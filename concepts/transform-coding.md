---
title: 변환 부호화 · 변환 처리 (DCT/DPCM)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, dct-transform, signal-processing, fourier-analysis, video-compression]
sources: [raw/books/dct-algorithms-applications.md, raw/books/digital-video-engineering-korea.md, raw/books/digital-image-processing-2ed.md]
confidence: medium
---
# 변환 부호화 · 변환 처리 (DCT/DPCM)

**DCT(Discrete Cosine Transform)** 로 신호를 변환 도메인에 옮기고(에너지 축적), 양자화·부호화해 압축하는 방식. 예측 부호화(DPCM)와 함께 데이터 압축의 두 축. 본 클러스터의 DCT 전문 서적(Rao·Yip)이 정의·알고리즘을, 한국 영상공학·영상처리 교재가 영상 적용을 담당한다.

## DCT 전문 서적 — Discrete Cosine Transform (Rao & Yip 1990)
- DCT 정의와 일반 성질 단위화: unitarity, time scaling/shift, difference·convolution property(제2장) `[raw/books/dct-algorithms-applications.md]`
- **KLT(Karhunen-Loeve)와의 asymptotic equivalence**(제3장) — 왜 DCT가 통계적으로 자연스러운 변환인가의 근거 `[raw/books/dct-algorithms-applications.md]`
- **Fast DCT 두 축**: DCT via FFT + sparse matrix factorization, DIT/DIF, DCT-I/II/III/IV 간 변환(제4장) — 실제 코덱은 **DCT-II** 사용 `[raw/books/dct-algorithms-applications.md]`
- 2차원 DCT 알고리즘(제5장)과 성능(제6장), 압축 기술 응용(제7장) — JPEG 8×8 블록의 알고리즘적 기반 `[raw/books/dct-algorithms-applications.md]`

## 디지털 영상공학 (한국 교재)
- 제3장 예측부호화: **폐회로 DPCM**, 선형/적응 예측기, DPCM 변형(양자화/자압축 결합) `[raw/books/digital-video-engineering-korea.md]`
- 제4장 **변환부호화**: 변환의 개념 → 이산여현변환(DCT) → 2차원/다차원 DCT → **DCT 영상부호화**(지그재그 스캔, **HVS 하중**), **DCT 고속 알고리즘**(2N점 FFT 기반) `[raw/books/digital-video-engineering-korea.md]`
- VQ(벡터 양자화)의 설계와 종류(2.2-2.3) — 스칼라 양자화 대비 `[raw/books/digital-video-engineering-korea.md]`

## 디지털 영상 처리 (Gonzalez & Wintz)
- 2차원 DCT의 forward/inverse 커널(3.5)을 선형대수적 변환(행렬)으로 정식 정의 — DCT의 수학적 구조 `[raw/books/digital-image-processing-2ed.md]`
- DPCM 포함 예측형/변환형 부호화 프레임워크와 양자화(quantization) 관점(본문에 quantization 논의 다수) `[raw/books/digital-image-processing-2ed.md]`

## 비교/요약

| 소스 | DCT 관련 범위 | 기여 |
|---|---|---|
| Rao & Yip 1990 | DCT 전역 (정의→KLT→Fast→2D→성능→응용) | **알고리즘·수학** 정석 |
| 디지털 영상공학 (한국) | 영상 코덱 내 DCT/DPCM | 적용: HVS, 지그재그, FFT 활용 |
| Gonzalez & Wintz | 2D DCT 커널 공식 | 수학적 정의(행렬/변환) |
| Porat 1997 (접점) | DCT Type I-IV 정의만 (제4.9절) | DSP 교과서 수준 소개 |

## 관련
- [[dct-algorithms-applications]] · [[digital-video-engineering-korea]] (기존) · [[digital-image-processing-2ed]] (기존)
- [[a-course-in-dsp]] (DCT 정의 접점), [[mp3-perceptual-coding]] (HVS/주관적 코딩), [[video-compression-mpeg]] (기존, H.261/MPEG)
