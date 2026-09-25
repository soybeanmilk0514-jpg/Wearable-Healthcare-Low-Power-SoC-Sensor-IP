# 05. Company Technology Comparison

제출 보고서는 삼성전자, 애플, 퀄컴의 wearable SoC 접근을 서로 다른 low-power design strategy 사례로 비교했다.

## Samsung — Exynos W1000

프로젝트에서 강조한 요소:

- 3 nm GAA process
- stronger electrostatic gate control
- leakage reduction
- FOPLP / ePoP packaging
- shorter interconnect path and thermal / area benefit

## Apple — S10 SiP

프로젝트에서 강조한 요소:

- custom System in Package
- hardware–software co-optimization
- Always-On Processor
- main CPU power gating
- minimizing energy for continuously active functions

## Qualcomm — Wearable Platform

프로젝트에서 강조한 요소:

- heterogeneous high-performance / low-power cores
- always-on coprocessor
- workload-based processing
- on-device AI / NPU use
- reduced dependence on continuous wireless data transfer

## Interpretation

세 사례는 low-power optimization의 출발점이 서로 다르다는 것을 보여주는 비교 틀로 사용했다.

- Samsung: process / transistor / packaging
- Apple: vertical system optimization
- Qualcomm: workload partitioning / accelerator architecture

## Evidence Scope

이 문서는 제출 보고서의 2026년 작성 시점 비교를 재구성한 것이다.

최신 제품 specification을 실시간 검증한 페이지가 아니므로, 향후 제품 세대가 바뀌더라도 당시 프로젝트의 분석 기록으로 유지한다.
