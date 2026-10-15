---
title: 소프트웨어 구성 관리 (SWM / 빌드·버전 관리)
created: 2026-10-15
updated: 2026-10-15
type: concept
tags: [programming, build-system, version-control, os, linux]
sources: [raw/books/linux-essential-utilities.md]
confidence: high
---
# 소프트웨어 구성 관리 (빌드·버전 관리)

다중 파일 C 프로젝트에서 **"누가·언제·어떻게 빌드했는지"**를 추적·재생성 가능하게 하는 체계. 리눅스 세계의 표준 3점 세트: **make(빌드) + autotools(이식성) + VCS(저장소)**.

## 빌드 자동화: make
- **Makefile** 규칙: `대상: 의존성` + 명령. 의존성 그래프에서 바뀐 파일만 재빌드(증분 빌드)
- 복수 타깃, 재귀적 make, 인클루드된 Makefile 분할로 대형 프로젝트 지원 `[raw/books/linux-essential-utilities.md]` 5부
- 핵심 변수: `MAKE`, `@`/`-` 접두, 자동 변수 `$@ $< $^` — "만들어야 할 것/요건/명령"의 분리

## 이식성 빌드: autotools
- **autoconf**: `configure.ac` → configure 스크립트, 시스템 함수/헤더 체크(Autoconf 함수 체크 매크로) `[raw/books/linux-essential-utilities.md]` 5부 ch4
- **automake**: `Makefile.am` → Makefile.in, 표준 make 규칙 자동 생성
- **세밀한 configure.ac 제어**·설정 헤더(config.h)로 소스에 조건부 설정 반영 — 한 코드베이스가 여러 플랫폼에서 빌드되게 하는 장치

## 버전 관리: 저장소
| 체계 | 모델 | 비고 |
|------|------|------|
| **Subversion (svn)** | 집중형(중앙 서버) | 2010년 표준. import·commit·merge, httpS 서버 설정, 권한 관리 |
| **CVS** | 집중형, 파일-레벨 경합 | svn의 전신 성격. 사용자 생성·권한 설정 |
| (후대) Git | 분산형 | 이 책 시점엔 미성숙. 현대 표준 — 위키 다른 페이지 참고 |

- **경합 모델**: CVS는 파일 단위 동시 편집을 lock(잠금) 방식으로 제어 — 집중형 VCS의 전형적 한계 `[raw/books/linux-essential-utilities.md]` 6부
- **메타데이터**: 커밋 로그(누가·언제·무엇을)는 팀 내 책임 추론의 근거

## 관련 콘셉트
- [[gcc-compilation-pipeline]] — 빌드(구성 관리)가 자동화하는 대상
- [[visual-basic]] — 대비: VB6는 프로젝트 파일(.vbp) 단일 저장소 방식
