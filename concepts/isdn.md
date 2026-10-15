---
title: ISDN (Integrated Services Digital Network)
created: 2026-10-15
updated: 2026-10-15
type: concept
tags: [networking, data-communication]
sources: [raw/books/lan-van-isdn.md]
confidence: high
---
# ISDN (종합 정보 통신망)

음성(전화)·데이타·음성(도화) 등 **다양한 정보를 하나의 디지털 망**으로 통합 전달하는 통신 체계. 이 책 9장이 "미래의 정보 통신 시스템"으로 위치시킨다. LAN(7장)·VAN(8장) 이후의 통합 단계.

> "개발중에 있는 VAN(부가가치 통신망)과 미래의 정보 통신 시스템인 ISDN(SH 정보 통신망)에 관한 이론" `[raw/books/lan-van-isdn.md]` p.2 (OCR: ISDN→"SH 정보 통신망")

## 핵심 구성
- **B 채널 (Bearer, 64 kbps)** — 사용자 데이타(음성·데이타) 전달
- **D 채널 (Delta, 16 kbps)** — 시그널링·소용량 데이타(호 콜, 메세지)
- **B·D 채널 분리**가 ISDN의 본질 — 데이타를 디지털로 전달하되, 시그널링을 별도 경로로 처리한다 `[raw/books/lan-van-isdn.md]` ch9
- **사용자-네트워크 인터페이스 (RSI, Reference Point)** — S/T 리퍼런스로 사용자 단말과 망을 구분
- **가설적 기준 연결 (Virtual Reference Connection)** — 로컬 ISDN 접속의 개념 모델

## ISDN 서비스
| 서비스 | 내용 |
|--------|------|
| 음성 | 디지털 회선(PCM) |
| 음성을 제외한 데이타 | B 채널을 통한 동기(동시)·비동기 데이타 |
| 시그널링 | D 채널의 호 제어 |

## ISDN 프로토콜 체제
- 물리(2층) → 데이타링크(2) → 네트워크(2) 계층 (ISDN 전용 7~4계층) + 상위 응용
- B-ISDN(광대역, B-ISDN 발전)으로의 확장 — 9.7절

## 관련 개념
- [[osi-7-layer-model]] — ISDN 역시 이 모델에 매핑
- [[local-area-network]] — LAN은 제한 지역, ISDN은 통합 망
- [[lan-van-isdn]] (책) — ISDN을 "미래 망"으로 설명한 9장
