---
title: 소프트웨어 테스팅 (Ron Patton, 2nd ed)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, software-testing-process, software-quality, programming-mindset]
sources: [raw/books/software-testing.md]
confidence: high
---
# 소프트웨어 테스팅 (Software Testing, 2nd Edition)

Ron Patton(론 패튼)의 원저 `Software Testing, 2nd Edition`(Pearson Education, Sams 계열)을 **김도균**이 번역한 한국어판. 정보문화사가 2006년 4월에 초판 발행한 것. ISBN 89-56-74-315-0. 437쪽짜리 텍스트 레이어 PDF로, 원서 22장의 내용을 1부~6부 구조로 재편해 놓은 교양~입문 레벨의 테스트 교과서다.

## 장 구성 (원문에 기초)
- **1부 큰그림**: 1장 소프트웨어 오류의 배경지식(라이온킹, 펜티엄 FDIV, NASA 화성 착륙선, 패트리어트, Y2K 등), 버그의 정의·비용·테스터의 자질. 2장 소프트웨어 개발 절차(빅뱅/짜고 고치기/폭포/나선 모델, 팀 구성). 3장 테스트 현실(테스팅 10대 원리, V&V, 품질과 신뢰성).
- **2부 기본**: 4장 명세 검토(스펙 테스팅), 5장 블라인드/동등 분할, 경계 조건, 상태기법, 데이터 테스트.
- **3부~4부 기법**: 6장 코드 리뷰, 7장 트리/경로 기반 화이트박스, 8장 구성(컴포넌트/통합/시스템) 테스트, 9장 호환성, 10장 국지화 테스트, 12장 문서, 13장 보안, 14장 웹사이트 테스트.
- **5부 도구·관리**: 15장 자동화/도구, 16장 버그 배시/베타, 17장 작업계획, 18~19장 리포트·측정, 21장 QA.
- **6부 미래**: 22장 테스터 경력 개발.

## 핵심 3~5개
1. **테스팅 원리(Testing Lxioms)**: 완전한 테스트는 불가능하다, 테스트는 위험을 감수하는 행위, 많은 버그 발견 = 더 많은 버그가 존재(살충제 패러독스). 3장에서 10개 항목으로 나열 `[raw/books/software-testing.md]`
2. **검증(Verification) vs 유효성(Validation)**: "잘 만들었는가 vs 제대로 만들었는가" — 명세 검토가 V, 동적 실행이 V에 해당.
3. **동등 분할과 경계값**: 동적 블랙박스 설계의 축. 5장에서 "기본값/비어/공백/널/제로/없음"과 "invail, wrong, garbage" 데이터 케이스를 체계적으로 제시.
4. **테스터의 10대 자질**: 1장 "좋은 테스터의 자질" — 호기심, 분석력, 의사소통 등. 6부 22장에서 경력·자격증으로 확장.

## 관련
- [[ron-patton]] — 원저자
- [[kim-dogun]] — 번역자(김도균)
- [[software-testing-cluster]] — 테스팅 3권 비교
- [[software-quality-cluster]] — 품질 공통 프레임
- [[cmmi-process-maturity]] — 프로세스 성숙도 관점
