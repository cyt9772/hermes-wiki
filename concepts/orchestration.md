---
title: 오케스트레이션 (Orchestration)
created: 2026-10-19
updated: 2026-10-19
type: concept
tags: [ai, ai-agent, llm, orchestration, multi-agent]
sources: [raw/books/ai-agent-engineering.md, raw/books/ai-agent-dev-ollama.md, raw/books/llm-ai-agent-7projects.md, raw/books/harness-engineering.md]
confidence: high
---
# 오케스트레이션 (Orchestration)

> "단일 에이전트로 시작해 멀티 에이전트 시스템으로 전환해야 하는 **시점과 기준**" — [[ai-agent-engineering]] 서문

## 개념
에이전트(단일 또는 복수)의 작업 순서·분기·도구 호출·컨텍스트 전달을 조율하는 구조. 4개 서적에서 모두 "모델 자체보다 구조"의 핵심으로 등장.

## 서별 패턴·패러다임
| 서적 | 장 | 핵심 패턴 |
|------|----|-----------|
| [[ai-agent-engineering]] | Ch.5 (p128) | 반사형(Reactor) · ReAct · Plan-Execute · 쿼리 분해 · 성찰형(Reflexion) — 5대 오케스트레이션 패턴 |
| | Ch.8 (p215) | Single→Multi 전환: 스웜, 조율 방식, **A2A 프로토콜**, 메시지 브로커, 액터 프레임워크 |
| [[ai-agent-dev-ollama]] | Ch.8 (p211) | 랭그래프(노드/에지) 기반 멀티 에이전트: 챗봇·도구·사용자 입력 노드 조합 |
| [[llm-ai-agent-7projects]] | Ch.7 (p282) | **계획과 실행의 분리** — 계획/실행 에이전트 패턴(스마트 스케줄러: 물류·재고) |
| | Ch.10 (p375) | 멀티 에이전트 체계: AutoGen, MetaGPT로 팀형 에이전트 구현 |
| [[harness-engineering]] | Ch.6 (p110) | 오케스트레이터 = 리더(이벤트 루프), 팀원 = 피어; TeamCreate/TaskCreate/SendMessage |
| | Ch.8 (p152) | **6가지 아키텍처 패턴**: 파이프라인 · 팬아웃/팬인 · 전문가풀(라우터) · 생성-검증 · 감독자(런타임 동적분배) · 계층적 위임(3단계 금지) |

## 단일 vs 멀티 판단 기준
- Albada서: "어떤 방식으로 선택해야 하는가" = 모델 능력 × 작업 복잡도 × 지연/비용 허용 × 디버깅 용이성
- 하네스서: "팀 모드 과용(비용 폭발)"과 "서브에이전트 과용(과다 호출)"을 안티패턴 2로 지정 — 즉 **도움이 되는 순간의 분업, 아니라면 단일 에이전트**

## 관련
- [[ai-agent]] — 오케스트레이션이 통제하는 대상
- [[agent-harness]] — 오케스트레이터의 하네스적 관점
- [[mcp]] — 오케스트레이션이 호출하는 도구 인터페이스
