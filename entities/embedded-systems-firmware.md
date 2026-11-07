---
title: 임베디드 시스템 펌웨어 분석
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, embedded, firmware, arm, flash, network, debugging]
sources: [raw/books/embedded-systems-firmware.md]
confidence: high
---
# 임베디드 시스템 펌웨어 분석

> 저자: 에드 서터(Ed Sutter) | 역자: 성원호
> 원서: Embedded Systems Firmware Demystified (Newnes, 2002) | 에이콘, 2002
> 375p `raw/books/embedded-systems-firmware.md`

## 개요
전원이 켜진 순간 CPU가 reset vector에서 스타트업 코드(부트 스티커)를 실행하고, 이후 플래시 메모리 인터페이스 - 플래시 파일시스템 - 명령 라인 인터페이스 - 모니터 기반 디버깅 - 네트워크로 이어지는 임베디드 펌웨어 구조를 분석한 서적. 운영체제 이전 단계인 펌웨어 세계를 ARM·MIPS 명령어셋과 버스 관점에서 다룸 `raw/books/embedded-systems-firmware.md`.

## 장 구조 (12+장)
| 장 | 제목 |
|----|------|
| 2 | 시작하기 |
| 3 | Microvision 소개 (부트 스티커/스타트업 코드) |
| 4 | 어셈블리 언어 |
| 5 | 명령 라인 인터페이스 (CLI) |
| 6 | 플래시 메모리 인터페이스 |
| 7 | 플래시 파일시스템 |
| 8 | 스크립트 실행 |
| 9 | 네트워크 연결 |
| 10 | 파일/데이터 전송 |
| 12 | 모니터 기반 디버깅 |

`raw/books/embedded-systems-firmware.md`

## 특징
- 리눅스·OS 없이 부트 스티커와 펌웨어 자체의 구조를 분석 — 스타트업 코드, 어셈블리, CLI, 플래시 인터페이스, 파일시스템, 디버깅, 네트워크 순서로 서술
- Microvision(가상 임베디드 보드)을 예제로, 명령어셋 수준의 디테일을 제공
- 플래시 메모리 인터페이스(제6장)와 플래시 파일시스템(제7장)을 별도 장으로 배치 — 임베디드 리눅스의 rootfs(MTD)의 하위 관점

## 핵심 컨셉 연결
- [[embedded-firmware-basics]] — 스타트업 코드-부트로더-커널-루트FS 파이프라인의 하위 단계
- [[embedded-linux-stack]] — 리눅스 스택 이전의 펌웨어 세계를 다룸
- [[embedded-linux-primer]] — 리눅스 입문서와의 비교 (이 책은 펌웨어, 그 책은 리눅스)
- [[embedded-linux-build]] — 빌드 체인의 하위 단계(스타트업 코드/부트로더)

## Related
- 저자: 에드 서터 (Ed Sutter)
- 개념: [[embedded-firmware-basics]], [[embedded-linux-stack]], [[embedded-linux-build]]
- 관련: [[embedded-linux-primer]], [[bbb-yocto-project]]
