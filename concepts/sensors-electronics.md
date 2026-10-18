---
title: 센서 전자공학 (Sensor Electronics)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# 센서 전자공학 (Sensor Electronics)

## 정의
**물리량→전자 신호 변환** 소자 및 회로. 정밀도·정확도·분해능(6.1)의 기초 개념과 함께, 온도·근접성·운동·힘·압력 센서의 작동 원리와 활용을 다룸 (6장).

## 센서 유형
- **온도** — 서미스터(NTC/PTC), 열전대(Seebeck), RTD, 적외선 온도계
- **근접성/접촉** — 초음파 거리, 광학 거리(ToF), 용량성 센서(capacitive touch)
- **운동** — 수동적외선(PIR), 가속도(a accelerometer), 회전(rotation), 유량(flow)
- **힘·압력** — 힘(force), 기울기(tilt), 진동/충돌(vibration/impact), 압력(pressure)

## 센서 특성 (6.1)
- **정밀도(precison)** — 반복 시 산포
- **정확도(accuracy)** — 참값과의 차이
- **분해능(resolution)** — 최소 감지 단위
- **관찰자 효과** — 측정 자체가 회로에 영향 (임피던스 정합, 부하)
- **보정(calibration)** — 편차 제거, 기준점 교정

> `raw/books/practical-electronics-eng.md` pp. 518-540

## Related
- [[analog-filter-design]] — 센서 신호의 노이즈 필터링
- [[microcontroller-arduino]] — 아두이노 아날로그 입력으로 센서 읽기
