---
title: 욕토(Yocto) 프로젝트로 시작하는 임베디드 리눅스 시스템
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, embedded-linux, yocto, openembedded, bitbake, build-system, linux-kernel]
sources: [raw/books/embedded-linux-yocto-project.md]
confidence: high
---
# 욕토(Yocto) 프로젝트로 시작하는 임베디드 리눅스 시스템

> 저자: **루돌프 (Rudolf)** | 역자: 김세영 · 정윤선
> 원서: Embedded Linux Systems with the Yocto Project (ISBN 9780133443240) | 에이콘(주), 2018
> ISBN 978-89-6077-091-1(세트) / 567p `raw/books/embedded-linux-yocto-project.md`

## 개요
OpenEmbedded/BitBake 빌드 엔진을 중심으로 임베디드 리눅스 운영체제 스택을 **레시피(recipe) 단위로 자동 빌드**하는 방법을 단계별로 서술한 실무서. 욕토프로젝트 개요(제2장) → 오픈임베디드 빌드 시스템·BitBake 문법(제3-4장) → 커스텀 배포판(제7장) → 커널 레시피·BSP(제9-10장) → 라이선스 준수(제12장)까지 이어지는 13장 체제 `raw/books/embedded-linux-yocto-project.md`.

## 장 구조 (13장)
| 장 | 제목 |
|----|------|
| 1 | 임베디드 시스템을 위한 리눅스 |
| 2 | 욕토프로젝트 개요 |
| 3 | 오픈임베디드 빌드 시스템 |
| 4 | BitBake 빌드 엔진 (문법) |
| 6 | 리눅스 시스템 구조 |
| 7 | 커스텀 리눅스 배포판 빌드 |
| 8 | 소프트웨어 패키지 레시피 |
| 9 | 커널 레시피 |
| 10 | 보드 지원 패키지 (BSP) |
| 11 | 애플리케이션 개발 |
| 12 | 라이선스 및 규정 준수 |

`raw/books/embedded-linux-yocto-project.md`

## 특징
- **BitBake 문법**(제4장)을 별도 장으로 분리, 레시피의 DEPENDS/RDEPENDS·SRC_URI·패스 매니지먼트를 집중 설명
- 커널 레시피(제9장)와 BSP(제10장)를 레시피 관점에서 다룸 — "커널을 빌드한다"가 아니라 **"커널을 레시피로 서술한다"**
- 라이선스·규정 준수(제12장)를 마지막 실무 장으로 배치, 오픈소스 배포 실무를 강조 `raw/books/embedded-linux-yocto-project.md`
- 567p 분량으로 Yocto/OpenEmbedded에 특화된 실용서

## 핵심 컨셉 연결
- [[embedded-linux-build]] — 레시피/BitBake은 그 개념의 **자동화 레이어**
- [[embedded-linux-systems-arm-an]] — 이 서적의 수동 커널 포팅(제20장)을 레시피로 대체하는 대비 책
- [[embedded-linux-cross-dev-hae]] — 교차 개발 환경 구축(12장)을 Yocto에서 자동으로 처리
- [[mastering-embedded-linux-programming]] — 이 서적에서 "빌드 시스템 선택"(제6장)으로 Yocto를 소개
- [[linux-kernel-development-love]] — 커널 내부 구조 심화 (제9장 커널 레시피 대비)
- [[linux-kernel-programming-itepert]] — IT EXPERT 시리즈 내 커널 프로그래밍 교재

## Related
- 저자: 루돌프 (Rudolf)
- 역자: 김세영 · 정윤선
- 개념: [[embedded-linux-build]]
