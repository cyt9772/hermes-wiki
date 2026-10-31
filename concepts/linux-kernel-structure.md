---
title: 리눅스 커널 구조 (프로세스 · 동기화 · 메모리 · VFS · 장치 모델)
created: 2026-11-01
updated: 2026-11-01
type: concept
tags: [linux, kernel, os, device-driver, programming, concept, book]
sources: [raw/books/linux-kernel-development-love.md, raw/books/linux-kernel-programming-itepert.md, raw/books/linux-kernel-device-driver-practice.md, raw/books/linux-kernel-source-beginner.md, raw/books/linux-device-driver-in-code.md]
confidence: high
---
# 리눅스 커널 구조 (프로세스 · 동기화 · 메모리 · VFS · 장치 모델)

Cluster B 5권이 공통적으로 다루는 리눅스 커널의 5대 축 — **프로세스 관리 / 동기화 / 메모리 관리 / VFS·파일시스템 / 장치 모델·드라이버** — 을 한 표로 정리한다. 세 번역서(러브·벤카테스와란)는 "구조의 지도"를, 두 한국 서(한동훈·정재준 계)는 같은 축을 "코딩·실습"으로 풀어 `[raw/books/linux-kernel-development-love.md]` `[raw/books/linux-kernel-device-driver-practice.md]`. 다섯 책은 서로 다른 커널 버전(2.6 기준 ~ 4.0)과 다른 접근(개념 지도 ↔ 실전 코드)을 취하지만, 아래 5개 서브시스템이라는 동일한 뼈대를 전제로 한다.

## 5대 축
1. **프로세스 관리** — task/process 구조, 생성·종료, 문맥 교환, 스케줄링(run queue, 우선순위, 정책). 러브 3-4장, IT EXPERT 9장, 정재준 실습 2장.
2. **동기화** — SMP/선점 커널 환경의 동시성 보호: 스피너락·세마포어·RCU(러브 9-10장), 보호 영역·경쟁 조건·locking(실습 4장, 부록 내 동시성).
3. **메모리 관리** — 가상 메모리, 페이지, slab/slob/slub 할당, 메모리 매핑·주소 변환(러브 12·15장, IT EXPERT 8장, 실습 6장).
4. **VFS·파일시스템** — 가상 파일시스템 계층, 문자/블록 장치, ext/proc(러브 13-14장, IT EXPERT 6·10장).
5. **장치 모델·드라이버** — char/block, 인터럽트 핸들링, 모듈, PCI/USB/I2C/TTY 등 버스, Device Tree(러브 17장, 벤카테스와란 5-18장, 정재준 실습 11-18장, device-tree 2-12장).

## 서별 전개 (5축 × 5서)
| 축 | love (러브) | itepert (한동훈) | practice (정재준) | beginner (정재준) | in-code (벤카테스와란) |
|---|---|---|---|---|---|
| 성격 | 개념 지도(20장) | IT EXPERT 실전(11장) | 2부 18장 실습 | 최신 소스 단계 해설 | 23장 드라이버 총서 |
| 진입점 | 2장 커널 첫 만남 | 1장 환경 구축 | 1장 커널 자료구조 | 커널 소스 빌드 | 2장 커널 내부 |
| 프로세스 | 3-4장(관점·스케줄) | 9장 | 2장(스레드·문맥·스케줄) | 자료구조·sort | — |
| 동기화 | 9-10장 | (내부) | 4장(locking·사례) | kprobes·debug objects | — |
| 메모리 | 12장(+15장 주소) | 8장 | 6장(slab/slob/slub) | 유저 메모리·커널 메모리 주소 | — |
| VFS/FS | 13-14장 | 6·10장(proc/ext) | 11장(문자)·14장(블록) | kobject·kmodule | 14장(blk) |
| 장치/드라이버 | 17장(개념) | 5·7장(char/blk) | 11-18장(버스 실습) | (드라이버 전제) | 5-18장(전 버스) |

## 공통 논리
- **자료구조가 먼저**: 프로세스·드라이버를 모두 "커널 자료구조(list/queue/tree)" 위에 세운다 — 러브 6장 ↔ IT EXPERT 11장 ↔ 정재준 실습 1·7장 ↔ beginner의 list sort/red-black tree·XArray 실습.
- **프로세스=커널의 단일 화자**: 3권 모두 task_struct/process를 출발점으로 스케줄→동기화→메모리로 확장.
- **동기화는 SMP 이후의 필연**: 2.0 SMP + 2.6 선점 커널 이후 locking/스피너락이 독립 서브시스템으로 격상(러브 9-10, 실습 4).
- **VFS는 장치를 "파일"로 추상화**: char device ↔ block device ↔ VFS 계층이 4권에서 동일한 구조로 재현.
- **드라이버는 장치를 소스에 붙임**: 인터럽트 핸들러 + probe + TTY/TTY ops — 러브 17개념 → IT EXPERT char/blk → in-code 전버스 → 정재준 실습/DT 실습.

## 연결
- 관련 서: [[linux-kernel-development-love]] · [[linux-kernel-programming-itepert]] · [[linux-kernel-device-driver-practice]] · [[linux-kernel-source-beginner]] · [[linux-device-driver-in-code]] · [[device-tree-kernel-4-0]]
- 저자: [[jeong-jae-jun]] — 정재준 3권의 공통 저자
- 상위서: [[unix-advanced-programming]] — 커널 바깥의 시스템 프로세스 모델과 대비
- 버스 접점: [[usb-bus-architecture]] — in-code 11장 & practice 17장이 공유
