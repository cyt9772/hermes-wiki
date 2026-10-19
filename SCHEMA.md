# Wiki Schema

## Domain
AI books, stock investing, and programming/systems books (책/도서 소스 + 주식·투자 분석 + 시스템·프로그래밍·통신 기술), plus a small **Physics/Consciousness** cluster, and an **Engineering (공학)** cluster:
- **AI 쪽**: AI/ML/LLM 관련 책의 핵심 개념, 저자, 주요 주장, 책 간 연결. **AI 에이전트 클러스터** (2026-10-19 USB 4권): AI/AI 에이전트 시스템 설계·구현·운영 실무서 — 에이전트 아키텍처(단일/멀티), 도구 호출·MCP, RAG·메모리, 오케스트레이션·멀티에이전트, 평가·모니터링·보안·거버넌스. 로컬 오픈소스 LLM(올라마)·랭체인/그래프·프롬프트 엔지니어링 실무서 + 에이전트 개발 프로젝트 기반 입문서(AutoGPT/CAMEL/MetaGPT 등) + 하네스 엔지니어링(클로드 코드 하네스·에이전트·스킬·오케스트레이터)
- **Investing 쪽**: 종목/섹터/거시 분석, 회사 리서치, 밸류에이션, 투자 논지(thesis), watchlist
- **Programming 쪽**: OS/컴파일러/디버거/빌드도구/버전관리 등 시스템 프로그래밍, Windows·VB, 유닉스·리눅스 실전 유틸리티, LAN·VAN·ISDN 통신 + **USB** (버스·대용량 저장장치) + **Windows 미디어** (오디오/비디오/스틸, 스트리밍) + **XML** + **TCP/IP·소켓 네트워크** 프로그래밍 (2026-10-18 확장: USB/미디어는 인터페이스·프레임워크라 공학 접경이지만 프로그래밍 개발서로 Programming에 분류 — 사용자 지시)
- **Physics·Consciousness 쪽** (2026-10-15 추가): 양자물리학 개념 + 양자물리학의 영성/뉴에지 해석 다큐멘터리. **규칙: 주류 물리학 내용과 다큐의 파생 해석(측정=관측 붕괴의 의식화, 의식이 현실을 창조 등)을 반드시 분리 기재; 해석 페이지는 `contested: true`.**
- **Engineering (공학) 쪽** (2026-10-18 추가): 무선·이동통신·전자공학 교재. **무선/이동통신** — MIMO·OFDM·채널 모델링·시공간 부호(STBC)·소프트웨어 정의 무선·MATLAB 시뮬레이션. **전자공학** — 회로/신호/전파·계측·전력전자 등 모듈 단위 실용 전자공학. **USB·미디어** (2026-10-18 사용자 지시: USB 관련 + Windows 미디어 파일을 공학에 분류) — USB 버스 프로토콜·대용량 저장장치(마스터 스토리지)·오디오/비디오/스트리밍 프레임워크. **규칙: 공학은 주류 학문 — 주류 내용이므로 `contested` 불필요. 수식·기호가 OCR에서 깨지기 쉬우니 식 번호·문맥으로 cross-check; MATLAB 코드 snippet은 `code` fence로 원문 보존하되 깨진 토큰은 원본 PDF 대조 후 `>` 주의표시.**
- **Network (네트워크) 쪽** (2026-10-18 사용자 지시: 네트워크 프로그래밍 4권을 network로 분류): TCP/IP 프로토콜 구조 + Windows Sockets·POSIX 소켓으로 하는 네트워크 프로그래밍

## Conventions
- File names: lowercase, hyphens, no spaces (e.g., `attention-mechanism.md`)
- Every wiki page starts with YAML frontmatter (see below)
- Use `[[wikilinks]]` to link between pages (minimum 2 outbound links per page)
- When updating a page, always bump the `updated` date
- Every new page must be added to `index.md` under the correct section
- Every action must be appended to `log.md`
- **Content language:** 페이지 본문은 한국어 또는 영어 혼용 가능 (소스 성격에 맞춰서).
  다만 파일명·태그·frontmatter 키는 항상 English.
- **Provenance markers:** 3+ 소스를 종합한 페이지에서 특정 소스에서 온 claim은
  문단 끝에 `^[raw/books/xxx.md]` 마킹으로 출처 연결.

## Frontmatter
```yaml
---
title: Page Title
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | comparison | query | summary
tags: [from taxonomy below]
sources: [raw/books/source-name.md]
# Optional quality signals:
confidence: high | medium | low
contested: true
contradictions: [other-page-slug]
---
```

### raw/ Frontmatter
```yaml
---
source_url: https://example.com           # or book metadata (author, isbn, chapter)
ingested: YYYY-MM-DD
sha256: <hex digest of the raw content below the frontmatter>
---
```

## Tag Taxonomy
**AI:** book, chapter, author, concept, llm, ml-basics, deep-learning, agents, architecture, inference, training, alignment, rag, mcp, orchestration, agent-harness
**Investing:** stock, company, sector, macro, strategy, valuation, earnings, risk, korea-kospi, watchlist
**Programming:** programming, object-oriented, os, unix, linux, compiler, build-system, debugger, version-control, ipc, signals, networking, data-communication, windows-api, xml
**Physics (신비·양자 영역):** quantum-mechanics, consciousness, measurement-problem, entanglement, new-age-interpretation, perception, consciousness-experiment
**Engineering (공학):** wireless-communications, ofdm, mimo, channel-modeling, space-time-coding, software-defined-radio, signal-processing, electronic-circuits, electromagnetic-waves, matlab-simulation, telecom-systems, electrical-engineering, usb-bus, usb-mass-storage, media-frameworks, audio-video
**Network (네트워크):** tcp-ip, sockets, network-programming
**Meta:** comparison, summary, thesis, source

Rule: 모든 페이지 태그는 이 분류에 있어야 함. 새 태그 필요 시 먼저 여기 추가.

## Page Thresholds
- **생성**: 엔티티/개념이 2+ 소스 등장 OR 1 소스의 핵심이면 페이지 생성
- **합치기**: 기존 페이지가 있는 언급은 기존 페이지에 추가
- **생성 금지**: 단발성 언급, 도메인 밖 사안
- **분할**: 200줄 초과 시 서브토픽으로 분할 + 상호 링크
- **아카이브**: 내용 전부가 대체되면 `_archive/` 이동, index 제거

## Entity Pages (회사, 저자, 책)
- Overview, 핵심 사실/날짜, 관련 엔티티 ([[wikilinks]]), 근거 출처
- 책 엔티티 페이지: 저자, 핵심 주장(thesis), 각 장 요약, 교훈, 관련 개념 링크
- 회사 엔티티 페이지: 비즈니스 모델, 핵심 지표, AI 관련성, 경쟁사, 밸류에이션 맥락

## Concept Pages
- 정의/설명, 현재 지식 상태, 미해결 논쟁, 관련 개념 링크
- 예: attention, moat, compound-interest, rpgm(RAG-Prompt-Grounding-Memory)...

## Comparison Pages
- 비교 대상과 이유, 비교 차원 (표 형식 권장), 종합 결론, 출처

## Update Policy
1. 날짜 우선 — 새로운 소스가 일반적으로 기존 내용을 대체
2. 진지한 모순이면 양쪽 입장을 날짜·출처 병기
3. frontmatter에 `contradictions:` 기록, lint 시 사용자에게 리뷰 요청
