---
title: 타이머·발진기 회로 (Timer & Oscillator Circuits)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# 타이머·발진기 회로 (Timer & Oscillator Circuits)

## 정의
**시간(시간 간격) 생성(타이머)** 또는 **정현파/사각파 발진(발진기)** 전자 회로. 펄스 제어, 시계, 주파수 생성에 필수.

## RC 완화 발진기 (RC Relaxation) — 10.1
- 커패시터 충전/방전 주기 → 사각파
- 기본: R·C = 시간상수
- 응용: 부트스트랩, 스윙 제어

## 555 타이머 IC — 10.2
- **비안정(Astable)** — 10.2.1 (사각파 발진, 100Hz~100kHz)
- **단안정(Monostable)** — 10.2.2 (펄스 타이머)
- 작동 원리: 2개의 비교기 + 플립플롭 + 방전 트랜지스터
- 응용: 버저, 신호 발생기, 펌프 제어
- 주의: 전원 전압 정격, 출전 전류 한계

## VCO (Voltage-Controlled Oscillator) — 10.3
- 전압 입력 → 주파수 출력
- 응용: FM 변조(무선, 최신이동통신 제3장), 주파수 합성기

## 빈 브리지 / 트윈 T 발진기 — 10.4
- 고-선택적(고 Q) 정현파 발진
- 응용: RF 신호, 주파수 표준

## LC 발진기 (정현파) — 10.5
- 커패시터 + 인덕터 공진
- Hartley, Colpitts, Clapp 회로
- 응용: RF 발신, 주파수 표준

## 결정(Crystal) 발진기 — 10.6
- 쿼츠 결정 기계적 공진 → 전자기 신호
- 특성: **고-정밀·고-안정** (ppm 레벨), 1~100MHz
- 응용: 시계, 통신 발신기, MCU 클럭(13장)

## MCU 발진기 — 10.7
- 마이크로컨트롤러 내부 발진기 (internal oscillator)
- 8MHz/16MHz/20000MHz (13장 MCU 기본 구조)

> `raw/books/practical-electronics-eng.md` pp. 685-702

## Related
- [[analog-filter-design]] — 발진 주파수 정밀도
- [[power-supply-regulation]] — VCO 주파수 합성
- [[microcontroller-arduino]] — MCU 내부 발진기
