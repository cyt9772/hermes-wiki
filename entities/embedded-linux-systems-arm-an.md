---
title: ARM으로 배우는 임베디드 리눅스 시스템 (IT EXPERT)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, embedded-linux, arm, soc, linux-kernel, device-driver, android, it-expert]
sources: [raw/books/embedded-linux-systems-arm-an.md]
confidence: high
---
# ARM으로 배우는 임베디드 리눅스 시스템 (IT EXPERT)

> 저자: **안효복** | 출판: 한빛미디어(주), IT EXPERT 시리즈
> ISBN 978-89-6848-068-?(마지막 자리 OCR 소실) / 개정 2013-12, 4쇄 2019-03 / 1078p `raw/books/embedded-linux-systems-arm-an.md`

## 개요
ARM 아키텍처에서 Android 애플리케이션까지, 하드웨어-소프트웨어를 종단(end-to-end)으로 다루는 임베디드 리눅스 종합 교재. ARM CPU 명령어·예외 처리(제3-6장)부터 SoC 구조(제9장), 임베디드 C 최적화(제12장), 부트로더(제15장), 리눅스 커널·디바이스 드라이버(제16-17장), 커널 포팅(제20장)에 이르기까지 단계를 밟은 뒤 마지막 제25장에서 Android 빌드·탑재·실행으로 수렴한다 `raw/books/embedded-linux-systems-arm-an.md`. 1078p 분량으로 IT EXPERT 시리즈 중 가장 포괄적인 책이다.

## 장 구조 (OCR TOC 기준, 25장)
| 장 | 제목 |
|----|------|
| 1 | 임베디드 시스템의 개요 |
| 2 | 임베디드 시스템의 설계 |
| 3 | ARM 아키텍처와 동작 원리 |
| 5 | ARM 프로세서 명령어 |
| 6 | 예외 처리와 시스템 리셋 |
| 9 | SoC 구조 |
| 12 | 임베디드 C 프로그래밍과 소프트웨어 최적화 |
| 15 | 개발 환경과 부트로더 |
| 16 | 리눅스 커널 |
| 17 | 디바이스 제어 |
| 20 | 커널 포팅 준비 |
| 25 | Android 빌드, 탑재 및 실행 |

(그 외 7·10·13·19장 등 25-26장 체제, OCR TOC 기준) `raw/books/embedded-linux-systems-arm-an.md`

## 특징
- ARM CPU 명령어(제5장), 예외 처리·리셋(제6장) 등 하위층(hardware-level)부터 시작해 Android까지 단일 서술로 묶음
- SoC 구조(제9장)와 임베디드 C 최적화(제12장)를 별도 장으로 분리, "하드웨어 이해 → 소프트웨어 구현" 흐름을 명시
- 부트로더(제15장) → 리눅스 커널(제16장) → 디바이스 드라이버(제17장) → 커널 포팅(제20장)의 포팅 파이프라인을 순차적으로 다룸
- 최종 장(제25장) Android 빌드·탑재·실행까지 포함, "커널 + Android" 조합을 하나의 서사로 완성 `raw/books/embedded-linux-systems-arm-an.md`

## 핵심 컨셉 연결
- [[embedded-linux-build]] — 이 책의 15→16→17→20장 구조가 그 개념의 핵심 예시
- [[embedded-linux-cross-dev-hae]] — 교차 개발·타겟 보드(제7장 vs 15장)를 다른 관점으로 다룸
- [[embedded-linux-yocto-project]] — 이 서적의 수동 빌드(커널 설정→컴파일)를 Yocto 레시피/BitBake으로 자동화한 대비 책
- [[mastering-embedded-linux-programming]] — 같은 범위를 다른 16장 체제로 정리한 미국 원서 기반 교재
- [[linux-kernel-development-love]] — 커널 내부 구조 심화 (제16-17장 대비)
- [[linux-kernel-programming-itepert]] — IT EXPERT 시리즈 내 커널 프로그래밍 교재

## Related
- 저자: 안효복 (IT EXPERT 시리즈)
- 개념: [[embedded-linux-build]]
