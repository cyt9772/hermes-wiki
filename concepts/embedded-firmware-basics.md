---
title: 임베디드 펌웨어 분석 (부팅·스타트업 코드·버스 구조)
created: 2026-11-07
updated: 2026-11-07
type: concept
tags: [embedded, firmware, bootloader, arm, mips, sparc, bus-architecture, concept]
sources:
  [raw/books/embedded-systems-firmware.md,
   raw/books/embedded-linux-primer.md,
   raw/books/mastering-embedded-linux-programming.md,
   raw/books/embedded-linux-systems-arm-an.md]
confidence: high
---
# 임베디드 펌웨어 분석 (부팅·스타트업 코드·버스 구조)

임베디드 시스템이 전원이 들어간 순간부터 운영체제가 오르기까지의 **하드웨어 부수(firmware) 세계**를 다룬 개념. 전원이 켜지면 CPU는 reset vector에서 스타트업 코드(부트 스티커)를 실행하고, RAM/버스 초기화 → 부트로더 → 커널 로드 순으로 시스템이 "일어나는" 과정을 **명령어셋과 버스의 관점**에서 분석한다.

## 스텍 구성
1. **스타트업 코드/부트 스티커 (startup code / bootstrapper)** — reset vector에서 실행. ROM에서 RAM으로 코드를 복사하고, 버스(RISC·PCI 등)와 메모리 초기화. `raw/books/embedded-systems-firmware.md` Part 1-2
2. **버스·메모리 구조** — Address Space, Memory Map, DMA, 버스 프로토콜(ARM·MIPS·SPARC 비교). `raw/books/embedded-systems-firmware.md` Part 3, `raw/books/embedded-linux-systems-an.md` 제10장
3. **부트로더** — 스타트업 코드 → 커널 로드/실행 인계. U-Boot/BSP의 위치. `raw/books/embedded-linux-primer.md` 제5-7장, `raw/books/mastering-embedded-linux-programming.md` 제3장
4. **BIOS·OS 구동** — M68K BIOS 분석(1680p급 분서). `raw/books/embedded-systems-firmware.md` Part 4

## 관련 서적
- 펌웨어 분석(1,680p): [[embedded-systems-firmware]]
- 아키텍처·시스템 관점: [[embedded-linux-primer]], [[embedded-linux-systems-arm-an]]
- 빌드 체인 파이프라인: [[embedded-linux-build]]
- 커널 구조: [[linux-kernel-structure]]

## Related
- 개념: [[embedded-linux-build]], [[linux-kernel-structure]]
- 아키텍처: [[embedded-linux-systems-arm-an]]
