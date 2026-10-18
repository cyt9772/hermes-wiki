---
title: 아날로그 필터 설계 (Analog Filter Design)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# 아날로그 필터 설계 (Analog Filter Design)

## 정의
**주파수 선택적 통과/차단** 회로. 신호의 원하지 않는 주파수 성분을 제거하거나 강조. 수동(RLC 소자)과 능동(연산 증폭기 + RLC) 두 방식.

## 수동 필터 (9장)
- **저역통과(Low-pass, LPF)** — 낮은 주파수 통과, 높은 주파수 차단
- **고역통과(High-pass, HPF)** — 높은 주파수 통과, 낮은 주파수 차단
- **대역통과(Band-pass, BPF)** — 특정 주파수 대역만 통과
- **노치(Notch/Rejection)** — 특정 주파수만 차단
- 설계: 커패시터·인덕터·저항 조합, 커텐 오프셋, Q-factor

## 능동 필터 (Active Filter)
- **저역통과 (Active LPF)** — 9.4
- **고역통과 (Active HPF)** — 9.5
- **대역통과 (Active BPF)** — 9.8
- **노치 (Active Notch)** — 9.9
- 장: 게인 제공(버퍼), 임피던스 정합, 소형화
- 단: 주파수 상한(연산 증폭기 대역폭), 전압 정격

## 통합 필터 IC (9.9)
- Switched-capacitor 필터 (SWITCH, 스위치드 커패시터)
- 프로그래머블 필터 IC
- 응용: 오디오 크로스오버(16장), RF 중계기, 센서 전처리

> `raw/books/practical-electronics-eng.md` pp. 663-686

## Related
- [[timer-oscillator-circuits]] — 발진 주파수 정밀도
- [[sensors-electronics]] — 센서 신호 필터링
