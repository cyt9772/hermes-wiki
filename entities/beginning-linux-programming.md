---
title: Beginning Linux Programming (비기닝 리눅스 프로그래밍)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, programming, linux, unix, os, ipc, shell-scripting]
sources: [raw/books/beginning-linux-programming.md]
confidence: high
---

# Beginning Linux Programming (비기닝 리눅스 프로그래밍)

> 원서: Beginning Linux Programming (Wrox Press, ISBN 1-874416-65-6). 저자: Neil Matthew·Richard Stones 공저. 번역: 이태용 역. 한국: 보문사, ISBN 89-7627-673-6, 1197쪽. 개정판 번역본 (원서 연도 OCR상 불분명) `[raw/books/beginning-linux-programming.md]`

Wrox 계열의 **리눅스 C 프로그래밍 입문·중급 교재** 개정판의 한국어 번역. 역자서는 당대의 두 사건 — Y2K 오류와 "리눅스의 도약" — 에서 출발해, 이 책은 "모두의 운영체제"를 향한 보급을 위해 기본 개념(컴파일·링크)부터 시스템 프로그래밍까지 한 권으로 정리하는 안내서라고 포부 밝힌다 `[raw/books/beginning-linux-programming.md]`. 초판 대비 개정판이라 최근 흐름을 반영한 주제들이 추가되어 입문자와 고급자 모두를 겨냥한다.

## 구조 (TOC, OCR 장 번호 교정)
| 장 | 테마 | 쪽 |
|----|------|----|
| 2 | 쉘 프로그래밍 | 57 |
| 4 | 유닉스 환경 (OCR 장 번호 혼용) | - |
| 6 | curses | 269 |
| 7 | I/O 관리 | 323 |
| 8 | 개발 도구 | 395 |
| 9 | 디버깅 | 443 |
| 10 | 프로세스와 시그널 | 481 |
| 11 | POSIX 스레드 | 523 |
| 12 | IPC: 파이프 | 561 |
| 13 | 명령어(신호 추정)·메시지큐·공유메모리 | 629 |
| 14 | 소켓 | 669 |
| 15 | TCL | 713 |
| 16 | X 프로그래밍 | 759 |
| 19 | 인터넷: HTML | 955 |
| 20 | CGI | 999 |

## 특징
- **쉘 → C → 시스템 호출 → IPC → 소켓 → GUI(TCL/X) → 웹(HTML/CGI)** 라는 단일 상승 축. 2장 쉘 프로그래밍으로 시작해 12~14장 프로세스·IPC·소켓으로 고도화되고 15~20장으로 GUI·웹으로 확장 `[raw/books/beginning-linux-programming.md]`
- 8장(개발 도구)·9장(디버깅)은 리눅스 C 개발 도구 체인(컴파일·디버거)을 실용 구간으로 배치 — [[gcc-compilation-pipeline]]과 [[linux-essential-utilities]]가 심화하는 바로 그 도구들
- 10장 프로세스와 시그널, 11장 POSIX 스레드, 12~13장 IPC는 이 클러스터의 [[unix-process-ipc]] 축에서 Wrox 입문 축을 이룸
- 저자 쌍은 Wrox 두 권(본서 + [[professional-linux-programming-wrox]])을 함께 쓴 [[neil-matthew]]·[[richard-stones]]

## 핵심 컨셉 연결
- [[unix-process-ipc]] — 10~14장 프로세스/시그널/스레드/IPC/소켓 축
- [[linux-shell-scripting]] — 2장 쉘 프로그래밍 (p57)
- [[unix-ipc-signals]] — 같은 신호·IPC 영역의 APUE 심화 축과 비교
- [[gcc-compilation-pipeline]] / [[linux-essential-utilities]] — 8·9장 개발 도구·디버깅의 실용 counterpart

## OCR 노트
- TOC 장 번호 OCR 혼용 (예: "7데4장 유닉스 환경"). 'Beginning' 표준 22장 구성으로 교정 후 기록
- 13장 "명령어"는 "신호(signals)"의 OCR 오류로 추정
- 표지/제목면 연도 미확인 — 원서 OCR상 초판 발행 연도 불분명 (raw 메타데이터 명시)
- 1197쪽 (pdfinfo)
