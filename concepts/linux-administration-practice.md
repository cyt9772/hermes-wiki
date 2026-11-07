---
title: 리눅스 관리 / 쉘 / 커널 프로그래밍 연습 (실무 3권 클러스터)
created: 2026-11-07
updated: 2026-11-07
type: concept
tags: [linux, shell, kernel, intro, system-management, concept]
sources:
  - raw/books/linux-10min-guide.md
  - raw/books/linux-mania-tutorial.md
  - raw/books/linux-kernel-programming-mania.md
  - raw/books/linux-kernel-development-love.md
  - raw/books/linux-shell-scripting-kim.md
confidence: high
---

## 개요

리눅스 사용자 실무 3권 클러스터. `raw/books/linux-10min-guide.md`와 `raw/books/linux-mania-tutorial.md`는 쉘·기본 명령·프로세스·네트워킹·시스템 관리까지 다루는 입·중급 사용서이며, `raw/books/linux-kernel-programming-mania.md`는 같은 독자를 넘겨 커널 내부 구조와 직접 커널 프로그래밍·드라이버까지 다룬다. 세 책은 서로 다른 난이도와 목적을 갖고 리눅스 사용→관리→커널 개발의 학습 경로를 이룬다.

## 3권 비교

| 책 | 특징 |
|---|---|
| `raw/books/linux-10min-guide.md` | 개념(유닉스·GNU·POSIX) → 설치 → 기본 명령 → bash → 개발환경 → 네트워킹 → X Window → 시스템 관리(부팅/사용자/파일시스템/메모리) 순. 9장 구성. |
| `raw/books/linux-mania-tutorial.md` | Paul Sheer 원서(`LINUX: A USER'S TUTORIAL AND EXPOSITION`, Pearson Education/Prentice Hall PTR 2002)의 한국어판. 기초 연산(2/8/10/16진수)에서 시작해 기본 명령, 정규 표현식, vi, 쉘 스크립트, sed, 프로세스, 메모리, 퍼미션, 심볼릭/하드 링크, 유닉스 디렉토리 구조, 디바이스, 파티션·파일시스템·마운팅, 고급 쉘 스크립트, C, 공유 라이브러리, grep, TCP/UDP, DNS, NFS, 메일 서비스, uucp/uux, 유닉스 파일시스템 표준까지. 30장 이상. |
| `raw/books/linux-kernel-programming-mania.md` | "눈으로 보는 책이 아니라 손으로 보는 책"(百見不如1打). 학부 OS 수강자 대상. 리눅스 역사 → 커널 구조·컴파일/리빌드 → 시스템 호출 구현 → 태스크 관리(task_struct·스케줄링) → 메모리 관리 → 모듈 프로그래밍 → 파일시스템(inode·ext2) → 디바이스 드라이버(문자·블록·네트워크) → 통신 프로토콜 → 11장 SnapFS(커널 레벨 검사점/복구 도구) 프로젝트. |

## 학습 경로

1. **개념·쉘·파일·명령**: [[linux-shell-scripting]] — 10min-guide 제2~4장, mania-tutorial 제3~7장.
2. **시스템 관리·네트워킹**: 10min-guide 제6·8장, mania-tutorial 제26~30장(TCP/UDP·DNS·NFS·메일).
3. **커널 구조**: [[linux-kernel-structure]] — kernel-mania 제2·3장, 이후 [[linux-kernel-development-love]]로 심화.
4. **커널 프로그래밍·드라이버**: kernel-mania 제7·9장 → [[linux-kernel-programming-itepert]], [[linux-kernel-source-beginner]].
5. **임베디드 맥락 확장**: [[embedded-linux-stack]], [[embedded-linux-build]], [[embedded-firmware-basics]].

## Related

- 쉘/스크립트: [[linux-shell-scripting]], [[linux-essential-utilities]]
- 커널 구조/개발: [[linux-kernel-structure]], [[linux-kernel-development-love]], [[linux-kernel-programming-itepert]], [[linux-kernel-source-beginner]]
- 드라이버/디바이스: [[linux-device-driver-in-code]], [[linux-kernel-device-driver-practice]]
- 임베디드 확장: [[embedded-linux-stack]], [[embedded-linux-build]], [[embedded-firmware-basics]], [[embedded-linux-systems-arm-an]], [[embedded-linux-yocto-project]]
- C 기반 심화: [[beginning-linux-programming]], [[professional-linux-programming-wrox]], [[mastering-embedded-linux-programming]]
