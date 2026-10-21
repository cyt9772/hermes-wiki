---
title: Electric Circuits, 4th ed. (James W. Nilsson & Susan A. Riedel)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, electrical-engineering, electronic-circuits, signal-processing, engineering-mathematics]
sources: [raw/books/nilson-riedel-electric-circuits.md]
confidence: high
---
# Electric Circuits, 4th ed. (James W. Nilsson, Susan A. Riedel)

> "the primary aim of giving students procedural models for solving problems... emphasize problem solving as a process in which one applies conceptual understanding" (Preface, p1)
> 저자: James W. Nilsson (Professor Emeritus, Iowa State University), with contributions by Susan A. Riedel — Addison-Wesley 4th ed., ISBN 0-201-54987-5 (©1992)

## 개요
> **대학 회로 해석(circuit analysis) 교과서의 표준 교재** — 20장 + 부록, 949p. DC 회로 기초(1-5장)에서 R/L/C 동적 회로(7-9장), 정현파 정계 해석(10-12장), 커플링·공진(13-14장), 라플라스/이전함수(15-17장), 푸리에(18-19장), 2포트(20장)까지 회로 해석의 전 스펙트럼을 체계적으로 다룸. PSpice(Design Center) 실습을 각 장에 통합한 것이 특징.

## 장 구조 (20장 + 부록 A-E, 949p)
| # | topic | p |
|---|-------|---|
| 1 | Circuit Variables (전압·전류·전력·에너지, SI) | 1 |
| 2 | Circuit Elements (전원·옴 법칙·키르히호프) | 25 |
| 3 | Simple Resistive Circuits | 55 |
| 4 | Techniques of Circuit Analysis (노드-전압·망-전류·Thévenin/Norton) | 93 |
| 5 | Topology in Circuit Analysis (이득·중첩) | 165 |
| 6 | The Operational Amplifier (연산증폭기·Bartlett 정리) | 189 |
| 7 | Inductance and Capacitance | 227 |
| 8 | Response of First-Order RL and RC Circuits | 253 |
| 9 | Natural and Step Responses of RLC Circuits (공진) | 321 |
| 10 | Sinusoidal Steady-State Analysis (Phasor) | 371 |
| 11 | Sinusoidal Steady-State Power Calculations | 429 |
| 12 | Balanced Three-Phase Circuits | 467 |
| 13 | Mutual Inductance (도트 규약·이상적 변압기) | 503 |
| 14 | Series and Parallel Resonance (Bandwidth/Q) | 553 |
| 15 | Introduction to the Laplace Transform | 601 |
| 16 | The Laplace Transform in Circuit Analysis | 643 |
| 17 | The Transfer Function (부분분수·적분) | 685 |
| 18 | Fourier Series | 737 |
| 19 | The Fourier Transform (Parseval) | 789 |
| 20 | Two-Port Circuits | 827 |
+ Appendix A-E (복소수·삼각함수 항등식·적분표, Examples/Answers Index)

## 핵심 기여 / 학습 포인트
- **문제해결 과정 중심** — "procedural models"보다 개념 이해를 통한 problem-solving 강조 (Preface)
- **PSpice 실습 통합** — 각 장에 PSpice/Design Center 화면 + 문제 (이 책이 PSpice 활용을 교과에 도입한 선구 교재)
- **DC → L/R/C 동적 → AC 정현파 → 라플라스/푸리에** — 회로 해석의 완전한 수학적 진화 경로
- **20장** = 대학 회로 해석 학기 과정의 표준 커리큘럼

## OCR/추출 신뢰도
- **추출**: pdftotext (양호) — 수식 토큰 일부 깨짐(`Th6venin`=`Thévenin`, `0ntern[trional`=International 등) — 식 번호·문맥 cross-check 권장
- **활용법**: 구조·개념 학습엔 충분, 수식 해석은 원본 대조

## Related
- 저자: [[james-w-nilsson]]
- 개념: [[dc-ac-circuit-analysis]], [[laplace-transform-circuits]]
- 관련 교재(회로·동적 회로): [[circuits-and-systems]] (차균현 — 라플라스/상태방정식), [[electronics-basics]] (Grob — 기초), [[theory-of-circuits]] (자격시험 관점)
- 관련 (증폭·실무): [[amplifiers-analog-circuits]], [[practical-electronics-eng]]
