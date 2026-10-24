---
title: Discrete Cosine Transform: Algorithms, Advantages, and Applications (Rao & Yip 1990)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, dct-transform, signal-processing, fourier-analysis]
sources: [raw/books/dct-algorithms-applications.md]
confidence: high
---
# Discrete Cosine Transform: Algorithms, Advantages, and Applications (Rao & Yip 1990)

> 표지/원저: **K. R. Rao** (The University of Texas at Arlington, Dept. of Electrical Engineering) · **P. Yip** (McMaster University, Hamilton, Ontario, Canada)
> 출판: Academic Press, Inc. (Harcourt Brace Jovanovich), 1990, 508p (ISBN 0-12-580203-X)

## 개요
DCT(Discrete Cosine Transform)를 **전담으로** 다룬 단행본. (1) DCT 정의와 일반 성질(unitarity, time scaling/shift, difference/convolution property, 제2장), (2) **DCT와 Karhunen-Loeve Transform (KLT)의 관계**·asymptotic equivalence로 "DCT가 왜 자연스러운 변환인가"를 수학적으로 정립(제3장), (3) **Fast DCT 알고리즘** — DCT via FFT, sparse matrix factorization, DIT/DIF, DCT-I/II/III/IV 간 전환(제4장), (4) **2차원 DCT 알고리즘**(제5장), (5) DCT 성능(제6장), (6) **응용** — 화상/데이터 압축·JPEG/MPEG 관련(제7장)으로 이어지는 7장 구조. FFT를 통한 DCT와 sparse matrix factorization 두 축의 Fast 알고리즘 비교가 핵심 `[raw/books/dct-algorithms-applications.md]`.

## 장 구조 (7장, 508p)
1. **Discrete Cosine Transform** — Introduction, 조직, 부록, 참고문헌
2. **Definitions and General Properties** — Fourier cosine transform, DCT 정의, **unitarity**, time scaling/shift, difference property, convolution property
3. **DCT and Its Relations to the Karhunen-Loeve Transform (KLT)** — DCT-I/II, **asymptotic equivalence**, generating unitary transforms (DCT-I에서 출발해 DCT-II를 유추)
4. **Fast Algorithms for DCT-II** — DCT via FFT, **Sparse Matrix Factorization**, DIT/DIF algorithms, DCT via other discrete transforms, other algorithms
5. **Two-Dimensional DCT Algorithms** (원문 TOC 1글자 깨짐)
6. **Performance of the DCT**
7. **Applications of the DCT** — compression techniques의 기본 개념

## 핵심 내용
- DCT-IV에서 출발해 **DCT-I / DCT-II / DCT-III / DCT-IV**를 한데 정리한 **정식 정의** 책 — DCT-II가 JPEG/MPEG 표준에서 실제로 쓰임 `[raw/books/dct-algorithms-applications.md]`
- Fast DCT 두 축: **DCT via FFT**와 **sparse matrix factorization** — FFT와 독립적 근사계산 방법 비교 `[raw/books/dct-algorithms-applications.md]`
- **KLT와의 관계** — "DCT가 왜 자연스러운 변환인가"를 asymptotic equivalence로 수학화(제3장) `[raw/books/dct-algorithms-applications.md]`
- 2차원 DCT 알고리즘(제5장) — 실제 영상 코덱(JPEG 8x8 DCT block)의 알고리즘 기반 `[raw/books/dct-algorithms-applications.md]`
- DSP 교과서([[a-course-in-dsp]] 제4.9절)의 DCT 정의와 **상호보완** — 본서는 알고리즘·수학, DSP 교과서는 정의만

## Related
- 저자: [[k-r-rao]] · (P. Yip — 본 클러스터에서 저자 페이지 미생성, basket 규칙)
- 개념: [[transform-coding]] — DCT/DPCM 변환 부호화 클러스터 개념
- 인접: [[a-course-in-dsp]] (DCT 정의만 다룸), [[digital-video-engineering-korea]] (DCT 영상부호화·JPEG/MPEG), [[digital-image-processing-2ed]] (DCT 변환)
