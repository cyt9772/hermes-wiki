---
title: A Course in Digital Signal Processing (Porat 1997)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, signal-processing, dsp, dft-fft]
sources: [raw/books/a-course-in-dsp.md]
confidence: high
---
# A Course in Digital Signal Processing (Porat 1997)

> 표지/원저: **Boaz Porat** (Technion, Israel Institute of Technology, Dept. of Electrical Engineering)
> 출판: John Wiley & Sons, 1997, 630p (ISBN 0-471-14961-6)

## 개요
보아즈 포랫(Boaz Porat)의 DSP 핵심 교과서. "Signals and systems" 과목이 끝나고 시작되는 지점(컨벌루션, 변환, 주파수응답, 전달함수, 안정성)을 제2장까지 복습한 뒤, 샘플링·양자화(제3장) → DFT(제4장, DCT/DST 타입별 정의 포함) → FFT(제5장, Cooley-Tukey) → 실질 스펙트럼 분석(제6장) → z-변환·차분방정식(제7장) → 디지탈 필터(제8-11장, FIR/IIR 사양·설계·구현) → 멀티레이트(제12장) → 랜덤 신호(제13장) → 응용(제14장)으로 이어지는 14장 체제. 매 장에 "Summary & Complements"와 MATLAB 프로그램·problems를 붙인 실무형 구성 `[raw/books/a-course-in-dsp.md]`.

## 장 구조 (14장, p.630)
1. Introduction
2. Review of Frequency-Domain Analysis
3. Sampling and Reconstruction — physical A/D·D/A, band-pass sampling, frequency-domain sampling
4. The Discrete Fourier Transform — DFT 성질, zero padding, circular/linear convolution, **DCT Type I-IV** (4.9), DST
5. The Fast Fourier Transform — Cooley-Tukey 분해, DIT/DIF, twiddle factors
6. Practical Spectral Analysis
7. Review of z-Transforms and Difference Equations
8. Introduction to Digital Filters — 사양, 위상응답(linear/GLP/minimum-phase/all-pass), IIR·FIR 설계 고려사항
9. Finite Impulse Response Filters — IRT, 창법, least-squares, **equiripple(Remez)**
10. Infinite Impulse Response Filters (p.328)
11. Digital Filter Realization and Implementation (p.389) — 상태공간/구현 구조
12. Multirate Signal Processing (p.461)
13. Analysis and Modeling of Random Signals (p.513)
14. Digital Signal Processing Applications (p.550) — radar/sonar/speech/telephony

## 핵심 내용
- DCT의 네 가지 타입(DCT-I/II/III/IV) 정의를 DSP 교과서 안에서 정의(제4.9절) — [[dct-algorithms-applications]]에서는 알고리즘·응용으로 전문 심화 `[raw/books/a-course-in-dsp.md]`
- FIR 등치파동(equiripple) 설계·Remez exchange와 IIR·FIR 위상선형성(GLP) 제약을 이산/연속 통합해 다룸 `[raw/books/a-course-in-dsp.md]`
- 신호-시스템 복습(제2장)을 먼저 배치해 "이론 → 설계 → 구현" 흐름이 명확 — [[signals-and-systems-korea]]와 연계 가능
- 랜덤 신호(제13장)와 DSP 응용(제14장)까지 포함해 교과서 범위가 넓음

## Related
- 저자: [[boaz-porat]]
- 개념: [[digital-signal-processing]] — LTI·샘플링·DFT/FFT·필터설계 클러스터 개념
- 인접: [[signals-and-systems-korea]] (Korean signals & systems), [[dct-algorithms-applications]] (DCT 심화)
