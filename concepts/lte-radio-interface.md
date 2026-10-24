---
title: LTE 무선 접속 (LTE Radio Interface)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, wireless-communications, ofdm, mimo]
sources: [raw/books/lte-wireless-technology-training.md, raw/books/bluetooth-connect-without-cables.md, raw/books/antenna-engineering-korean.md]
confidence: medium
---
# LTE 무선 접속 (LTE Radio Interface)

LTE(Radio Interface)의 무선 접속 계층 — 물리 계층(OFDM downlink / SC-FDMA uplink)·MAC·RRC(RRM/RRC·핸드오버)까지의 프로토콜 구조와 다중 안테나(MIMO) 적용. WPAN(블루투스)과 안테나 기초는 LTE 이전/인접 무선 시스템으로 함께 정리한다.

## 안테나공학 (최홍주 2004)
- LTE 무선 접속의 물리적 토대 — 전자파 기초(Maxwell·평면파·특성임피던스·Poynting 벡터)와 급전선·임피던스 정합(λ/4 변환기·스터브·Smith 차트)`[raw/books/antenna-engineering-korean.md]`
- 안테나 정수(이득·지향특성·실효개구면적) — 셀 안테나·빔포밍의 성능 상하위 지표로 직접 활용 `[raw/books/antenna-engineering-korean.md]`
- 주파수 대역별 안테나 분류(초단파: 야기·헤리컬, 극초단파: 혼·파라볼라) — LTE 주파수 대역(700MHz~2.6GHz IMT-2000) 적용 안테나 선정의 기초 `[raw/books/antenna-engineering-korean.md]`
- 전파이론(지상파·대류권파·페이딩) — 셀 커버리지·핸드오버 경계 판단의 전파학 배경 `[raw/books/antenna-engineering-korean.md]`

## Bluetooth: Connect Without Cables (Bray & Sturman 2001)
- 단거리(PAN) 무선 접속 — 주파수 호핑 FHSS + GFSK 변조 + SCO/ACL 물리링크, 2.4GHz ISM 대역 `[raw/books/bluetooth-connect-without-cables.md]`
- 안테나(방사 패턴·이득·칩 안테나)에서 프로토콜 스택(베이스밴드→L2CAP→프로파일)까지의 계층화 구조 — LTE PHY→MAC→RRC 계층 모델과 구조상 동일한 "무선 접속" 개념 `[raw/books/bluetooth-connect-without-cables.md]`
- 저전력(hold/sniff/park)·QoS·보안(페어링·본딩) — LTE RRC_IDLE/CONN과 유사한 접속 관리·전력 관리 패턴 `[raw/books/bluetooth-connect-without-cables.md]`

## 무선통신기술의 이해 (현대차 LTE 특강 2014)
- OFDM(하향 OFDMA)·SC-FDMA(상향) 다중 접속 + MIMO(빔포밍·space-time diversity·multiplexing) — LTE Physical Layer 핵심 `[raw/books/lte-wireless-technology-training.md]`
- Radio Interface 프로토콜 — PHY/MAC/RRC 계층 매핑, RRC·RRM, 채널 적응 스케줄링·링크 적응 `[raw/books/lte-wireless-technology-training.md]`
- 네트워크 — E-UTRAN+EPC, user/control plane, 핸드오버(간 셀), 세션 관리 `[raw/books/lte-wireless-technology-training.md]`
- LTE-Advanced (Rel.10/11) — CoMP, heterogeneous network (HeNB), carrier aggregation, D2D, MTC `[raw/books/lte-wireless-technology-training.md]`

## 비교 표 (안테나 기초 ↔ WPAN ↔ LTE)
| 차원 | 안테나공학 (최홍주) | Bluetooth (Bray & Sturman) | LTE 특강 (현대차) |
|---|---|---|---|
| 범위 | 전파·안테나 기초 (모든 대역) | 단거리 PAN (~10m) | 셀룰러 (km급) |
| 접근 방식 | 전송선로/정합/방사 | FHSS + GFSK | OFDMA/SC-FDMA + MIMO |
| 계층 구조 | (물리층 이하) | RF→BB→LMP→L2CAP→프로파일 | PHY→MAC→RRC(EPC) |
| 핵심 관점 | 안테나 정수·전파이론 | 프로토콜 실무·시험승인 | 네트워크·핸드오버·스케줄링 |

## 관련
- [[ofdm-orthogonal-frequency-division]] — OFDM/SC-FDMA 상세
- [[mimo-multiple-input-multiple-output]] — 다중 안테나·빔포밍
- [[antenna-design]] · [[array-antenna-beamforming]] — 안테나 설계·어레이 빔포밍
- [[wireless-channel-modeling]] — 무선 채널 모델
- [[cdma-dss-spread-spectrum]] — WCDMA (LTE 이전 세대)
- [[bluetooth-explained]] · [[bluetooth-connect-without-cables]] — 블루투스
- [[antenna-engineering-korean]] · [[lte-wireless-technology-training]] — 소스 서적
