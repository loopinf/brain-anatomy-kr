---
id: dopamine
kind: molecule
kr: 도파민
en: Dopamine
abbr: DA
class: monoamine (catecholamine)
source: 흑색질 (substantia nigra), VTA, 시상하부 활꼴핵
direction: motivation / reward / motor
timing: tonic + phasic (burst on prediction error)
tags: [monoamine, catecholamine, reward, motor, motivation, addiction]
see_also:
  - substantia-nigra
  - vta
  - norepinephrine
  - serotonin
  - acetylcholine
---

# 도파민 · Dopamine · DA

## 한 줄 요약

**보상·동기·운동**을 한 몸에 짊어진 모노아민. 두 큰 회로로 갈라져 일하는데 —
[흑색질](../nuclei/substantia-nigra.md)에서 기저핵으로 가는 운동 회로(파킨슨에서 손실)와,
[VTA](../nuclei/vta.md)에서 측좌핵·전전두엽으로 가는 보상 회로(중독·조현병의 무대)
— 이 둘이 별개의 시스템임이 핵심.

## 어디서 오나

세 가지 주요 도파민 시스템 (각각 다른 핵에서 출발):

| 경로 | 출발 | 도착 | 역할 |
|---|---|---|---|
| **흑질선조체(nigrostriatal)** | [흑색질 SNc](../nuclei/substantia-nigra.md) | 선조체(caudate, putamen) | 운동 시작·자세 |
| **중뇌변연(mesolimbic)** | [VTA](../nuclei/vta.md) | 측좌핵, 편도체, 해마 | 보상·동기·중독 |
| **중뇌피질(mesocortical)** | [VTA](../nuclei/vta.md) | 전전두엽 | 작업기억·인지·실행 |
| 결절누두(tuberoinfundibular) | 시상하부 활꼴핵 | 뇌하수체 전엽 | 프로락틴 분비 억제 |

합성 경로: 티로신 → DOPA → **도파민** → ([NE](norepinephrine.md) → [EPI](epinephrine.md)).
도파민이 카테콜아민의 출발점.

## 무엇을 하나

수용체 5종 (D1~D5), 두 패밀리:
- **D1-like (D1, D5)**: 시냅스 후 흥분.
- **D2-like (D2, D3, D4)**: 자가수용체 + 시냅스 후 억제. 항정신병약·파킨슨 약의 주표적.

핵심 개념:

### 보상 예측 오차 (reward prediction error, RPE)
도파민 phasic burst는 "받은 보상 - 기대했던 보상". Wolfram Schultz의 고전 발견.
- 기대보다 좋음 → DA ↑ (긍정 RPE)
- 기대대로 → DA 변화 없음
- 기대보다 나쁨 → DA ↓ (부정 RPE)

이게 강화학습의 신경적 등가물 — 학습 알고리즘이 도파민의 모양을 닮았다는 게
2010년대 결정적 발견.

### 동기 / "wanting" vs "liking"
도파민은 "원하는 것(wanting)"을 만들고, 실제 쾌락("liking")은 더 안쪽 작은
hedonic hotspots(opioid·endocannabinoid)이 만든다 — 중독에서 갈망은 강한데
실제 만족은 줄어드는 이유의 한 단서.

## 주요 약물 / 임상

- **파킨슨병**: SNc의 도파민 뉴런 사망 → 운동 시작 어려움. 치료: **levodopa**(BBB 통과 후 도파민으로 전환). 부작용: dyskinesia, 환각, 충동조절장애(병적 도박·과식).
- **항정신병약 (1세대 / 2세대)**: D2 길항제. 양성증상에 효과. 부작용으로 운동장애(EPS), 프로락틴 ↑.
- **자극제** (cocaine, amphetamine, methylphenidate): 도파민 재흡수 차단·역수송. ADHD 약(메틸페니데이트)부터 강한 중독성 약물까지.
- **아편(opioid)**: 직접 D 수용체에 작용하지 않지만, VTA의 GABA성 억제를 풀어 도파민 phasic burst를 만듦 → 보상 회로 활성.
- **모든 중독 약물의 공통점**: VTA → 측좌핵 도파민 burst를 만든다.
- **조현병**: 중뇌변연 DA ↑(양성증상) + 중뇌피질 DA ↓(음성증상)의 이중 가설.

## 어원

- *dopa* + *-mine* (아민) = "DOPA의 아민 형태". DOPA = dihydroxyphenylalanine, 합성 전 단계.

> 💡 **운동·보상·인지를 동시에 짊어진 분자.** 어느 회로에 손상이 났느냐로 파킨슨,
> 조현병, 중독, ADHD가 갈린다.

## 같이 보는 항목

- 만들어지는 곳: [흑색질](../nuclei/substantia-nigra.md), [VTA](../nuclei/vta.md)
- 친척 카테콜아민: [norepinephrine](norepinephrine.md), [epinephrine](epinephrine.md)
- 다른 모노아민: [serotonin](serotonin.md), [histamine](histamine.md)
- 길항 신경전달: [acetylcholine](acetylcholine.md) (선조체에서 DA와 음성 균형)
