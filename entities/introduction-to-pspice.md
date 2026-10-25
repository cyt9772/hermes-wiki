---
title: Introduction to PSpice (James W. Nilsson & Susan A. Riedel)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, circuit-simulation, electronic-circuits, electrical-engineering]
sources: [raw/books/introduction-to-pspice.md]
confidence: high
---
# Introduction to PSpice (James W. Nilsson & Susan A. Riedel)

> 저자: **James W. Nilsson** (Professor Emeritus, Iowa State University) · **Susan A. Riedel** (Marquette University) — *A Supplement to Electric Circuits, Fourth Edition*
> 출판: Addison-Wesley, 1993 (©1993), ISBN 0-201-51318-8, 156p
> PSpice는 MicroSim Corporation의 등록 상표. SPICE(Simulation Program with Integrated Circuit Emphasis)를 MicroSim이 상용화한 버전.

## 개요
*Electric Circuits* 4판(1992)의 공식 PSpice 실무서. 회로 해석 수업에 SPICE를 통합하기 위한 세 가지 목표를 가진다. (1) PSpice source file 작성법 학습, (2) op amp·변압기 등 기본 소스의 회로 모델 구성, (3) **컴퓨터 출력 데이터를 검증하는 능력** — "PSpice 출력의 신뢰성을 높이는 수단으로 컴퓨터 출력을 검증하기" (Preface). 67문제를 모두 풀어 solution manual이 제공되며, 교과서 Drill Exercise·chapter Problems 풀이에도 사용 가능.

## 장 구조 (18장 + 부록 A-D + Problems/Answers, 156p)
| # | topic | pp |
|---|-------|----|
| 1 | PSpice in General — Data·Control·Output Statements | 1–6 |
| 2 | DC Analysis Data Statements (독립·종속 DC 소스, 저항) | 7–14 |
| 3 | DC Analysis Control (.OP·.DC·.TF·.SENS) | 15–22 |
| 4 | DC Analysis Output Statements | 23–28 |
| **5** | **Operational Amplifiers** (저항+종속소스 모델, 서브회로 모델, op amp library) | **29–36** |
| 6 | Inductors and Capacitors | 37–38 |
| 7 | Time-Dependent Circuit Response (지수 펄스, 과도 응답, natural response) | 39–48 |
| 8 | Switches (분할선형 소스, V/C 제어 스위치) | 49–52 |
| 9 | Step Response | 53–56 |
| 10 | Varying Component Values | 57–60 |
| 11 | Sinusoidal Steady-State Analysis (정현파 소스·응답) | 61–66 |
| 12 | Computing AC Power with Probe | 67–70 |
| 13 | Mutual Inductance | 71–72 |
| 14 | Ideal Transformers | 73–74 |
| 15 | Frequency Response (주파수 변조, Bode plot with Probe) | 75–84 |
| 16 | Pulsed Sources | 85–88 |
| 17 | Fourier Series | 89–96 |
| 18 | Summary | 97–98 |

+ Appendix A–D (PSpice Control Shell & Probe 메뉴 가이드, 시뮬레이션 파라미터 지정, **SPICE와 PSpice의 차이**, Quick Reference) + Problems (131p) + Answers to Selected Problems (149p) + Index (153p)

## 핵심 기여
- **회로 해석 교과서와 1:1 통합** — 주제의 순서가 교과서와 동일하며, 교재 마진의 색상 마크가 이 서보의 해당 섹션을, 이 서보 마진의 "Nilsson" 마크가 교재의 대응 섹션을 상호 연결.
- **검증 습관** — 67문제의 2대 목적: "PSpice source file 작성법 교육" + "PSpice 시뮬레이션 출력을 체크하여 컴퓨터 해가 알려진 회로 동작에 합당한지 확인".
- **op amp 모델링 3단계** (Ch. 5) — 저항+종속소스 → 서브회로 → library 모델로 발전.
- **SPICE ↔ PSpice 차이**를 Appendix C에 명시.

## Related
- 저자: [[james-w-nilsson]] (공저 Susan A. Riedel은 이 wiki에 저자 페이지 없음)
- 모 교과서: [[nilson-riedel-electric-circuits]]
- 개념: [[circuit-simulation-pspice]]
- 인접 개념: [[dc-ac-circuit-analysis]] · [[laplace-transform-circuits]] · [[amplifiers-analog-circuits]]
- 회로 실무: [[circuits-diagnosis-practice]] (실무 진단) · [[intro-electronic-circuits]] · [[theory-of-circuits]]

## OCR/추출 신뢰도
- pdftotext 양호. 수식 일부 깨짐 (`Th6venin`=`Thévenin`, `0ntern[trional`=International) — 식 번호·문맥으로 cross-check.
