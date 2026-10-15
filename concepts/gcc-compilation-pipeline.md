---
title: C 컴파일 파이프라인 (gcc)
created: 2026-10-15
updated: 2026-10-15
type: concept
tags: [programming, compiler, build-system, os, linux]
sources: [raw/books/linux-essential-utilities.md]
confidence: high
---
# C 컴파일 파이프라인 (gcc)

C 소스가 실행 파일이 될 때까지의 4단계 변환 — **전처리 → 컴파일 → 어셈블리 → 링킹**. 각 단계는 gcc 옵션으로 분리 실행할 수 있고, 빌드 디버깅의 기본 언어.

## 4단계 파이프라인
| 단계 | 업무 | gcc 옵션 | 산출물 |
|------|------|---------|--------|
| 전처리 (Preprocessing) | 매크로 치환, `#include` 인라인, 조건부 컴파일 제거 | `-E` | 전처리된 C(.i) |
| 컴파일 (Compilation) | C → 어셈블리 코드 | `-S` | 어셈블리(.s) |
| 어셈블리 (Assembly) | 어셈블리 → 기계어 | `-c` | 객체 파일(.o) |
| 링킹 (Linking) | 객체 파일 + 라이브러리 → 실행 파일 | (기본) | 실행 파일 |

`gcc file.c -o prog` 은 4단계를 한 번에 수행하는 설타.

## 각 단계의 중요 포인트
- **전처리**는 "컴파일"이 아니라 **텍스트 치환** — 매크로 정의(`#define`), 헤더 삽입. 전처리 오류는 컴파일 오류와 위치·성질이 다름 `[raw/books/linux-essential-utilities.md]` 3부 ch1-2
- **컴파일**은 1개 파일 단위 — 각 .c가 독립적으로 .s/.o로. 이것이 다중 파일 병렬 빌드(make)의 기반
- **어셈블리** 단계에서 GAS 문법이 드러남 — 어셈블리 파일을 직접 쓰거나(C inline asm) 디스어셈블해 볼 수 있음 `[raw/books/linux-essential-utilities.md]` 3부 GAS 실습
- **링킹**은 심볼 해석 — 정의/참조 심볼 매칭, 라이브러리(`-l`) 순서 문제 발생 지점

## gcc 최적화
- `-O0`〜`-O3` 최적화 레벨 — 실행 시간 vs 코드 크기 트레이드오프
- 최적화는 컴파일 단계에서 수행. 링킹 단계에는 영향 없음
- 디버깅 시 `-O0` + `-g` 권장. 최적화된 코드에서 변수·주소가 사라짐

## 인라인 어셈블리
- C 코드 안에 GAS 문법 직접 삽입 — 하드웨어 명령어 직접 접근
- 리스제스트레지스터, clobber 리스트로 컴파일러에 자원 사용 선언 `[raw/books/linux-essential-utilities.md]` 3부 ch3

## 관련 콘셉트
- [[software-configuration-management]] — 파이프라인을 다중 파일·조건부로 확장(make, autotools)
- [[visual-basic]] — 대비: VB는 컴파일 없이 인터프리터+IDE 일체
