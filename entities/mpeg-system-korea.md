---
title: MPEG 시스템 (유시룡·장규환·이병욱·김종일·정해묵 1997)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, video-compression, mpeg-standard]
sources: [raw/books/mpeg-system-korea.md]
confidence: high
---
# MPEG 시스템 (유시룡·장규환·이병욱·김종일·정해묵 1997)

> 표지/원저: **유시룡 · 장규환 · 이병욱 · 김종일 · 정해묵** 공저 (대우전자 영상연구소 계보)
> 출판: (출판사 원문 미확인), 1997, 253p

## 개요
MPEG 표준 3개 파트(시스템·비디오·오디오) 중 **시스템**(ISO/IEC 13818-1) 부분만 기술적으로 해설한 국내 최초의 공저 교재. MPEG은 1988년 ISO/IEC JTC1/SC29/WG11에서 시작하여 1994년 싱가포르 회의에서 MPEG-2 IS(International Standard)로 확정됐다는 역사적 맥락(제1장) 아래, 용어·약자·기호(2-3장) → **트랜스포트 스트림(TS)·프로그램 스트림(PS)** 의 구조와 PES 패킷·타이밍 모델(제4장) → **시스템 목표 디코더(S-STD)** model: TS 기준 **T-STD**(buffer model·출출률)와 PS 기준 **P-STD**(제5장) → **PCR·SCR·DTS·PTS** 타이밍 시맨틱, TS 스플라이싱(제5장) → PES·PSM·PSD 패킷 신택스(제6장) → TS 패킷·적응필드·descriptors(제7장)로 전개 `[raw/books/mpeg-system-korea.md]`.

## 장 구조 (TOC 기반, 253p)
1. 서론
2. 용어 정의
3. 약자와 기호 (산술·논리·관계·비트·할당 연산자, 간략기호, 상수)
4. **트랜스포트 스트림과 프로그램 스트림** — 개요, 스트림·패킷·패킷화, 시스템 인코딩·뮴플렉싱, TS/PS 개요, 상호 변환·비교, **PES 패킷**, 타이밍 모델, 조건부 수신, 시스템 목표디코더 및 응용
5. **시스템 목표디코더 모델** — 프로그램 정의·구성정보, PSI 뮴플렉싱·역뮴플렉싱, **T-STD 모델** 구성·입출시간·버퍼·데이터 처리, **P-STD 모델**, 시스템 클럭 시맨틱 (PCR·SCR·ESCR·DTS·PTS), TS 스플라이싱
6. **PES 패킷의 신택스와 의미** — 일반적 PES, PSM(PSM pes), PSD(PSD pes)
7. **트랜스포트 스트림에서의 신택스와 의미** — 일반적 TS 패킷, 적응필드, 각종 descriptors
+ 부록: CSPS(constrained system parameters stream), 참고 국제표준, TS 디코딩

## 핵심 내용
- **시스템 정의**: MPEG 시스템은 비디오·오디오 elementary stream을 패킷화하여 저장/전송하는 과정; **저장매체 = PS**(MPEG-1), **방송/전송 = TS**(MPEG-2) `[raw/books/mpeg-system-korea.md]`
- **S-STD model**: 시스템 디코더의 정합 테스트 기준 — T-STD(TS 기준, buffer model 중심)와 P-STD(PS 기준)의 구조·입출시간·버퍼 운영 방법을 체계화 `[raw/books/mpeg-system-korea.md]`
- **타이밍 시맨틱**: PCR(Program Clock Reference), SCR(System Clock Reference), ESCR(Elementary Stream Clock Reference), DTS(Decoding Time Stamp), PTS(Presentation Time Stamp)의 정의·발생 메커니즘 `[raw/books/mpeg-system-korea.md]`
- **PSI**: Program Specific Information — PSM(Program Stream Map), PSD(Program Stream Directory)와 관련 뮴플렉싱·역뮴플렉싱 `[raw/books/mpeg-system-korea.md]`
- **TS 스플라이싱**: 실시간 스트림의 끊김 없이 이어붙이는 기법, 스플라이싱 정보(스탬프, PID) `[raw/books/mpeg-system-korea.md]`
- **PSM·descriptor 체계**: video window·system clock·bitrate·buffer·IBP 등 18종 이상의 descriptor 정의 `[raw/books/mpeg-system-korea.md]`

## Related
- 저자: [[yoo-si-ryong]] · (공저: 장규환·이병욱·김종일·정해묵 — 슬러 미지정)
- 개념: [[video-compression-mpeg]] — 영상 압축 표준 (MPEG/H.261 계열)
- 인접: [[mpeg2-source-code-commentary]] (MPEG-2 비디오 코드 해설) · [[video-compression-standards-korea]] · [[digital-video-engineering-korea]]
