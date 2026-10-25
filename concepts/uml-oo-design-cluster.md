---
title: UML·객체지향 설계 클러스터 (2026-10-25 5권)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [uml-oo-modeling, object-oriented, book, comparison]
sources: [raw/books/applying-uml-patterns.md, raw/books/teach-yourself-uml.md, raw/books/uml-user-guide.md, raw/books/uml-rational-rose.md, raw/books/software-design-techniques.md]
confidence: high
---

# UML·객체지향 설계 클러스터 (2026-10-25 5권)

이 클러스터는 UML(Unified Modeling Language)과 객체지향(OO) 설계를 다룬 2026-10-25 USB 5권(`Applying UML and Patterns`, `Teach Yourself UML in 24 Hours`, `UML 사용자 지침서`, `software design techniques`, `Mastering UML with Rational Rose 2002`)을 묶는 교차 비교 페이지다.

## 서별 전개 table

| 책 | UML 버전/시점 | 도구 | 저자 | 특징 |
|---|---|---|---|---|
| `Applying UML and Patterns` (Larman, 2001, 2nd ed) | UML 1.x (UP 1.x 시점) | Rational Rose / UML CASE (상당 부분 whiteboard) | Craig Larman | UML 표기 + 디자인 패턴 + GRASP + UP 반복개발 실무. NextGen POS 케이스. |
| `Sams Teach Yourself UML in 24 Hours` (Schmuller, 2001, 2nd ed) | UML 1.x | 도구 비의존적 (표기법 중심) | Joseph Schmuller | UML 표기(7종 다이어그램)를 시간 단위로 자기주도 학습. 22시간 디자인 패턴, 23-24시간 엔베드/표준화. |
| `UML 사용자 지침서` (Booch·Rumbaugh·Jacobson, 1999, 인터비전) | UML 1.x 표준 문서 (Addison-Wesley 원저) | 없음 (Rational UP 부록 포함) | UML 3인 공동 | UML 표준 자체의 "사용자 지침서". 32장/7단원. 단원 1~3 구조, 단원 4~5 행동, 단원 6 아키텍처, 단원 7 패턴/UP 부록. |
| `software design techniques` (Watanabe Kouzo 외 9인, 2002 Nikkei, 2004 성안당) | UML 1.x (현장 실무 적용) | IBM Rational Rose XDE (부록) | Watanabe Kouzo 외 9인 | 구조화 분석(DFD)·ER 모델링 → UML 8종 → GoF 디자인 패턴(7형제) → 객체지향 3대 기능 → "객체지향 설계 원칙 5가지". |
| `Mastering UML with Rational Rose 2002` (Boggs 부부, 2002 SYBEX, 2003 에이콘) | UML 1.x (Rose 2002 시점) | **Rational Rose 2002** (C++/VB/Java/J2EE/EJB/XML/CORBA/Data Modeler) | Wendy Boggs, Michael Boggs | UML 1.x 표준이 아니라, Rose 2002라는 하나의 CASE/IDE 위에서 "모델→코드→모델" round-trip 엔지니어링 실무. |

## 공통 축 (5권 공통)
1. **클래스 다이어그램 + 시퀀스 다이어그램**: UML "표기법"의 두 축. 5권 모두 클래스(구조)와 시퀀스/콜라보레이션/활동(행동) 다이어그램을 다룸. `UML 사용자 지침서` 단원 1~3에서 "왜 모델을 만드는가"를 기초로 클래스·관계·클래스 다이어그램을 다룬 뒤, 단원 4~5에서 교류(15-19장), `Applying UML and Patterns` 15장(Interaction Diagram Notation), `software design techniques` "정적/동적 분석(Part 6-7)"이 이 공통 축에 해당.
2. **GoF 디자인 패턴**: [object-oriented-design-patterns] 페이지 참조. `Applying UML and Patterns` 23장(GoF Design Patterns), `software design techniques` 장 4(GoF 7형제), `UML 사용자 지침서` 28장(패턴과 프레임웍), `Teach Yourself UML` 22시간(Design Patterns)이 이 축에 해당.
3. **설계 원리 (Responsibility/Pattern/Principle)**: `Applying UML and Patterns`의 **GRASP**(Responsibility Assignment)와 `software design techniques`의 **Watanabe 설계 원칙 5가지**가 이 축의 두 끝점. GRASP는 "UML+UP" 프레임워크 안에서 책임을 클래스에 배정하는 원칙이고, Watanabe 5원칙은 "현장 실무"에서 유지보수·재이용성을 높이는 실천 원칙이다.
4. **UML 3인 vs 실무 도구서**: UML 표준(3인)을 직접 다룬 `UML 사용자 지침서`는 "표준 문서는 어떻게 쓰이는가"에 집중하고, `Mastering UML with Rational Rose 2002`는 "표준을 하나의 CASE 도구(Rose 2002) 위에서 어떻게 실무로 전환하는가"에 집중한다. Larman과 Schmuller는 전자의 "표준 설명서"와 후자의 "도구 실무서" 사이의 **입문 실무서**에 해당한다. Watanabe는 "표기법"보다 "현장 실무"를 전면에 배치한 5권 중 유일하게 구조화 분석/ER 모델링을 함께 다루는 책이다.

## 비교 결론
- **UML 표준 자체**를 이해하려면 `UML 사용자 지침서`(3인 공동, UML 1.x 표준 문서)가 1차 소스.
- **UML 표기를 빠르게 훑으려는** 입문자에게 `Teach Yourself UML in 24 Hours`.
- **UML + 디자인 패턴 + 반복개발(UP) 실무**를 원하면 `Applying UML and Patterns`.
- **현장 실무(구조화 분석→UML→GoF→설계 원칙)**를 원하면 `software design techniques`.
- **특정 CASE 도구(Rose 2002) 상의 모델→코드 round-trip**를 원하면 `Mastering UML with Rational Rose 2002`.

## Related
- 책: [[applying-uml-patterns]] / [[teach-yourself-uml]] / [[uml-user-guide]] / [[software-design-techniques]]
- 저자: [[craig-larman]] / [[joseph-schmuller]] / [[grady-booch]] / [[james-rumbaugh]] / [[ivar-jacobson]] / [[watanabe-kouzo]]
- 컨셉: [[object-oriented-design-patterns]]
- 기존 관련: [[software-configuration-management]] (개발 프로세스와 접점; Rose/UP은 형상관리·요구관리 도구와의 통합을 전제로 하는 프로세스)
