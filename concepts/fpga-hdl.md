---
title: FPGA·HDL (Field-Programmable Gate Array & Hardware Description Language)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# FPGA·HDL (FPGA & HDL)

## 정의
**FPGA(Field-Programmable Gate Array)** — 사용자 정의 논리 회로를 프로그래밍 가능한 IC. **HDL(Hardware Description Language)** — FPGA의 논리를 기술하는 언어(Verilog, VHDL).

## FPGA 구조 — 14장
- **Logic Block (Configurable Logic Block)** — 기본 유닛
- **Interconnect** — Bus
- **I/O Pin** — 디지털/아날로그
- **Config RAM (Bitstream)** — 프로그래밍 데이터
- **SIP (Single-In-Package)** — 단일 칩
- **CPLD (Complex Programmable Logic Device)** — 작은 FPGA

## HDL (Verilog/VHDL) — 14장
- **Verilog** — ANSI C-like, `module`·`input`·`output`·`wire`·`reg`
- **VHDL** — 더 형식적, `entity`·`architecture`·`signal`
- **모듈(Module)** — 논리 단위
- **배선·저항·버스** — Bus
- **병렬실행** — 병렬(Sequential)·병렬(Synchronous)
- **수자 서식** — Number format (binary, decimal, hex)
- **FPGA 묘사** — FPGA Description

## HDL 설계 흐름
1. **요구사항** — 논리 사양
2. **설계** — Verilog/VHDL 코딩
3. **시뮬레이션** — Icarus Verilog, ModelSim
4. **종합(Synthesis)** — HDL → Netlist
5. **Floorplan·Place·Route** — 물리적 배치
6. **Time Simulation** — 타이밍 검증
7. **Bitstream 생성** — FPGA 프로그래밍
8. **Boards** — Elbert v2, Icarus, Basys3

## FPGA vs MCU
| | MCU | FPGA |
|---|---|---|
| 아키텍처 | Von Neumann/Harvard | Parallel |
| 프로그래밍 | C/C++/Assembly | HDL |
| 실행 | Sequential(순차) | Parallel(병렬) |
| 용도 | General-purpose compute | High-speed I/O, DSP, communication |
| 전비 | Low | High |

> `raw/books/practical-electronics-eng.md` pp. 905-940

## Related
- [[digital-logic-basics]] — 논리 게이트 기본
- [[microcontroller-arduino]] — MCU 대비
