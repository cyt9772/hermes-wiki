---
title: 유닉스 시스템 프로그래밍 (Haviland·Salama)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, programming, unix, os, ipc]
sources: [raw/books/unix-system-programming-homling.md]
confidence: high
---

# 유닉스 시스템 프로그래밍 (UNIX System Programming)

> 원서: UNIX System Programming (1987). 저자: Keith Haviland · Ben Salama 공저. 번역: 홍릉과학출판사 편집부 역. 한국: 홍릉과학출판사, 발행자 이연우, 1991-01, 429쪽 `[raw/books/unix-system-programming-homling.md]`

1990년대 초 한국시장에 풀린 **유닉스 시스템 프로그래밍 입문서**의 한국어 번역. 역자서문은 이 책의 대상 독자 — "UNIX에 기본적 지식을 갖추고 커널과 응용소프트웨어를 연결하는 프로그래밍 인터페이스를 이용하려는 사람" — 과, "모든 예가 C언어로 작성된 수행가능한 예제프로그램이 풍부"하다는 특징을 명확히 밝힌다. 비교 대상으로는 Bach의 `THE DESIGN OF THE UNIX OPERATING SYSTEM`(1986)를 들고, 본서가 "실제 프로그래밍에 필요한 부분을 중점적으로 다룬다"는 차이를 강조 `[raw/books/unix-system-programming-homling.md]`.

## 구조 (TOC, 11장)
| 장 | 테마 |
|----|------|
| 2 | 화일 |
| 3 | 화일에 대한 여러 가지 |
| 4 | 디렉토리 |
| 5-7 | 프로세스 (통신: 파이프 → System V 추가 기법) |
| 8 | 단말기 |
| 9 | 라이브러리 |
| 10 | curses |
| 11 | 기타 시스템호출 |

## 특징
- **입문자 눈높이의 시스템 호출 지도** — 2-4장(화일·디렉토리), 5-7장(프로세스·통신·통신 추가 기법), 8장(단말기)의 세 구간으로 유닉스 API의 "기본 골격"을 잡는 구성 `[raw/books/unix-system-programming-homling.md]`
- 5-7장의 "파이프 → System V 추가 기법" 전이는 **파이프(간단) → 세마포어/공유메모리(고급)** 라는 IPC 고도화 경로 — [[unix-process-ipc]]의 "단계별 IPC" 스키마와 정확히 부합
- 1987년 원서 기준이라 C(ANSI 전)와 4.3BSD/SysV 초기 시점의 API. 2000년 이후 POSIX/ISO C 환경에서는 부분적 불일치가 있으나 **개념 구조의 안정성은 유지**
- Bach 커널 설계서와 대비 — "커널 내부"가 아니라 **"커널과 대화하는 인터페이스"에 집중한다"는 역자서문의 포지셔닝이 책의 정체성

## 핵심 컨셉 연결
- [[unix-process-ipc]] — 5-7장 프로세스/통신·IPC 축 (초기 유닉스 관점)
- [[unix-ipc-signals]] — 시그널·IPC의 APUE 심화 축과 대비
- [[unix-network-programming-ste]] — IPC 특화권 (System V 세마포어·공유메모리 심화)
- [[unix-advanced-programming]] — APUE와의 대비: 본서는 1987 초기 유닉스, APUE는 1990년대 후반

## OCR 노트
- 원서 출판사 McGraw-Hill, 1987. 한국판 ISBN 원문 표기 없음 (raw 메타데이터 "원문에 표기 없음")
- 제목면 '흥룡', 역자서문 '홍릉' — 원문에 두 표기 모두 존재, '홍릉과학출판사'로 통일
- 발행자 '이연우'
- 429쪽 (pdfinfo)
