---
title: 반도체 소자 (Semiconductor Devices)
created: 2026-10-18
updated: 2026-10-22
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/practical-electronics-eng.md, raw/books/new-electronics.md, raw/books/intro-electronics.md]
confidence: medium
---
# 반도체 소자 (Semiconductor Devices)

## 정의
**부도체·도체의 특성 사이에서 동작 제어**되는 단결정 반도체(실리콘 중심) 소자. 전자회로의 핵심 부품 3대 계통: **다이오드 → 트랜지스터 → 사이리스터** (4장).

## 다이오드 (4.2)
- **PN 접합 다이오드** — 한방 통전, 정류
- **제너 다이오드** — 역선폭(저항) 정전압, 정조
- **버랙터(가변 용량) 다이오드** — 역선폭에 의한 정전용량 변조
- **LED / 레이저 / 광 다이오드** (5장 광전자와 함께)
- **마이크로파 다이오드** (샤피, 건, 터넬) — 고주파
- **스크티지 다이오드, 다이액** — 전압 보호·스위칭

## 트랜지스터 (4.3)
- **BJT (비포장형 접합)** — 전류 증폭기
- **JFET (접합형 전계 효과)** — 전압 제어 채널
- **MOSFET (금속 산화물 반도체)** — 고저항 입력, 전력 증폭
- **IGBT (절연 게이트 양극성)** — 전력 변환기
- **단접합 트랜지스터** — 발진·증폭

## 사이리스터 (4.4)
- **SCR (실리콘 제어 정류기)** — 전력 제어·전정
- **SCR-S (실리콘 제어 스위치)** — 양방향
- **트라이액** — AC 정류·조광
- **DIAC (다이오드 + 다이아크)** — 트리거
- **SUDS (초고속 다이오드 스위치)** — 고속 전류 제어

## IC 패키지 (4.6)
- DIP, SOIC, BGA, QFP 등 — 반도체 칩의 물리적 구현

> `raw/books/practical-electronics-eng.md` pp. 393-487

## 보충 소스 (2026-10-22 추가)
- **전자공학입문 (학당) ch.2** — 수험서 관점 소자 분류: 에너지대 구조·진성/불순물 반도체·홀 효과 → 다이오드(PN 접합·정류) → 트랜지스터 → **FET(접합형·MOS형)** → **반도체 스위칭 소자(PNPN·SCR·다이액·트라이액·단일접합 트랜지스터)** → 그 외(제너·터널·**더에미스터**·바리스터·가변용량·광전변환). `^[raw/books/intro-electronics.md]`
- **신전자공학 (학당) ch.1~2** — 전자현상(전자 방출 5종·에너지대·광전/열전/자기장 효과)에서 소자 동작으로의 물리 토대 + 진공관↔반도체 소자 대응. `^[raw/books/new-electronics.md]`
- **Digital Electronics 3ed (Tokheim)** — 같은 소자를 **디지털 동작**(SWITCHING) 관점에서: TTL/CMOS 게이트 내부 트랜지스터 동작, IC 래치, 74xx/40xx 시리즈 실전. `^[raw/books/digital-electronics.md]`
- **Levine 실험서** — 소자 동작의 **실험 검증**: Exp 4 TTL NAND/NOR 전달 특성, Exp 17·18 CMOS 특성·TTL 인터페이스, 부록 SCR(V-I 특성·게이트 제어)·CRO. `^[raw/books/digital-theory-experimentation.md]`

## Related
- [[analog-filter-design]] — 반도체 소자 기반
- [[digital-logic-basics]] — IC 구현
- [[sensors-electronics]] — 광전지·광 다이오드 소자
- [[amplifiers-analog-circuits]] — 트랜지스터·FET·MOSFET 증폭기(소자 활용)
