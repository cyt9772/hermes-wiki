---
title: 정재준 (리눅스 커널 저자)
created: 2026-11-01
updated: 2026-11-01
type: entity
tags: [author, linux, kernel, os, programming]
sources: [raw/books/device-tree-kernel-4-0.md, raw/books/linux-kernel-device-driver-practice.md, raw/books/linux-kernel-source-beginner.md]
confidence: high
---
# 정재준 (리눅스 커널 저자)

한국 리눅스 커널 저자·교육자. **커널연구회**(www.kernel.bz)를 운영하며, 리눅스 커널·자료구조/알고리즘 연구와 시스템 프로그래밍·디바이스 드라이버 개발로 임베디드 제품을 만들고 관련 교육을 제공한다. 본 배치(Cluster B)에서 아래 3권의 저자다.

## 저서 (본 배치)
- [[linux-kernel-device-driver-practice]] — *리눅스 커널과 디바이스 드라이버 실습 2판* (커널연구회, 2012/2013, ISBN 978-89-97750-05-4, 603p) — 커널 내부 이해(1부) + 드라이버 실습(2부) 18장.
- [[linux-kernel-source-beginner]] — *리눅스 커널 소스 해설 [기초입문]* (커널연구회, 2020, ISBN 978-89-97750-13-9, 353p) — 최신 커널 소스 단계 해설·디버그 도구(perf/ftrace/crash/kprobes).
- [[device-tree-kernel-4-0]] — *디바이스 트리 상세 분석 in Linux Kernel 4.0* (커널연구회, 2015, ISBN 978-89-97750-06-1, 314p) — DT 소스 분석 + UART(8250) 드라이버 상세분석.

## 특징
- **커널연구회 3종 세트**: 소스 입문([[linux-kernel-source-beginner]]) → 드라이버 실습([[linux-kernel-device-driver-practice]]) → Device Tree 심화([[device-tree-kernel-4-0]])로 이어지는 한국형 커널 학습 로드맵.
- **임베디드 실전 관점**: 커널을 "읽기"가 아니라 SoC 보드(UART·GPIO·USB 실습) 위에서 "돌려보고 고치기"로 다룸.
- **번역서와의 대비**: 정재준의 원서는 같은 커널/드라이버 주제를 한국 개발자 입장의 코드·실습 중심으로 풀어 [[linux-kernel-development-love]](러브), [[linux-device-driver-in-code]](벤카테스와란)와 보완 관계.
- **공동체 운영**: 커널연구회(www.kernel.bz)의 연구·개발·교육 산출물을 온라인에서 무료/유료로 제공 — 개인 블로그가 아닌 조직 운영형 저술.

## 관련
- 저술 범위: 리눅스 커널 내부, 디바이스 드라이버, Device Tree(ARM), 커널 디버깅 도구(perf·ftrace·crash·kprobes).
- 이 클러스터의 개념 공통 페이지: [[linux-kernel-structure]] — 5권이 공유하는 프로세스·동기화·메모리·VFS·장치모델 5축.
- 같은 주제의 개념서·번역서: [[linux-kernel-programming-itepert]](한동훈) — IT EXPERT 시리즈 실전 코딩 관점.
- 정재준 원서 3권 모두 커널연구회(www.kernel.bz)에서 무료/유료 문서로 병행 제공.
- 번역서와의 접점: [[linux-kernel-development-love]](러브)의 17장(장치·모듈) 개념을 드라이버 실습으로 확장.
