# Wearable Healthcare Low-Power SoC & Sensor IP

## Overview

웨어러블 헬스케어 기기의 제한된 battery / form factor 안에서 continuous biosignal sensing을 구현하기 위해, SoC integration, sensor IP, low-power device strategy, advanced process, packaging, and materials technology를 연결해 분석한 프로젝트입니다.

![Project flow](./figures/project-flow.svg)

## Architecture

```text
Sensor
  ↓
Analog Front-End
  ↓
ADC
  ↓
Local buffer / event logic
  ↓
Main SoC
```

The main SoC does not need to remain fully active. The project therefore emphasizes always-on sensor logic, power gating, and event-driven wake-up.

## Main Low-Power Levers

- LDD / junction-profile engineering
- HfO₂-based High-k gate dielectric
- supply-voltage scaling
- near-threshold / subthreshold operation
- power / clock gating
- event-driven smart wake-up
- GAA electrostatic control
- package-level thermal management

## Materials Connection

The project connects low-power SoC development to:

- High-k gate dielectric
- TIM / EMC thermal materials
- BN / graphene / CNT fillers
- PDMS / Parylene flexible materials

## Evidence Scope

This is a technology-analysis project rather than an original hardware implementation or measurement project.

See [Project Navigation](./guide/00_navigation.md) for the full documentation path.
