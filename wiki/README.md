# Brain anatomy wiki

이 폴더는 이 프로젝트의 **1차 진실(canonical source)** 입니다.
`data.json`, `data/*.json`, 각 HTML의 인라인 `DATA` 배열은 모두 여기서
파생되는 산출물(derived)이고, 향후 빌드 스크립트로 자동 동기화됩니다.

> **변경은 언제나 wiki에서만.** 파생 파일을 손으로 고치면 다음 빌드 때 덮입니다.

스타일은 Karpathy 식 LLM-friendly markdown wiki — **사람이 읽기 좋고**
**LLM이 한 페이지만 읽어도 맥락이 잡히는** 산문 위주. 스키마 단편 모음이
아니라 미니 위키로 운영합니다.

## 디렉토리

| 폴더 | 담는 것 |
|---|---|
| `regions/` | 15개 핵심 부위. 부위마다 메인 페이지. deep-dive는 동명 하위 폴더 |
| `nuclei/` | 핵(VMH, LH, ARC, PVN ...) 단위 |
| `molecules/` | 호르몬·신경전달물질 (ghrelin, leptin, dopamine ...) |
| `morphemes/` | 어근·접두사 (hypo, ventral, dorsal, lateral, arcuate ...) |
| `circuits/` | 회로 단위 (hypothalamic-feeding, fear-circuit ...) |

## 파일 = 한 개념

- 파일명은 **kebab-case**, frontmatter의 `id`와 **반드시 일치**.
  - `nuclei/vmh.md` → `id: vmh`
  - `morphemes/hypo.md` → `id: hypo`
- 한 파일은 한 가지를 다룬다. 길어지면 분리:
  - `regions/hypothalamus.md` (메인) → `regions/hypothalamus/feeding-circuit.md` (deep-dive)

## Frontmatter

YAML frontmatter 필수. 공통 필드:

```yaml
---
id: vmh
kind: nucleus            # region | nucleus | molecule | morpheme | circuit
kr: 복내측 시상하부
en: Ventromedial Hypothalamus
hanja: 腹內側 視床下部     # 해당될 때만
abbr: VMH                # 약어 있으면
parent: hypothalamus     # 상위 개념의 id (해당될 때만)
tags: [feeding, satiety] # cross-cutting 태그 (자유 어휘, 가능한 재사용)
see_also: [lh, arc, leptin]
---
```

`kind`별 추가 필드:

- `region`: `view: lateral | sagittal | both`, `category` (대뇌피질 4엽 / 변연계 / ...)
- `morpheme`: `origin` (Greek / Latin / 한자), `meaning_kr`, `meaning_en`
- `molecule`: `class` (peptide hormone / monoamine / ...), `source`, `direction` (orexigenic / anorexigenic / ...)

## 본문 컨벤션

- **한국어 우선**. 영어 용어와 한자는 첫 등장 시 병기.
  > 활꼴핵(arcuate nucleus, ARC)은 ...
- 표준 섹션 (해당하는 것만, 이 순서):
  - `## 한 줄 요약`
  - `## 위치` (region/nucleus용)
  - `## 기능`
  - `## 임상` (lesion/pathology가 있을 때)
  - `## 어원·형태소`
  - `## Deep-dive` (하위 페이지 링크)
  - `## 같이 보는 항목`
- mnemonic은 인용 callout으로:
  ```markdown
  > 💡 '이마 = 생각'
  ```

## 위키링크

- 다른 페이지 참조는 `[[id]]`. 표시 라벨 바꾸려면 `[[id|보일 글자]]`.
  - `[[vmh]]`, `[[leptin]]`
  - `[[hypo|hypo-]]`, `[[ventral|ventro-]]`
- frontmatter의 `parent`, `see_also`, `tags`는 빌드 때 자동 backlink로
  역참조됩니다. 본문에서 일일이 안 적어도, 예컨대 `morphemes/hypo.md` 하단에
  hypo를 쓴 모든 용어가 자동으로 모입니다.
- **깨진 링크는 정상.** 아직 안 만든 페이지로 가는 `[[]]`는 곧 만들어야 한다는
  TODO 신호로 운영합니다.

## 작성 흐름

1. 새 개념 → 어느 폴더에 들어갈지 결정 (region / nucleus / molecule / morpheme / circuit).
2. `id`를 정하고 같은 이름의 .md 생성.
3. frontmatter → 산문 본문 → `## 같이 보는 항목` 순서.
4. 다른 페이지에서 새 개념을 언급하면 `[[id]]`로 링크.

## 아직 없는 것 (의도적으로 미룸)

- 빌드 스크립트 (`wiki/` → `data.json` / HTML DATA 동기화).
- frontmatter 검증 (`kind`별 필수 필드 체크).
- SRS 카드 추출기 (각 .md에서 카드 후보를 뽑는 룰).

이것들은 페이지가 어느 정도 쌓인 뒤 한 번에 짭니다. 그 전까지 `data.json`과
`data/*.json`이 wiki와 잠시 병행하지만, **수정은 wiki에서만**.
