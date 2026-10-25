---
title: Computer-Based Exercises for Signal Processing Using MATLAB
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, dsp, matlab-simulation, dft-fft]
sources: [raw/books/computer-based-exercises-signal-matlab.md]
confidence: high
---
# Computer-Based Exercises for Signal Processing Using MATLAB

> C. Sidney Burrus · James H. McClellan · Alan V. Oppenheim · Thomas W. Parks · Ronald W. Schafer · Hans W. Schuessler — Prentice Hall, 1994, 410p. **6개 대학 DSP 교수 공동 "프로젝트 기반 실습서"** — "This book is a collection of computer exercises about digital signal processing. It is an outgrowth of our collective experience in incorporating computer-based projects into our signal processing courses" (Preface, p.xii) [raw/books/computer-based-exercises-signal-matlab.md].

## 개요
"각 프로젝트 = 한 개념의 MATLAB 구현 + 결과 분석" 구조. 교과서와 함께 사용하도록 설계 — "The exercises in this book are designed to be used together with a digital signal processing textbook and on the workstations and personal computers commonly used at most universities" (Preface, p.xii). 11개 장 + Appendix A(Software/Programming Notes, p.385) + Index(p.399). 장 1 서두: "examine the signal property called group delay. The sampling process is studied to show the effects of aliasing and the implementation of various reconstruction schemes" (p.29) [raw/books/computer-based-exercises-signal-matlab.md].

## 장 구조 (TOC 기준, 11장 + Appendix A)
1. **Basic Signals and Systems** (p.2) — 차분방정식, DTFT, group delay, 샘플링·재구성, zero-phase FIR
2. **Discrete Fourier Transform** (p.43) — DFT 속성·대칭, DFT as a matrix, 원형·블록 컨볼루션, DCT·DHT
3. **Spectrum Analysis** (p.83) — spectral window, 주파수 해상도, periodogram
4. **Multirate Processing** (p.113) — interpolation, decimation, 필터뱅크, 샘플률 변환
5. **Systems and Structures** (p.129) — IIR·FIR 구조, 격자형, 구조적 민감도
6. **Stochastic Signals** (p.159) — 이산 랜덤 프로세스, 주파수응답, 스펙트럼 추정
7. **Wordlength Effects** (p.205) — 연산정확도, roundoff, quantization
8. **Discrete-Time Filter Design** (p.247) — FIR·IIR 설계 MATLAB 구현
9. **DFT and FFT Algorithms** (p.289) — FFT 알고리즘 구현·비교, Goertzel
10. **Applications** (p.317) — 실신호 처리 프로젝트
11. **Signal Modeling** (p.351) — AR/ARMA 모델링
+ Appendix A Software and Programming Notes (p.385) · Index (p.399)

## 핵심
- **6교수×11장 = 6개 교실 프로젝트의 통합** — 각 장이 개별 교수의 실습 경험에서 온 "독립 모듈". [[discrete-time-signal-processing]](Oppenheim·Schafer 이론서)의 장 6–7(구조·필터설계)과 장 8–9(DFT·FFT)를 **프로젝트 단위로 재구성**
- **Wordlength Effects**(장 7, p.205)는 이론서(DTSF 장 6.7–6.10)의 limit cycle·roundoff를 **MATLAB 시뮬레이션으로 검증** — "이론의 한계 = 실습의 목표"이 이 책의 철학
- **Signal Modeling**(장 11, p.351)은 AR/ARMA → [[estimation-and-filtering]]·[[stochastic-processes-cluster]] 접점. 같은 저자(Porat)의 [[a-course-in-dsp]]와 다른 관점(이론 vs 실험)
- group delay(장 1, p.24)·zero-phase FIR(장 1, p.35)은 [[digital-signal-processing]]의 위상 이론을 **신호 처리 도구로 전환**하는 첫 장

## 저자·관련
- 저자: [[alan-v-oppenheim]] (Burrus·McClellan·Parks·Schafer·Schuessler 별도 페이지 없음)
- 개념: [[digital-signal-processing]] · [[dct-algorithms-applications]] · [[digital-signal-processing]]
- 인접: [[discrete-time-signal-processing]] (같은 저자 이론서) · [[a-course-in-dsp]] (Porat, 같은 클러스터) · [[contemporary-linear-systems-matlab]] (같은 MATLAB 기반 선형시스템 실습) · [[estimation-and-filtering]] (장 11 스펙트럼 추정)
