---
title: 매니아를 위한 리눅스 커널 프로그래밍
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, linux-kernel, kernel-programming, syscalls, task, memory, modules, drivers, communication]
sources: [raw/books/linux-kernel-programming-mania.md]
confidence: high
---
# 매니아를 위한 리눅스 커널 프로그래밍

> 저자: 조유근 · 홍지만 · 최종무
> 국내서 | 교학사, 2001
> 502p `raw/books/linux-kernel-programming-mania.md`

## 개요
**리눅스 커널 2.4 시대의 커널 프로그래밍을 구조부터 실전(프로젝트)까지** 다룬 국내 교재. 리눅스의 역사와 커널 구조 - 시스템 호출 구현 - 태스크 관리 - 메모리 관리 - 모듈 - 파일시스템 - 디바이스 드라이버 - 통신 프로토콜 - Snap FS 프로젝트의 순으로 이어진다 `raw/books/linux-kernel-programming-mania.md`.

## 장 구조 (11장)
| 장 | 제목 |
|----|------|
| 1 | (서론/리눅스의 역사) |
| 2 | 리눅스의 역사 |
| 3 | 리눅스 커널 구조 (소스 트리) |
| 4 | 리눅스 커널 프로그래밍: 시스템 호출 구현 |
| 5 | 태스크 관리 |
| 6 | 메모리 관리 |
| 7 | 리눅스 모듈 프로그래밍 |
| 8 | 파일시스템 |
| 9 | 디바이스 드라이버 |
| 10 | 통신 프로토콜 |
| 11 | 프로젝트 (Snap FS) |

`raw/books/linux-kernel-programming-mania.md`

## 특징
- 시스템 호출(4장)-태스크(5장)-메모리(6장)을 커널 프로그래밍의 축으로 배치
- 모듈(7장)·드라이버(9장)을 실무 관점으로 다룸
- 마지막 장(11장)이 **Snap FS 프로젝트**로 실전 마무리 — "읽고 끝"이 아닌 "만들고 끝"

## 핵심 컨셉 연결
- [[linux-kernel-structure]] — 커널 구조 개념 (이 책의 축)
- [[linux-kernel-development-love]] — 커널 개발 심화
- [[linux-kernel-programming-itepert]] — IT EXPERT 커널 교재
- [[linux-device-driver-in-code]] — 디바이스 드라이버 코드
- [[linux-mania-tutorial]] — 같은 "매니아/관리" 계열의 OS 활용서

## Related
- 저자: 조유근 · 홍지만 · 최종무
- 개념: [[linux-kernel-structure]]
- 관련: [[linux-mania-tutorial]], [[linux-10min-guide]]
