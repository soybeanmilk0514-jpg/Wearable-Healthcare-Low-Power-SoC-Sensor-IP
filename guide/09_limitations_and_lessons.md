# 09. Limitations & Lessons

## 1. No Original Silicon / Circuit Experiment

이 프로젝트는 technology-analysis project다.

다음은 수행하지 않았다.

- transistor fabrication
- wearable chip tape-out
- RTL implementation
- SPICE power simulation
- sensor measurement
- battery-life experiment

따라서 특정 기술의 직접적인 power-reduction percentage를 팀 자체 결과로 주장하지 않는다.

## 2. Company Comparison Is Time-Bounded

기업별 device / package / architecture 정보는 제출 보고서가 작성된 2026년 당시의 조사 내용을 구조화한 것이다.

실시간 product database가 아니다.

## 3. Layer Mixing Must Be Explicit

SoC, SiP, GAA, High-k, AFE, ADC, TIM은 서로 다른 abstraction level의 기술이다.

프로젝트의 핵심 학습점은 이들을 하나의 기술처럼 섞는 것이 아니라:

- product requirement
- system architecture
- circuit / IP
- device
- process
- materials
- package

로 계층을 구분한 뒤 서로의 연결관계를 이해하는 것이었다.

## 4. Stronger Career Relevance

반도체 개발 프로세스를 이해할 때 한 직무가 모든 기술을 담당하는 것은 아니다.

제품이 완성되려면 design, foundry, process, materials, packaging, sensor, system teams가 서로 다른 constraint를 주고받아야 한다.

이 프로젝트는 각 기술을 개별적으로 외우기보다 **cross-layer dependency**로 이해하는 연습이었다.
