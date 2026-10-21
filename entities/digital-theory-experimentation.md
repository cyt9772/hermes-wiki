---
title: Digital Theory and Experimentation Using Integrated Circuits (Levine, 2판)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, electrical-engineering, digital-electronics, electronic-circuits]
sources: [raw/books/digital-theory-experimentation.md]
confidence: high
---
# Digital Theory and Experimentation Using ICs (Morris E. Levine)

> 저자: Morris E. Levine (College of Staten Island, City University of New York), Revised and Enlarged (2판)
> 297p — 실험실 중심 디지털 전자학 교재. TTL·연산증폭기·CMOS 3 제품군으로 실험 수행

## 개요
**"실험 1개 = 이론 1차" 구조의 디지털 전자학 실험 교재**. 20개 실험을 통해 논리 게이트·부울대수·플립플롭·카운터·시프트 레지스터·슈머트 트리거·IC 타이머(74122/74121/555)·인코더/디코더·RAM·연산증폭기·D/A·A/D·CMOS-TTL 인터페이스를 다룬다. 모든 IC는 DIP 14핀/16핀. `^[raw/books/digital-theory-experimentation.md]`

## 실험 구조 (20개 실험 + 부록)
1. **Basic Logic Functions** (AND·OR·NAND·NOR—2판에 AND-OR-INVERT 게이트 추가)
2. **Boolean Algebra & Simplification of Logic Equations**
3. **De Morgan's Theorem**
4. **TTL NAND/NOR Gates — Definitions and Operation** (전달 특성 측정, 부하 오실레이션 주의, 7413/7414 슈머트 트리거로 펄스 정리)
5. **Exclusive-OR and its Applications**
6. **Full-Adder and Full-Subtractor** (2판: 4비트 MSI 74183 도입, LED로 논리 레벨 표시)
7. **Bistable or Flip-Flop (FF)** (R-S·D·T, 7473 등)
8. **Binary Counters and the Binary Number System** (리플 카운터, CRO로 bistable 동작 관찰)
9. **Divide-by-N Counters and Decade Counters**
10. **Shift Registers and Ring Counters** (2판: 5비트 MSI 시프트 레지스터, LED)
11. **Pulse Forming and Shaping; the Schmitt Trigger** (2판: 이전 1판의 2개 실험 통합)
12. **IC Timers — 74122, 74121, and 555** (2판 신설)
13. **Decoding and Encoding** (2판: 7-segment LED 디스플레이 추가)
14. **RAM / Scratch-Pad Memories** (2판: 16→64비트 LSI 메모리, 코드 변환)
15. **The Operational Amplifier** (기초 특성: 이득·주파수 응답)
16. **D/A and A/D Conversion** (연산증폭기를 매개로)
17. **CMOS — Principles and Characteristics** (2판 신설: 노이즈 면역, 고주파 소산)
18. **CMOS — TTL Interface** (2판 신설)

## 실험 포맷 (서문 명시)
- **E** — Experimental laboratory data (측정 데이터 표)
- **R** — Required results (데이터 → 논리 레벨로 해석)
- **D** — Discussion questions (측정값과 디지털 이론을 통합하는 질의응답)

## 부록 (Appendix)
- A: CRO 보정 + 전원 전압 확인 (IC 과전압 방지)
- B: 로직 기호
- C: Unit Load 개념
- D: IC 로직 회로도 + 핀 접속도 (상단 투시)
- G: 실험실 IC 소켓 + 스위치 뱅크 제작 상세 (알루미늄 채널, 바나나 플러그)
- 기타: Astable Multivibrator, FF, One-Shot/슈머트 트리거, 믹서/변조기/복조기, PLL(565), SCR

## 핵심 기여 / 학습 포인트
- **"기본 게이트 구축 → MSI IC로 교체"** 진행 순서: 논리 원리를 먼저 이해한 뒤 MSI/LSI 추세 체험. 배선도 동시에 단순화
- **TTL → 연산증폭기 → CMOS 3 제품군 실험 경험** — 한 실험 수반에서 제품군 간 차이(노이즈 면역, TTL-CMOS 인터페이스)를 체득
- **DIP 14/16핀 표준** — 1970~80년대 대학 실험실 표준 IC 패키지
- **74122·74121·555 IC 타이머 비교** (12장, 2판 신설)

## OCR 신뢰도
- PDF 내장 텍스트 레이어(pdftotext -layout, OCR 불필요). 서문·TOC·부록 라틴자 일부 깨짐('dk'des'=diode, 'FT'=fT, '2200-a'=2200-Ω, '565'=NE565 PLL) — 수치·회로 수치 해석 시 원본 PDF 대조 권장
- 실험 데이터 표(E/R/D 표) 구조는 양호

## Related
- 저자: [[morris-levine]]
- 개념: [[digital-logic-basics]], [[amplifiers-analog-circuits]], [[timer-oscillator-circuits]], [[fpga-hdl]]
- 관계서: [[digital-electronics]] (같은 주제 이론 교재)
