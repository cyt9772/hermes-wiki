---
title: MPEG-2: A Standard and Its Applications (Watkinson 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, video-compression, mpeg-standard, media-frameworks]
sources: [raw/books/mpeg-2-watkinson.md]
confidence: high
---
# MPEG-2: A Standard and Its Applications (Watkinson 1999)

> 표지/원저: **John Watkinson**
> 출판: Focal Press (Butterworth-Heinemann), 1999 (First published 1999, Reprinted 2000, ISBN 0 240 51510 2), 252p

## 개요
이해하기 쉬운 수준에서 MPEG-2를 처음 원리부터 설명하는 표준 해설서. 수학보다는 "평이한 영어로 프로세스를 설명"한다는 저자의 입장에 따라, 압축의 필요성·무손실·지각 부호화·압축 원리(제1장)를 서두에 배치하고, 오디오·비디오 신호 기초(샘플링·양자화·필터 설계, 제2장)→압축 처리(필터·DCT·위이블·움직임 보상, 제3장)→오디오 압축(MPG Audio Layer Ⅰ/Ⅱ/Ⅲ, Dolby AC-3, 제4장)→**MPEG-2 비디오 압축**(I/P/B 부호화, Elementary Stream, 코더·디코더, 제5장)→**프로그램 스트림과 트랜스포트 스트림**(PS, 타이밍, PSI, 뮴플렉싱, 제6장)으로 전개한다. 압축의 위험성(artifact)을 "불꽃놀이 비유"로 경고하는 등 실무 주의점을 많이 담은 실무형 매뉴얼이다 `[raw/books/mpeg-2-watkinson.md]`.

## 장 구조 (TOC 기반, 252p)
1. **Introduction to compression** — MPEG-2 개요·응용, 무손실·지각 부호화, 압축 원리, 오디오·비디오 압축 도구, profile/level, bitstream
2. **Fundamentals** — 오디오·비디오 신호, sampling·aliasing·PLL, 양자화·dither, binary code, 뮴플렉싱, packet·statistical multiplexing
3. **Processing for compression** — 필터(다운샘플링·QMF), Fourier, **DCT**, wavelet, **motion compensation** (block·gradient·phase correlation)
4. **Audio compression** — 심리음향(관요, critical band, beats), MPEG audio history, Layer Ⅰ/Ⅱ/Ⅲ, **Dolby AC-3**, stereo compression
5. **MPEG-2 video compression** — 시각 특성, progressive/interlaced, spatial·temporal redundancy, **I/P/B coding**, slice, **Elementary Stream**, coder·decoder, artifact, concatenation
6. **Program and transport streams** — packet·time stamps, transport stream, clock reference, **PSI**, multiplexing, remultiplexing

## 핵심 내용
- **부호화 원리**: lossless vs perceptual coding 구분; 공간·시간 중복도 reduction의 개념을 평이하게 제시 `[raw/books/mpeg-2-watkinson.md]`
- **DCT**를 Fourier transform → DCT → wavelet의 흐름으로 설명하고, MPEG-2 코더에서 어떻게 쓰이는지를 연결 `[raw/books/mpeg-2-watkinson.md]`
- **움직임 추정·보상**: block matching·gradient matching·phase correlation 3대 기법을 비교 `[raw/books/mpeg-2-watkinson.md]`
- **MPEG-2 비디오 부호화**: I/P/B 픽쳐, GOP, slice, interlaced 처리, elementary stream, bitstream 계위 `[raw/books/mpeg-2-watkinson.md]`
- **시스템**: program/transport stream의 구조, PCR/SCR, PSI(Program Specific Information), 뮴플렉싱 및 재뮴플렉싱 `[raw/books/mpeg-2-watkinson.md]`
- **실무 주의**: compression artifact 사례, "compression is a dangerous master" — 무분별한 압축의 위험 고발

## Related
- 저자: [[john-watkinson]]
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[rf-engineering]] · [[practical-digital-video-c]] (영상 프로그래밍 C 교재)
