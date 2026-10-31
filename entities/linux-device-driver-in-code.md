---
title: 코드로 읽는 리눅스 디바이스 드라이버 (임베디드 개발자를 위한)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, programming, device-driver, embedded-linux]
sources: [raw/books/linux-device-driver-in-code.md]
confidence: high
---
# 코드로 읽는 리눅스 디바이스 드라이버 (임베디드 개발자를 위한)

> 원서: 스리크루난 벤카테스와란(Srikrishnan Venkateswaran), *Essential Linux Device Drivers* (Prentice Hall / Pearson, 2008)
> 국내: 박재호 옮김, 에이콘(주) **2010(2016 재발행)**, ISBN 978-89-6077-149-9, 807p / 23장

## 개요
임베디드 개발자를 위한 리눅스 디바이스 드라이버 총서다. "기존 책과 차원이 다르다"는 추천의 글(아놀드 로빈스)처럼, 표준 유닉스 내부(직렬/DISK/file system)을 넘어 PCMCIA·USB·I2C·비디오·오디오·플래시 메모리·무선 통신까지 현대 PC와 임베디드 하드웨어가 커널과 접하는 요소를 빠뜨리지 않고 다룬다. 드라이버 소스를 코드 단위로 해설하는 것이 주축이다. 이 클러스터에서 장비를 가장 넓게(23장) 다루며, 한국 실습서([[linux-kernel-device-driver-practice]])와 같은 버스들을 더 넓은 맥락에서 연결한다.

## 장 구조 (23장)
| # | topic | 핵심 |
|---|-------|------|
| 2 | 커널 내부 | 커널 구조, 사용자/커널 공간 |
| 5 | 문자 장치 | char device 드라이버 |
| 6 | 직렬 | UART/직렬 드라이버 |
| 7 | 입력장치 | input subsystem |
| 8 | I2C | I2C 버스 드라이버 |
| 10 | PCI | PCI 드라이버 모델, DMA |
| 11 | USB | USB 드라이버 |
| 12 | 비디오 | video driver |
| 13 | 오디오 | audio driver |
| 14 | 블록 | block device |
| 15 | NIC | 네트워크 인터페이스 |
| 16 | 무선 | wireless |
| 17 | Bluetooth | bluetooth |
| 18 | 임베디드 | 임베디드 시스템 |
| 19 | 사용자 영역 드라이버 | userspace driver |
| 20 | 기타 | other |
| 22 | 배포 | 배포 |
| 23 | 종료 | 마무리 |

## 특징
- **23장 광범위**: 문자/블록/직렬을 넘어 USB·I2C·PCI·비디오·오디오·NIC·무선·Bluetooth까지 — 드라이버 범주를 한 권으로.
- **코드 중심 해설**: "코드로 읽는" — 드라이버 데이터 구조와 핸들러를 코드 단위로 분해.
- **임베디드 관점**: 현대 PC + 임베디드 하드웨어(플래시, PCMCIA, 무선)를 커널과 연결하는 요소를 빠짐없이 다룸.
- **번역서**: Prentice Hall / Pearson 2008 원서, 에이콘 2010 번역(2016 재발행).

## 핵심 컨셉
- [[linux-kernel-structure]] — 장치모델·프로세스·메모리 공통 축
- [[linux-kernel-device-driver-practice]] — 같은 버스 집합의 한국 실습서(동반 서)
- [[linux-kernel-development-love]] — 커널 개요(17장 장치·모듈)의 상위서
- [[linux-kernel-programming-itepert]] — IT EXPERT 커널 실전(동반 서)
