# Wiki Log

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> When this file exceeds 500 entries, rotate: rename to log-YYYY.md, start fresh.

## [2026-10-27] ingest | 말하기 영작문 트레이닝 (장근섭, 다락원 2013, 602p)
- **인제스트 대상:** /Down/말하기 영작문 트레이닝_220405_112929.pdf (스캔본, text-layer 없음).
- **방식:** tesseract 5.5.3 (kor+eng, 300dpi) 병렬 OCR (P=8) — 602/602 페이지 성공, 오류 0. USB/다운로드→`raw/books/malhagi-yeongjakmun-training.pdf` 로컬 백업 (git-ignore 대상) + sha256 `d6db4db9…03a870`. `raw/books/malhagi-yeongjakmun-training.md` 래퍼 (frontmatter + 9섹션·35법칙 목차 테이블 + OCR 전체 602 페이지).
- **산출물:** 엔티티 1 — `entities/malhagi-yeongjakmun-training.md` (Part 0 = 섹션 0010 '영어로 생각하기' 법칙 01~04 정리: 단도직입·논리·현재중심·끝까지 따짐; 저맥락 언어·SVO/SOV·술어 중첩 금지 예). 기존 페이지 5개 백링크 (english-writing-training, sungan-yeongjakmung-*, english-grammar-patterns, situational-conversation, lee-bo-yeong-conversation).
- **index.md:** Language 42→43, Total 442→443. **git:** raw 커밋 + final 커밋/푸시 (이 로그 작성 후).
> Format: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> When this file exceeds 500 entries, rotate: rename to log-YYYY.md, start fresh.

## [2026-10-25] ingest | 24 USB PDF — UML·설계 / 확률·추정·시스템 / SW 테스팅·품질 / 회로·수학·CDMA·MPEG (4 클러스터, text-layer 원서 24종)
- **인제스트 대상 (24종):**
  - **UML·객체지향 설계 (5권):** Applying UML and Patterns (Larman 2nd, Prentice Hall 2001, ISBN 0-13-092569-1) · Teach Yourself UML in 24 Hours (Schmuller, Sams 2nd) · UML 사용자 지침서 (Booch·Rumbaugh·Jacobson 3인, Addison-Wesley 원저, 인터비전 1999 심재철 외 공역) · UML과 Rational Rose (Wendy·Michael Boggs, SYBEX 2002, 김덕화 역) · 소프트웨어 설계 테크닉 (Watanabe Kouzo 외 9인, Nikkei 원저 2002, 성안당 2004, 김성훈 역)
  - **확률·랜덤 신호·추정·시스템 (6권):** Signals and Systems 2nd ed (Oppenheim·Willsky, Prentice Hall) · Probability, Random Variables, and Stochastic Processes 2nd ed (A. Papoulis, McGraw-Hill 1991) · Probability and Random Processes for EE 2nd ed (Leon-Garcia, McGraw-Hill) · Discrete Random Signals and Statistical Signal Processing (Charles W. Therrien, Naval Postgraduate School, Prentice Hall Signal Processing Series) · Lessons in Estimation Theory 3rd ed (J. Mendel, Prentice Hall) · Linear System Theory and Design (Chi-Tsong Chen, Prentice Hall)
  - **SW 테스팅·품질·프로세스 (8권):** 소프트웨어 테스팅 (Ron Patton 원저 2nd, 김도균 역) · 개발자도 알아야 할 SW 테스팅 실무 (STA 6인, 3rd) · MS 최고의 현직 테스터들이 밝히는 SW 테스팅 (앨런 페이지 외) · CMM 역량성숙도 모델 (CMU/SEI 원저, 송태국·이병헌 공역, Pearson 2003, ISBN 0-201-54664-7) · NHN은 이렇게 한다! SW 품질관리 (위키부스) · 소프트웨어공학론 (김태달, 형설출판사 2004) · 좋은 프로그램을 만드는 핵심 원리 25가지 (김종훈 외, 한빛MEDIA 2003) · 아무도 알려주지 않는 프로프로그래머가 되는 길 (김상호, 도서출판 아이콘 1995, ISBN 89-8126-002-8)
  - **회로·수학·통신 (5권):** Introduction to PSpice (Nilsson·Riedel, McGraw-Hill 4th sup., Electric Circuits 보조서) · Elementary Differential Equations with Linear Algebra (Finney·Ostberg, Addison-Wesley) — 파일명 미적분학.pdf이면서 실제 영문 ODE 교과서 · Coding and Information Theory 2nd ed (Richard W. Hamming, Prentice-Hall 1986) · CDMA/WCDMA 전파분석 (이상근, 2009) · MPEG 비디오 (대우전자 영상연구소, 1995)
- **방식:** text-layer 원서 24/24 → `pdftotext -layout` 추출 (총 9,585p) — Discrete Random Signals 751p는 초기 pdftotext 샘플 0자로 오해해 tesseract 병렬 OCR을 시작했으나, 전수 샘플(30페이지)에서 text-layer 존재 확인 → OCR 프로세스(751p) 종료하고 text-layer 경로로 대체. USB→`raw/books/<원본명>.pdf` 로컬 백업 + `sha256sum` (24/24, sidecar `raw/books/<원본명>.pdf.sha256`). `raw/books/<slug>.md` 래퍼 24종 (frontmatter: source_url·ingested·sha256 + 전체 원문).
- **산출물:** **새 엔티티 46** (책 24 + 저자 22: grady-booch·james-rumbaugh·ivar-jacobson·craig-larman·joseph-schmuller·watanabe-kouzo / alan-v-oppenheim·alan-willsky·a-papoulis·alberto-leon-garcia·jerry-mendel·chi-tsong-chen / ron-patton·kim-dogun·song-taeguk·lee-bonghyun·kim-tae-dal·kim-sang-ho / ross-finney·donald-ostberg·richard-hamming·lee-sang-geun) + **새 개념 11** (uml-oo-design-cluster · object-oriented-design-patterns / stochastic-processes-cluster · estimation-and-filtering · linear-system-control / software-testing-cluster · cmmi-process-maturity · software-quality-cluster / circuit-simulation-pspice · differential-equations-linear-system · cdma-radio-propagation-cluster).
- **기존 페이지 연결:** entities/james-w-nilsson.md — PSPIce 서 동인 확인(Iowa State, Electric Circuits 4th ed 동일인) → 저서 섹션에 [[introduction-to-pspice]] 1줄 추가, updated 2026-10-25. **이름 충돌 유의:** entities/kim-sang-ho(김상호, 아이콘 1995)와 기존 [[lee-bo-yeong-conversation]]·[[song-jong-gwan]] 등은 무관; 김성훈(software-design-techniques 번역)은 entities에 별도 slug 부재(단체 9인 저서 번역 → book 본문에 이름 기록).
- **신뢰도 플래그 (원본 대조):** discrete-random-signals 표지 "Tharles W. Therrier"는 OCR 왜곡 → 원문 내부 참고문헌에서 재확인한 "Charles W. Therrien"으로 기록(confidence: high). cmm-maturity-model은 CMMI 6등급 서술 **미확인** — NHN 책에 CMMI 언급 0건, 'QP 3단계 확산 구조'로 원문 근거 표현 대체. software-testing-practice는 STA 6인·software-testing-ms는 지음 3인+공역 5인·nhn은 9인·good-principles-25는 4인 — **단체 저자는 author entity 미생성**, book 본문의 저자 목록으로만 기록. mpeg-video(대우전자 영상연구소)는 회사 조직 저자 — author entity 미생성.
- **한자·링크·인수:** 작성 섹션 CJK-Han 0 (예외: 김태달·김상호 한자 표기 金泰達·金相澔 2건만 원서 표지 인용 원문 유지, `entities/kim-tae-dal.md`·`entities/kim-sang-ho.md`). `[[...]]` 미해결 0건 (전체 repo 대상 dangle scan — 기존 배치 유물 koreainvestment-openapi·log.md 3건 제외, 이번 배치 57개 파일은 0). `sources: []` 0건.
- **SCHEMA.md:** Engineering 도메인 섹션에 **신호·확률·제어 이론 (2026-10-25 USB 24권)** 클러스터 1문단 추가. Tag Taxonomy: Programming 태그 +4 (uml-oo-modeling · software-quality · software-testing-process · programming-mindset), Engineering 태그 +5 (stochastic-processes · estimation-filtering · state-space-control · circuit-simulation · differential-equations).
- **index.md:** Total pages 355 → 412 (entity +46, concept +11, comparison +0), Last updated 2026-10-25.
- **git 커밋:** 미실행 (부모 에이전트가 수행)

## [2026-10-24] ingest | 24 DSP·영상·통신·오디오·수학 PDF — USB `/run/media/yutae/Data` (공학 24종, 전부 text-layer 원서)
- **인제스트 대상 (DSP·영상·통신·오디오·수학, 24종):** DSP 교과서(Porat·Boaz 1997) · 신호및시스템(한국어, 1992) · DCT(Rao & Yip 1990) · 선형대수(Strang MIT 1988) · 정보공학(한국어 1996) · 디지털영상처리(Gonzalez & Wintz 2ed 1987) · Java 영상처리(Efford 2000) · C 화상처리 실무(NHK/국제테크노정보 1999) · Visual C++ 영상처리프로그래밍(황선규 2007) · Visual C++ 영상처리 구현(장동혁 1999) · Practical Digital Video C(Mattison) · MPEG-2(Watkinson) · Video Coding Standard Codecs(Ghanbari) · MPEG 시스템(한국어) · MPEG-2 코드해설(한국어) · 비디오압축표준(한국어) · 디지털영상공학(한국어) · 영상통신의 신호처리(문호, 대영사 1999) · 디지털오디오 MP3(송종관, 나남 2000) · 오디오프로세싱(박은경·권봉철, 소닉스) · Information Hiding/스텔레오그래피·워터마킹(Katzenbeisser & Pellet) · 안테나공학(최홍주, 차송출판사) · Bluetooth without Cables(Bray & Sturman) · LTE 무선기술 교육서(현대차)
- **방식:** text-layer 원서 → `pdftotext -layout` 병렬 추출(24/24 OK, 9,439p). `usb→raw/books/<slug>.pdf` 로컬 백업 + sha256sum. `raw/books/<slug>.md` 래퍼 24종(frontmatter: title·author·publisher·year·pdf·category + 전체 원문 본문). **6개 클러스터 서브에이전트 병렬**(DSP·수학 / 영상이론 / 영상프로그래밍 / 영상코딩·MPEG / 오디오·정보은닉 / 안테나·무선).
- **산출물:** **새 엔티티 48**(책 24 + 저자 24) + **새 개념 10**(digital-signal-processing · transform-coding · information-coding-theory · linear-algebra-applications · image-processing-fundamentals · image-processing-programming · video-compression-mpeg · mp3-perceptual-coding · steganography-watermarking · lte-radio-interface). 기존 엔티티에 cross-link: antenna-theory · antenna-design · Bluetooth · CDMA · OFDM · MIMO · wireless-channel-modeling.
- **권리·무결성:** 24종 PDF는 로컬 참조용만 — `.gitignore`라 text-only 원칙 준수. raw/books/*.pdf는 git 미포함. 모든 래퍼 sha256 = PDF 파일 sha256(기존 bluetooth/antenna convention 준수) — 24/24 cross-check 통과.
- **한자·링크 검증:** 작성 섹션(Extracted text 제외) CJK-Han 0, `[[...]]` wikilink 0건 미해결.
- **신뢰도 플래그 (원본 대조 필요):** signals-and-systems-korea 저자·출판사 원문 왜곡(희중당 추정 — 원문 미확인), video-communication-signal-processing 저자 문호·출판사 대영사 (원서명 확인 필요), mpeg-system-korea 출판사 원문 미확인, 정보공학 저자 3인 명칭 왜곡.
- **SCHEMA.md:** DSP·영상·통신·오디오프로세싱·수학 도메인 섹션 추가 + Engineering 태그 목록 확장.
- **index.md:** Total pages 297 → 355 (entity +48, concept +10).

## [2026-10-22] ingest | 13 공학 PDF — USB `/run/media/yutae/Data` (전자공학·전자기·통신, text-layer 원서 13종)
- **인제스트 대상 (공학, 13종):** Antenna Theory(Stutzman·Thiele 1981 608p) · Microwave Engineering(Pozar 4th 742p) · RF·초고주파 공학(Kai Chang 원저, 한빛미디어 2009 390p) · Time-Harmonic EM Fields(Harrington 1990 495p) · Engineering Electromagnetics(Hayt 5th 492p) · 만화로 배우는 전자기학(엔도 마사모리, 성안당 262p) · 유비쿼터스 홈 네트워킹(양재수·전호인, 전자신문사 400p) · CDMA의 모든 것(김갑용, 진한도서 2002 530p) · 기초전자기학(Griffiths 2nd 513p) · 전자기학 수험서(용홍택 1993 285p) · 전자회로입문(김병규 263p) · 해설 Bluetooth(MCPC, 신구문화사 2001 164p) · C++로 정전기학·기하광학(최행진, 내하출판사 2001 336p)
- **방식:** text-layer 원서 → `pdftotext -layout` 병렬 추출(13/13 OK). `usb→raw/books/<slug>.pdf` 로컬 백업(cp + sha256sum 기록). `raw/books/<slug>.md` 래퍼 13종(frontmatter: usb source path·title·category: engineering·confidence + 전체 원문 본문).
- **산출물:** **새 엔티티 19**(책 13 + 저자 6) + **새 개념 5**(electromagnetism-fundamentals · transmission-lines-microwave · antenna-design · cdma-dss-spread-spectrum · circuits-diagnosis-practice). 기존 개념·엔티티는 신생 소스로 cross-link.
- **김병규 구별 결정:** USB `전자회로입문` 저자 김병규와 기존 `[[kimbyeonggyu]]`(올라마·LLM 에이전트 개발 입문 공동저자)는 **동일 인물 아님** — `entities/intro-electronic-circuits.md`에 명시. 기존 `[[kimbyeonggyu]]` 엔티티는 유지.
- **Copyright:** 13종 PDF는 로컬 참조용만 — `.gitignore`라 text-only 원칙 준수. raw/books/*.pdf는 git에 미포함.
- **신뢰도 플래그 (원본 대조 필요):** Griffiths·Harrington·Pozar·Stutzman의 수식·도형은 원서 PDF 대조 필요(OCR 텍스트는 안정). `visualc-em-optics` MFC 코드 스니펫은 C++ 문법 표기 대조 필요.
- **index.md:** Total pages 273 → 297 (entity +19, concept +5).

## [2026-10-21] create | entities/koreainvestment-openapi.md
- 한국어 질문 "한국투자증권 API로 미국주식 투자, Linux 사용 가능?" 응답 내용을 엔티티화.
- Linux 호환성 결론(순수 HTTP 계열이라 OS 제약 없음), REST/WebSocket 구성, 공식 samples 설치 절차,
  키 발급 5단계, 미국주식 주문 시간, 실전전 검증 4단계, MCP 옵션을 정리.
- index.md: Entities +1 (255→256, entity 99→100).
- 소스: apiportal.koreainvestment.com, github.com/koreainvestment/open-trading-api (웹 검색, 2026-10-21 기준).

## [2026-10-17] ingest | 7 영어 PDF — USB `/run/media/yutae/Data` (3차, 전부 스캔본 → OCR) — **참고: 이전 17종은 USB에서 삭제됨**
- **인제스트 대상 (영어, 7종 / 총 2,947p):** 해커스 토익 VOCABULARY(504) · POINT CHECK 초보부터 고수까지 파이널 노트(242) · 미국영어발음 무작정 따라하기(400) · 송오현의 만점 영어에세이(248) · 영어스피킹 기적의 영단어 100(326) · 이기동 영어 구동사 연구(669) · 이기동 영어 전치사 연구(558)
- **방식:** 7종 **전부 스캔본**(`pdftotext` 0자, `Creator: Scanner System`) → tesseract 5-lang(300dpi) **재-OCR 필수**. `usb→raw/books/<slug>.pdf` 로컬 백업(cp -v, sha256 기록) 후 **병렬 5레인** OCR(`ocr-run7.sh`, ~13분, 7/7 OK·errors=0). 무결성: 7종 `pdfinfo` Pages == `full.txt` `===== PAGE N =====` 마커 수 1:1 일치.
- **산출물:** `raw/books/<slug>.md` 래퍼 7종(frontmatter: usb source path·sha256·OCR 경고 + `===== PAGE N =====` 본문) + **새 엔티티 7** + **새 컨셉 1**: english-pronunciation-phonetics. 기존 컨셉 5(english-listening-strategy · vocabulary-etymology · grammar-patterns · writing-training · business-english)에 신규 소스 링크 추가.
- **Copyright:** 7종 PDF는 로컬 참조용만 — `.gitignore`라 text-only 원칙 준수.
- **신뢰도 플래그 (OCR 아티팩트·원본 대조 필요):** hackers-toeic-voca 저자명(David Cho vs 김민정 — OCR '김민정'/'David Cho' 둘 다 확인, 교차 필요), point-check-up·lee-ki-dong-modals 출판사('OCR상 불분명'), lee-ki-dong-prepositions 저자 표기('이지동' vs '이기동' — 개정판 2020 기준 '이기동' 채택).
- **index.md:** Total pages 174 → 182 (entity +7, concept +1).

## [2026-10-17] ingest | 17 영어 학습/문학 PDF — USB `/run/media/yutae/Data` (2차, 전부 스캔본 → OCR)
- **인제스트 대상 (영어, 17종 / 총 7,168p):** 이보영의 영어회화사전(935) · 해커스 TOEIC READING(712) · 해커스 TOEIC LISTENING(569) · 거로 READING WORKSHOP(703) · Word Smart BASIC(684) · 위대한 개츠비(487) · 영어 경제뉴스 헤드라인(420) · 거로 CONVERSATION WORKSHOP(395) · 팝스 영단어(342) · E-mail 영어(298) · 어린왕자(298) · 여행영어 핸드북(273) · 잘 있거라(269) · News Reading(130) · 직독직해의 기술(196) · 순간영작문 중급(252) · 순간영작문 초급(205)
- **방식:** 17종 **전부 스캔본**(`pdftotext` chars=0, "Creator: Scanner System") → tesseract 5-lang(300dpi) **재-OCR 필수**. `usb→raw/books/<slug>.pdf` 로컬 백업(cp -v, sha256 기록) 후 ** 병렬 5레인** OCR(`run-parallel-ocr.sh`, ~40분, 17/17 OK·errors=0). 무결성: 17종 `pdfinfo` Pages == `full.txt` `===== PAGE N =====` 마커 수 1:1 일치.
- **산출물:** `raw/books/<slug>.md` 래퍼 17종(frontmatter: usb source path·sha256·OCR 경고 + `===== PAGE N =====` 본문) + **새 엔티티 17** + **새 컨셉 5**: english-reading-strategy · situational-conversation · english-writing-training · english-literature-bilingual · english-exam-toeic. 기존 컨셉 4(english-listening-strategy · vocabulary-etymology · grammar-patterns · business-english)에 신규 소스 링크 추가.
- **Copyright:** 17종 PDF는 로컬 참조용만 — `.gitignore`라 text-only 원칙 준수. raw/books/*.pdf는 git에 미포함.
- **신뢰도 플래그 (OCR 아티팩트·원본 대조 필요):** word-smart 저자(C.L. Green — 표지 OCR 'Brantley'), geo 2권 저자(김치기 — '치기' 언급 교차), email-english 출판사('2147/떼해삼영저판' garble), travel-english(**OCR 텍스트 34KB/273p 극소 → low confidence**).
- **index.md:** Total pages 152 → 174 (entity +17, concept +5).

## [2026-10-17] ingest | 8 영어 학습 PDF — USB `/run/media/yutae/Data`
- **인제스트 대상 (영어 학습, 8권 / 총 4,725p):** Profile 1 (OUP, 142p) · Larry King Live (242p) · 한방에 끝내는 영어 (문예림, 408p) · PERFECT WRITING (Freelec, 567p) · Perian Vocabulary (프라임영어, 719p) · KOREAONE Vocabulary 33000 (661p) · 신경향 아카데미 TOEFL (822p) · Graduate English (1204p)
- **방식:** 전량 **inner text 레이어** 사용 (tesseract 재-OCR 생략; A/B 2페이지 비교에서 embedded 텍스트가 영문은 고가독성이라 채택). `pdftotext`로 `raw/books/<slug>.md` 본문 생성 + `===== PAGE N =====` 마커, frontmatter(source_url/ingested/body sha256) 기록.
- **Copyright:** 8권 PDF는 `raw/books/*.pdf` 로컬 참조용만, `.gitignore`에 의해 git에서 제외 — `git ls-files 'raw/books/*.pdf'` 결과 0건 확인 (text-only 원칙 준수).
- **새 엔티티 8:** profile-1 · larry-king-live · ending-english-in-one-shot · perfect-writing · perian-vocabulary · vocabulary-33000 · sinyhyeong-toefl · graduate-english
- **새 컨셉 4:** english-listening-strategy(직청직해·chunking·받아쓰기) · english-vocabulary-etymology(접두사·어근·접미사) · english-grammar-patterns(5형식·준동사·문형 재분류) · business-english(OUP 6유닛)
- **Lint:** 새 12페이지에서 Cyrillic 0건(1건 adamant 발음기호 오타 수정), CRLF 0, broken wikilink 0(54개 전수 확인, 12개 중 54개 outbound). perian/vocabulary CJK 한자는 원서 표제·어원 표의 의도한 인용.
- **index.md:** Total pages 140 → 152 (entity +8, concept +4).
- **참고:** 4KB `._*.pdf`는 macOS AppleDouble 메타파일(trash 잔재)로 제외. USB `.Trashes/501/`의 큰 PDF는 이미 삭제(대체)된 사본이라 무시.

## [2026-10-17] lint | link graph · slug collision · style drift cleanup
- **슬러그 충돌 해소**: `entities/lifetime-financial-planning.md` → `entities/lifetime-financial-planning-book.md` (git rename). 이후 `[[lifetime-financial-planning]]`은 무조건 concept(3단계 설계)을, `[[...book]]`이 entity(책)를 가리킴 — 각 참조 의도와 일치
- **broken 링크 2건 시정**: `[[concepts/self-confidence-in-money]]`(dan-ariely-feeling-of-money.md) → 실존 페이지 `[[overconfidence-in-money]]`(ch.7 "돈에 대한 과신")로 재지정; `[[risk]]`(trading-timing-six-concepts.md, 대상 없음) → "위험 관리 관점" 텍스트로 대체
- **스타일 드리프트 정규화**: prefix 스타일 268개소(`[[concepts/x]]`, `[[concepts/x|라벨]]` 포함) → wiki 규약 `[[x]]`/`[[x|라벨]]`으로, 52개 파일. 전수 basename 유일성 검증 후 적용
- **글리프 정정**: concepts/seed-capital.md p63 인용문의 OCR 깨짐(`과과하기`, 불필요 富)을 clean 원문(pdftotext p62)과 대조해 "…종잣돈이라고 하면 그 중요성을 **간과**하기 쉽다…"로 정정
- **index.md**: Total pages 137 → 140 (comparisons/measurement-problem-interpretations 실존 확인, 헤더 stale 해소)
- **최종 검증**: 140개 페이지, 위키링크 전수 1049개 broken 0, prefix 0, entities/concepts CRLF/한자/키릴 drift 0
- Note: 이전 lint에서 flagged된 `[[measurement-problem-interpretations]]` 4개소는 오탐이었음 — 대상이 `comparisons/`에 실존(이전 커밋 f71a78a에서 생성)

## [2026-10-17] update | 27 raw/books/*.md — OCR text → clean pdftotext text
- USB `/run/media/yutae/UBUNTU 26_0/`에서 텍스트 레이어가 포함된 27권 PDF를 수신 (기존 27권과 1:1 매칭, 새 책은 없음)
- 모든 `raw/books/<slug>.md`: tesseract OCR 본문 → pdftotext(poppler) clean 본문으로 교체. 메타데이터·장 구성·페이지 구조 유지
- 4권에서 전제된 깨짐이 실제 해소 확인: `seventech`(IoT→`사물인터넷`, 5c→`5G`, NETS→`NFT`), `dan-ariely-feeling-of-money`(Poste→`포스트`), `money-study-over-toefl`(SSE/ES/Boch→정상), `mit-mba`(신비로운고속성장→정상 분리)
- 27개 raw 파일 모두 `source_url`, `sha256`(USB 바이너리 기준) frontmatter 반영 완료; 27개 `.prev` 백업은 `.gitignore`에 추가되어 local-only
- raw/는 불변 원칙 때문에 entities/concepts는 수정 안 함 → 본문 인용·wikilink·개념 페이지 그대로 유지
- Note: 이 작업은 raw text layer만 교체한 것이므로, 기존 entity/concept 인용 페이지 번호는 동일 PDF의 page marker에 의존 → 변경 없음

## [2026-10-05] create | Wiki initialized
- Domain: AI books & stock investing (AI 관련 책 소스 + 주식·투자 분석)
- Structure created: SCHEMA.md, index.md, log.md, raw/, entities/, concepts/, comparisons/, queries/

## [2026-10-05] ingest | 세븐테크 (The Seven Technologies, 2022)
- Source: /Down/전자책/세븐테크.pdf → raw/books/seventech.pdf (SHA-256 30e9...aed9)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 219/219 pages → raw/books/seventech.md 내장
- Created: entities/seventech.md, entities/kim-mi-kyung.md
- Created: concepts/artificial-intelligence.md, concepts/blockchain.md, concepts/robotics.md, concepts/iot.md, concepts/cloud-computing.md, concepts/metaverse.md
- index.md updated (7 pages), 5G 장 저자 OCR상 불분명 → 원서 대조 flag

## [2026-10-05] ingest | 금리의 역습 (rate-counterattack)
- Source: /Down/전자책/금리의 역습.pdf → raw/books/rate-counterattack.pdf (13M)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 204/204 pages → raw/books/rate-counterattack.md
- Created: entities/rate-counterattack.md
- Created: concepts/interest-rates.md, concepts/interest-rates-inflation.md, concepts/credit-cycle.md, concepts/fx-and-interest-rates.md
- Fixed pre-existing drift: blockchain.md 販売→판매, robotics.md 前→전직
- Author name not reliably OCR'd → flagged for cover/title-page cross-check

## [2026-10-05] ingest | 박곰희 투자법 (pakhomxi-investing)
- Source: /Down/전자책/박곰희 투자법.pdf → raw/books/pakhomxi-investing.pdf (23.5M, SHA-256 cf6bd6bf…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 299/299 pages → raw/books/pakhomxi-investing.md
- Created: entities/pakhomxi-investing.md (박곰희·박동호, 인플루언셜 2020-12, ISBN 979-11-91056-36-5)
- Created: concepts/asset-allocation.md, concepts/rebalancing.md, concepts/etf-investing.md, concepts/investment-asset-class.md
- chapter divider(p20/40/85/114/234) OCR garbled → 본문에서 주제 재구성, flag

## [2026-10-05] ingest | 미국 주식으로 은퇴하기 (retire-with-us-stocks)
- Source: /Down/전자책/미국 주식으로 은퇴하기.pdf → raw/books/retire-with-us-stocks.pdf (26.7M, SHA-256 bf0a4c6c…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 244/244 pages → raw/books/retire-with-us-stocks.md
- Created: entities/retire-with-us-stocks.md (황금부엉이·CIP 최철, (주)첨단, 2020~21 추정 — CIP 연도 OCR garble)
- Created: concepts/compound-interest.md, concepts/us-equity-market.md, concepts/index-investing.md, concepts/retirement-planning.md
- Parallel ingest race: dividend·etf·asset-allocation 페이지는 동시대 타 책 소스 → dividend 페이지는 생략(충돌 회피), 링크 purged

## [2026-10-05] ingest | 시대의 1등주를 찾아라 (find-the-top-stock)
- Source: /Down/전자책/시대의 1등주를 찾아라.pdf → raw/books/find-the-top-stock.pdf (SHA-256 6920bd5e…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 296/296 pages → raw/books/find-the-top-stock.md
- Created: entities/find-the-top-stock.md (이한영, 페이지2룩스 2021-09-08, ISBN 979-11-90977-38-8)
- Created: concepts/top-picking.md, concepts/momentum-investing.md, concepts/relative-strength.md, concepts/sector-rotation.md
- 증거 종목: 삼성전자·LG전자·포스코·SK하이닉스 등 + Package substrate 밸류체인(부록 p291-294)

## [2026-10-05] ingest | 배당왕 (dividend-king)
- Source: /Down/전자책/배당왕.pdf → raw/books/dividend-king.pdf (SHA-256 2734bd70…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 254/254 pages → raw/books/dividend-king.md
- Created: entities/dividend-king.md (삼성증권 리서치센터, 출판사 OCR상 미확인, 2019~20)
- Created: concepts/dividend-investing.md, concepts/dividend-growth.md, concepts/dividend-yield.md, concepts/payout-ratio.md
- 수치 토크(p034 회복률, p129 배당성향 28%) OCR 가독성 낮음 → "(OCR)" 표기로 flag

## [2026-10-05] ingest | 행동 경제학 (behavioral-economics)
- Source: /Down/전자책/행동 경제학.pdf → raw/books/behavioral-economics.pdf (SHA-256 ee14e779…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 343/343 pages → raw/books/behavioral-economics.md (18,522줄)
- Created: entities/behavioral-economics.md (도모노 노리오 著, 이명희 譯, 지형 2007-01, ISBN 89-957370-5-0)
- Created: concepts/loss-aversion.md, concepts/endowment-effect.md, concepts/anchoring-effect.md, concepts/mental-accounting.md, concepts/framing-effect.md, concepts/time-preference.md
- chapter-5(p132) 제목 garble → TOC p020에서 재구성 flag; 영문 저자명 OCR garble(Knetsch→60100 등) flag

## [2026-10-05] ingest | 슬기로운퀀트투자 (wise-quant-investing)
- Source: /Down/전자책/슬기로운퀀트투자.pdf → raw/books/wise-quant-investing.pdf (text-layer garble → OCR 우회)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 420/420 pages → raw/books/wise-quant-investing.md
- Created: entities/wise-quant-investing.md
- Created: concepts/backtesting.md, concepts/quant-investing.md, concepts/trend-following.md, concepts/value-investing.md

## [2026-10-05] ingest | 진짜 미국식 주식투자 (american-style-investing)
- Source: /Down/전자책/진짜 미국식 주식투자.pdf → raw/books/american-style-investing.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 463/463 pages → raw/books/american-style-investing.md
- Created: entities/american-style-investing.md
- Created: concepts/corporate-disclosure.md, concepts/investment-vs-speculation.md, concepts/valuation-multiples.md

## [2026-10-05] ingest | 지금 당장 재테크 공부하라 (start-investing-now)
- Source: /Down/전자책/지금 당장 재테크 공부하라.pdf → raw/books/start-investing-now.pdf (첫 시도 부제 포함 파일명 오류 → kill·재시작)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 364/364 pages → raw/books/start-investing-now.md
- Created: entities/start-investing-now.md
- Created: concepts/life-cycle-financial-goals.md, concepts/pipeline-income.md, concepts/real-estate-vs-financial-assets.md, concepts/rich-person-equation.md, concepts/wealth-four-elements.md

## [2026-10-05] ingest | 지금 당장 회계 공부 시작하라 (start-accounting-now)
- Source: /Down/전자책/지금 당장 회계 공부 시작하라.pdf → raw/books/start-accounting-now.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 359/359 pages → raw/books/start-accounting-now.md
- Created: entities/start-accounting-now.md
- Created: concepts/accrual-accounting.md, concepts/balance-sheet.md, concepts/cash-flow-statement.md, concepts/financial-ratio-analysis.md, concepts/income-statement.md

## [2026-10-05] ingest | 선대인의 대한민국 경제학 (seo-daein-korea-economics)
- Source: /Down/전자책/선대인의 대한민국 경제학.pdf → raw/books/seo-daein-korea-economics.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 383/383 pages → raw/books/seo-daein-korea-economics.md
- Created: entities/seo-daein-korea-economics.md (12강 토크쇼형 교양서)
- Created: concepts/creative-destruction.md, concepts/household-debt.md, concepts/korean-economy.md, concepts/longevity-risk.md, concepts/real-estate-market.md
- Fixed glyph drift: entities 集中度→집중도, concepts 聯储→연준(Fed), financial-ratio-analysis 三类→(3가지 축)

## [2026-10-05] ingest | 부의 감각 (dan-ariely-feeling-of-money)
- Source: /Down/전자책/댄 애리얼리_부의 감각.pdf → raw/books/dan-ariely-feeling-of-money.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 352/352 pages → raw/books/dan-ariely-feeling-of-money.md
- Author: 댄 애리얼리 (Dan Ariely, 듀크), 번역본
- Created: entities/dan-ariely-feeling-of-money.md
- Created: concepts/labor-illusion.md, concepts/money-illusion.md, concepts/overconfidence-in-money.md, concepts/pain-of-paying.md, concepts/present-bias.md

## [2026-10-05] ingest | 생애재무설계 지금 당장 시작하라 (lifetime-financial-planning)
- Source: /Down/전자책/생애재무설계 지금 당장 시작하라.pdf → raw/books/lifetime-financial-planning.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 165/165 pages → raw/books/lifetime-financial-planning.md
- Author: 홍은주 (삼성경제연구소, 2011-03)
- Created: entities/lifetime-financial-planning.md
- Created: concepts/lifetime-financial-planning.md, concepts/investment-golden-rules.md, concepts/retirement-income.md, concepts/reverse-mortgage.md, concepts/credit-management.md
- Warnings: p43-45 정의 garble → flag; p65 손절매 문구는 TOC p6에서 인용; p149 "약 15억~16억"은 예시 수치에서 추론(원문 없음)

## [2026-10-05] ingest | 경영의 모험 (adventure-of-management)
- Source: /Down/전자책/경영의 모험.pdf → raw/books/adventure-of-management.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 594/594 pages → raw/books/adventure-of-management.md
- Created: entities/adventure-of-management.md
- Created: concepts/corporate-communication.md, concepts/decision-making-under-uncertainty.md, concepts/entrepreneurial-leadership.md, concepts/innovation-through-iteration.md, concepts/organizational-culture.md

## [2026-10-11] ingest | MIT MBA (mit-mba)
- Source: /Down/전자책/MIT MBA.pdf → raw/books/mit-mba.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 172/172 pages → raw/books/mit-mba.md
- Author: 이원재 (출판사·연도·ISBN: 표지 OCR garbled → 기재 생략, 위조 방지)
- Created: entities/mit-mba.md
- Created: concepts/people-above-profit.md, concepts/weak-ties.md, concepts/batna-negotiation.md, concepts/social-enterprise.md
- Reused links: [[decision-making-under-uncertainty]] [[entrepreneurial-leadership]]

## [2026-10-11] ingest | 토익 공부보다 돈 공부 (money-study-over-toefl)
- Source: /Down/전자책/토익 공부보다 돈 공부.pdf → raw/books/money-study-over-toefl.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 241/241 pages → raw/books/money-study-over-toefl.md
- Author: 이권복 (한스미디어, ISBN 979-11-6007-361-4, 2019경)
- Created: entities/money-study-over-toefl.md
- Created: concepts/asset-vs-liability.md, concepts/seed-capital.md, concepts/inflation-hedge.md, concepts/investment-leverage.md
- Reused links: compound-interest, dividend-investing, value-investing, household-debt, credit-management 등 18개


## [2026-10-11] ingest | 실리콘밸리의 팀장들 (silicon-valley-teams)
- Source: /Down/전자책/실리콘밸리의 팀장들.pdf → raw/books/silicon-valley-teams.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 377/377 pages → raw/books/silicon-valley-teams.md
- Author: 김 스콧 (Kim Scott), 박세연 역 (2017 원서)
- Created: entities/silicon-valley-teams.md
- Created: concepts/radical-candor.md, concepts/feedback.md, concepts/team-management.md
- Normalized [[concepts/…]] prefixed links to plain [[slug]] for consistency with other 16 books

## [2026-10-11] ingest | 에센셜리즘 (essentialism)
- Source: /Down/전자책/Essentialism.pdf → raw/books/essentialism.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 310/310 pages → raw/books/essentialism.md
- Author: 그레거 맥쿼인 (Greg McKeown), 김원호 역 (RH코리아 2014)
- Created: entities/essentialism.md
- Created: concepts/essential-focus.md, concepts/selection-criteria.md, concepts/saying-no-as-choice.md, concepts/energy-as-performance-asset.md
- CJK glyph drift 1건(本书) 탐지·수정 완료

## [2026-10-11] ingest | 회계천재가 된 홍대리 (accounting-genius-hong)
- Source: /Down/전자책/회계천재가 된 홍대리.pdf → raw/books/accounting-genius-hong.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 963/963 pages → raw/books/accounting-genius-hong.md
- Author: 손봉석 (홍대리 시리즈)
- Created: entities/accounting-genius-hong.md
- Created: concepts/IFRS-accounting.md (신규 1개)
- Reused links: balance-sheet, income-statement, cash-flow-statement, financial-ratio-analysis, accrual-accounting, valuation-multiples, dividend-yield, payout-ratio, value-investing, corporate-disclosure
- Normalized [[concepts/…]] prefixed links to plain [[slug]]

## [2026-10-11] ingest | 신비로운 선물옵션가격이론 (futures-options-pricing)
- Source: /Down/전자책/신비로운 선물옵션가격이론.pdf → raw/books/futures-options-pricing.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 473/473 pages → raw/books/futures-options-pricing.md
- Author: 비슬산
- Created: entities/futures-options-pricing.md
- Created: concepts/futures-options-price-theory.md, concepts/turning-price.md, concepts/options-inversion.md, concepts/important-price.md
- Note: 이 책은 학술적 option-pricing이 아니라 국내 선물옵션 '가격 이론' 기법서 — arbitrage·implied-vol·Black-Scholes 없음(소스에서 확인됨), 해당 개념은 미생성

## [2026-10-14] ingest | 돈을 부르는 매매의 기술 (trading-technique)
- Source: /Down/전자책/돈을 부르는 매매의 기술.pdf → raw/books/trading-technique.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 425/425 pages (errors=0) → raw/books/trading-technique.md
- Author: 박병창 (포레스트북스, ISBN 979-11-91347-20-3)
- Created: entities/trading-technique.md
- Created: concepts/trading-timing-six-concepts.md, concepts/bull-bear-supply-demand.md, concepts/leading-stock.md
- Reused links: momentum-investing, trend-following, relative-strength, top-picking, futures-options-price-theory, value-investing, investment-vs-speculation 등
- Note: 103MB < 100MiB 한계라 PDF 그대로 push (LFS 불필요). OCR에서 수급표·차트 캡션 구간 손상 다수 — 엔티티 페이지에 코멘트 기록

## [2026-10-15] ingest | 파이썬을 활용한 금융공학 레시피 (finance-recipes)
- Source: /Down/전자책/금융공학레시피.pdf → raw/books/finance-recipes.pdf
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 400/400 pages (errors=0) → raw/books/finance-recipes.md
- Author: 김용환 (감수 장민자·노태협, 한빛미디어, ISBN 979-11-6224-082-3)
- Created: entities/finance-recipes.md
- Created: concepts/time-value-of-money.md, concepts/futures-theory-price.md, concepts/basis-contango.md, concepts/black-scholes.md, concepts/option-greeks.md, concepts/alpha-vs-beta.md, concepts/structured-products.md (신규 7개)
- Reused links: trading-technique, futures-options-pricing, value-investing, momentum-investing 등
- Note: 152MB > GitHub 100MB 한계 → git-lfs track(raw/books/*.pdf) 후 push. OCR 텍스트 레이어 0(완전 선별본), 수식·코드 블록은 garble 다수 — 개념 페이지 서론은 원본 PDF 인용으로 보완. 기존 futures-options-pricing(기법서)과 구별: 이 책은 학술적 option-pricing(B-S·그릭스)서


## [2026-10-15] ingest | NEW 비주얼베이직 6 입문 (vb6-introduction)
- Source: /home/yutae/work/pdf/20261015/프로그래밍/비주얼베이직6_입문.pdf → raw/books/vb6-introduction.pdf (local only, git-ignored, 148MB)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 357/357 pages (errors=0) → raw/books/vb6-introduction.md
- Author: HARUHIKO HAYASHI (하야시 하루히코, 원서 SoftBank 1998 / 영진닷컴 1999·2002, ISBN 89-314-1287-8)
- Created: entities/vb6-introduction.md, concepts/visual-basic.md
- Note: SCHEMA.md에 Programming 도메인 + 새 태그(programming, os, unix, linux, compiler, build-system, debugger, version-control, ipc, signals, networking, data-communication, windows-api, object-oriented) 추가 — 첫 비투자 도메인 책. OCR에서 "Visual Basic"→"Visual ㅁ2510" 등 영어 토큰 garble 다수, 엔티티 페이지에 기록

## [2026-10-15] ingest | 데이타통신과 컴퓨터통신 — LAN·VAN·ISDN (lan-van-isdn)
- Source: /home/yutae/work/pdf/20261015/통신_네트워크/LAN_VAN_ISDN.pdf → raw/books/lan-van-isdn.pdf (local only, git-ignored)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 422/422 pages (errors=0) → raw/books/lan-van-isdn.md
- Author: 김태윤 (고려대 전산과학과). 1994년 2월 28일 6판 발행, ISBN 89-303-0082-0
- Created: entities/lan-van-isdn.md
- Created: concepts/osi-7-layer-model.md, concepts/local-area-network.md, concepts/channel-access-protocols.md, concepts/isdn.md
- Note: 첫 통신/네트워크 도메인 책. B=64kbps·D=16kbps 확인(p.135). OCR garble: OSI→OsI, ISDN→"SH 정보 통신망", LAN→"씨/L씨의" — 엔티티에 기록

## [2026-10-15] ingest | 리눅스 프로그래밍 필수 유틸리티 (linux-essential-utilities)
- Source: /home/yutae/work/pdf/20261015/시스템/리눅스프로그래밍_필수유틸리티.pdf → raw/books/linux-essential-utilities.pdf (local only, git-ignored)
- OCR: tesseract (kor+eng, 300dpi), 796/796 pages (errors=0, parallel 10 workers) → raw/books/linux-essential-utilities.md
- Author: 백창우, 한빛미디어, ISBN 978-89-7914-759-9 (초판 2010-09-06)
- Created: entities/linux-essential-utilities.md
- Created: concepts/gcc-compilation-pipeline.md, concepts/software-configuration-management.md
- Note: 2010년 교재 — VCS는 Subversion/CVS 위주(git 없음), "당시 표준" 자료적 가치. OCR garble: TOC "AA"=C, "makeS"=make, "gecS"=gcc

## [2026-10-15] ingest | 유닉스 고급 프로그래밍 / APUE (unix-advanced-programming)
- Source: /home/yutae/work/pdf/20261015/시스템/unix_advanced_programming.pdf → raw/books/unix-advanced-programming.pdf (local only, git-ignored)
- OCR: tesseract (kor+eng, 300dpi), 802/802 pages (errors=0, parallel 10 workers) → raw/books/unix-advanced-programming.md
- 원저: W. Richard Stevens, Addison-Wesley APUE 2판 (ISBN 0-201-88854-8). 홍릉과학출판사 한국어 번역
- Created: entities/unix-advanced-programming.md
- Created: concepts/unix-ipc-signals.md
- Note: OCR이 5/6/7장 번호 혼동 → APUE 표준 19장 목록으로 정정(장 표에 기록). "모음"=I/O stream, "파수꾼"=Daemon, "의사 단말기"=pseudo-terminal(pty)

## [2026-10-15] ingest | What the Bleep Do We Know!? + Down the Rabbit Hole (what-the-bleep-do-we-know, 2008, video)
- Source: USB 삼성 T5 `/run/media/yutae/Samsung_T5/education/양자물리학/` — AVI 2편(What The Bleep 734,107,982B/108분, rabbit-hole 733,376,512B/80분) + SMI 자막 2편(1045줄·1253줄)
- **원본 AVI는 commit·raw 저장 모두 제외** (local only, ≈1.4GB). raw에는 자막 자막전문만: raw/videos/what-the-bleep-do-we-know.md (EUC-KR→UTF-8, HTML 태그 제거)
- 자막의 문자열 기록 = 이 다큐의 "텍스트 소스". ASR 불필요
- Created: entities/what-the-bleep-do-we-know.md (다큐 엔티티)
- Created: concepts/quantum-mechanics.md (주류 양자물리: 중첩·비국소성·불확정성·BEC·진공)
- Created: concepts/consciousness-and-observer.md (다큐 해석 — contested, confidence:low)
- Created: concepts/random-number-generators-and-intention.md (RIG·이모토·명상·원격뇌파 — 각 실험 근거 등급 low)
- Created: comparisons/measurement-problem-interpretations.md (주류 해석 vs 다큐 뉴에지 해석 비교)
- Note: SCHEMA.md에 Physics·Consciousness 도메인 + 태그(quantum-mechanics, consciousness, measurement-problem, entanglement, new-age-interpretation, perception, consciousness-experiment) 추가. **다큐의 "의식이 현실을 창조"는 contested·confidence:low로 등급 분리**, 주류 물리 서술과 반드시 분리 기재

## [2026-10-18] schema | Engineering(공학) 도메인 추가
- SCHEMA.md: Domain에 **Engineering (공학)** 클러스터 추가 — 무선·이동통신(MIMO·OFDM·채널 모델링·STBC·SDR·MATLAB) + 전자공학(회로·신호·전파·전력전자)
- SCHEMA.md: 태그 분류에 **Engineering (공학)** 태그 12개 추가 (wireless-communications, ofdm, mimo, channel-modeling, space-time-coding, software-defined-radio, signal-processing, electronic-circuits, electromagnetic-waves, matlab-simulation, telecom-systems, electrical-engineering)
- 이유: USB(Data)에 공학 교재 3권(MIMO-OFDM 무선통신과 MATLAB, 최신이동통신시스템, 실용전자공학) ingest 준비 — 새 도메인으로 체계화

## [2026-10-18] ingest | 최신 이동통신 시스템 (latest-mobile-comm-systems)
- Source: /run/media/yutae/Data/최신이동통신시스템.pdf (239G USB, exfat) → raw/books/latest-mobile-comm-systems.pdf (local only, git-ignored)
- 원서: Harada & Prasad, *Simulation and software radio for mobile communications* (Artech House, 2002, ISBN 1-58053-044-3). 국내 번역: 차종상·이종헌·강창목·왕진철 편역, 도서출판 그린 (ISBN 89-5727-063-9)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi) 509/509 pages, errors=0 (parallel xargs -P 8), → raw/books/latest-mobile-comm-systems.md (712KB, 24,876 rows)
- 장 (chapter) 구조: 서론(3-30) / 제1장 역사(3-42) / 제2장 MATLAB(36-64) / 제3장 변조 BPSK·QPSK·OQPSK·MSK(65-131) / 제4장 채널모델(131-?) / 제5장 CDMA(266-295) / 제6장 다중접속 ALOHA·CSMA(295-362) / 제7장 빔포밍(362-?) / 제8장 SDR(?-509)
- Created: entities/latest-mobile-comm-systems.md (책 엔티티)
- Created: entities/hiroshi-harada.md (원저자)
- Created: entities/ramjee-prasad.md (공동 원저자)
- Created: concepts/spread-spectrum-cdma.md
- Created: concepts/digital-modulation.md
- Created: concepts/wireless-channel-modeling.md
- Created: concepts/array-antenna-beamforming.md
- Created: concepts/software-defined-radio.md
- Created: concepts/ofdm-orthogonal-frequency-division.md
- Updated: concepts/channel-access-protocols.md (이 책에 ALOHA/CSMA 이동통신 시뮬레이션 추가, sources에 추가)
- Updated: index.md (3 entities + 6 concepts, Total pages 182→191)
- SCHEMA: 도메인/태그는 [2026-10-18] schema commit (2f53387)에 이미 등록
- OCR note: 수식·식 번호·MATLAB 토큰 깨짐 (02844&=CDMA에서, SEAALS=코드로, np-CSMA=비경합 CSMA, Splen=Send_len 등) — 원본 PDF 대조 권장

## [2026-10-18] ingest | MIMO-OFDM 무선통신과 MATLAB (mimo-ofdm-wireless-matlab)
- Source: /run/media/yutae/Data/MIMO_OFDM_무선통신.pdf (USB exfat) → raw/books/mimo-ofdm-wireless-matlab.pdf (285MB, 728p, sha256 기록, 커밋 제외)
- 저자 확정: 표지 vision으로 **조융수·김재권·양원영 공저, 홍릉과학출판사 2008** (OCR의 '조용수'는 오독) — **Harada/Prasad 원서가 아님** (첫 권과 저자·출판사 다름을 모든 페이지에 명시)
- OCR: tesseract 5.5.3 kor+eng 300dpi, 32코어 P=8 병렬 (parallel-ocr-pdf.sh v2, 위치인자 idiom) — 728/728pg, errors=0, ~5분
- Pages: entity 1 (mimo-ofdm-wireless-matlab) + author entity 3 (jo-yong-soo, kim-jae-gwon, yang-won-yeong) + concept 2 (mimo-multiple-input-multiple-output, space-time-coding) + raw wrapper (37,863줄) + sha256
- Links: index.md (entities +6, concepts +2, total 196), ofdm→mimo, channel-modeling↔mimo, harada/prasad에서 MIMO 서적 오연결 제거

## [2026-10-18] ingest | 모듈을 위한 실용 전자공학 (practical-electronics-eng)
- Source: /run/media/yutae/Data/실용전자공학.pdf (USB exfat) → raw/books/practical-electronics-eng.pdf (525MB, 1068p, sha256 기록, 커밋 제외)
- 소스 확정(권말 copyright p2): Scherz·Monk, *Practical Electronics for Inventors* 4ed (2016, McGraw-Hill ISBN 978-125958754-2) — **한문 번역본** 박진수 역, McGraw-Hill Korea+J Pub 2018-11-30 (ISBN 979-11-88621-32-3). Harada/조융수 2권과 무관
- OCR: tesseract 5.5.3 kor+eng 300dpi P=8 병렬 — 1068/1068pg, errors=0
- Pages: entity 1 (practical-electronics-eng) + author entity 2 (paul-scherz, simon-monk) + concept 8 (semiconductor-devices, sensors-electronics, analog-filter-design, timer-oscillator-circuits, power-supply-regulation, digital-logic-basics, microcontroller-arduino, fpga-hdl) + raw wrapper (74,852줄)
- Links: index.md entities+3 concepts+8 (total 207); SCHEMA Engineering 태그 12개 내로 정합

## [2026-10-18] ingest | USB 9권 배치 — 공학 3 + 프로그래밍 2 + 네트워크 4
- Source: /run/media/yutae/Data/ (USB exfat) → raw/books/*.pdf (sha256 기록, 커밋 제외). 전부 텍스트 레이어 있음 → OCR 생략, `pdftotext` 추출 (raw/*.txt + *.txt.d, 커밋 제외)
- 분류(사용자 지시): USB 2권 + Inside Windows Media → **Engineering**; XML 2권 → **Programming**; WinSock·TCP/IP 3권 → **Network**
- Books:
  1. USB 완전정복 (Jan Axelson, 신진철 역·디오이즈 감수, 에이콘 2011개정)
  2. USB 대용량 저장장치 (Jan Axelson, 성원호·최강민 역, 에이콘)
  3. Inside Windows Media (Microsoft Corporation, New Riders/Macmillan 2000, Think.Tec 역 Com&Books 2000)
  4. XML For the WWW (Elizabeth Castro, Peachpit 2001, 한국어 비앤비 2001-02)
  5. 10일 만에 배우는 XML (야마다 요시오 Yoshihiro Yamada, 쇼에이스 2001, 한국어 영진닷컴 2002)
  6. Windows Sockets Network Programming (Bob Quinn·Dave Shute, Addison-Wesley 1996, 17장)
  7. TCP/IP 완전정복 (Karanjit S. Siyan, New Riders 1997; 이도희 역, 성안당 2001-06)
  8. TCP/IP Network Programming (Murayama Yukio 무라야마 유키오, 오옴사·성안당 2005, 송봉길 역)
  9. 컴퓨터 네트워크 프로그래밍 (김화종, 강원대 정보통신연구소, 354p 7장 — 출판사/연도 원서에 표기 없음, 신뢰도 플래그)
- Pages: entity 17 (책 9 + 저자 8: jan-axelson, elizabeth-castro, yoshihiro-yamada, bob-quinn, dave-shute, karanjit-siyan, yukio-murayama, kim-hwa-jong) + concept 14 (usb-bus-architecture, usb-hid, usb-power-management, usb-mass-storage-class, streaming-media-architecture, xml-fundamentals, xslt-styling, winsock-api, socket-programming-patterns, tcp-ip, raw-sockets, java-sockets, winsock-bsd-compare, jdbc) + raw wrapper 9
- Links: index.md 207→239 (entities 88 · concepts 150 · comparisons 1); SCHEMA.md Programming/Network 도메인 태그 추가
- 저자 확인: raw front matter 1~12pg 직접 대조 (wrapper 메타데이터만 신뢰하지 않음); 추측 역자·출판사명 생략 정책 적용

## [2026-10-19] ingest | USB 4권 배치 — AI 에이전트 클러스터 (도메인: 인공자니/AI)
- Source: /run/media/yutae/Data/ (USB) → raw/books/*.pdf 4권 (sha256 기록, 커밋 제외). 전부 텍스트 레이어 확인 → OCR 생략, pdftotext -layout
- Books:
  1. 올라마·오픈소스 LLM을 활용한 AI 에이전트 개발 입문 (서영배·김병규·임재봉, 위키북스 2026-01, 365p) — 로컬 LLM 실습: 랭체인·프롬프트·RAG·랭스미스·랭그래프·MCP
  2. AI 에이전트 엔지니어링 (Michael Albada 원저 *Building Applications with AI Agents*, 강민혁 역, 한빛미디어 2026, 400p) — 설계·오케스트레이션·멀티(A2A)·보안(MAESTRO)·거버넌스
  3. 7가지 프로젝트로 배우는 LLM AI 에이전트 개발 (黄佳 원저 大模型应用实战 2024, 김진호 역, 제이펍 2025, 437p) — Assistants API·LangChain·LlamaIndex·AutoGPT·CAMEL·MetaGPT
  4. 하네스 엔지니어링 with 클로드 코드 (황민호, 한빛미디어 2026-06, 307p) — 에이전트·스킬·오케스트레이터 구성, 6단계 메타스킬, 6가지 아키텍처, CLAUDE.md 포인터
- Pages: entity 10 (책 4 + 저자 6: michael-albada, huang-jia, hwang-minho, seoyoung-bae, kimbyeonggyu, imjaebong) + concept 5 (ai-agent, rag, mcp, orchestration, agent-harness) + raw wrapper 4
- Links: index.md 239→255 (entities 99 · concepts 155 · comparisons 1); SCHEMA.md AI 도메인 서술 + 태그(rag/mcp/orchestration/agent-harness) 추가; concepts/artificial-intelligence.md에 에이전트 클러스터 섹션 연결
- 저자 확인: raw front matter 직접 대조; B2 원저 Michael Albada (강민혁 역), B3 원저 黄佳 (Posts and Telecom 2024, Media Solutions Tokyo 경유)

## [2026-10-22] ingest | 회로·전자 기초 3권 (electronics-basics, theory-of-circuits, circuits-and-systems)
- Source: /run/media/yutae/Data/ (USB exfat) → raw/books/{electronics-basics,theory-of-circuits,circuits-and-systems}.pdf (sha256 기록, 커밋 제외). 3권 전부 텍스트 레이어 확인 → OCR 생략, pdftotext -layout 추출 (raw wrapper: electronics-basics 616p, theory-of-circuits 506p, circuits-and-systems 671p)
- Books:
  1. 전자공학의 기초 — 원저 Bernard Grob『Basic Electronics』5ed, 최성재 편역, 학당, 616p. 전자현상→DC/AC 회로→자기/유도→반도체(29장)→트랜지스터 증폭(30장)→디지털(31장)→집적회로(32장) 32장 + 부록 A–H, 완전학습 문제 체제(약 2,000문항)
  2. 회로이론 — 검정연구회 편, 『전기기사시리즈』(전기·산업기사 자격시험 대비), 506p. 직류→정현파→RLC→교류전력→결합→다상(3상)→대칭좌표법→왜파→2단자/4단자망→분포정수→과도→라플라스→전달함수 17장, 기출분석·문제풀이 중심
  3. 회로 및 시스템 — 차균현(공학박사) 저, 대학 회로이론 교재, 671p. 회로개념→회로방정식→미분방정식(특성근)→라플라스(부분분수·Heaviside)→신호변환(중첩적분)→상태방정식(Cayley-Hamilton)→임피던스함수·테브난/노턴→극-영점·안정성→2단자 파라미터→정상상태·주파수응답(Bode·Nyquist)→Fourier→감도/허용오차→z-변환 20장 + 부록
- Created: entities/electronics-basics.md, entities/theory-of-circuits.md, entities/circuits-and-systems.md (책 엔티티 3)
- Created: concepts/dc-ac-circuit-analysis.md (3권 공통 회로해석 코어 — 옴·키르히호프·중첩·테브난/노턴·RLC·공진; sources 3권 전부)
- Created: concepts/laplace-transform-circuits.md (라플라스·S-평면·상태방정식·극-영점 — circuits-and-systems 주 소스 + raw/books/nilson-riedel-electric-circuits.md 소스 링크. 해당 raw 페이지는 별도 에이전트 작업 대상이라 링크만)
- Updated: concepts/digital-logic-basics.md (Related에 [[dc-ac-circuit-analysis]] 회로 맥락 링크 추가, updated 2026-10-22)
- Updated: concepts/analog-filter-design.md (Related에 [[dc-ac-circuit-analysis]]·[[laplace-transform-circuits]] 추가, updated 2026-10-22)
- Links: index.md entities+3 / concepts+2 (Total pages 256→261, Last updated 2026-10-22)
- 주의: 원 PDF 3권 모두 한자 혼용 표기 체재라 텍스트 추출 결과에도 한자 토큰이 섞여 있음 — 개념·장 구조 학습엔 무방, 수식·수치 재사용 시 원본 대조 권장. theory-of-circuits는 자격시험 문제집이라 문장 단편화 심함. confidence는 3권 모두 medium, dc-ac-circuit-analysis는 high(3수 교차 확인).
- git commit: 미실행 (부모 에이전트가 수행)

## [2026-10-22] ingest | 공학 수학·수치해법 2권 (kreyszig, numerical-recipes-in-c)
- Source: raw/books/advanced-engineering-mathematics.md (Kreyszig『Advanced Engineering Mathematics』8th ed., Wiley 1999, 1285p — pdftotext -layout 텍스트 레이어 추출, sha256 1fdca…acf6d), raw/books/numerical-recipes-in-c.md (Press·Teukolsky·Vetterling·Flannery『Numerical Recipes in C』2nd ed., Cambridge Univ. Press 1992, 1022p — 텍스트 레이어 추출, sha256 dcc34…634). PDF 원본은 로컬 참조용(git-ignored).
- Created: entities/advanced-engineering-mathematics.md (책 엔티티 — Part A–G 23장 구조, 모델링→해법→해석 철학, OCR 주의)
- Created: entities/numerical-recipes-in-c.md (책 엔티티 — 20장 구조, 알고리즘+C 코드 병기, gaussj snippet + 깨진 토큰 주의 표시)
- Created: entities/erwin-kreyszig.md (저자 — Ohio State University, 8ed 기준)
- Created: concepts/numerical-methods-science-computing.md (보간·적분·미분·고유값·푸리에 — 두 소스 모두에서 2줄씩 인용, 오차 분류 비교표)
- Created: concepts/differential-equations-engineering.md (상미분·편미분·라플라스·특수함수 — Kreyszig 중심, sources 1개)
- Cross-links: [[differential-equations-engineering]] ↔ [[numerical-methods-science-computing]] ↔ 책 2 ↔ [[erwin-kreyszig]] ↔ [[practical-electronics-eng]](관련 책) ↔ [[laplace-transform-circuits]](회로 맥락)
- Links: index.md entities +3 (books 2 + kreyszig) · concepts +2, Total pages 256 → 265 (sibling circuits-3권 entry와 병합 계수), Last updated 2026-10-22
- 주의: 두 raw 모두 텍스트 레이어 내장본(OCR 없음)이라 추출 자체는 양호하나 수식·C 코드 토큰 일부 깨짐(예 'mnt'→'int') — code snippet 인용 시 원본 PDF 대조 필요 표시. 한자(CJK)/키릴 문자 없음 확인.
- git commit: 미실행 (부모 에이전트가 수행)

## [2026-10-22] ingest | 디지털·증폭 전자공학 4권 (digital-electronics, digital-theory-experimentation, new-electronics, intro-electronics)
- Source: raw/books/{digital-electronics.md (Digital Electronics 3ed, Tokheim, McGraw-Hill Basic Skills 1990, 352p), digital-theory-experimentation.md (Morris E. Levine『Digital Theory and Experimentation Using ICs』2판 297p, 실험 20개), new-electronics.md (이수원·구기준·임영근·이영노 공저『신전자공학』학당 526p, 기술직 수험서), intro-electronics.md (국가기술자격검정시험연구회 편『전자공학입문』학당 573p, 통신공사·공무원 수험서)}. 모두 텍스트 레이어 추출.
- Created: entities/digital-electronics.md — 디지털 코어(2진 코드·게이트·부울대수 → MUX/디코더·FF/시프트/카운터 → 산술·메모리 → op-amp 매개 D/A·A/D), 직업학교 Self-Test 체제
- Created: entities/digital-theory-experimentation.md — 20개 실험: 게이트·부울대수 → FF·카운터(7493/7490)·시프트(7495/74164) → IC 타이머(74122/74121/555)·RAM → op-amp·D/A(74101/74114)·A/D(74165/74168) → CMOS/TTL 인터페이스
- Created: entities/new-electronics.md — 10장(전자현상·소자·펄스·BJT/FET 증폭·연산증폭·발진·변복조·전원·집적) 526p, 각장 3단 문제(단답→선다→비선다), 진공관↔반도체 대응
- Created: entities/intro-electronics.md — 11장(진공관·반도체소자·전원·증폭·op-amp·발진·변복조·펄스·논리·집적) 573p, 기술직 수험서
- Created: entities/morris-levine.md — Levine 2판 저자 (Staten Island CC, CUNY) — single-book author (book 1권 집중 → 임계 충족)
- Created: concepts/amplifiers-analog-circuits.md — BJT/FET/MOSFET 증폭(동특성·T/h 등가·바이어스·되먹임·전력증폭), 연산증폭기(가상 접지·미분/적분·BiFET/BiMOS·오실레이터), 발진기(LC·수정·RC·마그네트론). sources: new-electronics + intro-electronics
- Updated: concepts/digital-logic-basics.md (updated 2026-10-22; sources에 digital-electronics + digital-theory-experimentation 추가; 보충 소스 섹션 추가; Related에 [[amplifiers-analog-circuits]] 연결)
- Updated: concepts/semiconductor-devices.md (updated 2026-10-22; sources에 new-electronics + intro-electronics 추가; 보충 소스 4줄(전자공학입문 ch.2, 신전자공학 ch.1-2, Tokheim 디지털 스위칭, Levine Exp 4/17-18/SCR) 추가; Related에 [[amplifiers-analog-circuits]] 추가)
- Links: index.md entities +5 (책 4권 + morris-levine) · concepts +1 (amplifiers-analog-circuits), Total pages 265→271 (entities 110 · concepts 160 · comparisons 1), Last updated 2026-10-22
- 저자: morris-levine는 book 1권에 집중(single-book author → 임계 충족) → entity 생성. 신전자공학 4공저자(이수원·구기준·임영근·이영노)는 단발성이라 entity 미생성, 각 book entity frontmatter/본문에 이름만 기록.
- Cross-links: 4개 book entity ↔ concepts/digital-logic-basics ↔ concepts/semiconductor-devices ↔ concepts/amplifiers-analog-circuits ↔ entities/morris-levine
- 한자(CJK)/키릴 문자 확인: 새로 만든/수정한 파일 전부 grep 확인 — 한자(U+4E00-9FFF)·키릴 문자 미포함 (한국어 + 라틴 문자만).
- git commit: 미실행 (부모 에이전트가 수행)

## [2026-10-22] ingest | 회로 해석 표준 교재 1권 (electric-circuits)
- Raw: raw/books/nilson-riedel-electric-circuits.md (USB 원본 Electric_Circuits.pdf, 949p) — James W. Nilsson & Susan A. Riedel, Electric Circuits 4th ed. (Addison-Wesley, ©1992, ISBN 0-201-54987-5). pdftotext -layout 전수 추출, tesseract 재-OCR 불필요(텍스트 레이어 존재). raw SHA256: raw/books/nilson-riedel-electric-circuits.pdf.sha256.
- Created: entities/nilson-riedel-electric-circuits.md — 20장(DC 기초→R/L/C 동적 회로→정현파 정계→커플링/공진→라플라스/이전함수→푸리에→2포트) + PSpice(Design Center) 실습, 20장+946p
- Created: entities/james-w-nilsson.md — 저자 (Iowa State Univ. Emeritus) — single-book author (1권 집중)
- Links: index.md entities +2 (nilson-riedel·james-w-nilsson), Total pages 271→273 (entities 110→112 · concepts 160 · comparisons 1), Last updated 2026-10-22. laplace-transform-circuits.md의 "별도 에이전트 작업 대상" 주석 해소.
- git commit: 미실행 (부모 에이전트가 수행)

## [2026-10-25] ingest | USB 30권 배치 — 통신·전자·물리·무선공학 30권 (+ 복구 10권)
- Raw: raw/books/*.md +30 (pdftotext -layout 전수, raw total 146->176), 각 파일 sha256
- Created entities 30: stremler 3ed + sol / taub 2ed-trans + sol / digital-comm-kr / analog-digital-matlab / mobile-eng-kr / halsall 4ed / dtsf / cbe-matlab / cls-matlab / lst-3ed / sedra-3ed + sol / graphic-ii / fractal / ivcs / wavelets 4 / nr-c-2ed / hayt-5ed / halliday-2ed / pozar-sol / nilsson study-guide + sol-vol1 / leon-garcia / papoulis / oppenheim-sol
- 복구: 서브에이전트-3 공유캐시 경합으로 raw+entity 10권 삭제 -> USB PDF sha256 매칭 후 pdftotext 재추출, raw·entity 재작성 (stremler-sol·taub-sol·mobile-eng·halsall-4ed·sedra-sol·graphic-ii·hayt-5ed·halliday-2ed·nilsson x2)
- 대조: Sedra 508p PDF=원서 3판(sedra-3ed), 143p=한국역 문제풀이집(sedra-sol). Linear: 기존 2판 + 신규 3판(lst-3ed, 2단에 cross-link). Hayt=Giarrusso em-engineering과 별도. Nilsson 4ed=기존 nilson-riedel(949p) + study-guide + sol-vol1
- cross-link(서브에이전트 작성, 검증됨): sedra-3ed<->sedra-sol, lst-2ed<->lst-3ed, stremler-3ed<->sol, taub-trans<->sol, signals-oppenheim<->sol, alan-v-oppenheim->dtsf/cbe. james-w-nilsson 저자 entity에는 4ed study/sol 미링크 (book entity 상호링크로 대체)
- index.md: +30 entity 항목, Total pages 412->443 (entities 255 · concepts 186 · comparisons 1)
- git: 커밋 대기 (부모 에이전트)

## [2026-10-26] lint | 태그·분류 체계 재정비
- 진단: 허용 113개 외 283개 위반 태그 (793건, 283파일). 6개 도메인 Domain과 Tag Taxonomy 목록 불일치 발견.
- 정책: 확장 정책(정보 보존) + index 도메인 재배열 (사용자 승인).
- 파일 수정 14개: 서식 위반 태그 정규화 — `재테크`→`personal-finance`(5)·`Korea`→`korea`(3)·`IFRS`→`ifrs`(3)·`PER/PBR`→`pe/pbr`(2)·`r&d`→`innovation`(1)·`quant/trend/value investing`→하이픈화(3). 의미 없는 일반화 없음.
- SCHEMA.md `## Tag Taxonomy` 재구성: 빈도·도메인 기반으로 7개 도메인별 등록 체계 전환 (AI / Investing / Programming / Language(외국어) / Network / Engineering(공학) / Physics + Meta). 허용 태그 113→393, 코퍼스 태그 373개 **전부** SCHEMA 등록. 미등록 0. `Language` 도메인 신규 추가.
- index.md: type별 (Entities/Concepts/Comparisons) 나열을 **도메인 7개 기준** 재배열. 각 섹션에 도메인 설명 + 태그 레지스트리 + 페이지 목록. 분포: Investing 119 · Engineering 193 · Programming 49 · Language 42 · Network 17 · AI 17 · Physics 5 = **442** (index 엔트리 442건, 누락 0).
- backup: `index.md.bak-20261026` (로컬 전용, `.gitignore` `*.bak-*` 추가).
- git: 커밋·푸시 아래에서 진행.
