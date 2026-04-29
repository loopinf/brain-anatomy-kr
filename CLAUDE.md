# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Static, dependency-free educational website teaching the 15 core brain regions in three languages simultaneously: English, Korean (한국어), and Hanja (한자어/漢字). UI strings, comments, and content are written in Korean — preserve that when editing.

No build step, no package manager, no tests, no linter. Just HTML files with inline `<style>` and `<script>`.

## Run locally

```bash
# Either open the files directly
open index.html
# or serve (needed if you want clean URLs / avoid file:// quirks)
python3 -m http.server 8080
```

Deployment is GitHub Pages from `main` branch root (no CI). Pushing to `main` publishes immediately.

## Architecture: content is duplicated across files (intentionally)

The site is four self-contained pages plus a script doc and a JSON file. Each HTML page **inlines its own copy** of the region dataset and SVG drawings — there is no shared module, no `fetch('data.json')` call. This is the single most important fact for editing this repo.

### Pages

| File | Role | What it embeds |
| --- | --- | --- |
| `index.html` | Landing / mode picker | Static parts list only |
| `drill.html` | Auto-advancing 1s/region drill, 3 cumulative rounds (KR → +EN → +漢字) | DATA[15] (id/en/kr/hanja/view) + LATERAL_SVG + SAGITTAL_SVG |
| `study.html` | 3 tabs: Learn (clickable SVG + info panel), Flashcard, 10-question Quiz | Full DATA[15] + both SVGs (with leader-line labels) |
| `shorts.html` | 9:16 vertical auto-player for screen recording into TikTok/Shorts/Reels | DATA[15] (with `desc` field instead of `function`/`location`/`etymology`) + both SVGs |
| `data.json` | Canonical reference dataset (8 fields per region) | **Not loaded by any page** — documentation only |
| `data/hypothalamus-feeding.json` | Deep-dive: hypothalamic feeding circuit (VMH/LH/ARC/PVN nuclei + hormones + fasting/satiety pathways). Includes per-term `morphemes[]` for future word-part drills. **Not yet wired to any UI.** | — |
| `script.md` | Korean narration scripts (5–8s per region) for shorts.html voiceover | — |

### The duplication you must respect

When you change region content (name, description, etc.) or SVG geometry, you typically need to update it in **multiple places**:

- Region textual fields → check each of `data.json`, `drill.html`, `study.html`, `shorts.html`, and `script.md`. Each file embeds a different subset of fields:
  - `drill.html`: `id, en, kr, hanja, view`
  - `study.html`: full set (`category, etymology, location, function, mnemonic, ...`)
  - `shorts.html`: uses a flattened `desc` + `mnemonic` (not the same wording as study.html)
  - `data.json`: the most complete record
- SVG paths/coordinates → `LATERAL_SVG` and `SAGITTAL_SVG` constants are duplicated verbatim in `drill.html`, `study.html`, and `shorts.html`. They share the same 800×520 viewBox and the same `data-id` attribute scheme.
- Region color palette (`.r-frontal { fill: ... }` ... `.r-pituitary`) is duplicated in all three HTML files. Keep colors consistent across pages.

There is no tooling that enforces this consistency — it's a manual responsibility. When the user asks to "fix the description of the hippocampus", check whether they mean one page or all of them.

### Region identity contract

Every region has a stable `id` (e.g. `frontal`, `corpus-callosum`, `pituitary`). That id is used three ways and they must agree:
1. As `data-id="..."` on the SVG path/ellipse.
2. As the CSS class suffix `.r-<id>` for the fill color.
3. As `id` field in the DATA arrays.

The `view` field (`"lateral"`, `"sagittal"`, or `"both"`) determines which SVG renders the region. `study.html` auto-switches the view when a region is clicked from a chip.

## Conventions

- Korean is the primary UI language. EN and Hanja appear alongside KR labels, not as a translation toggle.
- Fonts: rely on system stack (`-apple-system`, `Apple SD Gothic Neo`, `Noto Sans KR`). Don't add web font dependencies.
- Color accent across pages: `#2d4a7a` (navy) for primary, `#c94a4a` (red) for highlight/active state, `#faf8f3`/`#faf5ec` for warm backgrounds.
- Keep pages dependency-free — no frameworks, no bundlers, no npm. The repo `.gitignore` lists `node_modules/` defensively but there is no package.json.

## In-flight direction (not yet built)

The user's longer-term goal is to extend this from a flat 15-region site into a richer learning tool:
- **Spaced repetition (Anki-style)** review of facts derived from the data files.
- **Morpheme drills** — surfacing what `hypo-`, `ventro-`, `dorsal`, `arcuate`, etc. mean and reusing those across terms.
- **Region deep-dives** — sub-region/nucleus/hormone level detail (e.g. the hypothalamus feeding circuit), accumulated topic-by-topic.

Data is being added before UI. When extending: keep deep-dive datasets in `data/<region>-<topic>.json`, include `morphemes[]` arrays on terms that have learnable word parts, and don't yet retrofit pages — confirm with the user before wiring data into HTML, since the duplicated-DATA architecture means each integration touches multiple files.

### `wiki/` — markdown-first canonical layer (WIP, seeded)

Experiment in progress: a Karpathy-style LLM-friendly markdown wiki under `wiki/` is being seeded as the **canonical knowledge source**. See `wiki/README.md` for conventions (frontmatter schema, standard markdown links `[label](relative/path.md)` — **not** `[[wikilinks]]` since those don't render on GitHub web view or GitHub Pages, file = one concept). Currently only three pages exist as a tone/convention check (`wiki/README.md`, `wiki/regions/hypothalamus.md`, `wiki/nuclei/vmh.md`); the wiki is **not yet load-bearing** and `data.json` / `data/*.json` are still hand-maintained alongside it.

The intended end state: `data.json`, `data/*.json`, and the inline `DATA` arrays in each HTML page all become derived build artifacts generated from `wiki/`, eliminating the 4–5-place duplication described above. Until that build exists, do not split changes between wiki and the legacy data files — confirm with the user which is the source for any given edit.
