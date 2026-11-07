---
title: 임베디드 리눅스 입문 (Embedded Linux Primer, 2판)
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, embedded-linux, linux-kernel, bootloader, device-tree, rootfs, debug]
sources: [raw/books/embedded-linux-primer.md]
confidence: high
---
# 임베디드 리눅스 입문 (Embedded Linux Primer, 2판)

> 저자: 크리스토퍼 할리내(Christopher Hallinan) | 역자: 강덕진
> 원서: Embedded Linux Primer, 2nd Ed. (Newnes, 2008) | 정보문화사, 2008
> 632p `raw/books/embedded-linux-primer.md`

## 개요
임베디드 리눅스 스택(하드웨어 → 커널 → rootfs → 디버깅)을 **개념·구조·부팅·디버깅** 4단으로 정리. 프로세서 아키텍처(제3장), 커널 구조(제4-5장), 부트로더(제7장), 드라이버(제8장), 파일시스템(제9-11장), 버그 디버깅(제14-15장), 리얼타임(제17장)까지 "어디서 뭘 읽어야 하는가"에 대한 지도서 `raw/books/embedded-linux-primer.md`.

## 장 구조 (17장)
| 장 | 제목 |
|----|------|
| 1 | 임베디드 시스템 개요 (개요) |
| 2 | 임베디드 처음 경험하기 |
| 3 | 프로세서 기본 (MIPS·ARM·SoC) |
| 4 | 다른 관점에서 본 리눅스 커널 |
| 5 | 커널 초기화 (initramfs/init) |
| 6 | 시스템 초기화 |
| 7 | 부트로더 (U-Boot) |
| 8 | 디바이스 드라이버 기초 |
| 9 | 파일 시스템 |
| 10 | MTD 서브시스템 |
| 11 | BusyBox |
| 12 | 임베디드 개발 환경 (교차 툴체인) |
| 13 | 개발 도구 |
| 14 | 커널 디버깅 기술 |
| 15 | 임베디드 리눅스 애플리케이션 디버깅 |
| 16 | 리눅스 포팅 |
| 17 | 리눅스와 리얼타임 |

`raw/books/embedded-linux-primer.md`

## 특징
- **부트로더(U-Boot)·커널 초기화(5-6장)를 별도 장으로 분리** — 스타트업 코드 → 커널 → rootfs 순을 집중
- 디버깅(14-15장)을 두 장으로 배치 — "잘못 났을 때 어디서 잡아야 하는가"
- 리얼타임(17장)까지 다루어 임베디드 리눅스의 범위를 "OS 전체"로 확장

## 핵심 컨셉 연결
- [[embedded-linux-stack]] — 4단계 파이프라인의 "개념+디버깅" 관점
- [[embedded-linux-build]] — 스택을 자동화(레시피)하는 관점
- [[embedded-firmware-basics]] — 스타트업 코드/부트로더 하위 관점
- [[embedded-linux-yocto-project]] — 이 입문서의 U-Boot/커널을 레시피로 조립
- [[linux-kernel-structure]] — 리눅스 커널 구조 심화

## Related
- 저자: 크리스토퍼 할리내 (Christopher Hallinan)
- 개념: [[embedded-linux-stack]], [[embedded-linux-build]], [[embedded-firmware-basics]], [[linux-kernel-structure]]
- 보드: [[bbb-yocto-project]], [[gnu-linux-rapid-embedded]]
