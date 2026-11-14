---
source_url: "/run/media/yutae/Data/알고리즘 기초.pdf"
ingested: 2026-11-15
sha256: 8308c5c8328a82cfaed62dd9ee8849e5ad14e55329cd17d7b21e3e45d5f87699
type: raw-source
method: ocr
---

# 알고리즘 기초 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/알고리즘 기초.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** tesseract 5.5.3 (kor+eng, 300dpi)로 OCR
> **쪽수:** 636쪽 | **추출 텍스트:** 1291 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/algorithms-basic.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** 알고리즘 기초
- **Pages (PDF):** 636
- **Source:** 알고리즘 기초.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 636 pages)


===== PAGE 1 =====
FIFTH
EDITION

FOUNDATIONS OF


===== PAGE 2 =====
NEAPOLITAN

홍릉과희출판사


===== PAGE 3 =====
Foundations of

ALGORITHMS. Fifth Edition

ORIGINAL ENGLISH LANGUAGE EDITION PUBLISHED BY
Jones and Bartlett Publishers, Inc.
5 Wall Street
Burlington, MA 01803

Copyright © 2015 by Jones and Bartlett Learning, LLC, an Ascend Learning Company

All rights reserved. No part of the material protected by this copyright may be reproduced
or utilized in any form, electronic or mechanical, including photocopying, recording, or by
any information storage and retrieval system, without written permission from the copyright

owner.
Translated Edition ISBN : 979-11-5600-503-2

Translated by HongReung Publishing Co.

Printed in Korea

이 도서는 홍릉과학출판사가 10065 and Bartlett Publishers, Inc.2} 정식 계약에 의하여 번역한
책으로서 어느 BEE 인쇄, 복제, 제본 등 기타 판권 소유에 위배되는 제반행위를 할 수 없습니다.


===== PAGE 4 =====
저자 머리말

“Foundations of Algorithms’ 의 5판은 4판의 장점은 그대로 두었다. 4판과 마찬가지로 실제
코드가 아닌 의사코드로 알고리즘을 기술한다. 복잡한 알고리즘을 프로그래밍언어로 표현
하면 AAS 흐려놓아 이해하는데 방해만 될 뿐이다. 사람에 따라 친숙한 프로그래밍언어
가 GSEs, 누구냐 자신의 알그 있는 프로그래밍 얻어와는 상관없이 의시코드를 ofa
수 있어야 한다. 따라서 특정 언어에만 종속된 부분은 의사코드에서 배제한다. 대부분으
학생들에게 친숙한 와 완전히 다른 부분은 교재의 앞부분에서 언급한다. 이 책은 알고리
즘의 설계, 알고리즘의 복잡도 분석, 계산복잡도 (문제의 분석)에 대하여 다룬다. 단, 정확
도 분석과 같은 다른 종류의 분석은 다루지 않는다. 이 책을 집필한 동기는 알고리즘의 복
잡도 BAS 엄밀하게 설명하면서 동북일리노이대학과 같은 4년제 대학에서 컴퓨터과학을
전공하는 학생들이 쉽게 접근할 수 있는 WAS 저자가 찾지 못했기 때문이다. 동북일리노
이대학의 학생 대부분이 미적분학을 배우지 않아서, 추상 수학과 수학용어에 익숙하지 않
았다. 기존 교재에서 사용하는 용어들은 수학을 잘하는 학생들에게는 별로 문제가 없지만,
우리 학생들에게는 좀 어렵다는 사실을 알게 되었다.
이 교재를 학생들이 좀 더 쉽게 느끼게 하기 위해서 다음 사항들을 고려하였다.

* 학생의 수학에 대한 기초 AALS Gea} 이산구조뿐이라고 가정한다.

* 수학적 개넘을 되도록 말로 설명한다,

© 정형 증명은 좀 더 자세히 기술한다.

* 예제를 많이 제공한다.

이 교재는 알고리즘 AAS} BAS 다루는 학부 고학년 또는 대학원 강의 수준에 맞추어
한 학기용으로 기획하였다. 이 교재는 학생들에게 알고리즘 작성 및 분석 방법을 이해하기
위한 기초 지식을 제공하고, 알고리즘 설계 표준 전략을 사용하여 알고리즘을 작성하는데
필요한 기술을 알려주는데 목적을 두고 있다. 전에는 분할정복, 동적계획, 탐욕알고리즘,
되추적, 분기한정법에 국한되어 있었다. 그런데 최근 들어 컴퓨터과학자에게 유전 알고리
즘의 사용이 점차 중요하게 부각되고 있다. 그러나 인공지능 관련된 강좌를 수강하는 학생

들만 유전 알고리즘을 접할 수 있을 뿐이었다. 인공지능 분야에만 유전 알코리즘이 쓰이는



===== PAGE 5 =====
iv

건 아니므로, 유용한 최신 기술에 대한 기본적인 레파토리를 제공해주기 위하여 유전 알고
리즘과 유전 프로그래밍을 다루는 BS 하나 추가하게 되었다.

복잡도 BAS 대수학과 이산구조에 대한 기초지식만 있으면 거의 대부분 이해 가능하다

할        . 즉, 미적분학의 개념은 거의 사용할 필요가 없다. 미적분학을 공부해본 적이

없는 학생은 수학 용어만 나오면 겁부터 먹는다. 따라서 “Ss O'S} 같은 수학 개념을 소개하
면서 가능한 수학 용어 사용을 자제하고 자연어로 설명하려고 노력하였다. 사실 설명을 명

료하게 하기 위해서 어느 정도의 수학 용어가 필요하지만, 너무 많이 사용하면 학생들에게

줄 수 있어서, 적절한 SES 지키는 일이 결코 쉬운 일은 아니다. 그동안 학생들의

반응을 보도 판단하면, 어느 한쪽으로 치우치지 않고 적절한 선을 잘 지켰다고 자부한다.

수학적인 엄밀함을 아주 포기한다는 말은 아니다. 이 책에서 공부하는 모든 결과에 대하
정             }다. 그러나 기존의 전공 도서에 비해서 더 친절하고 자세히 증명 A
많이 보여주려고 노력했다. 실례를 보여주면 학생들이 이론적인 개
념을 더 쉽게 파악할 수 있다. 따라서 수학 기초지식이 약간 부족한 학생들도 충분한 노력
을 쏟아 부을 각오가 되어 있으면, 수학적 논조를 따라갈 수 있고 그 주제에 대하여 더 깊이
이해할 수 있을 것이다. 더구나, (차수를 결정하는데 사용하는 극한이라든지, 일부 정리의
증명에 사용하는 것 같이) 미적분학의 지식이 필요한 경우도 있다. 그러나 이 교재의 나머
지 내용을 이해하기 위해서 학생들이 그 지식에 정통할 필요는 없다. 미적분학의 지식을
요하는 내용은 목차와 본문에 @ Jes 표시해 놓았다. 추가적인 수학기초 지식은
필요하지 않지만, 교재의 내용 중에서 본질적으로 난해한 부분은 로 표시해 놓았다.

앞에서 언급했듯이, 학생들은 대수학과 유한수학의 기초  ah: 있으면 충분히 이 책의 내
SS 소화할 수 있다. 실제 필요한 수학은 부록 에서 복습한다. 컴퓨터학 기초지식으로는
데이터구조 강의를 수강했다고 가정한다. 따라서 자료구조   띠에 a  전형적으로 나오는 내용
은 여기서 다루지 않는다.

전체적으로 응용분야별보다는 문제를 해결하는데 사용한 기술별로 이 교재를 구성하였다.
이렇게 구성하면 알고리즘 설계와 분석 분야를 더 일관성 있게 볼 수 있을 것이다. 아울러,
새로운 문제를 해결하는 방법들을 탐구할 수 있는 기술의 레퍼토리를 학생들이 더 쉽게 습
득할 수 있다. 책의 내용을 장 별로 요약해보면 다음과 같다.

© 142 알고리즘의 설계와 분석에 대하여 소개한다. 차수의 개념에 대하여 직관적인
면과 정형적인 면을 함께 atest

* 2장은 분할정복법으로                    는 방법을 다룬다.

+ 8장은 동적계획 설계기범을 제시한다. 어떤 경우 분할정복범 대신 동적계획법을 사


===== PAGE 6 =====
EJ

또

학생들에게 동기부여를 하기 위해서 각 장은 그 장
가능한 많은 예제를 foe   각 장의 뒷부분에서

ae

<<

용해야 하는지 설명한

* 4장은 탐욕적 방법을 논의하고, 최적화문제를 푸는데 동적계획법과 탐옥적 방법 중
어느 방법이 좋은지 비교한다.

* 5장과 6장은 되추적과 분기한정 알고리즘을 각각 다룬다.

* ?장에서는 알고리즘의 분석에서 (문제의 BAS 다루는) 계산복잡도로 주제를 바꾼
다. 여기서는 정렬문제를 분석하여 계산복잡도를 소개한다. 정렬문제를 선택한 이유
는 그 문제가 중요하기도 하고, 정렬 알고리즘의 종류가 매우 다양할 뿐 아니라, 가
장 중요한 이유로서 (키의 비교만으로 정렬하는 알고리즘인 경우) 정렬문제의 하한

만큼의 시간에 수행하는 정렬알고리즘이 존재하기 때문이다. 정렬 알고리즘을 비교

한 후, 키를 비교하여 정렬하는 문제를 분석한다. 마지막으로, 키를 비교하지 않고
정렬하는 정렬 알고리즘인 기수정렬을 공부한다.
* 8장에서는 검색문제를 분석하여 계산복잡도를 계속 설명한다. 리스트에서 하나의 4

색하는 문제와 리스트에서 《번째로 작은 키를 검색하는 문제인 선택문제를

Sn fe
dc om
= 쏘

e
co
on
rlo
된
sn
N
110

정도와 NP 이론을 알아본다. 이 AS 접하기 쉽고 엄밀함도 유
기 위해서 시중에 나와 있는 알고리즘 교재보다 더 자세히 이 내
식 시간 알고리즘을 찾은 문제, 다루기 힘들다고 증명된 문제, 그
증명되지도 않았고 다항식 시간 알고리즘도 아직 찾지 못한
설명한다. 그리고 집합 와 WP, //7-완전 문제, NP-S-S
이와 같은 여러 문제 HHS 사이의 관계를 분명히 이해하지 못하
논하기 쉼기 때문에 유의해야 한다. 이 장의 마지막으로 근사 알고리즘을 설명

지

6
에
rr
빔
=
Hu
Ee
nn

c
로
dn 00
때
7)

2 A
로
N
rh,
nf
i

a ol

a 고
nit 10,
>»
2,
my
illo
[모
>»

eae

1°
oh
if

에

에
Sor 개

[
pe
S
om by
rlo

So

ve 「
rr
tlo 」고   4

알고리즘과 유전 프로그래밍을 다룬다. 이론뿐만 아니라 금융 거래 알고
실제 응용 사례도 공부한다.
리드 알고리즘, 어떤 수가 소수인지 결정하는 새로운 다항식 알고리즘과

aU
oN
o 다
am

에
j

N,
lo
ox,
\
으
KI
모 미
N
ㅇ
및
a

m

e

S
om 【
rlo

텍처와 PRAM BES 다루는 병렬 알고리즘을 소개한다.
교재에 빠리 vee      a i 필요한 uss 복습한다.

ow 는
NFP at ok
00 So mk
ere
by 브   x7
weg
a 내:
tas \
ba
co 시
a 22

fu

=

pe

2°

퇴보

bo

i

a

clr

dO

ox,

호

x

Ac

[때

ot

ft

Q
rir 위
ANG
om,
2
ee
ofl
4

에
rr
ne,

Ky
aU
ON
비야

@
io ee
dt oR Sl 4

구현하는데 필요한 ASA 집합 데이터구조

tifa
ied
3
roe
대

1
=|

내용과 관련된 이야기로 시작한다.
별로 묶여있는 연습문제를 제공한다.

습문제를 추가적으로 제공한다.

A
[뽀

만

연습문제 뒤에는 도전할 만한 가치가 있는 연


===== PAGE 7 =====
@‥0@00000 0
vi

한 문제를 공략하는데 두 가지 이상의 방법이 있다는 걸 보여주기 위해서 어떤 BASS
두 가지 이상의 방법을 사용해서 푼다. 예를 들면, 외판원 문제를 동적계획법, 분기한정법,
근사알고리즘으로 풀고, 0ㄱ1 배낭 채우기 문제는 동적계획법, 되추적기법, 분기한정법으로
푼다. USS 전체적으로 잘 엮기 위해서 자신의 최적 판매경로를 찾는 낸시라는 외판원과
관련된 주제를 여러 장에 걸쳐서 보여준다.

교재로서의 사용
앞에서 언급했듯이 이 교재는 알고리즘을 다루는 학부 고학년 또는 대학원 강의 수준에 맞
추어 기획하였다.
한 학기 강의 교재로 사용하는 경우, 다음과 같은 순서로 강의를 진행하기를 권한다.
1장 : 전체
부록 2 : Bil, B2
2장 : 2.1-2.5, 2.8
3장 : 3.1-3.4, 3.6
4장 : 4.1, 4.2, 4.4
54h: 5,1, 5,2, 5.4, 5.6, 5.7
64t : 6.1, 6,2
7A} : 7,1-7.5, 7.7, 7.8.1, 7.8.2, 7.9
8장 : 8.1.1, 8.5.1, 8.5.2
94} : 9.1-9.4
104} : 10,1-10,3,2

2-6장에서는 장별로 다양한 설계 방법을 적용하여 다양한 문제를 푸는 알고리즘을 소개
고 있다. 나름대로 몇 개만 선택하여 제시했지만, 실제로 어떤 절을 선택하여 강의할 지는 강
사의 자유의지에 맡겨둔다.

LAS} 15장까지 한 학기에 모두 다루기는 불가능할지 모르겠다. 하지만 12449] 내용은 첫
10개의 장 내용을 모두 소회한 학생들에게는 별로 어렵게 느껴지지 않을 것이다. 그리고 미적
분학을 수강하여 수학적 기초가 단단한 학생이라면 장은 관심 있다면 혼자 읽고 따라 갈

수 있다

에
…

강사용 강의보조자료
강사용 연습문제 풀이집과 파워포인트 강의슬라이드

0
olN

빙을 득한 강사에게 제공한다.

감사의 글
이 원고를 읽고 유용한 제안을 많이 해주신 모든 분들께 감사를 표한다. 특히 요청할 때마
다 원고를 빠르고 철저히 검토해 주신 William Bultman, Jack Hade, Mary Kenevan, Jim
Kenevan, Stuart Kurtz, Don La Budde, Miguel Vian 등 동료들에게 감사를 표한다. 또한


===== PAGE 8 =====
@0000000
Vil

통찰력있는 비판을 통하여 이 AS] AS 향상시켜주신 전문가 심사위원들께도 감사를 표한
다. 그 중 많은 사람들이 우리가 기대했던 것보다 훨씬 자세히 검토해 주셨다. 그들의 이름
은 David D, Berry (Xavier University), David \. Boyd (Valdosta State University),
Vlaminir Drobot (San Jose State Univetrsity), Dan Hirshberg (University of California
at Irvine), Xia Jiang (Northeastern Illinois University), Raghu Karinthi (Western
Virginia University), Peter Kimmel (Northeastern Illinois University), C, Donald La
Budde (Northeastern Ilinois University), Y, Daniel Liang (Indiana Purdue University at
Fort Wayne), David Magagnosc (Drexel University), Robert J, McGlinn (Southern Illinois
University at Carbondale), Laurie C, Murphy (University of Mississippi), Paul D, Phillips
(Mount Mercy College), H, Norton Riley (California State Polytechnic University,
Pomona), Majid Sarrafzadeh (Northwestern University), Cliff Shaffer (Virginia
Polytechnical Institute and State University), Nancy Van Cleave (Texas Tech
University), William L, Ziegler (State University of New York, Binghamton), 끝으로
Taylor} Franciso]7] 감사하며, 특별히 201210] 출판한 나의 교재 Contemporary
Artificial Intelligence2] 내용을 이 교재의 새로운 10장인 유전 알고리즘과 유전 프로그래
Yo] 쓸 수 있도록 허락해준 8800 00802에게 감사를 표한다.

|

이 정도의 대형 책을 만드는데 오류가 있는 건 어쩌면 당연하다고 할 수 있다. 오류를 찾았
거나 개선에 대한 제안사항이 있다면, 언제든지 들어줄 용의가 있다. 제안사항은 다음 주소
로 보내주시기 부탁드린다. Email: RE-Neapolitan@neiu, edu

감사합니다.

Oo fl


===== PAGE 9 =====
“알고리즘의 설계와 BAS 컴퓨터과학의 핵심을 이루고 있으며, 컴퓨터과학 모든 분야를
이해하는 기초가 되는 아주 중요한 분야라고 할 수 있다. 컴퓨터로 특정 문제를 해결하는데
있어서, 그 문제를 과연 컴퓨터로 풀 수 있는지, 만약 그렇다면 어떻게 푸는지, 또한 얼마나
효율적으로 풀 수 있는지, 그리고 여기서 효율적이라는 것은 어느 정

JES 이야기하는지 등
을 이해하는 것은 매우 중요하다. 왜냐하면, 본문에서 계속 반복하여 강조하고 있지만, 특
정 문제를 풀 때 그 문제의 BAS 이해하고 접근하는 경우와 그렇지 않은 경우는 큰 차이

가 있기 때문이다.

알고리즘의 설계와 BAS] 원리를 설명하는 Ao] 시중에 많이 나와 있지만, 알고리즘의
설계방법과 BARES 체계적으로 이해하기 쉽게 쓴 Ae 의외로 드물다. 특히 외국어 책
은 국내 학생들에게 그 내용이 제대로 전달되지 못하는 경우가 있음을 알고 아쉬워해 왔다.
그러던 와중에 이 AS 접하게 되었고, 이 Bo] 다른 Aol] 비해 수학적이나 이론적인 지식
이 부족한 학생에게도 알고리즘의 설계와 분석에 대한 이론을 쉽게 이해할 수 있도록 자세
히 설명해주고 USS 발견하였다. 따라서 학부 3학년 또는 4학년에 개설되어 있는 “알고리
즘 설계 및 분석” 과목에 적합한 교재라고 생각한다.

이 AS 번역하면서 원서의 내용에 충실하면서 정확한 의미를 전달하도록 최대한 노력하
였으며, 빠진 내용이 하나도 없이 모두 번역하였다. 혹시라도 책에 오역이나 내용이 불분명
하게 기재된 부분이 있으면 망설이지말고 doh@hanyang.ac,kr= 연락해주길 바란다. 마지
막으로, 개정판이 나올 때마다 출판할 수 있도록 관심과 수고를 아끼지 않은 홍릉출판사의
관계자 여러분께 감사를 드린다.

2017년 1월
도경구


===== PAGE 10 =====
chapter 1

chapter 2

차례

알고리즘 : 효율, 분석, 차수 1
4.1 QETT ZS 아여아여아어이아아이어 2
123 BE 욱저의 알고리즘 개빌의 중요시 nnsentassensssnsenasnntnnsnssonnstinsnssnnsseesennsnonenseiss 9
1.2.1 _ 순차검색 대 이분검색 ……..아이이이9이이아아아이이이이이이이아아아아 9
1.2.2 피보나치 수열 ……어아아에어여아아이어아아아이이아이이이이이시이이이이이이이이이이이이이이이이이이이 그
1.3 알고리즘의 분석 ersessessesseeseeseeseeseensennsessessessenseseessessssnssnesnssnsenesseeaeeansanesessessneaneaneeneeseey 16
1.3.1 - 시간복잡도 분석 …아아아아아아아아아이이아아이이이이이이이이이이이시이이이이이시이이이이이이이아아아 17
13,2 이론의 적용 vrreeseeseeseeseeseeseeseeseeseeseeseeseesnessssnssesnssnssnesseesessseseesseseesecseseseseneey 23
1.3.8 정확성 분석 ……아아아아아아아아아이이이이이이이이이이이이이이이이이이이이시이시시이사시이아사사 24
모시 으개어0000000000000000000000000000000000000000000007000 24
1.4.1 차수의 직관적인 소개 ……………아%여여어999이이999이이이어이이이이이아아아이어아아 25
14,2 차수의 정식 소개 creeecseceseesseesessesseeseesesnesessseseesesesssnsssssnssnsssssssessensenseness 28
  1.4.8 극한을 사용하여 차수를 결정하기                              38
1.5 Of] BHO] 개요 vvvvrvrescreesesseseesetsessesseseseseseesenseseesesseesseesessssessssseessessesesessesseseeseseeeeseegs A
FAUT] vcrecseeseeesseeseeesseenesneseenseneseenssssssssenssessesnssesssssssesssssssneseanssssnsseenesnsaesassnssesneansaneneaneeney a
분할정복 49
40. 0 50
2.2 _ 합병정렬 ………아아아아아아아아아아이이아아이이이이이아아이아아 54
400므은는롱-!큰는볼0000000000000000000000000000000000000000000000000000000 61
2.4 빠른정렬(분할교환정렬) ee 62
2,5 ASE PWM O] 행렬곱셈 알고리즘 ……아아아아이아어이이아아이이이이시이 68
2.6 큰 정수 계산법 wrreeeseeseeeeeneeneeneeseesnenneeneessesseseesecsssssssseeseeseesscsnseseesessescsncsnssseeseeseesncens 73
2.6.1 큰 정수 표현: 덧셈과 기타 1차시간 연산 ………………아아아아에아아아바아사아사아아아아아아아 73
D6, 2 큰 정수 AR vesesseeseeseeseeseeseeneensenssnsenesnceseeseesceseesessessceseaseesseseeseeseeneeseaneeneeneens 74


===== PAGE 11 =====
x

chapter 3

chapter 4

chapter 5

2.7 임계값의 eS Nene 79
2.8_ 분할정복법을 사용할 수 없는 경우 ………………아아아아아아아아이이이아아아사사아아사아 83
AA cereceeeeeeeeeeeeseeeeseeeesesneseeeeseseesesteessseessseessssensssensssseessnssssessssesserssssresssneseeseneeneneenty 84
동적계획 91
3.1 _ 이항계수 구하기 ………아에아아아아아아아아아이아아이아이이아이시이이이이이이이이이이이이9이이어어이이시사아아아아 92
3.2 _ 프로이드의 최단경로 알고리즘 …………아아이아아이이아이아이이이아아이이이이이 96
3.3 동적계획과 최적화 SAA] ceececeeeeceeeeeeseeeeeeseeeseeseeeeseeseseeseesseessenssesssssseessensseseseeesess 105
3.4 연쇄 행렬곱셈 …………아아아아아아아아아아아아이아이이아아이이이이이이이9이이이이이서이이아아아아아아아아 106
3.5 최적 이분검색트리 …….…아아아아이아아이이이아이이이이이이이이이아이이이아이이이이이이이이이아아아 115
BG 기미느문그 이0000000000000000000000000000000000000000000000000007002 124
(두 BY NANO f= eS = EE 131
ALT] creceeeeeeecseseeeeeesesesesesseneneesessssseeneesesssssssssnenenssssssssssseeessssssssessessesacecseeseasesecessnsneneeey 138
탐욕 알고리즘 143
4.1 - 최소비용 신장트리 ………아아아바아아바아아아아아아이아아이이이이어사이이이이이이이이이이이이이서이이이아사아아 147
4.11 프림 알고리즘 ovvvesssesssessseensessvncessnsssvcnsvcenvossvssuncenseccnseensennsenneseeaesseesneeenessnees 150
4.1.23 크루스칼 알고리즘 ………아어아아아9어이어아아이이아이사아이이이이이이이이이이이이이이이아아아아아 155
4.18 프림과 크루슷갈 알고리즘의 YT 며……어어쳐애어어아어어애어애아시이어버사사아사저서시 160
4.1.4 마무리 토론 eeeeeteseeeeeeeteeeseetesesseneesenesssnessesesessssssesressssssssseesssseesseseseseessseees 161
4.2 단일출발점 최단경로 문제를 푸는 다익스트라 알고리즘 …아아아아 161
4.3 스케줄 MPD crrrceeeeeeeeeeeeeteee tees eeeseeneseseenessenesessenenessenessseesssseseesssessssssssssseesensnesseneys 164
4.3.1 - 시스템 내부의 총 시간의 최소화 erereeeereeeeseesseeeesseeesseessseessseessseeesseesseessses 165
4.3.2 마감시간 있는 스케줄 짜기 ……어어아아에아아아아아아아아아아아아이이이아사아이이이이이기아아사사아아 168
AA GATED 준그=0000000000000000000000000000000000000000000000000000000000000000077 174
4.4.1 - 전치 코드 EEE 175
4.4.2 -허프만 OPT AD eoeevvsesvencvensvvosseesscssnssssorsvonssoesnstesesnsescnsscnsensssnneesnecsneenneenasess 177
45 탐욕 알고리즘과 동적계획 알고리즘의 비교: 배낭 채우기 문제 ……………아아아아아아아 180
4.5.1 _0-1Ｌ배낭 채우기 문제의 탐욕적인 해법 ……여어…………아여8애애에아아애여야 181
45,2 배낭 빈틈없이 채우기 문제의 탐욕적인 접근방법 ……………어………애% 183
4.5.3 0-1 배낭 재우기 문제를 푸는 동적계획법 00000” 00770 183
4.5.4 O-L 배낭 채우기 문제를 푸는 동적계획법 알고리즘의 개선 ……………… 184
AAT] ccceeeeeteeseeseseeseeseneeteseereneeseeresssesssesessssnsssssssssesssssssnseenenensiseesienteneeeeeey 187
되추적 193
5.1 -되추적 EE 194

52     22-여왕말  문제 00000000000000000900000000000000000000020000000000000000000040000000000010000000000000000000000000000* 201



===== PAGE 12 =====
chapter 6

chapter 7

chapter 8

X1
5.3 몬테칼로 알고리즘을 사용한 되추적 알고리즘의 효율성 BA …………………… 206
5.4 부분집합의 St 쿠하 cvveneeeesceseerscescscevsccnssoescsesecnssesscnssecnsncsscassscssesecncesssensasenseeeaseoes 210
5.5 그래프 샘칠하기 coneeveeeeeeeseesssvesscsssnssecscesceseenssnsensensenscnssasenssascsscsscescessensensessessesesveees 215
5.6 해밀튼 회로 문서 ceceeeesseesssscccsececscsncscevcscscsscssncsssnssesscnesecsnacsegnscesscnsessscaseossesvsnssesvenses 219
5.7 0 배낭 채우기 SBA ccoeceeesesseeeeseeeessseesesssescescscnensseeneneneseesessesssssensssseassessesssneneseees 223
5.7.1 OL 배낭 채우기 문제를 푸는 되추적 알고리즘 …………… 223
5.7.2 O-1 배낭 채우기 문제를 푸는 동적계획 알고리즘과 되추적
알고리즘의 비고 …아아여이아이6아아이아이이이이이이이이이이이이아아사이이시이새아이사지 231
연습문제 …ㄴㄴㄴ 0이이여이이0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 232
분기한정법 237
6.1 분기한정을 0- 배낭 채우기 문제로 ABSIT] ………….%%… 239
6.1.1   분기한정 가지치기 너비우선검색 이이아000000000000000000000000000000000시00000 239
6.1.2  분기한정식 가지치기 최고우선검색 이이 244
6.2   외판원 문제 SOOO eee r meee seen nese eee eee eee eee ee eee esse ee eee eeE ee eee eee eee EEE EEE eee EE EE Eee eeeeeE eee eEeeeeeeeeeeeeeseeees 249
6.3 확률적 추론(진단) …………아아이이이이이이이이이이이이이이이이이이이이이이이이이이이이아아 258
다스 고고 이오 00은오으은을을으을으올선서 거 266
계산복잡도의 소개 : 정렬문제 269
71 계산복집도 ………아어아아아아아아이아에이아아아어이사아사아아아아다아이이이이이이이이디아아아아아이이시이이아어아어아에 270
7.2_삽입정렬과 선택정렬 ……………아아아009999099999999909999999999999999999999999999999999099009909009 272
7.3 비교 한 번에 기껏해야 역이 하나 제거되는 알고리즘의 하한선 ………………'.… 27
7.4 합병정렬(재고) cvvcrecessecessecessesesseseesesesssssssssssesscsesseenensasensneeesseseesesesseseessseessseeeseeeeseeees 279
7.5 퀵정렬(재고) RR 285
7.6 합정렬 …아아아아아아아아아아아아이이이이이9이이이이9이이이이이이이시0000000090900000009000000000000000000900000090 287
이 회 쿠조와 기본적인 회 UAE Bey wnsecncesetsesennessnnecssesconescnnescnneconnerenseosoneres 287
76,2 SAPO] 구현 crvreesscsesessesessesessssessssensseseesesseeseenseseensasessseseesssesssssesaesesseneaes 291
7.7 SE, 퀵정렬, 힙정렬의 비교 ……아이이아이이이아아이이아이이이이아 208
7.8 키의 비교만으로 정렬하는 경우의 하한선 ……………………%““여이 299
7.8.1 정렬 알고리즘의 결정트리 cercrereeeeseeseeteeeeeteseeeeseeeesesseeeessseesesesesssseseseesees 299
789  최악의 경우 계산복잡도 Fo) Se) 302
7.8.9 평균의 경우 계산복잡도 하한 ceveeseeseessessessessesseessesseeneensennennseneeneeneeneenensenaes 304
7.9 분배에 의한 정렬(기수정렬) ……………아00066 309
AZ A crcvceereceeeeeseseseessesceeeseessesencscesenssssessscsceceeenensnsnsaesesesssssnsseseseseenseeseseseseaeeesssssssasasenens 313
계산복잡도 : 검색문제 319
8.1 비교만으로 검색을 하는 경우의 하한 …………여여아 320


===== PAGE 13 =====
Xll

chapter 9

chapter 10

8.1.1 eS oo) 경우 하한 …어여어어어어아서사사사사사아사사아서아자사자시아서아사시사사사사서아이이이사사사아새 392
8.1. 2   평균의 경우 하한 Serer ere rerre reese rreer rere errr rrreer rere reer cere ir etree ere ere eee eee 324
8.2  보간검색 se eeececeecenceeeeeeeencenceaeeseaenseeseseneeseesessnsensesensensensnsersnsenensensenensenseserseeenseneeeeneen ens 330
8.3 BIO ATO] ZYAH cvssssssssseeccssssssseeeccensssssnnsecccnssssnnnsseeesssnnunnsscesennnnnssseeesennnnnnsseeeseeenneny 333
8.3.1 이진검색트리 erecesssssseeecccssseeeccssssnssseccnssnnncecsssnnnsscecssnnnseceesannanssseenannasseeetentey 333
33.0)   B-Ez] eeeeerre rere rrereererrererrrrrrrrrrrrrrrrrr rere ere eee rere eee eee eee eee 337
BA SHA crceeceseeseeseseeseesseeneenssteneeneenenteneensensnsensensatsnsensansnssssasssssassesessessecessessassecessesseseseesees 338
8.5 선택문제: 방해꾼(적) 논법의 소개 ………………아아아에아사아사에아새사사사사새사사사사새아사아 344
8.5.1 - 최대키 찾기 …아아어에아어에아새사아새어아아사아서아아사사아이어아자사아사사아사아사자사아사사사사사사아와 344
852  최소키와 최대키를 pm 찾기 000000000000000000000000000000000000000000000000000000000000000004 345
8.5.8 - 차대키 찾기 …어아에어아어어어어아아사새사사사아아시아사사아아사사아시아아이이아시아아사사사사사아사사아사 352
8.5.4 4-번째 작은 키 찾기 ……어어어어아아서사사새사사사새사사사사아시아아사시아사아사사사사사사아사새아세 357
8.5.5 선택문제에 대한 확률적 알고리즘 ……………….…여아아어에아애애세아사세세아사사아 365
연습문제| coseecsseesesseecssecessenessesesssnesssnensssensssecssnecssssecsnsceanccensccenscceansecansecanccensceennacennsceunscsanss 369

계산복잡도와 다루기 힘든 정도 : NP 이론의 소개 375

9.1 다루기 힘든 ed 376

9.2 입력크기 : 재고 vvecervesessesseseesssssecssssessnscssnsecenncennneesnneeennseesnseesnscesnnensanecennecsuseceasscsayss 378

9.3  문제의 3가지 일반적인 분류 00000000000000000000=0000000ㅠㄴㄴㄴㄴㅇㅠㄴㄴ……ㄴ……ㄷ…0ㅇ<…00000ㄷㄴㄷㅠㄴㄴㄴ<40000404<60000000000000040 381

9.3.1 _다차시간 알고리즘을 찾은 문제 …………………아여아어아어아애에새에아아사아사아사아사아서 389

9.3.9 다루기 힘들다고 증명된 문제 …………… 아어에아에에사에새아사아사아사사사사사사사새 389
9.3.3 다루기 힘들다고 증명되지도 않았고, 다차시간 알고리즘도

찾지 못한 문제 eceececesssssssseeeeseeeeecesssssnnnnseeecececsnnssnnnnsseececessnnsnsnnnasssseseenee 388

9.4   NP 이론 000……0000000ㄴ0……000ㄷ0ㄷ400ㄷ<<ㅠ0ㅠ0…004000466.04064044000460060060460060000000000064=66ㄴ………000000000090054044 383

9.4.1 와 NP 집합 vvrevesesesessssssssseeeesseseccesnssssnnnsssseeceecssnnssnnansseeeeesseesnnnnnnnsseeeeeeene 385

94  NP-Complete 문제 …ㅇ0000000000000000000000000000000000000000000000000000000000000000000000000000000000 390

9. 4. 3   NP-Hard,  NP-Easy, NP-Equivalent 문제 00000000000000040000000000000000000000시1 400

9.5 _ NP—Hard 문제를 푸는 방안 ………아아아아아아아아아아아아아아아이이자아아어사아아아아사사사아사사사아아아 404

9.5.1 외판원 문제를 푸는 근사 알고리즘 …………어……%여%여여%여%어아어아새아세아사아서 405

9.5.2 상자 채우기 문제를 푸는 근사 알고리즘 ,아아어애아아애에에에사아아아 409

연습문제| ……어어아아아아여여애아아아아아이이어아아이이이이이이이이아이이이이이이이아이이이이이이아아아이어어아아아아아사사사사사아아 414

유전 알고리즘과 유전 프로그래밍     417

[=]
10.1  유전학 리뷰 00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 417
10.2 오전 알고리즘 00000000000000000000000000000000000000000000000040000040000000000000000000000000000000400000000000000000000 420
1081 알고리즘 900000000000000000000000000000000000000000000000000000000000000000000000000000000이이이 420

10, De y)   사례 0000000000000090000000000000000000000000000000000000000000000000000000000000000000000000000000000000 491


===== PAGE 14 =====
chapter 11

chapter 12

xiii
10,2,3 외판원 문제 crceeeeeeeeeeeeeseeseseseeeeseeeeeseesesessssesneeaseneneeeeensensnsasenseseneeeseeseneses 424
10.3 유전 프로그래밍 ………아에이서 433
00 시스 으으으 으으 으으 434
10,3,2 인공 개미 vrvcveeseseseseeeeesesteeeesessssssssesesssssesneneneasaseeenenessseeseneneneneseeeeeasseseeeeees 437
10.3.8 금융거래 응용 EE 439
10.4 논의 사항 및 추가 공부 자료 …ㄴ……%……여0 666이다이00이이이아어라이아 442
ABBA ccccrercececesesstesesesseeseseesesesesesesesessssnsnsvsvsenensassessaesesenensesssssssseesseeeeeeeeeeeeeecesenesenenesen 442
정수론 기반 알고리즘 445
111 정수론 ATH crreereeseseseseeesesensnenesesesssenssssesssssssssesensnsessensessesssssssssssssscssaeeeseseseseecececeeevees 446
1111 합성수와 소수 …………어여어아애에어자사여이0여애애아아바0아이이이허아아바에아이아에아어이아이에아 446
11.1.23 최대공약수 veeereeeeteteteeseteteetesteteeneseeesseeessessessssessessssssesessesseseseesesaseeeaeeeeeeees 446
111.3 소수 인수분해 …………여이……메러자자해아에데에에니애에이애이에아하애어에메에에이이이이에에이 450
11.1.4 최소공배유 ……여어아에아아아아9이이이이이이아여이06이이아아0아아아이아어아 452
11,2 최때공약수 계선 ceeeeeeeeeeseeesesesesesesessssecssssssscsesseveceeeesesenesesesessseseseseseseseseseneasassseeesees 452
11 21 SD 알교리즘 acacia estes venestnesnesavernennennnannernnnncicnenreenascavensonenensany 453
1141.89 유클리트 알고리즘의 확심 …… ……………이나의니어아이에이네태이사거지에어네가이어에거 457
11.3 모듈러 연산 소개 Ce 459
11.8.1 Ba =o) BEE 459
132 oh 법으로 한 활몽여여거어이여겨에에여세서서에어에어이세이 이이에에테게게이 460
11,3,3 뿌부그륨여여여매어아어이셔너데겨타이이서저타서기저아히거해시아서이가여에이1아여데아데다데서어아나에나 466
11.4 모듈러 1차 방정식 풀기 …………아아아아아0990999960이이이시이 472
11.5 모듈러 거듭제곱 계산 ………아아아아아아아 477
116 큰 소수 찾기 wrrerererseeeseeseseseneeecesecenavevensnsssescsesesenesesenenenesesssssssssesessssseeeeesesecasenesesaseves 480
11.6.1 FE 소수 구하기 …여어아아아아라아아이이이이이이이이이이이이이이이시이이이이이아아이이이사이아이아아이이 480
11,6,2 주어진 수가 소수인지를 검사하기 ……………여“아아 481
11.7 RSA 공개키 암호제게 ……어어애에어서이레이이이자아이어이어어아아아아테아디이이이애어아아어이테에이아다이아 498
11.7.1 SLAF) 암호 체계 ………아아아아에아아아아아아이아이이이이이이이이이이이 499
11.7.9 RSA 함호체겨 ccceeeeeeceseeeeseseseeeeseseseseeseneeesescasseeeeeeneneneaeeeenseseeeseeeeneneneees 500
연습몬저| cotsersepcesaracncseres sesso ssssccetecsssneesercesssucbrenseaenessaceesacecstacsncesessoeotoneseonosctssaesenosesserstane 503
병렬 알고리즘 개론 507
12.1  병렬 구조 …ㄴㅇㅇㅇㅁㅇㅁㅇㅇㅇ0ㅇㅇ00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 510
1282.17 2 Ken in 2 Sc 510
12.1.2 주소-저장장소 구성 Seisnle Shaessia¥sleiannw oovlcds sauces esee secs segue vancees cons esau eeeeseestesesaseawemen 511
12,1,3 상호연결 네트워크 ceeeeeeseeeeeseeeeseeeesesseesnesessseescaeeneneeneaseneeaseeaeeneneeesneseenes 513
12.2 PRAM 모델 crrscsssessssesessssesessescsessssssesscerssesesesensesensssssnssscssscsenssesssssssssssssesssesessesesseees 516


===== PAGE 15 =====
X1V

appendix A

appendix B

appendix C

12.2.1 CREW PRAM 모델에 대한 알고리즘 설계 ccceseseeeeeeeeeeeeeeeeeteeeesneeesnnecesnnees 590
12.2.2 CRCW PRAM 모델에 대한 알고리즘 설계 ……바바바바사바아아바아사아아아 527
연습문제| ooeecssssecsssseesssssseesssseecsssseesssssecsssssccssssecsssssecsunseceenseceeanscensansecsannsccennccesansscessssssssssses 530
수학 533
AA :기드론00000000000000000660006 533
「느그은000000000000000000000로00000 535
A.B 수학적 귀납법 cecssseeeessssseessssssneecssssseensnsnneccsnnnsceennnsseessnnnscessnnasessnnscesssnssscessssssessssess 536
AA - 정리와 보조정리 vvvvveesseesccssssssssneecccssnnnnseeeecennnnnneseeecesnnnnneseecesssunassecessssunessseceessssessss 542
:열서비 00000000000000000009800006 543
A.5.1 CHAO] 정의와 특성 아아어에아아사사아사사새사새사새사사새아사사새아사사자사아아사사사사사사사사사사새 544
시 59 자연대수 vvvssssessesssssesesssssseecsssnnsecssssnsccessnnsceesnnnseeeeannsseesnnnsssessssnssscessssssressseey 545
AG 집합 ccvssseeseesseesecesssseecsssssecssssnssecsssseesssnseecsnsnsecesunsseesunsceeeannseceesusescesssesscesssesecsssessesey 547
Ty AS =) ga 549
A 8    확률 Preererre reer rere eer err rere errr rere reer reer e eee ee ete 552
시 81 - EERE QA ccsssssesssssssesessssnesccsssncecensnnscecsnnneccesnnneeeesnnnacecsnnnsecessnanssseessnessessssess 557
N82 기 대치 crveessressesesssssssssssssssseecsnsnssecccssnnseccesunseseesannneeesnnnsecessnnnesseessssssssessssssees 561
연습문제 eccosseeeceosssseeeesssseeecssssseecsssssseeessssseccsssunscecsnsnssceeeansaceensunnacensnnnscerenunssecsnunesscesssessten 563

B1   귀납법으로 재현식의 해 구하기 Prrrrreeee errr rrr rere eee eee eree rete eee eee teeter eeer reer 567
B.2 특성식을 이용하여 재현식의 해 구하기 ccreeeeeeeeeeeseeeeeeeseeeeeesssnneeeecesssseseeeeesssssens 571
2.20.1 - 동질 1차 nn 571
B.2.2 BEAL 1차 재현식 …아어아아어아아서사사사사사사사사사아사시사사아아시아아시아아사사사사사사사사사사사사 579
2.2.8 - 변수의 변경(치역 변환) ooreeeseesseeeseeeesnseecensnneeeeensnnseessnnaseeesnnnsessessssssessssssssen 584
8.3 치환에 의한 재현식의 해 구하기 ………….…아아서어에아사세아사사사사사사사새사사사새사사사사사아아아 587
BA n& /(양의 상수)의 거듭제꼽으로 하여 얻은 결과를 모든 으로 확장하기 ……… 588
8.5 _ 정리의 증명 oveeseccssssseseecsssssssssescsssssnnsssecsessnsnnsececesnnnssesseeeennnanseetessnnnnnsssseessssssssssesee 595
브그이00000000000000000000000008988006 597

서로소 집합의 데이터 구소 603


===== PAGE 16 =====
Chapter 1

알고리즘 :

효육

9

| Se SyROr 전화번로는 바르 'ㅎ6'

브브         으
부브로 넣기면 찾을 수 gm.

분석, 차수

o]    책은 컴퓨터로 문제 푸는 기법을 배우는 책이다. 여기서 “기법"이란 프로그램을

작성하는 언어나 스타일이 아니라 문제의 해답을 찾는 해결법이나 방법론을 뜻
한다. 예를 들어, 바니(88706/ Beagle, 위 그림의 만화 주인공)가 “홍길동"이란 이름을
전화번호부에서 찾으려 한다고 하자. “홍길동"이란 이름을 찾을 때까지 첫 쪽부터 시작하
여 한 장씩 넘겨가며 OSS 찾지는 않을 것이다. 사실 이런 식으로 전화번호부에서 이름
을 찾는 사람은 아무도 없다. SSS 바니는 전화번호부에 이름이 가나다순으로 정렬되
어 있다는 BS 이용하여, 'ㅎ'이 있을 만한 KS 어림잡아 바로 전화번호부를 편다. 너무
뒤로 갔으면 조금 앞으로 간다. 너무 앞으로 갔으면 조금 뒤로 간다. 이런 식으로 “홍길
동'이라는 이름이 있는 쪽에 도달할 때까지 계속 반복해서 앞뒤로 뒤적인다. 이 두 번째
방법을 개선된 °]42-444 (modified binary search)o]@} 하고, 첫 번째 방법을 순차검색
(sequential 868704/이라 한다. 이러한 검색 방법을 1.2절에서 자세히 공부할 텐데, 미리
언급하는 건 주어진 문제를 푸는 방법이 여러 가지가 있는 이유가 표현 언어나 표현 스타
일이 달라서가 아니라고 알려주기 위해서이다. 컴퓨터 프로그램은 여러 방법 중에서 그
저 한 가지 방법을 선택하여 구현한 것일 뿐이다.



===== PAGE 17 =====
2      chapter ㅣ 알고리즘: 효율,

차수

고

A

2장에서 6장까지는 문제를 푸는 다양한 기법을 제시하고, 각 기법을 여러 가지 문제를
푸는데 적용시켜 볼 것이다. 기법에 따라서 문제를 푸는 독특한 단계별 절차가 있는데
이를 Yaz] (algorithm)°]e}a1 한다. 문제를 푸는 기법과 적용방법을 익혀두면, 어떤
새로운 HA} 주어졌을 때 그 문제를 해결할 수 있는 다양한 레퍼토리를 준비해 놓음과
다름없다. 문제를 푸는 기법은 다양하지만, 기법에 따라서 알고리즘의 성능은 차이 날
수 있다. 전화번호부에서 이름을 찾는 경우 개선된 이분검색 방법이 순차검색보다 이름
을 훨씬 빨리 찾는다. 그러므로 어떤 문제를 어떤 기법으로 풀 것인지, 뿐만 아니라 만는
알고리즘이 시간(3206)과 공간(60800/의 사용량을 기준으로 얼마나 효율적인지를 분석하
는데 관심을 가져야 한다. 여기서 시간은 알고리즘을 컴퓨터로 실행할 때 걸리는 시간의
길이를 말하고, 공간은 필요한 메모리의 크기를 말한다. 컴퓨터의 처리속도는 계속 빨라
지고 메모리의 가격은 점점 싸지고 있는데, 왜 여기서 효율성이 관심거리가 되어야 하는
지 의아해하는 SALE 있을지 모르겠다. 이 장에서는 이 BO] 나머지 부분을 이해하는데
필요한 기초 개념을 공부한다. 이 과정에서 컴퓨터의 처리속도가 빨라지고 메모리의 가
Ao] 싸지는 것과는 무관하게 효율성이 왜 항상 중요한 관심거리가 되는지도 알아본다.

® 11

알고리즘

© 예제 11

지금까지 “문제”, "해답", “알고리즘"이라는 단어를 언급하였다. 이 단어들의 의미가 무
엇인지 대충 짐작이 가겠지만, 기반을 확실히 다지는 뜻에서 이 용어들을 자세히 정의
해보자.

컴퓨터 프로그램은 정렬하기(600008/와 같은 특정 작업을 수행하는 개별 모듈(0ㅁ0-
dule)& 모아서 구성한다. 이 책은 프로그램 전체 설계보다 특정 과제를 수행하는 개별
모듈의 설계에 중점을 둔다. 특정 FAS BAl(problem)2}51 한다. 다시 말하면, 문제는
해답을 찾으려고 물어보는 질문이다. 문제의 실례를 몇 개만 살펴보자.

개의 수로 구성된 리스트 SS 비내림차순(ㅁ0ㅁ0607688108 order) © = 정렬(60ㅁ0하시오. HES
SS 비내림차순으로 정렬한 리스트이다.

리스트0184)란 어떤 원소를 특정 순서로 나열해 놓은 것이다. 예를 들면, 다음은 수의
리스트이다.
S= (10,7,11,5,13,8]

첫 번째 수가 10이고, 두 번째가 7131, 등등 총 6개의 수를 나열한 리스트이다. 위의 예

제 1.1에서 오름차순(1006088108 0*064)이라 하지 않고 비내림차순이라 한 이유는 리스트
에 같은 수가 한 번 이상 나오는 경우도 허용한다는 뜻이다.



===== PAGE 18 =====
© 예제 1.2

© 예제 1.3

© 예제 1.4

© 예제 1.5

어떤 27} n7H 수의 리스트 에 있는지 알아보시오. 해답은 만약 <가 So} 있으면 “예"이고,
그렇지 않으면 “아니오"이다.

문제에서 값이 지정되어 있지 않은 변수를 그 문제의 Depo] el (parameter) Z}31 한다.
예제 1.1에는 ,9(리스트)와 7(4에 있는 원소의 개수)이 파라미터이고, 예제 1.8에는 9,
n, 2가 파라미터이다. 이 두 예제에서 n 값은 SS 검사하여 알아낼 수 있기 때문에 굳이
파라미터로 만들 필요는 없지만, nS 파라미터로 두면 문제를 표현하기 간편해진다.

파라미터가 달려있는 문제를 일종의 "문제 패턴"으로 볼 수 있고, 그 파라미터에 특정
RS 지정하면 "개별 문제"가 된다. 이렇게 파라미터에 지정할 값을 문제의 입력사례
020868000)라고 한다. 즉, 특정 입력사례에 대한 해답(601411020)이란 그 파라미터를 그 입
력사례로 지정하여 질문한 문제의 해답이다.

예제 1.1에 다음의 입력사례를 지정하면,
S=[10,7,11,5,13,8], n=6
이 입력사례에 대한 해답은 [5,7,8,10,11.13|이다.

예제 1.2에 다음의 입력사례를 지정하면,
S=[10,7,11,5,13,8], n=6, 2 = 5
이 입력사례에 대한 해답은 “예"이다.

예제 1,39] 입력사례에 대한 해답은 눈으로 SS 훌어보면서 바로 구할 수 있다. 97}
짧기 때문이다(너무 빨리 해답을 찾다보니 찾는 AAS 따져볼 여유도 없다). 그러나 n
의 입력사례 ge] 1000이면 눈으로 훌어보면서 정렬하긴 귀찮아지고, 그렇다고 눈으로
찾는 방식을 컴퓨터 프로그램으로 옮기는 것도 불가능하다. 어떤 입력사례가 주어지더라
도 해답을 찾아주는 컴퓨터 프로그램을 작성하기 위해서는 모든 인수에 대해서 해답을
찾아주는 일반적인 단계별 절차를 명시해야 한다. 이러한 단계별 절차가 바로 알고리즘

(algorithm)°]3), 문제는 알고리즘으로 푼다(60176)`라고 한다.

예제 1.8의 문제를 푸는 알고리즘은 다음과 같다. 의 첫째 원소에서 시작하여 *를 찾을 때까지
(2가 없는 경우 끝까지) 각 원소를 차례로 <와 비교한다. 만약 eS 찾으면 “예"라고 답하고, cS
찾지 못하면 “아니오"라고 답한다.

예제 1.5에서와 같이 우리말(자연어로 알고리즘을 표현할 수 있다. 그러나 이런 식으
로 알고리즘을 작성하면 두 가지 단점이 있다. 첫째, 복잡한 알고리즘을 말로 설명하기
쉽지 않다. 말로 설명할 수 있다고 하더라도 이해하기가 어려울 수 있다. 둘째, 일단 말로



===== PAGE 19 =====
4      chapter 1 알고리즘: 효율,

알고리즘 |.

Al, 치수

A

표현한 알고리즘에서 컴퓨터 프로그램을 어떻게 만들어낼지가 불투명할 수 있다.

C++ 언어에 익숙한 학생이 많으므로 C++9} 비슷하게 생긴 의사코드(6864000008)를
써서 알고리즘을 표현하기로 한다. C HE Java 같은 Algol 계열의 명령중심 언어로 프로
그램을 짜본 경험이 있다면, 이 의사코드를 이해하기가 별로 어렵지 않을 것이다. 예제
1,29] 문제를 푸는 알고리즘을 가지고 의사코드를 만들어보자. 예제 1.1과 1.2는 ol 국
한되어 있다. 그러나 일반적으로 순서집합(6ㅠㅠ06860 set) 속하여 BAS 매길 수 있는
원소라면 종류에 관계없이 검색하고 정렬할 수 있어야 한다. 레코드ㅠ60000) 또는 사전
(dictionary) 구조에서 그러한 원소를 키56")로 사용하기 때문에 정렬은 키를 대상으로
하면 좋다. 예를 들어, 개인의 신상 정보 레코드(사전)가 있다면, 개인의 주민등록번호를
키로 정할 수 있다. 키로 사용할 수 있는 데이터타입을 <6>6》066이라 하고 검색과 정렬
알고리즘을 만들어보자. 즉, 원소를 순서집합으로 AAS 수만 있다면 키로 사용할 수
있다는 뜻이다.

다음 알고리즘은 리스트 SS 배열(3ㅁ8)로 표현하고, “ol” 또는 “아니오"의 대답 대신
x7} 에 있는 경우에는 배열 내 의 leA(index)S 내주고, 그렇지 않은 경우에는 OS
내준다. 이 특정 검색 알고리즘은 순서집합의 원소만 다루도록 제한하지 않지만, 여기서
채택한 표준 데이터타입 keytypeS 사용해도 별 문제는 없다.

순차검색
문제 : 원소가 7개인 배열 에 원소 <가 있는가?
입력(파라미터) : 정수 7(> 0), 배열 (인덱스 WE 1부터 까지), 원소 a

출력 : 원소 가 위치한 SAAS location] AAS 안에 가 없으면 OF 저장)

void segsearch (int 22,

{

const keytype S|],
keytype x,
index& Jocation)

location = 1;

while (location <= n && S{location| != x)
location++;

if (location > n)
location = 0;

의사코드는 0++와 비슷해 보이지만 완전히 같지는 않다. 눈에 바로 드러나는 차이점
은 배열의 사용 방법이다. 0++는 배열의 인덱스를 0 이상의 정수만 허용하지만, 경우에
따라서 정수 범위를 배열의 인덱스로 사용하거나, 정수가 아닌 인덱스를 사용하여 알고

즘을 더 명확하게 설명할 수 있다. 따라서 의사코드에서는 배열의 인덱스를 임의의 집


===== PAGE 20 =====
나

@060600000
1.1 알고리즘 5

합에서 쓸 수 있도록 허용한다. 알고리즘의 입력과 출력 명세에 항상 인덱스의 범위를
표시한다. 예를 들면, 알고리즘 1.1에서 의 인덱스 범위가 1부터 까지라고 명시하였
다. 보통 리스트의 원소를 셀 때 1부터 시작하는 게 습관화 되어 있기 때문에 리스트에

는 좋은 인덱스 범위이다. 물론 이 알고리즘을 0++로 직접 구현할 때는 다음과

keytype S[n+1];

이이자리는 사용하지 않으면 된다. 앞으로 어떤 프로그래밍언어로 알고리즘을 구현할 것
인지는 고민하지 않을 것이다. 우리의 목적은 단순히 알고리즘을 명확하게 표현하여 바
로 이해하고 분석하는데 있다.

의사코드와 0++가 다른 점이 두 가지 더 있는데, 첫째는 배열을 프로시저의 파라미터
로 사용할 때 차원 배열의 길이를 미리 고정할 필요가 gical: 알고리즘 1.4). 둘째는
지역 배열의 길이도 고정할 필요가 없다. 예를 들면, 만약 이 example 프로시저의 파라
미터이고, 인덱스가 9부터 까지인 지역 배열이라면 다음과 같이 선언한다.

void example (int n)

{

keytype $([2..n];
    :
S12, n= 인덱스가 2부터 n 7A 배열 SS 나타내는데, 의사코드이지 C++ 프로그
램이 아니다.

절차를 더 간단하고 명확하게 표현할 수 있다면 실제 0++ 명령문 대신에 수학적 표현
A) 또는 말로 알고리즘의 절차를 기술하기도 한다. 예를 들어, 변수 가 low} 4%2값
사이에 있을 때만 명령을 수행하고 싶으면,

if low <= x && x <= high) {
}
대신 다음과 같이 쓴다.

if dow < x < high) {

}
가령 변수 cSt 변수 yo 저장된 값을 서로 Bet 싶으면

temp = X;

x J
yY = temp;


===== PAGE 21 =====
6

chapter ㅣ 알고리즘: 효율,

Ad, 지수

AC

대신 다음과 같이 쓴다.
exchange x and y;

데이터타입 keytype 이외에도 다음과 같이 0++에서 쓰지 않는 타입을 의사코드에는
사용할 수 있다.

데이터타입                                  의미
index              인덱스로 사용하는 정수 변수
number            Aint) 실수(ㅠ1021로 정의할 수 있는 변수
bool               “true 나 “false” 값을 가지는 변수

실수나 정수 중에 무엇 하나로 제한할 필요가 없을 때 number 데이터타입을 사용한다.
때로는 다음과 같은 표준이 아닌 제어 구조를 사용하기도 한다.

repeat (2 times) {

}

이 구조는 루프 내부의 코드를 nl 실행하라는 의미이다. 0++로 작성하려면 추가적
인 제어 변수를 사용하여 for 루프000로 작성해야 할 것이다. 루프 내부에서 제어 변
수를 설제로 표시할 필요가 있는 경우에만 for 루프를 사용한다.

알고리즘의 이름으로 보아 값을 내주어야 하는 경우에는 알고리즘을 함수로 작성한다.
그렇지 않은 경우에는 알고리즘을 프로시저(2++의 void 함수)로 작성하고, 값을 내주기
위해서 BAAS 파라미터(*6【6760006 parameter)S 사용한다. 배열이 아닌 파라미터는
선언할 때 데이터타입의 이름 끝에 앰퍼샌드(300678800) 기호 &를 붙인다. 이 경우 프
미터 변수에는 알고리즘이 내주는 값을 저장한다. ++에서 HSS 특별한 언급이 없어
도 주소를 전달하므로 굳이 앰퍼샌드 기호를 붙일 필요가 없다. 0++에서 예약어 0005
는 전달하는 배열 값의 수정을 막는 역할을 하므로, 알고리즘이 내주는 값이 배열이 아님
을 녀래배어    정한 WSS 알고리즘 실행 후 무시하려면) constS 붙인다.

른 언어를 주로 써서 0++가 익숙하지 않은 독자도 이해할 수 있도록 0++에만 독특
하게 사용하는 구족는 타레 피한다. 그러나 i] 저장되어 있는 HS 1 증가시키라는
의피인 i++ 같은 명령문은 간편하므로 사용한다.

Ore Bea =   J 연산자와 일 일부 관계 연산자 표기법이 생소하게 보일 수도 있다.
그 표기법은 다음과 같다.

비교       0++ 코드
연산자            0++ 심벌                      2=4               (a == y)
and                &&                              ay             (x!=y)
=                            (2 <y)         (2 <=y)
not                !                               r>y           (2 >=y)



===== PAGE 22 =====
@eeee@ @
11 알고리즘  7

이제 알고리즘의 실례를 좀 더 공부해보자. 첫째 알고리즘은 함수를 사용하는 예이다.
프로시저는 그 이름 앞에 4010라는 지정어667\070/를 쓰고, 함수는 내주는 값의 데이

. 함수가 내주는

터타입을 쓴

배열의 수 더하기

은 return#le 표현한다.

문제 : 수가 7개인 배열 So 있는 FS 모두 더하시오.
입력 : 정수 (> 0), 수의 배열 /9(인덱스의 범위는 1부터 7까지)

출력 : Sol] 있는 모든 수의 합

number sum (int 2, const number Sf ])
{

index /;

number result ;

result = 0;

for (7 = 1; 7 <= n; 4+)
result = result + S| i]

return result ;

»

이 책에서 여러 가지 정렬 알고리
리즘이다.

> 알고리즘 1.3     is}48(Exchange Sort)

리

STU, 다음은 크 중 제일 간단한 정렬 일

문제 : 비내림차순(ㅁ00ㅁ000『6088108 07094)으로 72개의 키를 정렬하시오.
입력 : 자연수 (> 0), 키의 배열 (인덱스의 범위는 1부터 까지)

출력 : 키가 비내림차순으로 정렬된 배열 s

void exchange (int 2, keytype 이 ])
{
index 2, /j;
for (¢ = 1; i <= n-1; H+)
for G = i+ 1; 7 <= m +4)
if (SL) < 의기)
exchange S[i] and S[/];

다음 명령문은 Sie SLI 값을 서로 바꾸라는 뜻이다.

exchange S{[i] and 912]


===== PAGE 23 =====
@0@000000
8      chapter ㅣ 알고리즘: 효율, 분석, 차수

이 명령문은 전혀 C++ 문장 같아 보이지 않는다. C++2] 문법을 지키지 않더라도 더 간
결하게 어떤 것을 표현할 수 있으면 그렇게 한다. 교환정렬은 :째 자리에 있는 수와 (1, +1)
A 자리부터 nA 자리에 있는 수들을 차례로 비교함으로써 작동한다. 주어진 자리의 수
가 i 자리에 있는 것보다 작은 경우 그 두 수를 교환한다. 이런 식으로 하면 0『-1
루프를 한 번 수행한 후 가장 작은 수가 첫째자리에 들어가고, 둘째 루프 이후에는 둘째
자리에 SAS 작은 수가 들어가고, 등등 이런 식으로 계속 반복한다.

다음 알고리즘은 VA (matrix) PIs 한다. 다음과 같은 두 개의 2×2 행렬이 있을 때,

011 912              011 |
A=               B=
ie ia ai       bs 022

그 H(product) C= AX BE 다음과 같이 계산한다.

Cig = 10177 02027

2,
00
mun
[요

: Ps: ‘| eae eee [38 3s]
4 1   68] |4x5+1x6 4X74+1x8   26 36

일반적으로 2개의 nxn 행렬 AS 2#가 있으면, 그 곱 CE 다음과 같이 구한다.
1<i,j<n@ BEi, 7에 대해서 <,= > 이
k=1

이 AIS 그대로 사용하여 행렬곱셈 알고리즘을 표현할 수 있다.

문제 : nxn YA 곱을 구하시오.
입력 : 정수 (> 0), 수의 :차원 배열 AM 2. 여기서 이 Belo] 행과 열은 모두 1부터
까지 인덱스를 붙인다.
출력 : 4 와 B 행렬의 곱이 표현된 차원 배열 C. 여기서 이 행렬의 행과 열은 모두 {부터
까지 인덱스를 붙인다.
void matrixmult (int n,
const number A[

I]
const number BI || |
I]

number C{

index i, j, k;

for (¢ = 1; 7 <= no; ++)


===== PAGE 24 =====
0000000
1.2 효율적인 알고리즘 개발의 중요성       9

a; k++)
7] + 지기[1 * BEANS);

@ 12 효율적인 알고리즘 개발의 중요성
앞에서 언급했듯이 컴퓨터의 실행 속도가 빨라지고 메모리의 가격이 싸지더라도 이에 상
                              관없이 알고리즘의 효율성은 언제나 중요하게 고려해야 한다. 같은 문제를 푸는 두 개의
                    알고리즘을 비교하여 그 이유를 탐구해보자.

1.2.1 순차검색 대 이분검색

순차검색보다 개선된 이분검색 방법을 사용하면 전화번호부에서 이름을 훨씬 빨리 찾을
수 있다. 이제 이 두 가지 방법을 비교하여 이분검색04081 search)] 얼마나 더 빠른지
측정해보자.

이미 알고리즘 1.1에서 순차검색을 하는 알고리즘을 공부한 바 있다. 비내림차순으로
정렬된 HAS 이분검색하는 알고리즘은 전화번호부를 앞뒤로 뒤적이는 것과 비슷하다.
즉, cB 찾고 싶은 경우 먼저 oS HA] 정중앙에 위치한 원소와 비교한다. 만약 같으
면, 찾았으므로 알고리즘을 끝낸다. 만약 <가 그 원소보다 작으면(=가 배열에 있는 경
우) 는 반드시 배열 전반부에 있을 것이므로, 배열 전반부에서 이분검색 절차를 되풀이
한다(즉, oS 배열 전반부의 정중앙에 위치한 원소와 비교한다. 만약 같으면, 찾았으므
로 알고리즘을 끝내고, 등등 이런 식으로 되풀이한다). 만약 x7} 배열의 중앙 원소보다
크면, 배열의 후반부에서 이분검색 절차를 되풀이한다. 이 절차를 eB 찾거나, 또는 27}
배열에 없음이 확실할 때까지 되풀이한다. 이 방법에 대한 알고리즘은 다음과 같다.

> 알고리즘 15

을

분검색

문제 : 원소가 개인 정렬된 배열 에서 원소 «cB 찾으시오.

입력 : 자연수 7, (비내림차순으로) 정렬된 배열 5(인덱스의 범위는 1부터 7까지), 원소 2
출력 : 10080402, 에서 2가 있는 위치(만약 가 So] 없으면 0)
void binsearch (int n,
const keytype 의],
keytype x,

index& Jocation)


===== PAGE 25 =====
10

chapter ㅣ 알고리즘: 효율,

A, 차수

A

index 700, high, mid;

low = 1; high = n;
location = 0;
while (low <= high && location == 0) {
mid = | (low + high)/2| ;
i (2 == 12201)
location = mid;
else if (x < S{mid\)
high = mid —1;

else

low = mid + 1;

순차검색과 이분검색 알고리즘이 실행한 작업의 양을 비교해보자. Zp 알고리즘이 A
행한 비교 횟수를 세어보자. 만약 배열 Sol] 32개의 원소가 있고 2가 배열에 없다면 알
고리즘 1.1(순차검색)은 32개의 ALS 모두 비교한 뒤에야 x7} 배열에 없다고 확신할
수 있다. 일반적으로 서술하면 순차검색은 크기가 nel 배열에서 비교를 nA 해야만 2
가 없음을 확신할 수 있다. 순차검색으로 크기가 nel MSS 검색할 때 이보다 많이 비교
해야 하는 BPE 절대 없다. 즉, 가 배열에 있는 경우에는 비교 횟수가 7보다 클 수
없다.

이제 알고리즘 1.5(이분검색)를 살펴보자. while 무프를 한 번 실행할 때마다 와 8
[2270)를 두 번씩 비교한다(를 찾은 경우는 한 번 비교). 이 알고리즘을 어셈블리언어로
구현하면 각 루프마다 cS Slmid|o} 한 번만 비교하고, 그 비교의 결과로 비교 코드를
설정하여 그 조건 코드의 값을 기준으로 하여 적절히 분기가 일어나도록 할 수 있다. 다
시 말하면, while 루프 한 번 실행에 와 .10ㅁ01는 한 번만 비교해도 된다는 것이다.
따라서 루프 한 번 실행할 때마다 비교를 한 번한다고 가정한다. 이런 가정 하에서 크기
가 329) 배열에 있는 모든 원소보다 27} 크면 이 알고리즘은 비교를 6번 한다(그림 1.1
참조). 여기서 6=18 82 +1임을 주목하자. 여기서 "18 는 log. S 의미한다. log. = 알고리
즘 분석에 꽤 자주 나오기 때문에 특수 심벌 18로 표시한다. 이 횟수는 이분검색 알고리
즘의 최대 비교 횟수이다. 즉, #가 배열에 있는지, 가 배열의 모든 원소보다 작는지,
어떤 상황에도 이보다 더 많이 비교하지 않는다.

S[16]                    [24]        [28] S[30] S[31] S[32]
4                         f            f *& ff
4st                                                      200                       gird 44 54 64

그림 1.1 <가 크기 32인 배열의 모든 원소보다 클 때, 이분검색에서 *와 비교하는 원소들


===== PAGE 26 =====
000600000
개발의 중요성  11

@ Hii x7} 배열의 모든 원소보다 클 때 순차검색과 이분검색에서의 비교 횟수

배열의 크기            순차검색 비교 횟수         이분검색 비교 횟수
128                      128                       8
1,024                    1,024                      ial
1,048,576                 1,048,576                      21
4,294,967,296             4,294,967,296                      33

가령 배열의 크기를 두 배로 늘여 64가 되어도, 이분검색은 추가적으로 한 번 더 비교
할 뿐이다. 왜냐하면 처음 한 번 비교하고 배열을 반으로 자르므로, 검색할 배열의 크기
가 327} 되기 때문이다. 그러므로 가 크기 64인 배열의 모든 원소보다 클 때 이분검색
은 비교를 ?번 한다. 여기서 7=16 64+1임을 주목하자. 일반적으로 배열의 크기를 두
배로 늘릴 때마다 한 번의 비교만 더하면 된다. 그러므로 ne] 29] 거듭제곱이고 가 크
기 인 배열의 모든 원소보다 크면, 이분검색에 의한 비교 횟수는 1g n+ 1이다.

표 1.1에서 2가 배열의 모든 원소보다 클 때, 여러 //값에 대해서 순차검색과 이분검색
에서 수행한 비교 횟수를 비교해 놓았다. 배열에 40억 개의 원소가 있으면(이 수는 전
세계의 총인구와 비슷하다), 이분검색은 비교를 기껏해야 38번하는데 비해서 순차검색
은 40억 개의 모든 QA} 비교해야 한다. 비록 컴퓨터가 01116 루프를 한 번 수행하는
데 40억분의 1초밖에 걸리지 않는다고 해도 순차검색은 x7} 배열에 없다는 걸 아는데
4초가 걸리는 반면, 이분검색으로는 바로 알 수 있다. 이 차이는 온라인 앰이라든지 대량
의 데이터를 검색해야 하는 경우 아주 치명적일 수 있다.

지금까지 이분검색을 다루면서 편의상 크기가 29) 거듭제곱인 배열만 고려하였다. 2
장에서 분할정복법을 공부할 때 다시 이분검색을 다루게 된다. 거기서 이 제한을 풀고
모든 크기의 배열에 대해서 생각해 보기로 한다.

검색하는 문제의 예로만 봐서는 향상된 알고리즘을 설계한다는 doy 대한 중요성이
크게 부각되지 않을지도 모르겠다. 왜냐하면 순차검색을 사용하더라도 우리가 기다릴 수
있을 만한 시간 안에 임무를 완수하기 때문이다. 다음에는 우리가 기다릴 수 있을 만한
시간 안에 임무를 마치지 못하는 좋지 않은 알고리즘에 대해서 살펴보기로 하자.

1.2.2 피보나치 수열
피보나치 수열을 계산하는 알고리즘을 공부해보자. 피보나치 수열의 7번째 수는 다음과
같이 AAZ(recursively: AAS 되부르는 꼴로) 정의한다.

000

/.-

fe fama fag OR! 경우)


===== PAGE 27 =====
@0@00000 0
chapter ㅣ 알고리즘: SS 분석, 차수

12

> 알고리즘 1.6

int fib (int 7)

{

처음 몇 개를 계산하면 다음과 같다.
| eee Ce tee 1 ‘dee!
fg= ht Piri =!
/4- faerie Srl=s
fo=Sfatfs =3+2=5 SS

컴퓨터과학과 수학에서 피보나치 수열은 널리 쓴다. 이 피보나치 수열은 재귀로 정의하
기 때문에 정의를 그대로 재귀 알고리즘으로 바꿀 수 있다.

/번째 피보나치 수 구하기(재귀)

문제 : 피보나치 수열에서 번째 수를 구하시오.
입력 : 양수 n(0 포함)

출력 : fib, 피보나찌 수열에서 7번째 항

if (기소 10
return 7;

else

return fb(n—1) + fib(n- 2);

알고리즘의 입력을 “OS 포함한 양수"로 명시하여 이 알고리즘이 음수를 취할 수 없음

6     .       알고리즘이 불필요하게 복잡해지는 걸 피하기 위해서 알고리즘
내부에서는 n& 그냥 QPS 표시하였으니 주의하기 바란다. 앞으로 이 책에서는 계속
이 관례를 따르기로 한다.

이 알고리즘은 간단하여 작성하기도 이해하기도 쉽지만, 불행하게도 아주 비효율적이
다(느리다). 알고리즘으로 fib(5)S 계산하는 과정은 그림 1,22] AAU HA (recursion
tree)S 보고 이해할 수 있다. 이 나무구조를 보면 모든 자식마디에서 재귀 SSS 한다.
예를 들면, 맨 위에서 fid5)S 얻기 위해서 fid(4)ot 7?0(3)을 호출하고, lad    ;
위해서 fib(2)2} fibd)S 호출하고 SS 이런 식이다. 이 트리에서 본대로 이 함수는
은 AALS 중복하여 호출하기 때문에 비효율적이다(느리다). 예제에서 /*0(2)를 3번 Pe
계산한다.

그러면 이 알고리즘이 얼마나 느릴까? 그림 1.2의 나무구조를 보면, 이 알고리즘은 0
<n<69 때 /80(002)을 얻기 위해서 계산하는 항의 개수가 다음과 같다.



===== PAGE 28 =====
그림 1.2 om 피보나찌 SS 계산하는 알고리즘 1.6의 재귀 SSS 보여주는 나무구조

n            계산하는 항의 개수
0                         1
1                         1
2                         3
3                         5
4                         9
5                       15
6                       25

처음 6개의 값은 1 = 7 = 5인 Z no] 대해서 fid(n)-S 뿌리로 하는 하위 나무구조의
마디 개수를 세어서 구할 수 있다. 그리고 fid(6)-S 계산하는데 필요한 항의 개수는 sid
(5)2} /10(4:를 뿌리로 하는 하위 나무구조의 마디 개수의 합에다 하나를 더하면 된다.
이분검색의 경우와는 달리 바로 AS 얻기는 어려울지 모르지만, 위에서 구한 처음 ?개
의 값을 보면 no] 3 증가할 때 나무구조의 항의 개수는 배 이상으로 증가한다. 예를 들
면, 7 =4이면 항의 개수는 9인데, ㅠ=6이면 257} 된다. T(n)-S nel] 대한 재귀 나무구
조의 항의 개수라고 하자. no] 8 증가할 때마다 항의 개수가 배로 늘어난다면, 다음과
같이 nol] 대해서 22] 거듭제곱으로 나타나게 된다.


===== PAGE 29 =====
14

chapter 1 알고

매

T(n) > 2× T(n-2)
>2x2x T(n—-4)
>2x2x2x T(n-6)

>2x2x2x---x2x T(0)
7/2번

T(0) =1이므로, T(n) > 2"/?7} 된다. 귀납법140401020)을 사용하여 no] 2°) 거듭제
곱이 아니더라도 n > 8인 모든 nol] 대해서 이가 사실임을 증명할 수 있다. 이 부등식은
no] 1일 때 성립하지 않는다. 왜냐하면 7(1) = 1인데 이는 2'“*보다 작기 때문이다. 귀
납법에 대해서 더 자세히 알고 싶으면 부록 AS] ㅅ.8을 참고하자.

> 정리 1.1

알고리즘 1.6의 재귀 나무구조에서 항의 개수를 717/)이라고 하면, 7 > 3인 모든 no} 대해서
다음이 성립한다.

T(n) > 2"?

증명 : no] 대한 귀납법으로 증명한다.
귀납기초 : 귀납절차 단계에서 2개의 이전 결과를 가정하므로 2개의 귀납기초가 필요하다.
”=?3이고 27=3일 때 그림 1,29] 재귀나무구조를 보면 다음과 같은 결론을 얻을 수 있다.

T(2) =3>2=2??

T(3) =5 > 2.8323 > 23/
귀납가정 : 보다 작은 모든 mol] 대해서 이 정리가 사실이라고 가정하고, nol] 대해서도 사실
이라는 것을 귀납절차에서 보이면 된다. 2<m<no] 되는 모든 mo] 대해서 다음을 사실이
라고 가정한다.

T(m) > 2702
귀납절차 : T(n) > 2°? 7; 사실임을 보여야 한다. T(n)-2 T(n-1) Ft T(n—2) 2] 합에다 하
나를 더한 값이 된다. 그러므로
T(n) = 2(2-1)+27(2-2)0+1
> gln-D/2 4 9(n—2)/2 44              (귀납가정에 의해서)

kil
2

느 9(n-2)/2 4 gin—2)/2 Spal  jn = nl?

7번째 피보나찌 수를 구하기 위해서 알고리즘 1.6으로 계산된 항의 개수는 2"'”보다
크다는 사실을 입증하였다. 이 알고리즘이 얼마나 느린지는 잠시 뒤에 알아보고, 우선
번째 피보나찌 수를 구하는 효율적인(빠른) 알고리즘부터 먼저 작성해보자. 재귀 알고


===== PAGE 30 =====
0000000
1.2 효율적인 알고리즘 개발의 중요성      15

리즘의 문제점은 같은 값을 중복해서 계산하는 것임을 상기하자. 그림 1.8에서 볼 수 있
듯이 72065) 계산하기 위해 /70(2)를 3H 중복 계산하였다. 만일 값을 처음 계산하고 그

을 배열에 저장해두고 나중에 필요할 때마다 쓰면 중복 계산을 피할 수 있다. 다음 반
복 알고리즘은 이 전략을 사용한다.

> 알고리즘 1.7     /번째 피보나찌 St 구하기(반복)

문제 : 피보나찌 수열에서 7번째 항을 구하시오.
입력 : 양수 7(0포함)
출력 : fib2, 피보나찌 수열에서 7번째 항

int 202 (int 22)

{

index /;
int f[0,.n];

지미 = 이
if (n > 0) {
Att) 크나
for (¢ = 2; 7 <= n; H+)
f(a] = £[f-1) 제 이:
}

return f[z];

를 사용하지 않고도 작성할 수 있다. 그 이유는 매번 aS
필요하기 때문이다. 그러나 배열을 사용하면 알고리즘을

사실 알고리즘 LTS 배열 /
때마다 가장 최근 2742] 항만
더 명확히 표현할 수 있다.
fib2(n)& 구하기 위하여 처음 나오는 7+1개의 항을 각각 한 번씩 계산한다. 즉,
번째 피보나찌 항을 구하기 위해서 7+1개의 BS 계산한다. 알고리즘 1.6으로는 nH
째 피보나찌 항을 구하는데 2"개의 항 이상을 계산해야 했음을 주목하자. 표 1.8에는
여러 7 값에 대해서 이 두 식을 비교해 보았다. 여기서 실행시간은 한 개의 항을 계산하
는데 어림잡아 10 “초가 걸린다고 가정하고 계산하였다. 이 HE 한 개의 항을 계산하는
데 1억 분의 1초가 걸리는 가상 컴퓨터를 가지고 알고리즘 1.7로 7번째 BS 계산하는데
걸리는 시간을 보여주고, 알고리즘 1.0으로 실행하는데 걸리는 시간의 하한을 보여준다.
n°] 80°] 되면 알고리즘 1.6으로는 최소한 18분이 걸린다. no] 120일 때는 36년 이상이
걸리는  ~  그렇게 오래 기다릴 만큼 참을성이 있는 사람은 현실적으로 없다. 비록 10억
배 빠른 컴퓨터를 개발한다 해도 알고리즘 1.6으로 200번째 항을 계산하는데 40,000년
의싱이 걸린다 이 결과는 200번째 항을 계산하는데 걸리는 시간을 10억으로 나누어서


===== PAGE 31 =====
16     chapter ㅣ 알고리즘: 효율, 분석, 차수

A

@ 표 1.2 알고리즘 1.67} 1.7의 비교

알고리즘 1.7을       알고리즘 1.6을
n            071               002             사용히 Ke 경  경우        사용하는 경  경우
실행시간            실행시간의 하한
40                 41             1,048,576                     41 ns*                   1048 ps!
60                 61             1,1 10°                       61 ns                        18
80                      81                  11108                             81708                             18 min
100                   101                1 12108                           101 ns                        13 days
120                  121               12108"                         121 ns                      36 years
160                161              1,210"                       161 ns                3.8 X10’ years
200                201              1,310”                      201 ns                4X10" years

*Ins = 10° second,
tls = 10° second,

얻을 수 있다. 아무리 컴퓨터가 빨라진다 하더라도, 알고리즘 1.6으로는 no] 작은 APS
제외하고 기다릴 수 없는 만큼의 시간이 걸린다는 AMIS 알았다. 반면에 알고리즘 1.7은
번째 피보나찌 항을 거의 즉석에서 계산한다. 컴퓨터의 계산속도가 빨라지는 것과는
무관하게 알고리즘의 효율성이 A 중요한 고려사항인지를 이 비교를 통해서 명확히 알
수 있다.

알고리즘 1.6은 분할정복 알고리즘ㅇ ie  분할정복 해결방법으로 정렬된 배열을 검색
하는 문제를 푸는 매우 빠른 알고리즘을 공부했다(알고리즘 1.5: 이분검색). 2장에서 공
부하겠지만 분할정복 해결방법은 어떤 부류의 문제에 대해서는 매우 효율적인 알고리즘

을 이끌어 내지만 매우 비효율적인 알고리즘이 만들어지는 BPE 있다. 7 번째 피보나찌
항을 계산하는 효율적인 알고리즘(알고리즘 1.7)은 동적계획법의 전형적인 사례로서 3장
에서 다룬다. 그중 가장 좋은 방법을 선택하는 것은 매우 중요하다.

알고리즘 1.6은 지수적으로(6000600811) 많은 개수의 항을 계산한다. 그러나 이보다
더 ats 수 있을까? 답은   pvt 부록 Bol 있는 기술을 가지고 계산에 필요한 항의
ASS 정확하게 나타내는 식을 유도할 수 있는데, 그 식은 n 2] 지수로 나타난다. 피보나
찌 수열에 대해서 더 자세히 ea 싶으면 부록 8의 예제 B52} BIS 공부하기 바란다.

개

ial

@ 13 알고리즘의 분석

AAR 알고리즘으로 문제를 얼마나 효율적으로 풀 수 있는지 알아보려면 알고리즘을 분
석해야 한다. 앞절에서 알고리즘들을 비교하면서 알고리즘의 효율성 분석을 해보았지만
분석은 다소 약식으로 이루어졌다. 이 절에서는 알고리즘 분석에 사용하는 용어와 표준
분석방법에 대해서 제대로 공부해보자. 이 책 전체에서 사용하므로 반드시 이해하고 넘
어가야 한다.



===== PAGE 32 =====
1.3.1 시간복잡도 분석

시간을 기준으로 알고리즘의 효율성을 분석할 때, #0에서의 실제 작동시간을 재지 않
는다. 왜냐하면 알고리즘을 수행하는 특정 컴퓨터에 따라서 결과가 달라질 수 있기 때문
이다. 실행하는 명령문의 개수를 세지도 않는다. 왜냐하면 알고리즘을 구현하는 프로그

래밍 언어에 따라서, 그리고 프로그래머가 프로그램을 작성하는 방식에 따라서 명령문의
개수가 달라질 수 있기 때문이다. 따라서 컴퓨터, 프로그래밍언어, 프로그래머뿐만 아니
라 루프 색인의 증가, 포인터의 세팅 등과 같은 모든 알고리즘 상의 복잡한 세부사항과는
독립적인 측정법이 필요하다. 알고리즘 1.5가 알고리즘 1.1보다 훨씬 효율적이라는 사실
은 no] 배열 원소의 개수일 때, 몇몇 7 HS 선택하여 그 값으로 두 알고리즘을 실행할
때 비교 횟수의 차이를 보고 알았다. 알고리즘 BAS 거의 이런 방식으로 한다. 일반적
으로 알고리즘의 실행시간은 입력의 크기가 커지면 증가하고, 총 실행시간은 (비교 같은)
단위연산이 몇 번 수행되는가에 거의 비례한다. 따라서 단위연산이 수행되는 횟수를 입
력의 크기에 대한 함수로 구하여 알고리즘의 효율성을 분석한다.

보통 알고리즘의 YAS7|(input 8120)를 재기는 쉽다. AS 들면, 앞에서 공부한 알고
리즘 1.1(순차검색), 1.9(배열의 수 더하기), 1.3(교환정렬), 1.5(이분검색)를 다시 살펴보
자. 이들 알고리즘에서 배열 원소의 개수 no] 입력크기를 나타내는 간단한 척도가 된다.
그러므로 을 입력크기라고 할 수 있다. 알고리즘 1.4 (행렬곱셈)에서는 행과 열의 개수
n°] 입력크기를 나타내는 척도가 된다. 그러므로 이 경우도 ns 입력크기라고 할 수 있
다. 알고리즘에 따라서 입력크기를 측정할 때 2개의 수를 사용하는 편이 더 적절한 경우
도 있다. AS 들어, 알고리즘의 입력이 그래프이면 마디(7660)와 이음선(6089)의 개수
형식으로 입력을 Ach 따라서 이 경우 두 파라미터(6888066[00)가 모두 입력크기이다.

파라미터를 무조건 입력크기로 볼 수 있는 것은 아니니 주의해야 한다. 예를 들면, 알
고리즘 1.607번째 피보나찌 항 구하기, 재귀)과 1.70번째 피보나찌 항 구하기, 반복)에
서 입력크기가 7,이어야 한다고 생각할지도 모른다. 그러나 /은 입력이지, 입력크기는
아니다. 이 알고리즘에서 적절한 입력크기는 /을 부호화(620008)한 7|Z(symbol) 2] 개수
로 잡는다. 이진표기법0610877” representation) S 쓰는 경우, 입력크기는 nF 부호화하면
차지하는 비트0640)의 개수 | Ign | +1이다. 예를 들어, 다음에서 = 13을 이진수로
바꾸면 다음과 같이 4비트만큼 자리를 차지한다.

n= 18 = 1101,
46166

따라서 입력 n= 13의 크기는 4가 된다. 각 알고리즘이 계산하는 항의 개수를 nO] 함수
로 구하여 두 알고리즘의 효율성 차이를 알 수 있었지만, no] 항상 입력크기를 나타내
주는 것은 아니다. 9장에서 공부할 내용에서는 입력크기가 중요하므로 그때 가서 입력크
기에 대해서 더 자세히 공부할 것이다. 그때까지는 간단하게 구할 수 있는 수치, 즉 배열


===== PAGE 33 =====
@0@00000 0
18     chapter ㅣ 알고리즘: 효율, 분석, 차수

안에 있는 원소의 개수를 입력크기로 사용해도 별 문제없다.
~ 구한 후, 어떤 명령문이나 명령문 VIE 선정하여 알고리즘이 실행

덩어리(군)를 실행한 횟수에 대략적으로 비례하
ES 완다. 이 '명령문이나 명령문 군을 알고리즘의 단위연산(68610 1086ㅠ40000)이라고
한다. 예로 알고리즘 1.1과 1.5는 루프를 한 번 수행할 때마다 cS 의 원소와 비교한다.

그러므로 비교문을 단위연산으로 정했다. 결국 Zn 값에 대해서 알고리즘 1.1과 1.5가
몇 번 수행하는지 구하여 두 이 효율성 차이를 알아냈다.

일반적으로 알고리즘의 시간복잡도 분석(12706 complexity 80ㅁ817818)은 입력크기를 기

산을 몇 번 수행하는지 구하는 것이다. 알고리즘 구현 방식의 세부사항은

고려하지 않지만 단위연산은 최대한 효율적으로 구현한다고 가정하고 분석해도 무방하

다. 예를 들어, 알고리즘 1.5에서 비교를 한 번만 한다고 가정해도 분석 결과에 차이가

및
oS eee 주검  ies ㅣ 않는다. 때로는 루프의 한 번 ABS 단위연산의 한 번 실행
명

으로 취급하면 충분한 경우도 있다. 또는 분석을 아주 세밀히 하기 위해서 기계적 명령문
각각의 실행을 하나의 단위연산으로 취급하는 극단적인 경우도 있다. 앞에서 말했듯이
컴퓨터와는 독립적으로 분석해야 하기 때문에 이 책에서는 그런 극단적인 방법은 쓰지
않는다.

때로는 두 개의 다른 단위연산을 고려해야 하는 경우도 있다. 예를 들어, 키를 비교하
여 정렬하는 알고리즘에서 비교문과 지정문(6881800606 statement) S 개별 단위연산으
로 취급해야 할 때도 있다. 이 두 가지 명령문을 합쳐서 하나의 단위연산으로 합한다는
뜻이 아니라, 두 가지의 개별 단위연산이 있다는 뜻이다. 그 중 하나는 비교문이고, 다른
하나는 지정문인 것이다. 이렇게 하는 이유는 정렬 알고리즘에서 비교하는 횟수와 지정
하는 횟수가 같지 않기 때문이다. 그러므로 각 단위연산이 실행되는 횟수를 따로 알아봄
으로써 알고리즘의 효율성을 더 세밀하게 파악할 수 있다.

알고리즘의 시간복잡도 분석은 입력크기를 기준으로 단위연산을 몇 번 실행하는지 구
하는 것이다. 어떤 경우에는 실행 횟수가 입력크기에 좌우될 뿐 아니라 입력의 값에도
좌우된다. 알고리즘 1.1(순차검색)의 경우 2가 배열의 첫 번째 원소이면 단위연산은 한
번 실행하지만, 가 배열에 없다면 nw 실행한다. 그러나 알고리즘 1.2(배열의 수 더하
기)의 경우 입력의 값에 상관없이 항상 단위연산의 실행 횟수가 일정하다. 실행 횟수가
일정한 경우 T(n)S 입력크기 7에 대해서 알고리즘이 단위연산을 실행하는 횟수로 정
의한다. 여기서 T(n)S 알고리즘의 일정 시간복잡도(60677-0886 time complexity) e}a1
하고, T(n)& 구하는 과정을 일정 시간복잡도 분석이라고 한다. 다음은 일정 시간복잡도


===== PAGE 34 =====
ae

13 알고리즘의 분석    19
분석의 실례이다.
『(배열의 원소 모두 더하기)의 일정 시간복잡도 분석
제어에 필요한 명령문을 제외하고 루프 안에 있는 유일한 명령문은 배열의 MAS sumo]

더하는 BRB, 따라서 이 awe 단위연산으로 정한다.

단위연산 : 배열의 원소를 507에 더함

입력크기 : 배열 원소의 개수, n

배열에 있는 원소의 값에 상관없이 for 루프를 7번 실행한다. 그러므로 단위연산을 항상
nel 실행하여 시간복잡도는 다음과 같다.

Tin) =7

(교환정렬)의 일정 시간복잡도 분석

앞에서 설명했듯이 키를 비교하여 정렬하는 알고리즘의 경우, 비교문이나 지정문을 단위
연산으로 정할 수   _ 여기서는 비교 횟수를 단위연산으로 정하고 분석해보자.
단위연산 : 9[7]와 sli] 2] 비교

입력크기     비비    소의 개수, 7

for—j FES 몇 번 실행하는지 세어야 한다. 주어진 nol] 대해서 for—i 루프를 실행하는
횟수는 항상 n— 1이다. 첫째 fori 루프를 실행할 때 for-j 루프를 실행하는 횟수는
- 1이고, 둘째 0「-1 루프를 실행할 때 for—j 루프를 실행하는 RHE 7- 2이고, 세
째 for-i 루프를 실행할 때 for-j 루프를 ae 횟수는 n— 30], ..., 마지막 For-i
루프를 실행할 때 for—j 루프를 실행하는 횟수는 1이다. 따라서 for—j 루프를 실행하는
총 횟수는 다음과 같이 계산한다.

iO,

3

(n—-1)n
2

마지막 등식이 어떻게 성립하는지 이해가 가지 않으면 부록 ao} 예제 Ars 공부하자.

T(n) = (02-1)+(02-2)+(02-3)+…+1=

가장 안쪽 for 루프에 있는 유일한 명령문은 곱셈과 덧셈을 하는 명령문이다. 곱셈을 덧셈
보다 더 많이 하도록 구현할 수 있으므로, 곱셈하는 명령문만을 단위연산으로 취급한다

단위연산 : 가장 안쪽 for 루프에 있는 곱셈
입력크기 : 행과 열의 개수, n

for-i BEL 항상 /번 실행하고, 0『- 루프가 한 번 실행할 때마다 70『-7 루프는 항


===== PAGE 35 =====
00000 0 0
20

chapter

v

스

1 알고리즘: 효율 분석, 차수

At

ox

} nH 실행하고, for—j 루프가 한 번 실행할 때마다 for-k 루프는 항상 nv 실행한다.
위연산은 for-k 루프 안에 있으므로, 단위연산을 실행하는 횟수는 다음과 같다.

c

T(n)=nXnXn=n3

앞에서 설명했듯이 알고리즘 112 크기 nel 사례에 대해서 단위연산을 실행하는 횟수
가 모두 같지 않다. 따라서 이 알고리즘의 경우 일정 시간복잡도로 분석결과를 측정할
수 없다. 그렇다고 분석을 포기할 SE 없다. 왜냐하면 사실 대부분의 알고리즘이 이런
경우에 해당하기 때문이다. 따라서 시도할 수 있는 다른 계측방식이 세 가지 더 있다.
Al 번째 방법은 단위연산을 수행하는 최대 횟수를 측정한다. W(n)S 입력크기 7에 대
해서 알고리즘이 실행할 단위연산의 최대 횟수로 정의한다. 그러면 W(n)S 알고리즘의
최악 시간복잡도(ㅠ08[-0886 time 0020ㅁ216119)라 하고, W(n)-& 구하는 과정을 최악 시
간복잡도 분석이라고 한다. 만약 7'01)이 존재하면 당연히 W(n) = 7'01)이 된다. 다음
은 T(n)°| 존재하지 않는 경우 Wn) S 분석하는 예이다.

(순차검색)의 최악 시간복잡도 분석

단위연산 : 배열 원소와 2와의 비교

입력크기 : 배열 원소의 개수, n

x7 HSS] 마지막 원소이거나 2가 배열에 없는 경우 단위연산을 7번 실행하고, 이 경우
가 단위연산을 가장 많이 실행하는 경우이다. 따라서 시간복잡도는 다음과 같다.

r.

비록 최악의 경우 BA Os 사용한 최대 시간을 S 수 있지만, 어떤 경우에는
이 평균적으로 얼마나 실행하는지 측정하면 더 일리가 있는 BPE 있다. 어떤 알고리
에 대해서, A(n)& 입력크기 7에 대해서 그 알고리즘이 수행할 단위연산의 평균 횟
(기대치)로 정의한다(평균의 개념에 관해서는 부록 AS] 4.8.2절을 참조하라). 그러
A(n)& 알고리즘의 평균 시간복잡도(2760880-0896 time 0020ㅁ01619)라 하고, 4 (00)
구하는 과정을 평균 시간복잡도 분석이라고 한다. W(n) 2] 경우에서와 같이 만약 T(n
이 존재하면 A(n) = T(n)°] 된다.

A(n)-& 계산하려면 7개의 입력에 확률을 각각 부여해야 한다. 가용한 정보를 모두
동원하여 HSS 부여하는 것이 중요하다. 예를 들어, 알고리즘 1.1의 평균 시간복잡도
BAS 해보자. 27} 배열 안에 있고, 이중 어디에 위치할 확률은 똑같다고 가정하자. x
가 배열의 어딘가 있다는 사실만 안다고 하면, 배열의 어떤 특정 위치를 다른 위치에 비
해서 차별을 둘 하등의 이유가 없다. 따라서 원소의 위치가 어디든 같은 SHS 부여하는

lo po 4> oy aly

wa


===== PAGE 36 =====
게 타당하다. 각 원소를 검색하는 횟수가 동일하면 평균을 구하면 된다는 뜻이다. 그러나
검색 횟수가 동일하지 않다면, 같은 확률을 부여하면 타당하지 않다. 예를 들어, 국민 모
두의 이름을 저장한 배열에서 무작위로 선택한 이름을 찾는다면, “희국"과 같은 흔하지
않은 이름보다 "정선"과 같이 비교적 흔한 이름을 아마 더 자주 YA 것이다(무작위의
개념에 관해서는 부록 AS) 4.8.1절을 참조하라). 검색 빈도가 다른 경우를 절대 무시할
수는 없지만, 여기서 배열 원소의 검색 빈도는 모두 같다고 가정한다.

음 분석에서 볼 수 있듯이 최악의 경우 분석보다 평균의 경우 분석이 보통 더 어

다.

rt,

『(순차검색)의 평균 시간복잡도 분석

단위연산 : 배열 원소와 와의 비교

입력크기 : 배열 원소의 개수, n

7} SH 있는지 아는 BPS 먼저 분석해보자. 여기서 So] 있는 원소는 모두 다르고, x7}
어떤 특정위치에 있을 확률이 다른 위치에 있을 확률보다 높다고 믿을 이유가 전혀 없다고
가정한다. 이 정보에 의하면 1 < 《 < 인 모든 《에 대해서 2가 배열의 《번째에 위치할
확률은 1/7,이다. 만약 2가 《번째에 위치한다면, oS 찾는데(즉, 루프를 빠져나가는데)
단위연산의 실행 횟수는 《이다. 따라서 평균 시간복잡도는 다음과 같이 구할 수 있다.

r.

A(n)= Sox 4}- +x Dike +x aed) = ~
세 번째 등식이 어떻게 성립하는 지 부록 A] 예제 ㅅ.1을 참조한다. 기대하던 대로 평균적
으로 배열의 반 정도를 검색함을 알 수 있다.

다음으로 27} 배열에 없는 BLS 분석해보자. 이 BOS 분석하기 위해서 2가 배열에
있을 확률 pS 부여해야 한다. 미리 만약 x 7} 배열에 있다면 1부터 7사이의 어느 위치에
있을 확률도 같다고 가정한다. 그러면 x7} 《번째에 위치할 확률은 2/7이고, x7} 배열에
없을 확률은 1- /이다. oS ^번째 위치에서 찾는 경우 루프를 nw 실행하고, <가 배열
에 없을 때 루프를 nel 실행한다. 따라서 평균 시간복잡도는 다음과 같이 구할 수 있다.

n

A(n) = 기쿠 2) + nlp)

=F
n(n+1)
2

~

+n(1=p)=nf1-2}+2

£y
n

위 식에서 마지막 등식은 대수학으로 간략화하면 얻을 수 있다. 만약 p= 1이면, 위에서와
같이 A(n) = (n+1)/291 반면, p= 1/20] A(n) = 30/4+ 1/4이다. 이는 평균적으

로 배열의 3/4 가량이 검색된다는 뜻이다.



===== PAGE 37 =====
@0@0 0 0 @
22    chapter

@ @
1 알고리

Oy

Al, 치수

A

S
=,

진도를 더 나가기 전에 Batol] 대해서 주의할 BS 하나 이야기하도록 한다. 비록 평균
이라는 말이 전형성을 나타내는 좋은 척도이긴 하지만, 평균이라는 BS 잘못 해석하지
않도록 주의해야 한다. 예를 들어, 기상학자는 지난 80년 동안 1월 15일 서울의 평균 최고
기온이 영하 8도이기 때문에 1월 15일 ASQ] 최고기온이 일반적으로 영하 3도라고 말할
수 있다. 서울 강남의 가구 당 연간 평균 소득이 5,000만원이기 때문에 서울 강남의 가구
당 연간 ASO] 일반적으로 5,000만원이라고 신문기사에 나올 수도 있다. 실제 값이 평
균에 크게 벗어나지 않는 AMS, 표준편차가 작은 경우)만 평균을 “일반적이다"라고 말
할 수 있다. 1월 15일 최고 기온의 경우 아마도 그렇게 말해도 통할 수 있을는지 모른다.
그러나 서울 강남의 경우 부유한 사함이 사는 동네와 가난한 사람이 사는 동네가 공존하
고 있다. 따라서 연 평균소득이 2.000만원 또는 1억 원이라고 말하기가 연평균소득이
5,000만원이라고 말하기보다 더 일반적인 ayo] 될 수 있다. 2가 배열에 있다고 가정하
고 A(n) = (n+1)/22}51 계산했지만, 이 결과는 일반적으로 받아들일 수 없다. 왜냐하
면 일반적으로 1에서 7 사이의 어떤 수를 검색할 지 확률적으로 동일하기 때문이다. 이
고려사항은 반응시간을 취급하는 알고리즘의 경우 중요하다. 예를 들어 핵발전소를 감시
하는 시스템을 생각해보자. 비록 반응시간이 나쁜 사례가 한 번 있었다 하더라도 결과는
치명적이다. 따라서 모든 반응시간이 거의 3초 부근이기 때문에 평균 반응시간이 3초인
A], 아니면 거의 대부분 반응시간이 1초이지만 몇몇 경우 60초이기 때문에 평균 반응시
간이 8초인지 알아두는 건 중요하다.

마지막 형태의 시간복잡도 BAS 단위연산을 실행하는 최소 횟수를 구하는 것이다.
어떤 알고리즘에 대해서, Bln) S 입력크기 7에 대해서 그 알고리즘이 실행할 단위연산
의 최소 횟수로 정의한다. 그러면 B(n)S 알고리즘의 최선 시간복잡도(6686-0886 time
complexity analysis)@} 하고, B(n)-& 구하는 과정을 최선 시간복잡도 분석이라고 한다.
W(n) 2} A(n) 2] 경우와 같이 만약 T(n)°] 존재하면, Bln) = 710)이 된다. 알고리즘
1.1에서 B(n)& 구해보자.

(순차검색)의 최선 시간복잡도 분석

단위연산 : 배열 원소와 2와의 비교
연 으

일정 시간복잡도를 구할 수 없는 알고리즘에 대하여 최선의 경우 분석보다는 최악의
경우나 평균의 경우 분석을 훨씬 더 자주 채택한다. 평균의 경우 분석은 다른 입력을 여


===== PAGE 38 =====
© 예제 1.6

0000000
1.3 알고리즘의 분석  23

Iz

러 번 사용할 때 알고리즘을 실행하는데 평균적으로 걸리는 시간을 알려주기 aioe
용하게 많이 쓴다. 예를 들어, 가능한 모든 조합으로 WE 입력을 모두 정렬하는 경
속도를 재는 좋은 척도가 될 a 있다. 속도가 느린 정렬 알고리즘이라도 평균적으로 시간
이 좋게 나오는 경우 때로는 쓸 만하기도 하다. 2.4절에서 살펴볼 BEY a (quicksort)°]
라고 하는 알고리즘이 바로 그런데, 가장 널리 쓰여지고 있다. 앞에서 잠깐 이야기했듯이
평균의 경우 분석은 핵발전소 감시시스템 같은 경우 적합하지 않다. 이 경우에는 최악의
경우 분석이 더 유용한데, 그 이유는 알고리즘이 걸리는 시간의 상한 값을 알려주기 때문
이다. 방금 살펴본 두 가지의 ABO] 최선의 경우 BAS 해볼 가치가 전혀 없다.
지금까지 알고리즘의 시간복잡도의 분석에 대해서만 다루었다. 고려해보았던 사항들
이 메모리(공간)복잡도(26007 complexity) 2] 분석(알고리즘이 메모리 irs 얼
마나 효율적인지를 분석)에도 모두 그대로 적용할 수 있다. 이 책에서는 거의 대부분 시
간복잡도 분석에 치중하겠지만, 필요한 경우 메모리복잡도 분석도 다룰 리타
일반적으로, 복잡도 함수(600ㅁ21606 function)= 양의 정수에서 양의 ASO 포함)로
매핑하는 함수이다. 어떤 특정 알고리즘의 시간복잡도나 메모리복잡도를 가리키지 않을
때는 복잡도 함수를 보통 7(7)과 gin) 같은 표준 함수 표기법으로 표현한다.

다음은 모두 복잡도 함수의 예이다.

~

n

ll

Ss

(n)=n
(n) =n?
(n)   lg
(

n)

Ss

3n? +4n

f
위의 복잡도 함수는 모두 양의 정수에서 양의 실수(0 포함)로 매핑한다.

분                         산, 주변 명령문, 제어 명령문을 실행하는데 실
제로 걸리는 시간들을 고려해야 할 수도 있다. “주변 명령문(606041680 instructions)”o] et
루프 이전에 실행되는 초기화 문 같은 명령문을 말한다. 이 명령문을 실행하는 횟수는
일반적으로 입력크기에 상관없이 항상 일정하다. “제어 명령문(60001 instructions)”©]

ne,
ky
aus
ON
i
Lr
oS
ro J
lo nl
iy
ofp
Ot
[묘
주
ro
oe
re

일보
란 루프를 제어하기 위한 인덱스 증가 명령문 같은 명령문을 말한다. 이 명령문을 실행하
eae dea vate 증가한다. 단위연산, 주변 명령문, 제어 명령문은 모두

'

=
같은 문제를 푸는 알고리즘이 = ra 첫째 alien 일정 시간복잡도는 neat

i
a
au
ON
41°

oO

St
es)
At
f
대
c¢

3
2,
ae
N,
Oh
5S
yu
과
ied
KI
au
ON
의
기
Dy
i


===== PAGE 39 =====
24

chapter ㅣ 알고리즘: 효율, 분석, 차수

더 빠를 것이라고 바로 알 수 있다. 그러나 둘째 알고리즘의 단위연산 실행시간보다 첫째
알고리즘의 단위연산 실행시간이 11000배 느리다고 가정해보자. 여기서 실행시간에는
제어명령문을 실행하는 시간도 포함한다. 따라서 만약 둘째 알고리즘의 단위연산 실행시
간을 라고 하면, 1,000tE 첫째 알고리즘의 단위연산 실행시간이다. AALS 간단히 하
기 위해서 주변 명령문 실행시간은 두 알고리즘 모두 충분히 작아서 무시할 수 있다고

가정하자. 크기 7인 입력에 대해서 실행시간은 첫째 알고리즘의 경우 2 ×1,0002이고,
둘째 알고리즘의 경우 ^ x tol, 다음 부등식을 풀면 no] 어떤 값일 때 첫째 알고리즘
이 빠른지 알 수 있다.

n?xt>nx 1,000¢
양변을 로 나누면 다음과 같다.
n > 1,000

입력의 크기가 절대로 1.000보다 크지 않은 경우, 둘째 알고리즘이 더 빠르다. 여기서
어떤 알고리즘이 다른 알고리즘보다 어느 시점부터 빠른지 정확하게 결정하기가 쉽지 않
다는 것을 반드시 알고 넘어가야 한다. 두 알고리즘을 비교하면서 얻은 부등식을 분석하
는데 근사범을 사용해야 하는 경우도 있다.

주변 명령문을 실행하는데 걸리는 시간은 무시할 수 있다고 가정했다. 만약 그렇게 가
수 없는 상황이면, 주변 명령문도 고려해야 한다.

정힘

11h

13.3 정확성 분석

이 책에서 “알고리즘 분석"이란 계산시간이나 사용메모리를 기준으로 효율성을 분석함을
뜻한다. 다른 종류의 BAS 있다. 알고리즘이 기대한 대로 실행되는지 증명하는 알고리
즘의 정확성 분석이다. 이 책에서도 필요한 경우 알고리즘의 정확함을 약식으로 증명하
지만 자세히 다루지는 않는다. 알고리즘의 정확성 분석방법을 제대로 공부하고 싶으면
Dijkstra(1976) 또는 Gries(1981) 또는 11088100(1990)의 책을 읽어보기 바란다.

1.4 차수

no] 충분히 큰 경우, 시간복잡도가 /인 알고리즘이 n’ Ql 알고리즘에 비해서 단위연산
실행시간에 관계없이 더 빠르다는 사실을 방금 공부했다. 같은 BAS 푸는 알고리즘이
= 있는데, 첫째 알고리즘의 일정 시간복잡도는 1007이고, 둘째 알고리즘의 일정 시간
복잡도는 0.017^이라고 가정하자. 첫째 알고리즘ㅇ ㅣ 둘째 알고리즘보다 궁극적으로 더
빠르다는 사실은 앞에서 공부한 논리로 증명할 수 ?

정한 단위연산 1회 실행시간이 같고, 주변 명령문 실행시간도 거의 같은 경우 다음 부등
식을 만족하는 /,값에 대해서만 첫째 알고리즘이 더 빠르다고 할 수 있다.

af


===== PAGE 40 =====
@‥60060000 0
1.4 차수 25

0.01n? > 100n
GAS 0.017;으로 나누면 다음과 같다.
n> 10,000

둘째 알고리즘 보다 첫째 알고리즘의 단위연산 실행시간이 더 길다고 하면, 더 걸리는
시간만큼 같이 더 커야 첫째 알고리즘이 빠르다고 할 수 있다.

시간복잡도가 7 과 1007 인 알고리즘은 1차시간 312] Z(linear—time algorithm) °]=}
고 한다. 왜냐하면, 그 알고리즘의 시간복잡도가 입력크기 nol] 대해 1차함수이기 때문이
다. 반면에 n? zt 0.01n? 같은 시간복잡도를 가진 알고리즘은 2차시간 o}712]S(quadratic
—time algorithm) °]e}31 한다. 왜냐하면, 그 알고리즘의 시간복잡도가 입력크기 7에 대
해 3차함수이기 때문이다. 여기서 근본적인 원리를 찾을 수 있다. 즉, 7추서간 eas
은 BE ANZ 앉22/줌보다 7구쪼으로 of ZC. 알고리즘의 분석에서는 이론적으
로 궁극적인 증가상태만 따진다. 다음 절에서는 궁극적인 증가상태에 따라서 어떻게 a
고리즘을 구분하는지 공부할 것이다. 궁극적인 증가상태를 보고 어떤 알고리즘이 더 빠
른지 바로 결정할 수 있다.

1.4.1 AES] 직관적인 소개

57 과 Sn? + 100같은 함수는 1차 항이 없기 때문에 순수2차함수(046 quadratic func—
tion)@} 한다. BHA} O.1n? +n+100 같은 함수는 1차 항이 있기 때문에 완전2차함수
(complete quadratic function)=} 한다. 표 1.3을 보면 궁극적으로 2%} 항이 이 함수를
지배함을 알 수 있다. 즉, 다른 항들의 값은 22} 항의 값에 비하여 궁극적으로 대수롭지
않기 때문이다. 그러므로 비록 함수가 순수2차함수가 아니더라도 순수2차함수로 분류할
수 있다. 즉, 알고리즘의 시간복잡도가 2차함수이면 eid 알고리즘이라고 할 수 있다
는 걸 뜻한다. 복잡도 함수를 분류할 때 낮은 차수의 항들은 항상 버릴 수 있다. 예를
들어, 0.1n? + 10n? + 571 + 25 를 순수2차함수로 분류할 수 bei 이래도 되는 이유를 알
아보기 전에 복잡도 함수의 분류방식에 대한 직관적인 감을 먼저 잡아보자.

순수2차함수로 분류되는 복잡도 함수의 집합은 O(n?) OS 표시한다. 여기서 그리스 대

@ 표 1.3 2x 항이 궁극적으로 지배한다.

n                       0.1n?               0.1n?+n+100
10                         10                       120
20                         40                       160
50                       250                       400
100                    1,000                    1,200
1,000                 100,000                  101,100



===== PAGE 41 =====
@0000000
26     chapter 1 알고리즘: SS 분석, 차수

문자 OL “wEH(theta)’"= 읽는다. 만약 어떤 함수가 O(n’) 집합의 원소라면, “그 함수
는 차수가 /^”이라고 한다. 예를 들어, 낮은 차수의 항은 버릴 수 있으므로, 다음과 같다.
g(n) = 5n? + 100n + 20€ O(n’)

g(n) 2] 차수가 7?이란 뜻이다, 더.자세한 예로 1.8.1절에서 공부한 알고리즘 1.3(교
정렬)의 시간복잡도는 T(n) = (2 -1)/2였다. 다음과 같이 전개한

n(n—1)  ron

2    2  2

낮은 차수의 항 7/2을 버리면 7(202)ㅎㅇ(/2”)이 된다.

어떤 알고리즘의 시간복잡도가 O(n?) ol] 속하면, 그 알고리즘을 2차시간 알고리즘 또

i  개

3

는 O(n’) 알고리즘이라고 한다. “그 알고리즘은 ㅇ(/』”)이다"라고 하기도 한다. 교환정
렬 알고리즘은 2차시간 ale] Sole,
SABE 분류될 수 있는 복잡도 함수의 집합은 O(n’ olay, 이 집합에 속하는
수는 차수가 7/"이라 하는 식으로 :차함수의 경우와 비슷하게 정의할 수 있다. 이런 집
SS 복잡도 카테고리(6027ㅁ2016×※1[ 0816801168)라고 한다. 가장 흔히 나타나는 복잡도 카       |
테고리를 몇 개 나열해 보면 다음과 같다.

O(lgn) O(n) O(nlgn) O(n?) O(n?) 0(2")

이 순서에서 만약 f(r) °] g(n) o] 속하는 카테고리의 왼쪽에 있는 카테고리에 속한다면,
f (n)& 그래프 상에서 궁극적으로 g(n) 2] 아래에 위치한다. 이 카테고리들에 속한 가장
간단한 함수들인 2, len, 7187 SS 그래프로 그려보면 그림 1.3과 같다. 시간복잡도
가 이 함수인 알고리즘의 실행시간은 표 1.4와 같다. 각 알고리즘의 단위연산을 실행하는
데 10억 분의 1초가 걸린다고 단순하게 가정하자. 이 Hol] 나타난 결과를 보고 아마도
놀랄지도 모른다. 알고리즘이 지수시간 알고리즘이 아닌 이상 쓸만하다고 생각할지도 모
른다. 그러나 2차시간 알고리즘조차도 크기가 10억인 입력을 실행하는데 31.7년이 걸린
다. 반면에 Oo} O(n lg n) 이비즈 같은 입력을 실행하는데 29.9초밖에 걸리지 않는
다. 보통 상당히 큰 YAS 허용할 만한 시간에 실행할 수 있다고 가정할 수 있기 때문에
알고리즘 O(nlgn) 또는 더 빠른 카테고리에 속해야 한다. 시간복잡도가 높은 차수의
카테고리에 속하는 알고리즘이 유용하지 않다는 말은 아니다. 24}, 84}, 또는 더 큰 차수
의 시간복잡도를 가진 알고리즘도 실제로 많이 쓴다.

단순히 차수만 아는 것보다 시간복잡도를 더 정확히 알면 더 많은 정보를 얻을 수 있다
는 사실을 간과해서는 안 된다. 예를 들어, 앞에서 공부한 시간복잡도가 1007 과 0.017^인
의 알고리즘을 비교해보자. 두 알고리즘 모두 단위연산과 주변 명령문을 실행하는데 걸
리는 시간이 같다고 하면, 입력크기가 10,000보다 작은 예에서는 2차시간 알고리즘이



===== PAGE 42 =====
@00@00000 0
14 치수 27

20                   /72
131,072
65,536 +
32,768 +                                                                 ane
16,384 +
8,192 -
4,096 -
2,048 -
1,024 -
512
256 |-
128
64
32

16|-
Ign

foe)
ㅣ

aS
T

ㅣ | ㅣ | | ㅣ | ㅣ aa
0  1  2  4  8 16 32 64 128 256 512 1024 2048

그림 1.3 흔히 나타나는 복잡도 함수의 증가율

더 효율적이었다. 만약 이보다 더 큰 크기의 입력을 전혀 사용하지 않는 경우라면, 차시
간 알고리즘을 사용하는 편이 나을 것이다. 반면 시간복잡도가 각각 ㅇ(7)와 O(n?) ee

만 안다면, 이에 대한 정보는 전혀 알 수 없을 것이다. 하지만 실제로 이런 극단적인
사례는 흔치 않다. 더구나, 시간복잡도를 정확하게 구하기가 굉장히 어려운 경우도 있다.
따라서 차수만 구하고 만족하기도 한다.



===== PAGE 43 =====
28

chapter

1 Qe

ab

ㅣ
mo
AL
Iz
Pall
+

@ 표 1.4 시간복잡도 별 알고리즘의 실행시간

      f(n) =lgn     f(n) =n     f(n)=nlgn     f(n)=nr?       f(n) =n3       f(n) =2"
10            0,003 ws*        0,01 ps           0,033 ps            0,10 ps            1,0 us                 Lys
20           0,004 ps          0,02 us          0,086 ys            0,40 us            8.0 ps                 ims’
30           0,005 ps         0,03 us          0,147 us            0,90 us            27.0 us               1s
40           0,005 us          0,04 ps          0,213 ys            1,60 ps             64,0 us               18,3 min
50           0,006 ps          0,05 us          0,282 us            2,50 ps            125.0 us              13 days
10°           0,007 ps          0,10 ps           0,664 js            10,00 ps           1,0ms                 4X10" years
10°           0,010 ps          1,00 us           9,966 us            1,00 ms             10s
10°           0,013 us          10,00 ps         130,000 ps         100,00 ms         16,7 min
10°             0,017 ps            0,10 ms            1,670 ms              10,00 s                11,6 days
10°              0,020 us            1,00 ms             19,930 ms             16,70 min            31,7 years
10“            0,023 ws           0,01s              2,660 s               1,16 days            31,709 years
10°             0,027 us            0,10s               2.660 s                115,70 days         3,17X10' years
10°             0,030 ps            1,00s               29,900 s               31,70 years
*1 ws = 10° second,
tims = 10° second,

1.4.2 차수의 정식 소개

앞 절에서 차수(6)에 대한 직관적인 감을 잡았다. 이 절에서는 차수를 엄밀하게 정식으
로 정의하기 위한 이론을 소개한다. 먼저 기본 개념 두 가지를 먼저 알아보자. 첫째로
살펴볼 WAS “= Olbig 0)"이다.

정의
주어진 복잡도 함수 f(n) 에 대해서 O(/(n)) S 정수 N 이상의 모든 7에 대해서 다음 부등식
이 성립하는 양의 실수 cS} 음이 아닌 정수 VO] 존재하는 복잡도 함수 (7) 의 집합이다.

g(n) < ex f(n)

만약 g(n)= 0(7(72))이면, “g(n)& f(n)2] 큰 OoltP eta 한다. 그림 1.408)는 '큰
O'S 그림으로 나타내 준다. 이 그림을 보면 비록 g(n)o] 처음에는 6/(72)의 위에서 시
작하지만, 궁극에 가서는 밑으로 내려가며 계속 밑에 머문다. 그림 1.5에서 상세한 oS
보여준다. 이 그림을 보면 7” + 10ne& 처음에는 비록 2n? 9] 위에 있지만, n= 10에 대
해서

n?+10n < 207?
따라서 “= 02] 정의에서 c= 29 N= 102 취할 수 있으므로, 다음과 같이 결론지을
수 있다.
n? + 10n€ O(n’)



===== PAGE 44 =====
© 예제 1.7

1.4 차수       29
cf(n)                                                                af(n)
90)                              90                               90
cf(n)
ㅣ                                               cf(n)                        |
!                    n—              i              n>                   i         n>
N                                     N                                    N
(a) g(n) € O(f(n))                  (b) g(n) 6 Q(F(n))                 (c) g(n) 6 8(f(n))

3221.4 ‘20°, (2, @의 Say 설명

예를 들어, 만약 g(n)°] O(n’) ov, g(n)- 2 궁극적으로 그래프 상에서 어떤 순수2차
함수 0/^ 아래에 놓이게 된다. 이는 만약 g(n)o] 어떤 알고리즘의 시간복잡도라면, 그
알고리즘의 실행시간은 궁극적으로 빠르기가 최소한 2차함수만큼은 된다는 뜻이다. 이
를 분석에 사용할 때 g(n) 2 궁극적으로 최소한 순수2차함수만큼 좋다라고 할 수 있다.
‘2 "(그리고 곧 소개하게 될 다른 개념도 포함)는 함수의 궁극적인 상태만 고려하기
때문에 함수의 점근적인(6872ㅁㅁ6040) 상태를 나타낸다고 말한다. “큰 OVE 함수의 점근
적인 AkeHasymptotic upper 00400)을 정한다라고 한다.

이해를 도울 예제를 몇 개 살펴보자.

Sn’ O(n?) YS 증명하자. c=52} N=0-S 선택하면 n = 0인 모든 nol] 대해서 다음 부등식이
성립한다.
572? < 5n?

따라서 5n°= O(n”) O}cy,



===== PAGE 45 =====
30

chapter 1 알고리즘: 효율,

© 예제 1.8

© 예제 1.9

© 예제 1.10

© 예제 1.11

Ad, 차수

AL

알고리즘 1.8(교환정렬)의 시간복잡도는 다음과 같이 계산하였다.

n(n—1)
2

T(n) =

T(n)=O[n?) YS 보이려면 정수 / 이상의 모든 7에 대하여 다음 부등식이 성립하는 <와 No]
존재하는지 찾아야 한다. c= 긍 과 N=O- 선택하면 0 이상의 모든 *에 대하여 다음 부등식이
성립한다.

따라서 7(/2)ㅇㅎ0(0”)이다.

“큰 OF; 학생들에게 종종 어렵게 느껴지는 이유는 어떤 함수가 다른 함수의 "큰 (/"임
을 보이기 위해서는 유일한 ㅇ와 이 존재해야 한다고 잘못 생각하기 때문이다. 사실 그
렇지 않다. 그림 1.5를 가지고 n? + 10n€ O(n”) 7} 사실임을 c= 2 와 N= 10을 사용하
여 보여줄 수 있다. 다른 값으로도 다음 예제와 같이 이를 증명할 수 있다.

n> +10n€ O(n?) Y-& 보이기 위해서 정수 / 이상의 모든 nol] 대하여 다음 부등식이 성립하는
6와 No] 존재하는지 찾아보자. 6==11과 /7=1을 선택하면 다음 부등식은 7 > 1인 BE 7에
대하여 항상 성립한다.

n?+10n < n?+10n? = 11722

따라서 n? +10n€ O(n”) ] ch,

일반적으로, ‘a o's 증명하려면 부등식

ito

ub4sS
pS ee |

rr

가장 찾기 쉬운 값을 빨리 찾는

nr’ O(n? +10n) 임을 보이기 위해서 N 이상의 모든 정수 nol] 대하여 다음 부등식이 성립하는
c2} 이 존재하는지 찾아보자. 6==1과 N=0S 선택하면 다음 부등식은 7 = 0인 모든 na
대하여 항상 성립한다.

n? 으 1 × (2? +ㅜ100)
따라서 n?= 002^+101)이다.

다음 마지막 예제를 든 이유는 “큰 O'S 표시된 함수는 그림 1.30] 표시된 대로 간단한
함수 중 하나일 B07} 없다는 걸모여주기 위함이다. 그러나 보통 그림 1.8에 있는 대로

간단한 함수를 쓴

3 3 코그  i ci ㆍ

n& On?) & 증명하기 위해서 정수 N 이상의 모든 7에 대하여 다음 부등식이 성립하는 와 NV


===== PAGE 46 =====
© 예제 1.12

@‥600000 0
1.4 차수 31

을 찾아야 한다. 6=1과 //=1을 선택하면 n = 191 모든 nol 대하여 다음 부등식이 성립한다.
n<1x<n

따라서 n= 000”)이다.

이 마지막 예제는 큰 Oo] 관한 중요한 SYS 보여준다. 복잡도 함수가 O(n’) of
속하기 위해서 굳이 2차함수일 필요가 없다. 그래프 상에서 궁극적으로 순수3차함수 oF
Holl 놓이기만 하면 된다. 그러므로 어떤 대수0088110400함수나 1차함수도 O(n") ol] 속
한다. 비슷한 논리로 대수함수나 1차함수나 2차함수도 O(n’) ol] 속한다. 그림 1.68/에서
O(n’) o] 속하는 함수의 예를 보여준다.

“2 O'7} 복잡도 함수의 점근적인 상한을 나타내듯이, 다음 AWS 복잡도 함수의 점
근적인 하한(387004060610 lower bound)-& 나타낸다.

정의

=

주어진 복잡도 함수 f(r) 에 대해서 O(f(n))S 이상의 모든 7에 대해서 다음 부등식을
만족하는 QO] 실수 <와 음이 아닌 정수 NO] 존재하는 복잡도 함수 0(7/)의 집합이다.

g(n) = cx f(n)

여기서 그리스 대문자 Q "오메가(00688) 로 읽는다. 만약 g(n)EQ(f(n))o}H,
“g(n)& f(n)2} 오메가이다"라고 한다. 그림 1400)는 “(2"”를 그림으로 보여준다. qs
몇 개 공부하자.

nS Qn?) YS 보이자. 정의에 의해서 ^ 이상의 모든 정수 nol] 대하여 다음 부등식이 성립하
는 와 No] 존재하는지 찾아보자. 6=1와 N=00]H 다음 부등식은 0 이상의 BE nol] 대하여
항상 성립한다.

502? > 1 ×% 722

따라서 Sn? 2(n") ©] ey,

@(n?)

3lgn+8 4n?
5n+7     6n? +9

4n+ 3772

6n® + n4*

2nlgn          5n?+2n                                                                                               20+ 47

(a) O(n?)
AZ 1.6 O(n’), Qn), O(n?) 242] 관계

(c) 0079 = O(n?) 0 Q(n*)


===== PAGE 47 =====
@0@00000 0
chapter 1 알고리즘: 효율, 분석, 차수

32

© 예제 1.13

© 예제 1.14

© 예제 1.15

^ +10nEQ(n?) YS 보이기 위해서 N 이상의 모든 nol] 대하여 다음 부등식이 성립하는 와
이 존재하는지 찾아보자. 6==1과 N=0S 선택하면 다음 부등식은 1 이상의 모든 nol] 대하여
항상 성립한다.

n?+10n > 72?

따라서 7^+107ㄷ1(2(027”)이다.

알고리즘 1.8(교환정렬)의 시간복잡도는 다음과 같음을 증명해보자.

n(n—1)
2

n> 2 BE nol] 대하여 다음 부등식이 성립한다.

2072) =           EN(n?)

alee

w|3

따라서 n= 291 모든 nol] 대해서 다음 식이 성립한다.

n(n—1)
2

2

= By ml
~2 2

mle

0=그과 N=2-2 선택하면 T(n) E(x?) o}ch.

J{y
illo

“2 "의 경우와 마찬가지로 29] 정의 BAS 만족하는 상수 cS} NO] 유일할 필요는
없다. 따라서 조건이 만족하는지 쉽게 알게 해주는 상수이면 뭐든지 선택해도 상관없다.

만약 g(n)°] Q(n*)o] 속하면 g(n)S 궁극적으로 그래프 상에서 어떤 순수2차함수
위에 놓이게 된다. 즉, 0(0))은 "궁극적으로 최소한 순수2차함수만큼은 나쁘다"라고 할
수 있다. 그러나 다음 예제에서 보듯이 그 함수가 2차함수일 필요는 없다.

EAAn2) YS 보이기 위해서 N 이상의 모든 7에 대하여 다음 부등식이 성립하는 <와 VO]
존재하는지 찾아보자. ㅇ=1과 N= 10] 다음 BEALS 1 이상의 모든 naj] 대하여 항상 성립한다.

n>ixn?

따라서 nFEQ(n?) O02 결론지을 수 있다.

그림 1600)에서 <2(002”)에 속하는 함수의 예를 보여준다.

만약 어떤 함수가 O(n?) St O(n?) ol] 모두 속한다면, 궁극적으로 이 함수는 그래프 상
에서 어떤 순수3차함수 아래에 위치하게 됨과 동시에 또 다른 어떤 순수2차함수 위에 위
치하게 된다. 즉, 궁극적으로 이 함수는 최소한 어떤 순수2차함수만큼 좋고, 또 다른 어
떤 순수2차함수만큼 나쁘다. 따라서 이 결과가 우리가 찾던 차수의 엄밀하고 정확한 정
의가 된다. 다음 정의를 보자.


===== PAGE 48 =====
© 예제 116

© 예제 1.17

@06000000
1.4 차수 33

33 ox
2 io

진 복잡도 함수 f(r) oll 대해서 다음과 같이 정의한다.
O(f(n)) = OF (n)) NT 2(F(n))

O(f(n))= 이상의 모든 정수 에 대해서 다음 부등식이 만족하는 양의 실수 <, dQ} SO|
아닌 정수 NO| 존재하는 복잡도 함수 g(n) 의 집합이다.

cx f(n) < g(n) < dx f(n)

만약 g(n)EO(f(n))OA, “g(n)& f(n)2] 차수(@ㅠ000)이다"라고 한다.

T(n) © O(n") (Qn?) = O(n’)

그림 1660)은 O(n*)°] O(n?) F} O(n?) 2] 교집합임을 BIST, 그림 11.4(0)는 OS
설명해 준다. 그림 1.6(0)를 잘 보면 함수 57, + 7S Qn?) ol] 속하지 않고, BE An? + 377”
은 0(2”)에 속하지 않음을 알 수 있다. 그러므로 이 두 함수는 BE O(n?) oy] 속하지
않는다. 직관적으로는 맞아 보이지만 아직 정식으로 증명하진 않았다. 이 증명을 어떻게
하는지 다음 예제를 통해서 살펴보자.

이 2(n*) ol] 속하지 않음을 모순유도 증명법(6:00【 by contradiction) © 증명해보자. 이 증명
We 증명하고 싶은 VAS 참이라고 가정하고 여기에서는 neon’), 모순을 유도한다. 즉 유
도한 결과는 가정과 모순이 되므로 애초에 가정했던 것이 참일 수 없다고 결론짓는다.

nE An") a 함은 정수 ^ 이상의 모든 에 대해서 다음 BEALS 만족하는 양의 상수 <와 음이
아닌 No] 존재한다라고 가정하자.

02 = EN
만약 이 부등식의 양변을 en OB 나누면, 정수 # 이상의 모든 nol] 대해서 다음과 같이 된다.
본 n
Cc

그러나 n> 1/0인 BE no} 대해서 이 부등식은 성립하지 않는다. 이는 n> Wel BE nol] 대해
서 성립하지 않는다는 Eo] 된다. 모순을 유도했으므로 no] An?) o] 속하지 SS 증명하였다.

함수 nd} 함수 7”의 관계를 표현하는 차수에 관한 정의가 하나 더 있다.


===== PAGE 49 =====
34

chapter 1 알고리

© 예제 1.18

© 예제 1.19

ol

(n) Ol 대해서 o( f(n)) 은 BE 양의 실수 에 대해서 n = NS 만

음 부등식을 만족하는 음이 아닌 정수 NO] 존재하는 SE 복잡도

=

ㅎ

수

ol!   is

0

g(n) < ex f(n)

만약 g(n)Eo(f(n))OVA, g(n)& f(n)2] 작은 오(60811 0)라고 부른다. "큰 (big

는 그 범위가 성립하는 “어떤” 양의 실수 c7} 반드시 존재한다는 A 의미한다. 바로

0 정의는 “WE” 양의 실수 col] 대해서 그 범위가 성립해야 한다. 범위가 모든 양수

co] 대해서 성립하므로, 임의로 작은 col] 대해서 성립한다. 예를 들어, 001)ㅋㅇ(7(42))
이면, n= NS 만족하는 모든 no] 대해서 다음 부등식을 만족하는 이 존재한다.

g(n) < 0.00001 x 7 (n)

n°] 커지게 되면, g(n)& f(ndol 비해서 하찮을 만큼 작아지게 된다. 분석의 관점에
서 바라봐서 만약 002)이 0(7(42))이면, g(n)2 fn) 같은 함수보다는 궁극적으로 훨씬
좋다. 다음 예제들이 이를 보여준다.

다음이 성립함을 증명해보자.
n€o(n?)
c> 0인 가 주어졌다고 하자. n> NS 만족하는 모든 no} 대해서 다음 부등식을 만족하는 V
을 찾을 필요가 있다.
n<cr
이 부등식의 양변을 cn OB 나누면, 다음을 얻는다.
i
é

=n

그러므로 N> - 을 만족하는 “을 하나 찾으면 충분하다.

의 BRE 상수 col] 의존한다는 사실을 주목하자; AWS 들어, 만약 6=0.00001이면 최소
100,000°] 되는 7 값을 취해야 한다. 즉, 7 = 100,000인 모든 7에 대해서 다음 부등식은 성립힌   i
n < 0.00001n?

ale

n& o(5n) ol 속하지 SSS 증명해보자. 모순유도법을 사용하여 증명한다. 0=1/6이라 하자.
만약 nEo(5n) 이면, n= NS 만족하는 모든 no] 대해서 다음 부등식을 만족하는 WO] 반드시
존재한다.


===== PAGE 50 =====
1.4 차수     35
이는 모순이므로 7은 o(5n) ol 속하지 않는

는다. 증명이 완료되었다.

다음 정리는 “작은 오"와 점근적 표기법의 관계를 설

명한다.
『정리 1.2
만약 g(n)Eo(f(n)) VA, 다음이 성립한다.
g(n)€ O(f(n)) — AfF(n)).
즉, g(n)& OF(n)) oH 속하지만, QF (n)) oH 속하지 않는다.
증명 : 0(2)ㅇㅇ(/(12))이므로, 모든 양의 실수 col 대해서, n => NS 만족하는 모든 nol 대해
서 다음 aed 만족하는 No] 존재한다.

g(n) < eX f(n)
이는 이 범위가 어떤 col] 대해서는 확실히 성립한다는 뜻이다. 그러므로 다음이 성립한다.
g(n)E O(f(n))
(n)°] Q4(n)) oH] 속하지 않음을 모순유도법으로 증명해보자. 만약 g(n)e
n2N& nth 모든 7에 대해서 다음 부등
이 존재한다.

Af(n)) OVA,
등식을 만족하는 ㅇ> 0인 어떤 실수 <와 어떤

g(n) = ex f(n)
그러나 g(n)€ol(f(n)) BS, n= 을 만족하는 BE 7에 대해서 다음 부등식을 만족하는
어떤 가 존재한다.

과 보다 큰 모든 7에 대해서 이 두 부

SAS 성립해야 한다. 이는 모순이므로 g(n) 2
AF(n)) } 속할 수 없다. 증명이 완료되었다

o(f(n))# O(f(n)) —                은 집합이라고 생각할는지 모르겠다. 이는 사실
이 아니다. 0(7(02))-02(7(2))에 이 o(f(n))oll 속하지 않는 색다른 함수가 있
다. 다음 예제를 보자.

QF (n))=

*예제1.20 다음 함수를 고찰해보자.
ae (" 7이 짝수인 경우
ww 1 ne] 홀수인 경우
음을 증명하는 건 연습문제로 남겨 둔다.
g(n)E O(n) -2

(n) OJAI g(n)-& o(n) oj 속하지 않는다.



===== PAGE 51 =====
@‥@00000 0
36     chapter ㅣ 알고리즘: 효율

4

Aq, 차수

Ad

예제 1.202 물론 억지로 끼워 맞춘 Ao] 자연스럽지 않다. 실제 알고리즘의 시간복
HES 나타내는 복잡도 함수의 경우, 일반적으로 O(f(n))— Of (n))o] 속한 함수는
07 (01))에도 보통 속한다.

@를 좀 더 공부해보자. 연습문제에서 다음 두 식이 서로 필요충분조건인지 증명하도
록 하였다.

g(n)EO(f(n)), f(n)EO(g(n))
예를 들면, 다음 두 식은 서로 필요충분조건이다.
n+ 10n€ O(n”),  ^ O(n? +10n)

이는 @가 복잡도 함수를 ABA 집합(01911 set) OS 나누어 구별할 수 있다는 뜻이
다. 이러한 집합을 복잡도 카테고리(60ㅁ2160” category) efi! 한다. 주어진 카테고리에
속한 어떤 함수도 그 카테고리를 대표할 수 있다. 카테고리를 표시할 때 보통 편의상 속
한 함수 중에서 가장 간단한 함수를 쓴다. 위 복잡도 함수의 복잡도 FIDE O(n’) 2
로 표시한다.

어떤 알고리즘은 시간복잡도가 7에 비례하지 않는 경우도 있다. 예를 들어, 알고리즘
1.1의 최선 시간복잡도 B(n) 2 모든 n gol] 대해서 1이었다. 이러한 함수가 포함된 복잡
도 카테고리는 어떤 상수로라도 표현할 수 있지만, 보통 가장 간단한 ㅇ(1)로 표시한다.

이제 차수의 특성을 살펴보자. 차수의 특성을 이해하면 복잡도 함수의 차수를 쉽게 a
정할 수 있다. 여기서 나열한 특성을 모두 증명하지는 않는다. 일부는 연습문제에서 증명
하게 했으며, 일부는 다음 절에서 얻는 결과를 이용하면 쉽게 증명할 수 있다. 2번은 이
미 앞에서 보았지만, 특성을 모두 한자리에 모아두면 좋으므로 여기에 포함하였다.
차수의 특성

1. g(n)\E 0(7(02))은 f(n)EQ(g(n))F} 서로 필요충분조건이다.

2 001)60(7(0))은 f(n)EO(g(n)) 3 서로 필요충분조건이다.

3, 0>1이고 0>1이면, 다음이 성립한다.

log, n=O (log, n)
대수 복잡도 함수는 모두 같은 복잡도 카테고리에 속한다는 뜻이다. 이 카테고리는
Ollgn) OS 표시한다.
4. 0 > 0> 0이면, 80] 성립한다.
a” €o(b")

지수 복잡도함수는 밑수가 다르면 복잡도 카테고리도 다르다는 뜻이다.
5. 0> 0인 모든 0에 대해서 다음이 성립한다.


===== PAGE 52 =====
© 예제 1.21

© ofall 1.22

* 예제 1.23

@0@000000
14 치수   37
a” €o(n!)

nl-& 어떤 지수 복잡도 함수보다 더 나쁘다(느리다).
6. 복잡도 카테고리들을 순서대로 나열하였다.

60087) O(n) 60187) O(n?) O(n’) O(n*) O(a") O(b") O(n!)
여기서 k> ) > 2이고 b> a> 이다. 복잡도 WF g(n)°] f(n)&S 포함한 카테고
리의 왼쪽에 위치한다고 하면, 다음이 성립한다.

g(n)€Eo(f(n))
7. ¢ = 0이고, d> 0이고, g(n)E OF (n))°]H, h(n)EO(F(n))o]H, 다음이 성립

한다.
0×0(02)+0×/0)ㅇ0(7(02))

특성 3에 따르면, 모든 대수 복잡도함수들은 같은 복잡도 카테고리에 속한다. 예를 들면,
O(log, n) = O(Ig n)

이는 log, nif 167과의 관계는 Tr? + 5g} 7”과의 관계와 같다는 뜻이다.

특성 6에 따르면, 대수 함수는 모두 다항식보다 궁극적으로 좋고(빠르고), 다항식은 모두 지수함
수보다 궁극적으로 좋고, 지수함수는 모두 계승((8060208))함수보다 궁극적으로 좋다. 예를 들면,
Ign€o(n) oat, n!€o(2") o]a1, 2" o0(n!) Oo],

특성 6과 7S 반복하여 사용할 수 있다. 예를 들면, 5n+3lgn+lonlgnt+7n’SO(n?) YS 다
음과 같이 증명할 수 있다. 특성 6과 7S 반복 적용하면 다음을 얻고,
7? E O(n?)
이는 다음을 의미하고,
10nlg n+7n?=O0(n?)
이는 다음을 의미하고,
3lg n+10nlg n+7n?= O(n?)
이는 다음을 의미한다.

5n+3lgn+10nlgn+7n?=O(n7)

실제로는 특성을 반복 적용하는 대신, 낮은 차수를 가진 항을 그냥 버리면 된다고 단
히 생각하면 쉽다.

A>


===== PAGE 53 =====
38

Pel
>

chapter 1 알고리즘: 효율, BA 차수

ㅣ
T(n)e ah  ))임을
Ae 경우가 때로 있다. 이런 경우 T(n)E O(f (n))           로
왜냐하면 T(n)°] f(n) 함수만큼은 최소한 SSS 알았기 때문이다. 비슷한 논리로,
T(n)EQ( (n)) at Gale 만족할 수도 있
큼은 나쁘타는 정보라도 최소한 주고 있기 때문이다.
마무리 짓기 전에 책이나 문서에 따라서 복잡도를 다른 형식으로 표시하기도 한다.
f(n)€O(n?) 대신 f(n) = O(n’)
f(n)€ O(n?) 대신 f(n) = O(n’)
둘 다 같은 뜻이다. “차수"의 역사를 알아보려면 <ㅠ468(1970)를 읽어보고, 여기 주어진
차수의 정의를 자세히 알고 ALO A Brassard(1985)S 읽어보기 바란다. 여기서 배운 “at
오", 2, OF 정의는 대부분 표준이다. 그러나 "작은 오'는 달리 정의하는 경우가 있다.
O(n), O(n’) 등의 집합을 “복잡도 카테고리"라고 부르는 건 표준이 아니다. 어떤 사람
은 9장에서 공부할 문제 집합을 가리키는데 더 많이 사용하므로 혼돈을 야기할 수 있음에
도 불구하고 “복잡도 AlS(complexity 888) 이라고 하기도 한다. 어떤 사람은 이름없이
설명하기도 한다.

@1.4.3 극한을 사용하여 차수를 결정하기

이제 차수를 결정하는데 극한01040을 사용하는 방범을 알아보자. 이 AS 이해하려면
일단 극한과 미분에 대해서 잘 알고 있어야 한다. 극한과 미적분에 관한 지식은 여기서만
쓰므로, 이 책의 다른 부분을 이해하는 데는 필요없다.

> Bel 1.3
다음이 성립한다.

one 이면, g(n) € O(f(n)) (e> 091 경우 성립)
lim Fn, co 0 이면, g(n) € o(f(n))
"            oo f(n) € o(g(n))

: 증명은 연습문제로 남겨눈다.

이
of



===== PAGE 54 =====
© 예제 1.24

© 예제 1.25

© 예제 1.26

@‥600000 0
1.4 차수 39

정리 1.8에 의해서 다음이 성립한다.

= aan)
왜냐하면 다음이 성립하기 때문이다.
n?
lim  시  = 1110 는  =0
n—0o 72”   n> 470

예제 1,249] 경우 굳이 정리 1.8을 쓰지 않아도 바로 결과를 알 수도 있기 때문에 정리
1,30] 그리 중요해보이지 않을 수 있다. 다음 예제를 보면 왜 정리 1,90] 쓸모 있는지 알
수 있다.

정리 1.8에 의하면 / > ㅇ> 0이면, 다음이 성립한다.
a" €o(b")

왜냐하면 다음이 성립하기 때문이다.

lim*-= lim|( 4 b I 0

noo b” — n—-s00

여기서 0 < a/b <10]7] 때문에 극한은 0이다.
이것은 차수의 S790. 4,289] 거의 끝부분) 중에서 특성 4에 해당한다.

정리 1.8에 의하면, a> 0이면 다음이 성립한다.
a” €o(n!)

만약 a = 1이면 결과는 사소하게 얻는다. a> 1이라고 가정해보자. 만약 no] 굉장히 커서 다음
과 같다면,

| 2
 8 | ^“
다음이 성립한다.
a     Cee 2 BL)"
ni   kG ooo (at)"/2   a
— ee
[n/2] times
이므로, 다음의 성립한나.
Pe
100.

noo Tle

이것은 차수의 특성들 중에서 특성 5에 해당한다.

다음 정리는 정리 1.8과 더불어 유용하게 쓸 수 있다. 이 정리의 증명은 대부분의 미적


===== PAGE 55 =====
40     chapter ㅣ 알고리즘: 효율, 분석, 차수
분학 책을 찾아보면 나와 있다.

© 예제 1.27

© 예제 1.28

> al 1.4

로피탈의 FA\(L'Hopital's Rule)
/(2)와 9(2)가 각각 비분계수 /(2)와 0'(2)로 미분 가능하고, 다음이 성립하면,

lim/(z) = limg(z) = 00

lim g(x)

정리 1.4는 실수 변수의 함수에 대하여 성립하는데, 복잡도 GPE 정수 변수의 함수이
다. 그러나 복잡도 함수(예: Ig n, n 등)의 대부분은 실수 변수의 함수이기도 하다. 더구
나, 함수 7(2)가 실수 변수 2의 함수라면, 다음 등식은 우변의 극한이 존재하면 항상
성립한다.

lim f(n)= lim f(x)

n—0©o         @—> co

여기서 n& 정수이다. 그러므로 다음 예제에서 보듯이 정리 1.4를 복잡도 분석에 적용할

수 있다.

정리 1.8과 1.4에 따르면 다음이 성립한다.

lgn € o(n)
왜냐하면 다음이 성립하기 때문이다.
. 162 _,. d(lgx)/dr_,. 1/(xln2) _
보오 lim gejae tim?

정리 1.8과 1.4에 따르면 b> 1이고 04 >1일 때 다음이 성립한다.
log, nE O(log, n)
왜냐하면 다음이 성립하기 때문이다.

} 1086. 0008.40)/08  1/(271ㅁ00) _ Inb
스미  M 4008.2)/62 0 1/(2100) Ina

이것은 차수의 특성들 중에서 특성 3에 해당한다.

>0



===== PAGE 56 =====
@ 1,5 이 책의 개요

이제 복잡한 알고리즘을 개발하고 분석할 준비가 끝났다. 전체적으로 응용 분야보다 기
법을 기준으로 구성하였다. 앞에서 언급했듯이 이렇게 구성한 목적은 문제를 푸는 다양
한 기법의 레퍼토리를 숙지하기 위함이다. 2장에서는 “분할정복"이라는 기법을 공부한
다. 8장에서는 동적계획법을 배운다. 4장에서는 "탐욕적인 접근방법” 제시한다. 5장에서
는 되추적 기법을 소개한다. 6장에서는 되추적과 관련된 “한계치에 따라 가지치기"라는
기법을 알려준다. ?장과 8장에서는 알고리즘을 개발하고 분석하는 것에서 문제 자체를
분석하는 것으로 주제를 바꾼다. 문제의 분석을 계산복잡도 분석이라고 하는데, 계산복
잡도 EAS 주어진 문제를 푸는 모든 알고리즘의 시간복잡도의 하한을 결정한다. ?장에
서는 정렬 문제를 분석하고, 8장에서는 검색 문제를 분석한다. 9장에서는 문제를 계층별
로 분류해본다. 문제의 계층 중에는 최악 시간복잡도가 지수보다 좋은(빠른) 알고리즘을
아무도 발견하지 못한 문제의 계층도 있다. 그렇다고 이런 알고리즘이 불가능하다고 누
가 증명한 것도 아니다. 이런 문제가 수천 개나 있으며, 이들은 서로 밀접하게 관련이
있다. 그러다보니 이런 문제의 연구는 전산학에서 새롭고 도전할 만한 한 분아로 성장했
다. 10장에 다시 알고리즘을 개발하는 문제를 다룬다. 하지만 3~6장 제시한 기법과는 달
리 색다른 유형의 문제를 다룬다. 즉, 정수론적 알고리즘을 공부한다. 정수론적 알고리즘
은 정수에 관한 문제를 푸는 알고리즘이다. 처음 10개 장에서 다루는 알고리즘은 모두
명령을 하나씩 차례로 실행하는 프로세서가 하나뿐인 컴퓨터를 위하여 개발된다. 컴퓨터
하드웨어의 가격이 급격히 내려감에 따라서 병렬 컴퓨터가 많이 등장하고 있다. 병렬 컴
퓨터는 프로세서가 둘 이상 있고, 두 개의 다른 명령을 (동시에) 따로 실행할 수 있다.
병렬 컴퓨터에 쓰려고 작성한 알고리즘을 “병렬 알고리즘"이라 한다. UAE 병렬 알

고리즘을 소개한다.

@ 연습문제

112
1. 개의 수로 구성된 리스트(또는 배열)에서 가장 큰 수를 찾는 알고리즘을 작성하시오.
2. 7개의 수로 구성된 리스트에서 7/개의 가장 작은 수를 찾는 알고리즘을 작성하시오.

3. 7개의 원소로 구성된 집합에서 3개의 원소를 가진 부분집합을 모두 인쇄하는 알고리즘을
작성하시오.

4. 삽입정렬(086040ㅁ0 80450 알고리즘을 작성하시오. 다음에 삽입할 BAS 찾는데 이분검색
알고리즘을 사용하시오(7.2절 참조).

5. 정수 2개의 최대공약수(@0068[086 common divisor)S 구하는 알고리즘을 작성하시오.



===== PAGE 57 =====
42     chapter 1 알고리즘: 효율 분석, 차수

At

(

oe

6. nA 수로 구성된 리스트에서 가장 작은 수와 가장 큰 수 모두를 찾는 알고리즘
시오. 배열의 AAS 기껏해야 1.57번 정도만 비교하는 WIS 찾도록 하시오

작성6

rr
1

7. 거의 완전한 이진트리(31008 complete binary tree)7} 힙08082)인지를 알아내는 알고리즘
을 작성하시오.

1.2절
8. 검색 작업을 하려 한다. 순차검색(알고리즘 1.1)이 적절함을 보여주는 상황을 설명하시오.

9. 정렬을 하는데 교환정렬(알고리즘 1.9)을 사용하지 말아야 할 실제 예를 드시오.

1.3절

10. 연습문제 1-7에서 작성한 알고리즘의 단위연산을 각각 정의하고, 각 알고리즘의 실행시간
을 조사하시오. 가능하면 알고리즘의 일정 시간복잡도를 구하시오. 일정 시간복잡도를 구할
수 없으면, 최악 시간복잡도를 구하시오.

11. 일반 삽입정렬 알고리즘과 연습문제 4에서 작성한 이분검색을 사용한 삽입정렬 알고리즘의
최악, 평균, 최선 시간복잡도를 구하시오.

12. *를 양의 정수라고 하자. 7개의 서로 다른 BFE 구성된 길이가 nel WSS 정렬히

선형시간 알고리즘을 작성하시오.

어
다

13. 알고리즘 AE 107”번의 단위연산을 수행하고, 알고리즘 BE 300127번의 단위연산을
행한다. 어떤 7 값부터 알고리즘 BI Woo] 좋아지는가?

14. 입력 크기가 7인 BAS 푸는 4191과 188라는 두 개의 알고리즘이 있다. 4101의 실행시간
은 7?마이크로세컨드01백만 분의 1초)이고, Alg2°] 실행시간은 1007 1087 마이크로세컨드
이다. 4401을 프로그램으로 구현하는데 4시간이 걸리고, 프로그램을 돌리는데 289] cpu
시간이 걸린다. Alege 프로그램으로 구현하는데 1$시간이 걸리고, 프로그램을 돌리는데 6
분의 CPU 시간이 걸린다. 프로그래머의 임금이 시간당 20,000원이고, CPU 사용료는 분당
50,000원이라 하면, 입력 크기가 500인 문제를 몇 번 시68로 돌려야 개발을 정당화(개발비

를 복구)할 수 있을까?

3
+>

1.438
15. f(n) =n? +3n°EO(n*) YS 직접 증명하시오. 즉 OM 29] BIS 사용하여 f(r) |
An?) 3 An’) 4 모두 속함을 증명하시오.

16. OS} 22] 정의를 사용하여 HSS 증명하시오.
6n? +20n © 0072" )이지만 6n? + 20n € 02(72”)이다.
17. 1.4.28 있는 차수의 특성을 사용하여 다음을 증명하시오.
577? +4n* +6n? +2n? +n+7 € O(n’)
18. p(n) =a,n* +a,_;n* 1 +...+ayn+ay 2432 하자. 여기서 a, > 0이다. 1.4.8절에 있는 차수
의 특성을 사용하여 p(n) O(n") YS 증명하시오.


===== PAGE 58 =====
0000000
연습문제  43

19. f(n) =3n* +10nlogn+1000n+dlogn +9999 함수는 다음 중 어느 복잡도 카테고리에 속
하는지 고르시오
(a) 0087) 00 0(0210687) (90 002) (0 00187)
(e) 0(2”)     (6) None of these

20. f(n) = (logn)? +2n+4n+logn+50 함수는 다음 중 어느 복잡도 카테고리에 속하는지 고
르시오.

(a) 0087)     (b) 0((1087)”)     (c) O(n)     (d) A(nlgn)
(e) 0(n(lgn)”) (e) None of these
21. 702) =7+77+ㅜ27+7"함수는 다음 중 어느 복잡도 카테고리에 속하는지 고르시오.
(a) O(n    (b) 0(n?)   (c) 0(n?)   (d) A(nlgn)
(6) 8(n*) (6) None of these
22. 다음 함수를 복잡도 카테고리별로 묶으시오.
ninn      (Ig n)?      5n?+7n      n?!?
n!     20    4”    n” n™+ilnn
pen      Ig(n!) (ign)! Vn e”™ = 8n4+12~—-10" +n

23. 1.4.2절에 있는 차수의 특성 중에서 특성 1 2, 6, 7S 확립(유도)하시오.

24. O, 2, 0, 0를 점근적으로 비교할 때 Bb}4\(reflexive), 대칭적(6/0006010), #°]A(tran—
sitive) 성질을 설명하시오.

25. 입력 크기가 7=1,000인 문제를 푸는데 Ho] 걸리는 컴퓨터를 가지고 있다고 가정하자.
지금 가지고 있는 컴퓨터보다 11000배 빠른 새 컴퓨터를 산다면 1분 안에 실행할 수 있는
입력 크기는 알고리즘의 시간복잡도가 다음과 같을 때 각각 어떻게 될까?

(a) T(n)
(b) T(n)=n3
(c) T(n)=10"

n

26. 정리 13S 증명하시오.
27. 다음 각 항의 정확성을 증명하시오.
(a) Ign © O(n)
060 n © O(nlgn)
(0 nlgn € O(n?)
0) Pawo)
(e) lg? n € o(n®*)

추가 문제

28. 시간복잡도가 O(2") 인 알고리즘 AS 사용하여 입력크기가 302] 문제를 1분 안에 풀 수 있


===== PAGE 59 =====
44

chapter 1

29.

30.

31.

32.

석, 차수

A

알고리즘: 효율,

다. 그런데 이보다 두 배나 큰 입력을 1분 안에 풀어야 한다. 더 빠른 (그리고 더 비싼) 컴퓨
터를 사면 이 문제를 해결할 수 있으리라 생각합니까?

다음 알고리즘을 이해하고 아래 문제에 답하시오.
for (7 = 15 7 <= 1152) 7 ++)
cout << 1;
for @ = 2; 7>= 40 i --)
cout << 2;

(a) n=2, n=4, ㅠ=6일 때 결과를 각각 예측하시오.
06) 시간복잡도 710/)을 구하시오. 입력 n& 8의 배수로 가정해도 좋다.

다음 알고리즘을 이해하고 아래 문제에 답하시오.
j=l;
while (j <= 2 /2) {
7= 1;

while (i <= 7 ) {
cout 70 2;
tates
}
ptt
}
(a) n=6, n=8, ㅠ=10일 때 결과를 각각 예측하시오.
00) 시간복잡도 T(n)S 구하시오. 입력 nz 의 배수로 가정해도 좋다.
다음 알고리즘을 이해하고 아래 문제에 답하시오.
for (.7 = 28, 7 © nm; t+) {
for (f=O; 7 <n) {
cout (i «7
f=j + ln/4

|

(a) n=4, n=16, n=32 일 때 결과를 각각 예측하시오.

06 시간복잡도 710)을 구하시오. 입력 7은 4의 배수로 가정해도 좋다.

아래 중첨루프(206660 loop)2] 시간복잡도 T(n) 2? BE 경우를 다 고려하면 너무 복잡해
지므로 no] 8의 거듭제곱이라고 가정하고 풀어보자. 즉, 어떤 YO] 정수 *에 대해서 7=2*
이다.


===== PAGE 60 =====
for (7=1; 7<= i++) {
J=D;
while (j)>=1) {
«while 루프 몸체 > //00) 소요
J=L7/2);

}

33. n7H 서로 다른 양의 정수 리스트가 주어질 때 그 BASS 크기가 각각 0/27} 되게 두
개의 부분 리스트로 분할하되 두 부분 리스트의 정수의 합의 차이가 최대가 되도록 분할하는
알고리즘을 작성하고, 시간복잡도를 구하시오. no] 29) 배수라고 가정해도 좋다.

34. 아래 SAF (nested 1002)의 시간복잡도 T(n) 2? 모든 경우를 다 고려하면 너무 복잡해
지므로, no] 8의 거듭제곱이라고 가정해도 좋다. 즉, 어떤 양의 정수 *에 대해서, n= ole,

7=2;
while (7 >= 1 ) {
Jats
while (j <= 2) {
(while 루프 몸체 > //00) 소요
7=2ㅋ7:
}
i=[i/2] ;
}
35. 다음 알고리즘을 이해하고 아래 물음에 답하시오.
int add_them (int 2 , int A[] )
{
index i, j, 4
J=0;
for (f=1;7Gn H+)
f=Z rally
k=1;
for (7=1;37<=n i++)
k=k+k
return j + k

}
36. 다음 알고리즘을 이해하고 아래 물음에 답하시오


===== PAGE 61 =====
46

chapter 1

37.

38.

39.
40.

41.

42.

알고리즘: 효율, 분석, 차수

A

int any_ equal ( int n, int A[][] )
{
index i, j, 4, m
for (7=1; 7 (=n; i++)
for (j=l; 7 En; jtt+)
for (k=1;k En; kt+)
for ( 22 = 1 ; 22 <= 2 ; mtt+)
if (A[i] [ 7 ]==4[ 4] | 2 ] && ! ( ==4 && j==m))
return 1 ;

return 0 ;

}

(a) (ㅠ>1 이라고 가정하고) 알고리즘의 최선 시간복잡도를 구하시오.
(b) 알고리즘의 최악 시간복잡도를 구하시오.

(9) 알고리즘의 HVS 향상시키시오.

(0) 알고리즘이 0을 내주는 경우 배열 가 가지는 성질은 Belelz
(6) 알고리즘이 1을 내주는 경우 배열 av} 가지는 AALS 무엇인7
"을 p# 나누어 나머지를 계산하는 Ollgn) 알고리즘을 작성하시오. 모든 경우를 다 고려
하면 너무 복잡해지므로, no] 29] 거듭제곱이라고 가정해도 좋다. 즉, 어떤 양의 정수 *
대해서, ㅠ=얀이다.

어떤 함수가 다음 집합에 속하는지 WHS 설명하시오.
(a) nO
(b) O(n™))

(0 O(n™))
함수 f(n) =|r’sinn|e Oln)= An) = 아님을 증명하시오.

f(n) Ft g(n)& 점근적으로 양의 함수라고 가정하고 다음을 증명하시오.

(a) f(n) +g9(n)] O(max(f(n)), g(n))

(b) P’ (n)EQ(F(n))

(©) f(n) +o(f(n)) EO(f(n)), 여기서 o( f(n)) H g(n) Eo(f(n))-& 만족하는 어떤 함수를
의미한다.

개 서로 다른 양의 정수 리스트가 주어질 때, 그 리스트를 크기가 각각 7/2가 되게 두 개의
부분 도 네자  두 부분 리스트의 정수의 합의 차이가 최소가 되도록 분할하는 문
AS                    JS}, 시간복잡도를 구하시오. no] 29] 배수라고 가정해도 좋다.

알고리즘 1.707번째 피보나찌 항 구하기, 반복)은 nol] 대해서 1차이다. 그러나 이 알고리즘
이 1차시간 알고리즘일까? 1.3.1절에서 입력크기를 입력의 크기로 정의하였다. 7번째 피보
나찌 항의 경우, no] 입력이고, 7을 부호화하는데 필요한 비트의 AS 입력크기로 사용할
수도 있다. 이렇게 재는 경우 64의 크기는 1164=06이 되고, 1024의 크기는 181024 = 100]



===== PAGE 62 =====
43.

. 알고리즘 1,7] 입력크기에 관하여 지수시간임을 증명하시오. 또한 7번째 피보나찌 항
AAS 일고리즘은 출력크기가 입력크기에 대하여 지수이기 때문에 지수시간 알고리

이

일 수밖에 USS 증명하시오. 입력크기 관련 사항은 9.9절을 참고하시오.

aly 00 무

알고리즘 1.60번째 피보나찌 항 구하기, 재귀)의 시간복잡도를 구하시오(연습문제 34 참
).

이

연습문제 1~7에서 작성한 알고리즘의 정확성을 증명할 수 있을까?


===== PAGE 63 =====
Chapter 2

uz
분할정복

Oo]   책에서 우리가 처음 배울 알고리즘 설계 기법은 분할정복(01106-800-00ㅁ-

0460)이다. 1805년 1월 291 아우스터리츠 전투에서 프랑스 황제 나폴레옹이 시
도했던 탁월한 전략에서 따왔다. 오스트리아-러시아 연합군은 나폴레옹의 군대보다
15,000명 정도 많았다. 오-러 연합군은 프랑스군의 우측면에 대규모 공격을 감행해오고
있었다. 공격을 예상한 나폴레옹은 오-러 연합군의 중앙으로 쳐들어가서 병력을 둘로 갈
라놓았다. 둘로 갈라진 병력은 개별적으로는 나폴레옹 군대에 비해서 규모가 작았기 때
문에 참패를 당하고 퇴각하지 않을 수 없었다. 대규모 병력을 두 개의 소규모 병력으로
갈라놓고 두 소규모 병력을 각각 점령함으로써 나폴레옹은 대규모 연합군에 승리할 수
있었다.

분할정복 전략을 문제의 입력사례에 적용하여 문제를 풀 수 있다. 즉, 문제의 입력사례
를 두 개 이상의 작은 입력사례로 분할한다. 분할한 입력사례의 답을 바로 얻을 수 있으
면, 원래 문제의 답은 얻은 답들을 통합하여 구할 수 있다. 분할한 입력사례가 여전히
커서 바로 답을 구하지 못하면 그보다 더 작은 입력사례로 다시 분할한다. 바로 답을 구
할 수 있을 만큼 충분히 작아질 때까지 입력사례를 계속 분할한다.


===== PAGE 64 =====
50

chapter 2 분할정복

분할정복은 하향식(600ㅁ-00\20) BAS] 방식이다. 즉, 문제의 상위 입력사례의 해답
은 하위의 작은 입력사례(들)의 해답을 가지고 구한다. 재귀함수가 작동하는 원리가 바로
이렇다. 문제풀이 중심으로 재귀함수를 작성하고, 해답을 어떻게 얻는지에 대한 세부사
항은 (스택 조작을 통해서) 시스템이 알아서 하도록 맡긴다. 분할정복 알고리즘을 설계할
때도 보통 이런 식으로 사고하고, 알고리즘을 재귀로 작성한다. 후에 재귀 알고리즘은
효율적인 반복 알고리즘으로 변형할 수 있다.

먼저 이분검색 알고리즘을 분할정복으로 설계해보자.

2.1 이분검색

1.8절에서 공부한 알고리즘 1.5는 WAiteration)S 이용한 이분검색 알고리즘이다. 재귀
함수의 재귀 SSS 분할정복의 하향식 문제풀이 방식과 원리가 같다. 이 절에서는 이분
검색 알고리즘을 재귀60490피로 설계해보자. (비내림차순으로) 정렬된 배열을 분할정
복으로 어떻게 이분검색을 할까? 먼저 배열의 정 가운데 MAS 키 를 비교한다. 만약
같으면, 원소를 찾았으므로 알고리즘을 종료한다. 만약 다르면, 배열을 이미 비교한 원소
를 기준으로 반으로 분할한다. 만약 <가 가운데 원소보다 작으면, 왼쪽 배열에서 찾아야
한다. 그렇지 않고 2가 가운데 원소보다 크면, 오른쪽 배열에서 찾아야 한다. 왼쪽 또는
오른쪽 중 원소가 있을 해당 반쪽 배열의 정 가운데 원소와 다시 비교한다. 만약 같으면
원소를 찾았으므로 알고리즘을 종료한다. 만약 다르면 그 반쪽 배열을 또 반으로 분할한
다. 를 PAY 가 그 배열에 없다고 SA 때까지 이 절차를 계속한다.

요약 정리하면 이분검색의 절차는 다음과 같다.

rt 정 가운데 원소가 같으면, 찾았으므로 종료한다. 다르면,

1. [분할] WSS 정 가운데 ALS 기준으로 반으로 분할한다(4006). 가 가운데 원
AMC 작으면 왼쪽 배열을 선택한다. 2가 가운데 원소보다 크면 오른쪽 배열을 선
택한다.

2, [정복] 선택한 반쪽 HSS 정복한다. 즉, 선택한 반쪽 배열에 x7} 있는지 재귀적으
로 이분검색한다.

3, [취합] 선택한 반쪽 배열에서 얻은 답이 최종 답이다.

이분검색은 분할정복 알고리즘 중에서 가장 간단한 부류에 속한다. 왜냐하면 입력사
례를 분할하여 해답을 구하고, 결과를 취합할 필요가 없기 때문이다. 입력사례의 최종
답은 분할하여 선택한 작은 사례의 답과 같다. 예를 가지고 구체적으로 이분검색을 이해
해보자.



===== PAGE 65 =====
Pal   이분검색

won

51

* 예제 21 x= 180]! 다음과 같은 배열이 있다고 가정하자.
10 12 19 14 18 20 25 27 30 35 40 45 47
t

가운데 아이템
1. [분할] 배열을 분할한다. 2 < 25이기 때문에 왼쪽 배열에서 검색한다.
10 12 13 14 18 20
2, [정복] 왼쪽 배열에 27} 있는지 결정한다(왼쪽 배열을 재귀적으로 정복한다).
예, ce 왼쪽 배열에 있습니다.
3. [취합] 왼쪽 배열에서 얻은 답으로 전체 배열에 대한 답을 구한다.
예, 7는 왼쪽 배열에 있습니다.

2번째 단계에서 반쪽 배열에 대한 해답은 재귀적으로 구해온다고 단순히 가정했다. 그
해답을 어떻게 구하는지 자세히 설명할 필요가 없는데, 여기에 재귀 알고리즘의 비밀이
숨어있다. 분할정복으로 재귀 알고리즘을 개발할 때 꼭 고려해야 할 사항은 다음과 같다,

* 분할한 작은 입력사례의 답으로부터 전체 입력사례의 답을 구하는 방법을 고
* 더 이상 분할이 불가능한 입력사례를 판단할 종료조건을 정한다.
* 종료조건을 만족하는 경우 답을 어떻게 구하는지 정한다.

안타:

해답을 어떻게 구하는지에 대한 세부사항은 염려할 필요가 없다(컴퓨터의 경우 스택
조작에 의해서 이루어짐). 이런 세부사항들을 고민하면 오히려 재귀 알고리즘의 설계를
방해한다. 그림 21 잘 따라가 보면 이분검색 알고리즘이 어떻게 작동하는지 구체적으

로 알 수 있다.

재귀로 작성한 이분검색 알고리즘을 보자.

ㆍ알29즘 21 이분검색 재귀

문제 : 원소가 7개인 정렬된 배열 So] 검색키 2가 있는가?

입력 : 양의 정수 n, 정렬된(비내림차순) 배열 SHE 1부터 까지), 검색키 7

출력 location, SA] x2] 위치(만약 가 sol] 없으면 0)

index /ocation (index 70, index high)

{

index mid ;

if low > high)
return 0 ;
else {


===== PAGE 66 =====
52

chapter 2 분할정

mid = |(low + high)/2 |;

if (x == Smid)

return mid

else if (x < S'[mid))

return Jocation (low, mid —1) ;

else

return location (mid + 1, high) ;

n, S, c= location 함수의 파라미터로 두지 않았다. 왜냐하면 알고리즘 실행 중 재귀
SSS 해도 이 값들은 변하지 않는 상수기 때문이다. 재귀 호출하면서 값이 변하는 변수
만 재귀 알고리즘의 파라미터로 둔다. 그렇게 하면 재귀 알고리즘이 좀 더 말끔해져서
좋기도 하지만 저장공간을 절약할 수 있다는 점이 더 실질적인 이유이다. 재귀 알고리즘
을 실제로 구현할 때 재귀 호출이 일어날 때마다 전달되는 변수들은 복사하여 저장해 두
어야 하므로 그만큼 저장공간이 필요하다. 상수 HS 반복 저장하는 건 명백한 공간 낭비
이다. 배열 상수인 경우 낭비가 특히 더 심할 수 있다. 배열의 SAS 전달하여 낭비를
줄일 수도 있다. 만약 0++로 구현하면 HSS 저절로 AAS 전달하고, 예약어 constS
앞 붙여두면 배열의 내용이 변하지 않음을 보장해준다. 그러나 이런 세부사항을 재귀 알
고리즘의 의사코드에 적어두는 건 알고리즘이 어수선해지고 명확성도 떨어지므로 지양
하도록 하자.

10 12 13 14 18 20 25 27 30 35 40 45 47

x< 250/982 왼쪽

배열을 선택한다.      ×를 25와 비교한다.

Y

10 12 13 14 18 20

xS 137} 비교한다.

한
×>13이므로 오른쪽
배열을 선택한다.

v

14 18 20

XS 182} 비교한다.


===== PAGE 67 =====
@0@00000 0
2.1 이분검색  53

재귀 알고리즘의 구현 방식은 언어에 따라서 다를 수 있다. 예를 들어, 0++로 구현한
다면 상수값을 모두 파라미터로 전달해도 문제없다. 사용 언어에 따라 클래스로 구현할
수도 있고 재귀 호출해도 변하지 않는 상수 변수를 전역변수(10081 variable)= 정의할
수도 있다. 이 책에서 알고리즘을 후자의 방식으로 표현하므로, 후자의 방식을 어떻게
구현하는지 공부해보자. SA 2는 전역변수로 정의한다. F 배열의 원소 개수인 n& 6의
길이를 재서 항상 구할 수 있으므로 따로 변수로 정하지 않는다. 알고리즘 2.1의 location
함수는 맨 바깥에서 다음과 같이 호출한다.

locationout = location(1, n);

호출 이후에 더 이상 연산이 없는 재귀 SSS 꼬리 AA (tail-recursion)z}a1 한다.
이분검색 재귀 알고리즘은 꼬리 재귀이기 때문에 1.2절에서 보았던 반복 알고리즘으로
변환하기 수월하다. 앞에서 언급한 대로, 이 알고리즘을 재귀로 작성한 이유는 입력사례
를 더 작은 입력사례들로 분할하는 분할정복 절차를 명확하게 설명해주기 때문이다. 특
히 꼬리 재귀는 재귀 호출 종료 후 해야 할 작업을 스택에 저장해 둘 필요가 없어서 저장
SUS 상당히 절약할 수 있다. 함수 /가 함수 GS SSA 때 /의 중간계산(6600108)
결과는 활성레코드(30018\410ㅁ records) 스택에 저장해둔다. 만약 0가 다른 함수 /,를 호
출하면, 0의 중간계산 결과도 마찬가지로 스택에 저장해둔다. A ABS 끝내고 호출한
g= 돌아오면, 활성레코드를 스택에서 꺼내어 남아있던 AALS 완결한다. 재귀 함수의
경우 스택에 넣어두는 활성레코드의 개수는 재귀 호출 횟수(재귀 호출에 의해서 도달된
깊이)와 같다. 이분검색의 경우 스택은 최악의 경우 oF @7+1의 깊이까지 쌓인다.

꼬리 재귀를 반복형으로 변환하는 또 다른 이유는 스택을 쓸 필요가 없어서(단지 상수
를 곱하는 정도지만) 실행속도가 빠르기 때문이다. LISP 부류의 언어는 대부분 꼬리 재귀
코드를 반복형으로 자동 변환하므로, 수작업으로 꼬리 재귀 코드를 반복형으로 교체할
이유가 없다.

이분검색 알고리즘은 일정 시간복잡도 분석이 맞지 않으므로 최악의 경우를 고려하여
분석한다. 1.8절에서 약식으로만 분석해 보았으므로, 여기서는 제대로 정밀하게 분석해
보자. 알고리즘 2.1을 분석하지만 알고리즘 1.5와도 관련이 있다. 재현식 푸는 방법을 잘
르면 부록 BRE] 먼저 공부해야 한다.

i

최악 시간복잡도 분석(이분검색 재귀)

HES 검색하는 알고리즘에서 가장 비용이 많이 드는 연산은 보통 검색 키와 배열 원소를
비교하는 연산이다. 따라서 단위연산과 입력크기는 다음과 같다.

단위연산 : 와 ,9[7780|의 비교

입력크기 : 배열 원소의 개수, n

먼저 no] 29] 거듭제곱인 BES 분석한다. 가 S[mid]9} 다른 경우, location BPS



===== PAGE 68 =====
@0000000
54    chapter 2 분할정복

호출하면 단위연산을 두 번 실행한다. 그러나 어셈블러 언어로 한 번만 비교하도록 효율적
인 구현이 카능하므로, 한 번만 비교한다고 가정해도 무방하다. 1.8절에서 Sg 이분검
AYO) 약식 분석에서도 같은 논리로 한 번만 비교하는 걸로 하고 계산했었다. 1.3절에서도
얘기했듯이 단위연산은 최대한 효율적으로 구현한다고 가정해도 무방하다.

최악의 경우가 가 배열의 어떤 원소보다도 큰 경우이다. no] 29] 거듭제곱이고 가
배열의 어떤 원소보다 크면, 재귀 호출을 할 때마다 입력사례의 크기가 반으로 줄어든다.
예를 들어, n= 16이면, 7/20=|(1+16)/2]=8이다. 27} 배열의 모든 원소보다 크므
로 오른쪽 8개 원소가 재귀 호출의 입력이다. 비슷하게 오른쪽 끝 4개 원소가 두 번째 재귀
호출의 입력이고, 이런 식으로 계속된다. 결과적으로 AAAl(recurrence)2 다음과 같다.

W(n)=     {2     +
재귀 호출에서 나머지 부분에서
비교 횟수         비교 횟수

이상 비교할 대상이 없다는 뜻이다). 그러므로 170)은 1이다. 따라서 재현식을
하수

5
로.
ㅣ
럭

(2+ 1, n> 1이고 no] 29] 거듬제곱인 경우

이 MAAS 부록 Be] 예제 8.1에서 푼다. 해답은 다음과 같다.
W(n)=lgn+1
no] 29] 거듭제곱이라는 제한을 없애면 다음과 같이 된다.
W(n)= lg n] +1 € 008 7)

여기서 Ly Fe 보다 작거나 같은 최대 정수를 의미한다. 이건 연습문제로 풀어보기 바란다.

@  2.2 yaya

쌍방 By (two-way 2ㅁ6ㅁ8108)이란 정렬된 배열 두 개를 정렬상태를 유지하면서 하나로
합치는 것이다. BW (merge)S 이용하여 임의의 WSS 정렬할 수 있다. 예를 들어, 원소
가 16개인 임의의 WSS 정렬해보자. WSS 정확히 반으로 분할하여 각각 따로 정렬한
뒤 합병하여 정렬된 배열을 만들 수 있다. 반으로 분할하여 원소가 8개인 배열도 같은
방법으로 반으로 분할하고 각각 따로 정렬한 뒤 합병하여 정렬할 수 있다. 이런 식으로



===== PAGE 69 =====
@‥ㅎ00000 0
2.

계속 반으로 분할하다 보면 언젠간 원소가 하나인 배열이 될 텐데, 하나짜리 배열은 물어
보나마나 정렬된 배열이다. 이 절차를 “합병정렬04018080[0)"이라고 한다(편의상 ne 3
의 거듭제꼽으로 가정하고). 원소가 nel WAS 다음과 같은 절차로 합병정렬한다.

1 분할 : 배열을 반으로 분할한다. 분할한 배열의 원소는 각각 2/2개이다.
2. 정복 : 분할한 배열을 각각 따로 정렬한다(배열에 원소가 2개 이상이면 합병정렬을
8. 취합 : 정렬한 두 배열을 합병하여 정렬한다.

실례를 가지고 합병정렬을 이해해보자.

*예제 22 다음 배열을 정렬해보자.
27 10 12 20 25 13 15 22

1. 배열의 분할:

27 10 12 20, 25 18 15 22
2, 분할한 배열을 따로 정렬:

10 12 20 27,18 15 22 25
3. 정렬한 배열을 합병:

10 22 13 15 20 82 25 27

두 번째 단계에서는 문제해결 수준에서 사고하고 분할한 배열에 대한 답은 안다고 가
& 더 자세히 살펴보면, 그림 2.2는 합병정렬 알고리즘의 수동 실행 절차를 보여
준다. 종료조건은 배열의 크기가 1이 된 경우이고, 바로 그 시점에서 Sg] 시작된다.

ox
ro
=

OSG 2.2 합병정렬

문제 : 7/개 MAS 비내림차순으로 정렬
입력 : 양의 정수 7, 배열 5(인덱스는 1부터 까지)
출력 : 원소를 비내림차순으로 정렬한 배열 9

void mergesort (int 2, keytype 의 ])
{
if (nm > 1) {

const ink = | 2/21, eee 2 2s
keytype U[1.. A], V[1.. m];
copy S{1] through 91 4] to U1] through UA];
copy 의 £+1] through S{ 2] to V[1] through Vm];
mergesort(h, U) ;
mergesort(m, V) ;



===== PAGE 70 =====
chapter 2 분할정복

56

10 12 20 25 13 15 22

27

15 22
. \

13

25

IH

/

ill
IH

22

15

13

25

20

\

12

10 12

27

20

IH

[

10

27

분할

22

15

i

H0
101

13

20

12

|

#0
101

10

12 18 15 20 22 25 27

10

lo
a
nN
A
0 ie
2
0
=
0
iol
NR
원
=
에 | ~
nN
에
ㅇ
은

merge(h, m, U, V, S);

}

분석해야 한다.

성하고

먼저 작

즈으
ue

고리

oO}
=

ey
=

Ｌ

iol

a 2.3

> 알고리

|나로 합병

ㅎ

: 정렬된 배열 두개를 정렬상태를 유지하면서

제

므
~

<|

a

터 AMA), 정렬된 배열 (인

|스는 1부

(브

1부터 까지)

es
| 빼지

1부터 2 +7ㅠ까지)

eS
| a

점

배열 SA

원:

: US 의 원소를 모두 포함하여 정렬

iis

xf



===== PAGE 71 =====
void merge (int A, int m, const keytype 01],
const keytype V[],
keytype 5[])

{
index i, j, k
a — ly ee = 1:
while (i <= 42 && j <= m){
if (Ui] < 02] ) {
jk] = U4);
Ps
}
else {
Sk) = Vs);
Itt}
}
Bt;
}
if (7 > A)
copy V[j] through V[ m] to S[k] through 91 A+m] ;
else
copy Uji] through U[ 4] to S[ 4] through S{ A+m] ;
}

@ 표 2.1 두 개의 배열 //와 ve

하나의 배열*로 합병하는 예

U             V                         (결과)
10 12100 27 | 1315 2225 | 10
10122027 | 13152225 | 1012
1012 2027 | 18152225 | 101213
10 12 20 27 | 13 15 2225 | 10 12 13 15

10 12 20 27    13 15 22 25

10 12 13 15 20

10 12 20 27    13 15 22 25

10 12 13 15 20 22

NLD 00] = | = | 52 | 다 |e

10 12 20 27    13 15 22 25

10 12 13 15 20 22 25

10 12 20 27    13 15 22 25

10 12 13 15 20 22 25 27 < 최종값

* 비교 원소는 Fe 글씨체


===== PAGE 72 =====
@0@0 0 0 ee
58    chapter

- @
@

연산과 입력크기는 다음과 같다.
단위연산 : Uli] 9} 『/]의 비교

입력크기 : 두 입력 배열의 원소 개수, /.와 ㅠㅠ

최악의 경우는 := +1이고 j= mel 상태에서 루프를 빠져나가는 경우이다. 예를 들면,
의 앞 ㅠ- 1개 원소는 모두 로 먼저 옮기고 US AW ASS 모두 6로 옮긴 직후 이

런 상황이 발생한다. 따라서
Wlh,m)=h+m-1

이제 합병정렬을 분석해보자.

단위연산은 22@86에서 일어나는 비교연산이다. 비교 횟수는 와 mst 함께 증가하고, A
와 m2 nt 함께 증가하므로, 단위연산과 입력크기는 다음과 같다.

단위연산 : 2@86에서 일어나는 비교연산

입력크기 : 배열 SQ] 아이템의 수, 7

총 비교 APE US 입력으로 mergesortS 재귀 호출하는데 실행하는 비교연산의 횟수
와 VS 입력으로 mergesortS 재귀 호출하는데 실행하는 비교연산의 횟수와 merges

호출하여 실행하는 비교연산의 횟수의 합이다. 따라서 다음과 같다.

W(n)=    Wh) + Wim) + htm-i1
US 정렬하는데      를 정렬하는데        합병하는데
걸리는 시간 걸리는 시간         걸리는 시간

먼저 no] 29] 거듭제곱인 경우를 분석해보자. 이 경우에는 다음과 같은 등식이 성립한다.


===== PAGE 73 =====
22 합병정렬      59
W(n) 대한 재현식은 다음과 같다.
W(n) = w{2|+ W{2 | n-1
= {2 +n-1
emer  이면, 종료조건이 만족하고 WIS 없다. 그러므로 1(1)은 0이다. 결과적으

Xx
=.
ㅣ
i)
=

그 |+ ㅠ-1, n> 1이며 은 29] 거듭제곱

이 재현식은 부록 8의 예제 8.19에서 푼다. 해는 다음과 같다.
W(n)=nlgn—(n—1) € O(nlg n)
n©| 22] 거듭제곱이 아니면, 재현식은 다음과 같은데, 어떻게 이런 결과를 얻게 되는지는
연습문제로 풀어보자.

Wn)= W |] + 써주 171

여기서 fy |와 Lyle 각각 올림수연산(69118, 크거나 같은 최소정수)과 내림수연산

(floor, 작거나 같은 최대정수)이다. 올림수연산과 내림수연산 때문에 정확하게 계산하기

는 어렵다. 그러나 부록 BS] 예제 B.259} 같이 귀납법을 사용하면 W(n)o] nol 대해서

감소하지 GSS 증명할 수 있다. 그러므로 부록의 정리 Bao] 따라서 다음이 성립한다.
W(n) € O(nlg n)

AVALEAAin-place sort)& 입력을 저장하는데 필요한 장소 이외의 추가적인 저장장
소를 사용하지 않는 정렬 알고리즘이다. 알고리즘 2.0% 제자리정렬이 아닌데, 그 이유
는 입력 배열 6 이외에 배열 VI} VS 추가적으로 사용하기 때문이다. 만약 4@<에서
(/와 V 배열이 변수 파라미터(주소로 전달)라면, mergeS SH 때 이 배열들의 복사
BS 만들 필요가 없다. 그러나 mergesoreS 호출할 때마다 배열 VS} VS 새로 만들어
OF 한다. 맨 처음 SH 때 이 두 배열의 원소 개수 합은 대략 /이고, 다음에 재귀 호출
할 때 두 배열의 원소 개수 합은 대략 7/2이고, 다음에 재귀 호출할 때 두 배열의 원소
개수 합은 대략 7/4이고, 일반적으로 각 재귀 호출 시 두 배열의 원소 개수 합은 바로
전 호출 시의 반 정도이다. 그러므로 추가적으로 만들어지는 배열 원소의 총 개수는 대략
n(1+1/2+1/44+...)=2n 정도이다.

알고리즘 8.8는 문제의 입력사례를 더 작은 입력사례들로 분할하는 과정을 명확하게


===== PAGE 74 =====
@eeee?e ®e
60   chapter 2 분할정복

> 알고리즘 2.4

void mergesort.

{

보여준다. 실제로 분할한 두 개의 배열(작은 사례)은 입력배열(원래 사례)을 가지고 만들
기 때문에 합병정렬을 소개하고, 분할정복을 설명하기에는 적절하다. 그러나 at 원소
를 가진 배열 하나만 추가적으로 있어도 합병정렬이 작동하도록 하여 알고리즘을 개선
하여 저장장소를 절약할 수 있다. 이는 입력 배열 SS 특정 형태로 조작하면 가능하다
개선한 다음 합병정렬 알고리즘은 알고리즘 2.1(재귀적 이분검색)과 유사한 방법을 사용
한다.

합병정렬 2

문제 : 7개 원소를 비내림차순으로 정렬

입력 : 양의 정수 7, 배열 .(인덱스는 1부터 까지)
출력 : 원소를 비내림차순으로 정렬한 배열 S

S

(index 70, index high)

index mid ;

if (low < high) {
mid = | (low + high)/2 |
mergesort2 (low, mid) ;
mergesort? (mid +1 , high ) ;
merge? (low, mid, high ) ;

> 알고리즘 2.5

값이 변하는 변수만 파라미터로 사용하는 관례에 따라서 nw} St mergesort? 프로시
저의 파라미터로 두지 않는다. 만약 배열 SS 전역적으로 정의하고 원소의 개수가 no]
면, 그 알고리즘에서 2209050772의 최초 호출은 다음과 같다.

mergesort2(1, 22);

mergesort22} 함께 작동하는 합병 알고리즘은 다음과 같다.

we 2
문제 : 합병정렬 에서 분할하여 Pas 배열을 합병
입력 : 인덱스 low, mid, high, 그리고 ,9의 부분배열(인덱스는 100부터 high),

1000 에서 7280까지 HSS] AE 이미 정렬되어 있고, mide] /207까지의 배열에
있는 원소도 마찬가지이다.
출력 : 원소가 비내림차순으로 정렬되어 있는 SQ] 부분배열(인덱스는 100 부터 highFAl)


===== PAGE 75 =====
     void merge2 (index 700, index mid, index high)
|     {
|       index i, j, k
      keytype Ullow .. high| —// 합병에 필요한 지역 배열
I= low; ./ = mid+1;k= low;
|      while (7 S mid && j < high ) {
|         if (S{ i] < Sy) {
Ok) = Si};
H+;
}
else {
Ok) = Sy] ;
i
}
싸+;
}
if (2 > mid)
move S{j| through S{ high| to U|k] through U| high] ;
else
move S{i] through S{ mid] to U|k] through U high] ;
move U|{ low] through U| high] to S{ low] through Sf high] ;

@ 2.3 Bags 설계방법
두 가지 분할정복 알고리즘을 자세하게 공부했으므로, 이제 분할정복 설계전략을 정리해
보자.
분할정복(010106-800-00ㅁ0460) 설계전략은 다음과 같은 절차로 이루어진다.
1, 문제의 입력사례를 하나 이상의 작은 입력사례로 분할한다.
2, 작은 입력사례들을 각각 정복한다(푼다). 작은 입력사례가 충분히 작지 않으면 재귀

3. 필요하다면, 작은 입력사례의 해답을 통합(6006100)하여 원래 입력사례의 해답을
구한다.

8번째 단계에서 '필요하다면'이라는 단서를 붙인 이유는 이분검색(알고리즘 2.1)과 같은
알고리즘에서는 분할한 입력사례를 하나만 쓰므로 해답을 통합할 필요가 없기 때문이다.

이제부터 분할정복 설계방법을 적용하는 사례들을 더 살펴보기로 한다. 앞으로는 이
설계전략(절차)을 따로 명시하지는 않을 것이다. 알고리즘을 따라가다 보면 절차는 명백
해지기 때문이다.


===== PAGE 76 =====
@0@00000 0
chapter 2 분할정복

62

2.4 빠른정렬(분할교환정렬)

* 예제 2.3

So}(Hoare, 1962)가 고안한 “빠른정렬(24080) 이라는 정렬 알고리즘을 공부해보자.
빠른정렬은 WSS 둘로 분할하고, 분할한 배열을 각각 재귀 SSE (recursively) 정렬하
여 합병하므로 합병정렬과 비슷하다. 그러나 빠른정렬은 WSS 분할하는 방식이 다르
다. 기준원소(01700를 선정하여 기준원소보다 작은 원소는 모두 왼쪽 배열로, 기준원소
보다 크거나 같은 Ase 모두 오른쪽 배열로 가도록 분할한다. 기준원소 AVS 중요하
지만, 편의상 일단 배열의 첫 원소를 기준원소로 잡자. 빠른정렬이 어떻게 작동하는지
예제 2.8을 공부하면서 이해해보자.

다음 WSS 정렬해보자.

소

15 22 13 27 12 10 20 25
1, 지준연손보다 작은 원소는 모두 AS 배열로, 큰 원소는 모두 오른쪽 배월로 가도록 배열을
분할한다.
기준원소
+
10 13 12 15 22 27 20 25

작은 수는              큰 수는
이쪽으로             이쪽으로
2, 배열을 각각 따로 정렬한다
기준원소

10 12 18 15 20 22 25 27

정렬완료      정렬완료

Ac
uct
=
ied
Jo,
rie,

JAES 어떤 순서로 나열하는지는 별로 중요하지 않다. 알고리즘의

한

핵심이 아닐 뿐 아니라 결과에도 JAS 주지 않기 때문이다. 위의 예제에서는 잠시 후
공부할 분할 알고리즘에 따라 원소를 나열하였다. 중요한 점은 기준원소보다 작은 원소
는 모두 왼쪽에 두고, 큰 원소는 모두 오른쪽에 둔다는 사실이다. 빠른정렬은 분할한 두

고
ne,
iho
Bt
Be
pra
고

호출하여 정렬한다. 원소가 하나뿐인 배열로 분할될 때까지 재귀 호출
을 계속한다. 원소가 하나밖에 없는 배열은 정렬할 필요가 없다. 예제 2.32 빠른정렬
알고리즘의 작동 사례를 보여준다. 그림 2.8은 빠른정렬을 수동으로 실행 추적할 때 취할
절차를 설명한다. 다음은 알고리즘이다.


===== PAGE 77 =====
15 | 22 13 27 12 #10 20 25

10      1

12                   15               22           27 25

그림 2.3 빠른정렬 알고리즘의 작동 사례. SSE 배열은 네모로 둘러 싸여 있음

FOP 26 빠른정렬
문제 : 비내림차순으로 원소가 //개인 배열을 정렬
입력 : 양의 Aen, 배열 SIAL 1부터 7까지)
x
2

력 : 비내럼차순으로 정렬된 배열 6

void quicksort (index 700, index high)

{
|       index pivotpoint ;
if (high > low ){
partition (low, high, pivotpoint ) ;
quicksort (low, pivotpoint — 1) ;
quicksort (pivotpoint + 1, high) ;
}
}

앞에서부터 해온 대로 과 SE quicksort 프로시저의 파라미터가 아니다. 알고리즘
이 SS 전역적으로 정의하도록 구현하고 no] ,ㅇ MA 개수라면, quicksort2] 최초 호
출은 test 같다.

quicksort(1, n);

배열      할하는 알고리즘은 7477402이다.

tho
A


===== PAGE 78 =====
64      chapter 2 분할정복
ORS 2.7 분할

제 : 빠른정렬에서 쓸 수 있도록 배열 SS 분할
: 인덱스 low} high, 배열 SHA] low FE] /70/까지의 부분배열
: 100부터 high) 인덱스로 된 6의 부분배열의 기준점, pivotpoint

m+ ㅁ으 ro
Jz

J

void partition (index Jow , index high,
index& pivotpoint)
{

index 7 , j
keytype pivotitem ;

pivotitem = Sflow] ;                 // pivotitem® = 첫 원소 AA
i = low ;
for (7 = low + 1 ; 7 <= high ; 4+)
if (Sf i] < pivotitem){
Itt;
exchange S{i] and S{/] ;
}
pivotpoint = J] ;
exchange Sflow] and S{pivotpoint| ; // pivotitem 값을 pivotpoint| 저장

partition YUBSL 배열의 WAS 하나씩 차례로 점검한다. 기준원소보다 작은 원
소는 배열의 왼쪽으로 옮긴다. 표 2.9% 예제 2.39] 배열에 partitions 적용한 사례를
보여준다.

이제 분할과 빠른정렬 알고리즘을 분석해보자.

@ 표 22 partition uals 실행사례*

7     J    Si] sl2] sz] sl[4) sis) 516] siz] sls)
=     =     15     22     13     27     12     10     20     28 <—-A gy
2      1      15     22     13     27     12     10     20     25
3      2      15     22     13     27     12     10     20     25
4      2      15    27     12     10     20     25
5      3      15     13     22     27     12     10     20     25
6      4      15     13    27    10     20     25
7      4      15     13     12    22    20     25
8      4      15     13     12     10     22     27     20     25
=      4    13     12    22     oy     20     88 “< 끝않

*
프
팀
rr
in
b>
er
이
ok

}게 표시했다. 바로 교환된 원소는 상자로 둘러싸여 있다.


===== PAGE 79 =====
0000000
24 빠른정렬(분할교환정렬)     65

경산 : 911] 와 pivotitem2] 비교

입력크기 : n=high—low+1 (부분배열 원소의 개수)
첫째 원소를 제외한 ASS 모두 비교하므로,
T(n)=n-1

여기서 n& 전체배열 의 크기가 아니라 부분배열의 크기를 나타낸다. partitions 처음
SST 때만 n& $2] 크기와 같다.

빠른정렬 알고리즘은 일정 복잡도 계산이 불가능하다. 따라서 최악의 경우와 평균의

단위연산 : 247220202에서 ,912]와 pivotitem2) 비교
입력크기 : nS 원소의 개수)
기이하게도 완전히 정렬된 배열     에셔  경우가 최악의 경우이다. 이유는 명백하다. 완
전히 cele 있으면, 첫째(기준) 원소보다 작은 아이템은 없다. 따라서 partitions 처음
호출할 때 기준원소 왼쪽으로 보낼 MALE 하나도 없고, /77082072/의 값은 1°] 된다. 재귀
호출할 때 iis pivotpoint= low 값을 받는다. 그러므로 배열은 왼쪽은 빈 배열 오른쪽은
길이가 1만큼 짧은 부분배열로 분할한다. 이미 정렬된 사례들로 재현식을 세우면 다음과
같다.
Tin)=    TO) + Tn-1) + n-1

왼쪽 배열을 정렬 오른쪽 배열을 za 분할하는데

하는데 걸리는 시간 하는데 걸리는 시간     걸리는 시간
여기서 Tn) OS 표시하는 이유는 이미 정렬된 경우 일정 시간복잡도를 따져야 타당하
다. 7(0)= 0이므로 다음과 같은 재현식을 얻는다.

T(n) = T(n-1)+n-1, 2 > 0

이 재현식은 부록 8의 예제 8.16에서 푼다. 해는
n(n—1)
2
(n—1)/2°] BS 알았다. 비록 직관적으로는 이게 우리가 얻을 수
있는 최악의 상태인 것처럼 BYEZ) 모르지만, 그래도 증명해야 한다. 모든 정수 nol 대

T(n)=

에
IS
412
on,
4o

스베
b>
ro
3


===== PAGE 80 =====
@000000 0
chapter 2 분할정복

66

해서 다음 부등식이 AAAS AYA (induction)S 사용하여 보임으로써 이를 증명한다.

Wn) < MAY)

귀납출발 : n=08 때
wo) =0 은

귀납가정 : 0 을 k< no] 성립하는 모든 《에 대해서 다음 부등식이 성립한다고 가정한다
Wk) < ae

귀납단계 : 다음 부등식이 성립함을 보이면 된다.

n(n—1)

Wn) <

어떤 no] 주어질 때 처리시간이 Wn) o] 되는 크기 //의 사례가 존재한다. 이 사례를 처리
. 때 AAS partition’) AAZ pivotpoint2| A peta! 하자. 크기가 2-1이고 7 - p
(2 -1)과 Win-p) B=, 다음과 같은

pain    는다
702) < Wp-1)+ Win-p)+n-1

“s (p~1)(p~2) | 00 2) 2- 1)
2           2

마지막 부등식은 귀납가정에 의해서 성립한다. 대수적(318007810/으로 식
= 인 BE pol 대해서 마지막 식은 다음과 같다.
n(n—1)
때     2
따라서 귀납법 증명이 완료되었다.
최악의 경우 시간복잡도는 다음과 같이 됨을 증명하였다.

fo)
n—-1)

가 1

ttlo

24 1<p

3

정렬된 AS 정렬하는 경우가 최악인데, 이유는 기준원소로 항상 첫째 MAS 선택
하기 때문이다. 따라서 거의 정렬된 배열을 정렬하는 경우, 첫째 원소를 기준원소로 주는
건 현명한 선택이 아니다. ?장에서 빠른정렬 알고리즘을 다시 공부할 텐데, 기
잘 선택하는 방법은 그 때 배우기로 하자. 그 방법을 사용하면, 정렬된 배열을
라도 최악의 경우가 아니다. 그러나 최악 시간복잡도는 여전히 7(01-1)/2이다.



===== PAGE 81 =====
v

2.4_빠른정렬(분할교환정렬)      67

최악의 경우로 따지면 알고리즘 2.6은 교환정렬(알고리즘 1.9)보다도 빠르지 않다. 그

러면서 왜 빠른정렬이라 했을까? Bato] 경우를 따져보면 of 빠른정렬이라고 했는지 이
해할 수 있다.

(빠른정렬)의 평균 시간복잡도 분석

단위연산 : partition) Sli] 2} pivotitem2] 비교
입력크기 : CHA 에서 원소의 개수)
배열의 원소가 순서없이 무작위로 흘어져 있다고 가정하자. WBA partitione] WHE
pivotpoint 값은 1부터 /사이의 입의의 수일 테고, 어떤 수가 되든지 HRS 모두 같다
이 가정을 믿을 수 없으면, 이 LAE LS 수 없다 따라서 평균 PEALE 가능한
순서조합을 정렬하는데 걸리는 시간의 평균을 구한다. 이 경우 평균 시간복잡도를
aie 재현식은 다음과 같다.

pivotpoint7}
pa ian

jad = [A(    p—1)+A(n—p)] + n-1           @ 0

p=

a

pivotpoint7} pd 때 Be 분할하는데
배열들을 정렬하는데 걸리는 걸리는 시간
평균시간

다음 등식의 성립여부 증명은 연습문제로 남긴다.
066 06621 an

이 AS 등식 (2.1에 적용하면 다음과 같다.

ee
PAS 7으로 곱하면 다음과 같다
0000)= 22]46-10+70-1)                (2,2)
등식 2.) ㅠㅡ1로 대치하면 다음과 같다.
(n—1)A(n~ 1) =2 AGI) + (n=) l—2)            (2,3)

등식 (2.9)에서 등식 (2.3) 빼면 다음과 같다.
nA(n)—(n—1)A(n—1)=2A(n—1)4+2(n—1)


===== PAGE 82 =====
68    chapter 2 분할정복
위 식을 다음과 같이 정리할 수 있다.
42(02) _ A(n—1) 4 2(n—1)
n+l on       n(n+1)
다음과 같이 놓으면
_ A(n)
on +1
다음과 같은 재현식을 얻는다
Qn  : 우바, n>0
ay = 0
부록 8의 예제 8.99의 재현식과 같이 이 재현식의 근사해는 다음과 같다.
a, ~ 2Inn
결론적으로 평균 시간복잡도는 다음과 같다.
A(n) = (n+1)2 ln n= (n+1)2(In 2)(Ig n)
= 1.38(n+1)lgn € O(nlgn)
빠른정렬의 평균 시간복잡도는 합병정렬의 시간복잡도와 차수가 같다. 합병정렬과 빠
른정렬은 7장과  ~ 책(1973)을 보면 더 상세히 공부할 수 있다.
@  2.5 FEzpas 행렬곱셈 알고리즘
알고리즘 1.4(행렬곱셈)는 행렬곱셈의 정의를 그대로 따라 두 행렬을 곱하였다. 곱셈 횟
수를 기준으로 구한 시간복잡도는 7이 행렬에서 열과 YO] 개수일 때 Tn) =n? YS
Sua, 덧셈 She eos EAE 수도 있다. 알고리즘을 약간 wa Se
횟수를 기준으로 분석하면 시간복잡도는 7(/,) =n? ㅡ-7/”인데, 연습문제로 증명해보기
바란다, 모두 시간복잠도가 @(0")이므로 nol 조금만 Aas 실용적으로 쓰기 힘들만큼
느려진다. 1969년에 F}EePa(Strassen) 2 곱셈을 기준으로 하든지 DA/MAS 기준
로 하는지 상관없이 시간복잡도가 3차보다 좋은 알고리즘을 발표하였다. 쉬트라썬 알고
즘을 공부해보자.
© 예제 2.4     두 개의 2x2 행렬 A} BI) Froduct)e CS 구한다고 가정하자. 즉

인 ve = ie oa s E |
08122       961 922       061 022


===== PAGE 83 =====
2.5 쉬트라썬의 행렬곱셈 알고리즘 69

쉬트라썬의 방법은 다음과 같이 놓았을 때,
m= (01 +ㅜ02761 + Bap)
7722 (ay, +ㅜ02270,

m3=  Ay (Dy      — byy )

M4 = Ag9 (by, — b,)
=n 00h
mma     — a1) (by, +By9)
ill     = gy) (By, + Boy)
B CE 다음과 같다.
C=  m,+m,—ms, +m,       m3 +Ms
My +m,      M,+M3—My+mMe

이 결과가 맞는지 연습문제로 증명해보자.

관적인 방법으로 두 개의 2x2 PBS 곱하려면 곱셈 8번과 G/M 4번이 필요

한 반면, FEES] 방법으로는 곱셈 7번과 GU a) 18번이 필요하다. 덧셈을 14번

더 하는 대신 곱셈 1번을 절약하였다. 별로 좋아진 것 같아 보이지 않는데, 사실 3×2

는 별로 성능향상의 효과가 없다. 곱셈의 교환법칙(6000246811019)을 쉬트라

}용하지 않았기 때문에 이 식은 4개의 부분행렬로 나눌 수 있는 큰 ㅎ

렬에도 ene 수 있다. 그림 2.4에서와 같이 행렬 4와 BS 먼저 분할한다. no} 29]
거듭제곱이라고 가정하면 행렬 A, 2 다음과 같은 4의 부분행렬을 나타낸다.

aay
r

=F
fo

표 프
뜨

※×

911 912 111 91,2/2

a.   Gi  eee  a
Ay =      21    22       fae
Qn /2,1  vee   An /2,n/2

FECA] 방법을 사용하여 다음을 우선 계산한다.
= (4 +ㅜ45272   11 + 256)

여기서 연산은 이제 행렬 덧셈과 곱셈이 된다. 같은 방식으로 MAMA 44;까지 계산한
다. 다음에는 CS 다음 식으로 계산하고,

<nl2—>
nl2\ Cy + 어2     Ait | At2     By, | By
worn nnse------ =  crore cdenece--] Xx  Secissiecleccice-
Coy 1 Cop      421 ㅣ 422      Boy ㅣ Bop

그림 2.4 72M! 알고리즘에서 부분행렬로의 분할 방식


===== PAGE 84 =====
@0 00000 0
chapter 2 분할정복

70

> 알고리즘 2.8

© 예제 2.5

004, = 424, + 44, - 44. + M,

Cio, Cy, Coo 비슷하게 계산한다. 마지막으로, 4 와 2의 Hel CE 네 개의 부분
렬 ({,를 통합하여 구한다. 이 절차는 다음 예제에서 설명한다.

행렬 4와 2가 있다.

1234       8912
15678     _ 13456
A= 19193   B= \7891
4567       2345

그림 2.53 보면 FEepa] 방법으로 어떻게 분할하는지 알 수 있다. AALS 다음과 같이 진행
된다.

M, =(Ay, + Ago) X (By 1 Bo)

=([sel+ eal) ([eal*[es])

[3 5], [1710
버러 이 ×부 」

행렬이 충분히 작아지면, 표준 행렬곱셈 방법으로 꼽한다. 이 예제에서는 7= 일 때 표준 행렬
곱셈 방법으로 곱한다. 따라서 a, 다음과 같다.

_13 5]. [1710
m=|53)x E 4

=| 3xX17+5xX7 3x1015x9 l= [sn 고
1LX17+13X711x10+13%*9   278 227

44;에서 2&,까지도 같은 방법으로 계산하고, 그 다음에 C1, Cro, Cy, CoS 계산한다. 이
네 개의 부분행렬을 합하면 C7} 된다.

이제 이 8의 거듭제곱일 때 ECPM] 방법을 이용한 알고리즘을 공부하자.

4+|E2}4l(Strassen)

문제 : no] 29] 거듭제곱일 때 2개의 nxn 행렬의 BS 구하시오.
입력 : 29) 거듭제곱인 정수 7, 2개의 nxn 행렬 AM B

t    12:34   89/12
2| Cy Cro     !
5617 8   38166
' 바바 aca 빠  =   8보오 투레gaa3   x   eae a
    1:2   7
G  C      |
aa ie   45:67   23:4 5


===== PAGE 85 =====
@0 @
2.5 쉬트라썬의 행렬곱셈 알고리즘 71

출력 : 4와 의 곱 ㅇ@

void strassen (int n
n X n_matrix A,
n X n_matrix B,
n X n_matrix& C)

  if (2 <= threshold)
표준 알고리즘으로 (= AX BE 계산한다;
else {
AS Aj, Aj, Ay, Ane 분할한다 ;
BS Bi, By, By, Bye 분할한다 ;
쉬트라센의 방법으로 C= Ax BE 계산한다 ;
// 재귀 호출의 예제
// strassen (n/2, Ay, + Ay, By + By, 44.) ;
}
}

2|A]Al(threshold)< strassen ZBA)AS 재귀 호출하는 것보다 표준 알고리즘을 사
용하는 A] 더 효율적인 지점이다. 2.7절에서 한계치를 구하는 방법에 대해서 알아본다.

coke ㆍ(쉬트라썬)에서 곱셈의 수의 일정 시간복잡도 분석
단위연산 : 곱셈 1회

입력크기 : 7 (행렬에서 행과 열의 수)
분석절차를 간단하게 하기 위해서 2개의 1x1 행렬이 될 때까지(이 시점에는 각 행렬의
수를 곱하면 된다) 계속 나누는 경우를 분석한다. 실제로 사용된 임계점은 차수에 영향을
미치지 않는다. = 1일 때 정확하게 곱셈을 한 번 실행한다. n> 1인두개의 nxn 행
렬이 있을 때, (n/2) x (n/2 ) Bas ?번의 재귀 BEE 하고, WMHS Bae

하지 않는다. 따라서 다음과 같은 재현식을 세울 수 있다.

이 > 1이며, 7은 8의 ASA
2600= Ｌ

이 재현식은 부록 BS] 예제 8.2에서 푼다. 그 해답은 다음과 같다.

T(n)= 728 ~ n?8! © O(n?!)

(쉬트라썬)에서 SU/MO| 수의 일정 시간복잡도 분석
단위연산 : 덧셉이나 wal 1회

+


===== PAGE 86 =====
72

chapter 2 분할정복

입력크기 : /,(행렬에서 행과 열의 수)

앞에서와 마찬가지로 2개의 1×1 행렬이 될 때까지 계속 나눈다고 가정한다. n= 1일 때
덧셈이나 WLS 실행하지 않는다. n> 1인 두 개의 nxn 행렬이 있을 때 (n/2) x (n/2)
행렬로 재귀 SSS ?번하고, (n/2)x(n/2) 행렬에서 덧셈과 WIS 18번한다. 9개의
(n/2) x (n/2) BAS 더하거나 텔 때 행렬 내부 원소들의 덧셈이나 WIS (n/2) a 실
행한다. 따라서 다음과 같은 재현식을 세울 수 있다.

T(n) = (24 12) n> 1이며 n& 29] 거듭제곱
270)=0

이 재현식은 부록 BS] 예제 8.20에서 푼다. 그 AES 다음과 같다.

T(n) = 6n'8" — 62? =~ 6n?*! - 6n? € O(n?*")

이 8의 거듭제곱이 아닐 때 앞의 알고리즘을 수정해야 한다. 간단한 수정방법 중 of
나는 원래 행렬의 행과 열에 OS 충분히 추가하여 BAS] 크기가 29] 거듭제곱이 되도록
하면 된다. 다른 방법으로는 재귀 호출마다 행과 열의 수가 홀수가 되면 0으로 된 행과
열을 하나 추가시킨다. HEepa969)2 다음과 같은 더 복잡한 수정방법을 제시하였다.
2*m AS] 행과 열을 가진 더 큰 행렬에 원래 행렬을 끼워 넣는다. 여기서 k= Lg n—4]
이고, m=|n/2*]+10]44,  sia 까지만 FEES] 방법을 사용하고,  erie
도달한 후에는 표준 알고리즘을 사용한다. 산술 연산(곱셈, 덧셈, Bel 총 횟수는
4.7n?*) aU} ASS 증명할 수 있다.

표 2.8에 no] 8의 거듭제곱일 때 표준 알고리즘과 HEE 알고리즘의 시간복잡도를

비교하였다. 재귀 SSS 발생하는 추가비용을 우선 무시하고, 곱셈 횟수로 따지면 쉬트
epal 알고리즘이 언제나 더 효율적이고, 덧셈과 wl 횟수로 따지면 no] 클 때 ae
알고리즘이 더 효율적이다. 재귀 SSH 추가로 발생하는 시간을 계산하는 분석 기술
2.7절에서 공부할 것이다.

쉬뮤엘 위노그라드(86046! \2008780)는 덧셈과 WS 15회만 수행하는 HEepa 알
고리즘의 BSS 개발했다. 자세한 내용은 850868810와 Bratley(1988)2] 책에 나와 있다.
이 알고리즘을 사용하면 D/A S 단위연산으로 하여 시간복잡도는 다음과 같다.

@ 표 2.3 nxn 행렬을 꼽하는 두 알고리즘의 비교

표준 알고리즘                    aeed 알고리즘

곱 셈                                 77"                                                                                     77^으

Bala]              72? ㅡ72?                                                    6n2*! —6n?



===== PAGE 87 =====
T(n) = 5n?®! — 57222

Coppersmith} Winograd(1987)= 곱셈을 단위연산으로 하여 시간복잡도가 O(n?**)
)수가 너무 커서 Heep 알고리즘보다 더

효율적이라고 보기 어렵다.

행렬곱셈을 하기 위한 알고리즘은 그 시간복잡도가 최소한 3차시간은 되어야 함은 증
명이 가능하다. 그러나 행렬곱셈을 %차시간에 할 수 있는지는 아직 모른다. 왜냐하면,
행렬곱셈을 하기 위한 차시간 알고리즘을 개발한 사람은 아직 없고, 그러한 알고리즘을
개발하기는 불가능하다고 증명한 사람도 없기 때문이다.

행렬의 YS 구한다거나 행렬식(00661040800을 찾는다거나 하는 다른 행렬관련 a
은 행렬곱셈과 직접 관련이 있다. 따라서 쉬트라벤의 행렬곱셈 알고리즘만큼 효율
행렬연산 관련 알고리즘들은 손쉽게 개발할 수 있다.

cS re

Pt

2.6

ru

정수 계산법

정수를 표현하는 저장공간의 용량을 초과하는 정수 연산을 해야 한다고 하자. 만약 유효
SAS 모두 보존해야 한다면, 부동소수점으로 표현을 바꾸어 MLS 해도 소용이 없다.

이 경우 유일한 대안은 소프트웨어로 정수를 표현하고 처리해야 한다. 분할정복의 도움
을 받아서 이를 성사할 수 있다. 이 책에서는 10진수 APS 중점적으로 다룬다. 그러나
고안한 방법은 다른 진수에도 사용할 수 있도록 손쉽게 변경할 수 있다.

2.6.1 큰 정수 표현 : 덧셈과 기타 1차시간 연산
큰 정수를 표현하는 직관적인 방법은 숫지 digit) 배열을 사용하는 것이다. 예를 들면, 정

5  4  3  1  2  7
S16] S15] Sl4l S13] So] Sia

양수와 음수를 모두 표현하기 위해서는 FS(sign)S 저장하는 배열 슬롯하나만 추가로
준비하면 된다. 0으로 양수를 표현하고, 1로 음수를 표현할 수 있다. 그리고 데이터타입
large_integerE 큰 정수를 표현하기에 충분히 큰 배열이라고 가정하자.

을 큰 정수의 숫자 개수라고 하면, 덧셈과 WANS 하는 1차시간 알고리즘을 작성하는
전 어려운 작업이 아니다. 단위 AALS 십진수(460081 0911 조작연산으로 정한다.
이 알고리즘을 설계하고 분석하는 작업은 연습문제로 남겨둔다. 추가로 다음 연산을 하
는 1차시간 알고리즘도 손쉽게 작성할 수 있다.

u x 10”   u divide 10”   u rem 10”


===== PAGE 88 =====
00000 0 0
74     chapter 2 분할정복

여기서 u 큰 정수, mS 음이 아닌 정수를 각각 나타내고, 0104106는 정수 Ue] RS

계산해주고, 『0은 정수 URIS] 나머지를 계산해준다. 이것도 역시 연습문제로 해보

기 바란다.
26.2 큰 정수 곱셈
큰 정수를 곱하는 간단한 2차시간 알고리즘은 초등학교에서 배운 방법을 그대로 쓰면 된
다. 그러면 2차시간보다 빠른 알고리즘을 개발해보자. 분할정복을 사용하여 7개의 숫자
로 된 수를 약 7/23개의 숫자로 된 두 개의 정수로 분할한다. 다음 두 ofS 보면 어떻게
분할하는지 바로 이해할 수 있다
567,832 = 567 ×10"+ 832
67H]          374             3개
9,423,723 = 9423 x<10°+ 723
7개            4개              3개

일반적으로 n& 정수 uo] 있는 숫자의 개수라고 하면, 그 정수 uS 다음과 같이 하나는
크기가 |7/21|이고 다른 하나는 [7/2]인 두 개의 정수로 분할한다.

4 =   a   x 10" +   y
개              |7/21|개                            Ln/2| 7

이렇게 표현하면, 위 식에서 me 다음과 같다.

m=|5
개의 숫자로 된 다음과 같은 두 개의 정수가 있다면,

24=2×10"”+?4

v=wxl0"+z

uv = (x& X10" + y)(w X10" +z)
= cw X10?" + (xz + wy) X 10” + yz

*예제 26 다음 연산 과정을 따라가 보자.
567,832 9,423,723 = (567 x 10° +832)(9423 x 10° +723)
= 567 X 9423 x 10° + (567 x 723 + 9423 x 832) x 10° +832 x 723


===== PAGE 89 =====
더 작은 정수들은 그보다 더 작은 정수로 분할되어 재귀로 곱해진다. 이 분할 과정은 임계점에
도달할 때까지 계속된다. 언젠가 표준방식으로 곱셈을 실행할 때가 온다.

숫자의 개수가 거의 같은 정수를 곱하는 경우로 이 마호 설명했지만, 숫자의 개수
차이가 많이 나는 경우에도 같은 방법을 적용할 수 있다. 단순히 7=[7/2]를 사용하여
두 수를 각각 분할하는데, 여기서 /은 Fo] 큰 정수의 Ar} 개수이다. 알고리즘은 다
음과 같다. 둘 중 SHU} 00] 되거나 정해놓은 임계점에 도달할 때까지 계속 분할한다.
곱셈은 하드웨어로 한다.

m4

> 알고리즘 2.9     aH

문제 : 2개의 2 AS uh ve 곱함
입력 : 큰 정주 와 2
출력 : prod (uS} ? 의 곱)

large_integer prod (large_integer u, large_integer v)
{

large integer x, y, w, 2

int 2, m

n= maximum(u®| 숫자 개수, 의 숫자 개수)
때 ( f= 0 || ㅠ== 0)

return 0;
else if ( 2 <= threshold)

return 일반적인 방법으로 구한 ux v;
else {

m= 1221,

x = u divide 10” y= urem 10”;

w = v divide 10” z= vrem 10”;

return prod (x, w) x 10°” + (prod (w, y)) x 10” + prod (y, 2);

OS
Wes >

정수 중에서 큰 정수의 숫자 개수이기 때문에 따로 입력으로 주지 않아도 알
수 있다. 그리고 divide, rem, ×는 작성할 1차 방정식 시간 알고리즘들이다.

| 호  ㆍ(큰 정수 곱셈)의 최악 시간복잡도 분석
A    A   인두 =

숫자 개수가 /인 두 개의 정수를 곱하는데 시간이 얼마나 걸리는지 분석한다.

단위연산 : 더할 때, 때, Le divide 10”이나, rem 10”이나, x 10”을 계산할 토이
의 3가지 연산은 각각 단위연산의 실행 횟수가 이다), 큰 정수에서 한자리 십진수 Be



===== PAGE 90 =====
76

chapter 2 분할정복

입력크기 : nS 정수 각각의 숫자 개수)
최악의 경우는 두 정수 모두 0과 같은 숫자가 없는 경우이다. 왜냐하면, 임계점을 지나야
만 재귀 호출이 끝나기 때문이다. 이 경우를 분석해보자.

n& 29] 거듭제곱이라고 가정하자. 그러면 x, 0, w, *는 모두 정확하게 숫자의 개수가
n/20\ch, 그러면 4개의 재귀 호출 각각에 주어지는 입력의 크기는 7/2이다. m=n/29]
기 때문에 덧셈, WA, divide 10"이나, rem 10"이나, x 10?의 연산은 시간복잡도가
모두 nol 대해서 1차시간이다. 이 1차시간 연산에 대한 최대 입력크기는 모두 같지 않으므
로, 정확한 시간복잡도의 산정은 쉼지 않다. 1차시간 연산을 모두 하나의 항 07으로(여기
서 cls 양의 상수) 묶는 편이 훨씬 더 간단하다. 그래서 얻은 BAAS 다음과 같다.

win) =40 (2 }+en, n> 8 이며, n& 22] 거듭제곱
W(s)=0

더 이상 입력사례를 분할하지 않는 지점의 실제 값 6는 임계점 값보다 작거나 같고, 294
거듭제곱이다. 왜냐하면, 여기서 입력은 모두 8의 거듭제곱이라고 가정했기 때문이다.

22] 거듭제곱이 아닌 nol] 대해서는 앞의 방정식과 비슷하지만 내림수연산과 올림수연
산을 포함한 재현식으로 작성 가능하다. 부록 BS] 예제 8.25에서와 같이 귀납 논법을 사용
하여 W(n)°] 결국은 감소하지 않는다는 AMIS 증명할 수 있다. 그러므로 부록 의 정리
B.6S 이용하여 HSS 유도할 수 있다.

Wn) € 0 (0280) = O(n’)

지금까지 공부한 큰 정수 곱셈 알고리즘은 시간복잡도가 아직 2차시간이다. 문제는 알
고리즘이 원래의 정수보다 숫자의 개수가 반인 정수를 가지고 곱셈을 4번 수행한다는 사
실이다. 이 곱셈의 횟수를 줄일 수 있다면, 8차시간보다 좋은 알고리즘을 얻을 수 있다.

다음과 같은 방법을 적용해본다. 함수 2200가 다음을 구해야 하고,

20, aztyw, yz                              (2,4)
그러기 위해서는 함수 prods WAS 4번 호출하여 다음을 계산하여 위의 값늘을 구했었다.
aw, 28, yw, yz

대신 다음과 같이 놓으면,
r=(e+y)(wtz) = ews (xz+ yw) + yz
다음 등식을 얻는다.

22+140=?7-ㅡ20242



===== PAGE 91 =====
> 알고리즘 2.10

이는 다음 세 값을 구하여 식 (2.4)에 있는 세 값을 얻을 수 있음을 의미한다.
7”=(2+4)(0+ㅎ),     rw,     yz

이 세 값을 얻기 위해서 약간의 1차시간 덧셈과 MALS 추가로 실행하는 반
9번만 하면 된다. 다음 알고리즘은 이 방법을 기반으로 작성하였다.

acd
tho

2 정수 곱셈 2
문제 : 2개의 큰 정수 ust ?를 BS
입력 : 큰 정수 uv

출력 : 27002 (u2 v2] 곱)

large_integer prod? (large_integer u, large_integer v)

{

large_integer x, y, Ww, Z, 7, D, 0;

int n, m;

n = maximum(u2] 숫자 개수, 의 숫자 개수) ;
if (7 == 0 || y= 0)

return 0;
else if ( 2 <= threshold)

return 일반적인 방법으로 구한 2 x v;

else {

m= od |,

x = u divide 10” y= urem 10”;

w = v divide 10” z= vrem 10”;

r= prod? (x+ y, wt 2);

p = prod? (x, w);

q = prod? (> 2);

return p x 10°” + (r—p—q) x 10" + q;

숫자 개수가 nel 두 개의 정수를 곱하는데 시간이 얼마나 걸리는지 분석한다.

단위연산 : 더할 때, MH 때, 또는 divide 10"”이나, rem 10”이나, x 10”-& 계산할 때(뒤
의 3가지 연산은 각각 단위연산의 실행 횟수는 7;이다), 큰 정수에서 한자리 십진수 곱셈.
입력크기 in (두 정수 각각의 숫자 개수)

최악의 경우는 두 정수 모두 0°] 없는 경우이다. 왜냐하면, 임계점을 지나야만 재귀 호출
이 끝나기 때문이다. 이 경우를 분석해보자.


===== PAGE 92 =====
78            chapter 2 분할정복

@ 표 2.4 알고리즘

2.10의 ㅎ+?에서 숫자개수의 예

n         2          8         ty      +yAA 숫자의 개수
4         10         10          20    =

4                           99                          99                           198            a

8                        1000                      1000                         2000            1

8                       9999                      9999                     19,998            oa

n°] 22] 거듭제곱이라면, <, y, w, ze 모두 숫자의 개수가 7/2이다. 그러므로 표 2.4
에서 보듯이 다음과 같은 부등식을 얻을 수 있

다.
꾸 = + 에서 숫자의 WES 긍+1
swt 2에서 숫자의 개수     at
이는 각 함수 호출에 대해서 입력크기가 다음과 같이 된다는 AS 의미한다.
입령크기
prod2(a+y, wt z)      aS   입력크기흐 긍  ah.
prod2(x, w)                는
prod2(y, z)                =

m = n/2°]7]| 때문에 덧셈, WAY, divide 10”, rem 10”, x 10" 3} 같은 1차시간 연산은
모두 nol 대해서 시간 복잡도가 1차시간이다. 그러므로 Wn) 2 다음을 만족한다.

3w(2}+en < Wn) = sw(2

9 +i}Fen, n> 8 이며 n°] 2°) 거듭제곱

W(s)=0

여기서 $는 임계점 값보다 작거나 같고, 29] 거듭제곱이다. 왜냐하면, 이 경우의 입력은
모두 8의 거듭제곱이기 때문이다. 29] 거듭제곱이 아닌 nol] 대해서는 앞의 방정식과 비슷
하지만 내림수연산과 올림수연산을 포함한 재현식의 작성이 가능하다. 부록 BO] 예제
8.25에서와 같이 귀납 논법을 사용하여 Wn)o] AHS 감소하지 않는다는 사실을 증명
할 수 있다. 그러므로 이 PAA] 왼쪽 부등식과 정리 Boo] 의해서 다음이 사실임을 알
수 있다

Wn) €  Q(n'®)


===== PAGE 93 =====
이제 다음이 사실임을 증명해보자.

Wn) € O(n'®*)
그러기 위해서 다음과 같이 놓는다.

W'(n) = W(n+2)
재현식의 오른쪽 BENS 사용하여 다음과 같이 전개할 수 있다.
n+2

W’' (n) = Wint2) < 30     +1}+eln +2]

= sw(2  +2}+en+20
<3" (2  J+ cnt 20
Wn) 감소하지 않기 때문에 W' (n) = 마찬가지이다. 따라서 부록 8의 정리 8.6에 의
해서 다음은 사실이다.
W'(n) € 0020)
따라서
~ (n) = W'(n—2) € O(n)
이 두 결과를 합하면, 다음과 같이 결론지을 수 있다.

W' (n) € O(n") > 6 (20)

Borodin} Munro(1975);= 빠른 뿌리에 변환(0886 Fourier Transforms)-& 사용하여 =
정수 BAIS 하는 O(n(len)?) 알고리즘을    발하였다. Brassard?! Monet2} Zuffelatto
는 1986년 조사 논문에서 아주 큰 정수 곱셈에 대하여 다루기도 하였다.
큰 정수에 대해서 Use oly 제곱근을 구하는 등의 다른 연산에 대한 알고리즘도 곱
셈 알고리즘과 시간복잡도의 차수가 SES 작성 가능하다.

임계값의 결정

2.1절에서 논의했듯이 AA (recursion)= 계산 시간 면에서 보면 꽤 많은 양의 추가비용

이 든다. AS 들어, 8개 키만 가지고 정렬하는 경우, O(n’) 알고리즘 대신 O(nign)
알고리즘을 사용하는데 드는 이 추가비용이 정말 가치가 있는 것일까? 또는 작은 7에
대해서는 교환정렬(알고리즘 1.9)이 재귀 합병정렬보다 아마도 빠르지 않을까? 사례를
더 이상 분할하는 것보다 다른 대체 알고리즘을                 최소한 더 빠르게 되는



===== PAGE 94 =====
80

chapter 2 분할정복

/의 값을 결정하는 WHS 공부해보자. 이 WSS BUGS 알고리즘, 대체 알고리즘,
그리고 구현하려고 하는 컴퓨터에 따라 달라진다. 이상적으로는 7의 최적 임계점이 되는
4{(optimal threshold value)& 찾고 싶은 것이다. 이 값보다 더 작은 입력사례에 대해서
는 계속 분할하는 것보다 다른 알고리즘을 호출하여 사용하는 편이 최소한 빠르고, 더
큰 사례에 대해서는 계속 분할하는 편이 더 빠르게 되는 사례크기가 바로 이 임계값이
된다. 그러나 앞으로 보게 되듯이 최적 임계값을 항상 구할 수 있는 것은 아니다. 분석을
하여 최적 임계값을 얻지 못한다 할지라도, 그 분석의 결과를 사용하여 임계값을 선택할
수 있다. 그리고 분할정복 알고리즘을 수정하여 일단 no] 임계값에 도달하게 되면 분할
을 중지하고 대체 알고리즘을 호출한다. 임계값을 어떻게 사용하는지는 알고리즘 2.8,
2.9, 2.10에서 이미 보았다.

임계값을 정하기 위하여 알고리즘을 구현하는 컴퓨터의 사양(실행속도)을 반드시 고려사
항에 넣어야 한다. 합병정렬과 교환정렬로 이 기술을 설명해보자. 이 분석에서 합병정렬의
최악의 경우 시간복잡도를 사용한다. 그래서 실제로 최악의 경우 벌어지는 상황을 최적
화 해보도록 한다. 합병정렬을 BAS 때 최악의 경우 다음과 같은 재현식을 얻었다.

합병정렬 2(알고리즘 2.4)를 구현한다고 가정해보자. 그리고 분석해 보려고 하는 컴퓨터
에서 합병정렬 27; 크기가 7인 입력사례를 분할하고 재합병하는데 걸리는 시간은 327
//5이라고 가정해보자. 여기서 us = 100만분의 1A(microsecond)S 나타낸다. 입력사례
를 분할하고 재합병하는데 걸리는 시간은 mid WS 계산하는데 걸리는 시간, 두 번의
재귀 호출을 위한 스택연산을 하는데 걸리는 시간, 두 부분배열을 재합병하는데 걸리는
시간을 모두 포함한다. 분할 재합병 시간은 여러 부분이 있으므로, 총 시간이 단순히 상
수시간 곱하기 n°] 될 가능성은 별로 없다. 그러나 분석과정의 단순화를 위하여 그렇게
가정하기로 한다. Wn) 2] 재현식에서 항 7ㅡ1은 재합병 시간이므로, 827.768 시간에
포함되어 있다. 그러므로 이 컴퓨터에서 합병정렬 2에 대한 재현식은 다음과 같다.

입력크기가 1이면 마지막 조건검사((6001481 condition 0016090만 실행하므로, 401)은
본질적으로 0이라고 가정한다. 편의상 처음에는 /을 2의 거듭제곱으로만 제한한다. 이
경우 다음과 같은 BAAS 얻는다.

W(n) = 2W(n/2)+32n ps, 7 > 이며, 7은 2의 거듭제곱
W(1) = Ops



===== PAGE 95 =====
© 예제 2,7

@®eeeeee
27 임계값의 결정   81

부록 Bo] 나와 있는 기술로 이 재현식을 풀 수 있다. 해는 다음과 같다.

W(n)= 32n lg n ps
같은 컴퓨터로 크기 7인 사례를 교환정렬로 정렬하는데 정확히 다음 시간이 걸린다고
가정해보자.

n(n—1)
5.

이 경우 합병정렬 8에서 교환정렬을 호출해야 하는 최적 임계점은 다음 부등식을 풀면
찾을 수 있으리라 생각할 수 있는데 이는 오해이다.

n(n—1)

pis < 32nlgn pus

의

00

풀면 다음과 같은 부등식을 얻는다.

n< 591

rlo

< 591이면 교환정렬을 호출하고, 그렇지 않으면 합병정렬 of 호출하는 것이 최적
이라고 AES 내리면 안 된다. 방금 한 분석은 분석 자체가 틀렸다. 합병정렬 로 7 = 1
일 때까지 계속 분할하게 되면 n < 591인 경우 교환정렬이 우월하다는 의미일 뿐이다.
우리가 알고 싶은 건 합병정렬 2= 분할하다가, 더 이상 분할하는 대신 교환정렬을 호출
하는 편이 더 좋을 임계점이다. = 1일 때까지 계속 분할하는 것과는 분명히 다르므로,
실제로 교환정렬을 호출하는 임계점은 591보다 작을 것이다. 왜 591보다 작아지는지 바
로 이해하기는 어려울 수 있으니 구체적인 예를 가지고 살펴보도록 하자. 지금부터는 7
이 29] 거듭제곱이어야 한다는 제약은 두지 않는다.

알고리즘 2.4(합병정렬9)에서 알고리즘 1.8(교환정렬)을 호출하는 최적 임계값을 구해보자. 어떤
계값 에 대하여 7 < to) 교환정렬을 호출하도록 합병정렬 oS 수정한다고 가정하자. 쓰던
퓨터를 그대로 쓴다고 하면, 새로 수정된 합병정렬 oo] 대한 재현식은 다음과 같다.
n(n— 1)
Wn)=4 ,?
w(|2| Js w| |) +52 us (n>t)
2] 최적값을 구하려고 한다. 그 값은 등식 (2.5)9] 위와 아래 표현식이 같게 되는 값이다. 왜냐
하면 교환정렬을 호출하면 입력사례를 더 분할하는 것만큼 효율적이 되는 지점이 바로 이 값이
되기 때문이다. 따라서 *의 최적값을 구하려면, 다음 등식을 풀어야 한다.

[1/2」와|7/21이 모두 #보다 작거나 같기 때문에 입력사례의 크기가 그 둘 중 하나라면 실행시간

=
이
|
컴

js                         (n < t)
(2,5)


===== PAGE 96 =====
@00@00000 0
chapter 2 분할정복

82

* 예제 2.8

은 등식 (2.9)의 위 표현식에서 나온다. 그러므로 다음과 같은 등식을 얻는다.
w(|<|}- 1/2] = w(|<]}-  [¢/2] ([ t/2 |-1)

t
2

등식 (2.0/을 이 등식으로 치환하면 다음과 같다.

[¢/2| (Le/2 |-1) , [4/2] (4/2 |=)     t(t—1)
2            2

2

+ 32¢=                               (2.7)

일반적으로 내림수연산과 올림수연산이 있는 등식에서 toll 짝수를 대입하는지 홀수를 대입하는
지에 따라서 다른 해답이 나올 수 있다. 바로 이것이 최적의 임계값을 항상 얻을 수 없는 이유이
다. 그러한 경우를 이제 조사해보자. 그러나 이 경우 tol BPS 대입하고(|《/2」와 |1/2|는 모
두 */2로 놓을 수 있음), 등식 (2.)을 풀면, 다음 해를 얻는다.

7= 128

~ 교 (t—1)/29} 같고, [¢/2]= (5+1)/2과 같음), 등식 ADS 풀면
t= 128.008

그러므로 최적 임계값은 128이 된다.

이제 최적 임계값이 없는 예를 보자.

어떤 특정 컴퓨터에서 실행되는 분할 정복 알고리

강고리즘에 대한 재현식이 다음과 같다고 하자.
(n)=37(|  | }+-16n ps

wm
2
여기서 167 uo 크기 nel AE 분할하고 Aas 필요한 Azole, Be BHA

떤 반복 알고리즘이 크기 nel 사례를 처리하는데 ^ ys 이 걸린다고 하자. 반복 알고리즘을 호출
해야 하는 값 tS 구하기 위하여 다음 식을 풀면 된다.

37 ieee
[¢/2|<to]HB, 입력이 이 크기가 되면 반복 알고리즘을 부르는데, 이는 다음과 같이 됨을 뜻

한다.

이오 | +16=2

tS 짝수로 치환하고(|1//2|=*/2가 됨) 풀면, 다음 aS 얻는다.
7= 64

tS 홀수로 치환하고|1/2|=(1+1)/2가 됨) 풀면, 다음 해

fu

얻는다.


===== PAGE 97 =====
@ 표 2.5 예제 2.8에서 nO] 짝수이면 임계값이 64이고 홀수이면 70임을 보여주는 사례

                  72?                     3 | 흥 ㅣ  +16n
62                3844                         3875
63                3969                         4080
64                4096                         4096
65                4225                         4307
68                4624                         4556
69                4761                         4779
70                4900                         4795
71                 5041                         5024
t= 70.04

여기서 구한 Ft 값은 같지 않으므로, 최적 임계값은 없다. 이는 사례의 크기가 64~70사이의
pg 사례를 한 번 더 분할하는 편이 더 효율적이고, 64~70사이의 홀수이면 반복 알고리즘

을 호출하는 편이 더 효율적이라는 뜻이다. 크기가 64보다 작으면, 반복 알고리즘을 호출하는
편이 항상 더 효율적이다. 크기가 70보다 크면, 사례를 다시 한 번 더 분할하는 편이 항상 더
효율적이다. 표 2.5를 보면 이게 사실임을 알 수 있다.

@ 28 분할정복법을 사용할 수 없는 경우

가능하다면, 다음 두 경우에는 분할정복법을 피해야 한다.
1, 크기 7인 사례가 거의 nol 가까운 크기의 두 개 이상의 사례로 분할된다.
2, 크기 인 사례가 n/c 크기의 거의 7개 사례로 분할된다.

Al 번째와 같이 분할하면 지수시간 알고리즘이 나오고, 두 번째와 같이 분할하면 ^")

알고리즘이 나온다. 이중 어떤 것도 /값이 크면 받아들일 수 없다. 왜 그렇게 분할하면

성능이 냐빠지게 되는지 직관적으로 봐도 알 수 있다. 예를 들어, al 번째 경우는 (이게
정말 가능한지는 모르지만) 나폴레옹이 30,000명의 적군 부대를 29,999명의 적군 두 개
부대로 나누는 경우와 마찬가지일 것이다. 적군의 수를 나누는 대신 그 수를 거의 두 배
로 늘린 Ao] 되었다. 나폴레옹이 정말 이런 식으로 분할정복을 이용했다면 위터루 전쟁
에서와 같은 참패는 훨씬 먼저 왔을 것이다.

알고리즘 1.6(재귀적인 방법으로 번째 피보나찌 항 구하기)이 7번째 BS 계산하는
사례를 (n— 1)번째 항과 (ㅠ- 2)번째 항을 각각 계산하는 두 개의 사례로 분할하는 분
할정복 알고리즘이라는 사실은 이제 쉽게 알아차릴 수 있을 것이다. 비록 그 알고리즘의
입력크기가 n-& 아니지만, 상황은 입력크기에 관하여 방금 설명한 그대로이다. 즉, 알고


===== PAGE 98 =====
84

chapter 2 분할정복

리즘 1.6으로 계산한 항의 개수는 7에 대하여 지수인 반면, 알고리즘 1.7(반복적인 방법
으로 7번째 피보나찌 항 구하기)로 계산한 항의 개수는 nol) 대하여 1차식이다.
반면 때로는 a at Artes 폴어도 We 경우가 있는데, 그 경우 간단한 분할

하면, 이 Bak /개의 nea 한 말뚝에서 다른 말뚝으로 옮기는테, 디스크를

방식에 제한이 주어진다. 이 문제를 푸는 표준적인 분할정복 알고리즘으로 구한 ene
를 순서대로 옮기는 REE no] 대하여 지수로 되고, 이야말로 주어진 제한을 지키면서
디스크를 옮기는 가장 효율적인 방법임을 증명하는 작업은 연습문제로 해보자. 결론적으
로 이 BAS 풀기 위해서 디스크를 옮기는 횟수는 /,의 지수에 비례한다.

2.1절
1. 이분검색(알고리즘 2.1) 알고리즘을 사용하여 다음 정수 배열에서 120을 검색하시오, 알고
리즘 실행과정을 단계별로 보이시오.
12 34 37 45 57 82 99 120 184

2. 좀 비현실적이기는 하지만 이분검색(알고리즘 2.1) 알고리즘을 사용하여 원소가 ?억 개인
배열을 검색한다고 가정해보자, 특정 원소를 찾기 위해서 비교를 최대로 번해야 할까?
특정 원소가 배열에 있을 수도 있고 없을 수도 있다.

3. 검색이 항상 성공한다고 가정해보자. 즉, 알고리즘 8.1에서 원소 를 배열 6에서 항상 찾는
경우만 따지면 된다. 불필요한 HES 제거하여 알고리즘 2.1을 날씬하제 다듬어보시오.
4. 이 8의 거듭제곱이어야 한다는 제한을 풀면, 이분검색(알고리즘 2.1) 알고리즘의 최악 시
간복잡도가 다음과 같음을 증명하시오.
Wn)  )=[Ign|+1
AS: Wn) 대한 재현식 다음과 같이 됨을 먼저 증명한다.
Wn) =1+ w(|2]).  n>1
Wn) =]
ㅣ 증명을 하려면 no] 짝수인 경우와 홀수인 BPS 따로 고려하고 귀납법으로 재현식을
풀어야 한다.
5. 알고리즘 2.1(4번째 줄)에서 분할 BES mid=low 로 바꾸었다고 하자. 새 검색전략을 제
시하시오. 그리고 이 전략의 성능을 분석하고, 분석결과를 차수 표기법으로 답하시오.
6. 원소가 개인 정렬된 WSS      mil n/3 72 배열 3개로 BUS, 거의 같은 크기로 분할)
하여 검색하는 알고리즘을               알고리즘은 분할한 세 배열 중에서 찾을 원소가
있을만한 배열에서 AAS 검색하는데,  이 HSS 다시 거의 같은 크기의 배열 3개로 분할

ㅇ



===== PAGE 99 =====
한다. 원소를 찾거나, 원소가 배열에 없음이 확실할 때까지 이 과정을 되풀이한다. 이 알고
리즘을 분석하고, 분석결과를 차수 표기법으로 답하시오.

7. 분할정복을 사용하여 원소가 7/개인 배열에서 가장 큰 YAS 찾는 알고리즘을 작성하시오.
알고리즘을 분석하고, 분석결과를 차수 표기법으로 답하시오.

2.2절
8. 합병정렬 알고리즘 2.2와 2.4를 사용하여 다음 HSS 정렬하시오, 알고리즘 실행과정을 ct
계별로 보이시오.

123   34   189   56   150   12   9   240
9. 연습문제 8에서 재귀 SSS 나무구조로 그리시오.
10. 다음 BAS 푸는 최악 시간복잡도가 O(nIn n) We} 나쁘지 않은 재귀 알고리즘을 작성하
시오. 정수가 개인 배월에서 수의 합의 차이가 alah 되도록 이 배열을 두 개로  분할하시
오. 배열에는 중복된 수가 없고, 7은 8의 배수라고 가정해도 좋다.
11. 재귀 SSO] 없는 합병정렬(알고리즘 2.29} 2.4) 알고리즘을 작성하시오.
12. 합병정렬(알고리즘 2,29} 2.4) 알고리즘의 최악 시간복잡도를 나타내는 재현식은 다음과

음을 증명하시오.

my.

Wn) = w(|2 |} 써주]
여기서 n& 29] 거듭제곱으로 제한하지 않는다.
13. 원소가 nA 배열을 8등분하고, 분할한 배열을 각각 따로 정렬한 후, 다시 합병하는 정렬
알고리즘을 작성하시오. 작성한 알고리즘을 분석하고, 분석결과를  en 표기법으로 답하시오.
2.3절
14. 다음 재현관계식으로 2(625)의 값을 구하시오.

T(n) =77(2),  n>1
JAG) al

15. 아래 solve (HUES) 살펴보자. 이 알고리즘은 어떤 입력 /에 대응하는 출력(해답) OF
찾아서 문제 #를 푼다.

void solve (input J output& 0 )

{
if ( size (I) == 1)
해답 OF 바로 찾는다 ;
else {
TS 다섯 개의 입력 4, 4, 4, 4,, hE 분할한다.
여기서 / = 1, .…, 5에 대하여 size) := 5220(7)/3 ;


===== PAGE 100 =====
86

chapter 2

16.

17.

18.

분할정복

tee (fe eH 51 2)
solve ( I;, O; ) ;
입력 로 PS = 해답 OF 구하기 위하여 O,, O,, O3, O1, OFS 합병한다.

}

g(n)& 분할하고 합병하는 단위연산이라 하고, 크기가 1인 입력사례의 단위연산 시간은 0

이라고 가정하자.

(8) 입력크기가 nel 경우 PS 푸는데 필요한 단위연산의 횟수를 표시하는 재현식 Tn) S
작성하시오.

060) g(n) = O(n) OVA 이 재현식의 해는 무엇인가? (증명은 생략해도 좋음)

(c) g(n) =7이라고 가정하고, 정확히 7=27인 경우 MBAS 푸시오.

(0) no] 39] 거듭제곱인 경우 일반해를 구하시오.

분할정복 알고리즘에서 크기가 인 문제의 입력사례를 7/3 크기의 10개의 입력사례로 항

A} 분할하고, 분할하고 합병하는 과정은 O(n’) 9 시간이 걸린다고 가정하자. 실행시간

2100)을 나타내는 재현식을 작성하고, 그 식의 해를 구하시오.

하노이탑(20\678 of Hanoi) 문제를 푸는 분할정복 알고리즘을 작성하시오. 하노이탑은 말

뚝 3개와 크기가 모두 다른 구명난 디스크 7개로 구성되어 있다. 문제는 한 말뚝에 쌓여있

는 7개의 디스크를 모두 지정한 말뚝으로 옮기는 것이다. 문제를 풀 때 다음 규칙을 반드시

준수해야 한다.

(1) 세 개의 말뚝 이외에는 디스크를 놓을 수 없다.

(2) 한 Hol 하나의 디스크만 옮길 수 있고, 말뚝의 맨 위에 있는 디스크만 옮길 수 있다.

(9) 큰 디스크를 작은 디스크 위에 올려놓을 수 없다.

(a) 작성한 알고리즘의 복잡도가 (72) = 2" ㅡ1임을 증명하시오(여기서 no] 디스크의 개수
이면 S(n)&  니체 엇수의더):

(b) 아무리                 만들어도 최소한 (8/에서 주어진 횟수만큼은 옮겨야 함을 중
명하시오.

분할정복 알고리즘이 크기가 ne 문제의 입력사례를 n/c 크기로 분할할 때, 재현식의 형태

는 보통 다음과 같다.

여기서 g(n) 2 분할하고 합병하는 비용이고, 0는 상수이다. ㅠ=ㅇ라고 하자.
(9) 다음을 증명하시오.

Tet) =dx at 210 0(0)]

go1

(b) g(n) € O(n) SH 재현식을 푸시오.



===== PAGE 101 =====
2.4절
19. 빠른정렬(알고리즘 2.6 알고리즘을 사용하여 다음 HAS 정렬하시오. 알고리즘의 실행과
정을 단계별로 보이시오.

1238 834 189 56 150 109 9 240
20. 연습문제 199] 실행과정에서 재귀 호출 나무구조를 그리시오.
21. 다음 부등식이 성립한다고 가정하고,

Wn) < (p—1)(p~2) , (n=p)(n=p-1) ,

2                                2
다음 부등식이 성립함을 증명하시오.

이 결과는 알고리즘 2.0(빠른정렬)의 최악 시간복잡도 분석에 사용하였다.
22. 다음 등식이 성립함을 증명하시오.
5)146-10)+ㅜ40-21=93]46-1)
이 결과는 알고리즘 2.6 (빠른정렬)의 평균 시간복잡도 분석에 사용하였다.
23. 재귀 호출 없는 빠른정렬 알고리즘(알고리즘 2.6)을 작성하시오. 알고리즘을 분석하고 분석
결과를 차수 표기법으로 답하시오.

24. 빠른정렬에서 배열의 첫째 원소를 기준원소(0704로 사용한다고 가정하고 다음에 답하시

lif

47S 보여주는 원소가 10개인 배열을 예로 드시오.
00) 최선의 경우를 보여주는 원소가 10개인 WSS 예로 드시오.

25. 알고리즘 1.4(행렬곱셈)가 실행하는 덧셈의 횟수는 이 알고리즘을 약간
로 줄일 수 있음을 보이시오.

26. 예제 2.4에서 두 개의 2x2 행렬의 ASeA 곱을 보여주었다. 이 곱이 정확한지 밝히시오.
27. 표준 알고리즘을 사용하여 두 개의 64x64 YAS] 곱을 구하는데 실행하는 곱셈의 HEL?

28. AJEzpPAle] 방법(알고리즘 2.8)을 사용하여 두 개의 64x64 행렬의 곱을 구하는데 실행하
는 곱셈의 횟수는?

정하면 n3 — 1? ©.

i
+

29. 곱셈과 aS 18번 대신 15번 실행하는 쉬뮤엘 위노그래드가 개발한 수정된 쉬트라썬 알고
리즘의 재현식을 작성하시오. 이 MBAS 풀고, 구한 답이 2.5419] 마지막 부분에 나온 시
간복잡도와 같은지 확인하시오.

2.6절
30. 알고리즘 2.10(큰 정수 곱셈 2)을 사용하여 1258과 23,1032] 곱을 구하시오


===== PAGE 102 =====
88

chapter 2 분할정복

31. 연습문제 30번에서 두 ASS 곱하는데 필요한 곱셈의 횟수는?

82. 다음 연산을 실행하는 알고리즘을 작성하시오.
wu x 10;    u divide 10”;     u rem 10”;
여기서 ut: 큰 정수를 나타내고, 은 음이 아닌 정수, divide: BHAT HS 넘겨
주고, rem 나머지를 넘겨준다. 작성한 알고리즘을 분석하고, 이 연산들이 1차시간 안에
수행될 수 있는지 보이시오.

33. 《개의 숫자로 된 ASS 다음과 같이 분할할 수 있도록 알고리즘 2.9(큰 정수 곱셈)를 수정
하시오.
(a) 숫자 7/3개씩 3개의 AB 분할(,=@#으로 가정)

06) 숫자 7/4개씩 4개의 APR 분할2=《으로 가정)
작성한       즘을 분석하고, 분석결과를 차수 표기법으로 답하시오.

2.7절

34. 원소가 개인 배열을 정렬하는 교환정렬과 빠른정렬 알고리즘을 구현하는 프로그
작성하시오. 작성한 프로그램을 각각 돌려서 실행시간을 비교하여 빠른정렬 알고리즘을 사
용하는 편이 더 유리해지기 시작하는 임계 하한 nS 찾으시오.

35. 두 개의 nxn 행렬(ㅠ=9")을 곱하는 표준 알고리즘과 HEM 알고리즘을 구현하는 프로
=H 가가 작성하시오. 작성한 프로그램을 22} 돌려서 실행시간을 비교하여 ASI 알
더 유리해지기 시작하는 임계 하한 7을 찾으시오.

36. 알고리즘 2.8(쉬트라썬)의 경우 크기가 nel 입력사례를 분할하고 재결합하는데 120^ ps 시
간이 걸리는 컴퓨터가 있다고 가정하자. 여기서 구한 시간은 덧셈과 WS 하는데 걸리는

시간도 모두 포함하고 있다. 표준 알고리즘으로 두 개의 nxn ioe dil ^” ps 시간
이 걸린다면, 입력사례를 더 이상 분할하는 대신 표준 알고              하는 임계값을
구하시오. 유일한 최적 임계값이 존재하는가?

2.8절

37. 분할정복을 사용하여 7!을 계산하는 재귀 알고리즘을 작성하시오. 입력크기(1장의 예제 34
참조)를 정의하고 다음 물음에 답하시오. 작성한 알고리즘의 시간복잡도는 지수인가? 2.8절

경우 1을 위배하는가?

38. 분할정복 알고리즘에서 크기가 nel 문제의 입력사례를 항상 3등분한다고 하고, 분할하고
합병하는 과정은 1차시간이 걸린다고 가정하자. 실행시간 T(n)-S 나타내는 AAAS 작성
하고, 그 방정식의 해를 구하시오. 해를 차수 표기법으로 답하시오.

더

16

추가 연습문제

39. 피보나찌 수열 알고리즘 1.6과 1.7을 모두 프로그램으로 구현해보자. 구현한 프로그램이 맞
는지 시험입력으로 검증해보자. 재귀 프로그램으로 66초 이내에 BS 계산하는 가장 큰 수
를 찾아보자. 같은 수로 반복 프로그램은 얼마나 시간이 걸리는지 재보자.

40. nXm 차원 배열에서 원소를 검색하는 효율적인 알고리즘을 작성하시오. 이 MAS 행과



===== PAGE 103 =====
41.

42.

43.

45.

열을 따라서 정렬되어있다. 즉,
Table [i][j] < Table {i][j+1]
Table [il[j] < Table [i+1][j]

n=2* 팀이 참가하고, 1회전에서 n/2 경기를 치르고, n/2=2'-! Sap} 2회전에 진출하는

방식으로 진행하는 (한 번 지면 탈락하는) 토너먼트가 있다고 가정해보자.

(8) 이 토너먼트의 회전의 수를 나타내 주는 재현식을 작성하시오.

00) 64 Bo] 참가한다면, 토너먼트에서 회전의 수는?

(0) (9)번에서 구한 재현식의 해를 구하시오.

정사각형이 3개 붙어있는 AS 트로미노(ㅠ00000)라고 한다. 가로와 세로로 개의 정사각

Bo] 연결되어 있는 바둑판이 있고, 1칸은 XK 표시가 되어 있다. 여기서 #은 29] 거듭제곱이

라고 가정한다. 다음 조건을 만족하도록 트로미노를 바둑판에 채우고 싶다.

* 바둑판 전체를 트로미노로 채워야 한다.

* × #A|7} 되어 있는 We 드로미노로 덮을 수 없다:
* 트로미노는 겹쳐 놓을 수 없다.

* 트로미노는 바둑 바깥으로 삐져나올 수 없다.

이 문제를 푸는 분할정복 알고리즘을 설계하시오.

다음 문제를 풀어보자.

(a) 1부터 10까지 ASS 매겨놓은 똑같이 생긴 동전 9개가 있다고 하자. 이 중에서 동전
하나만 다른 동전보다 무겁다. 양팔저울 하나로 두 번만 B+ 있다고 하자. 무거운 동전
하나를 골라내는 알고리즘을 고안하시오.

(b) 이제 동전이 개 있다고 하고, 이 중 하나만 다른 동전보다 무겁다고 하자. 7은 자연수
의 8승으로 한정하고, 양팔저울 하나로 10857번만 A 수 있다고 하자. 무거운 동전 하나
를 골라내는 알고리즘을 작성하고, 알고리즘의 시간복잡도를 구하시오.

세 개의 정수 2, 7, 2가 입력이고, 7"을 #로 나눌 때 나머지를 계산하는 ㅇ(2187) 재귀
알고리즘을 작성하시오. 편의상 nS 2의 거듭제곱(즉, 어떤 양의 정수 kel] 대하여 7 = 2“)
이라고 가정해도 좋다.

실수 7개로 구성한 리스트에서 Yo] 최대가 되는 인접 부분리스트를 찾는 재귀 알고리즘을
분할정복으로 설계하시오. 작성한 알고리즘을 분석하고, 분석결과를 차수 표기법으로 답하
시오.



===== PAGE 104 =====
번째 피보나찌 수 구하기(알고리즘 1.6를 분할정복 알고리즘으로 풀면 재귀 호

출의 횟수가 noi] 대하여 지수(2")로 증가한다. 왜 그럴까? 분할한 입력사례가
지수만큼 많기 때문이다. 3장에서 공부했듯이 분할정복은 S192 (top-down) 문제풀이
방식이다. 분할한 입력사례들끼리 서로 관련이 없는 정렬 문제를 푸는 경우 이 방식이
잘 통한다. 분할한 입력사례들은 각각 독립적으로 정렬할 배열들이라 서로 관련이 없고
중복도 없다. 그러나 /째 피보나찌 수 구하는 문제는 분할한 입력사례들이 여러 wi 중복
해서 나타난다. 예를 들면, 1.3절에서 본 대로 5째 피보나찌 수를 구하기 위해서 4째와
3째 피보나찌 수를 구해야 한다. 그러나 4째와 3째 피보나찌 수를 구하기 위해서 둘 다
om] 피보나찌 수가 필요하다. 분할정복 방식으로 이 문제를 풀면 이 두 수를 따로 구하기
때문에 8째 피보나찌 수는 두 번 이상 중복 계산한다. 분할한 입력사례들이 서로 관련이
있거나 두 번 이상 나타나는 문제를 분할정복 알고리즘으로 풀면 같은 입력사례를 중복
계산하게 되므로 매우 비효율적이다.



===== PAGE 105 =====
@0@00000 0
92            chapter 3 동적계획

이 장에서 공부할 알고리즘 설계방법인 동적계획(07ㅁ87010 programming) 분할정
과 문제해결 방향이 거꾸로다. 동적계획은 문제의 입력사례를 분할하여 BAS 푼다
Ae 분할정복과 비슷하다. 그러나 동적계획은 분할한 입력사례를 재귀 호출하여 FS
얻는 대신, 가장 작은 입력사례의 BS 먼저 구하여 저장해놓고, 필요하면 꺼내 쓴다. "동
적계획"이라는 용어는 제어이론(60ㅁ\ㅁ0! theory) A] 왔는데, 여기서 Al] (programming)
이란 해답을 구하기 위해서 배열(테이블)을 구축함을 뜻한다. 1장에서 공부했듯이, 7째
피보나찌 수를 구하는 효율적인 알고리즘(알고리즘 1.7)은 동적계획을 이용한 전형적인
사례이다. 인덱스가 0부터 7까지인 배열에서 앞부분의 nt 1항을 순서대로 구축하여 7
A 피보나찌 항을 구한다. SAAS 알고리즘은 HSS 이용하여 상향식으로 BES 구
한다. 따라서 SAAS ARR (bottom-up) 접근방법이다. 알고리즘 1.7과 같이 배열을
사용하여 알고리즘을 개발하고, 알고리즘을 개선하여 배열 AAS 기억해둘 필요 없게
해보자.

동적계획 알고리즘의 개발절차는 다음과 같다.

1. 문제의 입력사례에 대해서 HSS 계산하는 재귀 관계식(060478176 property)-&

rir ae

ㅇ

|

세운다.
2, 작은 입력사례부터 먼저 해결하는 상향식 방법으로 전체 입력사례에 대한 해답을
구한다.

동적계획을 적용하여 문제를 해결하는 방법을 이해하기 위해서 간단한 예제부터 복잡
한 예제에 이르기까지 차례로 공부해보자.

@ 3.1 이항계수 구하기
부록 A] ㅅ.7절에서 정의한 이항계수001000181 000[001604는 다음과 같다.

n       n!

te 시)!

값이 큰 nF} ko] 대한 이항계수를 구하는 경우 이 식을 가지고 바로 구하기는 힘들다.
왜냐하면, 그리 크지 않은 nol] 대해서도 !은 꽤 크기 때문이다. 다음 재귀 관계식을 사
용하면 nlolUy 신을 계산하지 않고 이항계수를 구할 수 있다.

2     22

비니 소타 0
밀이파다 1

이 ALS 유도하는 과정은 연습문제로 남겨둔다. 이 재귀관계식으로 분할정복 알고리즘
을 설계해보자.

for 0O= khan

(3,1)


===== PAGE 106 =====
0000000
3.1 이항계수 구하기   93

OSG 31 분할정복으로 이항계수 구하기

입력 : = 7을 만족하는 0 이상의 정수 과 k
출력 : bin, 이항계수 |

int bin (int 2, int 2)

{
ft (4=— 0 || 2 == 4
return 1;
else
return bin (n—1, 4-1) + bin (n—1, 4);
}

알고리즘 1.607번째 피보나찌 수 구하기, 재귀)과 같이 알고리즘 3.1은 매우 비효율적
이태 ("|e 를 구하기 위해서 이 알고리즘이 계산하는 항의 ASE 다음과 같은데, 증명은
연습문제로 남겨둔다.

문제는 재귀 호출할 때마다 같은 사례를 중복 계산한다는 것이다. 예를
(n—1, 4-1)과 bin(n-1, IE ST din(n—-2, k—1)2] 계산결  ak i 필요하고, 이
결과는 각 재귀 호출 시 각각 따로 구한다. 3.8절에서 언급했지만, 분할정복에서 입력사
alo] 원래 크기와 별 차이 없는 크기로 분할하면 항상 비효율적일 수밖에 없다

이제 효율적인 알고리즘을 동적계획으로 설계해보자. 재귀 관계식은 등식 (3.1에서
이미 세워 놓았다. 이 식으로 #0101|에 『  ] 값을 차례로 저장하여 배열 BS 구축해 나
간다. 이 문제를 푸는 동적계획 알고리즘을 작성하는 절차는 다음과 같다.

1 재귀 관계식(등식 8.1)을 세운다. #의 형태로 다시 작성하면 다음과 같다.

Bila) =1팬 MG— 11+ ati O0<j<i
1

=) 또는 7=0

2, 첫째 행부터 BS] 행에 값들을 차례로 계산하여 저장하는 SPI bottom—up) 방

식으로 문제를 푼
절차 2 그림 8.1에서 보여준다(이 그림에서 배열은 파스칼 삼각형임을 바로 tops
을 것이다). 각 행의 값은 절차 1에서 정립한 재귀 관계식을 적용하여 바로 이전에 계산한
값을 가지고 계산한다. 계산한 최종값 Bhalla e | ? |의 값이다. 예제 8.1에서 계산 절차
를 자세히 추적해보자. 예제에서는 앞의 두 열만 계산하는데, k= 2017] 때문이다. 일반


===== PAGE 107 =====
@0 00000 0
chapter 3 동적계획

94

© 예제 31

123 4   j k

honNnD = 0
은 6 00
ow =

※%

—_

Bli- 1][/— 1] Bli- 11/1

i                                        > BU IL]

n

그림 3.1 이항계수를 구하는데 사용한 배열 B

화하면 각 행에서 《번째 열까지 값만 계산하면 된다. n= k= 0281 때 이항계수는 1이므
로 예제 8.1에서 210][0] = 1이다. 사실 이 같은 다른 이항계수를 구하는데 쓰지 않지만
구색을 갖추기 위해서 포함시킨다.

214121=| 를 계산해보자.

0번째 Bo] 계산 : {알고리즘의 구색을 갖추기 위해서 포함시키는 AE
BO}(0] 값은 실제로 쓰지 않는다. }

22[0][0] = 1
1번째 행의 계산 :
21]10] =1
끼1]11] = 1
2번째 행의 계산 :
Bl2][0] =1
끼2]11] = Bl)[o]+ Bij] = 1+ 1 = 2
Bl2)\[2] =1
3번째 행의 계산 :
2213]10] =1

Bi3)1] = 22110] + 212]1] = 1+2 = 3

Bi3)[2] = 끼2]11] + Bl2][2] = 2 +1 = 3
4번째 행의 계산 :

Blaj[o] =1

Bl4\{1] = B[3)[0]+ B[3][1] = 1 + 3 = 4


===== PAGE 108 =====
0000000
3.1 이항계수 구하기   95

Bl4)[2] = B[3)[1] + 213][12]= 3 + 3 = 6

예제 3.1에서는 이항계수를 값이 증가하는 SLE 계산하였다. 반복 계산할 때마다 필
요한 값들은 이미 계산해서 저장해두었다. 이러한 방식은 동적계획법에서 기본적으로 쓰
이는 절차이다. 다음은 동적계획으로 이항계수를 구하는 알고리즘이다.

ㆍ 일조 3.2 동적계획으로 이항계수 구하기

문제 : 이항계수를 계산하시오.
입력 : k<n& 만족하는 0이상의 정수 nz} *
출력 : 8072, 이항계수 ("|
int bin? (int n, int 2)

{
index i, j
int Bl0..n] [0..4] ;

for (f= 0; 7 <= H+)
for (j = 0; j <= minimum(i, 420; #++)
if (== 0 || /== 9
             Bill] = 1;
else

|              AL) = Be-YU-1) + Bly];
return Bl nx |[ «];

파라미터 nF} 《는 이 알고리즘에서 입력의 크기가 아니다. 그들은 입력일 뿐이고, 입
력크기는 //과 《를 코드화(600009)하는데 필요한 심벌의 개수이다. 1.3절의 nv 피보나
찌 수 구하는 알고리즘과 비슷한 상황이다. 그러나 답을 구할 때까지 얼마나 작업을 했는
지 nit *의 함수로 표현하여 알고리즘의 효율성을 대략 알아볼 수는 있다. 과 eS 기
준으로 for—j 루프를 몇 번 실행하는지 계산해보자. Zi Gol 대하여 몇 번 실행하는지
를 세보면 다음 표와 같다.

i    0123 … k ktl «+ on
루프 실행 횟수  0123 -+kt+1 ktl ++ k+l

따라서 총 실행 횟수는 다음과 같이 계산할 수 있다.

1+2+34+4+--+k+(k+1)4+ (k+1)---+(k+1)

n—-k+13]


===== PAGE 109 =====
96

chapter 3 동적계획

부록 AS] 예제 ㅅ.1의 결과를 적용하면 다음 등식을 얻는다.
k(k+1)
2
할정복 대신 동적계획으로 훨씬 더 효율적인 알고리즘을 설계하였다. 앞에서 언급%
듯이, 동적계획은 입력사례를 더 작은 입력사례로 분할하는 재귀 관계식을 찾는다는 점
에서 분할정복과 비슷하다. 차이점은 동적계획은 맹목적으로 재귀를 적용하는 대신 재귀
BAAS 사용하여 작은 입력사례부터 시작하여 반복적으로 입력사례의 해답을 구해나
간다는 것이다. 이런 식으로 하면 작은 입력사례의 해답은 한 번만 구하면 되므로 중복계
산을 방지할 수 있다. 분할정복 알고리즘이 비효율적이면, 동적계획은 시도해볼 만한 기
술이다.
알고리즘 8.8를 표현하는 가장 손쉬운 방법은 이차원 배열 0 전체를 만드는 것이다.
그러나 하나의 행의 계산이 끝나면, 전에 계산했던 BSS 더 이상 필요하지 않다. 따라
서 인텍스가 0부터 《까지인 배열 하나만 가지고도 충분히 알고리즘을 표현할 수 있다.
어떻게 알고리즘을 수정할 것인지는 연습문제로 남겨둔다. | |= |, ” , |가 성립한다는

사실을 이용해도 이 알고리즘을 개선할 수 있다.

+(n-—k+1)(k+1)=

Ac

—

3,2 프로이드의 최단경로 알고리즘

비행기로 FBS 계획하면서 흔히 접하게 되는 문제는 직항로가 없을 때 어떤 도시를 경
유하면 가장 빠른지 최단경로를 구하는 것이다. 최단경로를 구하는 알고리즘을 이제 설
계해보자. 먼저, 그래프이론을 알아야 한다. 그림 3.2는 가중치포함 방향그래프의 예이
다. 그래프를 그림으로 표현하는 경우 Alcircle)-& utr] (vertex, vertices)e} 하고, 마디
를 잇는 AS 이음선(6086/@ㅁ0)이라고 한다. 이음선에 방향이 있는 그래프를 방향그래프
(directed 808080/01878010)라고 한다. 방향그래프는 화살표로 방향을 나타낸다. 방향그래
프에서는 두 마디를 서로 다른 방향으로 잇는 이음선이 두 개 있을 수 있다. 예를 들어,
그림 3,28 보면 WA] 《,로 가는 이음선과 에서 (으로 가는 이음선이 있음을 알
수 있다. 이음선과 관련된 값은 7ESAl (weight) =} 하고, 이음선에 가중치가 있는 그래프
를 가중치포함 그래프(\6180660 87821)이라고 한다. 가중치는 FO] 아니라고 가정한다.
가중치는 보통 거리를 나타내는 경우가 많다. 따라서 한 마디에서 다른 마디로 가는 경로
를 이야기 해보자. 방향그래프에서 다음 마디로 가는 이음선이 있는 마디의 나열을 경로
(28140라고 한다. 예를 들면, 그림 3.244 [1 , v4, 06]은 4, 에서 로 가는 이음선이
있고, 에서 v3 2S 가는 이음선이 있으므로 경로이다. [0<5, vy, ve 에서 이로 가
는 이음선이 없으므로 경로가 아니다. 어떤 마디에서 그 마디 자신으로 가는 ABE 순환



===== PAGE 110 =====
@eeeee 0
3.2 프로이드의 최단경로 알고리즘    97

그림 3.2_가중치포함 방향그래프

경로(6>018)라고 한다. 그림 3,24] 경로 [01 , vy, v5, ve 순환경로이다. 그래프에 순
환경로가 있으면 순환적(6010/이라 하고, 그렇지 않으면 비순환적(607010)이라고 한다.
같은 마디를 두 번 거치지 않는 경로를 단순경로(60016 0800라고 한다. 그림 3.8에서
경로 [0 , vo, ]은 단순경로이지만, 경로 [v,, 4, v5, 1, 001는 단순경로가 아니다.
단순경로는 순환이 있는 부분경로를 절대로 포함하지 않는다는 사실을 주의해야 한다.
가중치포함 그래프에서 경로의 길이060810는 경로 상에 있는 가중치의 합이고, 가중치
가 없는 그래프에서는 경로 상 이음선의 개수이다.
그래프 응용문제 중에서 가장 유명한 BAS 각 마디에서 다른 모든 마디로 가는 최단

경로를 찾는 문제가 있다. 여기서 최단경로가 당연히 단순경로이어야 한다. 그림 3.2에
서 0, 에서 으로 가는 단순경로로는 [2 , vp, vg], [이 , vg, 061, 141, vo, 4, %80가 있
다. 그 길이는 각각 다음과 같이 계산한다.

length|v,, vo, v3] = 1 + 3 = 4

length [v,, U4, 48]=1+2=83

length[v,, vo, v4, v3] = 1+ 2 + 2 = 5

이 중에서 경로 [0 , v4, %]이 어에서 v3 2 가는 최단경로이다. 앞에서 밝혔듯이 흔히
쓰는 최단경로 TAS] 응용사례로서 도시 간의 최단경로를 구하는 문제가 있다.

43 (shortest paths) 문제는 최적화 A] (optimization problem) 속한다. 최적
화 문제는 하나 이상의 SFE (candidate solution)7} 있을 수 있다. 해답후보에는 그
와 관련된 U(value)o] 있고, 그 문제의 해답은 해답후보 중에서 최적값004181 value)
이 된다. 문제에 따라서 최적값은 최대값이 될 수도 있고 최소값이 될 수도 있다. 최단경

문제에서 해답후보는 한 마디에서 다른 마디로 가는 경로이고, 그 값은 경로의 길이가
되고, 최적값은 경로 중에서 최소 길이가 된다.

한 마디에서 다른 마디로 가는 최단경로는 하나 이상 있을 수 있기 때문에, 여기서는
그 최단경로들 중에서 하나를 찾는다. 이 BAS 가장 쉽게 푸는 알고리즘은 각 마디에
대해서 그 마디에서 다른 각 마디로 가는 모든 경로의 길이를 구한 후, 그 길이 중에서


===== PAGE 111 =====
98

chapter 3 동적계획

최소값을 찾는 것이다. 그러나 이 알고리즘은 지수시간(66000ㅁ6008))보다도 나쁘다. 예를
들어, 모든 마디가 이음선으로 서로 연결되어 있다고 가정하자. 그러면, 한 마디에서 시
작하여 다른 마디에서 끝나며, 나머지 모든 마디를 한 번씩 거쳐 가는 모든 경로의 집합
은 시작하는 마디에서 끝나는 마디로 가는 모든 경로의 부분집합이다. 그 경로에서 둘째
마디는 2-8개의 마디 중 하나이고, 셋째마디는 4-8개 마디 중 하나이고, 이런 식으로
계속 나가다가 그 경로에서 마지막 둘째마디는 마디가 하나 밖에 없으므로, 한 마디에서
다른 마디로 가면서 나머지 모든 마디를 거쳐서 가는 경로의 총 개수는 다음과 같다.

(020-2)02-3)… 1= (0 - 2)!

이 값은 지수보다 나쁘다. 이러한 상황은 최적화 문제에서 많이 나타난다. 즉, 모든 가능
성을 다 따지는 알고리즘을 설계해보면 수행시간은 지수이거나 그보다 더 나쁘다. 따라
서 우리의 목표는 더 효율적인 알고리즘을 찾는 것이다.

동적계획을 사용하면, 최단경로 문제를 푸는 3차시간(01010-ㅁ08) 알고리즘을 만들어
낼 수 있다. 우선 최단경로의 길이만 구하는 알고리즘을 설계해보자. 최단경로도 구하도
록 나중에 알고리즘을 수정할 것이다. 7개 마디로 된 가중치포함 그래프는 다음과 같이
배열 We 표현한다.

이음선 가중치 《에서 vj 가는 이음선이 있는 경우
WIL] =} 00            viol 로 가는 이음선이 없는 경우
0            1 = )인 경우

에서 0, 가는 이음선이 있는 경우 ,는 《,에 인접하다(30080600라고 하기 때문에 이
배열을 그래프의 914 BA (adjacent matrix)°]e}31 한다. 그림 3.2의 그래프를 인접행렬
로 표현하면 그림 3.3과 같다. 그림 3,32] 배열 DE 그래프 마디 사이의 최단경로의 길이
를 나타낸다. 예를 들어, D[3][5]= 7인데, 에서 로 가는 최단경로의 길이가 7이기
때문이다. 의 값에서 D2] 값을 계산하는 방법이 바로 최단경로 문제를 푸는 알고리즘
이다. 따라서 일련의 7+1개의 배열 DS 만든다. 여기서 0 = 《*즈7ㅠ이고, 2""'는
다음과 같이 정의한다.
2띠[/][/] =집합 (vy, vo, 2... Yb 속하는 마디만을 거쳐서
에서 로 가는 최단경로의 길이

왜 이 AS 가지고 DOA) 를 계산할 수 있는지 알아보기 전에 이 배열 원소의 의미를
살펴보자.


===== PAGE 112 =====
© 예제 3.2

32 프로이드의 최단경로 알고리즘      99
1 | 0    1    00   1            ifo        3    1
2/9    0   3   2   00       218   0    3   2   5
이의 으 | 3 ie       3|10 11 0 4 7
41   00   2    0   3       4/6   7   2    0    3
513   00   00   00   0       5 | 3   4   6   4   0
44                           D
그림 3.3 WE 그림 3.29) 그래프를 나타내고, DE 최단경로의 길이를 나타낸다. 최단경로를 푸
는 알고리즘은 Wol 있는 값을 가지고 Doll 있는 값을 계산한다

그림 3,22] 그래프를 가지고 Dj] WS 몇 개만 계산해보자.
D[2\[5] =length [vg]iv,] = 00

]
Df2][5] = minimum (length [v., v5], length[v,, v,, v5)

= minimum (co, 14) = 14

D[2)[5] = D™[2][5] = 14      {0;를 출발하는 최단경로는 0,를 갈 수 없으므로
어떤 그래프에서도 이 두 값은 같
22912]6]= D[2][5] = 14      10; 를 포함해도 v, HA 로 가는 lee 경로가

추가되지 않으므로 이 그래프에서 이 두 Be 같다}
D(2)[5] = minimum (length|v, v,, vs]; length[v., vy vs],
length[v,, v1, Uy Us], length[vg, vg, Vy vs])
=minimum(14, 5, 13, 10) =
D®2][5] = D®[2][5] =5       {에서 끝나는 최단경로는 ;를 거쳐 갈
어떤 그래프에서도 이 두 값은 같다}

계산된 마지막 값 D2] 다른 모든 마디를 거쳐 가도록 허용하고 구한 vO] 로 가는
최단경로의 길이이다. 즉, 727“'21[6|가 최단경로의 길이다.

:
E

Ni

D” (ij) 7 다른 모든 마디를 거쳐 가도록 허용하고 계산한 v,o14 *,로 가는 최단
경로의 길이이므로, 그 Be (에서 로 가는 최단경로의 길이이다. 27"'7][/]는 다른
어떤 마디도 거쳐 가지 못하도록 하고 구한 최단경로의 길이이므로, ',에서 vB 잇는
이음선의 가중치이다. 따라서 다음 등식이 성립한다.

pu = W, D™=D

따라서 로부터 DS 구하기 위해서 7/?'"'으로부터 D\”™ & 구하는 방법만

al
|o
re
ri,


===== PAGE 113 =====
100

chapter 3 동적계획

다. 이를 이루기 위해서 동적계획을 적용하는 절차는 다음과 같다.

1. 27『-'로부터 ps 계산하는 재귀 관계식(과정)을 정립한다.
8. k= 1부터 /까지(절차 1에서 정립한) 과정을 상향식으로 반복하여 문제의 입력사

례를 해결한다.
20 25 222 0 20                 (3,2)
t           t
WwW          yD)

음 두 가지 경우를 고려하여 절차 1을 수행한다.
후 1.  101,  Vag, sey uv, } Hl 속한 마디만 중간마디로 거쳐서 에서 도 가는 최단경로
중에서 최소한 SUE 0,를 거치지 않는 경우이다. 그러면 다음 등식이 성립한다.
D™ fj] = D& Maly              (3,3)
다음은 그림 3.8에서 이 경우의 예이다.
D®fi][3] = D{1)[3] = 8
왜냐하면, ;를 포함하더라도 0, 에서 v3 0H 가는 최단경로는 그대로 [y, v4, v3]°]71
문이다.
경우 2. {,, vg, …, 0, }에 속한 마디만 중간마디로 거쳐서 ,에서 《,로 가는 최단경로
는 모두 를 거치는 경우이다. 이 경우 어떤 최단경로라도 그림 3.4와 같이 된다. 는
,에서 《,로 가는 부분경로 상에서 중간마디가 될 수 없기 때문에 그 부분경로는 {0,,
00; …, Up } 에 속한 마디만 중간마디로 거치게 된다. 이는 다음과 같은 이유로 부분경
로의 길이가 2“ Y[i][k] 2} 반드시 같게 된다는 AS 암시한다. 첫째로 부분경로의 a
이는 더 짧을 수가 없는데 그 이유는 DE MARIE {0,, v2, +++) %-』}에 속한 마디만
중간경로로 거쳐서 1, 에서 #,로 가는 최단경로의 길이이기 때문이다. 둘째로 부분경로
의 길이는 더 길 수가 없는데, 왜냐하면 만약 더 긴 경우 그림 3.4에서 그 BBS 최단경
로로 대체할 수가 있어야 하는데, 그것은 그림 3.4의 전체 경로가 최단경로라는 사실에
위배된다. 비슷한 논리로, 그림 3.4에서 v, 4 《,로 가는 부분경로의 길이는 반드시
D“~ ik] Lj] ot 같아야 함을 알 수 있다. 따라서 경우 8에서는 다음과 같은 등식이 성립
한다.
DE] =D Male] + 28 비0001                       (3.4)

다음은 그림 3.204] 이 경우의 예이다.


===== PAGE 114 =====
* 예제 3.3

@0@000000
3.2 프로이드의 죄단경로 일고리즘     101

10; Up» …, Uy, FO 속한 마디만 거쳐서 《,에서 *,로 가는 최단경로
ONG
co                                                 ^
\ ee                    ae 재2202                    J

10 a, 에 속한 마디만   {v,, 01 애서 U_, }에 속한 마디만
거쳐서 에서 <,로 가는 최단경로 AAA 에서 《,로 가는 최단경로

그림 3.4 _최단경로가 를 사용하는 경우

D5][3] = 7 = 4+3= DB][2] + 2218

경우 1이나 경우 8 중 하나는 반드시 성립해야 하므로, 77 |/][/]의 값은 등식 (B.3)z}
비치      ae 최소값이 된다. 이는 다음과 같이 DO ee} ps 구할 수 있다

Ha = minimum(D"® Mall],   D*“"al[k] + 2『 0001)

경우 1

경우 2
동적계획 알고리즘을 설계하면서 절차 LS 수행했다. 그리고 절차 를 수행하기 위해

| 절차 1에서 구한 재귀 관계식을 사용하여 표현식 3.8에서 보여준 일련의 배열들을 만

는다. 그러면 어떻게 배열로부터 다음 배열을 계산하는지 예를 통해서 살펴보자.

그림 3.8에서 인접행렬 We 표현된 그림 3.8의 그래프를 가지고, 다음과 같이 계산을 일부 실행
ABAD = 임을 기억하자)
D™[2][4] = minimum (D][4], D2)[1] + 22011114])
=minimum(2, 9+1) = 2
D[5)[2] = minimum (D5) 2], D5]1) + DL] 2))
=minimum(oco, 3+1)=4
D5 [4] = minimum (D5 )[4], D[5]1] + 20114]
=minimum(co, 3+1)=4
일단 DY 전체를 계산한 후, DS 계산한다. 계산 일부를 Basal 다음과 같다.
D[5][4] = minimum (D[5][4], D[5][2] + D™ 2] [4]
=minimum(4, 4+2)=4
DS 모두 계산한 후 계속해서 차례대로 D© 72] 계산한다. 이 최종 배열이 Deja, 최단경로
의 길이이다. 이는 그림 3.3 오른쪽에 나타나 있다.

이제 플로이드010》0)가 개발하여(1962) “프로이드 알고리즘”으로 알려진 알고리즘을


===== PAGE 115 =====
@0@00000 0
102    chapter 3 동적계획

살펴보자. 알고리즘을 먼저 살펴본 후 왜 입력 배열 이외에 D 배열 하나만 사용하는

지를 ABIES 한다

 알29즘 33 플로이드의 최단경로 알고리즘
문제 : 가중치포함 그래프의 각 마디에서 다른 모든 마디로 가는 최단경로를 모두 계산하
시오. 여기서 가중치는 음이 아닌 수이다.
입력 : 마디 개수가 7인 가중치포함 방향그래프. 그래프는 8차원 배열 We 표현하는데,
행과 So} 인덱스 범위는 1부터 7까지이다. 즉,11111[)1는 정점 i Ba j= 가는 이음
선의 가중치이다.
출력 : 행과 열의 인덱스 범위가 1부터 7까지인 8차원 배열 D. 즉, Die 정점 iol
정점 JB 가는 최단경로의 길이가 된다.

void floyd (int n
const number W[][],
number DI ]| ])
{
index i, j, k ;
7220 = W
for (4 = 1; & <= 2; +)
for (7 = 1; 7 <= 2; 가+)
for ( / = 1 7 <= | j++)
Dili] = minimam( DLs], Aik) + DEEL):

배열 D 하나만 가지고 계산할 수 있는 이유는 《째 행과 《째 열에 있는 값들은 루프의
kal 반복을 실행하는 동안 변하지 않기 때문이다. 즉, 《째 반복에서 알고리즘은 다음과

같은 저장문을 실행하는데,
D{i][k] = minimum (D{i\[k], Dlé][k] + DIk][é])

여기서 Dik] [k] = 항상 0이므로 우변의 값은 의심의 여지가 없이 Dli][k] 7 된다. 그리
고 다음 저장문에서도

D{k] lj] = minimum (D[{k]Lj], Dlk][k] + Dik] ly)

D{k)[k) = 항상 0이므로 우변의 값은 의심의 여지가 없이 D[k][j] 7} 된다. 《째 반복을
실행하는 동안 Dl] Al 값과 kA 행과 kA 열에 있는 값들만 가지고 계산한다.
이 값들은 (k— 1) Al 반복에서 구한 값들이기 때문에 필요한 값들이다. 나제 언급했듯
이 동적계획 알고리즘을 설계할 때 저장장소를 절약할 수 있도록 알고리즘을 개선할 수
있는 경우가 종종 있다:

이제 플로이드 알고리즘을 분석해보자.


===== PAGE 116 =====
0000
32 프로이드의 최단경로 알고리즘

oa 은 두려

단위연산 : +0『-루프 안의 명령문(저장문)
입력크기 : 7/(그래프에서 마디의 개수)

=
루프 안

안에 루프 안에 루프가 있다. 이 루프는 각각 nwa 실행한다. 따라서

T(n)=nXnXn=n? © O(n’)

알고리즘 3.32 다음과 같이 수정하면 최단경로를 얻는다.
> 알29즘 3.4 플로이드의 최단경로 알고리즘 2

제 : 최단경로도 찾는다는 사실을 제외하고는 알고리즘 9.33} 동일
가적인 출력 : 행과 열의 인덱스 범위가 모두 1부터 7,까지인 배열 7. 여기서

34 더

+ [에서 0,717] 가는 최단경로의 중간에 놓여있는 마디가 최소한
끼101=1 하나는 있는 경우, 그 놓여있는 마디 중에서 가장 큰 인덱스
ㆍ 최단경로의 중간에 놓여있는 Bao] 없는 경우, 0

void floyd? (int 2,

const number W{][],
number DJ ][],

index P{][])

index, i, j, 4

for (7 = 1; 7 <= n ++)
for = 1; j <= n j++)
Pill 7] = 0;
D= W;
for (kK = 1; k <= n; k++)
for (¢ = 1; 7 <= n; H+)
for (7 = 1; 7 <= 2; +)
if (Dl i][k] + 가서] < 가기[기) {
Pill] = &;
[7] =

fe;
Di      Dik] + D&I];

알고리즘을 그림 3,29] 그래프에 적용하면 만든 배열 PE 그림 3.59} 같다.

=
다음 알고리즘은 배열 PS 가지고 정점 vA 《,로 가는 최단경로를 출력한다.


===== PAGE 117 =====
@000000 0
104    chapter 3 동적계획

> 알고리즘 3.5

그림 3.5 알고리즘 3.4를 그림 3.2의 그래프에 적용하여 만든 배열 P

최단경로 출력

문제 : 가중치포함 그래프에서 한 마디에서 다른 마디로 가는 최단경로 상에 있는 중간 마

디들을 출력하시오.
입력 : 알고리즘 3.4가 만든 배열 와 알고리즘 3.4의 입력인 그래프 마디의 인덱스
0와 7

+, HA @;까지 가는 최단경로의 중간에 놓여있는 마디가 최소한
끼0]1/]=1 하나는 있는 경우, 그 놓여있는 마디 중에서 가장 큰 인덱스
*ㆍ최단경로의 중간에 놓여있는 정점이 없는 경우, 0
출력 : 0,에서 《, 로 가는 최단경로 상의 중간 마디

void path (index 0, 2)

{

if (PAL g|[z] != 0){
path (q, P@l[r));
cn as 60 세 |] | :

path (PL q|[r], 7);

재귀 호출할 때 값이 변하는 변수만 재귀 함수의 입력 파라미터로 하기로 한 2장에서
부한 관례를 기억해보자. 따라서 값이 변하지 않는 배열 P= 20//,의 입력으로 두지
는다. PS AA(global) HSH 정의하고 vA] 《,로 가는 최단경로를 Hohe path
의 최상위 호출은 다음과 같다.

path (q,r);

그림 3.5의 P 값을 가지고, 0와 7의 값이 각각 59} 3이라면 출력 결과는 다음과 같다.

of

I>

ished


===== PAGE 118 =====
33 동적계획법괴

vl         v4

이 마디들은 에서 vy 2 가는 최단경로 상의 중간마디들이다.
알고리즘 8.5의 시간복잡도가 1) © O(n) 9] 증명은 연습문제로 남겨둔다.

3.8 동적계획과 최적화 문제

알고리즘 3.4는 최단경로의 길이를 구할 뿐만 아니라 최단경로도 구축한다. 최적 해답의
구축은 최적화 문제를 푸는 동적계획 알고리즘의 세 번째 단계이다. 따라서 동적계획 알
고리즘의 개발절차는 다음과 같다.
1. 문제의 입력사례에 대해서 최적(688091의 해답을 주는 재귀 관계식(:0049116
property)-& = 세운다.
2. 상향식으로 최적의 해답을 계산한다.
3, 상향식으로 최적의 해답을 구축한다.

단계 29} 8은 보통 동시에 이루어진다. 알고리즘 3 2& 최적화 문제가 아니므로 세 번째
단계가 빠져있다.

최적화 문제를 모두 동적계획법으로 풀 수 있는 것은 아니다. 문제에 최적의 원칙이
반드시 성립해야 한다. 최적의 원칙은 다음과 같다.

정의
어떤 문제의 입력사례의 최적해가 그 입력사례를 분할한 부분사례에 대한 최적해를 항상 포
고 있으면, 그 SAE 최적의 BAl(principle of optimality)O| 성립한다고 한다.

함하고

최적의 원적은 설명히기 HAA, WS 가지고 이해하는 편이 낮다, 최단정로 문제에
서 를 vA 로 가는 최적경로 상의 마디라고 하면, <,에서 = 가는 부분경로와
OA 0, 가는 부분경로도 반드시 최적이어야 한다. 그런데 입력사례의 최적해는 모
는 부분사례에 대한 최적 해를 포함하므로 최적의 원칙이 성립한다.

주어진 문제에 최적의 원칙이 성립하면, 부분사례의 최적해를 가지고 전체사례의 최적
해를 구하는 재귀 관계식을 세울 수 있다. 최적해를 구하는 문제에 동적계획을 적용할
수 있는 이유는 부분사례들의 최적해를 가지고 전체의 최적해를 구할 수 있기 때문이다.
예를 들어, 최단경로 BAW 부분경로들이 최단경로라면, 그것을 합한 경로는 최적이
된다. 그러므로 재귀 관계식을 가지고 상향식으로 점점 더 큰 사례에 대한 최적해를 구축
해나갈 수 있다. 그 과정에서 구한 해는 모두 항상 최적이다.

최적의 원칙은 어떻게 보면 당연한 것 같지만 동적계획을 적용하여 최적해를 구할 수
있는지 단정하려면 이 원칙이 성립하는지 증명해야 한다. 다음 예는 이 원칙이 성립하지


===== PAGE 119 =====
@eeeee 0
106    chapter 3 동적계획

© 예제 3.4

않는 최적화 문제도 있음을

각 마디에서 다른 모든 마디로 가는 가장 긴 단순경로를 구하는 최장경로 문제0008086 paths
problem) = 생각해보자. 최장경로 pa JS 단순경로만으로 제한하는 이유는 순환이 있으면 그 순
BS 통과하는 임의로 긴 경로를 항상 만들 수 있기 때문이다. 그림 3.6에서 vA) 로 가는
최적(최장)단순경로는 [0 , 8, v2, 70914 그러나 부분경로인 [,, %1이 어에서 0 으로 가는
최적(최장)경로가 아니라, [,, vw, 91이 최적(최장)경로이다.
length[v,, v3] =1과 length[v,, vo, v3] = 4
그러므로 최장경로 문제는 최적의 원칙이 성립하지 않는다. 이유는 vo] %으로 가는 최적경
로와 에서 로 가는 최적경로를 묶어서 0, 에서 = 가는 최적경로를 만들 수 없기 때문이다.
그러면 최적경로 대신 순환이 생기게 된다.

이 장의 끝까지 최적화 문제를 계속 다룬다. 알고리즘을 설계하는 과정을 설명하면서
동적계획 절차를 구체적으로 언급하지는 않을 것이다. 그렇게 하지 않아도 절차대로 진
행됨을 쉼게 간파할 수 있으리라 보기 때문이다.

@ 34 연쇄 행렬곱셈

2x3 행렬과 3×4 행렬을 곱하면 다음과 같이 계산한다.

123
|   |x 2345 |=
456        74 89 104 83

7891
ae 35 41 S
6789

계산 결과는 2x4 행렬이 된다. 행렬 곱셈의 정의에 따라 행렬 곱셈을 하면, 결과 행렬의


===== PAGE 120 =====
oN

| 원소를 구하기 위해서 원소단위 곱셈을 3회씩 실행한다. 예를 들면, 첫째 열의 첫째
Jats 다음과 같이 구한다.

ri

1X7+2X24+3X6
원소단위 곱셈 3회

곱셈의 결과가 되는 행렬에 2x4= 87] 원소가 있으므로, 원소단위 곱셈의 총 횟수는
다음과 같다.

2×4×83=24
일반적으로, ?×7 행렬과 7 ×《 행렬을 곱하면 원소단위 곱셈의 실행 횟수는 다음과 같다.
2×7>×&번

est 같이 4개의 행렬을 곱하는 문제를 생각해보자.

A xX B xX @ xX DM
20x2 230 3012 128

각 행렬의 크기는 행렬 이름 아래쪽에 표시되어 있다. 행렬곱셈은 결합법칙이 성립하므

로, 곱셈을 적용하는 SAE 결과에 영향을 미치지 않는다. 예를 들어, A(B(CD)) a

(4.29)(02)의 Wak: 같다. Wh) PAS BE 때 5가지 서로 다른 ONS 곱할 수 있는

데, 각 순서마다 원소단위 Bao] 횟수는 다를 수 있다. 위 행렬 Bale] 경우 각 순서
별 원소단위 곰셈의 횟수는 다음과 같다.

A(B(CD)) 30×12×8+2×30>×8+ 20 2x8 = 3,680
(AB)(CD) 20x 2x30+30 X12 8+20 X30 <8 = 8,880
A((BC)D) 2x3012+2x12*8+20X2x8=1,232
((AB)C)D 20x 2x 30+20 30x 12+ 20 12x 8 = 10,320
(A(BC))D 2x30 12+202x12+20 128 = 3,120

이 중에서 셋째 순서가 이 4개의 BAS 곱하는 최적의 순서가 된다.
그러면 7개의 PAS 곱하는 최적의 순서를 구하는 알고리즘을 설계해보자. 최적의
네처 행렬의 크기에만 의존한다. 따라서 ny} 행렬의 크기가 입력이다. 무작정 알고리
는 방금 해봤듯이 가능한 모든 순서를 고려해본 다음, 그 중에서 최소값을 주는
순서를 선택하면 ~ 무작정 알고리즘이 최소한 지수시간이 걸림을 증명해보자. nH
의 행렬(4, , Ay, ..., 4, )을 곱하는 BE 순서의 가지 수를 《, 이라고 하자. Ay 을 마지막
으로 곱하는 순서의 집합은 모든 순서 aes =    부분집합이다. 아래에서 볼 수 있듯이 이
부분집합에 속한 서로 다른 순서의 가지수는 《, _』 인데, 그 이유는 4;에서 4, 까지를 곱
할 수 있는 서로 다른 순서의 가지수이기 때문이다.

대!


===== PAGE 121 =====
108

chapter 3 동적계획

41(4248… 4.)

《, 개의 서로
다른 순서

또 다른 하나의 부분집합으로 4, 을 마지막으로 곱하는 순서의 집합을 생각해보자. 이
부분집합에 속한 서로 다른 순서의 가지수도 또한 《,。 _」이다. 따라서 다음과 같은 부등식
을 얻을 수 있다.

ty 2 tga thy. = 27

두 개의 PAS 곱하는 방법은 하나밖에 없으므로, 《, = 1이다. 부록 poy 있는 기술을
사용하면, 이 재현식의 해는 다음과 같음을 알 수 있다.

20 -

이 문제에서 aio] 원칙이 성립하는지를 알아보는 일은 어렵지 않다. 즉, 개 Wee
곱하는 최적의 SHE 7개 PAY 부분집합을 곱하는 최적의 순서를 포함한다. 예를
어, 6개의 행렬을 곱하는 최적의 순서가 다음과 같다면,

A, ((((A2A3) A) As) Ao)
행렬 AWA 4,까지 곱하는 AAS 순서는 반드시 다음과 같이 될 수밖에 없다.

이는 농적제획으로 해탑을 구일 수 Whe 걸 의미환더:

(k—-1) Al 행렬 4,_, 과 《째 행렬 A,S 곱하기 때문에 4,_,의 열의 수는 4,』의 BI
수와 같아야 한다. 예를 들어, 앞에서 살펴본 행렬곱셈에서 첫째 BAS 열의 수가 8이
고, SA 행렬은 행의 수가 3이다. 0; 을 A, 의 BS] 수라 하고, 1 <k< nl 모든 《에
대해서 d,s 4,열의 수라고 하면, A, 9] 크기는 41 ×0,가 된다. 이는 그림 3.7을 보
면 쉽게 알 수 있다.

앞 절에서 본대로 해답을 구축하기 위해서 일련의 MSS 사용한다. 1 스즈 7) 스 7

<-0-~

<--0-1- ~

                                                     1         Ak

Ak 2         461                    |

그림 3.7 4,_,의 열의 수는 4,의 행의 수와 같다.



===== PAGE 122 =====
© 예제 3.5

0000000
3.4 연쇄 행렬곱셈   109

인 모든 it 7에 대하여 다음과 같이 재귀 관계식을 구축한다.
Mil) =? < 7일 때 APE 4,까지 YAS 곱하는데 필요한

원소단위 곱셈의 최소 횟수
22410][11] = 0

이 배열을 어떻게 사용할 지를 알아보기 전에 이 배열 안에 있는 원소의 의미를 먼저
이해해보자.

다음 6개의 행렬이 있다고 하자.
A, X A, X A; X Ay X A; X Ay
5x2] Ox3 8x4 46 6xT 278
dy d,  d,  d,  d,  d;  d; d,  d,  d;  d;  de,
Ay, As, 4;을 곱하는데, 두 가지 순서에 대해서 필요한 원소단위 곱셈의 횟수는 다음과 같다.
(4.4.)4, 원소단위 곱셈의 횟수 =d; Xd, Xds4 4 Xd; X dg
=4x6X7+4X7X8 = 392
A,(A,4g) 원소단위 곱셈의 횟수 =d, xd; x dy 4, X dy X dy
=6X7X8+4X6X8=528
따라서, 4414]16]의 값은 다음과 같다.
2214]16] = minimum (392,528) = 392

6개의 행렬을 곱하는 최적의 순서는 다음과 같은 인수분해 중 하나가 되어야 한다.
. 41(42463414646)

. 24.4.)(464246460

. (474.432)0(4.4.4.)
1 {
에

_

A, A,A3A,A; )Ag

aa fF WO WD

여기서 각 괄호 안 PA] 곱은 최적의 순서에 따라 구한 것이다. 이 인수분해 중에서
원소단위 곱셈의 횟수가 최소가 되는 것이 최적의 해가 됨이 틀림없다. ka 인수분해의
곱셈의 횟수는 각 인수를 구하는데 필요한 최소 원소단위 곱셈의 횟수 더하기 두 인수를
곱하는데 필요한 원소단위 곱셈의 횟수가 된다. 따라서 다음과 같이 식으로 표현할 수
있다.

M(1][k] + M[k+ 1][6] + dod,d,

따라서 2711116]을 구하는 식은 다음과 같다.


===== PAGE 123 =====
110

chapter 3 동적계획

M(1][6] = 22222224272(7211]14] + M[k+ 1][6] + 4600.06 )
1<k<5
지금까지 설명하면서 첫째 BSS 4,이고 마지막 BAS 4,이 되어야 한다고 제한
두지는 않았다. 예를 들면, 4,부터 AS 곱해도 비슷한 결과를 얻을 수 있었을 것이
따라서 이 결과를 7개의 행렬을 곱하는 재귀 관계식으로 다음과 같이 일반화할 수 있
L<i<j<nQl BE 와 jo 대하여,

Miil[j] = minimum (M{i)[k] + 2416 + 1][j]+d;-1d,d;), if i<j  (3,5)

i<k<j-1

Miilli] = 0

nfo

233

이 관계식에 기초한 분할정복 알고리즘은 지수시간이다. 동적계획법으로 2410][7]의 값
을 단계별로 구하는 효율적인 알고리즘을 설계해보자.

파스칼의 삼각형(3.1절)과 비슷한 형태의 격자를 사용한다. 3.1절의 계산보다는 | 더
복잡하지만, 식 3.59] 다음 특성을 기초로 하여 계산을 수행한다. el) 값은 Mil]
와 같은 행에서 왼쪽에 있는 값 모두와 같은 열의 아래쪽에 있는 값 모두를 가지고 계산

:

fl

CHA 1 대각선 2 대각선3 대각선                      |선5

N      Ns      aN      NS      \ 6

1         0               30              64            799          226             348 < 최종 ©
A                A
2                                      0                      24                    72                   156                  268
3                                                               0                      72                   198                  366
L        6

4                                                                                         0                     168                  392
5                                                                                0               336
6                                                                                                  0

그림 3.8 예제 3.6에서 작성한 배열 24. 동그라미 쳐진 47111[4|는 표시된 부분의 쌍으로부터 계산
한다.


===== PAGE 124 =====
              * 예제 3.6

@   0000 0
3.4 연쇄 행렬곱셈 111

한다. 이 특성을 이용하면 MS] 값을 모두 다음과 같이 계산할 수 있다. 먼저 대각선상에
위치한 값을 모두 0으로 놓고, 다음에 대각선 바로 위에 위치한 값(대각선 1이라고 부름)
을 모두 계산하고, 다음에 대각선 8에 위치한 값을 모두 계산하고, 등등 이런 식으로 최
종 답인 대각선 Sol] 위치한 유일한 값 4711][6]을 계산할 때까지 계속한다. 예제 3.5의
행렬의 계산절차는 그림 3.8과 같다. 다음 예제에서 이 계산을 추적해본다.

예제 3.5의 6개 행렬이 있다고 하자. SAAS 알고리즘으로 계산하는 ARE 다음과 같다.
대각선 0의 계산 :
74100] =0, 1<i<6

22111121=72222220277(741]101 + Mk + 1)[2] + dyd,d,)

= Miu|u) + Malla] + dyd,a)2
=0+0+5x2x3=30
Mi2][3], 24814], 44415], 745116]의 값은 같은 방법으로 계산한다.
대각선 8의 계산 :
7211]13]=7222007021(721]0] + 724/6+1]131+ 0200.)

1 = 또고
= minimum ( M{1][1] + 4412]131+ 4040,
Mi1)[2] + 14{3][3] + dydqds )
= minimum(0+24+5x2x4, 30+0+5x3x4) = 64

Mi2]I4], 24315], 44416]의 값은 같은 방법으로 계산한다.
대각선 32] 계산 :
M{1\[4] = minimum (M{L1][k] + Mik + 1][4] + dod,d,)

143
= minimum ( 741]111+ 72412]144]1 + 4000,
2211][21+ 2213]14]1 + dydyd,,
2211113]+ 7414]4]+000,)
=minimum(0+72+5x2x6, 30+ㅜ72+5×3×6,
64+0+5x4x6) = 132

Mi2][5), 7413116]의 값은 같은 방법으로 계산한다.
대각선 4의 계산 :
대각선 4에 위치한 값은 같은 방법으로 계산한다.
대각선 5의 계산 :
마지막으로 대각선 5에 위치한 값은 같은 방법으로 계산한다. 이 값이 해답인데, 원소단위 곱셈
의 최소 횟수이고, 그 값은 다음과 같다.
2211]16] = 348



===== PAGE 125 =====
@0 00000 0
112    chapter 3 동적계획

> 알고리즘 3.6

이제 이 방법을 구현한 알고리즘을 살펴보자. 입력은 개 행렬의 크기(즉, 0, 부터 0,
까지)이다. 행렬 자체의 값은 필요 없기 때문에 입력으로 줄 필요가 없다. 알고리즘이 구
축하는 배열 PE 최적의 SAS 출력하는데 사용한다. 어떻게 출력할지는 알고리즘 3.6
을 분석한 후에 살펴보기로 하자.

All

최소 곱셈

문제 : 행렬 7개를 곱하는데 필요한 원소단위 곱셈의 최소 횟수와 최소 횟수로 행렬 곱셈
하는 순서를 구하시오.

입력 : 7:(행렬의 개수), 인덱스의 범위가 OE] 7까지인 정수 배열 0, 여기서 0[[-1|
×0[0]는 iva Ba] 크기가 된다.

출력 : minmult (nq VAS 곱하는데 필요한 원소단위 곱셈의 최소 횟수). PAA 순
서를 구할 수 있는 이차원 배열). 여기서 의 Bo] 인덱스는 1부터 7ㅡ1까지이고, 열으
인덱스는 1부터 7까지이다. 2212][7]의 값은 ?부터 7까지 VAS 곱할 때 최적의 순서로
갈라지는 기점을 나타낸다.

따

int minmult (int n,

const int 이],

index P{][])

index 2, j, k, diagonal;

int M[1..n] [1..2];

for (7 = 1; i <= n; H+)
Mil[i] = 0;

for (diagonal = 1; diagonal <= n—1; diagonal++)    // diagonal-12- 주 대각선의

for (7 = 1; 7 <= n-—diagonal; 가+){            // 바로 위에 있는
J = 1+ diagonal                           // AAAS 의미한다
441 7]17] =

minimum(M 기[4] + M&A + 4][2] + di-1)*dk]* dJ));

{= b= 7-1

Pilly] = 최소 횟수를 나타내는 의 값:;

return M[1][ a];

이제 알고리즘 3.62 분석해보자.

『 (최소 곱셈)의 일정 시간복잡도 분석



===== PAGE 126 =====
입력크기 : 7/(곱하려는 행렬의 개수)
루프 안에 루프가, 그리고 그 루프 안에 또 루프가 있다. 주어진 값 4000706과 8에 대해
서 7=1+04000708이므로, *-루프에서 실행하는 횟수는 다음과 같다.
j—1—-1+1=i1+diagonal—1—i+1= diagonal
주어진 diagonal 값에 대해서 for-i 루프에서 실행하는 횟수는 n— diagonal] 된다.
diagonal 2] 값은 1부터 7-1까지이므로, 단위연산을 실행하는 총 ASE 다음과 같다.
mal.

=      [((n — diagonal) x diagonal]

diagonal = 1

풀면 다음과 같은데, 유도하는 과정은 연습문제로 남겨눈다.

n(n—1)(n+1)
6

이식

ttlo

= O(n?)

이제 배열 POA) 최적의 순서를 구하는 방법을 알아보자. 예제 3.5에 알고
하면, 배열 P= 그림 3.99} 같다. 예를 들어, P[2][5 5] = 4라는 사실은 4, 부터 . Ay 행렬
같은

을 곱하는데 최적의 순서가 다음과 같은 인수분해로 나타남을 뜻한다.
여기서 괄호 안의 PAL 최적의 순서이다. 즉 P[2][5] 9] Be ela, 인수들을 얻기 위

해서 Bae] 분해되는 기점을 나타낸다. 최적의 순서를 구하기 ae  저 최상위 인
HE 구하는 Pllln]-& 방문해야 한다. n= 6이고 [11161 = 1이므로, 최적의 순서
를 주는 최상위 swat aa 같다.
A, (A,A3A,A;5Ag)

다음 A, Pe] 4,;까지 곱하는 최적의 SAS 구하는 인수분해는 P[2][6]-S 방문하여

1       1            1    1
2           2    3   4   5
3               3   4   5
4                   4   5
3                        5

그림 3.9 예제 359) 크기로 알고리즘을 적용하여 US 배열 P


===== PAGE 127 =====
@0@00@0000 0
114   chapter 3 동적계획

> 알고리즘 3.7

구한다. P[2][6] 2] 값은 5이므로, 그 인수분해는 다음과 같다.

지금까지의 구한 최적의 순서인 인수분해는 다음과 같다.

여기서 4;부터 4,까지 곱하는 인수분해를 결정해야 한다. 다음에는 121[5|를 보고,
이런 식으로 모든 인수분해를 알 때까지 계속한다. 최종 답은 다음과 같다.

문제 : 7/개 행렬을 곱하는 최적의 순서를 출력하시오.
입력: ?(양의 정수, "(알고리즘 3.6014 만든 배엘. 여기서 PLL 갖은 부터 까지
행렬을 곱할 때 AA] 순서로 갈라지는 기점을 나타낸다.

출력 : 행렬을 곱하는 최적의 순서

void order (index i, index ./)

{

if Gi —= 7)

cout <= “AY << 고

else {

k= Pills] ;
cout << “( ”
order (i, k) ;
order (4 + 1, J) ;
COllbmecen 9) 71

재귀 루턴을 작성하는 관습을 따라서 와 no] order 함수의 입력은 아니지만, 알고리
즘의 입력이긴 하다. 와 ns 전역으로 AMSA, order2] 최상위 호출은 다음과 같다.

order(1, 2) ;
예제 3.52] 경우, 이 알고리즘은 다음과 같이 출력한다.
(41((((4243)44)45)46))

전체 BAS Bees We} 있는 ote 알고리즘이 MERE 무조건 Bes 싸기 a
문이다. 알고리즘 3,79] 분석결과가 어떻게 다음과 같이 되는지는 연습문제로 남겨둔다.


===== PAGE 128 =====
연쇄행렬곱셈에 대한 O(n*) 알고리즘은 600601601973)이 만들었다. 그 후 Yao(1982)
는 동적계획 알고리즘으로 연쇄행렬곱셈을 푸는 O(n’) 알고
Shing(1982, 1984)은 후에 연쇄행렬곱셈을 하는 O(nlgn) da

@ 3.5 AA 이분검색트리

이분검색트리01081 search \ㅁ66)의 원소들을 최적으로 정리하는 알고리즘을 만들어 보
자. 어떻게 Eel(tree)S 정리하면 최적이 되는지 알아보기 전에 이분검색트리를 복습ㅎ
자. 이진트리061ㅁ817 166/에서 어떤 PC] (node)2] 왼쪽 자식마디(24410)를 뿌리(80000로
하는 하위트리를 그 마디의 왼쪽하위트리16[ 8406ㅁ60)라고 한다. 트리에서 뿌리의 왼쪽
트리는 그 트리의 왼쪽하위트리라고 한다. 오른쪽하위트리(019 subtree) = 비슷하게 정
의한다.

정의

O|ZAHE2|(binary search 『66)는 순서가능집합(606「60 set: 순서를

구성된 집합)에 속한 원소(키라고도 He 구성된 이진트리인데, 다음 AAS 만족한다.
1. 각 마디는 하나의 원소만 가지고 있다.
2. 마디의 왼쪽하위트리에 있는 원소들은 모두 그 마디의 원소보다 작거나 같다.
3. 마디의 오른쪽하위트리에 있는 원소들은 모두 그 마디의 원소보다 크거나 같다.

i 빌

그림 3.10을 보면 각각 같은 원소를 가진 이분검색트리가 두 개 있다. 왼쪽 트리에서
“Ralph” 마디의 오른쪽 하위트리를 보자. 그 하위트리에는 "2004 , “Ursula”, “Wally’7} 있
고, 알파벳 Ajo] 따르면 이 이름들은 BS “Ralph” 뒤에 온다. 일반적으로 보면 같은

4소가 이진트리에 두 번 이상 나올 수 있지만, 여기서 편의상 원소는 모두 다르다고 가
한다.

트리에서 마디의 깊이(06000)는 뿌리에서 마디로 가는 유일한 경로 상에 있는 이음
의 개수이다. 이를 트리에서 마디의 수준676])이라고도 한다. 보통 “마디는 깊이가 9
다.'라고 하든지, "마디는 수준이 몇이다"라고 한다. 예를 들어, 그림 3.10의 왼쪽 트리에
서 “Ursula” 마디는 깊이가 8라고 하기도 하고, 그 마디는 수준이 8라고 하기도 한다. 뿌
리는 깊이가 0이고, 수준도 0이다. 트리의 깊이는 그 트리의 모든 마디의 깊이 중 최대값
이다. 그림 3.10의 왼쪽 트리는 깊이가 3이고, 오른쪽 트리의 깊이는 2이다. 모든 마디의
두 하위트리의 깊이가 1 이상 차이나지 않는 트리를 균형잡힌 트리(68180ㅁ060 1\ㅁ66)라고
한다. 그림 3.10의 왼쪽 트리는 균형잡힌 트리가 아닌데, 그 이유는 뿌리의 왼쪽하위트리
의 깊이는 0이고, 오른쪽하위트리의 깊이는 2이기 때문이다. 그림 3.10의 오른쪽 트리는

ot 09 |
“Olt


===== PAGE 129 =====
116

chapter 3 동적계획

보동 이분검색트리는 검색키로 검색할 수 있는 레코드를 마디에 저장해두고 있다. 우
리의 목표는 이분검색트리에서 검색키와 같은 원소를 찾는데 걸리는 평균시간이 최소가
되도록 원소를 잘 정리하는데 있다(평균의 의미에 관한 자세한 사항은 부록 AS} 4.8.2절
을 참조하기 바란다). 그렇게 정리한 트리를 최적(6004791)이라고 한다. 각 원소가 검색
7\(search key)Y 확률이 모두 같다고 가정하면, 그림 3.10의 오른쪽 트리가 최적임을
바로 알 수 있다. 원소마다 검색키가 될 확률이 다르다고 가정하자. 예를 들어, 미국 사람
의 이름을 무작위로 추출하여 그림 3.10의 나무 중 하나에서 검색하는 경우를 생각해보
자. "700 이라는 이름은 "07648 라는 이름보다 더 흔하기 때문에 "0 에게 더 큰 확률
을 할당할 수 있다(무작위에 대한 자세한 사항은 부록 ㅅ의 4.8.1절을 참조하기 바란다).

이제 검색키와 같은 원소가 트리에 있는지 알고 있는 BPS 생각해보자. 검색키가 트
리에 없을지도 모르는 경우의 일반화에 대해서는 연습문제로 남겨둔다. 평균검색시간을
최소화하기 위해서 원소를 찾는 시간복잡도를 알아야 한다. 그러므로 더 진도 나가기 전
에 이분검색트리에서 원소를 찾는 알고리즘을 작성하고 분석해보자. 알고리즘에서 다음
과 같은 데이터구조를 사용한다.

struct nodetype

{
keytype key ;
nodetype* 762 ;
nodetype* right ;

}

typedef nodetype* node_ pointer ;

이 AMS HA node_pointer H7>+ nodetype BES 가리키는 포인터임을 알


===== PAGE 130 =====
수 있다. 즉, 그 값은 그 레코드의 메모리 주소가 된다.

RS 38 이분검색트리의 검색

문제 : 이분검색트리에서 검색키와 같은 원소가 있는 마디를 찾으시오, 찾는 원소는 나무
4

입력 : 이분검색트리를 가리키는 포인터 po} 검색키 keyin
출력 : 찾은 원소가 있는 마디를 가리키는 포인터 7

void search (node_pointer tree,

keytype keyin,
node_pointer& p)

{
bool found ;
p= tree ;
found = false ;
while (! found)
if (p—>key == keyin)
found = true ;
else if (keyin < p—>key) ;
p = p->left               // 윈쪽 자식마디로 간다
else
p= p—>vight              // 오른쪽 자식마디로 간다
}

원소를 찾는데 프로시저 search| 수행한 비교의 횟수를 AAYA|ZHsearch ㅁ160)이
라고 한다. 우리의 SHE 평균검색시간이 최소가 되는 트리를 찾아내는 것이다. 1.2절에
서 살펴본 대로 비교는 효율적으로 구현한다고 가정한다. 이러한 가정 하에서 위 알고리
즘에서 while 루프를 한 번 반복할 때마다 한 번씩 비교한다. 따라서 주어진 원소의 검
색시간은 다음과 같다.

depth(key) +1
여기서 depth(key)= 검색키와 같은 원소가 SO] YE 마디의 깊이이다. 예를 들어, 그림
3,102] 윈쪽에 있는 트리에서 “Ursula” 마디의 깊이는 2이기 때문에 “0848 의 검색시간
은 다음과 같다.
depth(Ursula)+1=2+1=3

Key,, Key), ..., Key, & 순서대로 나열한 n 72] 원소라 하고, pS il 검색키
일 확률이라고 하자. 주어진 트리에서 원소 Key, S 찾는데 필요한 비교 횟수를 <,라고
하면 그 트리에 대한 평균검색시간은 다음과 같다.


===== PAGE 131 =====
0000000
118   chapter 3 동적계획

이 값이 우리가 최소화하려는 값이다.

예제 37 그림 3.11을 보면 = 3인 경우 5개의 서로 다른 트리가 있다. 원소의 실제 값은 중요하지 않다.
여기서 BARE RAT GAS. HAUSE oleh 한다는 것이다 만약 2a eel 확

=
9]
isl

>, =0%, p02, p= 01

그림 3.11에 있는 트리의 평균검색시간은 다음과 같다.
1, 3 (0.7) + 2(0,2) + 10.10 = 2.6
2, 2 (0.7) + 3(0,2) + 100.1) = 2.1
3, 2 (0.7) + 1(0,2) + 2(0.0 = 1.8
4. 1 (0,7) + 3(0,2) + 200.1) = 1,5
5, 1 (0.7) + 2(0,2) + 3(0,1) = 1.4                                                 |

다섯째 트리가 최적이다.

fea
oy

그림 3.11 원소가 374 있을 때 이분검색트리의 종류

일반적으로 최적 이분검색트리를 찾기 위해서 가능한 종류의 이분검색트리를 모두 만
들어보는 건 현실적이지 않다. 왜냐하면, 트리 마디의 개수가 no] a, 다른 모양의 이분
검색트리의 개수는 최소한 지수(6600ㅁ00480)개이기 때문이다. 깊이가 n— 19) 모든 이


===== PAGE 132 =====
* 예제 3.8

@ @
3.5 최적 이분검

”  *  eee
분검색트리의 개수를 세어보면 지수가 된다는 사실을 보임으로서 이 사실을 증명해보자.
깊이가 7-1인 이분검색트리에서 뿌리를 제외하고 7-1개의 다른 수준에 있는 BEG
일마디(30816 ㅁ009)는 그의 부모마디의 왼쪽 아니면 오른쪽에 위치할 수 있다. 이는 이
는 수준에서 두 가지 가능성이 있다는 것을 뜻한다. 따라서 깊이가 7-1이 되는 다른
이분검색트리의 개수는 2” 개이다.
동적계획으로 더 효율적인 알고리즘을 만들 수 있다. Key HA] 468,까지의 원소들을
다음 식의 값이 최소가 되도록 트리에 배치했다고 가정한다.

i  CmuPm

72 =?

여기서 6, 은 그 트리에서 Key, 을 찾는데 필요한 비교 횟수이다. 이러한 트리를 그 원
소들에 대한 최적 Eel(optimal \ㅁ60)라 하고, 최적값은 4[2][7]로 표시한다. 원소가 하
나 있으면 트리에서 원소를 찾는데 비교를 한 번하므로, Ali] [i] = 2,이다.

예제 3.7을 다시 보자. 원소가 3개이고, 각 원소의 확률은 다음과 같다.
pi =0.7, py=0.2, p,=0.1

그림 3,129] 두 개의 트리를 가지고 412]13]을 구해보자. 각 트리에 대해서 다음과 같은 결과를
얻는다.

1, 1(p,) +2(p,) =1(0.2) +2(0.1) = 04

2. 2(p,) +1(p,) =2(0.2) +1(0.1) = 0.5
첫째 트리가 최적이므로, 다음과 같은 최종값을 얻는다.

A(2][3] =

그림 3.12 Key, Key,le 구성된 이분검

예제 8.8에서 구한 최적트리는 그림 3, 7A] 구한 최적트리의 오른쪽하위트리이다. 비
록 이 트리가 오른쪽하위트리와 정확히 같지는 않지만, 검색하는데 소비한 평균시간은
같아야 할 것이다. 그렇지 않으면 그 부분을 그 하위트리로 대체할 수도 있을 것이다.
일반적으로, 최적트리의 하위트리는 그 하위트리 안에 있는 원소들에 대해서 반드시 최
적이어야 한다. 따라서 최적의 원칙이 성립한다.


===== PAGE 133 =====
120    chapter 3 동적계획
각 원소에 대해서 뿌리에서
추가로 한 번 더 비교한다.
이 하위트리의           S             이 하위트리의
평균검색시간은                                   평균검색시간은
A(1][k — 1]이다.                                                          A{k +1][n]O| Ct.

yeeey

그림 3.13 Key,7} 뿌리

[을

경우 최적 이분검색트리

트리 1을 Key,o] 뿌리라야 한다는 제한을 가진 최적트리라 하고, 트리 2S 468;가
뿌리라야 한다는 제한을 가진 최적트리라고 하며, ..…, 트리 을 Key, o] 뿌리라야 한다
는 제한을 가진 최적트리라고 하자. 1 < & <n 모든 kel] 대해서 트리 ko] 하위트리
는 반드시 최적이어야 한다. 따라서 이 하위트리들의 평균검색시간은 그림 3.18에서 보
여주고 있다. 이 그림을 보면 m= kel 모든 mo] 대해서 트리 ko) Key, S 찾는데
수행하는 비교 횟수는 그 MAT} 있는 하위트리에서 그 원소를 찾는데 수행하는 비교 횟
수보다 정확히 하나 더 많다(여기에서 뿌리에서 추가적으로 한 번 더 비교한다). 이 한
번의 비교 때문에 트리 *에서 Key, & 찾는 평균검색시간은 1×7, 만큼 늘어난다. 결과
적으로 트리 《에 대한 평균검색시간은 다음과 같다.

4091] + pte +04 + pm + Alktiln] 0 70007 90 +7,

왼쪽하위트리          뿌리에서 비교하는데 뿌리를 검색 오른쪽하위트리       뿌리에서 비교하는데
에서 평균시간             드는 추가시간         하는 평균시간 에서 평균시간           드는 추가시간

이 식을 정리하면 다음과 같다.
A[t][&-1]+ Alk+ tin] + 23,

개의 트리 중 하나는 반드시 최적이기 때문에 최적트리의 평균검색시간은 다음과 같다.

A[t][n] = minimum(A[1][k—-1] + A[k+1][n]) +  > De

Laka n                  m=1

여기서 A[1][0] 2} A[n+ 1][n] 2 0으로 정의한다. 이 마지막 식에서 확률의 합은 명백
히 1이지만, 그 결과를 일반화하고 싶기 때문에 합이라고 썼다. 이전에 설명한대로 꼭


===== PAGE 134 =====
> 알고리즘 3.9

0000000
3.5 최적 이분검색트리    121

원소가 Key 부터 Key, AAD 필요는 없다. i<j 때 Key ZH] Key, 712 일반화
하여 설명해도 상관없다. 따라서 최종적으로 다음의 일반식을 얻는다.

Ali]lj] = minimum (A[i][k-1] + A[k+ 11171) + 22. 2. 20, <j

i<k<j

Ali] [i] =p;                                                                  (3.6)
Ali][ii—1] = 0
Alj+1][j]=0

등식 B.S 사용하여 최적 이분검색트리를 구하는 알고리즘을 작성할 수 있다. 4 [?][7]
의 값은 (알고리즘 8.6에서 하듯이) 410][)]의 왼쪽 값을 제외한 ?째 행에 위치한 값들과
4101121의 아래 값을 제외한 FA 열의 값들을 가지고 계산하기 때문에 각 대각선에 있는
값늘을 차례로 계산해 나간다. 알고리즘이 진행되는 절차는 알고리즘 3,63} 비슷하므로
이 절차를 보여주는 예는 들지 않기로 한다. 대신, 그냥 알고리즘을 보여주고, 알고리즘
을 적용한 결과를 자세히 보여주기로 한다. 알고리즘이 만든 배열 AS 각 단계마다 뿌리
에서 선택된 원소의 인덱스를 가지고 있다. 예를 들어, 2[1112]는 처음 두 원소를 가지고
있는 최적트리의 뿌리에 있는 원소의 인덱스이고, ?[2][4]는 둘째, 셋째, 넷째 원소를
포함하는 최적트리의 뿌리에 있는 AL 인덱스이다. 알고리즘을 분석한 후, 어떻게 R
에서 최적트리를 구축하는지 알아보도록 한다.

mi

최적 이분검색트리

문제 : 주어진 원소의 집합을 가지고 최적 이분검색트리를 구축한다. 여기서 각 원소에 대
해서 검색키가 될 확률이 주어진다.

입력 : /,(원소의 개수), 7(인덱스의 범위가 1부터 7까지인 실수 배열). 여기서 pli]= iA
Jas 찾을 확률이다.

: 변수 2222478(이 값은 최적 이분검색트리에서 평균검색시간), 최적트리를 구축할
이차원 배열 A. 여기서 RS] 행의 인덱스 범위는 1부터 7+1까지이고, 열의 인덱
0부터 /까지이다. 221][7]는 ?째부터 JAVA] 원소를 포함한 최적트리의 뿌리
에서 원소의 인덱스이다.

be

]

> 4> my qe
nz, xo, 끄

de rir
clr

으

void optsearchtree (int n,

{

const float p[],
float& minavg,
index R[]|[})

index 1, 7, k, diagonal;

float A[l..2 + 1] [0.. a];

for (f= 1;i< = 2; H+){
제기 |: 1 | = 0:


===== PAGE 135 =====
@‥0@00000 0
122   chapter 3 동적계획

A[ i] [7]
Ri) [4]
[i] [7
}
Aln + 1][ 2

0;
Rin + ifn] = 0;
for (diagonal = 1;

| =

diagonal < = 21; diagonal++)

for (7 = 1; 7 <= n — diagonal; i++){      // diagonal—12 주 대각선 위에 있다.
J = 7 + diagonal;
2|2]11./] = minimum(A[ /][4— 1] + A[k+1][7]) + 기 Bx

Rl ][] ] = ALS 주는 4의 값;

}

minavg = A[1][ 2];

> 알고리즘 3.10

POUR 시간복잡도 분석(최적 이분검색트리)

단위연산 : *의 각 값에 대해서 실행하는 명령문. 명령문에는 최소값인지 검사하는 비교도

포함되어 있다.  회 Pn 의 값은 매번 처음부터 계산할 필요가 없다. 이 BS 계산하는 효

율적인 방법을 RE 것은 연습문제로 남긴다.

입력크기 : 7/(원소의 개수)

이 알고리즘의 제어구조는 알고리즘 3,63} 거의 유사하다. 차이점이라면 diagonals} i]
주어진 값에 대하여 단위연산을 diagonal + 1¥ 실행한다는 것이다. 알고리즘 3.6과 같이

분석을 실행하면 다음과 같은 분석 결과를 얻는다.

2 = 별 90 E O(n?)

알고리즘은 배열 #에서 이진트리를 구축한다. KL 각 단계마다 뿌리에서 선택
된 원소의 인덱스를 포함하고 있음을 명심하자.

db

문제 : 최적 이분검색트리를 구축하시오.

입력 : 7(원소의 개수), 7개 원소를 순서대로 나열한 배열 Key, 알고리즘 3.9에서 만든
배열 고. 여기서 212][7]는 8째부터 째까지 원소를 포함한 최적 트리의 뿌리에서 원소의
인덱스이다.

출력 : 원소가 7?개 최적 이분검색트리를 가리키는 포인터 tree


===== PAGE 136 =====
@‥ㅎ00000 0
3.5 최적 이분검색트리    123

node_ pointer tree (index i, J)

{

index 4;
node_pointer p;

k= 찌기[7];

if (k == 0)
return NULL ;

else {
p = new_nodetype ;
2 ~ key = Key k];
p—> left = tree (i, k = 1);
p—> right = tree (k + 1, J);
return PD;

명령문 p =new_nodetype& 새로운 마디를 만들어서 그 주소를 pol 저장한다. 재귀
알고리즘의 관습에 따라서 파라미터 7, Key, 은 tree 함수의 입력이 아니다. 2 , Key,
RZ 전역변수로 하고 알고리즘을 구현하면 최적 이분검색트리의 뿌리를 가리키는 포인
터 root= 다음과 같이 trees 호출하여 얻는다.

root = tree(1, n);

알고리즘 3,99] 실행절차는 알 Seo 비슷하므로 자세히 설명하지 않

는다. 알고리즘 8.10의 실행절차도 알고리즘 3.(최적순서 출력)과 비슷하므로 자세히 설
명하지 않는다. 대신 알고리즘 8.  aac 적용하여 얻은 결과만 자세히 보여주기로
한다.

* 예제 3.9     배열 Key2| 값이 다음과 같다고 하자.

| Don | Isabelle | Ralph | Wally |
6711]  Key[2]  Key[3] _— Key[4]

그리고 각 원소의 확률이 다음과 같다고 하자.

알고리즘 8.9로 만든 배열 A} #은 그림 3.14와 같고, 알고리즘 8.10으로 만든 트리는 그림 3.15
과 같다. 최소 평균검색시간은 7/4이다.

씨111|는 1일수도 LIFE 있음을 주목하자. 그 이유는 이중 어떤 인덱스도 처음 두 원소
포함하는 최적 트리에 있는 뿌리의 인텍스일 수 있기 때문이다. 따라서 이 F 인덱스 모두
리즘 3.9에서 40101의 최소값을 준다. 이는 둘 중 어떤 값도 #01101의 값으로 선택할 수 gh
을 의미한다.



===== PAGE 137 =====
124       chapter 3 동적계획
0      1      2      3     4                0      1      2      3     4
3       9       11       uA
1] 0     3s 8 8 «4           1] 0      1      1      2      2
6)      5
2           0     3 8     1            2           0     2      2      2
1      3
3                 0     ㅎㅎ           3                 0      3      3
1
4               0   eB      4               0   4
5                   0       5                   0
4                           R

Isabelle

그림 3.15 알고리즘 3.92} 3105 예제 3.92] 사례에 적용시켜서 만든 트리

(ql

이장에서 공부한 최적 이분검색트리 구하는 알고리즘은 86166와 Moore(1959)7} 만
것이다. SAAS 속도향상 AS 사용하면 O(n’) 알고리즘을 만들 수 있음
Yao(1982)7} 밝혀냈다.

7

fu

@ 3.6 4a 문제

외판원이 207] 도시로 판매출장을 계획하고 있다고 가정하자. 각 도시는 다른 몇 개 도시
와 도로로 연결되어 있다. 출장시간을 최소로 줄이기 위하여 외판원이 거주하고 있는 도
시에서 출발하여 각 EAS 한 번씩 방문하고, 다시 출발한 도시로 돌아오는 가장 짧은
여행길을 찾고 싶다. 이런 최단 여행길을 구하는 문제를 외판원 문제(876408 68168-
woman 280016200라고 한다.
이 문제는 마디(76668, node) = 도시로 하여 가중치포함 그래프로 표현할 수 있다.
8.2절에서와 마찬가지로, 한 방향으로 가는 가중치(거리)가 그 반대방향으로 가는 가중
치와 다를 수 있도록 문제를 일반화한다. 여기서도 가중치는 음이 아닌 정수로 가정한다.
가중치포함 그래프의 예는 그림 3.2와 3,160] 있다. 방향그래프에서 일주여행길604)[해
밀톤 회로(861011001870 0704119)라고도 함]은 한 도시에서 출발하여 다른 모든 도시를 한



===== PAGE 138 =====
06000000
3.6 외판원 문제    125

그림 3.16 최적 ASE |v, vg, vy vo, 히]이다.

번씩만 들리고 출발한 도시로 돌아오는 여행길이다. 가중치포함 방향그래프에서 최적일
주여행길(6041081 1040)은 그러한 여행길 중에서 최소거리 여행길이다. 외판원 문제는
최소한 하나의 일주여행길이 SASH 경우 가중치포함 방향그래프에서 최적일주여행길
을 찾는 문제이다. 출발하는 도시가 최적일주여행길의 길이와는 상관없으므로, 6, 을 출
발도시로 잡는다. 그림 3162] 그래프에서 3개의 일주여행길과 그 길이를 알아보면 다음
과 같다.

length |v, V2, V3, U4; v, |= 22

length|v1, Vg, Vg, V4, v1] = 26

length |v,, U3, U4) 06: v,|= 213

위에서 마지막 일주여행길이 최적이다. 가능한 일주여행길을 다 고려해 보고 이 사례
의 해답을 찾았다. 일반적으로 보면, 각 도시에서 다른 모든 도시로의 이음선이 존재할
수 있다. 가능한 모든 일주여행길을 다 고려하면, 일주여행길에서 둘째 도시는 7-1개
의 도시 중 하나일 수 있고, 일주여행길에서 셋째 도시는 7-2개의 도시 중 하나일 수
있고, .…, 일주여행길에서 nA] 도시는 하나뿐이다. 따라서 일주여행길의 총 가지 수는
다음과 같으며,
(02-1)(02-2)…1= (02-1)!

이는 지수개보다 많다.

SAAS 이 문제에 적용할 수 있을까? v1, 7} 최적일주여행길 상에서 v, 다음에 오는
첫 번째 도시이면, 0, O14 이로 가는 일주여행길의 부분경로는 다른 도시를 각각 정확히
한 번씩만 거치며 0,에서 | 로 가는 최단경로이어야 한다. 이는 최적원칙이 성립하고,
동적계획을 적용할 수 있음을 의미한다. 8.9절에서 하던 대로, 그래프는 인접행렬로 표
현한다. 그림 8.1/에 그림 3.162] 그래프를 인접행렬로 표현해 놓았다. 몇몇 필요한 용어
를 정의해보자.

= 모든 S/S) 집합


===== PAGE 139 =====
@0@00@0000 0
126    chapter 3 동적계획

110  2  9  00

211   0   6   4

3] © 7 0 8

416   3   00   0
그림 3.17 그림 3.16에 있는 그래프의 인접행렬식 표현 1"

A= V9] 부분집합
Div,][A] = Al 속한 도시를 각각 한 번씩만 거쳐서

,에서 , 로 가는 최단경로의 길이

* 예제 310 그림 3,169] 있는 그래프에 대해서,
= {에 Vg, Vg, U4}
집합은 SATS 사용하여 {v,, vq, vg, vi} 와 같이 표현하는 반면, 경로는 대괄호를 사용하여
[or 89 Ug v4] St 같이 BASH, 4=1%}이면, 2210.1141는  Sah a 계산한다.

21414 ]=length[v,, Us; 이]

A= {vg 4} 이면, DAA] 다음과 같이 계산한다.

2210] = minimum (length |v, v3, Vy 이], Length lve, v4, V3» 이)

= minimum (20,00) = 20

집합 V— (vy, 0, }는 4, 과 oS 제외한 BE 도시를 포함하고 있고, 최적원칙이 성립
하므로 다음과 같은 식을 얻는다.

최적일주여행길의 길이 = ㅠ88%ㅠ(14111[71|+ Dly|[V—{v,, v,}])

25950
그리고 일반적으로 ?=1이고 :가 Al] 속하지 않으면, 다음과 같은 관계식을 얻는다.
D\v;][A] = minimum ( Wi] lj] + Dlv,|[A— {vj}]), 4 = 0
JivjEAa                                                 (3,7)
Div, [o] = Wie][1]
Al (3.7)을 이용하여 외판원 SAS 푸는 동적계획 알고리즘을 작성할 수 있다. 그러나
먼저 어떻게 알고리즘이 작동하는지 살펴보자.

* 예제 311 그림 3.17에 있는 그래프에서 최적일주여행길을 구해보자.


===== PAGE 140 =====
> 일고리즘 3.1

3.6 외판원 문제      127
Div.][2]=1
Divs]|@] = 00
Div, |[9] =6

먼저 공집합인 경우를 알아보자.
Dios]l{v,}] = minimum ( Waly] + Devjlltv,} — {v,})

j:rjE {v.}

= Wi3][2]+ Div,][o] = 7 + 1 = 8

다음으로 하나의 원소만 있는 집합의 경우를 알아보자.

210.1110.}]= 8 ㅜ1=4

az ie  6 +00 =00
]
]

J=   00 + co + co
『 [{v,}] =4+6=10
Divs|[{v,}] =          =14

나머지는 비슷한 방법으로 다음과 같이 구한다.
210], v3 }] = minimum ( Wid] lj] + Dip, ][{v2, v3} — {v;}])

G30; S{vy, vs}
= minimum ( Wi4][2] + Divg][{v3}], W14][3] + Divg][{v, }])
=minimum(3+00, 0 +8) =
다음, 두 개의 ALS 가진 집합의 경우를 알아보자.
기법], v4 }] = minimum(7+10, 8+4) = 12
Div|[{v3, v4 }] = minimum (6+14, 4+ 00 ) = 20
나머지는 비슷한 방법으로 다음과 같이 구한다.
마지막으로 최적일주여행길의 길이를 계산해보자.
끼어], v3, v4 }] = minimum ( 1441)][21 +Dip,l[{o,, 0, %}-  {v;}])

jiu; S{v,, vs, v4}
= minimum ( Wi1][2] + Divll{v5, vt);
W11][3] + DioslI{v., v4],
Wi1][4] + Dey ll{v., vs }])

= minimum (2+20, 9+12, co +00) = 21

다음은 외판원 문제를 푸는 동적계획 알고리즘이다.

외판원 문제를 푸는 SAAS 알고리즘

문제 : 가중치포함 방향그래프에서 최적일주여행길을 결정하시오. 가중치는 So] 아닌 정
수이다.

입력 : 가중치포함 방향그래프, 7(그래프에서 도시(마디)의 개수). 그래프는 행과 열의 인


===== PAGE 141 =====
@eeeee 0
128    chapter 3 동적계획

덱스의 범위가 모두 1부터 /까지인 3차원 배열 WH 표현한다. 여기서 Wills] 1번째
도시에서 번째 EAS 연결하는 이음선의 가중치이다.

출력 : 변수 minlength ©] 변수의 값이 최적일주여행길의 길이가 된다), 8차원 배열 P
(이 배열을 가지고 최적일주여행길의 ARS 구축할 수 있다). Po Be 인덱스 범위가
1부터 #까지이고, AL 인덱스 범위가 V—(v,} 의 모든 부분집합이 된다. 2[1][41는 A
에 속한 모든 ENS 정확히 한 번만 거쳐서 에서 vB 가는 최단경로에서 v, 다음에
오는 첫 번째 도시의 인덱스이다.

void travel (int 22,
const number W][],

index F{][],

number& minlength)

index i, j, k;
number D[1 .. | [subset of V —{v,} ] ;

for (i = 의 7 <= 03 H+)
Di) [90] = Mill) ;
for (kK = 1; k <= n-—2; +)
ion (A EV {S 만족하며 마리가 4&개인 모든 부분집합 A)

for (4 12} 0, € AS 만족하는 모든 2){
2212114] = minimum (Wii) lj] + DIA - {oj 1);
j:v;EA
Pli)[A]=347} 되는 /값 ;
}
D[V— {v,}] = minimum (Wi1)L7] + DILV— 10, 2 }]);

25jsn

PULU[V— {v, }]=최소가 SE SH;
minlength = D[1][V— {v,}] ;

배열 "에서 최적일주여행길을 어떻게 SEZ] 알아보기 전에 알고리즘을 먼저 분석해
보자. 먼저 Bel(theorem)7} 필요하다.

『정리 3.1
= 1인 모든 no] 대해서 다음 등식이 성립한다.
가가 ee

명 : 다음 등식이 성립함을 보이는 것은 연습문제로 남긴다.

oly


===== PAGE 142 =====
@000000 0
3.6 외판원 문제   129

마지막 등식은 부록 AS] 예제 4.10에 있는 결과를 적용하여 얻는다.

알고리즘 3.2 다음과 같이 분석한다.

『일정 시간/공간 복잡도분석(외판원 문제를 푸는 동적계획 알고리즘)

막 루프를 실행하는데 걸리는 시간은 중간루프와 비교하면 극히 작
여러 ALS 중첩되어 있기 때문이다. 따라서 v, 9] 각 값을 실행
하는 명령문을 단위연산으로 하도록 한다. 단위연산은 덧셈 연산도 포함한다.

입력크기 : 7/(그래프에서 도시의 개수)

《개 도시를 포함하고 있는 각 집합 4에 대해서 7-1-《개의 도시를 고려해야 하고,
이 도시들에 대해서 각각 단위연산을 《번 실행한다. 《개 EAS 포함하고 있는 V—{v}
의 부분집합 의 개수는 |",  a. 단위연산을 실행하는 총 횟수는 다음과 같다.

다음 등식이 성립하는지 증명하기는 별로 어렵지 않다.
0-1-씨"은 ]=6-피"기
이 등식을 식 (3.8)에 치환하면 다음과 같다.

n—2
0)= be", |
마지막으로, 정리 31 적용하면 다음을 얻는다.
T(n) = (02-1)(02-2)2" 00 (0272)
이 알고리즘이 사용한 메모리도 양이 방대하므로, 메모리(공간)복잡도 42(72)을 분석해보
자. 배열 D[v,][A] 2} 씨0,][4]를 저장하는데 사용한 메모리는 명백히 전체의 거의 대부


===== PAGE 143 =====
@0@00000 0
130    chapter 3 동적계획

© 예제 3.12

분을 차지한다. 따라서 이 배열의 크기가 열마인지 알아본다. 「-{0, } 은 7ㅡ1개의 도
시를 포함하고 있으므로, 부록 에서 예제 A109] AWS 적용하여 부분집합 의 개수가
o" '개라고 결론지을 수 있다. 배열 DS} 2의 처음 인덱스의 범위는 1과 사이이다. 따
라서

M(n) = 2×72" = 722"ㅎ0 (022")

이 시점에서 우리가 얻은 게 무엇인지 의아해할 지 모르겠다. 왜냐하면 새로 개발한
알고리즘도 아직 O(n72")0]7] 때문이다. 다음 예제를 보면 별로 효율적인 것 같아 보이
지 않는 시간복잡도를 가진 알고리즘도 때로 유용할 수 USS 알 수 있다.

갑돌이와 갑순이는 둘 다 같은 외판원 자리를 놓고 경합 중이다. 상관이 금요일 둘에게 말하기를
다음 월요일부터 시작하여 20개 도시 AAS 더 빨리 다녀올 수 있는 사람이 외판원 자리를 차지
할 것이라고 선언했다. 사무실에서 출발하여 일이 끝난 후에는 반드시 사무실로 되돌아 와야 한
다. 모든 도시 사이에는 도로가 깔려있다. 갑돌이는 자신이 다녀야 할 노선을 알아내는데 긴 주
말이 있다는 A 간파하고, 무작정 알고리즘을 자신의 컴퓨터로 수행하여 (20ㅡ1)!개가 되는 일
주여행길을 모두 조사해보기로 했다. 갑순이는 알고리즘 강의에서 동적계획을 배웠다는 사실을
기억했다. 가능한 모든 수단을 동원하기로 한 그녀는 그녀의 컴퓨터로 그 알고리즘을 실행하였
다. 갑순이의 알고리즘에서 단위연산을 처리하는데 걸리는 시간이 1010ㅎ0800000라 하고, 갑돌
이의 알고리즘에서 각 여행경로의 길이를 계산하는데 걸리는 시간을 120100860000라고 가정해
서, 각 알고리즘을 수행하는데 걸리는 시간은 대략 다음과 같다.
무작정 알고리즘 : 19! ps =38574

동적계획 알고리즘 : (20-1)(20—-2)2" 3 ws =45%

AlSA)ZHfatorial-time) 알고리즘의 대안으로, ㅇ(',7"2") 알고리즘조차도 쓸모가 있다는 얘기이
다. 이 예제에서 동적계획 알고리즘이 사용한 메모리의 크기는 다음과 같다.
20 x 2° = 20,971,520 배열 슬롯
꽤 많은 bee ales 오늘날 기준으로 보면 가능하다.
@(7272")                                    을 찾는 일은 7이 작은 경우만 실현 가능하다.
예를 들어,  2 도시가 있는 경우 의 알고리즘도 수년이 걸리기 때문이다.

배열 PHA 어떻게 최적일주여행길을 찾아내는지를 알아보자. 알고리즘을 설명하는
대신, 알고리즘이 어떻게 진행되는지만 간단히 살펴보기로 한다. 그래프에서 최적일주
행길을 구하는데 필요한 배열 의 멤버는 다음과 같다.

3                    4                 2
Pi, 105 V3) v,}]        PB, 106, v,}]        PI4, {v,}]



===== PAGE 144 =====
@0‥000000
3.7 DNA 서열 정렬   131

여기서 최적일주여행길은 다음과 같이 구한다.

첫째 AAS] MAA = Pli][{vo, vg, 0. }] = 3
|

V
둘째 정점의 인덱스 = Pls|[{v., vy }] =4

셋째 정점의 인덱스 = 끼14][{ 0, }]= 3
최적일주여행길은 따라서 다음과 같다.
10, U3) U4) U2) v|

지수보다 좋은 외판원 문제를 푸는 알고리즘을 찾은 사람은 아직
다. 그런 알고리즘이 없다고 증명한 사람도 아직 아무도 없다. 이러한 특성을
공유하고 있는 여러 문제 중 하나이며, 뒤에 9장에서 상세히 공부한다.

3.7 DNA 서열 정렬

동적계획법을 분자유전학 분야인 동족 DNA 서열 4 (homologous DNA sequence 811-
gnment) 문제에 응용해보자. 먼저 유전학 개념부터 알아보자.

염색체(01002000802006)는 복합 DNA(deoxyribonucleic 800)로 구성된 실같이 긴 거대분

자이다. 염색체는 생물학적으로 표현된 유전적 형질을 지니고 있다. DNA 두 개의 상반

된 타래로 구성되는데, 각 타래는 ion 서열로 이루어진다. 뉴클레오티드(ㅁ4-
cleotide)= 2"tG(deoxyribose)F} 인산염(0708208816)과 퓨린(6041100) 또는 피리미딘
(pyrimidine) 포함하고 있다. 퓨린 ‘i 아데닌(4)과 구아닌(@)은 구조적으로 피리미던인
시토신(0)과 티민(1)과 유사하다. 타래는 뉴클레오티드 Yo] 수소결합으로 연결된다. oF
AUS 티민과 WS 이루고, 구아닌은 시토닌과 YS 이룬다. 각 쌍을 표준 염기쌍(6886
pair, 60)이라 하고, A, @ C, TS 염기06889)라고 한다.

1044의 섹션(66004020)은 그림 3.18과 같은 모양으로 구성된다. 타래는 오른쪽 방향으로
이중나선형으로 꼬인 형태이다. 그러나 편의상 그림과 같이 문자열로만 생각하기로 한
다. 염색체는 28 분자가 길게 Hoje 걸로 보면 된다.

DNA 서열(66046006)는 DNAS] 섹션이고, 사이트(616)는 서열에서 염기쌍이 위치한 장

fo)

소를 나타낸다. DNA ASS 뉴클레오티드가 서로 바뀌는 교환 SA4O|(substitution
A 6 6 1 6 ^ 6
T GC A GTC

그림 3.18 DNAS) 섹션


===== PAGE 145 =====
@0000000
132    chapter 3 동적계획

© 예제 3.13

mutation) 2} 염기쌍이 서열에 끼어들어가는 삽입 SA Ao|(insertion mutation) 2} 염기
쌍이 서열에서 사라지는 제거 돌연변이(4010010ㅁ mutations 겪는다.

특정 집단(종)에서 같은 DNA ASS 가진 개체가 있다고 하자. 다음 세대의 개체를
만들어내는 각 배우자가 ASS] 각 사이트에서 겪을 돌연변이의 확률이 세대별로 각각
다르다. 집단 전체 또는 대부분에서 특정 사이트의 염기쌍이 교환될 수 있다. 경우에 따
라서 새로운 종이 형성될 수도 있는데, 하나의 종이 둘로 분리되는 현상이다. 이 경우
분리된 각 종에서 염기쌍의 교환 패턴은 상당히 달라질 수 있다. 두 개의 종에서 꺼낸
개별 서열이 많이 다를 수 있다는 뜻이다. 이를 서열이 분기되었다고 하고, 분기된 각각
의 서열을 FSA A(homologuous 86046006)이라고 한다. 서로 다른 종끼리 동족서열을
비교하여 진화 측면에서 종족 간의 거리가 얼마나 되는지 추정할 수 있다.

른 종의 두 개체의 동족서열을 비교할 때 서열을 먼저 나열해봐야 한다. 왜냐하면,

분리된 이후 서열 중 하나만 또는 모두 삽입/제거 돌연변이를 겪었을 수 있기 때문이다.
예를 들어, 인간과 올빼미원숭이 eles 유전자의 첫 번째 인트론 서열을 살펴보면 106
개의 뉴클레오티드 중에서 163개 사이트가 같게 나온다.

동족서열이 다음과 같다고 하자.
AACAGTTACC
TAAGGTCA
정렬하는 방식은 다양하다. 그 중 두 가지만 살펴보자.
-AACAGTTACC
TAA-GGT--CA

AACAGTTACC
TA-AGGT-CA

서열에 대시(-)를 끼워 넣어 틈(682/을 삽입한다고 한다. 서열에 틈이 있다는 것은 그 서열에서
제거가 일어났거나 상대 서열에서 삽입이 일어났음을 뜻한다.

위의 예제에서 어떤 서열이 더 좋은가? 둘 다 5개의 염기쌍이 일치한다. 첫째 정렬 방
식으로 4개의 SS 삽입하여 일치하지 않는 염기쌍이 2개 생겼다. 둘째 정렬 방식으로는
ae 274 삽입하여 일치하지 않는 염기쌍이 3개 생겼다. 불일치로 생기는 손해와 SOB
생기는 손해를 먼저 재보지 않고 어떤 정렬이 더 좋은지 측정하는 건 일반적으로 불가능
하다. 예를 들어, SOS 생기는 손해가 1이고 불일치로 생기는 손해가 3이라고 하자. 정
렬에서 생기는 손해의 BS 정렬에 드는 비용(6084이라고 하자. 그러면 예제 3.18의 첫째
정렬의 비용은 10이고 둘째 QA 비용은 11이다. 따라서 첫째 정렬이 더 좋다. 그러나
틈으로 생기는 손해가 2이고 BAAS 생기는 손해가 1이라고 한다면, 둘째 정렬이 더



===== PAGE 146 =====
© 예제 3.14

0000000
3.7 DNA 서열 정렬   133

좋아진다.

틈과 불일치로 생기는 손해가 정해지면, 최적 정렬을 알아낼 수 있다. 그러나 아쉽게도
가능한 모든 조합을 다 검사하여 최적 정렬을 찾는 ar 방식은 계산양이 많아서 계산
하기 어려운 문제로 분류된다. 이제 서열 정렬 문제를 푸는 효율적인 동적계획법 알고리
즘을 공부해보자.

구체적으로 손해는 다음과 같이 미리 정하고 시작하자.

° 불월지로 생기는 Sale 1
e 틈으로 생기는 손해는 2

서열은 다음과 같이 배열로 표현한다.

A  A  Cc  A  G  T  4  A  0  Cc

aE    A    A    G    G    ab    @    A
ylo} 411] yl2] 913] yl4] 9415] 016] yf7]

opt(i, j)S 부분 AS cli..9) 2 yj. 719 최적 정렬 비용이라고 하자. 그러면
opt (0, te, .9]와 y[0..7] 29] 최적 정렬 비용이 되어 우리가 최종 구하려는 비용이
다. 최적 정렬을 구하는 계산은 다음 중 하나로 시작해야 한다.

i,  ap ]은 910]과 정렬한다. 만약 clo] = 910]이면 A 정렬 사이트에서는 손해가 없

210] = 010]이면 손해가 1이다.

2. - ]은 틈과 정렬하고, A 정렬 사이트에서 손해가 2이다.
3, yO] 2 틈과 정렬하고, Al 정렬 사이트에서 손해가 2이다.

7[0..9]와 /[0..7]의 최적 정렬 4, ,에 [0]과 /[0]이 정렬되어 있다고 가정하자. 그
러면 이 정렬의 내부에는 2[1..9]와 y[1..7]2] 정렬 가 포함되어 있다. 만약 B7} 이

m

af

두 부분 서열의 최적 정렬이 아니라고 하자. 그러면 비용이 더 싼 다른 정렬 C7} 있을

것이다. 그렇다면 정렬 Col 2[0]과 yo] 맞추어 연결하면 4, ,보다 비용이 싸게
210..9]와 0/[0..71을 BAW 수 있다는 의미이다. 따라서 2가 2[1..9]와 /[1-.71의 최
적 정렬임에 틀림없다. 같은 이치로, 210 ..9]와 /[0..71의 최적 PAW 2[0]과 So}
정렬되어 있다면, 그 정렬의 내부에는 [1..91와 yl0..7] 9] 최적 정렬이 포함되어 있고,
7[0..9]와 /[0..71의 최적 정렬에서 ylo] 2} So] 정렬되어 있다면, 그 정렬의 내부에는
710..9]와 0[1..71의 최적 정렬이 포함되어 있다.

210..9]와 /10..71의 최적 정렬이 다음과 같다고 가정하자.

209] 기] 1201] 기] 241 25) 06] 지7] 기] 219]
A A CA @ T YF 4 6 9



===== PAGE 147 =====
@0@0 0 0 0
134   chapter

> GSS 3.12

@ @
3 동적계획

그러면 2[1..9]와 411..7]의 최적 정렬은 다음과 같다.

만약 x [0] = y[0] ol Hey penalty = 0이고, 그렇지 않으면 손해가 1이라고 하면, 다
음과 같은 재귀 관계식을 세울 수 있다.
02【(0, 0) = min(opt(1, 1)+ penalty, opt(1,0)+2, opt(0, 1)+2)
비록 각 서열의 0번째 지점에서 시작하여 재귀 관계식을 세웠지만 임의의 지점에서 시작
에도 문제없다. 따라서 일반식은 다음과 같다.
opt (i, 7) = min(opt(i+1, j+1)+penalty, opt(it+1, 7)0+2, opt(i, 7+1)+2)

재귀 알고리즘을 만들기 위해서 종료조건을 구해야 한다. 서열 x2] 길이를 mole} 하
고, 서열 y 길이를 7이라 하자. 서열 의 끝 AMG = m)S 지났고 서열 의 7 지점
G<n)l 있다면, SS ㅁ- 개 삽입해야 한다. 따라서 종료 조건은 다음과 같다.

opt(m, j) = 2(02- 7)

비슷한 이치로 서열 의 S AAG = n)S 지났고 서열 2 의 :지점(? < my 있다면, 틈

을 ㅠ-1개 삽입해야 한다. 따라서 또 하나의 종료 AAS 다음과 같다.

문제 : 두 개의 동족 DNA ASS] 최적 정렬을 구하시오.
입력 : 길이가 mel DNA 서열 x} 길이가 7 인 DNA 서열 y, ASS 배열로 표현한다.
출력 : 두 서열의 최적 정렬의 비용

void opt ( int i, int /)

{
if (¢ == mm)

opt =2 (n 72);
else if (7 == n)
opt =2 (m —i);


===== PAGE 148 =====
}

@‥@000000
37 DNA 서열 정렬   135

else {
if (저기 == x{/])
penalty = 0;
else
penalty = 1;

}

opt = min(opt (i + 1, 7 + 1) + penalty, opt (i+ 1, J) + 2, opt (4, 7 + 1) + 2);
)/    (opt (    J               J

알고리즘 SSO 다음과 같이 한다.
optimal_cost = opt(0, 0);

이 알고리즘은 최적 정렬 비용만 계산하고 최적 정렬을 만들어 주지는 않는다. 최적 정렬
을 만들어내도록 알고리즘을 수정할 수 있다. 그러나 그 알고리즘은 아주 비효율적이어
서 현장에서 쓸 수 없으므로 시도조차 할 가치가 없다. 그 알고리즘의 복잡도가 지수시간
임을 알아보는 건 연습문제로 남겨둔다.

문제는 부분 서열의 최적 정렬을 여러 번 중복해서 계산하는데 있다. 예를 들어, opt
(0, 0)을 계산하려면, opt (1, 1), opt(1, 0), 02[(0, 1)을 계산해야 한다. A 재귀 호출
에서 opt(1, 0)-& 계산하려면, 02《(2, 1), opt(2, 0), opt(1, 1)을 모두 계산해야 한다.
opt (1, 1)을 두 번이나 따로 계산하는 건 낭비이다.

동적계획으로 이 문제를 풀려면 그림 3.19와 같이 m+1, n+1 크기의 2차원 aS
만들어야 한다. 서열에서 틈을 표현하는 문자를 하나 더 추가하였음을 배열에서 확인해
보자. 틈의 행과 열에서 출발하여 위쪽으로 HAS 채워나가며 반복 ALAC, opt (i, 7)

은 이 배열의 i, 7칸에 계산하여 저장한다. 이 값은 다음 등식을 사용하여 계산한다.

opt (i, j)=min(opt(i+1, j+1)+penalty, opt(it1, 7) +2,opt(i, 7 + 1) + 2) 00
opt(10, j) = 2(8—j)                        (2)
opt (i, 8) =2(10—i)                       (3)

배열의 맨 아래 행의 opti, 7) 값을 계산하려면 (9)식을 쓰고, 배열의 맨 오른쪽 열의
opt(i, 7) 값을 계산하려면 (3)식을 쓰고, 나머지 경우에는 (1)식을 쓴다. (AY 쓰는 경
우 구하려는 칸의 바로 아래 칸의 값과 바로 오른쪽 칸의 값, 대각선으로 바로 아래 칸의
he 가지고 계산한다. 예를 들면, opt (6, 5)는 opt (6, 6)과 opt(7, 5), opt(7, 6)을 가
지고 계산한다.

따라서 대각선 1번 값을 계산하고, 다음에 대각선 2번 값을 계산하고, 다음에 대각선
3H 값을 계산하고, 이런 순서로 그림 3.19의 모든 값을 계산하여 배열을 채운다. 대각선
3까지의 계산과정을 살펴보자.


===== PAGE 149 =====
136      chapter 3 동적계획
i)     0      1      2            4      5      6      7      8
1          1      ^     ^     G     G     T     Cc     A     -
0    ^
1    ^
2 6
을    ^
4    G
5    Li
=
am                                              t                                      대각선 3
> ^                                                              ~
    대각선 2
8 0                                                        「   ~
~         대각선 1
10 =                                         『_

e 대각선 1

026(10, 8) =2(10—10) = 0
e 대각선 2

opt(9, 8)= 2(10- 9) = 2

00(10, 7)=2(8—7) =2
e 대각선 3 :

ont(S, 8)9= 2(10-8)= 4

opt (9, 7)

= min(opt(9+1, 7+1)+ penalty, opt(9+1,7)+2, opt(9,7+1)+2)
=min(0+1, 3+2, 2+2)=1

opt (10, 6) =2(8—6) =

그림 3,202 AALS 완료하여 HAS 채운 결과를 보여준다. 최적 정렬을 위한 비용인
opt(0, 0)은 ?이다.

다음 최적 정렬을 완성된 배열에서 어떻게 추출하는지 알아보자. Al opt (0, 0)의 값
을 구하게 된 ASS 찾아야 한다. 왼쪽 맨 위 구석에서 시작하여 역추적한다. opt (0, 0)
의 값을 될 수 있었던 3칸을 조사하여 선택한 BES 선택한다. 그리고 그 선택한 BES 가지
고 같은 TAS 되풀이한다. 동점이 생기는 경우 임의로 선택한다. 맨 아래 구석에 도달


===== PAGE 150 =====
37 DNA 서열 정렬     137

j | 0     1     2               5     6     7     8
i        개     1 2|61|6|7ㅜ106 ㅅ     =
0 Al 7     8 | 10 | 12 | 13 | 15 | 16 | 18 | 20
1 Al 6     6     8 | 10 | 11 | 13 | 14 | 16 | 18
2 0] 6     5     6     8     9 | 11 | 12 | 14 | 16
3 Al 7     5     4     6     7     9 | 11 | 12 | 14
4 6] 9     7     5     4     5     7     9 | 10 | 12
5 ㅠㅜ] 8     8     6     4     4     5     7     8 | 10
6 ㅠㅜ] 9     8     7     5     3     3     5     6     8
7 Al 1     9     7     6     4     2     3     4     6
8 c| 13] 11 | 9     7     5     3     1     3     4
9 c| 14] 12 | 10 | 8     6     4     2     1     2
10 - | 16 | 14 | 12 | 10 | 8     6    4     2     0

그림 3.20 최적 정렬을 찾는데 사용할 배열의 완성된 모

tl)

jaa

할 때까지 이 과정을 되풀이한다. 찾은 경로는 그림 3,200] 진하게 표시되어 있다. 어떻
게 경로를 찾게 되는지 처음 몇 개의 값만 따라가 보자. 2째 행과 /째 열에 해당하는 배열
의 칸을 [2][7]로 표시하자. 그리고 다음과 같이 진행한다.

2.

1, [0][0]을 선택한다.

경로에 넣을 둘째 항목을 2  ho

(a) [O][1}-S 검사한다. [O][O]o] 도달하기 위해서 여기서 왼쪽으로 이동하므로, Ho]
삽입되었고 비용 와 sre 을 텐데, 그렇다면 다음과 같이 되므로 아니다.

opt(0, 1)+2=8+2=10=7
(b) (LOLS 검사한다. [01[이에 aah 위해서 여기서 위쪽으로 의동하므로, 틈이
삽입되었고 비용 fe 추가되었을 텐데, 그렇다면 다음과 같이 되므로 아니다.
opt(1, 0)+2=64+2=847
(c) (UMS 검사한다. [01[이에 도달하기 위해서 여기서 대각선 위쪽으로 이동하므

로, 틈이 삽입되었고 비용 penalty Ho] 추가되었을 텐데, [0] = 이고 010]
= 2이므로, penalty = 1이다. 그렇다면 다음과 같이 된다.

opt(1, 1)+1=6+1=7

따라서 경로에서 둘째 배열 칸은 [11[11이다.


===== PAGE 151 =====
@‥00@00000 0
138    chapter 3 동적계획

배열 값을 계산하면서 경로를 동시에 찾을 수도 있다. 즉, 배열 값을 저장할 때마다
해당 배열 칸을 기록해두면 된다.

일단 경로를 찾으면 정렬된 서열은 다음과 같이 추출할 수 있다(정렬된 서열은 역순으

u

1, 배열의 오른쪽 맨 아래 구성에서 시작하여 표시해둔 경로를 따라간다.

2, HSS] [é][j] 칸에 도달하기 위해서 대각선으로 이동할 때마다, ?째 Bol] 해당하는
EAS # 서열에 넣고, 7째 열에 해당하는 문자를 y 서열에 넣는다.

8. 배열의 [i] [7] 칸에 도달하기 위해서 위로 이동할 때마다, ?째 Bol] 해당하는 문자를
28 서열에 넣고, 틈 문자를 4 AS] 넣는다.

4. HSS] [i] lj] 칸에 도달하기 위해서 왼쪽으로 이동할 utr}, 7째 행에 해당하는

문자를 y 서열에 넣고, 틈 문자를 2 서열에 넣는다.
그림 3,202] 배열에 이 과정을 그대로 따라가면 다음과 같은 최적 정렬 ASS 얻는다.

AACAGTTACC
TA AG Gil © A

손해 값을 다르게 잡으면 최적 정렬 서열이 다르게 나올 것이다. 110997) 논문을 보면
손해 값을 어떻게 정할지 나와 있다.

서열 정렬 BAS 푸는 동적계획 알고리즘의 작성은 연습문제로 남긴다. Waterman
(1984)의 =o] 자세히 기술되어 있는 서열 정렬 알고리즘은 가장 널리 쓰고 있는 서열
정렬 방법 중 하나이다. 이 알고리즘은 BLAST (Bedell, 2003)과 DASH(Gardner—Stephen
and Knowles, 2004)와 같은 정교한 서열 정렬 시스템에 사용되었다. 이 A Neapolitan
(2009)의 교재를 기반으로 작성되었으며, 분자 진화유전학을 자세히 알아보려면 그 교재
를 참고하기 바란다.

3.1절
1. 등식 ODS 유도하시오.
2. 등식 BNE 기초로 하여 이항계수문제(알고리즘 3.1를 푸는 분할정복 알고리즘은 | 1 |를

구하는데 이 |-1개의 BS 계산함을 nol 관한 귀납법으로 증명하시오.

1

fe)

3. 이항계수문제를 푸는 = 알고리즘(알고리즘 3.1과 3.22 모두 구현하는 프로그램을 작성하
고, 다양한 문제 사례를 가지고 성능을 비교하시오.

4. 알고리즘 3.2(동적계획법으로 이항계수 구하기)를 인덱스가 OE] 《까지인 배열 하나만 사



===== PAGE 152 =====
@©eeeee e
연습문제  139

용하도록 수정하시오.

3.2절

5

7
8

9

10

. 최단경로 문제를 푸는 플로이드 알고리즘 (알고리즘 3.4)S 사용하여 다음 그래프에 대해
서 행렬 22(최단경로의 길이를 포함함)와 행렬 /^(최단경로의 중간정점 가운데 가장 높은 인
덱스를 포함함)를 구축하시오. 그리고 수행되는 절차를 단계별로 보이시오.

. 최단경로출력 알고리즘(알고리즘 8.9/을 사용하여 연습문제 5의 그래프에서 정점 에서 ov,
로 가는 최단경로를 구하시오. 여기서 그 연습문제에서 구한 행렬 PS 사용하시오. 그리고
수행되는 절차를 단계별로 보이시오.

. 최단경로출력 알고리즘(알고리즘 35S 분석하고, 1차 시간복잡도를 가짐을 보이시오.

. 최단경로 문제를 푸는 플로이드 알고리즘 3(알고리즘 3.4)를 구현하는 프로그램을 작성하
고, 여러 가지 다른 그래프를 가지고 성능을 비교해 보시오.

. 최단경로 문제를 푸는 플로이드 알고리즘 9(알고리즘 8.4)를 어떤 주어진 정점에서 다른 명
시된 정점으로 가는 최단경로만 주는 알고리즘으로 수정가능한가? 그리고 왜 그런 답이 나
오는지를 밝히시오.

LL

. 최단경로 문제를 푸는 플로이드 알고리즘 ates 8.4)가 음의 가중치를 가진 그래프에
서 최단경로를 구하는 알고리즘으로 사용될 수 있을까? 그리고 왜 그런 답이 나오는지를
밝히시오.

3.3절

11.

최적의 원칙이 성립하지 않고, 따라서 동적계획법으로 최적의 해를 구할 수 없는 최적화 문
제를 찾아보시오. 그리고 왜 그런 답이 나오는지를 밝히시오.

3.4절

12
13

, 다섯 개 VBS 곱하는 순서의 조합을 모두 나열하시오.
. 다음 행렬들의 곱인 A, x 4, × A,X A,X 4.를 계산하는 최적 순서와 그 비용을 구하시오.

A, 2) 37) (104)


===== PAGE 153 =====
140

chapter 3 동적계획
4,의 크기는 (4×5)
4;의 크기는 (5x 20)
4,의 크기는 (20×20)
4。의 크기는 (2x50)
알고리즘 3.6이 만드는 Ma} PS 구하시오.

14. 최소곱셈 알고리즘(알고리즘 3.0)과 최적순서출력 알고리즘(알고리즘 3.7)을 구현하는 프로
그램을 작성하고, 여러 가지 다른 문제 사례를 가지고 그들의 성능을 비교하시오.

15. BO} A] (3.5)를 기초로 작성한 분할정복 알고리즘은 지수 시간복잡도를 가짐을 증명하시
오,

16. 개의 VAS 곱하는 다른 순서의 경우의 수가 몇인지 계산하는 문제가 있다고 하자.
(a) 정수 #을 입력받아 이 HAS 푸는 재귀 알고리즘을 작성하시오.

내보시오.
17. 다음 등식이 성립하도록 유도하시오.
+}   [(n— diagonal) x diagonal] = n{n—1)(n+1)
diagonal = 1                                  6
이 SAS 알고리즘 3.69] BE 경우 시간복잡도 분석에 사용된다.

18. 개 행렬로 된 표현식 AAS SSE 둘러싸기 위해서는 괄호가 7ㅡ1쌍이 필요함을 증명하
시오.

19. 알고리즘 8.7을 분석하고, 이 알고리즘이 1차 시간복잡도를 가짐을 증명하시오.

20. 임의 양의 정수 do] 대해서 각 행렬의 크기가 1×1 또는 1×0 또는 40×1 또는 0×0인
개 Ba A, x A,X ...X A, 곱하는 최적 SAS 찾는 효율적인 알고리즘을 작성하시오.
작성한 알고리즘을 분석하고, 그 결과를 차수표기법을 사용하여 표시하시오.

3.5절

21. 6개 서로 다른 원소를 가지고 몇 개의 다른 이분검색트리를 만들 수 있는가?

22. 다음 아이템에 대해서 최적 이분검색트리를 구축하시오. CASE(.05), 81.80(.15), END(.05),
IF(.35), OF(.05), THEN(.35), 여기서 괄호 안의 수는 각 단어가 나올 확률을 나타낸다.

23. 최적 이분검색트리 알고리즘(알고리즘 3.9)에 사용된 Ya 계산하는 효율적인 방법을
찾으시오.                                         m=t

24. 최적 이분검색트리 알고리즘(알고리즘 3.9} 최적 이분검색트리 구축 알고리즘(알고리즘
3.10)을 구현하는 프로그램을 작성하고, 여러 가지 다른 문제 사례를 가지고 그들의 성능을
비교하시오.

25. 알고리즘 3102 분석하고, 그 시간복잡도를 차수표기법을 사용하여 표시하시오.


===== PAGE 154 =====
연습문제     141

26. 검색키가 트리에 없을 수도 있는 경우도 포함하도록 최적 이분검색트리 알고리즘(알고리즘
29% 일반화하시오. 즉, 없는 검색키가 Key, % Kesh & 수 있을 확률을 oS 하도록
한다. 여기서 :=0, 1, 2, …, 7이다. 이 일반화한 알고리즘을 분석하고, 그 결과를 차수표기

을 사용하여 표시하시오.

2/. 본문의 식 (3.0/을 기초로 작성한 분할-정복 알고리즘은 지수의 시간복잡도를 가짐을 증명
하시오.

3.6절
28. 다음과 같이 행렬 WE 표현되어 있는 가중치포함 방향그래프에서 최적회로(최적일주여행
길)를 구하시오. 수행되는 절차를 단계별로 보이시오.

0 8 131820
3 0 7 8 10
W=]| 4110107
667011
10621 0
29. 외판원 문제(알고리즘 3.11)를 푸는 동적계획 알고리즘을 본문보다 더 세부적으로 작성하시
uo
30. 연습문제 2794] 세부적으로 작성한 알고리즘 3.11을 구현하는 프로그램을 작성하고, 그 성
능을 여러 가지 사례를 가지고 평가하시오.
3.7절

3.7절에 있는 알고리즘 02*의 시간복잡도를 분석하시오.
32. 서열 정렬 문제의 동적계획 알고리즘을 작성하시오.

33. 불일치를 손해 1점, SS 손해 3점으로 하고, 다음 서열의 최적 정렬을 찾는 동적계획 알고
리즘을 작성하시오.

CCGGGTTACCA
GGAGTTCA

추가적인 AS SH

34. 7번째 피보나찌 항 구하기 알고리즘(1장의 연습문제 34 참조)같이 알고리즘 3.2(동적계획법
을 사용하여 이항계수 구하기)의 입력크기는 숫자 ni} *를 코드화하는데 필요한 심벌의 개
수이다. 이 입력크기를 기준으로 알고리즘을 분석하시오.

35. 개 행렬 4, A, … 4, 을 곱하는 가능한 순서의 ASHE 구하시오.
36. 개 원소로 구성된 이분검색트리의 개수는 다음과 같은 식으로 주어짐을 증명하시오.
1    2n
(n+1) | n ㅣ
97. 최적 이분검색트리 문제(알고리즘 3.9)를 푸는 8차시간 알고리즘을 개발할 수 있는가?
38. 동적계획법을 사용하여 주어진 n 7H 실수 값의 리스트0160에서 인접하는 부분리스트(600-



===== PAGE 155 =====
@…0@00000 0
142    chapter 3 동적계획

868에 속한 Zo] Go] 최대가 되는 부분리스트를 찾는 알고리즘을 작성하시오. 작성한 알
고리즘을 분석하고, 그 결과를 차수표기법을 사용하여 표시하시오.

39. 문자의 수열66046000) 과 SS 생각해보자. 예로써, S,=ASCMA*MNO|31, , =
AXMC4ANBS 들 수 있다. 수열의 부분수열(640860462006)은 어떤 지점에서라도 문자를
임의로 A AAA 수 있다고 가정하면, BAHU A843 의 최장 BE
++ (longest common 84686046006)을 찾는 알고리즘을 작성하시오. 이 알고리즘은 각 수

열의 최대길이 ae SE (maximum-—length common subsequence) a



===== PAGE 156 =====
Chapter 4

탐욕 알고리즘

킨스(18068 Dickens) 2] 고전 소설에 나오는 스크루지(86@0080)는 탐욕적
인 인물을 ASS 때 언제나 등장한다. 스크루지는 지나온 과거나 다가올 미래
는 별로 중요하게 생각하지 않는다.  언제나 탐욕스럽게 가능한 한 많은 금을 모으는 일에
만 몰두하였다. 과거천사가 과거를 상기시켜 주고, 미래천사가 미래를 경고하자, 비로소
탐욕스런 행태를 바꾸었다.

탐욕 알고리즘(860000> algorithm) 스크루지의 금모으기와 같은 방식으로 작동한다.
=, aa    alk 고르는데, 미리 정한 기준에 따라서 매번 '가장 좋아 보이는' 답을 선택
한다. '스크루지나 '탐욕'이라는 부정적인 느낌의 단어 때문에 탐욕 알고리즘이 좋지 않
을 것이라는 선입견은 버려야 한다. 매우 효율적이고 간단한 탐욕 알고리즘이 많이 있다.

탐욕 알고리즘은 동적계획과 마찬가지로 최적화 BAS 푸는데 주로 사용한다. 상대적
으로 탐욕 알고리즘이 설계하기 훨씬 더 쉽다. 동적계획은 재귀관계식을 세워서 입력사
례를 더 작은 입력사례로 분할한다. 반면, 탐욕 알고리즘은 입력사례를 분할하지 않는다.
탐욕 알고리즘은 순서대로 답을 하나씩 모아서 최종 GS 구축하는데, 가장 좋아 보이는

을 선택하여 모은다. 즉, 어떤 선택이든지 선택할 당시100919)는 최적이다. 전체적으

세

ro, |»


===== PAGE 157 =====
144

chapter 4 탐욕 알고리즘

고

로(06843) 최적인 BS 구하고 싶지만, 항상 최적인 HS 얻는다는 보장은 없다. 따라
서 탐욕 알고리즘은 최적인 해답을 얻는지 확인하는 절차를 반드시 거쳐야 한다.

거스름돈 문제를 푸는 탐욕 알고리즘을 공부해보자. 편의점의 계산대에서 일하는 은수
는 현금을 내는 손님에게 잔돈을 정확히 거슬러 주어야 한다. 서비스 차원에서 동전의
개수가 최소가 되도록 거스름돈을 주는 게 좋다. 예를 들어, 거스름돈이 870원인 경우
10원짜리 동전을 87개 주면 받는 손님은 분명히 짜증을 낼 것이므로 지양해야 한다. 따라
서 거스름돈을 정확히 세어 주는 작업 외에도 SAS] 개수가 최소가 되도록 AAS 동전
을 선택해야 한다. 은수의 거스름돈 문제에 대한 해답은 거슬러 줄 총액에 해당하는 동전
의 집합이고, AAS] 해답은 SA] 개수가 최소가 되는 집합이다. 이 문제를 푸는 탐욕
알고리즘은 다음과 같이 작동한다. 처음에는 빈손으로 시작한다. 그리고 액면가가 가장
높은 동전을 집어 손에 올려놓는다. 즉, 어느 동전이 가장 좋은지(지역적으로 최적)를 결
정하는 기준은 SAS] 액면가이다. 이를 탐욕 알고리즘에서 AAD (selection proce—
0078)이라고 한다. 손에 있는 거스름돈의 SAO] 거슬러주어야 할 액수를 초과하는지 본
다. 이를 탐욕 알고리즘에서 AAVAAH feasibility 00009라고 한다. 만약 거스름돈의
총액이 거슬러주어야 할 액수를 초과하지 않으면, 방금 올려놓은 SAS 거스름돈에 =
함된다. 만약 거스름돈의 총액이 거슬러주어야 할 액수와 같은지 검사한다. 이를 탐욕
알고리즘에서 HPA A(solution 006009이라고 한다. 만약 같지 않다면 다시 선택과정으
로 돌아가서 다른 동전을 찾고 같은 과정을 되풀이한다. 거스름돈의 총액이 거슬러주어
Of 할 액수와 같든지, 아니면 동전이 떨어질 때까지 이 과정을 되풀이한다. 후자의 경우
거스름돈을 다 거슬러줄 수 없게 된다. 이 절차를 알고리즘으로 정리하면 다음과 같다.

while (동전이 남아있고 문제 미해결) {

가장 가치가
더하여 거스름돈의 총액이 거슬러주어야 할 액수를 초과) // 적절성검사
도로 집어넣는다;

높은 동전을 집는다;                             // 선택과정

거스름돈에 BAS 포함시킨다;
스름돈의 총액이 거슬러주어야 할 액수와 같다)             // 해답점검

문제 해결;

적절성검사에서 SAS 집었다가 거스름돈의 SHO] 거슬러주어야 할 액수를 초과하
면, 해답이 될 수 없다. 따라서 집은 동전은 다시 내려놓아야 한다. 이 알고리즘이 어떻게
작동하는지 그림 4.1을 보자. 다시 말해서, 이 알고리즘을 "탐욕"이라고 하는 이유는 선택
의 잠재적인 결점을 선택과정에서 전혀 고려하지 않고, 가장 비싼 동전을 무작정 선택하
기 때문이다. 그 선택을 다시 물릴 기회는 없다. 일단 어떤 동전을 선택하기로 하면 그
동전은 영원히 거스름돈에 포함되고, 일단 어떤 동전을 포기하기로 하면 그 동전은 영원


===== PAGE 158 =====
거슬러주어야 하는 액수 : 36센트 ($0.36)

단계                                                                거스름돈의 총액

2. 첫째 CYS 집는다.

3. 둘째 다임을 집었다가 내려놓는다.

4. 니켈을 집었다가 내려놓는다.

5. 페니를 집는다.

그림 4.1 거스름돈을

히 거스름돈에서 제외된다. 이 과정은 아주 간단하지만, 과연 이렇게 얻은 답이 최적일
까? 즉, 거스름돈 문제에서 해답이 있을 때 탐욕 알고리즘으로 구한 거스름돈의 동전 개
수가 최소일까? 미국에서 통용되는 동전인 페니(66007, $0.01), 니켈04066, $0.08), 다
(dime, $0,10), AE] (quarter, $0.25), 반달러(068 dollar, $0.50)를 사용하고, 최소한 종
류별로 하나씩은 있다고 하면 거스름돈을 만드는 경우 탐욕 알고리즘으로 항상 동전 개
수가 최소인 거스름돈을 만들 수 있다. 이에 대한 SVS 연습문제로 남긴다. 우리나라
동전으로 해봐도 탐욕 알고리즘이 항상 최적인 거스름돈을 만들어 준다. 이것도 연습문
제로 살펴본다. 그러나 만약 미국 동전에 1241 E (cent, 1 cent = $0.01)짜리 SAS 추가
한다면 탐욕 알고리즘으로 최적해를 항상 준다는 보장이 사라진다. 그림 4.8에서 왜 그런


===== PAGE 159 =====
@0@00000 0
146    chapter 4 탐욕 알고리즘

동전의 종류

거슬러주어야 하는 액수 : 16센트 ($0.16)

단계                                                       거스름돈의 총액

2. 다임을 집었다가 내려놓는다.

3. 니켈을 집었다가 내려놓는다.

4. 페니를 4개 집는다.

그림 4.2_12센트짜리 동

지 설명하고 있다. 그림 4.8에서 탐욕 알고리즘의 해답은 거스름돈 동전의 개수가 5개인
반면, 최적의 해답은 다임과 니켈과 페니로 구성한 3개이다.

거스름돈 문제에서 보듯이 탐욕 알고리즘은 최적의 해를 보장하지 않는다. 따라서 탐
욕 알고리즘을 설계했다면 최적의 HS 주는지를 항상 점검해야 한다. 4.1, 4.2, 4.8, 4.4
절에서 탐욕 알고리즘이 항상 최적의 해를 주는 문제를 공부한다. 4.5절에서 그렇지 않은
문제를 살펴볼 텐데 탐욕 알고리즘과 동적계획 알고리즘을 비교하고, 각 알고리즘이 어
떤 경우에 더 좋은지를 탐구한다. 탐욕 알고리즘을 정리하면서 이 BS 마치자. 탐욕 알
고리즘은 공집합에서 시작하여 그 집합이 문제의 해답이 될 때까지 원소를 그 집합에 차
례로 추가한다. 이 과정은 다음의 세 절차를 차례로 반복한다.

6 선택과정은 집합에 추가할 다음 원소를 고른다. 그 당시 AAS 선택하는 탐욕 기준

에 따라 선택한다.
* 적절성검사는 새로운 집합이 해답이 되기 적절한지 검사한다.
* 해답점검은 새로운 집합이 문제의 해답인지 결정한다.



===== PAGE 160 =====
@ 41 최소비용 신장트리

도시계획사가 모든 도시사이를 연결하는 자동차 도로 건설사업을 계획하고 있다고 하자.
건설자금을 아끼기 위해서 건설하는 도로의 총길이를 최소로 하여 도로를 건설하고 싶을
것이다. 이러한 유형의 문제를 해결하는 알고
를 간단히 복습하고 시작하자. 그림 4.8(8)에 연결된 가중치포함(061940660), 비방향
(undirected) Le} G7} 있다. 여기서 가중치(\61844)는 음이 아닌 수로 가정한다. 그래
프의 이음선(6088/에 방향이 없으면 비방향04001760660)이라고 한다. 그림으로는 이음선
에 화살표가 없으면 비방향이다. 이음선에 방향이 없기 때문에 “이음선이 두 마디 사이에
있다'라고 말한다. 비방향그래프에서 경로(6800는 이음선으로 연결된 마디의 나열
(86046006/이다. 이음선에 방향이 없기 때문에 마디 에서 로 가는 경로가 있다는 사실

(a) 연결된, 가중치가 있는,           (b) (V4,v5) 를 이 부분그래프에서 제거하더라도,
비방향그래프 @.                   그래프는 연결된 채로 남아있다.

그림 4.3 가중지그래프와 8개의 부분그래프


===== PAGE 161 =====
148

chapter 4 탐욕 알고리즘

은 마디 에서 로 가는 경로가 있다는 사실과 같다. 따라서 비방향그래프에서는 "두
마디 사이에 경로가 있다"라고만 단순히 말한다. 비방향그래프에서 모든 마디의 쌍에 대
해서 경로가 있으면 “연결되어60ㅁㅁ60[60) 있다"라고 부른다. 그림 4.8에 있는 그래프는
모두 연결되어 있다. 그림 4.30)에서 vy St vy 사이의 이음선을 제거하면, 이 그래프는
더 이상 연결되어 있다고 할 수 없다.

비방향그래프에서 마디에서 자신으로 다시 돌아가는 경로에 최소한 서로 다른 3개의
마디가 있으면 단순순환경로(6300!6 cycle)e} 하고, 단순순환경로가 없는 비방향그래프
를 비순환적(307010)이라 한다. 그림 4.3(0)와 (0)는 비순환적인 반면, (8)와 00)는 비순환
적이 아니다. Bel(tree)\=E 비순환적이며 연결되어 있는 비방향그래프이다(트리를 기술
용어로 자유트리(66 ㅁ68)라고도 한다). 지금 정의한 트리는 특정 마디를 뿌리로 지정하
A] 않았다. 따라서 뿌리 있는 트리(00160 1\ㅁㅠ68)는 마디 하나를 뿌리로 지정한 트리이다.
그러므로 (3.5절에서 공부한) 트리가 여기서는 뿌리 있는 트리이다.

연결된, 가중치포함, 비방향그래프 Go 마디들은 최소한 모두 연결된 상태로 유지
한 채 이음선의 가중치의 합은 가능한 한 최소가 되도록 이음선을 제거하여 부분그래프
를 만드는 BAS 풀어보자. 이 문제는 응용 분야가 다양하다. 앞에서 언급했듯이 도로건
설에서 도로의 길이가 최소가 되도록 도시를 모두 연결하고 싶은 경우가 있다. 비슷하게
전화통신망에서는 케이블의 길이가 최소가 되어야 할 것이고, 하수도 배관공사에서는 배
관의 길이가 최소가 되어야 할 것이다. 가중치의 합이 최소인 부분그래프는 꼭 트리가
된다. 왜냐하면, 부분그래프가 트리가 아니면 순환경로가 존재하게 되고 순환경로 상의
이음선 하나를 제거하여 가중치의 합이 더 작은 연결된 그래프를 만들 수 있기 때문이다.
그림 4.8을 보고 이를 설명해보자. 그림 4.386)의 부분그래프 b= 최소 가중치를 가질
수 없다. 왜냐하면, 순환경로 [08, vg, v5, 9]상의 어떤 이음선을 제거하더라도 그 부분
그래프는 연결된 채로 남아있다. 예를 들어, 0,와 ;를 연결하는 이음선을 AAS 수 있
으며, 그 결과로 더 작은 가중치를 가진 연결된 그래프를 얻는다.

Go] 대한 신장트리(60800128 \ㅠ689)는 G2] 마디를 모두 포함하면서 트리인 연결된 그
래프이다. 그림 4.3(0)와 ME Go] 대한 신장트리이다. 가중치가 최소가 되는 연결된

수

부분그래프는 신장트리가 틀림없지만 신장트리라고 해서 모두 가중치가 최소라는 보장
은 없다. 예를 들면, 그림 4.3에서 신장트리 (0)는 가중치가 최소가 아닌데, 왜냐하면 신
장트리 Ad 가중치가 더 작기 때문이다. 앞에서 언급한 문제를 푸는 알고리즘은 반드시
가중치가 최소가 되는 신장트리를 구해야 한다. 이러한 트리를 최소비용 신장트리(0101-
mum spanning ㅁㅠ66)라고 한다. 그림 4.8에서 트리 (0)는 Gol] 대한 최소비용 신장트리이
다. 하나의 그래프에 하나 이상의 최소비용 신장트리가 존재할 수 있다. 에는 최소비용
신장트리가 하나 더 있는데 찾아보기 바란다.

존재하는 신장트리를 모두 찾아보는 무작정 방법으로 최소비용 신장트리 찾으
의 경우 지수시간보다 나쁘다. 탐욕적 방법을 사용하면 더 효율적으로 문제를

ce.
19,

, ae
A
nln

2

때


===== PAGE 162 =====
다. 먼저 비방향그래프부터 정식으로 정의해보자.

정의

비 Saute graph) G+= 마디의
성된다. 이 HSS 의 이음선이라고

한조

집합 와 voll 속한 마디의 쌍의 집합 2
다. GE 다음과 같이 표시한다.

So
0

SIC

한

의 멤버는 v= 표시하고, <,와 《/,를 연결하는 이음선은 다음과 같이 표시한다.
(0; v;)

© 예제 41     그림 4.8(8)에 대하여,

V= {v,, Vg) U3. Vgy vs }
EF={ (v,, Uy), (v4, 06) 06, 067, (v9, U4)5 (v5504)
(v3, Us), (vy, vs) }
이음선을 표시하면서 마디를 나열하는 SAE 비방향그래프에서는 중요하지 않다. 예를 들
(vy, vy) SH (vp, 1,)은 같은 이음선을 나타낸다. 우리는 인덱스가 낮은 마디를 앞에 두도록 하자.

Go} 대한 신장트리 TE  es 같은 마디 VS 가지지만, 7의 이음선의 집합은 |
부분집합 a 신장트리는 T=(V, FB 표시한다. 문제는 7=(, 20가 Gol 대
한 최소 비용 신정 im rae £9] 부분집합 FS 찾는 것이다. 이 문제를 푸는 탐욕
알고리즘을 고수준으로 표현하면 다음과 같다.

= 0                                   // 이음선의 집합을 공집합으로

// 초기화
while (사례 미해결) {

부분적으로 최적인 고려사항에 따라 이음선을 선택;       // 선택절차

 (그 이음선을 Fo] 추가하면 순환경로가 생기지 않음)     // 적절성 점검
그 이음선을 /에 추가;

if (T=(V, F)7} 신장트리)                  // 해답점검
사례해결 ;

이 알고리즘은 “부분적으로 최적인 고려사항에 따라 이음선을 선택한다"라고 단순히
말한다. 주어진 문제에 대하여 부분적으로 최적이 되는 성질이 하나만 존재하는 것은 아
니다, 이 BAS 푸는 두 개의 다른 탐욕 알고라즘인 프림 alga 크루스칼 알고리즘

을 공부해보자. 각 알고리즘은 부분적으로 최적인 서로 다른 특징을 사용한다. 탐욕 알고

= ㅋㅋ oe



===== PAGE 163 =====
@eee @
150   chapter

FH=@;
Y= {v,};

@ 0
4 탐욕 알고리즘

즘이 항상 최적의 해를 준다는 보장이 없다는 것을 상기해보자. 이 경우에 대해서 과연
그런지 또는 그렇지 않은지 증명할 필요가 있다. 프림 알고리즘과 크루스칼 알고리즘 모
두 항상 최소비용 신장트리를 만든다는 사실을 증명한다.

를 고흐

4.1.1 프림 알고리즘

프림 알고리즘(500ㅁ8 Algorithm)= 이음선의 2의 부분집합인 공집합과 임의의 마디

를 포함하도록 초기화된 마디의 부분집합에서 시작한다. 는 {v,} 로 초기화한다. Yo
서 가장 가까운(2987680 마디는 최소가중치를 가진 이음선으로 에 속한 마디를 AAs}
는 V- Yo] 속한  Dooce 그랬듯이 가중치그래프에서 가중치와 거리는 서로
더불어 사용할 수 있다). 그림 4.868)에서 = {v,} 일 때, we You 가장 가깝다. Y
에서 가장 가까운 마디는 에 추가하고, 그 이음선은 Fol] 추가한다. 같은 가중치가 두
개 이상 있으면, 임의로 선택한다. 이 예에서 는 에 추가하고, (01, vo) = Fol] 추가
한다. 가장 가까운 마디를 추가하는 이 과정은 "= 가 될 때까지 계속한다. 이 BAS
고수준으로 표현한 알고리즘은 다음과 같다.

// 이음선의 집합을 공집합으로 초기화
// 마디의 집합을 첫째마디만
// 포함하도록 초기화

while (사례 미해결) {

에서 기장

가까운 V-Yo] 속한 이음선을 선택 ;       // 선택절차와 적절성 점검

그 마디를 에 추가;

그 이음선을

a =-= 0                             // 해답점검

사례해결 ;

- 에서 새로운 마디를 취해도 순환경로가 생기지 않는다고 보장할 수 있기 때문
에 선택절차와 적절성 점검은 같이 이루어진다. 그림 4.4는 프림 알고리즘이 어떻게 실행

LAS 보여준다. 그림 4.4에서의 실행 단계마다 음영 처리된 마디는 \를 나타내고,
PAA| 표시된 이음선은 FS 나타낸다.

앞에서 공부한 고수준 알고리즘은 그림으로 표시된 작은 그래프를 가지고 수동으로
최소비용 신장트리를 만드는데 문제없이 사용할 수 있다. 그래프를 검사하여 에 가장
가까이 있는 마더를 찾기만 하면 되기 때문이다. 그러나 컴퓨터언어로 구현할 수 있는
알고리즘을 작성할 목적이라면, 단계별 AAS 더 세부적으로 묘사해야 할 필요가 있다.
그러기 위해서 가중치그래프를 인접행렬로 표현한다. 즉, 수의 nxn 행렬 WH 표현하
는데, 여기서 Will] 다음과 같이 정의한다.

pi



===== PAGE 164 =====
1. 마디 을 먼저 선택한다.

2. {4 1)에서 가장 가까이                 3. {V4, 땅에서 가장 가까이
있으므로 마디 를 선택한다.           있으므로 마디 를 선택한다

4. {V4, Vo, }에서 가장 가까이           5. 너를 선택한다.
있으므로 마디 \를 선택한다.

있는) 가중치그래프와 그 그래프에서 프림 알고리즘의 실행절차. 에 속한

|
|음선은 진하게 표시되어 있다.


===== PAGE 165 =====
152     chapter 4 탐욕 알고리즘
고         4    5
110    1         00    00

4100 6 4 0 5

5 | 0 00 2  5 0

이음선 가중치 《,와 vp 연결하는 이음선이 존재하는 경우
Willy] =} ©            v9} uF 연결하는 이음선이 존재하지 않는
0            1 = )인 경우

으
경우

그림 4.3(8) 그래프는 그림 4.5에 표현되어 있다. i= 2, .……, 7에 대하여 다음과 같이

정의되는 두 개의 배열 2702769와 distanceS 유지한다.

nearest[i] = 에 가장 가까운 에 속한 마디의 인덱스

distance |i] = v;2} nearest|i]7} 인덱스인 두 마디를 연결하는

이음선의 가중치

시작할 때 Y= {v,} 28, nearest(i]

1로 27|SS}11 distance [i] = 과 ,를

연결하는 이음선의 가중치로 초기화한다. 마디들을 에 추가하면, 이 두 배열은 바깥
에 있는 각 마디에서 가장 가까운 》 안에 있는 새로운 마디를 참조하도록 갱신된다. OF
느 마디를 yo] 추가시킬지 결정하기 위해 매번 반복할 때마다 44680760610] 값이 최소가
되는 인덱스를 계산한다. 이 인덱스를 02607라고 부른다. vnear7} 인덱스인 마디는

distance [unear] 3 12 놓음으로서 Yo) 추가된다. 다음 알고리즘은 이 절차를 구현

완다.

Re 41 프림 알고리

ol

문제 : 최소비용 신장트리를 구하시오.

입력 : 정수 n > 2와 마디의 개수가 nel 연결된 가중치포함 비방향그래프. 그래프는 행과
열 모두 인덱스의 범위가 1부터 7까지인 2차원 배열 We 표현한다. 여기서 Wie

im 마디와 )째 마디를 연결하는 이음선의 가중치이다.
출력 : 그래프에 대한 최소비용 신장트리 안에 있는 이음선의 집합 F

void prim (int n,
const number W{][],


===== PAGE 166 =====
@0‥000600000
41 취소비용 신장트리    153
set_of_edges& 2)
{
index i, vnear;
number min ;
edge e;
index nearest [2 .. x];
number distance [2 .. a] ;
F= ©
for (i= 2; 7 <= n; H+){
00000 1 = 14                    // 모든 마디에 대하여 Voy 속한 가장 가까운 마디
distance| i] = W1][ 7];            // (nearest i|)= 이로 초기화하고,
}                              // 로부터 Ael(distance i])E 0,2} v,&

// 연결하는 이음선의 가중치로 초기화한다.
repeat (2 — 1 times){
// 7-1개의 마디를 Yo 추가한다.
min = ©
for (f= 2; 7 <= a; #4)        // 각 마디에 대하여 distancel 기를 검사하여 》에
if (0 < distance[i] < min) {  // 가장 가까이 있는 마디(00084)를 찾는다.
min = distance| 1] ;
vnear = 1}
;
e = evnear7} 인덱스인 마디를 Yo) 추가한다.

add e to 2"
distance|vnear| = —1;           // Yo 속하지 않은
for (J = 2; i <= 2; H+)        // 각 마디에 대하여

if (Wii 기 eteas < distance 기) { // Yexeol A e|(distance| i]) =
distance| i] = Wli][vnear|; // 갱신한다.

nearest| i] = vnear

}

|  『ㆍ(프림 알고리즘)의 일정 시간복잡도 분석
위연산 : 06068【-루프 안에 있는 두 개의 《ㅠ-루프가 있는데, 각각 n— 13) 반복한다.

인 ㆍ

안에 명령문들의 한 번 실행을 단위연산으로 한다.
입력크기 : 7,(마디의 개수)

"6068『-루프를 -1번 반복하므로 시간복잡도는 다음과 같다.

ㄴㄴ ra

T(n) =2(n—1)(n—-1) € O(n?)

18
oe
nue,
KI
we
ON
2,
(a
om,
10
ww
nu
hh
fr
~

은 확실하다. 그러나 필연적으로 최소비용이


===== PAGE 167 =====
@00@00000 0
154     chapter 4 탐욕 알고리즘

될까? 각 단계에서 에 가장 가까운 마디를 선택하므로, 직관적으로 보면 트리는 최소
비용이 되어야 한다. 그러나 정말 그렇게 되는지 증명할 필요가 있다. 비록 탐욕 알고리
즘이 동적계획 알고리즘보다 만들기는 쉽지만, 항상 최적해를 주는지 결정하는 작업은
탐욕 알고리즘이 더 어려운 게 보통이다. 동적계획 알고리즘의 경우에는 AAS] 원칙이
성립하는지만 보이면 되었다. 탐욕 알고리즘의 경우에는 보통 정식으로 증명해야 한다.
이제 프림 알고리즘이 항상 최적해를 주는지 증명해보자.

비방향그래프 G=(V, £)7} 있다고 하자. FS] 부분집합 에다 최소비용 신장트리
가 되도록 이음선을 추가할 수 있으면 FS 유망하다(6ㅠ0018108)라고 한다. 그림 4.8(8)

에서 부분집합 {(v,, 0), (01, 5 )} 은 유망하고, 부분집합 {(06, 0, )} 는 유망하지 않다.

< | <보조정리 41
@=( 24) 를 연결된 가중치포함, 비방향그래프라 하며, FS #의 유망한 부분집합이라 하
고. YE Fo] 속한 이음선으로 연결된 마디의 집합이라 하자. 만약 Yo] 속한 마디를 v— voy
속한 마디로 연결하는 이음선 중에 가중치가 최소인 이음선을 ee} 하면, FU (e) 는 유망하다.
증명 : Fe 유망하므로, 다음 관계가 성립하는 이음선의 집합 /가 반드시 존재하고,

Fer
(V, 2")는 최소비용 신장트리가 된다. 만약 ee’ eps, 다음 관계가 성립한다.
F’ U{e} CF’

이는 FU {e} 가 유망하다는 AS 의미하고, 따라서 증명이 완료되었다. 그렇지 않으면(6ㄷ2"
이 아니면) (VY, 2")가 신장트리이므로 ^ ㄴ416} 는 정확하게 하나의 순환경로를 포함하게 =]
고, et 반드시 그 순환경로 Aho] 한 이음선이 되어야 한다. 그림 4.6에서 이를 설명해 주는데,
여기서 순환경로는 [,, vy, vy 0]이다. 그림 4.6에서 볼 수 있듯이 에 속한 마디에서 1- ※
에 속한 마디를 연결하는 어떤 다른 OSA (EF 도 그 순환경로 Aho] 반드시 속해 있게 된
다. FY Ufe} 에서 ec’ 을 제거하면 순환경로는 없어지게 되며, 다시 신장트리가 된다. 그런데
6는 에 속한 한 마디에서 V— Yo) 속한 마디를 연결하는 이음선 중에 가중치가 AAA 이음
선이기 때문에 6의 가중치는 ㅇ 의 가중치보다 반드시 작거나 같아야 한다(실제로는 반드시
같게 된다). 그래서 다음은 최소비용 신장트리가 된다.

※ㅠ01616
결론적으로 6 는 Fo] 절대로 속할 수 없으므로(에 속한 이음선들은 Yo] 속한 마디들만을
연결함을 기억하시오), 다음 관계식을 얻을 수 있다.

FU {e} CFU {e}—{e'}

따라서 FU {6}는 유망하고, 그래서 증명이 완료되었다.



===== PAGE 168 =====
그림 4.6 보조정리 4.1의 증명과정을 설명하는 그래프. 2" 에 속한 이음선은 진하게 표시되어 있다.

정리 4.1

프림 알고리즘은 항상 최소비용 신장트리를 만들어 낸다.

증명 : Ad Gnduction)& 사용하여 repeat -—F 7} 매번 수행 후에 집합 가 유망하다는
것을 증명하면 된다.

귀납기초 : 공집합은 당연히 유망하다.

귀납가정 : repeat—F ZA] 어떤 주어진 반복이 이루어진 후 그때까지 선택한 이음선의 집
합인 Fe 유망하다고 가정한다.

귀납절차 : 집합 FU {6} 가 유망하다는 것을 보   이면   된다. 여기서 6는 다음 반복을 실행할

이음선이다. 그런데 이음선 6는 Yo) 속한 어떤 마디를 ~ vo] 속한 어떤 마디로
결하는 이음선 중에서 최소의 가중치를 가지고 있기 때문에 보조정리 4.1에 의하여
U {6} 는 유망하다. 귀납 증명이 완료되었다.

귀납증명에 의하여 이음선의 최종 집합은 유망하다. 이 집합은 신장트리의 이음선으로 구성
므로, 그 트리는 최소비용 신장트리임에 틀림없다.

ra 포
rx
1

최소비용 신장트리 문제를 풀기 위한 크루스칼 알고리즘0@466816 Algorithm)-2 각 uf
디마다 자신만 포함하는 VO] ABA 부분집합들을 만드는 걸로 시작한다. 그리고 가중
치가 작은 것부터 차례로 이음선을 검사한다(가중치가 같으면 임의로 선택한다). 만약


===== PAGE 169 =====
@00@00000 0
156     chapter 4 탐욕 알고리즘

어떤 이음선이 서로소 부분집합들에 있는 두 마디를 연결하면 그 이음선을 추가하고, 두
부분집합을 하나로 합친다. 다음은 이 절차를 고수준으로 표현한 알고리즘이다.

F=9;                                         // 이음선의 집합을 공집합으로 초기화
[의 서로소 부분집합 구축(각 마디마다 하나씩, 그 마디만 포함하도록 한다);

Eo] 속한 이음선을 가중치가 작은 것부터 차례로 정렬;
while (답을 구할지 못했음) {

다음 이음선을 선택;                             // 선택절차

if (이음선이 ABA 부분집합의 두 마디를 연결한다) {  // 적절성 점검
부분집합을 합침 ;

크 의음신을 #에 주가:

if (모든 부분집합이 하나로 합쳐졌음)                 // Waa
Be 쿠했음

그림 4.7을 보면 크루스칼 알고리즘이 어떻게 진행되는지 알 수 있다.

크루스칼 알고리즘을 정식으로 작성하기 위해서는 서로소 집합 추상데이터타입이 필
요하다. 이 데이터타입은 부록 0에 구현되어 있다. 그 부록에서는 인덱스의 서로소부분
집합에 대하여 구현되어 있으므로, 그 구현을 사용하기 위해서는 마디를 인덱스로 표시
하기만 하면 된다. 서로소 집합 추상데이터타입은 1106×와 set_pointer 데이터타입과
initial, find, merge, equal7} 같은 연산으로 구성한다. 다음과 같이 선언하고,

index 27;
set pointer p, g;
연산은 아래와 같이 정의한다.

* initial (n)= nN] 서로소부분집합을 초기화하는데, 각 서로소부분집합은 1부터
/사이의 인덱스 중에서 정확하게 하나만 포함한다.

© p= find i) p7t 인덱스 +B 포함하고 있는 집합을 가리키게 한다.

© merge (p,q) 와 0가 가리키고 있는 두 개의 집합을 하나로 합친다.

* equal(p,q)= 2와 0가 같은 집합을 가리키면 trues 넘겨준다.

ㆍ 알고리즘 4.2 크루스칼 알고리즘


===== PAGE 170 =====
1. 이음선을 가중치가 작은 것부
차례로 정렬한다.

QO ©

("7
S

re  nN  00  =
a ^ oO ae)
BS  x  =  로
i  =e  몰  Ss
을 을 = =

(V4,V5)  5

(Vo,V4) 6

~
u

선택한

4. 이음선 (\,\)

7. 이음선 (\,닛)

한

그림 4.7 가중치 그래프(왼쪽 위 끝부분에 위치)와 그 그래프에 he


===== PAGE 171 =====
@0@00000 0
158     chapter 4 탐욕 알고리

OW

ㆍ  스
입력: 정수 2

a

> 2), 양의 Bm, n 7H] 마디와 7//개의 이음선을 가진 연결된 가중치포
함 비방향그래프. 이 그래프는 가중치와 함께 이음선이 포함된 집합 LE 표현한다.
출력 : 최소비용 신장트리에서 이음선의 집합

void kruskal (int n, int m,
set_of_edges E,
set_of edges& F)

index 2, / ;
set_ pointer p, g;
edge e;

Bo] 속한 #깨의 이음선을 가중치가 작은 것부터 차례로 정렬한다;
F=@;
initiak n) ;                 // 개의 소로소부분집합을 초기화
while FO} 이음선의 수는 4 - 1보다 작다) {

e = 이직 고려하지 않은 이음선 중 가중치가 최소인 이음선;
i, j= e@ 연결된 마디의 인덱스;

p = 20000,

q = find()) ;

if (! equaKp, q)) {
merge(p, 9) ;

eS Fol 추가;

신장트리에 이음선이 7ㅡ1개 있으므로, Fo} n—1749] 이음선이 있을 때 while 루
=

W(n)E O(m 18 m)

2, while 루프에서 걸리는 시간. ABA 집합을 조작하는데 걸리는 시간이 이 루프에서


===== PAGE 172 =====
의 시간복잡도를 좌우한다(왜냐하면, 나머지는 모두 상수이기 때문이다). 최악의 경
우, while FES 빠져나가기 전에 이음선을 모두 고려하는데, 이는 루프를 mH 반
복한다는 뜻이 된다. 부록 0의 서로소 집합 데이터구조 프라고 하는 구현방법을 쓰
find, equal, merge 2} 같은 SAS 호출하는 횟수가 상수가 되는 루프를 7) 번 반복
하는 시간복잡도는 다음과 같다.
W(m) © O(mlg m)

여기서 단위연산은 비교명령문이다.

3, nN ABA 집합을 초기화하는데 걸리는 시간. 앞에서 언급한 ASA 집합 데이터
구조의 구현방법을 사용하면, 초기화하는 시간복잡도는 다음과 같다.

T(n) © O(n)
m>n-1° BS, ABA 집합을 정렬하고 조작하는 시간이 초기화시간을 지배한
다. 따라서 다음과 같다.
W(m, n) © 0 (072 18 m)

최악의 경우가 의 값과는 상관이 없는 것처럼 보일지도 모른다. 그러나 최악의 경우
모는 마디는 다른 모든 마디와 연결되기 때문에 다음과 같다.

_ n(n—1)

5   = O(n’)

그러므로 최악의 경우에 다음과 같이 4 수도 있다.
w(m, n) €O(n? lg 72?) = O(n? 216 n) = O(n? 18 n)

크루스칼 알고리즘을 프림 알고리즘과 비교할 때 최악의 경우에 대해서 위의 두 가지

크루스칼 알고리즘이 항상 최적의 해답을 준다고 증명하기 위해서 다음 보조정리가

<

«BBP 4.2

GY, Ex 연결된 가중치포함 비방향그래프, 는 LS] 유망한 부분집합, 는 FU {6} 하여
순환이 생기지 않도록 하여 &-~ㅅ에 속한 최소 가중치 이음선이라 하자. 그러면 Fu {es =

81] SYS 보조증명 419] 중명과 비슷하다. 가 유망하기 때문에 다음 식을 만족하는
이음선의 집합 /^가 존재해야 하고


===== PAGE 173 =====
160

chapter 4 탐욕 알고리

oh

(V, F)E 최소비용 신장트리이어야 한다. 만약 62" 인 경우,
※ㄴ10 er

이는 FU {6} 임을 의미하고, 따라서 증명을 완료했다. 그렇지 않은 VP (VY, 7" )가 신장트
리이므로 FU {6} 는 정확하게 순환을 하나 포함하고 있어야 하며, 6기 비로 크 순환이어야
한다. 그런데 FU {6} 에는 순환이 없으므로 그 순환에 속한 어떤 이음선 6 EF’ 7} 존재해야
하고, 그 이음선은 Fol 속하지 않는다. 즉, 6 = & FA 된다. 집합 KU 16 } 에는 aH
분집합이므로 순환이 존재하지 않는다. 그러므로 6의 가중치는 6' 의 가중치보다 크지 않다(6
를 FU {6} 하여 순환이 생기지 않도록 하여 &- Fol] 속한 최소 가중치 이음선이라고 가정하
였음을 상기하라). FU {6} 에서 6' 를 제거하면 이 집합에서 순환은 없어지며, 이는 AVE
리가 됨을 뜻한다. 실제로 다음 집합은 최소비용 신장트리가 된다.

F Ufe} 을 {6}

왜냐하면, 위에서 보여준 대로 ㅇ의 가중치는 ㅇ'의 가중치보다 크지 않다. ㅇ'가 에 속하지
않으므로 다음과 같다.

FuU{e} CF U{e}—{e’'}
따라서 FU {6} 는 유망하고, 따라서 증명이 완료되었다.

크루스칼 알고리즘은 항상 최소비용 신장트리를 만들어 낸다.
집합에서 시작하여 귀납법으로 SRS}, 보조정리 4.2를 이용하여 SVS
습문제로 남겨 둔다.

도 Up

41.3 Hea} 크루스칼 알고리즘의 비교
시간복잡도가 다음과 같다.
프럼 알고리즘 :      T(n)€ O(n’)
ABAD 알고리즘 : Wm, 2) O(mlgm) A Wm, n)E O(n’ Ign)
연결된 그래프에서 다음 부등식이 성립함을 또한 증명하였다.

이음선의 개수 mo] 이 범위의 하한과 가까운 그래프에 대하여(저밀도 그래프-808186
graph), 크루스칼 알고리즘은 0ㅇ(2 18 7)이므로 크루스칼 알고리즘이 더 빠르다. 그러나
이음선의 개수가 이 범위의 상한과 가까운 그래프에 대하여(고밀도 그래프-46086 graph),

크루스칼의 알고리즘은 0(02^1870)이므로 프림 알고리즘이 더 빠르다.


===== PAGE 174 =====
4.1.4 마무리 토론
위에서 언급했듯이 어떤 알고리즘의 시간복잡도는 구현하는데 사용한 데이터구조에 좌우
되는 경우가 종종 있다. 1977년 Johnson°] 힙(8082) 데이터구조를 사용하여 O(m 18 n)
프럼 알고리즘을 구현하였다. 저밀도 그래프에서는 ㅇ(02187)으로 이 WAS] 알고리즘
에 비해서 빠르지만, 고밀도 그래프에서는 O(n? lg n) OS 더 느리다. 1987년 Fredman
과 Tarjan(1987)2 피보나찌힙 데이터구조를 사용하여 가장 빠른 프림 알고리즘을 개발
하였는데, 시간복잡도는 ㅇ(/77+ㅠ718 7)으로 저밀도 그래프에서는 ㅇ(72187)이고 고밀
도 그래프에서는 ㅇ(2”)이다.

프림 알고리즘은 1930년 Jarniko] 처음 발표하였고, 이름은 2420ㅇ| 1957년에 발표한
논문에서 유래한다. 크루스칼 알고리즘은 ㅠ048881이 1956년에 발표한 논문에서 유래한
다. 최소비용 신장트리 문제의 SAKE Graham} Hello] 1985년 발표한 논문에 정리되어
있다. 이 문제의 다른 알고리즘으로는 1975년 발표한 780의 알고리즘과 1983년 발표한

7?840482의 알고리즘을 들 수 있다.

@ 42 단일출발점 최단경로 문제를 푸는 다익스트라 알고리즘

8.2절에서 가중치포함 비방향그래프에서 각 마디에서 다른 모든 마디로 가는 최단경로를
모두 구하는 O(n*) 알고리즘을 개발하였다. 하나의 특정 마디에서 다른 모든 마디로 가
는 최단경로들만 알고 싶다면, 그 알고리즘은 쓸데없이 과다하다. 이제 탐욕적인 방법을
사용하여 단일출발점 최단경로 문제(810816-804706 shortest paths 20"001020라고 부르는
EAS 푸는 O(n’) 알고리즘을 개발해보자. 이 알고리즘은 1959년 다익스트라(20688)가
고안해 내었다. 관심 있는 마디에서 다른 각 마디로 가는 최단경로가 존재한다고 가정하
고 이 알고리즘을 설명한다. 그렇지 않은 경우를 처리하기 위해서는 조금만 SAS 가하
면 된다.

이 알고리즘은 최소비용 신장트리 BAIS 푸는 알고리즘과 비슷하다. 최단경로를 구하
려고 하는 마디만 포함하도록 집합 VS 초기화한다. 편의상 이 마디를 이라고 하자.
이음선의 집합 FE 공집합으로 초기화한다. 먼저 0, 에서 가장 가까운 마디 oS 선택하
여 에 추가하고, 이음선 (yy, 0>를 FO] 추가한다(여기서 <0;, vd 에서 v= 가는
방향성 이음선을 의미한다). 이 이음선은 명백하게 0, 에서 2 로 가는 최단경로이다. 다음
에서 V— Yo) 속한 마디로 가는 경로 중에서 에 속한 마디만을 중간에 거쳐 가는
경로를 검사한다. 이 경로들 중에서 가장 짧은 경로가 최단경로이다(이는 증명이 필요하
다). 그 경로의 끝에 위치한 마디를 Yo] 추가하고, 그 경로 상에서 그 마디로 가는 이음
AS Fo] 추가한다. 가 모든 마디의 집합인 와 같아질 때까지 이 과정을 되풀이한
다. 이 AAA] FE 최단경로에 속한 이음선을 포함하게 된다. 다음은 이 방법을 추상



===== PAGE 175 =====
@eeeee 0
162     chapter 4 탐욕 알고리즘

Y= {v,};
F=@;

while (BS 구하지 못했음) {
Yo] 속한 마더만 중간에 AA 가는 마더로 하여        // 선택절차와
vy, 에서의 최단경로를 가진 마디 를               // 적절성 점검
V— 에서 선택한다;

새로운 마디 를 에 추가한다;
(최단경로 상에서) 『로 가는 이음선을 에 추가한다;

if (Y ==

Be TUS                              // 해답점검
}
그림 4.8에 다익스트라 매시   실행절차를 예로 설명한다. 프림 알고리즘과 마찬
가지로 이렇게 고수준으로 표현한 알      ae 즘은 소규모 그래프를 보면서 사람이 답을 찾는
경우에만 쓸 만하다. 이제 세부적인 알고리즘을 살펴보자. 이 알고리즘에서 가중치 그래
프는 3.2절에서와 같이 이차원 배열로 표현한다. 이 알고리즘은 알고리즘 4.1(프림)과 매
우 유사하다. 2087657와 distance 배열 대신 다음과 같은 touch? length WSS 사용하
는 것의 다르다. 47/4 i= 2, ~ 0
touch|i] = Yo] 속한 마디들만 중간에 거치도록 하여 v, 에서 v= 가는 현재 최단
로 상의 마지막 이음선을 <0, 0,>라고 할 때, 에 속한 마디 v4] ara
length [i] = Yo) 속한 마디들만 중간에 거치도록 하여 v, 에서 <,로 가는 현재 최단경
로의 길이
이 알고리즘은 다음과 같다
+543 다익스트라 알고리즘

문제 : 가중치포함 방향그래프에서 ?(,에서 다른 모든 마디로 가는 최단경로를 구하시오.
입력: 정수 (= )와 마디가 *개 있는 연결된 BAD BAAS, 이 ate 이차
원 배열 We 표현되며, 행과 열의 인덱스는 각각 1부터 7까지이다. 여기서 ^011/]는
;번째 마디에서 번째 마디를 잇는 이음선 상의 가중치가 된다.
출력 : 최단경로 상에 놓여있는 이음선의 집합 7

void dijkstra(int 2, const number 141 ][], set_of_edges& F)

{


===== PAGE 176 =====
42 단일출발점 최단경로 PAS 푸는 다익스트라 알고리즘      163
1. \ 를 선택하는데 그 이유는         2. 를 선택하는데 그 이유는 {vg}o 속한
YO 가장 가깝기 때문이다.         마디만 중간에 거쳐서 버에서 가는

최단경로이기 때문이다.

3. 를 선택하는데 그 이유는        4. 너에서 \로 가는 최단경로는
{4, V5}Oll 속한 마디만 중간에           [V4, 9 V4, VoJOICH.
거쳐서 너에서 가는 최단경로
이기 때문이다.

그림 4.8 (상단의 왼쪽 구석에 위치한) 가중치가 있는 방향그래프와 그 그래프로 다익스트라 알고
리즘을 단계별로 실행한 결과. Yo 속한 마디들과 Fol 속한 이음선들은 각 단계에서 진하게 칠해
져 있다.
index 2, vnear;
edge e;
index touch|2..n];
number J/ength{2..n\;
= 23
for (7 = 2; 7 <= n; H+) {           // 각 마디에 대해서,
“00001 = 1;                        // 끼에서 출발하는 현재 최단경로의 마지막 마디를
99412] = W{1][4];            // 1423 초기화한다.
}                                   // 그 경로의 길이는 4,에서의 이음선 상의 가중치로

// 초기화한다.

repeat (2-번) {

Tin = Co:

for (i = 2; 7 <= m; H+) {         // 최단경로를 가지는지 각 마디를 점검한다.

u


===== PAGE 177 =====
@‥00@0060000 0
164     chapter 4 탐욕 알고리즘
if (0 < Jength| i] < min) {

min = length| i] ;
vnear = 1;

e = touch[vnear|7} 인덱스인 마디에서 vnear7} 인덱스인 마디로 가는 이음선 ;

eS Fo

주가

for (2 = 2; 7 <= n; H+) {

if (length|vnear| + Wvnear|[i] < Jength|
length| i| = length{vnear| + W\vnear[

){

2:

4
i]

touch{ i] = vuear;          // Yo) 속하지 않는 각 마디에 대해서,

}

// 최단경로를 바꾼다.

length|vnear| = —1;               // vnear7} VAAS 마디를 에 추가한다.

에서 다른 모든 마디로 가는 경로가 존재한다고 가정하기 때문에 변수 14000는 re-
peat 루프의 각 반복 단계에서 새로운 값을 가지게 된다. 만약 이런 가정이 없다면 이
알고리즘에 쓰여진 대로 repeat 루프의 n-1 반복이 끝날 때까지 마지막 이음선을 계
속해서 추가하게 될 것이다.

알고리즘 4 32 최단경로 상의 이음선만 찾는다. 이 경로의 총 길이는 계산하지 않는
다. 그 길이는 이음선을 가지고 계산할 수 있다. 대안으로 알고리즘을 조금 수정하면 그
길이를 구하여 배열에 저장하게 할 수 있다.

알고리즘 4.8의 제어구조는 알고리즘 4.1과 똑같다. 따라서 알고리즘의 4.1의 분석을
그대로 가져다 쓰면 알고리즘 435] 분석 결과도 다음과 같음을 알 수 있다.

T(n) = 2(n—1)? €O(n?)

명하는데 사용한 방법과 유사하게 귀납법을 사용하여 증명한다.                        ,
프림 알고리즘의 경우와 같이 다익스트라 알고리즘도 힙이나 피보나찌힙 데이터구조
를 사용하여 구현할 수 있다. 힙으로 구현하면 O(m lg n)o|a1, 피보나찌힙으로 구현하
면 0077 +7ㅠ1870)이다. 여기서 me 이음선의 개수이다. 피보나찌힙으로 구현으로 구현

하는 세부적인 ARES 1987년 발표한 Fredmans} 18000의 논문에 나와 있다.

@ 43 스케줄 짜기

어떤 미용사에게 여러 가지 다른 미용서비스를 받으려고 (예를 들어, 커트, 커트/샴푸,
파마, 염색) 기다리고 있는 손님이 있다고 하자. 이와 같이 머리하는 종류별로 걸리는 시


===== PAGE 178 =====
© 예제 4.2

@000600000
4.3 스케줄 짜기   165

간이 서로 같지 않고, 미용사는 각각 얼마나 걸릴지 알고 있다. 기다리고 머리하는데 걸
리는 시간이 최소가 되도록 손님을 서비스하는 스케줄 짜기(601604108)는 투자해볼 만
한 가치가 있는 일이다. 손님이 기다리고 머리하는데 걸리는 시간을 AAS 하는 스케줄
을 최적 스케줄이라고 한다. 기다리고 머리하는데 걸리는 시간을 시스템 내부 시간(41706
in the 8786600이라고 한다. 실제로 시스템 내부의 총 시간을 최소가 되도록 하는 문제는
주위에서 많이 찾아볼 수 있다. AS 들어, 디스크드라이브 사용자들이 기다리고 서비스
받는데 소요되는 총 시간이 최소가 되도록 디스크 사용 스케줄을 짜는 문제도 마찬가지
이다.

또 다른 스케줄 짜기 문제는 각 작업(또는 손님에 대한 서비스)을 끝내는데 같은 시간
이 걸리지만 각 작업과 관련된 보상을 얻기 위해서 시작해야 하는 마감시간이 있는 경우
이다. 목표는 총 보상을 최대가 되도록 작업의 스케줄을 짜야 한다는 것이다. 시스템 내
부의 총 시간이 최소가 되도록 하는 간단한 스케줄 짜는 BAIS 먼저 알아본 후에 마감시
간이 있는 스케줄 짜기(6016041108 with deadlines) HAS 공부하기로 하자.

4.3.1 시스템 내부의 총 시간의 최소화
시스템 내부의 총 시간이 최소가 되는 간단한 해법은 가능한 모든 스케줄을 고려해 보고
그 중 최소를 취하는 것이다. 이 방법은 다음 예제로 설명한다.

작업이 37] 있고, 작업을 하는데 걸리는 시간은 각각 다음과 같다.
i=) 2-0, «=a

실제 시간의 단위는 이 문제와는 관련이 없다. 만약 1, 2, 39] SAS 스케줄을 ze}el 이 작업
3개를 완료하는데 시스템 내부에서 걸리는 시간은 다음과 같다.

작업                        시스템 내부 시간
1      5 (작업시간)
2      5 (작업 1 대기시간) +10 (작업시간)
3      5 (작업 1 대기시간) +10 (작업 2 대기시간) + 4 (작업시간)

이 스케줄에서 시스템 내부에서 걸리는 총 시간은 다음과 같다.
5    +     (5+10) +    (5+10+4) =39

작업 1을 끝내는데 작업 28 끝내는데 작업 8을 끝내는데
걸리는 시간        걸리는 시간           걸리는 시간

a 다음과 같이 가능한 BE 스케줄과 시스템 내부에서 걸리는 총 시간을 만들어

스케줄        시스템 내부의 총 시간
외인   5 + (5 + 10) + (5 + 10 + 4) = 39
1 3, 의   5 + (5 + 4) + (5 + 4 + 10) = 33


===== PAGE 179 =====
166

chapter 4 탐욕 알고리즘

[2, 1, 3]   10 + (10 + 5) + (10 + 5 + 4) = 44
[2, 3, 1]   10 + (10 + 4) + (10 + 4 + 5) = 48
@ 이   4-+(4+5)-+(4+5-+ 10 = 32
[8 21]   4-+(4+10+(4+10+5)= 87

스케줄 [3,1,9]가 총 시간이 32로 최적이다.

가능한 모든 스케줄을 고려해 보는 알고리즘의 실행시간은 계승(68아00191-\106)이다.
앞의 예제에서 보았듯이 최적 스케줄은 작업시간이 가장 짧은 작업(작업시간이 4인 작업

3)& 먼저 하고, 다음에 작업시간이 두 번째로 짧은 작업(작업시간이 5인 작업 YS 하고,
마지막으로 작업시간이 가장 긴 작업(작업시간이 10인 작업 9을 하는 것이다. 직관적으
로 보면, 작업시간이 가장 짧은 작업을 먼저 수행하므로 이러한 스케줄이 최적인 것처럼
보인다. 이 방법을 고수준으로 표현한 탐욕 알고리즘은 다음과 같다.

작업시간 별로 작업을 비내림차순으로 정렬한다;

while (HS 구하지 못했음) {

다음 작업을 스케줄에 넣는다;                        // 선택절차와

// 적절성 점검

1 (작업이 더 이상 없다)

BS 구했음;                                                           // 해답점검

이 알고리즘이 진짜 탐욕 알고리즘임을 보여주기 위해 탐욕 알고리즘의 일반 형태로
작성하였다. 그러나 알고리즘이 하는 일은 작업시간별로 작업을 정렬하는 일 뿐이다. 따
라서 시간복잡도는 다음과 같다.

W(n) € O(nlg n)

비록 직관적으로 이 알고리즘이 만들어 낸 스케줄이 최적인 것 같아 보이지만, 증명할
EO %

필요가 있다. 이 스케줄이야말로 최적 스케줄일 수밖에 없다는 더 강력한 결과를 다음
정리는 증명한다.
정리 4.3

시스템 내부의 총 시간이 최소가 되도록 하는 유일한 스케줄은 작업시간별로 작업을 비내림차
순으로 스케줄이다.

증명 : 1s<i<n-19 범위를 가진 i 대해서 *를 어떤 특정 최적 스케줄(시스템 내부의
총 시간을 최소가 되는 스케줄)에 포함되어 있는 째 작업의 작업시간이라고 하자. 이 스케줄
은 작업시간별로 작업을 비내림차순으로 스케줄 S 작업들로 이루어짐을 증명할 필요가 있다.


===== PAGE 180 =====
@©eeeeee
43 스케줄 짜기   167

모         명방법으로 이를 증명해보자. 만약 비내림차순으로 스케줄이 짜져 있지 않다면,
1 <i <n-19} 범위 내에서 최소한 하나의 iol 대해서 다음 부등식이 성립할 것이다.

t, >t, +1

원래 스케줄을 :째와 (+ 1)째 작업을 바꿔서 재배치할 수 있다. 이렇게 바꾸면, (원래 스케줄
에서) (i+ 1) 작업이 시스템 내부에서 소모한 시간을 《 만큼 빼낸 결과를 초래한다. 이유는
(원래 스케줄에서처럼) *째 작업을 하는 동안 기다릴 필요가 더 이상 없기 때문이다. 비슷하게
(원래 스케줄에서) *째 작업이 시스템 내부에서 소모한 시간을 + 1만큼 추가한 결과를 초래
한다. 명백히, 어떤 다른 작업에 대해서는 스케줄을 변경하지 않았다. 따라서 원래 스케줄에서
시스템 내부의 총 시간을 7라 하고, 변경한 스케줄에서 총 시간을 7"라 하면, 다음과 같은

S  으  OA

| olN

T =T+t,+1=¢
그런데 4, >t, +1이기 때문에 다음과 같은 식을 유추할 수 있고,
T <=

이 부등식은 원래 스케줄이 최적이라는 사실과 상반된다.

이 알고리즘을 복수작업자 스케줄 짜기 HA] (multiple-server scheduling problem)=
푸는 알고리즘으로 일반화하기는 쉽다. 작업자가 my 있다고 가정해보자. 그 작업자의
순서는 무작위이다. 작업시간별로 작업을 비내림차순으로 정렬한다. 첫째 작업자는 첫째
작업을 하고, 둘째 작업자는 둘째 작업을 하고, .……, mal 작업자는 mA 작업을 한다.
첫째 작업자가 작업시간이 가장 짧은 작업을 하기 때문에 가장 먼저 끝날 것이다. 따라서
첫째 작업자는 (77 + 1)째 작업을 하게 된다. 비슷하게 둘째 작업자는 (7, + 2)째 작업을
하게 되고, 같은 식으로 계속된다. 이 방법은 다음과 같다.

」

작업자 Le 다음 작업들을 수행한다. 1, (1+m), (1+2m), (1+3m)....
작업자 22 다음 FHSS 수행한다. 2, (2+m), (2+ 272), (2+3m),...

작업자 은 다음 FHSS 수행한다. i, (i+m), (+ 272), (6 +3m),...

작업자 m= 다음 작업들을 수행한다. m, (m+m), (m+2m), (m+3m),...
명백하게, 작업은 결과적으로 다음 순서로 처리하게 된다.
dy 2 Mes Lm; 2b, ae mem: 12m, =.

즉, 서비스시간별로 비내림차순으로 처리된다.


===== PAGE 181 =====
@0@00000 0
168     chapter 4 탐욕 알고리즘

* 예제 4.3

4.3.2 마감시간 있는 스케줄 짜기

마감시간이 있는 스케줄 짜기 문제에서 각 작업을 끝내는데 1의 단위시간이 걸리고, 마감
시간과 보상이 할당되어 있다. 작업을 마감시간 전이나 마감시간에 마친다면 보상을 받
는다. 목표는 총 보상액이 최대가 되게 작업 스케줄을 짜는 것이다. 모든 작업을 스케줄
에 포함시킬 필요는 없다. 마감시간 후의 작업은 보상이 없으므로 아예 작업을 하지 않는
것과 마찬가지이다. 그러한 스케줄을 불가능02ㅁㅁ0881010)한 스케줄이라고 한다. 다음 예
제를 보고 이 문제를 잘 이해해보자.

작업, 마감시간, 보상이 다음과 같다고 가정해보자.

작업            마감시간           보상
1                  2                 30
2                  1                  35
3                  2                 25
4                  |                  40

“작업 1은 마감시간이 8이다"의 의미는 “작업 1을 시점 1 또는 8에 시작할 수 있다"가 된다. 시점
0이라고는 존재하지 않는다. 작업 QE 마감시간이 1이므로 그 작업은 시점 1에서만 시작할 수
있다. 가능한 스케줄과 총 보상은 다음과 같다:

스케줄                종 보상

1 3]            30 + 25 = 55
[2, 1]            35 + 30 = 65
[2, 3]           35 + 25 = 60
[3, 1]            25 + 30 = 55
[4, 1]           40 + 30 = 70
[4, 3]           40 + 25 = 65

불가능한 AASS 나열하지 않았다. AS 들어, AAS [1, 이는 가능하지 않고, 따라서 나열하
지 않았다. 왜냐하면, 작업 1을 먼저 시점 1에서 시작하고, 끝나는데 1 단위시간이 걸리게 되어
작업 2S 시점 에서 시작해야 하기 때문이다. 그러나 작업 29] 마감시간은 시점 1이다. 예를
들어, 스케줄 [1, 312 가능한데, 그 이유는 작업 1을 그 작업의 마감시간 전에 시작하고, 작업
8을 그 작업의 마감시간 전에 시작하기 때문이다. 스케줄 [4, to] 총 보상이 700] 되며 최적이라

는 사실을 금방 알 수 있다.

예제 4.8에서 보았듯이 모든 스케줄을 다 따지면 계승시간이 걸린다. 보상이 가장 많
은 작업(작업 4)이 최적 AAS] 들어가지만, SAS 많은 작업(작업 22 그렇지 않다
는 사실을 주목해보자. 두 작업 모두 마감시간이 1이므로 둘이 한꺼번에 스케줄에 들어갈
수 없다. 물론 보상을 가장 크게 내는 작업이 스케줄에 들어간다. 스케줄에 들어간 다른
작업은 작업 1인데, 그 이유는 그 보상이 작업 3보다 크기 때문이다. 이 문제를 푸는 A


===== PAGE 182 =====
0000000
4.3 스케줄 짜기   169

으

a

wu,
at uN
Ku

상이 큰 것부터 차례로 작업을 먼저 정렬하게 될 것임을 암시한다.
사하여 그 작업이 가능한 작업이면 스케줄에 포함시킨다. 이 방법
준 알고리즘을 만들기에 앞서서 몇 가지를 정의해보자. 작업 순서
업들을 기 }시간 내에 시작하면, 그 순서를 적절한 순서((6881616 sequence)
라고 한다. 예를 들어, 예제 4.8에서 [4, 11은 적절한 순서이고, [1, 41는 적절한 SAV}
아니다.  작업의 집합에서 최소한 하나의 작당한 순서가 존재하면 그 집합은 적절한 집합
(feasible 860이라고 한다. 예제 4.3에서 {1, 사는 스케줄 순서 [4, 11이 적절하므로 적절한
반면 {2, 사는 둘 중 어떤 작업도 마감시간 안에 작업을 시작하지 못하므로 적절한 집합이
아니다. 우리의 목표는 총 BAS 최대로 하는 적절한 SAS 찾는 것이다. 그러한 순서
를 최적 순서(6041081 886046008)라 하고, 그 순서에 속한 작업의 집합을 작업의 최적 집합
(optimal set of ]068)이라고 한다. 이제 마감시간이 있는 스케줄 짜기 문제를 푸는 고수

준 알고리즘을 소개한다.

2 of
ㅁ
we

re J
tho
Ay 나

a

o N (위
고
때
#
ae 때 ft

에 |ㅁ Ao
n

ox

Jo

}

N

더 다
g 뿌
ㅁ

오곤

fl
0 0

작업을 보상이 큰 것부터 차례로 정렬한다;
6= 0
while (EH 구하지 못했음) {
다음 작업을 선택 ;                          // 선택 절차
 (이 작업을 추가하면 가 적절하다)            // 적절성 점검
이 작업을 Sol 추가;
 (더 이상 작업이 없다)                   // 해답점검
답을 구했음;
}
다음 예제는 이 알고리즘의 실행과정을 보여준다.
*예제 44 작업, 마감시간, 보상이 다음과 같다고 가정하자.

작업          마감시간         보상
il                             3                            40
2                             iL                            35
3                             1                            30
4                             3                            25
5                             al                            20
6                             3                            15
7                             2                            10

라벨을 붙이기 전에 작업을 이미 정렬하였다. 앞에서 살펴본 탐욕적인 알고리즘은 다음과 같은
절차로 수행한다.
1. SE ㅇ으로 놓는다.


===== PAGE 183 =====
@0@000000
170     chapter 4 탐욕 알고리즘

순서 [1]이 적절하므로 SS {마로 놓는다.

순서 [2, 1이 적절하므로 SS {1, 아로 놓는다.

{1, 2, 이은 적절한 순서가 존재하지 않으므로 기각한다.
순서 [2, 1, 417} 적절하므로 SS {1, 2, 상로 놓는다.

(1, 3, 4, 하는 적절한 순서가 존재하지 않으므로 기각한다.
{1, 2, 4, 하은 적절한 순서가 존재하지 않으므로 기각한다.
{1, 2, 4, 아은 적절한 순서가 존재하지 않으므로 기각한다.

2 고이 ee eS 너

9의 최종값은 (1, 2, 시가 되고, 이 집합에 대한 적절한 SAME [2, 1, 신가 된다. 작업 1과 4는

모두 마감시간이 8이므로, 적절한 순서인 (2, 4, US 대신 사용할 수 있다.
이 알고리즘이 항상 최적의 순서를 만들어 내는지를 증명하기 전에 이 알고리즘을 정
식으로 작성해보자. 그렇게 하기 위해서는 집합이 적절한지를 효율적으로 결정하는 방법

이 필요하다. 가능한 경우를 모두 고려해 보는 건 계승시간이 걸리므로 받아들일 수
다. 다음 보조정리를 이용하면 집합이 적절한지 여부를 효율적으로 검사할 수 있

ae

< ㅣ .wxmal 43

© 예제 4.5

SS 작업의 집합이라고 하자. 그러면 “가 적절하다"는 “5에 속한 AAS 마감시간이 감소하
지 않게 나열하여 얻은 순서가 적절하다"의 필요충분조건이다.
증명 : (충분조건) $7} 적절하다고 가정하자. 그러면, Sol] 속한 작업들에 대해서 최소한 하나
의 적절한 순서가 존재한다. 이 순서에서 작업 <는 작업 yO} 앞에 스케줄되어 있고, 작업 0가
작업 보다 마감시간이 ZACH MECH a 가정해보자. 만약 여기서 두 작업의 순서를 바꾼다고
해보자. 작업 y= 더 빨리 작업을 시작하므로 당연히 마감시간 안에 작업을 시작하게 된다.
작업 는 마감시간이 작업 #보다 크고(늦고), 작업 vol] 주어진 새로운 작업시간 SEO] 작업
에도 적당하므로, 작업 *도 또한 마감시간 안에 작업을 시작하게 된다. 따라서 새로 바꾼
순서도 적절하다. 어떤 적절한 순서에 교환정렬(알고리즘 1.9)을 실행하면서 이 사실을 반복
적용시켜서 순서대로 나열된 순서가 적절함을 증명할 수 있다.
(필요조건) 순서대로 나열된 순서가 적절하면 당연히 s= 적절하다.

예제 4.4와 같은 작업이 있다고 가정하자. 11, 2, 4, 이 적절한 지를 결정해보자. 보조정리 4.3
에 의하면 다음 순서의 적절성을 점검하기만 하면 된다.
12 7, 1, 4]
tttt
12 3 3
각 작업의 마감시간을 그 작업 아래에 표시했다. 작업 4B 마감시간까지 스케줄할 수 없기 때문
에 이 순서는 적절하지 않다. 따라서 보조정리 4.9에 의하여 이 집합은 적절하지 않다.



===== PAGE 184 =====
> IG 4.4

@00@000000
4.8 스케술 짜기   121

이제 알고리즘을 살펴보자. 작업들은 알고리즘에 전달되기 전에 이미 보상이 큰 것부
터 차례로 정렬되어 있다고 가정한다. 보상은 작업을 정렬하기 위해서만 필요하므로, 알
고리즘의 파라미터에는 빠져있다.

문제 : 각 작업을 마감시간에 마칠 수 있도록 스케줄을 경우에만 WARS 얻을 수 있을
때 총 보상이 최대가 되도록 스케줄을 짜시오.

입력 : 작업의 수 과 정수 배열 4040/0(인덱스는 1부터 n), 여기서 deadlineti= iA
작업의 마감시간. 배열은 보상이 큰 것부터 차례로 정렬되어 있다.

출력 : 작업의 최적 순서 2

void schedule(int 24,

const int deadline ],
sequence_of_integer& J)

{
index /;
sequence of integer K;
J = (1);
for g =2; 7 <= n, H+) {
= = ./에다가 deadline[ 2]의 값이 작은 것부터 차례로 를 추가;
a 적절하다)
= ^:
}
}
이 알고리즘을 분석하기 전 이 알고
© 예제 4.6     예제 4.4와 같은 작업이 있다고 가정하자. 이 작업들의 마감시간은 다음과 같다.

작업          마감시간
al                                 3
2                                 il
3                             1
4                             3
5                             1
6                             3
th                             2

알고리즘 4.45 다음과 같은 절차로 수행한다.
1. Fe [1]가 된다.


===== PAGE 185 =====
172

chapter 4 탐욕 알고리즘

2, 는 [2, 1이 되고, 적절하다고 결정한다.

J= K7} 적절하므로 [2, 11이다.
3, KE [2, 3, 1]o] 되고, 적절하지 않으므로 기각한다.
4. Ke [2, 1, 시가 되고, 적절하다고 결정한다.

J= 가 적절하므로 [2, 1, 41이다.
5, KE [2, 5, 1, 신가 되고, 적절하지 않으므로 기각한다.
6. AE [2, 1, 6, 신가 되고, 적절하지 않으므로 기각한다.
7. KE [2, 7, 1, 신가 되고, 적절하지 않으므로 기각한다.

의 최종값은 [2, 1, 시이다.

『(마감시간 있는 스케줄 짜기)의 최악 시간복잡도 분석

단위연산 : 작업을 정렬하기 위해서 비교연산이 필요하고, 《와 작업 :가 추가된 JS 같게
놓을 때 비교연산이 또 필요하고, 가 적절한지 검사하는데 비교연산이 또 필요하다. 따
라서 비교연산이 단위연산이다.

입력크기 : 작업의 +n

작업들을 프로시저로 전달하기 전에 작업들을 정렬하는데 O(nign) 시간이 걸린다.
fori 루프마다 에 im 작업을 추가하는데 최대한 ?- 1번의 비교연산이 필요하고, K
가 적절한지를 검사하는데 최대한 1 1번의 비교연산이 필요하다. 따라서 최악의 경우 시
간은 다음과 같다.

21 16-10+0=-1ㄷ600)

첫째 등식은 부록 AS] 예제 A to} 얻는다. 이 시간은 정렬하는데 걸리는 시간에 지배되
므로 전체 시간복잡도는 다음과 같다.

W(n) € O(n’)

마지막으로 이 알고리즘이 항상 최적의 HS SS 증명해보자.

 > Bal 4.4

알고리즘 4.4% 항상 최적의 작업 집합을 만들어 낸다.
증명 : 작업의 수 에 대하여 귀납법으로 증명한다.

귀납출발점 : 작업의 수가 1인 경우는 명백히 정리가 성립한다.

귀납가정 : 처음 개 작업에 대해서 알고리즘으로 구한 작업의 집합은 처음 *개 작업에 대해
서 최적이라고 가정한다.

귀납절차 : 처음 +1개 작업에 대해서 알고리즘으로 구한 작업의 집합은 처음 7+1개 작업


===== PAGE 186 =====
@0000000
4.3 스케줄 짜기   173

에 대해서 최적임을 증명하면 된다. 집합 AS 처음 +1개 작업에 대해서 알고리즘으로 구한
작업의 집합이라 하고, 집합 BS 처음 7+1개 작업에 대하여 최적인 작업의 집합이라고 하
자. 그리고 job(k)S 정렬된 작업 리스트에서 *번째 작업이라고 하자.
다음의 두 가지 경우가 있다.
경우 1 job(n+1)°] Bol] 포함되지 않는 경우

이 경우 BS 처음 /개 작업에서 구한 작업의 집합이다. 그러나 귀납가정에 의하여 는
처음 n7 작업에서 얻은 최적의 작업집합을 포함하고 있다. 따라서 Bol] 속한 작업들의 총
보상은 Aol] 속한 작업들의 총 보상보다 더 크지 않고, 결과적으로 AE 최적일 수밖에 없다.
경우 2. job(n+1)°] Bo] 포함되는 경우

(n+1) HA] 작업이 Aol] 포함되어 있다고 가정하자. 그러면 다음과 같은 식을 구할 수 있다.

B=B' U {job(n+1)}, A=A’ U {job(n+1)}

여기서 BS 처음 7개 작업에서 구한 집합이고, AE 처음 7개 작업에서 알고리즘으로 구한
집합이다. 귀납가정에 의하여 4'는 처음 개 작업에 대해서 최적이다. 그러므로
profit( B) = profit(B’) + profit(n +1)
< profit(A) +profit(n+1) = profit(A)

7]A] profit(n+1)2 job(n+1)2] 보상이고, profit(A)= 에 속한 작업들의 총 보상이다.
Be 처음 7+1개 작업들에 대해서 최적이므로, 4도 마찬가지라고 결론지을 수 있다.

job(n+1)°] Aol] 포함되어 있지 않다고 가정하자. 이 시간 슬롯을 2에서 10002 +1)이 차지
하고 있다고 생각해보자. 만약 알고리즘이 job(n+1)\S 고려할 때 그 SKS 사용가능하다고
하면, 그 작업을 스케줄에 넣었을 것이다. 따라서 그 시간 SRS AQ] 어떤 2A jobli,)o]
차지했을 것이다. 만약 jobli,)o] Bol] 속한다면, 그 작업이 BoA] 차지하고 있는 어떤 SHO]
라도 AoA] 어떤 작업 10800)가 차지하고 있음이 틀림없다. 왜냐하면 그렇지 않은 경우 알고
리즘이 job(i,)S 그 슬롯에, 100(7+1)을 job(é,)2] 슬롯에 배치했을 것이기 때문이다. jobli,)
는 명백히 ]1000,)이나 job(n+ 1)과는 다르다. 만일 job(i,)7} Bo] 속해 있다면, 그 작업이 Bol]
서 차지하고 있는 어떤 시간 슬롯이라도 AOA] 어떤 작업 1080 )가 차지하고 있음이 틀림없
다. 왜냐하면, 그렇지 않은 경우 알고리즘이 jobli,)S 그 슬롯에, job(é,)-& jobli,)2] 슬롯에
배치했을 것이기 때문이다. jobi, <= 명백히 100(&6)나 1000,)이나 10007+ 1)과는 다르다. 이러
한 BAS 논리는 끝없이 되풀이할 수 있다. 스케줄들은 유한하므로, AME SOA BYE
속하지 않고 어떤 작업 jobli, Ik 궁극적으로 언젠가는 반드시 도달하게 된다. 그렇지 않으
BAS 2가 성립하게 되는데, 이는 알고리즘이 ]00(4+1)을 에 속해있는 작업으로 스케줄
에 포함시킬 수 있음을 의미한다. jobli,)S job(n+1)2] 슬롯에, job(i,)S 100(1,)의 슬롯에,
vey 1060,)를 1000,_,)의 슬롯에 배치하여 BS 수정할 수 있다. 효과적으로 Boll job(n+1)
을 10000)로 대치하였다. 작업들은 감소하지 않는 순서로 정렬되어 있으므로, 1006,)의 BARS
AAS job(n+1)9] 보상만큼 많다. 따라서 최소한 Bo] 속한 작업들의 총 보상만큼 많은 총


===== PAGE 187 =====
174     chapter 4 탐욕 알고리즘
보상을 가진 작업들의 집합이 존재한다. 그러나 그 집합은 처음 개의 작업에서 얻어진다.
따라서 귀납가정에 의하여 그 작업의 총 보상은 4에 속한 작업의 총 보상보다 많을 수 없다.
이는 4가 최적이라는 의미가 된다.

부록 Col] 나와 있는 ASA 집합 데이터구조 11으로 80160486(알고리즘 4.4)의 O(n lg m)

시간 프로시저를 만들 수 있다. 여기서 m2 7의 최소값이고, 7개 작업들에 대한 마감시
간의 최대값이다. 정렬하는데 걸리는 시간은 아직 ㅇ(02187)이므로, 전체 알고리즘은
O(n lg n)olth, 어떻게 수정하는지는 연습문제에서 다룬다.

@ 44 Fz 코드

보조저장장치의 용량이 계속 커지고 가격이 계속 싸지고 있음에도 불구하고, 필요한 저
장용량도 따라서 증가하기 때문에 저장장치의 공간은 계속 더 필요하다. 그러므로 파일
을 가능한 한 효율적으로 저장하는 방법을 찾는 것이 바람직하다. 데이터 압축(4368 com—
pression) 문제는 데이터 파일을 코드화(600000)하는 효율적인 방법을 찾는 것이다. 이제
허프만 SE (Huffman 0000)라고 하는 코드화 방식과 주어진 파일을 허프만 코드화하는
탐욕 알고리즘을 공부해보자.

데이터 파일은 통상적으로 이진코드001481” code) 표현한다. 각 문자는 코드워드
(code \070)라고 하는 유일한 이진 문자열로 표현한다. 길이가 WAS] 이진 BE (fixed—
length binary 0009)는 각 AHS 표현하는 비트0640)의 개수가 일정하다. 예를 들어, 문자
의 집합이 {a, b, 라고 하자. 이 경우 두 비트만으로 각 문자를 코드화 할 수 있다.
왜냐하면 두 비트로 네 가지 다른 코드워드를 만들 수 있는데, 사용하는 문자는 세 개뿐
이기 때문이다. 예컨대 코드화를 다음과 같이 하기로 했다고 하자.

a: 00          b: Ol           ¢: i
이 코드화 공식을 다음 파일에 적용하면
ababcbbbe                                                                       (4,1)
결과 코드는
000100011101010111

가 된다. 길이가 변하는 이진코드(781719016ㄱ16081 binary code)S 사용하면 공간을 |Z 사
용하는 효율적인 코드화 방식을 만들어낼 수 있다. 이 코드화 방식은 각 문자마다 표현하
는 HES 개수가 다르다. 위의 예제에서는 문장 중 하나를 0으로 코드화할 수 있다. ’b’
가 가장 빈번히 나오므로 '6를 0으로 코드화하는 게 가장 효율적일 것이다. 그러나 이
경우 를 '00'으로 코드화 할 수 없는데, 그렇게 하면 ‘a's 두개를 구별할 수 없기



===== PAGE 188 =====
@‥@0060000 0
44 oot 코드  175

때문이다. '@ 를 01's! 코드화 할 수도 없는데, 그렇게 하면 00] 나오는 경우 ‘v'ela '@'의
시작인지 뒤 숫자를 더 보지 않고는 구별할 수 없기 때문이다. 그러므로 다음과 같은 방
식으로 AEBS 수 있다.

afi 10          bi 0          Ci l            (4,2)
이 코드화 BAS 파일 4.1에 적용하면 결과 코드는 다음과 같다.
1001001100011

이 코드화 방식을 사용하면 137] 비트만으로 위 파일을 표현할 수 있는 반면, 이전 방식
으로는 18개 비트가 필요하다. 이진문자코드로 파일을 표현하는데 필요한 비트의 최소
개수라는 사실을 가지고, 이 코드화 방식이 최적이라고 밝히는 건 어렵지 않다.

최적 이진코드(00071 binary code) 문제는 주어진 파일에 있는 문자들을 이진코드로
표현하는데 필요한 비트의 개수가 최소가 되는 이진문자코드를 찾는 것이다. 먼저 전치

코드를 살펴보고 나서, 이 문제를 푸는 허프만의 알고리즘을 공부하자.

4.4.1 전치코드

길이가 변하는 이진코드의 특수 형태의 하나로 전치코드(68088 code)7} 있다. 전치코드
에서는 한 문자의 코드워드가 다른 BAS] 코드워드의 앞부분이 될 수 없다. 예를 들어,
01이 8 의 코드워드라면 011은 의 코드워드가 될 수 없다. 코드 4.2는 전치코드의 예이
다. 길이가 고정된 BSE 역시 전치코드라고 할 수 있다. 전치코드는 Yo] 코드문자로
구성된 이진트리로 표현 가능하다. 코드 420] 해당되는 이진트리는 그림 4.9와 같다.
전치코드의 AES 파일을 파스(68789)할 때 현재 파스하고 있는 지점의 앞부분을 미리
볼 필요가 없다는 것이다. 이는 트리를 보면 바로 명백해진다. BAS 시작하는 지점은
파일의 왼쪽 Al 번째 비트와 트리의 뿌리이다. 파일에서 한 비트씩 차례로 훌어가고, 0이
나오는지 16] 나오는지에 따라서 트리의 마디에서 왼쪽 또는 오른쪽으로 간다. Mo] 도달
하면 그 잎에 있는 문자를 취한다. 그리고 다시 뿌리로 돌아가서 다음 비트로부터 시작하
여 같은 절차를 되풀이한다.



===== PAGE 189 =====
@00060000 0
176   chapter 4 탐욕 알고리즘

© 예제 4.7    문자의 집합은 14, b,c de, f} 이고, 파일에 있는 문자의 빈도수는 표 4.1과 같다고 하자. 표
4.1에는 그 파일을 코드화하는데 사용 가능한 3가지 다른 코드도 나열하고 있다. 각 방법에 따라
서 소요된 비트수를 계산해보면 다음과 같다.
Bits(C1) =16(3) +5(3) +12(3) +17(3) +10(3) + 25(3) = 255
Bits (C2) =16(2) +5(5) +12(4) +17(3) +10(5) +25(1) = 231
Bits (C3) =16(2) +5(4) +12(3) +17(2) +10(4) +25(2) = 212

코드 C2E 길이가 고정된 SE 021보다 좋지만, (73(허프만)은 </2보다도 더 좋음을 알 수 있
다. 다음 절에서 보겠지만 C37} 최적이다. 코드 C22} (73에 해당되는 이진트리는 각각 그림
4.10(8)와 (b)2} 같다. 각 문자의 빈도수는 트리에 문자와 함께 표시되어 있다.

@ 표 4.1 동일한 파일에 대한 3종류 코드. cat 최적

문자         빈도수      1(길이 고정)        C2         63(허프만

a            16             000             10             00

b             5             001            11110           1110

@            12             010            1110            110

d            17             011            110             01

6            10             100            11111            1111

tf            25             101             0              10

0       1

1225

0       1

a:16
0       1
미베0
0       1
여12
0       1

(a)                b:5      e:10        (b)                    b:5      e:10
그림 4.10 예제 4.72) 코드 C20] 해당되는 이진문자코드는 (3)와 같은 반면, 코드 6#(허프만)는

(6)와 같다.

앞의 예제에서 볼 수 있듯이 임의의 코드에 해당하는 이진트리 2까 주어지고 파일을
코드화 하였을 때 차지하는 비트의 수는 다음과 같이 계산할 수 있다.


===== PAGE 190 =====
@06000000
44 oie 코드  177

bits (T)= 3 frequency (v;)depth(v;)                       (4,3)
i=1

여기서 {01 Vg, +) 0, } 는 파일에 있는 문자의 집합이고, frequency(v;)= v,7+ 파일
에 나타나는 횟수이고, depth(v,;)= 7에서 v,2] 깊이이다.

4.4.2 Smet 알고리즘
허프만은 최적 코드에 해당하는 이진트리를 구축하여 최적 이진문자코드를 만들어내는
탐욕 알고리즘을 개발하였다. 이 알고리즘이 만들어내는 코드를 허프만 코드라고 한다.
여기서는 허프만 알고리즘의 고수준 버전을 보여주겠지만, 트리를 구축하는 과정을 수
하기 때문에 다른 고수준 알고리즘보다는 더 자세히 표현한다. 먼저 타입 선언부터 공
해보자.

struct nodetype

{

tr

char symbol;       // ARE
int frequency ;      // 팍일에 있는 문자의 빈도수

nodetype* Jeft ;
nodetype* right;
Hi
여기서 우선순위 7] (priority queue) S 사용한다. 우선순위 대기열에서는 우선순
위가 가장 높은 요소가 항상 먼저 빠져나간다. 우선순위가 가장 높은 원소는 파일에서
빈도수가 가장 낮은 문자이다. 우선순위 대기열은 연결 리스트010560 184로 구현할 수
있지만, 힙02680/으로 구현하면 더 효율적이다(힙은 7.6절에서 설명한다). 허프만 알고리
즘은 다음과 같다.
n = 파일에서 문자의 개수 ;

우선순위 대기열 PQA) nodetype 레코드를 가리키는 포인터 n 7S 다음과 같이 배열
한다.
PQ? 각 포인터 pol 대해서,
2 -> symbol = 문자 ;
PD -> frequency = 문자의 빈도수 ;
2 -> left = p > right = NULL ;
우선순위는 빈도수에 좌우되는데, 낮은 빈도수가 높은 우선순위를 가진다.

for (i= 1; 7 <= 2-1; H+) {         // 해답 여부의 점검이 없다.
27622006(20, p);                     // 대신 7 = 2-1일 때 해답을 얻는다.
remove(PQ, q);                  // 선택절차


===== PAGE 191 =====
178   chapter 4 탐욕 알고리즘
r= new nodetype ;                  // 적절성 AAS 없다.
r-> lett = p;

© => wight = Gs
r-> frequency = p -> frequency + 0 -> frequency ;

insert( PQ,

}

return r;

© 예제 4.8

Di

remove(PQ, r

만약 우선순위 대기열을 힙으로 구현한다면, 초기화하는데 O(n) 시간이 걸린다. 더구
나 각 힙 연산은 00087) 시간이 걸린다. for-i 루프가 7ㅡ1번 반복되므로 이 알고리즘
을 실행하는데 총 ee i n) 시간이 걸린다.

다음에는 이          을 실행 예를 살펴보자.

문자의 집합은 14, b,c, d, 6, ./} 이고, 파일에 있는 문자의 빈도수는 표 4.1과 같다고 하자. 그림
4.1에 있는 일련의 그림들은 알고리즘에서 for-i 루프를 매번 반복실행하면서 구축된 트리 집
합이 변화하는 모습을 보여주고 있다. 이 THA 첫째 Wee 루프에 들어가기 전의 상태를
보여준다. 각 마디에 저장되어 있는 값은 그 UIA] frequency 필드의 값이다. 마지막 트리는
그림 4.1000)의 트리와 같다.

다음에는 이 알고리즘이 항상 최적 이진문자코드를 만들어내는지 증명해보자. 다음 보
조정리부터 시작하자.

| 보조정리 4.4
최적 이진전치코드에 해당되는 이진트리는 가득찬 트리(681 ㅠ66)이다. 즉, 잎이 아닌 마디는
모두 자식마디가 둘이다.
증명 : 연습문제로 남겨둔다.

더 진도 나가기 전, 용어를 몇 개 알아두자. 트리에서 두 마디의 부모마디가 같으면,
그 두 마디는 형제 마디(61011088)라고 한다. 트리 7'에서 뿌리가 vel 가지0678004란 뿌리
를 로 하는 하위트리를 의미한다. 이제 허프만 알고리즘이 최적임을 증명해보자.

> Bel 4.5

허프만의 알고리즘은 최적 이진코드를 만들어낸다.
증명 : 귀납법으로 증명한다. 즉, 1번째 단계에서 만들어진 트리집합은 최적 코드에 해당하는
이진트리에서의 가지들이라고 가정하고, (1+1)번째 단계에서 만들어진 트리집합도 최적 코
드에 해당하는 이진트리에서의 가지들임을 증명한다. 그리고 (/ㅡ1)번째 단계에서 만들어진
이진트리는 최적 코드에 해당한다고 결론짓는다.



===== PAGE 192 =====
44 ono 코드   179
b:5} Je:10) }o:12} Ja:16} |d:17] | f:25     012     a:16} |0:17| | f:25
0   1
b:5   e:10
(0)                 (1)

a:16] |d:17) | f:25                                    £:25

(2)                                                                           (3)
52
0                1            0                it
a:16         d:17] |f:25           27
0                1
co:12           15
0                ]
D5          e:10
b:5          e:10
(4)                                                                           (5)

그림 4.11 반도수가 표 4.1과 같은 파일에 대해서 허프만의 알고리즘에서 for—i 루프가 매번 반복
되면서 구축된 부분트리의 상태를 보여준다. A 번째 트리는 루프에 들어가기 MS 나타내주고
있다
A  ㆍ

귀납기초 : 명백히 0번째 단계에서 만들어진 하나짜리 마디의 집합은 최적 코드에 해당하는
이진트리에서의 가지들이다.

귀납가정 : 번째 단계에서 만들어진 트리집합은 최적 코드에 해당하는 이진트리에서의 가지
들이라고 가정한다. 그리고 그 트리를 7라고 한다.

귀납절차 : 허프만의 알고리즘의 (1+ 1)번째 단계에서 만들어진 트리들의 뿌리들을 와 라고
하자. 만약 7에서 와 가 형제 마디라면, 허프만의 알고리즘의 (+ 1)번째 단계에서 만들어
진 트리집합이 7에서 가지들이므로 증명이 완료된다.

그렇지 않으면, 는 THA 최소한 ?만큼 낮은 수준에 있다고 일반성을 잃지 않으면서 가정한



===== PAGE 193 =====
180

chapter 4 탐욕 알고리즘

다. 전과 마찬가지로 /76046700(0)는 *를 뿌리로 하는 가지들의 잎에 저장되어 있는 문자들

의 빈도수의 합이다. 보조정리 4.4에 따르면 uk 7에서 형제 마디 가 있다고 할 수 있다.

SS 허프만 알고리즘의 ?번째 단계 이후에 존재하는 트리들의 집합이라고 하자. 명백히 뿌리

가 인 에서 가지는 에 있는 트리 중 sala  그러한 트리 중 하나를 하위트리로 포함
하고 있다. SS 어떤 경우가 되든지, 뿌리가 vel 트리는 이 단계에서 허프만 알고리즘이 A
택하였기 때문에 다음 부등식이 성립한다.

frequency(w) = frequency(v)
더욱이 THAT 다음 부등식이 성립한다.
depth(w) > depth(v)
THA] 7와 wS 뿌리로 하는 가지의 HAS 서로 바꾸어 새로운 이진트리 7" 을 만들 수 있다.

이 상황은 그림 4.120] 묘사되어 있다. 식 (4.9)과 바로 위의 두개의 부등식으로부터 다음 식이
나옴을 이해는 것은 어렵지 않다.

bits (7) = bits (7) + [depth (w) — depth(v)]|[frequency(v) ㅡ7/7760060000(0)]
< bits( 7)
이는 To] 해당하는 코드가 최적이라는 뜻이다. 명백히 허프만의 알고리즘의 G+) Ha 단
계에서 만들어진 트리들의 집합은 7”에 있는 가지이다.

4.5 탐욕 알고리즘과 동적계획 알고리즘의 비교 : 배낭 채우기 문제

탐욕적인 방법과 동적계획법은 최적화 문제를 푸는 두 가지 방법이다. 둘 중 어떤 방법을
사용해도 문제를 풀 수 있다. 예를 들어, 단일출발점 최단경로 문제는 동적계획법(알고리
즘 3.9)으로도 풀었고 탐욕적인 방법(알고리즘 4.9)으로도 풀었다. 그러나 동적계획 알고
리즘은 모든 마디를 출발점으로 하여 최단경로를 구하는 해법으로, 단일출발점 문제의
해법으로는 과잉이다. 단일출발점에 대한 최단경로만을 구하는 경우라도 전체 배열 DS
구축하기 때문에 낭비가 심하다. 동적계획법으로는 O(n’) 시간에 BAS 푸는데 비해

58

그림 4.12 와 (를 뿌리로 하는 가지를 서로 바꾼


===== PAGE 194 =====
@‥0000000
4.5 탐욕 알고리즘과 동적계획 알고리즘의 비교 : 배낭 채우기 문제     181

A, 탐욕적인 방법으로는 O(n’) 시간에 풀 수 있다. 일반적으로 탐욕 알고리즘이 동적계
획법 알고리즘보다 더 간단하고 더 효율적이다.

반면에, 탐욕 알고리즘이 항상 최적의 해를 주는지를 증명하기는 보통 더 어렵다. 거스
ae 문제에서 보았듯이 탐욕적인 방법이 항상 최적의 해를 주지는 않는다. 임의의 탐욕
알고리즘이 항상 AA HS 주는지를 보여주기 위해서 증명이 필요한 반면, 그렇지 않
음을 보여주기 위해서는 반례(60406 example)7} 필요하다. 동적계획법의 경우에는 최
적의 원칙이 적용되는지만 확인하면 충분했다.

acs
da
of
re
Jo
Ne
peal
을
oy
ttlo
ary
고
에
ao
ot
에
이
그
30
와
.조
co)
ㅣ
만조
=
of
ay
Jo
ia)
je
=
of
=
mY,
의

채우기라고 하는 두 가지 아주 비슷한 문제를 살펴보자. 배낭 빈틈없이 채우기 문제를
완벽하게 푸는 탐욕 알고리즘은 만들 수 있지만 0-1 배낭 채우기 문제는 풀 수가 없다.

반면, O-1 배낭 채우기 문제는 동적계획법으로 완벽하게 풀 수 있다.

4.5.1 O-1 배낭 채우기 문제의 탐욕적인 해법

O-1 배낭 채우기 문제의 사례를 하나 살펴보자. 밤손님(도둑의 존칭!) 한 분이 보석가게
에 배낭을 메고 침입했다고 하자. FAI) 아이템의 총 무게가 배낭의 용량 WS 초과하면
배낭이 BojZlch, 각 아이템의 값어치와 무게는 알고 있다. 이 밤손님의 딜레마는 총 무
게가 WS 넘지 않으면서 아이템의 총 값어치가 최대가 되도록 아이템을 배낭에 담는
것이다. 이 문제를 0-1 배낭 채우기 문제(0-1 knapsack 2『0601600라고 한다. 이 문제는
다음과 같이 정식으로 기술할 수 있다.

아이템이 7개 있다고 가정하자. 그리고

9=1아이템,, 아이템, ..., 아이템, }
w; =아이템,의 무게

2, =아이템(의 값어치

11"=배낭의 용량

여기서 Wi. Dis We 양의 정수이다.
wu, < 를 만족하면서 >) pS 최대가 되는 9의 부분집합 AS 찾으
A

obey a, A                아이템,ㄷ
시오.

무작정으로 해답을 구하는 YAS 다음과 같다. nh 아이템의 모든 부분집합들 중에
A 총 무게가 WS 초과하는 것들을 버리고, 남은 것들 중에서 총 보상이 최대가 되는
것을 하나 선택하면 된다. 부록 Ao] 있는 예제 &.10에서 알 수 있듯이 아이템이 7H} 있는
집합은 부분집합이 "개 존재한다. 따라서 무작정 해법으로는 지수시간이 걸린다.

가장 쉬운 탐욕적인 전략은 가장 값어치가 높은 아이템을 먼저 채우는 것이다. 즉, 값
어치가 높은 순서로 채우는 것이다. 그러나 이 전략은 가장 값어치가 많이 나가는 아이템


===== PAGE 195 =====
182

chapter

4 탐욕 알고리즘
이 그 값어치에 비해서 무게가 많이 나가는 경우 좋지 않을 수 있다. 예를 들어, 아이템이
3개 있는데 첫째 아이템은 무게가 2588, 값어치가 10만원이고, 둘째와 셋째 아이템은 각
Zt 무게가 1068, 값어치가 9만원이라고 하자. 만약 배낭의 용량 1^가 30686이면, 최적해
가 18만원인데 비해서 이 탐욕적인 전략으로는 10만원어치 밖에 채우지 못할 것이다.

또 다른 탐욕적인 AS 가장 가벼운 아이템부터 SAE 것이다. 이 전략은 가벼운
아이템이 무게에 비해서 값어치가 별로 나가지 않는 경우 좋지 않다.

이 두 탐욕 알고리즘의 단점을 극복하기 위한 좀 더 복잡한 탐욕 알고리즘은 무게 당
값어치가 가장 높은 아이템을 우선 채우는 것이다. 즉, 무게 당 값어치가 큰 것부터 차례
로 아이템을 총 용량 WS 초과하지 않으면 배낭에 채운다. 이 방법은 그림 4.10에 그림
으로 설명한다. 그림을 보면 각 아이템의 무게와 값어치를 아이템별로 표시하고, We]
He 30으로 배낭에 표시하였다. 무게 당 값어치를 계산하면 다음과 같다.

아이템, : 50만원/5 = 10만원
아이템, : 60만원/10 = 6만원
아이템, : 140만원/20 = ?7만원
무게 당 값어치가 큰 것부터 차례로 나열하면 다음과 같다.
아이템, Orla, 아이템,

그림에서 볼 수 있듯이 이 탐욕적인 방법으로는 아이템,과 아이템,을 선택하게 되어
총 PAS 190만원이 되는 반면, 최적의 SHES 아이템,와 아이템,을 선택하여 총 수익이
200만원이 된다. 문제는 아이템,과 아이템,을 선택한 후 배낭에 558만큼의 빈 공간이 남
OF 있다는데, 아이템,는 108이어서 배낭에 넣을 수 없으므로 그만큼 공간이 남게 된다.
사실 더 복잡한 탐욕 알고리즘을 쓰더라도 0-1 배낭 채우기 문제는 탐욕적으로는 풀 수

없다.

5만원
남음
140만원
20만원 | 140만원
최대     20만원 | 140
30만원        만원
마유     :
60만원    20만원
te                           :
Stes    10만원                            10만원 | 60만원
ser |                     5만원 |50
=                               만원
아이템,    아이템,    아이템』     배낭    탐욕적인    최적의
해답     해답

그림 4.13 0-1 배낭 채우기 문제의 탐욕적인 해답과 최적의 해답


===== PAGE 196 =====
@‥0@00600000
45 탐욕 알고리즘과 동적계획 알고리즘의 비교 : 배낭 채우기 문제     183

4.5.2 배낭 빈틈없이 채우기 문제의 탐욕적인 접근방법

울 수 있다고 가정한다. 0-1 배낭 채우기 문제에서 아이템은 금괴나 은

고, 배낭 빈틈없이 채우기 문제에서 아이템은 금가루나 은가루가 든 자

된다. 그림 4.10의 아이템들을 다시 생각해보자. 탐욕적인 방법으로 무게

당 값어치가 많이 나가는 아이템을 순서대로 다시 선택하면 아이템,과 아이템,을 전과

마찬가지로 선택할 것이다. 그러나 58만큼 남은 공간은 아이템,의 108 중 518으로
채울 수 있다. 그러면 총 이익은 다음과 같이 계산할 수 있다.

50만원 + 140만원 + 5/10(60만원) = 2820만원

0-1 배낭 채우기 문제와는 달리 이 탐욕적인 방법으로 배낭 빈틈없이 채우기 문제
풀면 빈 공간이 절대 남지 않는다. 결과적으로 최적의 해답을 얻게 된다. 이를 SRS
]은 연습문제로 남겨눈다.

ful

fr

으
=

4.5.3 O-1 배낭 채우기 문제를 푸는 동적계획법

최적의 원칙이 적용된다고 증명할 수 있다면 동적계획범으로 0-1 배낭 채우기 문제를
풀 수 있다. AS 7개 아이템들 중에서 최적을 이루는 부분집합이라고 하자. 이때 4가
아이템 7을 포함하는 경우와 포함하지 않는 경우의 두 가지로 나눌 수 있다. 만약 4가
아이템 n-& 포함하고 있지 않다면 AL 처음 n— 174 아이템들 중에서 BAS 이루는
부분집합과 같다. 만약 4가 아이템 nS 포함하고 있다면 Ao] 속한 아이템들의 총 이익
은 총 무게가 1^- 0, 을 초과할 수 없다는 제약조건 하에서 AS n— 17H 중에서 아이템

들을 선택할 때 얻는 최적의 이익에다 /, 을 더한 것과 같다. 따라서 최적의 원칙이 적용

1
°:
aft

구한 결과는 다음과 같이 일반화할 수 있다. 1> 0과 w> 0인 경우 총 무게가
를 초과할 수 없다는 제약조건 하에서 처음 {개 아이템에서만 선택할 때 얻는 최적의
이익을 Plillw] eat 하면, 다음과 같은 식을 얻는다.

maximum (Pli—1][w], p,+ Pli-—1][w—w,]) ,

a

Piltel= {pea                             -w

최대 이익은 Pln|[WiSt 같다. 이 값은 이차원 배열 PS 사용하여 구할 수 있다. 이 배
열의 Yo} 인덱스는 0부터 이고, 열의 인덱스는 0부터 1까지이다. Plillw]] AS 사
용하여 순서대로 MA] 행 AS 계산한다. 101[1와 7[/110]은 0으로 놓는다. 실제 알
고리즘의 작성은 연습문제로 남겨둔다. 계산한 배열 엔트리의 개수가 다음과 같다는 사
실은 쉽게 알 수 있다.

nW ㅎㅎ O(nW)


===== PAGE 197 =====
@0@000000
184   chapter 4 탐욕 알고리즘

* 예제 4.9

4.5.4 O-1 배낭 채우기 BAS 푸는 동적계획법 알고리즘의 개선
계산한 배열 엔트리의 개수를 나타내는 식이 nol 대해서 일차라는 사실은 아이템의 개수
가 인 모든 예에 대해서 이 알고리즘이 효율적이라고 오해하게 할 수 있다. 그러나 이는
사실이 아니다. 그 식의 다른 항인 가 있고, nF} 『/사이에 상관관계가 없다. 그러므로
주어진 nol] 대해서 임의로 큰 WS 취하여 실행시간이 임의적으로 큰 예를 만들 수 있다.
예를 들어, W7 nlo] el 계산한 엔트리의 개수가 @(1×11!)가 된다. 만약 = 30이고
W= 20!이면 아무리 빠른 컴퓨터로 실행하더라도 수천 년 걸린다. nol 비해 까 극도
로 큰 경우 이 알고리즘은 부분집함을 모두 고려하는 무작정 알고리즘보다도 나쁘다.
이 알고리즘을 최악의 경우 계산한 엔트리의 개수가 ㅇ(2" 이 되도록 개선할 수 있다.
개선하면, 무작정 알고리즘보다 실행성능이 절대 뒤지지 않으면서 실행성능이 잘 나오는
BST] 종종 있다. 1과 WAP] 모든 에 대해서 iA Bol] 있는 엔트리는 계산할 필요
가 없다는 AALS 기초로 AAAS 시도한다. nA 행에서는 2[71| 14 만 계산하면 된다.
따라서 (7-1)째 행에서는 Pln)[WIS 계산하는데 필요한 엔트리만 계산하면 된다.
Pin|[WI= 다음과 같은 식으로 표현할 수 있다.
mazimum(P[n—1][W], p, + P[n—1][W—w,]), w, < WIA?
Poll = {pig ali                , w, > WA 경우

따라서 (n— 1) 행에서는 다음 두 엔트리만 필요하다.
Pln-1][W), Pln—-1][W-w,]

에서부터 뒤로 이 43S 계속하면 계산할 필요가 있는 엔트리를 결정할 수 있다. S,
iA] Vol 어떤 엔트리가 필요한 지 결정한 후에, 다음 사실을 가지고 (《- 1)째 Bo] 필요
한 엔트리를 Age}.

끼2][]는 끼2-1][1와 Pli—1][w—-wyS 가지고 계산한다
”=1이거나 w < 0이면 멈춘다. 필요한 엔트리를 결정한 후에 첫째 행부터 계산을 시
작한다. 이 방법을 예제를 가지고 자세히 숙지해보자.

그림 4.13과 같은 아이템들이 있고, 10= 30이라고 가정하자. 먼저 각 행에 필요한 엔트리를 결
정해보자.
행 8에 필요한 엔트리를 결정한다. 다음이 필요하다.

Pi3)[W) = 213]130]

행 20 필요한 엔트리를 결정한다.
2131130]을 계산하기 위해서 다음이 필요하다.
P{3 — 1)[30] = P{2}[30]>+P[3 — 1][30 -<081 = P[2][10]


===== PAGE 198 =====
0000000
4.5 탐욕 알고리즘과 동적계획 알고리즘의 비교 : 배낭 채우기 문제     185

행 lo] 필요한 엔트리를 결정한다.
꺼21130]을 계산하기 위해서 다음이 필요하다.
P(2—1][30] = P{1][30]>}P[2—1][30—w.; = 2011120]
2121110]을 계산하기 위해서 다음이 필요하다.
P(2—1)[10] = 211]110]과거2-1][10-“%8] = Pl1][10]
다음 이 계산을 수행한다.
행 1을 계산한다.
0 = ao 50ut + Pl0|[w—5]), w,=5<w 인 경우
[20191               , 0, =5 > 인 경우
_ |50만원, w, =5 < unl 경우
“na  , 0, =5 > 인 경우

r

따라서,
P{1][0]

P{i][10]

P{1][20]

]

0만원

50만

ll

rie

0
0     “|

504}
P({1}[30] =50만

He He

행 25 계산한다.

Pi2)[10] =  {rea  Pi1]{10], 60821 + Pli][o]) , w    ee <10°
P({1}{10]                             , W, =10>10 인
= 60만원

ㅇ

(2][30] = aa 60만원 + P[1][20]) ,      =10 ㄴ= 30
기1]130]                          ~ ~” 이
= 60만원+50만원 =110만원
행 8을 계산한다.
23110 a 0000 P(2][30], 1408191 +P[2][10]) , ws =20 < 30 인

(2][30]                      , w3 =20>30 인
= 140만원+60만원 = 200만원

원래 알고리즘으로는 (3)(30)=90 엔트리를 계산하는데 비해서 개선 알고리즘으로는 7
개 엔트리만 계산한다.

최악의 경우 이 개선 알고리즘이 얼마나 효율적인지를 알아보자. (n— 1) 행에서 최
대로 2'개 엔트리를 계산함을 주목하자. 따라서 계산하는 엔트리의 최대 총 개수는
과 같다.

1+24+27+ … +9" 1=9"-]


===== PAGE 199 =====
@0 @0 @
186     chapter 4 탐욕 알고리즘

미

이 등식은 부록 Ao} 예제 4.3의 의해서 얻는다. 다음의 경우 대략 a" Ho} 엔트리를
계산한다(이익의 값은 상관없다)는 사실을 증명하는 일은 연습문제로 남겨둔다.

0,= 2“ Laien), Wo

이 두 결과를 합하면 최악의 경우 계산하는 엔트리의 개수는 다음과 같다고 결론지을
있다.

+>

@(2")

지금까지 구한 시간복잡도는 모두 nO] 형식으로 표현하였다. /과 WS
로 시간복잡도를 표현할 수도 있다. 계산하는 엔트리의 개수가 O(n WAH 것은 이미
알고 있지만 개선된 알고리즘은 아마도 이 한계에 결코 도달하지 않을 것처럼 보일

모른다. 그러나 그렇지 않다. n= WH 1이고 모든 iol] 대해서 6, = 1이면, 계산하는 al
트리의 총 개수는 대략 다음과 같은데 증명은 연습문제로 남겨둔다.

n(n+1) _ (W+1)(n+1)

eet f=  5

첫째 등식은 부록 AS] 예제 ㅅ.1로 구하고, 둘째 등식은 이 경우 n= 11+1라는 사실에서
유추한다. 따라서 시간복잡도는 임의로 큰 7 과 『값까지 도달하여 최악의 경우 엔트리
의 개수는 다음과 같다.

이 두 결과를 합하면, 최악의 경우 계산하는 엔트리의 총 개수는 다음과 같다.
O(minimum(2™ nW))

이 알고리즘을 구현할 때 배열 전체를 쓸 필요는 없다. 대신, 필요한 엔트리만
된다. 전체 배열은 묵시적으로만 존재한다. 만약 알고리즘이 이런 식으로 구현되면 최
의 경우 데모리 사용량도 복잡도가 같다,

동적계획법 알고리즘을             한 식 Plillw]S 가지고 분할정복 알고리즘을
작성할 수 있다. 이 alse 최악의 경우 거산하는 엔트리의 AE 역시 6(0")이
된다. 동적계획범을 사용하여 얻는 주된 이점은 MAES nw 형태로 표현할 수 있다는
점이다. 분할정복법으로는 이런 식으로 복잡도를 표현할 수 없다. 복잡도의 표현의 차이
가 동적계획법과 분할정복법의 근본적인 차이점을 보여준다. 즉, 동적계획법은 같은 계
산을 두 번 이상 반복하지 않는다. nW 형식의 복잡도는 7에 배해서 『까 별로 크지

않은 경우 매우 PVE 있다.

외판원 문제의 경우와 마찬가지로, 최악 시간복잡도가 지수보다 좋은 0-1 배낭 채우기
qlee 채은 지킴이 아저 ofS GS -B 이니바 Tel AelSo] BrksaiCh S
명한 사람도 아무도 없다. 이러한 문제는 9장에서 집중적으로 다룬다.


===== PAGE 200 =====
4.1절
1. 탐욕적인 방법을 이용하면 항상 거스름돈 문제의 최적해를 구할 수 있음을 보이시오. 동전
의 액면금액은 ?> 0이고 2>0인   | oa    iQ} Dol] 대해서 D®, D', D?, … 22'이 된다고 가정
한다.
2. 프림 알고리즘(알고리즘 4.1)을 이용하여 다음 그래프의 최소비용 신장트리를 구하시오. 그
리고 수행되는 절차를 단계별로 보이시오.

32

          님

59 도 "고 4 ar 12

3. 다음 배열을 보고 아래 물음에 답하시오.
1 2 3 4 5 6

1] 0 | ©} 72} 50} 90] 35
2} ©] 71] 71} 70} 73} 75
3| 72} 70} 0 | ©] 77} 90
4| 50 | 73; ©] 0 | 60} 40
5| 90 | 75 | 77} 60} O | 80
6| 35                90} 40; 80 | 0

(@) 마디 v1 시작하여 프림 알고리즘을 적용하여 위 배열이 표현하는 그래프의 최소비
용 신장 트리를 찾으시오.

09) 최소비용 신장 트리를 이루는 이음선의 집합을 보이시오.

(0 최소비용 신장 트리의 비용은 얼마인가?

4. 하나 이상의 최소비용 신장트리를 가진 그래프를 하나 그리시오.
5. 프림 알고리즘(알고리즘 4.1을 구현하는 프로그램을 작성하고, 여러 가지 다른 그래프

가지고 성능을 측

=e

|

a

6. 가중치포함 비방향그래프가 연결되어 YEAS 검사하는 알고리즘을 프림 알고리즘(알고리


===== PAGE 201 =====
188

chapter 4

탐욕 알고리즘

즘 4.1을 수정하여 작성하시오. 수정한 알고리즘을 분석하고, 그 결과를 차수표기법을 사용
하여 표시하시오.

크루스칼 알고리즘(알고리즘 4.9)을 사용하여 연습문제 22] 그래프의 최소비용 신장트리를
구하시오. 그리고 수행되는 AAS 단계별로 보이시오.

크루스칼 알고리즘(알고리즘 4.9/을 구현하는 프로그램을 작성하고, 여러 가지 다른 그래프
를 가지고 성능을 측정해 보시오.

최소비용 신장트리에 사이클이 존재할 수 있다고 생각합니까? 그리고 왜 그런 답이 나오는
지를 설명하시오.

10. 컴퓨터 네트워크에서 어떤 두 컴퓨터도 서로 연결될 수 있다고 가정하자. 각 링크간의 추정
비용이 주어진 상태에서 알고리즘 4.1(프림 알고리즘)을 사용할지, 아니면 알고리즘 4.9(크
루스칼 알고리즘)를 사용할 지를 판정하시오. 그리고 왜 그런 Yo] 나오는지를 설명하시오.

11. 보조정리 4.8를 적용하여 정리 4.29] SYS 완성하시오.

4.2절

12. 다익스트라 알고리즘(알고리즘 4.9)을 사용하여 연습문제 3의 배열이 나타내는 그래프에서
마디 에서 다른 모든 마디로 가는 최단경로를 구하시오. 그리고 수행되는 절차를 단계별
로 보이시오.

13. 다익스트라 알고리즘(알고리즘 4.9)을 사용하여 연습문제 29] 그래프에서 마디 (에서 다른
모든 마디로 가는 최단경로를 구하시오. 그리고 수행되는 절차를 GABE 보이시오. 여
기서 각 비방향 이음선은 같은 가중치를 가진 두 개의 쌍방향 이음선을 나타낸다고 가정하
시오.

14. 다익스트라 알고리즘(알고리즘 4.9)을 구현하는 프로그램을 작성하고, 여러 가지 다른 그래
프를 가지고 성능을 측정해 보시오

15. 최단경로의 길이를 계산하도록 다익스트라 알고리즘(알고리즘 4.9)을 수정하시오. 수정한
알고리즘을 분석하고, 그 결과를 차수표기법을 사용하여 표시하시오.

16. 방향성 그래프에 사이클이 존재하는지 검사하는 알고리즘을 다익스트라 알고리즘(알고리즘
4.3% 수정하여 작성하시오. 수정한 알고리즘을 분석하고, 그 결과를 차수표기법을 사용하
여 표시하시오.

17. 다익스트라 알고리즘(알고리즘 4.9)을 음수의 가중치를 가진 그래프의 최단경로를 구하는
데 사용할 수 있는가? 그리고 왜 그런 답이 나오는지를 설명하시오.

18. 귀납법을 사용하여 다익스트라 알고리즘(알고리즘 4.9)의 정확성을 증명하시오.

4.3절

19. 다음 작업과 작업시간을 가지고, 4.8.1절에 있는 알고리즘을 사용하여 시스템에서 소요된

총 시간을 최소화하시오.


===== PAGE 202 =====
20.

1.

22.

23.

24.
25.

작업          작업시간
i                              tf
2                              3
3                            10
4                             5

4.3.1절의 알고리즘을 구현하는 프로그램을 작성하고, 연습문제 190] 나오는 예를 가지고
프로그램을 실행시켜 보시오.

단일작업 스케줄 짜기 BAS 4.3.1절의 다중작업 스케줄 짜기 문제로 일반화하여 알고리즘
을 작성하시오. 작성한 알고리즘을 분석하고, 그 결과를 차수표기법을 사용하여 표시하시

오.

다음 작업, 마감시간, 보상을 가지고, 마감시간이 있는 스케줄 짜기 알고리즘(알고리즘 4.4)

을 사용하여 총 보상을 최대화하시오.

작업             마감시간            보상
1                   2                  40
2                   4                  15
3                   3                  60
4                   2                  20
5                   3                  10
6                   1                  45
7                   1                  55

마감시간이 있는 스케줄 짜기 알고리즘(알고리즘 4.4)의 6416046 프로시저를 생각해보자.
dS 7개 작업의 마감시간 중 최대값이라고 하자. 마감시간을 넘기지는 않으면서 되도록 작
을 스케줄에 늦게 편성하도록 알고리즘을 수정하시오. 먼저 정수 0부터 0까지를 각각 포
함하도록 4+1개의 ABA 집합을 초기화한다. 그리고 small ($)= 집합 에서 가장 작은
멤버를 나타내도록 한다. 작업을 스케줄할 때 가장 작은 마감시간을 포함한 집합 6와 그
작업 7을 찾는다. 만약 small(S) = 0이면, 그 작업은 제거한다. 그렇지 않으면 small(S)
시간에 그 작업을 스케줄하고, SS} small(S) -1을 포함한 집합을 합친다. 부록 (의 서로
소 집합 데이터구조 IS 사용한다고 가정하고, 이 알고리즘이 O(nlgm) YS 보이시오.
여기서 은 0와 7 중 최소값이다.
연습문제 21에서 만든 알고리즘을 구현하는 프로그램을 작성하시오.

길이가 각각 Ly, ly, …, 《,인 개 파일을 테이프에 저장하는데 걸리는 평균시간을 최소화하
려고 한다고 005 년 파일 *를 요청할 확률이 2,이면, ky, ky, … 의 순서로 이 파
일들을 로드(1080)하는 기대접근시간(6600006060 access time) 다음 식으로 표시한다.

Taverage =    이 | Pry 거  |

여기서 상수 CE 테입 드라이버의 Seo} 기록밀도 같은 파라미터를 나타낸다.


===== PAGE 203 =====
190

chapter 4 탐욕 알고리즘

(8) 기대접근시간이 최소가 되도록 보장하기 위해서 탐욕적인 방법으로 이 파일들을 어떤
순서로 저장해야 하는가?

06) 파일을 저장하는 알고리즘을 작성하고, 작성한 알고리즘을 분석하고, 그 결과를 차수표
기법을 사용하여 표시하시오.

4.43
26.  a                                       있는 글자들에 대한 최적 이진전치코드를 구축하
시오.
글자 : A B 1 08 X 2
빈도수 : 12 7 18 10 9 5 8
27. 허프만의 알고리즘을 사용하여 다음 표에 있는 글자들에 대한 최적 이진전치코드를 구축하
시오.

Ht : 6    e    i    r    s    t     x
Wee: O11 0,22 0,16 012 015 0,10  0,14
28. 연습문제 262] 이진코드를 사용하여 Z 비트 BASS 복코드화하시오
(3) 01100010101010
(b) 1000100001010
(c) 11100100111101
(d) 1000010011100

29. 연습문제 279] 이진코드를 사용하여 각 워드를 코드화하시오.
(a) rise
(b) exit
(c) text
(d) exercise
30. a, b,c, d, eo] 대한 코드가 다음과 같이 주어졌다고 하자.
000, 001, 61101, 01210, 60281
여기서 x, y, ze 0 또는 1이다. 주어진 코드가 전치코드가 되도록 2, y, eS 결정하시오.
31. 허프만의 알고리즘을 구현하고, 연습문제 26과 279) 예제로 실행해보시오.
32. 최적 이진전치코드에 해당하는 이진트리가 가득 차야 함을 보여라. 가득 찬 이진트리(001
binary tree)@ 모든 마디가 잎이거나 자식마디를 두 개 가진 이진트리이다.
33. 최적 이진전치코드에서 문자가 빈도수가 증가하지 않는 순으로 정렬되어 있다면, 코드워드
길이는 감소하지 않는 순으로 되어 있음을 증명하시오.
34. 이진전치코드에 해당하는 이진트리가 있을 때 모든 문자들에 대한 코드워드를 결정하는 알
고리즘을 작성하라. 작성한 알고리즘의 시간복잡도를 결정하시오.
4.5절
35. O-1 배낭 채우기 BAS 푸는 SAAS



===== PAGE 204 =====
@0000000
연습문제   191

30. 7개 키가 있을 때 나올 확률이 가장 높은 IS 46),를 뿌리0001에 위치시키고, Key,,
Keys, Key, Key, 1, Key,» Key, S& 각각 왼쪽과 오른쪽 부분트리에 같은
방법을 사용하여 재귀적으로 구축하는 최적이진검색트리(6001081 binary search tree)S 탐
욕적인 방법을 사용하여 구축하시오.

(a) 키는 이미 정렬되어 있다고 가정하면, 이 방법의 최악의 경우 시간복잡도는? 그리고 왜
그런 답이 나오는지를 설명하시오.
00) 이 탐욕적인 방법이 항상 최적이진검색트리를 구축하지 못함을 aS 들어 보이시오.

37. 7명의 작업자를 7개 작업에 배치했다고 가정하자. CS 째 작업자를 7째 작업에 배치하
는 비용이라고 하자. 작업자 7명을 7개 작업에 모두 배치하는 총비용을 최소화하는 배치를
찾는 알고리즘을 탐욕적인 방법을 사용하여 작성하시오. 작성한 알고리즘을 분석하고, 그
결과를 차수표기법을 사용하여 표시하시오.

38. 연습문제 87S 푸는 알고리즘을 동적계획법를 사용하여 작성하시오. 작성한 알고리즘을
석하고, 그 결과를 차수표기법을 사용하여 표시하시오.

Ac

39. 개 파일을 BY (merge)SHEG] 레코드 이동의 횟수를 최소화하는 알고리즘을 탐욕적인 방
WS 사용하여 작성하시오. 쌍방합병패턴(60\0-\8》” merge pattern: 한 번 합병하는 동안 두
파일이 합병됨)을 사용하시오. 작성한 알고리즘을 분석하고, 그 결과를 차수표기법을 사용

하여 표시하시오.

40. 연습문제 39을 푸는 알고리즘을 동적계획법을 사용하여 작성하시오. 작성한 알고리즘을
석하고, 그 결과를 차수표기법을 사용하여 표시하시오.

41. 배낭 빈틈없이 채우기 문제를 푸는 탐욕적인 방법이 최적의 해를 만들어 YS 증명하시오.

는 개선한 동적계획법 알고리즘으로 최악의 경우 계산하는 엔트

하시오. "=" -8와 1 <i <n] 범위에서 w, =" 인 예

ㅁ
Ac

42. 0-1 배낭 채우기 문제를
리의 개수가 22") YS
를 고려하여 증명하시오.

겨

ol
of

43. 0-1 배낭 채우기 문제를 푸는 개선한 동적계획법 알고리즘에서 n= W+ 1이고 BE ;에 대
해서 8, = 1일 때 계산하는 엔트리의 총 개수는 대략 (+ 1) ×(+1)/3가 됨을 증명하시
oO

추가적인 연습문제

44. 미국의 동전 시스템을 사용하고 각 동전 중 최소한 SYS 제외시킨 상태에서 거스름돈 문
제를 탐욕적인 방법으로 풀면 항상 최적의 해가 나오지 않음을 반례를 통하여 보이시오.

45. 완전그래프(60001 graph: 모든 마디 간에 이음선이 존재하는 그래프)가 7" "개의 신장
EQS 가짐을 증명하시오. 여기서 7은 그래프에서 마디의 개수이다.

46. 외판원 문제를 푸는 알고리즘을 탐욕적인 방법을 사용하여 작성하시오. 작성한 알고리즘이

항상 최소길이 여행경로를 찾지 못함을 보이시오.

47. 연습문제 212] 다중작업 스케줄 짜기 BAS 푸는 알고리즘이 항상 최적의 스케줄을 찾지
KGS 증명하시오.



===== PAGE 205 =====
192    chapter 4 탐욕 알고리즘

48.
49.

50.

o

acu}

프만 트리를 구축하지 않고, 주어진 문자의 집합에 대한 허프만 코드를 생성하라.

}프만의 알고리즘을 3진 WE (ternary 0000)로 일반화하고, 그 알고리즘이 최적의 3진 코
만들어 냄을 증명하라.

문자가 빈도수로 정렬되어 있다면 허프만 트리가 1차시간에 구축될 수 있음을 보여라.

쓰ㅁ그

에
Hl

\n
aul |

md



===== PAGE 206 =====
여    국에 유명한 햄프튼 궁정0380060ㅁ Court 『81806/의 미로에서 출구를 찾아 나가

O 려다보면 막힌 곳이 나올 때까지 무작정 찾아가 보는 수밖에 없을 것이다. 막힌
곳에 도달하면 갈래가 있는 곳까지 되돌아가서 다른 쪽으로 가봐야 한다. 미로 퍼즐을
해본 사람이면 누구나 막힌 곳에 도달하여 당황해본 경험이 있을 것이다. 막힌 곳으로
가는 경로가 표시되어 있다면 이 퍼즐은 엄청나게 쉬워질 것이다. 만약 갈림길이 나오는
곳마다 그 표시되어 있다면 출구를 찾는데 엄청나게 시간 절약을 할 수 있을 것이다. 왜
냐하면 그 표시 뒤에 있는 경로는 무시해도 되기 때문이다. 즉, 막힌 곳을 따라가는 Bs
고는 없다는 의미이다. 미로 퍼즐에는 대부분 그러한 표시가 없다. 그러나 이 장에서 배
울 되추적 알고리즘은 그 표시를 이용한다.

Al (backtracking) = 0-1 배낭 채우기 문제와 같은 부류의 문제를 푸는데 아주 유
용하게 쓴다. 배낭의 용량이 그리 크지 않으면 효율적인 동적계획 알고리즘을 4.4.8절에
A 공부하긴 했지만 이 알고리즘도 최악의 경우에는 역시 지수시간이다. 0-1 배낭 채우
기 문제는 9장에서 공부하는 문제의 부류에 속한다. 이러한 부류의 문제들에 대해서 최
Sf 시간복잡도가 지수보다 좋은 알고리즘을 찾은 사람이 아직 아무도 없을 뿐 아니라 그



===== PAGE 207 =====
194

chapter 5 되추적

rr (쏘

알고리즘이 불가능하다고 증명한 사람도 아무도 없다. 0-1 배낭 채우기 BAS 다루
한 가지 방법은 실제 해답후보의 부분집합들을 모두 생성하면 되지만, 이는 마치 미로
에서 모든 경로를 막힌 Zo] 나올 때까지 무작정 따라가 보는 것과 마찬가지이다. 4.4.1
절에서 공부했듯이 이 부분집합의 개수는 2"0] 되므로 no] 작은 경우에만 통한다. 그러
나 부분집합을 생성하면서 생성할 필요가 없는 것들을 알 수 있다면 불필요한 노력을 절
감할 수 있을 것이다. 이게 바로 되추적 알고리즘이 하는 일이다. 0-1 배낭 채우기 문제
와 같은 부류의 문제를 푸는 되추적 알고리즘은 그래도 최악의 경우 지수시간이다(또는
그보다도 더 나쁘다). 그러나 되추적 알고리즘은 모든 경우 효율적이지는 않지만 많은
경우 효율적일 수 있기 때문에 유용하게 쓰인다. 5.7절에서 다시 01 배낭 채우기 SAS
되추적 방식으로 Zo} 예정이다. 그 전에 5.1절에서 간단한 사례를 가지고 되추적을
소개하고, 그 후 몇 가지 BAS 되추적으로 푸는 방법을 알아본다.

5.1 되추적 기술

되추적은 임의의 집합(600에서 주어진 기준(@ㅠ16000)대로 원소의 순서(664046006)를 선
택하는 문제를 푸는데 사용한다. 되추적의 전형적인 사례는 서양장기(01688)의 n-4S
말 문제(, -@46608 Problem)°]th, 이 문제의 BHE nxn 크기의 서양 장기판에 서로
잡아먹히지 않도록 7개의 여왕말을 위치시키는 것이다. 즉, 어떤 여왕말끼리도 같은 행
이나 열이나, 대각선상에 위치할 수 없다. 이 문제에서 순서는 여왕말을 둘 7개의 각각
다른 위치이고, 집합은 서양 장기판에서 BES 둘 수 있는 “개의 위치들이 되고, 기준은
어떤 여왕말도 서로 잡아먹히지 말아야 한다는 것이다. 7-여왕말 문제는 표준 서양 장기
판의 크기인 n= 8인 BPS 일반화 한 것이다. 편의상 7=4인 경우 사례를 가지고 되
추적 방법을 설명한다.

되추적은 트리(여기서 트리는 뿌리가 있는 트리를 말한다)의 변형된 깊이우선검
(depth-first 868700)이다. 더 진도를 나가기 전에 깊이우선검색을 복습해보자. 깊이
선검색은 일반 그래프를 대상으로도 정의할 수 있지만, 여기
한하기 때문에 단순히 트리의 검색만 설명한다. 부모마디우선(0ㅠ60700) 트리검색은 트
리의 깊이우선검색이다. 이는 뿌리마디ㅠ001)를 먼저 방문한 후, 그 뿌리마디ㅁ006/의 후
손들을 모두 방문한다. 비록 일반적으로 깊이우선검색이 자식마디들을 어떤 특정 순서에
따라서 방문하도록 하는 것은 아니지만, 이 장 예제에서는 왼쪽에서 오른쪽의 순서로 마
디의 자식들을 방문하도록 한다.

그림 5.1을 보면 이런 방식으로 트리의 깊이우선검색을 수행하는 예를 보여준다. 그림
에서 마디들은 방문하는 순서대로 번호가 AA 있다. 깊이우선검색에서 방문경로는 더
이상 갈 수 없는 마디까지 깊이로 내려감을 명심하자. 마지막 마디에서 다시 방문하지

주   J
1
4
Dn)
rlo
|!
4 aus
om
a)
BQ;
m + 4o 쏘



===== PAGE 208 =====
0 00000 0
5.1 되추적 기술   195

그림 5.1 HOIPNAA 순서에 따라 마디에 번호가 매겨진 트리

않은 자식마디가 있는 마디로 되돌아가고, 거기서 다시 내려갈 수 있는 깊이까지 내려간다.

깊이우선검색을 하는 간단한 재귀 알고리즘이 있다. 지금은 트리의 부모마디 우선횡단
(preorder \ㅠ876789])에만 관심이 있기 때문에 이것만 중점적으로 수행하도록 알고리즘을
작성하였다. 이 프로시저는 트리의 뿌리마디를 파라미터로 전달하여 호출한다.

void depth_first_tree_search (node v)

{

node u;
visit v;
for (each child wu of v)
depth_first_tree_search (u);
}

이 범용 알고리즘은 자식마디를 방문하는 순서에 대해서는 언급하지 않았다. 그러나
앞에서 말했듯이 왼쪽에서 오른쪽으로 방문한다.
=49 때 /-여왕말 문제를 되추적 기술로 푸는 방법을 설명해보자. 4×4 서양 장
기판에 4개의 여왕말을 서로 잡아먹히지 않게 두어야 한다. 같은 행에 두 말을 놓을 수
없다는 AMIS 가지고 바로 BAS 간단하게 만들 수 있다. 이제 각 여왕말을 다른 행에
놓고 각 여왕말이 어떤 열에 놓이면 해답이 되는지 검사해 보면 된다. 각 여왕말은 4개의
열 중에서 한 곳에 놓을 수 있기 때문에 BYE (candidate 80141100)는 43× 4 × 4 × 4 =
256 개가 존재한다.
첫째 여왕말(행 1에 있는 여왕말)에 해당하는 SS 트리의 +A(level) 1에 있는 마디에
저장하고(뿌리는 수준 ONS 상기하라), 둘째 여왕말(행 2에 있는 여왕말)에 해당하는 열
은 트리의 (level) 20] 있는 마디에 저장하고, 등등 이런 식으로 트리를 구축하여 해
답후보를 만들 수 있다. 뿌리에서 잎1680)까지 경로는 해답후보가 된다(트리에서 잎은



===== PAGE 209 =====
196

chapter 5 되추적

그림 5.2 n=42 때 ”-여왕말 문제에 대한 상태공간트리의 일부분. 각 마디에서 튜플 <, P=
8번째 행에 있는 여왕말이 7번째 열에 USS 의미한다. 뿌리마디에서 잎까지의 각 경로가 해답후
보가 된다.

|의

자식이 없는 마디임을 상기하라). 이 트리를 상태공간트리(66866 space ㅁ66)라고 한다.
그림 5.2를 보면 상태공간트리의 일부를 보여준다. 전체 트리는 잎의 개수가 256개이고,
Zt 잎이 해답후보를 나타낸다. 순서쌍(6806060 pair) <i, 7>가 각 마디에 저장되어 있음
을 눈여겨보자. 이 순서쌍은 번째 Bo] 있는 여왕말이 7번째 열에 WSS 의미한다.

해답을 구하기 위해서 각 해답후보(뿌리에서 잎까지의 각 경로)를 왼쪽 끝에 있는 경로
부터 순서대로 검사한다. 처음 검사하는 몇몇 경로는 다음과 같다.

Ki Db, 2 5, <8, 2, 4 DI
[d, D, 2 D, @, D, 4, 2]
Ld, Db, 2 D, 9, 12, 4, 3]
[d, >, @ D, @, D, 4, 4]
[d, D, 2 D, @, 2, 4, DI

마디의 자식들을 왼쪽에서 오른쪽으로 방문하면서 깊이우선검색에 따라서 각 마디를 방
문한다. 상태공간트리의 단순 깊이우선검색은 막힌 Fo] 도달할 때까지 미로의 모든 경
로를 모두 가보는 것과 같다. 중간에 아무런 정도도 이용하지 않는다. 도움이 될 만한
정보가 있으면 그 정보를 이용하여 검색을 더 효율적으로 수행할 수도 있다. 예를 들

그림 5.868에서 설명한 대로, 어떤 두 여왕말도 같은 열에 놓을 수 없다. 그러므로 그림
5.8에서 <, D7} 들어있는 마디에서 뻔어나가는 전체가지를 포함하고 있는 BRL 구축


===== PAGE 210 =====
5.1 되추적 기술      197
(a)
그림 5.3 첫째 여왕말을            :               S 1(3)이나 S 2(06)에 둘 수 없음을 보여주는

그림

하고 검사할 필요가 없다(그 당시 이미 여왕말 1을 열 1에 놓았기 때문에 여왕말 2를 거기
에 놓을 수 없다). 이 HALE 이 마디로부터 뻔어나가면 해답이 없다는 사실을 알려준다.
비슷하게, 그림 5.30)에서 설명한 대로 어떤 두 여왕말도 같은 대각선에 놓을 수 없다.
그러므로 그림 5.24] <2, 2>가 들어있는 마디에서 뻔어나가는 전체가지를 포함하고 있
는 경로는 구축하고 검사할 필요가 없다.

내려 가봐야 해답이 없는 마디를 만나는 순간, 그 마디의 검색을 중단하고 그 마디의
부모마디로 돌아가서 다른 자식마디의 검색을 계속하는 과정이 되추적이다. 해답이 될
가능성이 없는 마디를 유망하지 않다(ㅁ00ㅁㅁ『0ㅁ18108)고 한다. 그렇지 않으면 유망하다
(200008108)고 한다. 요약해 보면 되추적은 상태공간트리를 깊이우선검색하여 각 마디가
유망한지를 검사하고, 만약 유망하지 않으면 그 마디의 부모마디로 되추적한다. 이 절차
를 상태공간트리를 가지친다(6040108)고 하고, 유망한 마디만으로 구성된 부분트리를 가
상태공간트리(00040600 state space 1ㅠ66)라고 한다. 되추적 방법의 일반적인 알고리
다음과 같다.

void checknode (node vy)

{

node uw;

x
5

:

if (promising(v))
if (there is a solution at v)
write the solution ;
else
for (each child w of v)
checknode( u);

상태공간트리의 뿌리마디는 호출할 때 파라미터로 640044006에 전달된다. 마디를 방문

하면 일단 그 마디가 유망한지 먼저 점검한다. 만약 그 마디가 유망하고 그 마디에 해답
이 있으면, 해답을 프린트한다. 유망한 마디에 해답이 아직 없으면, 그 마디의 자식마디


===== PAGE 211 =====
@0@00000 0
198   chapter 5 되추적

© 예제 51

를 방문한다. 유망함수(670018108 『400000)는 되추적의 응용에 따라 다르게 설계한다.
되추적 알고리즘은 마디가 유망하고 그 마디에 해답이 없는 경우에만 그 마디의 자식마
US 방문하는 AS 제외하고는 깊이우선검색과 같다(』-여왕말 문제를 푸는 알고리즘
the 달리, 어떤 되추적 알고리즘에서는 해답을 상태공간트리의 잎에 도달하기 전에 찾
을 수도 있다). 되추적 2HAAS backtrack 대신 checknodet}31 불렀는데, 그 이유는
프로시저를 호출할 때는 되추적이 일어나지 않기 때문이다. 대신 마디가 유망하지 않아

서 그 부모마디의 다음 자식마디로 넘어갈 때 되추적이 일어난다. 재귀 알고리즘을 프로
그램으로 구현하면 24 2]2E (activation records) 스택에서 유망하지 않은 마디에 관련
된 활성레코드를 뽑아내어 되추적을 달성한다.

다음 되추적을 사용하여 7=4일 때 -여왕말 문제의 해답을 구해보자.

유망함수 promisinge 되추적의 응용에 따라 다르다. /-여왕말 문제에서 어떤 마디와 그 마디
조상마디들이 여왕말을 같은 열이나 대각선에 두면, 유망함수는 586186를 넘겨주어야 한다. 그
림 5.4를 보면 되추적을 사용하여 7=4인 문제를 풀 때 생성되는 가지친 상태공간트리의 한 부
분이 나와 있다. 첫째 해답을 찾기 위해서 검사하는 마디만 보여주고 있다. 그림 5.5에는 실제
서양 장기판을 보여준다. 그림 5.4에서 XB 표시된 마디는 유망하지 않은 마디를 나타낸다. 비
숫하게 그림 5.5에도 유망하지 않은 위치는 XH 표시되어 있다. 그림 5.44] 음영 처리된 마디
는 첫째 해답이 발견된 마디이다. 되추적에 의해서 이루어진 BAS 추적해 보면 다음과 같다.

°

ㅁ

x  x

그림 5.4 되추적을 사용하여 7=4인 SAS 풀 때 생성되는
째 해답을 찾기 위해서 검사하는 마디만 보여줌. 찾은 해답은 SS A
않은 마디는 ×로 표시되어 있다.

그
ra
ㅁ2
al
Ss
30
(기
30
0므
Olt


===== PAGE 212 =====
@‥6@00000 0
5.1 되추적 기술   199

마디는 그 마디에 저장되어 있는 순서쌍으로 표현한다. 같은 순서쌍을 가진 마디가 여러 개 있지

만, 그림 5.4에 있는 트리의 횡단을 추적해 보면 어떤 마디를 의미하는지 금방 알 수 있다.
(a) <1, D& 유망하다         {왜냐하면 여왕말 10] 두는 첫째 말이기 때문이다.}
00) <2, DS 유망하지 않다.    {USHA 여왕말 10] 열 1에 있기 때문이다.}
<2, DE 유망하지 않다.    {왜냐하면 여왕말 10] 왼쪽 대각선에 있기 때문이다.}
<2, 3 유망하다.
(0 8, 은 유망하지 않다.     {왜냐하면 여왕말 1이 열 1에 있기 때문이다.}
<3, DE 유망하지 않다.     {왜냐하면 여왕말 2가 오른쪽 대각선에 있기 때문이다.}
<3, 8>은 유망하지 않다.     {왜냐하면 여왕말 2가 열 3에 있기 때문이다.}
                   <3, 4>은 유망하지 않다.     {왜냐하면 여왕말 2가 왼쪽 대각선에 있기 때문이다.}
(0) <1, 로 되추적

bea

(a)                                           (b)                                           (c)                                           (0)

De) [pene
poe

(e)                                           (f)                                           (g)                                           (h)

i   1
| 16

그림 5.5 되추적을 사용하여 7=4인 문제를 풀 때 시도해 본 실제 서양 장기판에서의 위치. 유망
하지 않은 위치는 각각 ×로 표시.

=>
=
a


===== PAGE 213 =====
@0@00000 0
200   chapter 5 되추적

2, Di 유망하다.
(6) 3, 은 유망하지 않다.     {왜냐하면 여왕말 1이 열 tol] 있기 때문이다.}
<3, 2>는 유망하다.         {<3, 2S 둘째 검사하고 있다.}
0) <4, 은 유망하지 않다     {왜냐하면 여왕말 1이 열 1에 있기 때문이다}
<4, 2>는 유망하지 않다     {왜냐하면 여왕말 30] 열 2에 있기 때문이다}
4, D2 유망하지 않다     {왜냐하면 여왕말 30] 왼쪽 대각선에 있기 때문이다.}
4, D2 유망하지 않다.     {왜냐하면 여왕말 2가 열 4에 있기 때문이다.}
(g) <2, OS 되추적
3, 32 유망하지 않다.     {왜냐하면 여왕말 2가 오른쪽 대각선에 있기 때문이다.}
<3, DE 유망하지 않다.     {왜냐하면 여왕말 2가 열 4에 있기 때문이다}

=
ap
w~
raw
80
&

DS 유망하지 않다.  |왜냐하면 여왕말 1이 오른쪽 대각선에 있기 때문이다}
co, 는 유망하지 않다. !왜냐하면 여왕말 1이 열 에 있기 때문이다:
2, 8>은 유망하지 않다. {왜냐하면 여왕말 10] 왼쪽 대각선에 있기 때문이다.]
(2, 은 유망하다.
0) @, DS 유망하다.         (3, DS 셋째 검사하고 ach)
09 <4, DS 유망하지 않다. (왜냐하면 여왕말 3이 열 1에 있기 때문이다.|
(4, DE 유망하지 않다. {왜냐하면 여왕말 10] 열 294] 있기 때문이다.}
(4, 3-2 유망하다.
이 시점에서 첫째 해답을 찾았다. 해답은 그림 5.500에 나와 있고, 찾은 마디는 그림 5.4에 음
처리되어 있다.

되추적 알고리즘이 트리를 실제로 구축할 필요는 없다. 대신, 조사 중인 해당 가지00ㅠ8ㅁ004
의 값만 알고 있으면 된다. 되추적 알고리즘을 일반적으로 구현하는 방식이다. 트리를
실질적으로 구축하지는 않으므로, 상태공간트리가 알고리즘에서 묵시적으로(20010)
존재한다고 말한다.

그림 5.4에서 마디를 세어보면 해답을 찾을 때까지 되추적 알고리즘이 27개의 마디를
검사했음을 알 수 있다. 상태공간트리를 되추적 없이 깊이우선검색하여 같은 해답을 찾
는데 155개의 마디를 검사하는 작업은 연습문제로 ALES 하자.

날카로운 ES 가진 독자는 일반적인 되추적 알고리즘(4160890008/에 비효율적인 부분
이 USS 이미 topWS 수 있다. 즉, 마디를 프로시저에 전달한 후 마디의 유망여부를
점검한다. 이는 활성레코드 스택에 유망하지 않는 마디의 활성레코드를 불필요하게 쌓아
놓음을 뜻한다. 마디를 전달하기 =  마디희 유망성을 점검하면 이 비효율성을 제거할
수 있다. 이를 적용시킨 일반 되추적 알고리즘은 다음과 같다.

void expand (node v)

{


===== PAGE 214 =====
000000 0
5.2 2-82 문제   201

node u;
for (each child uw of v)

if (promising{u))
if (there is a solution at 2)
write the solution ;
else
expand (u);
}

고리즘에 파라미터로 전달된 마디는 역시 뿌리마디이다. 이 알고리즘을 6027640라고
하는 이유는 유망한 마디를 확장(660800/할 때 이 프로시저를 호출하기 때문이다. 이 알
즘을 프로그램으로 구현하면 활성레코드 스택에 유망하지 않은 마디의 활성레코드
를 쌓아놓지 않고 그 유망하지 않은 마디에서 되추적한다.

앞으로 이 장에서 알고리즘을 AVS 때 첫째 Gate] FS (checknode)-& 사용한다. 왜냐
하면 그 방식으로 되추적을 설명하면 훨씬 더 이해하기 쉽기 때문이다. 그 oP check
node®| 1회 실행이 마디를 한 번 방문하면서 수행하는 절차와 일치하기 때문이다. 즉
마디를 방문하면서 수행하는 절차는 다음과 같다. 그 마디가 유망한지결정한다  만약

유망하면 그 마디에 해답이 있는 경우 그 해답을 프린트하고, 그렇지 않은 경우 그 자식
마디를 방문한다. 반면, expand?) 경우 18] 실행하면 그 마디와 자식마디들을 모두 방문
하는 절차와 일치한다. 일단 첫째 알고리즘을 보고 나면, 둘째 알고리즘으로 수정하는
건 별로 어렵지 않다.

이제 /-여왕말 문제를 시작으로 여러 가지 문제들을 =   추적 알고리즘을 개발하
려고 한다. 이 문제들 모두, 상태공간트리의 마디의 개수는 지수만큼 크거나, 그 이상이
되기도 한다. 되추적은 불필요한 마디 검사를 피하기 위해서 사용한다. 같은 7 HS 가지
고 두 가지 다른 사례를 적용했을 때, 한 사례에서는 검사하는 마디의 수가 아주 작고,

른 사례에서는 inn one  cia AAS 검사해야 하는 경우가 생길 수 있다. 이는
앞에서 공부한 알고                    추적 알고리즘은 효율적인 시간복잡도를 얻지 못
할 것임을 의미한다.  ne 이전에 사용했던 분석방법 대신 몬테칼로 기법(4006 Carlo
Technique) ° = 되추적 알고리즘을 분석한다. 이 기법으로는 주어진 되추적 알고리즘이
특정 UA (instance) 대해서 효율적인지를 결정할 수 있다. 몬테칼로 기법은 5.3절에서
다룬다.

ET 2

:

5.2 2-Y9Y 문제

7-여왕말 문제의 목표는 이미 공부했다. 유망함수는 두 여왕말이 같은 열이나 대각선에
있는지 검사해야 한다. 만약 000(1)를 :째 행에서 여왕말이 놓여있는 열이라고 하면, ky
행에 있는 여왕말이 같은 열에 있는지 검사하기 위해서 다음 등식이 성립하는지 검사해


===== PAGE 215 =====
202

chapter 5 되추적

야 한다.
col(i) = col(k)

대각선은 어떻게 검사하는지 보자. 그림 5.6을 보면 7 = 8인 경우의 예가 그려져 있다.
그 그림에서 행 6에 있는 여왕말은 행 8에 놓여있는 여왕말에 의해서 왼쪽 대각선으로
위혐받고 있고, 행 8에 놓여있는 여왕말에 의해서 오른쪽 대각선으로 위협받고 있다. 다

00/(6)- col(2)=4-8=—4=2-6

즉, 오른쪽에서 위협하는 여왕말에 대해서 열에서 차이는 행에서 차이의 역과 같다. 행
ko] 있는 여왕말은 행 에 놓여있는 여왕말에 의해서 어느 한쪽 대각선으로 위협받고
있으면, 다음과 같은 식이 성립한다.

col(i)—col(k)=i-k 또는 col(k)—col(i)=k-i

이제 알고리즘을 제시한다.

4
5

:                  E

>

8

그림 5.6 행 6에 있는 여왕말은 행 3에 놓여있는 여왕말에 의해서 왼쪽 대각선으로 위협받고 있
고. 행 2에 놓여있는 여왕말에 의해서 오른쪽 대각선으로 위협받고 있다


===== PAGE 216 =====
@®eee2e 8 0
5,2 ㅠ-여왕말 문제   203

> 알고리즘 5.|     /7-여왕말 SAS 푸는 되추적 알고리즘
문제 : 서양 장기판에 어떤 두 여왕말도 같은 행, 열, 대각선에 있지 않도록 ny 여왕말을
놓으시오.
입력 : 양의 정수 7
출력 : 7×7 서양 장기판에 *개 여왕말을 서로 위협받지 않고 놓을 수 있는 가능한 모든
방법. 각 출력은 인덱스 범위가 1부터 7까지인 정수배열 60(로 이루어진다. 여기서 60110]
는 번째 행에 있는 여왕말의 놓여 있는 열이다.
void queens (index 1)
{
index 7;
if (promising{1))
if G@ == p)
cout << co/{1] through col [n] ;
else
for (/ = 1; 2 <= 2; #++) {          // (+1) 번째 행에 있는 여왕말을 2개의 열에
coli+1] = ./;                  // 놓을 수 있는지 각각 검사한다.
queens(i+1) ;
}
}
bool promising (index i)
{
index k;
bool switch ;
ike ie
switch = true ;                          // /뻔째 행에 있는 여왕말을 위협하는
while (k < i && switch) {              // 여왕말이 있는지 검사한다.
if (col| i] == col[ k] || abs(col[i]—col[k]) == 2
switch = false ;
ay
}
return switch;
}

어떤 알고리즘이 두개 이상의 루틴으로 구성되어 있으면, 특정 프로그래밍 언어의 규
칙을 따르지 않는다. 대신 주 Fel main routine) S 먼저 제시한다. 알고리즘 5.1에서 주
루틴은 000008이다. 2.1절에서 언급한 관례에 따라 nT} col’: 재귀 루틴 00004의 입력
이 아니다. 만약 nz} cold] 전역변수로 정의된다면, 00008의 최초 호출은 다음과 같다.

queens(0);


===== PAGE 217 =====
204

chapter 5 되추적

알고리즘 5.12 2 -여왕말 문제의 해답을 모두 생성한다. 왜냐하면 문제를 그렇게 제
시했기 때문이다. 해답을 하나 찾고 빠져나가는 경우를 대비해서 이런 식으로 문제를 서
술한다. 이렇게 하면 알고리즘이 덜 어수선해진다. 일반적으로 이 장에서 제시한 문제들
은 해답을 하나 또는 어릿 또는 모두 요구하도록 서술할 수 있다: 실제 상황에서는 응용
분야의 요구에 따라 좌우된다. 이 책의 알고리즘은 해답을 모두 찾아주도록 작성되었다.
답을 하나 찾고 멈추는 알고리즘으로 수정하기는 쉽다.

이론적으로 알고리즘 5.1을 분석하기 어렵다. 이 알고리즘을 분석하기 위해서 검사하
는 마디의 FS 여왕말의 개수인 7.의 함수로 나타내야 한다. 가지친 상태공간트리에서
마디 개수의 상한은 상태공간트리 전체에서 마디의 개수를 세어서 구할 수 있다. 전체
트리에는 수준 0에서 마디 1개, 수준 1에서 마디 7개, 수준 에서 마디 ”^개, .…, 수준
에서 마디 "개가 있다. 총 마디의 개수는 다음과 같이 계산한다.

'  『     "  ea
가 70770 ae et I =

n-1

이 등식은 부록 AS] 예제 &.4에서 얻어진다. n= 8 91 경우, 상태공간트리의 마디 개수는
다음과 같다.
gstl_4
8-1
이 BA ATE 가치가 별로 없는데, 그 이유는 되추적을 하는 목적 자체가 이렇게 많은
마디의 검사를 피하기 위한 것이기 때문이다.
다른 분석 방법으로 유망한 마디의 개수의 상한을 구해보는 방법도 생각해 볼 수 있다.
그 상한을 계산하기 위해서 어떤 두 여왕말도 같은 열에 놓지 않는다는 사실을 이용할
수 있다. AS 들어, 7= 8 인 경우를 생각해보자. 첫째 여왕말은 8개 열 중에서 어느 곳
에 놓아도 된다. 일단 첫째 여왕말을 놓고 나면, 둘째 여왕말을 놓을 수 있는 열은 최대로
7개이고, 둘째 여왕말을 놓고 나면, 셋째 여왕말을 놓을 수 있는 SS 최대로 6개이고,
등등 이런 식으로 나간다. 그러므로 유망한 마디의 최대 개수는 다음과 같다.
1+8+8×7+8×7×6+8×7×6×5+ … +8!= 109,601 유망마디
이 결과를 임의의 nol] 대해서 일반화하면, 유망한 마디의 최대 개수는 다음과 같다.
1+72+722(02-1)+7(02-1)07-2)+ … +n! 유망마디

이러한 분석으로는 이 알고리즘의 효율성을 제대로 파악할 수 없는데, 그 이유는 다음
과 같다. 첫째, 함수 promising A] 대각선 검사를 고려하지 않았다. 따라서 상한보다
유망한 마디의 개수가 훨씬 작을 수 있다. 둘째, 검사한 마디의 총 개수는 유망한 마디와
유망하지 않은 마디를 모두 포함한다. 앞으로 알게 되겠지만, 유망하지 않은 마디의 개수

= 19,173,961마디



===== PAGE 218 =====
000600000
5.2 #-여왕말 문제   205

는 유망한 마디의 개수보다 훨씬 많을 수 있다.

이 알고리즘의 BSS 결정하는 간단한 방법은 알고리즘을 실제로 실행하여 검사하는
마디의 개수를 세어 보는 것이다. HE 5.1에 여러 7값에 대한 결과가 나와 있다. 되추적
알고리즘을 7-여왕말 문제를 푸는 다른 알고리즘과 비교해 놓고 있다. 알고리즘 1은 되
추적 없이 상태공간트리를 깊이우선검색한다. 검사하는 마디의 개수는 상태공간트리 전
체의 마디 개수이다. 알고리즘 2는 여왕말 SS 같은 행이나 열에 둘 수 없다는 사실만
이용한다. 알고리즘 2는 /:개의 각 열에서 BY 1에 놓을 여왕말을, 첫째 여왕말이 차지한

을 제외한 n— 1H] 각 열에서 BY 2에 놓을 여왕말을, 처음 두 여왕말이 차지한 SS
제외한 n— 27H 각 열에서 행 에 놓을 여왕말을, 등등 이런 식으로 시험하여 총 n! 79]
해답후보를 생성한다. 해답후보를 생성한 후, 대각선상에서 서로 위협하는 여왕말이 있
는지 검사한다. 되추적 알고리즘의 강점은 nz 함께 급격히 증가한다는 사실을 주목하
자. = 4일 때 알고리즘 1은 되추적 알고리즘보다 6배 조금 안 되는 개수의 마더를 점검
하고, 되추적 알고리즘은 알고리즘 보다 약간 못한 것처럼 보인다. 그러나 7= 14일 때
알고리즘 1은 되추적 알고리즘보다 거의 33.,000,000배나 많은 마디를 검사하고, 알고리
즘 2가 생성한 해답후보의 개수는 되추적 알고리즘으로 검사한 마디의 개수보다 OF 230
배 많다. 검사한 많은 마디들이 유망하지 않을 수 있음을 보여주기 위해서 표 5.1에서
유망한 마디의 개수를 나열하였다. 이는 둘째 방법으로 되추적 알고리즘을 구현하면(5.1
절에서 공부한 BHAlAl expand), 상당한 시간을 절약할 수 있음을 의미한다.

BSS 결정하기 위해서(표 5.1을 만들기 위해서 한 것처럼) 알고리즘을 실제로 실행하
는 것은 진정한 분석이 아니다. 되추적으로 얼마나 시간을 절약할 수 있는지 설명하기
위해 알고리즘을 실제로 실행하였다. 분석하는 목적은 알고리즘을 실행하기 전에 알고리
즘이 효율적인지를 결정하는 데 있다. 다음 절에서 몬테칼로 기법을 사용하면 어떻게 되
추적 알고리즘의 효율을 추정할 수 있는지 알아본다.

/.-여왕말 문제를 푸는 상태공간트리에서 같은 행에 두 여왕말을 둘 수 없다는 사실

mel
=
이용하였다. 다른 방법으로 n? 장기판 위치에 모든 여왕말을 두어보는 상태공간트리를

@ 표 5.1 7-여왕말 문제를 되추적으로 풀어 절약하는 검사횟수

알고리즘 1의        알고리즘 2의       되추적의           되추적으로 찾은
n 검사마디 개수'    검사 후보해 개수" 검사마디 개수     유망마디 개수
341                  24                   61                   17
8 19,173,961           40,320               15,721               2057
12 9,73 10”              4.79 X 10°               1,01 < 10"               8,56 X 10°
14: 1,20 10°               8,72 X 10°               3,78 X 10°                2.74 X10"

* 답을 모두 찾는데 필요한 검사 개수를 나타냄
+알고리즘1은 되추적없이 상태공간트리를 깊이 우선으로 검색
$알고리즘8는 각 여왕말을 다른 행과 열에 놓는 후보해를 !개 생성


===== PAGE 219 =====
206

chapter 5 -되추적

만들 수 있다. 이미 놓여진 여왕말과 같은 행이나, 열이나, 대각선에 놓일 때마다 이 나무
에서 되추적이 일어날 것이다. 이 상태공간트리에서 모든 마디는 장기판의 각 위치 당
하나씩 n? HS] 자식마디를 가지고 있다. 모두 (7”)"개의 잎이 있는데, 각각 다른 해답후
보를 나타낸다. 이 상태공간트리에서 되추적하는 알고리즘은 우리 알고리즘보다 유망한
마디를 더 찾지는 못할 것이지만, 함수 promising] YS 검사하는데 걸리는 추가시
간과 조사하게 될 추가적인 유망하지 않은 마디(즉, 이미 여왕말이 놓여진 자리에 다시
말을 놓으려고 시도하는 마디) 때문에 그래도 더 느릴 것이다. 일반적으로 상태공간트리
에 가능한 한 많은 정보를 구축하는 게 가장 효율적이다.

어떤 되추적 알고리즘이라도 유땅함수를 실랭하는데 걸리는 시간이 중요한 고려시항
이다. 즉, 우리의 목표가 검사하는 마디의 개수를 줄이는데 있는 것만은 아니다. 대신
체적인 HLS 증대하는데 있다. 유망함수가 AES 아주 많이 소모한다면 마디를 덜 검

사함으로서 얻게 되는 이득을 상쇄할 수 있다. 알고리즘 5.1의 경우 이미 놓여진 여왕말
에 의해서 조절되는 열, 왼쪽 대각선, 오른쪽 대각선의 집합을 추적, 기록하여 유망함
를 개선할 수 있다. 이런 식으로 하면 이미 놓여진 여왕말이 현재 두려고 하는 여왕말
위협하는지 검사할 필요가 없다. 현재 여왕말을 조절된 열이나 대각선에 놓을 지만 검ㅅ
하면 된다. 연습문제에서 이 개선 알고리즘에 대해서 더 자세히 알아본다.

5.8 몬테칼로 알고리즘을 사용한 HFA 알고리즘의 효율성 추정

앞에서 언급했듯이 다음 절에서 공부할 알고리즘은 모두 상태공간트리의 마디 개수가 지
수개 이상이다. 두 ARS] 7값은 같더라도 하나는 검사해야 할 마디가 몇 개 되지 않는
반면, 다른 하나는 상태공간트리 AAS 검사해야 할 수도 있다. 되추적 알고리즘이 어떤
특정 사례를 얼마나 효율적으로 처리하는지에 대한 =| (estimate)7} 있다면 그 사례
에 대해서 그 알고리즘을                oot 지 결정할 수 있다. 몬테칼로 알고리즘을
사용하면 그러한 추정치를 구할 수 있다.

몬테칼로          은 확률 알고리즘(0ㅠ008101118010 algorithm)°|t}, 확률 알고리즘은 실
행할 명령이 무작위로 결정되는 알고리즘이다. 결정 Matz]S(deterministic algorithm)
은 그렇지 않다. 지금까지 공부한 알고리즘은 모두 결정 알고리즘이다. 몬테칼로 알고리
즘(40066 Carlo algorithm)-2 표본공간의 무작위 표본의 평균치를 가지고 표본공간에서
정의된 무작위변수의 기대치를  추정한다(#본종간,  무작위표본, 무작위변수, 기대치에
대해서는 부록 AS] 4.8.1절을 참조하자). 추정치가 실제 기대치에 근접하리라는 보장은
없지만 알고리즘을 오래 실행할수록 실제 기대치에 근접할 확률은 중가한다.

몬테칼로 알고리즘을 사용하여 특정 사례에 대한 되추적 알고리즘의 SSS 다음과
같이 추정한다. 주어진 사례를 가지고 트리에서 검사하리라 생각되는 마디로 구성된 "전
형적인 경로"를 생성하고, 경로에 있는 마디의 개수를 추정한다. 그 추정치는 해답을 모



===== PAGE 220 =====
a

@
53 몬테칼로 알고리즘을 사용한 되추적 알고리즘의 효율성 추정     207

두 찾기 위해서 검사하리라 생각되는 마디의 총 개수를 추정한 것이다. 즉, 가지친 상태
공간트리에서 마디 개수의 추정치가 되는 것이다. 이 기술을 적용하기 위해서 알고리즘
은 다음 조건을 반드시 만족해야 한다.
1. 상태공간트리의 같은 수준의 모든 마디에서 같은 유망함수를 사용해야 한다.
2, 상태공간트리에서 같은 수준에 있는 마디들은 모두 자식마디의 개수가 같아야
한다.
알고리즘 5.101-여왕말 BAS 푸는 되추적 알고리즘)은 이 조건을 만족한다.

몬테칼로 기술을 사용하기 위해서는 어떤 마디의 유망한 자식마디를 무작위로 생성할
필요가 있다. 이는 무작위로 유망한 자식마디를 생성한다는 뜻이다(무작위 절차에 자세
한 사항은 부록 AS] 4.8.1절을 참조하자). 이 기술을 프로그램으로 구현할 때는 의사무작
(pseudorandom) #3t 유망 자식마디를 생성할 수 있다. 이 기술은 다음과 같다.

© mo S 뿌리의 유망한 자식마디의 ASS 한다.

* 수준 1에서 유망한 마디 하나를 무작위로 생성한다. m, So] 마디의 유망한 자식
마디의 개수로 한다.

* 앞 단계에서 구한 마디의 유망한 자식마디 하나를 무작위로 생성한다. 7/;를 이
rs} 유망한 Alero] 래수도 하마.

* 앞 단계에서 구한 마더의 유망한 자식마디 하나를 무작위로 생성헌다. mek 이
마디의 유망한 자식마디의 개수로 한다,

유망한 자식마디가 없을 때까지 이 과정을 계속한다. 상태공간트리에 같은 수준에 있
는 마디들이 모두 자식마디의 개수가 같다고 가정하기 때문에 는 수준 (에서 마디들
의 유망한 자식마디의 평균 개수의 추정치가 된다. 다음과 같이 정의해보자.
(, =수준 에서 어떤 마디의 자식마디의 총 개수
어떤 마디 《,개의 자식마디 모두를 검사하고 #/,개의 유망한 자식만 검사한 자식마디이기
때문에 되추적 알고리즘이 해답을 모두 찾기 위해서 검사한 마디의 총 개수 추정치는 다
음과 같다.

16 + mot, + 7720072102 + «++ +mom,--- 77010 71 --

이 추정치를 계산하는 일반 알고리즘은 다음과 같다. 이 알고리즘에서 변수 mprod': 각
수준에서 만들어진 mom, 1,…」을 표현하는데 쓴다.


===== PAGE 221 =====
@00@000000
208    chapter 5 되추적

> 알고리즘 5.2

int estimate ( )

{

node rv;

몬테칼로 추정치 구하기
문제 : 몬테칼로 알고리즘을 사용하여 되추적 알고리즘의 ale 추정하시오.

입력 : 되추적 알고리즘이 풀려고 하는 문제의 사례

출력 : 알고리즘이 만들어 내는 가지친 상태공간트리에서 마디의 개수 추정치. 그 사례에
대하여 알고리즘이 해답을 모두 찾기 위하여 검사하는 마디의 개수가 됨.

int m, mprod, t, numnodes ;

v= 상태공간트리의 뿌리
numnodes = 1;

mi lk

mprod = 1;

while (22 != 0) {
t= v9} 자식마디의 개수;

mprod =

mprod * m;

numnodes = numnodes + mprod * t;

m= v2]

if (02 |=

유망한 자식마디의 개수;
0)

v= v9] 무작위로 선택한 자식마디의 개수;

}

return numnodes ;

> 알고리즘 5.3

다음은 알고리즘 5.101-여왕말 BAS] 되추적 알고리즘:에 대한 알고리즘 5,29] 특별
판이다. no] 알고리즘 5.1에 파라미터이므로 이 알고리즘에 7을 넘겨준다.

알고리즘 5.1에 대한 몬테칼로 추정치 구하기(/-여왕말 문제의 되추적 알고리즘)

문제 : 알고리즘 5.1의 효율 추정

입력 : So] 정수 7

출력 : 알고리즘 5.1이 만들어 내는 가지친 상태공간트리에서 마디의 개수 추정치. 두 여왕
말이 서로 위협하지 않도록 서양 장기판에 개 여왕말을 놓는 방법을 모두 찾기 전에 알고
리즘이 검사하는 마디의 개수가 됨.

int estimate_n_ queens (int 22)

{

index 7, j, co/[{1 .. aj;
int m, mprod, numnodes ;
set_of_index prom_ children ;



===== PAGE 222 =====
}

7 = 0:

numnodes = 1;

72 = Vs

mprod = 1;
while (m != 0 && i != n) {
mprod = mprod * m;

}

numnodes = numnodes + mprod * n;    // 자식마디의 개수는
fees
in = 0;

prom_children = @;

// 유망한 자식마디의 AWS 공집합으로 초기화

for § = 1; / <= n; 12400 {
cal|i|\, = J;

}

if (promising{i)) {
m++;                              // 함수 promising? 알고리즘 5.15} 동일
prom_children = prom_children U {j};

}

// 유망한 자식마디를 결정

if (m != 0) {

J = prom_children|\)) 무작위로 선택;

00/| | = 7;

return numnodes ;

몬테칼로 알고리즘을 사용할 때 두 번 이상 실행하여 추정치를 구해야 하고, 그 결과의
평균을 실제 추정치로 사용해야 한다. 통계학에서 표준으로 쓰이는 방법을 사용하면 시
도한 결과로 검사한 마디의 실제 개수에 대한 신뢰구간을 결정할 수 있다. 경험으로 보면
20번 정도 시도하면 보통 충분하다. 몬테칼로 알고리즘을 여러 번 실행시키면 좋은 추정
치를 구할 확률이 높아지지만, 결과가 항상 좋은 추정치라는 보장은 결코 없다는 걸 주의
해야 한다.

/.-여왕말 문제는 각 7값에 대해서 답이 하나밖에 없다. 그러나 되추적 알고리즘으로
푸는 문제의 대부분은 그렇지 않다. 몬테칼로 기솔을 한 번 적용해서 얻은 추정치는 하나
의 특정한 사례일 뿐이다. 이전에 설명했듯이 같은 7값을 가진 사례 둘 중에서 하나는
검사해야 할 마디가 몇 개 되지 않는 반면, 다른 하나는 상태공간트리 전체를 검사해야
할 수도 있다.

몬테칼로 추정법을 사용하여 얻은 추정치가 첫째 해답을 찾기 전에 얼마나 많은 마디
를 검사할 것인지를 반드시 나타내는 것은 아니다. HS 하나만 얻기 위해서 모든 해답
을 찾는 일부분의 마디만 검사할 수도 있다. 예를 들어, 그림 5,4를 보면 셋째와 넷째
열에 각각 첫째 여왕말을 놓는 두 가지를 해답 하나만 찾기 위해서 횡단할 필요는 없다.


===== PAGE 223 =====
@0@000000
0   chapter 5 되추적

21

부분집합의 합 구하기

© 예제 5.2

© 예제 5.3

4.4.1절의 0-1 배낭 채우기 BAS 되돌아보자. 이 문제에서 밤손님이 S42 수 있는 아이
템의 집합이 있고, 아이템은 각각 무게와 값어치를 가지고 있다. 밤손님의 배낭은 아이템
의 총 무게가 WS 초과하면 BolZlc, 따라서 총 무게가 WS 초과하지 않으면서 Sl
아이템의 총 값어치가 최대가 되도록 하는 것이 목표이다. 아이템 모두 무게 당 값어치가
같다고 가정하자. 그러면 단순히 총 무게가 WS 초과하지 않는다는 제한 조건하에서
총 FAIS 최대로 하는 게 밤손님의 최적 해답이 될 것이다. 밤손님은 먼저 총 무게가
까 되는 아이템의 집합이 있는지를 결정하려고 할 것이다. 왜냐하면, 이 경우가 최선
이 될 것이기 때문이다. 그런 집합을 결정하는 BAS 부분집합의 합 구하기 문제(640-
of—subsets 2070010200라고 한다.

세부적으로 보면, 부분집합의 합 구하기 문제에서는 양의 정수(무게) w,7h 7/개와 양의

정수 『까 있다. 목표는 합이 1까 되는 정수의 부분집합을 모두 찾는 것이다. 앞에서
언급했듯이 해답을 모두 찾을 수 있도록 문제를 기술한다. 그러나 밤손님은 해답을 하나
만 찾아도 충분히 행복해할 것이다.

n=5, 1\=20이고, 각 w= 다음과 같다고 가정하자.
401 =5, w, =6, wz =10, 10, = 11. w, =16
다음과 같기 때문에,
201+ㅜ10,2+106 =5+6+10=21

w, tw; =5+16=21
w,tw, =10+11=21

해답은 {wy wo, wz}, 101, ws}, (wy, wy} 가 된다.

ae)
SS
스

ake 검사하여 풀 수 있다. 그러나 Sn 값에 대해서 체계적인 접근이 필요하다.
를 만들어 푸는 방법이 하나 있다. 트리를 구축하는 방법은 그림 5."에 나와
있다. 편의상 그림 5,79] 트리는 무게를 세 가지만 고려한다. 0, 를 포함하려면 뿌리마디
에서 왼쪽으로 가고, w, 을 제외하려면 오른쪽으로 간다. 비슷한 방법으로 수준 1에서 6,
를 포함하려면 마디에서 왼쪽으로 가고 를 제외하려면 오른쪽으로 간다. 같은 방법으
로 계속 반복한다. 각 부분집합은 뿌리마디에서 잎으로 가는 경로로 표현한다. w/z
함할 때 포함하는 이음선 상에 4라고 표기한다. 를 제외할 때 0으로 표기한다.

그림 5.8을 보면 n=3, =6이고 w,; 값이 다음과 같은 상태공간트리가 있다.

wW,=2, we=4, 1065



===== PAGE 224 =====


===== PAGE 225 =====
@eeeee @
212   chapter 5 되추적

넘길 것이다. 따라서 weight? 와 같지 않으면(그 마디 해답이 있다는 의미임), 다음

BAS 만족하면, 수준 8의 마디는 유망하지 않다.
weight+w,., > W

덜 분명하기는 하지만 마디가 유망하지 않다고 알려주는 표시가 E 하나 있다. 어떤
주어진 마디에서 남아있는 아이템의 무게의 총 합에다 weightS 더해서도 최소한 와
같아지지도 않으면, 그 마디 이후로 아무리 확장하더라도 와 같아질 수가 없다. 이는
total] 남은 아이템의 총 무게일 때 다음 조건을 만족하면 이 마디는 유망하지 않음을
의미한다.

weight + total < W

다음 예제에서 이 되추적 전략을 설명한다.

*예제 54 그림 5.9에 n=4, 17=13이고, 다음 값들을 되추적에 사용할 때 가지친 상태공간트리

auf

보여

=8, 00=4, ms ws

유일한 해답은 음영 처리된 마디에서 찾을 수 있다. 그 해답은 (wz, wy, wy} 이다. 유망하지 않

그림 5.9 예제 5.4에서 되추적을 사용하여 만들어 낸 7
까지 포함된 총 무게가 저장되어 있다. 유일한 해답은 음영 처리된 마디에서 찾을 수 있다. 유망하
지 않은 마디는 각각 ×로 표시되어 있다.

AIS! 상태공간트리. 각 마디에는 그 마디


===== PAGE 226 =====
> 알고리즘 5.4

@0000000
54 부분집합의 합 구하기  213

은 마디는 ×로 표시한다. 12, 8, 9S 포함하는 마디들은 다음 무게(6)을 추가하면 \664/의 값이
WS 초과하기 때문에 유망하지 않다. 7, 3, 4, OF 포함하는 마디들은 남은 무게의 총 합이
weight?| 값을 WA) 올리기에 충분하지 않기 때문에 유망하지 않다. 해답을 포함하지 않은
상태공간트리에서 잎은 자동적으로 유망하지 않다. 왜냐하면, W724) weights 올릴 수 있는
만큼 충분히 무게가 남아 있지 않기 때문이다. 7S 포함하고 있는 잎이 이를 나타내 준다. 가지친
상태공간트리에는 15개 마디만 있는 반면, 전체 상태공간나무에는 31개의 마디가 있다.

어떤 마디까지 포함된 무게의 합이 와 같으면, 그 마디에 해답이 있다. 그러므로
아이템을 더 추가시킨다고 또 다른 해답을 구할 수는 없다. 이는 만약 다음 등식이 성립
하면,
W= weight

HAS 프린트하고, 되추적해야 한다. 이 되추적은 일반 프로시저 checknodeS Sele
사용할 수 있다. 왜냐하면 이 프로시저는 일단 해답을 찾은 유망한 마디 이후는 절대로
확장하지 않기 때문이다. 어떤 되추적 알고리즘은 상태공간트리의 잎에 도담하기 전에
해답을 찾는 BPE 때로 있다는 사실을 646642006를 공부할 때 언급했다. 이 알고리즘
이 그런 알고리즘 중 하나이다.

이제 이 전략을 쓰는 알고리즘을 제시한다. 이 알고리즘은 배열 includeS 사용한다.
wli]S 포함하면 220/2062]가 ‘yes’ BS 가지고, 그렇지 않으면 ‘no’ 값을 가진다.

주
문제 : 개 양의 정수(무게)와 양의 정수 WH 가지고, 합이 까 되는 모든 BHO] 조합
을 모두 구하시오.
입력 : 양의 정수 ×, (감소하지 않는 순으로) 정렬된 양의 정수의 배열 we 1부터 n),
양의 정수 W
출력

: 합이 『까 되는 모든 정수의 조합

void sum_of_subsets (index i,

i

int weight, int total)

if (promising{i))
if (weight ==
cout << include{1]A] includeli] 7A] ;

else {

includeli+1] = “yes”; // w{i+1]& 포함한다.
sum_of_subsets (7 + 1, weight + w{i+1], total— w{i+1]);
includeli+1] = “no”; // w{it+1]S 포함하지 않는다.
sum_of_ subsets (i + 1, weight, total—w\i+1]});

}


===== PAGE 227 =====
214

}

chapter 5 되추적

bool promising (index i);

{

return (weight + total >= W) && (weight == W || weight + w{it+1] <= W);

}

습에 따라서 n, w, W, includeH 이 프로시저의 입력이 아니다. 이 변수들을 전역
적으로 정의하여 sum_of subsets®] 최초 호출은 다음과 같다.

sub_of_subsets(0, 0, total);

여기서 total2] 초기값은 다음과 같다.
total = y wll
a

해답을 포함하지 않은 APNG a 잎은 유망하지 않다는 사실을 상기해보자.
그 이유는 \684/의 값을 까지 올릴 수 있을 만큼 무게가 남아 있지 않기 때문이다.
이는 이 알고리즘에서 종료조건인 ;:=#을 검사할 필요가 RSS 의미한다. 이 알고리즘
이 제대로 정확히 구현되었는지 검중해보자. ?=ㅠ일 때 total 값은 0이다(이유는 남아있
는 무게가 없기 때문이다). 따라서 이 시점에서 다음 등식이 성립하므로,

weight + total = weight + 0 = weight
이에 따라 다음 부등식이 성립한다는 사실은

weight + total > W

13

weight > WE 성립함을 의미한다. weight < W7t 항상 성립하도록 유지하기 때문에
weight = WY 수밖에 없다. 따라서 ?2=7일 때 함수 rn trues 넘겨주면
weight = W7} 된다. 그러나 이 경우 해답을 찾았기 때문에 재귀 호출은 없다. 그러므로
종료조건 i=n& WR 필요가 없다. @ 표현식에서 둘째 조건은 첫째 조건이 참이면
보통 계산하지 않기 때문에 함수 promising A 존재하지 않는 배열 아이템 417 + 1]은
절대 참조하지 않는다.
알고리즘 5.4가 검색하는 상태공간트리에서 마디의 개수는 다음과 같다.
1+24+27+ … +2" = 00711

이 등식은 부록 AL] 예제 ㅅ.8에서 구한다. 이 결과만을 가지고 보면, 최악의 경우가 이보
다 훨씬 좋을 수 있다는 fee   존재한다. 즉, 모든 사례에 대해서 상태공간트리의 작은
일부분만 검색하는 BPE 있을 수 있다는 것이다. 그러나 그렇지 않다. 각 nol] 대해서
알고리즘이 지수만큼 iv 개수의 마디를 방문하는 사례를 구축할 수 있다. 하나의 답만



===== PAGE 228 =====
06000000
5.5 그래프 색칠하기  215

원하는 경우조차도 마찬가지이다. 결과적으로 다음 (부)등식을 취하면,

호 20, < W      w, = W
하나의 해답 tw, |만 존재하며, 지수만큼 많은 개수의 마디를 방문할 때까지 찾을 수 없을
것이다. 이전에 강조했듯이 최악의 경우가 지수이지만 아주 많은 사례에서 이 알고리즘
이 효율적일 수 있다. 몬테칼로 기술을 사용하여 알고리즘 5.4의 효율을 여러 가지 사례
를 가지고 추정하는 프로그램을 연습문제로 해 보도록 하자.
답을 하나만 내주도록 문제를 기술해도 0-1 배낭 채우기 문제와 마찬가지로 부분집합
의 합 구하기 문제도 9장에서 다루는 부류의 문제 계층에 속한다.

@® 5.5 그래프 색칠하기

* 예제 5.5

-색칠하기 BARS 비방향그래프에서 서로 인접한 정점이 같은 색을 갖지 않도록 최대
/개의 다른 ALOR 칠하는 방법을 모두 찾는 문제이다. -색칠하기 문제는 m Flo] 다
르면 다른 문제로 취급한다.

그림 5.10의 그래프를 보자. 이 그래프에서 2-색칠하기 문제의 해답은 없다. 왜냐하면, 최대 2개
의 다른 색까지만 사용할 수 있다면, 인접한 정점이 같은 색을 갖지 않도록 정점을 색칠하기는
불가능하다. 이 그래프에서 3-색칠하기 문제의 해답 중 하나는 다음과 같다.

정점                 색
vy                  색1
2                                  색2
03                                  색2
팸                                  색2

이 그래프에서 8-색칠하기 문제는 해답이 총 6가지이다. 그러나 6가지 SHES 색이 조합된 방법

그림 5.10 2-색칠하기 문제에 대해서는 해답이 없는 그래프. 이 그래프에서 3-색칠하기 문제에
대한 해답은 예제 5.5에 나와 있다.


===== PAGE 229 =====
216

chapter 5 되추적

으로만 다를 뿐이다. 예를 들면, 또 다른 해답은 (을 ME 칠하고, 와 vB Me 칠하고,
을 색8으로 칠하면 된다.

그래프 색칠하기의 주요 응용분야는 지도 색칠하기이다. 두 개의 이음선이 서로 교차
하지 않도록 그린 그래프를 평면그래프(61808 81804)라고 한다. 그림 5,112] 아래쪽에
있는 그래프는 평면그래프이다. 그러나 o}LA (vy, v5) Pt (vo, vy) S 추가하면 더 이상
평면그래프가 아니다. 모든 지도는 그에 상응하는 평면그래프가 존재한다. 지도에서 각
지역은 정점에 해당한다. 만약 한 지역이 다른 지역과 인접해 있으면, 그에 해당하는 정
ASS 이음선으로 연결한다. 그림 5.1에는 위쪽에 지도가 있고, 그 아래 그에 상응하는
평면그래프가 있다. 평면그래프에서 7-색칠하기 문제는 최대 개의 색을 사용하여 인
접한 지역이 같은 색이 되지 않도록 지도를 색칠하는 BHO] 얼마나 있는지를 구한다.
、-색칠하기 문제에 대한 간단한 상태공간트리는 수준 1에서 정점 vO 가능한 모든
AWS 각각 시도해 보고, 수준 2에서 정점 《;에 가능한 모든 색을 각각 시도해 보고, 이런
식으로 수준 에서 정점 에 가능한 모든 색을 각각 시도해볼 때까지 계속한다. 뿌리에
서 잎까지 경로는 각각 해답후보가 된다. 어떤 두 두 인접한 정점이 같은 색인지를 결정함으
로써 해답후보가 해답인지를 검사한다. SES 피하기 위해서 앞으로 이 절에서 "마디'는
상태공간트리에 있는 마디(정점)를 가리키고, “BAS 색칠하는 THES] 정점(마디)을

2

V3                    럭

그림 5.11 지도(위)와        프(아래)


===== PAGE 230 =====
> 알고리즘 5.5

@‥《000000 0
5.5 그래프 색칠하기  217

그림 5.12 그림 5.10에 있는 그래프를 3-색칠하기 위해서 되추적 기법을 사용하여 구한 가지친
상태공간트리의 일부분. 첫째 해답은 음영 처리된 마디에서 찾을 수 있다. 유망하지 않은 마디는

×로 표시되어 있다.

가리키는 것을 기억하기 바란다.

이 문제에서 되추적할 수 있는데, 그 이유는 어떤 마디에서 색칠한 정점과 인접한 정점
이 이미 그 마디에 사용된 색인 경우 그 마디는 유망하지 않기 때문이다. 그림 5.18에서
그림 5.10의 그래프를 3-색칠하는데 되추적 전략을 적용하여 만들어진 가지친 상태공간
트리를 보여준다. 마디에 표시된 수는 그 마디에서 정점을 색칠하는데 사용한 색의 개수
이다. 첫째 HS 음영 처리된 마디에서 찾을 수 있다. 유망하지 않은 wpe ×로 표
시되어 있다. vy, 을 ALE 칠한 후, 에 색1을 선택하면 4, 이 《;와 인접해 있으므로 유망
하지 않다. 비슷하게, 0, vo, 을 AML, 색3, 색8으로 각각 칠한 후, 에 MS 선택하면
v,°] 에 인접해 있으므로 유망하지 않다.

이제 모든 mol 대한 ㅠ-색칠하기 BAS 푸는 알고리즘을 살펴보자. 이 알고리즘
에서 그래프는 4.1절에서와 마찬가지로 인접행렬로 표현된다. 그러나 그래프에 가중치가
없기 때문에 두 정점을 We 이음선의 존재여부에 따라서 Yao] 각 엔트리는 ㅠ46나
false7} 된다.

ㅠ-색칠하기 문제를 푸는 되추적 알고리즘

문제 : 비방향그래프에서 7/개의 색만 사용하여 인접한 정점이 같은 색이 되지 않게 정점


===== PAGE 231 =====
@0@000000
218   chapter 5 되추적

을 AAS 수 있는 BE WHS 구하시오.

입력 : 양의 정수 과 7, 그리고 7개의 정점을 가진 비방향그래프. 그래프는 행과 열의

인덱스가 모두 1부터 7까지인 2차원 배열 WHE 표현된다. 여기서 ?번째 정점과 /번째 정

점 사이에 이음선이 존재하면 10][7]는 ㅁㅠ06이고, 그렇지 않으면 186186이다.

출력 : 최대로 mM] 색을 가지고 인접한 정점이 같은 색이 되지 않게 그래프에 색칠하는
가능한 모든 경우. SAS 인덱스가 1부터 7까지인 배열 700/22이다. 여기서 00000] 값

inal 정점에 할당된 색(1부터 ㅠ사이의 정수)이다.

8 고

void 72 coloring (index i)

{

int color;

if (promising{1))
if @ =— 2)
cout << 00001 1 ]에서 veolor| n|7FAI ;
else
for (color = 1; color <= m; color++) {   // 다음 정점에 모든 색을 시도해 본다.
veolor|i+1] = color ;
m_ coloring{i+1);
}
}

bool promising{index i)
{

index /;

bool switch ;

switch = true;
J=1;
while (j < 7 && switch) {                // 인접한 정점에 이 색이 이미 칠해져
f (WL A]L/] && veolor{ i] == veoloj}) // 있는지 점검한다
switch = false ;
Jaco
}

return switch ;

보통 사용하는 관습에 따라서 7, m, WS veolor= 위 두 루틴의 입력이 아니다. 알

즘을 구현할 때 이 루틴들은 2, m, 가 입력인 간단한 프로시저 안에 지역적으로

정의하고, veolor= 지역적으로 정의한다. 22 _ coloring?) 최상위 수준 SSS 다음과
같이 하면 된다.

72 00702228(0)


===== PAGE 232 =====
@‥00060000 0
5.6 해밀튼 회로 문제   219

ㅇ

ㅣ 알고리즘의 상태공간트리에 있는 마디의 개수는 다음과 같다.

gaint

m= I
이 Bae 부록 AQ| 예제 A A044] 구한다. 주어진 mI} 7에 대해서 (n2] 형식으로) 최소
한 지수만큼 많은 마디의 개수를 점검하는 사례를 만들 수 있다. 예를 들어, mo] 단순히
이코, -   nA) 더은 모든 정점으로 가는 의음선의 있고 0,99} 1 & 잇는 이음
선이 유일한 다른 이음선이라면 해답은 존재하지 않는다. 그러나 이 사실을 알기 위해서
는 상태공간트리의 거의 모든 마디를 방문해야 한다. 다른 되추적 알고리즘과 마찬가지
로 이 알고리즘은 크기가 큰 특정 사례에 대해서 BSAA 수 있다. 5.3절에서 설명한
몬테칼로 기술을   이 알고리즘에도 적용할 수 있다. 이는 특정 사례의 효율을 추정하기
위하여 이 기술을 사용할 수 있다는 의미이다.

최악 sre nl] 대해서 지수가 아닌 2-색칠하기 알고리즘은 존재하는데 AS
문제로 이 알고리즘을 작성해 보도록 한다. m > 3인 maj] 대해서 최악의 경우 효율적인
알고리즘은 아직 아무도 개발하지 못했다. 부분집함의 함 구하기, 0-1 배낭 채우기,
m = 3 인 mAs} 문제들은 9장에서 다루는 문제의 부류에 속한다. 그래프에서 m
-색칠하는 방법을 하나만 찾는 경우라도 마찬가지이다.

l+m+m?+ -- +m" =

@ 5.6 AYE 회로 문제

같은 외판원 문제를 놓고 갑돌이와 갑순이가 BIS 벌였던 예제 3.18를 상기해보자. 20
개 도시 전체를 더 빨리 다녀올 수 있는 사람이 외판원 자리를 차지하게 되었다. 시간복
잡도가 다음과 같은 SAAS) 알고리즘을 사용하여 갑순이는 45% 안에 최단 여행경로를

찾았다.

T(n) = (02-1)(02- 2)27 0

갑돌이는 19!가지 여행경로 길이를 모두 계산하였다. 그의 알고리즘은 3,800년 이상 a
리기 때문에 그 프로그램은 아직도 돌아가고 있다. 물론 갑순이가 그 외판원 자리를 차지

USO 물어볼 필요도 없다. 그 후 갑순이가 판매실적이 아주 좋아서 감순이의 상관은
판매영역을 40개 도시로 늘려주었다고 가정하자. 그러나 이 영역 안에 있는 도시들 모두
가 도로로 연결되어 있지는 않다. 갑순이의 동적계획 알고리즘이 단위연산을 처리하는데
1 microsecond®] 걸린다고 가정하였다. 이 알고리즘으로 40개 도시를 여행하는 최단 OF
행경로를 구하는 시간을 계산해 보면 다음과 같다.

(40—1)(40—2)2*°~ 3s = 6.4614

이 정도의 시간 때문에 갑순이는 다른 알고리즘을 찾아보아야 한다. 그녀는 너무 어려워


===== PAGE 233 =====
220

chapter 5 되추적

A 최적 여행경로는 찾을 수 없으리라 판단하고, 그냥 아무 경로나 택하더라도 만족하게
된다. 도시를 직접 잇는 도로가 모든 도시들 사이에 존재한다면 도시를 어떤 순서대로
나열해도 여행경로가 된다. 그러나 갑순이의 새 판매영역의 경우는 그렇지 않다. 따라서
이제 갑순이의 문제는 그래프에서 어떤 경로라도 찾는 것이다. 이 문제를 처음 제안한
윌리암 해밀튼 경(817 William Hamilton)2] 이름을 따서 해밀튼 회로 문제(\1900111070187
Circuits Problem)2@}31 한다. 이 문제는 (외판원 문제와 같이) 방향그래프로 기술할 수도
있고, 비방향그래프로 기술할 수도 있다. 비방향그래프로 보통 많이 기술하기 때문에 여
기서도 그렇게 한다. 갑순이의 딜레마에서와 같이 이는 두 도시를 잇는 도로가 있다면
모두 왕복 차선이며, 그 도로는 하나밖에 없다는 걸 의미한다.

연결된 비방향그래프에서 해밀튼 회로(여행경로라 하기도 함)는 한 정점에서 출발하
여 그래프에 있는 모든 정점을 각각 정확히 한 번씩 방문하고, 다시 출발한 정점으로 돌
아오는 경로이다. 그림 5.13(8)의 그래프에는 ABE 회로 [01 , vo, vg, %, Ve, U5, Va,
03, 1]가 존재하지만, 그림 5.1800)의 그래프에는 해밀튼 회로가 존재하지 않는다. 해밀
튼 회로 문제는 연결된 비방향그래프에서 해밀튼 회로를 구한다.

이 BAS 풀기 위한 상태공간트리는 다음과 같다. 이 나무의 수준 OWA 출발 정점을
놓고, 그 정점을 경로의 0째 정점이라고 부른다. 수준 1에서는 출발 정점을 제외한 각

AAS 출발 정점 다음에 오는 첫째 정점으로 고려한다. 수준 2에서는 앞에서와 같은 정

그림 5.13 (

a)            밀튼 회로 [v,, Vo, Vg, V7, Ug, Us, V4, Uz, Vi ]7t 존재하고, (6)의
그래프에는 해

의 크래프에는 6

밀튼 회로가 존


===== PAGE 234 =====
알고리즘 5.6

06000000
5.6 해밀튼 회로 문제   221

점들을 각각 둘째 정점으로 고려한다. 그 이후 수준에서도 같은 방식으로 계속하다가,
마지막으로 수준 n— 144A] 앞에서와 같은 정점들을 각각 (n— 1) a 정점으로 고려한다.
이 상태공간트리에서 되추적하기 위해서 다음 사항을 고려한다.
1. 경로 상의 째 BAL 그 경로에서 (,-1)째 정점과 반드시 인접해 있어야 한다.
2. (n— 1)째 정점은 0째 정점(출발 정점)과 반드시 인접해 있어야 한다.
8. 1째 BAL 그 앞에 오는 1-1개의 BAS 중 하나가 될 수 없다.

다음 알고리즘은 위의 사항을 고려하여 되추적 한다. 이 알고리즘은 0, 을 출발정점으

로 고정시킨다.

해밀튼 회로 SAS 푸는 되추적 알고리즘

문제 : 연결된 비방향그래프에서 해밀튼 회로를 모두 구하시오.

입력 : 양의 정수 nz QAO] 7개인 비방향그래프. 그래프는 2차원 배열 WHE 표현한다.
이 배열의 행과 열의 인덱스는 1부터 /까지이다. 여기서 :째 BA [Al BAS 잇는 이음
Alo] 있으면 Willi] 값은 ㅁㅠ06이고, 그렇지 않으면 falseo]th,

출력 : 주어진 정점에서 출발하여 그래프상의 각 정점을 정확히 한 번씩 방문하고, 출발
정점으로 돌아오는 모든 경로. 각 경로의 SYS 인덱스가 0부터 ㅡ1까지인 인덱스의
WHS vindex|t}, 여기서 127206저기는 경로상에서 iA] BAL] 인덱스이다. 출발 정점의
인덱스는 127206퍼이이다.

void hamitonian (index 2)

{
index /;
if (promising{1))
cS 21)
cout << vindex{0]]A| vindex|n—1|7}A| ;
else
for (fj = 2; j <= n; #++) {               // 모든 정점의 다음 정점을 시도해 본다.
vindex| +1] = /;
hamiltonian(i+1);
}
}

bool promising (index i)

{

index /;

bool switch ;

== 2

1 &&! W|[vindex{n-1]][vindex{0]]) // AA 정점을 마지막 정점과


===== PAGE 235 =====
@0@00000 0
222   chapter 5 되추적

switch = false;                            // 인접해야 하고,
else if (7 > 0 &&! 9[102206저7 1]]| vindex{i)])     // A AAS (7-1)째 정점과
switch = false ;                            // 인접해야 한다.
else {
switch = true ;
j=
while (j < 7 && switch) {                 // 정점이 이미 선택되는지를 검사한다.
if (vindex| i] == vindex{/])
switch = false;
‘ae
}
}
return switch ;
}
관습에 따라서 2, W, vindex= 위의 어떤 루틴에도 입력이 아니다. 이 변수들을 전역
적으로 정의하면 /4777/707792 프로시저의 최초 SSS 다음과 같다.
vindex|0| = 1;           // y1& 출발정점으로 한다.
hamiltonian(0);

이 알고리즘의 상태공간트리에서 마디의 개수는 다음과 같이 계산한다.

1+(n—1)4+(n-1)? +

ㆍ+(2-1)" =

(n—1)"7?
글"

이 결과는 지수보다 훨씬 나쁘다. 이 등식은 부록 AO] 예제 ㅅ4에서 얻는다. 다음 사례는
상태공간트리 전체를 다 검사하지는 않지만, 검사하는 마디의 개수는 그래도 지수보다

많다(나쁘다). vB 가는 유일한 OAS v

8에서 온다고 하고, ov, 을 제외한 정점은 모두

서로 이음선으로 연결되어 있다고 하자. 이 그래프에 해밀든 회로는 존재하지 않으며,
알고리즘은 이 사실을 알기 위하여 지수보다 많은 개수의 마디를 검사한다.

갑순이의 딜레마로 돌아가서 (해밀튼 회로 문제를 푸는) 되추적 알고리즘은 (외판원
문제를 푸는) 동적계획 알고리즘으로 40개 inal AAS 주는데 결리는 시잔보다도 더 2

래 걸릴 가능성이 존재한다. 몬테칼로 기술을
을 사용하여 갑순이의 사례에 대한 효율을
를 모두 찾는데 걸리는 시간을 추정한다. 갑순
존재하는 경우) 첫째 회로를 찾은 후 알고

사용할 수 있는 조건을 만족하므로 그 기술

Aga + 있다. 그러나 몬테칼로 기술은 회로

이는 하나의 회로만 필요하므로 (회로가

}고리즘이 멈추게 할 수 있다. 독자는 7= 40인

경우의 사례를 만들어서 그 사례에서 모든 회로를 알고리즘이 얼마나 빨리 찾는지 추정

하고, 하나의 BRS 찾는 알고리즘을 실
대한 독자 자신 나름대로의 결론을 만들어

행시켜 보기를 권한다. 이런 식으로 이 이야기에

낼 주 잃을 테니까 팔이다:

하나의 여행경로만 찾고 싶다 하더라도 해밀튼 회로 문제는 9장에서 다루게 되는 문제

의 부류에 속한다.



===== PAGE 236 =====
@0000000
5.7 O-1 배낭 채우기 문제    223

@ 5,7 0-1 배낭 채우기 문제

4.4절에서 이 문제를 동적계획법으로 풀었다. 여기서는 되추적 기술을 이용하여 풀어본
다. 그 후 되추적 알고리즘을 동적계획 알고리즘과 비교한다.

oly

5.7.1 O-1 배낭 채우기 SAS 푸는 되추적 알고리
이 문제에서 아이템의 집합이 있고, 각 아이템은 무게와 값어치를 가지고 있음을 기억하
자. 무게와 값어치는 양의 정수이다. 밤손님은 배낭에 홈친 아이템을 담아갈 계획이고,
그 안에 넣은 아이템의 총 FA} WS 초과하면 배낭은 Bolzic}, 이 밤손님의 SHE
S 무게가 WS 초과할 수 없다는 제약 하에 총 값어치가 최대가 되는 아이템의 집합을
구하는 것이다.

부분집합의 합 구하기 문제(5.4절 참조)에서 사용한 것과 정확히 똑같은 상태공간트리
를 가지고 이 문제를 풀 수 있다. 즉, 첫째 아이템을 넣으면 뿌리에서 왼쪽으로 가고, 빼
면 오른쪽으로 간다. 같은 방법으로 둘째 아이템을 넣으면 수준 1의 마디에서 왼쪽으로
가고, 빼면 오른쪽으로 가고, 등등 이런 식으로 계속한다. 뿌리에서 잎까지의 경로는 각
각 해답후보가 된다.

이 문제는 최적화 4] (optimization problem)eH= 점에서 이 장에서 다룬 다른 문제들
과 다르다. 이는 검색이 완전히 끝날 때까지 마디가 해답을 포함하고 있는지 알지 못한다
는 뜻이다. 따라서 되추적을 조금 다른 방식으로 한다. 어떤 마디까지 넣은 아이템이 지
금까지의 최고 해답보다 값어치의 총액이 크다면, 지금까지의 최고 해답의 값을 바꾼다.
그러나 (아이템을 더 SAA) 그 마디의 후손 중 한 마디에서 더 좋은 해답을 찾을 수도
있다. 그러므로 ane 문제에서는 비서 한 마디의 자식마디들을 항상 방문한다. 다음은
최적화 문제의 경우 일반 되추적 알고리즘이다.

void checknode (node v)

{

node u;

Sy 5

if (value(v)7} 9657보다 좋다)
best = value(v);
if (promising{ v))
for (v2] 각 자식마디 2)
checknode( u);
}

변수 best: 지금까지 찾은 최고 해답의 값을 가지고, value= 마디 vol 해답의 값
이다. 어떤 해답후보의 값보다 나쁜 값으로 pests 초기회한 후, 최초 호출함 때 뿌리를

파라미터로 전달한다. 자식마디로 팽창할 수 있은 경우만 마디가 유망하다. 이 교재의
른 알고리즘도 해답이 존재하면 그 마디는 유망하다고 했다.


===== PAGE 237 =====
224

chapter 5 되추적

이제 이 기술을 0-1 배낭 채우기 문제에 적용시켜 보자. 먼저 마디가 유망하지 않다고
알려주는 표시를 살펴보자. 마디가 유망하지 SS 알려주는 분명한 표시는 배낭에 더
이상 아이템을 넣을 공간이 남아있지 않은 경우이다. 따라서 weight 어떤 마디까지 넣
은 아이템 무게의 합이라고 할 때 다음 부등식이 성립하면 그 마디는 유망하지 않다.

weight > W

최적화 문제의 경우 “유망“이란 자식마디로 더 팽창해야 함을 의미하므로, weight7} W
와 같은 경우조차도 유망하지 않다.

탐욕적 방법의 고려사항을 사용하여 좀 더 알아내기 어려운 표시를 찾아보자. 4.4절에
서 본대로 탐욕적 방법으로는 최적해를 구할 수 없었음을 기억하자. 여기서는 단지 트리
의 검색을 제한하는데 만 탐욕적 방법을 사용하지, 탐욕적 알고리즘을 개발하지는 않는
다. 먼저 2,/,의 값에 따라서 큰 것부터 아이템을 정렬한다. 여기서 와 p= 각각 iw
아이템의 무게와 값어치이다. 어떤 마디가 유망한지를 결정하려 한다고 가정해보자. 남
은 아이템을 어떻게 선택하는지에 상관없이 그 마디에서부터 배낭 빈틈없이 채우기 문제
(이 문제에서 HES 아이템을 부분적으로 $4 수 있음을 기억하자)에서의 제한을 At
용하여 얻는 값어치보다 더 많은 수익을 얻기는 불가능하다. 따라서 그 마디에서 팽창하
여 얻을 수 있는 수익의 상한을 구할 수 있다. prose 그 마디까지 넣은 아이템의 값어
치의 합이라 하자. weight= 그 아이템들의 FAS 합이라고 했음을 기억하자. 변수
bound?} totweight® profit?} weight 값으로 각각 초기화한다. 다음 탐욕적으로 아이
템들을 취하는데, 그 값어치는 bound} 더하고 FALE totweighto] 더한다. 이 과정은
totweight7+ WE 초과하게 되는 아이템을 집을 때까지 계속된다. 이때 남은 공간이 허
용하는 무게만큼만 그 아이템의 일부분을 취하고, 그 일부분의 값어치를 40240에 더한
다. 이 마지막 아이템의 일부분만 취할 수 있었다면 이 마디는 bound] 값과 같은 수익
을 얻게 될 가능성이 없지만, 40040는 그래도 그 마디에서 팽창하여 얻을 수 있는 값어
치의 상한은 된다. 그 마디가 수준 sol) 위치하고 있다고 하고, 수준 *에 위치한 마디는
무게의 합이 가 넘어가는 마디라고 하자. 그러면,

&^-1
totweight = weight +  > 0,
2=8+1

k=1

bound = | prosit +»)  D; 「       (W-—totweight)       x       Ae
j=itl             ee               Ws
kel       a                  a
처음 *-1개                 티져 이이 이           번째 아이템의
아이템의 값어치                                단위무게 당 값어치

maxprofit& 지금까지 찾은 최고 해답에서 값어치의 값이라고 하면, 다음 부등식이 성립

하면 수준 [에 위치한 마디는 유망하지 않다.


===== PAGE 238 =====
@‥0@00000 0
5.7 O-1 배낭 채우기 문제    225

bound < maxprofit

어떤 마디에서 확장해야 하는지 여부를 알려주는 한계를 구하는데 만 탐욕적 고려사항을
사용하였다. (탐욕적 방법에서와 같이) 후에 다시 고려해볼 기회도 없이 아이템을 탐욕적
으로 취하는 방법은 사용하지 않는다.

알고리즘을 설명하기 전에 예제를 먼저 살펴보자.

© 예제 5.6 ㅠ=4, 1=16이고 가져갈 수 있는 아이템의 내역이 다음과 같다고 가정하자.

.                                                    Pi
a                  P;                 W;               _—
W;
1                $40                2                $20
2                $30                5                 $6
3                $50               10                $5
4                $10                5                 $2

p/w; 값에 따라서 이미 정렬해 놓았다. 편의상 p,/w,; Io] 정수가 되도록 2,와 w,S 선택하였
일반적으로는 꼭 그럴 필요는 없다. 그림 5.14에 방금 설명한 되추적 기법을 사용하여 만든 7
친 상태공간트리를 보여준다. 총 값어치, 총 무게, 한계치는 위에서 아래로 각 마디에 표시힌  di
이들은 앞에서 언급했듯이 변수 profit, weight, bound? 값들이다. 최대 이익은 음영 처리된
마디에서 찾을 수 있다. 각 마디에 대해서 그 마디의 수준과 트리 왼쪽에서부터 위치가 마디 위
에 라벨로 표시한다. 예를 들어, a7] 칠해진 마디는 수준 3에 있고, 그 수준의 왼쪽에서 3째에
위치하고 있으므로 라벨 (3, 9)으로 표시한다. 이제 가지친 트리를 만들어 내는 절차를 설명한다.
이 절차에서 마디는 그 라벨로 나타낸다.

1, 7242770727을 $0으로 놓는다.

2, 마디 (0,0)(뿌리)를 방문한다.
(a) 그 값어치와 무게를 계산한다.

로 가 쑤

profit = $0

weight =0
(b) 그 한계를 계산한다. 23+5+10=17이고, 17 > 16(W2] 값)이므로, 셋째 아이템을 4]
하면 무게의 합이 WS 넘는다. 따라서 *=3이고 totweight?} bound= 다음과 같이

계산한다.

3-1
totweight = weight +  >  tue OOo =f
j=0+1

bound = profit +  ys  pit     (W-totweight) x    ae
j=0+1                            8
$50
= $0+$40+$30+ (16—  7) x 4p = $115

(0 무게가 0은 WE] 값인 16보다 작고, 한계 $115는 maxprofit?] 값인 80보다 크므로, 이
마디는 유망하다고 결정한다.


===== PAGE 239 =====
@00@00000 0
226   chapter 5 되추적

(4,2) (4,3)

그림 5.14 예제 5.601 되추적을 ASoto 만든 가지친 상태공간트리. 각 마디에 위에서 아래로

저장되어 = 값들은 그 마디에 도달하기까지 SE! 아이템의 총 값어치, 총 무게, 그리고 그 마디

에서 확장하여 얻을 수 있는 총 값어치의 한계. 최적의 해답은 음영 처리된 마디에서 찾는다. 유망
하지 않은 마디는 ×로 표시한다.

3, 마디 (1, 1을 방문한
(a) 그 값어치와 PAE 계산한다.

profit = $0 +$40 = $40
weight =0+2=2

(b) 무게 2= We] 값인 16보다 작거나 같고, 값어치 $402 maxprofit2] 값인 $0보다 크므
로, maxprofitS $40으로 놓는다.

(0) 그 한계를 계산한다. 23+ 5+10 =17이고, 17 > 16( 의 값)이므로 셋째 아이템을 취하
면 무게의 합이 WS 넘는다. 따라서 *=3이고 totweight2} bound= 다음과 같이 Al
산한다.

3-1
totweight = weight +  》  20. 29 마-
j=1tl

Bled!

2
bound = profit + SS pit  ( W—totweight) x   =
j=1tl            Ws

= $40 + $30 + (16 — 7) x 20 = gi15

10



===== PAGE 240 =====
(지금.

@06@00000 0
5.7 O-1 배낭 채우기 문제    227

(0) 무게가 2 WO] 값인 16보다 작고, 한계 $US 44807700의 값인 80보다 크므로, 이
마디는 유망하다고 결정한다.

. 마디 2, DS 방문한

(8) 그 값어치와 무 기를  계산한다.

profit = $40 + $30 = $70
weight =2+5=7

(b) 무게 은 WE] 값인 16보다 작거나 같고, 값어치 $70 maxprofit2] 값인 $40보다 크므
로, maxprofitS $70으로 놓는다.
(0) 그 한계를 계산한다.

3-1
totweight = weight +  >)  마 = 7
2=2+1

bound = $70 + (16 —  7) x = s115
(0) 무게가 7은 We] 값인

16보다 작고, 한계 $115는 maxprofit2| 값인 $70보다 크므로,
이 마디는 유망하다고 결정한

다.

~

. 마디 (3, 을 방문한다.

(a) 그 값어치와 무게를 계산한다.
profit = $70 + $50 = $120
weight =7+10=17

00 무게 17 WE] 값인 16보다 크므로, maxprofit®| 값은 변하지 않는다.

(0 무게 1/은 의 Bel 16보다 크거나 같으므로, 유망하지 않다고 결정한다.

(9 무게 때문에 이 마디는 유망하지 않으므로, 이 마디의 한계는 계산하지 않는다.

. 마디 (2, DS 되추적
. 마디 (3, 9)를 방문한다.

(a) 그 값어치와 FAS 계산한다. 아이템 은 포함하지 않으므로 다음과 같이 된다.

profit = 870
weight = 7
(b) 값어치 $70-2 maxprofit?] 값인 $70보다 작거나 같으므로, maxprofit?| 값은 변하지
OFS
jo

(9) 크 한계를 계산한다. 넷째 아이템의 FAS 더해도 합이 WS 초과하지 않고, 아이템이
4개만 있다. 따라서 *=5이고, ^40020는 다음과 같이 계산한다.
6-1
bound = profit +   >)  p; =$70+$10 = $80
2=3+1
(0) 무게 7은 의 값인 16보다 작고, 한계 $80 maxprofit®] 값인 $70보다 크므로, 이
마디는 유망하다고 결정한다.

부터 profit, weight, bound2| 계산은 연습문제로 남겨둔다. 게다가 maxprofite] 변하지


===== PAGE 241 =====
@00@00000 0
chapter 5 되추적

228

않으면, 그에 대해서 언급하지 않는다).

8. 마디 (4, 1)을 방문한

11,
, 마더 2, 2S 방문한대:

13,

14,

15,
16,

(a) 그 값어치와 AS 계산하면, $80과 127} 된다.

(b) 무게 12% We] 값인 16보다 작거나 같고, 값어치 $80-2- 2781270/8의 값인 $70보다 크
므로, maxprofit?| 값은 $80으로 놓는다.

(0) 그 한계를 계산하면, $80이 된다.

(0) 한계 $802 maxprofit2] 값인 $80보다 작거나 같으므로, 이 마디는 유망하지 않다고
결정한다. 상태공간트리에서 잎은 그 한계가 항상 224127042보다 작거나 같으므로 자
동적으로 유망하지 않게 된다.

. 마디 (3, VE 되추적
10.

마디 (4, 9)를 방문한다.

(a) 그 값어치와 무게를 계산하면, $70과 70] 된다.

06) 그 한계를 계산하면, $80이 된다.

(0) 한계 $70은 maxprofit2| 값인 $80보다 작거나 같으므로, 이 마디는 유망하지 않다고
결정한다.

마디 (1, 1)로 되추적

(a) 그 값어치와 무게를 계산하면, $40과 2이 된다.

06) 그 한계를 계산하면, $98이 된다.

(0) 무게 2는 의 값인 16보다 작고, 한계 $982 maxprofit2| 값인 $80보다 크므로, 이
마디는 유망하다고 결정한다.

마디 (3, 8)을 방문한다.

(a) 그 값어치와 무게를 계산하면, $90과 120] 된다.

(b) 무게 12는 We] 값인 16보다 작거나 같고, 값어치 $902 maxprofit2| 값인 $80보다
크므로, maxprofit= $90으로 놓는다.

(0) 그 한계를 계산하면, $98이 된다.

(0) 무게 12는 We] 값인 16보다 작고, 한계 $982 maxprofit2| 값인 $90보다 ABS, 이
마디는 유망하다고 결정한다.

마디 (4, 8)을 방문한다.

(a) 그 값어치와 FAS 계산하면, $1007} 17이 된다.

06) 무게 17은 의 값인 16보다 크거나 같으므로, 이 마디는 유망하지 않다고 결정한다.

(0) 무게 때문에 이 마디는 유망하지 않으므로, 이 마디의 한계는 계산하지 않는다.

마디 (3, oe 되추적

마디 (4, 4)를 방문한다.

(a) 그 값어치와 무게를 계산하면, $90과 12이 된다.

06) 그 한계를 계산하면, $90°] 된다.

(0) 한계 $90은 maxprofit2] 값인 $90보다 작거나 같으므로, 이 마디는 유망하지 않다고
결정한다.



===== PAGE 242 =====
@‥06060000 0
5.7 _0-1 배낭 채우기 문제    229

17, 마디 (2, YB 되추적
18. 마디 (3, 4)를 방문한다.
(a) 그 값어치와 무게를 계산하면, $40과 20] 된다.
09) 그 한계를 계산하면, $500] 된다.
(0) 한계 $502 maxprofit2] 값인 $890보다 작거나 같으므로, 이 마디는 유망하지 않다고
결정한다.
19. 뿌리로 되추적
20. 마디 (1, 9)를 방문한다.
(a) 그 값어치와 무게를 계산하면, $0과 00] 된다.
09) 그 한계를 계산하면, $820] 된다.
(0) 한계 $822 2241770/2의 값인 $90보다 작거나 같으므로, 이 마디는 유망하지 않다고
결정한다.
21. 뿌리로 되추적
(a) 뿌리에 더 이상 자식마디가 없으므로 완료되었다.

가지친 상태공간트리에 마디가 13개 있는 반면, 전체 트리에는 마디가 31개 있다.

이제 알고리즘을 설명한다. 이 문제는 최적화 문제이므로 현재 최고인 아이템의 집합
과 그 값어치의 BS 기록하는 작업을 추가하였다. 배열 465650/과 변수 maxprofitS 이
용하여 이 작업을 한다. 이 장에서의 다른 문제와는 달리 하나의 최적의 해를 찾도록 한다.

『 알고리즘 5.7     0-1 배낭 채우기 문제를 푸는 되추적 알고리즘

문제 : 무게와 값어치가 주어진 nA] 아이템이 있다고 하자. 무게와 같어치는 양의 정수
이다. 게다가 양의 정수 We 주어진다. 무게의 합이 가 넘지 못한다는 제약 하에서 총
값어치가 최대가 되는 아이템의 집합을 구하시오.

입력 : 양의 정수 nah 1 배열 wot p, 인덱스의 범위는 1부터 7,까지이고, 각 배열은
plil/wli) tel 따라서 큰 수부터 차례로 정렬된 양의 정수를 포함한다.

출력 : WS bestset, 여기서 인덱스의 범위는 1부터 /까지이고, 469296021의 값은 ia
아이템이 최적의 해에 포함되어 있으면 768 이고, 그렇지 않으면 'ㅁ0'이다; 최대 값어치를
나타내는 정수 maxprofit,

void knapsack (index 2
int profit, int weight)

{
if (weight <= W && profit > maxprofit) {      // 지금까지는 이 집합이 최고이다.
maxprofit = profit ;
numbest = i;                                // numbest& 고려한 아이템의 개수로
bestset = include ;                        // 놓고, bestset& 이 해답으로 놓는다.

}



===== PAGE 243 =====
00000 0 0
230   chapter 5 되추적

if (promising{i) {

includeli+1] = “yes”;                   // 퍼가] 포함
knapsack(i+1, profit + pli+1], weight + w{i+1));
include[i+1] = “no”;                   // wli+l1] 비포함
knapsack(i+1, profit, weight);
}
}
bool promising (index 1)
{
index j, k;
int totweight ;
float bound ;
if (weight >= W)                   // 자식마디로 확장할 수 있을 때만 마디는 유망하다.
return false ;                     // 자식마디에 BS 공간이 남아 있어야 한다.
else {
fe fas 1:
bound = protit ;
totweight = weight ;
while (7 <= n && totweight + wy) <= W) { // 가능한 한 BS 아이템을 취한다.
totweight = totweight + wl;
bound = bound + p\j\;
Yaa
}
k = /                     // 교재에서 사용한 식과 일관성을 유지하기 위하여 & 사용
부위               // kal 아이템의 일부분을 취함
bound = bound + (W- totweight) * p|k\/w\k;
return bound > maxprotfit ;
}
}

습에 따라서 n, w, p, 11, maxprofit, include, bestset, numberbest= 위의 두

루틴에 입력이 아니다. 만약 이 변수를 전역적으로 정의하면, 다음 SES 최대 수익(값
어치)과 그 수익을 만들어 주는 아이템의 집합을 US 것이다.

numbest = 0;

maxprotit = 0;

Kanpsack({0, 0, 0);

cout << maxprofit ;                     // 최대 값어치를 출력한다.

for (/ = 1; / <= numbest; j++)             // 최적이 되는 아이템의 집합을 보여준다.

cout << bestset| 1];

상태공간트리의 잎의 한계는 maxprofithu S 수가 없기 때문에 잎들은 모두 자동적
으로 유망하지 않았다. 따라서 함수 promising A) i = 인 최종 조건을 검사할 필요가


===== PAGE 244 =====
@0@000000
5.7 O-1 배낭 채우기 문제    231

없다. 이 알고리즘은 이 점검이 필요하지 않음을 확인해보자. i= no}, bound= 초기
값 profit|A| 변하지 않는다. profit? 224177070?보다 작거나 같으므로, 표현식 bound
> maxprofit<- 19186이다. 이는 함수 promising™ 19180이다.

수준 *에 위치한 마디에 도달할 때까지 반복하여 상태공간트리에서 윈쪽으로 나아가
므로 상한은 값이 변하지 않는다(예제 5.6에서 처음 몇 단계를 다시 보면 알 수 있다).
따라서 《같이 정해질 때마다 그 값을 저장하고, 수준 *- 1에 위치한 마디에 도달할 때까
지 promising 함수를 호출하지 않고 왼쪽으로 나아갈 수 있다. kal 아이템을 포함하면
총 무게가 WE 넘어가기 때문에 이 마디의 왼쪽 자식마디는 유망하지 않음을 안다. 따
라서 이 마디에서는 오른쪽으로만 간다. 오른쪽으로 움직인 후에만 함수 promising
호출하고, *의 새로운 같을 결정할 필요가 있다. 연습문제로 이와 같이 개선된 알고리즘
을 작성해보자.

O-1 배낭 채우기 문제에서 상태공간트리는 부분집합의 합 문제와 같다. 5.4절에서 보

여준 대로, 그 트리의 마디의 개수는 다음과 같다.
나가 il

알고리즘 5.72 다음과 같은 사례들에 대해서 상태공간트리에 있는 마디를 모두 검사한
다. 주어진 nol] 대해서 1^=7이라 하고,

최적의 해는 /째 아이템만 취하는 것이고, 깊이가 n— 1이 되는 곳까지 계속 오른쪽으로
간 뒤 왼쪽으로 갈 때까지 이 해답을 찾지 못한다. 그러나 최적의 해를 찾기 전에 잎이
아닌 마디는 모두 유망하게 되는데, 이는 상태공간트리에 있는 마디는 모두 검사를 하게
된다는 뜻이다. 몬테칼로 기술을 이 문제에 사용하여 특정 사례에 대해서 알고리즘의 효

ㅇ_으 Zz  = ~
율을 추정할 수 있다.

5.7.2 O-1 배낭 채우기 문제를 푸는 동적계획 알고리즘과 되추적 알고리즘의 비교
4.4절에서 0-1 배낭 채우기 문제를 푸는 동적계획 알고리즘으로 계산하는 최악의 경우
엔트리의 개수는 O(minimum(2", 7117)이었음을 상기하자. 최악의 경우 되추적 알고
리즘은 O(2") 마디를 검사한다. 추가적인 한계 nw 덕분에 동적계획 알고리즘이 더 좋
은 것처럼 보일는지도 모른다. 그러나 되추적 알고리즘에서 최악의 경우를 따지면 실제
로 되추적 알고리즘으로 점검하는 NES 얼마나 절약하게 되는지 별로 반영하지 못한
다. 고려해야 할 사항이 너무 많아서 이 두 알고리즘의 상대적인 효율을 이론적으로 분석
하기는 어렵다. 이런 경우 많은 사례를 가지고 알고리즘을 직접 실행해 보고, 어떤 알고
리즘이 더 좋은지 알아보아 비교할 수 있다. Horowitz} 806010978/가 이 실혐을 했는



===== PAGE 245 =====
@00@00000 0
232    chapter 5 되추적

데, 되추적 알고리즘이 동적계획 알고리즘보다 보통 더 효율적임을 알아냈다.

Horowitz} Sahni(1974)%= 분할정복법을 동적계획법과 결합하여 최악의 경우 O(2"/”)
인 0-1 배낭 채우기 알고리즘을 개발하였다. 그리고 이 알고리즘이 보통 되추적 알고리
즘보다 보통 더 효율적임을 보였다.

@ ase

5.1절과 5.2절

1. 문제 사례가 7=6이고 N=7 경우 JRA 알고리즘을 사용하여 7-여왕말 문제의 해답
을 각각 두 개씩 구하시오.

2. ＊-여왕말 문제를 푸는 되추적 알고리즘(알고리즘 5.1)을 문제 사례가 7=8인 경우 적용시
켜 보고, 그 실행과정을 단계별로 보이시오. 첫째 HPS 찾을 때까지 이 알고리즘이 만드는
가지친 상태공간트리를 그리시오.

3. 프로시저 checknode 대신 expands 사용하여 7-여왕말 문제를 푸는 되추적 알고리즘을
작성하시오.

4. 입력으로 정수 7을 받아서 7-여왕말 문제의 해가 몇 개인지 구하는 알고리즘을 작성하시오

5. ㅠ=4인 경우 되추적 없이 7-여왕말 문제를 풀면 첫째 HAS 찾기 전에(그림 5.4에서 27개
마디를 검사해야 하는 것과는 대조적으로) 155마디는 반드시 검사해야 한다는 사실을 보이
세우.

6. ㅠ-여왕말 문제(알고리즘 5.1를 푸는 되추적 알고리즘을 구현하는 프로그램을 작성하고,
n=4, 8, 10, 19인 문제 ARIS 가지고 실행시켜 보시오.

7. 유망함수가 이미 we 여왕말에 의해서 조절되는 열의 aA, 왼쪽 대각선의 We, 오른쪽

대각선의 집합을 기록하게 하여 7-여왕말 문제(알고리즘 5.1를 푸는
개선하시오.

8. 가능한 해답을 모두 생성하는 대신 해답을 하나만 찾도록 /-여왕말 문제(알고리즘 5.1를

추적 알고리즘을

9. ㅠ-여왕말 문제에서 7=4인 문제 사례에 대한 해답을 가지고 있다고 가정하자. 이 해답을
확장하여 ㅠ=5인 문제 사례에 대한 해답을 찾고, =4와 ㅠ=5에 대한 해답을 가지고
ㅠ=6인 사례에 대한 해답을 구축하고, 이 동적계획법을 계속 사용하여 n> 4인 어떤 사례
에 대한 해답을 찾을 수 있을까? 그리고 왜 그런 답이 나오는지를 밝히시오.

10. 7-여왕말 문제에서 해답이 존재하지 않는 사례를 최소한 두 가지 찾으시오.

5.3절

11. 알고리즘 5.30/-여왕말 문제를 푸는 되추적 알고리즘에 대한 몬테칼로 추정치 구하기)을
구현하는 프로그램을 작성하고, 7 =8인 문제 사례에 90번 실행시켜서 2071 추정치의 평균
을 구하시오.

fl



===== PAGE 246 =====
@ee
연습

0
N
o
o

12. n-FH9 문제를 푸는 되추적 알고리즘(알고리즘 5.1)을 문제의 사례에 대하여 점검하는
마디의 개수를 AES 수정하고, 그 알고리즘을 7=8인 문제 사례에 실행시키고 연습문제
9번의 평균과 이 결과를 비교하시오.

5.4절

13. 부분집합의 합 구하기 문제를 푸는 되추적 알고리즘(알고리즘 5.4)을 사용하여 다음 숫자의
조합 중에서 합이 『=52가 되는 조합을 모두 찾으시오.

wy=2 w.=10  406=18  44=17 w,=22 106 = 42

실행 절차를 단계별로 보이시오.

14. 부분집합의 합 구하기 문제를 푸는 되추적 알고리즘(알고리즘 5.4)을 구현하는 프로그램을
작성하고, 연습문제 U9] 문제 사례를 가지고 실행하시오.

15. 사전에 무게를 정렬하지 않고, 부분집합의 합 구하기 문제를 푸는 되추적 알고리즘을 작성
하시오. 이 알고리즘의 성능을 알고리즘 5.4의 성능과 비교하시오.

16. 가능한 해담을 모두 생성하는 대신 하나의 alae 찾도록 부분집합의함 구하기 문제를
는 되추적 알고리즘(알고리즘 5.4)을 수정하시오. 알고리즘 5.4와 비교ㅎ
떤가?

17. 몬테칼로 알고리즘을 사용하여 부분집합의 합 구하기 문제를 푸는 되추적 알고리즘(알고리
즘 5.4/의 BSS 추정하시오.

5.5절

18. ㅠ-색칠하기 BAS 푸는 되추적 알고리즘(알고리즘 5.5/을 사용하여 빨간색, 녹색, 흰색의
3가지 종류의 색을 가지고 아래 그래프를 색칠하는 모든 방법을 찾으시오. 실행절차를 단계
별로 보이시오.

럭                                  ^ ^                                  V3

2

Vi

19. 그래프를 적절히 색칠하기 위해서 가능한 한 많은 AAS 색칠하도록 출발 정점과 색을 하
나 선택한다고 하자. 그리고는 가능한 한 많은 정점을 추가적으로 색칠하도록 새로운 색과
색칠되지 않은 새로운 정점을 선택한다. 그래프의 모든 정점이 색칠되거나 색이 모자랄 때
까지 이 과정을 계속 반복한다. 이 탐욕적 방법으로 정점이 개인 그래프를 색칠하는 알고

알고리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

20. 연습문제 19의 알고리즘을 사용하여 연습문제 18의 그래프를 색칠하시오.

21. 그래프를 색칠하는데 사용한 색의 개수를 최소화하고 싶다고 가정하자. 연습문제 19의 탐욕
적 방법이 최적의 해를 보장해 주는가? 그리고 왜 그런 답이 나오는지를 밝히시오.



===== PAGE 247 =====
234

chapter 5 되추적

22. 8-색칠하기 되추적 알고리즘이 그래프가 3색으로 칠할 수 RSS 알아내는데 지수시간이
걸리는 정점이 개 있는 연결된 그래프를 그리시오.

28. ㅠ-색칠하기 문제를 푸는 되추적 알고리즘(알고리즘 5.8)과 연습문제 199) Ga} 알고리
교하시오. 비교 결과와 연습문제 199] 답을 고찰해 본 후 왜 탐욕적 방법을
Re 한 알고리즘을 사용하는 데 BIS 가지게 될지 이유를 서술하시오
24. 시간복잡도가 최악의 경우 7에 대해서 지수가 아닌 8-색칠하기 BAS 푸는 알고리즘
작성하시오
25. ㅠ-색칠하기 문제의 형식으로 표현 가능한 실제 응용사례를 몇 개 들어보시오

시

으

fl

564
26. WIE 회로 문제를 푸는 되추적 알고리즘(알고리즘 5.6)을 사용하여 다음 그래프의 해밀튼
회로를 모두 찾으시오.

oS
a7

lta
of
fd!

절차를 단계별로 보이시오.

27. ALE 회로 문제를 푸는 되추적 알고리즘(알고리즘 5.0)을 구현하는 프로그램을 작성하고
연습문제 239] 문제 ARIS 가지고 실행하시오.
28. 연습문제 34에서 구현한 해밀튼 회로 문제를 푸는 되추적 알고리즘(알고리즘 5.0)의 출발
성준 2

JS 바꾸고, 알고리즘 5.6과 그 성능을 비교하시오.

u

!
|

ov

29. 가능한 해답을 모두 생성하는 대신 하나의 해답만 ALS 해밀튼 회로 문제를 푸는 되추적
알고리즘(알고리즘 5.6)을 수정하시오. 알고리즘 5.6과 비교하여 수

30. 해밀튼 회로 BAS 푸는 되추적 알고리즘(알고리즘 5.6)을 분석하고, 차수 표기법으로 최
악 복잡도를 구하시오.

31. 몬테칼로 기술을 사용하여 해밀튼 회로 문제를 푸는 되추적 알고리즘(알고리즘 5.6)의 효율
을 추정하시오.

5.7절

32. 예제 5.665.7.1절)에서 마디 (4, 1)을 방문한 후 남은 값과 한계를 계산하시오.

33. 0-1 배낭 채우기 BAS 푸는 되추적 알고리즘(알고리즘 5.7)을 사용하여 다음 문제 사례에
서 수익을 최대로 하시오. 실행절차를 단계별로 보이시오.


===== PAGE 248 =====
연습문제      235
Wy
1     $20     2     $10
2     $30     5     $6
3}     $35     7     $5 W=9
4     $12     3     $4
5     $ 3     1     $ 3
34. 01 배낭 채우기 문제를 푸는 되추적 알고리즘(알고리즘 5. NS 구현하는 프로그램을 작성

하고, 연습문제 88의 문제 사례를 가지고 실행하시오.
35. 0-1 배낭 채우기 BAS 푸는 동적계획 알고리즘(4.4.8절)을 구현하는 프로그램을
고, 이 알고리즘의 성능을 0-1 배낭 채우기 BAS 푸는 되추적 알고리즘(알고리즘 5.7)과

큰 문제 사례를 가지고 비교하시오.

36. 오른쪽으로 간 후에만 유망 함수를 호출하여 0-1 배낭 채우기 문제를 푸는 되추적 알고리즘
(알고리즘 5.7)을 개선하시오.
37. 몬테칼로 기술을 사용하여 0-1 배낭 채우기 BAS 푸는 되추적 알고리즘(알고리즘 5.7)의

BRS 추정하시오,

추가적인 연습문제

SC Ce:

38. 되추적의 응용사례를 3가지 더 나열하시오

39. 대칭(0604600008)이나 회전(6068400)에도 불변(.ㅁ7811821)하는 해답만 결과로 내주도록, n
여왕말 문제를 푸는 되추적 알고리즘(알고리즘 5.1)을 수정하시오.

40. 7/"개의 셀(691)을 가진 nxnXn 정육면체(6468)가 주어지고, 서양장기(2.689)의 어떤 두

여왕말(400688'도 서로 위혐하지 않도록(즉, 어떤 두 여왕말과 같은 행이나, 열이나. 대각선

에 오지 않도록) 그 정육면체에 7개의 여왕말을 놓으려고 한다. /-여왕말 문제를 푸는 알

고리즘(알고리즘 .1을확장하여 이 BAL 풀 수 있을까? 만약 그렇다면, 그 알고리즘을

작성하고, 그 알고리즘을 구현하는 프로그램을 작성하여 7=4이고 7=8인 문제 사례의 해
답을 구하시오.

41. 길이가 일정하지 않은 리스트를 가지고 해답을 구할 수 있도록 부분집합의 합을 구하는 되
추적 알고리즘(알고리즘 5.4을 수정하시오.

42. 열습문제 0! = ithe 갤은 all 모이는 이음선들
으

베

A 이용할 수 주 있는지 설명하시오.

43. 가중치 그래프에서 최소비용을 가진 PLE 회로를 찾을 수 있도록 해밀튼 회로 문제를 푸
는 되추적 알고리즘(알고리즘 5.0/을 수정하시오. 작성한 알고리즘의 성능은 어떤가?

44. 길이가 일정하지 않은 리스트를 가지고 해답을 구할 수 있도록 01 배낭 채우기 문제를 푸

[=
되추적 알고리즘(알고리즘 5.7)을 수정하시오.

flr aN


===== PAGE 249 =====
Chapter 6

분기한정법

0    그 배낭 채우기 문제를 푸는 알고리즘인 동적계획 알고리즘(4.4절)과 되추적 알

고리즘(5.7절)을 모두 밤손님에게 제공해 보았다. 이 두 알고리즘 모두 최악의

우 지수시간이 걸리므로, 밤손님이 문제를 푸는데 어떤 알고리즘을 사용하더라도 수년

이 걸린다. 이 장에서는 27]8b9 a (branch-and—bound)o]#}31 하는 또 다른 방법을 밤

손넘에게 제공한다. 앞으로 알게 되겠지만, 여기서 이태    기한정 알고리즘은 되추

적 알고리즘을 개선한 것이다. 따라서 비록 다른 두 알고리즘들이 밤손님 문제를 효율

적으로 해결하지 못했지만, 분기한정 알고리즘은 아마도 해결할 수 수 있을지 모르니 기대
해보자.

분기한정 설계전략은 상태공간트리를 사용하여 문제를 푼다는 사실이 되추적과 매우
비슷하다. 차이점으로 분기한정법은 (1 트리 횡단방법에 구야받지 않고, (2) 최적화 문제
를 푸는데 만 쓰인다. 분기한정 알고리즘은 어떤 마디가 유망한지를 결정하기 위해서 그
마디에서 수(한계값)를 계산한다. 이 수는 그 마디 아래로 확장하여 구할 수 있는 해답
값의 한계(60000)를 나타낸다. 그 한계값이 그때까지 찾은 최고 해답 값보다 더 좋지 않
으면 그 마디는 유망하지 않다(ㅁ0ㅁ2『0048109). 그렇지 않으면 그 마디는 유망하다(600-



===== PAGE 250 =====
238

chapter 6 분기한정법

때8109). 최적값은 문제에 따라서 최대값이 될 수도 있고, 최소값이 될 수도 있으므로 여
기서 “SCP SE 문제에 따라서 더 작다는 의미도 되고 더 크다는 의미도 된다. 되추적 알고
리즘의 경우와 마찬가지로 분기한정 알고리즘은 최악의 경우 보통 지수시간이다(또는 이
보다 더 나쁘다). 그러나 큰 사례에서 매우 효율적일 수가 많이 있다.

O-1 배낭 채우기 BAS 푸는 5,749] 되추적 알고리즘은 사실 분기한정 알고리즘이
다. 그 알고리즘에서 한계값이 24410704/의 현재 값보다 크지 않다면 유망 함수는 false
를 넘겨준다. 그러나 되추적 알고리즘은 분기한정을 사용하여 얻을 수 있는 장점을 제대
Al

방문한다. 이렇게 하면 (깊이우선검색같이) 미리 정한 순서대로 마디를 방법론적으로 방
문하는 것보다 더 빨리 최적해에 도달할 수 있다. 이 방법을 분기한정 가지치기 최고우선
검색(668+-[118{ search with branch—and—bound 20047012708)이라고 한다. 이 HRY 분기
한정 가지치기 너비우선검색(67680111-[118{ search with branch—and—bound pruning)°]
라고 하는 또 다른 하나의 방법론적인 접근법을 간단히 수정하여 구현할 수 있다. 따라서
비록 깊이우선검색에 비해서 이점은 없지만 너비우선검색으로 0-1 배낭 채우기 문제를
먼저 6.1절에서 풀어본다. 이렇게 하면 최고우선검색을 더 쉽게 설명할 수 있고, 이를 이
용하여 0ㄱ1 배낭 채우기 BAS 푼다. 6.2절과 6.8절에서 최고우선검색을 적용할 수 있
는 두 가지 문제를 더 살펴본다.

더 진도 나가기 전에 너비우선검색을 복습해보자. 트리의 경우 너비우선검색0606804Ｌ
—first 868700/은 뿌리마디를 먼저 방문하고, 다음에 수준 1의 마디를 모두 방문하고, 다

ㅇ
음에 수준 29] WS 모두 방문하고, SS 이런 ALE 계속한다: 원쪽에서 오른쪽으로

그림 6.1 트리의 너비우선검색. 마디들은 방문하는 순서대로 번호가 매겨져 있다. 자식마디들은
왼쪽에서 오른쪽으로 방문한다.



===== PAGE 251 =====
06000000
61 분기한정을 0-1 배낭 채우기 문제로 설명하기   239

진행하는 경우 트리의 너비우선검색을 그림 6.1에서 보여준다. 이 그림에서 마디들은 방
문하는 순서대로 번호가 매겨진다.

깊이우선검색과는 달리 너비우선검색을 하는 재귀 알고리즘은 작성하기 어렵다. 그러
나 대기열(04606/을 사용하여 아래 알고리즘과 같은 방식으로 구현할 수 있다. enqueue
라는 프로시저로 대기열의 뒤에 아이템을 붙여 넣고, 0000000라는 프로시저로 앞에서
아이템을 제거한다.

void breadth_ 70797 tree_search(tree T);

{

queue_of_node Q;

node u, v;

initialize( Q);                           // OF 빈 대기열로 초기화

v = root of 7;

visit v;

enqueue Q, v);
while(! empty(Q)) {
dequeue(Q, v);
for (each child wu of v) {
visit u;
enqueue(Q, u);

}
}
}
이 프로시저만으로 너비우선검색이 잘 이해되지 않으면, 그림 6.12] 트리에 이 알고리
즘을 적용하여 따라가 보도록 하자. 앞에서 말했듯이 이 트리에서 자식마디는 왼쪽에서
오른쪽으로 차례로 방문한다.
@ 61 분기한정을 0-1 배낭 채우기 문제로 설명하기
0-1 배낭 채우기 문제에 분기한정 설계전략을 어떻게 사용하는지 살펴보자. 먼저 분기한
정 가지치기 너비우선검색이라는 간단한 알고리즘을 먼저 살펴본 후 분기한정 가지치기
최고우선검색을 공부한다.
6.1.1 분기한정 가지치기 너비우선검색
예제를 통하여 이 방법을 설명한다.
© 예제 6.1      예제 5.6에서 본 O-1 배낭 채우기 문제의 사례를 그대로 사용한다. S, n=4, W=160]31 가져

갈 수 있는 아이템의 내역이 다음과 같다고 가정하자.


===== PAGE 252 =====
240

chapter 6 분기한정법

;                                          P;
2              Pi             Ww;           도
WwW;
1            $40             2           $20
2,            $30             5           $6
3            $50           10           $5
4

$10            5          $ 2

예제 5.62} 같이 아이템들은 p,/w, 값에 따라서 이미 정렬되어 있다. 분기한정 가지치기 너비우
선검색은 깊이우선검색 대신 너비우선검색을 하는 것을 제외하고 예제 5.6에서의 되추적 방법과
똑같은 방법으로 진행한다. 즉, weight profit 그 마디에 오기까지 포함되었던 아이템의 총
무게와 총 이익으로 한다. 마디가 유망한지 결정하기 위해서 cotweightSt 40000를 weights}
profit © 2 각각 초기화하고, 그 다음 totweight7} WE 초과하게 하는 아이템에 도달할 때까지
탐욕적으로 아이템을 취하여 그 무게와 이익을 totweight9} boundd 각각 더한다. 배낭에 넣
을 수 있는 만큼만 그 아이템의 일부분을 취하여 그 BHO} woightS cotweightol| 더한다. 이런
식으로 hounds 그 마디에서 확장하여 얻을 수 있는 이익의 상한이 된다. 만약 그 마디가 수준
;에 위치하고 있고, 수준 ko} 위치한 마디는 무게의 합이 「까 넘어가는 마디라고 하자. 그러면,
다음과 같은 식을 얻는다.

k-1
totweight = weight + > Ww;
2=1+1

bound = | profit +  >) P; 「 ( W-totalweight) x a
jaitl                                 k
지금까지 찾은 최고 해답에서의 값인 maxprofitssc} 이 한계값이 작거나 같으면 그 마디는 유망
하지 않다. 다음 부등식이 성립해도 마디는 유망하지 않다.
weight > W

이 사례를 가지고 너비우선검색을 하여 만든 가지친 상태공간트리(위쪽에 표시된 한계값을 사용
하여 가지를 침)는 그림 6,20] 나와 있다. profit, weight, 40040의 값은 각 마디에 위에서 아래
로 표시한다. 음영 처리된 마디는 최대 이익을 찾은 마디를 나타낸다. 마디는 트리의 왼쪽으로부
터 수준과 위치에 따라서 라벨을 위쪽에 붙인다.

이 절차는 예제 5.6에서 본 것과 비슷하므로 다시 반복하지는 않고 중요한 요점 몇 가지만 언급
한다. 마디는 그 마디가 위치한 수준과 왼쪽에서부터의 위치로 표시한다. 먼저 마디 (3, 1)과 (4,
9)은 한계값이 80임을 주목하자. 분기한정 알고리즘은 어떤 마디에서 확장 여부를 결정할 때 지
금까지 구한 답 중에서 가장 좋은 값보다 한계값이 더 좋은지 검사한다. 따라서 가중치가 Wet
다 작지 않아서 마디가 유망하지 않게 되면 한계값을 $0로 놓는다. 이런 식으로 하면 한계값이
지금까지 구한 답보다 더 좋을 수 없다고 보증할 수 있다. 다음, 이 문제를 가지고 되추적(깊이
우선 검색)할 때 마디 (1, 9)가 유망하지 않음을 알아냈고, 그 마디 oppose 확장하지 않았다.

그러나 너비우선검색의 경우 이 마디는 방문하는 번째 마디가 된다. 이 마디를 방문할 때
maxprofit?| 값은 $40 밖에 되지 않는다. 이 시점에 한계값 $827} maxprofit 값을 넘기 때문에
그 마디 이후에도 계속 확장한다. 마지막으로 분기한정 가지치기 단순 너비우선검색에서는 어떤
마디의 자식마디를 방문해야 할지는 그 마디를 방문할 때 결정한다. 즉, 자식마디로 Be 가지는



===== PAGE 253 =====
06000000
61 분기한정을 0-1 배낭 채우기 문제로 설명하기   241

(0, 0)

(3, 4)

(3, 5)

(4,2) (4,3)

그림 6.2 예제 6.1014 분기한정 가지치기 너비우선검색을 하여 만든 가지친 상태공간트리. 24
마디에 저장하는 USE 위에서 아래로, 그 마디까지 S%! al 으어 총 이익, 총 무게, 그리고 그
마디에서 확장하여 얻을 수 있는 총 이익의 한계값이다. 음영 처리된 마디가 최적  의 해답을 찾은
마디이다.

그 마디를 방문할 때 친다. 따라서 마디 (2, 3S 방문할 때 그 마디의 한계값은 $82인 반면,
maxprofit 값은 $70 밖에 되지 않기 때문에 그 자식마디를 방문하기로 결정한다. 깊이우선검색
과는 달리 너비우선검색에서는 maxprofit2| 값이 자식마디를 실제로 방문하는 때에 변해버릴
수 있다. 이 예의 경우 228270/4/은 마디 (2, 8)의 자식마디를 방문할 때 $900] 된다. 이렇게
되면 이 자식마디를 검사하는 시간을 낭비하게 된 셈이다. 다음 절에서 설명하게 될 최고우선검
색에서는 이를 피한다.

이제 이 기술을 설명했으니 분기한정 가지치기 너비우선검색을 하는 일반 알고리즘을
살펴보자. 이 범용 알고리즘의 입력으로 상태공간트리 TS 언급하지만, 실제로 사용할
때 상태공간트리는 묵시적으로만 존재한다. 이 문제의 파라미터는 이 알고리즘의 실제
입력이고, 상태공간트리 7'를 구한다.

void breadth_first_ branch_and_ bound (state_space_tree T,

{

number& best)

queue_of_node Q;


===== PAGE 254 =====
@0600000 0
242   chapter 6 분기한정법

node u, =;
initialize( Q);                           // @= 빈 대기열로 초기화
v = root of T;                          // 뿌리마디를 방문

enqueue(Q, v);
best = value(v);
while (! empty(Q)) {
dequeue(Q, v);
for (each child wu of v) {                   // 각 자식마디를 방문
if (value(u)7} 2697보다 좋다)
best = value(u);
if (bound(u)7} bestt} 좋다)
enqueue(Q, u);

}
}
}
이 Bae 이 장 시작 작 부분에서 소개한 너비우선검색 알고리즘을 수정한 것이다.
그러나 이 알고리즘에서는 마디의 한계값이 당시 최고 argo) 값보다 좋은 경우에만 그
마디에서 계속 확장한다(자식마디를 방문한다). 당시 최고 해답의 값(변수 best) 뿌리
마디에서의 해답의 값으로 초기화한다. 경우에 따라서 해답을 얻기 위해서 상태공간트리
의 잎까지 도달하기도 해야 하기 때문에 뿌리마디에 해답이 없는 경우도 었다. 그런 경우
에는 best 값을 어떤 해답보다도 나쁜 값으로 초기화한다. breadth_first_ branch_and
_ 20000를 어디에 사용하는가에 따라서 함수 bound} 144/6는 달라진다. 앞으로 보게
되겠지만, 14406 함수는 실제로 작성하지는 않는 게 보통이다. 그 WL 바로 계산하다.
이제 0-1 배낭 채우기 문제를 푸는 알고리즘을 살펴보자. AAS 사용하는 이점이 사
라졌으므로(재귀 호출 시 만들어졌던 새로운 변수가 없다는 의미), 그 마디에 관련된 모
는 BES 그 마디에 저장해야 한다. 따라서 이 알고리즘에서 마디의 타입은 다음과 같다.
struct mode
i
int level;                // 트리에서 마디의 수준
int profit ;
int weight ;
}
> 알고리즘 6.1     O-1 배낭 채우기 SAS 푸는 분기한정 가지치기 너비우선검색 알고리즘

문제 : 무게와 이익이 주어진 7/개의 아이템이 있다고 하자. 무게와 이익
게다가 양의 정수 We 주어진다. 무게의 합이 W7 넘지 못한다는 Ao
이 최대가 되는 아이템의 집합을 구한다.

입력 : 양의 정수 과 Ws 양의 정수의 배열 wt p, 인덱스의 범위는 1부터 /까지이고,



===== PAGE 255 =====
@000000 0
6.1 분기한정을 0-1 배낭 채우기 문제로 설명하기    243

각 HSS plil/wli] el 따라서 큰 수부터 차례로 정렬되어 있다.
출력 : 최적의 집합에 있는 이익의 합을 나타내는 정수 maxproft
void knapsack? (int 22,
const int p[], const int w/],

int W,
int& maxprofit)

{
queue_of_node Q;
node 2, v;
initialize Q);                               // QS 빈 대기열로 초기화

v.devel = 0; v.profit = 0; v.weight = 0;         // v7} 뿌리마디가 되게 초기화
maxprotit = 0;
enqueue(Q, v);
while (! empty(Q)) {
dequeue(Q, v);

u.level = v.level + 1;                     // u& v2] 자식마디로 놓음
u.weight = v.weight + w{u.level;               // 를 다음 아이템을 포함하는
u.profit = v.profit + plu.level;               // 자식마디로 놓음

if (u.weight <= W && u.profit > maxprofit)
maxprofit = u.protit ;

if (bound(u) > maxprofit)
enqueue(Q, wu);

u.weight = v.weight;                         // oS 다음 아이템을 포함하지 않는
u.profit = v.profit ;                         // 자식마디로 놓음

if (bound(u) > maxprofit)
enqueue Q, u);
}

i

float bound(node u)
{
index j, 4;
int totweight ;
float result ;

if (u.weight >= W)
return 0;
else {
result = u.profit ;
J = u.level + 1;
totweight = u.weight ;
while (j <= 2 && totweight + wij] <= W) { // 가능한 한 많은 아이템을 취한다.
totweight = totweight + w\J];
result = result + pl jj;
Fane


===== PAGE 256 =====
@‥00000 0
244   chapter 6 분기한정법

}

k= /;                           // 본문에서 사용한 식과 일관성을 유지하기 위하여 《 사용
if (k <= »)                 // KA 아이템의 일부분을 취함

result = result + (W- totweight) * p| k|/w{ k];
return result ;

© 예제 6.2

현재 아이템을 포함하지 않고 w.profit©) maxprofits 초과하는지 검사할 BRE 없
다. 왜냐하면, 이 경우 2.27072은 uo] 부모마디와 관련된 이익이고, 따라서 maxprofit
을 초과할 수 없기 때문이다(그림 6,20] 그려진 것 같이). 마디의 한계값은 마디에 저장할
Bart 없다. 왜냐하면, 그 값을 maxprofity} 비교한 후에는 한계값이 더 이상 필요 없
기 때문이다.

함수 bound= 알고리즘 5.7의 함수 promising} 본질적으로 같다. 차이는 분기한정
알고리즘을 만들기 위한 지침에 따라서 bounds 작성했고, 따라서 bound= APS 넘
겨주는 반면, 함수 promising= 되추적 지침을 따라서 작성했으므로 E(boolean) 값을
넘겨준다. 우리의 분기한정 알고리즘에서 2741770/7과의 비교는 호출하는 프로시저에
의해서 이루어진다. 이 경우 bound7} 넘겨주는 값은 22412704보다 작거나 같기 때문에
(이 마디는 큐에 넣지 않음을 의미), 함수 bound i=n 조건을 검사할 BRE 없다.

알고리즘 6.1로 아이템의 최적 집합이 만들어지지 않는다. 단지 최적의 집합에 속한
이익의 합만 구한다. 알고리즘은 최적의 집합을 만들어 내도록 다음과 같이 수정할 수
있다. 각 마디에서 그 마디에 이르기까지 포함된 아이템의 집합인 77626라는 변수를 저
장하고, 당시 최고 아이템의 AWS 나타내는 변수 LestitemsS 유지한다. 27417707을
u.profits| 같게 놓으면 /6977700229 u.items2} 같게 놓는다.

6.1.2 분기한정식 가지치기 최고우선검색

일반적으로 너비우선검색 AS 깊이우선검색(되추적)보다 좋은 점이 없다. 그러나 마
디의 유망성 여부를 결정하는 것 이외에 추가적인 용도로 한계값을 사용하면 검색을 향
상시킬 수 있다. 주어진 어떤 마디의 모든 자식마디를 방문한 후 유망하면서 확장하지
않은 마더들을 모두 살펴보고 그 중에서 한계값이 가장 좋은 마디를 우선적으로 확장한
다. 지금까지 찾은 최고의 해답보다 그 한계값이 더 좋다면 그 마디는 유망하다. 미리
정해 놓은 순서대로 무작정 검색을 진행하는 것보다 이런 식으로 하면 최적해를 더 빨리
찾게 된다. 다음 예제에서 이 방법을 설명한다.

예제 6.1의 0-1 배낭 채우기 문제 사례를 다시 한 번 생각해보자. 최고우선검색을 하면 그림 6.3
의 상태공간트리가 그려진다. 이익, 무게, 한계값은 여기서도 위에서 아래로 트리의 각 마디에
표시된다. 음영 처리된 마디가 최대 이익을 찾은 마디이다. 이제 이 트리를 구축하는 절차를 살



===== PAGE 257 =====
06000000
6.1 분기한정을 0-1 배낭 채우기 문제로 설명하기   245

(0, 0)

그림 6.3 예제 6.2014 분기한정 가지치기 최고우선검색을 하여 만든 가지친 상태공간트리. 각
마디에 저장하는 WSS 위에서 아래로, 그 마디까지 SFI 아이템의 총 이익, 총 무게, 그리고 그
마디에서 확장하여 얻을 수 있는 총 이익의 한계값이다. 음영 처리된 마디가 최적의 해답을 찾은

마디이다.

펴보자. 여기서도 마디는 트리에서 그 마디의 수준과 왼쪽 마디로부터 위치를 가지고 나타낸다.
값과 한계값은 예제 5.6과 6.1과 같은 방법으로 계산한다. 절차를 밝아 가는 동안 계산은 보여주
지는 않는다. 더구나, 마디가 유망하지 않다고 판명되는 경우만 언급하고, 유망하다고 판명되는
경우는 언급하지 않는다.
검색 절차는 다음과 같다.
1. 마디 (0, 0)(뿌리마디)를 방문한다.
(8) 이익과 무게를 $0과 0으로 놓는다.
09) 한계값을 계산하면, $115가 된다(계산 절차는 예제 5.6을 보시오).
(0) maxprofit® 0으로 놓는다.
2, 마디 (1, 1)을 방문한다.
(a) 이익과 무게를 계산하면, $40과 2가 된다.
(b) 무게 2는 1/의 값 16보다 작거나 같고, 이익 $40은 $0보다 크므로, maxprofit?| 값을
$40로 놓는다.
(c) 한계값을 계산하면, $115가 된다.
8. 마디 (1, 9)를 방문한다.


===== PAGE 258 =====
246

chapter 6

10,

11,

12,

13,

, 마디 2, JS 방문한

. 마디 (8, JS 방문한

(a) 이익과 SAS 계산하면, $0과 00] 된다.
06) 한계값을 계산하면, $82가 된다.

. 아직 확장하지 않은 마디 중에서 가장 큰 한계값을 가진 유망한 마디를 구한다.

(a) 마디 01, 1은 한계값이 $1150]31, 마디 (1, 이는 한계값이 889이므로 마디 (1, 1이 한계값
이 가장 크면서 유망하고, 확장하지 않은 마디이다. 그 마디의 자식마더를 다음에 방문
한다.

. 마디 (2, 1)을 방문한다.

(a) 이익과 무게를 계산하면, $70과 7°] 된다.

(b) 무게 7은 We] 값 16보다 작거나 같고, 이익 $702 $40보다 ABS maxprofit?| 값을
$7022 놓는다.

(0) 한계값을 계산하면, $157} 된다.

(a) 이익과 FAS 계산하면, $40과 2가 된다.

06) 한계값을 계산하면, $98이 된다.

. 아직 확장하지 않은 마디 중에서 가장 큰 WAS 가진 유망한 마디를 구한다.

(a) 그 마디는 마디 (2, 1이다. 그 마디의 자식마디를 다음에 방문한다.

. 마디 (8, DS 방문한다.

(a) 이익과 무게를 계산하면, $1203} 170] 된다.

09 무게 17은 의 값 16보다 크거나 같으므로 이 마디는 유망하지 않다. 이 마디의 한계값
을 80으로 놓아서 유망하지 않게 한다.

(a) 이익과 무게를 계산하면, $00과 ?이 된다.

09 한계값을 계산하면, $800) 된다.

아직 확장하지 않는 마디 중에서 가장 큰 한계값을 가진 유망한 마디를 구한다.

(a) 그 마디는 마디 2, 9이다. 그 마디의 자식마디를 다음 방문한다.

마디 (3, 9)을 방문한다.

(a) 이익과 무게를 계산하면, $90과 127} 된다.

09 무게 12% WS] 값 16보다 작거나 같고, 이익 890은 870보다 크므로 244177048의 값을
890으로 놓는다.

(6 이 AMAA 마디 (1, 2)9} (8, 9'의 각 SARE $829} $80은 모두 새로운 maxprofit 값인
SOOT} 작거나 같으므로 그 마디들은 유망하지 않게 된다.

(0) 한계값을 계산하면, 898이 된다.

마디 (3, 4)를 방문한다.

(a) 이익과 무게를 계산하면, $40과 27} 된다.

(b) 한계값을 계산하면, $50이 된다.

아직 확장하지 않는 마디 중에서 가장 큰 한계값을 가진 유망한 마디를 구한다.



===== PAGE 259 =====
void best_ fit_

{

@0600000 0
6.1 분기한정을 0-1 배낭 채우기 문제로 설명하기    247

(a) 유일하게 확장되지 않고 남은 유망한 마디는 마디 (3, 3)이다. 그 마디의 자식마디를
다음 방문한다.
14. 마디 (4, DS 방문한다.
(a) 이익과 BAS 계산하면, $100과 17이 된다.
06) 무게 17이 의 값 16보다 크거나 같으므로 이 마디는 유망하지 않다. 그 한계값을 $2
로 놓는다;
15. 마디 (4, 2) 방문한다.
(a) 이익과 FAS 계산하면, $90과 127} 된다.
00) 한계값을 계산하면, $90이 된다.
(0) 한계값 890이 maxprofit2| 값 $90보다 작거나 같으므로 이 마디는 유망하지 않다고 A
정한다. 상태공간트리에서 잎마디들은 그 한계값이 maxprofit= 넘을 수 없으므로 자
동적으로 유망하지 않게 된다.

유망하고, 확장하지 않는 마디가 없으므로 작업이 완료되었다.

최고우선점색으로 1개 마디만 검사했는데, 이는 너비우선검색(그림 6.9:으로 검사한
마디의 수보다 6개 작고, 깊이우선검색(그림 5.14:으로 검사한 마디 수보다 8개 작다. 검
사하는 마디의 수를 8개 절약한 것은 별로 인상적이지 않지만, 큰 상태공간트리에서 최
고우선검색으로 최적해를 빨리 찾는 경우 차이는 꽤 심각할 수 있다. 그러나 최고라고
여겨지는 마디에서 최적해를 실제로 끌어낸다는 보장은 없다는 점은 주의해야 한다. 예
제 6.9에서 마디 (2, 10] 마디 (2, 9보다 더 좋은 것처럼 보였지만 마디 (2, 9)가 최적해
를 이끌어낸다. 일반적으로, 최고우선검색으로도 어떤 사례에 대해서는 상태공간트리 전
AS 거의 또는 모두 구축할 수밖에 없을 수 있다.

최고우선검색은 너비우선검색을 조금 변형시켜서 구현하면 된다. 대기열04646)을 A}
용하는 대신, 우선순위 대기열을 사용한다. 우선순위 C7] A (priority 044646)에서 우선순
위가 높은 구성요소를 항상 먼저 제거한다. 최고우선검색을 하면 우선순위가 높은 구성
요소가 최고의 한계값을 가진 마디가 된다. 우선순위 대기열은 연결된 리스트010600
lis) 구현할 수 있지만 heap) 2S 더 효율적으로 구현할 수 있다(7.6절에서 힙에 대
한 ABS 참조하라). 우선순위 대기열의 구현은 연습문제에서 다룬다. 최고우선검색의
일반 알고리즘은 다음과 같다. 여기서도 트리 7는 묵시적으로만 존재한다. 알고리즘에
서 insert (PQ, v)= 우선순위 대기열 POF vS 추가시키는 프로시저이고, remove
(PQ, v)= 최고 한계값을 가진 마디를 제거하고, 그 값을 ve] 대입한다.

branch_and_ bound (state_space_tree T,
number& best)

priority _queue_of_node PQ;

node u, Vv;

initialize( PQ);                               // PQS 빈 대기열로 초기화


===== PAGE 260 =====
@®eeee?e 0
248    chapter 6 분기한정법

v = root of 7;
best = value(v);
insert(PQ, v);

while (! empty(PQ)) {                         // AD 한계값을 가진 마디를 제거
remove(PQ, v);
if (bound(v) is better than best)             // 마디가 아직 유망한지 점검

for (each child uw of v){
if (value(u) is better than best)

best = value(u);

if (bound(u) is better than best)

> 알고리즘 6 9

insert(PQ, u);

대기열 대신에 우선순위 대기열을 사용하는 이외에 우선순위 대기열에서 마더를 제거
한 후 마디의 한계값이 beste} 아직 좋은지를 결정하는 검사를 추가하였다. 어떤 마디
방문한 후 그 마디가 유망하지 않게 되는지 이렇게 결정한다. 예를 들어, 그림 6.8의
더 (1, 9는 그 마더를 방문할 당시에 유망하다. 위의 알고리즘에서는 이때가 바로 PQ
에 마디를 추가하는 때이다. 그러나 maxprofit 값이 $900] 될 때 그 마디는 유망하지
않게 된다. 이는 마더를 우선순위 대기열에서 제거한 후 마디의 Shag maxprofieS
비교하여 알게 된다. 이런 식으로 방문한 후 유망하지 않게 되어버린 마디의 자식마디를
방문하지 못하게 한다.

다음은 0-1 배낭 채우기 BAS 푸는 세부 알고리즘이다. 마디를 추가하고 제거할 때
그리고 우선순위 대기열에서 마디의 순서를 매기기 위해서 한계값이 필요하므로, 그 한
ALS 마디에 기록한다. 마디의 타입은 다음과 같다.

struct node

{|

푸 때 (인

int level;               // 트리에서 마디의 수준
int profit ;

int weight;

float bound ;

Olt

0-1 배낭 채우기 문제를 SE 분기한정 가지치기 최고우선검색 알고리즘

문제 : 무게와 이익이 주어진 7개의 아이템이 있다고 하자. 무게와 이익은 양의 정수이다.
게다가 양의 정수 We 주어진다. 무게의 합이 Wt 넘지 못한다는 제약 하에서 총 이익
이 최대가 되는 아이템의 집합을 구한다.

입력 : 양의 정수 과 W; 양의 정수의 배열 wot p, 인덱스의 범위는 vee] /.까지이고,

r



===== PAGE 261 =====
@0600000 0
6.2 외판원 문제    249
각 ASS pli]/wli] el) 따라서 큰 수부터 차례로 정렬되어 있다.
출력 : 최적의 집합에 있는 이익의 합을 나타내는 정수 maxprofit
void knapsack3 (int n,
const int p[], const int 떠 ],
int W,
int& maxprofit)
{
priority. queue_of_node PQ;
node u, Vv;
initialize( PQ);                               // PQS 빈 대기열로 초기화
v.level = 0; v.profit = 0; v.weight = 0;         // v7} 뿌리마디가 되게 초기화
maxprofit = 0;
v.bound = bound(v);
insert(PQ, v);
while (! empty(PQ)) {                       // 최고의 한계값을 가진 마디 제거
remove(PQ, v);
if (v.bound > maxprofit) {                // 마디가 아직 유망한지 검사
u.level = v.level + 1;
u.weight = v.weight + wlu.level;         // ue 다음 게이 포함하는
u.profit = v.profit + plu.level;           if 자식마디로 놓음
if (u.weight <= W && u.profit > maxprofit)
maxprofit = u.protfit ;
u.bound = bound(u);
if (u.bound > maxprotit)
insert(PQ, u);
u.weight = v.weight;                    // 를 다음 아이템을 포함하지 않는
u.profit = v.protit ;                      // 자식마디로 놓음
if (u.bound > maxprofit)
insert(PQ, u);
}
i
}

함수 bound= 알고리즘 6.1과 동일하다.

@  6.2 외판원 문제

예제 3.12014 갑순이는 감돌이와 경쟁하여 외판원 직책을 따냈다. 왜냐하면 외판원 문
제를 푸는 O(n72") 동적계획 알고리즘으로 45초만에 20개의 도시로 이루어진 판매 영
So 최적 어행경모를 찾있기 패문이다, HEHE 1912] 어랭경로를 만들어 보하야하

는 무작정 알고리즘을 사용하였다. 무작정 알고리즘은 3,800년 이상 걸리기 때문에 아직



===== PAGE 262 =====
250

chapter 6 분기한정법

도 그 프로그램은 돌아가고 있다. 갑순이의 영역이 40개 도시로 확장되었음을 5.6절에서
마지막으로 보았다. 갑순이의 동적계획 알고리즘으로 이 영역의 최적 여행경로를 찾는데
6년 이상 걸리므로 그저 아무 여행경로나 cee 걸로 만족하게 되었다. 이 문제를 푸는
데 해밀토니안 회로 문제를 푸는 되추적 알                      . 이 알고리즘이 여행
경로를 효율적으로 찾기는 하지만 그 rae '최적6 고는 거리가 멀 수 있다. 예를
들어, 서로 9마일 떨어진 두 도시 사이를 연결하는 멀리 돌아가는 도로가 있다면, 두 도
시에서 각각 1마일 떨어진 도시를 통해서 그 두 EAS 연결할 수 있다 하더라도 그 알고
리즘은 긴 도로를 포함하는 여행경로를 선택할 수 있다. 이는 되추적 알고리즘으로 얻어
낸 여행경로를 사용하면 매우 비효율적인 여행경로를 얻을 수   ae 내시 된다. ‘
상황에서 갑순이는 아마도 최적의 여행경로를 찾는 게 Walch
다. 만약 40개 도시가 밀도 있게 연결되어 있다면, 되추적 알고리즘으로 모든 여행경로를
만들어 내려하면 뜻대로 되지 않을 것이다. 왜냐하면 여행경로의 수가 지수보다 많을 수
있기 때문이다. 만약 갑순이를 가르친 교수가 알고리즘 강의에서 분기한정 기술을 가르
치지 않았다고 가정해보자(이게 바로 그녀가 5.6절에서 아무 여행경로나 취하는 걸로 만
족해야 했던 이유이다). 알고리즘 교재를 다시 들추어보고 분기한정법이 최적화 문제를
풀기 위해서 특별히 고안된 방법이라는 사실을 깨달은 후에 갑순이는 외판원 BAS 푸
는데 그 기법을 적용하기로 결정한다. 아마도 다음과 같이 추진할 것이다.

방향그래프의 주어진 정점에서 출발하여 그래프에 있는 각 AAS 정확하게 한 번씩만
dias 정점으로 돌아오는 최단경로를 찾는 것이 이 BA 목표이다. 그러한

Z(optimal tour)2}31 한다. 출발정점이 어디인지는 상관이 없으므로 출발
aaa 첫째 정점이 될 수 있다. 그림 6.4를 보면 5개의 정점이 모두 서로
그래프를 표현해 놓은 인접행렬과 그 그래프의 최적 여행경로가 있다.
기 위하여 상태공간나무는 다음과 같이 구축한다. 출발 BAS 제외한 각
정점 이후의) 수준 1에 속한 첫째 정점으로 채택하고, 출발 정점과 수준 1에

ON @ of
kv 00
fu Ot

r@

am cir
at on
오구 bw

2

Ny

it yo 2% 기
 lr

ox
my
개
Hi
on

14    0    7    8

11    ~    9   0

18    ih   17   4

그림 6. 4 GE 정점을 연
이루는 그래프의 정점과



===== PAGE 263 =====
000000 0
6.2 외판원 문제   251

rx
고
ro
ox
my
tho

제외한 각 정점은 수준 3에 속한 둘째 정점으로 채택하고, 등등 이런
구축한다. 정점이 5개이고 모든 정점들 사이에 이음선이 있는 경우 구
트리의 일부분을 그림 6.5에서 보여준다. 앞으로, “마디"00000)라는 용어
트리의 마디를 나타내는데 쓰고, “정점”(0668이라는 용어는 그래프의 정점
데 쓴다. 그림 6.5의 각 마디에는 그 마디에 도달하기까지 선택된 경로가 모
두 포함된다. 편의상 그래프의 정접은 인텍스로만 표시한다. 잎이 아닌 마디는 모두 그
마디에 기록되어 있는 경로에서 시작하는 모든 여행경로를 나타낸다. 예를 들어, [1, 2,

이을 가지고 있는 OLS 경로 8, 2, 외에서 ARR: BE 여행경로를 나타낸다. 즉, 1
2, 3, 4, 5, 과 [1, 2, 8, 5 ,4 , 을 나타낸다. 각 잎은 여행경로를 나타낸다. 따라서 최적
여행경로가 포함된 잎을 찾아야 한다. 마디에 기록된 경로에 정점이 4개 있으면 트리 구
축을 멈춘다. 왜냐하면 다섯째 정점은 선택의 여지없이 하니뿐이기 때문이다. 예를 들
제일 AH] 있는 YS 여행경로 [1, 2, 3, 4, 5, 11을 나타내는데, 일단 경로 1, 2, 8,
1S 명시하면 다음 정점은 다섯째 정점일 수밖에 없다.

과
글
웨
노블 (0

Mm of

Al

0 alo clr Hy 쓰 조
fr
om,

5, on
호 포
& off
tes

(1, 2,3, 4]=
[1, 2, 3, 4, 5, 1]

그림 6.5 정점이 574 있는 그래프에서 외판원 문제의 한 사례에 대한 상태공간트리. 부
로의 정점의 인덱스가 각 마디에 기록된다.

여행경

HI


===== PAGE 264 =====
252

chapter 6 분기한정법

최고우선검색을 사용하기 위해서 각 마디의 한계값을 구할 수 있어야 한다. 0-1 배낭
채우기 문제에서는 총 무게가 WS 넘지 않도록 하면서 이익을 최대로 하는 게 목표였기
때문에, 주어진 마디에서부터 뻔어나가서 얻을 수 있는 이익의 상한을 계산하였다. 그리
고 어떤 마디에서 당시 최대이익보다 한계값이 큰 경우에 그 마디를 유망하다고 했다.
이 문제에서는 주어진 마디에서부터 뻔어나가서 얻을 수 있는 여행경로 길이의 하한을
구할 필요가 있다. 그리고 당시 최소경로길이보다 한계값이 작은 경우에 그 마디를 유망
하다고 한다. 한계값은 다음과 같이 구할 수 있다. 어떤 여행경로라도, 정점을 떠날 때
선택한 이음선의 길이는 그 정점에서 나오는 가장 짧은 이음선의 길이만큼은 최소한 길
다. 그러므로 정점 0, 을 떠나는 비용(선택한 이음선의 길이)의 하한은 인접행렬의 첫째
행에서 00] 아닌 모든 값 중에서 최소값이 되고, 그리고 vps 떠나는 비용의 하한은 둘째
행에서 0이 아닌 BE 값 중에서 최소값이 되고, 등등 이런 식으로 계속하면 된다. 그래
프에서 572] 정점을 떠나는 비용의 하한은 다음과 같다.

v, minimum(14, 4, 10, 20) = 4

Vg minimum(14, 7, 8, 7) =?

(

(

v3; minimum(4, 5, 7,16) =4

v, minimum(11, 7, 9,2) =2
(

vs; minimum(18, 7, 17, 4) =4

각 여행경로는 정점을 정확히 각각 한 번씩 떠나야 하기 때문에 여행경로 길이의 하한은
이 최소값들의 합이다. 따라서 여행경로 길이의 하한은 다음과 같다.

4+7+4+2+4= 21

이 길이의 여행경로가 있다는 BS 아니다. 이보다 더 짧은 여행경로가 있을 수 없다는
말이다.
그림 6.5에서 마디 [1 21S 포함한 마디를 방문했다고 가정하자. 이 경우 이미 0,를
여행경로의 둘째 정점으로 선택하였고, @;까지 가는데 든 비용은 4, 에서 v= 가는 이음
선의 가중치인 14가 된다. 따라서 이 마디 이후에 확장하여 구한 여행경로의 정점들을
떠나는 비용의 하한은 다음과 같이 구한다.
Vy                      14
Vo minimum(7, 8, 7)
7, 16)

(
v3 minimum(4,
v4, minimum(11, 9, 2)
(

7
4
2
4

| | ㅣ

vs minimum(18, 17, 4)

v2] 대한 최소값을 구하기 위해서 v1. 로 가는 이음선을 포함하지 않는다. 왜냐하면
에서 1 2S 바로 돌아갈 수 없기 때문이다. 다른 정점들에 대한 최소값을 구하기 위
해서 vo = 가는 이음선을 포함하지 않는다. 왜냐하면, 6;에는 이미 들렸기 때문이다. 1,



===== PAGE 265 =====
* 예제 6.3

를 포함하는 마디에서 확장하여 구한 여행경로 길이의 하한은 이 최소값들의 합이며
ann 같다.
14+7-+4+98+4= 31

한계값을 구하는 기술을 더 설명하기 위해서 그림 6,5에서 [1, 2, 3S 포함하고 있는 마
디를 방문했다고 가정하자. 《;를 둘째 정점으로, 《을 셋째 정점으로 하기로 이미 정했
다. 이 마디 이후에 확장하여 구한 여행경로는 정점들을 떠나는 비용의 하한을 가진다.

Vy               14
26                7
U3 minimum(7, 16) = 7
v4, minimum(11, 2)=2
v; minimum(18, 4)=4

와 v5] 대한 최소값을 구하기 위해서 v. 2 vz 고려하지 않는다. 왜냐하면 이 정
점들은 이미 들렸기 때문이다. [1, 2, 3}을 포함하는 마디로부터 확장하여 구할 수 * 있는
여행경로 길이의 하한은 다음과 같다.

14-7 +244 = 34
같은 방법으로 상태공간     트리에서 주어진 마디 이후로부터 확장하여 구할 수 있는 여행경

길이의 하한을 구할 수 있고, 이 하한을 최고우선검색에 사용할 수 있다. 다음 예제는
이 기술을 설명해 준다. 이 예제에서 계산과정은 보여주지 않는다. 설명한대로 하면 쉽게
구할 수 있다.

그림 6.4와 앞에서 설명한 한계값 구하는 방법을 사용하여 분기한정 가지치기 최고우선검색을
하면 그림 6.6과 같은 트리가 만들어진다. 한계값은 잎이 아닌 마디에 기록하는 반면, 여행경로
의 길이는 잎에 기록한다. 트리를 구축하는 절차를 살펴보자. 뿌리마디에는 해답후보가 없기 때
문에(해답후보는 상태공간트리의 잎에만 존재한다) 최고 해답의 값은 %(무한대)로 초기화한다.
알고리즘에 의하면 상태공간트리에서 잎 이후로는 확장하지 않기 때문에 잎에 대한 한계값은
계산하지 않는다. 마디를 참조하면 그 마디에 기록되어 있는 부분 여행경로를 참조하게 된다.
0-1 배낭 채우기 문제를 설명할 때와는 마디를 참조하는 방식이 다르다.
절차는 다음과 같다.
1, 14을 포함하는 마디(뿌리마디)를 방문한다.
(a) 한계값을 계산하면 219] 된다. {이 값이 여행경로 길이의 하한이다 }
(b) minlengthS 로 놓는다.
2. 1, 이를 포함하는 마디를 방문한다.
(8) 한계값을 계산하면 31이 된다.
3. 1, 31& 포함하는 마디를 방문한다.
(8) 한계값을 계산하면 22가 된다.



===== PAGE 266 =====
@006000000
254    chapter 6 분기한정법

, 4S 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 30°] 된다.
5. 0, 5S 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 427} 된다.
6. 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.
(a) 그 마디는 [Ｌ, 8]을 포함하는 마디이다. 그 마디의 지식마디부터 방문한다.
?. 0, 8, 1S 포함하는 마디를 방문한
(a) 한계값을 계산하면 22가 된다.
8. [1, 8, 시를 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 27이 된다.
9. [1, 8, 5S 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 39가 된다.
10. 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.

<7

[1]
Bound = 21

[1, 2]           [1, 3]                                [1, 4]           [1, 5]
Bound = 31             Bound = 22                                                     Bound = 30             Bound = 42

[1, 3, 4]
Bound = 27

[1, 4, 2]

(1, 4, 5]

Bound = 45                          Bound = 30

[1,.3, 2,4] =     [1,3;275]=
[1, 3, 2,4, 5, 1]} {[1,3, 2, 4,5, 1]
Length = 37         Length = 31

(1, 3, 4, 2]=
[1,,3:4;2;-5, 4]

(1,3, 4, 5]=
(1, 3, 4,5, 2, 1]

(1, 4, 5, 3] =
(157435; 35241]
Length = 48

Length = 43         Length = 34

그림 6.6 예제 6.3을 분기한정 가지치기 최고우선검색을 하여 구축            H
공간트리에서 YO] 아닌 마디에는 부분 여행경로가 위에 표시되어 있고, 그 마디에          구
할 수 있는 여행경로 길이의 한계값이 아래에 표시되어 있다. 상태공간트리에서 각 잎에는 여행경
위에, 그 길이가 아래에 표시되어 있다. 음영 처리된 마디는 최적 여행경로를 찾은 마디를

가
타낸다(여기서 Bound = 한계값> Length = 길이).



===== PAGE 267 =====
000000 0
6.2 외판원 문제   255

(a) 그 마디는 [1, 8, 이를 포함하는 마디이다. 그 마디의 지식마디부터 방문한다.
UW, [1, 3, 2, 448 포함하는 마디를 방문한다.
(a) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 37이 된다.
(b) 길이 37은 minlength 값 ㅇ보다 작으므로, miniength 값을 37로 놓는다.
(c) 11, 5]와 [1, 3, 5S 포함하는 마디들은 그들의 한계값 42와 39가 새 minlength 값 37보
다 크거나 같기 때문에 유망하지 않게 된다.
12, [1 8, 2, 5]를 포함하는 마디를 방문한다.
(a) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 31°] 된다.
(b) 길이 312 minlength 값 37보다 작으므로, minlength YS 31로 놓는다.
(0) [1, 21S 포함하는 마디들은 한계값 31이 Al minlength 값 31보다 크거나 같으므로 유망
하지 않게 된다.
18. 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.
(a) 그 마디는 [1, 8, 41S 포함하는 마디이다. 그 마디의 지식마디부터 방문한다.
14. [1, 8, 4, 이를 포함하는 마디를 방문한다.
(8) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 43이 된다.
15. [1, 3, 4, 5} 포함하는 마디를 방문한다.
(8) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 34가 된다.
16. 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.
유망하고 확장하지 않은 유일한 마디는 [1, 41S 포함하는 마디이다. 그 마디의 지식마디
부터 방문한다.
17. [1, 4, 이를 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 45가 된다.
00) 한계값 45는 minlength 값 31보다 크거나 같으므로 유망하지 않다고 결정한다.
18. [1, 4, 8]을 포함하는 마디를 방문한
(a) 한계값을 계산하면 38이 된다.
00) 한계값 382 minlength 값 31보다 AAU 같으므로 유망하지 않다고 결정한다.
19, [1, 4, 5S 포함하는 마디를 방문한다.
(a) 한계값을 계산하면 30°] 된다.
20, 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.
(a) 유망하고 확장하지 않은 유일한 마디는 [Ｌ, 4, 5|를 포함하는 마디이다. 그 마디의 지식
마디부터 방문한다.
21. [1, 4, 5, 이를 포함하는 마디를 방문한다.
(a) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 300] 된다.
(b) 길이 30°] minlength 값 31보다 작으므로, miniength2| 값을 30으로 놓는다.
22. [1, 4, 5, 3]을 포함하는 마디를 방문한다.
(a) 이 마디는 잎이므로, 여행경로의 길이를 계산하면 48이 된다.
28. 한계값이 가장 작은 유망하고 확장하지 않은 마디를 결정한다.
(a) 유망하고 확장하지 않은 마디가 없다. 완료되었다.

여행경로 1, 4, 5, 2, 8, 1S 나타내는 [1, 4, 5, 21S 포함하는 마디가 최적 여행경로이고, 그

—

(a


===== PAGE 268 =====
@00@00000 0
256    chapter 6 분기한정법

알고리즘 6.3

최적 여행경로의 길이는 30임을 구하였다.

상태공간트리 전체 마디의 개수는 + 4+4×3+4>×3>×28= 41인 반면, 그림 6.6의
트리에는 마디의 개수가 17개이다.
앞의 예제에서 사용한 전략을 구현하는 알고리즘에서 다음 데이터타입을 사용한다.

struct node

{
int level;               // 트리에서 마디의 수준
ordered_set path;
number bound;

he
path BEX 마디에 기록된 부분 여행경로를 포함한다. 예를 들어, 그림 6.6에서 뿌리마
디의 가장 왼쪽 자식마디의 28“/의 값은 [1, 이이다. 알고리즘은 다음과 같다.

외판원 SAS 푸는 분기한정 가지치기 최고우선검색 알고리즘

문제 : 가중치포함 방향그래프에서 최적일주여행길을 결정하시오. 가중치는 음이 아닌 정
수이다.

입력 : 가중치포함 방향그래프, /(그래프에서 정점의 개수). 그래프는 행과 열의 인덱스의
범위가 모두 1부터 7까지인 차원 배열 WE 표현한다. 여기서 Wile ?번째 정점에
서 GHA AAS 연결하는 이음선의 가중치이다.

출력 : 변수 2272/62874(최적일주여행길의 길이), 변수 0270/001(최적 여행경로)

void travel? (int n,

const number W ][ ],
ordered_set& opttour,
number& minlength)

{
priority queue_of_node PQ;
node u, v;
initialize( PQ);                               // PQS 빈 대기열로 초기화
v.level = 0;
vpath = [4];                                // 첫째 ABS 출발정점으로 놓음

v.bound = bound(v);
minlength = ©;
insert(PQ, v);
while (! empty(PQ)) {
remove(PQ, v);                            // 최고 MARS 가진 마디를 제거
if (v.bound < minlength) {
u.level = v.level + 1;                   // vw 의 자식마디로 놓음


===== PAGE 269 =====
}

}

}

0 000000
6.2 외판원 문제   257

for (all 7 such that 2 < 7 < n && 716 not in v. path ){
u. path = v. path ;
put 7 at the end of 2. path ;

i (2. devel == 2 - 2)f

}

// 다음 정점에서 FBS 마치는지 검사
put index of only vertex
not in uw. path at the end of u. path ;
put 1 at the end of u. path         // 첫째 AAS 마지막 정점으로 =
if (length(u) < minlength) {         // 함수 length= 여행경로의
minlength = length(u) ;         // 길이를 계산
opttour = u. path ;

}

else {
u. bound = bound(u) ;
if (u. bound < minlength)

}

insert(PQ, u) ;

함수 length?} bound= 연습문제로 작성해보기 바란다. 함수 JengthEe 여행경로
u.path| 길이를 넘겨주고, 함수 bound’: 이미 토의한 고려사항을 사용하여 마디의 한
계값을 넘겨준다.

한계값을 구하는 함수가 꼭 하나만 존재할 필요는 없다. 예를 들면, 외판원 문제에서
모든 정점을 정확히 한 번 방문해야 함을 관찰하고, 따라서 인접행렬의 행 값들 중 최소
US 택하는 대신 SHS 중 최소값을 사용할 수도 있다. 또 다른 방법으로 모든 정점은
정확히 한 번 들어갔다 나온다는 사실을 가지고, 행과 열의 값을 모두 이용할 수도 있다.

이음선이 나오는 정점에 그 가중치의 반을 주고, 이음선이 들어가는 정점에 나머지 반을
줄 수 있다. 그러면 정점을 방문하는 비용은 정점에서 나오고 들어가는 가중치의 합이
된다. 예를 들어, 여행경로 길이의 초기 한계값을 구한다고 하자. 6;로 들어가는 최소비
용은 둘째 열의 값들 중 최소값의 반을 취하여 얻어진다. v, HA] 나오는 최소비용은 둘째
행의 값들 중 최소값의 반을 취하여 얻어진다. 그러면 0,를 방문하는 최소비용은 다음과
같이 계산한다.

minimum (14, 5, 7, 7)+minimum(14, 7, 8, 7)
2

이 한계값 구하는 함수로 분기한정 알고리즘을 실행하면 그림 6,32] 사례에 대하여 15
개의 마디만 검사한다.

두 개 이상의 한계값 구하는 함수가 있을 때 한 함수는 어떤 마디에서 더 좋은 한계값
을 주는 반면, 다른 함수는 다른 마디에서 더 좋은 한계값을 줄 수 있다. 연습문제에서

=6



===== PAGE 270 =====
@®eeeee? 0
chapter 6 분기한정법

258

를 밝혀보라고 요구하겠지만 외판원 문제의 한계값 함수도 이 경우에 속한다. 이러한
경우 알고리즘은 가용한 한계값 함수를 모두 사용하여 최고의 한계값을 계산할 수 있다.
그러나 5장에서 토의했듯이 우리의 목표는 되도록 마디를 덜 방문하는데 있는 것이 아니
라 알고리즘 전체의 효율성을 최대화하는데 있다. 하나 이상의 한계값 함수를 사용하여 추
가적인 소요되는 AALS 마디를 덜 방문함으로써 얻는 절감을 상쇄하지 못할지도 모른다.

분기한정 알고리즘은 어떤 HYAMS 효율적으로 풀지만, 다른 사례에 대해서는 지
PEE 이보다 더 많은) 개수의 마디를 검사할지도 모른다. 갑순이의 딜레마로 돌아가
A, 분기한정 알고리즘으로도 40개 도시 사례에 대한 해답을 효율적으로 구하지 못한다
면 어떻게 할까? 외판원 문제 같은 문제를 취급하는 또 다른 하나의 방법은 근사 알고리
즘을 개발하는 것이다. 근사 알고리즘(300『0170814100 algorithms) 최적해를 준다는 보
장은 없지만, 최적에 꽤 가까운 해답은 준다. 외판원 문제의 근사 알고리즘은 9.5절에서
자세히 공부할 것이다.

@0

6.3

확률적 추론(진단)

이 AS 이산 확률이론과 베이즈(83768) 정리의 지식이 필요하다.

어떤 발견에 대한 가장 그럴듯한 BAS 찾아내는 것은 인공지능과 전문가 시스템에서
중요한 문제이다. 예를 들어, 의학에서 증상에 가장 맞는 병명을 알아내려고 한다든지,
전자회로에서 고장난 지점이 어디인지를 예측하려고 한다는지, 자동차에서 고장날 확률
이 가장 높은 부분을 찾는다는지 하는 문제들을 들 수 있다. 이와 같이 발견에 대한 가장
그럴듯한 설명을 찾아내는 과정을 BSA eZ (abductive inference)o]e}31 한다.

초점을 의학에 맞추어 보자. 7명의 환자가 가지고 있는 질병을 각각 ,, dy, …, @,이
라고 하자. 각 환자가 가지고 있는 증상의 집합을 라고 하자. 우리의 SHE 중상에 카
장 잘 맞는 AVS] 집합을 찾아내는 것이다. 기술적으로 두 개 이상의 집합이 존재할 수
있다. 그러나 맞을 만한 질병의 집합이 하나만 존재한다고 가정하고 문제에 접근한다.

신뢰 네트워크(66116【 network)= 질병과 증상 사이에 존재하는 확률적 관계를 나타내
는 표준이 된다. 신뢰 네트워크에 대해서는 이 BS] 범위에 벗어나므로 다루지 않는다.
지630011+8ㅁ0(1990)과 Pearl(1988)-2 보면 자세히 설명되어 있다. 신뢰 네트워크의 응용으
로, 특정 질병의 집합이 환자가 걸린 질병만을 포함하는 (증상을 발견하기 전) 사전 확률
(prior probability) 구하는 효율적인 알고리즘들이 있다. 이 알고리즘 또한 Neapoli-
180(1990)과 Pearl(1988)]A] 자세히 설명한다. 여기서는 이 알고리즘의 결과를 우리가
사용할 수 있다고 단순히 가정한다. 예를 들어, 이 알고리즘들은 환자가 걸린 질병들이
dy, dz, 0뿐일 사전 확률을 구할 수 있다. 이 확률은 다음과 같이 표시한다.

200 ds, dg)  또는 D= {d,, ds, Gar G1 때  p(D)

a



===== PAGE 271 =====
00000 0
63 확률적 추론(진단)    259

이 알고리즘들은 환자의 증상 So] 대한 ABS 가지고 질병 4,, dz, 들이 걸릴 확률도
구할 수 있다. 이러한 조건부 확률은 다음과 같이 표시한다.
p(d,, ds, dg| 5S) 또는 p(D|S)

(앞에서 언급한 알고리즘을 가지고) 이 확률들을 계산할 수 있다고 가정하면, 0-1 배낭
채우기 문제를 푸는데 사용한 것과 비슷한 상태공간트리를 사용해서 (증상에 대한 정보
가 있다고 가정하고) 가장 걸릴 확률이 높은 AY] 집합을 구하는 BAS 풀 수 있다.
0, 을 포함하려면 뿌리마디에서 왼쪽으로 가고, 제외시키려면 오른쪽으로 간다. 비슷하
Al, @,를 포함하려면 수준 1의 마디에서 왼쪽으로 가고, 제외하려면 오른쪽으로 가고,
이런 식으로 계속한다. 상태공간트리에서 잎은 각각 해답후보(즉, 그 잎에 오기까지 포함
한 질병들의 집합)가 된다. 이 문제를 풀기 위해서 각 잎에 포함되어 있는 질병들의 집합
의 조건부 확률을 계산하고, 그 중에서 가장 높은 조건부 확률을 택한다.

최고우선검색으로 가지치기 위해서 한계값을 계산하는 함수를 찾을 필요가 있다. 다음
정리는 대형 사례를 처리하는 방법을 제시하고 있다.

> 정리 6.1

202
증명 : 베이스의 정리에 따르면, 다음과 같이 HEA 유도할 수 있다
1) oy 2(6612)202)
= P(S|D')p(D)
~     p(S)
— P(D)
~ p(s)

첫째 부등식은 이 정리의 가정에 의하여 성립하고, 둘째는 확률은 항상 1보다 작다는 사실에
의하여 성립한다. 증명이 완료되었다.

주어진 어떤 마디에 대해서 DS 그 마디에 오기까지 포함된 질병들의 집합이라 하고,
그 마디의 어떤 후손마디에 대해서 D'S 그 후손마디에 오기까지 포함된 질병의 집합이
라 하자. 그러면 DS 27'이 성립한다. 보통 다음과 같이 가정하면 타당하다.

DEDAA pW’) < p(dD)


===== PAGE 272 =====
@00@00000 0
260    chapter 6 분기한정법

© 예제 6.4

환자가 어떤 질병들을 가지고 있을 확률은 그 AYSS 아니라 더 많은 질병들을 가지고
있을 확률보다는 보통 작기 때문이다(이는 SARS 알기 전 사전 확률이라는 사실을 상기
하자). 이러한 가정 하에 정리 6.1에 의해서 다음과 같은 부등식을 얻는다.

(22)
6

7,      2
p(D IS) < Ty

따라서 p(D)/p(S)%= 그 마디의 어떤 후손마디가 가지고 있는 조건부 확률의 상한이다.
다음 예제에서 이 한계값을 어떻게 가지치기에 사용하는지 설명한다.

~

d,, dy, ds, 0,의 4가지 AYO] 있다고 가정하고, 증상의 집합을 라고 하자. 이 예제에서 입력은
질병과 증상 사이의 확률적 관계를 담고 있는 신뢰 네트워크도 포함한다. 이 예제에 사용된 확률
은 앞에서 설명한 방법을 사용하여 이 신뢰 네트워크를 가지고 계산한다. 이 책에서 이 SHS
계산하지는 않는다. 최고우선검색 알고리즘을 설명하기 위하여 임의의 확률을 배정한다. 한 알
고리즘에서 얻은 결과(이 경우, 신뢰 네트워크에서 추론으로 얻은 결과)를 다른 알고리즘(최고우
선검색 알고리즘)에 사용할 때, 둘째 알고리즘에서 단순히 가정될 수 있는 결과를 첫째 알고리즘
의 어디서 주는지 알아내는 것은 중요하다.

그림 6.72 최고우선검색으로 구축한 가지친 상태공간트리이다. 트리에서 확률 값을 임의로
주었다. 조건부 확률은 각 마디의 위쪽에 표시되어 있고, 한계값은 아래쪽에 표시되어 있다. 음
영 처리된 마디는 최고 해답을 찾은 마디를 나타낸다. 6.1절에서와 마찬가지로 마디는 깊이와
트리의 왼쪽으로부터의 위치에 따라서 라벨을 붙인다. 트리를 구축하는 절차는 다음과 같다. 변
수 best= 현재 최고 해답인 BEA, p(best| 5)는 그 값의 조건부 확률이다. 우리의 목표는 조건
부 확률을 최대화하는 066*의 값을 구하는 것이다. 임의로 다음과 같이 가정한다.

p(S) =0.01

1, 마디 (0, 0)(뿌리)를 방문한다.
(a) 이 마디의 조건부 확률을 계산한다. {2 은 공집합이다. 이는 AV] 없음을 나타낸다}
2(019)=0.1 {o] 계산은 다른 알고리즘으로 ARH}
{따라서 임의의 값을 배정한다.}

00) 다음과 같이 놓는다.
best = @     p(best |S) =p(@ |S) =0.1
(0) 사전 확률과 한계값을 계산한다.

p(@) =0.9
_pP(S)_ 09 _
bound  m5)  Dor 90

2, 마디 (1, DS 방문한다.
(a) 이 마디의 조건부 확률을 계산한다.



===== PAGE 273 =====
0000000
63 확률적 추론(진단)    261

(0, 0)

p(o|S) =0.1
Bound = 90
p(,|S) = 0.4                        p(o|S) =0.1
Bound = 0.9                                          Bound = 90
ds)          (251)                          (2, 2)               (2, 3)                          (2, 4)
p(d,, 09) =0.1          p(d, IS) =0.4              p(d,|S) = 0.15           p(o|S) = 0.1
Bound =                 Bound = 0.9               Bound = 0.5             Bound = 90
ds)                                                       (3, 2)               (3, 3)                           (3, 4)
P(d;, 보일 =0.5         p(d,|S) = 0.4              Pd, 0 =0.1             p(o|S) = 0.1
Bound = 0.1             Bound = 0.9               Bound = 0.2             Bound = 90
a4)

(4, 3)                                          (4, 4)

p(d; |S) = 0.4
Bound = 0

00049) =0.6             p(o|S) =0.1
nd =0              Bound = 0

Bol

그림 6.7 예제 6.4에서 분기한정 가지치기 최고우선검색으로 구축한 가지친 상태공간트리. 각 마
디에서 위에 있는 값은 그 마디까지 포함된 병의 조건부 확률이고, 아래에 있는 값은 그 마디에서
확장하여 구할 수 있는 조건부 확률의 한계값이다. 음영 처리된 마디는 최적 해답을 찾은 마디를
나타낸다.

00 0.4 > p(best | 5)이므로, 다음과 같이 놓는다.

best = {d, }       p(best |.5) =0.4
(0) 사전 확률과 한계값을 계산한다.

p(d,) =0.009

p(d,) — 0.009 _

3, 마디 (1, 2S 방문한다.

(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.1이다.


===== PAGE 274 =====
@0000000
262    chapter 6 분기한정법

00) 사전 확률과 한계값은 단순히 부모마디의 값들 0.9와 90이다.
4. 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.

(a) 그 마디는 마디 (1, 9)이다. 이 마디의 자식마디를 다음에 방문한다.
5. 마디 (2, 8)을 방문한다.

(8) 이 마디의 조건부 확률을 계산한다.

200, |S) =0.15
(b) 사전 확률과 한계값을 계산한다.
p(dy) = 0.005
— Pda) - 0.005 _
bound =  (09  = 01 0.5

6. 마디 (2,4)를 방문한다.
(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.1이다.
06) 사전 확률과 한계값은 단순히 부모마디의 값들 0.9와 90이다.

7, 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.

(a) 그 마디는 마디 (2, 4)이다. 이 마디의 자식마디를 다음에 방문한다.
8. 마디 (3, 3)을 방문한

(a) 이 마디의 조건부 SHES 계산한다.

p(d, |S) =0.1
(b) 이전 확률과 한계값을 계산한다.
p(dz) = 0.002
_ p(d;) 0.002 _
bound = pS) 0.01. 0.2
않다.
9. 마디 (3, 4)를 방문한다.
(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.1이다.

(b) 이전 확률과 한계값은 단순히 부모마디의 값들 0.9와 90이다.
10. 가장 큰 MARS 가진 유망하며, 확장되지 않은 마디를 구한다.
(a) 그 마디는 마디 (3, 4)이다. 이 마디의 자식마디를 다음에 방문한다.
1. 마디 (4, 8)을 방문한다.
(a) 이 마디의 조건부 확률을 계산한다.
p(d,|S) =0.6
(b) 0.6 > p(best| 5)이므로, 이전 확률과 한계값을 계산한다.
best = {d,}
p(best | 5) = 0.6

(0) 이 마디는 상태공간트리의 잎이므로, 이 마디의 한계값은 0으로 놓는다.

(0) 이 마디의 한계값 0.2는 plbest | 9) 값인 0.4보다 작거나 같으므로, 이 마디는 유망하지


===== PAGE 275 =====
@‥00@0000 0
63 확률적 추론(진단)    263

(0) 이 시점에서 이 마디 (2, 9)의 한계값 0.5% p(best | 9) 의 새로운 값인 0.6보다 작거나
같으므로, 이 마디는 유망하지 않게 된다.
12, 마디 (4, 4)를 방문한다.
(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.1이다.
00) 이 마디는 상태공간트리에서 잎이므로, 이 마디의 한계값은 0으로 놓는다.
13, 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.
(a) 그 마디는 마디 (1, Nolet, 이 마디의 자식마디를 다음에 방문한다.
14. 마디 (2, 1)을 방문한다.
(a) 이 마디의 조건부 확률을 계산한다.
pld,, d,| 5) = 01
(00) 사전 확률과 한계값을 계산한다.
p(d,, 06.) =0.003

Pld, dy) - 0.003 _
p(s) 0.01
(0) 이 마디의 한계값 0.32 plbest | 5) 값인 0.0보다 작거나 같으므로, 이 마디는 유망하지
않다.
15. 마디 (2, 9)를 방문한다.
(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.4이다.
(b) 사전 확률과 한계값은 단순히 부모마디의 값들 0.009와 0.9이다.
16. 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.
(a) 유망하며, 확장되지 않은 유일한 마디는 (2, 9)이다. 이 마디의 자식마디를 다음에 방문
한다.
17. 마디 (3, 1)을 방문한다.
(a) 이 마디의 조건부 확률을 계산한다.
p(d,, 4190 =0.05
(b) 사전 확률과 한계값을 계산한다.
p(d,, ds) =0.001

bound =                                      0.3

p(d, ds)  0.001
706 oor
(c) 이 마디의 한계값 OLS p(best |S) 값인 0.0보다 작거나 같으므로, 이 마디는 유망하지
않다:
18, 마디 (3, 9)를 방문한다.
(a) 이 마디의 조건부 확률은 부모마디의 조건부 확률인 0.4이다.
06) 사전 확률과 한계값은 단순히 부모마디의 값들 0.009와 0.9이다.
19. 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.
(a) 유망하며, 확장되지 않은 유일한 마디는 (3, 9)이다. 이 마디의 자식마디를 다음에 방문
한다.

bound =



===== PAGE 276 =====
@eeee ee
264   chapter 6 분기한정법

He 6.4 호

20. 마디 (4, 1)을 방문한다.
(a) 이 마디의 조건부 SSS 계산한다.
p(d,, d, |S) =0.65
(b) 0.65 > p(best | .9)이므로, 다음과 같이 놓는다.
best = {d,, d,}
p(best |S’) = 0.65
(c) 이 마디는 상태공간트리의 잎이므로, 이 마디의 한계값은 0으로 놓는다.
21. 마디 (4, 2)를 방문한
(8) 이 마디의 조건부 8    률은 부모마디의 조건부 확률인 0.4이다.
00 이 마디는 상태공간트리의 잎이므로, 이 마디의 한계값은 0으로 놓는다.
22, 가장 큰 한계값을 가진 유망하며, 확장되지 않은 마디를 구한다.
(a) 유망하며, 확장되지 않은 유일한 마디가 없다. 종료.

가장 걸릴 확률이 높은 질병의 집합은 {d,, d,} 이고, 200, d, | 5) = 0.65 ©] TH,

이 BAS 풀기 위한 타당성 있는 전략으로는 조건부 확률이 높은 것부터 질병을 초기
에 정렬하는 것이다. 그러나 이 전략으로 검색시간을 최소화 할 수 있다는 보장은 없다.
예제 6.4에서는 이 전략을 적용하지 않고 15개 마디를   메주 질병이 정렬된 경
23개의 마디를 검색하게 된다는 사실은 연습문제로 알아보도록 한다.

이제       즘을 살펴보자. 다음 타입을 사용한다.

struct node

{
int level;               // 트리에서 마디의 수준
set_of_indices D;
float bound;

};

필드 DE 그 마디까지 포함된 질병의 인덱스 값을 가진다. 이 알고리즘의 입력 중 하나
는 신뢰 네트워크 #4이다. 앞에서 ABBE] 신뢰 네트워크는 질병과 증상 사이의 확
률적 관계를 나타낸다. 이 절의 시작 부분에서 참조한 알고리즘으로 그러한 네트워크에
서 필요한 확률을 계산할 수 있다.

다음 알고리즘은 쿠퍼(20086, 1984)7} 개발하였고, 쿠퍼의 알고리즘으로 알려져

= EME 푸는 쿠퍼의 분기한정 가지치기 최고우선검색 알고리즘

문제 : 증상의 집합에서 가장 걸릴 확률이 높은 질병을 결정하라. 질병의 집합 DE 질병의



===== PAGE 277 =====
집합 22 의 부분집합이면, p(D’) < 7(20)가 성립한다고 가정한다.

입력 : 양의 정수 n, "개 질병과 그 증상 사이의 확률적인 관계를 표시하는 신뢰 네트워크
BN, 중상의 집합 5

출력 : (의 조건하에서) 가장 걸릴 확률이 높은 질병의 인덱스를 포함하는 집합 dest, 6가
주어지고 best 9] SHES 나타내는 변수 phest

void cooper (int n,
Bayesian_network_of_z_diseases BN,
set_of_ symptoms 5S,
set_of_indices& best, float& pbest)

priority _queue_of_node PQ;
node u, Vv;

v.level = 0;                           // ve 뿌리로 놓는다.
v.D= ©;                      // SASS 뿌리에 저장한다.
best = 23
pbest = p( |S);
v.bound = bound(v);
insert(PQ, v);
while (! empty({PQ)) {
remove PQ, v);                    // 최고 한계값을 가진 마디를 제거한다.
if (v.bound > 20650 {
u.level = v.level + 1;            // u& v2] 자식마디로 놓는다.
u.D = v.D;                      // ue 다음 ABS 포함하는 자식마디로 놓는다.
put u.Jeve/ in u.D;
if (p(u.D|S) > pbest) {
best = u.D;
phest = p(u.D|S);
}
u.bound = bound(u);
if (u.bound > pbest)
insert(PQ, u);
uD = v.D;                              // 를 다음 질병을 포함하지 않은 자식마디로 놓는
u.bound = 2072220( 20);
if (u.bound > 20090
insert(PQ, u);
}

}
}

int bound(node u)
{
if (u.Jevel == n)                    // 잎은 유망하지 않다.
return 0;
else


===== PAGE 278 =====
@000000 0
266    chapter 6 분기한정법

return p(u.D |p(5));

;                 p(D)= D2 사전 확률을 나타내고, p(S)E 의 사전 확률을 나타내고, p(DIS)=
가 주어진 상태에서 D2] 조건부 확률을 나타낸다. 이 값들은 이 장 시작 부분에서 참조
한 알고리즘을 사용하여 신뢰 네트워크 2/+으로부터 계산할 수 있다.
최고우선검색 알고리즘을 작성하는 지침에 따라 엄격하게 알고
기서 성능 향상이 가능하다. 마디의 우측 자식마디에 대하여 함수 bound 호출할 필요
가 없다. 그 이유는 우측 자식마디는 그 마디 자신과 질병의 집합이 같고, 이는 한계값도
같음을 의미한다. 따라서 좌측 자식마디에서 phestS 이 한계값으로 바꾸는 경우에만 우
측 자식마디를 가지친다. 이러한 경우에 우측 자식마디를 가지치고, 그렇지 않은 경우
우측으로 확장하도록 알고리즘을 수정할 수 있다.
이 장에서 설명한 다른 문제들과 마찬가지로 확률적 추론 문제는 9장에서 다루는 문제
의 부류에 속한다.
하나 이상의 해답이 있는 경우, Ho] 알고리즘은 그 중 하나만 acta  최고 해답을
모두 찾도록 알고리즘을 수정하기는 쉽다. 가장 걸릴 SH] 높은 mS) ABS
찾아내도록 알고리즘을 수정할 수도 있다. Neapolitan(1990)o] 그 1 방법과 분석이 자세히
나와 있다.
@ 연습문제
6.1절

1. 알고리즘 6100-1 배낭 채우기 문제를 푸는 분기한정 가지치기 너비우선검색 알고리즘)을
사용하여 다음 문제 사례에 대한 이익을 최대화하시오. 알고리즘 수행 절차를 단계별로 보
의세오.

6

P;

$20
$30
$35
$12
$3

onaasd 르보

or WD
rPoN od

W=13
2. 알고리즘 61S 구현하는 프로그램을 작성하고, 연습문제 19] 문제 사례로 실행시켜 보시오.

3. 최적의 아이템 집합을 만들어 내도록 알고리즘 6.1을 수정하시오. 수정한 알고리즘의 성능
을 알고리즘 6.1과 비교하시오.


===== PAGE 279 =====
@0ㅋ00000 0
연습문제 267

4. 알고리즘 6.2(00ㄱ1 배낭 채우기 BAS 푸는 분기한정 가지치기 최고우  ae 알고리즘)를
사용하여 연습문제 1의 문제 사례에 대한 이익을 최대화하시오. 알고리즘 수행 절차를 단계
별로 보이지오.

5. 알고리즘 6.2를 구현하는 프로그램을 작성하고, AGHA 19] 문제 사례로 실행시켜 보시

6. 대형 문제 사례를 가지고 알고리즘 6.1과 알고리즘 6.8의 성능을 비교하시오.

6.2절
7. 알고리즘 6.8(외판원 문제를 푸는 분기한정 가지치기 최고우선검색 알고리즘)을 사용하여
아래 그래프에 대하여 최적 여행경로와 그 경로의 길이를 구하시오.

알고리즘 수행 절차를 단계별로 보이시오.

8. 알고리즘 6.8을 사용하여 인접행렬이 다음과 같은 배열인 그래프에서 최적경로를 찾으시오.
찾는 WS WIE 보이시오.

1    2 3 4 5
1; 0| 6} 6 | 10} 8
2| 31 0 | 12| 7
3/8 | 7/] 0 | 14} 20
4} 5] 13] 9       8
5} 9ㅣ| 8 | 10} 6] 0

10. 외판원 문제

(06) 작성한 알고리즘을 구현하고 크기가 6, 7, 9, 10, 15, 30인 사례의 해답을 구해보시오.
(0) 이 알고리즘과 알고리즘 6.8을 09의 AMS 가지고 성능을 비교해보시오.

. 알고리즘 6.8을 구현하는 프로그램을 작성하고, 연습문제 72] 문제 사례로 실행시켜 보시
오. 다른 한계값 함수를 사용해 보고, 결과를 검토해 보시오.



===== PAGE 280 =====
268

chapter 6 분기한정법

12. 대형 문제 사례를 가지고 외판원 문제를 푸는 동적계획 알고리즘(3.6절의 연습문제 27)과
알고리즘 6.8의 성능을 비교하시오.

6.3절

13. 알고리즘 6.4(0006@의 HEA 추론 문제를 푸는 분기한정 가지치기 최고우선검색 알고리
BES 가장 걸릴 확률이 높은 개의 질병을 찾아내도록 수정하시오. 여기서 me 임의의
양수이다.

14. 예제 6.4에서 질병들이 조건부 확률이 높은 것부터 차례로 정렬되어 있다면, 검사하는 마디
의 수가 157} 아니고, 230] 됨을 보이시오. p(d,) =0.008이고, play, d,) =0.007이라고 가
정한다.

15. 질병들의 확률의 eo] pur} 크거나 같으면, 그 질병의 집합은 안전측정치 pS 만족한다.
0 = 7 = 1인 pS 만족하는 BY] AWS 찾아내도록 알고리즘 6.4를 수정하시오. 가능한
한 적은 수의 질병을 가지고 하시오.

16. 알고리즘 6.4를 구현하는 프로그램을 작성하시오. 이용자는 AGHA 18에서 설명한 대로
m& 입력하거나, 연습문제 18에서 설명한 대로 안전 측정치 pS 입력할 수 있어야 한다.

추가적인 연습문제

17. 3장의 연습문제 3(에서 논의한 문제를 해결하는데 분기한정 설계전략을 사용할 수 있을까?
그리고 왜 그런 답이 나오는지를 밝히시오.

18. 4.8.9절에서 공부한 마감시간 있는 스케줄 짜기 문제를 푸는 분기한정 알고리즘을 작성하
시오.

19. 4장의 연습문제 26에서 공부한 문제를 해결하는데 분기한정 설계전략을 사용할 수 있을까?
그리고 왜 그런 답이 나오는지를 밝히시오.

20. 8.4절에서 논의한 연쇄행렬곱셈 문제를 푸는데 분기한정 설계전략을 사용할 수 있을까? 그
리고 왜 그런 답이 나오는지를 밝히시오.

21. 분기한정 설계전략을 사용하여 풀 수 있는 문제의 예를 3가지 더 나열하시오.



===== PAGE 281 =====
O(n) 정령 graze ae
{   때까지 난 포기하지 않을

정렬문제

1  1   절에서 8차시간 정렬 알고리즘(교환정렬)을 공부했다. 만약 컴퓨터 과학자가
°      이 정렬 알고리즘에 만족했다면 시중에서 사용하고 있는 소프트웨어들이 훨씬
더 느리게 작동하고 있거나, 아마도 일부는 아예 작동이 불가능했을지도 모르겠다. 22}
시간 알고리즘을 사용하여 10억 개 키를 정렬하는데 수년이 걸린다는 사실을 표 1.4에서
보았다. 다행하게도 2차시간보다 더 효율적인 정렬 알고리즘을 발견했다. 특히, 2.절에
서 최악의 경우 O(n lg 7) 인 합병정렬(44678660ㅁ을 공부했다. 이 알고리즘이 비록 10억
개의 데이터를 사용자가 느끼지 못할 정도로 빨리 정렬하지는 못하지만, 표 1.4에서 봤듯
이 오프라인 응용에서는 참을만한 시간 안에 데이터를 BAS 수 있다. 가령 10억 개의
아이템을 온라인으로 거의 즉시에 정렬하기를 원하는 사람이 있다고 가정해보자. 그 사
람은 1차시간 또는 그 보다 좋은 정렬 알고리즘을 개발하려고 많은 시간 심지어는 여러
해의 시간을 투자하려 할지도 모른다. 이를 위해 전 인생을 투자한 후에 그러한 알고리즘
은 불가능하다는 사실을 알게 된다면 얼마나 억울할까? 문제를 푸는 알고리즘에 도전해

는 방식은 두 가지가 있다. 하나는 문제를 푸는 더 효율적인 알고리즘을 설계하는 것이

고, 다른 하나는 더 효율적인 알고리즘 개발이 불가능함을 증명하는 것이다. 일단 증명을


===== PAGE 282 =====
270     chapter 7 계산복잡도의 소개: 정렬문제
하면, 더 빠른 알고리즘의 개발은 시도할 가치가 없다. 앞으로 알게 되겠지만, 정렬 문제
를 푸는 데 O(nlgn) BU 좋은 알고리즘은 불가능하다고 이미 증명되었다.

@® 71 계산복잡도

였다. 알고리즘은 시간(공간)복잡도나 시간(공간)복잡도의 APS 구하여 분석한다. 즉,
알고리즘이 푸는 문제 자체를 분석하지는 않았다. 예를 들어 알고리즘 1.4(행렬곱셈)를
분석하여 그 알고리즘의 시간복잡도가 7*임을 알았다. 그러나 그렇다고 해서 행렬곱셈
BAS 푸는데 O(n) 알고리즘 밖에 없다는 의미는 아니다. 함수 7은 그 알고리즘의
특성이지, 행렬곱셈 문제의 특성일 Woe 없다. 2.5절에서 시간복잡도가 0(@^')인 수
트라썬의 행렬곱셈 알고리즘을 공부했다. 더구나 0(7”※)인 변형 알고리즘도 Apes

[을    oot
fu

아보

다
me
으
Gi

보았다. 중요한 건 더 효율적인 알고리즘을 찾는 게 가능한지
ㅣ

알고리즘 설계 및 분석과 더불어 다루어야 하는 분야인 계산복잡도(000046840781
complexity)= 주어진 문제를 풀 수 있는 가능한 모든 알고리즘에 대한 연구이다. 계산복
=                             °

잡도 BAS 같은 BAS 푸는 모든 알고리즘의 효율성(복잡도)의 하한을 구하는 것이다.
2.5절의 마지막 부분에서 행렬곱셈 문제를 푸는데 필요한 최소 시간복잡도가 Qn’) A
이 증명되었음을 언급했다. 바로 이 결과가 계산복잡도 분석으로 구한 것이다. 즉, 행렬
곱셈 EAS 푸는 하한00\6『 00400)은 (2(/7”)이라는 결과를 얻은 것이다. 행렬곱셈을
푸는 O(n’) 알고리즘을 틀림없이 찾을 수 있음을 보장하는 것은 아니다. | O(n’) a

다 더 빠른 알고리즘을 만드는 것이 불가능함을 의미할 뿐이다. 지금까지 알려진 최고

H
의
ro
.으
주
대
더;
ki
So,
do
고
qu
고
%
요
ay
mo
0
N
At
™
lr
3
aw

개선하는 것 이외에 알고리즘의 성능을 더 이상 향상시킬 수 없다
저자에 따라서 “계산복잡도 분석"이라는 용어를 알고리즘과 문제 BAS 모두 포함하
는 것으로 사용하기도 한다. 이 책에서 계산복잡도 분석은 문제의 분석만을 의미한다.
이 장에서는 정렬 문제를 가지고 계산복잡도 분석을 소개한다. 이 문제를 선택한 이유
는 두 가지이다. 첫째, 이 SAS 푸는 알고리즘을 wy 많이 발견했기 때문이다. 같은 문제
를 푸는 여러 알고리즘들을 공부하고 비교함으로써 여러 알고리즘들 가운데 하나를 선택


===== PAGE 283 =====
@0000000
ㅣ 케센복점도  201

하는 기준은 무엇인지, 그리고 알고리즘을 어떻게 개선하는 방안

0
있다. 둘째, 정렬 문제는 시간복잡도가 하한만큼 좋은 알고리즘이 존재하는 몇 되지 않는
우          n

ix
ofN
z
N
BaF
§
ae
mI
od
use,
별
at
+
&
때 it
‘Ss
06
2
tho
ne
KI
※으
by
@
Ss
oe
S

알고리즘을 AR 발견했다. 따라서 정렬문제는 풀렸다고 할 수 있다.

거의 하한만큼 좋은 알고리즘이 있는 정렬 알고리즘의 부류로 키를 비교하여 정렬하는
알고리즘을 들 수 있다. 1장의 앞부분에서 설명했듯이 "키"라는 단어를 사용한 이유는 레
코드는 순서집합의 요소인 키0669)라고 하는 유일한 식별자가 보통 포함되어 있기 때문
이다. 엄의의 순서로 나열된 레코드의 정렬 4A (sorting 1898은 키의 값을 기준으로 한
순서로 그 레코드를 다시 나열하는 것이다. 이 ao] 알고리즘에서 키는 배열에 저장되어

keys)Sh= 알고리즘은 두 키를 비교하여 어떤 키가 큰지를 결정할 수 있고, 키를 저장할
수 있지만 키에 대한 다른 연산은 할 수 없다. 지금까지 접해 본 정렬 알고리즘(알고리즘
1,3, 2.4, 2.0)은 모두 이 부류에 속한다.

7.3절에서 7.8절까지 비교만으로 정렬하는 알고리즘을 공부한다. 세부적으로 보면,
7.2절에서는 가장 효율적인 8차시간 정렬 알고리즘인 삽입정렬과 선택정렬을 공부한다.
7.8절에서는 삽입정렬과 선택정렬의 YAS 고집하는 한 2차시간보다 좋게 개선할 수 없
다는 사실을 알려준다. 7.4절과 7.5절에서는 (218 7) 정렬 알고리즘인 합병정렬과 퀵
정렬을 복습한다. 7.0절에서는 또 하나의 O(nign) 정렬 알고리즘인 34a Heapsort)
을 소개한다. 7.7절에서는 이 3가지 O(nign) 정렬 알고리즘을 비교한다. 7.8절에서는
키를 비교하여 정렬하는 알고리즘의 하한은 O(n lg n) 임을 증명한다. 7.9절에서는 키를
비교하지 않고 정렬하는 정렬 알고리즘인 기수정렬08015 Sort) 공부한다.

키의 비교 횟수와 레코드의 저장(668180ㅁ7641) 횟수를 기준으로 알고리즘을 분석한다.
WS 들어, 알고리즘 1.8(교환정렬)에서 Sli] 2 917] 의 교환은 다음과 같이 구현한다.

temp = 912];
Sli] = Sly];
S{j] = temp;

이는 레코드를 3H 저장하여 한 번의 교환이 이루어짐을 의미한다. 레코드 저장의 횟수
를 분석하는 이유는 레코드의 크기가 크면 레코드를 저장하는 시간이 꽤 길기 때문이다.
또한 입력을 저장하는데 필요한 저장장소 이외에 알고리즘을 수행하는데 얼마만큼의 추
가적인 저장장소를 사용하는지도 분석한다. 추가적으로 사용하는 저장장소가 상수이면
즉, 정렬할 키의 수 nthe 증가하지 않으면), 그 알고리즘은 제자리 정렬0ㅁ-ㅁ1806 sort)
이라고 한다. 마지막으로, 항상 비내림차순으로 정렬한다고 가정한다.



===== PAGE 284 =====
@6 00000 0
272    chapter 7 계산복잡도의 소개: ASA
Sorted            Unsorted
ㅅ.              KA
c                  ~           ”
2   4   7   8   9   5   1   3

Sit] 의 S[3] S[4] 의] 의이 S[7]_— S83}

2     4                             1     3

Sit] Si2] 의] - 914] 의] 의이 S[7]_— 의하
그림 7.1 ＊=6이고 7=2일 때 삽입정렬을 수행하는 과정을 설명한 al. (위) 삽입하기 전 배열,
(아래) 삽입절차

@ 7.2 삽입정렬과 선택정렬

> 알고리즘 7.|

삽입정렬1086500ㅁ sort) 알고리즘은 이미 정렬된 배열에 레코드를 삽입하여 정렬하는
알고리즘이다. 삽입정렬이 어떻게 작동하는지 예를 SHS 다음과 같다. 처음 1-1 배
열 슬롯의 키들이 정렬되어 있다고 가정한다. cS iA 슬롯에 있는 키 값이라 하자.
x} (i— 1) HA 슬롯에 있는 키, (8 - 2)번째 슬롯에 있는 키, 등등 차례로 비교하되 x
보다 작은 키를 찾을 때까지 이를 계속한다. 7를 그 키가 위치한 슬롯이라고 하자.
(7 + 1)번째 슬롯에서 (＊- 1)번째 SEO] 있는 ISS (+ 2) 번째 슬롯에서 CA 슬롯
으로 옮기고, (7+ 1)번째 슬롯에 cS 삽입한다. 이 과정을 i = 2에서부터 i = 까지 반
복한다. 그림 7.1에서 삽입정렬을 그림으로 설명한다.

삽입정렬
문제 : 비내림차순으로 7개 키를 정렬
입력 : 양의 정수 7, 키의 배열 SIAL 1부터 7)

출력 : 비내림차순으로 정렬한 키들로 구성된 배열 6'

void insertionsort (int n, keytype 의 ])

{
index 2, J;
keytype x;

for (= 25

f <=> 2; e+) {

x= 이기;



===== PAGE 285 =====
J= 1-1;
while (j > 0 && Sj] > x) {
V+ i= 시기;

=:

『(삽입정렬)에서 키 비교 횟수 기준 최악 시간복잡도 분석

>

뚜

위연산 : .9[7]와 2의 비교
력크기 : 정렬할 키의 개수 /

주어진 io 대해서 가 0이 되면서 while 루프를 빠져나갈 때 6[/]와 <의 비교 횟수가

가장 많다. 8& 표현식에서 첫 번째 조건이 68166인 경우 두 번째 조건은 평가하지 않는다고
가정하면, 가 0인 경우에는 SLj] oF 비교하지 않는다. 따라서 주어진 col] 대해서 이
비교는 1-191 이루어진다. *값의 범위가 8에서 *까지이므로, 총 비교 횟수는 최대로 잡
으면 다음과 같다.

12

Me:

배열이 애초에 내림차순으로 (거꾸로) 정렬되어 있는 경우, 이 비교 횟수가 이 한계치만큼
되는데, 왜 그런지 따져보는 작업은 연습문제로 남겨둔다. 따라서 최악 시간복잡도는 다음
과 같다.

(삽입정렬)에서 키 비교 횟수 기준 평균 시간복잡도 분석

주어진 8에 대해서 cS 삽입할 수 있는 슬롯은 개 있다. 즉    베기 슬조에 머물 수도
an aie gee Ma, G—   2)번째 슬롯      으로 잘 수도 밌그 등등 이던

위치할 확률이 다른 어떤 SRO} 위치할 확듈보다 높다고 믿을만한 이유가 전혀 없다.
따라서 처음 (개 슬롯에 각각 같은 확률을 배정한다. 이는 각 슬롯에 삽입할 확률이 1/7
임을 의미한다. 다음 리스트는 각 슬롯에 eS 삽입하기 위해서 수행하는 비교 횟수를 보여
준다.


===== PAGE 286 =====
274

HEA O] 소개: 정렬문제

chapter 7 계산
슬롯      비교 횟수
2               1
2 1              2
2               21

1     (ae

1 인 이유 는 while 두프를 제어

를 첫 번째 슬롯에 삽입할 때 비교 횟수가 가 아니고 i
하는 HAAS 첫 조건이 j= 0일 때 false7t 되어 둘째 See 계산하지 않기 때문이다.
주어진 iol] 대해서 eS 삽입하는데 필요한 평균 비교 횟수는 다음과 같이 계산한다.

답1키남나 +6-피끔56-패을 그  >

_ 6200 , 11
20     2
_ toed. LE
2   2

따라서 배열을 정렬하는데 필요한 평균 비교 횟수는 다음과 같다.
헤를느느- 회 ~ yu. FN inn,

a
수적인 조작을 가미하여 구한다.

| fae

마지막 등식은 부록 Ao} 예제 &1과 &.9의 결과에다 대
최종적으로 시간복잡도는 다음과 같다.

402) = =e —Inn = a

nN

이제 추가적으로 저장장소를 얼마나 사용하는지 분석해보자.

4

그

i

렬)에서 추가적인 MAA 사용의

입력 배열 의 크기만이 유일하게 저장장

자자

제자리정렬이고, 따라서 추가적인 저장징

Zo

사용량이 nF 함께 증가한다. 이 알고리즘은

사용량은 ㅇ(1)이다.

5 Tere

b  P

 기준으로 하면 ao] 경우와 평균의 경우 삼입정렬의 시간복잡

레코드의 비이” ie
습문제로 증명해보길 권유한다.

도는 다음과
=     a                    fi
테이 IY yee ee


===== PAGE 287 =====
의 경

0000000
가 저장장소 사용량

제자리
제자리
제자리

츠
a

과 같다.

으

"놓았다. 표 7.1에 따르면 비교 횟

타

히

ㄴㄴ

| 00

정리
알고리

cm

레코드 저장 횟수

T(n) = 30
정 시간복잡도
교 Ax

| 제자리정렬이다.

Ko}

7| 비교 횟수

배

=a

사치이다.

으로 삽입

we

속도가 더 빠르다. 돌 다 제자리정렬

즘이다. AHA A(selection sort) 표 7.1에서 비

렬은 명

fo}

xz

고리즘
=
Ald
3

= |

=
a

=
항

보면 더 빠르다. 레코드 저장을 기준으로 따지면 삽입정렬이 최악의 경우와 평균

^ 그
=
때

때

pal.

my

리즘으로 교환정렬의 단점 중 하나를 제거하였다. 이제 선

EE

즈
i=}

>  알고리

00

: 비내림차순으로 nil 키

제

므
때
ra

|스는 1부터 2)

13]

ㅇ
1s

FO] 정수 ㅠ, 키의 배열 6(

이 ㆍ 16
at: 36


===== PAGE 288 =====
@6000000
276     chapter 7 계산복잡도의 소개 :정렬문제

void selectionsort (int n, keytype S{])

{
index 2, j, smallest;
for (7 = 1; i <= n-1; H+4){
smallest = 1;
for G = jf + 1; 7 <= ; F++)
if (S| < S{smallest])
smallest = J;
exchange S{[i] and S{smalles¢]|;
}
}

명백히 선택정렬 알고리즘은 7] 비교 횟수를 기준으로 하면 교환정렬과 시간복잡도가
같다. 그러나 레코드의 저장 횟수로 따지면 완전히 다르다. Sly] 가 9!]보다 작다고 판정
될 때마다 교환정렬(알고리즘 1.9)하듯이 Sli] St 9!7] 를 교환하는 대신, 선택정렬은 ?번
ASE] 번째 슬롯에 있는 키들 중에서 가장 작은 키의 인덱스만 단순히 기억한다. 그
레코드  드를 찾은 후 그 레코드와 i Ha 슬롯에 있는 레코드와 교환한다. 이렇게 하면 for—
Al 번째 패스 후 가장 작은 키가 첫 번째 슬롯에 놓이게 되고, 두 번째 패스
번째 작은 키가 두 번째 슬롯에 놓이게 되고, 등등 이런 식으로 계속 진행한다.
aah  교환정렬과 마찬가지이다. 그러나 for-i 루프의 끝에서 교환이 한 번만 이루어
지므로 전체 교환의 횟수는 정확히 -ㅡ1번이다. 교환을 한 번하는데 SH] 저장이 필요
하므로 레코드의 저장 횟수를 기준으로 하면 모든 경우를 고려한 선택정렬의 일정 시간
복잡도는 다음과 같다.

u
ae

ne

T(n) = 3(n—-1)

교환정렬의 레코드의 저장 횟수는 평균으로 대략 3/.^/4이었음을 기억하자. 따라서 평
균으로 따지면 8차시간을 1차시간으로 대치한 셈이다. 교환정렬이 선택정렬보다 좋을 때

있다. HS 들어, 레코드가 이미 정렬된 경우 교환정렬은 레코드 저장작업을 하지 않
는다:

선택정렬과 삽입정렬을 비교해 보면 어떨까? 표 7.1을 다시 보자. 키의 비교 횟수로
따지면 삽입정렬의 실행속도가 최소한 선택정렬만큼은 항상 빠르고, 평균으로 따지면 더
빠르다. 그러나 레코드 저장 횟수를 기준으로 따지면 선택정렬의 시간복잡도는 1차인데
반해서 삽입정렬은 2차이다. no] 클 때 1차시간은 2차시간보다 훨씬 빠름을 상기한다.
따라서 no] 크고 레코드가 크면(레코드를 대입하는 시간이 많이 소요되면), 선택정렬이
확실히 더 좋다.

순서대로 레코드를 선택하여 적절한 위치에 놓는 정렬 알고리즘

은 크게 분류하여 모두
선택정렬이라고 할 수 있다. 이러게 따지면 교환정렬도 선택정렬의 일종이다. 7.6절에서
공부할 힙정렬도 크게 보면 선택정렬의 일종이다. 그럼에도 알고리즘 7.27} "선택정렬"



===== PAGE 289 =====
7.3 비교 한 Hol] 기껏해야 역이 하나 제거되는 알고리즘의 하한선     277

oh

이라고 하는 대표 이름을 가지는 영예를 안았다.

교환정렬, 삽입정렬, 선택정렬을 비교해본 목적은 정렬 알고리즘을 비교하는 방식을
되도록 쉽게 소개하기 위함이다. 실제로 세 알고리즘 모두 최악 시간복잡도가 2차시간이
기 때문에 엄청나게 많은 ial  as    a iad  어떤 것도 실용적이지 않다.
다음 절에서는 이 부류으                          ore 기준으로 2자시간 미만으로 알고
리즘을 개선하는 건 불가능함을 라니

   a

@ 7.3 비교 한 번에 기껏해야 역이 하나 제거되는 알고리즘의 하한선

비교할 때마다 삽입정렬은 아무 일도 하지 않거나, 키를 /번째 슬롯에서 (+ 1)번째 슬
롯으로 옮긴다. 7번째 슬롯에 있는 키를 하나 위 슬롯에 옮겨 놓음으로써 2가 그 키 앞에
와야 한다는 AMIS 수정하였다. 그러나 이게 삽입정렬 알고리즘이 하는 일의 전부이다.
키만 비교하고 비교 결과에 따라서 재배치하는 정렬 알고리즘은 모두 최소한 8차시간이
필요하다. 정렬할 키가 모두 다르다고 가정하고 얻은 결과이다. 입력의 부분집합을 취하
여 구한 최악의 경우 수행시간의 하한은 전체 입력을 고려해도 마찬가지로 하한이기 때
Bo] 정렬할 키가 모두 다르다고 가정을 없애도 최악의 한계는 그대로이다.

일반적으로 어떤 순서 집합에 속한 서로 다른 키 nS 정렬하는 것만 따져보면 충분
하다. 더구나 정렬할 키를 단순히 FO] 정수인 1, 3, .……, 7이라고 가정해도 일반성을
실하지 않는다. 왜냐하면, 가장 작은 키를 1로 대치하고, 두 번째 작은 키를 8로 대치
고, 이런 식으로 계속 대치할 수 었기 때문이다. 예를 들어, [병칠, 갑돌, 말순|을 보자.
1을 갑돌이와 연관짓고, 2S 말순이와 연관짓고, 3을 병칠이와 연관지어, [3, 1, 이로 바꿀
수 있다. 비교만으로 이 정수들을 정렬하는           의 이름을 정렬하는데 비교
횟수가 같아야 할 것이다.

양의 정수 n HO] (permutation): 그 정수를 순서매기는 것으로 생각할 수 있다.
처음 7개의 양의 정수 순열은 nl 7H] 있기 때문에(&.7절 참조), 그 정수에는 nl HO} 다른
순서가 있다. AS 들어, 다음 6개의 순열은 처음 3개의 양의 정수의 서로 다른 ays
모두 나열해 놓은 것이다.

08 일 068, 일 61 일 281 [61 의 6081
이는 (정렬 알고리즘에서) 7/개의 서로 다른 키를 가진 입력의 SRE ni eke 의미이
다. 이 여섯 개의 순열은 크기가 8인 서로 다른 입력들이다.
BS (hy, ky …, hOB 표시한다. 즉, 《은 PAA 위치에 있는 정수이다. 예를
들어, 순열 [8, 1, 이는 다음과 같이 나타낼 수 있다.

위에"

스연
순열


===== PAGE 290 =====
278

chapter 7 계산복잡도의 소개 :정렬문제

순열에서 A(inversion)-2 다음과 같은 쌍(694)이다.

i< 7이코 k, = 인 0. 6)

oS 들어, 순열 [3, 2, 4, 1, 6, SE (3, 2), B,D, (2, 20, (4, 2, 6 52 역을 가지고
| 역이 없다는 말은     열      된 순서 1 2, .…,

%1이라는 말과 동일하
fe)

은   렬 ㄴ =
는 작업은 순열에서 역이 모두 제거되는 것임을

> Bel 7.1

비교만으로 개의 서로 다른 키를 정렬하고, 비교 한 번에 최대한 역이 하나만 제거되는 알고
리즘은 최악의 경우 최소 비교 횟수가 다음과 같
n(n—-1)
2
평균의 경우 최소 비교 횟수가 다음과 같다.
n(n—-1)
4
증명 : 최악의 경우에 해당하는 결과를 얻기 위해서는 7(ㅁ-ㅡ1)/2개의 4S 가진 순열이 존재
함을 보이면 충분하다. 왜냐하면, 그러한 순열이 있으면 알고리즘은 그 만큼의 역을
하고, 따라서 최소한 그만큼 횟수에 해당하는 비교를 수행해야 하기 때문이다. [n, n-, .…,
2, Io] 그러한 순열인지를 보이는 작업은 연습문제로 YA.

평균의 경우에 해당하는 ATS 얻기 위해서 임의의 순열 6, >, BS 가지고 그 순열
의 전치 순열ㅠ8080080 ,, 4, … 과 짝을 이룬다. 예를 들어, [3, 2, 4, 1, 519] 전
순열은 [5, 1, 4, 2, Jolt}. 7> 이면, 어떤 순열도 그 순열 자체와는 다른 유일한 전치 순열
이 존재한다는 사실을 확신하기는 어렵지 않다. 다음과 같이 정의하자.

ri} st 1과 7 사이의 정수이며, 6 > 이다

순열에서 쌍 (6, 7)은 그 순열이나 그의 전치순열에서 역이지만, 둘 모두에서 역이 되지

als

ag

떠
는 않는다. 1과 n 사이에 그러한 정수의 쌍이 7(04-ㅡ1)/2개 VSS 보이는 작엽은 연습문제로
남겨둔다. 이는 순열과 그의 전치순열에는 합해서 정확하게 7(ㅁ-1)/2개의 Fo] 있다는 의미
이다. 그래서 순열과 그의 전치순열에서 역의 평균 개수는 다음과 같이 된다.

1 - n(n—1) _ n(n—1)

2   2     4

따라서 입력에서 어떤 순열도 나올 확률이 같다고 가정하면, 입력에서 역의 평균 개수도
”01-1)/4개이다. 여기서 알고리즘이 비교 한 번에 최대한 역이 하나 제거된다고 가정하였으
므로, 평균으로 최소한 그만큼의 비교는 해야 역을 모두 제거할 수 있고, 따라서 입력을 정렬

할 수 있다.



===== PAGE 291 =====
@‥ㅇ00000 0
re

|병정렬(재고)          279

ro! @
o&

7.4

렬은 비교 한 번하고 9[7]와 2로 구성된 역을 최대한 하나 제거한다. 따라서
알고리즘                     한 알고리즘의 부류에 속한다. 교환정렬과 선택
정렬도 이 부류에 속하는지 알아내는 것은 조금 더 어렵다. 이 사실이 맞는지를 보기 위
하여 교환정렬의 예를 살펴보자. 먼저, 교환정렬 알고리즘은 다시 써보면 다음과 같다.

하

void exchangesort (int n, keytype 의 ])
{

index i, /;

for) (P= iy f <= 교 1; 7+)

for G= i+ 1; 7 <= 2; #++4)
if (Sj) 주씨 기)
exchange S[i] and SJ;

}

배열 5가 현재 순열 (2, 4, 3, 11 되어 있고, 29} 18 비교한다고 가정하자. 그 비교
후 29} 1을 교환할 것이고, 따라서 역 (2, 2, (4, 2, (8, 1이 제거된다. 그러나 역 (4,
이과 (3, 9/이 추가되므로, 순수하게 제거된 역의 개수는 하나뿐이다. 이 예로 보아 교환
정렬은 한 번 비교 후 전체적으로 기껏해야 하나의 역이 줄어든다.

삽입정렬의 최악 시간복잡도는 4(-1)/8이고, 평균 시간복잡도는 대략 ?”/4이므
로, 비교만으로 정렬하고 한 번 비교 후 최대한 하나의 역만 제거되는 알고리즘으로는
(키의 비교로만 고려하는 B 할 수 있는 만큼의 최고 시간복잡도를 얻은 셈이다. 합병정
렬(알고리즘 2,29} 2,43} 퀵정렬(알고리즘 2,6) 시간복잡도가 이보다 더 좋다. 합병정
렬과 퀵정렬 알고리즘을 다시 한 번 공부해보고, 삽입정렬과 비교하여 어떻게 다른지 살
펴보자.

@ 7.4 합병정렬(재고)

합병정렬은 2.8절에서 소개하였다. 이 절에서는 합병정렬 알고리즘이 비교 한 번에 하나
이상의 역이 제거될 수 있음을 보여줄 예정이다. 그리고 합병정렬 알고리즘의 개선 방안
을 살펴본다

정리 7.12] 증명에서 언급했듯이 비교 한 번에 최대한 역이 하나만 제거되는 알고리즘
은 입력이 역순으로 정렬되어 있을 때 최소한 7(4ㅡ1)/2번 비교한다. 합병정렬2(알고
리즘 2.4)가 그러한 입력을 어떻게 다루는지 그림 7.204] 보여준다. 부분배열 [3 4] [1
2S 합병할 때 비교 한 번에 역이 하나 이상 제거된다. 33} 1을 비교한 후 1을 A 번째
배열 슬롯에 넣으면 역 (3, 1)과 (4, Yo] AARC, 3과 2S 비교한 후 2S 두 번째 배열
슬롯에 넣으면 역 (3, 2)과 (4, 9)가 제거된다.

이 3의 거듭제곱일 때 합병정렬의 최악 시간복잡도를 키의 비교 횟수로 표시하면 다


===== PAGE 292 =====
280

chapter 7 계산복잡도의 소개 :정렬문제

4 3 2 1
/ Divide
4 3    2 1
Divide    Divide
Merge    Merge
3 4    1 2
\ Merge
12 3 4
그림 7.2
음과 같다.

W(n) = 7218 2 - (02 - 1)

이 시간복잡도를 일반적으로 표시하면 ㅇ(2187)이다.

비교 한 번에 하나 이상의 역이 제거되는 정렬 알고리즘을 개발하여 본 이득은 상당하
다. 1.4.1절에서 O(n?) 알고리즘은 매우 큰 입력을 다룰 수 없었던 반면, O(nign) 알
고리즘은 매우 큰 입력도 다룰 수 있었다.

“생성함수(6606『80108 functions)’2] 방법으로 WAALS 풀어서 no] 29] 거듭제곱일
때, 합병정렬의 평균 시간복잡도를 키의 비교 횟수로 표시하면 다음과 같다.

Ign

A(n)=nlgn-—2
iy)= mgm 수애

=nlen—1.26n
이 책에서는 이 HAAS 푸는 방법을 다루지 않겠지만, 궁금한 *he Sahni(1988) 2

AS 참고하기 바란다. 평균의 경우가 최악의 경우보다 많이 좋지는 않다.
합병정렬의 일정 시간복잡도를 레코드의 저장 횟수로 표시하면 대략 다음과 같다.

이제 합병정렬의 저장장소 사용량을 분석해보자.



===== PAGE 293 =====
0 ': 『(합병정렬2)의 추가 저장장소 사용량의 분석
2 an #부했듯이 개량된 합병정렬 알고리즘 2.4조차도 /만큼 크기의 배열이 추가로

asd, 더구나 알고리즘이 첫째 HAE 정렬하는 동안 활성레코드 스틱에 7400,
한다. 배열은 항상 가운데를 나누므로, 스택은
| 87 의 깊이로 자란다. 추가적인 ARES WEG Ae ABI AMES, 고
든 경우를 따졌을 때 추가 저장장소 사용량은 O(n) 레코드이다. ‘O(n) 레코드"란 레코드
의 개수가 @(01)이란 의미이다.

합병정렬 알고리즘을 개선 방식이 세 가지 있다. 첫째는 동적계획 방식이고, 둘째는 링크
된 리스트010600 list) 방식이고, 셋째는 복잡한 합병 알고리즘을 사용하는 방식이다.

첫째 YAS 알아보기 위해서 그림 2.29] 합병정렬을 다시 보자. 머리로 합병정렬을
실행하려 한다면 배열을 분할하는 과정이 사실상 필요 없다. 오히려 단독아이템에서 시
작하여 단독아이템들을 두 개로 된 그룹으로 합병하고, 다시 네 개로 된 그룹으로 합병하
고, 이런 식으로 전체 배열을 다 정렬할 때까지 합병을 계속한다. 이 방법을 반복형 합병
정렬 알고리즘으로 작성할 수 있고, 따라서 ANS 구현하는데 필요한 스택 연산의 비용
Wee 피할 수 있다. 잘 살펴보면 바로 Eason 합병정렬하는 dade 알 수 있
공부해보자. 주목할 점은 배열의 크기를 항상 29] 거듭제
Boe 유지한다는 접이다. 29 ABT 아닌 /값에 대해서는 루프를 2!) 번 반
복하고, n 이후에는 합병하지 않고 처리한다.

꾸

의

> 일고리즘 7.3     합병정렬3 (동적계획)
문제 : 비내림차순으로 ni 키를 정렬
입력 : 양의 정수 n, 키의 배열 9 (인덱스는 1부터 7)
출력 : 비내림차순으로 정렬한 키들로 구성된 배열 S

void mergesort3 (int n, keytype 이 |)

{
int m;
index low, mid, high, size;
m = Q''sn!,                             // 배열 크기를 2의 거듭제곱으로 취급
size = 1;                               // 합병될 부분배열의 크기

repeat (lg mH) {
for (low =1; low <= m-—2* size+ 1; low= low+2* size) {
mid = low + size —1;
high = minimum(low + 2*size—1, n);       // n 이후에는 합병하지 않음


===== PAGE 294 =====
282

}

}

}

chapter 7 계산복잡도의 소개: 정렬문제

merge3 (low, mid, high, S);

size = 2 * size;                        // 부분배열의 크기를 두 배로

이 개선으로 레코드의 저장 횟수도 감소시킬 수 있다. 2/66862(알고리즘 2.5에서 지역
적으로 정의한 배열 UWL 형식으로 인덱스가 1부터 7/까지인 WAS 2408050744에
지역적으로 정의하여 쓰면 된다. repeat 루프를 처음 한 번 통과한 후, 6의 아이템들이
합병된 단독아이템들의 쌍으로 《/에 저장된다. merge2] 끝부분에서 했듯이 이 아이템
들을 다시 에 복사하지 않는다. 대신 다음 repeat 루프를 통과할 때 《/에 있는 아이
템들을 Sz 합병한다. 즉, 두 배열의 역할을 바꾼다. FS repeat 루프에서 계속 역할을
이런 식으로 바꾼다. 이 작업을 수행하는 mergesortI} merges®| 작성은 연습문제로
남겨둔다. 이런 식으로 레코드의 저장 횟수를 OF nig nH] 약 7187으로 줄일 수
있다. 알고리즘 7,39] 일정 시간복잡도를 레코드의 저장 횟수로 표시하면 대략 다음과
같다.

두 번째로 연결 YASS 사용하여 알고리즘을 개량하는 방식을 알아보자. ?.1절에서
부했듯이 정렬문제는 보통 키 값을 기준으로 레코드를 정렬한다. 만약 레코드가 크다

고
면 합병정렬이 사용하는 추가 저장장소 사용량은 상당할 수 있다. 각 레코드에 링크(105)
필 드르

fi

드를 추가하여 추가 저장장소를 절약할 수 있다. 그러면 레코드를 옮기는 대신 링크를
정하여 연결 리스트를 정렬한다. 이는 레코드 배열을 추가로 만들 필요가 없다는 뜻이
링크가 차지하는 공간은 레코드가 차지하는 공간에 비해서 훨씬 작으므로 절약하는
저장장소의 크기는 꽤 된다. 더구나 링크를 조정하는데 드는 시간은 큰 레코드를 옮기는
데 필요한 시간보다 작으므로 시간절약도 된다. 그림 7.8에서 링크를 옮겨서 어떻게 합병
이 이루어지는지 보여준다. 합병정렬과 합병 알고리즘을 묶어서 제시하는데, 이유는 이
제 알고리즘을 분석할 필요가 없기 때문이다. 합병정렬은 가독성을 고려하여 재귀로 작
성한다. 물론 이전에 언급하였던 반복형으로 작성하면 알고리즘을 더 개선할 수 있다.
반복과 Yas 같이 사용하면 US} 6의 AWS 반복하여 바꾸는 개량방법은 적용시킬
필요가 없는데, 그 이유는 연결 리스트를 합병할 때 추가적인 저장장소가 필요없기 때문
이다. 이 알고리즘에서 배열 $9] 아이템에 대한 데이터 타입은 다음과 같다.

struct node

{

keytype key;
index link;

}

a iN



===== PAGE 295 =====
74 합병정렬(재고)          283

(         >        을

3                  5

list1                  list2

G  2    f  0    h  1    e  0    a  6    d  4
key link   key _ link   key link   key — link   key link   key _ link
S[1]     S[2]     S[3]     S[4]     S[5]     S[6]

t     |   t Lo

Merge
(                     들
- 후
mergediist
ㅇ  6    f  0    b  1 J  e  2 J  a  3
key _ link   key link   key _ link   key — link   key link
Sf]     S$ [2]     너티     S[4]     S[5]

t     ‘     _

그림 7.3 das 사용한 합병. 화살표는 링크가 어떻게 작동하는지를 보여
문     ㅅ

2 &
혼돈을 피하기 위해 문자를

『 알고리즘 7.4       병정렬4(연결 리스트 사용)

oe

2

| : 비내림차순으로 n 7 키를 정렬
: 양의 An, 위에 정의한 레코드 배열 SIAL 1부터 n)

: (key) 필드 값들이 비내림차순으로 정렬된 배열 6: 레코드는 링크 필드를 사용한
서 있는 연결 리스트이다.

void mergesort4 (index Jow, index high, index& mergedlist)

{

때 c2 ro
ald

a

(4

index mid, list1, list2;

if low == high) {
mergedlist = low;
S{mergedlist|.link = 0;

else {
mid = | (low + high) /2 |;


===== PAGE 296 =====
@eeeee 0
284   chapter 7 계산복잡도의 소개 :정렬문제

mergesort4 low, mid, 72572);
mergesort4 mid +1, high, List2);
merge4( list1, list?, mergedlist);
}
}

void merge4 (index Jist1, index Jlist?, index& mergedlist)

{

index Jastsorted ;

if (S{listI].key < S{listA.key) {     // 합병된 리스트의 시작부분을 찾는다.
mergedlist = List1;
list] = S\list1|.link ;
}
else {
mergedlist = List2;
list2 = S\list4.link ;
}
lastsorted = mergedlist ;
while (Jist] !1= 0 && List? != 0)
if S[list].key < S[listA.key {    // 작은 키를 합병된 BAEC] 연결한다.
S[lastsorted|.link = list1 ;
lastsorted = list1;
list] = S|list1|.link;
}
else {
S{lastsorted\.link = list2;
lastsorted = list2;
list? = S\list link ;

}
if (Jist1 == 0)                 // 하나의 리스트가 끝난 후,
S{lastsorted\.link = list2;       // 다른 리스트의 남은 부분을 연결한다.
else

S{lastsorted|.link = listl ;

list1°|U+ list27} merge42| 도입부분에서 0914] 검사할 B27} 없다. 왜냐하면, mer-
gesort4= 빈 리스트를 merges 절대 전달하지 않기 때문이다. 알고리즘 2.4(합병정렬
2)2] 경우와 마찬가지로 nw} SE mergesort42] 입력이 아니다. 최상위 호출은 다음과
같다.

mergesort4 (1, n, /797222020)

실행 후 listhronti: 정렬된 리스트에서 3 번째 레코드의 인덱스를 가지고 있을 것이다.
정렬 후 이분검색(알고리즘 2.) 사용하여 키 필드로 빨리 레코드에 접근할 수 있도



===== PAGE 297 =====
@ @
)          285

El @
@

@0 @0 @
75 퀵정렬(재
록 서로 이웃한 배열 슬롯에 정렬된 순서(즉, 보통 방식으로 정렬된 결과)로 레코드를 놓

싶을 때가 종종 있다. 링크에 따라서 일단 레코드가 정렬되면, 제자리 O(n) 알고리즘
을 사용하여 이웃한 배열 슬롯에 정렬된 SAS 재배치하기는 가능하다. 그러한 알고리
즘은 연습문제로 작성해 보도록 한다.

이 개선된 합병정렬로 두 가지를 성취하였다. 첫째, //개의 추가적인 레코드를 7개의
링크만 필요하게 대치하였다. 즉, 다음과 같은 결과를 얻었다.

|
He
ttlo
B=)

합병정렬4)에 대한 추가적인 저장장소 사용량 분석
= cm 고려하면, 추가 저장장소 사용량은 O(n) 링크이다. “O(n) 링크"란 링크
O(n) ole 의미이다.

jo

둘째, 레코드를 서로 이웃한 배열 슬롯에 순서대로 놓을 필요가 없는 경우 레코드의
저장 횟수의 시간복잡도를 0으로, 필요한 경우 0(0)으로 줄인다.

셋째, 개선 알고리즘은 Huangy} Langston(1988)°] 발표한 더 복잡한 합병 알고리즘을
사용하는 것이다. 이 합병 알고리즘도 0(0)이지만, 추가적으로 필요한 저장장소의 양이
작고, 상수이다.

@ 75 퀵정렬(재고)

먼저 퀴정렬 알고리즘을 복습하자.

void guicksort (index Jow, index high)

{

index pivotpoint ;

if (high > low) {
partition(low, high, pivotpoint);
quicksort(low, pivotpoint — 1);
quicksort(pivotpoint + 1, high);
}
}
비록 최악 시간복잡도가 8차시간이기는 하지만, 2.4절에서 보았듯이 키를 비교하는 횟
수를 기준으로 퀵정렬 알고리즘의 평균 시간복잡도는 다음과 같다.

A(n) = 1.38(n+ 1)len

이 시간복잡도는 합병정렬에 비해서 그리 나쁘지 않다. 퀵정렬 알고리즘은 합병정렬에
비해서 추가적인 배열이 필요없다는 장점이 있다. 그러나 그래도 제자리 정렬은 아니다.


===== PAGE 298 =====
286

chapter 7 계산복잡도의 소개: 정렬문제

고, 오른쪽(또는 왼쪽)에 한 아이템 작은 부분배열이 오게 배열이 계속 분할될 지도 모른
다. 이런 ACE 되면, 8 ㅡ1개 쌍의 인덱스가 스택에 쌓이게 되므로, 최악의 경우 추가
저장장소 사용량은 O(n) lth, 추가 저장장소 사용량이 AAAS O (lg n)o] 되도록 퀵정
렬 알고리즘을 개선할 수 있다. 어떻게 개선할지 공부하기 전에 퀵정렬에서 레코드의 저
장 횟수를 기준으로 시간복잡노를 따져보자.

정렬에서 교환하는 평균 횟수는 oF 0.69(n+ 17187 정도가 된다는 사실을 연습문제
로 증명해 보라. 한 번 교환하는데 3번의 대입이 필요하다고 가정하면 퀵정렬에서 레코
드의 저장 APS 기준으로 평균 시간복잡도는 다음과 같다.

ti

A(n) = 2.07(n+1)lgn

퀵정렬이 추가로 사용하는 공간(저장장소)을 줄이는 데는 다섯 가지 방법이 있다. 첫째,
quicksort 프로시저에서 어떤 부분배열이 더 작은지 알아내어 큰 배열을 정렬하는 동안
작은 배열은 스택에 저장해 둔다. 개선한 quicksort7} 사용하는 공간을 분석하면 다음과

므
ㅇ

=
partition®| 배열을 매번 정확하게 반으로 BHAA 공간을 최악으
된다. 이 때 스택의 깊이는 대략 1
량은 60870)개의 인덱스이다.

많이 사용하는 경우가

로
퀵정렬의 추가 공간 사용

09
3
2
ch
a
A
¥
Ni
ㅇ
눌
om 」
30 |

둘째, 연습문제로 보겠지만, 레코드의 평균 저장 횟수를 현저하게 줄이는 개선판 24&-
tition®| 있다. 이 개선판에서 레코드의 저장 횟수를 기준으로 평균 시간복잡도는 다음과
같다.

A(n) = 0.69(n+ 1)lgn

셋째, 프로시저 027049077에서 재귀 호출을 할 때마다 /2~, high, pivotpoint7} 스택
에 쌓이게 된다. 사실 이 값을 모두 매번 스택에 SASS 필요는 없다. quicksortS 처음
재귀 호출하는 동안 /7ㅁ0《770727와 high 값만 스택에 저장하면 충분하다. 다음에 quick-
607를 재귀 호출하는 동안은 아무 것도 저장할 필요가 없다. 이렇게 불필요한 연산을
하지 않기 위해서 quicksort 알고리즘을 재귀 대신 반복(1628402)으로 작성하고, 프로시
저 내에서 스택을 원하는 대로 조작하면 된다. 즉, 재귀 호출로 인해서 스택이 자동 조작



===== PAGE 299 =====
되게 하는 대신, 어떻게 스택을 조작할지 프로시저에 명시한다. 이 알고리즘의 작성도
연습문제로 남겨둔다.

넷째, 2.7절에서 공부한 대로 경계값을 정해놓고 BARS 기준으로 반복 알고리즘과
재귀 알고리즘을 선택적으로 호출하여 전체적인 효율성을 높여서 알고리즘을 개선할 수

다섯째, 알고리즘 3.0(퀵정렬)의 최악의 경우 분석에서 언급했듯이 알고리즘은 입력
배열이 이미 정렬이 되어 있는 경우 효윤이 가장 낮다. 입력 배열이 정렬된 것에 가까우

면 가까울수록 최악의 경우의 성능에 가까워진다. 따라서 배열이 이미 거의 정렬되어 있
다는 Sele] 서면, 첫째 lols 피봇 아이템으로 꼭 Als] 않아도 되게 하여 성능을
향상시킬 수 있다. 이 경우에 사용할 수 있는 좋은 전략으로 9100], S[|(low+ high)
/211, thigh] 2] 미디안006090/을 피봇 값으로 선택하는 방법이 있다. 물론 입력 배열
의 구조에 대해서 전혀 아는 바가 없다면 피봇 아이템으로 아무 아이템이나 선택하는 건
평균적으로 다른 아이템을 선택하는 것과 마찬가지가 된다. 이 경우 미디안을 취하여 실
제로 얻는 이득은 (이 세 값이 모두 다르다고 가정하는 한) 부분배열 중 하나는 비어있지
않다는 확실한 보장이다.

퀵정렬은 전치(\7808200610400)로 정렬하는 알고리즘의 부류에 속한다. 즉, 인접해 있는

레코드를 교환(전치)하여 정렬을 수행한다. 이 Ho] 속하는 2차시간 알고리즘은 버블
41 (Bubblesort)°|4}, 버블정렬은 연습문제로 공부한다.

SAV AVAIL 달리 힙정렬은 제자리 O(n ign) 알고리즘이다. 먼저 힙 구조를
복습하고, 힙을 사용하여 정렬하는데 필요한 기본 힙 연산 루틴들을 설명한다. 그리고
7

k

7.6.1 2] 구조와 기본적인 힙 연산 루틴

트리(~6@8)에서 UT] (node) 2] 깊이는 뿌리마디(8004에서 그 마디로 지는 유일한

상에 있는 이음선(6080/의 개수이고, Belo] 깊이 d= 트리에 속하는 모든 마디의 깊이
최대치이고, 트리에서 잎168)이란 자식마디(24110700)가 없는 마디임을 — 13.5

A 참조). 트리에서 Wea} (internal node)E 최소한 하나의 자식마디가 있다. 즉, 잎이
아닌 마디는 모두 내부마디이다. 완전한 이진트리(600ㅁ720!06 binary 1ㅠ68)는 다음 조건을
반족하는 이진트리이다.

* 내부마디는 모두 자식마디가 두 개 있다.
잎은 모두 깊이가 dole.

1

서어!
a)


===== PAGE 300 =====
288

chapter 7 계산복잡도의 소개: 정렬문제

그림 7.5 힙

본질적으로 완전한 이진트리(68860[139117 complete binary tree) E 다음 조건을 만족하는
이진트리이다.

* 0-ㅡ1의 깊이까지는 완전한 이진트리이다.

* 깊이가 dal 마디는 모두 왼쪽 Bos 모여 있다,

본질적으로 완전한 이진트리는 정의하기 어렵지만, 그럼으로 그 특징을 파악하기는 쉽
다. 그림 7.4의 트리가 본질적으로 완전한 이진트리이다.
이제 Blheap)S 정의해보자. 힙은 HSS 만족하는 본질적으로 완전한 이진트리이다.
e 마디에 저장된 값은 순서가능집합(6ㅠ06760 set: 순서를 매길 수 있는 Ate 구성된
집합)에서 온다.
e 각 마디에 저장된 값은 그의 자식마디에 저장된 값보다 크거나 같다. 이를 힙 성질
(heap property)°]2}31 한다.
그림 7.52] 트리가 힙이다. 현재 정렬을 다루고 있으므로 힙에 저장되어 있는 아이템은
키로 본다.
키를 적절히 배치하여 정렬할 수 있는 힙을 만들었다고 가정하자. 뿌리마디에 저장된
키를 하나씩 제거하면서 힙 성질을 유지시키면 큰 키부터 순서대로 힙에서 Boks 수 있
다. 제거한 마디를 HSS] 번째 SMA 시작하여 배열에 하나씩 위치시키면 비내림차



===== PAGE 301 =====
‥060060000 0
7.6

힙정렬          289

(3) 힙이 아님                  (6) 키 6과 9를 바꿈               (0) 키 6과 7을 바꿈

(»?    (9)

그림 7.6 siftdown 프로시저는 힙 성질을 회복할 때까지 6을 아래로 내린다.

순으로 배열이 정렬된다. 뿌리마디에서 키를 제거한 후, 뿌리마디에 있는 키를 바닥마디
(bottom node) ol] 저장된 키와 바꾸고(바닥마디는 맨 아래 오른쪽 끝에 위치한 WS 뜻한
다), 바닥마디를 지우고, 뿌리마디에 있는 키를 힙 성질이 만족될 때까지 아래로 "내리는
(sift)” siftdown ZBAAS 호출하여 힙 성질을 회복할 수 있다. 내리는 절차를 따라가
보자. 뿌리마디의 키와 뿌리마디의 자식마디의 키 중에 큰 값을 먼저 비교한다. 뿌리마디
의 키가 작으면, 비교한 키들을 서로 교환한다. 마디의 키가 그의 자식마디의 키 중에
큰 값보다 작지 않을 때까지 트리의 아래쪽으로 내려가면서 같은 과정을 반복한다. 그림
7.6에 이 과정이 나타나 있다. 내리는 작업을 하는 의사코드는 다음과 같다.

void siftdown (00006 20                // 실행 전: 뿌리마디를 제외한 HO] BE 마디들은
{                             // 힙 성질을 만족한다.
node parent, largerchild ;             // 실행 후: HE 힙이 된다.

parent = 의 뿌리마디;
largerchild = 큰 키를 가진 24702/의 자식마디;
while (parent2| 7|7} largerchild2| 키보다 작다) {
parent ©] 키와 Jargerchild2|] 키를 교환;
parent = largerchild ;
largerchild = 2 키를 가진 parent2| 자식마디;
}
}

뿌리마디에서 키를 제거하고 힙 성질을 회복하는 알고리즘의 의사코드는 다음과 같다.

keytype root(heap& 2)
"

keytype keyout ;

keyout = 뿌리마디의 7);

바닥마디의 키를 뿌리마디로 gz);            // 바닥마디는 맨 오른쪽에 위치한 잎
바닥마디를 지움 ;
siftdown( H) ;                        // 힙 성질 회복

return keyout ;


===== PAGE 302 =====
0000000
290   chapter 7 계산복잡도의 소개: 정렬문제

개 키로 구성된 힙이 주어지면, 키를 배열 So] 정렬된 순서로 위치시키는 알고리즘

의 의사코드는 다음과 같다.

void removekeys (int n,
heap H,
keytype 5{])

index 7;

ie =i S= 14 i)

SLi] = 20002) ;
}
이제 키들을 가지고 힙을 만드는 일이 남아 있다. 키들로 구성된 본질적으로 완전한
이진트리가 있다고 하자(이 트리가 힙 성질을 만족하는지 따질 필요가 없다). siftdown
을 반복 호출하여 이 트리를 힙으로 변환할 수 있다. 92002은 다음 절차로 연산을 수
행한다. 깊이가 4-1인 하위트리들을 모두 먼저 힙으로 변환하고, 다음에 깊이가 46- 2
인 하워트        두 힙으로 변환하고, .…, 마지막으로 전체트리를 힙으로 변환한다.
이 절차는 그림 7.7에 그림을 보면 쉽게 이해할 수 있고, 의사코드로 표시하면 다음과
같다.
void makeheap (int n, heap& 2)                 // He 결국 힙이 됨
{
index /;
heap Hsub;                                 // Hsub= 결국 힙이 됨
m= 0-1; 7 = 01 a)                 // 트리는 깊이가 0임
for (깊이가 7인 모든 하위트리 25240)
sittdown( Hsub);
}
마지막으로, BIBS 하는 의사코드를 살펴보자(여기서 AE 키가 들어 있는 본질적

으로 완전한 이진트리로 가정한다).
void heapsort (int xn,
heap H,                          // He 결국 힙이 됨
keytye 511)

makeheap(n, H);
removekeys(n, H, 9);

사실 이 4S 알고리즘은 ae] 정렬이 아너다: BS 저장하려떤 주기"공진이 B
하기 때문이다. 그러면 앞에서 거짓말을 한 것인가? 그렇진 않다. 배열로 Bs 구현  느
추가 공간이 필요 없다. (정렬해야 할 키로 구성된) WHS 같은 배열에 저장하여 WS



===== PAGE 303 =====
립정렬     291

(a) 초기 구조

(6) 깊이가 0-1인 하위트리를 2
= ba (9)
Wee

(0) 깊이가 0-2인 왼쪽 하위트리를

그림 7.7 61100\/으로 본질적으로 완전한 이진트리에서 힙을 만드는 과정. 보여준 절차를 거친
깊이가 4-인 오른쪽 하위트리는 반드시 힙이 되어야 하고, 결국 전체 트리도 힙이 되어야

[이
10
Hu

|무
al

ro!
10
Hu
[브
ain

10

rol  mT
oli

다.

구현하는데 사용하고, 하나 이상의 목적으로 같은 배열 슬롯이 결코 동시에 필요하지 않
다는 걸 다음 절에서 보여준다.

7.6.2 힙정렬의 구현

본질적으로 완전한 이진트리에서 뿌리마디는 배열의 첫째 슬롯에 저장하고, 뿌리마디의
을 이 29700 11021

식마디의 윈쪽과 오른쪽 자식마디는 각각 넷째와 다섯째 배열 슬롯에 저장하고, 이런 식

으로 계속하여 실질적으로 완전한 이진트리 전체를 배열로 표현할 수 있다. 그림 759

힙을 HAS 표현하면 그림 7.8과 같다. 임의 마디의 왼쪽 자식마디의 인덱스는 그 마디

인덱스의 두 배이고, 오른쪽 자식마디의 인덱스는 그 마디 인덱스의 두 배보다 1 더 크다.


===== PAGE 304 =====
292     chapter 7 계산복잡도의 소개: 정렬문제
키 30의      키 25의      키 20의      키 18의   키 12의
뿌리마디 자식마디     자식마디     자식마디     자식마디” 자식마디

ㅅㅅ   나     !   로     시     re   때     i‘   ‘al
30 | 25 | 20 | 18 | 12 | 19 | 17 | 16 | 14 | 41
S{1] S[2] S[3] S[4] Ss} S[6] Si[7}] Ss} Sig} Sfid}
그림 7.8 그림 7.5의 |S wae 표현

힙정렬 의사코드를 다시 잘 살펴보자. 애초에 키들은 본질적으로 완전한 이진트리를 이
루고 있어야 한다고 요구한다. 키를 배열에 임의로 위치시키면, 방금 설명한 표현방법대
로 본질적으로 완전한 이진트리로 해석하면 된다. 이 표현방법을 사용한 의사코드는 다
음과 같다.

> 힙 데이터구조

struct heap

{
keytype S{1..7];                        // SQ] 인덱스는 1부터 2까지임
int heapsize ;                             // heapsize= 0부터 2사이의 값만 Fe
i
void siftdown (heap& 4H, index i)               // 레코드의 저장 횟수를 최소화하기 위해서
{                                  // 뿌리마디의 초기 키(880600)는
index parent, largerchild ;                  // 그 키의 최종위치가 결정될 WEI
keytype siftkey:;                            // 어떤 마디에도 저장하지 않는다.

bool spotfound ;

siftkey = H.S{ i];
parent = 1;
spottound = false;
while (2*parent <= H.heapsize && ! spotfound){
if (2*parent < H.heapsize && H.5{2* parent] < H.S{2*parent+1))

largerchild = 2* parent + 1;            // 오른쪽 자식마디의 인덱스는 부모마디
else                               // 인덱스의 두 배보다 1 더 많다.
largerchild = 2* parent ;                 // 왼쪽 자식마디의 인덱스는 부모마디
if (siftkey < H.S{largerchild\) {            // 인덱스의 두 배이다.

H.S{parent| = H.S\largerchild\;
parent = Jlargerchild;

}

else
spottound = true;
}

H.S\{parent| = siftkey ;
5



===== PAGE 305 =====
keytype root (heap& 2)

{

keytype keyout ;

keyout = H.S{1];

2911] = H.S{heapsizel;

Hi. heapsize = H.heapsize— 1,
Siftdown(H, 1);

return keyout ;

}
void removekeys (int n,
heap& 4H,
keytyppe 5{])
{
index /;

1004 f=] 2) ise ia)

Si] = root(H);
}
void makeheap (int n,
heap& 2)
{
index 7;

Fi. heapsize = n;
for ¢ = | a/2 |; 7 == 1; 7- -)
siftdown( H, 1);

// 뿌리마디에서 키를 추출
// 바닥마디의 키를 뿌리마디로 이동
// 바닥마디를 지움

// 힙 성질 회복

// 메모리를 절약하기 위해서
|| He 주스 Ae}
// $2) 인덱스는 1부터 2까지

// He 결국 힙이 됨
// 개 키가 배열 HS} 있다고 가정
// 깊이가 2-1인 자식마디를 가진

// 마지막 마디는 배열의 [2/2 | A
if Sel 있다.

> 알고리즘 7.5

이제 힙정렬 알고리즘을 살펴보자. 이 알고리즘은 정렬할 키가 이미 2..에 있다고 가
정한다. 그림 7.8의 표현법에 따라 본질적으로 완전한 이진트리에 키들을 자동으로 배치
한 셈이다. 본질적으로 완전한 이진트리를 힙으로 만든 후, nA 슬롯에서 시작하여 첫째
슬롯으로 내려오면서 키를 힙에서 제거한다. 출력 배열에도 정렬된 순서대로 위치하게
되므로 힙에 키를 중복해서 덮어써울 가능성이 전혀 없이 ASS 출력 배열로 그대로 사
용할 수 있다. 이같은 전략을 사용하면 다음과 같은 제자리 정렬 알고리즘을 얻게 된다.

힙정렬

문제 : 비내림차순으로 7개 키를 정렬

입력 : fo] Aen, 힙을 배열로 구현한 크기 7의 배열 A
출력 : 비내림차순으로 정렬된 키들을 구성된 배열 ws


===== PAGE 306 =====
@00@000000
294   chapter 7 계산복잡도의 소개 :정렬문제

void Heapsort (int 2, heap& H)

{

makeheap (2, H) ;
removekeys (2, H, H.S) ;

}

(SABO 키의 비교 횟수 기준 최악 시간복잡도 분석

단위연산 : siftdown 프로시저에서 키의 비교

입력크기 : 7 (정렬할 키의 개수)

프로시저 makeheapy} removekeys 는 둘 다 siftdownS 호출한다. 이 두 프로시저를
따로 분석한다. 7,을 29] 거듭제곱으로 가정하고 분석한 뒤, 부록 BO] 정리 BAB 사용하여
그 결과를 모든 no] 대해서 성립한다고 일반화한다.

makeheap2| 분석

본질적으로 완전한 이진트리의 깊이를 dz} 한다. 그림 7.9를 보면, no] 29] 거듭제곱일
때, 트리의 깊이 d= 187이고, 그 깊이에 정확히 하나의 마디가 있고, 그 마디는 0개의
(ancestor)7} 있다. YS 구축할 때, 그 d 수준에 있는 마디의 조상마디가 가지고
모든 키들은 그 마디(수준 do] 있는 마디)가 거기 없는 경우 내리는(641) 횟수보다
 마디(수준 dol] 있는 마디) 더 내리게 될 수 있다. 다른 키들은 모두 그 마디가 거기 없더
라도 내리는 마디의 수가 같다. do] 깊이에 있는 마디가 거기 없는 경우 모든 키를 내리는
마디의 총 개수의 상한을 먼저 구한다. 그 마디는 조상마디의 개수가 0이고 각 조상마디에
있는 키는 한 마디를 더 내리게 될 수 있을 것이므로, 이 상한에 dS 더하여 모든 키가
내리게 되는 마디의 총 개수를 구할 수 있다. 결국 do] 깊이에 있는 마디가 거기 없다면,
초기에 4-1의 깊이에 있는 각 키는 힙을 구축할 때 한 마디도 내리지 않고, 초기에 46- 2

분
대
mus

Of YO
a ol

c

( ) < 201 30 있는
유일한 마디

그림 7.9 7이 2의 거듭제곱인 경우 7개의 마디를 가진 본질적으로 완전한 이진트리에서 그 트리
의 깊이는 0이고, 의 깊이에 있는 마디는 하나 있고, 그 마디는 조상마디가 0개 있다는 사실을
보여주는 예(ㅎ=8인 경우). 그 마디의 조상마디 3개는 “A'S 표시되어 있다.



===== PAGE 307 =====
@0 @0 @   @0 0 @
76 2S   295

의 깊이에 있는 각 키는 기껏해야 한 마디를 내리게 되고, 최종적으로 뿌리마디에 있는
키가 최대한 4- 1 마디를 내리게 될 때까지 계속 이런 식으로 각 마디의 키를 내리게 되는
상한을 구할 수 있다. no] 29] 거듭제곱일 때, 0 = ) < 0를 만족하는 79} Dojo] 있는
마디가 2'개 있다는 사실은 연습문제를 통해서 증명해보도록 하자. 다음 테이블을 보면,
7이 29] 거듭제곱일 때, (0의 깊이에 있는 마디가 거기 없다면) 각 깊이에 있는 마디의
개수와 그 깊이에 있는 키를 내리게 될 마디의 최대 개수가 나와 있다.

깊이      이 깊이에 있는 마디의 개수 키를 내리는 마디의 최대 개수
0                oy                     d-1
1                De                      d-2
9                2                     d-3
7                2!                    0-4-1
0-1              22                      0

따라서 0의 깊이에 마디가 없는 경우 모든 키가 내리게 될 마디의 개수는 최대한 다음과
같다.

=
Dre f= ¢1 )210- Ya) =" -
= 0

마지막 등식은 부록 AS] 예제 ㅅ.8과 ㅅ.5의 결과를 적용하고, 대수 조작에 의해서 성립한
다. 모든 키가 내리게 되는 마디의 총 개수의 실제 상한은 여기에다 dS 더해야 한다. 따라

20-0-1+0=890-1=7-1

두 번째 등식은 n°] 2의 거듭제곱일 때 6= 187이므로 성립한다. 키가 마디 하나를 내릴
때마다, siftdown 프로시저의 while FES 한 번 실행한다. 그 루프를 한 번 실행할 때
마다 두 번 비교하므로, 77104^6/1602에 의해서 행해지는 비교 횟수는 최대한 다음과 같다.
2(n- 1)
1차시간 안에 힙을 구축할 수 oie 사실은 다소 놀라운 결과이다. 1차시간에 키를 제거할
수 있다면, 1차시간 정렬 알고              수 있을 것이다. 그러나 곧 알게 되겠지만 그렇
지 않다.

removekeys2| 분석
그림 7.10을 보면 7 = 8 이고 64= 18 8 = 3 인 경우에 키를 제거하는 과정이 나와 있다. 그


===== PAGE 308 =====
@00@00000 0
296    chapter 7 계산복잡도의 소개: 정렬문제

림 7.10(8)와 00)에서 보듯이 첫째와 넷째 키를 각각 AAS 때 뿌리마디로 옮겨간 키는 최

대한 4-1 = 2개 마디를 내린다. 첫째와 넷째 사이의 두 키도 마찬가지일 것임은 확실하
다. 따라서 처음 네 개 키를 제거할 때 뿌리마디로 Bah 키는 최대한 개 마디를 내린다.

2마디를 내림

2마디를 내림
+ 1마디를 내림
~
(d)                                                       + 1마디를 내림
두
)                                                       } 0마더를 내림

그림 7.10 마디가 8개인 힙에서 키를 제거하는 과정. (3)는 첫째, (6)는 넷째, (는 다섯째, (0)는
여섯째, (6)는 일곱째 키를 제거하는 USS 보여준다. 뿌리마디로 HAZ! 키는 오른쪽에 표시한
마디 수만큼 내리게 된다.



===== PAGE 309 =====
@ @
7.6

그림 7.10(0)와 (0)에서 보듯이 다음 두 키를 각각 AAS 때는 뿌리마디로 옮겨간 키가 최
대한 d—2=174 마디를 내린다. 마지막으로 그림 7.10(8)에서 보듯이 다음 키를 AAS
때는 뿌리마디로 옮겨간 키가 0개 마디를 내린다. 마지막 키를 AAS 때는 내리는 과정이
확실히 필요 없다. 모든 키가 내리는 마디의 총 AS 최대로 다음과 같다.
81
(4)= 9) 92!
j=l
이 결과를 2의 거듭제곱이 되는 임의의 7 값으로 별로 어렵지 않게 확장할 수 있다. 키가
한 마디를 내릴 때마다 siftdown 프로시저의 while F2S 한 번 실행하고, 그 루프를
한 번 실행할 때마다 키를 두 번 비교하기 때문에 removekeys 2 행해지는 키의 비교 횟
수는 최대로 다음과 같다.
=
25110) = 2(d24—24+!42) =2nlgn—4n+4
j=l
첫째 등식은 부록 AS] 예제 4.5의 결과를 적용한 뒤 대수 조작을 하면 성립하고, 둘째 등식
은 n°] 22) 거듭제곱일 때 0=187이라는 사실에 의해서 성립한다.
두 분석의 통합
7706/1602과 removekeys 의 분석 결과를 통합하면 힙정렬에서 키의 비교 SPE nO]
2의 거듭제곱인 경우 최대로 다음과 같다.
2(n—1)+2nlgn—4n+4=2(nlgn—n+1) = 2nlgn
이 횟수만큼 비교를 해야 하는 경우가 존재함을 보이는 작업은 연습문제로 YAE 결론
AOS no] 2의 거듭제곱일 때 최악의 경우 비교 횟수는 다음과 같다.
W(n) = 272 18 n€ O(n lg n)

Wn)°] 궁극적으로 감소하지 않는다고 증명할 수 있다. 따라서 부록 Bo] 정리 BAS 적

용하면 일반적인 nol] 대해서 시간복잡도는 a 같다.
W(n)E O(n lg n)

힙정렬의 평균 시간복잡도를 해석적으로 분석하기는 어려워 보인다. 그러나 실험적인
연구결과에 의하면 평균의 경우가 최악의 경우보다 그렇게 좋지는 않다고 한다. 이는 힙
정렬에서 키의 비교 횟수 기준 평균 시간복잡도는 대략 다음과 같다는 의미가 된다.

A(n) = 2nlgn
힙정렬에서 레코드의 저장 횟수 기준 최악 시간복잡도는 대략 다음과 같다는 사실을
연습문제로 밝혀보기 바란다.


===== PAGE 310 =====
@…‥@00000 0
298    chapter 7 계산복잡도의 소개 :정렬문제

W(n) = nlgn
키 비교의 경우와 마찬가지로 여기서도 평균의 경우가 최악의 경우보다 별로 좋아지지
않는다.
마지막으로 (앞에서 이미 얘기했듯이) 힙정렬의 공간 사용량은 다음과 같다.

> (SABO 추가 공간 사용량의 분석

힙정렬은 제자리 정렬이다. 추가로 필요한 공간은 O(1) ole 의미다.

7284] 언급했듯이 힙정렬은 순서대로 ALES 선택하여 적절한 정렬된 위치에
택한 레코드를 놓아 정렬하므로, 선택정렬의 부류에 속한다. 레코드를 적절한 정렬된

x
위치에 SE AGS removekeysS 호출하여 이루어진다.

@ 7.7 합병정렬, 퀵정렬, 힙정렬의 비교

이 세 알고리즘의 분석 결과는 표 7,20] 요약해놓았다. 힙정렬은 키의 비교 회수와 레코
드의 저장 횟수를 기준으로 하면 평균적으로 퀵정렬보다 나쁘고, 퀵정렬은 추가 공간 사
용량이 최소이기 때문에 보통 힙정렬보다 퀵정렬을 선호한다. 이 책에서 다룬 최초 합병
정렬(알고리즘 2,29} 2.42 전체 입력 레코드 배열 크기만큼의 배열을 추가적으로 사용
하고, 또한 합병정렬은 레코드의 저장 획수가 퀵정렬의 평균보다 항상 3배가량 되기 때
문에 퀵정렬의 키의 비교 횟수가 평균적으로 약간 많음에도 불구하고 퀵정렬을 합병정렬

@ 표 7.2 _0(7187)알고리즘의 분석결과 요약*

A

알고리즘              키 비교               레코드 저장           추가 공간 사용량
합병정렬         (02) =nlgn      T(n) =2nlgn     O(n) 레코드
(알고리즘 2.4)         402) =nlgn
합병정렬             Wn) = 7218 2        T(n) =0'           O(n) Fa
(알고리즘 7.4)         A(n) =nlgn
퀵정렬              Wn) =n?/2                           Align) 인덱스
(개량알고리즘)         A(n) =1.38n 187      A(n) =0.69n lg n
힙정렬                  Wn) = 272 18 7         Wn) =nlgn         제자리

A(n) = 27187     A(n)=nlgn

*분석결과는 근사값이다. 합병정렬과 힙정렬의 평균의 경우는 최악의 경우보다 약간 좋다.
+ 인접한 배열 슬롯에 레코드가 정렬된 순서로 되어 있어야 한다는 요구사항이 주어지면, 최악의 경우가 O(n) o]
된다.



===== PAGE 311 =====
@00600000 0
78 키의 비교만으로 정렬하는 경우의 하한선     299

사라진다. 아직 남아있는 유일한 단점은 링크에 사용하는 공간이 O(n) TS 추가로 필요
하다는 것이다.

°

7.8 키의 비교만으로 정렬하는 경우의 하한선

O(n ign) 알고리즘을 개발하였고, 이는 3차시간 알고리즘에 비해서 상당히 개선된 것
이다. 시간복잡도 차수가 이보다 더 낮은 정렬 알고리즘을 개발할 수 있는가는 물어볼
가치가 있는 질문이다. 키의 비교만으로 정렬한다고 못을 박는 한 더 좋은 알고리즘의
개발은 절대 불가능함을 알아보자.

확률적(0008601640) 정렬 알고리즘에 적용해도 마찬가지 결과가 나오겠지만, 결정적
(deterministic) FA 알고리즘을 가지고 AS 구해본다(확률적 알고리즘과 결정적 알
고리즘에 대해서는 5.3절을 참조하라). 7.3절에서 했듯이 ni 키가 모두 다르다고 가정
하고 결과를 구한다. 더구나 그 절에서 공부했듯이 /개 키가 단순히 양의 정수인 1, 2,

., 7이라고 가정할 수 있다. 왜냐하면 가장 작은 키는 1로, 두 번째 작은 키는 8로, 등등
이런 식으로 대치할 수 있기 때문이다.

7.8.1 정렬 알고리즘의 결정트리

87] 키를 정렬하는 다음 알고리즘을 잘 살펴보자.

void sortthree (keytype S| ])            // SQ] 인덱스는 1부터 3까지이다.

{

keytype a, 200 c;

a= Sl]; b= 시기; ¢ = 시비)

if (a < b)
if (Bb < ic)
S= a, ^ 0;                    // 이 표현은 11] = a 9120] = b; 513] = gS 뜻한다.
else if (a < c)
1S a) 1G. 이
else
S:= & D:
else if (b < oc)
if (a < c)
시 = b ag
else
iS bie a:
else
S = 6 Dia:


===== PAGE 312 =====
300

chapter 7 계산복잡도의 소개 :정렬문제

sortthree 프로시저의 실행을 다음과 같이 이진트리와 연관 지을 수 있다. 의사코드의
WH 앞에 있는 aS} 62] 비교식으로 뿌리마디를 만든다. 뿌리마디의 왼쪽으로는 6 < bs
만족하는 경우 검사할 비교로 자식마디를 만들고, 오른쪽으로는 a > 를 만족하는 경우
검사할 비교로 자식마디를 만든다. 알고리즘의 모든 실행 경로 상에 있는 비교마다 마디
를 하나씩 모두 만들 때까지 트리에 마디를 만들어 내려간다. 정렬된 결과는 잎에 저장되
어 있다. 그림 7.11은 전체 트리를 보여준다. 각 마디마다 다음에 어떤 마디를 방문해야
하는지 결정해야 하므로, 이 트리를 AVE (dccision tree)z}a 한다. 어떤 특정 입력을
JIA\AL sortthree 프로시저를 실행하는 과정은 뿌리마디에서 잎으로의 한 Zest 일치한
다; 이 알고리즘은 입력크기가 8인 입력을 모두 정렬할 수 있으므로, 3개 키의 모든 순열
에 대해서 그에 해당하는 잎이 각각 존재한다.

개 키의 각 순열에 대해서 그 순열을 정렬하는 뿌리마디에서 잎으로의 경로가 존재
하면 그 결정트리는 7개 키를 정렬하는데 유효하다(0810)고 한다. 즉, 크기 7의 입력을
뭐든지 정렬할 수 있다. 예를 들어, 그림 7.11에서 결정트리는 3개 키를 정렬하는데 유효
하다. 그러나 그 트리에서 어느 가지라도 하나 제거하면 더 이상 유효하지 않다. 7개 키
를 정렬하는 결정적 알고리즘은 모두 최소한 하나의 유효결정트리가 존재한다. 그림 7.11
의 결정트리는 902864766 프로시저의 결정트리이고, 그림 7.122] 결정트리는 3개 키를
정렬하는 교환정렬 알고리즘의 결정트리이다(맞는지 지금 따져 보기 바란다). 그 트리에
서 6, 0, c= 11], 912], .913]의 초기값을 의미한다. 예를 들어, 마디에 비교 ㅇ< b"7}
들어있으면, 그 시점의 13]과 912] 값을 비교하는 게 아니고, 현재 c 값이 들어있는 By
열 아이템과 현재 0값이 들어있는 배열 아이템을 비교한다는 뜻이다. 그림 7.12의 트리에

그림 7.11 801 66 프로시저의 결정트리



===== PAGE 313 =====
7.8 키의 비교만으로 정렬하는 경우의 하한선     301

서 비교 “> < 0 가 들어있는 수준 29] 마디는 오른쪽 자식마디가 없다. 그 이유는 그 비교
결과가 40 인 경우 그 마디에 도달하기까지 구한 답과 띠기 때문이다. 즉, 뿌리마디
에서 시작하여 일관성 있게 순서대로 결정을 해서 내려오면 오른쪽 자식마디에는 절대로
ESS 수 없다는 뜻이다. 교환정렬 알고리즘은 그 비교에 대한: 답이 틀림없이 "268 라는

사실을 "모르기" 때문에 이 시점에서 불필요한 비교를 한다. 이런 일들이 부분적으로 al
적인(6400204008)) 정렬 알고리즘이 종종 발생한다. 뿌리마디에서 일관성 있게 순서대로
결정을 해서 모든 잎에 도달할 수 있는 결정트리를 가지친(04060) 결정트리라고 한다.
그림 7.129] 결정트리는 가지친 결정트리인 반면, 방금 언급한 마디에다 오른쪽 자식마

를 추가한다면 비록 유효한 교환정렬 결정트리이기는 하지만 가지친 결정트리는 아니
다. 7개 키를 정렬하는 결정적 알고리즘은 모두 가지친 유효결정트리가 하나 존재한다.
따라서 다음 보조정리가 이를 말해준다.

|   *보조정리 7.1

개 서로 다른 키를 정렬하는 결정 알고리즘은 모두 정확히 !의 잎을 가진 가지친 유효이진
결정트리가 존재한다.

증명 : 방금 언급했듯이 개 키를 정렬하는 어떤 알고리즘도 그에 해당하는 가지친 유효이진
결정트리가 존재한다. 키가 모두 다르다면, 비교의 결과는 항상 “< 아니면 “>"가 된다. 따라서
이 트리의 각 마디는 기껏해야 자식마디가 두 개 있을 수밖에 없으므로, 자연히 이진트리가
된다. 이제 이 트리가 개의 잎을 가지고 NSS 증명해보자. 7개 서로 다른 키를 가진 입력



===== PAGE 314 =====
00000 0 0
chapter 7 계산복잡도의 소개: 정렬문제

302

의 SRE !가지가 있고, *개 서로 다른 키를 정렬하는 결정트리가 유효하면 모든 입력에
대해서 잎이 하나씩 있기 때문에 트리에서 최소한 !개의 잎을 가진다. !개의 다른 각각의
입력에 대해서 트리에 유일한 경로가 존재하고, 가지친 결정트리에서 BE 잎은 틀림없이 도

달가능하기 때문에 트리는 잎이 nl wep 많을 수 없다. 따라서 트리의 잎은 정확히 nl Hole,

보조정리 71S 사용하여 ?!개의 YS 가진 이진트리를 검사하여 7개의 서로 다른 키
를 정렬하는 문제의 하한을 구할 수 있다.

최악의 경우 키 비교 횟수의 하한을 구하기 위해서 다음 보조정리가 필요하다.

*보조정리 7.2
결정트리로 구한 최악의 경우 키 비교 횟수는 그 트리의 깊이와 같다.

증명 : 주어진 입력에 대해서 결정트리로 구한 비교 횟수는 그 입력을 가지고 따라 내려가는
경로 상 eae 개수이다. 내부마디의 개수는 경로의 길이와 같다. 따라서 결정트리로 구한
최악의 경우 키 비교 횟수는 잎까지의 가장 긴 경로의 길이, 즉 결정트리의 깊이이다.

보조정리 7.13} 7.8를 가지고 최악의 경우 하한을 구하기 위해서 nl 7] WS 가진 이진
트리 깊이의 하한 찾기만 하면 된다. Dole] 하한은 다음 보조정리와 정리를 가지고
찾는다.

*보조정리 7.3
이진트리에서 mo] 잎의 개수이고, d7 깊이이면, d= | 1877 ㅣ 이 성립한다.
증명 : dol] 대한 귀납법으로 다음 부등식이 성립함을 먼저 증명한다.

20 > 722                                        (7,1)
이진트리가 완전하지 않으면 새로운 잎을 추가하여 잎의 ASE 늘어나지만 트리의 깊이는
그대로 유지할 수 있다. 따라서 완전한 이진트리에 대하여 부등식 (7.1)이 성립하는지만 증명
하면 된다. 실제로 완전한 이진트리만 따지면 등식이 성립하므로, 등식이 성립하는지 귀납법
으로 증명한다.
귀납기초 : 깊이가 0인 완전이진트리는 뿌리마디와 유일한 잎이 같은 마디가 된다. 따라서 그
트리에서 잎의 개수 me 1이고, 다음 등식이 성립한다.

Ov,

귀납가정 : 깊이가 del 완전이진트리에 대해서 다음 등식이 성립한다고 가정한다.



===== PAGE 315 =====
0000000
78 키의 비교만으로 정렬하는 경우의 하한선   303

2%=m
여기서 m= 잎의 개수이다.
귀납단계 : 깊이가 0+1인 완전이진트리에 대해서 다음 등식이 성립함을 보이면 된다.

2007,

여기서 m' = 잎의 개수이다. 그 트리에서 잎을 모두 제거하면, 깊이가 adel 완전이진트리의
각 잎에 자식마디를 두 개씩 추가하면 추가한 마디가 모두 새로운 Qo] 되면서 깊이가 4+1인
완전이진트리가 된다.
27072 =m’

이 등식과 퀴납가정을 적용하면 다음 SAS 얻는다.

oe 00000
Ae 중명의 완료되었다.
부등식 (7.1)의 양변에 leS 취하면 다음 부등식이 된다.

d=lgm
d= 정수이므로, 다음 부등식이 성립한다
d>[lgm|

> Bel 7.2

비교만으로 개 서로 다른 키를 정렬하는 결정 알고리즘은 최악의 경우 최소한 다음 횟수만큼
은 키를 비교해야 한다.

|1800)|
증명 : 보조정리 7.1에 따르면, 그러한 알고리즘에 해당하는 !개 잎을 가진 가지친 유효이진
결정트리가 존재한다. 보조정리 7.8에 따르면 그 트리의 Bole [ig(n!) |보다 크거나 같다.
보조정리 7,20] 의하면 결정트리 최악의 경우 비교 횟수는 깊이가 된다고 하므로, 이 정리는
성립한다.

함병정렬 최악의 경우 성능, 즉 nlgn—(n—1)3} 이 하한과 어떻게 비교할까? 보조
정리 7.49] 결과를 가지고 비교할 수 있다.

 | *보조정리 7.4
모든 양의 정수 에 대해서 다음 부등식이 성립한다.

lg(n!) > nlgn—1.45n


===== PAGE 316 =====
@“@0 000 0 0
chapter 7 계산복잡도의 소개: 정렬문제

304

증명 : 이 SYS ALS 알아야 이해할 수 있다.
lg(n!) =1812(2-1)(2-2) … (2)1]
= >》)18                    {101 =0이므로}
i=2
SS | ae 은 2 > nlgn—-1.45n
1         102
> Be 7.3

비교만으로 "개 서로 다른 키를 정렬하는 결정 알고리즘은 최악의 경우 최소한 다음 횟수만큼
키를 비교해야 한다.

17 lgn—- 1.45n |

증명 : 정리 7.22 보조정리 7,40] 의해서 성립한다.

합병정렬 최악의 경우 성능인 nig n—(n—1)°] 최적에 가깝다는 사실을 알았다. 이
제 평균의 경우에도 여전히 성립하는지 보자.

7.8.3 평균의 경우 계산복잡도 하한
eae 나올 Seo] 모두 같다고 가정하고 이 결과를 구한다.

개 서로 다른 키를 정렬하는 결정 정렬 알고리즘에 해당하는 가지친 유효이진결정트
리에 (그림 7,122] 트리와 같이) 자식마디가 하나만 있는 비교마디가 있다면, 그 마디를
그의 자식마디로 대치하고, 그 자식마디를 가지 쳐서 원래 트리보다 비교를 덜하면서 정
렬하는 결정트리를 얻을 수 있다. 새 트리의 잎을 제외한 마디는 모두 정확히 자식마디가
개씩 있을 것이다. 잎을 제외한 마디가 모두 정확히 자식마디가 2개씩인 이진트리를 2-
트리(2-\ㅠ66)라고 한다. 다음 보조정리에 이 결과를 요약한다.

*보조정리 7.5

개 서로 다른 키를 정렬하는 가지친 유효이진결정트리에 대해서 그에 해당하는 최소한 원래
트리만큼 효율적인 가지친 유효결정 2-트리가 존재한다.

증명 : 바로 위 문단에서 설명한 논리에 따라서 성립한다.

트리의 외부경로길이(021: External Path Length): 뿌리마디에서 잎으로 가는 모든
경로의 총 길이이다. 예를 들면, 그림 7.1의 트리의 PLS 다음과 같다.

ELPL=2+34+34+3+3+2=16

잎에 도달하기 위해서 결정트리에서 비교하는 횟수는 잎으로의 경로 길이와 같다. 따라



===== PAGE 317 =====
78 키의 비교만으로 정렬하는 경우의 ㅎ

서 결정트리의 EPCS 가능한 모든 입력을 정렬하기 위해서 결정트리에서 비교하는 총
횟수가 된다. 크기가 7인(모든 키는 서로 다르다) ?!개의 다른 입력이 존재하고, 입력은
선택될 확률이 모두 같다고 가정하고 있으므로, 7개 서로 다른 키를 정렬하는 결정트리
에서 비교하는 평균 횟수는 다음과 같다.
EPL
n!

이 결과를 가지고 중요한 보조정리 하나를 증명할 수 있다. 우선 잎이 7』개인 2-트리의
EPL2| 최소값을 minEPL(m)©2= 정의하자. 보조정리는 다음과 같다.

*보조정리 7.6

비교만으로 n7 서로 다른 키를 정렬하는 결정 알고리즘은 평균적으로 키를 최소한 다음 횟수
만큼 비교해야 한다.

minEPL(n!)
nl
증명 : 보조정리 7.19] 따르면 7개 서로 다른 키를 정렬하는 결정       es 모두, 그 알고리
즘에 해당하는 n! 7] 잎을 가진 가지친 유효이진결정트리가 pie          성리 7,30] 따르면,

그 결정트리를 최소한 원래 트리만큼 효율적인 가지친 유효이조  결정 2-   기 트로 변환할 수 있
다. 원래 트리의 잎 개수가 nlolBS, 그 트리에서 구한 2-트리도 잎의 개수가 같아야 한다.
이제 바로 위 문단에서 설명한 elo] 따라서 이 보조정리가 성립한다.

세

보조정리 7.62 가지고 평균의 경우 하한을 구하기 위해서 minEPL(m) 2] 하한을
기만 하면 된다. 이 하한은 다음 4개의 보조정리를 가지고 구한다.

 보조정리 7.7
잎의 개수가 이고 EPLO| minEPL(m) FH 같은 -트리에서 잎은 반드시 바닥에 있는 27H
수준에 위치한다.
증명 : 바닥의 27] FO] 아닌 곳에 잎이 있는 2-트리가 있다고 가정하자. 0를 그 트리의
깊이라 하고, AS 바닥의 27 수준이 아닌 곳에 위치한 잎이라 하며, *를 의 깊이라고 하자.
바닥 수준에 있는 마디는 깊이가 0이므로 다음 부등식이 성립한다.

kad

이 트리가 잎의 개수가 같은 트리 가운데 BPLS 최소화할 수 없음을 잎의 개수가 같으면서
더 작은 EPL 값을 가진 2-트리를 만들어 보여서 증명한다. 그림 ?.18에서와 같이 원래 트리
의 수준 4-1에 있는 잎이 아닌 마디 BS 선택하고, 그 마디의 두 자식마디를 제거하고, 그
두 자식마디를 에 주어서 이를 증명할 수 있다. 새로운 트리는 원래 트리와 잎의 개수가 분


===== PAGE 318 =====
306

chapter 7 계산복잡도의 소개 :정렬문제

10

개 일

(a) m
원래 2-

가진                     (6) m7} 잎을 가진 EPLO|
리                           감소된 새로운 2-트리

11"

+>
Fa
>
+>
Fa
~~

수준 k+1

그림 7.13 (8/와 (D/O 있는 트리는 YO] 개수가 같지만, (6)에 있는 트리가 4이 작다.

명히 같다. 새로운 트리에서는 도 B| 자식마디도 Yo] 아니지만, 원래 트리에서는 잎이다.
따라서 로의 경로 길이와 Bo 자식마디들로의 두 경로의 길이만큼 &이 감소했다. 즉,
다음만큼 EPL] 감소했다.

k+d+d=k+2d
새로운 트리에서 BY 의 두 새로운 자식마더들은 잎이지만, 원래 트리에서는 잎이 아니다.
따라서 EPL] #로의 경로 길이와 의 두 자식마디로의 경로의 길이만큼 증가했다. 즉, 다음
만큼 이 증가했다.

d-1+k+1+k+1=d+2k+1
EPL 값의 변화를 따져보면 다음의 결과를 얻는다.
(d+2k+1)—(k+2d) =k-—d+1 < d—2-—d+1=-1

k<d-20]2R 부등식은 성립한다. APL] 변화값은 So] 되므로, 새로운 트리의 PL 같이
더 작다. 결론적으로 원래 트리는 잎의 개수가 같은 트리가지고 APL MS 최소화 할 수 없다.



===== PAGE 319 =====
0000000
78 키의 비교만으로 정렬하는 경우의 하한선    307

| *보조정리 7.8

잎의 개수가 이고 EPL 값이 minEPL(m)z} 같은 2-트리는 반드시 다음과 같은 개수의
잎을 가지고,

수준 4-1에서 2-ㅠ개

수준 doy] 2m —24
더 이상 잎은 없다. 여기서 는 트리의 깊이이다.
증명 : 보조정리 7.7에 따르면 잎은 모두 바닥에 있는 두 수준에 위치하고 있고, 2-트리에서
glo] 아닌 마디는 반드시 자식마디가 둘 있으므로, 틀림없이 수준 4-1에 마디가 2 '개 있
다. 따라서 ro] 수준 4-1에 잎의 개수가 이면, 그 수준에 잎이 아닌 마디의 개수는 28 ㄱ-
이다. 8-트리에서 잎이 아닌 마디는 정확히 3개의 자식마디를 가지고 있으므로 수준 4-1에
있는 Yo] 아닌 모든 마디에 대해서 수준 ao} 잎이 두 개씩 있다. 이 잎이 수준 에 있는 HS
한 잎이므로 수준 do] 있는 WO] 개수는 202 ^-7) 과 같다. 보조정리 7.7에 따르면 잎은 모두
수준 d 아니면, 0-1에 있으므로 다음 등식이 성립한다.

r+2(2¢-!-r)=m

이 등식을 간단히 하면, 다음과 같다.
r=24-m

따라서 수준 0에 있는 잎의 개수는 다음과 같다.

m—(24—m) = 2772 - 20

*보조정리 7.9

잎의 개수가 이고, EPLO| 770174/2(70)과 같은 모든 2-트리에 대해서 깊이 d= 다음과
ae

d=[lgm|
증명 : mo] 29) 거듭제곱인 경우를 증명한다. 일반적인 경우에 대한 SRS 연습문제도 남겨
둔다. mo} 29] 거듭제곱이면,임의의 정수 ko 대해서 다음 등식이 성립한다.
772 = 2“

d& 최소화하는 트리의 깊이라고 하자. 보조정리 7.8에서와 마찬가지로, 7을 수준 4-1에 있
는 잎의 개수라고 하자. 그 보조정리에 의하면 다음 등석이 성립한다.

"= 20ㅡ12 = 900 ㅡ95

r> 0이므로, d>k7} 반드시 성립한다. 4 >*로 가정하고 BES 유도하여 증명한다. d>k


===== PAGE 320 =====
@006006000 0
chapter 7 계산복잡도의 소개: 정렬문제

308

이면, 다음 부등식이 성립한다.

= 00-아6 > oFt1_ok = 20 =

『흐ㅠ이므로, 이는 7=77이고, 잎은 모두 수준 4-1에 있음을 뜻한다. 그러나 수준 0에도
반드시 glo] 있어야 한다. 모순이 유도되었으므로 4=《*임을 알 수 있고, 따라서 7=0이 된다.
“= 0희므로, 다음 등식이 성립한다.

24-m=0

따라서 4=187이 된다. mo] 29] 거듭제곱이면, gm =[1gm] az 증명이 완료되었다.

4 BAP 7.10
212 BE 정수에 대해서 다음 부등식이 성립한다.
minEPL(m) =m|lgm|
증명 : 보조정리 7,80] 의하면 이 EPLS 최소화하는 2-트리는 모두 수준 4-1에 잎이 -
H 있고, 수준 dol] Qo] 272 -2“개 있고, 그 이외에 다른 잎은 없다. 따라서 다음 등식을 …
minEPL(m) =(24—m)(d—1)+(2m—2*)d=md+m-—2!
그러므로 보조정리 7.9에 의하여 다음 등식을 얻는다.
minEPL(m) =m/([lgm])+m—2"m

m0] 8의 거듭제곱이면 이 식은 m lg ms} 분명히 같고, 이 경우 ㅠ[1877와도 같다. mo}
29] 거듭제곱이 아니면, [igm]=L1gm]+10] 된다. 따라서 이 경우 다음과 같은 등식을 al
는다.

N

minEPL(m) =m(|lgm|+1)+m—2!sml
=m\|lgm|+2m—2!8"> m|1g m |

일반적으로 Im > 210이므로, 이 부등식이 성립한다. 증명이 완료되었다.

이제 minEPL(m) 2] 하한을 구했으니 최종 결과를 증명할 수 있다.

> 정리 7.4

비교만으로 7개 서로 다른 키를 정렬하는 결정 알고리즘은 평균의 경우 최소한 키를 다음 횟
수만큼 비교해야 한다.

17 들 1.45n |

명 : 보조정리 7.60] 의하면, 그러한 알고리즘은 평균의 경우 최소한 키를 다음 횟수만큼

oly



===== PAGE 321 =====
@
7.9 분배에 의한 정렬(기수정렬)    309

비교해야 한다.
minEPL(n!)
ni

보조정리 7,100] 의하여 이 식은 다음 값보다 크거나 같다.

이제 보조정리 7.4에 의하여 증명이 완료되었다.

합병정렬 Bt 경우 성능인 약 nign—1.26n2 비교만으로 정렬하는 알고리즘으
로는 거의 최적임을 이제 알았다.

7.9 분배에 의한 정렬(기수정렬)

앞 절에서 비교만으로 정렬하는 알고리즘은 O(nlgn) B4 좋을 수가 없음을 증명했다.
순서를 매길 수 있다는 것 이외에 키에 대해서 전혀 모르면, 키를 비교하는 방법이외에는
선택의 여지가 없다. 그러나 키에 대한 정보를 더 아는 경우에는 다른 방식의 정렬 알고
리즘도 고려해 볼 수 있다. 키에 관한 추가적인 정보를 사용하는 알고리즘을 하나 만들어
보자.

키가 10진수로 모두 음이 아닌 정수라는 사실을 안다고 하자. 숫자(4914의 개수가 모
두 같다고 가정하면, 먼저 가장 왼쪽에 있는 숫자의 값을 기준으로 서로 다른 더미(616)
로 키를 분배할 수 있다. 즉, 가장 왼쪽에 있는 숫자의 값이 같은 키는 같은 더미에 놓는
다. 그리고 각 파일은 다시 왼쪽에서 둘째 숫자를 기준으로 서로 다른 더미로 다시 키를
분배한다. 그러면 새로운 각 더미는 다시 왼쪽에서 셋째 숫자를 기준으로 서로 다른 더미
로 다시 키를 분배하고, 이런 식으로 계속한다. 모든 숫자에 대한 검사가 끝나면, 키는
정렬된다. 그림 7.14에서 이 절차를 예를 들어 보여주는데, 키가 더미로 분배되므로 “분
배에 의한 AA(sorting by 01812104[102) 이라고 한다.

이 절차의 단점은 더미의 개수가 일정하지 않다는 것이다. 정확하게 10개의 더미만 할
당하고(각 10진 숫자마다 하나씩), 오른쪽에서 왼쪽으로 숫자를 검사하고, 항상 검사할

당시의 숫자에 따라서 더미에 키를 놓는다고 가정하자. 이렇게 하면 다음 규칙을 준수하
는 한 키는 저절로 정렬이 되어버린다. 각 패스6869)마다 두 개 키를 같은 더미에 놓게
되면 (이전 패스에서) 왼쪽 더미에서 온 키를 다른 키의 왼쪽에 놓는다. 이 절차는 그림
7.15에 예를 들어 보여준다. 어떻게 키를 놓는지를 보여주는 예로서, 첫째 패스 이후에
키 416은 키 3172] 왼쪽 더미에 있다. 따라서 둘째 패스에 첫째 더미에 둘 다 놓을

키 AGS 키 3172] 왼쪽에 놓는다. 그러나 셋째 패스에서 키 416은 넷째 더미에 놓는 반면
키 3172 셋째 더미에 놓으므로 결국 키 4160] 키 3179] 오른쪽에 놓이게 된다. 이런 식으


===== PAGE 322 =====
310

chapter 7 계산복잡도의 소개 :정렬문제

전력한 A

= 고보         239 234 879 878 123 358 416 317 137 225

가장 왼쪽              1          \ \

ENS 기준   123 137   239 234 225        358 317   416   879 878
으로 분배한 수

왼쪽에서               Y                         Y       Y
둘째 숫자를
도시 개  123| |137| |225| |239 234| |317| |358| |416| |879 878

분배한 수

왼쪽에서  '  \  '     Y  Y
셋째 숫자를 |129| |137| | 225] |234| | 239] |317| | 358] |416| |878| | 879
기준으로
분배한 수

그림 7.14 숫자를 왼쪽에서 오른쪽으로 검사하는 분배에 의한 정렬

로 첫째 패스 이후에 가장 오른쪽에 있는 숫자를 기준으로 순서대로 정렬되며, 둘째 패스
이후에 오른쪽에서 둘째 숫자를 기준으로 순서대로 정렬되며, 셋째 패스 이후에 오른쪽
에서 셋째 숫자를 기준으로 순서대로 정렬되고, 결과적으로 정렬이 끝나게 된다.

이 방법은 컴퓨터가 생겨나기 이전부터 사용했던 방법으로, 과거의 카드정렬 기계에서
사용하던 방법이었다. 키를 정렬하는데 사용한 정보가 특정 기수(68018, 0886/이기 때문
에 기수정렬(0801 8010)이라고 한다. 기수는 4>(number base)7} 될 수도 있고, 알파벳이
될 수도 있다. 더미의 개수는 기수와 같다. 예를 들어, 164]4>(hexadecimal) 수를 정렬하
Al 되면 더미의 개수는 16°] 되고, 영어 알파벳으로 표현된 키를 정렬하게 되면 알파벳에
는 문자가 26개 있으므로 더미의 개수는 26°] 된다.

특정 더미에 있는 키의 개수는 각 패스마다 바뀌므로 연결 BASS 사용하면 이 알고

즘을 용이하게 구현할 수 있다. 각 더미는 연결 리스트로 표현한다. 각 패스 이후 FS
하나의 마스터 연결 FASS 합하여 리스트(더미)에서 키를 AAS. 키가 AAS 리스
트(더미) 안의 순서에 따라서 그 리스트에서 순서가 결정된다. 다음 패스에서 마스터 리
스트는 처음부터 순서대로 검사하며, 각 키는 그 패스에서 속하게 되는 리스트(더미)의
맨 뒤에 놓는다. 이런 식으로 주어진 규칙을 그냥 따르기만 하면 된다. 가독성을 높이기
위해서 키는 10진수로 표현된 음이 아닌 정수라 가정하고 알고리즘을 제시한다. 시간복
잡도 차수에 영향을 미치지 않고 다음 기수로 표현된 키도 정렬하도록 쉽게 수정할 수
있다. 알고리즘에 다음 선언이 필요하다.



===== PAGE 323 =====
@0 @   @0@0 0 @
7.9 분배에 의한 정렬(기수정렬)    311

ow
mua
na
+

239 234 879 879 123 358 416 317 137 225

으로 분배한

가장 오른쪽
STS 기준  HU 123|| 234||225]| 416|| 317 137 || 878 358 || 239 879
we
"942 3 4 5 6  7   8   9

오른쪽에서
둘째 숫자를
eo   | 416 317 || 123 225 || 234 137 239 [| 260]| | 878 879 때
분배한 수    0   1     2     3   4 5 6   7   00

오른쪽에서
셋째 숫자를   | 123 137 || 225 234 239 || 317 358 || 416 Wa 878 879 |
기준으로

0

분배한 수      1     2     3   4 5 6 7  8  9

urs

그림 7.15 숫자를 오른쪽에서 왼쪽으로 검사하는 분배에 의한 정렬

struct nodetype

{
keytype key;
nodetype * link;
hs

typedef nodetype * node_ pointer;
EES 기수정렬
입력 : So] 아닌 정수 7/개로 된 연결 리스트 masterlist, 각 정수에서 십진수의 최대

는 정수 numdigits

출력 : 비내림차순으로 정렬된 정수로 된 연결 리스트 masterlist

‘i
a
:

void radixsort (node_pointer& masterlist,
int numdigits)
{

index 27;

7ㅁ006 _7ㅁ01016 45000..9] ;

for (7 = 1; i <= numdigits; i++){
distribute( masterlist, i) ;
coalesce( masterlist) ;


===== PAGE 324 =====
0000000
312    chapter 7 계산복잡도의 소개 :정렬문제

}
}

void distribute(node_pointer& masterlist, index 1) ;
{

index /;

node_ pointer p;

for (/ = 0; 7 <= 9; j++)
List| 7] = NULL;

Pp = masterlist ;

while (p != NULL) {
J = p ->keyA| (오른쪽에서) MAA 숫자의 값;
를 450[./]의 끝에 링크;
p= p ->Ilink;

}

}

void coalesce(node_pointer& masterlist) ;

{

index /;

masterlist = NULL;
for Gj = 0; 7 <= 9; j++)
list 있는 마디들을 masterlist2| 끝에 링크;

// 는 검사하는 당시 숫자의 인덱스

// 더미를 비운다.

// masterlistS 처음부터 순서대로 검사

// masterlistS 비운다.

이제 이 알고리즘을 분석해보자.

간복잡도 분

즘은 키를 비교하지 않기 때문에 다른 단위연산을 찾아야 한다. 00&-
lesceS BEALS 구현하기 위해서 더미를 포함하는 리스트의 시작과 끝 부분에 모두
포인터를 두어 리스트를 처음부터 끝까지 따라가지 않도록 이전 리스트의 끝에 각 리스트
를 바로 추가하도록 할 수 있다. 따라서 그 프로시저에서 for 루프를 한 번 수행할 때마다
단순히 한 포인터 변수에 FAS 저장하여 YASS 224680776?의 끝에 추가한다. 이 저장

masterlist 전체를 처음부터 차례로 따라가려면 항상 0757770776의 while 루프를 nd 실

행해야 한다. masterliste] 리스트를 모두 추가하려면 항상 coalesce] for 루프를 10번



===== PAGE 325 =====
실행해야 한다. 이 프로시저들은 각각 7207~9077에서 77272707876번 호출된다. 따라서 분
석 결과는 다음과 같다.                                             」

T(n) = numdigits(n+10) € O(numdigits × n)

numdigits?| n& 기준으로 한계치를 표현하기 때문에 이 알고리즘은 O(n) 알고리
이 아니다. numdigits 값을 임의로 크게 하여 n& 기준으로 임의로 큰 시간복잡도를
들 수 있다. aS 들어, 1000,000,000은 숫자가 10개이므로 가장 = 수가 1000,000,000
이면 10개 수를 정렬하는데 O(n”) 시간이 걸릴 것이다. 실상황에서 숫자의 개수는 보통
수의 개수보다 훨씬 작다. 예를 들어, 1000,000개의 주민증록번호를 정렬한다면, 7은
1.000,000인 반면 numdigits= 9밖에 되지 않는다. 키가 모두 서로 다를 때 기수정렬의
최선 시간복잡도는 ㅇ(187)이고, 실전에서 거의 최선의 경우가 된다는 사실을 알아내
기는 그리 어렵지 않다.

다음에는 기수정렬이 사용하는 추가 공간을 분석해보자.

ae | 『(기수정렬)의 추가 공간 사용량 분석
masterlist2} 더미를 나타내는 리스트에서 동시에 하나의 키가 필요한 경우는 절대 없으므

로, 새로운 노드는 절대 할당하지 않는다. 이는 연결 리스트에서 처음 키를 표현하는데 필
요한 공간이 유일하게 사용하는 추가 공간이다. 따라서 추가 공간은 O(n) 7] 링크이다.
여기서 O(n) 링크"란 링크의 개수가 O(n) Oo} 의미이다.

[무 oly

@ 연습문제

7.1과 7.2절
1. 삽입정렬 알고리즘(알고리즘 7,)S 구현하여 실행해보고, 여러 개의 문제 사례를 가지고 최
선, 평균, 최악 시간복잡도를 구해보시오.
2. AIA 알고리즘(알고리즘 7.1에서는 입력키가 비올림차순으로 정렬되어 있는 경우 비교
횟수가 최대가 됨을 증명하시오.
3. 삽입정렬 알고리즘(알고리즘 ?.1에서 레코드의 저장 횟수를 기준으로 최악 시간복잡도와
평균 시간복잡도는 다음과 같음을 증명하시오.

_ (n+4)(n-1)_ 77      _n(n+7) ._ nt
aes eee a 오구    ie

4. 교환정렬 알고리즘(알고리즘 1,3) 레코드의 저장 횟수를 기준으로 최악 시간복잡도와
평균 시간복잡도는 다음과 같음을 증명하시오.



===== PAGE 326 =====
314

chapter 7 계산복잡도의 소개 :정렬문제

Wn) = 3n(n—1) Agi 3n(n—7)

5. 교환정렬(알고리즘 1.9)과 삽입정렬(알고리즘 7.1)의 최선 시간복잡도를 비교하시오.

6. 개 키의 리스트에서 비올림차순으로 《번째 큰(또는 비내림차순으로 《번째 작은) 키를 찾
을 때 교환정렬(알고리즘 1.9)이나 삽입정렬(알고리즘 7.) 중에서 어떤 알고리즘이 더 적절
한가? 그리고 왜 그런 답이 나오는지를 밝히시오.

7. 삼입정렬 알고리즘(알고리즘 7S 다음 요구사항 대로 재작성하시오. 어떤 키보다도 작은
값을 가진 배열 슬롯 910|을 추가한다. 이렇게 하면 while 루프의 맨 위에서 )와 0을 비교
할 필요가 없다. 새로운 만든 알고리즘의 정확한 시간복잡도를 구하시오. 알고리즘 7.1의
시간복잡도와 비교하면 더 좋은가 나쁜가? 어떤 알고리즘이 더 효율적인가? 그리고 왜 그런
답이 나오는지를 밝히시오.

8. 셀 정렬(6461 8000라고 하는 알고리즘은 리스트에 있는 아이템의 순서를 이용하는 삼입정
렬의 역량에 영감을 받았다. A 정렬에서는 어떤 수 hol] 대해서 전체 리스트를 아이템들
사이의 거리가 만큼 떨어진 이웃하지 않은 부분 리스트로 분할한다. 각 부분 리스트

rir
Ir a

입정렬을 사용하여 정렬한다. 다음 패스에서 /의 값은 감소하고, 각 부분 리스트의 크기는
증가한다. 각 / 같은 이전 값에 상대적으로 소수(60106)가 되도록 선택한다. 마지막 패스에
서는 AMOR 1을 사용하여 리스트를 정렬한다. 셀 정렬 알고리즘을 작성하고, 그 성능을

분석하고, 삽입정렬의 성능과 비교하시오.

7.3절
9. 4 [n, n-1, … 2, 1]의 역이 n(n—1)/27] 존재함을 증명하시오.

10. 순열 [2, 5, 1, 6, 3, 41의 전치순열을 구하고, 두 순열의 역 개수를 찾으시오. 역은 총 몇
개인가?

11. SAS 매길 수 있는 "개 서로 다른 원소의 순열에서 그 전치순열의 역이 7(4-1)/2개 존
재함을 증명하시오

12. 어떤 순열과 그의 전치순열에서 역의 총 개수가 n(n—-1)/29S 증명하시오. 이 결과를 사
용하여 연습문제 10의 순열과 그의 전치순열 역의 총 ASS 구하시오.

)

olN

너

7.4절(2.2절의 연습문제 참

13. 2.283} ?.4절에서 공부한 두 개의 다른 합병정렬 알고리즘을 구현하여 실행해보고, 여러
개의 문제 사례를 가지고 최선, 평균, 최악 시간복잡도를 조사하시오.

14. 합병정렬 알고리즘(알고리즘 8.8와 2.4에서 레코드의 저장 횟수를 기준으로 할 때 시간복
잡도는 대략 Tn) =27187이 BS 증명하시오.

pl

15. 합병정렬 4 알고리즘(알고리즘 7.408 구축한 AA 리스트를 입력으로 받아서고, 7] 값에
따라서 작은 값부터 차례로 이웃하는 배열 슬롯에 레코드를 저장하는 제자리, 1차시간 알고
리즘을 작성하시오.

16. 분할정복법을 사용하여 반복 합병정렬 알고리즘을 작성하시오. 작성한 알고리즘을 분석하
고, HS 차수 표기범으로 표시하시오. 이 알고리즘을 작성하기 위해서는 스택을 명시적으



===== PAGE 327 =====
유지할 필요가 있음을 유의하시오
17. 연습문제 162] 반복 합병정렬 알고리즘을
행해보고, 연습문제 19의 재귀 합병정렬의 결과와 비교하시오

하고, 연습문제 13의 문제 사례를 가지고

18. repeat 루프를 수행하는 각 패스에서 두 배열 SL} US] 역할이 바뀌도록 22008050770(알고

리즘 7.9)와 그와 관계있는 merges 알고리즘을 재작성하시오.

7.5절(2.4절의 ee dl
19. 2.4절에서 공부한 AA
제 사례를 eae   최선, 평균, 최악 시간복잡도를 구해보시오.

렬 알고리즘(알고리즘 2.6)을 구현하여 실행시켜보고, 여러 개의 =

20. 퀵정렬 알고리즘에서 평균적인 교환 횟수를 기준으로 한 시간복잡도는 HEF 0.69(n +

21. 반복 퀴정렬 알고리즘을 작성하시오. 작성한 알고리즘을 분석하고, WS 차수 표기법으로
이

22.    연습문제 28의 반복 퀵정렬 알고
시켜보고, 연습문제 20의 재귀 키정렬의 결과와 비교하시오.

시

JSS 작성하기 위해서는 스택을 명시적으로 유지할 필요가 있음

을 구현하고, 연습문제 209] 문제 사례를 가지고 실행

23. 다음은 더 효율적으로(빠르게) 실행되도록 구현한 28777007 프로시저인데, quicksort 프로

시저가 호출한다.

void partition (index Jow, index high, index& povotpoint)

{

index i, ./ ; keytype pivotitem ;

pivotitem = S{low| ; i= low; j= high+1;
do

I++ ;
while (i< high && S{ i]<= pivotitem) ;
do

J-~3
while (5[j]> pivotitem) ;
while (i< J) {

exchange S[i] and S{/];

do
퍼기
while (51 7 ]<= pivotitem) ;
00
—
while (5[ j]> pivotitem) ;
i
pivotpoint = ./ ;
Slhigh|2} S{pivotpoint|S 교환 ;         // pivotitem pivotpoint} 넣음


===== PAGE 328 =====
‥06@000000
chapter 7 계산복잡도의 소개 :정렬문제

316

24.
25.

이 partition ZBA)Z|S 사용하는 퀵정렬에서 레코드의 저장 횟수를 기준으로 할 때 시간복
잡도는 다음과 같음을 증명하시오.

A(n) = 0.69(n+1)lgn
그리고 키의 비교 횟수를 기준으로 한 평균 시간복잡도는 이전과 거의 같음을 증명하시오.
퀵정렬 알고리즘이 최선의 선택이 되는 두 사례를 드시오.
순서가 HMA 키를 교환하여 리스트를 정렬하는 또 하나의 방법으로 버블정렬이 있다. 버
블정렬은 인접한 레코드 쌍을 훌어보고, 순서가 FBI 키가 있으면 교환한다. 리스트를 한
번 Ba 나면, 가장 큰 (또는 가장 작은) 레코드가 제 위치로 간다. 리스트가 완전히 정렬될
때까지 정렬되지 않고 남은 부분에 대해서 이 과정을 반복한다. 버블정렬 알고리즘을 작성
하시오. 작성한 알고리즘을 분석하고, 결과를 차수 표기법으로 표시하시오. 버블정렬 알고
리즘 Bes 합병정렬, 교환정렬, 선택정렬의 성능과 비교하시오.

7.6절

26.

2.

28.
29.

30.

31.

32.

본질적으로 완전한 이진트리가 힙인지를 검사하는 알고리즘을 작성하시오. 작성한 알고리
Se 분석하고, 결과를 차수 표기법으로 표시하시오.

깊이가 0이고, 개63의 ASA HS 가진 힙에서 7 < 0가 되는 깊이 )에는 2'개 마디
가 존재함을 증명하시오.

개 마디를 가진 힙에는 [7/2|개 잎이 USS 증명하시오.

힙정렬 알고리즘(알고리즘 7.5. 구현하여 실행해보고, 여러 개의 문제 사례를 가지고 최
선, 평균, 최악 시간복잡도를 구하시오.

힙정렬의 최악 시간복잡도가 Wn) ~ 2nlen © O(nign)o] 되는 경우가 USS 증명하시
ay

힙정렬에서 레코드의 저장 APS 기준으로 한 최악 시간복잡도가 약 Wn) ~ nlends
증명하시오.

가장 큰 키부터 시작하여 제일 큰 키 WHE 찾은 후 PRES 힙정렬 알고리즘을 수정하시
오. 수정한 알고리즘을 분석하고, 결과를 차수 표기법으로 표시하시오.

7.74

33.

34.

35.

키의 비교 횟수와 레코드의 저장 횟수를 기준으로, 이 장에서 설명한 모든 정렬 알고리즘의
장점과 단점을 모두 나열하시오.

이 장에서 설명한 정렬 알고리즘을 구현하고, 여러 개의 문제 사례를 가지고 실행시켜 보시
오. 그 결과와 연습문제 34에서 얻은 정보를 사용하여 이 정렬 알고리즘들을 자세히 비교하
시오.

아래의 상황과 같은 리스트를 정렬하려면, 선택정렬, 삽입정렬, 합병정렬, 퀵정렬, 힙정렬
중에서 어느 알고리즘을 선택할 것인가? 그리고 왜 그런 Ho] 나오는지를 밝히시오.

(9) 리스트는 수백 개 레코드로 구성되어 있다. 레코드 자체는 꽤 길지만, 키는 아주 짧다.
0) 리스트는 약 45,000개 레코드로 구성되어 있다. 어떤 경우라도 상당히 빨리 정렬을 끝낼



===== PAGE 329 =====
필요가 있다. 메모리는 45,000개 레코드를 간신히 저장할 만큼밖에 없다.

(0) 리스트는 약 45,000개 레코드로 구성되어 있지만, 순서가 VY 레코드는 조금밖에 없다.

(4) 리스트는 OF 25,000개 레코드로 구성되어 있다. 평균적으로 가능한 빨리 정렬을 끝내면
좋겠지만, 꼭 모든 경우에 정렬을 빨리 끝내야 한다는 사실이 중요한 것은 아니다.

36. 이 장에서 설명한 (키의 비교를 기준으로) 각 정렬 알고리즘에 대해서 그 알고리즘을 선택하
면 가장 적절하게 되는 사례를 최소한 두 개씩 드시오.

7.8절

37. 1부터 7까지(1과 7 모두 포함) 정수의 순열을 정렬하는 1차시간 알고리즘을 작성하시오.
(Hd: 크기가 인 WSS 사용하시오.)

38. 연습문제 88에서 작성한 알고리즘의 성능이 1차시간이므로 비교만으로 정렬하는 정렬 문제
의 하한을 어긴 것인가? 왜 그런 답이 나오는지를 설명하시오.

39. 잎의 개수 mo] 29] 거듭제곱이 아닌 경우에 보조정리 7,99] 일반적인 경우를 증명하시오.

7.9절

40. 기수정렬 알고리즘(알고리즘 7.6)을 구현하여 실행해보고, 여러 개의 문제 사례를 가지고
최선, 평균, 최악 시간복잡도를 구하시오

41. 키가 모두 서로 다른 경우 기수정렬(알고리즘 7.6)의 최선 시간복잡도는 ㅇ0(2 187) 임을 증
명하시오.

42. 마스터 리스트를 재구성하는 과정에서 기수정렬 알고리즘(알고리즘 7.0)은 더미(기수:의 개
수가 클 때 빈 부분 리스트를 검사하느라 많은 시간을 낭비한다. 비어있지 않은 부분 리스트
만의 검사가 가능한가?

추가 연습문제

43. 7개 아이템의 리스트에서 가장 큰 아이템과 가장 작은 아이템을 찾아서 그 두 아이템과 처
음과 마지막 위치에 있는 아이템 교환하여 비올림차순으로 정렬하는 알고리즘을 작성하시
오. 그러면 이미 제 위치에 AIS 잡은 두 요소들을 제외할 수 있으므로 리스트의 크기는
둘 씩 줄고, 리스트의 남은 부분도 전체 리스트가 정렬될 때까지 이 과정을 되풀이한다. 작
성한 알고리즘을 분석하고, 그 AWS 차수 표기법으로 표시하시오.

44. 피봇 아이템을 선택하는 전략을 바꾸어서 퀵정렬 알고리즘을 구현하여 실행시커보고, 여러
개의 문제 사례를 가지고 최선, 평균, 최악 시간복잡도를 구하시오.

45. 삼진 (ternary heap) 가지고 정렬 알고리즘을 설계하는 방법을 연구해보시오. 삼진 힙
은 내부마디의 자식마디가 모두 3개라는 것 말고는 보통 힙과 같다.

46. 7개 아이템의 리스트에서 《*개의 가장 작은 아이템들을 찾되, 찾은 아이템들의 상대적인 순
서에는 관심이 없다고 가정하자. *가 상수일 때 1차시간 알고리즘이 있을까? 그리고 왜 그
런 답이 나오는지를 밝히시오.

47. 외부 메모리에 저장되어 있는 아주 큰 리스트를 정렬하고 싶다고 하자. 이 리스트를 내부
메모리에 저장하기는 너무 크다고 가정하면, 외부 정렬 알고리즘을 설계하는데 주로 고려해



===== PAGE 330 =====
@00@00000 0
chapter 7 계산복잡도의 소개: 정렬문제

318

48.

49.

50.

야 할 요소는 무엇인가?
이 장에서 설명한 정렬 알고리즘을 설계 아이디어를 기준으로 분류하시오. 예를 들어, 힙정
렬과 선택정렬의 설계 아이디어는 가장 큰 (또는 가장 작은) 아이템을 찾아서, 그 아이템과
마지막 (또는 처음) 아이템을 적절한 순서로 교환한다.

TY stable) 정렬 알고리즘은 동일한 아이템의 원래 SAS 보존하는 알고리즘을 말한다.
이 장에서 설명한 정렬 알고리즘 중 안정된 알고리즘은 무엇인가? 그리고 왜 그
는지를 밝히시오.

연습문제 SoA] 안정되지 않다고 확인된 알고리즘 중 안정된 정렬 알고리즘으로 쉽게 바꿀

수 있는 알고리즘은 무엇윈가?

rk o
mt fl
20;
fo



===== PAGE 331 =====
“흉길동"의 전화번호를 더
빨리 찾는 방법이 있을까?

Chapter 8

KLE,  22

계산복잡도 : 검색문제 OL

장의 시작부분에서 바니 비글은 개선된 이분검색법을 사용하여 “홍길동"의 전화

1    Hos 빨리 찾을 수 있었다. 바니는 이제 “홍길동"의 전화번호를 더 빨리 찾을
수 있는 방법이 있을지 궁금해 할 수 있다. 이 장에서는 더 빨리 찾는 방법이 있는지를
알아보기 위하여 검색문제(66870008 problem)S 분석한다.

정렬과 마찬가지로 검색은 컴퓨터과학에서 가장 유용하게 쓰이는 알고리즘
다. 검색문제는 키(567) 값을 가지고 전체 레코드를 찾아내는 것이다. 예를 들
는 개인의 신상정보가 될 수 있고, 키는 주민등록번호가 될 수 있다. 여기서 목
장과 비슷하다. 검색 문제를 분석하여 계산복잡도의 하한을 구하고, 시간복잡도가 그 하
한만큼 좋은 알고리즘이 있는지 증명하려는 것이다. 부가적으로 검색 알고리즘에서 사용
한 데이터구조를 공부하고, 응용 분야에 따라서 어떤 데이터구조를 사용하면 좋은지를
알아본다.

8.1절에서는 (앞 장의 정렬문제에서 그랬듯이) 비교만으로 배열에서 키를 검색하는 문
제의 하한을 구하고, 이분검색 알고리즘(알고리즘 1.5와 2.1)의 시간복잡도가 하한만큼
좋다는 걸 증명한다. 전화번호를 검색하면서 바니 비글은 사실 키를 비교하는 일 이외의



===== PAGE 332 =====
320

chapter 8 계산복잡도: 검색문제

다른 일도 하는 "보간검색"이라고 하는 개선된 이분검색법을 사용하였다. 즉, “홍길동"의
전화번호를 찾을 때 바니는 전화번호부의 중앙 부분에서 검색을 시작하지 않았다. 왜냐
하면 BU “so” 시작하는 이름들은 전화번호부의 뒷부분에 있다는 사실을 알고 있기
때문이다. 다시 말하면 그는 "보간"하여 책의 뒷부분에서 검색을 시작하였다. 8.2절에서
는 이 보간검색을 분석한다. 8.8절에서는 응용 분야에 따라서 배열이 검색 이외의 다른
용도로 쓰기에는 부적절한 데이터구조일 수도 USS 보여준다. 따라서 비록 이분검색
알고리즘이 4]A (optimal) o]7|= 하지만, 배열 구조에 의존하여 구현하기 때문에 경우에
따라서 알고리즘을 사용하지 못하는 경우가 생길 수 있다. 트리 구조를 쓰면 이 문제점을
해결할 수 USS 트리검색을 통하여 보여준다. 8.4절은 정렬되어 있지 않은 구조에서
데이터를 검색하는 경우에 쓰는 기술인 HAl(hashingyS 공부한다. 8.5절에서는 다른 A
색문제인 AEWA (selection problem) 대해서 알아본다. 선택문제는 개 키로 구성된
리스트에서 kA 작은(또는 《번째 큰) 키를 찾는 문제이다. 8.6절에서는 어떤 문제를
푸는 모든 알고리즘의 수행 성능에 대한 범위(604200)를 구하는 또 하나의 방법인 방해꾼
4-H (adversary arguments) 2 소개한다.

8.1 비교만으로 검색을 하는 경우의 하한

키를 검색하는 문제는 다음과 같이 AVS 수 있다. 7:개의 키로 구성된 배열 와 키 x7}
주어졌을 때, 가 배열의 키 중 하나와 같으면 x = Sli] 7+ 되는 첨자4ㅁ064) iS 찾아
주고, x7} 어떤 키와도 같지 않으면 검색이 실패했음을 보고한다.

이분검색(알고리즘 1.5와 2.1)은 배열이 정렬되어 있는 경우 이 문제를 푸는 매우 효율
적인 알고리즘이다. 이 알고리즘의 최악 시간복잡도는 |187^1+1이다. 이보다 더 실행
능력을 향상시킬 수 있을까? 비교만으로 검색하는 알고리즘으로만 국한시키면, 실행 능
을 그 이상으로 향상시키기가 불가능하다. 비교만으로 배열에서 검색키 cS 찾는 알고
즘들은 배열 내부키끼리 서로 비교하거나 검색키와 비교할 수 있고, 검색키를 복사할

있지만, 다른 연산은 할 수 없다. 그러나 검색을 돕기 위해서 (이분검색에서와 같이)

배열이 정렬되어 WSS 이용할 수 있다. 7장에서 공부한 대로 결정 알고리즘들에 대한
하한0004008)을 구할 것이다. 확률 알고리즘으로 따져도 마찬가지 결과가 나온다. 더구
나 THAIS 같이 배열의 키들은 모두 서로 다르다(480701고 가정한다.

결정 정렬 알고리즘에서 했던대로 결정트리를 키가 nN 배열에서 검색키 cS 찾는
결정 알고리즘과 연결시킨다. "개의 키를 검색하는 문제에서 그림 8.1은 이분검색에 해
당하는 결정트리이고, 그림 8.2는 순차검색(알윤리즘 1.1)에 해당하는 결정트리이다. 이
트리들을 보면 큰 마디는 각각 배열키와 검색키의 비교를 나타내고, 작은 마디(=잎)는
각각 찾은 결과를 나타낸다. 검색키 2가 배열에 있으면 그 인덱스를 내주고, 검색키 2가
배열에 없다면 검색 실패를 의미하는 "를 내준다. 그림 8.1과 8,204] 6, 부터 6;은 다

|

> 띠 wo

4



===== PAGE 333 =====
|는

=

그림 8.1 7개의 키를 검색하는 SS 이분검색에 상응하는

les

결정트리

결정트리


===== PAGE 334 =====
322

chapter 8 계산복잡도: 검색문제

검색 알고리즘은 배열의 값을 변경시키지 않으므로, 검색이 완료된 후에도 이 값은 변
하지 않아야 한다.

검색키 oS 찾기 위해서 7개의 키를 검색하는 결정트리의 잎은 각각 알고리즘이 멈추
고 = 8,가 되는 인덱스 1S 알려주거나 아니면 실패라고 알려준다. 각 내부마디는 비교
를 나타낸다. 가능한 모든 결과에 대해서 그 결과를 알려주는 뿌리마디에서 잎으로의 경

로가 있으면, 그 결정트리는 cS 찾기 위해서 7개의 키를 검색하기 유효하다(0810)라

<i<n@ 모든 8에 대해서 = 8,가 되는 경로들과 실패로 유도하는 경
로가 반드시 존재한다. 모든 잎이 도달가능(068018116)한   — 7}A\A tH pruned)
라고 한다. 7개의 키를 가진 배열에서 검색키 2를 찾는 알고리즘은 모두 그에 상응하는
유효한 가지친 결정트리가 존재한다. 일반적으로 검색 amage 검색키 x 2 배열키들
을 항상 비교할 필요는 없다. 즉, 두 개의 배열 내부키를 서로 비교할 수도 있다. 그러나
키가 모두 서로 다르다고 가정하기 때문에 검색키 2 와 비교할 때만 동일하다(60048419)는
결과가 나온다. 알고리즘이 검색키 가 배열에서 같은 키를 찾으면 이분검색과 순차검색
의 경우 알고리즘은 바로 멈추며 배열 아이템의 인덱스를 내준다. 어떤 비효율적인 알고
리즘은 검색키 2가 배열키와 같은지 결정한 후에도 비교를 계속하고 나중에 인덱스
BAS 수도 있다. 그러나 그런 알고리즘은 같은 키를 찾은 시점에서 바로 멈추고 인덱
를 GASES 고칠 수 있다. 새로 고친 알고리즘은 최소한 원래 것만큼은 빠를 것이
따라서 개의 서로 다른 키에서 검색키 cS 찾는 유효한 가지친 결정트리만 고려하면
되는데 동일한 키를 찾게 되면 인덱스를 넘겨주는 잎으로 가게 된다. 비교하여 얻을 수
있는 결과는 세 가지밖에 없으므로 결정적 알고리즘은 비교 후 기껏해야 세 가지 다른
경로를 택할 수 있다. 즉, 결정트리에서 비교마디는 각각 3개의 자식마디를 가질 수 있
다. 동일한 키를 찾으면 첨자를 넘겨주는 잎으로 가기 때문에 자식마디 중에서 최대 2개
는 비교마디가 될 수 있다. 그러므로 결정트리에서 비교마디만 따지면 이진트리가 된다.
예로서 그림 8.1과 8.29] 큰 마디의 집합을 보라.

0

1> qu

꾸

8.1.1 최악의 경우 하한

가지친 유효결정트리에서 모는 S   때 반드시 ES 가능해야 하기 때문에 그런 트리에서
행해지는 최악의 경우 비교 횟수는 비교마디로 이루어진 이진트리의 뿌리마디에서 잎까
지 가장 긴 경로 창에 있는 마디의 개수가 된다. 이 수는 이진트리의 깊이 더하기 1이다.
그러므로 최악의 경우 비교 횟수의 하한을 알아보기 위해서는 비교마디로 구성된 이진트
리의 깊이의 하한을 알아내기만 하면 된다. 이 하한은 다음 보조정리들과 정리를 통해서
알아본다.

| < 보조정리 8.1
이진트리 마디의 수를 7이라 하고, 깊이를 0라고 하면,



===== PAGE 335 =====
d= [1800)|
명 :
리마디에는 마디가 한 개, 깊이가 1이면 기껏해야 27H, 깊이가 이면 기껏해야 27H, ..…,
그리고 깊이가 0이면 2“개이므로, 다음과 같은 부등식을 얻을 수 있다.
n<14+24+2?+2?+---+24
부록 AS| 예제 ㅅ.8의 결과를 적용하면 다음과 같다.

20001

42 oly

| « EAI 8.2

7/개의 서로 다른 키 가운데서 cS 찾기 위한 가지친 유효이진트리가 되려면, 비교마디로 이루
어진 이진트리에 최소한 "개의 마디는 반드시 있어야 한다.
증명 :
개의 키 값을 $,(1 = 1 = 70)라고 하자. 먼저 sds 모두 최소한 한 개의 비교마디에는 속해
있다는 사실을 증명한다(즉, 비교하는데 최소 한 번은 사용해야 한다). 가령 임의의 cof 대해
서 그렇지 않다고 가정해보자. cA] 키만 빼고 키가 모두 같은 배열을 생각해보자. 그리고 oS
두 &, 값 중 하나라고 하자. 9% 비교하는데 전혀 사용되지 않았고, 다른 키는 키가 모두 같기
때문에 결정트리는 두 배열에 대해서 동일하게 동작해야 한다. 그러나 둘 중 하나의 배열에
대해서는 반드시 iS 내주어야 하고, 다른 하나의 배열에 대해서는 절대 』를 내주지 말아야
한다. 이는 모순이고, 따라서 6,는 모두 최소한 한 개의 비교마디에는 속해 있어야 한다.
ots 모두 최소한 한 개의 비교마디에는 속해 있어야 하기 때문에 비교마디의 개수가 개
미만이 될 수  =   유일한 길은 최소 어떤 한 키 5S a7} 아닌 다른 키하고만 비교가 이루어
a 6,는 절대로 *와 비교가 이루어지지 않는다. 가령 그런 키가 있다고 하자.
는 모두 같고, 6,7} 가장 작은 값을 갖는 두 개의 AS 생각해보자. 를 둘
중 한 배열의 ea 키와 같다고 하자. 5,7} 포함된 비교마디로부터의 경로는 두 개의 배열에
같은 방향으로 가야 하고, 두 배열에서 다른 키는 모두 같다. 그러므로 결정트리는
두 배열 모두 똑같이 동작해야 한다, 그러나 하나는 《라는 담을 주어야 하고, 다른 하나는 Heh
지 말아야 한다. 이는 모순이다. 증명이 완료되었다.



===== PAGE 336 =====
324

chapter 8 계산복잡도: 검색문제

ㆍ 정리 8.1
개의 서로 다른 키를 가진 배열에서 비교만으로 *를 찾는 결정 알고리즘은 최악의 경우 최소

한 키를

11941 +1번
비교해야 한다.

[우 08
KI    of

리즘에 따르면 개의 서로 다른 키 가운데서 cS 찾기 위한 가지친 유효결정트리가 존재
한다. 최악의 경우 비교 횟수는 결정트리의 비교마디만으로 된 이진트리에서 뿌리마디에서 잎
까지의 가장 긴 경로상의 마디 개수이다. 이 수는 이진트리의 깊이 더하기 1이다. 보조정리
8.2에 의하면 이 이진트리는 최소한 7개의 마디를 가지고 있다. 그러므로 보조정리 8.1에 의하
여 이진트리의 깊이는 |187.|보다 크거나 같다. 증명이 완료되었다.

에

2.1절에서 보았듯이 이분검색에서 최악의 경우 비교 횟수는 [Ig nj 1이다. 따라서
최악의 경우를 따질 때 이분검색은 최적이다.

8.1.2 평균의 경우 하한
평균의 경우 하한에 대해서 공부하기 전에 이분검색의 평균인 경우를 분석해보자. 이 분
석은 지금까지 미루어 왔는데, 그 이유는 결정트리를 사용하면 이 분석이 용이해지기 때
문이다. 먼저 정의와 보조정리가 필요하다.
깊이 0-1까지 SASH 찬) 이진트리를 거의 완전한 O]41 Eze] (nearly complete 01-
nary 1768)라고 한다. 그림 8.8에서 볼 수 있듯이 본질적으로 완전한 이진트리는 모두 거
의 완전하지만, 거의 완전한 이진트리라고 해서 모두 본질적으로 완전하지는 않다(완전
한 이진트리와 본질적으로 완전한 이진트리의 정의에 대해서는 7.6절을 참조하시오).
보조정리 8,29} 비슷하게 다음 보조정리는 당연한 것 같지만, 엄밀하게 증명하기는 쉽
지 않다.

그림 8.3 (8) 본질적으로 완전한 이진트리. (6) 거의 완전하지만 본질적으로는 완전하지 않은 이진
트리



===== PAGE 337 =====
| <보조정리 8.3

이분검색을 위한 가지친 유효결정트리에서 비교마더로 이루어진 트리는 거의 완전한 이진트
리이다.
증명 : 키의 개수 에 대한 귀납법으로 증명한다. 비교마디로 이루어진 트리는 각 키마다 한
개의 마디씩 총 /;개의 마디로 이루어진 이진트리이다. 따라서 이 이진트리에서 마디의 개수에
대한 귀납법을 적용할 수 있다.
귀납기초 : 한 개의 마디로 이루어진 이진트리는 거의 완전하다.
귀납가정 : *<7을 만족하는 모든 《에 대해서 *개의 마디로 이루어진 이진트리는 거의 완전
하다.
귀납단계 : 7:개의 마디로 이루어진 이진트리는 거의 완전하다는 사실을 증명하면 된다. 여기
서 7값이 홀수인 경우와 짝수인 경우를 따로 증명한다.

no] 홀수인 경우 이분검색의 첫째 분할에서 배열을 크기가 (n—1)/29) 부분배열로 각각
쪼개진다. 그러므로 왼쪽과 오른쪽 하위트리는 모두 (n—1)/27 키를 이분검색하기 위한 이
진트리이다. 이는 구조적으로 둘 다 같은 트리라는 뜻이다. 이 하위트리들은 귀납가정에 의하
면 둘 다 거의 완전하다. 둘 다 같은 거의 완전한 트리이므로, 이 트리들을 왼쪽과 오른쪽 하위
트리로 각각 가진 트리는 거의 완전하다.

no] 짝수인 경우 이분검색의 첫째 분할에서 오른쪽에는 HAS 크기가 7/3인 부분배열로
왼쪽에는 배열의 크기가 (2/2)ㅡ1인 부분배열로 각각 쪼개진다. 상세한 ABS 위해서 왼쪽
에 홀수 개 키가 있는 경우를 설명한다. 오른쪽에 홀수 개 키가 있는 경우도 증명 절차는 비슷
하다. AHO] 홀수인 경우 AS 하위트리의 왼쪽과 오른쪽 하위트리는 (앞에서 설명한 대로)
같은 트리이다. 오른쪽 하위트리의 한 하위트리는 또한 같은 트리이다(이를 증명해보시오).

\. YL (6

4     B

Cc
그림 8.4 n=20l 경우, 이분검색을 위한 결정트리에서 비교마디로 구성된 이진트리. 마디에는
키의 값만 나타나 있다. 하위트리 AB, Ce 구조가 모두 같다.

x
~



===== PAGE 338 =====
@®eeeee? ®@
326          chapter 8 계산복잡도: 검색문제

오른쪽 하위트리는 (귀납가정에 의해서) 거의 완전하고, 그 하위트리의 하위트리 중 하나는
왼쪽 하위트리의 왼쪽과 오른쪽 하위트리와 같은 트리이기 때문에 전체 트리도 반드시 거의
완전해야 한다. 그림 8.4의 그림을 보시오.

이제 이분검색의 평균의 경우 분석을 해보자.

: 와 S[mid] 의 비교

: 배열에서 아이템의 개수, 7

먼저 #가 배열에 있는지 아는 경우를 분석해보자. 이 BAS 할 때 2가 배열의 각 슬롯에
위치할 확률이 똑같다고 가정한다. 뿌리마디에서 어떤 마디까지의 경로 상에 있는 마디의
총 개수를 그 마디까지의 마디거리(ㅁ0006 018682006)라 부르고, 모든 ai 대한 마디거리
의 합을 총 마디거리(10181 Node Distance: TND)#}31 부른다. 마디거        뿌리에서 그 마
디까지 경로의 길이보다 하나 더 크다. 그림 8.1과 같이 비교마디로 이루어진 이진트리는
27770=1+9+2+3+-83+~83+3= 17

전체 배열슬롯에서 를 찾는 이분검색 결정트리에서 비교하는 총 횟수는 그 결정트리에서
비교마디로 구성된 이진트리의 77/22와 같다. 따라서 배열의 모든 슬롯에 위치할 확률이
똑같다고 가정하면, cS 찾는데 필요한 평균 비교 횟수는 TND/no] 된다. 설명을 간단히
하기 위해서 어떤 정수 kell 대하여 n = 2" — 1이라고 일단 가정하자. 보조정리 8.3에서
본 대로 이분검색을 위한 결정트리에서 비교마디로 이루어진 이진트리는 거의 완전하다.
거의 완전한 이진트리가 2'— 1개의 마디로 이루어져 있다면, 그 트리는 완전한 이진트리

는 건 어렵지 않게 알 수 있다. 그림 8.1에서 비교마디로 이루어진 이진트리는 k= 3인
경우를 보여준다. 완전한 이진트리에서 TNDE 다음과 같이 계산한다.

TND =1+2(2)+3(27)+ … +&(2*~*)

=(k- 1)2**1 49] =(k-1)2*+1

끝에서 둘째 등식은 부록 AS} 예제 ㅅ.5의 결과를 적용하여 구한다. 2° = + 1이기 때문
에 평균 비교 횟수는 다음과 같이 계산한다.
TND _  (k-1)(n+1)4+1

A(n)=                k-1=Lgn]
n            n
모든 no] 대해서 평균 비교 횟수는 대략 다음과 같은 범위를 가진다.
lign|—1< A(n) < Lg nJ

이 2°) 거듭제곱(60\60)이거나 29] 거듭제곱보다 약간 크면 평균은 하한에 가깝고, no]



===== PAGE 339 =====
@9eeeee 0
8.1 비교만으로 검색을 하는 경우의 하한     327

2의 거듭제곱보다 약간 작으면 평균은 상한에 가깝다. 어떻게 이러한 결과를 얻게 되는지
는 연습문제로 남겨둔다. 직관적으로 왜 그런지 이해하려면 그림 8.1을 보면 된다. 마디의
총 개수가 8이 되도록 한 개의 마디를 추가시키면 [18 」|는 2에서 3으로 뛰지만, 평균 비
교 횟수는 거의 변하지 않는다.
chaos 2가 Mitel 없는 22-8 Baie}, 27 1가지가능시 있다. 27h 모든
아이템보다 작을 수도 있고, 어떤 두 개의 아이템 사이에 있을 수도 있고, 모든 아이템 보
클 수도 있다. 즉, 다음과 같이 나누어 생각해 볼 수 있다.
1<i< nl io] 대해서 ㅎ= 8,
LSS;
1S%=n—1el 어떤 19] 대해서 <,

~

°

| 경우가 일어날 확률이 모두 같다고 가정하고 분석해본다. ABS 간
어떤 정수 kell 대하여 = 2*ㅡ1이라고 일단 가정하자. 성공적인 검색의 총 비교 횟수는
비교마디로 이루어진 이진트리의 77/2/이다. 이 수가 (k—-1)2* +13} 같음을 상기해보
자. n+ 1번의 실패한 검색을 하는데 《번의 비교를 한다(그림 8.1

비교 횟수는 다음과 같이 계산한다.

TND+k(n+1)_ (k—-1)2*+1+k(n+1)
2n+1           2n+1

a
nee,
off,
™
r

‘Oh
에
에
에
ae,
oh
ay

A(n)=

2" = + 1이므로, 다음과 같다.
_ (k-1)(n+1)+1+k(n+1)
avn)        In+1

_ 2k(n+1)+1—(n+1)
2n4+1

~k- $= [len|+1-$=UgnJ+>
BE no] 대해서 평균 비교 횟수는 대략 다음과 같은 범위를 가진다.

lignJ->< A(n   stent

nO] 의 거듭제곱이거나 의 거듭제곱보다 약간 크면 평균은 하한에 가깝고, no] 29] 7
SAB 약간 작으면 BRE 상한에 가깝다. 어떻게 이러한 결과를 얻게 되는지는 연습
문제로 남겨둔다.

이분검색

그런지는 그

oe   ze

평균의 경우 성능이 최악의 경우에 비해서 아주 많이 좋은 것은 아니다. 왜
8.1을 보면 알수 있다. 그림 8.1을 보면 트리의 바닥(최악의 경우가 일어


===== PAGE 340 =====
328

chapter 8 계산복잡도 : 검색문제

는 부분)에 있는 결과마디(잎)의 개수가 나머지 부분에 있는 결과마디(잎)의 수보다 많
음을 알수 있다. 실패한 PAS 뻐버리더라도 이는 사실이다(실패한 AAS 모두 트리의
바닥에 위치하고 있음을 주목하라).

다음은 위의 분석에서 설정한 가정 하에서 이분검색은 평균의 경우 최적임을 증명해보
자. 먼저 min TND(n)& nF] 마디로 이루어진 이진트리에서 77022의 최소치라고 정
의하자.

| *보조정리 8.4

"개의 마디로 이루어진 이진트리의 TNDES minTND(n) 2} 같다"는 "그 트리는 거의 완전하
다"의 필요충분조건이다.

eee :
(필요조건증명) 먼저 “트리의 TND=minTND(n)"| 4 "그 트리는 거의 완전하다"임을 증명
하자. 어떤 이진트리는 거의 ope 않다고 가정하자. 그러면 트리 맨 바닥의 두 ~

N
“
N
ont
EN,
10 으

수준)이 아닌 마디들 중에 자식마디가 하나인 마디가 반드시 존재할 것이다.
그러면 바닥 수준에 있는 임의의 oe AS 떼어서 그 마더의 자식미디로 만들 수 있다. 이
수정된 트리는 변함없이 7개의 마디로 이루어진 이진트리일 것이다. 그 수정된 트리에서 Az
로 상 마더의 개수는 원래 트리에서 AZ 가는 경로 상 마더의 개수보다 최소한 1이
것이다. 다른 모든 마더로 가는 경로 상 마더의 개수는 동일할 것이다. 그러므로 원래
트리보다 TND7} 작은 /:개의 마디로 이루어진 이진트리를 만들어냈다. 이는 원래트리의
TND= 최소치가              하게 된다.
(충분조건증명) 7개의 마더로 이루어진 거의 완전한 이진트리는 모누 2222가 같다는 사
AS 알아내기는 별로 어렵지 않다. 따라서 그러한 트리는 모두 7707/가 최소가 되는 것이
틀림없다.

ms
ito

*보조정리 8.5
개 키를 검색하고, 검색하려는 키 2가 배열에 있고, 배열 슬롯에 있을 확률은 모두 같다고
가정하자. 그러면 이분검색의 평균의 경우 시간복잡도는 다음과 같다.

min TND(n)

n

의 경우 분석에서 공부했듯이 평균 시간복잡도는 결정트리에서 비교마디로 이
리의 TNDS 7으로 나누어서 구한다. BABE] 8.3과 8.4의 결과로 증명한다.



===== PAGE 341 =====
8.1 비교만으로 검색을 하는 경우의 하한     329

| 보조정리 8.6
a7} 배열에 있고, 배열 슬롯에 있을 확률이 모두 같다고 가정하면, 개의 서로 다른 키로 된
배열에서 cS 검색하는 결정 알고리즘 평균의 경우 시간복잡도의 하한은 다음과 같다.
min TND(n)
증명 :
보조정리 8.204] 보았듯이 검색 알고리즘의 결정트리에서 각 배열 키 6,는 모두 최소한 한
번은 *와 반드시 비교해야 한다. oS &,와 oS 비교하는 마디로 가는 최단경로 상 마디의
개수라고 하자. 각 키가 7가 될 확률은 1/7로 모두 같기 때문에 평균 시간복잡도의 하한은
다음과 같이 계산한다.
위의 등식에서 우변의 분자가 min TND(n) We} 크거나 같은지를 SPE 일은 연습문제로
남겨 놓았다.

+… +

> Bel 8.2

개의 서로 다른 키로 이루어진 배열에서 비교만으로 oS 검색하는 결정 알고리즘 중에서

27} 배열에 있고 배열 슬롯에 있을 확률이 모두 같다고 가정하면, wale 평균의 경우

성능이 최적이다. 따라서 이 가정 하에서 그러한 알고리즘은 모두 평균적으로 키의 최소한 비
교 횟수가 대략 다음과 같다.

[18701 -1

|

며 :

조정리 8.5, 8.6과 이분검색의 평균 시간복잡도 분석 결과로 증명한다.

ㅇ

27. + 1가지의 가능한 결과(이분검색의 평균의 경우 분석에서 공부 한 대로)가 나올 확
BO] 모두 같다그 가징하고, 이분검색이 평균의 경우에 성등의 azo   는 사실을 종명
하는 것도 가능하다.

확률분포에 관한 하나의 구체적인 가정이 주어진 상태에서 이분검색은 평균의 경우
성능이 최적이라는 사실을 입증하였다. 다른 확률분포에 대해서는 아마도 최적이 아닐

도 있다. AS 들어, 가 Sl] 3 같을 확률이 0.9999라면, 를 S[1] zp 먼저 비교하는
게 최적일 것이다. 그러나 이 예는 조금 부자연스럽다. 대한민국 사람들 중에서 무작위로
이름을 뽑아서 검색을 하는 예는 더 실질적이라고 볼 수 있다. 8.5절에서 설명했듯이 “A
재수"와 “서문 강선"이 나올 확률이 같으리라고 아무도 생각하지 않을 것이다. 따라서 방


===== PAGE 342 =====
330    chapter 8 계산복잡도 : 검색문제
금 공부힌 atid aoe 수는 없고, 다른 고려사항이 추가로 필요하다. 3.5절에서 이
에 관한 고려사항들을 언급한다.

@ 82 보간검색
앞 절에서 구한 하한은 비교에만 의존하는 알고리즘의 경우에 한한다. AAS 도울 수

있는 어떤 다른 정보가 있는 경우에 이 하한을 향상시킬 ihe  있다. 바니 se ee
부에서 “홍길동"의 전화번호를 찾기 위해서 키를 비교ㅎ
기억해보자. 그는 전화번호부의 정중앙에서 검색을 시작하지 않았다. 왜냐하면 “ㅎ"이
거의 뒷부분에 있다는 ~ aa 있기 때문이다. 그는 oie ean  검색
을 거의 뒤에서 시작했다. 2         보간하는 AS 사용하여 검색 알고리즘을 개발해
보자:

10개의 정수를 검색하는데, 첫째 정수는 범위가 0에서 9사이이고, BALE 10에서 19사
이이고 셋째는 20에서 29사이이고, .…, SAE 90에서 99사이라는 A 안다고 가정하자.
그러면 검색키 2 가 0보다 작거나 99보다 큰 경우에는 바로 검색실패를 알려주고, 이 두
가지 경우가 아니면 와 [1+ | ㅎ/10]|]만 비교하면 된다. 예를 들어, 2 = 25는 Slt
[25/101] = s{3] 2} 비교하면 된다. 만약 같지 않다면, 검색실패를 알려주면 된다.

보통 이렇게 많은 정보를 알지는 못한다. 그러나 경우에 따라서 키가 첫째 아이템과
마지막 아이템 사이에 거의 균등하게 분포되어 있다고 가정해도 별 문제가 없다. 이러한
경우 2가 중간에 있는 키와 같은지를 점검하는 대신, cS 찾을 수 있을 만한 Bo] 있
는 키와 같은지를 점검할 수 있다. AS 들면, 10개 키가 0부터 99까지 거의 균등하게
BEE} 있다고 가정하면, <= 25는 셋째자리에 있으리라 le  615] 대신에

S[3) 3} cS 먼저 비교한다. 이와 같은 전략으로 검색하는 알고리즘을 보간검색0066ㄷ-
polation 868700)이라고 한다. 이분검색과 마찬가지로 처음에 fess 12 놓고 highE n
으로 놓는다. 그리고 선형보간법을 사용하여 07} 어디에 위치할지를 대략적으로 결정한
다. 즉 다음과 같이 계산한다.

x - S{low]
S|high] — Slow

mid = low+| X (high tow) |

예를 들면, 11] = 4 이고 110] = 97이고, 7 = 255 찾는다면 다음과 같이 계산한다.

25—4
97-4

mid= 1+     (10-1) |=1+1 2.032]=3

mid 계산하는 방법이 다르다는 것과 추가 자료기록이 필요하다는 걸 제외하고 다음
의 보간검색 알고리즘은 이분검색(알고리즘 1.5)과 비슷하다.



===== PAGE 343 =====
@‥ㅎ00000 0
8.2 보간검색  331

ㆍ일29즘 81 보간검색

문제 : 2가 크기가 인 정렬된 배열에 있는지를 결정하시오.
입력 : 양의 정수 /과 인덱스가 1부터 7까지인(비내림차순으로) 정렬된 수의 배열 ㅇ
출력 : SHAS] 가 있는 위치 1; 만약 2가 So] 없으면 0

void interpsrch (int n,
const number S|],
number x, index& 2)

index low, high, mid;
number denominator ;

700 = 1; Ligh = n3 7= 0;
if (Slow] < x < S{high))
while (low <= high && i == O){
denominator = S{high\— S{low} ;
if (denominator == 0)
mid = low;
else
mid = low + |((x— S{low]) * (high- low)) / denominator |:
if (x == S{mid))
1 =) mid:
else if (x < S[{mid\)
high = mid-1;
else
low = mid+ 1;

키가 거의 균등하게 퍼져 있으면, 보간검색이 이분검색보다 더 빨리 2 의 위치를 찾아
낸다. 가령, 앞의 예에서 = 257} .913]보다 작으면, 보간검색은 크기가 10인 입력을 a
기가 2인 입력으로 줄인다. 반면 이분검색은 크기가 4인 입력으로 줄인다.

키가 11]과 .917/] 사이에 골고루 분포되어 있다고 가정하자. 무작위로 선택한 키가
특정 범위에 속할 확률은 같은 길이의 다른 범위에 속할 확률과 같다는 A 뜻한다. 이게
사실이라면 보간검색에 의해서 결정된 슬롯 부근에서 2 찾기를 기대할 것이므로 보간검
Ao] 평균적으로 이분검색보다 월등하게 우수하다고 기대할 수 있다. 실제로 키가 균일
하게 분포되어 있고, 가 각 배열 슬롯에 해당하게 될 확률이 모두 같다고 가정하면 보간
검색의 시간복잡도가 다음과 같음을 증명할 수 있다.

A(n) = 18087)

만약 이 10억이라면, lg 7은 OF 300] 되는 반면, 1808 70)은 OF 57} 된다.


===== PAGE 344 =====
332

chapter 8 계산복잡도 : 검색문제

보간검색의 단점은 최악의 경우 성능이다. 10개 키가 있고, 그 Ff] 1, 2 3, 4, 5, 6,
7, 8, 9, 100이라고 가정해보자. 만약 2 가 10이라면 mide 계속해서 Jow7} 되며, 결과적
으로 는 모든 키와 비교할 수밖에 없게 된다. 최악의 경우 보간검색은 순차검색이 되어
버린다. 2470가 계속해서 low7} 되는 경우가 최악임을 주목하라. 보간검색의 변종인 보
강된 보간검색(70[648【 interpolation 808101)은 772727-/0ㅠ와 high-mid7} 항상 ㅎ22'보다는
크도록 변수 gap& 정하여 이 PIS 보완한다. gap] 초기값은 다음과 같이 놓고,

gap = | (high — low + 1)"? |

선형보간법에서 사용한 공식을 가지고 midS 계산한다. 계산 후, mid2] 같은 다음과 같
이 다시 계산한다.

mid = minimum (high ㅡ gap, maximum(mid, low+ gap))

+1)? |=3이고, mid 초기에 1°] 되어서 다음과 같이 계산한다.
mid = minimum(10—3, mazimum(1, 1+ 3)) = 4

이렇게 함으로써 비교하는데 사용하는 인덱스는 /0와 ^44로부터 최소한 642만큼 떨어
지는 게 보장된다. 에 대한 AAS 두 개 중 큰 부분배열에서 계속할 때마다 gaps] 값
은 배로 증가하지만 그 부분배열 크기의 반은 절대로 넘지 않는다. 앞의 예에서 <에 대한
AALS. 더 큰 부분배열에서 계속된다(5[5]에서 5110]까지의 부분배열). 그러므로 gaps
배로 증가시킬 텐데, 이 경우 부분배열은 배열의 크기가 6이고, gaps 두 배로 만들면
부분배열의 크기의 반을 초과하게 되므로 예외로 취급한다. gapS 두 배로 늘이는 이유
는 큰 덩어리로부터 빨리 빠져나가기 위함이다. <가 작은 부분배열에서 계속된다면 gap
은 초기값으로 다시 고쳐 놓는다.

키가 균일하게 분포되어 있고, 검색키 2가 각 배열 슬롯에 있을 확률이 모두 같다고
가정하면 보강된 보간검색의 평균 시간복잡도는 ㅇ08087))이다. 최악 시간복잡도는
@(087)?'인데, 이는 이진검색보다는 좋지 않지만 보간검색보다는 좋다.

보간검색에 비해서 보강된 보간검색이 계산량이 많아지고, 이분검색에 비해서 보간검
Ajo] 계산량이 많아진다. 따라서 비교 횟수의 감소가 계산량의 증가를 정당화하는지는
분석해 보아야 한다.

여기서 설명한 검색은 단어검색에도 적용할 수 있다. 왜냐하면 단어는 바로 수로 기호
화(000009)할 수 있기 때문이다. 그러므로 수정된 이분검색 방법을 전화번호부 검색에
사용할 수 있다.



===== PAGE 345 =====
@‥ㅎ00000 0
8.3 트리에서의 검색    333

@ 83 트리에서의 검색

비록 이분검색과 그 변종들인 보간검색과 보강된 보간검색이 매우 효율적이기는 하지만
응용할 수 없는 경우가 많이 있다. 왜냐하면 많은 양의 데이터를 적당한 구조가 아니기
때문이다. 실제로 많은 양의 데이터를 담는 적절한 데이터구조는 트리이다. 이 장에서는
EUs 검색하는 Ollgn) 알고리즘이 있다는 ABS 공부해보자.

AA AA (static 8687027709)은 레코드를 모두 파일에 한꺼번에 저장하고, 추후에 레코
드를 추가하거나 삭제할 필요가 없는 경우 주로 하는 검색이다. 정적검색이 적절한 경우
의 예로 운영체제(60608108 systems) BYE 검색을 들 수 있다. 그러나 레코드가 추가
삭제되는 빈도수가 높아서 동적검색(0708040 searching)o] 필요한 사례도 많이 있다. 비
행예약시스템은 동적검색이 요구되는 대표적인 경우이다. 왜냐하면 손님은 수시로 예약
을 하고, 또한 취소하기 때문이다.

배열구조는 동적검색에 적합하지 못하다. 왜냐하면 정렬된 배열에 레코드를 순서대로
추가시키는 경우 추가되는 레코드 다음에 오는 모든 레코드는 한자리씩 옮겨야 한다. 이
분검색을 효과적으로 하기 위해서 가운데 아이템을 효율적으로 찾을 수 있어야 한다. 즉,
이분검색은 동적검색에는 사용될 수 없다. 연결 FASS 사용하면 레코드를 자유자재로
추가 삭제할 수 있긴 하지만 연결 리스트를 효율적으로 검색하기는 불가능하다. 따라서
연결 리스트로 동적검색을 효율적으로 하기 충분치 않다. 정렬된 수열에서 키를 빨리 찾
아낼 필요가 있다면 직접접근 저장장소(4760 access storage, 해시구조)는 적용할 수 없
다(해시는 다음 절에서 공부한다). 동적검색은 트리구조를 사용하면 효율적으로 구현할
수 있다. 먼저 이진검색트리를 설명하고, 그 후에 이진검색트리의 개량인 8-트리를 설명
한다. 8-트리는 트리의 균형유지가 항상 보장된다. 우리의 SRE 검색문제를 더 깊이
있게 분석해 보는 것이다. 그러므로 이진검색트리와 8-트리와 관련된 알고리즘만 간단
히 살펴본다. 세부 알고리즘은 일반적으로 <ㅠ086(01994) 등의 데이터구조 책에 자세히 설
명되어 있다.

8.3.1 이진검색트리

이진검색트리는 3.5절에서 소개하였다. 그러나 거기서는 정적검색에서 어떻게 사용하는
지 설명하였다. 즉, 키를 검색하는 확률에 기초하여 최적의 트리를 구축하고 싶었다. =
FS 구축하는 알고리즘(알고리즘 3.9)에서는 키를 한 Ho] 모두 추가하도록 요구하였다.
이는 정적검색에 응용한다는 의미이다. 이진검색트리는 동적검색에 유용하다. 이진검색
트리를 이용하면 키를 빨리 추가 삭제할 수 있을 뿐 아니라 평균검색시간을 낮게 유지할
수도 있다. 더구나 트리를 부모중간횡단(1ㅁ-006『 traversal) 순으로 검색하여 키를 정렬
된 순서로 빨리 추출할 수 있다. 이진트리를 부모중간횡단 순으로 검색하면 먼저 왼쪽
부분트리의 마디를 모두 부모중간횡단 순으로 검색한 후 뿌리마디를 검색하고, 오른쪽



===== PAGE 346 =====
334

chapter 8 계산복잡도: 검색문제

부분트리의 마디를 모두 부모중간횡단 순으로 검색한다.

그림 8.5는 처음 7개의 정수로 이루어진 이진검색트리이다. 검색 알고리즘(알고리즘
3.8) 검색키 cS 뿌리마디의 값과 비교하여 트리를 검색한다. 만약 같으면 검색종료, 7
가 더 작으면 같은 검색전략을 왼쪽 자식마디로 적용한다. 가 더 크면 같은 검색전략을
오른쪽 자식마디로 적용한다. 이런 식으로 트리를 Sol 내려가서 cS 찾든지, 아니면 2
가 트리에 없음이 확실할 때까지 같은 과정을 되풀이한다. 그림 8.5에 있는 트리에 알고
리즘을 적용하면 이분검색을 위한 결정트리(그림 8.1)와 같은 순서로 비교를 수행한다는
사실을 이미 SormMSz|= 모르겠다. 이것이 이분검색과 이진검색트리의 근본적인 관계
를 잘 보여주고 있다. 즉, 7개 키를 검색하는 이분검색을 나타내는 결정트리에서 비교마
디는 또한 이진트리를 이루게 되고, 알고리즘 3.8의 비교 횟수는 이분검색에서와 같다.
그러므로 알고리즘 8.8은 이진검색트리에 적용하면 이분검색과 마찬가지로 개 키 검색
에 최적이다.

그림 8.5의 트리에서는 키를 효율적으로 추가하고 삭제할 수 있다. 예를 들면, 키 5.5
를 추가하기 위해서는 5를 가지고 있는 마디를 찾을 때까지 트리를 So] 내려가면 되는데
5,57} 마디에 있는 키보다 크면 오른쪽으로 내려가고, 그렇지 않으면 왼쪽으로 내려간다.
그리고 5.5를 그 잎의 자식마디로 만들어 준다. 앞에서 언급했듯이 실제 추가 및 삭제
알고리즘은 <ㅠ74860994) 등의 데이터구조 AS 참고하기 바란다.

이진검색트리의 단점은 키를 동적으로 추가하고 삭제할 때 결과 트리가 항상 HSS
유지한다는 보장이 없다는 것이다. 키를 증가하는 순서로 추가한다면 그림 8.6과 같은
Eqs 얻게 될 것이다. 이 트리를 w]Go}]4Z] 트리(66060 \ㅁ68)라고 하는데, 단순히 A
리스트와 다를 바가 없다. 알고리즘 3.8을 이 트리에 적용하면 순차검색을 하는 경우
마찬가지가 된다. 이 경우 연결 리스트 대신 이진검색트리를 사용함으로써 얻은 게 하나
도 없다.

만약 키를 무작위로 추가한다면 직관적으로 보았을 때 구축한 연결 리스트보다는 균형
잡힌 트리068180060 \66/에 더 가까울 것이다(무작위에 관한 자세한 사항은 부록 ㅅ의
A8 IAS 참조하라). 따라서 평균적으로 효율적인 검색시간을 기대해 볼 수 있다. 실제
로 그러한 취지로 만들어진 정리가 있다. 그 정리의 결과부터 먼저 설명해보자. 이 정리
에서 입력들은 모두 발생확률이 같다고 가정하고 개 키를 가진 입력을 검색하는 평균시



===== PAGE 347 =====
@0000000
8.3 트리에서의 검색    335

그림 8.6 AS 7개 정수를 포함하는 wSOlS! 이진검색트리

간을 구한다. 이는 *개 키에 순서매기는 가능한 모든 방법은
입력하는 것과 동일한 BSS 가진다는 의미이다. 예를 들면, 만약 7 = 3이
< 552] 3개 키가 있다면, 다음에 나열한 입력들은 모두 발생확률이 같다.

[sie eg] = [is Gap 951 0 Ls 9. 6

190. 83, 91]   [991 Si) 96]   199 89, 81]

2개의 다른 입력으로 같은 트리가 될 수도 있다. AS 들면, [5,, 58, 51] FA [52, 51, 53]
을 가지고 트리를 만들어 보면 같은 트리가 된다. 즉, 뿌리는 s,, 왼쪽에는 6,, 오른쪽에
는 83°] 되는 트리가 된다. 이 트리를 만드는 입력은 이 두 입력밖에 없다. 때로는 트리를
만드는 입력이 하나뿐인 경우도 있다. 예로서, [61, 58, 6891을 가지고 만든 트리는 다른
입력으로는 만들 수 없다. 여기서 강조하고 넘어가야 할 중요한 사실은 발생확률이 같다
고 가정하는 AS 트리가 아니라 입력이라는 것이다. 그러므로 위에 나열된 각 입력의
발생확률은 1/6이고, 입력 [56 83, 911과 [98, 91, 54]에 의해서 만들어진 트리의 발생확
률은 1/3이고, 입력 [s,, 92, 83] 0] 의해서 만들어진 트리의 발생확률은 1/6이다. 그리고
검색 키 가 nh 키 가운데 하나가 될 확률이 모두 같다고 또한 가정한다. 이제 정리를
정식으로 살펴보자.

입력들은 모두 발생확률이 같다고 가정하고, 검색 키 가 7개 키 가운데 하나가 될 확률이
모두 같다고 가정하면, "개의 다른 키로 이루어진 모든 입력의 평균검색시간은 이진검색트리
를 사용하면 대략 다음과 같다.


===== PAGE 348 =====
336

chapter 8 계산복잡도: 검색문제

A(n) = 1.38lgn

증명 :
검색 키가 트리에 있다고 가정하고 증명한다. 뒤에 연습문제에서 이 제한을 없애도 22+1가
지 결과(046002ㅁ8)가 발생확률이 모두 같은 한, 동일한 결론에 도달하게 됨을 증명할 것이다(어
떤 종류의 결과가 있는지는 8.1.2절의 이분검색의 Bato] 경우 분석에서 다룬 바 있다).

키가 개인 이진검색트리에서 KAAS 작은 키가 뿌리에 있는 경우를 생각해보자. 이런 이
진검색트리들을 보면, 왼쪽 부분트리의 마디 개수는 *-1개이고, 오른쪽 부분트리의 마디 개
수는 7-*개이다. 이런 트리를 만드는 입력에 대한 평균검색시간은 다음 세 가지 항의 합이
된다.

© 왼쪽 하위트리에서 평균검색시간 곱하기 가 왼쪽 하위트리에 있을 확률

0 오른쪽 하위트리에서 평균검색시간 곱하기 c7} 오른쪽 하위트리에 있을 확률

© 뿌리에서의 비교 1회
왼쪽 하위트리에서 평균검색시간은 4(《&-1)이고, 오른쪽 하위트리에서 평균검색시간은
A(n—k) O|t}, 검색 키 가 7개 키 가운데 어떤 것이 될 확률이 모두 같다고 가정했기 때문에
가 왼쪽과 오른쪽 하위트리에 있을 확률은 각각 다음과 같다.

일한

4(7040)뿌리에 KAS 작은 키가 있는 이진검색트리를 만드는 크기 no] 모든 입력에 대한
평균검색시간이라고 하면, 다음 식을 얻을 수 있다.

을         n—k

A(nlk) = A(k-1)=—*+ A(n=h)   nh   +1

모든 입력의 발생확률이 같으므로, 모든 키는 입력의 첫째 키가 되어서 뿌리에 위치하게
될 확률이 같다. 그러므로 크기가 /인 BE 입력에 대한 평균검색시간은 1부터 7까지의 모든
*에 대한 A(nlk) 2] 평균이다. 그러면 다음 식을 얻는다.

Anes: [그 40-0+ BoE Amb) +1]

p=

O(n) =nA(n) 28 놓고, A(n)-& Cln)/n2Z 대치하면 다음과 같다.

0200) _1|론-1 Clk-1) , 4-ㅅ^ C(n—k)
sp         '

yk
n        faa 빠    kal      n    mk     |

이 식을 정리하면 다음과 같다.



===== PAGE 349 =====
@0000000
83 트리에서의 검색    337

초기조건은 다음과 같다.

이 재현 방정식은 퀵정렬(알고리즘 2,6) BH] 경우와 거의 똑같다. 퀵정렬 평균의 경우 분석
결과를 그대로 이용하면 다음과 같은 결과를 얻는다.

C(n) = 1.38(n+1)lgn

ils

A(n) = 1.38lgn

정리 8.2014] 얻은 결과를 잘못 해석하지 않도록 주의해야 한다. 7개 키로 이루어진
어떤 특정 입력의 평균검색시간이 약 1.38187이 된다는 뜻은 아니다. 어떤 특정 입력에
대해서는 그림 8.6에서 본 트리와 같은 형태의 트리를 만들 수도 있는데, 이런 경우 평균
검색시간은 O(n)o] 된다. 정리 8.3은 n7 키로 된 모든 입력에 대한 평균검색시간에
관한 정리이다. 따라서 7개 키로 된 어떤 입력이 주어지면, 평균검색시간이 lig n)o}
될 확률이 많지만, O(n)o] 될 수도 있다. 즉 효율적인 검색이 항상 가능하다는 보장은
없다.

8.3.2 B-E2|
실제 사례에서는 선형검색시간으로 인하여 성능이 심하게 손상될 수 있다. 예를 들면,
거대한 데이터베이스 레코드의 키를 한꺼번에 모두 컴퓨터의 고속메모리(414 : Random
Access Memory®°]@} 부름)에 모두 올려놓을 수 없는 경우가 종종 있다. 그러므로 검색을
수행하기 위해서 보조기억장치인 디스크에 접근(300089)해야 할 수 있다(이러한 검색을
23-94 (external 8687040/이라 하고, 키가 모두 동시에 메모리 안에 있는 경우의 검색을
내부검색(10167081 8687040/이라고 한다). 디스크에 접근하기 위해서는 입ㆍ출력 헤드를 움
직여야 하고, RAMS] 접근하기 위해서는 전자적인 데이터 ASG 하면 되므로 디스크 접
근이 RAM 접근에 비해서 수백 또는 수천 배 느리다. 따라서 선형외부검색은 받아드릴
수 없는 걸로 입증되었고, 그러한 가능성의 여지를 남겨두는 것은 바람직하지 못하다.

이 덜레마에 대한 해는 이미 만들어진 이진검색트리를 입력으로 받아서 같은 키로 구
성된 균형 잡힌 이진검색트리를 출력으로 내주는 균형유지프로그램0631800108 program)
을 작성하는 것이다. 그러면 그 프로그램을 주기적으로 실행하면 이진검색트리의 균형이
유지될 것이다. 알고리즘 3.9가 균형유지프로그램을 만드는 알고리즘이다. 이 알고리즘
은 단순 균형유지알고리즘보다 더 강력하다. 왜냐하면 검색 키가 되는 각 키의 BSS
고려하기 때문이다.

매우 동적인 환경에서는 애초부터 트리를 절대로 불균형되지 않도록 하는 게 나을지도
모른다. 이진트리의 HES 유지하면서 마디를 추가하고 삭제하는 알고리즘은 1962년에


===== PAGE 350 =====
338

chapter 8 계산복잡도: 검색문제

러시아 두 명의 수학자 G.M, Adel'son—Velskii2} E,M, Landis7} 개발하였다(이러한 이유
로 해서 이 균형 잡힌 이진트리를 종종 4\1-트리라고 부른다). 이 알고리즘은 7486
(1994) 등의 데이터구조 AS 보면 나와 있다. 이 알고리즘에서는 검색시간뿐만 아니라
추가하고 삭제하는 시간도 ㅇ(187/)이 보장된다.

1972년에 R, Bayer2} E.M, McCreight= 이진검색트리를 향상시킨 8-트리를 개발하였
다. 키를 8-트리에 추가하거나, 8-트리에서 삭제할 GUase 모두 같은 수준으로 유
지가 보장되는데, 이는 트리의 균형을 유지는 것보다 we}, 8-트리를 조작하는 실제 알
TeSe Kruse(1994) 등의 데이터구조 AS 참조하기 바란다. 여기서는 어떻게 모든 잎
을 같은 수준으로 유지하면서 키를 추가할 수 있는지에 대해서만 간단히 살펴본다.

8-트리는 사실 여러 부류의 트리를 대표한다. 그 중에 가강 간단한 트리는 3-2 트리이
다. 이제 이 트리에 마디를 추가하는 과정을 설명해보자. 3-2 Belo] 특성은 다음과 같다.

© 각 마디에는 키가 하나 또는 둘 있다.

© 내부마디(ㅁ001684)에 키가 하나 있으면 두 개의 자식마디가 있고, 내부마디에 키가
둘 있으면 세 개의 자식마디가 있다.

* 어떤 주어진 마디의 왼쪽 하위트리의 키들은 모두 그 마디에 저장되어 있는 키보다

작거나 같다.
* 어떤 주어진 마디의 오른쪽 하위트리의 키들은 모두 그 마디에 저장되어 있는 키보
다 크거나 같다.

* 마디에 키가 둘 있으면 그 마디의 중간 하위트리의 키들은 모두 왼쪽 키보다는 크
거나 같고, 오른쪽 키보다는 작거나 같다.

＊ 모든 잎은 수준이 같다.

그림 8.7(8)는 3-2 트리를 나타내는데, 그림 뒷부분에서는 어떻게 새로운 키가 그 트리
에 추가되는지를 보여준다. 트리가 잎에서 자라는 대신 뿌리에서 깊이방향으로 자라기
때문에 트리가 계속 균형을 유지할 수 USS 주목하자. 비슷하게 마디를 제거할 필요가
있을 때 트리는 뿌리에서 깊이방향으로 줄어든다. 이런 식으로 모든 나봇잊은 항상 같은
FES 유지하게 되어 검색, 추가, 삭제 시간이 ㅇ(18 7))이 됨을 보장할 수 있다. 트리를
부모 중간횡단 순으로 키를 끄집어내면 정렬 순서가 됨은 명백하다. 이러한 이유 때문에
대부분의 최신 데이터베이스 관리 시스템에서 8-트리를 쓰고 있다.

8.4 해시

키가 1부터 100까지의 정수이고 대략 100개의 레코드가 있다고 가정해보자. 그 레코드를
저장하는 효율적인 방법은 100개의 아이템을 저장할 수 있는 배열을 만들고 키가 :인 레
코드는 Silo] 저장한다. 그러면 레코드를 끄집어내는 건 순간적이고 키를 비교할 필요



===== PAGE 351 =====
0 00000 0
8.4 해시  339

~ 2트리                     (6) 35가 들어갈 YS 찾아서 정렬된 순서로

추가
(0) 만약 Qo] 키가 3개 있으면, 마디를 둘로 나누면서      (0) 만약 부모마디에 키가 3개 있으면, 그 마디를 둘로
중간에 위치한 키를 부모마디로 보냄                  나누면서 중간에 위치한 키를  부모마디르 보냄

(6) 마지막으로 뿌리마디에 키가 3개 있으면, 그 뿌리마디를
둘로 나누면서 중간 위치에 새로 뿌리마디를

그림 8.7 3-2 트리에 새로운 키를 추가시키는 방법

[=|


===== PAGE 352 =====
340

chapter 8 계산복잡도 : 검색문제

가 없다. 대략 100개 정도의 레코드가 있고, 키가 13자리인 주민등록번호인 경우에도 같
은 방법을 사용할 수 있다. 그러나 이 경우 MAS 사용하면 메모리 중심으로 따져보아서
aS

©:

}당히 비효율적이다. 왜냐하면 단지 10072] 레코드를 저장하기 위해서 10조개의 아이
템을 저장할 수 있는 배열이 필요하기 때문이다. 대신에 0에서 99까지의 인덱스로 된 100
개의 아이템만 저장할 수 있는 WSS 만들고, 각 키를 0과 99사이의 값으로 “SHA](hash)”
할 수 있다. 해시함수01884 function) _ 키를 인덱스로 변환하는 함수이고, 어떤 특정한
키에 sell  함수를 적용하는 AS “71S 해시한다"라고 한다. 주민등록번호의 경우 가능한
해시함수는 다음과 같다.

h(7]) = 7] % 100

(여기서 %연산은 키를 100으로 나눈 나머지 값을 내준다) 사실 이 함수는 키의 마지막
두 디찌트만을 내줄 Bo an  Hof 어떤 특정한 키를 1 해시한다면 그 키와 해당 레코드
9101]에 저장한다. 이 방법은 키를 정렬된 순서로 저장하지 않는데, 이는 레코드를 정
el He Toh Bar} 전혀 없는 BOO ABA 있다는 걸 뜻한다. 만약 그
게 필요한 경우에는 앞에서 공부했던 방법들을 써야 한다.
만약 27H 키가 같은 인덱스 값으로 해시되지 않는다면 이 방법은 잘 돌아간다. 그러나
키의 수가 상당히 많을 때는 그럴 가능성이 거의 없다. 예를 들면, 키가 100개 있고, 각
키가 100개 중에서 서로 다른 인덱스에 각각 해시될 확률이 거의 같다고 하면 두 개의
키가 같은 인덱스에 해시되지 않을 확률은 다음과 같다.
100!
10010

최소한 두 개의 키가 하나의 인덱스로 해시된다는 건 거의 확실하다. 이러한 경우를 충돌
(collision) 또는 해시충돌(6888 0891)이라고 한다. SSS 해결하는 방법은 여러 가지가
있다. 가장 좋은 방법 중 하나는 열린해시(6060 hashing)o]t}, 이 방법은 열린주소찾기
(open 80076881709)이라고도 한다. 열린해시에서는 각 해시 값마다 바구니640561)를 하
나씩 만들고, 그 값으로 WISE 키는 모두 그 값에 딸린 바구니에다 넣는다. 열린해시
는 연결 리스트(10160 list) 보통 구현한다. 예를 들어, 수의 마지막 두 디지트로 해시
된다면 Bucket& 가리키는 포인터 HSS 0에서 99까지의 인덱스를 가지도록 만든다.
if 해시되는 키는 모두 2204600에서 시작하는 연결된 리스트에 위치시킨다. 그림 8.8
에서 예를 들어 잘 설명해 주고 있다.

바구니의 개수가 키의 개수와 같을 BRE 없다. 예를 들어, 수의 마지막 두 디지트로
해시된다면 바구니의 수는 반드시 100개여야 한다. 그러나 100, 200, 1000 또는 어떤 키
라도 저장할 수 있다. 물론 키의 개수가 많아질수록 충돌횟수도 많아질 것이다. 만약 키
의 개수가 바구니의 개수보다 크다면, SSS 확실히 발생한다. 바구니는 포인터만 저장
하기 때문에 바구니를 할당하는데 그리 많은 저장장소를 낭비하는 건 아니다. 그러므로

=9.3x10 %



===== PAGE 353 =====
@ㅎ00000 0
8.4 해시  341

———>|_567-21-7100 | ㅡ}--커| 234-76-8100 [NULL]

Bucket [0]

———— >} 267-89-5401 [NULL]

Bucket [1]

——>_330-38-0172 | —}——>|_435-87-9872 | —|>| ‘897-38-6872 [NULL]

Bucket [72]

—  432-87-0199 |NULL|

Bucket [99]
그림 8.8 열린해시의 사례. 마지막 = 디지트가 같은 ㅋ

는 같은 바구니에 들어감.

키의 개수만큼 바구니를 할당해도 별 문제가 없다.

키를 검색할 때 키가 있는 바구니(연결 리스트)를 순차검색할 필요가 있다. 만약 키가
모두 같은 바구니로 해시된다면 이 검색은 순차검색으로 퇴보되어 버린다. 이러한 경우
가 발생할 확률은 얼마나 될까? 만약 100개의 키와 100개의 바구니가 있고, 각 키가 100
개 중에서 서로 다른 인덱스에 각각 해시될 확률이 거의 같다고 하면, 키가 모두 같은
바구니에 들어갈 확률은 다음과 같다.

1

100     18

크러므로 키가 모두 같은 바구니에 들어갈 가농성은 거의 없다고 보면 된다: 그러면
90, 80, 70 또는 다른 많은 개수의 키가 같은 바구니에 들어갈 기회는 어떻게 될까? 실제
로 우리가 관심을 가져야 하는 건 해시검색이 과연 이분검색에 비해 평균적으로 얼마나
더 좋은지 여부이다. 파일(816/이 꽤 큰 경우 이 궁금중에 대한 해답은 거의 긍정적이다.
그러나 해시를 사용함으로써 얼마나 좋아지는지를 먼저 알아보자.

직관적으로 가장 좋은 건 키가 바구니에 균일하게 분포되어 있는 경우임은 틀림없다.
즉, 만약 개의 키와 m 7A] 바구니가 있을 때 각 바구니에는 n/m 742] 키가 있다는 것
이다. SAIS n°] m2] 배수일 때만 정확하게 n/m 7H] 키가 각 바구니에 들어가게
된다. 그렇지 않다면 대략적으로 균일하게 분포되어 있다고 얘기할 수밖에 없을 것이다.
키가 균일하게 분포되어 있을 때 어떻게 되는지 다음 정리에서 보여준다. 간단히 설명하
기 위해서 정확하게 균일 분포된 경우만 다룬다(즉, 7 이 mo] 배수인 경우).

> 정리 8.4
만약 n AHS] 키가 7/개의 바구니에 균일하게 분포되어 있다면 실패한 검색에서 비교 횟수는



===== PAGE 354 =====
@00@000000
342    chapter 8 계산복잡도: 검색문제

© 예제 8.1

/'번이다.
증명 : 키가 균일하게 분포되어 있기 때문에 각 바구니의 키 개수는 7/7이다. 즉 이는 실패한
검색은 모두 7/71번의 비교를 필요로 한다는 걸 뜻한다.

> Bel 8.5
만약 개의 키가 mA] 바구니에 균일하게 분포되어 있고, 각 키가 검색 키가 될 확률이 거의
같다고 하면, 성공한 검색의 평균 비교 횟수는 다음과 같다.
n    1
202 2

증명 : 각 바구니의 평균검색시간은 n/m HS] 키를 순차검색하는 경우 평균 검색시간과 같다.
평균의 경우 분석에 의하면 위와 같다.

만약 키가 균일하게 분포되어 있고 7=277이라면, 실패한 검색은 각각 2m/m =2번의 비교만
필요하고, 성공한 검색은 평균 비교 횟수가 다음과 같다.

200 」 1

2072 2 2

만약 키가 균일하게 분포되어 있으면 검색시간은 매우 작다. 그러나 비록 해시가 그렇
Al 예외적으로 좋은 결과를 줄 가능성이 있음에도 불구하고, 혹자는 검색이 거의 순차검
색에 가깝게 퇴보하지 않기 위해서는 그래도 이분검색을 사용해야 한다고 주장할지 모른
다. 그래서 다음 정리는 파일이 꽤 큰 경우 해시가 이분검색만큼 나쁘게 되는 기회가 적

는 걸 보여준다. 이 정리에서는 각 키가 서로 다른 바구니로 각각 해시될 확률이 거의
같다고 가정한다. 주민등록번호가 마지막 두 디지트로 해시될 때 이 가정은 전혀 무리가
없다고 할 수 있다. 그러나 모든 해시함수가 이 기준을 만족하는 건 아니다. 예를 들면,
영어이름이 마지막 두 디지트로 해시되는 경우 "로 해시되는 경우가 "02 로 해시되는
경우보다 훨씬 많을 것이다. 왜냐하면 "\'로 끝나는 이름이 훨씬 많기 때문이다. Kruse
(1994)와 같은 데이터구조 책을 보면 좋은 해시함수를 찾는 Bol 대해서 설명한다. oF
기서 우리의 목표는 해시가 검색문제를 얼마나 잘 해결하는지 분석하는데 있다.

> 정리 8.6
만약 개 키와 개의 바구니가 있고, 각 키가 서로 다른 바구니로 각각 해시될 확률이 거
의 같다고 가정하면 한 개의 바구니에 최소한 k7 키가 들어있을 SS 다음보다 작거나
같다.



===== PAGE 355 =====
@0000000
8.4 해시  343

n\{ 1 16
증명 : 주어진 바구니에 대해서 어떤 특정한 *개 키의 조합이 그 바구니에 들어갈 확률은
(1/7,)"이다. 이는 그 바구니에 최소한 이 조합으로 키가 들어있을 확률이 (1/m)* BRE 의미이
다. 일반적으로 두 Ab (events) S2} Tol] 대해서 다음 부등식이 성립한다.
p(S or T)<p(S)+p(7)                  (8.1)
그러므로 주어진 바구니에 최소한 개 키가 있을 확률은 《개 키의 각각 다른 조합으로 된 키
가 최소한 있을 확률의 총합보다 작거나 같다. *개 키의  7) 7424 다른 조합은 7개 키에서 구
할 수 있기 때문에(부록 AL] ㅅ.7절을 참조) 어떤 주어진 바구니가 최소한 《개 키가 들어 있을
확률은 다음보다 작거나 같다.
n\{ 1 \*

이제 위 식 (8.1)과 m7HS] 바구니가 있다는 사실에 의해서 이 정리는 성립한다.

이분검색의 평균검색시간은 대략 8 7이었음을 상기해보자. 표 8.1을 보면 여러 7 값
에 대해서 최소 한 개의 바구니에 최소한 개와 218 n7H 키가 들어있을 확률의 상한이
나타나 있다. 이 표에서는 > =7ㅠ이라 가정한다. 비록 no] 1289 때조차도 검색시간이
218 nS 초과할 SSS 10억분의 1보다도 작다. no] 1,024이면, 검색시간이 Ag nS 초
과할 확률은 1억 곱하기 1억분의 3보다 작다. nO] 65.580이면, 검색시간이 le ㅠ을 초과할
SSS 10억분의 3 가량이다. 한 번의 비행기 여행에서 사고로 죽을 확률은 100만분의
6 정도이고, 평균적인 경우 자동차 사고로 죽을 확률은 100만분의 270이다. 그러나 사람
들은 보통 비행기나 자동차 타기를 굳이 꺼려하지 않는다. 여기서 요점은 사리에 맞는
결정을 내리기 위해서 우리는 종종 극히 작은 확률은 거의 불가능으로 취급한다는 것이
다. no] 큰 경우 이분검색 대신 해시를 사용하면 성능이 보다 더 좋을 게 거의 확실하기
때문에 그렇게 해도 괜찮은 것이다. 1970년대에 일어난 재미있는 실례를 하나 들어보자.
어떤 컴퓨터 제조업자가 새로 나온 비싼 하드웨어를 사라고 데이터처리 관리인을 설득하
는 과정에서 주로 쓴 수법은 인위적으로 시나리오를 하나 만들어 놓고 그 시나리오대로
일이 일어날 경우 벌어지게 될 재앙을 설명하는 것이었다. 여기서 그 당시 데이터처리

@ 표 8.1 최소한 한 개의 바구니에 최소한 /개 키가 들어있을 확률의 상한
n            k=lgn@l 경우 상한         ^=2187인 경우 상한
128               .021                          7 00. iy
1,024            00027                       345 X10
8,192             0000013                      1,95 × 108

65,536            3.1 X< 10°                    D7 x10



===== PAGE 356 =====
@0 00000 0
344    chapter 8 계산복잡도: 검색문제

관리인이 종종 간과하였던 이 수법의 결함은 그 시나리오가 발생할 확률은 거의 무시할
만하다는 사실이었다. 위험을 싫어하는 건 개인이 선택할 문제이다. 그러므로 너무 심하
게 위험을 싫어하는 사람은 10억분의 1이나 1억 곱하기 1억분의 8의 기회도 취하지 않을
수도 있다. 그러나 개인의 취향에 따라 결정한 건 아닌지 심각하게 고민하지 않고 결정해
서는 곤란하다. 이러한 BAS 하는 방법은 Clemen(1991) 2] 책에 나와 있다.

@  8.5 선택문제: 방해꾼(적) 논법의 소개

지금까지 키가 개인 리스트에서 를 검색하는 방법을 공부했다. Sele 선택문제
(selection 2ㅁ7001620라고 하는 다른 종류의 검색문제를

인 리스트에서 《번째로 큰 (또는 《번째로 작은) 키를 찾는 것이다. 여기서 키는 정렬되지
않은 배열에 있다고 가정한다(배열이 정렬된 경우는 사소하게 쉽다). 먼저 = 1인 경우
즉 최대키(또는 최소키)를 찾는 경우에 대해서 생각해보자. 그 다음에는 최소키와 최대키
를 동시에 찾으면서 각각 따로 찾는 경우보다 비교 횟수가 적게 되는 경우를 살펴본다.
그리고 k= 23인 경우, 즉 두 번째 작은 키(또는 두 번째 큰 키)를 찾는 경우에 대해서 공
부해본다. 마지막으로 일반적인 경우에 대해서 다루어본다.

oN

8.5.1 최대키 찾기
다음은 최대키를 찾는 쉬운 알고리즘이다.

SRS 82 최대키 찾기

문제 : 크기가 nel 배열 에서 최대키를 찾으시오.
입력 : 양의 정수 7, 1에서 7까지의 인덱스를 가진 키의 배열 6
출력 : Soy 최대키의 We 가진 변수 4480

void find _Jargest (int 22,

const keytype 이],
keytype& Jarge)

{

index /;

large = S{1];
for (i = 2; i <= nm; H+)
if (S[7] > Jarge)
large = Sf i];

명백히 알고리즘에서 키를 비교하는 횟수는 다음과 같다.



===== PAGE 357 =====
eee
85 선택문제: 방해꾼(적) 논법의 소개   345

T(in)=n-1

직관적으로 여기서 더 이상 성능을 개선하기가 불가능해 보인다. 다음에 공부할 정리가
이 사실을 확인해 준다. 최대키를 결정하는 알고리즘을 키끼리의 토너먼트 경기로 생각
해 볼 수 있다. 이루어지는 비교는 각각 그 토너먼트에서 한 번의 시합으로 보고, 큰 키는
비교에서의 승자00ㅁ0@0가 되고, 작은 키는 패자00800가 된다. 최대키는 토너먼트의 우
승자가 된다. 이 절에서는 이 용어를 그대로 사용한다.

> 정리 8.7

가능한 BE 입력 :개 중에서 비교만으로 최대키를 찾을 수 있는 결정적 알고리즘
우라도 반드시 최소한 비교를 7ㅡ1번 해야 한다.

증명 : 모순유도로 증명한다. 즉, 크기가 7인 임의의 입력에 대해서 임의의 알고리즘이 7 -1
번 미만 비교한다면, 그 알고리즘은 임의의 다른 입력에 대해서는 틀린 답을 줄 수밖에 없다는
WAS 보인다. 결국 임의의 입력에 대해서 최대 7-2번 비교하여 최대키를 찾는다면 그 입력
에서 비교되지 않는 최소 2개 키가 반드시 존재한다. 최소 이 두 개의 키 중 하나는 최대키로
BUS 수 없다. (필요하다면) 그 키를 원래 입력에 있는 모든 키보다 큰 키로 바꾸어서 새로운
입력을 만들 수 있다. 여기서 새로운 입력에 대하여 비교한 결과도 원래 입력에서와 같을 것이
므로, 그 새로운 키는 최대키로 보고되지 않을 것이다. 이는 알고리즘의 새 입력에 대해서 틀
린 답을 준다는 것을 의미한다: 이와 같이 모순이 유도되었으므로 알고리즘은 크기가 인 모
는 입력에 대해서 최소 7ㅡ1번은 비교해야 한다는 사실이 증명되었다.

N

|

은 어느 경

'

정리 8.?을 정확하게 해석하는데 SAS 기울여야 한다. 비교만으로 검색하는 알고리
즘은 모두 가장 큰 키를 찾는데 최소 n— 14 비교해야 한다는 A 의미하는 건 아니다.
예를 들면, 배열이 정렬되어 있으면 한 번도 비교하지 않고도 배열의 마지막 아이템을
넘겨줌으로써 최대키를 찾을 수 있다. 그러나 배열의 마지막 아이템을 넘겨주는 알고리
즘은 최대키가 마지막 아이템인 경우만 최대키를 찾을 수 있다. 가능한 모든 입력에 대해
서 최대키를 찾을 수 있는 것은 아니다. 정리 8.72 가능한 모든 입력에서 최대키를 찾을
수 있는 일고리즘에 관련된 정리이타.

물론 알고리즘 8,29} 비슷한 알고리즘을 사용하여 7ㅡ1번 비교하여 최소키를 찾을 수
있고, 정리 8.7과 비슷한 정리를 사용하여 n— 1°] 최소키를 찾는 하한이라는 AMIS 증

명할 수 있다.

8.5.2 최소키와 최대키를 모두 찾기
최소키와 최대키를 동시에 쉽게 찾으려면 알고리즘 8.8를 다음과 같이 수정하면 된다.


===== PAGE 358 =====
@‥0000000
346 chapter 8 계산복잡도: 검색문제

> 알고리즘 8.3

bk

소키와 최대키 찾기
제 : 크기가 nel 배열 에서 최소키와 최대키 찾기

: 양의 정수 7, 1에서 7까지의 인덱스를 가진 키의 배열 9

: 배열 에서 최소키와 최대키를 각각 가진 변수 smalls} large

m+ c2 ro
J

J

void find_ both (int n,

const keytype 의],
keytype& small,

keytype& J/arge)

index /;
small = 5/1];
large = S{1];

for (¢ = 2; 7 <= nm; H+)
if (S[ 7] < small)

small = S{i |;
else if (S{i] > Jarge)
large = Sf i];

> 알고리즘 8.4

알고리즘 8.8을 사용하면 최소키와 최대키를 독립적으로 찾는 것보다는 좋다. 왜냐하
면 어떤 입력에 대해서 SLi] Qf 8780의 비교가 모든 에 대해서 이루어지지 않기 때문이
다. 따라서 모든 경우의 수행성능은 개선되었다. 그러나 9111이 최소키가 되면, WE iol
대해서 비교해야 한다. 그러므로 최악의 경우 키의 비교 횟수는 다음과 같다.

W(n) = 2(n—1)

이는 최소키와 최대키를 각자 따로 찾는 경우에 비교 횟수와 정확하게 같다. 이 경우 성
능개선이 불가능한 것처럼 보이지만 사실은 가능하다. 모든 키를 짝을 지워 각 쌍 가운데
작은 키를 찾는다. 이 작업은 7/2번 비교하여 이루어진다. 작은 키 가운데서 최소키를
찾는데 7/2번 비교하면 되고, 큰 키들 가운데 최대키를 찾는데 7/2번 비교하면 된다.
이런 ACS 하면 37/2의 총 비교만으로 최소키와 최대키를 찾을 수 있다. 이 방법의

알고리즘은 다음과 같다. 이 알고리즘은 no] 짝수라고 가정한다.

키를 짝 지워서 최소키와 최대키 찾기
문제 : 크기가 7인 배열 에서 최소키와 최대키 찾기

입력 : 얄의 정수이며 짝수인 7, 1에서 7까지의 인덱스로 된 키의 배열 6
출력 : 배열 에서 최소키와 최대키를 각각 가진 변수 small} large



===== PAGE 359 =====
0000000
85 선택문제: 방해꾼(적) 논법의 소

No
=
wo
KR
N

void find_ both? (int n,                         // ne 짝수라고 가정함
const keytype 의],
keytype& szall,
keytype& J/arge)

index 고
if (941 < 921) {
small = S{1];
large = 이기;
}
else {
small = S{2);
large = S{1];
}
for! (2 = "3s 1 <= n= 1p a = 742) 4       // R= 2씩 증가

if (S[7] < small)

small = Sf i] ;
if (S[i+1] > large)
large = S{i+ 1];
}
else {

if (917 + 1] < small)

small = ,9[7+ 1] ;

if (S[i] > Jarge)
large = S{ i];

이 홀수일 때도 이 알고리즘이 작동하도록 수정하는 것과 키의 비교 횟수가 다음과

Hee 증명하는 것은 연습문제로 남겨둔다.

no] 짝수이면, —2
aN) =           37 3
#이 줄쑤이에, 녹-즘

여기서 성능을 개선시킬 수 있을까? 답은 "아니오"임을 보여주려고 한다. 결정트리는
사용하지 않을 텐데, 그 이유는 결정트리가 선택문제와는 잘 맞지 않기 때문이다. 이유는
다음과 같다. 선택문제를 위한 결정트리는 /가지의 가능한 결과가 존재하기 때문에 최소
한 nA] AS 포함해야 한다. 보조정리 7.3에 의하면 이진트리와 7개의 잎이 있다면
그 깊이는 |1871|보다 크거나 같다. 그러므로 잎 개수의 하한은 최악의 경우 비교 횟수의
하한이 11871. 1이다. 이는 별로 좋은 하한이 아니다. 왜냐하면, 최대키를 찾는데만 최소한


===== PAGE 360 =====
348

chapter 8 계산복잡도: 검색문제

”- 1번은 비교해야 한다는 사실을 이미 알고 있기 때문이다(정리 8,7), 보조정리 8.1은
더 이상 유용하지 않은데, 그 이유는 결정트리에는 반드시 비교마디가 n— 174 존재해야
한다는 사실을 바로 확립할 수 있기 때문이다. 선택문제에는 결정트리가 잘 작동되지 않
는데, 왜냐하면 결과가 하나 이상의 잎에 나타날 수 있기 때문이다. 그림 8.9는 7=4일
때 알고리즘 8.2(최대키 찾기)에 대한 결정트리를 보여준다. 4의 답을 주는 잎이 4개 있
고, 8의 답을 주는 잎이 2개 있다. 그 알고리즘에서 수행되는 비교 횟수는 Ign = 184 = 2
가 아니라 3이다. 여기서 87의 약한(부실한) 하한이라는 것을 알 수 있다.

하한을 구하기 위해서 방해꾼 2 (adversary argument)o]e} 불리는 또 하나의 방법을
사용한다. “HSH Tt 경기에서 상대편이나 적을 말한다. 가령 한 여학생이 미팅을 나갔
는데, 관심있어 하는 어떤 남학생이 "너 떠가 뭐니?" 같은 Ags ALS 했다고 가정해
보자. 누구나 알다시피 띠에는 12종류가 있고, 태어난 해에 따라서 떠가 결정된다. 가령
1976년생이면 용떠가 된다. 이런 AYst 질문에 바로 대답을 하면 재미가 별로 없으므로
이 여학생은 방해꾼이 되기로 한다. 여학생은 “그래"/“아니"로 대답할 수 있는 질문만 하
여 떠를 맞추어 보라고 남학생에게 요구한다. 방해꾼이 된다는 건 자신의 WS 알려줄
의도가 없는 것이므로 무조건 남학생이 가능하면 BES 많이 하도록 유도해야 한다. 그
러므로 되도록 답을 늦게 AES 대답을 해야 한다. 예를 들어, 가령 남학생이 "너의 WS
나타내는 SSS 다리가 4개니?"라고 묻는다고 하자. 만약 "아니"라고 대답한다면 3개
(용, 뱀, 닭) 중에 하나로 범위가 좁혀지고, 만약 "그래"라고 대답한다면 나머지 ?개 중
하나로 범위가 좁혀지므로, "그래"라고 대답한다. 남학생이 다시 "그 동물이 가축이니?"
라고 묻는다면 "그래"라고 대답한다. 왜냐하면, 남은 동물 중에서 과반수가 가축이기 때
문이다. 여기서 대답할 때 주의해야 할 BS 이미 준 답과 일관성을 유지해야 한다는 사

그림 8.9 n=42 때 알고리즘 8.2의 결정트리



===== PAGE 361 =====
@00@00600000
8.5 선택문제: 방해꾼(적) 논법의 소개     349

실이다. 예를 들어, 만약 그 떠를 나타내는 SES] 다리가 4개라는 사실을 잊고 다리가
2개냐고 다시 묻는다면 "그래"라고 대답하면 이미 준 답과 모순이 되기 때문에 ot 된다.
일관성이 없는 Tol] 해당하는 WE 없다. 남아있는 해답후보의 개수가 최대가 되도록 A
문에 대답하고, 그 답이 일관성이 있기 때문에 그 남학생이 논리적인 결론에 도달하기
전에 가능하면 많은 질문을 하게 할 수 있다.

어떤 방해꾼의 목표가 (남학생의 경우와 마찬가지로) 알고리즘이 되도록 비효율적으
로 작농하도록 하는 것이라고 가정해보자. 알고리즘에서 결정을 해야 하는 지점마다 (예:
키의 비교 직후) 방해꾼은 가능하면 알고리즘을 느리게 실행하게 하는 ABS 선택한다.
여기서도 유일한 제한사항은 이미 준 답과 언제나 일관성 있게 결과를 선택해야 한다는
것이다. 결과를 일관성 있게 선택하는 한, 그러한 결과가 일어나도록 하는 입력은 반드시
존재한다. 만약 방해꾼이 알고리즘의 단위명령을 /(11)번 실행하도록 한다면 /(/))은 그
알고리즘의 최악 시간복잡도를 나타내는 하한이다.

최대키와 최소키를 모두 찾는데 필요한 soto] 경우 비교 횟수 하한을 구하는데 방해
꾼 논법을 사용한다. 그 하한을 구하기 위해서 키들은 모두 다르다고 가정한다. (키가 모
두 다른 경우) 입력의 일부분에 대한 최악 시간복잡도의 하한은 입력전체를 고려한 경우
의 하한이기 때문에 이렇게 가정할 수 있다. 정리를 살펴보기 전에 방해꾼이 세우게 될
전략을 생각해보자. 비교만으로 최소키와 최대키를 찾는 BAS 푸는 알고리즘이 있다고
가정해보자. 만약 키가 모두 다르다면 알고리즘 실행 중 언제라도 주어진 키의 상태
(state) = 다음 중 하나이다.

상태        상태의 의미

x           이 키는 아직 한 번도 비교하지 않았다

L            이 키는 비교에서 최소 한 번은 졌고, 한 번도 이기지 않았다
Ww           이 키는 비교에서 최소 한 번은 이겼고, 한 번도 지지 않았다
LW          이 키는 비교에서 최소 한 번은 졌고, 최소 한번은 이렸다

위의 상태들은 가지고 있는 정보의 개수를 나타낸다. 만약 키의 상태가 라면, 정보가
하나도 없는 걸 뜻한다. 만약 키의 상태가 Ｌ이나 라면, 그 키가 최소한 한 번은 비교에
서 이겼거나 졌다는 걸 알기 때문에 정보의 개수는 하나이다. 만약 키의 상태가 1\라면,
그 키가 비교에서 이기기도 지기도 했다는 A 알기 때문에 정보의 개수는 둘이다. small
키는 최소값을 가지고, Jarge 키는 최대값을 가지도록 알고리즘을 만들기 위해서는 244
을 제외한 모든 키는 최소한 비교에서 한 번은 이기고 largeS 제외한 모든 키는 비교에
서 한 번은 진다는 사실을 염두에 두어야 한다. 즉 알고리즘은 다음 개수만큼의 ABS
배워야 한다.
(n—1)+(n-1)=2n-2

알고리즘은 비교할 때마다 가능하면 ARS 덜 제공하고 싶어 한다. 예

때
que
[묘
12
ral
aus
ON


===== PAGE 362 =====
0 00000 0
350    chapter 8 계산복잡도 : 검색문제

© 예제 8.2

@ 표 82 최소키와 최대키를 찾는 알고리즘을 물리치기 위한 방해꾼의 전략

피코 4        방해꾼이 더 크다고        비교 주         알고리즘에 의해서

들            선언한 키            <        배운 정보의 개수
Xx      X                8;            W      L                2
X       L                8;            W      L                 al
xX      W                8;            L       W                1
x      WL               8;            \      WL               1
L       L                8;            WL     L                 1
L       W                8;            L       W                0
L       WL               8;            L       WL               0
W      \                8;            W      WL               if
W      WL               8;            \      WL               0
WL     WL      이전 답과 일관성 유지 Wh     WL               0

이 처음 8,5} 6;를 비교한다면, 방해꾼이 어떤 대답을 해도 상관없다. 왜냐하면, 제공되
는 정보는 어느 쪽이나 2개이기 때문이다. 방해꾼이 6,라고 답한다고 하자. 그러면 s, 2
상태는 ※에서 \로 바뀌고, 6, 의 상태는 ※에서 Ｌ로 BATH, 알고리즘이 다음 535} 6, 을
비교한다고 하자. 만약 방해꾼이 6, 이 더 크다고 대답하면, 6, 의 상태는 \에서 \Ｌ로,
552] 상태는 ※에서 Ｌ로 BRACH, 이는 정보 2개가 노출되었다는 뜻이다. 만약 6』이 더
크다고 대답하면 노출되게 될 정보는 한 개뿐이기 때문에 방해꾼은 이 FS 선택할 것이
다. 표 8.28 보면 항상 노출되는 정보가 최소가 되는 방해꾼의 전략이 나와 있다. 어떤
키를 선택해도 상관 없는 경우는 무조건 비교에서 앞에 있는 것을 선택한다. 이 전략만
가지면 아래 정리를 증명할 수 있다. 그러나 방해꾼이 이 전략을 실제로 어떻게 사용하는
지 먼저 살펴보자.

표 8.8을 보면 Yeo] 크기가 5인 경우 알고리즘 8.8을 물리치기 위한 방해꾼의 전략이 나타나
있다. 여기서 답들과 일관성 있게 키의 값이 할당되었다. 정말 꼭 필요하지는 않지만 두 키가
모두 WL 상태가 될 경우 일관성 있는 TS 줄 수 있게 방해꾼은 답이 나오는 키의 순서를 반드
기억하고 있어야 한다. 이를 쉽게 할수 있는 WUE BE 할당하는 것이다. 더구나 값을 할당
하게 되면 일관성 있는 답들이 그와 관련된 입력과 짝을 이루고 있는지 한눈에 알아낼 수 있다.
방해꾼의 전략으로 결정된 SHS 제외한 다른 PSS 임의로 선택한다. 예를 들면, 6,이 6,보
다 더 크다고 선언된 경우 6,에 159] 값을 준다. 사실 10보다 큰 값이라면 어떤 값이라도 줄
있었다.

5,3} 6,를 비교한 후 6,의 BS 18에서 30으로 바꾼다는 사실을 주목해보자. 알고리즘이 주어
지면 방해꾼은 실제 입력이 주어지지 않음을 기억하라. 방해꾼이 알고리즘의 결정을 넘겨받을



===== PAGE 363 =====
85 MERA: Botts) 논범의 소개     351
@ 표 8.3 입력의 크기가 5인 경우 알고리즘 8.3을 물리치기 위해 시도한 방해꾼의 |

ss      방해꾼이 더              상태/할당된 값           알고리즘에 의해서

크다고 선언한 기 _      85      98      94      s, We 정보의 개수
& Ss,           %,          L/10 W/20 x       X       Xx               2
5 aw,           85          L/10 Ww/20 x       X       x               0
iy Om,         8,        L/10 W/20 W/ls x      x            1
55 > 8»           85          L/10  WL/20 w/30 xX       Xx               1
이 So,       iy      L/10 WL/20 W/30 W/I5 xX         1
5,35,         이        L/10  WL/20 WL/30 W/40 <            1
S65 <8;       Ss      L/10  WL/20 WL/30 W/40  W/15       1
ee,         Ss        L/10  WL/20 WL/30 WL/40 W/50         1

때마다 답(그리고 따라서 입력 값)은 동적으로 만들어진다. 6,의 값이 15보다 크고 방해꾼의 답
은 이 6;보다 크다는 것이므로 6;의 값은 15에서 바꿀 필요가 있다.

알고리즘의 수행이 끝난 후 8,이 다른 모든 키에게 졌고, 5,7) 다른 모든 키에게 이겼다. 따라
서 8, 은 가장 작은 키이고, 6,는 가장 큰 키가 된다. 방해꾼이 만든 치려 9, 을 가장 작은 키로
했는데, 왜냐하면 그 입력이 알고리즘 8.8이 가장 힘들게 비효율적으로 수행하게 하는 입력이기
때문이다. 표 8.8에 의하면 모두 8번의 비교가 이루어졌고, 알고리즘 8.8에 의해서 이루어진 최
악의 경우 비교 횟수는 입력의 크기가 5일 때 다음과 같다.

W(5) =2(5-1) =8
이는 입력의 빠지 = i 우리의 방해꾼이 알고리즘 8.30] 가능한 힘들게 비효율적으로 수행
되도록 하는데 %   134

최대키와 최소키를 찾는 다른 알고리즘이 주어진다면 방해꾼

한 힘들게 비효율적으로 실행되도록 하는 답을 주려                다. 알고리즘 8.4(키
를 비교하여 최소키와 최대키 찾기)와 임의의 입력의 크기가 주어진 경우 방해꾼의 답이
무엇이 될지 말아보기를 권한다.

방해꾼의 전략을 개발할 때 주어진 문제를 알고리즘이 가능한 한 힘들게 풀도록 하는

Al 우리의 목표이다. 방해꾼 전략이 빈약하면 이 목표를 이룰 수 없을

> Bel] 8.8

가능한 모든 입력에서 비교만으로 nO] 7] 가운데 최소키와 최대키를 모두 찾을 수 있는 결
정 알고리즘은 최악의 경우 최소한 다음 만큼의 비교를 수행해야 한다.



===== PAGE 364 =====
352

chapter 8 계산복잡도: 검색문제

no] 짝수이면, S92
no] 홀수이면, SS

중병 . 77; 모두 다들 a 알고리즘이 최소한 이 GSS] 비교를 수행해야 한다는 걸 보임으로
써 이 값이 최악의 경우의 하한임을 보인다. 앞에서 말했듯이 최소키와 최대키를 모두 찾기
위해서 알고리즘은 24-  2742  정보를 반드시 배워야 한다. 우리 이 알고리즘에 방해꾼을 사
용한다고 가정해보자. 비교할 때 두 키가 모두 이전 비교에 쓰이지 않은 경우에만 방해꾼은
한 번 비교에 두 개의 ABS 제공한다는 AS 표 8.2를 보면 알 수 있다. 만약 no] 짝수이면,
최대한 다음의 횟수만큼의 비교를 수행하는 경우가 될 수 있다.

긍 회 비교

이는 이런 식으로 하면 알고리즘은 최대한 2(n/2) =7개의 정보를 얻을 수 있다는 것을 뜻

다. 다른 비교에 대해서는 방해꾼이 최대한 1개의 정보를 제공하기 때문에 알고리즘은 최소한

필요한 정보를 모두 얻기 위해서 다음 횟수만큼을 추가적으로 비교해야 한다.
2n-2-—n=n—-2

그러므로 방해꾼은 알고리즘이 최소한 다음 만큼의 비교를 하게 한다.

n      3n
6  20  2

전
pc
abs)
+
[은
on
4o
42
Ae
Le
rlo
ach

습문제로 남겨 둔다.

알고리즘 8.4는 정리 8.8의 범위 안에서 비교를 수행하므로 이 알                 의경
우 최적이다. 우리는 쓸모 테세 방해꾼을 선택했다고 할 수 있는데,  aus 제공되는
하한만큼 수행되는 알고리즘을 찾았기 때문이다. 따라서 어떤 다른 방해꾼도 더 큰 하한
을 제공할 수 없다는 걸   이제는 안타.

예제 8.2는 왜 알고리즘 8,30] 준최적(6400200109))인지를 보여준다. 그 예제에서 알고
리즘 8.8은 정보를 8개 배우기 위해서 비교를 8번 수행하였다. 반면 최적 알고리즘이었
다면 6번만 수행하였을 것이다. 표 8.8의 두 번째 비교는 쓸모가 없는데, 왜냐하면 배우
는 정보가 없기 때문이다.

방해꾼 논법을 사용할 때 방해꾼은 때로 오라클(60806, 현인)이라고 부르기도 한다.
고대 그리스와 로마사람들에게 오라클이란 인간이 제시한 질문을 대답하는 지식이 많은
실체였다.

85.3 차대키 찾기
차대키(6600ㅁ0ㄱ18868 key)S 찾기 위해서 알고리즘 8.2(최대키 찾기)를 사용하여 n- 1



===== PAGE 365 =====
@‥06@00000 0
8.5 선택문제: 방해꾼(적) 논법의 소개   353

번 비교하여 최대키를 찾고, 그 키를 제외한 후 알고리즘 8.2를 다시 사용하여 7-2번
Ae  wo 남은 키 중 최대키를 찾을 수 있다. 그러므로 22 - 3번 비교하여 차대키를 찾을
수 있다. 이 비교 횟수를 분명히 향상시킬 수 있는데, 그 이유는 최대키를 찾는데 수행한
비쿄들이 차대키를 찾을 때 필요한 비교를 생략하는데 사용할 수 있기 때문이다. 즉, 최
대키가 아닌 다른 키와 비교해서 패배한 키는 차대키가 될 수 없다. 다음에 설명할 토너
먼트 방법은 이 사실을 이용한다.
토너먼트 방법(1047ㅁ80606 27ㅁ60[800)은 패배하면 탈락하는 토너먼트 경기에서 사용한
방식을 =] 때문에 그렇게 명명하였다. 예를 들면, 미국 대학농구 우승팀을 가리기
위해서 64개 팀이 NCAA 토너먼트에서 겨룬다. 각 팀은 짝을 지워 1회전에서 32경기를
치른다. SES 3274 팀은 3회전에 다시 BS 지워 16경기를 치른다. 이 과정은 결승전에
서 두 팀만 남을 때까지 계속된다. 결승전에서 승리한 Bo] 우승한다. 우승팀을 가리는데
18 64= 6 회전을 치르게 된다.
간단히 설명하기 위해서 숫자는 모두 다르며 n= 29] 거듭제곱이라고 가정한다. NCAA
토너먼트에서 하듯이 키를 짝 짓고 마지막 회전이 남을 때까지 각 회전에서 짝을 비교한
다. 만약 8개 키가 있으면 1회전에서는 4번 비교하고, 3회전에서는 241 비교, 마지막 회
전에서는 한 번 비교한다. 마지막 회전의 승리자가 최대키가 된다. 그림 8.10은 이 방법
을 보여준다. 토너먼트 방법은 no] 29] 거듭제곱일 때만 바로 즈  비테 수 있다. 동이
않을 때는 배열의 크기가 2의 거듭제곱이 되도록 배열의 뒷부분에 충분한 아이템을 추가
할 수 있다. 예를 들면, 배열이 53개의 정수로 되어 있으면 - <0 (음의 : 무한대) 값을 가진
아이템 11개를 배열의 끝부분에 추가하여 64개 아이템을 가진 배열로 만든다. 지금부
단순히 7은 2의 거듭제곱이라고 가정한다.
마지막 회전의 승리자가 최대키지만 패배자가 꼭 차대키라는 보장은 없다. 그림 8.10
을 보면 차대키(16)는 최대키(18)에 3회전에서 패배한다. 이는 실제 토너먼트에서 가장
All 두 Ho] 항상 결승에서 만나게 되지 않기 때문에 종종 겪게 되는 어려움이기도 하다.

에 VVVY

18
그림 8.10 토너먼트 방법


===== PAGE 366 =====
354

chapter 8 계산복잡도: 검색문제

지난 여러 해 동안 벌어진 미식축구 수퍼볼 경기를 아는 사람들은 이같은 US 잘 알고
1을 것이다. 차대키를 찾기 위해서 최대키에 패배한 키를 모두 기록하고, 알고리즘 8.2
이용하여 그 중에 최대키를 찾을 수 있다. 그러나 어떤 키가 최대키인지 미리 모르는
에서 어떻게 그 키를 기록할 수 있을까? 각 키마다 하나씩 키의 연결 리스트를 유지
된다. 시합에서 패배한 키는 승리한 키의 연결 리스트에 추가한다. 이 방법에 대한
리즘의 작성은 연습문제로 YALE. 만약 no] 29] 거듭제곱이면 1회전에서 7/2번,
2회전에서 (2/2)”번, ... 그리고 결승전에서 (2/2)『\" =1번 비교한다. 모든 회전의 총
비교 횟수는 다음과 같다.

T(n) =n 33(4] =n 0 —1/=n-1

xo
ttlo

om, 때

fh

h

}

ie
=

1

어

KI

뒤에서 두 번째 등식은 부록 AS] 예제 ㅅ.4의 결과를 적용하여 얻는다. 이는 토너먼트 경
기를 하는데 필요한 총 비교 횟수이다(최적의 비교 횟수로 최대키를 찾았음을 명심하라).
최대키는 Ign 시합을 치르고, 이는 연결 리스트에 8 "개 키가 WSS 의미한다. 알고
리즘 8.2를 사용하면 연결 리스트에서 최대키를 찾는데 lg n— 14 비교한다. 그 키가 차
대키이다. 그러므로 차대키를 찾는 총 비교 횟수는 다음과 같다.

T(n)=n—-14+lgn-—1=n+lgn—2
일반적으로 nol] 대해서 다음과 같음을 증명하는 AS 연습문제로 남겨둔다.
T(n) =n+l[lgn|—-2
이 성능은 알고리즘 825 두 번 사용하여 차대키를 찾는 것에 비하면 대단한 개선이

다. 그렇게 하는 경우 22 - 3번 비교했음을 상기해 보라. 이보다 더 적게 비교하면서 차
대키를 구하는 알고리즘은 있을까? 방해꾼 논법을 사용하여 그럴 수 없음을 증명한다.

정리 8.9

비교만으로 가능한 모든 입력에서 개의 키 가운데 차대키를 모두 찾을 수 있는 결정적 알고
BASS 최악의 경우 최소한 다음만큼의 비교를 수행해야 한다.

n+[lg n|-2

증명 : 어떤 키가 차대키임을 결정하기 위해서 최대키를 제외한 7ㅡ1개 7] 중에서 가장 큰
키를 결정해야 한다. ms 최대키가 승리한 비교 횟수라고 하자. 이 비교들은 어떤 것도 차대
키가 남은 7ㅡ1개 키 중에 가장 큰 키임을 결정하는데 유용하지 않다. 정리 8.7에 의하면 이
AAS 하는데 최소 7-ㅇ2번 비교해야 한다. 그러므로 총 비교 APE 최소 7 +ㅜㅠ-2이다. 이
는 정리를 증명하기 위해서 방해꾼은 알고리즘이 최대키를 Be [len] We 비교하도록 하기
만 하면 된다는 뜻이다. 우리의 방해꾼 ASS 트리의 마디를 각 키와 연관짓는 것이다. 처음



===== PAGE 367 =====
@0000000
8.5 선택문제: 방해꾼(적) 논법의 소개     355

a7 Sats

D
무
nif
=
EJ
rok
ol

10

Sgt} S43 비교한

@)
@)
©)
©)

Sst} SoS Hl

©)
(#)

ial
ro

S77} 를 비

ov

El
rok
101
OM OO OM

Sot} s4S 비교한

“Ol
for
Hn)
(*)
)
CH) OO) Of
He) CHE)

66과 를 4

비
rot
for

©

©

과 를 비교한

oh
(0)
He) CHR
($)

그림 8.11 토너먼트 SHS 사용하고 입력의 크기가 8일 때 정리 8.9의 방해꾼이 만든 트리

0

때

에는 각 키마다 하나씩 7개의 단일마디(810816-2ㅁ006) 트리를 만든다. 우리의 방해꾼은 트리
사용하여 8,2} = 비교한 결과를 다음과 같이 내준다.


===== PAGE 368 =====
@0000000
356    chapter 8 계산복잡도: 검색문제

* 5,9} 6,가 모두 마디의 개수가 같은 트리의 뿌리마디이면, 임의의 답을 주면 된다. 트리는
작다고 선언된 키를 다른 키의 자식으로 만들어서 합한다.

© 5,9} 5,7} 모두 트리의 뿌리이고, 한 트리가 다른 트리보다 마디의 개수가 더 많으면,
작은 트리의 뿌리마디는 작게 선언되고, 트리는 그 뿌리마디를 다른 트리의 자식으로 만
들어서 합한다.

* 5,7} 뿌리이고, ,는 아니라면, $,는 작다고 선언되며 트리는 변하지 않는다.

* 5,9} 5,7} 모두 뿌리가 아니면, 답은 이전에 할당된 Ga} 일관성이 있어야 하고, 트리는
변하지 않는다.

그림 8.1은 어떻게 방해꾼이 토너먼트 방법을 사용하고, 입력의 크기가 8일 때 트리를 합하는
지를 보여준다. 선택이 임의적이면 큰 인덱스를 가진 키를 승리키로 한다. 토너먼트가 끝날
때까지의 비교만 보여준다. 그 이후에 최대키에 패배하는 키 중에 가장 큰 키를 찾기 위해서
비교가 더 이루어질 수 있다. 그러나 트리는 변하지 않는다.

size, S 최대키로 승리한 *번째 비교 바로 직후에 그 최대키를 뿌리마디로 가진 트리의 마
디 개수라 하자. 그러면, 다음과 같은 부등식이 성립한다.

size, < 2size,_,

왜냐하면 패배한 키의 트리의 마디 개수는 승리한 트리의 마디 개수보다 클 수가 없다. 초기
조건은 48866 =1이다. 이 회귀방정식을 부록 Bo] 있는 기술을 사용하여 풀면 다음과 같이 결
론 내릴 수 있다:

size, 즈 09

만약 알고리즘이 멈출 때 키가 뿌리마디이면, 그 키는 비교에서 한 번도 패배하지 않았다. 그
러므로 알고리즘이 PRS 때 트리가 두 개 남아 있으면, 두 키는 결코 비교에서 패배하지 않
았다. 최소한 그 키 중 하나는 차대키로 보고되지 않는다. 두 뿌리마디의 WS 바꾸고, 다른
BE 값을 똑같이 하여 새로운 WS 구축할 수 있다. 따라서 둘째로 크다고 보고되지 않을
걸로 우리가 아는 그 키는 실제로 차대키가 된다. 그 입력에 대해서 알고리즘은 틀린 답을 줄
것이다. 그래서 알고리즘이 멈출 때 7개 키는 모두 한 트리에 속해 있어야 한다. 명백히 그
트리의 뿌리마디는 최대키임에 틀림없다. 그러므로 만약 mo] 최대키가 승리한 총 비교 횟수
라면, 다음과 같은 식을 유도할 수 있다.
n= size,, <2”
lgn<m

[lg n| <m

마지막 부등식은 mo] 정수라는 사실에서 유도되었다. 증명이 완료되었다.

토너먼트 방법이 한계치 내의 성능으로 실행되기 때문에 최적이다. 다시 한 번 가치
있는 방해꾼을 찾았다. 어느 다른 방해꾼도 더 좋은 한계치를 만들어 낼 수 없다.



===== PAGE 369 =====
> 알고리즘 8.5

@eeeee? 0
8.5 선택문제: 방해꾼(적) 논법의 소개    357

최악의 경우 최대키를 찾는데 최소 ㅠ-1번 비교하고, 차대키를 찾는데 최소 nt [ign]
- 2번 비교한다. 차대키를 찾는 알고리즘은 반드시 최대키도 또한 찾아야 한다. 왜냐하
면 키가 두 번째로 큰지를 알기 위해서 비교에서 한 번 패배했다는 것을 알아야 한다.
그리고 그 패배는 반드시 최대키에게 당한 것이라야 한다. 그러므로 차대키를 찾는 게
더 어렵다는 것은 놀랄 일이 아니다.

fee)

5.4 ㅅ-번째 작은 키 찾기
일반적으로 선택문제를 풀기 위해서는 *-번째 큰 키나 《-번째 작은 키를 찾을 필요가
있다. 지금까지 최대키 찾는 방법을 공부했다. 왜냐하면 사용하는 용어와 더 적합해 보였
기 때문이다. 즉, 최대키를 승리자라고 부르는 것도 적절해 보인다. 여기서는 알고리즘을
더 명확하게 이해하기 위해서 《-번째 작은 키를 찾는 방법에 대해서 공부해보자. 설명의
편의를 위해서 키는 전부 다르다고 가정한다.

《-번째 작은 키를 O(n 187) 시간 안에 찾는 명백한 방법은 키를 정렬한
AS 넘겨주는 것이다. 우리는 비교를 덜해도 되는 방법을 개발한다.

퀵정렬(알고리즘 2.0)에 썼던 알고리즘 2.7의 partition ZBA|AE Bo} a (pivot
item) HC 작은 키는 모두 배열에서 그 앞에 오고, 피봇아이템보다 큰 키는 모두 그 뒤에
오도록 HSS 분할하였다. 피봇아이템이 위치한 SKS pivotpointe}s 부른다. 피봇아
이템이 《-번째 슬롯에 위치할 때까지 분할하여 선택문제를 풀 수 있다. k7} pivotpoint
보다 작으면, 왼쪽 부분배열을 재귀 호출하여 분할하고(키가 피봇아이템보다 작음), k7}
pivotpoint®ty 크면 오른쪽 부분배열을 재귀 호출하여 분할하여 선택문제를 풀 수
다. k= pivotpoint 이면 찾기를 완료한다. 다음은 이 방법으로 문제를 푸는 분할정복
고리즘이다.

4

4MEH(Selection)

문제 : n7] 다른 키로 된 배열 SoA 《-번째 작은 키를 찾으시오.

입력 k< 7인 양의 정수 nz 《, 1에서 ㅠ까지의 인덱스를 가진 서로 다른 키의 배열 6
출력 : SA) &-번째 작은 키. BH selection®] 값으로 내준다.

keytype selection (index Jow, index high, index k)

{

index pivotpoint ;

if ow == high)
return S{/ow] ;

else {

partition (low, high, pivotpoint) ;
if (k == pivotpoint)


===== PAGE 370 =====
@00@000000
358    chapter 8 계산복잡도: 검색문제

return S{pivotpoint] ;
else if (kA < pivotpoint)
return selection(low, pivotpoint—1, &) ;
else
return selection(pivotpoint + 1, high, k) ;
}

}

void partition (index Jow, index high,         // 알고리즘 2.79 프로시저와 같다
index& pivotpoint)
{

index 2, /;
keytype pivotitem ;

pivotitem = S{low] ;                    // pivotitem2= 첫 번째 아이템을 선택
7 = 700;
for (7 = Jow+ 1; i <= high, 4++)
if (9121 < pivotitem) {
J++;
이기와 Sj] 교환;
}
pivotpoint = J;
Sllow|2} S[pivotpoint| 교환:              // pivotpoint pivotitem& 넣음

이전 장의 재귀 함수와 마찬가지로 과 St BF selection? 입력이 아니다. 그 함수

kthsmallest = selection(1, n, k)

정렬(알고리즘 2.0)과 같이 각 재귀 SS 시 분할한 배열의 크기가 하나 작으면 최악의
우가 된다. 예를 들어 배열이 오름차순으로 정렬되어 있고 *=7《인 경우에 이같은 상
황이 일어난다. 알고리즘 8.5는 따라서 알고리즘 2.6과 같은 최악의 경우 시간복잡도를
가진다. 이는 알고리즘 8.5의 키의 비교 횟수 기준 최악 시간복잡도는 다음과 같음을 의

미한다.
비록 최악의 경우가 퀵정렬과 같지만, 다음 Bato] 경우 알고리즘 8.5는 훨씬 성능이
우수하다.



===== PAGE 371 =====
@06@00000 0
8.5 선택문제: 방해꾼(적) 논법의 소개 359

입력크기 : n, 배열에서 아이템의 개수
입력들은 모두 발생확률이 같다고 가정한다. 이는 모든 Kk He 같은 빈도수로 들어가고
는 pivotpoint 값은 같은 빈도수로 넘겨진다. p= pivotpointS 나타낸다고 하자. 재
귀 호출이 없는 경우(즉, = 1, 2, .… 7일 때 2 = 《*인 경우) 결과가 개 존재한다. 첫째
재귀 SSA] 입력크기가 1인 경우(즉, 4=1이며 p= 2이거나, k= n°] 2 = 7 -ㅡ이
면) 결과가 2개 존재한다. 첫째 재귀 SSA 입력크기가 2인 경우(즉, 4 = 1 또는 이며
2=8이거나 k=n-1 또는 이며 2= ㅠ-2이면) 결과가 3(2) = 4개 존재한다. 아래
에 모든 입력크기에 대한 결과의 개수를 나열하였다.

첫째 재귀 SSA     주어진 크기를
임의       산출하는 결과의 개수
0                    n
1                    2
2                  2(2)
3                  2(3)
i                   2(i)

각 입력크기에 대해서 《의 같은 같은 빈도수로 나타나리라는 AS 그리 어렵지 않게 알
수 있다. partition BBX AYA 비교 횟수는 ㅠ- 1임을 알고리즘 2,79] 평균의 경우를
석해보고 알았다. 따라서 평균은 다음 재현방정식으로 구할 수 있다.

10

nA(0)+2[A(1)+2A(2)+-+7A (i) +--+ (n—-1)A(n—-1)]
n+2(1+24--+i+--+n-1)

부록 AS] 예제 ㅅ.1의 결과와 4(0) = 0이라는 사실을 사용하여 정리하면 다음 식을 얻

5

A(n)=                                              +n-1

100 A ee Bere tid eer nie Ae Adel

다음에 알고리즘 2.6(퀵정렬)의 평균 시간복잡도 분석에서 사용된 기술을 그대로 써 본다.

즉, 양변을 7으로 곱하고, n-1S 적용한 다음 A(n-1)9] 표현식을 41 0/)으로부터 wh
고, 정리하면 다음과 같이 된다
2_          -_    =
n             n
< A(n—-1)+3

4(0) = 0이므로, 다음 재현방정식을 얻는다.


===== PAGE 372 =====
360

chapter 8 계산복잡도: 검색문제

부록 BS] 8.1절에 설명한대로, 이 재현방정식은 수학적 귀납법으로 해를 구할 수 있다. 해
는 다음과 같다.
A(n) < 302

방법으로 재현방정식을 사용하여 A (n)o] 선형함수의 시간복잡도를 가짐을 보일 수

4(0)의 재현방정식을 가지고 큰 7 Soll 대해서 다음 식이 성립함을 Sys
하다.

에
대

으
것은 간단

A(n)=3n

평균적으로 알고리즘 8.5(선택)는 1차함수 개수의 비교만 수행한다. 물론 알고리
2.6(퀵정렬)보다 평균적으로 성능이 더 좋은 이유는 AVA partitions 두 번 호출하
는데 비해서 이 알고리즘은 한 번만 호출한다. 그러나 재귀 호출의 입력이 7-1이면 둘
다 같은 복잡도로 퇴보해 버니 경우 퀵정렬에서는 한쪽에 빈 부분배열이 입력된다).
그 시간복잡도는 2차함수가 된다. 알고리즘 8.5에 이러한 일이 일어나지 않게 하려면,
최악의 경우 2차함수 시간을 개선할 수 있어야 한다. 다음에 이를 어떻게 하는지 공부해
보자.

gee 배열을 정확하게 반으로 나누면, 각 재귀 호출마다 입력이 반으로 잘리

므로 최상의 경우가 된다. 7개의 서로 다른 키의 미디안0ㅁ6082/)은 키 중에서 반은 그보
다 작고, 반은 그보다 큰 키를 가리킨다는 사실을 공부했다(이 사실은 이 홀수인 경우에
만 정확히 적용된다). 만약 항상 미디안을 270087702으로 선택할 수 있으면, 성능이 최
적일 것이다. 하지만 미디안은 어떻게 구하나? 28470002 프로시저에서 66/80002 함수
를 원래 배열로 된 입력과 그 입력의 반 정도 크기인 《*를 가지고 호출해 볼 수 있다. 바로
밝혔듯이 이는 제대로 작동하지 않을 것이다. 왜냐하면 원래 입력과 같은 크기의 입력을
가지고 계속 selections 호출해버리게 되기 때문이다. 그러나 다음과 같은 책략을 쓰면
SOURS 것이다. 잠시동안 no] 52] 홀수 배라고 가정하자(5를 쓸 필요는 없다; 이 A
끝부분에서 다시 다룬다). 개 키를 7/5개 그룹으로 나누는데 각 그룹은 5개씩 키를 가
지고 있다. 각 그룹별로 미디안을 직접 구한다. 연습문제에서 물어보겠지만, 구하는데
6번의 비교가 필요하다. 그리고 selection YES 호출하여 n/5 74 미디안의 미디안을 구
한다. 이 미디안들의 미디안이 개 키들의 미디안일 BRE 없지만, 그림 8.12에서 보듯
이 상당히 가깝다. 그 그림에서는 가장 작은 미디안의 왼쪽에 있는 키들(2와 9)은 미디안

=



===== PAGE 373 =====
> 알고리즘 8.6

@‥ㅎ00000 0
8.5 선택문제: 방해꾼(적) 논법의 소개 361

미디안                미디안                미디안

2 3<5 <8 12  1 7 <<10<=13 80 6 14<15<18 22
Vv
5 “<= 10) <=15

미디안 중 미디안

그림 8.12 색으로 표시된 키가 미디안 중 미디안보다 작은지 큰지 알 수 없는 사례

들의 미디안보다 작아야 하고, 가장 = 미디안의 오른쪽에 있는 키들08와 29)은 미디안
들의 미디안보다 커야 한다. 일반적으로 가장 작은 미디안의 오른쪽에 있는 키들(8와 12)
과 가장 큰 미디안의 왼쪽에 있는 키들(6와 140은 미디안들의 미디안의 어느 쪽에도 올
수 있다. 미디안들의 미디안의 어느 쪽에도 올 수 있는 키의 ASE 다음과 같음을 주목
하자.
15
| 2 - 7

nO] 5의 홀수 배가 될 때마다 미디안들의 미디안 어느 쪽에도 S 수 있는 키의 개수는
다음과 같다는 것을 아는 것은 별로 어렵지 않다.

한쪽에 있는지
아는 키의 개수

이 전략을 사용하는 알고리즘을 분석할 때 이 결과를 다시 살펴본다. 먼저 알고리즘을
보자.

21 양의 정수 /과 k, 1에서 7까지의 인텍스를 가진 서로 다른 키의 배열 s
출력 : SoA] &-번째 작은 키. 함수 96/890402의 값으로 넘겨진다.


===== PAGE 374 =====
@00@000000
362    chapter 8 계산복잡도: 검색문제

keytype select (int n,

keytype 5{],
index 4)

{
}

return selection? (S, 1, n, k);

keytype selection? (keytype 이],
index /ow, index high, index 4)
{

if (high == low)
return S{/ow] ;
else {
partition? (S, low, high, pivotpoint) ;
if (k == pivotpoint)
return S{pivotpoint ;
else if (k < pivotpoint)
return selectionA.S, low, pivotpoint—1, &) ;
else
return selectionAS, pivotpoint +1, high, k) ;
}

}

void partition? (keytype Sf],
index /ow, index high,
index& pivotpoint)

const arraysize = high — low +1;
const r = |arraysize / 5] ;
index i, ./, mark, first, last;
keytype pivotitem, T[1..z] ;

for (§ = 1; 7 <= ry H+) {
first = low + 5*i - 5;
Jast = minimum(low + 5*i — 1, arraysize) ;
717] = median of S{firs¢] through S{last¢] ;
}
pivotitem = select(r, T, |(r+1)/2];           // Woes 근사적으로 구한다.
J = low;
for (7 = low+ 1; i <= high; ++)
if (S[ i] < pivotitem) {

이기와 S[j] 교환;
mark = J;                          // pivotitem& 위치시킬 장소에 표시
I++ 5

}

else if (S{7] < pivotitem) {
이 기와 Sl 7] 교환;



===== PAGE 375 =====
85 선택문제: 방해꾼(적) 논법의 소개     363
Lr
}
pivotpoint = j — 1;
S{mark|2} S[pivotpoint] 교환;              // pivotpoint%) pivotitem& 넣음

}

알고리즘 8.0에서 다른 재귀 알고리즘과는 달리 재귀 함수를 호출하는 함수는 간단하
다. 이유는 이 간단한 함수가 다른 입력으로 다른 장소에서 호출될 필요가 있기 때문이
다. 즉, partition? 프로시저에서 7'입력으로 호출되고, 전역적으로(60081) 다음과 같
이 호출된다.

kthsmallest = select(n, S, k)
또한 재귀 함수 selection2 그 배열을 입력으로 넣는데, 그 이유는 그 함수는 전역 배열

SHAS 배열 TS 동시에 처리하도록 호출되기 때문이다.
다음에는 이 알고리즘을 분석한다.

. 8  *(미디안을 사용한 선택)의 최악 시간복잡도 분석

연산 : /2477220222에서 Sli] 와 /20077*022의 비교

입력크기 : n, 배열에서 아이템의 개수

간단히 하기 위해서 no] 5의 홀수 배라고 가정하고 재현방정식을 만든다. 재현방정식은
일반적인 nol] 대해서 근사적으로 성립한다. 재현방정식을 이루는 구성요소는 다음과 같다.

(pa
do

@ selection? 함수가 호출할 때 selection? 함수의 시간. 이미 토의한 대로 no] 52] 홀수
배라면 pivotpoint?| 한쪽으로 갈 키의 개수는 최대한 다음과 같다.

Tn 3

10 2

이 값은 selection? 호출의 입력에서 최악의 경우 키의 개수를 의미한다.

© partition? 프로시저가 호출할 때 selection? 함수의 시간. selection? 호출의 입력에
서 최악의 경우 키의 개수는 7/5이다.

* 미디안을 찾는데 필요한 비교 횟수. 이미 언급했듯이 5개 숫자의 미디안은 6번 비교하
of 찾을 수 있다. 7이 52] 배수일 때 알고리즘은 5개의 숫자를 가진 정확히 7/5개
그룹의 미디안을 찾는다. 따라서 미디안을 찾는데 필요한 총 비교 횟수는 60/5이다.

* 배열을 분할하는데 필요한 비교 횟수는 7이다(비교의 구현이 효율적으로 이루어졌다
고 가정).
다음 재현방정식을 확립했다.

2178 으  n)\, 6n
Wn) = W (2 34 w(2}+ an


===== PAGE 376 =====
364

chapter 8 계산복잡도: 검색문제

이 5의 배수가 아닐 때도 위의 근사 등식이 성립함을 보이는 것이 가능하다. 물론, Wn)
은 실제로 정수가 아닌 입력을 가지지는 않지만, 그러한 WAS 고려하면 분석이 간단해
진다. 이 재현방정식을 보면 귀납법을 사용할 수 있는지의 여부를 전혀 알 수 없다. 더구나
부록 BoA] 배운 어떤 기술을 가지고도 풀 수 없다. 그러나 AAW (constructive in—
duction) °]2} 하는 기술을 사용하여 귀납법에서 사용될 수 있는 후보해답을 구할 수 있다.
즉, Wn) 선형임을 알고 있으므로 7 < 7인 모든 mi 어떤 상수 co] 대해서 Wim)
< 07이라고 가정하자. 그러면 재현방정식은 다음 식으로 유도된다.

Tn   n  lin  702  72 , 1102
=  —   —|+ — < e— 4+ e+ + =
W(n) w (+ 씨프 5 SG oe e

Wn) < 07으로 결론짓고 싶으므로, 귀납법으로 작동되는 < HS 결정하려면 다음 부등

식을 풀어야 한다.
Tn 72 Lln
—— ee 은
eT 아티 5 = 002
그 해는 다음과 같다.
22 즈 6

그러면 이 부등식을 만족하는 ㅇ의 가장 작은 값을 선택하고, 형식적인 귀납논법으로 진행
하여 no] 작지 않을 때 최악 시간복잡도는 대략 다음과 같은 범위를 가진다.

W(n) < 22n
명백히 이 부등식은 7 < 5 에 대해서 성립한다. 귀납논법을 마저 끝내는 AS 연습문제로
남겨둔다. 정리 8.7에 의하면 *=1인 경우에 해를 구하기 위해서만도 1차시간이 필요하
다. 따라서 다음과 같이 결론짓는다.

최악의 경우 1차시간에 실행되는 알고리즘으로 선택문제를 성공적으로 해결했다. 앞
에서 언급했듯이 이를 위해서 AS 크기가 5인 그룹으로 나눌 필요는 없었다. 만약 m
이 그 그룹의 크기라면, m > 5인 어떤 홀수 값을 택해도 선형시간의 복잡도 결과를 얻
는다. 이제 그 이유를 알아보자. 언급한 결과를 얻는 절차는 연습문제로 남겨둔다. 임의
의 에 대하여 최악 시간복잡도를 구하기 위한 재현방정식은 다음과 같다.

(3m—1)n

=    J+ 떠픔+ an                  (8,2)

Wn) =  wv|



===== PAGE 377 =====
@0000000
85 선택문제: 방해꾼(적) 논법의 A

N
=
wo
22
27

여기서 axe 양의 상수이다. 우변에서 의 계수의 합은 다음과 같다.

9001 , 1 - 3770 10

4m          m          4m

.2는 우변이 1보다 작다는 사실은 m > 3이라는 사실의 필요충분조건이 된
간단히 알 수 있다. 다음 재현방정식이 p+ 0 < 1이면 1차방정식을 나타냄을
은 가능하다.

rir rat
o%
ox,
~
CO

W(n) = W(pn)+ W(qn)+an
따라서 재현방정식 8.2는 m > 59] 모든 mol 대한 1차방정식이다.
m=3% 때, 재현방정식 8.2는 다음과 같이 된다.

58
귀납법을 사용하면 이 재현방정식의 BE 다음과 같음을 증명할 수 있다.
W(n)EQ(nlg 72)

그러므로 1차시간의 성능을 갖게 해주는 가장 작은 7의 홀수이다.
m=T7, 9, 119 때 시간복잡도의 상한 cE 71 =5일 때보다 약간 작다. ㅇ의 값은 mo]
11 넘어 증가하면 매우 서서히 증가한다. mo] 작지 않다면, cE 대략 418 mo] 됨을 보
일 수 있다. 예를 들어, 7=100이면, 그 상수는 대략 418 100 = 26.6이 된다.
여기의 선택문제의 선형시간 알고리즘은 Blum—Floyd—Pratt—Rivest—Tarjan(1973) ©]
개발하였다. 원본은 더 복잡하지만 키의 비교 횟수는 5.57 정도밖에 ot 된다.
Hyafil(1976)-2 k > 1일 때 7개 키의 집합에서 *-번째 작은 키를 찾는 하한은 다음과
같음을 증명했다.

n+(k—-1) [피근기] —k

이 SB Horowitz—Sahni 2] 책(1978)에도 나와 있다. 정리 8.9는 이 결과의 특별한 경우
임을 주목하자.

다른 선택 알고리즘과 하한은 Schonhage—Paterson—Pippenger(1976)} Fussenegger
-0860\0970)에서 찾아볼 수 있다.

8.5.5 선택문제에 대한 확률적 알고리즘

알고리즘의 하한을 구할 때 그 알고리즘이 결정적(406600401640이라고 가정해왔다. 그
러나 그 하한이 확률적 알고리즘에도 성립한다는 것도 언급했다. 이러한 알고리즘이 언
제 유용한지를 설명해주는 선택문제의 확률적 알고리즘을 보여줌으로서 이에 대한 토의


===== PAGE 378 =====
366

chapter 8 계산복잡도 : 검색문제

를 마무리 짓도록 한다.

5.3절에서 재귀 알고리즘의 Bo] 대한 근사치를 구하는 몬테칼로 알고리즘이라고
하는 FEA 알고리즘을 공부했다. 몬테칼로 알고리즘이 반드시 맞는 답을 지는 않는
다. 오히려 그 답의 추정치를 제공하고, 그 추정치가 맞는 답에 가까울 확률은 알고리즘
의 사용 시간이 증가할수록 커진다. 여기서는 셔우드 알고리즘이라고 하는 다른 종     류의
확률적 알고리즘을 살펴보자.

APE 512) Z(sherwood algorithm) 항상 맞는 FS 준다. 이 알고리즘은 최악의
경우보다는 평균의 경우 훨씬 빠르게 실행되는 결정적 알고리즘에 적합하게 쓰인다. 알
고리즘 8.5(선택)의 경우 이게 사실로 들어났다. 그 알고리즘에서는 특정 입력에 대한 기
준점(01*06[00104이 재귀 호출에서 low} high] 계속 가깝게 나올 때 최악의 경우 2차시
간이 되었다. 예를 들어, 배열이 오름차순으로 정렬되어 있고 *=7인 경우가 그렇게 된
다. 대부분 입력은 그렇지 않으므로 알고리즘의 평균 Wee 1차시간이다. 특정 입력에
대해서 균등분포(40101 distribution) oj] 따라서 ana 기조 아이템을 선정한다고 가
정하자. 그러면 그 입력으로 알고리즘을 수행할 때 기준점은 끝점에 가까워지기보다는
멀어질 확률이 더 높다(무작위성은 부록 AS] A BAMA 시  그러므로 성능이
1차시간일 확률이 더 높다. 모든 입력에 평균적으로 적용하면 비교 횟수는 1차가 되기
때문에 균등분포에 따라서 무작위로 기준 아이템을 선정하면 특정 입력에 대해서 수행하
는 키의 비교 횟수에 대한 7] ql (expected ?8106)는 직관적으로 1차가 됨이 틀림없다.
이게 사실임을 증명하기 전, 우선 알고리즘 8.5에서 구한 기대치와 평균치의 차이점을
먼저 생각해보자. 입력의 크기가 모두 같다고 가정하면 알고리즘 8.5의 평균 비교 횟수는
1차이다. 입력에 따라 알고리즘 8.5의 비교 횟수는 변하지는 않는다. 어떤 입력에 대해서
는 2차가 되기도 한다. 우리가 이제 보여주려고 하는 APE 알고리즘은 실행할 때마다
비교 횟수가 같지 않다. 때로는 비교 횟수가 1차가 되기도 하고, 때로는 2차가 되기도
한다. 그러나 만약 알고리즘을 같은 입력으로 여러 번 수행한다면 평균 수행시간은 1차가
된다고 기대할 수 있다.

알고리즘 8.6(미디안을 사용한 선택)의 성능이 1차임이 보장되는데 왜 이런 알고리즘
을 사용하고 싶어 하는지에 대해서 의아해할 지도 모른다. 이유는 알고리즘 8.6은 메디안
의 근사치를 구하는데 필요한 상수 추가비용 값이 크기 때문이다. 셔우드 알고리즘이 알
고리즘 8.6보다 평균적으로 더 빨리 실행된다. 알고리즘 8.6을 쓸 건지 셔우드 owe
을 쓸 건지에 대한 age ny 사용하느냐에 따라 달라진다. 평균적으로 성능이 우수
해야 한                            한다. 반면에 성능이 2차가 되면 절대 et 되는 경우
에는 = … 한다 셔우드 알고리즘이 알고리즘 8.5(선택)보다 우수하다는
AS 다시 한 번 강조한다. 입력이 균등분포이면 알고리즘 8.5도 알고리즘 8.6보다 평균
적으로는 성능이 좋다. 그러나 어떤 응용 분야에 따라서 알고리즘 8.5의 최악의 경우와
항상 근접하게 되는 경우도 있다. 그런 경우 알고리즘 8.5는 실행 성능이 항상 2차가 된



===== PAGE 379 =====
85 선택문

제: 방해꾼(적) 논

다. 셔우드 알고리즘은 균등분포에서 무작위로 피봇아이템을 선정하여 이 단점을 극복할

A 수 있다
이제 확률적(셔우드) 알고리즘을 살펴보자.

> 알고리즘 8.7     확률적 MEH(Probabilistic Selection)
문제 : /개 다른 키로 된 배열 에서 *-번째 작은 키를 찾으시오.
입력 : k <n 양의 정수 nF k, 1에서 7까지의 인덱스를 가진 서로 다른 키의 배열 6
출력 : SoA) &-번째 작은 키. 함수 selection32] 값으로 내준다.

keytype selection3 (index 700, index high, index k)
{
if (low == high)
return S{/ow] ;
else {
partition3 (low, high, pivotpoint) ;
if (k == pivotpoint)
return S{pivotpoint| ;
else if (k < pivotpoint)
return selection3 (low, pivotpoint—1, k) ;
else
return selection3 (pivotpoint + 1, high, k);
}

}

void partition3 (index Jow, index high,
index& pivotpoint)
{

index 27, j, randspot ;
keytype pivotitem ;

randspot = random index between Jow and high inclusive ;

pivotitem = S{randpot| ;                      // ¥449= pivotitem= 선정

J = low;
for (7 = low + 1; i <= high; i++)
if (S[ i] < pivotitem) {
rH
이 기와 Sl 7] 교환;
}

pivotpoint = /;

Sllow\2} S{pivotpoint] 교환;                  // pivotpoint©| pivotitem& 넣음

알고리즘 8,72 피봇아이템을 무작위로 선정한다는

것만 알고리즘 8.5와 다르다. 다음


===== PAGE 380 =====
0000000
368   chapter 8 계산복잡도: 검색문제

에는 비교 횟수의 기대치가 어떤 입력에 대해서도 1차임을 증명한다. 이 BAS 알고리즘
8.5(선택)의 평균의 경우 분석과 분명히 다르다. 왜냐하면, 그 분석에서는 모든 《값이 같
은 빈도로 들어온다고 가정했기 때문이다. 각 입력에 대해서 1차시간 기대치를 얻고 싶
다. 각 입력은 나름대로의 《값을 가지고 있기 때문에 모든 《값이 같은 WES 나타난다
고 가정할 수 없다. 이제 *값과는 독립적으로 기대치가 1차임을 보인다.

ㅣ > (확율적 선택)의 기대치 시간복잡도 분석

단위연산 : 247770202에서 ,912]와 pivotitem2| 비교

입력크기 : n, 배열에서 아이템의 개수

입력의 크기가 7일 때 &-번째 작은 키를 찾는 경우 YA] 크기와 각 pivotpoint 값에
대한 첫째 재귀 SSA] 새로운 *의 값은 다음 표에서 보여준다.

pivotpoint      입력크기     새로운 《의 값
it             all            kl
2             ime?            b= 2
hl         n—(k-1)           i
k               0
ete          k
2            1
n          mn 그          k

pivotpoint 값들은 모두 발생확률이 같으므로, 기대치에 대한 재현방정식은 다음과 같다.

1

k-1          n-1
E(n, k)=—| >] E(n—p, k-p)+ >) Ep, k)}+n-1
p=k

p=1
이 재현방정식은 알고리즘 8,69] 최악의 경우 분석과 마찬가지로 건설재귀를 사용하여 분
석할 수 있다. 즉, 이 재현방정식이 1차인지가 의심스럽기 때문에 귀납논법으로 H(n, 《)
= nS 증명할 수 있도록 <값을 찾는다. 그러나 c= 4가 제대로 작동하는 최소 상수임
을 어떻게 결정하는지는 연습문제로 남겨두고, ㅇ= 4로 놓고 귀납법으로 증명한다.

귀납기초 : = 1인 경우 비교는 이루어지지 않으므로

201, k)=0 < 4(1)
귀납가정 : m < 7인 BE mab k = ml BE 《에 대해서 다음 부등식이 성립한다고 가
정한다.



===== PAGE 381 =====
연습문제     369
E(m, k) < 4m
귀납단계 : kK< nel 모든 ko] 대해서 다음 부등식이 성립함을 증명한다.
E(n, k) < 4n
재현방정식과 귀납가정에 의하여 다음 부등식을 얻는다.
1  ea          tf emt!
E(n, k) < —  21 Aln—p)+ 54 dp] +n—1              (8,3)
n p=l1       p=k

그러면 우변의 일부는 다음과 같이 전개한다.

k-1      n-1    fk—-1  k-1  n-1
YAn~p)+ 21 =4] Yin— Yiv+ Sp
p=1      p=k    lp=1 2=1  p=k
[       k= 1  n-1
=4 (k—-1)n—2 ¥} pt S|
L         p=1   p=1

=4[(k-1)n == Det Bou)

= 4 1)(n—k) + ae 3

< 4|k(n— K+ 2] < 4[ +5 | =n"

위에서 셋째 등식은 부록 AS] 예제 ㅅ&.1의 결과를 두 번 적용하여 얻은 결과이다. 마지막
부등식은 일반적으로 k(n—k) < 7”라는 사실로부터 끌어냈다. 방금 얻은 결과를 위의
부등식 8 30] 끼워 넣으면 다음과 같은 BEALS 얻는다.

E(n, k)< = (3n?) +n— 1=3nt+n-1<4n

k2] 값에 상관없이 다음이 AAAS 증명했다.
E(n, k) < 470 (02)

@ 연습문제

8.1절
1. 순차검색 알고리즘(알고리즘 1.1)을 사용할 때 검색이 리스트의 첫부분에서 시작하지 않고,
이전 검색이 끝부분에서 시작한다고 가정해보자. 그리고 검색하는 아이템을 이전 검색의 종
착지와는 관계없이 무작위로 선택한다고 또한 가정해보자. 이 가정 하에서 평균 비교 횟수
는 얼마가 될까?


===== PAGE 382 =====
@00@000000
370    chapter 8 계산복잡도 : 검색문제

2. SO TS 각각 개와 7개의 아이템으로 구성된 배열이라고 하자. 공통 아이템을 모두 찾
아서 배열 《에 저장하는 알                     작업이 O(n+m) 시간 안에
수행될 수 있음을 증명하시오

3. 검색이 성공한다고 가정하고 이분검색 알고리즘(알고리즘 1.5/을 개선하시오. 개선한 알고
리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

4. 만약 가 배열 안에 있고 각 배열 슬롯에 있을 확률이 같다고 할 때 이분검색(알고리즘 1.5)
에 대한 평균 시간복잡도는 대략 다음의 범위를 가진다.

lign|]—1< A(n) <|lgn}

HE: RAVE] 8.4에 의하여 어떤 《에 대하여 n—(2*—1) & 바닥수준(60560ㅁ level) ol] 있
는 마디의 개수이다. 이 마디들의 77022에 대한 기여는 (2 -2"-1)(&+1) 과 같다. 이 식에
다가 (ㅎ-1)2*“+1(이분검색의 평균의 경우 분석에서 얻은 식임)를 더하여 그 결정트리에
대한 TNDS 구하시오.

5. 다음의 21+1가지 가능성이 모두 발생확률이 같다고 가정하면,

1<i<nl 어떤 io] 대해서      r= 8;
r< 8,
1<i<n—-19] 어떤 io] 대해서   워스 이시이
LS Ss
이분검색 알고리즘(알고리즘 15) 평균 시간복잡도는 대략 다음 범위임을 증명하시오

lisn]-4< A(n) <LignJ+3

AE: 연습문제 4에 대한 ABS 보시오.
6. 보조정리 8.6에 대한 증명을 완성하시오.

7. 이분검색, 보간검색, 보강된 보간검색 알고리즘을 구현하고, 여러 가지 문제 사례를 사용하
평균의 경우, 최악의 경우 성능을 각각 학습하시오.

을 확률이 모두 같다고 가정하

우
9. 키는 균등하게 분포되어 있고 검색키 7가 각 배열 슬롯에 있을 확률이 모두 같다고 가정하
고, 보간검색의 평균 시간복잡도가 0((187)”)임을 증명하시오
8.3절

10. 이진검색트리에서 최대키를 찾는 알고리즘을 작성하시오. 그 알고리즘을 분석하고, 그 결과
를 차수 표기법으로 나타내시오.

11. 정리 8.8에 의하면 성공적인 검색의 경우 이진검색트리를  리너 개 키를 가진 모든 입
력에 대한 평균 검색시간은 6(187)이다. 검색이 실패한 경우에도 이 결과가 그대로 성립함



===== PAGE 383 =====
12. 가능한 모든 경우를 고려하여 이진점색트리에서 마디를 하나 제거하는 알고리즘을 작성하
시오. 그 알고리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

13, 키의 리스트를 3-2 트리로 만드는 알고리즘을 직            알고리즘을 분석하고, 그 결
과를 차수 표기법으로 나타내시오.

14. 자연스런 순서로 8-3 트리의 키를 모두 나열하는 알고리즘을
분석하고, 그 결과를 차수 표기법으로 나타내시오.

8.4절

15. SSS 방지하는 또 다른 하나의 방법은 선형탐사010087 probing)o]t}, 이 전략을 사용하면
아이템을 모두 바구니(해시 테이블)의 배열에 저장한다. SSO] 발생하면 테이블에서 다음
가용한(쓸 수 있는) 바구니를 찾는다. 선형탐사를 사용하여 그림 8.8의 문제 사례에서 발생
한 SES 어떻게 해결하는지 보이시오. 선형탐사는 닫힌해시(00860 hashing) #}il&= 한다.

16. 두 개의 충돌해결전략, 열린해시와 선형탐사(연습문제 15S 보시오)의 장점과 단점을 토의
하시오.

17. 선형탐사를 충돌해결전략으로 사용하는 해시테이블에서 아이템을 제거하는 알고리즘을 작
성하시오. 그 알고리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

18. 이중해시(004016 hashing) = 알려져 있는 재해시 AAl(rehashing 801606)는 충돌이 발생하
면 둘째 해시함수를 사용한다. 만약 첫째 해시함수가 /;이고, 둘째 해시함수가 라면 가용한
바구니를 검사하게 될 해시테이블의 위치 순서는 다음 식으로 결정한다.

p, (key) = [(h(key) +i x s(key) -1)% 1846 61201 +1
여기서 p= 이 순서에서 :번째 HAS 나타낸다(%는 첫째 배려 둘째 피연산자로 나

= 때 나머지를 내준다). 그림 8.8의 문제 사례에 대한 둘째 해시함수를 정의하고, 키가 모두
해시테이블에 삽입된 후의 테이블을 보이시오.

fu

알고리즘을

fl

8.5m
19. 알고리즘 8.4(키를 짝 지워서 최소키와 최대키 찾기)를 n(FOlZl 배열에서 키의 수)이 홀수
일 때 제대로 작동하도록 수정하고, 그 시간복잡도가 다음과 같음을 증명하시오

no] 짝수이면,        Say
no] 홀수이면,        aS

20, 정리 8.8의 S98 완성하시오, 4, 비교만으로 가능한 모든 입력에서 *개의 키 가운데 최
소키와 최대키를 모두 찾을 수 있는 결정적             칙악의 경우 no] 홀수이면 반드시
최소 (37-3)/9번의 비교를 수행한다.

21. 8.5.3절에서 공부한 주어진 배열에서 차대키를 찾는 방법을 알고리즘으로 작성하시오.
22. 8.5.3절에서 공부한 주어진 배열에서 차대키를 찾는 방법에 필요한 총 비교 횟수는 일반적



===== PAGE 384 =====
372

chapter 8 계산복잡도: 검색문제

으로 no} 대해서 다음과 같이 됨을 증명하시오.
T(n) =7+|11871-2

23. 5개 수의 미디안은 owl 비교하여 찾을 수 있음을 증명하시오.

24. 귀납법을 사용하여 알고리즘 8.6(미디안을 사용한 선택)의 최악 시간복잡도의 범위는 대략
다음과 같음을 증명하시오.

W(n) < 22n
25. 임의의 m(1H] 크기)에 대해서 알고리즘 8.6(미디안을 사용한 선택)의 최악 시간복잡도
에 대한 재현방정식은 0가 상수일 때 다음과 같음을 증명하시오.

(3m—1)n
4

W(n) ~ w|

te w(2)+ an
이 식은 8.5.4절의 재현방정식 8.2이다.
26. 귀납법을 사용하여 다음 재현방정식에 대해서 Wn) Q(nlg n) 7} 됨을 증명하시오. 이 식
은 \(그룹의 크기)이 3일 때 8.5.4절의 재현방정식 8.8이다.
2n

W(n) = w{2)+ w(2}+2

27. 알고리즘 8.7(확률적 선택)의 기대치 시간복잡도 분석에서 얻은 다음 부등식에서 상수 cE

4보다 작을 수 없음을 증명하시오.
E(n, k) < en

28. 알고리즘 8.5, 8.6, 8.7(배열에서 &-번째 작은 키를 찾는 선택 알고리즘)을 구현하고, 여러
가지 문제 사례를 사용하여 최선의 경우, 평균의 경우, 최악의 경우 성능을 학습하시오.

29. 7개의 아이템으로 구성된 배열이 대다수아이템(가장 많이 나타나는 아이템)이 있는지 결정
하는 확률적 알고리즘을 작성하시오. 그 알고리즘을 분석하고, 그 결과를 차수 표기법으로
나타내시오.

주가 문제

30. 아주 큰 정렬된 리스트가 외부 저장장소에 저장되어 있다고 하자. 그 YASS 내부 메모리
로 불러올 수 없다고 가정하고, 이 리스트에서 어떤 키를 찾는 검색 알고리즘을 개발하시오.
외부 검색 알고리즘을 개발할 때 무슨 요소들을 주로 고려해야 하는가? 주요 요소(들)를 정
의하고, 그 알고리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

31. 다음의 각 트리구조를 다른 트리구조를 사용하는 경우와 비교해서 AAS 토의하시오.
(8) 균형 맞추는 장치를 갖춘 이진검색트리
060) 83-2 트리

32. 해시 사용이 적절치 못한 경우의 실례를 두 가지 이상 작성하시오.

33. 와 TS 이미 비내림차순으로 정렬된 7개의 수를 가진 두 개의 배열이라고 하자. 27;개의
수 미디안을 찾으며, 시간복잡성이 ㅇ(187)인 알고리즘을 작성하시오.

34. 함수 primey} factorS 사용하여 정수의 약수(68000)를 구하는 확률적 알고리즘을 작성하



===== PAGE 385 =====
35.
36.

@0000000
연습문제 373

시오. 함수 primee 주어진 정수가 소수이면 “ㅠ06`를 넘겨주고, 그렇지 않으면 Dacia
넘겨준다. E> factore 주어진 합성수(600ㅁ00816 integer, 2427} 아닌 수)의 약수를 넘겨
준다. 그 알고리즘을 분석하고, 그 결과를 차수 표기법으로 나타내시오.

이 장에서 학습한 모든 검색 알고리즘의 장ㆍ단점을 열거하시오.

이 장에서 학습한 각 검색 알고리즘을 보고, 그 알고리즘이 가장 적절하게 쓰일 수 있는 실
례를 두 개 이상 작성하시오.


===== PAGE 386 =====
계

산복잡도와 다루기

으
빠른 알고리 ze 찾지 못했습니다. 하지만
저만 찾지 못한 게 아니라, oral 찾은
사람이 아무도 없습니다.

= 정도 : NP 이론의 소개

2|(Garey) 2+ 존슨(00008020)의 책(1979)에서 따온 이야기이다. AES 소프트웨
개   어 개발 회사에 다니고 있다. 어느 날 상관이 당면한 중요한 문제를 효율적으로
풀 수 있는 알고리즘을 개발하는 프로젝트를 할당해주었다. 한 달 이상 그 East 밤낮으
도 pei no aa rina 찾을 기미가 전혀 보이지 않는다. 포기하고 상관에

=                게 Hn eal 알고리즘을 we   원전적으로 불가능할 지도
모르니 시간을 더 달라고 상관을 설득한다. 상관은 마지못해 그게 맞는지 밝혀내는데 한
달의 시간을 더 준다. 이를 증명하려고 또 한 달을 밤샘으로 보내지만 혔수고이다. 이
율적인 알고리즘을 찾지도 못했고, 효율적인 알고리즘을 만드는 작업

이 원천적으로 wigan 중명하지도 못했다. 마감시간이 임박해서야 외판원 문제를
푸는 효율적인 알고리즘을 만들어보려고 수많은 컴퓨터과학자들이 오랜 기간 연구해왔
지만 최악 시간복잡도가 지수시간보다 좋은 알고리즘을 아직 개발하지 못했음을 알아낸
다. 게다가 그러한 알고리즘의 개발이 원천적으로 불가능하다고 증명도 하지 못했음도



===== PAGE 387 =====
376

chapter 9 계산복잡도와 다루기 힘든 정도:\ㅁ 이론의 소개

아울러 알아낸다. 희미하나마 ane 보인다. 길동이 그 BAS 푸는 효율적인 알고리
을 개발할 수 있으면, 외판원 문제를 푸는 효율적인 알고리즘도 개발할 수 있다고 증명ㅎ
보이면 어떨까? 수많은 우수 바사 이루지 못한 아주 어려운 작업을 상관이 요
구하고 있다고 주장할 수 있을 것이다. 당장 상관에게 달려가서 이를 증명할 기회를 달라

고 요청한다. 상관은 마지못해 허락한다. SSS 그 BAS 푸는 나씨 알고리즘을
만들 수 있다면 외판원 문제를 푸는 효율적인 알고리즘도 만들 수 있음을 단 일주일 노력
끝에 채색  결국 ASS 해고 대신 대 개발비용을 절감한 공        om 2a) 진하고, 상관
은 그 문제를 푸는 정확한 답을 얻는 알고리즘을 개발하는 대신 근사치를 찾는 등의 다른
방법을 추구해야 한다는 사실을 까맡는다.

이 이야기는 컴퓨터과학자들이 지난 25년간 성공적으로 알아낸 여려 그대로 대변하
고 있다. 외판원 문제와 수천 개의 다른 문제들은 어려운 정도가 같은 문제로 분류한다.
이 중에서 하나만이라도 효율적인 알고리즘ㅇ z 있다면 다른 모든 문제도 효율적인 알고리
즘이 있다는 사실을 알아냈다. ne 알고리즘을 하나도 찾지 못했지만, 찾기가 B7 KS st
다고 증명하지도 못했다.              들을 통 통털어:  ‘NP-Complete’ 로 분류하는데, 바로
이 장에서 다룰 주제이다. 효율적인 알고리즘을 만들기 불가능한 BAS "다루기 힘든
(intractable) 문제"라고 한다. 9.1절에서는 BAS 다루기 힘들다는 게 무엇을 의미하는
지 더 상세히 설명한다. 9.8절에서는 문제가 다루기 힘든지 아닌지 결정할 때 알고리즘의
입력크기를 매우 주의해서 정해야 한다는 사실을 알아본다. 9.3절에서는 다루기 힘든 정
"(intractability)S 가지고 분류한 문제의 세 가지 일반적인 카테고리를 설명한다. 이
장의 정점인 9.4절에서는 NPS} NP-Complete 문제의 이론을 공부한다. 9.5절에서는
NP-Complete 문제를 해결하는 방법을 살펴본다.

월 oly

91 다루기 힘든 정도

사전에 24 intractable(}#7] 힘들다)을 "취급하기 또는 작업하기 어렵다"로 정의한다.
컴퓨터로 문제를 풀기 어려우면 컴퓨터과학 용어로 "그 문제는 다루기 힘들다"라고 한다.
이 용어는 너무 막연하여 별로 사용하지 않는다. 용어를 더 상세히 정의하기에 앞서, “다
차시간 알고리즘"의 개념을 먼저 알아보자.

정의

=

다차시간 알고리즘(601/000181-!0106 algorithm)S 최악 시간복잡도의 상한이 입력크기의 다항
Al 함수가 되는 알고리즘이다. 즉, 7이 입력크기이면, 다음을 만족하는 CtStAl(polynomial)
p(n) 0| 존재한다.

Wn) = O(p(n))



===== PAGE 388 =====
© 예제 91

다음의 최악 시간복잡도를 가진 알고리즘은 모두 다차시간이다.
Qn 8n®+4n _ 5702+72? 0 21877
다음의 최악 시간복잡도를 가진 알고리즘은 다차시간이 아니다.

-00 0 9008 gvn 원

nig n-& no] 대한 다항식이 아니지만, 다음 부등식에 의해서
nign<n?

의 다항식이 상한이므로, nig nd 시간복잡도를 가진 알고리즘도 다차시간 알고리즘
으로 취급환다.

컴퓨터과학에서 어떤 문제를 다차시간 ener 풀 수 없으면, 그 문제를 다루기
@StHintractable)e}a1 한다. 다루기 힘든 정        를 푸는 어떤 특정 알고리즘의 성
질이 아니라 문제의 성질이라는 사실을 반드시 oe 한다. 다루기 힘든 문제가 되
려면 그 문제를 푸는 다차시간 알고리즘이 없어야 한다. 문제를 푸는 비다차시간(202ㅁ-
polynomial-time) 알고리즘을 찾았다고 해서 그 문제가 다루기 힘든 문제가 되는 것은
아니다. 예를 들어, 연쇄행렬곱셈 문제를 푸는 무작정 알고리즘(3.4절)은 비다차시간이
다. 3.4절에서 세운 재귀 관계식을 사용하는 분할정복 알고리즘도 마찬가지이다. 그러나
동적계획 알고리즘(알고리즘 3.6)은 ㅇ(@")이다. 이 HAE 알고리즘 3.68 사용하여 다
차시간에 풀 수 있으므로 다루기 힘들지 않다.

다차시간 알고리즘은 보통 비다차시간 알고리즘보다 보통 훨씬 좋다는 사실을 1장에
서 배웠다. 표 14S 다시 보면, 단위연산을 처리하는데 10억분의 1초가 걸린다면, 시간
복잡도가 “인 알고리즘은 크기가 100인 사례를 처리하는데 1천분의 1초가 걸리는 반면,

시간복잡도가 2”인 알고리즘으로는 수십억 Wo] 걸린다.

비다차시간 알고리즘이 다차시간 알고리즘보다 좋은 극단적인 예를 만들 수 있다. 예

를 들어, n=1,000,0009],

그

더구나 최악 시간복잡도가 다항식이 아님에도 불구하고 실제로는 효율적으로 실행되는
사례가 있는 알고리즘이 꽤 많이 있다. 되추적 알고리즘과 분기한정 알고리즘이 이에 속
한다. 따라서 다루기 험들의 정의는 실제로는 다루기 힘들 징후가 있다는 정도로만 해석
하면 된다. 경우에 따라서 다차시간 알고리즘이 있는 문제가 다차시간 알고리즘이 없는
문제보다 실제 상황에서 더 다루기 험든 경우도 있을 수 있다.

다루기 힘든 정도에 대하여 다음 세 가지 종류로 문제를 분류할 수 있다.

1 다차시간 알고리즘을 찾은 문제


===== PAGE 389 =====
378     chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개
2, 다루기 힘들다고 증명된 문제
3, 다루기 힘들다고 증명되지 않았지만 다차시간 알고리즘도 찾지 못한 문제
컴퓨터과학 문제가 대부분 첫째 또는 셋째 종류에 속하는 것은 놀라운 현상이다.
알고리즘이 다차시간인지 결정할 때 입력크기에 주의를 기울여야 한다. 더 진도를 나가
기 전에 입력크기에 대해 다음 절에서 좀 더 알아보자(입력크기를 처음 다룬 1.3절 참조)
©    입력크기 : 재고

지금까지 알고리즘에서 보통 n& 입력크기로 보았다. 왜냐하면, 7은 입력 데이터의 a

기를 나타내는 척도로서 적당했기 때문이다. 예를 들어, 정렬 알고리즘의 경우 정렬할

키의 개수인 ne 입력 데이터의 크기를 나타내는 좋은 척도이다. 따라서 n& 입력크기

라고 하였다. 그러나 nol 무조건 알고리즘의 Wela7/7 되는 건 아니다. 양의 정수 nel
소수(0000/인지 검사하는 다음 알고리즘을 보자.

bool prime (int 27)

{

int 7; bool switch;
switch = true;

while (switch && i < |n'”J)
if (2 % ==0)                       // %는 o& i 나눈 나머지를 FRE 연산

switch = false;

return switch ;

이 소수검사 알고리즘에서 while 루프의 실행 횟수는 분명 ㅇ(/2"“")이다. 그러나 이
알고리즘을 다차시간 알고리즘이라고 할 수 있을까? 파라미터 no] 알고리즘의 입력이긴
하지만, 입력크기라고 할 수는 없다. 즉, 7 값은 입력 사례일 뿐이다. 정렬 알고리즘과는
다르다. 정렬 알고리즘에서 n= 아이템의 개수이고 입력크기이다. 함수 227206에서 7값
이 입력이지만 입력크기로는 볼 수 없다면, 과연 입력크기는 무엇인가? 입력크기에 대해
서 1.8절보다 좀 더 상세히 정의한 후 이 질문으로 다시 돌아오자.

정의
주어진 알고리즘의 입력크기(1004 9126)는 입력을 작성하는데 필요한 문자의 개수로 정의
한다.

이 정의는 1.8절의 정의와 다르지 않다. 입력크기를 재는 방법에 대해서 | 더 명확히



===== PAGE 390 =====
0 00600000
9.2 입력크기: 재고   379

기술한 것뿐이다. 입력을 작성하는데 필요한 문자를 세어보기 위해서 입력이 어떻게 부
호화(620006)가 되는지 알 필요가 있다. 컴퓨터에서 사용하는 이진수로 부호화 한다고
가정하자. 그러면 부호화 하는데 사용하는 문자는 이진 숫자(비트)이고, 양의 ca 를 부
호화 하는데 필요한 문자의 개수는 Lg ㅠ|+ 1이다. 예를 들어, 31 = 11111, 04, [Ig 31]
+ㅜ1= 8이다. 이진으로 된 양의 정수를 부호화 하는데 대략 1』87개의 비트가 필요하다

고 간단히 말할 수 있다. 이진 숫자를 사용하고, 7개 양의 APS 정렬하는 알고리즘의
입력크기를 구해보자. 정렬할 정수들이 알고리즘의 입력이다. 따라서 입력크기는 그 정
수들을 부호화 하는데 필요한 비트의 개수를 세어보면 나온다. 가장 큰 AAI} Lo
LE 부호화 하는데 필요한 비트의 개수로 각 정수를 부호화 하여 각각 대략 18 L 비트

정도 필요하다. 따라서 /개 정수에 대한 입력크기는 대략 ^ lg Lo] 된다. ASS 십진수
로 부호화하는 경우는 어떨까? 그러면, 부호화하는데 사용한 문자는 십진 숫자이고, 가
장 큰 RAS 부호화 하는데 대략 log 개 문자가 필요하고, 7개 정수에 대한 입력크기
는 대략 nlog 』이다. 다음 등식이 성립하므로,

n log L = (0082) (n lg L)

이 입력크기 중 하나를 기준으로 알고리즘이 다차시간이다. S, 하나는 다른 하나를 기준
으로 다차시간이다.

“합당한(76880ㅁ81016)" 부호화 방법을 쓰기만 하면, 어떤 부호화 방법을 사용하는지는
알고리즘이 다차시간인지 결정하는데 SARS 미치지 않는다. “합당성"을 만족할 만한 정
의가 정식으로 존재하는 것 같진 않다. 그러나 대부분 알고리즘에서 무엇이 합당한지에
대해서 보통 의견일치를 본다. 예를 들면, 이 책의 알고리즘에 대해서 1을 제외한 어떤
베이스00886;를 사용하여 정수를 부호화하더라도 알고리즘의 시간복잡도에 영향을 미지
A] 않는다. 따라서 어떤 부호화 방법도 모두 합당하다고 여길 수 있다. 단, 단항인 베이스

부호화 하면 합당하지 않다.

앞장에서 정렬할 아이템의 개수 nS 정렬 알고리즘에서 입력크기라고 했다. n= 입력
크기로 하여 그 알고리즘이 다차시간임을 증명했다. 입력크기를 정확하게 따져도 다차시
간으로 남아 있을까? 이제 이를 증빙해보자. 입력크기를 정확하게 따지기로 했으므로 최
of 시간복잡도의 정의도(1.3.1절보다) 정확하게 따져야 한다. 정확한 정의는 다음과 같다.

IMS 비교연산 또는 저장연산으로 정한다. 기계독립적으로 분석하려면 비트의
연                       be 단위연산으로 정한다. 이렇게 정의하면 1.3절과 별로
다를 게 없고, 단위연산에 대해서만 좀 더 구체적이다. 입력크기로 n 대신 *를 사용한


===== PAGE 391 =====
380

chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개

이유는 다음과 같다. (1) 알고리즘의 파라미터 no] 항상 입력크기를 재는 척도는 아니다
(예를 들어, 이 절 시작부분에서 보여준 소수검사 알고리즘의 경우가 그렇다). (2) 7으로
입력크기를 Age, 이는 보통 입력크기의 정확한 척도가 아니다. 바로 위의 정의에 따르
면, 알고리즘이 실행한 단위연산의 개수를 모두 세어야 한다. 알고리즘 1.8(교환정렬)의
핵심만 골라 분석하여 어떻게 단위연산의 개수를 세는지 살펴보자. 설명의 편의성을 위
해서 키는 양의 정수이고 레코드에 다른 BES 없다고 가정한다. 알고리즘 1.8을 다시
살펴보자. 루프에서 증가하고 분기하는 단위연산의 개수의 상한은 상수 < 곱하기 nO]
다. 정수가 지나치게 크면, 컴퓨터로 한 번에 비교하거나 저장할 수 없다. 2.6절의 큰 정
수 연산을 공부할 때도 비슷한 상황을 목격했다. 이 경우 비교연산이나 저장연산을 단위
연산으로 잡지 말고, 기계독립적인 분석을 보장해주는 비트의 비교연산이나 비트의 저장
연산을 단위연산으로 잡아야 한다. 따라서 만약 Lo] 가장 큰 정수라면 정수를 한 번 비
교하거나 저장하는데 최대한 18 2 번의 비교연산을 거쳐야 한다. 1.8절과 7.3절에서 교환정
렬 알고리즘 1.8을 분석할 때 7개 So] 정수를 정렬하는데 최악의 경우 71S n(n—1)/2
번 비교하고, 3n(n—1)/24 저장함을 보았다. 따라서 교환정렬이 수행하는 단위연산의
최대 개수는 다음보다 크지 않다.

=           3n(n—1)
2    lg D+    2

비트의 비교 횟수      비트 대입 횟수

1827

입력크기로 ㅎ= 718 LS 사용해보자. 그러면,

W(s) = W(nlg L)       {6를 nlg Le 대치}

n(n—1)       3n(n—1)
0   lg 2+    5

< en? (Ig L)? +n? (Ig LZ)? + 3n? (lg 2)?

<cn?+                          lg Z

<(c+4)(n lg Ly = (c+ 4)s?

입력크기를 정확히 HAE 교환정렬이 다차시간을 유지함을 보았다. 부정확한 입력크
기를 사용하여 다차시간임을 확인한 알고리즘에 대해서도 비슷한 결과가 나온다. 더구
나, 비다차시간 알고리즘(예: 알고리즘 3.11)도 입력크기를 정확히 따질 때 비다차시간으
로 남음을 증명할 수 있다. no] 입력 데이터 크기를 재는 AES 때 단순히 nS 입력크
기로 해도 믿을만한 시간복잡도를 알아낼 수 WSS 알았다. 따라서 nS 그대로 입력크
기로 사용해도 문제없다.

이제 소수검사 알고리즘으로 돌아가 보자. 그 알고리즘의 YAS 7의 값이므로 입력
크기는 n& 부호화 하는데 필요한 문자의 개수이다. 십진수 부호화를 사용하면 을 부
호화 하는데 [108 1 + 1이 필요하다는 사실을 기억하자. 예를 들어, 수가 340이면, 그
수를 부호화 하는데 340개가 아니라 3개의 십진 숫자가 필요하다. 일반적으로, 십진수



===== PAGE 392 =====
@00@000000
93 문제의 3가지 일반적인 분류    381

부호화를 사용하고 $를 다음과 같이 놓으면,
s=logn

sx 대략 입력의 크기가 된다. 최악의 경우 prime 함수에서 루프를 7-2번 7
n= 10"“이므로, 최악의 경우 루프의 실행 횟수는 OF 10°7} 된다. 단위연산의 총 개수는
최소한 FEO] 실행 횟수와 같으므로 시간복잡도는 다차시간이 아니다. 이진수   부호회를
사용하면, n-& 부호화 하는데 OF 18 7개 문자가 필요하다. 따라서 이진 부호화를 사용하
면 다음과 같이 re 입력크기와 대략 같게 되고,

r=lgn

FES 실행하는 횟수는 약 2"번이다. 시간복잡도는 이번에도 다차시간이 아니다. "합당
한" 부호화 방법을 사용하는 한 결과는 항상 마찬가지이다. 단항 부호화를 "합당한" 방법
으로 여기지 않는다고 이미 언급하였다. 단항 부호화 방법을 사용한다면, nS 부호화 하
는데 개 문자가 필요하다. 예를 들어, 7S 1111111로 부호화 된다. 이 부호화를 사용하
면, 소수검사 알고리즘은 시간복잡도가 1차시간이다. 이와 같이 "합당하지 않은" 부호화
오아 ~ 사용하면 엉뚱한 결과를 얻는다.

수검사 알고리즘 같은 알고리즘에서 7을 입력의 AGa7|(magnitude)e}a1 한다. 절
dare 시간복잡도가 다차시간이지만 크기로는 다차시간이 아닌 다른 알고리즘도 이
미 본 적 있다. 7번째 피보나찌 BS 계산하는 알고리즘 1.7의 시간복잡도는 ㅇ(2))이다.
no] 입력의 절대크기이고, 187이 입력의 크기가 되므로 알고리즘 1.79] 시간복잡도는
절대크기로 1차시간이지만 크기로는 지수시간이다. 이항계수를 계산하는 알고리즘 3.2
의 시간복잡도는 0ㅇ(7”)이다. no] 입력의 절대크기이고, 18 neo] 입력크기이므로 알고리
즘 3,22] 시간복잡도는 절대크기로 2차시간이고, 크기로는 지수시간이다. 4.4.4절에서
공부한 0-1 배낭 채우기 문제에 대한 SAAS 알고리즘의 시간복잡도는 O(n W) ole.
이 알고리즘에서 nS 입력 아이템의 개수이므로 크기를 재는 척도이다. 그러나 We 배
낭의 최대용량이므로 절대크기가 되고, 18 WE ㅣ/의 크기를 재는 척도이다. 이 알고리
즘의 시간복잡도는 절대크기와 크기로 다차시간이지만 크기만 가지고는 지수시간이다.

최악 시간복잡도의 상한이 크기와 절대크기로 모두 다차시간이 되는 알고리즘을 의사
다차시간(086400201"0000481!-4108/이라 한다. 이러한 알고리즘은 지나치게 큰 수인 사례
를 처리할 때만 비효율적이므로 꽤 유용하게 쓸 수 있는 경우가 종종 있다. 예를 들
O-1 배낭 채우기 문제에서 가 지나치게 크지 않은 경우 문저 없이 쓸 수 있다.

9.3 문제의 3가지 일반적인 분류

다루기 힘든 정도(06808604109)로 분류한 문제의 세 가지 일반적인 카테고리를 알아보자.


===== PAGE 393 =====
382

chapter 9 계산복잡도와 다루기 힘든 WE: NP 이론의 소개

하는 007”) 알고리즘  "i isi,    연쇄행렬곱셈을  하는 O(n  *) 알고리즘을 찾았고, 등
등 이밖에도 많다. no] 이 을   고라즘의 he 데이터 크기를 나타내므로, ㅇ         즘들은
모두 다차시간이다. 사실 다차시간 알고리즘 목록은 한정없이 나열할 수 있다. 다차시간
알고리즘이 있는 문제를 푸는 shea} 알고리즘도 당연히 있다. 연쇄행렬곱셈 문제의

너너 누작정 알고리즘은     은 비다차시간이나 }시간 알고리즘을 찾았다. 무작정 알고리
즘을 찾은 기타 문제로는 최단경로 문제, 최적 이
진검색트리 문제, 최소비용 a 문제 등이 있다.

bi
ay
rN
quit

fal

9.3.2 다루기 31S               제
이 카테고리에 속하는 문제는 두 가지 종류가 있다. 첫째 종류는 지수이상 크기의 출력을
es 문제이다. 5.6절의 PLE 회로를 모두 구하는 문제를 보자. 모든 마디에서 다
는 마디로 이음선이 존재하면 해밀톤 회로가 (n— 1)! 7] 존재할 것이다. 이 문제를
푸는 배어 해밀톤 회로를 모두 출력해야 하는데, 이러한 요구사항은 현실적이지
않다. 5장에서 알고리즘을 간단하게 보여주려고 해답을 모두 구하도록 문제를 기술하였
지만, 하나의 해답만 출력하도록 이 알고리즘을 수정하기는 쉽다. 하나의 회로만 출력하
는 해밀톤 회로 BAL 다루기 힘든 Bayt 아니다. 이러한 종류의 다루기 힘든 문제를

Ho

|고 증명된
가

인식해내는 능력을 갖추어야 하지만 인식하기는 별로 어렵지 않다. 지수이상 크기의 출
력을 요구하는지 알아차리는 것은 쉽고, 일단 알아냈다면 필요이상으로 정보를 요구했을
경우가 많다. 즉, 문제 자체가 현실적이지 못한 것이다.

다루기 힘든 문제의 둘째 종류는 요구가 현실적이고(즉, 지수시간 이상 크기의 출력을
요구하지 않고), 문제를 다차시간에 풀 수 없다고 증명할 수 있는 경우이다. 기이하게도
이러한 문제는 상대적으로 별로 없다. 첫째로 진위판별불가능(00060108410) 문제가 이에
속한다. 푸는 알고리즘이 없다고 증명할 수 있는 문제를 “진위판별불가능 문제(2006000-
able problem)’2}31 한다. 가장 널리 알려진 진위판별불가능 문제는 멈춤검사 문제038-
Iting Problem)°|C}, 멈춤검사 문제는 임의의 알고리즘과 임의의 입력을 받아서 받은 알

고리즘에 받은 입력을 적용했을 때 알고리즘의 실행이 멈추는지를 판별하는 문제이다.
1986년에 알란 튜링(시80 Turing)o] 멈춤검사 문제는 진위판별할 수 없다고 증명하였다.
1958년 그레고르직(&. Grzegorezyk)-2 다루기 힘들지만 진위판별 가능한 문제를 하나 만
들었다. s4En}]A(Hartmanis)2} AAA(Stearns) = 1965에 발표한 ical Bier 결
과를 발표하였다. 그러나 그때까지 발견한 문제들은 모두 특                  = 인우
적으로 구죽한 것이었다. 1970년대 추반이 되서야(인위적으로 만들지 않은  일부 진위판
별 가능한 진위판별 문제가 다루기 힘들다고 증명되었다. 진위판별 문제(400.810ㅁ prob—



===== PAGE 394 =====
@0000600000
9.4 NP 이론  383

1600는 항상 “예(0) 또는 "아니오(×)"로만 대답한다. 즉, OX 문제이다. 따라서 문제의 요
구 출력 크기는 분명히 적당하다. 가장 널리 알려진 이 부류의 진위판별가능 문제 중 St
나는 1974년 피셔(001808360)와 라빈(88142)이 다루기 힘들다고 증명한 프레스버거 산술문
Al(Presburger Arithmetic)©]t}, 이 문제는 증명과 함께 SZ ASE (Hopcroft)2} 울만
(Ullman) 2] 책(1979)에 나와 있다.

지금까지 다루기 힘들다고 증명된 문제는 모두 NWP 집합에 속하지 않는다고 증명되었
다(9.4절 참조). 그러나 다루기 힘들 “것처럼 보이는" 문제는 대부분 NP 집합에 속한다.
다음 AA] 이러한 카테고리의 VAS 공부한다. 앞에서도 언급했듯이 다루기 힘들다고
증명된 문제가 상대적으로 거의 없다는 사실은 다소 놀라운 현상이고, 1970년 초가 되어
서야 인위적으로 만들지 않은 자연 진위판별 문제 하나가 다루기 힘들다고 증명되었다.

9.3.3 다루기 힘들다고 증명되지도 않았고, 다차시간 알고리즘도 찾지 못한 문제
다차시간 알고리즘을 찾지 못했지만, 그렇다고 다차시간 알고리즘이 불가능하다고 증명
하지도 못한 문제는 모두 이 카테고리에 속한다. 이미 설명했듯이 이러한 문제는 많이
있다. AS 들어, 해답을 하나만 내주도록 문제를 기술하면, 0-1 배낭 채우기 문제, 외판
원 문제, 부분집합의 합 구하기 문제, m7}4| 색으로 그래프 색칠하기 문제(7 = 3), 해
B= 회로 문제, 신뢰 네트워크에서 확률적 추론 문제들이 모두 이 카테고리에 들어간다.
다양한 대규모 사례에 대해서 이러한 문제를 효율적으로 푸는 분기한정 알고리즘, 되추
A 알고리즘 등의 알고리즘을 찾았다. 즉, 사례를 임의의 제한된 부분집합에서 취할 때
단위연산을 수행하는 횟수의 한계를 정하는 nol] 대한 다항식(6017ㅁ00489))이 존재한다.
그러나 모든 사례에 대하여 다항식이 존재하는 것은 아니다. 이를 보여주기 위해서 단위
연산을 수행하는 횟수의 한계를 정하는 nol] 대한 다항식이 없는 0“ linia     을 찾기
만 하면 된다. 랍비 되추적 알고리즘에서 이 작업을 ㅎ
이 카테고리에 속한 많은 문제들은 밀접하고 흥미롭게 서로 엮여있다. 이에 대해서 알
아보는 것이 다음 절의 목표이다.

@ 9.4 NP le

* 예제 9.2

처음부터 문제를 진위판별 문제로만 on 이론을 전개하기가 훨씬 더 수월해진다. 진
위판별 문제에 대한 해답은 단순히 "예(0)" 또는 “아니오(3)" 중 하나이다. 3, 4, 5, 6장에

서 최적화 문제를 공부한 적 ?   있다 터너 문제란 답이 최적해라는 말이다. 그러나 다음
예제에서 볼 수 있듯이 최적화 문제는 모두 각각에 대응되는 진위판별 문제가 존재한다.

외판원 문제
가중치가 있는 방향그래프가 있다고 하자. 이 그래프에서 여행경로는 한 마디에서 출발하여 다


===== PAGE 395 =====
@06000000
384     chapter 9 계산복잡도와 다루기 힘든 정도 :\ㅇ 이론의 소개

* 예제 9.3

* 예제 9.4

* 예제 9.5

른 모든 마디들을 정확히 한 번씩만 방문하고, 출발한 마디로 돌아오는 경로이다. 외판원 최적화
문제(178761108 Salesperson Optimization 『70016200는 이음선 상 총 거리가 최소가 되는 여행경
로를 구하는 문제이다.

외판원 진위판별 문제(178761108 Salesperson Decision Problem)+= 임의의 양수 d7} 주어지고,
총 거리가 0보다 길지 않은 여행경로가 있는지 판별하는 문제이다. 이 문제는 외판원 최적화
문제의 파라미터에다가 추가로 dS 파라미터로 사용한다.

0-1 배낭 채우기 문제

O-1 배낭 채우기 최적화 문제(0-1 Knapsack Optimization Problem)= 배낭에 넣을 아이템의 무
게와 가치를 안다고 가정하고 가치의 합이 최대가 되도록 아이템을 배낭에 어떻게 채울지를 알
아내는 문제이다. 여기서 배낭의 최대 용량은 이다.

0-1 배낭 채우기 진위판별 문제(0-1 Knapsack Decision 『ㅁ001600는 임의의 가치액수 가 주
어지고, 총 무게가 가 넘지 SOBA 총 수익이 최소한 P7} 되도록 HGS 채울 수 있는지
판별하는 문제이다. 이 문제는 0-1 배낭 채우기 최적화 문제의 파라미터에다가 추가로 PS 파라
미터로 사용한다.

그래프 색칠하기 문제
그래프 색칠하기 최적화 문제(37920-00101148 Optimization Problem)+= 인접한 두 마디가 같은
색이 되지 않도록 그래프를 색칠하는데 필요한 Mo] 최소 가지 수를 구하는 문제이다. 여기서
구한 가지 수를 그래프의 색채수(0ㅁ0008416 number)#}31 한다.

그래프 색칠하기 진위판별 4]|(Graph—Coloring Decision 『7001600는 임의의 정수 mo] 주어
지고, 최대한 #가지 색을 사용하여 인접한 두 마디가 같은 색이 되지 않도록 그래프를 색칠할
수 있는지를 판별하는 문제이다. 이 문제는 그래프 색칠하기 최적화 문제의 파라미터에다가 추
가로 ㅠ 을 파라미터로 사용한다.

파벌 문제

비방향그래프 ㅇ=(1, £) 에서 파벌(11046)은 Zt 마디가 다른 모든 마디에 인접해 있는 ve] 부
BAS 시다. 그림 9.1의 그래프에서 {0,, vy, vg} 파벌이지만, {,, vg, %} 은 이이 vz]
인접해 있지 않으므로 파벌이 아니다. 최대 파벌0ㅠ81081 01046)은 파벌 중에서 크기가 가장

럭                                             Vo

V5                                                         2

그림 9.1  최대 파벌은 10 Vg, Vay vs } 이다.



===== PAGE 396 =====
06000000
9.4 NP 이론  385

큰 파벌이다. 그림 9.1의 그래프에서 유일한 최대 파벌은 {0,, vy, vy %} 이다.

파벌 최적화 문제(01046 Optimization Problem)= 임의의 그래프에서 최대 파벌의 크기를 =
하는 문제이다.

파벌 진위판별 문제(11446 Decision 『『001600는 임의의 양 정수 《가 주어지고, 마디의 개수가
최소 《개가 되는 파벌이 존재하는지를 판별하는 문제이다. 이 BALE 파벌 최적화 문제의 파라
미터에다가 추가로 RS 파라미터로 사용한다.

Hie] 문제들에 대해서 진위판별 Gals} 최적화 문제 모두 다차시간 알고리즘을      을 아직
찾지 못했다. 그러나 어느 하나라도 최적화 문제에 대한 다차시간 알고리즘을 찾을 수
있다면, 그에 대응하는 진위판별 문제에 대한 다차시간 알고리즘도 존재할 것이다. 왜냐
하면, “최적화 문제에 대한 해답을 구하면, 그에 상응하는 진위판별 문제에 대한 해답은
쉽게 얻을 수 있기" 때문이다. 예를 들어, 외판원 문제의 어떤 특정 사례에 대한 최적 여
행경로의 총 거리가 190이라는 사실을 안다면 이에 대응하는 진위판별 문제에 대한 답은
다음 부등식을 만족하면 “예"가 될 것이다.

d= 120

만약 그렇지 않다면, “아니오"가 될 것이다. 유사하게 01 배낭 채우기 문제의 어떤 사례
에 대해서 최적 수익이 $930이라는 사실을 안다면, 대응하는 진위판별 문제에 대한 답은
다음 부등식을 만족하면 “예"가 될 것이다.

P < $230

만약 그렇지 않다면, “아니오"가 될 것이다.

최적화 문제를 푸는 다차시간 알고리즘을 가지고 그에 대응하는 진위판별 문제를 푸는
다차시간 알고리즘을 자동으로 만들어 낼 수 있으므로, 초기에는 진위판별 문제만 가지

고 이론을 전개할 수 있다. 따라서 먼저 진위판별 문제를 살펴보고, 다음에 최적화 문제
를 살펴보기로 한다. 그때가 되면 최적화 문제가 그에 대응하는 진위판별 문제와 훨씬
더 밀접히 관련되어 있음을 증명할 수 있다는 사실을 알게 될 것이다. 즉, (앞의 예제에서
다룬 문제들을 포함한) 많은 진위판별 문제에 대해서 그 진위판별 문제를 푸는 다차시간
알고리즘을 가지고 그에 대응하는 최적화 문제를 푸는 다차시간 알고리즘을 만들어 낼
수 있다고 증명되었다.

N

olN

9.4.1 Pt NP 집합
다차시간 알고리즘으로 풀 수 있는 진위판별 문제의 집합을 먼저 알아보자.

정의

P= 다차시간 알고리즘으로 풀 수 있는 모든 진위판별 문제의 집합이다.



===== PAGE 397 =====
386

chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개

떤 문제들이 01    하나? 다차시간 알고리즘이 있는 진위판별 문제는 모두 확실히
Po] 속한다. 예를 들어, 아이템이 배열 안에 있는지 판별하는 문제, 아이템이 정렬된 yy
에 있는지 판별하는 문제, 다차시간 알고리즘을 찾은 3장과 4장의 최적화 문제에
하는 진위판별 BASS 모두 Pol   ica  하지만   i }시간 알고리즘을 찾지 못한
ie 문제도 에 속할 수 있을까? 예를 들어, 외판       balay 문제가 에 속할
까? 아직 아무도 이 문제를 푸는 다차시간 i pee      만들어내지 못했지만 이
문제를 다차시간 알고리즘으로 풀 수 없다고 증명한 사람도 이리 없다. 따라서 이 문제가
에 속할 가능성도 있다. 결정문제가 Pol 속하지 SSS 알아내려면 그 문제를 푸는
개발하기가 불가능하다고 증명해야 한다. 외판원 진위판별 문제에
대해서는 아직 아무도 이를 증명하지 못했다. 예제 9.244] 9.5의 다른 진위판별 BAS
에도 모두 마찬가지이다.

어떤 진위판별 문제가 Poll 속하지 않을까? 예제 9.2부터 9.5의 진위판별 BASS 모

두 에 속하는지 알지 못하므로 이 문제들은 Pol] 속하지 않을지도 모른다. 그냥 단순히
알지 못할 뿐이다. 더구나 이와 같은 카테고리에 속한 See 문제가 수천 개 있다.

ㅇ

> mw ae
ay

그
a >
tte

42 그 문제들이 Po] 속할지도 모른다. 개리(38760)와 =A(Johnson)2] 책(1979)을 보면
이 카테고리에 속한 문제들을 많이 점할 수 있다. Pal 속하지 않음을 확실히 이는 진위
판별 문제는 실제 거의 없다. Pol 속하지 hee 확실히 아는 BAGS 다차시간 알고리

즘이 없다고 증명된 진위판별 문제이다. 이러한 문제들은 9.8.2절에서 몇 개 알아봤다.
그 중 가장 널리 알려진 문제는 프레스버거 산술문제이다.

예제 9.2부터 9.52] 문제들을 모두 포함한 더 넓은 범위의 진위판별 문제 집합을 정의
해보자. 우선 외판원 문제를 확실히 이해하고 시작하자. 외판원 문제의 어떤 사례에 대한
답이 “PAS 알고 있다고 주장하는 사람이 있다고 가정하자. 즉, 그 사람은 임의의 수
dol] 대해서 주어진 그래프에 총 거리가 dS 넘지 않는 여행경로가 있다고 말했다. 총
거리가 0보다 길지 않은 여행경로를 실제로 찾아보라고 그 사람에게 요구할 수 있다. 그
사람이 찾아낸 여행경로의 총 거리가 0 이하인지를 검증(06013)하는 알고리즘은 다음과
같이 쉽게 작성할 수 있다. 이 알고리즘의 입력은 그래프 G, 거리 0, 여행경로 문자열
Solty,

bool verify (weighted_ digraph G,

number d,
claimed_tour 5S)

if (S= 여행경로이다 && Sol] 속한 가중치의 합 <= d)

return true ;

else

return false ;

이 알고리즘은 가 여행경로인지 먼저 검사한다. 만약 여행경로가 맞다면 알고리즘은



===== PAGE 398 =====
@0000000
9.4 NP 이론  387

여행경로 상의 가중치(거리)를 모두 더한다. 가중치의 SO] 0보다 크지 않으면, "\ㅠ406 를
넘겨준다. 이는 총 바버 0 이하인 여행경로가 존재하고, 이 진위판별 문제에 대한 HS
"예"임이 검증                      . 만약 STE 여행경로가 아니거나 가중치의 합이 dS 초
과하면, 알고리즘은 "66186 를 : 넘겨준다. faseS 넘겨주면 주장한 여행경로는 총 거리가
4 이하가 아니라는 사실만 의미할 뿐이다. 총 거리가 ad 이하의 여행경로가 없다는 의미는
아니다. 왜냐하면, 총 거리가 0 이하인 다른 여행경로는 아직 따져보지 않았기 때문이다.

이 알고리즘을 더 상세히 기술하고 이 알고리즘이 다차시간임을 증명하는 작업은 연습
문제로 남겨둔다. 주어진 여행경로 후보를 가지고 진위판별 문제의 해답이 “예"임을 다차
시간에 검증할 수 있음을 의미한다. (그 사람이 거짓말을 하여) 제안한 여행경로가 여행
경로가 아니거나 총 여행길이가 0보다 크다고 해서 진위판별 문제에 대한 해답이 “아니
VMAS 증명한 건 아니다. 따라서 진위판별 문제에 대한 해답이 “아니오"임을 다차시간

에 검증할 수 있다고 할 수 있는 건 아니다.

NP 집합에 속한 BAS] 지니고 있는 다차시간 검증가능성(0017ㅁ4000181-10ㅁ6 ver—
ifiability) 9] 성질을 정의해보자. 이 문제들을 다차시간에 폴어야 한다는 의미는 아니다.
후보 여행경로의 총 길이가 0 이하임을 검증할 때 그 여행경로를 찾는데 걸리는 AZ
빼고 따졌다. 검증만 하는데 다차시간이 걸린다고 한 것뿐이다. 다차시간 검증가능성의
개념을 더 상세히 기술하기 위해 비결정 알고리즘(0400406[610010181410 algorithm) 의 개념을
도입한다. 비결정 알고리즘은 다음과 같이 두 단계로 구성되어 있다고 볼 수 있다,

1. (비결정) 추측 단계 : 문제의 사례를 가지고 단순히 임의의 문자열 SS 만들어 낸
다. 만든 문자열은 추측한 해답으로 보면 된다. 사실 전혀 무의미한 문자열이어도
상관없다(역주: 즉, 만든 문자열이 해답이 될는지는 완전히 Lol] 맡긴다).

2. (결정) 검증 단계 : 입력은 문제 사례와 추측한 문자열 이다. 이 단계는 일반적인
결정 실행방식으로 다음과 같이 진행된다. (1) 궁극적으로 “6ㅠ06 의 출력을 내주면
서 멈추거나(이 사례에 대한 해답이 "예'라고 검증되었음을 뜻한다), (2) “false” 의
출력을 내주면서 멈추거나, (3) 멈추지 않는다(무한루프). 뒤의 두 경우 이 사례에
대한 해답이 “예"라고 검증되지 않았음을 뜻한다. 앞으로 알게 되겠지만, 비결정
알고리즘으로 (2)와 (VL 구별할 수 없다.

verify 함수는 외판원 진위판별 문제의 검증단계에 해당하며, 결정 알고리즘이다. 비
결정적이 되는 부분은 추측 단계로서 어떻게 해답을 만들어내는지 명시하지 않으므로 비
AA (nondeterministic) 단계라고 한다. 이 단계에서는 오히려 아무 문자열이나 임의로
만들어도 된다. "비결정 단계"는 다차시간 검증가능성의 개념을 정립하기 위한 치장도구
에 불과할 뿐이며, 진위판별 문제를 풀기 위한 현실적인 WHS 아니다.

비결정 알고리즘을 실제로 문제를 푸는데 절대 사용할 수 없지만, 다음 두 조건을 만족
하면 비결정 알고리즘이 진위판별 BAS "푼다(6076) 고 한다.


===== PAGE 399 =====
@0@000000
388     chapter 9 계산복잡도와 다루기 힘든 WS = NP 이론의 소개

\

그림 9.2 여행경로 ,, vg, vg, vg vi JE 총 가중치가 15보다 크지 않다.

1, 해답이 “예"가 되는 사례에 대하여 검증단계의 결과가 “true’7} 되는 문자열이 있다.
2, 해답이 “아니오"가 되는 사례에 대하여 검증단계의 결과가 "ㅠ06'가 되는 문자열
이 없다.

다음 ES 보면 사례가 그림 9.8의 그래프이고 a7} 15일 때, 입력 문자열 SS verify
함수에 적용한 결과를 나열한다.

님              출력                          이유
yy Uy; Vey By 이       false        총 가중치는 15보다 크다
[vy V4» Ue) Vy» 이]       false        Se 여행경로가 아니다
#@12* &%a,\           fasle         SE 여행경로가 아니다
1 Ug) Vp) Uy 이]       true         SE 총 가중치가 15보다 크지 않은 여행경로이다

셋째 WAS (앞에서 설명했듯이) 가 전혀 무의미한 문자열이어도 상관없음을 보여
준다.

일반적으로 특정 사례에 대하여 해답이 “예'이면, 총 가중치가 0보다 크지 않은 여행경

들 중 하나가 입력일 Wh verity 함수는 "706 를 넘겨준다. 따라서 비결정적 알고리즘의
기준 1°] 만족되었다. 반면에 verify 함수는 총 가중치가 0보다 크지 않은 여행경로가
입력일 때만 “606 만 넘겨준다. 따라서 만약 어떤 사례에 대한 해답이 "아니오"이면, ver-
ify 함수는 어떤 S 값에 대해서도 “true’S 넘겨주지 않는다. 그러므로 기준 2가 만족되었
다. 결론적으로 추측 단계에서 단순히 문자열을 생성하고 AS SAMA verify 함수를
호출하는 비결정 알고리즘은 외판원 결정문제를 "푼다"고 할 수 있다. 이제 다차시간 비
결정 알고리즘을 정의해보자.

정의

o

다차시간 비결정 Vt12|ZB(polynomial-time nondeterministic algorithm)LS 검증단계가 다차
시간 알고리즘인 비결정 알고리즘이다.

이제 집합 NPS 정의할 수 있다.



===== PAGE 400 =====
0000000
9.4 NP 이론  389

정의

NP= 다차시간 비결정적 알고리즘으로 풀 + 있

rr

모든 진위판별 문제의 집합이다.

rin

NP = “Nondeterministic(4]A%) Polynomial(t}4})’2] 약자임을 주목하자. 진위판별
문제가 /7^에 속하기 위해서는 다차시간에 ASS 하는 알고리즘이 반드시 존재해야 한
다. 외판원 진위판별 문제는 검증하는 다차시간 알고리즘이 있으므로 NPol] 속한다. 검
증하는 다차시간 알고리즘이 있다고 해서 BAS 푸는 다차시간 알고리즘이 있다는 의미
는 절대 아니다. 사실, 외판원 진위판별 BAS 푸는 다차시간 알고리즘이 있는지 아직
모른다. 임의로 주어진 사례에 대해서 외판원 진위판별 문제의 답이 “예"라면, verify7}
‘true’ HS 넘겨주는 여행경로를 찾기 위해 비결정 단계에서 여행경로를 모두 조사해봐
야 할지도 모른다. 마디들끼리 모두 이음선으로 AAS] 있다면, 여행경로의 개수는 모
두 (ㅠ-1)!개이다. 따라서 여행경로를 모두 따져봐야 한다면 당연히 다차시간에 답을
얻지 못할 것이다. 더구나, 사례에 대한 대답이 "아니오"라면, 모두 다 따져보지 않고는
절대 답을 확신할 수 없다. 비결정 알고리즘과 NPI WIS 도입한 목적은 알고리즘을
분류하고 싶었기 때문이다. BASS 생성하고 검증하는 비결정 알고리즘보다 실제로 문
제를 푸는 더 좋은 알고리즘이 보통 존재한다. 예를 들어, 외판원 문제를 푸는 분기한정
알고리즘(알고리즘 6.9)은 여행경로를 생성하지만, 한계 함수를 사용하여 Fo] 될 가능
성이 없는 여행경로의 생성은 피한다. 따라서 여행경로를 무조건 생성하는 알고리즘보다
는 훨씬 더 좋다.

NP 속하는 진위판별 문제가 또 있을까? 예제 9.8에서 9.5까지의 진위판별 문제도
모두 NPF 속함은 연습문제로 확인해보도록 하자.

더구나 그 외에도 다차시간 알고리즘이 있는지는 아직 모르지만 문제를 푸는 다차시간
비결정 알고리즘은 있기 때문에 /7^에 속함이 증명된 진위판별 문제가 수천개 이상 존재
한다(개리와 존슨의 책(1979)에 많이 소개되어 있다). 마지막으로, 따져볼 것 없이 사소하
Al NP 속하는 문제도 상당히 많다. 즉, “에 속하는 문제는 모두 //7에도 속한다.”
Po) 속한 문제는 모두 다차시간 알고리즘으로 풀 수 있으므로 따져볼 것 없이 사소하게
사실이다. 비결정 단계에 아무 문자열이나 생성하고, 결정 단계에서 다차시간 알고리즘
을 실행한다. 알고리즘은 “ap 또는 “아니오"로 대답하여 문제를 풀기 때문에 ("예" 답을
주는) 입력 문자열 가 주어지면 대답이 “예"임을 항상 검증해준다.

어떤 진위판별 문제가 NP] 속하지 않을까? 신기하게도 /7^에 속하지 않는다고 증
명된 진위판별 문제들은 다루기 힘들다고 증명된 문제들이다. 즉, 멈춤검사 문제, 프레스
버거 산술문제, 그리고 9.8.3절에서 공부한 문제들은 NP] 속하지 않음이 증명된 문제
들이다. 다시 말하지만, 이 부류의 BASS 상대적으로 별로 없다.

그럼 9,394] 모든 진위판별 문제의 집합을 그림으로 보여준다. 이 그림에서 WPE
PS 진부분집합으로 포함하고 있는 걸로 그려놓았다. 그러나 그렇지 않을지도 모른다.



===== PAGE 401 =====
390

chapter 9 계산복잡도와 다루기 힘든 WE: NP 이론의 소개

모든 진위판별 문제의 집합

멈춤검사 문제와
프레스버거 산술
문제는 여기에 속한다

NP
So            여기에 확실히 속한다고
알려진 문제는 없다

그림 9.3 모든 진위판별 문제의 집합

rn

4, NP 속하면서 Pol 속하지 않는 문제가 있다고 아직 증명하지 못했기 때문이다. 따
가  는 공집합일 수도 있다. 사실 “와 ^/7가 같은가?"는 컴퓨터과학에서 가장      매리 al
고 중요한 오픈문제 중 하나이다. 이미 언급했듯이 알고 있는 진위판별 문제는
“에 속하므로 0] 오픈문제는 중요하다. 따라서 만약 P= 가 사실이라면 지금까
A) 알고 있는 대부분의 진위판별 문제를 푸는 다차시간 알고리즘이 있다는 얘기이다.
< NPYS 증명하려면 NP 속하면서 Pos 속하지 않는 문제를 찾아야 한다.
반면 P= NPYS 증명하려면 에 속한 각각의 문제에 대해 다차시간 알고리즘을 모
두 찾아야 한다. 그런데 이 작업은 단순화할 수 있다. 즉, 많은 문제 중에서 하나만 다차
시간 알고리즘을 찾으면 된다. 이와 같이 작업을 엄청나게 단순화했음에도 불구하고 P
가 NPS} 같다고 믿는 사람은 거의 없다.

9.4.2 NP-Complete 문제

예제 9.24] 9.572] 문제들의 어려운 정도가 모두 같진 않다. 예를 들어, 외판원 문제
를 푸는 동적계획 알고리즘(알고리즘 3.11)은 최악의 경우 ㅇ(/2^2"”)이다. 한편, 0-1 배낭
채우기 문제를 푸는 동적계획 알고리즘(알고리즘 4.4)은 최악의 경우 ㅇ(2"”)이다. 또한
외판원 BAS 푸는 분기한정 알고리즘(알고리즘 6.9)에서 상태공간트리의 잎이 (2-1)!
개인 반면, 0ㄱ1 배낭 채우기 BAS 푸는 분기한정 알고리즘(알고리즘 6.2)에서는 2" '
개뿐이다. 마지막으로 0-1 배낭 채우기 문제를 푸는 동적계획 알고리즘은 O(n W) 인데,
이는 배낭의 용량 W7} 아주 크지 않는 한 효율적임을 의미한다. 이 모든 것으로 미루어
보건대 0-1 배낭 채우기 문제가 원천적으로 외판원 문제보다 더 쉬운 것 같아 보인다.
그럼에도 불구하고, 이 두 문제와 9.2에서 9.5까지의 문제들, 그리고 수천 가지의 다른
문제 중 하나만이라도 Pol] 속하면 나머지 모든 BASE 마찬가지로 Pol] 속해야 한다
는 점에서 모두 동등하게 취급할 수 있다. 이러한 문                   고 한다.



===== PAGE 402 =====
* 예제 9.6

© 예제 9.7

@©@eee8ee6e@e
9.4 NP 이론  391

NP-CompleteS 이해하기 위해서 NP-Complete 이론에 기초가 되는 CNF-Satisfiability
문제를 우선 먼저 이해해보자.

CNF-Satisfiability 문제

논리(불) APE truct} false 값 중 하나를 가질 수 있는 변수이다. 2 가 논리 변수이면, 2 는 2 의
부정(0688400)이다. 즉 x7} true], r+ 『8186이다. 2]e] A (literal) 논리 변수이거나 논리
변수의 부정이다. A(clause)S 논리 연산자 or(v)S 사이사이에 끼운 리터럴의 나열이다.
CNF(Conjunctive Normal Form) 논리식(1091091 expression) 으로 논리 GA} and(A )= 사이
사이에 끼운 절의 나열이다. 다음은 CNF 논리식의 예이다.

(2,Vt_V 25) A (2, V £4) A (29V 23V 24)

CNF-Satisfiability 진위판별 문제는 주어진 CNF 논리식을 true 만드는 참값 대입(변수에 46
EE falseS 대입)이 존재하는지 판별하는 문제이다.

다음 사례에 대해서 CNF-Satisfiability 문제의 답은 “예"이다.
(2, V2) A (tV 23) A,

왜냐하면, x, =true, x, =false, x, =falseS 대입하면 이 논리식이 trueo]7] 때문이다. 다음 Ap
례에 대해서 CNF-Satisfiability 문제의 답은 “아니오"이다.

(2, Vt) A2,AZq

왜냐하면, 이 논리식이 true7} 되는 참값 대입이 없기 때문이다.

CNF 논리식과 변수에 대입할 참값을 입력으로 받아서 그 대입에 대해서 그 논리식이
1ㅠ46인지 검중하는 다차시간 알고리즘은 쉽게 작성할 수 있다. 그러므로 이 HAE WP
에 속한다. 그러나 이 BAS 푸는 다차시간 알고리즘을 아직 아무도 찾지 못했고, 이
TAS 다차시간에 풀 수 없다고 아직 아무도 증명하지 못했다. 따라서 이 문제가 에
속할지도 모른다. 이 문제를 특별히 주목하는 이유는 1971년 스티븐 (Stephen Cook)°]
CNF-Satisfiability 문제가 Pol] 속한다고 가정하면, P= NP7} 사실임을 증명하는 논문
을 발표했기 때문이다(이와 유사한 정리를 1973년 레빈(.ㅅ4. Levin)o] 독립적으로 발표
하기도 했다). +2] 정리를 엄밀히 검토하기 전에 "다차시간 축소변환가능도(0017ㅁ00181-
time reducibility)’2}31 하는 새로운 개념을 알아야 한다.

가령 진위판별 문제 AS 풀려고 하고, 진위판별 문제 BS 푸는 알고리즘이 있다고 가
정하자. 그리고 문제 BS 푸는 알고리즘이 yo 대해서 “예"라고 답하면 문제 Aol] 대한
답도 “예"가 되도록 문제 AS] 모든 사례 co] 문제 BS] 사례 yS 만들어내는 알고리즘
을 작성할 수 있다고 가정하자. 변환 알고리즘(\ㅠ808[01003110ㅁ algorithm)°]2}32 하는 이
고리즘은 문제 4의 모든 ABS 문제 BS] 사례로 실제로 매핑하는 함수이다. 이 함수

ue


===== PAGE 403 =====
@‥0 00000 0
392     chapter 9 계산복잡도와 다루기 힘든 AS: NP 이론의 소개

* 예제 9.8

문제 8를      Pee fa
>   tran = |} /=1727000ㅡ1 푸는      >a 아니오
알고리즘

를 진위판별 문제 GO| 사례 y= 매핑하는
. 진위판별 문제 BB 푸는 알고리즘을 가지고 rank 진위판별 문제 AB 푸는

y= tran(x)

문제 BE 푸는 알고리즘을 가지고 이 변환 알고리즘을 적용하여 문제 AS 푸는 알고리
즘을 만들어낸다. 그림 9.4에서 이 과정을 보여준다.

다음 예제는 NP-Complete 이론과는 무관하다. 단지 변환 알고리즘의 간단한 예를 보
여주기 위해서 제시하는 것이다.

변환 알고리즘

첫째 진위판별 문제는 "논리 변수가 7개 있을 때 그중 최소한 하나가 “true” AS 가지는가?"이
고, 둘째 진위판별 문제는 "정수가 7개 있을 때 가장 큰 수가 양수인가?"라고 하자. 변환식은
다음과 같다고 하자.

Big hayes 시 =tran(x,, 06. z)

여기서 2,가 006이면 는 1이고, 2,7} falseol el 는 0이다. 둘째 문제를 푸는 알고리즘이 “예"
를 넘겨준다는 사실은 최소한 하나의 “는 1임을 의미하고, 이는 다시 최소한 하나의 2,는 true
임을 의미한다. 그러므로 둘째 문제를 푸는 알고리즘이 “예"를 넘겨준다는 AMIS 최소한 하나의
싸는 006임을 의미하고, 이는 다시 변환 알고리즘이 성공적임을 의미한다. 따라서 둘째 문제를

=
알고리즘을 사용하여 첫째 HAS 풀 수 있다.

개
rir

방금 공부한 개념과 관련된 다음 BIS 보자.

정의
정의
진위판별 문제 AS 진위판별 문제 BS 변환하는 다차시간 변환 알고리즘이 존재하면, '문제
A= 문제 BE 다차시간 다일 BAHSHES(polynomial-time many—one 「60401010)`하다(보통

그냥 “문제 4는 문제 G2 축소변환된다"라고 한다). 심벌로는 다음과 같이 표현한다.

22

"다일0280”-006/ 이라고 한 이유는 변환 알고리즘이 문제 A] 많은 사례에서 문제 2



===== PAGE 404 =====
@0ㅎ00000 0
9.4 NP 이론  393

의 she] APS 매핑하는 함수이기 때문이다. 즉, 이는 다일 aot
변환 알고리즘은 다차시간이고 문제 BS 푸는 다차시간 알고리즘이 있다면, 변환 알
고리즘과 문제 BE 푸는 알고리즘을 결합하여 만든 문제 AS 푸는 알고리즘은 직관적으
로 보아 분명히 다차시간 알고리즘이다. 예를 들어, 예제 9.8의 변환 알고리즘은 명백히

다차시간이다. 그러므로 변환 알고리즘과 둘째 문제를 푸는 다차시간 알고리즘을 차례로
실행하면, 첫째 문제를 다차시간에 풀 수 있을 것 같다. 다음 정리에서 이를 증명한다.
> 정리 9.1

진위판별 문제 B7} Pol] 속하고, 다음이 성립하면,

AGB

(eal

위판별 문제 도 Poy 속한다.

명 : 문제 AS 문제 BE 변환하는 sala     변환 알고리즘의 시간복잡도의 상한을 나타내
는 다항식을 pe} 하고, BE 푸는 다차시간 알고리즘의 시간복잡도의 상한을 나타내는 다항식
을 4라고 하자. 크기가 7인 문제 의 사례가 있다고 가정하자. 변환 알고리즘에는 최대 p(n)
의 단계가 존재하고, 최악의 경우 각 단계마다 알고리즘이 무언가를 출력하므로 변환 알고리
즘이 만들어내는 문제 BS] 사례의 크기는 최대 p(n) oleh, 이 사례가 문제 BS 푸는 알고리즘
이 입력되면, 이는 AAS g(p(n)) 2] GA} 존재한다는 의미가 된다. 따라서 문제 의 사례
문제 BO] 사례로 변환하고 문제 Aol] 대한 맞는 답을 구하기 위해 문제 BS 푸는데 필요한
총 작업량은 다음과 같다.

이

lo (|

1 00

n) +q[p(n)]
이 식은 7에 대해 다항식이다.

이제 NP-Complete= 정의해보자.

정의

문제 B= 다음 두 AUS 만족하면 //^-0000!66라고 한다.
1. 에 속한디
2. 에 속한 모든 다른 문제 Aol] 대하여 다음이 성립한다.

4262

정리 9.1에 의하여 “어느 NP-Complete 문제 하나라도 Pol] 속한다고 증명할 수 있으
면 P= NPA 결론지을 수 있다.” 1971년 스티븐 0] NP-Complete?] 문제 하나를
용케 찾아냈다. 다음 정리는 그의 발견 결과를 설명한다.

정리 9.2

30] 정리 CNF-Satisfiability NP—-Complete°]t},


===== PAGE 405 =====
@eeeeee
394     chapter 9 계산복잡도와 다루기 SIS AS: NP 이론의 소개

© 예제 9.9

증명 : 증명은 Bo} 논문0971)과 개리와 존슨의 (1979S 참조한다.

4°] 정리를 증명하기 위해서 에 속한 문제를 모두 각각 CNF-Satisfiability 문제
로 축소변환하지는 않았다. 만약 그렇게 증명했다면, VP] 속한 문제를 새로 찾을 때마
다 CNF-Satisfiability 문제로 축소변환이 가능한지 확인해봐야 할 것이다. 대신, /2에
속한 문제하면 반드시 CNF-Satisfiability 문제로 축소변환할 수 있음을 증명하기 위해서
NP?7| 공통으로 지니고 있는 성질을 SB 사용하였다.

이 가공할 만한 정리가 일단 증명되고 나자, 다른 많은
속속 증명되었다. 다음 정리를 사용하여 이 증명을 할 수

문제들도 NP-Complete?]°]
있다.

정리 9.3

문제 Ch: 다음 두 조건을 만족하면 ^-000206이다.
1, C= NP 속한다.
2, 다른 NP-Complete 문제 Bol] 대하여 다음이 성립한다.
Bie C

증명 : B7} NP-Complete?|2=, NPol] 속한 임의의 문제 4에 대해서 Ax 가 성립한다.
이 축소변환 가능도가 ©] BA (transitive) YS 어렵지 않게 알 수 있다. 따라서 Ax (가 성립
한다. CL NPo] 속하므로, CL 42"-000ㅁ201066라고 결론지을 수 있다.

Bo) 정리와 정리 9.3을 가지고, 문제가 NP] 속하고 CNF-SatisfiabilityS 그 문제
로 축소변환 가능함을 보여서 그 문제가 MP-CompletedS 증명할 수 있다. 이 축소변
St 과정은 예제 9.7의 축소변환 과정보다 훨씬 더 복잡하다. 다음에 그러한 변형의 예를
하나 살펴보자.

파벌 진위판별 문제가 ^/2"-06002160[6임을 증명한다. 파벌 진위판별                  at AS
알고리즘을 작성하여 이 문제가 NP 속하는지에 대한 SYS 연습문제로 남겨둔다. 그러면
]제 이 문제가 NP-Complete2}3. 결론짓기 위해서 다음이 성립하는지만 증명하면 된다.
CNF-Satisfiability % 파벌 진위판별 문제

먼저 비방향그래프에서 파벌은 마디들의 부분집합으로서 그 부분집합의 각 마디가 그 부분집합

에 속한 다른 모든 마디들과 인접해 있다. 파벌 진위판별 문제는 그래프와 양의 정수 *에 대하여
그 그래프에 최소한 마디가 《개인 파벌이 있는지 판별하는 문제이다. 다음 등식을 CNP 논리식
이라고 하자.

ㅇ

BHO ACA KO.
여기서 각 CS BY 절이고, ay, 2,, …, #,은 BOY 속한 변수라고 하자. BE 그래프 C=(V; B)
로 다음과 같이 변환된다.



===== PAGE 406 =====
@000000
9.4 NP 이론  395

그림 9.5 B=(2,V2,V23)A(2,V2,V23)Y 때 예제 9.9의 그래프 G

V=ty7t A Gol 속한 리터럴인 (^, 2)}

E= {~ jolt 5=4인 ((y, a), (8, 9))}
GS 구축하는 실례가 그림 9.5에 나와 있다. 이 변환 과정이 다차시간인지 증명하는 작업은 A
습문제로 넘긴다. 따라서 “BE 000-88116884016하다"라는 말은 “CNF-Satisfiabled}4, 에 최
소한 크기가 kel 파벌이 있다"라는 말과 같다. 이를 이제 증명해보자.

1. B7] 040"-88466866하면 Gol) 최소한 크기가 kel 파벌이 있음을 증명한다. 만약 B7}

CNF-Satisfiabled}' 각 절이 true7} EE ay, xy, ..., x, 에 대한 참값 대입이 존재한다. 따
라서 이 대입으로 \06가 되는 리터럴이 각 Aol 최소한 하나는 존재한다. 각 {에서 그
리터럴을 하나씩 선택한다. 그리고

~ ={4가 (에서 ARS true 리터럴인 (^, 1)}
명백히 는 크기 kel 0의 파벌을 형성한다.

2, Go] 최소한 크기가 *인 파벌이 있으면, BE CNF-SatisfiableS 증명한다. 마디 (y, i) 에서
마디 (2, )로 가는 이음선이 존재할 수 없으므로, 파벌에 속한 마디의 인덱스는 반드시 모
두 달라야 한다. 다른 인덱스가 《개만 있으므로, 파벌에는 최대로 마디가 k7 있을 수 있다.
따라서 Gol] 크기가 최소한 《인 파벌 (^, # )이 있다면, 에서 마디의 개수는 정확히
“개가 되어야 한다. 따라서 다음과 같이 놓으면,

000 1) = 원. y}
에 리터럴이 &개 있다. 더구나 SE 《개의 절에서 온 리터럴이 하나씩 있다. 왜냐하면,
임의의 ySt 와 인덱스 :에 대해서 (y, i) St (>, 0) 를 연결하는 이음선이 존재하지 않기 때
문이다. 마지막으로 SE 리터럴 yS 그의 역 yS 둘 다 동시에 포함할 수 없다. 왜냐하면
임의의 1와 )에 대해서 (y, ?)  (y, 7) 를 연결하는 이음선이 존재하지 않기 때문이다. 따라

서 다음과 같이 놓고,

에 속하지 않은 변수에 임의의 참값을 대입하면, Bo] 속한 BE AS true7} 된다. 따라서 BE
CNF-Satisfiabled}t}.



===== PAGE 407 =====
@‥@000 0 0 0
396     chapter 9 계산복잡도와 다루기 힘든 정도 :\ㅁ 이론의 소개

© 예제 910

5.6절에서 해밀톤 회로 문제를 상기해보자. 해밀톤 회로 진위판별 문제는 연결된 방향
그래프에 최소한 하나의 여행경로가 존재하는지 판별하는 문제이다(한 마디에서 출발하
여 그래프의 각 마디를 한 번씩 방문하고, 출발마디에 도칙하여 끝난다). 다음이 성립함
을 보일 수 있다.

CNF-Satisfiable 해밀톤 회로 진위판별 문제

이 축소변환 과정은 앞의 예제보다도 더 지루한데, 호로위츠(3000\1[2)와 사니(3314)의
책(1978)에 나와 있다. 이 문제에 대한 다차시간 검증 알고리즘의 작성은 연습문제로 남
겨둔다. 따라서 해밀톤 회로 진위판별 문제는 //7^-060210[6이라고 결론지을 수 있다.

이제 파벌 문제와 해밀톤 회로 문제가 NP-Completed& 알기 때문에 에 속한 다
= 문제도 파벌 문제와 해밀톤 회로 문제가 그 문제로 축소변환됨을 보임으로써 NP-
00000!06임을 증명할 수 있다(정리 9.3 적용). 2 NP-Complete= 증명할 때마다 CNF-
Satisfiable= 돌아갈 필요가 없다. SAWS] 예를 몇 가지 더 공부해보자.

그래프에서 방향을 빼고 변형한 외판원 문제를 공부해보자. 즉, 가중치가 있는 비방향그래프와
양수 dS 주고, 총 가중치의 Bo] 0보다 크지 않은 비방향 여행경로가 있는지 판별한다. 앞서
공부한 외판원 문제의 다차시간 검증 알고리즘이 이 문제에도 그대로 적용할 수 있다. 따라서
이 문제가 에 속하는지 증명하고, NP-Complete 문제 중 하나를 이 문제로 축소변환할 수
있는지 증명하기만 하면 이 문제는 2^-0602!06이다. 즉, HSS 증명한다.

해밀톤 진위판별 문제 oc 외판원 (비방향) 진위판별 문제
해밀톤 회로 진위판별 문제의 사례 (『 29 를 같은 마디의 집합 VS 가지며 모든 마디 사이에
이음선이 있으며, 가중치는 다음과 같이 되도록 외판원 (비방향) 진위판별 문제의 사례 (< £’)
로 변환한다.
(u, 0) © Boye 1이고,
(u, 0) 2 Boye 8이다.

그림 9.6의 예를 보면 이해가 쉬워진다. VY, He 해밀톤 회로이다"는 “(^ )에 가중치의 합
이 n( Vol] 속한 마디의 개수)보다 크지 않은 여행경로가 있다“와 필요충분조건이다. 이 변환이

(4, 0) 의 가중치는 &

그림 9.6 예제 9.10의 변환 알
래프로. 변환한다:



===== PAGE 408 =====
© 예제 9.11

@eeeeee
9.4 NP 이론  397

다차시간임을 증명하는 작업은 연습문제로 남겨둔다.

별 문제의 다차시간 검증 알고리즘은 이미 작성하였다. 따라서 이 문제가 22^에
증명하고, 다음이 성립함을 증명하여 이 문제가 NP-CompleteyS 증명할 수 있다.
외판원 (비방향) 진위판별 문제 외판원 진위판별 문제
외판원(비방향) 진위판별 문제의 사례 (1; 2) 를 같은 마디의 집합 VS 가지며 (0, v) 가 Lol]
속할 때마다 이음선 <%, 04 >A < u>E 둘 다 "에 속하는 외판원 BA ARV, LS
변환한다. <u, 0 >와 < 4>의 가중치는 (4, 0) 의 가중치와 같다. “CV, 2) 에 가중치의 합이
0보다 크지 않은 비방향 여행경로가 있다"는 “( ^ )에 가중치의 합이 0보다 크지 않은 방향
여행경로가 있다"와 필요충분조건이다. 이 변환이 다차시간임을 증명하는 작업은 연습문제로 남
겨둔다.

앞에서 언급했듯이 예제 9.2에서 9.5까지의 문               수천 가지에 달하는
제가 축소변환을 사용하여 NP—Complete?°| 증명되었다 개리와 존슨의 si0070@
면 축소변환의 사례가 많이 나와 있으며, 3007} 2] 이상의 NP-Complete 문제를 소개하

있

El ih

=

NP2| 상태
그럼 9,30] 보면 P= NPY 진부분집합(60206 subset) O = 보이지만, 앞에서 언급했듯
이 동일한 집합일 수도 있다. NP-Complete 문제의 집합을 이 그림에 어떻게 끼워 넣을
까? 정의에 의하면 이 NWP-Complete 집합은 //7^의 부분집합이다. 따라서 프레스버거
산술 문제, 멈춤검사 문제, 그리고 ^/7?에 속하지 않는 다른 진위판별 문제는 NP-Com—
plete7} 아니다.

7/7에는 속하지만 NP—Complete= 속하지 않는 진위판별 문제는 무조건 "예"라고
대답하는(또는 무조건 “아니오"라고 대답하는) 사소한 진위판별 문제이다. 사소하지 않

P=NP                                     NP

NP-complete

NP-complete

확실히 여기 속하는
문제가 몇 가지 있다

무조건 "예"라고 대답하는 사소한
진위판별 문제는 여기에 속한다.
그림 9.7 집합 /《-는 왼쪽 그림일 수도 있고, 오른쪽 그림일 수도 있다.


===== PAGE 409 =====
@00@000000
398     chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개

© 예제 9.12

은 진위판별 문제를 사소한 진위판별 문제로 축소변환이 불가능하므로 사소한 진위판별
문제는 NP-Complete7} 아니다.

P= 772라고 가정하면, 그림 9.79] 왼쪽 그림이 맞다. Px NPY 오른쪽 그림이
맞다. 즉, 2 = NPA, 다음 등식이 성립한다.

P{\ NP-Complete = 2

여기서 NP-Complete= NP-Complete 문제들 전체의 집합을 나타낸다. Po] 속한 문
제가 하나라도 NP-Complete?}a1 한다면, 정리 9.1에 의하여 WPol] 속한 문제는 모두
다차시간에 풀 수 USS 암시할 것이므로 등식이 성립한다.

그림 9.7(오른쪽)에 의하면 그래프 동형사상 문제(37821 Isomorphism Problem)+= 다
음 집합에 속할 수 있음을 주목하자.

NP-—(PU NP-Complete)

(비방향, 방향 구별없이) 두 개의 그래프 S=(V, 4)와 G'=(V', #")는 다음 조건을
만족하면 FBAMHisomorphic) o}e}31 한다. AALS Vol] 속한 모든 마디 v, 3} vy of 대
해서 에서 『^으로 가는 일대일 함수 가 존재하고, 이음선 (4, v) 7} Lo} 속하고, 이
음선 (f(u), /(0))가 HO 속한다. 그래프 동형사상 문제는 다음과 같다.

그래프 동형사상 문제
두 개의 그래프 G=(V, HY G=(V, ^ )는 동형사상인가?

그림 9.8의 방향그래프는 다음 등식에 의해서 동형사상이다.
us= / (0)   ug= f (06)   u,= f (vs)   ug= f (v4)   Uy= f (vs)

그래프 동형사상 문제의 다차시간 AS 알고리즘을 작성하여 그래프 동형사상 문제가

그림 9.8 이 그래프는 동형사상이다.



===== PAGE 410 =====
© 예제 9,13

© 예제 9.14

© 예제 9,15

@0000000
9.4 NP 이론  399

202인지 증명하는 작업은 연습문제로 남겨둔다. /을 마디의 개수라고 할 때 "개의 일
대일 매핑을 모두 검사하면 쉽게 알고리즘을 작성할 수 있지만 시간복잡도가 지수보다도
높다. 아직 아무도 이 문제를 푸는 다차시간 알고리즘을 찾지 못했고, 아직 아무도 이
문제가 NP—Completet}al 증명하지도 못했다. 따라서 이 문제가 인지 알 수 없고
70/2-06002010[6인지도 알 수 없다.

PS 아니고 NP-Complete 아니면서 2에 속한 문제가 있는지 아직 증명하지 못
했다(이를 증명하면 Px NPE 저절로 증명하는 셈이다). 그러나 Nx NP    ie
문제는 반드시 존재한다는 사실은 중명되었다. 그림 9.7의 오른쪽 그럼으로 보여주는 이
AD: 다음 정리로 공식화할 수 있다.

> Bel 9.4
P+ NPO|A, 다음 집합은 공집합이 아니다.

NP-—(P UNP- Complete)

증명 : 증명은 FEU (Ladner)7} 논문(1975)을 참고하자.

대문
다음 두 문제 사이의 유사성을 살펴보자.

수 no] 대해서 7은 소수(0006 ㅁ47206602)인가?

합성수 문제
양의 정수 7에 대해서 7=1*가 성립하는 7 >1과 > 1인 정수 mah *가 존재하는가?

소수 문제는 9.282] 앞부분에서 알고리즘을 작성해본 문제이다. 소수 문제는 합성수
문제의 반대문제이다. 진위판별 문제의 BA] (complementary problem)= 원래 문제
가 “아니오"라고 대답하면 “예"라고 대답하고, 。예"라고 대답하면 “아니오"라고 뒤집어서
대답하는 문제이다. 상호보충 문제의 예를 또 하나 보자.

외판원 진위판별 문제의 반대문제
가중치 그래프와 양수 dol] 대해서 총 가중치가 0보다 크지 않은 여행경로가 없는가?



===== PAGE 411 =====
400

chapter 9 계산복잡도와 다루기 힘든 AS: NP 이론의 소개

a, 그 수가 소수인지도 판별할 수 있다. 그러나 BAS 푸는 다차시간 비결정 알고리즘
을 찾았다고 해서, 반대문제를 푸는 다차시간 비결정 알고리즘이 자동적으로 생기는 것
은 아니다. 즉, 문제가 NP 속함을 증명했다고 해서 반대문제도 //7에 속한다고 자동
으로 Sa abe, 외만원 asia 문제의 반대문제의 경우, 가중치의 Be) 4보다

크지 않은 여행경로가 없음을 다차시간에 검증하는 알고리즘을 작성해야 할 것이다. 이

문제는 가중치의 합이 0보다 크지 않은 여행경로가 있음을 aes |는 작업보다 훨씬 더
복잡하다. 아직 아무도 외판원 진위판별 문제의 반대문제를 검증하는 다차시간 알고리즘
을 만들지 못했다. 반대문제가 Peo] SBS] NP-Complete BARE 하나도 없다. 반
대문제가 MP7} 아님이 증명된 NP 문제도 하나도 없다. 정리하면 다음과 같다.

> Bel 9.5

NP-Complete 문제의 반대문제가 라면, NP 문제의 반대문제도 모두 Poth
증명 : 증명은 개리와 존슨의 책(1979)을 참조하라.

그래프 동형사상 문제와 소수 BAS 좀 더 얘기해보자. 앞에서 언급했듯이 그래프 동
형사상 문제를 푸는 다차시간 알고리즘을 아직 아무도 만들어내지 못했고, 그래프 동형
사상 문제가 //7^?-0000!066라고 아직 아무도 증명하지 못했다. 얼마 전까지만 해도 소수
문제도 마찬가지였다. 그러나 2002년 °}-1e}2}(Agrawal) 동료들이 소수 문제를 푸는
다차시간 알고리즘을 만들어냈다. 11.6절에서 그 알고리즘을 소개한다. 그 전 1975년에
Eze (Pratt)7} 소수 BA} NPUS 증명하였다. ee 반대문제인 합성수 문제도
772임을 증명하기 쉽다. 선형계획법(11068 Programming) 문제와 반대문제도 모두 MP
임이 증명되었고, 1979년에 차치안(2180180/이 다차시간 알고리즘을 개발하였다. 하지
만 그래프 동형사상 문제의 반대문제는 /2인지 아직 증명하지 못했다. 이 모두 결과를
미루어 보면, 그래프 동형사상 문제를 푸는 다차시간 알고리즘을 만들기보다 그래프 동
형사상 문제가 NP-Complete?]°] 증명될 확률이 더 높다. 아니면, 그래프 동형사상 문
제가 NP-(P U NP-Complete) 집합에 속하는 문제일지도 모른다.

9.4.3  NP-Hard, //2-ㄷ36, NP—Equivalent 문제

지금까지 진위판별 문제만 공부했다. 이제 지금까지 공부한 결과를 일반(00ㅁ06081020) 문

제로 확장하여 적용해보자. 정리 9.1에 의하면 진위판별 문제 AS 진위판별 문제 BS

다차시간 다일 SAS 가능하다면, 문제 #의 다차시간 알고리즘을 사용하여 문제 4
를 다차시간에 풀 수 있다. 이제 다음 정의를 통하여 일반 문제로 일반화해보자.

정의
=
문제 BS 푸는 가상 다차시간 알고리즘을 사용하여 문제 AS 다차시간에 풀 수 있다면, 문제 |



===== PAGE 412 =====
* 예제 9.16

@‥ㅎ00000 0
9.4 NP 이론  401

는 문제 FS 다차시간 튜링 SAWS ES(polynomial-time Turing reducible)S}C}i 한다
(보통 그냥 “AE 로 튜링 축소변환된다"라고 하기도 한다). 기호로는 다음과 같이 쓴다.

46072

이 정의에 의하면 문제 BS 푸는 다차시간 알고리즘이 반드시 있어야 할 BRE 없다.
단지 문제 BS 푸는 다차시간 알고리즘이 있으면 문제 AZ 다차시간에 풀 수 있다는
것을 말하고 있을 뿐이다. AS 2가 모두 진위판별 문제이면, 다음은 분명히 성립한다.

Ax Bolw A oc p BOltH,

이제 NP-Complete2] WAS 일반 문제로 확장하여 보자.

정의
임의의 NP—Complete 문제 A 에 대해서 다음 관계가 성립하면, 문제 BH NP-Hard 하다고
한다.

4607

튜링 축소변환이 ©} A (transitive)o] WSS 파악하기는 별로 어렵지 않다. 따라서
NP '문제는 모두 NP-Hard 문제로 축   조서베한 가능하다. 다시 말해서, “NP-Hard 문제
를 푸는 다차시간 알고리즘이 존재한다면 P= PF} 성립한다"는 의미가 된다.
그러면 어떤 문제가 NP-Hardo]] 속할까? NP-Complete 문제는 분명히 모두 NP-
Hard 문제이다. 최적화 문제를 푸는 다차시간 알고리즘이 있으면, 그에 상응하는 진위판
별 문제를 푸는 다차시간 알고리즘은 거저 얻을 수 있다고 언급한 바 있다. 따라서 “MP
Complete 문제에 상응하는 최적화 문제는 모두 MP-Hardo]t},” 다음 예제에서 튜링 축
소변환가능성의 정의를 정식으로 사용하여 외판원 문제가 ///^-188270임을 확인해보자.

외판원 최적화 문제는 NP-Harde|t},

외판원 최적화 BAS 푸는 가상의 다차시간 알고리즘이 있다고 가정하자. 그래프 6와 양의 정
수 를 포함하는 외판원 진위판별 문제의 사례가 주어진다고 하자. 이 가상 알고리즘을 그래프
Go} 적용하여 최적해 mindlseS 구한다. 그러면 진위판별 문제의 사례에 대한 답은 0 = mindist
이면 “아니오"가 되고, d> /04080이면 “예"가 될 것이다. 이 추가적인 절차와 함께 이 최적화
BAS 푸는 가상의 다차시간 알고리즘은 분명히 다차시간에 이 진위판별 문제를 푼다. 따라서
다음 관계가 성립한다.

외판원 진위판별 문제 > 외판원 최적화 문제

그러면 어떤 문제가 NP-Hardol] 속하지 않을까? 그러한 문제가 존재하는지는 알지
못한다. 사실, “NP-Hard7} 아님을 증명한 문제가 있다면, Px NPS 증명한 것과 다름


===== PAGE 413 =====
402

chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개

없다." 그 이유는 P= NPO|
|

SAS 모두 HH! 알고리즘으로 풀 수 있을 것이
기 때문이다. 그러므로 문저        로                                8

NP
를 푸는 가상의 다차시간 알고           그야
에 속한 문제를 모두 풀 수 있을 것이다. 따라서 모든 문제는 //7?-18820일 것이다.

반면에 다차시간 알고리즘이 있는 A NP-Hard7} 아닐지도 모른다. 사실, "다차
시간 알고리즘이 있는 문제를 //?-ㅁ370라고 증명할 수 있다면, P= NPS 증명한 것고
다름없다.” 그 이유는 어떤 NP-Hard 문제를 푸는 가상이 아닌 실제 다차시간 알고리
이 있을 것이기 때문이다. 그러므로 NP 문제를 NP-Hard 문제로 튜링 축소변환하
다차시간에 NP BAS 모두 풀 수 있게 된다.

그림 9.9는 NP-Hard 문제의 집합이 모든 문제의 집합에 어떻게 끼여 들어가는지 보
여준다.

NP-Hard BA (다차시간 알고리즘을 발견하는 희망의 정도로 비교하여) 최소한
NP -Complete 문제만큼 어렵다. 예를 들어, 외판원 최적화 문제는 최소한 ///?-00000106
문제만큼 어렵다. 그러나 A(reverse) = 사실일 필요가 있을까? 즉, NP-Complete 문제
가 최소한 외판원 최적화 문제만큼 어려울까? //7"-8870만 가지고는 대답할 수 없다.
Te 하나의 정의가 필요하다.

3
S

a
B
ㅎㅇ
BA

부

ae
tel

요

정의
정의
/^@에 속한 임의의 BO] 대해서 다음 관계가 성립하면, 문제 4는 //^-ㄷ86*라고 한다.

Ax,7B

명백히 “P= NP°|4, NP-Easy BARE 모두 다차시간 알고리즘이 존재한다.” NP-
888》의 정의가 NP-Hard2] 정의와 정확히 HAS 아님을 주목하자. “문제가 MP—Easy
CPE “그 문제가 NP-Complete 문제로 축소변환 가능하다"와 필요충분조건인지 증명하
는 작업은 연습문제로 남긴다.

어떤 문제가 //7?-0888》에 속할까? 명백히 Pol] 속한 문제들, NPo] 속한 BAS, 다차
시간 알고리즘을 발견한 일반 문제들은 모두 NP-Easy°|t}, NP-Complete 진위판별

ㅇ= NPO|S, 여기에

속하는 문제는 없다.

P+NPO|3H, 문제가
여기에 속한다.

NP-hard

NP-complete



===== PAGE 414 =====
© 예제 9.17

@000000 0
9.4 NP 이론  403

문제에 상웅하는 최적화 문제는 대부분 NP-EasyDS 증명할 수 있다. 그러나 다음 예
제에서 보듯이 증명이 쉽지는 않다.

외판원 최적화 문제는 NP-Easyo|t}, 이 결과를 얻기 위하여 다음 문제를 소개한다.

외판원 확장 진위판별 문제
외판원 진위판별 문제의 사례가 주어지고, 그 그래프 마디의 개수는 7이고 여행거리는 0라고
하자. 추가적으로, "개의 서로 다른 마디로 구성된 부분 여행경로(680081 tour) T7+ 주어진다
고 하자. 문제는 TSS 여행거리가 dS 넘지 않는 전체 여행경로로 확장할 수 있는지 판별하는
것이다. 이 문제의 파라미터는 외판원 결정문제의 파라미터에다가 부분 여행경로 7까 추가된다.
외판원 확장 진위판별 문제가 /\에 속하는지 증명하기는 그리 어렵지 않다. 따라서 다음 관계

가 성립하는지만 증명해보기로 하자.
외판원 최적화 문제 < , 외판원 확장 진위판별

이를 증명하기 위해서 외판원 확장 진위판별 문제를 푸는 가상의 다차시간 알고리즘을 polyarg
라고 하자. 20//8의 입력은 그래프, 부분 여행경로, 그리고 거리이다. 외판원 최적화 문제의
크기가 7인 사례 G7} 주어진다고 하자. 이 사례에서 마디는 다음과 같다고 하고,

{v,, Vg. ses v, }

수

저

da

다음과 같이 놓는다.
dmin=n
dmaz =n x maximum (v;, A] vj, 가는 이음선의 가중치)
Si /즈0
mindist7} 최적 여행경로에서 이음선의 총 가중치이면, 다음과 같은 부등식이 성립한다.
dmin < mindist < dmaz
여행경로의 첫째 마디로 뭘 선택해도 상관없으므로, <, 을 첫 번째 마디로 한다. 다음 호출을 4
각해보자.
polyalg(G, [v,], 0)

이 호출의 입력이 되는 부분 여행경로는 단순히 [v, Jolt}, 이것은 vf 떠나기 전 부분 여행경로
이다. 이 호출로 "ㅁㅠ06 를 넘겨줄 수 있는 do] 가장 작은 값은 0= 07707이고, 여행경로가 HAs}
는 경우, d=dmaro|4 이 호출로 확실히 “true’S 넘겨줄 것이다. d=dmaxY 때 "8186 를 넘
겨준다면, mindist = co, 그렇지 않으면, 이진검색을 사용하여 G2} [,]이 입력일 Wh polyarg7}
"ㅠ0@"를 WARE 가장 작은 4 값을 결정할 수 있다. 이는 최대로 polyargS 약 lgldnar)
호출하여 mindistS 계산할 수 있음을 의미하고, 이는 mindistS 다차시간에 계산할 수 있다는
의미가 된다.

일단 mindist 값을 알면, polyargS 사용하여 다음과 같이 다차시간에 최적 여행경로를 구축
할 수 있다. mindist =<이면 여행경로가 존재하지 않고, 따라서 작업이 끝난다. 그렇지 않으
면, 여행경로 [0,]은 가중치의 합이 71787086+인 여행경로로 명백히 확장 가능하다. [v,]o] 확장
가능하므로 [,, ,]가 확장 가능하게 되는 최소 하나의 v,7} 반드시 존재한다. 다음과 같이



===== PAGE 415 =====
@60600000
404     chapter 9 계산복잡도와 다루기 힘든 AWE: NP 이론의 소개

7000070를 최대로 7-?2번 호출하여 그러한 v,S 결정할 수 있다.
polyalg(G, [v,, v;], mindist)

여기서, 2<i<n-1, 확장 가능한 여행경로를 발견하거나, i7} 7ㅡ1에 도달할 때 멈춘다. 마
지막 마디를 빼고 다른 모든 마디가 모두 실패한 경우 마지막 마디는 반드시 확장 가능해야 하므
로 마지막 마디는 검사할 필요가 없다.

일반적으로 m 개의 마디를 가진 확장 가능한 부분 여행경로가 주어지면, 2000070를 최대로

m—-1H 호출하여 7ㅠ+1개의 마디를 가진 확장 가능 여행경로를 찾을 수 있다. 그래서
polyorg 최대로 다음 횟수만큼 호출하여 최적 여행경로를 구축할 + 있다.
(n—2) +---+(n—m-1)+---+1 ee

이는 다차시간에 최적 여행경로를 구축할 수도 있고, 다차시간 튜링 축소변환도 가능하다는 의
미가 된다.

예제 9.20114] 9.5까지에 있는 다른 문제들과 대부분의 WP-Complete 진위판별 문제
에 상응하는 최적화 문제에 대해서도 비슷한 방식으로 증명할 수 있다. 다음 정의는 그러
한 문제와 관련이 있다.

정의
‘|

문제가 NP-HardO|FHAY NP-EasyO|X NP-Equivalent2}i1

ro

다.

분명히, “P= 7/2"는 "모든 NP-Equivalent 문제를 푸는 다차시간 알고리즘이 존재한
다"와 필요충분조건이다.

이론을 진위판별 문제로만 제한해도 일반성을 상실하지는 않는다. 왜냐하면, wP-
Complete 진위판별 문제에 상응하는 최적화 문제가 NP-Equivalent=}al 증명할 수 있
기 때문이다. 즉, ae 문제를 를 푸는 ae eSieare 찾는 것은 진위판별 문제를
푸는 다차시간 알고리즘을 찾는

이 장의 SHE NP 이론을 < reps 소개하는데 ron  더 세부적으로 공부하려면,
이미 여러 번 chet 적 있는 개리와 존슨의 sien 바란다. 그 책이 나온
지 꽤 오래되기는 했지만 NP 이론을 상세히 공부할 수 있는 최고의 책으로 꼽힌다. Pa—
padimitriouS] 책(1994)도 입문서로 괜찮다.

@ 9.5 NP-Hard 문제를 푸는 방안

NP-Hard 문제를 푸는 다차시간 알고리즘이 없는데, 그러한 문제를 풀고 싶으면 어떻게
해야 할까? 5장과 6장에서 이미 한 가지 방법을 공부했다. 공부한 되추적과 분기한정 알
고리즘들은 모두 최악의 경우 다차시간이 아니다. 그러나 현장에서 꽤 효율적으로 쓰인



===== PAGE 416 =====
© 예제 9.18

9.5 NP-Hard 문제를 푸는 방안     405

다. 따라서 되추적이나 분기한정 알고리즘으로 충분할 수도 있다. 5.3절에서 특정 사례
에 대하여 알고리즘이 효율적일지를 몬테칼로 기술을   사용하여 추정할 수 USS STR
다. 효율적일 것으로 추정되면, 알고리즘을 사용하면 된

NP-Hard 문제의 일부 사례에 대해서만 효율적으로 작동하는 알고리즘을 찾는 방법

있다. 예를 들어, 6.8절에서 공부한 신뢰 네트워크의 확률적 추론 문제는 NP-Hard
wick 일반적으로 신뢰 네트워크는 방향 비순환 매가 버어 acyclic graph) 2} 확률
포로 구성되어 있다. 그래프가 단일경로로 연결된 경우에 aca   작동하는 다차시간 일
BSS 이미 발견하였다. 마디를 연결하는 Bar} 하나뿐인 방향 비순환 그래프를 단
일경로로 AA(singly connected) =]O] 있다고 한다. 세부 알고리즘은 26941의 책(1988)과
Neapolitan®] 책(1990)을 참고하기 바란다.

이 장에서 설명할 셋째 방법은 근사 알고리즘(60070×1013816 algorithm)°]t}, WP-Hard
최적화 BAS 푸는 근사 알고리즘은 최적해를 얻는다는 보장은 없지만 최적에 상당히
가까운 해를 내준다. 구한 해가 얼마나 최적에 가까운지를 보장해주는 범위값을 얻을 수
도 있다, 예로써, 외판원 최적화 문제 변종을 푸는 근사 알고리즘을 만들어보자. 근사 알
고리즘의 해를 minapproxt} 하고 mindistS 최적해라고 하면, 다음 부등식이 성립함을

증명할 수 있다.

ne   A

Ae
re

a

minapprox < 2X mindist

여기서 minapprox7t 언제나 거의 mindist2} 9배는 아니다. mindistol) 아주 가깝거나
아예 같은 경우가 A 많이 나타날 수도 있다, 220042000×가 200080의두 바는 절대로
되지 않음을 보장한다는 의미로 해석하는 편이 오히려 맞다. 일단 알고리즘을 만들고 개
량해보자.

삼각형 부등식을 만족하는 외판원 문제
다음 조건을 만족하는 가중치가 있는 비방향그래프 G=(V, 2^")가 있다고 하자.
1, USS 모두 이음선으로 연결되어 있다.
2, Wu, 0) 를 마디 ul] 마디 oS 연결하는 이음선의 가중치라고 하면, 다른 모든 마디 에
대하여 다음 부등식이 성립한다.
Wu, v) < Wu, y) + Wy, v)

삼각형 부등식(01808418『 inequality)°]@}31 하는 둘째 AAS 그림 9.10에 나타나 있다. 가중치
가 도지 사이의 실제 거리를 ( 일직선으로 ) ※현한다면 이 부둥식은 만족된다. 가중치 그래프에
서 "가중치"와 "거리"는 같은 의미로 사용되는 용어임을 주목하자. 첫째 AAS 모든 도시를 연결
하는 양방향 도로가 WSS 암시한다.


===== PAGE 417 =====
@‥ㅎ00000 0
406

그림 9.10 삼각형 부

“Hal's 더한 값보다 크지 않다.

외판원 문제는 출발과 도착 마디가 동일하고, 다른 모든 마디를
최단 경로(최적 여행경로)를 찾는 문제이다. 이 예제에서 살펴본
임을 증명할 수 있다.

chapter 9 계산복잡도와 다루

AS: NP 이론의 소개

HEA

식에 의하면 wold ?로의 "거리"는 wold 로의 "거리"에다 yO *로의

각각 정확히 한 번씩 방문하는

아어
변종도 마찬가지로 NP-Hard

이 변종 문제의 그래프는 방향이 없

ojo 909 2
muse

Ni

주목하자. 그래프의 최적 여행경로에서 어떤

이음선이라도 하나 제거하면, 최소비용 신장트리가 된다. 그러면 최소비용 신장트리의

주

애

하나뿐이면서 이미 방문한 마디인
러간다. 삼각형 부

9.11(0)은 이 기술
출발하였

에서
디에서

방금 설명한 방법은 다음과 같이 요약할 수

:  tele 최적 oes 총 가중치

=ojlo

cS

얻은 경로는

Ea “oO

그림 9.11(0)이다.
택해서 마

단하여

채보 }(shortcut)”"-&                      =F

Ad

=
4

때 그냥 가장 가까운 마디를

방문한다.
부등식에 의해서 지름길이 경로를 더 2
술을 사용하여 구한 여행경로이다.
는데, 결과로 얻어진 여행경로가 최적은
출발하면 최적 여행경로를 얻는

있다.

, 임의의 마디에서 출발하여 경로를 가로지르는데, 차례로 빙
다. 가로지르는 동안 현재 마디와 인접해

길거

이 그림에서

보다 작아야 한다. 알고리즘 4.1이나 4.8를 사용
수 있다,  Al ]장트 트리를 두
emis 방문하는 ARE 바꼴 수 있다. 이 과정은 그림 9.1에서 보여준

는 그래프이고, 그 그래프의 최소비용 신장트리는 그림 9. eee 1

번 횡단함으로써 그

그림을 보면 일부
번 이상 방 HE

미머는 주

문하지 않는 경로로
}문하지 않은
있는 방문하지 않은 마디가

현재 마디에 인접해 있는 마디가

경우, 지름길을 통해서 다음 방문하지 않은 마디로 질

게 만들지 않음이 보장된다. 그림
왼쪽 맨 아래에 있는 마디
아니다. 하지만, 왼쪽 맨 위의 마

구축한다.
여행경로)를 구축한다.

==
SS
로(즉
(주

a   cl

출발 마디에 관계없이 반드시 최적은



===== PAGE 418 =====
@
1 @
| @
@
@
@
@

95 NP-Hard 문제를 푸는 방안     407

아니다. 그러나 다음 정리로 구한 여행경로가 최적에 가까움이 보장된다.

> Bel 9.6

mindistS 최적 여행경로의 가중치 합이라 하고, minapproxS 방금 설명한 방법을 사용하여
구한 여행경로의 가중치 합이라고 하자. 그러면, 다음 부등식이 성립한다.

minapprox <2 mindist
증명 : 이미 공부했듯이 최소비용 신장트리의 가중치 합은 mindist Ar} 작다. minappros 2]
총 가중치는 두 개의 최소비용 신장트리의 가중치 합보다 작으므로, 이 정리는 성립한다.

minapproxS 2 ×7728720767에 임의로 가까워지게 할 수 있다는 사실을 보여주는 사례
를 만들 수 있다. 따라서 일반적으로 정리 9.0에서는 가능한 최선의 범위를 구한 것이다.
더 좋은 근사 알고리즘을 만들 수도 있다. 위에서와 마찬가지로 최소비용 신장트리를
먼저 구한다. 그리고 홀수개의 이음선에 연결되는 모든 마디의 집합 를 생각해보자.
그 마디의 개수는 짝수개가 틀림없음을 보이기는 어렵지 않다. 에 속한 마디들을 각



===== PAGE 419 =====
@0000000
408    chapter 9 계산복잡도와 다루기 힘든 ANP 이론의 소개

마디가 정확하게 다른 하나의 마디와 쌍이 되도록 AS 맞춘다. 이런 식으로 마디의 쌍을
만드는 것을 ^ 의 짝지움(0ㅁ+0408/이라고 한다. 각 마디의 YS 연결하는 이음선을 신
장트리에 추가한다. 그러면 각 마디는 이어져 있는 이음선의 개수가 짝수이므로, 결과로
나옴 경로는 모는 EAS 방문환더. 더구나; 의 형로에시 의음신의 총 개수는 드러들 두
번 횡단하여 구한 총 개수보다 크지 않다(대부분 작다). 그림 9.12(8)는 최소비용 신장:
리이고, 그럼 9.12) 한 번 짝지운 트리에서 구한 경로이고, 크림 9.12(0)는 지름길
택한 우에 구한 eee:

^ 의 최소가중치 짝지움(0ㅁ101081 weight matching)2 짝지워서 구한 이음선의 총 가
중치가 최소가 되는 트리이다. Se|(Lawler)2] 책(1976)을 보면, 다차시간에 최소가중치
짝지움을 구하는 방법이 나와 있다. 예제 9.18의 외판원 문제 변종을 다음 절차로 다차시
잘에 BS S 주 있다.

1. 최소비용 신장트리를 구한다.
2, Vol] 속한 마디의 최소가중치 짝지움을 구한다. 여기서 는 홀수개의 이음선
에 연결되는 신장트리에서 마디의 집합이다.
3, 짝지워진 마디를 연결하는 이음선을 트리에 추가하여 모든 마디를 방문하는 경로
를 구축한다.
4. ABD 택하여 마디를 두 번 방문하지 않은 경로(즉, 여행경로)를 구축한다.

그림 9.1204 실제 가중치를 보여주지 않은 채 이 ARES 설명한다. 이 방법이 앞에서
공부한 첫째 방법보다 더 좋다는 사실을 다음 정리를 공부하면 알 수 있다.

‘

m

illo |

no 27

(a) 최소비용 신장트리           (6) 마디는 짝지워지고,                    (0) 지름길을 택한다
이음선은 트리에 추가된다.

ole =

그림 9.12 짝지움을 사용하여 구한 여행경로



===== PAGE 420 =====
0 000000
95 NP-Hard 문제를 푸는 방안     409

> 정리 9.7

mindistS 최적 여행경로의 가중치 합이라 하고, minapprox2S 최소가중치 짝지움을 사용하
여 구한 여행경로의 가중치 합이라고 하자. 그러면, 다음 부등식이 성립한다.

minapprox2 < 1.5 X mindist

증명 : 홀수개의 이음선에 연결되는 BE 마디의 집합을 라고 하자. 최적 여행경로를 "에
속하지 않는 마디는 그냥 지나치고 에 속한 마디들만 연결하는 경로로 바꾼다. 삼각형 부
등식에 의해서 이 경로의 총 가중치는 mindist Ar} 크지 않을 수 있다. 더구나, 이 경로를 가
지고 다음과 같이 『^에 속한 마디들에 대해서 두 가지 방법으로 짝지울 수 있다. 「^에 속한
임의의 마디를 선택하고, 그 마디를 경로 상에 한쪽 Aol] 있는 마디와 BS 지운다. 그리고
같은 방향으로 계속해서 인접 마디들을 짝지운다. 이게 첫째 짝지움이다. 다음에 초기 마디와
경로 상에 다른 쪽 옆에 있는 마디와 짝지우고, 계속해서 그 방향으로 인접 마디들을 짝지운
다. 이게 둘째 짝지움이다. 이 두 짝지움의 이음선은 경로 상 모든 이음선을 이루게 되므로,
이들 총 가중치 합은 경로의 가중치와 같다. 따라서 최소한 두 짝지움 중 하나는 가중치 합이
경로의 가중치의 반보다 크지 않다. 이 BH] 가중치가 mindist Br} 크지 않고, 어떤 짝지움
의 가중치도 최소가중치 짝지움의 가중치만큼은 최소한 크므로, 다음과 같은 범위를 얻는다.

minmatch < 0.5 × mindist

여기서 minmatcht= 최소가중치 짝지움의 가중치이다. 최소가중치 짝지움의 가중치는 mindist
보다 작다. 최소가중치 짝지움 방법의 단계 8에서 구한 이음선은 신장트리의 이음선과 최소
짝지움으로 구한 이음선으로 구성되어 있으므로, 이 이음선들의 총 가중치는 1.5% mindist
다 작다. 이제 단계 4에서 구한 최종 여행경로에서 이음선의 총 가중치는 단계 3에서 구한 경
로의 이음선 가중치보다 크지 않으므로 이 정리는 성립한다.

근사치가 1.5 x mindist ol] 임의로 가까워지도록 사례를 만들 수 있다. 그러므로 정리
9.1에서 구한 것보다 이 알고리즘에 대한 더 좋은 범위는 일반적으로 없다.

외판원 낸시가 외판원 문제를 푸는 분기한정 알고리즘(알고리즘 6.9)을 사용하여 40개
도시 판매영역에 대한 최적 여행경로를 마지막으로 찾으려 했음을 상기하자. 그 알고리
Se 최악의 경우 다차시간이 아니므로, 그 문제를 푸는데 수년이 걸릴지도 모른다. 낸시
가 방문해야 하는 도시 사이의 거리가 삼각형 부등식을 만족하는 외판원 문제의 가정을
만족한다면, 그녀는 마침내 해답을 구할 수 있는 대체안이 생긴 셈이다. 즉, 최소가중치
짝지움 방법을 사용하여 최적 여행경로의 아주 가까운 근사 여행경로를 다차시간에 구할

수 있다.

9.5.2 상자 채우기 문제를 푸는 근사 알고리즘

새로운 문제를 하나 소개한다.


===== PAGE 421 =====
@eeeee @e
410     chapter 9 계산복잡도와 다루기 힘든 정도 NP 이론의 소개

© 예제 9.19    상자 채우기 44] (Bin Packing Problem)
크기가 다음과 같은 "개의 아이템이 있다고 하자.
915 908 ~ Sy
여기서 6,의 범위는 0 < &, 흐1이다. 그리고 여러 상자에 아이템을 채운다고 가정하자. 여기서
각 상자의 용량은 1이다. 이 문제는 아이템을 모두 채우는데 필요한 상자의 최소 개수를 구하는
문제이다.

이 문제는 4/7?-ㅁ840임이 증명되었다. 이 문제를 푸는 아주
"차례로 채우기(6786 110)" 라고 한다. 차례로 채우기 전략은 첫째 상자에 아이템을 넣는다.
상자에 들어가지 않으면, 새 상자를 사용한다. 큰 아이템부터 차례대로 아이템을 상자에
놓으면 더 중을 at. 의 “Zt 아이템부터 차례로 채우기(ㅁㅠ0ㅁ1007088108 first—

60"라고 한다. 이 알고리즘을 추상적으로 기술하면 다음과 같다.

아이템을 큰 것부터 차례로 정렬한다;
while (아직 채우지 못한 아이템이 있다) {
다음 아이템을 집는다;
while (아이템이 상자에 들어가지 않고, 새 상자가 있다) {
다음 상자를 집는다;
if (아이템이 상자에 알맞게 들어간다)

상자에 아이템을 넣는

Ee oe

}
if (Of} Ro] 상자에 들어가지 않는다) {
새 상자를 가져온다;
아이템을 새 상자에 넣는다;
}
}

이해해보자. 이 알고리
2 주목하자. 즉 즉, 탐욕스럽게
이 알고리즘을 상세히 작성

Bs      By

템부터 차례로 채우기를 적용한 결과



===== PAGE 422 =====
9.5 NP-Hard BAIS 푸

하그의 ee   O(n’) AS 증명하는 작업은 연습문제로 남긴다. 그림 9.139] 해답
은 최적이 아님을 확인하고 넘어가자. 크기가 0.5인 아이템과 0.8인 아이템과 0.8인 아이
템 중 하나를 두 번째 싱    }자에, 크기가 0.4인 아이템 2개와 0,291 아이템 하나를 세 번째
상자에 넣으면, 상자 세 개만 가지고 아이템을 모두 채울 수 있다.

근사해가 최적해에 얼마나 가까운지 범위를 구해보자. 이 범위는 정리 9.8에서 얻는
다. 그 정리를 증명하기 위해서 다음 보조정리 2개가 필요하다.

| *보조정리 9.1

opt 상자 채우기 문제의 주어진 사례에 대한 최적의 상자 개수라고 하자. 큰 아이템부터 차
례로 채우기 전략으로 여분의(6008) AHS, opt Act 큰 인덱스의 상자)에 채운 어떤 아이템
도 크기는 기껏해야 1/3이다.

< 증명 : 7를 (opt +1) Al 상자에 넣게 되는 첫 번째 아이템의 인덱스라고 하자. 아이템은 큰 것부
터 차례로 정렬되어 있으므로, 다음 범위가 만족하는지 보이면 된다.

1

a &

Bee 유도하기 위해서 6, > 1/3이라고 가정하자. 그러면,

Si So) eee?  Sh iro 모두   그보다 크다.

이는 opt ry 크지 않은 인덱스를 가진 상자는 모두 기껏해야 아이템이 개씩 들어있음을 으
미한다. 그러한 상자에 모두 아이템이 두 개씩 들어있다면, 최적해에서는 처음 ＊-1개 아이템
중 두 개가 모든 상자에 들어있어야 할 것이다. 그러나 그들의 크기는 모두 극보다 크므로,
그 상자에는 5,7} 들어갈 자리가 없을 것이다. 따라서 opt ct} 크지 않은 인덱스를 가진 상자
하나는 최소 한 개의 아이템만 들어있을 것이다. 02보다 크지 않은 인덱스를  in ! 모든 상자
에 아이템이 한 개씩만 들어있다면, 어떤 두 개도 한 상자에 같이 들어갈       , 8째 아이템
은 그 중 어떤 것과도 같은 상자에 들어갈 수 없을 것이다(그렇지 않다면,        = aL
하나의 상자에 넣었을 것이다). 그러나 그렇다면 최적해로서 상자가 opt AC} 더 많이 필요
하게 될 것이다. 따라서 opt htc} 크지 않은 인덱스를 가진 최소한 하나의 상자에는 아이템이
두 개 들어있다.

처음 )개 상자에 아이템을 하나씩 넣고, HS opt—j7H 상자에 아이템을 두 개씩 넣게 되도
= 0 < 7 < optS 만족하는 57} 존재함을 증명한다. 이게 사실이 아니라면, ,에 아이템이 두
개 있고, B,, el 아이템이 ah 9 있게 되도록 k<m& 만족하는 상자 2,와 B,, 이 존재할 것이
다. 그러나 아이템을 큰 것부터 차례로 넣기 채우므로, 2,,에 채워진 아이템은 2,에 채워진
첫째 아이템보다 크지 않을 것이고, 6,는 에 채워진 둘째 아이템보다 크지 않을 것이다. 따
라서 B, AM 들어있는 아이템 크기의 합과 6,는 Bo] SME 아이템 두 개의 크기의 합보다
크지 않을 것이다. 이는 6,가 B, 4 맞게 들어가리라는 의미가 된다. 따라서 위의 (/에 관



===== PAGE 423 =====
412

chapter 9 계산복잡도와 다루기 힘든 정도: 이론의 소개

A 상자에는 9+1, 912, . . . ,Si-4
중 2개의 아이템이 들어감
— oar,
sy          Sj         Sit
B,         B         Bias        Bopt

그림 9.14 8, > 1/3이면, 알고리즘이 이 그림과 같이 상자를 채울 것이다.

한) 억측은 사실임이 틀림없고, 이 상자들은 그림 9.14에 나타나 있다.

최적해가 주어진다고 하자. 그 해에는 처음 )개 아이템이 )개의 서로 다른 상자에 들어 있다.
왜냐하면, 그 중 하나라도 상자 하나에 같이 들어가게 되면 같은 상자에 넣었을 것이기 때문이
다. 더구나, 다음 아이템들은 남은 opt—j7h 상자에 들어있다,
왜냐하면, 그 중 아무 것도 처음 )개 상자에 맞지 않기 때문이다. 알고리즘은 이 아이템을 두
개씩 (opt—j) 7 상자에 넣으므로, 이러한 아이템이 3×(0#-))개 반드시 존재한다. 이 아이
템의 각각 크기는 1/8보다 크다고 가정했으므로, 남은 (0/『-))개 상자 중 어느 하나에도 37}
를 같이 넣을 수 없다. 이는 이 상자에 각각 아이템이 정확히 두 A 들어있어야 한다는 Eo]
다. 3,9] 크기도 1/8보다 크다고 가정했으므로 두 개의 아이템씩 들어있는 0-)개 상자에
채울 수 없다. 더구나, 처음 )개 아이템이 들어있는 상자들 중 하나에도 채울 수 없다. 왜냐하
면, 그 아이템 하나라도 채울 수 있게 되면 알고리즘이 그렇게 했을 것이다. 이 해가 최적해라
고 가정했으므로 《,는 반드시 상자 중 하나에 들어 있고, 이는 모순이다. 따라서 증명이 완료
되었다.

*보조정리 9.2

opt 상자 채우기 문제의 주어진 사례에 대한 최적의 상자 개수라고 하자. 큰 아이템부터 차
례로 채우기 전략으로 여분의 상자에 채운 아이템의 개수는 기껏해야 0ㅡ1이다.

증명 : 모든 fe] Ao] opt7 상자에 들어가므로, 다음 부등식이 성립한다.
Sm < opt
i=1

BES 유도하기 위해서 근사 알고리즘은 opt 7H 아이템을 여분의 상자에 채운다고 가정하자.
1 50 … Zope EL 아이템들의 크기라 하고, 1 = i < opto] 범위에서 10《를 알고리즘이 상자



===== PAGE 424 =====
@‥6@00600000
95 NP-Hard BAIS 푸는 방안  413

Bol 채우는 총 크기라고 하자. 그러면 다음 부등식은 반드시 성립한다.
tot; +z; >1

왜냐하면, 그렇지 않은 경우 크기 (의 아이템이 Bo} 채워질 수 있기 때문이다. 따라서 다음
식이 성립한다.

n      opt      opt     opt            opt
a = S at) e = S (open) > ee
3=1     t=1            1=1           2=1

이 사실은 증명의 앞부분에서 보여준 것과 모순이 된다. 따라서 증명이 완료되었다.

> Bel 9.8
optS 니시 채우기 문제의 사례에 대한 ns 상자 개수라고 하자. = 아이템부터 차례로 채
우기 알고리즘에 의해서 사용된 상자의 개수를 4227@2라고 하자. 그러면,
approx < 1.5 x opt
증명 : 보조정리 9.1과 9.9에 의해서 큰 아이템부터 차례로 채우기 알고리즘은 각 아이템의
크기가 최대로 증인 아이템을 여분의 상자에 AS opt—174 채운다. 그러므로 여분의 상자
의 개수는 *=  ' 1, 또는 3일 때 최대로 다음과 같다.

_   그 |_ | 00 _ 906 1
(op xs 3 |  3

“의 가능한 가장 큰 값을 취하면 여분의 상자의 HSE (opt+1)/3 Bc AAU 같다. 이는
음 부등식이 성립함을 의미한다.

0020 1

approx < opt+    3

approx _        opt + (opt +1 )/3_       4          ik

opt            opt          3 3opt
이 비율은 opt =10)H 최대가 된다. De opt =19 때 근사 알고리즘은 상자를 하나만 사용
하므로 최적이다. 이는 07/『=2를 취하여 비율을 최대화 할 수 있고, 다음과 같이 결론지을 수

있다.

approx 4, 1 _3
ope 3 3x2 2

비율이 정확히 3/27} 되는 임의로 큰 크기의 사례를 만들 수도 있다. 따라서 일반적으
로, 정리 9.8에서 구한 범위를 개량할 수 없다.

근사 알고리즘의 질을 더 잘 평가하는 aan 근사 알고리즘으로 구한 해와 최적해
를 비교 실험하는 방법이 있다. 상자 채우기 문제를 푸는 근사 알고리즘은 여러 개의 큰


===== PAGE 425 =====
414

chapter 9 계산복잡도와 다루기 힘든 정도 = NP 이론의 소개

nao 대해서 철저히 검사되었다. 최적해를 보장하는 다차시간 알고리즘이 없는데(즉,
UNE 시간에 큰 7:값에 대한 AAAS 구할 수 없는데) 어떻게 이 실험이 가능한지 의아
해할 지 모르겠다. 사실, 그러한 알고리즘이 있다면, 근사 알고리즘은 애초부터 고려조차
하지 않았을 것이다. 이 파라독스(0878003/에 대한 대답은 상자 채우기 문제의 경우 근사
해의 질을 알아내기 위해서 실제로 최적해를 구할 필요는 없다는데 있다. 실제로 근사
알고리즘이 사용하는 미사용 공간(빈 SWI 용량을 계산할 수 있다. 그 알고리즘이 Ap
용하는 여분의 상자 개수는 미사용 공간의 용량보다 클 수가 없다. 왜냐하면, 근사해의
아이템을 여분의 상쟈를 비우고 최적의 개수의 상자에 들어가도록 재배치할 수 있다. 이
최적해의 미사용 공간과 여분 상자의 총 공간의 BES 합하면, 근사해의 미사용 공간의
용량과 같다. 따라서 여분 상자의 총 공간이 여분 상자의 개수와 같으므로, 여분 상자의
개수는 근사 알고리즘에서 미사용 공간의 용량보다 클 수 없다.

입력크기가 128,000이고, 아이템의 크기가 OF} 1 사이에 균등하게 분포되어 있도록 하
여 실시한 실험연구에서 근사 알고리즘은 평균적으로 64.000개의 AHS 사용하였고, 평
균적으로 미사용 공간이 100개 정도 되었다. 이는 평균적으로 여분의 상자의 개수는 이
연구 사례로 100개 정도가 상한임을 의미한다. 정리 9.8이 암시하는 바에 따르면 64,000
의 근사해에 대하여 다음 부등식이 성립한다.

64,000 < 1.5 x opt

이를 정리하면, opt > 42,666 °]a1, 여분의 상자의 개수는 21,334보다 크지 않다. 이 A
험 연구가 제시하듯이 평균적으로 이 알고리즘은 상한보다 성능이 훨씬 좋다는 것을 ot

관심 있는 특정 사례를 골라서 근사 알고리즘으로 얻어낸 해답에서 미사용 공간의 용
을 계산할 수 있다. 이렇게 하여 그 사례에 대하여 그 알고리즘의 성능이 얼마나 좋은
지 결정할 수 있다

ads

근사 알고리즘의 사례를 더 보고 싶은 독자는 개리와 존슨의 책(1979)을 참조하기 바란다.

9.1-9.3절
1. 다차시간 알고리즘이 있는 문제 3개를 나열하시오. 그리고 왜 그런 답이 나오는지 이유를
설명하시오.

2. 문제 하나와 그 문제의 입력에 대한 기호화 방법을 두 가지 제시하시오. 제시한 기호화 방법
을 사용하여 성능을 표현하시오.

3. 사례의 크기를 재는 기준으로 마디의 ASS 사용하는 그래프는 이음선의 개수를 사용하는
그래프와 다항식으로 표현하여(601"00040819) 동일함을 증명하시오.



===== PAGE 426 =====
4. 번째 피보나찌 수를 계산하는 문제는 9.8절에서 논한 세 가지 일반 카테고리 중에서 어느
것에 속하는가? 왜 그런 Fo] 나오는지 이유를 설명하시오

5. 、“그래프가 오일러 회로(08168 04704이다"는 “(8) 그래프가 연결되어 있고, (b) 모든 마디의
degree7} 짝수이다"와 필요충분조건이다. 그래프가 오일러 회로인지 판별하는 모든 알고리
즘의 시간복잡도의 하한을 찾으시오. 9.3절에서 논한 세 가지 일반 카테고리 중 어느 것이
이 문제에 속할까? 왜 그런 답이 나오는지 이유를 설명하시오.

6. 9.8절에서 논한 세 가지 일반 카테고리 각각에 속하는 BAS 최소한 두 개씩 나열하시오.
9.4절

7. 9.4절에서 공부한 외판원 진위판별 문제 검증 알고리즘을 구현하고, 그 알고리즘의 다차시
간 Ves 원구하시오.

ie

8. 예제 9.2014] 9.5까지의 문제들은 모두 MPO] 속함을 증명하시오.
9. 파벌 진위판별 문제에 대한 다차시간 검증 알고리즘을 작성하시오.
10. @0-만족가능도 문제를 파벌 결정문제로 다차시간에 SAW 가능함을 보이시오.

11. 해밀톤 회로 결정문제의 다차시간 검증 알고리즘을 작성하시오.

12. ALE 회로 결정문제를 외판원(비방향) 결정문제로 다차시간에 축소변환 가능함을 보이
시오.
13. 외판원(비방향) 결정문제를 외판원 결정문제로 다차시간에 축소변환 가능함을 보이시오.

14. “문제가 NP-Easy°|t}"= "문제가 NP-Complete 문제로 축소변환된다"와 필요충분조건임
oO.

15. 문제 AS} 문제 #가 다른 진위판별 문제라고 가정하자. 그리고 문제 AL 문제 Be 다차시
간 다일 축소변환 가능하다고 가정하자. 만약 문제 4가 ^/2^-06021066라면, 문제 Bu NP
- Complete?]7}? 왜 그런 Fo] 나오는지 이유를 설명하시오.

16. CNF-Satisfiability 문제의 모든 사례가 절 하나에 리터럴이 정확히 3개씩 있을 때 3-88-
tisfiability 문제라고 한다. 3-Satisfiability 문제가 ///"-06070126임을 알고, 그래프 3색 칠
하기 문제도 NP-Complete$-S 보이시오.

17. 어떤 문제가 세 속하지 않다면, 그 문제는 NP-Rasy7} 아님을 보이시오. 따라서 프레스
버거 산술 문제와 멈춤검사 문제는 NP-Easy7} 아니다.

18. 외판원 문제를 푸는 근사 알고리즘을 구현하여 실행해보고, 여러 개의 문제 사례를 가지고

19. 9.5.8절에 주어진 상자 채우기 문제를 푸는 근사 알고리즘을 자세히 작성하고, 시간복잡도
가 O(n”) YS 보이시오.

20. 5장에서 SHR 부분집합의 합 문제에 대하여 다차시간에 실행되는 근사 알고리즘을 개발
할 수 있는가?



===== PAGE 427 =====
416

chapter 9 계산복잡도와 다루기 힘든 정도 :4ㅁ 이론의 소개

21. CNF-Satisfiability BAIS 최적화 Bale 놓고(즉, Ze] 되는 절의 HES 가능한 최대로
하는 표현식의 리터럴의 At AUS 찾는 문제로 놓고), 이 문제를 푸는 근사 알고리즘을

개발할 수 있는가?

추가 문제
22. 임의의 알고리즘이 하나의 기호화 방법을 사용하여 문제를 풀면 다차시간 알고리즘이 되고,
른 기호화 방법을 ping 같은 GAS 풀면 지수시간 알고리즘이 될 수 있는가? A

그런 답이 나오는지 이유를 설명하시오.

23. 9.4, 240A] 주어진 verify-composite 함수를 푸는 상서
다차시간 알고리즘임을 보이시오

24. 그래프에 degree7} 25 넘는 마디가 없다고 가정하고, 비방향그래프에 해밀톤 회로가 존재
하는지를 검사하는 다차시간 알고

25. 하노이 탑 문제가 NP—Complete?l7}? 이 문제가 //7"-8887인가? 이 문제가 NP-Hardel
가? 이 문제가 //7"-080417816파인가? 왜 그런 Fo] 나오는지 이유를 설명하시오. 이 문제는
8장의 연습문제 17에 기술되어 있다.

26. 개 양의 Ane 짝수) 리스트가 주어졌을 때 나눈 두 개의 부분 리스트 정수의 합의 차이
가 최소가 되도록 리스트를 두 부분 리스트로 나누는 문제를 생각해보자. 이 문제가 WP
—Complete?l7}? 이 문제가 NP-Hard?l7}?



===== PAGE 428 =====
]   SEvolution)= 개체군(집단)의 유전적 구성의 변화 과정이다. 2-47 ey (Natural
Le 861!600020)이란 환경적 압박에 적응할 수 있도록 해주는 SYS 가진 생물체가 다
른 생물체들에 비해 더 많이 생존하고 더 많이 자손을 남기면서, 그 유리한 변이를 미래의
후손들에게 전하는 과정이다.
진화 계산(087014[10ㅁ87 computation) 2 자연선택론의 진화 메커니즘을 패러다임으
로 채용하여 최적화 문제들의 근사해를 구하는 것이다. 진화 계산은 유전 알고리즘, 유전
프로그래밍, 진화 프로그래밍, 진화 전략의 네 분야로 나눈다. 이 장에서는 첫 두 분야를
자세히 설명한다. 이런 알고리즘을 어떻게 구상하게 되었는지 맥락을 Bo]H7] 위해 유

전학을 먼저 간단히 공부해보자.

10.1 유전학 리뷰

유전학은 이미 공부했다고 가정하고 간단하게만 복슴해보자. 유전학 입문서로는 An
Introduction to Genetic Analysis (Gritffiths et al,, 2007) 또는 Essential Genetics

(Hartl and Jones, 2006)3 추천한다.
YS) (organism) = 식물이나 동물과 같은 개별적인 형태의 살아있는 유기체이다. 하


===== PAGE 429 =====
418

@
chapter 10 유전 알고리즘과 유전

:

래밍

나의 세포(60)는 생물체의 기본 구조와 기능을 이루는 단위이다. B29] (chromosome)
는 생물학적으로 표현된 유전적 특성을 가진 운반체(63ㅁ060)이다. 게놈(66ㅁ02786)이란 유
기체 하나에 들어있는 염색체 AAS 일컷는다. 인간의 게놈에는 23개의 염색체가 들어
있다. Bhp] ZX (haploid cell) = 게놈이 하나 들어 있는데, 이는 염색체가 한 세트 있다
는 뜻이다. 그러므로 인간의 반수 세포에는 염색체가 23개 있다. 이배체세포(0101010 cell)
에는 게놈이 2개 있으니, 염색체도 두 세트 있다. 양 세트에 있는 각 염색체는 하나 씩
BS 지울 수 있는데, 이 염색체 쌍을 동종쌍(6000108048 pair)°]e}31 한다. 동종의 쌍에
Al 각 GAAS SS (homolog) e}31 한다. 인간의 이배체세포에는 염색체가 3×23 =
46개 있다. 동종체은 부모에게서 각각 하나씩 물려받는다.

체세포(802ㅁ811ㅇ cell) = 생물체의 몸에 있는 세포 중 하나이다. 반수 YHA (haploid
organism) 반수 체세포로 구성된 생물체이다. 이배체 생물체(0101010 organism)= 이배
Al 체세포로 구성된 생물체이다. 인간은 이배체 생물체이다.

생식체(680666)는 성숙한 성 생식 세포로서 다른 생식체와 결합하여 접합체(67806)가
되는데, 이 접합체는 결국 새로운 생물체로 자라난다. 생식체는 항상 반수체이다. 수컷이
만드는 생식체는 정자(60600)이고, 암컷물 만드는 생식체는 난자(689)이다. 생식세포
(germ 00)는 생식체가 되기 전 세포이며, 이배체이다.

성숙한 이배체 생물체는 생식체를 생산하고, 두 이성 생식체는 결합하여 접합체를 형
gory, 그 접합체는 새로운 성숙한 생물체로 자란다. 이 과정을 HBA (sexual re-
production) °]2} 한다. 단세포 반수체 생물체는 이분열01087 1188102)이라는 과정을 통
하여 무성 생식하며, 하나의 생물체가 두개의 새로운 생물체로 분리된다. 따라서 새로운
생물체는 각각 모생물체와 유전자가 정확히 일치한다. 융합(8481020)이라는 APS 통하
여 성적으로 재생성되는 단세포 반수생물체도 있다. 두 개의 성숙한 세포가 결합하여
일시적 이배체 감수분열 모세포((ㅠ8ㅁ81606 diploid meiocyte)S 형성한다. 그 감수 분열
모세포는 각 부모로 부터 하나씩 받은 동족염색체 한쌍으로 구성된다. 한 아이는 각 부모
로 부터 동족체를 받으므로, 아이들은 부모의 유전자 사본은 아니다. 예를 들어, 게놈의
크기가 3이면, 한 아이가 가질 수 있는 염색체 BEES 2° = 8개가 있다.

염색체는 디옥시리보핵산(000×ㅋ571000ㅁㅁ01616 acid, DNA) 복합물로 구성된다. DNA
뉴클레오타이드(ㅁ0401600408)라 하는 4개의 기본 분자로 구성되어있다. 각 뉴클레오타이
드는 GEA (deoxyribose), 21449 (phosphate) 군, 퓨린 또는 피리미던 염기를 함유 한다.
퓨린(6007106)인 ofa} (A) 및 구아닌(@)은 구조가 유사하며, 피리미딘(61040106)인 시
BAO) 및 FIDE 구조적으로 비슷하다. DNAE 두 개의 대응가닥으로 구성된 Ade
자이며, 각 가닥은 일련의 뉴클레오타이드로 구성된다. 그 가닥들은 뉴클레오타이드 쌍
사이에 있는 수소 결합으로 이어진다. 아데닌(4)은 항상 티민(』)과 WS 이루고, 구아닌
G2 항상 시토신(0)과 BS 이룬다. 이러한 각 쌍을 표준염기쌍(68ㅁ001081 base pair,
bp)°]@} 하며, A, G, C 및 를 염기(6880@)라고 한다.



===== PAGE 430 =====
© 예제 101

4—>
a
600

-
|
A

그림 10.1 DNAS) 일부분

== A)
0 — 4)

그림 10,12 DNAS] 한 단면을 묘사해놓은 것이다. 생물학 공부를 했으면 BA 있겠지
만 DNAS 가닥들이 오른쪽으로 서로 꼬인 이중 나선 구조로 되어 있다. 하지만, 계산할
데이터로 쓰려면 각각을 그림 10.1과 같이 문자열로 취급하면 충분하다.

유전자(6606)는 염색체의 한 부분으로, 종종 수천 개의 염기쌍으로 이루어지며, 크기
도 매우 다양하다. 유전자는 생물체의 구조와 생성과정에 핵심 역할을 한다. 유전자형
(genotype) 생물체의 유전적 구성을 뜻하고, 한 생물체의 표현형(00600[526)은 유전자
형과 환경과의 상호 작용으로 생긴 BSS 뜻한다.

대립유전자(31618)는 여러 가지 BES] 유전자 중 하나이며, 대개 돌연변이를 통하여
생긴다. 대립유전자는 유전 변이를 담당한다.

염색체 15번에 있는 bey2 유전자는 인간의 te AAS 담당한다. 8008라고 하는 파란 눈 대립유전
자가 있고, 880\씨이라고 갈색 te 대립유전자가 있다. 유전자라면 뭐든지 그렇듯이, 각각 부모로
부터 대립유전자를 하나씩 받는다. BLUE 대립유전자는 열성(860688176)이다. BLUE 대립유전자
와 BROWN 대립유전자를 하나씩 받으면 갈색 눈동자를 갖는다. 파란색 ES 가지려면 양쪽에서
모두 BLUE 대립유전자를 받는 경우뿐이다. 갈색 대립유전자를 우성(000108204이라고 한다.

인간 생식자의 염색체는 23개 이고 각 염색체는 부모 중 한 쪽 게놈에서 물려받을 수
있기 때문에, 부모가 후손에게 전달할 수 있는 유전자는 2” = 8,388,608 가지의 다른 A
합이 있다. 실제로는 이보다 훨씬 더 많다. 감수분열02610818)(생식자를 만드는 세포 분
열) 중, 4 염색체는 스스로를 복제하고 동족체와 정렬한다. 이렇게 복제한 염색체를 염
ANA] (chromatid) 라고 한다. 종종 서로 마주치는 동종 염색분체 사이에 유전 물질 교환
이 이루어진다. 이 교환을 교차(@ㅠ088148-070)라고 하며, 교차하는 과정은 그림 10,2와
같다.

세포분열 중, DNA 복제에서 오류가 발생하는 경우가 있다. 이러한 오류를 돌연
(mutation) 2}31 한다. 돌연변이는 체세포 또는 배아세포 어디에서든 일어날 수 있다.
화에서 변종이 발생하는 원천은 모두 생식 세포의 돌연변이이라고 믿어지고 있다. 반
체세포의 돌연변이는 (암을 유발하는 것과 같이) 생물체 자체에 영향을 미칠 수 있지
그 자손에 영향을 미치지는 않는다.

뉴클레오타이드 하나가 다른 뉴클레오타이드으로 단순히 교체되면 치환 돌연변이
(substitution mutation) @}31 한다. 다른 DNA] 한 부분이 염색체에 추가되면 삽입 돌연
변이(14860010ㅁ mutation)=}31 하고, 다른 DNAS] 한 부분이 염색체에서 제거되면 결실

번ㅇ

~

도
=
(0)

무 쁘 건


===== PAGE 431 =====
420

chapter 10 유전 알고리즘과 유전 프로그래밍

!
oz
ni

a
it
-
—

재조합염색분체

|                                      | 재조헌쩌오염색분체

그림 10.2 교차 과정

$24 °|(deletion 104[81102)라고 한다.

AlSHevolution)= 개체군의 유전자 구성이 변화하는 과정이다. 유전자 구성의 변화는
돌연변이가 원인으로 보고 있다. 앞서 언급했듯이, 자연 선택(ㅁ864ㅠ81 86160407)이란 포
식자 또는 기후 변화, 식량 경쟁과 같이 환경적 압박에 적응할 수 있도록 해주는 SYS
가진 생물체가 다른 생물체들에 비해 더 많이 생존하고 더 많은 AES 남기면서, 유리한
변이를 미래의 후손들에게 더 많이 남기게 되는 과정이다. 그래서 자연 선택은 개인에게
이러한 유리한 특성을 부여하는 대립유전자들의 증가를 야기한다. 확률적으로만 일어난
대립유전자의 빈도 변화 과정을 유전자 부동(660640 drift)o]e} 한다. 자연선택과 유전
자 부동에서 어떤 것이 진화과정에 더 많은 영향을 미치는지 관해, 생물학계에는 의견
차이가 있다 (Li, 1997).

10.2 유전 알고리즘

먼저 기초적인 유전적 알고리즘을 공부하고, 이어서 응용사례를 둘 살펴보자.

10.2.1 알고리즘

유전 알고리즘은 반수생물체의 융합을 모델로 사용한다. 유전 알고리즘에서는 모집단에
서 반수생물체 중의 하나의 개체0ㅁ011048])를 문제에 대한 해답 후보로 본다. 각 개체는
염색체를 한 개씩 지니고 있다. 실제 생물체 이름인 A, G, C, 문자로 염색체 개체를
표현한다. 각 세대마다 적합한 일정 수의 개체가 번식이 허락된다. 알고리즘이 내주는



===== PAGE 432 =====
0 00600000
10.2 유전 알고리즘 421

해답의 우량할수록 더 적합하다. 두 적합한 개체의 염색체는 각각 나란히 줄을 서고 유전
물질(문제 해답의 부분문자열)을 교환한다. 경우에 따라 돌연변이028400)가 발생할
수 있다. 돌연변이는 다음 세대로 이어진다. 이 과정은 주어진 종료조건을 만족할 때까
지 반복된다. 이와 같은 일반적인 유전 알고리즘을 의사코드로 표현하면 다음과 같다.

void generate_populations()

{

0 = (0%

모집단 Py 초기화;

repeat
모집단 P, 소속의 2} 개체의 적합도 평가;
적합도 기준으로 생식할 개체 선택;
선택한 개체를 대상으로 교차와 돌연변이 실행;
1299

until 종료조건 만족

적합도를 기반으로 개체를 선택할 때, 반드시 가장 적합한 개체를 선택하지 않아도 된
다. 오히려 해답 탐색공간에서 후보영역을 고를 때 다양한 방법을 시도해 볼 수 있다.
이미 좋아 보이는 영역에 집중하여 취득한 정보를 활용하는 방법을 개발(66010804027)이
라고 하고, 좋아 보이는 것과는 무관하게 새로운 영역을 개척해보는 YS 탐험
(exploration) °]2@}31 한다. 개체를 선택하는 경우, 확률 eS 개체를 탐험으로 무작위 선
택하고, 확률 1-<로 적합한 개체를 WE 선택할 수 있다.

10.2.2 사례
다음 함수의 값이 최대가 되는 2의 값을 구해보자.

f(e)= sin 2] 구간 : OSa <255

여기서 2는 정수로 제한한다. 사인 함수는 0/24] 최대값이 1 이니, 당연히 = 128
때 함수 값이 최대가 된다. 따라서 이 문제를 푸는 알고리즘을 고민해보는 건 실용적으로
는 별 의미가 없다. 하지만 이러한 방식의 알고리즘의 다양한 Suis 쉽게 설명하려면
최대한 간단한 예제를 사용하는 게 좋으니, 이 BAS 푸는 알고리즘을 개발하는 절차를
따라가 보도록 하자.

1 문제의 PS 표현하는 알파벳을 고른다. 해답의 PME 단순히 0에서 255까지의
정수이므로, 8비트를 사용하여 각 해답 후보를 나타낼 수 있다. 예를 들면, 정수
189는 다음과 같이 표현한다.

1005 1891 Ou,



===== PAGE 433 =====
422     chapter 10 유전 알고리즘과 유

rt
i
뿌

브

2, 모집단을 구성하는 개체가 얼마나 되는지 정한다. 일반적으로 보면 개체가 수천

개까지 있을 수 있지만, 이 사례에서는 개체가 8개 이다.

3, 모집단을 어떻게 초기화할지 정한다. 무작위로 하는 경우가 많은데, 이 사례에서

는 0과 255 사이의 정수 중에서 8개의 숫자를 무작위로 생성한다. 표 10.1은 무작
위로 생성한 ARIS 보여주고 있다.

4. 적합도를 어떻게 평가할지 결정한다. 목표가 f(x) = 81ㅁ(×7/356) 값을 최대화

하는 ABS, Malo] 적합노는 던순히 이 Bre] sto] 된다.

5. 번식을 위해 선택할 개체를 결정한다. 탐험과 WAS 결합한 방법을 시도해보자.

각 적합도를 적합도 전체 합인 5.088으로 나누어 정규화한다. 정규 적합도는 모두
더하면 1이다. 이렇게 정규 적합도는 누적 정규적합도를 구하는데 사용되는데, 이
누적 정규적합도를 기준으로 WS 무작위로 선택한다. 표 10.1을 보면 <의 값
에 따라 f(x), 정규 f(x), 누적한 정규 L(x) WS 어떻게 구하는지 볼 수 있다.
예를 들어, 둘째 개체는 정규 적합도가 0.098이며, 그 개체는 너비가 0.093인 간
격인 (0,144, 0.286|에 할당된다. 그런 다음 간격 (0,1에서 무작위수를 생성한다.
그 수는 정확히 한 개체를 선택하게 된다. 이 과정을 8번 반복하여 8개의 개체를
택한다. 번식을 하기 위해 선택한 개체들이 표 10.8와 같다고 가정하자. 개인은
러 번 중복하여 나타날 수 있으며, 나타나는 빈도는 적합도에 따라 결정된다.
자와 돌연변이를 수행하는 방법을 결정한다. 첫째, 개체를 무작위로 짝을 지어
주 4쌍을 만든다. 쌍별로 개체에서 두 점을 무작위로 선택한다. 교차점에서 유전
질을 교환한다. 이 과정을 거친 결과는 표 10,33} 같다. 둘째 점이 개체의 첫째
점 앞에 나타나면 교차가 휘감기며 일어난다. 표 10.8에서 세 번째 개체 쌍이 교차
가 휘감기며 일어난 경우이다. 표 10.1과 표 10.3의 값을 토대로 보면, 평균 적합
도가 교차 전엔 0.685이고 교차 이후엔 0.798이다. 더욱이 교차 후 두 개체의 적
합도는 0.99 이상이 되었다.

SS

오세

{

어

El 요

떠8 애

음은 돌연변이 수행 방법을 정한다. 각 개체의 비트별로, 비트를 뒤집을지(0에서 1 =

@ 표 10.1 초기 모집단의 초기 개체와 적합도
개체              a         f(z)       정규 f(x)         누적 정규 f(x)
LOLLI101     189      WES)       144            144
11011000      216      ATL       093             287
O10 001 1      99      937       (184             421
11101100     236      2438       048            469
10 10111     174      .845       .166            .685
00100011      74       .788       (155             790
00100011      35       416       082             872
O011010 1      58      650       128            1,000



===== PAGE 434 =====
@0000000
10.2 유전 알고리즘  423

는 1에서 0으로 변경) 여부를 무작위로 결정한다. 돌연변이 확률은 보통 0.01 에서 0.001
의대

7, 종료 시기를 결정한다. 최대치로 정한 만큼의 세대교체가 일어났거나, 정해놓은
시간이 흘렀거나, 가장 적합한 개체의 적합도가 일정 수준에 도달하면, 이 과정을
종료할 수 있다. 이 사례에서는 10,000 세대가 지났거나, 적합도가 0.999를 초과
하면 종료할 수 있다.

부한 알고리즘에서 2, 3, 5, 단계는 어떤 문제라도 동일하게 적용할 수 있다는 점에서
괄적으로 사용할 수 있는 단계라고 할 수 있겠다.

Hof

@ F 10.2 번식하기 위해 선택한 개체

개체
OA120;000 1
00110101
11011.0040
10101110
01001010
10101110
01100011
10111101

@ 표 10.3 WAS 통해 생긴 부모와 자식들

우미       자식     2   f(z)
pole Rae   011°J101] 211   119  994
001]|101|/0 1   001/000| 01   33   394
1411011/]27000   11]10101]|2000   168  .882
1/0101] 110  1/1011] 110  222  405
Fah orrtle   10/700101'10   138  1992
1011 0111|0    10111|0   110  .976
01 1 0 010 1 1|^   01100|101|"   101   .946
101111101   101111011   187  .749



===== PAGE 435 =====
424

나

chapter 10 유전 알고리즘과 유전 프로그래밍

10.2.3 외판원 문제

외판원 문제(178761108 Salesperson Problem, TSP) 잘 알려진 NP-hard 문제이다. 다
항식 시간 알고리즘을 개발 한 적이 아직 없는데다, 다항식 시간 알고리즘을 개발하기가
불가능하다고 증명하지도 못한 부류의 문제를 NP-hard 문제라고 한다.

영업 사원이 개 도시로의 출장을 계획하고 있다. 각 도시는 모두 도로로 연결되어 있
다. 영업 사원의 출장시간을 최소화하기 위하여, 영업 사원의 SAV} 있는 도시에서 출발
하여 각 도시를 한 WAT 방문하고 다시 회사로 돌아오는 최단 여행경로((042)를 찾고
싶다고 하자. 가장 짧은 여행경로를 결정하는 문제가 바로 71@『이다. 출발 도시는 최단
여행경로에 포함하지 않는다.

TSP 문제는 도시를 정점, 도로를 이음선, EHO] 길이를 이음선의 가중치로 나타내는
가중치포함 4b6F 12] (weighted directed graph) = 표현할 수 있다. 일반적으로 1862 문
제에서 다루는 그래프는 정점이 모두 서로 연결되어 있는 완전(60ㅁ21066) 그래프일 필요
는 없다. 더구나 이음선 vs > Sh yy > ":가 둘 다 그래프에 있는 경우, 각 가중치가
동일할 필요도 없다. TSPE 운송 일정 AHS 짜는 용도 외에도 회로 보드 배치문제 및
DNA A) 293} 같은 문제에도 널리 쓰이고 있다.

이제 SPH 푸는 유전자 알고리즘의 유형을 세 가지 공부하자.

순서 교차
순서 교차(20067 crossover)S 먼저 적용하는 유형이다. (10.2.2 절의 일반 알고리즘과 다
= 부분만 살펴본다.)

1 문제의 답을 표현하는 알파벳을 고른다. TSP 문제의 BS 표현하는 직관적인 방
He 그래프의 정점에 1에서 2까지의 WSS 붙이고 방문한 순서대로 정점의 번
SS 나열하는 것이다. 예를 들어, 정점이 9개 있으면 [2 1 3 9 5 4 8 7 06]은
1, Vi, 3, , 순으로 계속 방문하여 까지 방문한 다음 로 돌아온다는 것을
나타낸다. 여기서도 출발 정점은 정해져 있지 않다.

4. 적합도는 여행경로의 길이이며, 짧은 여행경로가 더 적합하다.

6. 교차 및 돌연변이를 수행하는 방법을 결정한다. 이전처럼, 개인들을 무작위로 짝
을 짓고, 쌍별로 개체에서 두 점을 무작위로 선택한다. 선택한 점 사이의 부분경
로를 픽(0109이라고 한다. 각 도시가 여행경로에 한 번만 포함되어야 타당한 of
행경로인데, 픽을 무조건 교환하게 되면 결과로 얻는 여행경로가 타당하다는 보
장을 할 수가 없다. 따라서 순서 교차 알고리즘은 픽한 부분경로는 그대로 물려받
고, Fo) 아닌 부분을 중복되는 값은 빼고 다른 부모의 | 값부터 시작하여 차례
로 채운다. 이렇게 선택한 값들을 템플릿66001066)이라고 하는데, 표 10.4에서
템플릿이 어떻게 만들어지고 자식의 나머지 경로로 채워지는지 확인할 수 있다.



===== PAGE 436 =====
> 알고리즘 10.|

@ 표 10.4 주문 교차의 예

Parents                             Other Parent Template       Children
p:213'/954|2876 | 6871 3 2700 p    @7667'\954| 2132
m:532|689| 714 |547213fromp    ©:547 |689| 213

자식 <은 부모 22의 픽 부분인 (9 5 41를 그대로 물려받는다. 부모 po] 대한 픽
부분은 [6 8 Jolt} 부모 /의 템플릿은 6에서 시작하여 정점 번호를 0 5 41에
있는 Use 빼고 순서대로 나열하여 ae, 이 ake 끝에 도달하면 다시 맨
으로 돌아가서 계속한다. 완성한 부모 의 템플릿은 6 8 7 1 3 9] 이다. 이
들은 자식 oo 남은 경로를 순서대로 채워 여행경로를 완성한다.

전 그래프가 아니면, 새로 복제한 자식이 실제 여행경로가 되는지 확인해야 한
. 만약 VIET 아니면 RAE 허용하지 말아야 한다

변이의 경우, 정점을 맞교환하면 같은 정점이 중복될 것이므로 맞교환으로
dole 완성할수 없다. 그러나 clade 내의 두 정점을 맞교흰하거나 정점
eS] cS 12 뒤집어서 돌연변이를 완성할 수 있다. 하지만 완전 그래프가
아니면, 돌연변이 결과가 실제 여행경로인지 확인이 필요하다.

cee ee ii 60

rc rh eh

tf

bt

|근

or

이웃간 교차

제를 푸는 Nearest Neighbor Algorithm(NNA)-2 탐욕 알고리즘이다. NNAE 임의
점으로 시작하여 여행이 완료 될 때까지 반복적으로 가장 가까이 있는 미방문 정점
여행경로에 추가한다. NNAL 그래프가 완전하다고 가정한다. aaa 완전하지 않
면 타당하지 않은 여행경로가 완성되는 Boe 있다. 알고리즘은 다음과 같다.

ec

=
P
Al

2 &
맨

1ㅇ tho

sxe)

판원 문제의 Nearest Neighbor Algorithm(NNA)

문제 : 가중치포함 비방향 그래프에서 최적 여행경로를 구하시오. 가중치는 음이 아닌 수
입력 : 가중치포함 비방향 그래프 G, 정점의 개수 2

출력 : G2] 여행경로 정점 리스트가 저장된 AS tour

void generate_tour (int 2, graph (7, orderedlist& tour)

{

tour = [더 여기서 는 GO 무작위로 선택한 정점;
repeat

tour] 마지막 정점에서 가장 가까운 여행경로에 아직 방문하지 정점 tourol] 추가;
until tour] 정점이 2개 모두 들어있음;

그림 10.8(8/에서 가중치가 있는 무방향 이음선은 동일한 가중치를 가진 양방향이음선
으로 보면 되고, 그럼 10.800)는 가장 짧은 여행경로를, 그림 10.3(0)는 에서 출발하여


===== PAGE 437 =====
426

@
chapter 10 유전 알고리즘과 유전 프로그래밍

(9 에서 출발하는 NNA             (0) v, 에서 출발하는 NNA

로를 보여준다. 이 후자의 여행경로가 최적이다.

다음으로 80781 연구진이 2010년에 개발한 Nearest Neighbor Crossover(NNX) 알고리
즘을 소개한다. 아래에 제시한 절차는 개발 연구원이 자신의 알고리즘을 평가하는데 사
용한 절차와 동일하다.

…

1. 문제의 답을 표현하는 알파벳을 고른다. 표현방식은 10.2.3 절의 도입부분의 순서
교차 알고리즘과 동일하다.

2, 모집단을 구성하는 개체가 얼마나 되는지 정한다. 모집단 크기는 50과 100으로
한다.

8. 두 가지 기술을 시도한다. 첫 기술은 모집단 전체를 초기에 무작위로 정한다. 둘
째 기술은 반만 모집단을 무작위로 초기에 정하고, 나머지 반은 104&와 탐욕 이음
선 알고리즘(뒤에 설명)을 활용하는 하이브리드 기술이다.

4. 적합도을 어떻게 평가할지 결정한다. 적합도 평가 방법은 순서 교차 알고리즘과
동일한다.

5. 번식을 위해 선택할 개체를 결정한다. 적합도 상위 50%는 번식을 허용한다. 각
개체를 4개씩 복제하여 놓고, 이 중에서 부모쌍을 무작위로 선택한다.

6, 교차 및 돌연변이를 수행하는 방법을 결정한다. 104&에서는 두 명의 부모가 하나



===== PAGE 438 =====
V6 에서 시작하여
결합그래프에 NNA 적용

자식

그림 10.4 결합 그래프를 만들고 정점 \6부터 시작하여 NNA 적용

5

의 자식만 생성하기 때문에 엄밀히 말해 교차라고 할 수 없지만, 그럼에도 불구하
고 그렇게 부르기로 한다. 부모들은 먼저 결합하여 두 부모와 이음선이 있는 그래
프인 결합 그래프를 만듭니다. 이 결합 그래프를 만드는 과정은 그림 10.4에 나와
{습니다. 그런 다음 NNA7} 이 결합 그래프에 적용된다. 이것도 그림 10.4에 나

있다. 이 그림에서 정점 ㅠ부터 시작하여 NNAS 적용하면 부모들보다 더 적합
한 AAS 얻는다. 그런데 만약 에서 시작한다면 그렇지 않다. 에서 시작하는
경우, ㅁ에서 막다른 골목에 직면하게 되고 여행경로를 얻지 못한다. 선택한 정점
으로 여행경로를 얻지 못하면, 다른 정점을 가지고 여행경로를 얻을 때까지 시도
해봐야 할 것이다: 모두 시도해 보고도 여행경로를 얻지 못한다면, 완전 그래프에


===== PAGE 439 =====
428

chapter 10 유

[것
mo
KI
fu
oly
보
30
rat
i
고
므

아이오 이 오오 여오지이
Y
C+) -@-@-0-O-)-)

그림 10.5 정점 1에서 vee 이어지는 부분경로를 뒤집는 돌연변이

서 다른 이음선을 여행경로에 포함시킬 수 있다.
각 부모를 4개씩 복제하여 사용하고, 각 부모가 자식을 하나씩 번식하므로, 자식
AAS 가면 번식 가능한 부모의 수는 두 배가 된다: 그러나 부모의 반만 그렇게
할 수 있으므로, 인구는 세대가 바뀌면서도 그대로 동일하게 유지된다.
돌연변이는 다음과 같이 수행한다. 정점을 2개 무작위로 선택하고, 그 정점을 연
결하는 하위 경로를 뒤집는다. 이 과정은 그림 10.5에서 설명하고 있는데, 여기서
선택된 정점은 vist ㅠ이다. 돌연변이는 Miz} M22] 두 가지가 있다. Mio 돌연
변이는 각 세대에서 최상의 개체에만 적용된다. MAAS 모든 자식에 적용된다.
하나의 변형으로서, NNXS] 확률론적 버전은 현재의 정점에 이어져 있는 이음선
중에서 확률적으로 선택할 것이다. 선택될 기회는 이음선의 길이에 반비례한다.
이렇게 함으로써 모집단 인구의 다양성을 증가시킬 수 있으며, 조사 공간을 확장
할 수 있다. 그러나 80781 연구진(2010)의 확률적 기법이 오히려 결정적 버전보다
현저히 성능이 좋지 SSS 알아내고 최종 검사 대상에서 이 방법은 제외하였다.
7. 종료시기를 결정한다. 평균 적합성이 두 세대에 거쳐서 연속적으로 같거나, 500
세대가 흐르면 종료한다.

NNAS} NNXE 최단 경로 문제를 푸는 Dijkstrad] 알고리즘과 매우 유사하며, 시간복
AEE 정점의 개수를 이라고 할 때 그 알고리즘과 동일하게 002”) 이다.

탐욕 이음선 교차

Greedy Edge Algorithm (GEA)2 먼저 이음선을 감소하지 않는 순서로 정렬한다. 그리
고 나서 첫 이음선부터 시작하여 탐욕적으로 이음선을 여행경로에 추가한다. 이 때 정점
은 이음선이 8개 이상 AAS 되지 않도록 하고 정점의 개수보다 작은 길이의 사이클이
생기지 않게 해야 한다. 084는 그래프가 완전하다고 가정한다. Bz] 않으면 여행경로
가 만들어지지 않을 수 있다. 알고리즘은 다음과 같다.



===== PAGE 440 =====
> 알고리즘 10.2    외판원 문제에 대한 Greedy Edge Algorithm (GEA)
제 : 가중치포함 무방향 그래프에서 최적의 여행경로을 구하시오. 가중치는 음이 아닌 수
: 가중치포함 무방향 그래프 @, 정점의 개수 2
: GQ] 여행경로 정점 리스트가 저장된 변수 tour

m+ ㅁ으 ro
J

ard

void generate_tour (int n, graph (7, setofedges& tour)

감소하지 않는 순서로 이음선을 정렬;
tour = 0; // 여행경로는 이음선의 집합으로 표현
repeat
 이음선을 하나 추가하더라도 연결된 정점에 이음선이 374 이상이 되지 않음
and 보다 작은 길이의 사이클이 생기지 않음
tour 이음선 추가;
until kaso] 이음선이 2개 있음

그림 10,64] 그림 10.8과 같은 예제를 가지고 GEAS 설명한다.
Greedy Edge Crossover(GEX) (9078! 연구진 2010) 알고리즘도 다음의 여섯째 단계만
다르고 NNXS} 동일하다.

6. 교차 및 돌연변이를 수행하는 YAS 결정한다. NNX 에서처럼 00에서도 먼저
부모들을 결합하여 결합그래프를 만든다. 그런 다음 GES 결합그래프의 이음선
에 적용한다. 이 과정으로 여행경로가 완성되지 않으면, 전체 그래프에 GEAS 적
용하여 남은 여행경로를 구한다. 그러나 이 과정은 탐험을 거의 하지 않아서, 가
중치가 높은 이음선이 그대로 남아있어 좋지 않은 해답으로 조속히 결론을 지어
버리게 될 가능성이 있다. SHS 증가시키려면, 새 여행경로의 전반부는 결합그
래프에서, 나머지 절반은 전체 그래프에서 가져오는 방법을 시도해볼 수 있다. 실
제로 실험해본 결과, 결합그래프에서 최대한 이음선을 많이 가져오는 방법에 비
해서 이 방법이 더 좋은 성능을 보였다. 다음에 살펴볼 평가에는 이 HAS 사용
한다.

NNAS} NNKE 최소비용 신장트리 문제를 푸는 크루스칼의 알고리즘과 매우 유사하
며, 그 알고리즘처럼 시간복잡도가 O(n? log 7) 및 A(mlog m) 이다. 여기서 n& 정점

의 수이고 m2 이음선의 수이다.


===== PAGE 441 =====
430

chapter 10 유전 알고리즘고

30
[것
고
0므

1. 이음선을 가중치 순으로 정렬       2 서로수 집합 생성

(0062.03) 1
(VV) 2
(624) 3

(02) 4

(003) 5

(V3,V4) 6
3, 이음선 (Vo, va) 선택           4, 이음선 (vy, va) 선택           5, 이음선 (Vp, vy) 선택
6. 이음선 <, Vo) 제거          7. 이음선 (/1, Vs) 선택

그림 10.6 Greedy Edge Algorithme 2 푸는 TSP 문제 사례

평가

유전자 알고리즘은 휴리스틱 알고리즘이므로 정확성을 엄밀하게 증명하는 진이 불가능
하다. 따라서 수많은 사례를 동원하여 결과를 검사해보고 평가해볼 수밖에 없다. 80781
연구진(2010)의 NNX2} GEXS 다음과 같은 방식으로 평가했다.

첫째, 788120에서 실제 도시 간의 거리를 나타내는 792 사례 10 개를 가져왔다. 도시
간에 거리는 양방향으로 동일하게 대칭이다. 이 중에서 가장 큰 사례는 도시의 개수 7
= 226 이었다. 돌연변이 없이도 해보고, 앞서 공부한 Mis} M2 ae 적용해보기도
했다. 첫 모집단은 THE 초기화하기도 하고, 최근접 이웃과 탐욕 이음선 알고리즘
에 기반한 하이브리드 기법(6) 으로 초기화하기도 했다. SAH] 유형과 초기화 유형의



===== PAGE 442 =====
@
10.2 유전 알고리즘          431

각 조합에 대해, 10개의 사례를 모두 각 알고리즘 별로 30번 실행하여 총 300 회 실행하
였다. 이 알고리즘은 ANSI CH 구현했으며 RedHat Linux 8.0을 실행하는 2568003 RAMS]
Pentium IV 1600MHz 컴퓨터로 실행되었다.

300회 실행하여 얻은 평균은 표 10.5에 알고리즘 별로 나열하였다. 표의 항목은 각각

ㄱㅋㄱ

oft
ro

SS

유형. '40 은 돌연변이를 사용하지 않음을 나타냄
는 하이브리드03) 초기화 방법 중 하나

* 편차 : 최적 솔루션과의 백분을 편차

* 세대수 : 수렴까지의 세대 수

* 시간 : 수렴까지의 걸린 시간 (단위: 초)

표 10.5를 보면, NNX2] 성능이 00×보다 훨씬 뛰어 났고, 돌연변이 중 M27} 가장 4
능이 좋았으며, 하이브리드로 초기화를 해도 무작위보다 그리 성능이 나아지지 않았음을
알 수 있다. GEXS| 사용률을 변화시키면서 NNXS 사용하면 성능이 향상 될 수 있는지
추가로 조사해 보았는데, 표 10.5에 그 결과를 보여주고 있다. 예를 들어, NNX7} 50%이
고 GEX7} 50%라는 말은 반은 NNXS 사용하여 모집단을 생            은 GEXS 사용하여
BAAS 생성했음을 의미한다. 돌연변이 M22] 경우, NNX 사용률이 높아질수록 406%만
사용한 경우에 비해서 약간의 개선이 관찰되었다.

두 알고리즘을 혼합하는 쓰는 경우 계산 시간이 늘어나는데, 성능은 그리 나아지지 않
았으니 굳이 GEXS 혼합하여 쓸 가치가 없다는 결론을 내릴 수 있다. 따라서 추가 실험
은 304※만 사용하여 수행하였다.

무작위로 모집단을 초기화하여 NNXY 적용하여 모집단의 크기를 100으로 증가시킨
평가 결과는 표 10.6에 나와 있다. 돌연변이 M22} 평균 편차는 0.85이고 평균 시간은
26.2이다. 표 10.5의 평가 결과와 비교해보자. 모집단의 크기 50에 동일한 ABS 사용하
면 평균 편차는 0.55이고 평균 시간은 5.50다. 정확도가 늘어난 반면 시간이 더 걸렸는
데, 투자한 시간만큼 정확도 향상이 가치가 있어야한다.

그리고 도시의 개수 318개에서 1748개 범위의 대규모 사례를 TSPLIBA 가져다 실험
을 시도해 보았다. 하이브리드 초기화가 별 효과가 없었으므로, 무작위로 초기화하여 모
집단 크기를 100으로 하여 NNXS 각각 10번씩 실행해보았다. 그 결과는 표 10.7에 나와
있다. 재미있게도 대규모 사례에서는 돌연변이 M22] 경우 소규모 사례와 비교했을 때
계산시간이 엄청나게 많이 소요되었다. 표 10.6을 다시 보면, 소규모 사례에서는 M27}
Mitt} 계산 시간도 더 많이 걸리지 않으면서 훨씬 성능이 좋았었다.

ox
웨
rl
ro
lo



===== PAGE 443 =====
@0000000
432     chapter 10 유전 알고리즘과 유전 프로그래밍

@ 표 10.5 모집단 크기가 50인 10개의 소규모 문제 사례별 30회 실행하여 얻은 평균

알고리즘 | 돌연변이 |모집단 초기화| . 편차          세대수          시간
No M          R           3,10         45,39         0,38

H            4,82          33,52          2,95

M1             R            1,67           40,21          0,62

H            1,57          36,09          3,55

M2             R            0,55          53,37          5,52

H            056          43.53           8.11

No M           R           12,54          17,35         48 23

H                            7,19                        16,37                      54,27
M1             R            4,36          60,44         208,70

one                                                             H                            3,67                       48, 44                     178,65
M2             R            3,30          26,30          82,79

H            3,01          25,83          90,58

No M           R            8,15          42,50         W325

H            5,53          38,47          75,67

50% NNX          M1              R             1,92           66,04          113,81
50 % GEX                         H             1,68           61,21          DOT
M2             R            1,76           19,25          26, 40

H                           1.61                       20,68                      34,19

No M           R            7,23          41,16          13,39

H            5,19          34,93          14,95

90% NNX          M1              R             1,84           50,60           19,14
10% GEX                          H             1,67           46,93           20,16
M2                           R                          0,51                       37,13                     19,26

H                           0,48                       37,24                      21,95

No M          R           6,69         41,23         6,74

H            5,06          33,04          8.93

95% NNX          M1              R             1006           52.62           10.08
5% GEX                         H            1,41          4433          11,30
M2                             R                            0,49                        37,15                       11,58

H                           0,44                        36,19                       14,88

@ 2106 모집단 37/7} 100이고 모집단을 무작위로 초기화하는 경우 10개의 소규모 문제
사례별 30회 실행하여 얻은 평균 Bu

알고리즘                        돌연변이                            편차                               시간
No M                 5.40                 18,4

NNX                         Mi                         1,44                        26,4
M2                         0,35                        26,2



===== PAGE 444 =====
@ 표 10.7 모집단 크기가 100이고 BF

사례별 10회 실행하여

10.3

집단을 무작위로 초기화하는

—
=
얻은 평균 결과

유전 프로그래밍

433

우 15개의 대규모 문제

알고리즘                  돌연변이                     편차                        시간

No M                 7.61                 25,3

NNX                         M1                         4,94                        65,0
M2                         4,70                       1063,0

@ F 10.8 NNX2} 다른 두 개의 휴리스틱 TSP 알고리즘의 10개의 문제 사례에 대한 성능

비교
문제                             NNX-MI1                       NNX-M2                    Meta—RaPS                      ESOM3
.             편차 | 시간' | 편차 | Ae | 편차 | 시간' | 편차 | 시간"
61101          0.98      Sel      0,82      14.3      NA       NA      3,43      NA
bier127         0,62      15.3      0,28      12,0      0,90       48       1,70      NA
pr136                    2,87           18,4           0,37           35,2           0,39             73              4-31             NA
kroa200         1,78      87,3      0,32      98.6      1,07      190      2,91      NA
pr226                   0,79           93.0           0,01           21,6           0,23            357             NA             NA
1in318                    1,87             8.0             2,01             105              NA              NA            2,89             NA
pr439                     3,44             10,              1,48             240            3,30           2265             NA              NA
peb442                  4.75           15,0           3,18            270             NA             NA            7,43            NA
pebl1173                  3,00           97.0            8.01            1230            NA              NA             9,87            200
vm1748                  7,05            203            7,09           4215            NA              NA             7.27            475
휴리스틱                                    는 문제 사례의 개수를 늘린다고 성능 향상을
os

두드러지게 알 수 있는 건 ‘etn 이미 알려진 휴리스틱 알고리즘과 어떻게 성능을 나타
나는지 상대적으로 비교해보아야 한다. 88781 연구진(2010)은 10를 10개의 벤치마크
TSPEA] 사례를 가지고 기존의 휴리스틱 TSP 알고리즘인 Meta-RaPS(DePuy 연구진
2005)와 ESOM(Leung 연구진 2004)과 비교했다. 그 결과는 표 10.8에서 보여준다.
04%-141(돌연변이 M1) 또는 4006-108(돌연변이 M2)7} 문제 사례에 관계없이 성능이 가
장 뛰어났다.

10.3 유전 프로그래밍

유전자 알고리즘에서 "염색체" 또는 "개체"가 문제의 해답 자체를 나타내는데 비해서, 유
전 프로그래밍(66ㅁ661ㅇ programming) A= 개체가 문제를 푸는 프로그램을 나타낸다.
개체의 적합도 함수는 프로그램이 문제를 얼마나 잘 푸는지를 나름의 방식을 동원하여
측정한다. 초기 모집단 프로그램을 모아서 시작해서, 교차를 통하여 더 적합한 프로그램
이 번식하고 자식 모집단에 돌연변이를 일으키는 과정을 종료 ZA] 만족할 때 까지 반


===== PAGE 445 =====
‥000000 0
434     chapter 10 유전 알고리즘과 유전 프로그래밍

복한다. 이 과정을 고수준 알고리즘으로 표
지만 복습하는 의미에서 다시 한 번 읽고 지나가자.

(에
에
re
so
로비
fl [0]
Ly
aus
ON
as
rfe
pa
OW
에
ne,
cs
eo)

void generate_populations()

{
c= 0;
모집단 Py 초기화:
repeat
모집단 P, 소속의 Z 개체의 적합도 평가;
적합도 기준으로 생식할 개체 선택;
선택한 개체를 대상으로 교차와 돌연변이 실행;
Var
until 종료조건 만족
}

유전 프로그램의 개체(프로그램)는 트리로 표현한다. 트리의 각 마디에는 터미널기호
(terminal symbol) 또는 @+=7]%(function symbol)7} 있다. 마디가 함수 기호인 경우, 마
디의 인수들은 그 자식들이다. 예를 들어, 다음과 같은 식(프로그램)이 있다고 가정 하자.

22

0202                                OD)

트리 구조로 표현하면 14 10,73} 같다.

10.3.1 사례
유전 프로그래밍은 점 x, 의 집합을 가지고 함수 y= /(저를 학습하는 것으로 간단히
설명할 수 있다. 예를 들어, 표 10.9와 같은 점의 집합이 있다고 하자.

이 ASS 다음 함수를 사용하여 생성하였다.

y=e72

그림 10.7 4] 10.19) 트리구조 표현



===== PAGE 446 =====
@00@00000 0
10.3 유전 프로그래밍 435

@ 표 10.9 점 ×와 >사이의 관계를 잘 나타내주는 함수를 이 10개의 점을 토대로 학습

6 00 -3 060 어 8 060 659 ㄴㅇ | 8
으
©
5

시킨다.

3. 함수 집합 FS 정한다. 함수 AWS +, -, ×와 / 기호로 설정한다. 원하는 경우
sin, 008 등과 같은 다른 함수도 포함시킬 FUSS 알아두자.

8. 모집단의 개체수를 정한다. 여기서 모집단의 크기는 600으로 한다.

4. 모집단을 초기화하는 방법을 정한다. 초기 개체는 나무키우기(@00\108 the tree)
라고 하는 절차로 만든다. 먼저 7 U 집합에서 기호를 무작위로 생성한다. 터미
널기호이면 바로 멈추고 그 기호만으로 구성한 (단일 마디) 트리를 생성한다. 함수
기호이면 그 기호의 자식들을 무작위로 생성한다. 트리를 타고 내려가며 기호를
무작위로 AS 생성하다 터미널 기호를 만나면 멈춘다. 예를 들어, 그림 10.7의 =
Fe 다음과 같이 기호를 무작위로 생성하여 만든다. 먼저 기호 /를 생성하고 그

자식인 + 와 - 를 이어서 생성한다. + 의 자식으로 x9} 2S 생성하는데, 이 자식들
은 모두 터미널이므로 더 이상 생성을 지속하지 않고 멈춘다. -의 자식으로 59}
×를 생성한다. 5에서는 생성을 멈추고, xe 자식 3과 ×를 마지막으로 생성한다.

5. 적합도 함수를 정한다. 적합도 함수는 제곱오차함수를 사용한다. 즉, 적합도 함수
Ax) 표 10.9의 각 점 (x, 에 대해서 다음과 같이 세울 수 있다.

10

고

(Ff (z,)— y;)”

오차가 작을수록 더 적합한 함수가 된다.
6 번식할 개체를 선택하는 방법을 정한다. 4-개체 토너먼트 선발 프로세스를 사용한
다. 토너먼트 선발 프로세스는 모집단에서 무작위로 개체 //개를 선택한다. 개체


===== PAGE 447 =====
@0@00000 0
436     chapter 10 유전 알고리즘과 유전 프로그래밍

Y
0        시

번
=]

그림 10.8 하위 트리를 교환하여 교차하

rr

방

개가 참가하는 토너먼트에서 가장 적합한 7/2가 승자가 되고, 가장 부적합한
7/3가 패자가 된다. 7/2개의 승자들은 7/2개 자식의 번식이 허용되고, 다음 세
대에서 이 자식들이 7/2개 패자들을 대체한다. 이 경우엔 n=4 이므로, 9개의
승자가 3개의 자식을 번식하여 2개의 패자를 대체한다.

7, 교차 및 돌연변이 수행 방법을 정한다. 두 개체의 교차는 무작위로 선택한 하위
트리를 교환하여 수행한다. 이 교차 YAS 그림 10.8의 사례를 보면 이해할 수
있다. 돌연변이는 마디를 무작위로 선택하고 그 마디의 하위 트리를 새로 키운
하위 트리로 대체하여 수행한다. 돌연변이는 후손의 5%에게 무작위로 수행한다.

8. 종료 AAS 정한다. 가장 적합한 개체의 제곱 오차가 0이거나, 100세대를 번식했

으면 WAS 종료한다.

Banzhaf 연구진(1998)은 표 10.9에 제시된 데이터에 이 기술을 적용하는 실험을 하였
따. 다음은 첫 4 세대에서 가장 적합한 개체가 어떻게 나타나는지 보여준다.
가장 적합한 개체는 8세대만에 매우 큰 트리로 확장되지만, 4세대에 가서 정확한 해답

(데이터를 생성하는 함수)으로 다시 축소된다.



===== PAGE 448 =====
세대                가장 적합한 개체
!                             [1
~                     0 22
x
9(a +1)
그                               +2
gain ee    본
4                  Em
2

10.3.2 인공 개미

음식 흔적을 쫓아다니는 로봇 개미를 개발하는 BAS 공부해보자. 그림 10,9% 산타페
트레일(68066 Fe trail) 개미의 흔적을 나타낸 그림이다. 각 검정 정사각형은 음식 알갱이
하나를 나타낸다. 그림을 보면 총 89 개의 그러한 정사각형이 있다.

개미의 목표는 “시작” 화살표가 가리키는 사각형에서 출발하여, 89712] 검은색 사각형
을 모두 방문하고 (즉, 먹이를 모두 먹어 치우고) ‘go's 표시된 사각형에 도착하는 것이
다. 트레일을 따라가 보면 중간에 틈이 많이 WSS 주목하자. 이러한 유형의 문제를 계
획문제(0180ㅁ0108 ㅁ『001600)이라고 한다.

개미에는 다음과 같은 센서가 있다.

food_ ahead - 먹이를 만나면 706값을 갖고, 그렇지 않으면 False 값을 갖음

AIS            Co

[ahaa
TTT y

|혀 xe] maf] |키기티에 8



===== PAGE 449 =====
438

chapter 10

H
브

@
유점 윌고리즘과 Se 프로크래

0

개미가 정해진 시간 단위마다 취할 수 있는 액션은 다음 세 가지가 있다.

* right: 움직이지 않고 90도 우회전한다.

@ left: 움직이지 않고 90도 좌회전한다.

@ move: 정방향으로 한칸 직진하고, 먹이가 있으면 그 먹이를 먹는다. 따라서 그 먹이는
트레일에서 없어진다.

30
ca

Koza(1992)= 이 HAS 푸는 다음과 같은 유전 프로그래밍 알고리즘을 개발했다.

1 터미널 집활 TS Bett. 터미널 VMehe 개미가 취할 수 있는 액션이 들어 있
다 ,
T = {right, left, move}.

2, 함수 집합 『를 정한다. 함수 집합은 다음과 같다
(a) if food_ahead(instruction1, instruction2);
(b) do2(instruction1, instruction2);
(c) d0B(instruction1, instruction2, instruction3);
첫째 함수는 “86000 ahead7} 2°) instructionlS 실행하고, 그렇지 않으면 in-
struction2= 실행한다. 둘째 함수는 무조건 77279777707702721과 777977770/70772를 실행
한다. 셋째 함수는 EA instruction, instruction2, instruction32 실행한다.
예를 들어, 다음은 개미를 우회전하고 앞으로 움직이게 하는 함수 호출이다.
do2(right,mo -
3, BAS] 크키를 Be, .몬집단의 크키는 800으로 Br},
4. 모집단을 초기화하는 방식을 정한다. 나무키우기 방식으로 초기화한다. (10.8.1절
참조)
5, 적합도 함수를 정한다. 정한 단위 시간마다 (2794, left, move) 중 액션 하나를
취하고, 개체는 각 400 단위시간까지 쓸 수 있도록 한다. 개체는 좌상단에서 동쪽
방향으로 출발한다. 배정 시간 내에 먹은 먹이 일갱이의 WES AMES 정한다
그러면 최대 적합도는 89가 된다.
6, 번식할 개체를 선택하는 방법을 정한다.
7, 교차 및 돋연변이 수행 ae   한다. 두 개체의 교차는 무작위로 선택한 하위
트리를 교환하여 수행한다. 이 교차 방식은 그림 10.8의 사례를 보면 이해할 수
있다. 돌연변이는 마디를 sacle 선택하고 그 마디의 하위 트리를 새로 키운 하
트리로 대체하여 수행한다. 돌연변이는 후손의 5%에게 무작위로 수행한다.
8, 종료 조건을 정한다. 적합도가 89인 MAS 찾았거나 반복의 회수가 미리 정해놓
최대치에 도달하면 종료한다.

|

de

flo o



===== PAGE 450 =====
@0ㅋ00000 0
10.8 유전 프로크래밍    439

[1000 '
ahead

그림 10.10 ACH 2201.4 적합도가 890! 개체

모집단의 각 개체(프로그램)는 400번(단위시간) 반복 수행한 다음, 개체별로 적합도를
평가한다. Koza(1992)9] 실험 결과에 의하면 9째 세대에서 적합도 89인 개체를 얻었다.
그 개체가 그림 10.10에 나와 있다. 세대 0 개체의 평균 적합도는 3.5이었고, 세대 0 개체
중에서 가장 적합도가 높은 개체는 적합도가 38였다.

10.3.3 금융거래 응용

주식 및 기타 금융 시장 투자자들이 직면하는 중요한 의사 결정 포인트는 특정일에 매수,
매도, 보유 여부이다. 이러한 ABS 내리는 자동화 시스템을 개발하려는 시도가 활발하
게 있었다. Farnsworth 연구진(2004)은 유전자 프로그래밍을 활용하여 이러한 시스템을
개발했다. 특정일의 시장 지표 데이터를 기반으로 투자결정을 내리는 시스템이다. 이 시
스템을 공부해보자.

금융거래 시스템 개발
시스템 개발에 적용한 8단계를 먼저 차례로 살펴보자.

1. 터미널 집합 TS 정한다. 터미널 기호는 시장 지표이다. 다양한 시장 지표를 가지
고 테스트해본 다음, 어떤 지표를 최종 시스템에 포함할지 결정하였다. 최종 결정


===== PAGE 451 =====
@0000000
440     chapter 10 유전 알고리즘과 유전 프로그래밍

경제의   주요 ALA = el 500대 선도 기업을 대상으로 만
정일의 S&P 500 지수는 다음 식으로 계산한다

5&72500,.,. -,5&72500. 44

5&2500,

S& P 500 ,, 는 해당 일의 S& 500지수이고, &ㅁ500,,,는 지난 200일
동안의 Bat 지수이며, S& 500, 는 지난 200일 동안의 표준 편차이다.
이 지수값을 여기에서는 단순히 SP500°8 표기하기로 한다.

b) 어떤 증권 k-day Exponential Moving Average(EMA)© 지난 kk 91
그 증권의 가중치 평균이다. 증권 x2] Moving Average Convergence
/Divergence(MACD)2 다음 식으로 계산한다.

MACD(zx) = 12-dayEMA (x) — 26-dayEMA (x)

비벼 탄력 지표로 간주한다. 값이 양수이면 상승 탄력이 증가하고 있다
고 보고, 음수이면 하락 탄력이 증가하고 있다고 본다.
이 시스템에서 사용하는 둘째 지표는 MACD (S& ^ 500)이며, 간단히 MACD
로 표기하기로 한다.
(0 지표 444(2279는 S& P5002] MACD 2] 9-일 EMA 이다.
(0) Diff= 상승하거나 하락하는 증권의 수의 차이라고 하자. McClennan
Oscillator (MCCL)= 다음 식으로 계산한다

MCCL = 19-dayEMA (Dif f )— 39-dayEMA (Dif 7)

MCCL > 1002 때 시장을 초과 매입으로 보고, MCCL < 100 일 때 초과매
출로 본다.
이 지표는 단순히 MCCLO# 표기하기로 한다.
(6) 522 500700, MACDlag, MACD9lag, MCCLlag= 전날 지표 값을 의미한다.
(8) 터미널 기호로 실수의 구간 [- 1, 1]이 있다. 지표 값은 모두 구간 [- 1,12

정규화 한다.

2, 함수 집합 #를 정한다. 함수 기호에는 +, -, x 연산자와 다음 제어 구조를 포함한

다.

(a) if x >0 then y else z, 이 구조는 기호 가 자식 x, y, ZS 가지고 있는 트리
이다.

00 if x >w then y else z, 이 tA 7|& IFGTY} 자식 x, w, y, cS 가지고
있는 트리이다.

8. 모집단의 개체수를 정한다. 개체수를 다양하게 시도해보았는데, 500개 미만의 개



===== PAGE 452 =====
@0000000
10.3 유선 프로그래밍   441

체수는 실용적이지 않았고, 2,500개 BEL] 개체수가 결과가 좋았다.

4. 개체를 초기화하는 방법을 정한다. 초기 개체는 10.8.1 절에서 설명한대로 트리키
우기로 만든다. 허용되는 최대 레벨(트리의 가지 깊이)은 4 이었고, 허용되는 최
대 노드 수는 24개 이었다. 이 제한은 후세대 모집단에도 적용되었다. 이렇게 제
한하는 SAS 트리가 학습 데이터에 매우 근접하게 일치하지만 보지 못한 데이
터로 인한 예측 값을 제한할 때 발생하는 WHE Als SH overfitting)S 방지하기위
원 것의다.

5. 적합도 함수를 정한다. ABE 1983년 4월 4일부터 2004년 6월 18일까지 S&P
종가를 모아서 사용했다. 사용한 트리는 첫 4750일들의 데이터를 우선 분석한다.
Bes 첫날 91로 시작한다. 특정일에 트리가 0보다 큰 값을 반환하면 구매 신호
를 생성하고, 그렇지 않으면 매도 신호를 생성한다. 가지고 있는 ES 모두 매입
또는 매도가 있을 때 언제나 투자 또는 철회 중 하나를 선택한다. 투자 또는 철회
를 부분적으로 나누어 할 수 없다. 트리가 전날 시장에 들어가 있고 구매 신호를
생성했는데 아무런 조치도 취하지 않을 수 있다. 유사하게, 트리가 전날 시장에
들어가 있지 않고 매도 신호 생성했는데 아무런 조치를 취하지 않을 수 있다.
4750 일의 거래가 완료되면, 최종 값이 이익을 나타내도록 초기 투자한 1달러는
공제한다. 추가 과도적합화를 막기 위해 총 거래 수에 비례하여 적합도 페널티를
부과한다.

6. 번석할 개체를 선택하는 WHS 정한다. 모집단을 적합도 순으로 정렬한다. 하위
25 %는 없애고 더 적합한 개체로 대체한다.

7, 교차 및 돌연변이를 수행 방법을 정한다. 두 개체의 교차는 무작위로 선택한 하위
트리를 교환하여 수행한다. 마디 돌연변이(0006 mutation)= 무작위로 소수의 마
디를 선택하고 그 마디의 값을 동일한 인수를 사용하는 마디로 무작위 변경하여
수행된다. 함수 마디 돌연변이는 연산자를 바꾸고, 터미널 마디 돌연변이는 표시
기 또는 상수 값을 변경한다. 트리 SAH|(tree mutation)=E 무작위로 하위 트리
를 선택하고, 이를 새로운 무작위 하위 트리로 교체하여 수행한다.
모집단의 상위 10%는 변경되지 않은 상태로 남는다. 상위 10 %에 있는 개체들과
의 교차하기 위하여 무작위로 50 %를 선택한다. 20 %는 노드 돌연변이를 하기 위
해 선택하고, 10%는 트리 돌연변이를 하기 위해 선택하고, 10%는 없애고 무작위
로 교체한다.

8. 종료 조건을 정한다. 최대 세대 수는 300-500 범위로 정한다.

평가

1983년 4월 4일부터 2004년 6월 18일까지 S&P 종가 데이터를 가지고, 첫 4750일 동안
AVES 결정하면서 ALAS 학습하도록 하였다. 나머지 500일은 이 데이터를 기반으


===== PAGE 453 =====
‥00@00000 0
442     chapter 10 유전 알고리즘과 유전 프로그래밍

그림 10.11 특정 실행에서 가장 적합한 트리로 살아남고 평가 결과가 좋은 트리

로 적합도을 계산하여 시스템을 평가하는데 사용하였다. 그림 10.119] Bele 보여주는
시스템은 평가한 적합도 Zo] 0,397 이다. 투자의 매입보유(607-600-1010) 전략은 증
권을 구입하여 그냥 보유하는 전략을 말한다. 알려진 바로, 매입 보유 전략의 적합도는
0.1098로 낮다.

@ 104 논의 사항 및 추가 공부 자료

진화 계산의 주가 영역으로 전화 프로그래밍과 전화 전략이 었다. 진화 프로그래밍
(Evolutionary programming)-2 특정 문제에 대한 해답으로 진화하기 위해 후보 해답 집
단을 이용한다는 점에서 유전 알고리즘과 유사하다. 진화 프로그래밍의 다른 AS 주위
환경과 상호작용하는 관찰가능 시스템의 행동 BAS 개발하는 데 SAS the 것이
다. Fogel(1994)-2 이러한 방식으로 진화 프로그래밍을 제시한다. 진화 전략(07014110ㅁ
strategies) 종(63000169)으로 문제 해답을 모델링한다. 86016060678(1994)는 진화 전략
분야는 진화의 진화에 기반한다고 한다. 진화 계산의 네 영역을 모두 Bestop
Kennedy and Eberhart (2001) 책을 읽어 보기 바란다.

e ae

10.14
1. 이배생물체의 유성생식, 반수생물체의 이분열, 반수생물체의 융합의 2 4S 설명하시오.
2. 이배생물체 게놈 중 하나에 염색체가 10개 있다고 가정한다.

(8) 체세포 하나에 염색체가 몇 개 있는가?

00) 생식세포 하나에 염색체가 몇 개 있는가?



===== PAGE 454 =====
3. 성인 반수생물체 둘이 용합으로 번식한다고 가정한다.
(a) AALS 몇 마리 생산하는가?
0) 자식의 유전자는 모두 동일한가?

4. 인간의 te 색깔은 bey2 유전자에 의해 결정된다. 갈색 눈의 대립 유전자가 우성유전자이다.
음 각각의 부모 대립 유전자 조합에 대해 개인의 눈 색깔을 결정하시오.
아버지       어머니
BLUE               BLUE
BLUE              BROWN
BROWN              BLUE
BROWN             BROWN
10.28

5. 8개 개체 적합도가 각각 61, .23, 85, 11, .27, .36, .55, .44 라고 하자. H 1012 보고
정규적합도와 누적 정규적합도를 계산하시오.

6. 표10.3에 설명하는 대로 기본 교차를 수행하고, 부모는 각각 0110 1110과 11010 101이
며, 교차의 시작점과 끝점을 각각 gah ?이라고 하자. 태어나는 두 자식은?

7. 10.2.절에서 공부한 /(7) =810(47/256)을 최대화하는 12] 값을 찾는 유전 알고리즘을
구현하시오.

8. 이음선에서 양방향 가중치는 같다고 하고, 그림 10.12의 797 사례를 보고 최단 여행거리를
구하시오.

9. 우리가 순서 교차를 수행한다고 하고, 부모가 각각 3 5 2 1 4 68 7 와 5 3 3 6 9 1 8 7
4이고, 선택 시작점과 SAO] 각각 4와 ?이라고 하자. 태어나는 두 자식은?

10. 24 10,122] TSP 사례에서, 각 정점부터 시작하여 Nearest 16190 알고리즘을 적용해보
자. 그 중 하나는 최단 여행경로인가?

11. 그림 10.13의 두 여행경로의 결합그래프를 만들고, Nearest Neighbor Algorithms 정점 vs
에서 시작하는 결과 그래프에 적용해보시오.

그림 10.12 TSP 사례


===== PAGE 455 =====
@00@00000 0
444    chapter 10 유

ra
no
티
ps
OW
ic)
30
[것
i
대
0므

8
그림 10.13 두 여행경로

12. Greedy Edge Algorithm 그림 10.12의 TSP 사례에 적용해보자. 최단 여행경로를 구할 수
있나?

10.3절

13. 그럼 10.8의 두 트리에서, 왼쪽 트리에서 “4"로 시작하는 하위 트리를 오른쪽 트리에서 "+"로
시작하는 하위 트리로 바꾸면 생기는 트리를 그리시오.

14. 그림 10.10의 개체(프로그램)에서, 첫 10 단위시간 단계 동안 산타페트레일을 따라가면 이
프로그램이 쟁성하는 움직임을 기술하시오.

15. 10.8.8절에서 설명한 산타페트레일 유전 프로그래밍 알고리즘을 구현하시오.



===== PAGE 456 =====
Chapter 11

정수론 기반 알 아고  고리즘

=     수가 영희에게 인터넷으로 연애 비밀 메시지를 보내려는데 도중에 누가 볼까 걱

정이다. 어떡할까? 메시지를 영희만 알 수 있는 비밀코드로 바꾸어 보낼 수 있다

면, 다른 친구가 그 메시지를 가로채더라도 걱정할 필요한 없을 것이다. 영희만 알 수

있는 비밀코드로 바꾸는 시스템은 정수론 기반 알고리즘을 사용하면 만들 수 있다. 이
장에서는 정수론 기반 알고리즘을 공부해보자.

정수론(0, number theory)-2 A422] 성질을 탐구하는 수학의 한 분야이다. 정수
른 기반 Gaels’ IE 다루는 Bae 푸는 일고리즘을 일런는다. AS 들어, 두 정
수의최대공약수를 찾는 알고리즘은 정수론 기반 일고리즘이라고 할수 있다. 11.1절어서
ARES 간단히 소개하고, 1.3절에서 최대공약수를 We 유클리드 알고리즘을 공부한
다. 1.8절에서는 모듈러 CNIS 간단히 복습하고, 11.4절에서 모듈러 1차방정식을 푸
는 알고리즘을 소개하고, 11.5절에서 모듈러 거듭제곱을 계산하는 알고리즘을 만들어본
|                         다. 11.6절에서는 소수 판정 알고리즘을 공부한다. 정수론 기반 알고리즘을 많이 AE 분
야는 암호학(0》06081820"/이다. 암호학은 전달하는 메시지를 암호로 만들어 제3자가 알
아볼 수 없게 하는 원리를 다루는 학문이다. 11.7절에서는 바로 그 작업을 She Rivest



===== PAGE 457 =====
446     chapter 11 정수론 기반 알고리즘
—Shamir—Adelman(RSA) 공개키 암호체계를 소개한다.
이 장에서는 2~6장과 비슷하게 알고리즘 설계법을 다룬다. 그러나 정수론 기반 알고
Se 정수에 관한 특정 형태의 문제를 푸는 것이지, 2-6장에서와 같이 알고리즘을 설
계하는 일반적인 기술은 아니라는 사실을 염두에 두기 바란다.
@ ll 정수론 소개

정수론의 기본 개념부터 익히고 시작하자.
11.1.1 Bape} 소수
다음은 W-p(integer)2] 집합이다.
Vi er — 2 = (05, 1, 25 wt
임의의 두 정수, ^, h | Zo] 대해서 등식 n= kho] 성립하는 정수 가 존재하면 nS

로 나누어떨어진다(01000)라 하고 Ain OB 쓴다. 다른 말로 nS 의 배수(ㅁ414219),
또는 hE 7 의 약수(010802)라고 한다.

© 예제 111  20=(5)(4이므로 4190로 쓴다. 30은 3으로 나누어지지 않는데, 20=(4)(3)이 성립하는 *가 없기

때문이다.

e 예제 11.2 122] 약수는 1 2, 3, 4, 6, 12이다.

1과 자신을 제외하고 약수가 없는 정수 (> 1)을 소수(6006 ㅁ400000'라고 한다. 소수
가 아닌 정수 n(> 1)을 합성수(600ㅁ00846 ㅁ400060)라고 한다. 합성수는 1과 자신 말고도
약수가 최소한 1개는 있다.

* 예제 113 가장 작은 소수를 10개만 나열해보면,

2, 8, 5, % 1, 08 14 19, 28, 29
이때.

* 예제 114 정수 12 합성수인데, 2, 8, 4, 6과 같은 약수가 있기 때문이다. 정수 4는 합성수인데, 약수 27h

있기 때문이다.

11.1.2 최대공약수

씨7 이고 hlmo}A, hS nF m2] 공약수(60ㅁ1ㅁ0ㅁ 0101800)라고 한다. nF} mo] 둘 다



===== PAGE 458 =====
© 예제 11.5

@0@00@00000
111 AS 소개   447

0°] 아니면 nz} m2] 최대공약수(@7681686 common divisor)= 두 수의 공약수 중에서 가
장 큰 정수이며, gcd(n, 70)으로 표시힌다:

249) 약수는

de 2 3 4, 16) 8, 12) 24
이고, 309} 약수는

1 28656 10 15 30
이다. 따라서 249} 309) 공약수는

1, 2, 3, 6
이고, ged(24, 30)은 6이다.
다음은 공약수에 관한 정리이다.
정리 11.1
이고 himoyA, 임의의 정수 ?와 jo] 대해서
h\(in+jm)
이 성립한다.

증명 : 이고 ^이므로, n=kh} m=lh7} 성립하는 정수 *와 (이 존재한다. 따라서 다음
등식이 성립한다.

in+jm =ikh+jlh = (ik+jl)h

이는 Al(int jm) °] AAAS 의미한다.

더 진도 나가기 전에 알아두어야 할 정의가 몇 개 더 있다. 임의의 두 정수 nak (= 0)
에 대해서 7을 '7;으로 나눈 Rquotient) 0는 다음과 같다.

q= |n/m|
n& m2 나눈 YAZ|(remainder) 은 다음과 같다.

r=n—qm
나머지는 n mod mo = 표시한다. m> 0이면 0 < r< 이고, m<0°Am<r<0
이라는 사실은 어렵지 않게 알 수 있다. 따라서 다음과 같이 정리할 수 있다.

OS  02 > 0

n= gre  이  m<0

(11,1)


===== PAGE 459 =====
@0@00@0000 0
448     chapter 11 정수론 기반 알고리즘

© 예제 11.6

나누기 알고리즘(0101610ㅁ algorithm)S 공부해보면 식 (11.1)의 정수 0와 ro] 존재할
뿐 아니라 유일함을 알 수 있다.

다음 표는 Sa} 나머지를 구한 예이다.

n                 m                  q=|n/m|                         r=n—qn
23                5                   |23/5| =4                        23-(4)(5)=3
-23                5               |-23/5] =-5                   ~23-(—5)(5)=2
23              -5               |23/-5| =-5                 23-(-5)(-5)=-2
-23              -5               |-23/-5]=4                 ~23-(4)(—5)=-3
20                5                   |20/5| =4                          2-(4)(5)=0

> 정리 11.2
과 mS 둘 다 0°] 아닌 정수라 하고,
i, j © 2이고 int+jm > 0인 경우, d= min{in+jm}
이라고 하자. 즉, 0가 과 m2] 1차 조합 중에서 가장 작은 수이면, 다음이 성립한다.
d=gcd(n, m)

명 : ;와 7를 최소값 dS 내주는 정수라고 하자. S, d=in+jmo|y, 또한 7을 0로 나눌
는 KR 은 나머지라고 하자. 그러면 식 (11.1)과 0가 양수라는 사실에 의해서 다음이 성립
TH,

즈
ㅇ
때
한

호

Bo reg

n=qd+r          QOsr<d
따라서 다음을 유도할 수 있는데,
r=n—qd
=n-—q(int+jm)
=n(1—qi) +m(—qj)
이는 7이 nF} 의 1차 조합이라는 의미가 된다. 0는 가장 작은 1%} 조합이고 7<0이므로,
"= 0이라고 결론지을 수 있고, 이는 dn 의미한다. 비슷한 절차로 dm AE 보일 수 있다.
그러므로 0는 과 no] 공약수이고, 따라서 다음 부등식이 성립한다.
0 < gcd(n, m)
ni} 은 모두 ged(n, m) 으로 나누어지고 d= in-+ /이므로, 정리 11 101] 의해서 ged(n, m)id
임을 유도할 수 있다. 따라서 다음 부등식이 성립한다.
0 > gced(n, m)

마지막 두 부등식을 합하면, d= ged(n, m)o] 성립함을 알 수 있다.



===== PAGE 460 =====
© 예제 11.7

© 예제 11.8

0000000
111 정수론 소개   449

800(12, 8) =4이고, 4=3(12) +(-4)8이 성립한다.

v 따름정리 11.1

과 mo] 둘 다 00] 아닌 정수라고 하자. 그러면 /과 m2] 공약수는 HE ged(n, m) 의 약수
이다. 즉, ^0이고 이면, 다음이 성립한다.

h| gced(n, m)

명 : 바로 위의 정리에 의해서 ged(n, 71) 은 7과 m2] 1차 조합이다. 나머지는 정리 11.1에
의해서 성립한다.

~
ㅇ

예제 11.5에서 보여준 대로 24와 302] 양의 공약수는
2 8. 6

이고, 80034, 30)의 값은 6이다. 바로 위의 따름정리가 암시하듯이 6은 1, 2, 8, 6 모두로 나누어
진다.

>» 정리 11.3

n(= 0)과 (> 0)을 정수라고 하자. 7=72ㅠㅁ00ㅠ이면,

gcd(n, m) = gced(m, 7)

이 성립한다.
증명 : 4=0이면 r=mo 되고, 위의 SAS 당연히 성립한다. nH 00]F gyed(n, m)z}
ged(m, ?) 는 서로 나누어짐을 보이면 이 정리의 증명은 완료된다. 왜냐하면 두 Wo] 정수가
서로 나누어진다는 말은 그 Se 같다는 말과 동일하기 때문이다. 이 문장의 증명은 연습문제
로 남기고, 서로 나누어짐만 각각 증명해보자. 먼저 800(08, m)lgcd(m, r) 임을 증명하자. 만약
d’ =gced(n, 70)이라고 한다면, @ |7이고 0 ㅣ7이다. 더구나 다음이 성립하고,
=a

여기서 ge n& mos 나눈 RUG, 이는 7이 nF mY] 144 조합임을 의미한다. 그러므로
정리 11.1에 의해서 @|7이 성립한다. 그런데 | 이고 0@'|7이므로 따름정리 11.1에 의해서
다음이 성립한다.

@ | gcd(m, r)
이제 한 방향의 증명은 완료되었고, Hele ged(m, r)|gcd(n, m)\ YS 증명하자. 만약
0" =800008,7)이라고 한다면, @“^|7이고 @“|10이다. 더구나, 다음이 성립하고,

n=qn+r

여기서 0는 nS mle 나눈 RIG], 이는 no] mI 7의 14} 조합임을 의미한다. 그러므로


===== PAGE 461 =====
450     chapter 11 정수론 기반 알고리

© 예제 11.9

© 예제 1110

OW

정리 11,19] 의해서 d’ |no] 성립한다. 그런데 “이고 @“17이므로 따름정리 11.1에 의해서
다음이 성립한다.

@ | gcd(n, m)

위의 정리에 따르면, 다음 등식이 성립한다.
gcd(64, 24) =800(24, 16)

왜냐하면 16 = 64 mod 240]7] 때문이다. 이런 식으로 계속하면 god (64, 24) 9] 같을 구할 수 있
다 즉

gcd(64, 24) = gcd(24, 16)

=gcd(16, 8)
=gcd(8, 0)
=

11.1.3 소수 인수분해
보타 분 정수는 모두 유일한

을 발전시켜보자.

오열

소수의 곱으로 표현할 수 있다. 이제 이 명제

mu)
olN
of,
ck
pics
ru

(relatively prime)@}a! 한다.

정수 122} @5는 서로소이다. 왜냐하면 800(12, 25) = 1이기 때문이다. 정수 129} 15 서로소가
아니다. 왜냐하면 800(12, 15) = 3이기 때문이다.

> 정리 11.4

hot mo] 서로소이고, 이 AZ 나누어지면 은 #로 나누어진다. 즉, 80008, 72) = 이 성
립하고, //1707이면 /.17이다.
증명 : 정리 11.29] 의해서 다음 등식을 만족하는 정수 St 7가 있다.
ih+jm=1
이 등식의 양변에 7을 곱하면 다음과 같다.
(ni)h+j(nm) =n

이 등식의 좌변에 있는 첫째 항은 *로 나누어진다. 그리고 *1707이므로 좌변의 둘째 항도 h
로 나누어진다. 따라서 좌변은 aw 나누어진다. 이는 no] AZ 나누어짐을 의미한다.



===== PAGE 462 =====
© 예제 11.11

@0000000
11.1 정수론 소개   451

수 9와 4는 서로소이고, 9|72이고, 72=18×4이다. 그러면 위의 정리에 의해서 9|18이 성립
이

Vv 따름정리 11.2
n, mo] 정수이고, p7} 소수일 때, 2177이면, pln 또는 210이 성립한다.

증명 : 정리 11.4로부터 쉽게 증명이 가능하다.

다음 정리는 유일 인수분해 정리(401046 factorization theorem), 그리고 산술의 기초
Ajz](fundamental theorem of arithmetic)@}i1 한다.

정리 11.5

정수 n(>1)2
다음 등식이 성립한다.

역기서 py Ss ape 모두 순수이고, 내므게 abe
p, 2) 차수(6@8000)라고 한다.
증명 : 이런 표현이 가능함을 귀납법으로 증명한다.
귀납기초 : 2=2!
귀납가정 : 2<m< 7의 범위에 속하는 모든 정수 mS 소수의 Fos 표현할 수 있다고 가정
한다.

귀납단계 : no] 소수이면 7 =7?'이다. 그렇지 않으면 /은 합성수이다. 그러면 다음 등식이 성
립하는 정수 2, h> 17; 존재한다.

내
에
lr
o%
re
rlo
ED
트래
ov
+>
es
uu
3
2
쪼

n=mh

여기서 m, ^ <7은 명백히 성립한다. 따라서 귀납가정에 의해서 mah 는 각각 소수의 Bo
로 표현 가능하다. 이를 다음과 같이 표현할 수 있다.

zi

ky ky   ky ht   l,
NM=P, 26 '   ㆍ 2 90? Go 4;

여기에 같은 소수는 하나로 묶고 순서를 증가하는 순서대로 재배열하면 원하는 결과가 나온
다. 따라서 귀납 증명이 완료되었다.


===== PAGE 463 =====
452     chapter 11 정수론 기반 알고리즘
이 곱이 유일하다는 사실에 대한 SBS 따름정리 11.8를 사용하여 증명할 수 있으며, 연습
문제로 남겨둔다.

* 예제 11.12 다음 등식이 성립한다.
22,275 = 3°5711

위의 정리에 의하면 등식의 우변은 유일하다. 4, 다르게 표현하는 방식이 없다.

> 정리 11.6

09
S.
Ss
3
rlo
3
쁘
=

을 인수분해하여 공통으로 존재하는 소수들의 곱이다. 얻어진 곱에 있는

각 소수의 차수는 /과 에 있는 차수들보다 작다.

증명 : 증명은 연습문제로 남겨둔다.

예제 1113 300 = 2"×81×5^이고, 1,125 =3? x 5"의면 800(300, 1,125) = 2 3! x 5?= 얀이다.

11.1.4 최소공배수

최대공약수와 비슷한 개념으로 최소공배수가 있다. nF} mo] 둘 다 00] 아닌 정수라고
할 때 / 과 m2] 최소공배수(16886 common multiple)= 과 mo] 공통으로 가지는 양의
배수 중에서 가장 작은 정수를 말하며, Iem(n, m) 2S 표시한다.

* 예제 11.14  6|18이고 9|18이므로, 10ㅁ(6, 9) =18이고, 그 보다 더 작은 (양의) BYE 없다.

> 정리 11.7

lem(n, m)& 과 mS 인수분해하여 공통으로 존재하는 소수들의 곱이다. 얻어진 Bol] 있는
각 소수의 AGE nt mo] 있는 ARES 보다 크다.
증명 : 증명은 연습문제로 남겨둔다.

*ㅎ예제 11.15 9 12=2?>×3이고, 45 = 3? ×문이면 lem (12, 45) = 2? x3? x 5'= 180이다,

@ 12 최대공약수 계산

정리 11.6에서 두 정수의 최대공약수를 쉽게 계산하는 방법을 알려주었다. 두 정수의 유



===== PAGE 464 =====
© 예제 11.16

> 알고리즘 11.|

11.2 최대공약수 계산    453
일한 인수분해를 각각 찾은 뒤 그 두 인수분해에 공통으로 존재하는 소수를 결정하고,

그 소수들의 곱이 최대공약수이다.  a 곱에 존재하는 각 소수의 차수는 두 정수의
차수보다 작다. 예제 11,1304] 이 과정을 예로 보았지만 다른 예제를 하나 더 보자.

3,185,325 = 35"11"79이코, 7,276,500 = 203"5”71771-이면,
gcd(3,185,325, 7,276,500) = 3"5?11= 7,425이다.

이 방법의 약점은 정수의 유일한 인 으으 찾기가 쉽지 않다는 것이다. 앞의 예제에
서 인수분해가 주어졌으니 망정이지, 인수분해를 찾아보라고 했더라면 어려웠을 것이다.
7자리 대신 25자리의 정수를 베개 한다면 얼마나 어려울지를 상상하기도 싫을
것이다. 사실 정수의 인수분해를 찾는 eae 알고리즘은 아직 없다. 고로, 이제 최대
공약수를 계산하는 좀 더 빠른 다른       즘을 공부해보자.

11.2.1 유클리드 알고리즘

정리 11.1에서 두 정수의 최대공약수를 구하는 쉬운 방법을 배웠다. 그리고 예제 11.9에서
는 그 방법을 예를 들어 보여주었다. 이를테면 800(, m)-& 구하기 위해서 /, = 0이 될
때까지 그 정리의 SAS 재귀적으로 적용한 뒤, 마지막 nS] 값이 최대공약수가 된다.
이 방법은 기원전 300년경에 유클리드(80010)가 알아냈기 때문에 유클리드 알고리즘이
라고 한다. 이 알고리즘은 다음과 같다.

문제: 두 정수의 ABS 구하라
입력 : 양의 정수 nz} So] 아닌 정

출력 : 과 mo] 최대공약수

int gcd (int n, int m)
{
if (mm ==0)
return 7;
else
return gcd(m, n mod m);          // 실제 코드에서는 2 % moe 많이 +
}
* 예제 11.17 알고리즘 11.1을 이용하여 예제 11.16의 수들의 최대공약수를 구해보자.

gcd(7,276,500, 3,185,325) = ged(3,185,325, 905,850)
= ged (90,5850, 467,775)


===== PAGE 465 =====
454

chapter 11 정수론 기반 알고리즘

=800(467,775, 438,075)

= ged(438,075, 29,700)

= gcd(29,700, 22,275)
(
(

gcd (22,275, 7,425)
= gcd(7,425, 0)
= 7,425

유클리드 알고리즘을 사용하여 최대공약수를 구하기는 매우 쉬워 보인다. 얼마나 쉬운
지 알아보기 위해서 이제 알고리즘 11.1을 분석해보자.

| 보조정리 11.1

n>m2>10|51, (알고리즘 11.1에서) 800(/、, m)S k(> 1)번 재귀 호출 한다면,

N= frroth m= frat
이 성립한다. 여기서 /,는 피보나찌 수열의 kA 수이다.
중명 : 귀납법으로 증명한다.
귀납기초 : gcd(n, m)-& 1번 호출한다고 가정하자. 7) =1이므로

m= fio fo
” > 이므로, n> 20] 성립하고, 따라서 다음이 성립한다.
m= firo= fg =2

귀납가정 : *<-1번 재귀 호출하는 경우 이 보조정리가 참이라고 가정한다.
귀납단계 : (> 2)번 재귀 호출하는 경우 이 보조정리가 참임을 증명하자. 그러려면 다음 두
부등식이 성립함을 보이면 된다.

n> /,+;와 m= frst
Al 재귀 SSS ged(m, nmodm)o|t}, 총 재귀 SSO] 《번이므로, 이 호출은 k-1H 재귀
호출이 필요함이 틀림없다. 그런데 《 = 5이므로, 최소한 재귀 SSS 1번은 더 해야 하고, 이
= nmodm > 1°] YASS 의미한다. 여기서 7 > n mod 7이므로 귀납가정 조건이 만족하
고, 따라서 다음 두 부등식이 성립함을 알 수 있다.

n> 77. 와 7ㅁ0027                           0120

이로서 우리가 보이려고 했던 부등식 중 하나는 얻었다. 다른 하나가 성립하는지 증명하기 위
해서 다음 등식을 만들어 보자.

n=qn+nmodm                            (11,3)

여기서 gi 을 으로 나눈 몰이다. 그런데 7>7이고 q> 1이므로 부등식 01.9/와 등식



===== PAGE 466 =====
bi

n=m+nmodm= frrithe= frre

> Be] 11.8

[라메(ㄴ806)] 모든 정수 (= 1)에 대해서 7>7ㅠ =1이고 m< /,이면, (알고리즘 11.1의)
800(”, m) 2] 재귀 호출 회수는 RH 미만이다.

증명 : 이전 보조정리에 의해서 바로 성립한다.

이제 알고리즘 11.1을 분석해보자. 수를 다루는 알고리즘에서 입력이 수인 경우 그 수
가 입력크기로 취급할 수 없는 경우가 있음을     을 9.3절에서 공부한 바 있다. 이   Ags 입력에
필요한 문자의 ASS 입력크기로 본다. 이진코드화 방식을 사용하는 경우 그 수를 코드
화하는데 필요한 비트의 개수(그 수의 18와 대략 같음)를 입력크기로 한다.

최악 시간복잡도(유클리드 알고리즘)
단위명령 : 나머지를 계산하는데 필요한 비트 조작 하나
입력크기 : 7을 코드화하는데 필요한 비트의 개수 6와 mS 코드화하는데 필요한 비트의

개수 t, =

s=|lg m|+1    t=|lg n|+1

일반성을 잃어버리지 않으므로, 1<m< nel 경우만 분석해보자. 즉, 7 =7이면 재귀
호출은 없다. 반면에 m> no} 최초의 재귀 SSS gcd(n, m)o] 될 것인데, 이는 A
인수가 더 크다는 의미가 된다.
시간복잡도를 정확히 구하지는 않는다. 재귀 호출의 BF Calls(s, 1)가 OC) YS 먼저
보이고 나서 최악의 경우 시간복잡도의 한계를 찾는 걸로 대신한다.
Calls (6, t)7} O(t()YS 먼저 보이자. 임의의 m(= 2)에 대해서 /,를 다음 부등식이
성립하는 피보나찌 수열의 수라고 하자.
fm = ME fy                   (11, 4)
8.2.1절의 예제 8.9에서 다음 등식이 성립함을 보였다.
, . Was 760/05-10- 6)/9
              V5
여기서 k— 1°] 홀수이거나, k— 27} 홀수이다. 일반성을 잃어버리지 않으므로, *-1이
홀수라고 가정하자. 등식 (11.5)와 부등식 (11.4)에 의해서 다음 부등식을 얻는다.

(11,5)


===== PAGE 467 =====
456

chapter 11 정수론 기반 알고리즘

[1+ 으시 [1+ 마프           어이
등식 01.4에 의해서 정리 1.8로부터 다음 부등식을 유도해낼 수 있다.
Calls(s, t)<k                              (11,7)
부등식 (11.6)과 (11.)에 의해서 다음이 성립한다.
Calls(s, t) 6 O(t)                     (11,8)

800(/,+ 1 f= 계산하는데 정확하게 ㅡ-1번의 재귀 SSO] 필요하다는 사실의 SBS
연습문제로 남겨둔다. Wealls(s, t)S 입력크기 6, tol 대해서 최악의 경우 재귀 호출 횟
수라고 할 때 다음이 성립한다고 결론지을 수 있다.
Wealls(s, t) € 0 (0)

재귀 SSS 할 때마다 나머지 하나를 계산한다. 나머지를 계산하는데 (2.6절에서 공부한)

표준적인 큰 정수 Ue 알고리즘을 사용하면, m < nd BF r =n mod mg 계산하는
데 필요한 최악의 경우 비트조작 횟수의 상한은 다음과 같다.
이(1 + 18 0)18 m]                                   01.9)

여기서 0는 을 으로 나눈 Hola, 는 상수이다. 이에 대한 증명  5  연습문제로 남겨둔
다. 충분히 큰 입력크기에 대해서 7 > 0이면 7을 계산하기 위해서 필요한 최악의 경우 비
트조작 횟수의 상한은 다음과 같다.

cl(1+ lg n)lg m—lg m lg 7]                       (11,10)

결국엔 g=(n—r)/mo|al, 1 < r< moles, 다음과 같이 유도할 수 있다.

1+166=1+81그|

SS 1+1g(2—]

n
= 1+1g("]
= 1tlen—ler
이 부등식과 상한 (11.9)를 이용하여 상한 (11,10) 구할 수 있다. 이 상한으로 모든 재귀
SSA 나머지를 모두 구하는데 필요한 총 비트조작 횟수의 상한을 구하면 다음과 같다.
c[(1+lg n)lg m—lg 72 18 7
1+18 m)lg r—lg rlg(m mod r)

{
+(141gr)lg(m mod r)— -+]
=c(lg nlgm+lgmtlgr+lg(m modr)+ -+]             (11,11)



===== PAGE 468 =====
@0000000
1.2 최대공약수 계산   457

관계 (11.8)로 재귀 호출의 횟수는 가 상한임을 유도할 수 있다. 여기서 dE 0보다 큰
상수이다. 이는 상한 01.11)에서 항의 개수 상한이 임을 뜻한다. 따라서 2 > 72 > 7 >
mmod 7 > … (여기서 점은 상한 (11.11)의 나머지 SS 나타냄)이므로, 상한 (11.11)로부
터 다음이 성립한다고 결론짓는다.

W(s, 7) © O(st)

11.2.2 유클리드 알고리즘의 확장
정리 11.1에서 다음 등식이 성립하는 정수 ih 7가 존재한다고 결론지었다.

gcd(n, m)=in+jm
다음 절에서 공부할 모듈러 1차 방정식을 푸는 알고리즘에 이 정수값이 중요한 역할을
한다. 이제 알고리즘 11.1을 수정하여 같은 APS 찾아내도록 해보자. 이 알고리즘에서
800를 변수로 놓는 이유는 알고리즘의 정확성을 더 투명하게 증명할 수 있기 때문이다.

> 알고리즘 |1.2     유클리드 알고리즘 2

문제 : 두 정수의 최대공약수를 계산하라,
입력 : 양의 정수 nah So] 아닌 정수 m

출력 : nat 의 최대공약수인 800와 800= int 777가 만족하는 정수 it j

void Fuclid (int n, int m, int& gcd, int& i, int& ./)

{
if (77 ==- 0) 4
ged =n 1S 1h 7 = Os
}
else {
int) 774 ged":
Euclid (zm, 2 mod m, gcd’, i’, 7);           // C++ 44334 2 % m
gcd = gcd’;
= 0
j= i |n/mls'
}
}

알고리즘 11,29] 시간복잡도는 알고리즘 11.1의 시간복잡도와 명백히 같다. 그러므로
그 알고리즘의 정확성만 증명하면 된다. 증명하기 전에 알고리즘이 어떻게 작동하는지
먼저 예를 들어 살펴보자.


===== PAGE 469 =====
458     chapter 11 정수론 기반 알고리즘
* 예제 11.18 알고리즘 11.2에서 A 호출이 다음과 같을 때,

Puclid(42, 30, gcd, i, 7)

의 흐름은 표 11.1과 같다. ABE ged=6, i=-2, 7=3이다.

ㅇ
노새

고리

nu
oN

@ 표 11.1 n=42,m=300! 경우 알고리즘 11,29] 계산 과정. A 호출은 0으로 표시하고, 3H
의 재귀 SSE 각각 1, 2, 3으로 구분한다. 화살표는 값이 구해지는 순서를 표시한다.

호출             n              m             ged              i               j
{                  {

0                         42                        30                         6                         =o                         3
1                         30                        12                         6                          1                         고

2                             12                             6                              6                             0                              1

8                          6                          0                          6                          1                          0

=                =                 t                  t                  t

> 정리 11.9

알고리즘 11.2로 계산한 값 iSt jE 다음 등식이 만족하는 정수이다.
gcd(n, m) =in+jm
증명 : 귀납범으로 증명한다.
귀납기초 : 마지막 재귀 호출에서 7=0이다. 이는 80002, m) =7임을 의미한다. 12} 72] 값
은 각각 1과 0이므로 이 호출에서 다음이 성립함을 알 수 있다.
ixnt+jxm=1Xnt+0Xm=n=gcd(n, m)
귀납가정 : kVA 재귀 호출에서 {와 )의 같은 다음 식을 만족한다고 가정하면,
gcd(n, m) =in+mj
그 호출이 넘겨주는 값 『 과 7 은 [(&-1)째 재귀 호출에서 쓰임] 다음 식을 만족한다.
gcd(m, n mod m) = 2 72 +ㅜ7 72 mod m
귀납단계 : (&-1)째 호출에서 HSS 유도할 수 있다.
int+mj =jnt+(i— Ln/m! 7’)m
=imt+j (n-  Ln/m 1 m)
=i'm+j'n mod m

=gcd(m, n mod m)

=gcd(n, m)

맨 아래에서 둘째 등식은 귀납가정에 의해서 성립하며, 마지막 등식은 정리 11.30 의해서 성
립한다.



===== PAGE 470 =====
@0‥ㅎ0006006000 0
11.3 모듈러 연산 소개    459

마지막 재귀 SSA] 알고리즘 11,27} 계산한 Fete 임의의 정수일 수 있다. 쉽게 설
택           Is 4            d(n, m)=in+ jmo| 성립하

'
ay
Ol
에
'
에
Py
09
<3

 1,3 모듈러 연산 소개

그룹이론(37042 theory) 2] 관점에서 모듈러 AAR 소개한다. 먼저 그룹이론을 공부
해보자.
11.3.1 그룹이론

집합 SOA] 닫힌 이진연산(20860 binary operation) ＊는 집합 So] 속한 두 원소를 결합
하여 So] 속한 다른 ASS 만들어내는 규칙이다. 이는 다음과 같이 정의한다.

정의

=

그룹(9040) G=(S, + )은 집합 와 다음을 만족하는 의 닫힌 이진연산 ＊으로 구성한다.
1. ＊는 결합법칙이 성립한다. 즉, BE a, 0, ㅇ & SO 대해서 다음 등식이 성립한다.

* (b*c)=(a *b) *c

2. 집합 Sol 항등원00670\/ element) ㅇ가 존재한다. 즉, 각 ㅇ = soll 대해서 다음 등식이
성립한다

ll

a
3. Z2ba & SO 대해서 다음 miles, ar   역원 — element) a’ 이 존재한다.

i
a*a =a *a=e

* 예제 11.19 8p 집합 와 덧셈은 그룹을 이룬다. 항등원은 0이고, al] AAS -0이다.

* 예제 11.20 0°] 아닌 실수와 BAS 그룹을 이룬다. 항등원은 1이고, a2] 역원은 1/0이다.

* 예제 11.21 S=(a, 6, 0/이고, 다음 등식이 성립한다면,

a*b=b*a=e

a*a=b
b*b=a
a*e—er*a=a
b*e=e*b=b
e*e=e

(S, *)7} 그룹임을 증명하는 작업은 연습문제로 남겨둔다.



===== PAGE 471 =====
@‥06@0060000 0
460   chapter 11 정수론 기반 알고리즘

그룹에서 한 원소에 하나 이상의 역원이 존재할 수 있는가? 다음 정리는 그렇지 않음
을 보여준다.

> 정리 11.10
그룹에서 각 원소의 역원은 하나밖에 없다.
증명 : 과 a" 가 둘 다 aM 역원이라고 가정하면, 다음 등식이 성립한다.

> 정리 11.11

ABA] a* b=a BE b*a=a7} 성립하는 원소 0와 67} 존재한다면, b= 그 그룹에서 BS
원 6가 된다.

증명 : a*b=all 경우, 다음 등식이 성립한다.
a’ * (a*b) =a’ *a=e
여기서 0 는 0의 역이다. 그러나 다음 SAE 성립한다.
a * (a*b) =(a' *a) *b=e*b=b

이 두 SAS 결합하여 a+ b= oF 증명한다. 8＊0ㅇ=<도 같은 방식으로 증명한다

그룹에서 항등원이 하나밖에 없음을 앞에서 확인하였다.
BE a, b= 에 대해서 다음 등식을 만족하는 그룹 C= (6, ＊ )은 교환법칙(00ㅁ-

mutative, 800182)이 성립한다고 한다.

0*0=0*0
집합 SO] 포함된 원소의 개수가 유한한 그룹 G=(S, * )를 유한한 그룹(626 group)°]
라고 한다. 예제 11,19, 11,20, 11.21의 그룹은 모두 교환법칙이 성립하지만, 유한한 BS
예제 11.21의 그룹뿐이다.

[도
=

11.3.2 nB 법으로 한
용어부터 정의해보자.

[에



===== PAGE 472 =====
© 예제 2.2

© 예제 11.23

@eeee0 0
118 모듈러 연산 소개    461

정의
와 k= 정수이고, 7은 양의 정수라고 하자. 여기서 (7 -ㅅ)인 경우, mS nS WHS
로 하여 와 SHS0|CKm is congruent to k modulo ?0)라 하고, 다음과 같이 쓴다.

m=kmodn

5|(33-18) JH =,
33 =18 mod 5

mS 7으로 나눈 나머지는 m mod 7이다. 다음 정리를 공부하여 mod 함수를 써서
합동임을 알아낼 수 있음을 익히자.

> 정리 11.12
=*1ㅁ007의 필요충분조건은 다음과 같다.

m mod n= k mod n

증명 : 연습문제로 남겨둔다.

33 = 18 mod 5임은 이미 안다. 바로 위의 정리를 적용해보면 33 mod 5 = 18 mod 5 = 3가 성립
한다.

다음은 합동에 관한 정리로 11.7절에서 RSA 암호시스템을 이해하는데 필요하다.

> 정리 11.13

My 70, 은 모든 쌍이 서로소(681'186 relatively ㅁㅁ0006)이고, 7은 다음과 같이 놓자.
N= Ng N;

dh

그러면 “모든 정수 mt *에 대해서 m =k mod no] 성립함"의 필요충분조건은 “1
대해서 m =k mod n,°] 성립함"이다.

증명 : 1 <i = jo] 대해서 다음이 성립한다고 가정하자.

lA

i< /에

m =k mod n;
그러면 다음 등식이 성립하는 정수 hy, hy, …, 들이 존재한다.

m—-k=hyn, = 72222 = … = 222,


===== PAGE 473 =====
@‥0@00000 0
462   chapter 1 정수론 기반 알고리즘

이 등식이 성립하고 n,, ny ㆍ‥, 의 모든 쌍이 서로소이면, 다음 등식이 성립함을 뜻한다는

hy =engng 111 1;
여기서 는 정수이다(이 등식의 SUS 연습문제로 남겨두니 정리 11.48 이용하여 증명해보
기 바란다). 그러면 다음 등식이 성립한다.

m—k=hyn, = (022 --- n;)n, =en

다른 방향을 증명해보자. m=k mod 7이면, 다음 등식을 만족하는 정수 /가 존재한다.
m—k=hn
따라서 다음 등식이 성립하고
72 -ㅅ= 22722 00 n;

이는 각 에 대해서 m—k= 의 배수(ㅁ4147216/임을 뜻한다. 증명이 완료되었다.

* 메제 11.24 정수 2, 5, 9는 모든 쌍이 서로소이고, 타음이 성립한다.

184 = 4 mod 2
184=4 mod 5
184 = 4 mod 9

2×56>×9=090이므로, 위의 정리에 의해서 다음이 성립한다.
184=4 mod 90

다음 정리는 nS HOS 한 합동은 동치관계(60447816006 relation) YS 보여준다.

> 정리 11.14
임의의 양의 정수 에 대해서 n& 법으로 한 WES 정수의 집합과 동치관계이다. 즉,
1. (반사)
m =m modn
2. (대칭)
m=kmodn >  k=m mod n
8. (추이)

m=kmodn A k=j modn => m=jmodn

증명 : 연습문제로 남겨둔다.



===== PAGE 474 =====
000000 0
11.9 모듈러 연산 소개    463

n& 법으로 하여 ma 합동인 모든 정수의 집합을 ms 포함하고 ns 법으로 한 동치
(equivalent class modulo n containing m)z} 한다. 합동은 동치관계이므로 주어진 류
(class) 내부의 정수가 그 류를 결정한다. 주어진 정수 mol] 대해서 그 집합은 다음과 같다.

mtinliEc 2

* 예제 11.25 133 포함하여 6S 법으로 한 동치류는 다음과 같다.
Uns “1, 8 8 8 28, 18, 28 BE, Be, ,

m& 포함하여 n& 법으로 한 동치류를 [m], 22 표시한다. 따라서 바로 위의 동치류
는 [13], 로 표시한다. [3], 또는 [8], 등으로 표시할 수도 있다. 보통 SL 가장 작은 양의

정수를 WES 표시하는 것이 일반적이다. 따라서 위의 예제에서 동치류는 보통 [3],으로
표시한다. nS 법으로 한 모든 동치류의 집합은 2, 으로 표시한다. =

2, = [이 [다 9 lait

* 예제 11.26 Z; = {[0];, 416 216 816 41}

Z, 속해 있는 두 원소에 대해서 덧셈(60014020/)을 다음과 같이 정의한다.
121, + lk], = [m+ kl],

이 정의가 말이 되기 위해서는 계산 결과가 [721,과 [],에서 어떤 원소를 선택하더라도
그 값에 종속되지 말아야 한다. 이를 증명해보자. 다음이 성립하는지 보여주면 된다.
s€[m], 이고, 1 |시,이면, s+telm+k], oc.

결국 다음 두 SAS 만족하는 정수 :와 가 존재한다.
s=mtin       t=k+jn
따라서 다음 등식이 성립하고,
stt=m+k+(itj)n
이는 다음이 성립함을 뜻한다.

8ㅎ+?ㄷ[22 +ㅜ시,

= 예제 11.27    [2]; 1s [4]; 덜 [6]; = [1];



===== PAGE 475 =====
464     chapter 11 정수론 기반 알고리즘
> 정리 11.15
BE 양의 정수 nol] Ha (Z,, +)는 유한 교환그룹(80116 commutative group)°]tt,
증명 : +는 정수에 대해서 결합 및 교환법칙이 성립하므로, 위의 +도 결합 및 교환법칙이 성립
함을

© 예제 11.28

© 예제 11.29

© 예제 11.30

바로 알 수 있다. BSL (identity 6160601)은 [0], 이다. 101], 의 BAA (additive inverse)-2
m), =l-m],,°] 되는데, 왜냐하면 다음 등식이 성립하기 때문이다.

Im], +[-m], = 020 +(-022)1 = 101,

?

룹 (Z;, +)S 보자.
Z; = {[0];, 0406 216 816 41}
19 덧셈역은 [[ㅡ1] = |4];이다. 그러면,
(1); + [4]; = [5] = [0
비슷하게, [2],의 덧셈역은 13],이다. 그러면,

121. ㅠㅠ [3]; = [5]; 고 (ol;

2,에 속해 있는 두 원소에 대해서 BAT (multiplication) 다음과 같이 정의한다.
[m],, X[k], = [22 × 시,

이 정의가 말이 되기 위해서는 계산 결과가 [71], 과 lk], AA 어떤 원소를 선택하더라도
그 값에 종속되지 말아야 한다. 다음이 성립하는지 보여주면 된다.

8드[70], 이고, 1ㄷ[/],。이면, ㅎ×7ㄷ[22×시,이다,

증명은 연습문제로 남겨둔다.

[2]; x [4]; = [81 = [3],

곱셈역이 없는 요소가 존재하는 Z,, 0] 존재하기 때문에 (Z,. ×)은 항상 그룹이라는 보
장이 없다. 즉, [11,을 항등원으로 한다면, [74], x [bly = [11, 이 성립하는 《가 없는 lm,
이 존재한다는 뜻이다.

다음 집합을 생각해보자.
Zy 10], 1 21, 18. 216, 5]q, 이, [7]g, 81. t



===== PAGE 476 =====
© 예제 11.31

@0000000
1.3 모듈러 Ast 소개    465

6];는 곱셈역 [ko] 있다고 가정하자. 그러면 다음 등식이 성립한다.
[6], X [ky = [6 x ky =[1]g
이는 다음 등식이 성립하는 정수 17} 존재하다는 뜻이며,
1=6k+9
따라서 정리 11,20] 의해서 1°] ged (6, 9)가 되며, 이는 명백히 말이 되지 않는다.

위 예제의 문제점은 6과 9가 서로소가 아니라는 것이다. 7에 서로소인 수만 포함시킨
다면 그룹을 이룰 것 같아 보인다. 다음 정리에서 이것이 사실임을 증명한다. 먼저 이
집합을 만들기 위한 표기법을 정의해보자.

Z,, = {[m], € Z, | [m], 의 ARE 7에 서로소이다}
WS] no] 소수이면 2, = 2 - [0]. ‘Im], 집합의 한 원소가 에 서로소임"의 Bae

그 집합의 모든 원소들이 그러함"이다. 따라서 Z; 의 원소를 구하기 위해서 A
“19 정수만 살펴보면 된다.

내    Ac     of
IN

> MP] 11.16

모든 양의 정수 nol] 대해서 (2, ×)는 유한 교환그룹이다.

증명 : 따름정리 11.20] 의해서 mk k= 나누어지는 FE 7 으로 나누어지거나 *로 나누어져
of 한다. 그러므로 mI 《가 각각 mol 상대적으로 소수라면 m x kE 에 상대적으로 Apo]
며, 이는 ×가 2;에서 닫힌 이진연산자임을 뜻한다. ×는 정수에 대해서 결합 및 교환법칙이
성립하므로 위의 x= 결합 및 교환법칙이 성립함을 바로 알 수 있다. 항등원은 [1], 이다. mo]
no] 상대적으로 소수라면 정리 11,20] 의해서 다음 등식이 성립하는 정수 :와 7가 존재한다.

1 = 272 + 7772
이는 다음이 성립함을 의미하고,
777 =1 mod n

따라서 !/],은 fm], 역이다.

© 예제 11.32 군 (26, ×)에 대해서 다음과 같은 곱셈역이 존재한다.

[1] x [1], = 006


===== PAGE 477 =====
466     chapter 1 정수론 기반 알고리즘
[2], x [5]p = [10], = [1],
[4 ls x [7], = 글 [28], = [1],
[8], x [8], = [64], = [1],
> Be] 11,17

© 예제 11.33

© 예제 11.34

© 예제 11,35

Z, 2] 원소의 개수는 다음과 같은 오일러의 함수(84168 totient function)= 구한다.
^2)=71] |

1
1 때도
p:pin  a
여기서 곱은 7으로 나누는 모든 소수에 대한 곱이며, no] 소수인 경우에는 n= 포함한다.
증명 : 그라함(37888200)과 그의 동료들이 1989년에 발표한 논문에 증명이 있다.

?가 소수이면 다음 등식이 만족함을 눈여겨 봐두자.

ZA 원소의 개수는 다음과 같다.

al

예제 11.81에서 세어보면 확인할 수 있다.

Zo A 원소의 개수는 다음과 같다.
0) =00[|-끄|=001-글| 0 (1-4}=16

70] 소수이므로, 않에서 원소의 개수는 다음과 같다.

6(7)=7-1=606

11.3.3 부분그룹
G=(S, * )7} 그룹이고, $’ 드 5이고, 0 = (6'", * )7} 그룹이면, GE GF 부분그룹
(subgroup)°]@}a1 한다. 그리고 S’ + SO} 진부분그룹(60006 84087042)이라고 한다.



===== PAGE 478 =====
@0@000000
1.3 모듈러 연산 소개 467

* 예제 11.36 ㅅ를 짝수의 집합, ZS 정수의 집합이라고 할 때, (4; +)는 (> +)의 진부분그룹이다.

AES 더 나가기 전에 용어를 몇 개 알아보자. 그룹 C= (9; ＊)에 대해서 ae $9}
그 Ya’, k> OL 다음과 같이 정의한다.

>

a=~-a*ta*-:---a        《번
a=]
a (0 0"
그룹 0= (6, ＊)와 0, 0 ㄷㄷ 6", ath © "가 성립하는 부분집합 6" 드 6에서 S'S
* 에 관하여 닫혀있다(00860)라고 한다.

> Bel 11.18

유한그룹 G=(S, ＊)와 *에 관하여 닫혀 있으며 Fo} 비어 있지 않은 부분집합을 90] 있다
하자. 그러면 (9, * )는 GO] 부분그룹이다.

증명 : 결합법칙은 명백히 성립한다. a © "이라고 하자. G7} 유한하기 때문에 다음 SAS
q                  m> 1이 존재함을 증명하는 작업은 연습문제로 남겨둔다.

이 SAS] 양변을 “의 역을 곱하면 다음과 같이 된다.

여기서 는 항등원이다. 5S 닫혀 있          는 “에 속한다. 다음으로 6" 집합에 속한 모
든 0의 역도 S'o] 속함을 증명해보자. rer 본대로 그런 모든 0에 대해서 ㅇ=ㅇ이 성립하는
m0] 존재한다. ㅠ=1이면, a=e( a2} 역이 ㅇ임을 의미함)이고, e7} 5” 집합에 속한다는
사실은 이미 알고 있다. 그렇지 않으면 다음 등식이 성립한다.

=
€=G4 0000"

이는 0" 10] 의 유일한 역임을 뜻한다. 그러나 %" 집합이 닫혀 있으므로, 0” 1g. 에 속한
다. 증명이 완료되었다.

> Bel 11.19

(라그량제) 유한그룹 C= (5, ＊)와 부분그룹 C= (5", * )이 있다고 가정하면 다음이 성립
한다.
Is’ 11S


===== PAGE 479 =====
@00@00000 0
468   chapter 11 정수론 기반 알고리즘

© 예제 11.37

© 예제 11.38

여기서 |S HE 에 속한 원소의 개수를 나타낸다.
증명 : SBS 1951년에 발표된 제이콤슨(03000802)의 =H 있다.

그룹 (Cy, HAA 다음이 만족함을 증명하는 작업은 연습문제로 남겨둔다. 다음 등식이 만족
하면,

@"= {[0],25 (Blam 1610 191}
(9", +) Zin +)의 부분그룹이다. 위의 정리에 의하여 |6“|=4, |2,,1=12, 4127+ 성립한다.

v 따름정리 11.3

@ =(S", + )이 G=(S, *) 9] 진부분그룹이라면, 다음 부등식이 성립한다.
ls’ |= 181.

증명 : 위 정리에 의해서 바로 성립한다.

G=(S, * )가 유한그룹이고, a= Sole} 하고, 다음과 같이 정의해보자.
<a>= {a* |k 양의 정수}

여기서 (a> 명백히 *에 닫혀 있다. 따라서 정리 11.18 때문에 (<a>, ＊)는 G2] 부분
그룹이다. 이 그룹을 aol] 의해서 생성된 부분그룹(6408704ㅁ0 8606『8660 by 0/)이라고 한
다. al] 의해서 생성된 부분그룹이 GEA, aS G2] BAV7|(generator)e}a1 한다.

그룹 (2, HAA 다음을 얻을 수 있다.
= [2], ee 11216, ie lle 바키 25 [2], +ㅜ[21610] + [ales }

부분그룹을 생성할 때 항등원을 일단 구한 이후에는 이미 생성된 원소가 반복되기만
하기 때문에 멈추어도 괜찮음을 바로 위 예에서 보여주었다. 다음은 이 결과를 정리한
것이다. 다음 정리를 기술하기 위해 정의 하나가 필요하다. 임의의 그룹에서 그룹 원소
a2] 차수(0ㅠ060)는 “ord(a)"= 표시하며 a! = eS 만족하는 가장 작은 양의 정수 *이다.
여기서 6는 항등원이다.

> 정리 11.20

G=(S, ＊)가 유한그룹이고, a © 이라고 하자. ?= 070(0)이면 0에 의해서 생성된 부분그룹



===== PAGE 480 =====
© 예제 11.39

© 예제 11.40

@0000000
11.3 모듈러 연산 소개     469

are 다음과 같이 서로 다른 개의 원소로 구성되어 있다.

증명 : 먼저 이 원소들이 서로 다름을 증명해보자. 1 = ㅅ&< ) = (를 만족하는 *와 )에 대해서
다음 등식이 성립한다.

7 > *이므로, > 1에 대해서 다음 등식이 성립한다.

a! = a’
바로 위의 두 등식과 정리 11 119] 의해서 a! =e YS 유도해낸다. 그런데 1 <?이므로, 이는 논
리적으로 모순이다. 다음으로 이 부분그룹에 다른 PAL 존재하지 않음을 증명해보자. * >
이면, 다음을 만족하는 양의 정수 go} ro] 존재한다.

k=qt+r      O=r<t

그러면 다음 등식들을 얻는다.

a® = qtr) — (a‘)4 a =ed=a

만약 r=00)4 a” =e=a'7} 성립하고, 그렇지 않으면 1<r<t7} 성립한다. 증명이 완료되
었다.

바로 위 정리에 의해서 ?= 0ㅁ0(0)일 때, 다음 등식을 얻는다.
<a>= {a, al, …, @ 나

여기서, <a> 2] 원소의 개수는 ord (a) VS 주목하자.

그룹 (Ze +)에서 다음 등식이 성립한다.
< 13] > = {1816 116 + 81} = 1316” 0}
< [216 > ={[2]g 1216 ㅜ[216 1216ㅜ[21 +[21}= {1216 416 101}
여기서 명백히 다음 등식이 성립하고,
([16>=Z¢
따라서 [162 2;의 생성기이다.

이전에 공부한 그룹 (28, ×)를 살펴보자.

26 = {016 216 410 (lg, [06 81}


===== PAGE 481 =====
@0000000
470     chapter 11 정수론 기반 알고리즘

© 예제 11.41

© 예제 11.42

< 41, > = {416 [Aly x lo [ly x [Aly x [4]}= {L4lo, 00600}
여기서 다음 등식이 성립하며
([2],)=Z
식의 증명은 연습문제로 남겨둔다. 따라서 [2],은 2;의 생성기이다.

의

oft

그룹 (zi, ×)를 살펴보자.
갔={비 216 (ly [ly ly, (61,}
음을 얻을 수 있다.

< [4] > =근418 [4], x 4], [4], x (4), x (4), }= (4); 218 00}

v 따름정리 11.4

G=(S, ＊)가 유한그룹이고, a ㄷ 6이라 가정하고, =070(0)이라고 하자. 그리고 다음 수열
을 생각해보자.

0 1
Qin Gs 세아

이 수열에서 두 AA aS} a7} 같음의 필요충분조건은 다음과 같다.
2= 7 mod 7

이는 의 수열이 tS 주기로 순환적이그, te SSA 가장 작은 주기이대: 즉| 0 스와

i209 모든 iol] 대해서 다음 등식이 성립하고, t= 이 성질을 가진 가장 작은 수이다.

277 — ak

증명 : 바로 S 정리를 이용하여 증명가능하며, 연습문제로 남겨둔다.

그룹 (2;, ×)를 살펴보자. 다음 HE [4],의 거듭제곱을 보여주

1] 0 1 2 38 4 56 7 8

([416)' )| 바빠 이바 바바 4s Gl ls; 0

다음 HE 13],의 거듭제곱을 보여준다.

0] 0 1 2 3 4 56 7 8
Hl; Gl ll 바바 l 바바 Ol;

이 그룹에서 ord([4];) = 22} ord([3];) =4가 성립한다. 따름정리 11.4에서 암시해주는 바와 같이



===== PAGE 482 =====
© 예제 11.43

@‥60060000 0
11.3 모듈러 연산 소개    471

이 차수에 관해서 거듭제곱의 순환적인 SS 주목하자. 더욱이 [3],은 2;의 생성기임도 주목하
자.

v eae] 11.5

G=(S, ＊ )를 항등원이 <인 유한그룹이라고 하자. 그러면 a © $l BE 0에 대해서 다음 등
식이 성립한다.

291 _ ,

여기서 ISH 집합 Soy 속한 원소의 개수를 나타낸다.

증명 : 정리 11.20으로부터 al 의해서 생성되는 부분그룹 <0>에 속한 원소의 APE ord(a)
임을 알 수 있다. 그러므로 정리 11.19로부터 어떤 정수 《에 대해서 |9|=ord(a) ×*이고, 따라
서 다음 등식이 성립한다.

als! = gorda) xk = <

증명이 완료되었다.

> 정리 11.21

(오일러) n> 1인 임의의 정수 nol] 대해서 721, | 2; 인 모든 lm], 대해서 다음 등식이 성립
환대:

00230
증명 : 정리 11.17과 따름정리 11.5에 의해서 바로 성립한다.

그룹 (Zyy, ×)를 살펴보자. 다음과 같이 계산할 수 있다.
y(20) =20 ] | [:-4}-20(1-2}(1-4]+s

p: pl20
그리고 앞의 위 정리에 의해서 다음 등식이 성립한다.
Claas” a 6561] 5, 바커

> Mel] 11,22
(페르마) 7가 소수이면 [ml], < Ze] 모든 07],에 대해서 다음 등식이 성립한다.



===== PAGE 483 =====
472     chapter 11 정수론 기반 알고리즘

© 예제 11.44

증명 : 바로 위의 정리와 p7} 소수인 경우 o(p) =7-1이 성립한다는 사실로부터 증명이 가능
하다.

군 (2;, ×)를 고려해보면, 위의 정리가 암시해주듯이 다음 등식이 성립한다.

({2],)’~* = [64], = [1],

Se 114

모듈러 14 방정식 풀기

© 예제 11.45

이제 아래 모듈러 방정식을 푸는 방법을 공부해보자.
[m], c= Ik],                                         (11,12)

여기서 cE n& 법으로 한 동치류이고, m, n> 0이다. 11.7절에서 884 암호시스템을
개발할 때 이 AHS 적용한다.
그룹 (Z,, +)에 상대적인 [01],에 의해서 생성되는 부분그룹을 <[71], >이라고 하자.
<[041』>= 니이, 01, [2m], … } 이므로 “등식 11,127 해를 가지고 있음"의 필요충분
조건은 다음과 같다.
[x], = <[m],,>

그룹 (Zz, +A] 다음이 성립하므로
<[6],>= 11016, 1616 416, Pia

등식 6], i [k],2] 해가 존재함"의 필요충분조건은 [k],°] [0], 또는 00 또는 [416 또는 [2]。이다.

다음 정리는 집합 (Im), 9 원소를 정확히 알려준다.

> 정리 11.23

그룹 (2。, +)을 살펴보자. Im], = 2,에 대해서 다음 등식을 얻는다.
(im), >= (Id), = {l0ln» [dla dl,» +++ [n/d—1)d],,}

여기서 d=ged(n, 70)이다. 이는 다음 등식이 성립함을 의미한다.

n

ord([m],,) =< im], >1 = :



===== PAGE 484 =====
@   0000 0
11.4 모듈러 iat 방정식 풀기     473

증명 : 먼저 <[0|。>드 <111。>가 성립함을 보이자. 정리 11,20] 의해서 다음 등식이 성립하는
정수 id} )가 존재한다.
d=im+jn
이 등식에 의해서 임의의 ko] 대해서 다음이 성립한다.
kd = kim mod n
이는 [kd], =lkim]),°] 성립함을 의미하고, 따라서 [kd),]<Im],°] 성립한다. 그러므로
<], >드 <], >가 성립한다고 결론지을 수 있다.
다음으로 <101]。>드 <101,。>가 성립함을 보이자. 47, 이므로, m= idel 정수 :가 존재한다. 따
라서 임의의 정수 《에 대해서 다음 등식이 성립한다.
[km], = [kid],
이는 [km],€< Id], >°] SHAS 의미하고, 따라서 <[m],,)¢S <101,>이 성립한다고 결론지을
수 있다.

최종 결과는 바로 보여준 결과들과 정리 11.20에 의해서 성립한다.

Vv 따름정리 11.6
“등식 (ml, =[h], 2] 해가 SAWS] 필요충분조건은 “d= god(n, 7/)인 경우 01 &가 성립함"이
다. 더구나 이 등식의 해가 존재하면 해의 개수는 0이다.
증명 : 이 절의 서두에서 언급했듯이 “등식의 해가 존재함"의 필요충분조건은 다음과 같다.
시, = <, >
정리 11,236] 의해서 다음을 유도해낼 수 있고,
lm), >= Cdl, )= 10, (yy 90. «+ [(n/d-1)all,}

이는 이 등식의 해가 존재함의 필요충분조건은 임의의 ㄷ [에 대하여 01&가 성립하는
것임을 의미한다. [],는 nS 법으로 한 동치류이고 00이므로, % © (kl, 2 하나의 “에 대하
여 d| 가 성립함”의 명백한 필요충분조건은 [\|,의 WE 원소에 대해서도 성립하다는 것이다.
이 따름정리의 앞부분은 증명이 완료되었다.

두 번째 부분의 증명을 해보자. 정리 11.98에 의하여 ord(lm],,) =7/0이다. 따라서 따름정리
1.4에 의해서 다음 수열은 n/d 주기를 가지고 있고, 그 중 최초 n/a] MASS 서로 다르다.

이는 [ele (im), ola, 다음 집합에서 4],이 정확히 0번 나타난다는 의미가 된다.



===== PAGE 485 =====
@0@00000 0
474     chapter 11 정수론 기반 알고리즘

© 예제 11.46

© 예제 11.47

© 예제 11.48

이들이 나타나는 이유는 7.9] 다른 원소이기 때문이다. 증명이 완료되었다.

 따름정리 11,7
다음 등식이

(m],,2 = (kl,

모든 동치류 [l,l 대해서 해가 존재함의 필요충분조건은 ged(n, m)=1 이다. 만약 이게 사
]이라면 각 4[,의 해는 유일하다.

명 : 따름정리 11.6에 의해서 바로 성립한다.

ne

2

v 따름정리 11.8

“동치류 [m],°] n& 법으로 한 곱셈역을 가짐"의 필요충분조건은 800, m) = 1이다. 즉, “등
식 071.』=[11,의 해가 존재함"의 필요충분조건은 8000, 1) = 1이다. 더구나, 그 해의 역이
존재하면 그 역은 유일하다.

명 : 따름정리 11.6에 의해서 바로 성립한다. 유일함은 정리 11.16에 의해서 성립한다.

oly

그룹 (2,, +)-& 고려해보자. 800(8, 6) = 이므로, 정리 11,230] 의하여 다음 등식이 성립한다.

ㅣ 결과는 예제 11,459} 일치한다. 따름정리 1.6에 의해서 등식 [6], o = [kl] SHE <16]。>의
원소가 [kl Ql 경우 정확히 두 개 있다. 예제 1.45014 Uhl, v= [4],인 경우 두개의 HE w=

ㅇ

그룹 (2, +)을 다시 한 번 고려해보자. 800(8, 5) = 1이므로, 정리 11,230] 의하여 다음 등식이
성립한다.

<5]g>= {101 [1], 1216, 016 416 1516 1616 16}
따름정리 11.7에 의해서 등식 [5], ㅎ=[시』의 해는 <[51]』>〉의 원소가 [/],인 경우 정확히 한 개 있
다. 예를 들 S71, [kls 2 - 13 3],21   경우 해는 z=(7 ]』이다.

집합 Zo 고려해보자. 800(9, 6) = 3이므로 따름정리 11.8에 의하여 [6],는 9S 법으로 한 곱셈역
이 있음을 알 수 있다. 그 역은 [2[;이다.



===== PAGE 486 =====
© 예제 11.49

0ㅇ00000
14 모듈러 1차 방정식 풀기 475

> 정리 11.24
d=ged(n, m)#} 하고, 다음 등식이 성립하는 정수를 iM} 라고 하자.
d=in+jm                                                         (11.13)

(정리 11,12)o]A] 본바와 같이 그러한 와 je 존재한다) 또한 d| ke 성립한다고 가정하자. 그
러면 다음 식은

200 > 130
다음과 같은 해를 가진다
_| ak
증명 : 등식 11.18에 의해서 다음 SAS 얻을 수 있다.
00000

qt 정수이므로 이 등식의 양변에 [4] 을 곱할 수 있고 다음과 같이 된다,

ml, [55] =띠
증명이 완료되었다
다음 식을 보자
1012 = [4],
gcd(8, 6) = 20] 31, 3=(1)8+(-1)6이고, 34이다. 따라서 바로 위 정리에 의해서 다음 등식은
다음과 같은 해를 얻는다
2= | 4] = 2le= lol
> Bel 11,25



===== PAGE 487 =====
‥00@00 000 0
476     chapter 11 정수론 기반 알고리즘

© 예제 11.50

> 알고리즘 113

x =[j],0] 하나의 해이며, d=ged(n, 70)이라고 가정하자. 그러면 이 식 0개의 다른 해는 다음
과 같다.

1=0, 1, …, 0-1인 경우 [e+e                   (11,14)

증명 : 따름정리 11.6에 따르면 정확히 0개의 해가 존재한다. 그러면 다음 부등식은 당연히
J
In
d
따라서 4] (11,14) 9] de 법으로 하는 류들은 모두 다르다. 이제 각 류가 이 식의 해가 됨을
보이면 증명이 끝난다. 1/],이 071,ㅁ=0,의 해이므로, 다음 등식이 성립한다,

021, = la,

따라서 각 1=0, 1, …, 0ㅡ1에 대해서 다음이 성립한다.

이는 |7+ 꾸| 도 역시 해가 됨을 의미한다.

1=0, 1, …, d-191 경우 0= —<n

n|  =[mjl, + [0], = lk,

예제 11.49에서 다음 식의 해 하나가 [6]』이 BS 보았다.

[602 = [4],
800(8, 6) = 20) 2s 바로 위의 정리에 의해서 다른 해는 다음과 같이 됨을 알 수 있다.
_ = [10], = [2],

따름정리 11,6, 정리 11,24, 정리 11.25 덕분에 모듈러 1차방정식을 푸는 간단한 알고리
즘을 작성할 수 있다. 즉, 따름정리 11.6을 먼저 적용하여 해가 존재하는지를 검사하고,
존재하는 경우 정리 11.94를 사용하여 해를 찾고, 정리 11.25S 사용하여 다른 WSS 4
는다. 알고리즘은 다음과 같다.

모듈러 1차방정식 풀기
문제 : 모듈러 1차방정식의 모든 해 찾기
입력 : 양의 정수 min, 그리고 정수 k

출력 : 식 [71],ㅁ= [시,을 풀 수 있는 경우, 모

해

10



===== PAGE 488 =====
06000000
15 모듈러 거듭제곱 계산   477

void solve_linear (int 2, int m, int 2)

{
index /;
int i,j, d
Euclid (n, m, d, i, j);                      // 알고리즘 11.2 호출
if (d|k)
for (J = 0; / <= d—-1; H+)
cout << |+ eat
}
알고리즘에서 입력의 크기는 YAS 코드화하는데 필요한 비트의 개수로서 다음과
같다.
8ㅎ=|18721+1   ?=|18711+1   u=(lIgk|+1
시간복잡도에는 알고리즘 11.2(유클리드의 알고리즘 2)9] 시간복잡도 O(st)2} for—-l F
프의 시간복잡도가 포함된다. 는 mol nubs 클 수 있기 때문에 이 시간복잡도는 최
악의 경우 입력크기로 환산하여 지수적이다. 그러나 최악의 경우 지수 개수의 값을 계산
하고 보여줘야 하는 문제이므로 이점에 대해서 WMS 수 있는 여지는 없다.
Ge 15 모들러 거듭제곱 계산
원소 [101], ㄷㄷ 2,와 음이 아닌 정수 ko] 대해서 다음을 계산하는 문제를 모듈러 거듭제곱
(modular powers)-& 계산하는 문제라고 한다.
0000
모듈 거듭제곱 계산의 예는 이미 예제 11.43과 11.44에서 보았다. 몇 개 더 살펴보자.
© 예제 11.51 _ 2,,의 경우, 다음과 같이 계산된다.
([7]o9)"! = [1 977 326 7481. = 01.
예제 11.51에서는 72] USS 하여 거듭제곱을 구하였다. 이 방법은 입력크기(대략, 개
수의 로그)로 환산하여 시간복잡도가 분명히 지수적이다. 다음은 더 효율적인 알고리즘
을 설계해보자.

이 알고리즘은 《를 이진수로 표현한다. 그 표현에서 이진 숫자의 순서집합(6806『60
8640을 다음과 같이 표현하자.


===== PAGE 489 =====
478     chapter 11 정수론 기반 알고리즘
{b;, 0;-11 mie) 01, by }
예를 들어, 132] 이진 HAS 101이므로, k= 139] 경우 다음과 같이 표현한다.

> 알고리즘 114

다음은 알고리즘이다. 이 알고리즘이 제곱을 반복하는 방법을 사용한다고들 하는데,
이유는 명백하다.

모듈러 거듭제곱 계산

문제 : 원소 [m],, ㄷㄷ 2, 와 음이 아닌 정수 에 대해서 ([m],,)*S 계산
입력 : 양의 ※ a+ ni} 음이 아닌 정수 mah k
출력 : ([m],)

void compute_power (int n, int m, int k, Z,member& a)

{
index 7;
a = [i],;
186 bj;     ; 01, bo} = k2] 이진 표현에서 숫자의 순서집합
for (2 = /| A S= 0; ~--)
a=a;
if (6, == 1)
a=ax |ml, ;
}
다음 알고리즘 11.4를 적용하는 예제를 살펴보자.
© 예제 11.52 2} 값이 다음과 같다고 하자.

n= 257             m=5                k=45
452] 이진표현이 101101이므로, 다음과 같이 표현할 수 있다.
{by By dg, 01 의 01210. 0, 1, 1, 0, 1}
이 입력이 주어지는 경우 알고리즘 11,42] for-i 루프의 각 반복이 끝난 바로 후 al] 상태는
표 11.8에서 보여준다. [147],,.9] a2] 최종값은 ([5].』,)*의 값이다.

표 11.8에서 &,는 《의 이진 표현에서 상위 7-?-+ 17H 비트에 의해서 결정된 값이다.

mI

’

i= 1, J oe bilo



===== PAGE 490 =====
@00@00000 0
11.5 모듈러 거듭제급 계산    479

@ 표 11.2 n=257, m=5, ^=45일 때 알고리즘 11.4의 +0『-3 루프의 각 반복이 So 바로
후의 0의 상 태 3번째 BS 보면 《의 이진 표현에서 상위 7-1+1개 비트에 의해서 값이 결정
됨을 알 수 있다

i | 5          4          3          2          1          0

b,         1          0          1          1          0

개     1          2          5          i         22         45

a       [51257       [25]1257      [41]257      [181]857      [122]o57      [147]o57

te 1000.01, = 101. =

hy = bY 분명하다. 다음에는 이 변수들을 사용하여 이 알고리즘의 정확성을 증명한다.

> 정리 11,26
알고리즘 11,49] for-i 루프의 각 반복이 끝난 바로 후에 a2] 값은 다음과 같다.

증명 : 귀납법으로 증명한다.
귀납기초 : 극소(0001080) 이진 HAS 한다고 가정한다. 그래서 최상위 비트 oS 항상 1이다.

k

for—i 루프에 진입하기 전에 a=[1], Olt. &가 1이기 때문에 if BABS 첫째 반복에서 참이
, 이는 6=ㅇ× 171, ESS 실행한다는 뜻이다. 따라서 첫째 반복 후 다음이 성립함을 알

고
수 있다.

귀납가정 : 반복문에서 인덱스 값이 가 되는 바로 직후, 0값이 다음과 같다고 가정한다.
0ㅇ= (021 )”

귀납단계 : 반복문에서 인덱스 값이 1-1이 되는 바로 직후, 0값이 다음과 같음을 보이면 된다.

a=({ml,)*"

두 가지 경우가 존재한다. 6, = 0이면, 바로 다음 등식이 명백히 성립한다.


===== PAGE 491 =====
0 00000 0
480  chapter 11 정수론 기반 알고리즘

if 문에서 조건문이 거짓이기 때문에 <=ㅇ만이 a2] 값을 변경한다. 귀납가정에 의해서 ㅇ의
이전 값이 a= (1701, )“이므로, 이 반복 직후 0값은 다음과 같이 된다.
a= ((m],,)* = (lm,
b= 1018, 바로 다음 등식이 명백히 성립한다.
시 ,=2 +

if 문에서 조건문이 참이기 때문에 a=ax [71,도 실행된다. 따라서 이 경우 이 반복 직후 a
값은 다음과 같이 된다.

0ㅇ= (0210) x fm], = (0204.01 = (00 )"그

증명이 완료되었다.

입력을 코드화하는데 필요한 비트의 개수를 6라고 하면, 알고리즘 11.4의 시간복잡도
는 0(8")이라는 사실은 쉽게 알 수 있다.

큰 소수를 찾는 일은 11.7절에서 다룰 RSA 공개키 암호시스템을 성공적으로 구축하기

위해서 필요하다. 큰 소수를 찾는 방법을 설명한 후, 주어진 수가 소수인지 검사하는 알

11.6.1 2 소수 구하기

큰 소수를 구하기 위해서 적당한 크기의 정수를 무작위로 뽑은 다음, 소수를 찾을 때까지
뽑은 정수가 소수인지 검사한다. 큰 소수를 이렇게 찾는 경우 주요 고려사항은 무작위로
은 정수 중에서 소수를 찾을 확률이 얼마나 클지 여부이다.

이제 공부할 소수분포정리는 이 확률을 근사치로 알려준다.

소수분포함수(011076 distribution function) 7(n)-2 7보다 작거나 같은 소수의 개수이
다. AS 들어, 12보다 작거나 같은 소수는 2 3, 5, 7, 1, 이렇게 5개 있으므로 712) = 5
이다. 정리 11.27에서 공부할 소수분포정리(00106 distribution theorem)= 7(7'7)의 근사
He 구할 수 있다.

xo:

=]

> Me] 11.27
다음 등식이 성립한다.

. tn) _
lim  n/lInn I



===== PAGE 492 =====
@0‥00000 0
16 큰 소수 찾기   481

증명 : 증명은 하디28709)와 라이트(\71944)의 1960년 논문에 있다.

바로 위의 정리에 의해서 큰 nj] 대해서 nc} 작거나 같은 소수의 개수의 추정값으
로 7712 7을 사용할 수 있다. 그러므로 균등분포에 따라서 1과 /사이의 정수를 무작위
로 뽑으면 그 수가 소수일 SSS 대략 다음과 같다.

72/ 12 0
n   Inn

* 예제 11.53 균등분포에 따라서 17} n= 10"사이의 AS 무작위로 뽑으면 그 수가 소수일 확률은 대략 다
음과 같다.
1    —
=a 0.027143
그러한 수 2009S 무작위로 뽑는다고 가정해보자. 그들이 모두 소수가 아닐 확률은 대략 다음
과 같다.
(1—0.027143)°° = 0.004
* 예제 11.54 균등분포에 따라서 1과 7 = 10사이의 정수를 무작위로 뽑으면 그 수가 소수일 확률은 대략 다
음과 같다.
In10™ 0.0043429
그러한 수 200개를 무작위로 뽑는다고 가정해보자. 그들이 모두 소수가 아닐 확률은 대략 다음
과 같다.
(1-0.0043429) = 0.04
이 절의 시작 부분에서 언급했던 것처럼 큰 소수를 찾기 위해서 적당한 범위에서 수들
을 무작위로 뽑아야 하고, 그 수들 중에서 소      수 ohh 찾을 때까지 각 수가 소수인지
검사해야 한다. 바로 위의 예제들을 봐서는 소수를 찾는 일이 (범위 내에 있는 수의 개수
에 비해서) 그리 오래 걸리지는 않을 것이 확실하다. 다음으로 주어진 수가 소수인지를
검사하는 방법을 알아보자.
< 11.6.2 주어진 수가 소수인지를 검사하기

9.2절의 서두에서 어떤 a4 소수인지 결정하는 간단한 알고리즘을 공부했다. 그러나 불
행하게도 그 알고리즘은 최악 시간복잡도가 지수시간이다. 그래서 큰 수를 ae 데
는 사용할 수 없다. 그 비흐율적인 알     고리즘은 합성수에 대해서는 그 수의 인수를 찾아주
며, 따라서 그 알고리즘은 수를 인수분해하는데 (반복해서) 사용할 수 a


===== PAGE 493 =====
482     chapter 11 정수론 기반 알고리즘
최근까지도 소수검사문제를 푸는 다차시간 알고리즘을 아무도 발견하지 못했고, 많은
학자들이 이 문제가 ^/#-완전일 것이라고 생각해왔다. 소수검사문제를 푸는데 전형적
으로 사용되었던 효율적인 알고리즘은 래빈ㅁ8610)이 1980년에 발표한 밀러-래빈의 무
작위적 A-PAALMiller—Rabin Randomized Prmality '【680라고 하는 나 알고리즘
이었다. 이 알고리즘은 소수에 대해서는 항상 소수라고 판정한다. 그러나 아주 드물게
QUE 소수라고 판정하는 정우가 있다. 이 BEL 너무 SBA 발생하므로 이 dae}
즘은 본질적으로 정확   하다고 Ce 큰 문제가 없는 걸로 여긴다. 밀러-래빈 알고리즘
은 합성수로 판정한 경우 그 수의 인수를 찾지 않으므로 인수분해에 사용할 수는 없다.
마침내 2009년에 에즈 그의 동료들이 소수검사문제를 푸는 다차시간
알고리즘을 만들어 내는데 성공했다. 그 알고리즘을 살펴보자.
다차시간 알고리즘
먼저 정수론의 연구결과가 좀 더 필요하다
정의
/(2)와 0(2)를 계수가 정수인 다항식이라고 하자. Zt 계수들이 7을 법으로 한 합동이면
/(2)와 0(2)는 7을 법으로 한 합동이라고 하며, 다음과 같이 쓴다
f(x) = 0(2) mod n
© 예제 11,55                        6=2 mod 4
9=1 mod 4
1=—3' mod: 4
이므로
(62?+ㅜ92+1) = (22?+2-3) mod 4
© 예제 11.56                                8n #1 mod 4
이므로
(62?+82+1)7 = (22?+2-3) 1000 4
없는 항의 계수는 0으로 가정한다.
© 예제 11.57                                10=0 mod 5
7=2 mod 5
21=6 000 5

이므로



===== PAGE 494 =====
© 예제 11.58

@
1.6 큰 소수 찾기     483

(1023 +727 +21) = (22?+ 6) mod 5

120 mod 5
이므로

x #2 mod 5

이 마지막 예제는 재미있는 점이 있다. 정리 11.220} 따르면 모든 정수 x ol] 대해서 다
So] 성립한다.

x =x mod 5

그러나 자애 “와 ct 5S YOR 한 합동이 아니다.

소수인지 결정하는 쉬운 방법을 유도해
보조정리부터: ee

A

rir

이
ㅁㅁ
tu
iT
el
HE
N
so
[소

| < 보조정리 11,2
no] 소수이면, 모든 정수 mol] 대해서

(c—m)" =(a"—m) mod n

따라서
(2-772)"”-(2"-ㅡ7172)  이 J(-m   jr-t g? — (4 —m)

a

0
ㅣ 7   ae       (11,15)

그런데 7은 소수이므로, 1<i<n—12l io] 대해서 다음은 분명히 성립한다.
("| =0 modn
i

그러므로 각 io] 대해서 등식 01.15)에서 은 /을 법으로 하여 0과 합동이다. 따라서 다음이
성립함을 보이기만 하면 된다.
(—m)"+m = 0 mod n
만약 = 3이면,
[((—m)?+m] =m(m+1) mod 2
=0 mod 2


===== PAGE 495 =====
@000000
484     chapter 11 정수론 기반 알고리즘

© 예제 11.59

© 예제 11,60

위의 두 번째 등식은 m 또는 ㅠ+1 중 하나는 짝수라는 사실에 의해서 성립한다. 만약 > 2

이면, 7은 홀수이고, 따라서
[((—m)?+m] =(—m"+m) 2ㅁ007

m(—m"~!+1) mod 2

lll

lll

이제 mo] 7의 곱이라면, m =0 mod no|t}, 그렇지 않으면 정리 11,220] 의해서 (—m"™!
+1) =0 ㅁ007이다. 증명이 완료되었다.

> 정리 11.28

mit 을 서로소(8618076 prime)e}3! 하자. 그러면 no] 소수가 되는 필요충분조건은 다음과
(2-72)"=(2"-ㅡ7172) mod n                                 (11, 16)

다른 방향의 SIS 하기 위해 nB 합성수라고 가정하자. oH "의 인수라고 하고, *를 에서
02) 차수(0000라고 하자. @ + | ":|가 아님을 보이는 작업은 연습문제로 남겨둔다. no] 에
서로소이기 때문에 명백히 는 (-77)"-*에 서로소이다. 그러므로 (")(—m) ns 인수로 @
를 포함하고 있지 않고, 이는 mB 법으로 하여 0과 BHO] 아니라는 뜻이다. 그러나 등식 1.15
에서 계수 중 하나이다. 증명이 완료되었다.

9와 2는 서로소이다. 정리 11.28이 암시해주듯이,

1=1 mod 2
—18=0 mod 2
81=—9 mod 2

이므로

(2-9)? =2?—-182+81 = (z?—9) mod 2

9와 4는 서로소이고, 4는 소수가 아니다. 정리 11,280} 의해서
(7-9)%\ㅋ=(2*-9) mod 4
증명은 연습문제로 남겨둔다.

정리 11.88을 가지고 어떤 수가 소수인지 결정하는 간단한 알고리즘을 만들 수
즉, 정수 nj) 대해서 no] 서로소인 을 선택하고, 합동 01.10)이 성립           정
그러나 합동 01.16)의 좌변에 있는 + 1개의 계수를 평가해야 하기 때



===== PAGE 496 =====
© 예제 11.61

© 예제 11.62

* 예제 11.63

은 시간복잡도가 지수시간이다. 시간복잡도를 향상시키기 위하여 재주를 부린다. 그러기

위해서 정의가 몇 개 더 필요하다.

정수의 경우와 마찬가지로 mod 함수(0ㅁ200 function) = 하나의 다항식을 다른 다항식으
로 나눈 나머지를 내준다. 즉, 다음 식은 fe) ge) = 나눌 때 나머지가 되는 다항식

이다.
f(x) mod 0(2)

다음 예제가 이를 설명해 준다.

8    2
122“+ 232 ETD Fg a4: 2279

dx? +2                   dn? +2

이므로
(122“"+232?+72+9) mod (42?+2) = 22 +9

f(x), g(x), h(x)S 계수가 정수인 다항식이라고 하자.
f(a) mod h(x)] = [0 (2) mod h(x)|mod n

이면
7(2)= g(x) mod [h(z), n]
로 쓴다.
(7-10)" mod (2?-1) = 3012 —1030
(2-10) mod (2?-1) =x—10
이고,
(3012 —1030) = (2-10) mod 3
(x—10)° = (2-10) mod (2?-1, 3)
(x—14)’ mod (2”-1) = —11 29018827 +52610 7132 — 104069 042
(27-14) mod (23-1) =2—-14
이고,
(-112901882?+526107132-104069042) = (2-14) mod7
이므로,

(7-14)'=(2'-14) mod (20-1ㄴ 7)



===== PAGE 497 =====
486     chapter 1 정수론 기반 알고리즘
© 예제 11.64         (7-20)' mod (x*—1) = 56000012? — 67 200 140x? + 448 008 4002 — 1280 280000

© 예제 11,65

(2’—20) mod (x*—1) = 2?—20

— 1280280000 #—20 mod 7

(x—20)" # (27-20) mod (x*—1, >)

위의 예제들이 다음 정리가 사실임을 보여준다.

> 정리 11.29
과 ro] 소수라고 하자. 그러면 모든 정수 mol] 대해서

(2—m)” = (c"—m) mod (2"—1, n)                       (11,17)
명 : 보조정리 11.28 이용해서 증명하며, 연습문제로 남겨둔다.

oly

no] 소수라는 사실의 필요충분조건은 WS 11,170] 만족한다는 것이라고 위의 정리가
밝혔다면 합동 (11.17)을 이용하여 바로 소수검사 알고리즘을 향상시킬 수 있을 것이다.
즉, (2"-11) mod (2" -1)의 계산은 아주 간단하고, 크누스(<ㅁ4100)는 1998년에 빠른
Fz] ol(Fourier) FAS 이용하여 시간복잡도가 Olr(Ign)?]el (ㅠ-11)” mod (2" -1)
을 계산하는 알고리즘을 만들었다. 따라서 정리 11.29가 필요충분하고 ro] 작은 수라면,
합동 (11.16)의 AVS 훨씬 작은 계수가 포함된 BSS] 결정으로 꽤 빨리 대치할 수 있었

을 것이다. 다음 예제가 이를 보여준다.

110] 소수인지 알아보고 싶다고 하자. 정리 11.29가 필요충분하다고 가정하고, m = 49+ =3을
선택하자. 그러면 다음 두 등식이 성립한다.
(2—4)" mod (20-1) = —12536 1272” + 62120522 +6 146 928

(at!—4) mod (2? -1) =2?-4

이제 다음이 합동인지 검사하는 대신
(—12536 1272? +6 2120522 +6 146928) = (2?-4) mod 11

다음이 합동인지 검사한다.

<(2-4)브 = (cl! —4) mod 11

결국 127) 합동을 검사하는 문제를 37] 검사하는 문제로 축소하였다.

위 절차의 문제점으로 정리 L295 비록 no 서로소인 ms 선택하더라도 “필요충분”



===== PAGE 498 =====
하지 않다는 것이다. 즉, 일부 합성수는 mo] no 서로소인 어떤 my} *의 값에 대해서
함동 01.10'을만족할 것이다. 따라서 단순히 특정 gol 대해서 함동이 성립하는지 검사
한다면, 검사를 통과하는 합성수가 있을 수 있다. 적절한 >을 선택하고, 여러 다른 mz
에 대해서 검사하여 이 문제를 피해갈 수 있다. 이렇게 하면 소수로 판정받는 합성수는
없고, 알고리즘도 여전히 다차시간이다. 먼저 이 알고리즘을 살펴본 후, 그런 시간복잡도

를 어떻게 얻었는지 알아보자. 일단 용어를 몇 개 더 정의한다.

룸 원소 ㅇ의 차수, 070(0), a! = 가 성립하는 ALS 양정수임을 상기하자(여기서

6는 항등원이다). 그러면 그룹 (2, ×,)에 HAA ord((n],)-& (141.)" =
는 최소의 양정수이다. 즉, 다음 합동이 성립하는 최소의 양정수가 된다.
n'=1 mod r

이를 7

tho

> 일고리즘 115     다차시간 A=SHAKPolynomial Determine Prime)

2

: 정수가 수수인지 결정

lrg

-n>12 정수

력 : no] 정수이면 참, 합성수이면 거짓

mt ㅁ으 ro

bool prime (int 22)

{

int g, r, m; bool switch;

if (2 == k’ for integers k, j > 1)
return false;
r= 2; switch = false;
while (r < n &&! switch) {
if (gced(n, r) #1)
return false;
if (r is prime) {
0 = the largest prime factor of r—1

if (q>=4Vrlgn &&n* #1 mod 2)
switch = true;

}
r=r+4+l;
}
if (switch) {
20. He

while (m <= 2y/r lg n) {
if ( (x—m)” = (x"—m) mod (x~—1, 2) )
return false;

[1],°] 성립하

법으로 한 7 의 차수(680@ of n modulo 7)라 하고, ord, (71)으로 표시


===== PAGE 499 =====
@000000 0
488   chapter 11 정수론 기반 알고리즘

m= m+1;
}
}

return true ;

}

알고리즘이 맞는지 증명하자. 먼저 소수에 대해서는 항상 소수라고 답해 주는지 증명
하자.
> 정리 11.30

소수가 알고리즘 11.5에 입력으로 주어지면, 그 알고리즘은 참을 내준다.
증명 : no] 소수이면 7<7인 모든 ro] 대해서 다음 등식이 성립한다.

gced(n, 7) =1

이는 첫째 while 루프에서는 AAS 내줄 수 BSS 의미한다. 정리 11,290] 의하면 nap rs
소수이므로 둘째 11186 루프에서도 AAS 내줄 수 없다. 따라서 알고리즘은 마지막 명령과
함께 종료하며 명령은 참을 내준다고 결론지을 수 있다.

합성수에 대해서는 항상 합성수라고 답해 주는지 증명하기가 훨씬 더 어렵다. 그렇
지만 해보자. 먼저 보조정리 11,29} 정리 11.29를 일반화한 다음 두개의 보조정리가 필요

하다.
| 보조정리 11,3
g(a) 정수계수를 가진 다항식이고 은 소수라고 가정하다. 그러면 다음 합동이 성립한다.

[g(x)|" = g(x") mod n
증명 : 다항식은 다음이라고 하면
g(x) =a,t+ar+ … +a,24
다음 등식이 성립한다.
g(z") =a, t+a,2"+ -- hee … +a,"                 (11,18)

더구나, [0(0)]”에서 7'의 계수는 다음과 같다.

;     !
=                     20     22    7:
b=    >     aid. gi} —           (11,19)
tot ee ayn
i, +2, + + +diy =i



===== PAGE 500 =====
@ㅎ6@060000 0
1.6 큰 소수 찾기   489

이올
는 a lth, 더구나 등식 01.19에서 볼 수 있듯이 《&에 포함되어 있는 모든 항에서 모든 joy
대해서 ,=7이다. 그러나 그러면 각 항은 7으로 나누어지고 이는 71&가 되며, 따라서
% =0 mod 7이 성립한다. 경우 1 증명이 완료되었다.
경우 3 : 0 <j = 0를 만족하는 jo] 대해서 i= jn 경우. 등식 01.18에서 볼 수 있듯이 0(ㅠ")
에서 의 계수는 (이다. 더구나 , =7을 취하면 ji, = ㅠ=1가 된다. 그러므로 등식 (119) 4
Al 볼 수 있듯이 0.9] 항 중 하나는 다음과 같다.

경우 1 : 임의의 7에 HAHA i = 77인 경우. 등식 01.18)에서 볼 수 있듯이 g(x") WA 7'의 계수
2

—_—
a;    a;

&의 다른 항들에 대해서는 명백히 모든 *에 대해서 i, = n7} 성립하는데, 이는 그 항이 7으로
나누어진다는 뜻이고, 따라서 그 BL 7을 법으로 하여 0과 합동이다. 정리 11.29에 의하면
다음 합동이 성립하므로

. . 워런
a; = 2ㅁ00 n

이 경우도 증명이 완료되었다. 따라서 전체 증명이 완료되었다.

| 보조정리 11,4

g(x) 정수계수를 가진 다항식이고 nz} 7은 소수라고 가정하다. 그러면 다음 합동이 성립
한다.

1 0(2)]" = g(x") mod (2"—1, n)

증명 : 바로 위 보조정리를 이용하여 증명할 수 있으며, 연습문제로 PAE.

다음 보조정리들도 필요하다.

*보조정리 11.5

과 《가 소수이고, r—10] 《로 나누어떨어지고, < > 41 lg no}, q lord,(n) 9] 필요충분조
건은 다음과 같다.

eit
72 1 #1modr

증명 : t=ord,(n) OB 놓으면, ro] 소수라는 사실과 정리 11.17과 정리 11.19 때문에 r-1=tk
인 정수 *가 존재한다. 7-1이 로 나누어떨어지고, 가 소수이므로, 따름정리 11,20] 의하면
qit 또는 01^&가 성립한다. 이제 필요충분조건을 증명해보자.

90

필요조건을 먼저 증명해보자. 27  =11ㅠ00 이라 가정하고, 모순을 유도하기 위해 q 1 tz}


===== PAGE 501 =====
490

chapter 11 정수론 기반 알고리즘

고 하자. 011 또는 01*이므로, 01^이 성립한다. 따라서 *-1=#이므로, 7-1=7140인 정수

가 EASA. 이는 (- 1)/0-7/가 성립함을 RTH, 그러나 nt =7를 얻을 수 있고, 따
라서 다음 합동이 성립한다.

7) : =1modr
이는 모순이므로 01*가 성립한다.
충분조건을 이제 증명해보자. ?는 로 나누어진다고 가정하자. 0 > 477 187/이므로 다음 부
등식이 성립한다.

Ed ee eg
;    2

그런데 ?= 07@.(7))이므로 다음이 성립한다.

2:

4 #1modr

n

| *보조정리 11.6
no] 합성수이고, ge 소수이고, glord,(n)}A, 다음이 만족하는 7의 소인수(0ㅁ106 factor)
가 존재한다.
01002)

SY : 21, Py) Pes 7의 수인수라고 하자. 다음이 성립하는지 보여주는 작업은 연습문제로

ord, (n) |lem(ord,(p,), 70.(2.), +++, ord,.(p,))

역서 lem 최소공배수(16886 common multiple)°|t}, glord,(n)°|al ge 소수이므로, 정리
11.7에 의하여 010@.(2,)이 성립하는 p,7} 존재한다. SY] 완료되었다.

앞으로 살펴 볼 정리는 다음 보조정리에 깊게 의존한다. 이 보조정리를 증명하려면 대

SHalgebra)o] 필요한데 이는 이 교재의 범위를 벗어나게 된다. 추상대수학(808\ㅁ8
8186678)을 잘 아는 독자를 위해서 이 절 끝부분에서 이 보조정리를 증명한 결과를 보여
주겠다.

| <보조정리 11.7
알고리즘 11.5에서 switch} 참이어서 두 번째 while 루프에서 빠져나왔다고 가정하자. pe



===== PAGE 502 =====
000000 0
116 큰 소수 B|   491

보조정리 11.6에서와 마찬가지이고, 1=|2 Vr 18 ”1이라고 하자. 그러면 다음 다항식이 존재
한다.
g(x) =(«—1)"(w@—2)" + (2-)7)"
이 다항식은 다음과 같은 성질을 가진다.
={m | g(x)" =g(a™) mod (2"—1, p)}
이면, 다음이 성립한다.
1. Jaq 곱셈에 닫혀 있다.
2. 76. 4 & 24)에 대해서
m=k mod r
이면,
m=k mod a
가 되는 4>7”"/ 20) 정수 a7} 존재한다.

증명 : 이 절 끝부분을 보시오.

이제 주된 결과를 증명할 수 있다.

> 정리 11.31

알고리즘 11.5의 입력으로 임의의 합성수가 주어지면, 그 알고리즘은 거짓을 넘겨준다.

증명 : 그 수가 합성수이고, 그 안에 QE return 문장 때문에 Al Aw while 루프에서 mate
는 경우, ALS 넘겨주게 되므로 증명작업은 끝이다. 7=7-ㅡ1이어서 A HA while 루.

에서 빠져나오는 경우 7은 반드시 소수이다. 따라서 합성수가 입력되고 30110가 참이므로

Al 번째 while 루프에서 빠져나왔다고 가정한다. 그러면 보조정리 11.5에 의해서 ord ,(2)은

0로 나누어진다. 이 알고리즘이 참을 넘겨준다고 하고 모순을 유도해보자. 두 HAlwhile 루

프 때문에 1 = <1=2vVr 18끼인 mol] 대해서 다음 합동이 성립하고

(x—m)" = (a"—m) mod (2"-1, n)
이는 다음 합동이 성립함을 의미한다.
(2 7012 = (20720) mod (a - 1. 2)                      (11,20)
여기서 pe 보조정리 11.0에서와 같다. 그러므로 보조정리 11,79] YE g(x) 2] A 항 (ㅎㅠ-172)
은 개별적으로 합동 11.208 만족한다. 이는 다음 합동이 성립함을 의미한다.
[g(x)]" = g(x") mod (2"-1, 2)

따라서 J) 3 보조정리 11.7에서와 같다고 하고, 7ㄷ./,,,;이라고 하자. 더구나 보조정리 11,4
때문에 2, ,;가 되고, 사소하게 1, ,;가 된다.


===== PAGE 503 =====
492

chapter 11 정수론 기반 알고리즘

이제 다음 집합을 보자.
E={0 <i, j<| /ㅠ|을 만족하는 2}

보조정리 LTS 1번 부분에 의하여 LS /,,;가 성립한다. 더구나, 다음이 성립한다.

[£l=(14+L Vr ])3 >
그러므로 피전홀 MA(pigeonhole 0ㅁㅁ0018)에 의해서 &에는 nip’ n'p*o} 두개의 원소가 존
재하는데, 여기서 다음 합동이 성립하며 ;=/ 또는 7= 이다.

n' p = 02" mod r

따라서 보조정리 11,79] 2H 부분에 의하여 다음 합동이 성립한다.

27 = 72" mod a                                      (11,21)
여기서 0는 그 보조정리에서와 같다. 217이고, 7은 합성수이고, 《 j<|VrlolBH, 다음이
성립한다.

0         vr    avr
np < nv( 2}   ="

비슷하게, ^, k<|Vrloles 다음 부등식이 성립한다.

n2vr
gvr

n'pk <

그러나 6>7”/?이므로 합동 11.91에 의해서 다음 등식이 성립한다.

nip! = ni p*
217이고, 1 = 또는 7 = 《이므로 바로 위 등식에 의하여 6 > 1인 정수 58에 대하여 다음이
성립한다.

102

그러나 이 알고리즘의 첫째 단계에서 no] ＊ = 221 /의 형태를 이루는지 검사하였다. 그러므
로 *=1이고, 7은 소수이다. 이는 모순이고, 따라서 증명이 완료되었다.

알고리즘의 시간복잡도
이제 알고리즘 11,59] 시간복잡도에 대해서 공부해보자. 먼저 보조정리와 정리 몇 개를
알아보자.

| 보조정리 11.8
Ame 7』의 가장 큰 소인수라고 하자. 그러면 n> 에 대해서 다음 부등식이 성립하는



===== PAGE 504 =====
소수이고 7 =7ㅠ이며, 《_, > nS 만족하는 2 ||= 어근

clr

i
의 상수 <와 정수 No] 존재한다.
명 : 1996년에 발표된 베이커(88660와 하멘0187080/의 논문에 증명이 있다.

°
e
a
ㅇ

| <보조정리 11.9
은 소수의 개수하고 하자, 그러면 m > 1에 대해서 다음 부등식이

7('1)을 보다 작거나 같은

성립한다.
=   << a(m) <
lgm

증명 : 1997년에 발표된 아포스톨(^4008101)의 논문에 증명이 있다.

*보조정리 11.10
양정수 7 과 7에 대해서 다음 곱은

(n—1)(n?—-1) … (2 -1)
최대로 mle nh] 소인수를 가진다.
증명 : 각 항은 최대로 187개의 소인수를 가지고, 항의 개수는 개이다.

> Bel 11.32
> 인 모든 nol] 대해서 다음 구간 안에 소수 ro] 존재하도록 하는

(ce, (ig 7209 (Ug 7209)

다음 두

clr

CT} 6,와 정수 NO] 존재한다. 그런데 여기서 7-1의 가장 큰 소인수 0

ㅇ
조건을 만족한다.
rol
q>= 4r'? 1g n, 72 1 #1 modr

임의의 양정수라고 하자. 보조정리 11.8에 의해서 (18 n)°> NV

증명 : 잠시 동안 ㅇ,과 <,는
에 대해서 다음 식이 만족하는 YO] 상수 <와 정수 NO] 존재한다.
5      ay           6087)"
|고 2 주 087)『이며, <, > [8087)이^ "을 만족하는 r}| 도개
(11,22)

부등식 011.29)로 다음 부등식이 성립함을 보이는 작업은 연습문제로 남겨둔다.


===== PAGE 505 =====
494

chapter 11 정수론 기반 알고리

OW

보조정리 11,94] m =c, (Ig n)°O]#}a 한다면, 식을 조금 조작하여 (18 7)"보다 작거나 같
은 소수의 개수가 다음보다 크지는 않다는 사실을 얻는다.

8c, (lg 72)"

eric                                             (11,23)
부등식 01.89)와 (11,23 합하여 다음 부등식을 만족하는
[40870 e (Ig n)°]                                (11,24)
다음 구간에서
1 > [608 720이그                             (11,25)
소수의 개수 p7} 다음 보다 크거나 같다는 사실을 구한다.
| 000 806. | 087)"
7 6 )18087)

이러한 소수를 특별소수(60601 ㅁㅁ2768)라고 한다. <,과 6,가 임의의 양정수임을 상기하자. 그
리고 이제 6, = PS 선택하자. 그러면 BE 특별소수 po] 대해서 다음을 얻는다.

2/3 _ p26

= ple (lg n)>|
> p'?[45(Ig n)§]/°

> pi?4 lg n

Gi > P
1/6

(11, 26)

부등식 (11,24) 9} 01.98/에 의하여 첫 번째 부등식이 성립하고, 부등식 01.95/에 의하여 두 번
부등식이 성립한다.

이제 4 =| 은 --운 |> 인 를 선택해보자. 그러면 n> 에 대해서 특별소수의 개수는
다음보다 크거나 같다.
(Ig 7)"
Cy ete                                      (11,27)
이제 *=6ㅇ,(187)"이라고 하면, 다음이 성립한다.
6
zr 18 n= [eg (lg 2)이2 187 =" (lg 72)" < (jee               (11, 28)

보조정리 11,10] 의하여 다음 곱은 최대로 leg 7개의 소인수를 가진다.

11=(2-1)02-1) … (60811)



===== PAGE 506 =====
따라서 부등식 (1.97)과 (11.28)에 의해서 [TS 나누는 특별소수 ro] 최소한 1개 존재한다.

이제 7이 이 정리의 조건들을 만족시킨다는 사실을 보이자. 부등식 (11.24)와 011.25)에 의해
서 7은 처음 두 조건은 명백히 만족시킨다. 따라서 (=《…,이라 하면, 다음을 증명하기만 하면
된다.

1.
72 1 # 1modr

그러기 위해서 다음 합동을 가정해보자.

(mee!

n‘’ =1modr
그러면 14 -11이 성립한다, 따라서 [Le re 나누어떨어지지 gone, 모순을 유도하
기 위해서 다음이 ABB 보이면 된다.
글
qd
부등식 (11,250 의해서 (> [eo (1g 0) 가 성립하므로, 다음 부등식이 성립함을 보이기만
하면 된다.

< 128] = | ch 08703]

r-1 < | 88087)" ] Le (gn)? |
< & (Ig 700

그러나 부등식 (11,24) 의해서 마지막 부등식은 성립한다. 이는 모순이므로 증명이 완료되
었다.

『 최악 시간복잡도(다차시간 소수검사)

기본동작 : 하나의 비트 조작
입력크기 : /,을 코드화하는데 드는 비트의 개수 $로, 다음과 같이 주어진다.

8ㅎ=|1871+1

을 의 형태로 표현 가능한지 결정하기 위해서 검사하는 뿌리마디의 개수는 (/(6)이다.
nil? 기 vee, oe. 검사할 필요가 있다. 여기서 m= Llg n! 이다. 2.6절에서
Bot 무작정 해보는 기술을 사용하면 각 뿌리마디를 검사하는 시간복잡도는 (($”)이
다. 그러므로 총 시간복잡도는

430 =

이

O(ss?) = O(s*)

정리 11,326] 따르면 첫 번째 while FXG 통과하는 패스의 반복 횟수는 0(6”)이다. 각
패스마다 얼마만큼의 일을 하는지 살펴보자. 7<7이므로 알고리즘 11.1을 사용하면


===== PAGE 507 =====
496

chapter 11 정수론 기반 알고ㅁ

매

60001, ne 계산하는 ANSE 0(")이다, 9.2419] BRAY 보여준 ro] 24
지를 결정하고 r— 19] 가장 큰 소인수를 찾는 2

Sols 바118 루프을 동과하는 aA] 반복 glee 최대한 이고 고 269014 공부한
무작정 기술을 사용하면 각 패스에서 나머지를 계산하는 시간복잡도가 0(6”)이다. 따라
서 총 시간복잡도는 0(“”6”)이며, 이는 정리 11,3264) 따라서 그 시간복잡도가 0(6*8")
= 60(#")임을 의미한다. 2,689] 기술을 다시 이용하면 7을 증가하고 첫 번째 while 루프
에서 빠져나가는 조건을 검사하는 시간복잡도는 0(6”)이다. 따라서 첫 번째 while 루프
의 총 시간복잡도는

fi
>

au           알고

Oss’) = 0(6)
< 008 7)“이므로 바로 알아낸 것보다 좀 더 자세한 한계 값을 구할 수 있다. 그러나 곧
보겠지만 두 번째 7116 루프가 전체 한계 값을 좌우하므로 상관없다.

두 번째 11116 루프를 통과하는 패스의 반복 횟수는 (0(7"'”8)이다. 이는 정리 11.82에
따라서 그 패스의 반복 횟수가 O(s*s) = O(s*) YS 의미한다. 정리 11,292] 바로 뒤에
언급했듯이 이 루프에서 합동을 결정하는 시간복잡도는 빠른 푸리에 곱셈을 사용하면
@0(78”)이고, 이는 다시 정리 11,320] 따라서 그 시간복잡도가 O(s*s*) = O(s'7) YS 의
미한다. 따라서 두 번째 while 루프의 총 시간복잡도는

O(s°s*) = O(s!”)
따라서 다음과 같이 결론짓는다.
W(s)= 2(61?)

2002년에 O}-12}2}(Agrawal)} 그의 동료들은 알고리즘 1.5이 실제 상황에서 방금
한 한계 값보다 훨씬 더 빠를 수 있다고 그들의 논문에서 언급하고 있다. 사실, 이 추론이
맞다 가정하고 이 알고리즘의 발견적인 시간복잡도가 (0($")임을 그들이 증명하였다.

보조정리 11.7의 증명하는데 ASE 결과

보조정리 11.7을 증명하는 보조정리들을 살펴보자. 이 SS 이해하기 위해서 추상대수학
의 사전 지식이 필요하다. 먼저 BS 설명한다. 환(0208) 에 대해서 그에 대응하는
다항식환(0017400181 ring) 2?[21로 표시한다. 예를 들어, Zo] 대응하는 다항식환은
Z, [지로 표시한다. 환 과 그 #에서의 아이디얼10681) Loy] 대해서 17+1 | 1ㅎ2}
의 형채로 구성된 잉여환(6800 ring) R/LS 표시된다. 또한, re] ROA LO] 7의 배
수들로 구성된 아이디얼이면 R/LS R/S 표시한다. AS 들어, 2, 은 277으로 표시할
수 있다. WS 또 하나 보면, 다항식환 R(x) ot 다항식 /(2)6ㄷ(2 )에 대해서 7(2)의 BH



===== PAGE 508 =====
수로 구성된 아이디얼에 의해서 결정되는 잉여환은 #(=)//(2)로 표시된다. 주어진 소
수 에 대해서 우리의 관심사는 환 ZAKS 필드8610), 다항식환 2,|2], 잉여환
2,121//(2)이다.

다음 제시하는 보조정리는 대부분 증명을 생략한다. 이 보조정리들은 일반적으로 많이
쓰이는 대수적 AAS 통하여 순서대로 증명할 수 있는데, Of eps] 2002년 논문에서
ROW 수 있다.

| *보조정리 11.11
po} r& 2 7인 소수라고 하자.
1. ^(2)가 2-19] 인수이고 m=k mod rola, 다음 합동이 성립한다.
2” = mod A(z)

2. 070,(2)을 7을 법으로 하는 #의 차수라고 한다면, (7" -1)/(ㅎ-1)은 ZS 나누어지지 않
LAY ord, (p) 2] 차수를 가진 다항식으로 인수분해 된다.

알고리즘 11.5에서 switch7} 참이고, pH 보조정리 11.6과 같고 i= ㅣ 27187 ㅣ 으
로 놓았기 때문에 두 번째 while FZS 빠져나왔다고 가정하자. 위의 보조정리 2번에
의하여 x” -1의 인수이고, 로 나누어지지 GEO AA] ord, (p) 2] 차수를 가진 다항식

(2 )가 존재한다. 다음 보조정리들은 모두 switch7} 참이고, pH 보조정리 11.6과 같고,
/^(2)는 방금 언급한 다항식이고, T= 27 18 7! 으로 놓았기 때문에 두 번째 while
루프를 빠져나왔다고 가정한다.

| 보조정리 11,12
2,.121/^(2)에서 GS 1개의 다음 이항에 의해서 생성된 그룹이라고 하자.

IN

c= 1<m<12 에 대하여 &, > 0을 만족하는      (2—m)|

lemstl

IA

그러면 GS 순환적이며 다음 부등식이 성립한다.

je > 모으

여기서 IGE Gola] 원소의 개수이다.



===== PAGE 509 =====
0000000
498     chapter 11 정수론 기반 알고리즘

| *보조정리 11,13
Ge 위 보조정리에서의 그룹, 0(2)는 G2] 생성기, ,는 4,121/^(2)에서 0(2)의 차수라고 하

자. 그러면 다음 부등식이 성립한다.

즈며 ㆍ

증명 : ;:= [217 1871! 이고 q>4vr leg 이므로, 0=232이다. 보조정리 11,60] 의하면
qlord,(p)7} 성립한다고 하였으므로, 이는 00@.(7) = 210] 성립함을 의미한다. 위의 보조정리
에 따르면 다음을 얻는다.

070 ,.(p)
1

nvr

l      1

IG|>

증명은 이제 g(x) 7b G2 생성자라는 사실에 의해서 완료된다.

| 보조정리 11,14
0(4)가 위 보조정리에서와 같다고 놓자. 그러면 다음 집합은 곱셈에 닫혀 있다.

Iyiz) = g(x)” = 00") ㅁ00(77-1, 2) 를 만족하는 m}

| 보조정리 11.15
(2), 는 모두 위의 보조정리에서와 같다고 놓자. 그러면 BE m, k SoH 대해서

다음 합동이 성립하면,
m=k mod r

다음 합동이 성립한다.

m=k mod a,

rlo
wl
au

0,로 놓는 경우 위의 보조정리들을 가지고 보조정리 17S 증명하는 것

a= a,       =

@ 11.7 RSA 공개키 암호체계
철수가 영희에게 인터넷으로 연애 비밀 메시지를 보내려 하는 일에 관하여 앞에서 이야
른 친구

기 한바 있다. 메시지를 영희만 알 수 있는 비밀코드로 바꾸어 보낼 수 있다면, 다
가 그 메시지를 가로채더라도 걱정할 필요가 없을 것임도 언급한 바 있다. 공개키 암호체



===== PAGE 510 =====
© 예제 11.66

@00@000000
11.7 RSA 공개키 암호체계    499

계를 이용하면 철수가 바라는 대로 할 수 있게 해준다. 공개키 암호체계를 먼저 이해한
후, RSA 공개키 암호체계를 공부해보자.

11.7.1 공개키 암호 체계
공개키 암호체계(000110-6》” 70108781609)는 허용 가능한 메시지, 참여자의 집합(각 참
여자는 모두 공개키(6004040 key) 2} 비밀키(66066 key)S 가지고 있음), 참여자 간에 메시
지를 주고받을 수 있는 네트워크로 구성한다. 주어진 길이 이하의 문자열은 모두 메시지
로 허용가능하다. 다음과 같이 놓는다면
44 =허용 가능한 메시지의 집합

각 참여자 의 공개키 2668,와 비밀키 skey,= MAA MOS 가는 서로 역인 함수
pub, 2} sec, 2 각각 정해진다. 즉, 각 be Mo] 대해서

b= pub, (sec, (b))

b=sec, (pub, (b))
참여자의 공개키는 참여자 모두에게 알려주지만, 의 비밀키는 2 만이 알고 있다. 예를
들면 철수가 영희에게 비밀 메시지 를 보내고 싶으면, 철수와 영희는 다음 작업을 한다.

1. 철수는 영희의 공개키 pkeygak c=pubgal(b)S 계산한다. 이 메시지 cE 암호
문(0006066800이라고 하며, 읽을 수 없다.

2, 철수는 영희에게 암호문 GS 보낸탁.

3, 영희는 자신의 비밀키 skeygnS b =secga(c)S 계산한다.

철수가 영희에게 "사랑해'라는 비밀 메시지를 보내고 싶어 한다고 가정하자. 그 절차는 다음과
같다.
1, ASE 다음을 계산한다.
pubga(“AR SH”)
그 결과가 “"@!\%*(!”라고 하자.
3. 철수는 이 메시지를 영희에게 보낸다. 철수 이외 다른 친구들은 “@!#\%*(!” 밖에 볼 수
없다.
8. 영희는 다음을 계산한다.
860영희( @!1##%*(!")="사랑해"

위의 1단계에서 pubaaS 적용하는 ARES 암호화(600”0400)라 하고, 3단계에서 860ㅇ영희
를 적용하는 절차를 복호화(000”0400ㅁ라고 한다. 이 절차가 그림 11.1에 그림으로 표현
되어 있다. 영희만이 secqaS 알기 때문에 GS 암호문 cS 원래 메시지 로 복호화할


===== PAGE 511 =====
500     chapter 11 정수론 기반 알고리즘
철수의 친구들
c
_     b            10    Cc           b      "
철수-ㅡㅡ-러| pubga      P| 560영희 | 영희
그림 11.1 ASE 보낼 메시지 를 영희의 공개키로 암호화하고, 영희는 자신의 비밀키로 암호문
을 복호화한다. 철수의 Se 암호문 ㅇ밖에 볼 수 없다.

4)

수 있음을 주목하자. 따라서 첨수의 다른 ATES 암호문밖에 볼 수 없다.

이 방법은 pkey, BRE] skey,S 알아내기 불가능하거나 최소한 매우 어려운 경우에
한하여 문제없이 사용할 수 있다. 다음 절에서는 pkey, BPE} 6&6《,를 알아내기가 매우
어려운 체계를 공부한

11.7.2 RSA 암호체계

RSA 암호체계는 큰 소수를 찾는 작업은 꽤 쉽게 할 수 있지만, 큰 수를 인수분해
효율적인 방법은 없다는 사실에 의존한다. RSA 암호체계를 먼저 알아본 후, 큰 소
쉽게 찾고 큰 수를 인수분해하기 매우 어렵다는 사실을 더 토의해보자.

fl

에
fr

fu
\
mf

:

체계
RSA 공개키 암호체계(0194 public-key cryptosystems)o]*| 각 참여자는 다음 절차로 각
자의 공개키와 비밀키를 생성한다.

1, 매우 큰 소수 pS 0 FHS 선택한다. 와 를 표현하는데 필요한 비트의 개수는

10249] 수 있다.
2, 다음을 계산한다.
n= pq
g(n) = (p-1)(q- 1)
p(n) 공식은 정리 11,176] 따른다.
g(n)o 서로소인 작은 소수 를 선택한다

8.                     al                                :
4. 알고리즘 11.8을 사용하여 [0],(,;의 BA multiplicative inverse) 계산하다. 즉,

lated lated - (Ll pitas

따름정리 11.8에 따르면 그 역은 존재하고 하나 밖에 없다.
5. pkey = 00, 0)를 공개키로 하고, skey=(n, h)S 비밀키로 한다.

허용 가능한 메시지의 집합은 2,。이다. 공개키 pkey = (n, 0)에 대응하는 함수는

pub(b) = 00                                       01.29)



===== PAGE 512 =====
0000000
11.7 RSA 공개키 암호체계    501

여기서 b = 2,이다. 비밀키 6668 = (n, hol 대응하는 함수는

sec(b) = b"                                        (11, 30)
이 함수들의 He 알고리즘 11.5로 계산할 수 있다.
이 체계가 정확하기 위해서는 공개키와 비밀키에 대응하는 함수들이 각각 서로의 역이

어야 한다. 이제 이를 증명해보자.

& > Bal 11.33

등식 (11,29)2} (11,30) 2] 함수들은 서로 역이다.
증명 : 등식 (11.29)와 (11.80)에 따르면 모든 b © 2, 에 대해서
pub(sec(b)) =sec(pub(b)) =“
따라서 다음만 보여주면 된다.
oo = b
그러기 위해서 m & 》#라고 하자(6 ㄷ 2, 임을 상기). 그러면 77 © 이다. 이제 다음을 증명
하면 된다.
2], = 041,                                             (11,31)
gH 는 y(n) =(p-1)(q-1)S 법으로 하는 곱셈역이므로, 다음 등식이 성립한다.
lh lp—1)(@-1) = 46200
이는 다음 등식이 성립하는 정수 《가 존재함을 의미한다.
gh=1+k(p—1)(q-1)
2가지 경우가 존재한다.
경우 1 : Im], = 10],인 경우, 다음과 같다.

02], = la ees)
= [m],(fn]e-?) A
=[m],1K°»

= 1,
세 째 등식은 정리 11,220] 의해서 성립한다.
경우 3 : (m], = 10],이면, 다음이 성립한다.
2], = [210 = [0] = [0], = 021,

따라서 등식 11,319] 성립함을 증명하였다.


===== PAGE 513 =====
502

chapter 11 정수론 기반 알고리즘

뜨

|숫한 원리로 다음도 성립한다.

| = 201,

등식 11.312} 11,320] 의해서 다음 두 합동이 성립한다.

(11,32)

ms" =m mod p

=m mod q

그러므로 정리 11.18에 의해서 다음 ese] 성립하고,

h

772" =m mod n

앞에서 언급했듯이 RSA 암호체계의 ASS 큰 APS 찾는 작업은 꽤 쉽게 할 수 있지만,
큰 수를 인수분해하는 효율적인 방법은 없다는 apo] 의존한다. 즉, 다음과 같이 BA
수를 쉽게 찾을 수 있다. 먼저, 적절한 크기의 정수를 무작위로 선택한다. 11.6절의 앞부
분에서 설명했듯이 꽤 큰 소수를 찾는데 조차도 시간이 오래 걸리지 않는다. 선택한 각
정수에 대해서 다차시간에 실행되는 알고리즘 11.5를 사용하여 주어진 수가 소수인지 검
사할 수 있다. 큰 소수를 두 개 찾을 때까지 이 절차를 반복한다. 11.6절에서 설명했듯이
알고리즘 11.5가 알려지기 전에도 밀러-래빈의 무작위적 소수검사 알고리즘을 주어진 수
가 소수인지를 매우 낮은 오차율로 효율적으로 사용해왔었다. 사실, 밀러-래빈의 무작위
적 소수검사 알고리즘은 그 시간복잡도가 (0(66")이기 때문에 소수검사에 사용해도 문제
가 별로 없다. 여기서 $는 입력을 코드화하는데 필요한 비트의 개수이고, 는 알고리즘
에 오류가 발생할 확률이 2" “보다 크지 않도록 선택한 정수이다. 따라서 eS 40으로 선
택하면 오류가 발생할 확률은 2 = 9.0949 ×10 "보다 크지 않다.

반면, 수를 인수분해하는 다차시간 알고리즘은 아직 아무도 발견하지 못했다. nF 인
분해하지 않고 비밀키 skey = (n, 』)에서 A 값을 찾을 가능성은 존재한다. 그러나 효
율적으로 그렇게 하는 방법을 알아낸 사람도 아무도 없다. 현재 1024비트 정도 이상 크기
의 정수를 사용한다면 RSA 암호 체계로 보안을 성취할 수 있다.

a



===== PAGE 514 =====
연습문제

11.1절

1. 다음 각 정수의 약수를 구하시오.
(3) 72
(b) 31
(c) 123

2. /,17 이고 7 17이면, h | nas 증명하시오.

8. 두 정수가 서로 나누어지면, 그 두 정수는 같음을 보이시오.

4. 와 gS 소수라고 하자. 2 = 0+2이면, poh 0는 쌍둥이 소수([\ㅁ0 prime ㅁ400000)라고 한다.
쌍둥이 소수를 2개 찾으시오.

5. gcd(n, m) =gced(m, n) YS 증명하시오.

6. mi} no] 모두 짝수일 때 ged(m, n) = 2gcd(m/2, n/2)7} HBS 증명하시오.

7. > 72 > 0이면, ged(m, n) =ged(m, n—m)7} 성립함을 증명하시오.

8. #가 소수이고 0<7/<2#이면, 800(20, ^) =1이 성립함을 증명하시오.

9. Qe] 11, 5A] 논의한 대로 정수의 소인수분해가 유일함을 추론 11.2를 사용하여 보이시오.

10. 다음의 각 정수를 소수의 곱으로 내타내시오.
(a) 123
(b) 375
(c) 927

11. 정리 11.6을 증명하시오.

12. 정리 11.78 증명하시오.

13. 양의 정수 mF} nol] 대하여 ged(m, n) =lem(m, n)°] 성립함의 필요충분조건은 m=nY
을 중명하시오.

11.2절

14. 최상위수준에서 SSO] 800(68, 40)인 경우 알고리즘 11,19] 실행 SSS 상술하시오.

15. 알고리즘 11.1을 반복형으로 재작성하시오. 메모리 사용량은 상수이어야만 한다(즉, 공간복
잡도는 0(1)이다).

16.  으으 11.1을 사용하여 HESS 가장 간단한 형태로 표현하는 알고리즘을 작성하시

오. 유리수가 72/7/과 같이 분수의 형태로 주어진다고 가정해도 좋다. 여기서 my 7은

정수이다.

17. 최상위수준에서 SSO] Auclid(64, 40, ged, i, 7)인 경우 알고리즘 11,29] 실행 SSS 상술

하시오.


===== PAGE 515 =====
@0000000
chapter 11 정수론 기반 알고리즘

504

18.

Wis 사용하여 최대공약수를 Ale Gaels eH eased MH 참조). 그리
고 작성한              분석하라.

11.3절

19.

20.
21.

22.
23.

24.

2:
26.
27.

예제 11,219] (5, * )7} 그룹임을 보이시오.
정리 11.12를 증명하시오.

정리 1.18의 증명에서 연습문제로 남겨둔 부분이 있다. hy =ㅇ0024, …,가 성립하는 정수
가 존재함을 보이시오.

정리 11.14를 증명하시오.
s & 01, 이고 t € [4], 이면, sxt Elm 시이 성립함을 보이시오.

G=(S, *)7} 유한그룹이고 6 © 이면, af =aka™0] 성립하는 BS k, m > 1이 SAS
= 보의지우.

= [0], Bho [61], 19],,이면, (6 +)가 (4, +)의 부분그룹임을 보이시오.
정리 11.19를 사용하여 추론 11.8을 증명하시오.
그룹 (2, ×)에서 <12]16>=2;가 성립함을 보이시오.

11.4절

28.

29.
30.

다음 각 모듈러 방정식을 풀어보시오.
(a)  817 = [416

(b) [4], t= [5],7
알고리즘 13S 구현하고, 여러 예제를 실행해보시오.
방정식 [1], C= [3],과 [12], = [6];의 해를 모두 구하시오.

11.5절

31.

32.

33,

34.
35.

(3]3)"& 계산하시오.

72] 15승을 구하여 ([7],』)『“을 계산하시오.
알고리즘 11.4를 사용하여 (13],』)'*을 계산하시오.
알고리즘 11.4를 사용하여 ([7],)『“을 계산하시오.

을         1.4를 구현하고, 여러 예제를 실행해보시오.

ne.
aN

고리

11.6절

36.
37.

100보다 작거나 같은 소수의 개수를 구하시오.

균등분포에 따라서 1과 10,000 사이의 ASS 무작위로 뽑을 때, 뽑힌 수가 ASU 확률은

대략 얼마인가?



===== PAGE 516 =====
@eeee @ 0
면습문제  505

wo
00
i

포에 따라서 1과 10,000 사이의 정수를 1007] 무작위로 뽑는다고 가정하자. 뽑은 수
“en  모두 소수가 아닐 확률은 얼마인가?

39. no] 소수이고 1<ㅅ《흐7-1이면, Bln, k) = 0 mod 임을 보이시오. 여기서 Bln, 4)는
이항계수를 나타낸다.

40. 0가의 인수이고 &가 에서 0의 차수라면, " | Bln, k) YS 보이시오. 여기서 Bn, 4)
는 이항계수를 나타낸다.

41. 920+822와 2? -4은 n& 법으로 하여 합동인가?

42. (2-9)“은 4를 법으로 하여 (#*“-9)와 합동이 아님을 보이시오.

43, (2-5)*은 8을 법으로 하여 (2“-5)와 합동임을 보이시오.

44. 정리 11.29를 증명하시오.

45. 알고리즘 11.5를 구현하고, 여러 예제를 실행해보시오.

46. 보조정리 11.8을 사용하여 보조정리 11.4를 증명하시오.

47. 다음은 보조정리 1169] 증명에서 연습문제로 남겨둔 것이다. 다음이 성립함을 보이시오.
ord,(n) | lem (070.(201), ord, (p,), +++, ord, (p,))

48. 부등식 11,225 사용하여 바로 다음 부등식을 구하시오.

11.7절
49. 공개키와 비밀키의 다른 점은 무엇인가?
50. p=7, 0=11, 0=18을 사용하는 RSA 암호체계를 고려해보자.
(a) 7 RS 계산하시오.
00) < 값을 계산하시오.
(0 h RS 찾으시오.
51. p=23, 0=41, 0=8을 사용하는 RSA 암호체계를 고려해보자. 메시지 [847]qyg& 암호화하
지오.
52. 연습문제 51의 RSA 암호체계로 그 연습문제에서 암호화된 메시지를 복호화하시오.

53. RSA 암호체계에서 o(n)S 찾아낼 수 있다면 암호체계를 SS 수 USS 보이시오.

추가 문제
54. 소수가 무한대로 많이 존재함을 증명하시오.

55. ged 연산자는 결합법칙이 성립함을 보이시오. 즉,
gcd(m, gcd(n, h)) =ged(ged(m, n), h) 임을 보이면 된다.

56. mo] 올수이고 no] BPo]A ged(m, n) =ged(m, 7/2)임을 증명하시오.
57. m, n°] 모두 So], gcd(m, 2) =ged((m—n)/2, n) YS 증명하시오.
58. mx=my mod 이면 r=y mod no] 성립하는 BRAALS AOAC,


===== PAGE 517 =====
@0@000000
506     chapter 11 정수론 기반 알고리즘

59. 』가 소수라 가정하고, 2? =[1],9] 해들을 찾으시오.

60. RSA 암호체계에서 poh 00를 큰 소수, n=pgq, pubS 공개키하고 하자. pub(a)pub(b) 7} 을
법으로 하여 240(00)와 합동임을 보이시오.



===== PAGE 518 =====
Chapter 12

병렬 알고리즘 개론

CC) 2 울타리를 치려하는데, 기둥마다 하나씩 총 10개의 깊은 구덩이를 파야 한
다고 하자. 혼자서 10개의 구덩이를 차례로 파는 작업은 힘들고 재미없는 작업

일 것이라고 깨닫고 대안을 찾아본다. 마크 트웨인00480 Twain)2] 작품에서 대표적인
주인공인 톰 소여(200 Sawyer)7} 울타리를 하얀 페인트로 칠하는 작업을 재미있는 것처
럼 친구에게 속여서 자신을 SES 만든 이야기를 읽은 적이 있는가? 이와 비슷하지만
약간 수정한 영리한 계략을 쓰기로 결정한다. 건강에 신경을 많이 쓰는 이웃 친구들에게
뒤뜰에서 구덩이 파는 대회가 열린다고 안내장을 돌린다. 누구든지 가장 건장한 사람이
구덩이를 빨리 팔 수 있어야 우승하게 된다고 한다. 친구들이 상 자체의 값어치에 대해서
는 별로 중요하게 생각하지 않는다는 사실을 알고, 맥주 6캔 정도의 하찮은 1등 AS 제
공한다. 그래도 친구들은 자신들이 얼마나 건강한지 그저 증명하고 싶을 뿐이다. 대회당
일, 10명의 건장한 이웃 친구들이 모여서 10개의 구덩이를 동시에 판다. 이를 병렬 구덩
                        이 파기라고 이름 지을 수 있다. 자신은 별로 노동을 하지 않았고, 혼자서 차례로 판 경우

보다 훨씬 빨리 구덩이 파기를 마쳤다.
친구들이 병렬로 작업하게 하여 더 빨리 구덩이 파는 작업을 마칠 수 있는 것처럼 컴퓨


===== PAGE 519 =====
508

chapter 12 병렬 알고리

00

개론

터도 여러 개의 프로세서를 가지고 BBS 병렬로 실행하면 작업을 더 빨리 마칠 수 있다
(컴퓨터에서 BSAA (processor)= 명령과 데이터를 처리하는 하드웨어 부품이다). 지금
까지 이 책에서는 직렬적인(66446008]) 처리에 대해서만 논해왔다. 즉, 제시한 알고리즘
은 모두 전통적인 직렬 컴퓨터에서 실행되도록 설계되었다. 이러한 컴퓨터는 10개의 구
덩이를 혼자서 차례로 파는 것과 비슷하게 하나의 프로세서가 BBS 하나씩 직렬로 실
행한다. 이러한 부류의 컴퓨터는 존 폰 노이만(00820 von Neumann)o] 소개한 모델을 기
초로 한다. 그림 12.1에서 BHO] 이 모델은 중앙처리장치(26701 Processing Unit:
0#20)라고 하는 하나의 프로세서와 메모리로 구성되어 있다. 이 BAe 일렬로 나열된
명령을 하나씩 받아서 일렬로 나열된 데이터를 차례로 처리한다. 이러한 컴퓨터를 단일
명령흐름, 단일데이터흐름(91016 Instruction stream, Single Data stream: 81810) 컴퓨터
라고 하고, 직렬 컴퓨터(66091 computer) = 많이 알려져 있다.

컴퓨터에 프로세서가 많이 있어서 BBS 동시에 (병렬로) 실행한다면, 많은 BINS
더 빨리 풀 수 있을 것이다. 병렬 ABS 10명의 이웃 친구들이 10개의 구덩이를 동시에
파는 것과 같다. 예를 들어, 6.3절에서 공부한 신뢰 네트워크를 기억해보자. 그림 12.2에
신뢰 네트워크의 ARIS 보여준다. 신뢰 네트워크의 각 마디는 환자의 상태를 나타낸다.
첫째 마디에서의 상태가 둘째 마디에서의 상태를 야기할 수 있으면 마디를 잇는 이음선
을 연결한다. 예를 들어, 오른쪽 상단의 마디는 흡연자 상태이고, 그 마디에서 나오는 이
음선에 따르면 SAS 폐암을 초래할 수 USS 뜻한다. Alo] 주어진다고 해서 항상
잠재적인 결과가 발생하지는 않는다. 따라서 ZF 원인이 주어진 상태에서 각 결과가 나타
날 확률도 네트워크에 저장할 필요가 있다. 예를 들어, 흡연자가 될 확률(0.5)이 “흡연자”
마디에 저장된다. 흡연자가 폐암에 걸릴 확률(0.1)과 흡연자가 아닌 사람이 폐암에 걸릴
확률(0.01)이 "폐암" 마디에 저장된다. 폐결핵과 폐암에 걸린 사람이 ※선 가슴촬영에 양
성 반응을 보일 확률(0.99)과 원인들의 다른 3가지 조합을 가지고 가슴 ※선 가슴촬영에
양성 반응을 보일 확률들은 “KA 가슴촬영 양성"에 저장된다. 신뢰 네트워크에서 기본
수론 문제는 마디의 상태를 알 때, 나머지 다른 모든 마디들이 그 상태를 가질 확률을
결정한다. 예를 들어, 환자가 흡연자로 알려져 있고, ※선 가슴촬영에서 양성으로 판명된
다면, 환자가 폐암, 폐결핵, 호흡곤란, 최근에 아프리카를 방문한 적이 있는지에 대한 확
SS 알고 싶을 것이다. 펄(06821, 1980)은 이 문제를 푸는 추론 알고리즘을 개발하였다.
이 알고리즘에서 각 마디는 부모마디와 자식마디에 메시지를 보낸다. 예를 들어, SV}
※선 가슴촬영에서 양성 반응을 보였다는 사실을 알면, ※선 가슴촬영 양성" 마디는 그의

프로세서                                                           메모리

그림 12.1 전통 직렬 컴퓨터



===== PAGE 520 =====
0600000 0
병렬 알고리즘 개론     509

부모마디인 "폐결핵"과 "폐암“에 메시지를 보낸다. 이 마디들이 메시지를 받으면, 그 마디
의 FHS 가질 확률을 계산하고, 그 마디는 다시 그의 부모마디와 다른 자식마디에 메시
지를 보낸다. 이 마디들이 메시지를 받으면, 마디의 상태를 가질 새로운 확률을 계산하
고, 그 마디는 다시 메시지를 보낸다. 이 메시지 전달 절차는 뿌리와 잎에서 끝난다. 환자
가 흡연자이기도 하다는 사실을 알게 되는 순간, 그 마디에서 다시 메시지의 흐름을 시작
한다. 전통적인 직렬 컴퓨터는 한 Hol] 오직 하나의 메시지나 하나의 확률 값만 계산할
수 있다. "폐결핵"에 보내는 메시지 값을 먼저 계산하고, 페결핵이 걸릴 새로운 확률, 그
리고 “폐암“으로 보내는 메시지 값, 그 확률, 등등의 순으로 계산할 수 있다.

만약 각 마디에 프로세서가 하나씩 할당되어 있고, 그 프로세서는 다른 마디에 있는
프로세서에 메시지를 보낼 수 있다면, 먼저 계산하여 메시지를 "폐결핵'과 "폐암“에 보낼
수 있을 것이다. 이 마디들이 각각 메시지를 받고, 각각 독립적으로 계산하고 메시지를
부모마디와 다른 자식마디에 보낼 수 있을 것이다. 더구나 환자가 흡연자라는 사실도 안
다면, “흡연자” 마디는 동시에 계산하여 메시지를 자식마디에 보낼 수 있을 것이다. 이
모든 일이 동시에 일어난다면, 추론을 훨씬 빨리 끝낼 수 있을 것이다. 실세계에서 사용
되는 신뢰 네트워크는 종종 수백 개의 마디로 이루어져 있고, 추론되는 확률이 즉시 필요
하다. 이는 시간 절약이 아주 중요할 수 있다는 의미가 된다.

방금 설명한 것이 바로 병렬 컴퓨터(0878110 computer)2| 구조이다. 이러한 컴퓨터를
“병렬"이라고 하는 이유는 각 프로세서가 다음 프로세서와 동시에 (병렬로) VBS 실행
할 수 있기 때문이다. 프로세서의 비용이 지난 80년간 큰 폭으로 감소해왔다. 현재 마이
크로프로세서 기성품의 속도는 가장 빠른 직렬 컴퓨터의 10배 정도 빠르다. 그러나 가격
은 10배 정도 싸다. 따라서 이전 문단에서 설명한대로 마이크로프로세서를 연결하여 훨

아프리카

방문

0.01

0.02
0.001

0.99
0.95
0.94
0.001

×선 가슴
촬영 양성

그림 12.2 신뢰 네트워크


===== PAGE 521 =====
510

chapter 12 병렬 알고

ny
=
rH

들이고 가장 빠른 직렬 컴퓨터보다 빠른 계산 효과를 볼 수 있다. 병렬
2           한 이익을 AS 수 있는 분야가 많다. 인공지능에서의 응용 Boke 앞에서
언급한 신뢰 네트워크, 신경 네트워크에서의 추론, 자연어 이해, 대화 인식, 영상 인식이
있다. 데이터베이스 질문처리, 일기예보, 오염 감시, 단백질구조 분석 등에도 많이 응용

멸 컴퓨터를 설계하는 방법은 많이 있다. 12.1절에서는 병렬 설계에 필요한 고려사항
과 가장 널리 알려진 병렬 구조에 대하여 공부한다. 12.3절에서는 PRAM(Parallel Random
Access Machine)°]¢}31 하는 특정 종류의 병렬 컴퓨터에 대한 알고리즘 작성 방법을 설

적            PRAMS 직렬 계산 모델에서 간단히 일반화할
수 있다. 더구나, PRAM 알고리즘은 실제 많은 컴퓨터에 쓰이는 알고리즘으로 변환할 수
있다. 따라서 PRAM 알고리즘은 병렬 알고리즘의 개념을 소개하기에 알맞다.

12.1 병렬 구조

r
1194
4>
xo
ot

병렬 Ase (parallel computer)= 다음과 같은 세 가지 방법으로 구축

1, 제어 메커니즘(60201 mechanism)
2, 주소-저장장소 구성(2007688-80806 organization)

3. 상호연결 네트워크(104[60000ㅁ600[102ㅁ network)

12.1.1 제어 메커니즘
병렬 컴퓨터의 각 프로세서는 중앙제어장치의 제어 하에 작동할 수도 있고, 자체 제어장
치의 제어 하에 독립적으로 작동할 수도 있다. 첫째 종류의 구조를 단일명령흐름, 다중데
이터흐름(810언6 Instruction stream, Multiple Data stream: 81002)이라고 한다. 그림
12.8(8)는 SIMD 구조를 나타낸다. 그림에 표시된 상호연결 네트워크는 프로세서가 서로
정보를 주고받는 하드웨어를 나타낸다. 상호연결 네트워크는 12.1.8에서 자세히 설명한
다. SIMD 구조에서는 같은 명령이 중앙제어장치의 제어 하에 모든 처리장치에 의하여
S7|Al(synchronously) 0! 실행된다. 모든 프로세서가 각 주기마다 하나의 명령을 반드
시 실행해야 하는 것은 아니고, 프로세서 별로 연결이 끊어지는 주기가 있어도 괜찮다.

각 프로세서에 자체 제어장치가 있는 병렬 컴퓨터는 다중명령흐름, 다중데이터흐름
(Multiple Instruction stream, Multiple Data stream: MIMD)°]2}a2 한다. 그림 12.300)는
MIMD 구조를 나타낸다. MIMD 컴퓨터는 각 프로세서에 운영체제와 프로그램을 모두 저
장한다.

SIMD 컴퓨터는 같은 BBS 여러 가지 다른 데이터로 실행하는 프로그램에 적당하다.
이러한 프로그램을 데이터 병렬 BSA (data parallel program)o]e}31 한다. SIMD 컴



===== PAGE 522 =====
전체
제어장치

|                                            HMOLZAlg

@®eeeee 0
121 병렬구조 511

(a)                             (b)
프로세서

프로세서,                 제어장치,
프로세서,

프로세서,                                                              제어장치>

프로세서3

연결                     상호연결
네트워크                    네트워크

ZEA,
제어장치』

프로세서。

그림 12.3 (8) 단일명령흐름, 다중데이터흐름(6140) 구조, (6) 다중명령흐름, 다중데이터흐름
(MIMD) 구조

퓨터의 단점은 같은 주기 내에서 다른 명령을 실행할 수 없다는 것이다. 예를 들어, 다음

과 같은 조건문을 실행한다고 가정하자.

x+y US 알아낸 프로세서는 > = 임을 알아낸 프로세서가 명령 aw 실행하는 동안
쉬고 있어야 한다(프로세서들은 다른 데이터를 동시에 처리하고 있음을 상기하자). 그리
고 = 임을 알아낸 프로세서는 다른 프로세서가 명령 BS 실행하는 동안 반드시 쉬어

일반적으로, SIMD 컴퓨터는 7] (synchronization) & 요구하는 병렬 알고리즘에 가
당하다. 대부분의 MIMD 컴퓨터는 동기성을 제공하는 하드웨어를 추가적으로 가지
고 있어서 SIMD 컴퓨터를 흉내낼 수 있다.

장

1212  주소- 1장장소 = A

oo

A
프로세서는 공통 주소 저장장소에서 데이터를 수정하거나, 메시지를 전달하여 서로 통신


===== PAGE 523 =====
512

chapter 12 병

Access: UMA)

지역변

~
가 프로

렬 One

고 2

A 저장장소

구조를

다. UMA 컴퓨터의 단점은 상호

근을 제공해야 한다. 이로 인해서 성능이 급

주소 저장장소는 사용하는 BA

유 메모리의 일부분만 제공하는 것이다. 이 구조

(a)

프로세서,

독자 메모리,

1

프로세서

독자 메모리,

TEMA,

독자 메모리4

프로세서』。

[

독자 메모리』

ㄴㄴ

세서에 속한 메모리에 접근할 수 있지만 다른 프로세서에 속한

소 구조(3139760-8001688 apace—architecture) AE 공
읽기/쓰기0680/\1+6) 접근을 모든 프로세서에 하드웨어로 허용
서는 공유된 주소 저장장소에 있는 데이터를 수
세서가 메모리의 워드(\070)에 접근하는데 걸리는 시간이 모두 Z
를 보여준다. 이러한 컴퓨터를 균일한 메모리 접근(00107 Memory
컴퓨터라고 한다. 그림 12.4(8)에서 EO] UMA 컴퓨터에서 각 프로세서
는 독자 메모리를 가질 수 있다. 독자 메모리는 프로세서가 계산을 수행하는데 필요한
변수를 저장하는데만 사용한다. 알고리즘의 실제 입력은 독자 메모리 어디에도 없
연결 네트워크가 모든 프로세서의 공
격히 저하될 수 있다. Heke 각 프로세서에
는 그림 12,4(b)oj] 나와 있다. 이 메모
리는 그림 12.4(8)의 지역 메모리와 같이 독자적이지 않다. 즉, 각 프로세서는 다른 프로
메모리보다 자신에 속한

정함으로써 서로 Lay

유 메모리에 동시 접

(b)

!방법에 따라 다르게 구성된다.

oper

프로세서,

상호연결 ㅣ
네트워크

ao
on:

메모리

공유 메모리,

I

프로세서,

ㅣ

메모리>

프로세서3

공유 메모리3

그림 12.4 (a) 균일한 메모리 접근(474) 컴퓨

상호연결
네트워크

터, (6) at



===== PAGE 524 =====
@0000000
Qi 병렬 구조  513

메모리에 더 빠르게 접근할 수 있다. 만약 프로세서가 대부분 자신에 속한 메모리만 접근
한다면, 수행성능은 좋을 수밖에 없다. 이러한 컴퓨터를 균일하지 않은 메모리 접근
(nonuniform memory access: NUMA) 컴퓨터라고 한다.

메시지 전달 구조

메시지 전달 구조(202688886-20886108 architecture)oA] 각 프로세서는 자신만이 접근할
수 있는 독자 메모리를 가지고 있다. 데이터를 수정하는 대신 메시지를 전달하여 프로세
서는 다른 프로세서와 통신을 한다. 그림 12.5는 메시지 전달 구조를 보여준다. 그림 12.5
는 LH 12,4(b) 2} 거의 비슷해 보인다. 차이점은 상호연결 네트워크가 연결된 방법이다.
NUMA 컴퓨터의 경우 상호연결 네트워크는 다른 프로세서에 속한 메모리에도 접근할 수
있도록 각 프로세서가 연결되어 있다. 반면, 메시지 전달 컴퓨터에서는 각 프로세서가
직접 다른 프로세서에 메시지를 보낼 수 있도록 연결되어 있다.

12.1.3 상호연결 네트워크
상호연결 네트워크는 크게 정적(66800과 FA (dynamic) | 두 가지로 나눌 수 있다. 정적
네트워크는 메시지 전달 PAS 구축하는데 주로 사용되고, 동적 네트워크는 공유된 주

프로세서, 4
|
독자 메모리,
I
프로세서      때

|
독자 메모리,

프로세서, [4

[
독자 메모리』

도
29 FQ
LU ni

oz
10 fol

프로세서, |

[
독자 메모리, |ㅜㅜㅠ

그림 12.5 메시지 전달 구조. 각 프로세서의 메모리는 그 프로세서만이 접근 가능하다. 프로세서는
상호연결 네트워크를 통하여 서로 메시지를 전달함으로써 통신한다.


===== PAGE 525 =====
514

chapter 12 병렬 알고리즘 개론

소 저장장소 FAS 구축하는데 주로 사용된다. 하나씩 차례로 공부해보자.

정적 상호연결 네트워크

정적 상호연결 네트워크(66800 interconnection networks)= 프로세서 사이에 직접 연결
하는 링크가 있는데, 때로는 직접 네트워크(41700 networks)e}a! 한다. 정적 상호연결 네
트워크에도 여러 가지 종류가 있다. 주로 많이 사용되는 몇 개를 살퍼보자. 가장 효율적
이지만, 가장 비용이 많이 드는 네트워크는 그림 12.68/에 있는 완전연결 네트워크(602ㅁ-
pletely connected network)°]t}, 이 네트워크에서는 각 프로세서가 다른 모든 프로세서
와 직접 연결되어 있다. 따라서 송신 프로세서는 다른 수신 프로세서에 직접 연결된 링크
를 통하여 메시지를 보낼 수 있다. 링크의 개수는 프로세서의 개수에 대하여 제곱에 비례
하므로, 이러한 유형의 네트워크는 매우 비싸다.

별모양 네트워크(663-000060[60 network)]A] 프로세서 하나가 중앙 프로세서 역할
을 한다. 즉, 다른 프로세서는 모두 그 중앙 프로세서로 연결하는 링크가 있다. 그림
12,6(b)7} 별모양 네트워크이다. 별모양 네트워크에서는 어떤 프로세서가 다른 프로세서
에 메시지를 보내기 위해서는 먼저 메시지를 중앙 프로세서에 보내고, 그 메시지는 다시
수신 프로세서로 보내진다.

dA} 한정 네트워크[6040060-068"606 network) AE 각 프로세서가 최대로 4개의 다
= ZENA 연결되어 있다. 그림 12.6(0)는 4차 한정 네트워크이다. 4차 한정 네트우
크에서 메시지 전달할 때, 먼저 한 방향으로 따라 가다가 적당한 위치에서 방향을 바꾸어
도착 프로세서에 ESS 때까지 그 방향을 따라간다.

약간 더 복잡하지만, 더 많이 쓰이는 정적 네트워크는 하이퍼큐브(60906004686/이다. 0
차원 하이퍼큐브는 하나의 프로세서로 구성되어 있다. 1차원 하이퍼큐브는 2개의 0차원
하이퍼큐브에 있는 프로세서를 연결하여 만든다. 2차원 하이퍼큐브는 1차원 하이퍼큐브
의 각 프로세서를 다른 1차원 하이퍼큐브의 프로세서 하나에 각각 연결하여 만는다. 재귀
적으로 정의하면, (4+1)차원 하이퍼큐브((0+ 1) -dimensional hypercube) 0차원 하

(a)                                                          (b)                                                          (0)

O  O

그림 12.6 (a) 완전연결 네트워크, (6) 별모양 네트워크, (0) 4차 한정 네트워크



===== PAGE 526 =====
066000000
121 병렬 구조  515

)

0차원                      1차원                     2차원                      3차원

그림 12.7 하이퍼큐브 네트워크

이퍼큐브의 각 프로세서를 다른 0차원 하이퍼큐브의 프로세서 하나에 각각 연결하여 만
는다. 첫째 하이퍼큐브의 각 프로세서는 둘째 하이퍼큐브에 대응하는 위치에 있는 프로
세서에 연결된다.

메시지 전달 구조를 구현하는데 정적 네트워크가 보통 사용되는 이유는 바로 이러한
네트워크에서 프로세서가 직접 연결되어 있어서 메시지의 SSS 가능하게 하기 때문이
라는 사실은 명백하다:

동적 상호연결 네트워크

동적 상호연결 네트워크(474810410 interconnection network)]A] 프로세서는 여러 개의
AAAS 통하여 메모리에 연결되어 있다. 가장 간단한 방법으로 크로스바 스위치 네트워
A(crossbar switching network)7} 있다. 이 네트워크는 그림 12.8에서 보여주듯이 8개
프로세서가 스위치의 AA grid)\S 사용하여 m 742] 메모리뱅크(0ㅁ6001” bank)>] 연결
되어 있다. 예를 들어, 프로세서8이 현재 메모리뱅크8에 접근할 수 있다면, 그림 12.8 동
그라미 친 격자 부분에 스위치가 켜진다(스위치를 AW 회로를 연결하고 전기를 흐르게
한다). 스위치를 킬 때 프로세서와 메모리뱅크가 동적으로 연결되므로 이 네트워크는 “동
적"이라고 한다. 크로스바 스위치 네트워크는 차단이 불가(40001009708)하다. 즉, 하나의
프로세서가 어떤 메모리 뱅크에 연결되어 있다고 해서 다른 프로세서와 다른 메모리뱅크
의 ASS 차단하지 않는다. 이상적으로 크로스바 스위치 네트워크에는 메모리의 각 위
드마다 하나의 뱅크가 있어야 한다. 그러나 이는 분명히 비현실적이다. 보통 뱅크의 개수
는 최소한 프로세서의 개수만큼은 된다. 따라서 언제든지 프로세서가 최소한 하나의 메
모리뱅크에 접근할 수 있다. 크로스바 스위치 네트워크에서 스위치의 개수는 27이다.
따라서 m& per 크거나 같게 요구한다면, 스위치의 개수는 2^보다 크거나 같게 될


===== PAGE 527 =====
516     chapter 12 병렬 알고리즘 개론
메모리뱅크,    메모리뱅크    메모리뱅크, ㆍ ㆍ ㆍ |메모리뱅크,

프로세서,

프로세서,

프로세서4                    쁘트!

a,
』프로세서。
그림 12.8 크로스바 스위치 네트워크. 격자의 각 위치에 스위치가 있다. 셋째 프로세서를 현재
둘째 메모리뱅크를 연결하고 싶을 때, 프로세서3과 메모리뱅크2 사이에 정보를 흐르게 하도록 동그
라미 쳐진 부분의 스위치를 ACh.
것이다. 결론적으로, 크로스바 스위치 네트워크는 프로세서의 개수가 크면 상당히 비용
이 많이 들 수 있다.

여기서 공부하지 않을 다른 동적 상호연결 네트워크로는 버스기반 YEMA(bus—
based network) 2} 다단계 상호연결 네트워크(241\186386 interconnection network)7}
있다

공유된 주소 저장장소 구조를 구현하는데 왜 동적 상호연결 네트워크를 사용하는지
이제 이유가 분명하다. 즉, 이러한 네트워크에서 각 프로세서는 메모리의 각 워드에는
접근 허용하지만, 다른 프로세서에는 직접 메시지를 보낼 수 없다.

이 장에서 제시한 병렬 하드웨어의 소개는 0408, Grama, Gupta, 1817018의 책(1994)
에 있는 내용을 기초로 하였다. 더 철저한 (특히 버스기반과 다단계 상호연결 네트워크에
대한) 소개를 원하는 독자는 그 AS 참조하기 바란다.

@ 12,2 PRAM 모델

앞 절에서 공부했듯이 병렬 HAE 다양하게 구축이 가능하고, 실제 컴퓨터가 이 FAS
을 바탕으로 만들어진다. 반면에, 직렬 컴퓨터는 모두 그림 12.1의 구조와 같은데, 이는
폰 노이만 모델이 모든 직렬 컴퓨터의 보편적인02017678891) 모델이라는 의미이다. 이전
장에서 알고리즘을 설계하는데 폰 노이만 모델에 맞는 컴퓨터에서 실행되리라고 가정하
였다. 따라서 알고리즘을 구현하는 프로그래밍 언어나 컴퓨터가 다르다고 알고리즘의 시



===== PAGE 528 =====
@000000 0
11.2 PRAM 모델   517

간복잡도가 달라지지 않는다. 직렬 컴퓨터의 사용이 급격히 증가하게 된 것은 이 사실이
주요 요인이 되었다.

병렬 컴퓨터의 보편적인 모델을 찾는 일도 중요하다. 첫째, 많은 종류의 병렬 구조의
주 BAG 충분히 HAL 보편적인 BOS 찾아서 한다. 둘째, 찾은 weg poe
AAR 알고리즘은 실제 병렬 컴퓨터에서 효율적으로 실행되어야 한다. 이 두 AAS 만

ㅇ
>
x,
1
=

보          2 하지           아어 Random Access Machine) 컴퓨터는
병렬 컴퓨터의 이론 모델   태이 사용하고 있다. PRAM 컴퓨터는 8개의 프로세서로 구성
되어 있고, 프로세서는 모두 공유하는 큰 메모리에 균일하게 접근할 수 있다. 프로세서는
시스템 시계(04005)를 Bete 각 주기마다 다른 명령을 실행할 수도 있다. 따라서
PRAM 컴퓨터는 동기적, MIMD, UMA 컴퓨터이다. 따라서 그림 12.300)와 그림 12.4(8)가
PRAM 컴퓨터의 HAS 나타낸다. 그리고 그림 12.8은 PRAM 컴퓨터로 구축 가능한 상호

결 네트워크를 보여준다. 이미 언급했듯이 이러한 컴퓨터를 실제로 구축하기는 비용이
： 많이 들것이다. 그러나 PRAM 모델은 계산의 직렬 모델의 자연스런 확장이다. 따라서
알고리즘을 개발할 때 PRAM 모델은 개념적으로 쉽게 사용할 수 있다. 더구나, PRAM
모델에 쓸 목적으로 개발한 알고리즘은 더 현실적인 컴퓨터에 사용할 수 있는 알고리즘
으로 변환할 수 있다. 예를 들어, PRAM 명령은 프로세서의 개수가 pS 때 한정 네트워크

에서 Olle 7)개의 명령으로 시뮬레이션할 수 있다. 더욱이, 점근적으로 하이퍼큐브 알
고리즘만큼 빠른 PRAM 알고리즘이 있는 문제가 많이 있다. 이러한 이유로 PRAM 모델은
병렬 알고리즘을 소개하는데 좋은 역할을 한다.

PRAM 같은 공유메모리 컴퓨터에서 하나 이상의 프로세서가 같은 메모리 ALS 동시
   읽고 쓰는 작업을 시도할 수 있다. 동시 메모리 접근을 어떻게 처리하느냐에 따라서

모델의 종류를 4가지로 나눌 수 있다.
1, 독점읽기, $4247|(Exclusive—Read, Exclusive-Write: EREW),
이 PHS 동시에 읽기나 쓰기가 허용되지 않는다. 즉, 주어진 시간에 하나의 =
로세서만 하나의 메모리 장소에 접근이 가능하다. 동시성을 최소로 허용하므로
PRAM 컴퓨터 중 가장 약하다.
2. 독점읽기, §A]247](Exclusive—Read, Concurrent—Write: ERCW)

이 방법은 동시에 쓰는 연산은 허용하지만, 동시에 읽는 AALS 허용하지 않는다.
3. 동시읽기, 54247] (Concurrent—Read, Exclusive—Write: CREW)

이 방법은 동시에 읽는 연산은 허용하지만, 동시에 쓰는 AALS 허용하지 않는다.
4. 동시읽기, SA)47|(Concurrent—Read, Concurrent—Write: CRCW)

이 방법은 동시에 읽고 쓰는 연산을 모두 허용한다.

CREW PRAM 모델과 CRCW PRAM 모델에 대하여 알고리즘을 설계해보자. 먼저 CREW



===== PAGE 529 =====
518

chapter 12 병렬 알고리즘 개론

모델을 살펴보고, CROW =a 사용하여 어떻게 더 효율적인 알고       sacle 수있
는지 공부하자. 병렬 알           떻게 표현하는지 우선 살펴보자. ner 알고
현할 수 있는 프로그래밍  1 eter 있긴 하지만, 써오던 표준 의사코드를 일부 기능    —
하여 사용하도록 하자.

알고리즘을 작성하고
서 각 프로세서는 알고리
서는 P,, Po, Ps 등의
넘겨준다.

22 = index of this processor;

주

한 후, 모든 프로세서가 알고리즘을 동시에 실행한다. 이
실행하는 동안 자신의 인덱스를 알 필요가 있다. 각 프로
음과 같은 명령으로 프로세서의 인덱스를

\ fe
P ae

:

fl

os

ro, ㅁ
모
»
fl
N
르그:
Bo
Pt

알프러즘에서 aera 공유메모러 변수일 수 있는데, 의는 모는 프로세서가 의 더
수에 접근 키능하다는 뜻으 rh 또는 AMS 변수는 개인 메모리 변수일 수도 있다(크림
12,4(a) 참조). 개인 메모리 변수의 경우, 각 프로세서는 변수의 독자 ARES 가지고 있다.
개인 메모리 변수를 이 때 1008!이라는 키워드를 사용하기로 한다.

여기서 다루는 알고리즘은 12.1.1에서 Set 대로 모두 데이터-병렬 알고리즘이다.
S, BEAMS 데이터 Adel 있는 다른 데의터를 카지그 SS 명령 집합을 실행한다:
alain 집합은 공유메모리에 저장한다. 명령이 공유메모리에 저장되어 있는 데이터 집합
의 한 원소 값을 지역변수에 저장하면, 공유메모리에서 읽는다ㅠ680)라고 한다. 반면, 지
역변수의 값을 공유메모리의 데이터 집합에 저장하면, 공유메모리에 Sch write)epat 한
다. 공유메모리로부터 읽기와 공유메모리에 쓰기 명령만 가지고 이 데이터 집합의 원소
를 조작할 수 있다. 예를 들어, 공유메모리 데이터 집합의 두 개의 원소 값을 직접 비교하
지 않는다. 대신, 값을 지역메모리의 변수로 읽고, 그 변수의 값을 비교한다. 데이터 집합
의 크기 /,같은 변수들은 직접 비교를 허용한다. 데이터-병렬 알고리즘은 일련의 Ao
로 구성되어 있고, 모든 프로세서는 4 AWS 동시에 지작하의 동시에 ia  더구나
A Se 중에 읽는 프로세시들은 모두 동시에 읽고, 쓰는 프모세시들은 모두 농시
에 쓸데:

프로세서는 원하는 만큼 구할 수 있더크 가정한다, 이미 Serie] 실제로 이 기정은
비현실적이다.

다음 알고리즘은 이 관습에 따른 것이다. 공유메모리에 인덱스가 1부터 7,까지인 정수
배열 가 있고, 인덱스가 1부터 7까지인 7:개의 프로세서가 알고리즘을 병렬로 실행하고
있다고 가정한다.

void example (int n,                         // S= 공유메모리의 데이터 집합이다.

{

int St ])

local index p;
local int temp ;



===== PAGE 530 =====
@eeeee 0
11.2 PRAM 모델   519

p = index of this processor;
read S{p] into temp;                     // 이 B82 공유메모리에서 읽기이다.
if (p < n)

write temp into 912 + 1];                  // 이 명령은 공유메모리로 쓰기이다.
else

write temp into 911];

배열 Sol] 속한 값은 모두 nA] 다른 지역 변수 temps 동시에 읽는다. 그리고 7개의
변수 temp 들어있는 값들은 모두 SH 동시에 쓴다. 의 원소는 모두 그 앞에 있는
값이 주어진다(맨 앞에 있는 값은 맨 뒤의 값이 42°}4] (wraparound), 그림 12.9는 알고
리즘의 연산 절차를 나타내었다. SE 공유메모리이므로 각 프로세서는 전체 배열 에
항상 접근할 수 있다. 따라서 pHa BBA (p+ 1)번째 배열 슬롯에 쓸 수 있다.
이 간단한 알고리즘에는 Ago] 하나뿐이다. Ago] | 이상이면, 루프를 다음과 같이
}성한다.
for (step = 1; step <= numstep; step++) {

// 4 AQae 실행할 코드가 여기 온다. 4 프로세서는 AWS

// 동시에 시작하고, 동시에 끝난다. AWS 읽는 프로세서는

// 모두 동시에 읽고, AHee 쓰는 프로세서는 모두 동시에

IN
ot,

// 쓴다.
}

이 루프의 구현 방법은 여러 가지 있다. 하나는 증가와 검사를 하는 제어장치를 따로
두는 것이다. 다른 프로세서에게 언제 읽고, 언제 지역변수 명령을 실행하고, 언제 쓸 것
인지 알려주는 명령을 만들어 낼 것이다. 루프의 내부에서 항상 같이 일정한 변수를 계산

Ss    12      10      5      15

| ㅣ ㅣ |

P;      20 기

11 |

12      10      5      15

temp, temp, temp; temp,

NN

「

S| 15     12      10      5

그림 12.9 BAIA example2| 적용 예


===== PAGE 531 =====
520

chapter 12 병렬 알고리즘 개론

할 때가 가끔 있다. 예를 들어, 알고리즘 12.1과 12.8은 둘 다 다음 VIS 실행한다.
size — 2 * size;

여기서 size 값은 항상 일정하다. 이렇게 값이 일정한 변수는 프로세서별로 값을 따로

가지고 있을 필요가 없으므로, 공유메모리 변수로 저징 그 명령은 따로 마련한 제어

장치로 실행하도록 구현할 수 있다. FAY TANS 더 이상 설명하지 않겠다. 대신
알고리즘을 작성해보자.

12.2.1 CREW PRAM 모델에 대한 알고리즘 설계
다음의 예제 문제를 가지고 CREW PRAM 알고리즘을 설명한다.

배열에서 가장 큰 키 찾기
정리 8.?에서 키만 비교하여 가장 큰 키를 찾으려면 최소한 n— 1번 비교를 해야 한다고
증명하였다. 직렬 컴퓨터로 수행하도록 알고리즘을 설계하면 시간복잡도가 O(n)o] 됨
을 의미한다. 병렬 알고리즘을 사용하면 실행시간을 향상시킬 수 있다. 병렬 알고리즘도
최소한 m4 비교는 해야 한다. 그러나 병렬로 하면, 더 빨리 끝낼 수 있다. 이제
병렬            발해보자.
알고리즘 &.9(가장큰 키 Ae) 다음과 ol 하여 가장 큰 키를 가장 빨리 찾는다
void find_Jargest (int n,

const keytype 의],
keytype& J/arge)

{
index /;
large = S{ 1];
for (7 = 2; 7 <= nm; i++)
if (S[i] > Jarge)
large = 의기:
}
이 알고리즘은 루프의 몸체를 실행한 결과를 다음에 몸체를 실행할 때 사용하므로 프로
세서를 더 많이 사용해봐야 전혀 도움이 되지 않는다. 8.5.3절의 가장 큰 키를 찾는 토너
먼트 방법을 연상해보자. 이 HHS 수를 두 그룹으로 나누어 각 그룹에서 가장 큰 값(승
자)을 찾는다. 그리고 키가 하나만 남을 때까지 이 HSS 계속한다. 그림 8.10에서 이
과정을 설명하고 있다. 토너먼트 WHS 푸는 직렬 알고리즘은 알고리즘 8.2와 시간복잡
도가 같다. 그러나 토너먼트 방법에서 프로세서를 더 사용하면 실행시간을 향상할 수 있
다. 예를 들어, 토너먼트 방법을 사용하여 8개 키 중에서 가장 큰 키를 찾고 싶다고 하자.
9회전을 치르기 전에 1회전에서 차례로 승자 4개를 결정해야 한다. 추가로 프로세서 3개



===== PAGE 532 =====
@‥ㅎ00000 0
11.2 PRAM 모델   521

의 도움을 받으면, 1회전의 승자 4개를 동시에 결정할 수 있다. 이는 1회전의 승자를 4배
빨리 결정할 수 ache 의미가 된다. 1회전이 끝나면, 프로세서 2개만 가지고 2회전 비교
를 실행할 수 있다. 결승전에서는 프로세서가 하나만 필요하다.

그림 12.10은 병렬 알고리즘이 이 방법을 어떻게 실행하는지 보여준다. 배열 크기의
반만큼의 프로세서만 필요하다. 각 프로세서는 두 개의 배열 AAS 지역변수 first}
second 읽어 들인다. 그리고 479/와 second 중 큰 값 읽은 배열의 첫째 슬롯에 쓴다.
이런 식으로 세 번 반복하면, 가장 큰 키는 Sl) 저장된다. 각 회전은 알고리즘의 한
ARO] 된다. 그림 12.10의 예제에서 7=8이고, AWS] 개수는 18 = 37} 된다. 알고리
즘 12.12 그림 12.10에서 보여준 동작을 실행하는 알고리즘이다. 이 알고리즘은 Beez
작성되었음을 주목하자. 병렬 알고리즘이 함수로 작성되었으므로, 최소한 하나의 프로세
서는 값을 내주고, 내주는 값은 항상 일정해야 한다.

+ 알20증 121 가장 큰 키 병렬로 찾기
문제 : 크기가 인 배열 SHA 가장 큰 키를 찾아라.
입력 : 양의 정수 n, 인덱스가 1부터 7,까지인 키의 배열 9
출력 : Sop 가장 큰 키의 값
주석 : nS 29) 거듭제곱이고, 알고리즘을 병렬로 실행하는 프로세서가 2/2개 있다고 가
정한다. 프로세서는 인덱스가 1부터 7/2까지로 되어 있고, “index of this 0ㅠ000880『 라는
명령은 현재 사용 중인 프로세서의 인덱스를 내준다.

keytype parlargest (int 2, keytype S[ ])

index step, size;
local index p;
local keytype first, second ;

p = index of this processor;
size = 1;                               // size= 부분배열의 크기
for (step = 1; step <= lg n ; step++)
if (this processor needs to execute in this step){
read S[2* p—1] into first;
read S'[2* p—1 + size] into second;
write maximum(first, second) into S{2 * p— 1];
size = 2* size;
}

return 91 1];

알고리즘의 명확성을 가능하면 유지하기 위하여 “if (this processor needs to execute


===== PAGE 533 =====
@“@0 0 06 0 0 ee
522     chapter 12 병렬 알고리즘 개론

in this step)’2} 같이 추상적인 의사코드를 사용하였다. 그림 12.10을 보면 임의의 정수
k(size 값은 각 AM} 배로 증가함을 주목)에 대해서 각 AR] 사용되는 프로세서는

7 7 V7 7
J\ /\, /\. /\,

 Se a ae Ve et fo ae

\   / \   /

큰 값을 쓰기                  P,                  Pp                  Ps                  P,

ff sf /

S    12     10     15     15     18     12     16     16

읽기

읽기                  Py

—~ a

12                             15                               “                             16
first,                  second,                  firs:                       seconds

ru
기
milo
Ir
N
교

12    16    16

읽기                                                                 P,
15                             18
first,                  second,

lu
a
10
I=
SS
49

S     18      10      15      15      18      12      16      16

가장 큰 값이 여기에

그림 11.10 병렬 프로세서를 사용하여 가장 큰 키를             「

%에
TP

제를 토너

|모
\m
o£
[또
10
fu
aul
[에
=
ital

Ao



===== PAGE 534 =====
> 알고리즘 12.2

@0000000
11.2 PRAM 모델   523

인덱스가 다음과 같다.
p=lt+size*k
따라서 프로세서가 실제로 실행되어야 하는지에 대한 점검은 다음과 같이 한다.
if ((2-1) % size == 0)     // %는 p-1& size@® 나눈 나머지를 BAS

대안으로 모든 프로세서가 각 AMS 실행하도록 허용할 수도 있다. 이 경우 실행할 필요
없는 프로세서는 단순히 쓸데없는 비교를 한다. oS 들어, 2회전에서 프로세서 PLE
3]값과 915]값을 비교하고, 큰 값을 9[3]에 써넣는다. 이 과정이 비록 필요하지는 않
쉬게 하여 얻을 게 없으므로 ^,를 실행시켜도 된다. 중요한 AALS 실행해야
프로세서는 실행시키고, 다른 프로세서는 실행 중인 프로세서가 사용하는 메모리
의 값을 바꾸지 말아야 한다는 것이다. 불필요한 프로세서가 BBS 실행하여 발생
{는 문제는 가끔 배열 의 범위를 벗어나는 배열 요소를 가리킨다는 것이다. 예를

어, 앞의 알고리즘에서 Pye 2회전에서 S[9]S 가리킨다. So] 추가 슬롯을 덧붙이면
처리할 수 있다. 이렇게 하여 공간을 낭비하는 대신, 프로세서를 수행할지 말지 점검하는
절차를 없애서 시간을 절약할 수 있다.

병렬 알고리즘을 분석할 때 알고리즘이 실행한 총 작업의 양을 분석하지 않는다. 대신
하나의 프로세서가 ABS 총 작업량을 분석한다. 왜냐하면, 그래야 컴퓨터가 입력
마나 빨리 처리하는지 제대로 알 수 있기 때문이다. 알고리즘 12.1의 for—step 루프를
각 프로세서가 약 len 실행하므로, 시간복잡도는 다음과 같다.

가
sl

NO ON

oe Sy 그

ty  He et

6              v
auf

때 (Het
+»
x
|r

Ho,

가

으 의
를 은
르

T(n) € Ollg n)

이 시간복잡도는 병렬 알고리즘이 직렬에 비하여 성능이 훨씬 SSS 보여준다.

Dy
과
Ser
오
»,
ott
으
i
=
ㅣ
es
i
4N
2
ea
re
|!
we
qu
rlo
띠 모
Be
a
a
두
N
lr
의
i
ok

병렬로 이항계수 구하기
문제 : 이항계수를 구하라
입력 : 음이 아닌 정수 과 《, 여기서 k<n

출력 : 00722(이항계수 |

주석 : k+ 1개의 프로세서를 가지고 병렬로 계산한다고 가정한다. 프로세서는 0부터 *까


===== PAGE 535 =====
@00@000000
524     chapter 12 병렬 알고리즘 개론

A] 인덱스되어 있고, “index of this processor” BAO 프로세서의 인덱스를 내준다.

int parbin (int n, int 2)

{

// step 대신 7 사용하여 알고리즘 3.29} 일관되도록
index 7;                            // 28S 조절한다.
int BO .. 기 0 .. A;
local index j;                      // p 대신 FS 이용하여 알고리즘 3.29} 일관되도록
local int first, second ;              // 되도록 프로세서의 인덱스를 구한다.

Jj = index of this processor ;
for (7 =0; 7 <= nm; H+)
if (7 <= minimum(i, k))
if (f ==0 || j == 2)
write 1 into Bi i][ 7];
else{
read Bli-1][j-1] into frst;
read Bii-1][j| into second;
write first + second into Bi 기[./];
}
return B{n|[4);

알고리즘 3,22] 다음 제어문은

for (j = 0; 7 <= minimum(i, 2; j++)
이 알고리즘에서 다음 제어문으로 대치된다.

if (7 <= minimum(i, 0)

왜냐하면 for-i FES 한 번 실행할 때마다 《개의 프로세서가 모두 한꺼번에 실행하기
때문이다. 7가 0부터 minimum(i, k) AAS] 값일 때 212][71의 WS 직렬로 계산하는
대신, 병렬 알고리즘은 0부터 minimumi(i, k) 범위의 인덱스를 가진 프로세서가 동시
에 값을 계산한다.

병렬 알고리즘에서 루프를 실행하는 ASE 7+1이다. 직렬 알고리즘(알고리즘 3.2)
에서 루프를 실행하는 APE O(nk) YS 기억하자.

연습문제 3.4를 돌이켜보면, 0부터 《까지의 인덱스를 가진 일차원 배열 #만 사용하여
알고리즘 3.2를 구현할 수 있다. 병렬 알고리즘의 경우 이렇게 수정하기는 매우 쉽다.
왜냐하면, For—i 루프의 번째 입구에서 파스칼 삼각형의 (i — 1)번째 행 전체는 Bl
변수 first2} second2| 《개의 지역 쌍으로 읽을 수 있다. 그리고 출구에서 :째 해 전체는
쇼로 쓸 수 있다. 의사코드는 다음과 같다.

for (7 = 0; i <= n; 가+)
if (j <= minimum(i, k))

fe i es 2
write 1 into Bij];



===== PAGE 536 =====
> 알고리즘 12.3

@‥ㅎ00000 0 0
11,2 PRAM 모델   525

else {
read Bl j—1] into frst;
read B[j] into second;
write first + second into Bij];

}
return Bl 4];
병렬 정렬
동적계획 합병정렬 8(알고리즘 7.8)을 기억해보자. 그 알고리즘은 키 하나로 시작하여 7]

두 개가 ASS 리스트로 합병하고, 다시 키 네 캐가 BBS 리스트로 합병하고, 이런
식으로 계속 합병한다. 즉, 그림 2.2와 같이 합병한다. 이 합병과정은 토너먼트 방법을
사용하여 최대값을 찾는 것과 매우 비슷하다. 즉, 각 AMA 합병을 YAH 실시한다.
ABS] 용이성을 위하여 은 29] 거듭제곱이라고 가정한다. no] 22] 거듭제곱이 아닌
경우 배열의 크기는 2의 거듭제곱으로 취급할 수 있지만, 7째 이후는 합병하지 않는다.
동적계획 합병정렬 (알고리즘 7.9)은 PIS 병렬로 어떻게 수행하는지 보여준다.

병렬 합병정렬

문제 : 감소하지 않는 순서로 7개 키를 정렬

입력 : 양의 정수 7, 키의 배열 ,(인덱스는 1부터 72)

출력 : 감소하지 않는 순서로 정렬된 키들을 구성된 배열 Ss

주석 : n& 29] 거듭제곱이고, 7/2개의 프로세서가 알고리즘을 Yas 실행한다. 프로세
서는 1부터 7/2까지 인덱스를 가지고, “index of this ㅁㅠ0008807 는 프로세서의 인덱스를

내준다.

void parmergesort (int 2, keytype 이 ])

{

index step, size;
local index p, low, mid, high;
p = index of this processor;

sizer = 1;

// size= 합병하는 부분배열의 크기

for (step = 1; step <= lg n; step++)
if (this processor needs to execute in this step){
low = 2*p-1;
mid = low + size—1;
high = low + 2* size—1;
parmerge(low, mid, high, S$);
size = 2* size;

}

void parmerge (local index 00, local index mid, local index high,


===== PAGE 537 =====
526

chapter 12 병렬 알고리즘 개론

keytype 이 ])

local index i, j, 4;
local keytype first, second, Ullow..high);

I= low; j = mid + 1; k = low;
while (7 <= mid && j <= high){
read S{i] into first ;
read S{j] into second;
if (first < second){

의 | = 29,
i++}
}
else {
U| 4] = second ;
I++;
}
k+4;
}
if (¢ > mid)
read S[j] through S{high| into U[A| through Ulhigh];
else

read 91 7] through S{mid| into U[A| through U{high|;
write U[/ow| through U[Aigh] into S{/ow| through S[high|;

v
bat

어떤 Ago] 프로세서가 실행해야 하는지의 BAS 알고리즘 12,19] 점검방식과 같
다. 즉, 다음과 같이 점검한다.

if ((2-1)% size== 0)  // %는 2-1을 size] 나눌 때 나머지를 내준다.

프로세서 하나로 반복적 실행하는 합병정렬(알고리즘 ?.9/에서 레코드 대입 SHE
for FES 수행하면서 US 의 역할을 바꾸어서 줄일 수 있음을 상기하자. 여기에서
도 같은 방법으로 향상시킬 수 있다. 이렇게 하면, VE 공유 메모리에서 인덱스가 1부터
까지 배열이 되어야 할 것이다. 그저 간단히 parmergeS 표현하기 위해서 그렇게 했을
뿐이다.

이 알고리즘의 시간복잡도는 금방 알 수 없다. 따라서 정식으로 분석해보자.

|악 시간복잡도 분석

단위연산 : parmerge|A|2] 비교
입력크기 : 배열에서 키의 개수, n

이 알고리즘은 일반 직렬 합병정렬과 비교 횟수가 정확히 같다. 단지 비교를 병렬로 수행



===== PAGE 538 =====
@‥ㅎ60000 0 0
11.2 PRAM 모델   527

한다는 것만 다르다. for—step 루프의 첫째 패스에서는 키가 하나만 있는 n/27H 쌍의 배
열을 동시에 합병한다. 따라서 어떤 프로세서도 최악의 경우 비교 횟수가 2-1=1이다

2절의 알고리즘 2,39] 분석을 참조하라). 둘째 패스에서는 키가 둘 있는 7/4개 쌍의
HAS 동시에 합병한다. 따라서 최악의 경우 비교 횟수는 4-1= 3이다. 셋째 패스에서
는 키가 4개 있는 7/8개 쌍의 배열을 동시에 합병한다. 따라서 최악의 경우 비교 횟수는
8-1= 7이다. 일반적으로 ?째 패스에서는 키가 2 개 있는 7/2'개 쌍의 MAS 동시에
합병하고, 최악의 경우 비교 횟수는 2'ㅡ1이다. 최종적으로, 마지막 패스에서는 키가 n/2

있는 DH] MAS 합병하고, 따라서 이 패스에서 최악의 경우 비교 횟수는 1 -1이다.
최악의 경우 각 프로세서가 실행하는 총 비교 BEE 다음과 같이 계산한다.

Wn) =14+34+7+--+2'-14+--+n-1

1872

= 20    )=2n-2-lgn€ O(n)

마지막 등식은 부록 Ao] 예제 ago] 결과와 대수적인 조작을 적용하여 얻는다.

키의 비교에 의한 병렬정렬을 1차시간에 성공적으로 수행하였다, 이는 JAVA O(n
187)에 비하여 성능이 현저하게 향상되었음을 의미한다. 병렬정렬을 ㅇ((187)”) 시간
에 하도록 병렬합병 알고리즘을 개량할 수 있다. 개량 알고리즘은 연습문제로 해보도록
한다. 개량 알고리즘도 최적은 아니다. 왜냐하면, 병렬정렬을 ㅇ(18 70) 시간에 수행할 수
있기 때문이다. 병렬정렬을 자세히 알아보려면 Kumar, Grama, Gupta, Karypis2] 책
(1994)과 Akl2] 책(1985)을 보라.

12.2.2 CRCW PRAM 모델에 대한 알고리즘 설계
CRCW+ Concurrent—Read, Concurrent—Write(4$-A] 읽기, 동시 쓰기)의 약자임을 상기
하자. 동시 읽기와는 달리, 동시 쓰기에서는 두 프로세서가 같은 ARIA 같은 메모리
장소에 쓰려고 할 때 충돌이 발생하므로 이에 대한 해결방안을 강구해야 한다. 충돌 해결
에 가장 빈번히 쓰는 프로토콜은 다음과 같은 것들이 있다.
* 일반(602ㅁㅁ020) 모든 프로세서가 같은 값을 쓰는 경우에만 동시 쓰기를 허용한다.
¢ 임의(32604ㅠ875) 임의의 프로세서를 그 메모리 장소에 써도 되는 프로세서로 선정한다.
우선순위(0ㅁ02469) 모든 프로세서에 우선순위를 미리 정해두고, 가장 높은 우선순위
를 가진 프로세서가 우선으로 쓸 수 있게 한다.
* 합(6000) 프로세서늘이 쓰는 Oe 합을 쓴다(이 프로토콜은 쓰는 값의 다른 얻산자를
적용할 수도 있다).

ㄴㄴ
수

일반-쓰기 프로토콜, 임의-쓰기 프로토콜, 우선순위-쓰기 프로토콜과 작동하며, CREW


===== PAGE 539 =====
528

chapter 12 병렬 알고리즘 개론
T   |    1    q    1
Ss  15   10   18   12
ee ae 이
읽기           Prp               Pig               Pig               Pog               Poa               Poa
?,' #\ £\ 065 LY S\N
15   10   15   18   15   12   10   18   10   12   18 123

배일 0 월 0 디노 될

          Pro             써3             Pra             Pog             Poa             P34
T      0        0        1        0

그림 12.11 알고리즘 12.4의 적용사례. 713]만 10] 되었다. 왜냐하면, .913]가 가장 큰 키이므로
비교에서 지지 않는 유일한 키이다.

모델의 알고리즘(알고리즘 19.1)보다 빠르게 실행되는 배열에서 가장 큰 키를 찾는 병렬
알고리즘을 작성해보자. 이 병렬 알고리즘은 다음과 같이 진행된다. 7개의 키가 공유 메
모리의 배열 Sol 있다고 한다. 공유 메모리에 7개의 정수 배열 TH 또 하나 만들고,
7의 원소는 모두 1로 초기화한다. 다음과 같은 인덱스된 n(n— 1)/279 프로세서가 있다
고 가정한다.

062   여기서 1l<i<j<n

모든 프로세서가 Sli) SS 병렬로 비교한다. 이런 식으로 So] 속한 원소는 모두
6에 속한 다른 모든 원소와 비교한다. 각 프로세서는 Sli] 7} 비교에서 지면 710]에 0을
써넣고, 17]가 지면 Till 0을 써넣는다. 가장 큰 키만 비교에서 지지 않는다. 따라서
T2| 원소 중에서 19] 되는 원소는 결국 하나뿐이며, Sk] ol 가장 큰 키가 들어 있는 경우
T{k] 가 1°] 된다. 따라서 알고리즘은 714] = 1이 되는 Slk] S| 값을 내주기만 하면 된다.
그럼 11.11에서 이 과정을 그림으로 보여준다. 이 알고리즘에서 하나 이상의 프로세서가
같은 메모리 장소에 쓰려 할 때 모두 같은 값을 쓴다는 사실을 주목하자. 이는 일반-써넣
기, 임의-써넣기, 우선순위-써넣기 프로토콜과 이 알고리즘이 맞게 작동됨을 의미한다.

> 알고리즘 12.4    병렬 CROWS 가장 큰 키 찾기

문제 : 키가 개인 배열 SOA 가장 큰 키 찾기
입력 : 양의 정수 7, 키의 배열 (인덱스 범위는 1부터 7)
출력 : 에서 가장 큰 키의 값



===== PAGE 540 =====
@‥《0 00000 0
11.2 PRAM 모델

in 29) 거듭제곱이고, n(n—-1)/279] 프로세서로 알고리즘을 병렬로 실행

ES
ㅜㅋㄱㅋ
고 가정한다. 프로세서는 다음과 같은 MAS 가지고,

PP, 여기서 1<i<jen

항

529

한다

“first index of this processor” 명령은 i ZS 내주는 반면, “second index of this process—

or Bae js 내준다.

keytype parlargest2 (int n, const keytype ST ])

{

int 7[1.. a];

local index i, /;

local keytype first, second;
local int chkfrst, chkscnd;

7 = first index of this processor;
j = second index of this processor;
write 1 into 212];// 1<i<n—-1°|3 2<j< nolHs,

write 1 into 7[/];                    // 이 write BAS 7의 각 MAS 1로
read S{i] into first;                   // 초기화 한다.
read 1 ./] into second;
if (first < second)
write 0 into 212];                   // 1 k\7t i 되면,
else                             // ST 4]는 최소한 한 번 비교에서 진다.
write 0 into 217];
read 717] into chkfrst ;
read 271.7/] into chkscnd;
if (chkfrst == 1)                         // TL k]7+ 아직 0이면, {7} 가장 큰 키이다.
return 의 기;                         // 가장 = 키가 9|끼인 경우,
else if (chkscnd == 1)                   // 71./]를 검사할 필요가 있다.
return 91];                        // i 값의 범위는 1부터 4-1까지임을 상기하자.

이 알고리즘은 루프가 없다. 이는 가장 큰 키를 상수시간에 찾는다는 의미이다. 10개
키에서 가장 큰 키를 찾는데 걸리는 시간과 같은 시간에 1000,000키에서 가장 큰 키를
찾을 수 있다는 의미가 된다. 그러나 이 최적 시간복잡도는 8차시간 프로세서 복잡도를
희생시켜 얻어낸 것이다. 1000,000개의 키 중에서 가장 큰 키를 찾는데 약 1,000,000°/2

개의 프로세서가 필요하다.

이 장은 병렬 알고리즘을 간단히만 소개하였다. 자세히 소개하려면 병렬 알고리즘만으
로도 책 한권 분량이 필요하다. 병렬 알고리즘을 자세히 소개한 책으로 Kumar, Grama,

Gupta, Karypis7} 공동으로 쓴 책(1994)을 추천한다.


===== PAGE 541 =====
530    chapter 12 병렬 알고리즘 개론
@ ASS
12.14

. 한 사람이 《, 시간에 두 수를 더할 수 있다고 가정하면, 덧셈을 단위연산으로 하여 그 사람이
두 개의 nxn VAS 더하는데 얼마나 시간이 걸릴까? 왜 그런 답이 나왔는지 이유를 밝히
시오.

2. 두 사람이 수를 더하고, 한 사람이 두 수를 더하는데 《, 시간이 걸린다면 VIS 단위연산으
로 하여 그 두 사람이 두 개의 nxn YAS 더하는데 얼마나 시간이 걸릴까? 왜 그런 답이
나왔는지 이유를 밝히시오.

3. 두 개의 nxn PAS 더하는 문제를 고려해보자. 한 사람이 두 수를 더하는데 《, 시간이
걸린다면, 최종 PS 구하는데 소비한 총 AAS 최소화하기 위해서 몇 사람이 필요할까?
사람이 충분히 있다면 답을 찾는데 필요한 최소 시간은? 왜 그런 답이 나왔는지 이유를 밝히
시오.

4. 한 사람이 《, 시간에 두 수를 더할 수 있다고 가정하고, 덧셈을 단위연산으로 하여 리스트의
개 수를 모두 더하는데 얼마나 시간이 걸릴까? 왜 그런 답이 나왔는지 이유를 밝히시오.

5. 두 사람이 리스트의 7개 수를 더하고, 한 사람이 두 수를 더하는데 《, 시간이 걸린다면 덧셈

을 단위연산으로 하고, 한 사람이 다른 사람에게 덧셈의 결과를 전달하는데 걸리는 시간 1
포함하여 이 두 사람이 리스트의 7/개 수를 모두 더하는데 얼마나 시간이 걸릴까? 왜 그

답이 나왔는지 이유를 밝히시오.

AES 7개 수를 더하는 문제를 고려해보자. 한 사람이 두 수를 더하는데 《, 시간이 걸리

한 사람이 다른 사람에게 덧셈의 결과를 전달하는데 전혀 시간이 걸리지 않는다고 가정

면 최종 답을 얻는데 소요되는 총 시간을 최소회하는데 필요한 사람은 몇 명인가? 사람이

분히 있다면 답을 찾는데 필요한 최소 시간은? 왜 그런 답이 나왔는지 이유를 밝히시오.

[또  EG

>
- ae

3

oft 운
에

~

12.2절
7. 60870) 시간에 리스트의 n7 수를 모두 더하는 CREW PRAM

8. 프로세서 ”^개를 사용하여 두 개의 nxn 행렬을 were © CROW PRAM 알고리즘을 작성하시

오. 작성한 AIFS O(n’) 시간 직렬 알고리즘보다는 수행 성능이 좋아야 한다.
9. 프로세서를 개 사용하여 크기가 인 리스트를 정렬하는 퀵정렬 PRAM 알고리즘을 작성하
시오.

10. 키가 개인 배열에서 가장 = 키를 찾
작성하시오. 작성한 알고리즘ㅇ

KH
AN lr
IN
use
im
by
au
ㅁ

11,        AAS "개 사용하여 두 개의 nxn 행렬을 곰하는 PRAM 알고리즘을 작성하시오. 작
알고리즘은 06087) 시간에 실행되어야 한다.

12. 3,289] 최단경로 문제를 푸는 PRAM 알고

분



===== PAGE 542 =====
플로이드의 알고리즘(알고리즘 3.9)과 비교하시오.
13. 3.4절의 연쇄행렬곱셈 문제를 푸는 PRAM 알고리즘을 작성하시오. 작성한 알고리즘의 성능
을 최소곱셈 알고리즘(알고리즘 3.0)과 비교하시오.
14. 3.5절의 최적 이진검색트리 문제를 푸는 28444 알고리즘을 작성하시오. 작성한 알고리즘의
성능을 최적 이진검색트리 알고리즘(알고리즘 3,93} 비교하시오.

추가적인 문제

15. 개 수로 구성된 리스트에서 수를 더하는 SAS 생각해보자. 한 사람이 ?/개의 수를 모두
더하는데 《,(ㅁ1) 시간이 걸린다면, m 사람이 』(ㅠ-1)1/'보다 작은 시간에 합을 계산
할 수 있는가? 왜 그런 답이 나왔는지 이유를 밝히시오.

16. 합병정렬 문제를 ㅇ(087)") 시간에 실행하는 PRAM 알고리즘을 작성하시오. GG: 프로
세서를 7개 사용하고, 각 프로세서마다 키를 할당하여 이진검색으로 최종 리스트 키의 위치
를 결정한다.

17. 3,629] 외판원 문제를 푸는 PRAM 알고리즘을 작성하시오. 작성한 알고리즘의 성능을 외판
원 알고리즘(알고리즘 8.1과 비교하시오.

fl


===== PAGE 543 =====
appendix  A

Ou Oz 표시된 부분을 제외하고는 이 책의 BES 이해하기 위해서 깊은 수학적인
기초지식이 필요하지는 않다. 특히 미ㆍ적분학에 대한 지식은 더욱이 필요 없다. 그러나
알고리즘 분석을 위해서 어느 정도의 수학이 필요한 것은 사실이다. 이 부록에서는 알고
리즘 분석에 필요한 수학을 복습한다. 아마도 독자는 여기서 나오는 내용의 대부분 또는

모두를 이미 알고 있을 수도 있다.

@ Al 표기법

때로는 실수 보다 크거나 같은 가장 작은 BES 나타낼 필요가 있다. 그 ASS [ele
표시한다. 예를 들면

[3.3]=4  /ol=s   [61=6

[-3.3]=-3 [-3.7]=-3 [-6|]=—6

[71는 2의 SARcoiling)e 한다. 모든 정수 nol] 대해서 [n]= noc}, 또한 때로는 실
수 #보다 작거나 같은 가장 큰 정수를 나타낼 필요도 있다. 그 정수를 |2|로 표시한다.
예를 들면

18.3|=8   히=4    16|=6

|-3.3]=-4 |-3.7]=-4 |-6]=-6

Le |= 2 의 내림수(1002)라 한다. 모든 정수 no] 대해서 [2 ]=7ㅠ이다.
결과의 근사치만 구할 수 있는 경우, “근사하게 같다"는 의미를 가진 ~ 기호를 사용한


===== PAGE 544 =====
534

appendix A 수학

다. 원의 면적과 둘레를 계산하는데 AL 많이 본 숫자 PIS 예로 들어보자. Pr 값은
개의 10진수로는 표현할 수 없다. 왜냐하면, 영원히 계속 소수점 이하 숫자를 만들어:
수 있기 WELO]CH + = 0,3333333 …과 같이 어떤 패턴이 있는 것도 아니다). Pro} 처음
6 숫자는 3.14159이므로, 다음과 같이 표현할 수 있다.
nm = 3.14159
= 기호는 "같지 않다"를 의미한다. 예를 들어, 변수 x9} y 2] 값이 같지 않음을 나타
내고 싶으면, 다음과 같이 쓴다.

Le UY
비슷한 BS 더하는 경우를 생각해보자. 항의 개수가 그리 많지 않다면 간단히 표현할
수 있다. 예를 들어, 양의  정수에서 처음 TNS 더하는 경우 다음과 같이 쓰면 된다.
12709 47000 7

또한 양의 정수에서 처음 7개의 제곱을 더하는 경우 다음과 같이 쓰면 된다.
1? +2? +37? +4? +57 +67 +77
이러한 표기법은 항의 개수가 그리 많지 않을 때 별 문제가 없다. 그러나 예를 들어 양의
쓰는

정수에서 처음 100개를 더하는 경우 이 표기법을 쓰는 건 별로 바람직하지 않다. 한 가지
방법으로 다음과 같이 처음 몇 개의 항을 쓴 후 일반항을 쓰고, 그 다음 마지막 항을 쓰면

1+2+…+?2+…+ 100
또한 양의 정수에서 처음 100개의 AS 더하는 경우 다음과 같이 쓰면 된다.
10 20 4-47? +--+ 1003

맨 앞에 나오는 몇 개의 항으로 일반항을 쉽게 유추해낼 수 있는 경우도 때로는 있는데,
그러한 경우에는 일반항을 굳이 쓸 필요는 없다. 예를 들어, 처음 100개 양의 정수의 합

1+2+…+100
항 몇 개를 보여주어서 도움이 되는 경우 그 항을 쓰면 된다. 그러나 Ate sigma)
발음하는 그리스 문자 US 사용하여 더 간단히 표현할 수도 있다. 예를 들어, 양의 정수
에서 처음 100개의 합은 SS 사용하여 다음과 같이 BA 수 있다. ㆍ



===== PAGE 545 =====
@0000000
A2 함수 535

이 표기법은 변수 1 1부터 100까지 취해서 그 값을 더한다는 것을 의미한다. 비슷하게
양의 정수에서 처음 100개의 제곱의 합은 다음과 같이 표현한다.
100

270

합의 마지막 정수가 임의의 수 /이어야 할 경우가 종종 있다. 방금 배운 표기법을 사용하
면 처음 7/개의 양의 정수의 합은 다음과 같이 표현할 수 있다.
100

1+20+…+?7+…-+7 또는 Wi
t=1

비슷하게 처음 7 양의 정수의 제곱의 합은 다음과 같이 표현할 수 있다.
100

VHP tet Ptetn? ER YS?

t= 1

=(1)+(1+2)+(1+24+3)4+(1+24+3+44) = 20

비슷한 형태로 합의 합의 합, 그리고 그 이상도 표현할 수 있다.
마지막으로 어떤 실수보다도 큰 수를 나타낼 필요가 종종 있다. 이를 무한대00800)
라고 하며, ㅇ 로 표시한다. 모든 실수 <에 대해서 다음 부등식이 성립한다.

Des CO

단히 보면, 단일 변수 함수(6100400) /는 변수 oS 유일한 값 /(2)와 연관 짓는 규칙
|이다. 예를 들어, 주어진 실수 #와 그 실수의 제곱과 연관 짓는 함수 /는 다음

fa)=2
함수는 순서쌍(60600 pair) 집합으로 나타낼 수 있다. 예를 들어, 함수 f(x) He?
모든 순서쌍 (2, 2”)을 나타낸다. 함수의 그래프(@8204)는 그 함수로 구하는 모든 순서

쌍의 집합이다. 함수 fle) = 22] 그래프는 그림 Ars} 같다.
다음 함수는 × 0일 때만 정의된다.


===== PAGE 546 =====
536

appendix A 수학

>

1 | ㅣ ㅣ ㅣ

| _._+ (2, 4)

-NWOFATAHDN WO O

eg OS ea

<>

03
be

ABA 함수 f(x) =272) 그래프, 순서쌍 (2.4)S 표시해놓았다.

함수의 변역(000800/은 함수를 정의하는 값의 집합이다. oS 들면, /(2) = 1/2의 변역
은 0을 제외한 모든 실수가 되는 반면, fle) = a2] 변역은 모든 실수가 된다
다음 함수는 음수 아닌 Wek 가진다.

f@)=2

여기서 “음수 아닌 값”이란 0보다 크거나 같은 값을 의미하고, “양수 값"이란 0보다 엄밀
히 큰 값을 의미한다. 함수의 AA (range)-& 함수가 가지는 값의 집합이다. f(w) = 279]
치역은 음이 아닌 ASI} 되고, f(x) = 1/#의 치역은 OF 제외한 모든 실수가 되고,

f(x) = (1/2)^의 치역은 모든 양의 실수가 된다. 함수는 변역에서 치역으로 간다라고 말
한다. ofS 들면, 함수 /(#)=^은 실수에서 음이 아닌 실수로 간다.

@ AZ 수학적 귀납법

어떤 합산은 일반형으로 표현할 수 있다. 예를 들어, 다음 등식을 보자.

n(n+1)
2

이 등식이 성립하는지를 보기 위해서 몇 개의 7에 대해서 검산해보자.

1+2+…+7=

4(4+1)

14+2+3+4=10=—>



===== PAGE 547 =====
ieee

그러나 양수인 정수의 개수는 무한하기 때문에 개별적으로 각 nol 대해서 일일이 검사해
서는 모든 양의 정수 nol] 대해서 이 등식이 성립하는지 결코 확신할 수 없다. 개별적으로
검사하게 되면 그 값에 대한 등식이 성립한다는 A 보여줄 뿐이다. 모든 양의 정수 nol]
대해서 등식이 성립함을 보여줄 수 있는 강력한 방법이 수학적 AA (mathematical 10ㅁ-
duction) ©] TH,
수학적 귀납법은 도미노 원칙(400ㅁ100 principle)y} 같은 방법으로 작동한다. 그림 A2

가 이 원리를 보여 주는데, 만약 두 도미노 사이의 거리가 도미노의 높이보다 항상 작다
면 첫째 도미노만 넘어뜨리면 모든 도미노를 넘어뜨릴 수 있다. 이게 가능한 이유는 다음
과 같이 요약할 수 있다.

1 첫째 도미노를 넘어뜨린다.

2, 두 도미노 사이의 거리가 도미노의 높이보다 작게 모든 도미노를 세우면, nA 도

미노가 넘어지면, (/+1)째 도미노도 넘어진다고 보장할 수 있다.

첫째 도미노를 넘어뜨리면, 그것은 둘째 도미노를 넘어뜨리고, 둘째 도미노는 셋째 도
미노를, 이런 식으로 계속 될 것이다. 이론적으로 임의의 아무리 많은 수의 도미노를 세
우더라도 모두 넘어진다고 할 수 있다.

귀납법에 의한 증명도 도미노 원리와 같은 방법으로 이루어진다. 먼저 7=1일 때 우
리가 증명하려고 하는 것이 사실임을 먼저 보인다. 다음, 임의의 양의 정수 에 대해서
사실이라면 7+ 1일 때도 반드시 사실임을 보여야 한다. 일단 이게 사실임이 밝혀지면
= 1일 때 사실이므로 7= 3일 때도 사실임에 틀림없고, n=29 때 사실이므로 7= 3
일 때도 사실임에 틀림없고, 계속 이와 같은 방식으로 무한히 계속 이야기할 수 있다.
따라서 모든 양의 정수 nol] 대해서 사실이라고 SEAS 수 있다. 양의 정수에 관한 어떤
문장이 사실임을 귀납법으로 증명할 때 다음 SS 사용한다.

그림 &.2 첫째 도미노가 넘어지면, 나머지도 모두 넘어진다.


===== PAGE 548 =====
@0000000
538   appendix A 수학

 귀납기초(ㅁ040110ㅁ base) : n= 1(또는 다른 초기값)에 대해서 그 문장이 사실이라
는 중명이다.

© 귀납가정(10040[10ㅁ hypothesis) ： 71 = 1(또는 다른 초기값)인 임의의 7에 대해서
그 문장이 사실이라는 가정이다.

 귀납단계(10040[10ㅁ step) : 만약 문장이 nol] 대해서 사실이라면, n+ 19] 대해서도
반드시 사실이어야 한다는 증명이다.

귀납기초는 결국 첫째 도미노를 쓰러뜨리는 것에 해당하고, 귀남절차는 만약 na 도
미노가 넘어지면, (+ 1)째 도미노도 넘어진다는 것에 해당한다.

*예제 441 = BE 양의 정수 nol] 대해서 다음 등식이 성립함을 보인다.

으라 분

귀납기초 : n=10] 대해서, 1= Bt)

귀납가정 : 임의의 양의 정수 nol 대해서 다음 등식이 성립한다고 가정한다.

n(n+1)
2

1+2+…+7=

귀납단계 :
(n+1)[(n+1) +1]

1+2+--+(n+1)=      5

위의 등식이 성립함을 보이면 된다.
1+2+…+(072+ 1) =14+2+-+ntn4+1

- n(n+1)

8

_ n(n+1)+2(n+1)
2

_ (n+1)(n+2)

7     2

_ (n+ D[(nt+1) +1)
2

ai apd

귀납법으로 증명할 때 귀남절차에서 귀납가정과 같은 항들은 진한 활자체로 구별해
놓는다. 귀납가정이 적용되고 있다는 걸 강조하기 위함이다. 귀납절차에서 무엇이 이루
어지는지 살펴보자. 귀납가정이 다음과 같다고 가정하고,

n(n+1)
2

대수적인 조작을 거쳐서 다음과 같은 결론에 도달한다.

1+24+--+n=



===== PAGE 549 =====
© 예제 4.2

0000000
A3 수학적 귀납법    539

(n+1)[(n+1)4+1]
9

eee ee) =

그러므로 nol] 대한 가정이 사실이면 n+ 19] 대해서도 반드시 사실이다. 귀납기초에서
n=19 때 사실임을 보였기 때문에 도미노 원칙에 의해서 모든 양의 정수에 대해서도
사실이라고 결론지을 수 있다.

왜 예제 ㅅ.1의 등식이 사실이라고 애초에 생각하게 되었는지 궁금할지도 모른다. 이
은 아주 중요하다. 몇몇 사례를 조사하고 현명한 추측을 통해서 사실일 가능성이 있는
HS 얻어낼 수 있다. 예제 ㅅ.1에 있는 등식도 원래 이런 식으로 찾아내었다. 그러고는
PHS 사용하여 그 문장이 사실임을 USS 수 있다. 물론 사실이 아니라면 귀납법
명이 실패할 것이다. 귀납법이 AMIS 문장을 만들어내는 BAS 아니라는 A 알아야
한다. 귀납법은 사실일 가능성이 있는 문장이 있는 경우에 이를 증명할 때만 제 FS
한다. 8.5.4절에서 사실인 문장을 찾아내도록 도와주는 직관적 ADH (constructive 1ㅁ-
0401000)에 대해서 공부한다.

또 하나의 중요한 AS 초기값이 7=1일 필요가 없다는 사실이다. 즉, 7 > 10인 모
는 nF] 대해서만 문장이 사실일 수도 있다는 것이다. 이때 귀납기초는 n= 10이다. 경우
에 따라서 귀납출발점이 n = 0이 되기도 한다. 분명히 모든 So] 아닌 Aol 대해서 증
명하는 경우일 것이다.

귀납법을 이용한 증명 AS 더 살펴보자.

에 이 그 Ad oy

c

BE 양의 정수 7에 대해서 다음 등식이 성립함을 보인다.

a a = 2

1(n+1)[(2«1) +1]
6

귀납가정 : 임의의 양의 정수 7에 대해서 다음 등식이 성립한다고 가정한다.

귀납기초 : n=19] 대해서 12 =1=

ah, Soe - n(n+1)(2n+1)
6

귀납단계 :

(n+1)[(n+1) +1][2(n+1) +1]

+2? 4+---+(n+1)? =            ;

위의 등식이 성립함을 보이면 된다.
10 +20+…+(06+ㅜ1)? =P 424-4024 (n+1)
6

_ n(n+1)(2n+1)+6(n+1)?
6

+(n+1)?



===== PAGE 550 =====
@9@ee7ee# ee
540   appendix A 수학

© 예제 AS

© 예제 4.4

_ (n+1)(2n?+n+6n+6)

_ iT toed)

_ 00609

= int)

다음 예제에서 AZ n=0.

음이 아닌 모든 정수 no] 대해서 다음 등식이 성립함을 보인다.

29421497? 4...49" =grti—y
시그마로 SAS 다음과 같이 표기할 수 있다.

pa  = 2071

귀납기조 : =0에 대해서, = 1 =-20+ㄴ-ㄱ
귀납가정 : 임의의 음이 아닌 정수 7에 대해서 다음 등식이 성립한다고 가정한다.

Se ee ee 00 = 00701
귀납단계 :

20+20+22+.…+ 0071 = 20701 1
위의 등식이 성립함을 보이면 된다.
2° +2242? 4..-49"71 =o 4at4o24...4974¢9"F1

=, grt —14 27+!

= 300" ') |
ah gint+I +1 =

예제 ASS 다음 예제에서 얻는 결과의 특수한 경우이다.

모든 음이 아닌 정수 nz} 10] 아닌 실수 rol 대해서 다음 등식이 성립함을 보인다.

위의 항을 기하 수열(6600660010ㅇ progression)°]2} 한다.

0+1 _
귀납기초 : ㅠ=0에 대해서 19 =1=——

귀납가정 : 음이 아닌 임의의 정수 7에 대해서 다음 등식이 성립한다고 가정한다.



===== PAGE 551 =====
귀납단계 :

541

귀납법을 이용하여 얻을 수 있는 결과들은 때로는 다른 방법을 통해서 더 쉽게 입증할

수도 있다. 예를 들어, 위의 보기에서 다음 등식을 증명했다.

"2 “~ |

n
yi
2= 0

… |.

귀납법을 이용하는 대신 오른쪽 등식의 분포를 왼쪽 식에 곱하여 다음과 같이 간략화 할

수있다

aid

itt

= … ee rae ee

a
=,” |

이 등식의 양변을 7-ㅡ1로 나누면 원하는 결과를 얻는다.
귀납범의 예제를 하나만 더 보자.

*예제 4.5 BE 양의 정수 nol 대해서 다음 등식이 성립함을 보인다.
Siz =( n—1)2"*1+2

귀납기초 : n=109] Tay 1x2! =2=(1-1)2'71+2
귀납가정 : 임의의 양의 정수 nol] 대해서 다음 등식이 성립한다고 가정한다.

Sia! =(n—1)2"*1 +2

t=1


===== PAGE 552 =====
@0@00000 0
542   appendix A 수학

귀납단계 :
ye  =([(nt1)-1Ja"*V*1 +49

위의 등식이 성립함을 보이면 된다.
n+l
pe

n
210+( (2+1)0"11
수

= (n—1)2"t1424+(n4+1)2"*!
= 902" +
=[(2+1)-1]287+140+14. 9

귀납가정을 설정하는 또 다른 방법은 초기값보다 크거나 같고 보다는 작은 모든 *에
대하여 문장이 사실이라 가정하고, 귀납절차에서는 nol 대하여 사실임을 증명한다. 이

방법은 1.8.9절의 정리 1.1의 증명에 사용한다.
이 절에서 본 보기들은 모두 합에 대한 일반식을 구하는 것에 고

관한 것이지만, 귀납법을

응용할 수 있는 다른 사례는 얼마든지 있다. 이 책에서 많이 마주치게 될 것이다.

@ A4 Azo} 보조정리

사전에 보면 Qe|(theorem)= 무엇인가를 증명해야 할 명제라고 정의한다. 수학에서도
같은 의미를 지닌다. 앞 절에서 본 사례들은 각각 정리라고 얘기할 수 있고, 귀납법으로
정리를 증명하였다. AS 들어, 예제 ALS 다음과 같이 기술할 수 있다.

> 정리 Ast

> 0인 모든 정수 7에 대해서 다음 등식이 성립한다.

1+8+…+ㅠ=끄빼브
증명 : 여기에 SIO] 와야 한다. 이 경우 예제 ㅅ.1에서 사용한 귀납법 증명이 여기에 오면
된다.
정리를 기술하고 증명하는 이유는 다른 사례에 두루 쓰기 위한 일반적인 결과를 얻기

위한 것이다. 예를 들면, 정리 Ar 이용하여 어떤 양의 정수 에 대해서도 /,까지의

합을 바로 계산할 수 있다.

학생들은 필요조건('ㅠ")이 있는 정리와 필요충분조건(ㅠ and only if’)o] 있는 정리의
차이점을 잘 이해하지 못하는 경우가 종종 있다. 다음의 두 정리가 차이점을 보여준다.



===== PAGE 553 =====
@00@000000
^&.5 대수 543

> Bel A.2
BE 실수 2에 대해서 Sn  x” > 0이다.
증명 : 두 양수의 곱은 양수라는 사실에 의해서 이 Bele 성립한다.

정리 A.20]] 기술된 문장의 A(reverse 102010811020)은 사실이 아니다. 즉, “2” > 0이면,
a> 0이다"는 AMI] 아니다. 예를 들면, 다음 부등식은 성립하고,
(-3)?=9>0
32 0보다 크지 않다. 실제로 어떤 음수의 제곱은 0보다 크다. 그러므로 정리 4.2는 필
SAAC) 문의 보기이다. 역도 사실이라면 그 정리는 필요충분조건(800 only if’)
문이 되고, 정07001108400)과 역을 모두 증명할 필요가 있다. 다음 정리는 필요충분조건
물의 보기이다.

> Bez] 4.3
“모든 실수 rol] 대해서 2> 0”는 “1/2 > 0"”의 필        건이다.

요충분조
증명 : AS 증명한다. o> 0이라고 하자. 그러면, 다음 부등식

성립한다.

rlo

6
x

왜냐하면 두 양수의 HS 0보다 크기 때문이다. 역을 증명한다. 1/7> 0이라고 하자. 그러면

으으으

1/a
이 된다. 왜냐하면 똑같이 두 양수의 RS 0보다 크기 때문이다.

사전에서는 보조정리160008;를 다른 명제를 증명하기 위해 사용되는 보조적인 명제로
정의한다. 정리와 마찬가지로 보조정리도 무언가를 증명하여 보여주는 명제이다. 그러나
보통 보조정리 안에 있는 명제들은 그 자체로서는 별로 가치가 없고, 오히려 Belo] 증명
이 하나 이상의 보조적인 명제의 사실 여부에 의존할 때 이러한 명제에 관한 보조정리를
기술하고 증명한다. 그리고는 그 보조명제를 이용하여 정리를 증명한다.

@ AS 대수

대수008800000는 알고리즘 분석에서 가장 많이 사용되는 수학 도구 중 하나이다. 대수
의 BAS 간단히 복슴한다.


===== PAGE 554 =====
@00@000000
544   appendix A 수학

* 예제 AG

© 예제 47

A5.1 대수의 정의와 특성
어떤 수 2 의 상용대수(600ㅁ0000 logarithm)+ log 로 표시하며, 2가 102] 몇 승(00\60)

이 되는지를 나타낸다.

상용대수의 예를 몇 개만 살펴보면 다음과 같다.

10810 =1              왜냐하면       10' = 10
log10,000 = 4         왜냐하면       10* = 10,000

3
log0.001 =— 3         왜냐하면        0 ~ Fa   =0.001
logl =0                왜냐하면       10° =1.

09 아닌 수의 0승은 1임을 기억하라.

일반적으로 어떤 수 <의 대수는 2가 또 다른 수 0의 몇 승이 되는지를 나타낸다. at
1을 제외한 모든 양수가 될 수 있으며, 밑수(6880)라고 한다. 반면에 et 반드시 양수이
어야 한다. 즉, 음수나 0의 대수란 건 없다. 기호로는 108, oH 쓴다.

log, 2] 예를 몇 개만 살펴보면 다음과 같다.

10878 =3                 왜냐하면        208
log,81 = 4                왜냐하면        3°=81

—                  ;            의 [나 그
10827 ~ 2.807         왜냐하면       a ee

예제 &.7의 마지막 예는 밑수의 거듭제곱(60\62이 딱 떨어지지 않는 경우이다. 밑수
의 거듭제곱이 딱 떨어지는 경우뿐만 아니라 모든 양수에 대수가 존재한다. 밑수의 거듭
제곱이 팍 떨어지지 않는 경우 대수의 의미에 대해서는 이 책의 범위에 벗어나므로 다루
지 않는다. 단지 여기서는 대수가 증가함수라는 사실만 밝혀둔다. 즉,

2<4이면, 1068』 x < log, y
따라서
2= log,4 < 10827 < 10828 = 3

위의 예제 &.7에서 본 대로 10827의 값은 약 2.807이니까 2와 3 사이에 들어간다.
알고리즘 분석에 많이 쓰이는 대수의 몇몇 중요한 특성을 나열해 보면 다음과 같다.

대수의 주요 특성 (모든 경우에 a>1, 0>1, 때> 0, y>0)



===== PAGE 555 =====
@0@00600000
AS 대수 545

1, log,1=0
2. 1960 =,

3. log, (zy) = log, «+ log, y
x
4,  0, 108.2-108.0

5. log, x’ =y log, x

10  log,
6. x 80 = 86

log, x

7, log, t=  00

*예제 4.8 위의 특성이 적용되는 예를 몇 개만 살펴보면 다음과 같다.

log,
ge =8                                                     (특성 2)
log, (4 x 8) =log,4+log,8 =2+3=5            (특성 3)
logy a= log,27 —log,9 =3-—2=1                            특성 4)
10874“ =3108.,4=3×2 = 6                                    (특성 5)
glext = gies = 43 =64                                (특성  6)
log,l6 4
=             =                                       BA
log,16     월                                       (S43 7)
_ logl28 2.10721 _                  —
1062128 = Too ~ 0.30103"                       (특성 7)
1           1.82607
1068.67 = oes          ~ 3.82728               (특성 ?)

1683 0.47712

과학용 계산기는 log 함수를 가지고 있기 때문에(여기서 log 108,,을 뜻한다) 예제
A.89] 마지막 8개의 예는 임의의 밑수를 가진 대수를 계산기를 통해서 어떻게 계산하는
지를 설명한다(여기의 결과도 실제로 계산기를 가지고 계산하였다).

알고리즘 분석에서는 믿수가 291 GES 많이 쓰기 때문에 따로 간단한 기호를 사용한
다. 즉, log, 는 182 로 나타낸다. 지금부터는 이 기호를 사용한다.

A.5.2 자연대수

6로 표시하며 약 2.7182818284859의 값을 가지는 수를 기억할 것이다. 와 마찬가지로
는 유한개의 소수로는 정확한 표현이 불가능하다. 사실 이 수는 소수점 아래에서 반복
는 부분마저도 없다. log. cS 1ㅁ2 로 표시하고 의 자연대수(ㅁ8[4781 logarithms) =}
한다. 예를 들면

^

KI


===== PAGE 556 =====
546

appendix A 수학

Inl0 ~ 2.3025851

이 답을 어디서 얻었는지 의아해 할지도 모른다. 단순히 In 함수 기능을 가진 ARV IS
사용했을 뿐이다. 미적분학(681011408)을 공부하지 않고 자연대수를 어떻게 계산하고 왜
"자연"이라 하는지 이해하기 힘들다. 6만 봐서는 자연대수는 상당히 부자연스러워 보인
다. 미적분학을 언급하는 것은 이 책의 현재 WAS 벗어나기는 하지만(@로 표시된 부
분은 제외), 알고리즘 분석에 중요한 자연대수의 특성 하나는 탐구해볼 필요가 있다. 대
학수학 지식으로 1 ce 1과 2 사이에 있는 1/2곡선 아래 부분의 면적임을 알 수 있다.
2ㅁ= 5일 때 이것은 그림 A392] 위 그래프와 같다. 이 그림의 아래 그래프에서는 각 단위
너비별 사각형의 면적을 합해서 전체 면적의 근사값을 어떻게 구하는지를 보여준다. 이
그래프를 보면 105의 근사값은 다음과 같이 구할 수 있음을 알 수 있다.

1     2     3     4     5

그림 &.3 위 그래프에서 음영 처리된 부분은 145이다. 아래 그래프에서 O1G7i] 칠해진 사각형의
AAS 합하면 Indo] 근사한다.



===== PAGE 557 =====
@0000000
^ㅅ6 집합 547

    [ x <]- 2.0833

4

여기서 구한 면적은 실제 면적에 비해서 항상 크다는 것을 알아두자. 계산기를 사용하면
다음과 같은 답을 얻는다.

Ind = 1.60944

여기서 구한 사각형들의 AAS Ind 의 정확한 PARES 아니다. 그러나 마지막 사각형(2
Zt 4와 5 사이에 있는 AS 보면, 그 면적은 7= 4와 = 5 사이 곡선 아래의 실제 면적
과 큰 차이가 없다. 그러나 첫째 사각형의 경우는 그렇지 않다. 연속적으로 나열되어 있
는 사각형은 각각 바로 왼쪽에 이웃해 있는 사각형보다 더 정확한 근사값을 가진다. 그러
므로 그 수가 작지 않으면, 사각형들의 면적의 합은 자연대수의 값에 가까워진다. 이 결
과는 다음 예제와 같이 사용된다.

* 예제 AQ 다음 식을 계산하고 싶다고 하자.
iL       1

gto
2

이 합은 일반항(10600 form) © 나타낼 수 없다. 그러나 앞에서 이야기 한 대로 만약 no] 작지
않다면 다음과 같이 된다.

0×10+|1×극]+ 때 +(1   2

1

5}         Jenn

n—
no] 작지 않으면 1/7의 값은 그 합과 비교해서 무시할 수 있을 만큼 작다. 따라서 이 BS 추가
해도 다음과 같은 결과를 얻을 수 있다.

oe ee
2     n

이 결과는 알고리즘을 분석할 때 쓴다. 일반적으로 다음 부등식을 증명할 수 있다.
1

ㅣ         1
이. alee ~<Inn<1+54+- 고 = 고

@ ㅅ.6 집합
약식으로 정의하면 집합(660은 물체의 모음이다. 집합은 보통 $9} 같이 대문자로 표시
하고, 집합에 속한 모든 물체를 열거할 때에는 중괄호로 에워싼다. 예를 들면, 다음은 첫
자연수 4개를 모은 집합이다.

911 2,3, 새


===== PAGE 558 =====
548

appendix A 수학

BAS 나열하는 순서는 관계가 없다. S 다음 두 집합은 같으며, 똑같이 첫 자연수 4개
의 집합을 나타낸다.
(1, 2, 8.4}와 13. 1, 4 2}
집합의 예를 또 하나 살펴보자.
S= {Wed, Sat, Tues, Sun, Thurs, Mon, Fri}
이것은 요일의 집합이다. 집합이 무한한 경우 그 집합에 속하는 물체의 성질로 그 집합을
표현하기도 한다. 예를 들어, 3의 배수인 양정수의 집합은 다음과 같이 표현할 수 있다.
S= {a io] 대해서 7= 317} 성립하는 n}
또는 다음과 같이 일부 항목과 일반항만 가지고 집합을 표현할 수도 있다.

집합 안에 있는 BAS 집합의 원소(6860601) 또는 멤버(0ㅁ622060)라고 한다. 만약 가
집합 So 원소이면 2 © SH 쓰고, 2가 집합 6의 원소가 아니면 2 Sz 쓴다. 예를
들어,

= 11, 2, 3, 4} 이면, 2 So) 5 = Solr},

만약 같지 않으면 = TS 쓴다. 예를 들어,

S={1, 2, 3, 4} 이고 T= {2, 1, 4, 3 } 이면, S= 4이다.

어떤 집합 So] 속하는 모든 원소가 다른 집합 THE 속하면 SE 7'의 BEAM osub-
860이라 하고, SC TH 쓴다. aS 들어,

S={1, 3, 5} 이고 T= 11, 2, 3, 5, 6} 이면, SS 2이다.

모든 집합은 자신의 부분집합이다. 즉, 어떤 집합 Sol] 대하여 Sc 6'이다. 9가 7의 부
분집합이고 7와 같지 않으면, 는 TS] 진부분집합(00206 subset)°]e} 하고, SC TH

쓴다. 예를 들어,
S={1, 3, 6} 이고 72- { 1, 2, 8, 5, 6} 이면, Se 이다.

두 집합 와 7가 있을 때, SL} T2] 교집합(216060001020)은 S2} To] 공통으로 있는
는 원소의 집합으로 정의하고, sn 2로 쓴다. 예를 늘어,

S=11, 4, 5, 6} 이고 2= 11. 8, 5 | 이며, 87 TH il. 5} 이다.

두 집합 SA 7`가 있을 때, 와 TS] 합집합022102)은 So] 있거나 To] 있는 모든 원소
의 집합으로 정의하고, SUTB 쓴다. 예를 들어,



===== PAGE 559 =====
S={(L 4 6. 6) 이고 T={1, 8. 8} 이면, 11 T=—41, 3, 4, 5, 6} 이다.

두 집합 와 7까 있을 때, St 7'의 AWWdifference)2 Sol] 있으나 7에는 없는
모든 원소의 집함으로 정의하고, oe 쓴다. 예를 들어,

S={1, 4, 5, 6}이고, T={1, 3, 5}이면,
S— T={4, 6}이고, T—S= {3} 이다.

공집합(6026 860)은 원소가 하나도 없는 집합으로 정의하고, o 로 표시한다. 예를 들어,
6= 11, 4 6)이고 = 10, 8, 5} 이면, FNP 0 이다.

AAA H(universal set) VE 고려 대상인 원소 전체의 집합으로 정의한다. SS 고려
중인 집합 중 하나라고 하면 SC (/이다. 예를 들어, 양의 정수로 된 집합을 고려한다면,
U=({1, 2, 3, =, i, --}

이다.

@ AT 순열과 조합
항아리 안에 A, 8, 0, DH 각각 표시된 공이 있다 하고, 2719] SS 항아리에서 끄집어
내려고 한다. 맞는 SS 순서에 맞게 Uo 복권에 당첨된다. 당첨 가능성을 알아보기
위해서 몇 가지 다른 결과가 나올 가능성이 있는지 알아봐야 한다. 가능한 결과는 다음과

os
AB AC AD
BA 80 BD
CA CB CD
DA DB DC

예를 들어, ABS} BAS 다른 결과로 취급하는데, 그 이유는 SS Be 순서가 있기 때문
이다. 위에 12714] 다른 결과를 나열하였다. 그러나 이것이 나올 수 있는 모든 결과인지
확신할 수 있는가? 여기서 4행과 3열로 AMS 정리하였음을 주목하자. 각 행마다 첫째
공을 다르게 선택하는데 그런 Bo] 4개 있다. 첫째 SS 선택한 후 각 행의 둘째 SS
남은 공 가운데 하나씩 선택하는데, 그런 선택이 3가지 있다. 따라서 나올 수 있는 결과
의 총 수는 다음과 같이 계산한다.

(4)(3) = 12

이 결과는 일반화 할 수 있다. 예를 들어, 4개의 공 가운데 3개를 뽑는다고 가정한다면,
첫째 공은 4개 중 어느 하나가 될 것이고, 일단 그 공을 꺼낸 후에 둘째 SS 남은 3개


===== PAGE 560 =====
550

appendix A 수학

중 하나가 될 것이고, 일단 둘째 FS 꺼낸 후에 셋째 공은 남은 oh 중 하나가 될 것이다.
따라서 결과의 총수는 다음과 같이 계산한다.

(4)(3)(2) = 24
일반적으로 nM] 공이 있고, 그 가운데 《개를 꺼낸다면 가능한 결과의 수는 다음과 같다.
inven 1)
이를 7개의 물체에서 한 번에 《개를 취하는 A (permutation) 2] 수라고 한다. 만약
/”=4이고 k= 3이라면, 이 식은 다음과 같은 결과를 준다.
(4)0(03)… (4-8+1)= (4)(3)(2) = 24

이 결과는 이미 앞에서 구하였다. 만약 7 = 10이고 *= 5라면, 이 식은 다음과 같은 결
준다.

a)
de

(10)(9) --- (10—5+1) = (10)(9)(8)(7)(6) = 30,240

만약 *=7이라면 BE 공을 꺼내는 경우가 된다. 이럴 때는 단순히 7개 물체의 순열의
수라고 한다. 이전 식에 의하면 이는 다음과 같다.

n(n—1)(n-—n-1)=

양정수 nol 대하여 7!은 그 수에다가 그보다 작은 모든 양의 정수를 곱하는 것으로 정의
되고, O19] 값은 1로 정의되며, 7!은 음수에 대해서는 정의되지 않음을 상

: 단순히 맞는 SES 선택함으로써 복권에 당첨될 수 있다고 생각해보자. 즉, 순서를 맞
요는 없다. 다시 4개의 공 가운데 두 개를 뽑았다고 가정해보자. 이 복권추첨의 결과
}각 이미 뽑은 2개의 공과 관련이 있다. 예를 들면, 이미 뽑은 결과인 Avs} BAY 이
권추첨의 규칙에 의하면 같다고 여길 수 있다. 따라서 우리는 이를 다음과 같이 한다.

AS} 8

이미 뽑은 9개의 공은 이 복권추첨 한 가지의 결과로 여기기 때문에 이미 추첨한 결과의
가지 수를 로 나누어 몇 가지 종류의 결과가 나오는 지를 구할 수 있다. 즉, 이 복권추첨
의 결과의 가지 수는 다음과 같다.

점  시   ni

J

여섯 가지의 서로 다른 결과는 다음과 같다.
AS} 8, 와 C, 와 D, 와 C, 와 D, 0와 2

이제 3개의 SS 뽑았고, SAS 맞출 필요가 없다고 가정해보자. 이 복권추첨의 규칙



===== PAGE 561 =====
@000600000
A7 순열과 조합  551

에 따르면 다음은 모두 같은 결과로 여긴다.
ABC ACB BAC BCA 0468 CBA

이 결과는 단순히 8712] 물체의 순열일 뿐이다. 이러한 순열의 값은 3!= 6임을 상기하

자. 이 복권추첨에서 몇 가지 서로 다른 결과가 존재하는지 결정하기 위해서 뽑는 순서를

따지는 복권추첨의 서로 다른 결과의 가지 수를 312 나눌 필요가 있다. 즉, 이 복권추첨

의 결과의 가지 수는 다음과 같다.

AS} BS} C, 와 BS} D, 와 0와 D, BS} C2} 2
일반적으로, 7개의 공이 있고, 《개의 공을 뽑고, SAS 상관하지 않는다면, 서로 다
른 결과의 가지 수는 다음과 같다.

(n)(n—1)-+ (n—k+1)
시

이를 7개의 물체에서 한 번에 《개를 뽑는 조합(66ㅁ0108400/의 수라고 한다. 위의 식에
서 분자는 다음과 같이 되기 때문에,

개의 물체에서 한 번에 《개를 뽑는 조합의 HS 구하는 공식은 보통 다음과 같이 쓴다.

n!
ki(n—k)!
이 SAS 사용하면 8개의 물체에서 한 번에 3개를 뽑는 조합의 AL 다음과 같이 계산할
수 있다.
sho
318-3) °°

대수학 책에서 배운 ©]4}9 2] (Binomial theorem)= 다음과 같다. WE Lo] 아닌 정수
ni} 실수 0와 bol] 대해서

=  는    n!    kgn—k
(a+b)  oP; 기 810 b


===== PAGE 562 =====
@00@000000
552   appendix A 수학

© 예제 A.10

/개의 물체에서 한 번에 《개를 뽑는 조합의 수가 이 식에서는 ako" “의 계수이기 때문
에 이 수를 이항계수0010ㅁ00181 0061110600라 하고, =  로 쓴다.

개의 항목을 가진 집함의 부분집합의 개수(공집합도 BA" AS 보이자. O< k= nl 때
A717} ke 부분집함의 개수는 개의 물체에서 한 번에 *개를 뽑는 조합의 수인 (7) 7b 된다.
즉, 부분집합의 총 개수는

sialic.   n —on

a)  Hae 1     (1+1)"=2

뒤에서 두 번째 SAS 이항정리에 의해서 성립한다.

@ As 확률

© 예제 A11

ae 공을 꺼낸다든지, 카드 한 벌에서 맨 위 카드를 뽑는다든지, SAS 던지는

우에 확률이론을 많이 사용한다. SS 꺼내고, 카드를 뽑고, SAS 던지는 VHS 실
니아 한다. 일반적으로 기술 가능한 HA] 결과들의 집합으로 이루어
진 실험에 확률이론을 적용할 수 있다. 가능한 모든 결과의 ee HEY ZHsample
space) 또는 BAt(population)]2}31 한다. 사회과학자들은 주로 "모집단"이라고 하는
반면에(사람에 관하여 연구하기 때문에), 수학자들은 주본공간" 이라고 한다. 여기서 우
리는 이 두 용어를 섞어서 쓴다. 표본공간의 부분집합은 사건(67604이라고 한다. 단지
하나의 원소만 가지는 부분집합은 원소사건(616060181” 6ㅇ604이라고 한다.

카드 한 벌에서 카드를 뽑는 실험에서 표본공간은 5장의 카드로 이루어진다. 다음 집합은 사건

이고,
9=|하트의 킹, 클럽의 A, 스페이드의 킹, 다이아몬드의 4
다음 집합은 원소사건이다.
2=|하트의 킹|
본공간에는 59개의 원소사건이 있다.

사건(부분집합)의 의미는 “부분집합에 있는 WAS 중 하나가 ABS] 결과"라는 것이
다. 예제 &.에서 사건 의 의미는 “뽑은 카드는 네 개의 킹 중에 하나"라는 것이고, 원
소사건 &의 의미는 "뽑은 카드는 하트의 킹"이라는 것이다.

주어진 사건이 실험결과를 포함하고 있을 확실성을 실수로 표현하며, 사건이 일어날
확률이라고 한다. 다음은 표본공간이 유한할 때 확률의 일반적인 정의이다.



===== PAGE 563 =====
*ㅇ예제 4.12

* 예제 A13

‥6060000 0
A8 확률 553

정의
개의 서로 다른 결과를 가진 다음과 같은 표본공간이 있다고 하자.

Zt 사건 에 실수 p(S) 를 지정하는 함수는
1100)라고 한다.
1. 1<i<nOll 대해서 0 < ple;) <1
2.  ple,) +p(e,) +-+-+p(e,) =1
3. 원소사건이 아닌 각 사건 에 대해서 p(S)=E 결과가 .5에 속하는 원소사건들의 확률의
합이다. 예를 들어, S={e,, eg, 6ㅇ;} 이면,
p(S) =p(e,) +p(e,) +p(ez)

함수 가 포함된 표본공간을 SSS7Kprobability 50806)이라고

다.

SS 집합의 함수로 정의하기 때문에 원소사건의 확률을 가리킬 때는 2(6,) 대신에
2(16, } )로 써야 한다. 그러나 혼돈 방지를 위해서 그렇게 하지 않는다. 같은 맥락에서
원소가 아닌 사건의 확률을 가리킬 때도 중괄호를 사용하지 않는다. 예를 들면, 사건
{e1, 68, 67} 의 확률은 2(61, eg, 607)로 쓴다.

어떤 결과에 대해서 그 결과가 포함되어 있는 원소사건과 연관 지을 수 있고, 따라서
그 결과의 확률에 대해서 말할 수 있다. 이는 그 결과가 포함된 원소사건의 확률을 뜻한다.

SHES 지정하는 가장 간단한 방법은 중립 AAl(principle of indifference)-& 사용하는
것이다. 이 원칙은 어떤 한 결과를 다른 결과보다 특별히 기대를 많이 한다거나 선호한다
거나 하지 않으면 각 결과는 같은 정도의 확률을 가진다고 여기는 원칙이다. 이 원칙에
따르면 개의 서로 다른 결과가 있을 때 각각의 확률은 1/7이 된다.

항아리에 A,B C, 로 표시된 4개의 공이 들어 있고, 그 중에서 하나의 SS 꺼내는 실험을 한다
고 가정하자. 표본공간은 {A BC, 마이고 중립 원칙을 따르면 다음과 같다.

p(A) =p(B) =p(C) =p(D) =+
사건 {A, 파는 공 AU, S BS 꺼냈음을 뜻한다. 그 확률은 다음과 같다.

p(A, B) =p(A) +p(B) = 4+

= 불
4    2

mle

한 벌의 카드에서 맨 위에 있는 카드를 뽑는 TIS 한다고 가정하자. 총 52g] 카드가 있으므
로, 중립 원칙을 따르면 각 카드가 뽑힐 확률은 ㅡ이다. 예를 들면,


===== PAGE 564 =====
@00@000000
554    appendix A 수학

© 예제 A.14

다음의 사건은 뽑은 카드가 킹임을 뜻한다.
6@={하트의 킹, SA] 킹, 스페이드의 킹, 다이아몬드의 4}
그 확률은 다음과 같다.
p(S) =7(하트의 킹) + 7(클럽의 킹) + 7(스페이드의 킹) + #(다이아몬드의 킹)
1   1   1   1   1

~ 52° 52 52° 52 13

앞 절에서 공부한 순열과 조합을 구하는 SAS 가지고 확률을 계산할 수 있는 경우도
있다. 다음 예제를 보자.

항아리에 A, 8, C, D, ES 표시된 5개의 공이 들어 있고, 꺼내는 SAME 상관없이 그 중에서
8개의 SS 꺼내는 실험을 한다고 가정하자. 7/(ㅅ와 BE} 를 계산하면 된다. 여기서 “Ast Bo}
@는 공 4, 8, CS 임의의 순서로 꺼낸 결과를 뜻함을 상기하라. 중립 원칙을 사용하여 확률을
결정하기 위해서 서로 다른 결과의 가지 수를 계산할 필요가 있다. 즉, 5개의 물체에서 한 번에
3개를 뽑는 조합의 수가 필요하다. 앞절의 SAS 사용하면 그 FE 다음과 같다.
5!
가"

그러므로 중립 Alo} 의해서 다음의 결과를 얻으며,
p(AS} BS} 0= 습
다른 9가지 결과에 대한 확률도 마찬가지가 된다.

확률 이론을 깊이 공부할 기회가 없었던 학샘들은 확률이 그저 비율에 관한 것이라는
인상을 가지고 있는 경우가 종종 있다. 아주 간단하게만 훌어보면서 조차 그러한 인상을
심어 준다는 것은 불공평할지도 모른다. 사실 확률의 가장 중요한 응용은 비율과는 전혀
상관이 없다. 이를 설명하기 위해서 두 가지의 간단한 예를 들어본다.

확률의 전형적인 교과서적 예는 동전 던지기이다. 동전은 대칭을 이루고 있기 때문에
보통 중립 원칙을 사용하여 확률을 지정한다. 따라서 다음과 같은 확률이 나온다.

반면에 압정을 던질 수도 있다. 동전과 마찬가지로 압정도 두 가지 방향으로 착지한다.
납작한 끝(앞면)이 땅에 By] 착지할 수도 있고, 납작한 면 가장자리와 뽀족한 끝점이 함
께 착지할 수도 있다. 뽀족한 끝점만 당게 착지할 수는 없다고 가정한다. 이 착지한 모양



===== PAGE 565 =====
@0000000
A8 확률 555

그림 &.4 압정이 착지하는 두 가지 방법. 압정은 대칭이 아니기 때문에 이 두 가지 결과가 SS
같다는 보장은 없다.

은 그럼 4.4와 같다. SAS 용어를 그대로 사용하여 납작한 끝을 "앞면"이라 하고, 다른
경우를 “뒷면"이라 하자. 압정은 대칭이 아니기 때문에 중립 원칙을 사용하여 앞면과 뒷
면에

같은 확률을 지정할 수 없다. 그러면 SHES 어떻게 지정할까? 동전의 경우 pee
5 이라고 하면 SAL 1.000번 던졌을 때 앞면이 500번은 나온다고 묵시적으로 가정
한다. 만일 실제로 앞면이 100번만 나온다면 가중치가 제대로 설정되어 있지 않았으며,
확률이 = +0] 아니었다고 의심하게 될 것이다. 같은 실혐의 반복 수행은 확률을 실제로
계산하는 하나의 방법이다. 즉, 같은 실험을 여러 번 반복하면 결과로 나온 확률은 꽤
WSUS 것이다(어떤 철학자는 확률을 이러한 시도의 수가 무한으로 접근할 때 이 분수
의 극한이라고 실제로 정의하였다). 예를 들어, 압정을 10,000번 던져서 납작한 면(앞면)
이 3.701번 착지했다고 하자. 그러면 그 압정은 다음과 같이 확률을 지정할 수 있다.

=<,

3,761

앞며   ~          -개00
2(앞면)     10.000   0.3761
6,239
3]     = -그      = (J.
2(뒷면)     10.000    0.6239

두 개의 사건의 확률이 같을 필요가 없다는 사실을 이제 알았다. 그러나 확률을 다 합하
lo] 된다. 이런 식으로 SSS 결정하는 WHS 확률에 대한 Ae yA] (relative
frequency approach)°]#}31 한다. 확률을 상대빈도 수를 가지고 계산할 때 = 심벌을 사
용한다. Hupsta 아무리 많이 실험을 반복 시도하더라도 상대빈도 수가 확률과 정확하
Al 일치하지 않기 때문이다. 예를 들어, 항아리에 와 로 표시된 2개의 공이 있다고 가
정하고, 이 중에서 하나의 SS 꺼내는 실험을 10,000번 반복한다고 하자. 그러면 Ast
표시된 SS 정확하게 5,000번 꺼낼 것이라고 확신할 수 없다. 4,967번 꺼낼지도 모른다.
중립 원칙을 사용하면 다음과 같은 결과를 얻지만,

상대빈모방식을 사용하면 다음과 같은 결과를 얻는다.
p(A) = 0.4967

상대빈도방식은 단지 두 가지의 다른 결과가 나오는 실험에만 국한되지 않는다. 예를


===== PAGE 566 =====
@00@00000 0
556   appendix A 수학

© 예제 4.15

들어, OBS 가진 주사위가 정육면체가 아니라면, 6개 원소사건의 확률은 모두 다를 수도
있다. 그러나 합은 그래도 1이 될 것이다. 다음 예제가 이 상황을 설명해 준다.

대칭이 아닌 6면 주사위가 있고, 1.000번 던져서 각 여섯 면이 나온 횟수가 다음과 같다고 가정
하자.

a          횟수
1            200
2           150
3           100
4           250
5           120
6           180
그러면
20) ~ 0.2
p(2) + 0.15
p(3) ~0.1
p(4) ~ 0.25
p(5) = 0.12
p(6) ~ 0.18

확률공간 정의의 ZA 3에 의해서 주사위를 던져서 24 30] 나올 확률은 다음과 같다.
p(2, 3) =p(2) +p(3) = 0.15+ㅜ0.1=0.25

확률의 개념을 결과에 대한 믿음(66160)의 정도라고는 조금도 여기지 않는 다른 접근
방식도 있다. 예를 들어, 시카고 베어즈가 달라스 카우보이스와 미식축구 경기를 하려한
다고 하자. AAV} 이 책을 쓰고 있는 지금 베어즈가 이기리라고 믿을 이유가 전혀 없다.
따라서 각 Bo] 이길 확률을 똑같이 할당하지는 않을 것이다. 이 경기는 여러 번 반복할
수 없기 때문에 상대빈도 접근방법을 사용하여 확률을 얻을 수 없다. 그러나 이 경기에
내기를 한다고 하면 베어즈가 이길 확률을 알아보고 싶을 것이다. 그러기 위해서 확률에
대한 주관적인 BAYA (subjective approach) 사용할 수 있다. 이 접근방식을 사용하
여 확률을 알아보는 방법 한 가지는 다음과 같다. 베어즈가 이기는데 거는 복권 HI $1
이라면 베어즈가 이길 경우 그 표가 얼마의 가치가 되어야 한다고 느끼는지를 결정해야
한다. 만약 그 가치가 $57} 되어야 한다고 생각한다고 하자. 즉, 이 BS 베어즈가 이길
경우 그 표의 가치가 최소한 $5가 되어야만 $1을 내고 그 HS 구입하려고 할 것이다.
이 경우 베어즈가 이길 확률은 다음과 같이 구할 수 있다.

7(베어즈가 이김)= ae 0.2



===== PAGE 567 =====
@0000000
A8 확률 557

즉, 이 확률은 공평한 내기라고 믿는 AES 가지고 계산한 것이다. 이러한 접근방식을
"주관적"이라고 하는 이유는 이 표가 $49] 1가치밖에 되지 않는다고 생각할 사람도 있기
때문이다. 그 사람에게는 8(베어즈가 이김'= 0.25이 된다. 이 두 가지 경우 모두 논리적
으로 잘 못된 것은 없다. 확률이라는 것이 단순히 개인의 믿음을 나타낼 때는 유일하게
정확한 확률은 없다. SHS 개인의 믿음에 대한 함수이다. 즉, 주관적이란 말이다. 만약
누가 자신이 따는 액수가 내기를 거는 액수와 같아야 된다고 믿는다면(즉, 그 표의 가치
가 반드시 $20] 되어야 한다고), 그 사람에게 SHS 다음과 같이 된다.

?(베어즈가 이김)= = 0.5

이제 확률은 단순히 비율만이 아님을 알았다. 확률의 의미와 철학에 대해서 자세히 알
아보기 위해서는 #ㅁ6(01973)을 읽어야 한다. 확률에 대해서 상대빈도방식은 Neapolitan
(1992)의 책을 참고하기 바란다. “중립 원칙”이란 표현은 <6706801948)에 처음 등장하였
THO] 책의 원본은 1921년에 출판되었다). Neapolitan(1990)-2 중립 원칙을 사용함으로써

순이 생긴다는 사실을 논한다.

^.8.1 무작위성

“무작위(880ㅁ0000"라는 용어가 일상 대화에서 자유로이 쓰이고 있기는 하지만, 엄격하게
정의하기는 패 어렵다. 무작위성은 WH process) 포함한다. 직관적으로 무작위 절차
란 다음을 의미한다. 첫째, 그 절차는 반드시 임의로 긴 GAS] 결과를 생성할 수 있어야
한다. 예를 들어, 같은 동전을 반복해서 던지는 절차는 앞면 또는 뒷면이라는 임의로 긴
일련의 결과를 생성할 수 있다. 둘째, 결과는 반드시 예측 불가능해야 한다. 그러나 여기
서 “예측 B7Hs8}cH unpredictable)" 말의 의미는 다소 모호하다. 우리가 처음 시작
했던 곳으로 다시 돌아간 것 같다. 그냥 "무작위"가 "예측 불가능하다"로 단순히 바뀌었을
뿐이다.

2047] 초에 리차드 폰 4]A]|ZA (Richard von Mises)7} 무작위(73000000689)의 개념을
더 상세하게 만들었다. 그는 “예측 불가능한" 절차는 작전을 아무리 잘 짜도 도박에서 성
공할 수 없어야 한다고 말했다. 즉, “예측 불가능한” 절차의 결과를 가지고 내기를 한다
면, BE Aso] 전부 ES 거는 대신에 결과의 일부분에만 돈을 걸어서 내기에 이길 기
회가 많아질 수 없다. 예를 들어, 반복해서 동전 던지기에서 앞면에 ESS 걸기로 했다고
하자. SAS 던질 때마다 ES 걸지 않고, 한 번씩 건너서 SS 건다고 이길 기회가 많아
질 수 있다고 생각하는 사람은 아무도 없을 것이다. 더구나 이길 기회가 많은 다른 "특별
한" 방법이 있다고 생각하는 사람도 없을 것이다. 어떤 특정 방법으로 돈을 걸어서도 이
길 기회가 많아질 수 없다면, 반복해서 동전 던지기는 무작위 절차가 될 것이다. 또 다른
예로 암에 걸린 환자와 그렇지 않은 환자가 있는 집단에서 반복해서 개인을 표본으로 뽑
고, 다음 표본을 뽑을 때 이전에 뽑은 표본은 다시 집단에 집어넣는다고 가정하자(이를


===== PAGE 568 =====
558

appendix A 수학

이

반환 후 표본 추출(680001108 with 76018060604/이라고 한다). 암에 걸린 환자가 뽑히는데
걸기로 했다고 하자. 어떤 특정 개인에게 전혀 우선권을 주지 않고 표본 추출을 한다면
매번 내기에 참여하는 대신 어떤 특정한 경우에만 참여한다고 해서 내기에 이길 기회가
많아진다고 생각하는 사람은 없을 것이다. 어떤 특정 방법으로 내기를 하여 이길 기회가
많아질 수 없다면 이 표본 추출 절차는 무작위가 될 것이다. 그러나 네 번에 한 번씩 흡연
자에서만 표본 추출을 하여 흡연자에게 우선권을 주고, 그 외에는 전체 집단에서 표본
FSS 한다면 그 절차는 더 이상 무작위가 아니다. 왜냐하면, 매번 내기에 참여하는 대
Al 네 번에 한 번씩만 참여함으로써 이길 기회가 많아지게 할 수 있기 때문이다.

직관적으로 “어떤 특정 개인에 우선권을 주지 않고 표본을 추출한다"는 Yo 표본 추출
을 행하는 방식에 어떤 패턴이 없다는 것을 뜻한다. 예를 들어, 항아리에서 반환 후 표본
추출을 할 때 표본 추출할 때마다 항아리를 잘 흔들어 공이 잘 섞이게 한다면 절대로 어
떤 공에도 우선권을 줄 수가 없게 된다. 월드컵 축구 조 편성할 때 얼마나 철저히 공을
섞는지 보아서 알 것이다. 사람의 집단에서 표본 ASS 할 때는 우선권이 주어지지 않았
다고 확신하기가 힘들다. 표본 추출 방법에 대해서는 이 HSS] Yoo] 벗어나므로 다루
지 않는다.

성공적인 도박 전략을 허용하지 않는 폰 미세즈의 요구사항은 무작위의 의미를 이해하
는데 도움을 준다. 예측 가능한 절차 또는 무작위가 아닌 절차는 성공적인 도박 전략을
짤 수 있도록 허용한다. 무작위가 아닌 절차의 aE 위에서 언급했듯이 네 Hol] 한 번씩
흡연자에게서만 표본을 추출하는 것이다. 또 다른 예로서 저자 중 한사람의 운동 계획을
살펴보자. 그는 화, 목, 일요일에 그의 운동센터에서 운동하고 싶어 한다. 그러나 그 중에
하루를 빠지면, 다른 날 중에 하루를 선택하여 보충한다. 그가 어떤 Yo] 운동을 하는지
내기를 한다면, 7개의 요일 중에서 선택하는 것보다 화, 목, 일요일 중에 하나를 선택하
는 것이 훨씬 좋다. 이 절차는 무작위가 아니다.

비록 폰 미세즈가 무작위를 더 잘 이해하도록 해줄 수는 있었지만, 정확하고 수학적인
ANS 만들어 내지는 못했다. Ashe 안드레이 콜모고로프(00761 Kolmogorov)7} 축소
가능한 수열 WAS 가지고 정확하게 정의하였다. 간단히 설명하면 어떤 유한 수열이 그
수열에 있는 모든 항목을 암호화하는데 드는 것보다 비트 수를 적게 사용하여 암호화할
수 있다면, 그 유한 수열은 축소 가능하다(60ㅁㅁ0『0881019)라고 정의한다. 예를 들어, 다음
"0 이 16H 반복되는 다음 수열은

10101010101010101010101010101010

다음과 같이 표현할 수 있다.
1610

이 HAS 암호화하는 것이 수열의 모든 PHS 암호화하는 것보다 비트의 수가 적게 들
기 때문에 이 수열은 축소 가능하다. 축소 불가능한 수열은 무작위 수열ㅠ80000. 86-



===== PAGE 569 =====
© 예제 4.16

© 예제 4.17

0000000
A8 확률 559

quence) 한다. 예를 들어, 다음은 무작위 수열이다.
1001101000101101

왜냐하면, 더 효율적인 표현 방법이 없기 때문이다. 직관적으로 무작위 수열이란 규칙적
이지 않거나 패턴이 없는 수열을 말한다.

콜모고로프 이론에 따르면 무작위 절차(80000 process) 절차가 충분히 오래 계속되
면 무작위 수열을 생성하는 절차이다. 예를 들어, 반복해서 동전을 던지고, 앞면이 나오
면 1, 뒷면이 나오면 OS 각각 할당한다고 가정하자. 6번 던지고 난 후 다음과 같은 수열
ㅣ 생겨날 수 있다.

ㅇ

101010

그러나 콜모고로프 이론에 따르면 결국에 가서 전체 FAS 위와 같은 규칙성을 가지지
않을 것이다. 무작위 수열을 "확실히" 생성하는 무작위 절차를 정의할 수 있는가 하는 철
학적인 어려움이 있다. 많은 확률학자들은 수열이 무작위가 될 확률이 높을 뿐 수열이
무작위가 되지 않을 가능성도 있다고 믿고 있다. 예를 들면, 동전을 반복해서 던질
그럴 가능성이 거의 없기는 하지만 동전이 영원히 계속 앞면만 나올 수도 있다고 믿고
있는 것이다. 앞에서 언급했듯이 무작위성은 어려운 개념이다. 오늘날까지도 무작위의
특성에 대해서 논란이 계속되고 있다.

무작위가 확률과는 어떤 관계가 있는지 토의해보자. 무작위 절차는 확률 표본공간을

결정하고(이 절의 초반부에 주어진 정의를 보시오), 절차가 결과를 생성할 때마다 이 표
본공간에서 실혐이 수행된다. 다음 예제들이 이를 잘 설명해준다.

on
flo

일
=

tho

계

cr
>

공 하나와 흰 공 하나가 들어있는 항아리가 있다고 하고, FS 꺼내고 집어넣
이 무작위 과정으로 다음과 같은 확률 공간이 결정된다.
p(black) = p(white) = 0.5
공을 꺼낼 때마다 이 공간에서 실험을 수행한다.

예제 4.18의 비대칭인 육면체 주사위를 반복해서 던지는 것은 다음과 같은 확률 공간이 형성되
는 무작위 과정이다.

p(1) = 0.2
p(2) = 0.15
p(3) ~ 0.1
p(4) = 0.25
p(5) = 0.12
p(6) = 0.18

주사위를 던질 때마다 이 공간에서 ABS 수행한다.



===== PAGE 570 =====
06 00000 0
560   appendix A 수학

© 예제 A18

© 예제 A19

명의 모집단에서 일부는 암에 걸려있고, 특정 개인에게 절대 우선순위를 주지 않고 공평
반환 후 표본 추출 한다고 가정하자. 이러한 무작위 과정으로 모집단이 표본공간이 되도록

을 결정하고("표본공간"과 "모집단”은 서로 바꾸어가며 사용할 수 USS 상기하라),
각 사람이 HBAS 될 확률(원소사건)은 1/7이다. Yo] 걸린 사람이 표본 추출될 확률은 다음

암에 걸린 사람의 수

n
실험을 할 때마다 모집단에서 무작위로(6 random) 사람을 뽑는다고 한다. 실험을 반복해서 나
온 결과의 집합은 모집단의 무작위 표본추출(60000 880019/이라고 한다. 무작위 표본추출의
크기가 크다면, 표본이 모집단을 대표할 확률이 높다는 사실은 통계 기술을 사용하여 보여줄 수
있다. AS 들어 무작위 표본추출의 크기가 크고, 표본추출한 인구의 Lo] 암에 걸려 있다면 모

집단의 인구 중에서 암에 걸린 사람의 비율이 Soll 가까울 확률이 아주 높다.

카드 한 벌이 있고, 카드를 순서대로 뒤집는다고 가정하자. 이 과정은 무작위가 아니고, 카드는
무작위로 뽑지 않는다. 이 비무작위 과정(00060000 process) OB 결과가 나올 때마다 다른
확률공간이 정해진다. 첫 시도에서 각 카드가 뽑힐 확률은 T 가 되고, 두 번째 시도에서는 처음

뽑힌 카드가 나올 SHES 00] 되고, 나머지 각 카드가 뽑힐 확률은 =o] 되고, 이런 식으로 계
속 확률이 변하게 된다.

만약 맨 위에 있는 카드를 뽑고, 다시 집어넣고, 한 번 뒤섞는 과정을 반복한다고 가정하자. 이
과정은 무작위 과정이고, 카드는 무작위로 뽑는 것일까? He “아니오"이다. 마술사이며 하바드
대학의 통계학자인 퍼시 다이아코니스(06791 Diaconis)= 카드를 THE 뒤섞어야 철저히 섞여져
서 그 과정이 무작위가 된다는 사실을 증명했다(40005와 Diaconis(1986) 참조).

폰 미세즈 무작위 개념이 오늘날에는 직관적으로 잘 받아들여지고 있지만, 그 이론을
개발할 당시(20세기 초)에는 그의 견해가 널리 인정받지는 못했다. 그의 가장 강경한 반
대자는 철학자 UPS (Marbe) Bt}, 마브는 자연은 기억을 부여받고 있다는 견해를 가지고
있었다. 그의 이론에 따르면, 공평한 동전(앞면이 나올 상대빈도가 0.5인 동전)을 가지고
반복적 동전 던지기에서 뒷면이 연속해서 15번 나오면, 다음 던질 때 자연이 이미 나온
BAS 보상해주기 때문에 앞면이 나올 확률이 높아진다. 만약 이 이론이 맞다면 뒷면이
여러 번 나온 후에만 앞면에 내기를 하면 이길 기회가 높아질 수 있다. 아이버슨(106080ㅁ,
1971) 등이 미세즈와 콜모고로프의 견해를 입증하는 실험을 하였다. 그들의 실험에서 구
체적으로 동전 던지기와 주사위 던지기는 무작위 수열을 만들어 냄이 입증되었다. 비록
꽤 많은 도박꾼들이 마브의 이론을 아직도 따르고 있지만 오늘날 마브의 이론을 인정하
는 과학자는 거의 없다.

폰 미세즈 이론의 원문은 76ㅁ 8486801919)이며, 그의 책 von Mises(1957)o]] 더 쉽게 설



===== PAGE 571 =====
© 예제 A.20

@‥00060000 0
A8 확률 561

명되어 있다. 압축가능(60ㅁ2『6881016) 수열과 무작위 수열은 박사논문 Van Lambalgen
(1987) oj] 자세히 나와 있다. Neapolitan(1992)7} Van ㄴ870081860(0198?)에서는 무작위 과
정이 무작위 수열을 확실히 만들어낸다고 정의하기 어렵다는 주장을 제기하고 있다.

A.8.2 기대치
기대치(평균)를 AAS 통하여 이해해보자.

키가 68, 72, 67, ?4인치인 4명의 학생이 있다고 하자. 평균키는 다음과 같이 계산한다.
_ 68+72+67+74

평균키= ~ 인치= 70.25 인치
다음과 같이 백분율로 키가 분포된 1.000명의 학생이 있다고 하자.
학생의 백분율     키(인치)

20             66

25             68

30             71

10             72

15             74

평균키를 계산하기 위해서 각 학생의 키를 구하고, 위의 방법대로 계산할 수 있다. 그러나 다음
과 같이 평균을 구하는 것이 훨씬 효율적이다.
Wat7]=66(0,2) + 68(0,25) + 71(0,3) + 72(0,1) + 74(0.15)인치=69.8인치

이 예제에서 백분율은 중립 원칙을 이용하여 구한 확률일 뿐이다. 즉, 학생 20%의 키
가 66인치라는 사실은 20039] 키가 66인치라는 의미이고, 1000명의 학생 중에서 무작위
로 한 학생을 뽑으면 다음과 같다.

200 _

=  0 치)= ——_ =
2(키=666인치= 200

0.2

일반적으로 기대치는 다음과 같이 정의한다.

{e,, €o) “""5 e, }

각 결과 e = 22} 관련된 실수 f(e;) 가 있다고 가정하면, fle, 는 표본공간에서 무작위 변수
(random variable)2} 하고, f(e;) 의 기대치(평균)는 다음과 같이 계산하다.

f(e,)p(e,) + f(e,)p(e,) xe + fle, )p(e,,)



===== PAGE 572 =====
@00@000000
562   appendix A 수학

* 예제 A21

© 예제 4.22

무작위 변수를 “무작위"라고 하는 이유는 무작위 과정을 통하여 무작위 변수의 값을
구할 수 있기 aac:  “기회변수(80406 variable)” 또는 추계 H==(stochastic varia—
ble)"2} 용어를 사용하기도 한다. 여기서 “무작위 변수"라고 하는 이유는 가장 많이 쓰기
때문이다.

예제 A 154419} 같이 대칭이 아닌 Gel 주사위가 있다고 가정하자. 즉, 각 면이 나올 확률은 다음
과 같다.

p(1) =                 p(4) A025
p(2) = 0.15        p(5) ~ 0.12
p(3) =              p(6) = 0.18

표본공간은 나올 수 있는 6개의 다른 면으로 구성되어 있으며, 표본공간에서 무작위 변수는 그
면에 쓰인 수이며, 이 무작위 변수의 기대치는 다음과 같이 계산한다.

1p(1) + 2p(2) +3p(3) + 4p(4) +5p(5) +6p(6)

= 1(0.2) +2(0.15) +3(0.1) +4(0.25) +5(0.12) +6(0.18) =3.48

만약 SAAS 여러 번 던지면, 나오는 수의 Bate 대강 3.48 정도 된다고 기대할 + 있다.
표본공간에서 정의하는 무작위 변수가 하나만 있는 것은 아니다. 홀수가 나오면 OS 배정하고,
홀수가 나오면 1을 배정하는 함수가 이 표본공간에서 또 하나의 무작위 변수로 될 수도 있다.
이 무작위 변수의 기대치는 다음과 같이 계산한다.

Op(1) + 1p(2) + Op(3) + 1p(4) +0p(5) +1p(6)

= 0(0.2) +1(0.15) +0(0.1) +1(0.25) +0(0.12) +1(0.18) =0.58

예제 A202} 1,000명의 학생을 표본공간이라고 하자. ㅅ.90에서 계산한 대로 키가 이 표본공간의
무작위 변수라고 하자. 다른 하나는 몸무게가 될 수도 있다. 만약 몸무게가 다음과 같은 백분율
로 분포되어 있다면,

학생의 백분율 무게(파운드)

15                      130
35                      145
30                      160
10                      170
10                      185

이 무작위 변수의 기대치는 다음과 같이 계산한다.
130(0.15) + 145(0,35) + 160(0,30) + 170(0,10) + 185(0.10)파운드=153.75파운드



===== PAGE 573 =====
rh

4

%

ㅁ

Ala

ile

다음 값을 구하시오.

(a) |2.8]                         (b) |-10, 42
(0 [4,2]                         (d) [ -34,92]
(e) |5.2-4.7]                     (f) [27]

다음 등식이 성립함을 보이시오.
[n]=-|-n]
BE 실수 7에 대해서 다음 등식이 성립함을 보이시오.

[2eJ=[2]+|2+3|

BE Bt a>0, 0> 0, 7에 대하여 다음 등식이 성립함을 보이시오.
+

다음 각 AS 덧셈(시그마)을 사용하여 다시 쓰시오.
(a) 2+4+6+---+2(99) +2(100)

(b) 2+44+6+4---+2(n—1)+2n

(c) 3+12+27+---+1200

다음 HS 계산하시오.
(a) 31(2i-+4)
t=1

10
00 >) (i? — 44)
i=1

wa( ? irl
2 기쁘 i ㅣ

(AS: 처음 두 개 또는 세 개 SS 약분하지 말고 작성하여 패턴을 보라.)
(d) (ain), n=4e 경우

i=0

4  i
(0) >1>)(0+5)

i=1j=1

^ 2절

i
8.
9.

함수 f(x) = Vz—4 의 TABS 그리시오. 이 함수의 변역과 치역은 무엇인가?
함수 f(x) =(ex-2)/(a@+5) 9] 그래프를 그리시오. 이 함수의 변역과 치역은 무엇인가?
함수 f(x) =l2] 2] 그래프를 그리시오. 이 함수의 변역과 치역은 무엇인가?


===== PAGE 574 =====
564

appendix A 수학

10. 함수 fla) =[2] 9] 그래프를 그리시오. 이 함수의 변역과 치역은 무엇인가?
Asa
11. 모든 정수 n>0o] 대하여 다음 등식이 성립함을 수학적 귀납법으로 증명하시오.

YG)
k=1

12. BE 양의 정수 ㅠ에 대하여 n?—no] 짝수임을 수학적 귀납법으로 증명하시오.
13. BE 정수 n> 40] 대하여 다음 등식이 성립함을 수학적 귀납법으로 증명하시오.

Sine
14. BE 정수 n> 0] 대하여 다음 등식이 성립함을 수학적 귀납법으로 중명하시오.
n   2    n
2 ~
i=l    i=1

^.4절
15. ㅇ와 》가 모두 홀수이면, atde 짝수임을 증명하시오. 역도 성립하는가?
16. “a+b7} 홀수이다"는 "와 《가 돌 다 홀수가 아니거나, 둘 다 짝수이다“의 필요충분조건(

'는
and only 14임을 증명하시오.

^.5절

17. 다음 HS 구하시오.
(a) log 1,000        (b) log 100,000              (c) log, 64
(d) 18 iz           (e) log, 125                 (f) log 23
(g) lg (16 x 8)      (h) log (1,000/100,000)     (i) gig 16

18. 같은 좌표에 함수 f(x) = 2° g(x) =1827의 그래프를 그리시오.

19. 2? +6r+12>8r+200] 성립하는 2값을 찾으시오.

20. > 50182이 성립하는 2값을 찾으시오.

21. 함수 /(2)=ㅇ2“가 지수함수가 아님을 보이시오.

22. 모든 양의 정수 에 대하여 다음 등식이 성립함을 보이시오.
lign|+1=[lg(n+1) |

23.

ㅅ.6절

합이다), 다음을 구하시오.



===== PAGE 575 =====
25.
26.

27.

연습문제      565
(a) SUT
(b) SNT
(00 S-T
(0) 7T-S

(e) (SNT)US)

0) U-S(S2] 보집합이라고 함)

집합 의 구성원소가 개 있을 때, 의 부분집합의 개수는 2"이 됨을 증명하시오.

IS|S 집합 6의 구성원소의 개수를 나타낸다고 하자. 다음 등식이 맞음을 증명하시오.
ISUTI=ISIFITI-ISN T|

다음이 모두 같음을 증명하시오.

(a) Se 2    (b) SLs   @ SUg=F

A728

28.
29.

30.

31.

32.
33,

35.

10개의 물체에서 한 번에 6개를 취하는 <ek(permutation) 2] 수를 구하시오.
10개의 물체에서 한 번에 6개를 취하는 조합(6074108400/의 수를 구하시오. 다른 말로,
[입을 구하시오.

10개 공이 들어있는 통에서 4개 BS 꺼내는 복권추첨이 있다고 가정하자. 뽑는 순서대로
공이 나열되어 있으면 당첨복권이다. 당첨될 수 있는 복권의 개수는 총 몇 장인가?

10개 공이 들어있는 통에서 4개 공을 꺼내는 복권추첨이 있다고 가정하자. 뽑는 순서에 상
관없이 맞는 공만 있으면 당첨복권이다. 당첨될 수 있는 복권의 개수는 총 몇 장인가?
ATH 있는 이항정리를 수학적 HIS 사용하여 증명하시오.

다음 등식이 성립함을 증명하시오.

2

[기이
첫째 종류의 물체가 《,개 있고, 둘째 종류의 물체가 개 있고 …, mA] SH] 물체가
개 있다고 가정하자. 여기서 4 + hy + +k, =n Olt, 이 7개 물체의 서로 다른 순열의 수
는 다음과 같이 됨을 증명하시오.

n!

(Ay!) (he!) «++ Ca!)

f(n, m)-& nM] 동일한 SAS 개의 집합에 분배하는 방법의 가지수라고 하자. 예를
들어, n=4, m=2 물체의 집합을 {4, A, A, A} 라고 하면 가능한 분배방법은 다음과
같다.

(1) {A, A, A, A}, @

(2) {A, A, A}, {A}

(3) {A, A}, 14, A}

(4) {A}, {A, A, A}


===== PAGE 576 =====
566

appendix A 수학

(5) @, {A, A, A, A}
여기서 f(4, 2) =5임을 알 수 있다. 일반적으로 다음과 같은 해를 갖게 됨을 증명하시오.

ln, m)=("F™ 1}
AG : 가능한 BE 분배의 집합은 첫째 슬롯에 7개의 4가 들어있는 집합, 첫째 슬롯에
nT AS] AP} 들어있는 Aah, .…., 첫째 SKA] 0깨의 .4가 들어있는 AGS 구성된다.
mo] 대한 귀납법으로 증명하면 된다.

36. 다음 등식이 성립함을 증명하시오.

^ 8절
37. 연습문제 302] 복권추첨을 ^ 고려해보자.
(8) 복권 한 장을 구입한 경우 당첨될 확률을 계산하시오.

(9 복권 일꼼 BS Fe 경우 GAM ISS 계산하시오

38. 한 벌(58장)의 카드를 가지고 (5장) 포커게임을 한다고 가정하자.
(a) 손에 4장의 A7} 들어올 확률을 계산하시오.
09) 손에 같은 종류의 카드가 4개 들어올 확률을 계산하시오.

39. 공평한 6면 주사위(즉, 각 명이 나옴 확률은 승) 던지기 놀이를 한다고 하자. 59} 6이 나오면
가가 $59} $6% 잃게 되고, 다른 수가 나오면 그 수에 해탕하는 VS] $를 딴다고 하자.
(9) 따거나 잃게 될 돈 액수의 기대치를 계산하시오.
(b) 100회 던지는 경우, 가장 많이 잃을 액수, 가장 많이 딸 액수, 따거나 잃을 기대 액수를
각각 계산하시오.
40. 7개의 서로 다른 원소의 리스트에서 하나의 구성원소를 검색한다고 가정하자. 순차검색 알
고리즘(직선검색)을 사용할 때 필요한 비교의 평     arate 횟수는 얼마인가?

41. 개 원소로 구성된 배열에서 삭제 연산을 하는데 구성원소를 옮기는 기대 횟수는 얼마인
가?



===== PAGE 577 =====
a.p p € ii dix B

재현식의 해 구하기 :

재귀 알고리즘 분석용

귀 알고리즘(6600478176 algorithm)2] 분석은 반복 알고리즘(1681176 algorithm)
재  과 달리 그리 간단하지 않다. 그러나 보통 재귀 알고리즘의 시간복잡도를 재현
Al(recurrence equation) © 나타내는 것은 그리 어렵지 않다. 그리고 시간복잡도를 구
하기 위해서는 그 재현식의 HS 반드시 구해야 한다. 이 부록에서는 재현식의 해를 구하
는 기술과 재귀 알고리즘의 분석에 그 HS 사용하는 기술에 대해서 살펴본다.

@ Bl 귀납법으로 재현식의 해 구하기

> 알고리즘 BY

수학적 귀남법은 부록 에서 공부하였다. 여기서는 재귀 알고리즘을 분석하는데 수학적
귀납법을 어떻게 사용하는지 살펴본다. 먼저 nS 계산하는 재귀 알고리즘을 보자.

Factorial

문제 : # > 1일 때 nl=n(n—1)(n—2)-+ (3)(2)(1)을 구하시오.
입력 : 음이 아닌 정수 7

출력 : n!

int fact (int 7)

)

return 2 * fact(n—1);

{
if (2 ==
return 1;
else
}

이 알고리즘의 SS 파악하기 위하여 각 7에 대하여 이 함수가 곱셈을 몇 번 수행하


===== PAGE 578 =====
@0000000
568     appendix B 재현식의 해 구하기: 재귀 알고리즘 분석용

는지 알아보자. 주어진 nol] 대한 곱셈의 총 수행 NSE fact(n—1)S 계산할 때 곱셈
의 수행 횟수에다 n-& /00(-1)로 곱할 때 수행하는 곱셈 1회를 더하면 된다. 주어진
nol] 대하여 곱셈의 수행 횟수를 《, 으로 표시하면 이를 다음 방정식으로 나타낼 수 있다.

시 = Be + I
재귀에서 상위수준에서
곱셈 횟수 곱셈 횟수

이와 같은 방정식은 nol] 대한 함수 값을 7보다 작은 값에 대한 함수 값의 형태로 나타내
기 때문에 재현식(8600776006 60481102)이라고 한다. 사실 재현 그 자체로는 함수를 제대
로 나타내 주는 것은 아니다. 또한 재현식에는 초기조건0010181 00ㅁ01402)이라고 하는 재
귀기초가 반드시 있어야 한다. 위의 알고리즘에서 7= 0일 때 곱셈의 횟수는 0이므로,
초기조건은 다음과 같이 나타낼 수 있다.

ty =0
이보다 큰 7값에 대한 《, 은 다음과 같이 계산할 수 있다.

= -1+1=8+1=0+1=1
ty =, +1=t,+1=14+1=2
ty =f. +1 =f +152+1583

이와 같은 방법으로 계속하여 어떤 《, 의 값도 구할 수 있지만, 0에서 시작하지 않고 임의
의 7에 대하여 바로 《, 을 계산할 수 있는 것은 아니다. 따라서 《, 을 명백히 Al(express—
ion) OS 나타낼 수 있어야 한다. 이러한 식을 재현식의 해(6014000)라고 한다. 귀납법을
사용하여 OS 찾는 것은 불가능하며, 단순히 예상해(68ㅁ01086 solution)7} 맞는지를 확
인할 수 있을 뿐이다(8.5.4절에서 다룬 직관적 FA (constructive 1001400102)을 사용하

면 해를 찾을 Se 있다). 위에서 계산한 몇 개의 값을 조사해보면 해는 다음과
알 수 있다.

fore)
et

6:
이제 이 예상해가 맞는지 귀남법을 사용하여 증명해보자.
귀납기초 : ㅠ= 0에 대하여 다음은 성립한다.
= 0
귀납가정 : 임의의 양 정수 nol 대하여 다음이 성립한다고 가정한다.

=

귀납절차 : 다음이 성립함을 보이면 된다.



===== PAGE 579 =====
* 예제 81

0000000
Bl 귀납법으로 재현식의 해 구하기   569

tag, =ntl
재현식에서 nS 7+1로 대치시키면, 다음과 같이 된다.

따라서 《, 의 예상해가 맞는지를 증명하였다. 여기서 진한 활자체로 된 항은 귀납가정과
같음을 주목하라. 귀납법 증명을 할 때 귀납가정이 적용되는 부분을 이 책에서는 이런
식으로 종종 표시한다.

재귀 알고리즘의 분석은 두 단계로 이루어진다. 첫째 단계에서는 재현식을 결정하고,
둘째로 그 방정식의 해를 구한다. 여기서 우리의 목표는 재현식의 해를 어떻게 구하는지
보여주는 것이다. 이 책에서 나오는 재귀 알고리즘의 재현식은 알고리즘을 논의할 때 결
정한다. 따라서 앞으로 이 부록에서는 알고리즘에 대한 논의는 하지 않고, 그냥 재현식만
을 주어진 대로 취한다. 귀납법을 이용하여 재현식의 해를 구하는 예를 몇 가지 더 살펴
보자.

다음 재현식을 보자.

th -%/271  (7>1이며, n°] 29] 거듭제곱일 때)

ty =6/2+1=86+1=1+1=8
ty =tyg +1 =t+1=24+1=3
tg =te+1=t,+1=3+1=4
tig =tygpt1=_zt1=441=5

따라서 일반항은 다음과 같다.
t, =lgn+1
이제 귀납법을 사용하여 이 일반항이 맞는지를 증명한다.
귀납기초 : ㅁ=1에 대하여 다음은 성립한다.
t, =1=181+1
귀납가정 : 2 > 0이고 29] 거듭제곱인 임의의 정수 nol] 대하여 다음이 성립한다고 가정한다.
t, =lg n+1
귀납절차 : 재현식이 2의 거듭제곱에 대해서만 국한되어 있기 때문에 7 다음에 고려해야 할 수
는 27이 된다. 따라서 다음이 성립함을 보이면 된다.
ton =lg(2n) +1


===== PAGE 580 =====
0000000
570     appendix 8 재현식의 해 구하기: 재귀 알고리즘 분석용

* 예제 8.2

재현식에 27을 대치시키면, 다음과 같다.

ty

=Ign+]lg2+1

=I1g(2n)+1

다음 재현식을 보자.

ty =-76./> (n>1°)H, no] 29] 거듭제곱일 때)

ty =Ttyjp = Tt, =7

ty = Tajo = Tt =7
ts = Vtg =7t, =7°
tig = Ttio/2 = Ts = 7

따라서 일반항은 다음과 같다.

이제 AHS 사용하여 이 일반항이 맞는지를 증명한다.
귀납기초 : 2=1에 대하여 다음은 성립한다.

= Ne ge
귀납가정 : n> 0이고 29] 거듭제곱인 임의의 정수 7에 대하여 다음이 성립한다고 가정한다.
Lan
귀납절차 : 다음이 성립함을 보이면 된다.
a — 782n)

재현식에 2nS 대치시키면, 다음과 같다.
따라서 귀납법 증명이 완성되었다. 마지막으로, 다음 성질에 의하여
70 — 767

이 재현식의 해는 보통 다음과 같이 쓴다.



===== PAGE 581 =====
* 예제 8.3

@ee2e @ @ 0
하여 재현식의 해 구하기     571

이
02
Jin

소

Ma
milo
을
00

다음 재현식을 보자.

 =26.2+7-1  01>1이며, no] 8의 ASA wh)
。-0

ay
lo
ye
ot
to
a
rlo

ty = Qtyyg +2—-1=2t, +1=1

ty = Qtyy +4—1=2t,+3=5

ty = 2g + 8-1 =2t,+7=17

16 = 2tyg/g + 16-1 = 24, +15 = 49
이 값들만 보아서 해가 무엇인지 분명하지 않다. 앞에서 밝힌 대로 귀남법은 예상해가 맞는지를
SRI 수 있을 뿐이다. 여기서 AVE 구할 수 없으므로 이 재현식의 해를 구하기 위해서 귀
납법을 사용할 수도 없다. 그러나 다음 절에서 공부할 기술을 사용하면 해를 구할 수 있다.

@ B2 특성식을 이용하여 재현식의 해 구하기

* 예제 8.4

다양한 종류의 재현식의 해를 구하는 기술을 전개한다.

B.2.1 동질 1차 재현

ra

Al
식

정의

정으

《와 a, SO] 상수일 때, 다음 형태의 재현식은 상수계수 동질 1차 재현식(「107709606046 linear
recurrence equation with constant coefficients)O|2} 한다.

Opt, Otay rer Gye, =p — 0

이러한 식을 “1AHlinear)"e} 하는 이유는 모든 항 *,가 일차이기 때문이다. 즉, th_;
ES ti, Ares 항이 없다. 추가적으로 가 19] 아닌 양 상수가 되는 to) Se
허용하지 않는다. 예를 들면, tayo, 3(,-4) SA 같은 VS 허용하지 않는다. 이러한 재
현식을 “동질0400ㅁ086060048) 이라 하는데, 그 이유는 항의 1차 조합(11068 combination)

이 0°] 되기 때문이다.

다음은 상수계수 동질 1차 재현식이다.
Tt, —3t,_, =0
6t, —5t,_, +8t,_» =0
8t, —4t,-3 =0



===== PAGE 582 =====
@0000000
572   appendix ㅁ 재현식의 해 구하기: 재귀 알고리즘 BAS

* 예제 BS 1.2.2절에서 공부하는 피보나찌 <A (Fibonacci 86046008)은 다음과 같이 정의한다.

th = +t,»
=o
시 =

SANA *。_,과 42S 빼면, 다음과 같다.
t tt 8 —0

n

이 방정식을 보면 피보나찌 순열이 동질 1차 재현식임을 알 수 있다.

다음은 동질 1차 재현식의 해를 어떻게 구하는지 알아보자.

*예제 86 다음과 같은 재현식이 있다고 가정하자.

시 — 5t,-1 + 6t, _» =0      (n>1°]*)
' =0
t,=1
t= 다음과 같이 놓으면,
t, =r"
다음과 같은 등식을 얻을 수 있다.

t, —5t,_,+6t,_. =r" -52 1 622 2

그러므로 ro] 다음 방정식의 근이면,
50 1680 1 = 0
t, =r" 재현식의 해가 된다.
여기서, 다음 등식이 성립하므로
fbr +62 =70(2-50+ 6)
oo ㅎ=0의 됨을 알 수 있고, 또 다른 ae 다음 빙정식으로 큰을 구한다.
r’—5r+6=0                                (B.1)
이 근을 구하기 위해서 인수분해하면, 다음과 같다.
r’—5r+6=(r—3)(r—2) = 0
여기서 DS 7=3과 7=ㅇ2가 된다. 따라서 재현식의 모든 BE 다음과 같다.
t, =0, t, =3"y} t, =2"

이를 3" oj] 대하여 해가 맞는지 입증하기 위해서 재현식의 좌변을 #으로 다음과 같이 치환해
보자.



===== PAGE 583 =====
B2 SSS 이용하여 재현식의 해 구하기     573

|

3n    gro    gr 2
4 4        '
bg 09 7106,
이렇게 치환하면 좌변은 다음과 같다:
3” —5(3"~*) +6(3""-?) =3" —5(3""7) ㅜ2(90 1)
= 3"—3(3""') =3"—3" =0
이는 8”이 이 재현식의 해자 된다는 뜻이다.
이 MAAS] HS 3개 찾았다. 그러나 해는 더 존재한다. 3" yp 2”이 해이므로, 과 <;가 임의
의 상수이면 다음 식도 해이다.
ty = 0,3" +¢,2”
이 결과는 뒤의 연습문제에서 얻은 결화이다. 비록 여기서 보여주지는 않지만, 이외에 더 이상의
해는 없음을 증명할 수 었다. 따라서 위의 식은 재현식의 일반해이다(~ =e =O 때 보통해인
t, = 0은 일반해에 포함되어 있다). 여기서 해는 무한개가 있지만 어떤 해가 우리가 원하는 해일
까? 이 질문에 대한 답은 초기조건으로 결정한다. 다음과 같은 초기조건이 있었음을 돌이켜보자.
ty) =O7} t, =1
이 조건을 가지고 다음과 같이 ㅇ, 과 <,의 유일한 값을 구할 수 있다. 일반해에 각 값을 적용시키
면, 다음과 같이 변수가 두 개인 연립방정식을 얻는다,
pes +52" = 0
i =0631+621 =1
이 연립방정식은 다음과 같이 간략화할 수 있다.
c +e, =0

3c, + 2c, =1
이 연립방정식의 해는 < = 13} 6 =-ㅡ1이다. 따라서 재현식의 해는 다음과 같다.

+, =1(3") —1(2") =3"— 00

바로 앞의 예제에서 초기조건이 다르다면, 다른 해가 나왔을 것이다. 실제로 재현식은
함수를 여러 개 모아놓은 것으로 볼 수 있다. 즉, 각 함수에 다른 초기조건이 대입한 것이
다. 예제 B62] 재현식에 다음 초기조건을 사용하면 어떤 함수가 나오는지 살펴보자.

예제 8.6의 일반해에 이 초기조건을 적용하면 다음과 같은 연립방정식

thlo

얻는다.
pes +e) = 1

= o3'+ a? = 2


===== PAGE 584 =====
06000000
574     appendix B 재현식의 해 구하기: 재귀 알고리즘 분석용

© 예제 8.7

이 연립방정식은 다음과 같이 간략화할 수 있다.
0061

3c, + 2c, = 2
이 연립방정식의 해는 6, = OF} 6, = 1이다. 따라서 이 새로운 초기조건 하에서 재현
식의 해는 다음과 같다.
t, = 0(3")+1(2") = 2"

예제 B62] 방정식 BAS 그 재현식에 대한 특성식이라 한다. 일반적으로 이 식은 다음
과 같이 정의한다.

정의
At, ta,t,_1 + +azt,_,=0

위 동질

et
>
=
[위
Iz
2
=

한 BAAl(characteristic equation 다음과 같이 정의한다.

ayr* tar} 리모 이 0" =0

"의 값은 단순히 1이다. 여기서 7"라고 쓰는 이유는 특성식과 재현식과의 사이의 관
AZ 보여주기 위함이다.

재현식에 대한 특성식은 다음과 같이 나타난다.
5t, —Tt,_1+6t,_» =0

5r’>7r+6 =0
화살표를 사용하여 특성식의 차수가 《*임을 보여준다(이 경우는 2).

예제 .6에서 해를 구하기 위해 사용한 단계는 정리로 일반화할 수 있다. 상수계수 동
질 1차 재현식을 풀기 위해서는 정리만 참고하면 된다. 그 정리는 다음과 같고, 증명은
이 부록의 끝부분에 있다.

다음과 같은 상수계수 동질 1차 재현식에 대해서

Got, Fab ae, — 0

apr* +a,r*—* 가 tar? =0



===== PAGE 585 =====
* 예제 8.8

@00@00000 0
B2 특성식을 이용하여 자현식의 해 구하기 575

이 특성식이 *개의 “서로 다른" 해 ry, ry …, ㅠ,를 가진다면, 이 재현식의 유일한 해는
t, = 이러 1 900 + 이시

여기서 og HE 임의의 상수이다.

KAS] 상수 <의 값들은 초기조건으로 구한다. *개의 상수들을 모두 구하려면 *개의
초기조건이 필요하다. 다음 예제에서 상수의 값을 구하는 방법을 살펴보자.

다음 재현식의 해를 구해보자.

t, —3t,_;—4t,_» =         (242 >1이면)
0
i =
1, 특성식을 찾는다
t, —3t,_, —4t,_» =0
| =0

2, 특성식의 해를 구한다.
r’—3r—4=(r—4)(r+1) = 0
이 방정식의 근은 7=4와 7=-ㅡ1이다.
3. 정리 BLS 적용하여 재현식의 일반해를 구한다.
t, =¢4"+e,(-1)"

4, 일반해에 초기조건을 적용하여 상수 WSs 구한다.

40 061
이 연립방정식의 해는 < =1/5과 6 =-1/5이다.
5. 일반해에 이 상수 AS 치환하여 다음과 같이 SPAS 구한다.



===== PAGE 586 =====
@0 00000 0
576     appendix ㅁ 재현식의 해 구하기: 재귀 알고리즘 분석

00

* 예제 89 피보나치 순열을 생성하는 다음 재현식의 해를 구해보자.

ta aaa SU =0     (n> 19°] 34)
ino
sl
1. 특성식을 찾는다
ty 애기 90 =
^ =0

2, 특성식의 해를 구한다.
이 8차방정식의 해를 구해보면, 근은

「

3. 정리 BIS 적용하여 재현식의 일반해를 구한다.

이

4. 일반해에 초기조건을 적용하여 상수 WSS 구한다.

Cian          C—O)
a+ a Gel
이 연립방정식의 해는 < =1/ V5 과 6 =—-1/ V5 이다.
5. 일반해에 이 상수 BS 치환하여 다음과 같이 특정해를 구한다.
_ (a+ v5)/2"-[a— 95721"
"                v5

a)

t

비록 예제 8.9에서 7번째 피보나치 항을 구하는 공식을 명백히 얻었지만 실용적인 가
치는 전혀 없다. 왜냐하면 no] 증가함에 따라서 VFS 나타내는데 필요한 정밀도도 증
가하기 때문이다.

정리 8.1에서 특성식의 모든 《개의 근이 서로 달라야 한다고 했다. 따라서 이 정리에
따르면 다음과 같은 특성식은 허용하지 않는다.



===== PAGE 587 =====
* 예제 810

@‥00@00000 0
B2 특성식을 이용하여 재현식의 해 구하기 577

(r—1)(r—2)? = 0

항 - 2가 세제곱이 되었기 때문에, 여기서 %는 방정식의 3번 중복된 근(006 of mul-
tiplicity 9/이라 부른다. 다음 정리는 중복된 ZS 가질 수 있도록 허용한다. 이 정리의
증명은 이 부록의 끝부분에 있다.

> Bel] 8.2

r& 상수계수 동질 1차 재현식의 특성식의 mel 중복된 근이라고 하자. 그러면, 다음은 모두
이 재현식의 해가 된다.

2 7   00, 고 =m lye

00 /1  = nm  =    =
수아 시루. 92028 t,=n

그러므로 이 해들의 BS 각각 재현식의 일반해(정리 8.1에서 주어진 대로)에 포함된다.

이 정리의 적용 예제는 다음과 같다.

다음 재현식의 해를 구해보자.

t, 0 +15t, »—-9t,-3 =0 (06>0의면)

|
1
sed
tllo
ye
lr
cu

ty — Tt, 1 +15t, 5 —9t,_3 =0

rP—7r+15r—9 =0
2, 특성식의 해를 구한다.
중복
'
r — 7 +15r—9 = (r—1)(r—3)? = 0

이 방정식의 근은 7=1과 7=3이고, 7=3은 2H 중복된 근이다.
3, 정리 8.2를 적용하여 재현식의 일반해를 구한다.

t, =c1" +¢,3" +¢,n3”

여기서 3°} 7#"항이 포함되어 있는 이유는 30] 9번 중복된 근이기 때문이다.
4. 일반해에 초기조건을 적용하여 상수 BSS 구한다.

&%@=0=010+6.30+6(0)(30)



===== PAGE 588 =====
0 0 0000 0
578     appendix 8 재현식의 해 구하기: 재귀 알고리즘 분석용

* 예제 B.11

t, =1=¢,1!+¢3' +¢,(1)(3')
tp =2=¢,1? +3" +c, (2) (3?)
간략화 하면,
Cy +e,    =0
¢ 3g 3G, =1
여그96 71806 = 2
이 연립방정식의 ARS  =-1, 6=1과 ㅎ=--
5. 일반해에 이 상수값을 치환하여 다음과 같이 특정해를 구한다.
1
t= (-1)0") +0)(8") +(- 2] (ns)

=—14+3"—n3""!

다음 재현식의 해를 구해보자.

ty —5ty—y+7ty_9—3t,-3 =0 (04 >?2이면)

1!
ox
Bes
tho
a
clr
a,

t, — Sty; + Tt,» —3t,_3=0

r—5r'+7r—3=0
2. 특성식의 해를 구한다.

J
o:

Pf —5r? + 7r—3 = (r—3)(r—1)? =0
이 방정식의 큰은 *=8와 7=1이고, r= 2 중복된 근이다.
8. 정리 B.2S 적용하여 재현식의 일반해를 구한다.
80078 +o,
4. 일반해에 초기조건을 적용하여 상수 값들을 구한다.
i =1=¢2°+e,1°+e,(0
t, =2=c,3' +e1' +e(1)(1')
tp =3 =c,3? +1? +¢,(2) (17)

)(1")
)

간략화 하면,



===== PAGE 589 =====
000000 0
용하여 재현식의 해 구하기     579

ies)
ine}
Jim
0x
Iz
jo
a
010

de, tegte, =2
9c, +e, +2c, =3
이 연립방정식의 해는 4 =0, — =15} 6ㅋ1이다.
5. 일반해에 이 상수값을 치환하여 다음과 같이 특정해를 구한다.
t, = 0(3") +1(1") +1(n1")
=1+n

B.2.2 HIS 1차 재현식

정의
=
“《와 @,항이 상수이고 f(n) 이 영함수(26(ㅇ 140예00)가 아닌 함수일 때, 다음 형태의 재현식은
상수계수 비동질 1차 재현식(「1077090606046 linear recurrence equation with constant co—
efficients)0|2} 한다.

이가 =f(n)

여기서 영함수란 f(n) = 0임을 의미한다. 영      사용한다면 동질 1차 재현식이 될
것이다. 비동질 1차 재현식을 풀 수 있는 일반적인 방법은 알려진 a] 없다. 흔한 특수경우
인 다음 방정식을 푸는 방법을 전개해보자.

gt, + a,t,—1 +--+ at, ~~ = 0200                         (B, 2)

여기서 b= 상수이고, p(n)-= nol] 관한 다항식이다.

*예제 812 다음 재현식은 k=1, 0=4, 그리고 p(n) =1일 때 재현식 8.2의 예이다.

t, — 3t,_, =4"

* 예제 813 다음 BAAS k=1, b= 4, 그리고 202) =8n+79 때 재현식 B29} 예이다.
t, —8t, 1 =4"(8n+7)

재현식 B29} 같은 특수한 BOL 다음 예제와 같이 동질 1차 재현식으로 변환하여 풀
수 있다.


===== PAGE 590 =====
@‥@000000
580     appendix ㅁ 재현식의 해 구하기: 재귀 알고리즘 BAS

a

*예제 B14 다음 재현식의 HS 구해보자.

이 재현식은 우변에 쏘이 있으므로 동질이 아니다. 그런데 다음과 같이 그 우변을 제거할 수
있다.

1. 원 재현방의 을 ㅡ1로 대체하여 우변을 로 만든다.

2. 원 재현식의 양변을 4B 나누어서, 또 다른 방법으로 우변을 "로 만든다.

i, Sha

4    4
3, 원 재현식은 반드시 위의 두 식과 같은 해를 가져야 한다. 그러므로 이 두 방정식의 차

두
(difference) 반드시 같은 HS 가져야 한다. 즉, 1단계에서 얻은 방정식을 단계에서 얻은
방정식으로 빼면 4” ' 항을 없앨 수 있다. 그 결과는 다음과 같다.
0
4 4

= 471

+3t,_» =0

t, — Ty, +12t,_, =0

2c:
i
ae
rlo
에
nw,
x
ea
rat
ee
aC;
&
ils
od
ay
w
tip
2
ofo
pol
ee
떼
+
ee
더
rr
>A
cd
=
요
이
~
고

r—Tr+12=(r—3)(r—4) = 0
다음과 같은 일반해를 구한다.
3 = 이 oA”

초기조건 = 0과 , =4를 사용하여 다음과 같은 특정해를 구한다.

FE

그리

6 =407ㄴ4(3")

예제 8.14에서 일반해는 다음과 같은 Bos 구성된다.
c,3" ZT} c,4”

첫째 항은 재현식이 동질이었다면 얻게 될 특성식에서 온 것이고, 두 번째 항은 재현식이
비동질적인 부분, 이름하여 에서 온 것이다. 위 예제에서 다항식 7(7)은 1이다. 이렇지
않을 경우에는 재현식을 동질적으로 변환하는 작업은 더 복잡해진다. 그러나 결과로 나



===== PAGE 591 =====
© 예제 8.15

B2 특성식을 이용하여 재현식의 해 구하기     581
온 동질 1차 재현식에 대한 특성식의 po] SRS 줄뿐이다. 다음 정리는 이 결과를 나타
낸다. 이 정리의 증명은 생략할텐데, 증명절차는 예제 8.14와 유사하다.
정리 B.3
다음의 형태를 가진 비동질 1차 재현식은

Agi, 이 -1 01117 0, = 0 p(n)

다음과 같은 특성식을 가진 동질 1차 재현식으로 변환할 수 있다.

(00 +” Pa sta.) (r— pet = 0

여기서 d= p(n) 2} 차수(008168이다. 이 특성식은 두 부분으로 구성되어 있음을 주목해보자.
상하는 동질 Ao 대한 Sa

1. 상응
2, 재현식의 비동질적인 부분에서 얻어낸 항

우변에 #'2(00)과 같은 항이 두 개 이상 있다면, 여기의 각 항이 특성식에 항 하나씩 만드는데

기여하게 된다.
이 FAS 적용하기 전에 다항식 2(0)의 차수는 /,의 가장 높은 승수가 된다. AS
들면,
다항식                  하수
p(n) = 3n?+4n—2         2
p(n) =5n+7               1
p(n) =8                    0

이제 정리 8.8을 적용해보자.

다음 재현식의 해를 구해보자.

2 -838 , =4"02271)     (2 > 1이면)
t) =0
i, =12
1. 상응하는 동질 재현식에 대하여 특성식을 구한다
6 -8% ,=-0
r'=3 =0

2. MAAS] 비동질적인 부분에서 BS 얻는다.


===== PAGE 592 =====
582   appendix 8 재현식의 해 구하기: 재귀 알고리즘 분석용
d
{ㅣ
4” (2n' +1)
t
b

* 예제 B.16

비동질적인 부분에서 항은 다음과 같다.
(7-7)01 — (r—4)1*1
3, 정리 BIS 적용하여 위의 두 단계에서 얻어진 항의 곱으로부터 비동질 방정식에 대한 특성식
구한다. 그 특성식은 다음과 같다.

(8 -8)(>-4)?
특성식을 구한 다음에는 동질 1차 식의 경        동일하게 진행한다.
4. 특성식을 푼다.

(r—3)(r—4)? =0
근은 r=39 *7=4이고, r=42 2H 중복된 근이다.
5. 정리 BLS 적용하여 재현식의 일반해를 구한다.
t, =¢,3" 0640 0604"
여기서 모르는 변수가 3개인데 반해서, 초기조건은 둘 밖에 없다. 이 경우는 다음으로 가장
an 값의 재현식 값을 계산하여 또 하나의 다른 초기조건을 반드시 찾아야 한다. 여기에서
그 Be 이다. 다음 식과 t, =12를 가지고

3h =F (26 2+1)
다음과 같이 《,를 구한다.
t, =3X12+80=116

(6) 상수의 값을 결정하는 것과 (7) 일반해에 상수값을 치환하여 다음을 얻는 과정은 연습문제
로 미룬다.

=20(3") -20(4”) + 8n4”

다음 재현식의 해를 구해보자.
t, —t,-, =n—-1, 72>0에 대해서



===== PAGE 593 =====
© 예제 8.17

2, 재현식의 비동질적인 부분에서 BS 얻는다.

그 항은 다음과 같다.

3, 정리 8.8을 적용하여 위의 두 단계에서 얻어진 항의 곱으로부터 비동질 방정식에 대한 특성식
구한다. 그 특성식은 다음과 같다.

더

미키

~
0
as
2
ttlo

(r—1)? =0
근은 7=1이고, 이 근은 3번 중복된 근이다.

5. 정리 8.2를 적용하여 재현식의 일반해를 구한다.
시 =C1" +en1"+en71"

=e, t+qnten?

여기서 다음과 같은 초기조건이 27} 더 필요하다.
G Sy Lb =0 50 0
tp =t,+2-1=0+1=1

(6) 상수의 값을 결정하는 것과 (7) 일반해에 상수값을 치환하여 다음을 얻는 과정은 연습문제

fo}       되지
로 미룬다.

다음 재현식의 해를 구해보자.

t, —2t,_, =n+2", 4 >1이면
a)

1. 상응하는 동질 재현식에 대하여 특성식을 구한다.

ig—2t, . =0

a)

0

2, 우변에 항이 두 개 있는 경우이다. 정리 8.3에서 밝혔듯이 각 항은 다음과 같이 특성식 하나씩

1

esa Zac.


===== PAGE 594 =====
@0000000
584     appendix ㅁ 재현식의 해 구하기: 재귀 알고리즘 분석용

* 예제 B18

@                     @
J               J
n=(1")n!        OP (OP)?
t               t
b                    b

그 두 항은 다음과 같다.
a Ga
3, 정리 8.8을 적용하여 모든 항으로부터 특성식을 구한다. 그 특성방정식은 다음과 같다.
(r—2)(r—1)?(r—2) = (r—2)?(r—1)?
이 문제의 나머지는 연습문제에서 완성하도록 남겨둔다.

B.2.3 변수의 변경(치역 변환)
정러 BIS 적용하어 SF 있는 형태가 ord 재현식은 ASS 그 VAISS 수 있는 행태
로 변환하여 풀 수 있다. 이 기술을 적용하여 푸는 예제들을 살펴보자. 변환 전 재현식은
2710))으로 표시하고, 변환 후 재현식은 ,로 표시한다. 2102)은 *,과 의미가 같다. 즉,
An Bt Mn) 값은 유일하게 존재한다.

다음 재현식의 해를 구해보자.

T(n) = 12 \+1  (n>10]31, n& 29) 거듭제곱이면)

FO) =1

BAO 이미 귀납법을 사용하여 이 재현식의 해를 구했다. 하지만 변수 변경 기법을 설명하기
위해서 해를 다시 구해보자. 이 재현식은 7/3항 때문에 정리 8.8을 적용할 수 없다. 그 정리를
적용할 수 있도록 재현식을 다음과 같이 변환할 수 있다. 먼저 다음과 같이 놓고,

n= 다시 말하면 *=187
둘째로, ng ez 치환하면 재현식은 다음과 같다.

9k
ZO = r(2|41= Te Qe a1) x24                    (B.3)

pT 2)

= 1

변환 후 재현식은 정리 BBS 적용할 수 있는 형태로 되어 있다. 그러므로 정리를 적용하면 다음

=
과 같은 일반해를 구할 수 있다.



===== PAGE 595 =====
0000000
B2 SAIS 이용하여 재현식의 해 구하기 585

i, =c, +ek
변환 전 재현식의 일반해는 이제 다음과 같이 두 단계로 구할 수 있다.
1. 변환 후 재현식의 일반해에서 《,를 7((2")로 치환한다.
2(2“)=0ㅜ06
2. 위의 단계에서 얻은 식에서 는 7으로, 《는 lg nls 치환한다.
T(n) =0ㅜ087
일단 변환 전 재현식의 일반해를 구하면, 여느 때처럼 진행한다. 즉, 초기조건 70
                     구하고, 그리고 상수들의 값을 계산하여 다음 해를 구한다.
27(02)0=1+18 n

수 느
tho
»
ofp

*예제 819 다음 재현식의 해를 구해보자.

200) =921|흥 Jen 1 (n>1°]Z, n& 2의 거듭제곱이면)

T(1) =0

예제 8.8에서 귀납법을 사용하여 이 재현식의 해를 구할 수 없었음을 상기하라. 여기서 변수 변
경 기법으로 AS 구한다. 먼저 ngs 2s 치환하면

r= roar 2) at 1=27(2*"!)+2*-1

t, = 2t,_, +2*-1
정리 BIS 이 변환 후 재현식에 적용하면 다음을 얻는다.
ty, = c, +02" + c4k2*
변환 전 재현식의 일반해를 주는     두 단계를 거친다.
1, 변환 후 재현식의 일반해에서 를 7(2") = 치환한다.
T(2*) =e, +¢,2°+¢,k2*
2. 위의 단계에서 얻은 식에서 a nos, ke 18 7으로 치환한다.
2002) =a +entenlgn

이제 여느 때처럼 진행한다. 즉, 초기조건 7(1) = 0을 사용하여 초기조건을 두 개 더 구하고,
그리고 상수들의 값을 계산한다. 해는 다음과 같다.


===== PAGE 596 =====
@0@0 0000 0
586     appendix B 재현식의 해 구하기: 재귀 알고리즘 분석용

* 예제 8.20

다음 재현식의 해를 구해보자.

T(n) =r7(2)+19(2) (n> 1이고 n& 29] 거듭제곱이면)

TQ") =7 TOF) 418 (08 102                         (B, 4)

재현식 8.4는 다음과 같이 된다.

= ,+18(0“그)2

=, eld
=7t,_,+18(4*"")

18
= Tt; +4(8)

이제 정리 8.8을 적용하면 다음을 얻게 된다.
ty =C,7t, +c,4*
변환 전 재현식의 일반해를 구하는 다음 두 단계를 거친다.
1, 《,의 일반해에서 t,.S 7(2")로 치환한다.

T(2*) =¢,7* +c,4*

2, 위의 단계에서 얻은 식에서 WE 7으로, KE lg 7으로 치환한다.

초기조건 7(1) =08 사용하여 둘째 초기조건을 구하고, 그리고 상수들의 값을 계산한다. 해는
같



===== PAGE 597 =====
@00600000 0
6.3 치환에 의한 재현식의 해 구하기     587

@ B38 치환에 의한 재현식의 해 구하기

© 예제 B21

때로는 치환(64086+461020)이라는 기술을 사용하여 재현식의 해를 구할 수도 있다. 앞의
두 절에서 배운 방법으로 해를 구할 수 없는 경우 이 방법을 시도할 수 있다. 다음 예제들
은 치환에 의한 방법을 설명한다.

다음 재현식의 해를 구해보자.

t, = + (02>1이면

n

1

어떤 면에서 보면 치환은 귀납의 반대되는 개념이다. 즉, 에서 시작하여 거꾸로 진행한다.
t

n

= 170

여여 0000.

n-1

068 Fn 2

Te
ty =t, +2
4=1
그리고 각 AS 이전의 식으로 치환하면 다음과 같이 된다.
t,t, 170
로 002 01102
그 29000 24177 1770

Sete — 27721 170

=e pee 2101 12
= n(n+1)
i=l     기

마지막 등식은 부록 Ao} 예제 ㅅ.1의 결과와 같다.

예제 8.21의 재현식은 특성식을 사용하여 해를 구할 수도 있다. 그러나 다음 예제에서
다룰 재현식은 특성식을 사용하여 BS 구할 수 없다.

에

© 예제 822 다음 재현식의 해를 구해보자.



===== PAGE 598 =====
0000000
588     appendix B 재현식의 해 구하기: 재귀 알고리즘 BAS

7에서부터 거꾸로 진행하면,

2
소우 후
2
th-4  thot n—-1
2
t,-2=t,-3  n—2
2
t=t, +=
2   a   9
t,=0

2
ty = tat
2  2
=t, 9+  +2
a
2  2
a ae a
2   2  2  2
오 오고 ga a
2   2  2  2
=e al ae
=95 S29
2
여기서 마지막 근사 등식은 no] 작지 않은 경우에 성립한다. 근사 등식을 얻는 방법은 부록 asl

예제 &.9에 있다.

@ BA n& *(양의 상수)의 거듭제곱으로 하여 얻은 결과를 모든 noe 확장하기

이 장에서 공부하는 USS 1장에서 다룬 UGS 잘 알고 있다고 가정하고 설명한다.

《가 양의 상수이면 재귀 알고리즘의 경우 no] 밑수 >의 거듭제곱으로 되는 경우만 정
확한 시간복잡도를 바로 구할 수 있다. 밑수는 보통 2가 된다. 특히 분할정복 알고리즘의
경우는 더욱 그렇다(2장 참조). 직관적으로 7을 의 거듭제곱로 하여 성립한 결과는 모
Eno] 대해서도 근사적으로 성립해야 할 것이다. 예를 들어, 어떤 알고리즘에 대해서
n°] 29] 거듭제곱일 때 다음이 성립한다면,



===== PAGE 599 =====
B4 nS 4양의 상수)의 거듭제곱으로 하여 AS 결과를 모든 poe 확장하기     589
T(n) = 27218 72

모든 7에 대해서 다음과 같이 결론지을 수 있어야 할 것이다.

T(n) € O(nlgn)
보통 그렇게 결론지을 수 있는 것으로 판명되었다. 이제 그런 경우가 되는 상황을 공부해
보자. 먼저 정의가 몇 개 필요하다. 이 정의는 변역과 치역이 모두 실수인 함수에 적용되
지만 복잡도 함수(즉, 음이 아닌 정수에서 음이 아닌 실수로 가는 함수)에 대해서 기술한
다. 그 이유는 여기에서는 그런 함수만 취급하기 때문이다.

정의
7이 커짐에 따라서 복잡도 함수 f(r) 이 항상 커지게 되면, f(r) 은 엄격히 증가한다(61예\

increasing). 한다. 즉, n, > 이면, 다음 부등식이 성립한다.

f(r) > 700)

그림 8.1(8/의 함수는 엄격히 증가한다(좀 더 자세히 말하면 그림 B19] 함수의 변역은

(a) 엄격히 증가하는 함수           (6) 감소하지 않는 함수

>
>

f(n)                           f(n)

~                         n>
(c) 감소하지 않는 함수가 아님     (0) 궁극적으로 감소하지 않는 함수
                            i
f(n)                           f(n)

n>       n>

그림 8.1 4종류의

nol
4


===== PAGE 600 =====
590

appendix B 재현식의 해 구하기: 재귀 알고리즘 분석용

모두 음이 아닌 실수이다). 알고리즘 분석에서 다루는 많은 함수들이 음수가 아닌 7 값에
대해서 엄격히 증가한다. 예를 So], len, n, 7187, 7", 2"은 모두 no} Lo] 아닌 이
상 엄격히 증가한다.

정의
정으
7이 커짐에 따라서 복잡도 함수 f(r) 0] 절대로 작아지지 않으면,
성
=

i
(nondecreasing) 한다. 3, n, > 이면, 다음 부등식이 성립한다.

|

(n)2 감소하지 않는다

엄격히 증가하는 함수는 모두 감소하지 않지만 평평함을 유지하는16061 out) 함수는
엄격하게 증가함없이 감소하지 않는다. 그림 B1(b)2] 함수가 그런 함수의 예이다. 그림
83.1(0/의 함수는 감소하지 않는 함수가 아니다.

대부분의 알고리즘은 입력을 처리하는데 걸리는 시간이 입력크기가 커지더라도 통상
감소하지 않기 때문에 알고리즘의 시간(또는 공간) 복잡도 함수는 보통 감소하지 않는다.
그림 8.1을 보면 함수가 감소하지 않는 한 nS 의 거듭제곱으로 하여 얻은 분석 결과를
모든 noe 확장할 수 있어야 할 것 같다. 예를 들어, no] 29] 거듭제곱인 경우 /(2)의
값을 구했다고 가정하자. 그림 8.1(0)의 함수의 경우 2° = 8과 24 = 16사이에서 어떤 일
이 벌어질 수 있다. 따라서 8과 16에 있는 값을 가지고 8과 16 사이의 함수 작용에 대해서
결론지을 수 있는 게 하나도 없다. 그러나 감소하지 않는 함수 f (n)2] 경우 7 이 8<n
< 16 의 범위에 있으면, 다음과 같이 된다.

f(8) < 702) < 7(16)

그래서 29] 거듭제곱인 nol] 대한 /(7/)의 값에서 f(n)2] 차수를 구할 수 있어야 할 것
같다. 직관적으로 맞아 보이는 이 사실이 많은 부류의 함수에 대해서 실제로 증명될 수
있다. 이 사실을 말해주는 정리를 공부하기 전에 차수는 큰 값하고만 관계됨을 상기하자.
함수의 초기값은 중요하지 않기 때문에 정리에서는 함수가 궁극적으로 감소하지 않기를
요구한다. 다음 정의를 보자.

정의

정으

nO| ASO 따라서 복잡도 함수 /(7) 이 어떤 지점을 지난 후 모든 에 대해서 절대로 작아지
지 않으면, f(n) 은 궁극적으로 감소하지 않는다(63043 nondecreasing) 한다. 즉, n, >
ny > 이면, 다음 부등식이 성립하는 이 존재한다.

f(r) = f(ng)

감소하지 않는 함수는 모두 궁극적으로 감소하지 않는다. 그림 3.1@2] 함수는 감소하
지 않는 함수가 아니면서 궁극적으로 감소하지 않는 함수의 예이다. no] 62] 거듭제곱일



===== PAGE 601 =====
* 예제 8.23

* 예제 8.24

@00@000000
B4 nS 양의 상수)의 거듭제곱으로 하여 얻은 ATS 모든 /?으로 확장하기     591

b> 0일 때 함수 ~ nlgn, 은 모두 유연하다. lg nol] 대하여 이가 성립함을 보이자. 다
른 함수의 유연성은 연습문제로 해보도록 한다. 이미 언급한 바와 같이 lene 궁극적으로 감소
하지 않는다. 다음이 성립하므로 둘째 AE 만족한다.

lg(2n) =182+18 7 € O(lg n)

함수 2"은 유연하지 않다. 왜냐하면, 1장의 1.4.2절에서 본 차수의 성질에 의하면 다음이 성립한다.
2” & 0(4”)
따라서
2” =4”은 0(2")
에 속하지 않는다.

n°] 의 거듭제곱인          진 결과를 일반화 할 수 있게 해주는 정리를 이제 기술

경우 얻어
한다. SRS 이 부록의 끝부분에 나온다.

> 정리 8.4

b> 291 bE 정수라 하고, f(n)-S 유연한 복잡도 함수라고 하며, T(n) Se 궁극적으로 감소하
지 않는 복잡도 함수라고 하자. 만약 no] 》의 거듭제곱인 경우 다음이 성립하면,

T(n) © O(f(n))

다음이 성립한다.
T(n) 06000)

더구나, 위에서 OS “큰 OU, 04, "작은 0"로 대치해도 마찬가지로 성립한다.

n°] 의 거듭제곱일 때 7(0) € 6ㅇ(7(2))이다"라는 BS 6 에 대해서 평소에 성립하
는 조건이 n& 19 거듭제곱으로 제한되더라도 성립한다는 뜻이다. 정리 8.4에서 f(n)
이 유연하다는 추가적인 요구사항을 주목하라.
이제 정리 8.4를 적용해보자.


===== PAGE 602 =====
6000000
592     appendix B 재현식의 해 구하기: 재귀 알고리즘 BAS

}° 예제 B25 다음 재현식을 보자.

nn)=7(|2|) +1    (n > 10°])

이 29] 거듭제곱일 때 예제 8.18의 재현식과 같다. 그러므로 그 예제에 의해서,
T(n) =lgn+1 © O(lg n)        (n°] 22] 거듭제곱이면)
18 7은 유연하므로 정리 8.4를 적용하기 위해서 2'0))이 궁극적으로 감소하지 않는다는 것을
보이기만 하면 다음과 같이 결론지을 수 있다.
Tin) € O(lg n)
18 n+1°] 궁극적으로 감소하지 않는다는 사실로부터 T(n)°] 궁극적으로 감소하지 않는다고
결론짓고 싶을 지도 모른다. 그러나 no] 2의 거듭제곱일 때만 7(7,) =18 + 1이라고 알기 때문
에 그렇게 할 수 없다. 그 사실만 가지고 T(n) = 22] 거듭제곱 값들 사이에서 어떤 결과를 나올
지 장담할 수 없다.
n> 2인 nol] 대해서 21(42)이 궁극적으로 감소하지 않는다는 사실은 "1 < ^ <7이면, 다음 부
등식이 성립한다"는 사실을 귀납법을 사용하여 증명하면 된다.
T(k) < T(n)

HAA : -2이면

FO) 1,

T(2) = r| [2 | |1= T(1)+1=1+1=2

따라서

TO) & FO)
귀납가정 : 귀납가정을 만드는 한 가지 방법은 m 으 인 BE mo] 대해서 사실이라고 가정하는
것이다. 그리고 BAS} 마찬가지로 7+1일 때 사실임을 보인다. 여기서도 이런 식으로 해야 한
다. n& 2보다 크거나 같은 임의의 정수라고 하자. m < 인 모든 mo] 대해서 *<ㅠ이면 다음

이 성립환대:
T(k) <= T(m)

귀납단계 : 귀납가정에서 *<7일 때 다음과 같이 된다고 가정했기 때문에
T(k) < T(n)

다음이 사실임을 보이기만 하면 된다.
T(n) < T(n+1)
결국 7 = 1일 때, 다음과 같이 됨을 이해하는 AS 별로 어렵지 않다.

따라서 귀남가정에 의해서



===== PAGE 603 =====
증명이 완료되었다.

마지막으로 많이 쓰는 재현식의 차수를 결정하는 일반적인 방법을 개발해보자.

fr

> M2] B.S
복잡도 함수 Mn) & 궁극적으로 감소하지 않고 다음을 만족한다고 가정하자.

200 =aT(F}rent (n> 1013, ne} 09) 거듭제곱이민
T(1)=d

여기서 b > 2이고 k= 0인 0와 KE 정수이고, 4 > 0이고, ㅇ>0이고, = 0이다. 그러면,

O(n")  (a <#이면)
T(n) €4O(n'ign) (6=#이면)         (B.5)
O(n") — (a> vko] I)

더구나 재현식에서 다음 식을
T(n) =ar[2)+en!
다음 식으로 대치한다면,
T(n )<ar| 2 sent 또는 270) > 기브

B52] 결과가 © 대신에 "큰 OU NF 각각 성립한다.

특성식을 사용하여 일반 재현식을 풀고, 정리 8.4를 적용하여 이 정리를 증명할 수 있
다. 다음에 정리 B52] 적용 예제를 보자.

* 예제 8.26 T(n)°] 궁극적으로 감소하지 않고 다음을 만족한다고 가정하자.

a  bo 6k
} 를 !
2102) =87(n/4)+5n?  (42>이고, no] 8의 거듭제곱이면)
T(1) =3



===== PAGE 604 =====
06000000
594     appendix B 재현식의 해 구하기: 재귀 알고리즘 BAS

정리 8.5에 의해서 8<《^이므로,
T(n) € O(n’)

* 예제 B27 = T(n)o] 궁극적으로 감소하지 않고 다음을 만족한다고 가정하자.

a    b ok

i    6 ㅣ
T(n) =9T(n/3)+5n' _ (02 >1이고, n°] 8의 거듭제곱이면)
T(1) =7

정리 8.5에 의해서 9 >#'이므로,

T(n) € O(n) = O(n?)

정리 BSE 중요한 정리를 가능하면 간단하게 설명하기 위해서 도입한 정리이다. 그
Age 사실 다음에 나오는 정리에서 상수 를 1과 같게 한 특별한 경우이다.

> Be] 8.6

복잡도 함수 7'0/)은 궁극적으로 감소하지 않고 다음을 만족한다고 가정하자.

200 =a7(%}+ent (n> 20131, 7이 #의 거들제꼽이면)

Ts) =d

여기서 8는 62] 거듭제곱이고, 0 > 2이고 b> 0인 DF 《는 정수이고, 4 > 0이고, ㅇ> 0이고,

d> 0이다. 이런 경우에도 정리 B52] 결과는 성립한다.

 예제 8.28 2700)이 궁극적으로 감소하지 않고 다음을 만족한다고 가정하자.

a    b uk

{    bd
T(n) =87(n/2)+5n® (n> 64°] 31, no] 22] 거듭제곱이면)
T(64) = 200

정리 8.6에 의해서 8=ㅇ2"이므로,
T(n) € O(n’ lg n)

재현식을 푸는 기술에 대한 SRE 여기서 마친다. BASF (generating function) S



===== PAGE 605 =====
06000000
BS 정리의 증명   595

사용하여 재현식을 푸는 기술도 있다. 이 기술은 8010010988)를 보면 설명되어 있다.
Bentley, Haken, Sax(1980)2 분할정복 알고리즘(2장 참조)의 분석에서 발생하는 재현식
을 푸는 일반적인 방법이 나와 있다.

8.5 정리의 증명

다음 보조정리는 정리 BLS 증명하는데 필요하다.

ㅣ ~ 보조정리 8.1
다음과 같은 동질 1차 재현식이 있다고 가정하자.
At, + at, 1 +--+ at, , = 0
만약 이 다음 특성식의 뿌리라면,
0 tare} +, =0

다음이 그 재현식의 해이다.

증명 : i=n—k, .…, 7에 대해서 만약 재현식의 {를 t= 대치하면, 다음과 같이 된다.
애서 1 10908 7 = "(agri + 이이 버그 98)
= *(0)

0,
= 왜냐하면 re] 특성식의
뿌리이기 때문이다.

따라서 은 재현식의 해이다.

정리 8.1의 증명 1차 동질 재현식에 대해서 해에 상수를 곱하거나, 어느 두 해를 더하거
나, 모두 마찬가지로 재현식의 해가 된다는 ARIS 이해하기는 별로 어렵지 않다. 따라서
보조정리 8.1을 적용하여 다음과 같이 결론지을 수 있다.

만약 다음이 특성식 《개의 서로 다른 뿌리들이라면,

Ty, Uo. aes Ue
ce, Bo] 임의의 상수일 때, 다음은 재현식의 해이다. 비록 여기에서는 증명하지 않지만 이
들이 유일한 해답들이라고 증명할 수 있다.

 정리 8.2의 SY 중복 근 mo] 인 경우를 증명한다. 큰 7의 경우 일반화는 간단하다.
7, 을 중복 2의 뿌리라고 하자. 다음과 같이 놓자.

ㅇ


===== PAGE 606 =====
0000000
596     appendix B 재현식의 해 구하기: 재귀 알고리즘 분석용

20) = aor +ayr*"*+---+a, |특성식}

g(r) = r” *p(r) = 06 + 012 2 feet age

u(r) = 720 (r) = agnr” + a; (n— 1) +…+ a,(n— 0) 0^

여기서 g(r) 1차 미분을 의미한다. 만약 재현식에서 ir 를 《,로 바꾼다면, 407 )을 얻
는다. 따라서 40, ) = 0이라고 증명할 수 있으면, 《, = nr} S 재현식의 해라고 결론지을
수 있다. 따라서 이제 4, ) = 0임을 증명하자.

u(r) - 7000
= 7[0^ 7 "^)200]'
= rr" "p' (r) + p(r)(n— k)r™*~]
따라서 u(r,) = 0임을 보이기 위해서 70, )과 p'(r,) 모두 OF BSS 보이기만 하면
된다. 다음과 같은 절차로 이를 보인다. <, 은 특성식 p(r) 9] 중복 29] 해이므로, 다음을
만족하는 v(r)o] 존재한다.

p(r) = (r—r,v(r)
따라서
p (r) = (r—1,)?v' (r) + 20(r) (r= 14)
그리고 p(r,) zt p'(r,)°] 모두 0이다. 증명이 완료되었다.
} 정리 8.4의 증명 “큰 ("에 대한 증명을 해본다. 29} Ol 대한 증명도 비슷하게 할 수
있다. n°] 의 거듭제곱이 되는 모든 nol 대해서 T(n) € 0(/(1))이므로 n> N,°|aL
#의 거듭제곱이 되는 모든 7에 대해서 다음 부등식이 성립하는 양수 c, FS] 아닌 정
수 ^, 이 존재한다.

210) 스이 7020                             (B,6)
모든 양의 정수 *에 대해서 다음 부등식이 성립하는 유일한 《가 존재한다.
be <n< pet?                                (B.7)
유연한 함수의 경우 b> 2이면 다음과 같이 됨을 증명할 수 있다
f (on)EO(f(n))

즉, 만약 이 조건이 8에 대해서 성립한다면, b> 인 어떤 《에 대해서도 성립한다. 따라
A, n> “인 BE no] 대해서 다음 부등식이 성립하는 FO] 상수 <,과 음이 아닌 정수
가 존재한다.



===== PAGE 607 =====
연습문제     597
f (bn) < eof (n)
따라서 “> 이면, 다음과 같이 된다.
f(o'**) =f (0x d*) ㅋ6/(00)             (B.8)

Tn) fn) 둘 다 궁극적으로 감소하지 않기 때문에 m>n> 2, 인 경우, 다음 부
등식이 성립하는 이 존재한다.

T(n)< Tim) 그리고 f(n) < f(m)                  03.9)
ro] 너무 커서 다음과 같은 부등식이 성립한다고 하자.

b” > max(N,, Ny, 2)
만약 n> 《"이고 《가 부등식 8.7에서 no] 상응하는 값이면, 다음 부등식이 성립한다.
6 > or
따라서 부등식 8.6, B.7, B.8, 8.9에 의하여 7 > "인 경우, 다음 부등식이 성립한다.
T(n) < 20000 나 으히/(00 즈이) < een f (n)
이는 곧 다음이 성립함을 의미한다.
T(n)€ O(f (n))

연습

u
u

제

6.1절
1. 다음 각각의 재현식에 대한 해답후보가 맞는지 귀납법으로 검증하시오.

(a) t, =4t,_,      (n> 10°]A)
= 8
해답후보는 《, =8(4”')

(b) t, =t,_, +5      (n> 이면)
t, =2
해답후보는 t, =5n-3

(c) t, = +     (2 >1이면)
t,=1

해달후보는 《 = Mat


===== PAGE 608 =====
598     appendix 6 재현식의 해 구하기: 재귀 알고리즘 분석용
(8) t, <tr      (n > 1이면)
fe
해답후보는 = fae 1)
opt. + a CEST     (n> 1이면)
AGERE t, = mat

(f) t, =3t,_,+2" (0>1이면
=
해답후보는 $ =5(3”ㄱ1) - 9“!
(g) t, =3t,j+n (4 >1이고, no] 1의 거듭제곱이면)

4=o

해답후보는 《, = Zn —2n

(h) t, =nt,—4     (n > 0이면)
ty =1
해답후보는 t, =n!

2. 수열 2, 6, 18, 54, .…의 7번째 항에 해당하는 재현식을 쓰고, 해답후보 =, =2(#" ')이 맞
는지 귀납법을 사용하여 검증하시오.
3. 하노이탑 문제(장의 연습문제 17)에서 필요한 이동의 횟수(디스크 7개에 m, We 다음 A
현식으로 표현된다.
mM, =2m,-,+1     (n> 1°])
m, =1
이 재현식의 해가 m, =2"-19S 귀납법을 사용하여 증명하시오.
4. 다음 알고리즘은 배열 6에서 가장 큰 요소의 위치를 넘겨준다. 가장 큰 요소를 찾는데 필요
한 비교의 횟수 《,을 구하는 재현식을 작성하시오. 이 식의 해답이 《, =7-ㅡ1이 됨을 귀납법
을 사용하여 증명하시오.

index 2026 position (index 700, index high)

{

index position ;

if (low == high)
return Jow;
else {



===== PAGE 609 =====
position = 224 7205720002 (low + 1, high);
if (Sllow| > S{position))

position = low;
return position ;

}
}

최상위 수준 SSS 다음과 같다.
max_ position (1, n)

고대 그리스 ASS 다음 삼각형 수 같은 기하 모양으로 얻어낸 수열에 관심이 있었다.

ㅇ
0.00.000ㆍ

이 수열의 7번째 항을 구하는 재현식을 작성하고, 해답을 추측하고, 그 해답이 맞는지 귀납
법을 사용하여 검증하시오.

어떤 두 선도 서로 교차하되, 같은 AS 세 A 이상이 공유하지 못하도록 평면을 7/개의 선으
로 나누면 몇 개의 지역이 생기나? nie] 선으로 나눌 때 지역의 개수를 구하는 재현식을
작성하고, 해답을 추측하고, 그 해답이 맞는지 귀납법을 사용하여 검증하시오.

B(n,k)=("**)o] 다음 재현식의 해가 됨을 구납법을 사용하여 증명하시오.

Bin, 4) =B(n-1, k)+ Bln, k-1) (0 <ㅅ<7 이면)
B(n, 0) =1
Bin, 2) =1

다음 재현식의 값을 계산하는 알고리즘을 작성, 구현하고, 다른 문제 사례를 가지고 수행하
여 보시오. 그 결과를 가지고 이 재현식의 HS 추측해보고, 답이 맞는지 귀납법을 사용하여
증하시오.
= +00-1     (2 > 이면)
t,=1

B.24

9.

10.
11.

12.

Bl] 문제에서 재현식이 다음의 어떤 부류에 속하는지 밝히시오.

(a) 1차 Al(inear equations)

06) 동질 4](homogeneous equations)

(c) 상수 계수 4](equations with constant coefficients)

상수계수 1차인 8.1의 재현식 모두에 대해서 특성식을 찾으시오.

7(2)과 g(n)o] 둘 다 상수계수 1차 동질 재현식에 대한 해라면, c2 0가 상수일 때
ex f(n)+dxg(n)= 그러함을 중명하시오.

특성식을 사용하여 다음 ARIE] 해를 구하시오.

(a) t, =4t,_; —3t,_»      (n> 1이면)


===== PAGE 610 =====
0000000
600     appendix B 재현식의 해 구하기: 재귀 알고리즘 BAS

il
4, =i

(b) 4, =3t,_;—-2t,-2 +n’     (n> 1의면)
』=0
=

(c) t, =5t,_,—6t,_9 +5" = (n>1°) 9)
_=0
$=

(d) t, =5t,_,—6t,_. +n? —5n+7"    (n> 이면)
n    m2

13. 예제 8.15에 주어진 재현식의 HS 완성하시오.
14. 예제 8.16에 주어진 재현식의 HS 완성하시오.
15. 특성식을 사용하여 다음 재현식의 해를 구하시오.
(a) t, =66_-96_,      (02 >1의면)
pO
=

(b) t, =5t,_,—8t,_»+4t,-, (07>2이면

i =0
6 =
= 1
(c) t, =2t,-1-t,-g tn’ +5"      (n> 이면)
=O
im

(d) t, =6t,_, —9t,_9+(n?—5n)7”      (02 >1이면)

16. 예제 8.1/에 주어진 재현식의 해를 완성하시오.
17. 다음 재현식을

t, =(n-1)t,_,+(n-1)t,_»    (n> 2이면)
。 -0
£1

다음과 같이 S 수 USS 보이시오.



===== PAGE 611 =====
t,=nt,~+(-1)"®  (2>1이면
=o

18. AGE] 172] 재현식의 해를 구하시오. 해는 개 물체의 교란(0681780860601) 횟수를
준다(교란이 완성되면 아무 것도 제자리에 없다).

19. 특성식을 사용하여 다음 재현식의 해를 구하시오.
(a) T(n )=27[2}+1ogyn   (n> 1°31, n& 39] 거듭제곱이면)

00 Mn) =107|2}+n?    (@>1이고, n& 52] 거듭제곱이면)

2011=0
(c) nT(n) =(n-1)T(n-1)+3  (07>1이면)
KG) =o
(d) nT(n) =3(n—1) T(n-1) —2(n—2) T(n—2) +4”   (02 >1이면)
전비 에
T(1) =
(e) nT%(n) =5(n—-1) T{n-1) +n?   (n > 0이면)
T(0) =6
8.3절
20. 치환 방법을 사용하여 연습문제 1의 재현식의 해를 구하시오.
8.4절

21. 다음을 증명하시오.
(a) f(n) == 엄격히 증가하는 함수이다.
09 g(n) =2n?—6n?-& 궁극적으로 감소하지 않는 함수이다.

22. 모든 n 값에 대해서 감소하지도 않고 증가하지도 않는 함수에 대해서는 어떻게 설명할 수
있을까?

23. 다음 함수가 유연함을 증명하시오.
(a) f(n)=nlgn
00) g(n)=n* (kK > 0인 BE *이면)

24. 정리 BSS 사용하여 다음 재현식의 차수를 구하시오.

(a) T(n )=ar(2 62   (4 >1이고, 7은 5의 거듭제곱이면)

5

(b) T(n) =  sor(2  2    (42 >1이고, n& 3의 거듭제곱이면)


===== PAGE 612 =====
0000000
602   appendix 8 재현식의 해 구하기: 재귀 알고리즘 분석용

(c) 22127 )=167(2  + 까    (2 >1이고, 7은 3의 거듭제곱이면)
T(1) =1
2. 정리 BES 사용하여 다음 재현식의 차수를 구하시오.
(a) T(n )=ur(2  |   (n > 25이고, 7은 5의 거듭제곱이면)
T(25) = 60
00 T(n) =  a7(4 22   (n> 16이고, n& 4의 거듭제곱이면)
T(16) =50
26. 다음 재현식은
Mn)=a7(2}+o(n) (n> 19151, 7은 0의 거들제곱이면)
T(1)=d
g(n) © O(n) A a>cQl 경우 다음과 같은 해를 가진다.

다음과 같이 가정한다해도 위의 재현식이 같은 해를 가짐을 증명하시오.

> 108.인 경우, g(n) ㄷ 007)



===== PAGE 613 =====
appendix C

SAD 알고리즘(4.1.2절의 알고리즘 4.9)에서는 HHA 부분집합들(각 부분집
=a  합은 그래프의 Z 마디를 하나씩만 메베에 US 말미 모든 마디들이 같
은 집합에 속할 때까지 되풀이하여 부분집호              . 이 알고리즘을 구현하려면,
서로소 집합에 대한 데이터구조가 필요하다. aes aee 유용하게 S    5 다른 응용 응용 분야
도 많이 있다. 예를 들어, 4.3절의 알고리즘 4.4(마감시간 있는 스케줄 짜기)의 시간복잡
도를 향상시키기 위해서 사용할 수도 있다.
추상 Fo]E\ (abstract data type)= 데이터 객체들과 그 객체에 허용하는 연산들로
구성한다. ABA 집합의 추상 데이터구조를 구현하기 전에 필요한 객체와 연산을 명ㅅ
해야 한다. 구성요소의 전체영역(40176086) VS 시작한다. 예를 들어, 전체영역을
과 같이 놓 놓을 ~ 수 있다.

U=A, B, ©, D, 2}

그리고는 US| 멤버로부터 집합을 만드
서 서로소 집합은 다음 BSE 만들어0
for (each x € U)
makeset(x);
pt q7} set_pointer 타입이고, 다음과 같이 호출하면, 2 는 BS 포함하는 집합을 가리키
는 포인터가 되고, (는 CH 포함하는 집합을 가리키는 포인터가 되도록 타입 set_point-
@와 함수 finds 정의해야 한다.

는 프로시저 2244690/이 필요하다. 그림 2.108)에
다.

호 |

Pp = find (‘B’);
q = find (‘C’);

이것은 그림 0.1(8)에서 설명한다. 두 개의 집합을 하나로 합병하는 프로시저 merge
필요하다. 예를 들어, 다음을 수행하면,


===== PAGE 614 =====
@0@0 0 0 0 0 0
604     appendix C AA 집합의 데이터 구조

(a) 5개의 MBA 집합이 있다. p= find(B) Lt 0= /%10(ㅇ"을 실행하였다.

{A} {B} {ch {D} {자
t  t

2      q
(b) {B} 와 (CS 합병한 후에는 4개의 MBA 집합이 있다.
{A} {Bch {D} {과
(c) p= find(B) 3 실행하였다.
{A} {Bch 12} {과

i
2

그림 0.1 MBA 집합 데이터구조의 예

p = find (‘B’);
@ = 200 ('C’);
merge (2, q);

그림 C100) 있는 집합들은 그림 C10) 있는 집합들과 같이 되어야 한다. 그림 0.10)
에 있는 서로소 집합을 가지고, 다음과 같이 호출하면,

p = find (‘B’);
그림 CAC} 보여주는 결과가 나와야 한다. 마지막으로 두 집합이 같은지를 검사하는
루틴 00081이 필요하다. 예를 들어, 그림 Ciel] 있는 WHS 가지고 다음과 같은 호출

을 하면,
p = find (‘B’);
q = find (‘C’);
r = find (‘A’);

equal(p, 0)는 trueS 넘겨주어야 하고, equal(p, 7)은 falseS 넘겨주어야 한다.

객체를 전체집합의 원소들과 그 원소들의 서로소 집합으로 구성하고, 연산이 make-
set, find, merge, equal?) 추상 데이터타입을 명시하였다.

ABA 집합을 표현하는 한 가지 HHS 역 Hele|(inverted pointer)S 가진 트리를
사용하는 것이다. 이 트리에서는 뿌리마디가 아닌 마디의 포인터는 그의 부모마디를 가
리키는 반면, 각 뿌리마디의 포인터는 자신을 가리킨다. 그림 0.3(8)에서는 그림 0.18)의
서로소 집합에 상응하는 트리를 보여주고, 0.200)에서는 그림 0.100)의 서로소 집합에 상
응하는 트리를 보여준다. 이 트리들을 가능한 간단하게 구현하기 위해서 전체집합을 인
덱스(정수)만 구성한다고 가정한다. 전체집합으로 확장하려면, 그 전체집합의 원소에 인
덱스를 붙이기만 하면 된다. 배열 VS 사용하여 트리를 구현할 수 있다. 여기서, VI
각 인덱스는 전체집합의 하나의 인덱스를 나타낸다. 만약 인덱스 가 뿌리마디가 아니라
A, Uli Be 그 마디의 부모마디의 인덱스이다. 만약 인덱스 가 뿌리마디라면,



===== PAGE 615 =====
06000000
서로소 집합의 데이터 구조    605

8) 역 트리로 표현된 5개의 서로소 집합

800@00@

(6) [8]와 [이를 합병한 후 역

dh @@
©

그림 0.2 서로소 집합 데이터구조의 4 트리 표현

Uli] 2] BS :이다. 예를 들어, 전체집합에 10개의 인덱스가 있다면, 인덱스가 1부터 10
까지로 된 인덱스의 배열 Vol 저장한다. 서로소 집합에 모든 인덱스를  ae 위치시키
기 위해서 모든 에 대해서 다음과 같이 놓는다.
Oi] = 4;

10개의 ABA 집합의 트리 표현과 그에 ARS SHE 배열 BAS 그림 C3) HAS
다. SYS] 예는 그림 0.800)에서 보여준다. 집합 {사와 {1아이 합병되면, 100] 포함된 마
디를 4가 포함된 마디의 자식마디로 만든다. 이 동작은 110] =4z 놓으면 이루어진다.
일반적으로 두 개의 집합을 합병할 때, 어떤 트리가 뿌리마디에 더 큰 인덱스를 가지고
있는지 먼저 결정한다. 그리고는 그 뿌리마디를 다른 트리의 뿌리마디의 자식마디로 만
는다. 그럼 0.8(0/에서 여러 번 합병이 이루어진 후의 트리와 그에 상응하는 HSS 보여
준다. 이 시점에서는 3개의 서로소 집합만 있다. 이 루틴들은 아래와 같이 구현한다. 편
의상 다음 데이터구조와 크루스칼 알고리즘(4.1.2절)을 설명할 때 전체집합 를 SH]
파라미터로 열거하지 않는다.

『 서로소 집합 데이터구조 |

const int 2 = 전체집합이 가지고 있는 요소의 개수;

typedef int index ;
typedef index set_ pointer ;
typedef index universe[1 .. ] ;           // AAAS 1부터 2까지로 인덱스된다.

universe U;

void makeset (index 2)

{


===== PAGE 616 =====
@®eeeee 0
606     appendix C ABA 집합의 데이터 구조

이 i] ae ls
}
set_ pointer find (index /)
{
index /;
4 -
while (U[j] != J)
J= OF);
return /;
}
void merge (set_pointer p, set_ pointer q)
{
if (p < 9)                          // pa 합병된 집합을 가리는 포인터
Ula] = 2;                      // G= 더 이상 집합을 가리키는 포인터가 아님
else
012] = 9;                    if 0는 Waa 집합을 가리는 Ze]
// /는 더 이상 집합을 가리키는 포인터가 아님
}
bool equal (set_ pointer p, set_ pointer q)
1
ik (== 0
return true ;
else
return false ;
}
void initial (int n)
{
index /;
for (7 = 1; 7 <= n; H+)
makeset(i) ;
}

find(i) 호출에 의해서 넘겨진 값은 iS 가지고 있는 트리의 뿌리마디에 저장된 인덱스
이다. nA] 서로소 집합을 초기화하는 루틴 initial 포함하였다. 왜냐하면, 서로소 집
합을 사용하는 알고리즘에 종종 그런 Selo] 필요하기 때문이다.

서로소 집합을 사용하는 많은 알고리즘에서 7개의 ABA 집합을 초기화하고, 루프를
ml 돌린다/과 mo] 같은 같을 필요가 없다). 루프의 yoy equal, find, merge
루턴을 호출하는 횟수는 상수이다. 알고리즘을 분석할 때 초기화와 루프의 시간복잡도를



===== PAGE 617 =====
@0ㅎ00000 @
서로소 집합의 데이터 구조     607

8) 10개 MBA 집합의 SA 트리와 배열

5668668866

U[1] U2] 이] Uf4] U[5} Uf6} U[7] Ul[s] 09] Ufi0]

8)에서 집합 {4} 2+ {10}이 합병되었다. 10H mM 배열 SS 이제 4 AS 가지고 있다.

0606, 00000

1     2     3     4     5     6     >     8     9     4

061] - 이21] - 이] Uf[4] Uf[5} U6] U[7] Us] 09] 0010]

|m
wu
Jo
SA
Pa
mu
ni
ox
rol
n

(0) 여러 번 합병한 후 A 트리와 배열. 합병의

1     2     3     2     1     3     4     3     3     4

A

ri

U[1]   U[2]   U[3]   U[4]   U[5]   U[6]   U[7]   U[8]   0[9] Uf[10]
그림 0.3 MBA 집합 데이터구조의 역 트리 표현에 대한 배열

과 m2} 형식으로 BAD 필요가 있다. initial SEO] 시간복잡도는 명백히 다음과 같다.

상수를 곱해도 차수는 영향을 받지 SOUS equal, find, merge 루턴은 각각 루프를
ml 거치는 동안 한 번씩만 호출된다고 가정할 수 있다. equalth merger 상수시간에


===== PAGE 618 =====
@‥0@000000
608     appendix C AWA 집합의 데이터 구조

실행되는 것이 확실하다. find 함수만이 루프를 가지고 있다. 따라서 모든 호출의 시간복
잡도 차수는 find 함수에 의해서 지배된다. 최악의 경우 420에서 이루어지는 비교의 횟
수를 세어보자. 예를 들어, m= 5라고 가정하자. 다음과 같은 순서로 합병하면 최악의
경우가 발생하고,

merge({5}, {6});

merge {4}, {5, 6});

merge({3}, {4, 5, 6});

merge({2}, {3, 4, 5, 6});

merge({1}, {2, 3, 4, 5, 6});

각 합병 이후 finds 호출하여 인덱스 6S 찾는다(설명을 위해서 실제 집합이 merge
의 입력으로 표시되었다). 최종 트리와 배열은 그림 C40] 나와 있다. 최악의 Al find
에서 수행한 비교의 총 횟수는 다음과 같다.

2+34+44+5+6
이 결과를 임의의 moj 대해서 일반화하면, 최악의 경우 비교 REL 다음과 같다.
2+3+…-+ (0771 + 1) € O(m’)

함수 equal= 함수 440에서의 비교를 몇 번 수행하는지에 전혀 영향을 미치지 않으므로

\

함수 finde 62 가진 집합을

> 가리키는 포인터를 찾는데
6번 비교해야 한다.

J

1  1   2   3  4   5

이] Uf2] 이이 U4} US) 006]

그림 C.4 ㅠ=5일 때 서로소 데이터구조 !의 최악의 경우의 of



===== PAGE 619 =====
06000000
서로소 집합의 데이터 구조    609

—————
i                @          (4)
or

그림 6.5 새로운 합
마디로 만든다.

3
또
>

는 김이가 작은 트리의 뿌리마디를 다른 트리의

에다.

에서

뿌리마디의 자식

o}
한 결과로 나온 트리의 깊이가 그 트리 마디의 개수보다 하나 작으면, 최악의
다

이러한 경우가 발생하지 않도록 22080 프로시저를 수정하면, 효율을 증

시킬 수 있다. 각 트리의 깊이를 추적하고, 합병할 때 깊이가 작은 트리를 항상 자식마디
로 만들어서 그러한 최악의 경우가 발생하지 않도록 할 수 있다. 그림 0.5에서 이전에

합병하는 방법과 새로운 방법을 비교한다. 새로운 방법으로 깊이가 작은

트리가 나오게

된다는 사실을 주목해라. 이 방법을 구현하기 위해서 각 뿌리마디에 트리의 깊이를 저장

할 필요가 있다. 이를 수행하는 구현은 다음과 같다.

『 서로소 집합 데이터구조 ||

const int 2 = 전체집합이 가지고 있는 요소의 개수,

typedef int index ;
typedef index set_ pointer ;

struct nodetype

{


===== PAGE 620 =====
@00@000000
610     appendix C MBA 집합의 데이터 구조

index parent ;
int depth ;

}

typedef nodetype universe[1..] ;
universe U;
void makeset (index 1)

  21 i].parent = 1;
U| i].depth = 0;
i
set pointer find (index 2)
{
index ./ ;
I= 25
while (U[ j].parent != /)
j = U|j).parent,
return ./ ;
}

void merge (set_pointer p, set_pointer 0)
{
if (U|p|.depth == Uq|.depth) {
Up|.depth = U|p|.depth + 1;
Ulq|.parent = p;
}
else if (U|p|.depth < Uq|.depth)
Ulp|.parent = gq;
else
Ulq|.parent = p;

}

bool egua/ (set_ pointer p, set_ pointer q)

{

if (p == q)
return true ;
else

return false ;

}

void initial (int 22)
{

index / ;

for (72 = 1; 7 <= nm; H+)

// 전체집합은 1부터 #까지로 인덱스된다.

// 트리의 깊이는 증가해야 한다.

// 깊이가 작은 트리를 자식마디로 만든다.



===== PAGE 621 =====
@0000000
서로소 집합의 데이터 구조   611

makeset(1);

equal, find, merge 루턴을 호출하는 횟수가 상수인 루프를 mA 반복하는 동안 최악
의 경우 비교 횟수가 다음과 같이 됨을 증명할 수 있다.

적용 분야에 따라서 집합의 가장 작은 멤버를 빨리 찾을 필요가 있는 경우도
Al 구현을 사용하면 쉽게 할 수 있는데, 그 이유는 가장 작은 멤버는 항상 뿌리마디에
있기 때문이다. 그러나 둘째 구현에서는 꼭 그렇지 않다. 변수 smallestS 각 트리의 뿌
리마디에 저장해 놓고 가장 작은 멤버를 빨리 넘겨주도록 구현을 쉽게 수정할 수 있다.
이 변수는 트리에서 가장 작은 인덱스를 가지고 있다. 구현은 다음과 같다.

>MBA 집합 데이터구조 Ill

const int 2 = 전체집합이 가지고 있는 요소의 개수;

typedef int index ;
typedef index set_ pointer ;

struct nodetype

{

index parent ;
int depth ;
int smallest ;

hs
typedef nodetype universe[1.. 끼 ;        // AAAS 145 2까지로 인덱스된다.
universe U;

void makeset (index 2)

이기.        :
Ui|.depth = 0;
이기

'|.smallest = 1;                   // 인덱스 7만 smallest o|th.

void merge (set_ pointer, set_ pointer 0)
i
if (U|p|.depth == Ulq|.depth) {
Upl.depth = Ulg.depth +1; ——// 트리의 깊이는 증가해야 한다.
Ulq\.parent = p;
if (Ug|.smallest < U|p|.smallest)    // 0의 트리가 가장 작은 인덱스를 가진다.
Up].smallest = (이 .52247/69 ;


===== PAGE 622 =====
@00@00000 @
612    appendix C MBA 집합의 데이터 구조

else if (0/21.0606 < Uld.depth) { // 깊이가 작은 트리를 자식마디로 만든다.
Ulp|.parnet = q;
if (U[p|.smallest < U|q|.smallest)    // p2\| 트리가 가장 작은 인덱스를 가진다.
U|q|.smallest = Ulp].smallest ;
}

else {

Ulq|.parent = p;
if (U[g|.smallest < Ulp|.smallest) // q2| 트리가 가장 작은
Ulp|.smallest = U|q|.smallest ;

진

ch
ain

다

|
0!
그
ie

}
}

int .5222// (set_ pointer p)

{

return U[p].smallest ;
}

서로소 집합 데이터구조 와 다른 루틴만 포함시켰다. 함수 small 집합에서 가정
작은 멤버를 넘겨준다. 함수 small 상수 실행시간을 가지므로, equal, find, merge,
small FAS 호출하는 횟수가 상수인 루프를 mY 반복하는 동안 최악의 경우 비교 횟
AL ABA 집합 데이터구조 와 같다. 즉, 다음과 같다.
O(m lg m)

74 = 9}(path compression) °]2}31 하는 기술을 사용하면 루프를 mH 번복하는 동안
최악의 경우 비교 횟수가 mol] 거의 1차가 되도록 구현할 수 있다. Brassard} Bratley
(1988)>]] 이 구현이 설명되어 있다.



===== PAGE 623 =====
References

Adel’son-Vel’skii, G. M., and E. M. Landis. 1962. An algorithm for the organization of
information. Doklady Akademii Nauk SSSR 146:263-266.

Agrawal, A., N. Kayal, and N. Saxena. 2002. Not yet published. Available at
http://www.cse.iitk.ac.in/news/primality.html.

Akl, S. 1985. Parallel sorting. Orlando, Fl.: Academic Press.

Aldous, D., and P. Diaconis. 1986. Shuffling cards and stopping times. The American
Mathematical Monthly 93:333-347.

Apostol, T. M. 1997. Introduction to analytic number theory. New York: Springer-Verlag.

Baker, R. C., and G. Harman. 1996. The Brun-Titchmarsh Theorem on average. Proceed-
ings of a conference in honor of Heini Halberstam 1:39-103.

Bayer, R., and C. McCreight. 1972. Organization and maintenance of large ordered in-
dexes. Acta Informatica 1, no. 3:173-189.

Bedell, J., I. Korf and M. Yandell. 2003. BLAST, O’Reilly & Associates, Inc.

Bentley, J. L., D. Haken, and J. B. Saxe. 1980. A general method for solving divide-
and-conquer recurrences. SJGACT News 12, no. 3:36-44.

Blum, M., R. W. Floyd, V. Pratt, R. L. Rivest, and R. E. Tarjan. 1973. Time bounds for
selection. Journal of Computer and System Sciences 7, no. 4:448-461.

Borodin, A. B., and J. I. Munro. 1975. The computational complexity of algebraic and nu-
meric problems. New York: American Elsevier.

Brassard, G. 1985. Crusade for better notation. SIGACT News 17, no. 1:60-64.

Brassard, G., and P. Bratley. 1988. Algorithmics: Theory and practice. Englewood Cliffs,
N.J.: Prentice Hall.

Brassard, G., S. Monet, and D. Zuffellato. 1986. L’arithmétique des trés grands entiers.
TSI: Technique et Science Informatiques 5, no. 2:89-102.

Chacian, L. G. 1979. A polynomial algorithm for linear programming. Doklady Adad. Nauk
U.S.S.R. 224, no. 5: 1093-1096.

Clemen, R. T. 1991. Making hard decisions. Boston: PWS-Kent.

Cook, S. A. 1971. The complexity of theorem proving procedures. Proceedings of 3rd annu-


===== PAGE 624 =====
614

References

al ACM symposium on the theory of computing, 151-158. New York: ACM.

Cooper, G. F. 1984. “NESTOR”: A computer-based medical diagnostic that integrates
causal and probabilistic knowledge. Technical Report HPP-84-48, Stanford, Cal.:
Stanford University.

Coppersmith, D., and S. Winograd. 1987. Matrix multiplication via arithmetic pro-
gressions. Proceedings of 19th annual ACM symposium on the theory of computing, 1-
6. New York: ACM.

Dijkstra, E. W. 1959, A note on two problems in connexion with graphs. Mumerische
Mathematik 1:269-271.

——.. 1976. A discipline of programming. Englewood Cliffs, N.J.: Prentice-Hall.

Fine, T. L. 1973. Theories of probability. New York: Academic Press.

Fischer, M. J., and M. O. Rabin. 1974. “Super-exponential complexity of Presburger Ari-
thmetic.” In Complexity of computation, R. M. Karp, ed., 27-41. Providence, R.L.:
American Mathematical Society.

Floyd, R. W. 1962. Algorithm 97: Shortest path. Communications of the ACM 5, no. 6:345.

Fredman, M. L., and R. E. Tarjan. 1987. Fibonacci heaps and their uses in improved net-
workoptimization problems. Journal of the ACM 34, no. 3:596-615.

Fussenegger, F., and H. Gabow. 1976. Using comparison trees to derive lower bounds for
selection problems. Proceedings of 17th annual IEEE symposium on the foundations
of computer science, 178-182. Long Beach, Cal.: IEEE Computer Society.

Gardner-Stephen, P. and G. Knowles. 2004. “DASH: Localizing Dynamic Programming for
Order of Magnitude Faster, Accurate Sequence Alignment.” In Proceedings of the 2004
IEEE Computational Systems Bioinformatics Conference.

Garey, M. R., and D. S. Johnson. 1979. Computers and intractability. New York: W. H.
Freeman.

Gilbert, E. N., and E. F. Moore. 1959. Variable length encodings. Bell System Technical
Journal 38, no. 4:933-968.

Godbole, 3. 1973. On efficient computation of matrix chain products. JEEE Transactions
on Computers C-22, no. 9:864-866.

Graham, R. L., D. E. Knuth, and O. Patashnik. 1989. Concrete mathematics. Reading,
Mass.: Addision-Wesley.

Graham, R. L., and P. Hell. 1985. On the history of the minimum spanning tree problem.
Annals of the History of Computing 7, no. 1:43-57.

Gries, D. 1981. The science of programming. New York: Springer-Verlag.

Grzegorczyk, A. 1953. Some classes of recursive functions. Rosprawy Matematyzne 4.
Mathematical Institute of the Polish Academy of Sciences.

Hardy, G. H., and E. M. Wright. 1960. The theory of numbers. New York: Oxford
University Press.

Hartmanis, J., and R. E. Stearns. 1965. On the computational complexity of algorithms.
Transactions of the American Mathematical Society 117:285-306.

Hoare, C. A. R. 1962. Quicksort. Computer Journal 5, no. 1:10-15.

Hopcroft, J. E., and J. D. Ullman. 1979. Introduction to automata theory, languages, and



===== PAGE 625 =====
@00@00000 0
References            615

computation. Reading, Mass.: Addison-Wesley.

Horowitz, E., and 8. Sahni. 1974. Computing partitions with applications to the knapsack
problem. Journal of the ACM 21:277-292.

——. 1978. Fundamentals of computer algorithms. Woodland Hills, Cal.: Computer Sci-
ence Press.

Hu, T. C., and M. R. Shing. 1982. Computations of matrix chain products, Part 1. SIAM
Journal on Computing 11, no. 2:362-373.

——.. 1984. Computations of matrix chain products, Part 2. SZAM Journal on Computing
13, no. 2:228-251.

Huang, B. C., and M. A. Langston. 1988. Practical in-place merging. Communications of
the ACM 31:348-352.

Hyafil, L. 1976. Bounds for selection. SZAM Journal on Computing 5, no. 1:109-114.

Iverson, G. R., W. H. Longcor, F. Mosteller, J. P. Gilbert, and C. Youtz. 1971. Bias and
runs in dice throwing and recording: A few million throws. Psychometrika 36:1-19.

Jacobson, N. 1951. Lectures in abstract algebra. New York: D. Van Nostrand Company.

Jarnik, V. 1930. 0 jistém problému minimdlnim. Praca Moravské Prirodovedecké Spolec-
nosti 6:57-63.

Johnson, D. B. 1977. Efficient algorithms for shortest paths in sparse networks. Journal
of the ACM 24, no. 1:1-13.

Keynes, J. M. 1948. A treatise on probability. London: Macmillan. (Originally published
in 1921.)

Kingston, J. H. 1990. Algorithms and data structures: Design, correctness, and analysis.
Reading, Mass.: Addison-Wesley.

Knuth, 12. E. 1998. The art of computer programming, vol. IT: Seminumerical algorithms.
Reading, Mass.: Addison-Wesley.

——.. 1973. The art of programming, Volume IT: Sorting and searching. Reading, Mass.:
Addison-Wesley.

——. 1976. Big omicron and big omega and big theta. SJGACT News 8, no. 2:18-24.

Kruse, R. L. 1994. Data structures and program design. Englewood Cliffs, N.J.: Prentice
Hall.

Kruskal, J. B., Jr. 1956. On the shortest spanning subtree of a graph and the traveling
salesman problem. Proceedings of the American Mathematical Society 7, no. 1:48-50.

Kumar, V., A. Grama, A. Gupta, and G. Karypis. 1994. Introduction to parallel com-
puting. Redwood City, Cal.: Benjamin Cummings.

Ladner, R. E. 1975. On the structure of polynomial time reducibility. Journal of the ACM
22:)00r1 (1s

van Lambalgen, M. 1987. Random sequences. Ph.D. diss., University of Amsterdam.

Lawler, E. L. 1976. Combinatorial optimization: Networks and matroids. New York: Holt,
Rinehart and Winston.

Levin, L. A. 1973. Universal sorting problems. Problemy Peredaci, Informacii 9:115-116 (in
Russian). English translation in Problems of Information Transmission 9:265-266.

von Mises, R. 1919. Grundlagen der Wahrscheinlichkeitsrechnung. Mathematische Zeit-


===== PAGE 626 =====
616

References

schrft 5:52-99.

——.. 1957. Probability, statistics, and truth. London: George, Allen & Unwin. (Originally
published in Vienna in 1928.)

Neapolitan, R. E. 1990. Probabilistic reasoning in expert systems. New York: Wiley.

. 1992. A limiting frequency approach to probability based on the weak law of large
numbers. Philosophy of Science 59, no. 3:389-407.

——.. 2003. Learning Bayesian Networks. Prentice Hall.

——. 2009. Probabilistic Method for Bioinformatics. Burlington, Mass.: Morgan Kau-
fmann.

Li, W. 1997. Molecular Evolution, Sinauer Associates.

Papadimitriou, C. H. 1994. Computational complexity. Reading, Mass.: Addison-Wesley.

Pearl, J. 1986. Fusion, propagation, and structuring in belief networks. Artificial Intell-
igence 29, no. 3:241-288.

. 1988. Probabilistic reasoning in intelligent systems. San Mateo, Cal.: Morgan
Kaufmann.

Pratt, V. 1975. Every prime number has a succinct certificate. SZAM Journal on
Computing 4, no. 3:214-220.

Prim, R. C. 1957. Shortest connection networks and some generalizations. Bel/ System
Technical Journal 36:1389-1401.

Rabin, MO. 1980. Probabilistic algorithms for primality testing. Journal of Number Theory
12: 128-138.

Sahni, S. 1988. Concepts in discrete mathematics. North Oaks, Minn.: The Camelot Pub-
lishing Company.

Schonhage, A., M. Paterson, and N. Pippenger. 1976. Finding the median. Journal of
Computer and System Sciences 13, no. 2:184-199.

Strassen, V. 1969. Gaussian elimination is not optimal. Numerische Mathematik 13:354-
356.

Tarjan, R. E. 1983. Data structures and network algorithms, Philadelphia: SIAM.

Turing, A. 1936. On computable numbers, with an application to the Entscheidungs-
problem. Proceeding of the London Mathematical Society 2, no. 42:230-265.

. 1937. On computable numbers, with an application to the Entscheidungsproblem.
Proceedings of the London Mathematical Society 2, no. 43:544-546.

Waterman, M.S. 1984. “General Methods of Sequence Comparisons.” Mathematical
Biology, 46.

Yao, A. C. 1975. An O(|E|log log|V|) algorithm for finding minimum spanning trees.

Information Processing Letters 4, no. 1:21-23.
Yao, F. 1982. Speed-up in dynamic programming. SZAM Journal on Algebraic and Discrete
Methods 3, no. 4:532-540.



===== PAGE 627 =====
A
abductive inference 아아아아아아아아아이이이이이이이이이이이이아 258
[가이인닌인06000006 97
adjacent sree eee reeset eereseeteseeteeetenegs 98
adjacent sats he > eee 98
adversary argument ‘sssssssssssssssseeeeesen 348
algorithm srrstssssesessseseseeeeeeteeeeeseseeteeseneanens 2 3
빈이악어000000000000000000000000000000000007002 419
asymptotic lower bound cirrtttttttttttsetettstttttesseeeeeeees 31
aSyMptotic Upper Hound eters eee: 29
average—case time complexity '1110아아아사아아사사아아아아 20
AVL—ELE] 아아아아아아아아이아어이아이이이이시아이이어이이이아아이어 338

B-=E         cecccccccecccceecseescecee
backtracking
balanced tree

best-case time complexity analysis
binary fission POOP eee EOC ORC OCerrererrrrrrrrrrrrrrrrrrrr errr errr errr
binary search tree PoeeeeeCCOCOCeeeeerrreererrrrrerer errr eerie reer
binary tree eee reer eee rere reer rere rere er rere reer rere eee rere eee e eres
binomial coefficient Pore eree ree eeOeeeerrerrrrrrerr rrr rrrsy

Binomial theorem Peer eeeeePeCeCEeCeeeee reer eee rere rere er eee eee eee

bott om—up   Aenea eee eee eee e eee creer eee eee n esses sees eeeeeeeeeeeeeeeeeee

branch—and—bound eee eee rere rere re ere reer reer reer errr eer rr eer

candidate solution

canonical base pair, bp

ceiling

chromosome
CNF-Satisfiability

collision eee rere rere rere rere reer reer ee ere eee reer reer eee eee eer eres

combi nati (0) 9 Wetec

common logarithm

complete binary tree ……ㄴㅇㅁ00000000000000000000000000000000000000 287
complexity categories Peeee eee eee eee ee eee eee ee eee ee eee eee ee ee eee 26
complexity category
complexity function

comput ati onal     Cl compl exity   Sere rcceeececeeecceeecenceceecscees   7 0
constructive induction '9아아아디다이이지아 364, 539, 568
cost   Oe e eee eC CU SOO CEO SOOO COCOeererrerrrrre rrr rr rr rrr rr rrr errr reir r ris

crossing-over

cryptography

decision tree

deoxyribonucleic acid, DNA

deoxyribose tee eeeeceeees
depth-first search
deterministic algorithm eee eee eee eee rere eee
difference POOPeeere eee eee ee ere ee eee eee reer errr rere ree eee eee ree Tere ee
diploid cell
directed graph/digraph dence eee ee cece een eseeeeceeeeeeeeeeeeeees


===== PAGE 628 =====
0000000
618   BLO ft? |

Divide—and—Conquer 사이아아아아아사아아아아아아아아아아아 49, 61
DNA AS 정렬 waa've sate see ese hUSU ESOS SSS US ee veSees seep eseseseees 131
GOMAIN 이이아이이아이이시이 536
dynamic programming sss: 92

empty set
EPL: External Path Length reer reer errr rere eee ere ee erry 804
essentially complete binary tree st 288

every—case time complexity
Exchange Sort POeeee Eee Creer rrr erer terrier rrr errr reer rere er errr rere ees
expected value POeeer ee eee eee er OOrerrrrr rrr reererrerrrer errr rr rrrsy
exploitati OM) **8sttsssnseensesescsccnsascsssascescececcoscecsesesceoes
exploration deem eee eeeeeescecesescessseesesees

external    search  rere eee eee eee eee eee reece rere eee eee ee eee eee eee eee

heap rere eee eee eet eee eee treet eter errr reer rere terre rere rrr rere ess 이 88
heap  property eee eee e eter ere eee reer reer reer err sy 2 8 8
homologous  pair Pere eee eee eee eee eee eee eee ee eee eee eee eee eee eee eT 418

identity element °°

in—place Sort ‘teteettetetteeeeeeeeetees teense
increasing order ‘ttissssssesssssseessessneesseeeeseeeeny

a red Viel se2esses ses cscesseceeesececesnene: eecceseetesersretesrsties
induction

induction base PoPrer eee eeeeeeereree rere errr errr rere r rere errr rere rey 538
induction hypothesis Rescuwatene ccusereerseresasi ses dusns sens eee 538
induction 8662 ttttseteteseteeteteteteeeeseseseseeees 538
input size

insertion sort eee e ee eee reer errr terre rr rrrrrrr rere rrrrrrrrtrrrr triers 2022
instance PPO ere ree e eee errr reer errr errr rr rrr rr rrrr rrr reer rere r rere errr Ts 3
SPAT AYA Mio (5) Xo or one Ceo

internal search

intersecti (0) 0 Wey
inverse  el ement …ㄴ9009이이이이이시이이시000000000000000000000000000000000000 4 59
iterative algorithm

GENOME eerste eseses estes es eseseseeeseetetsteeaeeeeneneeeneeeaeaees 418
BeEnotype seers esses eects teaeeteneneeees 419
(어인보번했언으06606 418
greedy algorithm ECOL ORO OTT OTE IO TTD 143
Group theory 000000000000000000000000000000000000000000000000000000 459

Hamiltonian Circuits Problem eee e cece eee eceeeceeceeseees 220
haploid cell eee eee ee tee eee eet ere reer reer eer errr rere ere ere eres 418
hash function Seen e cece eee ee cece eee eeceeeseneeesseneeesseesseeeeeees 340

MIMD ereee eee eee eee eee eee eer rere eee ee eee reer reer e ee eer eee reer reer eres 510
Monte  Carlo  al gorithm eee rere rere reer rere eee eee er ere eres 206
mutation Pree eee eee tere eee eee ee errr eee rere errr errr reer errr eee ree errr es 419

7-여왕말 문제

natural  logarithms teen eeee cee ceeeeeeeeeeeeeeeeseeeeeeneeeeeenes 545
Natural    selection  See e cence eee e een eeeeeeeeeenseneeseseeeseeseseses  417
node oerreeeeeeee reer rere rerrrrerrrrerrrrrerrerrrrerrrrrrrrrrrrerrr rrr reir  115



===== PAGE 629 =====
open hashing Pere eee e eee ee eee eee eee ee eee ee eee eee eee eee eee ree Tere ee 340
optimal tree Pree e er terete rere rrerrererrrrerrrrrrer rire r rere T rere ers 119
optimal value sssrsssessssssesssessesssseesssesssseesseeeesees 97
optimization problem Sete cece ene e eee eee eee eeeseescesseeesseseees 97
order Dee e cece eee eee e ee ee renee eee e eee e eens seeee eee ee esses eeeeeseenseeneees 39
parallel computer 사아아아사사사사사사사아아아아아아아아아아아아아 510
parameter Boece cece ee en cece n eee eeeeeeee sense eseeeeseeeneeeeecenseeesseees 3
path Dene ene cence rene nee ene eee seen eee ee esses sees esses see eeseseeeneneeeeees 96
permutation See e eee eeeeeceeeeeeseeeseeesreseseeeeeeeeeeees 277, 550
phenotype Dee meee eee cere eens ence ee seen sense sees esses eeeeeeeeeeeereees 419
phosphate strsssssssssssseseseseseeesseeesesssssesseessessssess 131
planar graph teen ence ence e reece eee e eee eeeseeaseeeeeeeeeeeesesseseees 216
polynomial Deen eee e eee e eee eee en ee ee eee ee sees essen eeeeeeeeneeeeneesees 876
polynomial—time algorithm dee e cece ee ceceseceseeeeseseeeeee 376
polynomial-time many—one reducible 99010 392
population eee eee e eee e ene e ee en ee een reese esses eee eseseeeseeeeeeeeeeees 552
PRAM Dee e eee e eee e teen teen eset eee e sees sees ee esee eee eeeeeseeeeeeeeeeeeees 510
preorder Pee cece e rece teen eee e ee ee eee eeeeeeeseseeeeeeeeeeeseseseseeersees 194
probabilistic algorithm doce cece cccncccccccccscccccccsescceoes 206
probability function eee eee eee ee eee eee ee eee eee ee ree ees 553
probability space 1사아사사사아사사사사사아아사사자아아아아아아아아 553
이인민긴히00000000000000000000000000000000000000000000000000 98
promising function Bence meee cece cence cece ee eeseesessesesseesseees 197
proof by contradiction Dee e eee e cece seceeceeeeceseeeeeeeeseseeees 33
proper subset eee eee eee eee ee eee ere eee eee eer eee ees 548
quadratic—time algorithm eee c cece cece cee eececcceccceseeseeeees 25

0000000
찾아보기   619

recurrence equation steerer:
recursive algorithm svete eee: 567
recursive property rts 92, 105
relative frequency approach ‘tte 555
right subtree 사아아아사사아사아아아아아이아아이아아아아사어아사아아사 115
이이 배서00000000000000000000000770 115
RSA 공개키 암호체계 609000000000000000000000000000000000000000 500

sample space
search  key Seem cece eee nee e neces ee eeeeeeeeeeeeeeseeseseeseseeeseeesees

search time

second-largest key reer eee rere rere eee reer r errr ree er err errr ey 352
selection procedure Peer eee reer rere eee eee eee eee eer ee eee rere ees 144
selection 014 Foo 275
sherwood algorithm rere errr teeter eee eter rere errr er errerergy 366
SIMD cece cece cece ence n ec ee cee e ee ee eee sense nese eeenseeeseenceeeseeseeenee 510
simple path eee ee eee errr eee etree reer ere etre errr errr e eer errr errr ess 97
solution eee eecce cece eee e eee eecen cen sccecceeeeeeeeeeeseeeeneeseneeeesseneee 38

solution check

somatic  cell eee ence cence enc eecceneeeeneeeeeen seen eeeneeeesseneeeseee 418

tail—recursion

time     complexity    analysis   Perret eee eee eee eee eee eee ee eee eee yy   al 8
Tournament     method   Peer reer rere ere eee reer eee eee rere ee ee eee   85. 3
travel ing    Ss al eswoman    probl (900 ee   12 4.
two-way    merging   eee rere rere reer errr e reer rere rere rere eee rere   5 4.


===== PAGE 630 =====
@0000000
620   찾아보기

weighted graph
worst—case time complexity 00000000000000000000000000000 20

0=1 배낭 채우기 문제 se eeeeeeenseeeeeeeeeees 181, 223, 384
1차시간 알고리즘 SO 25
2차시간 알고리즘 이이 25
[조준 크기000000000000000000000000000000006 338
3차시간 see neeeeescecenenenenceeeenseeesesesesesesceseeseeeeeeseseseeees 98

THEY sossesseesssseeesseessseessseesssneesssseesneessnessseeeesnneessy 418
가중치 이아099000000000000000000000000000000000000000000000000000000000 96
가중치포함  그래프 이이 96
가지 친  상태공간트리 아이 196
가지 친다 000000000000000000000000000000000000000000000000000000000000000 196
감수분열  모세 느0000000000000000000000000000000006 418
감수분열 11111111011001011110011000000 419
Zhe 9909000000000000000000000000000000000000000000000000000000000000000000000 97
개발 이이이1000000000000000000000000000000000000000000000000000000000000 421
개체 이이아이00900000000000000000000000000000000000000000000000000000000000 420
개체군(집단) Case eee ecneeeaeeeeeeeseeeescesesessesessesaseesaseseeeaes 417

듭제곱 이이이이000000000000000000000000000000000000000000000000000000 544
거의  완전한 이진트   edb rce tances secjmeses Seeeeevacseasees es 324
건설귀납 Poe Eee ee ee ee ereeeererrereerer rere erreeeerer rere eereerey 364
검색문제 …이시시시00000000000000000000000000000000000000000000000000000 319

검색시가 에여어어어아아가사어에애아아사아아아이아아아이이어아아아아아사사 117
검색키 Pee eee eee eee eee er ere eee eee eee eee eee eee eee reese 116
게놈 00000000000000000000000000000000000000000000000000000000000000000000 418
결정  알고리즘 Peereeeeeeeeeeer ee eerereereree ree er rereeeererrerereryy 206
결정트리 sseeceesescsccascesscscscscsesescscsccesesessscscsesesescscsons 300
결합그래 TL. stsscescescescsccseessessesenssnsessecsscnsensesseseeeoees 429
경로 아이0000000000000000000000000000000000000000000000000000000000 96,  147
경로의  길이 Shep tas tps apedshs tude sesieeaclooscccbeuesesbeaestssseterens: 97
계산복잡도 SPREE eer Sree eerererereerereereree errr ee eereee 270
TWF] ssssssesssssseecsssssesssssseessssesssssnesssssneesssnsesssneees 499
공개키 암호체계 ………어어어아아아아아아아아아아아아아아아아아아아 499
공약수 dee aee ee eeneeeeeneeeeeeneeeeeeneeeeeeeeaeeneeeaseeeeeeeeeeeeeeees 446
공집합 Sree eee eee eee eee ee eee rere eee e reer reer eee eee errr errr es 549
교집합 Pere eErEEereeererrrerererrerererereerrrreeer rer rereereereei ri eie) 548
교차 PPerereereerererreerreeeeeeererreerrrrrreeeeerer reer reer reece eee ee 419
교환정 렬 ce ee eee neeaencenenssaenenseneensssenenecaeseessnesssacnssnceaceeees 0
구아닌(@) 외터바태타대디비내시며기티대 태에 131
귀납가정 …여아어어아아아아아아사아아아아아아이아아이이아아아아아아아아에 538
귀납기초 PPP EE SSeS eee e eee eee eee eee reer ee eee eee eee eee 538
귀납단계 0000000000000000000000000000000000000000000000000000000000000 538
귀납법 PPPEeEeeereeeeererereerrrrerrererrer rere erred 14
균형  잡힌  트리 0000000000000000000000000000000000000000000000000000 334
균형잡힌  트리 ee eeneeneseeeencenescesensescesnsensesonccscnecsoeeeees 115
그래프 see e ee eeeeeeeneeneeeeneneeseneeeeneeaeeeneeeseseeensenenseneaseeens 535
그래프  색 칠하기  이이이이이 216
그래프 색칠하기 문제 ……….아아아아아아아아아아아아 384
fa 459
그룹이 론 어아아아아아아아아아사아아사아아아사사사사사사아아아아사가 459
근사  알고리즘 pedebseecssevssnssbecescdccsuecsscvevecsosceseeceseees 405
기 대치 아아아아아아아사사사아사사사사사사아아아사사사사사사사사사사아아아 366
기대치(평균) ……아애어아아아아사사사사아아사아아아아사사사사사사사아아 561

너비우선검색 00000000000000000000000000000000000000000000000000000 238
뉴클레오타이드 tis diuistoleaicle eis sit'sieiesis eulsie cic estelenes clesctsseawlasvaeecas 418



===== PAGE 631 =====
다루기힘들다 ……아아어어아아아에에아에여에아아어에아아아아아아아아 377
다익스트라  알고리즘 se eeeereceacesescsesesescscscscnescsceseees 162
다중데이 터흐름 suseueeseeseucsslsevims seve csetdsssasecaseccsadeeses 510
다중명령 f= 흐름 아아아사아아아이아이아이아이이이이이아이아이아이이아아 510
다차시간 다일 축소변환가능 …………… 아아아 392
다차시간 알고리즘 cece eceeeecevesascasesscesceseececsscesenseens 376
다항식 seen eeneenee cence eee eeeseeeneeeeeeeeee eee eeeea een sassneeeceseeeeees 376
단세포 0009000000.0100000000000004000009000000000.000000004400669500046604600 418
단순경 그서이기아아다다다0000000000000000020 97
단순순환경로 Bielsis se sin av ¥eiea'beiesitineigns oeou sista seceslesea se remenemeres 148
단일데이터흐름 fg cawdis no epee sisisau'sepieeise cusses ideuccsisiteee careacs's 508
단일명 령흐름 Se vessnenseevercsssssateaseesererrnreeeneneraven 508, 510
단일출발전 점  최단경로  문제 007000000000000070000000000 161
대기 열 see eee eeeeeeeeneesneneeeeeeeeeeeseneneeseeeeeeneneeeeareesers 8247
대 립유전자 see ee ee eceeneeeneneeeeeneeeeseeeeeeeeeeeeeeeeeseeeteeenens 419
데 이 터   wW 렬  프로 그램 아아아아아아아아아아아아아아이이이이이이이 510
돌연변이 지키5비지티지서기 배스 419
동기성 eee reed ceousse \estetsccouscoancesseussecesecsaeresseeeuiessceon tes 511
동적검색 eee eee eee eee eer eer eer er er rer err errr eer eer Te 333
동적 계획 Wa At a ere KER RES TRE ENCE iene ecerTEUEn Eee 92
동종쌍 Diels sine sinlsicieria.sie ssicisisinivn'e'yn'ed sa lsle ovesede see seassseesassesessacss 418
동치관계 Beoisse passe ceess ees eee saescanesseeevseueuruars sosecasseseasas 462

추적 이아00000000000000000000000000000000000000000000000000000000000000 193
디옥시 리보핵산 see ee eee eneneeeeeeeeneneeeeeeeeeneseneeaeneererees 418

a.

리스트 see ceeeeceenceceaveseeeereneerevessseeseseseseneeseceeeersosoeeseseees 기
마감시간  있는 스케줄  짜기 다저 애대애어이아디이이사어기이 171
마디 Sage hyseesne coNsa tenseb tess sclescepsseesuessesssuemccqmcecescns 96,  115
마디의  깊이 비세 이리사이시지기011019시즈시지지니치시쉬치치스지스지시시티14121 115
마디의 수준 어여어어아아여아사아이아아어아이이아이아아이이이사아사아 115
WS AA} 문제 waa e cena eecncneesescensescscssssnssccsccessseccsceece 389
메모리(공    간)복잡도 이090000000000000000000000000000000000000000000 23
모듈러  거듭제곱     Wdee eee neeeeneeneeceneesesenseeeeeassassseaesasens 477
모순유        유도 증  즈며 Hy  bisisidslsleisles wens Wen Fe sun ides cecal 사이 33
모집단 09000000000000000000000000000000000000000ㄴㄴㅇㄴㄴ00660050609100000000 552
TEE seseseeeteeeeeesesenseneneneeeneeneneneeneneneeenesseenseseeeesenenees 447
몬테칼로  기 법 에000000000000000000000000000000060000000000000000000= 201

Haze  알고리즘 1“2166640010216티비이서지 시티 206

찾아보기        621
무작위 이10000.00054000000006590690616106.000000069690060000000000 557
문제 Pepec eat saeh ss tes oseiys des ceinete eaesseietonsesecserepeues erueeieesss cert 2
밑수 weisip siege. 4 61s 6154 seine olen oleiniis'nleib'ole as ee uielo'v vo se\eie's(s'elepluu sv esie elev ee.elewe 544

본질적으로 완전한 이진트리 아아아아아아아아아아아아아아아 288
부모마디  우선횡단 00000.1111111111111011111111111177 194
부모마디우선 eee seue tees su ussmerersuaersenesencsimisenesiares sete re 194
부모중간횡단 Sasiclst avec eeresssoacdbaseascosaerssustneesetteascesstes 333
부분그룹 이시01000000001000000000000000000000000000000000000000000000000 466
부분집합 cee ee eceeeceveceeneesscsesenessscsenesenessssscscseeescscsoness 548
부분집합의  합 구하기  FRA] creer 210
분기한정  가지 치 기  1] 비우선검색 eseceecsees soe eeeeeesess 238
분기한정 가지치기 최고우선검색 …………아아아아 238
분기한정법 sais ssl eleinive sien slu.snls'o ole os(oleNosins eye sine'sseSieivesivecieees 237
분자 이000000000000000000000000000000000000000000000000000000000000000000 418
분할정복 ……아아아아아아아아아아아아아아아아아아아아아사아에아아 49, 61
비결정  알고리즘 Se cca escobecobsacetee cvesesemeeccensucedesaac sees 387
비교만으로 정렬 도리사 체치비이이이이이디대매이니이디이에디이1 271


===== PAGE 632 =====
@0000000
622   찾아보기

비내림차순 …아어어아아아거어에아사사사아사사사사아사사사아사사사사아사사 9
4] uy) 7|  00000000000000000000000000000000000000000000000000000000000000000 499
비방향그래프 Te 147, 149
비순환적 아아아아어아아사사사아사아아사사사아사사사사사사아사사사 97, 148
비용 00000000000000000000000000000000000000000000000000000000000000000000 139
빠른 정렬 에아어아아어아아사아아새아아사아아이아이이이이이이아사사사사아사 62
버마     00000600000000000000000000000000000000000000000000000000000000000000이00 115
Hz]   이드  트리 saceeseesecsceccscsescscccesesccccscoscscenscccaecs 148
WE] EEO] A] 트리 ceeseseseeeeeeeteesteeeeseetetesesteteseetseescans 334
사건 Le ee nee ee nee en eee ee sence sensu eu eeeeeeeaeeneeu nese eens sense sense sens 552
삽입정 렬 ce ee ne ee eee eeeneenesennceseesscnsenseeensenssscncscensneesenene 979
상대빈도방식 …어어에아아사서서서사사아사사서사사사사아사사사사사아아 555
상용대수 여어아아어어아사사사사사사사사아사사사아사사사아아사사아아사사 544
상자 채우기 문제 …아아어어아아아아아아아아에아아아아아아아아에에 410
상태공간트리 00000000000000000000000000000000000000000000000000000000 195
상향식  접근방법 Saale SANG Nene US aN eC N AN eee eNEN NER ee seer vicesersese 92
생물체(유기체) ………아아아아아아아아아아아사아아에아아사사아아아아아 417
생식세포 태자 가타 418
생식체 …아아아아아아아아이아이이아이자이지이이이이이이이이서이서사아아 418
서로소 see ee eee ee ee eeeneneneeeeeeeeeneneenseeneeeeueueseneseseenseues 450
서로소 집합 cvreseeseeeeeeseeessseeeesssesessneesssneeesnneessees 605
선택과정 see eeeneece ee seesesaensescscenennencescssenccscesescnsenccsces 144
선택 정 렬  9000000000000000000000000000000000000000000000000000000004 275
세포 0000000000000000000000000000000000000000000000000000000000400000006000 418
셔우드  알고리즘 tbe eeeeenencecsssesacsceesssceceseecsceesesseeeees 366
소수분포함수 see ee ne eeeeeneeneeeeneneeeenseeeeeeeenseeeeseeeeeeeenee 480
수학적  귀납법 00000000000000000000000000000000000000000000000000000 537
순서 000009900000000000000000.0.0.004000.000000004000000000000090004000000000000 193
순서 가능집합 000000000000000000000000000000000000000000000000 115;  288
순열 아아아아아아아사사아아아아아아어아사이아이이기사사아사사아사 277, 550
순차검색 …여아아아아여어아아아아아아아아아아이어서어아아아사사사사사아아아 4
순환경로 00000000000000000000000000000000000000000000000000000000000000000 96
순환적 0000000000000000000000000000000000000000000000000000000000000000000 97
4] 정렬 saeeeeeeeee nescence nsec eeeeeeeasenenseseseaeaenenenensaeeeeeneneees 314
Fez 0이0000000000000000000000000000000000000000000000000000000000000 68
스케줄 짜기 …여어어아아아아아아서어에에에아사사사세사사아아아사사세 165
시 간복잡도 90000000000000000000000000000000000000000000000000000000000000 17
시 간복잡도  분석 00000000000000000000000000000000000000000000000000000 18
시토신(@) dene eeeneeeeneeeeneeneneenseeeneeeseeeeeeeeeseeseseasesenseaee 418
신장트리 0000000000000000000000000000060000이이이시이00000000000000 148

쌍방 합병 어어어아아사아사사사사사아사사사사사사사사아아사사사사사사사에 54
아테 넌(4) 아아아아아아아아아사아아아이아이이이이어사아사아아아사 131, 418
알고리즘 dese ee neeeeeeesensaeceeessascesessssasceceneasassecsscesooeees 2  을
암호학 Ses bdgueeeesoeseneuseesonetetiecsessecsSeesuivecsseevsenesesis teers 445
암호화 0006000009660600060000000000000060000000000000000000060000.0000000000 499
약수 rn oid oliarceatels sates ciaielteie sintente siecle sisiswisisaitiasioeiomiemaisinea tees trectegs 446
역 000000000000000000000000000000000000000000000000000000000000000000000000 543
역 원 000000000000000000000000000000000000000000000000000000000000000000000 459
연결되 어 00000000000000000000000000000000000000000000000000000000000000 148
열린해시 PPPS eeeer ee eereerereerererrerer rere eee eee eee eee) 340
열성 00000000000000000000000000006000000600000000000000000000000.00000000000 419
염 | 0009000000000000000000000000000000000000000000000000000000000000000 418
염색분 ㅣ 이0000000000000000000000000000000000000000000000000000000000000 419
염색체 야이이이0000000000000000000000000000000000000000000000000000019 418
오라클 000000000000000000000000000000000000000000000000000000000000000000 352
오른쪽하위트리 이아 eeaeeaeeeeeeaeeaeeueeeeceeceaeseeseeseeeeeeeeesees 115
오름차순 ……아아아에아아아아아아이아이아아아아이이이이이아시이이이이이이아사 2
오탄당 90000000000000000000000000000000000000000000000000000000000000000 418
올림수 000000000000000000000000000000000000000000000000000000000000000000 533
완전한 이진트리 a seeceesseeesesrenescseseesessecscseserevecsessees 287
외부검색 이00000000000000000000000000000000000000000000000000000000000 337
Fo) le Bo) 304
외판원 (비방향) 진위판별 문제 eects 396
외판원  문제 seca nena sence eeeeeeneneeeseeeeeeees 124,  249,  383
왼쪽하위트리 creer reteset eset seeeeees 115
우선순위 대기열 ……어어어어어어어사사사서서사사사사사사사사사사사 177
우선순위-쓰기  프로토콜 …아아아아아아에아아아아아아아아아이 527
우성 vies eens oniniposiesieisiiswsese sie dceyeaeienensssyecseniinhi wads ebersneses 419
원소 000000000000000000000000000000000000000000000000000000000000000000000 548
원소사건 PPE eE eee reCeree etree eerereerereerer eee eee eee ee 552
유망하다 여아아아어어에아사어사아사사사사아사사사아사사사아아사 154, 196
유망함수 000000000000000000000000000000000000000000000000000000000000004 197
유전  프로그래밍 Pree eeeereeereeeerer ee etree eee eee eee 433
유전자  부동 0000000000000000000000000000000000000000000000000000000000 420
유전자 아아어어사아서아사사사아사사사사사사사사사사아사사아아아아아아아아 419
유전자형 아아아아아사사사사사사사사사사사사사아아사사사사사사사사서사시 419
유전학 Av eeeees duis scuswerecsb ge buscweoes ses sveeessesnelcieinsieccses'sieis c's 417
오지  변이 060006010900000666100910066003163111010151시이지사시이시이이이이이 419
유클리드  알고리즘 …00900000000000000000000000000000000000000000 453
유효 하나 여아아아사서서사사사사사사사사사사사아아사사사아아사사사사사아 300



===== PAGE 633 =====
융합 doe eeeesesceeesencsesseceeseeesseessosesesseescsesnoneneeesesosneesoss 418
이배체 0000000000000000000000000000000000000000000000000000000000000000000 418
이배 체  생물체 Pee eee eee eerereeeeeeree ee eeeer rere ere rere 418
이배 체세포 se eeesceeevenceceesescneeecnseseeeessescesesenseeesenseesens 418
이분검색 sbeeecenescesencscscescnscncscencnssesscscsscseences 9,  51,  320
이분검색트리 …어여어어어어여여아아아아아아아아아아이이이이아사 115
이문열 Sala saucwicgisinwos sap su es ees ese saps <cosue ose sepeswesece ss cob seseauee 418
이음선 oss beseeedeecsecesscseecssseegecetebsvecdsocsvesseccseseessseccoecs 96
이 진검색트리  00000000000000000000000000000000000000000000000000 333
이 진코드 9시0000000000000000000000000000000000000000000000000000000 174
이 진트리 Wgblslessdecedcdecadsucdssescssctviccstescorsurscosceteccbesssees 115
이항계수 se eeeeecceccccsocscccseccssceescesesssccescessceesceeces 92,   552
이항정리 여어어어어서사아아사사사사사사사사사사새사아아아사사사사아아아 551
인산염 eee eee eee eee eer eee ree eer eee eee eee eres 131

일시적  이배체  감수분열  모세포 래 오오오 아우 이주0 418
일정  시간복잡도 이이아이사000000000000000000000000000000000000000000000 18
일정  시간복잡도 분석 oases Suede be esnselstvnseecsuecwusewesverevees 18
일주여행길 eee eee ee eee eee eee eee rere reer errr reer eee 124
임의-쓰기  프로토콜 아아아 527
OV 력사려| …아아아아아아아아아아사아사아아사사이이이이이이이아에 3
9] 력크기 ce eeeccecccescecscsecesesescscsescsensnssonesscosscsesess 12  378
잎 dt eeeeeeeseeeceecseeecnecececessencescssensensscescnccsesccccscoesoccecees 195
zx
자식마나 아아아아아여여여애사아아아아아이이이이이이어아아아아아아가아아아 115
자연대수 se ecncecscccscscscscscscsesescsesecescsesesescsccesseseesseces 545
자 연선 택 sessseseseesssssseesseessssesneessneessessneesseessseesseees 417
재귀 관계식 enc 92. 105
재귀 알고리즘 …아아여어어아아아 567
재현식 어아아아아아아아아아사사사아사아아이이이이이이이이이아아아아아아에 567
적 절성 검사 ee er ee  144
전체집합 eee eee ee eee eee eee eee ere eee eee eee eee eee eee 549
AYA] vores eeeeseesseeeeseeeeneessensseensnessesesneesseeesneeesseesssess 287
저 치코드 바이스 Spa aencasacses ales a a tases Oe ee ies 175
점근적인 상한 ………아아아아어어어어어에아아어어어아아아 29
점근적인 하한 veeveeeseseeseesseeeseeesseeesseessesseeesneesseeesses 31
접합체 Peereereeereeerer rere eer ererer errr er errr rer er eee eee ee 418
정 렬 000000000000000000000000000000000000000000000000000이00000 9
정 리 이000000000000000000000000000000000000000000000000000000000000000 542

0 00600000
찾아보기   623

정수론 ee ue oe veccevoscesteastuaeseceeceescwsseeetetwew sw eseewecwserssied 445
정자 eee eter eee Terre eer eree ere ee rer ee er eere er eereee er eee ee 418
정 적 검색 이히 b05Seseseoesasnsessayesseesstetssassassecesonss ss 333
정확성  부석 아아아아아아아아아아아어아사어아사이어아이이아이기사사아사어 24
제자리  정렬 nn se sinisin¥ suigis eisv.aveuen vein sinewesiseossiesvwessiswers 59,  271
조합 이9이9990900000000000000000000000000000000000000000000000000000000 551
준최적 이아이0900000000000000000000000000000000000000000000000000000 352
중립  원칙 Poorer eer eeeeeereeeeeerereereeeeeerer ere eee eee 553
지수시간 대비반 제시 애저1 98
지 정문 a eneeccncscsccscccccccvcsccccccsscccsccccesecesscsacscscsscccssorcses 18
직관적  귀납법 ee 539, 568
직 렬  컴퓨터 아아 00177107.07077, 00700 508
진부분   룹 pdeedartceaeesrarwecscorsrcsoncmreneedsnoieesissttesssenes 466
진부분집합 이000000000000000000009000000000000.000000000000000000.0004 548

최고우선검색 ……여여어어에에아아어서에에에아사사세세에에아아아아아아 244
최단경로 알고리즘 아아에아아아사아사사아사아사사아사아사사아사어 96
최대공약수 Boece ease evovete cscs ees ssucas= te ovetsnes seers roreesereess 447
최선 시간복잡도 …여어어어어에아아아아사사사사사사사사사사아아아아 929
최선 시간복잡도 분석 에아아아사사아아사사아사사아아사아아아어 22
최소 곱셈 이0000000000000000000000000000000000050000000000000000001000000 119
BIA USS ………어어에에에아아아아어여여여아아아아아애아사사가아에에 452
최소비용 신장트리 ……아아아아어어어에에에에에아아사사사사사사사아 148
최악 시간복잡도 POS SO SOA OS COCCI OEE IK 3 20. 379
최악 시간복잡도 분석 …아아아아아아에아아아아아아아아아아이 20
최적 PeerEer eee Sree rere reer errere reer err re rrererrererrererrereerer err ereeres 116
최적 이진코드 000000000001000000000000400000000000000000-00000000000 175
최적 트리 sosnsceges ve Ves toceusessesccewessessescesesenssscacstecesses 119
최적값 sasescecsccccccnccscscnssecsessoscsesesesesceescescscssoscesscocoes 97
최적경로 Peer ee ee rereeeeree reer rere rereeerree rere errr eerie 250
최적의 원칙 애0000000000000000000000000000000000= 105
최적일주여행길 이999909090000000000000000000000000000000000000000 125


===== PAGE 634 =====
@6 06000 0 0
624   찾아보기

충돌 Sees eC asATOR UAE SOI Son prsntestecresscose-scncemacsansecsise sere ctces 340      피보나치 수열 seiwisieivis bein eels viv aid sleceeiesinwos pues eyUveSesseunesesseuseess 11
치역 ssisinwinnaisiaiaieiniceinipitinegienisgeinie goss ¢e\eeelteeeoalsieicisiesiesle sjesvinssiseelsicus 536        필요충 HAA Sg LOWEN CU sl evaels ssteee Ses Sue se euueeeesle cs ieee ece eee ose ses 543

티민(2) Pree eset ass ctsiscateeruestnasscotereestaenttsessasaecensetcaetes 418      해밀톤 회로 진위판별 문제 에 396
해밀튼 회로 문제 seeeeeecsesascscscscsecesccescsesesesesesesevercs 220
해시함수 oan sols cisnsiesienviseieny.ncieisiows ncivesioseineselecweseaicincisveeueven eye 340
행렬곱셈 sence ene eeeeceeenceeensenceseneeeeseeenseeeeseeenseeeeaees 8, 68
허 프만 알고리즘 바하마 1207
허프만 FLT 에아아아아아아아아이이이아이이사사이이이이이아이어 174, 177
형제 마디 …0900ㄴ060096906이이이이이시이이기이이00000000.0.0090004000000040009 178
확률 se ee eee e eee ee eee eee neeneeeeeeeeeeee ee eneeee een eseeeeseeseneeseeeees 552
확률 알고리즘 이이이이0000000000000000000000000000000000000000000 206
확률공간 se eee eee ne eee ne eee neenenseeseeeeeees sense eesensseeeseeeeeees 553
확률적 선택 cece nena eeceeenenceeeecenesseeenseeseeeaeeesaeeeeaseseanes 367
확률적 주문 Pree eee eee ee reereeereereerererrerrererrerrererreri rey 258
od = …아어아아아아아어사아아어사이어아이이이이이이아사이아사아아아 553
힙 see eeececeeneneeeesncncnenenseseeeeaeaeueeeaee ease eenenensnensesneneeeeees 988
— sae re -     is 성질 탭셔레리이기지이이시이이이이이리시1바/이이기테이이이이 288
입정렬 000000000000000000000000000000000000000000000000000000000000000 087

프림 알고리즘 Gilded caseveassiseteanseeessuscseessasctvessesteresese 150
피리미던=시토신+티민 sseeveseccecsaseeccccesesescssscsoscscees 418



===== PAGE 635 =====
&2-(doh@hanyang.,ac, kr)

1980년 한양대학교 산업공학 학사

1987년 미국 아이오와주립대학 컴퓨터과학 석사

1992년 미국 캔사스주립대학 컴퓨터과학 박사

1993~5년 일본 Sede 교수

1995~현재 한양대학교 ERICA 소프트웨어융합대학 소프트웨어학부 교수

정가 37,000원

2017년 2월 18일 초판 인쇄

2017년 2월 24일 초판 발행                    poses=i
Al 2}: Richard E. Neapolitan fas !
역 eee                   | 협의하에 |

| 인지생략 |

발행자:우명찬송 준
발행처 : 흥릉과학출판사
A: 서울시 강북구 인수동 455-60

ES
[이끄이913]

등 록:1976년 10월 21일 제5-66호

전 화:(02) 999-2274~5, 903-7037

팩 스:(02) 905-6729

e-mail: hongpub@hongpub.co.kr
http://www.hongpub.co.kr
ISBN: 979-11-5600-503-2

iain
낙장 및 파본은 구입처나 본사에서 교환하여 드립니다.
판권 소유에 위배되는 사항(인쇄, 복제, 제본)은 법에 저촉됩니다.


===== PAGE 636 =====
FIFTH        '
EDITION      S

=.
RICHARD E. NEAPOLITAN’ -         a

KEY FEATURES
INCLUDE:

ㆍ The only text of its kind with a
chapter on genetic algorithms                 |
and genetic programming

Use of C++ and Java

                                   pseudocode to help students
지만, 알고리즘의 설계방법과 분석방법을 체계적으로 이해하                            cine alee ane                    |
책은 의외로 드물다, 특히 외국어 책은 국내 학생들에게 .                            No calculus background                    |
로 전달되지 못하는 경우가 USS 알고 아쉬워해                                —                                  |

이 HS 접하게 되었고, 이 책이 다른 책에 비해                    |      ㅣ 마야려 instructor TRSOUFEES:
                                  including complete solutions,
지식이 부족한 학생에게도 알고리즘의 설계와 분석에                                an Instructor's Manual, and
:            3.         PowerPoint lecture outlines
'
‘

이해할 수 있도록 자세히 설명해주고 있음을 발

                                             93000         a
gee & BARTLETT                                  :                       | |                     3
9°791156' 005032

MMLEARNING

| ㅣ            An Ascend Learning Company                                                             /                     ISBN 979 -11- 5600 - 503 - 2

| ㅣ  5 Wall Street | Burlington, MA | 01803
978-443-5000 | www.jblearning.com

