---
title: Image and Video Compression Standards (Bhaskaran & Konstantinides 1995)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering, image-processing, video-compression, image-compression, dsp]
sources: [raw/books/image-video-compression-standards.md]
confidence: high
---
# Image and Video Compression Standards: Algorithms and Architectures (1995)

> 저자: **Vasudev Bhaskaran** (Hewlett-Packard Laboratories), **Konstantinos Konstantinides** (Hewlett-Packard Laboratories)
> 출판: **Hewlett-Packard Laboratories / Kluwer Academic Publishers**, 1995 (2nd printing 1996), 371p (pdfinfo)
> scope: JPEG, MPEG-1/2, H.261, MPEG/Dolby AC-3 audio, wavelets/VQ
> 원서 인용: "This book presents an introduction to the algorithms and architectures that form the underpinnings of the image and video compression standards, including JPEG (compression of still-images), H.261 (video teleconferencing), and MPEG-1 and MPEG-2 (video storage and broadcasting)." (Preface, p. xiii)
> 원서 인용: "The JPEG standard specifies four modes of operation: sequential DCT-based, progressive DCT-based, lossless, and hierarchical." (Ch.5, p. 137)

## 개요
**JPEG · MPEG-1/2 · H.261 · Dolby AC-3** 표준의 알고리즘과 하드웨어 아키텍처를 한 권에 정리한 실무서. 1990년대 HP Labs의 영상 코덱 개발 경험을 배경으로 작성. 16개 장 + 부록 + glossary. `^[raw/books/image-video-compression-standards.md]`

## 장 구조 (16장, 371p — TOC 기반)
1. **Compression Fundamentals** — rate-distortion, predictive coding (p.1)
2. **Lossless** — Huffman(Voorhis), arithmetic, Group 3/4, JBIG (p.15)
3. **Lossy Image** — DCT coding, fast DCT (p.53)
4. **Lossy Video** — motion estimation/compensation (p.87)
5. **The JPEG Standard** — 4 modes, quant tables, entropy (p.129)
6. **The MPEG Video Standards** — MPEG-1 & MPEG-2 (p.161)
7. **H.261** — video telephony (p.195)
8. **Processing Requirements** — complexity, load (p.207)
9. **RISC and DSP Cores** (p.215)
10. **Architectures for DCT** — vector, distributed arithmetic (p.225)
11. **Motion-Compensation Architectures** (p.235)
12. **JPEG Decoder Architectures** (p.249)
13. **MPEG Decoder Architectures** (p.260)
14. **MPEG Encoder Architectures** (p.272)
15. **Audio** — MPEG & Dolby AC-3, perceptual model, psychoacoustics (p.285)
16. **Future Directions** — wavelets, VQ, fractal, set partitioned (p.305)

## 핵심
- **Rate-Distortion Theory** — 압축 이론의 기초 (1.5, p. 5-7)
- **Motion Estimation (2-D, sub-pel)** — Ch.4, p.87-120
- **DCT-based coding + quantization + entropy** — Ch.3-5
- **Distributed Arithmetic & Wallace tree** — DCT/MDCT/ACOUSTIC 하드웨어 (Ch.10, p.225+)
- **Psychoacoustics** — Ch.15, p. 311-330

## Related
- 개념: [[video-compression-mpeg]], [[transform-coding]], [[image-processing-fundamentals]]
- 저자: Vasudev Bhaskaran (HP Labs)
- 인접: [[mpeg-video]] (MPEG-2 codec), [[mpeg2-source-code-commentary]] (MPEG-2 decoder), [[fractal-imaging]] (fractal compression)
