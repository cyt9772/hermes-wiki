---
title: NEW 비주얼베이직 6 입문
created: 2026-10-15
updated: 2026-10-15
type: entity
tags: [book, programming, windows-api, object-oriented]
sources: [raw/books/vb6-introduction.md]
confidence: high
---
# NEW 비주얼베이직 6 입문 (Visual Basic 6 Intro)

Windows GUI 프로그래밍의 입문 교재. 일본에서 쓰인 Visual Basic 6 교범(하야시 하루히코, SoftBank Publishing 1998)의 한국어 번역본. 영진닷컴이 1999년 초판(2002년 재발행)으로 냈다. 357쪽 분량에 이벤트 기반 개체 지향 프로그래밍의 개념, IDE의 조작, 제어문, 프로시저, 컨트롤, 그래픽 처리, 파일 입출력을 순서대로 다룬다.

> 비주얼베이직은 "클래스(컨트롤/폼)의 인스턴스를 만들고, 그 인스턴스에 이벤트를 연결하여 동작을 정의하는" 패러다임을 취한다. `Me`가 지금 다루는 폼 자신을 가리키고, 각 컨트롤(Command1, Text1, List1, Timer1…)은 독립된 개체로 이름으로 접근한다. `[raw/books/vb6-introduction.md]` p.1, p.30
> "윈도우 시대가 되자 컴퓨터의 기능이 비약적으로 발전했다… 그 복잡성을 실현하는 고도의 기능을 가진 윈도우용 프로그래밍 언어가 필요했다" `[raw/books/vb6-introduction.md]` p.3

## Book metadata
- **저자:** 하야시 하루히코 (HARUHIKO HAYASHI)
- **출판사:** 영진닷컴 (Youngjin.com) — 일본 SoftBank Publishing의 판권 계약 번역
- **초판/재발행:** 1999 / 2002
- **ISBN:** 89-314-1287-8
- **쪽수:** 357 (스캔본 OCR)
- **원서:** NEW Visual Basic 6 Nyumon (SoftBank, JP, 1998)

## 구성 (chapter map)
| # | 주제 | 핵심 내용 |
|---|------|-----------|
| 1 | VB의 기본 지식 | 클래스 vs 인스턴스, 이벤트 기반 구조, IDE 개요 |
| 2 | 프로그램 만들기 | 폼/컨트롤 추가, 프로젝트 구조, 속성 편집기 |
| 3 | 기본 조작 | 실행·중단점·디버거, 프로젝트/모듈 관리, 코드 에디터 |
| 4 | 변수 | 기본 데이터형(문자열/통화/Byte/Boolean), Variant, 동적 배열, 사용자 정의형(Type) |
| 5 | 연산자 | 산술/관계/논리/문자열/비트 연산자 |
| 6 | 제어문 | If, Select Case, For, While…Wend, Do…Loop, GOTO, Stop, Exit |
| 7 | 프로시저 작성 | Sub 프로시저 / 함수 프로시저, ByVal/ByRef, 모듈·공용 |
| 8 | 컨트롤 사용 | List, Text, Frame, CheckBox, OptionButton, Timer 등 |
| 9 | (API 등) | Windows API 호출 및 고급 동작 |
| 10 | 그래픽 처리 | 직선/도형/화면 출력, 그래픽 객체 |
| 11 | 재미있는 프로그램 | 응용 예제 |
| 12 | 파일 처리 함수 | 순차 액세스(Open/Print/Line Input), 랜덤 액세스(레코드/Type), 파일 조작 |

## 핵심 개념 연결
- [[visual-basic]] — 본 책이 다루는 언어 본체(개체지향, 이벤트, IDE, 데이터형, 파일 액세스)
- 이벤트 기반 프로그래밍: 클래스(컨트롤) vs 인스턴스, 이벤트 연결 패턴
- 파일 입출력: 순차(sequential) 액세스 / 랜덤(random) 액세스 — `Open`/`Print #`/`Line Input`/`EOF`
- `Type ... End Type` 사용자 정의형(struct)을 사용한 랜덤 액세스 레코드 구조

## OCR 품질 유의
- tesseract 5.5.3 (kor+eng, 300dpi). 영어 토큰 일부 깨짐(IoT→"107" 형태의 글리프 오류).
- "Visual Basic"이 "Visual ㅁ2510" 등으로 오독되어 있다 — 본문 의미는 시각적으로 교차확인.
