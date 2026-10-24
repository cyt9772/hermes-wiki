---
title: C 언어에 의한 화상처리 실무 (NHK, 국제테크노정보연구소 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-theory, image-processing, image-filtering]
sources: [raw/books/image-processing-practice-nhk.md]
confidence: medium
---
# C 언어에 의한 화상처리 실무 (NHK/국제테크노정보연구소 1999)

> 표지/원저: **NHK 방송기술연구소 화상연구부** (실무 엔지니어 8명과 함께 저술, 직원 교육용 교재) — 대표 저자 야마키·이노우에 (한자 표기 원문 OCR 가독 불가)
> 출판: 국제테크노정보연구소(편역), 발행인 최연희, 1999-11, 313p, 책값 45,000원

## 개요
일본 NHK 방송기술연구소 화상연구부의 8명이 공동 저술한 **C 언어 기반 실무 화상처리 교재**를 국제테크노정보연구소가 한국어로 옮긴 번역서 `[raw/books/image-processing-practice-nhk.md]`. 하드웨어적 요소를 의도적으로 배제하여 **표준 C 언어가 동작하는 컴퓨터(퍼스널컴퓨터~워크스테이션) 어디에서나 실행 가능한 소스 프로그램**을 중심으로 구성 `[raw/books/image-processing-practice-nhk.md]`. 장은 이론적 분류가 아니라 **"물체를 추출한다 / 윤곽을 추출한다 / 잡음을 제거한다 / 색을 변경한다 / 색으로 추출한다"** 같은 목적별로 독립되어 있어, 독자가 원하는 장만 선택하여 읽을 수 있다 `[raw/books/image-processing-practice-nhk.md]`.

## 장 구조 (TOC 기반, 313p, 12장 + 부록)
1. **화상처리의 세계로 초대한다** — 컴퓨터로 하는 화상처리, 주변 응용(사무실/의료/리모트 센싱/공장/방송·영화), 디지털 화상처리 특징, 칼럼(컴퓨터 그래픽스·뉴로 컴퓨터·디스크 입출력)
2. **화상처리를 체험한다** — 하드웨어 구성(프레임 메모리·화상 입력부·컴퓨터), 디지털 화상과 C 언어, 표본화·양자화, 화상처리 흐름, 메인 프로그램 image.c
3. **물체를 추출한다** — 임계값 추출(어떻게 정하는가), 2진 화상처리, 히스토그램 계산·표시·평활화
4. **윤곽을 추출한다** — 윤곽 성질, 1차미분(그라디언트)·2차미분(라플라시안), **Prewitt**, 템플릿 매칭, 세선화
5. **잡음을 제거한다** — 화상 잡음, 평활화(이동평균), **메디안 필터**, 2진화상 잡음 제거, 수축·팽창, 디저(dither)
6. **보기 쉬운 화상을 만든다** — 콘트라스트 강조(자동화), 농도 히스토그램 평탄화, 컬러 부가
7. **특징을 추출한다** — 2진화상 특징 파라미터, 라벨링, 연결성분의 원형도·면적으로 추출·잡음 제거
8. **색을 변경한다** — 색 정보, 컬러 바, **RGB↔Y(R-Y, B-Y) 변환**, 휘도·채도·색상 변환, 풀컬러 표시(HYPER-FRAME+, GG, shazzo [프레임 메모리])
9. **색으로 추출한다** — 2차원 히스토그램, RGB 임계값 처리, 화면 합성(경계부 색소거), 스크롤·줌 제어
10. **형상을 변경한다** — 기하학 변환(확대·축소, 이동, 회전, **투시 변환** — 선형 보간법), **동차 좌표**
11. **주파수로 처리한다** — 주파수 세계, **DFT**, 2차원 푸리에 변환, **2차원 FFT 구현**, 필터 처리(컨볼루션), 프린터 출력
12. **화상 데이터를 압축한다** — TV 전화, 가역·비가역 부호화, **run-length**, **DPCM**, **가변길이(하프만) 부호화**, DCT 압축, 스캐너 입력
13. **부록** — 전편 C 소스 프로그램 리스트

## 핵심 내용
- **목적별 독립장 구성**: 이론적 분류가 아닌 "윤곽 추출 / 잡음 제거 / 색 추출" 같은 작업 단위로 장을 나누어, 필요한 장만 선택하여 읽을 수 있는 실무서 구조 `[raw/books/image-processing-practice-nhk.md]`
- 제3~7장은 기초~중급 실무: **임계값(thresholding) → 미분/윤곽(Prewitt, Laplacian) → 평활화/메디안 → 콘트라스트/히스토그램 평탄화 → 특징 파라미터(라벨링, 연결성분)** `[raw/books/image-processing-practice-nhk.md]`
- 제8~9장은 컬러: **RGB↔YUV 변환**, 휘도·채도·색상 조작, 2차원 히스토그램과 RGB 임계값, 화면 합성(소프트웨어/하드웨어 키) `[raw/books/image-processing-practice-nhk.md]`
- 제11장: **DFT 이론 + 오일러 공식·진폭·위상 칼럼 + 2차원 FFT·2차원 컨볼루션 C 구현** — 영상 주파수 영역의 정석적인 실무 `[raw/books/image-processing-practice-nhk.md]`
- 제12장: **run-length / DPCM / 하프만** 3대 무손실 부호화를 C 소스로 구현, DCT 압축 칼럼 포함 — MPEG 계열 부호화의 선행 기법 `[raw/books/image-processing-practice-nhk.md]`
- OCR 품질: TOC/리스트명/한자 표기 가독성 낮음 — 원본 PDF 대조 권장, confidence: medium

## 관련
- 개념: [[image-processing-fundamentals]] — 이론(Gonzalez·Wintz) + Java 실무(Efford) + C 실무(NHK) 3책 비교
- 이론 기초: [[digital-image-processing-2ed]] · Java 실무: [[image-processing-java]]
- 인접 분야(기존): [[rf-engineering]] · [[microwave-engineering]] (NHK 방송기술 연구소 배경)
