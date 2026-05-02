---
id: trisynaptic-circuit
kind: circuit
kr: 해마 3시냅스 회로
en: Hippocampal Trisynaptic Circuit
parent: hippocampus
tags: [memory, ltp, plasticity, learning, consolidation]
see_also:
  - hippocampus
  - entorhinal
  - dg
  - ca3
  - ca1
  - glutamate
  - amygdala
  - fear-circuit
---

# 해마 3시냅스 회로 · Trisynaptic Circuit

## 한 줄 요약

[해마](../regions/hippocampus.md) 안에서 정보가 흐르는 **세 시냅스의 일방통행로**:
[EC](../nuclei/entorhinal.md) → [DG](../nuclei/dg.md) → [CA3](../nuclei/ca3.md) → [CA1](../nuclei/ca1.md).
짧지만 학습·기억의 거의 모든 분자 기전이 발견된 회로. **LTP**(장기 강화)의 무대.

## 회로 도식

{% include diagrams/trisynaptic-circuit.html %}

## 회로의 단계

```
신피질 ──┐
        ↓                     EC layer III
    [내후각피질] ─ perforant path ────┐
       (EC II)                       ↓
        │                          (CA1 가지돌기 끝)
        ↓ perforant path
   [DG dentate gyrus]
        │
        ↓ mossy fiber (이끼섬유)
   [CA3 cornu ammonis 3]
        │  ──── recurrent collateral (자기 자신으로)
        ↓ Schaffer collateral
   [CA1]
        │
        ↓ 분리부 → EC layer V → 신피질
```

각 단계의 역할:

| 단계 | 시냅스 | 기능 |
|---|---|---|
| 1 | [EC](../nuclei/entorhinal.md) → [DG](../nuclei/dg.md) (perforant) | **패턴 분리**: 비슷한 입력을 서로 다른 활성 패턴으로 |
| 2 | [DG](../nuclei/dg.md) → [CA3](../nuclei/ca3.md) (mossy fiber) | 강력한 단일 시냅스 — 새 정보 각인 |
| 3 | [CA3](../nuclei/ca3.md) → [CA1](../nuclei/ca1.md) (Schaffer) | **LTP**가 처음 측정된 시냅스. 회상된 패턴이 CA1으로 |

추가 갈래:
- **CA3 ↔ CA3 recurrent**: 패턴 완성. 자기연상 네트워크.
- **EC layer III → CA1 (temporoammonic)**: 현재 입력을 CA1으로 직접 → CA1이 "회상 vs 현재"를 비교.

## LTP — 학습의 분자 모형

CA3 → CA1 시냅스에서 1973년 Bliss & Lømo가 발견.

1. **Hebbian 동시성**: 시냅스 전 (CA3) 활성 + 시냅스 후 (CA1) 강한 탈분극이 같이 일어나야.
2. **NMDA 수용체 게이트**: NMDA가 시냅스 후 탈분극으로 Mg²⁺ 차단을 풀어야 Ca²⁺ 통과 → "동시성 검출기".
3. **Ca²⁺ → CaMKII → AMPA 수용체 추가**: 시냅스에 AMPA가 더 박힘 → 같은 자극에 더 강한 EPSP.
4. **장기적**: 단백질 합성·시냅스 모양 변화로 분~시간~일 단위 강화.

자세한 분자: [glutamate](../molecules/glutamate.md) 페이지.

> "Cells that fire together wire together" (Hebb 1949) — 이 원칙의 가장 직접적인
> 신경 회로 증명.

## 시스템 통합 (systems consolidation)

해마의 LTP는 분~시간~일 단위. 그러나 기억이 평생 유지되려면 결국 **신피질**이
저장해야 함. 변환 과정:

- 처음: 해마가 핵심 (해마 손상 시 새 기억 안 됨, [환자 H.M.](../regions/hippocampus.md)).
- 시간이 지나며: 수면(특히 NREM 동안 sharp-wave ripple) 중 해마가 같은 패턴을 반복 재생 → 신피질 시냅스가 강화됨.
- 결과: 오래된 기억은 해마 없이도 회상 가능. 최근 기억은 해마 의존.
- 이게 "역행성 기억상실의 시간 기울기(Ribot's law)"의 신경적 토대.

## [편도체](../regions/amygdala.md)와의 협업 — 감정·맥락 기억

- 단서 공포(소리·빛)는 [편도체](../regions/amygdala.md)만으로 학습.
- **장소·맥락 공포**("이 방이 무섭다")는 해마가 맥락 표상을 BLA에 보낼 때 학습. → [fear-circuit](fear-circuit.md).
- 강한 감정 사건의 기억이 또렷한 이유: NE([청반](../nuclei/locus-coeruleus.md)에서) + 코르티솔이 해마의 LTP를 강화.

## 임상

- **알츠하이머**: 회로의 입구([EC](../nuclei/entorhinal.md))부터 위축 → 회로 입력 자체가 줄어듦.
- **저산소성 기억상실**: [CA1](../nuclei/ca1.md)이 가장 취약 → 회로의 출력 단계가 끊김.
- **외상후 기억상실 / 환자 H.M.**: 회로 전체가 양측 다 손상되면 새 기억 형성 자체가 불가.
- **간질**: 해마 경화증(특히 CA1 손실)이 측두엽 간질의 흔한 병리.
- **항우울제·운동·환경 풍부화**: [DG](../nuclei/dg.md) 신경발생을 늘려 회로 가소성 회복.

## 어원·역사

- **trisynaptic** = "세 시냅스" (Greek *tri-* + *synapsis*). 1934년 Lorente de Nó가 회로 구조를 정리, 1971년 Andersen이 "trisynaptic loop"로 명명.

> 💡 **세 시냅스 안에 학습·기억의 거의 모든 분자 메커니즘이 모여 있다.** 이 회로
> 하나로 LTP, 패턴 분리, 패턴 완성, 시스템 통합, 알츠하이머의 시작점이 모두 풀린다.

## 같이 보는 항목

- 중심 region: [hippocampus](../regions/hippocampus.md)
- 부소영역: [entorhinal](../nuclei/entorhinal.md), [DG](../nuclei/dg.md), [CA3](../nuclei/ca3.md), [CA1](../nuclei/ca1.md)
- 분자: [glutamate](../molecules/glutamate.md) (LTP의 주역)
- 짝 회로: [fear-circuit](fear-circuit.md) (편도체와 함께 맥락 공포)
