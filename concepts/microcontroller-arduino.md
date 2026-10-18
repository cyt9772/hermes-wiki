---
title: 마이크로컨트롤러·아두이노 (Microcontroller & Arduino)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/practical-electronics-eng.md]
confidence: medium
---
# 마이크로컨트롤러·아두이노 (Microcontroller & Arduino)

## 정의
**내장 메모리(ROM/RAM) + GPIO + 내부 발진기 + 시리얼/USB**를 가진 단일 칩 컴퓨터. 임베디드 시스템의 핵심.

## MCU 기본 구조 (13.1)
- **CPU core** (8/16/32-bit, Harvard/Von Neumann)
- **Flash/ROM** — 프로그램
- **RAM** — 런타임 데이터
- **GPIO (General-Purpose I/O)** — Pin
- **ADC** (analog-to-digital) — 아날로그 → 디지털
- **Timer/Counter** — 타이머, PWM
- **UART/USART/SPI/I²C** — 시리얼 인터페이스
- **Internal Oscillator** — 4/8/16/32/72/100MHz

## MCU 예 (13.2)
- **ATtiny85** — 8-bit AVR, 저가
- **PIC 16Cx** — Microchip 8-bit
- **32-bit MCU** — ARM Cortex-M, STM32
- **DSP (Digital Signal Processing)** — 오디오/통신 신호 처리

## 아두이노 (Arduino) / 13.4
- **아두이노 Uno** — AVR ATmega328P, 16MHz
- **실드(Shield)** — GPIO 확장, RF, 센서
- **라이브러리** — 센서, 디스플레이, 통신
- **예제** — Blink, Serial, PWM
- **오프보드** — 3.3V/5V, USB, GPIO

## MCU 인터페이스 (13.5)
- **스위치** — 입력, 디바운스
- **아날로그 입력** — ADC, 분해능(10/12-bit)
- **고전력 디지털 출력** — MOSFET/트랜지스터 드라이버
- **사운드** — I²S, PWM
- **시리얼** — UART, USB, I²C, SPI
- **준위 변환** — 3.3V ↔ 5V, 분압기/레벨 시프터
- **LED 디스플레이** — 7-segment, LCD

> `raw/books/practical-electronics-eng.md` pp. 849-904

## Related
- [[digital-logic-basics]] — MCU의 GPIO·레지스터
- [[fpga-hdl]] — 하드웨어(HDL) 구현
- [[sensors-electronics]] — 아두이노로 센서 읽기
