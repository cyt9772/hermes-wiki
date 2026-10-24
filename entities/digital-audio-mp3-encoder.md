---
title: 디지털 오디오의 이해 — MP3 부호화기 (송종관 2000)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, mp3-audio-coding, mpeg-standard, signal-processing]
sources: [raw/books/digital-audio-mp3-encoder.md]
confidence: high
---
# 디지털 오디오의 이해 — MP3 부호화기 (송종관 2000)

> 표지/원저: 송종관
> 출판: 나남출판 (경성대학교 멀티미디어 연구총서), 2000, 169p

## 개요
이 책은 디지털 오디오 신호 부호화(부호화=encoding)의 이해를 돕기 위해 출간된 한국어 해설서로, 압축 부호화 개념 → 정보압축 국제표준 → MPEG → MPEG 오디오(MP3) → MP3 활용의 흐름으로 구성된다 `[raw/books/digital-audio-mp3-encoder.md]. 제4장에서 MPEG 오디오의 3개 레이어(레이어 1/II/III)와 MUSICAM·ASPEC 알고리즘을 소개하고, 청각심리 원리·청각심리 모델·서브밴드 필터링·MDCT를 압축 원리로 서술한다. 레이어 III(=MP3)의 비트할당/스케일팩터 구조(한 프레임 32×3×12 = 1152 샘플)까지 기술한다. 제5장은 MP3 파일 헤더·사이드 정보·메인 데이터 구조와 CD→WAV, WAV→MP3 등 실전 제작 예제(윈앰프 등)를 다룬다 `[raw/books/digital-audio-mp3-encoder.md].

## 장 구조 (TOC 기반, 169p)
1. **제1장 멀티미디어** — 개념, 특징, 전망, 응용(원격화상회의·의료·교육·VOD·대화형TV 등)
2. **제2장 정보압축의 국제표준** — 무손실/손실 압축 혼성·엔트로피 부호화, 부호화 역사, ITU/ISO/IEC/TTA 표준화
3. **제3장 MPEG** — MPEG-1/2, 표준 구성(비디오·오디오·시스템), H.261/JPEG 배경, MPEG-4
4. **제4장 MPEG 오디오** — 레이어 1/II/III, MUSICAM·ASPEC, 청각심리 원리·모델·서브밴드·MDCT, 파일 구조(헤더·사이드·메인)
5. **제5장 MP3의 활용** — MP3 플레이어, 파일 제작(CD→WAV, WAV→MP3, CD→MP3), 관련 사이트

## 핵심 내용
- **손실 압축 부호화의  기본**: "안 들리는 정보는 빼버린다"는 원리, 전 마스킹 등 청각심리 기반 압축 `[raw/books/digital-audio-mp3-encoder.md]
- **레이어 I/II 구조 차이**: 레이어 I은 32 서브밴드×3 블록×12 샘플(1152 샘플), 레이어 II/III는 비트할당·스케일팩터 보완 구조
- **MUSICAM·ASPEC 통합**: 14개 제안 중 MUSICAM과 ASPEC 우수 → 두 그룹 통합 초안 표준(AES 표준에 반영)
- **MDCT·서브밴드 필터링**: 압축 원리 핵심 단위로 서술 `[raw/books/digital-audio-mp3-encoder.md]
- **MP3 파일 구조**: 헤더(111p 기준), 사이드 정보, 메인 데이터 분해 설명

## 관련
- [[mp3-perceptual-coding]] — MP3·주지청각 부호화
- [[audio-processing-soundforge-vegas]] — 오디오 처리 실무(Sound Forge/Vegas)
- [[a-course-in-dsp]] — DSP 이론 기초
- [[steganography-watermarking]] — MP3 내 워터마킹 관련
