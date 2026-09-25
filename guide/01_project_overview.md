# 01. Project Overview

## Topic

웨어러블 헬스케어용 초저전력 SoC 및 센서 IP

## Problem

웨어러블 헬스케어 기기는 다음 요구를 동시에 만족해야 한다.

- 장시간 always-on operation
- 제한된 battery capacity
- 작은 form factor
- continuous biosignal acquisition
- 실시간 signal processing
- 높은 signal integrity와 reliability

프로젝트는 이러한 요구를 만족하기 위한 핵심 반도체 기술을 **system–circuit/IP–device–materials/process** 계층으로 나누어 분석했다.

## Development-Oriented View

단순 제품 비교가 아니라 다음 개발 흐름을 중심으로 정리했다.

```text
Wearable use case
    ↓
Power / area constraint
    ↓
SoC integration
    ↓
Sensor IP architecture
    ↓
Low-power device / circuit strategy
    ↓
Advanced process / packaging / materials
```

## Main Conclusion

웨어러블의 초저전력은 하나의 기술로 달성되지 않는다.

SoC 수준에서는 integration and power gating, sensor IP 수준에서는 low-noise / low-power acquisition, 소자 수준에서는 leakage suppression, 패키지·소재 수준에서는 thermal and mechanical reliability가 함께 맞물려야 한다.
