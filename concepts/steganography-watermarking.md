---
title: 정보 은닉 · 스테그노그래피 · 워터마킹
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, steganography, watermarks, information-theory]
sources: [raw/books/information-hiding-steganography-watermarking.md, raw/books/mpeg2-source-code-commentary.md]
confidence: high
---
# 정보 은닉 · 스테그노그래피 · 워터마킹

디지털 미디어(이미지·오디오·비디오·문서)에 숨길 정보를 부호화하여 삽입하는 기술. 스테그노그래피 = 존재 자체를 감추는 비밀통신, 워터마킹 = 저작권 표식 삽입.

## 스테그노그래피 (Katzenbeisser & Petitcols, eds.)
- **3계층 프레임워크**: pure / secret key / public key steganography `[raw/books/information-hiding-steganography-watermarking.md]`
- **변환 도메인 기법**: DCT, DFT, wavelet, Mellin-Fourier domain
- **오디오 스테그노그래피**: acoustic masking, phase coding, echo hiding `[raw/books/information-hiding-steganography-watermarking.md]`
- **스테가놀랩시스**: signature detection, extraction, disabling
- **스핏 스펙트럼**: direct-sequence, frequency-hopping — 워터마킹에 병행 사용

## 워터마킹 (Katzenbeisser & Petitcols, eds.)
- **설계 3요소**: host location (crypto + psychovisual), workspace, bit formatting `[raw/books/information-hiding-steganography-watermarking.md]`
- **로버스트니스 공격**: noise & overmarking, compression, distortion, oracle, protocol, court-of-law
- **핑거프린팅**: statistical, collusion-secure, asymmetric, traitor tracing, anonymous
- **MPEG2 워터마킹**: MPEG 표준 내 워터마킹 적용 — 저작권 enforcement `[raw/books/mpeg2-source-code-commentary.md]`

## 공격·탐지·복원 요약
| 공격 유형 | 대응 | 소스 |
|---|---|---|
| Compression | 로버스트니스 설계 (error-correcting codes) | Ch 7 |
| Oracle attack | collusion-secure fingerprinting | Ch 8 |
| Protocol attack | asymmetric fingerprinting | Ch 8 |
| Court-of-law | legal protection, WIPO | Ch 9 |

## 관련
- [[information-hiding-steganography-watermarking]] — 핵심 소스 (Katzenbeisser & Petitcols, 2000)
- [[mp3-perceptual-coding]] — 오디오 마스트리핑 기반 스테그노그래피
- [[digital-audio-mp3-encoder]] — MP3 내 워터마킹 (acoustic masking)
- [[a-course-in-dsp]] — DSP 이론
- [[mpeg2-source-code-commentary]] — MPEG2 워터마킹 (동일 클러스터)
