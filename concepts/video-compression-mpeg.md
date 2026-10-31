---
title: 영상 압축 표준 (Video Compression — MPEG/H.261 계열)
created: 2026-10-24
updated: 2026-10-31
type: concept
tags: [engineering, video-compression, mpeg-standard, h-261]
sources: [raw/books/mpeg-2-watkinson.md, raw/books/video-coding-standard-codecs.md, raw/books/mpeg-system-korea.md, raw/books/mpeg2-source-code-commentary.md, raw/books/video-compression-standards-korea.md, raw/books/digital-video-engineering-korea.md, raw/books/video-communication-signal-processing.md, raw/books/h264-avc-video-compression.md, raw/books/hdtv-theory-technology.md, raw/books/applied-mpeg-fig.md, raw/books/latest-mpeg-fig.md, raw/books/mpeg-theory-miki.md, raw/books/dsp-video.md]
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

## H.264/AVC — 차세대 (2007 배치)

### H.264/AVC 비디오 압축 (大久保 榮 외, 2007 개정, 419p)
- 기존 H.261→MPEG-1/2→H.263→MPEG-4 흐름에서 **H.264/AVC 세대를 독립 교재**로 위치 `[raw/books/h264-avc-video-compression.md]`
- **CABAC/CAVLC**(변형 entropy coding)·**deblocking filter**·**VBV rate control**·GOP 구조 — MPEG-2/H.263 대비 효율 개선 `[raw/books/h264-avc-video-compression.md]`
- 모바일 TV 5개 방식(DMB·DVB·MediaFLO·ISDB-T·MBMS)의 bitrate·해상도·latency 비교 — 2005-07 정책 기술 백서 `[raw/books/h264-avc-video-compression.md]`
- HD 1080p HD-DVD vs Blu-ray codec 비교 + 차세대 셋톱박스(IPTV) 활용 `[raw/books/h264-avc-video-compression.md]`
- 인접: [[steganography-watermarking]] (H.264 워터마킹) · [[mp3-perceptual-coding]] (오디오 코덱 병행)

## HDTV — HD 방송 시스템 (2000 배치)
- **HDTV 이론과 기술 (대한전자공학회, 2000)** — 고해상도·고주사율(100Hz)·1250선·wide-gamut·16:9, NTSC 대비 비교가 제1축 `[raw/books/hdtv-theory-technology.md]`
- HD 방송: **DVB/ATSC/ISDB-T**, 모바일 TV 표준(DMB·DVB-H·MBMS) — 2000년대 초기 HD·모바일 방송 전환기 총서 `[raw/books/hdtv-theory-technology.md]`
- 디스플레이: PDP·LCD·DLP·CRT, color space(YUV vs YCbCr), bit depth — HD 디스플레이 산업 배경 `[raw/books/hdtv-theory-technology.md]`
- 영상 압축 표준과 HD 전송의 연결점 — HD급 bitrate을 줄이는 코덱과 디스플레이가 만난 지점

## MPEG 표준화 실무 (일본 원저 3권, 1995-99 배치 추가)
### 그림으로 보는 응용 MPEG / 최신 MPEG (藤原洋 supervision, 1995)
- **응용 MPEG** — MPEG 오디오(·음성) 응용 CD·방송·통신, MPEG 비디오/모션 부호화 응용 DVD·브로드캐스팅, MPEG-4/7 신세대 표준 + 산업 적용 `[raw/books/applied-mpeg-fig.md]`
- **최신 MPEG** — MPEG 표준화 과정(ISO/IEC 11172·13811) 역사적 흐름, MPEG-1/2 구조(시스템·오디오·비디오 계층), MPEG-4 기초 + 산업 응용(리코·NTT·Sony) `[raw/books/latest-mpeg-fig.md]`

### MPEG-4의 세계 (三木弼一, 1999)
- MPEG 부호화 표준 구조 — 영상·음성 공동 부호화 프레임워크 `[raw/books/mpeg-theory-miki.md]`
- **MPEG-4 객체 기반(오브젝트) 부호화 모델** — ISO 표준화 논의와 병행 `[raw/books/mpeg-theory-miki.md]`
- 산업계(마쓰시타 등) 관점의 응용 장 — 표준화 현장 기술 `[raw/books/mpeg-theory-miki.md]`

## 영상 신호처리 (DSP × Video 접점)
- **영상을 이용한 디지털 신호처리 (엄민영·김성제 2014)** — 2D 공간 신호·주파수 평면·DCT/2D-DFT, 영상 압축·부호화(MJPEG 계열), 운동 보정까지 영상 특화 DSP `[raw/books/dsp-video.md]`
- 인접: [[image-processing-fundamentals]] (2D 영상 처리) · [[transform-coding]] (DCT 기반) · [[mp3-perceptual-coding]] (오디오 코덱)

## 관련
- [[mpeg-2-watkinson]] · [[video-coding-standard-codecs]] · [[mpeg-system-korea]] · [[mpeg2-source-code-commentary]] · [[video-compression-standards-korea]] · [[digital-video-engineering-korea]] · [[video-communication-signal-processing]]
- H.264/HD: [[h264-avc-video-compression]] · [[hdtv-theory-technology]] · [[applied-mpeg-fig]] · [[latest-mpeg-fig]] · [[mpeg-theory-miki]] · [[dsp-video]]
- 인접: [[image-processing-fundamentals]] (C2 cluster) · [[dct-algorithms-applications]] · [[a-course-in-dsp]]
