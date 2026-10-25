---
title: Wavelet Transforms (Rao & Bopardikar 1998)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering, signal-processing, wavelet, dsp]
sources: [raw/books/wavelet-transforms-1998.md]
confidence: high
---
# Wavelet Transforms: Introduction to Theory and Applications (Rao & Bopardikar, 1998)

> 저자: **Raghuveer M. Rao** (USC), **Ajit S. Bopardikar** (IIT Bombay)
> 출판: **Addison-Wesley Longman**, 1998 (First printing July 1998), 322p (ISBN 0-201-63463-5)
> cover: "Pseudocolor plot of the phase of the continuous wavelet transform of a complex-valued random signal. Wavelet used: Mexican hat." (copyright page, raw p.4)
> 원서 인용: "Rather than starting with one or two chapters devoted to notation and basic material such as Fourier analysis, the reader is led directly into the subject using basic linear filtering principles." (Preface, p. xiii)

## 개요
CWT → MRA → orthonormal/biorthogonal wavelet → **데이터 압축·denoising·통신 응용**까지를 "도입 + 응용" 체제로 묶은 학술서. cover image가 Mexican hat CWT 위상 plot인 점에서 **구현·응용** 편중이 특징. 7장 + 부록·index. `^[raw/books/wavelet-transforms-1998.md]`

## 장 구조 (7장, 322p — TOC 기반)
1. **CONTINUOUS WAVELET TRANSFORM** — CWT as correlation, operator, inverse, Cq (p.1)
2. **INTRODUCTION TO THE DWT AND ORTHOGONAL WAVELET DECOMPOSITION** — nested subspaces, Haar, MRA 예 (p.25)
3. **MRA, ORTHONORMAL WAVELETS AND RELATIONSHIP TO FILTER BANKS** — two-scale, decomposition/reconstruction, Daubechies D4, PRQMF, DTWT (p.51)
4. **ALTERNATIVE WAVELET REPRESENTATIONS** — biorthogonal (95), twindimensional (109), nonseparable (115), **wavelet packets (121)**
5. **WAVELET TRANSFORM AND DATA COMPRESSION** — transform coding (142), **DTWT image compression (147)**, embedded tree coding (151), JPEG 비교 (166), audio (170, ISO/MPEG subband, wavelet-based), video (181)
6. **OTHER APPLICATIONS** — denoising (183), speckle removal (189), edge detection (192), image fusion (200), communication: scaling as signaling pulses (208), **discrete wavelet multitone modulation** (214)
7. **ADVANCED TOPICS** — CWT revisited (Parseval, A trous, regularity, Daubechies construction) (p.219)

## 핵심
- **CWT → DWT bridge** — Ch.1 → Ch.2·3, 7.3
- **Two-scale relation + PR filter bank** — Ch.3 (p. 59-84)
- **Biorthogonal & nonseparable (2-D/3-D) wavelet** — Ch.4 (p.109-120)
- **Embedded Tree Image Coding (SPIHT 계열)** — 5.3.2, p. 151+
- **Discrete Wavelet Multitone Modulation (DWMM)** — 6.7.2, p. 214
- **Daubechies D4 예 + A trous** — 3.6.1, 7.3.2

## Related
- 개념: [[digital-signal-processing]], [[transform-coding]]
- 저자: Raghuveer M. Rao ([[k-r-rao]] 관련), Ajit S. Bopardikar
- 인접: [[introduction-wavelets-wavelet-transforms]] (Rice primer), [[fundamentals-of-wavelets]] (Goswami·Chan), [[image-video-compression-standards]] (JPEG/MPEG 실전)
