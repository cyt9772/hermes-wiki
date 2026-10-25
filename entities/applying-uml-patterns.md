---
title: Applying UML and Patterns (2nd ed)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, uml-oo-modeling, object-oriented, software-quality]
sources: [raw/books/applying-uml-patterns.md]
confidence: high
---

# Applying UML and Patterns / UML과 디자인 패턴 (2판)

Craig Larman(크레이그 라먼)의 `Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and the Unified Process`(2판, Prentice Hall PTR, 2001; ISBN 0-13-092569-1)은 UML 표기와 디자인 패턴을 *반복 개발(Unified Process)* 프레임워크 안에서 하나의 실습 사례(NextGen POS 시스템)를 따라가며 가르치는 객체지향 분석·디자인 입문서다. 이 책의 가치는 표기법을 외우는 데서가 아니라, 책임을 클래스에 배정하는 **GRASP**와 요구사항→디자인→구현의 흐름을 하나의 반복(iteration) 단위로 체득시킨다는 점에 있다.

## 저자·서지
- 저자: Craig Larman (Valtech Process Director). 원저는 Prentice Hall.
- 한국어판이 아니라 원서(영어)를 대상으로 한 페이지.

## 장별 개요 (원문 TOC 기준, 38장 / 6부)
원문 목차 기준 총 **38장**을 6개 파트로 나누었다:
- Part I Introduction: 1 OO Analysis and Design, 2 Iterative Development and Unified Process, 3 Case Study: The NextGen POS System.
- Part II Inception: 4 Inception, 5 Understanding Requirements, 6 Use-Case Model(요구사항 작성), 7 Identifying Other Requirements, 8 From Inception to Elaboration.
- Part III Elaboration (Iteration 1): 9 Use-Case Model(System Sequence Diagrams), 10~12 Domain Model(개념·연결·속성), 13 Operation Contracts, 14 From Requirements to Design, 15 Interaction Diagram Notation, 16 GRASP, 17 Use-Case Realizations with GRASP, 18 Determining Visibility, 19 Creating Design Class Diagrams, 20 Mapping Designs to Code.
- Part IV Elaboration (Iteration 2): 21 Iteration 2 Requirements, 22 More GRASP Patterns, 23 GoF Design Patterns.
- Part V Elaboration (Iteration 3): 24~34(UML 고전 모델링, Generalization, Statechart, Architectural/Analysis with UML, Persistence Framework).
- Part VI Special Topics: 35~38(도구·표기법, Agile UP, 프로젝트 이슈, 반복개발과 UP).

## 핵심 컨셉
- **GRASP (General Responsibility Assignment Software Patterns)**: `Information Expert`, `Creator`, `High Cohesion`, `Low Coupling`, `Controller` 5가지 기본 패턴으로 시작해, 2장에서 `Protected Variations`, `Polymorphism` 등을 추가한다. 2판에서 새로이 도입된 `Protected Variations`로 변하는 요소를 격리한다 (p. 215-222).
- **반복 개발 (Iterative/UP)**: `Inception → Elaboration (Iteration 1/2/3) → …`의 구조를 하나의 NextGen POS 케이스로 학습하게 하는 것이 이 책의 핵심 구조다. 2장(Iterative Development)에서 UP 단계와 Agile UP을 다룬다.
- **Use-Case 중심의 요구사항**: `Use-Case Model`은 요구사항을 `Actor/Use-Case`의 컨텍스트로 작성하고, `System Sequence Diagrams`(9장)와 `Operation Contracts`(13장)를 통해 디자인으로 이어간다.
- **GoF 디자인 패턴의 적용 (23장)**: `Design Use-Case Realizations with GoF Design Patterns`로, `Applying UML and Patterns`의 타이틀이 함축하는 UML 표기와 디자인 패턴의 통합을 실현한다.

## Related
- 저자: [[craig-larman]]
- 클러스터: [[uml-oo-design-cluster]] / [[object-oriented-design-patterns]]
- 기존 관련: [[software-configuration-management]] (개발 프로세스와 접점)
