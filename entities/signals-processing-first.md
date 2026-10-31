---
title: 신호처리 FIRST (McClellan·Schafer·Yoder 원저, 1st Edition 한국어판 2005)
created: 2026-10-30
updated: 2026-10-30
type: entity
tags: [book, engineering, signal-processing, digital-signal-processing, dft-fft]
sources: [raw/books/signals-processing-first.md]
confidence: high
---
# 신호처리 FIRST (1st Edition 한국어판, 2005)

> 원저: **James H. McClellan** · **Ronald W. Schafer** · **Mark A. Yoder** (Georgia Tech)
> 역: 김인택 · 김우식 · 한승수 · 서덕영 (공학박사 4인) · Pearson Education/KOREA + 홍릉(洪陵), 2005, 520p, (원서 2003 Prentice Hall, ISBN 0130909998)

## 개요
DSP 입문 교과 "DSP First". MATLAB R13~R2005 시대의 학부 1~2학년 수준에서 시계열·주파수응답·Filter design을 **실습(M-file) 중심**으로 배우는 접근을 정립한 Georgia Tech 3교수의 편성이다 `[raw/books/signals-processing-first.md]`.

## 장 구조 (TOC 기반, 520p)
1. 시계열 기본 (time-discrete sequence, shift/multiply/fold)
2. LTI 시스템과 컨볼루션 — `conv`, `deconv`, `filter`, `freqz`, `freqz`
3. 푸리에 변환 (DTFT, 주파수응답)
4. DFT/FFT — 스펙트럼 계산을 위한 이산 변환
5. IIR/FIR filter 설계 — FIR(equiripple·window), IIR(bilinear, Butterworth·Chebyshev)
6. 주파수응답, window, 다중비율 필터 (Multirate) — polyphase

## 핵심 내용
- "DSP First" 접근 — DSP 전공자가 아니어도 신호처리/음향처리/레이더/생물의학 신호 기초를 **MATLAB 실습**으로 배울 수 있는 학부 1~2학년 수준
- MATLAB R13(R2005) 시대의 `conv, deconv, filter, freqz, freqz, buttord, filtdesign` 등 DSP Toolbox 함수를 교과서로 활용
- 본 위키 신호처리 축([[digital-signal-processing]])에서 **DSP 입문 축**에 속하며, Oppenheim·Willsky(1983/1997) [[signals-and-systems-oppenheim]] 계열은 "신호-시스템 이론" 축, McClellan·Schafer·Yoder 이 권은 "DSP 실습" 축으로 분리된다
- 2005년 한국 학부 교과로, MATLAB R13→R2005 시대의 MATLAB/Signal Processing Toolbox 사용법 교과 `[raw/books/signals-processing-first.md]`

## 관련
- 개념: [[digital-signal-processing]] (DSP 입문 축) · [[spread-spectrum-cdma]] (응용) · [[mp3-perceptual-coding]] (DSP 응용)
- 책: [[signals-and-systems-oppenheim]] (신호-시스템 이론 축) · [[dsp-matlab-young-cho]] (DSP+MATLAB 한국 축) · [[dsp-image-matlab-charbit]] (DSP+Image MATLAB)
- 저자: [[alan-v-oppenheim]] (다른 축 — 신호-시스템 이론)
