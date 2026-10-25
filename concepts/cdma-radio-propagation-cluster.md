---
title: CDMA/WCDMA 전파분석 클러스터 (CDMA Radio Propagation Cluster)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [cdma-dsss, wireless-communications, telecom-systems, spread-spectrum]
sources: [raw/books/cdma-wcma-radio-analysis.md]
confidence: high
---
# CDMA/WCDMA 전파분석 클러스터

## 정의
**CDMA(IS-95/cdma2000)와 WCDMA(3GPP/UMTS)를 알고리즘·표준 규격이 아닌 전파 신호·실무 관점에서 다루는 클러스터**. 이 개념의 중심서 [[cdma-wcma-radio-analysis]](이상근, 2009)는 CDMA·WCDMA 무선 기술을 "전파 신호의 관점"에서 정리 — **기저국 RF 신호·전파 세기·품질·핸드오프·전력제어**의 현장 실무 언어.

## 핵심 주제를 클러스터를 넘어선 3관점
| 관점 | 클러스터 |
|------|----------|
| **전파 신호 (RF)** | 본 클러스터 [[cdma-wcma-radio-analysis]] (이상근) |
| **알고리즘·표준 규격** | [[cdma-all]] (김갑용) — IS-95 코드·Rake·전력제어·핸드오프·vocoder, [[spread-spectrum-cdma]] (Prasad) — CDMA 이론 |
| **LTE 관점** | [[lte-radio-interface]] — OFDMA/SC-FDMA, 채널 상태, HARQ |

## 핵심 주제 (cdma-wcma-radio-analysis 기반)
1. **전파 단위·세기·품질** — 전파의 단위(01장), 세기·품질(02장), 고주파 선형성(03장).
2. **안테나** — 구조·특성(04장), **안테나 다이버시티**(05장), VSWR·방사 특성·다이폴(모노폴) 안테나(실습 07-09).
3. **시스템 구분자** — **PN offset**(cdma2000)·**PSC**(WCDMA)·**SID**·**NID**(07장), cdma2000 vs WCDMA 구조 차이(08장).
4. **핸드오프·핸도버** (09장) — soft/hard handoff, 셀 재진입.
5. **전력제어** (13장) — closed/open loop, near-far effect.
6. **Random Access** (14장) — 채널 접근.
7. **DTX·Continuous·Slot Mode(DRX)** (15-16장) — 전력·수면 모드.
8. **위치 등록** (17장) — 이동성 관리.
9. **무선 데이터 전송** (18장) — HSDPA/EVDO(19-21장)의 하향·상향 링크 전송 속도 제어.
10. **계측** — **ACPR 불요파**(실습 05), **Directional Coupler**(06), **스펙트럼 분석기**(Part 3, 167), **네트워크 분석기**(177).
11. **DM 활용** (Part 4, 185+) — 데이터 모니터링.

## 관련 개념 (이 wiki)
- **핵심 기존**: [[cdma-dss-spread-spectrum]] (DSSS 실무) · [[spread-spectrum-cdma]] (Prasad 이론) · [[cdma-all]] (김갑용 실무서)
- **채널·무선**: [[wireless-channel-modeling]] · [[lte-radio-interface]] · [[software-defined-radio]] · [[space-time-coding]] (STBC)
- **안테나**: [[antenna-theory]] · [[array-antenna-beamforming]] · [[antenna-design]]
- **인접 클러스터**: [[video-compression-mpeg]] (영상 부호화 — 다른 도메인이 같은 "표준 실무서" 관점)
- **태그**: `cdma-dsss` · `wireless-communications` · `telecom-systems` · `spread-spectrum` · `antenna-design`

## 미해결 논쟁 / 현재 지식
- **CDMA vs LTE** — 3G CDMA 방식은 4G LTE(OFDMA)로 대체, 5G NR으로 진화. 본 클러스터는 2009년 3G 시점.
- **실무 관점** — LTE/5G 시대에도 **전력제어·핸드오프·전파 세기·안테나 다이버시티**의 원리는 유효.
- **실습 환경** — 스펙트럼/네트워크 분석기·다이폴 안테나 측정은 2026년에도 표준 실습.

## Related
- 책: [[cdma-wcma-radio-analysis]] · [[cdma-all]]
- 저자: [[lee-sang-geun]]
- 인접: [[lte-radio-interface]] · [[spread-spectrum-cdma]] · [[software-defined-radio]]
