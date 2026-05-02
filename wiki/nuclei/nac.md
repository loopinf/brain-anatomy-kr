---
id: nac
kind: nucleus
kr: 측좌핵
en: Nucleus Accumbens
hanja: 側坐核
abbr: NAc
parent: forebrain
tags: [reward, motivation, addiction, mesolimbic, basal-ganglia]
see_also:
  - vta
  - dopamine
  - reward-circuit
  - amygdala
  - hippocampus
---

# 측좌핵 · Nucleus Accumbens · NAc · 側坐核

## 한 줄 요약

기저핵의 **복측 선조체(ventral striatum)** 부분. [VTA](vta.md)에서 도파민을 받아
"이거 좋다, 또 하자"를 출력하는 **보상 회로의 중심 노드**. 모든 중독성 약물의
공통 종착지.

## 도식

{% include diagrams/nuc-nac.html %}


## 위치

- 전뇌(forebrain) 기저부, 선조체(caudate + putamen)의 가장 배쪽 부분.
- 두 부분으로 나뉨:
  - **NAc core**: 운동·행동 출력 측, 등쪽 선조체와 비슷한 역할.
  - **NAc shell**: 보상·동기·약물 효과의 핵심 측. 중독 연구의 주요 표적.
- 주뉴런: **GABA성 medium spiny neuron (MSN)** — D1·D2 도파민 수용체로 분리되는 두 종류.

## 기능

### 보상 회로 핵심 노드
- 입력:
  - **DA**: [VTA](vta.md)에서 (mesolimbic).
  - **글루타메이트**: [편도체(BLA)](../regions/amygdala.md) (감정 단서), [해마](../regions/hippocampus.md) (맥락), 전전두엽 (실행 통제).
- 출력: 복측 담창구 → 시상 → PFC → 운동 회로. 즉, "이 자극은 좋다 → 접근/반복하라" 신호를 운동 회로까지 보냄.

### "Wanting" vs "Liking"
- NAc 도파민 신호 = **wanting**(원함·동기). 도파민 차단·소실 시 동물은 음식을 원하지 않게 됨.
- **liking** (실제 쾌락) = 작은 hedonic hotspots(opioid·endocannabinoid 의존). NAc shell 안의 점들.
- 중독에서 갈망은 강한데 만족은 줄어드는 분리 — wanting/liking이 분자적으로 분리된 결과.

### 강화학습
- DA burst가 도착하면 NAc MSN의 시냅스 가소성이 일어나 "그 단서 → 그 행동"이 강화됨. 회로 위에서 일어나는 강화학습의 신경적 모형.

## 임상 — 모든 중독의 공통 표적

VTA → NAc DA burst를 일으키는 모든 약물:

| 약물 | 메커니즘 |
|---|---|
| 코카인·암페타민 | DAT 차단 / 역수송 → 시냅스 DA ↑ 직접 |
| 헤로인·모르핀 | VTA의 GABA 억제 뉴런을 μ로 누름 → 탈억제 → DA ↑ |
| 니코틴 | VTA DA 뉴런의 nAChR 직접 활성 |
| 알코올 | 다중 경로로 VTA → NAc DA ↑ |
| 대마(THC) | CB1 통한 시냅스 변화 |
| 도박·쇼핑·SNS | 자연 보상 신호로도 같은 회로 |

### 임상 응용
- **DBS of NAc**: 치료 저항성 강박장애·우울에서 시도되는 자극 표적.
- **Naltrexone**: μ 차단으로 알코올·아편 의존 치료 (보상 신호 약화).
- **Bupropion**: DA·NE 재흡수 차단 → 일부 보상 신호 회복으로 우울·금연에 효과.

## 어원

- *nucleus accumbens septi* = "중격(septum)에 기대어 있는 핵". *accumbere* (Latin '비스듬히 기대다').
- 한자 側坐核 = 옆에(側) 앉은(坐) 핵 — 같은 비유.

> 💡 **중독의 공통 종착지.** 화학적·자연적 모든 보상이 결국 여기서 갈망으로 변환됨.

## 같이 보는 항목

- 입력: [VTA](vta.md) (DA), [amygdala](../regions/amygdala.md), [hippocampus](../regions/hippocampus.md)
- 분자: [dopamine](../molecules/dopamine.md), [GABA](../molecules/gaba.md), [endorphin](../molecules/endorphin.md)
- 회로: [reward-circuit](../circuits/reward-circuit.md)
