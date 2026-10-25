---
title: CMMI/프로세스 성숙도 (Capability Maturity Model)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [software-quality, software-testing-process]
sources: [raw/books/cmm-maturity-model.md, raw/books/software-engineering.md, raw/books/nhn-software-quality.md]
confidence: high
---
# CMMI/프로세스 성숙도

**"소프트웨어 개발 프로세스가 정의되고, 관리되고, 측정되고, 지속적으로 개선되는 정도를 5단계로 구분한 모델"** — 이 배치의 품질·프로세스 서적(8권)을 관통하는 공통 개념. 원저는 CMM(Capability Maturity Model): 카네기멜론 SEI가 개발, 1994년 Addison Wesley(Pearson)로 공식 출간, 한국에서는 2003년 송태국·이병헌 공역으로 정식 번역. 이 개념은 "개인의 기량"이 아니라 **조직의 프로세스**가 품질을 좌우한다는 사고방식을 도입한 모델이다.

## 5단계 성숙도 레벨 (원문 2~3장 근거)
| 레벨 | 명 | 핵심 | 대표 프로세스 영역 |
|---|---|---|---|
| 1 | 초기(Ad-hoc) | 프로젝트별 영웅 개인 의존 | — |
| 2 | 반복(Repeatable) | 기본 프로젝트 관리, 요구관리, SQA, CM | 요구관리, SQA, 형상관리, SPM |
| 3 | 정의(Defined) | 조직 표준 프로세스 정의·훈련 | 조직 절차 정의, OPM, 조직적 훈련, PPQA |
| 4 | 관리(Managed) | 수량 관리 — 프로세스·제품 측정 | 수량 관리(QPM), 프로세스 성능 관리(PPM) |
| 5 | 최적화(Optimizing) | 지속적 개선, 결함 예방, 기술 변화 관리 | 결함 예방, 기술 변화 관리, 프로세스 변화 관리 |

레벨 간 **누적성**: 레벨 4 없이는 레벨 5 성립 불가 — "위 레벨의 관행은 아래 레벨의 관행 위에서 작동"[raw/books/cmm-maturity-model.md]

## CMM = 진단 + 개선 로드맵 (원문 4~5장)
- **해석(assessment)**: 평가단이 프로세스 관행(핵심 실천 영역+관행)을 점검해 현재 성숙도 수준 판별.
- **사용(usage)**: 갭 분석 → 단계별 개선 우선순위 → 표준 프로세스 확산 → 재평가. "CMM은 목적지가 아니라 나침반"이라는 프레이밍.
- **높은 성숙도의 실증(6장)**: 우주 왕복선 탑재 소프트웨어 — 고신뢰성 분야의 프로세스 성숙 사례를 본문이 직접 다룸.

## 이 클러스터의 다른 책에서 성숙도 관점
1. **[[software-engineering]](김태달)**: 20장 "소프트웨어 품질보증"에서 SQA 정형 접근, walkthrough/inspection, 품질 매트릭스를 교재화 — CMM 레벨 2~3 프로세스 영역의 대학 교재적 대응. 22장 형상관리(SWM)는 CMM 레벨 2의 핵심 프로세스 영역.
2. **[[nhn-software-quality]](NHN 9인)**: 원문에 CMMI 등급 서술은 직접 등장하지 않으나, QP(코딩 컨벤션·리뷰·커버리지·정적 분석·복잡도 + 품질 지표·기준)를 "적용준비→적용→적용지원" 3단계로 조직 전체에 확산하는 구조 = 성숙도 모델의 "평가→기준 제정→개선" 루프가 포털 개발 조직에서 어떻게 운영되는가의 실증.
3. **[[software-testing]](Patton) 21장 SQA** 및 [[software-testing-practice]]의 테스트 관리 — 테스팅 프로세스가 조직 표준으로 정의·관리되는 것 자체가 레벨 3 이상 성숙의 요건.

## 핵심 통찰
- **프로세스가 품질이다**: 개인의 재능보다 프로세스의 성숙도가 결과의 변동을 결정 — CMM의 전체 논지.
- **측정이 관리의 전제**: 레벨 4(수량 관리)가 레벨 5(개선)의 기반이 되는 이유 — 지표 없는 개선은 추측.
- **성숙도는 등급이 아니라 방향**: 평가 점수보다 "다음 레벨의 프로세스 영역을 갖추는가"가 핵심 질문.

## 관련
- [[cmm-maturity-model]] — 원 저작(본 개념의 근간)
- [[song-taeguk]] / [[lee-bonghyun]] — 공동 번역
- [[software-quality-cluster]] — 품질 공통 프레임
- [[software-configuration-management]] — CMM 레벨 2 프로세스 영역(형상관리)
- [[software-testing-cluster]] — 테스팅 프로세스를 성숙도 프레임으로 관측
- [[software-engineering]] — SQA·형상관리 교재 축
