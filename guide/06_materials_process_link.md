# 06. Materials & Process Engineering Link

이 프로젝트의 중요한 특징은 wearable SoC의 저전력 문제를 회로 수준에서 끝내지 않고 **materials / device / packaging engineering**으로 연결했다는 점이다.

## High-k Gate Dielectric

Problem:
- scaling → thinner SiO₂
- direct tunneling leakage increase

Materials approach:
- HfO₂-based High-k dielectric
- physically thicker dielectric at comparable EOT
- lower tunneling probability

## Advanced Gate Structure

보고서는 wearable processor의 low-power process example로 GAA를 다뤘다.

GAA는 gate가 channel을 더 많이 둘러싸는 구조를 통해 scaled transistor에서 electrostatic control을 강화하는 방향으로 설명했다.

## Thermal Interface & Packaging Materials

High-density SiP에서는 thermal management도 power / reliability 문제와 연결된다.

보고서에서 다룬 재료:

- Thermal Interface Material (TIM)
- Epoxy Molding Compound (EMC)
- BN filler
- graphene
- carbon nanotube
- AlN-related thermal composite approach

핵심은 die에서 발생한 열을 외부로 효과적으로 전달하고, heterogeneous-material interface에서 thermal resistance를 줄이는 것이다.

## Flexible & Stretchable Materials

Wearable sensor는 rigid semiconductor와 soft skin 사이의 mechanical mismatch를 해결해야 한다.

프로젝트는:

- PDMS
- Parylene
- flexible electrode
- crack sensor concept

을 통해 mechanical conformity와 sensor signal integrity의 연결을 조사했다.

## Engineering Takeaway

초저전력 wearable은 설계만의 문제가 아니다.

**transistor material + device structure + package thermal path + human-interface material**이 모두 제품 수준 PPA와 reliability에 영향을 준다.
