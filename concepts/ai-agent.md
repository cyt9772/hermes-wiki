---
title: AI 에이전트 (AI Agent)
created: 2026-10-19
updated: 2026-10-19
type: concept
tags: [ai, ai-agent, llm]
sources: [raw/books/ai-agent-dev-ollama.md, raw/books/ai-agent-engineering.md, raw/books/llm-ai-agent-7projects.md, raw/books/harness-engineering.md]
confidence: high
---
# AI 에이전트 (AI Agent)

> "AI 에이전트는 목표를 달성하기 위해 외부 환경과 상호작용하고, 인터넷, 검색, 계산기 같은 도구를 활용해 문제를 해결하는 애플리케이션이다." — [[ai-agent-dev-ollama]] 1장 (p13)

## 정의 (4서 종합)
- **[[ai-agent-dev-ollama]]**: LLM을 "확률적 앵무새"로 낮춰보는 시각에 반대 — 에이전트는 **자율적으로 작동하며, 세세한 지시 없이도 목표 달성을 위한 방법을 스스로 계획**하는 추론 가능한 장치. 핵심 3요소: LLM(두뇌) + 도구(손) + 메모리(기억).
- **[[ai-agent-engineering]]** (Albada): 사전학습이 일으킨 혁명(1.2) — 에이전트 = LLM + 도구 + 메모리 + 오케스트레이션의 **시스템**. '워크플로(고정 경유지) vs 에이전트(동적 의사결정)' 경계(1.7)와, 단일↔멀티 전환 시점 판단 기준(Ch.8)을 제공한다.
- **[[llm-ai-agent-7projects]]**: Life 3.0(테그마크) 관점에서 "인공지능은 Life 3.0으로 가는 열쇠"(1장) — 에이전트 = 4대 핵심요소(의사결정·기억·도구 호출·계획)를 갖춘 LLM 기반 시스템, AaaS(Agent as a Service)·자기 진화형 AI 경향.
- **[[harness-engineering]]**: 문제 정의 전환 — "병목은 능력이 아니라 구조다". 같은 모델을 두고 **구조(환경)만 바꿨더니 49→79점**으로 오른 실험(p31)으로 시작.

## 에이전트 = LLM + 도구 + 메모리 + (오케스트레이션)
| 요소 | Ollama서 | Albada서 | 7프로젝트서 |
|------|----------|----------|-------------|
| LLM | 로컬 모델(올라마), LCEL 조립 | 모델 선택·파인튜닝(Ch1, Ch7) | GPT(OpenAI API) |
| 도구 | 검색엔진·챗봇 도구(Ch7) | MCP·상태유지 도구(Ch4) | 함수 호출(Ch5) |
| 메모리 | 연속 채팅(Ch4) | RAG·시맨틱 경험 메모리(Ch6) | 기억 기제(Ch2) |
| 오케스트레이션 | 랭그래프(Ch8) | ReAct/Plan-Execute(Ch5), 멀티(Ch8) | ReAct(Ch6), 계획/실행(Ch7) |

## 관련
- [[agent-harness]] — 에이전트를 둘러싼 구조 설계
- [[orchestration]] — 에이전트 제어 구조
- [[rag]] — 지식 접목
- [[mcp]] — 도구 인터페이스 표준
- [[artificial-intelligence]] — AI 도구의 큰 틀
