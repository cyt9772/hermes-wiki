---
title: 디지털 신호처리와 MATLAB (양원영·조용수, 2006, 홍릉과학출판사)
created: 2026-10-30
updated: 2026-10-30
type: entity
tags: [book, engineering, digital-signal-processing, dsp, dft-fft, matlab-simulation]
sources: [raw/books/dsp-matlab-young-cho.md]
confidence: high
---
# 디지털 신호처리와 MATLAB (2006, 홍릉과학출판사)

> 저자: **양원영** · **조용수** (전자/통신공학)
> 출판: 홍릉과학출판사, 2006, 333p

## 개요
DSP 교과 + MATLAB 실습 9개 장: **CtFS/CtFT/DtFT/DFS/DFT** (제1장) → **LTI impulse response** (제2장) → **상관·Power Spectrum** (제3장) → **DFT filter 구조**(직렬·격자) → **IIR/FIR 필터** 설계 → **Kalman·Wiener·Adaptive·Multirate·Wavelet** 9개 장으로 DSP 이론과 MATLAB 시뮬레이션을 하나의 교과서로 통합한 한국 편성이다 `[raw/books/dsp-matlab-young-cho.md]`.

## 장 구조 (TOC 기반, 333p)
1. CtFS/CtFT/DtFT/DFS/DFT — 1.1 변환, 1.2 Sampling Theorem, 1.3 FFT, 1.4 DFT/FFT 스펙트럼 `[raw/books/dsp-matlab-young-cho.md]`
2. Impulse 응답과 시스템함수 (LTI) — 2.1 컨볼루션, 2.2 주파수응답, 2.3 DFT 컨볼루션 `[raw/books/dsp-matlab-young-cho.md]`
3. 상관과 Power Spectrum — 3.1 상관수열, 3.2 PSD, 3.5 DFT/IDFT 상관 `[raw/books/dsp-matlab-young-cho.md]`
4. DFT 기반 필터의 구조 — 직렬(Direct), 격자(Lattice) `[raw/books/dsp-matlab-young-cho.md]`
5-9. IIR/FIR filter, Kalman·Wiener, Multi-rate, Wavelet

## 핵심 내용
- DSP 교과 + MATLAB 실습(Kalman·Wiener·Adaptive · Multi-rate · Wavelet) — 9개 장, 333p 분량의 한국 DSP 교과 `[raw/books/dsp-matlab-young-cho.md]`
- MATLAB Signal Processing Toolbox의 `filter`, `freqz`, `designfilt`, `lsim`, `step` 등 실습 함수 활용 (MATLAB R14 era, 2006년)
- Oppenheim·Willsky `Signals and Systems` 2nd Ed ([[signals-and-systems-oppenheim]] — 1983 1st ed)과 DSP 실습 축으로 분리. 이 권은 DSP 응용(Kalman, Wavelet, Multirate)까지 다룬다
- DSP + Image MATLAB 교재([[dsp-image-matlab-charbit]])에서는 영상까지 확장 — 이 권은 DSP만

## 관련
- 개념: [[digital-signal-processing]] (DSP 실습 축) · [[spread-spectrum-cdma]] (응용)
- 책: [[dsp-image-matlab-charbit]] (DSP+Image) · [[signals-and-systems-oppenheim]] (신호-시스템 이론) · [[signals-processing-first]] (DSP FIRST, Georgia Tech)
- 인접: [[estimation-and-filtering]] (Kalman/Wiener)
