---
title: 라즈베리파이·아두이노 기반 IoT 실습 클러스터
created: 2026-11-07
updated: 2026-11-07
type: concept
tags: [raspberry-pi, arduino, iot, gpio, web-server, python, concept]
sources:
  [raw/books/raspberry-pi3-iot.md,
   raw/books/raspberry-pi4-iot-linux.md,
   raw/books/raspberry-pi-iot-im.md,
   raw/books/raspberry-pi-projects.md,
   raw/books/arduino-complete.md]
confidence: high
---
# 라즈베리파이·아두이노 기반 IoT 실습 클러스터

**라즈베리파이(PI 3/4)+ 아두이노** 보드를 활용한 IoT(사물인터넷)·웹·하드웨어 프로젝트를 단계별로 실습하는 실무서 묶음. 5권 모두 "보드 설치 → 리눅스/파이썬/GPIO → 센서/액추에이터 → 웹 서버/통신 → 종합 프로젝트"의 5단계를 공유하지만, 깊이가 다르다.

## 5단계 학습 곡선
1. **보드 설치·부팅** — RPI·BBB·아두이노 보드 구조·전원·케이스. `raw/books/raspberry-pi3-iot.md` 제1-2장, `raw/books/raspberry-pi-projects.md` Part 1, `raw/books/arduino-complete.md` 제1-2장
2. **리눅스·파이썬 기초** — 리눅스 명령어·셸·파일시스템. `raw/books/raspberry-pi4-iot-linux.md` 제2-3장, `raw/books/raspberry-pi-iot-im.md` 제2-4장
3. **GPIO·하드웨어 제어** — LED·버저·센서(CDS/DHT11). `raw/books/raspberry-pi3-iot.md` 제5-8장, `raw/books/raspberry-pi4-iot-linux.md` 제3장, `raw/books/arduino-complete.md` 제3-4장
4. **웹·통신** — Flask·WebSocket·RDP·SSH·시리얼(RS232)·이더넷. `raw/books/raspberry-pi4-iot-linux.md` 제5-8장, `raw/books/arduino-complete.md` 제4-7장
5. **종합 프로젝트** — 로봇 탱크·쿠토크서·RC차·3D프린터, AI(딥러닝). `raw/books/raspberry-pi4-iot-linux.md` 후반부, `raw/books/raspberry-pi-projects.md` Part 2-5

## 보드별 특화
| 보드 | 장수 | 특징 |
|------|------|------|
| Raspberry Pi 3 | 384p | IoT 실습·SSH·VNC·웹 |
| Raspberry Pi 4 | 941p | 리눅스 체계·딥러닝·종합 |
| Raspberry Pi | 615p | 리눅스+파이썬+웹+IOT |
| arduino UNO R3 | 288p | 전기·전자 기초→센서→프로젝트 |

## Related
- 상위 개념: [[iot]], [[microcontroller-arduino]]
- 보드·하드웨어: [[embedded-systems-firmware]], [[linux-device-driver-in-code]]
- 언어: [[linux-shell-scripting]], [[arduino-complete]]
