---
title: 리눅스 커널 심층 분석 (Linux Kernel Development, 3rd Ed.)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [book, linux, kernel, os, programming, device-driver]
sources: [raw/books/linux-kernel-development-love.md]
confidence: high
---
# 리눅스 커널 심층 분석 (Linux Kernel Development, 3rd Ed.)

> 원서: 로버트 러브(Robert Love), *Linux Kernel Development, 3rd Ed.* (Addison-Wesley, 2010)
> 국내: 황정동 옮김, 에이콘(주) **2012**, ISBN 978-89-6077-331-8, 618p / 20장

## 개요
리눅스 커널(2.6.x 기준)의 주요 서브시스템을 개발자 관점에서 훑는 정석 입문서다. 특정 장치를 깊이 파는 드라이버 책이 아니라, 프로세스·스케줄링·시스템 호출·자료구조·동기화·타이머·메모리·VFS·블록 I/O·주소 공간·모듈·이식성·커뮤니티까지 커널의 "뼈대"를 한 권에 정리한다.[`raw/books/linux-kernel-development-love.md`] 추천의 글(앤드류 모튼)은 커널 소스를 배우고 참여하는 방법론 — 코드 읽기, 직접 수정, 메일링 리스트 참여 — 과 잘 작성된 문서의 가치를 강조한다. 국내 리눅스 커널 서적 중 가장 넓은 시야를 지닌 "상위 지도" 격서로, 이 클러스터의 다른 실전서([[linux-kernel-programming-itepert]], [[linux-kernel-device-driver-practice]])의 개념적 기반을 제공한다.

## 장 구조
| # | topic | 핵심 |
|---|-------|------|
| 2 | 커널과의 첫 만남 | 커널 구조 개요, 실행 환경 |
| 3 | 프로세스 관리 | task_struct, 프로세스 생성·종료 |
| 4 | 스케줄링 | 선점형 스케줄러, CFS 이전 다중 레벨 큐 |
| 5 | 시스템 호출 | syscall 테이블, 인자 전달 |
| 6 | 자료구조 | 커널 표준 자료구조 |
| 9-10 | 동기화 | 스피너락·세마포어·RCU, 동시성 문제 |
| 11 | 타이머 | 타임스탬프, timer_list, hrtimer |
| 12 | 메모리 관리 | slab, 가상 메모리, 페이지 캐시 |
| 13 | VFS | 가상 파일시스템 계층 |
| 14 | 블록 I/O | 블록 장치 계층, 디스크 캐싱 |
| 15 | 주소 공간 | 메모리 매핑, 페이지 테이블 |
| 17 | 장치·모듈 | 장치 드라이버 기초, 모듈 빌드(kbuild) |
| 19 | 이식성 | 아키텍처 독립/종속 코드 분리 |
| 20 | 패치·커뮤니티 | 패치 작성, 개발 프로세스 |

## 특징
- **서브시스템 전체 지도**: 커널이 "무엇을 하는지"를 장별 서브시스템으로 체계화 — 개념 학습용 1교재로 최적.
- **동기화 9-10장 집중**: SMP + 2.6 선점 커널 환경의 동시성 보호(스피너락 등)를 독립 서두로 다룸.
- **커널 개발 문화까지**: 19-20장으로 이식성과 패치/커뮤니티 참여까지 — "읽기→수정→공유"까지 이어지는 개발 사이클을 권함.
- **2.6 커널 기준**: 2.6 신규 기능(percpu, 모듈 kbuild, 선점 커널)을 버전 비교로 부연.

## 핵심 컨셉
- [[linux-kernel-structure]] — 프로세스·동기화·메모리·VFS·장치모델 5축 공통 프레임
- [[linux-kernel-programming-itepert]] — 같은 주제를 IT EXPERT 실습 코드로 풀어낸 국내 서
- [[linux-kernel-device-driver-practice]] — 17장(장치·모듈) 이후로 넘어가는 한국형 드라이버 실습서
- [[linux-device-driver-in-code]] — 17장에서 시작해 23장까지 장비를 넓힌 임베디드 드라이버 총서
