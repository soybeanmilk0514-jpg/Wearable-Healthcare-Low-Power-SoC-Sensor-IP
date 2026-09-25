# 02. SoC Architecture for Wearable Healthcare

## Why SoC?

보고서는 wearable 내부의 주요 semiconductor blocks를 다음과 같이 정리한다.

- AP / MCU: 연산 및 operating system
- Sensor / AFE: analog biosignal acquisition
- PMIC: battery power distribution
- RF: wireless communication

개별 chip을 board 위에서 연결하면 interconnect 길이와 parasitic R/C가 커질 수 있다.

SoC integration은 여러 기능을 단일 die 안에 집적함으로써:

- physical wiring length 감소
- signal-transfer energy 감소
- area efficiency 향상
- external connector dependency 감소
- selective block power control 가능

이라는 장점을 제공한다고 분석했다.

## Power / Clock Gating

웨어러블은 항상 최대 성능을 요구하지 않는다.

대기 상태에서는 main processor를 끄고 센서 감시 logic만 활성화하는 방식으로 unnecessary switching and standby activity를 줄일 수 있다.

## Key System Insight

웨어러블의 문제는 “빠른 processor”를 만드는 것만이 아니다.

**필요한 block만 필요한 순간에 동작하게 하는 system architecture**가 battery lifetime을 결정하는 중요한 축으로 정리됐다.
