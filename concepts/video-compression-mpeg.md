---
title: 영상 압축 표준 (Video Compression — MPEG/H.261 계열)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, video-compression, mpeg-standard, h-261]
sources: [raw/books/mpeg-2-watkinson.md, raw/books/video-coding-standard-codecs.md, raw/books/mpeg-system-korea.md, raw/books/mpeg2-source-code-commentary.md, raw/books/video-compression-standards-korea.md, raw/books/digital-video-engineering-korea.md, raw/books/video-communication-signal-processing.md]
confidence: high
---
# 영상 압축 표준 (Video Compression — MPEG/H.261 계열)

영상 신호의 공간적·시간적 중복도(공간 adjacent 유사성·인접 프레임 similarity)를 제거하여 전송/저장 대역을 줄이는 부호화 기술과 이를 규정한 표준 체계. 표준화 세대는 **H.261(ITU-T, video conference) → MPEG-1(ISO, 저장매체) → MPEG-2(고화질/방송) → H.263(초저속) → MPEG-4(컨텐츠 기반)** 의 흐름으로 이어지며, 공통 원리는 **예측(DPCM/MC) + 변환(DCT) + 양자화 + entropy coding(Huffman/산술)**이다.

## 공통 부호화 프레임워크

- **공간 중복도 제거**: predictive coding(차이 분호화, DPCM 뿌리) 또는 transform coding(2D DCT) + HVS(인간 시각) 하중 양자화 `[raw/books/video-coding-standard-codecs.md]`
- **시간 중복도 제거**: 움직임 추정(block matching 등) + 움직임 보상(motion compensation), 움직임 벡터 분호화 `[raw/books/digital-video-engineering-korea.md]`
- **Entropy coding**: run-length(Huffman) + optional 산술 부호화 `[raw/books/video-communication-signal-processing.md]`
- **표준 코덱 공통 구조**: interframe loop = motion estimator → inter/intra switch → DCT → quantiser → VLC → IQ/IDCT → buffer (generic interframe codec) `[raw/books/video-coding-standard-codecs.md]`
- **DCT 기반**: Fourier → DCT(에너지 집중) → quantize → zigzag scan → VLC; MPEG-2 코더/디코더 파이프라인의 핵심 `[raw/books/mpeg-2-watkinson.md]`

## 표준별 특징

### MPEG-1 (저장매체)
- SIF 기반, GOP·I/P/B 픽쳐 구조, D 픽쳐(디스크) 지원 `[raw/books/digital-video-engineering-korea.md]`
- systems coding(뮴플렉싱·sync)과 비디오 코딩 분리, video conference와 storage media의 중간 수준 `[raw/books/video-coding-standard-codecs.md]`

### MPEG-2 (고화질/방송)
- **Profil/Level**(주사방식·해상도·bitrate·bitstream limit 조합)으로 다양한 응용(Digital TV, DVB, DCP) 지원 `[raw/books/mpeg-2-watkinson.md]`
- **Elementary Stream → Program Stream(저장) / Transport Stream(전송)** 이중 구조; TS는 188-byte 고정 패킷 + PSI(Packetized System Information) + PCR/SCR 타이밍 + T-STD/P-STD 정합 모델 `[raw/books/mpeg-system-korea.md]`
- 계위(스케일러빌리티) 부호화: 공간·SNR·시간 계위 `[raw/books/digital-video-engineering-korea.md]`
- 소스 수준 구현: TM5 test model — read frame → motion estimation → predict → DCT → quantize → VLC → rate control (부호기) / getbits → header → block → IDCT → display (복호기) `[raw/books/mpeg2-source-code-commentary.md]`
- 움직임 벡터 dual prime, chroma vector scaling, half-pel interpolation, skipped macroblock 등 세부 구현 `[raw/books/mpeg2-source-code-commentary.md]`

### H.261 (video conference)
- CIF(공통 중간 포맷) 320x240 기준, N x CIF (N=1..30) bitrate scaling `[raw/books/digital-video-engineering-korea.md]`
- MC/NO-MC decision, inter/intra decision, forced updating, 2-D VLC, loop filter, bit-rate control `[raw/books/video-coding-standard-codecs.md]`
- 계층적 다중화(hierarchical multiplex)로 bit-rate 변동 대응 `[raw/books/digital-video-engineering-korea.md]`

### H.263 (초저속)
- advanced inter coding(2 VLC table switching), PB-frame mode, deblocking filter, UV(unrestricted Vop) 모드로 64kbit/s 이하 저속 부호화 최적화 `[raw/books/video-coding-standard-codecs.md]`
- VBV(Video Buffer Verifier) 기반 HRD(Host Requirements Description) + TMN5 rate control + Telenor bit-rate control `[raw/books/digital-video-engineering-korea.md]`
- ATM 네트워크 전송·loss concealment·packetization 영향 분석 `[raw/books/video-coding-standard-codecs.md]`

### MPEG-4 (컨텐츠 기반)
- **VOP(Video Object Plane)** — 장면 내 객체를 단위로서 부호화; shape coding(alpha plane, chain code, quadtree) `[raw/books/video-coding-standard-codecs.md]`
- texture coding(shape-adaptive DCT), motion ME/MC, synthetic object(합성) coding `[raw/books/video-coding-standard-codecs.md]`
- still image coding: discrete wavelet + EZW(Embedded Zero-Tree Wavelet) + SPIHT(Set Partitioning in Hierarchical Trees) `[raw/books/video-coding-standard-codecs.md]`
- MPEG-7(멀티미디어 컨텐트 서술 인터페이스)로 이어지는 방향 `[raw/books/video-coding-standard-codecs.md]`

## 표준화 역사

| 시대 | 표준 | 목적 | 특징 |
|---|---|---|---|
| 1988~ | **ITU-T H.261** | video conference (56-2048kbit/s) | CIF, N x CIF, loop filter, bit-rate control |
| 1990s 초 | **ISO MPEG-1** | 저장매체(VCD, Digital Storage) | SIF, GOP I/P/B/D, 1.5Mbit/s |
| 1994 | **ISO MPEG-2** | 방송/고화질/DVB | HD, TS/PS, Profiles/Levels, DVB/DVB-S, DCP |
| 1996 | **ITU-T H.263** | 저속 video conference/PSTN | UV, PB-frame, SAC, VBV |
| 1999~ | **ISO MPEG-4** | 컨텐츠 기반, object-based | VOP, shape coding, wavelet |
| 2000s | **ISO MPEG-7** | 컨텐트 서술 | metadata, retrieval |

*(H.261 → MPEG-1/2 → H.263 → MPEG-4 → MPEG-7 의 시대순 진행; H.261 = ITU-T, MPEG-1/2/4/7 = ISO/IEC JTC1/SC29/WG11)* `[raw/books/video-compression-standards-korea.md]`

## 핵심 비교

| 항목 | H.261 | MPEG-1 | MPEG-2 | H.263 | MPEG-4 |
|---|---|---|---|---|---|
| 목적 | video conference | 저장매체 | 방송/고화질 | 저속 conference | 컨텐츠 기반 |
| 기본 단위 | frame | frame | frame | frame | **VOP** |
| 포맷 | CIF | SIF | HD 포함 | sub-CIF~QCIF | object-based |
| bit-rate | 56-2048k | ~1.5M | 4-20M (HD까지) | <64k~2M | 가변 |
| 계위 | — | — | spatial/SNR/temporal | — | spatial/temporal |

## 관련
- [[mpeg-2-watkinson]] · [[video-coding-standard-codecs]] · [[mpeg-system-korea]] · [[mpeg2-source-code-commentary]] · [[video-compression-standards-korea]] · [[digital-video-engineering-korea]] · [[video-communication-signal-processing]]
- 인접: [[image-processing-fundamentals]] (C2 cluster) · [[dct-algorithms-applications]] · [[a-course-in-dsp]]
