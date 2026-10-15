---
title: 유닉스 고급 프로그래밍 (APUE)
created: 2026-10-15
updated: 2026-10-15
type: entity
tags: [book, programming, os, unix, ipc, signals, compiler]
sources: [raw/books/unix-advanced-programming.md]
confidence: high
---
# 유닉스 고급 프로그래밍 (APUE 2판, 홍릉과학출판사 번역)

> 원저 W. Richard Stevens, Addison-Wesley(APUE 2판, ISBN 0-201-88854-8). 한국어 번역은 홍릉과학출판사가 Addison-Wesley 정식 계약에 의하여 발행 `[raw/books/unix-advanced-programming.md]` 저작권표기/역자서

유닉스 API의 **시스템콜·라이브러리 함수를 19개 장으로 체계 정리**한 프로그래밍 표준 교재. "유닉스가 제공하는 서비스 — 화일 열기, 프로세스 생성, 신호, 단말기, 프로세스간 통신 — 을 함수 단위로 자세히 알고자 하는 개발자"를 독자로 명시(서문). 4.3BSD 중심 용어로 서술하며 예제는 4개 유닉스 버전에서 실행 검증.

## 19개 장 구조 (TOC p15-19, 본문 시작 확인)
| 장 | 제목 | 시작(약) |
|----|------|---------|
| 1 | 소개 (Introduction) | p16 |
| 2 | 유닉스 표준화와 구현 | p30대 |
| 3 | 화일 입출력 (File I/O) | p78 |
| 4 | 화일과 화일명부 (Files and Directories) | p102 |
| 5 | 표준 입출력 (I/O) 모음 | p176 |
| 6 | 시스템 데이타 화일과 정보 | p210대 |
| 7 | 유닉스 프로세스 환경 | p230대 |
| 8 | 프로세스 제어 | p242 |
| 9 | 프로세스 관계 | p278 |
| 10 | 신호 (Signals) | p324 |
| 11 | 단말기 입출력 | p378 |
| 12 | 고급 입출력 (Advanced I/O) | p418 |
| 13 | 파수꾼 프로세스 (Daemon Processes) | p460대 |
| 14 | 프로세스간 통신 (IPC) | p482 |
| 15 | 고급 프로세스간 통신 (Advanced IPC) | p562 |
| 16 | 데이타베이스 모음 (DBM/ndbm...) | p584 |
| 17 | 포스트스크립트 인쇄기와의 통신 | p624 |
| 18 | 전화 걸기 (Modem Dialer/시리얼) | p664 |
| 19 | 의사 단말기 (Pseudo-Terminal) | p714 |

## 특징
- **함수(인터페이스) 중심 서술** — 매 장이 "시스템콜/함수 시그니처 → 동작 → 예제 코드 → 주의점". 개념 설명보다 *호출 패턴*을 보여주는 실용서
- **I/O 계층 3단계** (3장 File I/O → 5장 표준 I/O → 12장 고급 I/O): 저역에서 "모음"(stream)으로 번역된 I/O 흐름 단계별 심화
- **프로세스 3부(8·9·10장)**: 제어(fork/exec/wait) → 관계(부모/자식, 세션) → 신호 — 유닉스 프로그래밍의 핵심 삼각형
- **IPC 2부(14·15장)**: 파이프·펩·FIFO → 메시지 큐·세마포어·공유 메모리(System V+POSIX)
- **실무 특수 영역**(16~19장): DBM 데이타베이스, 포스트스크립트, 시리얼/모뎀 다이얼, 의사 단말기 — "유닉스 서비스"의 넓은 스펙트럼
- 2판 서술 기준은 **4.3BSD + ANSI C 표준(X3.109) + POSIX(IEEE 1003.1)** — 현대 Linux 프로그래밍의 개념 토대를 제공

## 핵심 컨셉 연결
- [[unix-ipc-signals]] — 14·15장(IPC) + 10장(신호)의 통합 정리
- [[gcc-compilation-pipeline]] — 이 책이 설명하는 대상이 gcc로 컴파일되는 C 라이브러리/시스템콜
- [[software-configuration-management]] — 유닉스 세계의 "빌드·버전" 관행(8장 프로세스 제어와 연결)

## OCR 노트
- 장 번호는 TOC(p15-19)와 본문 페이지(각 `제N장` 헤더)를 교차 확인. OCR이 5/6/7장 번호를 혼동(예: "제 5장 시스템 데이타" vs "제 6장 시스템 데이타") → APUE 표준 장 목록으로 정정 기록
- "모음"은 I/O stream(표준 입출력), "파수꾼"은 Daemon, "화일명부"는 directory, "의사 단말기"는 pseudo-terminal(pty)의 한국어 번역
