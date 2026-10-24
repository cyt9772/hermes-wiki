---
title: 알기 쉬운 MPEG-2 소스코드 해설 (이호석·김준 2000)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, video-compression, mpeg-standard, data-communication]
sources: [raw/books/mpeg2-source-code-commentary.md]
confidence: high
---
# 알기 쉬운 MPEG-2 소스코드 해설 (이호석·김준 2000)

> 표지/원저: **이호석 · 김준**
> 출판: 홍릉과학출판사, 2000 (머리말 2000. 11.), 562p

## 개요
국내에서 최초로 MPEG-2 **소스코드**(Test Model 5, TM5, http://www.mpeg.org)를 직접 분석해 해설한 실무서. ISO/IEC 13818-2(비디오) 기준의 부호기·복호기 루틴을 함수 수준으로 분해하며, MPEG-2 이론 3요소인 **DCT**(공간 압축, Fourier 뿌리), **DPCM**(차이 분호화), **움직임 예측·보상**(시간 압축, full search block matching)을 먼저 정리(제1-2장)한다. 이후 비트스트림 신택스(제3장) → **부호기 전체 구조와 알고리즘**(main(), frame reordering, motion estimation, transform(), DCT, quantization, VLC, rate control — 제4장) → **복호기 루틴**(getbits(), 프레임·블록 복호화, IDCT, 표시 — 제5장) → **움직임 부호화·복호화** 상세(움직임 벡터, dual prime, 반화소 필터링 — 제6장) → **스케일러빌러티**(SNR/space일 scalability, TM5 미구현 기능까지 원문 근거로 기술 — 제7장)로 이어진다 `[raw/books/mpeg2-source-code-commentary.md]`.

## 장 구조 (TOC 기반, 562p)
1. **MPEG 기초와 관련 기술** — MPEG 기초, JPEG, H.261, MPEG-1 비디오, MPEG-2 비디오
2. **MPEG-2 기본 압축 알고리즘** — 데이터 압축, 영상 표현(sequential/interlaced, frame/field, picture, chroma format), 공간·시간 압축, RLC, 픽처 타입·GOP, slice·macroblock·block, buffer control, Profiles and Levels
3. **MPEG-2 비트스트림** — 비디오 계층, bitstream syntax, syntax 구조와 표, 비트스트림 분석
4. **MPEG-2 부호기의 전체 구조와 알고리즘** — 전체 구조, main(), parameter file, read quant_matrix, init, frame reordering, frame/field 설정, read frame, **motion estimation**, predict(), dct_type_estimation(), transform(), **DCT**, 양자화, VLC, rate control, MPEG-2 rate control, 역양자화, inverse transform
5. **MPEG-2 복호기의 전체 구조와 알고리즘** — 복호화 루틴, init, **getbits()**, header decoding, frame decoding, block decoding, copy/add block, IDCT, addblock(), display
6. **움직임 부호화와 복호화** — 움직임 벡터 부호화·복호화, VLC, 움직임 벡터 예측기 갱신·초기화, dual prime, chroma 움직임 벡터, hidden vectors, half-pel filtering, skipped macroblock, motion compensation
7. **스케일러빌러티 (scalability)** — SNR/temporal/spatial 계위, TM5 구현과 문서 대조
+ 부록: MPEG-2 용어 해설

## 핵심 내용
- **TM5(테스트 모델) 소스 해설**: 부호기/복호기의 루틴을 함수 하나하나로 분해, 원문 소스 코드와 함께 설명 `[raw/books/mpeg2-source-code-commentary.md]`
- **부호화 파이프라인**: read frame → motion estimation → predict → dct_type_estimation → transform(DCT) → quantization → VLC → rate control `[raw/books/mpeg2-source-code-commentary.md]`
- **복호화 파이프라인**: getbits → header decoding → frame decoding → block decoding → IDCT → addblock → display `[raw/books/mpeg2-source-code-commentary.md]`
- **움직임 벡터 부호화**: dual prime, chroma vector scaling, half-pixel interpolation filter, skipped macroblock 등 세부 구현 `[raw/books/mpeg2-source-code-commentary.md]`
- **Rate control**: MPEG-2 rate control 알고리즘의 소스 수준 해설 `[raw/books/mpeg2-source-code-commentary.md]`
- **Scalability**: SNR·temporal scalability의 개념과 TM5 미구현 기능에 대한 원문 근거 기술 `[raw/books/mpeg2-source-code-commentary.md]`

## Related
- 저자: [[lee-ho-seok]] · [[kim-jun]]
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[mpeg-2-watkinson]] (MPEG-2 개념서) · [[video-coding-standard-codecs]] (표준 코덱 교차) · [[mpeg-system-korea]] (시스템 파트)
