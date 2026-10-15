---
title: 리눅스 프로그래밍 필수 유틸리티
created: 2026-10-15
updated: 2026-10-15
type: entity
tags: [book, programming, os, linux, compiler, build-system, debugger, version-control]
sources: [raw/books/linux-essential-utilities.md]
confidence: high
---
# 리눅스 프로그래밍 필수 유틸리티

> 백창우 (bckddn@hanmail.net), 한빛미디어, 초판 2010-09-06 / 2012-11-12 재발행, ISBN 978-89-7914-759-9, 796쪽 `[raw/books/linux-essential-utilities.md]` 전표/초판기

리눅스 상에서 C 개발을 실제로 돌리는 **유틸리티 체계를 단계별로 훈련**하는 실무 교재. "왜 쓰는지"보다 **"무엇을 어떻게 치는지" — 명령어·옵션·프로젝트 구조**가 중심. 원고를 2007년부터 쓰고 햇수 3년 만에 출간(자서서) — 저자 경험이 그대로 책 체계를 이루는 스타일.

## 6부 구성 (TOC p.7-21)
| 부 | 테마 | 핵심 툴 |
|----|------|---------|
| 1 | 튜토리얼 | hello world → gcc, make, gdb(벌레 잡기), svn, doxygen, autotools, RPM (순차 입문) |
| 2 | 에디팅 | vi/vim: 모드, 트레이닝, 고급 테크닉(10%), ctags·cscope·플러그인; 그 외 emacs·이클립스·gedit·KDevelop·anjuta 소개 |
| 3 | 컴파일과 링킹 | C 컴파일 과정(전처리→C 컴파일→어셈블리→객체→링크), gcc 옵션 규칙·최적화, ld 링킹, GAS 어셈블리, binutils(읽기·서치·프로파일·명령어 디코딩) |
| 4 | 디버깅 | gdb 소개·브레이크포인트·프로파일링, trace 계열 도구, 문제 진단 유틸리티 |
| 5 | 프로젝트 빌드 | make 심화(복수 타깃, 인클루드, 조건부, 자동화), autotools: configure.ac·automake·Makefile.am·재귀 빌드 |
| 6 | 프로젝트 버전 관리 | 버전 관리 개념 → Subversion(클라이언트, 서버 설정, httpS 서버, import/commit/merge) → CVS(서버, 사용자 권한, 프로젝트 진행) |

## 특징
- **도구-중심 서술** — 각 툴마다 "개념 → 실제 명령 → 실습 결과" 순서. 1부의 make·svn은 5·6부에서 되돌아와 심화(입문↔심화 이중 경로)
- **C 컴파일 파이프라인**이 3부에서 전처리(-E) → 컴파일(-S) → 어셈블리(-c) → 링킹까지 gcc 단계 옵션으로 직접 보여줌 — 개념이 아니라 *실행*으로 배우는 구성
- 2010년 시점이라 버전 관리가 **Subversion/CVS** 위주. git은 없음 — "당시 리눅스 개발 표준"을 보는 자료적 가치가 있음
- rpm 패키징을 튜토리얼 8장에 배치 — 빌드 결과가 *배포물*로 이어지는 흐름

## 핵심 컨셉 연결
- [[gcc-compilation-pipeline]] — 3부(컴파일과 링킹)의 중심 축
- [[software-configuration-management]] — 1·6부: make·svn·autotools
- [[visual-basic]] — 대비 사례: VB는 인터프리터+IDE 일체, 여기는 분리된 도구 체인

## OCR 노트
- TOC에서 "AA"는 C(C언어), "makeS"=make, "svnS"=Subversion, "gecS"=gcc 등 OCR 혼동. 본문 인용 시 원문 확인 필요
- `14부`/`15부`/`16부` 라벨은 OCR이 "4부/5부/6부"를 잘못 인정한 것. 실제 부 수는 1~6
