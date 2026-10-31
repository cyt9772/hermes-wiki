---
title: 리눅스 쉘 스크립팅 (grep/sed/awk/bash)
created: 2026-11-01
updated: 2026-11-01
type: concept
tags: [programming, linux, shell-scripting, os]
sources: [raw/books/linux-shell-scripting-kim.md, raw/books/beginning-linux-programming.md]
confidence: high
---

# 리눅스 쉘 스크립팅 (grep/sed/awk/bash)

리눅스 상에서 **명령어 체인을 스크립트로 구성하고 텍스트를 처리하는 기술** — 정규표현식·패턴 검색을 공용 언어로, grep/sed/awk을 전문 도구로, bash를 스크립트 언어로 삼는 축. 이 클러스터에는 두 권이 이 축을 다룸: 쉘 스크립팅 전담서 [[linux-shell-scripting-kim]]과, C 프로그래밍 입문서의 기초 구간인 [[beginning-linux-programming]] 2장(쉘 프로그래밍, p57). 기존 [[linux-essential-utilities]] 개념은 C 개발 도구 체인(gcc·make·gdb·vi)을 다룬다면, 이 페이지는 **쉘과 텍스트 처리 도구** 축을 다룬다.

## 서별 전개
| 권 | 구절 | 다루는 내용 | 관점 |
|----|------|-----------|------|
| [[linux-shell-scripting-kim]] | 1-8장 전체 | 1 쉘과 명령 기초 / 2 맛보기 / 3 정규표현식·패턴 / 4 grep / 5 sed / 6 awk / 7 bash / 8 vi·유틸리티 | 도구 하나를 1장씩 집중 — 정규식 개념(3장)이 grep/sed/awk 동작의 설명 축 `[raw/books/linux-shell-scripting-kim.md]` |
| [[beginning-linux-programming]] | 2장 쉘 프로그래밍 (p57) | 쉘 기초, C로 넘어가기 전의 명령·스크립트 문법 | C 입문자의 "쉘 리터러시" — 리눅스 환경에서 C를 돌리기 전의 필수 기초 `[raw/books/beginning-linux-programming.md]` |

## 공용 축: 정규표현식 → 도구 3부대
- **패턴이 공용 언어**: 3장이 정규표현식·패턴 검색을 독립 장으로 둘 뿐, grep·sed·awk이 모두 "패턴 매칭 후 동작" 구조. sed은 매칭 후 *대체*, awk는 매칭 후 *필드 처리/집계*로 분화 `[raw/books/linux-shell-scripting-kim.md]`
- **grep(탐색) → sed(변환) → awk(구조화·집계)** 의 무게가 오름. awk의 필드/레코드 모델이 sed의 라인 단위 조작 상위 개념
- **bash(7장)는 3부대를 호출·조립하는 언어**: `|` 파이프, `&&`/`||` 논리, 변수, 조건·반복, 함수 — 스크립트를 "명령어 나열"에서 "논리 프로그램"으로 승격 `[raw/books/linux-shell-scripting-kim.md]`
- C 프로그래밍 교재의 2장도 같은 기초(쉘과 명령)를 C 관점에서 다룸 — 쉘은 리눅스 C 개발자의 **실행 환경**이므로 `[raw/books/beginning-linux-programming.md]`

## 쉘 스크립팅 vs C 개발 도구 체인
| | 쉘 스크립팅 (본 축) | C 도구 체인 ([[linux-essential-utilities]]) |
|---|---------------------|----------------------------------------------|
| 중심 | grep·sed·awk·bash | gcc·make·gdb·svn·vi |
| 조작 대상 | 텍스트/프로세스 | 소스/빌드/디버그 |
| 학습 순서 | 리눅스 사용 기초(2장/1-2장) | C 컴파일 이후(1부 튜토리얼) |
| 공통점 | vi 편집기, "명령으로 실행한다"의 리눅스 철학 |

## 관련
- [[linux-shell-scripting-kim]] — 본 축의 전담서 (grep/sed/awk/bash 8장)
- [[linux-essential-utilities]] — C 유틸리티 실무서 (vi·gcc·make 접점)
- [[beginning-linux-programming]] — 2장 쉘 프로그래밍 (C 입문 전 기초)
- [[unix-advanced-programming]] — APUE ch3(쉘) 기준의 쉘·환경 심화
- [[gcc-compilation-pipeline]] — 쉘에서 실행하는 gcc·ld 파이프라인

## OCR 노트
- 두 source 권 모두 쉘 구간의 장 번호 OCR 혼용 (beginning TOC 장 번호 교정 참고) — 쉘 장은 p57
