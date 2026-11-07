---
title: 사물인터넷(IoT)을 위한 라즈베리파이 3 활용 (개정판)
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, raspberry-pi, iot, gpio, python, web-server]
sources: [raw/books/raspberry-pi3-iot.md]
confidence: high
---
# 사물인터넷(IoT)을 위한 라즈베리파이 3 활용 (개정판)

> 저자: 정원석
> 국내서 | 광문각, 2017
> 384p `raw/books/raspberry-pi3-iot.md`

## 개요
Raspberry Pi 3 보드 위에서 IoT 실습을 시작하는 국내 입문서. 1부(1-8장)에서 보드 설치-SSH/VNC 원격 접속-시스템 설정-파이썬 기초를 다지고, 2부(9-16장)에서 리눅스 장치-시리얼 통신-하드웨어 제어(감속모터/스텝모터)로 넘어가며, 후반부에서 웹 서버(Flask)와 하드웨어 연결까지 실습 `raw/books/raspberry-pi3-iot.md`.

## 장 구조 (16장+)
| 장 | 제목 |
|----|------|
| 1 | 라즈베리파이(RaspberryPi)란 |
| 2 | Host PC에서 라즈베리파이 연결하기 (SSH기반 제어·시리얼) |
| 4 | 라즈베리파이 시스템 설정 (raspi-config·한글·네트워크) |
| 7 | 나노(NANO) 편집기 |
| 8 | USB 부팅 |
| 9 | 파이썬 기초 |
| 14 | 리눅스 장치 |
| 15 | 시리얼 통신이란 |
| 16 | 하드웨어 제어 (감속모터·스텝모터) |

`raw/books/raspberry-pi3-iot.md`

## 특징
- **원격 접속 3종(SSH·시리얼·RDP/VNC)** 을 제2, 6장 전후로 집중 실습
- 보드·OS 설치 → 셸/파일시스템 → 파이썬 → GPIO/모터 제어 → 웹 서버 순의 학습 곡선
- 웹 서버(8장)와 데이터베이스(11장)를 IoT 실습으로 연결

## 핵심 컨셉 연결
- [[raspberry-pi-iot]] — RPI·아두이노 기반 IoT 클러스터
- [[arduino-complete]] — 아두이노 입문서와의 비교 (보급형 MCU vs SBC)
- [[microcontroller-arduino]] — MCU/아두이노 개념
- [[iot]] — 사물인터넷 상위 개념
- [[linux-shell-scripting]] — 리눅스 셸 기초

## Related
- 저자: 정원석
- 개념: [[raspberry-pi-iot]], [[microcontroller-arduino]], [[iot]]
- 보드: [[arduino-complete]], [[raspberry-pi4-iot-linux]]
