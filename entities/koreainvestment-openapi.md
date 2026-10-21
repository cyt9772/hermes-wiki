---
title: 한국투자증권 Open API (KIS Developers) — Linux 자동매매 가이드
created: 2026-10-21
updated: 2026-10-21
type: entity
tags: [stock, korea-kospi, programming, networking]
sources: []
confidence: high
---

# 한국투자증권 Open API (KIS Developers) — Linux 사용 가이드

한국투자증권이 국내 증권사 중 가장 앞서 제공 중인(2022-04 개시) 개인 대상 Open API.
국내/해외(미국 포함)주식, 선물옵션, 채권, ELW/ETF/ETN까지 REST + WebSocket으로 제공.
한국증권 API가 아니라 **순수 HTTP 계열**이라 OS 제약이 없다 — **Linux에서 그대로 사용 가능**.

## Linux 호환성 결론
- REST API: App Key/Secret → OAuth 방식 access token 발급 → `requests` 호출. Windows 전용 SDK 없음.
- WebSocket: 접속키 발급 후 실시간 시세/주문 수신. `websocket-client` 등 Python 패키지 사용.
- 공식 샘플 코드는 Python 3.11+ (`uv` 권장) — `git clone && uv sync`으로 Linux에서 바로 구동.
- 단, 키 발급(서비스 신청)은 증권사 앱/홈페이지에서 해야 하며, 그 외 개발·운영은 OS 무관.

## 구성 (두 방식)
| 방식 | 용도 | 인증 |
|---|---|---|
| REST | 조회/주문(매수·매도·정정·취소), 계좌/잔고 | App Key/App Secret → access token (유효시간 제한, 만료 시 재발급) |
| WebSocket | 실시간 시세 기반 자동매매 | 별도 접속키 발급 |

## API 문서 구조
해외주식(미국주식 포함) 관련 그룹: `overseas_stock` (조회·주문·잔고·체결).
전체 166개 REST 엔드포인트가 8개 그룹(주식·채권·선물옵션 등)으로 나뉘어 있음.

## 설치 절차 (Linux)
```bash
# 1) 공식 samples 클론
git clone https://github.com/koreainvestment/open-trading-api
cd open-trading-api
uv sync                # uv 미설치 시: pip install -r requirements 계열로 대체

# 2) 키 설정 (kis_devlp.yaml 또는 .env)
#    KIS_APP_KEY, KIS_APP_SECRET, KIS_CANO, KIS_ACNT_PRDT_CD (필수)
#    모의투자 / 실전투자 키를 각각 발급받아 분리 관리
```

저장소 폴더 구조:
- `examples_llm/` — 단일 API 기능별 원본 샘플 (LLM 자동화 최적). 인증은 `kis_auth.py`
- `examples_user/` — 상품별 완결형 워크플로우 예제 (`overseas_stock`, `domestic_stock`…)
- `strategy_builder/` — 비주얼 전략 설계 + 시그널 기반 매수/매도
- `backtester/` — 과거 데이터 백테스팅 엔진

## 필수 선행 (발급 절차)
1. 한국투자증권 계좌 (미국주식 거래 가능, 해외주식 거래 가능)
2. 증권사 앱/홈페이지에서 **Open API 서비스 신청** (앱에서 직접 신청)
3. App Key / App Secret 발급 — **모의투자 · 실전투자 각각 별도 키**
4. (실시간 시세용) WebSocket 접속키 발급
5. `KIS_DISABLE_TRADING` 같은 안전게이트 옵션이 있는 커뮤니티 도구는 기본값이 거래를 차단함 — 활성하려면 명시적 플래그 필요

## 미국주식 주문 시간 (한국 기준, 유의)
- 미국 정규장: 한국 시간 기준 동절기 21:30~06:00 / 하절기 20:30~05:00
- 프리/애프터 세션: 정규장 전후 약 3시간 (증권사 지원에 따라 상이)
- 미국 공휴일·반장일 미거래. 한국주식과 시간대가 달라 스케줄러 분리 설계 필요.

## 실전 전 검증 순서 (권장)
1. 모의투자 키로 `chk_inquire_price.py`(종목 시세 조회) — HTTP/통신 정상 확인
2. 잔고/구매가능금액 조회 (`overseas_stock` 잔고 API)
3. 1주 단위 소액 매수 → 체결 확인 → 매도 → 취소 API까지 전 구간 테스트
4. 실전 키로 동일 스크립트 재실행 (같은 코드, 키만 교체)

## MCP (LLM 연동) 옵션
한국투자증권이 공식으로 MCP(모델 컨텍스트 프로토콜) 지원을 제공함:
- **Coding Assistant MCP** — API 질의/샘플 생성/오류 진단
- **Trading MCP** — 주문·시세 조회를 Claude/Cursor/Codex/Gemini에서 직접 호출
- 커뮤니티 `kis_mcp_server` — 166개 REST API를 MCP 서버로 노출, `KIS_ENABLE_TRADING=true`로 매매 활성. stdio/SSE/streamable-http 트랜스포트.
Hermes/LLM 에이전트 연동 시 이쪽 경로가 Python 직접 호출보다 간편할 수 있음.

## 관련 페이지
- [[retire-with-us-stocks]] — 미국주식 투자 전략 (이 API로 운영 대상)
- [[finance-recipes]] — 파이썬 금융공학 기초 (전략 계산 기초)
- [[stock-portfolio-monitor]] — (생성 예정) 포트폴리오 모니터링 설계
- [[pakhomxi-investing]] — ETF 중심으로 미국/미국 자산배분
- [[wiki/index]]

## 참고 링크
- 개발자 포털: https://apiportal.koreainvestment.com/
- 공식 samples: https://github.com/koreainvestment/open-trading-api
- LLM용 가이드(llms.txt): https://github.com/koreainvestment/open-trading-api/blob/main/llms.txt
- AI 확장 패키지: https://github.com/koreainvestment/kis-ai-extensions
