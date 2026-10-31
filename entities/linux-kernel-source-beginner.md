---
title: 리눅스 커널 소스 해설 [기초입문]
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, programming]
sources: [raw/books/linux-kernel-source-beginner.md]
confidence: high
---
# 리눅스 커널 소스 해설 [기초입문]

> 국내 원서: 정재준 지음, 커널연구회(www.kernel.bz)
> **발행 2020-03**, ISBN 978-89-97750-13-9, 353p

## 개요
최신 리눅스 커널 소스를 "단계별로 쉽게 풀어 설명"하는 입문서다. 커널 소스를 처음 다루는 사람들을 위해 빌드·코딩 형식·데이터 타입부터 시작해 커널 자료구조(linked list→red-black tree→XArray)·모듈·성능 측정(perf)·ftrace·crash 도구·kprobes·debug objects·kobject·자료구조 실습까지 하나의 흐름으로 정리한 한국 원서다. 저자는 [[jeong-jae-jun]]이며, 같은 커널연구회의 [[linux-kernel-device-driver-practice]]와 [[device-tree-kernel-4-0]]로 이어지는 커널 학습 경로의 "소스 입문 단계"를 담당한다.

## 장(주제) 구조 — 소스 읽기 → 실습 → 디버깅
| 블록 | topic | 핵심 |
|------|-------|------|
| 1 | 커널 소스 빌드·버전관리 | 커널 소스 다운로드, 빌드·설치, 버전업 |
| 2 | 커널 소스 코딩 형식 | 들여쓰기·긴 줄·괄호·공백·작명·타입 재정의, 함수·goto·주석, macro/enum/inline·커널 매크로·C 속성·inline assembly |
| 3 | 커널 데이터 타입·비트·비트맵 | 커널 데이터 타입 이해, 비트 단위 연산, 비트맵 |
| 4 | 커널 모듈·sort·성능 | 커널 모듈 프로그래밍, 커널 sort 테스트, perf(perf record/report/probe, 소스 빌드) |
| 5 | ftrace | 이벤트/함수/함수 그래프 추적, 중요 옵션 |
| 6 | crash | 설치·실행(kdump/덤프파일), backtrace/ps/struct/task/vm/kmem/sym/p/list/tree/foreach 명령 |
| 7 | kprobes · debug objects | kprobes 이해, debug objects 개념·함수(init/free/activate/deactivate)·활용, 커널 디버그 메시지 출력(레벨) |
| 8 | kobject · 자료구조 실습 | kobject 이해, user memcpy·커널 메모리 주소·list sort·red-black tree·XArray 이해 |

## 특징
- **최신 커널 소스 단계 해설**: 빌드부터 자료구조 실습까지 커널 소스를 "어떻게 읽는지"를 단계별로 지도.
- **디버그 도구 세트**: perf · ftrace · crash · kprobes · debug objects 가 하나의 실습 흐름으로 연결.
- **자료구조 3종**: linked list / red-black tree / XArray — 커널 내부 컨테이너를 직접 실습.
- **한국 원서**: 커널연구회(www.kernel.bz)의 커널 교육 로드맵의 입문 단계.

## 핵심 컨셉
- [[jeong-jae-jun]] — 저자(커널연구회 운영)
- [[linux-kernel-device-driver-practice]] — 같은 저자의 드라이버 실습(2부 18장)
- [[device-tree-kernel-4-0]] — 같은 저자의 Device Tree 심층 분석
- [[linux-kernel-structure]] — 프로세스·동기화·메모리·장치모델 공통 축
- [[linux-kernel-development-love]] — 개념 지도 상위서
