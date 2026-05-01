---
id: fear-circuit
kind: circuit
kr: 공포 회로
en: Fear Circuit (Fear Conditioning & Defense)
parent: amygdala
tags: [fear, threat, conditioning, learning, defense, ptsd]
see_also:
  - amygdala
  - bla
  - cea
  - thalamus
  - pag
  - hypothalamus
  - locus-coeruleus
  - hippocampus
  - glutamate
  - gaba
  - norepinephrine
  - ascending-pain-pathway
---

# 공포 회로 · Fear Circuit

## 한 줄 요약

위협 단서가 [시상](../regions/thalamus.md)에 도착한 순간부터 동결·심박·각성이
폭발하기까지 모든 단계가 걸리는 시간은 **약 100밀리초**. 그 회로의 중심은
[편도체](../regions/amygdala.md) — [BLA](../nuclei/bla.md)가 학습하고
[CeA](../nuclei/cea.md)가 출력한다. 의식이 도착하기 전에 이미 몸이 반응한다.

## 두 길 — LeDoux의 high road / low road

같은 자극이 [편도체](../regions/amygdala.md)에 두 길로 도달:

| | low road (빠른 길) | high road (정밀한 길) |
|---|---|---|
| 경로 | 시상 → [BLA](../nuclei/bla.md) | 시상 → 감각피질 → [BLA](../nuclei/bla.md) |
| 속도 | ~12 ms | ~30~40 ms |
| 정보 정밀도 | 거침 ("막대기인지 뱀인지 모르지만 길고 가늘다") | 정밀 ("뱀 아니고 막대기") |
| 결과 | 일단 공포·동결 시작 | 필요 시 취소·교정 |

산길에서 막대기를 보고 깜짝 놀랐다가 곧 "막대기네" 하고 진정되는 경험은 두 길의
시간차를 직접 느끼는 것. 의식보다 빠른 첫 반응(low road)을 이미 시작한 뒤,
high road가 정정한다.

## 회로 단계 (감각 → 출력)

1. **감각 입력**: 청각·시각·촉각이 [시상](../regions/thalamus.md)으로.
2. **시상 → BLA (low road) + 시상 → 감각피질 → BLA (high road)**.
3. **[BLA](../nuclei/bla.md) 학습**: "이 자극이 위협과 짝지어진 적 있나?". 반복된 짝지음으로 [글루타메이트](../molecules/glutamate.md) 시냅스에서 LTP → 다음번엔 그 단서만으로도 강한 BLA 활성.
4. **[BLA](../nuclei/bla.md) → [CeA](../nuclei/cea.md)**: 위협 평가 신호 전달.
5. **[CeA](../nuclei/cea.md) 출력 분기**:
   - → [PAG](../nuclei/pag.md): **동결(freezing)** + 통증 둔화(stress-induced analgesia, [하행 통증 조절](descending-pain-modulation.md) 회로 활성).
   - → 외측 [시상하부](../regions/hypothalamus.md): 교감신경 → 심박·혈압·발한 ↑.
   - → 시상하부 PVN: HPA축 → 코르티솔 ↑.
   - → [청반(LC)](../nuclei/locus-coeruleus.md): NE 분비 → 각성·주의 ↑, 동공 확장.

## 공포 조건화 (fear conditioning) — 회로의 학습 측면

파블로프 패러다임의 공포 버전:

- **CS** (조건 자극): 중성 자극 (예: 청각 톤).
- **US** (무조건 자극): 혐오 자극 (전기 충격).
- 짝지음 후: CS만으로도 공포 반응(동결·심박 ↑) 출현.

회로상으로:
- US가 [BLA](../nuclei/bla.md) 뉴런을 강하게 흥분시키는 동안 CS 입력이 함께 도착 → CS 시냅스가 LTP로 강화 → 다음번엔 CS만으로도 BLA 활성.
- 이게 **"감정 기억"의 시냅스 모형**.

## 소거 (extinction) — 새 학습으로 덮기

- "CS만 반복해서 줘도 US가 안 따라옴"을 경험하면 공포가 약해짐.
- 이건 옛 기억을 *지우는* 게 아니라 **새 안전 기억을 학습**해 위에 덮는 것 — 인프랄림빅 전전두엽(infralimbic mPFC)이 [BLA](../nuclei/bla.md)를 억제.
- **노출치료(exposure therapy)**의 신경 회로 토대.
- 외상 단서가 다른 맥락에 다시 등장하면 종종 **공포가 재발(renewal)** — 소거가 맥락 의존적이라는 것은 [해마](../regions/hippocampus.md)와 BLA의 교차 연결이 만드는 결과.

## [해마](../regions/hippocampus.md)와의 협업 — 맥락 공포

- 단순한 단서 공포(소리, 빛)는 BLA만으로 학습되지만, **장소·맥락 공포**("이 방에 있으면 무섭다")는 [해마](../regions/hippocampus.md)가 맥락 표상을 만들어 BLA에 보낼 때 학습됨.
- 그래서 양측 해마 손상 환자는 단서 공포는 학습하지만 **맥락 공포는 못 학습**한다.

## 임상

- **PTSD**: 회로 전체가 위협 쪽으로 기울어 있음 — BLA 과활성, 전전두엽 통제 약화, [해마](../regions/hippocampus.md) 위축, 소거 학습 부전.
- **불안장애·공황**: BLA-CeA-PAG-LC 축의 만성 과활성.
- **노출치료**: 새 안전 학습(소거)을 회로에 넣는 행동 치료.
- **베타차단제(propranolol)**: NE의 BLA 작용 차단 → 외상 기억의 단단해짐 약화. 외상 직후 또는 재활성화 시점 투여 시도.
- **선택적 SSRI**: 만성적으로 회로 톤을 낮춤. 약효까지 4~6주 — 시냅스 재구성이 천천히 일어나서.
- **K. Bucy (Klüver-Bucy)**: 양측 편도체+측두엽 손상 → 공포·분노 소실 + 무차별 행동.
- **환자 S.M.** (양측 편도체 석회화): 외부 위협엔 무공포, 내부 위협(CO₂)엔 공포 → 회로의 분리 가능성.

> 💡 **의식보다 빠른 회로.** 뱀을 봤을 때 "뱀이다!"라는 생각이 들기 전에 이미 몸이
> 굳고 심장이 뛰는 이유. 회로가 의식을 기다리지 않는다.

## 같이 보는 항목

- 중심 region: [amygdala](../regions/amygdala.md)
- 핵: [BLA](../nuclei/bla.md), [CeA](../nuclei/cea.md)
- 입력: [thalamus](../regions/thalamus.md)
- 출력: [PAG](../nuclei/pag.md), [hypothalamus](../regions/hypothalamus.md), [locus-coeruleus](../nuclei/locus-coeruleus.md)
- 협업: [hippocampus](../regions/hippocampus.md) (맥락)
- 분자: [glutamate](../molecules/glutamate.md) (LTP), [GABA](../molecules/gaba.md), [norepinephrine](../molecules/norepinephrine.md)
- 짝 회로: [ascending-pain-pathway](ascending-pain-pathway.md), [descending-pain-modulation](descending-pain-modulation.md) (CeA가 PAG를 켜면 진통 회로도 같이 켜짐)
