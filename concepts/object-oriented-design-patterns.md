---
title: 객체지향 설계 패턴 (Design Patterns)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [uml-oo-modeling, object-oriented, software-quality, concept]
sources: [raw/books/applying-uml-patterns.md, raw/books/software-design-techniques.md]
confidence: high
---

# 객체지향 설계 패턴 (Design Patterns)

"디자인 패턴(Design Patterns)"은 객체지향 설계에서 반복되는 **문제→해결책** 쌍(problem/solution pair)을 카탈로그 형식에 이름을 붙여 정리한 노하우의 집합이다. 이 클러스터에서는 **GoF (Gamma·Helm·Ralph Johnson·Vlissides, 1994, `Design Patterns / Gang of Four`)** 와 **Watanabe Kouzo의 설계 원칙 5가지**(현장 실무)가 두 축을 이룬다.

## GoF 디자인 패턴

GoF 4인은 1994년 "객체지향 설계에서 자주 나타나는 23 종류의 노하우"를 이름과 카탈로그로 정리했다 (Watanabe `software design techniques`, "객체지향 설계의 비전서: 디자인 패턴" 섹션). 이 23종 패턴은 다음 4개 그룹으로 나뉜다(일반 분류, GoF 기준):
1. **생성 패턴 (Creational)**: `Factory Method`, `Abstract Factory`, `Singleton`, `Builder`, `Prototype`.
2. **구조 패턴 (Structural)**: `Adapter`, `Bridge`, `Composite`, `Decorator`, `Facade`, `Flyweight`, `Proxy`.
3. **행동 패턴 (Behavioral)**: `Chain of Responsibility`, `Command`, `Iterator`, `Mediator`, `Memento`, `Observer`, `State`, `Strategy`, `Template Method`, `Visitor`.

이 클러스터의 `software design techniques` 장 4는 "꼭 알아 둘 디자인 패턴 칠형제"로 `Factory Method / Abstract Factory / Singleton / Composite / Adapter / Observer / Command` 7개를 골라 UML 클래스 다이어그램과 함께 설명(p. 168-214), Part 3에서는 `Singleton/Template Method(Adapter/Observer/Command)`의 실전 활용(214-235, 교육용 웹 사이트, 실험 시료 관리 SW, 대화형 웹 애플리케이션)을 다룬다.

이 클러스터의 `Applying UML and Patterns` 23장 "Design Use-Case Realizations with GoF Design Patterns"는, UML 시퀀스/콜라보레이션 다이어그램 위에 GoF 패턴을 **사용 사례(use-case realization)** 단위로 배치하는 UML+GoF의 통합을 보여준다.

## Watanabe의 객체지향 설계 원칙 5가지

`software design techniques` "유지보수와 재이용성 높은 객체지향 설계 요령" 섹션(p. 361-366)에서 Watanabe가 정리한 5가지:
1. **역할분담은 확실히 한다**: `책임 = 1개, 그 이상이면 분할`. 같은 코드를 복사·붙여넣기 하는 "Copy & paste 프로그래밍"은 스파게티 코드로 직결.
2. **이름은 본질을 나타내도록**: 클래스·메소드의 이름을 읽는 사람이 의미를 바로 이해할 수 있도록 (유지보수성 향상).
3. **작은 것이 좋은 것이다**: 한 메소드는 20-30행(한 화면) 상한.
4. **숨기는 것이 많을수록 좋다**: 정보 은폐(`private/protected`), 속성·메소드는 바깥에서 직접 액세스 못 하게.
5. **타인과 관계되는 일이 줄인다**: 인수·반환값을 최소화하고, 필요 없는 인스턴스를 갖고 있지 않도록.

이 5원칙은 GoF 23종 패턴보다 **더 아래층(설계 원리)** 에 있는 원칙으로, "패턴을 쓰겠다"는 판단 이전에 "왜 이 클래스를 이 책임으로 설계하는가"를 결정하는 기준이다.

## GoF 패턴 vs Watanabe 5원칙: 교차

| 구분 | GoF 23종 패턴 | Watanabe 5원칙 |
|---|---|---|
| 층위 | 설계 기법/패턴 (중간) | 설계 원리 (하위, 원칙) |
| 형태 | 문제-해결책 쌍, 카탈로그 | 실천 규칙, 5개 |
| 목표 | 재사용성, 확장성, 유지보수성 | 유지보수·재이용성, 품질 |
| UML 표현 | 클래스 다이어그램, 시퀀스 다이어그램(23장, 17장) | 클래스 다이어그램(역할분담), `private/protected`(정보 은폐) |
| 관계 | "어떻게" (How) | "무엇/왜" (What/Why) |

즉, Watanabe 5원칙이 "설계의 판단 기준"이고, GoF 패턴이 "그 기준 위에서 재사용 가능한 표준 해답"이다. `Applying UML and Patterns`의 **GRASP**(16-22장)는 이 두 가지(원칙·패턴)를 "책임 배정(Responsibility)"이라는 단일 축으로 연결하는 **중간층**이다(p. 215-222): `Information Expert`, `Creator`, `High Cohesion`, `Low Coupling`, `Controller` 5가지 기본 패턴은 Watanabe 5원칙(역할분담/작은 것/숨기기/의존성 최소화)과 1:1로 대응하고, `Protected Variations`과 `Polymorphism`은 GoF 생성/구조 패턴과 결합한다.

## Related
- 책: [[applying-uml-patterns]] / [[software-design-techniques]]
- 저자: [[craig-larman]] / [[watanabe-kouzo]]
- 클러스터: [[uml-oo-design-cluster]]
