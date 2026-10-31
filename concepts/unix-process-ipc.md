---
title: 유닉스 프로세스 제어와 IPC 입문
created: 2026-11-01
updated: 2026-11-01
type: concept
tags: [programming, os, unix, signals, ipc]
sources: [raw/books/beginning-linux-programming.md, raw/books/unix-network-programming-ste.md, raw/books/unix-system-programming-homling.md]
confidence: high
---

# 유닉스 프로세스 제어와 IPC 입문

유닉스로 **개별 프로세스를 만들어(fork/exec 계열) 서로 사이로 데이타를 옮기는(IPC)** — 1987년 첫 입문서부터 2000년대 Wrox 교재까지 5권 클러스터가 공통으로 다리는 축. 기존 [[unix-ipc-signals]] 개념이 APUE 기준의 신호·IPC 심화를 다룬다면, 이 페이지는 **Wrox·Stevens·Haviland-Salama 입문권 관점**에서 "파이프 → System V IPC → POSIX IPC/스레드" 고도화 경로를 서별 전개로 정리한다.

## 서별 전개 (입문 → 특화)
| 권 | 장/구간 | 프로세스/IPC 처리 | 스타일 |
|----|---------|------------------|--------|
| [[unix-system-programming-homling]] | 5-7장 (프로세스·통신) | 프로세스 생성 → 파이프 → System V 추가 기법 (세마포어·공유메모리) | 1987 초기 유닉스, 수행가능 C 예제 중심 — IPC를 "통신" 장으로 5-7장에 압축 `[raw/books/unix-system-programming-homling.md]` |
| [[beginning-linux-programming]] | 10~14장 | 10 프로세스와 시그널 / 11 POSIX 스레드 / 12 파이프 / 13 메시지큐·공유메모리 / 14 소켓 | 리눅스 입문 교재 — 시그널·스레드·IPC·소켓을 연속 장으로 배치하고 GUI(X/TCL)·웹(HTML/CGI)으로 확장 `[raw/books/beginning-linux-programming.md]` |
| [[unix-network-programming-ste]] | 2·6·11·14장 | POSIX IPC(메시지큐·세마포어·공유메모리·뮤텍스·조건변수) / System V 3종(메시지대기열·세마포어·공유메모리) / 9장 레코드잠금 | IPC 특화권 — POSIX vs System V를 함수 프로토콜 수준(`msgget·semop·shmget·pthread·mmap`)에서 대조 `[raw/books/unix-network-programming-ste.md]` |

## 공통 구조: IPC 3단계 고도화
세 권 모두 동일한 난이도 계단을 걷는다 — 이 자체가 유닉스 IPC의 표준 교육 경로.
1. **파이프 (pipe, 단방향, 부자 프로세스 간)** — homling 5-7장 "통신", beginning 12장, ste 2장 함수 인덱스(`pipe`/`mkfifo`/`popen`) `[raw/books/unix-system-programming-homling.md]` `[raw/books/beginning-linux-programming.md]` `[raw/books/unix-network-programming-ste.md]`
2. **System V IPC (메시지 큐 · 세마포어 · 공유 메모리)** — 세 권 모두 전담 장. `key_t` + `msgget/semget/shmget` 체계 `[raw/books/unix-network-programming-ste.md]` ch6/11/14
3. **POSIX IPC + 동시성 (뮤텍스·조건변수·스레드·잠금)** — beginning 11장(POSIX 스레드), ste 2장(POSIX 메시지 큐 `mq_*`, 뮤텍스/조건변수), ste 9장(레코드 잠금 `fcntl`)

## 신호(Signal)의 위치
- **시그널은 IPC보다 한 단계 아래**: 데이타 없이 "이벤트 발생"만 통지 — beginning 10장(프로세스와 시그널)이 시그널과 프로세스 제어를 한 장으로 묶는 이유 `[raw/books/beginning-linux-programming.md]`
- 세마포어/잠금으로 IPC 동시성을 제어하는 패턴과, 신호로 경량 통제를 하는 패턴은 같은 "동기화 문제"의 두 무게 `[raw/books/unix-network-programming-ste.md]`
- 신호 상세(재진입, `signal`/`sigaction` 비교, 디폴트 동작)는 [[unix-ipc-signals]]에서 APUE 기준으로 다룸

## 프로세스 제어(생성·종료·대기)
- 기본 축은 세 권 공통: `fork`로 자식 생성 → `exec` 계열로 이미지 교체 → `wait`로 수거. homling "프로세스" 장(5-7장)이 가장 초기 형태로, beginning 10장이 시그널과 결합한 형태로 다룸
- 리눅스 확장 축: beginning 11장 **POSIX 스레드** — "한 프로세스 안의 동시성"으로 IPC의 대안(스택·공유 스택 대신 동시 실행) `[raw/books/beginning-linux-programming.md]`
- 네트워크 확장 축: beginning 14장 소켓 — "유닉스 도메인 소켓으로 로컬 IPC, 인터넷 소켓으로 원격 IPC"의 동형 구조. 이 확장군도 APUE 심화권([[unix-advanced-programming]])과 겹치며, 신호·IPC 전체 체계는 [[unix-ipc-signals]]에서 APUE 기준으로 정리된다

## 관련
- [[unix-ipc-signals]] — 신호·IPC의 APUE 심화 축 (본 페이지의 complement)
- [[unix-advanced-programming]] — APUE: 프로세스(8-10장)·IPC(14-15장) 전체 체계
- [[unix-system-programming-homling]] — 1987 초기 유닉스 11장 구조
- [[beginning-linux-programming]] — 리눅스 입문권 10-14장
- [[unix-network-programming-ste]] — Stevens IPC 특화권 (POSIX vs System V)
- [[gcc-compilation-pipeline]] — 이 모든 함수는 C 라이브러리/시스템콜로, gcc·ld로 링크되어 실행된다