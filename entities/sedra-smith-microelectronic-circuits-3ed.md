---
title: Microelectronic Circuits (3rd ed.)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, electronic-circuits, circuit-simulation, signal-processing]
sources: [raw/books/sedra-smith-microelectronic-circuits-3ed.md]
confidence: high
---
# Microelectronic Circuits, 3rd ed.

> Adel S. Sedra (University of Toronto) · Kenneth C. Smith (University of Toronto) — Rinehart & Winston / Saunders, 1991, 1159p. **전자공학 "회로" 교과서의 표준 (Semiconductor Devices → Analog IC → Digital IC 3부 구조)** — 서문: "Following an introductory chapter that presents some of the basic electronic concepts and establishes notation and conventions, the book is divided into three parts. Part I, Devices and Basic Circuits, is composed of Chapters 2 through 5 and deals with the op amp, the diode, the bipolar junction transistor (BJT), and the field-effect transistor (FET)" (Preface) [raw/books/sedra-smith-microelectronic-circuits-3ed.md].

## 개요
"Part I: Devices and Basic Circuits (장 2–5) → Part II: Analog Circuits (장 6–12) → Part III: Digital Circuits (장 13–14)" 3부 구조. Part II가 "the bulk of a first course in electronics" (Preface) — 1단기 전자공학을 **장 6(차동증폭기)에서 중단해도 Part III(디지털)를 곧바로 진행 가능**하도록 설계. Part II와 Part III의 순서를 **자유롭게 교체 가능** (Preface). 장 1 서두: "the book is divided into three parts. Part I, Devices and Basic Circuits ... deals with the op amp, the diode, the BJT, and the FET" [raw/books/sedra-smith-microelectronic-circuits-3ed.md].

## 장 구조 (TOC 기준, 14장 + Appendices A–G + Index)
**Part I: Devices and Basic Circuits**
1. **Introduction to Electronics** (p.1) — 신호, 스펙트럼, 아날로그/디지털, 증폭기, 회로모델, 주파수응답
2. **Operational Amplifiers** (p.48) — **3rd ed.에서 제2장으로 재배치** (2nd ed.에서는 후속 장)
3. **Diodes** (p.116)
4. **Bipolar Junction Transistors** (p.191)
5. **Field-Effect Transistors** (p.298)

**Part II: Analog Circuits**
6. **Differential and Multistage Amplifiers** (p.407)
7. **Frequency Response** (p.488)
8. **Feedback** (p.570)
9. **Output Stages and Power Amplifiers** (p.646)
10. **Analog Integrated Circuits** (p.698) — GaAs·BiCMOS, data converters, CMOS op amps
11. **Filters and Tuned Amplifiers** (p.762)
12. **Signal Generators and Waveform-Shaping** (p.841)

**Part III: Digital Circuits**
13. **MOS Digital Circuits** (p.906)
14. **Bipolar Digital Circuits** (p.989)

+ Appendices: A IC 공정 · B Two-Port · C Computer Aids for Design · D 회로정리 · E 단-시간상수 · F 표준 저항값 · G 문제답안
+ Index (I-1)

## 핵심
- **op-amp가 제2장**(2nd ed.에서는 Part II에 배치) — 3rd ed.의 "핵심 재배치". "new sections have been added on data converters (Sections 10.9–10.11)" + "Coverage of CMOS op amps has been expanded (Section 10.8)" (Preface) [raw/books/sedra-smith-microelectronic-circuits-3ed.md]
- **장 6(차동증폭기)가 Part II의 "문"** — "Except for requiring some knowledge of the differential pair from Chapter 6, the order of Parts II and III can be reversed" (Preface). 즉 **장 6 = 아날로그↔디지털의 경계선**
- **14장 = "디바이스→회로"의 완전 매핑** — 장 2–5(디바이스) → 장 6–12(아날로그 회로) → 장 13–14(디지털 회로). [[intro-electronic-circuits]]·[[intro-electronics]](기초)와 **장 2–5를 공유**하는 구조
- **장 10(Analog IC)에서 "data converter·CMOS op-amp·BiCMOS"를 모두 다루는** 3rd ed. 고유의 내용 — [[circuit-simulation-pspice]] 같은 클러스터의 PSpice·실무서와 **장 10–12를 매칭**하는 교재
- 1159p의 분량이 "Part I(300p) + Part II(800p) + Part III(170p)" — **아날로그:디지털 = 5:1** 비율. 1991년 "Analog IC가 디지털보다 중요"였던 시대적 반영

## 저자·관련
- 저자: Adel S. Sedra, Kenneth C. Smith (University of Toronto — 별도 페이지 없음)
- 개념: [[intro-electronic-circuits]] (전체) · [[circuit-simulation-pspice]] (장 10–12)
- 인접: [[intro-electronic-circuits]] (기초 회로) · [[new-electronics]] (같은 클러스터) · [[sedra-smith-microelectronic-circuits-solutions]] (같은 책 문제풀이) · [[practical-electronics-eng]] (실무서) · [[digital-logic-basics]] (장 13–14)
