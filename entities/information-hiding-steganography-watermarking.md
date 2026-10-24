---
title: Information Hiding Techniques for Steganography and Digital Watermarking (Katzenbeisser & Petitcols 2000)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, steganography, watermarks, information-theory]
sources: [raw/books/information-hiding-steganography-watermarking.md]
confidence: high
---
# Information Hiding Techniques for Steganography and Digital Watermarking (Katzenbeisser & Petitcols, eds., 2000)

> 표지/원저: Stefan Katzenbeisser & Fabien A. P. Petitcols (editors)
> 출판: Artech House, Inc. (Artech House Computer Security Series, series editor Rolf Oppliger), 2000, ISBN 1-58053-035-4, 235p

## 개요
정보 은닉(information hiding) 분야 — 스테그노그래피(steganography)와 디지털 워터마킹(digital watermarking) — 의 최신 기술을 집대성한 학술 모음집이다. Part I(Ch.1–4)은 스테그노그래피 원리·표적기법·스테가노랩시스(steganalysis)를, Part II(Ch.5–9)는 워터마킹 원리·기법·로버스트리스·핑거프린팅·인터넷 저작권을 다룬다 `[raw/books/information-hiding-steganography-watermarking.md]`. DCT/DFT/웨이브렛/멜린-푸리에 변환 도메인 워터마킹, 스핏 스펙트럼(직계 확산·주파수호핑), 펄프로그·오라클 공격, 코럴루션-시큐어(AES)핑거프린팅까지 폭넓게 다루며, 오디오(음향마스트리핑·에코히딩·페이즈코딩) 분야 스테그노그래피도 포함한다.

## 장 구조 (TOC 기반, 235p)
1. **Ch. 1** Introduction to information hiding (underground)
2. **Ch. 2** Principles of steganography — secret communication framework, security, noisy data
3. **Ch. 3** Survey of steganographic techniques — DCT, phase coding, echo hiding, spread spectrum, statistical
4. **Ch. 4** Steganalysis — detection, extraction, disabling
5. **Ch. 5** Introduction to watermarking — principles, applications, requirements, evaluation
6. **Ch. 6** Survey of current watermarking — DFT/DCT/Mellin-Fourier/wavelet domain, spread spectrum merging, fractal
7. **Ch. 7** Robustness of copyright marking systems — signal diminishment, detector failure, counterfeiting attacks
8. **Ch. 8** Fingerprinting — statistical/collusion-secure/asymmetric/traitor tracing/anonymous
9. **Ch. 9** Copyright on the Internet and watermarking — WIPO, legal protection, privacy

## 핵심 내용
- **스테그노그래피 3계층**: pure / secret key / public key steganography framework `[raw/books/information-hiding-steganography-watermarking.md]`
- **워터마킹 설계 3요소**: host location (crypto + psychovisual), workspace (DCT/DFT/wavelet), bit formatting (spread spectrum/ECC)
- **로버스트니스 공격 분류**: noise & overmarking, compression, distortion, oracle, protocol, court-of-law
- **핑거프린팅**: collusion-secure, asymmetric, traitor tracing — 저작권 enforcement 핵심 기법
- **오디오 스테그노그래피**: acoustic masking properties, phase coding in digital sound, echo hiding `[raw/books/information-hiding-steganography-watermarking.md]`

## 관련
- [[steganography-watermarking]] — 정보 은닉·워터마킹 개념
- [[mp3-perceptual-coding]] — 오디오 마스트리핑 기반
- [[a-course-in-dsp]] — DSP 이론
- [[mpeg2-source-code-commentary]] — MPEG 워터마킹 관련(동일 클러스터)
