---
title: 10일 만에 배우는 XML (10日間で作る XML 入門教室, 원제 추측: 10日でわかる? XML 입문 교실) (raw source)
source_url: /run/media/yutae/Data/10일만에 배우는 XML.pdf
ingested: 2026-10-18
sha256: a8ed4538d8428c587669c8bfb517e55e91e7f35395ac5c41e766887c6a59b66c
---

# 10일 만에 배우는 XML (10日間で作る XML 入門教室, 원제 추측: 10日でわかる? XML 입문 교실) (raw source)

> **Note:** PDF 내장 텍스트 레이어 사용 (OCR 없음). `pdftotext` 추출. PDF는 로컬 참조용 (`raw/books/*.pdf` git-ignored).

## Book metadata
- **원저:** Yoshihiro Yamada (山田義博), SHOEISHA Co., Ltd. 2001 (일본어판)
- **한국어판:** Youngjin.Com (영진닷컴) 2002, 에릭양 에이전시 계약
- **범위:** 318p, 10일 과정: XML 기본 → XSLT(레이아웃·상세정보·고도 기법) → DOM 프로그래밍 ①② → DTD → XML Schema → 클라이언트 XML 프로그래밍(JS) → 서버 중심(동적 XSLT·CSV 변환·도서검색)
- **page count:** 318 (pdfinfo Pages)

## 장 (chapter) structure
| # | topic |
|---|-------|
| Day 0 | 오리엔테이션 (XML이란 무엇인가·기능과 특징·SGML/HTML 비교) |
| Day 1 | 배우는 XML의 기본 (Lesson 1-2: 기본·다양한 표현/작성법) |
| Day 2 | XSLT 스타일 시트로 레이아웃하기 |
| Day 3 | XSLT에너 상세 정보 표시하기 (Lesson 5 이미지와 장식 / Lesson 6 조건 분기·수치 정형) |
| Day 4 | 고도의 XSLT+α 테크닉 · DOM 프로그래밍 ①(140p) |
| Day 5-6 | DOM 프로그래밍 ② (164p) |
| Day 7 | DTD (문서 형식 선언) |
| Day 8 | XML Schema |
| Day 9 | 클라이언트 중심 XML: XML 스키마 구문 체크(L20) · 동적 정렬(L21) · 도서 검색 프로그램(L22) |
| Day 10 | 서버 중심: XSLT 동적 변환(L23) · XML→CSV 변환(L24) |

## OCR/추출 주의
- Java·ASP·PHP 연동 강조 (서문 p.3)

## Text (all 318 pages)

===== PAGE 1 =====


===== PAGE 2 =====
1 =====
●

.

.

YoungJin.

일 만에 배우는

comY

===== PAGE 3 =====
2 =====
10일 만에 배우는 XML
10H z ' 扮1了元 乙 XML 入門敎室
by Yoshihiro Yamada
Copyright (D 2001 by Yoshihiro Yamada
Original Japanese edition published by SHOEISHA Co.,Ltd
Korean translation rights arranged with SHOEISHA Co.,Ltd
through Eric Yang Agency
Korean translation copyright 樞）2002 Youngjin.Com
본 저작물의 한귁거판 저작권은 에릭양 에이전시를 통한
하 O티아 A Co.,Ltd 사와의 계약으로
한국
《거판권을 영진닷컴이 소유합니다．
저작권법에 의하여 한국 내에서 보호를 받는 저작물이므로
무단 전재l와 무단 복제를 금합니다．

저 자 : Yamada Yoshihiro
감 수 : 이오커뮤니케이션
기 획 : 해외도서개발팀
진 행 : 이수정, 신정진, 김미정
편집 디자인 = 이오커뮤니케이션
（이은정）
표지 디자인 : C&D
（이충헌）
독자님의 의견을 받습니다 이 책을 구입한 독자님은（주）
영진닷컴의 가장 중요한 비평가이자 조언가입니다．
저희 책의 장점과 문제점이 무엇인지, 어떤 책이 출판되기릎 바라는지，
책을 더욱 알차게 꾸밀 수 있는 아이디어가 있으면 팩스나 이메일, 또는 우편으로 연락주시기 바랍니다．
의견을 주실 때에는 책 제목 및 독자님의 성함과 연락처
（전화번호나 이메일）
를 꼭 남겨 주시기 바랍니다．
독자님의 의견에 대해 바로 답변을 드리고, 또 독자님의 의견을 다음 책에 충분히 반영하도록 늘 노력하겠습니다．
팩 스 : 02-2105-2205
이메일 : support@youngjin.com
우 편 : 서울시 서초구 서초동 1623-10（주）
영진닷컴 해외도서개발팀（우）
137-878

===== PAGE 4 =====
3 =====
어서 오세요！XML입니다

'XML이 도대체 뭐가좋은지 잘모르겠어7"
"
“왜 그렇게 난리지7
라는얘기를자주듣는데, 이것은당연합니다．
XML은 컴퓨터 또는 물꼐 비유되는 경우가 종종 있는데, 실제로 사용하기에 따라서 어떻게든 이용할 수 있
는 언어입니다. 반대로 그 자신은 직접적으로 어떠한 끼능
＇을 갖고 있지는 않습니다. 주위의 각종 인터페이
스, 언어(Java와ASP, PHF등）
등과 연동함으로써 비로소 XML의 생명이 부여됩니다．
이 책은 이러한 X1dL의 시작 부분에 해당하는 기본적인 XMl꾀 구문, 사용법에 대해서 중점적으로 소개하
는것을목적으로합니다. 먼저 'XML이 어떤 것인지 사용해보고싶다”, "뭐든상관없으니까내 손으로작성해
보고싶디？', 'XML이 뭔지 보고싶디
＇'라는생각을가진분들은꼭보셨으면합니다．
HTML을 아시는분은 HTML의 연장선으로XML 구문을배우는 것도 좋습니다. XML뿐만 아니라, 그 주변
을둘러싼풍부한 관련 기술 - 문서 구조를 변환하거나 스타일을 정의하는 XSLT, 문서의 동적 동작을 가능하
게 하는 DOM, 정밀한 데이터 교환에 빼놓을 수 없는 UPD, XML 스키마 등 XML을 시작함에 있어서 기본이
되는 지식을 종합적으로 설명합니다. 그리고 책의 마지막에는 이들의 기술을 총괄한 실용 예제를 소개함으로
써 XML학습의 새로운단계로나아갈수 있는 계기를제시합니다．

===== PAGE 5 =====
4 =====
머리말

어서 오세L1! XML교실에！

제0일

오리엔내아션
XML이란 무엇인가？

玔일

10

XMl－의가본
Lessoni 배우재 XML의 기본
Lesson2 XML의 다양한 표현 - 다양한 작성법

제2일

3

32
42

XSLT 스티일 시트로 레이아웃하기
Lesson3 XSLT로 요소 · 속성의 내용 표시하기
Lesson4 목록표로 출력하기
Lesson5 데이터를 정렬하여 링크 작성하기

52
66
78

===== PAGE 6 =====
5 =====
께일 XML의 기본

30 50

제2일 XSLT 스타일 시트로
레이아웃하기

加

LT

제4일 고도의 X잇－T+ α 테크닉
，宬슬

…j 제3일 X듸－T에너 상세 정보 표시하기

제3일

-ti\ ) 116

k

xs邙dP넥 싱뻬 정보 표시하기
Lesson6 이미지 표시와 문장 장식하기
Lesson7 조건 분기 · 수치 정형으로 보기좋게 나타내기

제4일

j프ㄹ의 XSLT+ α 테크닉
Lesson8 xPath 함수 사용하기
Lesson9 유지 보수성의 향상과 보다 세밀한 표시 제어하기

제5일

92
106

118
130

DOM ㅍ쿠그ㄹ卄밍 ①
LessonlO DOM을 사용하여 XML 문서 읽기
Lessonhi XML 문서에서 요소 추출하기
Lesson12 XML 문서에서 속성값 추출하기

142
148
158

===== PAGE 7 =====
6 =====
제5일 DOM 프로그래밍 ①

슈

140

1 〃
제6일 DOM 프로그래밍 ②

r

拓

C

已

戶

「164
164

졔3일 DTD
（문서 형식 선언）

' ,.∼，
, . .. .. , ㄱ.,,, .. 一.ㄱ．
셰b닐 入ML 스기UI ㅅ「쓩xI

* 1

208J

A
제6일

188

DOM11쿠1래[I깅 ②
Lesson13 요소 추출하기
Lessonl4 XML 문서에 노드 추가하기
Lesson15 XML 문서를 갱신 · 삭제하기

제7일

166
174
182

DiD（문서 형식 수塑）
Lesson16 XML 문서 안에서 DTD 작성하기
Lesson17 XML 문서 밖에서 DTD 작성하기

제8일

.

190
200

XML스키마사夔끼
Lessonl8 기본적인 XML 스키마 작성하기
Lesson19 향상된 XML 스키마 작성하기

210
224

===== PAGE 8 =====
7 =====
제9일

于t이언트 중심의 XML :ii쿠-j근松밍
Lesson20 XML- 스키마에서 XML문서의 구문 체크
Lesson21 XSLT에서 동적인 정렬 실행하기
Lesson22 도서 검색 ㅍ쿠ㄱ램 만들기

ㅈm0일

세버 중심의 XML 프로그래밍
Lesson23 XSLT를 동적으로 변환하기
Lesson24 XMㄴ파일을 csv파일로 변환하기

口m

238
248
256

268
276

侈 테스트의 해답
실력 테스트의 해답
INDEX

286
315

===== PAGE 9 =====
8 =====
오리엔테이션
조금이라도 더 빨리 xTh을 접해보고 싶다는 조급한 마음을 누르고 우선은 준비 쳬조를 해 둡시다．
XML이란도대체 무엇이며, XML을구성하는요소는무엇인지, 앞으로XML을 배우는 데 있어서 구체
적으로 무엇을학습할 것인지, 실제로 XML을 사용하기 위해 무엇이 필요한지 등에 대한 여러 가지 지식
을소개합니다．

===== PAGE 10 =====
9 =====
Hㅇ 毗4오1 포 十改乂g

===== PAGE 11 =====
10 =====
XML의 기능과 특징
XML이란 무엇이며, XML을 사용하여 얻는 장점에 대해 알아봅니다．

]

( XML이란 무엇인가？:
은 '정보기술언어' 입니다．
한마디로말하자면XIML(eXtensible Mark끄p Language）
（plaintext)
을 알고 있을 것입니다. iffivil은 평문
여러분은 I{I爪4L(HyperText Markup Language）
에 태그라불리는 명령을 삽입하여 문서를 장식하거나 구조를 표시하는 웹용마크업 언어입니다. 예를
들면，
<B>WOPD< /B>흰현ㅈ甘가창널리 보급톼0｛혔는워cll 제人f조莖트웨어입니다

태그로둘러싸인문자열을굵은 글씨로 표시해 줍니다．
라고 기술하기만 하면 브라우저는 <B）
쉽고 무엇이든 구사할 수 있는다양한 기능, 그리고 적당히 작성해도 그런대로 표시되는 간단함이 인
터넷 보급에 커다란공헌을 했다는 것은 새삼스럽게 말할 필요도 없습니다．
그러나 그와 동시에 꼭 들어맞지 않는 여러 기능들과 구문 해석의 애매함이 웹을 시스템으로 사용하
고자할때의 애로점이 되는 것도 엄연한사실입니다. 위의 한문장을 예로들어봅시다. 진한글씨로 표
라고
시된 WORD라는 단어는 인간에게 굵은 글씨라는 표면적인 사실뿐만 아니라 '뚱요한 단어구니，
추측을 가능하게 해줍니다. 문맥에 따라서는 이것이 톄ㅁr , 타이틀？이라고까지 판별할 수 있을지도
모릅니다．
그러나 컴퓨터에서는 <B〉태그로 둘러싸인 WORD는 굵은 글씨로 표시해야만 하는 문자열에 지나지
않습니다. 컴퓨터에 있어서 그것은 톄마 도아니고 타이틀？도아닌 것입니다.
그렇지만XL을 사용하면 이를다음과 같이 명확하게 그 문자열 단위의 데이터로써의 의미를 정의
할수 있게 됩니다.
<keyword>WORD< /keyword＞은 현재 가장 널리 보급되어 있는 워ㄷfl 세서 소프트웨어입니다

이 데이터가 인간과 컴퓨터 양쪽에 있어서 매우 가독성이 뛰어난 언어라는 것은 쉽게 이해할 수 있을
것입니다（즉, 이렇게 해서 표현된 정보를 실제로 보기 쉽게 나타내기 위해 XSLT라는 기술을 사용하는
데,"이에 대해서는나중에 설명하겠습니다）
.
또, 이것은문서 데이터를시스템상에서 검색할경우에 커다란 의미를갖습니다. 예를들면, 지금까
지의 표I爪4L 문서에서는 WORD라는 키워드를 포함한 문서를 검색하기 위해 문서 전체를 빠짐없이 훑

4

===== PAGE 12 =====
11 =====
오리엔테이션

어보지 않으면 안 되었습니다. 그 결과 키워드도, 아무것도 아닌 WORD
（단어）
나 PassWord 간혹
sword라는 전혀 관계없는 말의 일부인 뉴0rf 등 본래 기대와는 상당히 거리가 먼 문자열이 계속하여
검색된끝에, 마지막으로Microsoft Office의 WORD가나오게 되었습니다．
（본래 목적으로 보면 결함이라고 해도
이는 Hmm이 정보의 속성 정보를 갖지 않도록 하기 위한 결함
과언이 아닐 것입니다）
에 불과합니다. 컴퓨터에 문서의 어디를 검색해야만 하는지의 정보를 구별하기
위한 힌트를 줄수 없었기 때문에 어쩔 수 없는 일이었습니다. 그러나 이렇게 해서는 목적한 결과를 얻
기 위해 컴퓨터가 얼마만큼 불필요한 정보를 검색해야 하는지 알수 없습니다. 불필요한 정보에 정말로
필요한 정보가 파묻혀 버릴 가능성도 있습니다．
그러나XML문서에 있어서는 키워드가 컴퓨터에 인식되도록 기술됩니다. 이로써 컴퓨터는 키워드
에 목적을 압축시켜 정보를 검색할수 있게 됩니다. 그 결과 XML 문서가 보급된 세계에서 인터넷이라
는광대한 정보 공간을 하나의 광대한 지식 데이터베이스로써다룰수 있게 됩니다.
머TML과 XML의 검색성】
_
HTML 문서
0기〉10일만에 배우는 XML(lhl)

？걍

f

이걷목늑댄첵.
.
타이틀인지 알 수 없다．
，걷.

Kb)XML 샘플집〈/b)
(strong)XML 레퍼런스〈/strong)

.
///

,,

〈서명〉10일만에 배우는 ×ML(／서명）
<1장＞XML 샘플집〈/1장〉

이렇게 하면
금방 알 수 있다．

\\

//-

件L >XML 레퍼런스〈／부록）

===== PAGE 13 =====
12 =====
〔SGML/HTML과의 비교
여기에서는XI꾀 특성을 기존의 SGML(Standard Generalized Markup Language)/HTIvll과 비
교하면서 좀더 명확하게 XTh의장점을살펴 보겠습니다．
다만, 이 비교가 XML이 HTML의 차세대 언어라는 것을 의미하지는 않습니다. XML이
SGvll끄｛I丕4L의 문제 의식을 기초로 생겨난 언어라는 것은 분명하지만, XML은 단순한 웹상의 표현
언어에 머무르지 않고 보다 폭넓은 가능정을 가지고 있습니다．
■ 메타 기술 언어
（언어 정의를 기술할 수 있는 언어）
EI爪4L이 고정적인 태그 세트
（<table〉이나 <frame> 등의 정해진 태그 세트）
밖에 갖고 있지 않는 것에
비해 Xff은스스로 태그를 정의할 수 있습니다. 이로 인해 데이터가 문서의 타이틀인지, 그렇지 않으
면상품명인지를 컴퓨터가 인식할수 있게 되었습니다．
■13년의 역사를 가진 SGML의 서브 세트／인터넷 시대의 HTML을 기초로 한다
XML은 새로운 언어이면서도 SGML이라는 오랜 역사를 가진 언어 사양에 준하므로
flUnxument 乃pe Definition : 문서형 정의）
에 의한．
문서 구조를 체크하는 등매우 숙성된 사양을
갖습니다. 또I{I丕JI로 발전된 인터넷에 대한 친밀함과 경쾌함, 충실한 기술 구조 사양01vTh 스키ㅁD과
보다발전된 링크 기능
（XIJ끄k XPointer）
은XTh만이 가진특성입니다．
■ 문서 구조 정의와 문서 수식 정의의 명확한 분리
（One Source, Multi Use)

겯

은롯선01,
- vc*T
AOL1
m 섯（문서 수식 언어隱 명확히
켯，
선읜끄釀呈선堡쏀군좃與읫츠와푠신．

분리함으로써 정보의 재이용성과 전용성을 높이고 있습니다. 하나의 XML 문서
（0ne Source）
를 여러
곳에서 활執Multi Use）
하는 것입니다. 최근 HTJvIL CSS(Cascading StyleSheet）
를 이용하여 문서
장식 기능을 분리하는 시도를 해왔지만, 본래 구조와 장식의 분리가 명시되지 않았던 I{I뇨4L에 비해
XML+XSJJJ페서는 보다 기능을 명확히 구분할수 있습니다．

===== PAGE 14 =====
13 =====
'.

C

"i

EF.

!i

。1

?

7I

c1

.

ohAIj71I

_
머TML과 XML의 검색성】

여

-

.

XML

~

HTML

鬧三

각각독립되어
／흡／
있어서 알기 쉽다. ∼

(XML을 둘러싼 풍부한 주변 요소
XR의 뛰어난 기술 환경은 기술 그 자체보다는 체계적으로 분산과 집증을 철저히 구분하는 개념
에 있습니다．
분산 이란 개개의 기술이 역할 분담을 명확히 구분하고 있다는 점
（XML 문서는 데이터 본체의 기
술, XSLT는 변환 · 표시 규칙의 기술, XML 스키마는 메타 데이터의 기술, DOM은 비즈니스 플로우의
기술）
이고, '집중 이란 이 개개의 기술들 을 전부 XTh이라는 극히 간소한干칙을 중심으로 혹성 궤도
를그리듯이 명확히 쳬계화되어 있다는 점입니다．
여기에서는 이러한XML 기술을 뒷받침하는 일련의 주변 기술에 대해서 설명합니다.
■XML 문서를 변환 . 젓혓화하

XSLT) 스타일 시트

XSLT(eXtensible Sty1esh6bt Language Transformations)는 1999년 11월에 W3C(World Wide
Web Consortium）
로부터 권고된 새로운xTh 문서 변환용 언어입니다．
원래 XSLT는 일반적인 XML 문서용 스타일 시트 언어인 XSL(eXtensible Stylesheet Language) 중
에서도 xll꾀 실용적인 면을 중시한 문서 변환 부분만을 선택한 기술입니다. XSL은 XSLT 외에
RXFormatting Objects）
라는 스타일 지정 역할을 담당하는 사양으로 구성되는데, 유감스럽게도 이
Ft）
는아직 권고되지 않고 있습니다．

===== PAGE 15 =====
14 =====
，詰IE
5.x豁甚翡XvTh4- F31I XSLT-XML年 }] 11*
RP1VII2
[XSLT와 css의 기능】

QA1

XSLT에 의해 円ML로
변환된 XML 문서

i
css에 의해 세부적인
레이아웃까지 정형화된
최종적인 출력

■XML 문서를 조작하는 DOM
（즉, 요
DOMCDocument Object Mode]）이란 그 이름이 나타내는 것처럼 XML 문서에 포함된 각노드
소와속정, 텍스트등）
를 범용적으로 조작하기 위한오브젝트 모음｛도구상자）
입니다. 즉,DOM을통해
서 비로소문서 모델에 접근
（읽기 · 쓰기 등의 가공과추출）
할수 있게 됩니다．
현재, W3C에서의 표준화, 레벨업 작업이 착실히 진행되고 있고, 2000년 II월에 DOM Leve12가 권
고된후 Leve13의 검토가 진행되고 있습니다. 현 시점에서는 아직 Leve12를 실제로 지원하는 파서도 적
은상횡끼지만, 앞으로 서서히 Leve12로의 대응이 확대되리라생각됩니다．
■XSLT와 DOM의 차이
위에서 소개한XSLT도 역시 XML 문서에서 지정한노드를추출하고 가공하기 위한 언어입니다．
그렇다면 仄〕
爪d
［과 XSLT의 차이점은 무엇일까요？또, DON
［은 XSLT와 어떻게 사용하면 좋을까요？
이것은매우중요한문제입니다．
실제, XSLT와 DON
［은 매우 흡사한 역할을 갖습니다. 그러나 XSLI까 XML 문서를 정해진 규칙어］
따라 조작하는 정적인 구조라 하면. DON
［은 XML 문서와 XSLT 스타일 시트를 동적으로 연결하거나
（예를 들면, 동일 데이터를 목록표 형식으로 나타내거나, 간단한 표 형식으로 제시하는 등）편집·가공

4

===== PAGE 16 =====
15 =====
오리엔테이션

하기 위한동적인 구조입니다．
ㅘ작성도 번거럽고 어떤 장점이 있는지
Xll과XSLT에만국한시킨다면 "XML이 오히려 HI爪4I」
알수 없디？'라는 생각을 갖게 될지도 모릅니다. 그러나 이 DOM을 배움으로써 XML과XSLT를 동적으
로 연결하는 그 유연성과 간단하고 쉬운 조작을 가능케 하는 인터페이스가 ffl

에서는 오히려 어렵

다는사실을 실감할수 있습니다．
또 이 책의 후반에서는 XSLT와 仄〕
M의 상호 보완적 기술 연동 테크닉뿐만 아니라, '뵤렇다면 실제
로 이러한 DOM 프로그래밍이 어떠한상황에서 사용되고 있는가'하는 실용적인 예를들어 소개하기로
합니다. XML을 우리의 생활에 연결지음으로써 단순히 기술적인 노하우의 습득에 머무르지 않고 실용
적인 지식으로까지 적용할수 있으면합니다.

■DTD와 타당
（Valid）
한 XML
ffl ll의연장선상에 있는 기술로서 말할때, XML이라고 하면표시 형식의 언어라고 오해하는 경향
이 있습니다. 그러나 XML의 유연하고 중성적인
（환경에 속박되지 않는）특성은 오히려 다른 플랫폼간
의 데이터 교환에 적당합니다．
태그를자유롭게 확장할수 있고구조 변경에도 강한XML은종래의 CSV(Comma Separated Value
의 중성적인 특성을 이어가면서 보다고도
: 쉼표분리 <b와皿V(Tab Delimited Value'; 태그 분류 값）
로, 보다유연한데이터 교환용도로사용할수도 있습니다．
그러나 XML의 자유로움은 생각지 못한 함정이 될수 있습니다．
X Th에 대한 각광은 예전 RDB(1굿e1ationa DataBase : 관계형 데이터베이스）
가 등장했을 때와 아주
비슷합니다. RDB는 열과 행으로 구성되는 테이블이라는 매우 단순한 개념을 조합하여 데이터를 간단
히 저장할 수 있다는 점 때문에 급속히 보급되었습니다. 그러나 그 간소함 때문에 유사한 의미를 가진
테이블이 정리되지 않은 채로 난립하여 데이터의 일원적인 교환을 어렵게하는 것도 사실입니다. 테이
블끼리의 호환성을 유지하기 위해 테이블 사이에 데이터 교환용 중간 테이블을 삽입하고, 테이블끼리

송

===== PAGE 17 =====
16 =====
의 관련이 점점 복잡해지는 과정은 악순환의 연속이었다고도할수 있습니다．
물론, 이 사실이 RDB의 공적을 부정하지는 않습니다. 그러나 xTh이 앞으로 실제 시스템에 투입되
는과정에 있어서의 좋은교훈인 것입니다．
xTh은I{I丕江I과 마찬가지로 마크업 언어이고, 초보자라도 데이터를 기술하는데 그다지 어려움은
없습니다. 또 ITI丕JI과 달리 자유롭게 태그를 정할 수 있기 때문에 개개인이 구속되어야만 하는 일이
적다고 할수 있습니다. 그러나 엄밀하게 비즈니스 환경에 xTh을 채택한 경우에는 간단함과용이함이
잘맞지 않는 경우가 있습니다. 예를들어 XML로만든 주문서를 생각해봅시다.
동일한주문 번호와고객 번호, 상품번호, 개수등을나타내는데 다음과같은 시스템이 있거나，
<order id="abc-OOO " customerlD= "00001"productslD="xyz-999" quantity="2" I>

다음과 같이 나타내는 시스템이 있다고 합시다．
<order>
<id>abc-000< /id>
<customerlD>0 0001< /customerlD>
<productslD>xyz-999< /productslD>
<quaritity>2< /quantity>
</order>

내용은 긷아도 시스템이 이젓을 해독하기 위해서는 2개의 프로그램이 작성되고, 포맷을 변환하기 위
한XSLT를갖추어야합니다. 이것이
<ocir oID="abc-OOO" cID="00001" pID='xyz-999' qty="2" I>

와같이 요소명, 속성명이 달라지거나
<order id="abc-OOO " customerlD= "OOOOl"
productsID= "xyz-999 " quantity= "2 " mexno='comment " I>

와같이 지정 이외의 요소, 속성이 추가된 경우는작성 방법이 복잡해집니다．
그러나 Well-Formed
（정형식）
이라 불리는 XMl의 규칙에 있어서는 위의 모든 것이 올바른 XML입
니다. 따라서 하나의 특정 데이터의 교환에 있어서는 "이 형식만 올바르디？'라는 규칙을 별도로 준비해
야할필요성이 있습니다. 이것이 lJlllXDocument吟pe Defmition : 문서형 선언）
의 역할입니다．
urn는 그 이름대로 한 문서 중에 기술할 수 있는 요소, 속성의 종류, 구조 관계를 정의하기 위한 문
서입니다. XML 파서는 종래 XMIL1.O에서 지정되어 있는 구문 干칙 외에 개별적으로 준비된 UfD를
참조하여 XML 문서가올바른지의 여부를 판정합니다.

===== PAGE 18 =====
17 =====
오리엔테이션

XML 본래의 구문과 urn의 양쪽에 따르는 XML 문서를 'Well-Formed XML' 과 구별하는 의미에
서 'Valid XML'이라부릅니다．

口口9 口긍口

_
IDTD의 필요성】

尸크m --n

-

.--

4∼

1■

■

p.

올바르지 않은 ×ML 데이터
여기서는 손상된
데이터가 흐름. 이
것을 알 수 없다．

-

올바르지 않은 XML 데이터

여기서는 올바르지
않은 데이터를
DTD가 차단해 주
므로 간단하다．

■DID의 결점 그리고 XML 스키마의 등장
그러나urn에는근본적으로실제적 사용에 있어서 한계가 있었습니다· 그것" I
1 j츠쁘－
XML스킨마기등장힌껫코쁘〕
입니다．아래 urn의 결점이라고도할수 있는포인트와그것이 XML
스키마가로 어떻게 개선되었는지 설명합니다．
(1) DTD는 XML 구문과는 다른 형식으로 기술된다
< 므ELEMENT books (owner, book+ 》>
< !ELEMENT owner (#PCDATA) >
<IELEMENT book (name, author,category) >

===== PAGE 19 =====
18 =====
이것은 D1J의 일부입니다. 이것을 봐도 XML과 구문 규칙이 전혀 다르다는 것을 알 수 있습
니다．
즉, Valid XML을 기술함에 있어서 XML 구문 외어］Un) 구문 규칙을 배워야합니다. 또, 파서와
기타 처리 프로그램에서도 XML을 읽어내는 장치 외에 UIiD를 읽어내기 위한 별도의 장치를 준비
해야합니다. 이는 개발시 번잡할뿐만 아니라 처리시에도 아주복잡합니다．
그러나XML스키마는XML의 구문 구칙에 따라서 기술되는XML문서입니다.
<?xml version="1.0" encoding="EUC-F珊' ?>
<xsd: " schema xi皿ns:xsd='http: //www.w3 .org/2001/XMLschema" >
<xsd:element name='title

" type= 'xsd:string"/>

</xsd: schema>

위에 기술한 것은 기본적인 XML 스키마의 예이지만, XML 문서 자체이기 때문에 UPD에 비하
면비교적 친근감 있게 여겨집니다．
이러한구문 子칙의 일원성은 새로 배우는데 있어서뿐만 아니라, 시스템적인 처리에 있어서두
매우유용합니다．
【자AL 스키마는 )(ML 문서】
_

샅，
－스
'-

7 _

ㅓ

XML문서

DTD는 ×ML과는 전혀 다르거1
만들어졌기 때문에 읽기 어렵다．

XML 문서와 XML 스키마는 같은
요령으로 읽는다．

DTD
XML 스키마

송

===== PAGE 20 =====
19 =====
오리엔테이션

(2) DTD 데이터형을 갖지 않는다
원래 DTD는 이전 XML 시대－SGML 시대에 개발된 규격입니다. SGIvll - XtL이나 R ll과
마찬가지로문서 구조를표현하기 위한마크업 언어이지만, 이 시대에는문서가곧 워드프로세서로
다뤄지는산문적인문서
（우리들에게 가장 친숙慤였습니다．
이 시대의 산물인Un〕
는문서의 구조관계를나타낼수는 있어도, 그안에서 표현되는 데이터형의
개념은희박합니다. 데이터형이라고하면 겨우＃FCDATA라불리는문자열형을나타낼뿐입니다．
한편, xML 시대인 오늘날에는문서라고 하면산문적인 일반문서뿐만 아니라 데이터베이스적인
다양한 데이터의 집합체도 포함합니다. 이러한 문서는 포함된 데이터가 수치인지 날짜인지, 또는
수치라고해도 정수인지 음수인지, 여러 가지 엄밀한정의가요구됩니다．
DIL는 이것을 전부 문자열형
（#RDAT.A）
으로만나타냅니다．
그러나XML스키마는 기본데이터형으로서 문자열형, 수치형, 날짜형, 논리형을 비롯해 데이터
베이스로 다룰 수 있는 일련의 형태를 미리 준비함과 동시에 개별적으로 데이터형을 정의할 수 있
습니다. 즉, 동일한문자형이라도문자열 길이는 몇 자리 이상인지 몇자리 이하인지, 수치형이라면
정수인지 소수인지, 양수인지 음수인지, 그 때 그 때의 용도에 맞춰서 변동하는상세한 정의를 엄밀
하게 표현할수 있는 것입니다．
이것만 보더라도 문서 교환에서 데이터 교환으로 바뀐 현재의 데이터 처리 요구를만족시키는 것
이 XML 스키마밖에 없다는 것을 알수 있욜 것입니다．
【XML 스키마는 데이터형을 표현할 수 있다】
_

`-,

一
。

륜

보내는 데이터는 문자열뿐．
이래서는 데이터를 정리할 수 없다．

여러 가지 데이터형의
정보가 보내진다．

True/False

19

=

.

궉－

ABC · . ·

===== PAGE 21 =====
20 =====
(3) DTD는 이름 공긴을 지원하지 않는다
XML을 지원하는 또 하나의 중요한 개념으로 이름 공간이 있습니다. 이름 공간은 2개의 문서 정
의를 하나의 문서 내에서 다룰 경우에 사용되는매우중요한 개념입니다．
예를 들어, 서적 XML에서는 <name> 요소는 도서명을 나타내고 있고, 저자 XML에서는
<name> 요소가 저자명을나타내고 있다고합시다. 이를동일한XML 문서 내에 통합한 경우, 다른
의미를 가진 <name) 요소가 함께 존재하게 되어 매우 혼란해집니다. 처음부터 XL을 채용한 것
" 뗘의냇jl올엄밀히 정의하고시스템적으로자동처리할수있도록
도HTML에서는 'ㅐ"ㅐ했던 "∥
하기 위해서였습니다. 그러나 이제는 뵤소명만으로는 올바르게 데이터 내용을 표시할 수 없게 된
것입니다.
（속
이런 이유로 이름 공간이 등장했습니다. 이름 공간은 이렇게 한 가지 뜻으로 되지 않는 요소
성）
명 앞에 접두사를달아 이것이 어느문서 干칙에 따르고 있는지를 정하기 위한규격입니다．
예를 들어, 저자명을 나타내는 <name> 요소는 <author.name＞으로 하고, 도서명을 나타내는
<name> -소는 <book.name＞으로 정하면 양자의 이름이 하나의 XML 문서 내에서 하나의 뜻이
되어 시스템적으로도 잉카를 판별할수 있게 됩니다.
그러나 SGML 시대에 있어서는 여러 가지 문서형 선언을 통함하여 전용하는 개념은 희박했습니
다. 당연히 패
［D에도 이름 공간을 생각하지 못했습니다. X\Th의 중요한 개념에 대응할 수 없다는
것 자체가 】:ii'i）
의 근본적인 한계를 그대로 드러낸다고 할 수 있습니다. 한편 XML 스키마는 XTh
문서 이므로 이름공간을표현할수 있습니다．
【이름 毓l卜에 의한 구볍】
_

===== PAGE 22 =====
21 =====
오리엔테이션

C이 책을 학습함에 있어서
이 책을 이용하기 위해 먼저 필요한 것은XML을 지원하는브라우저 Internet Explorer(IE) 5.x 이상
과MsXTh입니다. 皿 5.x는각자준비하리라 생각하고, 여기에서는 MSXIvTh3의 설치 방법에 대해서
만소개하기로합니다．
I MSXML3의 설치 방법
MsXMI은 JE 5.x 이상에 표준으로 장착되어 있는xTh 파서의 일종입니다．
파서란 xTh 문서를 해석하고 표시와 조작을 제어하기 위한 모듈로, XML 애플리케이션을 다룰 경
우 가장 기본이 되는 부분의 프로그램입니다. 종래 MSXML 파서는 IE 5.x의 한 모듈로 위치했지만，
2000년 II월에 독립한 프로그램 MSXML3
버전업 · 리소스 되었습니다. 앞으로 파서의 독립성에
대한 개발작업이 더욱충실히 진행되리라 생각합니다.
MSXIvIL(nisxm13sp2setupKor.exe) 및 인스톨러
（xmlinst.exe＞는 아래 사이트에서 다운로드할수 있
으며 부록
（D-ROM에도수록되어 있습니다．
http:IImsdn.microsoft .com/downloads/default.asp?url= /downloads/topic .asp?URL=/
msdn-fi1es/028/ OOO/072/topic. an1

따亡α〕 ！크o

모＞凹

a가1기凶

도구쎄u)

도．
1uP

i玄 dH. 孕
＝소QㅐF∼
力,

.PtI

.

汕 哺기。
g,

니mc」
d d,U∼｀
,
르크工i〕璉i크.

*

1

驪. m'

HSXML Part.
rm 勵

』硼” m 3 . m* n·.1tm．
』t'
口 H$X∥i. ,1 C* F* "kh 'm`n〃
u 째｀mf 二m出｀왜
＇H
□띠 一 크. 日
. 陌m 1 . C.̀) '11口1m`Lntm1硼 口X
ㅁ 녔｀,, v'` m 2三 .叱너n1"'1．
硼
ㅁ 치｀vd너11t.m 1m
□ 》m뻐11·m m甘at* H. J1 r띠
ㅁ 1n.mm.「目
＇km 功d, 佃 v1*dm1` ,
ㅁ "S一 mte' 3刀 5옭，
K1 p鷺* ` m轍
口 니m버
＇1; m`KY C머너b〃mㅐ
m U. 1'
【그 "5m 3 . P〃·r 니xH..d v1nm`
回 닛立
u M日X,t , . 5P` m치批d1月口』
H`t *
口 "s，
川 P겸，
' 크 . RIma1·
C」뵤1片 X5.《몌거．
뱃r
口｀拓노1在 2 5 5n`
u H＄小｀51, 3 . 山1h小1
□ 지吼 5taMa寸1

- 驪괌 m뇨亡，
.「氓벼

시R ｀ㄲ媤ㄱ시emmnnl1:7그11F. 一
0eNt

,

be . .fltfl

, 3. 0 S. rvic.

ParJr2

. .bOfl

」 尸미i
VMS

'SI

.

5r.S*

면괘 .

SM ·

Meleooo

`dn1 `1吼 '1rt1' (m5X戚J J .

饗壅蓼，

！,' ..；쓰，
重
" 三＝芬．
發：:1．
‘二
烈뼙꽈，
빴뇬巴巴쌨：
旣；
斗뱌1,J.
珊l尺欒楡烈：烈：l"
`．名麥，

C1 여기를클릭

I

.

·뺨따 변勵t)

"

여기를클릭하여 다운．
로드한다，

보기
【刃

1겨솽거山 도구q)

도8m·

a. a。수

iI1 1싫거 훽」i긔 翕 l立 J1M5

주소邸F. h心／
『，
「－ 〕｀Dh口〕n/d.*ㅃad丘dma나숴1길p, h/d0翩．
d
y1뇨什.mt ‘드‘기ㅐL ／巾흖d.새m，
心斗qL幻쿄，
拈口〔 ,m

“渺r,SM「

u5ㅂ〔프亘〕.口α야小 - 마
＇·．. 7 」h스 · J굼1·보 · ' 스포a 기코月 . 立g

】m

띠印 0m ㄴ·청뀀
□ 나Crm1nh M긔夔뜁m' 旺r
ㅁ M日XNL Pm1' 3 . 叩2 口1ma,.
ㅁ H6,HL ㅓ . PT"
나 H目XHL 〕. Hbrq·－`m ．」1
《h引川，
t口
【J H5X1m 3 ㅁ 5P1 ‘此 Fm 口1曲n'*U呻
口 玳吼 佃 1＾흴艸1 듸乂
u 5mX1m` ㅋ 0 口ㅜM
口 "sx'1 크 . ㄷ샙 F빼e 由1小＄tnl그ㄴt
［叭 mC
u X＇吐 드긔겨 VH`
｀기 2 ` .1乂바m크ㄲ꽈at円n

0

여기를클릭 ,

.

여기를 클릭하여
다운로드 한다．

xmllnet. .x日 Replace Mode T떼～

니 Jn`mm ＝비）
｀緘·
『 口빼쩍s n卄 Y
. H드X卜
（ P〃
｀' ｀댜 5日m(a P
u mmTT口 더my 二On寸口rJr日tmh
ㅁ H$x麗 ] . P.r5目
＇ Lnc汕2月d `
田 x일
ㅁ H5X驪 3 . 드Pl mf'1m山1·

昌橓，
發三三r-

^dd1". n거 Inf
（》
＇｀ㄲd1如n

-

-ii

군α ·

i尸며m

인i 뺨

===== PAGE 23 =====
22 =====
(1) MSXML3을 사이드 바이 사이드 모드에서 설치합니다
사이드 바이 사이드 모드는 기존 MSML 파서의 기능을 치환하지 않습니다. 3번째 설치 단계의 모
듈이 레지스트리에 등록되기만 합니다．
1 msxm]3sp2setupKor.exe를더블클릭하고인스톨러를시작한다．
설치 환영 화면이 표시되면[Next〕버튼을클릭한다．

죤登

Welcome to the Microsoft XML Parser
SetuD Wizard
재eSetup Wizard will inst히I Microsoft 4eIL Parser
on your computer. - Click Neot to continue or
Canc이 to e낚ntie Setup Wizard.

「販莖芝：: ＝쯔쯔느幻

여기를 클릭

2 사용동의 화면에서 [I accept the terms in the License Agreement]-- 선택하
고[Next] 버튼을클릭한다．
End-User License Agreemem

e兮

F기ease read the followiny license uyreernent carefully

三l

）USER LICENSE AGREEMENT
MICROSOFT CORPORATION nㅔ

IMPORTANT-READ CAREFULLY: This End-User License
Agreement I "EULA"I is a legal aqreenient between you
(eother an ㅗndiv1dual or a single ant1Cy) m,d
Microsoft Corporation for the 표icrosoft software
《끄nputer
duc℃ 그．deZ1tㅍltj. ed 出Dove, ahj.oh 』．t1cㅗudes c
p
mnn1月r尸d m.d1月' '" ' 1 nr-ㅐ
ㅋnf汁；可”rP ㅐ1們 ,rn`7 ` ㄲr므 】】］d尸 月，

=j

M1cr.B.fL xHL Par8er

( ！取匯.tthiterri iAthe1j醵莖E,reement

.

여기를클릭

.

여기를클릭

(- I d（〕notaccept the torms in the License Agreement

<back 1 Neet> ;

口ncc1

===== PAGE 24 =====
23 =====
오리엔테이션

3 사용자명, 조직명을입력한다．
灌Mieronoft ;4ofL F'OH

뜨닙L

口

ㅁ

Customer Inlormation
F기ease enter iour customer information

User Name

障n匐

0

Qrganizatiun

이름을입력

沁

<Uack - Neot> 1,

1

'，
一1

I

●

조직명 입력

.

여기를클릭

4 [Inst川I] 버튼을클릭한다．
二 tiicrosoft XML Pai r-

x

Ready to Install
The Setup WI2ard is ready to be卽n the installation

Click
。f
y。
ur
Install
to begin
installation.
If you want
to review
orthe
change
any
Installati。
n the
ettirigs,
click Back.
Cancel
t。
evil
wizard.
Click

』느
＇
<Back ILJ! rT
ㅈ쩍

肛

，ㅗ
'=
纛ncei L

여기를 클릭

===== PAGE 25 =====
24 =====
5 모듈의 복사가 정상적으로 종료되면[Friish] 버튼을클릭하여 설치를종료한다．
口

曙Microscil cML Pairer Senjp

죤台

Completing the Microsoft X1川．
- Parser
Setup Wizard
Click the Finish button to exit the Setup Wizard.

여기를 클릭

(2) MSXM口을 리플레이스 모드에서 설치한다
본격적으로 MSXML3을 사용하려면 리플레이스 모드에서 설치해야 합니다. 이것은 설치하는
MSXML3을 기존MsXMI과 치환하여 메인XML 파서로서 등록하는작업입니다．
1 xmlinst.exe를 더블 클릭하고 파일을 'b:\xml' 폴더
（또는 'd:\xml' 등 임의）
에 압축을
푼다．

To unzip al lIes in>&L1NST.EXE to (he specified
folder prezo the Unzip button

Wrn

Purr

Clooo

Unzip To Folder.

irrzip

P Overwrite Files Without Prompting

About
H elp

ㅁ Nico Mok Computing. Inc.

mwwwinzip corn

4

ip

-

압축을 풀 폴더를 입
력하고 [UnZip을 클
릭한다．

===== PAGE 26 =====
25 =====
오리엔테이션

브
To unzip 베 tiles in)슈壯水ST.EXE to me specified
folder press me Unzip button
Run！
世iriZi

Unzip To트older:

C뇨se

-J

卜크sm

WiriZip Self-Et<tractor驪i

r7 Uverwrit

압축 풀기가 완료되
었음을 알리는 대화
상자가 퐈 된다．

2 file(s) unzipped successfully

About
닌히p

2 file(s) unzipped successfully

WinZip

Run

Unzip To Folder

-

Unzip

To unzip 눼 tiles in Xtvl니NSTEXE to the specitied
folder press the Unzip button.

-

-

close

「7 qverwrite Files Without Prompting

About

-

쑈비已
2 tile(s) unzipped zuccesufully

2DOS 프롬프트에서 기존 MSXIvTh 파서를 언인스톨한다．
c:WxmlWxmlinst

-u

口
c:Vi LF 에 입력」

Hicrosoft(K) Hindows 98
α)Copyri ht Microsoft Corp ' *181--1999.
c＝臂LJHID0Hs>cd毋
C:臂＞c:蠟xn1枷mIinst -u

===== PAGE 27 =====
26 =====
[ 먼인스톨이 완료

Microsoft(H) 1hodows 98
(C比叩yright Microsoft Corp 1901d"9.
c＝嫩nHDOWS>cd눕
ㄷ：蠟>cd:甘xnlxnl inst -u
매개번수가 L 무 많습니다
:＝蠟＞c:jxml甘oniiUst

-U

U

出able
ren。
ved 。ld
tod i
scan,ewprocess
dli ,
e。to
tr민，
:, "" "'""" "
:＝甘＞

DOS 프롬프트에서 MSXML 파서3을 레지스트리에 등록한다．
regsvr32 msan13.dll

[ J

c:Yvi E4에 입콕그

槻
자동

二j 뾰二」
彗
「倒 宣1万 스」

Hicrosoft(B) Windows 98
(C)cop9ri妙1t Microsoft Corp 錚al-i, ,,C :枷I새VOWS>cdW
C:甘>c:쌓xniWuniinst -U

c＝甘MmDOWS> cd甘

- 등록완료

C:甘> w:쩍windows甘5y5te畔rngsorj 2 c :9, iodowsfsyst.r,5自oo,sI3.d1i

-J

.＝甘＞

,jH) 0llFlegisterServer in c:W*icdowsWs,stem￦msomJ3'dli succeeded
확인

l

===== PAGE 28 =====
27 =====
오리엔테이션

'코맨드 또는 파일명이 다릅니다' 라는 에러가 표시되는 경우는 'regsvr32.exe' 와 'msxml3.베' 앞에 각각
'c:\windows\system\' 을 추가하기 바랍니다
（단 'c:\windows\system\’의 부분은 'regsvr32.exe' , 'msxmI3.dII'

system\msxml3

.dll

C:

\windows\

system\

\windows\

C:

regsvr32

의 저장 위치에 따라서 다릅니다．

4 MSXML파서3을 리플레스모드에서 설치한다．
C: WxmlWxmlinst ｛교）
礪

幽F

c:W> 다음에 입력

ㅍ」 니 回上크j則

'4]crosoft
（ㅐ）1
'ind(）
헙，5 98
(C)Copyri4ht Hicrosoft Corp 19聊1 作90.
1나00卄S>cdl
亡二，
c：씰"no小'ws*sy St tfl蠟regsor32 c＝썹wondnus뭏5ys (eMteesxno13. d L【
c :쌉>c 布ont쫠0151inst
(ooa(de to scan process tabIc, re小iires llnoHl
USl凹 "C:鬱l1HII0WS甘SYST다I竹SXML3.0LL'. ∼
r이snoed 0hj dl l entr len
re驪istored dl灌 for " ' reqistry entrle5C 描＞

]
이상으로 설치가종료되었습니다．
또한, 만일 MSXML3을 설치한 후 시스템이 이싱해지거나 다른 XML 애플리케이션에 오류가 발생
할 경우는
c:W 1Wa1inst珽：
L
로 MSXTh 파서3을 제거할수 있습니다．

匈

===== PAGE 29 =====
28 =====
(CD-ROM을 사용하기 전에기．
CD-ROM에 관해서
CD-ROM에는 ''10일 만에 배우는 XML펙 본문 내에서 설명하는 각 Lesson의 완성 파일과문서
작성에 필요한 이미지 등이 들어 있습니다．
CD-ROM의 사용법
하드디스크에 폴더를 복사하여 사용하시기 바랍니다. CD-ROM에서 복사한 파일에는 읽기 전용
속정이 설정되어 있으므로 복사한후에는 읽기 전용속성을 해제합니다．
이 책에 수록된 예제는 C:WDt-D10가지의 임의의 폴더를만들어 저장하고 있습니다．
CD-ROM 테스트 환경에 관해서
CD-ROM은아래 환경에서 정상적으로 작동됨을확인했습니다．
' Internet Explorer 5.5+ Windows 98
' Internet Explorer 5.5/6.0 + Windows 2000

===== PAGE 30 =====
29 =====
Go to XML

===== PAGE 31 =====
30 =====
0

Lesson 1 ∼ Lesson 2

XML의 기본
XMI은 HThII과마찬가지로 태그 삽입형 마크업 언어입니다. HI爪4L을 어느 정도 작성해 봤다면 XML
은대부분 직감적으로 이해할수 있을 것입니다．
제 1일째인 오늘은 xML을 작성할 때 주의할 점과 꼭 알아두어야 할 포인트를 l{I刪I과 비교하면서 확
인해 보도록 하겠습니다．

===== PAGE 32 =====
31 =====
오늘 공부할 내용들
배우ㅈㅐ XML의 기본
XML의 다양한 표현－ 다양한 작성법

===== PAGE 33 =====
32 =====
배우자！XML의 기본
간단한 XML 문서를 작성해 봅니다．

학습 내용 미리 보기
bOok:

.!m1

D
@XML

파일
（E)

[4]- 臼

Less。
n1

（y)
편집（트） 보기

긷뒤로 …

（A)
즐겨찾기

도구
（I)

（H)
도움말

J 多
J 크 소 괴검색 上」즐겨찾기 汐미디머 -j 心，

<?xml version="l,U" encoding= 'EUC-KR" stand棚one="yes1' ?>
<boc外(5>
一<book isbn=1'ISBN89-314-1742-x">
<name>HTML 디자민 HI주얼 가미드＜/name>
<author>C.I.S</author>
<categorv>ㅐML</category>
<pnce>118(m</price>
<publish＞멈진닷컴＜/publish>
<pDate>2001-06-llc/ pDate>
</book>
- <book isbn="ISBN89-314-1978-3>
<name>ASP 사전</name>
<author＞니시자와 나오키＜/author>
<category>ASP</category>
cprice>15000</price>
<publish＞염진닷컴＜/publish>
cpDate>2001-11-30</pDate>
c/book>
c/books>

료

…

堪，
LH 컴퓨터

隧ML문서틀인터넷 익스플로러에서 실행힌빠ㅣ

Key Point
우선 소스 코드 그대로 입력하여 결과를 확인해 보기 바랍니다．
단순한 타이핑 작업이라고 생각될지도 모르지만 처음에는 생각지도 못한 실수를 하게 됩니다. 사실，
그 실수 하나 하나가 HTML에서는 애매하게 간과되었으나 XML에서는 정확해야 합니다. 단순한 타
이핑이라고 소홀히 생각하지 말고 집중해서 입력하기 바랍니다．

0

===== PAGE 34 =====
33 =====
제1일 XML의 기본

]

메모장으로새문서를열어리스트의코드를그대로입력한다．
리스트 : books.xm!
<?xr口．version="1.0" encoding= "EUC-KR'' standalone ="yes ' ?>
<books>
<book isbn="ISBN89-314-1742-x'>
<name>HTN1』 디자인 비주얼 가이드＜/nane>
<author>C .1. S</author>
<category>HTML</categorj>
<price>11800< /price>
<publish＞영진닷컴＜/publish>
<pDate>2001-06-11</pDate>
</b00k>
<book isbn='ISBN89-314-1978-3">
<name>ASP 사전＜/rLa1Be>
<author＞니시자와 나오키＜Iauthor>
<category>ASP< /category>
<price>15000</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-11-30</pDate>
</book>
</books>
핸버ㅎ륵 매기치 안으 핸으

Iaiec1 I H--- "' ' ' -- -'된列
'므로실제로입력할때는앞행에 ' 뻐Ai:1력합니如
'하동일）
·
ㅣ 「「「「「「「“「 1 ' 떤' 昭으로塾m

입력 후[Dl] 폴더에 books.xml이라는 이름으로 저장한다．
위치(j):

1」미

=l 到 到 貸l區回
.

파일 DI름(N):

books :omll

따일 형식江）

脾스트 문서

취∼

-

이름을입력

.

여기를클릭

===== PAGE 35 =====
34 =====
[I川 폴더의 bookaxml를 실행한다．
Cheek
恥4盼甲立砒

XML 문서의 확장자는
XML문서의 경우확장자는 '.x끄寸 로 합니다．

oooks. anr 을 실행하면 익스플로러에 트리 구조로 전개된 화면이 표시됩니다．

1 XML의 기본적인 구성 요소
XML문서는요소와속성의 두부분으로구성되어 있습니다．
요소는 태그라 불리는 <xJ〉∼</xx）
와 같은 문자열로 둘러싸인 부분을 가리키며 그 자체로 독립
된하나의 정보를 나타냅니다．
종료 태그

＜요소명＞

(／요소명）

속성은태그 내에 똑성명＝속정값과같은형식으로작성되며, 요소가나타내는정보에 대한부
수적인 정보를 포함합니다. 태그 내에는 여러 개의 속성을 기술할 수 있습니다
《예제 데이터의 속성
명으로 사용되고 있는 isbn(Internetional Standard Book Number）
은각책의II〕
번호와같은 것으
로 xfl가는관계없습니다）
.
〈요소명 속성명＝
『속성값‘ …〉임의의 데이터〈／요소영〉

요소명, 속성명은 원칙적으로는 자유롭게 정할 수 있지만
（XML이 확장성이 있기
（eXtensible)'
때문입니다）
, 사용할수 있는문자에는약간의 제약이 있습니다．

－一

다음의 표를 참고하시기 바랍니다．

;

iik ·

선두 문자로 사용할 수 있는 문자

（－》
영문자, 콜론《：), 언더바

2번째 문자 이후에 사용할 수 있는 문자

（.), 하이픈
（-)
선두 문자로 사용되는 문자, 숫자, 피리어드

위치에 관계없이 사용할 수 없는 문자

전각 영문자, 전각 숫자

===== PAGE 36 =====
35 =====
`-'

XML을 구성하는 요소와 속성 같은 구성 요소들을 일반적으로 노드라고 합니다. 요소 노드와 속성 노드 외에 처리
명령 노드, 실체 참조 노드, 주석 노드와 텍스트 노드 등이 있습니다．

,: XML문서임을 선언힌다
)ilJ문서에서는 1행에 <?xi〕
l

9）
를 선언하도록 권장되고 있습니다. XML 선언이 필수는

아니지만, 앞으로XML의 버전이 증가할 경우 호환성을 위해 습관적으로작성하는 것이 좋습니다．
<?xml version= "1.0" encothng='EUC-I1t' standalone="yes" ?>

문자 코드

버전 정보

L-

DTD*
DTDJ,'01

rI월

[F

藿

n。
yes：
: 2I

0I

외부 DTD의 참조 여부

(1) version 속성
刀，
4L의 버전
（현재는 LU）
을 선언합니다. XML 선언 자체는 임의적이지만xML 선언을 기술한 경
우에는반드시 version 속성을 작성해야만합니다．
(2) encoding 속성
파일 내의 문자 코드를 나타냅니다. 문자 코드에는 EUC-KR, UTF-8, UTF-16등을 지정할 수
있습니다．
디폴트는 XML 사양으로 권장되는 Unicode(UTF-8, UTF-16）
이며 이 문자 코드를 사용하는 경
우에는 encoding 속성을 생략할 수 있습니다. 그러나 그 이외의 코드를 채택할 경우에는 encoding
속성은 필수가 되며, 생략한 경우는 에러가 발생합니다. 또 선언된 문자 코드와 실제로 XML 문서
내에서 사용되고 있는 문자 코드가다른 경우에도 에러가발생합니다.
이 책에서는Windows 환경에서 한글구현을 위해 FXJC-KR 코드를 사용합니다.

自

===== PAGE 37 =====
36 =====
Uncode
（유니 코드）
는 Unicode Consortiumi게서 정해진 국제적인 문자 코드 체계입니다. Windows와 Java의 내
부 코드로 채택되는 등 사실상 표준
《defacto standard)으로 급속히 보급되고 있습니다．

를 읽어들일지의 여부를 지정합니다
외부 DTD(Document 凸pe Definition : 문서 형식 선언）
(DTD에 대해서는 제 7일에서 설명합니디）
. standalone 속정을 捻？로 했을 경우 MSXIVThCzsual
은 외부에
Bask과 Visual C++ 등 Java 이외의 마이ㅋ로431ㅌ사의 개발 환경에사 지원되는 파서）
존재하는 문서형 선언을 무시합니다. firE는 XML 문서의 구조와 제약 조건을 나타내는 매우 중요
가 필요하지 않을 경우 standalone
한 파일이지만 XML 문서에 있어서 필수는 아닙니다. 외부 fin）
속성을yes로 해둠으로써 읽어들이는 시간을줄일수 있습니다．
에 대해서는반드시 읽어들이므로 주의하기 바랍니다．
단, XML 본문 내에 기술된내부 n［工）
●STEP UP! ●
처리 명령
(?^7?＞로 툴러싸인 내욧은 OJdF적으로「 I(Processina Instruction ; 처리 명렇）
로 요죄ㅘ 속컫쿄과는 섬질이 약간 다릅
니다. 처리 명령은 그 이름처럼 처리 애플리케이션
（한 예로 XM[：을 처리하는 XML 파서, 브라우저입니다）
에 대한 XML
문서의 명령을 표시하는 것입니다．
자신이 작성한 애플리케이션에 이 처리 명령을 삽입하여 데이터를 전달할 수 있습니다, 그러나 요소와 속성을 사용해
서 데이터를 전달할 수 있으므로, 굳이 형식이 다른 처리 명령을 사용함으로써 얻는 효과는 거의 없습니다. 일반적으로
여기에서 소개하고 있는 XML 선언이나 스타일 시트와 관련된 <?xml-stylesheet?) 둥 극히 한정된 범위에서만 사용
됩니다.

를 갖는다
（경로 요소）
3 유일한 제 1요소
xTh문서 중에서 가장바깥쪽에 있는浮솟是
라부릅니다．
〈요소쟈
＜요소2> · · · <／요소2>
（요소3> · " · <／요소3)
(／됴소D

이요소를특별히匣프璽

===== PAGE 38 =====
37 =====
제1일 ×ML의 기본

HI爪Th 문서에도 경로 요소는 존재합니다. html 파일 전체를 포함하는 <html〉태그입니다. 다만，
FflvTh에서는 <html〉태그가 생략되어도 대부분의 브라우저에서 바르게 내용이 표시됩니다．
그러나xll문서의 최상위에는반드시 경로요소가있어야합니다. 경로요소는 쩨 1요소 , '최
상위 요소 라고도 불리며 모든요소는 이 경로 요소 내에 작성됩니다．
예를 들면, books.xml의 소스에서는 <books）
가 경로 요소이고, 바로 아래에 복수의 <book> 요소
가, 다시 아래에 개개의 <name> -소와 <author> 요소 등이 포함되어 있습니다.
(books>
모든 요소는
(bo아◇

／戶

(book)

경로 요소의
아래에 기술된다．

(name)

(name)

(author)

(author)

(category)

(category)

(price>

(price)

(publish>

(publish)

(pDate)

(pDate)
I

\
이러한포함관계에 있는바깥쪽요소를 부모요소 , 안쪽요소를 '자식 요소라부릅니다. 부모
요소, 자식 요소의 개념은 어디까지나 한 요소를 기점으로 했을때 그 바깥쪽에 있는지 안쪽에 있는
지의 상대적인 관계로 정해지는 것이므로, 한 요소에 대해서 부모 요소 인 요소가 다른 요소에 대
해서는 '자식 요조가되는경우도있습니다．
반드시 '시작 태그' 로 시작하여 '종료 태그' 로 끝나야 핸가
可I爪4L 문서에서는 아래와 같은 구문도 사용상문제가 없습니다．
<dt> xxL
.zdd> eXtensible Markup Language

송

===== PAGE 39 =====
38 =====
즉, 시작태그만있고종료태그가없는경우입니다．
그러나XML 문서에서는 태그의 생략은 허락되지 않습니다. 결국, 위의 예는 다음과같이 변경되
어야합니다．
<dt> XML <Idt>
<dd> extensible Markup Language <Idd>

一

단, 내용 데이터가 없는 경우
<img src=' webware. jpgH>
와 같은 요소도 있습니다．
《空要素）
' 라 힙니다. '공요소' 는 일반 요소와 마찬가지로
이렇게 노드를 갖지 않는 요소를 '공요소
ding src="webware. jpg'> </invj>
와 같이 기술할 수도 있지만, 생략형으로
d.ing Brc= "webware. jpg" />

뇨八小～＇→＼小～군｀一， 尸∼군｀ ．→·／∼尸八／

→－~－

一

와 같이 기술할 수도 있습니다．

XML은 왜 HTML.다 엄격한가？
'태그의 생략은 허락되지 않는다“는 것을 시작으로 하여 )(ML에 있어서의 규칙의 엄격화는 시스템적인 부하를 최대한
줄이는 것을 목적으로 하고 있습니다. 현재 HTML을 처리하는 엔진의 80％는 태그의 생략 등 애매한 기술을 자왱으
로 해석하기 위한 로직이 차지하고 있다고 합니다. 이들이 전부 제거됨으로써 엔진이 간소화되어 결과적으로 빠른 성능
을 얻을 수 있습니다. 20％의 주의로 80％의 효율을 도모하는 것이 당연하다고 할 수 있을 것입니다．
－느

모든 요소는 올바른 내포
（nest) 구조로 이루어져야 한다
<hl><font color= ' #FF0000">XML 기본 강F </hl></font>

“

===== PAGE 40 =====
39 =====
제1임 ×ML의 기본

예를들어, 위와같은 태그들이 오버랩되어 작성된 문장이 있을때 I'I소4L에서는 에러가발생하지
.
않습니대：브라우저가 친절하게 자동적으로 그대로 번역해 준 것뿐입니다）
그러나XML문서에서는 허락되지 않습니다. 반드시 태그끼리 내포된 형태로 작성해야만 합니다．
<hl><font co1or= '#FFO000 '>)afl, 기본 강k/ font></h1>

이와같은형태가되어야합니다. 수학식에서도
{ (X+Y) *2) /10

과같이 작성하지 않듯이 같은 원리입니다．

6 각 요소명의 대문자，
소분자는 구별된다
I{I取4L에서는 다음과 같은 문장이 허용됩니다．
<b>XML 기본 강좌＜/B>

시작 태그와 종료 태그의 대문자, 소문자가 달라도 브라우저는 그 대응 관계를 정확히 인식해 주
었습니다. RThTh 대문자, 소문자의 구별을 하지 않는 언어이기 때문입니다．
그러나XMl은요소명이나속성명의 대문자, 소문자를구별합니다. 즉, <b）
와 <B〉라는 태그는종
류가다른 2개의 태그로 인식되어 버립니다．
따라서 XML 문서에 있어서 앞과 같은 작성한 경우아는 시작태그 <b〉의종료태그〃b〉가존재하
지 않아 에러가발생합니다．
<b>XNL 기본 강좌＜/b>

이와 같이 XML 문서에서는 대문자, 소문자까지 정확하게 구별해서 작성할 필요가 있습니다．
（씽따옴표）
로 둘러싸.
속성 값을 " "

<il呵 src=sxnp. jpg a1t=Xn1 />

그러나Xll」
문서에 있어서는반드시속성값을 " "（쌍따옴표）
로감싸야합니다．
위의 예를Xll」
구문으로 작성하면아래와 같이 됩니다．

===== PAGE 41 =====
40 =====
cling src='s跡弑pg斗1:alt=",anl"

또, 속성은 요소의 시작태그 안에 예외 없이 속성명＝'쏙정값'으로 기술됩니다. HIvTh에서는
.ctd 11.Wr

과같이 기술되는경우가종종 있는데, 이것도XML에서는허용되지 않습니다．
사실 이 문장은 <td〉태그의 nowrap 속성이 반드시 값으로써 노1owrap' 을 얻기 위해 생략이 허락
된 것일 뿐, 실제로는
<td nowrap= "nowra

이 올바른작성법입니다. 그리고xTh에서는 이것을생략하지 않고 정해진 형식으로 기술하도록요
구하고 있습니다．

·XML 문서는 주로 요소와 속성으로 구성됩니다．
· 선두에는 반드시 <?xrr기？> 선언이 필요합니다．
· 유일한 경로 요소가 존재해야 됩니다．
· 요소끼리는 올바르게 내포되어야 합니다．
· 종료 태그는 생략할 수 없습니다．
· 태그의 대문자와 소문자는 바르게 대응시켜야 합니다．
· 속성값은 반드시 쌍따옴표로 둘러쌉니다．
· 속성값의 생략형은 사용할 수 없습니다．

===== PAGE 42 =====
41 =====
제1일 ×ML의 기본

7 실력 테스트
「k '

,

.-.

`/erq 刃V`

-:'

,

"1

?

《－

'b0

아래의 XML문서에는문법적인오류가 6개 있습니다. 틀린곳을칫아바르게 수정해 봅시다．

<D《J《JK lq=V쁘쁘？
<title>HTME』 디자인 비주얼 가이드＜/title>
<author>C .1. S</author>
<page>200</page>
<published＞영진닷컴
<memo><b><i>

1 </b></i

</b。
。k>

태그를 쉽게 활용도를 높였

∼－-/'

<book id='00002 ">
<title></title>
<au; r> c/
<page>

author>

눅口illished>< /published>
<memo>< /memo>

懲：,；뇨，
;

L

U

』3811』

===== PAGE 43 =====
42 =====
XML의 다양한 표현 - 다양한 작성법
Lessoni에서 작성한 ×ML 문서를 다른 형식으로 바꾸어 작성해 봅시다．

焄 학습 내용 미리 보기
books2.xml

G)

4 C:WxmI낚SampIeWLesson2Wbooks2.sml - Mlcroooft Internet E: 이Dyer
따임
（F,

XML

- ｀六

편집
（트） 보기
（y)
J

Less。
n2

듦겨찾기(加

J〕소

도구
（工） 도욤맡
《b)

괴검색 ＝」쥴겨찾기

今미디머 -j

．스，J

=

－」④ g

.n?eml sersior1=H1.D` encoding=nEUC-KR" ？》
<books>
r.b口아‘ isbn볍日18BN·9-3i4-1742-)r name=기-ITML 디자인 비주멀 가미드' Cu타sor=dC.I.S"
category="HTML" price='11000' pubtish=' 영진닷컴' pDate="200i-06-11' />
<book usbn="I8BNB9-314-1978-3' name="ASP 사전' euthor="니시자와 나오키∥
cateqory='ASP" pnce='15000' publish=' 멈진닷컴’ pDate="2001-11-30' />
<!- 최좀 갱신 =z.口2/1/2日 ->
</b미軟5>

圈완료

XML 문서를 인터넷 익스플로러에서 실행한다 -

( Key Point )
XML은 자유로운 언어입니다. 그러므로 같은 내용을 표현하는 데도 여러 가지 방법이 있습니다. 이번
Lesson에서는 이러한 표현 방법을 알아보고 각각의 장· 단점을 이해해 보다 효율적으로 XML 문서
를 작성하도록 합니다．

企

===== PAGE 44 =====
43 =====
제1일 ×ML의 기본

1 새문서를열어리스트의코드를입력한다．
at스트 : books2.xmt
<?xxnl version="l. O " encoding= "ETJC-KR" ?>
<books>
<book isbn="ISBN89--314-1742-x"
name= "HTMl』 디자인 비주얼 가이드" author="C.I. S" category="HTML"
price="11800 " pu]D1ish= " 영진닷컴" pDate="2001-06-ll " I>
<book isbn="ISBN89--314-1978-3" name= "ASP 사전"
author= " 니시자와 나오키" category= "ASP"
1i8h= " 영진닷컴“ pDate="2001-ll- 30 " I>
price="15000 " p띠〕
<!--최종 7 j" : 2002/l/ 28 -->
</books>

2

입력후［Dl］폴더에books2.xml라는이름으로저장한다．

(1: 이름을입력

:
파일 미暴《쑈）

沁ooks2. xmll

《I):
파읾현식

I

스트 믄서

3 [Dl］폴더를열어books2.xml을실행한다．

===== PAGE 45 =====
44 =====
데이터의 내용은 Lessoni의 lDoOks.xIDI 과 Lesson2의 'books2.xml' 이 거의 동일합니다. 그렇
지만구조는 크게 달라졌습니다．
즉, 전자가 하나의 서적 정보를 <book) 요소 아래 자식 요소군으로 기술했던 것에 비해, 후자는
<book> 요소의 속성군으로 작성하고 있습니다．
어느 쪽이 효율적인 작성법인지는 한마디로 단언할 수는 없지만, 여기에서는 각 기술들의 장점과
동시에 XML 문서를작성할 때의 주의점에 대해서도 설명하기로 합니다．

1 요소가 주체인 XML
Lessoni의 hioks.xi교과 Lesson2의 books2.xml을 비교하여 바로 느낄 수 있는 것은1xoks2.xm
쪽이 간결하다는 점일 것입니다. 반대로말하면요소주체로구성된 XML문서는매우장황해지는 경
소명〉데이터<I요
［'으로 표현되는 데 반해, 요소가 '<2．
향이 있습니다. 이것은속정이 속성명＝쓱：성겋
소명〉
' 으로표현되고 있는구문상의짜임을봐도쉽게 이해할수 있습니다．
그러나 요소는 자식 요소를 갖을 수 있기때문에 요소 내의 데이타를 보다 세밀하게 구분하고자
할 경우에 유연하게 사용할수 있습니다．
아래와같은 예를 생각해 봅시다．
<author＞니시자와 나오키＜/author>

이것을 성과 이름으로 보다 세밀하게 분류하고 싶다고 합시다. 이 경우，
<author>

…… ………

…

…

<firstName>니시자와＜/firstName>
<lastName> 나오키＜/lastName>
</author>

와 같이 작성할 수 있습니다. <firstName) 요소와 KlastName) 요소가 추가되어 있지만, <author>
요소의 텍스트는 변경 전이나 변경후나 니시자와 나오키' 이고, 성
（이름）
만 추출할 경우에는 각 자
식요소의 데이터를바로 얻을수 있습니다．

小

===== PAGE 46 =====
45 =====
제1임 XML의 기본

一
（단락）
를 적용하여 작성하는 것이 관례적입니다. 이렇게 함으로쩌 어
요소 아래 자식 요소를 기술할 경우, 들01 쓰기
느 요소가 동일 계층에 속해 있고, 어느 요소와 어느 요소가 친자 관계에 있는지를 시각적으로 파악할 수 있게 되어
코딩상의 실수도 줄일 수 있습니다．

2 속성이 주체인 XML
문서에서는 위와같은 데이터의 통합과분할은 어렵다고 할수 있습니다．
한편, 속성 주체의 xfl」
<book author=" 나시자와 나오키" />

（子屬慘 등의 개념이 없으므로 아래와
라는 데이터를 성과 이름으로 분할할 경우, 속성에서는자속성
같이 해야 합니다．

새로 작성된 firstName 속성과 lastName 속성은 원래의 author 속성과는·전혀 관계없는 것으로
인식되어 버리므로, 당연히 호출하는쪽의 프로그램도 변경해야만합니다. 굳이 원래 데이터와의 호
환성을 유지하고 싶다면 다음과 같이 데이터를 장황하게 기술해야 합니다．
<book author= " 니시자와 나오키" firstNaxne= " 니시자와" lastName = " 나오키" />

속성 주체에 있어 xTh의가장 큰 장점은 그 간격함에 있습니다．
앞에서는 말했듯이 어쨌든 요소 주쳬, 속성 주체 중 어느 쪽이 더 좋은지는 구분할 수 없습니다．
그때 그때에 맞춰 확장성, 용량등의 여러 가지 관점에서 구성을 생각해 보는 것이 중요합니다．
3XML 문서는 자유롭다
지금까지 다뤄온 XML 문서는 관계 데이터베이스의 필드, 레코드의 개념을 느낄 수 있는 정형적
인형식이었다고 할수 있습니다．

0

===== PAGE 47 =====
46 =====
[XML 문서와 례코드의 관계】
_
publish

HTML 디자인 비주얼 가이드

영진닷컴

11600

ASP 사전

영진닷컴

15000

name)

</

7

,(/

l-

(boo,
(name)HTML , F인 Hl，
k)
엌
(publish＞영진닷컴
（/publish)
(price>11600(/price)

-

price

·하나의 레코드가
하나의 <book>
요소에 내용

(books)
-

l,

L

-

name

(Jbook)

· 각 필드는 (book)
요소 아래의 각
자식 요소에 해당
한다．

(/books)

그러나XMl꾀 매력은 이러한 정형적인 문서뿐만 아니라 비정형의 자유로운 문서에 대해서도 이
용할수 있다는 점에 있습니다. 예를 들어
〈본문＞
（키워드〉XML(／키워드）
은 마크업 언어입니다．
<／본문）

와같은문서도XMl』
의 予칙에준한어엿한XTh문서입니다．
마크업이란 나중에 데이터를 추출할 때의 표시에 지나지 않으므로, 데이터가 어떤 목적을 가지고
마크업되어 있다면 그것이 정형이든 비정형이든 그다지 관계가 없다는 것입니다．
4 깊은 계층 구조는 바람직하지 않다
（孫要素）
로
XML 문서는 트리 구조라 불리는 것처럼 요소 아래에 자식 요소가 있고 그 아래 손요소
되어있는 계층 구조입니다. 그렇기 때문에 XML 문서 작성시 필요 이상으로 깊은 계층 구조를 취하
는 경향이 있기도 한데, 그럴 경우 문서가 복잡해집니다. 구조를 갖게 한다는 것은 데이터를 목록화，
그룹화하여 무엇인가 의미를 주기 위한 계층구조가 필요해서입니다．
깊은 계층 구조를 읽기 위해서 그만큼 복잡한 로직과 시스템에 대한부하를 요구한다는 점을 고려
해야합니다．

===== PAGE 48 =====
47 =====
제1일 XML의 기본

-

경로 요소

친자 관계

(book)

"

(name)

(author)

(publish)

(price)

(pDate)

형제 관계

데이터로 표현할 수 없는 내용은 주석으로
서적 정보의 수정 내용 등 나중에 참조하기 위한메모와 같은 정보는 보통 요소나 속성 등과 구별
하여 기록하는 것이 바람직합니다．
예를들면아래와같습니다．
'^

이 방식은 I了I刪L에서도사용하는 것으로 ◇－- ∼－-〉에 주석을작성합니다．
주석문을xTh 문서 내의 적당한 위치에 삽입함으로써 보기 솨운XML을작성할수 있습니다．

｀∼

· 요소로 기술된 데이터는 장황하고 데이터량이 많아지는 만큼 데이터를 더 세밀하게 구분하고자 할 경우 유연하게
사용할 수 있습니다．
· 속성으로 기술된 데이터는 데이터의 통합, 분할 등 구조 변화에 약한 만큼 데이터량이 소량으로 제한되어 간결하
게 기술할 수 있습니다．
·XML 문서는 비정형 문서를 작성하기에도 적합합니다．
· 필요 이상으로 깊은 계층 구조를 취하지 않도록 합시다．
· 주석문은 신－- N --> 안에 작성합니다．

===== PAGE 49 =====
48 =====
실력 테스트
-

아래와같은 두 가지 성질을 가진문서가 있습니다. 각각의 내용을 요소 주체로 기술하는 것이 좋은
지, 속성 주체로 기술하는 것이 좋은지 검토해 봅시다．
（〕
）정형적으로 정리된 코드가 주체의 데이터이고, 개개의 데이터가 앞으로 세분화되리라고는 생각
하기 어렵다. 데이터량이 많아서 아주 적은용량으로 기술하고 싶다．
(2) 아직 정확히 데이터가 분류되지 않은 산문적인 내용이다. 앞으로 데이터의 통합 · 재편집이 빈번
히 이루어질 것으로 예상된다．
해답은 책 끝에 今

Dr.XML과 나미의 원포인트 강좌

한글 태그를 사용해도 좋을까요？
나미

' 저, 박사님, XML에서 태그를 한글로 써도 좋을까요？"

Dr.XML

' 한글 태그라... 확실히 <order）
라고 쓰는 것보다도〈주문서）
라고 쓰는 편이 알기 쉽긴 하겠죠．
'

나미

'박사님 말씀엔 뭔가 의미가 확실치 않은데요…'

Dr.XML

"그래요, 확실히 나미양의 말대로 요소명과 속성명에 한글을 사용하는 것이 반드시 금지되어 있지는 않습니
다. 실제로 한글을 사용하고 있는 자／ㄴ도 적지 않습니다. 그렇지만 솔직히 그다지 권하고 싶지는 않아요"

나미
Dr.XML

' 왜 그렇죠？"
' 확실히 한글을 사용하면 보기 쉬워질거라 생각할 수 있습니다. 그러나 잘 생각해 보면 텍스트 부분이 한글
인 경우 본래의 한글과 태그의 한글이 서로 섞여버려 의외로 보기 어렵게 됩니다. 입력할 때를 생각해 봐도
태그를 나타내는 'C와 >' 같은 기호는 반각이므로 의외로 한글과 영문의 교에 둥 입력이 번거롭고 또 그만
큼 입력 오류가 많아집니다. 게다가한글 자4L보다 영어 XML이 많은데們TML이라고 해서 전부 영어 태그
인가？), 그것들을 사용하고자 할 때 한글과 영어가 혼재하게 되면 통일감이 없습니다．
그리고 마지막으로 강조하고 싶은 것은 아무리 )(ML이 한글에 대응하고 있다고 해도 실제로 한글을 표기할
수 없는 컴퓨터가 아직 어느 정도 있다는 것입니다．
"

나미
Dr.XML

'그래요？"
'한글 태그를 절대 사용하지 말라고 하는 것은 아닙니다. 다만 한글을 사용하면 그만큼의 단점이 있음을 미
리 확실하게 파악해 두자는 얘기입니다．
'

나미

' 네∼에！"

===== PAGE 50 =====
49 =====
제1일 >(ML의 기본

Go to XML

===== PAGE 51 =====
50 =====
n

了

n3,

Less。

Less。

包，

J

n5

XSLT 스타일 시트로

레이아웃하기

제 1일에서는 먼저 X1vTh 문서를 작성해 보았습니다. 그러나 이것만으로는 아직 실제로 사용할 수 없습
니다. 이를적합한형식으로변경해야할필요가있습니다．
이것이 XSLT(eXtensible Stylesheet Language 'ftansfonriations）
의 역할입니다．
XSLT는마크업 언어이면서 동시에 일반 프로그래밍 언어적 요소도 갖춘 약간특이한분위기를 가진 언
어입니다. 처음쩨는 다루기 어렵다고 생각될지도 모르지만 기본 내용을 확실히 알아두면 그 유연성과풍
부한 표현력에 매료될 것입니다.

===== PAGE 52 =====
51 =====
오늘 공부할 내용들
XSLT로요소 ' 속셩의 내용표시하기
목록표로 출력하기
데이터를 정렬하여 링크 작성하기

===== PAGE 53 =====
52 =====
XSLT로 요소 · 속성의 내용 표시하기
제 1일에 작성한 ><ML 문서는 익스플로러의 화면싱께 소스 코드만 표시되므로 실제
용도로는 사용할 수 없습니다. 익스플로러상에서 훌륭한 포맷으로 변경하기 위해서
는 ×SLT를 사용하여 ><ML을 HTML

변환합니다．

학습 내용 미리 보기
=books.xsl
｀冽eb관련 서적 목톡 - Micros嫩姓5K，
戟∼.「寸'
낫杉γ“
파일
（F) 편잡（트） 보기
（y) 줄겨찾기（스） 도구（工） 도움말（브）

느books.xml

J

三〕仝

즐겨찾기
烈검색 三」

.

三孕미디머 ,3 ∼노 =j

" 면궐 "

○XML

尸뒤로 , ＼剝

』」．므i즈1

L□

Q&a

→」

\ l Lesson 3
,

-

Web 관련 서적 목록
ISBN 코드서적 저자 출판사 가격 발간일

Youngjin.com Y.

韆藝囊…

r

「긔；LH 컴퓨터

내에 기술된 <books＞와〈owner> 요소의 내용이

표

-

-XML문서

-

시된다 1

(* Key Point ) _
이번 Lesson에서는 XSLT 스타일 시트에 대해 학습합니다．
는 XML의 구문 규칙에 따른 마크업
§叱mam.旦）
旦긴，
올t堤만ㅗ롓그9므9g르J胤〕
XSLT(eXt 9ible，
언어이지만, BASIC이나 C와 같은 일반 프로그래밍 언어적 요소도 함께 갖춘 일종의 독특한 언어입
니다．

自

===== PAGE 54 =====
53 =====
제2일 ×SLT 스타일 시트로 레이아웃하기

[I川폴더에있는books.xiril을열어리스트1의코드를추가한후［D2］폴더에books.xml
로 새로 저장한다．
리스트 1: bo이
《s.xml
※ 색 글씨 부분이 추가할 코드입니다．
<?xml version='1. O " encoding= "EUC-KR" ?>

<book isbn="ISBN89-314-1742-x ">
<name>HTMI』 디자인 비주얼 가이드＜/name>
<author>C .1. S</author>
<category>HTML< / category>

<price>11800</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-06-ll< /pDate>
</book>
<book isbn= 1'ISBN89-314-1978-3 ">
<name>ASP 사전＜/name>
<author＞니시자와 나오키＜/ author>
<category>ASP< /c:ategory>

l>

1

20
21

<price>15000</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-11-30< /pDate>

22

</book>

23

<book isbn== "ISBN89-314-1994-5

24

<name＞알짜 PC 용어 사전＜/name,

25

<author＞슈와 시스템＜/autho王

26

<category>김퓨터 사전＜/catego工y>

27

<price>19500< /price>

28

<publish>영진닷컴＜/publish>

0

===== PAGE 55 =====
54 =====
29

<pDate>2002-01-05</pDate>

30

</l거：)0k>

31

<book isbn="ISBN89-314-2014--5 ">

32

<name>10일만에 배우는 Visual C++ 6.0</name>

33

<author>Seto Haruka< /author>

34

<url>http: I/ www.youngjin.com <(unl>

35

<category>Visual C+ +< /category>

36

<pnice>15000</price>

37

<publish＞영진닷컴</publish>

38

<pDate>2002-02--05</pDate>

39

</book>

40 </1Coke>

새 문서를 열어 리스트 2의 코드를 입력하고, [D2] 폴더에 books.xsl이라는 이름으로 저장
한다．
리스트 2 : bo이〈s.xs1
<?xml versiori="l. O " encoding='EUC-KR' ?>
<xsl: stylesheet xinlns:xsl= "http: //www.w3.org/1999/XSL/Transform '
version= '1. 0 ">
<xsl :output method="html" encoding= "EtJC-KI之" I>
<xsl : template match=" /">
5

<html>

6

<head>

7

<title>

8

<(head>

9

<hl><xsl :value-of select= "books/@title" /></hl>

<xsl:value-of select="books/@title" I> <(title>

10

<table bcrder="l ">

l.1

<tr>
<th><xsl : text>ISBN 코드</xsl : text></th>

12
13

<th><xsl : text>Al적</xsl : text></th>
<th><xsl : text>저 k/ xsl : text></th>
<th><xsl: text>출판AF</xsl : text></th>
<th><xsl : text>가격</xsl = text></th>
<th><xsl : text>발간일</xsl : text></th>
</ t그？>

<(table>

===== PAGE 56 =====
55 =====
<div><xsl:value-of select= 'books/owner" I> </div>
</htnil>
</xsl:template>
</xsl:stylesheet>
Check
弘髮》鈿1

XSLT스타일 시트문서의 경우, 확장자는 ':xsi 로하여 XML문서의 '.xini 과구별합니다．

3[ D2］폴더에서books.xxnl을실행한다．
Check
point

데이터는 표시되지 않는다
"' " -- ' " --'
코드를추가한bookaxinl의 <book> 요소의 뎨이터는이번에 작성한books.xsl에서는표시
되지 않습니다．

books.xml을 실행하면 XSLT 스타일 시트 books.xsl어］의해 변환된 내용이 익스플로러상에 표시
됩니다．
이번에 작성한 XSLT 스타일 시트 books.xsl은 books.xml에서 <books> 요소의 title 속성과
<owner> 요소의 데이터만추출하여 표시합니다．

XML- 문서와 ×Sㄵ 스타일 사트를 연결힌다．
XSLT를 사용하려 해도 단순히 XML 문서와 )(SLT 스타일 시트만 준비해서는 안 됩니다. 먼저
)Uvll에 어느 XSLT를 연결할지를 지정할 필요가 있습니다. 이것을 연결하는 것이 books.xml의 2
행에 추가한다음문장입니다．
<?xml - stylesheet type="text/xsl ' href="books.xsl" ?>

스타일 시트의 형식

스타일 시트의 위치

===== PAGE 57 =====
56 =====
<9X끄〕l - stylesheet?> 처리 명령은 지금까지와 같이 xll 문서를 그대로 트리 구조로 표시하는
것이 아니라, 지정된 XSLT 스타일 시트를 적용하여 그 결과를 브라우저에 나타냅니다. 보통
<9xml9> 처리 명령문다음에 작성합니다．
(1) type 속성

슨탄앝麓i읫尖喙興多는豊순젖：휄욘손론쓰轉夢튱겸多합니다．만약，CSS(Cascading
SbleSheet）
를 이용할 경우에는 'text/cs 로 지정합니다．
(2) href 속성
스타일 시트를 저장한 위치를 지정하며 역시 필수적인 요소입니다. 이번과 같이 XML 문서와 같
은폴더에 저장되어 있을 경우는 파일명만 기술합니다．
이렇게 해서 XML 문서 bookaxrnl을 표시할 때에 XSLT 스타일 시트 books.xsl가 적용되게 됩
니다．
예를 들어, 앞으로 books.xml을 다른 스타일 시트를 사용하여 표시하고자 할 경우에는 이 2행의
href 속성만 변경하면 되므로 XML 문서 자쳬는 전혀 변경할 필요가 없이 데이터와 스타일을 분리
하여 편리하게 사용할수 있습니다．

0
XML- 문서와 XSLT 스타일 시트를 연결하는 방법은 이것 외에 앞으로 학습할 DOM(Document Object Model）
이
라는 장치를 이용하여 보다 다이내믹하게 잉따를 연결지을 수 있게 됩니다. DOM에 대해서는 제 5일, 제 6일의
Lesson에서 설명합니다．

2XSLT 스타일 시트를 선언힌다
jooks.xsr 의 1- 2, 23행을살펴 봅시다．
<?xml version="l. O ' encoding= 'EtJC-I汪
（" ?>
<xsl : stylesheet
version="l. O">
</xsl : stylesheet>

…n…m∥
寸………“… ……「
xmlns:xsl= "http= //www.w3 . org/19991X5L/ Transform"

===== PAGE 58 =====
57 =====
제2일 ×SLㅜ 스타일 시트로 레이아웃하기

1행은 첫째 날에 소개한 <?xml?> 선언입니다. XSLT도 XML 구문에 따라서 기술된 x}4L 문서입
니다. 문서 처음에 버전과문자코드를 선언합니다．

，숏公史쁘뜨으多손늡읜受上XSLT슷탰휄신員읜燧롯(쵯〔살；웬웃솟가됩니다勵dL문서에는
경로 요소는 필수임）
. 모든 스타일 정의는 이 <xsl:stylesheet> 요소 아래 기술됩니다. xmlns:xsl 속
설은 '<xs1:∼’로시작하는止소가어唾土균크에따르는가를지정하기 위한옵션입니다．XSLT의 경
우는반드시 다음과 겉끼 지정합니다．
http: /Iwwn.w3 .org/1999/XSL/Transforrn

`.'

이 3행은XSLT슷탰맡스煌계姃콧廻웃롯Z憶하는 것이므로 일종의 정해진 법칙이라고생각
하시기 바랍니다．

xmlns:xx( 속성은 정확히 말하면 이름꽁간을 지정하는 것입니다. 이름 공간이란 요소의 앞에 접두사 的o(:，와 같
이 표현되는 이름 짓기 규칙의 하나입니다, 같은 문서 내에 다른 의미의 동일 요소명이 있을 때 XML은 이름 공간을
사용하여 이를 구별합니다．
예를 들어, 동일 문서 내에 다른 의미를 가진 <name) 요소가 있더라도 이름 공간으로 <xyz:name>, <abc:name）
과
같이 지정함으로써 두 개를 구별할 수 있습니다，

3XSLT는 템플릿의 집합체이다
경로요소인 蜘l:s브．브쁘웃손읜－브트世빤三숏坐브뽀쁘욘솬기술되어 있습니다·
<xsl:template> 요소는xTh문서에 대해서 적용되는翼았슥탑是J쵠量」
윗，
니다1 이 일련
의 스타일 규칙을 템플릿’ 이라부릅니다．
books.xtht로부터 XSLT가 호출되었을때, 제일 먼저
<xsl:template match= ' / " >
</xsl: template>

===== PAGE 59 =====
58 =====
로 기술된 템플릿이 호출됩니다. match 속성은 '이 템플릿이 끄dL 문서의 어느 요소에 대해서 적용
되는지' 를지정ㅎ隱것으룁'I'
I i1_ 섦，
콧鉀를나타냅니다·
XSLT 스타일 시트에 있어서는 제일 먼저 ‘경로 요소에 적용될 템플릿’ 이 불려집니다. 즈sLT 스
타일 시트 내부에는 적어도 하나의 템플릿이 존재하며, X}dL 문서의 경로 요소에 적용되는 템플릿
은생략할수 없습니다．
앞으로 복수의 템플릿이 존재하는 XSLT 스타일 시트를 다루게 되는데 그 경우에도 기점은 항상
이 경로 요소에 대한 템플릿이며, 여기서부터 복수템플릿이 순차적으로 불려지게 됩니다.
XSLT 스타일 시트는 이러한 템플릿의 집합체인 것입니다．
[XSLT는 템플릿의 집합체】
_
l

-

(xsI:styIesheet>

1

ㅣ
-－入

(xsI:tempIatematch="f')

<xsl:template)

Kxsl:template)

다
XSLT의 출력 방법을 선언힌）
이번 예제 스크립트에서는 xTh문서를HThIL 문서로 변환시켰는데, XSLT는xTh 문서를반드
시 I{I刪I로 변환하기 위해서만사용되는것은아닙니다·驪프兮t그瓊只§包근哭歟鈐라는 이름
대로 원래의 xTh문서를 다른 형식으로 변환 하기 위한 것입니다．
그러므로 때로는 XML 문서를 I1I뇨4L이 아닌 다른 형식의 XML 문서' 로 변환하는 경우도 있고，
텍스트나 다른 형식으로 변환하는 경우도 있습니다. XSLT의 다양한 용도를 고려한다면 ITI丕4L로
의 변환은오히려매우 특수한하나의 패턴이라생각할수 있습니다．
3행의 鈿l:output> 요소는 이러한XSLT의출력 형식을 선언하기 위한것입니다．
:<xsl:output method='html" encoding="EUC-KR" I>

===== PAGE 60 =====
59 =====
제2일 XSLT 스타일 시트로 레이아웃하기

이 문장의 선언에서 XSLT 스타일 시트의 출력을 담당하는 클라이언트
（브라우저）
쪽은 I了I뇨江L 형식
으로, 문자코드는EUC-KR코드임을확인할수 있습니다. xML문서와XSLT스타일 시트본체를
기술하는문자 코드는다르므로 주의하기 바랍니다．

,-r

<xsl:output> 요소는 반드시 기술해야 하는 것은 아닙니다．그러나 브라우저에 의한 인식 오류를 방지하고 정확성을
위해 기술하는 습관을 기르는 편이 좋습니다．

r --1
r, ^ n 1 I ' ^ [1
``xㅂ ㅗ = (JuI;1Juㄴ＞ 뵤＝』느스ㅢ 시《긔I

<xsl:output method= "출력 형식
（XII)1 I html I text) . 디폴트는 html·'
[version= " 버전'1]
[encoding= " 문자 코드" 〕
[indent= "들여쓰기 여부
（yes I no) "]
[media-type="MIME EF입(text/htmJ. 등) "1 I>
※［∼］
로 둘러싸인 속성은 생략 가능함을 나타내고 있습니다．

indent 속성은 이동 기기 등 수신 용량에 제약이 있뇬 단말기의 경우 돌여쓰기를 생략하여 용량을
압축합니다‘

고정적인 텍스트를 표시한다
［늡全sltex으프손量스上：8합니다. 예를들어, 이번
竺띤
엔L늪브스튼量프스1흐브잔．
型些星선．
샘플과 같이 데이터를 표로 출력할때 표제어를달고 싶은 경우등입니다．
<th><xsl: text>ISBN 코드</xsl: text></th>

<XsI:text> 요소로 둘러싸인 부분은 그대로 텍스트로 출력됩니다. 다만, 鈿1:te) ) 요소는 특수한
경우를 제외하고는 생략할수도 있습니다．
위의 12행의 경우다음과 같이 기술해도 별다른문제는 없습니다．
<th>ISBN 코드＜/th>

이 책에서는 앞으로 특수한 경우를 제외하고는 <xsl:text) 요소는생략하고 기술하기로 합니다．

===== PAGE 61 =====
60 =====
r 小＇^] .

,..' - `

C A C)I `JAIl

L｀ㅅbJ~ z ㄴ口ㅅㄴ？ 」ㅍ＝J二＝

'r- ii

<xsl : text disable-output--escaping= "출력할 문자를 이스케이프 할지의 여부
（yes I no) ">
표시할 텍스트
< /x釘．text>

※ <xsl:text> 요소는 생략 가능합니다，

「o] 을그대로' ' 케"匡시
내부텍스트엔썅쓰르르旦曙브라우저에표시하고싶은경우
키지 않도록하기 위해 鈿l:text) 요소를 이용합니다. 이런 경우다음과같이 기술합니다．
<xsl:text disable-output-escaping="yes">&lt; </xsl:text>

.

요소의 내용을 표시한다
XSLT에서 가장 빈번히 나오는 요소가 <xsl:va]ue-of> 요소입니다. 柚l:value-of> 요소는 select
속성으로 지정된 요소
（또는속성）
의 내용을구하여 출력합니다．
select 속성으로 요소를 지정하는 방법은 HThIL 문서에서 폴더의 상대 경로를 지정하는 방법과
아주 비슷합니다．
<img src="sample/webware. jpg" />

이 표PML 태그는 현재 파일이 놓여 있는 폴더
（현재 폴더）
를 기점으로 하여 바로 아래의 sample
폴더에 저장되어 있는webware.jpg를 표시합니다. 단, XSL'T뻬서 기점이 되는 것은 현재 폴더가아
니라 현재 요소0〕
＝드）
입니다．
현재의 템플릿'ㅣ 표시하고 있는 것은ST AT르섶-

-- 손 CD으ㅗ므무 " 隱 기점으로 하여

<owner> 요소를 지정해 봅니다．
<div><xsl:value-of select= "books/owner" /></div>

결국, 20행의 select 속성 'books/owner'는 경로 요소를 기점으로 하여 <books> 요소 아래의
<owner> 요소를 나타내고 있습니다. 만약 삯x)oks> 요소 아래의 <book> 요소 아래에 있는 <name>
요소를 나타내면 select 속성의 값은 'books/book/name? 과같이 됩니다．
이렇게 요소 또는 속성까지의 경로
（path）
를 표시하는 방법은 xPath라는 규칙으로 정해져 있습니
다. xPath로 정해진 여러 가지 규칙에 대해서는 간단히 소개할 수 있는 것이 아니므로 앞으로 새로
운 子칙이 등장할때마다소개하기로합니다．

===== PAGE 62 =====
61 =====
n

＝ㄴ一 `'）ㄷJL紛沁入＝
出* 一』석’ ^t

'’

제2일 XSLT 스타일 시트로 레이아웃하기

탭．

"`

n`

珊，1

卜4틴‘卜겹

∥

꺅

＝그니
rr

/

바로 아래 요소

book/author
(book》요소 바로 아래의 <author> 요소

II

모든 자손

books//name
(bo아
（s> 요소 아래의 모든 (name> 요소

현재 요소

./category
현재 노드 바로 아래에 있는 <catego아 요소

*

모든 자식 요소

bookJ*
(bo아◇ 요소 바로 아래의 모든 요소

@

속성명의 접두사

book/@isbn
(book◇ 요소의 isbn 속성

이름 공간 분리 문자

(ym:books xmlns:ym="urn:books")

r
L<x8ㅗ :vaㅗue-.L>

r`

^ r니

』

` ,

ㅛ＝‘죠ㅋ 시식」

<XS]. :value-of select="추출할 요소의 경로《xPath식）
"
dible-output-escaping= " 출력할 문자를 이스케이프할지의 여부
（yes m no) " I>
※ 가장 빈번히 나오는 요소 중 하나입니다．

7 속성 내용을 표시힌다
XML문서 내의 속성礪鍵싶할경우도기본적인방식은같습니다．7행을살펴봅시다·
<title>

<xsl:value-of select="books/@title" I> </title>

현재 노드인 경로요소를 기점으로 하여 삯xoks> 요소 ㅇ 10 title속성을나타냅니다. 요소의 경
우와다른점은속성임을표시하기 위해속성명 앞꺼 반드 t ',.) , 추7fi다는점뿐입니다．
만약 <books> 요소 아래의 <book> 요소 아래에 있는 isbn 속성을 표시하면 select 속성은
'ooks/book/@isbn' 과같이 됩니다．

===== PAGE 63 =====
62 =====
-

【노드를 지정하는 방법은 상대 경로를 지정하는 방법과 비슷하다】
_
［요소 소스 지정 방법］

, ［상［거 경로 지정 방법］

[DayOl]

-

L

[Day03-01]

r

-－눋

[Day03-021
Day03/Day03-02

a

韆
｀中

·XSLT 스타일 시트의 경로
（최상위）요소는 <xsl:st닌esheet) 요소입니다，
·xmlns 속성으로 "htIp://www.w3.org/1999, (S나Transform"을 지정합니다．
·XSLT의 출력 형식을 선언하려면 <xsl:output) 요소를 사용합니다．
· 정적인 텍스트를 표시하려면 <xsl:text> 요소를 사용합니다．
· 요소와 속성값을 구하려면 <xsl:vatue-of) 요소를 사용합니다．
· 속성명을 지정할 경우는 속성명 앞에 '@' 를 추가합니다．

<name)

{Day03]

<author>

r’

伊
[Day02]

book/name

===== PAGE 64 =====
63 =====
제2일 XSLT 스타일 시트로 레이아웃하기

XML문서 diaiy.xnil을 아래 그림과같이 표시해 봅니다. diaiy.xml과diary.xsl의
dL문서와XSLT 스타일 시트를완성시키십시오．
채우고, 올바른X〕
=j그〕
多
급」뒤로 ,

스） 도구（J,) 도움말(H)

-

파일
（Er

D

J 〕 소 烈검색 汕즐겨찾기 秒UI디머 " 면결 "

J

2002-01-16의 일어난 일
날씨:
0 E요
El =

본문 :
개를 기르기 시작했습니다．이름은 공자．궐혼했습니다．
그의 이름도 공자．두 마리 모두 작고 귀엽습니다．
나미

!-l- r-J驪내 컴퓨터

완료

diary.xml
<?xml version='l. O" encoding= "ELJC-KR ?>
''
[ ] <"Y.Wt ;c,j수5l, a - )e二 "ie`t/ ( I " LY'{ = ',,!,nr너 丈
（之
<ch1ary owner= "LFuT ">
<day date="2002-0l-16">
<title＞공자＜/title>
<weather>맑음< /weather>
<body>
개를 기르기 시작했습니다. 이름은 공자．
결혼했습니다. 그의 이름도 공자．
두 마리 모두 작고 귀엽습니다：
</body>
</day>
</diary>

공백을

===== PAGE 65 =====
64 =====
diary.xs!
<?x祉 version="1.0' encoding= "EtJC-KR" ?>

〔 〕 노鞠（ :，늦批d畔枕 ＼贓m：川＝，《啣：/，「ww，따土.다／1汁e/ xcL/ Tr「cco-ri ' V8？唾
<xsl:output method="htxnl" encoding= "EUC-KR" />
<xsl:teinplate match="/ ">
<html>
<head>
<title＞나미의 일기장＜/title>
</head>
<body>
<hl> [

] 의 일어난 일＜/hl>

4이＼ V《t以.- cf 「님醜t: "出叫／啣斂曲" 乙＞／길

<hr I>
<dl>
zf ／乂d t슨yt `.>
긴
<dd><xsl:value-of select="diary/day/weather" I></dd>
I </dt>

' ＼니 ' t求t >

-1니

<dt> [

<dt><xsl:text>본문: </xsl:text></dt>
<dd><xsl:value-of select="diary/day/body" /></dd>
</dl>
<div alican="rioht"> f

1 <Idly>

..Ui.나갹 轍￡比 = " d蠟 ／gL盼’'"' r
(X니．

</body>

.

'/

</html>
<Ixsl : template>
<Ixs1: stylesheet>

해답은 책 끝에 =>
/

cli r' "坤 비씨

（냄 >
. '힁 kt如 十
甲뇨tml , liTmㄴ．. l
어너'{
回 he.,d 스

回 k映l · “댕분
히t궁di 驪 tjte ,o,ru4

.}) b수
, ..
기

區）뇨1` : 츨쟈흽 후 기 X;j
G) .1 - 엎 추 c 처긱
@) 눠y

嚼‘m " "'們口7
선그겨거 r h一」

헤 楓

윅혹‘
（회 LtL 色처 旨虐
숀서 眺 욕룅
껍늬욕芎 b恥 c1t:

ㅈt왁包북

',

〔빈크욉산륙거는 零옰）

===== PAGE 66 =====
65 =====
제2일 XSLT 스타일 시트로 레이아웃하기

.
G. t. 지＼川．

===== PAGE 67 =====
66 =====
제2일 XSLT 스타일 시트로 래이아눗oil

목록표로 출력하기
이번 Lesson에서는 <bo아◇ 요소로 표현되는 도서 정보가 반복 출력되는 )<ML 문서
를 작성합니다．

학습 내용 미리 보기

- 1books.
fl

css
긔(助

3: 1

,

도움말
（브）

d, =j “下 三」韜

Web 관련 서적 목록

○XML

Less。
n4

L n그 Q&a

ISBN 고드
서적
저자
출판사 1가격 발간일
;1SBN89-314-2014--15 10일 만에 배우는 Visual O++ 5.0 Seto Haruka
l영진 닷컴져Soc刈2002-02-05
巾SBN89-314-1994-5 먈짜PC 죵어 ' 나크
슈와시스템 삐濩친핫苕｛耐dj 2002-01-05
巾SBN89-314-1978-3 ASP 사…
L- ,새자와〔F231영짇닷컴＼1150西凶이-11-30
C.LS
-－陋진닷컴！
11800泛〕
01 0& 11
ㅔSBN89-314-1742- HTML디자인 비주얼 가이드
Youngjin.com Y

서적목록이HTML테이블로표시된다 ㅣ

l

S Key Point ) _

*

드디어 ×SLT의 <xsl:for-each> 요소가 등장합니다. 이것은 XSLT가 H쟈기L이나 자ALZ 어느 정도
분명한 구분을 짓는 프로그래밍 언어적인 요소입니다．
프로그래밍에 익숙지 않은 분은 닌旨ㅐ할 수도 있지만, 어떠한 흐름으로 처리가 진행되고 있는지의 기
본적인 사고법을 정확히 이해해두면 앞으로 다소 복잡한 처리를 하게 되더라도 쉽게 이해할 수 있을

년입

：누\

도구
（j)

盈검색 츠」즐겨찾기 今DI디머 J

"ㅣ
"L

===== PAGE 68 =====
67 =====
제2일 XSLT 스타일 시트로 레이아웃하기

Lesson3에서작성한books.xsl를열어리스트1의코드를추가하고같은이름
（books.xsO
으로 저장한다
리스트 ㅕ: books.xs!
※ 색 글자 부분이 추가할 코드입니다．
<?xml version="l. O" encoding= "ETJC-KR" ?>
<xsl = stylesheet

janlns:xsl="http = //W` w.w3 . org/1999 /XSL/Transform"

version="l. O ">
3

<xsl:output method="html" encoding= "EUC-KR" I>

4

<xsl:template match="/ ">
<html>

5
6

<head>
[

7

<title> <xsl:value-of select="books/@title" I> <Itit1e>

8
9

</head>

10

<hl><xsl:value-of select="books/@title" I> </hl>

U '

<table border= "1">

12

<tr>

13 :

<th>ISBN 코드＜/th>

14

<th＞서적＜/th>

15 '

<th＞저자＜/th>

16

<th＞출판사＜/th>

17

<th＞가격＜/th>

18 '
19

<th＞발간일＜/th>
</tㅍr>

士 伎鈿，
.t 9d-1
/-r0Ot 뇨，

20
21

</table>

22

<div><xsl:value- of select= "books/owner" I> <Idly>

23
24
25
26
27

</html>
<Ixs1:texnplate>

ch= "bo.:

「l
콰 Ir。k &'P)( 어한 依

<xs1乙f,or-each seiect=" ,

<l7,

]

<xsl : sort se1ect

0

}

===== PAGE 69 =====
68 =====
羽

order='ascending ' />
<xsl:sort selectr "pDate" data-type="text"
order= "descending" />

29

<tr>

"30

<td><xsl:value-of select=”균i삶)n " /><Itd>

31

<td><xsl:value-of eelect ="naiuo" /></td>

32 ;

<td><xsl:value-《娃 select ="author" f></td>

33

<td><xsl : value-of select ="publish" I></td>

34

<td><xsl : value-of select = "price" /></td>

35

<td><xsl = value-of select="pDate" /></td>

36

</tㅍr>

37

</xsl = for-each>

3.
</xsl : stylesheet>

2

새문서에 리스트2의 코드를입력하고, [D2］폴더에books.css라는이름으로저장한다
at스트2: books.css
body (background: *FFffFFn
hi {font-size:14pt; font-weight :bold;
th {font-size: l0pt;font-weight:bold;backgrourid:
*00ccff; line-height:15096;
td {font-size = 9pt; font-weight:normal;background:
#ffffcc;line-height: 15096}
div {font-size: 9pt; text-align:right; }

｀〕heck
055는 (Jascading Style Sheet의 약자로, ITI丕4L에 대해서 보다 세밀한 레이아웃을 지정하
고자할 경우에 이용합니다. cSS문서의 경우확장자는 '.css' 로합니다．

3 [D2〕폴더를열어bQOkS.XII1I을실행한다．

books.xml을 실행하면 관런된 XSLT 스타일 시트와 (ss스타일 시트에 의해 적용된 내용이 익스

===== PAGE 70 =====
69 =====
제2일 XSLㅜ 스타일 시트로 레이아웃하기

플로러상에 표시됩니다. 이번 스크립트에서는 앞의 Lesson에서 공백으로 되어 있던 테이블의 내용
을표시합니다．

1 템플릿어休 템욜릿을 부른다
앞의 Lesson에서 설명했던 것과 같이 XSLT는 템플릿의 집합체입니다. 단순한 스타일 시트라면
경로 요소에 적용되는 템플릿
（4- 24행）하나라도 충분하겠지만, 약간 복잡한 스타일 시트일 경우에
는 여러 개의 템플릿
（<xsl:temph扼）
）으로작성해야손쉽게 조작할수 있는 경우도 종종발생합니다．
예를들어, 이번의 경年옇횰촉흄玩이블의 반복부분을개별 템플릿으로조작하고 있습니다．
템플릿을 호출하는방법은 아래와 같습니다．
<xsl:apply-templates select= "'books " I>

" 凶은books.xmi의 (books> 요소에 대가여 뭔童蟹스：鑒쁘j三크：민입니다·
<xsl:apply-templates> 소의 select 속성의 books은 25행의 鈿i:template) 요소의 match 속
성으로 나타내는 books에 해당되며, 25- 38행에 정의된 일련의 템플릿을 참조합니다．
<xsl:template match="books">
</xsl template>

또한, 템플릿은 XSLT 스타일 시트 내부에 몇 개라도 기술할 수 있습니다. 템플릿 내부에 내포하
여 템플릿을 기술할수는 없지만, 템플릿에서 템플릿을 몇 번이라도 불러낼 수는 있습니다．
Q本 이 서신］

r. xsl = ann]v-temr,1

<xsl:apply-templates select="* " I>
"

" , ^, p

' ",/,-^7\

.／久／/\`7`－小，
一

<xsl츠empla놋match="多"
(name " 템플릿명" ]>
템플릿으로써 출력할 각종 요소, 스타일
<xsl 沈emplate>
<xsl= template> 요소는 <xsl : stylesheet> 요소 아래에 몇 개라도 기술할 수 있습니다．
<xsl : apply-templates> 요소의 select 속성과 <xsl= template> 요소의 match 속성에
는 각각 xPath식을 기술하여 서로 매치한 템플릿이 불려집니다．

===== PAGE 71 =====
70 =====
【非릿은 템플릿을 부른다｝

. .:. ---口 ' \esI:appIy-tempIate-;
sxsl.template , .
malcn= I 1

,`

select= booK)

`

q夕q,.，一．
*
→

템플릿은 변환
규칙의 집합

'

,^`J1.

``'~

1 珊J1｀
』｀`J

p/

match='bcok">

／〃－在F

\f

(xsl:appIy-tempIate
setect

memo 1

(xsl:template
match='memo")

현재 노드는 이동한다
<.xsl:apply-templates) 요소에서 다른 템플릿을호출할 경우주의해야할 점이 하나 있습니다．
（최상위 요소）
' 인 경우를 다뤄왔습니다. 그렇지만，
지금까지는 현재 노드가 항상 '경로 요소
<xsl:apply-templates> 요소에 의해 불려진 <xsl:template> 요소 아래에서의 현재 노드는 현재 템
플릿이 처리하고 있는대상의 요소로 이동합니다· 즉，
〈쩽뜨핀plate match='呼

，
텔퓰輞 경

우는 match 속정으로 지정되어 있는 <bQoks요촌가현괘少－드가 됩니다.

현재 노드는 이동한다
XSLT 스타일 시트는 처리중에 반드시 현재 위치를 나타내는 기점이 되는 현재 노드를 가집니다. xPath식으로 요소와
속성을 지정할 경우 반드시 이 현재 노드를 기점으로 하여 경로를 지정해야만 합니다．
따라서, 이 템플릿 내에서 (bcx水）요소의 isbn 속성을 표시할 경우도 <books> 요소를 기점으로 하고 있으므로 다음과
같이 작성합니다．
<xsl :va1ue-o
∼∼

//

select= 'book/@isbn" />

===== PAGE 72 =====
71 =====
제2일 ×SLT 스타일 시트로 레이아웃하기

또，
(book》요소 아래의 <title) 요소를 以 할 경우도 다음과 같습니다．
nV.＼七／\^^J

이와 같이 대상 노드까지의 경로
（path) 지정이 간소화되는 것도 템플릿화의 한 가지 목적이기도 합니다．

(xsl:template match='r
<xsl:apply-templatess seIect="books'/>
(IxsI:template)

(xsl.'template match= books
(xsl:for-each seIect='book")
(Jxsl:for-each>
(Jxsl:template)

(xsI:appty-tempIates)
요소와 (xsl:for-ead今
요소에서는 기점이 돠는
현재 노드가 이동한다．

테이블을 표시하고 싶다
鈿l:for-each) 요소는 select 속성으로 지정한요소의 내용을
<xsl:for-each select= thook">

</xsl : for-each>

26∼37행은 <books) 요소
（현재 노드）아래 기술된 모든 <book> 요소에 대해서 위에서부터 순서대
로반복처리합니다．
여기에서 <xs1:for-each) 요소는 1회의 루프로 (book) 요소를 테이블의 한 행
（<tr〉
태그）
에 출력하
고 있으며, 전체를반복 처리함으로써 하나의 테이블을구성합니다．

0

===== PAGE 73 =====
72 =====
[(xsl:for-each> 요소는 빈뼉된다】

1루프는 표의 한 행으로 출력

(xsl:for-each seIect=='book">
Ktr)
행의 내용
K/fr)
K/xsI:for-each)

하나의 요소가
표의 1행으로 변환

또한, 鈿i:for-each> 요소는 앞의 <xsl:apply-templates> 요소와 마찬가지로 현재 노드를 이동
시킵니다. 즉, 현재 템플릿의 기점은 <books> 요소이지만, <xsl:for-each> 요소에 의해 기점이 다시
아래 계층의 <book) 요소로 이동합니다．
따라서 鈿1:for-each> 요소 내에서 <book) 요소와isbn 속성을 표시할 경우는 <book) 요소를 기
점으로 하고 있으므로다음과같이 작성됩니다．
<td><xsl:value-of select= ''@Isbn" /></td>

또, <book> 요소 아래의 <name> 요소를 표시할 경우도 다음과 같이 작성됩니다．
<td><xsl:value-of select="naxue ' /></td>
【<xs1: for-each> 요소의 서식】
<xsl : for-each select= "xPath식, 매치돈l 요소와 속성에 대해서 반복 처리" >
루프 1회로 출력되는 내용
</xsl : for-each>

===== PAGE 74 =====
73 =====
제2임 ×S니 스타일 시트로 레이아웃하기

4 표의 Lㅐ돋；을 문자열로 정렬힌다
위의 <.xsl:for-each> -소만으로는 단지 X Th 문서에 쓰여진 내용을 순서대로 하나 하나 출력하

bb 1

..

.

.

..

"

-

..

.-

'ascending

-

.

'

I>

type

rder=

.

.

.

o

-

"text

<xsl: sort select= 'pu. b:Lish'.

data-

=;

;

기만합니다. 이것도 매우 편리한 기능이지만, 이것만으로는 뭔가부족한 것 같지 않습니까？
그래서, 여기에 한문장을추가하여 출력한표를 정렬해 보기로 합니다. books.xml의 27'-28행에
주목해 주집시오．

x5.L:sort seiect= 'pJJaㄷe' clata-type="text " oraer= "clescenaing" I>

鈿l:so武）요소는 <xsl:for-each) 요소에 의한출력 순서를 제어합니다．
data-type 속성은 데이터의 형태를, order 속성은 데이터를 오름차순
（ascending) · 내림차순
(descending) 중 어느 방식으로 출력할지를 지정합니다. 즉, 이 경우에는 27행의 코드로 XSLT는
<book> 소의 <publish> 요소를 오름차순으로 출력하고, 28행의 코드로 <pDate> 요소를 내림차순
으로출력합니다．
또 <xsl:sort> 요소를 여러 개 기술했을 경우에는 각 기술 순서대로 첫 번째 키, 두 번째 키가 되어
정렬됩니다．

口XSLT에서 css를 호출한다
앞의 Lesson에서 설명한 것과 같이｀그(SLT去 어디까지나 지금 작성한 XML 문서를 다른 형식의

문서
（예를들면 Imvm）
로 변환하기 위한기능에 지나지 않습니다· 보다鯉是題읫奚立프퀄흐L
횐：닌묘1 이 경우 I{rML에서
공뽄量多운멨뉼흐맨읜珪향ascathng Style Sheet) 읜：욜坐｝
cSS를 사용하는 것과 아주 똑같은방식으로 XSLT 내부에 (:SS의 호출을작성합니다. 예를 들면다
음과같습니다．
<iim< rel="stylesheet" type="text/cgs' href="books .css" />

<link〉
는 ITI刪I의 태그로, 현재 파일과 외부 파일의 관계를 나타냅니다. 각각의 rel 옵션은 href
속성으로 표시된 파일이 스타일 시트임을,type 속성은 그 스타일 시트가 (SS 스타일 시트임을나
타냅니다．
이 한 문장으로써 XSL'I뻬 의해 XML 문서를 변환한 후, 브라우저는다시 한 번(sS 스타일 시트
books.css를 적용하여 보다상세한 레이아웃을 적용할수 있습니다．

송

===== PAGE 75 =====
74 =====
[XSLT는 가공하고, css는 정리한다】
_

///

원래 ×M[ 문서

XSLT에 의해 HTML
변환된 ×ML

우선 XSLT에 의해
HTML 변환된 문서가
cSS에 의해
세밀한 레이아웃으로
정형화 된다．
cSS에 의해 정리된
마지막 출력

一

()
w

라 불리는 장치로도 실행할 수 있습니
XML 문서에 대한 스타일의 적용은 cSS가 아니라 F0(Formatting 아)jects）
다. 그러나 FO는 규격이 매우 크기도 하고 W3C에서도 아직 권고하지 않은 단계이므로 이 책에서는 더 이상 다루
지 않습니다．
XSLT와 FO를 합쳐 XSL(eXtensible St닌esheet Language）
이라 합니다．

-

`-

·XSLT 스타일 시트 내에는 여러 개의 템플릿을 포함시킬 수 있습니다，
· 템플릿 내에 템플릿을 기술할 수는 없지만, 한 템플릿에서 다른 템플릿을 호출할 수는 있습니다

咆얀appIy方mplates> 2송).
· 표나 리스트 같은 반복 항목을 출력할 경우는 <xsl:for-each) 요소 아래에서 현재 노드가 이동합니다
（노드를 지정할 때 주의합니다）
.
·<xsl:for-each> 요소에 의한 출력 순서를 제어하려면 (xs1:s0rt> 요소를 사용합니다．
.XSLT는 XML 문서를 HTML로 변환하기만 합니다. 보다 세밀한 레이아웃을 지정하고자 할 경우는
를 함께 사용합니다．
CSS(Cascading St닌e Sheet）

===== PAGE 76 =====
75 =====
제2일 ×SLㅜ 스타일 시트로 레이아웃하기

XML문서 music.xml을아래 그림과긷끼 표시합니다．
리스트내의 ①∼（亘：의공백을채우고, 올바른XML문서와XSLT스타일시트를완성시켜 주십시오．
i각곡가 리스트 냐1icro&ift Ir4ernet E: pIorer [旨

파일（F) 편집正） 面而r졸j膏飾i,－도구（T) 도움말（H)
긷뒤로 ,

3

1

仝

盈검색 스」즐겨찾기

=l口j x

.
" 연결 "

작곡가 리스트
요한 세바스찬 바하
1 시대 구분：바로크
2 탄샘밀＝1658-03-21
9 출생지＝독일
4 대표작：푸가b단조
루드비히 반 베토벤
1 시대 구분＝고전파
2. 탄생밀：1770-12-16
3' 출생지＝독밀
4 대표작＝ 교향곡 제 5변 문명
후리데릭 쇼팽
1 시대 구분＝냠만파
2. 탄샘밀＝1810-02-22
3; 출생지＝폴란드
4 대표작＝환상즉흠곡
클로드 드뷔시
1 시대 구분：민샴파
2 탄생밀＝1862-08-22
3 출생지＝ 프람스
뺑

댜J ㅠ 7가1 워 고

邕 완료

뇨，
; 나l 컴퓨El

music.xm!
<?xml version="l. 0 " encoding="EUC-KR" ?>
<?xml-style밟leet type="text/ xsl" href= "music .xsl " ?>
<music>
zmusician name=" 클로드 드뷔시" category=" 인상파"
birth='1862-08-22" countryr " 프랑스“ imp_work= " 월광“ />
<musician name='’요한 세바스찬 바하’' category= " 바로크’'
birth= "1658-03-21" country=“독일”imp work= "푸가 b단조" />
<musician name= ”루드비히 반 베토벤” category= ”고전파"
birth="1770-12-16" country=“독일" imp_work=" 교향곡 제 5번 운명" />
<musician name ＂후리데릭 쇼팽” category=" 낭만파＂ 三痲難懿蠱聽蜘小磁檎

===== PAGE 77 =====
76 =====
birth="1810-02-22" country= ”폴란드" irnp-work= "환상즉흥곡" />
<musician naxue= ”모리스 라벨「 category=" 근현대”
birth="1875-03-07 " country= "프랑스" ixnp_workr " 볼례로" />
</music>

music.xsl
<?xml version= "1.0" encoding= "EUC-KR" ?>
<xsl:stylesheet xrnlns:xsl="http: //www.w3.org/1999 /XSL/Transfonn''
version="1.0 ''>
<xsl:output [

]

encodirig= 'Euc-KR" I>

<xsl : template xnatch=" / '>
<html>
<head>
<title＞작곡가 리스트＜/title>
</head>
<body>
<hi＞작곡가 리스트＜/hi>
<dl>

[ I
<Id?>
</body>
</htiml>
</xsl : template>
<xsl:template [
[

I

>

]
[

I

<dt styie= 'font-size:ilpt; ">
[

I

</dt>
<dd style="font-size:l0pt; '>
<ol>
<li＞시대 구분 : <xsl:value-of select ="@-category" I><Ili>
<li>탄생일 : <xsl:value-of select =n@birth ' /></li>
<li>출생지 : <xsl:value-of select ='@country" /></li>

</

<li>대표F : <xsl:value-of select ="@imp work" /></li>
(:)1>

</dd>

===== PAGE 78 =====
77 =====
제2일 ×SLT 스타일 시트로 레이아웃하기

<hr I>
<Ixsl : for-each>
</xsl : template>
</xsl : stylesheet>

해답은 책 끝에 毫＞
`

/

Dr. XML과 나미의 원포인트 강좌

XSLT 예제가 나타나지 않아요！
나미

'박사님, 박사님！큰일났어외"

Dr.XML

' 뭔데, 뭔데, 뭐 때문에 그러나요？
（모처럼 낮잠 좀 자려는데···）"

나미

' 아까 배웠던 XSLT를 사용해서 ×ML을 표시해 보려고 했는데요, 그랬더니 보쎄요. 아무것도 표시되지 않았
'
어요. 뭔가 잘못됐는저 에러도 표시되지 않고, 도무지 모르겠어요．

Dr.XML

"응, 정확히 MSXML2은 설치했나요？"

나미

'‘물론이죠, 그렇게 간단한 건… MSXML' 모듈을 다운로드해서 더블 클릭하기만 하면 되잖아요？"

Dr.XML

（역시···）나미양, 그렇게 하면 XSLT는 움직이지 않아요．
"
"

나미

"네？ 왜 그렇죠？"

Dr.XML

"MSXML은 디폴트 상태로 설치됐을 경우, side by side 모드로 설치된다는 걸 잊었나요？"

나미

"OF! 그러고 보니까 오리엔테이션할 때에 그런 얘기가 있었는데... 뭐였지？'

Dr.XML

' 그래요. MSXML은 매일 매일 빠르게 발전 되기 때문
（게, 가끔 이전 버전과 호환성을 잃는 경우가 있어요.
그래서 side by side에서는 이전 버전의 기능을 남겨둔 상태에서 새로운 버전을 설치하는 방법을 취하는
거예요．
"

나미
Dr.XML

"그렇다면···"
"그래요, 이번에 나미양이 한 방법은 이전 버전의 MSXMLOI 우선시 되어서 새로운 ×SLT의 기능은 적용되
지 않는 거예요. xn洲nst.exe라는 프로그램을 사용하여 리플레이스 모드에서 설치해야만 하죠. 자, 한 번 더
오리엔테이션으로 돌아가서 노력해봐요．
"

나미

"네．
"

4

===== PAGE 79 =====
78 =====
，→∼

戚제2일XSLT

一∼끼b제2일xsL 스타입 시트로 레이Ok三
앞의 Lesson에서 작성한 리스트를 개선해 봅니다. 정렬 순서를 바꾸거나 각종 정보
로 링크를 작성합니다．
'

학습 내용 미리 보기

fl
壹H\'

Less。
n5
L 1 Q&a

和

J

꾜 소

烈감색 」」즐겨찾기

守UI[1

…∼出滋庶滋茁轟簪
J

－스，J

』＝」』切즈

只 =j 韜 뵤

면결 "

Web 관련 서적 목록
서…
저자
출판사
가격
발간일
ISBN 코드
樽진닷컴 11800 원 20미 06-1
SBNS9-314-什42-x HTML- 디자인 비주얼 가이드
c.I.S
ISBN89-314-1978-3 ASP사전
니시자와 나오키樽친닷컴 15000원泛001-11-30
IS8N89-314-2014-6!10일만에 배우는Visual C++ 6.0 Seto Haruka
영친닷컴 15000원2002-02-05 :
S8N89-314-l994-5 알짜 PC 용어 사전
슈와시스템
앙진닷캄 9500원 12002-01-05
Youngjin.com Y.

IiJㅗ

．…

臨XML

i 「v日b 관련 서적 목록 - Microsolt Internet EpIore蠱
（y) 즐겨찾기
（스） 도구（工） 도움맒
（ti玉
파일
（E) 편집（트＞ 보기

茴뫈료

…

…

낟lLㅐ컴퓨터

- 서적명에 링크가 연결되고，가격순으로 정렬되었다 -

앞의 Lesson도 복습 할겸 서적 목록을 수정해 보겠습니다．
아직 ×SLT의 개념에 익숙치 못하신 분은 다시 한 번 기본 구문을 확인하여 이번 ㄴesson의 내용을
기초로 여러 곳을 자기 나름대로 변경하1 봄으로써 확실히 이해하시기 바랍니다．

:

===== PAGE 80 =====
79 =====
제2암 XSLT 스타일 시트로 레이아웃하기

1

（books.xs1> -열어ㄷ梏리스트와같이코드를추
Lesson4에서작성한XSLT스타일시트
가 · 변경하고, 그대로 저장한다．
리스트 : books.x引

<?xml version="l. O " encoding= "EUC-KR" ?>
<xsl:stylesheet xmlns:xsl="http: //www.w3.org/1999/XSL/Transform"
version="l. O ">
<xsl : output method= 'html ' encoding= "EIJC-KR" I>
<xsl:template rnatch="/ ">
<html>
<head>
<title> <xsl:value-of se1ect' "books/@title" I></title>
<link rel= "stylesheet" type="textlcss ' href="books.css" I>
<Ihead>
<hl><xsl:value-of select='books/@title" /><Ihl>
<table border="l '>
<tr>
<th>ISBN 코드＜/th>
<th＞서적＜/th>
<th＞저자＜/th>
<th＞출판사＜/th>
<th＞가격＜/th>
<th>발간일＜/th>
</tr>
<xsl = apply-templates select= "books" I>
</table>
<div><xsl :value-of select= "books/owner" /></div>
</html>
</xsl : template>
<xsl:template match="books">
<xsl:for-each select="book">

===== PAGE 81 =====
80 =====
<tr>

28
29

<td nowrap="nowrap"><xsl:value-of select="@isbn" / ><,

30

.ztd nowrap= "nowrap" >

31

,.<xsl;e1einent 쁘些」
J?
<xsl:attributE
∼ 乙「 , =

32

八，
7＾

33

/

34 1

`

35

\

<jxsj.:attrjhiit '.,
<XSJ: va1ue∼of

36

</x8쟈e工emerltㅍ＞

37

1;=d>

</

→｀＝→／=\／∼

<xsl.
.va1ue-c
I>
se1ect= "pRm可

38

<td nowrap="riowrap"><xsl:value-of select ="author ' /></td>

39

<td nowrap="nowrap"><xsi:value-of select="publish" /></td>

40

<tㅍd riowrap= nowrap" >

41

<xsl : choose>
<xsl:when test= 'price[nuither( . ) &it; = 180001''>

42

<span style= 'font-weight:bold; " >

43

<xsl :value-of select="price" /> 원

44
45

</span>

46

</xsl n.hen>

47

<xsl = otherwise>
<xsl:value-of select="price" /> 원

48
49
50
5l.
52

</xsl:otherwise>
</xsl:choose>
</t,d>
<td nowrap= ''nowrap"><xsl:valuo-of select ="pDate" /></td>
<Itr>
</xsl : for-each>
</xsl : template>
</xsl: stylesheet>

[D2] 폴더를 열어 books.xiiJ을 실행한다．

===== PAGE 82 =====
81 =====
제2일 ×SLT 스타일 시트로 레이아웃하기

l ook&xn〕'을실행하면관련된 XSL'T꽈css에 의해H1용된내용끼 익스플로러상에 표시됩니다．
이 샘플에서는 정렬 순서가 바뀌고 서적명에 링크가 연결되며, 가격의 일부가굵은글씨로 표시되
는등의 변화를 확인할 수 있습니다．

1xs 는 정렬 기능을 깆춘다 - 수치 정렬
앞의 Lesson에서 다룬 鈿1:sort> 요소의 정렬 기능은 문자열에만 사용되는 것은 아닙니다．
1昱- -71
t!零고정렬도수치순으로처
data-type속성에number*坐f1 2솟 1 1,E1J01Er二Ar i리됩니다. 예를들어 27행을살펴봅시다．
<xsl:sort select= "price" data-type= "riuiriber" order= 'ascending' />

data-type 속정이 앞의 Lesson에서 지정했던 것처럼 text상태였을 경우, 1,000이나 50C따같은
수치는올바르게 정렬되지 않고, L000이 500보다작은＜肄로 정렬됩니다. 왜냐하면, 1,000과500
을문자열로 인식하여 우선 첫 번째의 1과 5가 비교되고 오름차순의 경우는1을 작은 것으로 인식하
여 먼저 출력해 버리기 때문입니다．
r ．∼口1 _ _._______
`<JLt5ㅗ = bUIㄴ＞

r` ㅅ '-"I ` 」人 ii
」i二亡＝ㅢ ＾γ긔I

<xsl:sort select=" 정렬할 대상의 요소, 속성을 나타내는 xPath식"

(data-type=" 데이턴혈(text ，
즈｝
뼛be社" ]
[order=" 정렬의 종류
（ascending：오름차순 - descending: 내림차순 "] />

2 調를 생성힌다
링크를 연결할 경우, 우선 <xsl:element> 요소로 HTMl꾀 <a> 태그를 생성할 필요가 있습니다．
졀而自荳自酉URL

<xsl:element> 요소아래의 <xsl:attribute> 요소로, 링크문자열은우리에게
익숙한 <xsl:vlue-of> 요소로 각각 출력합니다．
31-'36행을살펴보겠습니다．

0

===== PAGE 83 =====
82 =====
<xsl:element name="a'>
<xsl:attribute name='href''>
<xsl:value-of select="url" I>
</xsl:attribute>
<xsl:value-of select="name" I>
</xsl:element>

이 문장들은다음과 같은I{I取αL 문장으로 이해할수 있습니다．
r<a href='http: //www.youngjin.com"> HTM[』 디자인 비주얼 가이드＜Ia>

또, <xsl:element> -소는생략 가능하므로 이 경우는다음과같이 기술합니다．
<a>

<xsl:attribute name=''href">
<xsl:value-of select='url " I>
<Ixsl = attribute>
<xsl:value-of select= 1 name" />
<Ia>
r
1
`<X5L;

1

eiㅂ 1LL i1L>

^

人 r니

」＝〔＝:1ㅍㅋ

1」 ㅅ ,

AI'- 」

<xsl:element naxne= “요소명0>
요소 아래에 출력할 내용
</xsl = element>

,
^I 』JA1
뇨二亡ㅋ 八r긔」
r-

r
1
L<XSJ. = dㄴLLJjJuLe>

<xsl : attribute name= " 요소명" >
속성값이 되는 텍스트
</xsl : attribute>

조건별로 표시를 변경하고 싶다 - 조건 분기
여기에서는 18,000원 이하의 서적에 대해서 굵은 글씨로 표시해 봅시다. 서적 데이터가 '18,000
원이싱쏙l지 '18,000원 이하 인지에 의해 가격을굵은글씨로 처리할지의 여부를구분하게 됩니다．
이러한 조건 분기를 하고자 할 경우, XSLI뻬서는 2가지 방법을 제공하고 있는데 그 중의 하나인

令

===== PAGE 84 =====
83 =====
제2일 XSLㅜ 스타일 시트로 레이아웃하기

鈿l:ch&.』‘．요소에 의한분기를 예로들어 보기로 하겠습니다．
:cho月e> !ㅅ는 」 :`' ·

요소, 往sl:otherwise> ! ㅅ' 7 · ㅅ ！되며 令sl:when) -소의

扼st 속성에 지정한 조건이 일치했을 때에 내용을출력합니다. <x닢：湖ien> 요소는 여러 개 지정할 수
있고, 그 중의 어떤 것과도 일치하지 않을 경우아는 <xsl:otherwjse> 요소의 내용을출력합니다．
<xsl = choose>

첫걱

style= "fontweight: bold;
<xsl:value-of select="price" I> 원
">

<span

<xsl:when test= 'price [nuniber ( . 》 &lt; =18, 000]" >

첵万乙e 傘ot K·

</span>
</xsl :when>
<xsl : otherwise>
<xsl:value-of select="price" I> 원
<Ixs1:otherwise>
</xsl:choose>

test속성으로긴盧旦U늪크：앝껜뒝으브量린껸견굣坐蠟늦랄쇤－量曼二堆할수있습니다·
number(）
는 xPath 함수의 일종으로 괄호 안의 인수의 내용을 수치로 바꿉니다. 이 경우는 현재
요소0 즉, <price> 요소의 값을수치화하여 이것을18.QO과 비교합니다. 일반적으로 [number0囊
18,00(기으로 입력할 수도 있는데 XSLT 내에서는 '` cLess Than Equal)' 이라는 기술은 허용되지

`-'

'-

않으므로 '<' 를' 資坐l풋夔쁘蠟昱箕섶雹닌므·

'<' 와 ' >' 등은 XML, XSLT 등에서는 태그 구획 문자로써 공통적으로 채택되고 있는 예약 문자입니다. 이것을
XML에서는 시t; ,&gt; 라는 표현으로 기술함으로써 '<' 와 ' > ' 를 그대로 표시할 수 있습니다．이를 “이스케이프' 라
고 합니다．

===== PAGE 85 =====
84 =====
【파일 패턴의 구문】

price {number(.) &It;=3000]
기점이 되는 요소

r 一
＇^ 1 . '.11`

L` Ab. L 5 `J11`d'｀
』.口군

c AflI
O_ .L- -

비교 대상
（현재 요소 : <-）의
내용을 수치화한 것）

연산자
《∼ 이하）

L- AI1
"[ -IA

<xsl: choose>
<xsl:when test= "조건식“>
조건식에도 일치했을 때 출력할 내용
</xsl :when>.. .
[<xsl : otherwise>
어느 조건식에도 일치되지 않았을 때 출력할 내용
</xsl :otherwise>]
</xsl : choose>
<xsl :when> 요소는 <xsl:choose> 요소에 몇 개라도 기술할 수 있습니다．

xPam에서 사용희-'.- _Q스－ 여산ㅈ

可

（겨산자，
[1

파일 패턴

book[category= 'ASP']
(category) 요소가 ' ASP"인 <book> 요소

()

그룹핑

book[(author= Yamamoto" or author="Mochiduki") and category="XML']
<author) 요소가 \amamoto' 또는 ' Mochiduki"이며 (category) 요소가 'XML“인
book 요소

+

덧셈

number(price) + number(send)
(price) 요소에서 (send) 요소의 값을 더함

뺄셈

number(price) - number(send)
<price> 요소에서 <send> 요소의 값을 뺌

나눗셈

number(total) div number(number)
<total> 요소를 (number> 요소로 나눔

div

-

===== PAGE 86 =====
85 =====
제2일 XSLT 스타일 시트로 레이아웃하기

*

곱셈

number(price) * number(number)
<price> 요소를 (number) 요소로 곱함

mod

나머지

number(total) mod number(number)
<to轍）요소를 <number> 요소로 나눈 나머지

and

논리곱

book[url and logo]
<Um 요소와 <logo> 요소를 포함하는 (book) 요소

논리합

bookiurl or logo]
<un) 요소 또는 <logo> 요소를 포함하는 <book> 요소

not

부정

book[not(category=b(ML")]
<category> 요소가 b(ML' 이 아닌 <be아◇ 요소

같다

book[t万sbn=iSBN99-999"]
（) 요소
isbn 속성이 ' 1SBN99-999"인 <be아

느

같지 않다

book[@)isbn!=iSBN99-999"]
isbn 속성이 ' ISBN99-999' 가 아닌 <book) 요소

<

보다 작다

book[number(price)<18000]
아래의 (price> 요소가 18000 미만인 <book) 요소

이하

booktnumber(pnice)<=18000]
아래의 <price> 요소가 18000 이하인 <book> 요소

보다 크다

booktnumber(pnice))100001
아래의 (price> 요소가 10000보다 큰 (bo아) 요소

이상

booktnumber(price))=10000]
아래의 <price) 요소가 10000 이상인 <be아◇ 요소

결합

book/(chapten section)
<book) 요소 아래의 (chapter> 요소와 (section> 요소

<S

or

>==

)

1

xPatF，
의 용도는 단순히 노드로의 경로를 기술하는 것만은 아닙니다. 연산자와 함수 등을 병용하여 노드의 전반적인
내용을 얻을 수 있습니다．

속성값의 긴략형은 사용할 수 없다
XSLT 스타일 시트를 사용하면서 의외로 잊어 버리는 것이 XSLT도 )(ML 구문에 따라서 기술된
XML문서' 의 일종이라는사실입니다．
따라서 29행과긷끼 반드시 완전힌K생략되지 않은）형태로 기술해야 합니다．

自

===== PAGE 87 =====
86 =====
><xsl:value-of select="@isbn" />c/td> 難晷

<td

이 부분을항상fflvll
<td

기록하듯이

><xsl:value-of select="@isbn" I><Itd>

와같이 작성하면 에러가 발생합니다．
끄4L 작성시 주의했던 여러 가지 규칙도 의외로 XSLT을작성할 때 잊어버리는 경향이 있습니다．
다른 규칙을 포함하여 이번에 다시 한번생각해 보도록 합니다．
-

G. 化 XML
뿌
·(xsl:sort) 요소의 data-type 속성을 number로 지정하여 수치 데이터를 정렬하거나 처리할 수 있습니다．
· 링크를 생성하고자 할 경우0忙 (xsl:element) 요소, <xsl:attribute) 요소로 HTML의 <a> 태그를 출력합니다．
·XSLT는 반복 처리 외에 조건 분기의 기능을 갖습니다. 조건 분기에는 <xsl:choose> 요소를 사용합니다．
·XSLT 스타일 시트도 )<ML 문서입니다. XSLT 스타일 시트를 작성했을 때는 ×ML 구문과 연관된 내용을 다시
한번 확인합니다．

XH 문서 address.xml을 아래 그림과 같이 표시합니다. 리스트 ①∼⑤의 공백을 채우고, 새로운
XML 문서와XSLT 스타일 시트를 완성시켜 주십시오．
※ 단, 각각의 이름에는 각 사람의 메일 주소로 링크되도록 합니다．
Int=rn日t x
I주－록-∼ Mn,r1
r미n"r1 , ttflInt:rnet
M르 …
-=i미즈J
UF' (E) !t (트) 보기
（y) 퓰겨찾기(A) 도 " 口
, 斗 , i. －三勺 仝 슉검색 " 연결 "
ㅑ

연령
《기旨
주소
25세
갚다짚 서울시 강남구 논현동
25세
4감힝준서울시 도몽구창5동
！요祉희서울시 도봉구쌍문3동 25세
「툰쿠 제기2됨26세
좋은접 阿울시 동다
r」4 了 서울시 성동구 윽수2동 P7세
- ㅣ r已내 컴퓨E1

===== PAGE 88 =====
87 =====
제2임 ×SLT 스타일 시트로 레이아웃하기

address.xml
<?xml version= 'l. 0" encoding= "EUC-KR" ?>

[ ]

' /x「e "
《 " /,,4「－헨叭뇨枕 꿩？e=「枋，

<addressBook>
<mem(ber id="00003 ">
<name> 김미정＜/name>
<email>kongkong@youngjin. com</email>
<address＞서울시 강남구 논현동＜/address>
<old>25< /old>
</member>
<member id="00002">
<name> 김형준＜/name>
<emai1>dogotac(3hanmir .com<Iemaai1>
<address＞서울시 도봉구 창5동＜/address>
<old>2 5</old>
</member>
<member id="OOOOl">
<name＞홍은정＜/name>
<emnail>haruaki2 3@youngj in. com< /email>
<address＞서울시 동대문구 제기2동＜/address>
<old>2 6< /old>
</member>
<member id="00003 ">
汽二…

<name> 이동욱＜/name>

…

<email>d0ng297@hotmail .com</email>
<address＞서울시 성동구 옥수2누:/address>
<old>27</old>
</member>
<member id="00004 ">
<name＞유재홍＜/name>
<emnail>elfarternis@hanmail .net</emnail>
<address＞서울시 도봉 1 쌍문3昏/address>
<old>25</old>
</member>
</addressBook>

===== PAGE 89 =====
88 =====
address.xsl
<?xml version= "l.O " encoding="EUC-KR" ?>
<xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform"
version="l.O ">
<xsl:output method='html" encoding='EUC-KR" I>
<xsl:template match= " /'>
<html>
<head>
<title＞주소왁/title>
</head>
<body>
<table border= 'l ">
<tr><th＞이탉/ th><th＞주소＜/th><th＞연령＜/th></tr>
<xsl : for-each

[ ] >

〔

" `" ""I,벎츄； ,
，‘낑
,나秘，
（
麻

]

<tr>
<td nowrap

[ 1 >

<a>

<xsl : attribute naine= "bref">
[

1

</xsl : attribute>
<xsl:value-of select= "name" I>
<Ia>
<Itd>
<td><xsl:value-of select= "address" /></td>
<td><xsl:value-of select="old" />세＜/td>
</t=r>
< /x8l : for-each>
</table>
</body>
</html>
</xsl : template>
</xsl : stylesheet>

" """ "' " ’今J

"

"

"
`

0

===== PAGE 90 =====
89 =====
제2임 XSLT 스타일 시트로 레이아웃하기

G. to 지\IL

===== PAGE 91 =====
90 =====
Less。

包Less。

n6-

n7

XSLT에서
상세 정보 표시하기
계속해서 XSLT를학습합니다．
서적 정보 표시 화면을작성하면서 보다 다양한XSLT의 표현방법을배워 나갑니다．
XSLT와는 필수 불가분의 관계에 있는 xPath에 대해서도 사용할수 있는 구문의 폭을 조금씩 넓혀 가도
록하겠습니다．

===== PAGE 92 =====
91 =====
오늘 공부할 내용들
. 이미지 표시와 문장 장식하기
畛 조건 분기 ' 수치 정형으로보기좋게 나타내기

===== PAGE 93 =====
92 =====
제3일 x히J에서 상세 정보 표시하기

이미지 표시와 문장 장식하기
계속해서 XSLT를 학습합니다. 서적 목록 ><ML의 상세 정보를 표시해 봅니다．

학습 내용 미리 보기
L

b。
。k.xml

卜 b。。k2.
hdescr

css

a 끄 소 a겊색 스」즐겨찾기 횬卜미디머 길多 스，
J …／ 」 的 ！뵤

n.xsl
ipti。

상세 정보 표시

Lesson 6

m

XML
\

파압H) 편집娠） 보갸世） g겨찾기
（匈 도구
（끄 도움말
（비

긷뒤로 , ．好

∼》
→
L「너
뇨닢 Q&
（】
ㄴ

O [ S l [; N
∼二1色

01. HTML 디자인 비주얼 가이드 (cJs)
HTh 태그를 쉽게 이해할 수 있도록 설뎡한 책이다 이 책은 크게 세 가지
부분으로 구성되어 있다 첫 번째는 Tut.nal편으로 m그）
姃L의 기초를 알기 쉽
게 설명했다 두 번째는 Reference와 practC. 편이다 여기에서는 튜토리얼 편
에서 제출한 mldI』
의 기몬적인 기능에서 나아가 응용 심화 학습을 할 수 있
도쪽 하였다 세 번째는 Step UP 편이다
11800원

02, ASP 사전（니시자와 나오키）
A8P의 모든 명령을 내 포캣속에 Poket Reference ASP 사전은 ^SP의 기몬
적인 지식과 사용 가능한 명령의 구문, 구문에 대한 상세한 설명, 명령 활용
예츌 ASP 오브젝트, ADO. FOeSystemObject의 메소드, 프로퍼티로 분류하여
언제든지 쉽게 찾아 참조할 수 있도록 한 사전식 레퍼런스입니다
15000원

七훈；LH 컴再터

서적 목록 ×ML의 상세 정보를 세로로 열거한다

：●Key Point ) _
제 2일과는 전혀 다른 출력 방법을 학습합니다．
XML- XSLT는 스타일 시트의 조작만으로도 간단하게 표시 형식을 변경할 수 있도록 문서 구조 작
성 방식과 문서 장식 방식을 분리했습니다. 지금까지 문자상으로만 이해해온 XML의 특성를 직접 확
인해 봅시다．

4

===== PAGE 94 =====
93 =====
재3얻 ×SLㅜ에서 상세 정보 표시하기

※부록CD-ROM의[Lesson 6] 폴더에 있는 html.jpg, aspjpg, x.jpg를［田］폴더에 복사해 주십시오．

제 2일에 ㅅ陪한 books.x祉을 열어 리스트 1의 코드를 추가 · 변경하여〔D3] 폴더에
books.xml이라고 저장한다．
리스트1 ; books.xml
<?,anl version="l. 0 " encoding= 'ETJC-KR" ?>
:，ㅗㄷ＝ㅗ

u＝口cription.xsl " ?>

<books title= ”웹 관련 서적 목록“>
<owner adclress= "www.youngjin.com" >Youngjin.com
5

<book isbn="ISBN89-314-1742-x ">

6

<name>HTMt』 디자인 비주얼 가이드＜/nanie>

7

<author>C.I. S</author>

8
9

<category>HTML</category>
<url>http: IIww. youngjin.com <furl>
<price>11800</price>
<publish>영진닷컴＜/publish>
<pDate>2001-06-ll< /pDate>

15

</book>

16

<book isbn= 'ISBN89-314-1978-3 ">

17

<name>ASP 사전＜/name>

18

<author＞니시자와 나오키＜/author>

19
20
21

<category>ASP< /category>
<url>http: IIwww.youngjin.com <Iur1>
<price>15000</price>
<publish＞영진닷컴＜/publish>

Y.

1

</owner>

===== PAGE 95 =====
94 =====
<pDate>2001-ll-30</pDate>
25

∼ 경령을 내 포켓속에 </keyword>

' Poket

Reference ASP 사전은 ASP의 기본적인 지식과 사용 가능한 명령의 구문, 구문에 대한
상세한 설명, 명령 활용 예를 ASP 오브젝트, ADO, FilesystemObject의 메소드, 프로퍼
셉ㅋ 느크끄二Lrt C- rI亡rt 스hJ!

아 차t하 수 있도록 한 사전식 레퍼런스입니다．
</mertK)>

</book>
<book isbn="ISBN89-314-1994-5">
<name＞알짜 PC 용어 사전＜/name>
<author＞슈와시스템＜/author>
<category＞컴퓨터 사전＜/category>
<price>19500</price>
<publish＞영진닷컴＜/publish>
<pDate>2002-01-05</pDate>
lr媤工nO＞이 도서의 특징은 줄임말
（약어）
에서 풀네임을 찾거나 풀네임에서 줄임말을 쉽게 찾을
: 있도록 도와준다．
二한 삽화를 통해서 이해하기 어렵거나 생소한 용어에 대해서 이해도를 높이고 있다.</xnemo>
</book>

:,

<book isbn="ISBN89-314-2014-5'>
<name>10일만에 배우는 Visual C++ 6.0</name>

.

<author>Seto Haruka</author>

39
40
41

<url>http: //www.yourigjin.com </url>

42

<category>Visual C++< /category>

43

<price>15000< /price>

44

<publish>영진닷컴＜/publish>

45

</pDate>2002-02-05< /pDate>

,46

C++ 6.0에 대해 22개의 단원을 10일 동안 순서
대로 학습하도록 되어 있다．
Lessoni에서는 간단한 Windows 프르그램을 직접 만들어 봄으로쩌 앞으르 펴궉직 r기 무궁무진함을
맛보게 한다. Lesson2부터는 직접 Visual C+＋을 실행하고, 소스를 분석하면서 언어의 기
본적인 개념을 잡아 나가고, 마지막 Lesson22에서는 이미 습득한 API 함수 사용법, 리소스
l성법 등을 이용해 Windows 응용 프로그램을 독자 스스로 코딩할 수 있게 한다＜/n훰으r:,O>

,
4'

t

</book>
</books>

===== PAGE 96 =====
95 =====
제3일 XSLT에서 상세 정보 표시하기

새문서를열어 리스트2의 코드를입력하고, [D3］폴더에 description.xsl이라는이름으로
저장한다．
리스트 2 : descrip嫩)fl.X引
<?xml version="l. 0 ' encoding= 'EUC- KR" ?>
xmlns:xsl= 나노ttp = / Iv댔i,.w3 . org/1999 /XSL/Transform"

<xsl : stylesheet
version= " 1. 0 ">

<xsl template match= "I ">
<html>
<head>
<title＞상세 정보 표시＜/title>
<link rel＝二"stylesheet " type="text/css" href="book2.css"' I>
</head>
<body>
<hl＞상세 정보 표시＜/hl>
<xsl:apply-templates select="books " />

戶" : …

A,

r ' … ' ”『

</body>
</html>
</xsl : template>
<! -－이상, 경로 요소에 적용되는 템플릿 -->
<xsl:template niatch="books">
<xsl:for-each select="book">
<table border="0">

<tr> 츳：
卜 t!
, width=

"p1
"

150

">

name= "
<xsl : elemenE ;J.

孕t.

6’肖 ＜「'urc→

">
）두끼e`

img

프

<td

2

<xsl:attribute name="src">

<dl>
, 口’

<dt>

祭n의

<xsl:nuinber iformat="0l " />.
<xsl:value-of select="name" I>

,
i

</t=d>
<td valign="bottom">

！

·1

<xsl:attribute name="height">150 </xsl:attribute>
<Ixsl :element>

J
＂났

나口瑾＝; 시艸 qr乞n

<xsl :attribute name="width">120 </xsl:attribute>

m

</xsl : attribute>

결

1沚m

<xsl:value-of select="logo" I>
1``／才咬휄

汭

===== PAGE 97 =====
96 =====
(<xsl:value-of select="author' I>)
</dt>
<dd>

^ i즈＝1

의아
<xsl : apply-templates select= "nienk〕") I>
<br I>

/"'

"'蒜갸；,：魅

<div style="text-align:right; ">
<xsl:value-of select='price" I>원
</div>
</dd>
</dl>
<Itd>
</tㅍr>
</table>
<hr />
</xsl: for-each>
<Ixsl: template>
긴．-－이상＇ <books＞요소에 적용되는 템플릿－->
「>
<xsl:template match="keyword
<span style=" font-weight :bold; " >
<xsl:value-of select=". " I>
<Ispan>
</xsl : template>
<! -－이상， <keyword＞요소에 적용되는 템플릿－->
<xsl:template niatch= 'textO ">

<xsl:value-of select=·，'." I> 毛잭 R요귈 뇬H섶．
</xsl :template>
<!-－이상, 텍스트를 출력하기 위한 템플릿 -->
</xsl : stylesheet>

3

새문서를열어리스트3의코드를입력하고，
[D3］폴더에book2.css라는이름으로저장한다．
리스트 3 : book2.css
body {background: #FFf fFF사
hl{font-size:14pt;}
dt {font-size: llpt; font-weight :bold;color: *0080FF;
line-height:14pt;}
dd{font-size:9pt;color:#556B2F;line-height:9pt;}

===== PAGE 98 =====
97 =====
제3임 XSLT에서 상세 정보 표시하기

books.xi교에서는 XSLT 스타일 시트 description.xsl과 (Jss 스타일 시트 bookacss가 적용되어
상세 정보 목록이 표시됩니다. 이 때 하나의 그림이 깨져 있지만, 신경쓰지 마십시오. 이 부분에 대
해서는다음Lesson에서 처리 방법을 생각해 봅니다．
1 description.xsl의 전체 구성
개개의 세세한 명령을 보기 전에 우선 전체 내용을 파악해 보기로 합시다. description.xsl은 아래
의 4개의 템플릿으로 이루어져 있습니다．

n얏 ∼ …驪

3 '-'14행

경로 요소에 적용되는 템플릿．
출력될 HTML의 골격을 생성합니다．

16"- 49행

(books) 요소에 적용되는 템플릿．
篇밟驪봇읫鷺鼻寺專흇薑합니다．

51'-55행

(memo) 요소 아래의 (keyword> 요소에 적용되는 템플릿．
텍스트를 굵은 글씨로 변경한다．

57,-59행

(memo> 요소 아래의 평문 텍스트에 적용되는 템플릿．
텍스트를 그대로 표시하기만 합니다．

여기에서 나타낸 것은 각 템플릿의 역할뿐이지만, 우선 개요를 이해하는 것이 매우 중요합니다．
앞으로 복잡한 소스가 또 나오겠지만, 이럴｛대는 처음부터 한 행 한 행 검토하기보다는 전체를 블록 '
단위나 의미단위로 파악하면보다 이해하기 쉬워질 것입니다．

2 그림을 표시하고 싶다
books.xml의 요소를 ffl 로 변환하여 그림을 표시하여 봅니다. 예를 들어 다음과 같은 FfML
을작성합니다．
브.mg,src=
. " … ' 봇愍농＝프므스갱感얀欠只챘二／>
description.xsl의 21- 27행을봅시다．
그림을 표시한다고 해도 새로운 것은 없고, 앞의 Lesson에서 학습한 링크 생성과 거의 변함이 없
습니다．

===== PAGE 99 =====
98 =====
<xsl:elemerit name= " img" >
<xsl:attribute name="src">
<xsl:value-of select= " logo" I>
</xsl:attribute>
<xsl:attribute naine='width' >120</xsl:attribute>
<xsl:attribute name="height'>150</xsl:attribute>
</xsl:element>

<xsl:attribute> 요소로 src 속성을 정의하고, books.xml의 <logo) 요소의 내용을 입력합니다．
books.xml 내에는 <logo> 요소가공백으로 되어 있기 때문에 지금은 어느 부분에서 깨진 그림이 표
시되는데 이 경우의 처리 방법에 대해서는 뒤의 Lesson으로 다룹니다．
이 예와긷히 요소가 포함되는 속정이 여러 개 존재할 경우에는 <xsl:attribute> 요소를 여러 개 기
술할수도 있습니다．
3 문서의 일부를 강조해서 표시하고 싶다
지금까지는 구조적인 XML 문서를 다뤄왔지만, XML 문서의 장점 중 하나는 비정형적인 문서에
대해서도 유연한 접근이 허락된다는 점입니다. 예를 들면, 비정형 문서 내의 일부분만 이탤릭쳬로
표시해보거나 링크를 연결하는 제어가XSL'T뻬서는 가능한 것입니다．
이 예로써 텍스트 내의 <keyword> 요소로둘러싸인 부분만 진하게 표시해 봅니다．
지금까지는 하나의 <apply-templates> 요소가 하나의 <xsl:template> -소를 호출하는 경우가
대부분이었습니다
（부르는 쪽과 불려지는 쪽이 1대 D. 이번에는 하나의 부르는 쪽에 대해서 2개의
템플릿이 불려집니다. 익숙하지 않은 사람에게는 약간 이해하기 어려운 기술 방법이므로 주의하도
록합시다.
우선 2번째 템플릿 내의 37행에는 b00kS.XIIil의 <memo) 요소에 대하여 대응하는 템플릿을 적용
하라는 문장을 기술하고 있습니다．
<xsl:apply-templates select="memo" I>

지금까지의 예로 보면 鈿1:templates match="memd'〉로 시작하는 템플릿이 준비되어야 하지

만，o]1에는존재가지 않습니다· 饌，
<memo> a솟엣므好크트브荳렇안쓰a姓앗塗涎는
<memo) 요소의 데이터인 텍스트와 <memo> 요소의 하위 요소인 <keyword> 요소 각감의］
雜최되는

毁斐尺：上쁘요닷·
이로써 지금까지와같은특정 요소를 처리하는 것이 아니라, 텍스트와요소가 섞인문맥이라도 적
당히 매치하여 처리할수 있게 됩니다．

===== PAGE 100 =====
99 =====
제3일 ×SLT에서 상세 정보 표시하기

(1) (keyword> 요소의 위치
51 t <xsl: teniplate nratch="keyword" >
57

<span style="font-weight :bold; " >

r.1

<xsl: value-of select=" . " I>

5'

<Ispan>

55 : </xsl: template>

<keyword> 요소에 매지되고 <keyword) 요소로 둘러싸인 부분을 굵은 글씨로 지정하여 출
력합니다．

(memo)
Windows2.O/NT4.O/98/95에서 사용할 수 있는 서버측
- (keyword>ActiveServerPages(Ikeyword)3.O,
풍부하게 준비된 추가 콤포넌트와 Accsee, SQL Server로 대표돠는 데이
터베이스와의 연동에 의해 강력한 웹 애플리케이션을 구축할 수 있게 합니■
다．
(/memo)
텍스트는 여기에서 처리
<xsl:texnplate match= "keyword">

exal : template math= 노ext ( ) 1' >
… 중략 …

… 중략 …

</xsl : template>

</xsl: template>

Windows2.O/NT4.O/98/95에서 사용할 수 있는 서버측 가술
<span style =tont-weight:boId;")Actve ServerPages(Ispan) 풍부
하게 준비된 추가 콤포넌트와 Accsee, SQL Server로 대표되는 데이터베
이스와의 연동에 의해 강력한 웹 애플리케이션을 구축할 수 있게 합니다．

(2) 텍스트의 위치
<xsl = template xnatch="text ( 》" >
<xsl:value-of select=". " I>
</xsl : template>

===== PAGE 101 =====
100 =====
吟빻트致史읜長숯望푠曾하나로，match속성값으로／陪하면텍스트에매치됩니다．텍
memo>
'는<
'叫

'만씨

설

의텍뜨

.

-

7]

［르손률

1 FL]

'刻

“

'

"부분叫

은

.

“

tI-

LfEfflt

'. '

a

스트는 <xsl:value-of) 요소를 이용하여 어떠한 변경도 하지 않고 그대로 출력합니다．

그 외에 아래와같은표현이 갖춰져 있습니다．

富

-

comment( )

주석 노드에 매치

node( )

모든 종류의 노드에 매치

processing-instruction( )

처리 명령 노드에 매치

4 표에 澣적인 번호를 부가하고 싶다
XSL']뻬서는반복처리 루프 내에 연속적인번호를붙일수가 있습니다. 예를들어 32행을봅시다．
<xs1,:nunber format="01" /＞·

format 속성은출력할 연속 번호의 종류缸, 렉 01등）
를 지정합니다．
r J`k' 1 . "` ``,，ㄴ＾｀∼

(

L` ^.』＝ &LSUS1UJtL 7

ACI l JAIl

n.rs .r- "I '-91

<xsl:nuither [level=" 넘버링의 레벨"〕
(count=" 카운드할 대상의 요소와 속성을 특정하기 위한 xPath식"〕
[from= "XML』 문서 상에서는 형제 관계에 있지만, 넘버링에 있어서는
친자 관계를 갖는 노드0ㅔ 대해서 어디에서부터 카운트를 시작할지를 지정"]
[for切
［at=" 넘버링의 출력 형식" 〕 />

level속성의 설정값은 아래와같습니다．

==sin이e
m미h이e
any

m

'

…

-

' →「

"

'

-

心

·
．곯꿩뻔l,3｛毓농등치든쏀론是쁘한대디풀트）
V형제，
브샌嶝을 부가한 것·
브쁘oI엣분몬놋등C윗2I，
촁qg塢尺璧멨읜헨囊련됫늪，
count 속성으로 지정된 식에 매치된 순서대로 넘버링한다．

'

===== PAGE 102 =====
101 =====
제3일 ×SLT(게서 상세 정보 표시하기

-

Go to XML
러 개 갖는 요소를생성할 경우는 <xsl:attribute> 요소를 여러 개 기술할 수 있습니다．
불러내는 곳과 불려지는 곳이 반드시 1[fl 1로 한정되지는 않습니다．
·XSLT로 연속적인 번호를 달기 위해서는 <xsl:number> 요소를 사용합니다．

아래의 xML 문서 article.xml과 XSLT 스타일 시트 table.xsl을 기초로, 다음 그림과 같은 레이아웃
을출력해 봅니다. 올바른XSLT 스타일 시트가 되도록공백 부분을 적절한값으로채우기 바랍니다．
※ 주의 : name( ）은 xPath 함수의 하나로 현재 요소의 요소명을 나타냅니다．
｀기사 묵차 - Micros篩 nts,net Ecpkrre尹呼ㅉ
（D 도욤밀던）
파일
（D 편집t) 보기
（Y) i기찾기
（d) 도구
中뒤로 ' .9

3 」〕소

省

q검색 」d퓰겨찾가 송미口머 ,J " 연’ 月
j

1개요
1.1 XML이란 무엇인가？
Y.Yamada
1.2 HThILJSGML의 비교
N十(.akeya
2XML 문서륜 기술에 보자
2.1 XML 문서의 선언
V. Yamada
2.2 유일한 제 1 요소휼 가질 것
M.Mochiduk]
3「간행 서적 일람J 올 표시해 보자
3.1 XML 문서에서 ×SL올 불러낸다
K.Usui
3.2XSL 스타일 시트플 선언한다
HS敬a)
4 r서적 상세 정보.1 휼 표시에 보차
4.1 표휼 표시하고 싶다
（일자 정렬）
T.Kaneko
4.2 문서에 일 부분율 강조 표시하고 싶다
V. Vamada
階퇀菖

J

닙ㅍ 내 컴퓨日

<?xml version="l. 0 ' encoding= "ETJC-KR' standalone ="yes" ?>L"'一啣*七" '
<?xml-stylesheet type="text/ xsl " href='table. xsl " ?>
<article>
<chapter title= " 개요" >
<section tit1e='' 꼬4I』
이란 무엇인가？'' author="Y.Yaxnada ' chr="4500''>

===== PAGE 103 =====
102 =====
<P＞한마디로 말하면 XML이란「정보 기술 언어」
입니다.
（후략）</p>
</section>
<section tit1e=「HTML/SG1 ,의 HI교" author="N.Kakeya"chr="9000"
<p＞여기에서는 XML의 특성을 기존의 SGML (Standard Generaiiaed Markup
Language) /HTML고f 비교하면서, 좀 더 명확히 x14L의 장점을 개관해 봅시다.（후략）</p>
</section>
</chapter>
<cha鮮er titie= "XMI』 문서를 기술해 보자">
<section titie= "XML 문서의 선언" author="Y.Yamada" chr="950">
?&gt; 선언을 기술 해야만 합니다.（후략）

</p>

<p>XML 문서의 1행째에는 반드시 &it尸xml
</section>

<section titie= '’유일한 제 1 요소를 갖을 것’' author= 'M.Mochiduki">
<p>XMI』 문서의 최상위에는 반드시 경로 요소가 있어야 합니다．
경로 요소는 제 1요소, 최상위 요소라 불리는 경우도 있고,（후략）
</p>
</section>
</chapter>
<chapter titie= "「간행 서적 일람」
을 표시해 보자“>
<section title= "XMI』 문서에서 XsI』
을 불러낸다＂ author="K.tlsui" chr="1035">
<p>XSL을 사용하기 위해서도 우선 원래 XI』운서와 XsI』스타일 시트를
관련 지어야만 합니다．
（후략）</p>
</ section>
<section titie= "XSL 스타일 시트를 선언한다'' author="H.Sakai" clir="890">
<p＞경로 요소 &it; xsi : styiesheet&gt; 의 xmlns = xsi 속성은 xsi: ∼로 시작하는
각 요소가 어느 ㅁ〕［크〕
（문서 규칙）
에 따르는지를 정의한 것입니다．
（후략）</p>
</ section>
</chapter>
<chapter titie= "「서적 상세 정보」
를 표시해 보자“>
<section titie= "표를 표시하고 싶다
（일자 정렬）
" author ="T.Kaiieko" 아끄r= "650">
<p＞표 등 반복되는 부분을 출력하기 위해 &it; xsi : for-each&gt;
요소를 사용하는 것은 TIPSi2에서 소개한 바와 같습니다.
（후략）</r)>
</ section>
<section titie= " 문서에 일부분을 강조 표시하고 싶다'' author="Y.Yamada"
chr="500">

</p>

<p＞사고법으로서는 조금 전의 링크 표시와 아주 똑같습니다.（후략）
<Isection>

===== PAGE 104 =====
103 =====
제3일 XSLT에서 상세 정보 표시하기

</chapter>
</article>

ta톄e.xsl
<?xml version="l. 0 ' encoding= "EUC-KR" staridalone="yes" ?>
<xsl:stylesheet mti1ns:xsl="http: //www.w3.org/1999/XSL/Transform"
version="l. O ">
<xsl:output method="html" encoding= "EtJC-KR" I>
<xsl:template [

I >

<html>
<head>
<title＞기사 목차＜/title>
</head>
<body>
<xsl:element nanie="table">
<xsl:apply-templates select="article " I>
</xsl : element>
</body>
</html>
</xsl 六:emplate>
<xsl:template [

] >

<xsl:for-each select=" [

] ">

<tr>

ct'

<xsl:when test="naxneO='chapter ' ">
<td colspan="2 " style="font-size:12pt;

∼

background: #ffeeaa; font-weight :bold; '>
……

<xsl:value-of select= "@title " I>
</t：ㅍd>
<Ixsl :when>
<xsl :otherwise>
<td>
<xsl:value-of select= "@title " I>
<br I>

겯

<xsl: value-of select= "@author" I>

103

'1

『1m

</th>
<xsl : choose>

]

《

" foririat="l " count=" [

‘미C

I

1

<xsl:number level=" [

I>

<th align="right " valign="top">
t

===== PAGE 105 =====
104 =====
</td>
</xsl:otherwise>
</xsl:choose>
</t；ㅍr>
</xsl: for-each>
</xsl : template>
</xsl: stylesheet>

4581

Ic

Dr.XML과 나미의 원포인트 강좌

XMl－은 HTML이 진화된 것이다？
나미
Dr.XML

' 이렇게 보니 역시 ×ML은 HTML의 규칙을 좀 더 엄격히 한 것으로만 보이네요"
' 뭐, 문법적으로는 나미양이 말한 대롭니다. 그러나 나미양은 오리엔테이션에서 이야기한 ×ML의 가장 중요
한 특징을 잊고 있진 않나요？"

나미
Dr.XML

"네. XML은 자유롭게 태그를 정할 수 있어서．
..'
'아직 잊지는 않은 것 같군요. 말 그대로 XML에서는 자신이 사용할 태그를 자유롭게 정의할 수 있습니다．
바꿔 말하면 HTML에서는 그렇게 많던 태그가 ×ML에서는 하나도 존재하지 않습니다. 다만, 태그를 기술하
기 위한 규칙만이 정해져 있습니다. 이것만으로도 복잡한 XML인데, 실제로 W30으로부터 제시되고 있는 사
양서라는 것은 A4 용지로, 불과 20여 페이지에 지나지 않습니다.'

나미

' 음··· 그렇다면 자.lL이란 HTML의 축소판인가요？"

Dr.XML

"아직, 나미양은 HTML 대 XML의 서식에 사로잡혀 있진 않은지… 굳이 말하자면, XML은 HTML을 좀 더
범용화한 언어라고 말할 수 있을지도 모릅니다, XML이 자유롭게 태그를 정할 수 있다는 점은 >m4L로
HTML을 기술해도 좋다는 얘기입니다. 덧붙여 말하면, XML의 규칙에 따라서 종래의 HTML을 수정하고자
"
하는 것은 결코 새로운 시도가 아니며, 이미 HTML이라는 형태로 그것이 실현되고 있습니다．

나미

' 그렇군요. 지금까지는 XML이 HTML에 겹쳐서 들렸는데, 그런 얘기를 들으니 뭔가 데이터베이스처럼 들려
요．
"

Dr.XML

"확실히 데이터를 넣는 기구를 제공한다는 의미에서는 XML의 개념이 데이터베이스로 연결된다고 해도 그
다지 이상하지는 않습니다. 나미양도 이제 알게 된 것 같군요. 다음 수업을 알리는 종이 울리고 있네요 늦으
면 안 되는데… 가죠, 나미양."

===== PAGE 106 =====
105 =====
Go to XML

===== PAGE 107 =====
106 =====
제3일 XSLT에서 상11 졍보 표시하기

조건 분기 · 수치 정형으로 보기좋게 나타내기
앞의 Lesson에 이어서 화면을 좀 더 멋지게 표현해 봅시다．

'

학습 내용 미리 보기
xsl

lptlon.

ㄱdescr

-

e恥畔·－一
파일（E>

XML
=\Z

(j

卞뒤로 …

=

J

. ..

-

편집（트） 보기
（y) 츌겨찾기（스） 도구（T>
‘〕소

도웅말
（H)

功검색 ＝」즐겨찾기 沙미디머 J

- j.I x
日

心，i

；」④ tf

연글 "
比800원 스

Lesson 7

-

=

,

02 ASP 사전（니시자와 I "=＞규l,

L fl Q&a

착쩐
r→
7크＝

. 스何
塗：夔"4
?4m

業쁩? 螂i 서적일람×ML의내용이HTML의테이블로」 匡l다
명령 활용 예룔 ASP 오브젝트. ADO, PileSystemObject의 메소드．
프로퍼 囊
티로 분류하여 언제든지 쉽게 찾아 참조할 수 있도폭 한 사전식 레퍼런 珊
스입니다■
瓮
15.000원
艇

뿔

03 알짜 PC 용어 사전（슈와시스템）
이 도서의 특징은 즐임말
（약어）
에서 풀네임을 찾거나 푿네임에서 줄임
말을 쉽게 찾을 수 있도폭 도와준다 또한 삽화튤 뿡해서 이해하기 0{
렵거나 생소한 용어에 대해서 이해도를 높이고 있다；
19.500원
-

: …
：好叫驪
眄藝萱

包

04 10일만에 배우는 Visual O4-I- 6.0 (S
이 책은 Mscrosoft Jisua1 C卄 60 ` 링크가 생성된다 1일 동안 순서
대로 학습하도폭 되어 있다．
Lessoni '
= ._ ._므 Windows 프로그램을
직섭 만들어 봄으로써 앞으로 펼쳐질 이 책의 무궁무진함을 맛보게 한 二
ㄴ－3Lㅐ 컴퓨터

：夕 Key Point ) _
분기 명령인 <xsllf) 요소와 수치 데이터를 뫼용으로 가공하는 format-number 함수 등 새로운
내용이 소개됩니다. 이것은 자금까지 학습의 연장선에 지나지 않습니다. 이 새로 나온 키워드들을 레
퍼런스 등으로 확인하면서 자신의 힘으로 코드를 기술해 봅시다．
처음에는 시간이 걸릴지 모르지만, 자신의 힘으로 만든 것은 또 다른 시점에서의 발견으로 연결됩
니다．

===== PAGE 108 =====
107 =====
제3임 ×SLT에서 상세 정보 표시하기

실전！코드 조작
]

Lesson6에서작성한［D3〕폴더에저장된XSLT스타일시트description.xsl를메모징꼐서
열어 리스트의 코드를추가하고, 같은 이름으로 저장한다．
리스트 : description.x引
<?xml version="1. 0 " encoding= "EUC-KR" ?>
<xsl = stylesheet xmlns:xsl="http: //www.w3 .org/1999/XSL/Transform"
version="1.0'>
<xsl : template match= " /">
<html>
<head>
<title＞상세 정보 표시＜/title>
<link rel="styiesheet" type="textlcss" href="book2.css" I>
</head>
<b
《Jdy>
<hi＞상세 정보 표시＜/hl>
1노

<xsl:apply-templates select="books" I>

12

</body>

13

</htnu>

14

</xsl : template>

:1

<xsl:template match="books">

16

<xsl : for-each select= 'book'>

17

<table border= "0">

18

<tr>

19

<td width="lSO ">

…
=＝…

20

，느 ,

i ，…

1

lDg0〔 , ! = " ] ">

<xsl:element name=「1mg" >
<xsl : attribute name= " src" >
<xsl:value-of selectz "iogo"
24

</xsl : attribute>

25

<xsl:attribute name= "width">120
</xsl : attribute>
<xsl:attribute name="height">l50
</xsl:attribute>

빠
／
^
,
R
匕

＾

</xsl : element>
<Ixsl: if>

===== PAGE 109 =====
108 =====
29

</td>

30

<td valign="bottom">
<dl>

31

<dt>

32
33

<xsl:number format= "0l" I>.

34

<xsl:value-of select="name" I>
(<xsl:value-of select="author" I>)

35
36

< /dtㅍ＞

37

<dd>

38

<xsl :apply-templates select= 'memo" I>

39

<br I>

40

<div style="text-align:right; ">

41

<xsl :value-of select= 'format-number
(price, '#,###' ) " />원

42

</div>
<Idd>

43
44
45

</d1>
</td>

46

</tr>

47

</table>

48

<hr />

49

<Ixsl : for-each>

50

</xsl : template>

51

<xsl:texnplate match="keyword">

52

<span style="font-weight:bold; ">

53

<xsl:value-of select=". " I>

54

</span>

55

</xsl : template>

56

<xsl = template xnatch= "ref " >

57
58
59

<a>

<xsl:attribute name="href">
<xsl:value-of select= "@addr" I>

60

</xsl = attribute>

61.

<xsl:value-of select=". " I>

62

<Ia>

53

< /x倒 r 1-emp] ate

64

<xsl : template match= "text () ">

65

<xsl:value-of select=". " I>

===== PAGE 110 =====
109 =====
제3임 XSLT에서 상세 정보 표시하기

</xsl : template>
</xsl : stylesheet>

2 [D3］폴더에서books.xml을실행한다．

수정한 description.xsl를 저장한 후 books.xffil을 실행하면 깨진 그림이 삭제되거나문장 내 일부
에 링크가，
연결되는 등 익스플로러 화면상에 몇 가지 변화가 나타납니다. 앞의 Lesson 내용을 기초
로 갱신한 위치를 중점적으로 살펴 봅시다．

조건에 의해 표시를 갱신하고 싶다 - 단순 분기
鈿1:if> 요소는 test 속성으로 지정된 xPath식
（비교식）
을 평가하여 결과가 true
（참）
일 경우에 내
니｀ '`

'V－

日∼∼∼∼，

戶＼∼

용을출력합니다．
예를 들어 1ogo> 요소의 내용이 공백이 아닐 경우에만 <1mg〉태그의 출력을 실행하도록 하는
20∼28행을 살펴보겠습니다．
<xsl:if

test="logo(. !=' 1">

<xsl:element name= 1'img">
<xsl:attribute name="src">
<xsl:value-of select="logo" I>
<Ixsl:attribute>
<xsl:attribute narne= 'width">120</xsl:attribute>
<xsl:attribute name='height'>150</xsl:attribute>
</xsl : element>
</xsl:if>

포인트는 <xsl:if> 요소의 test 속성입니다．
속성값인梭晏핫七僉즈些史엣팠라서 기술된 비교식입니다· 앞의 Lesson에서 구조를소개했지
만, 한 번더 복습해 보기로 합니다．
우선 logo는 비교의 기점이 되는 요소를 나타냅니다. 즉, 여기에서는 books.xml의 문맥상의
1ogo> 요소입니다．
［∼］로 둘러싸인 부분은 파일 패턴이라 불리며, 실제 조건식을 기술한 위치입니다. ' .' 는 현재의

C

===== PAGE 111 =====
110 =====
노드
（요소）
, 즉 logo> 요소가공백이 아닌 경우 조건식은true를나타냅니다．
는단순분기의 경우는 <xsl:if> 요소가 편리합니다．
이렇게 " 00 의 경우는 ■■한디，
물론 동일한 내용을 또 하나의 조건 분기인 柚l:choose) 요소를 사용하여 기술할수도 있습니다．
<xsl : choose>
<xsl:when test= "logo[. ! =' I '>
<xsl:element name="img">
<xsl:attribute name="src">
<xsl:value-of select="logo" I>
</xsl:attribute>
<xsl:attribute name="width">120</xsl: attribute>
<xsl:attribute name="height">l50</xsl: attribute>
</xsl = element>
</xsl:when>
<xsl:otherwise I>
</xsl:choose>

단, <xs1:choose) 요소는 이러한 단순 분기를 나타내기에는 그다지 어울리지 않습니다. 위의 예에
서도 鈿1:choose) 요소와 <xsl:when> 요소가 내포 상태로 되어 있어 상당히 장황해진 느낌이 있다
는 것을 알게 될 것입니다（조건이 1개일 경우, 계층 구조는 그다지 의미가 없습니다. 조건이 2채 이
상 있을 경우에 비로소 조건 전체를 鈿l:choose) 요소로 정리하는 의미가 있습니C衿．
또, 역으로 다중분기를 나타낼 경우에도 <xsl:jf> 2소를 이용할수는 있지만, 분기가 많아지면상
（이전 Lesson의 鈿l:choose) 요소를 <xsl:if>
호 계층 관계가 보기 어려워진다는 결점이 있습니다
요소로다시 기술해 봅시다）
.

물론 "이 경우는 이쪽을 사용하지 않으면 안 된디y라는 절대적 규칙이 있지는 않습니다. 그러나
소스를보기 쉽고 간소화할수 있다는두 가지 관점에서，종乫t臭三fltl1型트￡色 7H11
鈿1:if> 요소를. 조건이 몇 개로 나눠진 다중 분기에서는 柚l:choose> 요소를 사용한다는 기준을

蠱어두는것흔매o -효한줄입礪r
n

^ ,-. I

1JkI '

L＜죠bㅗ : ㅗㅗ＞ 上Lr亡ㅋ ㅅr긔I

<xsi=if

test=“조건식" >

조건식이 true일 경우에 출력되는 내용
</xsl : if>

'

－∼
－小－

===== PAGE 112 =====
111 =====
쟤3임 XSLㅜ에서 상세 정보 표시하기

2 수치를 정鱗 한 싱태에서 퐈 하고 싶다
한마디로 데이터를표시할 경우, 컴퓨터가 다루기 쉬운 형태에서 인간의 눈으로 보기에 좋은 형태
로 변환하기 위해서는매우많은부가 정보와각종 데이터가 필요하게 됩니다．
예를 들어, <thble〉태그로 표시되는 I{IML 테이블이 그 대표적인 것으로, 특정 위치의 문자색과
폰트를바꾸는 것도 하나의 부가 정보입니다．
그리고 수치 데이터를다룰 때에도
（수치는 가장단적인 사실을나타내는 경우가 많으므로）정확성
을 위해 여러 가지 변환을 통한 가공이필요합니다. 그 중에서도 가장많은 것이 자릿수맞춤이나자
릿수 정렬의 변환등이 그 예에 속합니다.
XSLT에서는 빈번히 발생ㅎ吟수치의 변환 기능을 표준으로 갖추고 있습니다．근젖잊format
number 함수입니다．
\ x1]

이번에는＜price＞요소를3자리 단위로맞추어 출력하도록합니다．
<xsl:value-of select="format-nuxnber(price, '#,###' ) " />원

41행은 <price> 요소의 값을 천단위로 맞추라
（#,洲的는 의미입니다．
그 외에 소수점 이하의 자릿수를 정렬하고 싶은 경우 등은다음과 같이 기술합니다．
<xsl:value-of select="format-nuxnber(price, '#,###.00 ) " />원

이 예의 경우는소수점 이하두자리로수치 데이터를 정렬합니다．
3 문서의 일부에 링크를 연결하고 싶다
앞의 Lesson에서 소개한 문서의 일부를 강조 표시" 하는 경우와 거의 동일합니다. 38행에서
<memo> 요소에 적용할 템플릿을 불러내는 위치도 같습니다．
<xsl : apply-templates select= 'memo" />

이번에 새로 추가되는 것은 56--'63행의 <ref> 요소에 적용되는템플릿입니다．
56∼63행은 <ref> 요소와addr 속성의 내용을 기초로 다음과 같은 링크 문자열을 생성합니다．
<a href=" … "

>'"</a>J갚．
『쵸
「

링크 생성에 대한 자세한 내용을 Lesson5를 참조하기 바랍니다．

===== PAGE 113 =====
112 =====
<xsl:template xnatch="ref '>
<a>

<xsl:attribute name="href '>
<xsl:value-of select="@addr" I>
</xsl:attribute>
<xsl:value-of select= '." I>
<Ia>
</xsl:template>

61행의 柚l:value-of> 요소는 현재 요소인 <ref> 요소의 텍스트를 그대로 표시합니다．
또한, 텍스트 부분에 대해서는 앞의 Lesson에서 이미 소개한 64∼66행의 템플릿이 적용됩니다．
<xsl : template match='text ( ) " >
<xsl:value-of aelect=". " I>
</xsl = template>

-

恪
`-

· 단순한 분기 처리는 <xsllf> 요소를 사용합니다．
· 자릿수 정렬 문자 등 수치 데이터를 변환할 경우에는 format-number 함수를 사용합니다. format-number 함수
는 xPath 함수의 하나입니다．
태그를 생성하는 템플릿과 텍스트를 그대로 출력하는 템플릿의 두
· 문서 내에 링크 문자열을 생성할 경우에는 (a）
가지 형식으로 기술합니다．

===== PAGE 114 =====
113 =====
재3일 XSLT에서 상세 정보 표시하기

Lesson 6의 실력 테스트에 등장한XSLT스타일 시트를 아래의 화면과긷끼 고쳐 봅시다. 비어 있는
곳을채우고, 올바른XSLT를작성해 주십시오．
따일
（f:) 편집
（트） 보기〔y) 글기찾기
（스） 도구
（끄 도8말沮）
da뒤로 , 뺙

J

」〕소

a검색 j」i 31VI 今UL0머

4,

］계요
550
1.1 XML이란 무엇인가9
Y.Yamada
1.2 FITMLJSGML의 비 교
ac5。
N.Kakeya
2XML 문서！기숟헤 보자
950
2.1 XML 문서의 선언
'1Yamada
2.2 유일한 제 1 요소퓰 가질 것
NaN
M.Mochiduk
3 r간행 서적 일람J 읕 표시헤 보자
3.1 XML 문서에서 ×SL올 뷸러낸다．
1,095
K.Usui
3.2XSL 스타일 시트퓰 선언한다
850
H.Sak래
4 『서적 상세 정보」퓰 표시에 보자
4.1 표를 표시하고 싶다
（일자 정렬）
650
ㅜ．Kan아（〔〕
4.2 문서에 일부분을 강조 표시하고 싶다 N刀
'(Yamada
柏毋乙＝刃∥呵∥m

l

i

}

S

table.xsl
<?XTr江 version= "1. 0 " encoding="EUC-KR" standalone= 'yes" ?>
<xsl : stylesheet xmlns:xsl="http: /Iwww.w3 .org/l999lXSLlTrarisforrn"
version="l. O ">
[

I

<xsl:template znatch="/ ">
<htxu1>
<head>
<title＞기사 목차＜/title>
</head>
<body>
<xsl:element name="table">
<xsl:apply-templates select="article " I>
</xsl : element>
</body>
</html>
</xsl template>
<xsl:template match="article ">
<xsl:for-each select="/ /chapte미I/ section" >

===== PAGE 115 =====
114 =====
<tr>
<th aligii="right" valigri='top">
<xsl:nuniber level="multiple" format="l" count="chapterl section" I>
<Ith>
<xsl:choose>
<xsl:when test="name()= ' chapter' ">
<td colspan="2" style="font-size:l2pt;
backgrourid:#ffeeaa;font-weight:bold;">
<xsl:value-of select="@title" I>
<Itd>
</xsl:when>
<xsl:otherwise>
<td>
<xsl:value-of select="@title" I>
<br I>
<xsl:value-of se1ect= "(aauthor" I>
</td>
</xsl:otherwise>
</xsl:choose>
< [

I

test=" I

] ">

<td valign="top">
<xsl:value-of select= " [

I " I>

<I

</td>

I

I >

<Itr>
</xsl:for-each>
</xsl:template>

"은책끄
「’
'에4

"
「

L

채

</xsl = stylesheet>

===== PAGE 116 =====
115 =====
제3일 XSLㅜ에서 상세 정보 표시하기

Go to XML

===== PAGE 117 =====
116 =====
Lesson 8- Lessor'

고도의 XSLT+α 테크닉
3일간에 걸친 XSLT의 마지막 학습일입니다．
표현의 폭을넓히는 것뿐만 아니라 지금까지의 예제로는다룰수 없었던 표현상의 부적절한부분을 보다
완성도높게 만들어 나갑니다．
오늘로써 XSLT의 학습은 끝나지만, 이후에 DOM
［과 그 외의 기술과 연동해가면서 확실한 기반을 만들
어갑시다．

===== PAGE 118 =====
117 =====
오늘 공부할 내용들
xPuth 함수 사용하기
円 유지 보수정의 향상과 보다 세밀한 표시
제어하기

===== PAGE 119 =====
118 =====
제4일 고도의 x히．
.T＋α 4크닉

!
·｀

xPatI, 함수 사용하기
계속해서 ×SLT를 학습합니다. 서적 목록 XML의 상세 정보를 표시해 봅니다．

xsl

books.

多￦eb5!i A1 욱륙 - Microsoft int8met E跡o,e'
따일
（E) 편집（트） 보기
（y) 즐겨찾기（스） 도구（工） 도옴말
（t1)

……∼M衲曲：念葦塔

二1므注
r:

… －」蜘 ！三

연결 "

@XML

;‘立

학습 내용 미리 보기

＼눋뒤로 !

［누\ . Less。
n8
L鈿 Q&a

9 〕 仝

gt검색

」즐겨찾기 守ol디머 J

三5, J

Web 관련 서적 목…
ㅣ

乙BN 코드

서적

孰SBN89-314-1742-x Hㄲ卜ylL 디자완 : 1걸 가이－
ISBN的314-1978-3 ASP사천

저자

출판ㅅ
「

가격

발간일

O1.6
경진닷컴 ]1.800원 20이 06-il
l니시자오｝나오캐영친닷쾀；15.00O2i 2001-11-30

ISBN8커314-2014-6 10일만에 배우는Visui C++ 6.0 Seto Haruka

｛영진닷컴江5.000뭔2α -02--

肛SBN89-314-1994-히알짜PC 용어 사전

憎진닷퀘iasoo也2002-01-05
핑쾨15325원

倫와시스템

Youngjin.com Y.

町퇀…

썅囊講轟纛癬難二F＝ㅍ爾컴퓨E…

＝」
∼

(un> 요소가 없는 정보에 대해서는 링크를 연결하지 않는다．
또, 가격의 평균값을 구해본다．

/．
●Key Point

客똥崙；各Less。
n。H籍릎器筋紫籤이해하고있다면，개념적으
로 새로운 것은 거의 없습니다．
앞의 내용을 한번 더 복습함과 동시에 새로 나온 구문을 파악함으로써 XSLT의 부가 기능을 습득하
시기 바랍니다．

118

===== PAGE 120 =====
119 =====
제4일 고도의 ><SLT+α 테크닉

※[D2]폴더에 있는books.xml, books.ess를 ㄸ）4] 폴더에 복사해 주십시오．

1

제2일Lesson 5에서 작성한XSLT스타일시트books.xsl을메모장－으로열어 리스트의
코드를 추가하고 [D4] 폴더에 books.xsl 이름으로 새로 저장한다．
리스트 : bo이
（s.xsl
<?,anl version="l. O" encoding= "ETJC-KR" ?>
<xsl = stylesheet milns :xsl="http: //www.w3 .org/1999/XSL/Transforin"
version="l. O ">
<xsl :output method="html ' encoding='ELTC-KR" />
<xsl:texnplate match="/ ">
<html>
<head>
<title> <xsl:value-of select="books/@title' I><Ititle>
<link rel='stylesheet" type="textlcss" href="books.css" I>
<Ihead>
<hl><xsl:value-of select="books/@title" I></hl>
<table borderr∥i">
<tr>
<th>ISBN 코드＜/ th>
<th＞서적 </th>
<th＞저자 </th>
<th＞출판사 </th>
<th＞가격 </th>
<th＞발간일 </th>
<Itr>
<xsl:apply-templates select="books" I>

===== PAGE 121 =====
120 =====
</table>
<div><xsl:value-of select='books/owner" /></div>
</html>
</xsl:template>
<xsl:template match="books">
<xsl:for-each select="book'>
<xsl:sort select="price" data-type= 'number"
order="ascending" />
<tr>
<td nowrap= "nowrap"><xsl:value-of select

4一

="@isbn" /></td>

全
5
5
5

「

5:

<td nowrap="nowrap"><xsl:value-of select = "author" I>
</t；ㅍd>

5一

:rap= "no
:sl = if

tf

56

<xsl =rnE

57

</xsl:if>

58

<xsl:value-w.

59
60

<td nowrap= "nowrap">

6노

<xsl = choose>

62 '

<xsl:when test="price[nuxnber(. ) &lt;

= 3000] ">

===== PAGE 122 =====
121 =====
<span style= 'font-weight:bold; " >
<xsl:value-of select=∥format -number
(price, '##,###' ) " I>원
</span>
</xsl :when>
<xsl : otherwise>
<xsl:value-of select= 11format-nuxnber
(price, '##,### )" />원
</xsl : otherwise>

69

</xsl : choose>

70
71

</td>

72

<td nowrap= "nowrap"><xsl:value-of select ="pDate" I>
</td>

73
74

<Itr>
</xsl : for-each>
</xsl : template>
</xsl : stylesheet>

2 [D4］폴더를열어books.xml를살행한다．

앞의 Lesson에서 소개한목록에 가격의 평균값을추가했습니다．
또, 이전에는 <ur1 요소의 존재 여부에 관계없이 도서명에 링크를 설정했습니다. 따라서 링크가
연결되지 않았던 곳도 있었습니다. 그러나 이번에는 <un> 요소의 유무에 따라서 링크를 연갈할지의
여부를판단합니다．

공요소의 처리 - 분기 조건의 응용
<xsl:choose> 요소, <xs1:if> 요소에 의한 조건분기에 대해서는 이미 배웠습니다．
39--51행은 bOOkS.Xml의 <book) 요소 중에 <un> 요소가 존재하는지의 여부로 링크를 생성할지
를 결정하는 조건 분기를 작성합니다. <uI) 요소가 존재하지 않을 경우에는 링크를 연결하지 않고
단지 문자열을출력합니다
（링크를 연결하는 방법에 대해서는 Lesson5를 참조하기 바랍니디）
.

參

===== PAGE 123 =====
122 =====
<xsl:choose>
<xsl:when test="url">
<xsl:element nanie= "a">
<xsl:attribute name= "href">
<xsl:value-of select="url" I>
</xsl:attribute>
<xsl:value-of select="name" I>
</xsl:eleinent>
</xsl:when>
<xsl: otherwise>
<xsl:value-of select="name" I>
</xsl:otherwise>
</xsl = choose>

여기에서 포인트가 되는 것은 <un> 요소가존재하는 경우라는 조건식을 어떻게 기술할 것인가하
는 것입니다．
지금까지의 조건식
（xPath식）
은 ''price &1t;= 3000''과 같이 쏘소＋비교 연산자＋값'과 같은 구조
로 되어 있습니다. 그러나 이번 鈿1:when) 요소의 thst 속성에는단지 형식적으로 un이라는 한 문
장만 기술되어 있습니다. 얼핏 보고 '어？' 하고 생각하는 분도 결코 적지 않을 것입니다. XSLT에서
는 이렇게 생략형으로 기술되는 경우가자주 있으므로주의해야합니다．
조건식으로써 노드가 기술된 경우에는 현재 문맥상에 그 노드가 있는지 검색하고, 존재하면 식 전
체를true
（침）
, 존재하지 않으면 false
（거짓）
으로 간주합니다．
이와 겉끼, 익숙하지 않으면 좀 망설여지는 기술이지만, 반대로 익숙해질수록 간결한 기술을 할
수 있게 되는 것도 XSLT의 커다란 매력 중의 하나입니다.

`-r

books.xml의 <?xml-st닌esheet?> 처리 명령을 호출하는 곳이 books.xsL로 되어 있는지의 여부를 실행 전에 확인
하도록 흗川다．

===== PAGE 124 =====
123 =====
제4임 고도의 ×SLT+α 테크닉

평균값을 구하고 싶다
종래의 ffl入Th에 있어서 파일 내에 삽입된 각종 데이터를 집계하는 것은 매우 어려운 작업이었습
니다. 만약 굳이 하려고 한다면 아무리 간단한 평균값 계산이라도 JavaScript 등으로 프로그램을작
성해야했습니다．
그러나XML은 데이터를 다루기 위한 언어입니다. 이러한 단순한 계산 기능은 표준으로 미리 갖
춰져 있으며 프로그래밍을 간략화해 줍니다．
25행은 <books> 요소 내에 있는 <price> 요소값의 평균값을 계산하여 표시하고 있습니다．
<xsl : value-of select= " sum(books//price) div count
(books/ /price) " /)'

（sum）
를 산출하고，
sum(books//price）
는 <books> 요소 아래의 (price> 요소값의 합계
count(books//price）
는 <books) 요소 아래의 <price> 소의 개수
（count）
를 각각산출합니다．
'/' 가바로아래의 요소를 나타내는 데반해 '//' 는아래의 전쳬 요소를 나타내며, div는나눗셈을
의미합니다．
산출된 결과가 최종적으로 출력됩니다．
어떻습니까？아주 편리한 기능이죠？
아래에 이것 이외에 XSLT 내에서 사용할수 있는 xPath 함수 중에서 중요한 것을 간단히 정리해
놓았습니다. xPath 함수는 그 기능적 분류상 노드 설정 함수, 문자열 함수, 진위 함수, 수치 함수，
XSLT 함수로 구분됩니다．
여기에서는 각각의 상세한 사용법은 생략하고 있습니다. 어떤 종류가 있는지만 참고하기 바랍니
대［]안의 인수는 생략 가능합니다）
.
町ii忿ㅋ也z吐恪1
＝소4｀

닢

함수

`

n

U
= `

［,노드명,…］)
document
（노드명

노드 설정

노드의 값이 나타내는 외부 ×ML 문서를 나타낸다
0 documenl(@url)/books/fbook

Iast( )

수치

현재 노드 설정의 노드 수를 나타낸다

［노드명,…］)
bc테-name(

문자열

노드명
（이름 공간 접두사
（()0<x:^J）
를 삭제한다）

［노드명,…］)
name(

문자열

노드명
（이름 공간 접두사를 포함한다）

［노드명," " "])
namespace-uri(

문자열

노드 설정이 속한 이름 공간의 URI

position()

수치

몇 번째의 자식 노드인가

===== PAGE 125 =====
124 =====
concat
（문자열
［，
문자열," " "])

문자열

문자열을 연결
0 concat(title,subTitle) - (title) 2소와
(subTitle> 요소를 연결

contatins
（문자열1,문자열2)

true: false

문자열1이 문자열2를 포함하고 있을 경우 true
0 contains(keyword: 'ASP) - (keyword) 요
소에 문자열 ASP가 포함되어 있으면 true

normalize-space(
［문자열，
…］)

문자열

문자열 전후에서 스페이스를 제거
0 normalize-space(author) - (author) 요소의
전후에서 공백을 제거한다

start-with(strl,str2)

true false

stri이 str2에서 시작됐을 경우 true
固 start-with(tftle, )(ML') - <title) 2소에 문자열
XML이 포함되어 있으면 true

string(
［노드명，
ㅢ）

문자열

노드를 문자열로 변환
國〕sfring(price) - (price) 요소의 내용을 문자열
로 변환

string니ength(
［문자열, " ··］)

수치

문자열 길이
町 strin〔Hength(title) - 仙e> 요소의 문자열 길
이를 나타낸다

substring
（문자열,시작 위치，

문자열

문자열이 지정된 위치에서 임의의 문자수 만큼을

추출할 문자수）

추출）
回 substring(f sbn,5,20) - isbn 속성의 다섯
번째 자리에서부터 20문자 만큼을 추출

substring-attet
（문자열1, 문자열2)

문자열

문자열1을 문자열2로 나누었을 때 그 후반부의 문
자열
0 substring-after(url, ':1/ ) → (un) 요소를 '://
로 내구었을 때 그 후반부를 나타낸다

substning-before《문자열1,문자열2)

문자열

문자열1을 문자열2로 나누었을 때 그 전반부의 문
자열
0 substning-before(url. ':/1) - (url> 요소릍
':// 로 나누었을 때 그 전반부를 나타낸다

===== PAGE 126 =====
125 =====
\:：쟈1꺼毫‘，
:*.옰∼8 :

boolean峰드명）

true:false

노드를 불린값(true!轍se)으로 변환

false()

false

false

（문자열）
lang

true:false

xml:lang 속성이 지정된 문자열을 포함할 경우 true

not()

true:false

true이면 false, false이면 true

true()

true

true

1
ceiling
（수치）

수치

지정된 수치보다 작지 않은 최소의 정수
回〕ceilingmeight) - 0ieight> 요소의 값을 정형화

floor
（수치）

수치

지정된 수치보다 크지 않은 최대의 수치
D floor(weight) - <weight> 요소의 값을 정형화

（노드명）
number

수치

주어진 노드의 값을 수치로 변환
回 number(price) - <price) 요소의 값을 수치로 변환

round
（수치）

수치

지정된 수치를 사사오입한 값
ㅁround(height) - <height》요소의 값을 사사오입

sum
（수치）

수치

주어진 수치의 합계
回〕sum(point) - <point> 요소의 값을 합계

===== PAGE 127 =====
126 =====
，■i

拉■뺘
current( )

노드 설정

현재의 노드를 나타낸다

element-available
（문자열）

true:false

지정된 요소명이 현재의 XSLㅜ 프로세서에서 사용할 수 있는
지의 여부
0 element-avahable( 'xsl:template') → (xsl:template) 2
소를 사용할 수 있으면 true

format-number
（수치，문자열）

문자열

수치를 지정된 서식으로 변환
0 format-number(price. '#,###.OO') → (price) 요소의 값
을 천 단위로 자리수를 구분하고, 소수점 이하 두 번째 자
리까지 표시한다

function-available
（문자열）

true:false

지정된 함수를 사용할 수 있는지의 여부
0 function-available( 'format-number') format-number 함수를 사용할 수 있으면 true

system-property(string)

문자열

지정된 문자열
（xsl:version, xsl:vendor, xsl:vendor-url 등）
로 표시되는 시스템 프로퍼티
0 system-property( 'msxml:version') - MSXML의 버전
을 나타낸다

3 襄 데이터를 없애는 작업 테크닉
어느 정도 대량의 데이터를 다루게 되면 XML 문서에 잘못된 데이터가 들어 있는지의 여부를 출
력 과정에서 자동으로 검사하기를 원하는 경우가 있습니다. 그런 경우 鈿1:message) 요소를 이용
하여 강제적으로 에러를발생시킬 수 있습니다．
<t코 nowrap= "nowraP" >
<xsl:if

test="publish[.=' ']">

<xsl:nlessage tenninate= "yes" />
<Ixs1:if>
<xsl:value-of select="publish" I>
</t=d>

55행의 </xsl:if> 요소에서는 <publish) 요소의 내용이 비었는지의 여부를 판정하고 있습니다．
에는＜xsl:message〉요
만약비어 있을경우〈즉, 현재요소 '.' 인 <publish> 요소가빈 " 일경우）
소를 출력합니다. terminate 속성은 그 시점에서 XSLT에 의한 변환 처리를 정지할지의 여부를 정
하는플래그로도yes인 경우 <publish> 요소가공요소의 발생 시점에서 처리를 정지시킵니다．

===== PAGE 128 =====
127 =====
－졔4임 고도의 ×SLT-I-a 테크닉

L<xsi

:message>

上
（=
：亡틔 시식1冬黨多1瓠…1꺼擁珊珊따心n了

<xsl :message terminate=”처리를 중지할지의 여부
（yes I no) ">
출력할 내용
</xsl :message>

<xsl:message) 요소는 그 성질상 <xsl:if〉
나 <xsl:choose> 요소 등 조건 분기 명령과 함께 사용합
니다．
-

Go to XML

"
나

·(xsl:if〉와 <xsl:when) 요소의 test 속성 중에서 단지 단순한 노드가 지정된 경우에는 노드의 유무를 판정합니다．
·XSLT 내에서는 여러 가지 xPath 함수를 사용할 수 있습니다．
·XSLT에 의한 변환 도중에 강제적으로 에러를 발생시킬 때는 <xsl:message〉
를 사용합니다．

Q

실력 테스트

[D4] 폴더의 books.xs을 기초로 하여 아래 그림과 같은 표를 출력하는XSLT 스타일 시트를 작성해
봅시다. 이 때, 다음사항에 주의해 주십시오．
TSBN 코드는 ISBN을뺀 5번째 자리부터 출력한다．
· 서적은 7자리로 정렬한다．
· 서적에 ASP를 포함하는 서적 정보만 표시한다．
· 최근의 발간일순으로 정렬한다．
파일Cf) 편집
（E〕 보7i(V) 晉겨찾기
（莎도구m 토뮴닳(H)
卞뒤르 .

J

‘〕소 a검색 ．三』召겨찾거 沙미디머 3

스，
J

Web 관련 서적 목록
ISBN B드
서석
저자
출판사
가격
발간일
89-314-1978-3 A寸 노：그 니시자와 나오키 영잰긋컴 比刀LIJ뭔 2 〕
1-11羽
5nr]n뭐
ㅣ
Youngjin.com V

뫈료

k겯UI헙퓨터

===== PAGE 129 =====
128 =====
books.xsl
<?xml version="l.O " ericoding= "EUC-KR" ?>
<xsJ. = stylesheet xmlns:xsl="http://www.w3.orgl1999/XSL/Transform"
version="l.O">
<xsl:output method=「html" encoding= "EUC-KR" I>
<xsl : template match= " / " >
<html>
<head>
<title><xsl:value-of select= "books/@title" I>
</title>
<link rel="stylesheet" type="text/css" bref="books.css" I>
</head>
<hl><xsl :value-of select= "books/@title" /></hl>
<table border="l ">
<tr>
<th>ISBN 코드 </th>

匹－

<th＞서적 <Ith>
<th＞저자 <Ith>
<th＞출판사 <／나1>
<th＞가격 </th>
<th＞발간일 </th>
</tr>
<xsl:for-each select=" [
[

] ">

]

<tr>
<td nowrap="nowrap"><xsl:value-of select
<td nowrap="nowrap">
<xsl = choose>
<xsl:when test="url ">
<xsl:element name="a">
<xsl : attribute name= "href">
<xsl:value-of select="url " I>
<xsl:value-of select=" [

]

I>

<txsl:attribute>
</xsl :element>
</xsl:when>
<xsl:value-of select=" [

I

I>

<xsl : otherwise>

[

I

" /><ftd>

===== PAGE 130 =====
129 =====
제4일 고도의 XSLT-I-a 테크닉

</xsl:otherwise>
</xsl:choose>
</tc그＞
<td nowrap='nowrap"><xsl:value-of select ="author ' /></td>
<t(크 nowrap= "nowrap" >
<xsl:value-of select="publish" I>
</td>
<td nowrap='nowrap'>
<xsl:value-of select= ''forxnat-nuncber(price, '#,#### ' ) " />원
</td>
<td nowrap= "nowrap'>
<xsl :value-of select= "pDate" /></td>

1

< /tr>
</xsl = for-each>
<tr>
<td colspan="4 " I>
<td>
<xsl :value-of select= n [
<Itd>
<td I>
</ tㅍr>
</table>
<div><xsl:value-of select='books/owner" /></div>
<Ihtrn1>
</xsl : template>
</xsl : stylesheet>

해답은 책 끝에 4:)
I

===== PAGE 131 =====
130 =====
댄4일 고도의 XSLT+a 태크닉

유지 보수성의 향상과 보다 세밀한 표시 제어하기

小n

■ 학습 내용 미리

description.xsl

inc.xsl

노 \

騙상세 정驪표시 MiCFoeefl Pneret E :pIorerm：轉弊；
凝珊年‘
，파일
（E) 편집（트） 보기
（y》 뜰겨貫기( ) 도구
（T) 도뭄달坦）

Lesson 9

∼ ∼" 『

j ㅌ〕소 a검색 ＝」즐겨찾기 沙미디어 J －스，→j

：中뒤로 …

XML

보기

이번에는 제 3일에 작성한 상세 정보 표시를 수정합니다．

＝쏘j- 1
.

」

" 연결꽥
上荳

상세 정보 표시

1 LII Q&a
^17져
' 1'

二r ,/

':
1. `
' 녹孕"
'
’닉G

드J뫈료

02. ASP 사전（니시자와 나오키）
ASP의 모든 명령을 내 포켓속에 Poket Reference ASP사전
은 ASP의 기몬적인 지식과 사용 가능한 명령의 구문, 구문
에 대한 상세한 설명, 명령 활용 예를 ASI> 오브젝트, ADO.
FileSystemObject의 메소드, 프로퍼티로 분류하여 언제든지
쉽게 찾아 참조할 수 있도록 한 사전식 레퍼런스입니다
15.000원

堪；내 컴퓨El

ii
…

카테고리가 ASP인 서적의 정보가 以 된다

：》Key Point ) _
지금까지의 내용으로 XSLT의 기본적인 부분은 대부분 이해했을 것입니다．
여기에서는 장황하게 되기 쉬운 XSLT를 어떻게 간결하게 기술할지, 유지 보수를 어떻게 쉽게 할지，
以 상의 작은 문제 해결 등 7階상의 다른 테크닉을 소개합니다．

===== PAGE 132 =====
131 =====
제4임 고도의 ×SLnα 테크닉

※ D3]폴더에 있는htmLjpg, aspjpg, pc.jpg, books.xml, book2.css를 D4]폴더에 복사해 주십시오．

1

제3일Lesson7에서작성한XSLT스타일시트description.xsl을열어리스트1의코드를
추가하고, 嶼］
폴더에 descriptiorixs1이름그대로새로 저장한다．
리스트 1 : description.xs!
<?xml version="l. 0" encoding= 'EUC-IcR'' ?>
<xsl = stylesheet xmlns:xsl="http: //www.w3 .org/1999/XSL/Transform"
version="i. 0">
＜ㅈ5ㅗ

V以i ㅗ OL) d

n口도【L,;

」a,;}

가M汐t∼q / XsI

= Var」．aads =

=

<xsl:attribute-set name= 'imgAttr '>
<xsi:attribute name='width'>120</xsl:at

→

<xsl:attribute name= m∼‘ 小n→ 「 4「 ^
</xsl:attribute>
</xsl:attribute-set>

m毒……1
1

<xsl :decimal-format NaN= 」：∼，
L…／느
9
10

<xsi : template match=" / '~>
<html>

11

<head>

12

<title＞상세 정보 표시＜/title>

13

<link reir "stylesheet' type="text/css" href="book2.css" I>

14

<Ihead>

15

<body>

16

<hi＞상세 정보 표시＜/hl>

17

<xsi:apply-templates select="books" I>

18

</bㅇdy>

「19

</html>

20

</xsl : template>

2j.

<xsl:template match="books">
<table border="0">
<tr>
<td width=" 150">

26 ,
27 ;

<xsl:if

test="logo[. !=' ']">

＜工m9 x6ㅗ ．u5e-d｛凡工ㅗㅗ가jㄴe→i;eC6=’ㅗiiuAt亢；r「

0

===== PAGE 133 =====
132 =====
28

<xsl:attribute name="src">

29

<xsl:value-of se1ect="loqo" />

30
31
32

</xsl:attribute>
</1mg>
</xsl = if>

33

</td>

34

<td valign= "bottom'>

35
36

<dl>
<dt>

37

<xsl:nunther formatr "0l" I>.

38

<xsl:value-of select="name" I>

39

(<xsl:value-of select="author" I>)

40

</dt>

41

<ad>

42

<xsl:apply-templates select= "memo" I>

43

<br I>

44

<div style= "text-align:right;">
<xsl:value-of select= "fonnat-number

45

(price,'*,###')" />원
<Idly>

46
47
48

</dd>
<Idl>

49

<Itd>

50

<Itr>

51

<Itab1e>

52

<hr I>

53

</xsl = for-each>

54

<Ixs1: template>

55

<x$ L = 」．1lcㅗuαe h工et= " ir1c . xs1" /

56 </xsl : stylesheet>

2

새문서를열어 리스트2의코드를입력하고, D4］폴더에rnc.xsl이라는이름으로저장한다．

企

===== PAGE 134 =====
133 =====
제4임 고도의 XSLT+α 테크닉

리스트 2 : inc.xsl
<?xml version= "1.0 " encoding= "EtJC-KR" ?>
<xsl : stylesheet milns:xsl="http: /Iwg. w3 .org/1999/XSL/Transform"
version="l. O ">
<xsl = template match= "keyword'>
<span style="font-weight:bold; ">
<xsl:value-of select=". " I>
</span>
</xsl = template>
<xsl:template uiatch="ref">
<a>

<xsl : attribute name= "href">
<xsl:value-of select=" @addr" I>
</xsl : attribute>
<xsl:value-of select=". " I>
<Ia>
</xsl : template>
<xsl : template match=" text a ">
<xsl:value-of select=". " I>
</xsl = template>
</xsl : stylesheet>

3 [m］폴더를열고books.xml을실행한다．

이번에는 기술의 고안에 중점을두고 있어서 표시상의 새로움은그다지 느끼지 못했을지도 모릅니
다. 다만, 어느쪽이든앞으로보다실용적인XSLT를기술해 가는데 있어서 중요한작성법입니다．
단순히 구문 予칙만을 보는 게 아니라 왜 이 명령을 사용하는지, 왜 여기에서 사용하는지에 대해
서도주목합시다．
1 변수를 정의하고 싶다
여러 곳에서 동일한 문자열과 수치를 참조할 경우, 같은내용을 여러 곳에 작성하는 것은 여러 가
지 의미에서 불필요한 일입니다. XSLT를 수정할 경우는 물론이고 앞으로 외부 프로그램을 이용하

瘢

===== PAGE 135 =====
134 =====
여 동적으로XSLT를변경할 경우프로그램이 필요 이상으로 장황해지는한 가지 원인이기도합니다．
XSLT에서는 이러한공통 데이터를 변수로서 정의할수 있습니다. 3행을봅시다．
<xsl:variable riame="key">ASP</xsl:variable>

<xsl:variable> 요소는 name 속성으로 정의된 이름의 변수를 정의합니다. 예를 들어 이 XSLT 코
드에서는key라는 이름의 변수에 ASP라는문자열을 저장합니다．
또, 선언된 변수는 $ 변수명으로참조할수 있습니다．
이번 예는 22행으로 아래의 <c堆Dry> 요소에 변수 key로 정의된 문자열
（즉, ASP> 포함하는
<book) 요소를추출하려 하고 있습니다．
<xsl:for-each select="book[contains(category, $key)]">

예를들어 22행을다음과 같이 바꿔 써도 같은 의미입니다．
<xsl:for-each select= "book (contains (category, ' ASP' ) ]" >

아래의 <c峽＝oiy> 요소에 ASP라는 문자열을 포함하는 (book> 소만을 추출합니다. 변수를 사
용하지 않을 경우, ASP를다른 것으로 변경할 경우 여러 곳에 문창이 있으면 여러 곳을수정해야하
고, 당연히 수정을 빠뜨리기도 합니다. 하지만, 변수를 사용함으로써 柚l:variable> 요소의 내용만
수정하면간단합니다．
늘 변수를 사용하라는 것을 권장하는 것은 아니지만, 변수를 잘 사용하면 보다 유지 보수정이 좋
은소스를 작성할수 있습니다．
2 속성을 합쳐서 정의하고 싶다
예를 들어 그림의 크기, 주변의 공백 등요소의 속성을 중복하여 정의하고 싶은 경우가 있습니다．
물론 개개의 요소에 개별적으로 속정값을 설정해도 좋지만, 여러 곳에서 동일한 설정을 사용하고 있
을때 문장이 장황하게 늘어나고 수정 시간도 증가하게 됩니다．
그래서 XSL'I볘서는자주 사용하는 속정 설정 조합을 별도로 미리 선언해 둡니다．
<xsl:attribute-set name=" imgAttr">
<xsl:attribute name= "width">120</xsl:attribute>
<xsl:attribute naine="height">150</xsl:attribute>
</xsl : attribute-set>

예를 들면 4, 7행과같이 width 속성과height 속성을속성 세트 imgAttr라는 이름으로 선언합니
다. 덧붙여 말하면, 일단설정된 속성 세트는 아래와같이 자유롭게 참조하여 사용할수 있습니다．

參

===== PAGE 136 =====
135 =====
제4일 고도의 XSLT+α 테크닉

，」， <img xsl:use-attribute-sets= 'ixngAttr">
28

<xsl:attribute name=''src">

29
30

<xsl:value-of select="logo' I>
</xsl:attribute>

31; </1mg>

이것은다음과같이 작성하는 것과똑같은의미입니다．
<nflg>
<xsl:attribute name="src">
<xsl:value-of select= "logo' I>
<Ixsl : attribute>
<xsl:attribute naxne="width''>120</xsl:attribute>
<xsl:attribute namer "height''>150</xs1:attribute>
</1mg>

g：…

…

또 복수의 鈿1:attibute-set) 요소로 정의된 속성 세트를 병합하여 참조하고자 할 경우에는 다
음과 같이 속성 세트명을 열거합니다．
<1mg xsl :use-attribute-sets= " imgAttr ixngAttr2" >

r-

r
,
r. I 1 JAIl
L<xㅂㅗ = dLLLJI) uLㅂ-seL> 」i즈亡ㅋ ^r긔」

<xsl:attribute-set name= "속성 세트명“>
<xsl= attribute> 요소에 의한 속성의 정의
</xs1:attribute-set>
<xsl : attribute-set> 요소의 정의는 임의의 출력 요소상에서 참조할 수 있습니다．
＜요소명 xsl :use-attribute-sets= " 속성 세트명" >-<／요소명＞

3 수치가 아닌 경우의 처리를 정의하고 싶다
format-number 함수로 수치를 변환하고자 했을 때 XML 문서의 입력 오류나 다른 이유로 수치
가빠졌다면, 또는수치로서 인식할수 없는 데이터가들어 있다면 어떻게 하겠습니까9
XSLT는NaN(Not a Number）
이라는 문자열을 나타냅니다．
물론, 에러가 나지 않아 이대로 괜찮치 않을까 하고 쉽게 생각할 수도 있지만, 이것만으로는 재미
없다고 생각하는 이도 상당수 있을 것입니다．
그래서 여기에서는 format-number 함수로 지정된값이 수치가 아닌 경우에 지정한 문자열을표

小

===== PAGE 137 =====
136 =====
시하는방법을 소개합니다．
<xsl:decimal-format NaN="- 1' I>

이 예에서는format-number함수의 인수가수치가 아닌 '-' 라는문자열을표시합니다．
L<2t8ㅗ = uㅂCㅗ표k효ㅗ－』＝(J工Indㄴ＞

r,

r,

1 」人 ,

뇨二亡ㅋ ㅅr긔」

<xsl:decimal-format [name= ”포맷명"]
[decimal-separator= ”소수점
（ . . 1 등 "]
[grouping-separator= " 자릿수 지정 문자
（ 1 , 1 등） "]
[minus- sign=" 마이너스 문자
（ ' - 1 등） " 〕
[NaN= " 숫자가 아닐 경우의 표기
（ ' NaN ' 등） “〕
[percent= " 퍼센트 문자《 ' 잊긋 등） "]
[digit="O인 경우의 표기
（ '0 ' 등） "]

어디까지나 <xs1:decimal-format> 요소는 format-number 함수로 변환될 때의 기본값을 정의
할뿐으로, 그자체적으로는 어떠한출력도하지 않습니다．

4 외부 )SLT를 이용하고 싶다
XSLT는 템플릿의 집합체입니다. 작은 템플릿이 서로 호출하면서 하나의 스타일을 구축해 나가는
것이 기본적인 작성법입니다．
그 때문에, 구조상 XSLT는 부품화하기 쉽게 세밀한 템플릿을 밖으로 꺼냄으로써 복수의 스타일
시트 간에 사용할 수 있게 되어 있습니다．
예를 들어 55행을 봅시다．
<xSl = include href= "inc.xsl" />

이렇게 기술함으로써 현재의 스타일 시트에 inc.xsl이 삽입됩니다．
불려진 외부 스타일 시트는마치 현재의 스타일 시트 내에 기술되어 있는 것처럼 작동합니다．
또, 불려지는 템플릿은 부분적인 스타일 시트여서는 안 됩니다. 즉, 반드시 경로 요소에
鈿l:s敏lesheet> 요소를둔 독립된 XSLT의 형식에 따르고 있어야 합니다．
r

-'I

. l .`

L<Xsi- = inckuoe> 뇨소뵈 Al식I
<xsl : include href= ' 불러낼 스타일 시트의 경로" />

===== PAGE 138 =====
137 =====
제4임 고도의 ×SLT+α 테크닉

-

Go to XML
∼
·〈×히:varia네e> 요소를 이용하여 반복적으로 사용하는 데이터를 변수로 별도 정의할 수 있습니다，
·<xsl:attribute-set> 요소를 이용하여 반복적으로 사용하는 속성 정의를 별도로 정의할 수 있습니다．
·<xsl:decimal-format> 요소는 format-number 함수에 있어서의 수치 표시 형식을 설정합니다．
· 외부의 XSLT 스타일 시트를 가져오려면 <xsl:include> 요소를 사용합니다，

Lesson5의 books.xsl을수정하여 아래와같은XSLT스타일 시트를작성했습니다．
공백을 채우고 XSLT를 완성시켜 주십시오．
※ 주의 :
단, 가격 정보는 그림과같이 자릿수를 정렬하고, 만약 가격 정보가존재하지 않을 경우는 불명' 으로 표시하도록 합니다．

Web了03苕
C) -)IM(FcoftInternet
E:pior늚，踞맴m ,,：∼： ，…瓦쿄鐵斟薑無念無弊匹發
P뒤로 ,

J 그 소 괴검색 J」쥴겨찾기 ?UIOth J-:5-＝夕섐姓婢聾解轉瑟發器

Web 관련 서적 목록

」

IS비 고드
서적
저자
출판사
가걱
l 받간일
1S6N89-314 U42-x HTML 긔자인 비주얼 가이드
C仄）
영진닷컴＂i&c.cx而훤仁oJ1-c-11
ISBN89-314-1978-3 ASP사전
니시자와 나오키 영진닷훼15,a:o.ox원F2c01-11-3o
ISBN89-314-2014--5 10일만에 배부는＼risuaC++ 6.0 Seto Haruka
영진닷컴＂5,a0.oco웜12c02-02-05
ISBN89-314-1994-5알짜PC숑어 사천
슈와시스템
앙진닷레19,5
（刃嚥刃剛2W2-01-c
Youngjin.com Y

小나藎샀；
…
큔…쁘…

緘｝완弓

…

- ，尸
堪lL卄 暫퓨E1

===== PAGE 139 =====
138 =====
books.xsl
<?xml version="l.O " encoding= "EtJC-KR " ?>
<xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transfonn' 蟹
version="l. O ">
<xsl:output methods 'html ' encodings "EUC-KR" I>
[

1

< [

3

name="tblAtt ">

<xsl:attribute name= "border">l</xsl: attribute>
<xsl:attribute name="width">500</xsl: attribute>
<xsl:attribute names "align" >center</xsl :attribute>
</1

3

>

<xsl:template match="/ ">
<html>
<head>
<title> <xsl:value-of select="books/@title" I>
</title>
<link rel= "stylesheet" type="text/css" href="books.css" I>
</head>
<hl><xsl :value-of selects "books/@title" /></hl>
<table [

〕>

<tr>
<th>ISBN 코드＜/th>
<th＞서적＜/th>
<th＞저자＜/th>
<th＞출판사＜/th>
<th＞가격＜/th>
<th>발간일＜/th>
<Itr>
<xsl : apply-templates select= "books" I>
</table>
<div>.zxsl:value-of select="books/owner" /></div>
</htrnl>
</xsl : template>
〔

]

</xsl : stylesheet>

……

===== PAGE 140 =====
139 =====
제4일 고도의 ×SLT+α 테크닉

inc.xsl
<?그αnL version="l. O " encoding= "EtJC-KR" ?>
<xsl : stylesheet xmlns:xsl="http:I/ www.w3 .orgI1999IXSL/Transform
version="l. O ">
<xsl:template match="books">
<xsl:sort select= 'price ' data-type="nuinber" order="ascending"

I>

<xsl: for-each select= 'book'>
<tr>
<td nowrap="nowrap"><xsl:value-of se1ect= "@isbn" I>
<Itd>
<td nowrap= "nowrap">
<xs1=va1ue-of select= 'name" I>
</td>
<td nowrap= "nowrap">
<xsl:value-of select= "author" /></td>
<td nowrap="nowrap">
<xsl:value-of select="pu.blish" I>

m시

</tㅍd>
<td nowrap= "nowrap'>
<xsl:vaiue-of se1ect="forr【｀at-number(price, '00, 000. 000 ' ) " />원
</td>
<td nowrap="nowrap"><xsl:value-of seiect="pDate" /></td>
</tr>
</xsl : for-each>
</xsl: template>
<Ixsl : stylesheet>

해답은 책 끝에 毫＞

===== PAGE 141 =====
140 =====
QQI

Less。
n 1。 Less。
n 12

DOM 프로그래밍
드디어 DOM(Document Object Model)이 등장합니다．
지금까지는 미리 준비된 XML 문서와 XSLT 스타일 시트를 정적으로만 연결했지만 이 DOM을 이용함
으로써 이들을 다이내믹하게 편집하여 보다 유연한 조작을 실현할수 있습니다．
우선 오늘은 仄)M을 사용하여 XML 문서를 읽고 참조하는 내용부터 학습합니다．

===== PAGE 142 =====
141 =====
오늘 공부할 내용들
DON을 사용하여 XL 문서 읽기
자硼 문서에서 요소 추출하기
）驪孔 문서에서 속성값 추출하기

===== PAGE 143 =====
142 =====
,

DOM을 사용하여 XML 문서 읽기
지금까지 다뤄온 ×SLT는 XML 문서에 고정적으로 연결된 정적인 것에 지나지 않았
습니다. 이것들을 동적으로 변환하고, 조작해가는 것이 DOM의 역할입니다. 여기서는
먼저 ><ML 문서를 DOM으로 읽어들여 간단히 표시합니다．

disp.html

mcreuott Internet Euplorer

스

0XML

磁

학습 내용 미리 보기

=H 立교Less。
n 10
Lㄴ쿄Q&a

(?bml versiun="L〔rP>
<?om卜stvlesheet tvoe="text/xsr hrel=books.osl' ?>
<books 例e=Web 관련 서적 목록“>
<owner address="www, vounqiin. corn) Voungitn.com Y </owoer>
<book isbn=iSBNBS引4기742=u)
<name> HTML 디자인 비주얼 가｛JI드＜fname)
<author>C. l.S</authnr>
<category개TML</category>
<url>htto://wwwsounqi[n com</url>
［l<／口
『fce> <price>1泊며
<publish＞영진닷컴 </sublish>
<pDate>2el- 馬 R/oDate>
</boak>
<book isbn=iSDN89-3l4-t918-3'>
<nanue> ASP 사전 <Jname>
<author>니시차와 나오키 </author>
<category> ASP</category>
<ud>http//www.younqjin,corn</url>
<川ce기5〔n〕
</otfce>
<publish> 영진딧컴 <／ㅁu비1oh>
<pDate> 2［〕
（〕
ㅐ 卜30<InDate>
<Aroek>
<book isbn="lS8N89引4-1394-5'>
<name>먈짜 PC 용머 사전 </name>
<au甘，
or> 슈와 시스템 <Iauthor)
<category>컴퓨터 사천 <Jcateqorg>
<price> 19hO)<Inrice>
<publish> 영진닷컴 <IoubIish>
mDate> 2302- 0t-05</oDote>
<Ibook>
<book isbn="ISBNt9-3t4-2014S>
<name> t0 Effl II? VisuI Cu. S
"으0(/
<authur>Setu Haruka<
nome>
<un> http://www. youngjirr.
/author>
com </utb
<category>tesual C.
<price> 15113J<
<publi。
h> D Iprice>
<。Date> 21112-。2-0h<Irr。
</publish>
ate>
<Ibook>
(/books)

XML 문서를 읽고
대화상자를 표시한다

-.</category>

1

"

`' Prlnf

,

이번어臣三0OM 프로그래밍의 도입편으로，기본 중의 기본이 되는 XML 문서의 호출에 도전해 봅니다．
DOM은 XML- 문서로 잡근하기 위한 단순한 인터페이스에 지나지 않으므로 특정 언어를 요구하지는
않습니다．이 책에서는 브라우저에서 가장 일반적으로 쓰이는 Javascript를 채택하기로 하는데，
JavaScrip뻬 그다지 익숙치 않으신 분은 관련 서적으로 기본 구문을 학습하기 바랍니다．

===== PAGE 144 =====
143 =====
재5임 DOM 프로그래밍 ①

※U2]폴더에 있는bookaxiul을[D51폴더에 복사해 두기 바랍니다．

1 새문서를열어리스트의코드를입력한다．
리스트 : disp.htmI
<htn1>
<head>
<title>5-1.XME』 문서를 읽어본다＜/title>
<script lang-uage='JavaScript' '>
<!

-

-

var objDoc=new ActiveXObject ( 'Mson12 .DOMDocuinent ' ) '
objDoc .async=false;
objDoc . load( 'books.xinl " > '
window.alert (objDoc .xml) ;
II- ->
</script>
</head>
<body>
<hl>5-1.XMl』 문서를 읽어본다＜fhl>
</body>
</html>

'

'-

F.
,
~' …
1"- "
耳

.
: I
`

2

d파서의
．『
파서의 ㅂii
버전

.

"

MXvflA를 메인 XML 파서로 사용하고 있는 경우는 6행의 DOMDocument를 DOM
Document40으로 기술해야합니다．

입력한코드를［D5］폴더에dizp.html이라는이름으로저장한다．
DOM의 확장자는

『스타일시트화倒정해진확장;
}- 71지고있지는011Cf
I= =J mM은X毗문서와XSL
I

'

t 'I. ', -.L

브라우저상에서 동작할 경우에는 '.html' 로，ASP와 같은 서버측 환경에서 작동할 경우에

는 '.as1f로구분합니다．

3

[D5］폴더를열어disp.html를실행한다．

自

===== PAGE 145 =====
144 =====
저장한 IfI耿江L 문서 disp.html을 익스플로러에서 직접 동작시킵니다. 화면에 XML 문서의 내용
이 표시되면 성공입니다．
XML 문ㅅ居 조작하는 DOM
DOM(Document Object MOde1）
이란 그 이름 그대로 XML 문서의 각 요소와 속성, 텍스트 등을
일반적으로 조작하기 위한 도구와 같은 것입니다. 지금까지는 단순하게 미리 준비된 Xlff과 XSLT
를 표시했지만,DOM을 통해서 비로소 문서를 동적으로 변환하거나 문서를 갱신하는 행위가 가능
해집니다．

'

우선 여기에서는소스가작동하는 대략적인 흐름을살펴보기로 합니다．
_
【작동의 흐름】

문서의 태그가 읽힌다

!
태그 내에 기술된 DOM 프로그램이 작동

!
문서를 읽은 결과가 표시된다

'
버튼을 클릭하면 남은 태그가 읽혀진다

DOt［은 그 자체가 단순한 도구에 불과하므로 이를 조작하는 언어는 무엇이든 상관없습니다. 이
책에서는 브라우저상에서 가장 일반적으로 사용되고 있는 JavaScript를 채택하기로 합니다
.
(JavaScript어］대한자세한내용은관련 서적을참조하기 바랍니디）
JavaScript를 ffl

문서에 삽입하려면다음과겉끼 기술합니다．

<script language= 'JavaScript">

4

===== PAGE 146 =====
145 =====
제5일 DOM 프로그래밍 C)

이 시작 태그 ＜泳ript）
에서부터 종료 태그 </script> 사이에 기술한코드는JavaScript로써 해석하
태그를 해석할 수 없는 버전의 브라우저에서 스크립트 부분을 주적문으
여 처리됩니다. 또 <script）
로
（<!-- ∼ //-->) 처리합니다．
2 XML 문서를 호출한다
JavaScript를선언하면, 먼저 모든조작에 우선하여 조작할대상인 xll문서를호출합니다．
（요소들의 계층 관계）
를
DOM은 미리 XML 문서 전체를 메모리에 로드하고, 내부적으로 트리 구조
생성한다음그후의 조작을 실행합니다．
6, 8행을봅시다．
var objDoc=new ActiveXOl功ect《 'Msau12 . DOMDocumerit " ) '
objDoc.load('books. mil") ;

6행에서는XMLDOMDocument2 오브젝트를 생성하고, 이것을 변수 objDoc에 저장하고 있습니
다. 이 시점에서 생성된 XMLDOMDocument2 오브젝트는 말하자면 XML 문서를 다루기 위한 도
구에 지나지 않으며, 그 안에는 아무것도 들어 있지 않은 상태입니다．
r` ,-rn 1，
」八1〃ㄱ｀一→n－…ㅟ－ n
L^ LJJ_ j.)'JiiUOL LU1FU1i L '

(Th F-I XI ㄷ ㄹ I U ㅁ XI k-IF-Lt
그＝== '＝식스＝ 言 Afl. . ‘ㅢ dj《가＝=

U k ii
八r－커」

var 변수명＝:neW ActiveXObj ect ( "Msxnil2 . DOld: ocunient " ) '

변수명

임의의 변수명을 기술합니다．

※ 다만, MSXML4부터는 각 오브젝트를 버전 지정 형식으로 지정해야 합니다．
MSXML2.DOMDocument는 MSXML2.DOMDocument4.0으로 기술해야만 합니다．

이 비어 있는 도구에 실제로 문서를 저장하는 것이 8행의 load 메소드입니다. load 메소드는 지정
된 XJ띠문서를XMLDOMDocument2에서 해석 완료된 상태로 저장합니다．
즉, XMLDOMDocument2 오브젝트는 이 시점에서 비로소 구체적으로 조작할 수 있는 XML 문
서가되는 것입니다. 이는매우간단하지만DOM이 XML문서를다루는데 있어서의 공통된 절차이
，小一7`

,^1

기도합니다．

小

===== PAGE 147 =====
146 =====
r1 'S一ㅋ
L.,-'.,(1'-'

nfl 人 ㄷ Ut 니시，
lI- --=-=-1 "I- ,I

변수명, load( 1' 문서의 경로명" ) '

변수명

XML 문서 데이터를 저장하고 싶은 XMLDOMDocument2 오브젝트를 기술합니다．

문서명

불러내고 싶은 XML 문서의 경로명을 확장자를 붙여 작성합니다．

XML 문서의 호출을 비동기로 실행한다
도구의 생성
（6행）
과 내용의 호출
（8행）사이에들어 있는 한문장은 무엇일까요？
objDcc .async= false;

실제로 브라우저상에서 작동시켰을 경우는 이 문장과 관계없이 결과는 동일합니다. 그러나 일단
서버
（리모트 컨트롤）
에 표I入4I」
, X}dL 파일을 저장한 경우에는 7행의 한 문장이 생략되면 에러가발
생합니다．
async는XML문서의 비동기 호출을 가능하게 할지의 여부를 결정하기 위한프로퍼티입니다．
즉, 서버상에 xll 문서를 저장한 경우, 문서를 읽는 데 약간의 시간 지연이 발생합니다. 그럼에
도 불구하고 비동기 호출을 유효하게 했을 경우, XML 문서 자체는 읽히지 않는데도 클라이언트가
＇'라는 경고가발생합니다．
비동기로다음작업을수행하려 하므로 “아직 처리할수 없습니디
처음에는 작동 환경이 서버측인지 클라이언트측인지에 상관없이 원칙적으로 asmc 프로퍼티를
false
（비동기가 아님＝동기）
로 설정해 두는습관을 길러두면 실수하지 않을 것입니다.
자계－ 문서를 그대로 표시힌）
다

崙暢器落

를확인“'낟惶뺀型些뮈"를그대로대화

window,alert (objDcc .xml) ;

x끄〕l 프로퍼티는 오브젝트가 나타내는 XML 문서를 그대로 출력하기 위한 프로퍼티입니다. 앞으
로 DO乙
［을 사용하여 XML 문서를 조작할 경우, 그 결과혹은 진행 상황을 쉽게 확인하고 싶을 때가
있을것입니다. 이러한디버그작업시에도 이 x 1IJ프로퍼티는매우유효합니다．
또, XML문서가 아닌 텍스트를 얻고자할 경우에도 text 프로퍼티를 이용합니다．
wiridow.alert (objDcc . text) ;

===== PAGE 148 =====
147 =====
①
제5임 DOM 프로그래밍．

`-'

∼*

여기에서의 ×ml은 얼핏 보기에 확장자로 보이지만, 어디까지나 프로퍼티명입니다. 틀리지 않도록 주의합시다．

∼
·DOM은 )<ML 문서에 접근하기 위한 기능을 갖춘 도구 상자입니다．
·XMLDOMDocument2 오브젝트는 ×ML 문서를 저장하기 위한 도구와 같습니다. 생성된 시점에서는 아직 내용이
없는 공백 상태입니다．
（동기 호출）
로 설정해 둡니다．
·async 프로퍼티는 ×ML 문서의 호출 방법을 제어합니다. 보통 囹se
· 실제로 XML 문서를 불러내고 XMLDOMDocument2 오브젝트로 저장하는 것은 load 메소드입니다．

夕

Lesson7의 실력 테스트에서 외부 XSLT 스타일 시트 table.xsl을 읽고 그 내용을 대화상자로 표시하
는DOM 프로그램을작성해서 [D5]폴더에 저장해 봅시다．
해답은 책 끝에 今

奉

===== PAGE 149 =====
148 =====
；ㅔ.일DOM프로그래밍①

.^

"

XML 문서에서 요소 추출하기

■

9,

호출한 ><ML 문서에서 요소를 추출하는 방법을 학습합니다．

(

fl

학습내용미；
"
"-

elm .卄r.ht倒
(owner address="www,youngjin.corrf>Youngjin,cam Y. </owner>

i XML

J>

ㄴ -q Less。n 11

youngiirr.

PT Q&a

<book Isbter'ISBNB9-314--1742-x">
(name새m4L 디자안비주얼 가미드＜/rrame>
<autnor> C,I, S </author>
…
(category>HTML</category>
<url> trttp:/Jwww,
,com<
<price> ll800<
furl>
</publish>
<pubhsh> j pnce>
<pDate> 21J1J1-IJ6--l 1</pDate>
</book>

눙Key Point ) _

J\

Mlcrosoit Internet E지)Iorer
<book isbn:"'lS8N89-314-1978-T>
<name> ASP 사전 </name>
9바h므r＞니시．烈뫄.나오키 </author>
`u련IE뙨gui，
므Mor \/cate99ry1

：二E확밑11EH1

淵柳pi/J驛飜oungjin,
e>)5UUO</price> com<furi>
<publish>염신낫김 </publish>

DOM 프로그래밍이라고 하
면 왠지 어렵게 들리지만，
</book>

요점은 XML이라는 포맷으

<pDate> 20U1m-30</pDate>

로 기술된 데이터를 "어떻
게 효율적으로 읽을 것인
가’（게 관한 것입니다．
이런 의미에서 트리 구조로
된 자elL 문서를 경로 요소
에서 자식 요소, 손자 요소
로 가는 노드 워킹
（노드의

파일
（E)

편집（트） 보기
（）
（)
브

즐겨찾기
（A)

」 소

도구（工） 도움말
（t크…

」검색 三」
즐겨찾기

玗］
卜미디머 ，多 心！=j

－
" 면궐 "

검색）과정은 DOM 프로그
래밍 전체의 기본이라고 해
도 과언이 아닐 것입니다．

5-2.XML 문서에서 요소를 추출한다

이번 Lesson에서는 학습할
念덮LH 컴퓨터

내용은 앞으로 다뤄나갈 복
잡한 )<ML 문서에도 똑같이
적용되므로 의문점이나 불
분명한 점이 있다면 여기에
서 확실히 해결합니다．

的

j

===== PAGE 150 =====
149 =====
재5얻 DOM 프로그래밍 ①

1

새문서를열어리스트의코드를입력한후［D5］폴더에elm_attr.htm이라는이름으로저
장한다．
a스트: elm_attr.html
<html>
<head>
<title>5-2 .XMI』 문서에서 요소를 추출한다＜/title>
<script language= "JavaScript">
<!

-

-

var objDoc=new ActiveXObject ( "MsarJ2.DOMDocument " ) '
objDoc . async=false;
objDoc.1oad( "books. an1") ;
var objRoot=objDoc .documentElement; 치 4引 艮公 ,
var clnCld=obiRoot.childNodes;
I
I
＇ c汰｀
（하
∼m----－只∼－4 l IF 俳刈巴
tOr 1=U;1<c1r1Uic1. ㅗengtfl;1++) i
'
var objNod=clnCld.item(i) ;
window.alert (objNod. unl) ;
}
II- ->
<Iscript>
</head>
<body>
<hl>5-2 .X!U 문서에서 요소를 추출한다＜/hl>
</body>
</html>

2

[D5］폴더를열어elm_attr.html을실행한다．

===== PAGE 151 =====
150 =====
을 익스플로러에서 실행합니다．
저장한IfI爪4L문서 elm_attr.htm〕
화면상에 <owner> 요소, <book> 요소의 내용이 순서대로표시되면 성공입니다. ,

XML 문서의 경로 요소를 구한다
XML 문서를 읽는 하나의 방법으로 트리 구조로 된 x}dI』문서의 최상위 요소노드에서부터 하위
노드로순서대로 접근해가는 방법이 있습니다．
이 방법은 뒤에서 소개하는 것과 겉미 직접 목적 노드로 접근하는 방법에 비하면 비효율적이지만，
모든 仄)M 조작의 기본이기도 하고 결국 아주 신속히 대처할 수 있는 조작이기도 하므로 확실하게
이해하기 바랍니다．
var objRoot=objDoc.documeritElement;
ㅅ 으 크수
documentE1ement -DOM
（이번 예제의 경우는－qx毛趣）
합픈롱軫틴；입니다· 이 프로퍼티는요소노드를나타내는XMLDOMNode오브젝트입니다·

위

XMLDOIV1Node 오브젝트는 <book) 요소와 <author) 요소 등특정한요소나속성 노드를 저장합
니다. 노드의 조작은 이 XMLDOMNode오브젝트를통해서 실행합니다．
자식 요소군을 구힌다
（<books> 요소）
는 그 아래의 모든 노드를 포
경로 요소 또는 제 1요소라 불리는 트리 최상위 요소

childNodes;

.

var clnCld=

objRoot

함하고 있습니다. 하위로 내려가는단계로 이번에는바로 아래의 자식 요소군을 구해봅시다．

childNodes 프로퍼티는 그 결과값으로 XMLDOMNodeList 오브젝트를 나타냅니다．
XMLDOMNodeList 오브젝트는 XMLDOMNode 오브젝트의 집합체이며, 이 경우는 경로 요소
바로 아래의 자식 요소 노드
（<owner> 요소와복수의 <book) 요소）전부를 포함합니다．
3 요소 리스트에서 특정 노드를 검색힌）
다
10행에서 얻은 XMLDOIv1NodeList 오브젝트는 이 상태로는 사용할 수 없습니다. 노드의 집합
체로서 하나로 통합된 상태에서 실제로 조작하기 위해서는 개개의 노드를 검색해야 할 필요가 있
습니다．

150

===== PAGE 152 =====
151 =====
제5임 DOM 프로그래밍 ①

for(i=O; l<clnCld.length;i++) {
var objNod=clnCld.item(i) ;
window, alert (objNod.xrnl) ;

}
length 프로퍼티는 X1v1LDOIvINodeList 오브젝트에 포함되는 노드의 수를 나타냅니ㄷ
卜，
즉, 이번
.
예제의 경우에는 clnCldjength의 값, 즉 아래의 자식 요소 수는 5가 됩니다）
小
!
for(1=n,i<N;i++){

｝는 반복 처리를 하는 경우 사용하는 JavaScript 구문입니다. 초기값 i가 n일 경우, i가 N보

다 작은 동안
（N-i 이하인 동안）처리를 반복합니다. 1회 처리를 반복할 때마다 i는 하나씩 증가出＋）하므로 N-n회
실행됩니다. 이번 예제의 경우라면 N=5, n=0이므로 처리는 5회 반복됩니다．
→－-/

item 메소드는 인수로서 지정된 인덱스 수
（개개 노드의 순번을 나타내는 수. 인덱스 수 0은 첫 번
째 노드를 나타냅니다）
에 근거하여 XML1DOIV1NodeList 오브젝트 내에서 개개의 노드를 검색하여
XIV1LDOMNode 오브젝트로 나타냅니다．
결국, 위의 동작에서는 인덱스 수를 0에서부터 length-i（즉, 4）
까지 하나씩 변화시키면서 노드 집
합에서 요소 노드를 하나 하나, 총 5회 검색합니다．
어떤 의미에서 이 io'-44행의 조작은 DOM 프로그래밍 중에서도 가장 일반적인 방법입니다. 검색
한 요소 노드 아래에 다시 요소가 존재할 경우는 이 일련의 조작을 재귀적으로 반복함으로써 점차

令

===== PAGE 153 =====
152 =====
一

자ALDOMNode 오브젝트가 자꾸 반복되는데, 각 XMLD아ANode 오브젝트의 변수명이 틀리면 각각 다른 것으로
생각해 주십시오. 변수의 수만 다른 XMLDOMNode 오브젝트가 생기고 있는 것입니다．

documentElement ,

childNodes - item

childNodes - item
(name)

(author)

(publish)

(price)

(pDate>

뇨

4 요소를 구ㅎ는 다잉한 빙법
앞의 1'-3단계에서 소개한 내용은 요소로 접근하는 대표적인 방법이지만 유일한 수단은 아닙니
다.DOM에도 목적이나 문맥에 따라 여러 가지 적용방법이 존재합니다．
예를 들어 아래와 같은 경우를 생각해 봅시다．
(1) 첫 번째 자식 요소에 접근하여 순서대로 다음 요소로 이동하고 싶은 경우
10'14행을 아래와 같이 바꿔 봅니다．
var objCld=objRoot . firstChild;
while(objCld!=null) {
window.alert (objCld. xml) '
var objCld=objCld.nextSibling;

}
firstChild 프로퍼티는 현재 요소의 첫 번째 자식 요소를 나타냅니다．
그 다음 nextSibling 프로퍼티로 다음 자식 요소로 이동하면서 xn 프로퍼티가 요소의 내용을 나

다．

타냅니다. nextSibling 프로퍼티는 다음 자식 요소가 존재하지 않을 경우 In皿
（미정의）
을 나타냅니

0

===== PAGE 154 =====
153 =====
제5임 DOM 프로그래밍 ①

夕
while
（조건 A)｛처리 B｝
라는 구문은 조건 A가 참일 동안 처리 B를 반복하는 JavaScript 구문입니다．이번 경우는
"변수 0히Cid가 존재하지 않는다
（n
（川）
는 내용0I 없을 경우
（!=)' , 즉 “변수 0히0ld가 존재할 경우"에 { } 안의 처리를
반복합니다．

(2) 마지막 자식 요소에 접근하여 순서대로 앞의 요소로 이동하고 싶는 경우
10'-14행을 아래와같이 바꿔 봅니다．
var objC1d=objRoot.lastChild;
while (objCld! =null) ……：
window,alert (objCld.xml) ;
var objCld=objCld. previousSibling;

}
lastChild 프로퍼티는 현재 요소의 마지막 자식 요소를 나타냅니다．
그 다음, previousSibling 프로퍼티로 앞의 자식 요소로 이동하면서 요소의 내용을 표시합니다．
previouwSibling 프로퍼티는 앞의 자식 요소가존재하지 않을 경우 flu끄
（미정의）
을 나타냅니다．
(3) 현재 요소의 부모 요소를 구하고 싶은 경우
11∼14행을 아래와 같이 바꿔 봅니다．
for(i=O;l<clnCld.length;i++) {
var objNod=clnCld.item(i) ;
window.alert (objNod.parentNode . unl) '

}
parefitNode 프로퍼티는 현재 요소의 부모 요소
（<books> 요소）
를 나타냅니다. 즉, 이 경우 동일한
부모 요소 아래의 자식 요소에 대해 반복 처리를 하고, 그 부모 요소를 참조하고 있으므로 5회 모두
같은 내용이 표시 됩니다．
DOM 오브젝트는 관겨隱 갖는다
DOM은 상호 밀접하게 관련된 오브젝트의 집합체입니다. 앞으로 DOM을 다뤄나가는 데 있어서
오브젝트 간의 관계를 파악하는 것은 매우 중요합니다．
다음은 DOM의 주요 오브젝트에 관한 상호 관계도를 나타냅니다．

0

===== PAGE 155 =====
154 =====
XMLDOMDocument
i C}cumentE]ement

XMLDOMNode

attributes

XMLDOMN
NamedNodeMap

chidNodes
Item(i∼n)

XMLDOMNodeList

XMLDOMAttribute

Iem(i∼n)

XMLDOMNode

XMLDOM
티ement

XMLDOM
Text

XMLDOM
XMLDOM
EntityReference Comment

XMLDOM
XMLDOM
DocumentType Processinginstruction

그림을 보면 XMLDOMNode는 매우 일반적인 오브젝트임을 알수 있을 것입니다．
즉, 여러 가지 접근으로 얻어진 노드(X1vILDOMNode 오브젝트）
는 그 상황이나 문맥에 의해
로 다뤄지기도 하고, XMLDOMText
（텍스트 노드）
로 다뤄지기도 하
XMLDOME1ement(요소 노드）
는 것입니다．
노드의 종류는 MSXML 파서에 의해 내부척으로 판단되고, 또 그 종류에 따라 다룰 수 있는 메소
드와 프로퍼티도 달라지게 됩니다．

Go 化 XML

"

叫
＇.
· 경로 요소는 document티ement 프로퍼티로 얻을 수 있습니다．
DOM으로 XML 문서를 읽는 경우도 경로 요소가 최초의 기점이 됩니다．
· 한 요소의 바로 아래에 포함되는 자식 요소군은（가' ldNodes 메소드를 통해서 얻을 수 있습니다．
ChildNodes 메소드는 1개 이상의 XMLDOMNode 오브젝트의 집합체인 )(MLDOMNodeUst 오브젝트를 나타냅
니다．
·XMLDOMNodeUst 오브젝트의 item 메소드는 내부에 포함되는 XMLDOMNode 오브젝트를 나타냅니다. 인덱스
수는 0에서부터 시작된다는 점에 주의합시다．
·DOM의 각 오브젝트는 프로퍼티와 메소드의 값으로 서로 연관되어 있습니다．
상호 관계를 의식하여 프로그래밍한다는 점이 매우 중요합니다．

===== PAGE 156 =====
155 =====
제5일 DOM 프로그래밍 ①

sict.html은XML문서 report.xml에서 <creator> 요소를추출 · 표시하기 위한DOM 프로그램입니
다. 리스트의 공백을 채우고 프로그램을 바르게 완성시켜 주십시오．
Micro帥卄 r,te」re. E>:p!orer.

(creator> 요소의 데이터가 대화 상자로 以 된다

report.xml
<?xmi. version= 'l. 0" encoding= "EUC-KR" ?>
<reports>
<report day="2001-07-21'>
<header>
<title＞출장 LiiL</title>
<creator＞김미정＜/creator>
<Iheader>
<bㅇdy>
··· 본문 생략 …
</body>
</report>
</reports>

sct.xmI
<html>
<head>
<title>5-2 . 실력 테스트＜/title>
<script language='JavaScript">
-

]
]

objDoc.load( [

I

) '

var objRot=objDoc. 〔

,JkYt,

〕'
iteir

od,

childN.

objRot.

var
objR.
ep=
es.
(0) ;
var ox刀a
（그r=ox）
그上
《ep· cniia?ioues · 1teIt`u/ ;

var objCrt=objHdr . childNodes.item( 〔
window.alert (objCrt. f

,

^4?( " 汁0, '

〕 '

）낏끼
,,

I,, );

小

나l·

var objDoc=[
objDoc . async= [

",

-

"'

!

ㄴ싸

<

l

.

===== PAGE 157 =====
156 =====
//- >
-

<Iscript>
<Ihead>
<body>
<hl>5-2.실력 테스트＜/h1>
</body>
</htna>

해답은 책 끝에 今
`

●STEP UP! ●

XSLT와 DOM의 차이
앞의 Lesson에서 소개한 XSLT도 ×ML 문서에서 특정 노드를 추출하여 가공하기 위한 언어입니다．
그렇다면 D0M과 ×SLT의 차이점은 무엇일까요？ 또, D0M은 ×SLT와 어떻게 구분해서 사용하면 좋을까요？
실제로 ×SLT와 D0M은 어떤 면에서는 매우 유사한 특성을 가지고 있습니다. 그러나 XSLT가 현재 있는 그대로의
XML 문서를 결정할 수 있는 규칙에 따르는 정적인 장치라 한다면, D0M은 XML 문서와 XSLT 스타일 시트를 동적으
로 연결하거나
（예를 들면, 동일한 데이터를 일람표 형식으로 보이거나 단순한 표 형식으로 보이는 등）편집 " 가공하기
위한 동적인 장치입니다．
XML과 XSLT에만 주목한다면 b(ML이 오히려 HTMLJ보다 작성하기 번거롭고 어떤 장점이 있는지 알 수 없다"라는
생각을 갖게 될지도 모릅니다. 그렇지만 D0M을 배움으로써 ×ML과 ×SLT를 동적으로 연결하는 유연성과 간단한 조작
을 가능하게 하는 인터페이스를 HTML이 대신하기 어렵다는 사실을 실감할 수 있을 것입니다．
이 책의 제 9일 · 제 10일에서는 이러한 ×SLT와 D0M의 상호 보완적인 기술 연동의 테크닉에 머무르지 않고 "그렇
다면 실제로 이러한 D아예 프로그래밍이 어떠한 상황에서 사용되고 있는가？' 하는 실용적인 예를 소개하고 있습니다.
자lL을 우리들이 살고 있는 생활에 연결지어 봄으로써 단순한 기술 습득에만 머무르지 않고, 실용적인 지식으로까지 높
일 수 있도록합니다．

4
XSLT는 XML 문서를
정적으로 변환, 분리하는 장치

XML문서

DOM은 )(ML 문서를
동적으로 조작하는 장치

===== PAGE 158 =====
157 =====
제5일 DOM 프로그래밍 ①

Go to XML

===== PAGE 159 =====
158 =====
제5일 DOM 프로그래멓 ①

XML- 문서에서 속성값 추출하기
XML

XML 문서의 속성값에 접근하는 방법을 학습합니다．

학습 내용 미리 보기
h elm attr.html
1SBN89-引4-1142-x
○XML

ISBN89-3l4-l978-3

스－｀勻 Less。
nU

L r-1 Q&a
1S8N89-314-1994-

,X

-5

H쫠맙H::：」

집( )

보기
《y)

.

1S6N89-314-2014-5

푤겨찾기
（스） 도구
（工） 도움말（土1)

드〕소

a검색 」」즐겨찾기 守미디머 J

已，
J

5-3,XML 문서에서 속성값을 추출한다
陋환亶

뇨프1th 컴퓨E1
(bo아◇ 요소의 isbn 속성을 대화상자에 표시한다

I Key Point )
XML- 문서는 많은 종류의 노드로 구성됩니다. 접근 빈도가 가장 높은 것은 요소지만, 속성에도 상당
히 가깝게 접근합니다. 속성은 요소에 비해 정보를 세분화 · 계층화하고자 할 때의 유연성은 없지만
정보를 완벽하게 보호 · 유지할 수 있는 장점이 있습니다．

===== PAGE 160 =====
159 =====
제5임 DOM 프로그래밍 ①

I

Lssonlt에작성한DOM스크립트elm_attr.htm을열어리스트의코드를추가하고그대
로 저장한다．
리스트 : 이m_attr.mn기

<htnil>
<head>

<script language= ' JavaScript ">
<!

-

-

var objDoc=new ActiveXObject ( 'Msximj2 . DoMDocument" ) '
objDoc .asyric=false;
objDoc.load( "books.xxni") ;
var objRoot =objDcc. documentElement;
var clnCld=objRoot. childNodes;

'I-

-

>

</script>
</head>
<body>

</body>
<Ihtin1>

폴더를열어elm attr.html을실행한다．
205］

===== PAGE 161 =====
160 =====
저장한I了I뇨4L문서를 익스플로러에서 실행합니다．
화면상에 <owner> 요소, <book> 요소의 내용이 순서대로 표시되면 성공입니다．
요소 내 속성군을 추출힌다
먼저 Lessonil과같은 순서로 <book> 요소에 접근합니다．
for 루프의 카운터 변수 1가 좀전과 달리 1부터 시작하고 있는 것은 첫 번째 요소 <owner> 요소를
점프하고 두 번째의 <book) 요소를빼내기 때문입니다．
for(i=1;i<clnCld.length;i++) {
var objNod=clnCld.item(i) ;
var clnAtr=objNod.attributes;

}
에 포함되는 모든 속성군을 포함하는
（<book) 요소）
13행의 attributes 프로퍼티는 요소 노드
XMIJDOMNamedNodeMap 오브젝트를 나타냅니다．
XMLDOMNamedNodeMap 오브젝트는속정 노드를나타내는XMLDOMNode 오브젝트의 집합
체로 이 경우는 <book> 요소의 isbn 속정을 포함합니다. 여기서는 실제로는 하나의 속성만을 포함
하므로 하나의 내용만을 집합체로 간주하고 있습니다.

2 속성 리스트에서 특정 속성값을 추출츤파
XMLDOMNamedNodeMap 오브젝트에서는 item 메소드를 통해서 isbn 속정 노드를 나타내는
XMLDOIv1Node 오브젝트를 추출할 수 있습니다. 인덱스는 0부터 시작하므로 인수에 0을 지정합니
．
다
（결국 0은 가장 첫 번째의 속성 노드를 가리킵니디〕
속성 노드의 값은 검색한XMLDOMNode 오브젝트의 text 프로퍼티를통해 접근할수 있습니다．
var objAtr=clnAtr.itexn(O) ;
window. alert (objAtr. text)

===== PAGE 162 =====
161 =====
棚1

｀一 ＇

14씨5행은 하나의 문장으로 작성할 수 있습니다．
window.alert (clnAtr.item(O) .text) ;

즉, 여기까지의 흐름을 정리하면다음과 같이 됩니다．
（objRoot）
의 자식 요소
（cinCid）
를 두 번째부터 하나씩 순서대로 접
books. in](o1jDoc）
의 경로 요소
（objNod）
의 속성군
（clriAtr）
에서
근해가면서 (for (1=1;i<c1nC1d.1ength;i-H-):- :), 이 1번째 자식 요소
최초의 속성
（objAtr）
을추출하고, 텍스트로표시합니다
（vindow.a1ert(bojAtr.text);).
3 속성값을 구하는 여러 가지 빙법
프로그래밍 언어에는 동일한 내용을 여러 가지 방법으로 표현할수 있습니다. 이것은 이 D0M 오
브젝트에서도 마찬가지입니다. 속성값 혹은 속성 노드를 구하는 여러 가지 메소드를 열거해 놓았으
니 참고하기 바랍니다. 또한 이 메소드들을 사용함으로써 13-45행의 기술이 어떻게 바뀌는지 살펴
보기 바랍니다．
물론, 이 자리에서 모든것을한번에 외울필요는 없습니다. "이런 방법도 있었나2"하는가벼운마
음으로 살펴 보기 바랍니다.
(1) getNameditem
var clnAtr=objNod. atrributes;
var objAtr=clnAtr . getNamedltem( '" isbn' ) ;
window.alert (objAtr . text) '

XMLDOMNamedNodeMap 오브젝트에 대해서 인덱스 수가 아닌 속성명으로 접근합니다. 복수
개의 속성이 다르게 기술되어 있는 경우에 편리합니다．
(2) getQualifiedltem
var clnAtr=objNod.atrributes;
var objAtr=clnAtr.getQualifiedltem( "isbn", "") ;
window.alert (objAtr. tex비 ;

===== PAGE 163 =====
162 =====
getNamedTtem 메소드와 마찬가지로 속성명으로 XMLDOMNamedNodeMap 오브젝트에 접근
（<table xsl:use-attribute-sets='Thil"〉
라면 xsl：의 부분）
를
합니다. 제 2인수에는 이름 공간 접두사
지정하여 이름 공간의 속성에 접근할 경우에 편리합니다．

(3) getAltributeNode
var objAtr=objNod.getAttributeNode《 "isbn" 》'
windows,alert (objAtr. text);

getAttributeNode 메소드는부모 요소를 나타내는 XMLDOMNode 오브젝트에 대해서 속성명을
키로 사용하는속성 노드를 나타냅니다．
XIvIL]JOMNamedNodeMap 오브젝트를통하지 않0므로 보다간결하게 기술할수 있습니다．

(4) getAtrribute
:window,alert (objNod.getAttribute("isbn' ) 珏굽

가장 간단히 속성값에 접근할 수 있는 방법입니다. getAtrribute 메소드는 XJV1LDOMNode 오브
젝트에 대해서 속성명으로 접근하여 직접 속정값을구할수 있습니다．
이렇게 한 가지 일에 대해서 다양한 방법이 제공되고 있는 것은속성값의 취득에만 해당되지 않습
［은 메소드와프로퍼티라는 형태로 여러
니다. 요소의 취득과추출, 변수등모든 행위에 있어서 DOd
가지 방법을 제공하고 있습니다．
반복되는 이야기지만, 처음부터 모든 것을 알아둘 필요는 없습니다．
다만, 때로는 이를 실행하기 위한 다른 방법이 더 없는지 조금 더 깊이 있는 자료를 참조해 보는
것도좋을것입니다. 보다효율적이고, 보다다양한수단에 대한힌트가마련되어 있을것입니다．

Go to XML
∼
· 요소 노드에 포함되는 속성군을 구하려면 attributes 프로퍼티를 사용합니다．
attributes 프로퍼티는 복수의 속성 노드를 포함하는 XMLDOMNamedNodeMap 오브젝트를 나타냅니다．
·XMLDOMNamedNodeMap 오브젝트에서 개개의 속성 노드를 추출할 경우에는 여러 가지 방법oj 있습니다
(item, getNamedltem, getoualifiedltem).
·XMLDOMNode 오브젝트에서 직접 속성으로 접근할 수도 있습니다
（getAttributeNode, getAttribute).

===== PAGE 164 =====
163 =====
제5일 DOM 프로그래밍 ①

[D5] 폴더에 복사한books.Xn1에서 <owner> 요소의 address 속성을추출하여 표시해 봅시다．
이 때, 적어도 세 가지 방법으로 도전해 보기 바랍니다．
※ 힌트 :
·attribut ; 프로퍼티를 사용합니다．
·getAttributeNode 메소드를 사용합니다．
·getAttribute 메소드를 사용합니다．

해답은 책 끝에 4>

===== PAGE 165 =====
164 =====
Lesson 13- Lesson 15

DOM 프로그래밍
계속해서 ㄸ)M을 살펴봅니다．
제 5일에서는 DOM에 의한 XML 문서의 검색에 대해서 배웠습니다. 지금까지의 XSLT, xPath의 학습
에서 트리 구조의 개념을 보다 체계적이고 명확하게 이해했으리라 생각합니다．
이번 Lesson에서는 이러한 기본 개념을 토대로 XML 문서를 DOM으로 작성합니다. 이번에 학습할 내
용은 앞으로 XML 문서 작성의 기본적인방법이 되고마지막날
（제 10일）
의 응용편으로 연결되는 중요한
내용이므로 확실히 이해하기 바랍니다．

===== PAGE 166 =====
165 =====
오늘 공부할 내용들
r 요소 추출하기
' XML 문서에 노드 추가하기
'XML문서 갱신 " 삭제하기

===== PAGE 167 =====
166 =====
d`13

x1I
,,1flflL4U,1'IW O

요소 추출하기
이번 Lesson에서는 복잡한 )<ML 문서에서 요소와 속성을 효율적으로 추출하는
방법과 노드 정보의 취득 방법 등을 학습합니다．

■ 학습 ㅐ용미리보기
"

公

I select.html

눈\

@XML

Microsoft Internet Es이orer

Less。
n 13

aai
nulI
Di專亨
cE
(EtOIEl
1/element
i6f):xsI:sort
I 0I
):sort
htp//werw.w"
org/1999/X5LJTranstorrn
자요소가 있는가：false

나 ㄱ Q&.

16니．
직접 요소를 추출한다．- ]，川crosoft Internet E＞側Orer
파일IF)

편집（트＞

보기선I

즐겨찾기
（A)

도구
（工） 도욤말
（土i)

舍
주소
（흐나亡，
『： WxmlW5.anpIsWEEWselect (tin

塞 a245/
-Li71
＝」【슭미동

6-1. 직접 요소를 추출한다

추출한요소의 쨘큰룔 표시 -

(, Key Point ) _
XSLT에사는 요소와 속성 등 ×ML 문서상의 노드를 검색하기 위해 xPath를 사용했恪니다. xPath는
약간 특수한 구문이지만, 대상을 효율적으로 추출하기 위해 최적화된 언어입니다．
실제로 D0M에서도 이 xPam를 사용하여 효율적인 노드 검색을 할 수 있습니다. 이번 Lesson을 통
해 ×Path에 대해 한 번 더 복습함과 동시에 지금까지의 DOM 프로그래밍과는 조금 다른 접근 방법
을 살펴보기로 하겠습니다．

===== PAGE 168 =====
167 =====
黨疊

※ [D6] 폴더에 [D4] 폴더의 books.xsl, books.xml을 복사해 둡니다．

새문서를열어 리스트의 코드를입력하고, [D6］폴더에 select.htm'이라는이름으로저장
한다．
리스트 : select.html
1.

<html>

2

<head>

3

<title> 6-l . 직접 요소를 추출한다＜/title>
</head>
<script language= 'JavaScript '>
<!

-

-

var objDoc=new ActiveXObject ( "Msxml2 . DOMDocument " ) '
objDoc . async=false;
objDoc.load( "books.xsl ") ;
var clnSrt=objDoc.selectNodes( "xsl: stylesheet//xsl: sort") ;
for(i=O;i<clnSrt.length;i++) {
objSrt=clnSrt. item(i) ;
str= " 이름 공간 접두사：" + objSrt.prefix + "\r " '
str+="OI름 공간URI: " + objSrt.namespacetJRl + " \r" '
（기본）= " + objSrt.baseName + "\r";
str+='' 노드명
（전체）
: " + obj Srt . nodeNaxae + "\r " '
str+=" 노드명
8tr+= "노드형＝" + objSrt.nodeType + "I '
+

∥

\r

1

"

+ objSrt.nodeTypeString

;

str+=" 정의된 데이터형＝ " + objSrt.dataType + "\r " '
str+='' 자식 요소가 있는가＝ '' + objSrt .hasChildNodes 0;
window,alert ( str) '
}
醜
一

II- ->
</script>
<body>
<hl>6-l . 직접 요소를 추출한다＜/hl>
</body>

;J;

</htxn그＞

===== PAGE 169 =====
168 =====
폴더를열어select.html을실행한다．
2ux］

저장한 IfI取4L 문서 select.html을 익스플로러에서 실행합니다. 화면상에 鈿1:sort) 요소에 관한
대화상자가 표시되면 성공입니다．

1 요소에 직접 접근츤파
지금까지 仄OM에 의한노드의 검색은 경로 요소에서 순서대로 자식 요소, 손자 요소를 검색하거
나트리 구조에서 검색하는방식이 사용되었습니다, 이 방법은 일반적으로충실하게 적용할수 있는
효과적인 검색 수단이지만, 실용적인 측면에서 볼 때, 耶4L 문서에서 사용하기에는 그리 효과적인
방식은아닙니다．
이 방식을 개선한 것이 여기에서 소개하는 selectNodes 메소드입니다. 10행을 보기 바랍니다．
var clnSrt=objDoc.selectNode引"xsl:stylesheet//xsl:sort" ) '

selectNodes 메소드는 지정된 xPath식에 적용되는 노드를 포함하는 Xlv1LDOMNodeList 오브젝
트를나타냅니다. 이 경우 <sl:styiesheet) 요소 아래의 모든 <xsl:sort> 요소를추출합니다．

I.

戚，

xPath식0私1 'II' 는 복잡한 경로를 기술하지 않고, 한 노드 아래에 있는 전체 노드를 추출하는 연산자입니다．
그러나 무조건 트리 내의 전체 노드를 검색하기 때문에 부하가 매우 높은 연산자이므로 함부로 사용하지 않는 게 좋
습니다．
7

，뇨_

만약 이 방식 대신 기존의 방법으로 노드를 추출한다면, <xsl:stylesheet> 경로 요소에서
鈿l:templat> 요소, 鈿l:for-each> 요소, 白s1:sort> 요소로 접근해야 하므로 번잡한 프로그램이
.
（한번, 넉습을 겸해서 시도해 보십시오）
될 것입니다
실제로 DOM 프로그래밍을 실행할 경우에는 selectNodes 메소드로 최초의 기점이 되는 노드로
직접 접근한후, childNodes와 parentNode 등의 프로퍼티를 이용하여 개별 노드를 참조하는 2단계
방법이 효과적입니다．

===== PAGE 170 =====
169 =====
꺼6임 DOM 프로그래밍 ②

r 《그r>1 ∼卄小1∼극‘令.

1 口ㄷ ㅗ口｀
r ㄴㅗ｀ㄴJ\J口.

혜JcOI
니∥」－--j

Iㅢ시］

/\i ㄱJ

var 변수명 1＝변수명 2. selectNodes( " 추출식" )
변수명 1:

selectNodes 메소드에 의해 표시된 xMLDOMl1odeList 오브젝트를 기술합니다．

변수명 2:

추출원이 도는 요소 노드
（XMLDOMNode 오브전겯트） 또는 xM1』 문서(a'4LDOMDocument2
오브젝트》
룔 7슐합니다．

추출식

구하고 싶은 요소, 속성으로의 경로를 xPath식으로 기술합니다．

4- 요소에 직접 접근하는 다양한 방법
selectNodes 메소드 이외에 요소에 직접 접근하는방법을소개합니다．
(1) getElementsBylagName 메소드
10행을 아래와같이 明긱 봅시다．
var clnSrt=objDoc . getElementsByTagName (∥xsl : sort" ) '

이름이 <xsl:sort＞인 요소만 추출하고 복수 노드의 집합쳬인 XMLDOIv1NodeList 오브젝트를 나
타냅니다．
이방법은Thll 문서 내의 한특정 요소를 전부 추출하고 싶은 경우에 이용합니다. xPath식의 'II,
연산자와 비슷하지만, xPath식이 '//' 의 왼쪽에서 어느 정도 대상을 압축할 수 있음에 비해，
getElementsByIhgName 메소드는모든XML문서를참조하므로부하가더 높다고할수 있습니다．
(2) selectSin이eNode 메소드
10'-21행을 아래와같이 바꿔 봅시다．
var clnSrt=objDoc. selectSingleNode ( "xsl: styelsheet//xsl:sort") ;
if (clnSrt '. =null) {
window. aler디”노드를 찾지 못했습니다“) ;

1

」…

…

}
selectSingleNode 메소드는 이름처럼 인수의 xPath식에 적용되는 노드만을 추출하기 위한 메소
드입니다. 단일 노드를나타내는XMLDOMNode 오브젝트를 나타냅니다．
위의 예와 같이 대상 노드가 존재하는지의 여부를 알고자 할 경우나 대상 노드가 하나 밖에 없음
을미리 알고 있는 경우에 selectSingleNode 메소드를사용합니다．

===== PAGE 171 =====
170 =====
3 노드 정보를 나타내는 다양한 프로퍼티
추출한 노드에 대해서 이번에는 여러 가지 부가 정보를 표시해 보기로 합니다．
l.

for (i=O;i<clnSrt.length;i++) {

1j

objSrt=clnSrt. item(i) ;

1:

str= '~이름 공간 접두사：" +objSrt. prefix + "\ r " '

lq

str+=" 이름 공간 URI: ' + objSrt.namespaceuP.I

l
1{

（전체）= " + obj Srt . nodeName + ''\r '' '
str+ r '' 노드명

1r

str+=" 노드형＝ " + obj Srt . node叱／pe + "/ " + objSrt . nodeTypeString +

'~

\r~

+ "\r " '

str+=”노드명
（기본）
: " + obj Srt . baseName + " \r";

'

'

str+=“정의된 데이터형＝" + objSrt.dataType + "\r" ;
str+= "자식 요소가 있는가＝" + objSrt.hasChildNodesO;

1'

window, alert (str) ;

}

小

·"str+=XXX"는 놔r=str+XXX"의 생략형입니다．
· ' \r' 는 줄 바꾸기를 나타내는 특수 문자입니다．
· 이외에 ' \t'（태그 문자）
와 ' \n,（복귀）등을 사용할 수 있습니다．

가 속한 URI
（즉，
（예제의 경우, <xsl：∼）
namespaceURl 프로퍼티는 이름 공간 접두사
를 나타냅니다. 또, 기본
<,xsl:stylesheet> 경로 요소에서 xslns:xsl 속성으로써 선언되고 있는 UEJ）
이란 이름 공간 접두사를 뺀 요소의 원래 이름만을 나타냅니다. 동일한
명
（baseName 프로퍼티）
（prefix 프로퍼티）
XML 문서 내에서 복수의 이름공간을사용할 때, 사용하고 있는요소명이 접두사
（nodeName프로퍼티）
인지, 그렇지 않으면 기본값인지가매우중요합니다．
를포함한전체명
nodeType 프로퍼티는 그 노드가 요소인지 속성인지, 그렇지 않으면 다른 형태언지를 수치로 나
타냅니다. nodeT嬅tririg 프로퍼티는nodelype에 대응하는문자열을 나타냅니다．
（문자열형인
dataType 프로퍼티는 앞으로 소개할XML 스키마에 있어서 정의된 노드의 데이터형
지, 수치형인지 등：을나타내는 것입니다. 이번 Lesson의 books.xsl에서는XML 스키마가 존재하지
않으므로 프로퍼티는 null을나타냅니다.
마지막의 hasChildNodes 메소드는 해당 요소가 자식 요소를 가지고 있는지의 여부를 true/false
로 나타냅니다. 반복적으로 자식 요소, 손자 요소로 접근해갈 경우, 하위 노드가 존재하고 있는지의
여부를 판정하는 것이 중요합니다．

===== PAGE 172 =====
171 =====
제6일 DOM 프로그래밍 ②

-

1r

Go to XML
·selectNodes, selectSin이eNode 메소드는 xPath식에 적용되는 단일, 또는 복수 노드를 추출합니다．
·get티ementsByTagName 메소드는 태그명을 키로 하여 ×ML 문서 전체에서 요소 노드를 추출합니다．
·DOM에는 노드 정보를 참조하기 위한 프로퍼티와 메소드가 있습니다，

books.xsl에서 모든 柚1:value-of> 요소의 select 속성을 추출해 봅시다. 이 때 속성명, 노드형 및
값을 대화상자로 표시해 주십시오．
해답은 책 끝에 今

●STEP UP! ●
Dr.XML과 나미의 원포인트 강좌

이름 공간이란？
나미

XML을 공부하면 이름 공간이란 단어가 자주 나와요 별로 익숙치 않은 단어인데, 한마디로 말하면 무엇일
까요？'

Dr. XML

"음, 한마디로 설명하기가 좀 어려운데… 굳이 말하자면 '요소와 속성명의 다툼을 막기 위해 각각의 이름이
어느 그룹에 속하는지를 결정하는 장치' 라고나 할까…"

나미
Dr. XML

"박사님, 너무해요. 잘 모르겠어요. 한마디로 설명하지 않으셔도 좋으니까 자세히 설명해 주세요'
"사물을 처음에 외울 때는 노력을 아끼지 말아야 해요. 자, 그렇다면 잡지 기사를 나타내는 자vIL 문서를 생
각해 봅시다. 예를 들면 잡지 기사 XML은 저자 정보 ×ML과 기사 정보 )(ML을 조합하여 성립됩니다. 그리
고 저자 정보 ×ML은 저자의 이름으로써 <name> 요소를 정의하고 있고, 기사 정보 XML에서는 기사의 타
이틀로써 <name> 요소를 정의하고 있다고 하면 어떨까요？"

나미

"
'그렇다면 (name> 요소가 2가지 의미를 갖게 되죠．

Dr. XML

'그렇습니다. 저자 정보 ×ML과 기사 정보 자1L을 합친 잡지 기사 ×ML에서는 2가지 의미를 갖는 (name>
요소가 발생하게 되고, 문서 내에서 저자명을 추출하고 싶을 때, 어느 (name) 요소를 빼내면 좋을지 알 수
없게 되죠. 이렇게 되면 HTML의 櫛）
태그가 문서의 타이틀을 나타내고 있는지, 키워드를 나타내고 있는지
"
구별할 수 없는 것과 같은 의미를 갖게 됩니다．

나미
Dr. XML

"그러면 안 되잖아요．
'
（뻬
"그래서 이름 공간이 등징하는 겁니다. 이름 공간은 같은 이름의 요소를 구별하기 위해 각각의 요소명 오
접두사를 붙입니다. 예를 들면 <author:name>, <article:name）
과 같이,.."

나미

'
"어？ 2개의 <name) 요소가 전혀 다른 것으로 됐네요．

小

===== PAGE 173 =====
172 =====
Dr. XML

에 속하는 <name) 요소와
"그렇죠 XML은 이 이름 공간 접두사라 불리는 접두사에 의해 <author: --'）
(articlev'-'＞에 속하는 <name> 요소의 2가자로 구별할 수 있게 됩니다．
XML이 태그를 자유롭게 정의할 수 있다고 해도.. 언제나 하나 하나 태그 세트를 정의해 가는 것은 한계가
있고, 그렇게 되면 태그의 설계자매각 다른 규칙이 생기게 됩니다. 그래서 이미 있는 태그 세트들을 자신이
사용하기 쉽게 조합할 수 있다는 것도 XML의 커다란 매력 중 하나입니다. 따라서, 0I 이름 공간이 있어서
복수의 태그 세트가 서로 충돌하지 않고 공존할 수 있게 됩니다. 알겠어요 나미얻p'

나미

' 네！"

瘢

===== PAGE 174 =====
173 =====
제6잎 DOM 프로그래밍 :2)

Go to XML

===== PAGE 175 =====
174 =====
제f2i flOM 프로그래밍 ②

XML 문서에 노드 추가하기
불러낸 )<ML 문서에 대해서 새로운 요소와 속성을 추가합니다．

학습 내용 미리 보기

스 (?xfl
ygrs,
Iehoe
o,
(boOkPo
b。
ebkl.O?>pe
ibnS8N-3l4t742eeVeel諶某
。。nge,
x>
c。e)Y。
?>.dn.c。e
<e p, >FflM1EJXP
I k 7 E/ fl ee
< thor> C S<
<ta*a ory>
/epthe>
yPr9, c n ,
HTMLVcategory>
w*
<paee> I
<I
l>
5!vice>
</ ubivib)
<puWIsh>

14

-

.

縕緞ubn=<SBNfl9-3t4-I978- >

L쿄 Q&a

;;l多，
冕機簪隘難，
,’y,

（b
三目

pDcic>h>
)2-Ol

u/pO。
le>

融eh>

\

鰍으鰻h, =10RNR>-OlA-2flI&-c,

二

MfluObI’ 。>
pt</name>
Jouthor>
<outhor>
Tadanon
<pilcu> l
<<ate
0
</pnc。
>jovasc,
>
ipl</cale
<(ID留，
upobIish'
。>。)
<<D。
le>
2 l,Wl1
)4b。
，

\

Lesson

ㅗ

.

write

html

○XML

-1

파일(F)

4-

（트） 보기
（:/)
편집

뺘

3

（스） 도구
（끄
플겨찾기

도욤말
（브）

」 公 烈검색 ＝」즐겨찾기 딘卜미디어 ,J 心，" 면궐 "

6-2.XML 문서에 노드를 추가한다

J
d,
厘

괴뫈료

泮집된XML문서를 대호冷7뻬표시한이
（●"Key Point )
DOM의 기능은 미리 준비된 XML 문서를 읽는 것만은 아닙니다. 새로 ×ML 문서를 구축하거나, 기
존의 XML 문서에 대해서 노드를 추가 · 삭제하는 기능도 함께 갖추고 있습니다. 이로써 XML 문서
가 단순히 하나의 '데이터' 에 머무르지 않는 '데이터 베이스' 로, 정보의 동적인 축적 매체로 활용할
수 있게 돠는 것입니다．

4

===== PAGE 176 =====
175 =====
2)
제6일 DOM 프로그래밍 「．

1

새문서를열어디음리스트의코드를입력하고［恥］폴더에write.htm'이라는이름으로저장
한다．
21스트 : write.html
<html>
<head>
<title> 6-2 .XNL 문서에 노드를 추가한다＜Itit1e>
</head>
<script lariguage= "JavaScript" >
<!

-

-

var objDoc=new ActiveXObject ( "Msaiii2 .DONDocument" ) '
ob」
Doc . async=false;
objDoc.load( "books.xml") ;
var objRoot=objDoc .documentElement;
var ob§Book=objDcc . createElement ( "book" ) '
var objISBN=objDoc . createAttribute( "isbn") ;
objISBN. text="ISBN99-999-9999-9";
var objNam=ol功Doc . createElement《 "name" ) '
objNam. text=" 홈페이지에 바로 활용하는 JavaScript";
var ob:jAuth=objDcc.createElemen니"author" ) '
objAuth.text="Tadanori Matsuo";
var objCate=objDoc . createElement ( "category") ;
objCate.text="JavaScript";
var objLog=objDoc.createElement ( "logo") ;
var objPub=objDcc . createElemen니"publish" ) ;
objPub. text= " 영진닷컴" ;
var objPrc=objDcc .createElement ( "price") ;
objPrc , text= "18000 " ;
var objDat=objDcc .createElement ( "pDate") ;
objDat.text="2001108117 ";
objBook. setAttributeNode (obj ISBN) ;
objBook. appendChild(objNam) ;
objBook . appendChild(objAuth) ;
objBook. appendChild(objCate) ;
objBook. appendChild
（아）
jLog) ;

===== PAGE 177 =====
176 =====
objBook.appendChild(objPub);
objBook.appendChild(objPrc);
objBook.appendChild(objDat);
objRoot.appendChild(objBook);
window.a1ert(ob:jDoc. om1);
II-->
</script>
<body>
<hl>6-2.XML』 문서에 노드를 추가한다＜/hl>
</body>
</html>

폴더를열어write.html을실행한다．
2ux］

저장한I了I戮江L문서 write.html을 익스플로러에서 실행합니다．
화면상에 xll」
문서어］새로 추가한 <boo) 요소가표시되면 성공입니다．
1 새로운 요소 노드를 생성한다
데이터를 추가하기 전에 우선 새로 삽입할 각 요소의 노드를 생성합니다. 이 단계에서는 아직 상
호 계층 관계를 의식할 필요는 없습니다．
먼저 createElement 메소드를 이용하여

ook> 요소를 작성합니다. var objBook으로 변수

objBook를 설정합니다. 그리고 books. an1을 저장한 변수 objDo쩨 createElement 메소드를 사용
하여 (book) 요소를 작성합니다. createElement 메소드는 인수로 작성하고 싶은 요소명을 작성합
니다．
var objBook=ob」
Doc . createElement ( 'book") ;

===== PAGE 178 =====
177 =====
제6일 DOM 프로그래밍 ②

4rLLL
n1n八
., →－一1=`1
볍口L口￡』I_ㄷ上II JiI.

ri I ㅅ「 （기 니 k 円
u1l＝
￡＝==
"I "- LI

var 변수명 갸＝변수명 2. createElement ( “요소명" )
변수명 1

createElemerit 메소드에 의해 생성된 속성 (XMLDOMNode 오브젝트）
을 기술합니다．

변수명 2

요소를 추가할 대상이 되는 xML 문서
（x1dLDODocument2 오브젝트）
를 기술합니다．

요소명

새로 생성할 요소명을 기술합니다．

마찬가지로각각 <book>, <name>, <author>, <category>, <logo>, <publish>, <price>, <pDate>
요소를 생성하며 텍ㅅㅌ 노드를 가진 요소에 대해서는 앞의 Lesson에서 소개한text 프로퍼티를 사
용하여 텍스트를 설정합니다．
var objNam=objDoc. createElement ( "name" ) '
objNarn. text=" 홈페이지에 바로 활용하는 JavaScript";

다른 요소에 대해서도 같은방식으로 작성합니다．
요소 노드의 현재 상태는 서로 연관되어 있지 않고 각각분산되어 있는상태입니다．
【분산된 노드】

createElement,
createAttribute
메소드로 만들어진
노드는 아직
분산된 조각 상태

(publish)
(pDate)

(category)

(logo)

(author)

(name)

===== PAGE 179 =====
178 =====
새로운 속성 노드를 생성한다
속성을 생성할 때 요소와 같은 방식으로 작성합니다．
createAtthbute 메소드를 사용하여 우선 노드라는 기구를 생성해두고, 내용 텍스트를 설정합니
다. 요소노드와마찬가지로생성된 isbn속정은어느요소에도속하지 않고독립된상태입니다．
var objISBN=objDoc .createAttribute ( "isbn") ;
objISBN. text="ISBN9-99999-999-9";

L一．
＾스4-＾시H→｀= 찧，
1d= ^
LㄴㅗCOtCfl. .'.,L .L.JU Lt

r,JI A r- (I
L1lIa===H

iJ人I1
^ r 펴』

var 변수명1＝변수명2 . createAttribute ( " 속성명” )
변수명 1

createAttribute 메소드에 의해 생성된 속성 (XMLDOMNode 오브젝트）
을

변수명 2

요소를 추가할 대상이 되는 xMI』 문서
（)1dLtXJMDocument2 오브젝트）
를 기술합니다．

요소명

새로 생성할 요소명을 기술합니다．

기술합니다．

또한, create∼계의 메소드에는 이외에도 생성할 노드의 종류에 따라 아래와 같은 메소드가 있습
니다．
메소드명

구문
인수
createCDATASection

CDA丁A 섹션 노드
var objCDAT=objDoc.createCDATASection(strDat)
objCDAT : XMLDOMCDATASection 오브젝트
strDat : 문자 데이터

createComrnent

코멘트 노드

var objCom=objDoc.createComment(strDat)
아)jCom : XMLDOMComment 오브젝트
strDat : 문자 데이터
createDocumentFragment

문서의 단편
var objFrg=objDoc.createDocumentFragment()
objFrg : XMLDOMDocumentFragment 오브젝트

===== PAGE 180 =====
179 =====
제6일 DOM 프로그래밍 ②

createEntityReference

:

「참조노드
」실처
var objER=objDoc.createEntityReference(strER)
야)iER : XMLD0MEntityReference 오브젝트
strER : 실체 참조명

createProcessin이nstruction

처리 영령 노드
var objPl=objDoc.createProcessinglnstruction(strTrgt,strDat)
objPl : XMLD0MProcessin以nstruction 오브젝트
strlrgt : 대상명, strDat : 애플리케이션에 주어지는 데이터

createTextNode

텍스트 누ㄷ
var objTxt=objDoc.createTextNode(strDat)
obTxt : XMLD0MTextNode 오브젝트
strDat : 텍스트 데이터

※ 아)jDOC : XMLDOMDocument 오브젝트

3 속성 노드를 요소에 설정힌다
생성된 속성 노드와요소는 서로 연결시켜야 합니다．
현재 분리되어 있는 상태의 속성 노드를 요소 노드에 연결시키는 것은 setAttributeNode 메소드입
니다．
setAttributeNode(ob寸ISBN);

이것으로isbn속성은 仍ok) 요소
（dㅋj玆珏0의 속성이 되며 <book isbn='ISBN99-999-9999--出）
와
같은요소가생성됩니다. 그러나이상태에서는요소와xTh문서 자쳬는 연결되어 있지 않습니다．
4 속성 노드를 생성히는 다양한 방법
속성 노드를 생성하는다른방법을 설명하겠습니다．
(1) setAttribute 메소드
샘플의 12, 13행을 삭제하고 26행을 아래와 같이 바꿔 써 봅시다．
obiBook.setAttribute( ' i8bfl, '15BN99-999-9999-9') 朴

요소에 대해서 쉽고 간단하게 속성을 추가할 때 가장 좋은 방법입니다. setAttribute 메소드는 제
1인수에 속성명을, 제 2인수에 속정값으로 설정하고 싶은텍스트를 지정합니다．

===== PAGE 181 =====
180 =====
(2) setNarne비tern 메소드
샘플의 12, 13행을 그대로 남겨두고 26행을 아래와 같이 바꿔 써 봅시다．
var clnAtr=objBook,attributes;
clnAtr. setNamedltem(obj ISBN) ;

setNamedltem 메소드는 요소에 속하는 속성군
（XMLDOMNamedNodeMap 오브젝트）
에 대해서
새로운속성 노드를 추가합니다. 이미 XMLDOMNamedNodeMap 오브젝트가 생성되어 있는 경우
에 효과적인 접근방법이라고할수 있습니다．
5 요소 노드를 만들어 XML 문서에 삽입힌다
앞에서 설명한 것처럼 creathElement 메소드로 생성된 각 요소 노드는 생성편 단계에서는 아직
xll문서와는분리되어 있는상태입니다．
따라서 이 요소 노드에 계층 구조를 만들 필요가 있습니다. 이 계층을 만들어 주는 것이
appendChild 메소드입니다．
우선 가장 먼저 <book> 소에 미리 만들어 둔 자식 요소군을 추가합니다. appendChild 메소드
는추가된순서대로 자식 요소의 맨마지막에 요소를추가해 나갑니다.
objBook. appendChild(objNam) ;
objBook. appendChild (objAuth) ;
objBook. appendChiid (objCate) ;
objBook .appendChild(objLog) ;
objBook . appendChild(objPu1D) ;
objBook. appendChild(objPrc) ;
objBook. appendchild(objDat) ;
objRoot.appendChild(objBook) ;

27--32행에서 <book> 요소와 그 아래 자식 요소군의 계층 관계가 확정되면 마지막으로 33행에서
<book) 요소를 경로 요소
（<books> 요소）
에 추가합니다．
r

-

-- 」／헥1 」 ㄱ =

비

`dpyenqㄴnㅗㅗα 비l二亡스＝디 시｛긔』

변수명 1.appendChild( 변수명 2)
변수명 1

（x1LDOMDocuinent2 오브젝트）
를 기술합니다，
요소를 추가할 대상oj 되는 xl표』문서

변수명 2

를 기술합니다．
（XMLD04Node 오브젝트）
createElementㅍ 메소드에 의하1 생성된 요소

===== PAGE 182 =====
181 =====
제6일 DOM 프로그래밍 ②

또, appendChild 메소드는 insertBefore 메소드로 변경할 수도 있습니다．예를 들면，33행은 아
래와같이 바꿔쓸수 있습니다．

insertBefore 메소드는 제 1인수에 지정한 요소를 제 2인수에 지정한 자식 요소 바로 앞에 삽입합
（미정의）
로 합니다．
니다. 이 경우, 마지막에 요소를추가하기를 원하므로 제 2인수는 null

4

1
--

.create '-')ㅖ 메소드는 개개의 노드를 생성합니다. 생성된 직후의 노드는 서로 상호 관계를 갖지 않는 조각과 같은
상태입니다．
· 속성을 요소에 연결지으려면 setAttribute나 setAttributeNode, setNameditem 메소드 등을 사용합니다．
· 생성된 노드를 XML 문서에 추가하려면 appendChild, inseriBefore 메소드 등을 사용합니다．

-

제 2일 Lesson 5聊00kS.XSI를 DOM에서 동적으로작성해 봅니다．
（오름차순）
을추가
테이블이 표시될 때의 정렬키가출판사, 출판일순으로 되어 있는데, 제 1키로 가격
합니다．
해답은 책 끝에 듣＞

===== PAGE 183 =====
182 =====
제6일 DOM 프로그래밍 (2

XML 문서를 갱신 · 삭제하기
노드는 추가되기만 하는 것은 아닙니다．
이번 Lesson에서는 노드를 변경
（갱신）
하거나 삭제하는 방법에 대해 학습합니다．

학습 내용 미리 보기

fl edit.html

(7000 00r5i0n＝실l.B?>

J\

窈oHotyIOOh. e tp.neavnar hrof boak.eIl?>
<b.아n5bn＝갸S8聿qt걋〕3!4一17421》

@XML

<name)
<auth。r>Hi
C稽＜鷺0
<juniOr>tI주일가미드(/00010)

(nni叩0rH?HTML(/setn9015)
nun> ntiS:jJwumnyoungjln.>oIT,
<pnce> tt0JJ<j rice>
vliri,

솝－＼勻 Less。
n 15

<pua柚> a刀H拓－∥ <／口Date>
(/00011>
(0001101bfl= lS0NI→314-lOt83)

L 1ㄱ Q&a

<un,<tipi/Ieee u.youngiin seen
<price> l5aJRj fl
<publich>
._
<I
ue>
<pDal。
>
I-Il- </pteete>
ublish)

,

<name) t11tPC Lh A}31<
<
/000ee>
<aathee>
M
euisol>
E1
</cal040,
<001,9015>
y>
<publlsh>
<price>
I 。l I<.
ubIi
<I
<pDate>
</pDnie>
h>

/ 가mnir}

-Ul

rine>

,

Jae Stripl</namo> <author> Tadanod
Matoe,o</,sthor> <cale o >PHP</caregonni> <toaopcp,
<Ipubbah> <<rise> l
1/l7qpD。
>
。。11) <,1en。
kn,
1>。1 l/I。
</piice> <pDa。
hltnh>

驪6-3. XML 문서를 갱신．
삭ㅈi한다 - Microsoft Internet Es하orer
파일吃） 편집
（트）

보기
（y,

즐겨찾7l(스） 도구
（J.)

J

중지

〕

새로고침

도뭄말
（土1>

r立l
菩

ㅢ

검색

＝」

j

즐겨찾기

6-3.XML 문서를 갱신·삭제한다

戚

편집된 XML 문서를 표시

/'KAy Pciint ' _
학습 내용이 점점 어려워지고 있으니 현재 자신이 어느 노드를 대상으로 하고 있는지, 각각의 노드가
어떤 상태에 있는지 하나 하나 확인하면서 학습하기 바랍니다．

===== PAGE 184 =====
183 =====
Dㅇ
卜才프로그래망必

1

새문서를열어리스트의코드를입력한후［珊］폴더에edit.html이라는이름.0로저장한다．

리스트 : edit.html
<html>
<head>
<title> 6-3 .XMI, 문서를 갱신 · 삭제한다＜/title>
<Ihead>
<script language="JavaScript ">
<므

-

-

var objDoc=new ActiveXObject ( "Msxml2 . DONDocument" ) '
objDcc .async=false;
objDoc.load( "books. anl") ;
var objRoot=ob」
Doc . documentElement;
objRoot.removeAttribute( "title ") ;
var clnChld=objRoot.childNodes;
objRoot.removeChild(clnChld. item(0) );
var objBook=objDcc. createElement ( "book") ;
var objISBN=objDoc .createAttribute( "isbn") ;
야dISBN.text="ISBN99-999-9999-9 " '
var objNam=objDoc . createElement ( "name") ;
아力Nam. text=“홈페이지에 바로 활용하는 JavaScript";
var objAuth=objDoc . createElement ( "author") ;
objAuth. text= "Tadanori Matsuo";
var objCate=objDoc . createElement ( "category") ;
objCate.text="PHP";
var objLog=objDoc.createElement ( "logo") ;
var objPub=objDcc . createElement ( "publish" ) '
objPub. text=" 영진닷컴" '
var objPrc=objDoc . createElement ( "price" ) ;
objPrc.text="l8000";
var objDat=ob:jDoc.createElement ( "pDate") ;
objDat.text="2001/08/17 ";
objBook. setAttributeNode (objISBN) ;
objBook. appendChild(objNam) ;

===== PAGE 185 =====
184 =====
objBook.appendChild(objAuth);
objBook.appendchild(objCate);
objBook.appendChild(objLog);
objBook.appendChild(objPub);
objBook.appendChild(objPrc);
objBook.appendChiid(objDat);
objRoot.replaceChild(objBook,objRoot.lastChild);
window.alert(objDoc.xml)'
II-->
</script>
<b《〕
dy>
<hl>6-3 .XM1』 문서를 갱신 · 삭제한다＜/hl>
</body>
</ht;1m.>

폴더를열어eclit.html을실행한다．
2 [' ］

저장한I{I入4L문서를 익스플로러에서 실행합니다．
화면상에 <book) 요소의 title 속성, <owner) 요소가 삭제되고 새로 생성된 <book> 요소가 기존
의 (book> 요소로바뀌면 성공입니다．
1 요소를 삭제한다
<owner> 요소를삭제하겠습니다. 소스 코드의 12, 13행을 보기 바랍니다．
var clnChld=objRoot . childNodes;
objRoot .removeChild(clnChld.item(O) );

를 지정
（XIV1LIDOIV1Node 오브젝트）
removeChild 메소드는 인수로 삭제하고 싶은 자식 요소 노드
합니다．

===== PAGE 186 =====
185 =====
'

-

--

---- ＇져1- 』 기 =

LIernoveLI1JJ.u

n】 *

尸

fl l

J

AIl

볘소스＝쒸 "1<긔I

변수명 1.removeChild( 변수명 2)
변수명 1

삭제할 요소의 부모 요소에 해당하는 요소
（XMLDONNOde 오브젝트）
를 기술합니다．

변수명 2

삭제하고 싶은 요소
（)1LDOMNode 오브젝트）
를 저장할 변수명을 기술합니다．

속성을 삭제한다
(books> 요소의 title 속성을 삭제합니다. 11행을 봅시다．
var objRoot.removeAttribute ( 'title ") ;

removeAttribute 메소드는 인수로 지정된 속성을 삭제합니다．
r

LL ㅂLLIUV

kLLi

1-.,,A- ^
ijJLLLU

rlJIAr OI IJAIl
U기그＝==＝ㅢ 八r커J

변수명 1.removeAttribute
（속성명）
변수명 1

를 기술합니다．
삭제할 속성이 속해 있는 요소
（U1LDOMNode 오브젝트）

속성명

삭제하고 싶은 속성의 이름을 기술합니다．

속성 삭제에는 이외에도 다음과 같은 방법이 있습니다．
(1) removeQualifieditem 메소드
var clnAtr=objRoot,attributes;
clnAtr.rexnoveQualifiedltem( "title ", "' ) ;

속정군
（XJV1LDOMNamedNodeMap 오브젝트）
에서 특정 속성을삭제합니다．
removeQualifiedltem 메소드의 제 1인수에 속성명을, 제 2인수에는 이름공간 접두사를 지정합니다．
주로 이름 공간 접두사를 동반한 속성을 조작할 경우에 사용합니다．
(2) removeNameditem 메소드
var clnAtr=ob§Root.attributes;
clnAtr.reinoveNamedltem('titlen) ;

===== PAGE 187 =====
186 =====
에서 특정 속성을삭제합니다．
속성군cxMLDOMNamedNodeMap 오브젝트）
removeQualified Item 메소드와다른 점은 이름 공간을 명시적으로 지정할수 없다는 점입니다．
(3) removeAttributeNode 메소드
var objTtle=objRoot.getAttributeNode ( "title '' ) '
objRoot .removeAttributeNode(objTtle) ;

XMLDOIV1Node 오브젝트에 속하는메소드로, 인수에는속성 노드를 지정합니다. 이미 대상이 되
는속성 노드가특별히 정해져 있는 경우에는 이 메소드들을 사용합니다．
心 요소를 치환힌다
마지막의 <book> 요소를 새로 생성한 <book) 요소로 치환해 봅니다. 소스 코드의 38행을 보기
바랍니다．
objRoot . replaceChild(objBook,objRoot.laseChuld) ;

, 제 2인수
replaceChild 메소드에는 제 1인수에 새로삽입한요소 노드0UVILDOMNode 오브젝트）
에는 치환하고 싶은 요소 노드를 지정합니다. 마지막 <book> 요소를 치환하므로 이것을 lastChild
프로퍼티로구합니다．
r`fㅂ Pㅗ口ㄴUㄴ
n

1
mI 人「 n [ j i ii
ㅛㅗㅗu 배스＝=＝디 시 ‘긔A

변수명 1.replaceChild( 변수명 2' 변수명 3)
변수명 1

（xlLDOMNode 오브젝트）를 기술합니다，
치환하고 싶은 요소의 부모 요소

변수명 2

（XMLDOMNode 오브젝트）
를 기술합니다，
변수명3으로 지정된 위치에 새로 삽입할 요소

변수명 3

를 기술합니다，
（XMLDOMNode 오브젝트）
치환할 대상이 되는 요소

4 XML 문서를 저징힌다
실제로는 갱신된 XML 문서는 단독 파일, 혹은 데이터베이스로 저장되지 않으면 의미가 없습니
다. 따라서 MSXIVIL 파서에서는 save 메소드를 이용하여 아주 간단히 조작 결과를 파일로 나타냅
니다．
objDoc.save( "output. anl") ;

===== PAGE 188 =====
187 =====
제6일 DOM 프로그래밍 ②

r

- ----

`8aye

nil A n

fl i

tJ Ai`

1J∥소＝=＝ㅢ 시《끅』

변수명. save《 저장 위치）
변수명

저장하고 싶은 札虹』문서《XM1DOMDocumeut2 오브젝트）
를 기술합니다，

저장 위치 xlα』문서를 저장할 위치의 경로를 기술합니다．

유감스럽게도 이번 Lesson이 전제로 하고 있는 클라이언트측 환경에서는 디스크의 내용을 갱신
하는 등의 조작은 허용되지 않지만, 앞으로 JavaServlet이나 ASP(Active Server Pages) 등을 이용
한서버 프로그래밍에 도전할 경우를 위해 꼭 외워두는 게 좋을 것입니다．
-

· 요소를 삭제하려면 removeChild 메소드를 사용합니다，
· 요소를 치환하려면 replaceChild 메소드를 사용합니다．
·속성을 삭제하려면 removeAttribute, removeQualifiedNameditem, removeNameditem,

`,

removeAttributeNode 메소드 등을 사용합니다．

를DOM에서 동적으로 편집해 봅시다．
제 2일 Lesson 5의 books.xs］
（오름차
테이블을 표시할 때의 정렬키가 지금은 출판사, 출판일순으로 되어 있는데, 제 1키로 가격
순을 최상의 요소와 치환합니다．

4,.

I

===== PAGE 189 =====
188 =====
凡

DTD（문서 형식 선언）
는
여기에서 잠시 주제를 바꿔서 DTD(Document Type Defmition：문서 형식 정의 ）를힉습합니다. Un）
이제까지 자유롭게 기술해온 XML 문서에 어떤 일정한 틀을 부여하는 것으로 보다 정밀한 데이터 교환
을 가능하게 합니다．
이제까지 학습한XSLT나DOM과긷미 기술내용끼 직접 형태나움직임으로눈어］보이는 것이 아닌 만큼
좀처럼 이해하기 어려울지도 모르겠지만 실제 XML 문장과 대조해가면서 추상적인 功
［D 기술을 표시
가능한구쳬적인 형태로서 이해할수 있도록 노력합시다．

===== PAGE 190 =====
189 =====
오늘 공부할 내용들
XML 문서 안에서 urn 작성하기
XML 문서 밖에서 DTD 작성하기

===== PAGE 191 =====
190 =====
XML 문서 안에서 DTD 작성하기
이번 Lesson에서는 약간 이해하기 어려운 DTD(Document Type Definition : 문서
형식 선언）
에 대해서 학습합니다．

학습 내용 미리 보기

fl b。。ks.xml

파밂L)

-

-

\지

（三）

XML

긷두1로 .

Lesson 16

L □ Q&a

-- -

〔－蛔mm巫
편집
（트） 보기
（V)
畛

J

믈겨찾기
（스） 도구（工以

繃〕 仝

-- .-

=1Jj J

도옴말
（姓

a去검색 二」
쥴겨찾기 ￡.oI디어 J

■
d·

J

-; 」 蜘 ！…연결

軫
^

＇시 1e「5口1= ] 口기 Pn ＂山n仔궁듸 ㅏm r느
u'DOCTVPE books (View Scu,ce 1O, SAl duotype. - 緇
<books t,Ue='Web 관련 서적 목륵' >
<owner address='www.youngjin.com5Yonajln.com Y.c/owner>
<b00k Sbn='18BN.9-.l4} 742出' 》
<name,HTML디자인 비주얼 가미드
（/name>
<author,C.I.Bo/author,
dogoshtml.Jpqcloqo>
<catBgor-v,m 'm_c/category>
<ud,http://www.youngjin.comc/url>
oprioe>11800</poce,
rpubhsh,멈진단컵
《/pubhsh,
<pDate>2001-06-11o/pDate<
<memo,
d`eywords.HTML日그＜/keywnrd,
클 쉽게 이｀
앝 수 밌도꺅 설명한 홱미다．
이 콱믄 크계 써 가지 부분으로 구첨되머 잇다. 첫 변뻐는
TUtoria~ 편으로 HTML의 기초를 말기 쉽게 설명뺐다．
두 번· 는 Reference와 practice 편미다．
여기川서는 류토리얼 튄·서 끼출한 HTML의 기몬적인 기늠·서 나아가 용용 심화 학습을 할 수 있
도륵 하몄다．
月빈·는 8t日P Up 편미다．
c/memo,
<Thook,
<book Isbn=''BBN893l4-l97.-a' >
<nanle>ASP 사전c/name>
<author＞니시자와 나오키＜/authors
cl050>esp.jpgc/l000s
旺〕뫈료

-i

넣내 컴퓨터

-

'i
鹿

Dli) 선언을 동반하는 XML 문서

(, Key Point

)

DTD는 이름 그대로 XML 문서의 형식을 지정하는 것이므로 XSLT나 DOM과 달리 무엇인가 눈에
보이는 동적인 변화가 발생하는 경우는 없습니다. 실제로 DOM과 연동하는 것으로 XML 문서를 동
적으로 검중하고 바르지 못한 기술에 대해서 경고를 발생하는 데이터로 DTD가 존재합니다．
제 7, 8일에사는 문법적인 설명을 우선적으로 다루겠습니다. 그렇다고 [)TD가 단지 구문만으로 존재
한다는 것은 아닙니다. 이번 Lesson에서는 DID에 의한 XML 문서의 형식 선언과 이것이 구체화된
XML 문서를 꼼꼼히 비교하면서 학습하기 바랍니다.

駭

===== PAGE 192 =====
191 =====
（문서 형식 선언）
제7일 DTD

1

[D3〕폴더의books.xml을열어리스트의코드를추가해［D7］폴더에그대로저장한다．
리스트 : books.xml
※ 파란 글씨의 부분이 추가하는 코드입니다．
<?xml version= 'l. 0 " encoding= 'EUC-KR" ?>
2

·，, . ㅗ－/＼小→ ㅗ ㅗrj='

3

< !EL皿ENT books (owner, i∼｀
一 7/

4

< !ELEMENT book (name, author, categoLJ, logo, un1?,

ㅗ．心口人b

1

price, public, pDate, memo) >
5

< !ELEMENT owner (#PCDATA) >

6

<!ELEl1'E;NT name 댜(PCDATA) >

7

dELEMENT author (#PCDATA) >

8

<LELEMENT category (#PCDATA) >

9

dELEMENT url

10

<!ELEMENT price (#PCDATA) >

11

dELEMENT publi跳1 (#PCDATA) >

l2

<LELEMENT pDate 倂PCDATA) >

13

<!ELEMENT memo (#PCDATA - keyword i ref) *>

14

(#PCDATA) >

<!ELEMENT keyword (#PCDATA) >

15

dELEMENT ref (#PCDATA) >

16

< LATPLIST books title

CDATA #IMPLIED>

17

<!MPLIST book isbn CDATA #REQUIRED>

18

<!ATI'LIST ref adclr CDATA #1EQtJIRED>

그．
9
<books title= "Web 관련 서적 목록" >
<owner address='www.youngjin.com'>Yongjin.com Y.
<Iowner>
22

<book isbn="ISBN89-314-1742-x ">

23

<name>HTNL 디자인 비주얼 가이드＜/riame>

24

<author>C.I. S</author>

2

<logo>htxnJ. . jpg</logo>

2

<categony>HTML</category>

2;

<url>http: //www.yourigjin.com <furl>

28 i

<pnice>11800<Iprice>

29 '

<publish＞영진닷컴＜/publish>

===== PAGE 193 =====
192 =====
<pDate>2001-06-11< /pDate>
<memo><keyword>HTMI』태그＜Ikeyword＞를 쉽게 이해할 수
있도록 설명한 책이C…
이 책은 크게 세 가지 부분으로 구성되어 있다．
첫 번째는 ㄸutorial 편으로 W2ff』
의 기초를 알기 쉽게 설명했다．
두 번째는 Reference와 practice 편이다．
여기에서는 튜토리얼 편에서 제출한 HTML의 기본적인
기능에서 나아가 응용 심화 학습을 할 수 있도록 하였다．
</memo>
세 번째는 Step Up 편이다．
</book>
33

<book isbn= 'ISBN89-314--1978-3 ">

34

<name>ASP 사전＜/name>

3S

<author＞니시자와 나오키＜Iauthor>

36

<logo>asp. jpg</logo>
<category>ASP<Icategory>
<url>http: IIwww.youngjin.com </url>

39

<price>15000</price>

40

<publish＞영진닷컴＜/publish>

41

<pDate>2001-11-30< /pDate>

42

onemo><keyword>ASP의 모든 명령을 내 포켓 속에＜/keyword>
'Poket Reference ASP 사전은
ASP의 기본적인 지식과 사용 가능한 명령의 구문, 구문에 대한 상세한 설명, 명령 활용
예를 ASP 오브젝트，ADO, FileSystemObject의 메소드, 프로퍼티로 분류하여
언제든지 쉽게 찾아 참조할 수 있도록 한 사전식 레퍼런스입니다</memo>

43 ㅣ </book>
44 :

<book isbn= nISBN89-314--1994-5 '>
<name＞알짜 PC 용어 사전＜/name>
<author＞슈와시스템＜Iauthor>
<logo I>

48 :

<category＞컴퓨터 사전＜/category>
<price>19500<Iprice>
<publish＞영진닷컴＜/publish>
<pDate>2002-0l-05</pDate>
<memo＞이 도서의 특징은 줄임말
（약어）
에서 풀네임을
찾거나 풀네임에서 줄임말을 쉽게 찾을 수 있도록 도와준다．
；또한 삽화를 통해서 이해하기 어렵거나 생소한
</rnemo>
용어에 대해서 이해도를 높이고 있다．
</book>

===== PAGE 194 =====
193 =====
（문서 형식 선언）
제7일 DTD

<book isbn= '1ISBN89-314--2014-5">
<name>lO일만에 배우는 Visual C++ 6.0</name>
<author>Seto Haruka< /author>
<logo>vc . jpg</logo>
<url>http: //www.youngjin.com <lurl>
<category>Visual C++</category>
<price>15000</price>
<publish＞영진닷컴＜/publish>
</pDate>2002-02 -05< /pDate>
<lnemo＞이 책은 Microsoft Visual C++ 6.0에 대하I 22개의 단원을 10일 동안
순서대로 학습하도록 되어 있다．Lessonl에서는 간단한 Windows 프로그램을 직접 만들어
봄으로써 앞으로 펼쳐질 이 책의 무궁무진함을 맛보게 한다．
Lesson2부터는 직접 Visual C+＋을 실행하고, 소스를 분석하면서 언어의 기본적인 개념을
잡아 나가고, 마지막 Lesson22에서는 이미 습득한 API 함수 사용법，
리소스 작성법 등을 이용해 Windows 응용 프로그램을 독자 스스로 코딩할 수 있게 한다．
</memo>
</book>
</books>

2 [D7］폴더를열고books.xnα을실행한다．

익스플로러에서 books.xm을 열고 q [L를 적용한 XML 문서가 에러 없이 표시되면 성공입니다．
그러나 DTD는 레이아웃에는 별다른 영향은 주지 않으므로 화면상의 효과는 기대할 수 없고. 구체
적인동작캉식에 대해서는 뒤에 나오는 제 9일 Lesson 20에서 학습하기로 하겠습니다．

1 XML 문서 인에 DTD를 작성힌다
XML 문서
（xnil 파일）
의 일부로 기술되었는지 또는 독립된 외부 파일로서 기술되었는지에 의해
urn
（문서 형식 선언）
는 크게 두 가지로 분류합니다. 전자를 내부 서브 세트, 후자를 외부 서브 세트
라고 부르는데 이번에 다루는 것은 내부 서브 세트입니다．
XML문서는 정확하게는 아래와같이 구성됩니다．

夔

===== PAGE 195 =====
194 =====
[XML 문서의 골격｝

XML문서
XML선언
((?xml?>)

DID
（문서 형식 선언）
※와부 DTD를 인용한다．
요소 형식 선언, 속성 리스트 선언, 실체 선언, 기법 선언

XML 문서 본체
（인스턴스）

즉, 이제까지는 거의 의식하지 못했지만 위의 구문처럼, 엄밀히 설명하면 이제까지 등장한 XMI」
（인스턴스）
만을 기술하고 있었던 셈입니다．
문서는 11그
［D 부분을 생략하고 xTh 선언과xML 본체
books.xml의 예제에서 UP'）
는 2'-'19행에 해당합니다．

〕＞

<!DOCTYPE books [.

dDOCFYPE 경로 요소명［∼l> 뒤어］서술할 요소 형식 선언, 속성 리스트 선언, 실체 선언, 기법
선언등 일련의 문서 형식 정의가 기술됩니다．
UPD를 동반하는 xML 문서는 당연히 끄dL 본문
（인스턴스＞상에서도 】fri〕규칙에 의해 작성되야
（정형식）XML문서라고합니다．
하며, 이와같은문서를Well-Formed
'〕
를 동반하지 않고 XML 구문 구칙에만 따르는 XML
덧붙여, 이제까지 이 책에서 다루어온 fTP
문서를 이와는구별하여 Valid
（타당）XML 문서라고 부릅니다．

2 요소 형삭을 선언힌다
3행을살펴봅시다．

===== PAGE 196 =====
195 =====
<!ELEMENT books (owner, book*)

3행에는 경로 요소 ◇〕oo콰 내에 <owner> 요소 한 개와 <book> 요소가 0회 이상
（*) 등장하는 것
을나타냅니다．
자식 요소의 등장 횟수를 정의하는 기호는다음과 같습니다．
…一

기호

二1'

-，

…

.. ,

,

:：→，

一…

-

g:
（음

반드시 1회 등장

7

0회 또는 1호l 등장

*

0회 이상 둥장

+

1회 이상 등장

또, 콤마(,）는 요소의 등장 순서를 정의하는 것으로 IynJ에서는 자식 요소가두 개 이상존재할 경
우등장 순서를 지정할 수 있습니다．

요소에 포함된 데이터를 정의한다
dELE枉NT owner (#PCDATA)>

［D에서는 요소 내부
（#RDATA）
를 포함합니다. 이와 같이 以
5행의 <owner> 요소는 문자 데이터
의 사양을 선언할 수 있고, #FCDATA 외에도다음과 같은 키워드를 지정할수 있습니다．
기호
丘…

#PCDATA

…설멸∼－: 눋

…

'

,

문자 데이터만이 포함된다

ANY

모든 요소，문자 데이터가포함된다

EMPTY

아무것도 포함되지 않는다

이들 키워드는 ''2 요소 형식을 선언한디J’에서 설명한 등장 횟수, 순서를 정의하는 기호군과 조합
해서 사용하는 것으로 보다 다양한 표현을 가능하게 합니다．
예를 들면, 13행은 <memo> 요소에 문자 데이터, (keywoiii> 요소, <ref> 요소가 임의의 순서로

G

===== PAGE 197 =====
196 =====
임의의 횟수만큼 등장하는 것을 의미합니다．
긴．
ELEMENT memo (*PCDATA - keyword - ref) *>

문자 데이터와요소를 병렬로 기술하는 경우에는 반드시 #RDATA를 제일 앞에 기술한다는 것을
유념합니다．

요소는 아래 단계로 내려긴）
다
이제 요소 형식 선언의 전체 흐름을 살펴 보겠습니다．
에서부터 <memo> 요소까지 열한 개의 요소를, 5행은 <owner> 요
4행은 <book) 요소에 <name）
소에 문자 데이터만을 선언하고 있습니다．
<tELENENT book (name, author, category, grade, keyword,
logo, url? , price, public, pDate, memo) >
<!ELEMENT owner 야PCDATA) >

계속해서 5-48행에서는 <book> 요소의 각 자식 요소가 선언되고, 17-48행에서는 (mem하 요소
의각자식 요소가 선언되고 있습니다．
긴．
ELEMENT owner (#PCDATA) >
< !ELEMENT name (#PCDATA) >
< !ELEMENT author (#PCDATA) >
<!ELENENT category (*PCDATA) >
d . ELEMENT url

(#PCDATA) >

< !ELENENT price (#PCDATA) >
dELl亞1ENT publi澍1 佯PCDATA) >
<!ELEMENT pDate (#PCDATA) >
<!ELEMENT memo (*PCDATA I keyword I ref) *>
< !ELEMENT keyword (#PCDATA) >
< .~ELEMENT ref

(#PCDATA) >

< !ATrLIST books title

CDATA #IMPLIED>

< !ATTLIST book isbn CDATA #REQUIRED>
< '. A珏｀
LIST ref addr CDATA #REQUIRED>

===== PAGE 198 =====
197 =====
이와 같이 요소 형식 선언이라는 것은 일반적으로（경로）최상위 요소의 선언으로 시작해 순서대
로 하위의 자식 요소로 이동합니다．
IDTD는 경로 요소에서 내려간다】

(!ELEMENT books (owner,book*))

<book)

(name)

<author)

<!ELEMENT books (name.author,category.logo,...)>

（publish)
焄

<price) 1

<pDate)

KIELEMENT name (#PCDATA))…

속성 리스트를 선언힌빠
계속해서 각 요소에 속하는 속성 리스트를 선언해 봅시다．
< lATTLIST books title

CDATA #INPLIED>

16행은 <books> 요소에 문자 데이터를 포함하는 title 속성
（임의）
이 등장합니다. 일반적으로 속성
리스트는 다음과 같이 기술합니다．
<!ATTLIST 요소명

속성영

데이터 형식

디폴트 값＞

===== PAGE 199 =====
198 =====
1껴

.

CDATA

문자열

enumeration《열거） 후보 값 ( 1 단락）

QA1TUST book name CDATA>
(!A111JST book category (ASP I XML I JSP) XML)

타寸TnY

실체 참조

(IATTUST memo ref ENTITY #IMPUED>

ENTiTlES

ENTITY를 열거한 것

(!AT11JST memo ref ENT111ES #IMPUED)

ID

오직 하나의 식별자

<!ATrUST book isbn ID #REQUIRED)

DR티：=

I邊 참조

(!ATTUST related ref IDREF #REQUIRED>

IDREFS

IDREF를 열거한 것

(!ATTLJST related ref IDREFS #REQUIRED)

NMT0KEN

이름 토큰

(!ATrUST book name NMT0KEN #REQUIRED)

NMT0KENS

NMT아〈EN을 열거한 것

(!ATTUST book author NMT0KENS #REQUIRED)

디폴트 값으로는 구체적인 속성값을 기술할 수 있지만, 그 외 특수한 키워드를 지정할 수도 있습
니다. 데이터 형식을ID로한경우에 특수 키워드는 필수입니다．
= 수 있는 디폴트 ?'' 특수 키워드

叩－

'

r

궁

시

v

甘 m1

#REQUIRED

속성 값은 필수

(!ATTUST book isbn ID #REQUIRED)

#IMPUED

속성 값은 임의

(!AT11JST memo ref ENTITIES #IMPUED)

#RXED

속성 값은 고정 값

(!ATTLIST book cdrom CDATA #FIXED "true')

한 개의 요소에 복수의 속정이 존재하는 경우에는 다음과 겉끼 여러 속성을 동시에 기술할 수도
있습니다．

`-

< !A꼬rLIST book isbn CDATA *REQUIRED cdrom CDATA #IMPLIED>

· 내부 서브 세트는 신DOCTYP타로 정의합니다．
· 요소는 (!ELEMENT》선언으로 정의하고 친자 관계, 등장 횟수, 내부 사양 등을 표현할 수 있습니다．
· 속성 리스트는 <IAULJST) 선언으로 정의하고 속성 값의 데이터 형식, 정의 값 등을 표현할 수 있습니다．

===== PAGE 200 =====
199 =====
（문서 형식 선언）
재7임 DID

실력 테스트
w

제 2일 Lesson 4의 실력 테스트 music.xml에 내부 서브세트를추가해 봅시다. 단, music.xml은다
음조건을반드시 만족시켜야합니다．
·<musician> 요소는반드시 1회 이상등장해야 합니다．
·name, imp_work속성은필수, category, birth요소는 임의의 문자데이터로작성합니다．
·countiy속성은프랑스, 독일, 폴란드어느것이든값을취해야합니다．
해답은 책 끝에 4>

Dr.XML과 나미의 원포인트 강좌

XML의 링크 기능
나미

' 박사님. 저 요전에 ×ML 사양서를 전부 읽어 붰
《거요．
'

Dr. XML

'오, 요즘 열심히군요，그럼 오늘도 어떤 점이 궁금하나요？"

나미

' 네, 町ML에서는 하이퍼링크라고 하는 기능이 있었잖아요，해당 문자에 밑줄이 쳐진 곳을 클릭하면 다른
페이지로 이동하는 것이요，그런데 ×ML에서는 어디를 봐도 그런 것이 쓰여져 있지 않아요，편리한 기능이
XML이 되면서 없어져 버렸나요, 왜 이것이 답；
［지요？"

Dr. XML

' 정말 열심히 자AL을 공부하고 있는 것 같군요, 흠. 물론 XML에서도 링크 기능은 건재해요 게다가 HTML
보다도 한층 고도의 링크를 표현하기 위해서 xUr水라는 규격이 준비되어 있어요．
"

나미
Dr. XML

'그런데 링크는 모두 같은 것 아닌가요？ 무엇이 다른가요？'
"그렇지 않아요. 예를 들면 HTML은 한 개의 링크에서 한 장소로밖에 이동하지 못해요，그런데 실제로以ML
관련-I이라는 링크가 있다고 할 때 여러 장소를 지정하고 싶은 경우도 있겠죠. 그 경우 HTML에서는 복수의
링크를 열거하던지 링크 장소에 링크집 같은 페이지를 만드는 수밖에 없었어요，
"

나미
Dr. XML

"확실히 매우 귀찮았어요. 하지만 어느 샌가 그것이 당연하게 되었어요"
'그렇지. 하지만 xUm
（에서는 하나의 링크에서 여러 개의 링크를 걸 수 있어요，아직 xLi마灌 본격적으로
사용한 브라우저는 없기 때문에 어떠한 형태가 될ㅈ는 모르겠지만, 아마 링크를 클릭하면 팝업 메뉴가 열리
고 여러 개의 선택 부분에서 링크 장소를 선택할 수 있는 그러한 형태가 되지 않을까요？'

나미
Dr. XML

' 확실히 편리하겠네요. 다른 것은요？'
"쌍방향 링크라는 것이에요 글자 그대로 여러 개의 컨텐츠에 씽빵향 링크를 걸 수 있는 구조뢰 예를 들면
이미지나 PDF 문서와 같은 것에도 링크를 정의할 수가 있어요，
'

나미

' 이제까지는 mEML끼리의 링크 밖에 할 수 없었잖아요，컨텐츠끼리 좀더 유연하게 연결될 수 있겠네요"

Dr. XML

' 그렇지. 그 외에도 ×Ur水에서는 여러 가지 링크 형태가 정의되어 있지만 아까도 말했듯이 아직 실제로 작
동한 브라우저가 없어요，xU마
（를 어떻게 보급하고, 어떻게 구체적으로 실현시켜 갈지는 이제부터의 과제라
'
는 것이에요．

나미

' 와！너무 기대되요."

===== PAGE 201 =====
200 =====
XML 문서 밖에서 DID 작성하기
Lesson16에서는 ><ML 문서 내부에 기술한 DTD에 대해 학습했습니다, 이번
Lesson에서는 DID를 독립된 외부 파일로 작성합니다. 또 실체 참조라는 구조를
이용하여 ><ML문서를 작성하는 방법을 학습합니다，

학습 내용 미리 보기
books.xml
파잃
（f:)

（끄
편집
（트） 수 芬＃r긔 n尸 K스） 도구

도욤말
（비

4노 孕

뒤로 , 呻 . 驪固 소

books.dtd

<?srnl aeision="1,O" er,codinq="EUC-KRn ?>
dDOCTYPE books (View Source for fhf doc奴e..
<books title='Web 관련 서적 목륵' >
<owner sddress="www.younqjin.com'.rYonqjin.com Y.</owser>
<boot
一寸ISBN89-314-1742-x">
(floe
HTML 디자민 비주얼 가미드＜/rrarno>
<a'
c.L8</au比1or>
＜山r html.jpgvl四0>
＜〔 r
y>HTML</category>
<un http://www.youngjIn.com</url>
日1
11800</price>
(pr<
<publish＞명진닷컴＜/publish>
<pDate>2001-06-11r/pDate>
一 <teems>
rleyw<rd>HTML 태그＜/kevworth
를 쉽개 미해할 수 있도폭 설명한 책미다. 미 책믄 크게 세 가지 부분으로 구성되머 있다. 첫 번■는
［다．
두 번1H는 Reference와 practice 편미다．
Tutorial 편으로ㅐTML의 기초를 알기 쉽계 설명혔
며기메서는 튜토리얼 편에서 제출한 HTML의 기본적인 기능에서 나마가 믐용 심화 학습을 할 수 있
도록 하였다．
세 번째는 Step Up 편이다．
</meroe>
</book>
<book cbs寸I8BN89-314-1978-9">
<name>ASP 사전＜力iame>
<author＞니시자와 나오3k/author>
<Ioqo>asp.jpgc'Ic了丁〕

.xml-

b。
book1
。k4.xml

@XML

D
D
D

懲\ 꾜 Less。
n 17
匕〔〕 Q&a

陋

검색 」J줄겨찾기

守미口머

귈

「EE匣莩뒵퓨터
각각 입력된 XML 파일이 한 개의 도큐먼트로서 표현된다 -

（● Key Point
는 여러 문서 사이에서 공유할 수 있는 공통의 구조를 선언합니다. 각각의 특성
口rD
（문서 형식 선언）
상 ×ML 문서와 독립된 외부 파일로 작성됩니다．
물론 외부 파일로 작성한다고 해서 그 구조가 변하는 것은 아닙니다. 이번 학습을 통해 새로운 내용
을 접해 보시기 바랍니다．

===== PAGE 202 =====
201 =====
（문서 형식 선언）
제7일 DTD

전！코드 조작

새 문서를 열어 리스트 1∼ 리스트 5의 코드를 입력하고 [D7] 폴더에 각각 books. xml,
bookl.xml, book2.xml, book3.xml, book4.xml라는 이름으로 저장한다．
리스트 1 : books.xml
<?xml version="l . 0" encodingr "班Jc-F(1t " ?>
< 』DOCTYPE books SYSTEM "books . dtd"
[
< ! ENTITY book1 SYSTEM 'bookl . xml " >
< ! ENTITY bo아媤 SYSTEM "book2 . xml " >
< 르ENTITY book3 SYSTEM "book3 . xml ">
< ! ENTITY book4 SYSTEM "book4 . xml ">
<!ENTITY asp "Active Server Pages '>
I>
<books title= "Web 관련 서적 목록">
<owner address= "www.youngjin.com">Yongjin.com Y.</owner>
&bookl;
&book2;
&book3;
&book4;
</books>

리스트 2 ; bo아d.xmt
<?xml version="l. O " encoding= "EUC-KR" ?>
<book isbn="ISBN89-314-1742-x ">
<name>HTML 디자인 비주얼 가이드＜/name>
<author>C. I . S</author>
<logo>html . jpg< /logo>
<category>HTML,< /category>
<url>http: /I'wv`V.yourigj in. com</url>
<price>11800</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-06-11</pDate>
<memo><keyword>HTNI』 태그＜Ikeyword＞를 쉽게 이해할 수 있도록 설명한 책이다．

===== PAGE 203 =====
202 =====
이 책은 크게 세 가지 부분으로 구성되어 있다. 첫 번째는 Tutorial 편으로 l打ML의
기초를 알기 쉽게 설명했다. 두 번째는 Reference와 practice 편이다，
여기에서는 튜토리얼 편에서 제출한 묘IML의 기본적인 기능에서 나아가 응용 심화 학습을
할 수 있도록 하였다. 세 번째는 Step Up 편이다．
</memo>
</book>

리스토 3 : book2.xrnl
<?xxnl version="l. 0' encoding='EUC-KR" ?>
<book isbn= 'ISBN89-314-1978-3'>
<name>ASP 사전＜mnaine>
<author＞니시자와 나오키＜/author>
<logo>asp. jpg</logo>
<category>ASP< /category>
<url>http:I/ ww.w.youngj in. com</url>
<price>15000< /price>
<publish＞영진닷컴＜/publish>
<pDate>2001-ll- 30</pDate>
<inemo><keyword>ASP의 모든 명령을 내 포켓 속에＜/keyword>
Poket Reference ASP 사전은 ASP의 기본적인 지식과 사용 가능한 명령의 구문, 구문에
대한 상세한 설명, 명령 활용 예를 ASP 오브젝트, ADO, FileSystemObject의 메소드，
프로퍼티로 분류하여 언제든지 쉽게 찾아 참조할 수 있도록 한 사전식 레퍼런스입니다.</memo>
</book>

稶스區4 二 bOok3.xmi
<?xxnl version='l. 0" encoding= 'EUC-KR' ?>
<book isbn='ISBN89-314-1994-5'>
<name＞알짜 PC 용어 사전＜mnaine>
<author＞슈와시스템＜/ author>
<logo I>
<category＞컴퓨터 사전＜/category>
<price>19500< /price>
<publish＞영진닷컴＜/publish>
<pDate>2002-0l-05</pDate>
< nenK)＞이 도서의 특징은 줄임말
（약어）
에서 풀네임을 찾거나 풀네임에서 줄임말을 쉽게
찾을 수 있도록 도와준다．또한 삽화를 통해서 이해하기 어렵거나 생소한 용어에 대해서
이해도를 높이고 있다.</ineino>
</book>

202

===== PAGE 204 =====
203 =====
리스트 5 : book4.xm1
<?xml version='l. O" encoding= "EUC-KR" ?>
<book isbn= '긔ISBN89-314-2014-5">
<name>10일만0il 배우는 Visual C++ 6.0< m11aIne>
<author>Seto Haruka< /author>
<logo>vc . jpg</logo>
<url>http: //ww.youngj in. com</url>
<category>Visual C++< /category>
<price>15000</price>
<publish＞영진닷컴＜/publish>
<pDate>2002-02-05</pDate>
<memo＞이 책은 <ref addr="http://www.youngjin.corn'>
Microsoft Visual C++ 6.0</ref>(게 대해 22개의 단원을 10일 동안 순서대로
학습하도록 되어 있다. Lessonl에서는 간단한 Windows 프로그램을 직접 만들어 봄으로써
앞으로 펼쳐질 이 책의 무궁무진함을 맛보게 한다．Lesson2부터는 직접 Visual C++율
실행하고, 소스를 분석하면서 언어의 기본적인 개념을 잡아 나가고, 아지막 Lesson22에서는
이미 습득한 API 항수 사용법, 리소스 작성법 등을 이용해 Windows 응용 프로그램을
독자 스스로 코딩할 수 있게 한다．
</memo>
</book>

2

새문서를열어리스트6의코드를입력하고［D7］폴더에books.d＂라는이름으로저장한다．
리스트 6 : books.dtd
< !ELEMENT books (owrler,book*) >
<!ELEMENT book (name, author, category, logo,url? ,
price, public,pDate,meino) >
<!ELEMENT owner (#PCDATA) >
< 1ELEMENT name 야
（PCDATA) >
< IELEMENT author (*PCDATA) >
< .' ELEMENT category (#PCDATA)…
< IELEMENT url

(#PCDATA) >

dELEMENT price (#PCDATA) >
dELEMENT publi澍i (#PCDATA) >
<!ELEMENT pDate (#PCDATA) >
<!ELEMENT memo (#PCDATA - keyword ㅣ ref) * >
<!ELEMENT keyword 幟PCDATA) >
<!ELEMENT ref

(#PCDATA) >

===== PAGE 205 =====
204 =====
<!ATTLIST books title CDATA 4fIMPLIED>
< 므ATPLIST book isbn CDATA #REQUIRED>
< !ATrLIST ref addr CDATA *REQUIRED>

鞠겊·＇那띰扈뵤섭m
관례적으로 '.d璲라고합니다．

3[ D7］폴더를열고books.xm을실행한다．

的

코드해부하기
익스플로러에서 books.xml을 열어 Lesson 16과 같은 화면이 표시되면 성공입니다. DrD는 화면

의 창에 영향을주는 것이 아니므로 변경된 사항은발견할수 없습니다．

외부 DID를 작성힌）
다
외부 n［丁）
（외부 서브 세트；는주로 여러 개의 XML문서에서 공통으로 참조되며 공통의 작성 규칙
을 제공하는 것을 목적으로 합니다. 즉 앞의 Lesson에서 소개한 내부 서브 세트는 보통 외부 서브
세트에서 공통적으로 제공된 규칙 외에 그 문서 고유의 특수한
（예외H子칙을 기술하는 것이라 할수
있습니다．

내부 서브 세트

，∼

【외부 서브 세트와 내부 서브 세트】

/

『빽

「
「＼

B

,

내부 서브 세트

외부 서브 세트는 모든 XML 문서에
공통된 정의를 나타내고 내부 서브 세트는
거기에서 누락된 개개의 정의를 기술한다．

C
내부 서브 세트

D

r1
내부 서브 세트

===== PAGE 206 =====
205 =====
（문서 형식 선언）
제7일 DTD

DTI〕
를 외부에서 작성할 경우에는 XML 문서에 다음과 같이 기술함으로써 외부 파일과 연결시켜
줍니다．
< DOCTYPE books SYSTEM "books.dtd" >

외부 서브 세트의 구문은 내부 서브 세트와완전히 다른 것이 아닌, 단순히 해당 장소에 외부 서브
세트의 내용이 추가되어지는 것입니다．
이번 예제와 같이 외부 서브 세트를 기술하면서 내부 서브 세트도 작성할수 있습니다．
< 므DOCTYPE books SYSTEM "books .dtd"

]>

[

내부 실체 참조를 사용힌다
XML 문서에는많은 분량의 데이터가반복해서 사용되는 경우 이것을따로 분리하여 선언해 두고
필요에 따라 인용하는장치가준비되어 있습니다. 이것을 실쳬 참조라고 합니다. 8행을살펴보기 바
랍니다．
dEL田'lENT asP "Active Server Pages" >

이와같이 선언된문장은XML문서 내의 임의의 장소에서 &asp；라고 기술함으로써 인용할수 있
습니다. 따라서
&asp; 는 'Is상0私d 작동하는 서버 기반 처리 환경입니다．

는 다음과 같이 기술하고 있는 것과완전히 같은 의미입니다．
Active Server Pages는 'Is상에서 작동하는 서버 기반 처리 환경입니다

또, 실쳬 참조는 키보드어］
서 입력하는 것이 불가능한특수 문자를 표현하고 싶은 경우에도 유효합
니다. 그 경우 다음과 같이 기술함으로써 대응하는 문자를 표현할 수 있습니다．
「시于」
I 차ㅈ 구 드츠 드그 TI르 ㅍ A I
rL1
L ㄹ＾∥ 「ㄱ＝J.＝그＝ -, 否 iJ=/,I a
-'-'-'N i=J 1-1J

&*10진수 코드；
&#x16진수 코드；

===== PAGE 207 =====
206 =====
예를 들면다음의 코드는 탭 문자를 표시합니다．
&#x09;

다음 코드는줄바꿈 문자를 표시합니다．
&#xOa;

외부 실체 참조를 사용한다
실체 참조에 의해 인용할 수 있는 데이터는 동일 파일 내의 데이터에만 해당하는 것은 아닙니다．
다음과 같이 기술함으로써 외부 파일을 참조합니다．
< 므ELEMENT booki SYSTEM "booki . xml " >
5

< 므ELEMENT book2 SYSTEM "book2 . xml " >

6

< 뜨ELEMENT book3 SYSTEM "book3 . xml " >

口

< 므ELEMENT book4 SYSTEM "book4 . xml " >

_
【실체와 실체 참조】

&'-

(IENTITY^ )
';

실체 참조 A

실체

＆∼；

＆∼；

실체 참조 B

＆∼；

실체 참조 C
실체 참조 D

실체로 사전에 선택된 데이
터는 XML 문서의 어디에서
라도 참조할 수 있다．

===== PAGE 208 =====
207 =====
（문서 형식 선언）
재7임 DTD

예를들면 )ooks.xml에서는
&bOOk1;

와같이 기술되어 있지만 이 부분이 bookl.xml의 내용으로 교체됩니다．
때때로 XML 문서는 크기가 거대해지기도 하지만, 이와 같이 외부 실체 선언을 이용함으로써 파
일을 작은 단위로 분할 관리할 수 있습니다. XML 문서를 분산 관리하면 파일 크기가 줄어들고 각
데이터의 관리도 쉬워집니다．

r，
卜
Go to XML
∼
· 여러 문서에서 공유되는 DTD는 외부 서브 세트로 작성해서 별도의 파일로 관리합니다．
· 일반적인 여러 문서 사이의 공통 규칙을 정하는 경우에는 외부 서브 세트를, 개개 문서의 예외적인 규칙을 선언하
는 경우에는 내부 서브 세트를 각각 사용합니다．
·XML 문서0私d 공통적으로 사용되는 데이터를 미리 선언해 두고 문서내의 임의의 장소에서 참조하는 것을 실체
참조라고 합니다. 실체 참조는 키보드에서 입력할 수 없는 문자열을 표현하는 경우에도 이용합니다．
· 실체 선언은 내부에 데이터를 보유하는 내부 실체 선언과 외부 파일로써 별도 관리되는 외부 실체 선언으로 나누
어집니다．

실력 테스트
-

제 2일 Lesson5의 실력 테스트에서 작성한 address.xi교에 외부 DPD를 추가해 봅시다. 다음 사항
에 주의합니다．
· 외부 실체를 이용해서 각각의 <member> 요소를 외부 파일화 합니다．
· 요소 선언, 속성 리스트 선언은 외부 서브 세트로, 실체 선언은 내부 서브 세트로 작성합니다．
·<member> 요소의 id 속정 데이터 형식은 UD로 합니다．
해답은 책 끝에 今

===== PAGE 209 =====
208 =====
XML 스키마 사용하기
XML을 위한새로운문서 형식 정의용 언어로 xTh스키마가 있습니다．
이전의 Un）
에서는 부족했던 다양한 데이터 형식과 제약 조건의 정의, 유지 보수성을높이는 다양한 표
현등 여러 가지 사항이 XML 스키마에서 대폭적으로 개선되었습니다. 또한, DID와는 완전히 다르지만
기본적인 개념은 긷아서 뎨ED에서 기본적인 사고 방식을 확실히 익혔다면 XML 스키마는 그다지 어려
움이 없을 것입니다．
제 7일에서 이어지는 내용끼지만, 응용편에 들어가기 전에 필요한 준비 단계이므로 열심히 학습하기 바
랍니다．

===== PAGE 210 =====
209 =====
오늘 공부할 내용들
기본적인 XL 스키마 작성하기
() 향상된 X}L 스키마 작성하기

===== PAGE 211 =====
210 =====
제8일 XML 스키마 사具햐기

기본적인 XML 스키마 작성하기
이번 Lesson부터 문서 형식 정의 언어인 XML 스키마에 대해 학습합니다．

학습 내용 미리 보기
「스

books.xsd

긔books.xml

色）

XML

IH

\'지 Lesson 18

L「ㄱ Q&a

파일
（D

편집蠟)

찾기()

도욤맡
（U)

<?xml uersion="1.W encoding="EIJC-KR" ?>
(xsd:schema xmlns:xsd="http://uwu.w3.org/2001/XIILS햐lena">
<xsd:elepient name="books">
<xsd:Complexlype>
《xsd:sequence>
<Xsd:elenent nane="owler" 댜pe="owfler功pe" .iinOccurs='l " I*axoccu
《" type="bookl聊pc" mtnOccurs="O ' naxOccurs
<xsd:elenent nane= 'bo미
</Xsd:seqUence>
<xsd:attribute nane="title ' t9pe="xsd:strinq" USeㅋ"uptional" />
</xsd:co끼llexT!,pe>
<1usd: element)
<xsd:conplexlype name="ownerT봐pc" nixed="trUe">
<xsd:attribute name="address" tIpe="xsd:string" use="required" />
<Ixsd:conplexmpe>
<xsd:c0np1eu19pe name='"booklVpe">
<xsd:se때uence>
<xsd:elenent name="name 헹pe="xsd:strinq" ／》
<xsd:ele.ent name="author" type="xsd:string "/》
<xsd:elenent name="logo" type="xsd:string" ／》
<xsd:elenent nane" 'category" type='"xsd:string'" /》
<xsd:ele.ent nane쓰"url " type="xsd:string" minOccurs="'O'" ／》
<xsd:ele.ent name="price"' t1ipe="xsd:positiuelnteger" />
<xsd:elenent name=''미iblisil" t胛1e="xsd:string" ／》
<xsd:element namc="pDate" t弊re루"xsd:date" ／》
</xsd:seqUeflCe>
<usd:attribute nane="isbn" 헹pe="xsd:string" use="required" ／》
</xsd:co岬rlex麴1pe>
</usd: 5che~na》

완성한 XML 스키마의 정의

;1 Key Point )XML 스키마는 DTD를 대신할 수 있는 또 하나의 문서 형식 기술 방법입니다. DTD와는 완전히 다른
내용이지만 ×ML의 구문 규칙에 따른 XML 문서이므로 그리 어렵게 느껴지진 않을 것입니다 ．먼저
이 Lesson에서는 XML 스키마의 기본적인 구조와 DTD와의 차이점을 개념 중심으로 학습하기로 합
니다．

===== PAGE 212 =====
211 =====
茗J艾견繼箋：
；긺떻…

[D3] 폴더의 books.xinl를 열어 리스트 1에 따라 일부 요소를 삭제하거나 새로 만든 후 [D81
폴더에 저장한다．
리스트 1 : bo아〔s.xmI

<?xm1 version='l. O ' encoding= "EUC-K1 '1 ?>

<owner address= 'www.yourigj in. corn" >Youngjin.com Y.</owner>
<book isbn='ISBN89-314-1742-x '>
<name>HTME』 디자인 비주얼 가이드＜/name>
<author>C.I. S</author>
<logo>html . jpg</logo>
<category>HTME< /category>
<url>http: //www.youngj in. corn</url>
<price>11800</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-06-ll< /pDate>
</book>
<book isbn=''ISBN89-314-1978-3∥>
<name>ASP 사전＜/ name>
<author＞니시자와 나오키＜/author>
<logo>asp. jpg</logo>
<category>ASP< /category>
<url>http: / /www.youngj in. corn</url>
<price>15000</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-ll- 30</pDate>
<Ibook>
<book isbn= 'ISBN89-314-1994-5 ">
<name＞알짜 PC 용어 사전＜mnam】a>
<author＞슈와시스템＜/author>
<logo I>
<category＞컴퓨터 사전＜/category>
<price>19500</price>
<publish＞영진닷컴＜Ipublish>

===== PAGE 213 =====
212 =====
<pDate>2002-01-05</pDate>
</book>
<book isbn="ISBN89-314--2014--5">
<name>10일만에 배우는 Visual C++ 6.0</name>
<author>Seto Haruka< /author>
<logo>vc. jpg</logo>
<url>http: //ww7.youngjin.com</url>
<category>Visual C++<Icategoxy>
<price>15000< /price>
<publish>영진닷컴＜/publish>
<pDate>2002-02-05</pDate>
</book>
</ym:books>

-

,

-

이 행은 뒤의 x刻L 문서와XML 스키마문서를 연결하기 위한 열쇠가 됩니다. 자세한 내용은
서 소개되므로 지금은 "이런 기술이 있구나'라는 점만 기억해 두십시오．
제9일L3son20어］

2

새문서를열어리스트2의코드를입력하고［D8］폴더에books.xsd라는이름으로저장한다．
리스트 2 : bo아
（s,xsd
<?xml version="l. 0 " encoding= "EUC-I ." ?>
<xsd: schexna xmlns:xsd="http: //www.w3.org/2001/XMLSchema">
<xsd:element name= "books">
<xsd: complex巧pe>
<xsd: sequence>
<xsd : element name= 'owner ' type= "ownerType"
minOccurs="l " maxOccurs="l " />
<xsd: element name= "book" type= "bookType"
minOccurs= " 0 " inaxOccurs= "unbounded" />
</xsd: sequence>
<xsd:attribute nane="title " type="xsd:string" use="optional" />
</xsd:complexType>
</xsd: element>
<xsd: complexType name= "ownerType" mixed= "true">
<xsd:attribute name= "address"

===== PAGE 214 =====
213 =====
제8임 )(ML 스키마 사용하기

type= "xsd:string" use="required" I>
</xsd:complexType>
<xsd= complexType name= "book吻／pe" >
<xsd: sequence>
<xsd: element name="name" type="xsd:string" I>
<xsd: element name="author" type="xsd:string" I>
<xsd: element name="logo" type="xsd:string" I>
<xsd: element name="category" type="xsd:string" />
<xsd: element name="url " type= "xsd: string" minOccurs="O" I>
<xsd: element naxne="price" type= "xsd:positivelnteger" />
<xsd: element name="publish" type= "xsd:string" I>
<xsd: element naxne="pDate" type="xsd:date" I>
</xsd: sequence>
<xsd:attribute naiue= "isbn" type= "xsd: string" use= "required" I>
<Ixsd:coinplexType>
<Ixsd: schema>

Check
恥oifl

· 서의 버전업
실제로 XML 스키마를 동작시키려면 rvLXML 파서를 버전 4로 버전업시킬 필요가 있습니
다. 버전업의 자세한 설명은 제 9일 Lesson 20에서 다루도록 합니다．

urn와 다름없는 xll 스키마도 xTh 문서의 구조, 데이터 형식 등을 정의·규정하기 위한 언어
입니다. 따라서 이 자체로는동적인 변화는하지 않습니다. 여기에서 작성한xTh 스키마문서는 현
시점에서는 특별히 동작하지 않습니다．
제 9일 Lesson20에 DOM에서 Xll 스키마를 조작함으로써 실제로 XML 스키마에 의한 xil
문서가 어떻게 활용되는지 살펴보시기 바랍니다．
J XML 스키마 문서를 선언한다
먼저 기본이 되는xll 스키마의 기본 구조를 살펴보겠습니다．

===== PAGE 215 =====
214 =====
<?xml version= " 1.0" encoding= "EtJC-KR" ?>
<xsd:scheina cm1ns:xsd="http://www.w3.org/2001/xldLSchexna" >
</xSd = Schema>

1행은 일반적으로 XML 문서를 기술하는 고정된 선언이므로 이미 잘 알고 있을 것입니다. 기본이
되는xu꾀 버전과사용하는문자코드를 선언합니다．
2행의 <xsd:schema> 요소는XML 스키마 문서의 경로
（최상위）요소가 되는 것입니다. 모든 정의
는이 <xsd:schema> 요소에 기술합니다．
Xrn1ns:xsd속성은이름공간을정의합니다. 仕sd：∼로시작하는각요소는http://www.w3.org/
2001JXMLchema에서 정의된 문서 규칙에 따르는 것을 정의한 것으로 여기에 XML 스키마 권고
판이 정의되어 있습니다．
이 부분에 대해서는 정해조H干칙으로 이해해 두시기 바랍니다．
텍스트로 된 요소를 정의한다
xTh 스키마에 의해 표현할수 있는 대상은 여러 종류지만 기본이 되는 것은 요소의 정의입니다．
XML 스키마에서 요소를 정의하려면 <xsd:element> 요소를사용합니다．
<xsd:element naxne= ”요소명" type= " 데이터 형식" />

이것이 가장단순한요소의 정의입니다．
자식 요소를 갖지 않고 텍스트만 포함하고 있는 요소를 정의하는 경우에는 <xsd:element> 요소만
기술합니다. xML 스키마도 XML 규칙에 의해 기술된 문서이므로닫기 태그가 없는 仕sd:element>
태그의 가장마지막을 '∼／>' 로닫는 것을 잊지 마시기 바랍니다．
이번 예제에서는 최하위의 요소인 <book> 요소의 자식 요소군을 정의하기 위해 가장 단순한 요소
정의 방식을 이용합니다．
<xsd:element naxne= "name" type="xsd:string" />
<xsd:element name= "author'1 type== "xsd: string" />
<xsd:element naxne="logo" type="xsd:string" I>
<xsd:element name= "category" typer "xsd: string" I>
<xsd:element name="url " type="xsd:string" minOccurs= "O" />
<xsd:element namer "price" type="xsd:positivelnteger" />
<xsd:element naxne="publish" type="xsd:string" />
<xsd:elexnent name="pDate" type="xsd:date" I>

===== PAGE 216 =====
215 =====
name 속성은요소명을, 竝m속성은요소에 포함되는 텍스트의 데이터 형식을각각 정의합니다．
XML 스키마에서 사용할 수 있는 데이터 형식

＇mm” 月

.

<xsd:element) 요소의 pe 속정 등쇄서 지정할수 있는 데이터 형식은xll스키마에 이미 준비
되어 있는것만으로도매우풍부합니다. 그주요 형식은다음표와같습니다．

__

string

문자열

binary

바이너리 데이터

booloan

진위 (true, false)

'-

byte

바이트 형식 (-127/128)

century

세기（예 ; 20)

date

날짜 형식（예 : 2002-03-15)

decimal

10진수

double

64비트 배정도 부동 소수점

ENTiTY

실체 형식

float

32비트 단정도부동소수점

ID

ㄸ）형식

IDREF

D 침조 형식

IDREFS

D 참조 형식의 집합체

integer

정수 형식 (-2147483648"-2147483647)

"

long

긴 정수 형식 ( 223372036864775808"-'9223372036854775807)

month

월（예 : 2002-03)

NAME

이름 (XML 1.0)

NCNAME

기호 없는 이름

negativelnteger

（瑨 포함하지 않음）.
음의 정수 (

NMTOKEN

NMTOKEN 형식

『小兀
「아
（ENS

NMTOKEN 형식의 집합체

nonNegativelnteger

0이상의 정수 (0을 포함함）

nonPosftivelnteger

0이하의 정수 (0을 포함함）

NOTA110N

기법 형식

positivelnteger

양의 장수 (0을 포함하지 않음）

QNAME

이름 (XML Namespaces)

short

짧은 정수 형식 (-32768"-32767)

小

w

===== PAGE 217 =====
216 =====
데이터 형식

설…

time

시각 형식
（예 : 20:15:12.000)

timeDuration

기간
（예 : P2Y10M15DT15H3아／10.97 [2년 10개월 15일과 15시간 30분 10.97초〕
）

urisignedByte

부호 없는 바이트 형식
（0'-'255)

unsignedint

부호 없는 정수 형식
（0'wi294967295)

unsignedLong

부호 없는 긴 정수 형식
（0-"18446744073709551615)

unsignedShort

부호 없는 짧은 정수 형식
（0^765535)

uriReference

URI(Unitorm Resource Identifier = 네트워크상의 위치 정보）
(예: http://www.w3.org/2001/XMLSchema)

year

년
（예： 2002)

∼

4 요소를 포함하는 요소를 정의힌빠
보통 )Uv1L은 트리 구조라고 불리는 이름 그대로 요소 내에 자식 요소, 자식 요소 내에 손자 요소
가 연속해 있는 계층 구조로 되어 있습니다. 그러한 요소를 포함하는 요소는 어떻게 정의하는 것일
까요？
t0okaxn의 <books> 요소는한개의 <owner> 요소와복수의 <book) 요소를 포함하고 있습니다．
이렇게 계층 형식의 요소를 정의하는 경우에는 (xsd:element> 요소에 sd:comple1Irpe> 소를
기술합니다. <xsd:oomp1edpe> 요소는 자식 요소군 속성을 정의하기 위한 것으로 이 경우 <books>
요소에포함되는자식요소＜owner>, <book〉의정보혹은각각의등장규칙등을기술합니다．
<xsd: element namer "books">
<xsd:complexType>
<xsd: sequence>
<xsd: element naiue= 'owner" … />
<xsd:elemerit name="book" … />
</xsd: sequence>
<xsd: attribute naine="title "
</xsd: complexType>
</xsd: element>

또 자식 요소의 정의를 <xsd:sequence) 요소로 둘러쌈으로써 자식 요소가 "정의한 기술순서로 등
장하지 않으면 안 되븐'것을 나타냅니다. 즉 이 예제에서는 반드시 <owner>, (book> 요소의 순서로

===== PAGE 218 =====
217 =====
기술되어야합니다. 덧붙여 말하자면 <xsd:sequence> 요소 대신에 <xsd:ail> 요소를 지정한 경우요
소는 임의의 순서대로 기술할수 있습니다．

<xsd:sequence）
나 <xsd:訓〉
은 생략할 수 없습니다. <xsd:com이exType> 요소에 직접〈xsd:element) 요소를 가질
수 없습니다．

f 단순 형식 요소와 복잡 형식 요소
XML 스키마에 있어서 중요한개념을 이해해 두어야 합니다. 이제까지 텍스트만을 갖는 요소나
자식 요소
（단순 형식 요소）
와 속성을 갖는 요소
（복잡 형식 요소）
처럼 애매한 표현을 써왔지만 실제
XML 스키마에서 두 개념은 엄밀히 구분됩니다. 또한 이 두 가지 개념은 호출하는 방법뿐만 아니라
구문에 있어서도 차이가 있습니다．
꼼꼼한 ㅅ促｝
이라면 이미 알아챘을지도 모르겠지만 위에서 복잡 형식 요소를 정의하기 위해 物d:
complexTlype> 요소가 사용되었습니다. 단순형의 요소를 정의하는 경우에는 <xsd:sirnpletype) 요
소를 사용합니다. 예로 "2. 텍스트로 된 요소를 정의한디，
에서 소개한 단순 형식의 요소 정의를 참
고해 설명하겠습니다．
<xsd:element name= "name" type="xsd:string" I>

가장 단순한 형식으로 작성했지만단순형식의 요소인 것을보다 엄밀히 명시하는 것이라면 아래
와겉미 기술합니다．
<xsd: element riame= "name'>
<xsd: simpleType>
<xsd:restriction base= "xsd: string" />
</xsd = simpleType>
</xsd: element>

<xsd:restriction> 요소는데이터의 제약 조건을 기술하기 위한 것입니다．
Lesson19에서 좀더 자세히 설명 하겠지만 보통 기본 데이터 형식
（문자열 형식이나 수치 형식 등〕
을 기본으로 보다 구체적인 제약 조건
（자릿수나 최대치 등；읕 정의하고 싶은 경우에는 <xsd:restriction> 요소를 이용합니다．

參

===== PAGE 219 =====
218 =====
요소의 등장 횟수를 제한한다
리스트2의 6'-'9행을좀더 자세하게 살펴 봅시다．
여기에는 두 가지 주목해야 할 점이 있습니다. ninOccurs 속성 · maxOccurs 속성과 pe 속성
입니다．
<xsd: element name= "owner" type= "ownerType"
xninOccurs=" 1 " maxOccurs= "1 " />
<xsd:element name="book" type="bookType"
minOccurs= " 0 " xnaxOccurs= "unbounded" />

속성에 대해서는 다음 페이지의 "7. 사전에 정의된 요소 형식을참조한디？'에서 다시 설명하

Ly

므로 여기에서는 ninOccurs 속성과maxOccurs 속정에 주목합니다．
이들 속성은 정의된 요소의 출현 횟수를 제한합니다. minOccurs 속성은 최소 등장 횟수를 나타
내고ma（无curs속성은 최대 등장 횟수를 나타냅니다．
예를 들어 nnOccurs 속성을 0으로 지정한 경우, 그 요소는 생략할 수 있다는 것을 나타내고 반
대로 1 이상으로 지정한 경우에 그 요소는 필수임을 나타냅니다.
따라서, maxOccurs 속성은minOccurs속성 이상의 값을 지정합니다．
maxOccurs 속성이 miriOccurs 속성과 같을 경우, 그 요소는 반드시 지정된 횟수만큼 등장합니
다.（예를들면 minOccurs 속성, maxOccurs 속성 모두 1인 경우, 그 요소는 반드시 1회만등장해야
합니다）
. 또 최대 등장 횟수를 제한하고 싶지 않은 경우에는 maxOccurs 속성에 unbounded라는 특
수한 값을 지정함으로 그 요소는 minOccurs 속성에서 지정된 횟수 이상이면 무한히 기술할 수 있
습니다．
ninOccurs 속성과maxOccurs 속성 모두가 생략된 경우, 디폴트로 그 요소는 반드시 1회 등장합
니다．
,

m

-

,

∼d

. 냥횟 스
'

j

「
견
）一

`

I

"

「DTD에서의

y

반드시 1회 등장

없음

1

1

0회 혹은 1회 등장

?

0

1

0회 이상 등장

*

0

unbounded

1회 이상 등장

+

1

unbounded

===== PAGE 220 =====
219 =====
제8일 XML 스키마 사용하기

사전에 정의된 요소 형식을 참조힌다
리스트 2의 6-9행에서 또한 가지 주목해야할 점은蚊pe 속정입니다．
"2. 텍스트로 된 요소를 정의한다”에서 요소의 데이터 형식을 정의했을 때에는 XML 스키마가사
전에 준비하고 있는문자열 형식이나 날짜형식 등단순한 데이터 형식을type 속성으로 지정하였습
니다. 이것은type 속성의 가장단순한사용법에 지나지 않습니다．
실제로는 단순히 문자열 형식이라고 해도 문자열 길이를 10자리 이내로 제약하는 경우도 있고 어
느옵션중에서 선택하게 하는 경우도 있습니다. 이러한부수적인 제약 조건이나 "'4. 요소를포함하
는 요소를 정의한디
＇'에서 소개했듯이 자식 요소를 포함하는 복잡 형식 요소를 정의하는 경우에는
（플롯타입）
으로써 별도로 정의해 두고 이것을 참조하는 것
통합하여 한곳꼐서 정의하기 보다도 원형
이 세련된작성법이라할수 있습니다．
또한 어떤 요소에도 속하지 않는 추상적인 형식으로 정의하여 여러 곳에서 참조해서 사용할 수 있
는 이점도 있습니다.
참고로 이번 예제의 요소 정의 부분을 별도로 작성하지 않고 한 곳에서 통합해 기술한 경우는 다
음과같이 됩니다．
<?xml version="l. 0 " encoding= "EUC-KR" ?>
<xsd: schema xmlns:xsd="http: /Iwww.w3 .org/200lIXWJScherna" >
<xsd:elemerit name= "books">
<xsd: complexType>
<xsd: sequence>
<xsd:eleinent name= "owner" minOccurs= "1" maxOccurer " 1긔>
<xsd: complexType mixed= "true'>
<xsd:attribute name="address"
type="xsd:string" use="required" I>
</xsd: complexType>
</xsd: element>
<xsd:element name="book" minOccurs= " 0 " maxOccurs= "unbounded" >
<xsd: complex巧7pe>
<xsd: sequence>
<xsd: element name = ~'name" type="xsd:string" />
<xsd: element name=''author" type="xsd:string" I>
<xsd: element name= ~'logo" type="xsd:string" />
<xsd: element name=''category" type="xsd:string" I>
<xsd: element namer 'url " type= "xsd: string" minOccurs=" 0" />
<xsd: element namer ''price" type="xsd:positivelnteger" I>
<xsd:element namer ' publish" type="xsd:string" I>

===== PAGE 221 =====
220 =====
<xsd:elexnent name="pDate" type="xsd:date" I>
</xsd:sequence>
<xsd:attribute name= " isbn"
type="xsd:string" use="required" I>
</xsd:complexType>
</xsd:element>
</xsd:sequence>
<xsd:attribute name= "title" type="xsd:string"
use="optional" I>
</xsd:complexType>
</xsd:element>
</xsd:schema>

이번 예제에서는 <xsd:element) 요소의 rpe 속성으로 ownerIrpe, book'Iype을 지정하고 있습
니다
（6행, 9행 참조）
. 여기에서 참조하고 있는 ownefIrpe 형식은 15-17행에서, booklype 형식은
19'-'32행에서 <xsd:complex'lype) 요소에 의해 정의된 것입니다. xsd:element) 요소의 pe속성
과 <xsd:complexType> 요소의 name속정은대응하고 있습니다.
（이 부분만
15-'17, 19'--'32행은 각각 자식 요소와 속성을 갖는 임의의 요소를 정의하고 있습니다
보면 어디까지나추상적인 요소와구체적인요소, 속성의 관계를 owner'Iype 형식, bookIye 형식
으로 정의하고 있음을 알수 있습니다. 이 임의의 요소를 <owner>, <book> 요소로 표현하고 있는 것
．
은 6- -9행의 <xsd:element> 요소입니디〕
이것에 의해서 <books) 요소에서 부터 <book) 요소, 그 위에 자식 요소라는 계층 관계가 정의되
어집니다．
그리고 15행의 (xsd:comp1exType> 요소의 mixed속성이 true라면 지정된 요소뿐만 아니라 임의
의 텍스트 데이터도 기술할수 있다는 것을 의미합니다．
반대로 false인 경우에는 지정된 요소밖에 기술할수 없습니다．
8 속성을 정의힌다
Kxsd:attribute) 요소를 이용하여 속성을 정의 합니다．
끄행에서는 <books) 요소의 title 속성을, 16행에서는 <owner> 요소의 address 속성을, 31행에서
는 (book) 요소의 isbn속성을각각 정의하고 있습니다．

===== PAGE 222 =====
221 =====
제8일 ×ML 스키마 사용하기

<xsd:attribute name= " title " type="xsd: string" use="optional"' I>
<xsd:attribute name="address" type="xsd: string" use= "required" I>
<xsd:attribute name="isbn" type="xsd: string" use= "required" I>

竝e속정에서 데이터 형식을 정의하는 것은 (xsd:element> 요소의 경우와동일합니다．
<xsd:element) 요소와 다른 점은 use 속정이 사용되는 것으로 이것에 의해 그 속성이 필수인지
임의인지를 판단할수 있습니다. 속성값미 re批red라면 필수, optional이라면 임의인 것이 됩니다．
그 외에도 defai고t
（기본幼나fixed
（고정값）등도 지정할수 있습니다．
<xsd: attribute name= "orgAttr" use= "default" value="defValue" I>
<xsd:attribute name="orgAttr" use="fixed" value="fixValue" I>

-

·XML 스키마의 경로 요소는 (xsd：스키마〉요소가 됩니다．
·(xsd:element> 요소를 이용해 요소를 정의할 수 있습니다. 요소의 등장 횟수를 제어하기 위해서는
minOccurs, maxOccurs 속성을 이용합니다．
·<xsd:sequence>, <xsd:헤）요소는 요소의 등장 순서를 규정합니다．
·<xsd:attribute) 요소는 속성을 정의합니다. 필수, 임의의 구별 등을 정의하기 위해서는 use 속성을 이용합니다．
· 요소, 속성 모두 type 속성을 이용해서 데이터 형식을 정의할 수 있습니다．
· 요소의 개념으로는 단순 형식 요소와 복잡 형식 요소가 있습니다．
·(complexType>, 佃rT制eType> 요소를 이용함으로 추상적인 요소 형식을 정의할 수 있습니다．
· 사전에 정의된 요소 형식은 <xsd:element) 요소의 type 속성 등을 사용하여 인용할 수 있습니다．

包

===== PAGE 223 =====
222 =====
실력 테스트
-

제 2일 Lesson5의 실력 테스트에서 작성한 address.xml을 정의하는 XML 스키마 문서를 작성해
봅시다. 단, address.xml은 아래의 조건을반드시 만족해야 합니다．
·<member> 요소는 0회 이상 등장합니다．
·<old> 요소의 값은 응수가 아닌 정수가 됩니다．
·<member> 요소의 id 속정은 필수입니다．
해답은 책 끝에 4>

Dr.XML과 나미 의 원포인트 강좌

DID와 XML스키마란？
나미

"DTD와 XML 스키마, 겨우 끝났네요. 지쳤다．
"

Dr. XML "수고했어요. 그런데 수업 중에는 매우 졸린 것 같았는데？"
나미

"알고 계셨어요？ 이제 XSLT나 DOM이라면 오히려 구체적으로 작동해 주니까 뭔가 알 것 같겠는데
요, DTD라던가 XML 스키마는 단지 문법이잖아요？ 전 옛날부터 문법이라면 싫어했어요. 어째서 이렇
게 어려운 것을 하지 않으면 안 되는 것일까요？"

Dr. XML "확실히 그 기분은 알겠어요. 이제까지 DTD나 XML 스키마가 없어도 ×ML이 쓰여졌으니 쓸데없는
것 같다는 생각이 들겠지."
나미

"네, 결국 무엇 때문에 이런 것들을 해야 하는지를 모르니까 스트레스가 쌓여요."

Dr. XML "과연. 확실히 이제까지는 비교적 적당히, 그때뿐인 XML을 』서 왔기 때문에 그렇게 생각되는지도 모르
겠군요. 그러면 이것이 이미 정해졌던 룰에 따라 XML 문서를 교환하는 업무와 같은 경우에서는 어떨
까요？
주문서 ×ML에는 주문 번호와 품목 번호, 주문량, 고객 번호가 필요해서 사전에 정해두었는데, 상대편
이 잘못알고 고객 번호 대신에 고객명과 전화번호를 넣어 와 버렸다고 한다면？ 이것이 많은 XML 문
서 사이로 섞여 들어갔다고 한다면？"
나미

"그것을 체크하는 것도 큰일이겠군요. 하나 하나 전표를 넘겨서 조사하고． "

Dr. XML "그렇지. 이제까지 종이를 기초로 한 업무에서는 그러한 작업을 사람들이 밤늦게까지 했었어요.
이것이 전자를 기초로 하게 됐다고 해도, 이런 잘못된 것을 조사하는 것은 매우 귀찮은 것임에는 변함
이 없어요. 프로그램을 조금이라도 짜 본 사람이라면 알겠지만, 날짜 항목 하나 조사하는데도 날짜가
규칙적인 형식으로 쓰여져 있는지, 범위 내에 알맞게 들어가 있는지, 그 외의 날짜와의 대소 관계는

===== PAGE 224 =====
223 =====
틀리지 않았는지 등등 조사할 것이 무궁무진해요. 그것을 장황한 if문으로 써갔기 때문에 비효율적임
에 더할 나위 없지요. 게다가 항목끼리의 전후 관계, 결핍 등을 조사해 간다면 프로그램의 반 이상이
'
이런 잘못 찾기로 허비되고 말아요．
나미

' 점점 우울해져요 一 "

Dr. XML "그런데 DTD나 자vIL 스키마에서 자v1- 문서의 규칙을 사전에 기술해두었다고 해봐요. 이런 것이 결
에 건네주는 것만으로도 자기 스스로 ×ML의 타당성을
정되어 있다는 것을 미리 프로그램
（XML 파서）
조사해 에러를 검출해 줘요.
매우 긴 프로그램이 이것에 의해 단 1행으로 끝나버려요. 굉장하다는 생각 안 들어요？'
나미

' 점점 DTD와 ×ML 스키마가 의미 있는 것이라고 생각되네요. 아, 저는 왜 수업 중에 자버렸을까요？"

Dr. XML ' 이제부터라도 늦지 않았어요. 확실히 복습해서 내일 수업에 대비해요. 자, 오늘 숙제'
나미

'앳"

===== PAGE 225 =====
224 =====
제8일 x뻬．
, 스키마 사용하기

향상된 XML 스키마 작성하기
앞의 Lesson에서 작성한 XML 스키마 문서를 수정하면서 보다 자세한 사항을 정의
해 보겠습니다．

학습 내용 미리 보기
xsd

11 books.

K?xml version="l. 0" encoding="Euc-KR" ?>
(《sl1:schena xm]ns:xsd="htt꾸://uuw.w3.orgf200l/ XMLSchena">
<xsd:include scIemiaLocation="bookSSub. cSd" />

⑥XML

I 너 bookSub.xsd
[1- \ 勾 Lesson 19
니겨 Q&a

<xsd =e1e日ent name=" 1m이
（5" 》
<xsd:conp1exTIpe)
<xsd :sequence>
<xsd:e1emPnt name="owfler" 勻pe="ownerType"
minOccurs="1" naxoccurs=" 1 " />
(xsd:elenent nane="bOOk" type="book砂pe"
flinUccurs=" n" ia虹lccurs="unbounded" ／》
<REd :sequence>
<xsd:attri.bute name1'tit1e " type="xsd:string" use="required" />
</xsd:complexl!Ipe>
《／)l5d :elemerlt》
<xsd:sinplelype name="authorlVpe">
<Xsd:list iteIIT9pe="xsd:5tring" ／》
《／1'5d :sfmpleTyPe>
<xsd:attributeGroup name="bookfittr">
<xsd:attribute nauie-"isbfl" use="required"')
<xsd :simple체
＇pe>
<xsd : restrictii게 base="xsd:string">
《돠【0-91<3}-[ 0-9
<xsd:pattern ualue="ISBN[0-91{1}-[0-9l
</xsd:restriction>
</xsd :simpleTyPe>
</xsd:attriflutp>
</xsd:attributeGroup>
<xsd:comp1exT9pe nanP쓰∥bookT! pe">
<xsd:sequence>
< X 5 d = cr1ld c e >

완성된 XML 스키마의 정의

｀●Key Point ) _
XML 스키마가〔)TD에 비해 매력적인 점은, 데이터 형식을 보충할 뿐만 아니라 표준으로 되어 있는
데이터 형식을 기본으로 해서 보다 자세한 제약 사항을 표현할 수 있다는 점입니다．
DTD에는 없는 개념으로 기본적인 구조만 파악한다면 나중에 다양하게 응용할 수 있습니다．겉보기
의 복잡함에 헷갈리지 말고 ，기본 골격을 확실히 이해해 봅시다．

小

===== PAGE 226 =====
225 =====
제8임 ×ML 스키마 사용하기

Lesson18에서 작성한 xM, 스키마 문서 books.xsd를 열어 리스트 1의 코드를 추가해 저
장한다．
리스트 1: books.x히

<?xmJ. version="l. 0 " encoding="Euc-KR" ?>
<xsd: schema xrnlns:xsd="http: //www.w3.org/2001/XNLSchexna">

<xsd:elexnent naxne= "books">
<xsd: complexIype>
<xsd: sequence>
<xsd:element name=" owner' type="ownerType"
minOccurs="l " m&xOccurs="l " I>
<xsd:element name= "book" type="bookType"
minOccurs="0" xnaxOccurs= "unbounded ' I>
</xsd: sequence>
<xsd:attribute nme="tit1e " type="xsd:string" use="required" I>
</xsd: complexType>
<Ixsd: element>
l

/

17

<xsd:simple'.

18

<xsd:list

1P

1 〃t-- 기

,
21
22
23

<Xsa:attr1Duteuroup naJ11<xsd:attribute nan,e= ''i옵）
J.,
<x8d

24

<x：三一
<xsd: pattern value="IS

25

-(0- 9] {2「
26
27
28

<12'

29

</xsd

'

"

'

===== PAGE 227 =====
226 =====
<xsd:complexType name= ' bookPype">
32

<xsd= seqLience>

33

<xsd:choice>
<xsd:element name= "naine" type＝勺csd: string" />

35

<xsd:element name="title " type= "xsd: string"

36

</xsd:choice>

37

<xsd:element naxne="author">

38
39
40
41
42

<xsd: sixnp1eype>
<xsd:restriction baae="authorType 2
<xsd:rnaxLength value="3 " />
</xsd : restriction>
</xsd: simpleType>

43

< /xgd = element>

44

<xsd:eleinent name= "1ogo" type="xsd:string' I>

45

<x곱ci ; t」」．＜蠟
me1l(; ndm1,

46

1Ksd: simpleType

47

<xsd:restricti

48

<xsd:enumeration value="ASP" /

49

<xsd:enumeration va1ue= "X14L" 1.

50

<xsd:enumeration 一n4 －一 " ''r'『) ' 차-.1- y1 pt- '

51
52

/>

34

/ ,,

</xsd = restrictio二
</xsd:simplePvpe>

53

</xsd:element;

54

<xsd:element name="url " type= "xsd:string" niinOccurs= "O " I>

55

，∼1k→→ · 뇨∼나上｀L－뇨｀『戶

55
57
58
59
60
61.

L뇨u｀
ㄴ；

上／」 ㅗ｀一 ;

<xsd: simple叱／pe>
<xsd:restriction base="xsd볍positiveInteger
<xsd:inaxExclusive value="50000" I>
<xsd:minExclusive value='lOOO" F'
</xsd:restriction>
</xsd: s如
［p1eType>

62

</xsd: element>

63

<xsd:elernent name="publish">

64
65
66
67
68

<xsth simp1eT江）
e>
<xsd:restriction base="xsd:string ">
<xsd:maxLength value="20" I>
</xsd:restriction>
</xsd: sixnple叱／pe>

===== PAGE 228 =====
227 =====
제8일 ×ML 스키마 사용하기

<xsd:element name="pDate ' type="xsd:date" I>
</xsd: sequence>
</xsd:complexType>
</xsd = 8chema>

새로운문서를 열어 리스트 2의 코드를 입력하고, [D8] 폴더에 bookSub.xsd라는 이름으로
저장한다．
리스트 2 : bookSub.xsd
<?xinl version="1.0" encothng= "EUC-KR'' ?>
<xsd: schema sn1ns:xsd="http: //www.w3.org/2001/xiI,Scheim1" >
<xsd: complexType name= "ownerType" mixed= "true">
<xsd:attribute name="address" typer "xsd: string"
use="required" I>
</xsd: complexType>
.z/xsd: schema>

이번 예제에서는 )UvIL 문서의 요소를 좀더 자세하게 정의해 봅시다. 여기에서 작성한 XML 스키
마문서는 현재 상태로는 아무런 동작도 하지 않습니다．
제 9일 Lesson 20에서 실제로 XML 스키마에 의한문서의 동작을확인하기로 합니다．
'i 애매한 요소를 정의한다
불특정 다수를 대상으로 한 데이터 교환의 어려움은 각각의 데이터가 동일 형식으로 정의되어 있
지 않다는 점입니다. 예를 들어 A 회사는 도서명을 仍ame〉이라는 요소로 표현하고 있는 것에 반해
B사는 <itle＞이라는 요소로 표현하고 있을지도 모릅니다．
이것이 단순한 것으로 생각될지 모르겠지만 여러 시스템과 밀접하게 데이터를 교환하는 네트워크
시스템에서 이것을 수정하는 것은 번거로운 일입니다
（왜냐하면 규정되어 있는 요소명이 다르다면
데이터의 출력 장소가 변할 때마다 일일이 데이터 레이아웃의 편집 방법을 재검토하지 않으면안 되
기 때문입니디）
.
XML 스키마에서는 이러한 데이터 정의의 변동 사항을 미리 문서 정의로 기술할수 있습니다.

匈

===== PAGE 229 =====
228 =====
<xsd:choice>
<xsd:element name="name" type="xsd:string" I>
<xsd:element name= "title" type= "xsd:string" I>
</xsd:choice>

<xscl:choice) 요소에 기술된 두 가지의 요소－缶ame> 요소와 <title) 요소－는 XML 문서에서 어느
것이든 한 쪽을 선택하여 기술해야 합니다. 叩시 말하면 어느 쪽의 요소를 사용해도 무방하다는 것
으로 데이터간의 차이점을 해결할 수 있습니다．
r그 - 느」저01 /Vi.｀시 . ／톄＇,＾』r` ^`
C-, ㅅ 副
L/ h스rㅢ〔그 ｀入a`' i ㄴㅗ1`Jㅗㄴ．2 二＝止ㅗ

LLJ1
'r니」

<xsd: choice>
<xsd:element name= " 요소l" I>
<xsd:element name= " 요 N" I>
</xsd:choice>
문서 안의 요소 1부터 요소 N까지의 어느 쪽이든 기술하지 않으면 안 된다．

「 속성 그룹을 정의한다
여러 요소에서 공통해서 사용되는 속정 그룹이 있다고 합시다. 예를 들어 RThTh에서 border 속
성이나align속성, Id속정 등은<img＞태그나＜慟ble＞태그, 伋ame＞태그등 여러 요소에서 공통적으
로 사용되고 있습니다．
이러한 속성 그룹을 정의할 때 개개의 요소마다 반복해 기술하는 것은 개발 시간은 물론 변경된
경우의 수정 작업시 매우 복잡합니다．
이와 같은 경우 XML 스키마에서는 어떤 특정의 속성을 한 무리의 그룹으로 사전에 정의해 여러
장소에서 인용할수 있습니다．
21-29행을 봅시다．
<xsd:attributeGroup name= "bookAttr">
<xsd:attribute naxne="isbn" use="required">
<xsd: simple吼／pe>
<xsd:restriction base="xsd:string">

===== PAGE 230 =====
229 =====
제8임 )<ML 스키마 사용하기

<xsd:pattern value="ISBN[0-9] {2)-[0-91 <3) [0-91 {4} -[0-9] <1) " I>
</xsd: restriction>
</xsd: simple凸／pe>
</xsd:attribute>
</xsd:attributeGroup>

Lesson 18과 비교해보기 바랍니다. 조금복잡한 내용이 추가되어 있지만 기본적으로는isbn 속성

다．

（필수）한 개가 정의되어 있을 뿐으로 이것을 <xsd:atthbuteGroup> 요소에 의해 그룹화하고 있습니
이와같이 그룹화된 속성군은 72행에 다음과 같이 기술함으로써 사용할 수 있게 됩니다．
<xsd:attributeGroup ref="bookAttr ' I>

정의할때의 name속성과 인용｛참조）
할때의 ref속성이 이에 대응하고 있어 각각 연결키가됩니다．
<xsd:attributeGroup name=...〉에서 정의한속성을 <xsd:attributeGroup ref=...〉로참조한것
으로 Lesson 18과같이 缸）
ok> 소에 isbn속성이 추가 되었습니다．
（군）
을 한 부분에서만 인용하고 있어서 그룹화의 효과를 알기 어
이번 예제에서는 한 개의 속성
렵지만 bookAttr그룹을 여러 속성에 대해 정의하고 여러 장소에서 참조할 수도 있습니다. 여러
속성을 그룹화할 때는 <xsd:attributeGroup> 요소 안에 복수의 <xsd:attribute> 요소를 기술하
게 됩니다．
24행의 <xsd:restrictjon) 요소에 관해서는 다음의 '℃.선택할 수 있는 문자열의 값을 정의한다’에
서 설명합니다．
r -, I hI r4t1 I

L/ ㅣ

긴

』 = 써i- i- -4 t- .卜 一r｀一一｀'', `

（ㄱ 人

` 』ㅅ m

＜ㅅbu= αLLㅗ ㅗ1JuL.e`,Lou초J? 」ㅍ；』＝ 'I '- J

<xsd:attributeGroup nanie= " 속성그룹" >
<xsd:attribute naine= "속성1 ' I>
<xsd:attribute name= " 속성N

I>

</xsd:attributeGroup>
×참조할 때는 …
<xsd:attributeGroup ref= " 속성그룹" />

===== PAGE 231 =====
230 =====
3 선택할 수 있는 문자열의 값을 정의한다
예를 들어 HflvTh에 있는 align 속성이 left, center, right라는 값을 가지고 있는 것과 같이 XML
에 있어서도 어떤 요소 · 속성의 수치를몇 개의 값에 한정한다고 할수 있습니다．
예를들면 45-.-53행을봅시다．
<xsd:elexnent name= 'category '>
<xsd: simpleType>
<xsd:restriction base= "xsd:string ">
<xsd:enumeration value= "ASP" I>
<xsd:enumeration value= 'XNL" I>
<xsd:enumeration value="JSP · Serviet" I>
</xsd:restriction>
</xsd: simpleType>
</xsd:element>

여기에서는 XML 문서 안의 <c峽工ory> 요소가 ASP, XML, JSP · Serviet라는 세 개의 값 중 어
느 것인가를 채택할수 있다는 것을나타내고 있습니다．
<category> 요소는 텍스트밖에 가지지 않는 단순 형식 요소이므로 그 제약 조건은 <xsd:simple
Th2e〉에 기술합니다． "
< sd:restriction) 요소는 실제의 제약 조건을 정의하기 위한 요소로 base 속성에 기본이 되는 데
이터 형식을 지정합니다
《여기에서는문자열형）
.
그리고 <xsd:enumeration) 요소로 구체적인 값을 정의합니다. 여기에서는 세 개의 값을 기술하
고 있지만 경우에 따라서는 좀더 많은값을 정의할수도 있습니다．

'a-

(xsd:enumeration) 요소에서 기본이 되는 데이터 형식을 지정한 경우
《base속성）
, </xsd:element> 요소에서는
type 속성에 의한 데이터 형식을 지정할 수 없습니다．

===== PAGE 232 =====
231 =====
제8임 XML 스키마 사용하기

V .. .. ..
- - - ' -- ∼ - 八－∼
L<x8（그＝ re8ㄴ I끄n. .j_oI1>

r, ㅅ 01 1JAIl
」工＝亡디 ㅅ1
《심』

<xsd:restriction base= "' 데이터 형식" >
다양한 제약 조건
</xsd:restriction>
데이터 형식 베이스가 되는 데이터를 기술합니다．

r
L＜』
LbL上 = ㅂㅗ시ㅛ｀1ㅂㅗα LJOn

r) ㅅ 01 l JAIl
> ㅍ＝』스ㅋ "r 더J

<xsd:enuxneration va1ue= " 후보치i ' I>
<xsd:enumeration va].ue="후보치21' I>

*

<xsd:enumeration> 요소는 <xsd:restriction> 요소 아래oh 기술할 수 있는 다양한
제약 조건의 하나입니다．

문자열의 형식을 정의한다
문자 데이터를 다루는 경우 다양한 형식을 필요로 한다면 정의해야 할 필요성도 있습니다. 예를
들면 첫째 자리에는A--'M까지의 영문자, 2'-'5째 자리는숫자, 6째 자리는A, B의 값등을 체크하는
.
（예를들어, 코드를검색하는경우등입니디）
경우등입니다
이와 같은 복잡한 형식을 종래의 구조만을 사용하여 쳬크하는 것은〈불가능하지는 않습니다만）
곤란합니다. 이번에 소개할 정규 표현을 이용함으로써 매우 간결한 패턴으로 표현할 수 있습니다．
정규 표현이란 파일을 검색할 때 이용하는 *.xn1의 '*' 와 같은 기술을 말합니다《 '*' 은 0문자 이
. 정규 표현
상의 문자열을 나타내는 것으로 a.xml이나 xyz.xrnl과 같은 파일 이름으로 인식합니다）
은 이것을 더욱더 발전시킨 것이라고 생각하면 됩니다．
그렇다면 실제 斗子 표현 패턴을 정의해 봅시다．
<xsd:restriction base= "xsd:string">
<xsd:pattern value="ISBN[O-9] {2} -[O-9] {3)--[O-9] {4} -(O-91{1} " I>
</xsd:restriction>

===== PAGE 233 =====
232 =====
정규 표현 패턴을 기술하는 경우에는 <xsd:restriction> 요소에 出子 표현을 나타내는
<xsd:pattern> 요소를 기술합니다．
isbn 속성은 임시로 ' "ISBN"＋숫자 2자라“＝식숫자 3자리＋"-"伶자 4자리＋"-"숫자 1자리' 라
고 합시다. 이 패턴을 정규 표현으로 나타내면 25행과 같이 됩니다．
고정값은 그대로 ISBN이나 느’ 과 같이 다이렉트로 기술하고 0∼9의 수치 3자리의 경우는 ' 盼－
91{하' 라고기술합니다．
이 정의에 의해 isbn 속성이 위의 패턴에 일치하지 않는 경우에는 파서가 이것을 검출하여 에러를
발생합니다．
r 八
＇·
｀月. `．一1ㅢ－ 一｀
'.m∼

rThA (I

``＾甘｀
J ; 玉J口L ㄴ口LJ..L

I4AI I

^ ｀궈 I

<xsd: pattern value=" 정규 표현" / >
정규표현

데이터가 취할 수 있는 정규 표현 패턴

bXML 스키마에서 정의할 수 있는 주요한 제약 조건
옵션 후보나 문자열 패턴 외에도 XML 스키마에서는 다양한 제약 조건을 나타낼 수 있습니다. 아
래에 그주요한것을 열거해 보겠습니다. 모든구문은다음과같은 형태가 됩니다．
<xsd: ∼ va1ue=" 지정값" / >

m－

쨔쨍－

吐

(xsd:encoding)

인코드 형식을 제한
（hex,base64)

마지막 형식에만 유효

<xsd:length)

문자열의 길이, 리스트의 개수 등을
제한

음수가 아닌 정수

<xsd:maxExclusive)

데이터가 지정된 값 이하에 있는 것

대상이 되는 데이터 형식과 동등한 데이터 형식

<xsd:maxlnclusive)

데이터가 지정된 값 미만에 있는 것 대상이 되는 데이터 형식과 동등한 데이터 형식

(xsd:maxLength)

문자열의 길이, 리스트의 개수 등의
최대 길이

음수가 아닌 정수

<xsd:mininclusive)

데이터가 지정된 값 이상에 있는 것

대상이 되는 데이터 형식과 동등한 데이터 형식

<xsd:minExclusive)

데이터가 지정된 값 보다 큰 것

대상이 되는 데이터 형식과 동등한 데이터 형식

<xsd:minLength)

문자열의 길이, 리스트의 개수 등의
최소 길이

대상이 되는 데이터 형식과 동등한 데이터 형식

===== PAGE 234 =====
233 =====
世－
-－→｀

一－

!m

∼－

(xsd:precision)

최대 자릿수

양의정수

(xsd:scale)

유효 소수점 수

음수가아닌정수

]

ㅣ

,, 리스트 값을 포함한 요소를 정의핸가
XML문서에서는요소의 텍스트혹은속성값을빈 칸으로구분할수 있습니다. 예를들면
<author> 니시자와나오키 슈와시스템〈/author>

와같이 니시자와나오키라는 값과슈와시스템이라는 값을 리스트로 가집니다．
이와 같은 값 리스트는 XML 스키마 내에서 <xsd:list> 요소를 사용함으로써 정의할수 있습니다．
예를 들면 17'-19행을봅시다．
<xsd: simplerype name="au탓lorType" >
<xsd:list

itemType="xsd:string" I>

</xsd: simpleType>

단순 형식의 요소로 author type이라고 이름붙여진 형식을따로 정의하고 있습니다．
<xsd:list> 요소로 값 리스트를 사용할 수 있음을 정의합니다. 그리고 <xsd:11st＞요소의 itemiype
속정이 리스트 내의 데이터가문자열인 것을 나타냅니다．
17-19행에서 정의퇸 값 리스트는 3713행에서 사용됩니다．
<xsd:element name= 1' author '>
<xsd: simplerype>
<xsd:restriction base="authorType">
<xsd:maxLength value= "3" I>
</xsd:restriction>
</xsd: simpleType>
</xsd:element>

먼저, 기본이 되는 형식을 <xsd:restriction) 요소의 base 속성에서 정의가 끝난 author 乃pe 형
식으로 지정합니다. <xsd:maxLength> 속정은 리스트에 포함할 수 있는 값의 최대 개수를 조건으
로 하고 있습니다. 결국 이 경우 속성값을 3- 로 하고 있어 가질 수 있는 값은 최대 3개입니다. 따라
서 )aTh 문서에 있어 다음과 같이 4개의 값을 기술한 경우 파서는 이것을 에러라고 합니다．
<author〉니시자와나오키

슈와시스템

한정환

Haruka< /author>

===== PAGE 235 =====
234 =====
K ' Go to XML
· A, B 어느 것이 등장할지 예측할 수 없을 것 같은 요소는 <xsd:choice) 요소로 선언합니다．
XMI- 스키마에서는 최대치／최소치, 최대 자리／최소 자리, 리스트 값, 후보값, 정규 표현 등 다양한 제약 조건을 표
현할 수 있습니다．

실력 테AE
∼

제 2일 Lesson5 실력 테스트의 address.xml을 정의하는 XML 스키마 문서를 작성해 봅시다．
단 address.xml은 아래 조건을 반드시 만족시키도록 합니다．
· 令nember> 요소는 0회 이상 등장합니다．
·(address> 요소의 값은 10-'.-lOO자리 사이의 문자열로 합니다．
·(old) 요소의 값은 10-420 사이의 정수로 합니다．
·<ema파 요소의 값은 적절한 E-Mail 어드레스로 합니다．
단, E-Mail 어드레스의 정규 표현은 'T\w\. _]+(\+[\w_]*)?@([\w_]+\.)+Rw_]+" 로 합니다．
·<member> 요소의 Id 속성은 필수입니다．
해답은 책 끝에 今

C

===== PAGE 236 =====
235 =====
Go to XML

===== PAGE 237 =====
236 =====
Lesson 20 ，닐Lesson 2:

클라이언트 중심의
XML ㅍ 쿠그래밍
오늘은 앞에서 학습한 내용을 실제 프로그램에 적용하는응용편입니다．
이제까지는XML을단지, 구문척인 면에만관점을두고 설명해 왔지만지금부터는실제적인 XL사용
법과프로그램에 적용하는방법에 대해학습합니다．
먼저, 브라우저에서 실행되는프로그램을작성합니다．
이번 Lesson의 요점은 로직 자체의 이해도 중요하지만 XML에 의해 이제까지 작성한 프로그램이 어떻
게 변화하고 편리한 점이 무엇인지를 파악하는 점이 중요합니다. 이 점에 주의해서 학습하도록합니다．

===== PAGE 238 =====
237 =====
오늘 공부할 내용들
XML 스키마에서 沁4L 문서의 구문 체크하기
XSLT에서 동적인 정렬 실행하기
도서 검색 프로그램 만들기

===== PAGE 239 =====
238 =====
제9일 큘라이언트 중심의 XML 프로그래밍

XML 스키마에서 XML 문서의 구문 체크
XML 스키마는 어디까지나 문서 정의를 기술하는 구문에 지나지 않습니다. 실제로 이것을
사용해 ×ML 문서를 검증하고 검출한 에러를 표시하는 것은 D아／의 역할이 됩니다．
이번 Lesson에서는 실제로 XML 스키마와 ×ML 문서를 관련지어 양자를 조합 · 검증하는
프로그램에 대해 학습합니다．

。

m
ㅎ
h
e
ㅎ
d

口

학습 내용 미리 보기

一

硼小4L문서획 』금 . Microsoft Internet Eoplore
＠

4

XML

파일
（E)

편집
（트） 보기
（y)

퓰겨찾기《스》 도구
（工） 도뭄달(H)

J 크쇼

銓검색 ＝」즐겨찾기 少미디머 J

스！孕

亡〕Lesson 20
匕
［〕Q&a

XML 스키마（게 서 ×ML 문서의 구문 체크

·

Microsoft Internet Explore,
니｛)72897ㅌ5[)

J노XML문서는스키마呻따르고있습니다

…

罷데미터 헝식硼 EI I
(cetegory>HTM
categ。ry擁at090rO>
Eli Elt 값미 있습니다

〔1二薰엇1二二

XML 문서가 Valid
（타당）
인 경우，
에러가 없음을 나타낸다

- 예를 들면 <category) 요소가 올바르지 못한 경
- 우，
에러가 발생한 행과 내용이 표시된다

(. Key Point
제 7일, 제 8일에 이어 추상적인 내용이 계속되어 조금 지루할자도 모르지만, 남은 2일 동안은 이제
까지의 학습을 정리한 종합적이고 실용적인 프로그램에 도전하는 시간입니다．
내용이 복잡할 수도 있지만 세세한 내용을 이해하는 것보다는 처음에는 에러 없이 정상적으로 동작
되는지에 전념하시기 바랍니다. 이번 학습의 목적은 이제까지 8일긴뻬 걸쳐 배워 온 Lㅐ離i《기 실제
로 어떻게 응용되는가를 학습하는 것입니다．
우선, XML 문서 books.xml의 내용을 ×ML 스키마의 정의에 적합한 형식으로 변경하여 다양한 에
러를 발생시켜 보기로 하겠습니다．

===== PAGE 240 =====
239 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

실전！코드 조작
※[D8] 폴더의1xokamil, books.xaU)ooksSub.xsd를 [D9] 폴더에 복사합니다．

1 새문서를열고리스트의코드를입력하여［m］폴더에validate.ht祉이라는이름으로저
장한다．
리스트 : vatidate.html
<htrra.>
<head>
<title>XMI』 문서의 검今c/title>
<script lariguage= "JavaScript">
<!

-

-

var objScm=new ActiveXObj ect ( "MSxldL2 .xnilSchemaCache . 4 . 0 " 》;
objScm.add( "urn:books" ' 'books .xsd" ) '
var objDoc=new ActiveXObjec디 "MSx班L2 . DO工Document . 4 . 0 " ) '
objDoc . async=false;
objDoc . schemas=obj Scm;
objDoc.load( "books. cnl") ;
var objErr=objDoc .parseError;
if (objErr.errorCode!=0) {
str=objErr.errorCode + " \r" '
str+=objErr.line + " 행" + objErr.srcText + '\r" '
str+=objErr.reason;
window.alert (str) ;
)else{
window, alert ( "XML』 문서는 스키마에 따르고 있습니다“ ) ;
}
'I-

-

>

<Iscript>
</head>
<body>
<hl>XML 스키매게서 xl4I』 문서의 구문 체크＜/hl>
</body>
</htxnl>

===== PAGE 241 =====
240 =====
에서 .'Installer Korean"을 다운로드하고 msxm
2 .H의 ㅅㅒ트
（2002년 3월 20일 현재）
KOR.msi를 인스톨한다．
http: //msdn.microsoft.cQu/downloads/default.asp?url=/downloads/saniple.as
p?url=/MSDN-FILES/027/001/766/msdncompogitedoc .xml
만약 설치 마법사가 실행이 안된다면

check
114)int

위의 사이트에서 자신의 운영체제에 맞추어 아래 그림의 박스 부분을클릭하여 nstrnsLexe
파일을다운로드하여 실행시킨 후 msxmlKORmsi를 다시 실행시킵니다．

}MS['N Downloads - Microsoft Istetnyt Erplurer
파일
（E)

편집
（D

보갸
（y)

쥴겨찾기：츠） 도구
（工） 도음알언）

a)

蟲

*iAI j첨

솥1

發

Iftt7I
..ij
쥴

Jth7I

DI '

9i11

주소
（오）눋」h卄口〃m5dα mc
『.s0kc0m/d口바n山ads/de伯u"a5p0UdVd.Wn山ad5/5am미ea5p?U＂ㅋm5dnmes／□2〃0Uu76태m =j β미듬

川5DNㅐon比 - senDs 1ibra'y I .

Walnodx I [ndpi. ot. .

Sit. O.p

SISDS Vivdd`nidO
새c）
샤 C4 〕낙nends

r∼

二의
α

回 Up One L000
口 MSXML 수0 RTM

札r all opbOfls d』
d
【the file name and saled
"Run" in the p이）up 小alog M5xm14.msi 베∥
install MSx卜机- 4끄 RIM on your computer,
msxml4msms,ene and msxml4nab.exe will
ask coo to accept the 티JLA, and tn spec心 a
Incahm to save the file.
卄us release uses windows. Installer 2.0. If
you do not have 난vs versionJ download and
insto(it here for Wiodown NT/?000 or bocoig0 <
《뇨山d汕보｀긔nz묘즈）

ㅢ 여기를클릭

Notices
Impartant notice: too mast read 盼sin if yeU P
『e씨.1』
引y installed 盼10 April 20["
Technical Prewiew of MSXML 4.0. 5ecause version-independent ProgiDo existed in the
April releooe, but have be帥 removed from Hs)<H14刀Jinstolling this release will make
小em non-fun茵.n비‘To cc이d 난11치 runthe mllnwing two vommand0 from 卄1e mmmand「ne
before 1nstallivg thin r비ea`e
r05evr32/0r50x씨4dli
r 9

,

一戶

.

』

鮮1 MS【＞N Downloads

《：그heck

川1`

본 예제를 작동人

이 책에서 지금까지 사용해 온 M8XMIB가 아닌, M8XMI4를 인스톨해 둘 필요가 있습니
다. 업무환경에서 인스톨할 경우아는주의해서 실행하십시오．

240

===== PAGE 242 =====
241 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

3

버튼을클
［醴］
다운로드한msxmJKOR.msi를더블클릭하여 설치 마법사가실행되면
릭한다．
Microsoft XML Parser 및 SDK 설치 마
법사

t1t

flI LH
UE瀞i1 UF
LID.
Microsoft
A XML AI2.
Parser및
【 SUKI(

4

ㅅ陪허락화면에서［동의햅을선택해［rL0버튼을클릭한다．
최죵 사용자 사용권 계약
다음 사용권 계약을 자세히 읽머주십시오

MICROSOFT 소프트웨어 최 종 사용자 사용권
계약
MICROSOFT XML CORE SERVICES (MSXML) 4.
줌요한 내용미므로 자세히 읽으시기 바랍니다：몬 Micro드口卄 최증 사용자
믄 위에 명시된 Mcrosoft 소프트웨머 제품［네
사용권 계먁
（“사용권 계약‘）

!l

C1 여기를클릭

쟎 塔의헵咫i
戶 듬의 안 함(Q)

（뒤로( ) - 다음
（N：
口

1

.

여기를클릭

===== PAGE 243 =====
242 =====
5

ㅅ陪자이름, 조직을입력하고［亡榴버튼을클릭한다．
고격 점보
고객 정보릎 밉력하십시오．

e9

사용자 미롬（ㅗ」）:

(1l ㅅ용자 이름 입력 I

veon kyu chun
조직
（으）
:
lEQ communication

ol 조직을 입력

〈뒤로
（邸

6

-

Q1음qp>

:

칫스

.

I

」

여기를클릭

匡준설치〕버튼을클릭한다．
설치 뮤협 션택
요ㅋ기게 가장 잘 맞는 설치 유형읕 선택하십시오

e9

표준 설치
（D
I附巳ogreni FilesWMStML 4.0011 MStQ咀 40퓰 설치
dJLILL

여기를 클릭

사용자 지정 설치(ID...
섣치할 프로그램 기늠과 위치를 선택할 수 있습니다 고
납 사뇽사베거f 권 상팝니나」

-

취소

1

===== PAGE 244 =====
243 =====
인스톨 작업이 정상적으로 끝나 종료 화면이 표시되면［마침］버튼을 클릭해서 인스톨을 종
료한다．

죤今

Microsoft XML Parser 및 SDK 설치 마
법사 뫈료

섭치 마법사를 끝내려면 까침‘을 클릭하십시오．

여기를 클릭

aiidate.html을실행한다．
8 ［凶］폴더를열고，

books.xml의 내용을 XML 구문 규칙에 위반되지 않는 범위에서 books.xsd의 정의에서 벗어나도
（예를 들면 <name) 요소를 제거하거나 <price> 요소에 문자열을 기술하는등）
.
록 변경해 봅시다
validate.html을 기동할 때에 에러 대화상자가 표시된다면 성공입니다．

XML 스키마 문서를 불러낸다
먼저, 미리 준비한xML스키마문서를불러내 봅니다. 6, 7행을보시기 바랍니다．
var objScm=new ActiveXObject ( "MSX皿』
2 .xn1SchemaCache .4.0") ;
objScm. add( "urn:books " ' "books .xsd" ) '

MSXML의 DOM에는 XML 스키마 문서를 입력하기 위한 오브젝트로써 XMLDOM
SchemaCache가 준비되어 있습니다. 6행에서는 XMUSchemaCache 오브젝트를 생성해 이것을 변
수 OhjScm로 입력하고 있습니다. 단 생성된 지 얼마 안된 XlVLSchemaCache 오브젝트는 아무런
（XMLDOMDocument2 오브젝트를 생성했을
내용을 가지고 있지 않은 빈 영역에 지나지 않습니다
때와같습니다）
.
7행의 add 메소드를 실행하면 비로소 XtvfLSchemaCache 오브젝트에 구체적인 x戮d[L 스키마 문

簪

===== PAGE 245 =====
244 =====
서
（이 경우, books.xsd）
가 입력됩니다．
제 1인수가 되는 "urn:books"는 XML 스키마 문서가 XML 문서의 어느 부분을 정의한 것인지
를 나타내는 키가 되므로 XML문서 내에 기술된 xmlns:∼속성에 대입합니다
（p.172의
.
books. xml 참조）
<ym:books mi1ns : ym= "urn:books">

이 문장에 의해 'brn:book '이라는 키로 정의된 요소는 bookaxsd에서 정의된 문서 규칙에 위배
되지 않아야 합니다．
r_.AA

｀口｀
ㅛ上

r,JIAr- fl I
비1二ㅗ＝===

ㅗJAIl
^1 ' =U

변수．
add( "URN" ' "문서")
변수

XML SchexnaCache 오브젝트를 입력한 변수 이름을 기술합니다．

URN

XML Schema 문서를 한번에 표현하는 URN을 기술합니다．

문서

적용할 XML Schema문서 이름을 기술합니다．

2XML 문서와 XML 스키마 문서를 연결한다
XML 스키마 문서를 저장하는 영역을 XMhSchemaCache 오브젝트라고 한다면 일반적인 Xll
문서를 저장하는 곳은XML]DOMDocument2 오브젝트입니다．
var objDoc=new ActiveXobject ( "MSXML2 . DONDocument . 4 . 0 " ) '
objDoc .async=false;
objDoc. schemas=objScin;

:n

小多

8행에서는 먼저 변수 objDoc에 저장 영역을 입력합니다．
그리고 10행에서는 Schemas 프로퍼티에 6-'-7행에서 생성한 XMLSchemaCache 오브젝트를 입
력함으로써 불려나온 Xll 문서를 검증하기 위한 기초가 되는 XML 스키마 문서 books.xsd가
X!vll.4DOMDocument2 오브젝트에 연결됩니다．
Lscneiaas 三스도ㅗ셔디틔 A1＜늬J

변수1.schemas ＝변수2;
변수1 XME』 문서
（x1dLDODoucinent2 오브젝트）
를 입력한 변수명을 기술합니다.
변수2 XM1』 스키마 문서 (0江LSchemaCache 오브젝트）
를 입력한 변수명을 기술합니다．

===== PAGE 246 =====
245 =====
제9임 클라이언트 중심의 ×ML 프로그래밍

XML 문서의 검증 결과를 대화상자로 표시힌타
자, 드디어 XML 스키마문서를 사용하여 XML 문서를 검증하겠습니다．
이것은 그다지 어려운 것은 아닙니다. 10행에서 XML 스키마 문서인 books.xsd에 연결된
XMLDOMDocument2 오브젝트어］검증의 대상이 되는 XML 문서 books.xml을 호출하기만 하면
됩니다．
obj1Doc.1oad( "books.xml") ;

load 메소드에서 호출된 books.xml은 XML 스키마 문서 books.xsd에 의해 검증되고 에러가 있
는 경우에는 에러 정보가 보관됩니다．
var objErr=objDoc .parseError;
if (objErr.errorCode!=O) {
str=objErr.errorCode + " \r' ;
str+=objErr.line + " 행" + objErr.srcText + "\r "F
str+robjErr.reason;
window, alert (str) ;
}else{
window.alert ( 'x1江L 문서는 스키마에 따르고 있습니다" );

}
보관된 에러 정보는 parseError 메소드에 의해 구할수 있습니다．
parseError 메소드는 에러 정보를 보유하는XMLDOMFarseError오브젝트를 반환합니다．
errorCode 프로퍼티는 XMUJOMParseError 오브젝트에 속하는 프로퍼티에서 XML 스키마의
검증에 의한에러 코드가 입력됩니다. 결국 여기에서는 에러 코드가 0인 경우는 에러가 없는 것으로
간주하고 그 이외의 경우에 에러 코드와그것에 따른 상세한 정보를 대화상자에 표시합니다．

XMLDOMParseError 오브젝트의 중요 프로퍼티
프로퍼티

. 설
【
뇨■丘：

errorCode

에러 코드

filepos

에러 발생 위치
（절대 위치）

line

행

reason

에러 발생 이유

srclext

에러 원인이 된 소스 코드

un

에러가 발생한 도큐먼트 이름

===== PAGE 247 =====
246 =====
l

∼
·XMLSchemasCache 오브젝트는 XML 스키마 문서를 입력하기 위한 오브젝트입니다．
·XMLDOMDocument2 오브젝트의 Schemas 프로퍼티에 ×MLSchemas 오브젝트를 입력함으로 XML 문서와
XML 스키마 문서가 연결됩니다．
·XML 스키마에 관련지어진 XML 문서는 호출시 자동적으로 검증됩니다．
· 검증시의 에러 정보는 XMLParsedError 오브젝트에 자동적으로 입력됩니다．

실력 테스트
-

텍스트 영역에 입력한 XML 문서의 타당성을 체크하고 에러시 에러 정보
（에러 코드, 에러 행, 대상
소스 코드, 발생 이유隱 표시해 봅시다．
※ 힌트 ;
지정된 문자열을 X入／R」문서로 XMLDOMDcxument2 오브젝트에 입력하려면 1oadXL 메소드를 사용합니다. 1oadXML
메소드 구문은 아래와같습니다．
r`

냐oaw.r

볘소느：
쉬 시식』

야功Doc. 1oad.)(KL (strXML)

L_

objDoe

X4I』
DOTflDocument2 오브젝트

strXML

XMl』 문서를 나타내는 문자열

해답은 책 끝에 을＞

===== PAGE 248 =====
247 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

「

斗
Go to XML

===== PAGE 249 =====
248 =====
小 21

；ㅔ.일클라이언트중심의糊L프로그래*:

XSLT에서 동적인 정렬 실행하기
XSLT의 <xsl:sort> 요소를 조작하여 사용자가 정렬 방법을 지정할 수 있도록 합니다．

books.xsl

斗Veb 관련 M적 륵- Micrc,$ft nterfe(E (m口re
파일
（E) 편집（트） 보기
（y) 츨겨찾기
（聊 도구（工） 도움알＜H)

，∼， 써∼？纛恥斗斗孕
「

瀟ㄴ회盤
■

，눋뒤로 , 》／

心，
J

면결 "

@XML

口

I _학습 내용 미리 보기
3 口 ｝魏검색 ＝」즐겨찾기 沙미디머 3

－」韜 蠟

＝卜曲Less。
n 21
Web관련서적목록

匕區극
Q&a

발간일
축판人r 가격
저ㅈ…
峰BN코드
서적
ㅏ
냉신낫쉬1800뭔 2001-06-11
낟56N89-314-1742-x HTML 므자닌 나널 가이…c. I.s
SBN89-314-1978-3 ASP사선－
니시자와나오카영진닷컴 15000원 281-11-30
영진닷캄19500원 i02-(기ㅢ万
슈와시스템
S트N89-314-1的4히밭찐￡익용어 '놔선
- ISBN89-314-2014-5 11j낄Ei01l UH우는 Visual CI-+ 60Seto Haruk…영신닷컴 15000뭔 2002-02-05

H87I

1lSBN2E
youngjln.com 1.

j

:

…

圈

驢춈 LN 8AEI

… m=;

》

l

정렬키를 변경하면 표에 L忙十나는 내용이 바뀐다

Key Point )
정렬키는 항상 XSLT에 의해 미리 주어집니다. 그러나 이번 Lesson에서 처럼 여러 가지 방법으로
데이터를 참조하고 싶은 경우, 키마다 다른 ×SLT 스타일 시트를 준비해야 하므로 그다지 실용적이
라고 말할 수는 없습니다．
그래서 이번 학습게사는 DOM에 의한 동적으로 ×SLT를 변경하고，동적인 정렬 처리를 하도록 합니다．
이제까자는 ×SLT라면 ×SLT, D0M이라면 DOM을 각각 구분해 사용해 왔지만 여기에서는 XML을
작성하는 두 가지 방법을 병용하여 실용적인 작성 방법을 학습하도록 합니다．

小

===== PAGE 250 =====
249 =====
·

※{D9] 폴더에 [D2] 폴더의 bookaxml. books.css를 복사합니다．

'

새문서를열어리스트의코드를입력한후, [m］폴더에books.xsl라는이름으로저장한다．
리스트 : books.x引
1: <?xml version="l. 0" encoding= "EUC-KR" ?>
2

<xsl:stylesheet xmlns:xsl="http: //www.w3.org/1999/
; XSL/Transform" version="l. 0 ">

3 ;

<xsl:output method= "html" encoding= "EUC-KR" I>

4

<xsl:template rnatch="I ">

5

<html>

6

<head>

7

<title> <xsl:value-of select="books/@title" I> </title>

8

<link re1= "sty1esheet " type="text/css" href="books.css" I>

9

<script language="JavaScript">

10

< 1[CDATA[

11

var objDoc=document . XMLDocument;

12

var Ok功St1=document . XSLDocument;

13

var nodRow=objStl. selectSingleNode( " //xsl : sort") ;

14

function disp( ){

15;

key=document.forms[0] .srt. value;

1

16;
17

ㅣ

18

switch(key) {
case "1":
trnpl= "@isbn";

19

tmp2="text ";

20

break;

21
1

case "2":

22 l

tmpl= "name";

23

tmp2="text ";

24

break;

25

case "3":

26

tmpl="author";

27

tmp2="text ";

28

break;

29

case "4 ":

===== PAGE 251 =====
250 =====
tmpl="pithli粃1" '
tmp2="text ";
break;

3:
3싸

case "5" =
tmpl="price";
tmp2= "nuxnber";
bre出댜
case "6":
tmpl="pDate";
tmp2="text ";

3

break;
4

…

4:

nodRow. setAttribute (∥select" , tmpl) ;

4:

nodRow.setAttribute ( "data-type", txnp2) ;
dSrt.innerHTML=obj Doc . documentElement.transformNode(objStl) ;

44
4'

)

4t

]] >

4'

</script>

4E

</head>

4!

<body onload= "dispO ">

5(.

<hl><xsl:value-of select="books/@title" /></hl>

51

<div id="dSrt" >

52

<xsl: apply-templates select="books" I>

5:

</div>

5'

<p>

$T

<form>
정렬키
<select name=" srt " onchariger "disp Q ">

5:

<option value=" l ">ISBN 코드 </option>
<option value="2 "＞서적명 </option>
<option value="3">저자 </option>
<option value="4 "＞출판사 </option>
<option value= "5" >가격 </option>
<option value="6"＞발간일 </option>
</select>
<If orm>
<Ip>
<div><xsl:value-of select="bookslowner" I><Idiv>

250

===== PAGE 252 =====
251 =====
</body>
</ht.n1〕．.>
</xsl : template>
<xsl :template match= "books">
<table border="l ">
<tr>
<th>ISBN코드 </th>
<th＞서적 </th>
<th＞저자 </th>
<th＞출판사 </th>
<th＞가격 </th>
<th＞발간일 </th>
</tr>
<xsl: for-each select= "book">
<xsl:sort select= "@isbn"data-type= "text " order= ' ascending" I>
<tr>
<td nowrap="nowrap"><xsl :value-of select= "@isbn" /></td>
<td nowrap="nowrap">
<xsl:element name= "a">
<xsl:attribute name="href">
<xsl:value-of select="url " I>
<Ixsl : attribute>
<xsl:value-of select="name" I>
</xsl :element>
<Itd>
<td nowrap="nowrap '><xsl :value-of select="author" /></td>
<td nowrap="nowrap"><xsl :value-of select= "'publish" /></td>
<td nowrap="nowrap">
<xsl : choose>
<xsl:when test="price[number(. )&lt; =18000] ">
<span style="font-weight:bold; ">
<xsl :value-of select="price" />원
<Ispan>
</xsl :when>
<xsl = otherwise>
<xsl:value-of select="price" />원
<Ixs1: otherwise>
</xsl : choose>

===== PAGE 253 =====
252 =====
<／七d>
<td nowrap="nowrap"><xsl:value-of select= 'pDate'

/><Itd>

</t：ㅍr>
l,

</xsl : for-each>

1!

</table>

11. ;

</xsl:template>

若

i1

</xsl : stylesheet>

저장 파일의 확장자
이 경우에는 DOM을 기술해도 베이스는 어디까지나 XSLT입니다. 확장자는 '. csI' 로 저장
합니다．

2 [m］폴더를열고books.xnil을실행한다．
오류 발생시
p似fit

실행시 다음 화면과 같은 오류 발생시［아니오
［隱 클릭한 후 새로고침
（I制 키）
을 실행하면
정상적으로 동작합니다．

「煌탈렇 騙計A*H
FAI LIJJF?
Lj[
줄：7
오류 'objStl믄
（는：1 개체가 마닙니다

익스플로러에서 books. m〕
1을 실행하면 목록표의 하부에 콤보 박스가 표시됩니다. 이 콤보 박스의
값을 변경해 봅시다. 박스에 나타난 키를 기준으로 데이터가 오름차순으로 정렬되면 성공입니다．

1 스타일 시트의 내부에 스크립트를 기술한다
XSLT 스타일 시트 안에 DOM 프로그램을 작성할 경우 <script〉
태그를 사용하는 점은 ff 爪ll콰
같지만주의할점이 있습니다. 10, 46행을봅시다．

夔

===== PAGE 254 =====
253 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

<script langiiage='JavaScript'1>
< ! [CDATA

] 〕>
<Iscript>

코드 전체가 <![CDATAIHI＞로 둘러싸여 있습니다. 이것은 'CDATA 섹션’ 으로 그 내부에 기술된
데이터는 파서에 의해 해석되지 않는다는 것을 의미합니다．
DOM의 코드 안에는XML에서 해석의 대상이 되는문자
（'<' , ' >' 등）
가많이 포함되어 있습니다．
당연히 이것들은 파서가 정의하고 있는 태그의 시작 문자가 아니므로 에러가 발생합니다. 따라서
CDATA 섹션으로 코드 전쳬를 감싸 두면 내부에 기술된 모든 문자가 파서에서는 무시되므로 에러
를방지할수 있다는 것입니다.
물론 이러한 문자를 '&it;, &gt;' 와 같이 기술하면 에러를 방지할 수는 있지만 코드 자체가 읽기

2xM니 xsLT를 구한다
이 예제에서는 미리 연결된 XM과 XSLT를 다시 구해 표시 방법을 변경합니다．
XML나 XSLT을 호출할 때 지금까지는 load 메소드를 사용해왔지만, 이처럼 이미 동작하고 있
는 현재의 도큐먼트를 불러내는 경우에는 보다 편한 방법이 있습니다. 11, 12행을 살펴보시기 바랍
니다．
var objDcc=document . XMLDocument;
var objSt1=document . XSLDocument;

XMLDocument, XSLDocument 프로퍼티는 XMT 문서와 XSLT 스타일 시트를 직접 구해
XMLDOMDocument2 오브젝트로 반환합니다．
books.xml을 실행하여 연결된 books.x쿄 읽기가 종료한 시점에서 14-45행에서 정의하고 있는
사용자 정의 함수 disp가 실행됩니다．
thsp 함수 내부를 대략살펴보면 크게 전반부와후반부로 나뉩니다．
전반부는 15-'41행에 해당하고 선택 박스에서 선택된 옵션을 키로 하여 정렬키가 되는 요소
（tmp2）
을 취득합니다.
(tmpD와 정렬 형식의 데이터 형식

小

===== PAGE 255 =====
254 =====
후반부인 42-'44행에서는 구한 데이터를 사전에 얻었던 柚l:sort) 요소의 select와 data-炒pe
속정으로 설정하고 XSL'T뻬 의한 변환을 실행하고 있습니다．
XML을 동적으로 변횐힌다
11,12행에서 얻은 XSLT 스타일 시트는 콤보 박스에 입력된 내용에 따라 변경됩니다. 구체적으로
변경된항목은 <xsl:sort> 요소의 select 속성과data-type 속성입니다．
변경된 XSLT 스타일 시트는 최종적으로 다시 한번 xll 문서에 적용되게 됩니다. 이것이 44행
에 기술되어 있습니다．
Srt. innerHTML=objDoc . docunientEleinent . transforinNode (obj Sti) ;

transforrnNode 메소드는 인수에서 지정된 XSLT를 XML 문서에 적용하고 문자열
（즉, 변환된 결
과로서의 HThll을 돌려줍니다. 변환 결과는 innerHTlvlL 프로퍼티에 의해 51-'53행.d="dS台r에
서 나타나는 부분）
에 삽입됩니다．

innerHTML 프로퍼티는
문서 전채

dSrt에서 나타난 범위에
변환된 HTML을

dSrt

삽입한다．

===== PAGE 256 =====
255 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

궂'

Go to XML

∼
·XSLT 내부에 스크립트를 작성할 경우 ，원칙상 (![CDATA[씨］
＞로 소스 전체를 둘러쌉니다，01 부분은 CDATA 섹
션이라고 불리며 내부에 쓰여진 데이터는 파서에서 무시됩니다．
·XML 문서와 XSLT 스타일 시트를 얻으려면 XMLDocumerit, XSLDocument 프로퍼티를 사용합니다．
·transformNode 메소드는 지정된 XSLT스타일 시트에 의해 XML문서를 변환합니다．

-

샘플 books.xsl을 수정하여 오름차순, 내림차순의 선택을 추가해 봅시다．
해답은 책 끝에 毫＞

四

===== PAGE 257 =====
256 =====
이제까지 학습한 내용을 중심으로 books.xmF을 기초로 하여 도서 검색
프로그램을 작성해 봅시다．

index.html
I

srch.html

k기《긔가〔.html

I 학습 내용 미리 보기
（出
（E) 편召
（Er 보기
（y) i겨찾기
（印 도구① 도晷맡
파일
4」뒤로 '

9 〕 公

a검색 曳哥겨찾거 砂대디머 J

ㅢ，
J

도서 검색 프로그램

resulf.js

○XML

출판사 영진닷컴 =l

-

\'勾 Lesson 22
L［〕Q&a

카E∥고리 발간일ㅣ
71씌

n E Sㅣ G N
『'b누’
：「n“．
畛

（O15)
l IrnJ1, 디자인 비주얼 가이드
표ndI, 태그푤 쉽게 이해할 수 있도록 설명한 책이Ct 이 책은 크게 세 가지
부분으로 구성되어 있다 첫 번째는 Tutorial 편 으로 표1lJL의 기초를 알기 쉽
게 설명했다 두 번째는 kcfbrence와 practice 편이다 여기에서는 튜토리얼 편
에서 제츈한ㅐ：1ldL의 기본적인 기눙에서 나아가 응용 심화 학습을 할 수 있
도록 하였다 세 번째는 Step Up 편이다
n800원

包IH

〔．Key Point ) _
이번 Lesson에서는 ×SLT를 기초로 '제 9일 Lesson21 : XSLT에서 동적인 정렬 실행하기"와는 대
조적인 DOM을 실질적으로 응용합니다. DOM을 마무리함과 동시에 XSLT 프로그래밍과의 차이점에
주목하여 학습합니다．
이번 Lesson을 학습한 후에는 XSLT와 DOM을 분리하지 않고 상호 보완적으로 사용할 것이므로，
양쪽의 장단점을 파악해 두는 것이 대단히 중요합니다．

===== PAGE 258 =====
257 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

※ [m]폴더에 [D3] 폴더의 bookaxml, book2.css를복사합니다. 또한html.jpg, asp.jpg, pc.jpg도복사해 두십시오．

1

새 문서를 열어 리스트 1∼리스트 4의 코드를 입력하고, 각각 index.html, srch.htm,
blarik.html, resuit.js라는 이름으로 저장한다．
리스트 1: index.htrn
<html>

…

<head>
<title＞도서 검색 프로그램＜/title>
</head>
<frameset rows= "200, *" border="0">
<frame src="srch.html" name="up" scrolling= 'no'
noresize=1'noresize" I>
<frame src=''blank.html ' name= 'down ' scrolling="auto' I>
</frameset>
</html>
리스트 2 : srch.html
<html>
<head>
<title＞검색 조건 입력＜/title>
<script language= "JavaScript" src="result. js"></script>
</head>
6 ㅑ <body>
l

7 : <hl＞도서 검색 프로二l램＜/hl>
<hr />
<form name="fm" >
<table>
<tr>
<th align="right " ＞출판사＜/th>
<td>
<select name="pub">
<option value=" ' selected="selected">전i</option>
<option value=" 영진닷컴"＞영진닷컴＜/option>
<option value= " 정보문화사"＞정보문화사＜/option>

===== PAGE 259 =====
258 =====
<option value= " 길벗“＞길벗＜Ioption>
</select>
</ t=d>
</tr>
<tr>
<th align="right" ＞카테고리＜/th>
<td>
<input type="text " nanie="key" size="15" maxlength="15" I>
<Itd>
</tㅍr>
<tr>
<th align= "right "＞발간일＜/th>
<td>
<input type="text " riame= "pDat " size="12" maxlength="lO" I>
</tㅍd>
</tㅍr>
<tr>
<td colspan="2" align="right ">
<input type= "button" name="srch" value= " 검색'
onclick="disp() "I>
</ tㅍd>
</ tㅍr>
<Itable>
<If ornt'
<Ibody>
</htrnl>

리스트 3 : blank.html
<html>
</html>

===== PAGE 260 =====
259 =====
제9일 클라이언트 중심의 XML 프로그래밍

리스트 4 : res네t.js
function dispO{
var strPth=parent.up. fm.pub.vaiue;
var strKey=parent.up. fm.key.value;
var strDat=parent .up. fm.pDat .value;
var ob§Doc=new ActiveXObject ( "Msxml2 . DONDocument ) '
objDoc . async= false;
objDoc.load( "books.xml") ;
flg=faise;
strFlt=" /books/book'1;
if (strPub!="") {
strFlt+=' [(pablish = ' " + strPu.b + '1 ' ) " '
flg=true;
}
if (strKey!="") {
if (fig) {
strFit+=" and " '
}eise{
strFit+=" [";
flg=true;
}
strFlt+=" (category =' ' + strKey +

'1 '

) '
"

}
if (strDat!=' ") {
if (fig) {
strFit+=" and ";
}eise{
strFit+=" [";
fig=true;
)
strFlt+=' (pDate >= ' " + strDat + "" ) " '
)
if (fig) {strFlt+="]"; }
var cinNothobjDoc.seiectNodes(strFit) ;
with(parent .down.documentD {
open( "text/html" ) F
writein( "<htmi><head><title>검색결과＜/titie> " ) '
writeln( "<iink rel=\ "styiesheet\ '' type= \"text/css\ "

===== PAGE 261 =====
260 =====
bref=\"book2.css\" I>");
38

writeln("</head><body>");

39

var cnt=l;

40

for(i=0;i<clnNod.length;i++){

41

objNod=clnNod.item(i);

4그

objLog=objNod.selectSingleNode ( "logo") ;

4,

objNam=objNod. selectSingleNode ( "name") ;

44

objAut=objNod.selectSingleNode ( "author") ;

4…

objPrc=objNod. selectSingleNode ( "price") ;

4f

objMem=objNod.selectSingleNode ( "memo") ;

4;

writeln ( "<table border= '0 '><tr><td width= '150 '>") ;

48

if (objLog!=null && objLog.text! =' ' ) {

49 :

writeln ( "<img src= " + ob§Log. text +
width= '120 ' height= '150 ' I>") ;

l

50

}
writeln ( "<td valign= 'bottom'>") ;

32

writeln ( "<dl>.'zdt>" + cnt + " .「 ) '

53

writeln (objNam.text + " ( " + objAut.text + ") " + " </dt沈》" ) '

54

writeln ( "<dd>" + objMem.text + '<br I>") ;

55

writeln ( "<div style= text-aligii: right '>") ;

56

writeln (objPrc.text + " 원＜/div></dd></d1>

57

cnt++;

</td></tr><Itable><hr I>") ;

58

}

59

writeln ( "< /body></html>") ;
close ( 》'

60
6l
62

}
}

폴더를열어indexhtm1을실행한다．
2u ］

===== PAGE 262 =====
261 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

익스플로러에서 index.hti粗을 실행하여 검색 조건 입력 화면에 적당한 키를 입력했을 때 아래 프
레임에 검색 결과가 표시된다면 성공입니다．
1 각 파일간의 관계
이번 예제는 6개의 파일이 연결되어 작동하고 있습니다. 소스 코드를살펴보기 전에 먼저 각각 파
일의 관계를 명확하게 알아보겠습니다．

파일명

m

-

books.xml

도서 정보를 입력한 XML- 파일

index.html

상하 프레임을 생성하기 위한 HTML 파일

srch.html

검색 조건을 입력하기 위한 HTML 파일（위 프레임）

blanKhtml

초기 상태에서 아래 프레임을 표시하기 위한 더미 HTMㄴ 파일（아래 프레임）

result.js

srch.html에서 호출된 XML 파일의 검색 및 검색 결과를 표시하는 JavaSc야)t 파일

bookZcss

result.js에 의해 생성된 검색 결과를 출력하기 위한 css 스타일 시트

2 JavaScript 파일의 분리
로직이 복잡하게 되면 당연히 소스는 길어지고 전체적으로 파악하기 어려워집니다. XJvIL+XSLT
프로그래밍의 기본은 데이터와 스타일을 명확히 분리해 소스를 다루기 쉽게 하는 것이며, 仄OM 프
로그래밍을 통해서도 구현하는 것입니다. DOM 프로그램을 외부 파일로 작성하는 것도 가능합니
다. srch.html의 4행을살펴보겠습니다．
戶二：寸咫一IJ

纛魚｛殲
이 문장은 resuit.js에 작성되어 있는 프로그램을 srch.htnil에서 작성된 것처럼 사용할 수 있도록
해줍니다．

3 검색 조건어써 xPath식을 생성힌다
검색 프로그램이 작성된 result.js를 전체적으로살펴보겠습니다．
resut.js에 작성 사용자 정의 함수diSp는 크게 전반부와후반부로 나뉩니다．
전반부
（2-'33행）
는 srch.html의 <ta疇 요소에 입력된 검색 조건을 구해서 그 검색 조건에 맞는
（34---62행）
를 books.xml에서 추출합니다. 그리고 후반부
에서는 추출된
서적 정보
（<book> 요소）
<book> 요소의 상세 정보를 읽어내어 실제로 브라우저에 표시합니다．

26I

===== PAGE 263 =====
262 =====
후반부는 단지 결과 데이터를 읽어내는 것뿐이므로 제 5일의 학습을 참고로 하고 여기에서는 이
프로그램의 핵심인 전반부를중점으로 분석하겠습니다．
2--4행에서 먼저, srch.htnil의 佃ble) 요소에 입력된 검색 조건을 각각 변수에 대입합니다．
var strPub=parent . up. fin.pub. value;
var strKey=parent.up. fm.key.value;
var strDat=parent .up. fm.pDat .value;

一

JavaScript으l parent 프로퍼티는 현재 프레임의 부모에 해당하는 도큐먼트를 참조합니다．이 예제에서는
index.html이 해당됩니다．
<frame name="up") - <form name="tm") - (select name="pub"〉과 같이 단계적으로 검색하게 되면 최종적
으로 pub에 나타난 선택 박스의 vaiue 프로퍼티
（값）
를 참조해 데이터를 구하게 됩니다．

flg=false;

변수 fig는 10-'31행에서 설정한 필터 패턴에 따라 xPath에 의한 조건식을 추가합니다. 초기값은
false
（조건식이 없디〕
로 하며 10---31행에서 조건식이 추가되면 true가 됩니다
（12, 19, 28행）
.
strFlt=" /books/book' ;

9행에서는 서적 정보 요소
（(book> 요소）
를 selectNodes 메소드를 사용해서 추출하고, 변수 strFlt
에 인수가 될만한 xath식을 설정합니다．
초기값으로 기본이 되는 4ook> 요소의 경로를 지정하고 추출할 <book) 요소를 10---31행에서의
횔터 패턴으로 지정입니다．
if (strPub!=" ") {
strFlt+ ="[(publish = ' " + strPub + " ' ) ";
flg=true;
}

10--13행은 검색키로 출판사 가 지정되어 있는지를 결정합니다．
출판시꿱 검색 값이 '전부
＇가 아닌 다른 값
（이를테면 변수 strPub가 공백이 아니라면）
, 예를 들

e

===== PAGE 264 =====
263 =====
제9일 클라이언트 중심의 XML 프로그래밍

에 추가합니
어 '영진딧컴'이 선택되었다면 '[(publish '영진닷컴' y과 같은 문자열을 변수 strPul）
에 입력된 xPath식은 'books/book[(publish= '영진닷컴' )' 으로 설정됩
다. 이 시점에서 변수strPul）
니다．
이후14'-22, 23'- 31행에서는각각 카테고리' , 발간일’ 이 지정되어 있는지 없는지를판단하여
(14, 23행）
, 지정되어 있는경우에는 필터 패턴으로조건식을추가합니다
（21, 30행）
.
이때, 변수fig는두 번째의 조건식 이후의 fig의 값에 따라분기 여부를 결정하게 됩니다．
즉, fig가 true인 경우(15행）조건식이 이미 사용되었음을 의미하므로 조건식을 연결하기 위해
'and' 를 삽입하고
（16행）
, 만약 false라면
（17행째）
에는 조건식의 시작을 의미하는 r 을 삽입하게 됩
니다
（18행）
.
또한, 驢f(f1g거∼’는 if(fig=trueH∼’와같은의미입니다． '

"

'==' 는 JavaScript의 비교 연산자로 '같다' 라는 의민이며, 대입을 나타내는 '=' 과는 구별되므로 주의해 주십시오．
（비교식에서 '==' 를 사용하면 반듸 true 값이 반환됩니다,)

if (fig) {strFit+=.' 〕" } '

마지막으로 32행에서는 fig가 true라면 조건식이 이미 설정되어 있음을 의미하므로 필터 패턴에
'[' 를추가합니다．
var cinNod=ob3floc.seiectNodes (strFit) ;

완성된 xPath식은 33행의 seleetNodes 메소드의 인수가 되어 books.xml에서 조건에 해당하는
<book> 요소를 포함하는 XMLDOIV1NodeList 오브젝트를 얻습니다．
요소가 존재하지 않는 경우의 대응
프로그램의 후반무는 조건에 맞은 <book> 소군을 나타내는 XIV1LDOIViNodeList 오브젝트에서
하나 하나 伯0ok> 요소를 순서대로 골라내고 각 자식 요소의 검색 결과를 E Th로 변환합니다. 이
부분은 이미 앞에서 학습한 제 5일∼제 6일의 내용에 해당합니다．
여기에서 주의할 것은 48행째의 if문에 의한 조건 분기입니다．

===== PAGE 265 =====
264 =====
48

f(objLog!=null && objLog.text!= " ){

변수 objLog는, 42행에서 얻은 <logo) 요소를 나타내지만 XML 문서의 내용에 의해 이것이 존재
（얻은 objfrg가 flu끄）경우, 혹은
하지 않는 경우도 있습니다. 즉 logo> 요소 자체가 존재하지 않는
（얻은 objLog의 text 프로퍼티가 빈 문자열）경우입니다．
<logo> 요소는존재하지만그 안이 공백인
48행에서는 이런 경우, 에러가 발생하거나 화면이 비정상적으로 표시되는 상황을막아줍니다. 제
3일 Lesson7에서 다룬 descript.xsl의 20--28행을 참고하기 바랍니다.

'&&' 는 JavaScript의 논리 연산자로 2개 값의 논리적인 값을 구하는 것입니다. '&&' 로 연결된 양쪽의 비교식의
값이 true인 경우에만 참이 됩니다，

夕
·<script）
태그의 src 옵션을 사용함으로써 JavaScript의 코드를 HTML에서 분리할 수 있습니다．
·DOM에서의 XML 문서 검색은 xPath식을 이용합니다．
· '요소가 존재하지 않는다' 라는 정확한 의미는 요소가 존재하지 않는 경우는 물론 요소의 내용이 비어 있는 경우를
말합니다. 조건을 분기하는 경우, 양쪽을 포함하도록 조건식을 지정해야 합니다．

-

⑩ i실력 테스트
w

예제 result.js를수정해 검색 결과를 테이블로 표시해 보기 바랍니다．
표의 모양은제 3일 Lesson7의 내용을참고하기 바랍니다．
해답은 책 끝에 今

===== PAGE 266 =====
265 =====
제9일 클라이언트 중심의 ×ML 프로그래밍

Go to XML

===== PAGE 267 =====
266 =====
Lesson 23 - Lesson 24

서버 중심의
XML Jr르그래밍
드디어 마지막 학습일입니다．
이번 Lesson에서는 자바 기반 스크립트인 ASP(Acitive Server Pages）
를 이용한 프로그램에 대해 학습
하겠습니다. 지금까지의 클라이언트 기반 스크립트에서는 작성이 불가능했던 내용이 자바 기반 스크립
트에서는 해결되는 것을알수 있을 것입니다．
파일을 가동하는 것만으로 동작하는 클리이언트 기반 스크립트와는 달리 자바 기반 스크립트에서는 사
전 설정이 필요합니다. 그러나 이 책의 설명을 따라 설정한다면 결코 어려운 것이 아니므로 우선은 실졔
로작동시키는 것에 중점을 두어 학습하기 바랍니다．

===== PAGE 268 =====
267 =====
오늘 공부할 내용들
XSLT를 동적으로 변환하기
XML 파일을 csv 파일로 변환하기

===== PAGE 269 =====
268 =====
세0일 서버 중심의 XML 프로：〕래밍

XSLT를 동적으로 변환하기
URL에 쿼리 정보
（？∼의 부분：를 입력하여 ><SLT를 조작해 봅시다．

학습 내용 미리 보기
trans.asp

Q XML
土닙 曲Less。
n 23
ㄴE〕Q&a

띠얼江） 낀口正t 보겨，·겨 가l& 도구'It 도욥돠산f)

굽玄 새i뀀甘 송

ala . 「
Ill나

.,

，…

省立 튤j多 븍i各 在

,,1 ,,,?,.
511

｀』 →于

궉 온허듣

"

Web 관련 서적 목록
SBN 코…
서적
서시
츌핀시 가걱 발간밀
SBNBN-314-2014-S IS일만에 배우는 Asuot C++ C0 Seto Herota
영 찬 딧컴 I딧〔l) ai32-c12-cC
28N88-319-I894百할珂F>(F죵허 사전
슈와 시스∼영진딧컴 1또mSASS-Si碼
2B289-314니978-3 AS戶 사친
니시자와 나오SI옇진닷컴 ISAma〕
기iim
SW+SS314-t 042-c町At디자인 비추혈 가이드 C I.S
＼형친닷컴 Hㄸ
【〕an 田ㅢn
Yate,gmn.can V

- hhp:／기0CahoSt/
（혜10/tranS.asp라고 지정한 경우

Key Point
파일迂） B집｀트＞ 보기
（Y) i겨찾기IA)

이번 ㄴesson에서는 ASP

蟲 ＇「

규 새巍 令

(Acitive Server Pages}

주소：D）
ㅣ h"n U衲∼…m닛r

활용하여 ×ML 프로그램을

상세 정보 표시

작성해 보겠습니다. 처음에

■
211 R,,
Arn)r。
?e
發 儲기 儡기 P磅높' ,J

도구
（J) 도묩맣i出

L4니하： r

h內커H

4

: 1 iai둥

면료 ∥

01 ASnAl. 디자인 비주얼 가이드 (CLI)
HTld工 태그릍 쉽게 이해할 수 있도촉 설명한 책이다 이 책은 크게 세
가지 부분으로 구성되어 있다 첫 번째는 Tatonni 편 으로 ETlAL의 기초
률 앝긔 쉽게 설명했다 두 번째는 Reference와 practice 편이다 여기에서
는 류토리얼 편에서 제츨한 且盼4工의 기몬적인 기능에서 나아가 응용
심화 학습을 할 수 있도록 하였다 세 번째는 Step Up 편이다
11,80口뭔

는 당황할지도 모르겠지만，
자AlL에서 이런 것도 가능하
다는 것을 체험하기 위해서
라도 도전해 보기 바랍니다．
사현

ASP에 관한 상세한 소개는
생략하고 실제로 프로그램

0R ASP 사전 Cㅢ시자와 나오키）
ASP의 모든 명령올 녜 포캣속에 Pcket Reference ASP 샤전 은 ASP의
긔본적인 지식과 사용 가능한 명령의 구문，
구문에 대한 상세한 샐명
명령 활웅 예를 ASP 오브젝트．ADO, PdeSyntemObjectSl 메소드 프로퍼
티로 분류하여 언제든지 쉽게 찻아 참조할 수 있도록 한 사전샥 레퍼런
스입니다
1r 〕0읜

도서를 참고하기 바랍니다，

r］
완료

n

口

에 대한 자세한 내용은 관련

〕그 갖찌 P1 껄
ㅢ 二

二

용만 다루고 있습니다. ASP

ㅗ
n
슈 `

을 작성하는데 꼭 필요한 내

번

口

螺ㅏ 나

긍 ㅓ

H
＝」

이 책에서는 지면 사정상

민트라냇

乙

http://IocaIhost/xmllO/trans.asp?trn=descript라고 지정한 경우

===== PAGE 270 =====
269 =====
제10일 서버 중심의 XML프로그래밍

※[D21 폴더의 bOOkS.XSI, books.css, [D31 *더의 books.xml, description.xsl, book2.cs, asp.jpg, pc.jpg, vc.jpgD10]폴더에 복사하기 바랍니다．

새문서를열어리스트의코드를입력한후［D10〕폴더에trans.asp라는이름으로저장
한다．
리스트 : trans. 廷琿：蓼
<9taLang1iage= " JavaScript

96>

<96
var objDoc=new ActiveXObject ( "Msmi12 . DOMDocument' ) ;
objDcc. async=false;
objDoc . load(Server .MapPath ( "books .xml" )) '
var objgtl=new ActiveXObject ( "Msonl2 . FreeThreadedDOMDocument ') ;
objSt1.async=false;
if (Request.QueryString( "trn ") .ItemO=="descript") {
objStl . load(Server.MapPath( "description.xsl "fl;
}else{
objStl. load(Server.MapPath( "books.xslH) ;
}
var objTmp=new ActiveXOb§ect《 "Nsanl2 .XSLTexnplate" ) ;
objTmp. stylesheet=obj Sti;
objPrc=objTmp. createProcessor ( 》;
:L6 objPrc . input=objDoc;
17 야功Prc . transform ) '
Response.Write (objPrC . outpu디 '
%>

]

Check

ASP 파일의 확장자는
자바기반하에동작하는ASP파일은확장자 '.aSβ 로저장합니다．

===== PAGE 271 =====
270 =====
2

를인스톨한다．'setup.exe' (Check point참조）
를더블클릭하
PWS(Pers。
nal Web Server）
고설치 화면에서［다읨버튼을클릭한다．
므「gUn引 Web S回잃包 설치
lansottlRI

Personal Web Server
tlD.

Personal Web
sIoI
Server
(PWS)
SEII 0 2}
5vr

AF용SQI " ’「“컵 “ " "머 "

다믐 기능을 포함합니다：

．逾

Personal Web Server
Transaction Server
Data Access Comeonents
Messave Queue Servee Client
Easy Mministraxiofl

「百暫巫니

I

‘겨1`1,',.r
``/

11`

→日寸．
.，느
ㅃ－='｀

취소

-

,心－

1

｀느／1,

發許朴必

ASP를 동작시키려면 사전에 서버상의 설정을 해둘 필요가 있습니다. 이 Lesson에서는
Windows 98/200(〕
등셰서 동작하는 PWS(Personal Web Server）
의 설치 방법과 사용법을

간단히 소개하겠습니다．
PWS Windows 98 CD-ROM의（ㅇ 드라이브명）
:\add-ons\pws'setup.exe으로설치합니다．
Windows NT Workstation의 경우는, Windows NT Option Pack의 setup.exe으로 설치합니다．
Windows 200(）
에서는기본적으로PwS가설치 되어 있습니다．
그러나, Windows Me는PWSmS을 지원하지 않습니다．

설치방법에서 匡준설치］버튼을클릭한다．
" ∼mPersonal Web Server 글치

，∼g∼a

…∼m少씌

Personal Web Server

匈
（M)
!1鹹

S S EI 3 atQUI 5altUEI.

A10l5

t""" ?lE "
'

5I

，쯔쁘쯔 喜蟹譎蜀珊嚼瑟攝罷틋辯성'蠻當懿泉7'
4*5섶5W) 難晧料甛壕텔뛸泌器離諶机球든8璡

（뒤로咀＞

-

ㅣ

취＝

3

-

===== PAGE 272 =====
271 =====
4

홈폴더의 설정 화면에서, 초기값그대로［다음］버튼을클릭한다．
Miaomft

勿

Personal Web Server
다
미 I더I 기뵨 社 게시 甚 디텍터리로 섦치힙t」

w斟낚 서HI 스
（뾰）
卜
＝ ￦ne‘口Jb￦？79Y\，「긔川

찾마보기
（旦）
… -

미 薑더률 기뵨 Fㄲ 게시 디텍터리로 설치합니다

-

용용 프로그험 따일올 미 1더脯 섭치힘d」
口

다욤《N》＞

-

취소

-

［마침］버튼을 클릭하여 설치를종료한다．
Micros얘 Personal Yreb 1 r .0 설치

M oroP

必

Personal Web Server

MIc roSoft 소프트웨어를 사욤헤 주셔서 감사힙頀」
［L
혐치굘 甘내리면［마智l景 누르거나 (Enter> 키！누르십시오

'::,: 퍼스널 웹 서버를실행하여［고급］
툴을 선택한후,［추개 버튼을클릭한다．
*F日

나

`

＝」∼∼

…∼」
…m丘烈뜨注

斗n쟀n口緇擁轟客聽鞭_

x

（y) 도묩맡(出
I륵 정보但） 보거

衲

고급
옵션
가삼 口텍터리
.9 m0me구＞
」 川TAUt川N
4 /LISHELP
4 刈55AMPLb S
4 /rrrnadc
」 /SCAIPTS
걔 /WEBPUE

庶
苔

추가
（스）．一
듕륵 정보 편집
（l

F 기믄 문서 사욤(軫
'“
「'h

IC eN(.)r

i夕
'i

rUots> t htrn.DetaoIt. 」cp

「 디렉터리 찾마보기 허뮴
（뾰）
I7 쾨 礖匡墅I루구츠匿
《蛟

Hi 그」

1

스」

===== PAGE 273 =====
272 =====
7 ［디렉터리추개상ㅈF 1서,7FAcJ디렉터리를ㄷ梏과같이설정한다．
.

디렉터리 추가
디렉터리
（흐）
별명（스＞;

Wx떼

찾마보기
（旦）
…

IxrnhIo

액세스
「－！즈多랄蔞
（斟

口 읽기
（聊
확인

취소

'.
·'

ASP파일을 저장한 폴더의 경로를 지정
（예를 들어 'C:\xml')

［별명］

xmllO
（자유롭게 변경할 수 있다.)

［읽기］

체크한다．

［실행］

체크하지 않는다．

［스크립트］

체크하지 않는다

∼

'

∥

긴口

'1 「一

［디렉터리］

U

,

， ∼山

/ 꽈

，口

이것에 의해 http://1oc1host/xmJ10/trans.as 로 접근이 가능하게 된다．

ISS/PwS를 실행한 후 브라우저에서 http://1oca1host/xm110/trans.asp' 혹은'http://
1ocaIhost/xmll0/tmns.asp?trn=descript 라고 입력합니다. 도서 목록 화면과 도서 상세 화면이 각
각 표시된다면 성공입니다．
또한, ASP 파일은 익스플로러에서 직접 실행할 수 없기 때문에 주의해 주십시오．

1 XSLT 스타일 시트를 불러낸다
XMLDOMDocument2 오브젝트는, 용도에 따라두 종류의 오브젝트로 분류됩니다．
첫번째는 Renta-Thereaded 모델로 아래와같은 코드로 작성됩니다. 동시 엑서스에 대한감시를
행하지 않는 경우에 사용하며 높은 퍼포먼스를 제공합니다. 일반적으로 많이 사용되는 모델입니다．
var ob」
Doc=new ActiveXObject( "Msa].2 DONflocument " 》'

두 번째는한개가동시의 엑서스 제어 등을 가능하게 하는 Free-Thereaded 모델입니다．

===== PAGE 274 =====
273 =====
제10일 서버 중심의 >KMㄴ프로그래밍

여기에서는 호출된 )(SLT 스타일 시트가 여러 XML문서에서 공유될 가능성이 있기 때문에 동시
엑서스의 제어 기능을 갖는 Free-Thereaded 모델을 사용하기로 합니다．
Free-Thereaded 모델을 생성 할 경우도 기본적으로는 종래와같은방법으로 작성합니다．
var 山dStl=new ActiveXObject ( "Msxm12 . FreeThreadedDOMDocument " ) '
objStl .async=false;
if (Request.QueryString《 " tm1" 》. Item( ) == ' descript" ) {
objStl.load(Server.MapPath( "description.xsl' ) );
}else{
objStl.load(Server.MapPath( "books.xsl") );
}

또한 호출되는 XSLT스타일 시트는, 쿼리 정보로 전환됩니다. 쿼리 정보는 UBL의 마지막 부분에
'1를 입력한후 '키＝값으로작성되는간단한정보로, 이번 예제의 경우에서는 '∼？tm=descript
으로작성된 부분입니다．
'--?trn=descript 으로 지정된 경우는 description.xsl을 호출하며
（9행）
, 그 이외의 것이 지정된 경
우
（또는 지정되지 않은 경우片나）
ooks.xsl을호출합니다
（II행）
.
8행에서 사용하고 있는 Request.QueiyString' 문장은 인수에 지정된 키를 사용하여 쿼리 정보를
반환합니다．

∼
시작 부분의 <3'o@Language %＞는 선언문으로써, 여기에서는 '.asp' 파일에서 사용된 스크립트 언어를 선언합
니다. 반드시 페이지 시작 부분에 작성해야 합니다．

XSLT스타일 시트를 적용핸가
호출된 XSLT 스타일 시트는 MsXML 파서에 의해 XSLT 스타일 시트 프로세서에 의해 처리되도
록XSLTemplate오브젝트에 삽입됩니다《13, 14행）
.
var objTmp=new ActiveXObject ( "Msxm12 .XSLTeinplate" ) '
obj ㄸ노rㄸ）
. stylesheet=objStl;

다음에는XSLTemplate 오브젝트의 creatProcessor 메소드를 이용해 XSUrocessor 오브젝트를
생성합니다. XSLTemplate오브젝트가XSLT 전용의 저장 영역이라고한다면, XSLProcessor오브
젝트는XSLT를 조작하기 위한장치라고말할수 있습니다．

包

===== PAGE 275 =====
274 =====
c=야)jTntp. createProcessor() '

생성된 XSLProcessor 오브젝트에는 input 프로퍼티를 통해 xTh문서 books.xml이 전달됩니다．
transform 메소드는 입력된 xTh을 XSLT를 사용해 변환하기 위한 메소드입니다．
변환 결과는 output 메소드로 생성되며 이것을 ASP가 제공하는 Response.Write 메소드를 사용
해 결과를 브라우저 상에 표시합니다．
Doc;
objPrc . input=ob」
objPrc. transform( ) '
Response.Write(objPrc . output) '

또한, XSLTemplate 오브젝트를 사용한 변환은 클라이언트 기반에서도 사용할 수 있고, 종래의
（단, 이번에 소개한 변환 방법이 보다
transformNode 메소드를 사용한 변환도 사용할 수 있습니다
높은 퍼포먼스를 실현할 수 있습니다）
.
-

臘
`-

· XMLDOMDocument2 오브젝트는 Rental-Threaded 모델과 병행 처리할 수 있는 Free-Threaded 모델이 존
재합니다．
· 복수 처리에서 공유될 가능성이 있는 ×SLㅜ스타일 시트는 Free-Threaded 모델을 사용합니다．
· XSLT에 의한 변환시 XSLT 스타일 시트를 XSLTempla伯 오브젝트에 입력해야 합니다．
· XSLT에 의한 실제 변환은 XSLProcessor 오브젝트를 사용하며 XSLProcessor 오브젝트는 XSLㅜ 스타일 시트
가 입력된 XSLTem히ate 오브젝트를 통해 XML문서의 XSLT에 의한 변환 결과를 출력합니다．

-

w

ASP를 사용해 XML 문서 books.xml과 XSLT 스타일 시트 books.xsl을 연결시켜 봅니다. 단, 아래
조건을 만족하도록 작성합니다．
· <aate）
요소 키를 기준으로 오름차순으로 정렬되도록 스타일 시트를 작성합니다．
· 변환시 XSLProcessor 오브젝트를 사용합니다．
해답은 책 끝에 별：)

===== PAGE 276 =====
275 =====
제10일 서버 중심의 ×ML프로그래밍

Go to XML

===== PAGE 277 =====
276 =====
/24

。

xThO」

:

AIUI.
：』XML!!J

니

지AL. 파일을 csv 파일로 변환하기
사전에 준비된 )<ML 파일 books.x倒을 result.csv로 변환해 저장합니다．

4.
-

峰？

z f. 「'

也L'

"

H

. r
A
ㅣname 小 -B
1 loon
1name
2＜ b匕Nㅂ닝5]4니
긺
ISBN89-314-1742-x
/42-x HiM)
HML 니사빈
디자인 비수별
비주얼 가미느
가이드
3 I59N89 引4-1979-3 ASP 사전
-

-8

- :：븜싸8,U,-31-.：珊，
닝，
,/8.: ,3 ^，斗，含lP묘N ,,,,

小닢而石

.

sr,r

11

∼ …
author ∼〔i
C
authㅇr
OI.S
uLS
니시자와 나오키

E：
「F
logoD
mg
.a,
cnlegory
∼니n
ui)
0g
（… （ateg0ry
un
htm」
05111.ipg
http://aaam.younglin.com
p= HTMC
TML
h汁p「乙／
川硼此younglnc=1rn
enpipo
ASP
ht1p//waw.youngi)n.com

（三
陋，:.C三
prKe
ㅣ
S

W加∼5aJftE1C。-n
vc.lpg
IHJ http://wwa,y。ungfln.c。m

졈－

빴，
사와．,:／오키 a乳］p…裝,. 니,, h眈p//wv/wγ0un마nc0m

4 髓驪-314-1994-5 謐C ZO) Al뇨aJ CI-l 6.。饉'；盞.
n
니 ㄱ
J
t ＾
。 0
U

Less。
n 24
L 口 Q&a

"

1n
H d 卜 H\［且且묘坐丁
죤비

l

m-

솝- \

暳〕따일
（E) 편집
（트》 보7K꾀 삽입
（D 서삭(Ql 도구＜工） 더이터(2) 執뾰）도욤말(H)

,

Q XML

asp

!

학습 내용 미리 보기

욜＝

D

xml2csv.

L그

books.xml

변환된 csv 파일을 엑셀에서 실행한 경우

아무리 ×ML 파일이 범용성 있는 데이터 형식이라 해도 아직 지원되지 않는 프로그램이나 시스템이
다수 존재합니다. 이런 경우 )<ML 파일을 다른 형식의 파일로 변환해 줄 필요성이 있습니다．
이번 Lesson에서는 csv
（쉼표 분리 텍스트）
로 변환해 보겠습니다．

===== PAGE 278 =====
277 =====
제10임 서버 중심의 ×ML프로그래밍

의 books.xml을 열어 리스트1과 같이 요소의 순서 정리, 일부 요소를
Lesson23({D1이폴더）
추가하여 저장한다．
리스트 1 : books.x引
<?xinl version="1.0" encodirig= "EUC-KR" ?>
<?xml-stylesheet type= ''text/xsl' bref="description.xsl" ?>
<books title= 'Wel) 관련 서적 목록∥＞
<owner address= "www. youngjin.com'>Yongjin.com Y. <Iowner>
<book isbn= ''ISBN89-314-1742-x'>
<name>HTME』 디자인 비주얼 가이드＜/name>
<author>C.I. S</author>
<logo>htxnl . jpg</logo>
<category>HTb1L< /category>
<url>http: //www.youngjin.com </url>
<price>11800</price>
<publish＞영진닷컴＜/publish>
<pDate>2001-06-11</pDate>
<memo><keyword>HTML 태그＜/keyword＞를 쉽게 이해할 수 있도록 설명한 책이다．
이 책은 크게 세 가지 부분으로 구성되어 있다．
첫 번째는 Thtorial 편으로 可n4L의 기초를 알기 쉽게 설명했다．
두 벤재는 Reference와 practice 편이다．
여기에서는 튜토리얼 편에서 제출한 HTI』
의 기본적인 기능에서 나아가 응용 심화 학습을 할
수 있도록 하였다．
세 번째는 Step Ur) 편이다.</memo>
</book>
<book isbn= nISBN89-314-1978-3 ">
<name>ASP 사전＜/name>
<author＞니시자와 나오키 </author>
<logo>asp. jpg</logo>
<category>ASP< /category>
<url>http: //www.youngjin.com </url>
<price>15000</price>
<publish＞영진닷컴＜/pi.thlish>
<pDate>200l-ll- 30</pDate>
<memo><keyword>ASP의 모든 명령을 내 포켓 속에 </keyword>

===== PAGE 279 =====
278 =====
'Poket Reference ASP 사전은 ASP의 기본적인 지식과 사용 가능한 명령의 구문, 구문0ㅔ 대
한 상세한 설명, 명령 활용 예를 ASP 오브젝트, ADO, FileSystexnObj ect의 메소드, 프로퍼티
로 분류하여 언제든지 쉽게 찾아 참조할 수 있도록 한 사전식 레퍼런스입니다．
</rnerno>
</book>
<book isbn="ISBN89-314-1994-5">
<name＞알짜 PC 용어 사전＜/name>
<author＞슈와시스템＜/author>
<logo I>
<category＞컴퓨터 사전＜/category>
<price>19500</price>
<publish>영진닷컴＜/publish>
<pDate>2002-0l-05</pDate>
<lr冶끄幻＞이 도서의 특징은 줄임말
（약어）
에서 풀네임을
찾거나 풀네임에서 줄임말을 쉽게 찾을 수 있도록 도와준다．
또한 삽화를 통해서 이해하기 어렵거나 생소한
</memo>
용어에 대해서 이해도를 높이고 있다．
</book>
<book isbn="ISBN89-314-2014-5">
<name>l0일만에 배우는 Visual C++ 6.0< /name>
<author>Seto Haruka< /author>
<logo>vc . jpg</logo>
<url>http: //www.youngj in. corn </url>
<price>15000</price>
<publish＞영진닷컴＜/publish>
</pDate>2002 -02-05< /pDate>
갑neino＞이 책은 Microsoft Visual C++ 6.0에 대해 22개의 단원을 10일 동안 순서대로
학습하도록 되어 있다．
Lessoni에서는 간단한 Windows 프로그램을 직접 만들어 봄으로써 앞으로 펼쳐질 이 책의 무궁
무진함을 맛보게 한다. Lesson2부터는 직접 Visual C+＋을 실행하고, 소스를 분석하면서 언어의
기본적인 개념을 잡아 나가고, 마지막 Lesson22에서는 이미 습득한 API 함수 사용법, 리소스 작
성법 등을 이용해 Windowㅌ 응용 프로그램을 독자 스스로 코딩할 수 있게 한다.<Irnemo>
</book>
< /books>

===== PAGE 280 =====
279 =====
제10일 서버 중심의 ×ML프로그래밍

이 순서의 조작은

Check

요소에 가지런히 정돈해 둘 필요가 있기 마문입
（조；V 파일에 저장된 자식 요소를 모든 ◇ook）

莎뒝娃＇"

니다. 물론 자식 요소가 정리되지 않더라도 상관은 없지만 소스가 장황해지므로 정리하도록
합니다．

2

새문서를열어 리스트2의 코드를입력하고, [D10］폴더에 xnil2csv.asp라는이름으로저장
한다．
리스트 2 : xml2csv,asp
<%@Language= "JavaScriptn %>
<html>
<head>
<title> XMI』
파일에서 csv형식으로의 변환＜/title>
</head>
<body>
<%
var ohjFs=new ActiveXObject ( " Scripting.FileSystemObject' ) '
var objTs=objFs .CreateTextFile(Server.MapPath( "result .csv'1 ) ,true) ;
var objDoc=new ActiveXObject ( "Ms그cn12 .DOMDocument") ;
objDoc.async=false;
ohjDoc . load(Server.Mappath( 'books.xml " ) ) '
var clnNod=objDoc . documentElernent.childNodes;
var clnTtll= clnNod.item(l) .attributes;
var clnTtl2=clnNod.item(l) . childNodes;
for (i=0;i<clnTtll. length;i++) {
objTs.Write(clnTtll. item(i) .nodeName + " ' '1 ) '
}
for (i=0;i<clnTtl2 . length;i++) {
objTs.Write(clnTtl2.item(i) .nodeName + " , " ) '
}
objTs.Write( "\r ' ) ;
for(i=l; i<clnNod.length;i++) {
var clnDatl=clnNod.item(i) .attributes;
var clnDat2=clnNod.item(i) . childNodes;
for (j=0; j<clnflatl. length; j+-4-){

===== PAGE 281 =====
280 =====
objTs.Write(clnDatl.item(引 .text + " , " 》;
}
for (j =0; j <clnDat2 . length; j ++ ) {
objTs.Write (clnDat2 . item(j ) .text + " , " ) '
}
objTs.Write ( "\r ") ;
}
objTs.CloseO;
%>
</body>
</htinl>

3 lls/Pws를실행한후브라우저에서 'http://1ocalost/xml10/xml2csv.as 라고입력한다．

lls/Pws를 실행한 후 브라우저에서 h tp://(X名l
（冷t/xmll0/xm12csv.asd 라고 입력합니다. 실
행 후 xml2csv.asp 파일이 저장된 폴더에 변환 결과인 result.csv가 생성되며, EXcd 등의 표계산
소프트웨어에서 정확히 열리면 성공입니다．
I 출력 장소를 준비한다
이번에는 생성된 변환 결과를 텍스트 파일인 result.csv로 출력합니다. 텍스트 파일에 대한 액세
스를 가능하게 하는 것은 TextStream 오브젝트입니다. TextStream 오브젝트는 FileSystem
Object오브젝트를사용하여 CreateTextFile 메소드를실행함으로써 구할수 있습니다. 8, 9행을참
조하기 바랍니다．
var（攷功Fs=new ActiveXObject ( " Scripting.FileSystemObj ect" 》'
var objTs=objFs . CreateTextFile (Server.MapPath ( 'result . csv,' ) ' true) ;

CreateTextFile 메소드는 첫 번째 인수로 지정된 파일명으로 텍스트 파일을 작성하고 그 텍스트
파일을 조작하기 위한 TextStream 오브젝트를 반환합니다. 두 번째 인수의 true는 만일 그 시점에
서 이미 같은장소에 result.csv가존재할 경우, 이것을 덮어쓰기 합니다．

===== PAGE 282 =====
281 =====
제10일 서버 중심의 XML프로그래밍

2 타0隱 행을 출력힌다
csv 파일에 있어서 각각의 데이터가 무엇을 의미하는가를 판별하기 위해 1행에 타이틀 행을 갖
는것이 일반적입니다．
13행에서 구한 ◇xioks> 요소의 <book) 요소군에서 첫번째의 <book> 요소를 꺼내어 속성군, 자식
요소군을 얻습니다．
var clriNod=objDoc. documentElement.childNodes;
var clnTtll= clnNod.item(l) .attributes;
var clnTtl2=clnNod.item(l) .childNodes;

물론 첫번째의 <book> 요소가 아니어도 상관없지만 모든 <book) 요소의 자식 요소가 순서나 개

다．

수가 정돈되어 있다는 것을 전제로 여기에서는 첫번째의 <book〉요소를 기준으로 취득하고 있습니

for (i=O;i<clnTtll. length;i++) {
objTs.Write(clnTtll. itein(i) .nodeName + " ' " ) '
}
for (i=O; i<clnTtl2 . length;i++) {
objTs.Write(clnTtl2.item(i) .nodeName + " ' " 》;
}
objTs.Write( "\r ") ;

16-21행에는 속성군, 자식 요소군의 순으로 쉼표를 이용해 노드명을 작성합니다. 여기에서는 노
드명을 각 데이터의 항목명으로 사용하고 있습니다. 22행에서는 출력 행의 종료를 의미하는 뚤바
꿈 문자＜\r)' 를 출력하고 있습니다．
· 3 데이터 부분을 출력한다
이 부분은 타이틀 행을 출력하는 문장과 거의 변한 점이 없습니다. 타이틀 행 출력시 첫 번째의
<book) 요소를 했지만 이 부분에서는 모든 행에대한 처리를 하고 있습니다．
23--33행을보기 바랍니다．
2T

for (i=l; i<clnNod.length;i++) {

2:

var clnDatl=clnNod.item(i) .attributes;

2=

var clnDat2=clnNod.item(i) .childNodes;

26 ;

for (j=0繃<cinflati . length; j++) {

!

27 :

objTs.Write(clnDatl.item(j) .text + '" ' '') '

===== PAGE 283 =====
282 =====
}
for(j=0;j<clnDat2.length;」++ ) {
objTs.Write (clnDat2 . itein(j ) .text + " ' " ) '
}
objTs.Write ( " \r" ) '

}
（26--28행, 29'--31행）
안쪽의 루프
는 1회 실행시 한 개의 데이터를 생성하고, 바깥쪽의 루프
（23'33행째）
는1회 실행시 한행을생성합니다．
만약 콤마 대신 탭으로 텍스트를 작성한다면 27, 30행
（그리고 타이틀 행을 생성하는 17, 20행）
의
',' 를 ' \t' 로치환합니다．

I:<book)
요소 개수

J:<Iy아◇ 요소의
자식 요소 개수

<?xmJ. versiou= 1.0 encoding=Euc -KR?>
<bㅇ아ㄷ8>
<name> 10일2뻬 배우는 XNL</name>
<au口ier>Sei」
i .Kimata</name>
</book>
<book>
<Ibook>
</books>

／안쪽 루트에서 한 개의 <book> 요소를，
\
바깥쪽의 루프에서 <bo아◇ 요소 전체를
＼처리한다·
/

-

似
`-

· 텍스트의 작성은 TextStream 오브젝트를 사용합니다．
· 타이틀 행은 <bo아◇ 요소를 이용해 추출합니다．
· 데이터 행은 이중 루프를 사용합니다. 안쪽의 루프에서 개개의 데이터를. 바깥쪽의 루프에서 cSv 파일의 한 행을
생성합니다，

===== PAGE 284 =====
283 =====
제10일 서버 중심의 XMㄴ프로그래밍

실력 테스트

본문의 예제를XSLT를 이용해 실행해 봅니다. 정확히 실행되도록 아래 소스의 공백을 채워 봅시다．
xml2csv.asp
<96@Language= "JavaScript " %>
<ht;m그＞
<head>l0-2 . 연습문제＜/title>
<Ihead>

<%

<body>
var objDoc=new ActiveXObj ect ( "Ms]mt12 . DO1Document") ;
objDoc . async=false;
objDoc . load( Server .MapPath( ''books .,mil" ) ) '
var objStl=new ActiveXObjec티"Msanl2 . DONDocument" ) ;
obj Stl .async=false;
objStl. load(Server.MapPath( "result. xsl ") );

鞭3立첬駐鍵茗轟裝藿瑟纛珊甕黴：蟹핍n

var objFs=new ActiveXObject《 "Scripting.FileSysteinObj ect" ) '
var objTs=objFs.CreateTextFile(Server.MapPath( "result. csv") ,true) ;
objTs.Write( [

]) '

objTs.Close ( ) '
96>

</body>
</html>

<?xml version="1.0" encoding= "ETJC-KR" ?>
<xsl = stylesheet

xxnlns : xsl= "http : / /v＼
〃w. w3 . org/1999/XSL/ Transforui"

version="l. 0">
<xsl:output method="[

1" encoding= "EUC-KR" I>

<xsl :preserve-space elements="xsl =text" />
<xsl:template inatch= " / " >
<xsl:for-each select="books/book[l] /@*[
<xsl : value-of select=" [

〕" I>

]books/book[1]/nodeQ ">

錢難鍵籌籌締瑟瑟器轟畿撫드崗驩錢赫甕旨講發驀

<xsl:text disable-output-escaping="yes">, </xsl:text>
</xsl : for-each>
<xsl text disable-output-escaping= "yes" ></xsl =text>
<xsl:for-each select="books/book">

===== PAGE 285 =====
284 =====
<xsl:for-each se1ect="@*[

]nodeO ">

<xsl:value-of select="[

1 " I>

<xsl:text disable-output-escaping="yes">,</xsl:text>
</xsl:for-each>
<xsl:text disable-output-escaping='yes" ><Ixs1:text>
</xsl:for-each>
</xsl = template>
<Ixsl:stylesheet>
해답은 책 끝께 今

먀．
XML과 나미의 원포인트 강좌

마침내 최종회！!
나미

' 드디어 끝났네요，박사님 수고하셨습니다．
'

Dr.XML

' 오물오물'

나미

' 왜 그러세요？ 저런저런, 틀니를 잃어버리셨군요. Lesson 중에는 틀림없이 있었는데. 어떻게 하셨어요？"

Dr.XML

'오물오물"

나미

' 이런 연유로 박사님께서 말씀을 하실 수 없기 때문
（게 제가 마지막 인사를．
이번 XML 강좌는 기본편이었기 때문에 ×ML에 의해서 무엇이 어떻게 될 수 있는가 하는 것보다도 XML이
란 무엇인가 하는 쪽에 중점을 두었습니다. 그러나 ×ML의 매력은 '무엇이' 라고 하는 것보다도 '어떻게' 의
쪽이 훨씬 크다고 말할 수 있습니다. 여러분이 이것을 기본으로 다양한 실용 애플리케이션에 도전할 수 있어
서 기쁩니다. 10일간 정말로 수고하셨습니다.
앗, 주머니에서 박사님의 틀니가．
.."

Dr.XML

' 오물"

나미

"그럼 여러분, 안녕히 계세요'

284

===== PAGE 286 =====
285 =====
제10일 서버 중심의 ×ML프로그래밍

Go to XML

===== PAGE 287 =====
286 =====
실력 테스트 해답
여기에는 각Lesson의 실력 테스트 해답이 실려 있습니다．

===== PAGE 288 =====
287 =====

===== PAGE 289 =====
288 =====
( Lesson 1
틀린 곳은 아래의 6군데입니다．
1. x) <?xjJ?〉의 다음단락
O)1행에 아래의 한문장을 삽입
<?xnil version="l. O " encoding= "EtJC-KR" ?>
xTh 문서의 첫 행에는 반드시 XML인 것을 나타내는 XML 선언 <?Xln1?〉이 필요합니다. 단，
version 속성은 필수이지만 encoding 속성은생략 가능하므로 아래와 같이 기술할 수 있습니다．
<?xml version="l. O " ?>
경우, XML문서는 임의로 문자 코드가 UTF-8로 설정되므로 주의합니다．
x) <book id=00001>
O) <book id= "OOOOl">
XML 문서에서 속성값은 반드시 쌍따옴표로 감싸주어야 합니다．
x) <published>···</Published>
0) <pub1ished>···</pub1ished>
XML 문서에 대／소문자는구별됩니다. 따라서 시작 태그 <published〉와 종료 태그 </Published〉의
대／소문자가 다르기 때문에 양자는 다른 요소인 것으로 간주되어 의도했던 결과를 얻을 수 없게 됩
니다．
×）
b>＜」
．.>xM1』
＜/b>< / i.＞란∼
0) <b><i>xIL</i></b>란｀
요소끼리 바르게 대응되지 않습니다. xTh에서 요소끼리 오버랩 하는 일이 없도록 시작 태그와 종
료 태그의 대응꼐 주의할 필요가 있습니다．

曲

===== PAGE 290 =====
289 =====
실력 테스트 해답

5. x)<page>
O) <page!>
)vfl 문서에서 종료 태그의 생략은 허용되지 않습니다. 만일 요소에 텍스트 정보가 존재하지 않는
경우에는 ＜요．
소명／〉과 같이 합니다. 물론다음문장과 같이 작성해도 무방합니다．
蜘－-：∼－出出∼蓬i小꾸체月一一一一→→쌘‘嚼크幽蟹巒灐發萍哮心峰興珊型蠟絮纖盤擁辨湊쁘斟毓乫

《t)aαe> < /Daae>
6

x) <owner＞영진닷컴＜/owner＞가 <books> 요소의 바깥쪽에 있습니다．
O) <owner＞영진닷컴＜/owner＞를 <books> 요소의 값 아래
（예를 들면 2행째）
에 삽입합니다．

xll 문서에서 경로
（최상위）요소는 반드시 한 개입니다. 문제 중의 xL 문서는 缸〕
ok? 2소와
<owner> 요소가 최상위 요소로서 나란히 열거되어 있습니다. 따라서 <owner〉요소를 <books> 요소
하위로 이동시켜 <books> 요소를유일한 경로 요소로 지적해야합니다．

1. 속성 주체
'꼐이터가세분화되지 않는디，
, '용량을적게 하고싶디
＇'의 두가지로판단합니다．
2. 요소 주체
"이후데이터의 재편집이 실행된디
＇'라는 점으로부터 판단합니다．

(Lesson 3 〕
diary. xml, diary. xsl
1. <?an1-sty1esheet type=.text/xsl·· href= "books . xsl·· ?>
XML 문서와XSLT스타일 시트를 연결한 경우에는 <?mil-stylesheet?> 명령을사용합니다．
二

<xsl: stylesheet xmlns:xsl="http: /Ivr'.ivi.w3 .org/1999/XSL/Transfonn"
version= '1. 0 ">

MSXML 파서가 XSLT LU을 사용하는 경우에는 xs1:sty1esheet> 요소의 xmlns:xA 속성으로 값

===== PAGE 291 =====
290 =====
을 지정해야 합니다. 이것에 의해 파서는 '鈿l：
∼' 로 시작하는 요소가 XSLT1.O의 구문 干칙에 준
하는지 판단합니다. 또한version 속성의 지정도 필수이므로 잊지 않도록주의해 주십시오．
<xsl:value-of select= "diary/day/@date" I>
속성값을추출하고싶은경우, 속성 이름앞에 반드시 '@' 를붙입니다．
<xsl = text＞날씨 : </xsl : text>
텍스트를 나타내고 싶은 경우에는 鈿l:text) 요소를 지정합니다. 단, 이 柚l:text> 요소는 생략할
수 있습니다．
<xsl:value-of select= "diary/@owner"I>
요소의 내용을나타내고 싶은 경우, 柚l:value-of> 요소를 사용합니다．

(Lesson 4
music. xml, music. xsl
1 . method="html"
柚l:output> 요소를 지정한 경우에는 반드시 출력 형식을 나타내는 method 속성을 선언해야 합
니다．
2. <xsl:apply-teniplates select="music" I>
다른 템플릿을 호출하는 것은 柚l:apply-templates> 요소입니다. select 속정이 <xs1:temp1冷
요소의 match 속성에 대응합니다．
3 match= "music"
위의 2와 관련지어 보면 간단합니다. match 속성과 select 속성을 착각하지 않도록 주의 바랍
니다．
4, <xsl = for-each select="musician·．>
Kmusician> 요소에 대해 반복 출력을 하고 싶은 경우, 鈿l:for-each) 요소를 사용해 이와 같이 작
성합니다．
F <xsl:sort select="@birth" data-type="text" order="ascending" I>
birth 속성을 기준으로 오름차순 정렬됩니다. <xsl:for-each) 요소의 출력을 제어하는 것은
仕sl:sort> 요소입니다．

===== PAGE 292 =====
291 =====
실력 테스트 해답

L. <xsl:value-of select= "@name" I>
鈿1:for-each) 요소의 현재 노드는 <musician> 요소로 name 속성으로 액세스하는 경우에도 단
순히 속정 이름만을 기술하면 됩니다．

〔 Lesson 5 ;
address. xml, address. xsl
1. <?xinl-stylesheet type=,text/xsl·· href= ·．address . xsl,, ?>
XML문서와XSLT스타일 시트를 연결시키려면 <?xm1-stylesht?> 명령을 이용합니다．
2. select= "addressBook/xnernber"
<xsl:for-each> 요소의 위치에서 현재 노드는 경로 요소
（/）입니다. <member> 요소를 나타내기 위
해서는 addressBook/member라고 기술해야 합니다．
3. <xsl:sort select="old" data-type="nuinber" order="ascending" I>
<old> 요소를 기준으로 오름차순 정렬됩니다. 楓d) 요소는 값 데이터이므로 data-切e 속성은반
드시 number로 지정해야합니다．
4. ="nowrap'
XSLT도 역시 XML 문서입니다. 속성값을 생략한 <m nowrap）
과 같은 표현을 이용할수는 없습니
다. 반드시 속성값까지 포함된 완전한문장으로 작성해야 합니다．
mailto:<xsl:value-of select="email" I>
본문에서 소개한 링크 연결을 응용했습니다. 메일 주소의 경우, href속성값에 'rnaflto:' 라는 문자
열을 기술해야 합니다．

article. xml, table. xsl
] . match=./.
XSLT 스타일 시트에 반드시 경로 요소에 적용되는 템플릿이 필요합니다. 경로 요소는 7' 로 나타
납니다．

0

===== PAGE 293 =====
292 =====
2 match= "article "
에 대응하여 호출된 템플릿입니다. 기사목록의 반복되는
Kxsl:apply-templates se1ect="article" I〉
부분을 출력합니다. select 속성과 match 속성을 혼동하지 않도록 주의하십시오. 호출한
柚1:app1y-temp1ate> 요소쪽은상대편을 선택하는 것으로 (select), 불려나온 <xsl:template>-소
는 이것을받아매치하는 것
（match）
으로 기억하시기 바랍니다．
3. i/ chapter I i/ section
은 XSLT에 익숙
（반대로 말하면 (3）
여기를 이해할 수 있다면 다른 문장은 쉽게 이해할 수 있습니다
하지 않으면 상당히 어려울 것입니디）
.
XML 문서 내의 전체 <chapter> <section> 요소를 대상으로 반복 처리를 실행합니다. 두 개의 대상
을 결합하려면 연산자 KUnion）
을사용합니다．
4. multiple
형제 요소에 대해서 넘버링하고 동시에 부모 노드 단위의 넘버링을 부가할 경우 level 속성에
multiple을 지정합니다. 그 외에도 single, any 등의 지정이 있습니다만 이 경우 어떠한 작동을 하
는지 실제 실행해 보기 바랍니다．
5 chapterlsection
count 속성은 어느 단위로 넘버링할지를 정하기 위한속정입니다. 이번에는 <chapter>, <section>

7

Lesson

(

요소에 대해서 넘버링을합니다．

】·느
：

article. xml, table. xsl
1. <xsl=output method= 'html. encoding= '~EUC-KR" />
제 2일의 복습입니다. XSLT 스타일 시트에서는 우선 출력 형식과 문자 코드를 <xsl:output> 요소
로 선언합니다．
2. xsl:if
단순한분기는 <xsl:if> 요소로 나타냅니다．
3. name(

)!='chapter ' 혹은 name(

)='section'

처리 중 요소가 <section> 요소인 경우 chr속성값을 표시합니다.test 속정으로 지정된 조건식은
'<ection> 요소인경우 두가지로나타낼수있습니다．
'<chapter＞요소가아닌경우 , s

0

===== PAGE 294 =====
293 =====
실력 테스트 해답

4, format-number (number (@chr) . ,#.＃料· )
수치를자리 구분 기호를 포함해 표시할 경우 format-number 함수를 사용합니다．

( Lesson 8
books. xml, books. xsl, books.css
`

books/book (contains (name, !ASP. )]
출력하는 요소를 압축해 넣는 경우에는[］로 필터 패턴을 이용합니다. 필터 패턴이 true인 요소만
이 최종적으로 출력됩니다. 이 경우 <name) 요소에 문자열 'ASP 를 포함하는 <book) 요소만 출
력합니다. 현재 노드가루트 요소이므로 경로를 <books> 요소에서 기술해야만 합니다．

I

<xsi=sort select="pDate" data-type=·，text" order= "descending" />
<pDate> 속성에 대해서 내림차순으로 정렬합니다．
substring-after (@isbn, ' ISBN' )
isbn 속성에 포함되는 맨 처음 문자열 ISBN만을 제거합니다. 몇 가지의 방법이 있겠지만
substring-after 함수를 이용해 ISBN으로 문자열을 구분한 뒤 다음 부분의 문자열만을 추출하는
것이 가장 일반적인방법입니다．
그 외에 substririg 함수를 이용해 'ubsthng(@isbn,5,20Y 과 같이 작성할 수 있습니다. 세 번째
인수인 20은 ISBN속성으로 취할수 있는 최대 자릿수를 정의하고 있습니다. substring 함수에 있
어 추출해야만 하는 자릿수가 대상 문자 수를 초과하는 경우에는 시작 위치에서 해당 문자를 검색
합니다. 미리 최대 자릿수가 설정되어 있으면 이 방법도 가능합니다．
substring(name, 1,7)
substring 함수는 (name> 요소의 첫째 자리에서 7문자를추출합니다．

5. sum(books/book[contains (name, ,ASP· )]/price)
sum 함수로 합계 값은구합니다．
본문을응용한부분입니다. 단, 이번에는 표 자체를 '타이틀에 ASP를포함하는 것"으로 한정하고
있으므로 여기에서도 똑같은 조건으로 압축해 둘 필요가 있습니다. 이와 같이 도중에 필터 패턴[]
을 기술할수도 있습니다.

===== PAGE 295 =====
294 =====
books.xml, books.xsl, books.css, inc.xsl
1. <xsl= decimal-format NaN='불명" />
수치 정보가 존재하지 않는 경우 鈿1:decimal-format) 요소의 NaN 속정을 사용합니다. 본문 예
제에서 속성값 부분을 변경만 하면 됩니다．
2. xsl:attrjbute-set
속성 세트를 정의하려면 鈿l:attnbute-set> 요소를 사용합니다．
3 , xsl: use-attribute-sets= " tblAtt "

선언된 속성 이름을 참조하려면 xsl:use-attribute-sets 속정을 사용합니다．
4. <xsi:include href= "inc.xsl">
외부의 XSLT 스타일 시트 inc.xsl을 사용합니다．

/

.

』＾`

`

( Lesson TU

4

.rticIe.html, table.xsl
<html>
<head>
<title> 5-l . 연습문제＜/title>
<script langiiage="JavaScript">
<!-

-

var objDoc=new Activexob」
ec니 Msxinl2 . DONDocument " ) '
objDoc . async=false;
objDoc.load( "table.xsl") ;
window.alert (objDoc.」anl) ;
II- ->
<Iscript>
</head>
<body>
<hl>5-l . 연습문제＜/hl>
</bady>
</ht1n그＞

===== PAGE 296 =====
295 =====
실력 테스트 해답

본문의 예제과다른 점은불러낸 대상이 XML 문서가 아니라XSLT 스타일 시트라는 것뿐입니다．
XML 문서를 호출하는 법은 알지만 XSLT 스타일 시트 호출 방법을 모르는 분은 이 예제를 통해 XSL
T스타일 시트도 XML 구문 규칙에 준해서 기술된 XML 문서라는 것을 알게 될 것이고, 본문 예제의
load 메소드의 인수 부분만을바꿔 써주면 되는 것임을 알수 있을 것입니다．

report. xml, sict.htm'
new Act iveXObj ect ( "Msxml2 . DOMDocument");
앞의 Lesson의 복습입니다. XML 문서를 불러내기 위해서는 문서를 저장하는 XML
D0MDocument2 오브젝트를 미리 생성해 둘 필요가 있습니다．
false
XIvTh문서 호출시 보통async 프로퍼티를fats로 설정합니다. 디폴트상태에서 async 프로퍼티는
true로 되어 있어 서버에서 XML문서를불러내는 경우 에러가발생합니다．
"report . mi1"
load 메소드의 인수로서 불러낸 XML 문서의 파일 이름
（경로）
을 지정합니다．
4, documentElement
DOM에서 XML 문서로 액세스할 경우 기점이 되는 것은 XSLT와 같은 경로요소입니다．
documentElement 프로퍼티는 경로요소를 취득합니다．
이것은다음 코드의 생략 형식입니다．
var clnDsc=bojHdr.childNodes;
var objCrt=clnDac . item(1) '

JavaScript에서는 이와 같이 프로퍼티나 메소드의 되돌아오는 값을 전제로 복수의 프로퍼티, 메소
드를합하여 하나로 만들수 있습니다．
O1eader> 요소의 두 번째 자식 요소 <creator> 요소를 취득하고 싶으므로 item 메소드의 인수로는
1을 설정합니다．

===== PAGE 297 =====
296 =====
6. text
노드 산하에 포함되는 텍스트를 취득하려면 text 프로퍼티를 사용합니다. XML 형식 (<creator〉김
미정＜/creator〉와겉끼）
으로 노드를 그대로돌려주는 xml 프로퍼티와는 구분해서 기억합시다．

(Lesson

12:
answerl.html, answer2.html, answer3.html

해답 예를 들어 보겠습니다. 사람에 따라 기술 방법은 다르겠지만 본문에서 다루고 싶은 몇 개의 메소
드를 적극적으로 사용해 봅시다．
answerl.html
<html>
<head>
<title> 5-3 . 연습문제＜Ititle>
<script language=nJavaScript '>
var objDcc =new ActiveXObject《 'Ms,cn12 . DOX1Documen" 》'
objDoc . async=false;
objDoc.load( "books.xml") ;
var objRoct=objDcc . docuxnentElement;
var clnCld=objRoot .childNodes;
var objNod=clnCld.item(0) ;
var clnAtr=objNod.attributes;
var objAtr=clnAtr.item(0) ;
window.alert (objAtr . text) ;
'I-

-

>

<Iscript>
</head>
<body>
<hl>5-3 . 연습문제＜/h1>
</body>
</html>

===== PAGE 298 =====
297 =====
I

I
I

실력 테스트 해답

answer2.html
<html>
<head>
<title> 5-3 . 연습문제＜/title>
<script language="JavaScript">
<!

-

-

var objDoc=new ActiveXObject ( "4sxml2 .DOMDocument ' ) ;
objDoc . async=false;
objDoc.load( "books.xml") ;
var objRoot=objDoc .documentElement;
var clnCld=objRoot .childNodes;
var objNod=clnCld.item(0) ;
var objAtr=objNod.getAttributeNode ( 'address' ) ;
window. alert (objAtr. text) ;
II- ->
</script>
</head>
<body>
<hl>5-3 . 연습문제＜/hl>
</body>
</html>

answer3.html
<html>
<head>
<title> 5-3 . 연습문제＜/title>
<script language= 'JavaScript">
<!

-

-

var objDocrnew ActiveXObject ( "Ms,an12 .DOMDocument") ;
objDoc .async=false;
objDoc.load( "books.xml' ) ;
var objRoot=objDoc .documentElement;
var clnCld=objRoot. childNodes;
var objNod=clnCld.item(0) ;

===== PAGE 299 =====
298 =====
window.alert(objNod.getAttribute( "address"));
II-->
</script>
</head>
<bOdy>
<hl>5-3.연습문제＜/hl>
</body>
</html>

이번에는 본문에서 소개한 getElementsByTagName 메소드로 매긱 놓을수 없습니다. 만일 10행째를
아래와 같이 바꾼 경우，
var c1nVa1=objDoc. getE1ementsByTagName ( "@se1ect ") ;

어느 정도의 결과는 기대할수는 있지만 柚l:value-of) 요소에 속하는 다른 select 속성값도 추출되어
버립니다．

r Lescon 14`
sort.html
<html>
<head>
<title> 6-2 . 연습문제＜/title>
</head>
<script language="JavaScript ">
<므

-

-

var objDoc=new ActiveXObject ( "Msxml2 .DO11Document") ;
O1功Doc .async=false;
objDoc.load( "books.xsl ") ;
var objRoot=objDoc .documentElenient;
var objSort=objDoc .selectSingleNode ( "I/ xsl :sort") ;
var objSrt=objDoc.createEleinent ( "xsl: sort") ;
objSrt.setAttribute( " select", "price") ;
objSrt. setAttribute( 'data-type ', 'number") ;
obj Srt . setAttribute ( "order' , "ascending") ;

===== PAGE 300 =====
299 =====
실력 테스트 해답

objSort .parentNode. insertBefore(objSrt,objSort) ;
window.alert (objDoc.xml) ;
II- ->
<Iscript>
<body>
<hl>6-2 . 연습문제＜/h1>
</body>
</html>

<xsl:sort) 요소는 배치 순서대로 의미가 있습니다. 제1키를 추가하고 싶은 경우에 <xs1:sort> 소의 첫
번째에 작성합니다．
이와 같이 특정 장소에 요소를 추가하고 싶은 경우에는 insertBefore 메소드가 유효합니다. 또
insertBefoi℃의 제2인수
（삽입 장소）
는selectSingleNode 메소드를사용합니다．
insertBefoi℃ 메소드의 기초가 되는 오브젝트는 <xsl:sort) 요소의 부모 요소인 鈿l:for-each〉요소이
지만 이것은 삽입 장소의 부모 요소로 미리 구해져 있는 objSort에서 parentNode 메소드를 사용해 추
출하는 것입니다. 물론 selectNodes(selectSingleNode) 메소드로 다시 추출해도 상관없지만
parentNode 메소드를흔히 사용합니다．

15〕

Lesson

(

sort.html
<ht그汕．
>
<head>
<title> 6-3 . 연습문제＜/title>
</head>
<script 1anguage="JavaScript">
<!

-

-

var objDoc=new ActiveXObject ( "Msxm12 . flOMDocumerit '! ) ;
objDoc . async=false;
objDoc.load( "books.xsl ") ;
var objRoot =objDoc.documentElement;
var objEch=objDoc.selectSingleNode
( "xsl : stylesheet/xsl :teinplate/xsl: for-each' ) ;
var objSrt=ob」
Dcc . createElement《 "xsl: sort" ) '

===== PAGE 301 =====
300 =====
objSrt.setAttribute( " select " ; "price" )'
objSrt.setAttribute("data-type" ' "number" 》;
objSrt . setAttribute( "order", "ascending") ;
objEch.replaceChild(objSrt, objEch.childNodes. item(O) );
objEch.removechild(objEch.childNodes.item(l) );
window.alert (objDoc .xml) ;
II- ->
</script>
<body>
<hl>6-3 . 연습문제＜/hl>
</body>
</html>

두 가지의 鈿1:sort> 요소가 조작 대상이 됩니다．
예제에서 대상 노드의 추출은 selectSingleNode 메소드에서 실행하며 여기에서는 <xsl:sort〉요소의 부
모 요소인 鈿l:for-each> 요소를 추출합니다. 물론 맨 처음의 柚1:sort> 요소를 추출해 nextSibling
프로퍼티에서 다음 요소를 추출하거나 혹은 2회 selectSingleNode 메소드를 실행하는 등 방법은 여러
가지 있을 것입니다．
요소 자체의 바꿔 놓기는 본문에서도 소개한 replaceChild 메소드를 사용합니다. 물론 removeChild
메소드를 사용해 요소를 삭제한다음 insertBefore 메소드에서 요소를 추가해도 상관없습니다．

( Lesson 16
music.xml
<?xml version="l. O " encoding= "EUC-KR" ?>
'dDOCTYPE music [.
< !ELEMENT music (musician+ ) >
< !ELEMEN'T musician EMPTY>
< !APPLIST musician name CDATA #REQUIRED
category CDATA #IMPLIED
birth

CDATA #IMPLIED

country （프랑스 - 독일 - 폴란드） '' 독일''

1>

imp_work CDATA #REQtJIRED>

＜끄ruS1C>

===== PAGE 302 =====
301 =====
I

I

실력 테스트 해답

<musician name= “클로드 드뷔시“ category=" 인상파" birth="1862-08-22 "
country=“프랑스” im乙work=" 월광“ />
<musician name= “요한 세바스찬 바하” category= " 바로크“ birth="1658-03-21"
country=" 독일“ imp_work= "푸가 b단조“ />
<musician riame='’루드비히 반 베토벤’' category='' 고전파” birth= "1770-12-16"
countryr”독일“ imp_work= "교향곡 제 5번 운명" />
<musician naxne= ”후리데릭 쇼팽" category= " 낭만파” birth="1810-02-22 "
country=“폴란드” ixnp_work=“환상 즉흥곡” />
<musician name='’모리스 라벨’' category= ”근현대’ birth="1875-03-07 "
country= ”프랑스" imp work=" 볼레로" />
</1mlBic>

…

…긍＝∥∼쑈르샀m

문제 문장에 기술된 각 조건을Un）
의 각 키워드 기호로 변경하면 됩니다. < nusiciai分요소의 구성요소
는 EMP1,Y라고 합니다．

(Lesson 17 address. xml, addressl- 5. xml, address.dtd
address.xml
<?xmi version="l. 0" encoding= "EUC-KR" ?>
< !DOC1'YPE addressBook SYSTEM "address.dtd"
< !ELE4}i;NT addressl SYSTEM "address1. oa1" >
< !FTF:MENT address2 SYSTEM "address2.,anl" >
< !ELEMENT address3 SYSTEM '1address3 . xm1H >
< LETEMENT address4 SYSTEM "address4. cn1" >
< !ELEMENT address5 SYSTEM "adc3ress5.xmJ. " >
1>
<addressBook>
&addressl;
&address2;
&address3;
&address4;
&address5;
</addressBook>

[

===== PAGE 303 =====
302 =====
addresstxml
<?xml version="l.0" encoding= " EUC-KR" ?>
.zmember id='00003'>
<name> 김미정＜/name>
<email>kongkong(?youngjin. com</exnail>
<address＞서울시 강남구 논현동＝/address>
<old>25</old>
</member>

※address2∼5.xm1은똑같은구성이므로생략합니다
address.dtd
< 』EL때El寸T addressBook (member) '>
< 뜨EL때皿，
1
'r member (name,email,address,old) >
< ! ELEMENT name (#PCDATA) >
< 그ELEMENT email (#PCDATA) >
< 므EL皿4ENT address (#PCDATA) >
< ! ELEMEN'I` old (#PCDATA) >
< 』ATmLIsT member id ID #REQUIRED>

이번에는문제에서 조건으로 요소, 속성을 외부 서브 세트로, 실체를 내부 서브 세트로 각각 선언하도
록 지정하였으므로 해답과 같은 파일 구성으로 되어있지만 실제로는 요소, 속성을 내부 서브 세트에，
실체를 외부 서브 세트에 기술할 수도 있습니다. 외부 서브 세트인지 내부 서브 세트의 결정 여부는 그
것이 여러 파일에 공통적으로 선언되는지, 개개의 파일에만 선언되는지의 차이뿐입니다．
외부 실쳬 참조에서 인용되는 낱낱의 외부 파일은 반드시 XML 선언을 기술해야 합니다. 문자 코드의
선언이 없는 경우디폴트인UTF-8로 간주되어 버려 정상적으로 읽히지 않는 경우가 있습니다．

===== PAGE 304 =====
303 =====
실력 테스트 해답

(1三sson可
address.xsd
<?xml version="l. 0 " encoding= "EUC-KR" ?>
<xsd:schexna xmlns:xsd="http: //www.w3.org/2001/XMLSchema">
<xsd: element name= "addressBook">
<xsd: complexType>
<xsd: sequence>
<xsd: element namer "member"

type= "memberType"

minOccurs= " 0 " inaxOccurs= "unbounded'1 />
</xsd: sequence>
</xsd: complexType>
</xsd:element>
<xsd: complexType name= "me祉）
erType" >
<xsd: sequence>
<xsd:element name= "name" type="xsd: string" />
<xsd:element name="email" type="xsd:string" I>
<xsd:element namer "address" type="xsd: string" I>
<xsd:element name="old"
type= " xsd: nonNegativelnteger" />
<Ixsd: sequence>
<xsd:attribute name="id" type="xsd: string"use="required" I>
</xsd: complexType>
</xsd: schema>

… ∼＝…

(member〉요소의 형식은 별도로 정의하는 것이 아니라 <xsd:element name="member'〉요소에 기술
할수 있습니다. 그러나 필요 이상의 계층 구조가복잡해지면 소스도 난해해지므로 그리 권장하는 방법
은아닙니다．

===== PAGE 305 =====
304 =====
e

( Lesson 19

닢締JL·LH뻗

address.xsd
<?xml version="l. 0 " encoding= "EUC-KR" ?>
<xsd:schema cnlns:xsd="http: //www.w3.org/200l/)a':LSchema" >
<xsd:element namer "addressBook">
<xsd: comp1exType>
<xsd: sequence>
<xsd: element name= "meniber" type= "meniberType"
minOccurs="l " maxOccurs="unbounded" I>
</xsd: sequence>
<Ixsd: complexType>
</xsd: element>

<xsd:complexType name= "me祉）
er1,'pe">
<xsd: sequence>
<xsd:element name= "name" type="xsd:string" I>
<xsd:element name= "email">
<xsd: simpleType>
<xsd:restriction base= "xsd:string ">
<xsd:pattern value=" [\w\ .-] + (\ + [\w-] *)?@( [\w- J+\. )+ [\w-]+" I>
<Ixsd:restriction>
<Ixsd: simpleType>
</xsd: element>
<xsd:element name= "address">
<xsd: simplepype>
<xsd:restriction base= "xsd:string ">
<xsd:maxLength value="l00" I>
<xsd:minLength value="l0 " I>
</xsd:restriction>
</xsd: simpleType>
</xsd: element>
<xsd:element name= "old">
<xsd: simpleType>
<xsd:restriction base= "xsd:nonNegativelnteger">
<xsd:maxExclusive value="120 " I>
<xsd:ininExclusive value="l0 " />

===== PAGE 306 =====
305 =====
실력 테스트 해답

</xsd:restriction>
</xsd: simple叱＇pe>
</xsd: element>
</xsd: sequence>
<xsd:attribute naxne="id" type="xsd: string' use="required" I>
<Ixsd:complexTyps>
</xsd: schena>

<xsd:element name= "mexnber"

minOccurs="0"

type="mernberType"

maxOccurs= "unbounded" />

<Ixsd: sequence>
</xsd: complexType>
</xsd: element>
<xsd: complexType name= "mexberType">
<xsd: sequence>
<xsd:element name= "name" type="xsd:string" I>
<xsd:element neme="email" type= "xsd: string" />
<xsd:element name="address" type= "xsd: string" I>
<xsd:element name="old"
type="xsd:nonNegativelnteger" I>
<Ixsd: sequence>
<xsd:attribute name="id " type="xsd: string"

use="required" I>

</xsd:complexType>
<Ixsd: schema>

<xsd:restrictjon>요소는 복잡한 문서 형식 표현의 내용을 이해해야 합니다. 다시 한번 본문을 복습해
보기 바랍니다．

305

===== PAGE 307 =====
306 =====
validate.html
<html>
<head>
<title>XMI』 문서의 검증＜/title>
<script language="JavaScript ">
<!

-

-

function chk ( ) {
var objDoc=new ActiveXObject ( "MSxl4:L2 .DONDocument") ;
objDoc .async=false;
objDoc . loadXML (document. fm. strXNL.value) ;
var objErr=objDoc .parseError;
if (objErr.errorCode! =0) {
str=objErr.errorCode + " \r" '
str+=objErr.line + " 행" + objErr.srcText + " \r" '
str+=objErr.reason;
window.alert (str) ;
}else{
window.alert ( '' 올바른 xld＝』 문서입니다“ ) '

)
}
'I- >
-

</script>
</head>
<body>
<hl>xML 스키마에 의한 xMI』 문서의 검증＜Ih1>
<fonn name=" fm'>
<textarea rows= 1'10" cols=" 60 " name= "strXML"></textarea>
<If orm>

</body>
</html>

</xsd:complexType>

</xsd: element>

<xsd: complexType name= "memberType">

I>

<br I>
<input type="button" value="XML 문서 읽기“ onclick="chkO "

===== PAGE 308 =====
307 =====
실력 테스트 해답

<xsd: sequence>
<xsd:element name= "name" type="xsd:string " I>
<xsd:element name="email" type="xsd:string " I>
<xsd:element najne="address" type="xsd: string" I>
<xsd:element name= "old"
type="xsd:nonNegativelnteger" I>
</xsd = sequence>
<xsd:attribute name="id " type="xsd: string"

use="required" I>

</xsd: complexType>
</xsd: schema>

XMLSchema와의 관련짓기가 생략된 것뿐으로 본문 샘플과 거의 변한 점은 없습니다. JavaScript에
의한 텍스트 영역 처리에 관한 'document.fm.strXML.value' 의 문장이 사용됩니다．
이번에 사용한1oadXv1L 메소드는 새로운 명령이지만, 이후 문제 문장과 같은 형식에서 구문만 표시하
는 경우 점점 많이 등장할 것입니다．

qLesson 21:
books.xsl
<?xml version="l. O" encoding= "EUC-KR" ?>
<xsl: stylesheet xmlns:xsl="http: //www.w3 .org/1999/XSL/Trans
form" version="l. O ">
<xsl:output method= 'html" encoding= "EUC-KR" I>
<xsl : template match=" I ">
<html>
<head>
<title> <xsl:value-of select="books/@title" /></title>
<link rel= "stylesheet " type="text/ css" href="books.css" I>
<script language="JavaScript">
<! [CDAPA[
Document;
var objDoc=document . )ldI』
var objStl=document . XSLDocument;
var nodRow=obj Stl . selectSingleNode ( " //xsl : sort" ) '
function dispO{
key=document. forms [0] . srt . value;

307

===== PAGE 309 =====
308 =====
switch(key){
case "1":
tmpl="@isbn";
txnp2= "text";
break'
case "2":
tmpl="name";
tinp2="text";
break;
case "3":
tmpl="author";
tirip2= "text";
break;
case "4":
txnpl= "publish";
tmp2="text";
break;
case "5":
tmpl="price";
切
［p2= "nuxnber";
break;
case '1 6 1~=
tmpl="pDate";
tirip2="text ";
break;
}
nodRow.setAttribute ( " select" ,tmpl) ;
nodRow.setAttribute ( "data-type" ,tmp2) ;
nodRow. setAttribute( "order" ,document. forms [0] .ad.value) ;
dSrt . inrierHTML=objDoc . documentElement . transformNode(objStl) ;

}
1] >
</script>
</head>
<body onload="dispQ ">
<hl><xsl:value-of select= "books/@title" /><Ihl>
<div id="dSrt ">
<xsl :apply-templates select="books" I>

===== PAGE 310 =====
309 =====
I

<Idly>
<p>
<form>
소트키
<select neme="srt " onchange="disp() ">
<option value="l ">ISBN코드</optiori>
<option value="2">서적명</option>
<option va1ue="3">저 k/ option>
<option value="4 "＞출판사＜/option>
<option value="5" >가격</option>
<option value= "6" >발간일</option>
</select>
오름차순／내림차순
<select name="ad" onchange="disp() ">
<option value="ascending"＞오름차순＜/option>
<option value="descending"＞내림차순＜/option>
</select>

</p>

<Iform>
<div><xsl :value-of select= 1'books/owner' /></div>
</body>
<Ihtin1>
</xsl = template>
<xsl :template match="books " >
<table border="l ">
<tr>
<th>ISBN 쾨三</th>
<th＞서적＜/th>
<th＞저자＜/th>
<th＞출판사＜Ith>
<th＞가격＜/th>
<th＞발간일＜/th>
</tr>
<xsl:for-each select="book">
<xsl: sort select= "@isbn" data-type="text ' order=「ascending'

I>

I

실력 테스트 해답

<tr>
<td nowrap= "nowrap" ><xsl :value-of select= "@isbn" /></td>
<td nowrap="nowrap">

===== PAGE 311 =====
310 =====
<xsl:elexnent name="a">
<xsl:attribute name= "bref">
<xsl:value-of select="url" I>
</xsl:attribute>
<xsl:value-of select= "nanie" I>
</xsl:element>
</tㅍd>
<td nowrap="nowrap"><xsl :value-of select= "author" /></td>
<td nowrap= "nowrap"><xsl:value-of select="pi.thlish " /><Itd>
<td nowrap="nowrap">
<xsl : choose>
<xsl:when test="price[nuxnber(. )&lt; rlSOOO] ">
<span style="font-weight:bold; ">
<xsl:value-of select="price" I>원
</span>
</xsl :when>
<xsl:otherwise>
<xsl:value-of select="price" />원
</xsl : otherwise>
</xsl = choose>
</td>
<td nowrap="nowrap"><xsl:value-of select="pDate" /><Itd>
< /tr>
</xsl : for-each>
</table>
</xsl : template>
</xsl : stylesheet>

언뜻 보기에 어렵게 느껴질지도 모르겠지만 오름차순／내림차순의 선택 콤보 박스를 추가해 그 선택에
따라 order 속성을 변경하는 아래의한행을 추가만 했습니다．
nodRow. setAttribute ( "order" ,document. fonis[0) .ad.value) ;

정렬키의 콤보 박스를 변경해도 오름차순／내림차순의 콤보 박스를 변경해도 똑같이 공통해서 dip 함
수를 불러내고 있는 점에 주의해 주십시오．

===== PAGE 312 =====
311 =====
실력 테스트 해답

9?'

Lesson

(

res미t.js
function dispO{
var strPub=parent.up. fm.pub.vaiue;
var strKey=parent .up. fm.key.vaiue;
var strDat=parent .up. fm.pDat .value;
var objDoc=new ActiveXObject ( "Msxm12 .DOMDocument ");
objDoc .async=false;
objDoc.load( 'books.xmi") ;
flg=faise;
strFlt= ' fbooks/book ';
if (strPub!=" ' ) {
strFit+ ="[(pubiish =

" + strPub + " ' ) ";

flg=true;
)
if (strKey!= '" ") {
if (fig) {
strFit+ =' and ";
}eise{
strFi盼＝n〔 '1 '
fig=true;
}
strFit-i-=' (category ='「 + strKey + '" ) " '
}
if (strDat!=" ") {
if (fig) {
strFit+ = " and '1;
}else{
strFit+ =" [";
fig=true;
}
strFlt+ =" (pDate >=

+ strDat + " ' ) ' '

}
if (fig) {strFlt+="] "} ;
var cinNod=objDoc.seiectNodes (strFit) ;
with(parent.down. document) {

===== PAGE 313 =====
312 =====
open("text/htinl");
writeln( "<htxn1><head><title>검색 결과＜/title> ") ;

)

"

writeln ( "<link
I>

rel= \"stylesheet\ "

type= \"text/css\ " href= \"books.css\ "

;
writeln ( "</head><body>") ;
writeln ( "<table border= 'l '><tr>") ;
writeln ( "<tr><th>ISBN 코드</th><th>책</th><th>저자＜/th>") ;
writeln ( "<th＞출판사＜/ th><th＞가격＜/th><th>발행일＜/th></tr>" ) '
for(i=O;i<clnNod.length;i++) {
objNod=clnNod.item( i ) '
objlsb=objNod.selectSingleNode( "@isbn") ;
objNam=objNod. selectSingleNode( "name") ;
objAut=objNod. selectSingleNode ( "author") ;
objPub=objNod. selectSingleNode ( "publish") ;
objPrc=objNod. selectSingleNode ( "price") ;
objDat=objNod.selectSingleNode ( "pDate") ;
writeln ( "<tr>") ;
writeln ( "<td>" + objlsb.text + "</td> " ) '
writeln ( "<td>" + objNam. text + "<ltd>'1 ) '
writeln ( ".<td>" + objAut.text + " </ tㅍd> " ) '
writeln ( "<td>" + objPub.text + " </td>" ) ;
writeln ( "<td>" + objPrc.text + " 원＜/td>" ) '
writeln ( "<td>" + objDat.text + "</ tㅍd>" ) '
writeln ( "</tr>") ;
}
writeln ( "</table></body></html>") ;
close 0;

기본적으로는 후반의 장황한 출력 부분을 바꿔 써넣는 것만으로 끝나기 때문에 입력 실수 등만 하지 않
으면 겉보기의 복잡함과는 달리 그렇게 어려운 문제는 아닐 것입니다. 반대로 갈피를 못 잡겠는 분은
（경우에 따라서는 제 5일∼제 6일의 레슨：을재차 검토해 봅시다．
다시 한번본문의 내용

小

===== PAGE 314 =====
313 =====
실력 테스트 해답

trans.asp

<%

<%&Language= "JavaScriPt" %>

var objDoc=new ActiveXOb」
ect ( "MSXML2 . DONDocument "' ) '
objDoc . async= false;
ob」
Doc . load(Server.MapPath( "books.,cal" ) ) '
var objStl=new ActiveXObject ( "MSxl兀2 . FreeThreadedDO4ocument '' ) '
obj Stl .async=false;
objStl. load(Server.NapPath( "books.xsl ") );
var objSrt=objStl . selectSingleNode( "/ /xsl: sort") ;
objSrt.setAttribute ( "select", "author") ;
objSrt.setAttribute( "data-type' , 'text ' ) ;
objSrt . setAttribute( "order", "ascending") ;
var objTmp=new ActiveXObject ( "MSXML2 .XSLTeniplate" ) ;
objTmp. stylesheet=objStl;
var objPrc=objTmp.createprocessorO;
objPrc. input=objDoc;
objPrc . transform( ) ;
Response . Write (objPrc . output) '
,>

이번에는 불러낸 XSLT 스타일 시트를 그대로 사용하는 것이 아니라 <xsl:sort＞요소의 속성값을 변경하
여 정렬키를 변경합니다. 정렬키의 변경은J￡ son 14를참고하기 바랍니다．
selectSingleNode 메소드는 인수로 지정된 xPath식에 매치한 노드를단 한 개만 얻습니다. 인수로 지
정된 "//xsl:sort"는 도큐먼트에 속하는 모든 <xsl:sort〉요소에 매치합니다. 이 경우 XSLT 스타일 시트
안에 柚Rsort〉요소는 두 개 존재하지만 자동적으로 맨 처음 기술된
（첫번째 키）<xs1:sort＞요소를 구하
거］됩니다．
구한 物1:sort）
요소에 대해서는 setAttrihute 메소드를 이용해 각각 select 속성, data-type 속성，
order속성을다시 설정하며 출력시 <author〉요소를 키로사용해서 실행합니다．
이것을 응용하면 클라이언트 측에서 정렬키를 받아 소트 패턴을 변경하는 제 9일 Lesson21의 서버 버
전도 작성할수 있을 것입니다．

小

===== PAGE 315 =====
314 =====
K.

`

LeSSflfl / 4
-

1. objDoc.transformNode(objStl)
Lesson 21에서도 소개한 방법입니다. 이와 긷히 서버 중심에서도 trarisformNode 메소드를 사용
할수 있습니다．
2. text
이번 XSLT 스타일 시트에 의한 출력은 이제까지와 겉끼 HFML이 아니라 텍스트입니다. XSLT는
반드시 XML 문서를 FYFML로만 변환하는 것은 아닙니다. 텍ㅅㅌ쿠두 변환이 가능합니다．
r
그 외에 xTh에서 별도의 형식인 xll로 변환하는 경우도 있는데 그 경우 method 속성은 'xn〕
이 됩니다．
3. 1 （세로의 곧은선）
에 대해서 처리할 경우, 두 가지의 xPath식을
@*（속성군 모두）혹은 node()（자식 요소군 모두）
로 연결합니다. 이것에 의해 각각의 조건에 일치한노드를 결합한후에 추출합니다.
mJnion : 결힙〕
4. \name( )
현재의 요소, 속성의 노드 이름을 반환하는 것이 xPath로 정의된 name 함수입니다. 덧붙여 말하
면이름 공간을뺀로컬 이름만을 구하고 싶은 경우에는 local-name 함수를 사용합니다．
5. . （마침표）
현재의 요소, 속성의 값을취득하는것이므로 '.' 를지정합니다．

小

===== PAGE 316 =====
315 =====
A
add
addr
align
ANY
appendChild
apd叫emplates
sp 파일
async
attributes
author Type

229
125, 215
228
215

198
253
125
215
150
100
124
124
178
178
178
178
177
179
179

聊

C
CDATA
CDATA 섹션
ceiling
century
childNodes
comment()
concat
contatins
createAttribute
createCDATASecfion
createComment
createDocumentFragment
createElement
createEntityReference
createProcessinginstruction
CreateTextFile

輛

B
t inaw
bookAttr
boolean
border
b4e

帥 ∥ 棚 姚 仙 昭 曲 佈 硼棚

106, 110
136
118, 126, 127
100

(xsl:variable>
(xsl:when>
?xml?
@:
加

m佈셰쌥佈昭m

81, 112
150
121
134
99
98
111, 123
126

m湘,이

252
232
232
233
232
232

准 驟 宬 狂 棚 棚 m 姚 姚 姚 姚 楔拙 沔 佐

기호／숫자
(script)
(xsdencoding>
(xsd:lengttt) sd:lisf)
Kxsd:max[xclusive>
(xsd:maxLengtt
<xsd:maxlnclusive>
(xsd:minExclusive>
t)sd:minincIus\/e>
(xsd:minLengtf心
6<Sd:precisior
t) sd:scale>
<%@Language %>
#RXED
#IMPUED
#PCDATA
#REQUIRED
＄변수명
(![CDATAE'-]I>
(Jscript>
(?xml-stylesheet?>
(a>
(author>
(boo◇
(category>
(keyword) 요소
(logo) 요소
(price>
(publish>
(ret>
(script>
daue＞태그
(unl>
(xsl:attiibute-se0
(xsl:attribute>
(xsl:choose>
(xsl:it>
(xsl:include>
(xsl:message>
(xsl:number>

createTextNode
creatProcessor
cSS 스타일 사트
CSS(Cascading St4e Sheet)
CSV(Comma Separated Value)
current

179
273
68
12, 73
15, 279
126

73
data-type
215
date
215
decimal
123 143
Document4.0
documentEtement
150
DOM(Document Object Model)14, 140,143
150
DOM 조작
D아d 프로그램
261
215
double
DTD(문서 형식 선언）
190, 193
E
element-avaliabl
EMP1Y
encoding
ENTI11ES
ENTiTY
enumeration
errorCode
EUC-KR

126
195
35
198
198, 215
198
245
35. 59

F
talse
tilepos
FileSystem 야)ject
firstChild
firstName
tloat
tloor
FO(Forrnatting Objects)
format 속성
format-number
Free-Thereaded

125
245
28o
152
44
215
125
13, 74
100
106, 126 ,
272

===== PAGE 317 =====
316 =====
G

getAtnibute
getAttributeNode
getElementsBylagName
getNamedltem
getOualitiedltem

126

MSXML3
MSXML4

21
14.3, 240

162
162
169
161
161

N
name
narnespaceURt
NaN
NCN.4ME
negativehteger
nextSibling
NMTOKEN
NMTOKENS
node()
nonNegativelnteger
nonPositivelnteger
normalize-space
not
NOTATiON
nowrap
null
number

123, 215
123, 170
135
215
215
152
198, 215
198, 215
100
215
215
124
125
215
40
152
125

H
hasChildNodes
170
height
134
hret
56
I-ffML(l-lyperText Markup Language) 10

1

o

臘 加 佃 獅

加 聊 刀 聊

ID
198, 215, 228
IDREF
198, 215
IDREFS
198, 215
innerl-ITML
input
insertBetore
integer
isbn(lnternetional Standard
Bo아
（ Number)
34, 160
item
151

125
123
44
151
100
245
73
145, 146
246
123
215

P
parentNode
position
P05如7터nteger
previousSibling
processing-instruction()
P4IS(Personsi Web Server)

153
123
215
153
100
270

Q
다NLAME

215

P
69
218
98
218
215
154

RDB(Retational DataBase)
reason
removeAttribute
removeAttributeNode
removeChild
removeNamedltem
removeoualifieditem

4

化 師 衢 佈 侮 佈 溺

『n
match
maxOccurs
memo
minOccurs
month
MSXML 파서

S
save
schemas
sded
selectNodes
selectSingleNode
setAttribute
setNamedftem
SGML(Standard Generatzed
Markup Language)
short
src 속성
srcText
standalone
start-with
string
strin어ength
substring
sum 함수
system-property
td

187
244
60
169
169
179
180
12
215
98
245
36
124
124. 215
124
124
118, 125
126
40

T

L
lang
last
lastName
length
level 속성
line
link
bad
ba<1XML
bc눼 'ame
long

Rental-Thereaded
replaceChild
required
round

耽 佈 駟 仍

function-available

TDV(Tab Deitmited Value)
terminate
TextStream
time
timeDuration
Transformations
transtormNode
true
type

15
126
280
216
216
58
254
125
56, 219

U
Unicode
unsignedByte
unsignedlnt
unsignedLong
unsignedShort
uriReterence
un1
um:books

35, 36
216
216
216
216
216
245
244

===== PAGE 318 =====
317 =====
35
35

Valid
Valid XML
version

194
17
35

w

고정값
공요소
공유
-77 E
C〕
.

x

187
198

라
레이아웃
루프
리플레이스 모드
링크
링크생성

193
282
24
111
97

oF
마크업
메타 기술 언어
목록표
목적 노드
문자 데이터
문자코드
문자열 함수
문장 장식

帖

쾌
雄酬
竭뜨

羽ㅆ 准 咫

4

195, 218

71
133
217
37, 153
263
13, 177
126
97
263

분기 여부
분산
불량 데이터
블록 단위
비교 연산자
비교식
비동기
비정형
비정형 문서
사硼玔韶쌔桭洲胛姆쇄一솨如쇄如

다
다이내믹
단순 형식 요소
단순한 계산 기능
단순한요소
대문자
데이터베이스
동시 엑서스
동일 겨隱
동일 형식
《겨쓰기
들
등장
등장

반복 출력
변수
복잡 형식 요소
부모 요소

出 昉 弱 韶

내림ㅊ隆
내부 서브 세트
내부 실체 참조
내부 텍스트
내포
노드
노드 설정 함수
노드 정보
논al식
논리 연산자

弱 게 mㅄ 羽姚 m 弱 聊 巧加 碼

216

98
81, 82
229
217
15
195

디스크
디폴트

바
나

羽釧辨

V

관계
구조적인 XML 문서
굵은글씨
그룹화
기본 데이터 형식
기술 연동
기호군

兀 姚 刪 棚 羽弱m m 田 拙

XML(eXtensible Markup Language)10, 44
XMWOM SchemaCache
243
XML 스키마
17, 210, 213
XML 파서
16
XMLDOMDocument2
145
XMLDOMNamedNodeMap
160
XMLDOMNode
150
XMWOMNodeList
150
xmlns:xsd
214
xPath
61, 100
xPam 함수
118
xsd:complexType
216
xsd:enumeration
230
232
xsd:pattern
xsd:restnction
217, 230
xsd:schema
214
XSL(eXtensible Slylesheet Language) 13
xsl:apply-templates
69
xsl:attnbute
82
xsl:element
82
xsl:tor-each
66,71, 72
xsl:output
58. 59
xsl:sort
81
xsl:template
98
xsl:text
60
xsl:value-of
60, 61, 100
XSLProcessor
273
XSLT 함수
69, 9익 123
273
XSLTemplate

year

개별 템플릿
검색 조건
검색키
검증
경로요소
겨隱 구조

85
168
69
261
262
244
36, 58, 150
46, 110, 180
232
38, 121, 126
273
204
261

昉 促 朗 沁 % 弱 田 髓

W3C(Worid Wide Web Consortium) 13, 74
Well-formed
16, 194
width
134

가
긴략형
개별 노드

===== PAGE 319 =====
318 =====
160, 197
134

속성값
손요소

수치 정형
수치 함수
수학식
스크립트
시간 지연
시작 태그

애매한 요소
엄격화
에러 정보

차
처리 명령
최상튀 요소
출력 방법
출력 순서
출력 장소
치환
친자 관계

ㅈ
＜ --

타
타이틀 행
태그 세트

탭
탭문자
템플릿

282
252
268
11
쩨 泛 股刪

인용

집중

ㅂ

인스톨러

170
92
60,83
151
194
21
229

줄바꿈 문자
중성적
직접 잡근
진위 함수

。
，
7

인덱스 수
인스턴스

20, 57, 214

주석
주석문
주체
줄ㅂ곰

口 토 ㄹ
＝
ㄷ 조
ㄷ 쿠

원형
의미 단위
이름 공간
이름 공간 접두사
이미지 표시
아스케이프

정형
제 1요소
제약 조건
조건 분기
종료 태그

／
ㅢ

외부 XSLT
요소
요소 노드
요소 주체
요소 추출

정렬
정보 가술 언어

泌 兀貂 刀 聊 溺 巧

외부 미D

砥

옵션
옵션 후보
와부 사브 세트
외부 실체 참조
와부 프로그램

73, 252

羽 ∥ 加 饌 吼 批 m 拙 冊 ㅆ硼 碑 咫 加 m

연결
예약 문자
오름차순
오버랩
오브젝트 모음

파

재귀적
접근
접두사
정규표현

57, 69, 97

파일 패턴
퍼스널 웹 서버
퍼포먼스
팡균값
평문
표제어
표현 패턴
필터 패턴

하
현재 노드
현재 요소
현재 폴더
호환성
홈 폴더
확장성

70
60, 153

恥 弱 끼 巧

勿 羽臨 弱田

아

자속성
자식 요소

曖

실용적
실체 참조
쌍따옴표

트리 구조
특수 문자
특수 키워드

田 刪 m m 化 羽 囹 胛

수치 데이터
수치 정렬

자
자바 기반

囹 刀 沁 昉弱 狂佈 釘 邸 嫡 聊 쩨 批 巧 個 m氾

棚 弱 m 히 姚 棚 羽 凝 孀 釘 m 獅 羽

속성 리스트
속성 세트

