---
title: 리눅스 커널 프로그래밍 (IT EXPERT)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, programming, device-driver]
sources: [raw/books/linux-kernel-programming-itepert.md]
confidence: high
---
# 리눅스 커널 프로그래밍 (IT EXPERT)

> 국내 원서: 한동훈 지음, IT EXPERT 시리즈
> 한빛미디어(주) **초판 2007-07, 재발행 2012-02**, ISBN 978-89-7914-460-4, 1098p / 11장

## 개요
커널을 "읽어서"가 아니라 "코딩해서" 익히자는 국내 실전 입문서다. 각 장에서 커널 API를 실제로 호출하는 프로그램을 작성하고, 그 동작을 다시 소스 분석으로 되돌려 커널 내부 원리를 이해하는 순환 구조를 취한다. 부록 CD에 예제·완성 실습 소스와 VMWare 이미지를 제공해 2.4/2.6 커널 간 차이(EXPORTSYMBOL, 헤더, 모듈 빌드)까지 직접 확인하게 한다. 이 클러스터에서 [[linux-kernel-development-love]]의 개념 지도를 가장 실무 코드로 옮긴 서다.

## 장 구조
| # | topic | 핵심 |
|---|-------|------|
| 1 | 커널 프로그래밍 환경 구축 | VM, 커널 빌드 환경 |
| 2 | 커널 컴파일·소스 분석 | 소스 트리 구조, 빌드 |
| 3 | 시스템 호출 | syscall 직접 이용 |
| 4 | 커널 모듈 | module.c, EXPORTSYMBOL |
| 5 | 문자 디바이스 | char device 드라이버 |
| 6 | proc 파일시스템 | /proc 인터페이스 |
| 7 | 블록 디바이스 | block device 드라이버 |
| 8 | 메모리 관리 | 커널 메모리, 메모리 매핑 |
| 9 | 프로세스 | 자료구조·생성·종료·스케줄링 |
| 10 | 파일시스템 | VFS, ext/proc |
| 11 | 네트워크 | 커널 네트워크 프로그래밍 |

## 특징
- **코딩→분석 순환**: "작성된 프로그램 분석으로 커널 동작원리 이해"를 표방 — 드라이버를 직접 만들며 학습.
- **국내 실무 관점**: IT EXPERT(한빛미디어) 시리즈의 현장 노하우 성격으로, 부록 CD 실습 소스+VM 이미지를 동봉.
- **2.4 ↔ 2.6 버전 대비**: 커널 버전 간 모듈/헤더/심볼 차이를 코드 예시로 병기.
- **드라이버 2형제**: 문자 디바이스(5장)와 블록 디바이스(7장)를 분리 — [[linux-device-driver-in-code]]보다 범위가 좁으나 진입장벽 낮음.

## 핵심 컨셉
- [[linux-kernel-structure]] — 프로세스·메모리·파일시스템·네트워크 공통 축
- [[linux-kernel-development-love]] — 같은 커널 주제의 개념 지도(상위 문서)
- [[linux-kernel-device-driver-practice]] — 한국형 드라이버 실습서(동반 서)
- [[unix-advanced-programming]] — 커널 바깥의 시스템 프로그래밍 기반
