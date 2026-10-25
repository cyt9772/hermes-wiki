---
title: Fundamentals of Wavelets (Goswami & Chan 1999)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering, signal-processing, wavelet, dsp]
sources: [raw/books/fundamentals-of-wavelets.md]
confidence: high
---
# Fundamentals of Wavelets: Theory, Algorithms, and Applications (Goswami & Chan, Wiley 1999)

> 저자: **Jaideva C. Goswami** (Texas A&M), **Andrew K. Chan** (Texas A&M)
> 출판: **John Wiley & Sons**, 1999, 324p (ISBN 0-471-19748-3), Wiley series in microwave and optical engineering
> 원서 인용: "A reason for the popularity of wavelet is its effectiveness in representation of non-stationary (transient) signals ... wavelet analysis uses bases that are localized in time and frequency to represent nonstationary signals more effectively." (Ch.1 What This Book Is About, p. 1)

## 개요
웨이브렛을 **수학(선형 공간·기저) → Fourier/시주파수 → MRA·wavelet 구성 → 필터 뱅크·DWT 알고리즘 → DSP/압축·공학 응용**으로 이끄는 입문~중급 종합서. Texas A&M의 수업(IEEE-AP·ITRF·PIERS short course) 내용을 기반으로 함. 9장 + Appendix. `^[raw/books/fundamentals-of-wavelets.md]`

## 장 구조 (9장, 324p — TOC 기반)
1. **What This Book Is About** (p.1)
2. **Mathematical Preliminaries** — linear spaces, bases, z-transform (p.5)
3. **Fourier Analysis** — series/transform, DFT, Gibbs (p.31)
4. **Time-Frequency Representation** — STFT/Gabor, CWT, DWT, Wigner-Ville, ambiguity (p.57)
5. **Multiresolution Decomposition** — MRA, two-scale, splines (p.89)
6. **Wavelets — Basis Functions** — Shannon/Meyer/Battle-Lemarie/Daubechies, biorthogonal (p.108)
7. **DWT & Filter Bank Algorithms** — decimation, PR bank, polyphase, lifting (p.141)
8. **Fast Integral Transforms & Applications** — crack detection, image restoration (p.187)
9. **DSP Applications** — wavelet packets, thresholding, zero-tree, denoising, compression (p.210)

## 핵심
- **MRA → two-scale relation → cascade algorithm** 체계 (5-6장)
- **Daubechies·sharpest filter** — 4-tap/8-tap 예 (p. 108-115, D4)
- **PR quadrature mirror filter & polyphase** — 필터 뱅크 DWT (Ch.7)
- **Wavelet packet tree + thresholding (soft/hard)** — Ch.9 (p. 210-230)
- **Zero-tree algorithm** — Ch.9 (index, p. 236-238)
- **Fast integral transform** — 물리/공학 문제 응용(Chapter 8, p.187+)

## Related
- 개념: [[digital-signal-processing]], [[transform-coding]]
- 저자: Jaideva C. Goswami, Andrew K. Chan
- 인접: [[introduction-wavelets-wavelet-transforms]] (Rice primer), [[wavelet-transforms-1998]] (Rao & Bopardikar), [[image-video-compression-standards]] (MPEG/JPEG 실전)
