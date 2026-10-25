---
title: Watanabe Kouzo (와타나베 코우조)
created: 2026-10-25
updated: 2026-10-25
type: author
tags: [author, uml-oo-modeling, object-oriented]
sources: [raw/books/software-design-techniques.md]
confidence: high
---

# Watanabe Kouzo

Watanabe Kouzo(와타나베 코우조, 로마자 표기만 사용)는 `Zero Kara Manabu · Software Sekkei / software design techniques`(Nikkei Business Publications, 2002)의 대표 저자로서, 9인의 공동 저자(야자와 히사오, 후지모토 히지리, 히라사와 아키라, 바바 다이스케, 카즈요시 시, 유우지 미우라, 켄지 히라나베 등)와 함께 객체지향 소프트웨어 설계를 **현장 실무** 중심으로 다루는 저자다. 이 책의 "소프트웨어 설계 테크닉(소프트웨어 설계 기법)"이라는 타이틀이 반영하듯, Watanabe는 UML 다이어그램이나 GoF 디자인 패턴(GoF 7형제)을 "이론"이 아니라 "구조화 분석(DFD)·ER 모델링부터 시작해 UML로 이어가는 실무 도구"로 정리한다.

이 클러스터에서 Watanabe의 핵심 기여는 **객체지향 설계 원칙 5가지**다: (1) 역할분담은 확실히 한다(책임=1개), (2) 이름은 본질을 나타내도록, (3) 작은 것이 좋은 것이다(함수 20-30행 상한), (4) 숨기는 것이 많을수록 좋다(정보 은폐, `private/protected`), (5) 타인과 관계되는 일이 줄인다(인수·반환값 최소, 의존도 최소) (p. 361-366, 유지보수·재이용성 높은 객체지향 설계 요령). 이 5가지 요령은 Booch·Rumbaugh·Jacobson의 UML 표준이 다루는 "표기법"이 아니라, 설계 *원리*의 실천적 정리라는 점에서 이 클러스터의 다른 저자와 대비된다.

Watanabe는 UML 1.x의 3저자(Booch·Rumbaugh·Jacobson)와는 별개 인물이다. `software design techniques`는 UML 표준 문서가 아니라, 실무 개발자가 쓴 **현장 실무서**다. Watanabe는 일본 엔지니어로, UML 표준 3인(Booch·Rumbaugh·Jacobson)이 만든 표준 표기법 자체를 다룬 것이 아니라, 그 표준 표기법(UML)과 GoF 디자인 패턴(7형제: Factory Method, Abstract Factory, Singleton, Composite, Adapter, Observer, Command)를 "현장에서 쓰이는 실무 도구"로 재결합한 저자다.

## Related
- [[uml-oo-design-cluster]] — 이 클러스터의 UML·OO 설계 5권 비교
- [[object-oriented-design-patterns]] — GoF 패턴·설계 원리 축
- [[software-design-techniques]] — Watanabe의 실무 설계서
