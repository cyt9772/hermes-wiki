---
title: Introduction to Wavelets and Wavelet Transforms (Burrus, Gopinath & Guo 1998)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering, signal-processing, wavelet, dsp]
sources: [raw/books/introduction-wavelets-wavelet-transforms.md]
confidence: high
---
# Introduction to Wavelets and Wavelet Transforms: A Primer (Burrus, Gopinath & Guo, Prentice Hall International 1998)

> 저자: **C. Sidney Burrus, Ramesh A. Gopinath, Haitao Guo** (Rice University); 프로그램·부록: **Jan E. Odegard, Ivan W. Selesnick**
> 출판: **Simon & Schuster / Prentice-Hall International**, 1998 (Intl. ed.), 282p (ISBN 0-13-888702-0)
> 원서 인용: "In some areas, it is the first truly new tool we have had in many years. Indeed, use of wavelets and wavelet transforms requires a new point of view and a new method of interpreting representations that we are still learning how to exploit." (Preface, p. xi)

## 개요
웨이브렛의 **필터 뱅크·다중해석(MRA)·기저·프레이밍**을 필터 뱅크 입장에서 설명하는 Rice University primer. 이산 시스템(multirate, filter banks) 관점에서 DWT를 설명하는 선구적 접근. "A Primer" — 수학보다 구조(구조-역학, lattice, lifting)에 중점. 12장 + 부록. `^[raw/books/introduction-wavelets-wavelet-transforms.md]`

## 장 구조 (12장, 282p — TOC 기반)
1. **Introduction to Wavelets** — what is a wavelet, Haar, MRA preview (p.1)
2. **A Multiresolution Formulation of Wavelet Systems** — signal spaces, scaling/wavelet, MRA axioms (p.10)
3. **Filter Banks and the Discrete Wavelet Transform** — analysis/synthesis, lattice, lifting (p.31)
4. **Bases, Orthogonal, Biorthogonal, Frames, Tight Frames, Unconditional Bases** (p.41)
5. **The Scaling Function and Scaling Coefficients, Wavelet and Wavelet Coefficients** — cascade algorithm (p.50)
6. **Regularity, Moments, and Wavelet System Design** — K-regularity, Daubechies, Coiflets, biorthogonal (p.73)
7. **Generalizations of the Basic Multiresolution Wavelet System** — M-band, shift-invariant, local trigonometric, CWT (p.98)
8. **Filter Banks and Transmultiplexers** — PR, unitary, modulated, linear-phase, wavelet packets (p.148)
9. **Calculation of the Discrete Wavelet Transform** — periodic/cyclic DWT, complexity, filter-bank structure (p.188)
10. **Wavelet-Based Signal Processing and Applications** (p.196)
11. **Summary Overview** (p.219)
12. **References** (p.223)

## 핵심
- **필터 뱅크 + multirate = DWT** — Ch.3, Ch.9 (lattice·lifting)
- **Unitary filter bank 정리** — H*(z⁻¹)H(z)=I (Ch.3, Theorem)
- **Biorthogonal wavelet design** — Ch.6
- **2-D wavelets & tensor product** — Ch.7
- **Lattice·Lifting 구조** — Ch.9 (실무 구현)
- **Software (wavelets in C/C++, MATLAB)** — Ch.10-11

## Related
- 개념: [[digital-signal-processing]], [[transform-coding]]
- 저자: C. Sidney Burrus (Rice), Ramesh A. Gopinath (MIT), Haitao Guo
- 인접: [[fundamentals-of-wavelets]] (Goswami·Chan, 더 수학적), [[wavelet-transforms-1998]] (Rao·Bopardikar, 응용), [[image-video-compression-standards]] (JPEG/MPEG 실전)
