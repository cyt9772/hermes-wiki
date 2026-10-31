---
title: 리눅스 커널과 디바이스 드라이버 실습 (2판)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, programming, device-driver, embedded-linux]
sources: [raw/books/linux-kernel-device-driver-practice.md]
confidence: high
---
# 리눅스 커널과 디바이스 드라이버 실습 (2판)

> 국내 원서: 정재준 지음, 커널연구회(www.kernel.bz)
> 발행인 정재춘, **초판 2012-04, 2판 2013-05**, ISBN 978-89-97750-05-4, 603p / 18장+

## 개요
리눅스 커널의 내부 구조와 디바이스 드라이버 개발을 "자료구조→프로세스→인터럽트→구체 버스 드라이버" 실험 순으로 실습하는 한국 원서다. 저자는 [[jeong-jae-jun]]이며, 같은 커널연구회의 [[linux-kernel-source-beginner]]와 [[device-tree-kernel-4-0]]로 이어진다. 부록I은 커널 버전별 특징 비교로 정리되어, 여러 커널 버전에서 드라이버를 다룰 실무자의 참고서로도 쓰인다.

## 장 구조 (2부 구성, 18장+부록I)
**제1부 리눅스 커널 이해 및 실습**
| # | topic | 핵심 |
|---|-------|------|
| 1 | 커널 자료구조 | linked list / queue / tree, 데이터 구조 선택·알고리즘 효율 |
| 2 | 프로세스 | 프로세스·스레드 이해, 문맥 교환, 스케줄링(자료구조·우선순위·정책·run queue·wait queue) |
| 3 | 인터럽트 | interrupt/exception, 핸들러 등록, softirq/tasklet/work queue(하프) |
| 4 | 동기화 | 보호 영역·경쟁 조건, locking, 동기화 방법들과 사례 |
| 5 | 시간 | HZ(tick rate), 하드웨어 시계·타이머, 지연 실행 |
| 6 | 메모리 | 메모리 관리 기법, 주소 변환, slab/slob/slub 할당 |
| 7 | 자료구조 실습 | linked list / queue / red-black tree 실습 |

**제2부 리눅스 디바이스 드라이버 실습**
| # | topic | 핵심 |
|---|-------|------|
| 8 | 커널 내부 들여다보기 | 부팅, 커널/사용자 모드, 커널 타이머, 동시성, 프로세스 파일시스템 |
| 9 | 커널 내 기능 | 커널 스레드, 헬퍼 인터페이스 |
| 10 | 기본 원리 | 커널 모듈 프로그래밍, 장치·드라이버 기본, 인터럽트 핸들링 |
| 11 | 문자 드라이버 | 문자 드라이버 기초, CMOS 예제, 가상 문자 드라이버, 플랫폼 디바이스 |
| 12 | 직렬통신 | 계층 구조, UART, TTY, line discipline |
| 13 | I2C 버스 | I2C 인터페이스, RTC 드라이버 예제 |
| 14 | PWM·ADC | PWM 드라이버, ADC 드라이버 |
| 15 | 입력장치 | 입력 이벤트·입력 장치 드라이버 |
| 16 | PCI | 주소·식별, PCI 영역 접근, DMA, ISA 모뎀 카드 예제 |
| 17 | USB | USB 구조, 드라이버 데이터 구조, 실습예제(USB-FT245) |
| 18 | 비디오 | 디스플레이 구조, framebuffer, 콘솔 드라이버 |
| 부록I | 커널 버전별 특징 | 커널 버전별 특징 비교 |

## 특징
- **2부 18장 구조**: 1부(1-7장) 커널 내부 이해·자료구조 실습, 2부(8-18장) 디바이스 드라이버 실습으로 분리.
- **순차 실습 흐름**: 자료구조→프로세스→인터럽트→동기화→시간→메모리→드라이버로 "안에서 밖으로" 실험.
- **임베디드 버스 집합**: PWM·ADC·I2C·직렬(UART/TTY)·PCI·USB·비디오 — [[linux-device-driver-in-code]]보다 버스 실전 비중이 높은 한국 책.
- **커널 버전별 특장 부록(부록I)**: 커널 버전별 특징 비교 정리, 실무 유지보수에 유용.

## 핵심 컨셉
- [[jeong-jae-jun]] — 저자(커널연구회 운영)
- [[linux-kernel-source-beginner]] — 같은 저자의 최신 커널 소스 단계 해설
- [[device-tree-kernel-4-0]] — 같은 저자의 Device Tree 심층 분석
- [[linux-kernel-structure]] — 프로세스·동기화·메모리·장치모델 공통 축
- [[linux-kernel-development-love]] — 개념 지도 상위서
