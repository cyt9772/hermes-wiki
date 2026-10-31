---
title: 디바이스 트리 상세 분석 in Linux Kernel 4.0
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, device-driver, device-tree, embedded-linux]
sources: [raw/books/device-tree-kernel-4-0.md]
confidence: high
---
# 디바이스 트리 상세 분석 in Linux Kernel 4.0

> 국내 원서: 정재준 지음, 커널연구회(www.kernel.bz), 발행인 정재춘
> **2015**, ISBN 978-89-97750-06-1, 314p / 12장 + 부록I

## 개요
Linux Kernel 4.0의 Device Tree (DT) 소스를 "DTS 문법→실용 표현→실습→UART 드라이버 상세분석" 4단계로 풀어낸 한국 원서다. DTS 기본 문법(CPU/메모리/인터럽트/compatible/addresses/chosen 노드)에서 시작해, CPU·메모리·CLOCK·PCI·MMC·I2C·USB 등 실제 SoC DTS에서의 디바이스 표현을 실용 분석하고, Samsung(Exynos 계열) SoC 보드를 대상으로 개발 환경 구축→U-Boot 빌드→커널 포팅→UART/GPIO/USB 드라이버까지 실습을 진행한다. UART(8250) 드라이버의 구조체·등록·포트 등록·probe·TX/RX 흐름을 코드 단위로 깊이 파헤치는 5-12장이 이 책의 핵심이다. 저자는 [[jeong-jae-jun]]이며, 같은 커널연구회의 [[linux-kernel-device-driver-practice]]와 [[linux-kernel-source-beginner]]와 함께 커널 연구 로드맵을 구성한다.

## 장 구조 (12장 + 부록I)
| # | topic | 핵심 |
|---|-------|------|
| 1 | 작업환경 및 소스경로 | 개요, 작업환경, DT 소스 경로 |
| 2 | DT 소스 분석 | DTS 문법, 기본 예제(CPU/노드/I/O/compatible), 주소 표현(regions), 인터럽트 표현, special nodes(chosen) |
| 3 | DT 실용 분석 | CPU·메모리·인터럽트·CLOCK·PCI·MMU·MMC·I2C·SPI·UART·PWM·ADC·USB·TMU·멀티미디어 표현 |
| 4 | DT 실습 | Samsung(Exynos 계열) 보드, 개발 환경(Ubuntu·크로스 컴파일러), U-Boot 빌드, SD카드 부팅, 커널 포팅, 보드 소스 분석, GPIO/시리얼/USB 드라이버 |
| 5 | UART 드라이버 상세분석 | UART 구조체, 드라이버 등록, 포트 등록, 동작, 실행 함수 |
| 6 | UART 구조체 | UART_DRIVER / CONSOLE / UART_STATE / TTY_DRIVER / TTY_PORT / UART_PORT / UART_8250_PORT / TTY_OPERATIONS / UART_OPS / TTY_STRUCT / TTY_ICOUNT / LINE_DISC / TTY_BUFFER |
| 7 | UART 드라이버 등록 | serial8250_init(), uart_register_driver(), tty_register_driver() |
| 8 | UART 포트 등록 | serial8250_register_ports(), uart_add_one_port(), serial8250_isa_init_ports() |
| 9 | UART 8250 동작 | serial8250_probe()/suspend()/resume(), 인터럽트 동작(receive_chars / transmit_chars) |
| 10 | Samsung UART 동작 | 드라이버 등록, 포트 정보, probe, 동작, TX chars, RX chars |
| 11 | TTY 실행 함수 | tty_register_driver / tty_open / tty_read / tty_write |
| 12 | UART 실행 함수 | I/O 함수, uart_open / uart_write |
| 부록I | SENSOR 정보 요약 | photoresistor / phototransistor / distance / infrared / ultrasonic |

## 특징
- **Kernel 4.0 DT 특화**: 이 시대의 DT 표준(Arch/ARM, Device Tree binding)을 코드 단위로 분석.
- **UART(8250) 깊이 해설**: 5-12장까지 TTY/UART 구조체→등록→probe→TX/RX→Samsung 커스텀까지 — 커널 TTY/char device 코드를 가장 자세히 파헤친 한국 서교.
- **SoC 실습**: Samsung(Exynos 계열) 보드에서 U-Boot → 커널 → DT → 드라이버까지 전 과정.
- **부록I 센서**: photoreceptor/거리/적외선/초음파 센서 요약 — 임베디드 센서 드라이버 기초.

## 핵심 컨셉
- [[jeong-jae-jun]] — 저자(커널연구회 운영)
- [[linux-kernel-device-driver-practice]] — 같은 저자의 18장 드라이버 실습서(동반 서)
- [[linux-kernel-source-beginner]] — 같은 저자의 커널 소스 입문 해설
- [[linux-kernel-structure]] — 커널 구조 공통 축(장치모델 중심)
- [[linux-device-driver-in-code]] — 같은 장비를 더 넓게(23장) 다룬 번역서
