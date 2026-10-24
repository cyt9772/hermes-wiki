---
title: C 언어 영상통신의 신호처리 (문호 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-processing, signal-processing, video-compression]
sources: [raw/books/video-communication-signal-processing.md]
confidence: high
---
# C 언어 영상통신의 신호처리 (문호 1999)

> 표기/원저: **문호** (원서명 확인 필요 — 머리말의 "Moon Ho Lee 등" 표기)
> 출판: 대영사, 1999 (머리말 1999. 2. 20; 전신 1994『C 언어를 이용한 영상신호처리』 대영사), 524p

## 개요
영상처리를 **수식이 아닌 C 언어 프로그램** 중심으로, 결과를 눈으로 확인하며 배우게 구성한 실무 교재. 1994년 전작(대영사)을 대폭 수정·보완한 판. 크게 3부 — **1부 영상 처리의 기초**(영상처리 개요·이진영상 경계값·히스토그램·윤곽·미분, 잡음 제거·미디언 필터, 기하학적 변환, 영상 압축: DFT·Huffman·DCT·Hadamard·산술 부호화, 제1-6장) → **2부 영상 압축 표준**(정지영상 JPEG, 동영상: Wavelet·**MPEG-1/2/4/7**, 제7-8장) → **3부 멀티미디어 서비스**(개요·통신망 기술·제공 서비스, 제9-11장)로 구성, 부록으로 HomePage 디자인을 실었다 `[raw/books/video-communication-signal-processing.md]`.

## 장 구조 (TOC 기반, 524p)
1부 — 영상 처리의 기초와 이해
1. **영상 처리란 무엇인가** — 영상 종류·디지털 영상, 표본화·양자화, C 함수
2. **이진 영상 처리(I)** — 경계값, 히스토그램 평활화, dithering
3. **이진 영상 처리(II)** — 윤곽, 미분에 의한 영상 처리
4. **잡음 제거** — 평활화, 미디언 필터, 이진 영상 잡음 제거
5. **영상 데이터의 기하학적 처리** — 크기·위치·회전 변환
6. **영상 데이터의 압축** — DFT·2차원 푸리에, 가역·비가역, RLC·DPCM·Huffman, **DCT 압축**, Hadamard, 산술 부호화
2부 — 영상 압축 표준
7. **정지 영상 압축 부호화 (JPEG)**
8. **동영상 부호화 (Wavelet, MPEG-1/2/4/7)**
3부 — 멀티미디어 서비스
9. **멀티미디어 서비스 개요** · 10. **멀티미디어 통신망 기술** · 11. **멀티미디어 제공 서비스**
+ 부록: HomePage 디자인

## 핵심 내용
- **C 언어 중심 실무**: 각 장에 MAIN PROGRAM과 연습문제를 실어 결과를 직접 확인하게 구성 `[raw/books/video-communication-signal-processing.md]`
- **압축 기초**: DFT·Huffman·DCT·Hadamard·산술 부호화를 모두 C로 구현 `[raw/books/video-communication-signal-processing.md]`
- **표준 부호화**: JPEG(정지) + Wavelet·MPEG-1/2/4/7(동영상)을 2부에 집중 처리 `[raw/books/video-communication-signal-processing.md]`
- **멀티미디어 서비스/통신망**: 3부에서 서비스·통신망 수준까지 확장 `[raw/books/video-communication-signal-processing.md]`

## Related
- 저자: [[moon-ho]]
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[image-processing-fundamentals]] (C2 cluster) · [[video-coding-standard-codecs]] · [[mpeg2-source-code-commentary]]
