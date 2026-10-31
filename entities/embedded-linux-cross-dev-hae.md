---
title: 임베디드 리눅스 — 교차 개발 환경에서 윈도우 시스템까지 (IT EXPERT)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, embedded-linux, cross-development, linux-kernel, rootfs, linux, it-expert]
sources: [raw/books/embedded-linux-cross-dev-hae.md]
confidence: high
---
# 임베디드 리눅스 — 교차 개발 환경에서 윈도우 시스템까지 (IT EXPERT)

> 저자: **박재호** | 출판: 한빛미디어(주), IT EXPERT 시리즈
> ISBN 89-7914-208-0 / 초판 2002-07 / 824p `raw/books/embedded-linux-cross-dev-hae.md`

## 개요
임베디드 시스템 개념(제1-5장), 실시간 운영체제(제4장), 제품 기획·타겟 보드 선정(제6-7장) 등 **설계 단계**를 먼저 다룬 뒤, 교차 개발 환경 구축(제12장), 네트워크·디버깅(제13장), 부트스트랩 로더 이식(제14장), 커널 환경 설정·컴파일(제15장), 루트 파일시스템 구축(제16장), 실시간 리눅스 커널 이식(제17장)으로 이어지는 17-20장 체제의 교차 개발 실무서 `raw/books/embedded-linux-cross-dev-hae.md`. 제품 기획과 상용화(패키징, 제20장)까지 포함해 "설계→구현→상용화" 전체 사이클을 포괄한다.

## 장 구조 (16장+ 체제)
| 장 | 제목 |
|----|------|
| 1 | 임베디드 시스템 |
| 2 | 리눅스 |
| 3 | 임베디드 리눅스 |
| 4 | 실시간 운영체제 |
| 5 | 윈도우 시스템 |
| 6 | 제품 기획 단계에서 고려할 사항 |
| 7 | 타겟 보드 선정 |
| 8 | 장치 선정과 장치 드라이버 구현 |
| 9 | 임베디드 리눅스 이식 절차 |
| 12 | 교차 개발 환경 구축 |
| 13 | 네트워크와 디버깅 환경 구축 |
| 14 | 부트스트랩 로더 이식 |
| 15 | 리눅스 커널 환경 설정과 컴파일 |
| 16 | 루트 파일시스템 구축 |
| 17 | 실시간 리눅스 커널 이식 |
| 20 | 상용 제품을 위한 패키징 |

`raw/books/embedded-linux-cross-dev-hae.md`

## 특징
- **제품 기획·타겟 보드 선정**(제6-7장)을 빌드/구현 장(제12-17장) **앞서 배치** — "설계 → 구현" 순서를 명시
- 교차 개발 환경(제12장)과 네트워크·디버깅 환경(제13장)을 별도 장으로 분리, 빌드 환경과 디버깅 환경을 구분
- 부트스트랩 로더 → 커널 → 루트 파일시스템(제14→15→16장)의 포팅 3단계를 순차적으로 서술
- 실시간 리눅스 커널 이식(제17장)과 상용 패키지(제20장)로 끝, "구현 + 상용화"까지 포함 `raw/books/embedded-linux-cross-dev-hae.md`
- 2002년 초판으로 Yocto/BitBake 기반 자동화 전 시대의 **수동 교차 개발** 방법을 대표하는 교재

## 핵심 컨셉 연결
- [[embedded-linux-build]] — 이 책의 12→14→15→16장이 그 개념의 **수동 파이프라인**
- [[embedded-linux-systems-arm-an]] — ARM 아키텍처 중심, 이 서적과 대비
- [[embedded-linux-yocto-project]] — 이 서적의 수동 교차 개발을 Yocto로 자동화
- [[mastering-embedded-linux-programming]] — 툴체인·부트로더·커널 구성을 4장 단위로 정리한 대비 교재
- [[linux-kernel-development-love]] — 커널 내부 구조 심화 (제15장 커널 설정 대비)
- [[linux-kernel-programming-itepert]] — IT EXPERT 시리즈 내 커널 프로그래밍 교재
- [[park-jaeho]] — 저자

## Related
- 저자: [[park-jaeho]]
- 개념: [[embedded-linux-build]]
