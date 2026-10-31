---
title: 유닉스 네트워크 프로그래밍 2판 제2권 (IPC)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, programming, unix, networking, ipc, os]
sources: [raw/books/unix-network-programming-ste.md]
confidence: high
---

# 유닉스 네트워크 프로그래밍 2판 제2권 (IPC)

> 원서: UNIX Network Programming, 2nd Ed., Vol 2: IPC (Prentice Hall, 1999). 저자: W. Richard Stevens 저. 번역: 김치하(포항공대)·이재용(연세대) 역. 한국: 교보(제목면 '교보문고' 표기), ISBN 89-7085-468-1, 589쪽, 2000 `[raw/books/unix-network-programming-ste.md]`

W. Richard Stevens의 **유닉스 프로세스간 통신(IPC) 전문 권**. 제1권(Networking APIs)과 비교하여, 같은 저자의 2판 세트 중 "IPC 특화"를 담당하는 제2권이다. 원서 ISBN은 본문에 부분 표기(0-13-020639-3 계열)로, 한국판 ISBN(89-7085-468-1)을 신뢰할 수 있는 확정값으로 기록.

## 구조 (TOC, IPC 메커니즘 축)
| 장 | 테마 | 특징 |
|----|------|----|
| 2 | POSIX IPC | 메시지 큐·세마포어·공유메모리·뮤텍스·조건변수 |
| 6 | System V 메시지 대기열 | `msgget/msgsend/msgrcv/msgctl` |
| 11 | System V 세마포어 | 세마포어 세트, 동시 접근 제어 |
| 14 | System V 공유메모리 | 가장 빠른 IPC, 세마포어와 함께 동기화 |
| 9 | 레코드 잠금 | `fcntl`/`flock`/`lockf` 계열 |

## 특징
- **POSIX vs System V 대조 축** — 2장에서 POSIX IPC 메시지 큐(`mq_open/mq_send/mq_receive`)와 조건변수, 그리고 6/11/14장에서 System V 메시지 대기열·세마포어·공유메모리를 병렬로 다룸. 두 계열의 API 면을 같은 책에서 비교하는 구성 `[raw/books/unix-network-programming-ste.md]`
- Stevens의 2판 제2권이라, **제1권(NET: 소켓·RPC)과 대비**되는 IPC 특화 콘텐츠. 즉 "네트워크 프로그래밍"이라는 전체 세트 안에서 **로컬 IPC** 축을 맡음
- 9장 레코드 잠금(`fcntl` `F_SETLK` 계열)은 IPC와 결합한 동시성 제어 구간
- 함수 프로토콜 인덱스(p.44-589)에 `pipe`/`popen`/`mkfifo`(파이프·FIFO), `pthread_create`(POSIX 스레드), `mmap`/`munmap`/`mlock`/`munlock`(공유메모리 매핑)까지 포함 — **파이프 → System V IPC → POSIX IPC → 스레드 → mmap** 전체 스펙트럼을 한 권에 압축

## 핵심 컨셉 연결
- [[unix-process-ipc]] — 이 클러스터의 유닉스 프로세스/IPC 통합 축 (Ste IPC 심화)
- [[unix-ipc-signals]] — APUE가 다루는 신호+IPC 축과의 교차 (System V vs POSIX)
- [[unix-advanced-programming]] — APUE와의 대비: 본서는 IPC 특화, APUE는 시스템 프로그래밍 전편
- [[unix-system-programming-homling]] — 5-7장(프로세스·통신)의 초기 IPC 입문과 대비

## OCR 노트
- 원서 ISBN 부분 확인만 가능 (본문 0-13-020639-3 계열). 한국판 89-7085-468-1로 확정
- 발행자 '교보' — 제목면 '교보문고' 표기, 발행사 명칭 원문 확인 불명 → '교보'로 기록
- 2000(OCR상 발행연도 불명, 원서 1999)
- 함수 인덱스 OCR에 깨진 토큰 다수 (`msgget` 계열은 명확, 일부는 원문 대조 필요)
- 589쪽 (pdfinfo)
