---
title: BBB(BeagleBone Black)를 사용한 Yocto 프로젝트
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, embedded-linux, yocto, bitbake, beaglebone, arm, linux-kernel]
sources: [raw/books/bbb-yocto-project.md]
confidence: high
---
# BBB(BeagleBone Black)를 사용한 Yocto 프로젝트

> 저자: 이르판 사디크(Irfan Sadiq) | 역자: 배창혁
> 원서: Using Yocto Project with BeagleBone Black (Packt, 2015) | 에이콘, 2016
> 171p `raw/books/bbb-yocto-project.md`

## 개요
BeagleBone Black(BBB) 보드를 목표로 **Yocto 프로젝트 레시피로 임베디드 리눅스 스택을 빌드하고 커스텀 이미지로 실습**하는 실무서. BitBake·레이어·레시피 개념을 helloworld에서 감시 시스템·무선 AP까지 8장 내외로 집중. [[embedded-linux-yocto-project]](567p 종합서)에 비해 분량은 작지만, "보드 하나에 올린다"는 실습 곡선에 집중 `raw/books/bbb-yocto-project.md`.

## 장 구조 (8장)
| 장 | 제목 |
|----|------|
| 1 | 욕토 프로젝트와 비글본 블랙 시작 |
| 2 | BitBake의 모든 것 |
| 3 | helloworld 예제 생성 |
| 4 | 비글본 보드에 멀티미디어 추가 (GStreamer) |
| 5 | 레이어 생성과 분석 |
| 6 | 콘솔 게임 (팩맨) |
| 7 | 집안 감시 시스템을 위한 비글본 튜닝 (V4L2) |
| 8 | 무선 액세스 포인트로 비글본 사용 |

`raw/books/bbb-yocto-project.md`

## 특징
- BitBake 엔진(제2장)을 별도 장으로 다룸 — 레시피 문법·poky 소스 구조에 집중
- 레이어 생성(제5장)과 bbappend/패키지 추가(제6장)를 실무 예제로 처리
- GStreamer·V4L2 같은 멀티미디어/영상 스택을 레시피로 올리는 실습(제4, 7장)

## 핵심 컨셉 연결
- [[embedded-linux-build]] — 레시피/BitBake은 그 개념의 자동화 레이어
- [[embedded-linux-stack]] — 4단계 파이프라인(toolchain→bootrom→kernel→rootfs)의 Yocto 실습
- [[embedded-linux-yocto-project]] — Yocto 종합 교재와의 대비 (이 책은 BBB 특화)
- [[embedded-firmware-basics]] — 비트베이크가 자동화하는 하위 단계(부트로더/커널)

## Related
- 저자: 이르판 사디크 (Irfan Sadiq)
- 개념: [[embedded-linux-build]], [[embedded-linux-stack]], [[embedded-firmware-basics]]
- 보드: [[raspberry-pi-iot]] (BBB·RPI 비교)
