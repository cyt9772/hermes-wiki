---
title: Discrete-Time Signal Processing
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, dsp, fourier-analysis, dft-fft]
sources: [raw/books/discrete-time-signal-processing.md]
confidence: high
---
# Discrete-Time Signal Processing

> Alan V. Oppenheim · Ronald W. Schafer — Prentice Hall, 1989, 893p. **이산시간 신호처리 교과서의 표준 (reference standard)**. 1975년 저자들의 *Digital Signal Processing*의 "새로운 텍스트로의 발전"으로 서문에 명시: "The title Discrete-Time Signal Processing was chosen for this new book ... In the mid-1960s digital signal processing emerged as a new branch of signal processing" [raw/books/discrete-time-signal-processing.md].

## 개요
"이산시간(Discrete-Time)"이라는 제목이 핵심 — 연속시간 *Digital Signal Processing*(1975)의 내용을 **DTFT가 중심 개념, z변환·DFT·FFT가 파생 도구**로 재구축한 판. DTFT(장 2) → 샘플링(장 3) → z변환(장 4) → 주파수응답·시스템함수(장 5) → 구조·유한정밀도(장 6) → 필터설계(장 7) → DFT(장 8) → FFT(장 9) → 힐버트 변환(장 10) → DFT 신호해석·periodeogram(장 11) → 세프스트럼·호모모픽 역컨볼루션(장 12) 순서. 장 4 서두 "The Fourier transform plays a key role in representing and analyzing discrete-time signals and systems. In this chapter, we consider a generalization ... referred to as the z-transform" (p.149)이 이 위계 자체를 요약 [raw/books/discrete-time-signal-processing.md].

## 장 구조 (TOC 기준, 12장 + Appendix A·B)
1. **Introduction** (p.1)
2. **Discrete-Time Signals and Systems** (p.8) — 시퀀스, LTI, 차분방정식, DTFT 대칭·정리, 이산 랜덤 신호
3. **Sampling of Continuous-Time Signals** (p.80) — 주기 샘플링, 주파수영역 표현, 대역제한 신호 재구성, 샘플률 변경
4. **The z-Transform** (p.149) — 수렴영역, 역z변환, 복소 컨볼루션 정리, 파세발
5. **Transform Analysis of LTI Systems** (p.202) — 주파수응답, 합리 시스템함수, 진폭-위상 관계, **Allpass·최소위상·일반화 선형위상**
6. **Structures for Discrete-Time Systems** (p.290) — 블록다이어그램·신호흐름도, IIR·FIR 구조, transposed·격자형, **유한정밀도: 계수양자화·라운드오프·zero-input limit cycle**
7. **Filter Design Techniques** (p.403) — 연속→이산 IIR, 주파수 변환, 컴퓨터지원 IIR, 윈도우법·Kaiser FIR, equiripple 최적 근사
8. **The Discrete Fourier Transform** (p.514) — DFS→DFT, DFT 속성, 선형 컨볼루션
9. **Computation of the DFT** (p.581) — Goertzel, 디메이션-시간/주파수 FFT, 합성 N, 유한 레지스터 길이 효과
10. **Discrete Hilbert Transforms** (p.662) — 캐오스 시퀀스에 실·상상부 충분성, 진폭-위상 관계
11. **Fourier Analysis of Signals Using the DFT** (p.695) — DFT 신호해석, 시간의존 FT, 블록 컨볼루션, **periodeogram·자기상관 스펙트럼** (랜덤 신호)
12. **Cepstrum Analysis and Homomorphic Deconvolution** (p.768) — 복소 세프스트럼, 호모모픽 필터, **음성 처리 응용**
+ Appendix A Random Signals (p.835) · B 연속시간 필터 (Butterworth·Chebyshev·Elliptic, p.845) · Bibliography (p.851) · Index (p.869)

## 핵심
- **DTFT-중심 위계** — z변환을 FT의 "일반화"로 제시 (장 4 서두, p.149). 이 관점은 [[digital-signal-processing]]·[[digital-signal-processing]] 클러스터의 이산시간 쪽 축을 정하는 문장
- **유한정밀도 효과 3종**(계수양자화, 라운드오프 노이즈, zero-input limit cycle)을 장 6 6.7–6.10에서 IIR 구조와 함께 다룸 — p.373 "zero-input limit cycles whereby the output oscillates periodically when the input is zero. Limit cycles are caused both by quantization and by overflow" [raw/books/discrete-time-signal-processing.md]. 이 부분이 [[computer-based-exercises-signal-matlab]] 장 7 Wordlength Effects의 이론 근거
- **호모모픽 역컨볼루션**(장 12)은 음성처리 응용(12.9, p.815)으로 이어지는 유일한 교과서적 처리 — [[discrete-random-signals]](장 11 periodeogram)와 함께 이산 랜덤 신호↔음성 신호 접점
- FIR equiripple·IIR 계수양의·구조 민감도 3종이 [[dct-algorithms-applications]](장 8–9)와 연결: FIR 설계→DFT 샘플링, IIR 구조→FFT 기반 컨볼루션

## 저자·관련
- 저자: [[alan-v-oppenheim]] (R.W. Schafer 별도 페이지 없음)
- 개념: [[digital-signal-processing]] · [[digital-signal-processing]] · [[dct-algorithms-applications]]
- 인접: [[signals-and-systems-oppenheim]] (같은 저자 연속시간판) · [[a-course-in-dsp]] (Porat, 같은 클러스터 입문서) · [[discrete-random-signals]] (장 11 랜덤 신호) · [[computer-based-exercises-signal-matlab]] (같은 저자 MATLAB 실습서)
