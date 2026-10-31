---
title: MP3 · 주지청각(Perceptual) 부호화
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, mp3-audio-coding, signal-processing, mpeg-standard]
sources: [raw/books/digital-audio-mp3-encoder.md, raw/books/audio-processing-soundforge-vegas.md, raw/books/multimedia-signal-processing.md]
confidence: high
---
# MP3 · 주지청각(Perceptual) 부호화

사람의 청각 모델에 기반한 손실 오디오 부호화 — "사람이 듣지 못하는 정보를 압축한다"는 원리로, 저대역폭으로 오디오 신호를 전송·저장한다.

## MPEG 오디오 구조 (digital-audio-mp3-encoder)
- **레이어 1/II/III**: 프레임 1152 샘플(32 서브밴드×3 블록×12 샘플) 기반. 레이어 III = MP3 `[raw/books/digital-audio-mp3-encoder.md]`
- **MUSICAM·ASPEC**: 14개 제안 중 우수 → 통합 초안(AES/ITU 표준에 반영)
- **청각심리 원리**: 전 마스킹(pre-masking) 등 — 안 들리는 성분 제거
- **청각심리 모델**: 청각 모델 기반 비트할당
- **서브밴드 필터링·MDCT**: 스펙트럼 분해 핵심 도구
- **MP3 파일 구조**: 헤더 + 사이드 정보 + 메인 데이터 `[raw/books/digital-audio-mp3-encoder.md]`

## 실전 렌더링 (audio-processing-soundforge-vegas)
- **렌더링 출력 형식**: Wave(MP3), Streaming, AVI, MP3 — 출력 설정에 따라 형식 선택 `[raw/books/audio-processing-soundforge-vegas.md]`
- **음질보정 효과**: Equalizer·Compressor — MP3 부호화와 동일한 주파수 영역 작업
- **파일 변환**: Bit-Depth·Channel·Resample·Time Stretch — 출력 비트율을 조절하는 수단 `[raw/books/audio-processing-soundforge-vegas.md]`

## 핵심 요약
| 요소 | 내용 | 소스 |
|---|---|---|
| 청각 모델 | 전/후 마스킹 · 주파수 마스킹 | 송종관 제4장 |
| 변환 도메인 | MDCT (Modified Discrete Cosine Transform) | 송종관 제4장 |
| 양자화 | 비수반적(threshold) — 마스트리핑 레이어 이하 제거 | 송종관 제2장 |
| 비트할당 | 청각 모델 기반 스케일팩터 할당 | 송종관 제4장 |
| 출력 형식 | MPEG, MP3, Wave, Streaming | 박은경·구본철 Ch 14 |

## 관련
- [[digital-audio-mp3-encoder]] — 송종관 (2000) — 핵심 소스
- [[audio-processing-soundforge-vegas]] — 박은경·구본철 (2003) — 실무 렌더링
- [[multimedia-signal-processing]] — 음성 부호화(MP3·PCM)·영상 압축 통합 교과
- [[a-course-in-dsp]] — DSP 이론 기초
- [[steganography-watermarking]] — MP3 워터마킹 (acoustic masking 기반)
- [[mpeg2-source-code-commentary]] — MPEG2 부호화 코드 (동일 클러스터)
