---
title: 시공간 부호 (Space-Time Coding)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, mimo, space-time-coding, signal-processing]
sources: [raw/books/mimo-ofdm-wireless-matlab.md]
confidence: medium
---
# 시공간 부호 (Space-Time Coding / STC)

## 정의
**다수 송신 안테나(MIMO)의 시간 차원과 공간 차원을 함께 이용**해, 페이딩에 강하고 용량을 높이는 무선 채널 부호화. 단일 안테나 부호의 다이버시티/코딩 기득을 MIMO로 확장.

## 주요 방식
- **STTC (Space-Time Trellis Code)** — 격자구조 부호, 다이버시티·코딩 이득 극대화
- **SFBC (Space-Frequency Block Code / Alamouti)** — 2×2 MIMO 기본 정합 부호, 단순 디코더

> 시공간 부호의 이론적 배경은 MIMO 용량(제9장 Deterministic MIMO channel capacity)과 결합하여 `[raw/books/mimo-ofdm-wireless-matlab.md]` 다뤄짐 (개념 연동: MIMO·OFDM)

## Related
- [[mimo-multiple-input-multiple-output]] — MIMO
- [[wireless-channel-modeling]] — 채널 모델
- [[ofdm-orthogonal-frequency-division]] — OFDM과의 결합
