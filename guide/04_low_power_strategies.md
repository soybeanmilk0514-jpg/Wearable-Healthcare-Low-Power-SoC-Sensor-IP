# 04. Low-Power Implementation Strategies

프로젝트는 센서 IP와 SoC의 저전력 전략을 세 개 층으로 정리했다.

## 1. Leakage Suppression

### LDD / Junction Engineering

Short-channel scaling에서는 drain-side electric field와 leakage가 문제가 될 수 있다.

보고서는 LDD impurity profile을:

- implantation dose
- implantation energy
- annealing condition

등으로 최적화해 junction electric field와 leakage를 제어하는 방향을 언급한다.

### High-k Gate Dielectric

SiO₂를 매우 얇게 만들면 direct tunneling leakage가 증가할 수 있다.

HfO₂-based High-k dielectric은 작은 EOT를 유지하면서 더 두꺼운 physical dielectric thickness를 허용해 gate leakage 감소에 유리한 접근으로 정리했다.

## 2. Voltage Scaling / Weak-Inversion Operation

Dynamic power:

`P_dynamic ∝ C × V² × f`

따라서 supply voltage reduction은 매우 큰 power-saving lever가 될 수 있다.

프로젝트에서는 일부 low-power logic / analog blocks를 threshold 근처 또는 weak-inversion 영역에서 동작시키는 concept을 조사했다.

## 3. Duty Cycling / Smart Wake-up

Always-on sensor system에서 가장 중요한 것은 전체 SoC를 항상 켜두지 않는 것이다.

- sensor-side minimum logic remains active
- main processor remains in deep sleep
- meaningful event triggers an interrupt
- processing begins only when necessary

이 event-driven architecture는 clock-switching and standby waste를 줄이는 핵심 전략으로 제시됐다.
