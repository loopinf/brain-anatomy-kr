---
id: reward-circuit
kind: circuit
kr: 보상·중독 회로
en: Reward & Addiction Circuit
tags: [reward, addiction, dopamine, motivation, learning]
see_also:
  - vta
  - nac
  - dopamine
  - amygdala
  - hippocampus
  - acetylcholine
  - endorphin
  - gaba
  - fear-circuit
  - trisynaptic-circuit
---

# 보상·중독 회로 · Reward & Addiction Circuit

## 한 줄 요약

[VTA](../nuclei/vta.md)의 도파민 뉴런이 [측좌핵(NAc)](../nuclei/nac.md)·전전두엽으로
**"이건 좋다, 또 하자"** 신호를 뿌리는 회로. 자연 보상(음식·섹스·사회적 인정)과
모든 중독성 약물의 **공통 종착지**가 이 회로의 같은 시냅스. 도파민 burst가
"기대보다 좋았다"는 보상 예측 오차(RPE)를 부호화한다.

## 회로 도식

{% include diagrams/reward-circuit.html %}

## 두 큰 갈래 (mesolimbic / mesocortical)

| 경로 | 출발 | 도착 | 역할 |
|---|---|---|---|
| **중뇌변연(mesolimbic)** | [VTA](../nuclei/vta.md) | [NAc](../nuclei/nac.md), 편도체, 해마 | "wanting", 동기, 중독의 핵심 |
| **중뇌피질(mesocortical)** | [VTA](../nuclei/vta.md) | 전전두엽 (특히 mPFC) | 인지 평가, 작업기억, 실행 통제 |

같은 [VTA](../nuclei/vta.md) 핵의 다른 갈래라 약물·자극이 두 경로를 동시에 켠다.
이 둘의 균형이 깨지는 게 중독·조현병·ADHD의 공통점.

## 보상 예측 오차 (Reward Prediction Error, RPE)

[VTA](../nuclei/vta.md) 도파민 뉴런의 phasic burst는 **"받은 보상 - 기대했던 보상"**.
Wolfram Schultz의 고전 발견 (1990s):

- 기대 안 한 보상 → DA burst ↑↑ (긍정 RPE).
- 예측한 보상이 와도 → DA 변화 없음 (RPE = 0).
- 기대했는데 안 옴 → DA dip (부정 RPE).

같은 패턴이 **TD-learning**(temporal difference, Sutton 1988)이라는 강화학습
알고리즘과 일치. 2010년대에 "도파민 = 강화학습 신호"가 거의 확정 — 컴퓨터과학과
신경과학이 만난 지점.

## "Wanting" vs "Liking" — 분리된 두 시스템

같은 보상 안에 두 다른 신경 신호:

- **Wanting (원함, 동기)**: [NAc](../nuclei/nac.md)의 DA 신호. 도파민 차단 시 동물은 음식을 원하지 않음 (학습된 행동도 안 함).
- **Liking (좋아함, 쾌락)**: [NAc](../nuclei/nac.md) shell의 작은 점들 (hedonic hotspots) — μ 아편 수용체·내인성 칸나비노이드 의존. DA와 분리.

이 분리가 중독의 역설을 설명: **갈망은 점점 강해지는데, 실제 만족은 줄어드는** 패턴 —
wanting의 가소성이 liking의 가소성을 앞지른 결과.

## 모든 중독의 공통 회로

서로 다른 약물이지만 공통점은 **VTA → NAc DA burst를 만든다**는 것:

| 약물 | 메커니즘 (어떻게 DA burst 만드나) |
|---|---|
| 코카인·암페타민·메스 | DAT(도파민 수송체) 차단·역수송 |
| 헤로인·모르핀·펜타닐 | VTA GABA 억제 뉴런 누름 → 탈억제 |
| 니코틴 | VTA DA 뉴런의 nAChR 직접 자극 |
| 알코올 | 다중 (GABA·NMDA·아편·DA 시스템 동시) |
| 대마(THC) | CB1 통한 VTA 활성·NAc 가소성 |
| 자연 보상 (음식·섹스·게임) | 학습된 단서가 VTA를 켬 |

각 약물이 DA burst를 만드는 강도·속도가 다르고, 그게 중독성의 차이를 만든다.

## 중독의 회로 변화

반복 사용으로 회로가 변형:

1. **민감화(sensitization)**: 같은 약물에 NAc DA 반응이 더 강해짐 (wanting 폭증).
2. **내성(tolerance)**: 시냅스 후 응답이 둔해짐 (liking 감소).
3. **의존(dependence)**: 중단 시 도파민 baseline이 정상 이하로 떨어져 anhedonia·금단증상.
4. **갈망(craving)**: 약물 단서가 [편도체·해마](../regions/amygdala.md)를 거쳐 NAc DA를 강하게 켬 → 강박적 추구.
5. **전두엽 통제 약화**: 전전두엽의 NAc 억제가 약해져 충동 조절 부전.

## 임상

- **중독 치료**:
  - **Naltrexone** (μ 차단): 알코올·아편 의존. 보상 신호 약화.
  - **Methadone, buprenorphine**: μ 작용제·부분작용제. 안정적 톤 유지로 갈망·금단 줄임.
  - **Bupropion** (DA·NE 재흡수 차단): 금연·우울.
  - **Varenicline**: 부분 nAChR 작용제. 금연.
  - **DBS of NAc**: 치료 저항성 강박장애·우울 자극 표적.

- **DA 회로의 다른 질환**:
  - **조현병**: 중뇌변연 ↑ (양성증상) + 중뇌피질 ↓ (음성증상·인지). 항정신병약은 D2 차단으로 양성에 듣지만 음성엔 약함.
  - **파킨슨**: nigrostriatal DA 손실이 본질이지만, L-DOPA 부작용으로 NAc 회로 과활성 → 충동조절장애(병적 도박·과식·과성욕).
  - **ADHD**: 중뇌피질 DA 부족 가설. 메틸페니데이트가 DAT 차단으로 PFC DA ↑.

- **자연 보상의 재발견**:
  - **운동·사회적 연결·의미 있는 일**도 같은 회로를 켠다.
  - 만성 약물 사용으로 자연 보상에 대한 NAc 반응이 둔해진 상태에서 회복은 자연 보상 회로의 재활성화 — 행동 치료의 신경적 토대.

> 💡 **자연·인공 보상이 한 회로에서 만난다.** 음식과 코카인이 같은 시냅스에서
> 도파민 burst를 만든다. 차이는 강도와 학습 속도뿐.

## 같이 보는 항목

- 핵심 노드: [VTA](../nuclei/vta.md), [NAc](../nuclei/nac.md)
- 주연 분자: [dopamine](../molecules/dopamine.md)
- 입력: [amygdala](../regions/amygdala.md), [hippocampus](../regions/hippocampus.md), 전전두엽 (페이지 미작성)
- 약물 표적 분자: [endorphin](../molecules/endorphin.md), [acetylcholine](../molecules/acetylcholine.md), [GABA](../molecules/gaba.md)
- 짝 회로: [fear-circuit](fear-circuit.md), [trisynaptic-circuit](trisynaptic-circuit.md)
