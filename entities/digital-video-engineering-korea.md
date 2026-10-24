---
title: 디지탈 영상공학 (황재정 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, video-compression, h-261, image-processing]
sources: [raw/books/digital-video-engineering-korea.md]
confidence: high
---
# 디지탈 영상공학 (황재정 1999)

> 표기/원저: **황재정**
> 출판: 도서출판 아진 (A-JIN), 1999-05, 425p

## 개요
디지털 영상 부호화(영상 압축)의 **알고리즘 기초 → 표준 코덱**까지를 하나의 교재로 다루는 국내 표준서. 비디오·색 표현·샘플링(제1장) → 양자화(스칼라·**벡터 양자화** 제2장) → **예측부호화(DPCM, 선형·적응 예측기)**(제3장) → **변환부호화(DCT, 2D DCT, 고속 알고리즘)**(제4장) → **움직임 예측·보상**(제5장)을 일반 원리 단계로 다룬 뒤, **JPEG**(제6장) → **ITU-T H.261**(제7장) → **MPEG-1**(제8장) → **MPEG-2**(제9장) → **H.263**(제10장) → MPEG 오디오(제11장) → HDTV 응용(제12장)으로 표준 코덱을 세대로 이어 나간다. 매 장마다 문제·과제를 붙인 강의 교재형으로 구성된다 `[raw/books/digital-video-engineering-korea.md]`.

## 장 구조 (TOC 기반, 425p)
1. **비디오 및 샘플링** — 아날로그 비디오·NTSC, 색표현(RGB/YUV/YIQ/YCbCr/SMPTE 240M/colorimetry), 샘플링
2. **양자화** — 스칼라 양자화·균일 양자화기·블록 변환계수 양자화, **벡터 양자화**(코드북 설계)
3. **예측부호화** — 폐회로 DPCM, 선형·적응 예측기, DPCM 변형(이중 예측기·신호 몽롱화)
4. **변환부호화** — **DCT**, 다차원·2D DCT, DCT 영상부호화(직진스캔·HVS 하중), DCT 고속 알고리즘(FFT 기반)
5. **움직임 예측 및 보상** — 변환+움직임보상 부호화, 움직임 예측, 고속 ME 알고리즘
6. **JPEG 정지 영상 압축** — 베이스라인·점진·무손실·계층 부호화
7. **ITU-T H.261 동영상 부호기** — 계층적 다중화(CIF), 루프내 DCT/IDCT·양자화·VLC, 움직임 예측·보상, 루프 필터링
8. **MPEG-1 비디오 부호기** — SIF, GOP, 비트열 계위, I/P/B/D 픽쳐 부호화
9. **MPEG-2 비디오** — 확장 부호화 개념, I/P/B, 향상된 움직임보상, **계층부호화**(공간·SNR·시간), 비트율 제어
10. **H.263 초저속 부호화** — UV 모드·SAC·PB프레임, HRD·TMN5·Telenor 비트율 제어
11. **MPEG 오디오 부호화** — MUSICAL·ASPEC, 레이어 I/II/III, MPEG-2 오디오
12. **고선명 텔레비젼 응용**

## 핵심 내용
- **부호화 4요소**: 양자화·예측(DPCM)·변환(DCT)·움직임보상을 표준 부호화의 공통 뼈대로 정리 `[raw/books/digital-video-engineering-korea.md]`
- **DCT 고속 알고리즘**: N-점 DCT의 FFT 기반 분해법까지 실습 수준으로 기술 `[raw/books/digital-video-engineering-korea.md]`
- **H.261 코더**: CIF, 루프 DCT, MC, loop filter, bit-rate control의 표준 구조 상세 `[raw/books/digital-video-engineering-korea.md]`
- **MPEG-1/2**: GOP·I/P/B/D 픽쳐, 계위(스케일러빌리티) 부호화(공간·SNR·시간) `[raw/books/digital-video-engineering-korea.md]`
- **H.263**: 초저속 부호화, UV·SAC·PB프레임, VBV/HRD 버퍼 모델 `[raw/books/digital-video-engineering-korea.md]`

## Related
- 저자: [[hwang-jae-jung]]
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[video-coding-standard-codecs]] (표준 코덱 교차) · [[mpeg-2-watkinson]] · [[mpeg2-source-code-commentary]] · [[image-processing-fundamentals]]
