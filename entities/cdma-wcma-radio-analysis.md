---
title: CDMA/WCDMA 전파분석 (이상근, 2009)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, cdma-dsss, wireless-communications, telecom-systems]
sources: [raw/books/cdma-wcma-radio-analysis.md]
confidence: high
---
# CDMA/WCDMA 전파분석 (이상근, 2009)

> 저자: **이상근** (Lee Sang-geun / Lee Sang-gyun — 원문 머리말 2009년 2월 서명 "저자 이상근", rainbowstar @ dreamwiz.com)
> 출판: 2009년 2월 (원문 머리말), 한글 원서.
> 원문 머리말: "CDMA, WCDMA 기술은 인류의 생활 패턴을 바꾸어 놓을 만큼 큰 변화를 일으킨 대표적인 IT 기술이라 할 수 있으며, 관련한 많은 기술 서적들이 출간되어 있다. 이 책은 많은 다른 책들과 관점을 달리하여 CDMA, WCDMA의 무선 기술을 알고리즘이나 표준 규격의 관점이 아닌 **전파 신호의 관점**에서 쉽게 이해할 수 있도록 요약 정리하였다. 또한 간단한 실습을 통하여 실질적인 무선 기술 현상의 이해를 돕고자 내용을 구성하였다."

## 개요
한국 이동통신의 표준 방식이었던 **CDMA(IS-95)**와 **WCDMA(3GPP/UMTS)**의 무선 기술을 **전파(-radio, propagation) 신호의 관점**에서 정리한 실무서. 알고리즘·표준 규격 관점(김갑용 『CDMA의 모든 것』, R. Prasad 『CDMA for UMTS/IMT-2000』 등)이 아닌, **기저국 RF 신호·전파 세기·품질·핸드오프·전력제어**의 현장 실무 관점. 학생과 **무선망 최적화 업무** 엔지니어 모두를 위한 3~4부 구성 — 이론·실습·계측·DM 활용.

## 부 구성 (TOC 기반, 208p)
| Part | 내용 | pp |
|------|------|----|
| **1** | **CDMA/WCDMA 전파분석 이론** — 21장: 전파 단위(01), 세기·품질(02), 고주파 선형성(03), 안테나 구조·특성(04), **안테나 다이버시티**(05), 기지국 구성(06), **PN offset·PSC·SID·NID**(07), cdma2000 vs WCDMA(08), **핸드오프·핸도버**(09), 전파 속도와 서비스 반경(10·11), RF 신호 파형(12), **전력제어**(13), Random Access(14), **DTX·Continuous mode**(15), **Slot Mode(DRX mode)**(16), 위치 등록(17), 무선 데이터 전송(18), **HSDPA/EVDO 고속 데이터**(19·20·21) | 2–116 |
| **2** | **CDMA/WCDMA 전파분석 실습** — 15장: 전파 세기·품질 측정, 핸드오프, 셀룰러·PCS·WCDMA 주파수 채널 검증, 신호 레벨, **ACPR 불요파**, Directional Coupler, 안테나 **VSWR**, 안테나 방사 특성, **다이폴(모노폴) 안테나**, Slot Mode, **EVDO 기지국 출력 파형 분석**, **HSDPA 하향링크 throughput**, DTX·Continuous 측정, Replay 모드 핸드오프 분석 | 117–164 |
| **3** | **스펙트럼 분석기/네트워크 분석기 원리 및 응용** — 고주파 신호 측정 원리, **spectrum analyzer**(167), **network analyzer**(177) | 165–184 |
| **4** | **DM의 이해 및 활용** (185–208) | 185–208 |

## 핵심 기여
- **전파 신호 관점** — CDMA/WCDMA를 알고리즘·표준 규격이 아닌 **실시간 RF 신호**로 다룸 (머리말).
- **PN offset / PSC / SID / NID** (07장)로 CDMA2000 vs WCDMA의 **시스템 구분자**를 실무 언어로.
- **안테나 다이버시티** (05장), **전력제어** (13장), **핸드오프/핸도버** (09장) — 무선통신의 3대 핵심 변수.
- **HSDPA/EVDO** (19-21장)의 하향·상향 링크 전송 속도 제어.
- **실습 15개** + **스펙트럼/네트워크 분석기** (Part 3)로 계측까지 포괄.

## Related
- 저자: [[lee-sang-geun]]
- 개념: [[cdma-radio-propagation-cluster]] (이 책 중심) · [[cdma-dss-spread-spectrum]] (실무) · [[spread-spectrum-cdma]] (Prasad 이론) · [[cdma-all]] (김갑용 실무서)
- 인접: [[lte-radio-interface]] (LTE 관점) · [[wireless-channel-modeling]] (채널 모델) · [[antenna-theory]] · [[array-antenna-beamforming]]
- 태그: `cdma-dsss`

## OCR/추출 신뢰도
- 한글 OCR 일부 토큰 깨짐(한자형 혼입) — 표·식 번호와 문맥으로 cross-check.
- 머리말 26-27행서 저자 서명·이메일 재확인.
