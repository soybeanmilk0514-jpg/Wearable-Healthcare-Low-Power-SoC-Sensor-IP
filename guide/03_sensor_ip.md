# 03. Sensor IP & Analog Front-End

## Why Sensor IP Matters

웨어러블의 최종 입력은 대부분 매우 작은 analog biosignal이다.

따라서 sensor IP는 단순한 센서 소자뿐 아니라:

- Analog Front-End (AFE)
- amplifier
- ADC
- buffer
- low-noise power block
- event / control logic

까지 포함하는 system block으로 다뤘다.

## PPG

PPG는 LED light와 photodiode를 이용해 혈류 변화와 산소포화도 관련 optical response를 측정한다.

핵심 회로:
- LED driver
- photodiode
- transimpedance amplifier
- low-noise readout

## ECG

ECG는 심장 활동전위를 피부 전극을 통해 측정한다.

핵심 요구:
- very high input impedance
- low-noise instrumentation amplifier
- common-mode-noise rejection

## BIA

BIA는 인체에 작은 AC current를 인가하고 voltage magnitude / phase response를 측정해 body composition과 관련된 complex impedance를 분석한다.

핵심 요구:
- multi-frequency excitation
- phase detection
- accurate analog front-end

## AFE / ADC

보고서는 AFE에 chopper stabilization, high CMRR / PSRR 같은 noise-suppression 개념을 연결했다.

ADC는 목적에 따라:

- SAR ADC: power-efficient moderate/high resolution
- Sigma-Delta ADC: precision biosignal acquisition

으로 구분했다.

## Architectural Point

센서가 계속 데이터를 생성한다고 해서 main SoC가 계속 깨어 있을 필요는 없다.

Local buffer와 interrupt logic을 이용해 biosignal acquisition과 high-power processing을 시간적으로 분리하는 것이 중요하다.
