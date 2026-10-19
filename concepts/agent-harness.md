---
title: 에이전트 하네스 (Agent Harness)
created: 2026-10-19
updated: 2026-10-19
type: concept
tags: [ai, ai-agent, agent-harness, orchestration]
sources: [raw/books/harness-engineering.md]
confidence: high
---
# 에이전트 하네스 (Agent Harness)

> "병목은 능력이 아니라 **구조**다." — [[harness-engineering]] Ch.1 (p31)

> "챗봇과 싸우지 말고, **하네스를 설계하라.**" — 미셸 하시모토 epigraph, 권말

## 개념
**하네스 = models around** (모델을 둘러싼 모든 구조). LangChain이 명확히 한 대로, 하네스의 위치는 **모델 바깥**(서문). 모델 성능이 매번 신기록을 세우더라도 최종 결과를 결정하는 것은 **모델 + 하네스**의 조합이다.

- 프롬프트 엔지니어링: 단일 호출의 프롬프트만 다룸
- **하네스 엔지니어링**: 에이전트(roles) + 스킬(주식 절차) + 오케스트레이터(조율) + 툴 + 기억 + 검증 + 운영 루프를 **하나의 구조**로 설계

## 3가지 핵심 요소 (Ch.3, p57)
| 요소 | 질문 | 산출물 |
|------|------|--------|
| **에이전트** | Who (누가) | 역할 계약서 (본문 7섹션 + 가드레일 + 프론트매터 5필드) |
| **스킬** | How (어떻게) | `SKILL.md` — Description(호출 결정) + Progressive Disclosure 3단계 + Why-First |
| **오케스트레이터** | When & With Whom | 이벤트 루프(리더) — TeamCreate / TaskCreate(depends_on) / SendMessage |

## 6단계 메타스킬 파이프라인 (Ch.7, p133)
Phase 1 도메인 분석 → 2 팀 아키텍처 → 3 에이전트 → 4 스킬 → 5 오케스트레이션 → 6 검증 → **7 순환** (피드백 루프)

## 6가지 아키텍처 패턴 (Ch.8, p152)
1. **파이프라인** — 순차 (compile→review→deploy)
2. **팬아웃/팬인** — 병렬 분업 후 집계
3. **전문가풀(라우터)** — 라우터가 도메인별 전문 에이전트로 라우팅
4. **생성-검증** — 작성자와 검증자 분리 (hallucination 방어)
5. **감독자** — 런타임에 작업 분배·동적 분기
6. **계층적 위임** — 상위 팀이 하위 팀에 위임 (**3단계 금지** = 관리 과다)

## 하네스 진화 (Ch.10, p188)
- **Phase 0 현황 감사**: 모든 스킬 실행의 첫 관문 — 현재 구조/도구/실패 로그 점검
- **5-7 운영 루프**: 5-7개 운영 루프(로그·지표·피드백)로 정기 점검
- **두 가지 drift**: 문서-실무 drift(스킬 정의 vs 실제 수행) / 툴-drift(도구 버전 변화로 하네스 무결성 훼손)

## 하네스 등록: CLAUDE.md 포인터 (Ch.10, p189)
- **포인터는 4줄, 시스템은 4층** — CLAUDE.md는 **pointer only**(하네스 경로·엔트리포인트·환경 변수), 실제 스킬은 `./skills/`에
- 4단계 스코프: 전역(project) → 모듈(package) → 파일 → 함수
- 담을 것: 하네스 진입점, 도구 목록, 금지 동작, 운영 체크리스트
- 담지 말 것: 모델 내부(파인튜닝·RLHF), 상세 스킬 내용, 코드 상세

## 관련
- [[orchestration]] — 하네스의 오케스트레이션 레이어
- [[ai-agent]] — 하네스가 둘러싼 대상
- [[harness-engineering]] — 본서 entity
