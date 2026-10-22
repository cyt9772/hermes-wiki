---
title: CDMA / 확산 스펙트럼 실무 (Practice)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering]
sources: [raw/books/cdma-all.md]
confidence: high
---
# CDMA / 확산 스펙트럼 실무 (Practice)

확산 스펙트럼(SS)·코드 분할 다중접속(CDMA)의 **이론(Prasad)** + **실무/한국 역사(김갑용)** 두 관점.

## 이론 vs 실무

| 항목 | **이론(Prasad)** | **실무(김갑용)** |
|---|---|---|
| DSSS 원리 | 직접 확산(DSSS), 주파수 합핑(FFH), 시간 합핑(TH), chirp, 혼성 (p.267) | DSSS, Walsh/Gold/PN code, **IS-95** (제3장) |
| 수신기 | Rake receiver 개념 | **Rake receiver** 상세(제4장), PN code 동기, despreading |
| 전력제어 | near-far effect 개념 | **closed/open loop**, near-far effect 실무(제5장) |
| 핸드오프 | soft/hard handoff | **soft/hard handoff** 실무(제6장) |
| 시스템 | 3G (UMTS/CDMA2000) | **IS-95** (2G) → **IS-2000/CDMA2000** (3G) (제9장) |
| **한국 역사** | — | **1996년 세계 최초 CDMA 상용화** (머리말) — 2000만 가입자 |

## 기술 세대
- 1980s: 셀룰러(아날로그, AMPS/TACS/NMT)
- 1990s: **IS-95 CDMA** (디지털 · 2G) — **한국 세계 최초**(1996)
- 2000s: **IS-2000/CDMA2000** (3G) + WCDMA(UMTS)

## 관련
- [[spread-spectrum-cdma]] (기존) — Prasad 이론
- [[channel-access-protocols]] (기존) — FDMA/TDMA/CDMA 비교
- [[mimo-ofdm-wireless-matlab]] (기존) — 3G 이후(OFDM·MIMO)
