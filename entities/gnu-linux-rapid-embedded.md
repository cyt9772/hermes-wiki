---
title: GNU/Linux 쾌속 임베디드 프로그래밍
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, embedded-linux, gpio, i2c, spi, serial, usb, network, arm]
sources: [raw/books/gnu-linux-rapid-embedded.md]
confidence: high
---
# GNU/Linux 쾌속 임베디드 프로그래밍

> 저자: 로돌포 지오메티(Rodolpho Giometti) | 역자: 정병혁
> 원서: GNU/Linux Rapid Embedded Programming (Packt, 2017) | 에이콘, 2018
> 883p `raw/books/gnu-linux-rapid-embedded.md`

## 개요
BeagleBone Black·SAMA5D3·Wand 보드를 대상으로 **리눅스 커널·드라이버·주변장치(GPIO/시리얼/USB/I2C/SPI/이더넷/WLAN/CAN/SND/V4L/ADC/PWM)를 19장 체제로 실무한다.** 개발 시스템 설치부터 주변장치 드라이버까지 "스택 전체를 보드 위에서 돌린다"는 관점 `raw/books/gnu-linux-rapid-embedded.md`.

## 장 구조 (19장)
| 장 | 제목 |
|----|------|
| 1 | 개발 시스템 설치 (BBB·SAMA5D3·Wand) |
| 2 | 시스템 콘솔 관리 |
| 3 | C 컴파일러와 디바이스 드라이버, 유용한 개발 테크닉 |
| 4 | 스크립트와 시스템 데몬을 사용한 빠른 프로그래밍 |
| 5 | 임베디드 OS (JFFS2·UBIFS·Yocto) |
| 6 | 범용 입출력 신호 - GPIO |
| 7 | 시리얼 포트와 TTY 디바이스 |
| 8 | 범용 직렬 버스 - USB |
| 9 | PC 버스 (I2C 관련) |
| 10 | 시리얼 주변 장치 인터페이스 |
| 11 | 1-Wire |
| 12 | 이더넷 네트워크 디바이스 |
| 13 | 무선 네트워크 디바이스 - WLAN |
| 14 | 제어기 영역 네트워크 (CAN) |
| 15 | 사운드 디바이스 - SND |
| 16 | 비디오 디바이스 - V4L |
| 17 | 아날로그 디바이스 - ADC |
| 18 | 펄스 폭 변조 - PWM |
| 19 | 기타 장치 |

`raw/books/gnu-linux-rapid-embedded.md`

## 특징
- **주변장치 실습 15장(6-19장)** — 각 장이 하나의 하위 시스템(GPIO/시리얼/USB/I2C/…)을 다룸
- 커널·드라이버(3장)를 실습의 출발점으로, "드라이버 없이 보드를 못 쓴다"는 관점
- JFFS2·UBIFS 같은 임베디드 파일시스템(5장)을 커스텀 rootfs로 올림

## 핵심 컨셉 연결
- [[embedded-linux-stack]] — 4단계 파이프라인의 "주변장치 실습" 관점
- [[embedded-linux-build]] — 커널·드라이버·rootfs를 레시피로 조립하는 자동화
- [[embedded-firmware-basics]] — 스타트업 코드/부트로더/버스의 관점 비교
- [[embedded-linux-yocto-project]] — 이 책(주변장치 실습) vs 그 책(레시피/BitBake)

## Related
- 저자: 로돌포 지오메티 (Giometti)
- 개념: [[embedded-linux-stack]], [[embedded-linux-build]], [[embedded-firmware-basics]]
- 보드: [[raspberry-pi-iot]], [[bbb-yocto-project]]
