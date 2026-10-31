---
title: Professional Linux Programming (프로페셔널 리눅스 프로그래밍)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, programming, linux, unix, os, ipc]
sources: [raw/books/professional-linux-programming-wrox.md]
confidence: high
---

# Professional Linux Programming (프로페셔널 리눅스 프로그래밍)

> 원서: Professional Linux Programming (Wrox Press, ISBN 1-861003-01-3, Copyright 2001). 저자: Neil Matthew·Richard Stones 외 2인 공저. 번역: 김덕수 역. 한국: 보문사, ISBN 89-7627-831-3, 1392쪽, 2002 `[raw/books/professional-linux-programming-wrox.md]`

Wrox의 **리눅스 고급 프로그래밍 교재** 한국어 번역 ([[beginning-linux-programming]]의 상위권). 28장 체제로, 기본 C 프로그래밍을 넘어서는 응용 주제 — 데이터베이스, 디렉터리 서비스, 보안, 대체 언어, 클러스터, 커널, 문서화, 국제화 — 를 폭넓게 다룸. 본문 표지는 "WROX 사와 정보문화사 간의 정식 계약에 의하여 번역" 저작권 고지를 싣는다 `[raw/books/professional-linux-programming-wrox.md]`.

## 구조 (TOC 주요 장, OCR 교정)
| 장 | 테마 | 쪽 |
|----|------|----|
| 5 | MySQL | 197 |
| - | X.500/LDAP | 272 |
| 12 | 보안 | 523 |
| 15 | Python | 643 |
| 24 | Beowulf 클러스터 | 1049 |
| 25 | 문서화 | 1095 |
| 26 | 커널/장치드라이버 | - |
| 28 | 국제화 | 1211 |

## 특징
- **C 중심 리눅스 개발의 "주변 세계" 지도** — DB(MySQL), 디렉터리(X.500/LDAP), 보안, 대체 언어(Python), 클러스터(Beowulf 커널 기반 평행 계산), 커널/드라이버, i18n까지 28장에 걸쳐 리눅스 개발 생태계를 훑는 구조 `[raw/books/professional-linux-programming-wrox.md]`
- 24장 Beowulf 클러스터는 2000년대 초 평행 계산 열풍의 교과서적 사례 — CPU 군집으로 단일 문제를 분산하는 구성 (당시 "수천 달러짜리 슈퍼컴퓨터 대신 PC 클러스터" 논리)
- 26장 커널/장치드라이버는 리눅스 커널 개발로의 진입 구간 — [[linux-essential-utilities]]의 바이너리 도구 체인과 함께 읽을 실무 counterpart
- 저자 집단은 [[neil-matthew]]·[[richard-stones]] 외 2인. 본서는 Wrox 쌍 중 "심화권"으로, 입문권은 [[beginning-linux-programming]]

## 핵심 컨셉 연결
- [[beginning-linux-programming]] — 동일 공저자 집단의 Wrox 입문권
- [[unix-process-ipc]] — 12장 보안과 프로세스 격리, 클러스터 분산과 IPC의 접점
- [[unix-ipc-signals]] — APUE 축으로의 심화 경로 (시그널·IPC 상세)
- [[linux-essential-utilities]] — 리눅스 도구 체인 실무서 (C 개발 환경)

## OCR 노트
- TOC 장 번호 일부 OCR 혼용 (예: X.500/LDAP 장 번호 표기 누락). 28장 체제 확인
- "외 3인/외 13인" 표기는 "외 2인" 공저의 OCR 혼동으로 추정 (brief 교정 기준)
