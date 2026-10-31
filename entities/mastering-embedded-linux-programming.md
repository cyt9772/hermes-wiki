---
title: 임베디드 리눅스 프로그래밍 완전정복 (Mastering Embedded Linux Programming, 2nd Ed.)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, embedded-linux, cross-toolchain, linux-kernel, rootfs, gnu-toolchain, linux]
sources: [raw/books/mastering-embedded-linux-programming.md]
confidence: high
---
# 임베디드 리눅스 프로그래밍 완전정복 (Mastering Embedded Linux Programming, 2nd Ed.)

> 저자: **크리스 시먼즈 (Christopher Sims)** | 역자: 김기주 · 김병극 · 송지연
> 원서: Mastering Embedded Linux Programming, 2nd Ed. | 에이콘(주), 2018
> ISBN 978-89-6077-210-?(마지막 자리 OCR 소실) (세트) / 584p `raw/books/mastering-embedded-linux-programming.md`

## 개요
크로스 툴체인(GNU toolchain, 제2장) → 부트로더(제3장) → 커널 구성·빌드(제4장) → 루트 파일시스템(제5장) → 빌드 시스템 선택(제6장)의 **5단 빌드 체인**을 먼저 다룬 뒤, 저장소 전략(제7장), OTA 업데이트(제8장), 장치 드라이버(제9장), 프로세스·메모리(제12-13장), GDB 디버깅(제14장), 실시간 프로그래밍(제16장)으로 이어지는 16장 체제 `raw/books/mastering-embedded-linux-programming.md`. "빌드 → 운영 → 디버깅"을 하나의 서사로 묶는 실무서.

## 장 구조 (16장)
| 장 | 제목 |
|----|------|
| 1 | 시작 |
| 2 | 크로스 툴체인에 대해 배워보자 (GNU toolchain) |
| 3 | 부트로더에 대한 모든 것 |
| 4 | 커널 구성과 빌드 |
| 5 | 루트 파일시스템 만들기 |
| 6 | 빌드 시스템 선택 |
| 7 | 저장소 전략 만들기 |
| 8 | 소프트웨어 업데이트 (OTA) |
| 9 | 장치 드라이버와의 만남 |
| 12 | 프로세스와 스레드 |
| 13 | 메모리 관리 |
| 14 | GDB로 디버깅하기 |
| 15 | 프로파일링과 추적 |
| 16 | 실시간 프로그래밍 (PREEMPT_RT) |

`raw/books/mastering-embedded-linux-programming.md`

## 특징
- 크로스 툴체인(제2장)을 **빌드 체인의 첫 장**으로 배치, GNU toolchain(컴파일러·리더·assembler)을 집중 설명
- 부트로더 → 커널 → 루트 파일시스템(제3→4→5장)을 "빌드 체인"으로서 단일 서사로 묶음
- 빌드 시스템 선택(제6장)을 별도 장으로 두어 "수동 빌드 vs 자동화 빌드(Yocto/Buildroot)" 비교를 명시
- GDB 디버깅(제14장)과 실시간 프로그래밍(제16장, PREEMPT_RT 패치)을 후반에 배치, **빌드 후 실무**까지 포괄
- 584p 분량으로 크로스 컴파일·구현·운영을 통합한 실무서 `raw/books/mastering-embedded-linux-programming.md`

## 핵심 컨셉 연결
- [[embedded-linux-build]] — 이 서적의 2→3→4→5장이 그 개념의 **핵심 파이프라인**
- [[embedded-linux-systems-arm-an]] — ARM 명령어·SoC 중심, 이 서적과 대비
- [[embedded-linux-cross-dev-hae]] — 교차 개발 환경 구축을 설계 단계부터 다룬 IT EXPERT 교재
- [[embedded-linux-yocto-project]] — 이 서적의 "빌드 시스템 선택"(제6장)에서 Yocto로 자동화
- [[linux-kernel-development-love]] — 커널 내부 구조 심화 (제4장 커널 구성 대비)
- [[linux-kernel-programming-itepert]] — IT EXPERT 시리즈 내 커널 프로그래밍 교재

## Related
- 저자: 크리스 시먼즈 (Christopher Sims)
- 역자: 김기주 · 김병극 · 송지연
- 개념: [[embedded-linux-build]]
