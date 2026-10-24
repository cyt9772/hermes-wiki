---
title: Video Coding: An Introduction to Standard Codecs (Ghanbari 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, video-compression, h-261, mpeg-standard]
sources: [raw/books/video-coding-standard-codecs.md]
confidence: high
---
# Video Coding: An Introduction to Standard Codecs (Ghanbari 1999)

> 표기/원저: **Mohammed Ghanbari**
> 출판: The Institution of Electrical Engineers, 1999 (IEE Telecommunications Series 42, ISBN 0 85296 762 4), 271p

## 개요
영상 부호화 표준 코덱을 **역사·기본 원리·표준별 코덱** 3단으로 정리한 표준 해설서. 표준화 역사(제1장) → 비디오 기초(아날로그·디지털, SIF/CIF/QCIF/HDTV 형식, picture quality assessment, 제2장) → **압축 원리**(공간 redundant: predictive/transform coding·fast DCT, quantisation, 시간 redundant: motion estimation·hierarchical ME, VLC: Huffman·arithmetic, generic interframe codec, 제3장) → 표준별 코덱(Chapter 4-9: JPEG, H.261, MPEG-1, MPEG-2, H.263, MPEG-4, MPEG-7 preview)으로 전개 `[raw/books/video-coding-standard-codecs.md]`. 표준 코덱(H.261→MPEG-1→MPEG-2→H.263→MPEG-4)을 단일 프레임워크 안에서 비교하는 데 강점이 있다.

## 장 구조 (TOC 기반, 271p)
1. **History of video coding** — 표준화 역사
2. **Video basics** — 아날로그·디지털, 이미지 형식 (SIF/CIF/QCIF/HDTV/film/temporal resampling), picture quality
3. **Principles of video compression** — 공간·시간 redundant, DCT·fast DCT, quantisation, ME·hierarchical ME, VLC (Huffman·arithmetic), generic codec
4. **Coding of still pictures (JPEG)** — lossless·lossy, baseline, run-length, hierarchical, **JPEG-2000** preview
5. **Coding for video conferencing (H.261)** — MC/NO-MC·inter/intra decision, forced updating, 2-D VLC, loop filter, rate control
6. **Coding of moving pictures for digital storage media (MPEG-1)** — systems coding, GOP, picture structure
7. **Coding of high quality moving pictures (MPEG-2)** — 고화질 표준
8. **Coding for low bit rates (H.263)** — advanced inter/coding, PB-frame, deblocking filter, ATM, scalability (temporal/SNR/spatial/multilayer), H.263L
9. **Content-based video coding (MPEG-4)** — VOP, segmentation, shape coding, ME/MC, texture coding, still images·wavelet (EZW/SPIHT), MPEG-7 preview
+ Appendix A: fast DCT 'C' program / B-D: JPEG·shape coding tables

## 핵심 내용
- **부호화 원리**: spatial·temporal redundancy reduction + entropy coding을 3원칙으로 정리, generic interframe codec 구조화 `[raw/books/video-coding-standard-codecs.md]`
- **DCT/quantisation/VLC**를 표준별 코덱 모두에 공통 적용하는 통일 프레임워크 제시 `[raw/books/video-coding-standard-codecs.md]`
- **H.261** 코덱 — MC/NO-MC decision, forced updating, 2-D VLC, loop filter, rate control `[raw/books/video-coding-standard-codecs.md]`
- **MPEG-1/2** 표준 — GOP, picture structure, systems coding, high quality extension `[raw/books/video-coding-standard-codecs.md]`
- **H.263** — advanced inter coding, PB-frame, deblocking, error protection, scalability, ATM 전송 `[raw/books/video-coding-standard-codecs.md]`
- **MPEG-4** — VOP, shape coding, texture coding, synthetic objects, still image coding (EZW/SPIHT wavelet) `[raw/books/video-coding-standard-codecs.md]`

## Related
- 저자: [[mohammed-ghanbari]]
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[image-processing-fundamentals]] (C2 cluster) · [[dct-algorithms-applications]]
