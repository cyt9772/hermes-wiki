---
title: 전압 조정기·전원장치 (Voltage Regulator & Power Supply)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# 전압 조정기·전원장치 (Voltage Regulator & Power Supply)

## 정의
**입력 전압(AC/DC) → 원하는 출력 전압(안정 DC) 변환** 회로. 부하 변동·입력 변동에 대해 전압을 일정하게 유지.

## 고정식 조정기 (LDO) — 11.1
- **Linear Voltage Regulator** — 입력보다 낮은 단일 전압 출력
- 78xx(양전압) / 79xx(음전압) 시리즈
- 장점: 단순, 낮은 EMI
- 단점: 효율 저하(히트싱크 필요), ΔV = Vin − Vout

## 가변 조정기 (Variable) — 11.1
- 저항 디바이더로 출력 전압 설정
- LM317 등

## 변압기·정류기 — 11.3~11.4
- **변압기(Transformer)** — AC 전압 승격/강압, 전기적 분리
- **정류기(Rectifier)** — AC → DC, 단일반파/복합반파/브리지

## 스위칭 조정기 (스위처, Switching Regulator) — 11.8
- **Buck/Boost/Inverting** (DC-DC 컨버터)
- 작동: 스위치(MOSFET) 인덕터 커패시터
- 장점: 고효율(90%+), 넓은 입력 범위
- 단점: 스위칭 노이즈(EMI), 필터 필요

## SMPS (Switched-Mode Power Supply) — 11.9
- **플라이백·포워드·브리지** 토폴로지
- 응용: PC 전원, LED 드라이버, 충전기
- 효율: 85~95% 이상

## 산업용 패키지 — 11.10
- Brick, enclosed, board-mounted

> `raw/books/practical-electronics-eng.md` pp. 703-720

## Related
- [[timer-oscillator-circuits]] — VCO 주파수 합성기
- [[analog-filter-design]] — 스위칭 전원 EMI 필터링
