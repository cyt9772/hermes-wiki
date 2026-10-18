---
title: XML for the World Wide Web: Visual QuickStart Guide (raw source)
source_url: /run/media/yutae/Data/XML_For_WWW.pdf
ingested: 2026-10-18
sha256: 5c1fdf58761774d955b69001d34d10bc4ab897c438908313c563b511c02db0d0
---

# XML for the World Wide Web: Visual QuickStart Guide (raw source)

> **Note:** PDF 내장 텍스트 레이어 사용 (OCR 없음). `pdftotext` 추출. PDF는 로컬 참조용 (`raw/books/*.pdf` git-ignored).

## Book metadata
- **원저:** Elizabeth Castro, Peachpit Press (Addison Wesley Longman) 2001
- **한국어판:** B&B (한국저작권센터 KCC 통해 계약) — Peachpit Press 저작권 계약
- **범위:** 253p, Part 1~6: HTML의 한계→XML 기초 → 요소/속성 → DTD(엔티티·단축형) → 이름공간/XML Schema → CSS → XLink/XPointer
- **page count:** 253 (pdfinfo Pages)

## 장 (chapter) structure
| # | topic |
|---|-------|
| 서론 | HTML의 문제점 (표현 중심, 의미 정보 부재) / XML의 능력 / 자매 기술(Schema·XSLT·XLink·CSS) |
| Part 2 | 요소·속성 정의 (고유값·유효한 XML·속성 제한) |
| Part 3 | DTD (엔티티·단축형/단축자·외부 파일 단축형·해석되지 않는 컨텐트) |
| Part 4 | 이름공간 (기본 이름공간·개인 요소·DTD와의 통합) |
| Part 5 | Cascading Style Sheets (CSS 설정·HTML vs XML CSS·CSS1/CSS2·스타일 시트 작성) |
| Part 6 | XLink & XPointer (간단한 링크·링크 처리·리퍼런스포인트·연결 정의·파일 부분 링크) |
| 부록 | B |

## OCR/추출 주의
- 목차 일부 OCR 깨짐 ('Table of Centents', 'X겨kfL') — 토큰 교차 확인

## Text (all 253 pages)

===== PAGE 1 =====


===== PAGE 2 =====
1 =====
FOR THE WORLD W嶼f WEB
VISUAL QUICKSTART GUIDE

Peachplt Press

by Elizabeth Castro

===== PAGE 3 =====
2 =====
ㄴ

XML " ' the World Wide Web:
visud QuickS*.『ㅎ Guide
by Elizabeth Castro

Peachpit Press
Find us on the World Wide Web at:
http://www.peachpit.com
Peachpit Press is a division of Addison Wesley Longman
Copyright@ 2001by Elizabeth Castro
All images (except photogr村1s of wild animals)
are copyright @ 1997-2000 by Elizabeth Castro
Cover disign: The Visual Group

H●큔．
．● ●f rights
Allrights reserved. No part of this book may be reproduced or
transmitted in any form by any means, electronic, mechanical,
photocopying, recording, or otherwise, without the prior written
permission of the publisher. For information on getting permission
for reprints and excerpts, contact Peachpit Press.
이 책은 미국의 Peachpit Press와의 저작권 계약에 따라 출판된 것입니다．
이 책의 한국어판 저작권은 한국 저작권 센터 (KCC）
를 통한 저작권자와의
독점계약으로 B&B에 있습니다. 신 저작권법에 의해 한국 내에서 보호를 받는
저작물이므로 무단 전제와 복제를 금합니다．
이 책의 정보는 정보 획득의 용도로서만 사용되어야 합니다．
이 책에서 사용한 설명서나 컴퓨터 소프트웨어와 하드웨어 설명서에 의해서
야기되는 어떤 손해에 대해서도 저자, Peachpit Press사와 B&B는
어떤 책임도 지지 않습니다．
첫 판 찍은 날 / 2001년 2월 5일
첫 판 펴낸 날 / 2001년 2월 10일
원저자 / ELIZABErI'H CASTRO
옮긴이 / 권 필 석
펴낸이 / 홍순우
펴낸곳 / 비 앤 비
주소 / 서울 강남구 논현동 15-12
전화 / (02) 540-4425- 6
팩스/ (02) 517-8793
ISBN 89-86929-80-5

===== PAGE 4 =====
3 =====
21세기 신기술의 한 부분을 담고 있는 이 ㅎ隱，
21세기 우리가 살고 있는 지구와
그 안의 사람들을 지키기 위해서
헌신할 사람들에게 바칩니다．
또한 우리도 나선다면 멸종 위기의 호랑이큘
구할 수 있습니다．

===== PAGE 5 =====
4 =====
감사의 말
Peachpit출판사의Narny Davis, 그녀는유눙한편집자일뿐만아나라
나의 輧7로, 이렇41감사의 글을 쓸 수 았어 叫우 행복합나다. 이책은
그녀가 없었다연 존재하자 않았을 것입나다．
Pbac句)it 출판사의Kate Reber, 그녀의주의갚은 눈과 훌륭한좀짜는
책의완성본이 깔끔할수 있게 만들어 주었습나다．
로터스회사와W3C의XML스카마그룹의Noah Mendelsohn, 나의
질문이）대한그의 일반적아고 정확하고 /7］제한 답변은 이책의스카마와
이름공간파트를 풍요톱거）해주었습나다．
아 책을 저술하는 동안 내 인생의 친구로서 함41해주었고 새로운XML
웹사이트 出ttp1/www.cookwood.com/xmi)에계족 파드백을 해줄
A끄dren Cabre에게 감사드립나다．

===== PAGE 6 =====
5 =====
TABLE OF CONTENTS
차례

人氾

11
i2
13
14
i5
16
17
18

甘드．

ffTh 의문제점
XML의눙력
XML의자u/f가술.
쟐제섕활에서의xML
아책에 r/f해서
이책에저 다루자않는깃들
XML VQS웹사아트

m
。

1장；

XML 작성법
XML요소의속성과가치값
XML작성의규칙
忍fL 버전선인하기
루트요소 만들刀
공백없는요소작쟝하가
요소의중첩）
족성의부가
빈요소 0］
용하기
주석달기
다섯개의특수기호작성볐
문서내요소의표현탭

＾
。
＝
4
m
=a

Part 1: XML
21
22
23
24
25
26
27
28
29
30
31
32

Part 2: DTD
2장：

3장

DTD 만I기

35

내부DTD선언하기
와부I）
二侄）작성하가
외부工γm 아름붐이기
걔인적와부mD산언하기
공용와부DD선안하가

36
37
38
39
40

요소 정의하기와 DTD에서의 속성
요소 정의하刀
텍스트만을포함한요소정의하기
하나의자요소를포함하고 았는요소 정의하가
자퀀스를포함한요소정의하가
선택권정의
많은유낫을정의하는 방법
족성에관해사
간단한족성정의하刀
특정값을가잔족쟝정의하기.

41
42
44
45
46
47
48
49
50
52

V

===== PAGE 7 =====
6 =====
Table of Centents

4장

고유값으로족성설명하가
유효한X겨kfL 아름족성제한하가

53
54

DTC）
에서의 엔티티와 표기법
텍즈트를위한단축형 만들가...
텍스트를위한단축형4-9-하기
외부파일에저 텍즈트를위한단축형
I)Tz）
의단축형제작과사용
해석돠자않은컨텐츠의걔처）만들기
비ll식컨텐츠삽입

55
56
57
58
60
62
64

Part 3: XML. 스키마와 이룸공간
XML 스키마
간단하고도복잡한타입
지엽적선언과포괄쟉선언
간단한스카마사작하刀
간단한스카마의위치자정하가
스카마ll쥐7달기

69

6장

，딘순한 타입 정와1*＇기
단준한타입을가진요소선언
날짜와사간타입 아용하刀
줏자타입 아용하가
단순한주문형 타입작성하刀
무명의주문형 타입사용하가
수용가눙한가치값세트의지정.
단준한타입을위한괘턴정의하기.
가능한값들의 범위정하기
단순한타입의길아제한
줏자의자릿수제한하가
라스트 타입작성하기..
끄소컨텐츠 ㅁ／라정하가

75
76
78
80
81
82
83
84
86
88
89
90
倒

7장

복집한 타입 정의하기

93

요소만을포함하는요소의정의
지퀀스에등장하슨요소요구하刀
선택권세트 만들가
준차적인요소의등장8r용하기
명명된그룹정의하기
명명된그를설명하기
ㅁ／라정의된요소설명하가
등장횟수의조절
텍즈트만을포함하슨요소의정의
빈요소 정의하가
혼합된컨텐츠를가진요소정의하기
복잡한타입을기초로 한복잡한타입
복잡한타입의요소선언하가
무명의복잡한타입들을자닌꾜소
족성선언하가
족성요구하기
속성의컨텐츠 마라정의하刀
족성그를정의하가
족성그룹설명하기

94
95
96
97
98
99
i00
i（끄
102
103
104
105
106
107
108
109
끄0
끄그
112

5장：

Yi

볍＝ 으＝ 。
U *。 으궁H

70
71
72
73
74

===== PAGE 8 =====
7 =====
Table of Centents
8장

9장

113

아틈공간ㅇ／틈 다자인하기
다폴트 아틈공간선언하기.
개인요소들을위한아름공간.
족정에 甲한아름공간의 영향.
이름공간, DT). 우호한문서들

끄4
끄5
116
끄8
끄9

이룝공간, 스키마 그리고 유효성 처리

121

스캬마와이름공간
아름공간의상주
자엽적으로선언된모든요소 첨가하기
자엽적으로 선언된특정요소첨가하기
성분을아름공간으로 설명하가
다폴트로저의스키마들중의스7/r7/
아름공간과XML우효화하가
스7／口／의위치차정하가
복수파일에저의스7］
마
성분의우입...

122
123
124
i25
126
i28
i29
130
131
132

甘드0 。* ＾。＝.m= =

XML의 이름공간 ㅅ용하기

Part 4: XSLT2F XPath
10

11장

12장

XSLT
XSLT로XA 변환하가
XSLT스타일ㅈ］트지작하가
루트 텡플랏작성하기
HmIL코드출력하가
노드의컨텐츠출력하기
텡플랏규칙을만들고적용하가
배치 연산노드
졔한적으로노드 연산하刀
초건적선택권첨가하가...
연산하가전에ㅗ＝드분류하가
족성생성하기

135

XPath: 패턴과 표현
커런트노드 차정하기
커런트노드의설명..
노드의자 (child) 선텍하가
노드의부모나형제(sibling)찾가
모든후손선택하가..
캬런트노드꾸사하기
노드의속쟝선택하刀
부분집함전택하가

153

테스트 표현과 함수

163
164
165
166
167
168
i69
i7α
171
173

두개의값들 비교하가
위차 바：뜨璥7/
가치값소겨］
하기
노드줏자All가
곱하가, 나누가, 더하기, 畔刀
줏자포맷하기
줏자라운당하기
저브스트링끌아내刀
가호열 대문자로 uH7刀

예계의소스코드는www.cookwood.com)l있습나다.

136
138
139
140
142
144
146
z48
149
i50
151

154
/55
156
157
그58
159
拓D
161

VII

===== PAGE 9 =====
8 =====
Table of Centents

Part 5: Cascading Style Sheets
13장

14장
吻섶● *＝。닐 *
。 으二곱
15장

css 설정하기

177

ㅉ兀에저의ass와HTML에저의ass
cssi, CSS2그리고브라우저
스타일분석
스타일의적용위치정하기
와부스타일사트작성하가
Yw문서를위한스타일사트호출하기 .
문서를위한스타일사트호출하가
H'i
내부스타일사트사용하가
지엽적으로스타일적용하가

178
178
179
i8()
粥2
i84
186
187
188

css 레이.民

189

블록단계또는착렬형으로요소정의
요소를완전하캄추가
자여적흐름안에서요소오프셋하기
요소의절대척포자셔닝하가..
요소의높이와넓아설정하기
보더설정하가
요소주변에4탕 더하기
요소주변의 마진 설정하刀
요소주변에 텍스트강싸가
텍스트감싸가 멈추가
배경색상조정하가
배겋색 ㅂ符z刀..
3차원으로요소위치자정하기
제토로요소들정렬하가
초과분의행즈杯］결정하가.
요소 클리핑하기
라스트특정설정하기
페아자브레아크정하가

190
191
192
193
i94
195
196
197
198
199
200
20i
202
203
204
205
206
208

css로 텍스트 포맷하기

汕9

폰트 가족 선택하刀
4아자에폰트 첨가하가
이탤락체 만들기
볼드포맷적용하기
폰트사이．
즈 결정하기
라안높이설정하기
동사에모든폰트값설정하기
텍스트색상설징하기
텍즈트 배경 哨1가
공간조철하기
텍스트 정렬하기.
텍즈트 밑줄긋기
텍스트커）
아스조철하기

皿0
211
212
213
214
215
216
217
218
219
220
221
222

===== PAGE 10 =====
9 =====
Table of Centents

Part 6: XLink2l XPointer
16장

부륵 B

225

간단한 링크 만들가
링3A11트 만들기
ll퍼런스포인트 정의하기
연결 정의하刀
랑크시庫사용하가
파일의부분을 링크하가
가장간단한XPointer만들기
걸어 다나는XPointer만들기
XPointer 밖）우／반듭가

226
228
229
230
232
233
234
235
236

XHTML

239

어떻게브라우저가구별할수있을까？
끄汀l1甘fL작성법
끄끄쬐iL을위한DTL꺄／언하刀.

240
241
242

XML 도구1

243
244
245
246

DTD에관II XML파일유효화하가
스카ㅁ／툴가지고xM【』유효화하刀
XSML 연산차로xM【』변환하가
부륵 C

부ID

륵수 기호1
글자레퍼런스사용하기
표그：문자
표2:7］
호

247
248
249
250

16진법 색상

251

Z6진법이］
사색상의／코GB성분 발견하기
石찬볍）표기 코드

252
253

뻐
。 뜨。 。
m ＾。＝0. =

부I A

링크와 이미지듈

찾아보기, 설명
찾아보기

255

설명

268

예제의소스코드는www.cookwoocLcomc?I있습나다.

ix

===== PAGE 11 =====
10 =====
INTRODUCTION
서론
확실히 인터넷이라는 매체는 세계를 변화시키고
있다. Tim Berners-Lee의 월드 와이드 웹 디자인
(1991）
과 Marc Andreesen이 PC나 맥에서 월드
와이드 웹을 볼 수 있는 기능을 가진 소프트웨어를
개발한 후로 인터넷이라는 매체는 단순한 흥미거리
에서 우리 생활에 필요한 것으로, 그저 우리 생활의
보조적인 것에서 핵심적인 매체로 발전되어 왔다．
웹 사이트는 이제 우리에게 없어서는 안될 정보의
창고이며 나아가서는 개인 생활의 일부가 되어 가고
있는실정이다. 인터넷에서 검색할수 있는정보의
양은 헤아릴 수조차 없게 되었다. 인터넷 웹 페이지
의 정확한 숫자는 아무도 알지 못한다. 다만 20억
내외라는 것만 알려져 있다.
이러한 웹 페이지의 거의 대부분은 HTML - Hyper
Text Markup Language - 로 이루어져 있다．
이 언어는 어느 컴퓨터 기반에서든지 볼 수 있는
텍스트 파일 안에 특별한 태그 형식을 통해, 간단하
지만 우아하게 데이터를 구성할 수 있는 언어이다．
HTML의 간단함은 웹의 인기를 폭발적으로 증가
시켰지만 - 누구나 웹 페이지를 제작할 수 있다 웹의 거대하고 빠르게 늘어가는 정보의 양에 부딪
혔을 때는 한계를 느끼게 된다.
XML 또는 Extensible Markup Language라는
언어는 HTML 언어의 기술 기반으로 만들어졌지만
끊임없이 증가하는 인터넷 정보의 양적 증가를 더
효율적으로 관리할 수 있게 만들어진 것이 특징이다．
XML이라는 언어는 처음에는 많은 주의를 필요로
하지만 더욱 좋은 결과물을 만들어 내는 특징이
있다. 말하자면 HTML이 모든 사람에게 자그마한
혜택을 주었다면 XML은 소수의 사람에게 풍성한
혜택을준다고할수 있다. 이 책은XML을어떻게
시작하는 지에 대해 가르쳐 줄 것이다．

11

＝

。

＝

＾

탕

。

＝

=

===== PAGE 12 =====
11 =====
Introduction

HTML의 문제점
HrML의 성공의 요인은 단순함, 쉬운 사용법, 그리
고 프로그램의 융통성에 있었다. HI丕4L은 쉽게 쓸
수있는언어이다. 이것은대문자나소문자를쓰는
것에 아무 제약이 없고 인용 마크에도 영향을 받는
법이 없으며 마침 태그에 대해 세세한 신경을 쓸
필요도 없다. 이러한 편리함이 모든 사람들에게 친숙
하게 다가가는 이유가 되었다．

H릉토 ,＝클 ㅌ 으 궁 左 0吉

그러나 IㅠML의 단순함은 이것의 능력을 제한하는
면이 있었다.HTML의 태그는 화면의 구현에 무게
를 두고 있을 뿐이어서 웹 페이지의 내용에 대해서
어떠한 정보도 주지 못한다. 따라서 다른 화면에
있었던 정보를 재편성 하기에는 어려운 점이 많다．
HTJL은 대／소문자나 구두점 같은 것에 엄격하지
않기 때문에 HI爪4L 운서를 제대로 보여주기 위해서
브라우저는 두 배의 노력을 해야 한다．
그리고IfrML이 포맷팅과 동적인 화면을 보여주는
데에는 한계가 있기 때문에 많은 확장 명령어들이
효율성을 더하기 위해 추가된다. 불행히도 이러한
확장 명령어들은 몇몇 특정 브라우저에서만 작동
된다. 따라서 이것들을사용하는 페이지들은특정의
브라우저를 사용하는 방문자들에게만 보여지는 단점
이 있다．

-

.

de.htor,l

<center>cimg src=tiger.ipg></center>
Animal species are disappearing from the earth at
a frightening speed.
<P>According to the World Wildlife Federation, at
present rates of extinction, as much as a third of the
world's species could be gone in the next 20 years.
<hr width=50% size=5 noshade>
그림Li 여가에는 일반적브로 많아 쓰아는 ffTh 코드들ㅇ／있다．
여가에는 ㅈ］작HTML아라든치HEAD 태그들ㅇ／ 없는 것을 알 수
았다. 아띤 태그들은 소문자나 대문자들아 섞여있는 것도 볼 수
밌다. 왼쪽에는 표준 孑i刃kfL 규정에 맞자도 않는 것들하 있다. 어딴
값들도 인용 마크에 들아 았는 것아 없다（심지어는 URL까ㅈ］도7.
p 태그는그것과부합되이야 함</p>값도 가차고 았자 않으며
가차값을가자는 족정도 하나밖珊 帥卄또는 얼마나주의 갚거7
보느나에 따라 족쟝아 없는 가차값도 발견할수 았을 것아다）=
noshade α：r 태．
그 중에서夕．

i0 \,nl,,〕es.supk,to,흼il& ht, l- Hi.,,osoftlnle,,,etEwplo.e,
E1e

fm

Ym덖 F4'ot,,

Lo出 bet

Aa,a,tt apesoes are 出s.ppe町1ng from the earth 封 a 丘哮αe1m培 rpeed
Accorng to 仕LtWo,!d Wddife Fud, at prestos rates of exats0000. a, mo轍
at atfard ofthe motto's speoset ctodd be goat ar the teat 20 year,

그람i2mML 언어의느즌함에도 옭z하고 폐아지는 바르게
보여지고 있다．

12

의

<BODY bgcolor=#flcc99 text=red leftmargin=5>

===== PAGE 13 =====
12 =====
Introduction
琵m－

華穽玆홀Code .1,17,11

m

<?xml version="1.0" encoding=「UTF-8"?>
<endangered_species>
<animal>
<name language="English">Tiger</name>
<name language="Latin">panthera tigris</name>
＜十reats>
<threat>poachers</threat>
<threat나iabitat destruction</threat>
<threat>trade in tiger bones for traditional Chinese
medicine (TCMk/threat>
.c/threats>
<weight>500 pounds</weight>
<length>3 yards from nose to tail</length>
<source sectionid="101" newspaperid="21"I>
<subspecies>
<name language="English">Amur or
Siberian</name>
<name language="Latin">P.t. altaica</name>
<region>Far East Russia</region>
<population year="1999">445</population>
</subspecies>
</endangered_species>
그림i.3 첫눈이］보7］
에는XML 언아는｝
刃醜
［L 언어와 맣아 달라
보아자는 않는다. 아 언어도 태그와속성값，
가치값들아 많아 보인
다. 태그가 어떻게그 태＝Z안의 내용을포함하고 았는지주의깊게
보도록 하자. 어깼든ㅉkiL은 훨씬 엄격한규칙을요구하고 았다．
아 규착온1장XML 작성법에저살펴볼 것아다．

예제의소스 코드는 www. cookwood. comb/i 있습나다．

XML (Extensible Markup Language）
은 편리하지
만 기능의 한계를 가지고 있는 HTML 언어의 해답
이다. 밖에서 보면 XML은 거의 비슷하고 wFn콰
같이 태그, 속성값그리고 가치값들을 가지고 있다
（그림 L3).XML은 웹 페이지를 만들 수 있는 언어로
서 뿐만 아니라 다른 종류의 언어를 만드는 데 사용
할 수 있다. 우리는 XML 언어를 개인적인 마크업
언어를 만드는 것 뿐만 아니라 우리가 가지고 있는
문서를 포맷하는 데에도 XML을 사용할 수 있다．
xM.은통상적인 마크업 언어 뿐만 아니라, 그 안에
있는 정보를 표시하는 태그를 가지고 있다．
여기에 xML의 힘이 있다. 어떤 태그가 어떤 데이터
를 정리하고 있다면 그 데이터는 다른 작업에도 이용
할수있을것이다. 어떤소프트웨어는그프로그램
이 필요한 정보를 끌어올 수 있고 만일 다른 소스에
있는 데이터와 합쳐져 다른 포맷과 다른 목적으로
디자인된 결과를 얻을 수 있을 것이다. HTML을
기반으로 한 웹 페이지에서는 자칫 그 안의 정보들을
잃을 수도 있지만 xM.에서 확실히 정의된 정보들
은 필요한 만큼 언제든 다시 사용할 수 있을 것이다．
그러나 언제나 그렇듯이 편리함에는 대가가 따르는
법이다. XML 언어는 WIML처럼 너그럽지 못하다．
xM. 파서（구문 구조 해석기）
는 대／소문자 구분을
확실히 해 주어야 하고 인용 부호 마침 태그와 같이，
HTML에서는 기분좋게 넘어갔던 세세한 부분을
신경써야한다. 이런 xM.의 까다로운 성질이 개인
웹 페이지를 만들려는 사람들에게는 외면을 받겠
지만 보다 큰 스케일로 정보를 관리하고 싶은 웹
디자이너들에게는 각광을 받을 것이라 생각한다．

13

。 是 旦 。* 님결尸
구m 뜅

<picture filename="tiger.jpg" x="200" y="197"/>

XML의 능력

===== PAGE 14 =====
13 =====
Introduction

XML의 자매 기술
XML 그 자체는 간단하다. 그러나 XML의 능력을
높이는 것은 바로 XML의 자매 기술들이다．
스키마 (Schema)라는 것은 XMI으로 만든 통장적
인 마크업 언어이다. DTD로 쓰여졌든 XML로 쓰여
졌든 스키마 (Schema) 언어는 문서에서 사용된
태그들이 어떤 것들이었는지 또한 태그들이 가지고
있는속성들을 정의하고 있다. Part 2 (p.33 참조）
에
XML
(p67참조）
에서
凞오를배울것이고Part
3
서
l剋｝
a)릍 배울 것이다．
日上無』
坦l；
아마도 XML 문서를 작업하는 데 있어서 가장 강력
한툴& XSL7 Extensible Stylesheet Language
- Transformation그리고8殮如일 것이다．XSLT
m
느
● 프● ＇르呈乂

謐器높썲SLT搬擺 。]4
전체 버전을 만들 수 있다. 그리고 가장 중요한 것은
XSLT를 이용해서 XML을 HTML로 전환시킬 수
있다는 사실이다. XPath는 문서의 다른 부분을
정의하는 시스템이다‘X8LT와 XP 出- Part 4

(p133
蕁群霽象豪

）
에자세히泓윅Ttr.

우리는 scratch（컴퓨터 내부 또는 외부의 작업용
기억 매체）
에서 xML 태그를 만들었기 때문에 이러
한 태그들이 고유한 포맷팅이 없다는 사실에 대해 놀
랄일이 없다. 브라우저가＜animal> 태그를 알 수
있을까？대답은 물론 '알수 없다 이다. 그럼 주어진
태그를 어떻게 배치할 것인가. XML 문서를 포맷
하는 두 가지 방법이 있는데 XSL-FO와 cSS이다．
그 중 CSS (Cascading Style Sheet쩨는불안정한
면이 있지만 여러 브라우저에 대해 호환성이 있는
강력한 기능도 가지고 있다．
／溺毓上芼的 (p175
참조）
에서 배울 것이다.
마지막으로 XLink와）
(Pointer 등은 XML에 링크
또는이미지를삽입하는 기능을부과한다. 두 가지에
대한 설명은 마지막에 나와 있기는 하지만 둘 중
어느 것도 어떤 브라우저와도 호환성이 없다. 다시
말하면 아직 작동이 되지 않는다는 말이다. 그러나
이것들은 XML의 필수적인 부분이고 이것은 Part 6
(p233 참조）
에서 다룰 것이다.

14

===== PAGE 15 =====
14 =====
Introduction

山

品

■

d蠟
J
s1邙

,

고
n" [.d,

스
ㅐ여
＇.

댜
5'm口1

F

＝』

G.

炤C纖흩－幽i繃烏
Lei瓣ng the 什eb to iL JullPteential...
Ada기i粗e! 1 T.dmir.l a-

미 a.Ii4.치A如 tW3C c.ntart

lheW.r[dW,J. 구Jeb C:>1瑙Dm嶼1(W3C돈Jeve!;p3 n止er
《，
perable t．
￡Fㅗ心oaa
GPec'ca효
《，
t琨- 너』neS. 8岫
「四町乙.dak) aledt. Web tα 沈i 耽皿P0t仕＇血“- a
比l깁mf〕
rn址0m- cc. It. .
h에｀m岫mn．
ㄷbva m血
［或班t繃떵 Fn洲 0dt
mOI亡 벴기衿많 V／多c

邸蝦＾J보工
A￡‘eSS小d的
凡naVa
cc厘P
（媤S
二흐조끄쁘世즈
pQN

》xML Buse
Advanced to
cauhdate
요ecommendation

＇td
《加t`1v굻

'推空

씨蜘r翩녠1뇨72口娘 w犯,.
mJ‘→n1』*n `n→ ^ 1"．
' ㅐ｀`

Nn, fth,
轟꺽y, 薛驕굶，

'：쁘쁘∼“뻔헷＝一〃' : ‘亡
krPr.꼬rd1uba$e URi
XLk .d3。
0小月i XML

J』
｀，뛰mW
= ==
1口四U너Jr
;.-mrrㄷ兮dvn1e11
［珊
` 1 . '
也으므므

켰헒

藍
컨v1=

n
*
ani）
目can에5 .enemm?1r)m c0m1m
1
￥一누 H
,
蠟切＝T rem口7e u끄』
｀ ㅗ』1· ㄴm긔여二aㅈ亡
b
1 」
1 n
`L
【ㄴU"U」
Jㄷ】工｀m4v1J PC]i`nJ =LnJ* .
n
`^r小
"1
｀〃，^
ㅗJㄷ
｀r`11L7C1' eU｀
빙1 口J'C∥山r '5똬

莎

ect1t.
『河i:J띠tG[,）仰！町）
l프그蠟匹P｀긺
dthv·rpr.ofofu'e .rxML Ba北

불행히도 XML 사용의 현실과 이상에는 거리가
있다. 지금 현재 XML 언어를 지원하는 브라우저는
그렇게 많지 않다. 인터넷 익스플로러 5.0 버전
（매킨토시와 윈도우）그리고 넷스케이프 6.0 베타
버전 등이 지원을 하고 있다. 이전의 브라우저에서는
XML 파일을 생소한 텍스트로 인식하고 있다．
XML의 가장 큰 단점은 어떤 브라우저도 XLink와
XPointer 등을 지원하고 있지 않다는 사실이다．
어떤 브라우저도 XMT. 페이지에 링크와 이미지를
보여주지 않는다. 이러한문제들이 해결되지 않는한
아무도 XML 페이지를 직접 웹에 올리는 사람은
없을 것이다. 이같은 XML의 단점을 극복하고 XML
을 이용하여 정보를관리하기 위해서는製쁘＝立선
를 모든 브라우저에서 사용되는 HTML 문서로 바꿔

蓬及血茁亶3喚論결琿겅筒可繭－

:；芬；, N
pccl&Slolu.二d．kpfl
u14기Cnlt1“· 4'Um ·‘ ｀下ㅛㄴ口H`i1》

"mM

그림1.4 월드 와이드 연합 伽tp://www. w3. org)은 웹의가장
표준에 대해저 설명하고 있다. 아 책에서 다루고 았는 모든 언아에
CM한모든 공식적인 설명을 볼 수 있다 ( ML 그리고 DID). XML
&hema, namespaces, 乂弘T, X」
P砒h, xi
【出炚, X凡心1terH7?/fL
과xHmL등은물론이고, 好fL의쟐제상황, 쟐쟁활에저의XML
등도 다루고 있다．

사용한다면 손쉽게 XML의 뛰어난 기능 뿐만 아니
라 HTML의 보편성도 동시에 누릴 수 있게 된다.
월드 와이드 웹 건소시엄 (World Wide Web
Consortium (W3C)）에서는 XHTiz의 사용을 권장
하고 있다 - 이 시스템은 }I,1, 4 ,의 태그를 XML의
엄격한규칙을 적용해서 작성한 문서이다. 즉XMT
과 HTML의 중간 단계라고 할수 있다．
만일 XH呱4L만을 이용한다면 HTML의 편리함
뿐만 아니라 끄4L의 정보 표시 기능마저 잃게 되는
셈이 된다, 우리는XHIML에 대해서는 부록A에서
다루기로 한다．
이론적으로 익스플로러 5.0을 XSLT를 사용하여
XML을 방문자의 브라우저에 적용할 수 있는
HTML
바꿀수 있다. 그러나 불행히도 익스플
로러는 XSLT의 표준 버전을 지원하지 못하는 대신
에 마이ㅋ로추ㅍㅌ사가 정한 몇 가지 확장 언어를
포함한 이전 버전들의 조합을 지원한다. 따라서 우리
는 적어도 당분간은 XMT 문서를 HTML 문서로
변환시키기 위해서 외부 XSLT 프로세서를 이용해
야 한다. 이것에 대한 자세한 설명은 10장 X,SL7쩨
나와있다．

예계의소스 코드는 www.cookwood.com에 있습나다．

15

乂클P = 4= . ”츰 릎。 ，
=

조그
［꼬
三쪼논스흙찜브스밸卄괬珊스
三변媤뾰

실제 생활에서의 XML

===== PAGE 16 =====
15 =====
Introduction

versi。
n=" 1
<endangered_species>
<anim히＞
<name language="English">Tiger</name>
<name Ianguage="Latin">panthera
tigris</name>
<threats><threat>poachers</threat>
＜十reat寸1abitat destruction</小reat>
<threat>trade in tiger bones for traditional Chinese
medicine (TCMk/threat>
</threats>
<?xml

이 책에 대해서
이 책은 크게 6장으로 나누어져 있다. XML 작성법，
DTDs, XML스키마, XSLT와XPath, CSS그리고
XIㅍnk와XPointer등이다. 각파트는XML과관련
된 작업들에 대한 순차적인 설명이 들어 있는
하나 위에서 말한 여섯 개의 장으로 구성되어 있다．
가능한 관련된 코드를 실제 브라우저에서 보여지는
화면과 같이 설명할 것이다．

＝
。
。
m 쓰亡 *
。
。
＜

때때로 같은 페이지에 둘 이상의 문서를 보여지는
경우도 있는데 그것들은 아마도 XSLT 문서와 변형
되어질 XML 문서들일 것이다. 제목을 보면 어떤
문서인지 바로 알게 될 것이다（그림 i.5). 빨간색
으로 표시된 텍스트나 이미지는 일반적으로 그 페이
지에서 중요한 부분이다．
먼저 독자들이 웹 사이트 (pi8 참조）
에서 예제 파일
을 다운받기를 추천하고 싶다. 그리고 이 책을 공부
하면서 그것들을 항상 이용하기 바란다. 많은 경우
각 페이지에 문서 전부를 보여 주는 것은 불가능하다
고 생각하기 때문에 그 예제 파일을 보는 것이 많은
도움이 될 것이라 생각한다．
이 책에서 다루는 대부분의 브라우저는 XML의 여러
기능을 많이 지원할 수 있는 인터넷 익스플로러 5.0
일 것이다. 그러나 웹 사이트에 방문하는 방문자들은
다른 브라우저나 다른 플랫폼을 사용할 수 있다는
점을항상명심해야한다. 디자인하는웹 페이지가
누구를 위한 것인지 또는 사이트의 방문자가 주로 사
용할 웹 사이트가 무엇인지를 항상 염두에 두는 것이
중요하다. 그런 후어 웹 페이지가모든브라우저에서
제대로 작동하는지 시험해야 한다．
전문가의 수준은 아닐 지라도 적어도 IT꼬ML에 대해
어느정도 친숙해질 필요가 있다. 다른 사전 지식은
이 책을 공부하는 데 필요하지 않을 것이다．

16

그림i 5 타아틀 바를 보면 쉽재 아깃이XML 코드의 일부분아라는
것을 알수 있다（아ㅁ／도 구별하는 것은 어려운 일이 아닐 것아다．
.
의심이가는 경우에는 여가에 별도의 단서가 있다）

===== PAGE 17 =====
16 =====
Introduction

이 책이 다루지 않는 것들
XML은 정보를 다루는 아주 강력한 시스템이다．
다른 여러 가지 기술들과 더불어 XML을 이용할 수
있을 것이다. 명심해야 할 것은 이 책은 XML의 고급
편이 아니고 웹 페이지를 만드는 데 사용되는 입문서
라는 것이다．
이 책은DOM. SAX. SOAP 또는XML-RPC 등에

대해서횬여：章쿄힛可穫纛卞三而疏겹而耳和

특히 어떤 것을 처음 시작할 때 작은 범위의 주제들
에 대해 명쾌하고 특별한 지식을 갖는 것이 때로는
모든 것에 대해 넓은 이해를 가지고 시작하는 것보다
더 도움이 될 것이라고 생각한다. 이 책에서 XML에
대한 확실한 기초와 핵심 기술에 대해 깨닫게 될 것
이다．

셍聊의소스 코드는 www.cookwood.corn에 있습나다．

17

。
·
芝＝ 。
4 부 ＝ ．。。骨 = ＝

는 기술인 자바스크립트 또는 ASP에 대해서도 전혀
다루고 있지 않다. 이런 각각의 주제들은 그것에
관한 책을 하나씩 참고해야 한다. XML에 관련된
많은 기술들이 있지만 이 책은 XML의 핵심 요소들
XML, 스키마, 변형, 스타일링, 그리고링크등과
같은, XML을 기반으로 한 웹 사이트를 만드는 데
꼭 필요한 주제들만을 다룰 것이다．

===== PAGE 18 =====
17 =====
Introduction

XML VQS 웹 사이트
（기ㄷ 훼· 비ㅈㅇJ 퀴ㅅ
YMI 워ㄷ 야

ㅌ

이ㄷ 워］

（http://www cookwood.corn/Jan끄에서는
사이트
이책에 있는 모든 예제를 찾아보거나 다운받을 수 있
는장소다. 또한작가가사용하는XML parser,
XSLT processor 그리고 schema validator 등의
사용자 툴 링크도 찾아볼 수 있다．
또한XML 월드 와이드 웹．
‘ 비주얼 퀵스타트 가이드
웹 사이트에서는 컨텐츠와 인덱스의 온라인 테이블，
Q&A 코너 업데이트 등등의 부가적인 요소들을 포함
하고 있다．

●璜 ,m뇰8> “
宅
님 ●亡

이 책의 모든 예제, 컨텐츠 테이블과 정오표（양이
적기를 바란다）등을 제공하는 사이트의 주소는
http.i/www.peachpit.com/vqs/xrn]이다．
질문 시촹들은？
질문 사항에 대해서는 별도의 XML Q&A 보드를
이용하기 바란다 (http.i/www.cookwood.corn!
xrn均anda). 공개적으로 질문에 답하는 것은 더
많은 사람에게 동시에 답할 수 있는 효과를 나타낸다
（그리고 독자들이 서로 도울 수 있는 기회가 된다）
.
그리고 작가와 직접 연락할 수 있는 방법도 볼 수
있을 것이다．

18

===== PAGE 19 =====
18 =====
PART 1:

x卜m..

XML 작성법 21

]9

===== PAGE 20 =====
19 =====
1

WRITING XML
지네．
. 작성법

XML이란 통상적인 마크업 언어 (custom markup
language）
를만들수 있는문법 체계라할수 있다．
예를 들어 XML을 이용하여 계통학이나 수학, 화학
등을 정리하고 웹 상에서 구현할 수 있다．
XMl로 만든 모든 통상 언어 (custom language)
들이 자4L 문법으로 만들어졌으니 당연히 XML은
이 문법에서 시작해야한다. 이번 장에서는XML
문서 외에도 XML로 이루어진 통상 언어를 작성
하는 기본 규칙을 배울 것이다．
XTh로 만들어진 통장적 마크업 언어 (Custom
Markup Language）
들을 'XML적용이라고말할
수 있겠지만 이것은 'XML에서 사용된다’ 라는 느낌
을갖게 한다. 그러나정확하게 '적용 이라고하는
것은 포토샵과 같이 완성된 프로그램을 의미할 것이
다. 따라서 이러한 개념들을 명확하게 파악하는 것은
어려운 일이므로가급적 ' XML적용과같은개념
을 피해 설명하고자 한다．
XMl．
의 작성 도구들
XML은 HTMl과 마찬가지로 텍스트 에디터나 워드
프로세서 등으로 작성할 수 있다. 매킨토시의 아주
기본적인 SimpleText나 윈도우의 WordPad 등이
여기에 포함된다. xML을작성하면서 XM1 문서를
테스트할수 있는 텍스트 에디터 등도 있다. 마지막
으로 다른 종류의 프로그램（레이아웃 프로그램부터
스프래드시트 데이터베이스 등）
에서 XTh 문서로
전환시키는 프로그램들이 있다．
여러분들은 문서를 열고 저장하는 방법 정도는 알고
있을 것이다. 모든 XML 파일은 .XML 확장자로
저장하는 것을 명심하기 바란다．

2경

===== PAGE 21 =====
20 =====
다apte리
1lL…,

m
● ＝=>,＝。｀m● *＝욘， = ＜ 立 ＝ 0ㅌ 으빌

족정은 시작 태그와 함께 포함되는데 인용 부호를
이용하여 특정의 목적과 개념 정보를 설명하고 있는
가치값의 한계를 정의한다（그림 1.2). 속성 안에
들어있는 정보는 일반적으로 메타 데이터 (metadata）
로 인식된다. 다시 말해 이것은 그 정보 자체를
〃관한정보를 가지고
가지고 있는 것이 아니라 정보ㅇ
있는 것이다. 하나의 요소는 그들 각자의 고유한
제목이 있는 한 필요한 만큼의 속성들을 가지고 있는
것이다．
이 장의 나머지 부분에서는 요소와 속성 그리고 가치
록 하자.
값을 작성하는 방법을 알아토도．
공백
XML 코드 주변에 여분의 공백을 넣을 수 있는데
이것은 편집과 보기를 용이하게 하기 위해서 사용
한다（그림 1.3).

'，
”「

h1nerl;
<n.meγ～
1 .--/nnmn.
-

마침태그

“기

XML은 HTML과 마찬가지로 요소의 속성과 가치값
같은 구성 단위를 사용한다. XML의 요소는 문서의
가장기본적인 단위이다. 이것은 텍스트들을포함한
다른 요소들을 포함한다. 하나의 요소라는 이름을
가진 시작 태그는 < 기호와〉사이에 있는 것들을
가지고 있다（그림 Lp. 제목은 자신이 임의로 만드
는데 요소의 목적과 특히 이것의 개념 정보가 있을
경우는시작태그를따라야한다. 요소는 일반적으로
부등호 부호의 시작 태그에서 이름 앞에 / 기호를
붙인마침 태그로 마무리된다．

.

1

L

XML 요소의 속성과 가치값

4t

…

…；;A]

그림i그 전형적인요소는사작 태그와 마침 태＝Z로 구성되어 있다．
이러한요소들은그 안에 텍스트를포함한다．

속성

<name language="English '> Tiger </name>
가치값（안용 부호 안의 것）
속성 이름
등호 표시
그람 工2 이제꼭요소에는 가차값아English인 언ㅇ7로 불라는
투성을가자고 있다. Eng1ish

단어가제목pA, 의부분이 아님

을 명심하자. 아 제꼭은English가 아나고 더욱아English Tiger
는 더더욱 아나며이특쟝은 그것의개념 정보를 나타내고 았다．

시작 태그

<animal>'
<name longuage=hlEnglishhl>Tiger</name>
<name language="Latin">Panthera
tigris</name>
<weight>500 pounds</weight>
</animal>
따침태그

컨텐츠
그람 工3 아 예제에있는animal 요소는 세개의 다른 요소를
포함하고 있고 (.듀〃의제꼭과 한개；의무게요소J 텍즈트는 없다．
는
제꼭皿 (name element)와 무게요소 佃eight eleme或）
텍스트를포함하고 있지만 다른 요소는 없다. 이코드를 앍가 쉽게
만들아 놓은공백 (white space汀여가 예제에저는 핑크川 주꼭해
보자. 아 공백은html에서처럼IE5（인타넛ir 익스플로라 5. 이와
Mozilla (넷스케아프 6.0 베타 버전：）에서 파서로 넘어가게 된다.

22

===== PAGE 22 =====
21 =====
Writing XML
code.ernl ‘ㅌ睾스三

口

XML 작성의 규칙

<2 cml version="1.0''?>

<?xml version="l .0"?>

최대한으로 유연성과 강력함을 갖춘 XMT.을 만들기
위해서 XMT.은 어떠한干칙에 의해 정의되어야 하
고 반드시 예상 가능한 구조를 가지고 있어야 한다．
아래의 내용들은＝巧구칙들 중에서도 가장 중요한
것들이다. 만일 어떤 문서가 이러한 규칙들을 잘
지키고 있다면 이것은 구조가 좋은 것으로 평가된다．
만일 어느문서가잘정돈된 干칙을지킨다면브라
우저 상에서도 멋지게 보여질 수 있을 것이다．

<endangered_spedes>
<name>Tiger</name>

8수j gt.eIeme뺏트瀷욧ㅎ卜다
룬틋，

<e dangered_species>
<n ]me>Tiger</name>
<I sndangered_species>

r

小

Coee.Hnit

函ㄱ

그림工4 구성이찰된 문서에는 다른 요소들을모두 포함하는 하나
의근원 요소가 필요하다. 첫번째 줄은 연산 명령아고 아것은 근원
요소를 벗어나도 괜찮은 것들이다．

<picture filename="tiger.jpg"/>
c/endangered_species>

．…

모든 요소에는 반드시 마침 태그가 필요하다. 빈 태
그들은 < > 표시 전에／를 가지고 있는 시작 태그와
마침 태그를 동시에 표시해 주거나（그림 :1.5) 또는
하나의 다른 마침 태그를 갖는다．

code.N i三

<name>Tiger</name>
<Name>Tiger</Name>
訂前

미칩 태그는 필요하다

c dejsn기

<name>Tiger</Name>

요소둘은 잘 罌되어야 한다

그람 1.6 위의 예겨）
는 혼란스럽기는 해도 규칙이）
는 맞다. 두 요소
들온완전하독립적안것으로간주된다. 밀의예제는틀린깃아다．
왜나하면 ㅈ／작 태그와 마침 태：Z가 서로 일치되자 않았기 때문아다．

요소 A를 시작하고 요소 B를 시작한다면 요소 A를
닫기 전에 요소 B를 닫아야 한다（그림 L5).

飾i훌츤＝二ㅌ든斗’三－ ---

즈 cl〕
de．
ㅐnㅐ

냠．

<picture fiIenamejger.jpd7>
그람 i7 아B／한 인용 부호는 꼭 필요하다. 그들《）
]찰 일차되는한
인용부호는작은따꼼표 (p든큰 따옴표 ( ')든상관없다．

대／소문ㅈ浩 중요히다
XML은대／소문자에 민감하다. animal, ANIMAL,
그리고Animal이라는 요소들은 완전히 별개의 것
이고 아무 관련이 없다（그림 L6).
가치값은 반드시 인용 부호 인에 있어야 한다

어느- 1설읜．
Z브雙量3트스上흐臘폿늪置의
（그림 '.7).
鱗흰t交i의으上쑈다
원；
실제 지시어들은 반드시 표시해야 한다
HThII꽈는 달리 다섯 개를 하나로 만든 것을 제외
하고는 (p31참조) XML에 쓰인 모든 실제 지시어
(entity reference）
들은 사용되기 전에 반드시 DTD
에서 밝혀져야 한다．

여／z7）의 소스 코드는 1` vw,cookwooc加om에 있습나다．

23

".=m* 휴 是 ＝ ==.X글尸

그림1.5모든요소들은 마무라가잘되어아 한다. 공백에는 사작
태그와 마침 태그, ／믈 가지고 있는 집약된 태＝Z를표시함수 있다．
명심해야 할 깃은 중복된 꾜소는 존재하자 않는다는 것이다. 다사
말에요소들은 쟐 정리함 필요가 있다．

모드 XML 문서들은 문서의 다른 요소를 포함하는
4나의루트 ! ' 浬요하다. 루트요소에서 벗어날
이나 연산 명령
수 있는 ㅊ百슨 주석 (comments）
(processing instructions) 뿐이다（쑈l림 '.4),

===== PAGE 23 =====
22 =====
Chapter 1

XML 버전 선언하기
일반적으로 각각의 XML 문서는 버전을 밝혀 주어야
한다. 이 라인을 XML 버전 표차라고 한다．
시용하고 있는 XML. 버전 밝히기：
1, 먼저 문서 첫부분에＜?xml을입력한다．
2. version=" 1.011（이것이 이제까지 있었던 버전
이다）
3. ?> 이 공표를마친다．

V Tips
＝욕， 0
> H름님0츱。 ＝：。＝●。

■ <？로 시작하고？＞로 끝나튼 태그를 연간명령
이라고한다. 이것은
(processing instruction）
XML의 버전을 밝히는 것 외에도 사용해야 할
스타일 시트 (style sheet）
를 정의하기도 한다．
스타일 시트에 대해서는 p175에서 시작하는 5장
에서 자세히 다룰 것이다．
■ 버전의 숫자를작은따옴표나큰따옴표로마무
.
리해야 한다（어느 것을 써도 상관없다）
■XML 버전 표지는 선택 사항이다. 이것은 문서
의 첫째줄에 위치해야 한다．
■ 문서가다른문서와연관이 있는지를밝혀야
.
한다 (p3940 참조）
■ 만일문서가UTF-8이나UTF-16으로구성
되어 있지 않다면 XML 연산 명령을 사용하고
있는 문자의 종류를 밝히는데 이용해야 한다．

24

C0d

<?xml version= 1 .0∥ 2>
그림i8刃iIL 버전표자 요소가 아나고 연산 명령
（)］가 때문에
마침 태그가 없다．

===== PAGE 24 =====
23 =====
Writing XML
奢圄三；노三i=j裏길1〕
三 긴A4 c1〕de.ㅐI`11 華列∼1珊→＝

<endangered_species>

</endangered_species>

루트 요소 만들기
모든 XML 문서는 여러 요소들을 포함한 하나의
요소를 갖고 있어야 한다. 이러한 일련의 요소를
루트요소라고한다．

그림工9Jf7m갼L에서 루트 요소는 언4나 HTML아다. XAU에저는
루트 요소의 아틈；으로 아딴 아틈을써도 꾸방하다. 예제에서 보둣ㅇ］

투트 요소 매I기：

endangered_species 등도 어딴 내용 정보와 다른 요소도

1. XML문서의 처음에＜r.이＞라고입력한다．
root가 있는 곳에 나머지 다른 요소들을 포함
하는 요소의 이름을 입력한다．

사작과 아침 루트 태그 전후叩올 수 없다．

2. 문서의 나머지를 만들기 위해서 몇 줄의 공백을
남긴다．

I, 7iPS
■ 대／소문자가중요하다. <NAME＞은＜Name＞이나
<name＞과는 전혀 다르다．
■ 유용한요소（그리고특성）이름들은글자또는
하선( ) 또는 콜론 (:）으로 시작할 수 있고, 그
수에 상관없이 다른 글자나 숫자 하선 ( ) 하이
픈, 마침표, 그리고콜론등이 올수 있다．
■ 콜론은대체로특정 이름공간을한정하고
x, m, 1로 시작하는 이름은（대／소문자 상관
없이）W3C가 먼저 독점해 놓았다．
■ 루트 요소의 마침 태그는 필요하다
■ 다른 어떤 요소도 시작 태그와 마침 태그를 벗어
나서 사용할 수 없다. 시작루트 요소 (opening
root element) 앞에 쓸 수 있는 유일한 것은
연산 명령 (processing instructions) (p24
참조）
과 스키마 (schemas) (p67참．
조）
뿐이다．

예제의소스 코드는 www.cookwcod.com.# 있습나다．

25

。 m 。 ＝＝山4于m” 。。*쯔m크。 ＝
4

3. c/root> root위치에 1번에서 선택한 이름을
넣는다．

===== PAGE 25 =====
24 =====
태apter ]

공백없는 요소 작성하기：
1. <name＞을입력한다. name자리에 나타내고
자 하는 내용을 이름으로 입력한다．

3. </name＞을입력한다. name자리에1번에서
정한 이름을 쓴다．

=＝●ㅌ으W， 뵤ㅌ 뿌
＝ 。＝m＝ 픈 多

'/ nP`
■ 마침 태그는 필수 사항이다 (HTML에서는 선택
사항이었다）
.
■ 일반적인요소들의 이름을만드는방법은루트
요소의 이름을 만드는 방법과 같다. 다만 대／소
문자는중요하다. 이름은글자나하선 (-) 또는
콜론으로시작된다. 이름은글자, 숫자, 하선，
하이픈, 마침표, 콜론등이 사용된다. 콜론은
이름공간을 정의하는데 사용된다. 그리고
대／소문자에 관계없이 x, ＇끄, 7 등의 글자는
W3C가 선점해 놓았다．
■ 이름이 꼭 알파벳이나 라틴 문자라야 하는 법은
없다．
■ 특성과그것의 가치값들을표시하는방법에
대해서는 p28에 나와있다．
■ 스키마 (schema）
를 이용하여 어떤 태그가 XML
문서에 사용되는지 정의할 수 있다. 스키마에
대한 세세한 설명은 p67부터 시작되는 Part 3에
자세히 나와있다．
■ 작성된요소를뜻하는이름을사용한다면다른
작업시 편리하다．

26

"

1iger`

./name>

<name

슬래시

각괄호

그림끄0 단순한xML꾜소는 사작 태＝Z와 내용 정보（턱？Z：트나
다른요소를 포함하든자 또는 비아 있든지：)그리고 단자 사작 태그
의끝에／가 붙은 마침 태그로 1성되아 있다．
높m_' '_·ㄳrr(

2. 내용정보를작성한다．

"

태그

XML 문서에서는 원하는 어떤 요소도 만들 수 있다．
나중에 정보를 관리하기 쉽게 하기 위해 내용 정보를
나타내는 이름을 사용할 수 있다．

뽁

공백없는 요소 작성하기

노 code.HmI …

클

<endangered_species>
<cinimal>Tiger</animal>
</endangered_species>
그림i끄XML의모든요소는 루트 요소의사작 태L:z와 마침 태그
사아에 있다．

===== PAGE 26 =====
25 =====
Writing XML
올바른 요소（중복된 라인이 없다）

<name>Tiger 1<baby>cub</baby></name;
<name>Tiger <baby>cub</name></baby>
틀린 요소（태그들이 서로 엇갈려 교차되어 있다）
그림1.12 태그가올바르게 중첩돠었는차 알기 위ll저는 선으로
각칵의 묶음을 연결한다. 어딴 태그의 묶끔도 다른 묶음과 섶ㅇ／자
않았다면 각각의안쪽 묶음아 더큰 묶응과 잘봉합된 것이다．

요소의 중첩
가끔 각각의 파트를 정의하거나 그것에 관한 작업을
하기 위해서 큰 조각의 데이터를 작은 조각으로 나누
고 싶을 때가 있을 것이다．
요소들 중첩시키기：
1. p26의 1번과같이 외부요소의 시작태그를
만든다．
2. <inner＞를 입력한다. inner의 자리에 나누려는

귿銜葦금云횬즘존
「尋手三폭募륙7＝르

code.HInI

데이터의 첫부분 이름을 쓴다．
3. (inner> 태그의 내용정보를작성한다．

<name>Tiger</name>
<threab.poochers</threat>

4. </inner 2에서 만들었던 이름을inner자리에
넣는다．

<weight>500 pounds</weight>
</animal>

5. 2-4번을원하는대로반복한다．

</endangered_species>
그림i끄 animal 요소는우라가접근헤서ㅈ罹함수있는정보룰
포함한 서로 다른 세개의요소를포함하고 았다．

6. p26의 3번에 나온 것처럼 외부 요소의 마침
태그를만든다．

I, nm
■ 여기서 중요한것은각각의 요소가완벽하게
마무리되는 것이다. 다시 말해 안쪽의 요소가
닫히기 전에는 외부의 태그를 쓸 수 없다.
■ 원하는만큼 레벨의 요소들을분할할수 있다
■ 다른요소와중첩된요소는외부또는상위요소
의 하위요소로불린다．

예제의소스 코드는 sww.cookwood.c0m에 있습나다．

27

공呈＝ ．쯩킁＝ 쟎

<endangered_species>
<anim비＞

===== PAGE 27 =====
26 =====
Chapter 1

속성의 부가
하나의 속정은 요소에 텍스트를 넣지 않아도 부가적
인 정보를 만들 수 있다．

속성

<name language="English" 5 Tiger c/name>
가치값（인용 부호 안에）
속성 이름

속성 부기하기：
1. 시작태그를마감하기 전에이iribute＝를입력
한다. attribute자리는부가정보를정의하는
공간이다
2. 그리고나서 "value"를입력한다. value는부가
정보의 자리이다. 인용부호는 필수적이다．

등호 표시
그림끄4 족성온요소의사작 태그 안에 중첩되어 았는name
value의 한 쌍이다. 가치값은 인용 부호에 들어가 았어아 한다．
（큰 따옴표 또는 작은 따꼼표7.

回

즈－==5＝等義髥和拓三 mde, HnH 승，̀ 一 ' `

im

*
<
m
＝乞召
·
●
*
。
곰
，*

.' Tips

<endangered_species>
<animal>

■ 속성의 이름은 유효 요소의 이름에 非干칙과
.
같다 (P26 참조）

<name Ianguage="English">Tiger</name>
<name language="Latin'>panthera tigris.c/name>
<threahpoachers.c/threat>

■HTML에서와는 달리 속성값은 반드시 인용
부호 안에 있어야 한다．

<weight>500 pounds</weight>
</animal>

■ 우리는작은 따옴표나큰따옴표를쓸수 있다.
단 하나의 속성에서는 서로 매치되는 인용 부호
를 사용한다．
■ 가치값이 큰따옴표를포함한경우 가치값을
저장하려면 작은 따옴표를 적용한다. 예
comments='She said, 'The tigers are
almost gone!" '.
■ 주어진 요소에서 똑같은 이름을 가진 두 개의
속성을 가질 수 없다．
■ 어떤 속성도 외부의 엔티티 (p.58 참조）
에 대한
설명을 할 수 없다. 그리고 속성에서는 < 표시를
할수 없다. 부득이한 경우에는 그것을 대신
표현하는 표시인 씨t;를 사용할수 있다．
■ 일반적으로 속성에 포함된 정보는 요소의 내용
보다 덜 중요하다. 이것은 꺼）타 정보 劤eta
information)가 되는데, 다시 말해 내용에 대한
정보라고 할 수 있다．
■ 별개의 정보를표시하고 정의하는 다른방법은
p27에 나오는 요소의 중첩이다.

28

</endangered_species>
그림1.15 족정은 요소의 내용 정보를 부가할수 았게 한다．

===== PAGE 28 =====
27 =====
Writing XML
부두（:r

빈 요소 이용하기

<picture fiIename="tiger.jpg"/>

어떤 요소들은 텍스트를 가지고 있지 않다. 예를

슬래시와부등호
그림끄6 빈요소들은 여가 그림에저보둣이자작 태：Z와 마참
태＝Z틀 하나로 합쳐 놓았거나또는 독랍적인 아침 태＝z가 바로
연결된 하나의ㅈ］작 태그로 구성되어 았기도 하다．

F戚＝∼＝∼…＝∼

-

code.nrnl

一∼＝-

들면 '어떤 속성을 가진 사진 요소를 가지고 있다’
라고 한다면 거기에는 텍스트 컨텐츠라는 것은 없을
것이다．
하나의 시작 태그와 하나의 마침 태그를 가지고
있는 빈 요소 작성하기：

<endangered_species>
<animal>

1. <name을 입력한다. name이 있는곳에 빈
요소를 정의할 만한 단어를 입력한다．

<name longuage="English">Tiger</name>
<name longuage="Latin">panthera tigris.c/nome>
<threot>poachersc/threat>

2. 속성이 필요하다면p28에 나온방식에 따라
작성한다．

<picture filenome="tiger.jpg" x="200" y="197'/>
</animal>
c/endangered_species>
그림끄7 전형적안 빈요소들아란그들의족성들에 대한 더］이El만
포함하고 았는소스인 경우나 텍즈트가 0爬-/ 와부 이진법 El아E緡
자사하고 있는 사진 등을 의미한다．

3. /＞을입력하고요소작성을마친다．
분리된 시작 태그와 마침 태그를 가진 빈 요소
매1기：
1. <name을 입력한다. name이 있는곳에 빈
요소를 정의할 만한 단어를 적어 넣는다
2. 속성이 필요하면 p28의 방법에 따라 작성한다．
3. ＞을 입력하고시작태그를완성한다．
4. </name＞을입력하고요소작성을마친다．
1번에서 정의한 단어를 name 자리에 넣는다．

V 1ips
■XML에서 빈 요소 작성의 방법은 위의 두 가지
방법으로 가능하다．
■HTML에서와는달리 시작태그에 상응하는
마침 태그없이 시작 태그를 만들 수 없다. 그러
한 태그가 포함된 문서는 제대로 정리된 문서가
아닌 것으로 간주되어 XML 파서에서 에러가
발생한다．

혀）
群의소스 코드는 wwvi cookwood. corn에 있습나다．

29

．已＝ 山m크三뻑쓰m크m= =

<weight>500 pounds</weight>
<source sectionid=" 120"
newspaperid="21"></source>

===== PAGE 29 =====
28 =====
Chapter 1
각괄호 , 느낌표, 그리고두 개의 하이픈

주석달기
XML 문서에 주석을 다는 일은 문서 작성시 왜 특정
요소를 사용했는지 또는 언제 정보의 업데이트가
필요한지를잘 알기 위해서 아주유용하다. 방문자
에게는 보이지 않게 문서에 주석을 달 수 있다．

주센꽈

1. r<！·｀홑 입력한다．
2. 눙옇陪주석 내용을넣는다．
3. .-＞을입력한다．

V nP`

주석

·>
<!--updated May 3, 2001．
두개의 하이픈과각괄회
그림1.18 XML 주석은 ffTh 의주석과 같은 문장 구조를 갖는다．
麗琵뜨

·ㅌㅌ芦비m多므노od

Jim! =m

＝∼＝年

<endangered_species>
<animal>
<name language="English">Tiger</name>
<name language="latin">panthera tigris</name>
<threat>poachers</threat>
<weight>500 pounds</weight>
<!--the source tag references the carresponding article
on the World Wildlife Fund web site-->

■ 주석 사이에는 더블 하이픈 (--）을 쓸 수 없다
따라서 주적들은 중첩될 수 없다.

<picture filename="tiger.jpg" x="200" y="l 97"/>

■ 개발중이거나또는 디버깅 중일 때 XML코드
를숨기기 위해 주적을사용할 수 있다. 이것이
소위 말하는 "코멘팅 아웃 (Commenting Out)"
섹션이다. 이 코멘팅 아웃 섹션에 있는 요소들은
파서에는 보이지 않게 되고 따라서 포함될 쉬
있는 어떤 에러들이 일시적으로 화면에서 사라
지게 된다．
■ 미래에 있을 변화나 업데이트를용이하게 하기
위해서 XML 문서의 구조를 정리하는 데에도
주석은 아주 요긴하게 쓰인다．
■ 주석들은브라우저에서는보이지 않는다, 그러
나 XML 코드 안에서는 보인다．

3O

<source sectionid="120"
newspaperid=" 21"></source>

</animal>

=＝·ㅌㅌ。Um＝ 픈 多

■ 두개의 하이픈 (--）과주석 내용사이에는공간
이 필요하지 않다. 다시 말해서 <!－ㅎhisisa
comment--＞는 아주좋은 주석이다．

</endangered_species>
그림1.19 주석은 코드에 대한 정보를 더한다. 이것은 문저를 다시
볼 때또는 어떻재 만들어 겼는지보고자 할 때 uf/우 유용하대

===== PAGE 30 =====
29 =====
Writing XML
寞巨

F콰立르＝

code.urnl

<endangered_species>
<animal>

다섯 개의 특수 기호 작성법

<!--the source tag references the corresponding article
on the World Wildlife Fund web site-->

다음은 네임 개체를 이용하여 HTML 문서로 삽입될
수 있는 특수한 기호들에 대한 설명이다. 기본적으로
& 뒤에 이름이 오고 그 후에 세미콜론이 오게 된다．
XML에서는 단지 다섯 개의 개체들만 기본적으로
허락된다. 다른 개체들은 그들이 합법적으로 사용되
기 전에 DTD에서 미리 정의되어야한다．

<source sectionid="120"
newspaperid="21">c/source>

다섯 개의 특수 기호 만들기：

<picture filename="tiger.jpg" x="200" y="197"/>
</animal>

■ 앰퍼샌드 (&）를 만들기 위해서 &amp;를 입력
한다.
＾∼7

<name language="English">Tiger</name>
<name Ianguage="Latin">panthera tigris</name>
<threahpoachers</十reat>
<weight>&It;500 pounds</weight>

</endangered_species>
그림i20 ㅇ／문서가화면에 나타날때 &it;의깨제는 ＜르 표사된다．

■ 적다는 의미의 부등호 기호 (<）를 만들기 위해서
■ 많다는 의미의 부등호 기호 (>）를 만들기 위해서
&뎄；를입력한다·
■ 직접 인용부호
（"）를만들기 위해서&quot;를
입력한다．
'
■ 간접 인용부호나 (') 기호를만들기 위해서
進販엿；를 입력한다．
V Tips
U DTD (p55참조）
에서 미리 정하기 전에 다른
어떠한 개쳬는 쓸 수 없다．
■ XMT문서에서는태그를시작하거나개체를
시작하는 것을 제외하고는 < 또는 & 기호를 쓸
수 없다. 만일 태그나 개체를 사용하려는 것이
아니라면 위에서 설명한 방법으로 기호들을
표현하면 된다．
■ 그것들이 잘못 해석된 것이 아니라면 ", ', 또는
> 같은 기호들을 문서에 표시할 수 있다．
■ 간접 인용 부호와 직접 인용 부호를 함께 가진
속성값이 있는경우”, ' 기호 대신에 &quot사
＆아m$；를 입력한다. 가치를 포함하기 위해서
둘 중의 하나는 사용해야 하고 가치값에서 다른
것을 표현하는 개체를 사용할 수 있다．

예제의소스 코드는 www.cookwood.corn에 있습나다．

31

릎＝ ==.=<0샅m스。 留 클 口 묶

，쬈i읕입력한다·

===== PAGE 31 =====
30 =====
（가，
apter 】

문서내 요소의 표현법
XML 문서에서 요소와속성에 대해 파서 (parser:
구문 구조 해석기）
는 그것들을 해석하지 못한다．
대신에 보통의 문서에서처럼 그것들은 CDATA 섹션
에 있는 정보와 중첩될 것이다．
태그1텍스트로 나타내기：

l.cCDj3고입력한다．

2. 화면에 보이고싶지만해석은필요 없는요소，
속성 그리고 내용을 작성한다．
3. ]]＞를입력한다．

口

(eile.

<tags><appearance>
<I[CDATA[<endangered_species>
<animal>
<name language="English">Tiger</name>
<name Ianguage="Latin">panthera tigris</name>
<threat>poachers</threat>
<we1ghh500 pounds</weight>
<!--the source tag references the corresponding article
on the World Wildlife Fund web site-->
<source sectionid=" 120"
newspaperid="21"></source>
<picture filename="tiger.jpg" x="200" y="197'/>

*X곁m。 m섶● ㅌ으띱m＝ 吾 후 ＝

'/ nP`

</animal>

I

1]

CDATA 섹션의 좋은 사용은 0(;ML 자체에 대한
XML 문서 작성은 제외）CSS (Cascading Style
Sheet）
로 둘러주는 것이다 (p187'참조）
.

■ CDATA섹션은중첩될수없다．
I

CDATA 섹션의 모든 포인트는 기호로부터 특별
한 의미를 끌어내는 것이기 때문에 < 표시와 &
기호를（와 邑으로 쓸 수 있다. 이 경우 &It;나
&amp;라고 입력하면 안된다．

enH

（>
<xn기 bo아

c/endangered_species>
>

</appearance>.c/tags></xmLbook>
그림1.21예제에저 CDATA를 쟐제 코드로 해석하기 전에보기 위해
A陪했다．

노比叫

F효心t4`

工畔

汐

크

仝

S【여그

He寸m希

如1m

a

5eaC}`

ii

FaV口
＇

《기rn 구en씨cn= ; J
<xrni bo이傘
<ta닿5>
<appearanc.>
《 !ECD4T시

■ CDATA섹션은루트요소의 시작태그와종료
태그의 사이 어디서나 나타날 수 있다．

4；仕nJ楓r1댜ere凸

n

1nr『

（日1l나軫mr논
m M l已『눕q驪出다嶼ㄴ H可靭鱗l三h'tTtVetc/ heh亡＞
．빈r1楓n密 柚UHy소a S1' Tat 1V> p.et뇨SVS t 1gr 15<, Va,
＇rhr己mㄷ；
4才hre．
ㄷ.,1山acrier〃二

I

CDATA섹션을마치기 전에 어떤 이유引］
＞를
사용하고 싶다면 > 기호는＆gt;로 대체한다．
p31과 부록에 특수 기호 작성에 관한 더 많은
정보가 있다．

<veS弔｀
<US00 poUnd.-JeeLflt>
< 口－口m 寸口ur.e t흖q ref. r, iion

th

c rre石孕Cnd11띠 <;

4:4口Ume 三ee. 1r논r1그α｀나lㅍ口m nea5PaPerㅗd5- 노H: 치／密D뇌峯．
U
<Pㅗ.tUre

rnenaNC. 'nq之t .3Pg"

):."2(U'

V- h 」

'I ah魯Jm l >
</end,,,口er·d－日P·Cle鱗

］】＞

《／까pearanc.>
(/ ra. r,

l
그림1.22 인타넛／ 익스플로레 5.0 윈도우 파저를 아용해사
서 어떻7/f 태：z가 턱）즈트로
본 화면이다. CDATA 섹션어）
보여자는지 알수 있다. 반연에 onl_book, tag,
appearance 태＝Z 등은 허석된 상태로 보여지고 았다．

32

===== PAGE 32 =====
31 =====
PART 2:

DTD
DTD 만들기 35
요소 정의하기와 DTDOII저의 속성 41
DTD에서의 엔타티와표기법 55

33

===== PAGE 33 =====
32 =====
CREATING A DID
DID 만들기

스키마를 쓰는 두 가지의 주요한 법칙이 있다. DTD
와XML스키마가그것이다. Ufl〕(Document
는오래된 것이지만 특수하고 한정
吻pe Definition）
된 syntax와잘 어울리고 광범위하게 쓰이는 시스템
이다. 앞으로의 세 장에서 DTD 스타일의 스키마를
작성하는 방법에 대해 설명할 것이다. 새로운 유행인
XML 스키마는 W3C에 의해서 개발되었으며 p67
부터 시작되는 Part 3에서 세부적으로 다룰 것이다．

35

＾금口驪＝ 山。 。甘

스키마라는 것은 꼭 필요한 것은 아니라도 문서를
일관성 있게 만드는 데 중요한 역할을 한다. 어느
한문서의 유효화 하7/ (p244-245참조）과정에는
그것에 상응하는 스키마를 볼 수 있다. 만일 어떤
문서가스키마에 명시된 모든 干칙에 잘부합되었다
면 그것은 문서가 바람직한 모습으로 완성되었다는
것을의미한다．

朴

문서에서 요구되고 승인된 요소나 속정들을 구분하
여 이러한 언어들을 정의할 수 있다. 이러한 일련의
규칙을스캬마(schema)라고한다. 예를들면야생
동물보호자들은EndmL, 즉Endangered Species
Markup Language（위협받고 있는종의 마크업
언어）
를 만들고 싶어할 것이다. 이 시스템은 열종
위기의 종들에 대한 데이터를 위한 시스템이다．
EndML에서는동물, 비슷한종, 인구수, 그리고
위협 등의 요소가 있을 것이다．

瓣

전에 언급한대로, XML에서는문서를 작성한다고
할 수 없다. 대신에 XML을 이용해서 각자의 고유한
마크업 언어（공식적인 명칭은 xL 애플라케이션
이다）
를 작성하는 것이고 그러한 프로그램 언어로
문서를 작성하는 것이다．

===== PAGE 34 =====
33 =====
다iapter2

내부 DTD 선언하기

트·聾三

code.HmI

를
각각의 XML 문서에서는 XML 문서 안에 ㅁI,'）
만드는 방법이 가장 간단하다．

<!DOCTYPE endangered_species[

一－--＋∼一－- --m蕣

<?xml version="1.01' ?>

내부 DTD 선언하기：
1. XML문서 가장상단에 위치한xM.선언（p24
참조）이후에子!DOCTYPE ro아［라고 입력

한다. 여기서草萱f fo iyr17i茸좋：털
XML 문서에 루트 요소 이름을 넣는다．
2. 문서 타입을정의할내용이 들어갈빈공간을
남겨놓는다．
3. ]＞으로DTD를마친다．
'/ 1iPS

口
m
=：
口
＝
，●
＝ ＝
e
。 믄
。
●

에 대해
■ 여기에는재미있는 기술이 있다.DTI）
상세히 설명하고 있거나 DTD에 속하는 것을
문서 형식 선언 (document type declaration)
이라고 부른다. 물론 일련의 규칙의 집합을
DTD, 또는 문서 형식 쟝의 (documen比ype
definition)라고 한다. 이것들을 구분하기 위해
서는 ◇DOCIYPE으로 시작하고 〉로 끝나는
것을문서 형식 선언이라고 생각하면 된다, 〕yIl〕
는[] 사이에 들어 있는 일련의 규칙 집합이다．
(DTD도 별개의 파일이 될 수 있다. 그것에 관해
서는 p37에서 설명할 것이다.
■ 유효한문서가되기 위해서는상응하는DTI）
의
규칙에 잘 및아야 한다 (DTD가 외부나 내부에
있거나관계없이）
.

36

>

<endangered_species>
<cinlm이＞
그람 幻 여刀에 내부 DTD의 첫부분이 았다. 아것은XML 선언 후
xML 문저의 실제 태－그 전에 위치하게 된다．

===== PAGE 35 =====
34 =====
Creating a DTD
.de,dtd 驪二
<!ELEMENT endangered_species (anumj;

냉

<!ELEMENT anim비 ( name+, threats, weigh也 length?,
source, picture, subspecies+)>
<!ELEMENT name (#PCDATAI>
.c!ATTLIST name language (English I Latin)>

그림22 특정 선언의작성밥에 대해서는 다음 두 장헹저 다루가로
한다. ㅈ／금 중요한 것은 와부 i刃γ）의 규칙아 빈 텍즈트 문서의 위쪽
에서 바로 사작한다는 점ㅇ／다. 그라2 그들이ㅉ＇L 문저의 한부분
아 아닌 독립된 파일로 존재한다슨 것을 알마야 한다. 와부 D7丁）
파일은 .DTD 확장차로 저장하면 된다．

외부 DID 작성하기
만일 서로 관련이 있는 몇 개의 문서를 갖고 있다면
그것들을 모두 같은 ㅍ［I）
로 사용하기 원할 것이다．
ml）
를 각각의 문서에 복사해 넣는 대신에 ㅁID를
포함한 XML 문서로부터 문서의 URL을 알려주는
외부 파일을 만들 수 있다．
외부 파일 작성하기：
1, 텍스트에디터에새 파일을만든다．
2. 3장과4장에서 설명될 DTD의 규칙을정의한다．
3. 텍스트파일을 .毗d확장자로저장한다．

1// 1iF1
.

p38-40에서 외부Dn［〕
〕를이용하는방법과
이름 붙이는 방법에 대해 알아볼 것이다．
＝
。 。甘
芝＝ =＝山。 ＝m님4。 ，

역）제의소스 코드는 wsvw. caokwaod.corn에 있습나다．

37

===== PAGE 36 =====
35 =====
Chapter 2

외부 DID 이름 붙이기

외부 DTD 이름 붙이기：
1. 만일IyD문서가ISO와같은표준기준에
승인을 받았다면＋를 입력한다．
DTD 표준 양식에 맞지 않는 형식이라면·를
입력한다．
2. //Owner//DR》
를입력한다. owner의 자리에
DTD를 작성했거나 관리자나 회사명을 밝힌다．
*
口
， ●ㅎ
m
＝ 。…＝＝요＝ ＝。小， 。

3. label다음에공간을둔다. bb이자리에는IYPD
의 설명이 들어간다．
4. //XX/／라고입력한다. XX자리에는〕
)TI〕
가
적용되는XML 문서의 언어를 표현한 두글자의
약자가들어간다. 예를들면 EN이라는 의미는
English를 의미한다（다른 언어에 대해서는 跏
을보자）
.

1'Tips
■ 인터넷사이트（http://www.unicode.org/
unicode/onfinedat/language.htin))에는
ISO639에서 인정하는 두 글자 언어 약자의 공식
적인 리스트가 나와있다.
■DTD에서 이름은특정이나지정된URL대신에
라벨로서 〕y［〕
〕를 정의하게 한다. 이것은 lID를
찾고 있는 하나의 프로그램이 최신 버전이나
가장 보편적으로 쓰여지고 있는 버전에 속해
있다는 것을 말하는 것이다．

38

.

"
작斟

」살명

만일 UFD가 다른 사람에게도 이용된다면 FPI
(format public identifier를 이용해서 표준 방식
으로 작성한 DTD의 이름을 붙여주는 것이 좋을
것이다. 이 방법은 XML 파서 웹에 있는 퍼블릭 서버
에서 외부I)ID의 가장 최신 버전을 찾기 위해 FPI
를 사용하는 것에서 아이디어를 얻은 것이다．

언어

수직 기호가아님

-I/Liz Castro//DID'End_Species//EN/I
그림Z3 여가에는 멸종 위가의종 (Endangered Spethes)에관한
xM
【，
문서를 설명하고 았는DTD의공식적인 아름0/ 있다．

===== PAGE 37 =====
36 =====
Creating a DTD
妾．
：莩＝二土즈＝
＝스＝ㅍ－- code.Hrnl

<?xml version=" 1.0" standalone=- no ?>
<!DOCTYPE endangered_species SYSTEM
"http://www.cookwood.com/xml/examples
/dtd_creating/end_species.dtd">

<endangered_species>
<animal>
그림요4 아 예제에저는XM 문서를 정의하는 아ㄹL의와부DT瑨
사용한다．
code.,sml
醉－
<?xml version=" 1.0" standalone=' no"?>
<!DOCTYPE endangered_species SYSTEM
"http://www.cookwood.com/xml/examples
/dtd_creating/end_species.dtd"

개인적 외부 DID 선언하기
만일 특별한 개인적인 목적으로 DTD를 만들었다면
XMT. 문서에서 이것의 기원을밝히는 유일한 방법
은 URL을 사용하는 것이다．
1. 문서맨처음에나오는XML선언에서｀tanddone="no＂를 추가한다．
2. 쳉四g밧鑽핫라고입력한다· root자리에
는 이DTD가 적용된 XML 문서의 루트 요소
이름에 상응하는 것을 넣는다．
3. 외부ㅁfD가개인적이고표준적인DTD라는
것을 밝히기 위해서 SYSTEM을 입력한다.

]

5. ＞을넣으면서 문서 타입 선언을마친다．

>

I, 1:P
<endangered_species>
<animal>
그림2.5 원한다면DOCTYPE 선언의 끝에저 별도의 甲부 DTD
선언을ㅈ珊할수 있다. 별도의규착은 경좌 꽐：호 (TI) 안에 넣어아
한다. 로컬하게정의된 규칙들은 와부 파일으로부타 정의된 규칙을
무시한다．

예제의소스 코드는 www:cookwood.corn에 있습나다．

■ 만일 필요하다면 외부 DTI）
를 링크시킨 후에
（다시 말해 4번 이후에）별도의 내부 DIID를
추가함으로서 하나의 외부와 내부 DTD를 사용
할수 있게 된다. 그것들은 꺾쇠 괄호 세트 ([])
로 감싸져 있고 내부 DTD에 대한 보다 자세한
정보를 알고 싶다면 p36에 있는 내부DTD 선언
하기를 참고하면 된다. 내부 그
［D에 있는 子칙
들은 외부 DTD에 적용되는一干칙을 무시한다．

39

X
* 떻 금 。甘
。 m
。．＝。＝＝山。 ｛。，m。 ＝

[
<(ELEMENT continent lAsia I Europe I Africa)>

4. "file.dtd" 를입력한다. file.dtd자리에는DTD
의 위치를 지정하는 URL（절대적인 것 또는
상대적인）
을 넣는다．

===== PAGE 38 =====
37 =====
대apter2

공용 외부 DTD 선언하기

좇團ㅌ…

가매우 인기를 얻어
만일 위의 멸종 위기의 종 DTI）
그것의 수많은 복사본이 넓게 퍼져 있다면, p38에서
그것의 이름을 붙인 공용 식별자를 가지고 그것을
명명할수 있다. XML 파서가공용 식별기를 발견하
게 될 때 파서는 가능한 소스 중에서 가장 좋고 가장
최근 버전의 복사본을 얻으려고 노력할 것이다. 만일
를 발견하지 못한
파서가 공용 식별기를 가지고 IyIl〕
다면 URL을 이용하여 분류할 것이다．

<!DOCTYPE endangered_species PUBLIC

공용 외부 DTD의 기원짖기：
1. XML에서는문서 첫머리에＄tandolone="no"
를 입력한다．

m
＝ 。＝닐＝ =*七＝ 。·느。 *口느mㅎ

2. <IDOClYPE root를입력한다. root자리에
l끄D가 적용될 xM ' 문서 안의 root 요소 이름
을 넣는다．
3. PUBLIC을 입력한다. 이것을쓰는이유는DTD

芩注돋화되었고 이것이 XML 문서를坪청경尾
耳可苔척：흐E＝禧글r뉴因횰힘횰餉勒
위함이다．
4. "DTD_name＂을입력한다. DTD_name자리
에는】
y［〕
〕를 정의할 공식적인 이름을 입력한다
.
(p38 참조）
5. 'I계e.dtd∥를입력한다. file.dtd자리에는
에 관한URL이 있고 이것은 리모트
public DTI〕
서버에서의 위치를 알려주는 역할을 한다．
6. ＞로문서 타입의 선언을마감한다．

I, 1ip
■ 내부DTD를가지고외부DTE를무시할수
있다. 자세한사항은 p39의 Tip을 보자．

40

code.HmI

m겸

<?xml version=" 1.0" stondolone="no"?>
"-I/ Liz Castro//DTD End_Species//EN//"
"http://'..ww.cookwood.com/x세/examples
/dtd_creating/end_species.dtd">

<endangered species>
<anim비＞
그쾀요6 아번叩xML 파서는 공유 장소에사 zγm룰 사험하고
찾刀 위해서 공용 삭별가를 아용한다. 만일 아 사도가 성공척아차
않을 때는 주어잔 URL에서 정의된iγ1r를 ㅇ］용할 것아다．

===== PAGE 39 =====
38 =====
DEFINING ELEMENTS
AND ATTRIBUTES IN A DID
요소 정의하기와 DTD에서의 속성
2장 DTD 만들7／에서는 】)TL를 셋업하는 법을 배웠
다. 여기서는 이것의 컨텐츠를 어떻게 만드는가를
배울 것이다. 내부나 외부 〕)TD 작성시 XML 문서
에서 허락된 요소나 속성들이 무엇인지를 결정하는
규칙들을 살펴볼 것이다．

41

.
m
二
＝ `>=＝·＝4mm ＝。。甘
。。＝＝言쯩크。 ．

DTD에는 XML 문서에 나타날 모든 속성이나 요소
들을 정의해야 한다. 그렇지 않으면 그 XML 문서는
유효한문서가될 수 없다. 만일 XML문서에 어떤
요소를 더할 경우 관련 ㅍ［D에 그 정의를 넣어야만
.
한다（경우에 따라 새로운 】JTE를 만들 수도 있다）

===== PAGE 40 =====
39 =====
태apter3

요소 정의하기
XMT 문서를 어떤 특정 내용이나 구조안에 제하화고
싶다면 XML 문서 안에 있는 각각의 요소 구조나
내용을 정의해야 한다．

Li

l)de'd'd 릊三一＝
－두믈三욕2ㅗ二＝`1藍

<!ELEMENT endangered_species(animal)>
그림3.1XJvIL 문서에 나와 았는 각칵의모든 요소들을 정의할
꾈요가 았다. 여가서 endangered_species 꾜소는 단차 다른
하나의요소 欌nimalJ를 가ㅈ］고 있도록 정의되어 았다．

요소 정의하기：
1. <!ELEMENT tag를입력한다. 태그자리에 정의
하고자 하는 요소의 이름을 넣는다．

또다른하나는ANY를입력하는것이다. 이것
은 요소가 지정되어 있지 않은 요소나 텍스트의
조합을 포함하는 것을 허락하는 것이다．
3. 마지막으로＞로요소선언을마친다．
＝ㅌ●ㅌe= ＝口m灌＝ ＝·。

'/ YiP`
■ 속성들은 컨텐츠로 인식되지 않는다. 빈 요소
라고 해도 그것과 관련된 속성들을 가지고 있을
수도 있다 (P49 참조）
.
■ ANY를사용하는것은신중을기해야한다．
DTD의 가장 핵심적인 포이트는 하나의 요소가
포함함 수 있거나 포학하지 무하뷰 컷．
에 대호h干
칙을 정해주는 것이다. 각각의 요소가 어떤
것이라도 포함할 수 있다면 DTD를 모두 무시한
채 건너뛰게 하는 편이 더 나을 것이다. LYPD는
반드시 필요한요소는 아니다. 그들은 데이터를
일관되게 정리할 뿐이다．
UANY는 어떤 요소가 Un〕
에서 정의되지 않은
요소를 포함하는 것을 허락하지 않는다．

42

그람 3.22잔법 녜이E7를 가지고 았는요소들은 일반척으로
EMm'Y 선언된다. 왜냐하연그들은 어떠한xML 녜아타를 갖고
았자 않刀 때문아다. 대걔그들은 그들과 관란되아 있는 속정들을
갖고 있다 (p49 참조걋．

t de.dㅎd 三 =J-=＝른；三 느Fㅌ 1 - －三 ＝콩 〕
endangered_

species

帥
-<'ELEMENT

2. 만일요소가없는상태면EMPTY라고입력한다．
또는 (contents）
라고 입력해도 무방하다．
content 자리에는 요소를 설명하는 것과 요소가
포함하고 있는 and/or 텍스트가 포함된다. 반드
시 괄호를 입력한다. 이 변수에 관한 가능한
옵션은 p44-48에 나와 있다．

<!ELEMENT picture EMPTY>

ANY>

그랗 3.3 ANY 값은 사실모호해서 쟐저）직으로는 무용한 것아다．
XML 문서를 한정잣차 않을 바에는 모든 DTD를 건너뛰는 편아
나을 것아다. 아endangered_species 요소는a血/or 텍스트
와 다른요소들（아 요소들 역사 DTD에서 정의되어야 한다少을포함
할수 았다．

===== PAGE 41 =====
40 =====
Defining Elements and Attributes in a DTD
■ 하나의 요소는 다른 요소들을 원하는 만큼 포함
할 수 있다. 그래도 모든 요소는 반드시 한 번씩
은 정의되어야한다. DTD에서 정의되지 않은
요소는 유효한 XML 문서에는 나타나지 않는다．
■ 어떤 위치에 얼마나 많은 특정 요소가 들어가는
가는지 임의로 조절할 수 있다 (P48 참조）
.
■ 요소들을 선언하는 순서는 크게 중요하지 않다．
예를 들면 그 요소가 포함된 요소 선언 전에는
아무런 악영향 없이 하나의 요소를 선언할 수
있다．
■ 시퀀스를 이용하여 XML 문서에서 요소가 등장
.
해야 하는순서를 조절할수도 있다 (p46 참조）

■IYfl〕
선언은XMI요소가아니다. 따라서 이것
들은 〉로 마치기 전에 슬래시 (/）를 쓸 필요가
없다．

예자의소스 코드는 wwwcookwoocLcomo] 있습나다．

43

。．m三＝ ．。＝=m크m크＝

EMENT는
■XML은맞춤법에 민감하다. <！티．
반드시 이런 식으로 써야 한다. <！티emenㅎ라고
쓰는 것은 허용되지 않는다. 느낌표를 잊어서도
안된다. 물론 대／소문자를 섞어서 쓰는 것도
허용되지만 그 경우에는 먼저 그런식으로 정의
되었고 정확하게 그대로 사용한 경우이다. 어떤
때에는 전부 소문자를 쓴 경우가 더 쉬워 보일
때가 있다．

===== PAGE 42 =====
41 =====
Chapter 3

텍스트만을 포함한 요소 정의하기
XML 문서에서 어떤 요소들은 텍스트만을 가지고
있다. 주소라는 것은거리명, 도시명, 주 이름, 그리
고 번지수 등의 요소로 구성되어 있는데 주 이름의
(state) 요소는 단지 두 글자의 텍스트만을 가지고
있다（예 wisconsin WI).

ㅁ

츳섶믐三

=－∼－ -－ 트 c(}de.dtd죽컨出－ =

< ㄷLEMENT name (#PCDATA)>
<!ELEMENT weight (#PCDATA)>
<!ELEMENT threat (#PCDATA)>
그림3.4 대부분의DTD문저는 텍즈트만을가지고 정의된다．

c d已Hnn

요소 정의하기：
1. <!ELEMENT tag를입력한다. tag자리에는
정의하고 싶은 요소의 이름을 입력한다．

<name Ianguage="English">Tiger</nome>
<name language="Latin">panthera tigris</name>

。
*Xm눋＝ ＝。＝乞* =8。 **ㅌ읕● ＝＝。m＝ 융＝ ●

2. (#PCDATA）
를입력한다（괄호포함）
. 이 표시는
이 요소가 텍스트 컨텐츠만을 포함한다는 것을
알려준다．

＜十reat낫，
abitat destruction</十reat>

3. 마지막으로＞으로요소정의를마친다．

<threat>trade in tiger banes far traditional Chinese
medicine lTCMk/threat>

'/ Tips
■PCDATA는βarsed character data의 약자이
고 마크업 텍스트를 제외한 모든 숫자, 글자，
기호, 속성 등을 포함한다 (p55 참조）
.
■ PCIJATA를포함하도록정의된요소는다른
요소들을 포함할 수 없다.
■ 일련의 선택 중의 하나로 #PCDATA를 포함할
수 있다 (p47참조）
. 이것은 연속해서 사용할수
없다．
■DTD의 중요한한계는data를숫자, 날짜, 텍스
트, 또는 그밖의 것으로 한정 지을 수 없다는 것
이다. 다시 말해서 <YEAR>dragon</YEAR>
를 가지고 있는 XMl. 문서는 <YEAR>2005
c/YEAR＞과마찬가지로유효한것이다. 이것은
소위 정보 입력 (data typing）
이라고 하고 XML
스키마와 함께 사용이 가능하다．

44

首

<endangered_species>
<animd>

<threats>
<threat>poachers</threat>

<／什ireats>
<weight>500 pounds</weight>
그림昱5 아걋은name 요소가 텍즈트뿐인 유효한XML 문저에서
발췌한 것임을 주의하자. 각칵의threat 요소는 단순한 텍즈트안
반면에 threats는 아나다（아것은 텍즈트없아 threat 요소를
포함하고 있다）
.

===== PAGE 43 =====
42 =====
Defining Elements and Attributes in a DTD
巨口呼

code.dtd-

g

<!ELEMENT endangered-species (animal)>
.2림3.6 이정의에서는 아 endangered_species 요소는 하나의
animal 요소를 가질 수 있다．

刃__________________ tode.HmI ___________________可
<endangered_species>
<animal>
<name Ianguage="English">Tiger</name>
<name language="Latin">panthera tigris</name>
<threats><threat>poachers</threat>
<threat>habitat destruction</threat>
<threat>trade in tiger bones for traditional Chinese
medicine (TCMk/threat>
</threats>
<weighb.500 pounds</weight>

c/endangered_species>
그림 3. 7endangered_species 요소는 하나의animal요소를
포함하고 있는 반면에 이animal 요소의 컨텐츠는 아깃의 선언에
전적으로 의차한다. 또한 이endangered_species 요소의
선언에 영향을 받지 않는다．

어떤 정보를 작은 조각으로 나누려고 할 때 다른
요소들을 포함하고 있는 요소들이 있을 것이다．
하나의 자 요소1포힘하고 있는 요소 정의하기：
1. <!ELEMENT tag를입력한다. tag자리에는
정의하려는 이름을 입력한다．
2. (diild）
를입력한다. child자리에는정의하고
있는 요소에 포함되어 있는 요소의 이름을 입력
한다．
3. ＞로선언을마친다．

'/ nP$
■ 하나의 요소는 다른 요소들을 포함하고 있다．
이 의미는 DTD가 적용된 모든 XML 문서에
그 요소가 포함되어 있다는 말이다. 그렇지 않다
면 그 문서는유효한 것이 아니다.
■ 다른요소를포함하도록한정된태그는그요소
를 제외한 다른 요소를 포함할 수 없다. 또한
다른 요소를 포함하지 않을 뿐만 아니라 텍스트
도 포함할 수 없다.

여）
제의소스 코드는 www.cookwoo加orn에 있습나다．

45

＾。＝互 。
＝
e
^ ==

■ 자요소는 원하는 만큼의 많은 모요소들을 가질
수 있다. 각각의 자 요소와 모요소는 한 번씩은
정의되어야한다．

。
4

■ 자요소는선택적이거나여러 번사용할수있다.
더 자세한사항은 p48의 많은우낫을 정의하는
방법을참고하자．

。．m三＝ 口
口
＝ 쯩킁크*

</onimal>

하나의 자（아iild) 요소를 포함하고
있는 요소 정의하기

===== PAGE 44 =====
43 =====
Chapter 3
시퀀스를 포함한 요소 정의하기
간혹 어떤 하나의 요소는 일련의 다른 요소들을 포함
할 필요가 있다. 모요소 안에 포함되어 있는 일련의
자 요소들을 정의할 수 있다．
시퀀스를 포함한 하나의 요소 정의하기：
1. <!ELEMENT tog를입력한다. tag자리에는
정의하고 싶은 요소의 이름을 입력한다．
2. (child1을입력한다. d沚dl자리에는모뵤소에
처음으로 나타나는 첫번째 요소를 입력한다．

e
＝ ●弓瀷。 ＝
…
므
＝。
U
。 **ㅌ●ㅌ·＝＝口m＝ ㅌ＝●。

3. . 小i1d2를입력한다. child2자리에는모요소에
다음으로 나타나는 요소를 입력한다. 각각의
요소는 다음 요소와 하나의 콤마와 스페이스
공간으로 구별해 줘야 한다.
4, 모요소 내에 나타나는 각각의 자 요소에 대해
3번의 방법을 반복해 준다．
5. ）으로서 시퀀스를마친다．

릎目부휑叫 --

tode.dtd－

陋

<'ELEMENT animal (name, threats, weight, length,
source, picture, subspeciesl>
그림且8animal요소는 준저대로 나열된 각칵의요소들을 반드사
가자고 있어야 한다. 그라고 아것은 그밖의 것들은 가질수 없다．

肛∼

-

code.ilmi

<endangered_species>
<animal>
<name Ianguage="English">Tiger</name>
<threats>
＜小reot>poochers</threat>
<threa나abitat destruction</十reat>
<threat>trade in tiger bones for traditional
Chinese medicine (TCM}.</threat>
</threats>
<weight>500 pounds.c/weight>
<length>3 yards from nose to tail</length>
<source sectionid="lOl" newspaperid="21"I>
<picture filename="tiger.jpg" x="200" y="197"/>

■ 시퀀스에서 가장중요한것은콤마를찍는일이
다. 콤마라는 것은 시퀀스에서 요소들（요소의
무리들）
을 구분하는 기호이다.

<subspecies>
<name language="English">Amur or
Siberian</name>
<name language="Latin">P.t. altaica</name>
<region>Far East Russia</region>
<population year=" 1999">445</population>
</5祉）
spedes>
</animal>

■ 시퀀스안에서는＃PCDATA를사용할수없다．

</endangered_species>

■ 시퀀스안에포함된요소들은다른요소들을
포함한다. 그림 3.9에서 보면 threats 요소는
각각의 threats 요소들을 포함하고 있다．

그림 3.9 유효한x기kf【』문저에서는각각의요소가 하나싹 있다는
것을 주의해야 한다. name 요소는 두 번 나올 수 없고 subspecies
요소도 한 번 아상 나오자 꼿한다. 그라나p48에서는 여a/ 번등창
하는 경우툴보게될 걋아다．

'/ 1iPS

■ 또한 각각의 유닛이 하나의 요소이든（괄호내의）
요소들의 선택이든（괄호 내의）
, 일련（시퀀스）
의
요소들이든 유닛들의 일련（시퀀스）
을 만들 수
있다．
■ 각각의 시퀀스 안에 있는 각각의 유닛은 나오는
.
횟수를 정의해야한다 (P48 참조）

46

===== PAGE 45 =====
44 =====
Defining Elements and Attributes in a DTD
刃∼交르숫숫穫궂

code.dtd…흩

<'ELEMENT characteristics ((weight, length) I picture)>
그람 3.10 이보기에서는 characteristics 요소는weight
요소, length요소 중에서 선택한 깃 중 하나와picture요소를
포함하고 있다．

하나의 요소를 가지고 하나 또는 다른 요소를 선택
하는 권리를 포함하는 경우는 흔한 경우이다．
하나의 요소의 컨텐츠에 대한 선택권（比oice)
정의하기：

小輾護權盡毒codejeni
룔．

纛긍＝二－ →弘＝=＝ㅍ∼∼∼1唯

<d1aracteristics>
dength>3 yards from nose to tc川＜기ength>
</characteristics>
뇨 , , , ` tod8Mm! 毓 `,"

` → 小∼，

1. <!ELEMENT tag를입력한다. tag자리에는
정의하고 싶은 요소의 이름을 입력한다．
2. 岫ildi을입력한다. 다른것이 나타나지 않는
다면 childi 자리에는 처음 요소를 입력한다．

<weight>500 poundsc/weighb.

三圈＝ 료＝二＝三딥- -

선택권 정의

m筌

<characteristics>
<picture fi(ename= 'tiger.jpg" x="200" y="197"/>
</characteristics>
그림3.11여가에 았는 두 가자의 x74L 보기는 완벽하게 유효한 것
들아다．

3. I- 입력한다. 이것의 기능은만일첫번째요소
가 나타나면 두번째 요소가 나타나지 않는다는
것을 알려주는 역할을 한다（그 반대의 경우도
마찬가지）
.
4. 小∥d2를입력한다. 만일다른것이 나타나지
않는다면 child2자리에는 나타날 두번째 자
요소를 적는다
5. 선택권이 나올때마다3-4번을반복한다.

<characteristics>
<weight>500 pounds</weighb.
</characteristics>
口

!

辛CodeM쫠1"

<characteristics>
<weight>500 pounds</weight>
<Iength>3 yards from nose to tail-c/length>
<picture filenome=「tiger.jpg" x='200" y="l 97"/>
</characteristics>
그림3. z2 여기에 았는 두 개의XML 보가 모두 다 유효하자 않은
것이다. 첫번째 깃은weight와length 요소를포함해아 하는
데weight 요소만을포함하는오류를 범했고 두번째 것은 하나의
선택만 했어야 하는데 두 걔의요소를 다 가지는 오류를 범했다．

예群의소스 코드는 www.cookwood.corn에 있습나다．

6. I을 입력하여 선택의 구문을마친다．
7. ＞으로요소선언을마친다．
V 1iPS
■ 어떤 요소에 많은 선택을 할 수 있게 만들고
싶으면 위의 6번을 실행한후에 *를한다. 이것
은 모요소 안에 속해 있는 정돈되지 않은 리스트
를 정의하는 방법이다 (p48 참조）
.
■ 첫번째 선택은＃PCDATA가될 것이다. 사실
혼합된 컨텐츠를 가지고 한 요소를 작성하는
것이다. 그러나 앞의 Tip에서 밝혔던 것처럼 *를
넣을 필요가 있다．
■ 또한 각각의 유닛이 하나의 요소이든（괄호
안의）요소들의 선택이든（괄호 안의）일련（시퀀
스）
의 요소들일 때 유닛들 사이에서 선택할 수
있다．

47

。
m
＝三
＝ ．우。 ｛
g

럴1蝕七눗｀
七＜t＝七｀
`-＝느＝c.de.11n"

===== PAGE 46 =====
45 =====
Chapter 3

많은 유닛 정의하기：
1. 요소선언의 컨텐츠부분에서 내it이라고입력
한다. wit자리에는 하나의 요소, 두 개 이상의
（괄호가 쳐져 있는）선택문 또는 괄호가 쳐져
있는 요소들의 시퀀스가 올 수 있다．
2. ？가오는 경우에는요소를정의하는과정에서
유닛이 기껏해야 한 번 정도 온다는 의미이다．
＋의 의미는 요소를 정의하는 과정에서 유닛이
적어도 한 번 이상, 원하는 만큼 많이 올 수
있다라는 의미이다.

==>＝을뇰윤m= ＝
●
。

*의 의미는 요소를 정의하는 과정에서 유닛이
필요한 만큼 많이 나오거나 또는 나오지 않을
수도 있다는 의미이다．

V Tips
■ 주어진 유닛의 특정 갯수를 정의하는 좋은 방법
은 없다. 만약세 개를 정의할 경우 다소 조잡한
표현 방법은 (unit, unit, unit+）를 사용하는 것
인데 이것의 의미는 적어도 세 개의 유닛이 필요
하고 그 이상의 것도 가능하다는 의미이다．
■ 괄호 안에 포함되어 있는 선택들에 적용된 별 (*)
모양 표시는 그 요소가순서에 관계없이 개별
선택의 어떤 수량을 포함하고 있다는 의미이다．

48

－杜＝x논注∼

code.dtd 繁4三驀：一一韆별戚一m

<IELEMENT animal (name+, threats, weight?,
length?, source, picture, subspedesi>
그쾀3.13수량계 (quantifier는 선언을 더욱우연하게 만든다．
위에서보둣이animal 요소는 적어도 하나（그라고 유한의 줏자）
의이름요소를 가ㅈ］고 있다. weight와length 요소는 섕략돨
수도 있고 나올 경우 최대가在7에 한하따, subspecies 요소의
등장 홧수에는 제한아 없다슨 의口／이다. 그러나 둥창하자 않마도
무방하다. 그 밖叩threat, source, picture 요소들은 정확
夕
하게 한 번싹등장할 것아다. 이값아 다폴트값아다．

「． c0de.dtd
…cede.dtd拌虹
I阿，筐．
，∼．
=－「「．
.1
.1 --_
阡’
筐可느 ` , 광亡느三X｛三｛二言；
＝큐m

" CLCmㄷ

I nlreaTs(rnrear, Inrear, Tnrear-

J>

DTD에는 하나의 요소에 나오는 요소들의 숫자를
표현하는 세 가지 특별한 기호들이 있다. 하나의
유닛은 하나의 요소가 될 수도 있고, 두 개 이상의
요소의 선택이 될 수도 있고 또는 요소들의 시퀀스가
될 수도 있다．

훑目= 三三三三一毛三＝

1-

많은 유닛을 정의하는 방법

켜

그람314 threats 요소는적어도세개의threats 요소를
포함할것아다. 아의마는무한의줏자도포함된다는깃아다．

===== PAGE 47 =====
46 =====
m-

e d·．H11H
year= " 1999">445<

속성에 관해서
/population>

-<population

)

Defining Elements and Attributes in a DTD

에dejmd

<population>
<year>l 999</year>
<quantity>445</quantily>
</population>
그랖 3.15 두 ifi의XMl 코드 모두 같은 정보릍 가자고 있다. 그
정보는1999년에445아라의ㅈ／버7라아 야섕호랑아가 냠았다는
정보아다. 차아점은 정보가 어떻게조쟉되아 았는가 8＇는 것ㅇ／다．
위의예켜］
에저1999는족정값하다. 밑의예처］
에서는1999와445
둘 다 각칵의 다른요소에 있는 컨텐츠아다. 두 방식모두 유효한
깃아다. 선택은독ㅈ搢의몫아다．

하나의 요소를 더 작은 정보의 덩어리로 만들 수
있는 반면 가끔 추가 데이터를 요소의 컨텐츠에 넣는
대신에 요소 자체에 직접 넣는 것이 더 유－용할 것이
다. 속성이 하는 일이 바로 이런 것이다．
속성에 포함된 정보는 XML 컨텐츠 부분에 대한
것이 아니라XML 컨텐츠에 대한 것이다. 예를 들면
멸종 위기의 종 (endangered species) 데이터 베이
스에서 name 요소는 name 요소의 컨텐츠 안에 있는
언어를 설명해 주고 있는language 속성을 가지고
있다.
우리는 이미 각각의 요소 안에 같은 정보를 포함시킬
수 있다. 그 name 요소는 하나의 language 요소와
하나의 local_name 요소를 포함할 수 있다. 두 가
지 방법 모두 무방하다. 요소들은 보여주고 싶은
정보에 적합한 반면 속성은 정보에 대한 정보에 더
적합하다.

예젱의소스 코드는 www.cookwooi.c0m어］있습L幷／;

49

＞口。 드 >==g言m

속성은 빈 요소와많은 공통점이 있다. 왜냐하면 그
들 모두 요소의 컨텐츠를 설명하고 있기 때문이다．

===== PAGE 48 =====
47 =====
Chapter 3

간단한 속성 정의하기

콥r그

속정이 DTD 안에서 선언되지 않았다면 하나의 속성
은 XML 문서에 나타날 수 없다．

<!ATTLIST population year CDATA #IMPLIED>

속성 정의하기：
1. <!A11LIST tag를입력한다.tag자리에는속성
이 나타날 요소의 이름을 입력한다．
2. .卄ribute를적는다. attribute자리에는tag에
넣고 싶은 추가 정보의 이름을 입력한다．
3. 만일속성값이 태그가없는문자들의 조합으로
이루어 졌다면 CDATA를 적는다（괄호 또는 #n
이 없는 것에 주의해라）

＝ 。。
m
0
*．
욘
， =＜읖ㅌ am= i

또는（dioice_1 - m永e-2 ）를입력한다．
choice_n 자리에는 XML 문서에서 유일하게
사용된 속성의 가능한 값들을 넣는다. 각각의
choice는끝에 붙어있는하선 ( ）에 의해 L분이
되고 이 모든 것은 괄호 안에 놓여진다．
4. "defa이t"를입력한다. default자리에는만일
명백하게 정해진 것이 없다면 디폴트값이 속성
값이 될 것이다．
또는＃FIXED"defa이1"를 입력한다. default
자리에는 디폴트값이 들어가고 이것으로 속성
값을 가지고 싶을 때 입력한다．
또는＃REQ내RED라고 입력한다. 이의 의미는
속성값이 어떤（미리 정의된 값은 아니다）값을
갖는다는 의미다．
만일 속성이 디폴트값을 가지고 있지 않거나
완전히 생략될 경우＃IMPUED라고 입력한다．
5. 요소가포함하고 있는 각각의 속성에 대해ㅏ
번을 반복한다．
6. ＞으로서속성 선언을마친다．

Code.(nd

<!ELEMENT population (#PCDATA)>

그림 3.拓 아 속정 정의는population 요소가 글자들의 어떤
조합 (CDATA 때문에｝
을 가치고 있는year 족정을 선택사항
(#IMPIJED 때문이
【L으로 포함하고 밌어야 한다고 말하고 았다．
code.Hn넒 뛸ㅌ느
.
<population>445</population>

區

흩
＇ 二－-=.｀工쏘∼∼－mJ－프꾜小 c.de.1n1H 疊∼‘一그；

三．
톨

<population year="1999">445</population>
c쨍》de.'111,1；꾜；
=＝三三＝5三즈g｀
寸三＝ 4

<population year="of the
Rabbit">445</population>
그림 3.17.2림 3.16에 나와있는DTD에 따르면세개의xML
문서는모두 유효하다. 왜냐하연year 속성은 선택사항야고
(#IMPIJED) o/것의 컨텐츠는 이딴 글자들의조합도 가능하기 때문
O1다. 하나의족정의가치값까 쟐제의 일년아라는 것을확실하 할
수 았는 방빕은 없다는 깃을 주의11라. 아것을 위해XML 스7／마가
필요한 것아다 (p69 참조？.
[j

c0de.d'd

<IELEMENT population (#PCDATA)>

미

<iATftlST population year 11999 I 20001
#REQUIRED>
서는year 요소 1999 또는 20刀에 았는
그림3.18 아 예제이］
population 족성의가차값이）두가차 가눙성만을 하락했다．
아 선뱍들은 수칙 바 (bar). 나뉘어진 꽐호 안에 나타난다. 족성은
설정되어 있어야 한다 (211냐하면 #REQUIRED 값아가 때문이다）
.

：口

tode.Hml

<population year='1 999">445</population>
cocle.I4mI
m1de
.ㅐrlH 奴* -平쌥＝솟＝e授∼三 ＇ 큘
pulation>
=f그

－듣小code. irnd t느三르44三－=:i뀁＝＝드붇兵5;

<pop이ation year="1998">445</population>
그림3.19 이세가자 XMl 예중에서그림 3.18/i DTD0// 대해서는
맨 위에 았는 예제만이 유효하다. 중간의 예제는#REQU1RED 음
에도 불구하i2year 속정을 잊어 버렸기 때문에 유효하차 않다．
맨 밑의 예제는 1998아 족정의 컨텐츠에 대한 허락된 선택이 아1.7
었기 때문에 유효하자 꼿하다．

50

===== PAGE 49 =====
48 =====
Defining Elements and Attributes in a DTD
口
COde. dtd
<!ELEMENT population (#PCDATA}>

騙

<!A1TLIST population year CDATA "1999">
2림3.20 아번에는year 족성에1999의 다폴트값을 넣어보았다．
력

三톺code.m01

<population year="1998">445</population>

.

口
c0de.HnH
<population>445</population>

回l릎

2림3.班 세개의XML 예경）
는꼬두 유효한 것들j/다. year는
어딴 값으로 설정되어도 괜찮고 심지ㅇ7는 생략되어도 무관하다．
훙아로운 부분은 값이 섕략된다면 세번째의 예졔처럼파저는year
족성아 아차 현존하는 것ㅊ／렁 그리고 그것의값이1999.u 설정된
것처럼 작동한다．

code.dtd 쏘ㅍㅎ쑈르＝=＝흐六三＝勉ㅊ노型좋

<lAiTLIST population year CDATA #FIXED "1999">
그림3.22 고정된 값은 아것이 실제XML 꾼저에 나타나든 아나든
하나의속성아 주아진 값을가지고 있다는 깃을확신사7］
는녜우용
甲：뀌
ㅁ
code. 村1n
<population year="1 999">445</population>

凹

邏饔 Cod ．ㅐnH
口
<population year="1998">445</population>

彗旺

톺

그림3.23 이예제들은 그림 3.21에보여진 것들과 같은 깃들아다．
그림3.22에 나오는 DTD가 유효하다면 어깼든 중간의 예제는 유효
하치 꼿하다. 족성아 설정되어 았다면 속썽은 1999값을 가차고
있어야한다 (1998아 아나고 다른글자들아 아나라？. 밑의 예제를
보면 파서는 마차year 족성
（汕999- 설정되어 있는 것으로
동작을 한다．

p52-53에 설명되어 있는ID, IDREF, IDREFS
와p54에 설명된 NMTOKEN, N1OKENS
등의 여러 가지 특별한 종류의 속성값이 있다．
다만 엔티티 속성의 ins와 outs는 4장 DTD에서
의 엔타타와표기법이전에는 언급되지 않을 것
이다．

■ 어느속성값을디폴트값으로정의했을경우
만일 그 속성이 xM. 문서에서 명백하게 정의
되어 있지 않다면 XML 파서는 디폴트값을 자동
적으로 첨가할 것이다（그림 3.21).
■#FIXED"defa이ㅎ＂를 가지고 하나의 속성을
정의한다면 XML 문서의 속성값은 디폴트값으
로 맞춰 주어야 한다. 만일 그 속성값이 맞춰져
있지 않다면 그 파서는 자동적으로 디폴트값으
로 정할 것이다（그림 3.23).
■ DTD가＃REQ내旺D로정의되었지만그것에
상응하는 XML 문서가 그 속성에 대한 값을
갖고 있지 않을 경우, 제대로 작동되는 파서는
에러값을발생시킨다．
■ 파서는또한XML문서에서 자동적으로 맞춰져
있지 않은倒M더」
ED로 정의된 속정에 관한
정보는 돌려주도록 되어있다．
■ 속성 정의의 모든 부분에서 대문자, 소문자는
엄밀히 구분된다. 이 책에 나와 있는 대로 입력
하는 것이 옳은 것이다. #Required와같은 것은
DTD에서는 아무런 의미가 없게 된다．
■ 디폴트값과＃REQ내RED 또는쒸씨；)LIED 등은
혼용할 수 없다．

예제의조스 코드는 w￦W. cookwood.corn에 있즙나다．

51

。．出三＝ 山蠟 크七＝ >==r言m

<lELEMENT population l#PCDATA)>

C0de.H'n1
口
<population>445</population>

■ 하나의 리스트에 있는 각각의 선택은 반드시
유효한 XMl. 문서騙干칙을따라야 한다 (p26
참조）
.
■ 하나의 속성 선언에서 모든 속성을 선언하거나
(5번에서 설명했던 바와 같이）아니면 각각의
속성에 개별적 속성 선언을 만든다．

codej4ml－一口줄

<population yeor="1999">445</population>
□

'/ nP`

===== PAGE 50 =====
49 =====
C比pter3

특정 값을 가진 속성 정의하기
특별한종류의 속성들이 있다. ID 속성들은 XML
문서에서 고유한（반복되지 않는）값을 갖는 것으로
정의되어 있다. 하나의 ID 속성은 검색표나 정체성
정보（상품 코드, 소비자 정보 코드 등）
에 아주 이상
적이다．
止》속성 정의하기：
1. p50의 1-2번을따라한다．
2. 만일 X｝
札문서안에서 가치값이 고유하고반복
적이지 않을 가치값을 원한다면 ID를 입력한다，
다시 말해 어떠한 다른 요소들도 똑같은 값을
갖지 않는다는 의미이다．

[m퀘

tode.dtd릊三

<IELEMENT animal (name+, threats, weight?,
length?, source, picture, subspecies+)>
<lATFUST animal code ID #REQUIRED>
그림 3.24 XL 문서이］
저특청요소를 정의 하기 위해서 JD 타입
속성을 만들려 한다면ID 속성을 팔요로 하는 것은 좋은 생각이다．

三｝

<animal code="Tl 4i >
<name language="English">Tiger</ncime>
</animal>
<animal code=∥BRr"

>

<name language="English'>Black Rhino</name>

</animal>

3. p50의 4-6번으로속성 정의를마친다．
·
e
= =＞●二！ =＝三灌m● *＝곰， =＜。 灌＝ ＝·。

V Tips
lID 타입의 속성이 그 속성들 가운데 같은 값을
가지고 있다면 그 문서는 더 이상유효한문서가
아니다．
■ID 속성의 가치값은유효한XML 문서 이름에
적용되었던 같은 규칙을 따라야 한다. 다시 말해
가치값은 글자나 밑줄로 시작되어야 하고 그 후
에 추가글자, 숫자, 밑줄, 마침표, 하이픈이
올 수 있다는 규칙이다（이 의미는 하나의 ID
속성값은 단순히 주민등록번호나 전화번호와
같은 숫자의 조합이 아니라는 의미다）
.
■ 속성 타입에서 ID를 사용하는 것은 고유한
NvffOKENs를 사용하는 것과 같다 (p54 참조）
.

52

퓰l크三－

<anin洲

꽉 ∼→끈＝

code.eml

∼二＝ /，∼1,

∼二브曹측

>

<name language="English"> Tiger</name>
</animal>
<animal Jae= T143">
<name language="English">Black Rhino</name>
</animal>
.2림3.25.2림3.24에 보여진 DTD에따르면 이cade 족성은
겨｝는
XA 문저를통해저고우한값을가져야만 한다．첫번째 여）
유효한 것이고 둘째는 유효하지 못하다．

===== PAGE 51 =====
50 =====
Defining Elements and Attributes in a DTD
J:j

cnde,dtd 囊立

陋를

<lELEMENT specialized_website (title, un)>
<'AiTLIST specialized_website
#REQUIRED>

n DREF

그림3.26 어느 특정동물에 관한 웹사이트를 찾슨XML 문서에
있는 하나의요소를 상상해라. 동꿀의코드와 웹사이트를 연결사카
는 데에는IIJREF를 사용한다．

고유값으로 속성 설명하기
p52에서 정의했던 ID 속성에 속하는 가치값을 갖고
있는속성을IDREF라고한다. IDREFS속정은
문서의 끄〕속성 안에서 발견된 빈 공간으로 나뉘어
진값들의 목록을 포함한다．
속상I과 고유값 연결시키기：

른1J

\

－→－

code.)mI

그림3.27 하나의IDREF 타입속성은 문서 어단가에 하나의 zD
타입족성을 가，
(］
고 았는 가차값을포함하고 았아아 한다（예를
들딴p52에 나오는그림325의 위쪽 예제를보라). 하나 이장의
specialized_website 요소는 animal_focus " f
대한 같은가치값을가질치도 모른다．
회53

c{}de.dh1

<!ELEMENT general_website(title, un1)>
<!ATTLlST generol_website contents IDREF5
#REQUIRED>
그림 3.28 일련의ID 값둘을포함하고 밌는 IDREF 타입 족성들을
이우해라．

code.Hmt

在：甚壅＝＝탭丘하l石…

1. 속성 정의를시작하기 위해 p50의 1-2번을
따른다．
2. 다른속정의 II）
가치값과상응하는가치값을
포함할 속정을 정의하려引DREF를 입력한다．
몇몇의 빈공간으로 나누어진 ID 가치들을 포함
하는 속정인 경우에뉘DREFS를 입력한다．
3. p50에나온4-6번으로속성 정의를마친다．
'/ 1iPS
■ 만일 DTD가ID 타입의 속성 정의를 포함한다고
한다면 IDREF 타입으로 속성을 정의하는 것이
규칙에 맞는 것이다（β52 참조）
.
■ 같은 ID에 기인하는 여러 개의 IDREF 타입
속성들이 존재하는 것이 가능하다는 것을 주목
하자（그림 3.27). 하나의 요소에 하나씩만 가져
야 하는것은 단지 ID 그 자신일 뿐이다．
■ 하나의 IDREFS 타입 속성 내에서 반복되는
아이템들은 존재하지 않는다. contents="1143
1143 1143＂과같은 것은 원하든 그렇지 않든
파서에게는완벽하게 유효한 것이다. 요소와
속성 컨텐츠의 제어력을 더하기 위해서는 XML
스키마에 잘 호응하는 DTD들 을 포기해야 한다
.
(p67'참조）

t5='T一 O735 BR4 >
<gener히－website1
<title>World Wildlife Fund</title>
<url>http://www.worldwildlife.org/.c/url>
</general_website>
그괌 3.29 하나의IDRE'F 타입족성은 반드사 하나 아장의 빈공간
으로 나뉘아진 가차값들을 포함하고 있어야 한다. 각각의 것들은
같은 문서의 어딘가011w 타입족정들에포함되어 있ㅇ7아 한다．

예제의소스 코드는 wwe cookwood.com에 있습나다．

53

召* m, .＝슥＝ 썹＞ =＝口됴m· 트 芬 ． ＝￡．。＜。 ＝ '

<resources>
<specialized_website onimal_focus="1143">
<title>Tigers in Crisis</title>
<url>http://www.tigersincrisis.com/.</url>
</specialized_website>
<specialized_website onimal_focus=「T1 43">
<title>ligersl</title>
<url>http://www.geocities.com/RainForest/6
612/c/un>
</specialized_website>
<specialized_website animal_focus="O735">
<title>InternationaI Otter Survival Fund</title>
<url>http://www.otter.org/</url>
</specialized_website>

===== PAGE 52 =====
51 =====
다1apter 3

유효한 XML 이름 속성 제한하기
DTD는 많은 양의 정보 입력을 허락하지 않는다．
그러나 속성에 적용할 수 있는하나의 제한 조건이
있다. 그것은 바로 가치값은 유효한 XML 이름이어
야한다’ 는 것이다. 다시 말해 가치값은 하나의
글자나 하나의 하선 (-）으로 시작되어야 하고 그것은
단지 글자, 숫자, 하선 ( ）들, 하이픈, 마침표만으로
구성되어야 한다는 것이다．
유효한 XML. 이름의 규칙읖 따라가는 속성값
정하기：
1. p50의 1-2번을따라한다．
2. 만일 가치값이 p26에 정의된 것처럼 XML이름
이 되고자 한다면 NMTOKEN을 입력한다.
·●ㅌ。＝H宅님겯i＞ 오m● 섭손느* *<m= ===m곁

또는 속성의 가치값이 빈 공간으로 나누어진
（타1s라고
XML 이름 목록을 원한다면 NMT이
입력한다．
3. p50의 4-6번으로속성 정의를마친다.

'/ Tips
U NMTOKEN 타입 속성은 절대 빈 공간을 포함
하지 않는다. 이것은 이러한특별한 타입을 사용
하는 좋은 이유가 된다．
■ 만일 어떤 하나의 속성값이 유효한 XML 이름인
동시에, XM. 문서 중에서 유일한 것을 원한다
면 NMTOKEN을 쓰는 대신에 ID를 사용하는
.
것이 좋을 것이다 (P52 참조）

54

t0de.dtd

<lELEMENT appearance (#PCDATA)>
<!AflhIST appearance most_prominenL color
NMTOKEN #IMPLIED>
.2림3.30 ㅇ／렇게 만들아잔 예제 인쩽저는most_prominent
color의한 단어값을포함한 나의동물의간단하고 정확한 설명
을 원한다. most_prominent_color 족성의값을 한 단어
（빈 공간없이屆 만들가 위해서는N玉fJOKEN 타입을사우하는
것아 좋을 둣 싶다．

c de.1섶 1

「그

<appearance mOst_prominent_colar="orOngeU>
The might tiger is typically orange with black stripes
and some white hic少1lights.
</appearance>
뜨，Code.出lH 멨근G섶슨3편늦囊疊솟i烈욤三

<appearance most_prominent_color='dark orange">
The might tiger is typically orange with black stripes
and some white highlights.
</appearance>
그림 3.31첫번째 예제만하 유효한 문장이다. 왜냐하면 두번째 예제
에서는most_prominent_color 속성아 가차값혀7 하나의
공간아 았기 때문에유효하자 꼿한문장ㅇ／ 되었다．공간은
NMTOKEN 타입의족성에저사용해서는 안된다．

===== PAGE 53 =====
52 =====
ENTITIES AND

NOTATIONS IN DTDs
DID에서의 엔티티와 표기법
Entities（개체）

Parameter（인자 )U떼
/\\

internal（내부）external（외부）
General（일반》
//-\\\

intern히（내부） extem이（와부）
///

\＼∼∼

parsed（파스된 것） unparsed（파스되지 않은 것）

여러 가지 종류의 개체들이 있지만 그들 모두는 같은
방식으로 작동한다. 차이점은 개체가 어디서 정의
되었고 어떤 종류의 정보를 포함하고 있는가에 달려
있다．
개체들은두가지의 큰그룹으로나누어진다. 일반적
인 개체들과 인자 개체들이다. 일반적인 개체들은
XML 문서 자체로 데이터를 전달하는 것이고 인자
개체들은 I丑D의 일부분이 되어 데이터를 설명하는
것이다．
일반적인 개체들은 외부와 내부로 분리될 수 있다．
DTD에서 그것들이 정의되는지 또는 외부에서 정의
되는지에 따라 결과적으로 외부 개체들은 파스
(parse) 될 수도 있고 그렇지 않을 수도 있다. 파스된
개체들은 XML 문서에서 XML 파서에 의해 분석되
어 진다. 파스되지 않은 개체들 - 일반적으로 텍스
트 데이터가 아닌 이진법 데이터 - 은 파서에 의해
분적되지는 않는다.
인자 개체들은 언제나분석 (parse）
된다. 이 개체에
도 내부 개체와 외부 개체가 있지만 내부 개체들은
한정되어 있는 이유로 여기서는 외부 개체를 중심
으로 설명한다 (p60 참조）
.

55

m= *
=
r
m 。
＝
` ＝
。
4
。＝
。
＝
· =듸 뮤

=z림4.1 DTD에서사용되는다섯가치종류의개체들아있다. 일반
갠체들은XMI』문서 인세저사용된다. parameter7〃체들은J:）끄）
에서만사용된다（내부parameter개체들은그 용빕아 너무 한정
적안 면아 오卜읜卄梧욜 권하고 싶자 않다）
.

개체라는 것은 물이 닿으면 표준 사이즈로 팽창하게
되는작고납작한스펀지와같은것이다. 개체를
이용해 약자를 정의할 수 있고 XML 문서에서 지시
될 경우 팽창하는 데이터도 정의할수 있다. DTD나
XML 문서에서 개쳬 설명을 입력한다면 그것은
스펀지 전체를 가진 것과 마찬가지다．

===== PAGE 54 =====
53 =====
（知pter4

변：
＝芝＝.=－小da.dtd－ 轟 _-

텍스트를 위한 단축형 만들기
간단한 종류의 개체들은 DTD에서 정의되고 텍스
트로 표현된다. 공식적으로 그들은 내부 일반개처）
라
불리고 여기서는 텍즈트를 위한 단축형이라고
부른다．
텍스트로의 단축형 작성하기：
1. DTD에서 <!ENTITY를입력한다．
2. abbreviation이라고 입력한다. abbreviations
에 개체 설명의 텍스트 부분이 들어가게 될 것이
다（다시 말해 개체를 사용하기 위해서 입력되는
코드를 말한다）
.
3. "content＂를입력한다. 여기서 content는XML
문서에서 개체를 사용할 때 나타나야 하는 텍스
트를뜻한다．
4. ＞을입력하여 개체 정의를마친다．
'/ 1iPS
*
님
●눋느。 *금닐＝ 。云m＝ 云ebU

■ 이 단축형을사용하는 데에 대한세부사항은
p57에서 나오는 텍스트를 위한단축형 사용법
에서 언급될 것이다．
은 유효 XML
■ 개체 설명 (2번 전에 있는 약자）
이름을쓰는 干칙을따른다．
■ 다섯 개의 내부 일반 개체들이 있다：&amp;,
帥;, &gt;, &quot;, &이0st; (p.31참조）모든
개체들은 선언 후 사용해야 한다．
■ 하나의 개체는간접적인 설명이 없는한다른
개체를 포함할 수 있다．
■ 문서에 특별한 기호를 넣을 때 사용되는 캐릭터
에 관한 설명들은 비슷하게는 보이지만 개체들
이 아니므로 DTD에서 선언될 필요가 없다
(p247참조）
.
■ 많은 일반적인 개체들은 벌써 정의되어 있다．
세부 사항을 보기 위해서는 p60-61을 참고한다．

56

!FJNI I I i nwi

nornoc er vyi,otire ins,rure >

그림 4.2 'II부 일반걔체들은 빨ㄹ7 입력하가에는 길고 함든 문중쎄
사용된다．

===== PAGE 55 =====
54 =====
Entites and Notations in DTDs
－口＞스스＝스盧斗

`

`

Code.uml

<description>The &hwi; focuses on the research 0f
threatened species and sensitive ec히ogic히 systems.
For more information, check out their Web site at
http://www.uidaho.edu/rsrch/hwi/main.htm.

n

텍스트I 위한 단축형 사용하기

</description>

일단 한 번 개체를 정의하게 되면 주어진ㅁrD를
설명하고 있는XML 문서에서 개체를 사용할 수
있게 된다．

그람4.3Hornocker Wildlife Institute보다는&hwi릍

텍스트 단축형 ㅅㅐ료하기：

입력하는 편아 더쉬울 깃아다．

「헝1꺾；瓦7,，』. .)

1. XML문서에서 &（이것은하나의 앰퍼샌드（&)
가 아니다）
을 입력한다．

，鬼

<'on닒 v日r5mn="工α encod1'ta-'UrFㅢy >>
띠OOCrrPE document (lC. e Sown. 15, f너／1出乙하／)8∥』』斗
니 < cUment>
<dystniptlon>The 比｝
rn(j따in, mmme Institute 釉wson on the
research of 솨1reatelied specie` and 5e.,`it纛Ye ec`H町1ic∥
systems. For more hformation, Ch.ck not the什 web site at
http://wwe..oidaho.edn/rsrcbmr.l/maln.htm.</d'tscription>
町cum밈cc>

勿力虹締 －…

…

-

小∼

ㅑ1

融t.a 'iia,可‘ →

그람 `4 파서를 가지고 볼 때는 깨체가 펼쳐보여진다（하 경우
인Ej넷 익스플로러 5.0에저본 깃이다). p175부타 사착되는Part
5에서 배울 몇가자 종루의스타일들을 적용하기 전까ㅈ］는브라우
저를 가차고 제대．
로 된그림을 만들기는 어렵다는 것을주의하자．

2. abbreviation을입력한다. 여기서 abbrevia枷fl은 개체를 정의하는 이름이며 또한p56에
나오는 2번에서 쓰이는 것과 p58의 4번에서
사용된 것과도 상응되는 것이다．
3. 세미콜론
（;）을입력한다．

V Tips
■ 간접적인 설명이 있지 않은한 다른 개체의 정의
에서 개체를 사용할 수 있다

■ 컨텐츠가 결과적으로 XML 문서의 본문에 사용
된다면 일반 개체 (p56와p58에 설명된 것들과
같은 것）
는 DTI）
에서 사용할 수 있다. 독점적으
로 사용되어 ㅁrD를 확장시키거나 DTD 자체를
더해주는 개쳬들을 인자 개체라 하고 이것은
약간 다른구문을 갖고 있다 (p60 참조）
.

예제의소스 코드는 www,cookwootjcorn에 있습나다．

57

呈＝ ．쑤。 ＝＾듬* ●＝驪X4

■ 문서의 DI1）
에서 개체가 설명되지 않을 때는
개체를 사용할 수 없다. 사용한다면 파서는 에러
로 처리할 것이다．

===== PAGE 56 =====
55 =====
Chapter4

외부 파일에서 텍스트를 위한 단축형
더 큰 개체가 있다면 분리된 외부 문서에 이것을
저장시키기는 쉬워질 것이다. 이 시스템은 개체들을
다른 사람들과 공유할 수 있게 해준다．
외부 문서에서 단축형 만들기：
1. 하나의 외부파일에 개체를위한컨텐츠를만든
다. 텍스트 파일로 저장해 준다．
2. XML문서에서 첫 XML 프로세싱 명령 (p24
참조）
에 standalone="no"를 첨가한다. 왜냐
하면 그 문서는 개체 정의를 포함하고 있는 외부
파일에 의존해야 하기 때문이다．

4.

3, 개체를사용할XML문서를위한DTD에서는
<!ENTITY를 입력하는 것이 개체 정의를 시작
하는 것이다．
abbreviation을 입력한다. abbreviation은
외부 개쳬의 정의된 이름이다．

小으… ， 。＝，●*X띱 = *X굡 ，
。
* ·섭V＝ 。＝m

5. abbreviation이 다른문서에서 정의되었다는
것을 알리기 위해서 SYSTEM을 입력한다．

스｛그

」ㅋ

쐰

code.sml 髥콰

<0匕,C, pLU급＞口 七. HCiV0(ker 낚／∥레ite nsh .,ie
focuses on the research of threatened species and
sensitive ec이ogic네 systems. For more information,
check out their Web site at
http://www.uidaho.edu/rsrch/hwi/main.htm.
</description>
그림 45 아번에는 ㅇ／모든xL코드가 막 정의하려는 갱체의
컨텐츠가 되었다. hwient라고 불리우는 텍즈트 파일로 저장할
것ㅇ／다．
客蔽→－--

Co e*dtd

<!ENTITY hwi_descrip SYSTEM "hwi.ent「>
2림4.6 hwi_descrip 개쩌）
는 걔체의 컨텐츠룰포함하고 있는
파일의 URL을 가라킨다 (2림4.5).
느二 껀 '＝口r느三一＝
ㅌ三r＝ 간｀
노屍

굿

口｝
de．
ㅐ11M 輟缶二＝

뜨心켤

<?xml version= ' 1.0" standalone= 'no∥?>
<organizations>
<org_name>Hornocker Wildlife Institute</org_name>
鮎wi_ descrip;
</organizations>

6. "entity.url" 을입력한다. en毗Y. wi은1번에서
작성된 파일의 위치이다．

<organizations>

7. ＞을입력하여 마친다．

그림 47XML 선언에standalone= "no" 를 넣는 깃을 맞자
밀마라. 그라고 나서문사에 있는 외부 일반개제를ㅈ悟할수 았을
것아다. 여가서보여진 &hwi_descrip처럼 말이다．

58

===== PAGE 57 =====
56 =====
Entites and Notations in DTDs
多F tdtd\e났e,naJOenma1nMfy.ooJ - Hc1o=of* I' tennt E* *.
Ek

i*

글」
〔1혀＝*,

Yow
mh

Fovoige, loil,

a

SI야》

口回口

小嶼

＝」

R的e1+,

<t,nnI Sarsiotm''1ff, nncodurpg. UIF-8 standnInns-"nr 7>
cIDOCSYPE orQanizatoor,, 泌好o SOWW fof,jl doofypi. .江
＜口rgafleabon5>
0010끄Woe가佃rno太er Wndille lnotltotee/ord_narne>
oerL fltc- - The Hornocker Wildlife Institute focuses on the
resnorα．of threatened optden ond Sensitive et이四kai
syoteltls F0r morn information, clwck not their Web 引te at
h0p://roroe. oid耐medigjrsrcfl(hWl/1n.iahtol.<〃e5 -nm山n:
<jorgan.zab0n5>

그람 王8 아빈에는 요소뿐만 아나라7姻）
를포함한와부 걔처）
에
대한 叩71다. 짧은 문장을쓰면 파저가 그 짧은 문장 대신 설명
컨텐츠로 바꾸는 형직은 같다. 하나의 와부 개제에서오는 어딴
개체는 유효한 문서의DTD에저 반드사 정의돠이야 한다는 것을
주의ll라．

'/ 1iFIs
■ 새로운개체를사용하는방법을알고싶다면
p57의 텍즈트를 위한 단축형사용하刀를 참조
한다．
■ 이것은 여러 가지 다른 것들로부터 하나의 문서
를작성하는방법이다．
■ 개체들의 컨텐츠가XML이거나텍스트이지만
XML 문서의 ㅁPD 외부에서 정의된 개체들은
공식적으로 외부 일반 7fl쩌）
라고 한다．

。
4 큐X* = mX빼멱금 ==m
뿌。 ＝^== *

혀］제의소스 코드는 www.cookwood.corn叩 있습L7다．

59

===== PAGE 58 =====
57 =====
Chapter4

DTD의 단축형 제작과 사용

듈m－

지금까지 언급했던 개체들은 모두 XML 문서의 컨텐
츠에서 사용되는 것을 설명하고 있지만 Dㄱ
［〕 자체에
관한 단축형을 만들 수도 있다. 이러한 종류의 약자
들을 와부 인자 개체라고 한다．

<!ATTLIST picture filename CDATA #REQUIRED

1. 하나의 외부파일에 있는개체의 컨텐츠를
만든다. 텍스트 파일로 저장한다．
2. XML문서 안에서는처음XML 처리 명령
（p24
참조）
에 S紬nddone="no'＇를 넣는다. 왜냐하면
문서는 개체 정의를 포함한 외부 파일에 의존해
야 하기 때문이다．
3. 개체를사용할XML문서의 DTD에서 개체
정의를 시작하기 위해 <!ENTITY를 입력한다．

5.
6.

ㅃbreviation을 입력한다. abbreviation 자리
에는 외부 개체의 이름을 입력한다．

또는PUBLIC"name＂을입력한다. name자리
에는 대중적으로 유효하고 표준화된 개체 목록
의 공식적인 이름이 들어간다．

!

클

<2xm1 version="1.0"stcindalone='no?>
.c!DOCTYPE endangered_species I
<!ELEMENT endangered_species )anima1')>
<'ELEMENT animal (name+, picture)>
c1ELEMENT name (#PCDATA)>
<!ATTLIST name language lEnglish I Latin)
#REQUIRED>
<!ENTITY % full_pic SYSTEM 'pic.dtd">
그림 4.10picture요소와그것의 속성들을 선언하고자 하는 각각의
DTD 안에서는 걔처）
를 정의해야 한다（여가서보이는 것처럼）
.

"entib.url"을 입력한다. entity. un자리에는
1번에서 만든 파일의 경로가 들어간다．

鄂i賈鑿髥盤茗＝楓聊蠶蓉 code.dtd

뱝竇

<?xml version=" 1.0"standalone="no"?>
<IDOCTYPE endangered_species [
<IELEMENT endangered_species )animal')>
<!ELEMENT animal (name+, picture)>
<!ELEMENT name (#PCDATA)>
<IA1TLIST name language lEnglish I Latin)
#REQLJIRED>
<IENTITY % full_pic SYSTEM "pic.dtd">
% full_pic;
]>

8.

그림 4.9 여가이／ 대가 다른 여러DTD에서 사용하고 싶온 i刃7ㅍ）들아
있다．이것은picture 요소의 선언과그것의 속성들을포함하고
있고 pic.dtd- 불라우는 분라된 파일로 저장된다．

공간을 남긴다（스페이스바를 클릭한다）
.

7. 약자가다른문서 안에서 정의된다는 것을알리
기 위해 SYSTEM을 입력한다．

9.

。 云 m = = = , ＝ 。 m = ＝。●，U
·。눋。 ，。*==V* 느

4. ％을 입력한다. 이것은약자가ㅁrn를위한것이
라는 것을 알리기 위한 것이다．

x CDATA #REQUIRED
y CDATA #REQUIRED>

鄂．

DID의 단축형 만튤기：

奎竇三 code.dtd 톺릎룰弓占立二＝年ㅉ 屎 臘彗

<!ELEMENT picture EMPTY>

＞을 입력하여 마친다．

60

그람 빅끄 깨처7가 한 번 쟝의되ㅇ／자면 아것에 대한 설명으로 이용할
수 있다．여기 예제에저는%full_pic 이다．

===== PAGE 59 =====
58 =====
Entites an山｀Jotations in DIDs
口

code.dtd

陋

<?xml version= 1.0'standalone='no'?>
<!DOCTYPE endangered_species [
<IELEMENT endangered_species (anim(
<!ELEMENT animal (name+, picture)>
<!ELEMENT name (#PCDATA)>
<IAIILIST name language (English I La
#REQUIRED>
<IELEMENT picture EMPTY>
<lAULIST picture filename CDAIA #RE(
x CDATA #REQUIRED

1>

y CDATA #REQUIRED>

그림 412 XML parser는 갱4 설명을관련된 파일의 컨텐츠로
대잔하다
（쀼에서보여잔DTD는parameter개4 설명을사용할 때
나타나는 dramatization' 의 일종아다t

인자 개체를 정의한 적이 있다면 그것을 사용해도
무방하다．
DID를 위한 단축형 사용하기：
%abbreviation을 입력한다. abbreviation은 p60
의 6번, 개체 정의에 사용된 이름을 입력한다（그림
4.10.

'/ Tips
■ 인자 개체들은 Dli〕
에서 사용되기 전에 반드시
정의되어야한다. 이 경우에는순서가중요하다．
■ 내부I工
「D에서는내부인자개체들을만들수
있지만 이 경우에는 그것을 포함하고 있는 완전
한 선언에만 제한된다 - 일부분은 허용되지 않
는다 따라서 이것은 그리 유용한 것이 아니다．

■ 이런 기술을 독자 자신의 DTD 물론 다른
사람의 DTD에도 사용할 수 있다. 예를 들면
그것들을 스스로 정의하지 않아도 정의된 요소
（이것은 우리에게 친숙한 HTML 요소의 생김새
와 사용법이 비슷하다）
를 사용할 수 있게 하기
위해서 XHTML DTD에 설명할 수 있다.
■ 또는 개체들의 표준화된 리스트들을 h山）
：〃
www.schema,net에서 사용 가능한 목록들처럼
링크를 시켜줄 수도 있다. 이것은 각각에 개체를
직접 정의하지 않고도 문서에서 강조된 기억하
기 쉬운 개체 설명을 사용할 수 있게 해준다.
■ DTD는원하는대로사용할수있다는것을
기억하자．

qll의소스코드는www,cookwoocL corn에았습나다.

6]

^
4
e
。 ＝＝口。 ＝｀툐＝ 口孚。 ＝＾됴m* 。4듸뮤

■ 구두점 찍기에는 더 세심한주의를 할 필요가
있다. 직접 인용부호와 < , > 표시 괄호 등이
많다．

===== PAGE 60 =====
59 =====
대apter4

해석되지 않은 컨텐츠의 개체 만들기
지금까지 컨텐츠가 텍스트인 개체에 대해 알아보았
다. 컨텐츠를 포함한 개체들은 해석된 걔체 (parsed
entities)라고한다. 그 이유는XML파서가XML
문서로 이행되는 과정에서 개체들을 분적하고 있기
때문이다. 비해석개체unparsed entities)는이번
섹션에서 설명할 것인데 반드시 텍스트를 포함하는
것은아니다. 그러나가장중요한것은그들은XML
파서에 의해 완전히 무시된다는 사실이다. 그들은
XML 문서에서 텍스트가 아니거나 또는 XML 컨텐
츠가 아닌 것을 삽입하는데 사용된다．

그림 4.13 아것은 JPEG 파일로 해석되치 않은 정보의 전형적인
것이다. 아것은tiger.jpg. 불ㄹ／운다

Cod0,dtd

비하넉 컨唯 맨i기：

<?xml version=「1.0「encoding="UTF-8"
standalone="no"?>

XML문서에 삽입하기 원하는 데이터를 만든다. 이
것은텍스트나이미지 화일, 영화, pdf파일, 그밖의
것들을 포함하고 있다.

<!DOCTYPE endangered_species[

돕芸

<!ELEMENT endangered_species (animals)>
<!ELEMENT animal (name+, photo)>
<!ELEMENT name )#PCDATA) >

비해卜석 컨騙에 대한 개체 정의하기：
*=0* ＝。U큅● m
， 口｀ =＝느。 *m겸* =＝山 m= ＝。0느U

1. 데이터를끼워 놓고싶은문서의 DTD안에서
<'ENTITY를 입력하여 비해석 개체의 정의를
시작한다．
2. abbreviation을입력한다. abbreviation자리
에는 외부 개체의 이름이 들어간다.
3. 개체가다른문서에 정의되어 있다는것을알리
기 위해 $YSTEㅆ을 입력한다．
4. "entib.url"이라고입력한다. entity. wi자리
에는 비해석 컨텐츠를 가지고 있는 파일의 위치
가들어간다.
5. NDATAid를입력한다. 여기서 Id는비해석
데이터를 설명할 개념을 정의하는 단어가 들어
간다．
6. ＞을입력하여 개체 정의를마감한다．

62

<!A1TLlST name language (English I Latin)
#REQUIRED>
<IENTITY tiger_pic SYSTEM 'tiger. pg" NDATA jpg>
a림4.14 개체는 tiger_pic이라는 아語가자고 있는데 아
것은 tiger.jpg라고 불라우는 와부 SYSTEM 파일을 설명하고 있다．
그라고jpg라고 불라우는NOTATION을봄으로서파일에 대한
정보를 얻을 주 있다．

===== PAGE 61 =====
60 =====
Entites an山\lotations in DTDs

<?xml version="1 0"encoding="UTF-8"
standalone="no"?>
<lDOCTYPE endangered_species[
<!ELEMENT endangered_species (animali>
<!ELEMENT animal (name+, photo)>
<!ELEMENT name (#PCDATA) >
<!A1TLIST name language (English I Latin)
#REQUIRED>
<lENTITY tiger_pic SYSTEM "tiger.ipg" NDATA jpg>
<!NOTATION pg SYSTEM "image/jpeg'>
그림 4j5 걔념요소의 이름은 걔제선언 안에있는NDATA 뒤에
았는 가치값叩장웅되ㅇ／아 한다．

컨텐츠 타입에 대한 정보 삽입하기：
1. 상응하는 개체 정의 뒤에 있는DTD의 새로운
라인에＜!NOTATION id를 입력한다. 여기서
Id자리에는 개념의 이름과p62의 5번에서 사용
된 것과 똑같은 정의 단어를 넣는다．
2. SYSTEM을입력한다．
3. "content_information"을입력한다. content
information 자리에는 끼워 넣어야 할 데이터
를정의한다. 이러한정보는공식적인형식이
있는 것은 아니다．
4. 마지막으로＞을 입력하여 개념 선언을완성
한다．

I, nPs

■ 비해석 개체들은단지 XML문서의 일부분만
될 뿐이다. 그들은 DTI〕
의 부분이 될 수 없다．
다른 말로 하면 비해석 개체들은 인자 개체가
아닌 일반적인 개체들이다．
■ 개념 선언의 컨텐츠는MIME 타입, 비해석 데이
터를 다루는 외부 적용을 지시하는 URL 등이
며, 실제적으로는어떤것이든무방하다. 여기에
공식적인 형식은 없다. 각각의 끄‘4L 적용은 그
것의 방식대로 개념 선언을 할 수 있다．

예제의소스 코드는 1m w.c0傲wocxj corn에 있습나다．

63

。m。 ＝＝口m＝ 壬首m* 。，=＝큅。 ，m요＾ 。＝4e= *

■ 비해석 개체의 컨텐츠는무엇에 관해서든무방
하다. 가끔이것은이미지, 사운드, 영화, 또는
다른 종류의 멀티미디어 파일이 될 수 있다．
또한 이것은 순수한 텍스트 파일이 될 수도
있다. 컨텐츠가무엇이든상관없다. 왜냐하면
XML 파서는 이것들을 인지할 수 없기 때문
이다．

===== PAGE 62 =====
61 =====
Chapter4

p62에 언급한 바와같이 비해석 데이터를 위한하나
의 개체를 정의하였다면 XML 문서에 그것을 끼워
낳을수 있게 된다. 비해석 개체들은 개체 설명을
갖지 않는다. 대신 특별히 선언된 속정들을 통해서
그들을 부를 수 있다．
비해석 컨텐츠의 설명을 포함한 속성 선언하기：
1. DTD에서 비해석 데이터를설명할속성을포함
할 요소를 정의한다 (p42 참조）
.
2. <!ATFLIST element_name을입력한다．
elei끄entname 자리에는 1번에서 선언한
요소를 설명한다．
3. aft_name을입력한다. att name자리에는
비해석 데이터의 설명을 포함할속정의 이름을
입력한다．
4. 비해석 데이터의 설명을포함할수 있는 것으로
이 속성을 정의하기 위해서 ENTITY를 입력한다．
｀ ==m＝ 믈경＝ ㅌ
山
*＝으＝ 。U경m， 口

또는 만일 어떤 속정이 여러 개의 빈공간으로
나뉘어진 비해석 데이터 파일의 설명들을 포함
하게 하고 싶다면 티｀4TㄲES를 입력한다．
5, 속성에 대해서는디폴트값을넣는다. 세부사항
은 p50의 간단한족성 정의하기를 참고한다．
6. ＞으로속성 선언을마친다.

64

盤．

ㅊ

＋→ code.dtd-

晋듈

<?xml version=" 1.0" encoding="UTF-8"
standalone="no"?>
<!DOCTYPE endangered_species
<!ELEMENT endangered_species (animal' )>
<IELEMENT animal (name+, photo)>
<!ELEMENT name (#PCDATA) >
<'ATTLIST name language (English I Latin)
#REQUIRED>
<!ENTITY tiger_pic SYSTEM "tiger.ipg" NDATA ipg>
<!NOTATION ipg SYSTEM "image/jpeg">
<'ELEMENT photo EMPTY>
<!AnLIST photo source ENTITY #REQUIRED>
]>

비해석 컨텐츠 삽입

그람 4.16 첫번째로 파저되자 않은 데아El를 설명할족정을포함할
photo 요소를 정의해아 한다. 그리고 中作ource라고 불라
우는 걔처］속정자쳐7를 정의한다．

===== PAGE 63 =====
62 =====
Entites and Notations in DTDs
지刪．
. 문서에 비해석 컨텐츠 끼워 넣기：

i一르느

cee.mm

<?xml version= "1.0" encoding="UIF-8"
standalone="no"?>

XML 문서에서 속성값을 만나게 되면 att_name=
"value＂를 입력한다. att-name자리에는 개체
타입과 함께 선언해 놓은 속성을 정의하는 것을 입력
하면 되고 value 값에는 p62의 2번에 나오는 비해석
데이터를 포함하게 만들어 놓은 개체의 약자를 쓰면
된다．

<!DOCTYPE endangered_species [
<'ELEMENT endangered_species (animal')>
<!ELEMENT animal (name+, photo)>
<!ELEMENT name (#PCDATA) >
<IATTLIST name language (English I Lain)
#REQUIRED>
<'ENTITY tiger_pic SYSTEM "tiger.jpg" NDATA jpg>
<!NOTATION jpg SYSTEM "image/jpeg">
<!ELEMENT photo EMPTY>

V Tips
■XML파서들은그들이 속성과함께 있는 개체에
의해 설명된 비해석 데이터를보게 하기 위해서
개넘내의 정보를 사용할수 있게 되어 있는데
반해, 익스플로러나넷스케이프6.0버전（최근
의 XML 파일을 읽을 수 있는 유일한 브라우저
들）
은 효과적으로 개념 정보를 사용할 수 있게
설정되어 있다. 간단히 말해 브라우저들은삽입
한 데이터는 보여 주지 않을 것이다（그림 4.18).

1>

<IATTLIST photo ,ource ENTITY #REQURED>

<endangered_species>
<animal>
<name Ianguage="Engtish">Tiger.c/name>
<photo source="tiger_pic"/>
</animal>
</endangered_species>

．呼

Mj o'Oft h,t1met E,,pio.o`

!oe$
J
smp

n 「 '-

5e
끄
Rale굻，

s，h

ㅂ

.
B k

F소vote

꿨，

y,ew

，궜.

｝「人dh1뇨＇npa'`ed cm寸enL〃m

펴
月

그림 4.18 아제챗 나온 브라우저들 중oflAJ )(iiL을 읽을 수 았는
브라우저들인 익스플로러（여刀서보여징）
나Mozilla (9 케ㅇ］프
6. 0 乙〃）타 버전인）
에저의 결과는 쟐망스러울 것이다. 그러나사스템
자체는 이진법파일을 까아 놓을 수 밌게 설정되아 았는 것이다．
다만브라우저가 ㅇ／시스텡을 아떻게 이용하슨자 아작 꼬를뿐이다．

예제의소스 코드는 www.cookwooL corn에 있습나다．

65

m클口m口튜＝ ．口＝ ｛。，mm` ＾。＝言三

그림 4.17 source 족성의값은 해석되자 않은 데아E7를 설명하슨
걔체의 이틈과 상웅되이야 한다．

■ 개넘 선언 (p63 참조）
의 데이터를 직접 설명하기
위해서 NOTATION의 속성을 만들 수 있다. 구
문은 다음과같다 <!A1TLIST element_name
aft name NOTATION default value>

===== PAGE 64 =====
63 =====
PART 3:
XML 스키마와 이름공간
XML 스7／마 69
단순한 타입 정의하기 75
복잡한 타입 정의하기 93
XML2I 이틈공간사용하기 γγ3
아름공간, 스키마 그리고 유효성 欠但／ 121

67

===== PAGE 65 =====
64 =====
XML SCHEMA
XML 스키마

중요 노트
xML 스키마는 마감 시간이 임박했음에도 불
구하고 여전히 유효한 기사이다. 이 의미는
W3C가 구문에 변화를 줄 수 있는 가능성이 아
직 있다는 애기다. 만일 변화가 있다톈이 책의
웹 사이트 (P炤 참조）
에 업데이트 된 내용을 올
릴 것이다. 그리고 XML 스키마의 가장 최근
소식은 http://www.w3.org/XML/schema에
서 찾햐볼 수 있다．

요소들이 포함하는 것 그리고 그것의 순서, 컨텐츠의
내용, 포함하고 있는 속성들을 보면 스키ㅁ／라는 것은
ㄸ［n처럼 하나 또는 그 이상의 XML 문서의 모임같
이 보일 것이다. 사실 DTD라는 것은 단어의 일반적
인 의미로는 스키마의 한 종류이다. 이 장에서 스캬
마라는 것은 XML 언어 안에 있는 스키마만을 의미
한다．
n [L는 XML 스키마에 있는 것과 비교한다면 여러
가지 불편한 점이 있다. 첫번째로 DTD는 Xn꽈는
거의 상관이 없는 구문에 씌어져 있어서 xML
파서에 의해 해석되지 않는다. 둘째로 mD에 있는
모든 선언들은 포괄성을 갖고 있다. 이것의 의미는
다른 문맥에 있는 이름이라고 할지라도 같은 이름으
로 두 개의 요소를 정의할 수 없게 된다는 것이다．

W3C에 의해 개발된 XML 스키마 언어는 이러한
문제들을수정하고자 했다. XML에 있는XML 스키
마는 포괄적 요소들 (X\4. 문서를 통틀어 똑같은
방식으로만 사용되어야 하는 것들）
과 지엽적 요소들
（특별한 문맥에서 고유한 의미를 가질 수 있는 것들）
모두를 정의할수 있게 한다. 부과적으로 XML 스키
마는 데이터 타입 (datatypes) 시스템을 갖고 있는
뎨 이것은, 첫째로 주어진 요소가 하나의 정수를 가
지는 것, 다른 요소는 어느 정도의 시간을 가지게 하
는것, 마지막요소는기호열을가지는것으로지정
할 수 있게 해준다. 요약하면 XML 스키마는 XML
문서의 컨텐츠에 대해 더 큰 장악력을 가지게 한다．

69

，글尸 m수m클。

마지막으로 가장 중요한 이유는 DH）
가 주어진 요소
나 속성이 어떤 종루의 정보를 포함하고 있는 가를
제어할 수 없다는 것이다．

===== PAGE 66 =====
65 =====
태apter5

간단하고도 복잡한 타입
스키마에서 하나의 문서는 두 가지 타입으로 나누어
진다. 바로 간단한 것과 복잡한 것이다. 틔슨튼맡요
는 요소는 간다한 타입의 것이다. 다루 요소나 속성
들을 갖는 것은 복잡한 타입이다. 속정들은 텍스트만
을 가지고 있기 때문에 단순한 타입으로 간주된다．
단순한 타입들에 대해 더 자세히 알아보자. 하나의
DH）
에서는 요소를 #PCDATA와 같은 컨텐츠를
분류하는 텍스트를 가지는 것이라고 정의한다．
PCDATA는 이름, 숫자, 날짜 - 실제적으로 어느것
이나 될 수 있는 것이다. XML 스키마에서는 하나의
요소가 포함하고자 하는 종류의 텍스트를 특별히
단순한 타입의 정의를 배정함으로써 구분하고자
한다. 여기에는 여러 가지 단순한 타입이 있다. 예를
들어 날짜, 숫자, 기호열 등과 같이 변형없이 쓸 수
있는 것들이 있고, 요소의 컨텐츠가 어떻게 보이는가
를 더 잘 조절하기 위해서 직접 만들 수 있는 단순한
타입들도 있다. 6장 단순한 타입 정의하刀에서 더
자세한 정보를 볼 수 있을 것이다．

·●뫘눋Xm료ㅌ 。U, ＝。읕ㅌ 二

복잡한 타입의 요소들은 그것의 컨텐츠를 설명하기
보다는 어떤 문서의 구조에 대해 설명한다. 복잡한
타입에는 4가지 기본 종류가 있다. 단지 다른 하나의
요소들만 가진 요소들, 요소와 텍스트를 가진 요소
들, 텍스트만을 가진 요소들, 빈 요소들. 물론 각각의
것들은 각각 속성들을 갖고 있다. XML 문서에 필요
한특정의 복잡한타입을 정의하면 된다. 이것은 7장
복잡한 타입 정의하刀에 자세히 설명되어 있다．
단순한 타입과 복잡한 타입은 모두 이름을 가지고
있다. 복잡한 타입은 스키마 안의 다른 곳에서 쓰였
던 이름을 다시 쓸 수 있거나 이름이 없어도 되는
반면에 단순한 타입은 정의가 나타난 요소에 한 번만
사용해야한다

70

口

；七窈끅拿器토三一c.de.ㅃd

<xsd:element name="weight" type=' xsd:striny"
<xsd:element name="population"
type="xsd:integer"/>
그람 5.1 여기두요소들은 정해진 단준한 타입－으로 정의돠어 있다．
weight 요소는 가호열로 한정되어 았는 반면에population
요소는 줏자로 정의되어 았다．

翌1
；牛댑븍呼始斗구룻녹｀
텍뿌－媤臂 COde.HSd－流磅

毒轟

騙i黍

<xsd:simplelype name="zipcodelype">
<xsd:restriction base="xsd:string">
<xsd:pattern value="\d{5}(-\d{4})?"/>
</xsd:restriction>
</xsd:simplelype>
.2림5.2 이시용자 정의 타입은zipcodeType으로 겋의되어
있는 요소의 컨텐츠를 선택사힝1으로 하솨픈 C)과 네걔의숫자가
뒤따라오는 다섯 걔의 줏ㅈ屠가진 7/－흐열로 정의한다．

W

-

i,', " ``y "V`

'-' code,e$d

.cxsd:complexType name="endlype">
<xsd:sequence>
<xsd:element name="animal"
type="animalType"minOccurs="1"
maxOccurs="unbounded"/>
</xsd:sequence>
</xsd:complexlype>
그림 5.3 아 복잡한 타입의 정의는endType을 다른 하나의요조
（다른 복잡한 타입인anima1Type_ 정의되어잔animal
요소7喝포함하슨 것．
으로 정의한다．

큅

===== PAGE 67 =====
66 =====
XML Schema
들驕可口F넓극三＝

습

code.nsd

<2xml version="1.0" ?>
<xsd:schema xmlns:xsd="http://www.w3.org
/2000/10/XMLSchema">
<xsd:element name＝
「endangered_spedes"
type="endType"/>
<xsd:element name="name" type "xsd:string"/>
<xsd:complexType name="endType">
<xsd:sequence>
<xsd:element name="animaI">
<xsd:complexlype>
<xsd:sequence>
<xsd:element ref="name"
minOccurs="2"/>
.'zxsd:element nome="source"
type="sourcelype"/>
</xsd:complexType>
<xsd:compexType name="habitatType">
<xsd:sequence>
<xsd:element name="river">
<xsd:complexlype>
<xsd:sequence>
<xsd:element ref=' name'
minOccurs="1"
maxOccurs궁'unbounded"!>
<xsd:element name="source'
Iypo="xsd:string 'I>

그림 5.4 이schema 인용구에는포괄적으로 선언된 네72/ 부분이
있다. 왜냐하면 아것들은XSD =schema 요소 아래에밌는 첫번째
레벨에 나타나가 때문아다. root 요소 (endangered_ specie콰
는 자동적0로 설명되는 반면name 요소 r이것은 루트 요소가 아나
7/ 때문에／L는 여7/에서처럼 직접 설명되어먀 한다．

XML 스키마에서는 문맥이 매우 중요하다. 스키마
의 가장 위쪽 줄에서 선언되었고 xsd: schema 요소
바로 밑에서 정의된 스키마의 구성물들인 요소, 속성
그리고 명명된 단순한 타입과 복잡한 타입들（나중에
설명할 그룹들과 속정 그룹들도 포함해서）
은 포괄적
으로선언되어졌다고여겨진다. 그리고이것들은
스키마의 나머지 부분을 사용하는 것이 가능하다．
포괄적 요소 선언들은 하나의 요소가 XML 문서의
어느 부분에 나타날 수 있는지를 결정하지 못하고
단지 그 요소가 어떻게 생겼는지를 판단한다. 포괄적
요소 선언에 대해 자세히 설명할 필요가 있다. 왜냐
하면 상응하는 XML 문서에서 이것이 실제로 나타
나기 때문이다．
이런 干칙의 유일한 예외는 어디서 선언되었든 저절
로 설명이 되는 루트 요소에 관한 것이다．
복잡한 타입을 정의할 때는 이미 존재하고 있는 포괄
적으로 선언된 요소를 참조할수도 있고 또는 그
지점에서 새로운 요소를 선언하고 정의할 수 있다．
이러한 지엽적 선언이 된 요소들은 일단 선언되면
스키마 안에서는 다른 곳에서 사용이 제한되는 복잡
한 타입의 정의에 제한된다. 그리고 그들이 나오는
문맥에서 이름은 유일한 것이어야 한다．
이렇게 지엽적 선언이 된 요소들은 자동적으로 설명
된다. 다시 말해 그들이 정의된 지점과xML문서에
서 반드시 나타나야 할 곳을 정하게 된다．

여／ㅋI｝의소스 코드는 www.cookwood.com에 있습나다．

71

。m＝ 。｀。＝。＝m

두꺼운 글자체로 되어 았는 부분은 같은 이름이치만 다른 정의들을
가지고 았는 두 가자의부분척으로 (locally) 선언된王
［소들이다．
문맥은 아깃들을 뚜렷하게 만들어주는 경향이 있다. 포콸적꾜소
선언들은 반드시고우한 아름을가차고 았어야 한다．

Un）
에서는 모든 요소가 포괄적으로 선언된다．
이 의미는 모든 요소는 각각 하나의 고유한 이름을
가지고 있고 정확히 한 번 정의된다는 것이다. 하나
의 요소는 다른 요소들의 어떤 숫자에 의해 정의될
수 있는데, X Th 문서에서 한 곳 이상 나타날 수
있다는 것이다. 그러나 이것이 어디에 나타나든 요소
는 언제나 똑같은 정의를 가지고 있다．

尸
。＾
흽 。＝` 으。 g

</xsd:complexlype>

지엽적 선언과 포괄적 선언

===== PAGE 68 =====
67 =====
다iapter5

간단한 스키마 시작하기
스키마는텍스트만있는형식에서 .xsd확잣자름
갖고 있는XML 문서이다. 이것은 표준XML 선언과
함께 시작되고 뒤이어 XML 스키마 이름 공간
(namespace）
의 선언이 뒤따라오게된다．
스키마 시직하기：
1. 스키마문서의 처음에＜?x씨version=
"1.0"?》을 입력한다. XML 선언에 대해
더 알고 싶다면 p24의 XML 버전 선언하기를
참조한다．
2. <xsd:schema를입력한다．
3. xmlns:xsd="http://www.w3.org/2000
/10/XMLS小ema＂라고 입력한다. 이것은
스키마들의 스키마를 위한 이름 공간을 선언하
기 위함이다. 지금부터는xsd로 미리 정해진
어떤 요소나 타입등은 이름 공간으로부터 왔다
고 생각하면 된다．
4. ＞으로시작된스키마시작요소를마친다.

。ㅌ●七m읕ㅌ ㄵ。m灌＝ ＝楡m

5. 스키마의 규칙을포함할몇줄을남겨두자．
이 규칙에 대해서는 6장 단순한 타입 정의하기
와 7장 복잡한 타압 정의하기에서 살펴보자．
6. 마지막으로＜/xsd:sJlema＞를입력하여스키
마문서를마친다．
7. .xsd확장자로스키마를저장한다．

s/ Tip
으로부가적인
■ 디폴트이름공간（namespace）
이름공간과XML 스키마를 선언할 수 있지만
이기 때문
나중에 설명될 부분 (p126-128참조）
에 여기서 자세히는 설명하지 않을 것이다. 여기
서는 스키마를 어떻게 만드느냐에 집중하기
위해서 간단히 설명할 예정이다．

72

느薑軫느∼훈큔妊轟code.Hsd 纛坪릎＝;＝느－十＇녹∼∼→썹쿄

<?xml version="1.O" ?>
<xsd:schema xmlns:xsd=
'http://www.w3.org/2000/iO/XMLSchema">

</xsd:schema>
그랖 5.5 Schema의root 요소에저 schema들의schema룔 위한
이름공간을 선언해야 한다．

===== PAGE 69 =====
68 =====
XML Schema

"

回言

간단한 스키마의 위치 지정하기

?>

0

1

;

<?xml

口〕de.ㅐn기
version= "

<endangered_species
xmIns:xsi= http;//www.w3.org/2000/10/
XMLSchema-instance"
xsi:noNamespaceSchematocation=
"http://www.cookwood.coni/ns/end_species/
end_species.xsd'>
그림5.6 XML 문서의root 요소에 았는xsi:schemaLocation 요소를사용함으로써문저을 정의하는스카아
파일에겨）processoi를 자정할수 았다．

XML 문서와스키마를 비교하기 위해 유효성 처리
기에 의존하게 되면 상응하는 스키마가 XML 문서
어디에서 발견되는가를 지적해 주어야 한다．
스키마의 위치 지점봐 선언하기：
1. XML문서의루트요소안에서xmlna:xsi=
"http://www.w3.org/2000/10/XM1Sche
ma-instance＂를 입력한다. 이것은스키마장소
를 지정할 요소들을 가능하게 만드는 것이다
（이것을 이름공간선언하기라 하고 p116에 자세
한 사항이 나와 있다）
.
2. xsi:noNamespaceschemaLocation＝을 oJ
한다．
3. 그리고마지막으로 "file.xsd"를입력한다．
file.xsd 자리에는 XMl. 파일을 유효화하기
위해 사용하고 싶은 실제 스키마 파일 (p72의
7번에서 만들어 놓은）
의 IJRL이 들어간다．

'/ nPS
■ 하나의 스키마에 대비하여 문서를 유효화하는데
사용가능한 여러 가지 프로그램들이 있지만，
가장 믿을 만한 것은 XML 스키마 유효성 처리
기 (Schema validator) (p245 참조）
이다. 또는
XMLspy, XMLeditor등을사용해도무방하다．
이것들은 http.i/www.xrnlspy.corn에서 찾을
수 있다．
U xsi:noNamespaceSchemaLocation속성은
스키마 안에 선언된 목표 이름공간이 없을 때만
작동한다. 그리고 아마 책을 전반적으로 보지
않은 독자라면 목표 이름공간에 대해서 들어본
적이 없을 것이다（이것은 9장 이름공간스7/n/
그리고 유효성 처리에서 배우게 된다）
.

예졔의소스 코드는 www.cookwoo加0rn叩 있습나다；

73

===== PAGE 70 =====
69 =====
다iapter 5

스키마에 주석달기
스키마에 어떤 정보나 또는 이것의 요소를 다른 사람
들에게도 이해하기 쉽게 하기 위해 첨가할 수 있다．
스키마에 주석달기：
1. <xsd:annotation＞을입력한다．
2. 다음에＜xsd:documentation＞을입력한다．
이것은 컴퓨터가 아니라 사람이 읽을 수 있는
노트를 적는 것이다．
3. 노트를 입력한다．
4. </xsd:documentation＞을입력하여노트를
마친다．
5. 마지막으로＜/xsd:annotation＞으로주석을
마친다.

'Tip
■ 주적은xsd: schema 요소 바로 다음이나 개별
요소 선언 이후 또는 마지막에 만들 수 있다．

m
口
ㅌ ●七mm= ＝
口
*믄 둔
74

에de.H$d 쿄＝二系ㅋ芬芬喜＝輾＝
＝ㅍ팁틀
雪·
<xsd:schema xmlns:xsd="http://wvfw.w3.org/
2OOO/1O/XMLSchema">

<xsd:annotation>
<xsd:documentation>
재is schema will be used to v히idate 十e set of XML
document for the Endangered Species
project.c/xsd:documentation>
</xsd:annotation>
그림5.7주석은스7］
마를자세하 설명하는더7도움을준다. 아것은
또한 미래에 있을교정을 다욱 쉽게 한다．

===== PAGE 71 =====
70 =====
DEFINING SIMPLE TYPES
단순한 타입 정의하기

XML 스키마는 가장 일반적인 텍스트의 단순한
타입들을 포함하고 있다．
이것에는기호열, 부을표현식과URL, 다양한날짜
형식, 그리고 모든 종류의 숫자 등이 포함된다. 또한
제한 조건들을 단순한 타입에 적용함으로써 제한을
강화하는 동시에 고유한 타입을 만들 수 있을 것이
다. 예를 들면 하나의 요소가 하나의 어떤 패턴（전화
번호나 물건 코드）
에 상응되는 기호열을 포함하거나，
혹은 특정한 일련의 날짜들 중 하나를 포함하는 요소
들의 경우가 이에 해당된다.

75

。．m三＝ ． 묘 크 릉 뻐＜七mm

단순한 타입을 가진 하나의 요소는 단지 텍스트만을
포함한다. 다른요소나속성들을가질 수는 없다．
여기서 '텍스트’ 라는 것은 일반적 개념의 용어이다．
하나의 요소에 있어서 컨텐츠를 떽스트’로 제한하
는 대신 요소의 컨텐츠가 특별한 종류의 텍스트를
포함하도록 요구할 수 있다. 우리들은 미리 확정된
단순한 타입의 정의를 사용함으로써 컨텐츠를 제한
하는 일관된 기준을 세울 수 있다．

===== PAGE 72 =====
71 =====
다tapter6
口

단순한 타입을 가진 요소 선언

1. <xsd:elemen*을입력하여선언을시작한다．
2. name=1tI바뇌" 을입력한다. label자리에는
선언하고자 하는 요소의 이름을 넣는다. 다시
말해 XML 문서에서는 <label>과 같은 것이다.

c0dP.HsI1

嘴一

클 尸尸

團릎

그람 6.1 요소를 선언할 때는 그 아틈과 어딴 종류의 컨텐；츠를 갖는
가를선텍해아한다．

蚌＝=

code.eml 둥－

H'박t>500,p"unds</weight>
<popuiurion>zo<i popuiurian>

그림 6.2 刀호열은 Cㅈ隱 줏자들, and/or 가호들의사리츠아다．
정수는줏차전부아다. 따라저weight와population f상주）
요소들은 그림 6.1에서의 선언에 의하면 유효하다．

3. 1ype=＂를입력한다．

*＝·ㅌ으띱＝ 。
m
= ：룬금

다음xscl:sfring을 입력한다. 만일 이 요소가
글자의 기호열을 포함해야 하고 정수의 수를
포함하고 있다면 xsd:clecimd이라고 입력한다.
가능한숫자 타입을보려면 80p를 참조한다．
만일 그 요소가 진위 요소 (1혹은 0）
를 가지고
있다면 xscl:bodean이라고 입력한다.
혹은 요소가 날짜가 될 경우에는xscl:d이e라고
입력하면 된다. 다른 날짜 타입을 보려면 p78을
참조한다．
만일 그 요소가 시간이면 xscl:iime을 입력한다．
또 다른 사용 가능한 시간 타입을 보려면 p78을
참조한다．
혹은 요소가URI를 갖고 있다면 xsd:urireference이고 URL을 갖는다면 xsci:Iangua9e라고
입력한다. 만일 요소가 IS0639 리스트에 나와
있는 두 글자의 약자들 중 하나를 포함하고 있다
면 Cu引om 이라고 입력한다. custom 자리에는
고유한 단순한 타입의 이름이 들어간다．
4. '＇을입력하여 타입을마친다．
5. 마지막으로／＞을입력하여 태그를마친다．

76

ㅁ

-

읜 鷺 읕 ㅌ ㄵ。圭

단순한 타입의 요소 선언법：

-

<xsd:element name= 'population"
type="xsd;integer"/>

트．

다른 요소들이나 속성들을 포함할 수 있는 요소가
있다면 그것은 단순한 타입이라고 할수 있다. 많은
종류의 고유함을 가진 단순한 타입들이 있는데 여러
분 스스로 자신의 것을 고유한 타입 중 하나를 모델
로 하여 만들 수 있을 것이다．

＝ㅋ둣毛∼ `,`\

급 element name="wL ,

…一

ctele.nml

<weight>500</weight>
<populotion>not very mony</population>
.2림丘3 이보기에저는 처음 보기에는 weight요소가 옳차 않은
것처럼보일수 있다. 그라나 사실은 하나의 줏자도 가호열의 일종
이가 때문叩（역으로 모든 가호열아 줏자슨 아나다）이것은 유효한
깃이다. 그랴나 population 요소는물론 유효하자 않다. 'not
very many"J는 z절은정수가아나다．

===== PAGE 73 =====
72 =====
Defining Simple Type
一 一F－∼쟈三三一 에deJ쵱8d 蚌

纛4崙븍혹斗莩릎트昌븍＝'=li‘一

ent name="Iost modified"
:d아e∥／>
그림64 아 예제에서는 last_modified 요소가 날짜를포함
하려 한다．

-m

' ∼一

＜II

그쾀 6.5 유효화되가 위해서는요소는（刃YY-MM-DD의 형식으
로 날짜룸포함하고 았아야 한다. 다사 말해 네자라수 연도 다음에
甲쉬가오고, 월을 나타내는두자라수가오고또다른 甲쉬가오게
된다. 그 다음 날을 나타내는 두 자릿수가오게될 것아다. 다른
많은고우의사용 가눙한 형식들아 있다 (p78).

口

…

－三1

＝馨휼code.HnH二驪r 「

回言

<lasL-modified>May, 16, 1999<기ast_modified>
그림 6.6 날짜가 적절한 형삭아 아나가 때문에last_modified
요소는 유효하ㅈ］
않다．

■ 단순한주문형 타입들은 일반적으로 XSD로
시작한다（예p128). 이것은 단순한주문형 타입
들과 구별하기 쉽게 해 준다 (p81
■ 속정 자체는 언제나 단순한 타입이다. 속성은
자신의 컨텐츠나 속정을 갖고 있지 않기 때문이
다. 그리고 그들은 단순한 타입의 요소들과 선언
하는 방식에 있어서 공통점이 많다. 그러나 다음
장에서 (p108 참3) 설명할 요소 안에서의 선언
하기를 배우기 전에 그들을 선언하는 것은 상식
밖의 일이다．
■ 하나의 요소가속성이나 다른 요소들을 포함한
다면 그 요소는 복잡한 타입이 될 것이다. 자세
한 사항은 7장 복잡한 타입 정의하기를 보자.
■ 유효한요소이름은하나의글자나하선으로
시작되어야하고, 그 뒤에 글자들 혹은 숫자들
혹은 밑줄들, 하이픈, 마침표 등이 뒤따라온다.
상세 사항은 p26에 공백없는요소 작성하기를
참고하자．
■ 단순한타입의 요소들은포괄적으로 선언되거나
(xsd: schema밑의 첫 줄에서）복잡한 타입의
정의에서 설명될 필요가 있을 때, 또는 복잡한
타입 정의에서 지엽적으로 선언된다. 이 경우에
단순한 타입의 요소들은 자동적으로 참조된다.
더 자세한 사항은 7장의 복잡한 타입 정의하기
에서 볼 수 있다．

예제의소스 코드는 www.csokwoofwm叩 있습나다．

77

… 。m舌玉널口。 ＝쓰m크． 三 트 * 丁。 느 즐 릉 뻐 겸 m

" " '" " " >' "

■ http://www. w3.org/TR/xmlschema--2/
#built-in-datatypes에는 단순한 주문형 타입
의 목록들을 볼 수 있다．
■ 단순한타입을 이용해서 단순한 주문형타입을
만들수 있다. 자세한 사항은 p81에 나오는 단준
한주문형 타입작성하기를 참고하자．

阿 , F，
… ,.. 誓．
code.HmI
'I
1 astmodified>1999-05-16<加St modified>
'" "

V 1iPS

===== PAGE 74 =====
73 =====
다iapter6

阿
<gestation>

XML 스키마는 여러 가지 고유한 날짜에 관한 타입
을 갖고 있다. 각각의 목적에 맞는 것을 사용 (p76의
3번）
하거나p81중에서 하나를 선택하면 된다．

츤ㅌㅌ＝三 ＝雨
二 code.Ksd --7下二，

<xsd:element name='gestation"
Iype="xsd:timeDuration"/>

날따와 시간 타입 사용하기：

m
● ｀亡● E二겯口으口。 m
＝ 玄＝

1. 어느정도의 시간예를들면2시간, 12분, 그리
고 45.3초와 같은특정한 시간을 나타내는 컨텐
츠를 원한다면 xsd:timeDuration을 선택하자．
지속적 시간은 PnYnMnDTnHnMnS로 설정되
어 있어야 한다. 여기서 P는 언제나 필수 요소
이다 (P는 period를 의미한다）
. T는 선택 시간
부분 (section）
을 시작하는 것이며, 각각의 n
（언제나 non-negative integer이다）
은 뒤에
얼마나 많은 유닛들이 따라 오느냐를말해 주고
있다（년, 월, 일, 시간, 분, 초）
. 지속기간이 뒤
로 갔다는 것을 나타내기 위해서（앞쪽이 아니
라）선택적인 하이픈을 첨가한다．
2. 컨텐츠가하루의 특정 시간, 예를들어 4:15pm
을 가리키고자 할 때 xsd：卄me을 선택한다.
이것은 다음과 같이 설정되어야 한다．
hh:mm:ss.ss＄와시간대 별 표시기 α는 UTC
（협정세계시）
를 의미하고 卄i:mm 또는
+hh:mm은In℃와의 시간차를 의미한다．
3. 컨텐츠가1935년 5월 6일의 4:15분과같이 특정
시간을 의미하려면 xsd:timelnstanㅎ를 선택한
다. 이것은CCYY-MM-DDThh:mm: ss.sss와
시간대별 표시기로 설정되어야 한다．
4. 컨텐츠가1935년 5월 6일 같이 어느특정한
날을의미하려면xsd:date를선택한다. 이것은
ccYY-川M-DD 형식으로 설정되어야 한다．

78

\ →，一 , ``1, ‘→一．클

code.HmI

P3M15D<

/gestotion>

날짜와 시간 타입 이용하기

그림6.7호랑이는 약3걔월 반의 잎신 기간을가지고 있다. 모든
유닛을 징해줄 필요는 없다는 깃을 주목하자. 단차 차음P라는
것은 항상괼요한것이다. 만일period가 ㅈ／간 qj이E7릍포함
하고 았다면 T를 첨가ll아 한다．
輦■1`，各，
누朴뱃，
,,\｀뇨 -녹
（스
＇' code. isd 蘆

1크I

<xsd:element name=恪edtime" type=「xsd:fime"/>
횰．
!,`,>d+ ‘누k>＝뇩＋4- code.tmt

穫．
큭

<bedtime>20:15-05-05:00</bedtime>
그림6.8 사간은 뉴i胱a莎" 혹은 일반적인 폼에 았다는 것을주꼭
하자. 아bedtime 요소의 컨텐츠는8:15pm FiST섬ㅁ／타임 적용
사가 아님，
L를 나타낸다．
토1

三三：뉴

m 풀

三 三

=

∼

…

=

ㅗ1

<xsd:element name="birth"
type='xsd:timelnstant"/>
一 code.gml

흩區

___-.

-

<birth>1999-03-14T1 8:27:46.2398Z</birth>
그림 6.9 이요소의 컨텐츠는호랑이의출깽이 정확하게1999년
3 ' 12일 6:27pm 그라고 46.2398 (- t4j셜 타임）
라는 것을
의마한다．

引：크＝

一

c(}de．
ㅐsd 亡三＝＝뜨∼＝三쬔궉三＝＝∼三三＝三 ：三三＝크

<xsd:element name="birthdate"type="xsd:date"/>
D

: - 一code. HmI-

<birthdate> 1999-03-' 4</birthdate>
그림丘lOxsd:date 타입요소는ㅈ］간data없는xsd: time
Instant와무척유사하다．

===== PAGE 75 =====
74 =====
Defining Simple Type
c de.Hsd

5. 컨텐츠가1935년5월과같이 어떤특정한달을
의미하려면 xsd:m이itf·를 선택한다 이것은
cc,Y.Mㅆ으로 설정되어야 한다．

<xsd:element name="campaign_start"
type="xsd:month"/>
c.deJH111

6. 컨텐츠가1935와같이 어느특정한연도를의미
하려면xscl:year을선택한다. 이것은ccYY로
설정되어야한다．

.｀흐

톨麗－

<campaign_starb.1999-03</campaign_start>
그림 α끄 만일 날짜가 상콴하 없다면xsd:month 타입의요소
안에서 연도와 월만 정할수 있다．
졸灌…

codeisd些墮讐輦蘆쯔르츠三年여

8. 컨텐츠가1월 1일과같이 연도에는상관없이
특정한 달의 특정한 날을 의미하려면 xsd:
recurringdate를선택한다. 이것은－MM--DD
의 형태로 설정되어야한다. 처음 나오는 두 개
의 열 중 하나는 연도의 무시를 의미하고 나머지
하나는 분리 역할을 맡고 있다.

련，心云自－쁘芒嬖妊.'Ode"i4mI
I i_ .
ii
<Iasr_seefl> I Y" u <f lasT_seen>

그랖612 마차마Cespian tiger는1950년에 발견되었다. 월과
날짜는 알려차ㅈ／ 않았다. 그래서 연도만을요구하는 요소를 갖는
깃이논라에 맞는다．
n〕
de．
ㅐSd

lement name="greatest_Ioss「
xsd:century"/>

'grearesT_

헨C0de.
- --. - -릎琴一
9
.HmI푤
Ioss> I ye,

rearesr_uoss>

i

그람 6.1319라는 것은 2(:）세가를 설명하고 있다는 것을刀억해라．
다ㅈ］
말해1900-1999사아의 연도들（아 가간동안 전세계 96%의
호랑./.7／사라겼다）
.
code.nsd' =－一구＝ <xsd:element name="birthday"
type="xsd:recurringDate"/>

ㄱ뉵

.cbirthday>--03-14.c/birthday>
그랖 6.14 연도는 상관없으나 월과 일아 관련아 있을 때는xsd:
recurringDate를 사용한다．
톨阿…

9. 컨텐츠가매월 6일같이 연도, 월에 상관없이 특
정한 날만을 의미하려면 xsd:recurring Day를
선택한다. 이것은－DD로 설정되어야한다（처
음 세 대쉬중 두 개는 무시하는 부분을 표시하고
나머지 하나는 분리하는 역할을 하고 있다）
.

V Yip
■u'rc（세계협정시）
는국제 시간 협회에 의해 정
해진 것이고 이것은 그리니치 시간과 같은 것이
다. 미국의 동부 시간 (EST）
은 UTC-5이고 태평
양시간은UTC-8이다. 대부분의 서부유럽의
시간은UTC+1이고, 러시아는｛JTC+10, 일본은
TJTC+9, 호주는UTC+10이 된다. 웹사이트
(p18 참조7에 세계 각 지역별 시간이 나와 있다．

eode.isd 손礫＝크斗봇궂슭中令뇹수놈＝논． 훑

<xsd:element name="payday"
type="xsd- recurringDay"/>
霙圄

c1}de.11'n1

<payday>---30</payday>
그림615 叫달 같은 날짜에 발섕하는 아벤트에 대해서는xsd:
recurringDay를 사우한다．

예제의소스 코드는 www.cookwoocL corn에 있습나다．

79

듬 ＝ 口。 。*m。 ＝｀얽크m뻐겸g

<xsd:element name="Iast seen"
type="xsd:year"/>

7. 컨텐츠가1900대와같이 어느세기를의미하려
면xsd:century를선택한다. 이것은cc로
（이것은 20세기가 19로 나타난다）설정되어야
한다．

===== PAGE 76 =====
75 =====
Chapter6

숫자 타입 이용하기

프臘근一프璽료各毛－

XML 스키마는 요소의 컨텐츠나 속성을 제한하기
위해서 사용 (p76의 3번）할수 있는 여러 가지의
고유숫자타입을가지고 있다. 또 이런 타입들은
자신의 숫자 타입을 만드는 기초로 이용할수 있다．

<xsd:element name="density"
type="xsd:decimalV>
그랖 6.16population(주거）
에 대해서는음수가 아닌 정수룔
요구하는 것아 더 정확한 것이다（양의 정수는 적당하자 않은 것아
다. 왜L하면 불행하도 값아 0아 된다면xsd:positivelnte. density 요소（아것은
ger 가 87락하차 않을 갓아가 때문이다）
주거지역i평방 킬로α］E／이］얼아나 많은 동꿀들아 살고 있는자
알려주는J는 소줏점의 정확성까자 필꾜로 한다．

숫챠의 이용법：

<popolation>342</population>

2. 542나－7과같이 소수부분이 없는양이나
음의 숫자를 포함하는 컨텐츠를 한정하기 위해
서는xsd:intege
『를 사용한다．

<density>4 2</density>
그림缸7population아 0아나그 아상안 요소는 유효한 것아
다. density는 분수나 정수 둘 다를가질 수 았다．

3. xsd:positivelnteger (1, 2등등）
을사용한다．
x$d:ne9아iv이n始ge
xsd:negativelnteger
『 (-1,
(-l, -0 -등）
,

cotte.sml 三－

m＝

스노

/population>

위와 같은 종류들의 숫자를 제한하기 위해서는
아래와 같이 사용한다．
4. 43e-2와같은32bit부동소수점을포함하는
컨텐츠를승인하기 위해서는xsd:float을사용
한다. 여기에는 양과음의 0 (0, -0）
과 양과음의
무한대 (ll'w, -INF）
는포함되지만일반적인
숫자들은 포함하지 않는다．
5. 64bit부동소수점을포함하는컨텐츠를승인
하기 위해서는xsd:double을 사용한다．

i/ Tip

■ http.I/www.w3.org/TR/xmischema-2／에는
몇 가지 다른 종류의 숫자 타입과 지금 여기서
설명된 것들의 더 자세한 사항이 들어있다．

80

7<

xsd:nonNegativelnteger (0, 1, 2 **)

_王

OP이베On>
<population>112.5</population>
<density>

m
● 묘H， ●，ㅌ。＝m= ==

1. 4. 26, -100, 혹은0과같이 양수이거나, 음수이
며 소수점 아래 한정되어진 자릿수를 가진 숫자
들을 포함한 컨텐츠에는xscl:decimal을 선택
한다．

xsd:nonPositivelnteger (0,-1,-2 등등),

c.de.H$d

<xsd:element name="population"
type="xsd:nonNegativelnteger"/>

그랖 刪8 여가서보여진population（추거7의 컨텐츠가그렇둣
정수가소수부분을가치지못하기 때문에2 population ,조
는유효하차꼿하다. density요소는여전하유효하다. 왜나하면
수가분수 부분을 가질 수 았기 때문이다. 그러나 꼭 가져아 하는
것은아나다．

===== PAGE 77 =====
76 =====
Defining Simple Type
트甘∼三自＝三j프긺

三二 딥 -{

Code,aisd

단순한 주문형 타입 작성하기

<xsd:simpleType name="zipcodelype'>

XML Schema 언어는 고유하고 단순한 타입들을
포함하고 있기에 특별한목적에 따라 이런 타입들을
많이 확장할 수 있을 것이다．

<xsd:restricton base="xsd:string">
<xsd:pattern value="\d{5} (-\d{4}?"/>
</xsd:=restriction>
</xsd:simpIeType>

단순한 주문형 타입의 직성법：
그림6.19여가에zip-codeType 아라불리는새로운타입을
안들었다. 아새로운 타입은xsd: string 타입의기초를 갖고

1. .cxsd:simplelype을입력하여단순한주문형
타입의 정의를 시작한다．

있．
고 선택걱오忙｝
이픈과4개의부가적인 정수들아 따라오는 다섯
자리수로 요조의 컨텐츠를 제한하는 파턴을 포함한다．

蠟

훰町七＝」攝一丘三＝巧民Code.Hsd

<xsd:element name="zipcode"
type="zipcodeType"/ minOccurs="1">

ㅈ除할수 았다. 여7/서는loip에 나오는minOccurs속쟝 (싸
의요소가 몇 번 나타나는차 결정하가 위한속성；）을 설명할 깃이다．

＝口7

pcode>45632</zipcode>
目野一翌뇰三－一큐드r=:＝길斗i갚m1河,lflf-

4. 새로운주문형 타입을 정의하기에 필요한모든
제한점을 명시한다 (p84-90 참조？.
5. </xsd:restriction＞을입력한다．

5薑꺼；=，크；
＝긴什躇측美철
「灌

<zipcode>42398-0987.</zipcode>

6. </xsd:simplelype＞으로단순한주문형타입
정의를 마친다．

그림621아 zipcode 요소들 5두 우효하다．

V Tips
r匹 寸

--

三

뻑驪囊c.d.. HnH

<zipcode>4398- 1 2349</zipcode>
Code.I1in뀀 멸嘗

百클

pcode>
,1쾀 6.22 두 개의 z ipcode 요소들S두 유효하자 않다．첫빈째
걋은 4자리의줏자 아후에 하나의 하이픈과 다섯 자라의줏자가
따라온다. 두번째 것은 비록 이것ㅇ/ Manas Tiger Reserve 근처에
있는 인토의 Guwahati의 실제우편번호아가는 해도 패턴을 따르
자 않았가 때문어］유효하차 못하다. 口／국 외의우편번호를 조절하가
위해서새로운요소를 만드는 것아 괼요할 것이다．

예젱의소스 코드는 www.cookwoc1,com叩 있습나L士

■ 독자들이 한 번 정의했던 단순한 주문형 타입은
p76의 3번 마지막에 묘사된 것 같이 사용할수
있다. xsd:1aie1로 설명되어 있지 않고 단지
label로 설명되어 있다는 것에 주의한다（그림
6.20).
■ 또한하나의요소선언에서무명의단순한타입
들을 만들 수 있다.
■ 단순한타입의 리스트또한만들수있다. 더
자세한사항은 p90의리스트 타입작성하기를
보면 된다．

81

륭

1스二二－…＝＝∼－:r｝荳길＝ c de．
.ㅐ
`1m빵 ＼∼∼

3. <xsd:restricrion base="foundationu1>을
입력한다. foundation 자리에는 주문형 타입의
기초가 되는단순한 타입이 들어간다.

탑
一

.1甘 620요소 선언에서 (p76참조？새로운 zipcodeType을

2. name키.bd"＞을입력한다川）
e／에서는새로
운 단순한 주문형 타입을 밝혀주게 된다（그러나
요소의 이름은 아니다. 왜냐하면 그 타입은 하나
이상의 요소에 사용될 수 있기 때문이다）
.

===== PAGE 78 =====
77 =====
Chapter6

무명의 주문형 타입 사용하기
모든 주문형 타입에 이름을 붙일 필요는 없다. 특정
요소 설정을 위해 하나의 타입을 사용한다면 그 요소
와 그 타입에 관한 중복된 설명을 생략할 수 있다．
무명의 주문형 타입을 정의하고 사용하기

m
● 鷺 H ㅌ 。*g닐m。 。ㅌ，＝。＝<m＝ 名＝

1. <xsd:element name="IabeI"＞을입력하여
요소 선언을 시작한다. labe/ 자리에는 선언하고
있는 요소의 이름이 들어간다. 다시 말해 XML
문서에서 이것은 (label〉처럼 보이게 될 것이다．
2. <xsd:sim이elypes＞라고입력한다．
3. <xsd:restriction base="foundatton '>이45L
입력한다. foundation 자리에는 주문형 타입을
만들고 있는 단순한 타입이 들어가게 된다．
4. 새로운주문형 타입을정의하는데 필요한가능
한 많은 제한점들을 정의해야 한다．
5. </xsd:restriction＞을입력한다.
6. </xsd:simplelype＞을입력하여새단순한
타입의 정의를 마친다．
7, 마지막으로＜/xsd:element＞를입력해무명의
단순한 타입을 가진 요소 선언을 마친다．

I, nPS
■ 물론 이것은주문형 타입들에 관해서만유효하
다. 고유타입에서는타입의 속정을갖고 타입을
설명해야한다．
■ 이름이 있는 타입과 이름이 없는 타입의 유일한
차이점은, 이름이 있는타입은속성을이름에
설정함으로써 여러 번 사용할 수 있다는 것이고，
무명 타입은 그것을 포함하고 있는 요소들을
위해서만 사용할 수 있다는 것이다．

82

！그

n〕
de.Hsd

陋클

<xsd:element name="zipcode「>
<xsd:simpleType>
<xsd:restriction base="xsd:string'>
<xsd:pattern value="\d{5} (-\d{4}?"/>
</xsd:=resfriction>
</xsd:simpleType>
</xsd:elemen쫠>
그림 6.23 여가에 나오는요소 선언과pBl에 나오는그림 釘鮮／
그림 6.20에의복잡한주문형 타입 정의와요소 선언의조합을
바교해보자. 두 여）
제에 나오는 zipcode요소의 겋의는 동일하
【구. 근본적인 차이점은 위에저 보여진 복잡한주문형 타입은 다른
요소.朔］
는 다사 사용될수 없다는 점ㅇ／다 6<sd: simpleType
요소가 그것을 설명하고 았는 이름ㅇ／ 어떻게 없어지게 되었는자
주목하자）
.

===== PAGE 79 =====
78 =====
Defining SimpeType
二J

1푿긷 m

回

e.ㅐ＄d

<xsd:element name="continent">

수용 가능한 가치값 세트의 지정
XML 문서를 일관되게 만들기 위해서는 하나의
요소 혹은 속성을 수용 가능한 값들로 한정하기를
원할 것이다．

<xsd:simplelype>
<xsd:restriction base="xsd:string">
<xsd:enumeration value="Asia"/>
<xsd:enumeration value="Africa"/>

새로운 수용가능의 가치값 세l트 지정하기

<xsd:enumeration value="Australia"/>
<xsd:enumeration value="Europe"/>
<xsd;enumeration value="South America"/>

2. vdue='놔ioice"을입력한다. choice자리에는
그 요소나 속성의 컨텐츠를 위한 수용 가능값이
들어가게 된다．

<xsd:enumeration value="Antartica"/>
</xsd:restriction>
</xsd:simpleType>
</xsd:elemenb.

3. /＞으로xsd: enumeration요소를마친다．

그림 6.24 continents소는 아러한값들의 하나를가질수

4. 요소나속성이 가질수있는부가적인값들에
대해 1-3번을 반복 적용한다．

았다．
日 톤和－一

寸딩毛

code.Hnn

r町｀
－켜갸m于＋+n-＝
끽뢰

<continent>Asia</continent>
그림6.25continent요소는 완벽하게 유효하다. 왜냐하면 이깃
은 열7／된 선텍권들叩 상끙되어야 하가 때문아다．

V Tips
■ 부울표현식을제외한모든단순한타입에서
xsd: enumeration 제한을쓸수 있다．
■ 각각의 계산값은 반드시 고유값이어야 한다．

1 =-=＝츤＝

觸尋

nent>

乍1]

c1〕deJnn1寺도＝亞三互三三三一· 轉
Americac/

-<continent>

■ 계산값들은빈공간을포함할수있다．

continent>

그림α26 여기에 나오는 continent요소는 모두 유효하자 꼿하
다. 첫번째것은 하나밖에 87용되지못한때에두가자 선택권을포
함하고 있다. 두번째 것은 단치 하나의 선택권의 부분일 뿐아다（전
세계의 많은 부분에서 '4me [ca 는 하나의 대륙으로 간주되고 았
는 반면에 ㅇ／곳에 열가되어 있는 리스트에서는 단차 열가되어 았는
뒤7/f 가치값의부분으로 나타나 있을 뿐아다. 따라서이자제르는
유효하차 못하다）
.

예갰의소스 코드는 www. cookwood. corn에 있습나다．

83

盼亡m驪*丘＝ 볍小m4。 *>^＾●찧口口首 ＜口＝ ●
m

:1. 주문형 타입 선언에서는 (p81의 4번）.cxsd:enumeration＞을 입력한다．

cxsd:enumeration value="North America"!>

===== PAGE 80 =====
79 =====
Chapter6

.（마침표）어느 글자에서나 사용할 수 있는 것
\d 모든 숫자；\D 숫자가 아닌 것

<xsd:pattern value= INV #99\d{3}"/>
</xsd:restriction>
</xsd:simpleType>
</xsd:element>
］라한괘탄은invoice_number 요소를ThW#99
.2림丘2캬）
사작하고 세개의자릿수를가진 가호열로 한정한다. regex 안에
았는 어딴 글자도 우효화된요소의 컨텐츠 안에같은 자라에 나타나
아 한다．
艮1

｀노짓도＝길rj耳亢핑‘
ode.HmI ＝토르三프＝=＝길＝

number>INV #99426<

number>

/invoice_

다음으로value= 'regex" 를 입력한다. regex
자리에는 컨텐츠의 모양과, 다음 사항들이 어떻
게 만들어 졌는지에 관한 표현이 들어가게 된다．

<xsd:simplelype>
<xsd:restriction base="xsd:sfring">

-<invoice_

1. 주문형 타입 선언에서 (p81의 4번）＜겨5d:pattem을 입력한다.
2.

그림 6.28 여刀에는 그림 6.27에서보여진스7／마의부분에 유효한
여］아다. 여가저는 단자 뒤에세자라수가 붙는 7NV#99"가 필요할
뿐아다．

\$ 모든 빈 공간（스페이스 탭, 새 줄, 리턴 등）
;
'S 빈공간이 아닌 어떤 글자들

＝士
Code, H$d 풋포珏프→＝쏘ㅊ」各）

<xsd:element name= 'gestation">

x* 0혹은이상의x를갖는경우；Ixy)' 0이나
그 이상의 xy를 갖는 경우

<xsd:simpeType>
.cxsd:resfriction base='xsd:timeDuration">
<xsd:pottern value="P\d+D' I>
</xsd:restriction>

x? 하나혹은 0개의x를 갖는 경우；(xy}? 하나
혹은 0개의 xy를 갖는 경우

</xsd:simplelype>
</xsd:element>

x+ 하나 이상의x를 갖는 경우；( (y)+ 하나 이상
의 xy를 가질 때

그림 6.29 다른 타입을 기초로 한요소의 컨텐츠를조절하가 위하
（주 단위나
패텬을사용할수 있다. 예룰들어 날짜로 된호랑이의
월 단위가 아나다）임산 기간을gestation 요소에포함하려면
여기에보.］는패턴을설정할수있다. 아파턴은타입아원하는
것을 '아례87슨' 것이 아나다. 아것은컨텐츠 하나혹은줏자가
따라오는「〃문자P를 포함하고 았는 깃을요구한다．

！毗）c] 값 (a,b,c）
의 그룹의 하나를 포함하는 경우

code.HmI

Pl11

[0뀌 0부터 9까지의 값 범위를 포함할 경우

그 ,`

,

團霽

-" " " h' "' 이08D</gestation>
U

유
●옰H을ㅌ ㄵ。，。*E으* 。｀。m＝ 횬＝ ●

유효화 되기 위해서 컨텐츠는 패턴과 상응하는 패턴
을 만드는 언어（리젝스 (regex)－일반표현 언어）
를
사용할수 있다. XML 스키마에서의 리젝스 언어는
Pen1의 일반 표현 언어를 기초로 한다. 여기서 이
일반 표현 언어에 관해 설명하기에는 분량이 너무
많으므로 간단한 요약으로 설명을 대신하기로 한다．
단순한 타입을 위한 패턴 정의하기：

巨

c de.HSd
口
<xsd:element nome=∥invoice number>

단순한 타입의 패턴 정의하기

그림 &30 여가저는 그림 6.29에보여진 스7／마에 알맞는 유효한
보가가 있다．

84

===== PAGE 81 =====
80 =====
Defining Simple Type
code.I4sd∼囊二與一每
口一∼
<xsd:element name='Ianguoge'>

<xsd:simpleType>
<xsd:restriction base="xsd:string">

什115 I 小야 여기서는수직 막대로부가적인
선택권을구별한다．
x{5｝
는 정확하 5개의x를 포함한다（연속적

</xsd:restriction>

x{5,} 적어도 5개의 x를 포함한다（연속적으로）
川5,8}최소 5개최대 8개의 x를포함한다
（연족
적으로7.

</xsd:simpleType>
</xsd:element>
그림631요소의 컨텐츠에 선택권을 제공하는 패턴을 사용할수
았다. 선택권을계공하는보다표준적인 방법은그들을 열거하는
것아다 (PS3).

（느三二亡＝玗iF；긷＝三｀5
?f= 4三＝

= ` `
=r겯
쩍
X＝
毛｀
： 三 ==
手莫4二i
鑿
츠， → =
=＝길三＞
1 = `

>

그랗 6'32그림6.31叩 나오는스카마의우효한 예가 여刀에도 있다．

{xyz}{2］
는 정확하 2꺼의xyz를 포함하고
（연속적으로）괄호들은 구부러진 괄호와 다른
수정 기호 (?,+ 그리고 *) 등의 영향을 조절한다．

I, nPS
■XML 스키마와 Penl 일반 표현식과의 중요한
차이점은 요소의 이전 컨텐츠를 비교하여 발견
할수 있는데, xM. 스키마에는 Pen 일반표현
식에서 볼 수 있는 줄의 시작과 끝에서 매체로의
전환을 제어하는 ^ 기호와 $ 기호 등이 없다．
■ 더 이상 일반 표현의 세부 사항을 기술하는 것보
다 그에 관련된 책을 소개하는 것으로 마무리를
하려고 한다. B&B에서 나온 퀵스타트 Pen and
（〕
（뀨를참조한다. 여기에는좀더 많은예제와
배경 지식들이 있을 것이다. 그리고 Penl 일반
표현에 대해서는 h山)://www.penl.corn!
pub/doc/manual/htrn꺄tod/perlre.htrn／에서
찾을 수 있을 것이다.

여］제의소스 코드는 www.cookwood.com o/f 있즙나다．

85

읗m쇽뜁＝ ．。！。＝旦＝ *。，。닉클프m검경

<xsd:pattern value="English I Latin"!>

으로）
.

===== PAGE 82 =====
81 =====
다iapter6
1」갼
code.Ksd
<xsd:element name="population">

가능한 값튤의 범위 정하기
속정이나 요소의 컨텐츠를 제한하는 다른 방법은
그것이 가질 수 있는 최고의 값 또는 최저값（혹은 둘
다）
으로 정하는 것이다．

m큭

<xsd:simplelype>
<xsd:restriction base="xsd:integer'>
<xsdrmaxIncIusive value= '5000'/>
</xsd:restriction>

,陪한 최고값의 지정：

그림螺昭xsd:maxlnclusive 제한점은하나의요소에가능한
최고차의값을정한다．

2. value="n"이라고입력한다. 컨텐츠는반드시
끄 보다는 작거나 같아야 유효한 것이 된다．

乍· 릎

c de.nnd

r=

=；二

1눗

二二

흰 三

∼

/population>

-<population>

5000<

3, /＞을입력하여xsd:max-Inc1usive요소를
끝낸다.

＇dd1n'm
三三i琵흐＝귿길횬憂二二一竇

三귑三

r＝尸＝ 一느느￡핍一甘乍

<population>4999</population>

또 다묜 가능한 최고값의 지정
1. 주문형 선언안에서 (p81의 4번）cxscl:maxExdusive (Exclusive 단어에서 대문자 E를 주의）
를 입력한다．

그림 丘34 여가의population 요소들은 유효하다．왜나하면
첫번새는xsd:maxlnclusive 값과같고두번째는 xsd:
maxlnclusive보다 작기 때문아다．

2. value="n''을입력한다. 유효화되기 위해서
컨텐츠는 반드시 끄 보다는 작거나 같아야 한다．

아｀de,i1 d
<xsd:element name="populotion">

<xsd:simplelype>
<xsd:restriction base="xsd:integer">

3. /＞을입력하여xsd:max-Exclusive요소를
끝낸다．

<xsd:maxExclusive value="5000"/>
</xsd:restriction>
</xsd:simplelype>
</xsd:element>
.2림6.35xsd:maxExclusive 제한점은 받ㅈ）匿여질 수 없는
최소값을정한다. 다지 말해요소의 컨텐츠는xsd:maxExclusive값보다 적어아 한다（같아저도 안된다)

codej{ml

5000<

/population>

population>

溺
旨日i<

=
m
● 오口＞ e

</xsd:simplelype>
</xsd:element>

1. 주문형 선언안에서 (p81의 4번）<xsd:max
Indusive (Inclusive에서 대문자 I를 주의）
를
입력한다．

- 阡=＝一슬三ㅌ三

=b줄三＝斗三i표三쬔＝仁ㅎ섶三i t돋

<population>4999.c/population>
그림 6.36 첫빈째 population요소는 유효하자 못하고 두번째는
유효하다．

86

===== PAGE 83 =====
82 =====
Defining Simple Type
回

coile.ssd

<xsd:element name="start date">

7侖한 최저값의 지정
1. 주문형 선언안에서 (p81의 4번）<xsd:
mininclusive (Inclusiv쩨서 대문자 I주의）
를
입력한다．

<xsd:simpleType>
<xsd:restriction base="xsd:date">
<xsd:minlnclusive value= ' 1999-07-25"/>
</xsd:restriction>

2. value=hmn"을입력한다. 유효화되기 위해서
컨텐츠는 반드시 끄보다는 작거나 같아야 한다．
3. /＞으로，
xsd:nin-Inc1usive요소를마친다．

.2림6.37xsd:minlnclusive제한짐은요소의가눙한 최조값
을 정한다. 中／말해start_date는1999년 7월 25일아거나
그 아후다．

놓日

．量

c de.Hml

<start_date>] 999-07-25</start_date>
輦筒－→一三三됴순드＝三ㅍ＝∼，
》c ds.lim1

<start_date>] 999-07-26</start date>
.2림 638 아러한start_date 요소들은 유효하다. 왜나하면
첫번째 깃은xsd:minlnclusive 값아랑같고, 두번째 것은
그보다 크가 때문이다．

또 다른 가능한 최저값 지정법：
1. 주문형 선언안에서 (p81의 4번）<xsd:min
Exclusive (Exclusive에서 대문자 E를 주의
하자）
를 입력한다．
2. vdue="n＂을입력한다. 유효화되기 위해서는
건텐츠는 반드시 끄 보다 작아야 한다（같아서도
안된다）
.
3. /＞을입력하여xsd:min-Exclusive요소를
끝낸다．

'/ Tips
<xsd:히ement name="start date">
<xsd:simplelype>
<xsd:restriction base="xsd:date'>
<xsd:minExclusive value="l 999-07-25∥/>
</xsd:resfriction>
</xsd:simpleType>
</xsd:element>
.2림639xsd: minExciusive 제한점은가장큰거부값을
자정한다. 다사 말해꾜소의 컨텐‘츠는 반드사xsd:minExclusive

■ 같은 타입의 최저치를 동시에 사용할수는 없지
만 필요하다면 최저치와 최고치를 같이 사용하
는 것은 가능하다. 또한 하나만 사용하는 것도
가능하다．
■ 숫자라는 것은 그 대소의 구분이 확실하다. 날짜
나 시간의 경우 이것이 크다는 의미는 이후의
날짜나 시간을 의미한다. 물론 적다는 의미는
그전의 시간을 의미하는 것이다．

값보다 커아（같아／̀）도 안퇀다）
한다．
『 ∼二每珊 cods.liml

<start_date> 999-07-25</start_date>
느擡code.xml =

;-11

<start_date늬 999-07-26</start date>
그림 640 여기저 찻번째start_date 요소는 유효하자 않다
（이것은xsd:minExciusive 값과긷하서도안된다）
. 반면에
두번째 것은 우효하다. 왜나하연 이깃은.
27/ r나중）때문아다．

역］
제의소스 코드는 www.cookwood.com에 있습나다．

87

m
경
＾ =`=．。”。＝띵。 *>^^m三튜＝ ＜口百． m

</xsd:simplelype>
</xsd:dement>

===== PAGE 84 =====
83 =====
다iapter6

단순한 타입의 길이 제한
기호열이나 URL 단순한 타입으로부터 나오는 하나
의 요소를 더 자세히 정의하는 방법은 그것의 길이를
제한하거나 지정해 주는 것이다．

［j
萱

…

〔0de．
ㅐM1

<xsd:element name="animal code'>
<xsd:simplelype>
<xsd:restriction bose='xsd:string">
<xsd:length v비ue="4「／>
</xsd:restriction>

요소의 정확한 길이 정하기：

</xsd:simplelype>
</xsd:element>

읜 鷺 을 ㅌ ㄵ。*。士m＝ 잽● 츱m＝ ㅌㅌ＝

주문형 선언에서 (p81의 4번）<xsd:Iengthv이ue=
'Ix／》을 입력한다. 여기서 x는 요소가 반드시 포함
해야 하는 글자의 숫자이다．

그胃 6.41패난을 우자하는 깃이좋음에도 가호열의 길아툴 설정
할수 있다．

요소의 최소 길이 정하기：

희■－cedeJ1m1

주문형 선언에서 (p81의 4번）<xsd:mi미eng出·
VdUe="m"/＞을 입력한다. 여기서 m은요소의
글자의 최소 길이를 의미한다．
요소의 최대 길이 정하기：
주문형 선언에서 (p81의 4번）<xsd:maxlengthVdUe="n"/＞을 입력한다. 여기서 n은 그 요소의
최대 길이이다．
I', 1옵＇I5
■ 만일 길이를 지정한다면 최대치나 최소치를
지정할 수는 없다. 물론 그 반대의 경우 역시
마찬가지이다．
■ xsd: length, xsd:min-Length 그리고
xsd:maxLength는 모두음수가 아닌 정수가
되어야한다．
■ 만일 어떤 요소가 이진법 타입에 기초하고 있다
면 길이는 이진법 데이터의 8개조의 숫자를 제
한한다. 만일 그 요소가 리스트에 의해 얻어진
것이라면 그 길이는 리스트 아이템들의 숫자를
결정하게 된다．

결

<animaL-code>TlGR</animaL-code>
그림 6.42 0/ animal code 요소는 아깃이 4글자를 포함하기
때문에 우효하다（그림 6.41참조걋．
: ㅋm§
Pㅁ
.code.asd,'
<xsd:element name="description">

一月륵

<xsd:simplelype>
<xsd:resfriction base="xsd:string">
<xsd:maxLength value= '200"/>
</xsd:restriction>
</xsd:simpLeType>
</xsd:element>
그람 6.43 기호열요소가초절 불가눙한장넌蜘］되자 않게기호열
의길하를 제한할수 았다．
code.HmI 一哮姓－
培月蜀
町
<description>The tiger (panthera tigris), largest of
all cats, is one 0f the biggest and most fearsome
predators in the world.</description>

.2람 `44 아description 요소는 유효하다 .왜냐하면 이것의
컨텐츠는113글자로되어있고, 아것은200글자한계안아다．
'；動·－

code.Nmt

<description>The tiger (panthera tigris), largest of all
cats, is one of the biggest and most fearsome predators
in the world. PowerfuLL汁)uilt with fierce retractile claws
Ithey can be p얘ed into the paw, like 帥ouse cat's),the
tiger's distinctive g히d coloring with 비ack stripes 베ows
it to melt unseen into its environment.</description>
그림螺45아description 요소는유효하자 않다. 왜나하면
317 글차툴포함하고 있가 때문이다．

88

===== PAGE 85 =====
84 =====
Defining Simple Type
姃j

Code.ㅐsd

'

<xsd:element nome='numbers">

숫자의 자릿수 제한하기
숫자의 소수점 왼쪽이나 오른쪽으로의 자릿수를
결정할 수 있다．

<xsd:simpleType>
<xsd:restriction base="xsd:decimdrr>
<xsd:precision value='5"/>
<xsd:sc이e value="2"/>

숫자에서 자릿수 겹장하기：
1. 추문형타입선언에서 (p81의4번）<xsd: precision을 입력한다．

</xsd:restriction>
</xsd:simplelype>
</xsd:element>

2. value=hmn＂을입력한다여기서n은숫자에서
나타날 수 있는 가장 큰 자릿수이다．
3. /＞을입력하여 태그를마친다．
소숫점 오好의 자릿수 정하기：

,* r , U m戮
tode.uml . \\\ d , , 人，

阡g--，芦“*
"m
cnumoer5>Jo4.Jv</ numoers>
∼，
∼

∼斗戶∼｀한 ．뽄 code.ssnd 蠟式寸緻엥노쓰됴눔노ㅈㄱ－

m重

<numbors>34.5.c/numbers>
그림6.47 이두요소 다 유효하다. 그들은 촤甲 다섯자라릍포함하
고 있기 때운이
［卄간혹 적을 수도 있다）
. 그리고 분수 (수）
부분의
촤甲두 자라 혹은 ㅇ／것보다 적은 것을포함하고 있刀 때문아다．

驢
m

.d8.HflH

-

mbers>1476.32</numbers>

阿나―

t deJ11쟈1

<numbers>4.3987</numbers>
2람648이두줏차요소들은유효하자 않다. 칫번째는자릿수（'6)
가 넣은 경우ㅇ／고, 두번째는 적당한자랏수 ('5)를 가졌음에도 불구
하고 너무 많은 소수 자랏주를 가차고 았刀 때문아다. 4711가 아나라
2갱가되아한다．

1, 주문형 타입 선언에서 (p81의 4번）<xsd:sc이e
을 입력한다．
2. vdue="n"을입력한다. 여기서n은소숫점
오른쪽에 나타나는 가장 큰 자릿수이다．
3. /＞을입력하여 태그를마친다．

I, nPS
U xsd:precision의 제한점은 반드시 양수 (1,
2, 3 혹은 더 큰 수）
여야 한다. 이것은 0이 될 수
없다. 그리고xsd: scale 값보다작을수 없다．
U xsd:scale의 제한점은음수가될 수 없다 (0,
1, 2, 혹은그이상）
.
■ xsd:precision과xsd: scale 둘모두최대
값을 제한한다. 만일 더 작은 자릿수가 존재한다
면 그 숫자는 유효한 것으로 간주된다．
■ xsd:precision과xsd: scale은숫자의
형태로 정할수 있다（기호열, 날짜등의 타입은
제외）
.

예제의소스 코드는 wws. cookwooiicorn에 있습나다．

89

＝亘＝ ＝山。 ＝．클口m큐므욜m

2쾀6.46 precision값은총자릿수를결정한다. scale은
소수첨오른쪽 (수부분）
에저 얼마나 많은 자릿수가 나타나는자
를결정한다．

===== PAGE 86 =====
85 =====
Chapter6

리스트 타입 작성하기
이제껏 언급한 요소들은 하나의 개체만을 포함할 수
밖에 없었다. 만일 하나의 요소를 날짜로 정의한다면
그 요소는 단지 하루만을 포함하게 된다. 그러나 전
리스트의 날짜를 포함하는 요소가 필요하다면 상황
을 편리하게 하기 위해 날짜 타입에서 리스트 타입을
끌어낼 수가 있는 것이다．
리스트 타입 작성하기：
1. <xsd:simHelype을입력하여 리스트타입의
정의를 시작한다．
너
● 口鷺* 쓰dm＝ 님 ● ，U

2. name=hhlobelhl＞을입력한다. label자리에는
선언하고 있는 요소의 이름을 입력한다. 다시
말해 XML 문서에서 <label）
과 같은 것이다．
3. .cxsd:Iist base="inclividud"＞을입력한다．
individua/ 자리에는 리스트의 각각의 값을
정의하는 단순한 타입의 이름이 들어가게 된다．
4. 필요한경우xsd:length, xsd:minlength,
xsd:rnaxLength (p88 - ；고) 와 xsd: enuineration과 같은 제한점을 가지고 리스트를 제한
할 수 있다．
5. </xsd:Iist＞를입력하여 리스트정의를마친다．
6. 마지막으로＜/xsd:sim이eType》을입력하여
단순한 타입 정의를 마친다．

'/ nP`

■ 리스트를더 제한할필요가없다면4-5번과정
을 생략하고 /＞으로 xsd:list 요소를 마칠 수
있다．

■ 리스트타입은단순한타입으로만기초를삼을
수 있다（복잡한 타입은 될 수 없다. 복잡한 타입
은 다음 장에서 다룰 것이다）
.
■ 공백이 리스트의 아이템 수를 결정하기 때문에
기호열 중심의 리스트 길이를 정할 때는
주의를 요한다．

90

섶룐芸 c d.."$d

<xsd:simpleType name"datelist">
<xsd:list base="xsd:date"/>
</xsd:simplelype>
<xsd:element name="list_of_birthdays"
汐pe="datdi5t"/>
그림 6.49 '/스트는 반드사 아라 존재하고 있는고유의 단준한
타입에 7/초해야 한다. datelist 라즈트 타입은xsd: date
타입을 기초로 하-ii 았다. list_of_birthdays 요소를 선언
할 때새로운고유의 단순한 타입을 사우했음을 주의하자．

code.HnH 긔
곁
＇
dist_of_birthdays>1893-04-20 1904-05-11
<luist_of_birthdays>

…陋＝

그림6.50 이유효한 예제와 같이 라스트는 빈 공간으로 구별되고
기본 수섶으로 정해진 타입에 0 흑은 그 이상의 값을포함하고 았어
야 한다．

쾨릍＝芒노조긍슨半쵱＝ =＝릍 code.Hsd 騙쪼＝玉스蘆스二公二- -'== - - m료

<xsd:simpleType name="three_datelist">
<xsd:list base="xsd:date">
<xsd:length value="3"!>
</xsd:Iist>
</xsd:simplelype>
<xsd:element name="Iist_of_3_birthdays"
type="three_datelist"/>
Z림6.51xsd: length, xsd:maxLength, xsd:minLen
gth, 그리고 xsd: enumeration 제한점을가ㅈ／．고리스트
한할수 있대
타입을 더세밀하겨）저）
-=-,1r｀
콘｀ ！쯔主뇬논，
쁜r=1ct)de.Hnn 돌旨三

一

ist_of_3_birthdays>1893-04-20 1904-05-11
1852-06-25</list-of_3_birthdays>
그림 6.52 list_of_3_birthdays가 유효화되가 위해저는
반드사 세개의 날짜틀 포함해아 한다．

===== PAGE 87 =====
86 =====
Defining SimpleType
돌．
∼每三騙拿뜨

c0de.11$d 뜁

1크』

<xsd:element nome="status「 type="xsd:string"
fixed="endangered"I>
그림 α弱status 요소가X71工L 문저에 등장ㅎ梏 한 반드사
"endangered" 가호열을포함해아 한다 (은 빈공간아거나 빈
.
경우 endangered' 7／호열을포함하는 것으로 간주한다）

Code.Hn`` 걍흴콜∼＝∼ -

= 1…三＝:1」 1

요소 컨텐츠 미리 정하기
요소의 컨텐츠가 무엇인지를 미리 정하기 위해서
스키마를 사용하는 방법에는 두 가지 방법이 있다．
요소의 컨텐츠를 지정하거나 혹은 XMl.에서 요소가
빈 공간으로 나타날 경우 요소에 대한 가치값을 정할
수 있다. 전자의 것을 고정값이라 하고 후자의 것을
다폴트 값이라고 한다．

그림 6.54 그림 6.53의스카마 데이터와 비교할 때 아 StamS 요소
는유효하다. status 요소가없을경우에도유효한것은마찬가
又］다．

요소 컨唯 지정하기：
1. 요소태그사이에fixed＝를입력한다．
2. 그리고나서 " Vdue"를친다. value자리에서
요소의 컨텐츠가 어떤 것이 될지를 밝힌다．

돎m

d*de.1섶1t11

<status>v이nero비e.</st아us>

요소의 처욥 i媛 설정하기：

그림 6.55 그림 6.53의주아잔 선언에서는 유효한 status.9. 가

1. 요소태그안에서default＝를입력한다.

아나다．

2. "v이ue＂를입력한다. value자리에는그요소
가 생략되거나 공백으로 남겨져 있을 경우 자동
적으로 설정되는 요소의 컨텐츠값이 오게 된다．

닐

Code.Ksd

뗘

<xsd:element name="status" type="xsd:string"
default="endangered"/>
그림丘拓status 요소를 다폴트 값으로 정의한다면그 값은
status 요소가xML 문서에 명백하게 등장하는 여부에관계없아
처음 컨텐츠로 설정돤다．

口

壤

c.de.1nm 一콰흘ㅋ∼ 길二＝兵i三二毛三르回

<status>endangered</status>
（
mde．
川｝
H 葛돝一塔좋單驀蕁囊茹百

tatus>vulnerable</s쫠aius>
그림螺57아status 요소들꼬두유효하다. 다폴트족성은처음
값으로만 설정되고 다른 값들도 역시 받하들여질 수 았다．

'/ Tips
■ 그 요소가 XML에 등장하게 된다면 고정 속정은
단지 컨텐츠를 설정할뿐이다. 생략되었을 경우
설정되는 컨텐츠는 없다．
■ 고정 속정이 설정되고 그 요소가 비어있다면
요소의 값은 자동적으로 고정값으로 설정된다．
■ 디폴트값이 설정되었지만요소가XML에서
생략되었다면 요소의 값은 자동적으로 디폴트
값으로 설정된다．
■ 디폴트속성이 설정되고요소가XMT.에 나타난
다면 이것의 컨텐츠는 제한되지 않는다．
■ 디폴트속성과고정 속정을동시에 설정할수는
없다．

예재의소스 코드는 www.cookwood.com에 있습나다．

9】

珊m뭏出＝ =．。＝뭉크e＝ 츄g= *
。
＝
4

針아us>

===== PAGE 88 =====
87 =====
DEFINING COMPLEX TYPES
복잡한 타입 정의하기
':j ＝足vt죽

다른 요소나 속정들을 포함할수 있는 요소는 복잡한
타입이라고 한다. 많은 XMl 문서들이 다른 요소들
을 포함하는 요소들을 가지고 있기 때문에 스키마 안
에서 복잡한 타압을 만들어야 하는 경우가 발생한다．

〔0de.HrnI

<S沚》spedes>

<region>Far East Russia</region>
<population year="1999">445</population>
c/subspecies>
그림 7.1 subspecies 요소는 다른 요소를포함하치만느슨한
텍스트는포함하자 않는다. 아 부분요소는 속성을 가지고 았차는
않지만가질 주는 있다. 아깃을요소만을포함하는요소라고 한다．
－唾
4毒code.jimi 纛－
<source sechonid=「101"newspaperid="21'7>

劉찮－卞

1래

<picture filename="tiger.jpg" x="200" y="197"/>
그림 7.2소스 (source) 와그림 (picture) 요소들은 빈요소

복잡한 타입의 요소에는 4가지 종류가 있다：요소만
을 포함하는 (element only) 요소 - 이것은 다른
요소들과 속성들을 포함하고 있고 텍스트는 없다
（그림 7.1). 빈 (emp缸）요소 - 속성들을 포함할 수
있는 요소. 그러나 요소나 텍스트는 없다（그림 7.2).
혼합 컨텐츠 (mixed contents）
는 요소와 속정 and!
or 텍스트 등의 조합을 포함하고 있다. 특히 텍스트
만을 포함하는 (text only) 요소는 텍스트（그림 7.3)
와 속성을 포함할 수 있다（그림 7.4). 앞으로 이 4종
류를 차례로 설명할 것이다．

들식다. 그들은 컨텐츠룰포함하고 았지 않다. 이러한특정 빈요소
들은 족정을가지；고 있다 (2금7나모두가가ㅈ］고 았는 것은 아나다）
.
code.xml
<description length="short">The <name>
language="English">tiger</name> Ipanthera
tigrisl, largest of all cats, is one of the biggest and most
fearsome predators in the world.</description>
그림 Z3 이description 요소는 텍즈E와 하나의 아름 꾜소
(성도 마찬가지이다＞1를 포함하고 있다. 이것은 혼합된 컨텐츠를
가지．
고 있다고 인식된다．

그림 Z4 name 요소는 텍스트 (2라고 하나의 속성；喝포함하고
텍스트만을포함하슨요소로 간주된다．

93

。m戮 三＝ 口＾ 。크프mX뻐겸m

<name language="English'>Amur</name>
<name languoge="Latin">P.t. oltoicac/name>

===== PAGE 89 =====
88 =====
태apter7

요소만을 포함하는 요소의 정의
대부분의 기본걱인 복잡한 타입의 요소는 텍스트를
제외하고, 다른요소들을포함하고 있거나속정을
포함하는 것이 가능하다. 이것의 컨텐츠는속성이
있음에도 불구하고 요소뿐인 것으로 묘사된다．

｀》｀,,
驪｀

, 中

－섶琴co1e.Hs.＝埠玉돌느

階彗

.cxsd:complexType nome-"endspeciesTypE >
<xsd:sequence>
<xsd:element name="animal"
type="animallype'/>
.c/xsd:sequence>
</xsd:complexType>

요소만을 포함한 복잡한 타입의 요소 작성법：
= i＝ ●
。
==0ㅌ 음 ＝ ＝。＝븝* ＝。닐。 *=＝●ㅌ으山 m

1. <xsd:comHexlype＞을입력한다．
2. name="IabeI∥을입력한다. label자리에는
복잡한 타입임을 명시하는 것을 입력한다（하나
이상의 요소의 선언에서 이와 같은 복잡한 타입
의 정의를 사용할 것이므로 이것은 요소의 이름
이 될 수 없다）
.
3. ＞을 입력하여 시작태그를마친다．
4, 시퀀스 白95참조), 선택권 (p96참；조？혹은정렬
되어 있지 않은 그룹을 선언하고 명명된 그룹을
참고한다. 이것은 이전의 3가지를 포함할 수
있다 (p99 참；조？. 이 선언의 이유는 어떤 요소가
복잡한 타입을 포함할 수 있는지를 정하기 위해
서이다.
이나이 타입에 포함될
5. 그리고속성 (p108참조）
요소 내에 나타나야만 하는 속성 그룹 (p끄1
참조）
을 선언하거나 설명한다.
6. 마지막으로＜xsd:complexlype＞을입력한다．

'/ nPS
■ 복잡한타입을 만들었다면 이것에 의해 정의된
요소를 반드시 선언해야 한다. 더 자세한 사항은
p106에 나오는 복잡한 타입의요소 선언하기를
참조하자．
■ 복잡한타입을포함한그요소들은반드시 시퀀
스, 선택권, 정렬되어 있지 않은그룹, 명명되어
진 그룹 중의 일부분이 되어야 한다．

94

그림 Z5 여71에는 복찹한 타입의 정의가 있다 (endangered_
species 요소를정의하는데 아것을사용해아 한다？. 아것은
animalType 타입을가지고 징의되는 하나의animal요소를
포함할 것아다. 복잡한 타입이 복잡한 타입의 다른 꾜소들을 포함
하는 것은 일반적이자 않다．

===== PAGE 90 =====
89 =====
Defining Complex Type
횰阿蔞蕁귤肇摯三 긺孕노肖 c.de.卄＄d

닐
＇

<xsd:complexlype name="animalType">
<xsd:sequence>
<xsd:element ref="name"minOccurs="2"/>
<xsd:element name="threats"
type="threatslype"/>
cxsd:element name="weight"type="xsd:stringV>

시퀀스에 등장하는 요소 요구하기
하나 혹은 그 이상의 요소를 차례로 포함하는 복잡한
타입의 요소를 만들려면 그러한 요소들의 시퀀스를
정의해야한다．
시퀀스에 등징하는 요소의 요구법：
1.

<xsd:element name="Iength"type="xsd:string"/>

2. 필요할경우p101에 나오는최소／최다발생치를
설정해서 요소의 시퀀스 등장 횟수를 정한다．
3. ＞를입력하여 시작태그를마친다．
4.

<xsd:element name="subspecies"
type="subspecieslype"/>

5.

</xsd:sequence>
</xsd:complexType>
그림 7.6 animalType 타입으로정의된요소는name, threats,
weight, length, source, picture 그리고 subspecies
요소를 순서대로 포함q야 한다．

<xsd:sequence를 입력한다．

시퀀스 안에서 순서대로 나타나야 하는 각각의
내용물을 선언하거나 (p78과l06p 참조）설명한
.
다（βi（刀참조）
</xsd:sequence＞를 입력한다．

'/ nP`
■XML문서 안에 나타날수 있는요소들의 순서는
시퀀스가 정하게 된다．
■ 또한시퀀스는다른시퀀스선택권（p96참조）
,
명명된 그룹의 참조 사항들 (P99 참조）
을 포함할
수 있다．
■ 하나의 시퀀스는복잡한타입 정의 (P94 참조）
또는 선택권들의 세트 (p96참조）안에서나 명명
된 그룹 정의 (p98 참조）
에 포함될 수 있다．
U xsd:seguence 요소는 DTD에서의 콤마에
해당하는 것이다．
■ 하나의 시퀀스가 단지 하나의 요소만을 포함
하는 것이 합당하다．

예겨）
의소스 코드는 www.cookwood.com叩 있즙나다．

95

"m亡듸＝ =．쯩크． =
4
． 。＞겸m묵 ＝ 旨 二 言 三 ．

<xsd:element name="source"
type="sourcelype"/>
<xsd:element name="picture"
type="pictureType"!>

===== PAGE 91 =====
90 =====
（十apter7

선택권 세트 만듣기
하나의 요소를 선언하는 것은 때로 유용하다. 따라서
이것은 하나의 요소（혹은 요소의 그룹）
나 다른 하나
의 요소를 포함할 수 있게 된다. 선택권을 만드는 것
으로 이러한 것이 가능하다．
선택권의 제공：
1. <xsd:choice를입력한다．
2. 원한다면p101에설명된최소／대발생치를설정
함으롸서 선택권 세트의 등장 횟수를 정한다．
3. ＞을 입력하여 시작태그를마친다．

Code.11$d ’…

1」

巨r

<xsd:complexType name=flanimallypeu>
<xsd:choice>
<xsd:element name="subspecies"
type="subspeciesType"/>
<xsd:sequence>
<xsd:element name="region"type="xsd:string"/>
<xsd:element name="population"
Iype="popType"/></"xsd:secuence>
</xsd:choice>...

= ＝。●，U
m
· 셩 占 * 。*●小。 m

그림 7.7 어떤 위험叩 빠진 종들은 변종을 가차고 있치 않은 것들도
있다. 만일 라즈트가 밌다면 변종cjf 관한 리스트를작성하는 것은
叫우 유우할 것아다. 또는 라스트가 없다면（아깃은 보여ㅈ］지 않았던
반면에no_subspecies 그룹은 단자 region과 population
요소들만을꼭록에 올라고 았다）모든 종叩관한 자역과 인구에 대해
딘준히작성한다．

4. 세트안에 있는선택권을형성할각각의 요소들
을 선언하거나 (p76과p106참조）설명한다
.
(p100 참조）

료－彗三ㅌㅌ三핑＝
르汪三三三ㅌㅌ三4三＝ cOde.Hnd

5. </xsd:choice＞를입력한다．

<animal><name language="English">Tiger</name>

V Tips

<subspecies>
<name Ianguage="English">Amur</name>
<name language="Latin">P.t. altaica</name>
<region>For East Russia</region>
<population year="1999">445</population>
</subspecies>
<subspecies>
<name language="English">Balian</name>

■ 최소／대 발생치 속정의 디폴트값（모두 1로 생각
한다）
이 포함된 XML의 유효한 문서는 선택권의
세트 안에서 오직 하나의 요소만 나타날 수
있다. 그러나 최다 발생 속성의 값이 1보다 클
경우 그 값은 선택권의 등장 횟수를 결정하게
된다.

</animal>

maxOccurs= "unbounded"를사용하는
것은 한 DTD에서 선택권의 세트에 별표 (*）를
첨가하는 것과 같은 것이다 (p47참조）
.

<animab.<name Ianguage="English">Greot River
이ter</name>

■ 선택권의 세트는시퀀스 안에나 선택권의 다른
세트안에서, 또는명명되어진그룹정의 안에
에 포함될 수
있는복잡한 타입 정의 (p94 참조）
있다

<region>Peru, Northern Argentina</region>
<population yeor="2000">5000</population>
</animal>

U xsd:choice요소는Dㅁ
［〕
〕안에서의수직바와
같은 역할을 하는 것이다.(p47참조）
.

96

겻즈크＝;F三j云츠三르ii놀二＝尸表느

＝섭＝一二j
0d0.HOH 군撞푿륵트긷云再：

그림 Z8 여기 나온animal요소들은 유효한 것들아다. 맨 위의
animal叩서는 몇몇 변종요소가 나타난다. 밑의animal에서는
변종 대신에region과 population 요소들로 구성되어찬
중첩된 사퀀스를 가지고 있다．

=

===== PAGE 92 =====
91 =====
Defining Complex Type
튬·j

code.Ksd

<xsd:complexlype name="subspeciesType">
<X5d:（캐＞
<xsd:element ref="name"/>

</xsd:all>
</xsd:comHexType>
.2림 Z9 ali.2툽은subspeciesType 요소 안몌저name,
region, .2라.2 popu1ation五. 가준저에관계없아 나타나
는깃을 87락한다. 덧붙여서 region요소는 아것의minOccurs
속정이 (7으로 설정돠어 았7/ 때꾼에 (p101 참：죄선텍적인 것아다．
아깃은 아무 문제없아 섕략될수 있다．

요소가 다른 요소들을 순차적으로 포함하려고 한다
면 내부 요소들을 모든그룹과 한데 묶을 수 있다．
순차적인 요소의 등장 허용법：
1. <xsd:네＞로정리되어 있지 않은그룹의요소를
시작한다．
2. 필요에 따라101페이지에설명된minOccurs/
niaxOccurs（최소／다 발생치）
를 설정함으로써
정리되어 있지 않은 그룹의 등장 횟수를 명시
한다．
3. ＞을입력하여 시작태그를마친다．
4. 정리되어 있지 않은그룹내에 있는각각의 요소
들을 선언하거나 (p76과p106 참조）설명한다
(P加0참조）
.
5. </xsd:네＞을입력하여그룹을끝낸다.

髥픈1 C de,ㅐ

<subspecies>
<name Ianguage='English">Bengal</name>
<population year="1999">3159</population>
<region>lndia</region>
</subspecies>
<subspecies>
<population year="1998">1227</population>
<name language="English">Amoy</region>
</subspecies>
.2림z꼬아subspecies 요소들둘다유효한것들아다. 왜냐
하연region은 선텍사항이.2 준사는 중요하차 않까 때문아다．

여］제의소스 코드는 wwv,.cookwood.corn에 있습나다．

V 1iF小
■ 모든그룹의 멤버들은 이름과는달리 단한번만
등장하거나 전혀 등장하지 않는다（그 멤버들의
minOccurs와maxOccurs 속성에 기인한다）
.
■ minOccurs와ㅍsaxOccurs 속성들은 () 또는 I
로 설정되어 있다．
■all 그룹은 개별 요소 선언과 설명을 포함할 수
있지만 다른 그룸들은 포함하지 못한다. 더불어
어떠한 요소도 한 번 이상 나타나지 못한다．
■ a끄 그룹은 단지 포함될 뿐이다. 그리고 복잡한
타입 정의 (P94 참조）
나 명명된 그룹 정의 (p98
참조）
의 유일한 자 (child）
가 될 수 있다．

97

브百트＝ ．쯩크m= =4。 ＞召． 。， =>＝녘。 ，뭏떽

<xsd:element name="reglon"
type="xsd:string"minOccurs="0"/>
<xsd:element name="population">
<xsd:complexlype base="xsd:integer"
derivedBy="extension">
<xsd:attribute name="year"
type="xsd:year"/>
</xsd:complexType></xsd:element>

순차적인 요소의 등장 허용하기

===== PAGE 93 =====
92 =====
（十apter7

명명된 그룹 정의하기
XML 문서 여러 곳에서 요소의 컬렉션이 함께 나온
다면 그것들의 설명을 용이하게 하기 위해서 그룹으
로 묶을 수 있다．
명명된 그룹 정의：
1. <xsd:group을입력한다．
2. name="Iabd∥을입력한다. label자리에는
이 특정 그룹을 확인할 단어가 들어간다．
3. ＞으로서 시작태그를마친다．

昱
＝e
。 경ㅌ 。
＝
m
= 뎡
。
＝
m

4. 명명된그룹을형성할시퀀스들（p95참조）
,
선택권들의 세트 (p.96 참조）또는 정리되어 있지
않은 그룹 (p97참조）
을 선언한다．
을입력해그룹정의를마친다．
5. </xsd:group》

'/ nP`
■ 하나의 그룹은 DTD 안의 매개체에 해당한다．
■ 하나의 그룹은스키마의 높은 레벨에서만 정의
되는 반면 (xsd: schema 밑에서）여러 상황에서
설명될 수 있다 (P99 참조）
.
■ XML스키마설명에서는시퀀스나선택권세트
의 정리되지 않은 그룹, 그리고 명명된 그룹을
설명하기 위해서 group（그룹）
이라는 단어를
쓰거나 가끔 model group（모델 그룹）
이라는
용어를입력한다. 여기서는xsd: group 요소
로 정의된
（따라서 이것은 이름을 가진 요소이다）
요소의 컬렉션을 설명하기 위해 named group
（명명된 그룹）
을 사용한다．

98

口

三눗→i斗－code.Hsd F:

<xsd:schema>
<xsd:group name="physical_truits'>
<xsd:sequence>
<xsd:element name="weight"type="xsd:string"/>
<xsd:element name="Iength"type="xsd:string"/>
<xsd:element name="gestation"
ype="xsd:timeDuration"/>
<xsd:element name="distinguishing"
type="xsd:string"/>
</xsd:sequence>
</xsd:group>

그림 γ．끄 그툽은 하LO］
상의요소 안어7서 함께A渗돨 수 았는
관련된요소들의 라스트를 정의한다．

回

===== PAGE 94 =====
93 =====
;：〕

coije.scil

口」

Defining Complex Type
<xsd:element name="animol'>
<xsd:complexlype>
<xsd:sequence>
<xsd:element ref="name"/>
<xsd:group ref="physicaL-traits"!>
<xsd:element name="subspecies"
type="subspeciesType"/>
</xsd:sequence>
</xsd:complexlype>
</xsd:elemenf>

하나의 그룹을 만들었다면 이것을 다른 그룹에서
설명하거나 복잡한 타입 정의에서 설명할 수 있다．
하나의 그틥올 설명하기：
1. 그룹에서 요소들이 등장할스키마의 부분에
<xsd:group을 입력한다．
2, 그리고나서ref=1 lab이II을입력한다. label
자리에는 앞 페이지의 2번에서 만들어 놓은
그룹을 확인하는데 사용하는 단어를 넣는다．

<xsd:complexlype>
<xsd:group ref="physical-traits"!>
<xsd:attribute name="birthdate"
type="xsd:date"!>
<xsd:attribute name="nickname'
type="xsd:string"/>
</xsd:complexlype>

3. /＞을입력하여 설명을마친다．

·／ nP
■ 복잡한타입 정의 (P94 참조）
, 시퀀스 (p96
참조）
, 선택권들의 세트（p97참조）
, 또는다른
이름의 그룹들 (p98 참조）안에서 그룹을 설명할
수 있다．

element>

그림 Zl2animal과individual요소들은 physical_
traits 그룹 (p98의그림 7．
끄에저 정의된）안에저목록화돤
요소를포함해아한다. 그들은또한부가적, 걔별요소나족정을
가지고 있다．
맬〕de.m】
1· 醬蘿흩 撻亶 층i學黨冬咬멥

<animal><name language="English">Tiger
<!name><weight>500
pounds<!weight><Iength>3 yards from nose to
tail<!length>. .<subspecies>...<!animal>
<individual birthdate="1999-06-10"
nickname="Zoe"><weight>268
pounds</weight>dengih>2.5
yards</Iength>...<!individual>
그림 7.13 같은 요조들은 저로 다른 포함하는요소 안에서 다른 방식
으로사용될수았다．

렝제의소스 코드는 www.cookwood.corn에 았즙L/Z十

99

”
。
*
＇
。 ＝＾言口＝ 口
ㅋ 昱。 ｀흩졉

<xsd:element name="individual">

</xsd:

명명된 그룹 설명하기

===== PAGE 95 =====
94 =====
Chapter 7

미리 정의된 요소 설명하기

珊·－

포괄적으로 설명된 단순하거나 복잡한 타입의 요소
들 (xsd: schema 요소 바로 안의 요소）
은 XML
문서 내에서 나타나기 위해서는 명명되거나 설명
되어야한다．

<xsd:complexlype name="animallype">
<xsd:sequence>
<xsd:element ref="name∥ minOccurs="2"/>
<xsd:element name="thre이y`
type="threatslype"/>
</xsd:complexlype>

포괄적으로 설명된 요소 설명하기：

2. ref="Iab이" 을입력한다. 川e1자리에는포괄
적으로 선언된 요소의 이름이 들어간다．
3. 필요에 따라 이 시점에서 그 요소가 몇 번나타
낼 수 있는가를 정의한다．
4. 乃를입력하여 요소설명을마친다．

'/ nPS
■ 시권스, 선택권들의 세트, 정리되지 않은그룹
그리고 명명된 그룹 정의 안에서만 요소 선언을
설명할 수 있다．
■ 필요한만큼의 위치에서 요소를 포괄적으로
설명할 수 있다. 각각의 설명은minOccurs와
maxOccurs의 분명한 값을 설명할 수 있다．
■ 지엽적으로선언된요소들은그들이 나타나는
성분 정의에서 자동적으로 설명된다. 다른 곳에
서는 설명할 수 없다．
■ 지엽적이거나포괄적인 선언에 대해 더 많은 정
보를 원한다면 p71에 나와 있는 지엽적 선언과
포괄적 선언을 참조하자．

100

<xsd:complexType name="subspeciesType"/>
<xsd:sequence>
<xsd:element ref="name" minOccurs=' 1"I>
<xsd:element name="region"
type="xsd:string"/>
</xsd:complexType>
. 그리고
,1림 Z14 name 요소는 포괄척으로 선언된다（첫번째 줄）
복찹한 타입 정의 안에저 설명될 수 있다．

i」

L0de.∥nH

<animal>
<name language="English">Tiger</name>
<name language="Latin">Ponthera tigrus</narne>
<threats><tbreat>poachers</threat>
<subspecies>
<name Ianguage=「English '>Amur</name>
</subspecies>
</animal>

召
● 言m= =
=＝●ㅌ·＝경＝ 뎡。 ＞
＝
●
，
●
*
●
“

1. 그요소가나타나야하는시퀀스（p95참조）
선택권들의 세트 (p96 참조）정리되지 않은 그룹
(p97참조）또는 명명된 그룹 정의 (p98 참조7
안에서 <xsd:이ement을 입력한다．

[0de.H$d r

<xsd:element name="name" type="nameType"/>

그람 z巧두name 요소들은 복잡한 타입 정의 (- 여又］차는 않았
대에저 겋의되어진 규칙을 반드시 따라야 한다. 부가척으로 그들
은 711별의minOccurs와 maxOccurs 족성값을요구한다. 이
경우 그림 714의스9/마에 따르면 name은animal요소에서
적어도 두 번은 나와꺄 한다. 21러나subspecies요소 안에포함
되었을 때는 한 번만 나와도 된다．

===== PAGE 96 =====
95 =====
Defining Complex Type
돋11a手
code.ssd
<xsd:element name="threat" type="xsd:string"
minOccurs="2" maxOccurs="5"/>

回

주어진 요소 시퀀스 선택권들의 세트나 정리되지
않은 그룹 또는 명명된 그룹의 등장 횟수를 조절할
수 있다．

<xsd:element name="population"
type="xsd:integer"/>
.2랖 7.拓minOccurs와maxOccurs 족성들은요소의둥장
흣）
수를 조철하711 한다．

요소나 그룹의 촤소 툼장 횟수 지정：
요소나그룹의 시작 태그 안에서 minOccurs=1'n'
을 입력한다. 여기서 끄은문서가 유효한 것이 되기
위해서 요소나 그룹이 등장해야 하는 최소한의 갯수
를 의미한다．

c deJmd
<threat>poachers</threat>
<threob.habitat destructionc/threat>
<threat>trade in tiger bones for traditional Chinese
medicine (TCM)</threat>

요소나 그룹의 최다 툼장 횟수 지정：

<population>28</population>

1衲

<xsd:element name="sister name"
type"xsd:string"/>
<xsd:element name="brother name"
type"xsd:string"/>
</xsd:야voice>
.2림 7.18minOccurs와maxOccurs 족성들은 사퀀스나 선택
권젱트의 정렬돠아 았자 않은 그룹 또는 명명된 그룹에 적용할수
있다. 아 예4에서는 이선택그툽의어딴 줏; (0을포함한）
가
司용된다. 아것꽈의마는sister name과brother--name
요소의등장횟주가어딴줏자가되어도무방하다는것아다. 아깃
은 DTD에저 하나의 선택권에 하나의 별표 (*)틀 첨가하는 깃과
동등한 것이다 (p96참조그．

요소나 그룹의 시작 태그안에서 maxㅇCcurs="n"
을 입력한다. 여기서 끄은 문서가 유효한 것이 되기
위해서 요소나 그룹이 등장해야 하는 최대한의 갯수
를 의미한다

V Tips
■minOccurs 속성은음수가 아닌 정수여야
한다 (0, 1, 2, 3 또는 그 이상）
.
■maxOccurs 속성은음수가 아닌 어떤 정수가
nded의 의미는 요소가 나오
될 수 있다. Unb이』
는 횟수가 제한되어 있지 않다는 의미다．
■ininOccurs와xnaxOccurs의 디폴트 값은 모두
1이다．
■ minOccurs와ㅍtaxOccurs 속성은포괄선언된
요소들과함께 사용할수 없다 (xsd: schema
요소 바로 밑에 선언되어 있는 것들）
. 그것들은
지엽적으로 선언된 요소와 사용할 수 있으며
포괄적인 요소들의 설명과 함께 사용하는 것도
가능하다．
■ 이러한속정들은xsd:sequence, xsd:
choice, xsd:ail 둥에서 사용할수 있으며
명명된 그룹의 설명에서 사용 가능하다．

예4의소스 코드는 www.cookwornjcorn에 았습나다．

101

＾
。
＝
4
， 으＝ =
. ＇
。 毛3。 ＝
<

.2림 7.17 적어도 2자 아상 촤대차 5개의threat 아 있어야 하기
때문에 아 저γ 걔의요소들은유효한것들이다. minOccurs와
maxOccurs 둘 다 섕략되었을 때 丘）opu1ation 요소 안에서）
두 값손 다폴트 값인 i을가자고 밌71/ 된다. 따라서 그 요소는XAU
문서에저 정확하 한 번만 등장해야 한다．

[J
導e.de．
∥＄d<xsd:choice minOccurs="0"
maxOccurs="unbounded">

둥장 횟수의 조절

===== PAGE 97 =====
96 =====
Chapter 7

텍스트만을 포함하는 요소의 정의

言．
一毫：
code.Hsd:
「－
<xsd:complexType name="popType">

속정들을 포함하는 주어진단순한 타입 - 컨텐츠가
특별한 종류의 텍스트만으로 제한되지만 - 을 텍스
트만을 포함하는 복잡한 타입으로 끌어낼 수 있다．

·뾔

<xsd:simpleContent>
<xsd:extension base="xsd:integer">
<xsd:attribute name="year" type= 'xsd:year"/>
</xsd:extension>

텍스트만을 포함한 복잡한 타입 정의하기：

</xsd:simpleContent>

2. 그리고name="hbd＂을입력한다. label에서
는 복잡한 타입을 확인하는 내용을 넣는다（이
복잡한 타입 정의를 하나 이상의 요소의 선언
안에서 사용할 수도 있으므로 이것은 요소의
이름이 될 수는 없다）
.

그림 7.19 단순한 컨텐츠 (simpleContent) 요소는 아 복잡한
타입정의．
로 정의된요소가 어느 한종루의 텍스트 r단준한 타입에
7］
초한／喝 포함할 것아라는 것을 정해준다（다른요소들은 포함
하차 못한다）
. 그들은 또한 속정도 가칠 수 았다．

3. ＞을 입력하여 시작태그를마친다.

<xsd:element name="population"
type="popType"/>

6. base="foundation"＞을입력한다. foundation 자리에는 새 복잡한 타입의 기초가 되는
간단한 타입의 정의가 들어가게 된다．
7. 5번에서 xsd:restriction을선택한다면
복잡한 타입 정의를 한정하는 부가적인 제한점
을 선언한다．
(p83- 90 참조）
8. 속성들을선언하거나（p108참조）또는이 타입
의 요소 안에 나타나야 하는 속성 그룹을 선언
한다．
을
9. 5번에상응하기 위해＜/xsd:reshicii이1》
쓰거나＜/xsd:extension＞을 입력한다．
10. <xsd:sim이eC이，
tent＞를 입력한다．
11. 마지막으로＜/xsd:complexlype＞을입력하여
선언을마친다．

102

그림 Z20 항상복잡한 타입정의틀사용하는꾜조를 선인해아 한다．
code.uml－口2
"1999

">

445<

/popuIation>

…

year=

5. 부가적인제한점들을가지고기초적인단순한
타입을 제한하고자 한다면 <xsd:reshiction이
라고 입력한다. 또는 간단한 타입을 확장하고
싶다면 <xsd:extension을 입력한다．

맨

4. <xsd:simpleContent＞을입력한다.

c de.ㅐ d

-<population

*K곁＝ ＝。＝뮬* ＝。닐。 *m섶● ㅌ●＝경＝ ，●。

1. <xsd:comHexType을입력한다．

</xsd:complexlype>

그괌 7.21아population요소는 그림 7.19에 나오는 복잡한
타입 정의와 함계 우효하다. 2/f냐하면 아것은 하나의 정수 (2리고
하나의year요소？를 가자.2 있기 때문아다．
돝1i…

code.HmI 4두蜜∼＝=-－→－＝톺箋鉀i蕣

<population year=" 1999">Less than
500</population>
그림 Z22 아 population 요소는 유효하지 않다. 왜나하면
복잡한 타입의가초가 되는 단준한 타입에서 정의된 것같아 500 다
작은 수는 정수가 아나刀 때문이다．

===== PAGE 98 =====
97 =====
Defining Comp'ex Type
1근듀云區甕
f` e` ，入굿긋．
＝髥 code.Hsd →斗눗｀

j

<xsd:compiexlype name="sourceType'>
<xsd:complexContent>
<xsd:extension base="xsd:anyType"/>

속성은 포함할 수 있지만 시작 태그와 마침 태그
사이에 컨텐츠가 없는 요소들을 빈 (EMPTY) 요소로
간주한다．

<xsd:cittribute name=' sectionid"
type="xsd:integer"/>
<xsd:attnbute name="newspaperid"
type="xsd:integer!>
</xsd:extension>

빈 요소를 위한 복집한 타입 정의하기：
1. <xsd:complexlype를입력한다．

</xsd:comHexContent>
</xsd:complexlype>
.2림 Z23 복함컨텐츠 t omp1exContent7 꾜소는 당신아 족성
을 선언하는 것아 필요할 때사용된다. 그러나포함된요소는 시용
할수 없다．
:：丁동三듣＝；므

그랖 7.24 요소가 나타나는 곳에서요소를 선언해야한다．

三＞1견，

c1》de.HnH

2, 그리고name="Iabd"＞을입력한다. label
자리에는 복잡한 타입을 확인하는 내용을 넣는
다（하나 이상의 선언에서 이 복잡한 타입 정의
를 사용할수 있으므로 이것은 요소의 이름이 될
수 없다）
.
3. <xsd:complexConteni>를입력한다．

큔手年횰편r二＝ c0de."d

<xsd:element name="source"
type="sourceType"/>

〔…＝

빈 요소 정의하기

騙

<source sectionid="lOl" newspaperid="21"/>
그람 Z25 한 번 선언된후에는XML 문저에저소스 요소를 사용할
수 았다．

4. <xsd:extension base=h1xsd:anytypeTh/>을
입력한다（하이픈없이）
. 이것은복잡한타입을
기초로 하는 타입은 없다는 것을 지시하기 위해
서이다（그리고 컨텐츠를 갖고 있지 않기 때문에
좋다）
.
5. 속성을선언한다. 만약에 있으면 이 타입의 요소
안에 나타날 것이다 (Pz08 참조）
.
6. c/xsd:complexContent＞를입력하라．
7. 그리고＜/xsd:complexlype＞을입력하여
선언을마친다．

1nP
■ 복잡한타입을정의하는데보다자세한정보를
알기 위해서는 p94에 나오는 요소만을포함하는
요소의 정의와p107에 나오는 무명의복잡한
타입을 ㅈ／난 요소를 참조하면 된다．

예저）
의소스 코드는 wV
『v.cookwood.com0J/ 있즙나다．

103

===== PAGE 99 =====
98 =====
Chapter 7

혼합된 컨텐츠를 가진 요소 정의하기

<xsd:sequence>
<xsd:element name="nome"
type="nameType">
</xsd:sequence>
<xsd:attribute rlame="leng小“
type="xsd:string'/>
</xsd:complexlype>

혼합된 컨텐츠로 복잡한 타입들 만들기：

3. mixed="true"를입력한다. 이것의 의도는그
요소가 요소들, 속정들 그리고 텍스트까지 포함
할 수 있다는 것을 알려준다．
4. ＞을입력하여 시작태그를마친다．
5. 시퀀스선택권（p95참조）
, 또는정리되지 않은
그룹（p96 참조）또는 명명되어진 그룹 (p97
참조）
을 설명하는 것 - 이것은 앞의 세 개를 포
함할 수 있다 - 들을 선언한다. 이 의도는 어떤
요소가 복잡한 타입을 포함할 수 있는지를 알리
기 위해서이다.
6. 그리고 이 타입의 요소 안에 나타나는 속성들，
속정 그룹들을 선언한다.
7. </xsd:comHexlype＞을입력하여 선언을
마진다．

VTip
■ 혼합된 컨텐츠 요소들은 사적이고 텍스트를
기초로 한 정보에 이상적이다．

104

.2림 Z26paragraph 정의는 하나의꾜소와 하나의족정을포함
하고mixed=' true" 속정 덕분에느슨한 턱）스트를포함할수도
았다．
撞町래

code.Nsd蓑뇨순걋
稱노

*
二
● *＝。닐경灌呈솥m뇰＝ ＝·ㅌ스山 量＝ 뎡。

2. 그리고name=시먀）
d"을입력한다. label자리
에는 복잡한 타입을 정의하는 내용을 넣는다
（하나 이상의 선언에서 복잡한 타입 선언을 이용
할수 있기 때문에 이것은 요소의 이름이 될 수
없다）
.

',

&'>

mixed=

순수한 데이터베이스 위주의 컨텐츠는 대부분 다른
요소들과 텍스트를 포함하는 요소들을 포함하지 못
하는 반면에 텍스트 중심의 문서는 요소나 텍스트를
포함하는 경우가 많다. 다른 요소나 텍스트를 포함하
는 요소를 정의할 복잡한 타입의 작성시에는 반드시
컨텐츠의 혼합이 선언되어야 한다．

1. <xsd:complexlype을입력한다．

｀됴互됴즈＝5＝亡口1
rode.esd妾立＝ㅌ二三로－

→：

<xsd;complexType name= 'paragroph"

<xsd:e)ement name='description"
type="paragroph"I>
그림 7.27요소가 나타나는 곳q서요소를 선언해야 한다．
`

핍 = ＝길 == ＝느 즌＝三

J亡．

code.HnH ＝丁 一 `

!

-

∼三

＝色

첵＝ ,

<description length="short">The <name
Ianguage=" English">tiger</name>
(ponthera tigris), largest of all cats, is one of the
biggest and most fearsome predators in the
wor)d.</description>
그람 z羽description 요소는느슨한（붉은색）텍즈트와요소
들（붉꼰객과 bold 제；쁠포함한다．

===== PAGE 100 =====
99 =====
Defining Complex Type
틀■十，一

`` m ,\`', ∼ 'r>

ode.Hsd 毫－

∼＝

<xsd:complexType name="characteristicsType">
<xsd:sequence>
<xsd:element name="weight"
type="xsd:string"/>
<xsd:element name="length"
type="xsd:string"/>
<xsd:attribute name="Kind"
type="xsd:strung"/>
</xsd:sequence>
</xsd:complexlype>

童m椿흄＝

이미 존재하고 있는 복잡한 타입을 가지고 복잡한
타입을만들수있다. 새로운복잡한타입은기존의
타입에서부터 모든 정보를 가져와서 특징을 더하거
나 뺀다．
기존의 타입을 기초로 복잡한 타입 만듈기
1. <xsd:compIexType을입력하여새복잡한
타입의 정의를 시작한다．
2. name="label"＞을입력한다. labe／자리에는
만들려는 복잡한 타입을 정의한다．

rede.
ㅐd

<xsd:complexlype name= birthType">
.cxsd:complexContent>
<xsd:extension bcise="choracteristicslype'>
<xsd:sequence>
<xsd:element name="mother"
type="xsd:string"/>
<xsd:element name="birthdate"
type="xsd:date"/>
</xsd:sequence>
</xsd:extension></xsd:complexContent>
</xsd:complexType>

3. <xsd:complexContent＞를입력한다.

그쾀 7.30새로운birthType은 아것이 정의하는요소 안쎄저
반드사 나타나야 하는 부가적인요소만을 목록화하고 았다．

5. base='existing" 을입력한다. Existing자리
에는 복잡한 타입이 세워질 타입의 이름을 입력
한다．

ode.nsd
「李 ________롸
<xsd:element name="birth characteristics"
type="birthlype"/>

6. 》을입력한다．

냑g'
구- 눔＝녹누낳뇩-"- '츤수心구：
郵1》

그람 Z31 당산은 항상복잡한 타입정의를사용하는요소를 선언
해야한다．
c de.eml
<birth characteristics Kind="normal">

듈田瑟＋큐二뿜芸

<weight>2-3 pounds.c/weight>
<Iength>18-24 inches-c/length>
<mother>Danai</mother>
d)irthdate>1999-06-10c/birthdate>
</bir卄1 diaracteristics>

4. 복잡한타입의 새로운특징들이 기존의 타입에
첨가되어야 한다는 사실을 알리기 위해서
<xsd:extension을 입력해야 한다．
또는 복잡한 타입의 새로운 특징들（적어도 몇몇
의 것들은）
이 전의 것들보다 제한적이고 압도한
다는사실을 알리기 위해서 <xsci:resfriction을
입력한다．

7. 부가의 또는제한적인시퀀스나선택권을선언
하거나 새로운 타입의 부분이 될 명명된 그룹을
설명한다．
8. 새로운타입의 부분이 될부가의 속성을선언하
.
거나 설명한다 (p108 참조）
9. 4번에 알맞은 마침 태그를 입력한다．
10. </xsd:complexContent>를 입력한다．
11. 복잡한타입 정의를마치기 위해 </xsd:
complexlype＞을 입력한다．

그쾀 7.32birth_characteristics 요소는characteristicsType 6aeight와length 요소뿐만 아나라 kind
속성도7의특성을포함해야 하i2 새로운 특겅들 4nother와
birthdate) 포함하아 한다．

여］群의소스 코드는 www.cookwood.corn 있습i-/다．

105

四口驪＝ .＾。클릉X뻐뚱● m
。 ＝＾。크브。 X뻐뚱● m

그림 7四characteristicType정의는weight와 length
요소와 kind요소를 필요로 한다．

복잡한 타입을 기초로 한 복잡한 타입

===== PAGE 101 =====
100 =====
다tapter 7

복잡한 타입의 요소 선언하기
복잡한타입을정의하였다면, 이제 이것을요소에
할당하면 그 요소가 XML 문서에서 사용할수 있는
것이 된다．
복잡한 타입의 요소 선언하기：
1. <xsd:이emenㅎ로요소선언을시작한다（그림
7.33).
읖 漱 X 으 ｀ ㅌ。U* 。*＝●ㅌ으山＝ 。m= ：。＝m。

2. 竗pe="Iab이"을입력한다. label자리에는복잡
한 타입을 정의할 때 사용했던（예 p94의 2번）
단어를 넣는다．

口

<xsd:sequence>
<xsd:element name="weight"
type="xsd:string"/>
<xsd:element name="length"
type="xsd:string"/>
<xsd:atfribute name="kind"
type="xsd:string"/>
</xsd:sequence>
</xsd:complexlype>
그림 7.33 여기에서는 전형적인 복잡한 타입정의 (p105에 나온
그림 7. 29와같이）
가 았다．
妾骨

3. /＞를입력하여 요소선언을마친다．

V Tips
■ 요소들은복잡한타입의 정의 (P94 참조）
나，
시퀀스 (p95참조）
나, 선택권세트 (p96 참조）
나，
이나 또는 명명된
정렬되지 않은 그룹 (p97참조）
그룹 정의 (p98 참조）
에서 포괄적으로（스키마의
첫부분 xsd: schema 요소의 바로 밑에）
나 또는
지엽적으로 선언할 수 있다．
■ 지엽적으로요소를선언한다면minOccurs와
rnaxOccurs의 속성과 함께 요소의 등장 횟수를
조절할수 있다. 더 자세한 사항은 p101의 등장
횟수의조절을 참조하자．

길 cede.nsd

<xsd:complexType name="characteristicsType「>

，읽 codeJ{Sd

<xsd:element name="choracteristics"
type="charocteristicsType"/>
<xsd:complexlype name="animallype"/>
<xsd:sequence>
<xsd:element name="name"type="nameType"
minOccurs="2"/>
<xsd:element ref="characteristics"
minOccurs=" 1"I>

그림 Z34 스7／마 문서의상위 단계에서는 요소를 포괄적으로 선언
할 수 있다. 아 경우요소를 사용하가 위해서 당신의스카마 안에
았는 다른 성분 안의요소를 설명할 필요가 있다．
< ',t,"<'1, - code.nsd ---- -－午m可
<xsd:complexlype name="animalType"/>
<xsd:sequence>
<xsd:element name="name"type="namelype"
minOccurs="2"/>
<x5d:element name="characteristics"
type="characteristicslype"minOccurs="1"I>

그림 Z35또는 다른요소 (- 여잔 것과 같은 복잡한 타입 정의나
또는 명명되어진 그룹）안아서 당신은 그 요소를 자엽적으로 선언
할수 있다. 아 경우요소는자동적으로 설명된다．

106

===== PAGE 102 =====
101 =====
Defining Complex Type
巨j

복잡한 타입을 다시 사용할 필요가 없다면 요소 선언
안에 있는 무명의 복잡한 타입을 만드는 편이 더
빠르다．
익명의 복잡한 타입을 가진 요소 선언하기：
1. <xsd:elemenㅎ를입력한다．

그림 7.36 ㅇ／번에는 우라는 글자 타입을 익명의 타입정의로 다사
정의할수 았다. 여가서 우리는 복잡한 타입 정의를그것 (cha
racteristics)을포함하는요소를 위해저사용할수 있다．
그 요소는 ㅈ／엽적으로 또는포괄적－으로 선언될 수 있다．

rj
〔0de,H針1
<characteristics Kind="physical">

무명의 복잡한 타입들을 지닌 요소

qj

<weight>500 pounds.c/weight>
<length>3 yards from nose to tail</length>
</characteristics>
그림 7.37 여기서는 유효한보가를 보여준다. 아름아 있가나 아릉이
없는 복잡한 타입을사용하거나 폭같아 보일 깃아다．

2. name="label"＞을입력한다. label자리에
선언하고자 하는 요소의 이름이 들어간다．
다시 말해서 XMT 문서에서는 <label〉과 비슷한
모양일 것이다．
3. 다음에＜xsd:complexlype＞으로익명의복잡
한 타입을 시작한다
4. 어떤요소가복잡한타입을포함할수있는지
정하기 위해 시퀀스（β95참조）
, 선택권들 (p96
참조）
, 또는 정리되어있지 않은 그룹 (p97참조）
,
명명된 그룹의 설명 - 이것은 앞의 세 가지를
모두 포함할수도 있다 (p99 참조）- 등을 선언
해야 한다．
5, 그리고 나서 이 타입의 요소 안에 나타나야 하는
속성 (p108 참조）또는 속성 그룹들（β끄i 참조）
을 설명하거나 선언해야 한다．
6. </xsd:complexType＞을입력하여 익명의
복잡한 타입 정의를 마친다．
7. </xsd:element>를입력하여 복잡한타입 요소
의 선언을 마친다．

V Tip
■ 명명된 그룹과무명 그룹의 유일한 차이점은，
전자의 것은 원하는 만큼 다른 요소들로써 또는
부가의 복잡한 타입들의 기초로써 선언하는데
사용될 수 있는 반면, 후자의 경우에는 이것이
발견되어진 요소들을 정의하는데 사용될 수
밖에 없다는 점이다．

中I）
의소스 코드는 www.cookwooci.corn에 있습나다．

107

=e크● ＝．鷺킁軫● ＝닉크흩m＾ ●클찧eX뻐뚱g

量r;：珊
휼cOde,Hs1
<xsd:히ement name='놔aracteristics">
<xsd:com이exType>
<xsd:sequence>
<xsd:element name="weight"
type="xsd:string"/>
<xsd:element name="length"
type="xsd:string"/>
<xsd:attribute name="Kind"
type="xsd:string"/>
</xsd:sequence>
</xsd:complexjype>
</xsd:element>

===== PAGE 103 =====
102 =====
태apter7

속성 선언하기

<xsd:eement name="source">

하나의 속성은 언제나 단순한 타입인 반면에（다른
요소나 속정들을 포함하지 않으므로）이것은 언제나
복잡한타입의 요소에 나타난다. 여기서는 이것을
만드는 방법에 대해 살펴보기로 하자．

<xsd:complexlype>
<xsd:complexContent>

속성 선언하기：

<xsd:attribute name="newspaperid"
type="xsd:string"/>

1. 복잡한타입의 정의에서 <xsd:attribute를
입력한다．
2. name="I아）
이H을입력한다. Lsbei자리에는
XMT 문서에서 속정을 설정하는데 사용될 이름
을쓰면된다．

●
m
。
＝
●
。
섭슨， 驪m= ＝

3. type="simHe"을 입력한다. simple자리에는
속성이 속해 있는 단순한 타입이 들어가게 된다．
단순한 타입에 대한 더 자세한사항은 p76에 나
오는 단준한 타입을 가잔 요소 선언을 참조한다．
또는ref=" hb이＂을 입력한다. label자리에는
이미 포괄적으로 선언되어진 속성 정의를 검증
한다．
4. ＞을 입력하여 시작태그를마친다．
5. 원하는만큼의 제한점을첨가한다. 자세한사항
은 p83-90을 참조하다．
6. </xsd:athlbute＞를입력한다．

'/ nP$
■ 만일 제한점이 없다면 4-6번 과정을 생략하는
대신 /＞을 입력한다.
■ 단지 속정들을위한부가적인 단순한타입들이
있다. 이것은http://www. W3.org/TR/
xmlschema-2 에 나와 있다．
■ 무명의 단순한타입을가진속성을정의할수
있다.
■ 속정은그것이 속한복잡한타입의 가장마지막
부분에서 선언되어야 한다. 다시 말해 그 위치는
선언된 복잡한 타입 안에 있는 모든 성분의 다음
에 오게 된다．

108

<xsd:extension base="xsd:anylype">
<xsd:attribute nome="sectionid"
type="xsd:string"/>

</xsd:extension>
</xsd:complexContent>
</xsd:complexlype>
</xsd:element>
그림 7.38 하나의속정 선언은 여느 단준한 타입요소 선언과 같이
섕겼다．

. deJ1n11

ㄴ 젼 짠 ∼랖＝
ㅌ꼴

＝콰

<source sectionid="lOl" newspaperid="21"I>
그람 Z39 수y들은 언제나포함하고 았는요소의 ㅈ／작 태그 인에
나타난다．

===== PAGE 104 =====
103 =====
Defining Complex Type
團1
t de.Hsd
<xsd:element name="source">

·

<xsd:complexlype>
<xsd:complexContent>
<xsd:extension base="xsd:anylype">
<xsd:attribute name="sectionid"
sype="xsd:string" use="required"/>
<xsd:attribute name="newspaperid"
type="xsd:string'/>

속성 요구하기
자신이 정한 속성의 정의법과 다르자않다면 속성은
언제나 선택적이다. 다시 말하면 속성은 문제를 발생
시키지 않고 XML 문서에서 나타나거나 없어질 수
있다는 것이다．
그러나문서가 유효화 되는지 여부를 판단하는 시점
에서 속성의 등장 여부를 밝힐 수 있다．

</xsd:

</xsd:extension>
</xsd:complexContent>

툼징할 속성의 요구：

</xsd:complexType>

1. 속성을정의할때 use＝를입력한다．

element>

그람 z40 하나의 족정에 甲한 다폴트 값은 선택사항하刀 때문에
특별하 이것은 의무적아라는 깃을요구해야 한다．

瓠．
<source sectonid="101 'I>
code.Hml , "- 注－→욕斗슥｀슥汽∼뇩am蓍

<source sectionid="lOl ' newspaperid="21"I>
그림 7.41아런 source 요소들은 유효한 것들아다. 왜나하면 단치
sectionid가요구되는 것아刀 때문아다. 만일 하나의요소가
특별ㅎ／요구되는 것이아나라면 ㅇ］것은 선택사항으로 간주된다．

2. 다음에 "required"로문서의유효화를위해그
속성이 반드시 등장해야 함을 밝혀준다．
3. 필요에 따라value="must＂를첨가한다. must
자리에는 속정에 가능한 가치값만이 올 수 있다．
둥장하지 않이야 할 속성 요구하기：
속성을 정의할 때 use="pr햐1ibited" 를 씀으로써
이 속성이 등장하지 않아야만 문서가 유효하다는 것
을 표시한다．

v' Tip
U use="야州ond" 또한속정 정의에 첨가시킬수
있다. 그러나 이것은 디폴트 값이므로 번거롭게
될 것이다．

예群의소스 코드슨 www cookwood. corn에 았습나다．

109

===== PAGE 105 =====
104 =====
（十apter7
＝츠프 code.HSd 료－

속성의 컨텐츠 미리 정의하기

속성의 컨텐츠 지정하기：

<xsd:attribute nome="newspaperid"
type="xsd:string"/>
kfL 문서에 나타나는 한
.2림 Z42sectionid 족성은 아것아x〕
（또는 이것이 비아 있을 경꾸？ 반드사 101값을포함하고 았어야
한다. 그러나속성은꼬두 섕략할수 있다 (note:pi09의그림
7. 40의복잡한 타입정의에서 발w
寸目三르三＝r＝淫＝--F근＝＝三든－
：斗
；code 140기

2. 'v이ue=content＂를입력한다. content자리에
는 그 문서가 유효화되기 위해 속성의 값이 무엇
이어야 하는지 정한다 0（ㅅ／[L 문서 안에 그 속성
.
이 나타날 경우）
속성의 처옴값 설정하기：
1. 속성 태그에서 use="defauIt"를입력한다．
2. vdue="content"를입력한다. content자리에
는 그 속성이 XML 문서에서 생략될 경우 속성
값을 어떻게 정해야 하는지를 결정하는 내용이
들어간다．

'/ nP`
■ 속성이 실제로 xM. 안에서 나타난다면 그 고정
값은 컨텐츠를 설정하게 된다. 만일 생략된다면
어떠한 컨텐츠도 설정되지 않는다．
■ 디폴트속정이 설정되었지만그속정이 XML에
서 생략되었다면 속성값은 자동적으로 디폴트값
으로 설정된다．
■ 디폴트 속성이 설정되고 그 속성이 XML에 등장
하면 이것의 컨텐츠는 제한적이지 않다（고정
속성값에 의해）
.

110

<source sectionid=" 101" newspaperid="21"I>
.2림 7.好 .2림 742의스카마 더／아e/와 바교해볼 때 아 source
요소는유효하다. 만일 sectionid 속성이 없을 경우에는 아것은
유효한것아다．

仁1}

；三＝===1크
code.em 3큐F驪再言잿之멸＝
sectionid="456

-<source

*
=
e
* ＝。U견0섭슨鷺占＝ 。m灌＝ ＝●경t

1. 속성 태그안에서는use=Ifixed∥를입력한다．

" newspaperid= '21

"/

속성의 컨텐츠를 미리 정하는 스키마를 사용하는데
에는두 가지 방법이 있다. 속성의 컨텐츠를 지정하
거나（속성이 XML 안에서 나타날 때）또는 이것의
등장 여부에 상관없이 그 속성의 처음 값을 설정한
다. 전자의 것은 고정값이라고 하고 후자의 것은
디폴트값이라고한다．

<xsd:attribute name="sedionid"type="xsd:strrig「
use="fixed" value="lOl∥/>

>

그림 7.44그림 7.42의주어진 선언에 의하면 아것은유효한
source -［소가 아나다．
m－
릎三code.Hsd
<xsd:ottribute name="sectionid" type="xsd:string"
use="Iixed"value="101"!>

·可

<xsd:attribute name="newspaperid" type=
"xsd:string" use="default" volue="21"/>
그랖 7.45 만일 우리가newspaperid 속쟝을 다폴트 값을 가자
고 정의한다면그 값은newspaperid 족정아XML 문저叩 등장
하는 여부에상관없아 차음 값으로 설정되어진다 御09의그림
7.40 복잡한 타입정의의 인용걋．
c de*11m'

<source sectionid=" 101" newspaperid="21"I>
톨田

ㅋm－틘mK乙겸乙 code.eml

<source sectionid="101" newspaperid="25"/>
.2림 7.46아두걔의 source 요소들은유효하다. 다폴트속성
은 초7／값으로만 설정되고 다른 값들또한가능하다．

===== PAGE 106 =====
105 =====
Defining Complex Type
쭐匠

에de.11$d

<xsd:aitributeGroup name="imageAtts">
<xsd:attribute name="filename" type="xsd:urireference"!>
<xsd:attribute name="x" type="xsd:inte9er"!>
<xsd:attribute name="y" ype="xsd:integer"/>
</xsd:attributeGroup>
.2림 7.47 아틈으로 족정그룹을 정의함으로써 이ㄹ／한 속성들을
복주의타입 정의叩 다사 사우하는 것아 용아하겨）되었다．

폴

속성 그룹 정의하기
하나 이상의 요소에서 속성의 같은 세트를 사용할 경
우 속정 그룹을 정의해 주거나 요소에 상응하는 복잡
한 타입에서 그룹을 설명하는 것이 더 효과적이다．
속성 그岳올 정의하기：
1. <xsd:atfributeGroupnome="IabeI">*
입력한다. labe／자리에는속성 그룹을증명하는
것을 넣는다．
2. 그룹에속하는각각의속성을선언하거나설영
.
한다 (P/08 참조）

3. </xsd:attributeGr이샤）
＞을입력하여마친다.
V Tips
■ 하나의 속성 그룹은 스키마의 상단에서 (xsd:
schema 요소바로 밑에）포괄적으로선언되어
야 한다．
■ 속성 그룹을 선언하면 p112에 나와있는 것과
같이 설명을 해야 한다．
■ 스키마의 상단에서 선언된 포괄적으로 설명된
속정들만 설명한다. 자세한사항은 p71에 나와
있는 차엽적 산언과포괄척 선언을 참조한다．
■ 속성 그룹에서 속성을 지엽적으로 선언할 수
있다. 이러한속성들은특정 속성 그룹들에서만
가능한 것이지만 그것으로도 충분하다.
■ 하나의 속정 그룹은 다른 속성 그룹들의 설명을
포함할 수 있다.

中의소스 코드는 wwwcookwoocL c0m에 있습나다．

1】
1

===== PAGE 107 =====
106 =====
Chapter7

속정 그룹을 정의해 주면 이러한 속성들이 어디서
필요하든지 설명을 할 수 있다．
히니의 속성 그룹 설명하기；
1. 복잡한타입 정의 안에 포함되어야할속정을
선언한후＜xsd:attributeGroup을 입력한다．
2. 다음ref="Iabel"/＞을입력한다. labe／자리에
는 pill에 1번에서 사용한증명 이름을 넣는다．
표＝ 。，。0섭욘느＝ <m= ==0느● *
●
“

·'Tips
■ 속성 그룹은 DTD (p60 참：조）
에서의 인자 개체
와유사하다. 그러나물론 이것들은속성의 컬렉
션을 나타내는데는 한계가 있다．
■ 속성과속정 그룹은 언제나한 성분의 마지막에
요소들이 선언된 후에 선언되어야 한다．

蚤1醫，
,,｀스 -` ，「

·

code.xsd

口클

<xsd:element name="picture">
<xsd:complexlype>
<xsd:complexContent>
<xsd:extension base="xsd:anylype">
<xsd:atfributeGroup ref="imageAtts"/>
</xsd:extension>
</xsd:complexContent>
</xsd:complexlype>
</xsd:

속성 그룹 설명하기

element>

<xsd:element name="video">
<xsd:complexType>
<xsd:com이exContent>
<xsd:extension base="xsd:anyType">
<xsd:element name="description"
type="xsd:string"I>
<xsd:element name="running_time"
type="xsd:timeDuration"/>
<xsd:ottributeGroup ref="imageAtts"/>
<xsd:atfribute name="format"
type="xsd:string"I>
</xsd:extension>
</xsd:comHexContent>
</xsd:complexlype>
</xsd:element>
그림7.48 ref=' imageAtts " 를쓰는깃은세개의걔별속성을
재정의하는깃보다 훨씬 빠르고 일관척아다. Video 속성아부가
적인포맷 족성을 족정그를 후에 선언사킨다는 것에주꼭하자．

目1-

cede.nnd

驪

<piciure filename="tiger.jpg" x="200" y="197"/>
<video filename="tiger.ram" x="100' y="l 00"
format="reolplayer">
<description>A tiger moves gracefully through the
dappled light of the Forest.</description>
<running_time>PT3M43S.c/running_time>
</video>
그림 7.49그림 (picture) 요소와 비디오 (video) 꾜소들모두
filename x와 y 속정들을 공우하고 았다. 그라나그들은 한 빈
만 정의하면 된다．

112

===== PAGE 108 =====
107 =====
USING NAMESPACES IN XML
XML의 이름공간 사용하기

돝컫 code.usd
［亘
<xsd:schema xmlns:xsd="http://ww.w3.org/
2OOO/1O/XMLSchema">

</xsd:element>

그림 8;' 소걸적인RiversML에 대한 아스카마 안에저각각의
끄소는 문저의상위 단계에저 포괄척으로 산언된다. 그라고 나서
각각의 요소는 그들하 나타날요소꽈 복잡한 타압 정의 안에사
설명된다．

<xsd:schema xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema">
<xsd:element name="name" type="xsd:string"/>
<xsd:element name="source" type="xsd:string"I>
<xsd:element name="animal">
<xsd:complexType>
<xsd:sequence>
<xsd:element ref="name"!>
<xsd:element ref="source",/>
</xsd:element>

그림a2Endangerel Species schema의 번역 안에저모든요소
들을포콸척끄로 선언했다. 만일 아 스카ㅁ／와 함께 만들어진 문사
와그림 8.1에저 볼 수 았는 스카마와 함꼐 만들어진 문저룰
혼합한다면 name과 source 꾜소 안에 있는 데아E7는 저로
초화될 것이다．

이 문제의 해결 방법은 둘의 요소를 구별할 수 있는
수퍼라벨 (superlabel)을 만드는 것이다. 예를들면
나는 Liz라는 단어를 나의 모든 요소 이름에 붙일 수
있다（콜론과함께）
. 그러면나의Liz: source는
당신의 your:source와혼동되지 않을 것이다．
물론 Liz는 특별하게 고유한 것은 아니다. 수퍼라벨
의 이름은 보통 독점 도메인을 기초로 한 URL의
형태를 취한다. 그 이유는 이것이 고유한 것이고（아
무도 당신의 도메인 이름을 사용할 수 없기 때문이
다）또한 지속적인 것이기 때문이다（도메인은 좀처
럼 바뀌는 법이 없다）
.
수퍼라벨은 이름공간 (narnespace) 이름이라고
불려진다. 이름공간자체는 이름공간 이름에 의해
확인된 연관된 요소 이름의 컬렉션이다．
（지엽적으로 선언된 요소들은 그 문맥에 의해 고유한
것으로 만들어진다 -p71참조. 그들은 대부분 이름
공간을 가지고 승인을받을 필요는 없다）
.

113

．已＝ .＝。ㅋm씀只샀 ＝님글尸

<xsd:element name="name" type="xsd:string"/>
<xsd:eement name="source" type="xsd:string"I>
<xsd:element name=" rivera>
<xsd:complexlype>
<xsd:sequence>
<xsd:element ref="name"!>
<xsd:element ref="source"/>

지난 두 장에서 우리는 XML 문서를 구성하고 있는
스키마 내부에서 요소들의 세트와속정들을 어떻게
정의하는지에 대해 배웠다. 만약 다른 사람이 만든
문서를자신의 것과합치려고하는데, 다른사람은
스키마 안에서 당신이 포괄적으로 선언한 이름과
같은이름을사용했다고생각하자. 예를들면같은
이름이지만 하나의 문서가소스를 세계 야생 동물
펀드 웹사이트에서 사용된 데이터 소스임을 지시하
고 있고, 다른 하나의 소스는 강의 상류를 명시하고
있는데 그 둘을 합친다면 소스 요소 데이터는 왜곡될
것이고 의미없는 것이 된다．

===== PAGE 109 =====
108 =====
Chapter 8

이묩공간 이름 디자인하기
이름공간의 모든 포인트는 유사하게 이름 붙여진
요소들을 구별하는 것이기 때문에 이름공간은 반드
시 고유하고 지속적인 이름을 가져야 한다. XML에
서 이름공간 이름은 URL 형식이다．

시작프로토콜
도메인 이름

http://www.domain.com/ns/rivers/l .0
이름공간에 대한 짧은 설명
선택 사양인 버전

이름공간 .好 디자얀하기：
1. 도메인이름으로시작한다．
2. 이름공간을위한고유한이름을만들어 설명의
정보를 첨가한다 (IJRL에서의 path와같이）
.

I,, nPS

藍

■ 모호하게 들릴 수도 있지만 사실 이름공간을만
드는유일하고공식적인 설명은, 이것이 URL의
형태를 가지며 고우한것이어야 하고 또 지족적
이어야한다（실제적으로 영원해야한다）
. 여러
개의 이름공간을만들 때에는 모순되지 않는 것
을 권한다．
■ 원한다면이름공간에다버전정보를첨가할수
있다．

빼難髓難解

■ 이름공간의 기초가 되는 것으로 자신의 도메인
을 사용하는 것으로 그것이 고유한 이름임을
확신할수 있다. 누구도 당신의 도메인 이름을
사용할 수 없다．
■ 이름공간 이름에 다른 사람의 도메인 이름을
사용하지 않는다．
■URL이 이름공간에 사용되는 이유는 고유함때
문이고 다른 이유는 없다. 그 {JRL이 DTD나
스키마를 지시할 수 있지만 꼭 그래야만 하는
것은 아니다. W3C의 의도 역시 아니다. URL을
선택할 때는 변하지 않는 것이나 특정 파일을
설명하지 않는 것을 사용하기를 추천한다．

1 14

선택 이름공간
디렉토리 정보

그림 8.3 이름공간은 반드사 VRL의 형태표준http 프로토콜로 사작
하고 자신의도咐인 이룸 , 다렉토리 이틈 안에저 선택사양인 아틈
공간표사, 이름공간에 까한짧은 설명, 그리고 선뱍사양인 버전 두아
따라오는 형태가되어야 한다. URL은 실제 파일을자적함꽐요는
없다．

===== PAGE 110 =====
109 =====
Using Namespaces in XML
름．

CodeJ1'n·

숟슬三컫귿솥＝娑毫길 三＝긴른르三르二

<endangered_species>
<animal>

이름공간 이름을 디자인했다면 이것을 모든 문서나
문서의 일부분에서 디폴트값으로 선언할 수 있다．

<name language="English">Giant River
Otter</name>
<source sectionid="122" newspaperid="21"
contentid="630"
xmlns="http://w'ww.cookwood.com/ns/
end_species 1"/>
<picture Iilename="otter.jpg" x="200" y="l 97"/>
.1W 8.4 Source 요소는 017/Al http://www.cookwood.com/
ns/end_speciesl이름공간의부분으로 정의되어 밌다. 다른요소들
의 어느 것도 이름공간과 연결되어있차 않다（아깃은 가끔ii1끄0
namespace라고 불린다).
c.de.川ni

= : ( 논i른二製1

<name language="Latin">pteronura
brasiliensis</name>
＜小reats><卄ireat놔｀abitot destruction</卄1reoh
<threat>hunting</threat>

그림 8.50/ 예제에저는root요소에저 아름공간 선언과 함계문저
에았는.
2 의22든 것은 http://www.cookwood.comlns/
end_speciesi의 ㅇ／륭공간과 연결되어 았다 (p116-117의 다폴트
이름공간을 무사하는 방밥에저 아것을 다룰 것아다）
.

예젱의소스 코드는 www.cookwooct corn에 있습나다

"I 1iPS
■ 위에서 설명한이름공간으로요소를분류하는
것은 이것이 다른 이름공간으로 분류되어 있지
않는 한, 특정 요소뿐 아니라 그 요소에 포함된
모든 요소에 영향을 준다．
■ 따라서 루트 요소에 알맞은 디폴트 이름공간을
선언하면 그 문서에 있는 모든 요소들은 그 이름
공간으로부터 나온 것이라고 간주된다（다른
방향으로 분류되지 않았다면 p116-117을참조）
.
■ 문서 전체（혹은 부분）
를 위해 선언된 이름공간
은디폴트이름공간으로부른다. 이는다른이름
공간이 다시 적용되지 않았다면 모든 문서
（부분）
의 요소에 적용할 수 있기 때문이다．
■P116-117에서 설명한 것처럼 개인적인 요소를
위한 미리 정해진 이름공간을 정하게 되면 디폴
트 이름공간（혹은 이름공간 없음）
을 무시할 수
있다. 자요소들은 영향을 받지 않는다．

1 15

離

山

轟
如
一
碑
照
m

<threat>pollution from fossil fuel
extractionc/threat>

2, 그리고∥U끼．
∥을입력한다. URL은이름공간의
.
이름이다 (P끄4 참조）

一正恬

<threat>mercury poisoning from gold
mining</threat>

1. 이름공간으로분류하고싶은요소의 시작태그
안에서 xmlns＝를 입력한다．

打肇騙＝ ，꾜好騙

<endangered_species
xmlns="http://www.cookwood.com/ns/
end_species1">
<animal>
<name language="English">Giant River
Otter.c/name>

요소나 자요소를 위한 디폴트 이룝공간
선언하기：

黨藩

．■－

디폴트 이릅공간 선언하기

===== PAGE 111 =====
110 =====
Chapter 8

개인 요소들을 위한 이름공간
이름공간으로 문서 안에 있는 특정 개별 요소를
그 요소들의 자 (children) 요소에 영향을 주지 않고
구분하려면 그 이름공간에 특정 닉네임 혹은 접두사
를 선언하여 개별 요소를 구분할 수 있다．
이흽공간 이름을 위한 접두사 中refix) 선언하기
1. 문서의 root요소안에서xmlns:Prefix를쓴다．
접두사는 이 이름공간의 닉네임이 될 것이다．
2, 그리고나서＝'URL＂을쓴다.［爪L자리에는
첩두사가 설명할 이름공간의 이름이 들어간다.
=＝·ㅌ으叫 。。七三겯 ，。*m● V。 튜● ㅌ．=

'/ nPS
■ 접두사들은x, i끄, ／등의 단어로시작할수 없다．
이러한순서로 쓸수도 없고 소문자, 대문자
역시 사용할 수 없다．
■ 접두사를선언했던요소안에포함된요소안에
서나, 포함하고 있는 요소 안에서는 접두사를
사용할 수 있다. 만일 루트 요소 안에서 접두사
를 선언했다면 문서의 어떤 요소와 속정 안에서
루트 요소 자체를 포함해서 그 접두사를 사용할
수 있다. 만일 다른 요소안에서 접두사를 선언
했다면 이것은 그 요소 안에서 혹은 그 요소의
자요소에서만사용할 수 있다．
■ 어떤 요소 안에서 필요한 만큼의 접두사가 붙은
이름공간을 선언할 수 있다.

] 계6

홰그

code,川ni 크

<endangered_species xmlns="http://www.
cookwood.com/ns/ end_species 1"
xmlns:rivers="http://www.cookwood.com/ns/
rivers 1">
<animal>
<name language="English">Giant River
Otter</name>...
<source sectionid="122" newspaperid="21'
그림8.6riversi 아름공간을문저 안의 루트 요소 안에서 선언
함으로써그라고 아깃에 접두ㅈ屠부가함；으로써그 접두사를 7/
요소가riversi 이름공간에속해 았다는 것을 지정하7/ 위해서
(117p 그림8.8) 문서전반에 컬쳐사용할수 았다. endangered_
species 요소 인에있는riversi 공간을 선언하슨 것으로
endangered_species .1소의 아틈공간에 영향을 마치차
못한다．
카：了∼면三－

二－ㅋ크딱耳code.HnH 邕

纖

<endangered_species xmlns="littp:/Iwww.
cookwood.com/ns/end_species 1"
<animal>
<name language="English">Giant River
Otter</name>...
<source sectionid="122" newspaperid="21"
contentid="630"/>
<rivers:habitat xrnlns:rivers=
"http://www.cookwaod.com/ns/rivers 1">
<rivers:rivers>crivers:name>Amazon</rivers:name>
<rivers:source>Andes Mountain in
Peru</rivers:source>...
그림& 7riversl 아름공간아 rivers:habitat 요소 안에저
선언되었기 때문에 ㅇ／것은 그 요소와 아를 포함하는 요소 안에저만
사용할수 았다. 아것은 rivers:habitat 요소의 밖에서는
사용할수 없다．

===== PAGE 112 =====
111 =====
Using Namespaces in XML
-

lj

c0de'HnH ====＝寸－-

여

<endangered_species
xmlns="http://www.cookwood.com/ns/
end_species! 1.0"
xmlns:rivers="http:!!www.cookwood.com/ns/
rivers! 1.0"!>
<animal>

<!animal>
그림8.8riversl ㅇ／羲z간인珊있는각칵의요소에는rivons
가붙는다. 이것의목척은riversi아름공간에족해았다는것을
보여주는 것아다. rivers:룸쓰는 것은 번거러운 일일 것아다．
http://www.cookwood.com/ns/riversl을쓰는 깃은물론 다
어려울줏）
아다．

댜른 이름 요소돌로 개별 요소듈 구분하기：
1. ＜을입력하아요소를선언한다．
2. prefix：를입력한다. prefix자리에는전페이지
에서 설명했던 것처럼 이 요소가 속해 있는 이름
공간을 지시한다．
3. element를입력한다. element자리에는사용
하고 싶은 요소의 이름을 넣는다．
4. 평소대로요소를마감한다（요소에속성을첨가
하려고 할 경우, 이것이 빈 요소라면 > 혹은 /〉으
로 시작 태그를 마칠 수 있다. 자세한 사항은 1장
.
의 ㅈML 작성밥을 참조）

·／ nPS
■ 요소중에서 그 이름이 접두사에 의해서 선행되
는 것만이 선언된 이름공간으로 확인될 수 있다．
■XML프로세서 (processor）
는 이름공간이 있는
경우에는 접두사가 없는 요소가 디폴트 이름공
간에 속하는 것으로 간주하고（刃끄5참조）이름
공간이 없을 경우에는 이름공간에 속해 있지 않
다고 간주한다．
■XML프로세서는접두사를요소 이름의 필수적
인 부분으로 간주한다. 따라서 마침 태그는 반드
시 시작 태그와 상응해야 한다. 시작 태그의 이
름으로 <rivers:source＞를 썼다면 마침 태그는
</rivers:source＞를 사용한다．
■ 포함된 부분에서 주어진 이름공간으로부터
많은 요소와속성을 사용하고 있다면 최상위의
요소 안에 있는 부분에 관한 디폴트 이름공간을
선언하는 편이 더 편리할 것이다 (P끄5 참조）
.

예제의소즈 코드는 'vw씨cookwood c0m에 았습나다．

117

＝。크m씀只mm* 。
｀ ＝ 느 됴 ㅎ 。 쓰e클． ==

<name language="English">Giant River
Otter</name>
<name language="Latin">pteronura
brasiliensis<!name>
<threats><小reat놔IC址)itat destruction
<rivers:name>Amazon<,/rivers:name>
<rivers:source>Andes Mountains<!rivers:source>
<!threat>
<threat> hunting<!threat>
<threat> overfishing<!threat>
<threat> infection by canine distemper
너rus<／什weal>
<!threat>
<source sectionid=" 122" newspaperid="21"
contentid="630"!>
<picture filename="otter.jpg" x="200" y="197"!>
<rivers:picture fiIe="amazon. pg" x="200"
y="197"!>
<weight>60 pounds<!weight>
<Iength>8 feet long<!length>
<diet><rivers:fauna>fish,
crustaceans<,Irjvers:fauna><,'diet>

접두사를 선언하였거나 이것이 설명하고 있는 이름
공간을 선언하였다면 요소들의 자식들 (children）
에
게 영향을 미치지 않고 접두사를 사용함으로써 개별
요소들을 XML 문서에서 다른 이름공간으로 구분할
수 있다．

===== PAGE 113 =====
112 =====
Chapter 8
속성에 대한 이름공간의 영향
적당한 접두사를 가지고 미리 정하기로 한 속성과
특정한 이름공간을 연계시킬 수 있지만 이것은 거의
필요가 없는 것이다. 속성은 이미 속성들을 포함하고
있는 요소들에 의해 고유한 것이기 때문이다．

내
● *。슨느言＝ 잽奇小● 날。 튜0ㅌ 。 ＝ 多 은

예를들어 source 요소안에 있는 sectionid
속성을보면이것은end_speciesi 이름공간에속
해 있는 source 요소에 속해 있다는 것을 명확하게
알수 있다. 만일 또 다른 sectionid 속성이
orange 요소 안에 있다고 가정하면 다른 여타의 증
거 없이 orange 요소의 부분으로서 sectionid
를 인식할 것이다．
디폴트 이름공간은 속성에 적용하지 못한다는 것을
알아야한다. 어떤 속성이 접두사를（거의 그들이 갖
지 않은）갖지 않았다면 이것은 이름공간이 없는 곳
에 있는 것으로 간주되고 따라서 이것의 범위는 지엽
적일 것이다.
사실 속성의 상황은 지엽적으로 선언된 요소들의 상
황과 크게 다르지 않다. 이것 또한 그들을 포함하고
있는 요소들에 의해서 정의되고 대부분 이름공간으
로 동일화될 필요가 없다．

118

聲邑

,，一，

,

4 code.HrnI

團츠

<source sectionid=' 122 newspaperid=「21
contentid="630"/>
「I>
<orange sectionid="3A
2림89 source와orange 모두sectionid 족정을가지고
있음에도 옭z하고 그들은 동일하게 명명된 요소들아 오버랩돠는
것과같은 방직으로 오버랩되자는 않는다. 첫번째sectionid는
소스에 속해 있고 두번째 것은orange에속해져 았다는 것은 그
무仁］
로 볼 때확실하다. 따라서특정 이름공간으로 그들을 확인하
는 것은 필요하지 않다．

===== PAGE 114 =====
113 =====
Using Namespaces in XML

이름공간, DID, 유효한 문서들
우리는 요소를 단지 그것의 이름으로만 생각하지만
XML 연산자는 prefx:eIemenㅎ로 불리는 요소로
간주한다. 만일 문서를 DTD에 유효한 것으로 만들
려면ㅁrD 안에 있는 각각의 접두사 요소를 선언
해야한다．
덧붙여서 이것이 디폴트 이름공간인가 또는 산발적
으로불리는가에 따라xmln＄나xmlns:prefix와같
은 이름공간으로 선언하는 속정을 선언해야 한다．

DTD에 대한 자세한 정보는 2장 i/m만들刀 (p33)
를참조한다．

예제의소스 코드는 www.cookwoojcorn에 았습나다．

119

＝。크m씀흣mm｀ 듸뮤｀ 。＝`＜흽＝ 。。숟클m= =

이러한 것들이 불편하게 느껴지겠지만 당연한 것이
다. 이름공간에 대한 직접적인 도움의 부족은ㅁrD
가 XML 스키마에 쓰여진 스키마들에 의해 대체되
는 주원인이 된다．

===== PAGE 115 =====
114 =====
NAMESPACES,
SCHEMAS, AND VALIDATION
이름공간, 스키마 그리고 유효성 처리

XML 문서가 8장에서 설명된 것과 같이 다른 이름공
으로 부터 나온 요소들로 만들어졌
간
（Namespaces）
다면 문서를 유효화 하는 일은 보다 복잡한 작업이
될 것이다．
이 장에서는 유효화를 위한 문서 설정법의 세부 사항
이 언급될 것이다．
（실제 유효화를 실현하기 위한 스키마 유효성 처리기
를 사용하는 방법에 관한 자세한 사항은 p245에
나오는 XML 유효화하기를 참조하자）
.

121

＝。클m씀흣mm， 너各m크。 r。 ＝`＜흽＝ 。＝。＝

6장 단순한 타입 정의하기와 7장 복잡한 타입 정의
하기에서 요소를 정하는 스키마와 XML 문서가
구성되어 있는 속성을 만드는 것으로 하나의 종류
혹은 한 계열의 XML 문서를 정의하는 법을 배웠다．
이러한 개별 XML 문서들, 공식적인 명칭으로 실례
와 문서가 유효한 것인가를 알아낼 수 있는 스키마를
비교할수 있다. 다시 말해 XML 문서가 어떤 종류의
문서가되야하는지를（p73참조）보는것이다. 이
방법은 당신의 데이터를 일치시키는 좋은 방법이다．

===== PAGE 116 =====
115 =====
（가apter 9

스키마와 이름공간
이전 장에서 본 것과 같이 이름공간은 일반의 URL
이름에 의해 정의된 관련 요소들과 속정들의 모임이
다. 이름공간은 가장 빈번히 유사하게 이름 붙여진
포괄적으로 선언된 요소들과 다른 것들（고유한 본문
으로 일반적으로 만들어진 지엽적으로 선언된 요소
들）
을 구별하는데 가장 빈번하게 사용된다. 이름공간
의 이름은 언제나 고유하기 때문에 이름공간과 요소
이름은 역시 고유한 것이기 때문이다．

m
● V。 튜● ㅌ。＝ 七
＝ 。m。 ㅌ 료 욹

하나의 이름공간으로 정의된 요소를 가진 문서를
유효화할 때 특정 요소가 고유하다는 것을 아는 것만
으로는충분하지 않다. 이것이 어떻게 정의되어 있는
가또한 알아야한다는 것이다. 예를들어 언제 얼마
나자주요소가등장하는지, 요소가포함해야하는
다른요소는무엇인지, 요소가포함할속정은무엇인
지 등이다．
모든 정보는 주어진 스키마 즉 특정 이름공간의 요소
들이 정의된 스키마에 포함된다．
따라서 스키마는 XML 문서의 형태를 정의하는 동시
에 이름공간을 만들고, 스키마가 포함하고（또한
정의하고）
있는 요소와같이 존재하게 만들 수 있다．
스키마의 요소들은 특정 이름공간과 연결된 후에는
이름공간으로 접두사가 붙은 요소는 다른 문서에서
도사용할수 있다. 그리고 그러한문서들은 이름공
간과 공존하고 있는 스키마를 봄으로써 유효화될 수
있다.

122

===== PAGE 117 =====
116 =====
Namespaces,Schemas,and Validation
<?xml version="1 .0" ?>

c de.tisd

<xsd:schema xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema"
targetNamespace="http://www.cookwood.Com!
ns/end_spedes 1 ">
<xsd:element name="endangered_spedes">
<xsd:complexType>
<xsd:sequence>
<xsd:element name="animal"
type="animallype"
maxOCCurs="unbounded"/>
</xsd:sequence>
</xsd:complexType>
</xsd:element>

</xsd:sequence>
</xsd:complexlype>

.1림9.1 ㅇ／예처］에서endangered_species 요소와animal
Type 복잡한요소는http :www. cookwood. com/ns/end_
speciesl ㅇ］름공간으로 정의되어 았다. animal threats,
의요소가 아나므로 이틈
weight 요소들은그들아 촤상위 단겨）
공간으로 정의될 수 없다．

예제의소스 코드는 www.cookwood.com에 있즙나다．

최상위 단계에서 포괄적으로 선언된 스키마의 성분
과이름공간을연결시킬수있다. 이는다른스키마
문서에서 이러한 성분을 이용할 수 있게 하기 위한
것이다. 포괄적으로 선언된 성분은xsd: schema
요소의 직계 자요소 (direct child）
이고 요소 선언과
속성 선언, 복잡하거나간단한타입 정의, 명명되어
진 그룹 정의 그리고 속성 그룹 정의가 될 수 있다．
실제적인 정의 혹은 선언에서 특별한 조치를 할 필요
는 없다. 다시 말해 단순히 6장과 7장의 지시에 따라
하면 되는 것이다. 그러나 성분과 연결시키고 싶은
타것7 이릉공간을 정해야 한다．
타겟 이름공간 정하기
스키마 문서의 루트 요소에서 targe削amespace=
"URL＂을 입력한다. 여기서 URL은 이 스키마 안에
서 정의된 성분과 연결하려는 이름공간이다. 이것은
상주 이름공간이라고 한다．

'/ nPS
■ 최상위 단계에서 단지 포괄적으로 선언된 성분
들은 그 이름공간과 연관이 있다. 이것은 지엽적
으로 선언된 것 그리고 그림 9.1의 animal
요소처럼 관련없는 아이템을 사용하지 못하거나
유효화되지 못한 것을 의미하는 것은 아니다．
그림에 나온 스키마에 의해 XML의 예를 유효화
할 때 연산자는 endangered_species 요소의
정의를 어디서 찾아야 할지 알게 될 것이다．
연산자는 endangeied_species 요소가 반드
시 부적격의 animal 요소（이름공간과는 상관
없는 것）
를 포함한 것을 알게될 것이다．

123

七。 ＝등＝ =．。＝。크巾씀흣g

</xsd:complexlype name="an imallype">
<xsd:sequence>
<xsd:element name="name" type="nameType"
minOccurs="2"/>
<xsd:element name="threots"
type="threatslype"/>
<xsd:element name="weight"
type="xsd:string" minOCCurs="0"
maxOccurs=" 1 "I>

이름공간의 상주

===== PAGE 118 =====
117 =====
（十apter9

지엽적으로 선언된 모든 요소 첨가
하기
디폴트 값에 의하면 최상위 단계에서 단지 포괄적으
로 선언된 성분들만이 타겟 이름공간과 관련되어
있다. 지엽적인요소선언과정의를더하고싶다면
（예를 들어 하나 이상의 단계 아래 있는）모든 요소를
한번에 첨가할 수 있거나 혹은 아래 보이는 것과 같
이 모든 속성 선언을 한번에 첨가하거나혹은 p125
에 나온 것처럼 요소와 and/or 속정들을 각각 첨가
할 수 있다．
탸겟 이름공긴애 지엽적으로 선언된 모든 요소
첨가하기：
＝口· ㅌ으山， ●，。＝음＝ iV。 “ -＜。 ＝乞召

xsd: schema 요소에서 이ementFormDefa이ㅎ＝
"qualified" 를 입력한다．
타겟 이斗따긴에 지엽적으로 선언된 모든 속성
첨기하기：
xsd: schema 요소에서 얘ributeFormDe拓dㅎ＝
"qudified"를 입력한다．

code.HSd
<?xml version= 1 .0∥ ?>
<xsd:schema xmlns:xsd="htip://www.w3.org/
2000/10/XMLSchema"

回F

targetNamespace='http://www.cookwood.com
Ins/end_species1">
elementFormDefault= 'qualified '>
<xsd:element name="endangered_species">
.cxsd:complexType>
<xsd:sequence>
<xsd:element name="onimal"
type="animalType"
maxOccurs='unbounded"/>
</xsd:sequence>
</xsd:complexlype>
</xsd:element>
<xsd:complexlype name="animallype">
<xsd:sequence>
<xsd:element name="name" type="namelype"
minOccurs="2"/><xsd:element
name="threats" type='threatslype"/>
<xsd:element name="weight'
type="xsd:string" minOccurs='0"
maxOccurs="1"I>
</xsd:sequence>
</xsd:complexlype>

I, 1iPS
■ 위에서 언급된 바와 같이 그 속정들의 각각의
디폴트 값은 적당하지 않은 값이다. 이것은 다른
방식으로 정의하지 않는 한 최상위 단계에서
단지 포괄적으로 선언된 성분만이 타겟 이름공
간과 연결될 수 있다는 것을 의미한다．

124

그림9.2자엽적으로선언된요소들animal, threats, 그라고
weight들은 이름공간과 연결돠아 있고xML 문서叩서조화톱게
설명될 수 밌다．

===== PAGE 119 =====
118 =====
Namespaces,Schemas,and Validation
Code.usd

rㅍL

<?xml version="l .0' ?>
<xsd:schema xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema"
targetNamespace="http://www.cookwood.com
/ns/end_species1"
elementFormDefaulf="qualified">
.cxsd:element name="endangered_species">
<xsd:complexType>
<xsd:sequence>
<xsd:element name="animal"
type="animallype"
maxOccurs="unbounded"/>
</xsd:sequence>
</xsd:complexType>
</xsd:element>

폼속정은특정의, 개인의, 지엽적으로선언된요소
가 디폴트에 관계없이 (p124 참조）타겟 이름공간과
연결되는 것을 정하는데 유용하다．
타겟 이룝공긴허1 지엽적으로 선언된 요소 첨가
하기：
요소 선언에 form="qu이ifieci" 를 입력한다. 이
요소가 어디서 선언되었는지에 관계없이 이것은
타겟 이름공간과 연결될 것이다．
Xsd: schema 요소안에서 elementForinDefault
="qualified∥속정을 사용했다면 지엽적으로
선언된 특정 요소가 타겟 이름공간과 연결되지 못하
게 하는데 폼속성을 사용할 수 있다．
지엽적으로 선언된 특정 요소가 타겟 이묩공간과
:
연결되지 못하게 하기（디폴트 값에 관계없이）
요소선언에서 form="unqualified" 를 입력한다．

</xsd:sequence>
</xsd:complexlype>
.2림오3xsd: schema 요소叩저 elementFormDefault를
설정했응에：도 불구하고 threats나weight 요소들은 타겟 아름
공간과 연결될 것ㅇ／다. 왜냐하면그들의폼(form) 속성은
elementFormDefault 값을 무사하가 때문아다．

예제의소스 코드는 www.cookwood.com에 있습나다．

125

口
m
● ｀쯔審크● 三
盼
＞立＝ .，口言드口m尸。 ＾흽i붕＾日

</xsd:complexlype name="animaIType">
<xsd:sequence>
<xsd:element name="name" type="namelype"
minOccurs="2"/>
<xsd:element name="threots"
type="threatslype" form="unqualified"/>
<xsd:element name="weight"
type="xsd:string" minOccurs="0"
maxOccurs=" 1" form="unqualified"/>

지엽적으로 선언된 특정 요소 첨가
하기

===== PAGE 120 =====
119 =====
태apter9

성분을 이묩공간으로 설명하기
스키마 성분（단순한 혹은 복잡한 명명되어진 타입
들：요소, 속정, 속성 그룹, 그리고 명명되어진 그룹
들）
을 이름공간과 연결시켰다면 (pi23참조）그것은
그스키마나혹은다른스키마로설명할수 있다. 그
리고 그들은 이름공간과 연결되어 있기 때문에 그들
을 설명할 때는 이름공간을 정해ㅇ爐枓．
이 책에서는 xsd 접두사를 모든 XML 스키마 요소
에 사용했다. 그리고 스키마의 루트 요소 안에서 적
절하게 xM. 스키마의 스키마（일반적으로 이것은
스카마들 중의스7／마라고 불린다）
를 선언해 왔다．

그러나 자기 자신에서 유래를 찾는 주문형 타입（단
순한 것이나 복잡한 것）
의 경우는 어떨까？혹은 설명
하고 싶은 요소 혹은 속정 선언의 경우는 어떨까？혹
은 설명하고 싶은 그룹의 경우는？이들 중 어느 하나
의 설명도 반드시 그들과 연관된 이름공간에 대한 정
보를 포함하고 있어야 한다．
관련된 성분의 디폴트 이름공간과 스키마 안에서
성분의 관련 지정하기：
1. 스키마문서의 루트요소안에서xmlns="URL"
을 입력한다. 田話자리에는설명된 성분들과
관련이 있는 이름공간을 입력한다．
2. type과ref 성분의 값에서 reference를 입력
한다（접두사없이）
. reference자리에는디폴트
이름공간과 관련된 성분의 이름이 들어가게 된다．
다．

·
●
V
。 튜● ㅌ口＝ 츱m놀＝ ＝·＝읖ㅌ 。닐m= =＝●，●*●“

이의 이유는 고유의 타입（스키마들 중의 스키마에서
미리 정의된 타입들）
을 설명할 때 이들 앞에 XS(f
접두사를 넣을 필요가 있어서이다. 이런 방식으로
스키마는 그들의 정의를 찾을 수 있다.

126

mde.Hsd 휼公

<?xml version="1.0' ?>
<xsd:schema xmlns:xsd="http://w-ww.w3.org/
2000/10/XMLSchema"
targetNamespace="htip://w-ww.cookwood.com/
ns/end_speaesl "
xmlns="http://www.cookwood.com/
ns/end_speciesl "I>
<xsd:element name="endangered_species">
<xsd:complexlype>
<xsd:sequence>
<xsd:element name="animal"
type="animclType"
maxOccurs="unbounded"/>
</xsd:sequence>
</xsd:complexType>
</xsd:element>
<xsd:complexlype name="animallype">
<xsd:sequence>
<xsd:element name="name"type="nameType"
minOccurs="2"/>
<xsd:element name="threats"
type="threatsType">
<xsd:element name="weight"
type="xsd:string" minOccurs="0"
moxOccurs=" 1"/>
</xsd:sequence>
</xsd:complexlype>

그림요4스7／마의루트 요소 안녜저 이스카마문저를 위한 다폴트
아름공간인end_speciesl을선인했다. 이것의의II／는 접두사가
없는（unprefixedj타입의정의가(animal Type, nameType,
2라E threatsType) end_speciesi 이륭공간에상응하는
스키마 안에저 발견된다는 것을 의U'한다（첩두사 타입xsd:
string의정의는xl4L스키마 이름공간과상응하슨스카마
x인에서 발견된다）
.

===== PAGE 121 =====
120 =====
Namespaces,Schemas,and Validation
수축子＝==-m릎
tode. isd＝소욕뉵슥뉵뇩H4i日．

孕口

<?xml version="1.0" 2>
<xsd:schema xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema"
targetNamespace="http://www.cookwood.com/
ns/end_speciesl"
xmlns:end="http://www.cookwood.com/
ns/end_speciesl "I>
<xsd:element nome="endangered_species">
<xsd:complexlype>
<xsd:sequence>
<xsd:element name="animal"
type="end:animalType"
maxOccurs="unbounded"/>
</xsd:sequence>
</xsd:complexlype>
</xsd:element>
<xsd:complexlype name="animallype">
<xsd:sequence>
<xsd:element name="name"
type="end:namelype" minOccurs="2"/>
<xsd:etement name="threots"
Iype="end:threatslype">
<xsd:element name="weight"
iype="xsd:string" minOccurs="0"
maxOccurs=" 1"I>

예젱의소스 코드는 www.cookwood.com에 있습나다．

2. type과ref 족성값안에서prefix:reference
를 입력한다. reference 자리에는 접두사（이
prefix는1번의 것과 같다）
에 상응하는 이름공간
과 연결된 성분의 이름이 들어간다.

'/ nP$
=

■ 필요한만큼의 이름공간을 선언할수 있고, 상응
하는 접두사를 사용함으로써 그들 사이에서
정의된 정의를 사용할수 있다．
m

■ 족성값이 이敭｝
간과（혹은 이름공간이 없을 때
도）연결되어야 한다는 것은 절대 직관적으로
와닿는 것이 아니다. 그러나 이것은 이 책에서
의 작업 방식이다．
■ 이 중요한 차이점을 기억하자：타겟 이름공간은
실제 활동적으로 성분과 이름공간을 연결한다．
x세ns="URL" 혹은xmlns:end="URL"과
같은 이름공간은 어떤 이름공간이 성분과 연결
되어 있었음을 단순하게 밝혀준다．

127

一

蠟

m
一
淞
篩

그림 9.5 아문서는p126의그림9. 4이］나오는 것과동등한 것아다．
이번에는end_speciesi 아름공간을 설명하는 접두사end룰
정의하였다. 따라서end: animalType, end:nameType,
end: threatsType 셋모두가end_speciesi 아름공간에
속해 있다슨 것을 ㅈ］사하는 그 접두사틀 사용해야 한다. 요소가
예전과 같은 이름공간에 속해 있다는 점이］주목해야 한다（아것은
targetNamespace족정에의해서조절된다커 여가서는그들을
중명하는 방탭을 단순하게 바꿨다．

1. XML문서의루트요소에서xmlns:prefix=
"IJRL＂을 입력한다. prefix자리에서는 URL에
의해 지정된 이름공갼에 속한 스키마 안에 정의
를 표시하는 방법을 밝힌다．

蹠蛾

</xsd:sequence>
</xsd:complexlype>

접두사가 있는 이룝공z욜 선언하고 그 접두1隱
사용하여 스키마에 있는 설명된 성분에 자격
부여하기：

===== PAGE 122 =====
121 =====
Chapter 9

디폴트로서의 스키마들 중의 스키마

騙·－눗듈一

xsd를 갖고 있는 스키마 중의 스키마로부터 요소와
타입들께 접두사를붙여야하는 법은 없다. 예를들
어 개인적인 취향에 따라 zap 혹은 boffo와 같은 것
을 쉽게 사용할 수 있다. 실로 만일 자신의 스키마가
고유 타입들로 주로 구성되어 있다면 다폴트 이름공
간으로서 스키마들 중의 스키마를 선언하는 것이
훨씬 빠르고 쉬운 방법이고 이것의 이름공간부터
요소에 접두사 붙이는 것을 생략할 수 있다．

<schema xmlns="http://www.w3.org/
2OOO/1O/XMLSchema"

。 ·。ㅌ르날너 *。 。ㅌ●七 ＂0츱
=＝遼음 ●솥 m

1, 스키마를시작하며, XML선언후에＜schema
를 입력한다（이것이 xsd:schema가 아닌 것을
주목）
.
2. 다음에xmlns="http://www.w3.org/
2000/10/XMLSchema''를 입력한다. 이것은
당신이 쓰고 있는 스키마의 디폴트 이름공간으
로서 스키마 중의 스키마임을 선언하기 위해서
이다．
3. targetNamespace="URL"을입력한다. URL
자리에는 최상위로 명명된 타입 정의와 요소
（보통의）
를 연결하고자 하는 이름공간이 들어
간다．
4. xmlns:prenx="URL" 을 입력한다. prefix자리
에는 URL에 의해 지정된 이름공간에 속해있는
이 스키마 안에서 작성자의 정의를 표시하는
방법이 들어가게 된다.
5. 이 스키마에 사용된 정의를 포함한 각각의 이름
공간을 위해 4번을 반복한다．
6. ＞을입력하여 스키마태그를마친다．

'/ 1:P
■ 당신은 타겟 이름공간에 하나의 접두사를 설정
할 필요가 있을 것이다（만일 다른 이름 공간으
로부터 정의를 유입하지 않았다면 자세한 사항
은p132를참조）
.

128

區듣

</sequence>

targetNamespace="http://www.cookwood.com/
ns/end_species 1"
xmlns:end="http://www.cookwood.com/
ns/end_species 1">
<element name="endangered_species">
<complexlype>
<sequence>
<element name="animal"
type="end:animalType"
maxOccurs="unbounded"/>
</camplexType>
c/element>
<complexType name="animalType">
<sequence>
<element name="name"
type="end:nameType" minOccurs="2"/>
<element name= threats"
type="end:threatslype"/>
<element name="weight" type="string"
minOccurs="0" maxOccurs="1"I>

</sequence>

스키마를 위한 디폴트 이름공간으로서 스키마들
중의 스키마 선언하기：

c.de.H$d－專毫二二玉＝

<?xmt version="l .0"?>

</complexType>

그림9.6 아 문서는p126에 나오는그림9.4와같은 것아다 (.2라고
2람9.5-i같은걋아다）
.단한가자치까컴은
p127에나오는.
표가밥叩 甲한문제아다. 여가저는스키마중의스7／마를 다폴트
아름공긴으로 선언했다. .2래서요소 아話(schema, element,
복잡한타입둥）
에xsd를가지2 prefix 할괼요가 없었다. 다른
한편으로end:animalType, end: naineType 그리고 end:
threat Type의 경우치렁 다른 이름공간으로부타 오는 타입에
대해 접두사 붙이7／를 해야 한다．

===== PAGE 123 =====
122 =====
口

cOtle.W.d

1羈·

Namespaces,Schemas,and Validation
<2xm1 version="].0" 2>
<end:endangered_species
xmlns:end="http://www.cookwood.com/ns/
end_species]">
<animal>
<name language="English">Tiger</name>
<name language="Latin">panthera tigris</name>
<threats>
<threat>poachers.c/十roots>
＜小reat카abitat destruction</threcit>
<threahtrade in tiger bones for traditional
Chinese medicine (TCM)</threat>
c/threats>
<weight>500 pounds</weight>
<length>3 yards from nose to taik/Iength>
</end:endangered_species>

이제는 성분들의 세트를 정하고 그러한 성분들을
사용하는 문서를 유효화할 준비가 되어 있을 것이다．
6장과 7장에서 문서를 유효화할 때 이름공간에 대해
서는 걱정할 필요가 없었다. 왜냐하면 정의하고 있는
어떤 성분도 타겟 이름공간과 연결시키지 않았기
때문이다. 이제 성분의 전부 혹은 일부분은 이름공간
에 속하게 되었고 그러한 문서를 유효화할 때 XML
문서 안에서 이러한 성분에 대한 이름공간을 정해야
한다．
또한 연산자가 이름공간이 연결되어 있는 성분이
정의되어 있는스키마 문서를 어디서 찾을 수 있는지
정해야한다．
숭인된 성분으로 유효한 XML. 문서 작성하기：
을
1. 당신은디폴트이름공간 (xmlns="URL"）
선언하고 성분이 있는 접두사를 사용하지 않음
으로써 혹은 접두사 (xmlns:prefix="URL"）로
이름공간을 선언후 원하는 성분을 접두사 붙이
기를 하여 원하는 성분의 이름공간을 지정해야
한다. 8장xML의 아름공간사우하기에 이 과정
이 보다 자세하게 나와 있다．
2. 간혹요소들에게 권한을부여하는데 사용하는
이름공간을 정의하거나 혹은 동시에 존재하게
하는 스키마문서들이 어디서 발견되는지 지정
하는 것도 필요하다．

V nF'
■ 이름공간과실제적으로연결되어진요소들에
권한을 부여하는 것을 기억하자．

예계의소스 코드는www.cookwood.com叩 있습나다．

129

＝。클m씀흣mm。 ＝`＜흽＝ 。＝=．乂글尸

그람9.7p126의그림9. 4의스7／마 인珊저그리고 그 스카ㅁ／안의
峽getNa／끄espace 족겅 때문에 endangered_species 요소
는 이름공간
（http://www.cookwood.com/ns/endspecies])과
연결되어져 있다. 만일 이요소（보여진 XML 보기ㅊ／럼；틀포함한
문저를유효화 하고 싶다연 endangered_species가상응되게
해야한다．왜나하연animal (2리고 다른요소들）
은 target
아름공간과 연관되아 있자 않으므로 嫩f에 나와있는 차사 사항은
팔꾜없다.

이름공간과 XML 유효화하기

===== PAGE 124 =====
123 =====
Chapter9
스키마의 위치 지정하기

ㅁ

XML 문서에 정해진 요소가 없을 때 스키마의 위치
.
를 어떻게 정하는지 이미 살펴보았다 (p73 참조）
정해진 요소를 포함하는 XML 문서에 대한 스키마의
위치를 정하는 것은 그와 비슷하다．

<end:endangered_species
xmlns:end="hnp://www.cookwood.com/ns/
end_species 1"
xmIns:xsi="http://www.w3.org/2000/ 10/
XMLSchemo-instancen

정해진 요소들에 대한 스키마의 발견 위치 지정
하기：
1. XML문서의 루트요소안에서 정해진요소와
연결되어 있는 이름공간의 선언 다음에서
xmlns:xsi="http://www.w3.org/2000
〃O/XMLSd,ema-instance∥를 입력한다．
이것은 스키마 위치를 지정하는 속성이름을
선언하기 위함이다．
갭口ㅌ 읖Vm。 쑈● ，클m= ＝。＝{=

2. xsi:schemaLocati이｀="URL을입력한다. 여기
서 URL은 위치하고자 하는 스키마 문서의 이름
공간의 이름이다（여기에는 큰 인용 부호가 없음
을주의해라）
.
3. 스페이스바를누른다（리턴 키도무방）
.
4. 다음仙e.xsd"를 입력한다. file.xsd는 이 XM.
문서안에서 사용되는 이름공간을 정의하는 스키
마를 포함하는 실제 파일의 URL이 들어간다.
5. XML문서가요구하는스키마만큼2-4번을
반복할 수 있다．

V Tip
■ 대부분의 XML 연산자들이 상응하는 스키마
파일을 찾기위해 xsi= schemaLocation 속성
을확인할것이다. 모든 연산자가 언제나찾는
것은 아니다. 자세한 사항은 xM. 연산자의
설명서를참조한다．

130

c0de.11nH

<?xml version=" 1.0 " ?>

xs:schemaLocation='http: //www.cookwood.com/
is/end_species]
呻：//www.cookwood.com/xml/schemas/
end_species1.xsd'>
<animal>
<name language="English">Tiger</name>
<name language='Latin">panthera tigrisc/name>
<threot>
<threat>poachersc/threats>
<threo나abitat destruction</十reat>
<threat>trade in tiger bones for traditional
Chinese medicine (TCM)</threat>
</threats>
<weight>500 pounds</weight>
<Iength>3 yards from nose to taik/Iength>

그림9.8 처음 빨간색으로 된 줄은xsi를 접두사로 가진 아이템을
위한 아륭공간을 선언하고 있다. 두번째 빨간색ro 된줄은 이틈
공간을 차정하고 았는데 아것은 세빈째 열이 아름공간아 정의된
서버의질제 파일임을 ㅈ］정햐고 있다．

===== PAGE 125 =====
124 =====
Namespaces,Schemas,and Validation
m
＝느尸code.Hsd…
<?xml version="1.0" ?>

퓨．
肖

스키마의 성분을 여러 가지 개별 파일（공식적으로는
스키마문서라고 한다）
로 나눌 수 있다. 이것의 목적
은 여러 가지 다른 스키마와문서에서 개별 파일을
다시 사용하거나 혹은큰 스키마들을 다루기 쉽게
하기 위함이다．

<xsd:schemo xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema"
targetNamespace="http://www.cookwood.com/
ns/end_species 1"
</xsd:complexlype name="threatsType">
<xsd:sequence>
<xsd:eement name="threat"
maxOccurs="unbounded1'!>
</xsd:sequence>
</xsd:complexlype>

스키마 성분 포함하기：

그림9.9 처음0로 threatsType 복잡한 타입 정의를 아용하여
새로운파일 (threat.xs 여刀서보아는)을 만들었다. 又／금부타
다른스캬마에서이정의를 사용할수 있다．

旣；j
code.esd
<?xml version="1.0" ?>

…

복수 파일에서의 스키마

ㅁ卽

<xsd:element name="endangered_species">
<xsd:complexlype><xsd:sequence>
<xsd:element name.="animaI"
type="animallype"
maxOccurs="unbounded"/>
</xsd:sequence>.c/xsd:complexlype>
</xsd:element>

VTiF1s
■ 포함된 스키마문서의 타겟이름공간 (targetNamespace) 속성은 반드시 성분을 받을 수
있는스키마문서와같은것이어야한다. 스키마
성분을 다른 타겟 이름공간에 첨가하기 위해서
는 p132에 나오는 성분의 우입을 참조한다．
■ 만일 포함된 스키마가 정해진 타깃 이름공간이
없을 경우 이것의 타깃 이름공간은 이것이 포함
되어지고 있는 스키마 문서를 위한 타깃 이름공
간으로 가정한다．

<xsd:complexType name="animallype">
<xsd:sequence>
<xsd:element name="name"type="namelype"
minOccurs="2"/>
<xsd:element name="threats"
type="threatslype"/>
.</xsd:complexlype>
그림9.10 xsd: include 요소를사용함으로써 다른스7／ㅁ7들로
부타 나온스캬마 성분을 같은 아름공간을 이용하여포함할수 있게
돠었다．

예재의소스 코드는 www.cookwood.com에 있즙나다．

131

茗크무 ＝클드孑r= =
m

targetNamespace="http://www.cookwood.com/
ns/end_speciesl"
xmlns="http://www.cookwood.com/
ns/end_spedesl ">
<xsd:include schemaLocotion=
"http://www.cookwood.com/xml/schemas/
threats.xsd"/>

2. 성분을포함하려고하는스키마문서 안에서
xsd: schema의 바로 다음에 <xsd:include
schemaLocation="incIuded-file.xsd"/>를
입력한다. indudedfi]e.xsd자리에는포함하려
고 하는 성분을 포함하는 스키마 문서의 Urn川
들어가게 된다．

＾
盼

<xsd:schema xmlns:xsd="http://www.w3.org/
2000/10/XMLSchema"

1. 스키마성분을파일로나눈다. 각각의 파일은
텍스트여야하고 .xsd확장자로 저장된다．

===== PAGE 126 =====
125 =====
Chapter9

성분의 유입

斗j

당신은 XML 문서의 요소들이 하나 이상의 이름공간
과 연결된 XMI 문서의 유효를 위해서 다른 타겟
이름공간들을 가지고 다른 스키마들로부터 상위
단계의 스키마 성분을 유입할수 있다．

<xsd:schema xmlns:xsd="http://w'ww.w3.org/
2000/10/XMLSchema"
xrnlns:xsi="http://www.w3.org/2000/10/
XMLSchema-instance"
targetNamespace="http://www.cookwood.
com/ns/end_species1"
xmlns="http://www.cookwood.com/
ns/end_speciesl "
xmlns:rivers="http://www.cookwood.com/
ns/riversl ">

다른 타깃 이룸공간의 스키마로부터 성분 유입
하기：
1. 스키마성분을넣으려는스키마문서 안의
xsd: schema 요소바로다음에 <xsd:import
를 입력한다．
2. 그리고namespace="URL"을입력한다. 여기
서 URL은 입력된 스키마 성분과 관련이 있는
이름공간의 이름을 지정한다．

=＝·＝。｀ㅌ。Um= =bO口ㅌ

3. 필요에따라파일의 위치를정한다. 그파일은
스키마를 포함하고 있고 그 스키마는 2번에서
xsi:schemaLocation="URL을씀으로서 이름
공간을 정의하는 스키마이다. 여기서 UR1은
위치를 지정하고자 하는 스키마 문서를 갖고
있는 이름공간의 이름이다．
4. 스페이스바를누른다（리턴키를눌러도된다）
.
5. file.x,sd를입력한다. me.xsd＂는당신이유입하
고자하는 성분을 갖고 있는 스키마를 포함하는
실제 파일의 URL이다．
6. /＞을입력하여xsd: inportant 태그를마감
한다．
7. p126에설명된것처럼유입된이름공간을위한
접두사를 선언하게 된다. 이렇게 되면 자신의
스키마에서 유입된 성분을 설명할 수 있게 된다．

VTip
■ 아직 모두완성하지 못했다면 l30p의 1번과
같이 XML 스키마 보기 요소를 선언해야 한다．

132

=

c0de.l4$d小i1릎

<?xm version= 1.0∥ ?>

<xsd:import namespace=
"http://www.cookwood.com/ns/rivers 1'
xsi:schemcitocotion=
http://www.cookwood.com/ns/riversl
"http://w'ww.cookwood.com/xml/schemas/
rivers.xsd"/>
<xsd:element name="endangered_species">
<xsd:complexlype><xsd:sequence>
<xsd:element name="animol"
type="animalType"
maxOccurs="unbounded"!>
</xsd:sequence></xsd:complexlype>
</xsd:element>
<xsd:complexlype name="animalType">
<xsd:sequence><xsd:element name="name"
type="namelype" minOccurs="2"/>
<xsd:element name="threats"
type="threatslype"!>
</xsd:element name= 'habitat"
그림9．
끄 하나의스7／마를 다른스카마로 끌어오는 것은 (import)
은 포함하고 았는스카마 안에서 성분을 정의하는녜 사용 가눙한
스7／마로부타 성분을 만드는 깃아다．

===== PAGE 127 =====
126 =====
PART 4:
XSLT와 XPath
乂弘T 135
XPath: 패틴과표현 γ53
테즈트 표힌과 함수 γ63

133

===== PAGE 128 =====
127 =====
10

XSLT
XSLT

XML을 포맷하고 변환하는 완전하고 공식적인 제안
은XSL（이것은 Extensible Style Language의
약자이다）
이라고 불리는 상세서 안에 포함되어 있는
것이다. 그러내 이것은 결론을 짓기 어렵기 때문에
W3C는XSL을두조각으로 나누었다. 그것은
XSLT（변환용）그리고 XSL-FO（포맷용）
이다．

XSL-FO가 아직 정형화되지 않았고 어떤 브라우저
도 지원하지 않기 때문에 이것은 이 책에서는 다루지
않을 것이다. 이것의 최근 동향에 대해서는 http.
www.w3.org/Style/XSL／에서 짖아볼 수 있다．
그동안 XSLT는 널리 알려진 CSS (Cascading
S柳e Sheets, 이것은 실제 포맷을 다루는 것이다）
와의 연동을 해왔다. css에 관한 더 자세한 사항은
p175에서 시작되는 Part 5를 보면 된다．
책의 이 부분의 예제들은 하나의 XML 파일과 각각
의 것이 이전 것을 기초로 하는 XSLT 파일의 연속
적인 세트를 기초로 한 것들이다. XSLT 파일의
전부는 아니더라도 XML 파일을 다운로딩하거나
프린트하기를 권유한다.

135

님鷺뻐

이번장과 뒤에 나올 두 장에서는 XSLT를 이용하여
XML문서를변환시키는것을설명할것이다. 새로
운 버전의 브라우저에나 기존의 브라우저에 보이는
결과는 보다 평범한 HTML 문서나 또는 다른 XML
문서가 될 것이다. XML 문저를 변환하슨 것은 이것
의 컨텐츠를 분석하고 어떤 요소들이 발견되는가에
의존하여 특정한조치를 취하는 것이다. XSLT를
이용하여 특정 표준에 따라 결과물을 다시 주문할 수
있고 어떤 정보의 덩어리를 보여줄 수도 있고 그 외
에도 많은 것들을할 수 있다．

===== PAGE 129 =====
128 =====
XSLT 연산자가 하는 첫번째 일은xM. 문서를 분
석하는 일이다（그림 10.D. 그리고 이것을 노드 트리
(node tree）
로 변환하는 것이다（그림 10.2). 하나의
노드는 XML 문서의 하나의 개별 조각에 불과하다
（하나의 요소나 속정 또는 텍스트 컨텐츠）하나의
노드 트리는 전 XML 문서의 계급 체계의 상징이다.

． 큽 님 圭 클 “毛님m＝ 겯느。 七＝ 므h

소스 XML에서 연산자가 노드를 정의하였다면 이것
은 노드를 가지고 무엇을 할 것인가에 대한 설명서인
XSLT스타일 시트를주의할 것이다. 이러한설명서
들은 템플랏 안에 포함되어 있다. 각각의 템플릿은
두부분을가지고 있다. 하나는템플릿이 적용될 수
있는 XML 문서 안에서 노드를 정의하는 라벨 종류
이고 다른 하나는 실제 변환에 대한 설명서이다．
연산자는 자동적으로 루트 템플랏을 찾는데 이것은
XML 문서（가장 먼 요소를 포함하는 것）
의 루트
노드에 적용할 수 있다. 루트 템플릿은 일반적으로
문자 요소의 조합을 포함하고 소스 문서에서 결과를
내거나 노드들을 더 연산하는 XSLT설명서를 포함
한다．

136

그림蚣i 책의 웹사이트에는 아 장의 예제 안녜서사용된XM【』
전문을 발견할수 있다. 아 여7격］룰보는 동안에참조울로 아것을
다운벋까프린트할 것을 권우한다．

루트노드
. ,

endange員， .s
-

name //

C

pecies

실제 변환을 하기 위해서 XSLT 연산자가 필요하다．
Instant Saxon (Michael Kay）
을 포함해서 온라인
으로 가능한 것들이 있다. 자세한 사항은 p246에 나
오는 XSLT 연산자로 XML 반환하기를 보면 된다．

一呼努韆·

<endangered_species>
<animal>
<name language="English">Tiger</name>
<name language="Latin">panthera
tigris</name>
<threats><出reat>poachers</十reat>
《十reat하祉itat destruction</threat>
<threat>trade in tiger bones for traditional
Chinese medicine (TCMk/threat>
</threat>

d_

전체 변환 과정을 살펴보는 것으로 시작하자. 그
다음 세부 사항을 알아보기 위해서는 이 장（그리고
앞으로 나올 두 장）
의 나머지 부분을 보아야 한다．

ode.HmI

J

<?xml version=" .0" ?>

-1

XSLT로 XML 변환하기

f=

Chapter 10

Hanguage- LEnglish
Luiger

name
language ．텍스트
Latin二／노드
p미,thera tigris
出teats
小reat
poachers
t卜re햐
"bitat destruction
什we아
trade in tiger...
weight
500 pounds

-

an,

斗 name
니anguage

I Ln_..I:.1.
- ㄴ∥V벳∥
미ack Rhino

etc.

etc.
그림10.2 그림10.1에저보여진 XML 문서에 상웅하는노드 트리의
부분적안 모습을보고 있다．

===== PAGE 130 =====
129 =====
XSLT
c de.11$n

巨

<?xml version="l.0"?>

<xsl:sMesheet
xmlns:xsl="http://www.w3.org/19 루트 템플릿
orm"version="1.0">
_- （언졔나 우선한다．
)
<xsi:temoiare matcn= I ">

<h呻<head><t

오타들
（출력 그대로의）

En和n百er렉－

</ title></ necia><Doay ogcolor=" 다른 템플릿을 호출하는
xs' 지시 명령

<xsl:opply=template -

select="endangered_species/animal"I>
뼈y>

'／

부가적인 템플릿（명확히
명명될 필요가 있는）
</html></xsl:template>
I .
,,（기 >
<xsl:rempuore mulcn= crnim
-

-

-

-

-

<p olign="center"><xsl:apply-templates
select="name"/></font></p>
<br/?<font size="+3">cxsl:apply-templates
select="name"/></fonb.</p>
<table width="100%"border="2"
<tr><th>S아)species</th><th>
Number Left</th><th>As Of<

결과를 연산하는 xsl 지시
명령（다른 템플릿은 호출
하지 않는다）

<xsl:sort S히ect="pop이.
type="number"/>
<xsl:sort select="population/@year「datatype="riumber"/>
<tr><td><xsl:apply-temHates
select="name"/>.c/td>
<td><xsl:value-of select='region"/></td>
그림10.3 XSLT스타일시트 전문은책의 웹사이트에서 볼수 았고
편의를 위해저 다운로드와프린트를 하는 편이 좋다．

예젱의소스 코드는 vcww.cookwood.corn에 있습나다．

표현과 패턴을 이용하여 노드 세트와 그에 상응하는
템플릿을 정의하고 선택한다. 이런것들은 Xpath
syntax에 쓰여져 있으며 그들자신의 장들을보장해
줄 수 있는복합체이다. Xpath 패턴과표현 (Pattemns and Expressions)은 p153에서 시작되고
표현의 터）
즈트와기능 (Test Expressions and
Func ion사은 p163에서 시작된다．
변환된 데이터는 보여지거나 또는 다른 파일로 저장
된다．
사용자는 XSLT를 모든 종류의 문서를 변환해서
다른 종류의 문서로 만드는데 사용한다. 이것은 접근
하기에는모호한부분이다. 이 책에서는XSLT를
사용해서 XML을 WfML로 변환하는 데 초점을
맞출 것이다. 이것은 작성자의 데이터와 HThII과의
호환성을 사용하게 함으로써 자신의 사이트 방문자
들이 실제로 데이터에 접속할 수 있게 할 것이다．

137

뻐
4
。＝
盼
*요 윅 ＝ ． 乂 콜 르 흥 X 볍 뻐

<xsi:for-each select='subspecies">

하나의 특별한종류의 XSLT 설명서 (xsl:apply
-templates）
는 node의 세트 (node set이라 하는
것이 적당하다）
를 정의하고 이러한 노드가 사용 가능
한 템플릿 중에 가장 알맞은 것을 가지고 연산되어야
하는것을기술한다. 이러한서브템플릿들은다른
서브템플릿 (subtemplate＞을 지정하는 부가의
xsl:apply-templates 설명을 포함할수 있다．
이것은 작성자가 소스 문서의 컨텐츠가 연산되고
결과가 나오는 순서를 조절할 수 있게 한다．

===== PAGE 131 =====
130 =====
XSLT 스타일 시트 시작하기

口

모든 XSLT 스타일 시트는 그 자체 안에서는 XMT
문서이다. 따라서 표준 XML 선언과 함께 시작되어
야 한다. 한번 길에서 벗어나면 반드시 스타일 시트
를 위한 이름공간을 정의해야 한다．

<xsl:sMesheet
xmlns:xsl="http://www.w3.org/1999/XSL/
Transform version="l.O">

XSLT 스타일 시트 시직하기：
1. <?xml version='1.0"?＞을입력한다. 이것은
XSLT 스타일 시트가 XML 문서라는 것은 지시
한다. 자세한 사항은 p24에 나오는KW. 버전
선언하刀를 보면 된다．
2. 다음에 xsl:slylesheet xmlns:xsl="http:
//www.w3.org/1999/XSL/Transform
"version=" 1.0"＞을 입력한다. 이것은스타일
시트에 대한 이름공간을 정하고 이것의 접두어
(xsl）
를 선언한다．
섧 로 m e 三 ＝큽님＝ 口m灌＝ =`em

3. 스타일 시트를만들 빈 공간을 남겨 놓는다（이
장과 뒤에 나올 두 장에 포함될 설명서와 함께）
.
4. </xsl:sMesheet>를입력하여스타일시트를
마감한다．

V Tips
U xsl:stylesheet에는 빈 공간이 없다（이것은
xsl:style sheet가아니다）
. 결국이 책에서
style sheets를 설명하기 위해서는 두 단어를
사용해야한다．
■ 만일 XSLT를 위한 익스플로러 5를 사용하면
아마도 다음 이름공간 선언을 사용해야 한다：
<xsl:stylesheet xmlns:xsl="http://www.
w3.org/TR/WD-xsl">.
■ 이름공간을 선언하는데 더 자세한 사항은 XMl
를 보면 된다．
에서 이름공간사용하7］

l38

C ode.flslt

陋－

Chapter 10

<?xml version= 1.0n ?>

<xsl:st인esheet>
그림忍4 스타일 ㅈ］트의 머랏 부분은 언제나거의 바슷하다．
아 정보를복사와 붙여넣가를통q 아전 스타일 사트에서 다끔으로
넣어갈수 았다．

===== PAGE 132 =====
131 =====
XSLT

"

=__i

凹

루트 템플릿 작성하기

?>

0

(0de.xs1t
version= "

1.

<?xml

！그

<xsl:stylesheet
xmlns:xsl="http://www.w3.org/1999/)(SL/
Transform" version="1.0">
<xsl:template match="/">

XSLT 연산자가 스타일 시트에서 가장 먼저 찾는
것은 XML 문서의 루트 노드에 연산자가 적용할 수
있는 템플릿이다. 템플릿을 루트 템플랏이라고 한다．
루트 템플릿 만들기：

</xsl:template>
</xsl:stylesheel>
그림10.5루트 템플랏은xML 연산자에 의q자동으로 불라는
우일한 템l플랏아다．

1. <xsl:temHate을입력한다．
2. match="/" 을입력한다. 슬래시는XML문서
의 루트 노드에 상응하는 패턴이다．
3. ＞을입력한다．
4. XML문서에 어떤 것이 발생해야하는지를정할
몇 줄을 남긴다 (p140-151에서 다룰 것이다）
.
5. </xsl:template＞을입력하여루트템플릿을
마감한다．

'/ Tips

그림10.6 만일 스타일 ㅈ］트와루트 템플릿의가장〃본적인 깃으로
XML 문저를 연산한다면 빈문저를 얻거7 될 것이다. 이것은 그림
加. 5의 텡플료（）아 말한 것이다. 두 7fl의 빈 줄을 나타내자．

여）제의소스 코드는 www.cookwooLcomofl 있습나다．

■ 만일XML문서의루트노드와상응하는템플릿
을 포함하지 않는다면 고유의 템플릿이 사용될
것인데 이 템플릿은 기본적으로 루트 노드의
자 (child) 노드의 각각을 위한 적당한 템플릿을
찾으려고 할 것이다（이 고유의 루트 템플릿은
<xsl:template><xsl:미：1ply-templates/>
</xd:temF寸ate＞와동일한값이다）
. xsl:
apply-templates에 대한 자세한 사항은
p144에 나오는 템플릿 규칙을 만들고 적용하기
를 참조한다．

139

。m口＝ =．芬m” 。。＝｀크흽口4。

U XSLT 연산자는 이 템플릿이 XSLT 스타일시트
어디에서 나타나는지 신경 쓰지 않는 반면에
가장 상단에 이것을 놓을 경우 작성자에게는
가장 명확한 것이 된다．

===== PAGE 133 =====
132 =====
Chapter 10
HTML 코드 출력하기

羽죠芸若一∼一－莎∼有픈code,esit小

XSLT 스타일 시트에는 기본적으로 두 가지 종류가
있다. 설명과오자 (literal）
이다. XSLT 설명서는
어떻게 소스 XML 문서가 변환되어질 것인지 설명해
준다. 오자들은 - 전형인 HTML 코드와 텍스트 스타일 시트에 그들이 나타난 것 같은 결과이다．

<html><head>ctitle>Endangered
Species </title>.c/head>cbody bgcolor="white '>

루트 요소 안에서는 마지막으로 변환된 문서의 구조
를만든다. HTML 결과를 위해서는마지막부분에
IfI爪4L정보（head, body, etc）
를첨가하려 원할
것이다. 그리고 필요에 따라 광범위한 HTML 포맷
을 또한 첨가할 수 있다．
루트 템플릿이 아닌 템플릿 안에서는 결과물을 설정
하는데 HTML 포맷이 필요로 하는 것 모두를 첨가
할수있다. 그러나html, head, body 요소들은
아닐 것이다.

,

穫七－呼7三루；
日쾨

<xsl:template match="/">

<p>Endangered animals face numerous threats.
For more information, check out the World Wil비ife
Federation's <a
href="http://www.worldwildlife.org/
species/species.cfm?">pagesc/a>.
</p><hr/>c/body></html>
</xsl:template>
그림10.7is]설명서가 아난 것은 아것과 같은 결과가 나올깃이다．
H'1 코당과 텍스트를 첨가하슨 깃은 쉬운 방법이다．／玎孔iL은
찰 콩성돠어야 한다. 예를들연＜p> 태그는 반드사 쑤우하는＜/p>
태그를가져야 하고 <hr>아 아닌 <hr/＞을ㅈ渗했다．

릎驪

,

c'}de.Km1斟쐤뷰美定퓨妾瑾時唯

<htmls.'zhead>
<meta http-equiv=「Content-Type"
content="text,샤tml;d1orset=utf-8">

●경U． 름H工m= =*＝큼＝ 。

결괴묠에 html 코드 첨가하기：

<title>Endangered Species</title></head>

템플릿 규칙 태그 안에서는（다시 말해 <xsl: teinplate match=" . .. ..>와</xsl:template>
사이에서는 특정 템플릿이 불려졌을 때 결과로 보고
싶은 HTML 코드를 첨가해라．

<bod간)gcolor=「white">
<p>Endongered animals face numerous threats.
For more information, check out the World Wildlife
Federation's<a
href="http://wvw.worldwildlife.org/species/species.
cfm?">pages</o>
</p><hr></body></html>
그림10.8 XSLT 연산자（아 경우에는 Saxo파는刀姃L에착접 전달
하치꼿했차만 컨텐츠는 모든工刃孔iL 태스z와 텍즈트와 함聊 나와
있다. 55X0fl0/ 어떻거／<meta> 태＝Z를자동적으로 첨가하는자
주꼭하자. 이것아<html> 태그를보면우라가결과로RTML
코드를 내는 것을 알깃이다. 이것은또한＜hr/＞을 더찰 인자되는
<hr＞로 바꾼다．

140

===== PAGE 134 =====
133 =====
XSLT
■回8

牙 End.nq슨＇eJ Specie$ kicro.oft 1nte1ne EXpIo,e,
트1e

트山t

> .
治＝,,

y w

F立o,

工0d:

b哨〕

.

[：〕 公

自

5mp

Rd,esh

Se미比 FaV여ie5

-Ion.

山

;i
駒LoC穫 ,,ene

그림10.9 이것은브라우저에서 보이슨 깃이다. 아작 훙마로운 단겨7는
아나자만그러한 단계로 나아가는 과정아라고 섕각하자

'/ 1iF隅
■HTML코드가잘정돈되기 위해서는반드시
xfl겨구칙을따라야한다. 그리고 이것이
XHTML（유일한 부가적인 변화는 모든 당신의
요소와속정 이름을 소문자로 쓰는 것이다）
이될
필요는 없지만 이 아이디어는 좋은 생각이다．
XMl겨子칙에 맞게 IfI以4L을 쓰는 것에 대한
정보의 일반적인 사항은 1장 XML 작성법을
참조하고 특별한 사항은 p23에 나오는XML
작성의 규칙을 참조한다. 부록 A에 나오는
XHTML을 참조해도 된다.
■ 상응하는속성이 설명서 안에서는무엇인지
정하지 않겠다. 왜냐하면 어느 템플릿에서나
（단지 루트 템플릿이 아닌）HTML 결과물을
첨가할수 있기 때문이다.
■ 실제적으로 어느 종류의 노드나 이런 방식으로
만들 수 있다. XSL 설명서가 아닌 것은 마지막
문서에 등장하는 결과물이다．

U HTML 작성법에 대해서는 B&B에서 나온 월드
와이드 웹 HTIvIL 4를 보고, 더 자세한 사항은
http://www.cookwood.corn! htm14_4e를
참조한다．

야체의소스코드는www.cookwood.corn에있습나다.

141

。．긍＝ ==．百글尸＾ 。탔

■ 또한xsl:element, xsl:attribute (p151
참：조？그리고 xsl: text를 사용함으로써 요소
들（그리고 속성들과 텍스트）
을 만들 수 있다．

===== PAGE 135 =====
134 =====
Chapter 1 0
노드의 컨텐츠 출력하기
주어진 노드 컨텐츠를 형성할 IfI爪4L 코드를 만들었
다면 당신은 그 컨텐츠（이것의 기호열 값）
의 결과를
보고 싶을 것이다. 노드의 컨텐츠（하나의 요소와
같은）
를 결과물 문서에 첨가하는 가장 간단한 방법은
있는 그대로 그것을 쓰는 것이다．

∼∼굼긷∼一－＝毒目릍
code.emt '
口
<?xml version="1.0" ?>
<endangered_species>
<animal>
<name Ianguage="English">Tiger.c/name>
<name languoge="Lotin">panthera tigris.c/name>
<threats><threohpoachers</threat>

그림10.10 XML 소스 문저의 인용은 아름요소와그것의 컨텐츠를
보여준다．

노드의 컨饅 츨력하기：
1. 필요할경우 컨텐츠를형성할HTML코드를
만든다．
2. <xsl:v이ue-d를입력한다．
3. select="expression" 을 입력한다. expression
자리에는 X Th 문서에서 설정된 노드가 들어
간다. XML문서의 컨텐츠는 여기에서 결과로
나와야 한다.
4. /＞를입력한다.

U
m
·●
｛
。
＝ 。m= m졉으。 。
*＝으＝ 。

'/ nPS
■ ＄이ect="." 를 이용하여 최근노드의 컨텐츠를
출력한다. 더 자세한사항은 11장의 XPath:괘턴
과표현을 참조한다．
■ 만일 표현에 의해 정의된 노드 세트가 하나 이상
일 경우 첫번째 노드의 기호열 값만이 결과가
된다（그림 10.11의 예제）
. 두 개의 노드로 설정
된 하나의 노드는 표현을 만족시키는 두개의
노드가 있기 때문에 발견되는 것이다. 그러나
이러한규칙 때문에 첫번째 것 (tiger）
의 값만이
결과가 된다．
■ 노드 하나의 기호열 값은 일반적으로 그 노드가
포함하고 있는 텍스트이다. 만일 노드가 자 요소
를 가지고 있다면 기호열 값은 이런 자요소들을
포함하고 있는 텍스트를 포함할 것이다.
■ 만일 그 노드의 설정이 비어 있다면 결과물은
없다．

142

c（〕de.ㅐS簒1

<xsl:tempkite mat래＝"/">
<html><heod><title>Endangered Species
</title></heod><body bgcolor="white">
<p>The mighty <xsl:value-of
select="endangered_species/animal/name
[@language='English']"/>faces numerous threats.
For more information, check out the World Wildlife
Federation's <a
href="http://www.worldwildlife.org/
species/species.cfm?">pages</a>.
「／>
</P＞태
</body>
</html>
</xsl:template>
그림＇0；끄 낚험에빠진동물(endangered animals)의속' 甲신에
name 요소의 컨텐츠를포함할 깃아다（이깃은 endangered
species 요소 안의anmal요소 안에 있다. 그라고 아것은 영어로
.
설정되어진 language 족썽을 갖고 았다）

===== PAGE 136 =====
135 =====
XSLT
,codejuml 瓮곳좇盆薨콰三

<html><head>nznieta htfp-equiv="Content-Type"
content="text/html;charset=utf-8">ctitle>
Endangered Speciesc/title></head> <body
bgcolor="white">

</

<p>The mighty Tiger faces numerous threats.
For more information, check out the World Wildlife
Federation's <a href=
"http://www.worldwildlife.org/species/species.cf
m?">pages.c/a>.

P>

＜卜r>.c/body></hm>
그림蚣I2XSLT 연산자가루트 템플릿에 적용될 때 연산차는
모든Jrm吼 아ㄹ7 부분을 처음 결과로 출려할 것아다. 그라고 연산
자가xsl:value-of 요소에가서는 두 개의노드를 가진 노드
제트롤 찾게 된다＝ 영아로 설정되아 았는animal name 꾜소의
컨텐츠. 연산2陪 다음에 이런노드 중의 첫번째값을 결과．
르 내게
된다. 그것은 Tiger아다．

E1e

트a

y屹.,

F:}sonr,

傘sS

U <xsl:value-of> 요소가 컨텐츠를 갖지 않기
때문에 언제나 위와 같이 시작 태그와 마침 태그
를 합칠 수 있다．
■ 만일 표현이 부을 표현식을 평가한다면 결과는
"참” 값과 "거짓" 값이 나올 것이다. 만일 표현이
숫자라면 숫자는 기호열로 바뀔 것이다.
■ 함수를사용하는값을계산하는표현을만들수
있다. 더 자세한사항은 12장의 테스트 표한과
함수를보자．

dop

Q
［〕 〔a
sor, R帥·卄1 Hcm

Q 匹〕

$e카盼， Foon괩8$

。．*겯＝ ＝山。 ＝。｀mmm＾ 。＝*m= m

4그 .
B뇌

■ 일부 익스플로러 버전에서는XSLT 연산자의
select 속정을 요구하지 않는다（이 속성을 잊어
버렸을경우에는최근노드로가정한다）
. 그러나
이것은 공식적으로 요구되는 사항이다．

1l`e n娼hty끄4비 faces numerous threats For more information, check out the
WodJ wa出a Federabon's Pores

그림10.13그리고 결과꿀은 질졔걱으로 소스XMl 문저로부타 나온
input을사우한다. 정확한가눙정아 여가 있다．

예제의소스 코드는 www.cookwood.corn에 있습나다．

143

===== PAGE 137 =====
136 =====
Chapter 10

템플릿 규칙을 만들고 적용하기
템플릿 규칙들은 소스 XML의 특정 부분이 어떻게
결과로 나타나는지를 설명하고 있는 기본단위들이
다. 템플릿 규칙은 세 가지 부분이 있다. : 시작 태그
는 문서에서 어떤 부분에 템플릿이 적용되어야 하는
지를 설명하고, 가운데 부분은 하나의 매치가 발견될
경우 발생되는 일들을 설명하고 있으며 마침 태그는
템플릿을마친다．
템푤릿 규칙 작성하기：
1. <xsl:template으로템플竅干칙을시작한다．

·
내

2. matd1="pattern"을입력한다. pattern은템플
릿이 적용될 수 있는 XML 문서의 부분을 확인
한다. 패턴을설명한신텍스는p154-161에 묘사
되어 있다.

。
m
= ＝口쁜U
,＝
i 으 읕 ㅌ 꾑m＝ 三 믈 ＜

3. ＞을 입력한다
4. 2번에서 패턴과상응하는노드가발견되었을때
발생하는 일들을 정한다. 가능성에 대해서는
이번 장의 나머지 부분에서 다룰 것이다．
5. </xsl:template＞을입력하여 템플릿규칙을
마친다．

'/ 1iPS
.

p139의 루트 템플릿은 루트 노드에 상응하는
패턴을 가진 템플릿에 불과하다．

■ 루트 템플릿만이 자동적으로 호출된다. 다른
템플릿들은 수동적으로 호출해야 한다 (p/45
참조）
. 수동적으로 호출하지 않을 경우 그들은
간단하게 무시되어 버린다．
■ 스타일시트와 템플릿의 순서는 전혀 무관하다．
템플릿이 연산되는 순서를 결정하는 것은
xsl:apply-templates 요소들의 위치나
순서이다．

144

郭·

\

,=,1씻 ` ,

,

code.ㅐsIt 蓼

<xsl:templote match="/">chtml><hecid>
<title>Endangered Species </title>.c/head><body
bgcolor="white">
<xsl:apply-temHates
select="endangered_species/animal"I>
</body></html>
</xsl.template>
<xsl:template match="animal">
<p align="center">
<br/>cfont size="+3">.cxsl:apply-templates
select="name"/></font></p>
<p>The migthty <xsl:value-of
select="name[@Ianguage='English']"/>faces
numerous threats.For more information, check out
the World Wildlife Federation's <a
href="http://www.worldwildlife.org/species/speci
es.cfm?">poges</a>.c/p><hr/>
</xsl:template>
<xsl:template match="name[@language=
'English']"><nobr><b><xsl:value-of select=" "/>:
</b></nobr>c/xsl:template>
<xsl:template match="name[@language=
'Latin']'><nobr>ci><xsl:value-of select=" ."/></i>
</nobr>.c/xsl:template>
그림10.14 이곳의XSLT스타일 사트의 인용 안에는 4가차의 텡플
릿규칙아있다. 루트 템플릿, animal 노드를위한것 , 영어로
language 족징아 설정된 naInec드를 위한것 하나, 라틴어로
language 족성아설정된 naxne5E를위한것하나 . 뒤의세
다．
가치루트 템플릿이 아닌 것들은 반드사 명백古川）호출되어ㅇ棧｝
ㅁ

Code,k$It 률－

回

<xsl:template match="/"><html>chead>
<title>Endangered Species </title></head><body
bgc이or="white">
<xsl:apply-templates
select="endangered_species/animal"/>
</body>.c/html>
</xsl:templote>
<xsl:template match="animal">
<p align="center">
<br/>.cfont size="+3"><xsl;apply-templates
select="name"/></font></p>
그람 10.15 아것은 그림1Q14ll서보아는 것과 같은 스타일 시트의
일부분아다. 하아라이트가쳐진부분은 아것과상웅하는xsl :
apply-templates 속성을 나타내는 부분이다．

===== PAGE 138 =====
137 =====
xsLT
長祗눕븍驀논긍一芚身方一肖賽蠶 .

템플릿 규칙을 만드는 것만으로는 충분하지 않다．
특정 상황에서 역시 템플릿 干칙을 호출해야 한다．
이러한 것이 템플릿에 의해 설명된 변환이 마지막
문서의 어느 부분에서 출력이 되는지를 조절할 수
있는 방법이다．

da小tml

<body bgcolor="white">
<p align='center '><br><font size="+3">
<nobr><b>Tiger: </b>.c/nobr><nobr>
<i>panthero tigris</i></nobr>
</font>

</p>

<p>The mighty Tiger faces numerous threats. For
more information, check out the World Wildlife
Federations <a
href="http://www.worldwildlife.org/species/
species.cfm?">pages.c/a>. </p>
<hr>

템플릿 규칙 적용하기：
1. 템플如칙안에서＜xsl:apply-tem이ates를
입력한다．
2. 필요에따라＄dect="expression"을입력한다．
expression에서는 문서 안에 있는 템플릿이
적용되어야 하는 XML 문서 안의 요소를 정의
해야한다．

.c/

</font>

<p align="center"><br><font size="+3 '>
<nobr><b>Black Rhino: </b>.c/nobr>
<nobr><i>diceros bicornis</i></nobr>

p>

<p>The mighty Black Rhino faces numerous threats.
For more information, check out the World Wildlife
Federation's <a

3. /＞을입력하여 태그를마친다．

口
E* E·
ㅇ．
B出

y1n中 F小eta

.

5m

工여」
｀

印

［〕 公
"

」

H뎨”

自

$ead,

巨〕

"

L〃六

Tiger: panthera tigris
The畔加y Tgec face numerous t eats For more irihsmahon. check out the
wof仰月thfa Feder吐on'a pause

mkLCk klim]o: 繭ceros hicornis
The a甘1￡yBInckFAust faces numerous threats下or more ,nfocmason. check
.ut the World WIdAfa FederahOt出 PAStS

그림蚣l7endangered_species /anima1c드 세트는
animal 노드들둘다(tiger one과Black Rhino one)를포함
하고 있다는 것에주의하자. 따라저p143011았는그림1a13과는
반대로 정보의두 세트는모두 결과꿀하다. animal3드가 연산되
어질 때마다 name 텡플랏들은호출될 것아다（그라고 이것은
위와 같은 맛진타아韶가질 수 았는 방법ㅇ］다）
.

'/ nPS
■ 만일 2번에서 select 속성을 정의하지 않았
다면 연산자는 템플릿을 찾아서 최근 노드의
모든 후계자들에게 각각 적용한다．
■ xsl:apply-templates 요소는각각의
연산되어지는 노드에게 가장 적합한 템플릿
규칙을 찾아서 호출한다. 요소 자신의 표현을
통해서 어떤 노드가 연산되어야 하는지를 요소
가 결정한다. 요소는 또한 템플릿들의 패턴들을
살펴보고 노드 세트 안에 있는 각각의 노드에서
가장 적당한 것을 찾음으로 어떤 템플릿을 사용
할 것인지를 결정하게 된다. 다른 템플릿이 각기
다른 노드에서 사용되는 것은 가능하다．
■ 만일 사용가능한상응하는 템플릿이 없다고
하면 고유 템플릿이 호출될 것이다. 루트나 요소
노드에서 이것의 의미는 모든 자 노드들을
위한적당한템플릿을찾는다는것이다. 텍스트
노드에서 이것은 텍스트가 있는 그대로 출력된
다는 것이다. 속성 노드에서 이것의 의미는 텍스
트로서의 속성을 출력한다는 의미다.
■ xsl : apply-templates 요소는xsl:sort를
포함할수 있다 (p150 참조）
.

예제의소스 코드는 srwv.cookwood corn에 있습나다．

145

。·。＝＝山二＝ ` ＞ 휼 도 금 검 클 으 으 m ” 드m出

.2림10.16 얇은 빨간색은 각각의animal .!rE（이 x姃L 문서에는
두 7/가 았다）
에서 발섕한 것아다, 굵은 글씨체는 name 텡플릿으로
부Ej의 결과이다．

===== PAGE 139 =====
138 =====
Chapter 1 0

배치 연산 노드
또한xsl: for_each 요소는 주어진 세트 안에서
똑같은방식으로모든노드를하나하나 연산한다. 이
것과xsl:apply_templates와의 차이점은 방법
상의 차이일 뿐 결과는 차이가 없다．
배치 연산 모드：
1. 템플朝干칙에서＜xsl:for-ead1＞를입력한다．
2. s이ect= 'expression"을입력한다expression
자리에는 연산될 노드의 세트를 정의한다．
3. 》을입력한다．
4. 어떤 연산이 실행되어야하는지 정한다．
5. </xsl:for-ead`＞를입력한다

二口＝

"`de.1섭引t 료

鷺目릎

<xsl:template match="animal">
<p align="center"><br/><font
size="+3"><xsl:apply-templates select="name"
/></font></p>
<table width=" 100%" border="2">
<tr><th>Subspecies</th><tb>Region</th><th>Number
Lefk/th><th>As Of</쫠h></tr>
<xsl for-each select="subspecies">
<tr><td><xsl:apply-templates
select="name"/></td>
<td><xsl:value-of select="region"/></td>
<td>.cxsl:value-of select="population"/></td>
<td><xsl:vdue-01
select="population/@yeor ' /></td>c/tr>
</xsl:for-each>
</k1비e>
<p>The mighty <xsl:value-of

·
m

그림兀u8 <table>과 이것의 첫번제 부울표현은 xsl: foreach 설명 아전과 마침 태그인 </table> 후에 위차한다슨 깃에
주의하자. xsl: for-each 설명서 안에저는 선택된지트 안의각
각의모든노드에 발섕되는모든 걋들을 설명해아 한다（ㅇ／ 겋우에
.
는 한 animal에 대한각칵의subspecies 0/다）
첫번째 줄에서는 테이블의 攘꼐줄의 첫번째셀이 결과로 출력된 후
name 노드 /J）
트를 연산하고 셀을 닫게 된다．
두번째 줄ofi서는 다른 톄이블 셀을 만들고 테아블 셀 안에 있는
region 노드의 값을 넣고 셀을 닫는다．
세번째 줄은 다른 테아블셀을 만들고 셀안에 았는 population
노드의값을 넣고 셀을 닫는다．
녜번째 줄은 다른 EN이블셀을'! -iZ population 요소의year

七。 ＝m＝ 濂으으륵七* 。m

속성의값을 넣고 셀을 닫는다．
각칵의 줄은 선택되어진노드 세트（여기서는 subspecies) 안에
서각각의노드를 위해서 연산되jZ 있다. 결과적으로 이것은 동물
변종의각칵 구별된 줄을 안든다.

146

===== PAGE 140 =====
139 =====
XSLT
〔丑

三言르菖트＝츨多성료g／二尸！
薑．
<i>panthera tigris</i></nobr></fonh</p>

■ xsl: for-each요소는전형적으로시작과
마침 table 태그가요소의 앞뒤에 있는 것과
함께 RrML 테이블을 만드는 요소이다. 위의
4번에서 설명된 연산의 일부로서 tr과 ts 태그
들도 갖고 있다．

<table wudth="100%"border="2'>
<tr><th>Sudspecies</th>
<th>Region</th>
.cth>Number Left.c/th>
<th>As Of</th></tr>
<tr><td><nobr>.cb>Amur or Siberian: </b>
</nobr><nobr><i>P.t. altaica</i></rsobr></td>
<td>Far East Russia</td>
<fd>445</td>
<td>1999c/td>
</tr>

■ 일반적으로각각노드가발견될때마다반복되
는 干칙 바로 전에 xsl:for-each가 자리
잡는다. 프레임 요소를（테이블과 같은 것）시작
태그와 마침 태그 전후에 각각 넣고 싶을 수도
있다．

<tr><td><nobr><b>Balian: </b>c/nobr>
.cnobr><i>P.t. bolica</i></nobr>c/td>
<td>Bdi</td>
<td>0<가d>
라d>] 937</td>'c/tr>
</table>
<p>The mighty Tiger faces numerous threats. For

Eis

트45

Ye눠

F소soioi

蟲,

1

如lo

"

St。Pl。
p
searP。
et 黑 Ft。。ie。' 岫n

「

J1:

"『445

.

B' ng시
『P4. t:gsss

L1t

,a/,,'
inca Far
: East
Regms
Russia:
505

Joe
,
utopian
India

긔

I

rLaft ' 955
I9_0;

「’

1,

：口．

'

s.

P.

Subopeciet
An。
ur 。t: Sihetuan;
danan「 ’「：" 0a150ra

- ∼P
竺a0.'一:z.∼Soudaka
ㅣ
∼叫
-

= ㅁ.

난e1〕

Tiger: panthera tigris

[如.

I

L ∼1·dS. clot 」Mm:· soft Internet Cii· DuO:

"

' "' " 「’

기59

1999

1999

1 indo-chinc:r, a-.;. Dmblh

hda-Chuns

ITO '

1999

"'

,

"'

I 999

／「

O.

40111…

성oulIs chma

1

India kharuaj

0500y; P. " ,oowsrgs

.

Smoatram, 1-Si. ansstaivae

1

U HTML 테이블이 XSLT 파일의 부분이고 이것
은 반드시 XML의 신텍스 규칙을 따라야 하기
때문에 테이블을 설정할 때는 이러한 규칙을
명심해야 한다. 특별히 모든 시작 태그는 상응
하는 마침 태그를 갖고 있어야 하고 요소들은
중복되어서는안된다는것을기억해야한다. 더
자세한사항은 p23에 나오는XMl 작성의규칙
을참조한다．

Th

e mighty Tiger facet nemoerous threats For more ooformaloon. check en the
rld Wddhfe Prdsnaps。
W。
。4sg

-

Black Rhino: diceros bicornis

毛玉友玉轟露길擢－

｀∼堪耀

95

…

'

螂：
艇戚蝸騙珊

그림10.20 화면에는 가려진 타아틀 밑에 있는 BackRhino에
대한 다른 모든 데a/s7 테아블아 았다．

예젱의소스 코드는 www.cookwo:d（刃m에 있습나다．

147

四요수七떽으。 旦＝ 山＝ 。응m

.2림10.l9xsl; for-each 차지 설명서는최근 animal의
subspecies 각각에 맞는 새로운줄을 근）들었다（주의：공간이
.
한정되어 있가 때문에모든 변종들아 여가에보아는 것은 아나다）
선택된 /J）
트에저치사 설명서가 모든 노드를 연산하였다연 아걋은
나ㅁ杯／ 템플릿 에서도 겨）
속될 것《）
／다 (:
2라고 아 경우에는
</table>아침 태그를 출력한후에꾜사부분을 출력했다）
.
，牙E

V Tips

===== PAGE 141 =====
140 =====
태apte리0

1. 템플릿규칙 안에서＜xd:if를입력한다．
2. test="expression" 을입력한다. expression은
노드세트, 기호열또는숫자를 정한다. 표현을
쓰는 방법에 자세한 사항은 11장의 XPath.괘턴
과표현을참조한다．
3. ＞을입력한다．

5. </xsl:if＞를입력한다．

V Tips
■ 그표현이 진실이라는 것을 어떻게 알수 있을
까？만일 노드 세트가 비어 있지 않다면 그 노드
세트는 진실로 간주된다. 다시 말해 노드 세트는
몇 개의 노드를 포함하고 있다．
■ 만일 표현이 틀렸을 경우, 예를 들어 다른 조건
- 대안의 결과를 정하고자 한다면 xsl:choose
.
를 사용한다 (pi49 참조）
■ 작성자는모든종류의 조건들을테스트할수
있다. 테스트 표현을 만드는 법을 자세하게 알고
싶다면 11장 XPath. 패탄과표현을 참고하자．

<xsl:value-ol select="."I>
<xsl:if test=". =0'>
<font color="red" title="that means there ore no
move Ieft">--&gt;Extinctlk/font>

.2림10.2lpopulation 값을 단준하 출력하는 甲산에 텡플릿을
서는 첫째로 값을 출력한다. 그라고 나서
적용해보자. 템플릿 인띠）
population 값이 0이 돠는자 테스트 해본다. 안일 그렇1다면 JExtinct를 빨간색으로（타아틀과 함 ll) 촘）
가하는q o/
꼭쟉은
흐는
(）
을눈에더찰띄게 하가 위해서아다. 적다는 의미의부등호 가．
반EA/ &g로 써아한다．
ㅁ

:FF；二三立＝-

mdBJ·bn1 幷一李每－ 辯穩m룁

<tr><td><nobr><b>Amur or Siberian: <lb.
</nobr><nobr><i>P.t. altaica</i></nobr></td>
<td>Far East Russia</td>
<td>445</td>
<td>1999</td></tr>
<tr><td><nobr><b>Balian:</b>c/nobr>
<nobr><i>P.t. balica</i></nobr></td>
<td>BaIk/td>
<td>O<f。
nt col。
r="red" title="that means there are
no more Ieft">-->Extinctlk/fonb.</td>
<td>1937</td></tr>
그림10.22 빨간색으로 되어 있는 별도의 텍즈트는population이
0일 때만 첨가된다 C4rnur나siberian 호링까는 445아라나 남하
.
있기 때문에 별도의 텍스트가 팔요 없다）
互 Endanqe,ed Sper.e. - Mio,o.oll 1n1e'1,er Eaplo.e,
E出

트상

恥s.

FV

de如

工=9

［〕 t恪

拓，巨：섰： 晸唾갭

日帥a助

H.re

區그

餓

Seoth Fa,aie1

Tiger: panthera tigris
,

Sokpecieo

。，
`
= = ＝ 。 芝 七 ＝ 。Ume， 。＝m= mmm● 닐

4. 만일 노드가정해지고2번과같이 정해진 기호
열 또는 숫자가 비어 있다면（또는 숫자의 경우
0 값이 아니라면）어떤 결과가 발생할지 정해
준다．

<xsl:template match="population">

Region

-

Number

제한적으로 노드 연산하기：

－三→口
m于＝드느 - =＝三르＝

汗＞

어떤 조건이 충족될 때만 노드나 노드 세트를 연산하
고자하는것은당연한일이다. 조건사항은표현처
럼 쓰여져 있다. 예를들면 만일 특정한 노드 세트가
비어 있지 않거나 노드의 기호값이 특정 단어와 동일
하다면 작성자는 어떤 조치를 취하고 싶을 것이다．

(ode.eslt
口
<td><x寸아)ply-templates
「/></td>
select="population

</xsl:

제한적으로 노드 연산하기

Left

Amuror 51benan P.1. a1taraF ar Esst Ruaua

飇1 ∼J1999

EeJiaoJ2L basbra

t0J二迪共｝
生rL [1937
0二？ ,,坐匹n{192
,여긴＞E s ctii 11950

…

Jovan, 只E쁘쌘뜨
C.spian: P.t. vfrgaa

Beeg.I Pt. ag
赳 D,겨눼

--『 ∼ －…

佃ah
Ir393
-Ca'pian Sea

…

壅쓰竺쁘'螂二：二省 e 님1
簪LmJi*하났
'

그림 加ㄴ23 만일population아 0이라면 별도의 텍스트（그라고
타이틀 속성）
는 정보가 명확ㅎ］
보아겨］하가 위해저 첨가될 것아다．

148

===== PAGE 142 =====
141 =====
XSLT
c1,de.HSIt
.1
<x5 :template match="populaion">
<xs :choose>
<xs :when test=' . =0'>
<font color="red" title="that means there are
no more left">Extinct</bnt>
</xsl:when>

·룔

;＝三흴ㅌ 뻑 ＝二1- r∼ ㄷ：==｀三：
긷汐

지난 페이지에서 설명되었던 xsl:if 지시 설명은
단지 하나의 조건과 하나의 결과 행동만을 허용한다．
xsl:choose는 여러 다른 상황을 테스트하기를
원할 때 그리고 가장 일치한 반응을 얻고자 할 때
사용할수있다．

<xsl:when test=". &gt; 0 and . &lt; 50">
<font title="they're almost gone"><xsl:value
J$dect="."/></bnt>
</xsl:when>

조건적인 선택권 첨가하기：

<xsl:otherwae>
<xsl:value-ohdect="."/>
</xsl:otherwise></xsl:choose>
</xsl:template>

1. 템플릿규칙에저 <xsl:dioose＞를입력한다．
2. <xsl:岫en을입력하여 처음조건을시작한다．

그림10.24 밴枉SLT 연산자는population아 0인차 아닌자
가장 먼저점검해 본다. 만일 그렇다면 아것은 폐ㅈ］돠었다는 결과로
나올깃아다. 만일population아 0아 아나면 연산자는 이것ㅇ／
0보다 크고 50보다 쟉은지를 체크하ijJ 된다. 그라고 만일 그렇다연
값주변에경고성의툴팁을촘）
가한다. 다른경우에는 단준하값만을
출력한다．
code.htnI

6. </xsl:when＞을입력한다．
7, 각각의 조건에 2- 6번을 반복한다．

그림10.25 ㅇ／작은 인용에저는 당신은 값 다음에Extinct를 첨가
하는 甲신叩 (148p에그림刃L22처럼9 population아 0일 때
단又/ Extinct라는 단어를 출력한다．

E出

됴出

Vv,

F且v아1m

<P .

0

s1여）

.出

目伺勵

Iod1 ㅂa

[：〕 〔f玉

R하．
e컨｀
+,

H야1比

Seach 陌c.dc;

Reg.en

'/ nP

ㅣNumber L「ft 」＼` O「

Arnur or Sibeoo. P.t. c,Jkthra 區프 uso1乙阡
Uoiirn, P.t. bu&O
__a_
뇨____
Java,,: Ft. sondaica
Java
- :

고999
匣희
r回
隔띠

CocpiaO: Pt. vwg.ota

Icaspum Sea

- \

5regat: Pt. agna

뇨경‘a

`159

Isumatraic P.c um000ra.

jInda,BingJadesh 』o0

n5§§ㄱ

巨aeytP.Lavoyer,as

Saudi Sotia

1999

匡和

,'

만일 xsl:when 요소들에 의해 정해진 조건 중
아무것도 진실이 아니라면 어떤 발생 결과를
얻게 되는지를 정하라．
9. </xsl:d'oose＞를입력한다.

Tiger: pan楙era tigris
S沚cperiee

8. 필요에따라<xsl:otherwise＞를입력한다.

</xd:otherwise＞를 입력한다．

l견그

礪且

4. ＞을 입력하여 xsl:when 요소를 마감한다．
5. 만일 3번에서 테스트된노드세트, 기호열, 숫자
등이 비어 있지 않다면（또는 숫자의 경우에 0과
같거나）발생해야 하는 연산을 정한다．

래

<tr><td><nobr>cb>Balian: </b></nobr>
<nobr><i>P.t balica</i></nobrv</td>
<td>B이i</td>
<td><font color="red" title="that means there are
no more left">Extinct</font></td>
<td>1937.</td></tr>

牙 rnI..av,ed Spvc,e. - Mic,o,nlt Int,,neI E.pla.o.

3. test="expression" 을입력한다. expression
자리에는 노드 세트 기호열 또는 숫자를 정하는
것을넣는다. 11장Xpath. 패턴과표현에서
표현을 쓰는 법에 대한 상세한 사항을 보기로
한다．

■ 발견된 첫번째 진실 조건 안에 포함된 활동이
실행될 것이다. 다음에 나오는 조건들은 무시
된다．

1999

r－∼葫Lota .hote

;

.2림10.26 여가에는population의 값에 따라 세 걔의 행동아
았다. 여가서는population 값아 叫우적은곳을강조하가
위해저 툴팁을 첨가했다．

예제의소스 코드는 www.cookwood.corn에 았습나다．

149

夔드＝ .＾。＝드＝ 。
＝
。 9
。＝
g

灌巨＝ 」

조건적인 선택권 첨가하기

===== PAGE 143 =====
142 =====
Chapter 10

연산하기 전에 노드 분류하기

一

code.1oit

郵工

디폴트 값일 때는 노드가 문서에 나타난 순서대로
연산된다. 다른순서대로 연산을 하고 싶다면 xsl:
sortㅍ 요소를 xsl; apply-templates 또는 xsl:
for-each 요소에 첨가하면 된다．

<xsl:sort select="population"
data-type="number"I>

연신하기 전에 노드 분큐하기：

<xsl:sort select="populaton/@year"
data-type="number"/>

t

xsl; apply-templates, xsl:for-each
혹은 또 다른xsl:sort 요소 바로 다음에
<xsl:sort를 입력한다．

2. $dect="criteria"를입력한다. criteria자리에
는 연산된 노드 중에서 어떤 노드가 분류되는지
를 정하는 표현이 오게 된다．

二a

<table width=' 100%" border="2">
<tr><th>Subspedes</th><th>Region</th><th>Nu
mber Lefk/th><th>As Of</th></tr>
<xsl:for-each select="subspecies">

<tr>uztd>uzxsl:apply-templates
select="name"/></td>
.2람10.27 XSLT스타일ㅈ］트의 맨 위에서 하강과상승두 개의
xsl : sort 차사 명령저를xsl : for-each 꾜소 후에 2ㄹ/1Z
결과가 나오7] 전에청가한다．

壞巨 3

-

de力mn 絿一一李一攀拉宰啣＝月득
디）

:

<table width=" 100%" border="2">

4. 분류하고자하는것에 따라data·type=htexth1
또는d이a·竗pe=hmnumber" 를 입력한다．

<tr><td><nobr><b>Balian: </b></nobr>
<nobr><i>P.t balica.t/i></nobr>uz/td>
<td>Bah<가d>
<td>uzfont colar="red" title="that means there are
no more left">Extinct</font></td>
<td>1937</td>

.sztr><th>Subspecies</th><th>Region</th>
<th>Number Left</th>.tth>As Of</th></tr>

5. /＞을입력하여xsl= sort 요소를마친다．
6. 원하는만큼의 많은키를정하기 위해서 1-5번
을반복한다．
'a, n '`
■4번에서 정확한데이터 형식을정하는것을
명심하자. 텍스트가100, 7, 89와같은에러
결과를 가지고 있는 것 같이 숫자를 분류한다．
텍스트에서 숫자를분류하는 것은 100, 7, 89와
같은 에러의 결과가 나타난다. 숫자에서 텍스트
를 분류하는 것 역시 효과적이지 않다．
■ 하강의 의미는높은숫자에서 낮은 숫자로 z에
서 A로 간다는 의미다. 상승의 의미는 적은 숫자
（그리고 글자）
가 위에 나타난다는 의미다．

그림如L羽 여가서슨Bail t』
ger 끼；장 먼저 멸종된호랑이）
는 가장
먼저 연산되어치고 테아블의가장 위叩 나타날것아다，
牙〔edangeied Soe.1o, Meie,toll kaei,,es EX1l1mer
'

E* 트as

y"1' Fvoc5e, 拗li he누

! <> .

.

BSd,

［〕 凸

닭야） R甘,o功

H여，
陷

曦

ㅌ그

5edct, Favt겡ie$

Tiger: panthera ngris
Suh. er` s

和giPn

I

끄aliatt Pt. hu錟？a

田汕

S. s'asgata
catpistt. 尸．

r뇨∼눼n Sea

INumbor Loft飇石?

Javan: f '.S. ate* sura
my= P.S. aewyoums

a
匕Ut, 뇨．

Samatean: P.S suuml,mo

괘J

ndsa, Ban字adesb 40()

Amur CrSiborrnn, 尸．
t. 砥ak:nFarEoat Russia

445

a汐s

Ind伊d.ine`e: JnL, cu小ott

12z7

크995

!Bengalj노酋g，
了i

뇨d.'c뇨m
IJndia

m
＝ 云 ● 날。 ，｀●，。*●mm● 경 ＝ m
= ＝느● m

3, 필요하다면
（)rder="descending" 을입력한다．
디폴트 값은 오름순서로 분류하는 열쇠가 된다．

3159

'

Thu r咬yTi er faces awnecous fr ene. For mote Sbzmatkn, check out出. ＝」
區L여力．
*轍

拒J Ste.

그림10.29세계의호랑이를처음에는7柄］순저대로, 두번째는
멸종된 연도수 대로 라스트했다 씨테이블은 쟐4의 더）아E7를 포함
하고 있고 전저）
겨γ 야생 호랑이를 나타낸다는 점에 주의／.

150

===== PAGE 144 =====
143 =====
XSLT
飾目－----1---------

속성 생성하기

tode .Hslt

<xsl:template match="picture">

속성을（그 값을）주어진 요소에 첨가할 수 있다는
것은 때때로 유용하다．

<img>
<xsl:attribute name="src"><xsl:volue-of
select="./@filename"/>c/xsl:attribute>
<xsl:attribute name="widfh"><xsl:volue-of
select="./@x"/></xsl:attribute>
<xsl:attribute name="height"><xsl:value-of
5히ect="./@y"/></xsl:ottribute>

속성 생성하기：

</img>

1. 새로운속성이 나타나는요소의 시작태그바로
다음에 <xd:attribute를 입력한다．

</xsl:template>
그람10.30 여가서는그림요소를표준HTML imp 태＝z로 변환
鞭／는 템플릿을 만들었다. /@fi1ename 표현의의ㅁ／는 촤근 노드
의 filename 족성을선텍하라는것이다. 아경우picture

3. ＞을입력한다．

node) 자세한사항은β石
（）
에 나오는노드의족성 선택하가를
보자．

4. 새로운속성 값을입력하거나출력한다．

i」

「十＝꿈Code力tnH

二］

<body bgcolor="white">
<img src="tger.jpg" width="200" height=" 197">
<nobr><b>Tiger: </b></nobr>
그랖10.31완벽하게유효한HThIL img 태그이다．
目r日．

j I nd,,.qe,.d So.C. . - Micro. 4L Ine,neI E,.oIi1rer
y. .

F-o,e父

t

E

a

be幻

仝

J

Slop

R너r.卄1

■ 주문형 이미지 요소들을 표준 HTML hag 태그
로 변환하는 것은 좋은 방법이다

出｀ r
L．

Ho,r,e

Tiger: panthera tigris
%h'pscies

4

Reeau

NwoberLpft

B,lion: P.L 占a&a 如
Cas91007 P4. wrgata

陸｀
caBplal Exa

1Exnt
`E油not

19刃

Javan 只L 5口edthca

JaVa

二 착：

]972

l950

c
《，
맬·鷺 c이1Ynㄼdㅎlot- ,四叫h ll" a e히ed *en4

그람 10.32 위엄이 있는 호랑이그림은 요구되이진 대로 나왔다．

혀）겨7의소스 코드는 www.cookwooci.corn에 있습나다．

151

g ＝ 멱。 ＝＝口＞ =＝口＝ 4
m
m

■ 자신의 XML 문서에 있는 컨텐츠의 속성값을
생성하기 위해서 4번의 xsl :value-of 요소
를 사용할수 있다．

<br>4ont size="+3">

트O

5. 마지막으로＜/xsl:attribute＞를입력한다．

V nPS

<p align="center">

日e

2. name="att_name＂을입력한다. att name
자리에는 요소 안에서 속정이 갖고 있는 이름을
입력한다．

===== PAGE 145 =====
144 =====
XPATH: PATTERNS
AND EXPRESSIONS
XPath: 패턴과 표현

XSLT에서는 문서에서 정보를 변환하기 위해 템플
릿을만들고 적용하는 법을 배웠다. 실제로 템플릿을
적용할 때 노드 세트가 모든 적합한 템플릿（복수의
의미）
에 의해서 연산될 수 있고 단순히 주어진 템플
릿만으로 실행하는 것은 아니라는 것을 기억하는
것이 중요하다. 다시 말하면 템플릿이 그 노드에 잘
맞기만한다면 모든name 노드가 연산된다. 그러나
nameLlanguage='EnglishU템플릿이 생략되어도
된다는 의미는 아니다. 그것은 미묘하게 보이지만
바로 그 차이가 중요한 것이다．

153

m
．

이 장에서는 더 자세하게 설명될 XML 문서 안에서
노드 세트의 위치를 정함으로 그것을 설명하는 시스
템인 XPath신텍스를 이용하여 패턴과 표현을 쓸 수
있다. 패턴과표현의 가장큰차이점은 전자의 것은
기본척으로문맥이 없는 것, 다시 말해 ''name＂같은
패턴이 위치와는 상관없이 XML 문서에서 name
요소와상응하는 것을 의미한다. 표현이라는 것은
그와는 달리 표현이 등장하는 문맥을 통해서 그 가치
를 인정받을수 있는 것이다. "name＂과같은 표현
은 이것이 어디에서 사용되었는지에 따라 단순히
subspecies 요소 안에서 name 노드를 설명할뿐
이다．

츰 힁 ＝ ，。＝멱＝ m
。 뢴mX격g驪。

작성자는 템플릿을 만들 때 템플릿이 적용할 수 있는
노드를 정의하는 패턴을 사용한다. 또한 템플릿
(xsl:apply-templates）
을호출했을 때 연산되
어야 하는 적당한 템플릿으로 노드 세트를 정하는
표현을사용해야한다. 또한주어진노드세트를
고립시키고 연산하기 위해서 다른 XSL 지시 명령
안에서 표현을 사용할 수 있다．

===== PAGE 146 =====
145 =====
Chapter 11
커런트 노드 지정하기

D
c《｝de.H＄뺨t ; =
<?xml version=' 1.0∥?>

XSLT 연산기는 스타일 시트나 문서를 처리할 때
한 번에 한노드씩 처리한다. 커런트 노드, 다시 말해
연산기가 현재 작업하고 있는 노드에 관해서 다음에
연산될 것이 무엇인가를 정하는 것은 일반적으로
가장수월한 지정 방법이다. 물론 이것을 정하기 전
에 커런트 노드를 정하는 방법을 먼저 알아야 할 것
이다．

<xsl:stylesheet xmlns:xsl="http://www.w3.org/
1999/XSL/Transform"version="1.0">

커런트 노드 정하기：
1. 디폴트값에 의하면 커런트노드는현재사용되
고 있는 템플릿에 의해 정해진 것이다. 다시
말해 커런트 노드는 템플릿의 상응하는 속성
내에서 정해진다는 것이다．

·경＝ *
＝
쁜
， 。Uef驪灌＝ i
，●
*
●
。

2, 만일xsl:apply-templates 지시 설명이
있다면 사용되고 있는 노드는 상응하는 템플릿
（따라서 xsl:apply-templates 지시 설명에
의해 정해진）
에 의해 짝지어진 것이 된다. 그같
은xsl:apply-templates 지시 설명으로부
터 돌아 왔을 때 커런트 노드는 예전 템플릿과
상응하는 속성으로 돌아가게 된다．
3. 만일xsl: for-each 지시 설명이 있다면
커런트 노드는xsl:for-each의 선택 값에
의해 정해진 것으로 변환된다. xsl: for-each
지시 설명 후에는 커런트 노드는 지시 설명이
연산되기 전에 무엇이었던건 간에 상관없이
변환되기 전의 것으로 돌아가게 된다．

'/ 1ip
■xsl:apply-templates 지시는한 개 이상의
노드를순서대로 연산한 것이다. 연산되는 각각
의 노드는 교대로 통용되고 있는 노드가 될 것
이다．

154

m릎

<xsl:template match="/"> (1)
<html><head><title>Eridan5red Species
</title></head><body bgcolor="white">
<xsl:apply=templates (j=,
select="endangered_s$ ies/animal"/>
</body>.c/htrnl></xsl:tem이ate>
<xsl:template

match="animal ">

⑦

<p align="center">
<br/>cfont size="+3">cxsl:apply-tempIate廷9J
select="name"/></font>.c/p>
<table width=" 100%"border="2">
<tr>.cth>Subspecies</th><th>Region</th><th>Nu
mber Left.c/th><th>As Ok/th></tr>

<xsl:for-each select="subspecies"洹9
<xsl:sort select="populotion" datatype="number"/>

그랖lu i번ㅈ］점에서 커런트 노드는／
（루트 노드？ 템플랏에 의해
징해진 것과 같다. 연산자가Ia 자점이）도착할 경우（결국2번 자점）
커런트 노드는endangered_species 요소 안에포함되어
있는 첫번째 animal꾜소가된다. 처음 animal. 소가 연산
되어진후두번째 animal 요소가커런트노드가되고모든
animall 가 연산될 때까차 (.2리.11통용되고 있는노드의준서
를 다 받을 때까지）이깃은 겨7족된다．
加 자점에저는 연산되고 있는 animal 요소안의 첫번째 name
요소가커런트요소가된다. 다끔으로 name 텡플릿을사작하갱
된다 (3번 자점아 될 수 있다. 그러나 아것은 보아차는 않고 그곳에
있는 자사 명령을 따른다. 그라고 나저 두번째 name요소를 연산
하겨］
되고 이러한 방식으로 진행된다7.
2a 지점에서 직용된 name 템플릿으로부F7 돌아온 후 커런트
노드는2b 자점xsl : for-each 지사 명령에도달하기까치 한 번
더animal꾜소가 된다. 아 사점에저 통용되.2 있는노드는 통용
되ㅇ7지는animal 노드 안에서 첫 subspecies. 소가 된다．
다음에 두번째 subspecies.9소가 연산되며모두 끝날 때까차
아 과정ㅇ］
반복된다.

===== PAGE 147 =====
146 =====
XPath: Patterns and Expressions
t()de.H引t 呼

＝甕－

뜁勇

<xsl:template match="animal">
<p align="center">
<br/><font size="+3"><xsl:apply-templates
select="name"/>c/font>.c/p>

커런트 노드의 설명
만일 선택 속성 안에서 사용하고 싶은 노드를 연산하
고 있다면 노드의 바로가기를 사용하는 편이 루트의
모든 위치를 설명하는 것보다는 훨씬 쉬울 것이다．

</xsl:template>

커런트 노드 설명하기

<xsl:template
match="name(@language='English']">
<nobr><b>.rxsl:value-of select="."/>:
</b>c/nobr>

1. 마침표（.）를입력한다（마침표하나이다）
.

</xsl:template>

■ 언제나노드세트의 전쳬를선택하는것을원하
는사용자는 없을 것이다. 커런트노드의 부분
집합을 얻기 위해서는 서술부라고 불리는
테스트를 첨가할 수 있다. 더 자세한 사항은
p161에 나와 있는 부분 집합 선택하기를 참조．

.2림끄2통용되는노드는language 속성이 영어인 name
꾜소의 컨텐츠가될 것이다. 변환과정혀］
서우리가 어다에 있는가에
따라 name 요소가 결정된다．

1 c de.ht1ㅜn

■ .은문맥 노드를설명하는부분집합에서 사용할
.
수 있다（부분 집합에 의해 시험되는 노드）

,.*.,==．呻。 4'. ^.,,0= * ＝ 。 뭏

<body bgcolor="whife">
<p align="center"><br/>4oat size="+3">
<nobr><b>Tiger: </b></nobr><nobr>
<i>panthera tigris</i></nobr></fons></p>
<table width="100%" border="2">

V Tips

<tr><th>Subspecies</th><th>Region</th>
<th>Number Left</th><th>As Ok/th></tr>
<tr><td><nobr><b>Balian: </b></nobr>
<nobr><i>P.t. balica</i>.'z/nobr></td>
.2람끄3 첫번째로 중요 표ㅈ／되어 았는 것들 ⑦ger와panthera
tigris) animal 템플랏의 처음아저 name 템플랏을 적용할 때
나타난다. 디끔결과물은 name 템플릿을xsl= for-each 치시
명령으로부ej subspecies요소이）대해서 작업할 때와 같이
호출할 때 나타난다. 따라서 커런트 노드는 각각 subspecies
요소（여기저는B砒fan과／사 ba批5) 안에서 각각의 name요소가
돤다．

여）群의소스 코드는 www.cookwaxt corn에 있습나다．

155

===== PAGE 148 =====
147 =====
Chapter 11

노드의 자（아，
iId) 선택하기
만일 커런트 노드가 실제로 선택하고자 하는 요소
（노드의 자）
를 포함한다면 루트에서 비롯하는 완전한
경로 대신에 그 이름을 사용함으로써 원하는 자 노드
를 선택할 수 있을 것이다．
노드의 자 얻기：
1. 커런트노드가무엇인지 알고있고 (p154참조夕
관심을 갖고 있는 노드 세트가 바로 커런트 노드
의 자（혹은 후손）
라는 것을 명심해라．
2. child를입력한다. d宙d자리에는커런트노드
에 의해 설명된 요소 안에 포함된 요소의 이름이
들어간다．
3. 필요하다면／grandd1ild를입력할수있다．
grandchild 자리에는 2번에서 설명된 자 (child)
세트 안에 포함되는 노드 세트가 들어가게 된다．
이것의 목적은 계급 체계를 더 자세히 설명하거
나 노드 세트를 더 자세히 설명하기 위함이다．

늬

code.HmI 墟珏－ -＝쵱∼拿츤르重三每華1i을

<subspecies>
<name>Amur or Siberian</name>
<region>Far East Russia</region>
<weight>500 pounds</weight>
<Iength>3 yards from nose to toik/length>
<current_population yeor="1999">450
</current_population>
<threato.poachers</threat>
<threat>habitat destructiona/threat>
<threat>trade in tiaer bones for traditional
Chinese medicine (TCM)</threat>
닐

c/subspecies>
그림끄'4 여가에는XML 문서의 인용아 들어 있다. ㅇ／ 별종요소는
8개의자요소들을 가자고 았다．
co4e.H針
,.
<xsl:for-eac卜 Sdect="subspecies '>

<xsl:sort select=「population" datatype="number"/>
<xsl:sort select="population/@year"datatype="number"/>

＝ ● ， 경 도 닐 견 · 七。 ＝ 。 m 灌 ＝ 으 ● 너

4. 원하는레벨이 될 때까지 3번을반복한다.

<tr>.ctd><xsl:apply-templates
select=''name"/>'c/td>

'/ nPS

<td>.cxsl:value-of select=「region"/>c/td>

■ 물론 자에 대해 의문을 갖기 전에 커런트 노드가
무엇인지를 아는 것이 더 중요하다. 세부 사항은
p154를보자．

<td><xsl:apply-template
select="population"/>c/td>

■ * 를 입력하여 모든 노드 자를 선택할 수 있다．
■ 이 과정을잘하기 위해서는반드시 ./child를
사용해야한다. c卜∥d는 더욱 간단하고 정확하게
동등한 것이므로 그것을 사용함에 있어서 주저
하지말자．

]56

<td>.cxsl:value-of
그림끄．
5 우라가 for-each에도달할 때 변종은 커런트 노드가
된다. 첫번째xsl:sort 지지 명령 안으斥elect 족성은 연산
되고 밌는 변종의 2든 자요소인 2든population Jc5를 선택
한다. apply-templates 지사 명령 안의select속성은
subspecies 요조의자들인 2든 name 노드를찾는다．

===== PAGE 149 =====
148 =====
XPath: Patterns and Expressions

노드의 부모LF 형제 (sibling) 찾기

곧· 聿髥듣三竇좋具立컫立圭孑cedeJsmI

<animal>

만일 커런트 노드와 원하는 노드의 관계가 명확하다
면 숏컷을 사용하는 것이, 루트부터 시작하는 모든，
절대 관계를 전부 쓰는 것보다 훨씬 수월하다．

<name language= 'English">Tiger</name>
<name language="Latin">panthera
tigrisc/name>
＜小re아5>
＜出reat>poachers</threat>
하｀re《그ㅎ
놔1아小아 destruction</十reat>
<threat>trade in tiger bones for
traditional Chinese medicine
(TCM}</threot>
c/threats>
<weight>500 pounds</weigth>

노드의 부모 선택하기：
1. 커런트노드가무엇인지 그리고관심있는노드
가 커런트 노드의 부모（혹은 조상）
라는 것을
알고 있다는 것을 명심하자．

그림끄6 threats와name 요소는 둘 다anima1요소안의
（바로 포함되어 았는J 자요소들아다. 따라서 아깃들은 형제들아다．

. 이것은노드의
2. .. 을 입력한다（마침표두개）
부모를 선택하기 위함이다．

쵭．
昏

노드의 형제 찾기：

--= code.HSII

<xsl:tem이ate match='小reats">

1, 위의 2번에서노드의부모에도달한후／SI비in9
을 입력한다. sibling은 원하는노드（통용 노드
가 아닌 통용 노드 안에 포함되어 있는 것이다）
이다．

＜이>The mig卜盼 <xsl:v히ue-하
select="../namef@Ianauaae='Enalish']"/>faces
numerous mreats: <xsl:ror-eacn select="tnrear>
<li>ezxsl:value-of select=" ."/>＜川＞

그림끄70/ 새로운threats 템플릿을적용할때threats는
커런트 노드가 될 것아다. 만일name 요소（이것은 이것의 형졔｝
를
모요소
설명하려고한다면 .. 룰한단겨）위의레벨로올라는데（부．
animal夕사용되어야 한다. 그 다읍에／을사우함으로써 다른
자를 얻거）돨 깃아고 어딴 자인자를 정하는name을 사용한다．
}Endangesed Speni亡｀ Miss's.이th낚coinS (川Inie.
F호noVer

目回口

■

be轎

1000

V's,

4」 .

的 ［〕 緇

蝨

5mr〕

Sees하， Fm's甘68

Pr.

ees al。
shieene,
P.
c rrgit's coiWits
.

Th

e zesh,ty To,o-r
p。
achers

faces

隘o-

b

B00k

I

5,

Eo

Rci',針， H00e

-

1ni-

□

"

;;;;

h,na

1999

"

걍

numerous teats

1 habitat d'ssuastsosn

2. 필요할경우／niece를입력한다. niece자리에
는 커런트 노드의 형제의 자 (child) 노드가 들어
간다．
3. 필요한만큼2번을반복한다．

卜／ nPS
■ .．은가끔부모노드（../@name）
의속정을
찾기 위해서 속성 축과 합쳐진다. 더 자세한
사항은 p160에 나와있다．
■ 당신은path 안에서의 와일드카드로서 별표를
사용할수 있다. 예를들면 /s/nephew는 통용
노드의 모든 형제의 조카요소를 선택할 것이다．

-

tresde as bgoi bones lbr tradibonal Chinese medicine (1CM)
For snore ,rsfosenatios,, check onit the World Wildlife Federahoson cigeel

V

I

I

1% I

I

'` nwii i-cHina: aiceros 01cαrn's

也

웝 Lood 00,'soi,

--

ㅣ
ㅣ

-

-

-

-

-

-

-

.

-

＝」

.2림끄8문맥아 변했음에도 불구하고（현재는animal 템플릿
안에 았는 깃이아나고 threats 텡플릿 안에 있다＞새로운 관계
룰정한다면적당한결과값아 나온다. 여기서는각칵threats의
보가 좋은포맷을추가하섰다．

예제의소스 코드슨 www.cookwood.com에 았습나다．

157

m응主＝ ．。＝。뭏늑盼， 。，.=*。4닉뜨言m

</xsl:Ior-each></ul>
For more information, check out the world Wildlife

===== PAGE 150 =====
149 =====
Chapter 11

모든 후손 선택하기
더블 슬래시는 특정 노드의 모든 후손들을 선택하는
것이 필요할 때 사용하는 것이 좋다. 다른 기호들과
마찬가지로 이것을 절대 path 혹은상대 path 모두
에 사용할 수 있다．
쿠트 노드의 모든 후손 선택하기：
/／을 입력한다（이것은 두개의 슬래시이다）
.
커런트 노드의 모든 후손 선택하기：
./／을 입력한다（마침표 후의 두 개의 슬래시）
.

풀全숟…＝졀辛즌旺目

Code.onti

<animal>
<name language="English">Tiger</name>
<name language="Latin">pantliera tigrisc/name>
<thre아5>
<subspecies>
<name language="English'>Amur or
Siberian</name>
<name language="Latin">P.t. altaica</name>
<region>Far East Russia</region>
<population year=" 1999">445</population>
.2림끄，
9 animal요소에 name 요소들이 았고 subspecies
요소 안에 name 요소들이 았다．

노드의 모든 후손 선택하기：
1, 관심있는자손을가진노드를 얻기 위해서 이전
장에서 습득한 기술을 사용하자．
2. 그리고／／을입력한다．
노드의 후손의 일부 선택하기：
=＝。겯● Vm음● 츱* 。 -<m= =V으● 내

1, 이전 페이지에 묘사된방법을이용해관심이 있
는 후손을 가진 노드로 향하는 path를 만든다．
2. /／을입력한다.
3. 관심있는후손요소의 이름을입력한다．

code.nslt , , ` `

팔1

, ,`, \

陋릎

<body bgcolor="white">
<xsl:apply-templates select="//name"/>
</body></html>.c/xsl:template>
<xsl:templ아es
match="name[@language='English']">
<br/><nobr><b><xsl:value-of select=".7>:
</b></nobr>
그림1u0 빨간색으로 표사된 select 속성은 name 요소들아
소스 문서에 어다 았든자 name 요소의모든 깃에상응한다떠
확실하게 만들가 위해저 animal 템플릿을 완전하 제거했고 영어
name 템플릿에 <br/＞을첨가하였다).

'/ nP
■ 마지막 기술은문서 안에 노드가 어디 있는지
모를 때 노드에 도달하는데 아주 좋은 방법이다．
//name과 같은 표현은 이름 요소들이 어디
있든지 모든 요소를 출력한다（그림 11.끄）
.

a
Fk

트d'

yes,

F크Votos
st卯

Itd$

ㅂ텨〕

Rdre`h

H삼叱

Ssac's F.ooste,

Ut.

hger= 1Li.:.0.'42
Aln11r .r Sib..iaJ1r ／긴I. othtoes.o
Ba五al`: P.L bα／'Cα
Javan: F길￡．요？月m그』Cα
caspian= 尸.0.
BeugaL ?.o. ttgoss
駐natran: f.t. sismatra,
Amoy: P.t. ainoyensts
Iodo- Ntoots, Pt. ,,,沁iui
mark 1t뇨ins: threrosb,cosms
加ud1ent l기ack Pl山1m ZㅗZL 〃麗川口r
知tsihwestern!칸그＇k Rhhtlr D心．
b,co,ms
Eastern Blask Rl山l`,: D.b. ,,nc月uk
Northwestent P1ad
《 P 山m 즈누i ㅊ'ttpes
우1 Dnn.

h也 二긷

그림II.끄 모든 name 요소들은（영어와 라틴어？animal
에포함되어 있다는 깃을주의하고
(tiger, Black Rhino 두등）
subspecies (amui, Balian, Southern BlaackRhino 두등州］
포함된 name 요소들은 여가에보아는 것아다．

158

===== PAGE 151 =====
150 =====
XPath: Patterns and Expressions
커런트 노드 무시하기

이，
de.Hs1t∼

<xsl:temF놔아e matd1=「anim히”>
<p align="center">
<br/><font size="+3">.cxsl:apply-templates
select="name" /></font>.c/p>
<table wldth=" 100%" border="2">

이제껏 만들었던 모든 패턴과 표현들은 통용 노드에
종속되어있다. 예를 들면 animal 템플릿에서 name
을 선택하는 것은 연산되고 있는 커런트 animal
요소 안에 있는name 요소의 외부와상응된다. 원하
는 노드로 가는 길을 루트로부터 오는 모든 길로 써
주는 것으로 통용 노드를 무시할수 있다．

<tr><th>Subspecies</th><th>Region</th><th>Nu
mber Lefk/th><th>As Ofoz/th></tr>
<xsl:for-each select="/endongered_species/
animal/subspecies">
<xsl;sort select="population" data-lype=
-7림끄l2animal 템플릿으로 돌아가보면 여기서는 루me부터
바롯돤subspecies 노드 저）
트로의 path룰 적아 놓았다．
口
l)de.}1 1
<tr>.ctd><nobr><b>Javan: </b></nobr>
<nobr>ci>P.t. sondaica</i>.c/nobr></td>
<td>Java</td>
<td><font color="red" title="that means there are no
more left">Extinct.az/tont></td>
<td>1972</td></tr>

3. ／로서 문서의 서열 구조에서 한단계 낮은 레벨
로 이동한다는 것을 표시해 준다．

Vee

t:e:,r,

客，

臼
skO

.

J.ooe

t各

Rehed,

Home

Q

6. ／이ement를입력한다. element자리에는상응
시키고자 하는 요소의 이름이 들어간다．

,

He놉

[:)

5. 관심있는요소의 모든조상을정의할때까지 34번을 반복한다．

ㅌ그

se첩이，Favulto

l

ㄲger: pca倂2era tigris
l

Subspecies

Regime

漣뺑&n:P.1. 6 by : －… 區i
뚜Cmupso,o P.1. Vea1.v
［으 Op,00Sea

'/ 1iPS

Nu漱1er
l Left

lJaume, P.1. s7vio,,.,

Tavt -

=:：닙＂·

陋汀

N ortbwesternBla' k劾j끄0:
O· 1αng＇》
＇5

Cameroun

1IJ

H』h

4m0y P.1. amoyensza

South Chum

120

ft 5i

Baa adee,

400

indoa.

Ante ar hmmnP.f. oaltumoo阡Emi Looooo4)445

■ 만일 원하는 요소가 루트 요소의 자라고 한다면
3-5번을 뛰어넘을 수 있다．

n999,

r ' n…
!1

Famen, 졔ark R뇨h1{r

-

-

fi이

Swumtyn: F.Lscavm,otmae

■path의 어떤 지점에서라도 *을 그 레벨의 모든
요소를 정하는 와일드카드로 사용할 수 있다．

츰기

仁츠『 「l9끼
卜ㅋ」：『 [1i15매

渗U廷orwoae

.:

그림lu4 커런트 노드를 무사했을 때는작업자가 현재 실행하고
있는 작업을 알고 있어ㅇ戶 한다는 깃을 명심하자. 이것은 위에서
보이는 깃처럼혼란스럽게 되는 것을 피할수 있는 구조를 갖게 할
것아다．

예걱）
의소스 코드는 www. cookwoodcom1/ 있즙니다．

159

＝ 빼＝ 。긍
。＝4m， 。，욕＝ 口47e口ㅋ m

4. cont미ner를입력한다. container자리에는
원하는 요소를 포함하는 다음 레벨의 요소 이름
이 있다.

그림끄i.' 어떻11subspecies of tiger (. 랑이 변종？ 다응에
Northwestern Black Rhino를 연산하게 되었는자 주꼭하자．

5.d

1. XML문서의 루트에서 출발한것임을명시하기
위해／으로 시작한다．
2. root를 입력한다. root자리에는XML문서의
루트요소가들어간다．

<tr><td><nobr><b>Northwestern Black Rhino:
</b></nobr><nobr>cp>D.b.
longipes</i>.c/nobr></td>

E.e

루트로부터 오는 길을 쓰는 것으로 커런트 노드
무시하기：

===== PAGE 152 =====
151 =====
다iapter 1 ]

노드의 속성 선택하기
만일 요소보다 노드의 속성에 관심이 많다면 ＠을
사용함으로써 속정 축을 정할 수 있다．
노드의 속｛引I 정하기：
1. 이 장에서 설명된 기술을 이용해서 노드로 가는
path를 적는다．
2. /＠를 입력하여 작성자가속성에 관심이 있다는
것을 알린다．
3. attribute｀를입력한다. attributes는관심이
있는 속정의 이름이 들어간다. 또는 노드의 속성
모두를 선택할 수 있는 와일드카드로써 *을
입력한다．

'/ 1ip

。 ＝。m= ＝닐으● m
m
● ＝슨， 驪 견 ● 큉

■ 새로운 태그 안에서 주문형 속성을 만들기 위해
서 이 방법과xsl:attribute 요소를 합칠 수
있다. 예를들면 비표준방식으로 포맷된 그림
데이터를표준WThll 1mg 태그로변화시킬수
있다. xsl:attribute 속성에 관한 더 자세한
사항은 p151의 속성쟁성하기를 참조한다．

至口j르F三쿠一＝ㅌ；＝∼一＝二拉∼code.HsIt窺논섶學 - E3높汪娑느

! 'U

<xsl:for-each select=「subspecies/region I
subspecies/population">
<tr>.ctd>cxsl:apply-templates
select="name"/></td>
<td><xsl:value-of select="region"/></td>
<td>.cxsl:apply-templates
select="population"/>.c/td>
<td><szxsl:vdue-of
select="population/@year"/></td></tr>
</xsl:lor-each>
그람 끄15요소의족성을 얻기 위해저 속성아귿 불라보는 @
가호를 이용한다．
軒i昇

<tr><td>-cnobr><b>Balian: </b></nobr>
<nobr><i>P.t. balica</i></nobr></td>
<td>Bali.c/td>
<td>.cfont color="red" title="that means there are no
more Ieft">Extinct</font></td>
<td> 1937.c/td></tr>
<tr><td><nobr>cb>Caspian: </b></nobr>
<nobr>ozi>P.t. virgata</i></nobr>.c/td>
<td>Caspian Sea</td>
<td>ozlont color="red" title="that means there are no
more left">Extinct.c/foni>c/td>
<k」
＞1950</td></ti>
그림끄拓 족정의 컨
［텐츠는 결과물이다．

fear

!000

닌e

3e`ch FaV이*eS

Tiger: panthera tigris
l

8ab`Pe.ie8

R. ion

}

l Nnb.r LiftlK` Of
`[Ex1凶그ct

｛끄al료u11s P.S. 施奇ca

!B'

Iit-a횅"isv rc Wrg刪

(1UasP긔m노.ea

作nxm」
L[

iJvasv P.S. oo,sdincα

三1J.Va

iIEbsct

ilAmoy: P.S. ,sso勿feW

渭oath China

120

褶.m,ata'an: P.S. 5.sma口av

1nd1쵸 Bsn山dethiI400

耆IAasmr or Sihrian, P.S. ajta,a의 Fur Eas唯l1조딴 . i변4午…

「Issdo-ehines.: P.S. eeeb久－壘do-Cbma
ITMo
fiessgal: P.s. ngeas

∼

主227
43159

그림11.17 웹iifl이ㅈ］에저는【ll이El가 원래XM 문서에서 족정아었
77나요소섰거나상관없다．

160

===== PAGE 153 =====
152 =====
XPath: Patterns and Expressions
二
＇

rode.nslt

r크J

<xs나empl아e
match="namef 'language='English']'>

모든 노드 세트를 선택하는 것은 언제나 완벽한 정확
성을 갖고 있는 것은 아니다. 부을 표현식（서술부라
고 한다）
을 만들어서 조건을 시험하고 테스트의 결과
에 따라 노드의 부분 집합을 선택할 수 있다．

<nobr><b><xsl:value-of select="."/>:
<b></nobr>
</xsl:tempkite>
그림끄18 이 템플릿은 language 족성이 영ㅇ／안 name 요소
에만 적용할수 있다．

==＝一독；
＝一一一三三ㅗ

크르＝三＝三＝

2. [（키보드의β 옆의사각괄호）
를입력한다．
3. 부분집합을정의하는표현을입력한다．
4. ］을입력한다．
'/ 1iF心
■ 부분집합을정의하고있는표현은비교변화형
이 될 필요는 없다. 이것은 위 예제에서 language속성을 가진（값과는 상관없이）모든 name
요소를 선택하는 기호인［이anguage］
를 쓰면
된다는 의미이다．

<subspecies>
<name lariguage="English">Amur or
Siberian</nome>
<name Ianguage="latin">P.t. altaica<!name>
<region>Far East Russia</region>

」＞ .

B柚

놔口LJ
■

「 꺼m

0

s啣

［〕 公

Rm.甘→m陋

自

幢〕

" L，
小＄"

sonch Favo*ee

드汕

Region

N mober Left

"

i

Snbspcieo
Balino, P4. bahca

nepao: P.1. c'rgo1α
쫀」D야＂

"∼
:' 히」，『

[Ac可

Tiger:panthera ngI'S
nn

l

l？加
和Loclerccool

그림끄2. 볼드체로 쓰여진 영ㅇ／이름은 그들의 템플랏에 의해
명기된 것차럼 콜론이 따라．
오게 된다．

예겨）의소스 코드는 www.cookwood. c.om에 있습나다ㄴ

＝」

■ 함수를사용해보다복잡한서술부（predicates)
를 쓸 수 있다. 더 자세한 사항은 12장의 테즈트
표현과 함수에 나와 있다．
■ 사용되는괄호가둥근괄호나보통괄호가아닌
사각 괄호인 것을 주의해라.
■ 검색의 범위를좁히기 위해서 복수의 서술부를
사용하자. name[이anguage='English']
는 language 속성값이
[position o=Iast 0］
영어인 name 요소와 세트에서 마지막 노드인
name 요소를 선택한다．
■ 또한 필요에 따라 서술부 다음에 속성 선택자를
첨가할수 있다. 예를들면 커런트 노드 세트
마지막요소의 모든 속성을 얻고자한다면 nast
o]/@' 을사용한다．

16 l

盼으m^ =＝山· ．口m. .
m

그림끄1.9 그림11.18에서보이는 텡플릿은 빨간줄로 표ㅈ／돤 아이
템들에만적용될깃아z批language 족성아라틴으로설정된
name 요소이）
는 적용되지 않는대．

F19어超5 bole Sole

부분 집합 선택하기：
1. 이 장의 나머지 부분의 지시에 따라 원하는 부분
집합을 포함하는노드로 가는 path를 만든다．

Cade.1i11n
楓
<animal>
<name longuage="English">Tiger</name>
<name Ianguage="Latin">panthera tigris.c!name>
<threats><threat>poochers</threat>
<threat하iabitat destruction</threat>
<threat>trade in tiger bones for traditional Chinese
medicine (TCMk/threat>
</threats>
<weight>500 pounds</weight>
<length>3 yards from nose to taik/length>
<source sectionid="120"
newspaperid="21"><Isource>
<pictrue filename="tiger.jpg" x="200" y=" 197"!>

才
Ek E예 ae'

부분 집합 선택하기

===== PAGE 154 =====
153 =====
12

TEST EXPRESSIONS
AND FUNCTIONS
테스트 표현과 함수

작성자가 어떻게 xsl:value-of를 가진 노드의
컨텐츠를도출할수 있는지를 배웠다. 사실 xsl:
value-of는 노드 세트 안에서 첫째 노드의 기호열
값을 결과로 나타낸다. 이 장에 설명된 것과 같이
함수를 이용해서 출력되기 전에 기호열에 하나 이상
의 조작을 할 수 있을 것이다．
때로는결과를출력할필요가 없다. 그대신에 xsl:
if 혹은xsl :when 지시 사항 안의 테스트 조건과
같이 데이터를사용하고 싶을 것이다. 함수는보다
복잡한 상황에서 테스트할 수 있도록 할 수 있다.
노드 세트 안에서 노드의 부분 집합을 선택하기 위해
서는 서술부 내에서 함수를 선택할 수 있다．

163

큐m* m
X
亡
， mm驪。 ＝m。 ＝`m口굿궁＝ 驕

함수에 관한 공식적인 설명은 월드 와이드 웹 콘소시
움 사이트 http://www.w3.org/TR/xpath#corelib
에서 볼 수 있다．

===== PAGE 155 =====
154 =====
Chapter 1 2

두 개의 값들 비교하기
작성자가 수행할 가장 일반적인 테스트는 하나의
값이 다른 값보다 클 것인가 하는 점일 것이다. 작성
자는 어느 조치가 결과를 도출할 것인가를 결정하기
위해서 답을 사용할 수 있다．
두 개의 값 비교하기：
1. 비교하고자하는첫번째 노드세트를 연결하는
path를만든다．
,
2. 두값을어떻게 비교할것인가에따라＝（등호）
, &gt;（크다）
,
!=（같지 않다는 의미, 부등호）
（적다）혹은씨t;=
, 帥；
&gt;=（크거나 같다）
（적거나 같다）
을 입력한다．
3. 노드세트로의 path나또는1번에서 노드세트
와 비교하기를 원하는 값을 입력한다．

V Tips
■ 만일 단지 하나의 노드 세트가 존재하는지（컨텐
츠와 관계없이）테스트하고 싶다면 2-3번을
건너뛴다．
■3번에서 기호열과 텍스트 값은 작은 인용 부호
로 감싸줘야 한다．
·e크口＞ O긺卜m튼口｀ ㅌ。U

■and를 사용하여 복수 조건들의 시리즈가 옳은
지 여부를 테스트한다. or을 사용하여 복수
조건들의 시리즈 중 적어도 하나의 조건이 옳다
는 것을 테스트한다．

II

aj

code.xslt

이베on,,>
<xsl:template match="p아）
<xsl:choose>
<xsl:when test=". = 0">
<font color="red" title="that means there are
no more Ieft">Extinct</fon>
</xsl:when>
<xsl:when test=". &gt; 0 and .&lt; 50">
<font title="they're almost gone">
<xsl:value-of select="."/></font>
</xsl:when>
<xsl:otherwise>
<xsl:value-of select="."/>
</xsl:otherwise>
</xsl:choose>.c/xsl:template>
그림I幻 처음 예제에저 커런트 노드（마침표叩 의해저표시된？
값아 0인又］
를 테스트할수 있다. Extinct라는 단어가 결과이다．
두번째 예제에서는 커런트 노드가 (7보다크고 50 다 적은자를
살펴보아야한다. 아경우to汕p과함께밌는they are almost
gone이 결과아다（이 예제를pz49의조건적인 선택권 첨가하가
에서볼 수 있었다？.

cDde.htm르 三

스I二

巨I

<tr><td><nobi-><b>Balian: </b></nobr>
<nobr><i>P.t. balica</i></nobr>.c/td>
<td>Bali.'z/td>
<td><font color="red" title="that means there are
no more Ieft'>Extinct</font></td>
<td>1937</td></tr>
그림lz2Balian tiger는l937년에 멸종되었고 이깃의 개체수는
0아 되었기 때문에Extinct가 결과：르 나타난다（빨간줄로 되아
있고 중첩되아 있는 것夕．

Eh E出 y月1쎄
4=
e配k

Tiger: panthera tigris
Subope,ies

;

Region-n Nmnber t뻐Aoor

Anon홴rSken P봔igaC2 Far EnatFaran l:i4드
Beline, P.L ba&a
!
java
4
Ja1ra』
r尸亡立갯山叱α

녠999 :
ㅣ
ㅣ四37 .

生壅多뜨f씻yivg,r
Benga1 P.뜨agvav
Semetran, P4. ononL,vao

Cavp,nv Sea
1
Iv여a
如-59
In出a, Br, adev다1」
〕
0

a 1950
"999
nd999

Amoy, P4. nn얻. non

Sva Cln,a

뱐” 5

겯，
輛富m굽

」三 ∼ 」 t

; 2q

1972 ]

'1 r－卞弩i舞i＇日可

그림12.3 하나의 값과 다른 값을 비교한 것은 일반적인 종류의
바스트이다．

164

===== PAGE 156 =====
155 =====
Test Expressions and Functions
［ㅍ…

琴戮

tade.ssnul

위치 테스트하기

<threats>
<threat>poachers</threat>
<threat카labitat destruction</小reat>
<threahtrade in tiger bones for traditional
Chinese medicine (TCM)</threat>
</threats>

작성자는 처음, 둘째, 나아가노드의 마지막자식을
선택할 수 있다．
노드의 위치 테스트하기：

그림12.4XML 문서의 안용은 threats 요소 안에포함된세개의
threat 요소들을보여준다．

노드 세트 안에서 마지막 노드 찾기：

握 code.ks1t …1릎
口
<xsl:templ아e matd`＝싸ire아5">

las네으로 마지막노드를 얻을수 있다．

c/

<p>The migthy <xsl:value-of
select="../name[@language='English']"/> laces
numerous threats, among them <xsl:for-each
select="threat">
<xsl:value-of select="."/>
<xsl:choose>
<xsl:when test="position 0=last (l">.c/xsl:when>
<xsl:when test="position ()=last ()-1 ">,and

'/ 1iPS
I

xsl:when>

<xsl:otherwise>, </xsl:otherwise>
</xsl:

choose>

</xsl:for-each>.c/p></xsl:template>
그림125 threats 요소 帥reat요소가 아나다）
를 위한 텡플릿이
존재하슨것아중요하다. 만할각칵의threat에threat 템플랏
을 적용한다면 그것은 차음 위챠斗저 나타낳 것이다. threats
템플랏에서 개별 threat 요소들은z,2와3등의 번호가붙여진다．
多Eadangeaed Ipeciso - M,oio,aoft aaernet Euploac,
y"｀착 Fuoo,ia

U position()=n의 약자로서 n을사용할수 있지만
그것은단지 서술부 내로 한정된다. 예를 들면
subspedes[1］
은 첫번째 subspecies 노드
안에서 결과가 나올 것이다 (xsl:if 혹은
xsl:when 시험 표현 안에서나xsl: valueof 지시 사항 안에서는 약자를 사용할 수 없다）
.

·回口

如ali 난*

ㅇ ［〕 公

(> .

Ba아，

position과 last 함수에 있는 괄호 사이에
어느것도넣을수 없다（다르고, 형식적인 단어
안에서 그들은 논쟁을 일으키지 않는다）
.

큐盼手． 추e， 。
驪
＝

E.e Eβ

position0=n을 입력한다. n자리에는통용노드
세트 안에서 노드의 위치를 정하는 숫자가 들어간다．

돠아》 Rple,h

lana

룐그

自

LH쟁4

Se려사， Faa여Jes

스」

Tiger: pan枋era tigris
s甘뇨＄Perie$

Re驢on

Nninthen left A, ( )r

Ea五a끄＝ P.L b, 奇ca
Caopna, 도누a

Java, : P.:. so做ica

Java

A'nor: 只스 s,'aoiansis

South 아mla

Sms,atran: FL a,aoaz,sao

Iotha. Sa넣adenli 4)U

Au,uo on Sihotian, F;i. aibk씨FatEaol Russia

1J

m:5
下F衿

44…

LX꿴」
H'"

b1do-shinoao, Pb. peeb.t.h

Lldo-曲na

1227

Benogal: PLkgeoo

,inndia

3159

＝
。

caspiata P.L v坦ta

999

가a nu竗ty Tsgbr foot,m,raneons tlaeoda. a noog them

r!

L1

i引 foot

MyCanaan

」
a림1Z6 threat 꾸j7）
는a것아 어딴 것이든 상관없이 결과로
나오게 된다. 만일 아깃이 마자막 위치에 나오면 마침표도 역사
결과물아다. 아깃이 끝乙브）
저두번째 위차라i2 하면 (position
( ) 1) , 쉼표와스폐이즈는 이 다음 결과물이다．그리고 이것아
다른 위치에 있다면 더해2/는 깃은 아무 깃도 없을 것이다．

예群의소스 코드는 www cookwood.com에 있습나다．

】65

===== PAGE 157 =====
156 =====
Chapter 12

가치값 소계하기
sum ( ) 함수를 사용하여 노드 세트 안에 있는 노드
들의 모든 값을 더할수 있다. 이것은 표로된 데이터
에아주좋다．
가치값 소계하기：
1. sum (．
을입력한다
2. 노드가더해져야하는노드세트에path를입력
한다.
』
3. I을입력하여 함수를마감한다．

톨賠릎긴

-

pl

→ 口）
dP.H引t 三：

<td><xsl:value-of select="population/@year"I>
</td></tr>
</xsl:for-eoch>
<tr><td><br/></td><td
aling="right"><b>lotal: </b></td><td><xsl:valueof seled="sum (subspecies/popuIaton)"/>
</td><td><br/></td></tr>
az/table>
서 xsl:
그림1요7xsl: for-each 요소후에 터）아블끝전이）
value-of 자사 명령을 넣는다. 이깃은각동꿀군의 합을 얻기
위함아다．
簿Enda四e,ed Specien M蹈＂}cn5t Inusnet [휘pIn,c.
쿄Vcne了 工
（d`

Eip 트｀

1

麻

5t口P

·

Rdrr나， ㅐam

뇨ad, Fa'meㅎ

Tiger: ptnthera tigris
NoireberLeft An Of

R￡땔inn

SubsFerie`

Buliasos P.t. InuIra---－曾뾔

遣쁘翌

1「

Cuopian= Pt. vrg.ua

- 樊世rt

I'

Java】
1： 』아．sond청fca

1--Ce斗sasi iee
汀ava

套sm毖午斟
工r,ba

Boing汕尸．
Lsigns

1的口

3l59
T0tat

도三

三

The mt甘1ty Tn8to lines numerous threats, moot准 thens psarhrrs, bubotat
dentstsctson, end trade on tiger bones for traditional Chinese medicnnt (11CM)

m
● 크口＞ m 灌 경 으 겸 m

In요ck I겸；hino: diceros bicornis
m= ==

그＝→二＝===.==-

-

=

=

Re흩i1〕
n

』

As 三
Of t

=

10

Cameroon

Black Ridsie:

以- ∼ 以

N1끄1`ber
Left

'

Kenya (Ethsopsa
-send Rwassda)

d4irs
∼…

1미＞a
‘

1T.
rmbin
1…
1SeEn,

그4S
74r
…-

195心
1-9?-9 :

．줅 ．
---－輅－

∼－ -

y茗ons masonn』m'"
焦o
S。uthsow:
Adecuann
寸∼→－;---－上－∼컨亡∼－;-T5tl:

/
1

!

＇뇨1,Y;dJ`, nInd. PiH50 u..c1nsuc.n,出山cc팟5. mㄲma d比mmmdmc tU

수이다）
.
그람128 각동의동물군은 소계되고 출력되었다（하것은 실저）

166

===== PAGE 158 =====
157 =====
Test Expressions and Functions
Cj

Code.n引t ∼∼－--－∼口∼－ ∼三三考· ＝

<td>cxsl:value-of select="population/@year"/>
</td>sz/tr>
</xsl:lor-each>
ctr> ctd aling="right"><b>lotal: </b></td><td>
<xsl:value-of select="count (subspecies)"!>
subspeciesoz!td>
<td><xsl:vdue-of
select="sum (subspecies/population)"!>
<!td><td><br!></td>'c!tr>
<,'table>

때로는 노드 세트를 소계하는 것보다 단지 얼마나
있는지 알고 싶을 수도 있다
노드 숫자 세기：
1. count（를 입력한다．

그림끄9 아 인용은 animal 텡플릿 안에 았다는 것을 가억하차．
그라고 연산된 각각의 animal요소 안．
의 subspecies 요소
들의줏ㅈ屠셀 것이다．
斗Endontesed Speyhi, · Mio,osaat lntee,cl Es,plinn,

노드 숫자 세기

2. 노드세트가세고자하는노드에path를입력
한다．
3. ）를입력하여 함수를마감한다．

·ㅁ口

E긺． 丘ㅄ Yno 臼

幢그

L

Tiger: panthera tigris

1

[；〕 公

0

5'at

縊

'

喚

R盼a甘→mm

Sns,d1 Fav驪＇a零

Beag枇 P.s. Signs
T0tal=
The miajity T,ger face, ownerous threats, among them poachecs. habitat
desttucbon, and trade a tiger bones for traditional걋ateoe medicine (C山

＾。．===.＝。｀mm

Black Rhino: diceros bicornis
』，1
.
.】．n`Pe.le…

,m .
're凹on

=
샌,.r끄wa`uonsmaanmoums,n:
LID. iofl叩口t
.

1

一·

-1-

PEanteriuB1ackRhino:
:;D.b. onchsoh
Southweetesn Black

1`T괘」1r1ber
Lrft

Ol

icalner的n
f

기〕

1999

iRenya (Ethiopa
and Ratanda)

4요｀

『1q勺勺

－一r-

－一

－

小∼

-1

Rhino,

Imihas

(1999

1￥

t
i{S.띠心seen Blank Rhj皿m
\!D.b. manseㄱ

=

=

=

」

`

Zsro,b毓bWe a1ld
궁oot} Afhca

---n가－

B68

ㅓ 99

`-

ht出：

,

The yra蜘ty Black Rhino faces numerous thrtats among then, poaching to
satisfy dnanand for rhino hors, in trarhsionaj ASian medicmes and as decorative
dagger bandles m小ddle EasS. a끄d habitat dctslacbon
) Sans

…

O L。
計寸aa示一－-－三

그림1幻0 subspecies라는 단어는count 함수에 의해 섕성되는
것이 아나라는 깃을 주의하자. 이것은 단지 문자상의 단어아고 위의
스타일 시트에 나타난다（여가저는 Total아라는 단아룰 테아블
안의 첫째칼럼叩 넣었다는 것에주의. 이우는subspecies count를
위한공간이 있가 때문아다）
.

예켜）
의소스 코드는 wwss cookwood.com에 있습나다．

167

===== PAGE 159 =====
158 =====
약간 복잡해진 조건을 테스트하기 위해서 표현에
사칙 연산을 넣을 수 있다．
곱하기，나누기，더하기，빼기：
1. 첫번째 연산수를입력한다. 이것은12와같은
상수 혹은 노드 세트（이경우에는 첫째 노드의
기호열이 사용된다）
가 될 수도 있다．
2. 수학적 연산 기호를 입력한다：*（곱셈의 경우）
,
비V（나눗셈 / 은 이미 의미를 내포하고 있기
.
때문이다）+（덧셈）또는 ·（뺄셈）
3, 두번째 연산수를입력한다．

V Tips
■ 숫자들은 언제나 두 자리 이상의 유동적인 소수
점을 만드는데 이것은 지저분한 나눗셈을 만든
다（그림 12.12). 작성자는 dlv와 다른 함수를
합치고 싶을 것이다 (p 169-170).
m
==
V
。，
*
겸
＝ ＂占＝ 乞七빈m= m
경
＞

■ 평상시대로곱셈이나나눗셈은덧셈, 뺄셈 전에
행해진다. 다시 말하면 4+5*3은 19이지 27이
아니다. 괄호를 사용함으로써 디폴트 원칙을
무시할수 있다. 그래서 (4+5)*3은사실 27이다．
■ 다섯번째 연산자가 있다. mod 나눗셈의 나머지
를 결과로 나타내는 것이다. 그래서 20 mod 4
.
는 0（왜냐하면 4는 20을 나머지 없이 나눈다）
이지만20 mod 3은2이다. 왜냐하면 20/3은
6과 나머지 2이기 때문이다．

。
m
｀
m
＝ 三 읖 ＝론
168

U

回rUㅋ

:口｀de. l1$1t

.cxsl:templote match= 'population">
<xsl:choose>
<xsl:when test=". = 0">
<font color="red" title="that means there are
no more left">Extinctc/lont>
</xsl:岫en>
<xsl:otherwise>
<xsl:volue-ohelect="."I> kxsl:value-of select=" .
dic sum (..1./subspecies/population) ' 100"/>%)
</xsl:otherwise>
</xsl:choose>
</xsl:template>
a림12.끄population 텡플랏 인珊서는population아 0아
아나라고 하면 커런트 노드가 연산되고 있는 변종의 동물군을 그
동물의 변종 동물군 수로 나누고 결과0力00을 곱한다（명료함을
위해서 xsl : when 지사 명령을 생략한 것을 명심하차7.

‘尹驪낚口

「

윤 1‘呼

0

5瞰

l. m

口一

nmhm니

Tiger:

S꽈fk.R.p.阿：
r

panthera

곱하기, 나누기, 더하기, 빼기

=

Chapter 1 2

tigris-

L.ft

－…

콘

시

立lfld13339M81
9建3 1
394344989t
441496
88

陋甕荒T驅쩨
陋三齋m궉爵夔그
뇨겯닢
나蛾熬鑿學戶亡；

材빰雀弄＝尋辯葦覲舞母老戴-靄聃싸資腑曙硝蒜月늉統珊촬J義g驪鬱m－胛聃

그림f2.l2퍼센ㅌ仁］
는 정확하지만보기에좋ㅈ］
않다. 다음폐아지
에서보가 좋게 만들 것아다．

===== PAGE 160 =====
159 =====
Test Expressions and Functions
code.Hslt 7

톨藁1嘴

<xsl:tem이ate match="population「>

수동으로 퍼센티지와 지난 페이지에서 시도했던
다른 종류의 숫자들을 포맷하는 대신에 포맷 숫자
함수를 이용하는 것이 훨씬 편리할 것이다．

<xsl:choose>
<xsl:v小en test=". == 0">
<font color="red" title="that means there are
no more Ie1t">Extinct.t/font>
</xsl:when>

숫자 포맷하기：

<xsl:otherwise>
<xsl:value-of select="."I> kxsl:value-of
select="format-number ( .出v sum
(../../subspecies/population),'##O.O%')"/>)
</xsl:otherwise>
</xsl:choose>

1. format-numberI를입력한다．
2. 포맷되어질숫자를포함하는표현을입력한다．
3. ' '을입력한다（쉼표하나하나의 스페이스，
.
인용 부호）

</xsl:template>
그림I幻3 포맷되는 줏자슨 정확i168의그림i2.끄과같게 된다．
그리고 이것은 소수첨 왼쪽자라에 (1라나 왼쪽의 줏자를 생략
소한 한자리를 가진 퍼센C杯／로 포맷될
하는 것은 불가눙하cj-) 최．
것아고 소수쩜오른쪽 자라에 정확하 한자리가 올 것아다．
斗 En4..qeeod Speeses - Mse.s.oft Inlesees tsplo,e,
드1뇨 희n Vn윙i m-acute 工ocr

느 .

（꾜 ［스

心

自

力

G그

),
L, (s

'I ' iger: 끄anthera tigris
小욘e夔뻔－－〕끄뜨9뜨L쁘VF卜Of
쬐
트쁘뜨－∼∼l匣》
Cospiseso P.L vsrgaia
Caspian Sea－긔陝쁘뜨∼.-m. 巨E툴미
;
JavaO: Pd. sondasca
눋些브一－→J匣壅그
Jana
`쁘工珊기 l巨§j기
ama90 P. '5's- !" 's: S.ud1 cbina
Susnatrans m . m71口m결e
fr스츠尨叩덛a르esj400 (- 7?1, f1999
'.
)
or Sibesiasso Pd. aitascra F첵E超t르쁘쁘色－,l
S'sb'Faries --- ,

L

…

－」

－

J

蜘ur

l445

如

的99

쁘中

Bali000/tL ba쇼s-u

Indo-cbinese:끄corbetfl

Indu-Cisina

"227 (=「」.-) 1998

Bangola Pd. Ugno

hda

3159（汕 m n999

Totald8s叱species

5251

The mi竗y Tiger faces saassseruoss threats, anceg them po'selsoti. hubiut
desbuchon, and trade no tiger bonco for Irs-baboon 아끄neS亡 rαe山cme 丁CM)

羹i.며裙
[
和 Lnrd.0000
그림1Z14 퍼센티지는 많은 자릿수가 없어보7］
에 훨씬 좋다（파센
타차 주변에 콸호들은 줏자를 만드는xsl ;value-of 요조 주변
에스타일시트 안에써놓은 문자상의요소들아대）
.

예제의소스 코드는 www.cookwood.com叩 있즙나다．

숫자 포맷하기

4. 언제나나타나는숫자에0을쓰고0이 아닐 때
（중요하지 않을 때）
만 나타나는 숫자에＃을
쓰고, 정수부분과분수부분을구분하고싶다면
．를 쓰고 정수 파트의 정수 그룹을 나누고 싶다
면, 퍼센티지로숫자를보이려면％를쓰면
된다．
5. ·）
（괄호가따라오는인용부호）
를숫자패턴과
함수를 마감하는데 입력한다．

'/ nPS
■ 정수부분의 한자리수, 매 3자리마다 나누어지
는 쉼표와 함께 분수 부분의 숫자에서 정확히
두자리（달라와 센트처럼：269.40）
를 표현할 때
#$0.00을사용한다. #,000.0＃와함께라면
십자리를 가지고 있지만 백자리를 가지고 있지
않은 숫자는 마지막 0을 갖지 않는다．
■ 디폴트 값에서 음수는 그 앞에 (-) 사인이 나온
다. 그들이 괄호에 둘러싸여 있다면 위의 4번에
쨔
（o）
을 첨가한다．

]69

===== PAGE 161 =====
160 =====
Chapter 1 2

숫자 라운딩하기
숫자를 라운딩하는 세 개의 함수가 있다. 언제나
반올림할 수도 있고 반내림할 수도 있다. 혹은 가장
가까운 정수로 만들 수도 있다．
숫자 ㄹ운딩하기：

；그

團

code.Rm1

「/>
「200" y="197
<p1cture filename="tiger.jpg" x=
그림12.15 XML 파일의 안용에저는 이마자의오라자널 사아즈가
2(X:）팍셀 와이드 197팍셀 tall이다．
勤1
<xsl:temHate motch="picture">
<img>
<xsl:attribute nome="src">cxsl:value-of
select=" ./@filename"/></xsl:attribute>
<xsl:attr,bute name="width"><xsl:value-of
select="ceiling (./@x div 2)"/></xsl:attribute>
<xsi:attribute name="height"><xsl:value-of
select="ceiling I ./@y div 2)"/></xsl:attribute>

1. 반올림하고싶은지 반내림하고싶은지 아니면
가까운 정수로 만들 것인지에 따라ceiling (,
floor(, round
（를 입력한다．
2. 포맷할숫자를포함하는표현을 입력한다．

</img>

3. ）을입력하여 함수를마감한다．

</xsl:template>
그림12.16 아 메안 페아자에서는사진이그들의 반사아즈로 보여
자刀를 원한다.RThL 태2width와height는 단자 숫자만을
하우하가 때문에 여가서는ceiling 함수를 아용해서 나눗셈을
가장가까운 줏자로 반올림했다 (p151에서의그림10.30과 비교7.
口

c de.htnㅐ

<body bgcolor="white">
<p align="center">odmg src="tiger. pg'
width="100" height="99">
그람i幻γ이ㅁ／자의높이값은99이다. 이것은98.5후에 나타나는
정수이다 α97을2로 나눔？.

。
“
·，。＝ㅌ문m＝ 乞
＝＝

互 Endanoe,ed SpCr,CO Mir,ooolt 1flOroflOt Fopto,e,
E'S

ym밈

Ft.or.oCo

ㅗoco

0

■H口

브Ce

［ㅍ） 口｝

余여） n轍d넓1

H口m

巨그

自

Se.d1 FaY嫩e$

Tiger: panthera tigris
Snbqoerie`

Region

Nn'nbcc Left ASOf

Balla】
1: P.i, b加a

Lal`

(atpioni P.,.. t'irgoolo

}Coopo , Sco

F

Javaic P.S. awsdaica

hray.

1

宅3 Due

'1972

d999

.d,a, Bordadcoh 400 (76%r1999 ,

【 East kussia
AmUr Or 駐beiialr 尸．
￡，‘出mr`J Fa
i끄e`r F.1. ro,batls
工odorh」

ㄱ

沁 (0.3幻

Am,o什
Sm,rntoanIF,Ls '77,tbtOe

1937

d95(L

1끄小）아끄1la

445 (8 4%>

1999 ㅓ

1227 (23 3%) 1992

」

茁〔而i而云

=Z림 工2.招 메인 페이자의호랑이 사잔은 보통 사아즈의 거의 절반
사하즈다 :100*99 픽셀．

170

===== PAGE 162 =====
161 =====
Test Expressions and Functions
匡月

code.Hm(

，ㅋ1, n, '느1긋- ＝커＝r 麗릎

<animal>
<name language="English'>Tiger</name>
<name language="Latin">panthera tigris</name>
<threats><threabspoachers</threat>

<subspecies>

서브스트링 끌어내기
기호열을 탐구하는 것과 동시에 필요로 하는 정보만
을꺼내는것은유용한일이다. 예제에서는anmal
의 라틴 이름으로부터 속과 종의 첫 글자를 끌어냄으
로서 변종 이름의 약자 버전을 만들 수 있다．

<name Ianguage="English">Amur or
Siberian</name>
<name language="Latin">altaica</name>
<region>Far East Russia</region>

1. substring(．
을입력한다．

<population yeor=" 1999">445</population>

2. 소스기호열을포함하는표현을입력한다．

그림12.19 XML 문서아서는 라틴 animal name은 언제나족과
종의 정식아。
e 포함하고 았다. XSLT. 그들을 섕성할 때그것
아 복사되차 않도록x人凡 문서 인메저 각각의 변종의라틴 아름
으로부El 찻 글차를 제77한다．

3. In을 입력한다. n의 자리에는끌어내려 하는
첫번째 글자의 위치가 온다. 쉼표는 서브스트링
함수 안에서 각각의 독립 변수를 분리한다．

서브스트링 끌어내기：

code.eslt

<xsl:template match="name [@language='Latin']">
<nobr><i><xsl:value-of select="."/>
</i></nobr></xsl:templote>
<xsl:templ아e
match='Subspecies/name [@language='Latin']'>
<nobr><i><xsl:vdue-of s이ect="substring
(../../name[@language='Latin'],1,1)"/>
<xsl:value-of select=".''/></i></nobr>

4. 필요에 따라＇m을 입력한다. 여기사m 자리에
는 끌어내고자 하는 글자의 수를 넣는다. 쉼표는
서브스트링 함수에서 독립 변수를 분리한다．
5. I을입력하여 함수를마감한다．

</xsl:template>

口＝ 。
＾
土
＝ ．내틉m* ==g

그림1Z20 subspicies의 라든？ 아틈을 위한새로운 템플랏 안에Al
서브스트링( substring)을 animal 라탄 아릉의 첫 글ㅈ屠
끌어오는더］사우함수 았다．
` Ends.,qesed Species H,crn,oft Into.
,.甘 E柳toss,
f:to

Y比1니 「흐V了료擊i

i＝』m므

느Sp

<h .

ㅇ

D

t各

曦 〔끄

Otek

Slop

A.ls. l,

Hoe,.,

SensE roVo,te,

Subs1,.dCs
Balian: v6口쇼rα

Regis..

iBab

陣umber

Tiger: panthera tigris
Of
兩캬－

Left An

陋됴F

cas꾸1am pelrgaea

Caspiar. Sea

[EsEOC:

作50

Janal.
.

眈和ii I

准yㅍ心 -

1972

' 20 (03%)
스moy. /armoyenaas .
i South Ch.a
Swnab'an:p.Soaslalrae
l 뇨i. Ba,넣adeob 4`)0 (76%)
lAmtorSIbee6aIopaitalca J끄r츠a프t型竺쁘 」쁘憂堡491)

Ii
:3.5

1]999

그림1Z21각각의subspice.s 라틴 이름 앞에소문자 p룰 넣는것
아 사작이다．

여）
제의소스 코드는 www.cookwood.com f/ 있습나다．

17】

===== PAGE 163 =====
162 =====
Chapter 12
특정 글자 전후에 등징하는 서브스트링 끌어내기
1. substring-after(혹은｀ubsfrmn어：)efore
（을
입력한다. 이것은글자 전후에 오는 기호열의
부분을 끌어내느냐에 따라 결정된다．
2. 소스기호열을포함하는표현을입력한다．
3. 'C를입력한다. C자리에는서브스트링이올
글자의 전후이다．
4. ）을 입력하여 함수를 마친다．

回尸

＝三－=＝三 c.de.H引t ？三

口

<xsl:template
match="subspecies/name [@Ianguage='Latin']'>
<nobr>ud><xsl:value-of select=
"substring (../../name[@Ianguage='Latin'],l ,1)"/>
<xsl:value-of select="substring (substring
aher (../../name[@Ianguage='Latin'J,"),l ,1)"/>.
<xsl:value-of select="."/></i></nobr>
</xsl:tem이ate>
그림l2.22animal의 라틴 아름 안에 았는 두번째 단어의 첫 글자
를 얻가 위해서 공간 다음에 나오는substring을 끌어낼 것아다
（그리고 결과의첫째 글자를 뻬는 substring 함수를 乂悟할 갓
아다）
. 여가서는 필요한 아침표와 스페아스를 수동으로 첨가했다는
것에 주목한다．

Eie im Y- F9vodes 工여* H여）
B珊1

余며） n1打鰕h

Hsea

F剝〕
r!5

Tiger: panthera tigris

;.

Amoysp. seauyeaas

V
口
， *=
各＝ 三내금mm= =

p슨 ‘ aeaL,si'

uth〕
ma

Es
《ri:t

1950

드｝m」
파t

n972

120(03%)

11999

J1,sdsi. 0au&udesh 400 (76%/

1佇99

Jㅋaup,an Sea
(Java
:

Coopions p.:. vvguou
Java p.;. sr'ndthca

'Saaa

NmberLe派
-5蔬rF h937

묘e騙on

－恥

-

Sabape,,ies

Bo1ianp.,. ba&a

AiaurorSibenap. a1taica 陸East Russia -1445 (9 4%( n999
1227 (23 3%) l 1993
胚」
뗀喚e.e=！二ssi,bau,
lnd5-Chu-si
：…

1

l驪di加1.
＝가耳
r－晦』

그림12.23 아제 두번째initial과 구두점을 갖고 있다. 거의 막바자
단계아다．

172

===== PAGE 164 =====
163 =====
Test Expressions and Functions
-－∼－ ＝죙뇨小 【ode.Iislt

기호열 대문자로 바꾸기

=

<xsl:templ아e
match="subspecies/name [@Ianguage='Latin']">
<nobr><i><xsl:value-of select="
tronsate (substring (..1../name[@tanguage=
'Latin'],l,l),'obcdefghijk(mnopqrstuvwxyz',
ABCDEFGHIJKLMNOPQRSTUVWXYZ')"/>
<xsl:value-oI select="substring (substring-after
(../../nome[@Ianguage='Latin'],' '1,1,1)"!>.
<xsl:value-ol se(ed="."/>oz/i></nobr>

텍스트를 다룰 때 글자를 대문자에서 소문자로, 또는
그 반대의 경우로 변환할 수 있는 것이 중요할 때가
있다．
기호염 대문자로 바꾸기：
1. tr미｀如눈
（을입력한다．
2. 소스기호열을포함하는표현을입력한다．

그림끄24 첫째initial에 대해서 아것을 대문자로 변환해주는
translate 함수를사용한다．

日e 日*

F,looa.

Y比V'

jo碼

■

배：1

놀 .

(3 ［〕 凸

B

s,op

R.he枷

楡

幢그

L.*I

FaY며ie三

Hova

3. 'abcdefgh喇mn이）
qrstuvwxyz'를입력한다
.
（쉼표, 공간, 변해야할글자를포함한기호열）

1

5. ）을입력하여 함수를마친다.

Tiger:／》α砒hera tigris
l

Subapenea
Ba1jav, F.t. balka

Region
노a1i

HCaspian Ft. wgata
「ㅎ

Caspiav Sea

卜Java.,, e. WI,

Java

쁘,

`

g.

`

1

I, 'iPS
■ 글자를 대문자에서 소운자로 바꾸려면 3번과
4번을 반대로 시행한다．

Namaber Left
a스7,
！兩7
n스 〔

p950

I

ll1

「

ㄱ

nnn

.;'-

.

ia

,a

-e5auth Cbma
m 날Vo)- 999
Jo&o, B ngiadvah攫씰蠟塑勻曜느

3 S。
ya

'

Amar or Sibenan, P4. 인恥lea 甘la SOOt Raa쁘 t4뗀2
（뽀冽 l쁘y5J
Ind。
-rhi。
。。e, F.t. carbew
怖d;:blWa
h227 (23 3%니1998

.

出綸『 '
느 畜L。1，

→

■translate 함수를 이용하여 글자가 다른
글자로 幽과게 할수 있다. 3번에서 변환될 글자
를 쓰고 3번에서 바뀔 결과의 글자를 입력하면
된다．

＾。흘흽＝ ＝山꽝＝ ＝
볍

Amoy弘amoyena,a
So lab-an, P.C anmat,-ae
-

4. 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'입력한다（쉼표, 공간그리고최종적으로 변화
.
해야 할 글자를 포함한 기호열）

그림12.25첫째initial은 대문자가되었다. 아렇녀］되면사작한녜
서부타 후퇴했다슨 생각이 들지도 모른다. 그랴나 차아점은 속
데아터가 animal name 요소 안에서 그리고 subspecies
name 요소 안에서 더 이상복사되지 않는다는 깃이다．가눙할 때
마다 뎨이타는오로자 한곳에만 저장아 되어야 하고 다음에가능
리와
한 많은 시용을 위해서 쓰이게 된다. 아것에는 더］이5/
에라모두저장된다．

예겨）
의소스 코드는 www.cookwood.com에 있습나다．

173

===== PAGE 165 =====
164 =====
PART 5:

Cascading Style Sheets
css 설정하기 177
css 레아아웃 γ89
cSs로 텍즈트 포맷하기 209

]75

===== PAGE 166 =====
165 =====
13

'

SETflNG UP CSS

css 설정하기

一code. HrnI

」

<?xml version="l.0" ?>

<picture filename="panther.ipg"text="Florida
Panther" x="216" y="215"/>
<name>Florida Panther"z/name>
<description>With perhaps no more than
<population>50.c/population> adults left in wild
areas of Southwestern Florida, the majestic but
그림＇粗 아것은 아 장에서 예저）
로 사용될XML 폐아자의사작
부분이다. 아것은 웹火尸／트에서 다운받아프린트할수 았다．

口

code J,杜ni 獗瓣璹轟擁蓑都川

d1tml><head><title>Panthers and
Otters</title></head>
<body>
<p class="intro">The animals and plants on our planet
are disappearing at alarming rate. It's time to do
something aboout it right nowi</p>
<img src="panther.jpg" alt="Florida Panther"
width="216" height="215" border="0">
<hi >Florida Panther'c/h1>
<p>With perhaps no more than 50 adults left in
wild areas of Southwestern Florida,
그림i` 2 여가에는 RThff 쓰여진 같은 파일 (.2림i列의다듬
아자자 않은 근사값아 나와 았다．

XML 문서 안에서 태그를 포맷하는 두 가지의 인기
있는 방법은 확장형 스타일 시트 언어 (Extensible
Stylesheet Language）
를 이용하여 변환하는것
(XSLT）
과 직렬형 스타일 시트 언어 (Cascading
Style Sheets (CSS）
를 사용하여 포맷하는 것이다．
XSLT를 이용하여 XML 문서를 HTML 문서로 바꿀
수 있기 때문에 스타일 포맷 (HTML 태그를 현명하
게 사용하는 것으로）
을 적용하는데 사용된다. 그러나
XSLT는 명백한 포맷 지시 설명을 갖고 있지 않다．
다시 말해 CSS는 포맷을 위해서 태어난 것이라고 할
수 있다. 이것은 배경색과 타입의 크기를 결정한다．
문서를 변환시킬 필요가 없을 경우에는 CSS를 이용
하여 XML로 직접 포맷할수 있다. 그러나 많은
사람들이 아직 XML을 직접 읽을 수 없는 브라우저
를 사용하고 있기 때문에 이것은 지금의 현실적인
대안이라기 보다는 미래 가능성에 관한 이야기이다.
지금 당장은 CSS를 XSLT와 함께 xML 문서로부터
생성된 ITI取αL 문서에 적용하는 것이 보다 일반적이
라 하겠다. 다음 장들에서는 XML에 CSS를 적용하
는 것에 초점을 맞출것이다. 그러나 CSS를 HTML
에 적용하는데 필요한 모든 정보도 제공될 것이다.

177

m
.= ＝ 山 ．, ＾ 旨

<endangered_species>
<intro>The animal and plants on our planet are
disappearing at an alarming rate. It's time to do
something about it right nowk/intro>

HTML에서 모든 태그는 고유의 디폴트 포맷을 갖고
있다. 만일 이 포맷이 맘에 들지 않는다면 다른 태그
들을 첨가함으로써 혹은 스타일 시트를 적용하여
알맞게 할수 있다. XML에서 태그들은 어떠한스타
일 캐릭터들과도 같이 시작하지 않는다. 작성자는
태그가 어떻게 보여야 하는지 정확히 정해야 한다．
사실 XML 문서는 그것를 정할 때까지 브라우저에
서 보이지 않을 것이다．

===== PAGE 167 =====
166 =====
Chapter 13

H毛토 ,＝글 口U ·쁠닐름X ,＝뇰 m匕

css를 작성하는 데 있어서 스타일이 XML의 비어
있는 판（그림 13.3）
에 적용될 것인지 혹은I{IML의
다양한 색상을 가진 판에 적용될 것인지를 판단하는
것은 매우 중요하다. 특히 XML에 직접 적용할 css
를 작성할 때 display 특성 中 9
（沙비 주의하자.
尸IML 작성할 때 스타일이 기존의 포맷팅에 첨가될
것이고 직접적인 모순이 있을 때에는 이것의 특성을
무효로 한다는 것에 주의한다．
css가 적용된 XML문서 내의 이미치와 링크I
이제까지의 어느 브라우저도 XLdnk와 XFointer
(p 225）를 지원하지 못하기 때문에 css에 직접적으
로 포맷되는 XML 문서들은 일반적으로 이미지와
링크를포함할 수 없다. 그러나background 속성
을 이용해서 실제 배경 이미지에 첨가된 이미지처럼
보이게 할수 있다. p201에서 볼수 있다．

`，미切 F」
￡了1,
'1h- anan組$ and plants on ow planet aro disoppearasg at as alamor,h rate tsr
vane to do something about it sight nawl F柚sda Paother '51姓1perhaps no
more than 50 adilts It且 m wild areas ofsou仕iWettesi5 F跡ssda, 난Se snateslic
b出 elusive Plosida Panther (Puma roncolar cotyi) iv perhaps one of the most
endangered species 헴그the wosid Grass roots and government널 agencies
have joined forces 跡 help keep the panther from erstinctioss 域beta have
focused on rrstannggenetsr 出versity m the hny P.P따ation by impo祗喀 8
Teven cougars an 1,95, and on avoiding arc,deats 771曲 cars by boiluing
ocdeepaoses below highways that pass through thest dwindling habitats
Scleotots believe 仕tat m仕1sat an t汪ertive mona8moms PIan, me Florida
Panther will disappear from the wild swtlan 25 yearn Giant River Otter The
Giant River OUts (Pterossura brasthensia) ts a remarkably socm ansea
ttavehng m grauPt of4-9 called ' b야I?. hendedby a mono8amous par 겹l《1
usually also con呵：)nsmg several generations .fo盼인05sf lhey hunt, groom
and rest t.ge나er, and have 9 vocalizations for consmussscati驪 And while
tbey can lull an Anaconda, they are no match for humans, who have brought
them to the br止 of erstssctson lhere are P텨十，
aP$ about roe thoosoc,1 I祗
/ *」
一 一 ：一 卜
＇ 1 r\
‘一 '
r」
＋ [
1 '1
∼
r
令 Loud eossssd

그림13.3 빈스타일 사트를 치적하는XML 문서는 약간 叩력 없아
보일수도 았다. 포맷팅도 뿐만 아나라 다른 아무즈
［도 없다. 만일
XA 문저를 ass 파일이］차정하자 않았다면 익스플로러 안에서는
X4fL 문서 컨텐츠의 "4/급 구조를보게 될 것아다. 그것은 아깃보다
보가에 좋자 않다 (p185의그람 13.13),
}Panshe,. and 미ten'- Miosssaft 5551eeen5 I spinner
聊e

트d

국」
Bsac

.

Yens

工耐

*

楡
s功口

_i)
"atinas,

·回口

*5■

css의 속성은 연속된 레이어의 각각이 마지막의 것
을 지배하는 레이어 안에서 포맷팅 정보를 더하는 것
이다. css를XML에 적용하는 것과 css를 H呱凡
에 적용하는 것 사이에 가장 큰 차이는I{I爪｛L 태그
가 이미 그들 사이에 포함된 포맷팅 정보를 가지고
있는 반면에 XML 태그는 그렇지 않다는 점이다．

l。
。n

■,

css

졸F\rs.',pae5heiis.sI - 54,r,nsutt ! ,dns. ns Esnkae,

5

H煮

XML에서의 css와 HTML에서의

nne animals and 더dots ru Our planiet are dsnappeexmg at an alassnsng rate It's
tone to ds some出istg about at sight noM

CSS1, CSS2 그리고 브라우저
css를 사용하는데 가장 극복하기 힘든 장애는 많은
브라우저들이 css의 부분적인 특징만을 지원한다는
것이다. 윈도우와맥을 위한 익스플로러 5는 css1
의 거의 모든 특징을 지원하는 반면에 CSS2에 대한
지원은 안정되어 있지 않다. Mozi끄a（이제 새로 출
의 초기 버전도 고르지
시될 넷스케이프 6의 엔진）
못한 지원을 드러냈다. 최선의 방법은 많은 온라인
호환성 차트를 찾아보는 것이다（이 책의 웹사이트를
링크하자）
. 그리고 나서 css의 특징에 관한 사경을
브라우저 중에 가장 효과적인 것으로 선택하여 사용
한다．

178

Florida Panther
wm1perhapt no more tha」
150 a(hs助 It杜 m sold areas ofSoumwesterss
P跡sida, vfithout ins e侄ictsve managemen냐elan, 仕Se PlovdaPanther will
d1s呵P.ar w心an25 years ' me an司rstc b,t elusive FIonda Pand긔er rn‘〃m
co,tco1orcon砂 is peels芩,s one of the most endangered species an 由eworld

「 rm 瀚LindrdoideL_,：…石二
그림13.4 폭같은 정보를X7匠L에서 쓴 것아다. css 없아 조금
다르게보인다. ji7孔i1차 함ll 시작하는 것 凸：ML 문서로부p7
（원하던
XSLT 생산한 것；쁜포맷팅의차음 사작을 줄 것이다
그랗자 않뎐 간吼）
.

===== PAGE 168 =====
167 =====
Setting up CSS

스타일의 분석

굽은괄호

「셀렉터

i.
.

. .

"언

세미콜론
，,

,

\,

aescriprion talspi.ay:DlocK; -

p역변엣:relativ
AI I 엔e甲Z이,. ,

,

wIurn:`)4v;ooraer:TnIn soiia rea;

padding:5;margin-top:5}
부가샨언

마지막굽은
괄호

셀렉터는 예제에 나온 subspecies 혹은 threat
같이 요소 이름만큼 간단할 수 있다. 혹은 포맷하기
를 원하는 특정 요소들과 상응하는 패턴을 형성하기
위하여 여러 종류의 셀렉터를혼합할수 있다. 자세
한사항은 p180의 스타일의적용 위치 정하기를
참조한다．
적용되는 실제 포맷팅은 선언에 의존하는데 선언은
특성, 콜론 그리고 하나 이상의 값으로 형성되어
있다. 예를들면 텍스트의 색을 바꾸려고 하면 red의
값인color 속성을사용한다, 정의는Cdor:red로
읽을 수 있을 것이다. 콜론 다음에 있는 공간은 선택
사항이다. 복수의 선언들은세미콜론에 의해 나누어
져야한다.
몇몇의 특성들은 특별한 우산 속정으로 (font,
background 그리고border) 묶을 수 있다．
예를 들어 font:b히d l2ptlekton은 bnt-size:
l2pt; font-weight:bold; font-family Tekton과
같은 것이다．
많은 속성들은 부모 요소로부터 자 요소들로 우전된
을 부모
다. 따라서 유전될 수 있는 속성（예 font）
요소에 적용하면 자 요소는 자동적으로 속성을 갖게
될 것이다. 속성의 다른 값을 자 요소에 명확하게
적용하는 것으로 유전되는 속성을 무시할 수 있다．
사용 가능한속성들과 스타일들을 정의하는데 사용
된 상응하는속성값들은 p190-222에 자세히 설명
되어 있다．

여）ㅊ甘）
의소스 코드는 www.cookwood.com에 있즙나다．

179

구． >＝요。 클녘。 *。닢三m

그림13.5스타일은 셀렉El ‘요소를 자정하거나흑은스타일아 적용
할요소들을 지정한다）그리고 하나 아상의요소들아 어떻게포맷되
어야 하는자를 설명할전언으로 구성되어 있다．

스타일은 셀렉터와 하나 이상의 선언으로 되어 있다．
셀렉터는 스타일이 어떤 요소에 적용되어야 하는지
（예를들면 모든 subspecies 요소）
를 정한다．
선언은 선택된 요소가 어떻게 보여지는지（빨간색，
12포인트 크기로 Lithos Regular체로 보여질 것이
다）결정한다．

===== PAGE 169 =====
168 =====
Chapter 13

스타일의 적용 위치 정하기
셀렉터는 문서에서 선언 안에 있는 포맷된 정보가
적용되어질 요소를 정한다．
스타일의 적용 위치U 정ㅎ七 샐렉터 작성하기：

횰口럴覃
「

그찮三毛－匹i
r돝를 code.css 1=-1jl긴－=；겯｝

intro, atmn_name {color:red}
2림好.6 여가의 ㅁ〃우 간단한스타일사트 안에 여7/저는 intro
와 latin_nanie 꾜소들을위한스타일ㅈ］트를선언했다 (,2들
은 빨간색으로 칠해질 것아다. 그라나 선언 자치7에 까해서는 아직
많은 걱정을 할 필요는 없다夕．

■ * 을 입력하여 스타일을모든 요소에 적용한다．

■namel, name2, name3 등을 입력하여 스타
일이 명명된 요소 각각에 적용되게 한다. 각각의
요소 이름은 마지막 것과 쉼표에 의해 분리되어
야 한다．
■ parent descendanㅎ를쓰는것으로스타일이
부모 요소 안에 포함되는 자손요소에 적용되게
한다．
■ parent> 小ild로 스타일이 부모요소 안에
직접적으로 포함된 자요소에만 적용되게 한다
■ name:first-Jmd를써서 name요소가이것의
부모 요소의 찻 자요소일 때 name 요소에 스타
일이 적용되게 한다.
■ Before + af始r로 스타일이 before 요소 다음에
오는 after요소들만을 적용할수 있게 한다．
■name[att_name］
을 입력하여 att name이라
불리는 속성을 가진 이름 요소들에 스타일을
적용시킨다．
■ nam可att_name=att_value］
로스타일을
att value 값을 갖고 attnarne 이름과 속성을
가진 name 요소들에 적용시킨다．

180

3F On11\4》aa5iwasi,I - Mic,osoll IntemnI Esploini
stev 畦vours !oa ㅂek》

B;

●
휴
●
，
多
m
＝ 二* ＝
m굄｀ ㅎ·m鷺e， 졌 읓 占 ● ，

■name으로스타일을문서 안에있는모든 이름
요소에 적용한다．

k

a

Sen

뜨〕

ㅐ曲e;1)

늬
縕표．e 노 」r 3以IIirtflo.k O1- 『n it ugh n 긋U‘. 王4anda Pa祉icr W祉｀Perhaps no
mare than 50 adnltn left as wild areas of Southwestern Floisda, the majestic
bm dmice Flonda P．
』出or muma C oncolor- ovi, is pedsaps one ofthe most
endangered specses sotheworld 눗ass roots and governmen』a8encies
have joated forces to help keep the panther from entascnosn 班ortu hav·
focuoea on restonng gefletit dverssty m the tiny P0p山abon by a叩otting 요
Texan cougars os 1995. and on avoidi叱 accidents with Car` by butlding
undeqiasoes below haghways that pass throu助 their dssoudhng habitats
SconSists beheve 仕sat With.m aSicffectave management plan. 小e nOnda
25 year$ Gsans Paver Otterllie
PantherW1끄d`$aPPearBam仕IC W교d꿔出：山，
Giant River Otter mti -:,uoo 1'i ouihec: u' so a ren,atlcably social ansanal.
，d by a monogamous pan and
gaveh堪 m goups of4-9 C汕ed nh出四' , head』
m, groom
邸ua卦y also c0mPsizing several generatu000 of o函pnng They h1』
and rest together, and have 9voc勘onnons for conuinusucatst堪 Asd while
humans,
who
have
brou寸t
Anaconda,
they
are
no
match
for
也ey can kill an
1hㅎm t0 1he brash of entsnriosc lllere are perhaps about one thousand lrft
(maybe as many as 5we dsousa4 m a 6aCh이l of they former I嫩dIal that
.nce covered mud, .f goodl Amenca
世그Dme

匏0000 001000

그림13.7스타일은 셀렉터 안의7사 쉼표로 분라된 각각의요소들
에재 적용된다．

===== PAGE 170 =====
169 =====
Setting up CSS
\\ , `,,\ 1,\ 一，
,，
口츨
code.csu 一，

picture[filename='panther. jpg'] {background:bule}
그림弱；8 아 규칙은m批her.jpg의가차값을 가잔 filename으로
명명된 속정올포함하는 그림 요소에만 적용되어야 한다．
`F bc`$\panihrosusit - M,riosnts 1erasers Esplsrei
E1e
呻

■回口

loots 느eli
J
smc

끄
R轍e針〕

仝
Ones

穹
5e小아，

》）

■
),

U小

The animals and plants on our ;doimrt are dir妙peooi唯aj on 祉arrrLu堪 rate its
brat to do tome난dl〕
g ab.ut 沈 nitht 끄.vH 恥ssda RantherWid나arshup. nㅇ
more dtins 50 adsilts tea m Wdd areas of Southwestern Fbnda, 甘‘0 majesftC
but ehsssve nondaPnother mima concolor cosyi) is perhaps one of the 050st
endasigend species as the mciid Grags roots md gneerninent出 agencies
have joinedfdries to help keep tlse P翩玭‘er斤ㅇm extilichon E표이t5bave
focused ott restosssjg genenc 出vernty its 甘Se tiny P.P山anra by imports깜 8
Texan c0텍gar' ㅁ 초995, and on avoiding accidents m姓cars by budding
sasderpasaes below highways Lh然pass throu鱗 their dwindling habitats
Scientsnta beheve that wdh.Ut ass effectave snanagement PIan, the Flossda
Pal썹her an끄disappear丘.n1小ew,ldwsthm 25years Gant River Otter Thy
Giant Rover Otter (Pteromira brauilssnssu) so a remarkably social atom出
iravehiug m g onps 0f4-9 ca血d ' holt", headed by a monogamous Pa」
r and
usually also ccsi4》nsssig several gesieraboiuo of offspssng They hunt, 莩oom
and rest t.8＇吐‘ef. and haqe 9 coca뇨tons for conunuincab핑 And 澈沚e
dIcy Ct k：皿 an Aniaconda, dIty are no tunich for hornaasO, Wh() have brou帥t
them to the bunk of eliesuchon There are Perh町＞i about one tbousand he丘
(maybe as many as 됴＇e 山ousand) its a 丘actooss of their former habitat that
0nCe「．0vered n1Uch ㅇfS.Uds Mosenca
igj Diem

蠱；Lordrtsuw'

그림13.9 스타일은 속상의 값에 의존하여요소에스타일을 적용하슨
것은, 여가서보여진 익즈플로러5 윈도우 버전을포함해 아착 어느
브라우저에 의해서도 자원되자 않는다．

U name#id_name을입력하여id_name값을
갖고 ID 속정을 가진 name 요소에 스타일을
적용시킨다．
■name:link를 입력하여 아직 방문되지 않았던
링크인 name 요소에 스타일을 적용시킨다．
U name:visited를 입력하여 방문된 링크인 name
요소에 스타일을 적용시킨다．
■name:active를 입력하여 클릭하고 있는 링크인
name요소에 스타일을 적용시킨다．
U name:hover를입력하여 마우스로지정되고 있
는 링크인 name 요소에 적용 스타일을 시킨다．
■name:focu＄를 입력하여 키보드에 의해 선별되
어졌지만 아직 시행되지 않은 링크인 name
요소에 스타일을 적용시킨다．

'/ 1iP`
■ 불행히도모든셀렉터를지원하는브라우저는
없다. 대부분은처음네개와＃을지원한다．
■ 이론상으로는이러한셀렉터들을합침으로서
스타일을 적용하고자 하는 요소를 더 정확하게
정할수 있다. 그러나 현실상 많은 브라우저들이
표준을 지원하지는 않는다.
■ HTML문서에서 .class name（마침표다음
클래스 이름）
을 "[class=class_nameJ"（이전
의 약자형으로 사용할 수
페이지 마지막 절차）
있다．

예群의소스 코드는 wwsn,cnokwood.com에 있습나다．

1 81

。 老프궁｀
읗0＾ ㅋ룁＝ 山른7。 ，0꽝三mm＞ 긍뻐。 四

B

F0-ioise0

■ name[att_name.=att_v이ue］
를입력하여
스타일을 끄a끄2e 요소에 적용시킨다. 그 끄a끄1e
요소는 하나의 값과 함께 att-name 이름을
포함하는속성을갖고 있다. 하나의 값은 일련의
공간으로 나누어진 단어들을 포함하고 있고
이것들 중 하나가바로 att value이다．

===== PAGE 171 =====
170 =====
Chapter 13

외부 스타일 시트 작성하기
스타일 시트는 XML 문서에서 요소를 포맷하기
의 리스트
위해 정의했던 스타일（규칙이라고도 한다）
이다. XML 문서는 다이나믹하게 정보의 모음을
변화시키고 더구나 쉽게 포맷할 수 있도록 디자인되
어 있으므로 스타일 시트는 개별적이고 독립적인
텍스트문서이다．
*●0云으亡m 。＝느으X山＝ 。m灌乞0느U

스타일 시트 만돌기：
1. 텍스트 에디터와함께 새로운텍스트문서를
만든다．
2, 스타일이 적용될요소를설명하는셀렉터 이름
을 입력한다. 자세한사항은 p180을 보자．
3. ［을입력하여 적용되어야할속정의 시작을표시
한다.
4. 14장의 css 러）이아웃그리고15장의 Cs's로
텍즈트 포맷하기의 지시 명령을 사용하여 원하
는 만큼 많은 속성을 정의한다．
5. ｝을 입력하여 이 규칙의 끝을표시한다．
6. 스타일규칙에 따라2-5번을반복한다.
7. 원하는디렉토리에 텍스트로포맷된문서를
저장한다. 문서가 직렬형 스타일 시트 (Casca
로 정해졌다는 것을 표시하기
ding Style Sheet）
위해 확장자 .css를 문서에 삽입한다．

182

듣f＝…「

=

卄 code.css

＝毒노－
；三耳쿄珏 紆

endangered_species {display:block}
name {display:block;position:absolute;left:9}
intro (display:block;border:medium dotted red;
padding:5;margin-top:5}
description {display:block;position:relative;
left: 125width:340;border:thin solid red;
padding:5;morgin-top:5}
picture {display:block}
population {display:inline}
lotin_name {disploy:inline}
more_info {display:inline}
그림1缸0 스타일 사트는 셀렉타의 리즈트와그들이 나타내고
았는요소叩적용되어야할선언을포함하고 있다. 이것은 텍스트
만으로 .css확장차룰가지；고 저장되어야한다．

===== PAGE 172 =====
171 =====
Setting up CSS

v' Tips
■ 스타일 시트를 text oniy（텍스트 문서 혹은
ASCII라고도 한다）
로 저장하는 것을 명심하고
이것에 .css 확장자를 붙이는 것을 잊지 말자．
이것은 ASCII 모드로 - 2진법이 아님 - 업로드
해야한다．

■ 또한XMI로 스타일 시트를 만들수 있고 개별
태그로도 만들수 있다. 더 자세한사항은 p187
의 내부스타일 시트 사용하기와p188의 지엽적
으로 스타일 쟉용하기를 참조하면 된다. 로컬
스타일 시트는 외부 스타일 시트에 우선한다.
■ 원하는 만큼의 XML 문서에 외부 스타일 시트를
적용할 수 있다. 또한 하나의 XML 문서에 복수
스타일 시트를 적용할 수도 있을 것이다. 각각
의 연속되는 스타일 시트는 이전 선언된 스타일
시트보다 우선권을 가지게 된다.

예격）
의소스 코드는 www. cookwood. corn

있습나다；

183

4
＝ 。 꽝드m孚mm4
。．。＝＝山。 ＝mX. m

■ 속성의 개별 세트는 반드시 시작괄호 "["로
시작하고마침 괄호 "]"로마쳐야한다. 개별
속성과이것의 값은 ";" 세미콜론으로분리되야
한다．

m
呱

■ 스타일 시트 작성하는 법에 대한 더 많은 정보를
알고 싶다면 p179의 스타일의분석을참조한다．

===== PAGE 173 =====
172 =====
Chapter 1 3

XML 문서를 위한 스타일 시트
호출하기

*＝●ㅌ긍。 。H름님＝ 。，。＝●로 ＂으軫너。 m
＝틈 U

직렬형 (cascading) 스타일 시트를XM. 문서에
적용하기 위해서는 특별한 연산 지시 설명을 사용한
다. 만일 XML 문서가 XSLT로 연산되지 않을 경우
수동으로 연산 지시 설명을 해야 한다. 그렇지 않을
경우에는 XSLT 연산기가 그것을 첨가하게 해 주는
지시 명령의 두번째 세트에 따라야 한다．
수동으로 연산 지시 명령 만들기：
t

XML문서에서 처음XML선언다음에 <?xndSt코e낚teettype="text/css"를 입력한다．

2, 그리과iref="st닌e.css"를입력한다．
style.css 자리에는 직렬형 스타일 시트의 이름
이들어간다．
3. 마지막으로？＞을 입력하여 연산명령을마친다．

cei1e.Hml

=1平薑

<?xml version="l .0' ?>
<?xml-sMesheet type="text/css"
href="end_species.css" ?>
<endangered_species>
<intro>The animals and plants on our planet are
disappearing at an alarming rate. It's time to d0
something about it right nowl</intro>
<picture filename="panther.jpg" text="Florida
Panther" x="216" y="215"/>
<name>Florida Panther</name>
<description>With perhaps no more than
<population>50</population>adults left in wild
areas of Southwestern Florida, the majestic but
elusive Florida Panther <latin_name>(Puma
concolor coryik/latin_name>is perhaps one of the
그림13.11XML 문서 안에서 명확하게샹응하는 스타일 시트를
자정할수 있다（이경우 end_species.css).
c de.ㅐsH＇둑쿡룻＝두묩于룻4示窄＝之71弓
<?xml version=" 1.0" ?>

XSLT로 연산 명령 작성하기：
1. XSLT스타일 시트의 루트템플릿안에서
<xsl:processing-instructionname="xml｀이e寸teet"＞를 입력한다. 이것은 연산 명령을
작성하는요소이다.
2. 그리고type="text/css"를입력한다. 이것은
css 스타일 시트를 호출하는 것이다.
3. href="sMes.css"를입력한다. style.css자리
에는 스타일 시트의 이름이 들어간다．
4. 마지막으로＜/xsl:processing-instruction＞을
입력한다．

184

<xsl:siylesheet xmlns:xsl="http://www.w3.orgl
1999/XSL/Transform" version=" 1.0">
<xsl:template match="/">
<xsl:processing-instruction name="xmlSMesheet">
type="text/css" href="end_species.css"
</xsl:processing-instruction>
<xsl:apply-templates
select="endangered_species/animal"I>
</xsl:template>
그림1V2 아XSLT스타일 사트에 의해서 섕성된XML 문저는
(? 그끄l-stylesheettype='type/css'href 'erntspecie .css7.)
서의스타일 시트
라인을포함하고 따라저 생싱된XML 문서 인H）
호출은 그림13. 끄에서보았던 것과 동일한 것이다．

===== PAGE 174 =====
173 =====
Setting up CSS
斗F:\c$8'1〕anIknr, vol - Uvoonolt lon,nnv Fa, lo,ev
드M iJ
?
.楓寒

yn1o
.

mv｀
낮ie'

＇小

＞」r미 Y中＇$nm

V 'iPS

工nob H*
J
S따

＝〕
R轍e出

■ 원하는 만큼의 스타일 시트를 호출할 수 있다．
뒤의 것이 앞에 오는 것에 우선한다．

仝
Hone

…

스fU

{

:

含LnC小*미k냘

4
。 ＝님글尸。 。슨클0= *

여）겨］의소스 코드는 www.cookwood.com叩 있습나다．

■ 만일 각각의 모든요소 선언을 만들지 않았다면
그러한 요소들은 디폴트 사이즈와폰트로 보여
질 것이다. 어떤 이유에서 공백 스타일 시트를
사용하게 된다면 인터넷 익스플로러나 Mozifia
는 디폴트 사이즈와 폰트를 가진 텍스트의 한
블럭으로 출력하지는 않을 것이다．

。
m

그림13.13 만일 어느 스타일〃트도 정의하자 않았다면 악스플로
러는 문서를 겨r급 II Y의 형태로 보여줄 것이다. 문저의 컨텐츠를
보다분명하게보가 위q저문저를 접거나확장할수 오
（브나 아깃은
아착보가에흉하다．

■ 만일 XML 문서를 위한 스타일 시트를 호출하지
않았다면 익스플로러는 이것을 계급 체계의
형태로 나타낼 것이다（그림 13.13). 반면
Mozilla는 디폴트 사이즈와 폰트를 가진 텍스
트의 한 블럭처럼 모든 문서를 보여줄 것이다．

￡＝=．。꽝吾뿟g.

r, The ."in1出sand plants on our planet ore
小nappea
『ing at an 川arn엷ng rate. It1s htoo to do
`1}memjng aboat It hght flowlc/Intot>
apic Tu
「e 印enarn∼"p이lnver.jp9칡 tevta
『F始rldn Panther"
기＝"2l6" y驪
「2l5" />
caame,Fk,nda Pantherc/na*e,
c尨5t'ptean>
WIth perhep5no more than
｀【J口pU>>>,,,50.／心甘JmtD디，
:
adults left In wild areas of Soothwestem 디orlda,
the on이estip bot ebonite Florida Panther
∼뀁rarrer (Puma concolor coryi)e>恥mrate>
is perhaps one of 卄on most endangered species h】
the world. Grass roots and governmental agendas
have 徊hoed mrces to h미p keep the panther from
eatinction. Efforts haUe focused or, restar衲g
〔胛net沈 diversity in 盼op tiny mopolotion by
《r7캬口re rmo
『http://wsow.Panther나楸e 凡Is/penn,er/handbook/r
nrnu
B Texan coagars in lq95
/ prorl on oooirlinq e,ddCnts vitir cars by br.vildi,四

185

===== PAGE 175 =====
174 =====
Chapter 13

HTML 문서를 위한 스타일 시트
호출하기
만일 XSLT 연산자를 사용하여 XML 문서를 ITI丕4L
로 변환한다면 이것으로 마지막 포맷팅 정보를 갖고
있는 외부 스타일 시트를 호출할 수 있을 것이다．

률函韓＝賊－

c.d·J불引t `

<xsl template matc卜="/"><ht혜><head>
<title>Endangered Species</title>

*
＝
●
ㅌ
크
● 。결토＝ 口
， 。**●●云읓占口m트경

<link rel="sMesheet"type="text/css∥
href="end_species.css"/>
</head><body bgcolor="white">

1. XSLT 스타일 시트 안의 IfI以4L의 Head 부분
에서 <link rel=hstylesheetlIype=hltext/css1
를 입력한다．

<xsl:apply-templates
select="endangered_species/animal"/>
</body></html>
</xsl:template>

3. 만일XSLT스타일시트를통해 코드를첨가한
다면 /（물론 IT珏4L에서는 이것을 이용할 필요
가 없다）
을 반드시 입력해야 한다．
4. ＞을입력하여 uin]
（요소를마친다．

V Tips
■link 요소를XML문서에 첨가한다는 것은
말이 되지 않는 일이다. uin]( 요소는 XML에서
고유의 의미를 갖고 있지 않고 아무런 영향도
끼치지 못한다．
■XSLT에 의해 생성된 결과물에 표I爪江L 태그를
더하는 것에 대한 자세한사항은 p140에 나오는
RTML 코드 출력ㅎ7］
를 보면 된다．

186

．릍

<xsl:siylesheet xmlns:xsI="http://www.w3.org/
1999/XSL/ Transform" version="1.0">

HTML 문서튤 위한 스타일 시트 호丹하기：

2. href="刪es.css"를입력한다. styles.css자리
에는 직렬형 스타일 시트의 이름이 들어간다．

`

<?xml version="1.0" ?>

그胃13.14 아 XSLT스타일 A］
트에의해생성된／刃기iL 문저는
<link rel='stylesheet" type=" text/css"
href= "end_species . css"/> 포함할것아다. 아깃은
ffTh 문서가와부스타일 사트를호출하는표준적안 방법이다．

===== PAGE 176 =====
175 =====
Setting up CSS
口

tode.HSn

口Y

<?xml version="l .0' ?>
<xsl:stylesheet xmlns:xsl="http://www w3.org/
1999/XSI/ Transform" version="1.0>
<xsl:template match="/">.chtml><head>
<title>Endangered Species.c/title>
<5Me>

<![CDATA[
<L

endangered_species {display:block}
name {display:block;position:absolute; eft:9}

pop이ation {display:inlin놔
latin_name {display:inlink}
more_info {display:inlink}

]]>
</style>
</head>.cbody bgcolor="white">
<xsl:apply-templates
select="endangered_species/animal"I>
</body></html>
</xsl:template>
그림13.15스타일 태그는HTh 문서에스타일 사트 정보가위치
할 것아라 언급하고 았다. 긴.－는 스타일 정보를 자원하자 않는
브라우저로부타 줌긴다. 마자막：으로 < l [CDATA[ 비트는XAL
파서가스타일 정보를 보거나 분석하는 것을 막는다

예제의소즈 코드는 www.cookwood.corn에 있습나다．

HTML에서 스타일 시트를 문서 안쪽에 넣는 것은
완벽하게 규칙에 부합되는 것이다. 만일 XSLT로
IㅠML 문서를 생성한다면 추가적언 과정을 갖게
되는 것이다．
성하기：
HTML 문서에서 내부 스타일 시트 샘｝
1. XSLT스타일시트안의 RTML코드의Head
섹션 안에서（아마도 루트 템플릿 안）＜引닌e＞을
입력하여 내부스타일 시트를시작할수 있다．
2. 그다음에＜!ECDATA
［로xM.파서로부터 온
스타일 정보를 숨긴다（필수 사항은 아니지만
좋은 예방책이다）
.
3. 그리고＜!－을 입력하여 이것을 인식하지 못하
는 브라우저부터 온 스타일 정보를 숨긴다
（이것은 코멘팅 이웃 이라고 한다）
.
이아웃과15장의 css로포맷하刀
4. 14장css라）
에 설명한 대로 셀렉터와특성들을 입력한다.
5, 다음에··＞을입력하여 지원되지 않는브라우저
에서 스타일을 숨긴 코멘팅을 마친다．
6. ]]＞을입력하여 CDATA를마친다．
7. 마지막으로, <／刪e＞을입력한다.

I, 1i'
■ 내부 스타일 시트는 존재하고 있는 문서를 포맷
하는 데만 사용할 수 있기 때문에 이것은 보편
적인 것은 아닐 수 있다. 대신에 하나 이상의
문서에 적용할수 있는 외부 스타일 시트 柳82)
를 사용하는 편이 더 합리적이다.

187

．且＝ 山 =*m4금 닢三。 孚mm=

intro {display:block;border:medium dotted red;
padding:5;margin-top:5}
description {disHay:block;position:relative;
left:125,width:340;border:thin solid red;
padding:5;margin-top:5}
picture {display:block}

내부 스타일 시트 사용하기

===== PAGE 177 =====
176 =====
Chapter 1 3
지엽적으로 스타일 적용하기
XMT 혹은IfIML 태그 안의 특정 태그에 스타일을
적용하는 것은 스타일 시트의 효율성이나 능력을
이용하지 못하는 것인 반면에 스타일 시트가 제공하
고 있는 발전된 포맷에 접근하는 것은 유용하면서도
상대적으로간단한방법이다. 물론 이것은ffl
문서 (XSLT에 의해 생성）안에서만 작동할 것이다．
지엽적으로 스타일 적용하기：

m
＝ 三 듣＜
=＝트m으蘆 吻

1, 포맷하고자하는태그안에서引닌e=" 을입력
한다．
2. 14장과15장의 설명대로셀렉터와특정을입력
한다．
3, 부가스타일 정의를만들기 위해；（세미콜론）
을
입력하고 2번을 반복한다．
4. 마지막＂
（인용부호）
를 입력한다．

'/ nP`
■ 등호 기호와콜론을혼동하지 않도록주의하자．
그것은 값을 부여하기 때문에 별도의 알림 없이
둘을 혼동하기 쉽고 이것은 에러를 발생 시킨다．
■ 세미콜론을 가지고 복수의 특정 정의를 나누는
것을 잊지 말자．
■ 작성자는세미콜론과마지막까지를포함한가치
값으로 모든특정을마친다. 그러므로 이것을
첨가하는 것을 기억할 필요는 없다. 만일 그들이
한 쌍을 덧붙인다면 그것은 무방하나 요구 사항
은 아니다．
■ 인용부호 안에서 스타일 정의를중첩시키는
것을 잊지 말도록 하자．
■ xsl:attribute 요소로태그를만들수있다
(P151참조？.

188

ㅋcude.H引t

煌．
藝

<xsl:template match="animal">
<p style="background:yellow;color:red;texttransform-capitalize;border:double medium
green;font-weight:900;padding:O.5em">
<font size="-i-3"><xsl:apply-templates
select="name"/></font></p>
<p>The mighty <xsl:value-of
select="name[@language='English']"I> faces
numerous threats. For more information, check out
the World Wildlife Federation's <a
href="http://www.worldwildlife.org/species/species.
cfm?"> pages</a>. </p>chr/>
</xsl:template>
그림13.16 자엽적으로 스타일을 적용할 때 굽은 괄호 대신에큰
인용 부호를사용하여 선언 주변을 감싼다（아깃은 계족해저 All미
콜론과 구별되게 한다）
.

===== PAGE 178 =====
177 =====
LAYOUT WITH CSS

14

css 레이아웃

XML 요소들은 디폴트 포맷팅이 없기 때문에 첫번
째로 정해야 하는 것은 아주 기본척인 레이아웃 세팅
이다．

작성자가 조절할 수 있는 박스의 공간은 세 개가 있
다. 첫째로컨텐츠를둘러싸고있는것은괘딩이라고
하는공간이다. 작성자는 패딩의 넓이를조절할수
있다. 패딩의 주변부는보더이다. 보더는색을넣을
수 있거나 두껍게 만들 수 있고 또한 구성을 가질 수
있다. 보더의 주변부에 있는 것은 마잔이라고 하는
투명한 공간이다. 작성자는 이것의 색을 바꿀 수는
없지만 넓이나 높이를 조절할 수 있으며 따라서 페이
지에서 요소의 위치를 조절할 수 있다．
어떤 레이아웃 스타일은, 특히 퍼센티지 값 같은
것은 요소의 부모에 의존한다. 부모는 커런트 요소를
포함하는요소이다. 예를들어 animal 요소는
subspecies와name 태그를포함할 수도 있고
따라서 그들에게는 부모가 된다. 그러나 만일
animal 요소가subspecies 태그로나뉘어 있고
name 태그들은subspecies 안에 포함되어 있다
면 subspecies는name의 부모이다（또한 animal
. 마지막으로name
은subspecies의 부모이다）
태그가language 요소를포함할수도 있는데 차례
를 明긱서 이번에는 이것의 부모가 된다．

189

짢
경＝ ．트芬 ＾

하나의 요소 박스는 블록 단계（새로운 절을 생성한
다）
이거나 또는 직렬형（새로운 절을 생성하지 않음）
이다．

。
尸

css로 스타일된 모든 요소는 보이지 않는 박스로
감싸져 있다. 사이즈와 색 그리고 박스의 공간뿐
아니라 그 페이지의 다른 객체들과 관계된 흐름을
조절할 수 있다．

===== PAGE 179 =====
178 =====
Chapter 14

블록 단계 또는 직렬형으로 요소 정의
HTML에서는 모든 요소가 블록 단계（새로운 줄에
서 시작하고 이것을 따라오는 요소 또한 새로운 줄
안에서 시작할 것이다）또는 직렬형（이것은 줄 안에
서 나타난다）XML 요소를 사용한다면 이 특성을
명확하게 정의해야 한다．
鵑

단계 또는 직렬형으로 요소 정의하기：

。 ＝>0H～七。 玉m。 쓰＝ ●ㅌ으山m三＝ ＝●。
●灌ㅌ 느

1. display：를입력한다．
2. 비cck을입력하여블록단계（새로운줄쩨서
시작하고 이것을 따라오는 요소 또한 새로운 줄
로서의 요소를 보여 준다．
안에서 시작할 것이다）
또는 inline을 써서 직렬형（선행하는 요소 바로
뒤에 온다）
으로서의 요소를 보여 준다. Inline은
디폴트값이다．

i/ Tips
■ display를위한디폴트값은inline이다．
■ 이론적으로요소inline을만드는직접적인방법
은많지 않다. 작성자는display: compact,
display:run-in과 display:inlinetable을 사용할 수 있다. 이러한 것들의 유일한
문제는 지원하는 브라우저가 없다는 것이다．
U display특성은요소들을완전히숨기는데
. 또는 리스트 아이템
사용할수 있다 (p191 참조）
으로 그들을 보여주는데 사용한다 (p206 참조）
.
리스트 아이템은 블록 단계이다．
■ 넷스케이프4.x는HTML -소를위한디폴트
디스플레이 값의 무시를 지원하지 않는다．

190

目．
큰죠 느｀`&`,

,

code.css 三난1: 쬔斗큉릎죤휼蕣놀숩參莖陋즘

endangered_species {display:block}
name {display:block}
intro {display:block}
description {display:block}
picture {display:inline}
population {display:inline}
latin_name {display:inline}
more_info {display:inline}
그림蠟＇여기저는 name 아 그 라인에서 나타나가를 원한다．
block 다스플레이스타일을그걋이）적용한다. 반대로latin_
name아 inline에등장하기를 원한다．
돌 F;\c＄珊hiaethnts isiS - Us 'oistl Inleetri Espkises
Ea,
수J
B配k

.

-a,

J그

Re5寸｝

全

Hoes

The animals and plants oo Otto planet ore disappeanng at an alarming sate ifs
mne to do something about it ngbt news
Fk了卜1a 11U1t}nn
Wdh perhaps no more than 50 &d피is leftm wid rest .fs수U曲Westem
FIonda. 山e majestic but eluoive F1orida Por比er rPm11a concok, coey?) Is
pedtaps one ofthe most endin好teed speclea Sn 小twodd Graze roots Md
goverernental agencies ha甘e抑n已d forces to help keep me panther thoin
extinction E汪ores have fbcu'eJ on restore凹8enetic 出verssty m the tmy
population by snporto也 ft Texans이팡exam 1995, and on avoiding accidents
w.tb cars b미otoldmg s慽．
tpassea below highways tb鮮 pass thro哮 盼test
dwmdlasg habitat, Scsentistn believe that m‘山이it tat C丘ccliv, management
plan. the Floods Pocthtr trill dssappvar boro the odd within 25 years

」
麴 Landimesee

그림妊2XML 파일은 각각의name 요소 전후에서 현재 라안이
끊어치는 것을보여준다. 그러나 나u仁/ 텍즈트와같아 홀러온
latin name 요소의주변에는그렇자않다．

===== PAGE 180 =====
179 =====
Layoutwi出 css
요소를 완전히 감추기

컥련立三프드：
＝쵸도毛．
상크＝==＝프纖·

endangered_species {display:block}
name {display:block}
intro {display:block}
description {di利ay:block}

css 특성 즉 XSLT의 변환 속성을 닮아가는 것은
주어진 요소를 보여주지 않는 능력이다．
요소를 완전히 감추기：

picture {display:inline}

display:none이라고 입력한다．

population {display:inline}
latin_name {disploy:none}
more_info {display:inline}

·／ nP`

Ek

Eat

수』
B枕k

tais Paveiri
'

-I

工m」三 b*

」

nehen,

소

On,t

a

seα하，

》》

斗
Lr1(s

■ 스크립트와합쳐진display:none 정의는
같은 문서에 포함된 여러 버전 중의 하나에 속하
는 요소를 숨기는데 이상적이다．

The animals and plants on our planet are disappears낌 at an slanting rate Irs
tate to do something aboat d匕＇낳It now
Ftorid Pan":Ler
With peahapa sin more than 51) adnlts left as wild wele of Southwestern
恥nda, dit majestic bnt elusive Fb.uds 눠1】此니 L n -shas : one ofdle m.$.
endangreed species ndhr world Gcans roots and govershoem出 agenvies
have joined forces to heb keep the panther from entnrnosv Sifoeto have
focused ossrestos唱 genetic divensity m the 山】
yP.Pu油겋.11bymsportrng 8
Texan cougars m 1995' 흽nd 051 av.山ug accidents with cars bybnilding
saodespssseo below hi iwayt that pass theou鱗 then dwiridlmg habitats
Scientists believe that without an effective nassagement plan, the Flonda
Panther wit disappear front the wild within 25 yeav
玉ast 요aver ㅇLter
Tlie 白래nt Fieee C tier a a rrflsark淋1 sociN animal, traveling m groups sf4孑
c刈ed ho如',liesded by a msnoganoous Pan and usua표l also cowpnsss好
several generations .f수표lipemg They boast, groom and rest together 打1d
n* `,r卜＾＇놀41,,`1n..M솎｀n '1`d `d닒1' 伶｀mi m"卜'I, 口h ^n-＾·a*
h口,...0 口＾
＇口a-굻，

그림且4 latin_name 요소들은사라졌다．

역）
제의소스 코드는 www, cookwood. con끄어γ 밌습나다．

191

프
독
＝ 山쯩킁妾＾ 。＝릉흐

■display:none을사용한다면브라우저 창안에
있는 숨겨진 요소의 어떠한흔적도 남아있지
않다. 빈 공간도 없을 것이다．

그림14.3 display:none을사우함으롸〃요소들올 줌킬수
았다. 그들은 흐름에서완전하 밧어났다r 어띤 빈 哉：
＇도 그들이
0／다에 있ㅇ／야 하는자 표지하ㅈ／ 않는다．

===== PAGE 181 =====
180 =====
Chapter 14

자연적 흐름 안에서 요소 오프셋하기
각각의 요소는 페이지의 흐름에서 자연스러운 위치
가 있다. 원래 위치의 관점에서 요소를 움직이는
것을 상대적포자셔닝이라 한다. 주변의 요소들은
절대 영향을 받지 않는다．

立日∼一

-1-

code.cs$ 蒡

intro {display:bloc日
description
{display:block;position:relative;Ieft- 125px}
picture {display:inline}

*
●
m
**
。
多。 ＝ 므크。 ＝0츱＝ =＝●ㅌ으叫m= =

자연적 흐름 안에서 요소 오프셋하기：

pop너atice {display:inline}

1. position:rdative;를입력한다（세미콜론을
잊지 말자）
.

latin_name {disploy:none}

2. top, right, bottom또늬eh를입력한다．
3. :v를 입력한다. γ자리에는그것의 원래 위치로
부터 분리하려고 하는 요소의 원하는 거리가
있다. 이것은절대값또는상대값으로표현될수
도 있다 (lOpt 또는 2em).
4. 필요에 따라；
（세미콜론）
을쓰고부가위치에
대해서 2번과 3번을 반복한다．

'/ Tips
■ 상대적포지셔닝에서 상대적 (relative＞은요소
의 원래 위치를 설명하고 주변의 요소는 설명하
지 않는다. 다른 요소들의 자리로 요소를 움직일
수는 없다. 대신 원래 이것이 있었던 곳으로는
움직일수있다. 이것은중요한문제이다．
■ 다른요소들은파생에 대해서는 영향을받지 않
는다. 그들은 요소가 원래 포함하고 있는 박스로
흘러가고 있고 오버랩 될 수도 있다．
■ 다른요소 주변의 텍스트를흘러가게 하기 위해
서 그 요소는상대적으로 포지셔닝을 해야 한다．
■ position:r이아ive를포함하는것은오프셋을
가능하게 한다. 그것이 없다면 오프셋은 작동하
지 않을 것이다（익스플로러 안에서 오프셋들은
작동하지 않을 것이다）
.

192

-==＝ㅋ＝7學團彗

endangered_species {display:block}
name (display:block}

그림뵤5 description을 들여쓰가 하가 위헤저 여기서는괘라
그래프믈 그들이 원래 나타나야 하는 곳이）
/n25팍셀만큼 왼쪽으로
보냈다．
」｀F= \c8`\panlhe뢸！,rsrI Horrosoll tnlornot Eoirlo,e,
E* 트（눗 y흴BW F」
0050Cr 工ooJ 브*

논

Bark

.

呻

J

5呼

口

RH1e1h

소

ㅐan.

·回口

執

seJd,

lIre o,omals end 련ants oil Our planet are disappearoog at air alattieng rats itt
moo to do something abor* ltrl加newt
notsda Pallther
긱'砥 perhaps no snore 出an ,
nonda. the mme戚IC but eluor
亡r노dangered sP已r1e5 m 스ㅗ 밟
hsee oared forces vr
由cose小00 reotofl也핫1
"
Texan coogart or 1995. and 0n aooi껍ng a
as, the.
mderpoorer bH<)whghw.vr 出a댜）
Sceetenots believe 仕1帥 rvrth수rO an e표crave enairageloroit
Po止er a汕＆켜opour hooP the wdd W1ttm} 25 pears
G1깁〕t 拓ver 0me
Ihe Gsati River Otter .$ a remarkably sect可 anlmaL 甘a
d; ! 싣 . 1 : ` 4 . L … :'n
겠J n ; .

-7람 耳6 두 7ff의description은 그들의 원래 왼쪽 사작 사점
으로부터125팍셀 오프셋 되어 밌다．

===== PAGE 182 =====
181 =====
Layout with CSS
鄂珊奐＝
＝三－=＝三 Y ∼ 듣斗

cOde.c$8

요소의 절대적 포지셔닝하기

endangered_species {display:block}

문서 안에 있는 요소들은 일반적으로 나타나는 순서
에 의해 흘러간다. 다시 말해 name 요소가 description 요소 앞에 오게 되면 name은 description 이전에 나타나게 된다. 이것을 자연적 흐름이라
고 한다. 그들의 부모 요소에 관해서 정확한포지션
을 정해줌으로써 자연적 흐름에서 요소들을 꺼내올
수 있다. 또한 철대적포지셔닝을 할 수 있다．

name {display:block;position:absolute;!eft:9px}
intro {display:block}
description
{display:block;position:relative;Ieft:125px}
picture {display:block}
population {display:inline}
latin_name {display:inline}
more_info {display:inline}

츌F \. \pualhto. 샅ieL - M,o,oeoti lotv1n.U Ewloie.

4d

트at

B'3ㄴ

恥w

.

1뚜

Fori甘ei

目回ㅁ

J

5．
미）

n轍e곯1

仝

H뎌m

T뇨 ammals and plontu on ow planet arc 出＄appenn媤 at a쇼 alarossotgr砒e 玭
llrne to do eatrietlocag obosatst right now1
ㄳ／～軌 perhaps no mote than 50 adults luff its wtld areas nIh
r nda Famhm
Plors& the n빠cube bUt elusive Flondo Pa＇漱set (Puma c이
PemaPg .ne .fthe moat endasagered 叩ecies in th8 wotiJ
governmental ageneses have joined forces to help keep the
tietoeboto E出＞sts have focused on restori낑genetso 出ver,
population by ssnportsssg 8 Texan cossgars os 1995, and on
soUls cars by budding underpasses below岫ways that p.s
&aindhaghabitOts sciessbsts believe nsat use山Out an eEfecin
plan, 比e Flonda Panther will disappear from the wdd w虹
,nant Paster Otter The Giant River Otter (Pteronura bsssshensis) so a rensarka
aaveiasg iv goispe of4.9 called 'bolts', headed by a mona.....
tonally also carrspnsasg oevnsalgenvratons of offspring. Th= j
---－∼－1

1. positon:abs이ute；를입력한다（세미콜론을
잊지 말자）
.
2. top, right, bottom, 또뉘諦를 입력한다．

多 3. :v를 쓰고 γ자리에는 요소의 부모 요소로부터

kins live
＝〕

Fte

요소의 절대적 포지셔닝하기：

[-

'iㅍㅌ 'asocce－뗀ㅍ

.2랖 14.8 이름들은 문서의흐틈에저완전하 벗어나 있고 오司려
description 걸의흐틈과같55/ 가는것처럼보인다. 명확하겨7
설정되아 았자 않은 들여쓰7／나 (JW 경우에는오른쪽 , 왼쪽，
그리고 맡부분ㅇ／다夕 만일 절대적으로 위차 자정아 안되어 있는 경우
꾜소가 원래가겼어아 하는 위치로부C7 나온다．

파생시키고자 하는 요소까지 원하는 거리를
넣는다. 이것은절대값또는상대값으로표현될
수도 있고 (lopt 또는 2em) 또는부모 요소의
퍼센티지로서도 표현이 가능하다．
4. 필요에따라；
（세미콜론）
을쓰고부가지시에
따라 2번과 3번을 반복한다.

'/ 1iP`
■ 부모요소에관한것은p179를참조한다．
■ 절대적으로포지셔닝된요소들은문서의흐름으
로부터 나오기 때문에 그들은 서로를 또는 다른
요소들을 가끔 오버랩한다（이것이 나쁜 것만은
아니다）
.
■ 만일 절대적으로포지셔닝된 아이템의 파생을
정하지 않았다면 아이템은 그것의 자연스러운
에 나타나지만 결과로
위치（여기서는 헤더 다음）
나타나는 아이템에는 영향을 미치지 못한다

예珊의소스 코드는 wwar cookwood.com에 있습나다．

193

！。驪＝ 。三＝ 山쓰． ㅋm= ＝客m。 百 흐

a림14.7 여가서는 9픽셀을 사용하여 네임아 intro요소와 같이
정렬될수 있도록 한다. 다폴트 값아라면 아깃은 브라우저의 왼쪽
빈공간으로 9픽셀만큼 갔을 것이다．

===== PAGE 183 =====
182 =====
（小apter ] 4

요소의 높이와 넓이 설정하기

二츳 cl1l柚. C$$

picture {display:block}
population {display:inline}
latin_name {display:inline}
more_info {display:inline}
그림14.9 넓이룰 적절하 조절함으로써 절을 앍기 쉽게 만들 수 았다．

요소의 높이와 넓이 설정하기：

'/ 1iF*
■ 넓이 특성의 퍼센티지 값을 사용하는 것은 약간
애매한 면이 있다. 예를 들어 RI꺼江L을 사용할
때 50％의 의미는 원래 이미지 사이즈의 반이라
고생각하기 쉽다. 그러나 이것은 원래의 이미지
사이즈의 넓이와는 상관없이 부모 요소 넓이의
절반을 의미한다（부모 요소에 관한 더자세한
사항은p179를보면 된다）
.

194

J
s〔예》

Rt耘므出

소
Home

%n'낫，

The 可）
心，
씨a and plants on rise planet are diaappeasu琨 atom ailartna떰rate. I六
unto to 飾 something about it sight now'
Flonda P繃出er Withpedsaps no mace 仕lar1 5D ad'긔tneft m 'arid areas ，寸
Son나'Weston, F노ssda, the mn)estse but elusive FIanda
Panther［工'ama roncolor 0O5)1) iS perhaps one otthe
most endangered species st the world Grass roots aid
governmental agen口e$ have jomed &roe. St나尸’ l …
the pan由er 什Dm extm000ct E汪이ts have f.口
restoring gersntsc diversitym甘｝
e mwP아iolah
importing P Texan cougars in 1995, and on avo,dss5
accidents 印比 carS b，
갸 1．
교dsng csnderpasses below
higliavays that pass thsruajs these dwindling habitats
Scientists bcheer 1hat Without an e汪ective manageflielt
plan, the Florida Panther cecil disappear from the sndd
`mdml 25 years
Giant River Otter The Giant Rices Otter (Pteroaura brasthntaie) is a
renlarkably socsal pasan出，bavebng tn 8Co.-,PI ef48
attic크 "h LSt. hr꺼ㅟ on 〕nnn 'oasn"sa rose and U71신1·
；
＝」

2. hei餉탸1를입력한다. 여기서h자리에는요소
의 높이가 들어가게 되고 절대값으로만 표현
가능하다．

카 5c1stissanthn..1el - Missosati Internet Eeptoer,
15,-ass, 1ooii deis
／ㅊ

1. wic洲：w를 입력한다. 여기서 w자리에는요소
의 넓이가들어가게 되고, 이 값은 절대값으로
표현되거나 부모 요소의 퍼센트값으로 표현될
수 있다.

坐立닙比
『祗〔

*
·
m
｀ 。*士七多느。 主 읗 ㅈ ·＝*m= =
*＝·ㅌ으띱＝ 口

우리는 대부분의 요소, 즉 이미지와 폼 요소, 텍스트
블록을 포함한 요소의 넓이와 높이를 설정할 수
있다. 한 페이지 안에 같은 사이즈의 여러 요소들이
등장하게 되면 그들의 높이와 넓이를 동시에 설정할
수 있다. 이런 정보는 브라우저로 하여금 필요한 만
큼의 적당한 공간을 옆으로 정렬할 수 있게 하고 따
라서 나머지 페이지를 - 일반적으로 텍스트이다 더 빨리 보여줄 수 있게 된다．

」

endangered_species {di剝ay:block}
name {display:block;position:absolute;left:9px}
intro {display:block}
description (di숴ay:block;position:relative;
left:125px, width:340px}

石iJii活k

그림14.10 넓이틀 조정했을 때 설명 부분은 더좁아졌고 ㄷ／알아
보가 쉬워겼다．

===== PAGE 184 =====
183 =====
Layout with CSS
口
code.css
endangered_species {display:block}

보더 설정하기

name {display:block;position:absolute;left:9px}
intro {display:block;border:medium doffed red)

작성자는 요소 주변에 보더를 설정할 수 있고, 그것
의 두께 스타일이나 색을 설정할 수 있다. 만일 패딩
을 정했다면 보더는 그 요소의 패딩과
(p196 참조）
컨텐츠를감싼다．

-

description {display:block;position:relative;
left:125px;width:340px;border:thin solid red)
兩cture {di咐ay:block)
population {display:inline}

보더 설정하기：

latin_name {display:inline}
more_info {display:inline}

1. 뇨rder를입력한다．

그림i4.끄 여7/서는 단치보더스타일만아 요구된다. 원한다면
위치, 두께, 색을첨가할수았다．
}I tces\panllse,s s.sl - M,c,osall maniac, Espinie,
y"V냇

FayoOes

Toils

HB노

J

〕

slip

R繃esh

3. 다시 공간없이 :（콜론）
을 입력한다．
，,,

:Toe animals sod plants on 010 pluors are thaappearmg at ass 幽rnurig ease
: 1六 time to 巍 something about it right nowl
'品汕Yass;e}

G1ant 拓ver Otter
～山

니

위Dos.

Pernai>5 n. tn.
of Southwestern Flonda. the usajestie but .h'i've
Florida Panther (Pumna coucotor coxyi) a pethaps one
0f出e m0$t essda의tered species inshe world Graus
roots and governmental agencies have joined forces to
help keep the panther from extiucisoni E汪oils have
fbrused .n eestosstg genetic dversity nl the bny
pop미anon by in'oetil芭 8 Texan cougars in 1995, and
on avoids叱 accidents w姓L cars by budding underpasse
below highways tha댜sass tlsro哮mle,r dwindling
hihtaie, sr1·nh寸＄ beheve th.t W宜h0ut a』
1 s丘esbve
masiagement plan, the 듸onda Panther w,끄 disappear
from the w1ld within 25 years,
r이arc brsoiheniisl is a
一 衡白e코1굵a叱t

그림14.1.2보더는 텍스트 블록의 한겨7를 정한다．

4. 필요에따라보더의두께를정하기 위해서thin,
medium, 什Iick 또는 절대값 (4px와 같은）
을
입력한다. medium값은 디폴트값이다．
5, 보더의 스타일을정하기 위해 n이ie, dotted,
dashed, solid, double, groove, ridge, inset
또는 .utset을 입력한다．
6, 필요에 따라C이or를쓰고, color자리에는16색
이름 (p251 참：조)의 하나를 쓰거나 p200에 표현
되어 있는 것을 입력한다．

·／ nPS
■ 작성자는 개별적인 사항을 보더의 어느 부분에
라도 정할 수 있다. 예를 들면 border-leftwith용i:5를 사용하여 왼쪽 보더의 넓이만을
정할수 있다. 또는 border-color:red를 이용
하여 lㅖ 개의 사이드에 있는 색깔을 정한다．
보더 스타일에는 20가지의 다른 특정이 있다.
border-style (border-top-style, borderright-style, 7]타), border-color (border, border-width (bordertop-color, 7J타）
top-width,기타）그리고 border (border-top,
기타）등의 종류가 있다．
■ 만일 보더의 색을 정하지 않았다면 브라우저는
요소 컨텐츠에서 정의된 색깔을 사용할 것이다．

예제의소스 코드는 www.cookwood.com에 있즙나다．

】95

·．＝言芬● 日。 쿄
e
m

-

s螺

丘d궈

紬

H꿱，

EIs

2. 필요에따라·top, -bottom, 仙 , 또는－ru이it
如『der 다음에 빈 공간 없이）입력한다. 이것은
보더의 위치를 지정한다．

===== PAGE 185 =====
184 =====
다iapter 】4

요소 주변에 패딩 더하기
패딩은 이것이 의미하는 그대로다 ; 요소의 컨텐츠
주변은 여분의 공간이지만 보더의 안쪽은 살집이
붙은 산타클로스의 배와 같이 그 벨트 (the border)
에 의해 둘러 싸여져 있다. 패딩의 두께를 정할 수는
있지만 색이나 섬유 등은 정할 수 없다．
요소 주변에 패딩 더하기：
1. padding을입력한다．
*＝●름。 ＝ ＝ 口 ， =＝。，4…m

2. 원한다면·top, -bottom, 卄또는·right,
@adding 후에 빈 공간은 없다）
를 입력하여
padding을 객체의 한 면으로 제한한다.
3. :x를 입력한다x자리에는첨가하려는만큼의
양을 넣는데 이것은 워d으로 표현되어 있거나
부모 요소의 퍼센티지로 표현되어 있다.

표츠 code.css一

iij

「呼m菖

endangered_species {display:block}
name {display:block;position:absolute;left:9p차
intro {display:block;border:medium dotted red;
padding:5px}
description {display:block;position:relative;
left:125px;width:340px;border:thin solid red;
padding:5px}
picture {display:block}
population {display:inline}
latin_name {display:inline}
more_info {display:inline}
을
그림14.13 패딩은 경계와 텍스트 사아에 공간（여기서는 5팍셀）
넣는다．
】F:kna1H,sa` hots.e,sd - Minsosolt latrines Esplo,er
i出 브.va Fita5rs 工ode 브e中

J
;t가

n
Rine劾

」
Hone

V Tips

The anna,粃 and teas. : :` q그：; 노山H ‘￡尸『뇨apoeassua at ass aiatrras.g n｀汁
.5六 time In do nomedang abutit n 以잦료n…니

■ 패딩값을 설정하는데는 여러 가지의 숏컷이
있다.padding: trbl을 사용하여 top, right,
bottom, left 값을, 각각의 값을 분리하고 있는
공간과 함께 이와 같은 순서로 동시에 설정할 수
있다. 또는 padding: v h 위에 있는 값과 밑에
있는 값을 동일하게 하거나 (V) 오른쪽이나 왼쪽
나padding: 나山
값을같게 할수도 있다. (h）
을 설정하고, 왼쪽과
를 입력하여 위의 값 (t）
오른쪽의 값을 하나의 값으로 (h) 정하고, 그
다음 밑의 값을 설정할 수 있다. (b) 또는 padding: a를 입력하여 각사이드의 값을 정할수
있다.

Flnitda Panther

Jll』
므 人上』

■ 값들은 절대 값이나 부모 요소 안에서 상응하는
넓이의 퍼센티지로 표현될 수 있다.

196

」』1JJ

』」」JJJJJ

l」』」上 1ㅢ

cdi perhaps cc more then 51 adult; left a weld as eat 1
of Southwestrrse Florida,由esoajeitc butelusive
11
orida Panther (Puma concolor cory is perhaps one翩
ofthe eawit endangered speciesmthe wodsil Grass "
Hots and goverrassental agencses have joined forces tot
nip keep the panther thorn entinctoer Ffforta have ㅐ
ocuted on restoemg genetic diversity as the tiny
冒
opulaton by importing 8 Tessun cougarsm 1995, ass시
에avoiding accidents with carsbybudding
derpsssns below lsinjsseays that pass through tlsosr
effective
esnrnt
plan, the Fl。
rida
Panther
ovtthoutwill
an
dwin,dlingmatsn。
habitats
S,cientist艀eve
that
!dseappesr&omthew1dwltlim25 yeart

!

Gtint 瓦ver ㅇflov

그람 14.i4 빨간색의 부분은 겋겨／ 안의 패딩을 나타낸다（아것은 아
.
책에서만 색깔을 가지고 있다）

===== PAGE 186 =====
185 =====
Layout with CSS
口》de1c$$ 트－

드1

돈」

endangered_species {display:block}
name {display:block;position:absolute;left:9px}
intro (disploy:block;border:medium dotted red;
padding:5px;margin-top:5px}
description {display:block;position:relative;
left:125px, width:340px;border:thin ＄히id red;
padding:5px;margin-top:5px}
picture {display:block}

의 바깥쪽에서 요소
마진은 어떤 패딩 (p196 참조）
주변의 경계 (p195 참조）
의 하나의 요소와 그 다음
요소 사이에 있는 투명한 공간이다．

population {display:inline}

2, 필요에따4-top, -bottom, -left또는·right를
입력한다 (margil, 이후에는 공간이 없다）
.
이것은 공간이 어디에 첨가되어야 하는가를
한정한다．

그림14.15 단아margin에 top, bottom, left, right룰 더하여상자
한사이드의 마진을 설정한다．
jF\c,i\panthe,i soil b45usio11 lsle,nvl E,qsto,r,

rd

i The animals and plants 예 ourplasatr are Jssappearm0【1ㄴ山 alaioiang late
= 1ta tine to do somethi咀 about it rt助t now'
!
Florsda Panther
w洽i per岫：)s no more thai, 二0 vdult, 1ea m wild neat
of Sou山western FksodaJh0 maJestic bate胞1ive
Honda Panther (Puma concotor corn) is perhaps .one
.r仕Ic most endanger仕dspecies Inth. w.dd Graso
roots and governmental a8toots huse jusied forces L,
heb keep뇨 pa汕set from eitosction Efforts have
focuted .꿋1 eestoilltg genehc 山Versi竗 m 山e t=ny
labm냐＞y m叩oro喀 8 Texa』
】
c(）
꺾garS nl l995』ard
Pㅇ】：川』
에 avoiding accidents wi出 curs by buildhig
undespasses below highways tba쟈）
asS t1ieOU2J5 their
dwhoflir떰hshutnts, Sruesstists behest 山at wit玩ut an
e汪rc000 management plan, the F柚td心n沮1or wil
disappear from dIc wild w咐in 25 yeart
盼ant F그Jer ^m·

1

驪므sari 뇨，
巴 갸te= PI-c c: i hraouhenssi 心 a

「yn

그랖 14.16 마진을 첨가하는 것은요소 사이의 공간（꽤당차럼그
안쪽아 아나다숏을 늘아는 것이다．

요소의 마진 설정하기：
1. margin을입력한다．

3. :x를 입력한다. x자리에는첨가되기 원하는
만큼의 공간의 양이 유닛으로 또는 부모 요소와
상응하는 값의 넓이의 퍼센티지로서 표현된다．

V Tips
■ 또한margin: t r b I을사용하여 top, right,
bottom, left 값을 동시에 각각의 값을 분리하고
있는 공간과 함께 위와 같은 순서로 설정할 수
있다. 또는 margin: 나1 위에 있는 값과 밑에
있는 값 (V）
을 같게 할 수 있으며 또는 오른쪽이
나 왼쪽 (h) 값을 같게 할 수도 있다. 또는
margin 나ib를 입력하여 위의 값 (t）
을 설정하
값
(h）
으로, 그
고 왼쪽과 오른쪽의 값을 하나의
다음 밑의 값을 설정할 수 있다. 마지막으로
margin: .를 입력한다. 여기서 a의 자리에는
모든 side에 사용될 값이 들어간다．
■ 값들은 절대 값이나 부모 요소 안에서 상응하는
넓이의 퍼센티지로 표현될 수 있다．
■ 절대적으로 위치가 설정된 상자 안에서의 마진
값들은오프셋 특성 - top, bottom, right
그리고 left 佃93 참고，
）를 갖고 정해진다．

예제의소스 코드는 www.mokwood.com에 있습L／다．

197

松 ＝ ＝썹추* 글口매口菩斗● ＇口｀ 口
＝ ＝●클● 三

latin_name {disploy:inline}
more_info {display:inline}

陋〔

요소 주변의 마진 설정하기

===== PAGE 187 =====
186 =====
（十apter ] 4

요소 주변에 텍스트 감싸기
작성자는문서의 나머지가요소들을오른쪽, 왼쪽
모두 감싸게 하기 위해 요소들을 정의할 수 있다．
다른 요소 주변의 요소돋 감싸기：
1. float：를입력한다．
2. 만일 왼쪽의 요소와나머지 문서를오른쪽으로
흐르게 하고 싶다引eft를 입력한다．

'/ 1iPS
■ 정리된요소의 넓이를정하는것을명심하자．
■ 작성자가선택한 명령이 정리하고 있는 요소에
적용되고 그 주변에 있는 요소에는 적용되지
않는다는 것을 명심하자. float:leh를 입력한다
면 문서의 나머지 부분은 오른쪽으로 흐르게
되고 그 반대의 경우는 반대로 흐르게 된다．
■ 요소 사이에 어떤 것들을 흐르게 만들 때는 유동
적인 요소를 흐름이 시작되어야 할 지점 바로
이전 컨텐츠의 앞에 넣어야 한다．

그림耳17여기서는side-bar타입의 blurb요소를XML문저에
첨가했다．

口

巨

t0de, c$$ 蓼…

endangered_species (display:block}
name {display:block;position:absolute;left:9px}
intro {display:block;border:medium dotted red;
podding:5px;margin-top:5px}
description (di利ay:block;position:relative;
left:125px;width:340px;border:thin solid red;
padding:5px;margin-top:5px}
blurb (float:rigth;width:125px;
border:thin solid green,padding:5px}
picture (display:block}
population {display:inline}
a림14.18 여가저는 오른쪽 blurb를 흐르겨）설정했다．
＇skims
`F: \ct,',prmrrhesiblo,bsml . Mjc,o.oIt tnte.eot【月

4』
.ack

YnetY 「크V예e'
-

-

h」
i be4)
口
s心》

끄
RJre寸｀

尸nil,

Edㅎ 〔da

ㅐ玖，

;The ansoals and plants on our planet arc 'sappvarosg at as, olartsun rate
나 's sane to do sornetlung about it ri isrsowi
Fhnda Panmer

乞 的냉

W沚｀perhaps no more dian 50 ad毗 1e且 'B w正4 areas
of Southwestern Ftoe,da, dis majestic bU소 elusive
Honda Panther (Puma conroloe
'Without ari
cozy,) is perhaps one ofthe most
亡匹손？t`ve
elldangreed species m the '7.rld
roassagemene Pla』
＼
Grags roots andgovernmezstal
the Fkoda
a8msirs hare J.】ne4 forces to
Panther ,.,ll
help ksep the pan仕Ler from
disappean 니祉』
l
entinesoto E汪Orts have foconed
25 \re露r` "
on rests,,,,g 8efletic 出otrs止y ㅍ1
出e tiny P.Pdataunbylrnpothng 8 Texan car갬art as
1995, and on avoi函ng cccidcots wsth ㄷar5 bp bu,td岫
tasdespasseg bslow h띵hways 籬at pass 寸'routh 山吐

ㅍa1i5.-r F－區．

그림14.19 텍스트 블록을 띄우는 것은 주의를 집중사카슨 좋은
방법이다．

'98

＝」

콜
=＝●ㅌ으W七＝ 긍 놉 * X山hm＝ 횰 。 느

또는 오른쪽에 있는 요소와문서의 나머지를
왼쪽으로 ㅎㄹ게 하고 싶다면 righㅎ를 입력한다．

이｝
de.Is [

<description>With perhaps no more than
.cpopulation>50</population>adults left in wild
areas 0f Southwestern Florida, <blurb>"Without on
effective management plan, the Florida Panther will
disappear within 25 year."</biurb> the majestic
but elusive Florida Panther <latin_name>(Puma
concolor coryik/latin_name>is perhaps one of the
endangered species in the world. Gross roots
and governmental agencies have joined forces to
help keep the panther from extinction. Efforts have

===== PAGE 188 =====
187 =====
Layout with CSS
…흩

텍스트 감싸기 멈추기

mde. csS =

endangered_species (display:block}
name {display:block;position:absolute;left:9px}
intro {display:block;border:medium dotted red;
padding:5px;margin-top:5px}
description {display:block;position:relative;
left:125px, width:340px;border:thin solid red:
padding:5px;margin-top:5px}
blurb {float:right; clear:right; width:125px;
border:thin silod green,padding:5px}
picture {dispkiy:block}

다른 요소들（텍스트와 같은）
이 스타일시트 주변에
흐르지 못하도록 스타일시트 안에서 특정 태그로
표시할 수 있다．
텍스트 감싸기 멈추기：
1. clear：를입력한다．
2. leh를 입력하여 왼쪽 면의 모든 요소가 없어질
때까지 흐름을 멈춘다．

population {display:inline}
latin_name {display:inline}
more_info (display:inline}

또는righㅎ를 입력하여 오른쪽 면의 요소들이
없어질 때까지 흐름을 멈춘다．

뺘q.

`FIn홈｀
` paniheachimb cml M,n,oioft lnteamt hap佃·
＇
h*

*
SI아〕

Pd【eats
-

工was

〕

소

H이m

Se sh

The animals and plants on our 힌oneS are disappeanng at an aiarntmg rare
It's Sure to do sonnetha堪 about Its낳It nonet
FiondaPasather

w咐1Perh町is no more than 50 adalts it且 m wild areas
C·fSou小wentem Plostda. dit m司colic but thieve
L止 h/1
r ' n七1 I LIt!.벼 r上겨1r11a 니，
싸ndl0ut m1
rOt) Is perhaps 01St .：】fdit mess
effcrtsve
-isdangeted species m the wml l
mana呂easieSt plan,
뇨a5'roots and government出
the F1.nda
唯encies hnot jomed forces t(
Pa曲er an
h日아seep the panther from
由sappear wes恤
P:=mcoon Eiforts have fC〔u5뻐
25 years '
」n reeton退 atenetlc 小riertl.' ti
出 hnyP야》
따alm.a by impelm堪 8 Tetian cougars sn
1995' and 이，
a'. ldus8 accidents nit甘1 cart by brsiid也
mdespaoves below highways ma쟈sass through thee
和 Lord 01,500

그림14.21 익스플로러 5는 clear 특성을 자원하자 않는다．빨간
색으로 표사된 텍스트는 사하드바의 끝부분 아래부E7 시작하차는
.
않는다 ("the tiny populationtm에서 사작된다）

또는 both를 입력하여 두 면이 깨끗해질 때까지
흐름을 멈춘다．
또는 none을 입력하여 흐름을 계속한다．

'/ nPS
■ 만일 확률이 반반인 퀴즈 게임을 좋아한다면
“시스틴 성당의 천지창조 벽화에 등장하는 하나
님과 아담은 어느 쪽 손을 들고 있을까？”와 같은
문제를예로정하는것도좋겠다.（미켈란젤로의
천지창조 벽화는 서로의 손가락을 맞닿은 것으
로 신과 인간의 연결을 묘사하고 있다 - 역주）
:
여기서 clear:rig卜t를 사용한다면 오른쪽이사라
질 때까치텍스트 흐름을 멈추고 싶다는 것을 의
미한다. 엉뚱한 말이지만 퀴즈의 정답은 왼쪽이
확질해보인다.
■ 확실한 스타일의 사용은 IfrML에서 clear
속정에 br 태그를 쓰는 것과 같다．
■ 윈도우의 익스플로러 5에서는clear 속성을
지원하지 않는다（그림 14.2p.

예제의소스 코드는 www.cookwooci.corn에 밌습나다．

]99

꽝섬｀ =
．
뻐
m
X
* 是a볍

그림14.20 만일 animal의 완쪽에흐르는 것을 원하차 않는다면
clear: right를 첨가한다．

===== PAGE 189 =====
188 =====
Chapter 14

배경 색상 조정하기
사용자는 수평 라인을 포함해서 폼 요소들과 테이블
요소 등의 색상을 조절할 수 있다．
배경 색상 조절하기：
1. C이or：를입력한다．
2. colomame을입력한다. colorname자리에는
16개의 미리 정의된 색상중
（'p251참조) 하나가
들어간다．

endangered_species {display:block;color:magento}
name {dis이ay:block;position:absolute;Ieft:9px}
intro {disploy:block;border:medium dotted red;
padding:5px;margin-top:lOpx}
description {di制ay:block;position:relative;
left:125px;width:340px;border:thin solid red;
padding:5px;margin-top:5px}
blurb {float:right; width:125px; border:thin solid
green,padding:5px;c히or:black}
picture {di泂ay:block}
population {display:inline}
latin_name {display:inline}
more_info {display:inline}

또는rgb (r, 9, 비를 입력한다. r, g, b는 원하는
색상 안에 들어 있는 red, green, blue의 양을
0 - 255의 정수를 이용하여 표현한 것이므로
0 - 255의 정수가 들어가게 된다．

그림且22 color 특성은유전되jZ또 여기저는루트 endan
gered_species 요소 안에서분홍색으로 색장을 정했기 때문
에모든 요소들은 다른 식으로 (blurb에겊은색으로 조정을 가혔i
던 깃 같이）징하ㅈ］
않는 이상분홍색으로 나올 것아다．

또는rgb (r%, g%, b%)를 입력한다. r, g, b는
원하는색상안에서 red, green, blue가포함된
양을 퍼센티지로 표시하면 된다．

蛋F 'c!' \,dnito,s55a,bunsl - Hic,o.n55 Ins 1,1,i F,atI, rei

·／ 1iPS

4J
.
8a：』（

→

■ 만일r, g, b의 값에 255보다큰정수를넣을때
그숫자는255로 대체된다. 마찬가지로 100%
보다 큰 퍼센티지는 100％로 대체될 것이다．
■color 특정을 이용하여 텍스트의 색상을 조절
（'p217참조7.
할 수 있다
■ 이미지의 배경 색상을 조절하는 것은 아무런
효과가 없다（이미지 편집 프로그램을 이용해서
. 그러나 투명
이미지의 색상을 조정할 수 있다）
한 부분을 통해서 보이는 부분의 색상을 조정할
수 있다. 더 자세한 정보는 p201에 나오는 배경
색 바꾸기를 참조한다．

2OO

＝〕
Rtheih

“

;Tht asarnalu and plants 》n os.ir planet are disappeansig at an atannutig rate
:li- B lime to in Borne吐ate about it at dst tow
비 nda rann1er

■ 색상을 정하는 더 자세한 사항은 부록 D의 Hex
색쟝을 보면 된다．

J
戮여〕

5臭

ESe 트出 Y比빔 pasones 工mis 브eb
니

H쉈，

，。＝U, ＝긍늠● ，오● 솥m= `＝口＝ U

또는＃rrggbb를 입력한다. rrggbb 자리에는
원하는 색상의 16진법의 표현이 들어간다．

de. c $ 裝饔甕箋鐄囊蕁늦羨昇－뜨프町弓

委日毫뜨

With PedlapB ISO li-lOre 吐ma 50 ad미tneft m odd areas
.f S.udtwestern Flotsda- shB maiesflc卜it elusive
Randa Panther (Puma concoler
c이y川t perhapi one 硼出e most
endangered species m the WoolJ
GTans roots and 8ovesnmrntal
）
agencies have joined forc en t」
hrip keep the panther from
eotuscbOfl Ethosts have kcissed
0n reston낑genet1c 出verssty d1
the tiny populatson by nnporss땅 8 Tecian cougars iii
四95. and on avoiding accidents with cars by b뗘duo
onderpasses below S哮표ways that pass through then
dwsndlmg habitats Scientists beheve 小atwsthosit a끄
effectine managemens Plan. 仕｀e F}.ndaPanth'rwsll
山sappear from 小. sndd w漱m 25 ye可r

그림14.23 또한工刃弧兀 안에서수평으로 된 규칙,form 요소，
테이블 셀 등의 색상을 바꿀 수 았다．

===== PAGE 190 =====
189 =====
Layout with CSS
鄧i르쓰一즈多쥬拓彗쩍 cl〕
d.．【SS --4=－寸琴囊贊三＝乙 슴目三

endangered_species {display:block;color:black;
background:url(pantherlight. jpg)}

배경은 모든 페이지의 배경을 의미하는 것은 아니고
특정 태그의 배경을 의미하는 것이다. 다른 말로
하면 요소 - 이미지 폼 요소, 테이블 등을 포함한 의 배경을 변화시킬 수 있다．

name {display:block;position:absolute;left:9px}
intro {disploybock;border:medium dotted red;
podding:5px;morgin-top: lOpx}
description {disploy:block;position:relative;
left:125px;width:340px;border:thin solid red;
padding:5px;morgin-top:5px}
blurb {float:ri帥;width:125px;border:thin solid
green;padding:5px;color:black}
picture {dis이ay:bloc놔

배경색이나 이미지 바꾸기：
1. ㅄckground：를입력한다．

population {display:inline}

三F \csS',pn1h, rst,l,sl, ,,e,l Minsanoul leir,nol lopintis

With pediaps no more than SC au1dio le且 in wild fleas
硼 S.｀心］western FIosda, 出e St可CiSc but elusive
Plonda Panther (Pans conoolso
cosys) 0 perhaps one of the 55050
endangered species nl 出e woold
Gvan roots asid govenmeit甘
agencies have jointd forces to
뇨elP keep 小e Pm甘tee front
e껍5501505 Eㄸ
｀rts ha口e focuted
onrestoring genetic divers好 m
the bny P.Pu核son by l1껴殄itm名 8 Te驪an c.唾ar5 n1
}99하 and on avoiding acc泌sits w轍 cnn by husldmg
tindetpasses bets,싸嫩wavs thu냐7ann tksasjs their
dloin必righabitati Sd`entists bd1ree that w醜out an
e侄votive inSiSt乎sites plan, the Florida Pan仇en tell
如appear 丘sm 由r wild W沚an 25 years

Giant 瓦ve, Qtter
The Giant River Otter (Ptercnsien beanihensti) ii a
1 l 山toeali*anet

3. 필요할경우un (image.gif)을입력한다．
image.gif자리에는 배경으로 사용하고 싶은
이미지가들어간다．
repe이을 입력하여 이미지를 가로와 세로로
붙일 수 있게 한다. repeat-x는 이미지를 가로
로만붙이게 한다. repeat-y는 이미지를 세로로
붙이게 한다. no-r이：》eaㅎ는 이미지를 붙일 수
없게 한다．

Tbe asaalt* a iJ下）
lanti on 口町 Pi缸比t are 由sap9eanng at an alasming ratr
It's sire to dii something abaut it rajit nowl

면」乫）며”

2, 필요에따라ㅎransporenㅎ 또는color를쓰고
color 자리에는 foreground에서 정의된 색상을
입력한다 (p200 참조7.

fixed 또는 $cr해을 입력하여 배경 이미지의
위치를 설정한다．
여기서 x와y는 퍼센티지 값이나 절대 거리로
표시된다. 또는 吻）
, center, bottom 값을 x로
사용하고 /eft, center, right를y로 사용한다．

-늬

그림14.25 만일 배경 아마자를 사용한다면 배경색아 그 위에 있는
텍스트와 살 대바되는자 주의하자

'/ 1im
■ 첨가된 이미지처럼 하기 위해서 배경 이미지를
picture 요소에 적용할수 있다. 셀렉터 안에
＃을사용하여 이미지를특정 picture 요소에
제한한다．
■ 만일 배경을위한색상이나URL을정한다면
색상은 URL이 로딩될 때까지 사용될 것이고
이미지의 투명한 부분에 적용될 것이다

예제의 소스 코드는 www.cookwood corn이7 있습나다．

201

우。 ＝뱀＝ .*＇· ．。숫역。 ．
＝
ㄴ

그림14 24 이마자의 파일 이름은 인용 부호가 아난 괄．
흐와 같이
나온다．

Fk'rtda꾸ndinn

배경색 바꾸기

===== PAGE 191 =====
190 =====
Chapter 1 4

지금까지는상대적／절대적 위치 정하기에 대해서
살펴보았다. 이것들은2차원문제, 높이에 관련된 것
들이다. css는 3차원（깊이）
에서의 위치를 정할 수
있게 하고 따라서 오버랩 될 수 있는 요소를 조정할
수 있다．
3차원으로 요소 위치 지정하기：
1. z-index：를입력한다．

。m= =＝●ㅌ·＝m灌＝ 욘…

2. n을입력한다. n자리에는축적된 객체 안에서
요소의 레벨을 지정해 주는 숫자가 들어간다．

i- c
（》d. .cS$

―ㅁ

3차원으로 요소 위치 지정하기

endangered_species {disploy:block;c히or:black;
background:url(pantherligh니pg)}
name {display:block;position:absolute;
left:9px;z-index:-11
in솥ro {display:block;border:medium dotted red;
padding:5px;margin-top: lOpx}
description {display:block;position:relative;
left:125px, width:340px;border:thin solid red;
padding:5px;margin-top:5px}
blurb {floot:rigth; width:125px;
border:thin solid green,padding:5px}
picture {display:block}
population {display:inline}
latin_name {display:inline}

'/ nPS

morejnfo {display:inline}

■ z-index가높으면높을수록축적된요소에서
그것은 높은 위치를 차지한다．

그림14.26 이것0/ bottom-most꾜소가 될 깃아라는 것을확쟐하
하가 위해저 z-index에음수를사용한다．

■ z-index에서는양수와음수를둘다사용할수
있다．

U EIe

`r

}l

\'g`ponlhv,abln,I, sort M,coovtl Inh,onrt [aplo,o,
l出

+4
8m火

freas
'

→

F立vmt,o
'

5oal.

:a
-

5k.

Ceb
-

n

R甘
『m},

仝
H며00
-

皿
oev卄
.'

J

sloandPIris O55O5KP】
asSet 0ie 出oappeavrngat ass 出asvomg rate
닌 do something about it m낮It flown

。
m
｀

With perhaps n. 1nOre th棚l 50 adalto !eftmwd meat
of Southwestern Flonda. 出eat司tins bm etu翩｀'e
hlonda Panther (Piana c이1c이娜
cony) is pethars one of the roost
亡ndm，
욤·r뉩d 차》eciev at th. w.dd
Gran. roots and gOVtlTitoeot出
agencies bave Jouled forces to
h탸P keep the panther from
eX山5cnOc E匠otis have 如custd
m re計O5mg gerotic 士ettorSy nl
tSr b呵 Pott미anon by n꺽》O1tn也 8 Texan coogaro Ul
竹
md on avoids,팜 accidents ot心scars by b曲drng
undespeasea beI.w Iisways that pass 仕．
ougts thro
dwaidling뇨bitats Sciectorts beheve 小at Withoot an
effective inisiagtowns ploo. me Fto,sduP.sttsersssfl
1甘l래叱t

그랖 14.27 Flonda Panther 텍스트는 자금 안쪽에 있다. 왜나하면
이것은 배경 아래 았기 때문아다(p201그림14.2꽈 바i22

202

===== PAGE 192 =====
191 =====
Layout with CSS
！그

세로로 요소들 정렬하기

= "} de

endangered_species {display:block}
name {di剝ay:none;position:absolute;left:9px;
z-index:가
intro {display:block;border:medium dotted red;
padding:5px;margin-top:5px}
description {display:inline;width:200px;
border:thin solid red;padding:5px;margintop:5px; vertical-align:top}

만일 페이지에서 똑같은 방식으로 정렬되기를 원하
는 요소들이 있다면, vertical-align 특정을
이용해서 요소를 조화롭게 보일 수 있다．

picture {display:none}

2. ㅄ｀dmne을 입력하여 부모요소의 베이스라인
을 가지고 요소의 베이스라인을 정렬한다．

population {display:inline}
latin_name {display:inline}
more_info {display:inline}
저는 아름과 picture 요소를숨衲十 또한(description
박스의 넓이를 작게 만들어서 박스들은화면이）
서저로 장 정렬되ㅇ7
있다．

禱，

,

lbe anmmsr and P1ants ml .ur F4tnet 祗e 如 potrsegat Soc liamnngra5.
Ifs time to do something tbout lt n蜘t yowl
edca恥 no more 寸'an 50
J`dtsbi仕 m wild sweat .f
0u仕'western F柚da, d止
majestic but elusive Flotida
Panther (뇨na conrolor cosys)
op_ 야s one 0fthe m0鮮
enduseered species m 안比
弘onId Gruss roots and
government滋 agencies have
sled forces to hlip keep 由e
panther frome磁nc5010 E枉ortu
have focused 0n restore堪
8eneso 由unit,汐 m th. hny
popcdalson by mpostosg 8
Tcxix Cougars a, 1995. and

또는 sub을 입력하여 부모 요소에 관해 아래
첨자로서 요소의 위치를 정한다．

또는 te雜bp을 입력하여 부모 요소의 위를
가지고 요소의 위를 정렬한다．

5끼

R-

轍

또는 mid비e로 부모 요소 가운데로 요소의 가운
데를 정렬한다．

또는 $uper를 입력하여 부모 요소에 관해서
우측 상단 첨자로서 요소의 위치를 정한다．

FAc몬5`Par간1erㅎ 'mj H노r.ㅎ머1 Ins이ml rmisses
rp i O Y- F'7agec hO. bop
litnp

1. vertical-이ign：을입력한다．

琿be 臼ist l <1ver 0flee
αeromoy bruadienorn) si a
remarkably social axial페
treoeh＇唯 n1以oups of4-9
called b1毗s5, headed by a
monogamous r`a且 and situ쾨J卜7
Sic compnnng severm
字r'eratsons of祗opsss客 They
hlint, groom and cc就 t08ether.
Nid hson 9 voca뇨ations for
cOfnrnomoatsng A끄d with
出cjr ca'l big an Aoar onda.
.ley are no mulch for hunsu.
itho have broughlthemtnthe
br
『4r r,f*,:T뱄1cbd1 Thnre are

臣難證纛暾.

또는 text-b이torn을 입력하여 부모 요소의 밑을
이용해 요소의 밑부분을 정렬한다．
또는top을 입력하여 줄에서 가장 높은 요소의
위를 가지고 요소의 위를 정렬한다．
또는 b이torn을 입력하여 줄에서 가장 낮은
요소를 갖고 요소의 아래를 정렬한다.
또는 요소의 줄 높이의 퍼센티지를 입력한다.
이것은 양수 나 음수에 구애받지 않는다．

囊뱀LocS eu,aesi

그림耳29 이러한두 7//9/ description 박스（여〃저는 다른

'Tip

모든조각들을 숨겨서 아딴 것도 상차즐을 분라하자 않는z譏는 그들

■ 인라인요소는세로로정렬해야만한다（각각의
라인에서 시작한 요소들을 세로로 정렬하는 것
은 안된다）
.

의제일 상단모서라에 맞춰서 정렬되어 있다．

예제의소스 코드는 www.cookwood.corn에 있습나다

203

브c三＝ 山쯔m크m＝ 잖 ＜
。 ＝＝흽i

그림14.28 인라인 요소를세로로 쟝렬할수 밗에 없가 때문에 여가

텍스트 위치 정하기：

===== PAGE 193 =====
192 =====
다tapter 】4

초과분의 행선지 결정하기
으로 그것의 컨텐
만일 높이와 넓이 특성 (p194 참조）
츠보다 작은 요소 상자를 만든다면 초과되는 컨텐츠
는 어딘가로 이동해야 것이다. 당신은 초과분의 특성
을 이용하여 이 행선지를 밝혀 줄 수 있다．
초과분의 행선지 결정하기：
1. overflow：를입력한다．

ㅌ ，·＝。
。。끄긍云놀。 ＝
느
· 占 쁜 ● ＝多m灌＝ m

2. visi비e을 입력하여 상자의 콘텐츠에 맞도록
요소상자를확장한다. 이것은디폴트옵션이다．
또는 Hdden을 입력하여 요소 상자에 맞지 않는
컨텐츠를숨긴다．
또는＄cr해을 입력하여 스크롤바가 요소에 첨가
됨으로써 초과분의 컨텐츠에 접속할 수 있다．

·／ nP
■ 만일 초과분의 특정을 정의하지 않는다면 초과
된 컨텐츠는 요소 상자의 밑으로（오른쪽 아래는
아니다）가게 될 것이다. 이것은 텍스트에 높이
를 부여하는 것이 간혹 쓸모 없게 보이는 하나의
이유가 될 것이다．

肛量

1: code.css

團？

endangered_species {display:Hock;color:black;
background:url(pantherlight.jpg)}
name {display:block;position:absolute;left:9px}
intro {display:block;border:medium dotted red;
padding:5px;margin-top: lOpx}
description {disploy:block;position:relative;
left:125px;width:340px;border:thin solid red;
padding:5px;margin-top:5px; height:300px;
overflow:scroll}

blurb {Hoat:rigth;width:125px;
border:thin solid green;padding:5px}
picture {di制ay:block}
population {display:inline}
그림14.30 높아를 제한한초과분의특정을 적용하는 것안아 맞는
즈：）아다．
` Ftc8`\psnlheiebhs,b ,si- I4rc,onott Intcn.el EnpIoe1

눴

，‘

m回口

y,esl F,vvles !osli 蜘b
.

-

.j
S1叩

」〕
R甘‘母낙，

2t
緻eel

Sc.nrh

The aerosols and plants en ate pl000tUIe 如appestasft at an m帥m咆 ra:t
工r$ tone t0 d. assnething 앍》otett轍t now!
日）
nda Panther

Gl繃 River ㅇtter

由

w砬 pediafl no aDore than 50 a伽lts left te
ar'as DfSnuthwefleen Ftar,aa. 出e ma〕e5bc but
eleeiee Fkssdn Panther (Porno
c0nc해or coo,이 O PCIhos's
one of the volt esiJotsgerrd
species to the world, GraS5
roots and gOvenmnvfltu
ag目soses have y刈1ed fircet to
he辦 keep dle panther 什cm
e,an,05.ors Effoits have
sciosed on rertonna geneOg 山teen孕 anthe row
popmasian by typomvs 8 Texen COUO!1 UI l95.
andon al:,出叱 accidents md1 car零 by b祉du1g
'andeipossee below lt甘tease that pass thres甘 thee

l1se aa11s River Otter (Pteronwo bra吐tnoso) is a
canoek棚y g0며님 a佃m쿄，eaveitigin groups of4.9
』

婆g Lasd Itynelt

그림14.31 만일 텍＝트:1/ 높아플 모든 텍스트가보이깊 않게 졔한
한다면 나口／지 텍스트에 접근하가 위q서스크롤바를 졔공하는 것도
하나의옵션이다．

204

===== PAGE 194 =====
193 =====
Layout with CSS
\:7醬｀多

code.issg

요소 클리핑하기

endangered_species {displby洲ock;c히or:bla吐；
background:url(pantherlight.jpg}
name {display:block;position:absolute;Ieft:9;
background:white;clip:rect(5 80 15 20)}
intro {display:block;border:medium doffed red;
padding:5;margin-top:101

사용자는 요소의 특정 부분을 나타내는 창을 만들 수
있다. 최근의 창은반드시 직사각형이지만 미래의
css 버전에서는 다른 모양도 가능하게 될 것이다．

desc야)tion {display:block;position:r이ative;
left:125; width:340;border:thin solid red;
padding:5; margin-top:5;height:300;

1. 내p:rect
（를입력한다．

요소 클립핑하기：
2. tr니을입력한다. t, i , b, 1자리에는보여주고
싶은 요소의 직사각형 부분 위, 오른쪽, 아래
그리고 왼쪽 좌표를 표시한다．

overflow:scoll}

blurb {Iloat:rigth; width:125;
border:thin solid green,padding:5;color:black}
picture {display:block}

Paris

,

elm

J〕
Reham

仝
itara

즌＼

■ 오프셋값사이에는쉼표를첨가할수없다는것
을 기억하자．

nPy此戶仁h』．b )n니

The asrisss幽 arid plants on oar planet are 缸appraseag at sir alararsig rate
Ifs rime t口 do something about it right now
with perhaps no more than 50 adnilta letS m rvdd
areas of Southwestern Florida, the no司casio be
elusive FIends Panther α‘urina
mnc이0r cos3nr) 1s PenhaP$
one of the roost enda堪ered
5Pe口eg m山e w.dd Grags
roots insd goxermuentat
agencies base joined forces t0
help keep the Pa끄小es horn
extraction E1:fvita have
s-oursd 叱 restoring genetic 由versity 끄1 the tu,y
population by sopor勿堪 8 Tenors cougars ri 1995,
and on avoiding sod`dtrite With cars by b出drig
undespasses below 3鱗o'ays that pan through their

邕 Dora

V Tips
■ 커런트요소는요소를클립하기 전에 절대적인
위치가 지정되어야 한다 (p193 참조？.

驪F.Ocsa5punihersbissb.smi - Hinsossil ieir,net Eaplass,
드Sr gsa fan FoovOr, ho He如

o,dae.ㅢg' n

3. ）을입력하여 마친다．

■ 오프셋값은절대값（3px）또는상대값（3em）
이
될 수 있다．
■ 클리핑은요소의 컨텐츠에 영향을주지 않는다．
이것은 패딩과 보더를 숨긴다．

→－〕

■ 클리핑은월드와이드 웹 컨소시엄에서 재검토
에 들어갔다. 이 책을 읽는 동안에 바뀔 수도
있다．

1
The GiantRiver,Otter(Fteronusabrasshenrrs)
Ian ㅢ =J
玉姦＝蕉

ig b0oO enniaver

=z림14.33아작클랍의孑은사용을찾지못했다. 좋은제안은환영
한다．

예冽의소스 코드는 www.cookwood.com에 있습나다．

205

스甘｀ ＝口。 ＝쯩킁二4

그림1王羽 여가서는 name 요소의 배경을 환색으로 바꾸섰다．
clip 특정의 결과를 더잘볼 수 있을 것이다．

===== PAGE 195 =====
194 =====
（小apte시4

리스트 특성 설정하기

口

정렬되어 있지 않은 리스트를 위한 것에는 여러 개의
기호 표시 스타일과 번호가붙여 있는숫자 스타일이
있다. 이러한스타일을리스트스타일특성을가지고
포괄적으로 설정할 수 있다．

<xsl:sMesheet type="text/css" herf="Iists.css" ?>
<Iists>ezanimal>
<name>Florida Panther</name>
<threats>
<threat>Habitat Loss, Fragmentation, and
Degradation</threat>
<threat>Inbreeding</threot>

돋留－

또늬ower-al캬1.를 입력하여 알파벳 소문자를
사용한다 (a,b,c,기타）
.
또는 뱌가)er-이pha를 입력하여 알파벳 대문자
를 사용한다 (A,B,C,기타）
.
또늬ower-roman을 입력하여 로마수의 소문
자를사용한다．
또는 upper-roman을 입력하여 로마수의 대문
자를 사용한다．
또는 un (image.gif)을 입력한다. 여기서
image.gil는 리스트의 표시자로 사용하기 원하
는 이미지의 URL이다．
4. 필요에 따라.utside를 입력하여 표시자를
리스트 아이템의 왼쪽에 위치하게 한다. inside
를 입력하여 리스트 아이템 안에 있는 모든 라인
들을 가지고 표시자가 왼쪽으로 정렬되게 한다．

?>

춈 F oc,.opseihe,ast asS Msa,osoft intssnos Esplo,.,
트台

4J
的CS

5aes
.

F크V(s, ,s

→

目回口

多

I-ta2 닌뺘
J
Sk中

」
Ri's얽1

.3.

드：
屯

H콘.

또는decimd을 입력하여 아라비아숫자를
사용한다 (1,2,3,기타）
.

하고 요소에 이［7］又］를 삽입해야 한다. 그리고 텍스트 안에서보기를
정해주어야한다．

』rL』riclu 노 a11轍e!
Habstat Loss, Fraissentatiosa, sad Degradstson Inbreeding Disease Insufficient
Large Prey Meectay and Other Environmental Contanunants Insetamsssal
Cons打a』
』났8 PU씨iC Perceptsons
Gtaut FasCO c」杜er
Habstat Lass Heavy Hunesg Mercsay passon1g from gold stoning Poi (oon
丘m끄 白sot flint entruction I뇨t」
rbanee fran나ounttv O"rrshmd (de짇ens
fㅅdsurr:s. 노Secb
＇【；놔｀ Masse dsttr,nner 'ml
；街 ㄴma1姓‘이柏〔

Done

그림표3阡炸瀷 익즈플로러는 display:list-item -／착을
자원하차 않는다. 따라서 xML 문서 안에저 라스트들을 제대로 보여
줄 수 없다（加7p의그림14.38).

타e

Osolla bBuild ID 200＂【〕8［】7`?}
듣e,,出 as B 如1 心

＇回口
He

5l닐e:llIF:Iss* E5,eulst／『헤 쾨－ 1
勿

1囊的매如 什Seas
m1」
a Pmm八

.

包日긔1S밈

日呵＇m

〔1l,ss,sffln,ent Large Prey
"
ㅓ

心

Merceny and Other Sits roanaesst出 Contor,onaaits
'

i

Rentm
「s돠ni岑J꿇比＇J四
,

그림14.37 넷스커7아프 6 이전 바전은 아마자 가호 표시륭자원
하지만 안정되어았자 않다．

206

小d1

Lots. Frs nesstansn, sad Dr可sdabon

囹Habstst

또는 square를 입력하여 하나의 사각을 사용
한다．

그림且弱 threat 요소를 라스트 아이텡으로 보7/로 정의해아

Inbreedasg

또는 circle을 입력하여 비어있는 원형의 써클을
사용한다．

red}

threats {display:block}
threat {display:list-item;
Iist-style:url(minipanther.jpg) inside}

囹Disease

3.

m
==
흐＝ 。
｀
。
，
`
*
셥“
*
·
＂

리스트 아이템 속성을, 원형의 끊김 없는 써클에
설정하기 위해서 disc를 입력한다．

0

-咨결히黨 code.css｀캬∼＝＝蚣노M：룩＝=3=＝상눗目츨

lists {display士)IOCk}
name

2. 다음刪ist-si닌e：을입력한다．

"

그림14.34 여刀에는 라스트들의XML 코드가 았다．

{color:

1. displa叫ist-item：을입력한다. 요소가리스트
로서（블럭이나 인라인이 아닌）보여져야 한다는
것을 알려 준다．

1.

<?xml

리스트 특성 설정하기：

陋

一二－∼：二＝뇰 1汁）d..1m11 궉……
version="

===== PAGE 196 =====
195 =====
Layout with CSS

■． '/ Tips

趨Pa1卄h机Li.t Mic,o.oU Inte,n.O E,pIoer,
i出

恥UV

FbV히요e'

」畔

YJ
'

J肛*

구

s吻

.3執

·I可.

小누
-

E屯

〕

Re1
【eq,

소
Hero

功
Seoch

」 夕Go

Aoaj〕
F,-P찮HmmI
Ftodda Paidher

駐，
：』Hab,tat Less, Fragnaeotases, arcd DegrHdsDos

[.J Iesbreedacg
덖 恥ea5e
絡；』Ll5uffieseest Lurge Prey
dOther Euv,ronmeestuj Contam,naests
E:：』Mercexy철，

g;j I tsthenuiCens5ernts
Pub뇨Percepteons
Gh"1 Ri` er ntier
鈿 L.c이 v닙노α탭

그림 楓38 익스플로러는 ff

문서에서 아것을 오i아ㅇ／템에 적용

예젱의소스 코드는 www.cisokwcod.com에 있습나다．

■ 불렛을위한큰이미지를사용한다면, outside
값을 들여쓰기를 적절하게 만들지 못한다. 그전
에는 inside가 더 좋다．
■ list-style 특성은list-style-type,
list-style-image, list-style-position으로나누어진다. 이러한것들은유전된
리스트 스타일의 개별 관점을 무시할 때 유용할
것이다. 그러나 대부분의 경우 list-style만
을 사용하는 편이 쉬울 것이다．

207

m
. ==.=＝珊。 ｛m빽4rm

하는 한 list-style 특성과는 어파한문제도 일으7／ㅈ／ 않는다．

■ 익스플로러는IfI取1L문서의 리스트들을지원한
다（그링 14.38). 그러나 이것은 현재까지 dis헨’列ist-item을 지원하고 있지 않기 때문에
XML 문서 안에서 무엇이 특정에 적용되는지는
알 수가 없다．

===== PAGE 197 =====
196 =====
다tapter ]4

어떤 시점에서 방문자들은 웹 페이지를 프린트할 수
도 있다. 대부분의 브라우저들은 페이지 설정 대화
상자 안에서 방문자들이 선택한 종이 크기에 가장
잘 맞게 자동으로 페이지의 컨텐츠를 조절할 것이다．
CSS2로 방문자가 프린트할 때 페이지의 어느 부분
을 나눌 것인지 정할 수 있다．

주어진 태그 후에 페이지 브레이크 정하기：
page-break-after:always를 입력한다．
주어진 태그 전에 페이지 브레이크 정하기：
page-break-before:alway＄를 입력한다．
·＝。인m● m
。 ｀m＝ 二경● 유

페이지 브레이크 없애기：
page-break-after:auto나 page-break-before:
aut.를 입력한다．

208

릍衢느七是七七t勿긴＞大컥ㅋ＝七븍괍뜅댜 code.css 즌드三三＝三＝三三汪흐묘鞭匹뜩

lists {di制ay:block}
animal (page-break-ofter:always}
name

{color:

페이지 브레이크 정하기

red}

threats {display:block}
threat {display:list-item;
list-style:url(minipanther.jpg) inside}
그림珏39개별 animal 요소 다응에는페아자브레이크가
반드사 았어야 한다．

===== PAGE 198 =====
197 =====
15

FORMATFING

TEXT WITH CSS
css로 텍스트 포맷하기

XML 문서에 css를 이용하는 것은 빈 종이 위에
그림을그리는 것과같다. XML 요소들은HTML
태그와는 달리 디폴트 포맷팅이 없기 때문에 텍스트
가 필요로 하는 모든 특징을 정의해야 한다．

209

m
。 ，클。 ＝=．뻐mX4트呻＝ ＾以

스타일은I{I取4L 태그와확장자가 했던 것보다 많은
가능성을제시한다. 여기서는사이즈무게, 경사, 줄
이나배경색, 여백 그리고
높이, 전경 (foreground）
텍스트의 정렬 등을 바꿀 수 있고 또 텍스트의 하선
이나상선의 유무 여부, 그리고 대／소문자로의 변환
이나 문자의 사이즈 등을 결정하는 법을 살펴보기로
한다．

===== PAGE 199 =====
198 =====
다lapter 15

폰트 가족 선택하기

릎m示‘+

모든 사람들이 같은 종류의 폰트가 아니기 때문에
font-family 속성은특별한특징이 있다：첫번째
선택한 폰트가 방문자의 시스템에 사용 불가능 할
경우 하나 이상의 폰트를 정할 수 있다. 작성자는
일반적인 폰트인 세라프와 모노스페이스와 같은
폰트를 정함으로써 방문자의 시스템에서 나타나는
상황을 조절할 수 있는 최종 시도를 할 수 있다．

intro, description {font-family:Georgia, Times, serif}

一一一＝」二詔：一三무code.tss 蕁i긺二

name {font-family:Trebuchet MS, Anial, sons-seril}

그림15.i 여기서 ㅇ／떻거7조자아폰트 가족을 (Georg)a font family)
intro와 description 요소들의）적용했는치 알수 있다仁／
자제한사항은p180의복잡한셀렉E／를참조한다t

Z七W

mY미甘e1 工0th !jek)

J

끄

《크

5t야）

R甘
（e寸，

ㅐ아麗

只，

E紀 i*

폰트 가족 선택하기：
1. fon나amily:拓．
洲yname을입력한다. family
끄ame 자리에는 첫번째 폰트 선택이 들어간다.

＝
。
，
。
m
= =g占
＝겯口， *

2. 필요에따라，
familyname2를입력한다．
familyname 2 자리에는 두번째 폰트 선택이
들어가게 된다. 각각의 선택은 쉼표로 구분한다．
3. 필요한만큼2번을반복한다．

'/ nP$
■ 적어도두 개의 폰트 선택을하는 것이 좋다. 그
중 하나가 일반적인 폰트라면 작성자는 문서에
관한 조정 능력을 가지게 된다. 맥킨토시 시스템
의 일반적인폰트는세리프를위한타임체, 팔라
티노체, 산스세리프체를위한헬베티카체이다．
대부분의 윈도우 시스템은 타임체를 포함하나
산스세리프로서는 Anial이 더 보편적이다．
■ 어떤폰트가사용될지에 영향을주기 위한마지
막 시도로서 다음의 일반적인 폰트 이름들을
사용할수 있다 - 세리프 (serif), 산스세리프
(sans-serif),커시프 (cursive), 판타지 (fantasy) 그리고 모노스페이스 (monospace).
■ 일반적인 폰트 스타일을 이용해서 폰트의 가족，
폰트 사이즈, 줄 높이를 한 번에 설정할 수 있다．
■ 자요소들은 그들의 부모 요소로부터 폰트의
가족을 유전 받는다．
■ 인용부호（작은, 큰）
들은요구사항은아니다．
그러나 이것들은 어떤 브라우져들이 공간을
가지고 있는 폰트 이름들을 이해하는데 도움을
준다．

21 0

apsno 기
n pe먀，
ed areas of 90나：
「r一
majestic but 이solve Fl 1
Panther (Puma cm,C이∼
ccl
coryu S rerhap$ 이，
most end.incer너 gDe

k. Sued ci, restoroig genetic 山flersitu m 由C
tiny population by importing 9 Texan cougars
灌fl 1995, and on avoiding accidents with cars
by building underpasses below highways that
pass throu함｝their dwindling habitats.
Scientists believe that wi다tout an effective
m050gemout plan. 냐to n츤rids por,타1nr 헤］
物 1sed e*,ea

그림15.2조자아폰트가 블러브 佃urb) ll 다사 사용되었다는 것을
주목한다. 요소들의부모로부타 폰트 가족이유전되었刀 때문아다．

===== PAGE 200 =====
199 =====
Formatting Text with CSS
뇰町

c`1de.c1$

페이지에 폰트 첨가하기

@font-foce {font-family:Trebuchet MS;
src:url(TREBU어0.eot)}

작성자는 원하는 어느 폰트나 선택할 수 있지만 방문
자의 컴퓨터에 폰트를 설치하지 않았다면 폰트를
읽을수 없을 것이다. 페이지에 폰트를 첨가하는 것
이 이 문제를 해결하는 방법 중 하나이다．

@font-foce {font-fomily:Georgia;
src:url(GEORGIA0.eot)}
name {bn나or洲y:Trebuchet MS}
intro, description {font-family:Georgia}
그림15.3 첨가된파일로의 경로와폰트의 정확한 아름을사용8梏
것을 주의한다．
`

m回口

F.`c! -ieKiCparihe,abio.b.mI - Hmo8oii inteinel E,,ploiei
Ee
如
【

翩

y"W
-

F호부.寸已二

工m丸

J

sm.

페이지에 폰트 첨가하기：
1. @fon나ace{fon나amily：을입력한다．
2, 첨가하고자하는폰트의 전체 이름을입력한다．

닌出〕

」〕

RJreoh

仝
恥os

3. ; src:url(을입력한다．

ㅙ

gem쟎노

4. 폰트의 UEL을입력한다．
" nre disappearing at an
. oi.ing about 헌' 1…t 卜 nC무기

*甘h = 느m 'n^ m뷔 '` ` 1 미．
1』쑤．
*汁1.;-

^n

11尸 `n-

그람15.4 적절한폰트는 trebuchet나Georgia가설차되어 있자
않은 ㅈ／스템에서도 보여질 것아다．

5. I｝
을입력한다．
6. 필요한만큼의 스타일 정의를 위해 2번으로
부터 폰트 이름을 사용한다．
'/ 1iF'S
■ 첨가된 폰트 (4번）
를 위한 소스로서 아무 폰트나
선택할 수는 없고 폰트의 특별한 포맷을 사용해
야한다. 인터넷 익스플로러는 .eat 포맷 안에
있는폰트를요구한다. 작성자는 설치된 폰트를
WEFT라는프로그램과함께 .eat로 변환해야
한다. 더 자세한사항은 www.rnicrosoft.corn
/typography/web/ernbedding/을 본다．
■ 비츠트림 (Bitstream）
사는넷스케이프나 익스플
로러의 웹 페이지 안에 폰트를 첨가하게 만드는
웹 폰트 메이커 (Webfont Maker）
를 개발했다．
이것은 윈도우를 위한 익스플로러에서는 좋은
성능을 보이는 것 같지는 않다（맥킨토시를 위한
익스플로러에서도마찬가지다）
. 자세한사항은
地p://ww .bitstream.corn/webfont/를 참조
한다．
■ 인용부호가공간이나특이한구두점을포함한
폰트를 몇몇의 브라우저가 이해하는 데 도움을
주는 것에도 불구하고 인용 부호 표시는 폰트
이름 주변에 요구되지 않는다．

예쩌7의 소스 코드는 www.cookwocxt corn에 있습나다．

211

m크口뙨독＝ .m。 ＝＝。＝。，。口m

' … ' .0 nomoretho.
wild areas of SOUthwesteri,
majestic but 이seine Fk'rh!
Panther (Purso ,
,
coryD is pe卄그 치
most endanger : 'F，
ㅍㄴ
the world. Grass room as i
governmental agenvies
hay이nined forces to heir
keep the pandicr from
extmcLi0n. Eflorts hav츤．
focused on restoring genetic diversity in the
tiny P)pulation by Imlxirting 8 Texan cc.ugarr
in 1995, and on avoiding accidents with cars
by building anderpasses below highways that
！」크sn through their dwindle밞iabitatn.
1ent1sts b슨heve d,at without an effestive
,onagement plan, the Florida Panther will

===== PAGE 201 =====
200 =====
Chapter 15

이m릭체 민튤기：
1. font-st코e：을입력한다．
2. oblique텍스트에는아小que를입력하고, 이탤
릭 텍스트에서는iidIC을 입력한다．

@fon나ace｛拓ntfamily:Georgia; src:url(GEORGlA0.eot)}
name {font-family:Trebuchet MS}
intro, description {font-family:Georgia}
latin_name {font-style:italic)
그림15.5 여가서는모든 latin_name 요소를 아탤락체로 보여
주가를 원한다．
}

b뇨d) ,ml - Mic,o,ofl
【，
F \c脈＇e났｀Panthe

! tb 트a yi.. F,eus 工o, b沖
픈

Rorida Panther

2. normal을입력한다．

V Tips

를 없애고싶은 이유는부모 태그로부
■ 이탤릭처］
터 이탤릭체로 유전된 절 안에서 어떤 문장을
강조하고 싶을 때이다. 더 자세한사항은 p179의
유전된 스타일을 참조하자．
■ 자요소들은그들의 부모요소들로부터 fontstyle을 물려받는다．

212

j
s'야1

도〕
P m괆

,

h

Witi니)erhaps no more than 50 adults left in
wild areas of Southwestern nor,da. the
malestic but elusive Florida ∥Wi甘out an
Panther r／뇨ma coccolur
effectiVe
'·S/iI n in Perhapt one of 나'C manegement
most endangered species in plan, the
the world. Grass roots and Florida Panther
governmental agencies
w미 小sappear
have joinin卄orces t아'S坤
within 25
keep dte panther from
years."
extinction. Efforts have
伽used on re敢oring genebC diversity in the
tiny population by importing 8 Texan cougars
in 1995, and on avoiding accidents with cars
by building underpasses below highways that
pass through their dwindling habitats.
Scientists believe that without an effective
management 비on, the Florida Panther will
=j

m上三 ·＝＝口● ｀U

1. bnt-st인e：을입력한다．

■ 만일폰트스타일로이탤릭을설정했는데사용
가능한 이탤릭 스타일이 없는 경우 브라우저는
oblique 스타일로 표현한다．

畔

The animals and planta on our planet are diaappearing at an
祉armuig rate. ks time tod0 somethin8 about it dght no＼이

이탤릭체 없애기：

■ 폰트의 이탤릭 버전은 아무 것도 없는상태에서
폰트 디자이너에 의해 만들어지는 과거의 방식
인 반면에 oblique 버전은 컴퓨터에 의해 만들어
지는 것이다. 이러한구별은 사실 명확하지는
못한 것이지만 일반적으로 통용되는 것이다．

凹

s斗，

이탤릭 포맷을 하는 두 가지의 방법이 있다. Garamond Italic 또는 Palatino Ita끄Ic（또는 그밖의 것）
을 폰트로서 설정하는 방법 (p210 참조7이나 처음
폰트를 선택하고 (Garamond 또는 palatino) 다음
에 이탤릭을 선택하는 방법이다. 만일 주어진 폰트
안의 텍스트 전부가 이탤릭으로 쓰여져 있다면 첫번
째 방법이 간단할 것이다. 그러나 Roman이나
Itallic체의 경우에는 두번째 방법이 보다 유연한
방법일 것이다.

＝쩡髥 code.css
口
아ont-face {font-family:Trebuchet MS;
src:url(TREBUCHO.e에}

澈．

이탤릭체 므蠟기

i콩仇’c

！늬 L叱y1,1r`m1

그랖 z丘6 이탤락은 텍스트의조각을 강조하는 아주 훌륭한 방법
아다. 특하 와국어로 쓰여진 단이의 경우에는 더욱 그렇다．

===== PAGE 202 =====
201 =====
Formatting Text with CSS
D

＝二聲Code.c$5- -

j

@font-face {font-family:Trebuchet MS;
src:url(TREBUCHO.eot)}

볼드 포맷은 아마도 텍스트를 눈에 띄거 하는 가장
보편적이고 효과적인 방법일 것이다. 스타일 시트들
은 볼드 텍스트를 가진 선택의 범위를 제공할 것이며
상대값을 제공하고 한번에 이것을 없앨 수 있는 범위
를 제공할 것이다．

@font-foce {font-family:Georgia;
src:url(GEORGIA0.eot)}
name {lont-family:Trebuchet MS;font-weight:bold}
intro, description {font-family:Georgia}
latin_name {font-style:italic}
population {font-weight:bold}

볼드 포맷 적욤하기：

그림15.7 텍즈트를 깅조하는 다른 일반적인 방볍은 볼.i체를 사용
하는것아다．
i 「＼"1teX뿔｀
｀】a1낚J1e1gb'u1杜Xm' Mic,o,oa ] sa.net E쎄）
』여er

눋

트m

恥w
나

F1voae,

工며놔＄

J

Sap

·回口

닌dp

」〕

Ren'놔

H窺，

트k

With perhaps no more than 50 adults left in
wild areas of Southwestern Florida the
majestic but 이calve Florida "WIthout an
Pand}er (Puma ooncoiar
effective
evryi:l isperhaps one of the mm1agernest
moot endangered species in pIan,탓le
the wㅇrk」
. Grass roots and norida Panther
governmeflt出 agencies
will disappear
have joined forces to help
within 25
keep the panther Irons
year8.'
extinction. Eff0rt計｝
ave
focused on restoring genetic diversity in the
枕rsy population hInmporting 8 Tesan cougars
in 1995, and on avoiding accidents with cars
by building underpasses below highways 싼sat
pass through their dwindling habitats.
Scientists believe that without an effective
management plan, the Florida Panther will
r

臘imd1自1닐

그림15.8 여기A-/ name(F7orjda Panther)과 population
(50) 요소들온 훨씬 푸렷하다. 그래서 앍가가 쉬워진다．

1. font-weighㅎ를입력한다．
2. b이d로서보통의볼드weight를텍스트에줄
것이다．
3, 또는bdder또늬ighter를입력하여사용되는
weight의 상대값을 사용한다．
4. 또는100과900사이의 100의 배수를입력한
다. 여기서 400은 책의 무게를 나타내고 700은
볼드를 나타낸다．
볼드 포맷 제거하기：
1. font-weight를입력한다．
2. normd을입력한다．
'/ 1iF*$
■ 무게가정의되는방법은폰트마다다르기 때문
에 값들은 폰트마다 상대적일 수 밖에 없다．
그들은 주어진 폰트 가족 안에서만 상대적이게
디자인 되었다．
■ 만일 폰트 가족이 9 weight보다 적을 때 또는
그들이 스케일의 한쪽 끝에서만 집중되어 있을
때는 어떤 숫자 값이 같은 폰트 weight와상응
할 수 있다．
■ 자 요소들은 그들의 부모 요소로부터 fontweight 특정을 물려받기 때문에 자 요소들이
너무 볼드체같이 되지 않도록font:wei이it:
normd을사용한다．

예제의소스 코드는 wwpi. cookwood.com에 있습나다．

213

君 三 도 ＝ ．四。 ＝m닉크。 ＝=.

The animals and plants on our planet are disappearing at an
alarmix好 rate. It's time to do something about it right now'

듣lD뎌叱

볼드 포맷 적용하기

===== PAGE 203 =====
202 =====
Chapter 15

폰트 사이즈 결정하기
특정 요소로 표시된 텍스트의 폰트 사이즈를 부모
요소의 포인트나 픽셀의 정확한 사이즈, 설명 또는
상대적 사이즈를 지정하는 것으로 정할 수 있다．
폰트 사이즈 설정하기：
1. bnt-size：를입력한다．
2. 절대 폰트사이즈：xx-sm애. x-sm혜. sm베，
mediumJarge, x-large 또는xx-Iarge를
입력한다．
또는 상대적 폰트 사이즈Jager 또는 $mailer
를 입력한다．
또는 정확한사이즈】2pt, l5px를입력한다．

별！拓＝三편

…三兵三舌기－룸三陋=

1＝눋一릎 code.csn ∼ r

@font-face {font-family:Trebuchet MS;
src:url(TREBUCH0.eot)}
@font-face {font-fomily:Georgia;
src:urllGEORGIA0.eot)}
name {font-family:Trebuchet MS;font-weight:bold;
font-size:24pt,width:100;margin-top:10}
intro, description {font-family:Georgio;
font-size:10pt}
latin name {font-style:italic}
population {font-wei前t:bold}
그림15.9 name, intro, description 요소들의폰트 사ㅇ］
즈를 설정하는 것과는 별도로 여가서는 name 이본문과오버랩돠는
것과mtro와 충돌하는 것을 막기 위해서 name 요소의 윗마진과
넓이를 (p194와p197) 쟐정해주었다. 텍스트의사아즈를바꿀때
레이아웃 요소들을 변화시카는 것은 일반적이자 않다．

v' Tips
■ 숫자와유닛들사이에는공간이 없어야한다．
■ 상대적인값（larger, sma끄er그리고퍼센티지）
들은 부모 요소의 사이즈와 함께 계산이 된다．

:The an,mals and platen on oar더anetIre. sappearing at an alarming
: rite. Itv tniue to dotomethiogaboutit right now1
perhaps so more than 5o adult引aft in wild

the w.rid. Grant rOOt$ ㄻd
plan, the F卜rrida
goveronsental agced1er have
Panther will
b mnwnbroes to help keep the
dmuappearwi탸nn
Fan卄1er from extinction. EfEDrt5
25 years.'
mSe bossed on restoring
genetic diversity m the tiny pot싸atlon by im凶rting
S Texan vongare in l9,51asd .h avO`dn,g adddents
with oars by building enderpasses helow highways
that pans through their dwindling habitats. Swienttstn
believe that without an effective management plan,
the Florida Panther will disappear from the emld
within up years.

■ 다른폰트 값과함께 폰트 사이즈를 설정할수
있다．
■ 자요소들은그들의 부모 요소로부터 fontsize 특성을유전 받는다．

Giant

The Giant River Otter (t'mmaniara busthstsi&iu a
an.imal, traveling is groups of a-u
remarkably so. cial」
called h。
lts,
bya
P.iver 。ttersj
.

jcant

그림五刃 name 요소는 여가서 더 돋보인다．

214

:
:

With
Florida areas
of Southwestern Florida, them키antic but
elus,ne F뇨rida Pan轍Cr α，ssm
"Winiout an
ranrnJareo17e)ie perhaps one of effective
Panther the
most endangered species in rnanagement

bcaded

●겊m* ＝。，●솥m= =*●m

또는 어느 특정 요소와의 상대적 크기를 입력
한다（예：150%),

===== PAGE 204 =====
203 =====
Formatting Text with CSS
튿．
;=======＝三J

口ld.. c$$ 羞긺

므」

@font-face {font-family:Trebuchet MS;
src:url(TREBUCH0.eot)}

라인 높이는 절의 leading을 설명하고 있다. 다시
말해 절 안에서 각각 라인 사이의 공간을 말한다．
큰 라인 높이를 지정하는 것은 본문을 읽기 쉽게
만든다. 헤더의 작은 라인 높이는（하나 이상의 라인）
그것을 고급스럽게 보이게 한다．

@font-face {font-family:Georgia;
src:url(GEORGIA0.eot)}
name {Iont-family:Trebuchet MS;font-weight:bold;
font-size:24pt;width:100;margin-top:10;
line-height:22p寸
intro, description {font-family:Georgio;
font-size:10pt}
latin_name {font-style:italic}

라인 높이 설정하기：
1. line-heigh＇를입력한다．

population {font-weight:bold}
그림拓．
끄 1 mne-height족성은 라안 사
（)］에 있는leading과
공간을 결정한다．
牙F:\sssI.`ltpantheehkab.,,st Mis,osett tntr,snt Espte,r,
Ek

i-a. Ym'

F

令
ㅐsme

4

With perhaps no more than 50, adults left in wild
FLorida areas
。fS。
uthwestern Pl。
t-ida, the rca
Ic but
Florida PunthCr (Passe
Panther elusive
'Withㅇut an
eeneelmrerpslm perhaps one of
...

o什ertive
me most endanger슨d species in
managemext
the world. Grass roots and
PIan, dto Florida
governmental agencies have
Panther will
joined tom.es t. halp keep the
disappear within
pan小or from entiuction. Efforts
25 years.'
hare focuued on reuturing
genetic小varsity in thetinypoPulation by It까icc山坦
EISoxan cougarsix Sf95, andes avniding accidents
텡1th Car$ by buslding underPamen below higheaps
tha냐》
ass 比It-OURh 仕1e1r dwin出Ing habitatv.ScionhOs
disappear fr。m
the wild
believe
the
Fl。
rida
thatPanther
without an
willeffe畿
management
plan,
within 55 years.

口.

n1eGiant Pover Otter (Ptosxrnee bsseelieesie)is a
remarkably social animal, traveling.in gmnups生스：
且
m。
n。
gam。
us pair
andby a
15t1al1y
called
headed
i,

hunt,sr。
。m,an퇴
Giant
River Otte

鉀，?，胃：므쁜．쀼購＝，뻑
ra,1 ㅜ뇨, U rest together,andl ㅟ
'holtn,

Giant
River
Otter
也Dun

그림15.12 큰 사아즈 텍스트는 다소 빽빡한 라인 높아일 때 더보가
좋다 (p214의그림15.10과 비교2

叩제의소스 코드는 www.cookwooci corn에 있습나r궈

I, 1iF小
■p216에 설명된 폰트 가족 (font family), 사이즈
(size), 무게 (weight), 스타일 (style), 이형
(variant) 등과 함께 라인 높이를 정할 수 있다．
■ 라인 높이를 결정하는 숫자를 사용한다면 이
요소는 모든 자 아이템들에게 유전될 것이다.
만일 퍼센티지를 사용한다면 결과 사이즈만이
유전될 것이고 퍼센티지는 유전되지 않는다．
U line-height 특성은 그들의 부모 요소들로
부터 자 요소들에게 유전된다．

215

==．추m= ＝●＝욤＝

또 를입력한다. a는포인트나픽셀등의
절대값이다．

:The animals and plants on our planet are disappearing atari alarming
=rate.ltd tim카edo something about it right uowl

．
盼

口
Rehe놔｀

2. n을입력한다. n자리에는원하는라인높이를
얻기 위해서 폰트 사이즈에 의해 곱해진 숫자가
들어간다．
또는p％를 입력한다 여기서 β는 폰트 사이즈의
퍼센트이다．

브e如

」4

라인 높이 설정하기

===== PAGE 205 =====
204 =====
태apterl5

동시에 모든 폰트값 설정하기
폰트가족, 사이즈, 무게, 스타일, 이형 등을한 번에
설정할 수 있다．
모든 폰트값 한 번에 섭정하기：
1. bni:를입력한다．

@bnt-face (font-拈mily:Trebuchet MS;src:
url(TREBUCH0.eot)}
아on나ace [bntfamily:Georgia;src:url(GEORGIAO.eot)}
name {font:bold 24pt/22pt; :Trebuchet MS;
width:100;margin-top:10)
intro, description (font:10pt Georgia)

2, 필요에따라normd, 이)lique, italic들을입력
하여 폰트 스타일을 설정한다 (p212 참초7.

latin_name (font-style:italic)

3. 필요한경우normal, bold, bolder, Ii이iter
또는 100의 배수 (900까지）
를 입력하여 fontweight를 설정한다 (b213 참조？.

그림15.13 적어도 font 특정에서 폰트 가족과폰트 사하츠는
항상지정해주아야 한다. 모든 다른 특성값은 선택사항《）］다（명확
하게 설정되어 있자 않은 경우에는 다폴트 값으로 간주된대．

*
0
m
。
， -<m= =
0
＝ 。*口旨크모* ＝

4. 원한다면｀m해-caps를입력하여small cap
폰트 변수를 사용할수 있다 (p222 참조？.
5. p214의 2번에 주어진 값들을 사용하여 원하는
폰트 사이즈를 입력한다．
6. 필요하다면／line-heighㅎ를입력한다. lineheight는 폰트 사이즈와 똑같은 폼으로 표현되
어 있다 (p215 참조？.

population {font-weight:bold}

p.efllu',,Ldu巾 x.．∥ MI,:In5,.lt 1sUnset r "pin's
3 F `．驪1
Ek 트出 Y比, Fjes,iss In
'S dto
5-

-

■ 작성자는개별선택사항을따로설정할수있다．
그 단계가 설명된 페이지를 본다．
■ 여기서 위에 정해 놓았던 순서와공식적인 설명
은 넷스케이프에서 필요한 부분이다. 익스플로
러는 구애받지 않는 것 같다.
■ 그들이 디폴트값으로 설정되었을 경우단지
사이즈와family만이 요구된다. 다른 모든 정의
들은 생략될 수 있다，
■ 만일폰트사이즈를설정했다면폰트를가지고
라인 높이를 설정해야 한다．
■ 폰트 특성은 그들의 부모 요소로부터 자 요소로
유전된다．

216

j

stop

」

Rehe寸，

H히1也

=The animals and plants on oar planet are disapPearing at an alarming
:rate.r.8 tune todo something about it right now!
perhaps no more than go adult引cit in wild
FLorida With
areas ofSoothwestern Florida· the majestic but
Florida Pan仕1er (?am.
Panther 아ooive
caer必rnupel눔 perhaps one ar
the most endangered species in
小e wonld. Graze roots and
governmental agencies haVe
joined forces to hedP ke.P the
panther 丘이n extinction. Efforts
bave llcuoed on restoring
genetic diversity in the tiny pomlotion by,snportit坦
8 Tcoon 000gars m 5995, and on avoiding accidentn
with oars by building underpauneo I님ow highways
that pass through dleir dwindli,垠 habitats. Scientists
believe that without an effective management plan,
由e Florida Pan나ter will d`$aPpear from 出e wild
wi枋on 25 years.

7, 스페이스를입력하고그뒤에 원하는폰트가족
을 입력한다. 순서는 원하는대로 쓰면 되고
p210에서 보이는 것처럼 쉼표에 의해 구분된다．

p1 nPS

-'

Giant
River
Otter
池】0m好

The Giant River Otter (S'seesoam tneailameie)is a
remarkably social animal, traveling isgryupyyj
c캐ed 屯이
＇r'headed by a
Giant River Otters
monogamous pair a끄d usualb htint, groom, and
also comprising several
rent t어teeher1and
esnerations 0fo麻.rinc. The7
m 瀚 ∥m띠1hr山
· 口 m
isis

그림15.14 결과슨 7〃별특정들을 각칵 졍의한 깃과 같을 깃이다．

===== PAGE 206 =====
205 =====
Formatting Text with CSS
ㄴI

트 c de."`

円

아ont-face {fon나amily:Trebuchet MS;
src:url(TREBUCH0.eot)}

그것이 절이든 단지 몇 개의 단어든 간에, 사용자는
텍스트의 색상을 변화시킬 수 있다．

@font-face {font-family:Georgia;
src:url(GEORGIA0.eot)}
name {lont:bold 24pt/22pt; :Trebuchet MS;
width:100;margin-top:10;color:#A50063}
intro, description (font: 10pt Georgio}
lotin-name (font-style:italic}

텍스트 색상 정하기：
1. Cdor：를입력한다．
2. colorname을입력한다. colorname자리에는
미리 정의된 16색상 중의 하나가 들어온다．

population {font-weight:bold}
그림15.15 여기서는 보라색을표준 16찬볐 시즈템으로 설정했다．
奪
「tc,i-te·t\pa,uhr.,hlu,b enl - HerniaS Internet Enptco,

= 까｀5 SIIILOSLS and힌ants on Our디ariet arc lrsappearmg at an alarming
:rate.Ifs time undo somethmg about it right newt

:
:

또는rgb(r, g, b）
를 입력한다. r, g, b자리에는
원하는 색상 안의 red, green, blue의 양을 각각
0-255의 숫자로 표시하는 정수가 온다．
또는『gb(r%, g%, b%）를 입력한다. r, g, b
자리에는 원하는 색상 안의 red, green, blue의
퍼센티지를 정한다.

I', nm

,

ined

j。

With parh캬Is no more dlan 5. aduh引可tin wild
areas ofSouthwestern Florida, the majestic but
이naive Florida Panther 伊tm'=
떽51tthㅇut 카1
roeroJesrseytiio perhaps one of 胡；eCt1ve
themost endangered 町ecies 恤
management
p1st치the Florida
governmental agencies have
Panther 卄m
f。
rces t。
help keep the
dioappear within
extinction.
Efforts
panther from
Osyears.'
hav· focuued on rmto!ing
genetic diversity in the tiny popalatiots by importing
STexanc。
ugars in n995,and 。n av。
iding accidents
with cars by building nnderpassen below highways
that pam throu밖1their dwindling habitats. Scientists

또는＃rrggbb를 입력한다. rrggbb 자리에는
원하는 색상의 16진법 표기법이 온다．

the
believe
Fl。
rida
thatPanther
without an
willeffe pear
die짧vemanagement]
fr。m the wild
plan,
`Y汎山S ngyears.

Giant
River
Otter

ㅜhecㅗant R』
ver ㅇtter (洶oanss 뇨sa祗ee柚.lo a
r叩tar닢big social animal, traveling in groupeof s-c .
ral1ed'hotts, heeded bya -,, I Giant
River otters I
1n.n？쁘쁘as pan ass rissaoy I hunt, groom, and !

s就e驪mxg蒿縕. They k雙together,in시 」
簪轟發磁醇黨難轉蜘邸蜘轅藿磁

그림15.16 만일 방문자들ㅇ／폐《）
／자 앍기를 원한다면 텍스트의
색을 결정할 때 배경색과 텍즈트 색의 대초가 분명한차를 명심하고
주의q아한다．

■ 색상을 정하는 더 자세한사항은 부록 D의 16진
법색샹을 보면 된다．
■ 만일 r, g, b의 값에 255보다 큰 정수를 넣을
경우그숫자는255로 대체된다. 또한100%
보다 큰 퍼센티지는 100％로 대체될 것이다.
■ 우리는요소의 색상을조절할 때 필요한color
특성을사용하는방법은 이미 알고 있다. 텍스트
색상을 조절하는 것도 다른 것이 아니지만 여기
언급된 정보들은 중요한 것들이다．
■ 또한＃rgb를 사용함으로써 16진법의 값이 어디
에서 반복되는 자릿수가 나타나는지 설정할 수
있다. 그것은＃FF0099를＃F09로쓸수 있다．
■16진수는 직접 인용 부호에 의해서 감싸지지
않는다．
■ color 특성은유전된다．

예제의소스 코드는 www.mokwood,comq 있습나다．

217

發

g = ＝口4訂甘X4＾ 。＝떼

FLorida
Panther

텍스트 색상 설정하기

===== PAGE 207 =====
206 =====
태apter ]5

2.

1.

텍스트의 배경 바꾸기：
background：를 입력한다．
transparen* 또는Cdor를 입력한다. color
자리에는 색상의 이름이나 16진법 색상이 들어
가게된다．

r
* X곁● fm= mm듬占
쩍＝ =e量V。 m

3. 원한다면un (image.gin를입력한다. image
.gif자리에는 배경으로 사용하려는 이미지의
URL이 들어간다．
필요에 따라repe아를 사용하여 이미지를 세로
나가로로붙일수있게한다. r야)eat-x는단지
가로로이미지를붙이는것이고, repeat-y는
세로로붙이는것이고, no-repe아는 이미지를
붙이지 않는 것이다．
원한다면 fixed 또는＄crㅞ을 사용하여 배경이
스크롤되어야 하는지를 판단한다．

@font-foce {font-family:Georgia;
src:url(GEORGIA0.eot)}
endangered_species (background:#ffe7c6}
name｛拓nt: bold 24pt/22pt Trebuchet MS;
width:100;margin-top:10;color:#a50063}
intro, description (font:10pt Georgia;
bockaround:#阡d
blurk나bockground:#ffc6o5}
latin_name {font-style:italic}
population {font-weight:bold}
그림15.17 여가서는 루트 요크 (endangered_specie하，
intro와description 요소와 blurb를위해 배경색을

설정하였다. 아것들은복잡하게느껴지자만사질은 서로 찰 어울
린다．
}F:`nsn-tnt`pasthorsblu.h ant - M,n,nsott Internet Explore,
Eto

S.dt

yen Fvelea

굿

■ 색상과GIF 이미지의 URL을 배경으로 설정할
수 있다. 색상은 이미지가 로딩될 때까지 사용될
것이다. 또는 어느 이유로 로딩되지 못할 경우에
도 사용된다. 그리고 이미지의 투명한 부분을
통해서 보이게 될 것이다．
■ 배경 특성 (background proper取）
은부모
요소로부터 자 요소로 유전되는 것은 아니다．

218

工.001,

J

Sins

느e누
H出om

소

ㅐne.

h

;The animals and plaurn on oar planet are小nappearing at att alarming
1rate.Its山ne to do something about it r.ght now!
With perhaps no more 댜‘an 5oadults left it, wild
Florida areas
ofSouthwestern Florida' dto majestic but
Panther elusive Florida Panther (P1m낚

tcmostendangredspecsesin
隘듦됴 emt
`l1d nU` lU~
나1d>b '`7나L: d』
lU

필요에 따라xy를 입력하여 배경 이미지의
위치를설정한다. x나y는왼쪽위 구석으로부터
의 절대적 거리나 퍼센티지로 표현된다. 또는
x를 위해서 top, center, bottom을 사용하고，
γ를위해서 /eft, center, right를사용한다．

1/ nPS

mr

도斗，

배경은 페이지 전체에 대한 배경을 의미하는 것이
아니고 특정 태그의 배경을 의미하는 것이다. 다시
말해 배경을 다른 색으로 설정하여 단지 몇 구절이나
또는 몇 단어의 배경을 바꿀 수 있다는 것이다．

＝느－
：솝a午．
뇨＝
－노＝
cole.css 藁玉；

@font-face {font-fomily:Trebuchet MS;
src:url(TREBUCH0.eot})

－그

텍스트 배경 바꾸기

卜시놔）H`, ＝ㄵ1,ia`

will.:,. :..
the
（
help keep
;'i芬；
崗갊搖苔；
f。
rces t。
c業
j。
insel
；닙 Pa빤Icr
∼rr " ∥‘`" '1」
〃卜J- ㅗ＾줅 oa,....I'"｀
「，
뒤 `h.' 4→，, a｀
嚆；祗그； 茹品丁＝G幕r"-4亞些竺즈－--[
genetic diversity in the tiny pepulatian by 1mF.nrtisg
8 Texan cougars m 2995, ana ㅇn avoiding accidelIte
with cars by building suderpasses below highways
that Pass throtigh their dwindhissg habitats. Scientists
believe that without an effective management
the Fl。
rida Panther will disappear fr。m the wild
plan,
withm 25 years.

(hant
River
Otter
亡］0ne

The Giant River Otter (plsmoms &usiliensiolin a
remarkably social anitoal,tcav액l驟in groups of4-y

call竺’t1o1tr, neasesbya ,. 比iant River Ottarn
na'an,'ogar컵驪；ps騙ou,asuasy fhsnt,grvcen,剖14

M "- . +=.二n J믓丘一J.:= ㅜㄴ｀.. ! rest sogernst, ass
트도H月ㅅ兄｝`z」
拉未i닢戇혹y뇨嶼毛4J1F! 工L一一 →ㅈ
'
…포藿難꽉4… 1 旺竪L.．펭xe.닐

.zi

그림15.18 색상의 현명한 사용은 정보의중요성과 그 내용으로
이끄는 깃을도와 준다（이것은 여기서보아는 것보다 더색갚있재
보여잔다. 웹사이트를본다）
.

===== PAGE 208 =====
207 =====
Formatting Text with CSS
口

Cude.Css

공간 조절하기

@font-face {font-family:Trebuchet MS;
src:url(TREBUCH0.eot)}

단어들 (tracking) 사이와글자 (kerning）
들사이의
공간을
더할
수 있고
공간을 더하거나 줄일 수 있다.
특정 절 이전에 들여쓰기를 할 수 있다．

@font-face (font-family:Georgia;
src:url(GEORGIA0.eot)}
endangered_species (background:#f1e7c6}
name (font: b히d 24pt/22pt Trebuchet MS;
width:100;margin-top:10;color:#A50063}

트랙킹 정하기：

intro, description (font:10pt
Georgia; background:#ffffc6}
blurb {background:#ffcoa5;Ietter-spacing:.lem;
text-indent:15p다
latin_name (font-sMe:italic}
population {font-weight:bold}

J
5t叩

仝
吼s

1. text-indent:를입력한다．

SearS

a 1 , * . · 1 . . m 1 ' * ' 1 1 . 1 1 * 1 1 * * 日m * . m * 日弗 m

1 * `

W1gb perhaps so more than 50 adUlts loft ow,딨
Florida 0mam
ofSouthwestern Florida, thernajeat1' 컨n戚
elusive
Flor
Pan앉1er rasralisrcs껼o
haPanther
perhaps。ne
(Pawns
。f 寸，
：씻）낟n:

the most endangered sParias m
山eworld. cram roots and
governmental agencies hays
1ㅇmea fcr000, toJiaru banru n1e
panther h-on, nsltinotios.E而rt즙 , 르
nave 00005eα os restoring
, .
rsnet；콘ㅐi-owre, 汁 H갸슈 十；n口
iiea"5
population by繃舜r而如'
Texan coogare in 1995,and on avoiding sc口,dents
with caruby bunding ondarpassar below highways
that pans throughtheir dwindling habitats憑ientists
b싫inva 나lot withontan effective masagement plan,
出白 Florida Panther wln disappear from 山e wdd
within 25 y·ar5.

쬔〕D미낙

hnadedbya

The Giant River Otter ( 넋enms 뇨a姐nnmplis a
remarkably social animal, traveling in groxpe
ci
oal1odholta,
m。
gam。
us pair and us'aall
, .. 1
n。
alsoq으mnrisi,agseooral .
（H11r래繃
르뇽 以
.

ntt샐＝〕r

2. length를입력한다. length자리에는픽셀，
포인트, ems 등등의 숫자값이 들어간다．
들며쓰기 정하기：

b0w

:The animals and plants on our planet are dinappearing atan alarming
=rate.Its time I., do nomething about it r岵lt now

Giant
River

커닝 정하기：

그림1520 악스플로러는 최근에 텍즈트 들여쓰기와 글자 공간
r딘ㄴ이공간이 아님）
을 지원한다．넷즈쾡이프는 단자 텍스트 들여
쓰가만을지원한다．

2. 텍스트 인덴트에 대한값을적는다. 그값으로는
, 또는퍼센
절대적인값（양수나음수상관없이）
티지를 사용할 수 있다．

I, 1im
■ 단어와글자공간에 음수의 값을 사용할수 있다．
실제로 보여지는 것은 언제나 브라우저의 감당
능력에 달려있다고 해도 말이다．
■ 단어와글자공간값은 정렬 방식 선택에 의해
영향을 받을 것이다．
■normal 값을 사용하여 그들의 디폴트 값에
글자나 단어 공간을 설정한다．
■ 가지런한텍스트안에서 벌어진틈을피하기
위해서 글자 공간에 0의 값을 사용한다．
■ 최근에는넷스케이프만이 text-indent를
지원한다．
■ 모든공간특성들은유전된다．

예제의소스 코드는 www` cookwood.c(Jm에 있즙나다

219

＾
。
＝
4
， 의＝ =．읗。 ＝=.

互 t\c5$-te,t\p,xth,xbtu,b,nt - Mnansvfl ln1nmet E치,tn,r,

」〕
R轍e,h

2. leng卄’를입력한다. length자리에는픽셀，
포인트, ems 등의 숫자값이 들어간다．

1. letter-spacing＝을입력한다．

.2림15.19 여가서는 blurb 요소 안의글자사이 공간을 .lem
만큼 넓할 것아고 i5포인트로 들여쓰가 할 것아다．

b7ussa hw

1. word-spacing을입력한다．

===== PAGE 209 =====
208 =====
Chapter 15

텍스트 정렬하기：
1. text-이ign：을입력한다．
2. left를입력하여 텍스트를왼쪽으로정렬한다．
또는 ru이l1t를 입력하여 텍스트를 오른쪽으로
정렬한다．
또는center를 입력하여 텍스트를 스크린의
가운데로 정렬한다．
또는jus而를 입력하여 텍스트를 오른쪽과
왼쪽 끝으로 정렬한다．

V nP$

■ 자요소들은 그들의 부모 요소들에게서 text
align 특성을유전 받는다．

@font-foce (font-family:Georgia;
src:url(GEORGIA0.eot)}
endangered_species {background:#ffe7co}
name (font: bold 24pt/22한 Trebuchet MS;
width:100;margin-top:10; color:#A50063}
intro, description (font:10pt Georgia;
background:싸lffc6;text-비ig띠ustify}
blurb (background:#侃6a5;margin:8 102;
text비ign:center가
latin_name (font-style:italic}
population {font-weight:bold}
그림15.21여刀서는 intro와 description텍스트를 정렬했다．
blurb 텍즈트를 가운데 징렬하여 blurb에서유전되ㅈ／ 않았을
경우 나타날 결과를 무사했1打blurb의마잔을 조절함으로 아깃은
정렬된 텍스트에찰 맞게 할수 았다. 자세한사항은197을보자l.

互F:ioi1-【쁜Kr\od'ihe,ibtiaib sini - Micmsoft inteinet Esplow.
Eis

E St

yi．
叫 F호v《y놀e; 1.
→

:

j

St야）

5。
ais*i

=The animals and plants on our planet are disappearing at an計arming
:rate.It's Ib is to do sosnething abc ns it r喀lit noM
·1

florida
Panther

7u나i-ester?' r
r그코 ．口αrㅂbr we,콰
p3 one 0f the lrP
nger出 species iii "
rimental agencies }i:
n1 forces to help I:, from extinct
1,
have f。
cused cx
∼…
cup gefletic dleerutty n} the nmy poptila'i
-iing 日 ㅜ슨xan cougars n겋 5095, and 0n a!1
ontO with cats by building utiderpasseo "
its 由at pass 小roagh 나驢sir dwindling ha
노m: L너／，一 태r L→i ㅌ｀ 1n 尸
!.other,

*X꾑m灌＝ 르

■ 만일 텍스트 행 길이를 가지런히 하기를 선택
했다면 단어 간격과 글자 간격이 반대로 영향을
받는다는 것에 유념하자. 더 자세한 정보는
p219의 공간조절하기를보면 된다．

[.

스j

어떤 IfI取1L 태그를 설정하여 왼쪽이나 오른쪽 가운
데 원하는 대로 정렬할 수 있다．

\ 1j code.rss

@font-face {font-family:Trebuchet MS;
src:url(TREBUCH0.eot)}

H象，

텍스트 정렬하기

이ant
River
Otter
i老그 D“壬

그림15.22 행의 길이가 징렬된 설명 (description) 안에서 텍즈트
（마진 정렬도 함聊는 블금／브를드러나보이게 하고 블러브를 가운
데로 하는 것은 아것을 더욱 우아하廢枓

220

===== PAGE 210 =====
209 =====
Formatting Text with CSS
￡1}de.c$$

u

j穫· 菊

@font-face (font-family:Trebuchet MS;
src:url(TREBUCH0.eot)}

텍스트의 아래, 위 텍스트의 중간에（아마도 문서
내의 변화가 생길 것이다）라인을 넣을 수 있다．

@font-face {font-family:Georgia;
src:url(GEORGIA0.eot)}
endangered_species {background:#ffe7c6}
name {font: bold 24pt/22pt Trebuchet MS;
width:100;margin-top:10; color:#A50063}

텍스트 밑줄 긋기：
1. text-decoration：을입력한다．

infro, description {font:10pt Georgia;
background:#冊c6;text-align: justify)

2. text아래에줄을긋기 위해underline을입력
한다．

blurb {background:#ffc6o5;margin:8 10 2;
text-align:center;}

또는 텍스트 위에 줄을 긋기 위해서 .verline을
입력한다．

latin_name {font-siyle:italic}
population {font-wei小t:bold)
more_info {text-decoration:underline}

또는 텍스트에 줄을 그어 지우기 (strike-out)
위해서늬mne throug卜를 입력한다．

그림i丘23 more info 요소는 링크（이아x工伽k와xPointer
들은 브라우저 안에서 쟐행되어져 았다. p223)가되도록 만들어
겼다. 웹표준을 따르기 위해저 밑줄을가치고 요소를포맷했다．

Ld1 恥e, loose'.

loOn

브a5

j

儡

빼回口

■ 대부분의 그래픽 디자이너는밑줄을싫어한다.
그들은 그것을 타이프라이터 시대의 유물로
간주한다. 그러한 디자이너들은 링크의 텍스트
를 꾸미는 옵션으로 아무것도 사용하지 않는다．
그러나 링크들은 다른 방법으로라도 표시되어야
하고 그렇지 않다면 아무도 그것을 클릭하지
않을 것이다．

乞

Tire 뇨」t River ㅇtt已r mes꾜ara 加an,Unaasti, is a
remarkably too,히 animal, traveling mmgrvtmps of 4 0
ailed 'holtn", beaded by a
nasnngamosmu pairP, and
msially alt
pritir.g
랖i LeO etnuven
.ts.

＝」

pear

겯isap,

pchaps one .f the moot
mesagernest
endangersd species hl the
, the,Florida
world. Grass roots a긔d
plan,
Panther will
governmental agencies have
joined forces to h이P keep
the panther front etitinotien.
teirkis
Effvrte have focused ()n
restoring genetic diversity in time tiny p아,ulatien by
'nidmg
.noIgacs긔n
口．
a
디and이1as
一士끄切且끄Jron
anusdOsts with cars by bUr
［出ng underpassen below
lsighmeays that pass through their desiss棚ing habitats,
loientists believe that without an effective
management plan, the Florida Panther will disappear
from the neild Wi난un as yearn.

.

2. none을입력한다．

■ 보통 라인을 가지고 있는 태그에서 라인을 제거
할수 있다（특히 HI爪4L 안에서 u, strike,
del, ins와 같은 것들）
.

i'Iith perhaps no mare than go adults left in wild
Ftorida area5
口f 面uthwestern FIsrida, the m司5St1C bdt
eluSive
Panther
Panther t"乃Sisa o,Florida
mmoi mnoyi) is

'

1. text-decoration：을입력한다．

V nPS

= ㅜheanimalsand p14n0 on Otis 짇aCetate dinappearisget ass alarm】
ing
=rate,Ifs tints t0 dosomet贓mmg atout it cightoessl
'孔.. → 1｀立軋，
〃＾｀孰쵭凡

Giant
mver
Otter
Dove

라인 지우기：

■ 자요소들은그들의 부모요소들로부터 七色《七－
decoration 특성을 물려받지 않는다.

그림15.24 요조에 단순하 밑줄을 긋는다는 것아 링크를 의11/하슨
것은 아L／다. 이것을 클락한다고 해저 어다로 연결된다는 의미도
아나다（다자 말해XLink와XPointer 등이 빠져있는 깃O/다）
.
그리고 밑줄 굿기를 아떠한 것（랑크가 아닌 깃아라 할자라도갸叩도
적용할수 있자만 아러한 행동은 방문자를 혼란스럽게 할 것이다．

예4의소스 코드는 www.cookwood.com에 있습나다．

221

두｀ .＝呈＝ 山甘三

F:`C＄찮1닙8놔＼i1ara1m1t' "'*.三긔· Im.imsftt,남5'- E三pk)1·
트is

텍AE 밑줄 긋기

===== PAGE 211 =====
210 =====
Chapter 15

작성자의 스타일로 text-transformation 특성
을 사용하여 텍스트 케이스를 정의할 수 있다. 이런
방법으로 첫 글자만 대문자로, 모두 대문자로, 모두
소문자로, 또는쓰여진 그대로 텍스트를보여줄수
있다．
텍스트 케이스 조절하기：
1. 枷e-fransform：을입력한다．
2. c이：巾dize를입력하여 각단어의 첫단어가
대문자가 되게 한다．
또는 uppercase를 입력하여 모든 글자가 대문
자가 되게 한다．

또는 none을 입력하여 원래 텍스트대로 표현
한다（유전된 값은 취소 될 것이다）
.
많은 폰트들은 상응하는 소문자 변수를 가지는데
소문자 변수들은 부분적으로 소문자 크기의 대문자
버전 글자를 포함하고 있다. font-variant（이형
폰트）특정을 가지고 소문자 크기의 대문자 변수들을
호출할 수 있다．
소문자 폰트IA權F하기：

@font-face (font-tam如Georgia;
src:url(GEORGIA0.eot)}
endangered_species {background:#ffe7c6}
name {font: bold 24pt122pt Trebuchet MS;
width:100;margin-top:10; color:#A50063}
infro, description (font:10pt Georgia;
background:#ff1fc6;text-align:justify}
blurb {background:#ffc6a5;margin:8 102; textalign:center;}
latin_name {font-style:italic;
text-transform:uppercase}
population (font-wei寸t:bold}
more_info (text-decoration:underline}
그림15.25 여가서는 latin name 요소가모두 대문자로 보여자
게하가로결정핸다. text-transform 특성은꼬든 latin_
name 요소의 컨텐츠를 다사 써아 하는 의무갚에저 해방자켜 줄 깃
이다．
jF-tc.i-teet\panthmibhob eel - Min,o.smrennet Enpiote,
E魅 Ode y'5, , Farm,, ir'츱 巾如
』〕
Hd1e甘1

is perhaps one ot the most
endangered species i5 the

222

걀m
__

goversmentai
ined
f。
rces t。
agenc鰥ave
keep
____________
나iv panther from extinction.
Efforts have focused on
vectoring gswetic diversity in the tiny P아citation卜y
cyortina 8 Texan cougars in iss5, and on aV.'ding
accidents with cars by building usderpasses below
highways that pam 出rough their dwindling habitats.
Scientists believe mat without en effective
management plan, the Florida Panther will disappear
f1 ar】m 'odd eith,s euvearo.

·／ nP$

■ text-transform과 font-variant 특성
모두유전된다．

:
=

Perhaps no tore thatt 5《）adults left in 싸1닝
Florida 1qid`
areas of Southwestern 디orida, the majestic bat
디orida Panther
Panther 이naive
PL伋f4 （刀NO兀뱁가z C口幻7I
＝璥

2. sm네-cap＄를입력한다．

■ 다양한폰트값을가진조합안에서는texttransform을 사용하는데 어려움을 느낀다．
만일 text-transform 사용을 계획한다면
폰트값을 각각 정의하는 것을 충고한다．

功
to心oh

1 * 兀t 1 .

1. 拓nt-variant를입력한다．

■ 독립적인스타일을위해작은대문자변수의
사용을 피하기 위해서 拓nt-varianl.none을
사용한다．

소
Hore

=The animals and plants on our planet are disappearing at an alarming
:rateJtn time todosomethtngabout卄 right none'

j。

●믐닐* 닙
m
． ●
上
* m
＝ 튱g口占

또
`vercase를입력하여 모든글자가소문
자가 되게 한다．

즐鎣纛阿률

츨聲 mde.cS$

아ont-face {fon나omily:Trebuchet MS;
src:url(TREBUCH0.eot)}

Giant
River
otter
也 Liner

help

텍스트 케이스 조점하기

rhe Clan' Paver Otter i fl 万RotaL叱 F／亡5SIZJ三Nuts
Ira remarkably soci出 anim出！traveling in groups d
a-p waIted ' h·.hs'1headedby
monogamous pair and
usually aIm0 cvwpnstng
∼m〃
［m1 = n恥

폄

로 나타
그림15.26 아가의 latin name 요소들은모두 대문자．
내7）
다

===== PAGE 212 =====
211 =====
PART 6:

XLink2F XPointer
링뵤와 이미지들 225

223

===== PAGE 213 =====
212 =====
]6

LINKS AND IMAGES:
XLINK AND XPOINTER
링크와 이미지들： x니N（와 xP이NTER

ffl 의 인기는 두 가지 요소에 기인한다：하이퍼
링크와 이미지. 전자의 것은 웹 페이지에 있는 정보
를 세계의 다른 웹 페이지 정보에 연결하는 역할을
하고 후자의 것은 웹 페이지에 시각적 요소를 준다．

이것은 또한 이 책의 설명들이 XLink (h婢〕
．‘〃
www.w3.org/TR/xlink4와XPointer（砒加：//
www. w3. org/TR/xptr)의 정의들이 주로 가설에
근거한 것이라는 것을 의미한다. 브라우저들이 결국
링크를 어떻게 다룰 것인지 추측할 수 있는반면에
테스트 할 방법이나 실제 세계에 직면했을 때 설명이
어떻게 보일지는 알 수 없다. 그래서 이 장을 이용하
여 XLink와XPointer의 맛을 볼 수 있겠지만 이것
이 실제 어떻게 될 것인가는 조금 더 기다려 봐야 할
것이다．

225

크。 붊 m ＂닙＝ ＝升。 ＝`,，。＝4m4

유일한 문제점은 어떤 브라우저도 XIㅍnk와XPoin
ter를 지원하지 못한다는 점이다. 이 의미는 기능성
의 링크와 첨가되는 이미지를 가진 XML, 페이지를
小카스할수 없다는 말이다. 아니 서비스를 할 수는
있지만그것을아무도볼수 없을뿐이다. 이것은
크나큰장애이다. XLink와XPointer가브라우저에
사용되기 전까지 보통 사람들이 링크와 이미지를
자신의 브라우저를 통해 볼 수 있도록 최종 파일은
HTMl로 변환시키는 것이 필요하다．

=．月。 ＝
`

그러나 XML의 디자이너들은 HTML의 기초적인
시스템에 만족하지 못했다. 작성자로 하여금 여러
방향의 링크를 만들게 하고 링크들이 어떻게 혹은
언제 활동하게 되는지를 조절하는 것 등의 더 믿음직
한 방법을 선택했다. XLink와 XPointer 이 두 언어
에 시스템이 의존하는데 이 두 언어는 이 장에서
자세히 설명할 것이다.

===== PAGE 214 =====
213 =====
（十apte시 6

간단한 링크 만들기
IfI玉4L 에서는 링크와 이미지를 매우 다른 것이라고
생각하지만 실제 이것은 매우 유사한 것들이다．
우리는 외부 파일의 설명을 갖는 요소를 갖고 있다．
만일 외부 파일이 다른 웹 페이지라고 한다면 링크를
클릭하는 것은 가끔 다른 웹 페이지가 윈도우의 현재
컨텐츠를 대신하게 만든다. 만일 외부 파일이 지원
되는 파일 포맷 - JPEG 또는 GIF 파일 - 이라고
한다면 외부 파일은 페이지 안에서 그 자체가 보일
것이다. XML 안에서는 어떤 외부 파일이든 같은
메카니즘에 대한 두 종류의 설명을 만들 수 있다.
간단한 링크 만돋기：

= ＝。●느U
=
=
m “ 을 ㅌ 驪。 m

1. 문서의 루트요소안에서는（또는링크를만드는
요소 안에서）xmlns:xlink="卜1卄p://www.
w3.org/1999/xlink"를 사용하여 XUnk
이름공간을 선언한다. 더 자세한 사항은 8장의
XML의 이름공간사용하기를 참조한다.

C de,!n川

<endangered_species xrnlns:xlink=
'http://www.w3.org/1999/xlink">
그림16.1 XLink 족성또는요소들 중 어떤 것을ㅈ梧하가 전에
문서의루트 요소 안에저无
［功k 아름공간을 선언해야 한다 (또는
XLink 속성과요소들을ㅈ陪할개별요소에서).
瑙

4. 필요에따라치ink:r이e="use＂를입력한다．
use 자리에는 - 정보를 읽을 기계에게 - 설명이
무엇에 관한 것인지를 설명한다．
5, 원한다면）
dink:title=hdescripiion"을입력한
다. description은 방문자들에게 링크가 어디로
방문자를 인도할지 알려주기 위해 파서에 의해
사용될 것이다.

226

心de=1{n11

<endangered_species xmlns:xlink=
"http://www.w3.org/1999/xlink">
<animal>
<name Ianguage="English">Tiger</name>
<source xlink:type="simple" xlink:href=
"http://www.warldwildlife.org/species/
species.cfm2sectionid=I 20&newspaperid=21
「
xlink:role="info source' xlink:title="Source of
Information" xtink:show="replace"
xlink:actuate='onRequest"/>

그림16.2 이xML 문서 안에 source 요소는브라우저 안에서
최근 문서의 컨텐츠를 甲진할와부 파일의 링크를포함하고 있다．

2. 다른것과연결하기를원하는시작태그안에서
치ink:type="simple"을 입력한다.
3. 다음xlinl沙iref="URL"을입력한다. URL자리
에는 설명하기를 원하는 파일 위치가 있다. 만일
파일 안에서 특정 부분 또는 포인트를 설명하려
면 XPoint를 첨가할 필요가 있다 (p233 참조그．

三三＝눴느횬1三三뜨三ㅌ三ㅍ＝괏흩三＝七育‘∼

, code.HmI , , , `

, , ,' . d ,+.r

巴클

<picture xlink:type="simple" xlink:href='tiger.jpg"
xlink:role="image" xlink:title="Tiger:Panthera
tiaris" xlink:shaw="embedded"
xllnk:actuate= 'onLoaa「 X="LUU y= ri/'f>

그람 16.3 그림16.2의같은 문서에서가져온 예제에서 picture
요소는 나중에로냥될 때문저 안에저 첨가될 tiger.jpg라고 ㅎ陪
와부파일에 대한설명을포함하고 있다. picture 요소는겨7족
해서XLinl, x, γ와관4' 없는 족성을포함하고 있다는 것에주의
한다．

===== PAGE 215 =====
214 =====
Links an山mages: XLink and XPointer
c de.∥m1 ,

口

<xlink:simple xIink:href."tiger.jpg"
xlink:role="image" xlink:title="Tiger: Panthera
tigris" 치ink:show="embedded"
xlink:actuate="onLoad"/>

.2림16.4 刀존의요소로부타 링크를 만드는 대산에 라파런스룰
포함하는 ?ree-standing" XLink 요소를 만들주 았다. xlink:
type='simple" 족정은요소 (Xlink: simple)Q/ 이름이
되고 속성의 나叫지부분은 변함아 없다．

6. 다음〕
clink:寸low＝를입력하여 외부파일이
어디서 나타나야 하는지 결정한다．
다음에 " replace"를브라우저 안의모든최근
문서를 대체하는 표준 HTML 스타일 링크를
위해 입력한다．
또는 최근 문서 안에서 바로 보여진 표준 HTML
스타일 이미지를 위해 "embedded" 를 입력
한다．
또는 참조된 파일을 위한 새로운 창을 열기 위해
"new∥를 입력한다．
7. 마지막으로치ink:actuate＝를입력하여 외부
파일이 언제호출되는지 결정한다．

또는 설명된 파일이 링크가 로딩될 때（첨가된
파일에서는 전형적인 것이다）파일이 자동적
으로 나타날수 있도록 ''onload∥를 입력한다．
'/ 'iPS
■ 여기서 설명된 방법 1은다른파일과 연결되기를
원하는 XML 문서 안에서 요소에 XLink 속정을
더하는 것으로 구성되어 있다. 또한 완전 새로운
XLink 요소（그림 16.4）
를만들 수 있다. xlink:
竗pe="simIJe"은 요소의 이름과 다른 속성 <xlink:simple xlink:href="URL"...>이 여전
히 남아있는 - 안에 흡수되어 있다. 이것은 작성
자가 사용한 방법과는 무관하다．
■ 자신의 문서에 첨가한XLink속성들（또는요소
들）
은 유효한 문서를 위한 DTD 안에서 정의되
어야한다. DTD에 대한자세한 사항은 2장의
DTD 만들7／를 보자.

예21/의소스 코드는 www cookwoo心：om에 있습나다．

227

^
,
m
。 ＝=．。珊크릉＝ =
,

그리고 설명된 파일이 나타날수 있게（하이퍼
링크에서는 전형적인 것들이다）방문자들이
클릭같은것을하게 하기 위해서 " on-Request'1
를 입력한다．

===== PAGE 216 =====
215 =====
다tapter ]6

링크세트 만듈기
링크세트는 파일 안에서 모든 시리즈 또는 개별
포인트들또는둘모두를동시에 연결한다. 연결되어
질 파일에 관한 모든 정보를 포함하는 중심 요소를
만들고 다음에 그들 사이의 관계를 규정한다. 결과는
링크세트이다．
링크체트 만匠기：
1. 문서의 루트요소 안에서（또는당신이 링크를
만들고 있는 요소 안에서）xmlns:넜ink=" http:
//www.w3.org/1999/치ink" 를 입력하여
XLhIk 이름공간을 선언한다. 더 자세한 사항은
8장 XML의 이름공간사용하기를 보자．
2. 링크정보를포함할요소안에서치ink:type=
"extended＂를 입력한다．

*
●
m
= ＝븝口m= ＝口쁜닐

3, 원한다면p226에설명된것처럼넜ink:r이e과
넜ink:title을 작성한다．
4. p229에서 설명된 것처럼 링크될 포인트나파일
을 정의한다．
5. p230에설명된것처럼 그런파일의관계를정의
한다．

v' Tips
■ 링크세트의 정의는관계가정의된 파일 안에
위치하고 있을 것이다. 또는 독립적인 외부 파일
안에 위치하고 있을지도 모른다．
U p227에 설명한것과같은방식으로＜넜ink:
extended...> 요소를 <your_element xlink:
竗pe= 'extended"...> 대신 사용할수 있다．
이것은 같은 결과를 갖는다．
■ 링크세트는 하나의 확장돤 랑크 (p226의 간단한
링크와 대조되는 개념이다）
로 설명된다．

228

듣圄컫媛릎藍暴臻叢髥鞋聲難푿tOdOj4llflk

<linkset xmlns:xlink=
"http://www.w3.org/1999/xlink">
<resources xlink:type="extended"
xlink:role="animal resources"
xlink:title="Additional Sources of
Information">
.c!--here's where you describe the files to be
hnked-->
<I--here's where the connections are defined-->
c/resources>
.2림姓5 링크세E는 xlink: type= "extended" 를 포함하는
요소와함계사작한다．

===== PAGE 217 =====
216 =====
Links and Images: XLink and XPointer
피■－

ㄻde.HIi11k

견누三每亮＝二스！1∼느＝닉

dinkset xmins:xlink=
"http://www.w3.org/1999/xIink">
<resources xlink:type="extended
xlink:role="animal resources"
xlink:title="Additional Sources of
Information">
<animal_info xlink:type="locator"
xlink:href="tiger.xml" xlink:role="ti9er"
xtink:title="Tiger"/>
<animal_info xlink:type="Iocator"
xlink:href="panther.xml" xlink:role="panther"
？小nk:title="티orida Panther"!>
<anim비_info xlink:iype='니ocator"
xlink:href="rhino.xml" xlink:role="rhino"
세nk:title="Black 帥no7>
<animal_info xlink:type="locator"
xlink:href="otter.xml" xlink:role="otter"
xlink:title="Great River Otter"!>
<l--here's where the connections are defined->
</resources>
그림16.6 링크ㅈ7）트에 있는 걔별 례퍼런스 포인트는 특정 파일
（링크의사작과 끝으로서 역할을 하게 될瑨 정의하게 된다．

레퍼런스 포인트 정의하기
하나의 링크는 레퍼런스 포안트와 시작하고 끝난다．
만일 레퍼런스 포인트가 링크 정보를 가지고 있는
파일 안에 있다면 이것은 resource라 할 것이다．
다른 파일 안에 들어 있다면 이것은 /ocatoi콰 할 것
이다. 레퍼런스포인트는모든파일을설명하거나
하나의 축적물（우리가 짧게 다룰 예정인 XFointer
와 함께）
을 설명할 것이다．
레퍼런스 포안트 점l의하기：
의
1, 링크될 파일（하나의 파일 안에서 포인트）
레퍼런스를 만든다. <ref－이emenㅎ를 입력한다．
여기서 ref element 자리에는 레퍼런스 포인트
에 관한 정보를 포함할 xM. 문서 안의 요소
이름이 들어간다．
2. 새nk:切Pe="locator" 를입력한다. 이것은이
링크세트를 포함하는 파일 밖에 레퍼런스 포인
트가 있다는 것을 알려 주고 있다．
또는】
clink:bpe=hlresource" 를 입력한다. 이것
은 링크세트를 포함하는 파일에 레퍼런스 포인
트가 있다는 것을 알려 주고 있다，
3. 치ink:href="URL"을입력한다. URL자리에는
설명될 외부 포인트의 위치가 들어간다. 만일
파일 안의 특정 포인트나 부분을 지정하려면
XPointer를 첨가해야 할 것이다 (p233 참조？.
4. xlink:role="id"를 입력한다. 여기서 id는주어
진 레퍼런스 포인트를 의미한다. 하나의 포인트
를 다음 것과 연결할 때 이것을 사용할수 있다．
5. 원한다면xlink:title을첨가할수있을것이다.
6, 필요하다면다른속성 또는컨텐츠를첨가한다．
7. 평상시대로태그를마친다．
8. 당신이 링크를걸고싶은것이나링크를끌어오
고 싶은 각각의 레퍼런스 포인트에 대해 1-6번
을반복한다．

예제의소스 코드는 www. cookwood. corn off 있습나다．

229

===== PAGE 218 =====
217 =====
Chapter 16

연결 정의하기
지금좋은부분이 나왔다. 가능한 링크포인트를
정의하면 dots를 연결할 수 있다．
연결 정의하기：
1. <connection_elemenㅎ를입력하여 하나의
포인트에서 다음 포인트로의 연결을 정의한다．
connection element 자리에는 연결 정보를
포함할 태그의 이름이 나온다．
2. 그다음）
dink:汐pe="arc" 를입력한다. 이것은
연결을 정의할 것이라는 것을 지시한다．
3. xlink:from='id"를입력한다. id는 랑a가시작
되어아 하슨 레퍼런스 포인트 (p229의 4:)를
위해서 정한xliri]c:role의 값과상응한다．

m
＝ 욘닐● ＝＝。Um灌＝ ＝●。

4. 다음에xlink:to="ici＂를 입력한다. Id는 링a가
차정해야 하는 러）퍼런스 포인트 (P229의 4벤를
위해서 정한xlink:role의 값과상응한다．
5. 다음에딨ink:show="where＂를입력한다．
where은 설명된 데이터가 어떻게 어디서 나타
나는지를 설명한댓. 선택 사항들은『eHace,
embecled, new 그리고p227의 6번에 자세한
사항이 설명되어 있다．
6. 다음에）
dink:show="when＂을입력한다．
when은 설명된 데이터가 페이지와 함께 로딩
되어야 하는지 (nload) 또는 몇 번의 사용자
를 정한다．
action 후 해야하는지 (onRequest）
7번을
보자．
자세한 사항은 p227의
7. 원하는만큼의 다른속성을첨가하고1번에서
시작한 connection_element를 닫는다．
8. 정의하기 원하는각각의 연결을위해 1-7번을
반복한다．

230

卽．
琴i

code.Httflk 二

∼

ㅋ1哨

<linkset xmlns:xlink=
"http://www.w3.org/1999/xlink">
<resources xlink:type="extended"
xlink:role="animol resources1'
xlink:title="Additional Sources 하
Information">
<anim이_info xlink:type=미ocator"
xlink:href="tiger.xml" xlink:role="tiger"
xlink:title="Tiger"!>
<animal-info xlink:type="locator"
xlink:href="panther.xml" xlink:role="panther"
xlink:title="Florida Panther"!>
<animal_info xlink:type="locator"
xlink:href="rhino.xml" xlink:role="rhino"
xlink:tffie="Rhino"/>
<animal_info xlink:type="locator'
xlink:href="otter.xml" xlink:role="otter"
xlink:tiile="Great River Otter"!>
<connection xlink:type="arc" xlink:from="otter"
xlink:to="panther" xlink:show="replace"
xlink:actuate="onRequest"/>
<connection xlink:type="arc" xlink:from="panther"
xlink:to="rhino" xlink:show="replace"
xlink:actuote="onRequest"/>
<connection xlink:iype="arc" xlink:from="rhino"
xlink:to="tiger"xlink:show="reploce"
xlink:octuate="onRequest"/>
</resources>
그림16.7여가에otter폐아자에저panther폐아지로,panther
저rhino 괘이자로, rhino페아자에서 tiger페이지로
페이자이）
가 있다．
연결하는 4 개의간단한 예저）

===== PAGE 219 =====
218 =====
Links and Images: XLink and XPointer
至． , ,

，ㄴ｀ d,，찬＜小 code.fflink=＝止됴보－

羅茸目풂

《＝
dinkset xmlns:치i미
"http://www.w3.org/1999/xlink">
<foodchain xlink:type="extended xlink:role="'prey"
xlink:title="Tiger Food">
<animal_info xlink:type="Iocator"
xlink:href="tiger.xml" xlink:role="predator「
xlink:title="Tiger"/>
<animal_info xlink:type="locator"
xlink:href="deer.xml" xiink:role="prey「
xlink:title="Deer"/>

'/ 1:P
■ 똑같은xlink:role 값을각각의 원하는 레퍼
런스 포인트에 부가하여 하나의 단계에서 복수
의 레퍼런스 포인트를 다른 것과 연결시킬 수
있다. 그다음에xlink: from이나 xlink:
to를사용할 때 주어진 역할을 가진 2든레퍼
런스 포인트는 연결될 것이다（그림 16.8).

<onimal_info xlink:type="tocotor"
xlink:href="wild_pig.xml" xlink:role="prey'
xlink:title="Wild Pig"!>
<animal_info xlink:type="locator"
xlink:href="fish.xml" xlink:role="prey"
xlink:title="Fish"/>
<connection xIink: ype="orc"
xlink:from="predator"xlink:to="prey"
xlink:show="replace"
xlink:actuate="onRequest"/>
</fooddlain>

。●m= ＝口＾ 。＝=m^ ＝。＝m

그림16.8 여기에는 링크세트의 다른 예제가 밌다．그라나 아번에
tiger.xml 파일은 제걔의 prey 파일각각에 랑크하고자 한다．
단차모든predator（육식동물7 叫 경우 하나밖이）없q)와세걔의
모든 먹아들을 연결하는 하나의 연결만을 정의하면 된다．

예자의소스 코드는 www.cookwooct corn에 있습나다．

23 l

===== PAGE 220 =====
219 =====
Chapter 16

링크세트 사용하기
개별, 독립적인 파일 안에서（하나의 레퍼런스 포인
트를 포함하는 파일에 속해있지 않은）확장된 링크의
모음을 링크제트라고 한다. 파일이 링크세트를 이용
하기 위해서는 링크세트의 존재를 밝혀 주어야 한다．
림冒세트 시용하기：
1. 문서의 루트요소 안에서（또는당신이 링크를
만들고 있는 요소안에서）xmlns:넜ink='http:
//www.w3.org/1999/치ink" 를 입력하여
)0血k 이름공간을 선언한다. 더 자세한 사항은
8장의 XML의 이름공간사공하기를 참조한다．
2. XML문서에서는＜이ement를입력한다．
element 자리에는 링크세트에 대한 정보를
포함할 요소의 이름이 들어간다．
3. Hink:type="extendeci" 를입력한다．
*
●
벼
＝灌 “口m＝ 玄＝

4. 그다음치ink:r이e="extern배inkset'뺨을입력
한다. 이것은 외부 링크세트의 존재를 알려준다．
5. ＞을입력한다．
6. ＜치ink:Iocator= 'LJRL＂을입력한다. Ul?I은
링크세트의 위치를 지시한다．
7. <／이ement＞를 입력해 2번에서 시작한요소를
닫는다．

I, np
■ 브라우저 안에서 이것이 실제 어떻게 나올지
누가 알 수 있을까？

232

諷－

c0de.HnH

<endangered_species xmlns:xlink=
"http://www.w3.org/1999/xlink">
<animal>
<name language="English">Tiger</name>
<foodsupply xlink:type="extended"
xlink:role="external-linkset">
<xlink:locator="tigerfood.xml"I>
</faodsupply>
그림16.9p231의그림16.8에서 만들파일은tigerfood.xml이라
부르기로 하자. Endangered Species XML 문서 인뎨서 아라한
랑크들을사용하가 위해서는 여기서보여진 외부 링크세트를 호출
할 필요가 있다．

===== PAGE 221 =====
220 =====
Links and Images: XLink and XPointer
code.KItnk斗詠－－壅g…一＝叫

파일의 부분을 링크하기

<source xlink:type:="simple" xlink:href=
"http://www.cookwood.cpm/xml/examples/
xlink/tiger.xml#xpointer(animal[positionU= 11)
"xIink:roIe="info source"xlink:title="Source of
Information" xlink:show="replace'
xlink:actuate="onRequest"/>

모든 파일을 링크하는 대신에 특정 파일이나 파일의
범위를 링크하고 싶을지도 모른다. 이러한 것들을
XPointer로 할 수 있다. XPointer는 XFath를 이용
해서 파일의 특정 부분을 정의하고 다음에 그러한
부분에 링크하게 한다．

그쾀姓10 아XPointer는tiger.xml 문서에저 첫 animal 요소를
가라킨다．

파일의 부분을 링크하기：
p226의 3번 또는 p229의 3번처럼 xlink:href
속성의 값을 쓸 때 URL 대신 또는 후에 #xpointer
(expression）
을 입력한다. expression 자리에는
연결하고자 하는 파일의 특정 부분을 정의한 )(Path
절이 들어간다．

'/ nm

■XPath 표현에 대한 더 자세한 사항과 그들을
이용해서 XML 문서의 부분을 정의하는방법을
알고 싶으면 11장의 XPath 괘턴과표현을 보면
된다．

■XPointer는XPath안에서 사용할수 없는 몇
개의 여분의 함수를 포함하고 있다. 우리는 다음
페이지에서 이들 중 두 개를 다룰 예정이다．
■ 여기서는XPointer의 약간의 맛을보여주었을
뿐이다. 현실 상황에서 이것을 테스트 하기 전
까지는 특정 상황에서 가능한 것만을 주는 것은
피하려고 한다．

예제의소스 코드는www.caokwood.com에 있습나다．

233

=

■ 만일 < 표시가 속성의 값 안에서 나타나는
XPointer의 부분이라면 피해야 한다. 대신시t;
를사용한다.

。* 。 ＝

■ 刀Pointer 표현 안의 괄호 앞에＾이 선행되는
것을피해야한다. 이것과상응하는괄호는그것
을 피할 필요는 없다. ^ 또한 피해야 한다 (M처
럼 부가의＾표시는 피해야 한다）
.

= = = ＝ 山 呻。 七 。 ＝

■ 만일URL을생략한다면XPointer는최근파일
（링크를 포함하고 있는 것）안의 어떤 것을 지정
한다．

===== PAGE 222 =====
221 =====
Chapter 16

가장 간단한 XPointer 만들기

讐口

XPointer는 II)타입 속정을 쉽게 정의ㅎ庭ㄹ록 디자
인 되어 있다. 만일 ID 속성을 가진 요소에 링크를
하고 싶다면 XPointer는 단순히 그 속성의 값으로
구성되어 있을 것이다．

<source xlink:type:="simple" xlink:href=
"http://www.cookwood.com/xml/examples/
xlink/tiger.xml#T143"xlink:role="info source"
xlink:title="Source of Information"
xlink:show="replace"
xlink:actuate="onRequest"/>

一

: code.Hlink '

: = 1一＝굴二큐＝？큐갸陋＝

가장 간단한 XPointer 만들기：
1. ＃을입력하여 XPointer를시작한다．
2. id를 입력한다. 여기서 Id자리는연결하고자
하는 요소를 위한 ID 속성의 값에 상응한다．
·／ 1iF心
■xpointez라는 단어와괄호는 완전히 생략된다는
사실을주의한다.

。
m
,U
，●*＝훈님玄으｀ ㅌㄵ·fm= ＝

U ID 타입 속성과 (52p에 자세히 설명되어 있는）
속성의 이름이 ID（또는 Id）
인 속성과는 혼돈
하지 말자. 후자의 경우에는 )(Pointer는
xpointed//*[@ id=T?valuehl]）가될 것이다．

234

그림16.11아 XPointer는ID 속정 값이 T143인ID 타입 속성을
포함하는요소를가라킨다．

===== PAGE 223 =====
222 =====
Links and Images: XLink and XPointer
口

:7

뢸 code.K1I.,k

巨j

<source xlink: ype:="simple" xlink:href=
"http://www.cookwood.com/xml/examples/
xlink/tiger.xml#/1/1"xlink:role="info source"
xlink:tille="Source of Information"
xlink:show="replace"
xlrnk:actuate="onRequest"/>

걸어 다니는 XPointer 만들기
다음으로 쉬운 종류의 刃Pointer는 글자 그대로
원하는 요소에 이를 때까지 XML 문서를 걸어 다니
는 종류이다. 이 종류의 XPointer는 공식적으로는
자 시퀀스 (child sequence）
라한다．
겁에 다니는 XPointer 만들기：

그림俎12 tigerxinl 안에저루트요소의 첫번째자식은 endan
gered_species아다. endangered_species의첫번째
자식은 animal 아다. 그래서 아 예제의 빨간색으로 표시된
XPointer는 첫번째 animals소를 가르카는데 아것은 루트의
첫번째자직의첫번째자직이다．

1. ＃을 입력하여 XPointei를시작한다．
2. In을 입력한다. n은문서의 루트요소의 n번째
자식을 나타낸다．
3. /m을입력한다. m은2번에서 발견된자식의
m번째 자식을 의미한다．
4. 내려가야할만큼의 많은레벨수만큼3번을
반복한다．

■ 이 기술을p234에서 논의된 ID 기술과혼합할
수 있다. 예를 들면 #T143/3/1을 사용하여 T143
값을 가진 ID 타입 속성을 가진 요소의 세번째
자식의 첫번째 자식을 찾을 수 있다．

예群의소스 코드는 wwwcookwood.como) 있습나다．

235

。。。＝=．是。 ＝ ＝ 蠟 츰 。 ＝*m4m

V Tip

===== PAGE 224 =====
223 =====
Chapter 16

XPointer 범위 만들기

三陋覃표닐柒7 袁＝∼－→＋一튿 code.Hlink 囊큔毛三癡芼蚤큰＝ㅌ身＝헌H．彗

만일 문서 안의 두 개의 주어진 포인트 사이의
범위를 링크하고 싶다면刀Pointer의 range-to
함수를 사용할 수 있다．

<source xlink:type:="simple" xIink:href口
"http://www.cookwood.cpm/xml/examples/
xIink/tiger.xmI#xpointer((animaI[positionU=1])
/range-to (animol[positionU=2]))"
xlink:role='info source"xlink:title="source of
Information" xlink:show="replace"
xlink:actuate="onRequest"/>

XPointer 범위 만I기：
1. XPointer를시작하기 위해서＃xpointer
（를
입력한다．
2. (start_expression)을입력한다．
start_expression 자리에는 원하는 범위의 시작
을 가리키는 )(Path 표현이 온다．
3. 加nge-to를입력하여 범위를원하는것을
알린다．

各＝ 星， 으＝ 奐 ＝ 。m= ＝
。
●
노
U
。
m

4. (end_expression）
을입력한다. end_expression 자리에는 원하는 범위의 끝을 가르키는
XPath 표현이 온다．
5, 마지막으로）
을입력하여 刀Pointei를마친다．

V Tips
■ 모든괄호를주의한다．
■ XPath표현을만드는것은II장의XPath.괘턴
과표현에서 더 자세한 정보를 얻을 수 있다．

236

그림16.13 XPointer는 tigerxML 파일 안에서 첫번째와두번째
animal 요소 사아의 범위를 정한다．

===== PAGE 225 =====
224 =====
부록 (Appendices)

237

===== PAGE 226 =====
225 =====
XHTML
자TML

서론에서 설명하고 이 책을 통해서 보았듯이 XML
은 이것을 둘러싸고 있는 과대 선전만을 가지고는
- 최소한 아직은 - 살아남을 수 없을 것이다. 많은
브라우저들이 XML을 지원하지 않고 있고, 지원하
는 것들도 부가적인 기능들, XSLT, XPath, XLink,
XFointer와 같은 부가적인 기능들을 지원하지는
않는다. 이러한상황은XML페이지들을서비스
하는 것을 매우 위험하게 하는 상황이다．

XHTML은 HThIL과XML을 합치는데 매우 유용하
다. 이미 10장에서 XHㄸML을사용했고XML의
엄격한 요구 사항을 만족시키며 첨가된 XSLT,
HTML코드를사용했으며, 이는실제XHTML이다.
나는 Xll콰는 별도로 XHTML을 사용하는 성향이
있음을 인정한다. 왜냐하면 XITI取4L은 XML에서
사용하는 정보를 표시하는 기능 없이 XML의 엄격
함을 가지고 있기 때문에 적은 성과를 위해 많은
수고를 해야 한다．
주주들을 위해 사업을 하는 어떤 브라우저 제조업자
들도 HTML 지원을 중단할 것이고 지원을 시작할
가능성은 거의 없다. 유용한XML 페이지를 실제로
보여줄브라우저가나타날때까지는mm을, 정보
를 저장하거나 경영하고 이것을 H呱｛I로 변환하여
브라우저에 보이게 하는 것이 더 일리있는 행동일 것
이다．

239

X＇뻐3尸

W3C는 사람들이 HT兀을 XML로 전환하는 것을
도와주는 매개 언어를 개발하고 있었다. 이 새로운
언어는XHTML이라불리우는 것이다. 표면적으로
이것은XML의 엄격한 syntax 상騙子칙 伽p.
//www. w3.org/MarkUp)을 가지고 쓰여진 HTML
태그와 다를 것이 없다．

===== PAGE 227 =====
226 =====
Appendix A
tode.Hml 聳느：

어떻게 브라우저가 구별할 수 있을까？

三ㅁ…________

XH呱4L과HTML은 다르게 생기지 않았다. 태그
이름들은동일하고신택스는매우유사하다. 그렇다
면 브라우저들은 어떻게 XHTML을 사용했는지
아니면 HIML을 이용했는지 알 수 있을까？해답은
파일의 확장자에 있다．

<hhnl><head><title>Otters in
XHTML</title></head>

그리고 최근까지 XML 페이지를 특히 링크와 이미지
등을 제대로 보여주는 브라우저가 없었기 때문에
신택스에 주의를 기울이는데도 불구하고 아마도
XH呱4L 페이지를 EI爪楓L 페이지처럼 보여줄 것
이다．

<bad가)gcolor="#ffcc99" text="red">
<center><img src="otter. jpg"/></center>
<p>Animal species are disappearing from the
earth at a frightening speed..c/p>
<p>According to the World Wildlife Federation, at
present rates af extinction, as much as a third
of the world's species could be gone in the next
20years.</p>
<hr width="50%" size="5" noshade="noshade"/>
</body></html>
그림Al 여가에는xL 문서의보가가 있다. 이것은 HThU로
오헤받기 쉽차만 작성하는데 애우 엄격한 규칙이 칙용된다．
乫<sties ,n )CHTML H'C cioti Int,,r,st yip,0.5,
EV

트*

4」
Bsok

吟ooois, loth

<ci,
.

→

j
s1叩

口

닌텨p

」

Rdm功

L4寸
（$
H色，

만일 파일을 .htm이나 .html로 저장을 한 브라우저
는그것을wTh 처럼 다룰것이다. 만일 .Xml이나
같은 파일을 위한 확장자를 사용했다면 브라우저는
그것을 XML처럼 다룰 것이다 (xhtml 확장자를
다루는 것은 없다）
.

<?xml version="l .0" ?>

A寸,e시C F \sindoo'o,

m 口m· 。。 多● ＇
卜多。 ＝닙 ，●·뇰。 ，

汕1nahpecien me thisPpeoci,yfro.m thee耐h at a frsgbte회ss媤 apsed:
A」
Accoso. sgto the Wodd 꾸md匠 Fedsratsoo. 毗 Preser,tetes 01e,stsocton, ac
uch as a dad <1the W.dd's species c.미d be g.ne m the east 20 year$

＝」

그림A.2 만일 문저에.htm이나.挑珌 확장ㅈ陽쓴다면 보다 보기
좋을 것아다．
`yocksis1och,.is 川d M<,s.oit l nto,nos Esploso,
Eke

Eds

8aㅄ

yso.

Ftoi0s,
0

工．oth

j

s*야》

Hek
-j
Rme寸｀

소
Hem

)) Lids,

샌山e미a. 尸，
4,4,54.05sI

尸G.

<入rnt versiofl="l d1H>
→ d,tmto.
- 간伯ad>
ototleo.Otters in XHTMLo.ft,bes
《／head》
‘맣ffc.,99" teotb*"red",
<body bc히Or．
<ce伏er>
<hey OrC= ’이HerJP·“ />
c/center>
<<<Animal species are disappesring frono the essth of d
fH汕tenlnq 5p·죤d,c/n>
三f Lord sOrest
咽 D驪

그람A.3.끄끄／확궝脾陽 가지고 (2라고 스타일 사트 또는 다른
부가요안 帥觸z별코드는 계급 구조 형태로 보여질 깃이다．

240

===== PAGE 228 =====
227 =====
＞어TML
Co e．
刪n1E

I

I

I

0

1.

.

XHTML 작성법

.』

.I

" e '. .
?>

阿－

\:
<?xml version="

/nr멨．
鷺_ulVU</
LA,
． /...I
neaa><iirie>
- 믄ne띠n
- An11.
nne></ ne
（《
】】
＞
그림A.4 여7/ 할고 있고 사랑하는 태그들ㅇ］
있다. 아린 태그들을
소문자로 입력한다. 족성들과 가치값들도 마찬가자아다．

XHTML은｝
ITML 4와 비슷하다. 만일 HTML 4를
이미 알고 있다면 XH또丕JL을 작성하기 위해 조금의
규칙만을 배우면 된다．
XHTMI. 작성하기：

드口

code.nml

="

'「' ｀心m퀵

<body bgcdOr="#侃c99" text="red">
<center>.cimg src="otter.jpg"/><Icenter>
그림A.5모든족성값들은 인용부호로 감싼다．
墨口

c0de.Hm1笠薑i==-

--＝二＝∼스斗箋

<center><img src="otter.ipg' /></center>
<p>Animal species are disappearing from the
earth at a frightening speed.</p>
<p>According to the World Wildlife Federation, at
present rates of extinction, as much as a third
.hhe world's species co이d be gone in the next
20 yeors..c/p>
<hr width="50%" size="5" noshade="noshade"I>

-rF＝맨＝ㅋ∼「 code.11mI ∼二＝…＝

<hr width=「50%" size="5" noshade=「noshade"/>
그람A.7 명확한족정 아름을 입력한다 帆7孔fL 안叩A7는속성
아름 없아noshade 값을사용함수 있L抄．

回峰‘

2. 이 책에 설명되어진XML작성법, 특히 p23에
설명되어진 부분 구조가 좋은 것을（요약해서
말하자면 모든 요소 - 빈 요소라 할지라도 - 는
마침 태그를 가지고 있고 적절히 중첩되어야
한다. 그리고 인용 부호 안에 있는 모든 속정값
을 잘 감싸고 모든 속성 이름을 명확히 해라）
따른다．
3. p32에 나와있는문서내요소의표현법과p187
에 나와 있는 내부 스타일 시트 사용하刀에 나와
있는 CDATA 부분 안의 스크립트와 스타일을
감싸는 것을 잊지 않는다.
4. a, applet, form, frame, ifreame, 1mg

그리고map 요소들에 대한 이름 속정을 사용하
는 대신에 그 가치를 포함하는 id라 불리우는
ID 타입 속정을 만들어라．

'/ 1iP`
■ 모든xM.문서에서처럼xM.선언（p24참조）
으로 XITI丕4L 운서를 만들 수 있다．
■ 만일 XHTML 문서를 DTI）
에 비춰봐서 유효한
것으로 만들고 싶다면 어떤 Dㅁ
［l〕
가 적당한 것인
지 정해야한다. 더 자세한 사항은 p242에 나온
Xm〕
iL을 위한DTD 선안하刀를 참조한다．
■ (X)I{I爪iL 태그의 도움을 위해서는 B&B에서
출판된 /'7丕iL 4 fbr the World Wide Web
Fourth Edition: Visual QuickStart Guide를
보면 된다. 또는h婢,://www. cookwood.
com/htm14 4e를 참조한다．

예제의소스 코드는 www.cookwood.com에 있습나다．

241

름
＝ ==．鎣뻐글

그림A.6모든 요소들은 알맞거］캄싸졌다 - 위의p와center처럼
걔별 마침 태그로저또는 img와hr처럼빈요소 끝의슬래사로 - 는
갓을 명심한다．

1. HTML4에서의 요소와속성에똑같은이름을
사용하지만 언제나 소문자로 써야 한다．

===== PAGE 229 =====
228 =====
Appendix A

XHTML을 위한 DTD 선언하기

Cj
一莩좇to,je.KmI＝ㅗ→뇩斗受헷美뇩－극뇩由＝口텍
<?xml version="1.0" ?>

ITIML에 세 가지 종류가 있는 것처럼 XITIldL에도
세 가지 종류가 있다. 그 세 가지 종류는 strict,
transitional, frameset이다. 각각의 타입은타입과
함께 입력된 문서 안에서 어떤 요소나 속성이 요구되
거나 허락되는 것인가를 설명해 주는 DTD 가지고
있다. 만일 문서가 XITI爪4L의 특정 타입 안의 규칙
을 따르는 것을 확인하기 위해 문서를 유효화하려면
상응하는 DTD를 선언해야 한다．

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML
1.0 Transitional//EN" SYSTEM
"http://www.w3.org/TR/ xhtml 1/DTD/xhtmll
transition이.dtd">

XHTML．
을 위한 DID 선언하기：
1. XHTML문서의 윗부분그리고XML선언 후에
<!DOCTYPEhimI PUBLIC"-!! W3C//DTD
XHTML 1.0을 입력한다．
2. 스페이스를입력하고유효화하고싶은문서와
상응하는 XHTML의 타입에 따라 Stri比 Tr미卜
sitiond. Frameseㅎ을 입력한다．

m
=：
口
＝
“름토즈요e。 口
。
●

3. 부가의공간없이 /!EN"SYSTEM"http:/!
www.w3.org/TR/xhtml1!DTD!xhtml1-을
입력한다．
4. strict, transitional 또는frameseㅎ을（소문자로
공간없이）입력한다．
5. 마지막으로．
dtd"＞을（빈공간없이）입력하여
DTD 선언을 마친다．

'/ Tips
■ 만일 XH呱4L을 모든 평가절하된 태그와 프레임
세트에서 자유롭기 위해서 XITI以4L을 사용한다
면 엄격한DTD를사용해야한다. 평가절하 되어
진 태그들은 미래（곧은 아니다）
에 제거될 것을
알리기 위해서 W3C에 의해서 표시된다．
■ 만일XH呱4L평가절하된태그를조금포함한다
면 transitional DTD를 사용한다．
■ 만일 XHTML이 프레임세트를 포함하려면 프레
임세트 태그를 사용한다．
■ ㄸ［D에 대한자세한사항은p35를참조한다.

242

<html><head>ctitle>Otters in
XHTML</title></head>
<body bgcolor='#f1cc99" text="red">
<center><img src="otter. jpg"/>c/center>
<p>Animal species are disappearing from the
earth at a frightening speed.c/p>
<p>According to the World Wildlife Federation, at
present rates of extinction, as much as a third
of the world's species could be gone in the next
20 years.</p>
<hr width="50%" size="5" noshade="noshade"/>
</body></html>
그림A.8xH洲ilL 문서를 위해DTD를 정했다면 아것아 특정DTD
안에저잘 지켜지고 있는자를 감ㅈ］하는녜 validatoi룰 사용할 수
았다．

===== PAGE 230 =====
229 =====
XML TOOLS
XML 도구들

간단한 텍스트 에디터 즉, 윈도우의 노트 패드 혹은
매킨토시의 Simple text를 사용하여 XMT을 쓸수
있고, 익스플로러를 이용해서 볼 수 있는 반면에
XML 화일을 변환하고 유효화 하는데 다른 도구가
필요할 것이다．
여기서 이러한 도구들을 찾을 수 없거나 어떻게 사용
하는지 모르거나 또는 시스템에서 작동하지 않는다
고 말하기 전에 이것들은 예제임을 기억하라. 운영
사항이나 어떻게 작동하는지 보기를 원할 뿐이다. 이
장에서는 임무를 하기 위한 도구들이 많이 나와 있고
상황에 알맞은 도구를 찾아서 사용하면 된다. 그 알
맞은 도구는 설명한 것일 수도 있고 아닐 수도 있다．
간단하게 말하면 이 장은 단지 무슨 일이 일어났는지
에 대한 간단한 설명으로 구성되어 있고 각 도구에
대한 단계적인 설명은 아니라는 말이다．

243

X결尸 킁。 ＝

이 책이 출판될 쯤에는 이미 구닥다리가 될 LIRL을
리스트하는 것 대신에 웹 사이트 (p18 참조）
에 유용
한 XML 도구들을 위한 업데이트 리스트를 계속해
서 제공할 예정이다.

===== PAGE 231 =====
230 =====
Appendix B

DID에 관해 XML 파일 유효화하기

包

만일 잘 정돈되지 않은 XML 데이터를 넣지 않는다 4
면 모든XML 파서는 에러를 발생시킬 것이다. 그러
나 만일 xM,문서가 특정 DTD 안에서의 규칙에
따라 유효한 것인지 아닌지를 시험하려면 validator
가 필요할 것이다. 여러 가지의 가능한온라인 사이
트가 있지만 브라운 대학의 Scholarly Technology
그룹의 XML Validator를 추천한다．

냥 ㄴ聊눠眈 -1 1
성 肛Yjh的 本시ta＼」dta[1rt 李ㅒTHL凹枕na2翩

' g ,,/
．·,, ,乫 案, 劈,, ,無,

키『

m駐 汁n" 由^b11,20 m始 n. 1吐1l n1e f. b1 勿U m1y .h 나山b an albIto,)
b by 竗vmg 1b UI口 ulTo no 110n r브뇌
OS'Ldㄱ￡m볍Om01, n녑 ' 工“．
肉1i山it n驪b那b口끄＆ 胛캬 낱口芦 S.1 ab. ni 心楓

卜r천1 v-

sr

■ 가끔하나의 에러가 에러 다음의 모든 것을오해
하게 만들 수 있다. 가끔 리스트의 첫번째 있는
것을 수정한 후 다시 부가적인 에러가 실제 상황
인지 혹은 원래의 에러에 기인된 것인지를 확인
하기 위해서 다시 살펴 본다（이것이 해결되면
해결된 것이다）
.

Lㄸ祉m루
1 0,02000

楓
耐斗윔，
t媤1t갇

1

B縕縕驪醫焄學'
r而표司 cOCJ
--－나

ㅁ O*ppv51r..on“弔o社1學5
U F눕hXmn·3꾸a‘옰c〕
mh
i va；岫눈 , 1i面n

汪논工
＇

，出뇨

。1112
I 11。2。
10100000黨00
1。
0:
.T

B

Vthxv1。
fl p.a COCOS '

瀝日
Instrucbom

너
1니 l

可k1
峀세P=

I ' 11

11. j12

斑

그람刪 특하 많은 이］러를 터］스트 하고 있을 때XML 파일을 복사
하고 텍즈트 박스에 붑여 넣는 것아 훨씬 쉬울 것이
［打에러가보이
는가刀．
tots 21혀ne:volldstinn tlest,Itnormser-nompHod 002101

口

'

。늠。 玄＝ 뭅 콩 내 으 ＝ “至님m= ＝。겯口＞

■ 만일 외부ㅁfD를사용한다면 이것은대중적으
로 사용가능한 것임이 틀림없다. 그렇지 않다면
XML Validator가 이것을 넘어가지 않는다．

驪

1,
) *比0눈죠｀꺾m끄끄驪Ldㄸ一n니出
＇볜1bi` mbn吐出1f.m4好뽀aㅈ펴1ut吐．

2. 온라인상에서는h따湫www.stg.brown.edu/
service/xmlv訌放／
（그림 B.1｝
를 참조한다．

V. 1iPS

} 心 Vh1r'R이*驢d
李Pdr1m力n1』
：m 李c여*Y에d ' bt－γ m

XML Validation Form

STG

1. 문서 안에서 DTD를선언했다는것을기억한다.
자세한사항은p36의 내부DTD선안하기나
P39의 개인적 와부DTD선언하기나 p40의 공용
를 참조한다.
외부DTD 선언하7］

4. Validate를클릭한다. XML Validator는에러
에 대한 유용한 리포트를 준다（그림 B.2).

4 )., 1 國

SCHOLARLY TaCHNOLOOY OROUP

DTD에 관해 XML. 파일 유효화하기：

3. 문서 중공개 접속이 가능하도록만든XML
파일（다시 말해 이것은 어딘가에 있는 서버
안에 있는 것）안에서 쓰거나 텍스트 박스 XML
문서를 복사하면 된다．

므｝덤

三- P450001lt.ut6xMl Validation Ewnn

。
8。

，

8.。14

I'm.

S。
。th

。。
2。
,15.

.。5。 Swray

FD日

回

U：챦'l.1i.t P010210
' 420.1.2唾1221,://wVI.SWI『I00IOO/on,-bolnmloolld/ollln.ISn
r.-。。t 革mTht 。n *11。。.2 40.2,。011.2。
2 511004110*0 雅0ktIt21.
y St no。
n 4 AIrWI。

Validation Results for [user-supplied text]

녘

l=
내恥

"-

髓 늡和吐‘釀口 曲

,1걜기

그림B;2 Validator는 족정 값인 English"의사작 인용 부호를
빼먹섰다는 깃을, 그라고 이문제가부가의 'ghost0 에라 즉, 인용
부호를 넣기만 하연 사라차는 것이라는 것을 밀해추고 있다．

244

===== PAGE 232 =====
231 =====
XML To히S
Xr0 Schema cheamne Service (Mfl6&IEST)xlct._ j

！百
4
E1"

t》
目r介外h

柄
「rrH m 〕

唐
`U卜口F1

P「m1

인．
目
」無
r"

四
＂히

∼，
→, :
a '님fl. T.c, 白cccet4o&a OJP.(TQSA ucnat［鱗 th)et$4ms
玔
--

「－;

1붜茗一

]
二

「
1

哥XML Schema Va1idator, XML
hOutput version
三 XSV versi。n. XSV 1;15711.66 。f2。
。。1。8122 13,11:3。

1. XML과스키마파일을서버에 업로드한다．

iopecificotion

2. http://www.W3.org/2000/06/webdata/xsv
（그림 B.3）
에 방문한다．

下 Use this form for checking a schema which is accessible ma the Web. ondlor
乶 sthema-vel6050ganInstance withaschema of your own

3. 주소록안에 있는XML파일을위한URL을
입력한다．

/Ir0

哥Addresses;

towN ,otkwood totvcttlrenlsr,,0Is cmi fluehams. 000loqoadhai,ti
ntribute
beep G。
rnq D C。
Defaut output is now terd/onl with ao XSLT sti/esheet Selectfallbacks for
browsers which don't support뺘ylbVdYww3org/1999tXSl.JTransfornr
st>teshe副I
Q teutloml * Olftctal XSLT(suit引055. lEA 나dsxML3)
0testtorrl+ earfy MS XSL support (suds yenta 105)
軌extlturrd (styled seruer-nide suits Netscape, older JE)
0rml. but labeled text/plain (works for a〃browser, loll bard to 1066)

'
4
J
l
3
텨；

Net eesarc斗
* 卜枕논14tz咐

그람 B.3 만일XML 화일아 스7/마 파일（아깃은 공식적으로 ㅈ除
가눙하z뀌딸 설명하자 않았다면（아 경우X7k[L 파일만아 충분 조건
아나）
. X人
［L 스7／마 (schema) Validator (KSV)를 가자고 XML
서시험된 파일은 tool&xml과 toolts 溜d이고 아깃은 웹사이트
址竗:1/ ￦ㅠ．
cookwood.corn. xml eats에 나와았다．
ㅈ〕sellemovollclattoul reportlar ItttpJ,

,it,S,

.00t. 芝／寸쿄資蚩資햄目

∼ 熙 只

e

玉＝口Dhte;ifms. n/2.叩/%ivad.t.I 『N.voㅃ
『，
otrasies2cna.닐1o& .,a.%rt) =
心 ＾川J/*t`r*,' O나r吐4（好＾ ㅇe.rc&o 口065.0 650.5000*.
‘口
`
; Schema emlidatiag with XSV iktlll. 66 of 2000/08/22 l3nlbn30
r니
累
ㅣ
l
· Tat-get 0000://000.fiQ*k0*d.C*cclvcaute.tsf *0*10.*,,,!
F
1
簾
(Reel norm htrp:/Ae*rovmokaoudoem.tconlrenraflaolaomt
';
Lesgrlr 155 bylen
1
露
Last Mwii0ed Wad. 06 Sep ItTE 151745 GMT
I
i
Sm-eec A h&13.9 (limo) PHPIS01I on七,enl/llt lkoutPage/404좌 r
1
1 decEit luoso,//on.co*kvvva.v*edcssj
軫
e54_speoloollood000ec,
,d_0000*o,
I
!
· ki:rlatron war strict oraixiry rIta type t5000s'sOuSI
I
!
1 wiameLecs
m
* 뎔上心】
日D 10 5000;/fon.0000700d.ecelalmotoitcsl..K"d
i
· The echeera(o)끄8edfororheola-vabda0on toad 0005000.
「
'
. O*stuoseo-Aaucsse,I true
l
ㅣ
* 1oclseme-eabdlty problem woo foundmone larger
i

璽

4. 만일 XML 화일 안에 있는 스키마 파일의 위치
를 제공할수 없다면 (p73에서 설명된간단한
스7/01/-의 위치 차정ㅎ汐／나 p130에서 설명된
스7/01/-의위치차정하기를 참조한다）스페이스
를 입력하고 XML 파일의 URL 바로 뒤에 상응
하는 스키마를 위한 UHL을 입력한다．
5. 결과물포맷을선택한다（text/htrm에서 가장
운이 좋았다）
.
6. 페이지 밑에 있는Get Result를클릭한다. Xsv
는 이것이 발견하는 문제의 리포트를 보여줄 것
이다（그림 B.4),

'/ 1:P
■ 리포트안에서는 "유효화는엄격하다" 라고써
있을 것이고 instanceAccessed에 해당하는
값으로 "true" 값을줄 것이다（그림 B.4). 이
시점에서 리포트된 에러를 신뢰하기 시작해서
맨 나중 라인까지 신뢰할 것이다．

ㅏ

E Losrolevnl XML sepil-formedoem m.d/or solidity peoceuiog oWpont ㅣ
希
t
0000lnO; 050sairns *03 n. net, eau1000soo os00000eu
I
`40000aoa at tad .t 000100 .f 400,0000 lttpe/i voo.cuokooud.coa/ ='et4

ㅣ

-

l
ll

Problems with U.n srhemo.v.Iidily of thefarg미

;n
. 1d-". O3

n쥑

그림B.4 ㅇ］번의）는 name 요소틀XML 파일 안에 넣었
［打여기
스7/cif 안에서는 쟉아도 두 711의 것이 팔요하다夕. 결과적으로 Xsv는
animal 요소가 너꾸 빨라 끝났다고 말하고 았다．
에제의소스 코드는 www.cookwooricorn에 있습나다．

245

＜흽＝ 。＝＝山님클P트* ＇口m튤m크。

파일의 URL 안에서와스7／마파일각칵의 안에서작성한다. 여가

4

월드 와이드 컨서시엄은 xv1. 파일과 그것에 상응
하는 스키마를 비교하기 위해서 온라인 XML 스키
마 Validator (XSV）
를 제안했다．
스키마를 가지고 XML 유효화하기：

바 NOTICE: This son씨1PHAT두S of a serorce for a뾰인塑土〕
赳9효m雖

彷 ∼ 스즌Jr '

스키마를 가지고 XML 유효화하기

===== PAGE 233 =====
232 =====
Appendix B
釀code.HsIt豪

-

________

X히．
T 연산자로 XML 변환하기

驪口

이제까지 발견된 가장간단하고 최고의XSLT 연산
자는 Instant SAXON이라불리우든 연산자로 이것
은Michael Kay (XSLT Programmers Reference
의 저자이기도 하다）
에 의해서 만들어 졌다. 이 연산
자의 약점은 이것이 윈도우 안에서만 작동한다는
에 알맞은 연산
사실이다. 다른 포맷（특히 매킨토시）
자를 발견하면 책의 웹 사이트에 링크시킬 예정이다．

<xsl:stylesheet xmlns:xsl="http://www.w3.org/
1999/XSI/lranslorm"version="1.0'>

SAXON을 가지고 XML 변환하기：
1. Instant SAXON을다운로드후unzip（압축
풀기）
을 한다 (http.1/users.iclway. co. uk/
mhkay/saxon/instant/htmi').
2. DOS윈도우를열고SAXON을인스톨한디렉
토리로 바꾼다．

<2xm1 version="1.0" ?>

<xsl:template match="/">
<html><head><title>Endangered
Species</title></head>
<body><xsl:apply-templates/>.c/body></htrnl>
</xsl:template></xsl:stylesheet>
그랖B.5XSLT스타일시트의 예제이다．
；프晏客＝code.Hmt
蠶室흣ㅌ＝도呈芬三ㅌ

m졸

<endangered_species>
<animal>
<name language="English">Tiger</name>
<name language="Latin">panthera tigris</name>
</animal>
</endangered_species>
그림B6XML 화일은 叫우 눈에 익은요소들로 구성되어 았다．

3. saxon을입력한다．
，
。
·
小
● V。 ，`HHm님＝ 。 f 灌 ． 毛님m＝ 灌｀ 。七＝ 므뉴

4. 원한다면·o res이t.url을입력한다. result자리
에는 결과물의 파일명이 들어가게 되고 unl은
디폴트 결과 방법을 결정하게 된다．

뇨MS-DOS r.os

바C
『. 드1f!
（므）뷰1ndn니｀ !1
d: C.p,riqSt H,.r. ..tt

加rI 011-I押8

5. file.xnㅔ을입력한다. file.xm/ 자리에는변환하
기 원하는 xM. 파일이 오게 된다．
6. s이e.xsl을입력한다. style.xsl자리에서는
변환 과정에서 사용하기 원하는 XSLT 스타일
시트가 오게 된다．
7, 리턴 키를누른다. 4번에서 파일 이름을정해주
지 않았다면 결과물 파일은 표준화된 결과가
나올 것이다．

.1림B 7 ㅇ何서보여진 rB. command line//서 Saxon을 실행할
수 있거나혹은 UltraEdit와 같은 텍스트 편집가에서 실행할수
있다．
塢MS-DOS F,n

VI 1iP`
■ 이 책의 첨부 문서에는 Saxon에 대한 더 자세한
사항이 나와 있다．
■ UltraEdit와같은 텍스트 편집기와함께 (DOS
명령에서 Advanced 〉를 선택한다）Saxon을
실행시킬 수 있다. 이것은 Saxon을 훨씬 쉽게
만든다．

目回.

'

i Lr旴U* d n, 니nmUu, 끼각
C C珏OIy『1q1d H1rrn,M 1 如r쵸 1qn'
c八나nmm1SC".

`99n

.

C: \)'d 忖. 뙨"-

.5'.

5:5H, I. 醜枓P"t功14 san
C)'Hy 5.5,5'. ............m

X, 1 t . e, r γm

155.11
.', c..t. .t ' ".t. 'tlbtM;
Diet. , Sttp,et. i. .'C. .t,e.tC
<titI. >5.4.s e e4 Spec i. .<ltltl.

T

.ku. ,(. .If.
r>

；洑誌，
Ii, i;

그림B'8 만일 결과울 파일을 정하자 않았다면 결과물의 변환은
standard outputP_ 보내진다．

246

===== PAGE 234 =====
233 =====
SPECIAL SYMBOLS
특수 기호들
XML 문서에 영어 알파벳의 어느 글자나 어떤 숫자
라도 첨가할 수 있고 모든 컴퓨터 시스템이 그것을
올바르게 해석할 것이라는 자신감을 가질 수 있다．
그러나 문서에 외국 문자 혹은 특별 기호 등이 포함
될 경우 페이지에 이것들이 제대로 보여지는지 확인
하기 위해서 특별한 코드를 사용해야 할지 모른다．
Unicode 문자 세트는 XML 문서의 표준 문자 세트
이다. 이것은 각각의 글자, 숫자 또는 기호 등에 하나
의 숫자를 부여한다．

다음 기호들에서는 글자 레퍼런스를 사용할 수 없다
（외래 글자의 숫자들이 정보를 위한 차트안에 포함되
어 있음에도 불구하고）
: 느낌표 (!), 우물 정자 (#),
달러 기호 ($), 퍼센트 기호 (%), 괄호“ 0", 별표 (*),
덧셈 기호 (+), 뺄셈 기호 (-), 마침표 (.), 쉼표 (,),
슬래시 (/), 콜론 (:), 세미콜론 (:), 등호 (=), 의문
부호（?), 삼각기호（^), 밑줄기호（夕, 굽은괄호（m,
.
수직 기호 이）

247

＂경승 m＜클口。 ＝

불행히도 극소수의 텍스트 편집기（또는 편집기가
운영되는 시스템）
만이 Unicode를 지원한다. 이 문제
에 대해서는두 가지의 해법이 있다. 하나는 평소대
로 문서를 작성해서 이것을 Unicode로 변환하는
방법과, 다른 한 가지 방법은 외래 글자에 효과적인
방법인데 외래 글자를 설명하는 글자 레퍼런스를
사용하는 방법이다．

===== PAGE 235 =====
234 =====
Appendix C
글자 레퍼런스 사용하기
Unicode는 모든 캐릭터 편집기와 Os의 표준인
ASCII와127글자를 나누고 있다. 이것의 의미는
영어 알파벳과 모든 숫자, 일반적인 기호 등을 포함
한ASCII 글자들이 어떤 시스템의 키보드로부터
입력될 수 있다는 의미다. 128을 넘어가는 Unicode
글자들은 글자 레퍼런스를 이용하여 문서 안에 삽입
될 수 있다．
굴차 레퍼런스 사용하기：
1. &＃을입력한다．
2. n을입력한다. n자리에는원하는기호에상응
하는숫자가들어간다．
또는xn을 입력한다. n자리에는 원하는 기호에
상응하는 16진법 코드가 들어간다.
3. ；을입력한다．

'/ Tips
■p249에나오는테이블을참조하여서부유럽
언어의 방언에 상응하는 숫자를 알 수 있다．
m
● V= 0느잽· “ ，으븝느。 ㅎm＝ 丁＝

■p250에나오는테이블은일반적인기호들에
상응하는 숫자를 포함한다．
■ 다른 글자에 대한 16진법 코드를 알고 싶다면
http://charts.unicode.org를 참조한다．

code.eml :

<endangered_species language="Catalan">
<animal>
<name longuage="Catalan">Tigre</name>
<name language="Latin">panthera tigris</name>
<threats><threat>ca&#231;adors furtius</threat>
<threab.destrucci&#243;de I'ambient.c/threah
<threat>tr&#xeo;lfic de ossos de tigre per Ia
medicina tradicional xinesa (TCMk/threats>
</threots>
</animal>
</endangered_species>
그림c' 이 예저）안에서는ㅈj) 개의방언 글자들이세개의글자
레과런스를가자고 등장하고 있다. 처음 두 걔의것은 수로 표ㅈ］되는
것인 반면에 나머자 하나는 石진법코드아다. 두 지스템 다 등가의
것들이다．
打－긴∼：' －國flIer/I/ at1ses/`fecrolderfsymbols/t.flerrat.zml

뻑 m ,* … ,0

■HTML에서 일반적으로사용되는&agrave나
&oacute 등의 엔터티 레포런스를 이용하고
싶다면 DTD에서 선언되어야 한다 (p.56 참조）
.

248

-

…

0UO.5汀U:10a tHT5t4Q&A 釀p$瘢 꿸V1싫.q'
町眄

竇
霽

亘

뚜

춘蹇》
回펌

'a .

各X臘 鈿놂
＇m…

Cxml varsion='1.0" encod,ng="tSO-88594' ?>
csndangered..species lanquage='Cata油IC>
<animal>
<name lan9uage=tataIan">TIgreOnamo>
<name language=tatIn'>penthare tigflsc/name>
《threars>
＜軫，
reat>ca5ador5fU1卄USC／卄rreat>
crhreat>destru口」
. do Iamblentnthreat>
<threatMrafflc do ossos do t눕re perm
medictee tradlcion川 Olnesa (TcM).r'threat>
C/threats>
<Janrmal>
c/endangered_SpecIes>

昏L. Im.rSC.z口r.

■ 적당한Os시스템 또는설정된폰트가 없다면
브라우저는 모든 Unicode 글자를 보여줄 수
없을 것이다．

『一陋큭

<?xml version="1.0" encoding="ISO-8859-1"?>

以

.2림c2 브라우저로 모았을 때 글자 레퍼런스는 알맞은 방언 글자
(은 특수 기호？에의해서 z泂］
돨 것아다．

===== PAGE 236 =====
235 =====
H뻐》

迅 설 迫 吟 今 汕 ㄴ m 巾 쩍 쩍 쩍 §育 一 乂 乂 쑹 옵 온 地 吟 工 ㅉ

닥》

컥
b.
ㅇ
.\

侍》

닥》

4t=
t9
ㅇ
UI

눋뻐，

孝＝

角＞

요

'9

令’

H뻐／

汁

느d

侍》

孝

H
畛
，ㅇ

`r)

侍》

14:
'9
ㅇ
UJ

4

t9
tJ.
H

<=

tl1

,1

.

`1

1

dI

-

封
><

느I

)
익

C.

凶

D， 亡

tl卞

8

4:

t9

tJI
U/I

팎
',.

＜=

｀니
（겁：

t치 ()
（·》 醜

（희＞

言】

(-

：>

4
><

：겪

.>

44:
님

1

（스

四 >

ㅊ＝

4卜
><

`1

4:

R`

t9
H
閃

CD>

誥 蠶

(1*:

UJ
(J,

c

너

1

딛
니

컥
卜.

芯

==

t.
bJ
t9

c청
＇

,1

1

凶

딛
山
的

柚

H
c
치

：】：＞ㅔ

(7`

(.

4
t9
4,
,.

=/

令.

侍）

汁

1

令）

갸
4h
bJ t9
(J」 딛
的
.,

. Q

너

UI
t9

m

·

莽

`.

汁 汁

心
U/I

H
口
4,

》

令）

밖

딛
\D
UJ

>,

ㅇ＝

ㅇl

UJ

1

.\

U/i

亘

4

'9
H
'9

.

ㅇ

驢9
H

컥

自

侍｀

C:

4뇨

니

.

4:

U
U
U』 t9

乙；
m
U.)

44:
><
仕1
口｀

쐼
팎
U」 t9
t9
(JJ 』， 4,
的
口
o\

요

U1

剪 發 芽 識
杜〕

,1

4h
t9
H
H

0

0\

汁 令 汁 F寺）

0

H

4t=
>4

t9
山

芼

p乫

g.

4
t9
t9
口｀

p》

g=

'

4t=

汁
4
'9

C>

t,J

仕I
U/i

令》

誅 識
뵤

(J1

뵤 t

食》

ㅇl

(.J

孝＝

'

t9
4,
t9

油

'

컥

C

箋每

t9
4,
UJ

令.

C

Ll1
ㅇ

汁

p

4
14:
t\J 卜.
'9
',.
I-,>
4,

m,

活 ㅂ 口 蓄 t치 ru ru

bJ
ㅇ

侍》

4t=
t9
t9
的

m:

湊 汁
汁 汁 汁 汁 伽 汁 汁
4
4t=
님

0>

t9

밖
닥》

軫.

芯 誥

臼

黨 汁芽 Fa= 汁 剪汁 募 汁芽 汁芽

각b
,0
t9

>'

汁
脅 汁 汁 汁
각

；工＞

4卜
겪 4
乂 님
><
) （스 （스 （스 （스
4뇨
R.

食.

封
-

＞귄

芽 識 芽 芽 芽
결경 . U .

貫量

(JI
'9

럽，

4卜
X
m
口

斟

H
口
.,

>=

汁 汁 汁
汁 汁
4卜 14:
컥

팎
tS.)
UJ
UJ

（心，

醫 黨 汁 汁 汁 =汁酋 甚

．》

ㅂ
四 >

纛＝

tl탭

닥）

汁 汁

（희／

箋
口 . . U

1

令 汁

니

44:
t9
H
,D

芽 芽

4
t9
IS.)
ㅇ

d,

的

r겨

＄』카)IUnII) 체 키때n요

舅. ㅁ汁 識汁 汁芽 촐차=識

노)

4t=
t9
ㅇ
딛

ㅂ，

汁 汁 汁 汁

聿
'9
ㅇ
t9

口1: t거＞

醫醫黨 汁 汁 黨 汁 藤 汁

U

口1 《，

Z1

醜

버

n

t11 .

(m)

*d/

醫蠶

Hm,

募 識汁 識汁 汁 驪?S 舅 霽 汁 蓄汁 黨C훵 募
田U

t9
UJ
凶

ㅒ＞

油 汁
4놉

4b
'9
(JJ
山

눋． :

芽 ru
剪 芽 芽 《스
芽 盡
（스 r,

汁

t9
ㅇ
니

汁
汁
4

- =

'-I

141

r넙

｀』

브，

聖

r.

甘1
니

-

甘1

rio>4

℃
m
m二0百季ㅇ ＝

出 =巾以

===== PAGE 237 =====
236 =====
Appendix C
표 ∥： 기호
기호

표기1

표기 2

기호

" " 춈

HT/m., XML과 Web

표기 1

표기 2

Math and Sci《〕nce
&#6l·
，

&#x3D;

+

&#43;

&#x2B;

&#x2F;

&#45·，

&#x2D;

&#126;

&#x7E;

x

&#215;

&#xD7;

&#64;

&#x40;

&#247;

&#xF7;

&#95;

&#x5F;

士

&#177;

&#xB1;

<

&#60;

&#x3C;

ㄱ

&#172;

&#xAC;

>

&#62;

&#x3E;

%

&#37;

&#x25;

&

&#38;

&#x26;

#

&#35;

&#x23;

/

&#47;

@

&#8240;

&#x2030;

.

&#176;

&#xB0;

P

&#181;

&#xB5;

&#40;

&#x28;

&#41;

&#x29;

&#91;

&#x5B;

&#93;

&#x5D;

ㅣ

&#124;

&#x7C;

4

&#162;

&#xA2;

\

&#92;

&#x5C;

$

&#36·，

&#x24;

￡

&#163;

&#xA3;

￥

&#I65;

&#xA5;

Other punctucition
&#44;
&#46;

&#x2E;
&#x3A;

TM

&#8482:

&#59;

&#x3B;

c)

&#169;

&#xA9;

@

&#174;

&#xAE;

&#42;

&#x2A;

&#8224;

&#x2020;

&#182;

&#xB6;

&#167;

&#xA7;

&#x21;

&#161;

&#xA1;

Legal

Typographk

&#63;

&#x3F;

*

&#191;

&#xBF;

十
1
§

&#39;

&#x27;

&#34;

&#x22;

&#8220;

&#x201C;

&#xBA;

&#170;

&#xAA;

&#8221;

&#x201D;

&#8216;

&#x2018;

·

&#183;

&#xB7;

&#173;

&#xAD;

&#160;

&#xA0;

&#8217;

&#x2019;

《
《

&#171;

&#xAB;

Non-breaking
8pace

>>

&#187;

&#xBB;

&#123;

&#x7B;

&#125;

&#x7D;

250

&#186;
a

Soft hyphen

{
I

&#x2122;

：이

&#33;

i
'

Currency

&#58;
!

'7

씀， ㅌ＃, 으겹H

;

&#x2C;

%Y〕

(
)
[
]

===== PAGE 238 =====
237 =====
COLORS IN HEX
16진법 색상

이 책의 웹 사이트에는 숫자의 16진법 코드와 함께
있는 여러 개의 색상 테이블들이 있다 (h婢）
．‘〃
www.cookwood.conm山끄／4_4e/colors). 이것은
원래 HTML 4 책을 위해 만들어진 것이지만 XML
문서에서 사용하는 데에도 아무 문제가 없을 것이다．

251

. 굼． X

색을 표현하는데 있어서 색상의 red, green, blue
성분을 0 - 255의 숫자의 형태로 표현하여 색을
정의할 수 있다. 이 이야기를 복잡하게 한다면 각각
의 숫자에 해당하는 16진법의 숫자로 이 성분을
정해야한다. p253에 있는테이블은red, green,
blue에 해당하는 각각의 16진법 수를 나타낸다.

＾。＝=

배경의 색 뿐만 아니라 텍스트나 링크의 색도 선택할
수 있다. 넷스케이프나 인터넷 익스플로러 등의 브라
우저는 16개의 미리 정의된 이름을 가지고 있다．
silver, gray, white, black, maroon, red, green,
lime, purple, fuchsia, olive, yellow, navy, blue,
teal그리고aqua등. 어떤브라우저들은또한
magenta (fuchsia와같은 색）
와 cyari (aqua와
같은 잭）
을 인식할 수 있다．

===== PAGE 239 =====
238 =====
Appendix D

5=

+
田뜨
T

그림 D.1 포토십꼐서, Cclor Picker 대화
상자가 나타나도록도구 상자의색장상자
중 하나를 클릭한다．

‘걋

<？

〕* 1릎

\

'7

?

t,

多｀

才/
晶 )
a

2. 나타나는Color Picker대화상자안에서 원하
는 색상을 골라라．

戚

圍團
口〔：3

3. R, G, B 텍스트상자안에 나타나는숫자를작성
한다. 여기의 숫자들은 색상의 R, G, B 성분을
나타낸다（그림 D.2).

cn1.r Pirk

. 시

L 口 h
1 1
흽 *
■ ,

c M , k
■ 1

回匡
回 쁘
凹匣
回
m匡
而回

@ ㅇ

. *
* d

그림 D.2 필요한색상을 선택한후, 보이는 값을R, G,B 텍스트
상자에 입력한다. 0/ 색장, teal blue는R 48 (l6i법30), (n43
α6잔법 8F), B i58 (16진빕 9E)을 갖는다. 따라서 이색상몌상응
하는16진법표가는#308F9E가 될 것아다．

ㅁ
lPi. ker "'윗 $'.'1tthe$ \ C0rto

B-

＝=

R。

252

0 O O

■p201에 배경색을 정하는 설명이 나와 있고，
p217과 p218에는 텍스트 색을 정하는 방법이
나와 있다．

% %

'/ nP

*

5. #rrggbb형태의 16진법의 수를연구해 보자．
rr은 red 성분의 16진법 등가값이고, gg는
green 성분의 16진법 등가값이다. bb는 blue
성분의 16진법 등가값이다.

ㅁ

回匿露팜

回

4. 3번에서 나온숫자에 대한16진법 등가값을
찾기 위해서 다음 페이지에 있는 테이블을 사용
하라．

143
’뜨

1. 포토샵꼐서 도구상자안에 있는칼라상자중에
하나를 클릭한다（그림 DM.

-

X
● ＇두m* ＝·＝且ㅌ 。Um널· ，。百닐。 m
＝ 乞＝ =

색1121 RGB 성분 찾기：

)

-

웹 사이트에서 독자가 원하는 색상의 red, green,
blue성분을 나타내기 위해서 독자들은 포토샵을
이용할수 있다. 다음에 이러한 성분들의 16진법의
등가값을 나타내는 p253의 표를 참조하면 된다．

＼匹耳

16진법에서 색상의 RGB 성분 발견
하기

\,

D.3 색상을 선택하고
卜 그림
그 RGB 성분을 선택하가
위하Picker Palette를
사우할 수도 있다．

===== PAGE 240 =====
239 =====
Color in Hex

16진법 표기 코드
#

^
J
4
`
U
6
m
/
8

4
<
J
,
1
口
<
J
,
<7
＇·
<
J

洲昑孤兄父m犯 郊

80
81
82
83
84
85
86
87
88
89
8A
8B
8C
8D
8E
8F
90
9l
92
93
94
95
96
97
98
99
9A
9B
9C
9D
9E
9F

#
160
161
l62
t63
164
165
156
167
l68
169
170
]7 l
172
173
174
175
176
177
178
179
180
181
l82
183
184
185
186
187
l88
l89
190
l9l

Hex.

#

Hex.

#

Hex.

AO
Al
A2
A3
A4
A5
A6
A7
AS
A9
AA
AB
AC
AD
AE
AF
B0
Bl
B2
B3
B4
B5
136
B7
B8
B9
BA
BB
BC
BD
BE
BF

-9 그 ( 0
193 C l
194 C2
l95 C3
196 C4
197 C5
I98 C6
199 C7
200 C8
201 C9
202 CA
203 CB
204 CC
205 CD
206 CE
2o7 CF
208 DO
209 Dl
210
211
기2
213
214
2l5
216
217
218
219
220 DC
221 DD
222 DE
223 DF

224
225
226
227
228
229
230
231
232
233
234
235
236
237
238
239
240
24l
242
243
244
245
246
247
248
249
250
25 l
252
253
254
255

E0
El
E2
E3
E4
E5
E6
E7
E8

16진법 시스템
'일반적인" 숫자들은기본10진법을사용한다. 다시
를
말해 10개의 기호（우리는 이것을 숫자라고 한다）
가지고 있다：0, 1, 2, 3, 4, 5, 6, 7, 8, 9. 9보다큰
수를 나타내기 위해서는, 처음 숫자가 얼마나 많은
숫자1을 지정하고, 두번째 숫자가 얼나나많은숫자
10을 지정하는지를 결정하는 방식으로 조합을 만들
어 나간다．

f 등이 있다. f (10진법에 기초하면 이 수는 15가
된다）
보다 큰 수를 표현하기 위해서는 우리는 다시
기호들의 조합을 이용해야 한다. 이번에는 첫번째
숫자가 일의 갯수가 몇인지를 나타내고, 두번째
숫자에서는 몇 개의 16이 있는지를 알려준다. 따라
서 10은 16을 하나 가지고 있고, 일의 자리수는 없고
단순히 16이다（십진법으로 보았을 경우）
.

16진법에서는 16을 기초로 한다. 따라서 16개의
기호가 있다. 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e,

색상에 관해서 16진법을 사용함하여 p249-250의
테이블에서 보여진 특수 기호를 나타낼 수 있다．

예群의소스 코드는 www.cookwooci.com에 있습나다．

253

긍X且m＝ 클。 m
二
． ？。百＝ 才

八
／느 ^
J
<
J
，
口

128
129
130
131
I32
l33
134
135
136
137
l38
I39
140
141
142
143
144
145
146
147
148
149
150
151
152
153
154
I55
156
l57
158
159

Hex.

m m 먀이 恥 mm m ㅄ m

l
<
U

羽xm貂汪犯引꾜"겨拓拓刃貂羽ㄳ犯兀D犯叩

7!
72
73
74
75
76
77
78
79
7A
7B
7C
7D
7E
7F

4

태ㅄ朗吼恥 跳탸mRm円타"恥m珊"m印m 沁邱印

9

胛%"떼m阻蝴嶼啼啼m때 朋m m

八
乙

112
n3
l 14
115
l t6
117
l l8
l l9
l20
l 2l
122
l23
124
125
126
127

Hex.

的m旬CM的妬旬眺0砧明配⑩ 能卵兀

Hex.

的ㅖ仁心섞的妬幻明的執妃托m妬姃m

4

"栢的旬ㅃ的兀기刀刀科乃兀 刃招袗帥잎舵" 鱗的 恥肌韶"卯이兜"익 站

Hex.

加기끄 好가乃妬刃괘四
%

l

0A
0B
0C
0D
0E
0F
10
11
12
13
14
15
l6
17
18
19
1A
lB
1C
l1)
1E
IF

4

꾜"弘弱妬胛羽軫的m舵 好M好妬心硼 的鉛 引兜貂弘弱弱釘貂羽印 이旬 貂

0

10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31

Hex

m이m떠여仍%m硼的

#

===== PAGE 241 =====
240 =====
INDEX

찾아보기

出
小

難

이 책의 인덱스를 만드는 작업은 꽤 신경쓰이는 작업
이었다. 왜냐하면 이 책의 모든 부분은 XML에 관련
되었던 부분이었지만xML, mDs, XML 스키마，
XSLT, CSS, 그리고 XLink와XPointer 등의 6개
토픽으로 나누어져 있다. 여기서는 각각의 토픽이
등장할 때마다 독자들이 쉽게 구별할 수 있도록 필요
한문맥을삽입하였다．

늙
＝
＝
二

=
=
=
＝
드
=
=

걜붚誓三넌냘＝ 큭享j＝ 푸管多聲嵋組團出m咐mm갑mm

255

＝
一

모두 인정하는 바이지만 기술 서적에서는 인덱스가
가장중요한부분이라고 생각한다. 누락된 부분을
발견하면 연락하기 바란다 (xml@cookwood.com).
여러분의 의견은 장차 발간될 책이나 새 버전에서
참조될 것이다. 독자들은 이 책의 웹 사이트에서
(p18 참조）인덱스를 볼 수 있을 것이다．

三三＝ 를 ￡ 三
글
： 珊二石耳 !

XML 스키마, XSLT, XLink와XPointer, 1711〕의
성분과 css 스타일 시트 등 안에서 정의된 모든
요소들과 속성 중 일부는 쉬운 열람을 위해서 알파벳
순서로 정렬되어 있다. 주제어 밑에 있는 요소들이
알파벳 순서로 되기 위해 여기서는 접두어 (xs]
xsd.', xlink:) 등은 생략했다. 디폴트 이름공간을
선언한 다음에 각 타입의 문서 안에서는 접두어들을
생략할 수 있다 (p128 참；조）
는 것을 이 책에서 들어
보았을거라 믿고, 독자 여러분들이 이 시스템 때문에
혼동하는 일이 없기를 바란다．

===== PAGE 242 =====
241 =====
Index
symbols
#（우물 정자）
cSS 셀렉터 안에서 181
XPointer 안에서 233
#PCDATA 44
DTD 안에서 선택권 47
시퀀스46
%（퍼센트）
,DID（매개 개체）
의 숏컷 안에서 60
& (ampersand) 31
텍스트（개체）
를 위한 숏컷 57
( )（괄호）
DTD 안에서 42
XML 스키마 안의 패턴 안에서 85
*（별표）
cSS 셀렉터 안에서 180
urn 안에서
선택권 정의하기 47
하나 이상의 유닛을 위한 48
xM. 스키마 안의 패턴 안에서 84
XSLT 안에서 156, 157, 160, 168
+（덧셈 기호）
cSS 셀렉터 안에서 180
un〕
안에서 48
XML 스키마 안의 패턴 안에서 84
XSLT 표현의 부가 사항 168
,（쉼표）
cSS 셀렉터 안에서 180
mㄷ）안에서 시퀀스를 정의하기 위한 46
-（하이픈）XSLT 표현 안에서 뺄셈 168
.（마침표）
xML 스키마 안의 패턴 안에서 84
XSLT에서 커런트 노드 142, 155
..（두 개의 마침표）
XSLT 안에서 부모 산택하기 157
/（슬래시）
DTD43
XSLT안에서 139, 156, 157
//（두 개의 슬래시）
XSLT 안에서 158
16진법 251-253
64bit 부동 소수점 80
:（콜론）
cSS 셀렉터 안에서 180
이름공간 113
<（부등호）
XPointer 안에서 233
속성값 안에서 28
작성법 31
0--（주석의 시작）30
그리고 내부 스타일 시트 187
<?（연산 명령의 시작）24

256

>（부등호）
cSS 셀렉터 안에서 180
작성법 31
?（의문 부호）
珝
［D 안에서 48
XML 스키마 안의 패턴 안에서 84
@XSLT 안에서 속정들 선택하기 160
ㅁ（사각 괄호）
cSS 셀렉터 안에서 180
DTD 36
XML 스키마 안의 패턴 안에서 84
XSLT 표현 안에서 161
.（굽은 괄호）
css 안에서 182, 183
끄dL 스키마 안의 패턴 안에서 85
-（수직 기호）
I工
［l〕안에서
속성의 선택권 정의하기 50
요소의 선택권 정의하기 47
XML 스키마 안의 패턴 안에서 85
' (apostrophe), 작성 31
"（인용부호）
XSLT 안에서의 테스트 표현들 164
간접 인용 부호 vs 직접 인용 부호 28
개체 31
속정들22, 23. 28
A
ASP 17
Adobe 포토샵에서 RGB 성분의 색상을 찾기 252

C
case (upper/lower)
cSS를 가지고 조절하기 222
xll』
안에서 23
XSLT를 가지고 조절하기 173
CDATA
urn의 속정 정의란에서 50
섹션
XHTML 241
xML 안에서 32
내부 (155 스타일 시트 187
〕8
color 특성 200, 217
display특성 200, 217
float 특성 198
foreground 색상 200
HT〕
꽈 XML 비교 178
left 특성 192, 193
right 특성 192, 193
Text Only format 183
text-align 특성 220

===== PAGE 243 =====
242 =====
Index
text-decoration -' 221
text-indent 특- 219
text-transform 특정 222
top 특정 192, 193
vertical align 특성 203
XLink와 XPointer 178
z-index 특성 202
글자 (kerning) 219
글자 공간 219
글자 공간 특성 219
기본 179
넓이 특성 194
넘침 204
높이 특정 194
들여쓰기 219
레벨 1과 2 178
레이아웃 189-208
리스트 특정 206
마진 특성 197
모든 폰트 값 조절하기 216
배경 201, 218
배경 특성 201, 218
보더 특정 195
볼드 형태 213
부모 요소 189
블록단계 vs 직렬형 189
색상217
설명 14
스타일 기본 179
스타일이 어디에 적용될지 정하기 180-181
요소숨기기
）鋼L 파서로부터 187
방문자로부터 191
요소의 높이와 넓이 194
이탤릭체 212
이탤릭체 제거하기 212
자 요소 189
작은 대문자 폰트 222
정렬하기
텍스트 220
가로로 203
줄 높이 특성 215
지엽적 188
지원하는 브라우저 178
클리어 특성 199
클리핑 요소 205
텍스트 감싸기 198
텍스트 小사기를 멈추기 199
텍스트 밑줄 긋기 221
텍스트 줄을 그어 지우기 221
텍스트 포맷하기 209-222

예젱의소스 코드는 www.cookwoo加om에 있습나다．

트래킹 219
특성 189-222
파일 확장자 182
패딩 196
패딩 특성 196
페이지 브레이크 208
포지셔닝 요소
3차원9_ 202
가로로 203
상대적으로 192
절대적으로 193
폰트 216
폰트 weight 특성 213
폰트 가족 특성 210
폰트 변수 특정 222
폰트 사이즈 특성 213
폰트 스타일 특성 212
폰트 첨가하기 211
호출 HTML에서 186
흐름과 함께 요소 오프셋하기 192
088 셀렉터 181
088 안에서
border특성 192, 193
display 특성 190
float 특정 198
font-family 특성 210
font-size 특정 214
font-style 특성 212
font-variant -' 222
font-weight 특성 213
height 특성 194
letter-spacing특성 219
padding 특성 196
position 특성
상대적인 포지셔닝 192
절대적인 포지셔닝 193
right특성 192, 193
text-allign 특성 220
text-decoration 특성 221
text-indent 특성 219
text-transform 특성 222
top 특성 192. 193
vertical-align 특성 203
마진 특성 197
배경 특성 201, 218
선언, 정의 179
줄높이 215, 216
css로 설정된 높이 194
css를가지고
볼드체로 포맷하기 213
배경 설정하기 201, 218

257

===== PAGE 244 =====
243 =====
Index
이댈릭 포맷 212
조절하는 Kerning 219
텍스트 밑줄 긋기 211
포지셔닝 요소 192-193, 203

D
decimal, 포함하는 요소를 정의하기 80
DTD 35-65
HTML을 위한 242
XML 유효화하기 244
XI刪」스키마와 비교 69
개인적인 외부 선언하기 39
개체들과 개념들 55-65
내부 선언하기 36
대중의 외부 선언하기 40
샬명 14, 35
외부 Un〕작성하기 37
외부와 내부 합치기 39
이름공간119
이름붙이기 38
작성을 위한 숏컷 57
작성하기 35-40
정의하기 41-65
ENTITY와 ENTITIES 속성 64
IDREF 속성 53
text only 요소 44
간단한 속정 50
개체 외부 파일 안에서 58
고유한 값을 가진 속성 52
내부 일반 요소 56
선택권을 포함한 요소 47
속성 49-54
시퀀스를 가진 요소 46
외부 파일 안에서 텍스트를 향한 숏컷 58
요소 42-48
유닛 등장 횟수 48
텍스트를 향한 숏컷 56
하나의 자 요소를 포함한 요소 45
제한 44
포괄적으로 선언된 요소 71
안에서 !ATI'LIST 50
nil〕
Ufl〕
안에서 SYSTEM 39, 58, 60
Un〕
의 숏컷 60
순서 61

E
elelment 요소
elementFormDefault 속성 x入d山 안에서 스키마 124
Extensible Markup Language XML을 참조
Extensible Style Language XSL 참조 135
Extensible Stylesheet Language - Transformation XSLT
참조

258

H
HTh
header 정보 140
xIT1rll과 비교 239
XML 포맷하기 140
XSLT 생성하기 140
XSLT를 가지고 작성한 테이블 147
내부 (SS 스타일 시트 187
단순성 12
디폴트 포맷 177.178
외부 스타일 사용하기 186
제한 12
지엽적인 cSS 스타일 시트 188
파일 확장자 240
필요한 지식 16
HTML 안에서
hr 태그 199
hag 요소 151
style 속성 188
style 요소 187
XSLT로 작성된 header 정보 140
XSLT를 가지고 생성된 테이블 147
링크 요소 186
테이블요소147

ID 속정 52
IDREF 속성 53
if 요소, XMLT 안에서 148
Instant SAXON 246
ISO639 언어리스트 76
J
java 17
javascript 17
L
language 약자, 리스트 38
language코드, 포함하는요소 선언 76
M
mod 함수, XSLT 표현 168
N
NMTOKEN 속성 54
Notepad 21

P
畔rl
규칙적인 표현 언어 84-85
더 자세한 정보는 85
상주 이름공간 123

===== PAGE 245 =====
244 =====
Index
R
reccuring thy/date, 포함하는 요소 정의 79
RGB 색의 성분 252

S
SAX 17
SAXON 246
SinmpleText 21
standalone 속성 39
cSS를 가지고 텍스트 감싸는 것 중단하기 199
cSS를 가지고 포맷 줄 긋기 221
UPD 안에서 60
xML 선언 안에서 58
substring-after(）
와 substring-before
XSLT 안에서 함수 171
sumO 함수 XSLT 안에서 166

U
UltraEdit과 SAXON 246
Unicode 248
URL
이름공간 이름 114
포함하는 요소 선언하기 76
UTC, 샬명 79
UTF-8 혹은 UTF-16 encoding 24

x
XHTML 239-242
DTD 242
H〕
衲皿과 비교 239
IITM1로 서비스하기 240
XSLT 239
브라우저가 아는 방법 240
신택스241
작성 241
파일 확장자 240
XLink 225-236
XLink 안에서
actuate 속성 227
href속성 226
resource 229
role 속정 226
show 속성 227
simple 요소 227
title 속성 226
위치 지정자 229

炳의소스 코드는 www.cookwcod.com에 있습나다‘

=`mX

T
Techtext 21
text-only요소, 정의 44
Text Only 포맷과CSS 183
times 포함한요소 정의하기 78-79
to XML 문서 작성하기 21

XML
applications 13, 21
XHJMI로 서비스하기 240
XSLT를 가지고 변환하기 135-173, 246
overview 136-137
가치값 22
고유 개체 31
다른 문서으로부터 문서 생성하기 59
도 '243-246
루트 요소, 작성 25
리소스 243
링크 225
문서 작성 21
블록 단계 직렬형 요소 비교 190
빈 요소 29
서비스의 위험요소 239
선언 24
속성 22,28
신택스 21-32
실제 세계 15
요소 22
요소 중첩하기 27
웹 사이트 18
유효한 문서 36
유효화
스키마에 반해 73, 122, 129
이름공간 113-132
이미지 225
작성 21-32 243
작성 도구 21
작성의 규칙 23
주적 30
직접 페이지 서비스의 문제점 225
책의 예제 다운로드 16
캐릭터 인코딩 24
텍스트로서 요소 보여주기 32
편집기 73
포맷, 디폴트의 부족 177,178
XML SPY 73
XMT. 문서 저장 21
XML 문서 편집하기 21
XML 스키마 69-132
any江ype 타입 103
attribute 요소 108
attributeFormDefault 속성 124
attributeGroup 요소 111
base 속성 102, 105
boolean 타입 76
centuly 타입 79
date type 76, 78
decimal 타입 76, 80

259

===== PAGE 246 =====
245 =====
Index
documentation 요소 74
double 타입 80
element 요소 76,106
elementFormDefault 속정 124
enumeration 제한점 83
extension 요소 102, 103, 105
fixed 속성 91
form 속성 125
group 요소 98
import 요소 132
include 요소 131
integer 타입 76
length 제한점 88
list 요．
소 90
maxExclusive 제한점 86
max[nclusive 제한점 87
maxLength 제한점 88
maxOccurs 속성 101
minExclusive 제한점 87
minlnclusive 제한점 87
minLength 제한점 88
minOccurs 속성 101
mixed 속정 104
month 타입 79
negativeinteger 타입 80
nonNegativelnteger 타입 80
nonPositivelnteger 타입 80
positivelnteger 타입 80
precision 제한점 89
recurringDate 타입 79
recurringDay 타입 79
ref속정 108, 126-127
reguLar 표현 84-85
restriction 요소 102, 105
restriction 타입 81
scale 제한점 89
schema 요소 72,108
sequence 요소 95
simpleContent 요소 102
simpleType 타입 81, 82
time 타입 76,78
timetluration 타입 78
timelnstant 타입 78
type속정 106, 108, 126-127
un-reference 타입 76
use 속성 109,110
xm1ns 속성
디폴트 이름공간을 부가해서 115
이름공간의 접두어 선언하기 116
지정된 이름공간과 비교 127
xmins와 비교하기 127

260

year 타입 79
기호열 타입 76
디폴트 속성 91
디폴트 스키마 128
모든 요소 97
복잡한타입 요소 94, 102, 103, 104, 105, 107
선택권 요소 96
설명 14
이름공간 72
주석 요소 74
커런트 상태 69
패턴 제한점 84
XML스키마보기
noNamespaceSchemaLocation 속성 73
schemaLocation 속성 130, 131, 132
이름공간 73
타깃 이름공간과 함께 130
XML스키마안에서
anytype 타입 103
attributeFormflefault 속정 124
attributeGroup 요소 111
base속정 102, 105
century 타입 79
decimal 타입 76,80
extension요소 102, 103, 105
XML 스키마 안에서 76,106
XSLT 안에서 141
float 타입 80
form 속정 125
import 요소 132
language 타입 76
list 요소 90
maxExciusive 제한점 86
maxLength 제한점 88
maxOccurs 속성 101
산택권 96
정렬되지 않은 그룹 97
minExciusive 제한점 87
minlnclusive 제한점 87
minOccurs 속성 101
mixed 속성 104
month 타입 79
nonNegativeinteger 타입 80
nonPositivelnteger 타입 80
positivelnteger 타입 80
precision 제한점 89
reccuningDate 타입 79
reccuringDay 타입 79
ref속성 99, 100, 108, 126-127
restriction 요소 102, 105
scale facet 89

===== PAGE 247 =====
246 =====
Index

예群의소스 코드는 www.cookwood.com에 있습나다．

誼nple 요소 227
title 속성 226
刀山止225-236
설명 14
지원의 부족 225
타입 속성 226
확장된 요소 228
XML-RPC17
XML에 첨가되어진 이진법 파일 62-65
XML을 위한 resources 243
XML의 도구들 243-246
XMT의 버전, 선언 24
XPath 153-173
XPointer 233
설명 14
함수 163-173
XPath와XSLT 안에서 함수 163-173
XPointer 233-236
간단한 XPointer 234
걸어 다니는 XPointer 235
범위 236
설명 14
지원의 부족 225
XSL-F0 135
설명 14
현재 상황 135
xsl:sort 안에서 order 속성 150
XSLT 135-173
apply-templates 요소 145
커런트 노드 정하기 154
attribute 요소 141,151
batch 연산 노드 146
CDD 스타일 시트 호출하기 184
choose 요소 149
element 요소 141
for-each 요소 146
HTML 출력하기 140
HTML 테이블 147
if 요소 148
match 속성 139,144
otherwise 요소 149
select 속성 142. 145
sort 요소 150
template 요소 139,144
when 요소 149
XML 변환하기 246
XPath 153-173
XPath 함수 163-173
XSV XML Schema Validator 참조
노드 136
부모／형제 선택하기 157

=`mX

schemaLocation 속성
보기 130, 131, 132
선택권 96
정렬되지 않은 그룹 97
simpleContent 요소 102
time 타입 76,78
timeDuration 타입 78
timelnstant 타입 78
uri-reference 타입 76
use 속성 109, 110
value 속정 109, 110
year타입 , 79
고정된 속성 91
그룹 요소 98
기호열 타입 76
단순한 타입 75-91
xsd 접두어 77
가능한 값들의 세트 83
길이 88
날짜78-79
리스트 90
모든 리스트 77
미리 정의될 컨텐츠 91
범위, 정하기 86-87
복잡한 타입과의 비교 70
속성 77
숫자 80
열거된 값 83
요소 선언하기 76
익명 82
자릿수, 제한된 89
지엽적인 선언과 포괄적인 선언 비교 77
패턴 84-85
리스트 타입 90
목록 제한점 83
문서 요소 74
선택권요소96
스키마요소72, 128
정수 타입 80
주석 요소 74
지정 이름공간 속성 123
다른 문서로부터 온 성분 131
XML 스키마 유효성 처리기 73
XML 스키마 패턴 제한점 84
XML 신택스 21-32
XML 유효성 처리기（브라운 대학의 STG) 244
XML 파서 13
actuate 속' 227
href속정 226
role 속성 226
show 속성 227

261

===== PAGE 248 =====
247 =====
Index

X겸＝

부분 집합 산택하기 149
속성 선택하기 160
자식 선택하기 156
후손 선택하기 158
노드 안에 있는 기호알 대문자로 하기 173
노드값 라운딩하기 170
노드값을 소계하기 166
노드로부터 서브스트링 끌어오기 171-172
노드의 위치 테스트하기 165
노드의 컨텐츠 출력하기 142
루트 템플릿 139
마침표 142
복잡한 타입 93-112
vs 간단한 타입（과의 비교）70
다른 복잡한 타입에 기초한 105
빈 요소 103
선언 요소 106
선택권 96
시퀀스95
요소만을 94
익명 107
정렬되어 있지 않은 그룹 97
정의 93
텍스트 뿐인 요소 102
혼합된 컨텐츠 104
사칙연산 168
생성되는 속성 151
생성된 HTML 문서를 위한 스타일 시트 호출하기 186
설명 14
스타일 시트 시작하기 138
스타일 시트 요소 138
연산 명령 요소 184
연산자136, 246
연산하기 전에 노드 분류하기 150
요소의 값 142
xsl:attribute 151
이름공간 선언하기 138
조건부 선택권 149
조건적으로 노드 연산하기 148
커런트 노드 142
결정 154
설명 155
표현 153-173
두 값을 비교하기 164
텍스트 요소 141
템플릿규칙, 작성과적용144-145
패턴과 표현 153-173
포맷하기 위해 HTML 사용하기 140
표현 153-173
표현을 가지고 숫자 포맷하기 169
함수 XPath 함수 참조

262

XSLT 안에서
apply-templates 요소 145
floor () 함수 170
format-number 0 함수
last 0 함수 165
match 속성 139, 144
otherwise 요소 149
position () 함수 165
select 속성 142, 145
sort 요소 150
xs1;app1y-templates 145
substring 함수 171
표현 169
translate 0 함수 173
value-of 요소 142
xsl:attribute 151
기호열 값 142
스타일 시트 요소 138
커런트 노드
결정하기 154
무시하기 159
설명하기 155
템플릿
가장 적절하게 연산하기 145
고유의 139 145
루트 139
순서 139 144
자동적으로 호출되거나 안되거나 144
작성하고 적용하기 144 145
커런트 노드 결정하기 154
템플릿 요소 139,144
테스트 표현 안에서 or 164
테스트 표현 안에서 & 164
XSLT로 끌어낸 서브스트링 171. 172
XSLT를 가지고
기호열 대문자로 만들기 173
라운딩 숫자 170
출력한 오자들 140
XSLT를 위한 루트 템플릿 139
XSLT 안에서
ound 0 함수 170
processing-instruction 요소 184
XSLT에서 ceiling 0 함수 170

가
가능한 값의 세트, 포함하는 요소 정의하기 83
가치값
XML 안에서 22
XSLT 안에서 164와 비교
고유값을 포함하는 속성을 정의하기 52
간단한 링크의 역할 226
간단한 링크의 타이틀 226

===== PAGE 249 =====
248 =====
Index

나
내부 urn, 선언 36
내부 매개 변수 개체 61
내부 일반 개체 56
사용 57
노드
batch 연산 146
XSLT를 가지고 작성하기 141
값 비교하기 164
값을 소계하기 166
값의 사칙연산 168
기호열 대문자로 하기 173
선택하기
부모／형제 157
부분 집합161
속정 160
자식 156
후손 158

예제의소스 코．
드는 www.cookwocd.com에 있습나다；

세기 167
숫자포맷하기 169
연산전에 밝루하기 150
위치 165
정의 136
조건적으로 연산하기 148
커런트 노드
결정하기 154
무시하기 159
설명하기 155
컨텐츠 출력하기 142
노드 세트
값 비교하기 164
값을 소계하기 166
노드 세기 167
노드의 위치 165
노드 분류하기 150
복수의 노드일 때 142
조건부의 선택권 149
존재를 위한 테스트하기 164
진실일 때 148
노드트리, 정의 136
노드로부터 서브스트링 끌어내기 171-172

흽付븜

개체
고유의 31
글자 설명과 비교 56
내부의
사용법 57
작성법 56
다른 사람의 61
매개체 60
설명 55
외부의 58
속정 28
중첩된 56
해석되지 않은 컨텐츠를 위한 62-65
개체 설명 23
고유한 값, 포함하는 속성 정의하기 52
고정된 값
속성을 위한
urn 안에서 50
스키마와 함꼐 110
요소를 위한 스키마와 함께 91
공간 넣기
요소 주변에 (css를 가지고）196-197
텍스트의 (0ss를 가지고）219
규칙
XML 작성을 위한 23
요소 이름을 위한 26
규칙적인 표현 언어 84-85
글자 레퍼런스 이용 p248
기술적 지원 18
기호 247-250
사용248
테이블250

다
다른 문서로부터 문서 생성하기 59
다른 스키마로부터 성분 유입하기 132
단순한 타입을 위한 열거된 값들 83
디폴트 값
속정을 위한
I기
［D 안얘서 50
스키마와함께 110
요소를 위한, 스키마와 함꼐 91
디폴트 값으로서 스키마 중의 스키마 128
디폴트 이름공간 115

라
레이아웃
cs를 가지고 189-208
Hl丕4L을 가지고 XSLT와 함께 생성하기 140-141
left 특성 css안에서 192,193
length, 요소 컨텐츠 제한하기 88
XML 스키마 인에서 length 제한점 88
레퍼런스 포인트 229
루트 요소 23
작성 25
포괄적 선언 71
링크
링크세트 228
간단한 링크 작성하기 226
css 셀렉션 181
css와 함께 xM. 문서 안에서 178

263

===== PAGE 250 =====
249 =====
Index
XML 안에서 225
XPointer 범위 236
간단한 링크 작성하기 226
걸어 다니는XPointer와함꼐 235
설명 포인트 229
커넥션 정의하기 230
확장된 228
링크세트 228
사용 232
정의된 안갈 230

마

乂
●겯

마이크로 인터넷 익스플로러 5
cSS 지원 178
xML 15
XSLT를 위한 이름공간 선언 138
스크린 샷 16
스타일 시트없이 꼬dL 보여주기 185
마침 태그 23
빈 요소 안에서 29
접두어 117
매개 변수 개체 60
설명 61
모델 그룹 98
무명（익명）타입
단순한 형태 82
복잡한 형태 107
문서 변환 135-173
XSLT와XPath 참조
문서 타입 선언 36
미리 정의된 컨텐츠 110

바
부모 요소 189
비어있지 않은 요소 26
빈23, 29
cSS를 가지고 숨긴 191
XMl 안에서 22
비어있지 않은 26
스키마 안에서 103
접두어가 없는 117
중첩되어진 27
빈 요소 23, 29
스키마 안에서 103

사
상대적인 포지셔닝 192
색상들
16개의 정의된 이름 251
16진법 등가값 252
CSS 안에서 설정 200, 217
RGB 성분 252

264

서술부 이름공간에 의한
선언 116
성분의 지정된 이름공간 127
지정된 이름공간 117
선택권
XML 스키마 안에서 등장 횟수 101
XSLT 안에서 조건적인 149
요소 컨텐츠 결정
urn 안에서 47
xM. 스키마 안에서 96
셀렉터
적성 180-181
정의 179
속성
〕yII) 안에서 정의하기 49-54
ENTIY와 ENTITIES 타입 64
ID 속성을 설명하는 53
II) 타입 52
IDREF와 IDREFS 타입 53
고유값과 함께 있는 52
단순한 50
단순한 타입 77
디폴트 값과 고정값 50
미리 정의된 컨텐츠 110
선언하기 108
속성 그룹 111,112
유효한 xML 이름과 함께 있는 54
의무적인 109
xML 안에서 속성 22,28
XSLT를 가지고 속성 생성하기 151
XSLT 안에서 노드의 속성 정하기 160
스키마 안에서 정의하기
외부 개체 28
유효한 xM.이름에 대한 속정 54
이름공간 118
속성 요소
xML 스키마 안에서 108
XSLT 안에서 141, 151
속성 정의 안에서 #IMPLIED 50
숫자
XSLT를 가지고 라운딩하기 170
XSLT를 가지고 포맷하기 169
스키마에서 포항하는 요소 정의 80
슈퍼라벨 113
스키마69-132
以
［〕
〕와 비교 69
xML 유효화 하기 73
간단한타입 75-91
xsd 접두사 77
가능한 값들의 세트 83
길이 88

===== PAGE 251 =====
250 =====
Index
리스트 90
모든 리스트 77
미리 정의된 컨텐츠 91
범위, 정하기 86-87
복잡한 타입과 비교 70
속성 77
속성을 위한 고유의 108
숫자 80
열거된 값 83
요소 선언 76
익명의 82
자릿수, 제한89
주문형 76
지엽적과 포괄적 선언 비교 77
패턴 84-85
같은 이름공간을 가지고 다른 문서로부터 성분 유입하기 131
그룹, 명명된98
설명하는 99
다른 이름공간으로부터 성분 유입하기 132
등장 횟수 101
디폴트 값으로서의 스키마 중의 스키마 128
명명된 그룹 98
설명 99
문맥, 중요성의 71
문서 유효화 하기 122
복수의 파일 131
복잡한 타입 93-112
간단한 타입과 비교 70
다른 복잡한 타입으로부터 105
명명된그룹98, 99
선언 요소 106
선택권 96
시퀀스 95
정렬되어 있지 않은 그룹 97
정의 93
텍스트뿐인 요소 102
혼합된 컨텐츠 요소 104
복잡한 타입의 요소 선언하기 106
빈 요소 103
선택권 96
설명 14, 69
설명 71
명명된 그룹 99
속정 그룹 112
요．
소 100
이름공간을 가지고 성분 설명 126- 127
속성 77, 109, 110
선언108
속성 그룹 111, 112
속성들의 그룹 111,112
시작 72
위치 73, 130

예제의소즈 코드는 www.cookwood. corn에 있습나다

유효한 문서 작성 121
이름공간 113- 132
XML 스키마를 위한 72
성분 설명 126
익명 타입
단순한 82
복잡한 107
정렬되어 있지 않은 그룹 97
주석 달기 74
지엽적으로 산언된 요소 106
개별의 것을 이름공간에 넣기 125
모두를 이름공간에 넣기 124
설명하기 100
포괄적과 비교 71
텍스트뿐인 요소 102
파일 확장자 72
포괄적으로 선언된 100, 106
지엽적으로와 비교 71
혼합된 컨텐츠 요소 104
스키마 안에서 등장 횟수 조절하기 101
스키마 안에서 명명된 그룹 98
등장 횟수 조절하기 101
설명하기 99

아
연산 명령 24
연산 전에 노드 분류하기 150
온라인 도움 18
외부 일반 개체 58
요구되어지는
속성
聊
［ㄲ 안에서 50
스키마를 가지고 109
요소들
DTE를가지고45, 46. 48
스키마를 가지고 101
요소
DTD 안에서 정의하기 42-48
등장 횟수 48
선택권 47
시퀀스 46
텍스트 뿐인 44
하나의 자식 요소를 가진 45
디폴트 이름 공간 115
스키마 안에서 정의하기 75-112
고유한 이름을 가진 71
등장 횟수를 조절하는 101
미리 정의된 컨텐츠 91
복잡한 타입 선언하기 106
비어있는 103
선택권 96
설명 71. 100

265

===== PAGE 252 =====
251 =====
Index

X0큅＝

시퀀스 95
요소만을포함한94
익명의 복잡한타인 107
지엽적인 선언과표괄적인 선언 비교 118
텍스트 뿐인 102
혼합된 컨텐츠 91
이름 부여하기 117
요소 오버랩핑하기 193
요소 컨텐츠를 위해 정한 최소 길이 88
요소 컨텐츠를 위해 정해진 범위 86-87
이름 공간과 함께 126
요소들의 마진 197
유효한문서
스키마와함께 121
정의 36
이름
DTE를 위한 38
유효한, 요소를위한26, 77
이름공간을 위한 114
이름공간 113-132
DTD 119
NDATA, 1711) 안에서 62
targetNamespace 속성과xl교끄s 속정 비교 127
XIjnk 선언하기 226
XMl. 스키마 보기 73
XML 스키마 산언하기 72
XML스키마 안에서 negativeinteger 타입 80
XSLT 산언하기 138
개개의 지엽적으로 선언된 요소 첨가하기 125
개별 요소를 위한 116
넷스케이프
css 지원 178
XML 15
스타일 시트 없이 XML 표시하기 185
디폴트 115
모든 지엽적으로 샨언된 요소 첨가하기 124
모여드는 123
정의 122
성분 설명하기 126
속성 118
스키마118
스키마 유효 문서 121
스키마 중의 스키마 72
스키마 중의 스키마 디폴트 값 128
연관되지 않은 요소 123
요소가 연결되지 못하도록 125
유전 115
유효화 문서 129
이름, 디자인된 114
이름공간을 가지고 스키마 성분에게 자격을 주는
접두어 127

266

중첩
개체 56
선택권 96
시퀀스 96
요소들 23, 27
지엽적으로 산언된 요소와 118
타깃 123
포괄적으로 선언된 요소 123
이미지
css를 가지고
가료 포지셔닝하기 203
텍스트 감싸기 198
텍스트 감싸기를 멈추기 199
XML 안에서
DfD를 가지고 첨가하기 62-65
HTML을 통해서 XSLT 생성하기 151
css를 가지고 178
XSLT를 가지고 태그 생성하기 151
리스트 기호 206
배경 css를 가지고 201
사이즈 조절하기 194
일반 개체
사용 57
설명 55
외부 58
작성 56

자
자 요소 정의 27
작은 대문자, css를 가지고 설정 222
정렬되지 않은 그룹 97
등장 횟수 101
정렬하기
css를 가지고 요소를 가로로 정렬하기 203
스타일 시트를 가지고 텍스트 정렬하기 220
제한점
enumeration 83
length 88
maxExciusive 86
maxlnclusive 86
minExciusive 87
minlnclusive 87
minLength 88
precision 89
간단한 타입 제한하기 81
속성 108
스케일 89
패턴 84
주문형 타입
이끌어내기 81
익명의 82

===== PAGE 253 =====
252 =====
Index
지엽적으로선언된
개별의 것을 이름공간에 넣기 125
모든 것을 이름공간에 넣기 124
샬명 100
이름공간113, 118, 122
정의 71
지원18
질문 답변 보드 18

차
책의 사용법 16
책의 예제 다운로드 받기 18
책의 예제 다운로드 파일 18
최대 길이, 요소 컨텐츠를 위해 정하기 88

카
캐릭터 설명 vs 개체 설명 56
커런트 노드 결정하기 154
클리어 속성 css 안에서 199
클립핑 요소 205

明］
의소스 코드는 www.cookwood.corn에 있습나다．

파
파일확장자
c88를 위한 182
DTC를 위한 37
HTML을 위한 240
XHTML을 위한 240
XML 문서를 위한 21
스키마를 위한 72
패턴
XML 스키마 안에서 포함하는 요소 정의 84-84
XPath 안에서 153-173
페이지 브레이크 208
편집을 위한 XML 문서 시작하기 21
포괄적으로 선언 100
이름공간113, 122, 123
자동적으로 설명되기 71
정의 71
포맷
case 222
kerning 219
들여쓰기 219
디폴트 HTML 안에서 177, 178
밑줄 긋기 221
배경색상218
볼드 213
사이즈 214
이탤릭 212
정렬 220
줄 높이 215
트래킹 219
폰트 210 211
포함하는 요소 선언의 boolean 76
포함하는 요소를 정의하는
부동 소수점 80
정수 80
폰트
css 안에서 설정하기 210, 216
css에서 설정된 줄높이 215, 216
css에 첨가된 211
변수 222
작은대문자222
프린트하기, 페이지 브레이크 조정하기 208

＝뚱X

타
타깃 이름 공간 123
상응하는 스키마의 위치 130
타입속성
xML스키마안에서 106, 108. 126-127
XSLT 안에서 226
테스트표현 148, 149, 163-173
텍스트 32
case
css와 함께 222
XSLT와 함께 173
css를 가지고 윗줄 긋기 221
가운데 정렬 220
감싸기 198-199
밑줄 긋기 css를 가지고 221
색상 c83를 가지고 217
숏컷 56
사용 57
스타일 시트로 정렬하기 220
요소들 보여 주기 32
정당화 하기 220
포함하는 요소 정의하기 102
텍스트 정당화 하기 220
텍스트의 사이즈, 스타일 시트를 가지고 조절하기 214
텍스트의 숏컷 56
사용 57
외부 화일 안에서 58
특성 정의 179
특수 기호 247
강조된 글자들（테이블）249
개체 56
고유한 개체 31

사용 248
테이블250
특정（이름공간과관련된）124, 125

하
해석되지 않은 컨텐츠 62-65

267

===== PAGE 254 =====
253 =====
Colophon

예제에서 사용된 사진들은Adobe Image Library
(Animal Life）
를 참조하였다．

"WF* L巧｀騙1n『｀dY'dd11
＇츈rUnd

二
*

1芒

ㅁ日

,睾 料. 孚,

쇠

=

`
一∼…

／雙

∼－

」『
『呻

毓十久知，
.m》

-

＼∼一」一，
4』
，1．
·．…∼…∼·→∼，
1∼一 ∼．
，∼

,

;',
[

(11111

1

;邕

,\\ pl. n. t
1

'

I

u

I

-

-

SAv1 0UR SEAS

ww

I

｝콥- -푀

＝。i。 ＝
닐

호랑이에 관한 설명

」：;;＝各．

이 책의 예제들은 실제 데이터를 기초로 하고 있고
이 데이터들은 야생 동물 펀드 웹 사이트에서 참조하
였다（물론 그들의 허가가 있었다）
: h曲）
：〃￦ㅠW.
worldwildfife.org. 또한 독자들은 Peter
Matthiessen글, Maurice Hornocker사진의
"Tigers in snow'란 책을 읽어 보기 바란다．

, FNflSI굻…

;

이 책의 모든 화면 레이 아웃은 QuarkXPress 3.3을
사용하였다. Paint Shop Pro（윈도우）
와Flash-It
（매킨토시）
을 이용해서 화면 캡쳐를 하였고, Adobe
Photoshop 5.5를 가지고 수정했다. 또 Adobe
ifiustrator 6.0을 이용하여 줄 긋기를 만들었고
이 책의 폰트는 Courier와 Futura, 윤명조체를
사용하였다．

=

！跡；

C이ophon

;.,..一.,,....,,,",.

쑹‘弘愧’之섧 I

'一！）『'4.

곁尹견'므’r寸""쬔 祇

9uIoPwflU
pidy
Chd,
.n‘鬱聾MI
難t (g4tt%q$nI.
戮 by

4- `i`'

` , 』뇨t 긱. - 뇨

=z림 乂굿 야섕 동물 괸드는 멸종 위刀의호랑아룰 ㅈ／카는 환겋 단鄒
중의 하나이다. 더자세한사항은http://www.worldwildlife.org
에서볼 수 있다．

호랑이의 절박한 멸종 위기는 우리를 슬프게 한다．
이것은 우리가 얼마나 환경을 잘못 다루고 있는지를
보여준다. 이 모든 것은 환경 주의자 뿐만 아니라
우리 모두의 책임이라할 수 있다. 이 책의 내용과는
상관없이 개인적인 바램은 독자들이 야생 동물 펀드
와 Hornocker Wildlife Institute (http://www.
uldaho.edu/rsrch/bwiA와 같이 지구의 환경과
사라져 가는 여러 종류의 동물을 보호하는 조직을
지원하기 바란다．
세계에는 단지 5000마리의 호랑이가 남아 있을 뿐
이다．

268

]

그랗 z2 Hornocker Wildlife Institute에 대한자저7한 정보는
http://www.uidaho.edu/rsrch/hwi에서볼 수 았다．

