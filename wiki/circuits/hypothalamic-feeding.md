---
id: hypothalamic-feeding
kind: circuit
kr: 시상하부 섭식·포만 회로
en: Hypothalamic Feeding & Satiety Circuit
parent: hypothalamus
tags: [feeding, satiety, hunger, homeostasis, endocrine]
see_also:
  - hypothalamus
  - vmh
  - lh
  - arc
  - pvn
  - ghrelin
  - leptin
  - insulin
  - pyy
  - glp-1
  - cck
---

# 시상하부 섭식·포만 회로

배고픔과 포만은 뇌가 즉흥적으로 결정하는 게 아니다. [시상하부](../regions/hypothalamus.md)
안의 작은 핵 네 개가 위·장·췌장·지방세포에서 올라오는 호르몬을 받아, 길항하는
두 갈래로 신호를 처리한 뒤 행동(먹기/멈추기)과 자율신경·내분비 출력으로 보낸다.
이 페이지는 그 회로를 한 장으로 정리한다.

## 한 줄 요약

> **공복** → 그렐린 ↑ → ARC의 AgRP/NPY 활성 → LH 자극 → **식사**
> **식사 후** → 렙틴/인슐린/PYY ↑ → ARC의 POMC 활성 → VMH·PVN 활성 → **포만**

## 등장 인물

### 핵 (nuclei) — 시상하부 안의 네 개

| 핵 | 역할 | 한 줄 |
|---|---|---|
| [VMH](../nuclei/vmh.md) (복내측 시상하부) | **포만 중추** | "그만 먹어"의 출력 |
| [LH](../nuclei/lh.md) (외측 시상하부) | **섭식 중추** | "먹어라"의 출력 |
| [ARC](../nuclei/arc.md) (활꼴핵) | **혈중 호르몬 감지 허브** | 길항 뉴런 두 종이 모여 의사결정 |
| [PVN](../nuclei/pvn.md) (실방핵) | **통합 출력 허브** | ARC 신호를 자율·내분비로 내보냄 |

### 호르몬 — 어디서 오나

| 호르몬 | 분비 | 방향 | 타이밍 |
|---|---|---|---|
| [그렐린](../molecules/ghrelin.md) | 위 (공복) | orexigenic ↑ | 단기 |
| [렙틴](../molecules/leptin.md) | 지방세포 | anorexigenic ↓ | 장기 |
| [인슐린](../molecules/insulin.md) | 췌장 | anorexigenic ↓ | 장기 |
| [PYY](../molecules/pyy.md) | 장 (식후) | anorexigenic ↓ | 단기 |
| [GLP-1](../molecules/glp-1.md) | 장 (식후) | anorexigenic ↓ | 단기 |
| [CCK](../molecules/cck.md) | 장 (식후) | anorexigenic ↓ | 단기 |

## ARC가 핵심 허브인 이유

[ARC(활꼴핵)](../nuclei/arc.md)는 **혈뇌장벽(BBB)이 약한** 영역이라, 혈중 호르몬을
다른 뇌 영역과 달리 **직접** 감지할 수 있다. 그 안에 길항하는 두 뉴런 집단이 함께
산다:

- **AgRP/NPY 뉴런**: [그렐린](../molecules/ghrelin.md)에 반응 → 배고픔 촉진. [LH](../nuclei/lh.md)를 자극, [VMH](../nuclei/vmh.md)를 억제.
- **POMC/CART 뉴런**: [렙틴](../molecules/leptin.md)·[인슐린](../molecules/insulin.md)에 반응 → 포만감 촉진. [VMH](../nuclei/vmh.md)·[PVN](../nuclei/pvn.md)을 활성, AgRP/NPY를 억제.

서로의 활동을 억누르면서 동시에 작동하기 때문에, 결국 한쪽이 우세한 만큼 뇌가
"먹는 모드" 또는 "멈추는 모드"로 기운다.

## 흐름 1 — 공복 (먹게 만드는 회로)

1. 위가 비면 위벽에서 [그렐린](../molecules/ghrelin.md) 분비 ↑.
2. 그렐린이 혈류를 타고 [ARC](../nuclei/arc.md)에 도달, **AgRP/NPY 뉴런** 활성.
3. AgRP/NPY 뉴런이 [LH](../nuclei/lh.md)를 자극 → 오렉신(orexin) 뉴런 활성.
4. LH 출력 → 행동(음식 탐색·섭취), 동시에 [VMH](../nuclei/vmh.md) 억제.
5. 식사 시작.

## 흐름 2 — 식사 후 (멈추게 만드는 회로)

1. 음식이 장에 닿으면 단기 포만 호르몬([CCK](../molecules/cck.md), [GLP-1](../molecules/glp-1.md), [PYY](../molecules/pyy.md)) ↑.
2. 췌장에서 [인슐린](../molecules/insulin.md) ↑ (혈당 상승 반응). 지방 저장이 늘면 장기적으로 [렙틴](../molecules/leptin.md) ↑.
3. 이 신호들이 [ARC](../nuclei/arc.md)의 **POMC/CART 뉴런** 활성 + AgRP/NPY 억제.
4. POMC/CART → [VMH](../nuclei/vmh.md) 활성 → "그만 먹어" 신호. 동시에 [PVN](../nuclei/pvn.md)을 자극.
5. PVN이 자율신경·내분비로 출력 → 에너지 소비 ↑, 식욕 억제, 포만감 인지.

## 외워두면 두고두고 쓰이는 짝

- **위치 짝**: 안쪽([medial](../morphemes/medial.md))의 VMH ↔ 바깥쪽([lateral](../morphemes/lateral.md))의 LH.
- **호르몬 짝**: 단기 신호(CCK·GLP-1·PYY는 장에서, 그렐린은 위에서) ↔ 장기 신호(렙틴은 지방에서, 인슐린은 췌장에서).
- **방향 짝**: orexigenic(식욕 촉진, 그렐린만) ↔ anorexigenic(식욕 억제, 나머지 다섯).

## 임상

- [VMH](../nuclei/vmh.md) 손상 → 폭식·비만 (VMH syndrome).
- [LH](../nuclei/lh.md) 손상 → 식욕 상실·체중 감소.
- 렙틴 결핍/저항성 → 비만 (특히 ob/ob 마우스 모델, 사람의 일부 단일유전자 비만).
- GLP-1 작용제(예: semaglutide)는 이 회로의 anorexigenic 측을 직접 자극하는 비만·당뇨 치료제.

> 💡 **요점은 한 그림**: ARC가 가운데에서 호르몬을 감지하고, 두 뉴런 집단이
> 서로 밀고 당기며 LH(먹기) ↔ VMH/PVN(멈추기) 두 출력 중 하나를 우세하게 만든다.

## 같이 보는 항목

- 상위: [hypothalamus](../regions/hypothalamus.md)
- 핵: [VMH](../nuclei/vmh.md), [LH](../nuclei/lh.md), [ARC](../nuclei/arc.md), [PVN](../nuclei/pvn.md)
- 호르몬: [ghrelin](../molecules/ghrelin.md), [leptin](../molecules/leptin.md), [insulin](../molecules/insulin.md), [PYY](../molecules/pyy.md), [GLP-1](../molecules/glp-1.md), [CCK](../molecules/cck.md)
- 형태소: [ventral](../morphemes/ventral.md), [medial](../morphemes/medial.md), [lateral](../morphemes/lateral.md), [para](../morphemes/para.md), [arcuate](../morphemes/arcuate.md)
