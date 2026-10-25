---
title: MPEG 비디오 (대우전자 영상연구소, 1995)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, video-compression, mpeg-standard]
sources: [raw/books/mpeg-video.md]
confidence: high
---
# MPEG 비디오 (대우전자 영상연구소, 1995)

> 저자: **대우전자 영상연구소** (집단 저자 — 단체. 원문: "대우천자 영상연구소 지음"[OCR, 대우전자]). 머리말 서명: "1995년 7월, 대우전자 유시룡 상무"
> 출판: 1995 (연암출판 계열 — 원문 감사문 "연암책만들기의 유정룡 주간")
> 원문 머리말: "MPEG은 부호기쪽은 언급하지 않고 **복호기 쪽만의 표준**을 정했기 때문에 더욱 어렵게 보일 수 있다. 이 책은 MPEG표준 중 영상압축 부분을 소화한 후 쉽게 풀어서 설명했다. **MPEG(1)은 MPEG-2의 부분집합**으로서 완전 호환성을 갖고 있어 MPEG-2를 이해하면 MPEG-1은 자연스럽게 이해할 수 있다."

## 개요
1990년대 초 한국에서 출판된 **MPEG-2 영상 부호화 표준** 기술서. "MPEG에서 정의한 용어나 매개변수는 그대로 영어로 썼으며, 표들도 MPEG 표준에 있는 표를 그대로 이용" — 표준규격서(IS 11172/13819 계열, 복호기 쪽)의 **표·syntax**를 한국어 해설과 함께 재구성한 실무서. MPEG-1을 MPEG-2의 부분집합으로 다루어, MPEG-2 기준의 단일 서술이 특징. 부록 2에 **elementary stream 예**를 수록.

## 내용 구성 (원문 TOC·표 기반, 308p)
1. **MPEG 개요** — 압축 표준화(1988 회의 시작), CD Video·VOD·무궁화위성, MPEG-1 = MPEG-2 부분집합
2. **영상 프레임** — I/P/B picture, frame/field, progressive, **dual prime**, **GOP**, temporal prediction, **resampling**, **Deinterlacing**
3. **부호화·복호화** — **가변장 부호화(VLC)**, **역양자화**, DCT(`dct type`), skipped macroblocks
4. **Syntax** — sequence/picture header, extension, **quant matrix**, **slice extension**, **macroblock modes**, marker bit
5. **motion compensation** — 16x8 prediction, forward/backward motion vector, **DMV**(delta), dual prime, reference frame 선택
6. **DCT coefficient** — run/level coding, `coded_block_pattern`, **DC/AC coefficient tables**, intra·non-intra, chroma
7. **Profile·Level** — **Simple/Main/SNR/Spatially/High** profile, scalable layer(base/enhancement), `vbv_delay`, **VBV buffer**, `constrained_parameters_flag`
8. **Video format** — CCIR 601, PAL/SECAM/NTSC, SMPTE 170M/240M, ITU-R BT.470-2, `chroma_format`
9. **부록** — 부록 2: **MPEG2 elementary stream 예**; 참고 문헌(Netravali·Haskell, Didier Le Gall, T. Sikora, A. Pun, M. Iwahashi 등)

## 핵심 기여
- **복호기(디코더) 관점**의 MPEG-2 표준 — "복호기 쪽의 표준"을 한국어로 재구성.
- **MPEG-1 = MPEG-2 부분집합** 논리로 단일 서술.
- **표·syntax 그대로** — MPEG 표준에서 정의한 표를 그대로 사용(머리말).
- **profile/level + scalable layers** — Simple/Main/SNR/Spatial/High, base/enhancement layer, **VBV buffer**, **DMV/dual prime**.

## Related
- 저자: 대우전자 영상연구소 (단체 — 이 wiki에 저자 entity 없음)
- 개념: [[video-compression-mpeg]] · [[video-compression-standards-korea]] · [[video-coding-standard-codecs]]
- 인접: [[mpeg-2-watkinson]] · [[mpeg2-source-code-commentary]] · [[mpeg-system-korea]] · [[digital-video-engineering-korea]] · [[transform-coding]] · [[mp3-perceptual-coding]]

## OCR/추출 신뢰도
- 한글 OCR 일부 토큰 깨짐(한자형 혼입) — 표준 표 번호(표 4-4, 5-8, 6-10, 6-30~6-55 등)와 식 번호·문맥으로 cross-check.
