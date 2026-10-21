---
title: 디지털 논리 기초 (Digital Logic Basics)
created: 2026-10-18
updated: 2026-10-22
type: concept
tags: [electrical-engineering, electronic-circuits, digital-electronics]
sources: [raw/books/practical-electronics-eng.md, raw/books/digital-electronics.md, raw/books/digital-theory-experimentation.md]
confidence: medium
---
# 디지털 논리 기초 (Digital Logic Basics)

## 정의
**이산 신호(2가치 로직)로 정보를 처리**하는 회로. 논리 게이트 → 조합 논리 → 순차 논리 → 저장장치로 진행.

## 디지털 논리 상태 (12.1)
- **High/Low** (1/0), 전압 레벨(5V TTL: 0.8V~2.0V uncertain zone)
- 숫자 코드: BCD, ASCII, Gray code
- 클럭 타이밍, 병렬→직렬(Parallel-to-Serial) 전환

## 논리 게이트 (12.2)
- **기본 8종** — AND, OR, NOT, NAND, NOR, XOR, XNOR, BUFFER
- **다중 입력 게이트** — 4-input AND, 4-input OR 등
- **디지털 논리 IC** — 74xx 시리즈(TTL), 40xx 시리즈(CMOS)
- **조합 논리 (Combinational)** — 출력 = 입력의 순간 함수
  - 멀티플렉서 (MUX) → 데이터 선택기
  - 디멀티플렉서 (DEMUX) → 데이터 분배기
  - 인코더 (Encoder) / 디코더 (Decoder)
  - 2진 가산기 (Binary Adder), 2진 가산/감산기
  - 비교기 (Comparator, magnitude comparator)

## 제품군 (12.4)
- **TTL (Transistor-Transistor Logic)** — 74xx, 전압 5V, 고속
- **CMOS (Complementary MOS)** — 40xx, 전압 3-15V, 저전력
- **HCT/ACT** — 혼합
- I/O 전압, 잡음 여유(noise margin), 전류 정격, 팬아웃, 전파 지연

## 순차 논리 (Sequential) — 12.6
- 상태 기억: **클럭(Clock)** 에 동기화
- **플립플롭 (Flip-flop)**
  - **SR** → S/R 저장
  - **D (Data)** → Q = D@ rising/falling edge
  - **JK** → TOGGLE 모드
  - **T (Toggle)** → CLK마다 반전
- **계수기 IC (Counter)**
  - 비동기(Ripple) — 클럭이 순차 전달
  - 동기 — 클럭이 동시에 전달
  - 시프트 레지스터 (Shift Register) — 직렬→병렬, 병렬→직렬, Johnson/Ring

## A/D·D/A 변환 (12.9)
- **ADC (analog-to-digital)** — 샘플링·양자화·코딩
- **DAC (digital-to-analog)** — R-2R, R-ladder, weighted-resistor

## 기억장치 (12.11)
- **ROM (Read-Only Memory)** — 고정
- **PROM/EPROM/EEPROM** — 프로그래머블
- **RAM** — SRAM(고속/비휘발성), DRAM(고용량/휘발성)

> `raw/books/practical-electronics-eng.md` pp. 721-848

## 보충 소스 (2026-10-22 추가)
- **Digital Electronics 3ed (Tokheim)** — 같은 개념을 직업학교 수준에서 실전 IC로: 코드(BCD/Excess-3/Gray/ASCII, ch.2·6), 게이트+부울대수(ch.3), 74151/74154·7447 MUX/DEMUX/디코더(ch.5-6), R-S·D·JK·Schmitt(ch.7), 리플/동기/다운 카운터+주파수 분배(ch.8), 74194 시프트 레지스터(ch.9), Half/Full Adder·2의 보수(ch.10), RAM/ROM/PROM(ch.11), 디지털 시계·주파수 카운터(ch.12), 연산증폭기 매개 D/A·A/D(ch.13). `^[raw/books/digital-electronics.md]`
- **Levine 실험서 (Digital Theory & Experimentation)** — 논리 논리를 **실험으로 검증**: Exp 1 Basic Logic Functions, Exp 2 Boolean Algebra and Simplification, Exp 3 De Morgan, Exp 4 TTL NAND/NOR 전달 특성, Exp 5 Exclusive-OR, Exp 6 Full-Adder/Subtractor(74183 MSI), Exp 7 Bistable/FF, Exp 8 Binary Counters, Exp 9 Divide-by-N, Exp 10 Shift Registers & Ring Counters, Exp 13 Decoding & Encoding(7-segment), Exp 14 RAM·Exp 16 D/A·A/D. 부록: 로직 기호 · Unit Load. `^[raw/books/digital-theory-experimentation.md]`
- **전자공학입문 (학당) ch.10** — 한국 기술평가 시험 수준: DTL/TTL/MOS 3 제품군, 반가산자·전가산자·해독기·멀티플렉서·부호기, RS/D/JK-FF, D/A·A/D. `^[raw/books/intro-electronics.md]`

## Related
- [[microcontroller-arduino]] — MCU의 GPIO·레지스터
- [[fpga-hdl]] — HDL을 이용한 논리 구현
- [[semiconductor-devices]] — IC 내 트랜지스터 기반
- [[dc-ac-circuit-analysis]] — 디지털 회로의 물리 토대인 DC/AC 회로 해석(논리 게이트의 정전위 해석, 전원·잡음 여유의 회로 근거)
