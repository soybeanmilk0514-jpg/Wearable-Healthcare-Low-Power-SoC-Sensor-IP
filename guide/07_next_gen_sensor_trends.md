# 07. Next-Generation Sensor IP Trends

프로젝트의 결론은 wearable 경쟁력이 점점 **front-end biosignal acquisition**으로 이동할 수 있다는 방향에 초점을 맞췄다.

## Ultra-Low-Power High-Precision AFE

차세대 wearable은:

- sweat chemistry
- optical biomarker
- continuous pressure / pulse
- complex electrical biosignal

등 더 약하고 복잡한 signal을 처리해야 한다.

이 때문에 sensor-side AFE는 낮은 전력과 높은 SNR을 동시에 요구한다.

## Intelligent Wake-up

모든 raw signal을 계속 digitize / transfer하면 energy cost가 커진다.

따라서 sensor-side threshold logic 또는 lightweight detection block이:

1. local signal monitoring
2. event recognition
3. hardware interrupt
4. main SoC wake-up

순서로 동작하는 event-driven architecture가 중요하다고 정리했다.

## Flexible / Chemical Sensor Expansion

PPG / ECG와 같은 기존 modality뿐 아니라:

- piezoelectric sensing
- sweat-ion sensing
- flexible strain / crack sensing

등으로 input modality가 확장되면서 sensor-material and AFE co-design의 중요성이 커질 것으로 분석했다.
