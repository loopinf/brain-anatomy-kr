---
id: insulin
kind: molecule
kr: 인슐린
en: Insulin
class: peptide hormone
source: 췌장 β세포
direction: anorexigenic
timing: long-term
tags: [feeding, satiety, glucose, energy-balance]
see_also:
  - arc
  - vmh
  - leptin
  - hypothalamic-feeding
---

# 인슐린 · Insulin

## 한 줄 요약

췌장이 혈당에 반응해 분비하는 호르몬. 전신 대사 조절(혈당 ↓)이 본업이지만,
뇌에서는 **장기적 포만 신호**로도 작용한다.

## 도식

{% include diagrams/mol-insulin.html %}


## 어디서 오나

- **췌장 랑게르한스섬의 β세포** 에서 분비.
- 자극: 식후 혈당 ↑. 또한 체지방이 늘면 baseline 인슐린도 ↑ (인슐린 저항성에서).

## 섭식 회로에서의 역할

- [ARC](../nuclei/arc.md)에 인슐린 수용체. [렙틴](leptin.md)과 비슷한 패턴으로 작동:
  - **POMC/CART 뉴런 활성** (포만 ↑)
  - **AgRP/NPY 뉴런 억제** (배고픔 ↓)
- 즉 인슐린은 췌장에서는 혈당을 떨어뜨리고, 뇌에서는 식욕을 떨어뜨린다 —
  같은 호르몬이 전신과 중추에서 협력하는 좋은 예.

## 본업 (참고)

- 혈당이 오르면 분비 → 근육·지방세포가 포도당을 받아들이게 함 → 혈당 ↓.
- 간에서 포도당 신생성 억제, 글리코겐 합성 촉진.
- 지방 합성 촉진.

## 길항 짝

- 섭식 회로에서: [그렐린](ghrelin.md).
- 혈당 회로에서는 글루카곤이 짝.

## 임상

- 1형 당뇨: β세포 자가면역 파괴 → 인슐린 결핍.
- 2형 당뇨: 인슐린 저항성 + 분비 저하. 비만에서 흔히 동반.
- 뇌의 인슐린 저항성은 식욕 조절 둔화에도 기여 — 비만이 비만을 강화하는 한 고리.

> 💡 **두 일을 동시에.** 혈당을 내리는 것이 본업이지만, 뇌에 "에너지가 충분하다"고
> 알리는 보조 일도 한다. 장기 신호인 [렙틴](leptin.md)과 한 팀.

## 같이 보는 항목

- 표적 핵: [ARC](../nuclei/arc.md), [VMH](../nuclei/vmh.md)
- 같이 작동 (장기 anorexigenic): [leptin](leptin.md)
- 길항 짝: [ghrelin](ghrelin.md)
- 회로: [hypothalamic-feeding](../circuits/hypothalamic-feeding.md)
