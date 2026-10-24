---
title: 안테나 설계 (Antenna Design)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering]
sources: [raw/books/antenna-theory.md, raw/books/rf-engineering.md]
confidence: high
---
# 안테나 설계 (Antenna Design)

안테나(전자기 방사체)의 원리·분류·설계 — 이론(Stutzman·Thiele) + 실무(Chang) 두 관점.

## 안테나 분류 (5종)

| 유형 | 예 | 소스 |
|---|---|---|
| **와이어(선)** | 반파장 쌍극자, folded, log-periodic, V, wire grid | [[antenna-theory]] 제5장 |
| **소형(전자기적)** | small dipole, small loop | [[antenna-theory]] 제2장 |
| **광대역(broadband)** | **spiral**, log-periodic, 리플로렉터(horn) | [[antenna-theory]] 제6장, [[rf-engineering]] 제2장 |
| **개구(aperture)** | slot, horn, dish, **patch(Microstrip)** | [[antenna-theory]] 제8장, [[rf-engineering]] 제2장 |
| **어레이(배열)** | linear/circular array, **phased array**, endfire/broadside | [[antenna-theory]] 제3장, [[array-antenna-beamforming]] (기존) |

## 설계 관점 (이론 → 실무)
1. **기초 정의** (Stutzman 제1장) — 이상적 쌍극자, radiant pattern, **directivity/gain**, reciprocity, polarization
2. **이론 해석** (Stutzman) — 어레이 팩터·패턴 곱법(endfire/Hansen-Woodyard)·**Moment Method**(제7장)·**PO/GO**(제9장)·synthesis(제10장)
3. **실무 설계** (Chang 제2장) — 등방성 방사체, 원거리장, microstrip 패치, horn, parabolic, **측정**
4. **셀룰러 어레이** (기존) — beamforming, DOA(MVDR/MUSIC), spatial diversity

## 관련
- [[array-antenna-beamforming]] (기존) — 어레이 + 빔포밍
- [[wireless-channel-modeling]] (기존) — 무선 채널 모델
- [[antenna-engineering-korean]] (최홍주) — 한국어 안테나 공학 기초 교재
