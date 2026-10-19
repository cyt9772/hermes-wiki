---
title: 올라마·오픈소스 LLM을 활용한 인공지능 에이전트 개발 입문
created: 2026-10-19
updated: 2026-10-19
type: entity
tags: [book, ai, ai-agent, llm, rag, mcp]
sources: [raw/books/ai-agent-dev-ollama.md]
confidence: high
---
# 올라마·오픈소스 LLM을 활용한 인공지능 에이전트 개발 입문

서영배 · 김병규 · 임재봉 지음, **위키북스** 2026-01-02 초판, ISBN 979-11-5839-655-8, 365p. 예제 코드: <https://github.com/godstale/ollama-mcp-tutorials>. 실습 환경: 올라마 + Qwen3 8B (로컬), Python 3.10+, uv 패키지 매니저, VS Code.

> "AI 에이전트는 목표를 달성하기 위해 외부 환경과 상호작용하고, 인터넷·검색·계산기 같은 도구를 활용해 문제를 해결하는 애플리케이션이다." (1장 p13)

## 구성 (12장)
| # | 장 | 핵심 |
|---|----|------|
| 1 | 대규모 언어 모델과 AI 에이전트 | 오픈소스 LLM 개념, LLM 구조·파라미터, 에이전트 정의/3요소 (p1) |
| 2 | 올라마와 랭체인 (개발 환경) | 올라마 설치, Qwen3 8B 로컬 실행 (p~27) |
| 3 | 랭체인: AI 프로그래밍의 시작 | LangChain 설치·LLM 호출·스트리밍·JSON 출력·LCEL (p~53) |
| 4 | 프롬프트 엔지니어링 | 템플릿·변수·연속 채팅 (p98) |
| 5 | RAG | 올라마 임베딩·벡터 저장소·랭체인 RAG·PDF RAG (p123) |
| 6 | 랭스미스: LLM 앱 모니터링 | 테스트·평가·트레이싱 (p156) |
| 7 | 에이전트와 도구적 LLM | ReAct·검색엔진 챗봇·멀티 도구 에이전트 (p182) |
| 8 | 랭그래프와 멀티 에이전트 | 노드/에지 구조·멀티 에이전트 (p211) |
| 9 | MCP 활용법 | Smithery·클로드 데스크톱·MCP 에이전트 (p261) |
| 10 | 프로젝트: AI 뉴스 블로그 자동화 | 노션 MCP + 긱뉴스 MCP (p297) |
| 11 | 프로젝트: 자동 회의록 | 위스퍼 + 로컬 LLM 멀티모달 (p317) |

## 위치 (4권 내 차별점)
- 4권 중 **가장 입문·로컬(올라마) 특화**. 클라우드 API 대신 로컬 LLM 전제.
- LangChain → 랭그래프 → MCP → 프로젝드로 이어지는 **실습 위주** 경로.
- 개념론적 깊이(Albada서)보다 **코드 실행 중심**.

## Related
- [[ai-agent]] [[rag]] [[mcp]] [[orchestration]]
- [[ai-agent-engineering]] (동일 주제, 이론+멀티에이전트 심화)
- [[llm-ai-agent-7projects]] (프로젝트 위주, 7개)
- [[harness-engineering]] (에이전트 팀 구조 설계)
- [[seoyoung-bae]] [[kimbyeonggyu]] [[imjaebong]] (저자)
