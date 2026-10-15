---
title: Local Area Network (LAN)
created: 2026-10-15
updated: 2026-10-15
type: concept
tags: [networking, data-communication]
sources: [raw/books/lan-van-isdn.md]
confidence: high
---
# Local Area Network (LAN)

제한된 물리적 영역(건물·캠퍼스) 내 단말기 간 고속 통신을 위한 공유 매체 망. 이 책 7장에서 근거리 통신망의 **계층 모델 → 프로토콜 → 시스템 구축 → 실제 예 → 시장 동향**을 다룬다. 핵심은 "여러 단말이 하나의 전송 매체를 어떻게 공유할 것인가"를 정한 **채널 액세스 프로토콜**이다.

> "제 7 장 근거리 통신망(씨 : Local Area Network) …… 7.1 개요 / 7.2 LAN 계층 모델과 프로토콜 / 7.3 LANS| 시스템 구축 / 7.4 L씨의 실제 예 / 7.5 LANS| FS 및 시장 동향" `[raw/books/lan-van-isdn.md]` TOC p.7

## 채널 액세스 방식 (4장의 기반)
LAN의 근본 문제는 **충돌** — 공유 매체에서 다수가 동시에 송신했을 때. 접근 방식은 대분류로:
- **고정 할당 (Fixed Assignment)** — 각 단말에 시간/주파수 슬롯 예약
- **임의 할당 (Random Assignment)** — ALOHA, CSMA, CSMA/CD (경쟁 기반)
- **요구 할당 (Demand Assignment)** — 필요 시 채널 요청 (Token Ring 계열: 토큰 순환으로 충돌 회피) `[raw/books/lan-van-isdn.md]` ch4 p.140-164

## 두 대표 체제
| 체제 | 접근 | 특징 |
|------|------|------|
| **이더넷 계열** | CSMA/CD (경쟁) | 단순·저가, 충돌 발생 가능 |
| **토큰 링 (Token Ring)** | 토큰 순환 (접근권 보유 전송) | 예측 가능·대칭성, 충돌 없음 |

이 책 7.4 "실제 예"에서 이 두 실제 LAN(토큰 링·이더넷 계열)을 비교하고, 7.5에서 시장 동향을 보인다.

## 계층 모델
LAN은 OSI 모델의 **1·2계층(물리+데이타링크)** 위주. MAC(매체 액세스 제어) 서브레이어가 채널 액세스를 담당하며, LL(논리 링크)은 프레임·오류 제어를 담당 — 2장의 데이타링크 제어·멀티플렉싱과 직접 연결된다.

## 관련 개념
- [[channel-access-protocols]] — 고정/임의/요구 할당과 CSMA, Token Ring
- [[osi-7-layer-model]] — LAN이 매핑되는 1~2계층
- [[isdn]] — WAN/통합망으로 확장된 후속 개념
- [[local-area-network]] 본 항목

## 참고
"씨"/"L씨의" 등 OCR에서 "LAN"이 깨진 토큰이 많다 — 의미상 모두 LAN.
