---
title: Fractal Imaging (Ning Lu, 1997)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering, image-processing, image-compression]
sources: [raw/books/fractal-imaging.md]
confidence: high
---
# Fractal Imaging (Ning Lu, Academic Press 1997, 437p)

> 저자: **Ning Lu** (1963–, Texas A&M) — Iterated Systems Inc. 기술 기반.
> 출판: Academic Press, Inc., 1997 (ISBN 0-12-458010-6), 437p (pdfinfo). C/C++ 동반 코드(Iterated Systems Inc. 저작권, 설명·시위 amaç, 미컴파일 — 원서 p.8-9).
> 전제: 원서 표지 "Fractal Imaging — Ning Lu", "ACADEMIC PRESS, San Diego London Boston..." 확인.

## 개요
**fractal image compression**의 학술적·실무 종합서. IFS(iterated function system) 수학적 기반 → fractal image model(IFS code) → image partition · spatial search · clustering → realization → multiresolution(웨이브렛) · 영상 · color · entropy coding까지 12장 체계.

원서 인용:
- "For the last six years I have been dedicated to fractal image compression ... Fractal imaging, a mathematical wonder, has been transformed into commercial success" (Preface, p. xiii)
- "IFS decoding theorem" · "IFS encoding theorem" — Ch.2.4 (p. 13-19)
- "Quadtree code selection algorithm" — Ch.4.3 (p. 95)

## 장 구조 (12장, raw TOC 기반)
1. **Introduction: It's Magic** — fern·leaf, fractal, Cantor set, 자기비슷성 (raw p.1-10)
2. **Mathematical Foundation** — metric space, IFS(decoding/encoding 정리), recurrent IFS (raw p.11-43)
3. **Fractal Imaging Model** — fractal elements, square masking, **collage theorem** (raw p.44-90)
4. **Image Partition** — rate-distortion, **quadtree** partition (raw p.91-112)
5. **Spatial Transforms** — region search, seed image, VQ (raw p.113-138)
6. **Brightness & Contrast** — intensity/contrast scaling, Haar·DCT 비교 (raw p.139-172)
7. **Clustering Searching** — **Heckbert clustering** + C 구현 (raw p.173-204)
8. **Fractal Realization** — pixel training, pyramid, blowup, decompression (raw p.205-226)
9. **Multiresolution Decomposition** — Fourier/Haar/MRA, wavelet, fractal-wavelet hybrid (raw p.227-258)
10. **Images in Motion** — 3-D fractal compress, fractal video, H.263/MPEG-4 (raw p.259-276)
11. **Color Image** — colorimetry, color compress, fractal vector coding (raw p.277-292)
12. **Entropy Coding** — Huffman, arithmetic, fractal billiards, Burrows-Wheeler transform (raw p.293+)

## 핵심 기여
- **collage 정리** — IFS code 품질의 이론적 상한 (3.3, raw p.48-60)
- **Heckbert 클러스터링 알고리즘** — 블록 압축 실무 표준 (7.2, raw p.177-181)
- **fractal-wavelet hybrid** — MRA·PR quadrature filter 접목 (9.3, raw p.254-257)
- **분원-빌리어즈(Burrows-Wheeler) 변환** — entropy coding 장에서 제시 (12.4, raw p.321+)

## Related
- 개념: [[image-processing-fundamentals]], [[transform-coding]]
- 저자: Ning Lu (Texas A&M, Iterated Systems)
- 인접: [[image-video-compression-standards]] (JPEG/MPEG/H.261 기준), [[video-compression-mpeg]]
