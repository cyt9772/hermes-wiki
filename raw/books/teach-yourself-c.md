---
source_url: "/run/media/yutae/Data/teach_yourself_c.pdf"
ingested: 2026-11-15
sha256: b5d96ccf082668bdf216318112de79219402f717bdfcf0773bc9b8adf04247dd
type: raw-source
method: ocr
---

# Teach Yourself C (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/teach_yourself_c.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** tesseract 5.5.3 (kor+eng, 300dpi)로 OCR
> **쪽수:** 858쪽 | **추출 텍스트:** 1231 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/teach-yourself-c.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** Teach Yourself C
- **Pages (PDF):** 858
- **Source:** teach_yourself_c.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 858 pages)


===== PAGE 1 =====
배움    4 다

” ale ue
발견합니다

단계별 예제와 연습을 통해
as 지향 =    토그래및 밍 범을 ee

탐구합니다
+ + 프로그래밍의 특징을

PUBLISHING

정보문화사

Information Publishiig Group



===== PAGE 2 =====
작상하는 법을
E C/C++ 3.1
Bane 포함

: 단계별 예제와 연습을 5s    a
객체 지향 프로그래밍 YS

COMPLETE COMPILER EDITION

SAMS

PUBLISHING

정보문회시

Information Publishing Group                                             Jesse Liberty 저ㆍ 양재찬 역



===== PAGE 3 =====
Complete Compiler Edition
teach yourself C++
정품 소프트웨어가 들어 있는 c++

Teach Yourself C++ in 21 Days,
Complete Compiler Edition

Jesse Liberty

Original English Edition
Copyright by SAMS
ISBN 0-672-31261-1

All rights reserved. No part of this book may be
reproduced or transmitted in’ any form or by
any means, electronic or mechanical, including
photocopying, recording, or by any information
storage and retrieval system, without written
permission from the publisher, except for the
inclusion of brief quotations in a review.

이 책은 54446" 사와 정보문화사 간의 정식 계약에 의하여
번역 한 젝이므로 이 이 책의 일부 혹은 전체 내용을 무단 복사,
에 저촉됩니다.



===== PAGE 4 =====
었습니다. 처음 이 책을 번역하여
많았습니다. 이 Bo] 얼마 만큼의
다가는 내용이 부실하다고 한구석
독자들을 며칠 동안 고생시키지나

더

에 처박아 두지나 않음까? 혹
않을까? 나를 믿고 책 was             러분의 Bos AAW} 않을까?

그러나 언제나 서점의 한자리를  내어 이 책을 발견하게 되고, 또 다행히
회 a 구미에 맞아 TEs     Hol] 대한 수요가 있는 AS 보고 나서 내심

길이 없게 되었습니다. 조금이나마 제가 가진 지
쓸 수 있다는 것이 얼마나 기쁜 일입니까? 물론 독자 여러분의
관심과 이 책의 출판에 관계하신 여러분의 도움 위에서 가능한 일이었지만 말입

(은 tt

N

그러던 차에 미국에서 이 책에 대한 2판이 입수되었습니다. 출판사에서는 본서에
대한 = AAA 의뢰를 하였으며, AE 이를 기꺼이 승   낙하였습니다. 사

제가 BAS 번역해서가 아니라, 사실 이 책은 팬찮습니다. 저자 자신이 이 분야
에 깊은 AAS 가졌고 또 상당한 경험이 있는 가운데 이 책을 만들었으며, 많은
예제를 통해 독자 여러분의 실력 향상에 상당한 ESS 주게끔 만들었습니다. 또
한 독자 FES 초보자로 잡았음에도 불구하고 이 분야의 중급자들에게도 상당히
유익하도록 AS PAGUG. 전산학적 깊은 토대 위에서 일반 cH 언어를 설명
하였고, 상당한 을 We 현실적인 888 가질 수 있게 하면서도 Vee

루었는데, 이러한 점들의 유용성이 초판에

본서가 출간되기 전까지 도움을 주신 여러분께 감사드립니다. 특히 바쁜 와중에
책의 교정을 기꺼이 맡아준 재원군에게 감사를 표하며, 이 작업에 매달
히 저를            와준 처 이미혜와 그 동안 같이 시간
혜옴이에게 미안한 마음 금할 A 없습니다. 또 본서가 나오

때ㅁ
ina
of
[묘
9, |o
Hu
Le

\


===== PAGE 5 =====
깊은 감사를 드리는 바입니다
역자 소개

-^~
에
~
J8
~~

학 사 : 서울대 자연과학대학 게산풍계학과

석 사 : 숭실대 정보과학데학원 정보통신학과

- 한국 『<통신 개발부에서 MITEL 개발 및 서비스 참여

CHITEL'S] 전신인 한국경제신문사의 'KETEL’ 초창기 게발부

- AF ep 서비스 회사의 개발부를 거쳐
- 현재 이동통신회사의 연구소에서 이동통신 연구원으로

rd

주

참여)

양재 At



===== PAGE 6 =====
Adal ee 3

제1주 시작하면서

제일
C++ 시작

제 2? 일
C++ 프로그램의

Zi Bee
각 TL

a a Se ee ee 24
간단한 CA] 역사 에여 tandgnevnrcsneepysivndaresvosnuuszvansises24
포로 그램히랄 =아에에어서메매메데에에 cnio sre uye oto avesayavaptearereeesactees nest25
문제 해결 방식 …………% 기드 0 이을 으여여이이에에 이26
+과 객체 지향 프로그래밍 .…………………………………ㅇ……………………………28
C++ 어떻게 진화되어 왔는가? …-……………………………………………………………………………………………… 29
ANS 다 주: eftce wants carpets enn cet owspera vat mes Rov oleccapeaeevernaeriveceerctinn 30
를 먼저 배워야 하는가? ………………………………ㄴ……………………………………… 30
쁘무교랭 술비ㅋㅋ 8 ee ee ee ee 31
개발자의 개발 환경(060610001604[ Environment) ………………………- 31
원제 코트 컴패일하기 socesties cecum ess ecssatsesencrarasseaeeensenenariedonesaesstivere ses 32
BAS 가지고 실행 가능한 파일 만들기 ……………………………33
개발 주기([06\61000760 Cycle) ……………………여아아아나아여아에에아아아아아아아아아 33
HELLO.CPP --- 첫 번째 C++ 프로그램 작성 …………………………………………… 35
컴파일 왼류들 a cssssssassunecgensensesensenscessnncscdlesnecvscunvsetssussenarsususasness36
SAGE 비여애으션베녁레더해며버여애연휴일여농셔새켜시셔매인셔여이=8애애이이니빈덴이에여여 37
QGEA hs ccestzesoves ees Bevresenue Mien ttveeauteces eaneees Ha jcenecancenceasersenseseseoveee Sates 37
연구 <cevsssinsemeshtnyéosonnpcatinesdeyvanennoubencavennceeta Gr cedensicvssavetionanaveneouniawel 38
Fa es oer owt oi os cten rho enact42
간단한 프로그램의 각 부분들 …………………………………………………………………………………………………………………………….42
간단히 EB COE ……………예…~포이이이셔여메메이44
수석 Fe(Commmients) «vessessviesseessacssacercecsseothjesssseonecaracncnarctscvonsesvaneers46
eee ee ec eee eee ree ee49


===== PAGE 7 =====
4 ec Kel

제 3 일
변수와 상수

제 일

수식과 문장

에 약 ..……-…녀애잉겨여여개메여=래채채2930 52
이스 meme eens cassasnicresaseeonverceresmremnetneeesctemaneunmncereiqanentieniand sient52
I cxcssanesrsametire frreorcmemomconnacemabestomeisinietnesntin sik SECHE 52
YS iacnig BEA Has cohen sascrranesinced enn enveervebesecs omen chalet tncped at56
WA(Variable) Gt 부터인가) o-escsnscccsnsecssnsscecnneeceneennunsacnnnvesnsssatbavecss56
변수 정의하기 eS EEE 60
한꺼번에 같은 형 변수를 하나 이상 만들 때 .……………………아아아아 62
변수에 값 대입하는 법 ……………아아아아아아아새아아아어어이어어이아이이아아어사아아아아62
언제 short 쓰고 언제 long-S 쓰는가? eevee ee eee eee 65
SCAG Serta) teoucbcsescccworasncertte eomerennntnm acme civic tAah 67
ASE (Comstant) ----e-peecececeeeeeeeseeeseeeeesssseeeeneneneeseseeeeneneeeseeneaeeeeresseseees69
상수 4S A (enumerated constant) ………아아아아아아아아아아사아사아아사아아아아아아 71
Ce ne eee ene ts73
IRA, a secccnnrsereon sens snoemnmnteatte a SATE RATES ERIE 74
cine msatcsssnarsus uncmnvencememmennemssereceenifnarememenyensiraseiitonii Bi15
JER sa nsceressasereesusessenvonninontenencton tonne semen pit siti PRRO SEAN ROE 78
FAl(Statement) --.----:cceececeesesee esse sees ee eeeeee eee neeeneeneeeeeeeeeneneeney78
cod) 분 berrteaetian) |a-sennicsoniscenstcrmmemsnrenollierertemmsctcernemnneneteneneene 79
OVAL AH Operator) ……아아아아아아아아아아아아어어어어어어이이이어사사아사사사사사아애애애어여 81
대입 연산자(&991800160[ Operator) 2}

수학 연산자0\40016080081 Operator) 2] 혼용 …………………아아아아아아아아아아83
증가 연산자와 감소 연산자

(Increment operator and Decrement operator) ………아아아아아아아아사사사사사사84
연산자 -2-214= 9] (Precedence) ………아나아아아가아아아아아여여아아아아사아사아아사아아에 86
중첩 괄호(04690108 Parentheses) ………………………여아아애에아새아사에에아사아아아 87
참값의 속성 cecccsdeccecsecseeneeneeenenseeseeneesesnesnsessensennenscenenneaneennennennenneny 88
아우 차: sc cancanensnsshesrraneonernvemrameecimennenveceehbenicarsinaieymenaaeratiinens sti 89
중첩 #문에서의 중괄호 사용 eee teeter eects96
논리 연산자(08108 operator) ……………아아아아아아아아사아아사아아여사아어사아아아아아99



===== PAGE 8 =====
차례 ee 5
관계 연산자 -9-Al<e9](Relational Precedence) ……………………………………… 100
창과 PUA SEB 마더 추가 .…… .…………~에개 는 101
조건 연산자 혹은 삼항 연산자
(Conditional Operator or Ternary Operator) ……………아아아사아아아아아아아아 102
a ee ee 으이게데여여배시이에애다이아 명 103
OER cecag egg len rout ete pe rmmenrpt rm endcchetil dapeornormneminnctncrngont ome 104
Or SE sauevencanesvawcongiewinwese swan vesiecuneenecestcrsseantst eee Sheeverac don ptaesezashenesteescesr 104
제 2             써뭔 = 1 a es 제 이이 108
함수                    함수(0000000)란 무엇인기) ~. ……………올에…여애애애어여아사: 108
함수 선언02608008)과 함수 YO] Definition) …………………- 109
함수 Ala (Execution of Function) ………………………………………………… 113
지역 변수(0081 Variable) …………………………………%……… 114
전역 변수(81081 Variable) ………………………………………%의이이의이 116
전역 변수 - 주의해야 할 단어 ……………………………ㄷㄴㄴ………ㄷ=……………………………ㄴ…ㄴ 118
지역 변수에 대한 추가사항 …………………………………………………………. 118
함수문(『00400010 Statement) ……-…………아아아아아아아아아아이아아아아아아아아아아아 120
함수 °)z}(Function 7000) .……………ㄴ겨리 120
매개 변수는 지역 변수 ………………………………………………………… 121
반환값(\60470 Value) ……………………-………………에에에에에에에에에에아에아아아이 123
기본 매개 변수([06[341[ Parameter) ……ㄴ…-……아나나아아아아아아아아아아아아이 125
함수 BA (Overloading Function) ……………-……………………………… 128
함수에 관한 특별한 주제들 ………………………………………………………… 131
함수는 어떻게 동작되는가 .……………………………아아아아아아아아아아아아아아아아 137
1:이겨케가 142
(EA seecpeemrmprme sans. premmncerene tena ths gira 어이 이 이 20 142



===== PAGE 9 =====
6 ee Kal
제 (일              Fay 분 escxevsecsk dete gi) sc scuswerastc cesses tee on metas cease dvsogansngs Tob OnEOHE EST? 146
기본적인            재로운 형0806\ Type) CHE] …-………-…여아에내래애아너에에아배에서연재여아새애애사 146
클래스와 멤버((21069| and Membr) ………ㄴ……여여여애아애애에 147
Al-2-(private)Z} 범용(04040)에 관해 ……………………아아아아아아아아아아아사아아아 151
클래스 메쏘드 구현04001070600108 Class Method) ……ㄴ…ㄴ‥…………… 157
생성자와 소멸자(000604060『 and Destructor) ………………아아아아아아아아아 160
600랄멤버 | 함구 rcced scerseacceosenneaeerecneseenrenceryatcceecin emrenenesiimeeaeresnien 164
인터페이스와 구현 do neseeceencaencsesenenerensnnnauensnsnanersmastonssnstinnlintayatoneass 165
클래스 선언과 메쏘드 정의를 YMA 할 것인가 ………………… 168
a a ee 169
른 클래스를 멤버 자료로 갖는 클래스 ………………………에제어여여며이애 122
구조체(900000406) ----4.-eecececsecerseeceesseeseeeresvensssnssassessassessssenseensneenare 176
a a ea 으으 이 177
PRA, . 0000 | 801 거으여애백기이 911 177
es eet 179
제 일              FATE ..여재네대52 182
프로그램 흐를       수 한 문(00008) | simcntenctemanienter isn Loe 182
le: IE. ccxscenachsmseseesncsannecnre nmmasionieqenraihecernonceescvonenvenseeenenenneen 184
30. .떠116 줄환분 | 3 0 마 SOaRnts Sarre oy cPens teaser ere crertt aor 191
ee ea rere en ee 194
수 한문 유약 a a ee203
SFL HE easy cssr cae c see |S couse verreris cea toc seiner seae 8p Fre. cara errant eee205
nn ere212
RA ee rsa chcceonever ee vrsneonssveninoing eensemennnnsnntyrinrsitaamnimy enna inte rhais213
영구 ssesneussnvsaietiaif ct emntindenestoinet nani isn ev eoigliiese sD uRO Ant 213



===== PAGE 10 =====
Nal ee 7

제2주 시작하면서

제 2              Aa] Sie exer esas enezectaae east asccersractecee- se vepenernenedeeee bbensterance eueuenensnuonenseenen224
포인터                 포인터란 부엇인가? .………~…에메이 이네애매메메메에에224
도대체 왜 포인터를 쓰는가? .…………………………아아나아아아아아아아아아나아아아아233
스택과 자유 기억 공간(066 8006) ………………………………아아아아아아아아이234
페포리 누줄(66007 16849 -… ~ …~밸시아이테디니238
자유: 기억 eee ges, es bd |e ere eee239
객지 이터 cherie eterna gil NB 2000 20209 이 240
자료 멤버0280 Member) 접근 ………………………………………………아아아아아아241
자유 :기억.종갈의 펠버-재유에 대해 … ee242
thse 포인터) cesses etcetera eee eet reece244
실종된 391 E| (Stray or Dangling Pointer) ………………………………………………… 246
CONSE 이터 cess iesevsstecsicl Araetcta sereeeaveretse ac i sce stains dssv stun sa lseoscetoee,248
여이. 에 leaner tee Rima rather alist a tivexntivapoonsasehircisd en251
시 에게 에메에게에거 치트 기252
그 기기”252
제 일              「: sasscrsrnnconncsiuansonossnonanecossorsunsesicesosessinersusavnrnansnpensetanencccatneuniciaiions256
참조자                  참조자(606009)란 무엇인가? .………………………………………………………… 256
참조자에 주소 연산자 & 쓰기 ………………………………………………………………………………257
무엇이 참조될 수 있는가? a260
널 포인터와 널 잠조자 terse ee sectens rs es cae eer -ceeieteesvecasesoWertoneeal 262
함수 ol--(Argument)S 참조자로 전달하기 ………………………………‥263
함수 표제0000000 Header) 2}
함수 214 Prototype) ol] 대환 이해 .……-……아에예재겨여새사여제며레메이메:267
여러 개의 값을 반환하는 법 ………………………………………………………ㅇ………268
B= Efficiency)S 위해 참조자를 APSA ……………………%……272
언제 참조자를 쓰고 A) MES 서나. …………~…~머여이에280
참조자와 포인터를 섞어서 쓸 때 .……………………………ㄴㄷㄷㄴ………ㅇ………………ㅇ…ㅇ……281
범위 벗어난 객체에 대한 BAAS 반환하면 안됩니다 ………282


===== PAGE 11 =====
8 ee 차례

제 10 일
고급 함수들

제 11 일
배열

So] 있는 객체에 때한 참조자 반환하기 ……~서어나…애%머아아에에나 284
포인터, 도대체 누가 포인터를 가지고 있는가? .………………………아아아아286
Ch) ee ee ee287
00 ^ fartah 288
a ee ee 288
Le a ee292
멤버 함수 ZA (Overload) ……………………………아아아에에에에에아아아아아이292
기본 (아케 Wile) SAF] corssivccsnsircamaruscenersconcmmencnnes 294
기본값과 중첩 함수 중 어떤 것을 고를 것인가? one297
기본 생성자(26[341[ Constructor) ……………아아아아아아아어아아아아아아아아아아아이297
잼성자 좋접 caccree curenaecmmenananenanden yrmemmanmnunpnemenen:298
기기 :즌기화 . | .  . 메어 며브내거에에 300
복사 쟁성자(0007 Comstructor) ………………………개어애어거캐사애애어셔이이케사셔이터의 301
연산자 중첩 cevesalle suri ensscia so minor ute nenmann ern 305
병환 연산자 rescore eevee ga ateeav sex eoroent em Scr Se ons Sewensnes cata aave 179 325
a a ee a 329
OBA sce cepted baesae scores ccanartes osare msnoyaen nee miner reer terete 329
a ee ee 330
DEE sccnirsaios devs wvresth sieersvscoestiewicet ster tssasas: x ecoanna et  AaG RSA ARE URE 334
배열(&085)이란 FI STD evcvcsansestencricnersonerenwernmneneanennerarodtroranennies 334
배열 원소(418\ 비버) ………~…내여여거애저셔셔데여이여에래여여이어여새애이내 335
배열의 끝을 지나 값을 저장할 경우 ……………………………………………… 336
ee ee ere er 339
배열 ced tl ees eee eee ce ee cs 340
변수. 전언 ccccccccsesseeseccssssneneesecesnsnnmeccennssnmeseeecsnssmneeeeesssnnmneeteee 341
객제의 배열 areas ca cps rece sa caron econ tates cnepaee so osytecns sues ueectenton ener eects 342
다차원 BA (Multidimensional Array) ………………아아아아아아아아아아아아아아아아 344
타자원 비열 초기화 rece ncrccmomerncrnecroos cancers s¥encbinaaseemisetos cencn seat anes 345
메모리에 관하여 ………………………………………………아에아아에아아이 347



===== PAGE 12 =====
차례 ee 9

포인터 wS(Array of Pointer) ……ㄴ………-여여가아개개애겨애겨여녀여여여여석새애산 347

자유 기의 Sechelt 배열 AIST] 비며어제제일 떼메에테레딩이아게 349

배열을 가리키는 포인터와 포인터가 저장된 배열 ……………… 350

SHOVE) Sb. BY 열병 %에세빼제재제이네애지익내애재급으녀이애연애재이며에대벼제대기350

자유 기억 공간의 배열 지우기 …………………………………………………………… 352

806 HY SS GA 배월) <n cseces awesncaeens ote stseentons dieacvsserscwn sovesuseseteaeewenten 353

strepy() 2} StInc py.) ease ee eevee eee teenie 355

문자열 클래스(90008 Class) ....-.....ccccccesesecseccressssorssseveesteseenesesstss 357

연결 e]2E(Linked 1490와 다른 구조체들(9000046) ……………… 364

클래스 배열(4089 Class) …………………………………아아아에에에아마아아아아아아아아 371

DOOD psc sce con UN cy RNR omen pring 372

REA, winereecdpscortictressnen nis Ml tach eerie ael ae 02 그 구이 372

Se ee a eS a eee 373

제 12 일            헤매 세게 0 거기 nan shed 레테 에게 376
2                   Al =(mheritance)O| Ct SOV? 여때에시캐새새액메비애이잭에비애벼년대 376
전용(001816)과 IAS (protected) ………………ㄴ……………아나나아아아아아아아아00 380

생성자: Ast Alb suservescesersssyousaesmmverovessareneecaeacatoncgransaseen thant tsa 383

l= Ayu Overmdine’ Function) | cs. m-dueecved Areoemeneederoristesteaers 390

가상 PAE (Virtual Method) …………………………………………………… 396
a a sea409

ee a ee409

oe ee Se410

제 13 일            Se ee er ee ee 제0414
다형성                단항 상속성(9016 1016018006)의 문제점 ……………………………………………414
다중 상속(4010716 Inheritance) ……ㄴ………………………에에에어에이에메에에애아에아이420

주상 자료형(41608 1088 1506) …………-……………아아나아아아아아아아아아이아438

RA cccuccnamreeummnmeseuinimmigmansomcscianast hevnrassmnssoadincisenticiiomel452


===== PAGE 13 =====
10 ee Kal

제 14 일
특수 클래스와
함수들

제 {5 일
고급 상속 기능

제 16 일

스트림

제 epcccnecgpypetnsie former etinen heen Sing456
정적 멤버 자료(96006 Member Data) …………………아아아아아아아아아아아아아아456
정적 멤버 함수(96000 Member Function) ………………아아아아아아아아아아아아462
함수를 가리키는 포인터 cn cmencesnonerenencnesnasveneg tite cntenaioas causennyesveeiones464
멤버 함수에 대한 포인터 ………………………………………………………………… 477
ee ee a ae 배바며482
1B, coco rv aemnaamegntnpete Sissi OST OTITS482
a 00000 쓰게483

De 500
SESH(Containment) ………………………나에나에아아아메아마아마머마메아메아메아에아아아아500
상속/포함, 대리02666880020) 관점 구현 oo eee eee eee512
전용 상속(#ㅁ866 Inheritance) ……………아아아아아사아아이이이아아이이이이이이아이이이522
호 래트 SU ZA(itenid 61866) -.0--coro wane jonainsaheeonnrvenienricneninesnssonsbestani 526
BE, Sheeler (Panetlian) oncniesscossnneracradiecomnasranmnaenmeomne536
프랜드 함수와 연산자 B*(Operator Overloading) ………………ㅇ…537
삽입 연산자000960000 Operator) 중첩 ee eeceeee ee eerste eens540
Cn a re542
a a ae Avner542
00000 sunt fennel ke ese 543
JAE scarecmezetiorcaenn  arersarraecmacer emboli ees Purses548

JE) (Stream) 9] 대한 FASE eaceceeecer eer eres548



===== PAGE 14 =====
차례 ee 11
표준 입출력. ZA (Standard YO: Object) =…~.…………여아기어552
Al ZIAD (reditection ters... waved vse es te yter resrwesizes nee Re ees553
이을 사용한 9) rstccssactibsaiastacsnnconnnssscatdengenerereeoucrenennsvoroseenvoneald553
Cine]. '또 다른 멤버 BSE i etercect eerersderne eter apeenantees navesteszens559
아로 See colle eal AO eta re eatecectancuce, Bt tes coathitas tontberrn ceecoem, dosor's eT567
관련된 SERS conssseaccsszevieconssaarsevaaniencovcanss oaretonnvconsvoconnenannsbestinéannots568
4€A(Manipulator), 2} (Flag),
규격 명령어(800000800108 UNSEPUCHON pact 5 how ec ages essareeceverTixeevecoeneeys 570
PoE GTP 00000 ,함수 oeeeesesecsessecseeneesesseeneenecsesseeseeneeseeneeneeneenes 574
까일의 입력기 '졸력! -…에티스~매게병이비 이0이에에에에이 576
이진 파일과 텍스트 파일(8144 versus Text File) …………………… 581
명령어줄 프로세싱(20000000-1106 Processing) ………‥…‥…‥…………… 583
BEEP sosccnsrdiscsavencnunsouscanitaneipchapetensiessaltn tus cellg vane vin cotanenitlbasinasaciinn 587
fen eee eer Cee, eee nee SSE ee ee587
BASF anuneerenyeonnennsnanurenemenannaslierisnusicesabneviienionsne tanseneeryninensemnceticoneints588
제 17 2            FEL 베 viet acumen nse nhac a agtaeanacnsaawnaoEooNnagy592
전처리계               전처리계와 컴파일러(※7000006990ㅠ and Compiler) …………………………592
중간 형태00060000866 80020)의 보기 ……………………………………………592
Hdefine 지서자 사용하기 .…...이나여이세여새아개사여새새시셔아이애새대이시지서으593
포함040149100) 및 포함 감시자0401049100 Guard) ………………………- 595
매크로 함수(540000 000000) ……………:………………아아에아아아아아아아아아아아아아599
확장: 황수미06 8006000) oan nimcntonnneteomnamnmnanannnnas 602
문자열 연산(90108 Manipulation) ………………………아아아아아아아아아아아아아아아604
내장 매 그 (PRECETINIER MAGTO) | ieantoncts nes argpbeceannut Unaaiesnosntenswlaneye sel 605
ASSEN)! elses sspears enneadreMerrtean eran rasan606
GY sracenssasesaestaisnncknapasbnsantaapa’ psennerneprtoernannened nprnenct<tuenngenonbenveorttone620
RON, seweceencmesracunemnasedorcsmngesianesi sur tinemosecrtn nicer annnnncenceaNsineT621


===== PAGE 15 =====
12 ee Kal

제 18 일
객체 지향 분석과
설계

세 19 2
템플릿

제 20 2
예외 사항과 오류
저리

서문 이여에네데애새내매에9밥여겨여새벼지레지벼애인624
개발 427|(Development Cycle) ………아아아아아아아아아아사사아아새서어아사사아아아아624
경보 지스템 시뮬레이션 ………………여~여여겨여선려=9데애베버비애시며625
우편 .시즈템(006040채아) es sersccrnscreteronscaneensternnarenacarennnanvensonconnves631
생각은 여러 번, 결정은 한번에 …………………ㄴ…………아아아아아아아에 632
분열시킨 뒤 정복하라 …………………아아아아아아아아아이이이이이이이이사이서아아아아 633
메시지 곰거회 0 으으으633
추기 클래스 FAA cl serecencesecemeenrmecsoersnnensnind can CSE 634
순종 A\S(Rooted Hierarchies)3} 잡종 계층

(Non-Rooted Hierarchies) ...--.-..cccccccsiesieeeceesneeneseeneseneeseeensenees 635
인터페이스 설계 a Ee ES637
PostMasterMessage 클래스 설계 -o---sseescseeeseseeeseesstessstesseenenneseneessess 640
ae er642
구동 프로그램0001@ Program)S 가지고 작업 ……………………………… 644
위아 ~... nee nner cen meee on652
VB vas cercnrinsesnsnparernenarse snnson rs LS MO on mI RID 652
영구 sccssenrssnosennacnenseareremnasnanmencenenayeeenenouanem marerceneneeneren muntimtinn653
PE: a sncvanorsuircgsnipo dl oesone ne enn 8 SN ES 000 656
€] E21 (Template)O] GE 무엇입니까) waseeseteccseeesssssosnnvorsnsnensavevenavennns656
YT] 별수화된 형 |…………여여여애아여아아여애여제657
템 플릿 정의 …………~악………여겨여새99422 657
TREES) 월수 ccteipesedtvcncrcersuveeunnanmndtauneerel dos osetia meamearsinaws sevdeannccenioni663
b= = eo ne 664
템플릿 항목 .사룡해기 ceeneevemcenramemcearsneonrmenmenesegeracymnencab omc671
예와 | eee ee ee 684
RA 녀여여내여685
GASP cacvsssessinsnvezeviiosh coneunomnaimercarneesomrenseniiessnsacminastsonsgensonndenuns tes 686
시름 2 2 0] 으으으 으으 으으으 08 1 690
버그, 오류, 실수, 프로그램에 녹이 슬 Code Rot) …………………690
예외 AVE Bicep) … …-………ㄴ……어…네에더데이셔어예저가객새거매진애3 692



===== PAGE 16 =====
차례 ㅎㅇ 13

try 블록과 catch 블록의 사용 ……………………………………………………………… ……. 698

예외 사항의 자료와 예외 사항 객체 작명법 …-…………………………… 705

예외 사항과 템플릿 …………………………………ㅇ~ ……………. 713

오류가 없는 예외 사항 ………………………………………………………………………………………………………. 716

버그와 디버깅 …………………에이여여며며그에. 717

아오 scrnanunwnance satis ir teahdsnxarea nade tie vntueresnyeesvuehuvmis epee eiceeneni 718

oe eee en 719

SAAT erexscorineortatneessneunesamcecosnmswowuunanoessneseineyipsesisaWiUisLssehanbansarorehe 720

제 21 일            | HE snot senaconsenaotosenemustles shaw saves wsenstaknemnarnaryeeecacunses oiaa 724
다음은 무엇을 할  pe Sie Z}O] He] e](Standard Library) ………………………………… 724
것인가?         7  WALA (String) 라이브러리 함수 .…………………………………………………………………………………………… ……… 724
렐 시간과 날자 관련 한수 ………………… 00730
Se | 732

비트 AAMBIt Twiddling) ……………………………%%……22. 736

| 8] ne ee 742

BE A             ee ee 764
연산자 우선순위
HE B              se ee ee768



===== PAGE 17 =====
14 ee 차례

부롬 Cc              Po) SB seas cvsessunes Ale sn oad es seses cach nen tbaen de seeesssau trae nn atornesen ksnstess eng st eee722
이진법과 16진법       다른 기수들(0016 Bases) ………………아아아아아이아아아어아사어어사사세사사아아사어 772
기수에 BEY sesvccvsslevsesbencecwcnacs evecqetessuernaseasanevovenetecerestversncasenenerte 773
Ce ee ee ee ee716
부록 D 해답편 cvewsveuwasavadwaswupontstvelvteusvoousued/aas ucla enemas tnjncusiealenaesseanieanicusecnusuiesss cies Ueetesese eres 781
부록 【 CDROM 사용봅 cccccccceccccccecsssssneesesntntntntntinsictstststntvtneienenenees



===== PAGE 18 =====
an

2차 판에서 HHA AS ee 15

판에서 4

이번 2차 판은 초판을 완전히 검토한 뒤 수정하였습니다. 바핀 부분들은 다음과
같습니다.

를 새로운 ANS 표준에 관한 항목이 추가되었습니다.

를 초판의 모든 7001) 2TH] 새로운 ANS! BEY 따라 int 값을 반환하도록 다시 쓰여

졌습니다.
를 친시 코드들이 ANS 표준에 따르고 있는 Microsoft 컴파일러로 시험되었습니다.
를 자바, 인터페이스, 다중 상속에 관한 부분이 추가되었습니다.

를 (의 설계 방식에 몇 가지 추가가 있습니다.
를 표준 팀플릿의 라이브러리가 포함되었습니다.

를 예외 사항 처리 및 메모리 관리에서 몇 가지 문제점을 다루는 부분이 추가되었습니다.

이러한 수정 부분 및 새로운 추가 항목 이외에도 여러분은 저자의 웹 사이트 혹
은 Sams 출판사의 웹 사이트에 접속을 하여 최근의 원시 코드와 다른 추가적인

Jesse Liberty2| 웹 사이트

www.libertyassociates.com

Sams 출판사 웹 사이트

www.samspublishing.com/codecenter.htm!


===== PAGE 19 =====
16

66 BAD 글

감사의  ~ |

이번 2차 판은, 그분들의 도움이 없었으면 이 책의 2차 = wel 불가능했을, 그분들
에게 두 번째 WAS 드릴 기회라고 생각합니다. 그분들 중 UA) Stacey, Robin,
Rachel 146609께 감사드립니다.

In Se

또한 이 책과 연관된 Sams 및 Wrox 출판사의 훌륭한 자질을 갖춘 전문가 ae
Al ZAKS 드립니다. Sams 출판사의 편집자들께서 깔끔하게 YS 하셨는데, So
fran Hatton, Mary Ann Abramson, Greg Guntle, Chris Denny 씨께 감사드립니다.

이 A 가지고 몇 년간 온라인 강의를 하였는데, 많은 학생들이 버그와 오류를
as 하였습니다. 많은 WS 졌는데 그 중 Greg Newman,
Corrinne Thompson, Katherine Prouty, Jennifer 001080에게 특별히 감사드립니다.

한편, 저에게 어떻게 프로그램을 해야 하는지 해 분들에게 WS 드립니다.
Skip Gilbrech, David McCuneo] 그분들이고 또 C++  저에게 가르쳐 주신 Steve
Rogers} Stephen 2891600500에게 감사드립니다. Mike Kraley, Ed Belove, Patrick
Johnson, Mike Rothman, Sangam Pant 이분들에게도 감사를 드리는데 저에게 어떻게
프로젝트를 관리하고 결과물을 만들어야 하는지 가르쳐 주신 분들입니다.

이 AG 만드는데 직, 간접적으로 ESS 주신 분들은 다음과 같습니다. 9004
Boag, David Bogartz, Gene Broadway, Derw, Al Carlson, Frank Childs, Jim Culbert,
Thomas Dobbing, James Efstratiou, david Heathe, Eric Helliwell, Giesele, Ed Herlihy,
Mushtaq Khalique, Matt Kingman, Steve Leland, Michael Smith, Frank Tino, Donoban
White, Mark Woodbury, Wayne, Wylupski, Alan Zeitchek.

이 책 초판에 많은 OHS 발견하여 주신 다음 독자 여러분에게 감사를 드리고
싶습니다. Gordon Anderson, Ari Blachor, Charles Campuzano, C. Raymond Church,
Charles I. Desch, Jr. Charles Dingman, John Embow, Jay Erikson, Mark Fiedler,
Adam Fordyce, Lari Kirby, Roger Leininger, Ray Lush, Sheryl McKenna, Frank
Marrero, Tery Milner, Neeral Patel, Raoul van Prooijen, Karen Risser, Ralph Russo,
Gregory Safford, Joe Scalone, Robert Sikes, Walter Sun, Paul Sutton, James
Thompson, Orlando Vanin, Jr., Pascal Verdieu, Stephen Wain, Jack White, Nick
Witthaus, Michelle Zulli.



===== PAGE 20 =====
감사의 글 ee 17

프로그래밍이란 기술적인 한 창조적인 경험이 많이 필요한데, 이러한 경험 축적
에 많은 도움을 주신 Tom Hottenstein, Jay Leve, David Rollert, David Shnaider

Robert Spielvogel7] 감사드립니다.

>

마지막으로 Kalish 여사에게 감사를 드려야 하는데, 그녀는 1965년에 저에게 이진
연산을 다루는 6학기 수업을 가르쳐 주셨습니다. 당시에는 그녀와 저 자신이 이
진연산이 왜 이토록 많이 필요한지는 몰


===== PAGE 21 =====
18 ee 저자에 대해

Jesse Liberty

Jesse Liberty Liberty Associates, Inc.(http://www.libertyassociates.com)2] -회장인데
여기에서 그는 객체 지향 프로그래밍에 대한 APES 통한 교육 및 모니터링,
컨설팅, 프로그래밍 사업을 하고 있습니다. 16696는 Xerox] 소프트웨어 설계자였
고 AT&T 사에서의 뛰어난 소프트웨어 엔지니어였으며, 씨티은행 개발부 부사장
이었습니다. 그는 메사츄세츠 캠브리지 근교에서 그의 아내 9006와 두 딸 Robin
및 Rachelz} 같이 살고 있습니다. ele} YI jliberty @libertyassociates.com-2- 통해 그와
연락할 수 있습니다.



===== PAGE 22 =====
소개 ee 19

4)

이 AL 독자 여러분이 0++을 가지고 자습할 수 있도록 꾸며졌습니다. 219) 안에
여러분은 YO 처리의 기초, 순환과 배열, 객체 지향 프로그래밍, 템플릿, c++ 응
용 프로그램 제작을 배우고 알게 될 것입니다. - 모두   구조적으로 잘 정리되고 따
라서 배우기 쉽게 꾸며졌습니다. 각 과정은 몇 개의 예제 프로그램을 게공하고
있습니다. 모두 완전한 출력 및 그 프로그램에 대한 RIS 제공하는데 그 날 배
운 주제를 예제화하였습니다. 또 문법란을 만들어 쉽게 참조할 수 있도록 하였습
니다.
심화시키기 위해 각 과목은 여러 개의 질문과 답변(2&4), 연습

끝에 달아 놓았습니다. 부록에 나오는 AHS 여러분이 작성한 답안과 비
진전되어 가는 여러분의 실력을 체크하십시오.

[N wl}

요   떼   ttlo

El 고 에

i

에

이 책을 읽기 위한 특별한 조건은 필요 없습니다.

이 책으로 CHS 배우기 위한 특별한 프로그래밍 Zee 필요치 않습니다. 기초
부터 시작하여 C++ 언어와 개념을 같이 가르칩니다. 문법에 대한 여러 예제와 자
세한 코드 분석은 여러분의 여행에서 상당히 훌륭한 안내자가 될 것입니다. 여러
분이 초보자이건 이미 몇몇 프로그램을 경험하였건, 이 BS 여러분이 0++을 쉼

「

고 빠르게 배울 수 있는 적절한 구조를 가지고 있다는 것을 알게 됩니다.

이 책에서 사용하는 여러 개념들

이 박스에서는 CH 프로그래밍을 SHOR 만들 수 있는 정보를 담고 있습니다.

os
bes
Ir
>
oe
예
에
win


===== PAGE 23 =====
ee 소개

목     분    들의 gore         'T   를 사용합니다.
과목에서 기본 원리들의 요약을 위해 00/ㅁ014" 박스를 사용합니다
00     이 과목      본

DON'T 이 박스 안의 정보들을 간과하지 BAIT.

<r          수경                  ck 저 ma

코드                    번호가 매겨지지 않은 코드는 전 줄

2       는 번호가 매겨져 있습니다. 번                   :

이 버너 코드는 한 줄에 쓰기에 부족한 경우가 있기 때문입니다. 이
연속을       Ww aL 중서         :

aide 줄을 한 줄이라 생각하고 입력하십시오

ㅇ   UL     = =



===== PAGE 24 =====
(;++의 AM FS 시작아기에 앞서 독자 여러분은 몇 가지를 준비애야 합니다. 컴파일러와 편집기, 그리고 바로
Ol 책입니다. C++ 컴파일러와 편집기가 없어도 Ol AS 공부할 수는 있지만, 그래도 실습을 SoH 얻을 수 있는
것만큼 많이 얻을 수는 없습니다.

프로그램을 배우는 가장 SE 방법은 실제 프로그램을 짜 보는 것입니다. 각 단원의 마지막에 몇 개의 HAO 연
습 문제를 실었습니다. 공들여 0! 문제들에 답아고 가능한 한 객관적으로 점수를 매기십시오.

본서의 뒷부분은 0] MO] 앞부분 과정을 기반으로 설명아기 때문에, 다음 진도를 나가기 전에는 항상 현재의 부분
을 중분이 이애아시기 바랍니다.


===== PAGE 25 =====
mec 프로그래밍을 해본 독자에게
HE 5일간의 학습은 HAO! 매우 잘 아는 부분일 것입니다. 대강 읽어나가면서 연습 SME 풀도록 아는데, 6일깨
학습으로 넘어가기 전까지 빠른 속도로 읽어나가도 무방합니다.

첫째 FOE St 일반적인 프로그램 및 C++S 시작아는 데 필요한 OIE 아였습니다. 저음 이틀 과정은 프로그
매밍의 기본 개념과 프로그램의 으름에 CHOW MSLICL SQM 과정에서 변수와 상수 및 프로그램의 자료 사용법을 배우
는 프로그램에서 주어진 자료의 값 및 프로그램 수행시 만나는 조건문에 의애 분기되는 과정을 wWEUG. 5일
는 함수란 SHO 또 어떻게 사용아지를 배우고, 6일패는 클래스와 AME WEUC. 마지막 7일깨는 프로그램의
으름에 HO 좀더 배우고, 0] 첫째 주의 마지막 날에 여러분은 진짜 객제 지향 프로그램을 한 번 제작애 보게 됩니다.



===== PAGE 26 =====


===== PAGE 27 =====
24 ee AIF

서문

ee 오늘 의 시간, fie 유능한 C++ 프로그래머가 되기 위해 이제
2

Moy CH] 소프트웨어 개발의 표준으로 되는가?

Bch 프로그램을 개발하는 각 단계

간단한 0++의 역사

퓨터 언어는 세계 2차 대전중 탄도 AAS 하기 위해 처음 개발되었는데, 그
우로 많음 ㅋ적인 ele 겪어왔습니다. 초창기 프로그래머들은 F

명령어들과 기계어들을 가지고 작업을 하였습니다. 이러한 명령어들

일반인들은 알 수 없는 긴 문자열들로 이루어져 있었습니다. 곧이

는 연상화된 언어, 즉 어셈블리어

식으로

현재에는 84910이나 COBOL 같은 고급 언어들이 개발되었는데, 이들은 사람들로
하여금 인간의 단어와 문장에 유사한 형태의 a a 수 있게 ㅎ
예를 들어 16 I = 100과 같은 식인데, 이 언어들은 인
파일러라는 것에 의해 기계어로 거꾸로 번역이 aaa See eae ©
로그램을 Hay 곧바로 기계어로 번역하는 도구인데, 프로그램 명령어 또
rapes ihe 나갑니다. 컴파일러는 원시 SES 일단 중간적인 ‘|
엇`으로 만듭니다. 이 과정을 컴파일이라 하고, 이를 가리켜 '컴파일러는 목적 파
일을 만든다'라고 합니다. 그 다음에 컴파일러는 링크라는 과정을 수행시켜 =z
파일을 실행 파일로 만듭니다.
인터프리터는 ACS 쓰여진 대로 읽고 그때그때 수행하므로 프로그래머가 작업
하기가 agian  ilies iil a Bathe 다른 과정을 alana aks



===== PAGE 28 =====
제1일 C++ 시작 ee 25

게다가, 또 하나의 장점은 일단 컴파일된 실행 파일은 컴파일러를 갖지 않은 다
른 사람들에게 나누어 줄 수 있다는 점입니다. 인터프리터로 수행되는 프로그램

은 실행시 인터프리터가 반드시 필요합니다.

오랫동안 컴퓨터 프로그래머의 일차적인 목적은 빠르게 수행되는 한 짧은 코드를
작성하는 것이었습니다. 메모리가 비싸므로 SEE 짧아야 했고, 또 수행시키는

물적인 자원들도 HR] 때문에 되도록 짧은 시간에 작업을 마칠 수 있어야 했습
니다. 그러나 컴퓨터가 점점 소형화되고, 가격은 내리고, 속도는 빨라짐에 따라
지금에 와서는 컴퓨터 자원을 BS 노력보다는 프로그래머의 생산성을 높이
려는데 그 노력이 기울어지게 되었습니다. 사업적인 관점도 그 방향으로 눈을 많
이 돌리게 되었습니다. 아주 잘 짜여진 유지 보수가 용이한 코드가 이제는 최고
가 되었습니다. 유지 보수가 쉽다는 BE 다음의 의미입니다. 사업은 계속 변화를
필요로 하므로 이를 뒷받침하는 프로그램이라는 것도 그때마다 큰 지출이 없이

쉽게 확장되고 AAS 수 있다는 의미입니다.

|

rir 『

프로그램이란

“프로그램"이라는 단어는 두 가지 뜻으로 사용됩니다. 프로그래머에 의해 창조된
각각의 명령어 혹은 원시 코드를 말하기도 하고, 또 하나는 실행시킬 수 있는 전
체 소프트웨어를 의미하기도 합니다. 이 구분은 때때로 상당한 SAS 야기하기
도 하는데, 따라서 앞으로 이 책에서는 원시 코드와 실행 파일을 따로따로 구분
하려 합니다.

&
&


===== PAGE 29 =====
26 ee AS

문제 oa 방식
프로그래머들이 해결해 온 문제들은 WAS 거듭해
그램은 많은 원시 이          몰
ㆍ램을 사용하는 사람은 모두 컴
사람들에 의해 사용되는  eu, 대부분은 |컴퓨터와 프로그램의 작동 더 ae pen
알뿐입니다. 과거 컴퓨터 그 자체와 싸움하던 시절은 지나갔고 이제는 사업상 문
AS 해결하기 위해 컴퓨터를 이용합니다.

at)
ra Se
rd
“
x2
ry
fe
a
nl
oe
a
+H
te
t,t
re |
ge
8무
rlo

역설적이기는 하지만 이 새로이 등장한 관중들에게 쉽게 사용되기 위해 프로그램
은 더욱 더 수사적으로 되었습니다. 지난 날 사용자들은 원시 ABS 흐름을 보
기 위해 비밀스럽기 조차한 프로그램에 암호 같은 명령들을 입력했습니다. 오늘
날 프로그램은 다중 윈도우와 메뉴들, 다이얼로그 상자들 같은 복잡한 도구들을
사용합니다. 이런 시도들을 지원하기 .위해 만들어진 프로그램은 10년 전 것보다

훨씬 복잡합니다.

프로그램에 대한 요구가 Mo] 따라 프로그램 언어와 제작 기법이 진화되어 왔
습니다. 순차적 프로그래밍으로부터 객체 지향 프로그래밍으로 전환되어 가는 흥
미로운 역사에 초점을 맞춰보겠습니다.

순차적 프로그래밍, 구조적 프로그래밍, WA 지향 프로그래밍
최근까지 프로그래밍이란 자료에 어떤 행위를 가하는 일련의 과정으로 생각되었
습니다. 프로시저 혹은 함수는 순차적으로 실행되는 특정 명령어들의 집합입니다.
자료들은 프로시저로부터 분리되어 있었고, 프로그래밍 기법이란 어떤 함수가 어
떤 함수를 부르는가, 어떤 자료가ㆍ바뀌었는가를 추적하는 방법들이었습니다. 이러

한 혼란스런 상황을 해결하기 위해 구조적 프로그래밍 기법이 만들어졌습니다.

구조적 프로그래밍 뒤에 숨은 첫째 AS 소위 “분열시킨 A 차례로 정복한다"
는 군사 전략처럼 간단합니다. 프로그램이란 일련의 작업 단위의 집합으로 이루
어졌다고 생각될 수 있습니다. 너무 복잡해서 쉽게 설명될 수 없는 어떤 프로그
램도 아주 작은 수행 단위로 분해될 수 있고, 이는 또 다시 쉽게 이해될 수 있는
최소 단위로 쉽게 분해될 수 있습니다.

{af

예를 들어, 회사의 모든 SYM] 평균 임금을 구하는 일은 매우 복잡할 수 있습
니다. 하지만 이 작업을 다음과 같이 나누어 전개할 수 있습니다.



===== PAGE 30 =====
제1일 C++ 시작 ee 27

새로운
응어

3. 금여를 모두 더한 뒤
4&5 금여를 총 인원으로 나눈다
급여를 모두 더하는 과정은 다음과 같습니다
1, 2} 고용인의 레코드에 접근하여
2. 금여를 알아낸 뒤
3 각 SOS 현재까지의 총액에 더하고
@ 다음 고용인의 레코드로 넘어간다.
다음 각 고용인의 레코드를 구하는 방법은 또 나누어집니다.

구조적 프로그래밍은 복잡한 문제를 처리하는데 상당히 성공적인 방식으로 여겨

집니다. 하지만 1980년대 후반에 이르러 구조적 프로그래밍의 결함들이

러나기 시작했습니다.

첫째, 자료들은(고용인 레코드 등) 그 자료들을 가지고 처리할 수 있는 여러 가지

일들(정열, 편집, 기타 등등)과 연관지어 생각하는 방법이 자연스럽습니다.

둘째, 프로그래머는 자신들이 그 오래된 문제들에 대해 비슷한 해결 방식들을 자
꾸 만든다는 것을 알게 되었습니다. 비슷한 것을 자꾸 만들어 내는

소위 '재사용" 철학과 정반대로 대치되는 개념입니다. 재사용이라는

알려진 각 구성 부분을 표준 형태로 만들어 놓고, 그것들이 필요할 때마다 그때
그때 끼워 맞추는 것입니다. 이는 하드웨어에서 나온 개념입니다. 기술자는 트랜

지스터가 필요할 때 새로 만들어 내지 않습니다. 부속 창고로 들어가서 기존의
원하는 트랜지스터를 찾아내어 끼워 Bey. 불행히도 소프트웨어 기술자에겐
이런 것이 없습니다.

사건 구동 HAl(Event-driven) 지금 0, 개.  sie HELE 가지고 컴퓨터를
=

사용라는 방식은 좀더 강력한 사건 구

2
하는 방식입니다. 프로그램은 더욱 대화식이 되고

°
=             을
이러한 부류의 함수를 설계하는 것이 매우 중요하게 되었습니다.

ㅇ
BAG, 현재의 사건 구동 방식은 모든 AS 한 번에 하고 또 컴퓨터는 이에

즉각적으로 반응합니다.


===== PAGE 31 =====
28 ee 제1주

ap 기량 프로그리밍은 als 요구에 부응되도록 만들어졌는데, 엄청나게 복잡
한 BASS 처리하는 기술을 제공하고 각 소프트웨어의 구성 분자를 재사용할
수 있게 하며 자료와 그 i 가지고 작업하는 업무 사이의 관계를 밀접하게
만듭니다

객

체 지향 프로그래밍의 %   ae 자료 및 그 자료를 가지고 조작하는 과정을 하나
는 것이고 그 객체는 자체의 동질성과 자신만의 특성

6++과 AA 지향 프로그래밍

CH+2 객체 지향 프로그램을 완전히 지원하는데 이의 4대 핵심은 캡슬화, 자료

캡슬화와 자료 SE (Encapsulation and Data Hiding)
를       7  ales AQIS 필요로 할 때 이 기술자는 저항기를 새로
요는 없습니다. |저항기 창고로 가서, 각 특성을 나타내는 규
표를 보고 빌요한: oe 골라옵니다. 저항기는 소위 “블랙박스`인데 저항기가 기
기만 하면 그 저항기가 어떻게 돌아가는지 알 필요가 없

고, 내부 구조가 어떻게 이루어졌는지 알 필요가 없습니다

자기 완결 구조를 갖고 있는 한 단위의 특성을 '캡슬화"라 부릅니다. 그 캡슬화를
가지고 우리는 AR SYS 이룹니다. 자료 은닉이란 그 캡슬화된 한 단위의 내
부 구조를 잘 몰라도 사용될 수 있는 특징을 말합니다. 마치 냉장고 안에 있는 압
축기 같은 것을 잘 몰라도 냉장고를 잘 사용하듯이, 자료 멤버(나중에 MSU)
라는 것을 몰라도 잘 설계된 객체(역시 나중에 SYS 사용할 수 있습니다.

유사한 예로 기술자가 저항기를 사용할 때, 기술자는 저항기의 내부 상태를 알
필요가 없습니다. pits 모든 SAL 저항기라는 객체 안에 캡슬화되어 있는
데 그 내부 특징은 전기회로 바깥 부분과 독립적으로 존재합니다. 저항기를 효율
적으로 쓰기 위해 내부 동작 원리를 굳이 잘 알 필요도 없습니다. 그 ASE A
항기 내부에 잘 은닉되어 있습니다.

+은 사용자가 정의한 어떤 형(이껏을 클래스라 DS 만들게 함으로써 캡슬화

와 자료 은닉의 특징을 잘 구현하게 합니다. 6일째 되는 날 독자들은 이것을 맛
보게 될 것입니다. 일단 만들어졌다 하면 잘 정의된 클래스는 캡슬화된 존재로
잘 사용됩니다. 클래스의 실제 내부 작동 구조는 은닉되어야 합니다. 잘 정의된



===== PAGE 32 =====
제1일 C++ 시작 ee 29

클래스의 ASAE 어떻게 클래스가 동작하는지는 알 필요가 없고 어떻게 쓰는지
만 알면 됩니다.

상속성과 MALS (Inheritance and Reuse)

자동차 회사 기술자가 자동차를 만들 때 두 가지 방법이 있습니다. A 번째 방법
은 처음 출발점부터 만들어 나가는 방법이고, 다른 방법은 기존 모델을 수정하는
방법입니다. WS 들어, 과거에 쓰던 '스타'라는 완벽한 모델이 있는데 여기에 터
보 엔진과 6단 변속 기능이 부가된 자동차를 만들려 합니다. 이때 고급 기술자는
새로 설계부터 다시 만들어 분여  기존의 “스타` 모델에 기능을 추가하고
이에 새로운 모델명 - dS 들어, “뉴스타' - 을 붙이기를 원할 것입니다. 이 Fe
AEPS 「스타`의 한 종류이긴 하지만 새로운 SAS 가진 모델입니다.

CHE 상속성을 통해 재사용성을 가집니다. 새로운 형태가 선언될 수 있는데 이
는 기존 형태의 확장일 수 있습니다. 이 새로운 부클래스는 기존 형태로부터 가
생되었다고 표현하거나 파생형(08000 046이라 블리기도 합니다. '뉴스타 모델
은 ‘AEP 모델로부터 파생되었고 따라서 “스타'형의 모든 특징들을 상속받았으며
더 나아가 새로운 특징도 추가되었습니다. 상속성과 그 에 대한 응용에 관해서는
12일째와 15일째에 배우게 될 것입니다.

Chi (Polymorphism)

'뉴스타 모델은 ‘AEP 모델과 가속기를 밝을 때 다르게 반응할 것입니다. 아마
"스타" 모델이 그저 가솔린만 엔진에 공급하는데 반해 '뉴스타" 모델은 새로운 터
보 충전기와 연료 분사기를 사용할 것입니다. 하지만 운전자는 그 엔진들의 내부
구조에 대해 자세히 알 필요는 없습니다. 단지 밝기만 하면 그에 따라 정확히 반
응할 따름입니다.

0++은 이러한 개념을 잘 지원하는데 각 다른 객체는 소위 ㆍ함수의 다형성'과 '클
AAS] 다형성'이라고 불리는 것에 따라 정확히 반응합니다. “다형(000-"이란 말
그대로 많다는 것을 의미하고, mophe = 것은 형태를 의미합니다. 다형성은 같은
이름에 여러 형태를 떠는 것을 가리키는데 10일째 되는 날과 13일찌 날에 공부할
것입니다.

=

C++2 어떻게 진화되어 왔는가?
객체 지향적인 분석과 설계, 프로그래밍이 유행하기 시작할 때 ye 스트라우스트
HW Bjame 50005080)"이라는 사람은 당시 상업용으로 크게 유행중이던 0언어에 객


===== PAGE 33 =====
30 ee 제1주

|  ee 특징들을 00 확장하였습니다. 그는 (++을 만들었는데, 초창기

만 쓰던 것이 지금 10년도 안되어 전세계 약 백만
자들이 agen g  는 = 파악되고 있습니다. 그리고 앞으로 10년째 0 해
에 +은 전세계에서 상업용 소프트웨어 개발에 있어 독보적인 언어가 될
니다.

CHE 0언어의 부분집합이고 0에서 쓰이는 것이 0++에서 그대로 쓰일 수 있는
것이 사실이지만, 0로부터 0++로의 도약은 매우 중요한 의미를 지닙니다. 0++은
오랫동안 0와의 관계 때문에 많은 이익을 얻었습니다. 왜냐하면 CH 배운 사람은
섭게 CHS 사용할 수 있기 매문입니다. 그러나 0++의 충분한 BAS 얻기 위해

서는 많은 프로그래머는 자기가 알고 있던 0의 MIS 버려야 하며, 새로운 개념
과 새로운 문제 해결 WIGS 익혀야 한다는 것을 발견합니다

ANSI

미국 국가 표준 7)|5+(American National Standards Institute : ANSI) 산하의 공인 3

준 위원회(&0060160 Standards Committee)= ++의 국제 HES 만드는 중입니다
이 표준 초안이 출간되었고 wwwlibertyassociates.comsS 통해 연결할 수 있습니다
ANSI HEE Cero] 모든 컴퓨터에서 동용되게 하기 위해 만든 것입니다 마이

a
fel Eel

크로소프트 컴파일러에서 오류 없이 돌아가는 것이 다른 업체의 컴파일러에서 잘
돌아가게 만듭니다. 이 책의 원시 HEE ANS HES 따라 작성되었으므로 맥,
알파 등 다른 업체 제품에서도 오류 없이 돌아갑니다.

표        동안 공인받아 왔으며] 대부분의 업체에서는 ANSI 표준을 지원합니
다. 이 책의 모든 “BEES ANS] HES 따르도록 하였습니다.

먼저 배워야 하는가?

반드시 다음 질문이 생길 것입니다. “0++은 0의 부분집합이므로 우리는 (를 먼
A 배워야 하는 거 아닌가?”

스트라우스트럽과 대부분의 다른 CH 프로그래머는 그 질문에 olga
다. CH 먼저 배울 필요는 없고 또 안 배우는 것이 좋을지도 모른
42 미리 CE 배우지 BE 사람들을 위해서도 만들어졌습니다. 사실 이 ALS 2
혀 프로그래밍 경험이 없는 사람들을 위해서도 만들어졌습니다.

  fr



===== PAGE 34 =====
제1일 C++ 시작 ee 31

프로그램 준비

CHe 다른 어떤 프로그램보다 실제 코딩에 들어가기 전 많은 설계를 요구합니
다. 사소한 문제들은 사실 그렇게 많은 설계를 필요로 하지 않지만 복잡한 문제
에 있어서는(직업적인 프로그래머가 매일 직면하는 문제이지만.) 설계가 Bas
니다. 철저히 설계하면 할수록 시간과 비용에 있어서 효과적으로 문제를 더욱 쉼
게 해결할 수 있습니다. 또 하나, 좋은 설계일수록 버그가 적고 유지 보수가 매우
용이한 프로그램을 만듭니다. 프로그램 제작 비용의 거의 90%는 디버깅과 유지
보수에 드는 비용이라는 사실은 잘 알려져 있습니다.

설계를 할 때 가져야 할 첫 번째 ALS “내가 풀고자 하는 문제가 무엇인가
입니다. 모든 프로그램은 명확하고 분명한 목표를 가져야 하고, 실제 이 책의 아
주 간단한 프로그램도 그렇다는 것을 여러분은 알게 될 것입니다.

훌륭한 프로그래머가 질문하는 두 번째 점은 “이 문제점을 기존의 소프트웨어를
사용하지 않고 해결하는 WHS 없을까?”입니다. 하지만 과거의 프로그램을 재활
용하거나 쉽게 구입할 수 있는 프로그램을 구매하는 것은 문제를 해결하는데 더
좋을 경우가 많습니다. 이러한 대안을 제시할 수 있는 프로그래머에게는 항상 일
}이 팔리지 않습니다. Lato] 문제를 해결하기 위해 저가의 해결책을 제시할

수 있는 프로그래머는 항상 새로운 기희를 창출할 수 있습니다.

이제 여러분이 문제점을 이해하였고 그 문제점을 해결하기 위해서 새로운 프로그
램을 짜야만 한다면, 이제 설계를 시작할 단계입니다.

oftN

oN

개발자의 개발 Z3(Development Environment)

이 AS 독자 여러분이 컴퓨터 스크린에 곧바로 Yas 할 준비가 되어 있다고
가정합니다. 그것이 윈도우이건 매킨토시이건 관계 없이 말입니다.

그리고 컴파일러는 자체의 편집기를 갖고 있거나 혹은 독자 여러분이 텍스트 편
집기 또는 위드프로세서를 갖고 있다고 가정합니다. 중요한 점은 어떤 편집기를
쓰더라도 그 편집기는 간단하고 평   a 파일 형태로 저장되어야 하며, 편집기 명
령이 텍스트 안에 포함되지 않는 형태로 저장해야 한다는 것입니다. 편집기 예로
는 윈도우의 Notepad, DOSS] edit 미리 | Brief, Epsilon, EMACS, vi 동이 있습니다.
그 외에 WordPerfect} Word 같은 많은 편집기들이 좋은 기능을 제공합니다.

~


===== PAGE 35 =====
32 ee AIS

편집기로 여러분이 만드는 파일을 원시 파일
CPP 또는 CP 혹은 .0라는 확장자를 갖고 있는데 이 책에서는 CPP 확장자를
쓸 예정입니다. 여러분의 컴파일러를 한번 조사해 보기 바랍니다.

대부분의 ++ 컴파일러는 원시 코드에 어떤 확장자를 주어도 관계하지 않지만, 여러

분이 특정 확장자를 지정하지 않는 한 기본값으로 .0를 설정합니다.

BO    원시 SEB 작성하기 위해 단순 명료한 AMIE 사용하거나 컴파일러에

불어 나오는 편집기를 SH

DONT 특정 편집 명령을 파일 안에 같이 저장하는 편집기를 사용하지 마시오. 만
일, 그러한 편집기를 사용한다면 Asc 형태로 저장하시오

00    파일을 .C, .CP, CPP 확장지로|적장빅시오

DONT 당신의 컴파일러와 링커에 맞는 컴파일 방법 및 링크 방법을 DI 위해 사
용자 지침서를 확인하시오

원시 코드 컴파일하기

원시 코드는 다소 비밀 같은 부분도 있고
무척 애를 쓰기도 하지만 그럼에도 불구하고 원시 SEE 인간이 읽을 수 있
태로 되어 있습니다. 여러분의 원시 코드는 실행할 수 있는 프로그램이 아닙니다.

여러분의 원시 코드를 실행 파일로 바꾸기 위해서 여러분은 컴파일러를 써야 합
니다. 어떻게 컴파일러를 부르고, 또 어떻게 컴파일러가 여러분의 원시 코드를 찾
아내게 하는지는 컴파일러마다 다르므로 안내서를 참조하기 바랍니다. 예를 들
800000의 Turbo C++] = 메뉴 화면에서 RUNS 선택하거나 또는

Q
+
+
tuo
년
ru
rr
»
Beas
at
ro
pos
0!
40,
oN

tc <filename>

을 명령 줄에서 입력합니다. 여기서 <0160806>은 여러분의 원시 코드 파일명입니
다.(예를 들어, 69000) 컴파일러마다 조금씩 다를 수 있습니다.



===== PAGE 36 =====
제일 C++ 시작 ㅎㅇ 33

여러분이 운영체제에서 원시 코드를 컴파일을 하려면 다음을 입력합니다.

Borland C++ 컴파일러            bec (filename)
Borland C++ HES 컴파일러 666 (filename)
Borland Turbo C++ 컴파일러       te (filename)
마이크로소프트 컴파일러          cl (tilename)

여러분의 원시 코드가 컴파일되면 목적 파일이 생성됩니다. 이 목적 파일들은 보
통 확장자가 .081입니다. 이 목적 파일은 아직은 실행 파일이 아닙니다. 실행 파
로

일로 만들기 위해서는 링커를 수행시켜야 합니다.

GAS 가지고 실행 가능한 파일 만들기

CH 프로그램은 하나 이상의 OBI 파일을 하나 이상의 라이브러리 파일들과 링
크함으로서 생겨납니다.

라이브러리라는 것은 여러분이 만들거나, 컴파일러에서 주어지거나 혹은 여러분
이 어디선가 따로 구입한 파일로 링크할 수 있는 파일들입니다. 모든 cH 컴파일
러들은 유용한 함수들 - 혹은 프로시저들 - Fe 여러분 프로그램에서 사용할 수
있는 클래스들의 라이브러리들과 함께 제공됩니다.

함수라는 것은 일정 서비스를 제공하는 SES] 한 덩어리로, 예를 들면 숫자 두
개를 더하거나 화면을 출력하는 것 등입니다. 클래스라는 것은 자료들의 집합 및
관련 함수들의 집합인데 5일째의 “함수 편에서 함수에 대해 많이 논할 것입니다.

oO
022
|
=
ne
qin
milo

mE!
to
rok
fu
2

1ㅁ
fe
그
mn
ng
=
ou
Lu
그
Yt!
[>
ost
브
med
nulo
므
ain
ie
Kal

개발 27|(Development Cycle)
Z 프로그램을 개발하여 완전한 동작이 되는 순간의 전체 과정은 하나의 개발 주
기를 통해 이루어집니다. 프로그램의 aa  원시 코드 컴파일, 링크 및 실행의 단
계입니다. 불행히도 대부분의 많은 프로그램은 아주 사소한 것일지라도 장애와


===== PAGE 37 =====
34 ㅎㅎ 제1주

[그림 1.1]
C++ 프로그램 개발
의 2} 단계들

러분은 버그를 잡아야 하고, 원시 코드를 수
1

및 ae 를 고  | 하며 마지막에 재실행해야 합니다. [그림

그들은 컴파일을 중지시키고,

0보

_—

A

원시화일

편집
+

컴파일

Lt Y

컴파일오류

아니오

예



===== PAGE 38 =====
제1일 C++ 시작 ee 35

HELLO.CPP --- 24 번째 C++ 프로그램 작성
전통적인 프로그래밍 BSL “Hello \000!”라는, 또는 유사한 문장을 화면에 한
번 써보는 프로그램을 짜보는 것부터 시작합니다. 그 오            도
해보고자 합니다.

S
(쏘
에
lo ㄷ
2
SS
Es

다음에 있는 첫 번째 프로그램을 직접 편집기에 입력합니다. 맞게 입력했는지 파
일을 저장하고 컴파일한 뒤 실행해 봅시다. 여러분의 스크린에 “Hello '\000!”라
는 문장이 출력될 것입니다. 어떻게 SAS 한 것인지 너무 궁금해할 BRE 없
습니다. 지금은 여러분이 개발 주기를 한 번 거쳐보게 하는 것이고, 앞으로 이틀
동안 이 프로그램에 대해 자세히 알아볼 것입니다.

Hinclude (iostream.h)

[리스트 1.11 HELLO.CPP, Hello World 22724

: #include <iostream.h>

1

2
3: int main()

ae <

5    cout << "Hello World!\n";
6      return 0;

7

프로그램을 예제에 주어진 대로 정확히 입력합시다. 구두점을 주의합시다. 5번
의 << 기호는 AAA 기호인데 대부분의 키보드에서는 <Shift>7] 9 <<]>키를
시에 누르면 입력이 됩니다. se So] 세미콜론으로 끝나는 것에 주의합시다. wl
=)
i=]

off 뼈

분이 갖고 있는 컴파일러의 지시에 잘 따라야 합니다. 대부분의 컴파일
적으로 링크를 하지만 다시 한번 사용 안내서를 확인하기 바랍니다. 만

일 장애가 발생하면 여러분이 입력한 코드를 자세히 살펴보고 무엇이 잘못되어

있는지를 발견합니다. 1번 줄에서 장애가 발생되면, y= 들어 “cannot find file


===== PAGE 39 =====
36 ee 제1주

iostreamh”2}= 장애가 발생되면 컴파일러 안내서를 살펴보아 “include path” 혹은
“environment variables” 사항을 설정합니다. “main” 원형을 발견하지 못한다는 장
애가 발생하면 3번 줄 전에 “int manos 입력합니다. 이러한 컴파일러를 가진

독자는 모든 프로그램의 min 함수 전에 이 SES 항상 입력해야 합니다. 물론
대부분의 프로그램은 이런 일을 필요로 하지 않습니다.

여러분의 원시 프로그램은 다음과 같이 될 것입니다.

: #include <iostream.h>

1

2
3:
4: int main()

를

6    cout << "Hello World! \n";
7      return 0;

88 +

이 FAIS 실행하면

Hello World!

라는 문장이 여러분의 화면에 곧바로 나타날 것입니다. 제대로 됐다면 축하합니
. 여러분의 a 번째 C++ 프로그램의 입력과 컴파일, 실행이 성공적으로 끝난
입니다. iia 일이 아닌 것처럼 보이지만 BE C++ 전문가들도 이렇게 정확
; 프로그램으로부터 시작하였습니다.

럼파일 OFS

컴파일 장애는 여러 가지 이유 때문에 나타납니다. 대부분은 입력 실수나 그 외
사소한 부주의 때문에 일어납니다. 좋은 컴파일러는 대개 무엇이 잘못되었는지와
어디에서 잘못되었는지를 자세히 말해줍니다. 더욱 좋은 컴파일러는 어떻게 장애
를 수정할 것인지도 알려줍니다.

부러 dee 만들어 장에 데시지를 보기로 합시다. 18110.00까 잘 수행되는
것을 확인했으면 6번 줄의 중괄호를 없애보기로 합시다. 즉, [리스트 1.2|와 같이
입력하는 것입니다

[리스트 1.2] 컴파일러 오류의 보기

1: #include <iostream.h>
28



===== PAGE 40 =====
제1일 C++ 시작 ee 37

3: int main();

4G: 1

5    cout <<"Hello World! \n";
6       return 0;

다시 컴파일을 하면 다음과 같은 오류 LIS 보게 될 것입니다.

Hello.cpp, line 5: Compound statement missing terminating } in
function main().

이 오류 HAS 여러분에게 파일 이름, S 번호, 그리고 무엇이 문제인지를 알려
줍니다.(다소 난해하게 표현하기도 하지만) 오류 메시지가 여러분에게 SH SS
지적하였음을 주의 깊게 봅시다. 컴파일러는 중괄호를 5번 줄 마지막 칸에 넣어
야 할지 또는 6번 줄 처음에 넣어야 할지 잘 판단을 못합니다. 따라서 오류 메시
지는 가끔 오류 난 곳의 근처를 지적하기도 합니다. 컴파일러 오류를 모두 찾아
내어 고쳤으면 이 프로그램 코드를 확정합니다.

1장을 읽고 난 후 여러분은 C++] 어떻게 발전해 왔으며 어떤 문제를 해결하기

| 알게 되었을 것입니다. 0++을 배우는 것은 다음 시대의 프로
관심 있는 사람에겐 탁월한 선택임을 자신있게 확신할 것입니다. 0++은
객체 지향 프로그래밍의 유용한 도구이며 시스템 수준에서 좋은 수행성 또한 보
장하는데, 이것이 C+ 프로그램을 개발 언어로 선택하게 만드는 이유입니다.
오늘 여러분은 어떻게 프로그램을 입력하고, 컴파일하며, 수행하는지 배웠고 일반
적인 개발 주기에 대해 알아보았습니다. 그리고 객체 지향 프로그래밍에 대해 약
간 알아보았습니다. 앞으로 3주 후에 다시 이 주제를 접하게 될 것입니다.

O&A

Q 텍스트 편집기와 워드프로세서의 차이점은 무엇입니까?
A 텍스트 편집기는 단순히 텍스트만을 만들어 Yo. El 명령어나 특별한 워드프
로세서에 필요한 특수 기호는 없습니다. 텍스트 파일은 Fe 글씨체라든가 이탤릭
체 같은 서체 형식, 줄 BAIA 단어가 잘릴 것 같을 때 알아서 자르지 말고 다음

줄로 이동시켜 주는 기능 같은 것이 없습니다.


===== PAGE 41 =====
38 ee 제1주

나의 컴파일러 안에 내장된 편집기가 있을 때 반드시 그것을 써야 하는지?

쇼 대부분 모든 컴파일러는 어떠한 텍스트 편집기로 만든 원시 코드도 컴파일합니다.
하지만 내장된 편집기를 쓸 때 편리한 Ge 개발 과정의 사이클 도중 쉽게 컴파일
러와 편집기 사이를 앞뒤로 왔다갔다하게 해 준다는 것입니다. 기교적으로 잘 만들
어진 컴파일러는 완전히 통합된 개발 SA(integrated Development 80\170001601)을 지

원하는데 개발자가 도움말 파일을 보다가 편집도 하고, 그러다 컴파일도 하며, 또
그 중간에 컴파일 및 링크 장애도 볼 수 있게 해줍니다.

컴파일러의 경고문을 무시해도 좋습니까?

A 많은 책들이 이 문제에 대해 애매한 태도를 취하는
히 말합니다: 오늘부터 경고문을 장에로 간주8
러분이 의도하지 않은 행동을 했을 때 경고를 하
기울이고 경고문을 제거하도록 노력합시다,

| Aare '아님니다"라고 단호
He 갖도록 함시다. Cre 이
We

Q Hale! 시간이란 무엇인지?

A 컴파일 시간이란 여러분이 컴파일러를 수행시키는 시간을 말하며 링크를 수행시키
는 링크 시간, 또는 실행 파일을 실행하는 실행 시간과는 다릅니다. 오류 발생시 이
세 개의 시간을 구별하여 어느 단계에서의 오류인지 구별하는 것이 오류 처리 시간
을 절약해 줍니다.

연구

이 연구란은 이번 장에서 다루어진 FAS 여러분이 얼마나 잘 이해하였는가를
Hele 보는 퀴즈들과 여러분이 Me 것을 시험해 블 수 있는 연습 EAS 구
성되어 있습니다. 부록 에 있는 답을 보기 전에 각 물음에 대답을 할 수 있도록
노력하고, 다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다.

1, 인터프리터와 컴파일러의 차이점은?

2 컴파일러로 여러분이 제작한 원시 BES 어떻게 컴파일합니까?
3% SAS FAS 합니까?

4 개발 주기의 A 단계는 무엇입니까?



===== PAGE 42 =====
제1일 0++ 시작 ㅎㅇ 39

연습 문제

1 다음 프로그램을 보기만 하고 무엇을

Ol
다

프로그램인지 짐작하여 봅시다.

: #include <iostream.h>
: int main()

‘                      ja  3G.
int x =5;

int y=7;                    —

cout "\n";                c (L, 3
: cout <x ty <e" "KKK Ry, N

© cout "내";
zreturn 0;
Os}

그 OANA VMUFWNDN =

x
do
10
>t
re
2
[FI

로그램
습니까?

3. 506 을 입력하고 컴파일합시다. 어떠한 오류가 나타났습니까?
00 <iostream.h>

: int main()

5

: cout << "Hello World\n";
은 return O;

글

ilo

입력하고 Auge 뒤 링크합시다. 무엇을 하였습니까? 여러분

jo
건
건
으
| ㅁ
+O

nu EW PP

[개
wo

번 질문의 프로그램에서 OFS 찾아 고처봅시다. 그리고 컴파일, 링크, 실행을 해봄시
다. 무엇을 합니까?
 그

=) Welle … "As


===== PAGE 43 =====
oo
에어 08



===== PAGE 44 =====
C++ 프로그램의 각


===== PAGE 45 =====
42 ee A=

서

2
a

CH 프로그램은 대상체, 함수, 변수 그리고 기타의 다른 부분으로 구성되어 있습
니다. 이 책의 RRS 각 부분에 대해 깊이 AVS 하고 있지만, 먼저 어떻게
감            =

프로그램이 구성되어 있는지 감을 잡기 위해 우선 하나의 완전하게 돌아가는 =
로그램을 살펴보도록 합시다. 이것이 오늘 여러분이 공부할 내용입니다.

McH 프로그램의 각 부분

첫 번째 날 배운 HELLOCPP 프로그램을 보면 홍미있는 부분이 많습니다. 이번
주제에서는 이 프로그램을 좀더 자세ㅎ        것입니다. [리스트 2.1]은
HELLO.CPP2} 원래 버전을 편의상 다시 보

러
AN
yy 이
re
cu
된

[리스트 2.1] HELLO.CPP C++ 프로그램의 3 부분 al

: #include <iostream.h>

1

25
3: int main()

4: f

5    cout << "Hello World! \n";
6   return 0;

7

lg  Hello World!

분석  첫째 줄에서 10606804가 파일에 포함되어 있습니다. A 번째 문자는 # 기

호인데, 이는 전처리계060000500에게 보내는 신호입니다. 여러분이 컴파
VIS 수행할 때마다 전처리계가 수행됩니다. 전처리계는 여러분의 원시 코드를
읽어 내려가면서 # 기호로 시작하는 줄을 찾아내어 컴파일을 시작하기 전 해당
줄에 어떠한 동작을 수행합니다.

100006는 전처리계에게 다음과 같은 명령을 내립니다. “다음에 오는 것은 파일명
인데, 그 파일을 찾아 여기로 읽어들여라”. 한편 파일명 앞뒤의 각괄호는 전처리
계에게 다음과 Zo] 말합니다. “이 파일을 지정된 모든 장소에서 찾아라” 만약

©:



===== PAGE 46 =====
제2일 C++ 프로그램의 각 SHES eo 43

여러분의 컴파일러가 올바르게 설정되어 있다면 각괄호는 전처리계로 하여금 파
일 iostreamhS 여러분의 헤더 파일들을 저장하는 장소에서 찾아낼 것입니다. 파
일 iostream.h(Input-Output 5184540)은 004에 의해 사용되는데 스크린에 출력하는
기능을 합니다. 1번 줄의 FSS iostreamhS 마치 여러분이 직접 입력한 것처럼
여러분의 원시 파일에 포함하는 기능을 합니다.
새로운 BAA 전처리게는 컴파일러가 사용될 때 컴파일 바로 전에 ep 니다. + 기로
SO 로 시작하는 SS 특별한 명령으로 해석하여 컴파일이 실행되도록 준비를 갖추게 합

니타.

3번 줄은 2800이라는 함수로 실제 프로그램을 시작합니다. 모든 C+ 프로그램
은 main() 너티 갖고 있습니다. 일반적으로 함수란 하나 히장의 동작을 수행하
도록 고안된 한 단위의 원시 코드입니다. 일반적으로 함수는 다른 함수에 의해
불려져 as main) 함수만은 다릅니다. 여러분의 aa 프로그램이 처음
시작할 때 0800은 자동적으로 호출됩니다.

main)? 다른 함수와 마찬가지로 어떤 종류의 RS 되돌려주는지 기술해야 합니
다. 여기서의 반환되는 값의 BS inte] 이것은 정수값을 반환한다는 의미입니
다. 반환값에 대한 이야기는 4일찌 되는 날에 배울 것입니다.

모든 함수는 열기중괄호 {로 시작하고 닫기 중괄호 }로 끝납니다. ㅁ800함수의
중괄호들은 4번 줄과 7번 줄에 있습니다. 열기중괄호와 닫기 중괄호 사이의 부

이 함수의 몸체입니다.

이 함수의 AAS SH So] 있습니다. 객체 004는 메시지를 스크린에 출력하는데
쓰입니다. 객체에 대한 일반론은 6일째 되는 날 학습할 것이고 004 및 그와 관계
되는 cin] 대해서는 17일째 되는 날 배울 것입니다. 004과 00이라는 객체는
0++에서 문자열과 값들을 스크린에 출력하는데 쓰입니다. 문자열이란 문자들의
집합입니다.

다음이 cout?] 용법입니다. cout: 출력 재지정 연산자(<<) 다음에 오는 단어를 출
력합니다. 어떤 것이 와도 출력합니다. 문자열을 출력하고자 할 때에는 BAAS
쌍따옴표(“로 막도록 주의합시다.

새로운

응이   텍스트 BAA (Text String) 텍스트 문자열은 출력할 수 있    작들의 나열입니다.

Tlo
rir
Au

마지막 두 문자02)는 cout 하여금 8610 World! 뒤에 SS 바꾸라는 의미입니다.
이 특수 코드는 17일째 우리가 004에 대해 자세히 배울 때 설명됩니다.


===== PAGE 47 =====
44 ee 제1주

= ANSI 표준 함수는 mando] 정수형을 반환하도록 선언합니다. 이 값은 프로
그램이 끝날 때 운영체제에 반환됩니다. 어떤 x     들은 오류가 발생할 때
1 값을 반환하도록 합니다. 이 책에서는 0000은 항상 0을 반환합니다.

main) PE 7번 줄에서 끝내기 중괄호와 함께 종료합니다.

갑단힌 살퍼보는 60나

16일째 되는 날 우리는 cout7} 자료들을 출력하기 위해 어떻게 하는지를 MH
다. 하지만 이제부터 우리는 004가 어떻게 동작하는지 충분히 알지 못하더라도
사용합니다. 값을 화면에 출력하기 위해 cous 쓰고 그 다음에 출력재지정 연산
자(<<)를 BUC. 비록 2개의 문자이지만 0+은 그들을 한번에 처리합니다.

입력연산자 다음에 출력을 원하는 ASS 입력합니다. [리스트 2기는 그 예를 보
여줍니다. 예제에 있는 대로 정확히 입력하도록 합시다. 단 Jesse LibetyS 여러분
이름으로 바꾸어도 괜찮습니다.

[리스트 2.2] cout 사응

1: // [리스트 2.23 cout 사용법

2:

3: #include <iostream.h>

4: int mainQ)

57 +t

6:   cout << "Hello there.\n";

te    cout << “Heré is 5: ™ <<.5 지니

ou    cout << "The manipulator endl writes a new Line to the screen." << endl;
os   cout << "Here is a very big number:\t" << 70000 << endl;

10: cout << "Here is the sum of 8 and 5:\t" << 8+5 << endl;

11: cout << "Here's a fraction:\t\t" << (float) 5/8 << endl;

12: cout << "And a very very big number:\t" << (double) 7000 * 7000 << endl;
13: cout << "Don't forget to replace Jesse Liberty with your name...\n";
14: cout << "Jesse Liberty is a C++ programmer!\n";

15: return 0;

16: }

Hello there

Here is 5: 5

The manipulator end1 writes a new Line to the screen.
Here is a very big number: 70000



===== PAGE 48 =====
제2일 C++ 프로그램의 각 부분들 ce 45

Here is a sum of 8 and 5:   13

Here's a fraction:        0.625

And a very very big number 4.9e+07

Don't forget to replace Jesse with your name...
Jesse Liberty is a C++ programmer!

분석  3번 줄 문장 #include <10900801.11>은 1050608011 파일을 여러분의 원시 코드
~ 에 삽입합니다. cout 및 그와 관계된 함수들을 쓰려면 반드시 필요합니다.

6번 줄은 BAGS 출력하는 004의 가장 간단한 사용 예입니다. we 특수 기호
로 스크린에 개행 문자를 출력한다는 의미입니다.

TH 줄에서 3개의 Zo] cout] 전달되었습니다. 각각 입력연산자에 의해 분리되어
있습니다. Al 번째 값은 “Here is 5: ”입니다. 콜론 뒤에 빈칸문자가 있고 그 역시
문자열입니다. 다음 5라는 값이 입력연산자 다음에 전달되었고 다음에 개행 문자
가(항상 BUSEY 홀따옴표로 둘러싸임) 전달되었습니다. 이로써

Here is 5: 5

가 출력됩니다. A 번째 문자열 뒤에 개행 문자가 없어서 다음 문자열은 앞의
AS 뒤에 붙어서 출력됩니다. 이를 두 WS “연결(000086608008)”한다고 합니다.
8번 줄에서 정보를 나타내는 메시지가 출력되고(600이가는 연산자가 쓰였습니
다. 6001은 개행 문자를 쓰라는 의미입니다.(600의 다른 의미는 16일째 배울 것입
니다.)

9번 SoA] 새로운 문자 Wl 쓰였습니다. 이는 탭문자를 입력하자는 뜻인데 8부
터 12번째 줄까지 줄을 맞춰 출력하기 위해 쓰였습니다. OW 줄에서 정수뿐만
니라 long 정수도 출력됨을 보여줬고, 10H SS cout7} 간단한 덧셈을 할 수
다는 것을 보여주는데 8 + 57} cout 전달되어 13이 출력됨을 보여줬습니다.

11번째 SA} 5/8이 cout 입력되었습니다. (0080의 의미는 Zo] 소수로 측정되
기를 원한다는 의미이고, 따라서 소수 He] 출력되었습니다. 12번째 줄에는 7000
* 7000°] cout] 출력되었고, 또 (40004010라는 값이 쓰였는데 이는 004에게 과학적
기호로 출력하자는 의미입니다. 이들 모두 3일째 되는 날 자료형에서 배울 AQ
니다.

14번째 줄에 Jesse 11660》(또는 여러분이 임의로 집어넣은 이름)와 Fy] is a C++
Programmer! 2}= 말이 나올 것입니다.

Be

ㅇㅇ
는 0

pees


===== PAGE 49 =====
46 ee 제1주

2A4(Comments)

프로그램을 MASE 도중에는 여러분이 입력하는 모든 내용이 명백하고 자명합
니다. 하지만 한달 후 여러분이 그 프로그램을 보았을 때 도대체 이해할 수 없는
경우가 많이 발생합니다. 어떻게 그렇게 했는지 모르겠지만 BAY 그 프로그
램은 여러분이 입력한 그대로인 것입니다.

이러한 경우를 피하기 위해 주석을 달아놓을 필요가 있습니다. 주석은 컴파일러
에 의해 무시되는 단순 문장입니다. 하지만 프로그램을 Ye 사함에게는 그 부분
에서 무엇을 하는지 가르쳐 줍니다.

주석문의 형태

CH 주석문은 두 가지 방식이 있습니다. 겹사선(/이 그 하나인데 cH 컴파일러
에게 그 줄의 끝까지 주석이니 무시하라는 표시입니다.

또 다른 하나는 사선 별모양(인데 이는 컴파일러에게 별모양 + IE] 올
때까지 그 안에 모든 것들을 무시하자는 표시입니다. 이런 표기는 0에서 쓰이던
표기법입니다. 모든 /* 표시는 % 표시와 쌍을 이루어야 합니다.
이런 C 형태의 주석은 Co} 0++에서 쓰였지만 그렇다고 0++이 Co} 일부분이라고
공식적으로 선언한 것은 아닙니다.

많은 CH 프로그래머들은 대부분 CH 형태의 주석을 쓰며 0 형태의 주석문
프로그램에서 큰 부분을 무시하고 싶을 때 사용합니다. 그리고 C+ Bale] 주
문을 0 형태의 주석문 사이에 넣을 수 있습니다. C 형태의 주석문은 그 안에 %
모든 내용 - 심지어 CH 형태의 주석문도 - 모두 무시해 버립니다.

xo 4 ro

rr

주석문 쓰기

일반적으로 대부분의 프로그램은 시작 부분에 이 METS 소개하는 주석문을
가져야 합니다. 각각의 함수들도 역시 이 함수의 역할을 소개하고 반환값을 일러

는 주석문을 가져야 합니다. 마지막으로 프로그램에서 어렵거나 불명확한 부분
석을 달아놓아야 합니다.

기은 주석의 WIS 보여주는데 주석문은 프로그램의 진행을 방해하거
ea 영향을 끼치지 않습니다.

tlo +N

4

+i



===== PAGE 50 =====
제2일 C++ 프로그램의 각 부분들 ee 47

[리스트 2.3] HELP.CPP 주석의 보기

1: #include <iostream.h>

25

3: int main()

Ae {

5: /*주 4

6: 이 주석은 다옴에 FAB 표시가 SE 곳까지
7: 적용이 됨*

8    cout << — World! \n";

9:   // 이 주석은 한 줄만 해당됨
10: cout << "That comment ended!";
ib

12: // 접사선은 한 줄에 하나만 있으면 됨
13:  /* C 령태의 주석문도 한 줄만 주석으로 처리할 수 있음 */

14: return 0;
152 개

결과 Hello World!

That comment ended!

Ea Ay oul Ste] 7번 줄까지는 컴파일러에 의해 완전히 무시되고 9, 12, 13번째
줄도 마찬가지입니다. 9번의 주석문은 So] 끝남과 동시에 주석도 끝나는데
반해 5번과 13번 줄의 주석은 주석의 끝 표시가 필요합니다.

과 파일의 eel 필요한 주석들

를 작자 이름
mus

Mo) 프로그램을 만들기 위해 쓰여진 컴파일러, 링커, 그리고 다른 도구들
Mm 필요한 추가 사항


===== PAGE 51 =====
48 ee 제1주

예를 들어, 다음과 같은 주석문이 Hello World 프로그램 처음에 기록되어야 $F
니다.

[RR KKRKK RRR KER EK RRR KERR RRR KR 기가 세게 세 세 세 고 세 고 고 고 로 고 로 고 라고 개 고 소라 가 가 개 가 KERR EERE RK

Program:       Hello World

File:           Hello.cpp

Function:      Main (complete program listing in this file)
Description:    Print the words "Hello world" to the screen
Author:        Jesse Liberty (jl)

Environment:    Turbo C++ version 4, 486/66 3206 RAM Window 3.1
DOS 6.0 EasyWin module.
Notes:         This is an introductory, example program.
Revisions:     1.00 10/1/94 (jl) First release
1.01 10/2/94 (jl) Capitalized "World"
KKK KKK KKK KKK KKK KKK RRR KK IKE KKK RRR IK KR RRR RRR RRR KERR REE |

최근까지의 메모와 FAS 달아두는 것이 중요합니다. 일반적인 문제는 프로그래
머들이 처음에만 주석을 달고 그 다음부터 게을리 하는 것인데 그러다 보니 실제
코드 내용과는 다른 주석이 있어 이런 경우가 누적되면 상당히 잘못될 수가 있습
니다. 주석이 잘 유지되면 전체 프로그램에 좋은 안내자가 됩니다.

이 책의 나머지 부분에서의 예제에서는 지면을 절약하기 위해 주석들이 없을
입니다. 그렇다고 중요성을 간과해서는 안됩니다. 각 주의 마지막에 나타나는
로그램에서는 주석을 달아놓을 것입니다.

ja

hy

[Hl ya!

주석에 BEBE 마지막 주의 사항
명백한 것에 주석을 다는 것은 의미가 없습니다. 괜히 프로그램을 수
을 때 문제가 208 하지만 한사람에게 명확한 것ㅇ
에겐 불명확한 것이 될 수도 있습니다. 잘 관단하기 바랍니다.

정하
le

Hk

무궤

오조

DON'T

DON'T 자명한 코드에 주석을 달지 Brey,



===== PAGE 52 =====
제2일 C++ 프로그램의 각 부분들 eo 49

[아

스
~

10000도 함수인데, 다른 함수와는 다른 함수입니다. 전형적인 함수들은 프로그램
진행 도중 호출되거나 생성됩니다. 프로그램은 함수를 만날 때까지 한 줄씩 실행
됩니다. 함수를 만나면 그 함수로 분기가 됩니다. 그 함수가 끝나면 다시 제어권
을 그 함수를 불렀던 위치의 다음 줄로 즉시 넘겨줍니다.

비유를 하자면 연필까이를 예로 들 수가 있습니다. 그림을 그리다 age) 부러지
그리기를 멈추고 연필을 까습니다. 연필을 Ae 뒤 다시 그림 그리는 곳으로
아와 직전에 그리던 그 곳으로 찾아가 다시 그립니다. 프로그램이 특정 서비스
요구하면 그 서비스를 수행하는 함수를 부르고 그 함수가 끝나면 다시 원 위
치로 돌아옵니다. [리스트 2.4|에서 이 개념을 보여줍니다.                    |

Sd 때 ee 프

[리스트 2.4] 함수 BBQ al

#include <iostream.h>

1
2
3: // 함수 예제

4: // 메시지 출력함

5: void DemonstrationFunction()

6: 제

1     cout << "In Demonstration Function\n";
on 가

9:

10: // 함수 main 부분

11: // DemonstrationFunction();8 부르고
12: // 두 번째 메시지 출력

13: int main()

148 이

158   cout << "In main\n" ;

16:   DemonstrationFunction();
fies   cout << "Back in main\n";
18:   return 0;

19% 3

Ai » In main

a

In Domenstration Function
Back in main

함수 DemonstrationFunction()-<- 5 - 8H 줄에 정의되어 있습니다. 호출되었을
때 메시지를 출력하고 다시 돌아갑니다.


===== PAGE 53 =====
50 ee 제1주

프로그램의 시작입니다. 15번 SS main()o] “In 0080^이라는 단어
}라는 뜻입니다. 출력 후 16번 줄은 DemonstrationFunctionQS 호출합니다.

이 호출은 DemonstrationFunction) 안의 명령을 실행하게 합니다. 이 경우  실랭되
는 함수는 TH So] 있습니다. 호출된 함수가 8번 줄에서 끝났을 때 그 함수를
부른 다음 줄, 즉 17번 줄로 돌아와서|0000 JE] 마지막 SS 출력합니다,

함수느 us 되돌릴 수 있고 아무 값도 돌려주지 않기도 합니다. 두 개의 숫자를
그 합을 되돌려줄 수 있습니다. 이런 때에는 정수값을 되돌려줍

돌려줄 Ho] 없기 때문에 700로 선언됩니다.
머리0680)와 몸체(6005)로 구성됩니다. 머

함수는

함수로 전달되는 매개 변수(0800000060)들로 구성되
정 값들이 함수로 전달되게 합니다. 함수가 만약
두 7
니

오오
xe
7 |
을
ple
=
ea
4y
un
rlo

개의 숫자가 매개 변수로 전달될 수 있습니다. 전형적인

int Sum(int a, int b)

매개 변수는 어떤 종류의 값이 전달되는가 하는 선언이기도 합니다. 부르는 함수
에 의해 전달되는 an 인수(4840600)라고 합니다. 많은 프로그래머들은 매개 변
하기도 하고 다른 사람들은 기술적인 차이를 꼼꼼히

oft 30 ,

일하게 부를 것입니다.

함수의 BAL 시작 중괄호, 0개 이상의 NSE, 그리고 종료 중괄호로 구성되어
있습니다. Aes Ute 심제 Se 구성합니다 함수는 16000 문장을 통해
주료             ^
. FT

서술문은 함수의

dD
3일째 수업에서 좀더 배울 것입니다. 오늘 배운 것은 함

에서 쓰이므로 미리 데강 살펴본 See.

of rir oot



===== PAGE 54 =====
제2일 C++ 프로그램의 각 부분들 ㅎㅎ 51

[리스트 2.5]는 2개의 인수를 취하고 한 개의 정수 반환값을 가지는 함수의 예를
들었습니다. BAS 가지고 어떻게 동작하는지에 대한(예를 들면, int 30 자세한
정보나 구문에 구애되지 Walch. 이는 3일째에 다룰 것입니다.

[리스트 2.5] FUNC.CPP 단순한 함수 예

1: #include <iostream.h>
2: int Add (int x, int y)
of «
4:    cout << "In Add(), received " << x <<" and" << y << ""\n";
De    return (xty);
6: }
(4c
8: int main()
os: 그
10:    cout << "I'm in main() !\n";
415    Int ap by ce
12    cout << "Enter two numbers: ";
S's    Cin >> a;
14:    cin >> b;
190    cout << "\nCalling Add()\n";
16:    c=Add(a, b);
i AT Ge    cout << "\nBack in main().\n";
18:    cout << "c was set to" << c;
198    cout << "\nExiting...\n\n";
20:    return 0;
ue 2
Zi b I'm in main()!
Enter two numbers: 3 5

Calling Add()
In Add(), received 3 and 5

Back in main().
c was set to 8
EXTting)s os

(naa

AH 하수 4000는 2번 줄에 정의되어 있습니다. 두 개의 정수 인수를 갖고 정수
반환값을 가집니다. 이 프로그램 자체는 10번 줄과 12번 출력하는 줄에서

시작합니다. 프로그램은 사용자에게 두 개의 숫자를 입력하라고 합니다.(12 - 14

줄) 사용자는 두 개의 숫자를 빈칸을 사이에 두고 입력을 하고 입력키를 누릅


===== PAGE 55 =====
52 ee AIF

다. main()-2- 사용자가 입력한 두 개의 숫자를 FE 하여 4000 함수에 전달합
니다.(16줄)

프로세스는 400() 함수로 LSS 합니다.2번 줄) 인수 8와 be 출력된 뒤 더해집
니다. 결과는 5번 줄에서 반환되고 프로세스는 2800으로 돌아갑니다.

13번과 14번 줄에서 cin 대상체는 변수 8와 에 해당되는 값을 입력받고, 004는
합을 출력하기 위해 쓰여집니다. 변수나 그 외 다른 부분은 며칠 후 자세히 배울
것입니다.

요와
프로그래밍 같은 복잡한 주제를 배우는데 있어서 어려움은, 여러분이 배우고자
하는 내용이 아직 배우지 않은 내용에 의존하는 경우입니다. 이번 장에서는 간단
한 C++ 프로그램의 각 부분들에 대해서 배웠고, 개발 주기와 몇몇 새로운 용어들
을 배웠습니다.

Q&A

Q #include= FAS 합니까?

A 컴파일러를 불렀을 때 실행되는 전처리계에 대해 내리는 명령의 일종입니다.
include 뒤에 오는 단어를 파일명으로 간주하여 읽어들입니다. 마치 원시 코드의 바
로 그 위치에 입력한 것처럼 말입니다.

Q // 주석문과 /* 주석문의 차이는 무엇입니까?

A // 주석은 줄 끝에서 주석이 저절로 종료됩니다. /*는 Ss 만날 때 가긴 제 주석으로
간주합니다. /* 주석 i 함수가 BUS 종료되지 않습니다. 7S 만나지 않으면 반드
시 컴파일 장애가 발생합니다.

Q 좋은 주석문과 나쁜 주석문의 차이점은 무엇입니까?

A 좋은 주석은 이 특정의 코드가 왜 이렇게 쓰였는지 말해주고 어떤 부분이 어떤 일
을 하려는지 설명합니다. 나쁜 주석은 특정 코드의 줄이 하는 일을 재서술합니다.

연구

id _으
fey (요

마나 잘 이해하였는가

를 fos as      on
큰        =
인해 보는 퀴즈들과 배운 AS Ag 볼 수 있는 연습 문제들로 구성되어



===== PAGE 56 =====
제2일 C++ 프로그램의 각 부분들 ee 53
있습니다. 부록 Do} 있는 답을 보기 전에 A 물음에 대답할 수 있도록 노력하고,
다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다.
퀴즈
ㆍ ADAYA 전처리계의 차이점은 무엇입니까?
2 왜 main) 함수는 특별합니까?
FAO 두 가지 SHE 무엇입니까? 그리고 어떻게 다릅니까?
4. 주석 안에 또 주석을 넣을 수 있습니까?
$, 주석은 한 SE 넘을 수 있습니까?

연습 문제

1. | love C++ 화면에 출력하는 프로그램을 작성합시다.
2 컴파일되어서 링크되고 실행되는 조그만 프로그램을 작성합시다.
3. 버그잡기 :
1: #include <iostream.h>
2: int main()
Se 6       i
qs   cout << Is there a bug here?";
5    return 0;
6: }
4 3번의 HIS 고친 후 컴파일하고 링크한 뒤 실행해 봅시다


===== PAGE 57 =====


===== PAGE 58 =====


===== PAGE 59 =====
56 ee MIF

프로그램은 자신이 사용하는 자료(000)들을 저장하는 방법을 가집니다. 변수와 상
수는 이 자료들을 표현하고 다루는 다양한 방법을 제공합니다. 우리가 오늘 배울
것은 다음과 같습니

변수(\014010)란 무억인가?

CHO] 변수란 정보를 저장하는 장소입니다. 변수란 여러분이 gee 저장하고
후에 그 값들을 검색하는, 컴퓨터에서의 메모리의 특정 위치입니다

컴퓨터의 메모리0260000는 조그만 방 같은 것이 나열된 곳으로 간주될 수 있습
니다. 각 방은 줄줄이 늘어서 있는 방중         z       은 메모
치는 - 준자적으로 시 매겨져| 있

address) Ch, 2  각 변수들은 여러분이 사용하는 값들

타

들어, myVariable) 메모리의 주소를 실제 모르더라도 이 YS
도록 붙여놓은 ine 꼬리표입니다. [그림 3.12 이러한 개
보

10/808016의 크기에 따라 방이 적당한 Hee 할 할당됩니다.

[그림 3.1]                                                  myVariable
메모리의 도식화        변수명

100     101      102     103     104     105     106

참고

RAM°|#t random access memory2| 약자입니다. 프로그램을       면
스크의 파일로부터 RAMLES SASF}. 모든 변수들도 660/에 PUA 프로그래머
들이 메모리를 이야ㄱ| 할 때 보통은 RAMS 말합니다.



===== PAGE 60 =====
제3일 변수와 상수 ee 57

메모리 St e+1|(Setting Aside Memory)

0++에서 변수를 정의할 때 여러분은 컴파일러에게 그 변수가 어떤 종류인지를
가르쳐 줘야 합니다. 정수형인지, 문자형인지 등등을 말입니다. 이 que 컴파일
러에게 얼마나 많은 메모리를 할당해야 하는지 그리고 그 안에 어떤 종류의 값이
들어갈 것인지를 알려줍니다.

각 방은 한 바이트 크기입니다. 변수의 종류가 두 바이트이면 두 바이트의 메모
리를(혹은 두 개의 방을) 할당해야 합니다. 변수의 종류(예를 들어 정수형)는 컴파
VAS 하여금 얼마만큼의 메모리(몇 개의 Hs 할당해야 하는지를 말해줍니다.

컴퓨터는 값들을 나타낼 때 비트와 바이트를 사용하고, 또 메모리는 바이트 단위
로 측정되므로 이 개념을 잘 이해해 친숙해져야 합니다. 이 점을 충분히 이해하
기 위해서는 부록 8의 “CH 예약어*를 숙지하기 바랍니다.

정수(|11+680)의 크기

어느 컴퓨터에서나 각 변수는 한 단위의 변하지 않는 양의 WS 차지합니다. 이
말은 정수형은 어떤 컴퓨터에서는 2바이트를, 또 다른 컴퓨터에서는 4바이트를
차지할 수 있지만 해당 컴퓨터에서는 그 크기가 항상 일정하다는 뜻입니다.
문자형 변수(00 \804806)는(문자를 저장하기 위해 사용되는데) 보통 1 바이트 크
기입니다. short 정수는 대부분의 컴퓨터에서 2 바이트의 크기이고 1008형 정수
는 보통 4 바이트이고 정수형은(0000 혹은 1008형이라는 예약어가 - 잠시 후 배움
니다 - 없는 한) 2 또는 4 바이트가 됩니다. [리스트 3.1]은 여러분의 컴퓨터에서
각 변수의 크기를 아는데 도움을 주는 프로그램입니다.

새로운 문자 Z*h(character)et |바이트의 메모리를 차지하는 하나의 글자나 숫자, 기로입
응어 니다.

[리스트 3.1] 컴퓨터에서 2 HAO) 크기를 아는 프로그램

: #include <iostream.h>

1
2:
3: int main()

4:

5: cout << "The size of an int is:\t\t" << sizeof(int) <<" bytes.\n";
6: cout << "The size of a short int is:\t" << sizeof(short) <<" bytes.\n";
7    cout << "The size of a long int is:\t" << sizeof(long) << " bytes.\n";
8    cout << "The size of a char is:\t\t" << sizeof(char) <<" bytes.\n";
9    cout << "The size of a float is:\t\t" << sizeof(float) <<" bytes.\n";


===== PAGE 61 =====
58 ee AI

10: cout << "The size of a double is:\t" << sizeof(double) << " bytes.\n";
ae

120    return 0;
135 2:
a    The size of an int is           2 bytes.
The size of a short int is       2 bytes.
The size of a long int is       4 bytes.
The size of a char is           1 bytes.
The size of a float is          4 bytes.
The size of a double is          8 bytes.

여러분의 컴퓨터에서는 각 바이트 크기가 다를 수 있습니다.

그 [리스트 3.1]은 그리 생소하진 않을 것입니다. 단지 5 - 10번 줄까지의

91260[0라는 함수가 있는데, 이것은 컴퓨터에서 제공되는 ACE sizeof) 함

수의 매개 변수로 전달되는 객체의 크기를 알아내는 함수입니다. 즉, SH 줄에서

는 예약어 int7} 9260[0의 매개 변수로 전달됐습니다. 이 함수를 쓰면 내 컴퓨터
에서는 int short 파와 똑같이 2 바이트를 사용한다는 AS 알 수 있습니다.

Signed2} Unsigned
또 하나 모든 형태의 변수들은 두 가지 특징을 가집니다. signeds} 0098000입니
다. 여기서 이 PIS 여러분이 음수를 사용할 때와 그렇지 않을 때 필요합니다.
unsigned7} 붙지 않은 정수형은 98060로 간주되는데 signed 정수형은 음수 및 양

수를 가질 수 있고 unsigned 정수형은 항상 YES 갖습니다.

ee:
es

signed 정수형이건 0098000 정수%     모두 같은 크기의 메모리를 차지하므로,
unsigned 정수형에 저장되는 숫자 중 가장 큰 숫자는 98000 정수형에 저장되는
숫자에 비해 2배가 Bch. 즉, unsigned 정수형은 0부터 65.535까지의 숫자들을

룰 수 있지만 98060 정수형에 있어서는 -32,768부터 32,767 까지 다룰 수 있습
니다. 이해가 잘 안되는 분은 부록 AS] “연산자 우선 순위”를 참고하기 바랍니다.

기본적인 변수형
여러 다른 변수형들이 0++에 내장되어 있습니다. 그들은 편의상 지금까지 이야기
해 왔던 정수형 변수00068@ variable), 부동소수점형 YA4-(floating-point variable), 문
자형 변수(0080006 1808018)로 Ud 수 있습니다.



===== PAGE 62 =====
새로운
£0

| ASCH 문자와 확장 ASCH 문자의 집합들을 갖습니다.

:
!
fu
4y
x
rr

ㅇ

ASCIl 문자 집합 ASCH 문자 집합이란 컴퓨터에서 쓰기 위해 표준화된 문자들

집합입니다. ASCIGE American Standard Code for Information Interchange2} 약자입

니다. 요즘 모든 컴퓨     SAMS 다른 많은 국제 BSE 지원하지만, ASHE
반드시 지원합니다

C++o]A] 쓰이는 변수형 들은 [표 3.1]에 나와 있습니다. 이 HE 변수형과 그 크
기(컴퓨터마다 다를 수 있습니다.) 그리고 어떤 값들이 저장되는지

저장되는 값의 크기는  노베 주 크기와 ag ae 여러분이 [리스트 3.1]을 실행
했을 때 여러분의 컴퓨

[표 3.1] HAY

unsigned short int      2 bytes      0 ~ 65.535

short int             2 bytes      =32,168 ~ 32,767

unsigned long int      4 bytes      0 ~ 4,294,967,295

long int              4 bytes      -2,147,483,648 ~ 2,147,483,647
int (16 bit)           2 bytes      =32,/68 ~ 32:767

int (32 bit)           4 bytes     -2,147,483,648 ~ 2,147,483,647
unsigned int (16 bit)    2 bytes      0 ~ 65,535

unsigned int (32 bit)    4 bytes      0 ~ 4,294,967,295

char                   1 bytes      256 문자 값들

float                4 bytes      1.2e-38 ~ 3.4e38

double               8 bytes      2.2e-308 ~ 1.86308

터에서 나온 졸력이 [리

에 그대로 Mast 수 있는



===== PAGE 63 =====
60 ee AIF

변수 정의하기

변수의 정의는 먼저 변수형을 쓰고 하나 이상의 빈칸을 입력한 뒤 Wess 쓰고
세미콜론을 입력합니다. 변 변수명은 EAS 배합해서 쓸 수 있는데 단 빈칸은 허용
이 안됩니다. x, J23qrsnf, myAge 모두다 변수가 될 수 있습니다. 좋은 변수명은
그 변수가 어디에 쓰이는지 알게 합니다. 좋은 변수명은 프로그램의 SES 알게
합니다. 다음 문장은 myAgette 정수 변수명을 기술합니다

int myAge;

일반적인 프로그램에서 12309 같은 해괴망측한 변수명은 피할 것이며 = 한 글
자로 된 변수명 (× 1 )등의 사용은 제한적으로 사용합시다. myAget} howMany
같은 의미 있는 변수명을 쓰는 것이 먼 FY 왜 이렇게 프로그램을 만들었는지

알아보기 쉽게 합니다.

한번 시험해 봅시다. 각각의 프로그램에서 몇 줄만 가지고 다음 프로그램이 무엇
을 하는 것인지 짐작해 봅시다.

보기 1 :
int 08710 (0)
{

unsigned short x;
unsigned short y;
unsigned short z;
z=x*y;
return 0;

보기 2:

int main(Q)

{
unsigned short Width;
unsigned short Length;
unsigned short Area;
Area = Width * Length;

return 0;
}
두 번째 프로그램이 이해하기 FAQ. 변수명을 길게 쳐야하는 어려움은 후일 =
로그램을 유지 보수하는데 드는 비용을 '종방허고도 남습니다



===== PAGE 64 =====
대소문자의 구별
CHo 대소문자를 구별합니다. 즉, 대문자와 소문자는 각각 다른 문
여집니다. 따라서 변수 age} Age, 또 AGEY 각 |각 다른 변수들입니다.

변수명을 어떻게 지을 것인가에는 많은 방법이 있지만, 어떤 방법을 채택하든 그

다지 큰 관계는 없고 단지 여러분의 프로그램이 변수명 Ago] 대해 일관성만 있

으면 됩니다

많은 프로그래머들이 변수명에 소문자를 쓰기를 즐겨합니다. 변수명이 두 단어를
싱                                    쓸

같이 써야 좋은 상황이면(예를 들어, my} car), my_car 또는 “sist
EVs

습니다. 후자의 명칭법을 낙타식 표기라 부르는데 중간의 대문자가 꼭 낙타의 혹

중간에 '_' 기호를 이용한 (my_car) 변수명이 읽기 쉽다고 즐기는 사람이 있고, 또
다른 이는 입력하기 어렵다고 하여 '_'기호를 안 쓰는 사람이 있습니다. 이 책에
서는 낙타식 표기를 쓰기로 합시다. 두 번째 이후에 나오는 단어는 모두 대문자

로 시작합니다. myCar, theQuickBrownFox 등입니다.

예약어((67\010)
특정 단어들은 ++에서 미리 쓰기로 예약을 해놓았기 때문에 사용자는 이들을
수명으로 쓸 수 없습니다. 이를 예약어06\000)라 하는데 컴파일러가 여러분의
제할 때 필요합니다. 예약어는 if, while, for, main 등을 포함하고 있
니다. 여러분의 컴파일러 안내서에 예약어에 대한 상세한 보기가 나올 것입니다.

ty |e ee


===== PAGE 65 =====
62 ㅇㅇ 제1주

DONT c++ 에약어를 변수명으로 사용하지 BAA.

DO 각각의 변수형이 갖는 메모리 크기를 이래하고 그 변수에 어떤 값이 저장되

DON'T unsigned 변수형에 음수를 사용하지 BIE.

하나 이상 만들 때

=

ㆍ변수형을 쓰고 변수명들을 섬표로 구분하여 여러 WS 쓰면 한꺼번에 같은 형을
~
수

가진 여러 개의 변수들을 만들 수 있습니다.

unsigned int myAge, myWeight; // 두 개의 unsigned int 변수

long area, width, length;     // 세 개의 1009 변수

보다시피 myAge2} myWeight= 각각 unsigned 정수형 변수로 선언되었습니다. 두
번째 줄의 보기는 세 개의 long 변수를  ae enon’ width, length) long
변수형은 세 개의 변수에 각각 적용됩니다. 또한, 하나의 정의문 내에서 다른 변
수형을 섞어 쓸 수 없습니다.

변수에 값 대입하는 법
대입 연산자( = )를 사용하여 변수에 값을 할당할 수 있습니다. \00에 SS 할당
하여 봅시다.

unsigned short Width;
Width = 5;

변수를 처음 정의할 때 값을 초기화할 수도 있습니다.
unsigned short Width = 5;

초기화는 대입과 똑같아 보이고 정수형 변수에서는 차이점이 WE 없어 보입니
다. 후에 상수에 대해 배울 때 특정 값들은 대입이 불가능하므로 초기화가 반드



===== PAGE 66 =====
시 이루어져야 한다는 것을 배울 것입니다. 기본적인 차이점은 초기화란 a 처음

선언시 나타난다는 것입니다.

오
요
.또
=
od

(03
me
4+y
28
Sy
꽃
미티
a2,
EN
aw,
Sot
br
에
ce,
2
요
ats)
es
4}
000
11S

// 두 개의 변수를 정의하면서 로기화
long width = 5, Length = 7;

이 보기는 1008 변수 widhS 52 초기화하고, 역시 long 변수 16080를 72 초기화
합니다. 변수 정의와 초기화를 섞어서 쓸 수도 있습니다.

int myAge = 39, yourAge, hisAge = 40;

이 보기는 세 개의 변수를 정의하였는데 첫 번째와 세 번째 변수만 초기화하였습
니타.

[리스트 3.2]는 사각형의 면적

ttlo
에

wy
덕

i

nt
rir
6
il
uy
ay
ro,
보태
그

구하고

[리스트 3.2] 변수 사응 보기

1: // 변수 사용 예

2: #include <iostream.h>

3:

4: int main()

ae

6: unsigned short int Width=5, Length; // = 개의 변수 만들, 앞의 변수만 초기화함.
7: Length = 10; // 초기화 안된 변수에 값 대입

8

9: // unsigned 510『+를 선언한 두
10: // Width] LengthS 곰한 값 대입
11: unsigned short int Area = Width * Length;

13: cout << "Width:" << Width << "\n";
14: cout << "Length: " << Length << endl;
15: cout << "Area: " << Area;

16: return 0;

Fa 해 Width: 5
결과 Length: 10

Area: 50


===== PAGE 67 =====
64 cc ANF

Ey Ay 2 SS 004 함수를 쓸 때 필요한 라이브러리를 포함하기 위한 40006 문
뜨 |

입니다.
6번 줄에서 Widtht= unsigned short 정수형으로 정의되었고 5로 초기화되었습니다.
unsigned short 정수형 Lengh= 정의되었지모      는

Ｌ6080에 10이 대입되었습니다.

1181 줄에서 unsigned short 정수형 Area7} 정의되면서 Width} LengthS 곱한 값
으로 Arad 초기화하였습니다. 13번 줄부터 15번 줄까지 변수값들이 화면에 |S
력됩니다. nde 새로운 SS 만듭니다.

typedef
unsigned short int 쓴다는 것은 그야말로 떠분하고, 반복적이며, 그럼에도 불구
하고 중요하면서 또한 잘못 입력하기 쉽습니다. 0++에서는 예약    lef(t
definition?) 약자)를 써서 이러한

때 이를 새로운 형 만드는(일째 배움) 방법과 구분
요합니다. 6060하는  bee 다음에 현재 C++ A] 존재하는
변수

typedef unsigned ‘sho  rt
나라

이는 USHORTZH= 새로운 BAS 만들었는

short int 대신 USHORTS 써서 정의를 할

3.2]를 USHORTE 써서 다시 입력한 것입니

데 여러분은 이렇게 6 unsigned
있습니다. [리스트 33) [리스트

[리스트 3.3] typedef 예제

// RREKKKKKKKKKEEKEEE
// typedef 예약어 사용법
#include <iostream.h>

typedef unsigned short int USHORT // typedef 정으

int main®

{
USHORT Width = 5;
USHORT Length;
Length = 10;

PH Se ACOANauUuUrFWDr =

= Ou



===== PAGE 68 =====
제3일 변수와 상수 ee 65

12:   USHORT Area = Width * Length;

13:   cout << "Width:" << Width << "\n";
14:   cout << "Length: " << Length << endl;
15:   cout << "Area: " << Area;

16:    return 0;

결과  Width: 5

Length: 10
Area: 50

분석  5번 2] USHORT®= unsigned short int= typedef= 써서 별칭을 만든
~ 니다. [리스트 3219} 그 외 모든 것은 동일합니다.

>브
ro

언제 shot 쓰고 언제 longS MET 1
도아

CHS 처음 시작하는 프로그래머에게                           고
것인가 하는 점입니다. 사   an 하면 누워 떡먹기입니

언제 1008형을                      실
값은 큰 변수에 넣는다는 것입니다.

쓸 3
다. 기본원리는 큰

Ni

[표 3.1]에서 보았듯이 0098000 short 정수는, 가령 2 바이트라 하면, 65.535까지의

Re 가질 수 있습니다. 98060 short 정수는 그 값의 반값만 가질 수 있습니다.(대
신 음수 WS 갖습니다.) unsigned lng 정수는 엄청 큰 FS 표현할 수 있는데

(4,294,967,295) 사실 이 정도면 무한대 값이라 생각해도 좋습니다.
야 하면 008형이나 00006형을 사용해야 하는데 대신 정확도가 조
있습니다. 800[형과 000016형은 매우 큰 수를 다루지만 대부분 처음 7
까지가 의미가 있습니다. 그 말은 그 AES               될

미입니다.

= we >
32 2 오 때
nl,
a
Sl

unsigned 성수형에서의 올림 초기화

unsigned long 정수형이 감당할 수 없을 정도의 큰 수를 갖는 APE 흔치 않은
경우지만, 그럼에도 불구하고 그러한 일이 일어나면 어떻게 될까요?

unsigned 정수형이 가질 수 있는
하고 처음부  두터 다시 시작ㅎ 빠 것


===== PAGE 69 =====
66 ㅇㅇ AI

[리스트 3.4] unsigned PAYO 감당할 수 없는 2S 다룰 때

1: #include <iostream.h>

2: int main()

Se <

ee    unsigned short int smallNumber;

Ds    smal lNumber = 65535;

63    cout << "small number:" << smallNumber << endl;
tT:    smal lLNumbert+;

8:    cout << "small number:" << smallNumber << endl;
9:    smal LNumber++;

10:   cout << "small number:" << smal lNumber << endl;
11:   return 0;

(425 +

결과  small number: 65535

small number: 0
small number: 1
분석  4번 ©] smallNumbert= unsigned short inte 선언되었는데 저자의 컴퓨터에
서는 2바이트 짜리 변수이고 0부터 65535까지의 값을 가질 수 있습니다. 5
번 So 그 최대값을 대입하였고 of 줄에서 출력합니다.
Ta 줄에서 그 BS 하나 증가하였습니다,(즉, 1을 더함) WS 하나 증가하는 기호
는 ++입니다(마치 (에서 하나 진화된 이름이 (++인 것처럼) 따라서 smallNumber
의 값은 65.536이고 unsigned small 정수형에서는 65,535 이상의 값은 감당할 수가
없기 때문에 올림 초기화가 되어 0이 되고 BA SoA, 출력되었습니다.

9번 줄에서 다시 하나 값이 증가되었고 새로운 값 leo] 출력되었습니다.

signed 성수에서의 올림 초기화

signed 정수형에서는 unsigned 정수형의 경우와 다른데 왜냐하면 그 값의 반은 음
수 값이기 때문입니다. 자동차의 주행거리 측정기 대신에 여러분은 가장 큰 양수
끝에 도달하면 이번에는 절대값이 가장 큰 음수 값으로 넘어가는 측정계를 생각
히                                                    증가하

하면 됩니다. 즉, 가장 큰 양수의 정수에 도착하였을 때 거기에서 하나 더
절대값이 가장 큰 음수 값으로 되고 거기에서 0을

입니다. [리스트 3.5|에서 가장 큰 양수에 1이 증가하면 어떤 결과가 나오는지
보여줄 것입니다.

> |묘
oO



===== PAGE 70 =====
제3일 변수와 상수 ㅇㅇ 67

[리스트 3.5] singed 정수형의 SCHZtol 1이 중가될 때

#include <iostream.h>

int main()

<
short int smal lNumber;
smal lNumber = 32767;
cout << "small number:" << smal lNumber << endl;
smal lNumbert+;
cout << "small number:" << smallNumber << endl;
smal lNumbert+;
cout << "small number:" << smallNumber << endl;
return 0;

CON DU FWD |=

~ ak AO
- O88

125 +

24 small number: 32767

small number: -32768
small number: -32767

분석 4번 줄 90081404000@는 이번에는 98060 short 정수형(명시적으로 unsigned}
=, =!       _

Ads 않으면 90000로 자동 선언됩)으로 하였습니다. 프로그럼은 앞선
Wiad 같은 작엽을 하지만 결과는 다릅니다. 이 결과를 충분히 이하하면 두
바이트 정수형에서 어떤 과정으로 정수형 숫자들이 비트 단위로 움직이는지 이래

하게 될 것입니다. 자세히 알고 싶으면 부록 CS 참조하기 바랍니다.
크

양수 KIA 가장 큰 음수 값으로 넘어가는 과정을 보여줍니다.

t= AlK(Character)

문자형 변수는 일반적으로 1 바이트이므로 256 개의 BSS 가질 수 있습니다.(부
록 C 참조) 문자형은 0에서 255까지의 small 숫자로 해석될 수도 있고 4901
문자형으로 AAS 수도 있습니다. ㅅ901 문자 집합과 그에 대응하는
150(10[600800081 Standards (27880128000)에서 설정한 값은, ASCII 문자 집합이 모든

문자들, 숫자들, 구두점 등으로 번역, 대응될 수 있도록 하였습니다.


===== PAGE 71 =====
68 ㅇㅇ AS

아니면 0으론 인식을 합니다. 이 '0'과 '|'들의 한 멍어리의
|                    쿼

[고, 다시 그 Stee OS

1”,

38
rir
>» fH
건
wn
Hu
re
고
 '
ai

ASCH SEA ‘VW 972 할당되어 있습니다. 모든 대, 소문자, 0부터 9까지의
숫자, 그 외 구두점들은 1부터 128 사이에 BSS 할당받았습니다. 남아있는 128
개의 기호들은 컴퓨터 업자들의 특정 목적을 위해 남겨두었는데, 사실 184의 확

장문자 집합이 어느 정도 표준으로 되어 있습니다.

문자와 숫자
예를 들어 "라는 글자를 특정 문자변수에 GIS 하면 실제는 0부터 255 사이의
값이 할당이 됩니다. 컴파일러는 이 문자들과 SLES 둘러싸인 문자, 숫자,
두점 등등) 컴퓨터의 숫자 값들을 써로 번역

해 줄 수 있습니다.

이 EA 사이의 관계는 임의적입니다. 가 값 97에 대응되는 특별한 이유는
없습니다. 단지 모든 주변기기(키보드, 컴파일러, 화면)들과 사람들이 그것을 인정
해주면 됩니다. 컴퓨터가 저장하는 Gt 5와 우리가 인식하는 문자 "에는 커다란

커
차이가 있습니다. "라는 문자는 컴퓨터가 저장할 때 53으로 저장하는데 이는 '
라는 같을 컴퓨터가 저장할 때 9로 저장하는 것과 마찬가지 이유입니다.

2

[리스트 3.6] 컴퓨터가 저장하는 값에 의거하여 문자들을 출력하여 보기

1: #include <iostream.h>

2: int main(

a: ft

4s    for Gint 1 = 32) i<128> Tt)
D     cout << (char) i;

6     return 0;

ve oD

결과 !10#$%6!()*+./0123456789; ;<>?@ABCDEFGHIJKLMNOP
QRSTUVWXYZE\I*' abcdefghi jklmnopqrstuvwxyz<|>~

분석  이 간단한 프로그램은 32부터 127까지의 RSS 출력합니다.



===== PAGE 72 =====
제3일 변수와 상수 ee 69

특수 줄력 ZAl(Printable Character)

CH 컴파일러는 특정 문자들을 규격 조정용 문자들로 이해합니다. [표 3.2]는 가
흔한 경우를 보여줍니다. 여러분은 역사선(이를 이스케이프 문자라 함)뒤에 이
ES 입력함으로써 WIS 할 수 있습니다. 따라서 탭문자를 여러분의 코드에
}입하기 위해 홀따옴표를 입력한 뒤 역사선을 입력하고 [문자를 입력하고 =a}
표로 막습니다.

om
Flot
ro

= Hl

qo

char tabCharacter = '\t';

이 예는 tabCharacter 변수를 선언하고 \로 초기화하는데 이는 탭으로 인식이 ¥
니다. 특정 문자들은 화면에 출력하거나, 파일 또는 특정 출력장치에 출력할 경우
쓰입니다.

[표 3.2] 이스케이프 문자

문자                                 의미

\n                                  개행 문자

남                                   r=

\b                                   백스페이스

‘                                   쌍따옴표

나                                   훌따옴표

\?                                   의문부호

                                   역사선 그 자체

새로운 이스케이프 문자 이스케이프 문자는 다음에 LE 문자의 의미를 바꿈니다. ye 들어,
SO (은 문자 /을 의미하지만 이스케이프 문자(\>에 의해 개행 문자로 의미가 바낌니다.

상수(3009[301)
변수와 마찬가지로 상수들도 컴퓨터 안에서의 자료저장 장소를 말합니다. 단 변
수와 달리, 그 이름이 말하고 있듯이 상수란 변하지 않는 값을 가집니다. 상수는
만들어질 때 그 값을 초기화해야 하며 그 후 새로운 값을 할당할 수 없습니다.


===== PAGE 73 =====
70 ee MIF

문자 4¥(literal constant)
0++는 두 가지 형태의 상수를 갖습니다. 문자 상수와 기호 상수입니다.
문자 상수는 여러분의 프로그램에서 필요한 곳에 입력을 하는 값입니다. 예를 보면,
int myAge = 39;

myAget= 정수형 변수이고 “39”는 문자 상수입니다. 여러분은 이 39에다 다른 a
을 할당할 수 없고 이 39라는 값은 변할 수 없습니다.

기호 상수(600060116 constant)

기호 ASE 특정 이름에 의해 표현되는 상수입니다. 변수와 달리 Are 초기화
된 후 값이 변하지 않습니다.
여러분의 프로                             또 이85568라는 전체 학급

그램에서 9400끄라는 정수형 변수를 갖고
를 의미하는 변수를 가졌을 때 여러분은 전 학생 +S 구하는 프로그램을 짤
수가 있습니다. clases} 학생수가 SAY 떠 총 학생 FE

student = classes * 15

입니다.

% 표시는 곱셈을 의미합니다.

자 상수입니다. 여러분의 프로

문                   그램어
고, 유지 보수가 쉬워질 수 있습니다.

student = classes * studentsPerClass

여기서 15는             에서 이 값을 기호 상수로 바꾸
| 놓으면 읽

으면

호날 여러분이 각 학급당 학생 +S 바꿀 필요가 있을 때 프로그램 안에 15로 표
시된 학급당 학생 SS 일일이 찾아 바꿀 필요 없이 studentPerClasse}= 기호 상
수 값만 바꾸면 됩니다.

@++에서 기호 AES 정의하는 2가지 방법이 있습니다. 가장 오
며 이제는 잘 안 쓰는 방식이 전처리계 명령어 #$06006를 쓰는 것

#defineS 가지고 상수를 정의하는 법
전통적인 방법으로 상수를 정의하려맨



===== PAGE 74 =====
#define studentPerClass 15

라 하면 됩니다. 주목할 AS studentPerClas= HAY - 정수형, 문자형이 아니라

는 것입니다. #00806는 단순 텍스트 치환만을 합니다. 전처리계는 studentPerClass
는 단어만 만나면 그것을 15로 바꼽니다.

컴파일러가 실행되기 전에 전처리계가 BE studentPerClas= 15로 바꾸기 때문에

컴파일러는 90406006004858라는 단어를 못 만납니다.

const= 상수 만들기
#defines? 쓰는 방법도 있지만 (++에서는 더 좋은 방법으로 상수를 정의하는 방

법이 있습니다.

const unsigned short int studentPerClass = 15;
이것은  studentPerClasse}= 기호 상수를 선언하는 방법인
8040600068"(1886는 unsigned short 1끄로 정의되어 있

로그램을 읽기 쉽게 하고 유지 보수를 쉽게 하며
터태 가장 큰 차이점은 으 이러한 상수 AAS 는 oe

상수는 프로그램이 실행되는 동안 변할 수 없습니다. studentPerClass®| 같을 바꾸고
싶으면 BES 재수정한 뒤 컴파일을 다시 하여 실행시켜야 합니다.

DON'T ite 따를 27] PIS 크기를 명확히 하기 위해 Chort (ongS 명확히 밝힙시다.

po     erect 크기를 넘는 변수를 잘 관찰하고 올림 호기화를 주의합시다.

[=]           Le      dD
00 변수에 그 의미를 부여할 수 있는 이름을 사용합시다

DONT 예약어를 변수명으로 하지 Bet,

값들의 집합으로 제한된 변수명들을 만들

공합니다. 예를 들어, 여러분은 COLORS 나열형으로 선언할 수 있고 이 COLOR



===== PAGE 75 =====
72 ee 제1주

에는 RED, BLUE, GREEN, WHITE, BLACKe}= 5개 값을 가질 수 있게 할 수 있
Bs
습니다.

상수 YAP] FES 예약어 ems 쓰고 형 YAS 지정한 뒤 중괄호를 열고
각각의 정확한 RSS ALE 이용해 나열하고 마지막에 중괄호로 막은 뒤 세미
콜론을 쓰면 됩니

Ces 100 { RED , BLUE, GREEN, WHITE, BLACK };

이 수행문은 두 가지 일을 합니다.
1. COLORS 나열형 명으로 정하는데 이는 새로운 형입니다.
2 중괄호 안의 각각의 값들을 기호 상수로 정의하는데 REDE 0; '6Ｌ나는 1, GREEN2
2

enum Color { RED=100, BLUE, GREEN=500, WHITE, BLACK=700 3;

에서 REDE 100이라는 값을 갖고 BLUEE 101 갖습니다. GREENS 500이고
WHITE 501, BLACK2- 700이라는 값을 갖습니다.

여러분은 COLORYS 변수들을 정의할 수 있지만 각각의 상수 나열형에 단 하나
의 값만을 할당할 수 Wer] 예의 경우 RED, BLUE, GREEN, WHITE,
BLACK®- 100, 101, 500, 501, 700을 가짐) 여러분은 어떤 값도 COLOR 변수에 입
력할 수 있으며 사실 꼭 색깔이 아니어도 정수형이면 입력이 가능합니다. 나열형
변수들은 unsigned 정수형  이며, 나열형 상수들은 각각에 대응하는 정수값들을 가
집니다. 이 방법들은 색깔들이나 날짜, 주, FS 집합들을 가지고 작업할 때

매우 편리합니다.

we:

[리스트 3.7] 상수 나열형의 보기

#include <iostream.h>
int main()
{
enum Days { Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday };

Days DayOff;
int x;

Nour WDM —



===== PAGE 76 =====
9s    cout << "What day would you Like off (0-6)? ";
10?   610 22 XK:

11, DayOff = days xe Alb

125

13   if (DayOff == Sunday || DayOff == Saturday)

14:      cout << "\nYou're already off on weekends! \n";
15   else

16:      cout << "\nOkay, I'll put in the vacation day.\n";
10   return 0;

1S: >

겔과 What day would you Like off (0-6) ? 1

Okay, I'LL put in the vacation day.
What day would you Like off (0-6) ? 0

You're already off on weekends!

"  4번 줄에서 상수 나열형 Days7} 정의되었고, 그 안에는 0부터 시작하는 7개

의 값들이 포함되어 있습니다. OH 줄에서 사용자는 요일을 선택할 수 있
고, 선택 Ke 0부터 6 사이의 값입니다. 입력값은 13번 줄에서 Sunday?! Z|
580408》인지가 비교되고 적절한 행동이 취해집니다. if LIS 4일째 수업에서 다
루어질 것입니다.

“Saturday"@h= 값을 프롬프트에서 입력할 수 없습니다. 프로그램은 Yaa 단어
를 나열형 값으로 해석하지 못합니다.

이 책의 모든 프로그램에서 저자는 여러분이 잘못된 자료를 입력하였을 때 어떠한 일
이 발생할 것인지는 고려하지 않았습니다. 예를 들어, 이 프로그램에서는 여러분이 0부
터 6까지의 숫자를 입력하는지 아닌지를 검사하는 과정을 넣거나 하는 등의 과정은 취
하지 않았습니다. 단지 프로그램을 오늘 학습의 목적에 맞도록 그저 7  간단하고 쉽게 만

드는메에만 AGS 썼습니다.

(Fag
it

이번 장에서는 숫자형과 문자형 변수들 및 상수들을 알아보았는데 0*++에서는 =
로그램을 수행시킬 때 자료들을 저장하기 위해 쓰입니다. 숫자형 변수들은 정수


===== PAGE 77 =====
74

co ANA

(char, short, long int)o] 있고 부동소수점형00806 double)o] 있습니다. 숫자형은
signed] 7]} unsigned JUG. 모든 Be 컴퓨터마다 다른 크기를 가질 수 있지만
하나의 컴퓨터에서는 하나의 값만을 갖습니다.

a . 용량보다 큰 = abe  : 할당하면 올림 초기화
나타납니다.

이 장에서는 문자 상수와 기호 상수도 알아보았고 상수 나열형도 알아보았습니
다. 또 상수정의의 두 가지 방법, AdefineS 쓰는 법과 예약어 0008를 쓰는 법도
보았습니다.

we

Q&A

Q 만약, short 1마에서 용량이 모자라 올림 초기화가 일어난다면 왜 항상 long 정수형을
쓰지 않습니까?

A short 정수형 및 lng 정수형 모두 Leto] 부족해 올림 초기화 현상이 일어날 수 있
습니다. unsigned short 정수형에서는 65,535 이상의 수는 올림이 일어나는데 반해
unsigned long 정수형에서는 4.294,967.295에서 올림이 일어납니다. 그런데 대부분의
컴퓨터에서 long 정수형은 shot 정수형에 비해 두 배의 메모리를 잡아먹습니다.(예
를 들어 4바이트 대 2바이트) 그리고 이러한 변수가 100개 ate 그 컴퓨터에
서는 200바이트의 RAMS 소비하게 되는 것입니다. 그런데 요즘 와서는 사실 이 문

= 큰 문제가 아닙니다. URE PCE 수천, 수백만 se] = 9} 메모리를 갖기 때

문입니다.

Q 정수형 변수에 소수점을 할당하면 어떤 결과가 발생합니까? 예

int aNumber = 5.4;

a

A 좋은 컴파일러는 경고를 내보내고, 실제 할당은 소수점 부분은 절삭됩니다. 548
수형 변수에 입력하면 그 변수에는 5가 저장됩니다. 정보는 상실되고, 그 정수형
수를 다시 008 변수에 입력해도 값은 그냥 5가 됩니다.
Q 문자 상수를 왜 쓰지 말아야 합니까? OH 까다로운 기호 상수를 써야 합니까?
A AAS] 프로그램에 거쳐 여러분이 하나의 특정 상수를 쓸 때, 기
형

6
oF
+}
1
x,
ni
4 fi
ay
32
ny 미
zi
우
i

부호형 상수의 값만 바꿈으로써 전체 프로그램     를
기호 상수는 자기가 자신을 설명하기가 tes 예를 들어, 프로그램에서 갑자기
것은 때때로 이해하기가 어렵습니다. 그러나 0681660.&61006 같은 기

호 상수를 곱하면 이해하기가 쉬울 aga.



===== PAGE 78 =====
Q unsigned 변수에 음수를 대입하면 어떻게 됩니까?

unsigned int aPositiveNumber = -1;
컴파일러는 경고를 내보내주고 AMS 하긴 합니다. 음수는 비트 형태로 연산
다. 그리고 unsigned 정수로 환원됩니다. 따라서 -1은 그 비트 연산이 1111
11111111(16진수로 OxFF)9]¢]] 이는 unsigned Zt 65,535로 해석됩니다. 이해가 안되면
부록 (를 잘 읽어보기 바랍니다.

Q 비트 패턴이나 이진연산, 16진수 SS 모르면서도 C+

>
rit, oft

Te flo

들이 제공하지 못하는 막강한 힘을    aaah 이 노구으 Nez age 0++이 A
퓨터 내부에서 어떻게 돌아가는지를 잘 알아야 합니다 이진연산에 대해 잘 모르면
프로그램 결과에 혼란이 올 때가 많습니다.

3 기호 STS 쓰는 이점은 무엇입니까?
4 const 예약어를 쓰는 것은 #defineS 쓰는 것에 비해 무엇이 좋습니까?
§. 좋은 변수명과 나쁜 변수명의 차이점은 ics ii
6. 아래와 같은 나열형이 FOURS 때 BLUE

enum COLOR { WHITE, BLACK = 100, RED, BLUE, GREEN = 300 };

7 아래에서 어떤 변수명이 좋은 것이고 어떤 변수명이 나쁜 것입니까? 그리고 어떤 변수명

이 규칙에 어긋나는지 찾아보십시오


===== PAGE 79 =====
76 ㅇㅇ AIF

a. Age

bs tex  x

c. R79J

d. TotalIncom
e. Invalid Y

p= |
연습 문제
 다음의 정보를 저장하려면 어떤 변수형이 적당합니까?
. 여러분의 나이
뒤뜰의 면적
. 은하의 Bo} 개수
. 2월의 평균 강우량

aasg :
ㆍ

므
nun
KI
2
N
2
Ho
aoe
=
pel
rin

상수로 초기화하여 봅시다.



===== PAGE 80 =====


===== PAGE 81 =====
78 ee 제1주

서문
프로그램은 차례로 수행되는 명령들의 집합입니다. 프로그램에서의 생명은 특정
ㅣ 참이냐 거짓이나에 따라서, 하나 혹은 다른 명령어 집합을 실행하는 능
터 나타납니다. 오늘 우리는 다음을 배울 것입니다.

ay
rlo

jo WN IH
Oo
ob

HU 고
ro
ow
<=
rt
4o
노오
FE
pa
5

+>
J
ro
Ee:
qu
7

Beees«
번   mn
ers   ku
=   ro
=   ES
aga

4a
i   2
4   (es
mm |
of   =
더
그
주
요
~]
re}
=
OF
=

mt
_—
cu
4a
뉴원
=
kJ
B.A
이모
크
offl
aa)
안
rir

sk
5

문장(5【3[6106001)

(++에서 문장($6160000은 연속적인 실행(06406006 of 8%600000)을 제어(20000!)하
고 수식(860005900)을 평가(8\010000)하거나 혹은 아무 것도 하지 않습니다.(이를
널 문장이라 함) 모든 CH 문장은 세미콜론으로 끝나는데 세미콜론 그 자체로
표현되는 널 BAS 아무 것도 하지 않습니다. 가장 일반적인 문장의 하나는 다
음과 같은 Ug (Assignment) 문장입니다.

수학에서의 표현과 달리 이 BAO x 가 8 + 『와 같다는 의미가 아닙니다. 이 문

장은 다음과 같이 읽힙니다 “ad bo] 합의 RS xo) 대입한다.” 혹은 “×에 8 + 6
은 2가지 일을 하지만 하나의 문장이고 그래서 하나의 세

미콜론을 갖고 있습니다. 대입 연산자는 오른쪽에 있는 AS 왼쪽에 대입합니다.

2
새로운      장 널 문장은 아무 것도 하지 않는 문장입니다.

공백 FAKWhitespace)

공백 문자(탭, 빈칸, 개행 문자)는 문장에서 무시됩니다. 위의 대입 문장은 다음과
같이 쓰여질 수 있습니다.

x=atb;

× =a



===== PAGE 82 =====
장 ee 79
여러

o

}는데 그렇지 않

Ke}

>

아 ap     이!             au
10     IH           Ie oD
te     a           my
ag     8           이" 22 =                  a                   ei
O                    그
주    ia          20 때 =                                     -
a              Je Hh pty                                습   ry
ae    o      =a 4 mw                                     a9  ay
>    고       Soo . 깨                    i                sa ®
5    ck      은 모으                  그             0
eo     =        o 과 ra, iy                     WE     ‘           a KO ON
앤    오       이 이 4 To                   고   ir          ey, ne
+     ir        “A io x                      마    é              aoe    <i
(0    ae          OW ㅇ                    te    ipl          ov 마   rai)
     4     UerZ                      -           eS OT       <b st
a          ‘Dp                      ee    al                 :    ㅇ
오 4 8 우표 별                 오운         모비 두 ee
pd    mu °°     은 or 14 이 +                ip 브 매         fie Hoon   Ald Ke
=. om        oF oe                  fw           to @ BM
roy ow     Oo wo = wy                  oy &          To =   nj a
머 고      De        oO 4)         ie                           Bs Ol  oR                om 매   ie   때 븐 90
| fon Be 신   호 보호보회          ~ 2 =      ay xr 부 “ia
wo  7 Fo     a <= ny  .                   Ul 메 ape           RT db  Hw . 0 im
Ww me wo     Oo +   S                   ue =           세 우애 7 7 7
hy oat 5    Bop eH                 © ie      ~ te =
_ WP oe    매 ae or                i oll Alt      evr ®
ry     gl <          ah   68                  al qu =       ^       oF
= 때 =e  가 op te ss 2     me oy    Qan =
eee meses ss     oa   Hake 은
보증    i    we oy mr 80    a 의 로         < oh ‘|       Mo I} fo  bn     2
ey HE    러    qn aly      eu                     oro »     =
RI 50  Ao i     ok  주 ro    ny    5 8                         4  2 00  <      -
=        빠 i <b a                     gases    대
of} Ss                     my             A            g  4  fe)          —      th   이!        =
He =                             =      Hh 2. 로 oe
=                                                           Sy 4 0800
4



===== PAGE 83 =====
80

ee 제주

PI7} 3.14, SecondPerMinute7} 60이라고 가정하면 위의 세 개는 모두 수식문입니다.
다음의 복합 수식문
x=athb;

8와 bE 더해서 결과를 xo 대입하고 그 대입값을 반환합니다. 따라서 이 문
시 수식문입니다. 또 수식문이기 때문에 대입 연산자의 오른쪽에 위치할

와 bo] 값을 머한다
와 6의 연산 결과를 xo] 대입한다.
대입 연산 x = a + bol Babe >에 대입한다.

a, 0, x, ye 모두 정수이고, 8가 2이고, 6가 5일 Wx, 》는 모두 7입니다.

[리스트 4.1] 복합 수식 계산하기

1: #include <iostream.h>

2: int main()

38 '

4:    int a=0, b=0, x=0, y=35;

5    cout << "ar" << a <orgubs |" <S by

6     COUt KS UKE KKK See el! KK 9 KS 61000
7

8

a=9;
:    b=7;
oO:    y = X = atb;
10%    cout << “a: " << 3" bal << by
11    cout << " KE " K< < 때보 << % << endl;
12   return 0;
132 3

결과  ay 0 bi 0 Ks O ys 35

az 9b: 7 x: 16 ys 16

불샐 fe 주이서 4개의 변수가 선언되고 이 5, 6번 줄에서 출력
~ 、 되고 7번 SOA ae 9를 할당받습니다. 8번 줄에서 6는 7을 할당받습니다.
9번 줄에서 ash BE 함해져서 결과가 vol 대입됩니다. 이 수식 6 = a + HSA

줄
산되어져 결과가 다시 에 대입됩니다.



===== PAGE 84 =====
연산자(00하하아)

연산자란 컴파일러로 하여금 행동을 Asa 만드는 기호입니다. 연산자는 연산체
(008000)에 작용을 가하는데 0++에서 모든 연산체는 수식입니다. 0++에서 연산
자는 몇 가지 범주로 구분됩니다. 연산자 WHE 다음 두 가지가 있습니다.

를 대입 연산자

를 수학 연산자

대입 연산사(359191171011【 operator)

대입 연산자 OE 대입 연산자 윈쪽의 연산체가 대입 연산자 오른쪽의 값
도록 합니다.

X=atb;

thlo

a

는 8와 의 FS 연산체 xo] 대입합니다.

왼쪽의 연산체를 왼쪽 값0-0106 : left \000)이라 하고 오른쪽 연산체를 오른쪽
ék(t-value : right \8106)이라 합니다.

상수들은 오른쪽 값입니다. 상수들은 왼쪽 값이 될 수 없습니다. 따라서

× = 35; // 맞습니다.

는 틀립니다
새로운 왼쪽 Ae 수식의 왼쪽에 있을 수 있는 연산체입니다. 오른쪽 값은 수식의 오른쪽에
SO 있을 수 있는 연산체입니다. 모든 값들은 오른쪽 값이 될 수 있지만 모든 오른쪽 값
은 왼쪽 값이 될 수는 없습니다. 왼쪽 값이 될 수 없는 오른쪽 ye 문자들입니다
따라서 여러분은 x = 5라고 SFE 있지만 5 = *라고 쓸 수는 없습니다

수학 04 AFAH(mathematical operator)

5가지의 수학 연산자가 있습니다. SUH, WO, FAO, 나늦셈0), 나머지 연산자(4)
입니다.


===== PAGE 85 =====
82 ee 제1주

덧셈과 wae 보통 수학에서처럼 계산되는데, 만약 결과는 음
unsigned 정수형인 경우 기대하지 않았던 값들이 나타납니다. 어제 보았듯이
오버플로우(606010\)가 발생합니다. [리스트 4.2]는 작은 수에서 큰 수를 빼는
러한 예를 보여줍니다.

4y
rc lo
=
ch
re 그
이

[리스트 4.2] Salo] 의한 정수 오버플로우의 발생 예
빼서

1: // CHAE 4.21 - Belo 의한 정수 오버플로우의 발생 예
2: df

3: #include <iostream.h>

4:

5: int main()

62

(3    unsigned int difference;

os    unsigned int bigNumber = 100;

93    unsigned int smallNumber = 50;

102   difference = bigNumber - smallNumber;

We   cout << "Difference is: " << difference;

122   difference = smallNumber - bigNumber;

13:   cout << "\nNow difference is: " << difference <<endl;
14:   return 0;

15: 3

결과  Difference is: 50
:     Now difference is: 4294967246

aa 연산자는 10번 줄에서 불려 집니다. 결과는 11번 줄에서 우리가 기대
한 대로 나타납니다. 12번 줄에서 다시 Bao] 일어나는데, 이번에는 조그
만 수에서 큰 수를 Mc 결과는 음수여야 하는데 변수가 0098000이므로, 오버
플로우가 발생합니다. 부록 에서 더 자세히 다룹니다.

(ag
dz

정수 Lie ela} 나머지 연산
정수의 나늦셈은 일반적인 나늦셈과는 다릅니다. 21을 4로 나누면 결과는 분수가

가질 수 없습니다. 따라서 나머지는 잘려 ree 답

머지를 구하기 위해서는 여러분은 나머지 연산자(%)를

결과는 1 입니다.

용할 수가 있습니다. 예

때 10으로 나머지 연

anu

들어, 매번 10번째 연산 때마
취한 뒤 결과가 0일 때 출력

re
illo



===== PAGE 86 =====
을 하면(즉, 10으로 나눈 나머지가 0일 때 출력을 하면) 원하는 결과를 얻을 수
있는 것입니다. 1 % 10은 1이고, 2 % 10은 2이고 10 % 10은   절과가 0인데, 이런
계산을 계속하면 20 % 10일 때 결과가 0이 됩니다. 이런 기법을 우리는 순환문을
배우는 7일째에서 써보게 될 것입니다.

ee ae eee
많은 초보 (++ 프로그래머들이 문장에서 세미콜론을 잘못 입력합니다.

if (someValue < 10) ;

someValue = 10 ;

여기서 하려고 했던 WE someValue™t 10보다 AL someValues 10으로 설정하는
것입니다. 위 BES 컴파일하여 실행하여보면 someValue= 항상 10°] 된다는 것을 알
수 있습니다. 왜냐하면 it 문장이 세미콜론에서(아무 일도 안하는 연산자) 끝나기 때문

Bett,
띄어쓰기는 컴파일러에게는 아무런 소용이 없습니다, 위의 조그만 예제는 다음과 같이
막시 을 수 ear,
if ( someValue < 10 )      // 비교해봄
;               // 이부 동작 eter
someValue = 10 ;         // 10을 대입
it 문장 끝의 세미콜론을 없애면 원하는 대로 동작될 것입니다.

대입 21AtLKAssignment Operator) 2}
수화 2JAITHMathematical Operator)°] =

변수에 값을 더하는 것은 아주 혼한 연산이고, 그 값을 다시 그 변수에 되돌려
더하는 것 또한 흔한 연산입니다. myAge 변수가 있고 그 WEBS 2를 증가시키
려면 다음과 같이 할 수 있습니다

int myAge = 5;

int temp;

temp = myAge +2; // 5 + 28 하여 temp 대입
myAge = temp ;    // temp 값을 다시 myAge™ 대입

이 프로그램은 한바퀴 꼬여 있고 소모적입니다. 0++에서는 대입 연산자 양쪽에
wee 같이 쓸 수 있습니다. 따라서


===== PAGE 87 =====
84 ee 제1주

myAge = myAge + 2;
가 가능하고 또 Bal USUeh. 수학에서는 이 수식은 의미가 없지만 0++에서는
}

가능합니다. 좀더 쉽게 쓸 47

myAge += 2 ;

자기대입 덧셈 연산자+=)는 오른쪽 값을 왼쪽 값에 더한 뒤 그 결과를 다시 a
쪽 sol 대입합니다. 이 연산자는 '플러스-이콜"이라 읽습니다. 따라서 문장은
“myAge Se]2--o] Ae 2”라고 읽으며 만약 myAge7} 4라면 연산 후 결과는 6이
됩니다.

비슷한 자기 대입 연산자는 빼기(=), 나누기/=),곱셈(*=), 나머지 연산(%=)에도
적용됩니다.

증가 엽산자와 감소 연산자
(Increment operator and Decrement operator)

덧셈후 자기자신의 변수에 다시 대입하는 연산 중 가장 흔
것입니다. 0++에서는 이 연산만을 위한 특별한 연산자가 있습니다.

증가 연산자0+)는 변수의 값을
니다. 0라는 변수가 있고 1을 증가하려면

ott // 6로부터 시작하여 1을 BE

라고 쓰는데 이는

과도 동일합니다.

전치 연산자와 후지 연산사(마애× |배배려 and Postfix operator)
증가 연산자(++)와 감소 연산자(-) 모                  있습니다. 전치와
후치의 문제입니다. AAS 변수명 앞에 베이크   치는 뒤에 쓰입
Ch(myAget+) 단순한 문장에서는 어떤 것을 쓰더라도 문제가 안되지만 복합문에



===== PAGE 88 =====
서는 사정이 다릅니다. 증가 연산(또는 감소 연산)을 하고 그 결과를 다른 변수에
저장하면, 그 결과는 상당히 달라집니다. 전치 연산자는 대입이 일어나기 전 연산
되고, 후치 연산자는 대입 연산자가 실행된 후 연산이 일어납니다. [리스트 4.31에

서 볼 수 있습니다.

[리스트 4.3] 전치 및 후치 엽산자

1: // [리스트 4.3

a 11 전지 및 후지 연산자의 중가 및 감소

53

4: #include <iostream.h>

5: int main()

62

7:    int myAge = 39; // = 정수형 AH+S 초기화 함.

8:    int yourAge = 39;

9:    cout << "I am:\t" << myAge << "\tyears old.\n";

10:   cout << "You are:\t" << yourAge << "\tyears old\n";
118 myAget+, // 우치 증기 연산자

12:  ++yourAge; // 전치 증가 연산

1355   cout << "One year passes...\n";

14:   cout << "I am:\t" << myAge << "\tyears old.\n";

15:   cout << "You are:\t" << yourAge << "\tyears old\n";

16:   cout << "Another year passes\n";
17: cout << "I amz:\t" << myAget++ << "\tyears old.\n";    //두 B2| 차이를
18; cout << "You are:\t" << ++yourAge << "\tyears old\n"; //주목하십시오

192   cout << "Let's print it again.\n";

20:   cout << "I am:\t" << myAge << "\tyears old.\n";

21:   cout << "You are:\t" << yourAge << "\tyears old\n";
22:   return 0;

235: 3)

결과  I am:     39 years old.

You are: 39 years old
One year passes...

I am:     40 years old.
You are: 40 years old
Another year passes

I am:     40 years old.
You are: 41 years old
Let's print it again.

I am:     41 years old.
You are: 41 years old


===== PAGE 89 =====
86 ee AIF

분석  7번과 BA SoA 2개의 APS 변수가 선언되었고 각각은 39로 초기화되
=~
번

었습니다. 그 We 9번과 10
11번 줄에서 myAget= 후치 연산자를 사용하여 증가되었고, 12번 줄에서 yourAge
는 전치 연산자를 이용하여 증가되었습니다. 결과는 14번 줄과 15번 줄에 출력되
었고 결과는 동일합니다.(둘 다 40이 됩니다.)

17번 줄에서 7&86는 출력문장의 일부분에서 증가되었고 후치 증가 연산자를 사
용합니다. 후치 연산자이기 때문에 출력 뒤에 증가가 일어납니다. 따라서 40이 다
시 한번 출력됩니다. 대조적으로 18번 줄에서 1004&86는 전치 연산자를 사용하여
증가되었습니다. 따라서 Seo] 일어나기 전 증가가 되고 따라서 출력은 41로 됩
니다.

마지막으로 20번과 21번 SoA RSS 다시 출력이 됩니다. 증가문은 끝났기 때
문에 myAgeS} yourAge= 모두 41의 AS 갖게 됩니다.

엽산자 우선순위(바666006066)
복합 문장에서
x=5+3%*8;

이 있을 때 연산 순위는 어떻게 되겠습니까? 덧셈이 먼저 된다면 결과는 8 * 8인
@가 나올 것입니다. Halo] 먼저 된다면 결과는 5 + 24인 29가 나을 것입니다.

모든 연산자는 우선순위가 있고 그 완전한 보기는 부록 Aol 실려있습니다. 곱셈
은 덧셈에 비해 높은 우선순위를 가지고 있고 따라서 결과는 29가 됩니다.

두 개의 연산자가 똑같은 우선순위를 갖고 있다면 윈쪽부터 오른쪽으로 연산이
일어나게 됩니다. 따라서

K=5¢ Zt BO GHG;

는 곱셈이 먼저, 왼쪽에서 오른쪽으로 진행되어 일어납니다. 따라서 8 * 9 = 72,
6 * 4 = 24가 일어납니다. 수식은 다시

×=543+7ㅠ29240

로 됩니다. 이번에는 Gao] 왼쪽에서 오른쪽으로 Yop 5 + 3 = & 8 + 72 =
80; 80 + 24 = 104;가 됩니다.



===== PAGE 90 =====
ol}

연산자(대입 연산쟈)는 오른쪽에서 왼쪽 순으로 연산이 일어납
니다. 어떤 경우든 우선순위가 여러분의 요구에 부응하지 못하면 어
생되겠습니까? 다음을 생각해 봅시다.

TotalSeconds = NumMinutesToThink + NumMinutesToType * 60 ;

re
ing
EL
N
Es
뚜

이 식에서 여러분은. NumMinutesToTypeo] 60S Ft 의도는 없었고 . 단지
NumMinutesToThink?} NumMinutesToTypeS 더한 뒤 총 AQ 초를 구하기 위해 OL 곱
할 필요가 있었습니다.

이런 경우 연산 우선순위를 바꾸기 위해 BES 사용할 수 있습니다. 괄호 안의
항목들이 먼저 연산이 됩니다. 따라서

TotalSeconds = ( NumMinutesToThink + NumMinutesToType ) * 60 ;

이 여러분에게 원하는 결과를 가져다 S 것입니다.

괄오(]650100 Parentheses)

복잡한 수식을 하려면 BES 중첩하여 S 경우가 있습니다. |S 들어, 총 소요
초를 구하고, 그 시간을 곱하기 전에 총 인원을 전부 구하려면

TotalPersonSeconds = ( ( NumMinutesToThink + NumMinutesToType ) * 60 )
* ( PeopleInTheOffice + PeopleOnVacation ) ) ;

이 복잡한 +42 안쪽으로부터 읽혀집니다. 먼저 NumMinutesToThink7}
NumMinutesToTypeol] - 더해지고 60°] | 곱해집니다. 다음 PeoplelnTheOffice7}
PeopleOnVacation®]] 더해집니다. 마지막으로 두 개가 곱해집니다

이 예제는 중요한 관련된 주제를 이끌어냄니다. 이 문장은 사람이 이해하긴 힘들
지만 컴퓨터는 이해하기 쉽다는 것입니다. 똑같은 AS 임시 정수형 변수들을 써
서 다시 구현하였습니다.

TotalMinutes = NumMinutesToThink + NumMinutesToType ;

TotalSeconds = TotalMinutes * 60 ;

TotalPeople = PeopleInTheOffice + PeopleOnVacation ;
Total PersonSeconds = TotalPeople * TotalSeconds ;

이 예문은 쓰기에 시간이 걸리고 더 많은 임시 변수들을 요구합니다. 하지만 이
해하기는 쉽습니다. 이 코드가 무엇을 하는지 알기 쉽게 하기 위해 땐 위에 주석
을 만듭시다. 그리고 60을 기호 상수로 바꾸어 봅시다. 이해하기와 유지 보수가
다소 쉬워질 것입니다.


===== PAGE 91 =====
88 ee Ait

DON'T

DO     수식은 US 갖는다는 것을 기억합시다

DO     변수가 수식에 사용되기 전 증까(감소)를 시키려면 전치 연산자를 사용합니다.
DO    변수기 수식에 사용된 F 증가(감소)를 시키려면 FA] 연산자를사용밥니다.
00     우선순위를 임의로 바꾸려면 ABTS 사용합시다.

DON'T 중첩은 깊게 사용하지 AA 이해와 유지 보수에 힘듭니다.

참값의 속성

0++에서 0은 거짓 값으로 간주되고 그 이외의 모든 값은 참값으로 간주됩니다
(하지만 참값은 보통 1을 씀니다) 따라서 수식이 만일 거짓이면, 수식은 0과 같
고 수식이 0이면 그 수식은 거짓입니다. 수식이 참이면 그 수식은 0 이외의 값을
갖고 수식이 0아닌 값을 가지면 그 수식은 참입니다.

관계 연산자는 두 eazy} 같은지 혹은 shy} 다른 수보다 크거나 같은지 결정할
때 쓰입니다. 모든 관계 연산자의 연산 결과는 1(참)이거나 0(거짓)입니다. 관계
연산자는 뒤의 [표 4.1]에 나와 있습니다.

만일 정수형 변수 myAge7} 40이라는| 값을 갖고 yourAge7} 39를
닌지를 등치 연산자(==)를 사용하여 판단할 수 있습니다.

myAge == yourAge // myAget yourAge2} 같은가?
이 수식은 거짓이므로 0을 반환합니다.

myAge > yourAge; // myAge ft yourAge#*} 큰가?

uv
많은 프로그래머들이 대입 연산자(=)와 등지 연산자(==)를 론동합니다. 이런 경우 지
fk ad a hee hal

6가지의 관계 연산자가 있습니다. 등치 연산자(==),

른 MA >), 크거나 같은 연
산자( >= ), 작은 연산자( < ), 작거나 같은 연산자( <= ), 부

등 연산자( != )입니다,


===== PAGE 92 =====
7
A
A
4
A
A

보기

100 == 50
50 == 50
100 != 50
50 != 50
100 > 50
50 > 50
100 >= 50
50 )= 50
100 < 50
50 < 50
100 <= 50
50 <= 50

Ho}
tc}

이름

등치
다

크거나
작거나

크다

[표 4.1] 관계 연산자

as              = TD)            midi ae
ip]             ny
2    <b             그 도            ol 대
g    <i              Kas            xr Se
= K               5
an              Bs 이!             aay
a               Nu            이 그
r|            sR             ay
떠              ™ AF             x
비             시 ®            7 ol
old                Ub.          Wo ho
rs             ae             K
ee             고 교우          moh
Be ite          D> 27       9 더
글 호            그 @ 그         아시,
a °             Sx aS          4+ 더
mK             Ul ox A            oy
ol IP           m   3}         ow
a          -*é        rm
호     ST.
= ee              oe ov tH 의       4b =
0   이 2       버
10 K              3 yn a          aS
는 40             이 & IF  a       4b 은
41 a              nn Fo yy OF       는
303           시어 고모      ee
<  <              더 이 ri  118          5
Bl Bl           만     주     이 oO
=         대요 프      고.
65 90 브         머 끄   :      가
00 or a           al 2 com  ee       nh 이
icy  S ae. ot
는          ow Seo 이
z              ah) ‘Ke 로  5 <b oh  Ar +
88        wo pe wm yO wT
Te AN    AU d\n

봅시다.

=

=

GE

으로 간주되고 문장은 실행됩니다. 다


===== PAGE 93 =====
90 ce ANS

if ( bigNumber > smal lNumber )
bigNumber = smallNumber ;

이 SLE bigNumber$} smallNumberS 4 ]교합니다. bigNumber7} 크면 두 번째 줄
에

서 smallNumber 값을 bigNumberol] 대입합니다.

중괄호에 의해 둘러싸인 블록 문장은 단일 문장과 동등하기 때문에 다음과 같은
분기는 큰 BBS 발생합니다.
if (수식)
{

문장 1 ;

문장 2 ;

문장 3
3

간단한 사용 예가 있습니다.

if (bigNumber > smal LNumber)

{
bigNumber = smallNumber ;
cout << "bigNumber: " << bigNumber << "\n" ;
cout << "smallNumber: " << smal lLNumber << "\n" ;
가
ㅇ

1번에는 bigNumber7} 50001400006보다 크면 bigNumber= smallNumber 값으로 설
duly, 결과 메시지도 출력됩니다. [리스트 4.4|는 관계 연산자에 의거한 보다 중
분한 분기의 모습을 보여줍니다.

전

[리스트 4.4] 관계 연산자에 의거한 분기 al

14: // [리스트 4.4]

2: // By 였산자 시용

3: #include <iostream.h>

4: int main

55

6:    int RedSoxScore, YankeesScore;

144    cout << "Enter the score for the Red Sox: ";
8:    cin >> RedSoxScore;

9:

10:    cout << "\nEnter the score for the Yankees: ",;
11:   cin >> YankeesScore;

12%

133   cout << "\n" 7

=
a



===== PAGE 94 =====
Wey
165
a WA
18:
AD:
20:
els
22:
25%
24:
251
26:
2
287
29:
30:
S18
32:
53:
34:
55%
36:
3s
503
598
40:
41:
G2: J

if (RedSoxScore > YankeesScore)
cout << "Go Sox!\n";

if (RedSoxScore < YankeesScore)
{

cout << "Go Yankees!\n";

cout << "Happy days in New York!\n";
}

if (RedSoxScore == YankeesScore)

{
cout << "A tie? Naah, can't be.\n";
cout << "Give me the real score for the Yanks: ";
cin >> YankeesScore;

if (RedSoxScore > YankeesScore)
cout << "Knew it! Go Sox!";

if (YankeesScore > RedSoxScore)
cout << "Knew it! Go Yanks!";

if (YankeesScore == RedSoxScore)

cout << "Wow, it really was a tie!";

cout << "\nThanks for the telling me.\n";
return 0;

Ai b Enter the score for the Red Sox: 10

Enter the score for the Yankees: 10

A tie? Naah, can't be.

Give me the real score for the Yanks: 8
Knew it! Go Sox!

Thanks for telling me.

00

=

셀 < 프로그램은 두 아구팀의 성적에 대한 입력을 요구하여 변수에 저장합니
다

이 변수들은 15, 18, 24번 So] 문장에서 비교됩니다.

한 팀의 성적이 다른 팀보다 높으면 안내 메시지가 출력됩니다. 점수가 같으면
24번 줄에서 시작하여 38번 줄에서 끝나는 블록문으로 들어가게 됩니다. 두 번째
성적이 다시 요구되고 입력된 성적이 다시 비교됩니다.


===== PAGE 95 =====
92 co 제1주

처음의 Yankees®] 성적이 Red Sox 성적보다 좋으면 15번 줄의 #문이 거짓으로
판명하고 16번 Sl 호출되지 않습니다. 18번 So] FOB 되고 20, 21번 Fo] 호
출될 것입니다. 그리고 24번 줄이 실행될 것이고 거짓으로 판명될 것입니다. 프로

그램은 나머지 BSS 건너뛰어 39번 줄로 가게 됩니다.
이번 보기에서는 앞의 if 문장에서 참값이 되도 HS if 문장을 또 검사합니다.

$04 '1|(Indentation Style)
[리스트 4시는 if 문장의 들여쓰기에 있어서 들여쓰는 하나의 방식을 보여줍니다.
프로그래머들에게 어떤 중괄호 배열이 가장 좋은지 주장해 보라는 것은 마치 종
교 전쟁을 일으켜 보자는 이야기와 똑같습니다. 십인십색이겠지만 그래도 대략
세 가지로 요약됩니다.

를 시작 중괄호를 SHE 뒤에 붙여쓰고 마감 중괄호는 | 칸에 맞춰 쓰자는 주장이 하나입

ro

eeu
버터
if (#4) 《
문장 ;
}

if (수식)
<i

문장 ;
3

if (수식)

{

wil @

+
이 책에서는 중간에 있는 방법을 쓰기로 합니다. 왜냐하면 이 방법이 중괄호들이
각각 한 줄씩 열기 때문에 블록의 이 끝나는 aS 쉽게 알 수 있기 때문입
니다. 다시 말하지만 어떤 방침을 고집하느냐 보다는 한번 선택한 것을 일관성
있게 사용하는 것이 보다 중요합니다



===== PAGE 96 =====
조건이(\6090×900[66 > Yankees) 참이면 “Go Sox!"2 수행하고 거짓이면 “00
g  z

Yanks!" 수행하게 할 수 있습니다. 여태껏 보여준 것은 하나의 조건을
고, 또 하나의 조건문을 수행하여 원하는 것을 찾는 것인데, 중복되게 조건을 비
교합니다. 예약어 elses 쓰면 BA 좋은 SES 만듭니다.

[리스트 4.5]는 656를 사용하는 예를 보여줍니다.

[리스트 4.5] else 사응한 off

1: // [리스트 4153

2: // else 사용

3: #include <iostream.h>

4: int main()

5s 에

6%    int firstNumber, secondNumber;

2    cout << "Please enter a big number: ";

8:    cin >> firstNumber;

oF    cout << "\nPlease enter a smaller number: ";
10:   cin >> secondNumber;

V1:   if (firstNumber > secondNumber)

12:      cout << "\nThanks!\n";

13°   else

14:      cout << "\nOops. The second is bigger!";
15:

16:   return 0;

17587

겔과  Please enter a big number: 10

Please enter a small number: 12

Oops. The second is bigger!

a 줄의 if 문장이 계산됩니다. 조건이 참이면 12번 줄의 문장이 수행됩니
다. 거짓이면 14번 줄의 문장이 수행됩니다. 13번 줄의 else 절이 없다면 if
조건문에 관계없이 14번 줄이 수행될 것입니다. #문은 12번 줄에서 끝나기 때문
입니다.                                   |

00
4


===== PAGE 97 =====
94 eo 제1주

와 cleo] 각 부분은 중괄호를 사용하여 블록문으로 만들 수 있습니다.

if 문장
if 문장의 FEE 다음과 같습니다.
제 1 형태

if (주식)
문장 1;

ee

Pr

수식이 참으로 판명되면 문장 1이 수행되고 프로그램은 다음 문장 22 넘어갑니다. 수식
이 거짓이면 문장 1은 무시되고 다음 문장 2로 넘어갑니다. 여기서 문장이란 세미콜론으
로 끝나는 하나의 문장일 수도 있고 중괄호가 있는 블록문일 수도 있습니다.
제 2 형태

if (수식)
1;

Ao
ot

else

om

=

Ao

문장 3;

수식이 참이면 문장 1이 수행되고 그렇지 않으면 문장 2가 수행됩니다. 그후 문장 30] +
행됩니다.                      |
예제 1

if (SomeValue < 10)

cout << "SomeValue is less than 10");
else

cout << "SomeValue is not less than 10!");
cout << "Done." << endl;

ifs} else 문장 안에는 어떠한 BIS - 심지어 또 다른 와 066도 - 쓰일 수 있다
으

는 점을 유의해야 합니다. 이런 경우 복합 #문을 보게 됩니다.
if ( 수식 1 )
af
if C44) 2)
문장 1
1 ㅇ  7



===== PAGE 98 =====
{
if ( 수식 3 )
문장 2
else
문장 3;
}
}
else
문장 4;
$4 1이 참이고 수식 2가 참이먼 문장 1을 BNI. 수석 1이 참이고 수석 2
가 거짓이면 그리고 수식 3이 참이면 문장 2를 수행합니다. 수식 1이 참이고 수
식 2 및 수식 30] 거짓이면 문장 3을 수행합니다, 마지막으로 수석 1이 거깃이떤
문장 4를 수행합니다. 보다시피 복합 #문은 약간 복잡합니다.
[리스트 4.6|이 이러한 보기를 보여줍니다.

[리스트 4.6] 복합, 중첩 문

CONDUPFWD =
er 090 이 이 이 0

ee 그 2 ee ee ee ee 6
SOON A UAWNH BSB OF
 00 00 00 00 00 ne 00 00 one

[69 [60 [60 60 NM PLP PY
NOU FWD |=
ee … ee ee

ine)
oO
os …

// [리스트 4.6] 복합, 중첩 1+문

//

#include <iostream.h>

int main()

6
/7/ 두 개의 값 값을 요구
// 각값 갔을 bi gNumberSt LittleNumber] 대입
// 만일 bighuaberf LittleNumber#*} 크면
// 나누어 떨어지는지 검사하고
// 그렇다면 같은 수인지 검사함.

int firstNumber, secondNumber;

cout << "Enter two numbers.\nFirst: ";
cin >> firstNumber;

cout << "\nSecond: ";

cin >> secondNumber;

cout << "\n\n";

if (firstNumber >= secondNumber)
{
if (< (firstNumber % secondNumber) == 0) // 나누어 펄어지는가?
Hf
if (firstNumber == secondNumber)
cout << "They are the same!\n";
else
cout << "They are evenly divisible!\n";


===== PAGE 99 =====
96 co 제주

28:      else

29%      .   cout << "They are not evenly divisible!\n";
30:   }

$1:   else

52:      cout << "Hey! The second one is larger!\n";
55:   return 0;

348 3

결과  Enter two numbers.

First: 10
Second: 2

Thery are evenly divisible!

불샐 두 개의 숫자를 입력받아 비교합니다. 19번 줄의 첫 #문은 첫 번재 숫자가

두 번째 입력숫자보다 크거나 '같은지를 검사합니다. 그렇지 않으면 31번 줄
의 050문이 수행됩니다. 처음의 가 참이면 20번 Se] 블록문이 수행되며 21번
줄의 두 번째 #문이 검사됩니다. 이 부분은 첫 번째 FS 두 번째 수로 나머지
연산을 한 뒤 나머지가 없는지 검사합니다. 참이면 두 개의 숫자는 약수ㆍ 배수

a)

관계입니다. 23번 줄의 #문은 같은지를 검사하고 적절한 메시지를 출력합니다.

중첩 [문에서의 중괄호 사응

#문에서 문장이 하나일 경우 중괄호를 we 무방하고 다음과 같이 써도 됩니다.

if Ox>y)        // Of 보다 크면
if €x<z)        // xf [2보다 작으면
KEY;             // ×에 yah 대입합시다.
매우 여러 번 중첩된 프로그램을 작성할 때, 이미 혼란을 가져올 수도 있습니
다. 공백 문자와 들여쓰기가 프로그래머에게 상당히 편리할 수 있다는 것을 기억

합시다. 컴파일러에게는 아무런 영향도 foe. 혼동하기 쉽
8186를 쓸 수 있습니다. [리스트 4.71은 이러한 본보기를 보

요
퍼시
도
무비

[리스트 4.7] [와 BS 이루는 156에서 중괄호가 왜 편리한가

12 27
2: // [리스트 4.7] 와 BS 이루는 6156에석 중괄호가 A 편리한가
3: #include <iostream.h>



===== PAGE 100 =====
4: int main()

5s 솜

6:    int %

Te    cout << "Enter a number Less than 10 or greater than 100: ":
8                                    ‘

cA

:    cin >> x;
or    cout << "\q';
10:
1716   if (x > 10)
122      if (x > 100)
156       cout << "More than 100, Thanks!\n";
14: else     // 어느 if 붙은 else 인지 모호함
158     cout << "Less than 10, Thanks!\n";
16:
1s   return 0;
18% 3

겔과  Enter a number less than 10 or greater than 100: 20
Less than 10, thanks!

BAY o] 프로그램은 103 100 바깥의 숫자를 물어보고, 올바른 값이 들어오면
“…118016!”를 출력하는 프로그램입니다.

—
—

줄의 1문이 참으로 판단되면 124 So] 실행됩니다. 이 경우 2a Se 입
수가 10보다 크면 수행됩니다. 12번 Se 역시 #문을 포함하고 있습니다. 7
입력된 수가 100보다 크면 수행됩니다. 입력된 수가 100보다 작으면 13번
수행됩니다.

입력된 수가 10 이하이면 10번 문장을 거짓이 되고 프로그램의 제어권은 다음
항목으로 분기하는데 이 경우는 16번 줄입니다. 따라서 10보다 작은 숫자를 입력
하면 아래와 같이 아무 것도 출력되지 않습니다.

으 ro tt ez

nN {St

Enter a number less than 10 or greater than 100: 9

144 줄에 있는 이 elseAL 들여쓰기 표현만 가지고 보면 분명히 11H 줄의 ifs

과 BS 이룬 듯 보이지만 실제 ian 12 a  줄의 #와 BS 이루고 있고
이 프로그램은 프로그래머의 의도와 다른 모호한 버그를 간직하고 있습니다. 이
버그는 컴파일러도 모르는 버그입니다. 이 프로그램은 eit 제대로 되며 게
다가 잘 수행됩니다. 100보다 큰 수를 입력하는 한 이 프로그램은 잘 돌아갑니다.
[리스트 4.8]은 필요한 중괄호를 사용함으로써 프로그램을 가려


===== PAGE 101 =====
98 ee MIF

[리스트 4.8] 문에서 적절한 중괄호 사응하기

1: // [리스트 4.8] 1+문에서 적절한 중괄호 사용하기
2: Ss

3: #include <iostream.h>

4: int main()

a: ft

6:    int x-

ie:    cout << "Enter a number Less than 10 or greater than 100: ";
8:    Cine> xr

9:   “cout << ma;

10:

As    1f «x > 10)

123   {

15%      if (x > 100)

Th       cout << "More than 100, Thanks!\n";
158   E

16:   else

10      cout << "Less than 10, Thanks!\n";
18:   return 0;

18: 3

결과  Enter a number Less than 10 or greater than 100: 20
분석  12번과 15번 So] 중괄호는 그 안의 모든 AS sje] 블록문으로 만듭니
다. 그리고 16번 노노. else 문은 11번 줄의 와 JES 바대로 짝을 이룹니
다. 사용자가 20을 입력하면 11번 So] if BFS 참이 됩니다. 그러나 13번 줄으
#문은 거짓이 됩니다. 따라서 아무런 출력도 없습니다. 프로그래머가 14번 줄 다

니                         프로
음에 656절을 집어넣어 장애 발생시 출력을 하게 하였으면

이 책에 있는 프로                                       프로
그램은 되도록 tes                                         위한
특별한 장치를 ^                                          사용
자의 실수를 다루기 위

더 좋을 뻔했습니다.



===== PAGE 102 =====
논리 24At logical operator)

여러분은 가끔 동시에 하나 이상의 관계 연산자를 사용할 때가 있습니다. “xt y
보다 크고 또 》는 2보다 큰가” 프로그램은 어떤 행동을 취하기 위해 때때로 이
두 조건이 참인가 혹은 어떤 다른 조건이 참인가를 조사할 필요가 있습니다.
다음과 같은 논리를 가진 다소 재미있는 벨060000)을 생각해 봅시다. “현관 wo}
울리면서 오후 6시가 넘었고 공휴일 혹은 주말이 아닌 경우엔 Aas 불 러라.”
(+에서는 이러한 종류의 AAS 위해 3개의 논리 연산자를 갖습니다. [표 4.21에
나타나 있습니다.

[표 4.2] 논리 연산자

a 2: a       _ 보기

논리곱          &&         수식 1 && 수식 2
논리합                it /                수식 1 || 수식 2
논리적 부정          !              !수식

논리곱(1091081 AND)
논리곱 문장은 두 개의 FAS 계산하여 두 개가 동시에 참이면 논리곱   은
참이 됩니다. 누군가 배가 고프고 또 동시에 돈을 가지고 있다면 we 사먹을 것
이다'라는 식입니다. 따라서
if ( (x == 5) && (> == 5) )
는 만일 xs} 가 동시에 5이면 참이고 S 중 하나가 57} 아니면 거짓입니다. 문
장이 참이 되기 위해서는 두 개의 FAO] 모두 Ao] 되어야 합니다.

은 두 개의 && 기호입니다. 하나의 &는 19일째 배우게 되는 다른 연산자

논리합(09108 OR)
논리합도 두 개의 AS 계산합니다. 둘 중 하나가 참이면 수식은 참이 됩니다. +
군가 돈이 있거나 신용카드가 있다면 금액을 지불할 수가 있다라는 식입니다. 돈
런 신용카드 두 개를 동시에 갖고 있을 필요는 없습니다. 하나만 있으면 됩니다.
물론, 둘 다 있어 UB 것은 없지만) 따라서


===== PAGE 103 =====
100 ee AIS

if ( (x == 5) tt Cy == 5) )

에서는 xt y S 중의 하나가 5이면 참이 됩니다.(물론, 둘 다 5이어도 참입니다.)
논리곱은 두 개의 || 기호입니다. 하나의 | 기호는 19일째 배우게 될 다른 연산
자입니다.

논리적 (logical NOT)
논리적 부정문은 수식이 거짓으로 판명되면 참이 됩니다. 다시 말해 수식이 거짓
으로 판단되면 그 검사의 ea  i 됩니다. 다음 예를 보면 이해가 됩니다.
if (!(<==5) )
라는 문장은 x7} 5가 아닐 때 참이 됩니다. 바꾸어 쓰면 다음과 같습니다.

if (x != 5)

관게 엽산자 QAZP(Relational Precedence)
관계 연산자와 논리 연산자는 CH 수식이므로 반환값을 갖습니다. 1(참) 혹은 0
(거짓) 입니다. 그리고 다른 모든 수식처럼 그 연산자들도 우선순위를 가지며(부
록 ㅅ 참조) 어떤 식이 먼저 연산되는지를 가립니다. 이 사실은 다음 문장의 값을
결정할 때 중요합니다.
if (% > 57866 y> 3 i 2852

만약 x3} y7t = 다 동시에 5보다 크거나 SS 2가 5보다 크면-이 “a 참이라
고 할 수도 있고, x7} 5보만 크고 동시에 )가 5부다" 크거나 2가 5보다 크면 참이
라고 할 수도 있습니다.

만일 x7} 3이고^$와 2가 들 마 10이면 첫 번째 해석은 is 이 될 것입니다.2가 SB
다 크므로 x9} yo} 값은 무사됩니다.) 그러나 두 번째 방식으로 해석하면 거짓이
됩니다.※가 5보다 작으므로 나머지는 무시됩니다.)

우선 EAE 어떤 관계가 처음 연산될 것인지 정합니다. 괄호가 우선순위
수 있고 문장을 보다 명확히 할 수 있습니다.

if ((x>5) 868 (2511 22522

0

바꿀



===== PAGE 104 =====
제4일 수식과 문장 ee 101

앞에서 주어진 값들을 쓰면 이 문장은 거짓이 됩니다. x7} 5보다 작기 때문에 논
qe 연산자의 Ase 무조건 거짓이고 따라서 전체 문장은 거짓이 됩니다. 논리
곱 연산자는 둘 다 참이어야 한다는 점을 기억합시다.

여러 개의 연산자가 있을 땐 괄료를 쓰는 편이 닛습니다. 프로그램을 작성하는 최대
목표는 제대로 작동하면서 이테하기 쉬운 문장을 쓰는 것입니다.

참과 거짓에 대한 몇 마디 추가

++에서 OF 거짓이고 그 이외의 값은 참입니다. FAS 항상 값을 갖기 때문에
많은 프로그래머들은 #문에서 이러한 특징을 잘 활용합니다. 다음의 문장은

if (x)   fi ot 참 ¢ 0의 아님 ) 월 경우

X = >
는 “%가 0이 아닌 값을 가지면 0으로 설정합시다”라고 말할 수 있습니다. 이는
약간 HS 쓴 것 같은 경우인데 다음과 같이 쓰면 간결해집니다
if (x != 0 ) _ // xf 0이 아니면

x = 0;
두 개의 문장 다 맞지만 후자가 더 간명합니다. 후자 SO} 논리검사를 하는 방식
이 전자의 0 아닌 값을 검사하는 방식보다 더 좋습니다. 아래의 두 개는 같은 직

입니다.

if ( !x )// xt 거짓이면
if (x == 0 )// xf 0이면

하지만 두 번째 식이 더 이해하기 쉽고 명료합니다.

00 논리 검사시 명확하고 우선순위를 정확히 하기 위해 Bee 사용합시다
00 FHF +문에서 666문을 명확히 하게 하고 버그를 피하기 위해 중괄호를
사용합시다.

ㅁ

DON'T if (x )와 + ( ×!= 0 )는 같은 식이지만 Sapp 명료합니다. 전자를 쓰
지 BEA] EF

DON'T if ( ik )와 +} (x == 0 )는 같지만 후작가 명료하므로 전자를 쓰지 ot
지맥,



===== PAGE 105 =====
102 ee 제1주

여러분 자신의 불린 (논리) HAYS 쓰는 것은 Est 예입니다. enum Bool { FALSE,
TRUE }2t 정의하면 FALSEE 0이 되고|106는 1°] 됩니다.

조건 연산자 SX 삼항 연산자
(Conditional Operator or Ternary Operator)

건 연산자 (2: )는 0++에서 단 하나 있는 삼항 연산자인데 3개의 항을 갖는
산자입니다.

(수식 1) ? (수식 2) : (수식 3)

|는 “수식 1이 참이면 수식 2의 값을 반환하고, 그렇지 않으면 수식 3을 반환한
다” 입니다. 반환값이 변수에 대입됩니다. [리스트 4의는 ES 사용한 프로그램
을 조건 연산자를 써서 나타내었습니다.

[리스트 4.9] 조건 연산자 예제

1: // [리스트 4.9] 조건 연산자 예제
2: 7/
3: #include <iostream.h>
4: int mainQ
be 4
6:    Int Xp Vo Zp
C3    cout << "Enter two numbers.\n";
8:    cout << "First: “3
9:    610 >> xe
10:    cout << "\nSecond: ";
11:   cin 223
12:   cout << "\ni"s
155
14s    if (x >y)
1590      2=×;
16:   else
ACs      z=y;
18:
19%    cout << “zi " << 25
cout << "\n":

nm mM
= oO



===== PAGE 106 =====
제4일 수식과 문장 ee 103

22:  Z's (x oy) 2x lye
23:

24:    6046 25 02)
25:   6046 < 디오

26:   return 0;

27: 고

결과 Enter two numbers.
Firste.5

Second: 8

ze 8
z: 8
분석 세 개의 정수형 변수가 만들어졌는데 yy 그리고 2입니다. 처음 두 개의
변수는 사용자에 의해 값이 주어졌습니다. 14번 So} 문은 어떤 수가 더
큰지를 검사하고 큰 AS 2에 대입합니다. 그 Yo] 19번 줄에서 출력됩니다.

22번 줄의 조건 연산자가 똑같은 검사를 하고 큰 값을 2에 대입하였습니다. “가
ya 크면 ×값을 반환하고 그렇지 않으면 )값을 반환한다.”라고 읽습니다. 반환

은 2에 대입됩니다. 그 Re 24번 So] 출력됩니다. 보다시피 조건 연산자는 if
… 656 문장의 축약형입니다.

이번 91 BE 것을 다루었습니다. 무엇이 Cero] 수식이고 문장인지를 배웠
c                  게 #문은 작동하는지 배웠습니다. 한 쌍의 중괄호
에 의해 ae 블록문이 단일 문장이 쓰일 수 있는 곳에서 사용되는 법을 알아

ogy
a
.
ttlo
에요
us

산                       하는7 도 2
관계 연산자를 이용하여 비교하는 WS 배웠고 대입 a

위를 바꾸는데 어떻게 사용되는 지도
더 명확하고 다루기 쉽게 된다는 것을 배


===== PAGE 107 =====
104 ee 제1주

O&A

어떤 연산자가 먼저 계산될 것인가를 결정할 때 때때로 불필요하게 BSS 쓰는 이
Q

유는?
A 컴파일러가 우선 순위를 잘 알게 하고 또 프로그래머가 우선 순위를 잘 알 수 있게
하는데, 무엇보다도 B7] 쉬운 프로그램이 유지 보수하기도 쉽습니다.

&
re

계 연산자가 항상 0이나 1S 반환하면, 왜 다른 값들은 참으로 생각됩니까?

A 관계 연산자는 1이나 0을 반환합니다. 그러나  0   식은 값을 반환하고 그 값들
은 문에서 계산될 수 있어야 합니다. 보기를 보

om

if ((x=atb) == 35)
이는 올바른 C++ 문장입니다. 만약 a + 『의 값이 35가 아니더라도 값은 계산되어야
하고 ×는 그 값을 대입 받아야 합니다.

Q 탭, 빈칸, 개행 SAKE 프로그램에 어떤 영향을 미칩니까?

A 프로그램 그 자체에는 영향을 안 미치나, 적절한 사용은 프로그램의 가독성을 높여



===== PAGE 108 =====
$ 만일 myAge, a, \가 모두 정수형 변수라면 각 연산후의 값들은 어떻게 됩니까?
myAge = 39;
a = myAgett;
b = ++myAge;

@ 8 + 2 * 3 의 값은?
7x = 3 과 × == 3의 차이점은?

8 각 값은 참입니까 거짓입니까?

=0
== 0 // ×가 0 의 값을 가졌다고 할 때

호 두 개의 StS 변수를 조사하여 큰 값을 작은 값으로 바꾸는 프로그램을 작성하되 ct
한 줄의 if 문장을 쓰고 단 하나의 6156문을 쓰도록 합시다.

: #include <iostream.h>
: int main ()

1
2
3
4    Int a, b, 0

De   cout << "Please enter three numbers\n";
6    cout << "a: "주          :

a    cin >> a;

8:   cout << "\nb: ";

9%   cin >> bs

10: cout << "\ner "5

11. 1h >> 0;

13: if (c=Ca-b) )

145 cout << “ar ":

158 6006 << a;

16: cout << "minus b: ";

17: cout << b;

18: cout << "equals c: ";

19: cout << c << endl;}

20: else

21: cout << "a-b does not equal c: " << endl;
22: return 0;


===== PAGE 109 =====
106 ee 제1주

3 위의 연습 SAS 입력한 뒤 컴파일ㅎ

링크한 뒤 실행시켜 보십시오.

20, 10, 50을

tal
차례로 입력합시다. 원하는 결과를 얻었습니까? 아니면 왜 그런지 ABS 하십시오.

4 아래의 프로그램을 살펴보고 결과를 예상해 봅시다.

이

1: #include <iostream.h>
2: int main®

3: 고

4:  int a= 1, b=1, c;

Dt if (c=Ca-b))

6:   cout << "The value of c is: "<< cj;
7   return 0;
8

[시
그
jo
18
Hu
U

모
milo
12
Ju
ow
부
mo
molly
kl
om
Ww
[위
an
>
oot
Ob
2
nL
>
모
ns
보
rr

보
16
흐
oo
niu
ux 2
of
oh
ask
fal



===== PAGE 110 =====


===== PAGE 111 =====
108 ee AIF

서문

객체 지향 프로그래밍은 그 관심점을 함수에서부터 객체로 옮겼지만, 그래도 함
역시 어떤 프로그램에서도 중심적인 부분을 차지합니다. 오늘 여러분은 다

= -ㅁ
아모
크
ont
de
ot
kl
=
ust
val
Fz
al
5

함수란 자료0200/에 동작을

니다. 모든 C+ 프로그램은 적어도 349 함수를 갖는데 바로 0800입니다
로그램이 처음 시작할 때 mando] 자동적으로 호출됩니다. 0000은 다른 함수를
부를 수 있고, 그것은 또 다른 것을 부를 수 있습니다
모든 함수는 그 고유의 이름을 갖고, 프로그램에서 그 ES 마주치게 되면 그
함수의 몸체 부분으로 실행이 분기됩니다. 함수가 반환되면 분기되었던 함수의
그 다음 줄을 실행합니다. 이 흐름은 [그림 5.1]에 있습니다
[그림 5.1]                프로그램
프로그램이 함수를 호   Main ()            함수
{ Statement;            함수
au 때 실행이 함수 | {Seem ㅣ ,           ：
로 Sl, 함수를   Statement   mal     비즈    함수
ㅎ추ㅎ     ox     func2 ():  — 7]  F return    함수      도래
= jhe =    Sete end  <          16000 | | =
되돌아갑니다.                                    ) ane                          func3 ();
14004 ();                   1
} Statement;    “                  return;       return;
함수4
return;
잘 설계된 함수는 특정한 그리고 이해되기 쉬운 업무를 수행합니다. 복잡한 업무
는 여러 개의 함수로 나뉘어지고, 각각이 차례로 불려집니다.
함수에는 두 개의 변종이 있습니다. 사용자 정의함수와 내장 함수입니다. 내장 함
수는 여러분의 컴파일러 안에 있는데 공급자가 여러분을 위해 제작한 것입니다.



===== PAGE 112 =====
함수

“1241(Declaring) it 함수 7Y°}(Definition)

프로그램 안에서 함수를 사용하려면 먼저 함수를 선언하고 다음에 정의를 해야
합니다. 선언은 컴파일러에게 함수의 이름, 반환값76040 value), 그 함수의 매개
변수를 알려줍니다. B= 컴파일러에게 함수가 어떻게 동작하는지 알려줍니다.
선언되지 않은 어떤 함수도 호출될 수 없습니다. 함수의 선언 부분을 함수 원형
(prototype)°]2} 합니다.

에 쓰고, 프로그램에서 #\00006문을 써서 그 파일을 포함시킴니다.

다른 함수에 의해 호출되기 전에 정의합니다. 이렇게 하면 정의는 선언의 효과를

0 oe |
£
a
rn
de:
met
4)
-구
Is
=
rir

비
은
=
rie
ost
010
그
tu
ot
5
pil

첫째, 함수가 특정 이유 때문에 파일 안에서 특정한 SAS 지녀야 한다는 것은
나쁜 생각입니다. 요구사항이 ube me  프로그램을 유지 보수하기 힘듭니다.

둘째, 특정 경우에 함수 20가 함수 6           2 다시 함수 DOE 함수 ale 부르
는 경우가 있습니다. 함수 00를 asta | 전에 함수 80를 정의하고, 또 동시에

함수 80를 정의하기 전에 함수 HOF 정의할 수는 없습니다. 따라서 둘 중의 하나

셋째, 함수 원형은 SIE 훌륭한 디버그 기술입니다. 여러분의 ago] 특정 개수
의 a1 HSE 선언하거나 혹은 특정형의 값을 반환하도록 한 뒤 실제 함수를
쓸 땐 원형과 다르게 했다면 컴파일러는 컴파일시 여러분의 Ass 가르쳐 줄 것
입니다

많은 내장 함수들은 그 Bee] 원형들이 이미 여러분이 #00006하는 파일 안에
선언되어 있습니다. 여러분이 여러분을 위해 만든 함수는 그 ABS 만들어 놓아
야합

니다.


===== PAGE 113 =====
110 ee 제1주

함수 원형은 문장인데 끝에 세미콜론을 붙여 원형임을 알립니다. 함수의 반환형
과 함수명, 매개 변수 일람들을 가지고 있습니다
매개 변수 일람은 모든 매개 변수들을 섬표에 의해 그 형과 함께 A 놓은 것입니

[그림 5.2]                                       oe
함수 원영의 3t                                       매개명
부분들                                                   /
unsigned shortint 1004168        (int length, int width) ;
반환값형       함수명         매개변수   세미콜론

함수 원형과 함수 정의는 반드시 위의 세 가지 점에서 일치해야 합니다. 그렇지
으면 컴파일 할 때 장애가 발생합니다. 그러나 함수 MIS 매개 변수의 이름
반드시 가질 필요는 없습니다. 하지만 형은 가져야 합니다. 아래와 같은 원형
완전히 올바른 것입니다.

ro ao ag

long Area (int, int)

ㅣ

oO

MAS AreaQZR= 함수명과 1008형의 반환형을 갖고, & 두 개의 aes 매개
수를 갖는다는 것을 알립니다. 이런 것이 올바른 것이긴 하지만 그리 좋은 생
으

아닙니다. 매개 변수가 이름을 갖는 것이 보다 명료합니다. 즉

long Area (int length, int width).

as)

가집니다. 아무 것도 공공연하게 서술되지 않았다면 기본적인
형입니다. 그러나 여러분의 프로그램에서 명료하게 함수형을 선언

이해하기가 쉽습니다. 물론 mainQe 포함해서 ' 입니다 [리스트 al]
46680라는 함수의 원형을 포함한 프로그램의 예제입니다.

oft    ie

[리스트 5.1] BAO 선업과 정의, 사웅법을 보여주는 예

1: // [리스트 5.13 함수의 선언과 정의, 사용법을 보여주는 예
2

3: typedef unsigned int USHORT;

4: #include <iostream.h>

5: USHORT FindArea(USHORT Length, USHORT width); // 함수의 원령
6

7

int main()



===== PAGE 114 =====
제5일 함수 ee 111

9:    USHORT LengthOfYard;

10:   USHORT widthOfYard;

Vs   USHORT areaOfYard;

12:

10    cout << "\nHow wide is your yard? ";
14:   cin >> widthOfYard;

15:    cout << "\nHow long is your yard? ";
16:   cin >> LengthOfYard;
174

18%   areaOfYard= FindArea(lengthOfYard,widthOfYard) ;
19:

20:    cout << "\nYour yard is ";

218   cout << areaOfYard;

22:   cout << '" square feet\n\n";

23:   return 0;

24: }

2o%

26: USHORT FindArea(USHORT lL, USHORT w)

27: {                 Fu whey Be 1 Set -
28: return l * w;

29: }

How wide is your yard? 100

que

How long is your yard? 200

Your yard is 20000 square feet

i] 0047680라는 함수의 원형이 SH So] 있습니다. 함수 원형    번

함수 정의와 비교하여 봅시다. 함수명, 반환형, 매개 변수형이 똑같습
만일 다르다면 컴파일러 장애가 발생할 것입니다. 사실 다른 점은 함수 원형
세미콜론으로 끝나며, 함수 본체를 갖지 않는다는 점입니다.

또한 원형에서의 매개 변수 이름은 10080 와 \00인데 실제 함수에서의 이름은 1과 \입
니다. 앞서 말한 대로 원형에서 매개 변수명은 쓰이지 않습니다. 하지만 그 매개 변수들
은 프로그래머에게 정보를 가르쳐 줍니다. 매개 변수명이 포함되어 있을 때 가능하면 맞
도록 구현시켜야 합니다. 이렇게 하는 것이 좋은 프로그래밍 습관이고 SES 줄입니다
하지만 반드시 필요 BAS 아닙니다.

Ag
a

드으
= ~

인수들이 선언되고 정의된 순서대로 함수에 전달되는데 이름이 같을 필
없습니다. 호출하는 함수에서는 widthOfYards} lengthOfYard= 전달하였는데

인

Ae  ir


===== PAGE 115 =====
112 ee 제1주

함수 원형에서는 160801와 widhe 선언하였습니다. 함수의 몸체는 비록 문장이 하
나밖에 없다고 하더라도 항상 중괄호로 끝납니다.

함수 정의(00108 the Function)                           .
함수 정의는 함수의 표제 부분과 몸체로 구성됩니다. 표제는 함수 원형과 정확히
똑같습니다. 단, 매개 변수의 이름이 있어야 된다는 점과 마지막에 세미콜론이 없
다는 점이 다릅니다.
함수의 몸체는 중괄호에 의해 둘러싸인 문장들로 구성되어 있습니다. [그림 53]
은 표제와 몸체 부분을 보여줍니다.

[그림 5.3]               반환값형          함수명         매개변수
Unsignd short int FindArea      int length, int width
몸체 부분                     !      이뽀        ,
{. 시작중괄호
// 문장

return   (length * width);

고 a   \

반환값
} 마감중괄호
1

함수
함수 원형

Mtg 함수명 Cl Bc 변수명 3 1   1G)
함수 정의

반완령 함수명 < [령 매개 변수명 1     )

{

문장 ;

}
함수 AGS 컴파일러에게 반환형, 함수명, 매개 변수 SSS 알려줍니다. 함수들은 꼭 매
개 변수를 가질 필요는 없는데, 이런 경우에는 매개 변수 목록을 가질 필요는 없습니다
매개 변수가 있을 때는 원형에서는 매개 밴수 OSS 반드시 필요로 하지 않으나 변수형은
필요로 합니다. 함수 AVS 항상 세미콜론으로 끝납니다



===== PAGE 116 =====
수 정의는 반환형과 매개 변수 목록에서 함수 원형과 일치해야 합니다. 함수 정의에서는
함수의 매개 변수에 반드시 이름을 주어야 하고 함수의 몸체는 반드시 중괄호로 둘러싸여
세미콜론으로 끝나야 하는데 함수 자체는 그럴 필요는 없

[때
습니다. 마감 중괄호로 끝나기만 하면 됩니다.

으
에
도
모
oh
고
is
1ㅁ
rn
Ao
0건

10

함수가 반환값이 있기만 하면, 함수는 (6[4이라는 문장으로 끝나야 하는데 이 returno|
어는 함수 내 어느 곳에서나 나타날 수 있습니다.
반환값을 갖습니다. 반환값이 명백하게 지정되어 있지 않으면, 반환형은 정수
스                                              fs]
[=

탁한 반환형을 주도록 합시다. 함수 값이 반환값이

트
at
bs!
Tok
+>
2
0묘
fet
[

[

[

함수 원형의 예
long FindArea (long Length, long width); // Longe 반환하고
// 두 개의 매개 변수를 가짐

void PrintMessage(int messageNumber) ;  // 4010형을 반환하고 하나의

int GetChoicd();           // 정수령을 반환하고 매개 변수는 없음
BadFunction();             // BEES 반환하고 매개 변수 없음

함수 정의 예

long FinArea (long Ｌ , long w)

{

return - & uw >
3
void PrintMessage (int whichMsg)
t

if (whichMsg == 0)

cout << "Hello.\n";

if CwhichMsg == 1)

cout << "Goodbye.\n";

if (whichMsg > 1)

cout <<" I'm confused.\n";
}

람수 AlY(Execution of Function)


===== PAGE 117 =====
114 ㅇㅇ AN

지역 변수(1061 Variable)

변수는 함수에게 전달될 수 있는 것이지만 여러분은 함수 몸체 안에 변수를 선언
할 수 있습니다. 이러한 것은 지역 변수를 사용함으로써 이루어지는데, 이 '지역
변수"란 이름은 그 함수 안에서만 존재하기 때문에 붙여진 이름입니다. 함수가 반
환되면 지역 변수는 더 이상 존재하지 않습니다.

지역 변수는 다른 함수와 마찬가지로 정의됩니다. 함수 안으로 전달된 매개

들도 역시 지역 변수처럼 생각될 수 있고 마치 함수 몸체 부분에서 정의된 것처
럼 명료하게 사용될 수 있습니다. [리스트 5그는 매개 변수 및 함수 안에서 지역
적으로 정의된 변수의 사용 예입니다.

[리스트 5.2] 지역 변수와 매개 변수의 사응 예

#include <iostream.h>

float Convert(float);
int main®)
{
float TempFer;
float TempCel;

CONAOUFWDY

cout << "Please enter the temperature in Fahrenheit: ";
cin >> TempFer;

TempCel = Convert (TempFer);

cout << "\nHere's the temperature in Celsius: ";
cout << TempCel << endl;

return 0;

ok of 5 8: = So
UW EWP RS] OO ㅣ

ae:

x ==
“I Oo

: float Convert(float TempFer)
a 개

== oo
‘Oo ©

float TempCel;
TempCel = ((TempFer - 32) * 5) / 9;
return TempCel;

nN Mm
- oO

cee 구

r=  Please enter the temperature in Fahrenheit: 212
Here's the temperature in Celsius: 100

Please enter the temperature in Fahrenheit: 32



===== PAGE 118 =====
Here's the temperature in Celsius: 0
Please enter the temperature in Fahrenheit: 85

Here's the temperature in Celsius: 29.4444

분석 6번과 7번 SAL 두 개의 408 변수들이 선언되었고, 하나는 화씨 온도를
저장하고 다른 하나는 섭씨온도를 저장합니다. 사용자는 9번 줄에서 화씨온
를 입력하고 그 값은 함수 0001600로 전달됩니다.

실행은 INA 줄의 함수 0000600의 첫째 줄로 분기되고 거기에서 지역 변수
TempCel°] 선언됩니다. 이 변수는 7번 줄의 TempCelz} 다릅니다. 이 변수는 함수
0001600에서만 존재하는 지역 변수입니다. 매개 wee 전달된 TempFer= main()
에 의해 전달된 지역 변수의 복사본입니다.

이 함수는 매개 변수 TempFerS} 지역 변수 180006을 가지고 프로그램에서 돌아
갑니다. 이 이름들을 바꾸어 입력하고 재컴파일한 뒤 실행되는지 볼 수 있습니다.

변수 16004@에서 32를 값의 결과값이 5가 곱해진 뒤 9로 나뉘어져 지역 w
수 7600208에 저장됩니다. 이 값은 함수의 반환값으로 반환되고 11번 줄의 0400
함수에서 변수 180008에 저장되고 13번 줄에서 출력됩니다.

이 함수는 3번 실행됩니다. 첫 번째는 물의 비등점인 화씨 212도가 섭씨 100도로
정확히 바뀌어짐을 확인하기 위한 212값이 전달됩니다. 두 번째 ae Bo} 어
는 점입니다. 세 번째 ABS 임의의 값을 주어 소수 값이 나오게 하였습니다.
연습 삼아 아래에 지정된 다른 변수명으로 위의 프로그램을 변환하여 실행해 봅
시다

1: #include <iostream.h>

2

3: float Convert(float);

4: int main()

뜨인 녹

6:    float TempFer;

C3    float TempCel;

i

9:    cout << "Please enter the temperature in Fahrenheit: ne
105   cin >> TempFer;

ate   TempCel = Convert(TempFer) ;

125   cout << "n\Here's the temperature in Celsius: ";
135   cout << TempCel << endl;

14:   return 0;

156. +


===== PAGE 119 =====
116 ee AF

: float Convert(float Fer)

= 4

float Cel;

Cel=(CFer - 32) * 5) / 9;
return Cel;

전역 4}¥A(Global Variable)

특정 함수의 바깥에서 정의된 변
함하여 프로그램내 어디에서나 사용 가능합니

FE

 다

저역
전역

로

을 가진 지역 변수
. 그러나 그 지역
비 전역 변수와 같

가리키게 됩

=
I

[리스트 5.3] 전역 및 지역 변수 al

ttlo of > 42

oy

1: #include <iostream.h>

2: void myFunction();     // 함수 원형

3

4: intx=5,y=73  // 전역 변수

5: int main()

6G: 고

ts

8:    cout << "x from main: " <«K x << "\n";
9:    cout << "y from main: " << y << "\n\n";
10:    myFunction();

qs    cout << "Back from myFunction!\n\n";



===== PAGE 120 =====
제5일 함수 ee 117

12:   cout << "x from main: " << x << "\n";

Ss    cout << "y from main: " << y << "\n";

14:   return 0;

15: 3

16:

17: void myFunction()

182) ¢

19:  (int y = 10;

20%   Nog var i

21: cout << "x from myFunction: " << x << "\n";
22: cout << "y from myFunction: " << y << "\n\n";
25%) J

겔과  x from main: 5

y from main: 7

x from myFunction: 5
y from myFunction: 10

Back from myFunction!

× from main: 5
y from main: 7

Jay 이 간단한 프로그램은 B 가지 핵심을 보여주는데, 잠재적으로 혼동을 7
오는 지역 변수와 전역 변수를 이야기합니다. 4번 줄에서 두 개의 전역

수 *와 》가 선언되었습니다. 전역 변수 xE se 초기화되었고 전역 변수 ye 7로

초기화되어 있습니다.

함수 78000에서 8번 줄과 9번 SS 이 변수들을 화면에 출력합니다. 4800 함

에서는 이 HSS 정의하지 않았음을 주목하기 바랍니다. 왜냐하면 그들은 전

변수이고 main) 함수에서 유용하기 때문입니다.
번

10번 줄에서 myFunction)°] 호출되었을 때 프로그램의 실행은 18번 줄로 갑니다.
여기에서 지역 변수 》가 선언되었고 그 값이 10으로 초기화되었습니다. 21번 줄
myFunction)-2 변수 xS 출력하는데      역 변수입니다. 한편 22번 줄에서 변
수 》라는 것이 사용되는데 이는 지역 변수입니다. 이름이 같기 때문에 전역 변수

므  4

는 감추어집니다.

함수 SSO] 끝난 뒤 제어권이 0800으로 되돌아오고 여기에서 다시 전역 변수
들을 출력합니다. 전역 변수 y= 함수 00800000000의 지역 변수 의 값에 전혀
영향을 받지 않았음을 보기 바랍니다.


===== PAGE 121 =====
118 ee 제1주

저여 변수 - 주의해야 할 단어
0++에서 전역 변수는 쓰일 수 있는 변수이지

만 실제 거의 안 쓰입니다. 0++은 0
필요악이라고까지 말해집니다. 여러

로부터 성장하였는데 (에서도 전역 wee

프로그램에서 필요하면서 매개 변수로 그 값을 일일이 전달할 필요가 없을 때 전
역 변수가 쓰입니다

전역 변수는 공유된 자료이기 때문에 위험합니다. 그리고 어느 함수 하나가 다른
함수 모르게 전역 변수를 바꿀 수 있기 때문에 더욱 그러합니다. 이러한 경우에
진짜 찾아내기 VE 버그를 만들어냄니다

공되지 않지만 0++만이 제공하는 매우 유용
한, 그리고 전역 변수를 대신하는 그 어떤 새로운 것을 접하게 될 것입니다.

지역 변수에 대라 추가사항

함수 yor 선언된 변수들은 지역범위 규칙을 갖습니다. 이는 앞서 말했듯이 그
번수들은 크 변수    one   JO) =] 함수 pu 올바로 사용될 수 있다는 AS 의미
합니다. 사실 빠삐 서는 여러분은 꼭 처음 부분에서가 아니라 함수내의 어느 곳
에서도 변수를 정의할 수 있습 at 변수의 범위 규칙은 정의된 블록 안에서 입
니다. 따라서 여러분이 함수 안의 특정 블록 안에서만 변수를 정의했다면 그 변
수는 그 블록에서만 유효합니다. [리스트 5.4]가 이 개념을 잘 보여줍니다.

[리스트 5.4] 블록 안에서의 범위 규칙

1: // [리스트 5.47] 블록 안에서의 범위 규칙
ae ff
3
4: #include <iostream.h>
_ 38
6: void myFunc();
C3
8: int main)
o: £
10:   int xX = 5;
41:   cout << "\nIn main x is: " << x;
12:
15:   myFunc();
14:
15:   cout << "\nBack in main, x is: " << x;



===== PAGE 122 =====
16%   return 0;

1 가

18:

19: void myFunc()

205

21%

22%    int x = 8;

25:    cout << "\nIn myFunc, local x: " << x;

24:

255   ne

26:      cout << "\nIn block in myFunc, x is: " << x;
201

28:      int x =9;

29:

50:      cout << "\nVery local x: " << x;

31¢   }

325

6161   cout << "\nOut of block, in myFunc, x: " << x;
342 }

결과  In main x is 5

In myFunc, local x: 8

In block in myFunc, x is: 8
Very local x: 9
Out of block, in myFunc, x: 8

Back in main, x is 5

myFunc()7} 불려졌고, 역시 xe} 이름지어진 또 다른 지역 변수가 22번 줄에서 8

로 초기화되었습니다. 이 RE 23번 줄에서 출력되었습니다.
블록 하나가 25번 줄에서 시작하고 26번 줄에서 함수의 변수 x7} 다시 출력되었
습니다. *라 이름지어진 새로운 변수가 블록 안 28번 SoA 생겨났고 9로 초기
화되었습니다. 이 새로운 값은 30번 줄에서 출력이 됩니다. 블록은 31번 줄에서
끝나고 28번 줄에서 생성된 변수는 범위 규칙을 벗어나게 되며 더 이상 유효하지
않습니다.

x7} 33번 줄에서 출력되었을 때 이는 22번 줄에서 선언된 ×입니다. 이 x9] We
28번 줄에서 정의된 *와 관계가 없습니다. 그 값은 여전히 8입니다.


===== PAGE 123 =====
120 ee AIF

34번 줄에서 myFunc= 범위 FAS 벗어나게 되고 그 지역 변수 xe 소용

됩니다. AVS 15번 줄로 돌아오게 되고 지역 변수 x dod 줄에서 생성된

력됩니다. 이 값 역시 0080000에서 BIR 값에 의해 어떠한 영향도 받지 않
니다.
이

나도 없습니다.

S}A (Function Statement)

없게
)가 &

=

로그램에서 보면 3개의 변수가 같은 이름을 가졌지만 그리 혼동될 것은 하

함수의 Zao] 들어갈 문장의 형태나 개수에는 제한이 없습니다. 여러분은 함수
안에 다른 eS 정의할 수는 없지만, 다른 함수는 부를 수 있고, 대부분의 CH
프로그램에서는 mainQo] 이 일을 도맡아 합니다. 함수는 자기 자신을 부를 수도
있고, 이는 자기 호출 부분에서 설명됩니다.

0++에서 함수의 크기에는 제한이 없지만 잘 설계된 함수는 작아지는 경향이 있
습니다. 많은 프로그래머들은, 함수는 여러분의 화면 하나에 다 들어갈 정도로 작

게 만들어 한번에 전체 함수를 다 볼 수 있게 하자라고 합니다.
Bo] 의한 법칙이지만, 때때로 매우 훌륭한 프로그래머가 이 WAS

커지면 분리할 만한 곳을 찾아야 힙니다

함수 인자(『40어00 Argument)

Hu
oe

함수의 매개 변수    수를 사용하는 함수
어떤 값을 반환하는 함수를 매
버그가 어렵습니다.

도 A 하지만 작은 프로그램이|역시 이해하기 쉽고 유지 보수가 쉽습니다.

단 하나의, 이해하기 쉬운 업무를 수행해야 합니다. 여러분의 함수가

깨기

함수의 인자는 모두 같은 형일 필요는 없습니다. 여러 개의 정수형과 1006, 문자
형을 가진 함수가 당연히 있을 수 있습니다. 상수, 수학적 또는 논리적 수식들,
심지어 BS 반환하는 함수 등 어떠한 CH 수식도 인자가 될 수 있습니다

개 변수로 써도 BAS 없지만, 읽기가 힘들고 디



===== PAGE 124 =====
제5일 함수 ㅇㅇ 121

보기로 0040160, triple(), square(), 00060라는 함수들을 쓸 수 있는데 각각

ae 갖습니다.

Answer = (double (triple (square (cube (myValue))))) 3

반환

ro

이 문장은 변수 myValueS 가지는데 o|S cubeQ@H= 함수의 매개 변수로 전달하
al, HE 00000의 반환값은 함수 50408060로 전달되며, 940060의 반환값은 다시
triple] 매개 변수로 들어가고, triples] 반환값은 마지막으로 000060의 매개

수로 전달됩니다. 이 함수의 반환값이 마지막으로 40600에 전달됩니다.

이 코드가 정확히 무엇을 하는지 확신하기 어렵습니다. 장애가 발생하면 어디에
서 발생했는지 도대체 알 길이 없습니다. 만일 장애가 나면 각 과정을 중간 단계
로 나누는 방법밖에 없습니다.

unsigned long myVaLlue = 2 ;

unsigned long cubed = cube(myValue) ; // cubed = 83

unsigned Long squared = square(cubed) ; // squared = 64;

unsigned long tripled = triple(squared) 7// tripled = 196 ;
unsigned Long Answer = double(tripled) ; // Answer = 5925

고, 수행의 순서가 명확해집니다.

Ad

각 중간 과정이 검사될 수 있

함수로 전달된 매개 변수는 그 함수에 있어 지역적입니다. 그 인자에 가해진 변
버 미치지 않습니다. 이것은 ‘gt 전달 방식(685908 by

A 함수에서 전달 인자의 지역적 복사가 이루어진다는
것을 의미합니다. 이 ane  복사는 지역 변수처럼 취급됩니다. [리스트 5.5]는 이
점을 보여줍니다.

[리스트 5.5] '값 전달 방식'의 예

1: // [리스트 5.5] ‘Bt Met 방식"의 of
2:
#include <iostream.h>

void swap(int x, int y);

int main()
£

3
4
5:
6:
Vs
8
9     int x =5, y= 10;
1

0:


===== PAGE 125 =====
122 ee MIF

113   cout << "Main. Before swap, x: "<<x<< "yi" <<y << evn" 3
12:   swap(x,y);

13:   cout << "Main. After swap, x: "<< x << "y: "<< y << "\n";
14:   return 0;

152 2

16:

17: void swap (int x, int y)

(Se 4

19:   int temp;

20:

21:   cout << "Swap. Before swap, x: "<< x << "yi" <<y << "VAS
22:

25:   temp = x;

24:   x = 3;
25:   y = temp;
26:

ere   cout << "Swap. After swap, x: "<<x<< "yi" <<y << ONG 오

295 7

겔과 Main. Before swap. x: 5 y: 10

Swap. Before swap. x: 5 y: 10
Swap. After swap. x: 10 y: 5
Main. After swap. x: 5 y: 10

분석  이 프로그램은 0800에서 두 개의 변수를 초기화 한 뒤 swap) 함수로 hs

전달하는데 두 개의 값을 바꾸는 듯 보입니다. 그 두 개의 RS 20800에서
다시 살펴보면, Oh my god! 그들은 변함이 없습니다.

변수들은 9번 줄에서 초기화가 되었고, 11번 줄에서 그 값이 나열되었습니다.
swap] 호출되었고 변수가 전달됩니다.

AYA] swap) 함수로 가고 21번 줄에서 HS] 다시 출력됩니다. 그 RSE
main) 2] 값과 다를 바가 없습니다. 23번부터 25번 줄까지 값들은 바뀌어지고
이 YES WA 줄에서 확인이 됩니다. swap) 함수 안에서 WSS 틀림없이 바뀌
었습니다.

실행이 다시 13번 줄로 돌아오고 min) 함수로 다시 돌아왔습니다. 그런데 거기
에서 값들은 whFo] 없습니다. 짐작하였듯이 swap) 함수로 전달된 값은 값으로만
전달되었고, 이는 90800에서 지역적인 값들로 전달값이 복사되었다는 의미입니
다. 23번 Sz} 25번 So] 거쳐서 이 값들은 교환되었지만 mains] 값에는 영향을
끼치지 못하였습니다.



===== PAGE 126 =====
제5일 함수 ee 123

80
>
we
x
{a
rr
× we
요
ave
Ac
rlo
a
eu
ag.
ox,
“i>
가
aut
ath
ne
ey
eu
ug
rau
aN
2
호
고
val

에
+
o Cr
a
lo
[푸
rol
Dit
»
호
호.
oa.
uf
[푸
rok
194
ae
a
대
fan
aU
다니
기
ne
SH
오
=
2
-1ㅁ
be
re
re

return 5;
return (x > 5) ;
return (MyFunction()) ;

함수 MyFunction)o] 어떤 값을 반환하기만 한다면 위의 문장들은 모두 맞는 표현

입니다. 둘째 문장의 70470 (x > 5)은 만약 x7} SHU} 크지 않으면 Oo] 되고, 크면
10] 됩니다. 앞에서 배운바 있지만 반환값은 x7} 아니라 그 수식의 값(참이면 1,

거짓이면 0)이 반환됩니다.

:0000이라는 예약어를 만나면 00000 다음에 오는 수식이 그 함수의 반환값으로
되돌려집니다. 프로그램 실행은 호출한 함수로 즉시 되돌려지고, 6000 다음에 있
는 문장들은 실행되지 않습니다.

하나의 함수에서 복수개의 0000 BAS 갖는 것도 가능합니다. [리스트 5.6|이 이

예를 보여줍니다.

[리스트 5.6] 복수의 retun 문장을 갖는 함수

1: // [리스트 5.67 복수의 return BAS 갖는 함수
28 //

33

4: #include <iostream.h>

5

6: int Doubler(int AmountToDouble) ;
ts

8: int main()

os 고

10:

VTS   int result = 0;

123   int input;


===== PAGE 127 =====
124 ee 제1주

13:

14:    cout << "Enter a number between O and 10,000 to double: ";
15%   cin >> input;

165

17:    cout << "\nBefore doubler is called... ";
18:   cout << "\ninput: " << input << " doubled: " << result << “\n";

195

20:   result = Doubler (input) ;

21:

22:   cout << "\nBack from Doubler...;"

23:   cout << "\ninput: " << input << " doubled: " << result << "\n";
24:                                                     ：
25%

26:   return 0;

acs }

28:

29: int Doubler(int original)

SO: £

312   if (original <= 10000)

52:      return original * 2;

33;   else

34:      return -1;

555   cout << "You can't get here!\n";

56: 2

결과  Enter a number between 0 and 10,000 to double: 9000

Before double is called...
input: 9000 doubled: 0

Back from doubler...
input: 9000 doubled: 18000
Enter a number between 0 and 10,000 to double: 11000

Before doubler is called...
input: 11000 doubled: 0

Back from doubler...
input: 11000 doubled: -1

14번과 15번 줄에서 숫자를 요구하고 18번 줄에서 지역 We result} 함께
출력이 됩니다. 함수 2008160가 20번 SA 호출되고 입력값이 매개 변수

00
4



===== PAGE 128 =====
제5일 함수 ee 125

23

rE,
ny

acy

달됩니다. 결과는 지역 변수 resulto} 대입이 되고 그 값은 22번         에
권

31번 줄의 함수 2000180에서 매7

4
약 작은 수이면 함수는 인자에 26

rl
=e
ro

ag

지

EL

수는 10,000보다
하여 반환하고 그

변
곱

됩니다. 만
시

류의

a
때 프
bo

1 으

떠

습니다. 왜냐하면 값이 10,000보다 크건 작건
2번 줄이나 34번 줄에서 반환되기 때문입니다.
행될 수 없다고 주의를 줄 것이고, 이때 좋은

^
기본 매개 HiA(Default Parameter)

함수 원형에서 혹은 함수 정의에서 선언한 모든 변수에 대해, 호출 함수는 값을
전달해야 합니다. 전달되는 Re 선언된 형과 같아야 합니다. 함수를 다음과 같이
선언했다면

long myFunction(int) ;

수형 변수를 취해야 합니다. 만일, 함수의 정의가 다르거나 여러분이
정수형을 전달 안하면 컴파일러 장애가 날 것입니다.
이 법칙의 하나의 예외는 함수 원형에서 매개 변수로 기본값을 사용했을 때입니
다. 기본값이란 아무런 값이 주어지지 않을 때 사용되는 값입니다. 위의 함수는
다음과 같이 다시 쓰일 수 있습니다.

long myFunction (int x = 50) ;

1 ~

그 dee 4

이 원형은 ‘myFunction)-S 1008형을 반환하고, 정수형 매개 변수를 가진다.
인수가 없다면 기본값으로 50을 사용한다.”라는 의미입니다. 함수

개 변수의 이름은 불필요하므로 이 선언은 타음과 같이 다시 쓰일
Long myFunction (int = 50) ;

함수 정의는 기본 매개 ASS 썼다고 하여 달라질 것이 없습니다. 함수 정의부
분에 가서 이 함수의 떠리 부분은 다음과 같습니다

long myFunction (101 x)


===== PAGE 129 =====
126 ㅇㅇ AI

출 247 매개 변수를 포함하지 않는다면, adele wl 기본값 50을 채우
을 것입니다. 함수 UB} 매개 변수명은 함수의 머리부분에서의 이름과 달라
무방합니다. 기본값은 그 위치에 (의해 할당되는 것이지 이름가지고 할당되는
것이 아닙니다.

함수의 그 어떠한 매개 변수도 기본값을 할당받을 수 있습니다. 단 하나의 제한
조건은 이렇습니다. 만약 어떤 매개 변수가 기본값을 갖지 않는다면, 그 앞의 매
개 변수들은 기본값을 가질 수 없습니다.

만약 함수 원형이 다음과 같다면

long myFunction (int Param1 , int Param2 , int Param3) ;

i of fol

여기에서 Param3el 기본값이 있어야만 Param27} 기본값을 가질 수 있고, 또
000001이 기본값을 가지려면 Param29} Param3-2- 모두 기본값을 가져야만 합니다.
[리스트 SS 기본값의 예를 보여줍니다.

[리스트 5.7] 매개 변수의 기본값 갖기

1: // [리스트 5.77 매개 변수의 기본값 갖기

25 Lf

6

4: #include <iostream.h>

a5

6: int AreaCube(int Length, int width = 25, int height = 1);
ca

8: int mainQ

oF <<

10:   int length = 100;
V1:    int width = 50;
12:   int height = 2;
133   int area;

14:

19   area = AreaCube(length, width, height);

16%   cout << "First area equals: " << area << "\n";

7s

18:   area = AreaCube(length, width);

19%   cout << "Second time area equals: " << area << "\n";
20:

21%   area = AreaCube(length);
22:   cout << "Third time area equals: " << area << "\n";
235%   return 0;



===== PAGE 130 =====
제5일 함수 ee 127

26: AreaCube(int length, int width, int height)

2re <

28:

29:    return (length * width * height);
350: }

결과  First area equals: 10000

Second time area equals: 5000

Third time area equals: 2500

분석 6번 줄에서 AreaCube() 함수 원형은 476800660 함수가 3개의 정수형 매개

"WS 갖는다고 하였습니다. 뒤의 WHE 기본값을 갖습니다.
이 함수는 육면체의 체적을 구하는 함수인데, 각각의 길이가 매개 변수로 전달됩
니다. 만약 깊이가 전달되지 않으면 깊이는 25이고 높이는 1입니다. 만약, 높이만
값이 지정되지 않는다면 높이는 기본값이 1입니다. 깊이를 전달하지 않은 a =

10 -12번 줄에서 길이와 높이, 깊이가 초기화되었습니다. 15번 줄에서 그 값들이
AreaCube) 함수에게 전달됩니다. 값들이 계산되고 결과는 16번 Soy 출력됩니다.
실행은 또 18번 줄로 넘어갑니다. 여기서 사6600660가 다시 호출되는데 높이값이
지정이 안됩니다. 기본값이 사용되고 값들이 계산되고 또 출력이 됩니다.

AVS 21번 줄로 넘어가고 이번에는 깊이와 높이 둘 다 전달이 안됩니다. 실행
세 번째로 27번 줄로'넘어가고 기본값이 사용되며, 체적은 계산되고 또 출력

1 변
00407 두 번째 이하의 마기 번수가 기본같이 없을 떠 첫 번째 매개 변수에 기본값
을 사용하지 맘시다
DONT 인자로 전달된 갔은 SS 함수에서의 갔에 PHS 못 미친다는 것을 잊지
맡시다

DONT 전역 변수가 하나의 함수에서 바뀌면 다른 함수 전체에 영향을 미칩니다. 잊
지 avis,



===== PAGE 131 =====
128 ee 제1주

“알수

응어

새로운 함수 다형성(『40아100 Sigel ge  함수 너가 함수 다형성이라고도 불립니
|란                많은 형

cha aed mee

> (Overloading 00040
CHIME 같은 이름을 가진 함수들을 중첩시켜 만들 수 있습니다. 이를 중첩 함
수라 부릅니다. 그 OSES 매개 변수 목록에서 다르거나 마개 Wz] 형에서
다르거나, 매개 변수의 개수가 다르거나 아니면 그런 것들이 혼합된 경우입니다.
보기가 있습니다.

int myFunction ( int , int ) ;

int myFunction ( long , long ) ;

int myFunction ( long ) ;
myFunction()-<- 세 가지의 다른 매개 변수 SSS 가지고 중첩되었습니     4
째와 두 번째는 매개 변수의 형에서 다르고, 세 번째 것은 매개 변수의 개수에서
차이가 납니다.

반환값은 중첩 함수들 사이에서 같거나 다를 수 있습니다. 만일 두 함수가 이름
도 같고 매개 변수도 같은데 반환형만 다르다면 컴파일러 오류를 발생시킬 것입
니다.

예를 들어, 여러분이 입력한 값의 두 배의 값을 구하는 함수를 생각해 봅시다.
여러분은 int, long, float, double 등 여러 개의 ge 전달할 수 있는 기능을 원할
것입니다. 만약 Sa 함수의 기능이 없다면 여러분은 4개의 BES 만들어야 합
니다.

int DoubleInt(int) ;

long Doublelong(long) ;

float DoubleFloat(float) ;
double DoubleDouble(double) ;

중첩 함수를 쓰면 다음과 같습니다.



===== PAGE 132 =====
제5일 함수 ee 129
int Double (int) ;
long Doubel (long) ;
float Double (float) ;
double Doubel (double) ;
이 중첩 함수가 WIE 쉽고 사용하기도 편합니다. 어떤 함수를 호출할까 고민할
이유가 하나도 없습니다. 변수만 전달해 주면 올바른 함수가 정확히 호출됩니다.

[리스트 5.8]이 이 중첩 함수의 예를 보여줍니다.

[리스트 5.8] 중첩 함수의 예

1: // [리스트 5.83 FH 함수의 예
2) ff

5

4: #include <iostream.h>
Die

6: int DoubleCint);

7: long Double(long);

8: float Double(float);
9: double Double(double) ;
10:

11: int main()

128 세

131   int myInt = 6500;

14:   long myLong = 65000;

15%   float myFloat = 6.5;

16:   double myDouble = 6.5e20;

17:

18:   int doubledint;

19   long doubledLong;

20:   float doubledFloat;

215   double doubledDouble;

22°

25%   cout << "myInt: " << myInt << "\n";

24:   cout << "myLong: " << myLong << "\n";

25%   cout << "myFloat: " << myFloat << "\n";
262   cout << "myDouble: " << myDouble << "\n";
Crs

28:   doubledInt = Double(myInt);

29%   doubledLong = Double(myLong) ;

30:   doubledFloat = Double(myFloat);

S12   doubledDouble = Doube(myDouble) ;

32:

329   cout << "doubledInt: " << doubledInt << "\n";
34:   cout << "doubledLong: " << doubledLong << "\n";


===== PAGE 133 =====
130 ee ANF

55:
36:
37:
$82
39?
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
513
52s
535:
54:
ape
56:
575
58:
59:
60:
61:
62:
63:

cout << "doubledFloat: " << doubledFloat << "\n";
cout << "doubledDouble: " << doubledDouble << "\n";

return 0;

int DoubleCint original)

Hi

cout << "In DoubleCint)\n";
return 2 * original;

}

Long Double(long original)

{

cout << "In Double(long)\n";
return 2 * original;

3

float Double(float original)
{

cout << "In Double(float)\n";
return 2 * original;

}

double Double(double original)
{

cout << "In Double(double)\n";
return 2 * original;

}

myInt: 6500

myLong: 65000
myFloat: 6.5
myDouble: 6.5e20

In Double (int)

In Double (long)

In Double (float)
In Double (double)
DoublediInt: 13000
DoubledLong: 130000
DoubledFloat: 13
DoubledDouble: 1.3e21



===== PAGE 134 =====
제5일 함수 ee 131

ge AY 200060 항수는 16. long, float, 00006로 중첩되었습니다. 원형은 6 - 9번 줄
에 있고 정의는 41 - 63번 줄에 있습니다.

main’) 함수의 몸체에서 8개의 지역 변수가 선언되었습니다. 13 - 16번 줄에서 4
개의 변수가 초기화되었고, 28 - 31번 줄에서는 처음 4 개의 변수를 200060 함
수에 전달한 뒤 반환받는 값으로 4 개의 값으로 할당되었습니다. Double 호출
한 후, 호출 함수는 어떤 함수를 호출할지 신경을 쓰지 않습니다. 그저 매개 변수
를 전달하면 해당되는 함수가 정확히 호출됩니다.

컴파일러는 인자들을 살펴보고 네게의 Double) 중첩 함수 중 어떤 AS 부를지
결정합니다. 결과에 의하면 여러분이 기대한 대로 4 개의 함수가 차례로 불려집
니다.

라수에 관한 특별한 주제들
함수들은 프로그래밍에 있어서 중심적인 것이기 때문에, 여러분이 어떤 |
문제에 부닥칠 때 아주 재미있는 이야기 거리가 생김니다. 잘만 쓰여진다
(inline) 함수는 수행성을 좋게 하여 줍니다. 자기 호출 함수는 놀라운 비법이
긴 프로그래밍 기법인데, 아주 가끔 쓰이긴 하지만, 아주 어려운 문제를 감쪽같이
해결하는 능력이 있습니다.

of Aer 찌

AH inline) 함수  cn  관로 >

함수를 정의할 때, 보통 컴파일러는 일련의 명령어들을 메모리에 만들

다. Feo] 함수를 호출할      은

환되면 Ade 호출한 직전 함수의 다음 줄로 넘어갑니다. 함수를 10
프로그램은 그때마다 이 명령어 집합을 10번 실행해야 합니다. 즉, 이
사본이 10개 있는 것이 아니라 단 한 개의 함수 복사본이 있습니다.
함수로 WS 왔다갔다하는 것은 상당한 지출을 수반합니다. 함수들은 대부

장으로 이루어졌습니다 -

ch
ie +
ou

re,
ㅇㅇ

령으       면 프로그램 수행성에 적절한
률을 이야기할 때, 보통 속도를 이야기하는



===== PAGE 135 =====
132 ee 제1주

u
얻었다는 얘기는 들은 적이 없습니다. 더욱 중요한
로 수행성을 약화시킨

[리스트 5.9] 확장 함

상당한 비용을 수반할 때가 있습니다. 함수가 10번 불린다면
프로그램에 각 10번이 복사됩니다. 속도에 있어서의 조그만 개
실행 파일의 팽창이라는 대가를 치를 수가 있습니다. 그런데 요즈음에는
상일 수도 (있습니다. 오늘날, 사실 최적화된 컴파일러가
를 사용하여 아주 큰 소득을

어난 크기는 그 자제

iH

I>
Ke)
2

1
2
3
bs
5:
6
7
8

9:

10:
415
128
13:
14:
15:
16:
103
18:
19%
20:
21:
22:
23:
24:
25:
26:

// 예제 5.9 확장 함수의 예
#include <iostream.h>
inline int Double(int);

int main®
+
int target;

cout << "Enter a number to work with: ";
cin >> target;
cout << "\n";

target = Double(target);
cout << "Target: " << target << endl;

target = Double(target) ;
cout << "Target: " << target << endl;

target = Double(target);
cout << "Target: " << target << endl;
return 0;



===== PAGE 136 =====
27: int Double(int target)

28: £
29: return 2*target;
50: }

결과  Enter a number to work with: 20

Target: 40

Target: 80

Target: 160
EMA SH S Double) int 매개 AES 취하고 i= 반환값으로 하는 확장 함수
= =

입니다. 이 AVS 다른 함수의 원형과 똑같지만 10106라는 예약어가 함수
의 반환형 앞에 놓여 있습니다.

target = Double(target);

이 부분은 다음과 같이 다시 써넣습니다.

target = 2 * target ;

여러분이 프로그램을 실행하기 전까지 명령어들은 바뀌어져 있고, .081 파일 ot
에 컴파일 되어져 있습니다. 이것이 왕복달리기를 줄여주고, 대신 크기를 증가시
킴니다.

inline Ht

자기 *2(Recursion)

함수는 자기 자신을 부를 수 있습니다. 이를 자기 SF Recursion)o]z} 부릅니다.
버버  이 호출은 직접 호출과 간접 호출로 UMUC. 함수가 자기 자신을 부를

]를 = AR 후졸(0060 recursion)°]¢}31 하고, 함수가 다른 Ae ee 고 부른 은 우 그
ne 내 Ses 호출할 때 이를 간접 0 1900000)이가 합나 합니다.

어떤 문제들은 자기 SSS 써서 매우 쉽게 풀리는데, 보통 어떤 자료에 aes
가하고 그 결과물에 대해 같은 ASS 가해야 하는 경우입니다. 직접 호출이건 간

:


===== PAGE 137 =====
134 ee MIF

접 호출이건 두 가지의 종류가 있습니다. 궁극에 가서는 종료가 되어 답을 주는
경우이고, 다른 하나는 끝나지 않고 실행이 실패되는 경우입니다. 프로그래머들은
프로그래머가 이러한 일을 할 때) 비웃지만 자주 이러한 ASS 범합니다.

함수가 자신을 호출할 땐, 그 함수의 새로운 복사본이 만들어진다는 사실을 아
것이 매우 중요합니다. 복사된 함수의 지역 변수들은 처음 함수의 지역 변수들과
는 무관하고 서로에게 영향을 미치지 않습니다. 마치 [리스트 5.4]의 maine} 지
역 변수들이, mind 안에서 호출한 함수의 지역 WES 바꾸지 않는 것과 마찬가
입니다.

자기 호출을 사용하여 문제를 푸는 예로 피보나치 수열을 생각해 봅시다.

1, 1. 2. 3, 5, Bp 13... 212 38

Zt 숫자는, 두 번째 이후는 앞의 두 수의 합입니다. 피보나치 문제는 이 수열에서
21번째의 숫자는 무엇인가 하는 것입니다.
이 BAS 푸는 한 가지 WHS 이 수열을 열심히 분석하는 것입니다. 처음
ME 1입니다. 각각의 HE 앞의 두수의 합이므로 THA 수는 5번째와 6번째
의 합입니다. 일반적으로 풀이하여 0번째의 수는0이 2보다 크다는 가정 하에)
- 1 번째 수와 2 - 2 번째의 수의 합입니다.
자기 호출 BRE 정지해야 하는 BHO] 있어야 합니다. 프로그램을 종료시키는
무엇인가가 일어나야지 그렇지 않으면 끝까지 돌아갑니다. 피보나치 수열에서는
no] 3보다 작을 때가 정지조건이 됩니다.
여기서 사용되는 알고리즘은 다음과 같습니다.
사용자에게 이 수열에서의 위치를 물어봅니다.
2. 이 위치에서 fib() 함수를 호출하는데, 사용자가 입력한 RS 전달합니다.
AO

3. 116() SPE 인자 nS 조사합니다. nol 3보다 HOM 1을 반환합니다. 아닌 경우는
116()는 AVIS 호출하며 n - 2를 전달하고, 다시 러버 또  또 자신을 호출하는데 이번에는
0 -1을 전달합니다. 그리고 그 합을 반환합니다.

{ej

rir

24,

.@

s oy cn

만일 806(1)을 호출하면 10] 반환   ae  fib2sS 부르면, 1S meee
fib3)S 부르면 800)과 80(2)의  강의 합을 반환합니다. 860)과 80(2)는 각각
반환하기 때문에 86(3)은 2를 반환합니다.

fib(4)= 호출하면 66(2)와 fib3)2] YS 반환하는데 80(3)은 2를 반환하고010(01)과
fib(2)2- 1의 합을 반환하므로) fib 12 반환하므로, 80(4)는 이들의 합 4를 반
환합니다. 그런데 86(4)는 수열에서 4번째의 수입니다.



===== PAGE 138 =====
한번 더 생각하여 8065)를 호출하면 80(3)와 fib] 합을 반환하는데 각각은 2와
4이므로 그 합은 6이 됩니다.

사실 이 Yo] 가장 효율적인 방법은 of I Yr}. ib) 계산하기 위해서는 860
함수가 무려 13.529번씩이나 호출됩니다.) 게다가 실행조차 되지 않습니다. 주의해
야 할 것은 여러분이 너무나도 큰 숫자를 입력하면, 프로그램은 메모리가 모자란
다고 할 것입니다. 매번 800가 SSA 때마다 메모리가 할당됩니다. 반환되면 메
모리가 방출됩니다. 자기 호출에서는 메모리가 방출될 때까지 계속 메모리가 할
당되고, 시스템은 메모리를 계속 잡아먹습니다. [리스트 5.10|은 fo IES 구현
하였습니다.
ee. es
[리스트 5.10]을 실행할 떼 !5보다 작은 수를 사용하도록 합시다. 왜냐하면 자기 eS
을 사용하는데 이는 엄청난 메모리를 잡아먹기 떼문입니다.

[리스트 5.10] 피보나치 수열을 사응한 자기 호출

// [리스트 5.107 피보나치 수열을 사용한 자기 SB

//

// nl Febonacci 숫자를 찾음

// 사용되는 알고리즘: fib(n) = fib(n-1) + fib(n-2)
// BRE 조건: ㅁ=2 || ㅁ=1

#include <iostream.h>

CONBDU FWD =
×… ㅁㅁ 00 00 ㅁㅁ 00 00 000

xo

int fibCint n);

10:

11: int main()

12: ¢

13:

145   int n, answer;

150   cout << "Enter number to find: ";
16:   cin >> n;

171
18:   cout << "\n\n";
19:
20:   answer = fib(n);
211

22:   cout << answer <<" is the " << n << "th Fibonacci number\n";
25%   return 0;
245 3


===== PAGE 139 =====
136 ce 제1주

208                                                =
26: int fib (int n)

2s &

283    cout << "Processing fib(" <<n <<")... "7
29:

50:    if Cn 3)

Svs   {

322      cout << "Return 1!\n";

55:      return (1);

54:   가

35:   else

36:   {

37%      cout << "Call fib(" << n-2 <<") and fib(" << n-1 << ").An";
38:      return( fib(n-2) + fib (n-1));

39:   >

40: }

결과  Enter number to find: 5

Processing fib(5)... Call fib(3) and fib(4).
Processing fib(3)... Call fib(1) and fib(2).
Processing fib(1)... Return 1!
Processing fib(2)... Return 1!
Processing fib(4)... Call fib(2) and fib(3).
Processing fib(2)... Return 1!
Processing fib(3)... Call fib(1) and fib(2).
Processing fib(1)... Return 1!
Processing fib(2)... Return 1!
5 is the 5th Fibonacci number.

AH 58 중에서 찾아야 할 수를 입력받아 [이라는 변수에 대입함니다. 다음 ㅁ
을 가지고 함수 800를 부릅니다. 실행은 800 함수로 분기됩니다. 이는 28

번 줄에 있는데 그 인자를 출력합니다.

30번 줄에서 인자 no} 1인지 2인지가 검사됩니다. 그렇다면 Ado 1을 반환됩니
다. 그렇지 않으면 AOE n29 nS 전달한 850 함수의 반환값의 합을 반환합
니다.

예에서 은 5였고 따라서 0800에서는 fibG)S 부릅니다. 실행은 860함수로 분기
되고 30번 줄에서 oe 작은지 검사됩니다. 검사는 실패되고 따라서 10(5)는
fib(3) 9} 860)의 합을 반환합니다. 060는 n2 (5 - 2 = 3)를 인자로 한 HF wl (5
- 1 = 4)를 le 한 값으로 하여 호출됩니다. 80(4)는 3을 반환하고 06(3)은 2를

반환하므로 값은 5가 됩니다.

(a



===== PAGE 140 =====
i

식으로 하여 6까지 입력하여 보고 결과를 주의 깊          한
20을 입력하여 봅시다. 메모리가 충분하다면 아마 굉장한 볼거리를 asa 것입
니다.

자기 SSL 프로그래밍에 있어서 아주 재치 있는 부분입니다. 여기서는 그 작동되는
근본 원리를 이해하는 것이 유익할 것 같아 제공하였는데, 만일 여러분이 그 자세한
부분을 모른다고 해도 너무 걱정할 필요는 없습니다.

Ts
ri
오
ra
=!
애
Ja
때
iS

함수를 호출하면 불려진 함수로 분기하고, 매개 변수는 전달되며, 함수의 몸체가
실행됩니다. 함수가 끝나면 그 함수가 100형으로 되어 있지 않는 한 값을 반환하
고 제어는 호출 함수로 돌려집니다

어떻게 이런 일이 수행될까요? 어떻게 코드에서 어디로 분기할지를 압니까? 변수
들이 전달될 때 변수들은 어디에 저장될까요? 함수의 몸체에서 변수가 선언되면
변수들에겐 어떤 일이 일어날까요? 반환값은 어떻게 되돌려질까요? 코드는 자기
가 되돌아갈 자리를 어떻게 알고 있을까요?

대부분의 입문서들은 이에 대한 답을 주지 않습니다. 하지만 이 부분을 모르면
프로그램은 여러분에게 알 수 없는 수수께끼가 될 뿐입니다. 이 설명은 컴퓨터
메모리에 대한 간략한 접근을 요구합니다

주상화 단계(66015 of Abstraction)
새로운 프로그래머가 항상 싸우는 주요한 장벽 중 하나는 수많은 추상화의 단
입니다. 컴퓨터는 물론 전기기계입니다. 컴퓨터는 메뉴나 윈도         릅
프로그램이나 명령에 대해 모르고 1과 0들에 대해서도 ws          행
것은 집적 회로의 여러 곳에서 측정되는 전압입니다. 이것조차 또한 추상입
전기 그 자체는 두뇌 속의 개념이고, 전자의 흐름을 표현한 것입니다.

무모


===== PAGE 141 =====
138 ee 제1주

RAM 안에 갖는 값들 뒤에 숨겨진 각각의 자세한 WAS 고민하는 프로그래머는
거의 없습니다. WE 여러분은 물리학의 자세한 WAS 모르고도 차를 잘 몰
수 있고, 라면을 끊일 수 있으며, 야구도 하고, 또 프로그램을 하기 위해 컴퓨터
의 자세한 전기역할을 이해하지 않아도 됩니다.

하지만 여러분은 메모리가 어떻게 구성되어 있는지는 알아야 합니다. 변수가 어
디에 저장되고, 언제 생성되며, 어떻게 값들이 함수로 전달되는지를 수월하게 머
리 속에서 상상할 수 없다면 프로그램을 하는 것이 그야말로 미로에 빠지게 되는
것입니다.

RAM 나누기
여러분이 프로그램을 시작할 때 ae 운영지제(008 측은 까이크로소프트 윈

는 중앙 연산 장치(0) 안에 자리잡은 특별한 메모리의 영역입니다. 레

내부 집안 일을 다 도맡아|합니다. 레지스ㄷ

를 벗어납니다. 그러나 우리가 관심을 가지는 부분은, 항상 다음 부분의 코드를

갓리키는 임무를 수행하는 레지스터들입니다. Fae 이러한 레지스터의 ate
ae   ~ 고저         .    a   a      =e

명령 ,포인터라고 호칭합니다. 명령 포인터의 역할은 다음에 실행될 코드를 가리

코드 그 자체는 코드 영역에 있는데, 이는 메모리의 일부분에 여러분이 프로그램
에서 만든 명령들을 이진형태로 저장하기 위해 따로 만들어 놓은 장소입니다. 원
시 코드의 각 Se 일련의 명령어들로 변환되는데 이 각각의 명령은 메모리의 특
정 주소에 있습니다. 명령 포인터는 다음에 실행될 명령의 주소를 가지고 있습니
다. [그림 sat 이 개념을 설명합니다.



===== PAGE 142 =====
제5일 함수 ㅇㅇ 139

[그림 5.4]                코드 영역
명령 포인터

100 Int x=5;

102           명령포인터
101 Int y=7;

102 Cout << x;    <I

103 Func (x,y);

104 y=9;
105 return;

Gg 영러분의 프로그램에서 각 함수에 의해 필요로 되는 자료들을 보관하기

위해 할당된 메모리의 특수한 영역입니다. 이것이 스택이라 불리는 이유는 마지
막에 들어간 것이 처음에 U7H=(Last-in first-out), 마치 [그림 5.5]에서처럼 카페테
리아의 접시꾸러미(영어로 하면 스택이 됩니다.)를 닮았기 때문입니다.

Last-in first-out-> 마지막에 스택에 쌓이는 것이 빼어낼 때는 처음에 꺼내지기 때

문에 붙여진 것입니다. owe] Ge 마치.극장에 입장하기 위해 늘어선 줄고
같습니다. 처음에 선 사람이 처음에 늘언가다 스택은 차곡차곡 쌓아놓은 동전
과 같습니다. 마지막 위에 올려놓은 동전이 A 번째로 꺼내집니다.

자료가 스택에 저장되었을 때(09060) 스택은 증가합니다. 자료들이 스택으로부터
빠져나갈 (popped) 스택은 감소합니다. 나중에 저장된 자료들을 먼저 빼내지 않
고 처음에 저장된 자료들을 빼내는 방법은 없습니다.

[그림 5.5]
스택

접시꾸러미는 일반적인 예입니다. 어떤 의미에서는 좋은 비유가 되지만 근본적으
로 생각하면 다릅니다. 좀더 정확한 그림은 바닥에서 꼭대기까지 줄서 있는 사각
방의 연속이라 생각하면 됩니다.


===== PAGE 143 =====
140 ee ANA

각 사각 방은 연결되는 주소가 있습니다. 그리고 그 사각 방 중 하나의 주소가
스택 포인터 역할을 하는 레지스터에|있습니다. 스택 포인터가 지칭한 스택 꼭대
기에 있는 주소보다 아래에 있는 방들은, 스택에 쌓여있는 부분입니다. 스택 꼭대
기보다 위에 있는 BRS 스택에서 빠져나간 부분입니다. [그림 5.6|이 이 개념을
설명합니다
[그림 5.6]                        스택
스택 포인터                         Re
100          스택포인터
theVariable    80    101   스택에서 빠짐
102 JQ           -
MyAge    50    103
104
105
YourAge '      37       106       스택상에 있음

107

108

109

110
자료가 스택에 저장될 때 그 자료는 스택 포인터가 가리키는 바로 위의 방에 위
치하게 되고 스택 포인터는 하나 증가합니다. 자료가 스택으로부터 빠져 나올 때
에는 실제 일어나는 일은 ms Eat 가리키는 주소만 하나 감소될 뿐입니다.

[그림 5.7]                       …
스택 포인터를 옮김                                 스택포인터
대                                               100
theVariable                   80                    101
102
MyAge       50        103
104       스택에서 빠짐
105
YourAge       37        106
107
108 <
109
스택상에 있음
110



===== PAGE 144 =====
제5일 함수 ee 141

스택과 함수
DOS 기반 하의 PCO 수행되는 프로그램이 함수로 분기될 때 일어나는 과정이
아래에 있습니다.

1. 명령포인터에 있는 FA 다음 주소가 함수 호출 후 다음의 명령 주소인데 그 증가된
주소가 스택에 저장이 됩니다. 이는 함수 호출이 끝난 뒤 되돌아오는 주소입니다

2 스택 위에 방이 하나 만들어지는데 여러분이 선언한 반환형이 저장되는 곳입니다. 2 바
이트 정수형을 지원하는 시스템에서는 반환형이 정수형으로 선언되었다면 2 바이트가
스택에 추가로 올려집니다. 하지만 현재까지는 아직 값이 저장되지 않습니다.

$ 호출된 함수의 주소(이는 이러한 함수들을 위해 특별히 마련된 일련의 메모리의 주소입
니다.)가 명령포인터에 저장됩니다. 따라서 명령포인터에는 호출된 함수 안의 다음 실행
될 명령이 자리잡게 됩니다.

4.

택의 현재의 꼭대기가 특별히 표시가 되는데 그 꼭대기는 스택 프레임이라고 불리는
별한 포인터에 잡혀 있습니다. 지금부터 함수가 되돌려질 때까지 스택에 쌓이는 모든
은 그 함수에 대해 지역적이라 생각될 수 있는 것입니다.

Yim 1>

5. 함수의 인자들이 스택에 위치합니다.

6 명령어 포인터에 있는 명령어가 수행됩니다. 이는 함수의 처음 명령어입니다.

?, 지역 변수들은 정의가 될 때마다 스택에 쌓입니다.
함수가 반환될 준비가 끝나면 위의 2번 과정에서 할당된 방에 반환값이 저장됩니
다. 그리고 나서 함수가 끝나는 과정이 시작되는데 스택 프레임 포인터에 잡혀있
= _ NAS 모두 꺼내버립니다. 이것이 그 동안 쌓여있던 내용들을 가장 효과
적으로 없애버리는 방법입니다.
반환값이 스택에서 꺼내져 함수 호출 그 자체의 값에 할당됩니다. 그리고 위의 1
번 과정에서 저장된 스택의 값이 명령포인터로 저장됩니다. 프로그램은 함수 호

출 다음으로 즉시 복원되고 실행된 함수 값은 남아있습니다.

지금까지의 자세한 과정은 컴파일러에 따라 혹은 컴퓨터에 따라 달라질 수
만 기본 개념은 환경과 무관하게 유지됩니다. 일반적으로 여러분이 함수를

하면 반환값과 매개 변수가 스택에 쌓입니다. 함수의 한 주기 동안 지역 변
이 스택에 쌓입니다. 함수가 반환되면 이 PSS 모두 스택에서 제거됩니다.

내일 우리는 함수의 주기와 무관하게 유효해야 하는 자료들을 갖기 위해 사용되
는 메모리의 다른 부분들에 대해 살펴볼 것입니다.

+ " 29
ni ny 쓰


===== PAGE 145 =====
142 ㅇㅇ

제1주

요와

함
니

수는 함수 원형을 가지고 선언되

를 시작하였습니다. 함수란 사싶은 여러분이 매개 변수를 전
}고 반환값을 돌려받는 부프로그램입니다. 모든 C++ BEE 2ㅁ800에서 비롯
ㄷ 그르     이

는데 그 반환값, 함수명, 매개 변수형을 서술합
다. 함수는 때에 따라 1100으로 선언될 수 있습니다. 함수 원형은 하나 이상의

매개 변수에 대해 기본값을 선언할 수 있습니다.

함수 정의는 함수 원형의 반환값, 이름, 매개 변수목록과 일치해야 합니다. 함수
는 매개 변수의 형이나 개수를 바꿈으로써 중첩될 수 있습니다. 컴파일러가 인자
목록을 보고 필요한 함수를 찾습니다.

함수의 지역 변수들, 또 함수에 전달된 매개 변수들은 그들이 선언된 구역에서
지역적입니다. 값으로 전달된 매개 변수들은 복사되고 호출한 함수에서의 gel
영향을 안 미칩니다

Q 왜 모든 변수를 전역 변수로 만들지 않습니까?

A 전역 변수를 써야한다라고 생각되던 때가 있었습니다. 프로그램이 점차 복잡해짐에
따라 자료들이 다른 함수들에 의해 변형되므로 프로그램에서 버그를 잡아내기가 힘
들어졌습니다. 전역 변수는 프로그램의 어떤 곳에서도 wl 수가 있습니다. 오랫동
안의 경험 끝에 프로그래머들은 자료란 지역적으로 보존되어야 한다는 것을 확신하

게 되었습니다. 그리고 그 값을 바꾸는 것은 매우 제한되어야 한다라고 생각되었습
니다.

함수 원형에서 언제 예약어 inlineO| 쓰입니까?

함수가 매우 작아 한두 So] 끝날 때, 또 프로그램의 여러 곳에서 불려지지 않을
때 inline] 자격이 있습니다.

인자값이 바뀌어도 호출 함수의 변수값에 영향을 of 미치는 이유는?

함수에 의해 전달되는 인자는 값 전달 방식입니다. 이는 함수에서의 인자가 원래
29] BABE 것입니다. 이 개넘은 연구 다음에 나오는 심화학습 부분에서 깊
이 다룰 것입니다.

 인자들이 값들로 전달된다면, 내가 변환시킨 AS 호출 함수에서도 변화되게 하려면 무
히

> =

ge



===== PAGE 146 =====
A 8일째 포인터에서 논의됩니다. 포인터를 쓰면 이 Bay} 해결됩니다. 물론 반환값을
사용하여 하나의 변화된 값만을 되돌릴 수도 있습니다.

Q 다음 두 개의 함수에서 어떤 일이 발생합니까?

int AreaCint width, int Length=1);
int Area(int size);

이 함수들은 중첩된 것입니까? 매개 변수의 개수가 다르지만 첫 번째 함수는 기본값을

Ao 선언문들은 컴파일되긴 하지만, 하나의 매개 WES 사용하여 Aras 호출하면
컴파일 오류가 발생합니다. 4768006 100와 Area(int) 사이에 모호성이 존재합니다.

연구

Ltt 원형과 함수 정의 사이의 차이점은 무엇입니까?

2 매개 Heol 이름은 원형과 정의와 실제 함수 호출에서 일치해야 합니까?
3. 함수가 값을 반환하지 않는다면, 어떻게 함수를 선언합니까?

4 반환값을 선언하지 않는다면 어떤 형의 반환값이 가정됩니까?

$ 지역 변수란 무엇입니까?

6 범위 규칙이란 무엇입니까?

7. 함수의 자기 호출이란 무엇입니까?

@, 전역 변수들은 언제 사용됩니까?

9 함수 중첩이란 무엇입니까?

10. 다형성이란 무슨 뜻입니까?

연습 문제

I. Perimeter)Ft= 이름을 22 unsigned long int 값을 반환하며 unsigned short

int 두 개를 매개 변수로 갖는 함수의 원형을 작성하시오.

+>
!
cr


===== PAGE 147 =====
144 ee 제1주

2.

1번에서 서술된 『6「107616『()라는

mee    의를
떠1   ote                           |
사각형의 가로와 세로를 의미합니다. 함수는 그 직사각형의 둘레길이를 반환합니다
3 버그잡기 : 아래에서 HIS 잡읍시다.
#include <iostream.h>
void myFunc(unsigned short int x) ;
int main()
{
unsigned short int x, y ;
y = myFunc(x) ;
cout << "xe " <<1K <<." yr << y << Nn” |
return 0;
}
void myFunc(unsigned short int x)
{
return (4%*x);
}
4. 버그잡기 : 아래의 코드에서 무엇이 잘못되었습니까?
#include <iostream.h>
int myFunc(unsigned short int x);
int main()
{
unsigned short int x, y;
y = myFunc(x);
cout << "xe MK<ix << oye y "Xn";
return 0;
}
int myFunc(unsigned short int x);
1
return (4%* x );
a
5. = 개의 unsigned short int 인수를 갖고 A 번째 수를 두 번째 수로 나눈 수의 결과
를 반환하는 함수를 작성합시다. 두 번째 수가 0일 때엔 나누지 말고 -1을 반환합시다
6. 사용자에게 두 개의 ANS 입력할 것을 요구한 뒤 위 5번의 함수를 부르는 프로그램을
작성합시다. 답을 출력하거나 -1을 얻을 경우는 오류 메시지를 출력합시다
7. 숫자와 거듭제곱 값을 받는 프로그램을 작성합시다. 숫자에 거듭제곱하는 기능을 호출
함수를 써서 만듭시다. oS 들어, 숫자 2와 거듭제곱 4를 입력받으면 2를 4제곱하는
값을 반환합니다



===== PAGE 148 =====


===== PAGE 149 =====
146 ee 제1주

서문

레싱 가여 복잡한 실생활에서 일어나는 x4 분 구현하고 풀어
움을 주는 0+의 내장된 기능 중 하나입니다
같습니다.

BM 클래스|0056란 무엇이고 YAllobject= 무엇인가?
어

아모
크
ot
de
ot
kb
|

WE 멤버 함수|767006: 141010ㅁ|란 무엇이고 멤

48-84 t(constructorlet 무엇이고 어떻게 사용하는가?

새로운 (New Type) 만들기

여러분은 이미 여러 개의 변수형
A 많은 것을 알려줬습니다. 예를
선언했다면, 각각은
다.(정수형이 2 바이트라면
ae 가지는 것은 오류들
이름을 저장할 수 없습니다.

WSS unsigned short inte 선언하면서 여러분
그 결과를 다른 숫자에 더할 수 USS 알았습니다.

이 형이라는 것은 여러분에게 Ges 말하여 줍니다.
를 변수가 사용하는 메모리

들어 여러분

I

현실 세계의 BASS 해결하기 위해 무

에 대하여 배웠습니다. ©
이 Height} wii unsigned int=
0부터 65,535 사이의 숫자를 가질 수 있다는
말입니다.) 이것이 unsigned inteh= 의미입니다. 이 변
발생시킴니다. unsigned short into] 여러분의

은 Height?} Width=

클래스의 객체는 어떻게 ELE

자료|76066「 00이란 무엇인가?

형들이 여러분에

것을 알았습니

서로 더하고

만들어집니다. 예를 들

이의 레코드를 추적하기 위해 만들어지거나 열 시스템의 작용을 시뮬레



===== PAGE 150 =====
새로운
응어

[>
fo
[모
&
~~
©
20
Ww
7)
20
3
으
=
ㅇ@
글
oy
@

차에 대하여 아는 모든 것을 하나의 클래스로 캡슬화하는 것은 프로그래머에게
상당한 이점을 줍니다. 모든 것이 하나의 장소에 있습니다. 이는 그 자료들을 참
조하기 쉽게 하고 복사, 연산하기 쉽게 합니다. 똑같이 클래스의 Se}o] gE (client

여러분의 PAT 쓰는 프로그램의 부분)들은 여러분의 객체를 그 안에 무엇
이 있는지, 또는 어떻게 동작하는지 알 필요 없이 잘 사용할 수 있습니다.

멤버 변수(0ㅠ60066『 variable), 자료 멤버(0313 member) 멤버 변수(록
멤버)는 여러분의 클래스의 변수들입니다. 멤버 변수들은 여러분의 클래스의
니다. 마치 바퀴와 엔진이 여러분 자동차의 일부인 것처럼.
클래스 안의 함수들은             을 연산합니다. 그들은 멤버 (member
클래스의 메쏘드라 부릅니다. 자동차 클래스의 메쏘드는

가질 수 있고 메쏘드에는 916620, Meow(), ChaseMice) 등을 가질 수 있습니다.


===== PAGE 151 =====
148 ee ANF

로운 Bt Bi+(member function), 메쏘
용이

In
ii
[10

러분의 클래스 안의 함수들입니다. 멤버 함수
래스의 한

합니다.

클래스의 A (Declaring a Class)

클래스를 선언하기 위해 005라는 예약어를 사용합니다. 그 뒤에 클래스 이름과
시작 중괄호를 쓰고 자료 멤버의 목록0190을 쓰고 그 클래스의 메쏘드를 Hye.
마감 중괄호로 AVS 마치고 세미콜론을 씀니다. 여기 (#라는 클래스를 선언하
여 봅시다.
class Cat
ne

unsigned int itsAge;

unsigned int itsWeight;
Meow();

이 클래스를 선언한다고 (0#에게 ALIS 할당하지는 않습니다. 단지 컴파일러
에게 Cato] 무엇인지를 알려주고 어떤 자료들을 갖고 있으며046486 , itsWeight),
무          는지04460\0) 알려줍니다. 그리고 컴파일러에게 (#이라는 클래스
가 얼마나 큰지(얼만큼의 메모리를 차지하는지)를 알려줍니다. 예를 들어, 정수형
이 2바이트이면 (#은 4바이트입니다. itsAge7} 2바이트 크기이고 16\8194도 2바
이트의 크기입니다. Meow 크기를 차지하지 않습니다. 왜냐하면 멤버 함수를
위해서는 공간이 할당되지 않기 때문입니다.

ra

이름짓는 법

프로그래머로서 여러분의 모든 멤버|변수와 멤버 함수, 클래스에 이름을 붙여야
합니다. 3일째 날의 학습에서 배웠듯이 이해하기 쉬워야하고 이름에 의미가 있어
ok 합니다. Cat, Rectangle, Employe= 다 좋은 클래스의 이름입니다. Meow0,
ChaseMice(), StopEngine)= 그 이름들만 보고도 EAS 하는 함수인지 알기 때문
에 좋은 멤버 함수명입니다. 많은 프로그래머들이 멤버 변수에 라는 접두어를
붙입니다. itsAge, itsWeight, itsSpeed SAW 말입니다. 이는 멤버 변수와 비멤버
변수를 쉽게 구별하게 합니다.



===== PAGE 152 =====
를 붙이기를 좋아합니다 - |S So} cCat, cPersnS YU. 또 딴 사람은 이름
모두 대문자로 한다든지 또는 소문자만으로 합니다. 저자가 즐겨 쓰는 방법은 첫
글자를

대문자로 쓰는 것입니다.(086 Person)
와

한편 이와 유사하게 많은 프로그래머들이 함수는 대문자로 시작하고 모든 변수는
SEAS FU. 단어들은 밑줄 문자로 분리(2066.809하거나, 혹은 각 단어의

시작을 대문자로 쓸 <F(ChaseMice, DrawCicle) 있습니다.
러분은 하나의 스타일을 선택하여 계속 그것을 쓰라는 것입니다.

여                          쓰
to] 흘러 여러분의 이름짓기, ~ SUS 정렬, 주석문 다는 방법들이

a

소프트웨어 제작회사는 여

이는 타인의 프로그램을 4

고 .또
ㅇ     | >
aa)
The
Je
Ao
=
ps
그
뼈
가
tulo
ot
에
rir
>고
=
ol
ko
rat
oa
mu

객체 78 2](Defining an Object)
APY 변수를 정의하듯이 객체를 정의합니다.

unsigned int GrossWeight;      // unsigned int® 정의
Cat Frisky;                 // Cat2 = 정의
~~

이 SE unsigned 1따형으로 GrossWeight4H= 변수를 정의하였습니다. « 클래스
명이 04인 객체 Frisky 정의하였습니다.

클래스와 객체

고양이에 대한 정의 그 자체를 애완동물처럼 키울 순 없습니다. 우리가 키우는 고
Sols 개념이 아닌 실제의 고양이입니다. 여러분은 고양이의 개넘과 실제 여러분
의 집안을 배회하는 고양이를 구별해야 합니다. 같은 방식으로 ++에서는 클
(과 - 이는 cate] 개념이고 - 실제의 Cat] 객체를 구별해야 합니다. Frisky Cat
형의 객체인데 이는 GrossWeight7} unsigned 정수형의 변수인 것과 같습니다.

ib 3

새로운 객체 WHE 클래스에 있어서의 각각의 실체(14666066)입니다. 실체화하는 것을 인

객체 객체는 클
응어 스턴스한다고 합니다.


===== PAGE 153 =====
150 ee AI

클래스 멤버에의 접근(^&66655108 Class Member)

일단, Cato] 객체를 정의하였으면(여기선 Frisky) 여러분은 A.) 연산자를 AA
객체의 Bo] 접근을 할 수 있습니다. 따라서 80090/의 Weight 멤버 변수에 50을
대입하려면 아래와 같이 Bue.

Frisky.Weight = 50;
같은 방식으로 Meow) 함수를 쓰려면
Frisky .Meow();

라 FUT. 클래스 메쏘드들을 사용하려면 메쏘드를 호출해야 합니다. 여기서 여
러분은 0096의 Meow0S 호출하였습니다.

클래스에 대입하지 말고 Wao] 대입해야 합니다
0++에서 여러분은 값들을 변수형에 대입하지 않고 변수에 대입하였습니다. 즉

106 = 5 5    // 틀림

컴파일러는 오류 메시지를 내보낼 것입니다. 왜냐하면 여러분은 정수형에 5를 대
임할 수 없기 때문입니다. 숫자는 정수형 변수에 대입이 가능한 것입니다. 즉
int x;     // xB int® 정의

x=5;   // ×를 5로 설정

즉, 5를 정수형 변수 xo] 대입합니다. 똑같은 방식으로

cat.age=5; // 틀림
라고 쓰면 컴파일러는 다음과 같은 CHES 보여줍니다.

222 I suggest that the "wrong" comment be changed to "cat not defined"
or some other message. The code is not wrong ( if Cat has been defined )

왜냐하면 여러분은 클래스 Cato] age 부분에 5S AVS + 없기 때문입니다. 바
른 방법은 Cat 객체를 만든 뒤 그 변수에 5를 대입하는 것입니다.

Cat Frisky ;    // int x ;와 같음
Frisky.age=5; //x=5 ;와 같음



===== PAGE 154 =====
이런 실험을 해봅시다. 어런애에게 가서 고양이를 보여줍니다. 그리고 말합니다.
“이 고양이 이름은 8096입니다. Frisky= 장난을 좋아합니다. Frisky= 멍멍하고
ASU” 어린이는 당장에 비웃을 것입니다. “나 원 a. 고양이가 어떻게 멍멍

Cat Frisky;         // Frisky*@f= 이름의 cat& 만들고

Frisky.Bark();       // Frisky2| Bark®J= 함수를 실행합니다.

컴파일러는 말할 것입니다. Cate BakS 수행 안함(꼭 이렇게 말한다기보다 비슷
하게 말할 것입니다.) ABUL Cat 클래스가 8000 FEE 선언하지 않았기 때
문에 수행할 수가 없다는 것을 압니다. 컴파일러는 8094가 가령 MeowOZh= 함
수를 안 가지고 있다면 역시 AVS 하지 않을 것입니다.

하려면 0655라는 예약어를 씀시다.

00 클래스를 선언
DONT 정의와 선언을 온동하지 WL 선언은 클래스가 무엇인지를 컴파일러에게
알리는 것이고 정의는 실행시 실제 메모리를 할당받게 하는 것입니다

객          |
DON'T 클래스에 갔을 대입하지 AML. 객체 또는 자료 멤버에 할당래야 합니다.
버

변수와 함수에 PSs] 위해 점(': )ㆍ연산자를 씀시다.

전응(0110016)과 E4-2(public)ol] 관해

또 다른 예약어가 클래스를 MAD 때 사용됩니다. 범용(600880과 AV (private)
니다.

= 클래스의 멤버는(자료와 메쏘드) 기본적으로 전용입니다. 전용 멤버들은 그
래스 안의 메쏘드들에 의해서만 접근될 수 있습니다. 범용 멤버     =

스의 객체에 의해서도 접근될 수 있습니다. 이 차이는 매우 중요

가져옵니다. 좀더 분명히 하기 위해 이번 장의 처음 부분에 있는 보기를 봅시다.

class Cat
£

 td

unsigned int itsAge;
unsigned int itsWeight;


===== PAGE 155 =====
152 ee 제1주

Meow() ;
+;
여기의 선언에서 itsAge, itsWeight, Meow 모두 전용인데, 왜냐하면 클래스의
모든 멤버들은 기본값이 전용이기 때문입니다. 다른 방식으로 범용임을 지정하지
않으면 ago] 됩니다. 다음 예에서

Cat Boots;

Boots.itsAge=5; // 오류 , 전용 자료는 접근 못함

컴파일러는 오류를 Yayo 실제 여러분은 컴파일러에게 des 같이 말한
셈입니다. “나는 16486, itsWeight, 460\(를 Cat 클래스의 멤버 함수 범위 내에서
접근하려 했다” 그럼에도 불구하고 여러분은 Cat 메쏘드의 바깥으로부터 접근하
려 한 것입니다. Boots7} Cat SHA 객체라 해도 여러분이 전용으로 되어 있는
0006의 일부분에 접근할 수 없습니다.

이러한 부분이 처음 CHE 접하는 사람에게 상당한 EFS 일으키며 이해하기도
힘듭니다. 여러분은 말할 AMC. “Boots= (으로 지정돼 있다. 왜 8006는
itsAgeo] 접근할 수 없는 것일까?" 거기에 대한 HAS 여러분은 할 수 없다는 것
입니다. 8006는 그 자신의 메쏘드를 통해서 그의 모든 부분을(전용이건 범용이
건) 접근할 수 있습니다. 여러분이 CaS 만들었지만 그렇다고 여러분이 그 전용
으로 지정된 부분을 보거나 바꿀 수 없는 것입니다.

Cato] 자료 WH 접근할 수 있는 WAS 다음과 같이 하는 것입니다.

class Cat

{

public:
unsigned int itsAge;
unsigned int itsWeight;
Meow();

3;

itsAge, itsWeight, Meow) 모두 범용입니다. 8006.15&686 = St 아무런 오류 없이
컴파일됩니다. [리스트 6.1]은 간단한 클래스의 범용 멤버에 접근하는 예제입니다.

[리스트 6.1] 간단한 클래스의 HF 멤버에 접근하는 예

// [리스트 6.17 간단한 클래스의 범용 멤버에 접근하는 예
//                                                    .          \

1

2

3:
4: #include <iostream.h> // cout 용
5



===== PAGE 156 =====
제6일 기본적인 클래스 ee 153

6: class Cat          // -클래스 선언
te £

8: public:           // 범용 멤버
oe   int itsAge;

10%   int itsWeight;

12:

135

14: int main(Q)

15: £

16:   Cat Frisky;

17:   Frisky.itsAge =5; // 멤버 Hoy 대입

18:   cout << "Frisky is a cat who is " ;

19%   cout << Frisky.itsAge << " years old.\n";
20:   return 0;

결고   Frisky is a cat who is 5 years old.
불셀 6H SL 예약어 class 가집니다. 컴파일러에게 그 다음에 오는 것은 선언임
을 말해줍니다. 0898라는 단어 다음에 클래스명이 옵니다. 여기선 0#입니다.

선언부의 몸체는 TH 줄에서 시작 SBSH 함께 시작되어 11번 줄의 마감 중괄호
에서 세미콜론과 함께 끝납니다. 8번 al 예약어 publicS 지정하였고 이는 다음
의 private7} 나오거나 혹은 클래스의 BS 만나기 전까지는 범용임을 지정합니다.

9, 10번 줄에서 15486와 169\819보라는 클래스 멤버를 선언하였습니다.

14번 줄에서 프로그램의 main) 함수를 시작합니다. 8096/는 16번 줄에 Cato] 한

객체로 정의되어 있고 Frisky2] 나이는 17번 줄에서 5살로 되었습니다. 18에서 19

번 줄의 16486 멤버 변수는 Friskyo] 대한 메시지를 출력하기 위해 쓰였습니다.

8번 줄을 주석 기로로 막아버리고 다시 컴파일하여 봅시다. 17번 줄에서 오류가 나올

i

ro

멤버 자료를 전응으로 만들기
프로그램 설계의 일반 wae 클래스의 멤버 자료를 apo 를 전용으로 만드는 것입니다.
이렇게 하려면 여러분은 전용 변수를 설정하고 가져올 수 있기 위해 소위 접근

자 메쏘드로 알려진 범용 함수를 만들어야 합니다. 이 접근자 메쏘드는 여러분

ee


===== PAGE 157 =====
154 ee AIF

ie
is
오비
ofo
oe
~
i
mfr
nee
ox
=
i.
en
bo
as)
ae
“Ol,
모
포
ㅁ웨
+

로그램의 다른 부

니다.

새로운 WS 접근자 메쏘드(604611ㅇ accessor method) 범용 접근자 메쏘드는 클래스의
변수

20 |

웅이 전용 멤버 변수를 읽고 설정하는 멤버 함수입니다.
왜 이러한 우회적인 접근 Woe 일을 복잡하게 만듭니까? 나중에 두고보면
알겠지만 사실 이 방법이 더 쉽고 일반적인 접근자 함수보다 사용하기가 간단합

니다.

접근자 함수들은 여러분으로 하여금 “어떻게 자료가 저장되는가"라는 문제와 '어
떻게 사용되는가"라는 문제를 분리할 수 있게 하여 줍니다. 이는 여러분이 자료를
사용하는 함수를 다시 만들 필요 없이 자료가 저장되는 방식을 바꿀 수 있게 하
여 줍니다.

만일 여러분이 자료의 저장되는 YAS 바꾼 후, Cato] 나이를 필요로 하는 함수
가 16486에 직접 접근하려면, 그 BPE 다시 작성되어야 합니다. 0064860라는
함수를 가짐으로써 Cat 클래스는 여러분이 16486에 접근하지 않고도 886의 Su}
른 값은 반환할 수 있습니다. 호출 함수는 886가 어떤 형으로(098000 정수형 이
건, 1008형이건) 저장되는지 알 필요도 없고 여러분이 요구하는 대로 계산하는지
도 알 필요가 없습니다.

이 기법은 여러분의 프로그램을 유지하기 쉽게 하여줍니다. 애초의 설계가 바뀌
어도 코드는 바뀌지 않으므로 여러분의 코드가 긴 생명을 갖도록 해줍니다.

[리스트 6기는 전용 멤버 자료와 범용 접근자 메쏘드를 가지도록 수정되었습니다.
단, 아직 실행할 He 없습니다.

[리스트 6.2] 접근자 메쏘드를 가진 클래스

// Cat class 선언
// THEE 전용이며, BS 페쏘득가
// 전용 자료를 설정 및 가져옴

class Cat
{
public:
Jif 범용 메쏘드
unsigned int GetAge();
void SetAge(unsigned int Age);

= - OANA UFWN —

= Os . «



===== PAGE 158 =====
제6일 기본적인 클래스 ee 155

V2:   unsigned int GetWeight();
13%   void SetWeight (unsigned int Weight);

TAS

15:  // 범용 멤버 함수
16:   Meow();

AS

18:   // 전용 멤버 자료
19: private:

20:   unsigned int itsAge;
215   unsigned int itsWeight;

j a 이 클래스는 다섯 개의 범용

itsAge= 위한 접근자 메쏘드
위한 접근자 메쏘드를 가지고 있습
고 그 값을 반환합니다.

ag

메쏘드를 가지고 있습니다. 9, 10번 SS
가지고 있습니다. 12, 13번 SS itsWeight=

ㅇㅇ

=

2                    곤

니다. 이 접근자 합수들은 멤버 변수를 설정하

범용 멤버 함수 MeowQt 16번 줄에 선언되어 있습니다. Meow 접근자 함수
가 아닙니다. 멤버 변수들을 얻거나 설정하지 않습니다. 이는 클래스에게 다른 서
비스를 제공합니다. 0604라는 단어를 출력하는 것입니다.

멤버 변수들은 20, 21번 So] 선언되어 있습니다.

Frisky] 나이를 설정하려면 다음과 같이 90648600라는 메쏘드에 값만 전달하면
됩니다.

Cat Frisky ;
Frisky.SetAge(5) ;

전응성과 보안성에 대하여

메쏘드 또는 전용 자료를 선언하면 컴파일러로 하여금 프로그래밍 오류를 일찍
wad 수 있게 합니다. 또 능력 있는 프로그래머라면 맘만 먹으면 ag 방식을
사용하여 여러 문제를 해결할 수 기이 Ceo] 창시자 스트라우스트림은
“++의 접근 통제 방식은 우연한 실수로 보안을 깨는 일을 막을 수 있습니다. 물
론 의도적인 침입자로부터의 문제는 별개 자 만…(404, 1990)라고 기술하였습니다


===== PAGE 159 =====
156 ee 제주

class 에악억
class class name
<                             |
// 접근 통기 AB Alt AAAS
// 클래스 변수와 LES OP 써 동습니다.

23
class 예약어는 새로운 BS 선언하기 위해 사용합니다. 클래스는 클래스 멤버 지료들의
집합인데 이는 다른 클래스를 포함하여 여러 형들의 변수를 포함합니다. 클래스는 또한 클
래스 함수(메쏘드)를 포함합니다. 이는 클래스의 자료들을 연산하고 클래스의 다른 서비스
들을 수행하기 위한 함수입니다.       |
여러 변수들을 정의하는 방식으로 새로운 형의 ”   정의합니다. 형을 기술하고(0855)

ecole 쓰고(객체), 클래스 멤버와 함수에 점( . ) 연산자를 서서 점근합니다.
클래스를 전용으로 할 것인가 $2 범용으로 할 것인가는 접근통제 예약어를 사용하면 됩
니다. 기본 접근 방식

은 전용입니다. 각 예약어의 ane 클래스 선언의 끝 부분까지이거
나 다른 접근 통제 예약어를 만날 때까지입니다.  마감 중괄호와 세미콜론을 만나면 클래스
선언이 끝납니다.

보기 |

class Cat

{《

public :
unsigned int Age;
unsigned int Weight;
void Meow();

+?

Cat Frisky ;
Frisky.age = 8;
Frisky.Weight = 18;
Frisky.Meow() ;

보기 2
class Car
1
public :

void Start( ;// 다음의 5개는 범용임
void Accelerate() ;
void Brake() ;
void SetYear( int year ) ;
int GetYear() ;
private :// 나머지는 전용임
int Year ;



===== PAGE 160 =====
char[255] Model ;
+; df BAA 선먼의 글

Car OldFaithful;// Car2| 종류

int bought;// int9l 직역 변수
OldFaithful.SetYear(84) ;// Year 84 대입

bought = OldFaithful.GetYear();// 848 bought 대입
OldFaithful.Start();// StartQOS 코줄

Do       전용 멤버 변수를 선언합시다.

Do       범용 접근자 메쏘드를 사용합시다.

DONT 클래스 바깥에서 전용 멤버 변수를 사용하려는 불필요한 노력을 하지 oY
서드
It

Do       클래스 멤버 함수 안에서부터 전용 멤버 toy 접근합시다

클래스 메쏘드 구현(|070!86100004109 Class Method)
보았듯이 접근자 함수는 SHAS] 전용 멤버 자료에 범용 인터페이스00000009를
제공합니다. 각 접근자 함수는 여태껏 여러분이 선언한 다른 클래스 메쏘드와 마
찬가지로 FAS 할 수 있습니다.(당연합니다) 이 수행을 함수 정의라 합니다.

멤버 함수 정의는 클래스의 이름으로부터 시작하여 두 개의 콜론을 넣고 함수명
을 쓴 뒤 매개 BFS 씀니다. [리스트 63°] 간단한 ce Balas 완전한 Uae

보여주고 그 접근자 함수 및 일반적인 클래스 wy dpe] 구현을 보여줍니

[리스트 6.3] 간단한 클래스 메쏘드의 구현

1: // [리스트 6.3] 간단한 클래스 메쏘드의 구현

Ze 17

3

4: #include <iostream.h>      // cout &
55

6: class Cat                // 클래스 선언
8 게

8: public:                  // 범용 부분
9    int GetAge();        // 접근자 함수


===== PAGE 161 =====
158 ee 제1주

10:
113
12:
13:
14:
15,
16:
10
18:
19%
20:
21%
22:
23:
24:
Zoe
26:
2:
28:
29:
30:
ons
32:
334
34:
55:
S56:
Sf:
38:
59:
40:
al:
42:
43:
44:
45:
46:
47:
48:
49:
50%
D1:
52:
55:

void SetAge (int age);   // 접근자 함수
void Meow();             // 일반 함수
private:                   // 전용 부분
int itsAge;             // 멤버 변수
3;
// GetAge, 범용 접근자 함수
// itsAge 멤버값 반환
int Cat::GetAge(
{
return itsAge;
J
// SetAge 범용

// 접근자 함수

// itsAge 멤버값 반환

i   Cat::SetAge(age)

// 멤버 변수 itsAgeS
// age= 대입
itsAge = age;

// Meow RE
// 반환값 .: void
// 매개 변수 : 없음
// 하는 일 ： "Meow." 화면에 출력
void Cat: :Meow()
{
cout << "Meow.\n";

// cat 만들고 나이를 설정함
// 0ㅁ601를 하고ㆍ나이를 알린 뒤 다시 한번 meow
int main(Q)
{
Cat Frisky;
Frisky.SetAge(5);
Frisky.Meow();                  :
cout << "Frisky is a cat who is " x
<< Frisky.GetAge() << " years old.\n";
Frisky.Meow() ;
return 0;



===== PAGE 162 =====
제6일 기본적인 클래스 ee 159

결교  Meow.

Frisky is a cat who is 5 years old.
Meow.

ere 클래스의 정의입니다. 8번 줄은 public 예약어가
~ 있는데 컴파일러에게 다음 줄부터는 범용 멤버임을 알립니다. 9번 se
용 접근자 메쏘드 084860 선언입니다.

ㅁ또

GetAge(i= 전용 멤버 변수 16486에 접근 권한을 주는데 13번 줄에 선언되어 있
습니다. 10번 So] 범용 접근자 MRE SetAge7} 있습니다. 9664800 인자로 정
TBS 취하고 인자값을 16480에 설정합니다.

11번 So] 클래스 메쏘드 Meow07} 있습니다. 4460\0는 접근자 함수가 아닙니다.
이는 4460를 출력하는 일반 메쏘드입니다.

12번 줄은 전용 부분입니다. 13번 줄의 16486 하나를 가지고 있습니다. 14번 So]
서 마감 중괄호와 함께 세미콜론으로 끝납니다.

18부터 21번 SS 멤버 함수 0844800의 정의가 있습니다. 이 메쏘드는 매개 변
가 없습니다. AEBS 빈환합니다. 18번에 나와있듯이 클래스 메쏘드는 클래스

에 콜론을 두 개하고 함수명을 넣습니다. 이 FES 컴파일러에게 지금 기는
08880 함수는 Cat IAS) 있는 함수라는 것을 말해줍니다. 표제 부분만 피고
aero] 정의와 똑간습니다

GetAge) 함수는 한 줄로 되어 있습니다. 15486에 있는 WS 반환합니다. 0200
함수는 15486가 Cat 클래스의 전용으로 선언되어 있기 때문에 접근할 수가 없슴
니다. 반면 mainQ2 범용 메쏘드 0664860에 접근할 수가 있습니다. 0664800는
Cat 클래스의 멤버 함수이기 때문에 16480에 접근할 수 있습니다. 따라서
GetAge()= main()o] 7] 18486의 값을 반환할 수 있게 해줍니다.

26번 줄은 SetAge) 멤버 함수의 정의가 있습니다. 정수형 매개 Wes 가지고
16486의 AS 매개 변수의 값으로 대입합니다.30번 줄) Cat 클래스의 멤버 함수
이기 때문에 165486에 접근 권한이 있습니다.

37번 줄은 Cat 클래스의 Meow() 메쏘드의 정의(혹은 수행)로 시작됩니다. Meowe}
는 단어를 화면에 출력하는 한 줄의 함수입니다. we 화면에서 새로운 SS 여
개행 문자입니다.

44번 줄은 main) 함수의 몸체입니다. 여기서 인자는 없고 정수값을 반환합니다.
46번 줄에서 main-2 Cat 객체로 FriskyS 선언하였습니다. 47번 줄에서 SetAge()
ACA 메쏘드를 써서 값 57} 15486 멤버 변수에 대입되었습니다. 보다시피 클래

ct rr


===== PAGE 163 =====
160 ee AIF

스 이름 다음에 점 연산자가 있고 메쏘드 이름(604800)이 있습니다. 이런 방식으
로 다른 메쏘드를 호출할 수 있습

르츠
2a

48번 SS Meow) 멤버 함수를 부르고 SOW 줄에서 GetAge) 접근자를 써서 나이
력하고 다시 51번 SoA] 4460\0를 실행합니다.

생성자와

b>

©3Xi(Constructor and Destructor)

정수형 변수를 정의하는 두 가지 방법이 있습니다. 변수를 선언하고 나중에 RES
대입하는 방법이 있습니다. 예를 들

int Weight ;          // 변수 정의

nee                   // 다른 BES

Weight = 7;           // 값을 대입

혹은 정수형을 선언하고 즉시 초기화할 수 있습니다. 예를 들어
int Weight = 7 ;// 정의하고 7로 초기화

27a} 변수 정의와 동시에 진행됩니다. 물론 나중에 WS 바꿀 수 있습니다,
기화는 변수가 의미 있는 AS 가지고 시작함을 알려줍니다.

클래스의 멤버 자료는 어떻게 초기화합니 까? 클래스들은 생성자(6009004000라는
별한 멘버 함수가 있습니다. 이 생성자는 필요한 만큼의 매개 wes 가질 수
습니다. 그러나 반환값은 - 100형조차 - 가질 수 없습니다. 이 생성자는 클래스
신과 같은 이름을 가진 클래스 메쏘드입니다.

소멸자(06600000라는 것도 만들어야 합니다. 생성자가
있는 것처럼 소멸자는 여러분의 객체값을 소멸시키고 할당되
다. 소멸자는 클래스와 같은 이름을 갖는데 ~기호가 앞
반환값도 없습니다. 따라서 Cat 선언은 다음

베 EN

노계 Sul

고

Bom WU
L oF

th
Sy

에

ay 쿄

고
wt 도 ig fy fl

lo & >?
Het ot
it oy

“CatQ;

기본 생성자와 AGAKDefault Constructor and Destructor)
생성자와 소멸자를 선언하지 않는다면 컴파일러는 생성자와 소멸자를 하나씩 만
들어 놓습니다. 기본 생성자와 소멸자는 인자가 없고 아무 일도 하지 않습니다.



===== PAGE 164 =====
제6일 기본적인 클래스 ㅎㅎ 161

아무 일도 하지 않는 생성자가 무슨 소용이 있는가. 사실은 형식적으로 그렇게
합니다. BE 개체는 만들어지고 없어집니다. 그리고 그때마다 이 아무 일도 않는
생성자와 SAA} 불려집니다. 아래와 같이 매개 WES 전하지 않고 개체를 선
언하면

—

Cat Rags ;// Rags= 매개 변수가 없음

다음과 같은 생성자를 갖습니다.

CatQ ;

클래스의 객체를 정의할 때 생성자가 불려집니다. 08 생성자가 = 개의 매개 변
TS 가지려면, 여러분은 Cat] 객체를 다음과 같이 정의합니다.

Cat Frisky (5,7);

만일 생성자가 하나의 매개 변수를 가지려면, 객체는 다음과 같이 정의합니다.
Cat Frisky (3);

생성자가 매개 변수를 하나도 안 갖게 하려면 BSE 쓰지 말고 다음과 같이 씀
니다. (지금까지 이렇게 써왔습니다.)

Cat Frisky ;
이는 모든 함수는 설령 매개 변수가 없더라도 괄호를 Dee 한다는 법칙에 예외
조항입니다. 그래서 다음이 가능합니다.

Cat Frisky ;

그리고 이는 기본 생성자(06041 000500000라 부릅니다. 매개 변수는 없고 괄호
도 없습니다.

여러분은 컴파일러가 제공한 기본 생성자를 쓰지 않아도 됩니다. 여러분은 매개
변수가 없는 자신만의 생성자를 맘대로 쓸 수 있습니다. 심지어 매개 변수가 없

는 생성자가 몸체를 가지고 그들의 객체를 초기화할 수 있고 다른 일도 할 수 있

습니다.

메레 으로 생성자를 만들었다면 소멸자도 만드는 것을 ow 안됩니다. 물론
멸자가 아무런 ㄴㄴ ey 해도                        해도

qoz  만들어  ay ~


===== PAGE 165 =====
162 ee AIF

[리스트 6시는 Cat 객체를 초기화하기 위한 생성자를 사용하기 위해 Cat 클래
다시 작성하였습니다. 초기화는 나이를 여러분 임의로 지정하는 것입니다.

를
es,
론 소멸자도 지정하였습니다.

[리스트 6.4] 생성자와 소멸자에 대한 예제

Zs
u
se

1: // [리스트 6.41 생성자와 소멸자에 대한 예제
2s 7/

3

4: #include <iostream.h>

55

6: class Cat

ti x

8: public:

9:   Cat(int initialAge); // 생성작
10:   “Cats           1] 23s

11:   int GetAge();

ia   void SetAge(int age);
15   void Meow();

14: private:

15:   int itsAge;

167 33

17.

18: // Cat2| 생성자

19: Cat::Cat(int initialAge)
20: £

21:   itsAge = initialAge;
22: }

23:

24: Cati::~CatQ          // 소멸자, 아무 행동 없음
255 <

26: +}

2c:

28: // GetAge

29: // itsAge 멤버 반환

30: int Cat::GetAge()

Ss

52:   return itsAge;

$5: >

34:

35: // SetAge 선언

56: //

37: // itsAge 멤버 설정

38: int Cat::SetAge(age)
59: £



===== PAGE 166 =====
제6일 기

THE
전
[을
mu

래스 ee 163

40:   //
41:    // itsAgeS age® 설정
42:    itsAge = age;

452 }
44:

45: // Meow 메쏘드 선언
46: // 반환값: void

47: // 매개 변수: 없음
48: // 하는 일 : Meow 출력
49: void Cat::Meow()

50: {

D1:   cout << "Meow.\n";

52830
352
54: //

55: // meow 하고 나이를 알린 뒤 다식 meow
56: int main()

aire 1

58:   Cat Frisky (5) =

59:   Frisky.Meow();

60:   cout << "Frisky is a cat who is" ;

61:   cout << Frisky.GetAge() << " years old.\n";
62:   Frisky .Meow();

63:   Frisky.SetAge(7);

64:   cout << "Now Frisky is " ;

65:   cout << Frisky.GetAge() <<" years old.\n";
66:   return 0;

67: }

fl

Meow.
Frisky is a cat who is 5 years old.

Meow.
Now Frisky is 7 years old.

(ag
Jd
cc)
|
\m
a
>
rl
때
|
\m
a
x
=z
>
ies
a
우
된
{ru
oy
rlo
\O
cE
nt)
Jeo,
on
4)
oot
tho
N,

가졌다는

도 반환값

19부터 22번

다. 반환값

400 yy!

pes

Or
a

입니다. 소멸자는 매개 변수를 갖지 않고, 생성자 및 소멸자 아무 것

- 심지어 100형도 - 갖지 않습니다.

줄까지 생성자가 구현됩니다. 마치 SetAgey 접근자 함수와 비슷합니
없습니다.


===== PAGE 167 =====
164 ee AF

24부터 26번 줄까지 소멸자 ~080의 구현입니다. 이 함수는 아무 일도 않고 마치
클래스 선언에서 하듯이 단지 함수의 정의만을 하였습니다.
58번 SS Cato] 객체 FriskyS 정의하였습니다. 값 5가 Frisky2] 생성자에게 전해

졌습니다. 따라서 SetAgQS 부를 필요가 없어졌습니다. 63번 줄에서 『096의
itsAge7} 7의 값을 받았습니다. 65번 줄에서 새로운 값을 출력합니다.

00. ote) ats SISter] Het Vote 씀시다

DON'T 소멸  aro 매개 A RT| SEATET.

const 멤버 함수

클래스 메쏘드를 constz 태이 해당 클래스의 어떠한 Buiee 바
꾸지 말아야 합니다. 클래스의 상수       선언하려면 괄호와 세미콜론 사이
에 const 예약어를 넣습니다. 상수 멤버 함수 90068000000의 선언은 매개 변수가
없고 void & 반환합니다.

void SomeFunction() const ;
접근자 함수들은 가끔 const 써서 상수 함수로 선언됩니다.

void SetAge (int anAge) ;

int GetAge() ;

SetAge(= 상수형으로 선언될 수 없습니다. 왜냐하면 멤버 변수 15406의 AS 바
꾸기 cree 한편 6   버버  클래스의 값을 전혀 바꾸지 않기 때문에 상수
형으로 선언될 수 있고 또 되어야 ver 단지 현재 멤버 변수 15406를 반환하
기 때문입니다. 따라서 이러한 BESS 다음과 같이 쓰여야 합니다.

void SetAge ( int anAge ) ;

int GetAge() const ;

하고, 실제 함수 실행시 객체값을 바꾼다면 컴
어, GetAge() 안에 Cato] 나이를 물어보는
를 내보냄니다. 왜냐하면 이 메쏘드를 호



===== PAGE 168 =====
const 가능한 한 많이 쓰도록 합시다. 객체의 갔을 바꾸지 않는 곳엔 멤버 함수를
상수령으로 선언합시다. 이는 컴파일러가 She SER 하는데 도음을 즐 것입니다
컴파일러가 오류를 찾는 것이 빠르고 과적입니다.

가능      하면         많  은

입터페이스와 구현

이미 배웠듯이 클라이언트(01600는 여러분의 클래스를 가지고 객체를
프로그램의 일부분입니다. 여러분은 여러분의 클래스(즉, 클래스
이 클라이언트와의 인터페이스를 계약오로 생각해 보아야 합니다. 이 계약서는
자료를 여러분의 클래스가 갖고 있고 여러분의 클래스는 어떻게 움직일 것

인가를 보여줍니다.

예를 들어, Cat 클래스 선언에서, 여러분은 다
즉, 모든 Cate 생성자에 : 해 초기화될 수

여러분이 만일 GetAgeNS 상수 함수로 했다면 - 물론 그랬어야 하지만 - 그 계약
서에는 GetAge(7} Cate] 값을 바꾸면 안된다고 쓰여있을 것입니다.

C++2 강형 언어(60008 typed 180084880)입니다. 이는 여러분이 이 계약을 어기면
컴파일러는 오류 메시지를 통해 이 ANS 강요하는 것입니다. [리스트 6.5]는
이 계약서를 위반하여 컴파일되지 않는 프로그램의 예를 보여줍니다.

[리스트 6.5]는 험파일되지 않습니다,

[리스트 6.5] 인터페이스 파기 예제 프로그램

1: // 컴파일러 오류 예
2
35


===== PAGE 169 =====
166 ee 제1주
4: #include <iostream.h>
뚜르
6: class Cat
(meet
8: public:
Os    CatCint initialAge);
10:   “CatQ;
11:   int GetAge() const; // 상수 접근작 함수
125   void SetAge(int age);
13%   void Meow();
14: private:
13s   int itsAge;
162 공오
0s
18: // 생성자
19: Cat::Cat(int initialAge)
20: ¢
218   itsAge = initialAge;
22:   cout << "Cat Constructor\n";
23: +}
24:
25: Catz: "CatQ)      // 소멸자
26: {
27:   cout << "Cat Destructor\n";
28: }
29: // GetAge, 상수 함수
30: // 그러나 상수 법칙을 어김
31: int Cat::GetAge() const
32: £
33: return CitsAget+); // 상수가 아니게 2
34: }
555
36: // SetAge 정의
371 // BS BS} 함수
38: // itsAge 멤버 반환
39: int Cat::SetAge(age)
40: {
41:    // itsAgeS age= 설정함
42:   //
43:   itsAge = age;
44: }
45:
46: // Meow 메쏘드 선언
47: // 반환값: void
48: // 매개 변수: 없음
49: // 하는 일 : Meow 33



===== PAGE 170 =====
제6일 기본                         ee 167

i
lu
0
1>

50: void Cat::Meow()

51: £

52°    cout << "Meow.\n";
535 2

54:

551 // 인터페이스를 파기히고
56: // 여러 가지의 오류 발생시킴
57: int main()

58: -£

59: Cat Frisky;        // AA 일치 않음
60:   Frisky.Meow();

61; ~ Frisky.BarkQ);      // 안 이루어짐

62:  Frisky.itsAge=7; // itsAge=E 전용임
63:   return 0;
64: }

(nus
1
=

(ag

이 프로그램은 컴파일이 안되므로 출력도 없습니다.

이 프로그램은 그 안에 오류가 많습니다. 11번 줄에서 064860를 상수 A
근자 함수로 선언하였습니다. - 그리고 그래야 합니다. 그런데 00800 함
수 몸체인 33번 줄에서 멤버 변수 16406가 중가하였습니다. 이 MALE 상수로
선언되었기 때문에 16486가 바뀌어서는 안됩니다. 따라서 이 프로그램이 컴파일
될 때 오류가 발생합니다.

a Bd Mendes 장주염으르 USA Wag ws ole oe she
라도 나쁜 프로그래밍 습관입니다. 훌륭한 설계는 이 메쏘드가 0#의 멤버 변
를 바꾸지 않는다는 점을 고려합니다. ie Bee 합니다.
줄은 Cato] 객체 ae ANS 보여주었습니다. Cat] 현재 생성자를 가졌
는데 정수형을 매개 변수로 갖습니다. 이는 여러분이 매개 변수를 전달해야 한다
는 것을 의미합니다 SH SANS 매개 변수가 없기 때문에 OHS 처리됩니다
61번 SL 메쏘드 80000를 호출합니다. 그런데 8000는 선언조차 안되어 있습니

7.

XG
m

n
Ne)
oo

다. 틀립니다.
62번 ZL 16400에 7이라는 We 할당하였습니다. itsAgee 전용 자료 멤버이기
때문에 프로                                ~

그램이 컴파일될 때 오류를 발생합니다.       ps vote


===== PAGE 171 =====
168 ee 제1주

왜 컴파일러를 SEE 잠기 위해 사용하는가?

100% 버그 없는

래머는 거의 없습니다. 그2

하여 최 sie!  AAAS 개발하는 것이었습니다.
나게 만들고 프로그래머의 명예를 훼손하는 것이지

러분의 프로그램은 실행시 깨질 것입니따. 아마 교수님이 혹은 직장 상사가 뒤에서 보고
있을 때 컴파일 오류 - 컴파일시 나타나는 오류 - 는 실행 오류(실행시 나는 오류) 보단
씬 OSUCH. 왜냐하면 컴파일 오류는 추측하기가 쉽기 때문입니다. 실행시 프로그램이
죽지 않고 여러 번 실행이 되는 경우가 많습니다. 왜냐하면 실행 오류는 잘 숨기 때문입니
다. 컴파일 SFE 컴파일할 때마다 나타납니다. 그래서 오류를 잡아내고 확인하기가 쉽습
0 프로그래머에게 실행 오류가 나타나지 않게 하는 것이 하나의 목표가 될 수 있습니
|. 컴파일러를 써서 미리 오류를 잡아내는 노력을 하는 사람은 이 SHS 성공시킬 수 있
ae

클래스 선언과 메쏘드 정의를 어디에서 할 컷인가

여러분이 여러분의 클래스를 위하여 선언한 A 함수는 정의를 지녀야 합니다. 정
의는 또한 함수 구현이라 부릅니다. 다른 함수와 깥이 클래스 메쏘드의 정의는
함수 표제와 함수 몸체를 가집니다.

AM 컴파일러가 찾을 수 있는 파일이어야 합니다. 대부분의 cH 컴파일러는
파일이 .0, CPP 끝나길 바라는데 이 책에서는 CPPS 사용합니다. 하지만 여러
분의 컴파일러를 검사해 보기 바랍니다.

=

* 4

많은 컴파일러는 Ce 끝나는 것은 6 포로그램이고 cH 프로그램은 crepe 끝나는 것
으로 알고 있습니다. ARS 어떤 sete 쓸 수도 있지만 cpt Ze 줄일 것
입니다.

여러분은 이 선언을 이 파일 안에 꼭 안 써넣어도 됩니다. 하지만 좋은 프로그램
습관이 아닙니다. 대부분의 프로그래머들이 사용하는 개념은 헤더 파일00840868
FILE) 이라는 ol 선언을 air ?  AMC. 헤더 파일은 H, HP, HPP 등으로

납니다. 이 AS 헤더 파일을 HPS 끝나는 것으로 하였지만 여러분의 컴파일
4% 참고하여 주기 바랍니다



===== PAGE 172 =====
Hol 기본적인 클래스 co 169

예를 들어, Cato] 클래스 선언을 CAT.HPPZHE 헤더 파일에서 선언하였고 클래
메쏘드는 CAT.CPP] 정의하였습니다. 그리고 헤더 파일을 047.0의 꼭대기
분에 적음으로써 CPP 파일에 포함시켰다.

=)
부

#include "Cat.hpp"

|도록 합니다. 마치 이

go               위치
러분이 그 USES 직접 입력한 것처럼 말입니다. 이를 다시 읽어 들일 것이면
도대체 왜 파일을 분리하는 것일까요. 많은 경우 여러분은 각 클래스의 상세한
구현에 대해 신경을 쓰지 않는 경우도 있습니다. 단지 헤더 파일을 읽음으로써
클래스의 선언 및 메쏘드 정의만 알고 파일의 상세 코드를 알 필요가 없는 경우
헤더 과일만 읽으면 됩니다

클래스 AAS 컴파일러에게 클래스가 무엇이고 그
수들을 가지는지를 알려줍니다. 클래스의 선언은 인
용                    가르쳐

작에게 그 클래스와 “rel 교신을 할지를

종종
#4 정의는 엄파일러에게 이볼기: 함수가 sper 알려줍니다. 함수 정의는 클래
A 메쏘드 구련이라고 불립니다. 이는 cpp 파일 안에 있습니다. 클래스의 상세한 구
He 단지 클래스를 만든 사람에게만 관심이 있습니다. 클래스의 클라이언트들 - 그
클래스를 쓰는 프로그램의 한 부분들 - 은 그 함수가 어떻게 구련되는지 알 필요가
없습니다

inline 구현

는 것처럼 여러분은 클래스 메쏘드를
반환형 앞에 나타납니다. GetWeight() 함

일반 함수에서 10106형 함수를 만들 수 있
inline= 할 수 있습니다. aeko} inline: 보
수의 inline 구현은 아래와 같습니다.

inline int Cat::GetWeight()
€

return itsWeight ;// Weight2| 자료 멤버를 반환

함수의 정의를 클래스 안에 YS 수도 있는데 이는 자동으로 함수를 106형으로
이이 오스 바기 이 이부또16
들


===== PAGE 173 =====
170 ee ANS

class Cat
{
public :

int GetWeight() { return itsWeight; } // inline
void SetWeight ( int aWeight ) ;
+;

GetWeight() 함수의 정의를 봅시다. inline 함수의 몸체가 클래스 메쏘드의 선언 바
로 뒤에서 시작합니다. 함수의 괄호 다음에 세미콜론이 없습니다. 다른 drs 같
이 정의는 시작 중괄호로 시작하여 마감 중괄호로 끝납니다. 보통 때와 마찬가지
로 공백은 문제가 되지 않습니다. 정의를 다음과 같이 써도 됩니다.

class Cat

it

public :

int GetWeight()
{

return itsWeight;
+ // inline
void SetWeight ( int aWeight ) ;
+;
[JAE 6.6|과 [리스트 OTS Cat SAAS 다시 만듭니다. 하지만 정의를
CAT.HPPol] 함수 구현을 041.02『에 만듭니다. [리스트 6.7] 역시 접근자 함수와
Meow() 함수를 10106으로 하였습니다.

[리스트 6.6] CAT.HPPONM Cat BAAD! 선언

1: #include <iostream.h>

2: class Cat

Ss   <

4: public:

Die   Cat (int initialAge);

6:   “CatQ);

ts     int GetAge() { return itsAge;}            // inline!
Se     void SetAge (int age) { itsAge = age;}    // inline!
05     void Meow() { cout << "Meow.";}           // inline!
10: private:

113   int itsAge;

2: };



===== PAGE 174 =====
제6일 기

rH
mPa
ro

! 클래스 ee 171

I>

[리스트 6.7] CAT.CPPONA Cat) 구현

// [리스트 6.73
Lf

1
2
3
4: #include "cat.hpp" // 헤더 파일 포함함

5: #include <iostream.h>

6  \

7: Catz:Cat(int initialAge)

Be

9:    itsAge = initialAge;

10: }

113

12: Cate:"CatO

1S: £

14: }

15°

16: // cat 생성

17』 77

18: int main()

19: £

20:   Cat Frisky(5);

21:   Frisky.Meow();

22:   cout << "Frisky is a cat who is" ;

235%   cout << Frisky.GetAge() <<" years old.\n";
24:   Frisky.Mewo();

251   Frisky.SetAge(7);

26:   cout << "Now Frisky is " ;

27:   cout << Frisky.GetAge() <<" years old.\n";
28:   return 0;

292 3

결    , Meow

Frisky is a cat who is 5 years old.
Meow
Now Frisky is 7 years old.

oy  [리스트 6.6]과 [리스트 6.7|에서 제안된 AEE [리스트 6.4]와 비슷합니다.
세 개의 메쏘드가 파일의 선언에서 inlineo 2 되었다는 점과 선언이 84007
로 나가있다는 점만 제외하고 말입니다.
GetAge= 7번 Zl] 있고 inline 구현되었습니다. 8, 9번 줄에서 14106 함수가
더 지정되었으나 실제 기능 면에서 40006이 아닐 때와 다를 것이 없습니다.


===== PAGE 175 =====
172 eo ANZ

[리스트 6.7]의 4번 SS “#include 080000”"를 보여주는데 |= cat.hppS  읽어 옵니
다. cathpp= 포함함으로써 여러분은 컴파일 Aol cathppS 마치 여러분이 써넣은
것처럼 SH Zo] 불러 들여옵니다.

이러한 기법은 선언부를 구현부가 있지 않은 다른 파일에 넣을 수 있게 하는데,
필요시 컴파일러가 사용하게 합니다. 이러한 기법은 0++에서 유용한 기법인데 선
언은 bpp, 해당 ANS Bee 하는 BEE 해당 cpp 함수에서 10006로 호출
합니다.

18부터 29번 줄은 [리스트 641의 main 함수를 반복합니다. 여기서 inline 함수로
해도 함수의 성능을 바꾸지 않습니다.

간단한 클래스를 선언하고 그 클래스를 좀더 복잡한 클래스의 선언에 포함시키는
복합 클래스를 만드는 것은 흔한 일입니다. 예를 들어, 바퀴의 클래스, 엔진 클래
스 등을 AMM 뒤 이를 자동차 클래스에 포함시킬 수 있습니다. 이 션언은 '
함"이라는 관계를 지니고 있습니다. 자동차는 자동차의 바퀴를 가지고 또 자동차
의 엔진을 가졌습니다

봅시다. 사각형은 선분으로 구성되어 있고 선분은 두 개의 점으로
의됩니다. 점은 ×축과 축으로 UAT. 베쓰 6.8]은 Rectangle 클래스
의 완전한 선언을 보여주는데 이는 RECTANGLEHPPo] 나타날 수 있습니다. At
은 4개으 = 연결한 4개의 선으로 정의되어 있고, 각각의 점들은 그래프
찾아질 수 있습니다. 우리는 먼저 각 점의 x y AHS 가지고 80

. [리스트 6이는 각 클래스의 완전한 선언을 보여줍니다.

[리스트 6.8] 완전한 클래스의 선언

// Rectangle.hpp 시작

#include <iostream.h>

class Point // x,y 가짐

£

// 기본 생성자 사용

public:
void SetX(int x) { itsX = x; }
void SetYCint y) { itsY = y; }
int GetX() const { return itsX;}

Oi    int GetY() const { return itsY;}

SP OANA UFWNDr =



===== PAGE 176 =====
제0일 기본적인 클래스 ee 173

11: private:

125    int 1tsx;

TS    Int Ttsy;

14: 3; // Point 클래스 선언의 B
15%

16:

17: class Rectangle

18: <

19: public:
20:    Rectangle (int top, int left, int bottom, int right);

21    “Rectangle () {}

22:

235    int GetTop() const { return itsTop; }

24:    int GetLeft() const { return itsLeft; }

25:    int GetBottom() const { return itsBottom; }

26:    int GetRight) const { return itsRight; }

YATES

28:    Point, GetUpperLeft() const { return itsUpperLeft; }
29:    Point GetLowerLeft() const { return itsLowerLeft; }

50%    Point GetUpperRight() const { return itsUpperRight; }

$1:    Point GetLowerRight() const { return itsLowerRight; }

522

55%    void SetUpperLeft(Point Location) {itsUpperLeft = Location;}
54:    void SetLowerLeft(Point Location) {itsLowerLeft = Location;}
S58    void SetUpperRight (Point Location) {itsUpperRight = Location;}
56°    void SetLowerRight(Point Location) {itsLowerRight = Location;}
SC:

58:    void SetTop(int top) { itsTop = top; }

595    void SetLeft(int left) { itsLeft = left; }

40:    void SetBottom(int bottom) { itsBottom = bottom; }
41:    void SetRight(int right) { itsRight = right; }

42:

43:    int GetArea() const;

44:

45: private:

46:    Point itsUpperLeft;
47:    Point itsUpperRight;
48:    Point itsLowerLeft;
49:    Point itsLowerRight;
50:    int itsTop;

5    int itsLeft;

52:    int itsBottom;

53:    int itsRight;

548 Fe

55: // 글



===== PAGE 177 =====
174 ee Is

[리스트 6.9] RECTANGLE.CPP

1
2
3
4:
Ble
6
7
8

9:

10:
11
12:
13:
14:
15:
16:
Ts
18:
19:
20:
21:
22:
25%
24:
25:
26:
20%
28:
29:
30"
Sle
32:
S52
34:
55:
56:
Ss
58:
59:
40:
41:
42%
43:

#include "rect.hpp"
Rectangle::Rectangle(int top, int left, int bottom, int right)
£

itsTop = top;

itsLeft = left;

jitsBottom = bottom;

itsRight = right;          (20, 120)             L bo, we)

       1
jtsUpperLeft.SetX(left);     \              |
itsUpperLeft.SetY (top);       { 기
itsUpperRight.SetX(right);
itsUpperRight.SetY (top);

itsLowerLeft.SetX(left);
itsLowerLeft.SetY (bottom) ;

itsLowerRight.SetX (right);
itsLowerRight.SetY (bottom);

“a  ㅁ
//
int Rectangle::GetArea() const
ce

int Width = itsRight - itsLeft;
int Height = itsTop - itsBottom;
return (Width * Height);

int main()
{
// Rectangle 변수 초기화
Rectangle MyRectangle (100, 20, 50, 80);

int Area = MyRectangle.GetArea();

cout << "Area: " << Area << "\n";

cout << "Upper Left X Coordinate: ";

cout << MyRectangle.GetUpperLeft() .GetX();
return 0;



===== PAGE 178 =====
제6일 기본적인 클래스 ee 175

개 Area: 3000
결과  Upper Left X coordinate: 20
way |  [리스트 6.8]의 3 - 14번 SO i Point ©] 션언인데 그래프상의 x, y 좌
~ 。 표를 가집니다. as  이 프로그램은 PoinkS 쓰지 않습니다. 하지만 다
= 그리기 메쏘드는 Points 필요로 sat

Point 클래스의 선언 안에는 두 개의 멤버 변수 - 19%, 18? - 를 12, 13H 줄에서

선언하였습니다. 이 변수들은 좌표값들을 가 251 있습니다. x 좌표가 증가함에 따
라 그래프의 오른쪽으로 이동합니다. 좌표가 증가함에 따라 그래프의 위쪽으로
이동합니다. 다른 그래프들은 다른 시스템을 $Ud. 어떤 윈도우 프로그램에서는
》좌표를 증가시킴에 따라 윈도우 안에서 아래로 내려갑니다.

Point 클래스는 x 》의 값을 설정하고 PSHE inline 접근자 BES 사용합니다.(7
- 10번 줄) 따라서 여러분은 그들의 FES 명시적으로 설정해야 합니다.

ITH 줄은 Rectangle 클래스의 선언을 시작합니다. #6000816는 사각형의 4좌표를
구성하는 4개의 점들로 구성되어 있습니다.

860080916의 생성자는 20번 on ana 정수행을 갖는데 100, left, bottom, right=

갖습니다. 생성자에게 4개의 ASE [리스트 6의에서 4개의 매개 변수로 복사되
고 그러면 4개의 Point7} 모  보기 i,

일반적인 접근자 함수 이외에도 #6000916는 함수 08647680를 43번 줄에서 가집니
다. WAS Wee 저장하는 대신 [리스트 OA 00160 함수는 27 - 29번 줄
에서 면적을 계산합니다. 면적을 구하기 위해 밑변과 Sols 구하고 두 WS 곱
합니다.

사각형의 좌상 점의 *좌표를 구하기 위해 여러분은 좌상 점을 접근한 후 그 *×좌
표를 구합니다. 08[46680는 Rectangle®] 메쏘드이기 때문에 Rectangle2] 전용 자료
So 직접 접근할 수 있고 16070001.@도 접근할 수 있습니다. 16000600.08는 Point
이고 80따의 itsX 값은 전용이기 때문에 GetAreaQi= 직접 이 자료에 접근할 수가
없습니다. 그보다는 범용 접근자 함수 GetXS 사용하여 ARS 구합니다.

[리스트 6.9]의 32번 줄은 실제 프로그램의 몸체 BH] 시작입니다. 35번 줄 전
까지는 메모리가 할당되지 않았고, 아무 일도 일어나지 않습니다. 여러분이 한 일
은 컴파일러에게 어떻게 Points} Rectangles 만드는 지입니다.

35번 줄에서 100, left, bottom, right 전달하여 여러분은 Rectangles 정의하였습니
다. 37번 줄에서 지역 변수 Aras 정수형으로 선언하였습니다. 이 변수는

fA


===== PAGE 179 =====
176 ee ANF

Rectangle®] WAS 갖습니다. 여러분은 AreaS] gt Rectangle2] GetArea() 함수를
이용하여 구합니다.

Rectangle] 클라이언트는 86080916의 객체를 만들고 GetArea®| 구현은 모르는
상태에서 면적을 구할 수 있습니다.

RECT.HPP [리스트 6.8]에 나와있습니다. 헤더 파일을 보면서 프로그래머는
GetAreaQi= 정수형을 반환함을 알 수 있습니다. 어떻게 0044680가 그런 AS 하
는지는 #\600096는 전혀 관심이 없습니다. 사실은 #60080816의 소유자는 Rectangle
의 사용자에게 영향을 미치지 않은 al) GetAreaQS 바꿀 수 있습니다.

“12 Al(Structure)

클래스 예약어와 매우 가까운 사촌이 바로 struct 예약어인데 구조체를 선언할 때
쓰입니다. 0++에서 구조체는 0099와 똑같으며 단지 그 wwe 기본적으로 범용이
라는 점이 다릅니다. 여러분은 006를 선언하는 것과 똑같은 방법으로 구조체를
선언하고 또 똑같이 AE wus 함수들을 SF 있습니다. 사실 여러분이 클래
스 선언에서 정확히 전용과 범용 부분을 가릴 줄 아는 좋은 프로그래밍 습관을
ACA 클래스와 구조체 중 어떤 것을 써도 관계가 없습니다.

[리스트 6.8|에서 다음 부분을 바꿔서 입력하여 봅시다.
Hi 3 줄 0056 Point struct Point 바꿈니다.
Mi 17H & class 『6000016를 struct 『6000016로 바꿈니다.

프로그램을 다시 컴파일하여 실행시키고 출력을 비교하여 봅시다. 변화가 없을
것입니다.

왜 두 개의 예약어는 같은 일을 할까요?
왜 두 개의 예약어는 같은 일을 하는지 의아해 할 것입니다. 이는 역사적인 유래
가 있는 것입니다. 0++가 처음 개발되었을 때 0++은 Co} 확장으로서 만들어졌습
니다. Ce FAAS 가지고 있지만 클래스 메쏘드를 갖지 않았었습니다. 반 스트
라우스트럽(02++의 창시자)은 struct 위에 더 기능을 SARE 새로운 개념의 classe}
는 것을 만들었습니다.



===== PAGE 180 =====
to
Ie

오늘 여러분은 클래스라 불리는 새로운 YS 만드는 We 배웠습니다. 이 새로운
형의 변수들을 정의하는 YS 배웠는데 이를 객체라 부릅니다

클래스는 자료 WAS 갖는데 이는 여러 형들의 변수이고 다른 클래스도 Kae
니다. 클래스는 멤버 함수도 갖는데 메쏘드로 알려져 있습니다. 이 멤버 함수는
멤버 ARES 연산하고 다른 서비스도 하기 위해 만듭니다

클래스 멤버(자료와 함수)는 전용이거나 범용입니다. 범용 멤버는 여러분의 프로
그램의 어느 부분에서도 접근 가능합니다. 전용 멤버는 해당 클래스의 멤버 함수
들만 접근 가능합니다.

래스의 인터페이스(혹은 선언)를 헤더 파일에 나누어 두는 것은 좋은 프로그래
J satay. 이런 파일은 HPP 확장자로 끝납니다. 클래스 메쏘드의 Pao
CPP 확장자로 끝나는 파일에 저장합니다.

클래스 생성자는 객체를 초기화합니다. 클래스 소멸자는 객체를 없애고 그 클래
스의 메쏘드에 의해 할당된 메모리를 풀어놓습니다

fu

o

N

oD 때
of

Q&A
Q 클래스의 객체는 얼마나 BLY}?
A 클래스의 객체의 메모리에서의 크기는 그 멤버 변수들의 크기의 합에 의해 agg
니다. 클래스 메쏘드는 그 개체를 위해 마련한 메모리에서 자리를 차지하지 않습
니다.
어떤 컴파일러는 Whole 변수들이 실제 2바이트 이상의 메모리를 잡도록 메모리

상에 변수들을 정렬하곤 합니다. 여러분의 컴파일러 사용 안내서를 확인해야 하는
데, 이 시점에 있어서는 그리 관심을 가질 필요는 없습니다.


===== PAGE 181 =====
178 ee

제1주

Q

전용 멤버 itsAge= 가진 클래스 Cats 선언하고, 그 (하의 두 개의 객체 FriskySt
Boots= 만든다면 Boots 『「19!의 itsAgedl 접근할 수 있습니까?

A 가능합니다. 전용 ABE 클래스 멤버 함수에 의해 접근할 수 있고, 클래스의 각기

다른 인스턴스(실체 부분)들이 다른 자료에 접근할 수 있습니다. J, FriskyS} Boots
가 둘 다 Cato] 인스턴스라면 8090/의 멤버 함수로 8096와 8006의 자료에 접근할

멤버 자료를 전용으로 하면 클래스의 클라이언트들이 어떻게 그 자료가 저장되고

계산하는지 걱정할 필요 없이 사용할 수 있습니다. 예를 들어, Cat 클래스가

061&860라는  미조  쏘드를 가지고 있다면 Cat ae pilin      고양이의 나이
고 계      알지 못해도 그

Q const 함수를 만들고 함수를 바꾸면 컴파일러 오류가 납니다. CFS 피하려면 0005

를 빼야합니다. 그 이유는?

A 만일, 여러분의 멤버 함수가 SAAS 바꾸지 않는다면 예약어 constS 쓰는 것은

좋은 습관입니다. 왜냐하면 컴파일러가 오류를 찾아주기 때문입니다. 예를 들어,
GetAge()7} Cato] 클래스를 바꿀 이유가 없고, 여러분의 프로그램은 다음 줄을 가진
경우를 봅시다.

if ( itsAge = 100 )cout << "Hey! You're 100 years ild\n"

GetAgeQ= const® 선언하면 이 REE OFS 발생시킴니다. 15486가 100인지 검
사하려하였으나 여러분은 100을 15486라는 값에 대입하고 말았습니다. 이 과정에서
클래스를 바꾸었기 때문에 - 여러분은 이 메쏘드가 SAAS 바꾸지 않는다라고 착
각했습니다 - 컴파일러는 오류를 HoH.

이러한 종류의 실수는 찾아내기 힘듭니다. - 인간의 눈은 종종 무엇이 일어나리라

도 기대한 코드로 보아버립니다. 더욱 중요한 것은 이런 경우에
가 안 난다면 프로그램은 잘 돌아가고 15486는 틀린 값으로 되어 버
릴 것입니다. 이 경우 언젠가는 장애가 발생합니다.

C++ 프로그램에서 구조체를 쓸 이유가 있습니까?

많은 프로그래머들이 함수 없는 class 대신에 쓰려고 struct 예약어를 사용합니다. 이
옛날의 함수를 갖지 않은 0로의 퇴조입니다. 사실 저자는 구조체가 때로는 혼동
고 좋지 않은 프로그래밍 습관이라는 것을 알았습니다. 오늘 메쏘드 없는 구조
내일 메쏘드를 Bee 할 것입니다. 이럴 경우 여러분은 005의 형태를 바꾸
ct9] 메쏘드를 갖게 해야 하는 두 가지 중 하나를 선택해야 할 것입니다.

© 가



===== PAGE 182 =====
세6일 기본적인 클래스 ee 179

연구

El 32 때

oO

ㅣ 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가

확인해 보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어

SUE: 부록 Del 있는 답을 보기 전에 각 물음에 대답을 할 수 있도록 노력하
, 다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다

퀴즈

표 점 연산자란 무엇이고 왜 Buy}?

2 언제 메모리를 준비하여 SLA? - 선언할 때입니까? 아니면 정의할 때입니까?

3 SAHA AAS 인터페이스입니까 아니면 구현입니까?

4 전용 자료 AHS 범용 자료 멤버의 차이점은 무엇입니까?

$ 멤버 함수는 전용으로 될 수 있습니까?

6 멤버 자료는 범용입니까?

7 Cat 객체를 두 개 만들 때 그들은 각기 다른 6406 멤버 ABS 가질 수 있습니까?
8 01855 선언은 세미콜론으로 끝납니까? 클래스 메쏘드 정의는 어떠합니까?

% Cat 클래스의 헤더 함수 /60\/(매개 변수가 없고 voids 반환하는)는 어떻게 표현합
니까?

10. 클래스를 초기화하기 위해 어떤 함수가 호출됩니까?

연습 문제

1. Age, YearsOfService, SalaryS 자료 멤버로 갖는 ㄷ70601066라 불리는 클래스를
써봅시다.

% 자료 멤버들을 전용으로 하는 Employee 클래스를 다시 작성하여 봅시다. 그리고 자료
멤버를 설정하고 가져오는 범용 접근자 메쏘드를 작성하여 봅시다.

3 + 명의 Employees 만드는 Employee 클래스를 작성하고 그들의 Age,
YearOfService,  SalaryS 설정하고 출력합시다.

4 3H 문제에서 고용인의 ASS 출력하는 프로그램을 작성하여 봅시다. 단 금액은 1000
단위로 자릅니다.

5. Employee 클래스를 수정하여 여러분이 고용인을 만들 때 Age, YearsOfService,
SalaryS 초기화합시다.


===== PAGE 183 =====
180 ee AIF

6 버그잡기 :

class Square
5g
public :

int Side;
}

7. 버그잡기 :

class Cat
t
int GetAge() const;
private:
int itsAge;
3;

8 버그잡기 :

class TV
€
public:
void SetStation (int Station);
int GetStation() const;
private
int itsStation;

3;

int main®)

te
TV myTV;
myTV.itsStation = 9;
TV.SetStation(10);
TV myOtherTv(2);
return 0;



===== PAGE 184 =====


===== PAGE 185 =====
182 ee 제1주

서문
프로그램은 분기와 순환을 통해 그 대부분의 기능을 수행합니다. 4일째 되는
여러분은 여러분의 프로그램이 어떻게 FES 써서 분기하는지를
늘 여러분이 배울 내용이 아래에 있습니다.

B Sates 무엇이고 어떻게 쓰이는가?

를 여러 가지 다양한 순환문 만들기

를 꾸게 중첨된 |/6656 문장에서의 대안

많은 프로그램 문제들을 같은 자료에 대해 반복적으로 수행을 함으로써 풀어나가
는 방법이 있습니다. 두 가지 방법이 있습니다. 자기 호출(이미 배웠음)과 반복
(iteration) 통해서입니다. 반복이란 같은 일을 계속해서 한다는 뜻입니다. 반복의
기본 방식은 순환입니다.

순환문의 조상 : goto
컴퓨터 과학의 아주 초기시대에는 프로그램이 아주 지저분하고 구질구질하고 a
았습니다. 순환은 라벨, 문장들 그리고 점프문으로 이루어졌었습니다.
CHA] 라벨이란 특정이름을 쓰고 꺼기에 콜론(:)을 붙이는 식으로 되어 있습니
다. 라벨은 C++ 문장의 AF] 위치하고 한편 pened goto 다음에 라벨이름을
씀으로써 이루어집니다.

[리스트 7.1] ASO 0010와 함께 쓰여진 순환

// [리스트 7.17 예약어 60+0와 함께 쓰여진 순환문
//

#include <iostream.h>

x
int counter = 0;    // initialize counter
Sah counter ++;      // top of the loop
cout << "counter: " << counter << "\n";

1

2

3

4

DY

6: int main()
7:

8

9

1

1     if (counter < 5)    // test the value

ie



===== PAGE 186 =====
제7일 프로그램 흐름 ee 183

124      goto loop;       // jump to the top

13:

145   cout << "Complete. Counter: " << counter << woh
15:   return 0;

16% 3

결과  counter:

counter:
counter:
counter:
counter:
Complete. Counter: 5.

ues Dr oS

분석  8번 SA] counters 0으로 초기화되었습니다. 라벨 loop: 9번 So] 있는
데 top of the 100?이라는 주석문이 붙어 있습니다. counter=E 하나씩 증가하
고 그 Se] 출력됩니다. 0000@의 Be 11번 줄에서 검사됩니다. 5보다 작으면
ifr 참이 되고 800문이 실행됩니다. 이는 프로그램 Ago] ow 줄로 가
합니다. 이 프로그램은 0040@가 5가 될 때까지 순환되고 이때가 되면 순환
빠져 나와 마지막 결과가 출력이 됩니다.

왜 gotom®| 기피되는가?

최근 들어 800는 다소 좋지 않다고 여겨지는데 그럴만한 이유가 있습니다. goto
문은 여러분의 프로그램에서 앞뒤 어떤 위치로도 점프를 할 수 있게 합니다. 이
무차별적인 800의 사용은 엉키고, 읽기 어렵고, 한마디로 골치 아픈 '엉킨 실타래
코드'를 만들어 냈습니다. 바로 이러한 이유 때문에 지난 20년간 컴퓨터 공학 교
사들은 학생들의 머리가 마르고 PEs 다음을 교육시켰습니다. “절대로, 무슨 일
이 있어도, 제발 goto 쓰지 마시오. 그것은 죄악입니다”

8000문을 피하기 위해 매우 기교적이고, 잘 통제된 순환문들이 도입되었습니다.
for, while, do...whileo] 그것들입니다.  이들을 쓰면 프로그램이 좀더 이해하기 쉬워
집니다. 8000문은 잘 피해질 수 있습니다. 하지만 혹자는 이런 상황이 다소 과장
되었다고 주장하기도 합니다. 다른 도구들과 마찬가지로 잘 그리고 정확히만 쓰
인다면 800문은 아주 훌륭한 구조물이 될 수 있다고 합니다. 하지만 이를 맘대로
쓰지 BANC.


===== PAGE 187 =====
184 ee 제1주

9010문
gotoS 쓰기 위해 00[0문 다음에 라벨 BS Buch. 사실 이 때문에 무원칙한 점프가 일
어납니다.
예제
if (value > 10)
goto end;
if (value < 10)
goto end;

cout << "value is 10!";
end:

cout<< "done";

aS
ai

while =LE
while 순환문은 시작조건이 참인 동안 반복해서 특정문들을 반복 수행하게 합니
다. 800문의 예에서([리스트 7.1) counter= 57} 될 때까지 증가되었습니다. [리스
트 7.2]는 같은 프로그램을 while 순환문을 써서 다시 작성하였습니다.

[리스트 7.2] while 순환문

// [리스트 7.23 while 순환문
//

#include <iostream.h>

《

1

2

3

4

58

6: int main()
7

8     int counter = 0;     // conditions 초기화
9

1

0:  while(counter < 5)    // condition 검사값이 참이면



===== PAGE 188 =====
제7일 프로그램 흐름 ee 185

별   te

12:       countertt;          // 순환문 본체

135%      cout << "counter: " << counter << "\n";

14:   +

1s

165   cout << "Complete. Counter: " << counter << TN" 고
17:   return 0;

18: +

결과  counter:

counter:
counter:
counter:
counter:
Complete. Counter: 5.

분석 이 간단한 프로그램은 \406문의 기본을 보여줍니다. 조건이 검사되고 그

조건이 참이면 \006 순환문의 몸체가 실행됩니다. 이 경우에 있어서는 조

건이 10번 줄에서 검사되는데 counter7} 5보다 작은가 하는 검사입니다. 조건이

참이면 순환문의 몸체가 수행됩니다. 12번 SoA] counters 증가되고 13번 줄에

서 ao] 출력이 됩니다. 10번 줄의 조건문이 실패하면60406@가 5보다 더 이상 작

지가 않다면) while 순환문의 몸체 전 부분(11부터 14번 줄까지)이 생략되게 됩니
다. 프로그램은 15번 줄로 가게 됩니다.

Ue 4 60 =

while=

while (   (조건문>

eel;

조건문은 어떠한 C++ 수식이어도 관계없고, 문장 12 + +상의 문장 또는 블록문이면
됩니다. 조건문이 참(1)으로 BAYH 문장 1은 실행되고 조건문이 다시 검사됩니다. 이
HAS 조건문이 ARCS 판명될 때까지 계속 수행됩니다. 그리고 whilese 종료되고
문장 1 다음의 문장으로 넘어갑니다.
예제

//count to 10
int x = 0;
while ( x<10)
cout << "x: "<< x+4+;



===== PAGE 189 =====
186 ec 제1주

다소 복잡해진 whilez

whileo]]

다. 이는 EQNS &&, 논리합 |, 부정|! SI 연산자를 써서
다. [리스트 7.3]은 다소 복잡해진 ”016문을 Bos

의해 검사되는 조건은 다른 0++의 수식문들처럼 복잡해질 수가 있
ㅁ             ]

=

[리스트 7.3] 복잡한 while S22

1: // [리스트 7.33 복잡한 while 순환문

2: //

3:

4: #include <iostream.h>

Dd

6: int main(

78 £

8:    unsigned short small;

9:    unsigned long Large;

10's   const unsigned short MAXSMALL=65535;
VW:

12:    cout << "Enter a small number: ";

15   cin >> small;

14:    cout << "Enter a Large number: ";

15%   cin >> Large;

16:

171   cout << "small: " << small;

18:

19:  // 매 순환마다 세 가지를 검사함

20: while (small < Large && large > 0 && small < MAXSMALL)
215   {

22:      if (small % 5000 == 0) //5,0008 일 때마다 점을 찍음
235        cout << "호

24:

25:     small+t;

26:

Zt:     large-=2;

28:   }

29;

50:   cout << "\nSmall: " << small << " Large: " << large << endl;
Sa:   return 0;

52: }

24 Dh  Enter a small number: 2

Enter a Large number: 100000
Smalls Zia wn ne
Small: 33335 Large: 33334



===== PAGE 190 =====
제7일 프로그램 흐름 ㅎㅎ 187

설  이 프로그램은 게임입니다. 두 개의 숫자를 입력하는데 하나는 작고 하나는
BUC. 작은 숫자는 하나씩 커지고, 큰 숫자는 두 개씩 작아집니다. 이 게

임의 목적은 두 개의 숫자가 만나는 점을 추측하는 것입니다.
12 - 15번 줄에서 숫자는 입력됩니다. 20번 SS 1046문을 정하는데 다음의 세
가지 조건 BES 만족해야 수행이 됩니다.

I. smallO| 13「96보다 크지 않아야 한다.

2 large= 음수가 아니어야 한다.

3% 작은 FE small 정수형의 크기를 벗어나서는 otelct. (MAXSMALL)

00
J

22번 줄에서 9081의 값은 5.000의 나머지 연산을 하였습니다. 이 dake smalls}
값을 바꾸지는 않습니다. 하지만 이 수식은 small Zo] 정확히 5.000으로 나누어
떨어질 때 0 RS 반환합니다. 그럴 때마다 점(.)이 화면에 출력되어 상태를 보여
줍니다. 25번 줄에서 9001은 하나 증가되었고 large 둘씩 감소되었습니다.
\00문에서 세 개 조건 중 하나라도 실패하면, 순환문은 끝나고 프로그램의 실행
은 while 블록이 끝나는 28번 줄 다음으로 넘어갑니다.

나머지 연산자(%)와 복합 조건문은 3일쩌 공부 “Meo 상수"에서 언급되었습니다.

continue2} break
여러분이 프로그램 SS whileFo] 몸체를 다 실행하기 전 \416문의 꼭대기로 가
고 싶은 경우가 있습니다. 0000006는 \00문의 꼭대기로 점프시키는 문장입니다.

또 때때로 여러분은 종료 조건을 만나기 전 순환문을 종료하고 싶은 때가

one
Maa
것입니다. 06@문은 즉시 while 순환문을 벗어나게 하고 프로그램은 마감 중괄호

[리스트 7시는 이 문장들의 사용법을 보여줍니다. 이번에는 게임이 좀더 복잡해
습니다. 프로그램은 역시 작은 숫자와 큰 숫자, 건너 될 숫자와 0088 숫자를
HAG 것을 요구합니다. 작은 숫자는 하나씩 증가하고 큰 숫자는 둘씩 감소됩니
다. 감소는 작은 숫자가 건너 GB 숫자의 배수가 될 때마다 생략됩니다. 게임은 작
은 숫자가 큰 수보다 커질 때 종료됩니다. 만약 큰 수가 target] 정확히 도달하게

문장이 출력되고 AMS 끝납니다.


===== PAGE 191 =====
188 ee Ae

[리스트 7.4] break9} continue

1: // [리스트 7.43 break& continue

ee //

St

4: #include <iostream.h>

Dt

6: int main()

Tae €

8:    unsigned short small;

9:    unsigned long large;

10:   unsigned long skip;

VT:   unsigned long target;

12%   const unsigned short MAXSMALL=65535;
13%

14:    cout << "Enter a small number: ";

15   cin >> small;

16:    cout << "Enter a large number: ";

ara   cin >> large;

18:    cout << "Enter a skip number: ";

195   cin >> skip;

20:    cout << "Enter a target number: ";
218   cin >> target;

eee

eo   cout << "나";

24:

25: // 순환을 멈추는 3가지 경우를 설정함

26:   while (small < Large && Large > 0 && small < MAXSMALL)
2c:   {

28:

29:     small++;

30:

SV:      if (small % skip == 0) // skip the decrement?
32      x

338        cout << "skipping on " << small << endl;
34:        continue;

35°     ey

36:

37:      if (large == target) // target} 정확히 같은가?
38%     {

398?        cout << "Target reached!";

40:        break;

41:      BE

42:

43:     large-=2;

44: }        // while #22 2

~
al



===== PAGE 192 =====
제7일 프로그램 흐름 ee 189

46:   cout << "\nSmall: " << small << Large: " << large << endl;
Af:    return 0;

48: }
Enter a small number: 2                               ^
aX
Enter a large number: 20                            X  NG
Enter a skip number: 4                          wit 420    4,
Enter a target number: 6                      on         @
skipping on 4                                        gr

skipping on 8
Small: 10 Large: 8

분석  이 게임에서 large7} target 숫자 6을 만나기 전에 9001이 1086보다 커졌습

니다. 26번 줄에서 while 조건이 검사됩니다. 만일 small°] large tt} 작고

large7} 0보다 크고, smallo] MAXSMALL#t} 정수형보다 4° while 순환문의
몸체가 실행이 됩니다.

31번 줄에서 9001값이 907값에 의해 나머지 연산됩니다. smallo] 902의 정확한
배수가 되면 0000006문을 만나게 되고 프로그램의 실행은 26번 Zo] 순환문의 꼭
대기로 갑니다. 이때 targets} 같은 값인지 검사하는 과정과 largeS 2만큼 감소ㅅ
키는 과정이 생략됩니다.

38번 줄에서 larges} target? 검사됩니다. 두 개의 수가 같다면 메시지가 출력되고
break UC}. 이는 while 즉시 빠져 나오게 하는 계기가 되고 프로그램의 실
행은 46번 줄로 갑니다.

00 ath break= 주의하여 써야합니다. NES goto 다음으로 위험
= 9060의 경우와 같습니다. 갑자기 진로를 제멋대로 바꾸는 프로
래하기 어려운 프로그램이 됩니다. continues break 때문에 아주 조그

독 못하는 경우가 많습니다.

JR

pach

continue=
continue  whileZOl|-+ 10[문에서 2+ 순환문의 꼭대기로 가게 합니다
예제

[리스트 7.43엑 continue2| 예제가 있습니다.



===== PAGE 193 =====
190 ee AF

break=

break: while@ 또는 for
니다.

예제

while (조건 1)
{

문의 끝

if (271 2)
break;
// 문장들

로 가게 합니다. 실행은 마감 중

까지  세는

[리스트 7.5] while ( 1 ) 순환

vio
ce

6

이 구문을

.으
it

식이면 됩니다. 그 수식이 Be
숫자 1을 넣
}이기 때문에 068&(문을

끝없는

사용하여

=

：  =

=

1

// [티스트 7.53 while (1)
AD

#include <iostream.h>

1
2
3
4
Ds
6: int main®

areas?

8     int counter = 0;
Or

10:   while (1)

113   {
12[

13

14:

15%   }
16:   cout << "Counter:
103   return 0;

18: 2

counter ++;
if (counter > 10)
break;

" << counter << "\n";



===== PAGE 194 =====
제7일 프로그램 흐름 ce 191

분석  10번 줄 while 순환문은 결코 거짓이 될 수 없는 값으로 지정되어 있습니

다. 순환문은 0000@를 12번 줄에서 하나 증가시키고 13번 줄에서 counter7}
는지를 검사합니다. 아직 안 넘었으면 \06문은 계속 돕니다. 0040@가

되면 14번 줄에서 breakS 만나 \06문을 끝내게 됩니다. 프로그램

의 AVS 16번 줄로 넘어가고 거기에서 결과물이 출력됩니다.

이 프로그램은 돌기는 하지만 그리 예쁜 모양은 아닙니다. 이 프로그램은 좋지

않은 표본이기도 합니다. counters whileHo] 넣어 AAS 검사해도 됩니다.

DON'T

DON'T goto@S 쓰지 Bf ]=F,

DO     조건이 참인 Foret 순환문을 SEE whileRS 만듭시다
00     continueS} breakS 쓸 Well 주의를 합시다.
DO     순환문은 AME 끝나게 만듭시다.

do...while PLE

\00문의 몸체가 실행이 안되게 할 수 있습니다. while 다음 문장이 실행되기
전 먼저 조건문을 검사하는 것입니다. 만일 조건문이 거짓으로 판명되면 while 순

환문 전체가 생략될 것입니다. [리스트 7.6|이 이 예를 보여줍니다.

[리스트 7.6] while= 전체를 뛰어넘기

// TRAE 7.6] AM] 거짓일 때 whilee 전체를 뛰어넘기
//
//

#include <iostream.h>

int main()
{

CONDU FWD =


===== PAGE 195 =====
192 ee ANF

9°:    int counter;

10:   cout << "How many hellos?: ";
1:   cin >> counter;

12:   while (counter > 0)

13%   {

1G      cout << "Hello!\n";

1094     counter--;

16:   }

1c   cout << "Counter is OutPut" << counter;
18:   return 0;

198 개

결    How many hellos?: 2
Hello!
Hello!

Counter is OutPut: 0

How many hellos?: 0
Counter is OutPut: 0

분석 10번 줄에서 프로그램은 시작값을 입력받습니다. 이는 정수형 변수 counter
=" of 저장됩니다. 00006는 12번 줄에서 검사 받고 \46문에서 감소됩니다.
counter7} 처음에 2로 설정되었을 때 while 두 번 수행됩니다.

그런데 두 번째 실행할 땐 사용자가 of 입력했다고 합시다. 0000의 ge 12번
줄에서 검사되고 그 ASHE 거짓으로 됩니다. 0000@는 0보다 크지 않습니다. 전
체 '0416문은 건너뛰고 4610는 출력되지 않습니다.

hello7} 항상 적어도 한번은 출력되게 하려면 어떻게 해야 합니까. \46문은 이것
을 수행하지 못합니다. 왜냐하면 조건문은 출력 전에 검사되기 때문입니다. 여러
HO whiled-o] 들어가기 전 문을 써서 최소값을 강제로 넣을 수도 있습니다.

|

if ( counter < 1 )// 최소값을 강제로 넣음
counter = 1;

하지만 이런 AS 보고 “음! 아직 AMM 이라고 표현합니다.

do...while
환문은 조건문이 검사되기 전 순환문의 몸체를 실행하고 따라서 적어
도 몸체가 한 번은 실행이 됩니다. [리스트 7712 앞의 프로그램을 00..\06을 써
서 다시 보여줍니다.



===== PAGE 196 =====
제7일 프로그램 흐름 ee 193

[리스트 7.7] 00...41116의 예

1   // [리스트 7571 do... while] 에
2   //

5

4:  #include <iostream.h>

De

6: int main()

7   {

8     int counter;

Oe     cout << "How many hellos? ";
105    cin >> counter;

11s    do

121    £

15:      cout << "Hello\n";

14:      counter--;

155    } while (counter >0);

16:    cout << "Counter is: " << counter;
17: return 0;

18, 3

결Ｌ    How many hellos?: 2
Hello!
Hello!
Counter is: 0

분석 9번 줄에서 프로그램은 횟수를 입력하라고 합니다. 이는 B+} counters]
저장이 됩니다. 00..040866 순환문에서 조건이 검사되기 전 순환문이 수행되
고, 따라서 적어도 한번은 수행되도록 보장받습니다. we 줄에서 메시지가 출력
되고 14번 줄에서 0000@는 감소되고 15번 줄에서 조건이 검사됩니다. 조건이 참
으로 판명되면 AVS 13번 줄의 순환문의 꼭대기로 올라갑니다. 그렇지 않으면
16번 줄로 넘어갑니다.
0000006와 break 문장은 00..04416문에서도 사용할 수 있습니다. 1\04416문과
do...while# 2] 차이점은 조건문이 검사되는 시점입니다.

do...while=
do

문장

while (AWB) ;


===== PAGE 197 =====
194 ee AIS

행되고 조건이 검사됩니다. 만일 조건이 참이면 순환문이 반복되고, 그렇지 않으
on

문장이 실
면 순환문은 끝납니다. 그 외의 점을 제외하고는 문장과 조건은 \1110문과 동일합니다.

예제 1
// 10까직 세기
int x = 0;
do

COUE KS UXS "SS xtt;
while (x < 10)

예제 2
// 소문자를 줄력함

char ch = ‘a';

do

+f
cout << 이 74%
cht+;

} while ch <= "2" doy

:         DON'T
00 순환문이 적어도 한 번 실행되게 하기 위해서는 do... while BS 사용합니다.
00 조건이 거짓일 때 AALS 실행하지 않으려면 4006문을 사용합니다.
DO 여러분이 기대한대로 순환문이 작동하는지 항상 검사하십시오.

for Zee
‘while-S 프로그래밍 할 때, 여러분은 종종 시작조건을 초기화하고, 4 조건이
참인지를 검사하며, 또 변수를 각 순환문이 실행될 때마다 변화시킴니다. [리스트
7.8]이 이러한 예를 보여줍니다.

[리스트 7.8] while@S 다시 봅시다.

// [리스트 7.8] 비116문을 다시 봅시다.
il

1

2

5:

4: #include <iostream.h>
5:

6

int main®



===== PAGE 198 =====
제7일 프로그램 흐름 ce 195

tT? <

Se    int counter = 0;

Or

10:   while(counter < 5)

12   {

125      countertt;

135     cout << "Looping! ";
14:   }

15

16:   cout << "\nCounter: " << counter << ".\n";
173    return 0;

1S: +

겔과 Looping! Looping! Looping! Looping! Looping!
Counter: 5.
분석  조건문이 BH SoA, 설정되는데 00006@ 값이 0으로 초기화가 됐습니다. 10
~ 번 줄에서 counter7} 5보다 작은지 검사되고 12번 줄에서 하나가 증가합니
다. 16번 줄에서 간단한 하나의 문장을 출력합니다.

17 순환문은 이 세 가지 과정 - 초기화, 검사, 증가 - 을 하나의 문장에 잡아넣습
니다. fords 예약어는 한 쌍의 소괄호와 그 안에 세계의 문장이 세미콜론으로
나누어져 있습니다.

처음의 문장은 초기화입니다. 0++에 맞는 어떠한 문장도 들어갈 수 있는데 we
적으로 숫자를 세는 변수의 선언 및 초기화가 이루어집니다. 두 번째 문장은
Heda Ceol 맞는 어떠한 문장도 들어갈 수 있습니다. 이 Ete  mht

문과 같은 역할을 합니다. 세 번째 문장은 수행입니다. 대부분은 숫자를 나타
re 변수를 CH 문법에 맞게 하여 증가시키거나 감소시킴니다. 첫 번째와 세 번
AL 문장은 0++에 맞는 문장이면 되는데 두 번째 문장은 수식 - 반환값을 갖
이어야만 합니다. [리스트 7이가 사용법을 보여줍니다.

rr

[리스트 7.9] for S22) 여제

// let re a

#include <iostream.h>

int main()
{

NOW KF WD


===== PAGE 199 =====
196 ee AI

8:    int counter;

9:    for (int counter =

10%      cout << "Looping! ";
Ae

121   cout << "\nCounter:

13%    return 0;

142 J

0; counter < 5; countert++)

"<<-caunter << “.\n"s

Looping! Looping! Looping! Loo
Counter: 5.

분석  8번 줄의 1ㅠ문은 0000@의 초기화,

ping! Looping!

counter7} 5보다 작은 지의 검사, counter

의 증가 - 이 모든 것이 하나의 문장으로 이루어져 있습니다. for 문장의 몸
AS 9번 줄이며, 블록문이 여기서 쓰일 수도 있습니다.
for 문장
for (초기화 ; 검사 ; 수행)
프자 ,
| 글 ea
초기화는 숫자변수를 초기화하거나 순환문을 위한 준비를 합니다. 검사는 C++ 문장에
맞는 수식문이면 되고 매번 수행 시마다 검사됩니다. 검사 결과가 참이면 아문의 몸체가
실행된 후 세 번째 문장이 수행됩니다.
예제 1

// helloS 104 28
for © = 8-9 10 1
cout <<:"Helto! ">

예제 2
for Cnt 1 = 0 2 7-<910) 5-144)
{
cout << "Hello!" << endl;
cout << "the value of 1 is:
}

"<< i << endl;

for 순환문의 고급 사용
for 문장은 강력하고 유연성이 높습니다.
수행) 세 가지는 각각의 변환들을 합니다.

세 개의 각각 독립된 문장(초기화, 검사,



===== PAGE 200 =====
제7일 프로그램 흐름 ee 197

1@문은 다음의 과정을 밝습니다.
I, 조기화 Vv
2 조건 검사 “
3. 검사 결과가 Ae! 때 순환문을 실행하고 세 번째 문장을 수행합니다.

그리고 매번 2와 3의 과정을 반복합니다.

복수개의 초기화와 복수개의 증가
하나 이상의 변수를 초기화하고 여러 개의 논리식을 검사하며 하나 이상의 문
을 수행하는 것은 그리 흔한 일은 아닙니다. 초기화와 수행문은 0++ 문법에 맞는
여러 개의 문장으로 섬표를 분리점으로 하여 대체될 수 있습니다. [리스트 7.10|
은 두 개의 변수의 초기화와 증가를 보여줍니다.

If o&

[리스트 7.10] for 순환문에서의 SA 문장의 보기

Te 77

2: // [리스트 7.101 for 순환문에서의 복수 문장의 보기
oe -//

4:

5: #include <iostream.h>

6:

7: int main()

8: <

os    for Cint i=0, j=0; i<3; i++, j++)

10:      cout << "is" << 1 << '™ 11 <K j << endl;
11:   return 0;

12: 3

BAH ?번 줄에서 변수 i, ]가 0으로 각각 초기화되었습니다. 검사가6 < 3) 이루어
지고 참이면 수행문이 수행됩니다. forks] 몸체가 실행되고 값들이 sag

| Hw
mul
rH
때
Sots
1 =
o>
pl
: 위
kN
NM

Ae 다시 검사되고, 참이면 수행문이
j 중가) 그리고 10의 몸체 부분이 설행됩니다. 검사가 실패할 때까

데, 마지막 수행문은 실행이 안되고 프로그램은 순환문 밖으로


===== PAGE 201 =====
198 ee AF

for 순환문에서 널에미) 문장

은 전부는 널 문장(빈 문장)이 될 수 있습니다. 이는 문장
분에 아무 것도 쓰지 않고 단지 제미아  을 만납니다. \46문과 똑같이 수행하
for 순환문을 만들기 위해서는 처음과 세 번째의 문장을 빼버립니다. [리스
7.111이 이 AAS 보여줍니다.

fs

\m clr

[리스트 7.11] for 순환문에서의 널 문장

1: // [리스트 7.113 for 순환문에서의 널 문장
ae tf

3

4: #include <iostream.h>

De

6: int main()

08 x

8     int counter = 0;

9

10%   for ( ; counter < 5; )

11   €

12     countertt;

15%      cout << "Looping! ";

14:   가

198

16%   cout << "\nCounter: " << counter << ".\n";
1:   return 0;

18% 3

결과  Looping! Looping! Looping! Looping! Looping!
Counter: 5.

way 이지 [리스트 7.8]의 while 순환문과 똑같습니다. 8번 줄에서 초기화가
이루어졌습니다. 10번 줄의 문장은
5를 검사합니다. 증가문도 없고 따라서 이 EAS 다음과 똑같은 역할
while ( count <5 )
C++ 은 여러분에게 위와 똑같은 역할을 하는           지
경험 있는 프로그래머는 이런 방식으로 10문을 쓰지는 이너 단지 때 가

지는 융통성을 보여주기 위함입니다. 또 하나 1@문에 아무런 문장도 써넣지 않고
중간에 continue} 68문을 넣어 일반적인 forts 똑같이 만들 수  있습니다. [리
스트 7.12]를 봅시다.



===== PAGE 202 =====
제7일 프로그램 흐름 ㅇㅇ 199

[리스트 7.12] 널 for 순환문

1: // [리스트 7.123 널 for 순환문
28 //

3

4: #include <iostream.h>

Bye

6: int main()

2 <

8    int counter=0; // 초기화
9    int max;

10:   cout << "How many hellos?";
118   cin >> max;

12: for (33)    // BYE for®
13   {

14:     if (counter < max)   // 검삭
‘5     {

16:        cout << "Hello!\n";
17:       counter++;   // 증가
18:     }

TOs      else

20:        break;

213   }

28   return 0;

25: }

결과  How many hellos? 3
Hello!
Hello!
Hello!

Ay forte) 최대로 변형되었습니다. 초기화, 검사, 수행문, 모두가 빠져버렸습니
다. 초기화는 8번 줄에서 됐고 검사문은 14번 줄에서 ifS 통해 이루어졌고,
검사가 성공할 때 일어나는 수행문은(60406 증가) 17H 줄에서 일어났습니다. a
사가 거짓으로 판명되면 21번 줄을 빠져나갑니다.
좀 엉뚱하긴 하지만 10( ; ; )가 while ( 1 )과 똑같이
동작하는 ie eeepc HS switche] 논의될 때 좀더 합리적인 사용법을
보게 될 것입니다.


===== PAGE 203 =====
200 ee 제1주

Hl for 순환문

1@문의 표제 BES 바꿔서 여러 가지를 할 수 있는데, 몸체 부분
아무 것도 수행 안하게 할 수 있습니다. 이런 경우는 널 문장 ( ;
대신합니다. 표제 부분에 세미콜론을 넣을 순 있지만 못보고 지나칠

[리스트 7.13]을. 봅시다.

[리스트 7.13] for 순환문에서의 빈 문장

을 guy

)으로 몸체를
수 있습니다.

= -53 COON 에 UFWN —
… ㅁㅁ ㅁ90 990 99 0990 09009

) xe

hy
// [리스트 7.133 for 순환문에서의
//

r=
Ao
ㅇ

#include <iostream.h>
int main®)
sf
for Cint i = 0; 1<5 cout <4 "i: " << it+ << endl)
>

return 0;

re

=

ㅣ

~ 에 00 = O

1
‘
i

분석 8번 줄의 1@문은 세 개의 문장을 가지고 있습니다. 초기화

어 0을 대입하였습니다. 검사문은 1 < 5를 검사하고 수행문

하나 증가시킴니다.

몸체에서 할 일은 하나도 없습니다. 빈 문장이 있을 BAYA; )

장은 1

때
운 뚜

kL 때

1를

력

이 예제는 잘

설계된 for 문은 아닙니다. 수행문이 너무나 많은 일을 합니다. 차라리 다음과 같
이 쓰는 것이 WFC.

8:
9:

for (int i=0O0;i1<5 7; i++)
cout << "i: " << i << endl;

똑같은 YS 하는 프로그램이지만 이 예제가 이해하기 BA 쉽습니다.


===== PAGE 204 =====
제7일 프로그램 SE ee 201

순환문은 중첩될 수가 있는데 하나의 순환문이 또 다른 순환문의 몸체 부분에 들
어앉는 것입니다. [리스트 LMS 중첩 순환문을 사용하여 매트릭스 모양을 만드
는 프로그램입니다.

[리스트 7.14] 중첩 for 문장

1: // [리스트 7.147 중첩 for 문장

2: Jf

3:

4: #include <iostream.h>

ae

6: int main()

te =

8:    int rows, columns;

oO    char theChar;

10:    cout << "How many rows? ";
Ls   cin >> rows;

12:    cout << "How many columns? ";
13:   cin >> columns;

14:    cout << "What character? ";
153   cin >> theChar;

16:   for (int i = 0; i<rows; i++)
VC:   x,

18:      for (int j = 0; j<columns; j++)
ADs        cout << theChar;

20:      cout << "\n" 』

21¢   J

22:   return 0;

255)

How many rows? 4

How many columns? 12
What character? x
XXXXXXXXXXXX

XXX XK MANN KX
XXXXXXXXXXXX
XXXXKXKXKKKKK

이 프로그램은 사용자가 행과 Se
다. 16번 줄의 처음 for 순환문에
의 몸체가 실행됩니다.

(us
=

&

00

ao} 수
서 를

및 출력할 문자를 입력하도록 합니
0으로 초기화하였고 바깥 for 순환문


===== PAGE 205 =====
202 ce AIF

18번 줄에서(처음 for 순환문의 AS 실행부) 또 GS 10문이 실행됩니다. ]가 02
로 초기화되고 내부 forts] 몸체가 실행됩니다. 19번 줄에서 선택된 문자가 출

되고 통제권은 내부 for 순환문의 표제 부분으로 되풀이됩니다. 내부 for 순환문은
단 한 졸의 BAYS 주목합시다. 조건문이 검사되고 G < column) 이 수식이 참
이면 j= 증가되어 다음 x7} 출력됩니다. 이는 가 001000과 같아질 때까지 계속
됩니다

일단

eas 하나 출릭합니다 ore ened 이제 표제 부분으로 올라가고 여기서 1의
ah 검사됩니다. Ale] 나오면 [는 증가되고 순환문의 몸체가 실행됩니다. 두
date] 외부 eee] 다시 시작하고 따라서 내부 순환문은 처음부터 다시 시작
a              고 전체 내부 순환문이 실행이 됩니다

여기에서 중요한 개념은 중첨된 순환문      a
돌 때마다 전부 다시 수행이 된다는 것입니다. 따라
이 됩니다.

덧붙여 말하면 많은 C++ 프로그래머들이 if j LATS 숫자 ATE Series.

은 『0071604으로 가는데, FORTRANUAE 단지 i,j,k, | 0, (만이 숫자 변수로
습니다.

다른 프로그래머들은 좀더 의미를 지닌 숫자 HFS 쓰는메, 예를 들면 Ctrl, 00? 등
입니다, 그러나 |, |를 쓴다고 그리 온동되지는 않는 것이 현실입니다.

for 순환문에서의 범위 규칙
변수들은 그들이 만들어지는 블록에서 유효하다는 것을 여러분은 기억할 것입니
다. 다시 말하자면 지역 변수는 그 변수가 만들어진 블록 안에서만 그 AS 보장
받습니다. 한편 for 순환문에서 그 표제 부분에서 만들어진 변수들은 그 외부 순
환문에서도 유효하다는 것을 기억해야 합니다. 즉, 여러분이 한 함수에서 두 개
이상의 순환문을 갖는다면 여러분은 다른 숫자 WES 주어야 한다는 것입니다
그렇지 않으면 그들은 서로 값을 주고받아 오류를 발생시키게 되는 것입니다.



===== PAGE 206 =====
제7일 프로그램 흐름 ee 203

1}

10

=

환문 Q
5일째 되는 날 여러분은 어떻게 자기 호출을 사용하여 피보나치 수열을 풀어나가
는지 배웠습니다. 간단히 복습하면 피보나치 수열은 | 1, 2, 3, …으로 시작하며
각 항의 숫자는 앞의 두 항의 합입니다.

12 1287 35% Dp. 8, 13, 215.545

Neale] 숫자는 4-1과 4-2번째 수의 합입니다. slay 공부한 내용은 씨번째 피보
나치 수를 찾는 것이었습니다. 그리고 이는 자기 호출을 통해 해결되었습니다.
[리스트 7.15|는 순환문을 통해 이를 푸는 방법을 제시하였습니다.

Le

[리스트 7.15) 순환문을 써서 피보나치 AB 구하는 방법

fe df

2: // [리스트 7.151] 순환문을 써서 피보나치 수를 구하는 방법
Si //

4:

5: #include <iostream.h>

6:

7: typedef unsigned long int ULONG;

8s

9: ULONG fib(ULONG position);

10: int main()

11: <

as   ULONG answer, position;
{Roi   cout << "Which position? ";
14:   cin >> position;

1D:   cout << "\n"

16%
17s   answer = fib(position);
18:   cout << answer <<" is the ";

19:   cout << position << "th Fibonnacci number.\n";
20:   return 0;

21: 3}

22:

23: ULONG fib(ULONG 0)

24: {              ¢

25:   ULONG minusTwo=1, minusOne=1, answer= =2;
26:

20:    if (n< 3)

28:      return 1;

29:

30:   for (n -= 3; n; n--)

1


===== PAGE 207 =====
204 ee 제1주

치기     ovis   Bret

nes         \                3
31:           ：                                          주 =
32:      minusTwo = minusOne;          m4        8.      e
33:      minusOne = answer;
34:      answer = minusOne + minusTwo; 1
35:   3
36:
a7   return answer;
381 +

결과  Which position? 4

3 is the 4th Fibonnacci number.

Which position? 5

5 is the 5th Fibonnacci number.

Which position? 20

6765 is the 20th Fibonnacci number.

Which position? 100

3314859971 is the 100th Fibonnacci number.

[리스트 7.15]는 피보나치 수열의 HAS 자기 SSS 하지 않고 순환을 통
해 풀어나갔습니다. 이러한 방식이 훨씬 빠르고, 메모리도 작게 잡습니다.

14번 줄에서 사용자는 구하고자 하는 항을 입력합니다. 함수 800가 호출되고 이
때 값을 계산합니다. 위치가 3보다 작으면 1을 반환하고 3항부  터 시작하면 다음
과 같은 알고리즘을 사용합니다.

1. 시작점을 잡습니다. 변수 305'\6[에 2를 minusTwool 1을 minusOnedl 1을 te

다. 처음의 두 개의 숫자가 시작점으로 잡혔기 때문에 구하고자 하는 항의 위치에서 3을
빼고 시작합니다.

(faa
Bea

2 각 숫자에서 피보나치 FAS 더해 나갑니다. 이는 다음과 같이 수행됩니다.
minusOne= minusTwooll 대입합니다.

. answer2| 값을 001045006에 대입합니다.

minusOnez} minusTwoS 서로 더해서 answeroll 대입합니다.

0. n& 하나 AAAQUCct.

3. no| Oo] 도달하면 answerS 반환합니다.

oo ®



===== PAGE 208 =====
이것이 실제 여러분이 종이와 ABS 가지고 푸는 방법입니다. 여러분이 5번째의
피보나치 수열의 항을 구한다고 했다면 이렇게 할 것입니다.

12172,

그리고 생각할 것입니다 두 개 더해야 한다" 여러분은 2 + 1을 한 뒤 3을 쓰고
또 생각합니다. '한 번 더하면 된다." 마지막으로 3 + 2를 하여 5라는 답을 구합
니다. 실제 여러분은 여러분의 계산을 한번씩 우측으로 이동시킴니다. 그리고 앞
으로 계산해야 할 횟수를 하나씩 줄입니다.

30번 줄의 검사문 00을 한번 봅시다. 이는 0++에서 쓰이는 방법인데 정확히는 1
I= 0과 같습니다. for 순환문에서 no] Oo] 도달하였을 때 거짓으로 됩니다. 왜냐하
면 (++에서는 0은 거짓이기 때문입니다. for 순환문의 표제 부분은 다음과 같이
쓰여질 수 있습니다.

for (n-=3;n !=0; nt+ )
이것이 SU 명확합니다. 하지만 너무 흔하여 S 재미가 없습니다.

컴파일하고 링크한 뒤 이 프로그램을 5일째 배운 프로그램과 같이 비교하여 실행
시켜 봅시다. 25번째 수열을 구하게 해보고 걸리는 시간을 측정하여 봅시다. 자기
출 방법이 우아한 방법이긴 하지만 함수 호출에 너무나 많은 Bap} 걸립니다.

그리고 너무나 많이 호출되기 때문에 순환식 프로그램보다 상당히 느립니다. 80

는 수학연산에 있어 최적화가 되어 있기 때문에 순환 방식이 Ba 빠릅니다.

5\【아분 wreath 8 He 수리
4일째 학습 날 여러분은 if 및 if / 056에 대하여 배웠습니다. 이러한 것은 깊게
중첩이 될 경우 혼란이 될 수 있는데 0++은 여기에 다른 방법을 제공합니다. 단
한번 검사를 하는 #와 달리 switche 몇 번이라도 검사를 할 수 있게 합니다.
switche] 일반적인 형식은 다음과 같습니다.

switch (수식)

t
case valueOne: 문장
break;
case valueTwo: 문장
break;
case valueN :      문장

break;


===== PAGE 209 =====
206 ee ANF

만일, 수식 A case] 값이 AAS 하면
지 않는 한 switch 블록의 마지막까지 수행이

default! 분기가 됩니다. default 없고 딱 맞는 case 해당 값도 없다면
행은 9때문의 바깥으로 빠져 나갑니다.

switch 항상 defoutttS 갖는 것이 중요합니다. 만일, defaults 쓸 8
하더라도 있을 만한 오류를 생각하여 오류 메시지를 줄력하도록 합니다.
된
[1]

아주 도움이

각 case 문 7  끝에 ‘break7} 없는지 주의합시다. 없으면 다음 0@850문까지 실행이 AS
됩니다. 물론 일부러 이렇게 할 경우엔 그 이유를 주석으로 달아 놓읍시다.

리스트 7.16]은 switcht2} 예입니다.

—

[리스트 7.16] switch= 예

1: // [리스트 7.161 switche 예

2: //

3

4: #include <iostream.h>

55

6: int mainQ

ve 4

8    unsigned short int number;

9:    cout << "Enter a number between 1 and 5: ";

10:    cin >> number;

113   switch (number)

12:   x

13%     case 0: cout << "Too small, sorry!";

14:        break;

15:     case 5: cout << "Good job!\n"; // 실행이 아래로 ASS
16:     case 4: cout << "Nice Pick!\n"; // 실행이 아래로 게속됨
4 WA     case 3: cout << "Excellent! \n"; // 실행이 아래로 계속됨
18:     case 2: cout << "Masterful!\n"; // 실행이 아래로 HSE
195     case 1: cout << "Incredible! \n";



===== PAGE 210 =====
세7일 프로그램 흐름 eo 207

20%        break;

2%      default: cout << "Too Large!\n";
22        break;

235:   y

24:    cout << "\n\n";
252   return 0;
26: 7

결과  Enter a number between 1 and 5: 3
Excellent!
Masterful!
Incredible!

Enter a number between 1 and 5: 8
Too large!

분석  사용자는 RAS 입력하도록 요구됩니다. 그 숫자는 9\애문에 Ato] 됩니
다. 숫자가 0이라면 13번 BS] case 문과 만나게 되고 메시지는 700 small,
sorry!7} 됩니다. 66#(문을 만나서 switch we] 나옵니다. 값이 sel 경우는 A
행문은 15번 줄로 가고 거기에서 SAS 한 뒤 이번에는 16번 줄로 가 또 다른
메시지를 출력하며 20번 줄의 breakS 만날 때까지 계속 메시지를 출력합니다. 이
프로그램에서 실제 영향을 미치는 AS 1부터 5까지의 수이고 그에 따라 여러 메
시지들이 출력됩니다. 숫자가 0 - 5가 아닌 BPE 21번 줄의 default 문장이 수행
됩니다.

switch

switch (4 4] )

ic
case valueOne: 문장 ;
case valueTwo: 문장 ;
case valueN :      문장 ;
default: 2%} ;

}

switch22 수식의 값에 따라 여러 문장으로 분기할 + 있게 합니다. ANS 계산되고,
각 6850문에 해당하는 값이 나오는 경우 그 6856문으로 실행이 넘어갑니다. 실행은
switch22| BS 만나거나 혹은 6「68(문을 만달 때까지 계속됩니다.



===== PAGE 211 =====
208 ee AIF

만일, 수식의 결과물에 해당되는 값이 6356에 없고 defaultZo| 있다면 수행은 0618니[
문으로 갑니다. 만일 0613411문도 없다면 9\1[아문은 끝이 납니다.
예제 1
switch ( choice )
{
case 0:
cout << "Zero!" << endl;
break;
case 1:
cout << "One!" << endl;
break;
case 2:
cout << "Two!" << endl;
default:
cout << "Default!" << endl;
?
예제 2
switch ( choice )
{
case 0:
case 1:
case 2:
cout << "Less than 3!" ;
break;
case 3:
cout << “Egquals-5!" 5
break;
default:
cout << "greater than 3!" ;
}

메뉴 구성 BSBA switche 쓰기
[리스트 TITS 다시 앞서 논의하였던 60 ( ; ; ) 순환문으로 돌아옵니다. 이 순환
문은 무한 순환문이라고도 합니다. 왜냐하면 breakS 만나기 전에는 순환문을 |
져 나오지 않기 때문입니다. 무한 순환문은 메뉴 구성 프로그램 같은 곳에서 쓰
입니다. 사용자로부터 메뉴를 선택받아 해당 메뉴를 실행한 뒤 다시 메뉴로 돌아
옵니다. 사용자가 종료를 원할 때 끝납니다.

=


===== PAGE 212 =====
N72 프로그램 흐름 ㅎㅎ 209

다음과 같이 쓰는 프로그래머도 있습니다.

H#define EVER    y
tor ( EVER )
{

종료 조건이 없는 순환문을 말합니다. 종료하기 위해서는 dreakBES
3

[리스트 7.17] 무한 순환문 예

Ae df

2: // [리스트 7.171 무한 순환문 혜

S: J/

4: #include <iostream.h>

5:

fei

7: enum BOOL { FALSE, TRUE };

8: typedef unsigned short int USHORT;
oe

10: // 원형

11: USHORT menu() ;

12: void DoTaskOne();

13: void DoTaskMany(USHORT) ;
14:                  ‘
15: int main          wits
16: 1

Uf:

18:   BOOL exit = FALSE;

AG:   for Css)

20:   {

212     USHORT choice = menu();
22:     switch(choice)

23%     £

245       case (1):

25:          DoTaskOne();

26:          break;

20:         case (2):


===== PAGE 213 =====
210 ee 제1주

28:          DoTaskMany (2);

29:          break;

50:        case (3):

31          DoTaskMany (3);

32:          break;

$3:       case (4):

34:           continue; // 불필요함!
35:           break;

365       case (5):

Sf:          exit=TRUE;

38:           break;

39%       default:

40:           cout << "Please select again!\n";
41:           break;

42:      +    // end switch

43:

44:   if (exit)

455       break;

46:   }      // end forever

47:   return 0;

48: }       // end main®

49:

50: USHORT menu()

51: x

D2:   USHORT choice;

DS:   cout << " **k* Menu ****\n"7
54%   cout << "(1) Choice one.\n";

553   cout << "(2) Choice two.\n";

56:   cout << "(3) Choice three.\n";
Dt   cout << "(4) Redisplay menu.\n";
58:   cout << "(5) Quit.\n";

59:    cout <<""s ">

60:   cin >> choice;

61:   return choice;

62: +

63:

64: void DoTaskOne()

655 ¢

66:   cout << "Task One!\n";
60: +

68:

69: void DoTaskMany (USHORT which)
70: ¢

(Ale   if (which == 2)

2:      cout << "Task Two!\n";

(3%   else


===== PAGE 214 =====
제7일 프로그램 흐름 ee 211

74:      cout << "Task Three!\n";
758 2

결과  *kKK Menu ＊ㅎ*%*%*

(1) Choice one.

(2) Choice two.

(3) Choice three.
(4) Redisplay menu.

(5) Quit.
24
Task One!

kkk Menu **x*x*

(1) Choice one.

(2) Choice two.

(3) Choice three.
(4) Redisplay menu.

(5) Quit.
= 5
Task three!

kkk Menu ****

(1) Choice one.

(2) Choice two.

(3) Choice three.
(4) Redisplay menu.
(5) Quit.

Mo] 프로그럼은 어제와 오늘 배운 여러 개념들을 한 군데로 모아 사용하였
습니다. 51매문의 일반적인 사용법도 보여주었습니다.

7번 줄에서 상수 나열형 800Ｌ이 0값을 갖는 FALSES} 1 값을 갖는 TRUEZ 선
언되었습니다. 8번 줄에서 typedefS 써서 unsigned 9807를 USHORTS. 재정의하였
습니다.

19번 줄에서부터 무한 순환문이 시작됩니다. menu) 함수가 호출되어 메뉴를 화면
선택을

|
에 출력하고 사용자의       반환합니다. switch 문장은 22번에서 시작하여 42번
줄에서 끝납니다.

(rag


===== PAGE 215 =====
212

ee AIF

사용자가 1번을 입력하면 APS 24H Sol] 있는 case 로 갑니다. 25번 줄에서
10018900060 함수를 부르는데 이는 메시지를 출력한 A 되돌아옵니다. Brey
실행은 26번 줄로 오게 되고 여기서 breakS 만나 switches] 끝으로 나가 43번
줄로 가게 됩니다. 44번 줄에서 변수 6짜를 검사합니다. 참이면 45번 줄의 break
가 실행되고 1ㅠ ( ; ; )문은 끝나게 됩니다. 그러나 거짓으로 판명되면 19번 줄의
순환문 꼭대기로 다시 올라가게 됩니다.

34번 49) 00007006문은 불필요한 문장입니다. 0000006가 없더라도 breakS 만나
switche 끝날 것이고, exit 변수는 거짓으로 판단될 것이며, 순환문은 다시 실행

되고 메뉴는 다시 출력될 것입니다. 하지만 0000006문은 exit 변수를 검사하는 과

을 생략하게 해줍니다.

00     깊이 SMS PLS FS] 위해 switch BS 사용합시다.
DON'T 2 <ㅎ66문의 끝에 6768<문을 실수로 빠뜨리지 BACH.
00     각 6856문에서 일부러 breaks WE 경우는 주석을 넣읍시다

00     switch 끝에 defaut2S 답시다. 보기에 있을 FA

우를 대비해 봅시다.

에는 여러 가지 순환문들이 있                  사하고 참이면 몸
을 수행합니다. 00..0440문은 순환문의 몸체를 한 번 수행하고 난 후

색합니다. forte 값을 초기화하고 FAS 검사하며 수식이 참일 때
for: 표제 부분의 마지막 수행문을 실행하고 몸체를 실행합니다. 각 순환문이 한

번씩 돌아올 때마다 조건문이 검사됩니다.

8000문은 피합시다. 이는 코드상의 임의의 아무 위치로 건너뛰기를 하기 때문인데
따라서 원시 코드를 이해하기 어렵게 하고 유지 보수가 힘들게 WUC. continue
문은 while, do...while, 1@문에서 다시 시작을 하게 하고 breaki= while, do...while,
for, 9\110문에서 수행을 빠져나가게|합니다.

픽%
1S
ay
=

로
oO

Ad
rlo
EN
ae
ilo
dm


===== PAGE 216 =====
제7일 프로그램 흐름 ee 213

Q&A

Q if / else@2} switch= 각각 어떤 때 쓰입니까?

A 여러 개의 056문을 쓰면서 그들이 같은 BS 검사할 때 swithBe 쓰는 A
하여 봅시다.

Q while} do...while#= 각각 어떤 때 쓰입니까?

A 순환문의 몸체가 일단 한 번은 꼭 실행이 되어야 할 때 do..whileS 쓰고 나머지는
'\416문을 써도 됩니다.

Q while2} for2S 구별하시오.

A 초기 숫자 변수를 초기화하고, FAS 검사하며, 각 순환 때마다 변수를 수정해야
한다면 10를 생각해 봅시다. 변수가 이미 초기화되어 있고, 각 순환 때마다 변화가
없으면 \46문이 더 좋은 선택이 됩니다.

Q 자기 호출과 SHES 어떤 때 각각 쓰입니까?

쇼 어떤 문제들은 자기 호출을 요구합니다. 하지만 대부분의 프로그램은 순환문으로
해결이 됩니다. 그래도 자기 호출방식을 잘 aga.

고려

tho

Q while (1)이 for (;;) SiC} 좋은지.
A'S = 차이 없습니다.

1. for 순환문에서 하나 이상의 변수를 초기화하는 방법은?
2 왜 9010는 피해야 합니까?
3 실행이 되지 않는 몸체를 가진 +아문이 가능합니까?

쓸 수 있습니까?

그.
oO
Ho
010
마

4 10「문 안에 중첩된
등합니까?

7
어떤 일이 발생됩니까?


===== PAGE 217 =====
214 ee 제1주

= |
연습 문제
1. 다음의 10「문이 끝나면 ×값은 어떻게 됩니까?
for ( int x = 0; x < 100 ; xt+ )

2 10°109] 0 EAS 출력하는 SAE 10문을 만들어 보시오

3. 100부터 200까지를 두 단위 씩 세어보는 {0「 프로그램을 짜십시오.

4 100부터 200까지를 두 단위 씩 세어보는 while =2IAS 짜십시오.

$ㆍ 100부터 200까지를 두 단위 씩 세어보는 00...101116 프로그램을 짜십시오.

6 버그잡기 :

int counter = 0
while ( counter < 10 )

a
cout << "counter: " << counter;
+
7 버그잡기 :
for ( int counter = 0 ; counter < 10 ; countertt ) ;
cout << counter << "";
8& 버그잡기 :

int counter = 100;
while ( counter < 10 )

{
cout << " counter now: " << counter;
counter-—;
+
9 버그잡기 :

cout << "Enter a number between 0 and 5: ";
cin >> theNumber;
switch ( theNumber )
{
case Q:
doZero() ;
case 1 :// 계속
case 2 :// 계속
case 3 :// 계속
case 4 :// 게속
case 5 :// 계속
doOneF ive(
break;
default :
doDefault() ;
break;

wpa  Ara
= ara ara
0% of! of off of



===== PAGE 218 =====


===== PAGE 219 =====
216 ee AIF

[리스트 『1.1] 첫째 주 복습 목록

#include <iostream.h>

1:

2:

3: typedef unsigned short int USHORT;

4: typedef unsigned long int ULONG;

5: enum BOOL { FALSE, TRUE};

6: enum CHOICE { DrawRect = 1,GetArea,

16      GetPerim, ChangeDimensions, Quit};
8: // Rectangle 클래스 선언

9: class Rectangle

10: +

11: public:

12:     // 생성자

13:     Rectangle(USHORT width, USHORT height);

14:     “Rectangle();

15:

16:    // 접근자

War     USHORT GetHeight() const { return itsHeight; }
18:     USHORT GetWidth() const { return itsWidth; }

19:     ULONG GetArea() const { return itsHeight * itsWidth; }
20:     ULONG GetPerim() const { return 2*itsHeight + 2*itsWidth; }
218     void SetSize(USHORT newWidth, USHORT newHeight) ;
22:

23:     // 키타 연산자

24:     void DrawShape() const;

20%

26: private:

2¢:     USHORT itsWidth;

28:     USHORT itsHeight;

29% 35

50:

31: // Class method 구현

32: void Rectangle::SetSize(USHORT newWidth, USHORT newHeight)
55: !:

34:    itsWidth = newWidth;

552    itsHeight = newHeight;

56: }

STs

38:

39: Rectangle::Rectangle(USHORT width, USHORT height)
40: ¢

41:    itsWidth = width; // 초기화

42:    itsHeight = height;

AS:

44:

45: Rectangle::~Rectangle() {}



===== PAGE 220 =====
제1주 끝내면서 ee 217

46:
47:
48:
49:
50:
512
a2:
535
54:
D5
56:
57:
58:
59%
60:
61:
622
63:
64:
65%
66:
67:
68:
69:
CUE
1s
tee
738
74:
er
76:
CC:
78:
(9:
80:
81:
82;
83:
84:
85%
86:
Sf:
88:
89:
90:
91:
92:

USHORT DoMenu();

void DoDrawRect (Rectangle) ;
void DoGetArea(Rectangle);
void DoGetPerim(Rectangle);

int main()

{
// initialize a rectangle to 10,20
Rectangle theRect (30,5);

USHORT choice = DrawRect;
USHORT fQuit = FALSE;

while (! fQuit)
AE
choice = DoMenu();
if (choice < DrawRect || choice > Quit)
£
cout << "\nInvalid Choice, please try again.\n\n";
continue;
}
switch (choice)
{
case DrawRect:
DoDrawRect (theRect) ;
break;
case GetArea:
DoGetArea(theRect);
break;
case GetPerim:
DoGetPerim(theRect) ;
break;
case ChangeDimensions:
USHORT newLength, newWidth;
cout << "\nNew width: ";
cin >> newWidth;
cout << "New height: ";
cin >> newLength;
theRect.SetSize(newWidth, newLength) ;
DoDrawRect(theRect);
break;
case Quit:
fQuit = TRUE;
cout << "\nExiting...\n\n";
break;
default:
cout << "Error in choice!\n";


===== PAGE 221 =====
218 eo AIF

935:           fQuit = TRUE;
94:           break;

95:      + // end switch
96:    Bs    // end while
Of:    return 0;

98: }      // end main

99:

100: USHORT DoMenu()

1013 <

102:    USHORT choice;

105%    cout << "\n\n_ *** Menu *** \n";

104:    cout << "(1) Draw Rectangle\n";
105%    cout << "(2) Area\n";

106:    cout << "(3) Perimeter\n";

107:    cout << "(4) Resize\n";

108:    cout << "(5) Quit\n";

1095

T1108    cin >> choice;

105    return choice;

1128 가

113

114: void DoDrawRect (Rectangle theRect)
se x

116:    USHORT height = theRect.GetHeight ();
(ira    USHORT width = theRect.GetWidth();
118:

119:    for (USHORT 1 = 0; i<height; i++)
120:    {

A218       for (USHORT j = 0; j<width; j++)
122:         cout << "내

125:       cout << "\n";

124:    }

1258 +

126%

127%

128: void DoGetArea(Rectangle theRect)

129: <<

150:    cout << "Area: " << theRect.GetArea() << endl;
AS: +}

132:

133: void DoGetPerim(Rectangle theRect)
134: <

135%    cout << "Perimeter: " << theRect.GetPerim() << endl;
136: }



===== PAGE 222 =====
제1주 끝내면서 ee 219

겔과  ***× Menu ***

(1) Draw Rectangle
(2) Area

(3) Perimeter

(4) Resize

(5) Quit

불셀 여기 프로그램은 여러분이 이번 Fo] 배운 BE 기술을 다 사용합니다. 여

러분은 단지 이 코드를 입력, 컴파일, 링크, 수행하는 것은 물론이고 무엇을

하는지, 어떻게 동작하는지를 여러분이 이번 주에 배운 것을 기반으로 하여 살펴
봅시다.

처음 TA 줄까지는 이 프로그램에서 사용될 형들을 만들었습니다.

8 - 29번 줄까지는 \0000806 SAAS 선언하였습니다. 여기서 사각형의 밑변과
높이를 설정하고 구하기 위해, 또 면적과 둘레길이를 구하기 위해 범용 접근자
메쏘드를 썼습니다. 31 - 43번 줄은 클래스 함수 정의가 있는데 10106으로 선언하
지는 않았습니다.

클래스 함수가 아넌 일반 함수의 원형은 46 - 49번 줄에 있고 실제 프로그램은
51번 줄부터 시작합니다. 이 프로그램의 핵심은 사각형을 만드는 것이고 5가지
SAS 제공하는 메뉴를 출력하는 것입니다. 사각형을 그리고 면적과 gas 계
산하고, 다시 사각형을 계산하거나 By.

플래그는 57번 줄에 있습니다. 이 플래그가 참이 아닌 한 메뉴 순환문은 계속 진
행됩니다. 사용자가 메뉴에서 Quits 선택하면 플래그는 참이 됩니다.

사용자가 선택을 하게 되면 ChangeDimensionsS 제외하고는 다른 함수들을
합니다. 이것이 9\\때문을 보기 좋게 합니다. ChangeDimensions= 사각형의
를 변화시키기 때문에 BFS Sse) 않습니다. 만일 rectangle7}
DoChangeDimensions() 같은 함수에 매개 변수로 전달되면 00086는 지역적으로
복사가 되어 DoChangeDimensions() 안에서 값이 변화가 되며 쓰이지만 2800 안
에서의 값은 변화가 없습니다.

불린형을 AAS 뒤 9\1 안에서 사용하여 프로그램이 깨끗해졌습니다. 9\대문
안에 숫자를 가지고 6890문에서 썼다면 어느 숫자가 어느 메뉴인지 알기 위해 여
z     항상 다른 표를 참조해야 했을 것입니다.

62번 줄에서 사용자의 선택이 그 범위 안의 값인지 검사합니다. 만일 범위 안의
ako] 아니면 경고문이 출력되고 메뉴가 다시 출력됩니다. 9\때문 안에는 불가능

49

째

a
rlo


===== PAGE 223 =====
220 ee Ae

한 경우를 담은 defo] 있습니다. 이는 디버깅용으로 넣은 것입니다. 만일 =
로그램이 제대로 동작하면 이러한 현상은 안 나타날 것입니다.

첫째 주를 마치며

첫째 주의 공부가 끝났습니다. 일단은 축하를 드립니다. 여러분은 이제 약간 복잡
한 CH 프로그램을 만들 수 있게 되었습니다. 물론 아직 할 것이 많습니다. 다음
주에는 0++에서 다소 복잡한 개념인 포인터를 가지고 시작할 것입니다. 절대로
포기하지 WA. 여러분은 이제 객체 지향 프로그램, 가상 함수, 그리고 다른 매
우 유용한 MISS 배우고 사용할 수 있게 될 것입니다.

잠시 쉬고 여러분이 그 동안 공부한 것의 WS 누린 뒤 둘째 주의 BRS 시작

하여 봅시다.



===== PAGE 224 =====
> 둘째 주의 학습 목표

여러분은 AM 주 동안 (;++의 프로그래밍을 배웠습니다. 이제 여러분은 아무런 부담감 없이 ACH 입력아고,
컴파일러를 사용아고, 그리고 객체, 클래스 및 프로그램의 으름을 생각할 수 있을 것입니다.

둘째 주는 20 (pointer)S 배우면서 시작합니다. 사실 포인터는 CHE 처음 시작아는 분들에게는 어겸운
주제일지 모르겠습니다. 그러나 중분이 그리고 BHO 설명되어 있기 때문에 그리 어렵지는 않으리가 생각됩니
다. 9일째 되는 날 여러분은 포인터의 사존이라 할 수 있는 BTreference)o 대애 배울 것입니다.

10일깨는 함수 재생을 배우고, 11일패는 배열(3[『8\), 12일쩌는 AWA 지향 프로그래밍의 그야말로 근본 개념인
상속에 대애 HISLUCL 13일째는 12일째 학습이 연장인 다형성에 대애 배우고, 14일패는 정적 함수와 프랜드에
대매 배움니다.       |

ro


===== PAGE 225 =====


===== PAGE 226 =====
224 ee 제주

서문
CH 프로그래머가 쓸 수 있는 가장 강력한 도구 중의 하나는 컴퓨터의 메모리를
자유롭게 연산할 수 있는 포인터라는 것입니다. 오늘 여러분이 배울 것은
를 포인터란 +
BUS 선언하고 사용하는가?

Bt 기억 장소란 무엇이며 메모리 연산하는 방법

엇인가

입니다. 0++을 배울 때 포인터라는 항목은 여러분에게 두 가지 넘어야 할 장벽을
쳐 놓았습니다. 하나는 혼동이라는 장벽이고, 다른 하나는 왜 포인터가 필요한 것
인지 하는 회의라는 장벽입니다. 이번 장에서는 이들에 대한 설명을 차근차근 해
나갈 것입니다. 이 책을 점점 공부해 나가면서 도대체 왜 포인터가 필요한 지를
하나씩 알게 될 것입니다.

포입터란 무었인가?

새로운 교인터 포인터란 메모리의 주소를 가리킬 수 있는 변수입니다.

응어
포인터를 이해하기 위해서는 여러분은 컴퓨터의 메모리에 대해 조금 알아야 합니
다. 컴퓨터의 메모리는 그 위치를 가리키는 연속적인 번호가 붙여진 부분으로 나
누어질 수 있습니다. 각 변수는 메모리의 각 유일한 위치(주소라고 함)를 가리키
고 있습니다.(이미 5일째 수업에서 배웠죠.) [그림 8.1]은 040918060 long 정수형 변
4 the Age] 기억 장소를 도식화하여 나타내었습니다.

[그림 8.1]                   메모리
the 406의 도식
the Age
|    T    T    T    T    |    T    T    T    T    |    T    T
10110101 11110110

01110110 911101110

|  |  !  |  ‘ie  |  |  |  |  |  i  ㅣ  |
100 101 102 103 104 105 106 107 108 109 110 111 112 113

24 눈금 = 1바이트
unsigned long int the Age = 4바이트(6116) = 32비트(610)
the 90 변수명은 AX 번째 바이트를 가리킴니다.
the ^06의 주소는 102번입니다.



===== PAGE 227 =====
제8일 포인터 ce 225

다른 컴퓨터들은 이 메모리를 다른 복잡한 그림을 사용하여 번호를 붙입니다. 보

프로그래머가 주어진 변수의 주소까지 자세히 알아야 할 필요는 없습니다.
왜냐하면 컴파일러가 다 알아서 처리하기 때문입니다. 이 주소를 알고 싶다면 여
러분은 주소 연산자(를 사용하여 알 수가 있는데 [리스트 8.1|에서 보여줍니다.

[리스트 8.1] 변수의 주소를 보여줌

: // [리스트 8.1] 변수의 주소
2/7

lu

보여줌

1

2

ae

4: #include <iostream.h>
5:

6

: int main()
Cit
8:   unsigned short shortVar=5; byte
9:   unsigned long lLongVar=65535;
10: long sVar = -65535;

12: cout << "shortVar:\t" << shortVar;
13: cout <<" Address of shortVar:\t";
14: cout << &shortVar << NT UE

16: cout << "LongVar:\t" << lLognVar;
17: cout <<" Address of longVar:\t";
18: cout << &longVar << "\n";

20: cout << "sVar:\t";
21: cout << sVar <<" Address of sVars\t";
22: cout << &sVar << "\n";

(naa
ie

23%

24: ~return 0;

2567}

결과  shortVar: 5      Address of shortVar:0x8fc9:fff4

longVar: 65535   Address of lLongVar:0x8fc9:fff2
sVar:     =65535   Address of sVar: Ox8fc9:ffee
8 - 10번 줄에서 3개의 변수가 나  초기화되었습니다. unsigned +”
unsigned long, 1008입니다. 그들의 값 및 주소가 12 - 22번 줄에서 주소 a

산자(@를 사용하여 출력되었습니다.

80386 컴퓨터에서 수행되었을 때 shortVar wo] 같은 5이고 그 주소는
Ox8fc9:fff4 FUT}. 이 복잡한 주소는 각 컴퓨터마다 다릅니다. 그리고 같은 컴퓨터


===== PAGE 228 =====
226

ee 제2주

에서도 수랭 시마다 달라질 수도 있습니다 따라서 그 결과는 달라짐 수 Sle
다. 변하지 않는 것은 여러분의 컴퓨터가 shot 정수형을 2바이트를 사용한다면
항상 수행 시마다 처음에 두 개의 변수 주소 간격이 2바이트라는 것입니다. 여러
분이 컴퓨터가 lng 정수형을 4바이트 쓴다면 여러분이 사용한 두 번째 변수와
세 번째 변수의 주소의 간격이 4바이트가 됩니다. [그림 BIKE 이 프로그램의 변
수들이 어떻게 저장 장소에 저장되는지를 보여줍니다.
LongVar
ShortVar         SVar
|               |
|   | |   | ] | |   |   |   | |) ㅣ] 4   | 」   |   |   |
0000 0000                              65.535                           -65.535
0000 0101      ,    a    ne     4
5  0000 0000. 3001 7141. 0000 00000 0011 "나

| | | | | | | | | | tt tt ㅣ 」
] |] | ] | | 7 | |

fff3                                fff                                 ftef                                ffed                                ffeb

fff                      fff2                      fff                     ffee                     ffec                     168                     168                     166                     164

[그림 8.2] 변수 저장의 보기

a       는 것
입니다. 여러분은 변수형을 선언함으로써 컴파일러에게 그 변수형에 해당하는 길
이 만큼의 메모리를 잡아 놓을 것을 말해줍니다. 컴파일러는 자동적으로 그 변수
의 주소를 할당합니다. |S 들어, tong 정수형은 4바이트이고 이는 메모리에서 4

바이트를 차지한다는 의미입니다.

wy
KI
2
tly
SG
=
4N
2
cy
ied
00

몰라도 여러분

rlo
4\
00

예를 들어, howOld7} 정수형이라고 합시다. 100000의 주소를 저장할 포인터를
pAgez} 하면 여러분은 다음과 같이 쓸 수 있습니다.

int *pAge =0;

가

이 선언은

수라는 뜻



===== PAGE 229 =====
제8일 포인더 ee 227

pAgct= 변수입니다. 여러분이 정수형 변수를 선언하면 그  「 851 Aas Be
정수로 해석됩니다. 여러분이 pages 포인터로 선언했으면 page 저장되는 내용
은 주소로 해석됩니다. pAgets 변수는 변수이되 그 0 약간 다를 뿐입니다.

여기의 예에서 pAges= 0으로 초기화되어 있습니다. 그 값이 0인 포인터를 널 포
인터라고 합니다. 모든 포인터는 그들이 4 때 어떤 oe 초기화가 됩니다.
포인터에 어떤 WS 초기화시켜야 할지 모르겠거든 0으로 초기화합시다. 초기화
되지 않은 포인터를 와일드(00010) sehen 합니다.

안전주의로 나갑시다! 포인터는 항상 토기화할시타

여러분이 포인터를 0으로 초기화했다면 언젠가는 10\000의 FAS pAgesl) 저장

해야 합니다. 다음과 같이 저장합니다.

unsigned short int howOld = 50;// 변수를 만듬
ㅁ

unsigned short int *pAge = 0;// 포인터 만듬
pAge = &how0ld ;// how0ld2| 42 pAge 저장

—

Al 줄은 변수 40\000를 만들었는데 그 BS unsigned shot 정수형입니다. 그리
그 값을 50으로 초기화하였습니다. 이. 줄은 pAge= unsigned short 정수형의
인터로 선언하고 (으로 초기화하였습니다. 7486는 포인터입니다. 왜냐하면 변
수 앞에 *가 붙어 있기 때문입니다.

셋째 줄은 howOld2] 주소를 0480에 저장하였습니다. & 연산자를 썼기 때문에
howOld9] 주소가 저장되는 것입니다. 만일 주소 연산자(&)가 안 쓰였다면 10010

의 값 50이 저장될 것이고, 이는 틀린 주소가 될 것입니다.

> 버니 낸

ㅇ

이 시점에 있어 pAget= 80\000의 주소를 저장하고 있고 howOld= 50이라는 값을
가지고 있습니다. 이 과정을 좀더 줄여 써 봅시다.

unsigned short int howOld = 50;// 변수를 만들
unsigned short int *pAge = &howOld;// 1104010의 포인터를 만듬

이제 pAger> 80\000의 주소를 저장하는 포인터입니다. 2486를 사용하여 여러분
은 실제적으로 10\000의 WS 알 수 있습니다. 포인터 pAge= 사용하여 10\010
에 접근하는 것을 간접 지정( abel 합니다. 왜냐하면 pAges 경유하여
howOld= 접근하기 때문입니다. 잠시 후 어떻게 간접 지정을 통해 변수의 Zhe]
접근하는지 알아보게 될 것입니다.


===== PAGE 230 =====
228 ee 제2주

새로운
응어

간접 지정0001(60000) 포인터에 지정된 주소값을 통해 원래의 변수에 접근하는
방식을 의미합니다. 포인터는 그 안에 지정된 주                      을

°
알 수 있는 WHE 방식을 MSE.

간접 지정 연산자

간접 지정000060000) 연산자(＊ )는 조회 연산자(4006009)라고도 부릅니다. 포
인터가 조회되었을 때 그 포인터에 저장된 주소에 있는 값이 검색됩니다. 일반적
인 변수들은 그 값에 직접 접근 BAS 제공합니다. 가령 Fete] yourAger} =
리는 unsigned short 정수형을 선언했다면, 여러분은 40\000의 WS 그 새로운 변
수에 저장할 수 있습니다.

unsigned short int yourAge;
yourAge = how0ld;

==
합니다. 포인터 pAgeS 통해 yourAges] howOld 값을 저장하려면 다음과 같이 합
니다.                3
unsigned short int yourAge;
yourAge = *pAge;
pAge 앞에 붙어있는 간접 지정 연산자(*)는 “이 주소에 저장된 WS 의미합니다.
따라서 둘째 줄은 다음과 같이 해석됩니다. '0486에 저장된 값(이는 FAS 가리
킴)을 가져와, 이 주소가 가리키는 곳으로 찾아가 저장된 값을 찾아 >00480에 저
장합니다.'

간접 지정 연산자(*)는 포인터에 있어서 두 가지 방식으로 쓰입니다. 포인터가 AAS
때 이 * 표시는 일반 변수가 아닌 포인터 변수임을 알려줄 때 쓰입니다. We 보면
unsigned short *pAge = 0;  // unsigned short 형 포인터를 만들

포인터가 소환될 때 간접 지정 연산자(*)는 포인터에 저장된 메모리의 주소갖이 가리

키는 실제 값을 찾아가게 합니다.



===== PAGE 231 =====
제8일 포인더 66 229

*pAge = 5 ;      // 2 SB 0066 안에 적장된 주소 위치에 저장하라.

이 * Wee 곱셈 연산자에서도 쓰이는데 다른 것입니다, 컴파일러가 문      을 보고

떤 연산자인지 알이냄디다.

포인터, 주소, 변수

포인터라는 변수와 그 포인터 Wo] 저장된 주소값 그라고 그 포인터 변수에
저장된 FAH] 가리키는 메모리를 찾아가면 장되어 있는 Aas, 이 세 가지
를 구별하는 것은 매우 중요합니다. 이 세 가지가 포인터에 관한 수많은 혼동의
원천이 되는 것입니다.
아래부분을 살펴봅시다.

int theVariable =5;

int *pPointer = &theVariable ;

theVariable? 52 .초기화된    a

소를 저장하는 포인터입니다.

pPointer=
pPointer7} 지닌

다. [리스트 8.31은
[그림 8.3]                                      thevariable
포인터에 관련된                |
메모리 그림표      변수명

포인터입니다.  ees
주소의 메모리를 SOPH 거기에는 5라는 값이 저장되어 있습니
이것을 그림으로 보여줍니다.

ee ee 여수

형 go] 저장되는 주

= (vei 주로 aS  있습니다.

저장된

ZARrmK

주소는 theVariableo]) 주소입니다.

pPointer

|

써)

010

oe

, 0000    ^ 10

|              ㅣ              |              00        1,
a,

000
<
101

|       |       |       !       !       |

100

주소위치

101    102

다다 사용한 자료 연산

수가 있습니다. [리스

103

수의 주소값을 할당받았다면, 그 변수

포인터는 어떻게 그 변수에 저장된 값을

104     105     106     107     108     109

의 자료에 접근하기 위해 여러분
트 8기는 지역 ara 주소가 어떻게 포인터
연산하는지 보여줍니다.


===== PAGE 232 =====
230 ee 제2주

[리스트 8.2] 포인터를 사응한 자료 연산

1: // [리스트 8.27 포인터를 사용한 자료 연산
2:

3: #include <iostream.h>

4:                          때
5: typedef unsigned short int( USHORT;
6: int main(                 )

C2 &

8:    USHORT myAge;     // 변수

9:  USHORT ®pAge =O // 포인터

10:   myAge = 57

Ti:   cout << "myAge: " << myAge << "\n";
128

13%   pAge = &myAge;

14:

15,   cout << " *pAge: " << *pAge << "\n\n";
16:                        :

102   cout << "*pAge = 7\n";

18:

19%   *pAge = 7; // sets myAge to 7

20:

21,   cout << "*pAge: " << *pAge << "\n";
22:   cout << "myAge: " << myAge << "\n\n";
23s:

24:

25   cout << "myAge = 9\n";

26:

are   myAge = 9;

28:

29:   cout << "myAge: " << myAge << "\n";
30:   cout << "*pAge: " << *pAge << "\n";
318

328    return 0;

S52)

결과   myAge: 5

*pAge: 5

*pAge = 7
xpAge: 7
myAge: 7

myAge = 9
myAge: 9
*pAge: 9



===== PAGE 233 =====
제8일 포인더 ee 231

=
unsigned short myAgeS 가리키는 - 를 선언하였습니다. myAgeE 10H 줄

에서 5가 할당되었고 이는 11번 줄에서 출력하며 확인되었습니다.

13번 줄에서 2486는 myAge®] 주소를 할당받았습니다. 15번 줄에서 2486는 조회

었고 출력되었습니다. pAge 저장된 주소가 가리키는 메모리에는 myAger] 저
장된 5라는 HO] 있습니다. 19번 줄에서 2486에 저장된 주소가 가리키는 값에 7
을 대입하였습니다. 이는 myAges] 값을 7로 Beech 21 - 22줄에서 출력하여
이를 확인하였습니다.

27번 줄에서 값9가 변수 myAges] 저장되었습니다. 29번 줄에서 직접 호출 방식
로 Ho] 얻어졌고 30번 SA] 간접 호출 방식으로 - pAgeS 소환하여 - HS

(aa

8 이 프로그램은 두 개의 변수 1098060 short myAgeS} 포인터 pAge -

포인터는 여러분이 주소를 - 실제 그 주소를 정확히 알지 못하더라도 - 연산할
수 있게 해줍니다. 오늘 이후로 포인터에 변수의 주소를 대입하면 그 주소가 대
입이 되고 그 포인터는 그 변수의 주소를 가지고 있다는 것을 자신 있게 알게 될

[리스트 8.3]을 살펴봅시다

[리스트 8.3] 포입터에 무엇이 저장되어 있는가?

// [리스트 8.3] 포인터에 무엇이 저장되어 있는가?
#include <iostream.h>

1

2

3

4:

5: typedef unsigned short int USHORT;
6:

7

8

int main()
{
unsigned short int myAge = 5, yourAge = 10;
Oe    unsigned short int * pAge = &myAge; // a pointer
10:

1   cout << "myAge:\t" << myAge << "\tyourAge:\t" << yourAge << "\n";

fz:   cout << "&myAge:\t" << &myAge << "\t&yourAge:\t" << &yourAge << "\n";
135

14:   cout << "pAge:\t" << pAge << "\n";

15:   cout << "*pAge:\t" << *pAge << "\n";

16:

17:   pAge = &yourAge;


===== PAGE 234 =====
232 ee Hae

18:

19:    cout << "myAge:\t" << myAge << "\tyourAge:\t" << yourAge << "\n";
20:   cout << "&myAge:\t" << &myAge << "\t&yourAge:\t" << &yourAge <<"\n";
ae

22: cout << "pAge:\t" << pAge << "\n";

252   cout << "*pAge:\t" << *pAge << "\n";

24:

25   cout << "&pAge:\t" << &pAge << "\n";

26: return 0;

272)

결과 myAge:       5       yourAge:   10
&myAge:         0x355C      &yourAge:   Ox355E
pAge:          0x355C
*pAge:          5
myAge:          5         yourAge:    10
&myAge:         0x355C      &yourAge:   Ox355E
pAge:          Ox355E
*pAge:          10
&pAge:          Ox355A
(여러분의 출력은 달라질 것입니다.)

분석  8번 줄에서 myAge?} yourAge= unsigned short 정수형     선언되었습니다.

9번 줄에서 2486는 unsigned short 정수형을 가리키는 포 포인  ae  선언되었습
니다. 그리고 그 값은 myAges] 주소로 초기화되었습니다.

11, 12번 줄은 myAgeS} yourAge®] 값과 주소를 출력합니다. 14번 SS 2486의 내
때 출력하는데 이는 myAges] 주소입니다. 15번 Se pAges 조회한 결과값을
하는데 myAgeo] 저장된 값 5입니다.

여기가 포인터의 핵심입니다. 14번 줄은 2486에 myAge 주소가 AAS 있음을
보여주고, 15번 줄은 포인터 2486를 조피함으로비 myAge] 저장된 값      방
법을 보여줍니다. 다음으로 나가기 전에 여기를 충분히 이해하십시오.

부하고 출력을 잘 살펴봅시다.

17번 줄에서 pAge= 다시 yourAge ©] 주소를 할당받았습니다. 주소와 값이 다시
출력됩니다. 이번에는 2486가 704486의 주소를 가지며 2486를 간접 지정 연산하

면 704486의 값을 얻음을 알 수 있습니다.

25번 BS 0486 그 자체의 주소를 출력합니다. 다른 변수와 마찬가지로 2486도

역시 주소를 가지고 있습니다. 그리고 그 주소 자체 또한 저장될 수 있습니다.(포

인터의 주소를 또 다른 포인터에 저장하는 방식은 나중에 또 이야기됩니다.)

Wy



===== PAGE 235 =====
DO 포인터가 가리키는 주소에 저장된 값에 접근하려면 간접 지정 연산자(*)를 씀
“Ft.
를 유표한 주소갔이나 널( 0 )로 초기화합시다.
즈
늘보

SUS} 그 FAS 메모리에 저장된 값을 구별할 줄 압시다.

포인터(60116)
선언하려면 저장되는 주소가 가리키는 값의 변수형 또는 객체형을 쓰고, 포인
쓰며 (*) 그 포인터의 이름을 Such.

a

unsigned short int * pPointet = 0;

0묘
i}
오
3
b>
r2
수
x

포인터에 값을 저장하거나 초기화할 때 저장하고자하는 주소의 변수
(&)를 붙여 대입합니다.

unsigned short int theVariable = 5 ;
unsigned short int * pPointer = & theVariable ;

포인터를 소환하려면 소환연산자(*)를 포인터 앞에 붙입니다.

unsigned short int theValue = *pPointer ;

도대체 왜 포인터를 쓰는가?

여태껏 여러분은 변수의 FAS 가리키는 포인터에 대해 자세히 배웠습니다. 그
으   24    Z

런데 여러분은 이렇게 복잡한 방식이 맘에 안들 것입니다. 왜 gol 직접 접근할
수 있는 변수가 있는데 포인터를 쓰는 것일까요? 위의 ae 단지 포인터가 어떻
게 연산하는지           쓴 것일 따름입니다. 여러분이 포인터의 구문에



===== PAGE 236 =====
234 eo 제2주

오늘은 자유 기억 공간  클래스 멤버 자료와 클래스 멤버 함수에 대해 배우고
내일 주소 전달 방식의 함수에 대해 배울 것입니다.

스택과 자유 기억 공간(『「66 Store)
5장에서 es 메모리의 57-2] 영역에 대해 배웠습니다.

를 자족 기억 공간
mars]

fo}
Bae 영역

를 스틱

지역 변수는 함수의 매개 변수와 함께 스택에 저장됩니다. SEE 코드 영역어
     전역 변수는 전역 공간에 저장됩니다. 레지스터는 여러 잡다한 일들을
합니다.(예를 들어, 스택의 꼭대기와 명령 포인 베버 계속 추적하는) 그리고 나머
지의 메모리는 자유 기억 공간(666 store) 분     는데 힙08680)이라고 불립니다.

———_-     매매               Se aaa

8수의 Bade 영원히 지속되지 않는다는 것입니다. 함수가 반환되면 지
수들은 버려집니다. 또한 전역 변수들은 그 문제를 해결했지만 프로그럼의

Hes 제한 없이 det 수 있다는 aH 치러야 합니다. 이는 앞서 본
이 이해하기 어렵고 유지 보수를 어렵게 합니다.

를 자유 기억 공간에 넣어두면 양쪽의 두 가지 문제가 해결이 됩니다.

tt 719 공< 공간이란 다량의 메모리 집합으로 생각하면 되는데 거기에는 여러분이
는, 순차적인 번호가 붙은 방들이 수없이 있습니다. 여기에
스택과 같이 MIRE 붙일 수가 없습니다. 하지만 여기에는 여러분이 비축해
놓은 방들의 FAS 원할 수 있고, 여러분은 이 주소를 포인터에 저장할 수 있는

것입니다. 비유적으로 설명해 봅시다.

전화기에는 메모리 기능이 있습니다. 김군 집의 전화번호는 1번 단추에, 이
의 전화번호는 2번 단추에 기억을 시켜 넣는 것입니다. 이렇게 하면 여러분
# 집에 전화를 gen 일일이 그 번호를 다 des 하지 않아도 됩니다 그 전
화번호는 어디 구석에 넣어돕니다. 여러분이 번호 하나만 누르면 전화가 알아서
찾아가 줍니다. 그 자세한 전화번호는 무엇인지 모릅니다. 하지만 그 집에 통화는
할 수 있습니다.

=

|

i

06 AH
pM oN

ㅇ

씀



===== PAGE 237 =====
제8일 포인더 ee 235

여러분은 컴퓨터의 메모리에. 주소를 통해 접근할 수.있습니다. - 이는 실제 전화
번호입니다. 하지만 여러분은 실제 메모리의 주소를 몰라도 됩니다. 단지 포인터

에 잡아넣으면 됩니다. - 특정 번호만 누르면 됩니다. 포인터는 여러분이 여러분
의 자료에 자세한 SAS 몰라도 접근할 수 있게 하여줍니다.

AG9) WEL 함수가 반환되면 자동적으로 지위집니다. 모든 지역 변수는 범위 규
4g 벗어나게 되고 그들은 스텍에서 지위집니다. 자유 기억 Bae 여러분이 여러
분의 프로그램을 끝낼 때까지 지워지지 않습니다. 여러분이 여러분의 메모리 사용
을 끝냈을 때 그 공간을 유지하느냐 뻐리느냐는 여러분의 책임이 되어버립니다

자유 기억 공간의 이점은 여러분이 그 공간을 외형상 명백히 풀어놓을 때까지는
여러분을 위해 보관된다는 것입니다. 여러분이 어느 함수에서 자유 기억 공간에
메모리를 잡아놓으면 그 함수가 끝나도 그 공간은 잡혀 있습니다.

이러한 방식으로 메모리에 접근하는 방식이 전역 변수를 사용하는 것보다 좋은
점은 단지 그 포인터에 접근할 수 있는 함수만이 자료에 접근할 수 ie AY
너다. 이런 방식은 해당자료에 철저히 통제된 방식의 인터페이스를 제공하고, oF
무런 함수가 대책 없는 방향으로 자료들을 바꾸는 것을 막아줍니다.

이런 작업을 하기 위해 여러분은 자유 기억 공간을
있어야 하고 그 포인터를 필요로 하는 함수에게 전달해 주어야 합니다. 다음의
설명

te

% | oN

new

여러분은 20\라는 예약어를 통해 자유 기억 공간에 메모리를 할당할 수 있습니
다. new 다음에 여러분이 할당하기 원하는 객체의 Bs 써, 컴파일러로 하여금
얼만큼의 메모리가 필요한지를 알려줍니다. 따라서 여러분이 new unsigned short
파라고 쓰면 컴파일러는 자유 기억 공간에 2바이트의 메모리를 할당하고 new
1008이라고 하면 4바이트를 할당합니다.

10\로부터 반환되는 것은 Gwe] 주쇼입니다. ©  ote 포인터에 할당되어야 합니

다. 자유 기억 장소에 unsigned short 정수형을 만들려면 이렇게 합니다.

unsigned short int * pPointer;
pPointer = new unsigned short int ;

여러      론 포인터를 만들면서 초기화를 할 수 있습니다.

unsigned short int *pPointer = new unsigned short int ;

re
ro


===== PAGE 238 =====
236 ee 제2주

어느 경우  별 pPointer= 자유 기억 공간 상의. unsigned shot 정수형을 포인트합니
다. 이렇게 하여 여러분은 이 포인터가 WES 지정하게 하고, 그리고 Hee 다
음과 이 메모리에 저장할 수 있습니다.

*pPointer = 72 ;

는 곳에 2S 대입하라'라고 하던가 또는 '72를 자유 기억
공간 상의 pPointer7} 포인트하는 곳에 저장하라"라고 말할 수 있습니다.

~

수

없다면 - 메모리도 결국은 F
계가 있으니까 - 널 포인터를 반환합니다. 여러분은 새로운 메모리를 요구할 af

다 이를 검사해야 합니다.

new “NFS 사용하여 메모리를 tet 떼마다 포인터가 널이 아님을 왁인해야 합

al

delete

여러분의 메모리를 가지고 작업을 다했으면 그 포인터를 0666를 사용하여 반환

해야 합니다. 포인터 그 자체는 - 포인터가 가리키는 메모리가 아니라 포인터 변

수 그 자체 - 지역 변수입니다. 포인터가 선언된 함수가 반환되면, 그 포인터는

범위 규칙을 벗어나고 효력을 상실하게 됩니다. 하지만 news 통해 할당된 메모
는 자동적으로 풀어지지는 않습니다. 그 메모리 부분은 못쓰게 됩니다. 이 상황

을 가리켜 메모리 누출00600 1600'이라고 부릅니다. 즉, 프로그램이 끝나기 전

까지 이 메모리는 쓰여질 수가 없기 때문에 “메모리 +e ole} 불리는

다. 이는 여러분의 컴퓨터에서 메모리가 누출된 것과 똑같은 의미입니다.

메모리를 다시 자유 기억 장소로 돌려보내기 위해서는 예약어 deletes 사용합니다.
delete pPointer ;

EES deleteYS 때 실제 일어나는 일은 여러분의 포인터에 저장된 주소의 메
리가 자유 기억 Baz 다시 반환된다는 것입니다. 이 포인터가 가리키던 메모
를 자유 기억 장소로 반환하라'라고 명령을 내린 것입니다. 이때 포인터는 그대

포인터 0 여기에 다른 값을 할당할 수 있습니다. [리스트 8.4]가 힙에 변수
할당하고 그 변수를 사용하다 반환하는 예를 보여줍니다.

“ fd He


===== PAGE 239 =====
제8일 포인더 ee 237

deleteS 하면 포인터가 가리키던 메모리 부분이 풀어집니다. 여기서 다시 deletez wl?
면 여러분의 프로그램이 깨집니다. 여러분이 포인터를 0606하면 널(0)로 설정하여 버
리십시오, 널 포인터를 0666하는 것은 괜찮습니다.

Animal *pDag = new Animal ;

delete pDog ;     // 메모리를 반환
0009 = 0;// 포인터를 널로 막음
delete pDog ;     // 아무 이상 없음

[리스트 8.4] 포입터에 자유 기억 장소 할당 및 사응, delete

1: // [리스트 8.47 포인터에 자유 기억 장소 할당 및 사용, gelete
2877

St

4: #include <iostream.h>

5: int main()

6: 1

he   int localVariable = 5;

8: int @#Local=(BLogal Variable;

0s   int * pHeap = new int;

10: if (pHeap == NULL)

1418 해

125     cout << "Error! No memory for pHeap!";
1S:     return;

148 +}

15:  *pHeap = 7;

16: cout << "LocalVariable: " << LocalVariable << 도
17: cout << "*pLocal: " << *pLecal << a =
18: cout << "*pHeap: " << *pHeap << HAV hae

19: delete pHeap;

20: pHeap = new int;

21: if (pHeap == NULL)

22: 에

25:     cout << "Error! No memory for pHeap!!";
24:     return;

20 5

26: *pHeap = 9;

27: cout << "*pHeap: " << *pHeap << oN s

28: delete pHeap;

29: return 0;

WN
oO
wy



===== PAGE 240 =====
238 eo 제2주

겔과  lLocalVariable: 5

*pLocal: 5
*pHeap: 7
*pHeap: 9

셀  7번 줄은 지역 변수를 선언, 초기화합니다. 8번 줄은 포인터를 선언

지역 변수의 주소로 초기화합니다. 9번 SS 포인터를 또 하나 만든 두
수형을 70\로 호출하여 얻어진 결과로 초기화합니다.(자유 기억 장소의 메모리?
니다.) 10번 줄은 메모리가 할당되었고 포인터가 유효하다는 AS 보여줍니다.(
nullo] 아니었습니다.) 만일, 메모리가 할당되지 않는다면 포인터는 널이 되고 오
류 메시지가 출력이 됩니다.

간단히 하기 위해 이 오류 AWARE 다음 프로그램부터는 안 적을 것입니다. 하지
만 여러분은 여러 종류의 오류 검사 과정을 여러분의 프로그램에 적어야 합니다.

15번 줄은 7이란 BS 새로 할당된 메모리에 잡아 넣습니다. 16번 Se 지역 변

를 출력하고, 17번 SS pLocalo] 의해 포인트되는 RS 출력합니다. 생각대로
같습니다. 18번 BS pHeapo 의해 포인트된 값을 출력합니다. 15번 줄에서 대입
된 값을 보여줍니다.

19번 줄에서는 9번 줄에서 할당된 메모리를 deletes 호출함으로써 반환합니다.
이렇게 하여 메모리가 풀어지고 포인터는 그 메모리 번지와 무관하게 됩니다.
pHeapt 이제 다른 메모리 주소를 할당할 수 있습니다. 20, 26번 줄에서 같은 과
정이 되풀이 되었고, 27번 줄에서 결과를 출력하였으며, 28번 줄에서 deletes] Rs
니다.

사실 28번은 불필요한 과정이지만 - 프로그램의 끝에 가서는 잡혀진 메모리는 반
환됩니다. - 이렇게 명시적으로 Weds 풀어놓는 것은 아주 잘한 일입니다. 만
일 프로그램이 나중에 바뀌거나 확산된다면 위의 예제처럼 한 것이 아주 잘하게
된 것입니다.

(aa
An (원
ro of Ad

ms +>

메모리 + (Memory Leak)

메모리가 누출되는 또 다른 경우는 여러분의 포인터를 0866하기 전에 다른 값을
그 포인터에 대입하는 경우입니다. 이 부분을 봅시다.

1: unsinged short int *pPointer = new unsigned short 106 =
2: *pPointer = 72 ;


===== PAGE 241 =====
Ase 포인더 ee 239

WN

pPointer = new unsigned short int ;
: *pPointer = 84 ;

>

1번 줄에서 pPointers 만들고 자유 기억 장소의 한 부분의 sre 할당하였습
다. 2번 줄에서 72라는 값을 그 메모리에 대입하였습니다. 3번 줄에서 000000에
다른 메모리 FAS 할당하였습니다. 4번 줄에서 84라는 값을 그 메모리에 집어
넣었습니다. 윈래의 영역은 - 72라는 ge] 지금 저장되어 있는 - 원래 포인터에
다른 메모리 번지가 들어가 있는 이유 때문에 사용할 수가 없습니다. 원래의 메

모리에 접근할 방법이 없습니다. 프로그램이 끝날 때까지 그 영역을 풀어놓을 방

원래 코드는 다음과 같이 쓰여져야 했습니다.

1: unsinged short int *pPointer = new unsigned short int ;
2: *pPointer = 72 ;

3: delete pPointer ;

4: pPointer = new unsigned short int ;

5 *pPointer = 84 ;

맨 처음에 할당되었던 0006 메모리는 004006된 후 다시 할당되었습니다.

이런 064를 SEU 매마다 delete “HLA 언벤가는 사옥이커야 IM. rt
가리키는 메모리의 영역을 계속 주적해야 합니다. 그리고 여러분은 그 메모리에 대한
SUS 끝낸 루 자유 기억 장소로 폴어놓아야 합니다

_—
자유 기억 장소에 랙체 만들기
정수형에 포인터를 만들 수 있는 것처럼 언떠핫 객체에도 포인터를 만들 수
니다. 여러분이 08이라는 형의 객체를 만들        분은 그 클래스를 가
는 포인터를 선언하고 또 힙에 Cats] 객체들을 만들어 포인터에 저장할 수
니다. 구문은 정수형 만들 때와 똑같습니다.

Cat *pCat = new Cat ;

이 호출은 기본 생성자를 스택이나 힙에 Ws. - 매개 변수를 갖지 않는
생성자. 생성자는 객체가 만들어지는 어느 곳에서나 호출됩니다.

ay
00
d
fu

x9 |
a
Bh
요
또

르면 xO
피복 ly


===== PAGE 242 =====
240 ee 제2주

7HX delete

힙의 객체를 가리키는 포인터를 0066하면 객체의 소멸자가 먼저 호출되고 다음
에 메모리가 풀려집니다.086056) 이는 여러분의 클래스가 깨끗이 BER 기회를
마치 스택에서 객체가 없어지는 것과 마찬가지로 - 주는 것입니다. [리스트 8.5]는

자유 기억 장소에서 객체를 만들고 00066하는 YS 보여줍니다.

[리스트 8.5] 자유 기억 공간 상에 AAS 만들고 삭제하기

1: // [리스트 8.53 자유 기억 공간 상에 WHS 만들고 삭제하여 보자
Zu 7/

3:

4: #include <iostream.h>

5

6: class SimpleCat

Gt

8: public:

9: SimpleCatQ);

10: “~SimpleCatQ;

11: private:

12: int itsAge;

1333

14:

15: SimpleCat::SimpleCat()

168 1

17: cout << "Constructor called.\n";
18: itsAge = 1;

195 +}

20:

21: SimpleCat::~SimpleCat(

228: £

23: cout << "Destructor called.\n";
243 3

25:

26: int main()

OTe <

28: cout << "SimpleCat Fresky...\n";
29: SimpleCat Frisky;

30: cout << "SimpleCat *pRags = new SimpleCat...\n";
31: SimpleCat * pRags = new SimpleCat;
32: cout << "delete pRags...\n";

33: delete pRags;

34: cout << "Exiting, watch Frisky go...\n";

WN
uv

i}



===== PAGE 243 =====
제일 포인터 ee 241

겔과  SimpleCat Frisky...

Constructor called.

SimpleCat * pRags = new SimpleCat..
Constructor called.

delete pRags...

Destructor called.

Exiting. watch Frisky go...
Destructor called.

Hd

분석  6 - 13번 줄까지 90001608의 클래스를 선언하였습니다. 9번 SS SimpleCat

의 생성자를 선언하였고 15 - 19번 줄에서 AAAS 정의하였습니다. 10번

줄은 91001608의 소멸자를 선언하였습니다. 21 - 24번 SO 소멸자를 정의하였습

니다. 29번 SoA] 8096는 스택 상에 만들어 졌고 생성자가 호출됩니다. 31번 줄

에는 28885에 의해 포인트되는 540201608이 힙에 만들어지고 생성자가 다시 호출

되었습니다. 33번 줄에서 70888에게 소멸자가 호출되었습니다. 함수가 끝나면
Frisky 범위 규칙을 벗어나게 되고 소멸자가 호출됩니다.

자료 멤버(02413 Member)o] 접근

여러분은 점 연산자를 이용하여 지역적으로 선언된 Cato] 객체의 멤버 자료와 멤 ㆍ
버 함수에 접근하였습니다. 힙의 Cat 객체를 접근하려면 여러분은 포인터를 소환
해야 하며 포인터에 의해 포인트된 객체에 점 연산자를 사용해야 합니다. 좀 복
잡해 보이는데 GetAge 멤버 함수에 접근하려면 이렇게 쓰면 됩니다.

(*pRags) . GetAge() ;

소괄호가 쓰여야하는데 이는 0844860가 접근되기 전 먼저 pRag7} 소환되게 하기
위해 쓰여졌습니다. 이 과정은 좀 따분하므로 0++에서는 간접 접근 방식을 위해
좀더 간단하게 표현했습니다. BIE 연산자입니다( -> ) 이는 '-' 기호다음에 >
를 곧바로 붙여서 사용합니다. CHE 이것을 하나의 기호로 인식하므로 주의해야
합니다. [리스트 8.612 힙에 만들어진 멤버 함수와 멤버 변수에 접근하는 wae
보여주었습니다.

|

[리스트 8.6] 자유 기억 공간 상에서 AO] 멤버 자료에 접근하여 봅시다.

// [리스트 8.61 자유 기억 공간 상에서 Ways] 멤버 자료에 접근하여 봅시다.
ne

1

2

3:
4: #include <iostream.h>
5


===== PAGE 244 =====
242 ee 제2주

6: class SimpleCat

(is

8: public:

9:    SimpleCat() {itsAge = 2; }

10:   ~SimpleCat() {}

11%   int GetAge() const { return itsAge; }

12:   void SetAge(int age) { itsAge = age; }

13: private:

14:   int itsAge;

158 23

16:

17: int main()

1821

19%   SimpleCat * Frisky = new SimpleCat;

20:   cout << "Frisky is " << Frisky->GetAge() << " years old\n";
215   Frisky->SetAge(5);

22:   cout << "Frisky is " << Frisky->GetAge() << " years old\n";
25:   delete Frisky;

Zac   return 0;

255 >

QM ey nsyann
24 '  19번 줄에서 힙에 SimpleCat2] 객체가 만들어졌습니다. 기본 생성자는 ageS
로 설정하였고 GetAge) 메쏘드가 20번 줄에서 호출되었습니다. 8090는
auras 멤버 함수와 멤버 자료에 접근하기 위해 간접 지정 연산자(->)가 At
용되었습니다. 21번 SHA] SetAge() 메쏘드가 호춤되었고 22번 줄에서 GetAge()7}
다시 접근되었습니다.

자유 기억 공간의 멤버 자료에 대해
하나 이상의 ul 자료가 자유 기억 공간의 AAR 가리키는 포인터가 될 수
습니다. 이 메모리는 클래스의 생성자나 혹은 그 메쏘드에 할당될 수 있으며
래스의 소멸자에서 삭제될 수 있습니다. [리스트 8.71을 봅시다.

my 32

[리스트 8.7] 멤버 자료로서의 포인터

1: // [리스트 8.73 멤버 자료로서의 포인터
os Si

Ss

4: #include <iostream.h>



===== PAGE 245 =====
제8일 포인터 ee 243
58
6: class SimpleCat
c: 4
8: public:
9:    SimpleCat();
10:   “SimpleCat();
i   int GetAge() const { return *itsAge; }
WZ   void SetAge(int age) { *itsAge = age; }
1208
14:   int GetWeight() const { return *itsWeight; }
15:   void setAge(int weight) { *itsWeight = weight; }
16:
17: private:                                            「
18:   int * itsAge;
19%   int * itsWeight;
20: Dy;
21:
22: SimpleCat::SimpleCat()
235 <:
24:   itsAge = new int(2);
Zoe   itsWeight = new int(5);
262 }
ore
28: SimpleCat::~SimpleCat()
292 £
30:   delete itsAge;
308   delete itsWeight;
52s: 3
55:
34: int main()
358 +"
36:   SimpleCat *Frisky = new SimpleCat;
S7:   cout << "Frisky is " << Frisky->GetAge() <<" years old\n";
38:   Frisky->SetAge(5);
So:   cout << "Frisky is " << Frisky->GetAge() <<" years old\n":
40:   delete Frisky;
41:   return 07;
42: }
결과  Frisky is 2 years old
Frisky is 5 years old
분석  클래스 SimpleCato] 두 개의 멤버 변수 - 둘 다 정수형 포인터입니다 - 를
~    갖도록 선언되었습니다. 22 - 268 So] 생성자에서 힙에 기본값을 갖도록

초기화됩니다.


===== PAGE 246 =====
244 ee 제주

28 - 32번 줄의 소멸자에서 할당된 메모리를 방출합니다. 소멸자이기 때문에 포인
터에 널을 대입할 필요는 없습니다. 더 이상 접근할 필요가 없기 때문입니다.
06166된 포인터는 널을 대입해야 한다는 WAS 여기서는 무시해도 됩니다. 물론
Was 지켜 해 될 것은 없지만.…

호출 함수 - 이 경우 08400 - 는 16486와 itsWeight7} 자유 기억 공간을 가리키는
포인터인지     못합니다. main()-2- GetAge(, 9666860를 호출하기만 하고, 자세

알지
한 나머지는 모두 클래스에 감춰져 있으며 또 그래야만 합니다.

Frisky7} 40번 줄에서 0066되었고 소멸자가 호출되었습니다. 소멸자는 각 멤버
포인터를 삭제합니다. 만일 여기서 멤버 포인트들이 다른 사용자가 정의한 객체
를 포인트한다면 그 소멸자도 역시 호출됩니다.

나15라는 포인터

모든 클래스 멤버 함수들은 숨겨진 매개 변수들을 가지고 있습니다. 005라는 포

인터입니다. 이 006라는 포인터는 각 객체를 포인트 합니다. 따라서 각 GetAge()
나 961&860를 호출할   그             포인터가 숨겨진 매개 변수로 포함
되어 있습니다. 이 this 포인터를 명시적으로 쓰는 것이 가능하고 그 예가 [리스트

8.8|에 나와 있습니다.

[리스트 8.8] 106라는 포인터를 써봅시다.

1: // [리스트 8.83 thistt= 포인터를 써봅시다.

a: di

3:

4: #include <iostream.h>

58

6: class Rectangle

we 오

8: public:

9:    Rectangle();

108   “Rectangle();

11:   void SetLength(int Length) { this->itsLength = length; }
125   int GetLength() const { return this->itsLength; }
15:2

Th   void SetWidth(int width) { itsWidth = width; }
ER   int GetWidth() const { return itsWidth; }

16:

17: private:

18:   int itsLength;



===== PAGE 247 =====
제8일 포인더 ee 245

19:   int itsWidth;

20: 3;

212

22: Rectangle::Rectangle()

25% +

24:   itsWidth = 5;

Zoe   itsLength = 10;

26: +

27: Rectangle::~Rectangle()

25: {}

29:

30: int main()

312 ¢

52:   Rectangle theRect;

55:   cout << "theRect is " << theRect.GetLength() << " feet long.\n";
34:   cout << "theRect is " << theRect.GetWidth() << "feet wide. Nis
35:   theRect.SetLength(20);

36:   theRect.SetWidth(10);

371   cout << "theRect is " << theRect.GetLength()<< " feet long.\n";
38:   cout << "theRect is " << theRect.GetWidth()<< " feet wide.\n";
39:   return 0;

40: }

결과 theRect is 10 feet long.

theRect is 5 feet long.
theRect is 20 feet long.
theRect is 10 feet long.

EN AY SciLength()9} GetLength() 접근자 G4 Rectangle 객체의 ye 변수에 접근

하기 위해 명시적으로 005 포인터를 썼습니다. 하지만 SetWidtht} GetWidth
접근자는 쓰지 않았습니다. 각각에 대해 이해하기는 쉽지만 차이점이 없습니다.
005라는 포인터에 대해 이런 것이 모두라면 사실 귀찮게 08라는 포인터를 쓸 이

는 Base ele ep Ae 오대 이니 eee 게9으
강력한 도구로 쓰일 것 같습니다.

여러분은 10일째 공부 - 연산자 중첩 - 에서 이 008라는 포인터에 대해 자세히 공
부할 것입니다. 당분간은 이 048라는 포인터가 그저 무엇인지 정도만 알아돕시다.
이것은 객체 그 자체에 대한 포인터입니다.

건 그렇고 여러분은 이 thiseH= 포인터의 생성과 삭제에 대해 걱정할 필요가
습니다. 컴파일러가 알아서 해줍니다.


===== PAGE 248 =====
246 ee 제2주

실종된 포입터(58) or Dangling Pointer)

진짜 찾기 힘들고 어려운 버그는 ASA 포인터입니다. 이 실종 포인터는 여러분이

포인터에 대해 deletes 호출하여 이 포인터가 가리키는 메모리를 풀어준 뒤(600

나중에 그 포인터에 주소를 대입하지 않은 채 그 포인터를 쓸 때 일어납니다.

|는 전의 예에서 전화기에 저장된 전화번호가 헝클어졌을 경우와 마찬가지로 비

수 있습니다. 여러분은 메모리된 전화번호가 헝클어진지 모르고 1번 또는 2
누를 수 있습니다. 아무 일도 안 일어 날 수 있습니다. 하지만 잘못된 전화

} 『0통신에 연결되어 폭탄공장의 자동장치를 건드려 도시 전체가 날아갈
있습니다.

요약하면 deletes 메모리를 방출한 포인터를 쓰지 Yc. 이 포인터에는 그 전
니다. 이 메모리 주소를 쓰면 여러분의 프로그램이 깨질 수 있습니다. 더 안 좋은
경우는 여러분의 프로그램이 아무런 오류가 밭견됩이 없이 잘 돌다가 다른 곳에
서 죽는 경우입니다. 시한폭탄이 따로 없습니다. 그런데 웃을 일이 아닙니다. 안

전 제일주의로 나가기 위해 포인터를 삭제한 후 포인터를 널( 0 )로 지정합시다.
것이지

비유하면 포인터를 무장해제시키는 것이지요.

실종된 포인터를 영어로 48619109)포인터라 합니다.

°

7

4) fe fe Ho
Ht fot 406 ait rir

[리스트 8이는 실종된 포인터의 예를 듭니다.

[리스트 8.9] AFH SUAS 한번 만들어 봅시다.

1: // [리스트 8.91 실종된 포인터를 한번 만들어 봅시다.
28 77

3: typedef unsigned short int USHORT;

4: #include <iostream.h>

Ds

6: int main()

ti x

8:    USHORT * pInt = new USHORT;

0    *pInt = 10;

TOE   cout << "*pInt: " << *pInt << endl;
115   delete pInt;

en   pInt = 0;

os    long * pLong = new long;


===== PAGE 249 =====
제8일 포인더 ee 247

14:   *pLong = 90000;

15%   cout << "*pLong: " << *pLong << endl;
16:

17: -*pInt = 20; // 삭제되었는데. . .

18:

4)   cout << "xpInt: " << *pInt << endl;
20:   cout << "*pLong: " << *pLong << endl;
212   delete pLong;

22%   return 0;

23% J

겔과  *pInt:          10

*pLong:           90000
*pInt:            20
*pLong:           65556

(여러분의 결과는 물론 달라질 + 있습니다. 그 이유는 바로 알게 됩니다.)

8번 줄은 pint7} USHORTS 포인트하게 해놓았고, 0따는 새로이 메모리를
할당받았습니다. 9번 줄은 그 메모리에 10이라는 값을 할당하였고 10번 줄
에서 출력해 보았습니다. 그후 0066가 그 포인터에 호출되었고 0띠는 지금 실종
포인터가 되었습니다.

13번 SoA] 새로운 포인터 pLongs 만들었는데 news 호출하여 메모리에 주소
를 할당받았습니다. 14번 줄에서 ㅁㅁ008에 9000을 대입하였고 15번 Soja] 출력하
였습니다.

17번 줄에서 20이라는 값이 plnt7} 가리키는 메모리에 저장되었는데 여기서 따는
더 이상 유효한 FAS 가리키지 않습니다. pint7} 가리키는 메모리는 0666 호출
을 통해 풀어졌고 따라서 값을 대입한다는 것은 재난을 초래하는 것이 됩니다.
19번 줄은 plat? 프린트합니다. 20입니다. 20번 줄에서 ㅁ008의 BS 출력합니
다. 그런데 값이 갑자기 65556으로 바뀌었습니다. 두 가지 의문이 발생합니다.

1. 어떻게 pLong2| 값이 바뀌었는가? 누가 값을 건드렸는가?

2 17번 SAA pinto] 20을 HAWS 때 그 값은 어디로 가는가?

(rag

짐작하겠지만 두 개는 서로 엉켜있는 문제입니다. 17a 줄에서 값을 [때에 저장
하였을 때, 컴파일러는 아무 거리낌없이 20이라는 QS pla} 위에서 포인트 한
메모리 위치에 저장합니다. 그 메모리 주소는 11번 줄에서 풀어졌지만, 컴파일러
는 아무런 방해 없이 tS 저장할 수 있습니다. pLong7} 13번 줄에서 만들어졌을


===== PAGE 250 =====
248 ee 제2주

ot 20001 pla 폴어지기 전 메모리 위치가 저장됩니다.(물론 컴퓨터마다 다
르고, 다른 컴퓨터에서는 이런 일이 안 일어날 수 있습니다.) 20이라는 값을 과거
pint7} ee 주소에 저장함에 따라 그 값은 pLongel 의해 저장된 값을 go}
버렸습니다. 실종된 포인터를 쓴 대가입니다.

재미 삼아 어떻게 pLongZto] 65556이 나오는지 봅시다.

1. pint= 특정 메모리 위치를 가리키고 거기에 처음에 10이 저장됩니다.

2 pinto delete7} 호출되었습니다. 이는 전의 메모리 위치를 다른 포인터가 가져갈 수
있다는 얘기입니다. 그리고 pLongtt= 포인터가 그 위치를 가리키게 되었습니다.

3- 90000이 *pLongol 저장되었습니다. 저자가 예를 든 컴퓨터에서는 4바이트의 값
90,000 - 16진수로 00 01 5F 90 -을 메모리의 바이트 순서에 맞춰 집어넣습니다.
따라서 저장은 5F 90 00 01로 저장이 됩니다.

4ㆍ ”0210[에 20이 저장됩니다. - 00 14 -. pint= 아직 같은 FAS 가리키기 때문에
0!ㄴ000의 처음 두 바이트가 Hol 써지고 따라서 값은 00 14 00 01로 됩니다.

$ㆍ pLong2| 값이 출력됩니다. 바이트 순서에 맞춰 다시 뒤집으니 0) 01 00 14로 되었
고 005값으로 66556이 됩니다.

DONT

DON'T newt deleted 한 쌍씩 맞추는 것을 잊지 Bt
DON'T deletes 호줄한 뒤 포인터에 널을 집어 넣는 것을 잊지 Bt

const int * pOne ;
int * const pTwo ;
const int * const pThree ;

pOne= 상수형 정수에 대한 포인터입니다. 포인트된 H

rlo

변할 수 없습니다.


===== PAGE 251 =====
제8일 HIE ee 249

711069는 상수형 정수를 가리키는 상수형 포인터입니다. 포인트되는 값도 weg 수
로                                      eT EE

원칙은 0008라는 예약어의 바로 오른쪽 항을 상수형으로 보면 됩니다. Bo} const
의 오른쪽에 나오면 저장된 go] 상수형입니다. 변수명이 const 오른쪽에 오면 포
인터 변수 그 자체가 상수형입니다.

oot

const int *p1 ; // 포인트된 정수형이 상수형입니다.
int * const 02 ;// p2= 상수령이고 다른 주소값을 가리킬 수 없습니다.

const 포인터와 const 멤버 함수
6일째 날 기본 클래스 단원에서 여러분은 멤버 함수에 상수형을 지정하는 것을
배웠습니다. 함수가 0008형으로 선언되었을 때, 함수 안으로부터 객체의 자료를
바꾸려는 어떠한 시도도 컴파일러는 오류를 낸다고 하였습니다.
여러분이 포인터를 const 객체로 선언하면, 단지 그 포인터를 호출할 수 있는
KES const 메쏘드입니다. [리스트 8.10|]을 봅시다.

고

[리스트 8.10] const 랙체에 대한 포인터

// [리스트 8.103 const Wal] 대한 포인터
//

#include <iostream.h>

class Rectangle
{
public:
Rectangle();
“Rectangle();
void SetLength(int length) { itsLength = length; }
int GetLength() const { return itsLength; }

CONBDU FWD =
en se ss ee 00 00 00 00

3 RS 3 = = ~o
FWN | oO
… …… … … …

void SetWidth(int width) { itsWidth = width; }
56   int GetWidth() const { return itsWidth; }

16:

17: privates

18:   int itsLength;

1198   int itsWidth;


===== PAGE 252 =====
250 ee 제2주
203 35
21:
22: Rectangle::Rectangle():
232   itsWidth(5),
24:   itsLength(10)
25: <}
26:
27: Rectangle::~Rectangle()
28: {}
29:
30: int main()
312 £
32:   Rectangle* pRect = new Rectangle;
$5:   const Rectangle * pConstRect = new Rectangle;
34:   Rectangle * const pConstPtr = new Rectangle;
353
36:   cout << "pRect width: " << pRect->GetWidth(@) <<" feet\n";
St:   cout << "pConstRect width: " << pConstRect->GetWidth() <<" feet\n";
58%   cout << "pConstPtr width: " << pConstPtr->GetWidth() <<" feet\n";
395
40:   pRect->SetWidth(10);
41:   // pConstRect->SetWidth(10);
42:   pConstPtr->SetWidth(10);
43:
44:   cout << "pRect width: " << pRect->GetWidth@Q) <<" feet\n";
45:   cout << "pConstRect width: " << pConstRect->GetWidthQ <<" feet\n";
46:   cout << "pConstPtr width: " << pConstPtr->GetWidthQ) << " feet\n";
E(z   return 0;
48: }
결과  pRect width:              5 feet
pConstRect width:           5 feet
pConstPtr width:            5 feet
pRect width:                10 feet
pConstRect width:           5 feet
pConstPtr width:            10 feet

00

=]

=| 6 - 208 줄에서 Rectangles 선언하였습니다. 15번 줄에서 Getwidth) 멤버

메쏘드를 상수형으로 선언하였습니다. 32번 줄에서 포인터가 86080816을 가

리키도록 하였고 33번 SoA) pConstRectS 선언하였는데 이는 상수 Rectangles
가리키게 하였습니다. 34번 SS pConstPrS 선언하였고 이는 #60008910을 가리키
는 상수형 포인터입니다.



===== PAGE 253 =====
제8일 포인더 ee 251

36 - 38번 줄은 이 BSS 출력합니다.

40번 줄에서 pRect7} rectangle? 10으로 설정하도록 사용되었습니다. 41번 줄에서
pConstRect7} 사용되려고 하였으나 상수형으로 선언되어 그만두고 주석으로 막아
버렸습니다. 42번 줄에서 pConstPire 900\1000를 호출하였습니다. pConstPre
rectangles 가리키는 상수형 포인터로 선언되었습니다. 다른 말로 하면 포인터는
상수형이고 따라서 다른 주소를 가리킬 수 없지만 &6000916는 상수형이 아닙니다.

const this 포인터

로 선언할 때 여러분은 실질적으로는 006 포인터가 Bea 객체
것입니다. const this 포인터는 상수형 멤버 함수에서

lr rx

만 쓰

그

DO 객체갔이 바킬 수 있는 경우 일반형으로 설정, 전달합시다.
그만

DO 변하지 않는 조

to
i

포인터는 간접 접근 방식으로 자료에 접근할 때 강력한 도구를 제공합니다. 모든
변수는 주소를 가지고 있는데 이는 주소 연산자 &를 통해 얻을 수 있습니다. 이
주소가 EMEA 저장됩니다

포인터는 그 포인터가 가리키는 객체의 형을 쓰고 간접 연산자(*를 붙인 뒤 포
인터의 이름을 써서 완성시킴니다.

포인터는 객체, 또는 널을 가리키게 하여 추기화시킴니다.

간접 연산자(를 사용하여 포인터에 저장된 주소값을 접근합니다. 상수형 포인터
를 선언하여 그 포인터에 다른 객체의 주소를 대입할 수 없게 하고 또 상수형 a
체의 포인터를 선언하여 포인터가 가리키는 값을 바꿀 수 없게 할 수 있습니다.


===== PAGE 254 =====
252 ee 제2주

힙에 new AAS 만들어 포인터에 그 BS 대입할 수 있습니다. delete 예약어를
호출하여 메모리를 폴어놓을 수 있습니다. delete 메모리를 풀어놓지만 그 포인터
를        는 않습니다. 따라서 다른 주소값을 그 포인터에 저장할 수 있습니다.

Q 왜 포인터가 중요합니까?
A 오늘 여러분은 힙에 한 a 잡고 그 주소를 포인터에 저장하는 WS 배웠고, 주
소를 매개 변수로 전달하는 것을 보았습니다. 더 나아가 13일째에는 다항 클래스에

Q 왜 자유 기억 공간에다 선언하는 번거로움을 겪는지?

A 함수가 반환된 후에도 자유 기억 장소에 객체는 남아있습니다. 게다가 힙에 객체를
저장하는 것은 실행시 미리 선언한 뒤 사용하는 것이 아니라 필요에 따라 마구 메
모리를 잡아 사용할 수 있는 이점이 있습니다. 나중에 깊이 다룰 것입니다.

년,

Q 왜 ASS 선언할 때가 있습니까?
A 프로그래머로서 컴파일러가 버그를 잡도록 할 Ba 있는 7  nd 가 있습니다. 잡아내
기 정말 어려운 버그는 명백하게 함수를              를 바꾸는 함수입니다.

후
상수형으로 선언하면 바꿀 때 오류가 남으로 버그를 사전 +  Ae 수 있습니다.

연구

Ｌ 변수의 주소를 잡아내는데 쓰이는 연
2. 포인터가 가지고 있는 주소에 들어있는 값을
3. 포인터란 무엇입니까?

4. 포인터에 저장된 FA 그 주소에 저장된 값의 차이점은 무엇입니까?

|아내는데 쓰이는 연산자는?

no



===== PAGE 255 =====
제8일 포인더 ee 253

5S. 간접 연산자와 그 연산체의 주소와의 차이점은 무엇입니까?

he

6 const int * ptrOne*} int * const ptrTwo2| 차이점을 말하십시오.

연습 문제
1. 다음의 선언이 하는 일은?
a. int * 0006 ;
6. int vTwo ;

c. int * pThree = &vTwo ;

2 yourAgeFt= 이름의 unsigned short 변수를 가지고 있을 때 yourAge= 연산할
포인터를 어떻게 선언합니까?

3 2번에서 선언한 포인터를 사용하여 yourAgedl] 50을 할당하십시오.

4 정수

정수를 선언하고 그 정수를 가리키는 포인터를 선언하는 프로그램을 작성하십시오. 그
정수형의 주소를 포인터에 저장하십시오. 그 정수형 변수에 값을 저장하기 위해 포인터

#include <iostream.h>

int main()

{
int *pInt;                   >
kpInt = 9>                          깃당 ※×
cout << "The value at pInt: " << *pInt ;
return 0;

)

6 버그잡기

int main()

{
int SomeVariable = 5;
cout << "SomeVariable: " << SomeVariable << "나"
int *pVar = & SomeVariable ;

evar =9;       Rraiby

cout << "SomeVariable: " << *pVar << "\n" ;
return 0;


===== PAGE 256 =====


===== PAGE 257 =====


===== PAGE 258 =====
256 ee 제2주

서문
어제 여러분은 자유 기억 공간에 객체를 연산하는 포인터를 사용하는 법을 배웠
고 이 객체에 대한 간접 연산을 배웠습니다. 오늘의 주제는 포인터의 거의 모든
강력함을 제공하면서 좀더 쉬운 TES 가진 참조자00066009)에 대해 배옵니다.

참조자는 포인터와 무엇이 다른가

Z2t%TtreferenceyEt 무어인가?

참조자란 일종의 다른 이름 - 별칭 - 입니다. 여러분이 참조자를 만들 때 다른 4
체의 이름으로 - 이를 ephole} 합니다. - 초기화합니다. 그때부터 이 참조자는
이 E}Alo] 대한 다른 이름으로 행세합니다. 그리고 여러분이 이 참조자에게 가한
변화는 이 Eo) 가해집니다.

BAS 형을 쓰고 참조 연산자 & 다음에 참
만듭니다. 참조자는 변수 이름으로 쓸 수 있는 것은 모두 다 되는데,  「 책에서는
?'이라는 GS 접두어로 사용할 것입니다. 여러분이 5006따라는 정수형 변수명
을 가진다면 그 변수에 대한 참조자를 다음과 같이 만들 수 있습니다.

tH yy BN

int &rSomeRef = someInt ;

이는 ‘rSomeRef= somelIntS SEIS 초기화된 ASS 참조자이다'라고 AGU

다. [리스트 9.1]에서 참조자의 탄생 및 사용에 대하여 알아봅시다.

연산작(6)는 주소 연산자와 같은 기호이지만 같은 연산자는 아닙니다, 비록 상당
Az

되어있지만.

[리스트 9.1] 참조자 만들고 사응하기

1: // [리스트 9.17 참조자 만들고 사용하기
2: //


===== PAGE 259 =====
제9일 BAN ee 257

3:

4: #include <iostream.h>

a:

6: int main()

72

SF    int intOne;

oi    int &rSomeRef = intOne;

108

113    intOne = 5;

12:   cout << "intOne: " << intOne << endl;

131   cout << "rSomeRef: " << rSomeRef << endl;
14:

15:   rSomeRef = 7;

16:   cout << "intOne: " << intOne << endl;

17s   cout << "rSomeRef: " << rSomeRef << endl;
18:    return 0;

19: }

24 Df  intOne: 5

rSomeRef: 5
intOne: 7
rSomeRef: 7

분석 8번 줄에서 정수형 지역 WS} intOne7} 선언되었습니다. 9번 줄에서 그 a
수형에 대한 참조자 rSomeRef7} 선언되고 intOne=s 참조하도록 초기화되었

습니다. 참조자를 만들고 초기화를 하지 않는다면 컴파일러는 오류를 출력합니다.

조자는 반드시 초기화되어야 합니다.

11번 줄에서 intOneo] 5가 대입되었고 12 - 13번 줄에서 intOne2} rSomeRef2] 값

ㅣ 출력되었는데 그 둘의 값이 예상대로 같습니다.

15번 줄에서 7이라는 값이 rSomeRefo] 대입되었습니다. 이는 참조자이고 intOnes]
다른 이름이기 때문에 7°] 까006에 역시 대입되었고 16 - 17의 출력 값에서 또
증명이 되었습니다.

참조자에 주소 연산자 & 쓰기

참조자의 주소를 물어보면 그 eps] 주소가 반환됩니다. 이것이 참조자의 본질
입니다. Epa) 대한 또 다른 이름이기 때문입니다. [리스트 92S 봅시다.


===== PAGE 260 =====
258 ee 제2주

[리스트 9.2] ATO] FAB 알아보자.

// CAE 9.21 참조자의 주소를 알아보자.

//
#include <iostream.h>

int main()
£
int intOne;
93    int &rSomeRef = intOne;
10:
11%    intOne = 5;
12:   cout << "intOne: " << intOne << endl;
132   cout << "rSomeRef: " << rSomeRef << endl;
14:
152   cout << "&intOne: " << &intOne << endl;
16:   cout << "&rSomeRef: " << &rSomeRef << endl;

1:
2:
3%
4:
5
6:
14
8:

Tt:
18:   return 0;
19: }
겔과 intOne: 5
rSomeRef: 5
&intOne: 0x3500
&rSomeRef: 0x3500
여러분의 컴퓨터에서는 밑의 두 줄의 출력이 달라질 수 있습니다
분석  여기의 예에서도 rSomeRef= intOneS 참조하도록 초기화되었습니다. 여기
re                   _                               =
서 두 변수의 주소가 출력되었는데 그 Se 똑같습니다. cHoye 참조자
그 자체의 주소에 접근하는 방법을 제시하지는 않는데 이는 의미가 없기 때문입

니다. 참조자는 만들어질 때 초기화되고 그 Epo] 대한 동의어로 여겨지는데 주

소 연산자를 쓸 때에도 그렇습니다.

예를 들어, Presidemeh= '클래스를 여러분이 가지고 있다면 그 클래스의 객체를

다음과 같이 선언합니다.

President William_Jefferson Clinton;

oz] President?] FAAS 다음과 같이 선언하고 초기화할 수 있습니다.

President &Bill_ Clinton = William_Jefferson Clinton;



===== PAGE 261 =====
제9일 AAA ee 259

President 변수는 하나입니다. 그러나 두 개의 식별자가 클래스의 같은 객체를 접
2344. Bill_Clintono]] 가하는 변화가 William_Jefferson_Clintono] = 가해집니다.

9번 줄의 & 기호를 15, 16번 줄의 intOnes} rSomeRefol] 쓰인 & 기호와 구별할 줄

알아야 합니다. 뒤의 & 기호는 주소 연산자입니다.

참조자를 쓸 때엔 주소 연산자를 쓰진 않습니다. 단지 A 변수를 쓰듯이

AS BUC. 13번 줄에 있습니다.

}조자는 다시 대입될 수 없고 그 Epo] 대한 다른 이름이라는 사실을 잘 아는
련된 Ctt 프로그래머조차도 여러분이 참조자에 다른 값을 다시 설정하려 하는

혼란을 겪는 경우가 많습니다. 다른 값을 대입을 하는 경우 나타나는 ae A
로운 값  ke EVA 대입되는 것처럼 보입니다. [리스트 9.31이 이를 보여줍니다.

주

aM

[리스트 9.3] 참조자에 대입하기

// [리스트 9.37 참조자에 대입하기
//

#include <iostream.h>

int main()
a
int intOne;
Or    int &rSomeRef = intOne;

11:   intOne = 5;

12:   cout << "intOne:\t" << intOne << endl;    5
15:   cout << "rSomeRef:\t" << rSomeRef << endl; 5
14:   cout << "&intOne:\t" << &intOne << endl; —
15%   cout << "&rSomeRef:\t" << &rSomeRef << endl; —

a WAR   int intTwo = 8;
18:   rSomeRef'= intTwo; // not what you think!

19:   cout << "\nintOne:\t" << intOne << endl;
20;   cout << "intTwo:\t" << intTwo << endl;
21%   cout << "rSomeRef:\t" << rSomeRef << endl;

228   cout << "&intOne:\t" << &intOne << endl;

25°   cout << "&intTwo:\t" << &intTwo << endl;

24:   cout << "&rSomeRef:\t" << &rSomeRef << endl;
25%   return 0;



===== PAGE 262 =====
260 ce 제주

결과 intOne:             5
rSomeRef:                 5
&intOne:                 0x213e
&rSomeRef:                0x213e
intOne:                  8
intTwo:                  8
rSomeRef:                 8
&intOne:                 0x213e
&intTwo:                 0x2130
&rSomeRef:                0x213e
불셀 8, oe 중에서 또 한 번 정수형 변수가 선언되었고 그 정수형에 대한 참조
~ 자가 선언되었습니다. 11번 줄에서 이 베이 5 5가 대입되었고 12 - 15번
줄에서 그들의 값과 주소가 출력되었습니다.
17번 SoA, 새로운 WS intTwo7} 만들어지고 8로 초기화가 되었습니다. 18번 |S

에서

하였습니다. 그러나 무산되었습니다.

프로그래머는 79006#하를 10[1“0의 다른 이름으로 만들기 위해 대입을 시도

단지 rSomeRef= intOne2] E}Ae] 역할을 하

면서 단지 다음과 같은 일을 하게 된 것입니다.

intOne = intTwo ;

19 - 214 줄에서 intOneS} rSomeRef7} 출력
다. 그러나 22 - 24번 줄에서 그들의
다는 108006의 BS 계속 가지고 있었습

되었을 때 그 Be intTwos} 같았습니
AAT} 출력되었을  rSomeRefE intTwok

                 DON'T
DO. 객체에 대한 다른 이름을 만들 때 참조자를 사용합시다.
00 모든 참조자는 로기화해야 합니다.
DON'T 참조자를 재치환하려 하지 BEAL ET.
DONT 24 연산자와 참조 연산자를 론동하지 Blt.
무엇이 참조될 수 있는가?
사용자가 정의한 AIS 포함하여 아무 객체나 참조될 수 있습니다. 참조자를 클
래스가 아니라 객체에 대해 만들 수 있음을 주목하십시오. 다음은 안됩니다.

‘int & rIntRef = int ;// 잘못


===== PAGE 263 =====
제9일 HAAN ee 2061

rntRef= 다음처럼 특정의 정수형으로 초기화해야 합니다.

int howBig = 200;
int & rIntRef = howBig ;

같은 방식으로 여러분은 참조자를 CATS 참조하도록 만들 FE 없습니다.
CAT & rCatRef = CAT ;// 잘못              rattance 2 Arbetavok ay .
rCatRef= 특정의 CATS] 클래스로 초기화해야 합니다.

CAT frisky ;
CAT & rCatRef = frisky ;

객체에 대한 참조자는 객체 그 자체처럼 사용됩니다. 멤버 자료와 메쏘드는 클래
스 멤버 접근 연산자()를 사용하여 접근될 수 있습니다. 그리고 참조자는 그 객
체에 대해 다른 이름으로 사용됩니다. [리스트 9.4|가 예를 보여줍니다.

[리스트 9.4] 랙체에 대한 참조자

1: // 리스트 9.4] Wao] 대한 참조자

2: //

3

4: #include <iostream.h>

5:

6: class SimpleCat

te 에

8: ‘public:

9:    SimpleCat (int age, int weight);
10:   “SimpleCat() {}

11:   int GetAge() { return itsAge; }

12;   int GetWeight() { return itsWeight; }
13: private:

14:   int itsAge;

158   int itsWeight;

16: }s

17%

18: SimpleCat::SimpleCat(int age, int weight)
192 <

202   itsAge = age;

21:   itsWeight = weight

222 J

25%

24: int main()

25: 1

26   SimpleCat Frisky(5,8);

ar?   SimpleCat & rCat = Frisky;


===== PAGE 264 =====
262 ee 제2주

28:

29:    cout << "Frisky is: ";

50:   cout << Frisky.GetAge() <<" years old. \n";
B1:    cout << "And Frisky weighs: ";

32:   cout << rCat.GetWeight() << " pounds. \n";
335%   return 0;

54: 2

결과  Frisky is: 5 years old.

and Frisky weighs 8 pounds

@ 264 줄에서 Frisky: SimpleCato] 객체로 선언되었습니다. 27H 줄에서

SimpleCat2] 참조자 1Cato] 선언되었고 8096로 초기화되었습니다. 30번과
32번 줄에서 SimpleCat 접근자 메쏘드가 SimpleCat 객체를 사용하여 접근되었고,
91001608의 참조자를 통해 접근되었습니다. 양쪽 다 똑같습니다. 다시 한 번 말
하되 참조자는 실제 객체에 대한 참조자입니다.

(aa

참조자

참조자는 다음과 같이 선언합니다. BS 쓰고 참조 연산자(&)를 쓴 뒤 참조자 USS F
니다. 참조자는 처음 만들어질 때 초기화됩니다.

예제 1

int hisAge;
int &rAge = hisAge;

예제 2

CAT boots;
CAT & rCatRef = boots;

널 포인터와 널 참조자

포인터가 초기화되지 않았을 때 혹은 삭제되었을 때 BE 치환되어야 합니다. 참
조자에서는 이게 아닙니다. 사실 참조자는 널로 될 수가 없습니다. BS 참조하는
참조자는 잘못된 프로그램입니다. 이런 때는 별일이 다 일어납니다. 잘 동작되는
같기도 하고 혹은 여러분의 디스크를 yas 수도 있습니다. 다 잘못된 프로
그램이 할 수 있는 일입니다.

스


===== PAGE 265 =====
제9일 SAA ee 263

대부분의 컴파일러는 오류 메시지 없이 널 객체를 지원하는데, 실제 사용하려고
하면 깨집니다. 설혹 이런 일이 없다손 치더라도 이 프로그램을 다른 컴파일러
또는 컴퓨터로 옮기면 장애가 일어납니다.

함수 인수(6@/9400604를 참조자로 전달하기
5일째 학습에서 함수는 두 가지 한계를 가지고 있다는 점을 배웠습니다. 하나는

매개 변수가 값으로 전달되는 것이고, 다른 하나는 반환값은 단 하나밖에 없다는
eo 이여 직 아
것입니다.

참조자를 이용하여 WSS 함수에 전달하면 이 두 가지 한계를 극복할 수 있습니
다. 0++에서 참조자 전달 방식은 두 가지로 일어납니다. 하나는 포인터로 전달하
는 것이고 다른 하나는 참조자로 전달하는 방법입니다. 사용하는 구문 방식은 다
릅니다. 하지만 효과는 같습니다. 함수의 범위 규칙 내에서 값이 복사되는 것이
아니라 진짜 객체가 함수로 전달이 됩니다. 참조자를 전달하는 방식은 함수로 하
여금 그 객체를 변화시킬 수 있게 합니다.

—

mut

ay

i a

는 주소                  스택엔 아무 것도 없게 됩니다.
러는 윈래의 객체에 도달하는 방법을 알고 그 객체에 변화를 가하
}하는 것이 아닙니다.

그
3

[리스트 5.5]를 상기해 봅시다. swap) 함수는 호출한 함수의 값을 바꾸지는 않습

니다. [리스트 5.5]가 편의상 여기에 다시 쓰여졌습니다.

[리스트 9.5] (5.5) 값 전달 방식의 예

// CHAE 9.5] (5.5) Bt Met 방식의 에
#include <iostream.h>
void swap(int x, int y);

int main()
{

CONBDU FWD =
×… er ㅁㅁ ㅁㅁ 00 000


===== PAGE 266 =====
264 ee 제2주

9:   int x =5, > = 10;

10:

11%   cout << "Main. Before swap, x: "<< x << "y: "<< y << "An";
12:   swap(x,y);

13:   cout << "Main. After swap, x: " << x\<< " ys " << y << "Nn";
14:   return 0;

15: 3

16:

17: void swap(int x, int y)

18: £

19: int temp;

20:

21: cout << "Swap. Before swap, x: "<< x << "y: "<< y << "\n";
22:

23: temp = x;

24: x=y;

25: y = temp;

26:

27: cout << "Swap. After swap, x: "<< x << "ys "<< y << "An";
28:

29: }

a 1h Main. Before swap. x: 5 y: 10
Swap. Before swap. x: 5 y: 10
Swap. After swap. x: 10 y: 5

Main. After swap. x: 5 y: 10

분석  이 프로그램은 두 개의 WSS main») 초기화하고 50800로 그 변수를
^” 전달하며, 두 개의 값은 바꾸는 것처럼 보입니다. 그러나 0000에서 다시
보아졌을 때 그들은 바뀌지 않았습니다.

여기서 문제는 x, 》가 WOE swap) 함수에 전달되었다는 것입니다. 이는
인 복사가 함수에서 만들어졌다는 것입니다. 여러분이 원하는 것은 x 》를
로 전달하는 것입니다.

이 BALE 푸는 방법은 0++에서 두 가지가 있습니다. 54000에의 매개 변수를 포
하는 방식이 하나요, 나머지는 참조자로 원래의 ae 전달하는 것입니다.

6\80()를 포    ane pile   만들어 때
가지고  연산을 ye 수 mead swap() a7 Coe 사용하여 실제값

l= 값
2.
=

을
변화


===== PAGE 267 =====
제9일 HAA ee 265

시키려면 90000는 두 개의 포인터형을 매개 변수로 가질 수 있도록 선언되어야
합니다. 포인터를 사용함으로써 *와 》의 Qe 실제로 wy 것입니다. [리스트 96]
이 이를 보여줍니다.

[리스트 9.6] 포인터를 of Sot 전달 방식

: // [리스트 9.6] 포인터를 이용한 전달 방식

: #include <iostream.h>

: int main()

e {

OF   int x

105

1

2

3

4:

5: void swap(int *x, int* y);
6:

/

8

=5,y = 10;

11: cout << "Main. Before swap, x: "<< x << "y: "<< y << Nhs
12: swap(&x,&y);

13: cout << "Main. After swap, x: "<< x << "y:" << y << Nn
14: return 0;

153 개
16%

17: void swap(int *px, int *py)

188 1

19:   int temp;

20:

21: cout << "Swap. Before swap, *px: " << *px <<" *xpy: " << xpy << "\n";

22:

25%    temp = *px;
24: *px = *py;
252   *py = temp;

265

CAGE   cout << "Swap. After swap, *px: " << *px <<" kpy: " << xpy << "\n";

28:
293. F

결과 Main.

Swap.
Swap.
Main.

성공입니다. 5번 줄에서 50800의 원형이 바뀌었습니다. 매개 변수로 두 개
의 값 대신 두 개의 포인터를 받도록 고쳐진 것입니다. 12번 줄에서 90800

|

(aa

Before swap. x: 5 y: 10
Before swap. *px: 5 *py: 10
After swap. *px: 10 *py: 5
After swap. x: 10 y: 5

이 호출되었을 때 xo} yo] 주소가 인수로 전달되었습니다.


===== PAGE 268 =====
266 ee 제2주

19번 줄에서 지역 변수 temp7} 5800함수 안에서 선언되었습니다. temps 포인터
일 필요가 없습니다. *%04(호출 함수에서 3) RS 해당 함수가 살아있는 동안 가질
것입니다. 함수가 반환되면 1600는 더 이상 불필요합니다.

23번 줄에서 temp 의 값으로 치환되고 24번 줄에서 px] Re 로 대입됩니
다. 25번 줄에서 tempol] 저장된 값은(원래의 에 있던 값) 05에 저장됩니다.
여기서 실제의 효과는 호출 함수의 값이 실제 바뀌다는 것인데 이는 swap) 함수
에 포인터로 전달되기 때문입니다.

Oo} HO swaps 참조자를 써서 구현

앞선 프로그램은 SAS 하지만 swap) 함수의 구성이 두 가지 부분에 있어 따분
하기 그지없습니다. 첫째는 swap) 함수에서 포인터를 소환하는 것은 오류가 발생
하기 쉽고 읽기도 쉽지 않습니다. 둘째, 호출 함수에서 변수의 주소를 전달하는
것은 swap) 함수의 내부 과정을 너무나도 뻔하게 만듭니다.

0++의 목적 중 하나는 사용자로 하여금 함수가 어떻게 돌아가는지 걱정 안하게
하는 것입니다. 포인터를 전달하는 것은 사실 호출된 프로그램보다 호출한 프로
그램에게 부담이 됩니다. [리스트 9.7]은 swap) 함수를 참조자를 써서 사용하였습

니다

[리스트 9.7] 참조자를 써서 다시 쓴 90800) 함수

1: // [리스트 9.73 참조자를 써서 다시 쓴 swap 함수

28 //

a

4: #include <iostream.h>

5:

6: void swap(int &x, int &y);

(2

8: int main()

99 4

10%   int x = 5, y = 10;

113

123   cout << "Main. Before swap, x: "<< x << "y: "<< y << "An";
13:   swap(x,y);

14:   cout << "Main. After swap, x: "<< x << "yi "<< y << "\n";
152   return 0;

16% +

V0:

18: void swap(int &rx, int &ry)

=
xo

“al



===== PAGE 269 =====
}

제9

Ted
>t

ㅁ
녀

자 ee 267

20: int temp;

21;                                              :

22: cout << "Swap. Before swap, rx: " << rx << "ry: " << ry << "\n";
25%

24: temp = rx;

Zo: TX = ry;

26: ry = temp;

er:

28: cout << "Swap. After Swap, rx: " << rx << "ry: " << ry << "\n";

30: }

결과 Main. Before swap. x: 5 y: 10

Swap. Before swap. rx: 5 ry: 10
Swap. After swap. rx: 10 ry: 5
Main. After swap. x: 10 y: 5

IA SS 써서 만든 프로그램에서와 같이 10번 줄에서 두 개의 변수가 A

언되었고 그 값이 128 줄에서 출력되었습니다. 13번 줄에서 함수 0020가

호출되었는데 그런데 여기서는 ×, 》의 Bo] - 주소가 아니라 - 전달되었습니다.
호출하는 함수는 단순히 값만 전달하였습니다

코

swap)7} 호출되었을 때 함수의 실행은 18번 줄로 건너뛰고 여기서 변
자로 식별되었습니다. 그 값이 22번 줄에서 출력이 되었는데 특별한 연
요가 없었습니다. 원래 값의 다른 이름이고 그대로 쓰이면 되었습니다.
24 - 26번 줄에서 AS] 바뀌었고 28번 줄에서 출력이 되었습니다. menage
ao SS PTE 돌아오고 14번 줄에서 값들이 다시 출력되었습니다. swap) 함
수에 대한 매개 변수가 참조자로 선언되었기 때문에 0800의 값들은 참조자로
전달되었고 따라서 0000에서의 값들도 바뀌었습니다. 참조자는 포인터를 사용할
때의 강력함과 함께 일반 변수를 사용할 때의 간편성과 편리성을 제공합니다.

4         pC it B, wt 2 )
수 표제(『40에101 Header)Q}  …   win AS
수 H%G(Prototype)oll 대한 이해

wu
|»
10
No)

.이은 포인터를 사용한 swap) PES 보여주었고 [리스트 OTL 참조
를 사용한 예를 보여주었습니다. 참조자를 사용한 함수가 사용하기 훨씬 쉬웠고
읽기가 쉽습니다. 그런데 어떻게 호출하는 PEE 값이 참조자로 전달되었는

자

지


===== PAGE 270 =====
268 ee 제2주

함수로 전달되었는지 알 수 있습니까? 사용자 여러분은 사용자로서 swap) 함수
가 매개 변수들을 바꾼다고 전제를 해야 합니다.

여기에서의 예는 함수 원형의 또 다른 사용법을 보여주었습니다. 함수 원형에서
선언된 매개 변수를 보면, 다른 함수 원형에서와 마찬가지로 함수 표제 부분에
있는데, 프로그래머는 swap) 함수에 참조자를 통한 전달 WIS 썼다는 것을 알
수 있습니다. 따라서 값은 vee.

만일, swap) 함수가 SAAS) 멤버 함수였다면 클래스 선언에서 이러한 정보를
전해야 합니다.

0++에서 함수와 클래스의 사용자들은 원하는 AS 함수의 표제 부분을 보고 알
아야 합니다. 마치 클래스와 함수에 인터페이스처럼 작용합니다. 실제 구현은 사
용자에게는 숨겨져 있습니다. 따라서 프로그래머는 문제점에 직접 몰두할 수 있

게 하고 함수 내부에서 어떻게 돌아가는지 걱정할 필요가 없게 만듭니다.

:코로닐 존 로블링`이라는 사람이 브루크린이라는 다리를 만들었을 때 그는 많은
걱정을 하였습니다. 콘크리트가 어떻게 부어지는지, 그 다리의 전선줄이 어떻게
만들어지는지 등입니다. 그는 이 다리를 만드는 모든 물리적, 화학적 공정에 참여
하였습니다. 하지만 오늘날은 기술자들은 다른 부분들이 어떻게 만들어졌는지 걱
정할 필요 없이 각 부분들의 기능을 잘 이해한 상태에서 자기 부분에 좀더 신경
을 쓸 수 있게 되었습니다.

0++의 목적은 프로그래머들이 잘 만들어진 클래스와 함수들에 대해 그 내부 구

조는 모르는 채 잘 쓸 수 있게 하는 것입니다. 이 각 부분들은 전체 프로그램을

만들기 위해 조립만 되면 되는 것입니다. 마치 건물과 다리를 만들 때 재료들을

가져다 조립만 하면 되듯이 말입니다.

똑같은 방식으로 기술자는 파이프의 하중, 용량, 크기 등을 결정할 때 사양서만
보면 됩니다. 똑같은 방식으로 프로그래머는 클래스나 a3 인터페이스 부분만

보고 어떤 서비스를 하는지 어떤 매개 변수를 갖는지 반환 값이 무엇인지를 알게

됩니다.

여러 개의 값을 반환하는 법
앞서 말했듯이 함수는 한 개의 값만을 반환합니다. 두 개의 We 반환하고 싶을
때는 어떻게 합니까? 이 문제를 해결하는 한 가지 방법은 두 개의 객체를 참조자
로 함수에 전달하는 방법입니다. 함수는 그 객체를 원하는 값으로 채울 수 있


===== PAGE 271 =====
제9일 HAA ee 269

니다. 참조자 전달 방식은 함수로 하여금 그 값을 변화시킬 수 있기 때문에, ㅇ
방법은 실질적으로 함수로 하여금 두 개의 값을 반환하게 하여줍니다. 이러한
식은 함수가 원래 retum 예약어를 통해 반환하는 값을 다른 목적 - 오류코드를
반환하게 하는 등 - 에 쓸 수 있습니다.

~

뚜

다시 한번 말하지만 이는 참조자를 사용할 수도, 포                     !
[리스트 9.8]은 세 개의 값을, 두 개는 매개 변수를 통해 하나는 함수의 반환값을
통해 반환하는 예제입니다.

[리스트 9.8] SUAS 값을 반환하는 al

1: // [리스트 9.8] 포인터로 BS 반환하는 예

2: 7/

3:

4: #include <iostream.h>

508

6: typedef unsigned short USHORT;

(3

8: short Factor (USHORT, USHORT*, USHORT*) ;
9:

10: int main()

11: 4

12   USHORT number, squared, cubed;

Wie   short error;

14:

155    cout << "Enter a number (0 - 20): ";
16=   cin >> number;

Avs

18:   error = Factor(number, &squared, &cubed) ;
19:

20:   if Clerror)

215   {

22:      cout << "number: " << number << "\n";
25%      cout << "square: " << squared << "\n";
24:      cout << "cubed: " << cubed << "\n";
25:   I

26:   else

27:   cout << "Error encountered! !\n";

28: return 0;

29: }

30:

31: short Factor (USHORT n, USHORT *pSquared, USHORT *pCubed)
See 1

33: short Value = 0;

34:   TF Ca 5°20)


===== PAGE 272 =====
270 ee 제2주

35%      Value = 1;

56:   else

St?   {

38:       *pSquared = n*n;
59       *pCubed = n*n*n;
40:       Value = 0;

41%   Bs

4e:   return Value;

43: 가

결과 Enter a number (0-20): 3
:          3

number:
square: 9
cubed: 27

ra

섹  12번 줄에서 number, squared, cubed= USHORTS 선언되었습니다. number=
사용자가 입력하는 값으로 대입됩니다. 이 numberS} squaredm cubed2] 주소
가 함수 880000에 전달이 됩니다.

“nce 값으로 전달된 A 번째 ee 변수를 살펴봅시다. 이 함수가 다룰 수 있
는 최대값 20(이 함수가 다룰 수 있는 가장 큰 값)보다 크면 오류 RS Valued

저장하여 반환합니다. Factor()2] 반환값은 이러한 오류 값 혹은 모든 일이 잘되었

THE 0의 BS 가지고 있다가 42번 줄에서 반환합니다.

7000086에 대한 제곱과 세제곱 값이 반환값 전달 방식이 아니라 Go] 전달된 포

인터 값을 변화시켜 반환됩니다.

38번과 39번 줄에서 포인터는 그들의 반환값으로 대입됩니다. 39번 줄에서 반환

값 8106는 성공 값을 할당받습니다. 41번 줄에서 반환값 Value7} 반환됩니다.

한 단계 발전시키면 다음과 같습니다.

enum ERROR_VALUE { SUCCESS, FAILURE } ;

이

(el

로그램

thlo

이렇게 하면 0 HE 12 반환하는 대신 BBA SUCCESS1 FAILURES 반환
할 것입니다.

참조자를 사용한 값 반환
[리스트 9.8]은 잘 돌아가긴 하는데 포인터 대신 참조자를 쓰면 읽기도 쉽고 유지
보수도 쉽습니다. [리스트 OE 포인터 대신 참조 자를 쓰고 또 ERROR 나열형을
썼습니다.



===== PAGE 273 =====
제9일 BAM ee 271

[리스트 9.9] 참조자를 써서 다시 작성한 [리스트 9.8]

00 기 에 내 FWP =

2

10:
11:
128:
13:
14:
158
16:
1?
18:
19:
20:
21:
22:
235%
24:
(ae)
26:
27:
283
29:
30:
$15
52:
33:
545
55:
56:
ST:
38:
$9?
40:
41%
42:
43:

ai
// [예제 9.91 참조자를 써서 다시 작성한 [리스트 9.87
//

#include <iostream.h>

typedef unsigned short USHORT;
enum ERR_ CODE { SUCCESS, ERROR [가

ERR_CODE Factor (USHORT, USHORT&, USHORT&) ;
int main)
{

USHORT number, squared, cubed;

ERR_CODE result;

cout << "Enter a number (0 - 20): ";
cin >> number;

result = Factor(number, squared, cubed) ;

if (result == SUCCESS)

£
cout << "number: " << number << "\n";
cout << "square: " << squared << "\n";
cout << "cubed: " << cubed << "\n";
가
else
cout << "Error encountered! !\n";
return 0;
3               /왜001 1
ERR_CODE Factor (USHORT &rSquared, USHORT &rCubed)
{
if (n > 20)
return ERROR; // simple error code
else
{
rSquared = nn;
rCubed = n*n*n;
return SUCCESS ;
}
}



===== PAGE 274 =====
272 ce Woe

Enter a number (0-20): 3
number: 3
square: 9
cubed: 27

us
1 -

[리스트 9.이는 [리스트 9.8]과 두 가지만 제외하고 같습니다. ERR-CODE 나
열형은 36과 41번 줄의 오류 보고 및 22번 줄의 오류 처리를 좀더 명확하
게 합니다.

종더 큰 변화는 828000가 squared9} 00660에 대한 포인터가 아니라 참조자를 사

용했다는 것입니다. 이렇게 하는 것이 매개 변수를 다루기 쉽고 이해하기 쉽게
합니다.

(faa
ee

Sy 2-y(Efficiency) 위해 참조자를 전달하자

매번 함수에 객체를 Boe 전달할 때마다 그 객체에 대한 복사가 일어납니다.
매번 함수로부터 객체를 값으로 하여 반환할 때마다 또 복사가 일어납니다.

5일째의 심화학습에서 이 객체들이 스택에 복사됨을 배웠습니다. 이렇게 하면 시
간과 메모리가 소요됩니다. 내장된 정수형 같은 객체를 쓸 때 이러한 과정은 별
일이 아닐 수 있습니다.

그러나 큰 객체의 경우는 대가가 FUG. 사용자가 스택 위에 만든 객체는 각 멤
버 변수들의 총합입니다. 이 객체들 또한 사용자가 정의한 것일 수 있고 이 큰
구조물을 스택에 복사하는 일은 성능과 메모리 사용에 매우 큰 대가를 지불할 수
있습니다.

또 oe  대가가 있습니다. 여러분이 만든 클래스와 함께, 컴파일러가 특정 생성자

출할 때마다 각각에 대한 임시복사가 - 복사 생성자 - 만들어집니다. 오늘
seh 어떻게 복사 생성자가 동작하는지, 어떻게 여러분 자신의 것을 만드는
지를 배우게 될 것입니다. 그러나 지금 당장은 객체의 특정 생성자가 이 스택에
저장될 때마다 복사 생성자가 불리운다는 것만 아는 것으로도 충분할 것으로 생
각합니다.

임시 객체가 없어지면 - 함수가 반환될 때 일어납니다. - 객체의 소멸자가 호출됩
니다. 객체가 함수에서 값으로 부 나서 그 객체에 대한 복사본이 역시 만들어지
고 소멸됩니다.

큰 프로그램에서 이 생성자와 소   fasted SSS FEM 메모리 사용에 있어 크나
큰 Boo] 수 있습니다. 이 개념을 보여주기 위해 [리스트 9.10은 SimpleCato] e}



===== PAGE 275 =====
4 rir

객체를 만들었습니다. 실제 객체는 더 크고 더 복잡할
기만으로도 얼마나 자주 생성자와 소멸자가 호출되는지 보

[리스트 9.10]}2 SimpleCat-& ee 두 개의 함수를 호출합니다. A 번째 함수
coy

CaS 값으로 받고 또 값으로 반환합니다. 두 번째 함수는
받고 그 객체의 포인터를 반환합니다.

[리스트 9.10] 참조자에 의한 AA 전달

// [리스트 9.91 참조자를 써서 다시 작성한 [리스트 9.83
//

#include <iostream.h>

class SimpleCat

£

public:

9:    SimpleCat ();

10:   SimpleCat(SimpleCat&) ;
11:   “SimpleCat();

123 5

CONOU FWD =

an
14: SimpleCat::SimpleCatQ
15: ¢        |
16:   cout << "Simple Cat Constructor...\n";

19: SimpleCat::SimpleCat (SimpleCat
20: {                         |

21:   cout << "Simple Cat Copy Constructor...\n";

22: )
24: SimpleCat::~SimpleCat()

25° <
26:   cout << "Simple Cat Destructor...\n";

29: SimpleCat FunctionOne (SimpleCat theCat);
30: SimpleCat* FunctionTwo (SimpleCat *theCat);

32: int main()

55: £
545   cout << "Making a cat...\n";
35    1        Frisky;

36: cout << "Callihg FunctionOne...\n";


===== PAGE 276 =====
274 ㅎㅇ 제주

St?   Funct ionOne(Frisky) ;

38:   cout << "Calling FunctionTwo...\n";

39:   FunctionTwo(&Frisky);

40:   return 0;

41: +

42:

43: // FunctionOne, 값 전달          ae
44: SimpleCat Funct ionOne(SimpleCat, ‘thecatp
45: {                               ’

46:   cout << "Function One. Returning...\n";
47:   return theCat;

48: }

49:

50: // functionTwo, #27} 전달

51: SimpleCat* FunctionTwo (SimpleCat *theCat)

52: £

53:   cout << "Function Two. Returning...\n";

54:   return theCat;

552}             “Sie                                          =

: Making a cat...

Simple Cat Constructor...
Calling FunctionOne...

Simple Cat Copy Constructor...
: Function One. Returning...

: Simple Cat Copy Constructor...
: Simple Cat Destructor...

: Simple Cat Destructor...

: Calling FunctionTwo...

10: Function Two. Returning...
11: Simple Cat Destructor...

EASE 원래 SH] 안되는 것이지만 Agel 좋게 el 위해 불였습니다:

CONAOU FWD

\o

6 - 128] 줄에서 아주 간단한 SimpleCat 클래스가 선언되었습니다. 생성자
와 소멸자, 복사 생성자는 모두 자기가 호출되었음을 알리는 문

합니다.

34번 줄에서 main)o] 문장을 출력하고 출

에서 9000160&의 객체가 선언되었습니다. 이는 또 생성자가 호출    합니다. 그
표시가 출력 2번 줄에 되었습니다.


===== PAGE 277 =====
제9일 BAA ee 275

36번 줄에서 270100은 FunctionOnes 호출함을 보여줬고 이는 출력 3번 So] 나타
습니다. 800084000060은 910201608의 객체를 값 전달 방식으로 호출하였기 때문
에 5000160#의 객체가 호출된 함수에서 지역 변수로 되어 스택에 저장되었습니
- 다. 이때 복사 생성자가 호출되고 이는 4번 출력 줄에 나타납니다.
로그램은 호출된 함수에서 46번 줄로 가고 출력 5번 줄에 문장을 출력합니다.
리고 반환되고 SimpleCat 객체가 값으로 반환됩니다. 이는 또 다른 객체의 복사
만들고 복사 생성자를 호출하는데 이는 oF 출력 So] 나타납니다.

함수 80000000060으로부터의 반환값은 어떤 객체에도 저장되지 않고, 따라서 임
시로 만들어졌던 반환값은 소멸자를 호출하면서 버려집니다. 이는 7번 출력 줄에
서 나타납니다. 80200000060이 끝났기 때문에 지역 복사본이 범위를 벗어나고 «A
멸되며 그 소멸자가 출력한 문장이 8번 So] 나타납니다.

프로그램은 7800으로 되돌아오고 FunctionTwo)7} 호출됩니다. 그런데 여기서는
매개 변수가 참조자 전달 방식으로 전달되었습니다. 아무런 복사본도 일어나지
않았고 따라서 출력도 되지 않았습니다. 80000001\00는 문장을 10번 출력 줄에
출력시켰고 그리고 SHES SimpleCat 객체를 반환하였습니다. 다시 참조자로 반환
하였는데 따라서 생성자나 소멸자가 호출되지 않았습니다.

마지막으로 프로그램이 끝나고 82096는 YAS 벗어나게 되며 마지막으로 소멸자
가 호출됩니다. 이는 출력 11번 So] 표시되었습니다.

: 이 프로그램의 실제 효과는 80000000060의 호출입니다. SimpleCatS 값으로 전달
하기 때문에 각각 두 개의 복사 생성자와 소멸자를 호출하였습니다. 하지만
10000001\00)는 아무 것도 호출하지 않습니다.

[KI

re 나

2. =
2 Le

상수 ZPlEl(const Pointer) 전달하기
10000001\00에 포인터를 전달하는 것이 좀더 효율적이긴 하지만 다소 위험합니
다. FunctionTwo()= SimpleCat- 바꾸지 못하게 되어 있습니다. 그럼에도 그 주소
를 전달합니다. 이는 그 객체의 값이 w@ 소지가 있고, WS 전달하는 방식에서

그 점이 뒤집니다.

값 전달 YAS 박물관에 여러분 소유의 명화 대신 그 명화의 복사본을 게재하는
것과 똑같습니다. 누군가 손상을 시켜도 원본에 손상은 없습니다. 참조자 전달 방
식은 명화가 있는 여러분 집의 주소를 박물관 게시판에 보내는 것과 같고 그러면
구경꾼들이 여러분 집 주소를 보고 들이닥쳐 명화 원본을 감상하다 손상을 입힐
것입니다.


===== PAGE 278 =====
276 ee 제2주

[리스트 9.11] 상수형 포인터 전달

600 기 내 FWD

94

108
rs
12:
13
14:
Vo
16:
le
18:
19%
20:
ale
22°
23%
24:
25%
26%
2%
28:
29%
50:
31%
S22
$5:
34:
53!
565

// (ASE 9.111 상수령 포인터 전달
Lf

#include <iostream.h>

class SimpleCat

{

public:
SimpleCatQ;
SimpleCat(SimpleCat&);
“SimpleCatQ);

int GetAge() const { return itsAge; }
void SetAge(int age) { itsAge = age; }

private:
int itsAge;
3;

SimpleCat::SimpleCat()

€
cout << "Simple Cat Constructor...\n";
itsAge = 1;

SimpleCat::SimpleCat(SimpleCat&)
{

cout << "Simple Cat Copy Constructor...\n";

SimpleCat::~SimpleCat(
t

cout << "Simple Cat Destructor...\n";
}

const SimpleCat * const FunctionTwo (const SimpleCat * const

theCat);

Sf:
358:

int main()



===== PAGE 279 =====
제9일 BAA ee 277

392 <

40:   cout << "Making a cat...\n";
41:   SimpleCat Frisky;

42s   cout << "Frisky is ";

43:   cout << Frisky.GetAge();

44:   cout <<" years old\n";

453    int age = 5;

46:   Frisky.SetAge(age) ;

47:    cout << "Frisky is ";

48:   cout << Frisky.GetAge();

49:   cout <<" years old\n";

50:   cout << "Calling FunctionTwo...\n";
511   FunctionTwo(&Frisky) ;

525    cout << "Frisky is ";

535   cout << Frisky.GetAge();

54:   cout <<" years old\n";

55°   return 0;

562 3

578

58: // functionTwo, const 포인터 전달
59: const SimpleCat * const FunctionTwo (const SimpleCat * const

theCat)

60: +

612   cout << "Function Two. Returning...\n";

62:   cout << "Frisky is now " << theCat->GetAge();
63:   cout <<" years old \n";

64:   // theCat->SetAge(8); const!

652   return theCat;

66: }

(naa
iz

Making a Cat...

Simple Cat constructor...
Frisky is 1 years old
Frisky is 5 years old
Calling FunctionTwo
FunctionTwo. Returning...
Frisky is now 5 years old
Frisky is 5 years old
Simple Cat Destructor...

SimpleCat= 두 개의 접근자 함수를 가졌는데 134 SS] GetAgeQe 상수
함수이고, 14번 SS] SetAgeQ=E 일반 함수입니다. 17번 줄에서 16486라는

멤버 변수를 추가시켰습니다.


===== PAGE 280 =====
278 ㅎㅇ Hz

생성자와 복사 생성자, 소멸자가 그들의 EAS 출력하게끔 정의되었습니다. 복사
생성자는 호출되지 않았는데 왜냐하면 객체는 참조자 형태로 전달되었고 따라서
복사본은 만들어지지 않습니다. 41번 줄에서 객체가 만들어지고 그 기본 나이 값
이 42번 줄에서 출력됩니다.

46번 줄에서 접근자 SetAgeS 사용하여 15486가 설정되었고 그 결과가 47번 Sol
서 출력되었습니다. FunctionOne? 이 _ 프로그램에서 «ARR EZ] 않았지만
10000001\0()는 호출되었습니다. 80000001\00는 약간 변화되었습니다. 36번 Fol
서 매개 변수와 반환값이 선언되었는데 상수형 객체에 상수형 포인터를 가지고
또 싱수영 “aaah 상수형 반환값을 반환합니다.

매개 변수와 반환값 모두 참조자로 전달되었으므로 아무런 복사본이 만들어지지
않으며 또 복사 생성자도 호출되지 않습니다. 8000100100의 포인터는 상수형이
고 따라서 비상수형 메쏘드 9064800를 SSH 수 없습니다. 만일 64번 줄에서
966&860가 주석문으로 막히지 않았다면 컴파일되지 않았을 것입니다.

main] 생성된 객체는 상수가 아님을 주목합시다. 그리고 『096(는 56860
를 호출할 수 있습니다. 이 비상수형 객체의 주소가 FunctionTwoNZ 전달되었으
나 FunctionTwo()2] 선언이 le 터를 3  상수형 객체에 대한 포인터로 선언하였으므
로 객체는 상수형처럼 취급됩니다.

그 대안으로써 참조자를 쓰자

[리스트 9.11은 추가 복사본을 만드는 문제를 해결하였습니다. 따라서 호출될 때
복사 생성자와 AVS 스택에 저장하는 과정을 생략하였습니다. 상수형 포인터
를 상수형 객체에 사용하였고 따라서        를 수정하는 것을 방지하였습니
다. 그러나 아직 뭔가 부족합니다. Gee 전달된 객체가 포인터이기 AEG.
객체는 널이 될 수가 없음을 여러분은 알기 a 함수 안에서 포인터보다는 참

조자가 전달되게 하는 것이 쉽습니다. [리스트 9.121가 이 예를 보역품니다

[리스트 9.12] 랙체에 BAT 전달하기

‘    Ol"

// [리스트 9.121 객체에 참조자 전달하기
//

#include <iostream.h>
class SimpleCat

{
public:

CONDOUFWYDY =



===== PAGE 281 =====
제9일 AAT ee 279

9

10:
11:
12:
13:
1:4
(5s
16:
178
18:
19:
20:
21:
22:
23:
24:
Dols
26:
27%
28:
29:
30:
318
52:
55:
34:
35:
36:
Sf:
58:
39:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
503
51's
52°
5%
54:
DD?

SimpleCat();
SimpleCat(SimpleCat&) ;
“SimpleCat();

at

int GetAge()/const   | urn itsAge; }
void SetAge(    age) { itsAge = age; }
private:

int itsAge;
a:

SimpleCat::SimpleCat()

{
cout << "Simple Cat Constructor...\n";
itsAge = 1;

}

SimpleCat::SimpleCat(SimpleCat&)
{

cout << "Simple Cat Copy Constructor...\n";
3

SimpleCat::~SimpleCat()
{

cout << "Simple Cat Destructor...\n";
}

const SimpleCat & FunctionTwo (const SimpleCat & theCat);

int main()
{
cout << "Making a cat...\n";
SimpleCat Frisky;
cout << "Frisky is " << Frisky.GetAge() <<" years old\n";
int age = 5;
Frisky.SetAge(age) ;
cout << "Frisky is " << Frisky.GetAge() << " years old\n";
cout << "Calling FunctionTwo...\n";
FunctionTwo(Frisky);
cout << "Frisky is " << Frisky.GetAge() << years old\n";
return 0;
J

// functionTwo, const 객체에 대한 참조작 전달
const SimpleCat & FunctionTwo (const SimpleCat & theCat)
{

cout << "Function Two. Returning...\n";


===== PAGE 282 =====
280 ce 제2주

56:   cout << "Frisky is now " << theCat.GetAge(;
ae   cout <<" years old \n";

58:   // theCat.SetAge(8); const!

59:   return theCat;

60: }

24 I Making a Cat...

Simple Cat construcor..
Frisky is 1 years old
Frisky is 5 years old
Calling FunctionTwo
FunctionTwo. Returning...
Frisky is now 5 years old
Frisky is 5 years old
Simple Cat Destructor...

불샐 2oHe [리스트 9.111에 나타난 것과 같습니다. 단 하나의 중요한 변
될    se eae 상수 객체에 대한 참조자를 취하고 | 반환한다는 A
말하지만 참조자를 가지고 작업을 하는 것은 포인터보다 간단하고

대되고 상수형을 쓰는 것과 같은 안전성이 있다는 것입니다.

tf
-
또

ae
의
fol
tio
ot
rlo
be

>
ie

XKconst Reference) C++ 종종 ‘SimpleCat™] 대한 #73 BAP
SimpleCat] 대한 HAAS   veel

er] 할당할 수 없기 때문에 Att
잠   [에 적용되었 다면 이는 객체가 상수형  형을 참조하라는 oar

1   근 ㅁ

ofo
오

Jz Je

=

wu o% (인
>
of!

Pall
주
bi
a

언제 잠조자를 쓰고 언제 포인터를 쓰나?

C++ 사용자들은 포인터보다 참조자를 훨씬 선호합니다. 참조자가 말끔하고 사용
하기 쉬우며 정보 은닉000008000 801008)이라는 좋은 기능을 수행하는데 이미
위에서 살펴보았습니다.

하지만 참조자는 다시 할당되지 않습니다. 만일 여러분이 ※      어

인트하고 다음엔 다른 객체를 포인터할 때에는 kguae EVES 써야 합니다.
참조자는 널이 될      eg! 따라서 찬조자가 널로 채워     할 경우엔 여러분은
나중의 예가 new 연산자입니다. 만일, new7} 자유 기억

수 없으면 널을 반환합니다. 참조자는 널로 될 수가 없기 때문에 메



===== PAGE 283 =====
SATO! SUAS 섞어서

해 참조자를 초기화하려면 그 메모리가 널이 아닌지를 먼저 검사해야 합니다. 다
음의 예가 이를 다루는 예를 보여줍니다.
int *pInt = new int ;

if ( pInt ! = NULL )
int &rInt = *pInt ;

여기에서는 정수형 포인트6000가 생성되고 00에 의해 만들어진 메모리로 a7
화됩니다. pinto] 주소가 검사되고 Wo] 아니면 pln 소환됩니다. 정수형 변수를
소환하는 결과는 정수형 객체가 VISE 것이고 7띠는 그 객체로 초기화되도록
됩니다. 이때 마는 new 연산자에 의해 반환된 정수형의 다른 이름이 됩니다.

~

|

DO 가능하면 매개 변수를 참조자로 전달합시다.
00 가능하면 참조자를 반환합시다
DONT 지역 객체에 참조자를 반환하지 맘시다

<i

(저기
la

같은 함수에서 매개 변수에 포인터와 참조자 및 값 전달 방식을 섞어 쓰는 것은
들린 것이 아닙니다. 한번 봅시다.

rum

CAT * SomeFunction ( Person & theOwner , House *theHouse, int age ) ;

이 선언은 SomeFunction®] 세계의 변수를 가진다는 AS 보여줍니다. 처음
Person 객체를 참조하는 것이고, 두 번째는 10056를 포인트하는 것이고 세 번째

정수형을 전달합니다. CATO 대한 포인터를 반환합니다.

변수들을 선언할 때 어디에 BANOS 위치시킬 것인가 Se 어디에 간접 지정 연
산자(*)를 위치시킬 것인가가 상당한 문제입니다. 다음 중 아무거나 써도 됩니다.
T: CATS rFrisky :

2: CAT & rerisky ;
53) CAT -Srkrisky >


===== PAGE 284 =====
282 ee 제2주

el 주장은 Sat 같슴니다. rFriskye 그 °° Frisky?
객체에 대한 AA 그 형으로 생각될 수 있습 5. 이

것이 1 Ge sis) Mise sim 선언자의 일부

CAT& rFrisky;
CAT boots ;

마지막으로 많은 프로그래머들이 논쟁에 말리길 싫어하여 중간 위치를 선택합니다. 즉

ㅣ
2번의 sh 깥이 6를 Sie] Se 이 |
접

범위 벅어나 2410] 대한 참조자를 반환하면 안됩니다

일단 C+ 프로그래머가 참조자 전달 방식을 익히면 마구 남용하는 경향이 있습
니다. 물론 지나쳐도 상고 es 없습니다. 하지만 참조자는 항상 특정 객체에 대한
다른 이름임을 잊어서는 안됩니다. 참조자를 함수에 또는 함수로부터 전달할 때



===== PAGE 285 =====
제9일 HAA ee 283

=

=

항상 다음과 같은 질문을 해야 합니다. '내가 쓰는

[리스트 9.13]은 더 이상 존재하지

보여줍니다.

객체에 대한 4

[리스트 9.13] 존재하지 않는 랙체에 대한 참조자 반환

참조자는 무엇을 가리키는

1: //

2: // [리스트 9.137 존재하지 않는 객체에 대한 참
S57

4:

5: #include <iostream.h>

6:

7: class SimpleCat

8s 고

9: public:

10:   SimpleCat (int age, int weight);

112   “SimpleCat() {}

12:   int GetAge() { return itsAge; }

13:   int GetWeight() { return itsWeight; }
14: private:

15   int itsAge;

16:   int itsWeight;

Tes 33

18:

19: SimpleCat::SimpleCat(int age, int weight):
20: itsAge(age), itsWeight(weight) {}

21:

22: SimpleCat &TheFunction();

23:

24: int main()

2561

26:   SimpleCat &rCat = TheFunction();

27%   int age = rCat.GetAge();

28:   cout << "rCat is " << age <<" years old! 나"
29:   return 0;

308 }

51:

32: SimpleCat &TheFunction()

3538

34: SimpleCat Frisky(5,9);

35: return Frisky;

36: 》            “SS  비했는 으으 7



===== PAGE 286 =====
284 ee 24

겔과  Compile error: Attempting to return a reference to a local object!

이 프로그램은 수랭되지 않습니다.

분석  7 - 17번 줄까지에서 SimpleCato] 선언되었습니다. 26번 줄에서 9000160#에
~    대한 참조자가 TheFunction)S 호출한 결과로 초기화되었는데 이는 22번 줄
에서 SimpleCato]] 대한 참조자를 반환하게 되어 있습니다.

TheFunction()2] 몸체는 91001608형의 지역객체를 선언하였고 그 886와 weightS
초기화하였습니다. 그리고 지역 Ads 참조자로 전달하였습니다. 좋은 컴파일러
라면 이 오류를 잡아낼 것이고 그렇지 못한 경우는 실패하여 알 수 없는 결과를
낼 것입니다.
함수 '1600008000이 반환되면 지역객체 Frisky= 없어질 것입니다. 이 함수로 인
해 반환되는 참조자는 존재하지 않는 객체에 대한 다른 이름이 될 것이고 이는

안 좋은 일입니다.

힙에 있는 랙체에 대한 참조자 반판하기

여러분은 [리스트 9.13]의 문제를 푸는데 있어 0@00008000이 Frisky 힙에 만들
면 될 것 같은 기분을 가질 것입니다. 11680008000으로부터 반환될 때 『096는

|속 존재할 것입니다. 이러한 접근 방식의 문제점은 다음과 같습니다. 8094에
할당된 메모리를 가지고 작업을 마친 뒤 어떤 일이 발생되는가? [리스트 9.1417}
ㅣ 문제의 예를 보여줍니다.

고

=
ㄴㄴ

[ej

[리스트 9.14) 메모리 누출 발생

// [리스트 9.147 메모리 누출 발생
//
#include <iostream.h>

1

2

3

4

5: class SimpleCat

6: ¢€

7: public:

8    SimpleCat (int age, int weight);
9    “SimpleCat() {}

1     int GetAge() { return itsAge; }
1

Q:
V3   int GetWeight() { return itsWeight; }


===== PAGE 287 =====
제9일 BAN ee 285

12:
13:
14:
15%
16:
Ve
182
19;
20:
ete
22:
23%
24:
255
26:
20:
28:
29:
30:
315
52:
55°
34:
So
36:
S73
58:
59:
40:
41:

private:
int itsAge;
int itsWeight;
3;

SimpleCat::SimpleCat(int age, int weight):
itsAge(age), itsWeight(weight) {}

SimpleCat & TheFunction();

int main()
{
SimpleCat & rCat = TheFunction();
int age = rCat.GetAge();
cout << "rCat is " << age <<" years old!\n";
cout << "&rCat: " << &rCat << endl;
// 메모리를 없애고 나면
\
SimpleCat * pCat = &rCat;    께보기  Yon) $f  사요  peer Ae
delete pCat;            님
// rCat 이 가리키는 값은?
a
return 0;             이  x Cet ol  We WL:
>                               이흔어 샤분하카 FECL .

SimpleCat &TheFunction()

<
SimpleCat * pFrisky = new SimpleCat(5,9);
cout << "pFrisky: " << pFrisky << endl;
return *pFrisky;

>

pFrisky: Ox2bf4
rCat is 5 years old!
&rCat: Ox2bf4

Zz
Bs
5
|
lo
호
oO
o&
NN
JZ
[표
+)
트여
oa
IN
x
fue
r=
re
OK
N
&o
it
fu
=z
고
로
wy


===== PAGE 288 =====
286 ㅇㅇ R24

참조자로 반환되었

피>

잠             니다.

25번 줄에서 TheFunction()°] 9100160#을 가리키는 참조자에 할당되었고 그 객체
고       이를 얻는데 쓰였으며 그 결과가 27번 SIA 출력되었습니다.

08100에서 선언된 참조자가 1068000004000에서 할당된 자유 기억 장소의 AAS

을 증명하기 위해 주소 연산자가 708에 사용되었습니다. 108가 가
리키는 주소가 출력되었고 이는 자유 기억 장소 주소와 변화가 없습니다.

og
의
의
ee

aa 좋습니다. 하지만 그 메모리는 어떻게 풀 수 있습니까? FAAS 0066할
니이 애스 시 eS

수 없습니다. 하나의 해결 방안은 또 다른 포인터를 만드는 것이고 여기에 #의
om

주소로 초기화하는 것입니다. 이럼으로써 메모리를 삭제하고 메모리 누출을 막습
나다-그럼에도 불구하고 하나의 Baas 가지고 있습니다. 31번 줄 다음에 실행
시 Cat FAS 가리키고 있겠는가 하는 것입니다. 앞서 말했듯이 참조자는 항
A 객체에 대한 다른 이름입니다. 만일 널 Aas 가리킨다면 그 프로그램

함조자가 널을 가리키는 프로그램은 험파일은 될지 모르지만, 실랭은 ase 수 없

비티.

피>

이 문제에 대한 해결책은 AME 3개입니다. 첫째는 25번 줄에 9000160#의 객체
를 선언하고 '1600000000으로부터의 반환을 값으로 받는 것입니다. 두 Wale
TheFunction()ol*] 9100160#를 힙에 만든 뒤 10600000000이 포인터를 반환하게
만드는 것입니다. 그리고 호출 프로그램에서는 그 포인터를 0066할 수 있습니다.
마지막 세 번째 답변 - 그리고 Sued] - 은 호출 함수에서 객체를 선언하고 그
참조자형을 16800000080에 전달하는 것입니다.

다. 그 메모리 FAS 포인터에 잡아두는 것이 절대절명인『
게 된다면 그 메모리는 풀어놓을 수가 없고 따라서 메모리
이 한 단위의 메모리를 함수들 사이로 전달하면서 항상 어떤 부분에선가가 그 포
인터를 가지고 있을 것입니다. 실제로는 메모리에 있는 값

니
때에

by

(nu

ae

= 28



===== PAGE 289 =====
제9일 BAN ee 287

되고 메모리를 만든 함수가 대개는 그 메모리를 풀어놓습니다. 이것이 법
니지만 그래도 일반적으로 지켜집니다.

sie) 함수가 heels 만들고 다른 함수가 지우는 것은 위험한 일입니다. 누가

가에 따라 다음과 같은 둘 중의 하나의 문제를 가지게 됩니
다. 메모리를 풀어놓는 것을 잊거나 아니면 두 번 풀어놓게 됩니다. 어느 쪽이든
심각한 문제를 야기합니다. 하나의 함수가 메모리를 만든 뒤 그 함수가 지우는

세

은 아

득     가 있는 함수를 하나 만들고 그리고 호출 함수
에게 그 메모리를 반환한다면, 여러분의 프로그램을 고칠 생각을 해봅시다. 호출
함수가 메모리를 할당하고 그 메모리를 참조자 전달 방식으로 전달합니다. 필요
로 하는 모든 BRS 돌아다닌 뒤 AS 함수로 돌아와서 지워버립시다.

오늘 여러분은 참조자란 무엇이며 포인터와 어떻게 다른지 비교하여 보았습니다.
참조자는 현존하는 객체를 참조하도록 초기화되어야 하고, 그후 다른 객체를 할
당받아서는 안됩니다. 참조자에 변화된 배용  은 모두 그 Epo] 가해진 것입니다.
참조자의 FAS 반환하면 Elo] 주소가 반환되는 것이 이에 대한 증명입니다.
잠조자를 통해 AA] 내용을 전달하는 것이 값을 전달하는 Aug 더 좋다는 것
을 알았습니다. 참조자 전달 방식은 역시 호출된 함수에서 그 내용을 변화시킨
뒤 호출 함수로 전달할 수가 있게 합니다.

를 전달하거나 반환을 할 때 참조자 또는 포인터를 써서 참조
수 있습니다.

어떻게 함수와 함수 사이에 ARS 효율적으로 전달하기 위하여 const 포인터와
const 참조자를 쓰는지를 보았습니다.

Pu ot
mgs 4}
2
=
코
때 ,표


===== PAGE 290 =====
288 ee 제2주

O&A

연구

Q 참조자가 할 수 있는 SE 일을 포인터가 할 수 있다면 참조자를 SLIM?

A 참조자가 사용하고 이해하기 더 쉽습니다. 간접 호출이 은폐되고 그 변수를 자꾸
소환할 Bor 없습니다.

Q 참조자가 사용하기 쉽다면 포인터는 왜 필요합니까?

A 참조자는 Yo] 될 수 없고, 또 한번 이상 치환될 수 없습니다. 포인터는 융통성

제공하지만 사용하기 다소 어렵습니다.

tho

Q AAAS 반환하는데 위험이 있다면 of 항상 값으로 반환하지 않습니까?
A

참조자로 반환하는 것이 훨씬 효율이 좋습니다. 메모리가 절약되고 프로그램이 빨

연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가

즈들과, 당신이 배운 것을 시험해 볼 수 있는 연습 문제들로

1. HAAS 포인터의 차이는 무엇입니까?

2 AEA 말고 포인터를 MOSHE 때는 언제입니까?

3. 여러분의 메모리가 충분하지 않을 때 newS 쓰면 무엇이 반환됩니까?
4 상수형 참조자는 무엇입니까?

$ㆍ 참조자에 의해 전달되는 것과 AAAS 전달하는 것의 차이는?


===== PAGE 291 =====
제9일 AAA ee 289

연습 문제

정수형을 선언하고 그 정수형에 대해 참조자, 포인터를 선언하는 프로그램을 작성하십시

1.

2.

cree

7.
8.

오. 포인터와 SEAS 사용하여 그 정수형에 있는 값을 다루도록 해봅시다.
AKA

STS 정수에 상수형 포인터를 ANSE 프로그램을 작성하십시오. 포인터를 정수형 변
수 18「016로 초기화하고 varOned| 6을 대입하십시오. 48[0116에 7이 들어가도록
포인터를 사용하십시오. 두 번째 정수형 변수 varTwoS 만드십시오. 포인터가

varTwos 가리키도록 다시 대입해 봅시다.

위의 프로그램을 컴파일하십시오. 오류가 있습니까? ADE 있습니까?
실종된 포인터를 만드는 프로그램을 작성해 봅시다.

4번 문제를 올바르게 고쳐봅시다.

메모리 누출을 일어나게 하는 프로그램을 만들어 봅시다.

6번의 문제를 올바르게 고쳐봅시다.

버그잡기

1: #include <iostreams.h>

a

3: class CAT

4% £

5: publ ics

6:   CATCint age) { itsAge = age; }
(3   “CAT(){}

8:   int GetAge() const { return itsAge; }
9: private:

10: int itsAge;

Wie 3s

12:

13: CAT & MakeCat(int age)

14: int main()

Vor Ke

16: int age = 7;

17: CAT Boots = MakeCat(age) ;

18: cout << "Boots is " << Boots.GetAge() <<" years old\n";

19: return 0;

20: }

2s

22: CAT & MakeCat(int age)

23: <

24:   CAT * pCat = new CATCage);
25%   return *pCat;

26: }

% 위의 프로그램을 잘 돌아가게 고쳐봅시다.


===== PAGE 292 =====


===== PAGE 293 =====


===== PAGE 294 =====
292 ee 제2주

5일째 학습에서 여러분은 함수를 다루는 기초들을 학습하였습니다. 이제 여러분
포인터를 다루는 법, 참조자를 다루는 법
다

을 좀더 배위야 합니

5일째 학습에서 여러분은-같은 이름

상의 함수를 가지고 다항 함수를 만들거나 함수 중첨을 구현하는 방법을 배웠습
니다.

[리스트 10.1]에 있는 보기에서 Rectangle 클래스는 두 개의 DrawShape() 함수를
가지고 있습니다. SAKE 매개 변수를 갖지 않고 클래스의 현재의 RS 가지고
Rectangle? 그립니다. 다른 하나는 2개의 값 - width, length - 을 가지고 Rectangle
를 그리는데 현재의 클래스 Be 무시합니다.

[리스트 10.1] 멤버 함수를 중접시키는 a       overLoading 4a

// [리스트 10.1] 멤버 함수를 중첩시키는 예
#include <iostream.h>

typedef unsigned short int USHORT;
enum BOOL { FALSE, TRUE};

// Rectangle 클래스 선언

class Rectangle

{

: public:

// 생성자

Rectangle(USHORT width, USHORT height);
“Rectangle() {}

CONBWOU FWD

SS td oe =5 =ㄴ SO
Ue We RS oO 8

// DrawShape 중첩
void DrawShape() const;
void DrawShape(USHORT aWidth, USHORT aHeight) const;

SS) oct
CON BO



===== PAGE 295 =====
세10일 고급 함

me
HU
Ot

ㅁ
+>
min

As
20:
218
228
23:
24:
255
26:
2c:
28:
298
30:
S13
S22
35%
34:
$5¢
565
371
38:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
51
52
35%
54:
55:
268
571
58:
59:
60:
61:
62:
63:
64:

private:
USHORT itsWidth;
USHORT itsHeight;
};

// 생성자 구련
Rectangle::Rectangle(USHORT width, USHORT height)
{

itsWidth = width;

itsHeight = height;
}

// DrawShape 선언 - 값이 없음
// 현재 클래스 멤버값에 의거
void Rectangle::DrawShape() const
{

DrawShape(itsHeight, itsWidth);
}

// DrawShape 중첩- 두 개의 값 가짐
//
void Rectangle: :DrawShape(USHORT height, USHORT width) const
{
for CUSHORT i = 0; i< height; i++)
{
for CUSHORT j = 0; j< width; j++)
{
cout << "x";
》
cout << [0
+

// 중첩 함수를 가지는

1

동 프로그램
int main()
{
// initialize a rectangle to 30,5
Rectangle theRect(30,5);
cout << "DrawShape(): \n";
wWbhr awShape() ;
cout << "\nDrawShape(40,2): \n";
rawShape(40,2);
return 0;
}

ee 293


===== PAGE 296 =====
294 ee Hox

a     DrawShape():

KKKKKKKKRKKRKRERERERKERRREKERRERERE
KKKEKKKKEKRKKKKEKRKEREKRKERERERRRKRERE
KKRKKKKKEKKEKRKER KERR ERR ERERERE
KKKKKEKKKRKKEREREREKRERR RE RERERERE
KKKKKKKEKERERERERE RE KRRRREKRERE

DrawShape(40,2);
KKK KKK KKK EKER ERE RE RERRRRRERERERERERERK
KKEKKK KEKE KKK ERE RE RRR RK RRR REREREREREKRK

분석  [리스트 10.1]은 첫째 주 복습 프로그램의 변형입니다. 지면을 절약하기 위
을          을 제외하였고 접근자 함수도 제외하였습니다.
주 프로그램이 메뉴를 출력하지 않고 간단하게 고쳐졌습니다.
그런데 중요한 부분은 16과 17번 DrawShapeQ7} 중첩된 부분에 있습니다. 이 부분
에 대한 중첩된 클래스 메쏘드 구현이 32-52번 줄에 있습니다. 매개 변수를 갖지
않는 DrawShape()°] 두 개의 매개 변수를 갖는 DrawShape)S 호출하는데 현재의
멤버 변수들을 전달합니다. 두 개의 함수에서 같은 코드를 중복시키지 않도록 심
혈을 기울였습니다. 왜냐하면 하나를 VAS 때 다른 하나를 잘못 고치면 프로그
램이 엉망이 되기 때문입니다.
54-64번 줄에서 객체를 만들고 DrawShape)S 호출하였는데 처음에는 매개 변수
가 없고 다음에 두 개의 unsigned short 정수형을 매개 변수로 전달합니다.

컴파일러는 사용된 매개 변수의 숫자와 형에 따라 알아서 함수를 호출합니다. 독
자는 때에 따라 하나의 변수와 하나의 나열형을 매개 변수로 갖는 2000680000라

는 또 하나의 중첩 함수를 만들 수 있습니다.

기본값(06【3나}[ Value) 쓰기

비클래스 함수가 하나 이상의 기본값을 가질 수 있는 것처럼, 클래스의 멤버 함
수도 그렇습니다. 기본값을 선언할 때 같은 법칙을 보여주는 예가 [리스트 102]
에 있습니다.

[리스트 10.2] 기본값을 사응하기

1: // [리스트 10.2] 기본값을 사용하기
2: #include <iostream.h>
3S:



===== PAGE 297 =====
제10일 고급 함수들 ee 295

typedef unsigned short int USHORT;
enum BOOL { FALSE, TRUE};

// 설원

class Rectangle

9: 4

10: public:

11;  // 생성자

12:  Rectangle(USHORT width, USHORT height);
13: “~Rectangle(){}

14:   void DrawShape(USHORT aWidth, USHORT aHeight, BOOL UseCurrentVals
= FALSE) const;

15:

16: private:

te   USHORT itsWidth;

18%   USHORT itsHeight;

19: 3s

20:

21: // 생성작 구현

22: Rectangle: :Rectangle(USHORT width, USHORT height):
23: itsWidth(width),

24: itsHeight (height)

Zor <F

26:

are

28: // 세 번째 매개 변수에서 사용되는 기본값
29: void Rectangle: :DrawShape (

50:   USHORT width,

S18   USHORT height,

52:   BOOL UseCurrentValue

33%   ) const

B4: 1

55:   int printWidth;

36:   int printHeight;

CONDO U >
ee …… 0 …

37:                                     4, No
38:   if (UseCurrentValue == RUB)          ah,

59:   {                               aa

40:     printWidth = itswidth; ~ p/®

41:      printHeight = itsHeight;

42:   By

43;   else                            put  AS.
44: <                        0

45°      printWidth = width;     =)  "

46:      printHeight = height;

47   Bg

48:


===== PAGE 298 =====
296 ee

제2주

49:

50:   for (int i = 0; i< printHeight; i++)
51%   18

525      for (int j = 0; j< printWidth; j++)
53%     {

54:        cout << "x"

55:     }

562      cout << "\n"

571

585 >

59

60: // 구동 프로그램

61: int main ()

625 1

63:   // initialize a rectangle to 30,5
64:   Rectangle theRect (30,5);

655   cout << "DrawShape(0,0,TRUE)...\n";
66:   theRect.DrawShape(0,0,TRUE) ;

67:   cout << "DrawShape(40,2)...\n";

68:   theRect.DrawShape(40,2);

69: return 0;

705 >

DrawShape(0,0,TRUE)...

KKKKKKKKKKKKEK KKK KEKE KKK KK
KKKKKKKKKKKKK KEKE KEK EKKKKKE
KKKKKKKKKKKKK EKER 헤세 해 규소 KKK
KKKKKKKKKKKKKKKKKE RRR
KKKKKKKKKKKKKKRKE KERR KEKR

DrawShape(40,2)...

KKK KKK KKK KK KK KEKE KER ERK RRR RRR RRR 규슈 고고 가가 가
KKK KKK KKK KKK KEKE KKK KKK KKK RRR RRR RRR

[리스트 10.2]는 FAH DrawShape) HES 기본 매개 변수를 가진 함수로
대체하였습니다. 14번 줄에서 3개의 매개 변수를 갖도록 선언되었습니다.

처음의 두 개는 0980#7형으로 선언된 aWidth, aHeighto|a 세   번째는
BOOL(TRUE 또는 84198)형의 06600060[8106이고 기본값은 FALSE@)U th.

의

SAE 29번 줄에서 시작합니다. 세 번째 매개 변수 UseCurrentValue7} 계산되

었습니다. TRUE} 멤버 변수 16\100와 itsHeight7} 지역 변수 printWidth,
printHeightS 설정하기 위해 사용되었습니다.


===== PAGE 299 =====
제10일 고급 함수들 ee 297

만일 UseCurrentValue7} 『41.98이면 - 기본값을 가지건 사용자가 설정하였건 - 처
음 두 개의 매개 변수가 지역 변수 200[\100, printHeight== 설정하기 위해 사용
었습니다.

106600060008106가 TRUE] 두 개의 매개 변수는 완전 무시됩니다.

기본값과 중첩 함수 중 어떤 AS 고를 것인가?

[리스트 10.1]과 [리스트 102]는 같은 WS 하지만 [리스트 1011에 있는 중첨된
함수가 이패이이 쉽고 자연스럽습니다. 프로그램에 대해 또 다른 변형이 wea
다면 - 예를 들어, 사용자가 width} heightS 사용하고 AAU 아니면 둘 다 사용
하기 싫은 경우 - 중첩된 함수를 응용하기란 어렵지 않습니다. 그러나 기본값은
새로운 변수가 더해지는 것처럼 복잡해집니다.

첩된 함수를 쓸 것인가 아니면 기본값을 쓸 것인가? 여기 법칙이 있습니다.
다음과 같은 때 £2 함수블 Balch

기본 *§’JXKDefault Constructor)

6일째 이야기하였듯이 여러분이 명시적으로 클래스에 대해 생성자를 선언하지 않
으면 기본 생성자가 생기고 매개 변수는 갖지 않으며 또 아무 일도 없습니다. 여
러분은 기본 생성자를 마음대로 만들 수는 있는데, 매개 변수는 없으나 객체를

초기화하는 일은 할 수 있습니다.

자동적으로 생기는 연산자는 기본 연산자라고 부르지만 말 그대로 아무런 매개
변수도 갖지 않습니다. 여러분이 명시적으로 만드는 것과 자동적으로 생성되는
것을 구별하십시오.

여러분이 생성자를 만들면 컴파일러는 기본 생성자를 안 만듭니다. 따라서 매개
변수가 없는 VHS 원하는데 이미 다른 생성자를 만들였다면 이를 기본 생성
정해야 합니다.


===== PAGE 300 =====
298 ㅎㅇ 제2주

생성자 중첩

생성자의 요점은 객체를 만드는데 있습니다. AS 들어, 8000080 생성자의 요점

은 사각형을 만드는 것입니다. 생성자가 동작하기 전엔 사각형은 없고 메모리의
3자가 호

출된 후엔 완전한, 언제라도 사용할 수 있는 개체가

[드어 eS 시 )

생성자는 멤버 함수처럼 sad 수 있습니다. $a 생성자를 만들 수 있다는 것
은 매우 강력하고 또 융통성이 있습니다.

예를 들어, 여러분이 두 개의 생성자를 갖는 사각형 객체를 갖는다 합시다. 처음
것은 가로와 세로를 갖고 그 치수의 사각형을 만듭니다. 두 번째 것은 WS 갖지
않고 기본값의 사각형을 만듭니다. [리스트 10331이 이러한 개념을 보여줍니다

[리스트 10.3] 생성자 중첩

1: // [리스트 10.37 생성자 중첩
28 //

3

4: #include <iostream.h>

52

6: class Rectangle

a x

8: public:

9:    Rectangle();

410   Rectangle(int width, int length);
113   “Rectangle() {}

12:   int GetWidth() const { return itsWidth; }
13:   int GetLength() const { return itsLength; }
14: private:

1B:   int itsWidth;

16:   int itsLength;

10e

18:

19: Rectangle::Rectangle()

20: £

21:   jtsWidth = 5;

22%   itsLength = 10;

23: >

24:

25: Rectangle::Rectangle (int width, int length)
26: £

af:   itsWidth = width;

28:   itsLength = length;



===== PAGE 301 =====
제10일 고급 함수들 ee 299

295 7}

30:

31: int main()

32: <

33:   Rectangle Rect1;

34:   cout << "Rect1 width: " << Rect1.GetWidth() << endl;
552   cout << "Rect1 length: " << Réct1.GetLength() << endl;
36:

37:   int aWidth, aLength;

38:    cout << "Enter a width: ";

39:   cin >> aWidth;

40:    cout << "\nEnter a length: ";

41:   cin >> aLength;

42:

435   Rectangle Rect2(aWidth, aLength);

44:   cout << "\nRect2 width: " << Rect2.GetWidth() << endl;
45:   cout << "Rect2 length: " << Rect2.GetLength() << endl;
46:   return 0;

47: }

결과 Rect1 width: 5

Rect1 Length: 10
Enter a width: 20

Enter a length: 50

Rect2 width: 20
Rect2 length: 50

분석  사각형의 클래스가 6 - 17번 줄에서 두 개의 생성자로 선언되었습니다. ow
- 줄의 기본 생성자와 10번 줄의 두 개의 변수를 가지는 생성자입니다.

33번 줄에서 Rectangle7} 기본 생성자를 사용하여 만들어졌고 그 값이 3435번 줄
에서 출력되었습니다. 3741번 줄에서 가로와 세로를 입력하도록 요청받았고, 두
개의 매개 변수를 취하는 생성자가 Be 줄에서 호출되었습니다. 마지막으로 밑
변과 높이가 44-451 줄에서 출력되었습니다.

컴파일러는 다른 중첨된 함수에서 그러하듯이 매개 변수의 개수와 형에 기반

여 적절한 생성자를 선택하여 사용합니다.

—

Ol
=


===== PAGE 302 =====
300 ㅎㅇ 제주

AYA 초기화

지금까지 여러분은 생성자 안에서 객체의 멤버 WES 추기화하여 왔습니다. 그
런데 생성자는 초기화 단계와 몸체의 두 곳에서 호출

다
WRB] 변수는 양쪽 어느 단계에서나 설정될 수 있습니다. 즉, 초기화 단계에

서
초기화하든지 생성자의 몸체에서 대입을 8258 일어납니다. 멤버 변수들을 추
기화 단계에서 초기화하는 것이 깔끔하고, 효율적입니다. 다음은 어떻게 멤버 변

기화하는지 보여줍니다.

687() :// 생성자 이름과 매개 변수
itsAge(5),// 초기화
itsWeight (8)

{3 // 생성자의 몸체

A
T

|

괄호 다음에 콜론을 써줍니다. 다음 멤버 변수들
습니다. 하나 i etl 과정이 일어난다면
정

마감
다
ge

때
HL
요
로
rir
모
oe
포
cE
4}
0!
고
ro
원
으
의 %
aw
aus
EN
nS)
원 |
45
&
> 16
tN
N
x
lo
re
off
ie
Gs

[리스트 10.4] 멤버 HAS 초기화하는 부분의 Sel

1: Rectangle::Rectangle():

2   itsWidth(5),

3   itsLength(10)

4:

5: Je

6:

7: Rectangle::Rectangle (int width, int Length)
8   itsWidth(width),

9   itsLength(length)

1
1

처음에 초기화되어야 하고 중간 몸체에서 대입할 수 없는 몇몇 변수들이 있
다. 참조자와 상수들이 그것입니다. 생성자의 몸체 부
들을 쓰는 경우가 Saad 가장 좋은 방법은 가능한 한 초기화하



===== PAGE 303 =====
제10일 고급 함수들 ce 301

복사 생성자(200\' Constructor)

기본 생성자와 기본 소멸자를 제공하는 것 외에도 컴파일러는 기본 복사 생성자
를 제공합니다. 복사 생성자는 개체의 복사본이 일어날 때마다 항상 호출됩니다.

AAS gee 전달할 때 - ta 전달하건 The 반환값으로 하건 - 그 객체

의 임시 복사본이 만들     . 만일 객체가 사용자가 정의한 객체라면 클래스

의 복사 생성자가 [리스트 9.6|에서 보았듯이 만들어집니다.

모든 복사 생성자는 하나의 매개 변수를 가집니다. 같은 클래스의 객체에 대한

참조자입니다. 이를 상수 참조자로 만들어 놓는 것이 좋은데 왜냐하면 생성자는

전달된 객체를 바꾸지 않을 것이기 때문입니다. 예를 들면

CAT(const CAT & theCat) ;

집니다. 복사 생성자의 목적은 0008에 대한 복사본을 fe . 것입니다

기본 복사 생성자는 매개 변수로 전달된 객체의 각 wy 변수들을 새로운 객3

멤버 변수들로 복사하기만 합니다.

ㅇ

대부분의 멤버 변수들에겐 좋은 일이지만, 자유 기억 장소 상의 객체를 가리키는
멤버 변수들은 다소 문제가 발생합니다.
새로운 얄은 SAt(shallow or member wise copy) >얄은 복사는 하나의 객체의 멤버 변
지져
웅이 FES] US 다른 객체에 정확히 복사하는 것을 말합니다. 양쪽의 포인터는 WES
Oe SS EE
같은 메모리를 WEBATAL 일반적언^ we BF deep copy)= 임의 새로 할당된 에   힙의 새로 할당된 메
모리에 갔을 복사합니다.
ODO ga mm
CAT 클래스가 자유 기억 장소상의 정수를 포인트하는 16486라는 멤버 변수를 가

]를 얄은 3 Amember-wise copy, shallow 000)라고도 하는데 비록 이런 방식이

진다면, 기본 복사 생성자는 전달된 047의 16486 멤버 WSS 새로운 047의

16486 멤버 변수에 복사합니다. 두 개의 객체는 같은 메모리를 포인트하며
다음 그림과 같습니다.

[그림 10.1]                            자유기억공간
기본 복사 생성자                                  5
사응하는 그림             old CAT                                        New CAT

itsAge     ㅋ                                               -     itsAge

이는


===== PAGE 304 =====
302 ee 제2주

이는 = 중 하나의 CATO] 범위 규칙을 벗어날 때 문제가 발생합니다. 8일째 공
부할 때 말하였듯이 소멸자의 역할은 메모리를 깨끗이 지우는 것입니다. 원래의
CATS] 소멸자가 메모리를 반환하는데 반해 WEE CATS] 아직도 지워진 메모리
를 가리키고 있다면 누출된 포인터가 만들어지고 프로그램은 비상에 돌입하게 됩
니다. [그림 10.2]가 이를 설명해 줍니다.

  ny

[그림 10.2]
잃어버린 포인터         5          /               자유기억공간
만들기                                      0]       ~
oN CA                                                New CAT

Atsage \         5°                                                                -        itsAge

이에 대한 해결책은 여러분 자신의 고유한 생성자를 만들고 새로운 메모리를 할
당하는 것입니다. 일단 메모리가 할당되면 과거의 gel 새로운 메모리에 복사됩
니다. 이를 깊은 복사(268 0000라하는데 [리스트 10.5에서 이를 보여줍니다.

[리스트 10.5] 복사 생성자

1: // [리스트 10.53 복사 생성자
25 77

3°

4: #include <iostream.h>

5:

6: class CAT

(i <

8: public:

9:    GAT Oy;    // 기본 생성
10: CAT (const CAT 8); // 복사 생성자
a fi   “CATO?   // 23s

12:   int GetAge() const { return *itsAge; +
15:   int GetWeight() const { return *itsWeight; }
14:   void SetAge(int age) { *itsAge = age; }

16: private:

17:   int *itsAge;
18:   int *itsWeight;
198 3?



===== PAGE 305 =====
제10일 고급 함수들 ee 303

21: 66116 600

225 <

23:   itsAge = new int;

24:   itsWeight = new int;

255   *itsAge = 5;

26:   *itsWeight = 9;

2s 3

28:

29: CAT::CATC(const CAT & rhs)

308 <

31:   itsAge =

32:   itsWeight

55%   *itsAge = rhs.GetAge();

34:   *xitsWeight = rhs.GetWeight();

358 >

36:

Sf: 66155 CATO

58: ¢

398   delete itsAge;

40:   itsAge = 0;

41:   delete itsWeight;

42:   itsWeight = 0;

43: }

44:

45: int main()

46: {

47:   CAT frisky;

48:   cout << "frisky's age: " << frisky.GetAge() << endl;
49:   cout << "Setting frisky to 6...\n";

50:   frisky.SetAge(6);

512   cout << "Creating boots from frisky\n";

52:   CAT boots(frisky);

53%   cout << "frisky's age: " <<  frisky.GetAge() << endl;
54:   cout << "boots' age: " << boots.GetAge() << endl;
55:   cout << "Setting frisky to 7...\n";

56:   frisky.SetAge(7);

571   cout << "frisky's age: "<< frisky.GetAge() << endl;
58:   cout << "boot's age: " << boots.GetAge() << endl;
59   return 0;

60: }



===== PAGE 306 =====
304 ee R24

겔과 frisky's age: 5

Setting frisky to 6...
Creating boots from frisky
frisky's age: 6

boots' age: 6

Setting frisky to 7...

frisky!  e: 7
boots' age: 6

6-198 줄에서 CATS] 클래스가 선언되었습니다. 9H 줄에서 기본 생성자가
AAT 10번 줄에서 복사 생성자가 선언되었습니다.

17, 18번 줄에서 두 개의 멤버 변수가 선언되었고 각각 정수형 포인터로 선언되
었습니다. 대개의 경우 클래스가 정수형 멤버 변수를 포인터로 저장할 이유는 없
습니다. 하지만 여기서 자유 기억 장소 상에서 어떻게 멤버 변수들을 다루는지
예를 보여주기 위해 사용된 것입니다.

a
AeA

나 21-27번 SNA BU ote Horse 가 Kes SOX
복사 생성자는 29번 줄에서 시작합니다. 매개 변수는 06임을 주목합시다. 복사
생성자의 매개 변수를 08라고 하는 것은 흔한데 이는  a (right-hand side) ©]
약자입니다. 33번과 34번 줄의 대입 문장을 보면 매개 변수로 전달된 객체는 '='
기호의 오른쪽에 VSS 주목합시다. 이것이 동작 이
31과 32번 줄에서 메모리가 자유 기억 Bool 할당되었습니다. 그리고 33, 34번
줄에서 새로운 메모리상의 값에다 기존의 04&1으로부터의 Ho] 대입되었습니다.
매개 변수 26는 상수 참조자 형태로 복사 생성자에 전달된 04&1입니다. 멤버 함
수 ths.GetAge()= rhs°] 멤버 변수 16480에 의해 포인트 된 etal 저장된 값을
반환합니다. thst CATS] 객체로서 다른 CATS] 모든 멤버 변수들을 가지고 있습
니다.
복사 BAZ} 새로운 CATS 만들기 위해 호출되었을 때, 기존의 CATO] 매개
wee 전달됩니다. 새로운 CATS 그 자신의 멤버 변수들을 직접 참조할 수 있
습니다. 하지만 새로운 CATS 범용 접근자 메쏘드를 사용하여 06의 멤버 변수들
을 접근해야만 합니다.
[그림 10.31은 여기서 무엇이 발생하였는지 보여줍니다. 기존의 CATH 의해 포
트 된 값이 새로운 CATS] 의해 BIA 메모리에 복사되었습니다.

cs


===== PAGE 307 =====
제10일 고급 함수들 ㅎㅎ 305

[그림 10.3]                            자유기억공간
Z2 복사0660 copy)
의 a

5

old CAT                                                                            New CAT

itsAge                                                                     ㄴㄴ       itsAge

47번 줄에서 CATO] 만들어졌고 ©) ES friskye} 칭해졌습니다. 나이가 출력되고
50번 줄에서 6으로 설정되었습니다. 52번 줄에서 복사 생성자를 사용하여 새로운
CAT boots7} 만들어지고 friskyS 매개 변수로 전달하였습니다.

53번과 54번 줄에서 각각의 CATS] 나이가 출력되었습니다. 당연히 boot] 나이는
frisky 2} 버러 6을 가졌고 기본 나이 5를 갖지 않았습니다. 56번 줄에서 82196의
나이가 7로 설정되었습니다. 그리고 나이가 다시 출력되었습니다. 이번에는 6496
의 나이가 비포 boot2] 나이는 6입니다. 이는 각각의 나이가 다른 메모리에 존재
한다는 것을 보여줍니다.
ie cee

CATS] 범위 규칙을 벗어나면 그 소멸자가 자동으로 호출됩니다. 047의 소멸자
구현 방식이 3743번 줄에 나타나 있습니다. delete7} 양쪽 포인터 itsAge,
itsWeight] 불려져 각각 메모리로 반환되었고 안전을 위해 각 포인터는 널로 재
할당되었습니다.

ky
에
로

연산자 =

oz 피
mH
ny
olf
s
reo
yy
2 of
iw a 2
4 #
Cy
+
+
*
>»
그
피  ew
an
fru
위
요
=
a
re
ie
x
qulnt
'.
Su
a2
ofp
x

분히 연구하기 위해서 [리스트 10.64) 새로운 클래스 Counter
만들었습니다. Counter 객체는 숫자가 증가하거나 감소하거나 또는 추적되어야
하는 순환문과 다른 응용 프로그램에서 숫자 세기를 할 수 있는 곳에 사용됩니다.


===== PAGE 308 =====
306 ee R24

[리스트 10.6] Counter 클래스

CONAOUFWYDY

60 60 [60 60 60 60 60 -5 2 그 그 그 그 그 그 그 그 wf
RAuRWNRBODWDOANADAUMUFWN HO Pe ee ee

PAGE
28:
29:

// [리스트 10.63 Counter 클래스
//

typedef unsigned short USHORT;
#include <iostream.h>

class Counter
{
public:
Counter ();
“Counter () {}
USHORT GetItsVal() const { return itsVal; }
void SetItsVal(USHORT x) fitsVal = x; }

: private:

USHORT itsVal;

o oe
: Counter::Counter():
아내

: int main(Q)
Ha

Counter i;

cout << "The value of i is " << i.GetItsVal() << endl;

return 0;

결과  The Value of i is 0

분석 보다시피 다소 불

정의된 기본 생성자는 하나의 멤버  변수 16\81을 0으로 초기화합니다

필요한 클래스입니다. 7-18번 Zo] 정의되어 있습니다. At
용하는 단 하나의 WE 09808#7입니다. 10번 줄에 선언되고

20번 줄에서

여기서 00006는 증가, 감소, 덧셈, 할당 등의 연산하지 못합니다. 단지 출력

데 쓰입니다.

하는



===== PAGE 309 =====
제10일 고급 함수들 ㅎㅎ 307

중가 £4(Increment Function) 만들기

연산자를 중첩하면 많은 기능들을 사용할 수 있습니다. 예를 SA Counter 객체를
증가하는 기능을 Vial 방법에는 두 가지가 있습니다. A 번째는 증가 연산자
BAS 쓰는 것인데 [리스트 10.7]에 있습니다.

[리스트 10.7] 중가 연산자 추가하기

// [리스트 10.77 증가 연산자 추가하기
//

1

2

3

4: typedef unsigned short USHORT;
5: #include <iostream.h>
6:

7

8

class Counter
때
9: public:
10%   Counter ();
148   “Counter (){}
12:   USHORT GetItsVal()const { return itsVal; }
148   void SetItsVal(USHORT x) CitsVal = x; }
14:   void Increment() { ++itsVal; }
i BYE
16: private:
172   USHORT itsVal;
1S!
193 가고
20:
21: Counter::Counter():
225   itsVal (0)
23:. 0%
24:
25: int main()
26: £
278    Counter i;
28:   cout << "The value of i is " << i.GetItsVal() << endl;
29:   ij.Increment();
30%   cout << "The value of i is " << i.GetItsVal() << endl;
51%   return 0;
328

겔과  The value of i is 0
The value of i is 1


===== PAGE 310 =====
308 ee 제2주

Bad [AE 1072S 14번 줄에 정의된 증가 함수를 사용하였습니다. 이렇게 해
~ 。 도 원하는 대로 동작은 하지만 다소 따분합니다. 단지 프로그램 내에 +a
산자를 사용해도 되는 것입니다.

전치 연산자(만에× Operator)S 중접(0+01080108)시키기
전치 연산자를 다음과 같이 함수를 선언함으로써 중첩시킬 수 있습니다.
반환형 060ㅎ6ㅁ810ㅇ『 op (매개 변수)

여기서 opt 중첩시킬 연산자입니다. 따라서 + 연산자를 다음과 같은 모양으로 |

중첩시킬 수 있습니다.
void operatortt+ ()

[JAE 1082 이러한 AIS 보여줍니다.

[리스트 10.8] operator++ Fa

// [리스트 10.83 operator++ 중첩
ff

typedef unsigned short USHORT;
#include <iostream.h>

class Counter

a

9: public:

10:   Counter ();

11;   “Counter () {}

125   USHORT GetItsVal()const { return itsVal; }
13:   void SetItsVal(USHORT x) {itsVal = x; }

CONOUFWYD

14:   void Increment() { +titsVal; }
158   void operator++ () { +t+itsVal; }
16:

17: private:

18:   USHORT itsVal;

19:

205 35

215

22: Counter::Counter():
23:   itsVal (0)
262 4};

26: int main(
2708 1"


===== PAGE 311 =====
제10일 고급 함수들 ee 309

28:   Counter i;

29   cout << "The value of i is " << i.GetItsVal() << endl;
50:   i.Increment();

Sie   cout << "The value of 1 is " << i.GetItsVal() << endl;
52:   +15

SSt   cout << "The value of i is " << i.GetItsVal() << endl;
34:   return 0;

35: +

The Value of i is 0
The Value of i is 1
The Value of i is 2

us
Ee

ISH 줄에서 연산자 ++가 중첩되었고 32H 줄에서 사용되었습니다. 0000
객체에서 기대했던 것과 많이 비슷합니다. 이 시점에서 사용자는 추가되어
야 할 부가적인 기능도 생각해야 합니다.

증가 연산자가 잘못 사용될 때에는 치명적인 결함이 발생합니다. 여러분이 대입
연산자의 오른쪽에 증가 연산자를 사용하면 실패합니다.

(rad
2

Counter a=++i; OY de .

ㅣ 코드는 새로운 Counter 8를 만들어 1를 중가시킨 후 1 값을 대입하려 합니다.

내장된 복사 생성자가 대입할 것입니다. 그러나 현재의 증가 ARE Counter 객
“ee wee 9

체를 반환하지 않습니다. 100형을 반환합니다. 여러분은 void 객체를 Counter 7

체에 대입할 수 없습니다.(아무 것도 없는데 뭘 만들 수 있는지)

ㅇ

중첩 연산자 함수에서의 반환값의 형

분명히 여러분은 00006@ 객체를 반환하여 이를 다른 00406@ 객체에 대입하려
AYE. 어떤 객체가 반환되어야 합니까? 하나의 접근 방식은 임시 객체를
뒤 이를 반환하는 것입니다. [리스트 10.9]7} 이를 보여줍니다.

ro (원

fn YF

[리스트 10.9) 임시 AME 반환하기

// [리스트 10.97 임시 Ways 반환하기
//

typedef unsigned short USHORT;
#include <iostream.h>

AOauUurWN =


===== PAGE 312 =====
310 ee 제주

7: class Counter

Se 4

9: public:

10%   Counter ();

V1:   “Counter () {}

125   USHORT GetItsVal()const { return itsVal; }
15%   void SetItsVal(USHORT x) {itsVal = x; }

14:   void Increment() { ++itsVal; }
15¢   Counter operator++ ();

16:

17: private:

18:   USHORT itsVal;

19

20: 3;

Palle

22: Counter::Counter():

23:   itsVal (0)

24: 3

255

26: Counter Counter: :operator+t+()

eta x

28:   +t+itsVal;

29%   Counter temp;

30%   temp.SetItsVal (itsVal);

a1:   return temp;

32% F

53:

34: int main()

55: £

36:   Counter i;

Sts   cout << "The value of i is " << i.GetItsVal() << endl;
38:   j.Increment();

39:   cout << "The value of i is " << i.GetItsVal() << endl;
40:   +r 12

413    cout << "The value of i is " << i.GetItsVal() << endl;
42:   Counter a = tti;

43:   cout << "The value of a: " << a.GetItsVal();

44:    cout <<" and i: " << i.GetItsVal() << endl;

45:   return 0;

46: }

겔과  The Value of i is 0

=
The Value of i is 1
The Value of i is 2
The value of a: 3 and i: 3


===== PAGE 313 =====
제10일 고급 함수들 ㅇㅇ 311

(ra

44)  이 버전에서 15번 SoA] Counter 객체를 반환하기 Sai] operator++7} 선언

되었습니다. 29번 줄에서 임시변수 temp7} 만들어지고 그 Be 현재의 객체
에 있는 값으로 설정됩니다. 임시 변수가 반환되고 즉시 42번 줄에서 8에 치환이
됩니다.

이름 없는(430101655) 임시 2A] 반환
29번 줄에서의 변수에 굳이 이름을 만들 BRE 없습니다. Ve) Counter7} 값을
지니는 생성자를 가진다면, 여러분은 단지 증가 연산자의 반환값으로써 생성자의
개

결과를 반환만 하면 됩니다. [리스트 10.10|이 이 개념을 보여줍니다.

[리스트 10.10] 이름 없는 임시 WAS 반환하기

1: // [리스트 10.107 이름 없는 임시 객제를 반환하기
22 ATE

3%

4: typedef unsigned short USHORT;
5: #include <iostream.h>

6:

7: class Counter

Be ft

9: public:

10:   Counter();

11:   Counter (USHORT val);

12:   “Counter (){}

13:   USHORT GetItsVal()const { return itsVal; }
14:   void SetItsVal(USHORT x) fitsVal = x; }
1581   void Increment() { ++itsVal; }
16:   Counter operatortt ();

103

18: private:

19:   USHORT itsVal;

20:

21: Fe

228

23: Counter::Counter():

24:   itsVal (0)

25 A}

26:

27: Counter::Counter(USHORT val):
28:   itsVal (val)

29: 42)

30:

31: Counter Counter::operator++()


===== PAGE 314 =====
312 ee 제2주

321: ¢

338   ++itsVal;

34:   retuned Counter (4tsval)

$55)

36:

37: int main()

38: {

59:   Counter i;

40:   cout << "The value of i is " << i.GetItsVal() << endl;
41:   i.Increment();

42:   cout << "The value of i is " << i.GetItsVal() << endl;
43:   af

44:   cout << "The value of i is " << i.GetItsVal() << endl;
45:   Counter a = tti;

46:   cout << "The value of a: " << a.GetItsVal();

47:   cout <<" and i: " << i.GetItsVal() << endl;

48:   return 0;

49: }

(a

&

|

The Value of i is 0
The Value of i is 1
The Value of i is 2
The value of a: 3 and i: 3

i  11번 줄에서 USHORTSS 가지는 새로운 생성자가 만들어졌습니다. 그 +
Ae 27-29번 So] 있는데 전달된 값으로 16\81을 초기화합니다.

operator++7} 매우 단순화되었습니다. 33번 SoH] itsValo] 증가되었습니다. 34번
줄에서 임시 Counter 객체가 만들어지고 16\8의 값으로 초기화되었고, operator++

의
이
시
이

면

this

결과가 반환되었습니다.

프로그램이 더욱 우아합니다. 그런데 왜 임시 객체를 et 만들려고 합니까? 임
객체는 생성되어야 하고 또 나중에 소멸되어야 하는데 각각은 그 만큼의 비용
소요됩니다. 또 이미 {라는 객체가 존재하고 이미 값을 가지고 있습니다. 그러
{를 반환하면 되는 것이 아닌지요?

포인터 사용하기

8일째에서 이야기한 this 포인터가 operator++ 멤버 함수에 전달되었는데 이는 다

콤

cs
객

모든 멤버 함수에도 전달이 됩니다. 005 포인터는 1를 포인트하고 소환이 되면
체 iS 반환합니다. 그리고 이때에는 그 멤버 변수 16\81에 원하는 We 가지고


===== PAGE 315 =====
제10일 고급 함수들 eo 313

있습니다. [리스트 10.11]은 이 006 포인터를 반환하고 불필요한 임시 객체를 만들
필요성을 제거하여 줍니다.

[리스트 10.11] this 포인터 반환하기

// 리스트 10.11] this 포인터 반환하기                         ：
//

il

2

3

4: typedef unsigned short USHORT;
5: #include <iostream.h>
6:

7

8

class Counter

£

public:

10:   Counter ();

118   “Counter(){}

12:   USHORT GetItsVal()const { return itsVal; }
13:   void SetItsVal(USHORT x) {itsVal = x; }

xo

14:   void Increment() { ++itsVal; }
15%   const Counter& operator++ ();
16:

17: private:

18:   USHORT itsVal;
19:

20: };

213

22: Counter::Counter():

23: itsVal¢o)
24: {3;           |                    09 Const Retume inp x

25:     —           @
Lyset a
26:| gonst Counter& Counter: :0perator++()    Cppr He Be  < abi ,
^

2781 (                                   Refe:        Re:          2
mn                                                        rence Return ae cae
&

t+titsVal;
return *this;
ea

29:

30% }

31:                                             인바692  Reference  Retum?
그 i main()                            Const 복어
34:   Counter i;

So!   cout << "The value of i is " << i.GetItsVal() << endl;

36;   i.Increment();

SC:   cout << "The value of i is " << i.GetItsVal() << endl;

38:   +4715

59%   cout << "The value of i is " << i.GetItsVal() << endl;

40:   Counter a = ++i;

41:   cout << "The value of a: " << a.GetItsVal();

42:   cout <<" and i: " << i.GetItsVal() << endl;


===== PAGE 316 =====
314 ee 제2주

45%   return 0;
44: }

결과 The Value of i is 0

The Value of i is 1
The Value of i is 2
The value of a: 3 and i: 3

2

= 2  operator++7} 구현되는 26-3081 줄에서 this 포인터를 소환하도록 바뀌었습니

다. Counter 객체가 ao] 대입되도록 합니다. 앞서 논의했지만, 만일 Counter
객체가 메모리를 할당받는다면 복사 생성자를 따로 만들어야 안전합니다. 이번
경우에서는 기본 복사연산자로도 충분합니다.

반환되는 것은 Countero 대한 소환값이므로 따로 추가의 객체를 만     = 없
습니다. Counters 쓰는 함수에 의해 값들이 변하지 않으므로 상수형 참조자를 사

용합니다.

J

후치 연산자 SAAlA]1|(Overloading the postfix Operator)

여태껏 여러분은 전치 연산자를 중첩하는 AS 배웠습니다. 후치 증가 연산자를
중첩하려면 어떻게 해야 합니까? 컴파일러는 전치자와 후치자를 구별 못하는데
문제가 있습니다. 개념상으로만 정수형 변수가 연산자 선언에 매개 변수로 제공
됩니다. 그 매개 변수의 값이 무엇이 되든 상관이 없습니다. 무시가 됩니다. 단지
이는 후치 연산자라는 BAS 나타내기 위한 하나의 약속일 뿐입니다. 잠시 후에
나올 [리스트 10.2]가 이 양자의 차이를 보여줍니다.

전치와 후치 연산자 차이
후치 연산자를 사용하기에 앞서 전치 연산자와의 차이점을 알아야 합니다. 이미
4일찌 [리스트 4.3|에서 보았습니다.
복습하면 전치는 “SA 후 가져오는 것"이고 후치는 “가져온 후 증가시키는
것"입니다.

따라서 전치 연산자가 값을 증가한 후 객체 그 자체를 반환하는 것에 반해, 후치
연산자는 증가되기 전에 값을 반환해야 합니다. 후치 연산자에서는 이람 하기 위
해 먼저 원래값을 갖는 임시 객체를 만들어야 합니다. 그 후 원래 객체의 He
증가시키고 임시 객체에 있는 값은 반환합니다.



===== PAGE 317 =====
A102 고급 함    ee 315

4>
min

다시 살펴봅시다. 다음 코드를 생각합시다.

a = xt+5

x7} 5라면 이 문장이 수행된 후 at 5이지만 x= 6입니다. 먼저 ×값 5를 반환하여
ao) 할당하고 *의 값을 증가합니다. 만일 x7} 객체라면 xo] 후치 연산자는 원래
값 5를 임시 객체에 숨기고 *를 증가시킨 후, 임시 객체의 WS ao] 할당합니다.
우리는 임시 객체에 담긴 값을 반환하므로 값00100으로 반환해야지 참조자로 반
~ 시

환하면 함수가 반환되는 EZ 개 임시 객체는 범위 규칙을 어기게 됩니다.
gp ae A Te IT A 가 가 가

[리스트 10.12] 전치 연산자와 후치 엽산자

// [리스트 10.12] 전치 연산자와 후치 연산자
//

typedef unsigned short USHORT;
#include <iostream.h>

class Counter

{

public:
Counter ();
“Counter () {}
USHORT GetItsVal()const { return itsVal; }
void SetItsVal(USHORT x) {itsVal = x; }
const Counter& operatort+ ();    // 전치 연산자
const Counter& operator++ (int); // 후치 연산자

CONDU FWD =
… es se ee oe …… oe ee

=A RP RS 3 3 = = = oO
NOU FWDN S| OO
… … … … ee ee …

: private:
USHORT itsVal;

Ry «3 oS
Oo 0 oC

인 가섰

NM
이 발스1

: Counter::Counter():
itsVal (0)

nN
Ww
…

인 4a)

6090 6090 60
nu 도

: const Counter& Counter: :operator++()
2 ‘t

nm Mm
00 N
…

+t+itsVal;
return *this;

WM
oO 이

ae

WNW
A) as

: const Counter& Counter::operator+t+(int x)
ria fi
34:   itsVal++;

Ww
Ww


===== PAGE 318 =====
316 ee 제2주

55%   return *this;

36: +

Ste

38: int main()

39: {

40:   Counter i;

41:   cout << "The value of i is " << i.GetItsVal() << endl;
42:   Vt;

43:   cout << "The value of i is " << i.GetItsVal() << endl;
44:   +475

45:   cout << "The value of i is " << i.GetItsVal() << endl;
46:   Counter a = ++i;

47:   cout << "The value of a: " << a.GetItsVal();

48:   cout <<" and i: " << i.GetItsVal( << endl;

49:   a= itt;

50:   cout << "The value of a: " << a.GetItsValQ;

51:   cout << "and i: " << i.GetItsVal() << endl;

525   return 0;

53: 가

결과  The Value of i
The Value of i

iis 0
1 15 1
The Value of i is 2
The value of a: 3 and i: 3
The value of a: 3 and i: 4

후치 연산자가 15번 줄에 선언이 오고 31-36번 줄에서 구현되었습니다. 14
번 줄 전치 연산자의 선언에서는 정수형 매개 변수 표시가 없습니다. 32번

줄에서 후치 연산자를 나타내기 위해 정수형 매개 변수 *를 사용하였습니다. 그
러나 그 값은 사용되지 않습니다.

연산자 중첩 - 단항 C4tA(Unary Operator)
중첩 연산자를 함수에 사용하듯이 선언합니다. 예약어 operators 연산자와 함께 사용합
다. 단항 연산자는 매개 변수를 사용하지 않는데 ct 후치 연산자의 BP 예외입니다.
후치 연산자(증가든 감소든)는 정수형 매개 변수를 하나 갖습니다.
on aoeanSseeaeSeoa ene es
예제 1

const Counter& Counter::operatortt ();

예제 2

Counter Counter::operator--(int);



===== PAGE 319 =====
r

DO    operator++ 로부터의 객체에 상수형 참조자를 반환합니다.
DON'T operator t+ REF] 반환값으로 임시 객체를 만들지 opaycy

덧셈 연산자
중가 연산자는 단항 연산자입니다. 증가 연산자는 단 하나의 객체에 대해서만 작
연산자(+)는 이항 연산자입니다. 두 개의 객체가 포함되어야 합니
다. Countero] 어떻게 덧셈 연산자의 Bao 만들 수 있을까요?

「

두 개의 Counter WS 선언하고 두 AS 더합니다. 아래 보기에 있습니다.

Counter varOne, varTwo, varThree;
varThree = varOne + varTwo;

여기서 Counters 인수로 갖는 4000 덧셈 함수를 만들고, 값을 더한 후, Counter
를 결과로 반환합니다. [리스트 10.13]이 이 방법을 보여줍니다.

[리스트 10.13] Add() 함수

// C2|ZE 10.13] ^00() 함수
//

1

2

3

4: typedef unsigned short USHORT;
5: #include <iostream.h>
6:

7

8

class Counter

인 에

9: public:

10:   Counter();

11%   Counter (USHORT initialVaLue) ;

V2:   “Counter () {}

152   USHORT GetItsVal()const { return itsVal; }
14:   void SetItsVal(USHORT x) {itsVal = x; }

Die   Counter Add(const Counter &);
16:

17: private:

18:   USHORT itsVal;

19:

20: 3;


===== PAGE 320 =====
318 ee 제2주

21:
eon
23:
24:
25
266
ars
28:
29:
30:
oe
325
oo:
54:
53
36%
37%
38:
39%
40:
41:
42:
43:

Counter::Counter(USHORT initialValue):
itsValCinitialValue)
nee,

Counter::Counter():
itsVal (0)
{}

Counter Counter::Add(const Counter & rhs)

<

return Counter(itsVal+ rhs.GetItsVal());

int main®)

{
Counter varOne(2), varTwo(4), varThree;
varThree = varOne.Add(varTwo) ;
cout << "varOne: " << varOne.GetItsVal()<< endl;
cout << "varTwo: " << varTwo.GetItsVal() << endl;
cout << "varThree: " << varThree.GetItsVal() << endl;
return 0;

결과

=

으로 초기화되어야 하기 때문에 또
니다. 이런 문제에 대한 또

varOne: 2
varTwo: 4
varThree: 6

15번 줄에서 4000가 선언되었습니다. 상수 00006 참조자를 가지는데 현재
의 객체에 더해질 값입니다. Counter 객체의 값을 반환하는데 38번 줄에서
보여지듯이 대입 연산자의 왼쪽 항으로 대입됩니다. varOnee 객체이고 varTwo7}
4000 함수에 매개 변수로 전달되고 결과가 \『11066에 저장이 됩니다.

varThreeS 초기화하지 않고 만들기 위해서는 기본 생성자가 필요합니다. 26-28번
줄에서 기본 생성자는 16\81을 0으로 초기화합니다. varOneS} varTwo 0아닌 값
른 생성자가 22 - 24번 줄에서 만들어졌습
른 해결책은 기본값 OF 11번 So 선언된 생성자

에 제공하는 것입니다.



===== PAGE 321 =====
제10일 고급 함수들 ce 319

operator+ #4
4000 함수 그 자체는 30-338 줄에 보여졌습니다. 아무 문제없이 작동은 하지만
다소 어색해 보입니다. + 연산자를 중첩하면 훨씬 부드러워 보입니다. [리스트
10.14]입니다.

[리스트 10.14] + 연산자

00 기 녀 에 에 060 =

609 060 060 060 PPP 2 2 2 그 2 그 그 6
의 90 = 2 DONA WU PWD | © cs os cs

nN
vu

NWWNW WG DP PO
WN = OC 6 ON

nN
~

nN
^

// 리스트 10.143 + 연산자
//

typedef unsigned short USHORT;
#include <iostream.h>

class Counter

a

public:
Counter();
Counter (USHORT initialVaLlue) ;
“Counter (){}
USHORT GetItsVal()const { return 16608, 고
void SetItsVal(USHORT x) {11500 = KrF
Counter operator+ (const Counter &);

: private:

USHORT itsVal;

은 강고

: Counter::Counter(USHORT initialValue):

itsVal CinitialValue)

은 C3

: Counter::Counter():

itsVal (0)

2 <2

: Counter Counter::operator+ (const Counter & rhs)
Oe

return Counter(itsVal + rhs.GetItsVal());

5 }

: int main()
르보
55%
36:
St

Counter varOne(2), varTwo(4), varThree;
varThree = varOne + varTwo;
cout << "varOne: " << varOne.GetItsVal()<< endl;


===== PAGE 322 =====
320

ee 제2주

38:   cout << "varTwo: " << varTwo.GetItsVal() << endl;

39:   cout << "varThree: " << varThree.GetItsVal() << endl;
40:   return 0;

41: }

결과  varOne: 2

varTwo: 4
varThree: 6

분섹 ㆍ 연산자가 15번 줄에서 선언되고 28-31번 줄에서 정의되었습니다. 이

수 4000와 비교하여 봅시다. S 다 거의 같습니다. 그러나 사용되는 구문은
ABE 다릅니다.

varThree = varOne + varTwo;
라고 하는 것이

varThree = varOne.Add(varTwo) ;

에

++ 연산자 중첨에 사용된 기법들이 다른 단항 연산자에 사용될 수 있는데 -- 연산자
가 이러한 것입니다

이항 연산자는 단항 연산자와 같은 방식으로 만들어지는데, 단 매개 변수를 갖습니다. 매
개 변수는 같은 형의 객체를 참조하는 상수 참조자입니다

Counter Counter::operator+ (const Counter & rhs) ;

예제 2

Counter Counter::operator- (const Counter & rhs. 3



===== PAGE 323 =====
제10일 고급 함수들 ee 321

연산자 중첩에서 몇 가지 이야끗거리

이번 장에서 말하였듯이 중첨 연산자는 멤버 함수가 될 수 있는데, 비멤버 함수
될 수 있습니다. 후자는 14일째에 프랜드 함수에 대해 논의할 때 이야기할 것
니다.

래스 WH} 되어야 하는 연산자는 대입 연산자(=), 첨자 연산자6]), 함수 호출
(a 간접 지정 AAT. opto 내일 배열이 이야기된 뒤 다룰 것
이고 간접 지정 연산자 중첩은 14일째 다룰 것입니다.

ro   "

연산자 중첩에 있어서의 한계

내장된 형에는(예를 들어, 정수형) 연산자가 중첩될 수 없습니다. 우선순위는 바
 수 없습니다. 또 항의 ee 항에서 다항으로, 또는 이항을 단항으로)

바꿀 수 없고 새로운 연산자를 만들 수가 없습니다. 따라서 * 연산자를 제곱 연
산자로 정의할 수 없습니다.

새로운 항의 W(arity) 항
용어 의 C++ 연산자는 단

이항이고 두 개의
?

중

=
딱 한 개 있습니다.

작입니다.

Cia eb 2x sy)

FAS 중첩시킬 것인가?

연산자 SAS C++ AM 프로그래머에 의해 가장 많이 사용되고 또 남용되는 기'
SS 하나입니다. 다소 애매 모호한 연산자를 만들고 사용해 보고 싶은 유혹이
생길 것입니다. 하지만 이러한 것은 SES 가져오고 읽기 어렴습니다.

정의하는 것은 재미있기도 하지

+
aS;
fo
mu
(로
nz
6
Hu
oe
to,
어
na
+
mu
em
nz
 10


===== PAGE 324 =====
322 ee laze

a
DON'T 직관적

대입 연산자

컴파일러에 의해 제공되는 마지막 함수는 대입 연산자(676000=)입니다. 이 연산
자는 여러분이 객체에 RS 할당할 때마다 호출이 됩니다.
CAT catOne(5,7);
CAT catTwo(3,4);

. 다른 코드 기술
catTwo = catOne;
여기서 64006이 만들어져 16486가 5로 초기화되었고 16\86194는 72 초기화되었
습니다. 6@01\0는 역시 각각 3과 4로 초기화되었습니다. 잠시 F catTwot catOne
의 값으로 할당되었습니다. 여기서 두 개의 이야깃거리가 발생합니다. 15486가 포
인터인 경우 어떤 문제가 발생할지와, 6010의 원래 값에는 어떤 변화가 오는가
입니다.
자유 기억 장소에 그 값을 가지고 있는 멤버 변수에 대한 논의는 앞서 복사 생성
자를 살펴보는 과정에서 이야기했었습니다. [그림 10.1]과 [그림 1022]에서 살펴보
았던 주제의 이슈가 다시 발생되었습니다.

C++ 프로그래머는 알은 복사(91010\ copy)%+ 깊은 복사(0660 copy)2] 양쪽을 구

양쪽
합니다. 얄은 BAS 멤버를 복사하고 양쪽의 객체는 자유 기억 장소상의 같
영역을 포인트하고 있습니다. 깊은 복사는 필요 메모리를 할당하고 이는 [그
| 아이 cae eet
10.3]에 보여줬습니다.

대입 연산자에는 추가로 다른 문제가 또 하나 있습니다. 00900 객체는 이미 존
a 할당된 메모리가 있다는 것입니다. 메모리 누출00600 1600이 없으려

면 다 사용된 메모리는 삭제되어야 합니다. 그런데 catTwoR 자신에다 할당하면
어떠한 문제가 발생할까요?

catTwo = catTwo ;

아무도 이런 US 고의로 하지는 않을 것입니다. 하지만 어
처리할 줄 알아야 합니다. 더욱 ae 것은 ae a
자기 자신에게 대입하는 경우를 BOSE 드러나지 않게 at
입니다.

no ro Ac

Ae



===== PAGE 325 =====
제10일 고급 함수들 ㅇㅇ 323

여러분이 이런 문제를 주의 깊게 해결하지 BAe catTwoe 할당된 메모리
삭제할 것입니다. 이후에 오른쪽 항에서 왼쪽으로 대입하려고 하는 경우 큰 문
가 발생합니다. 메모리는 이미 가고 없다는 것입니다.

이를 미연에 방지하기 위해 대입 연산자의 우변 항이 실제 존재하는 객체인지를
확인해야 합니다. OE this 포인터를 검사함으로써 나타납니다. [리스트 10.15]가
이를 보여줍니다.

골 때

[리스트 10.15] 대입 연산자

// [리스트 10.157 대입 연산자
if

#include <iostream.h>

class CAT

{

: public:

9:    CAT();    // 기본 생성자

10:  // 복사 생성자와 소멸자의 생략

[가오   int GetAge() const { return *itsAge; }
12:   int GetWeight() const { return *itsWeight; }
13:   void SetAge(int age) { *itsAge = age; }
14:   CAT operator=(const CAT &);

15%     7

16: private:

178   int *itsAge;

13:   int *itsWeight;

198 Fe

20:

21: CATS 3CATO

22% £

25°   itsAge = new int;

24:   itsWeight = new int;

23%   *xitsAge = 5;

26:   *itsWeight = 9;

27: }

28:

29:

30: CAT CAT: :operator=(const CAT & rhs)

51: £

S32:   if (this == &rhs)

53);      return *this;

34:   delete itsAge;

35:   delete itsWeight;

1
(2
3
4:
a:
6:
7
8


===== PAGE 326 =====
324 ee 제2주

36:   itsAge = new int;

ore   itsWeight = new int;

38:   xitsAge = rhs.GetAge();

59°   *itsWeight = rhs.GetWeight();

40:   return *this;
ATi 2

42:

43:

44: int main()

452 £

46:   CAT frisky;

47:   cout << "frisky's age: " << frisky.GetAge() << endl;
48:   cout << "Setting frisky to 6...\n";

49:   frisky.SetAge(6);

50:   CAT whiskers;

Hr   cout << "whiskers! age: " << whiskers.GetAge() << endl;
52: -cout << "copying frisky to whiskers...\n";

5S:   whiskers = frisky;

5A:   cout << "whiskers! age: " << whiskers.GetAge() << endl;
See   return 0;

568 +

결과 frisky's age: 5

Setting frisky to 6...
whiskers' age: 5

copying frisky to whiskers...
whiskers! age: 6

분석  [리스트 10.15]는 047 클래스로 FAS 돌리고 공간을 절약하기 위해 복사
~    생성자와 소멸자 AAS 생략합니다. 14번 줄에서 대입 연산자가 선언되고
30-41번 줄에서 정의되었습니다.
32번 줄에서 현재의 객체(좌변항)가 대입되는 객체와 같은지 검사되었습니다. 이
& thso] 주소가 045 포인터의 주소와 같은지 검사함으로써 이루어집니다.
이는 단일 상속자에서는 잘 동작되는데 다중 상속자에서는 13일째 논의가 이루어
지겠지만, 실패할 것입니다. 대신 다른 검사 방법이 있는데 this 포인터를 소환한
뒤 두 객체값이 같은지를 보는 것입니다.
if (*this == rhs)
물론, 등치 연산자(==)가 중첩되어야 하고 같다는 것이 어떤 의미인지 알아야 합
니다.


===== PAGE 327 =====
no
4>

A102 고급 함   ee 325

nin

변환 연산자

여러분이 내장된 BS] 변수(정수형 또는 5000)를 여러분이 정의한 클래스의 객체
로 대입하려면 어떤 일이 발생합니까? [리스트 10.16|은 다시 이야기를 Counter 클
래스로 돌려 0680#7형의 변수를 00006@ 객체로 대입하려 합니다.

[리스트 10.16]은 컴파일이 되지 않습니다.

도

oft
6

[리스트 10.16] 해야 를 00000에 대입하기

// [리스트 10.16] USHORTS Counter 대입하기
// 컴파일 안됨

typedef unsigned short USHORT;
#include <iostream.h>

class Counter
{
public:
Counter ();
“Counter () {}
USHORT GetItsVal()const { return itsVal; }
void SetItsVal(USHORT x) fitsVal = x; }
: private:
USHORT itsVal;

CONOU FWD =

= =] = = = = a2 2 co
NOW FWDY | 02

Heep

a at
‘Oo ©O

: Counter::Counter():
itsVal(0)

nm Mm
= ©

5

Nm mM
W PM

: int main()
s 고

6090 60 NY
 ~ 으

USHORT theShort = 5;

Counter theCtr = theShort;

cout << "theCtr: " << theCtr.GetItsVal() << endl;
return 0;

NN MY
~ CON
res)



===== PAGE 328 =====
326 ee 제2주

  설  7 - 17번 So] 선언된 0040@ 클래스는 기본 생성자만 가지고 있습니다. 이
프로그램에서는 USHORTS Counter 객체로 바꾸기 위한 특별한 다른 메쏘
있지 않습니다. 따라서 26번 SS 장애가 납니다. 컴파일러는 USHORT

갖고
멤버 변수 18\8에 대입하라고 말해주기 전까지는 알지 못합니다.

리스트 10.17]은 형 변환 연산자를 만들어 이 HAS 해결합니다. 이는 USHORT
를 가지고 00406@ 객체를 만듭니다

파일 장애! USHORTS Counter Boz 변환 못함

0 mus

를
=

.   10

=

[리스트 10.17] USHORTS Counter= 변판하기

// C2]A£ 10.17] USHORTS Counter= 변환하기
//

typedef unsigned short USHORT;
#include <iostream.h>

class Counter

{

9: public:

10:   Counter ();

Vis   Counter (USHORT val);

ize   “Counter () {}

1S   USHORT GetItsVal()const { return itsVal; }
14:   void SetItsVal(USHORT x) {itsVal = x; }
15: private:

16:   USHORT itsVal;

CONAWAU FWD
Pere ee ee ee eT ee

1382.33

20: Counter::Counter():
21%   itsVal (0)
22: (}

24: Counter::Counter(USHORT val):
25:   itsVal (val)

26: (7

ore

28:

29: int main®

50: <

Si:   USHORT theShort = 5;

32: Counter theCtr = theShort;       unaryner . Short
ROO OEE OOO



===== PAGE 329 =====
제10일 고급 함수들 ee 327

`

SS:   cout << "theCtr: " << theCtr.GetItsVal() << endl;
34:   return 0;
552 3

과  theCtr: 5

섹  중요한 변화는 생성자가 USHORTS 사용하도록 SAA 11번 So] 있고 |
생성자가 구현된 24-26번 줄에 있습니다. 이 생성자의 역할은 USHORTHY
터 CountrS 만드는 것입니다.

(ia us

여기에 이르면 USHORTS 그 매개 변수로 받아들이는 생성자를 호출할 수 있
니다. 그런데 대입을 다음과 같이 바꾸면 어떤 일이 발생할까요?
1: Counter theCtr(5);

2: USHORT theShort = theCtr;
3: cout << "theShort : " << theShort << endl;

ay

이러면 다시 한번 컴파일러는 CFS 발생시킬 것입니다. ase USHorRTZ
부터 0040@를 만드는 Ye 알지만 그 역은 모릅니다.

형 변환 연산자(60000 Operator)
는 유사한 BAS 풀기 위해 0++은 여러분의 클래스에 추가할 수 있
영 변환 연산자를 제공합니다. 이렇게 하면 여러분은 여러분의 a 내장
묵시적02001010으로 형 변환 할 수 있게 하여줍니다. [리스트 10.18]이
를 보여줍니다. 그러나 주의합시다. 형 변환 연산자는 반환값을 명시하
지 않습니다. 또 그렇게 해도 실제로는 변환된 값을 반환합니다.

[리스트 10.18] 000110로부터 47519060 9101[()로의 Y 변환

1: // [리스트 10.183] 00410[6『로부터 unsigned short() 로으 의 형 변환
28 7/

3

4: typedef unsigned short USHORT;

5: #include <iostream.h>

6:

7: class Counter

381

9: public:

1

08   Counter();


===== PAGE 330 =====
328 co 제주

a1:   Counter (USHORT val);

12:   “Counter () {}

15°   USHORT GetItsVal()const { return itsVal; }
14:   void SetItsVal(USHORT x) fitsVal = x; }

15s   operator unsigned short();
16: private:

17”   USHORT itsVal;

18:

195 33

20:

21: Counter::Counter():
22:   itsVal (0)
258 LF

25: Counter::Counter(USHORT val):
26:   itsVal (val)
208 (ㅠㅠ

29: Counter::operator unsigned short ()
303 <
315   return ( USHORT (itsVal) );

34: int main()

S55 1:

36:   Counter ctr(5);

3(:   USHORT theShort = ctr;

38:   cout << "theShort: " << theShort << endl;
59:   return 0;

과  theShort: 5

| 15번 줄에서 형 변환 연산자가 선언되었습니다. 반환값이 없습니다. 이 함
수의 구현은 29.32번 Zo] 있습니다. 31번 줄에서 반환값 16\81이 USHORT
로 변환되었습니다.

이제 컴파일러는 어떻게 USHORTS Counters 변환할지 또 역으로 어떻게 변환
하지르        압
할지를 제대로 압니다.      a   Unmanned  Shorte

(ust

(i
ie



===== PAGE 331 =====
요와

오늘 여러분은 어떻게 여러분의 클래스에서 멤버 함수들을 중첨하는지를 배웠습
니다. 또 기본값들을 함수에 주는 법을 배웠고 언제 기본값을 쓸지 또 언제 Sy
할지를 배웠습니다.

클래스 생성자를 SAE 것은 다른 객체로부터 만들어질 수 있는 아주 융통성
있는 클래스를 만들도록 해줍니다. 객체의 초기화는 생성자의 초기화 단계에서
일어나고 생성자의 몸체에서 WS 대입하는 것보다 훨씬 효율적입니다.

복사 생성자와 대입 생성자는 여러분이 고의로 만들지 않으면 컴파일러가 만들어

줍니다. 하지만 이는 He 복사입니다. 자유 기억 장소를 가리키는 포인터를 포함

한 멤버 자료를 가진 클래스에서는 이러한 메쏘드가 Ba 객체를 위한 메모리를

할당할 수 있도록 사용되어야 합니다.

대부분의 C++ 연산자는 중첩될 수 있습니다. 물론 자의적인 메쏘드가 맘대로 만

들어져서는 안됩니다. 연산자의 우선순위는 바꿀 수 없고 새로운 연산자를 만들

수도 없습니다.

ths 포인터는 현재의 객체를 참조하며 모든 멤버 Spo] 전달되는 보이지 않는

매개 변수입니다. 이 this 포인터를 소환하는 것은 종종 중첩된 연산자에 의해 이

루어집니다. |

형 변환 연산자는 객체간의 다른 형을 표현해야 하는 FA 사용될 수 있는 클
를 만들 수 있도록 해줍니다. 그런데 여기서 모든 함수는 명확한 반환값을

가져야 한다는 법칙은 적용하지 않아도 됩니다. 생성자와 소멸자와 같이 이들은

Q&A
Q #8 중첩시킬 수 있을 때에도 기본값을 쓰는 이유는?

A 함수가 두 개 있을 때보다 하나 있을 때 관리하기가 편합니다. 그리고 두 개의 함
수의 BAS 연구하는 것보다는 기본 매개 WSS 갖는 하나의 함수를 이해하는 것
이 쉽습니다 또 하나의 YEE 고치고 BASIE 두 번째 함수를 고치지 않는 것이
버그를 만드는 혼한 예입니다.

Q 중첩된 함수가 위와 같은 문제점들이 있다면 왜 항상 기본값을 쓰지 않습니까?


===== PAGE 332 =====
330 ee 제2주

A 중첩된 함수는 기본값이 제공하지 않는 SAS 보유하고 주 매개 변수의 목
ㅣ

록을 개수에 의해서가 아니라 형에 의해 바꾼다든ㅅ

Q 클래스 HAAS 만들 때 초기화 과정에 FAS 넣을 것이고 생성자 몸체에 TAS 넣

것인지를 어떻게 결정합니까?

Q 중첩된 함수가 기본 매개 변수를 가질 수 있습니까?

A 물론입니다. 이 강력한 특징을 가지지 못할 이유는 없습니다. 하나 이상의 중
함수들이 기본값의 일반 WSS 준수만 한다면 그 자신의 기본값을 가질 수 있

선 법칙을 초기화 과정에서 가능한 한 많은 것을 하라는 것입니다. 즉, 모든 멤버
수를 초기화합니다. 다른 일 - 계산, 출력 ㆍ Se 함수의 몸체에서 합니다.

첩된
스
[=]

Q 왜 어떤 멤버 함수들은 클래스 선언시 정의되고 다른 것들은 그렇지 않습니까?
A 선언부 안에 멤버 함수로 구현을 정의하는 것은 일을 그때그때 처리할 수 있게 합

니다. 단 이는 함수가 매우 간단할 때 합니다. 단 함수가 클래스

연구

있습니다. 버버 Dol 있는 답을 보기 전에 각 물음에 대답을 할 수

1. 멤버 함수를 중첩할 때 어떤 방식으로 그들이 구별되어야 합니까?
2% AAD 정의의 차이점은 무엇입니까?
3 언제 복사 생성자가 호출됩니까?
4. 언제 소멸자가 호출됩니까?
$ 복사 생성자는 대입 연산자(=)와 어떻게 다릅니까?
6 this 포인터란 무엇입니까?
% 전치 증가 함수와 후치 증가 함수를 중첩하는 것을 어떻게 구별합니까?
8 operator+S 11011 정수형으로 중첩할 수 있습니까?

선언의 바깥에 있
다고 할지라도, 예약어 1106를 써서 멤버 함수를 만들 수 있습니다.

연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가
를 확인해보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어
있도록 노력하


===== PAGE 333 =====
제10일 고급 함수들 eco 331

9% ㅜㅜ에서 operator+ +3 여러분의 클래스에서 값을 감소시킬 수 있도록 중첩시킬 수
있습니까?

10. 형 변환 연산자는 그 선언부에서 어떤 반환값을 가집니까?

뼈

연습 문제

1. 단 하나의 멤버 변수 itsRadiusS 갖는 SimpleCircle 클래스 MAL 만드시오. 기본
생성자와 ABA, 반지름에 대한 접근 AAS 포함시키도록 하십시오.
2 1H 문제를 가지고 만든 클래스를 사용하여 기본 MAAS 구현하는 함수를 작성하고

itsRadiusS 52 초기화하십시오.     v

3 같은 클래스를 사용하여 두 번째의 MAAS 만드는데 매개 변수로부터 값을 받고 그 값
을 itsRadiusol] 저장하도록 하십시오.  、^

4 SimpleCircle 클래스에서 itsRadiusS 증가시키는 전치, 후치 증가 연산자를 HEAL

5. SimpleCircle 클래스에서 itsRadiusS 자유 기억 장소에 저장하도록 바꾸고, 현재의
ACS 맞도록 고치시오.

6. SimpleCircleol] 복사 생성자

7. 510701601「016에 operator=

&@ 두 개의 SimpleCircle 객체를 만드는 프로그    만드시오. 하나는 기본 생성자를 갖
도록 하고 ,다른 하나는 그 값을 9로 설정하여 생성하시오. 각각을 증가시키면서 출력합
시다. 마지막으로 첫째 객체를 두 번째 객체에 대입하고 값을 출력하여 봅시다.

9 버그잡기

SQUARE SQUARE: :operator=(const SQUARE & rhs)
{

nujnu

만들도록 하십

십시오
만들도록 하십시오.
램을

AHA

생성

mio   내

itsSide = new int;
*xitsSide = rhs.GetSide();
return *this;

}

10. 버그잡기

VeryShort VeryShort::operator+ (const VeryShort& rhs)
{

itsVal += rhs.GetItsVal();

return *this;


===== PAGE 334 =====
가는 페이지2



===== PAGE 335 =====


===== PAGE 336 =====
334 ee 제2주

서문

를 문자열이란 무엇이고 문자열을 만들기 위해 어떻게 문자 배열을 쓰는가?

ui A(array)o]@+ 자료를 해 장소들의 모임체(60160000)인데 각각은 같은 형
을 저장합니다. 각 저장 장소는 배열의 €125(element) 2} 불립니다.
여러분은 각 배열     을 쓰고 배열의 이름을 쓴 뒤 첨자(64080100를 합니다. 첨

자는 항의 ASE 나타내고 대괄호로 묶여집니다. 예를 봅시다.

long LongArrayl25];

이는 2572] long AEBS 1008403라는 이름으로 선언하였습니다. 컴파일러가
이 BAS 보면 25개의 PS 보관할 메모리를 할당합니다. long 정수형이 4바이트
의 메모리를 가지므로 이 배열은 100개의 연속되는 메모리를 차지하게 됩니다.
[그림 11.1]에 있습니다.

[그림 11.1]
배열 선업하기

100 바이트


===== PAGE 337 =====
제11일 배열 ee 335

배열 SYA(Array Element)

여러분의 각 배열의 MAE 배열 이름으로부터 변위(08*00를 지정하여 접근할 수
있습니다. 배열의 원소는 0부터 시작됩니다. 따라서 첫 번째 원소는 448400히이
이 됩니다. 1008408》의 예에서는 LongArray[0]o] 배열의 첫 번째 원소가 되고
LongArray[1]°] 두 번째 원소가 됩니다.

다소 혼동될지 모르겠습니다. 9006408>[3]은 3개의 AAS 가지고 있습니다. 각
각은  SomeArray[0],  SomeArray[1],  900064208112]입니다. 일반화시켜 말하면
SomeArray[n]-= 개의 원소를 가지고 있는데 그 배열은 9006408)|이부터 시작하
여 SomeArray[n-1]= 끝납니다.

따라서 LongArray[25]*= 1008400이부터 시작하여 LongAmay[24]7}2] 있습니다.
[리스트 11.11에 MAS 가진 배열을 선언하고 각각을 값으로 채우는 과정을 보여
줍니다.

[리스트 11.1] 정수형 배열을 사응하는 예

1: // [리스트 11.1] 정수형 배열을 사용하는 예

2: #include <iostream.h>

3:

4: int main)

ps

6:    int myArray(5];

(?    Int: 12

8:    for (int i=O; i<5; i++) // 0-4

or    C

10:     cout << "Value for myArrayL" << i << "J: ";
a fia     cin >> myArrayLil;

2%   내

122   for (i = 0; i<5; i++)

14:     cout << i << "i" << myArrayLlil] << "\n";
158   return 0;

162 >

24 Df  Value for myArrayLOJ: 3
Value for myArrayL[11]: 6
Value for myArrayL[2]: 9
Value for myArrayL[3]: 12
Value for myArrayL[4]: 15


===== PAGE 338 =====
336 ee 제2주

FWN = OO
= FS OAWN

2

5
불셀 oe SS myAmyete 이름의 배열을 선언하였고 5개의 Bre 변수의 값
을 갖습니다. 8번 SS 0부터 4까지 세는 - 5개항의 WAS 나타내는 - =
환을 반복하였습니다. 사용자는 값을 입력하도록 요구받고 각 ge wee 적절
한 변위에 위치하여 저장됩니다. 첫 번째 WS myAmay[OJo] 저장이 되고 두 번째
값은 79&009111에 저장이 됩니다. 두 번째의 for 순환문에서는 각각의 값을 출력

합니다.

배열은 0부터 시작하지 1부터 시작하지 않습니다. 이런 것이 사실 ++에서 많은 버그
의 원인이 되기도 합니다. 여러분이 MSS Aree 떼마다 주의해야 함니다.
ArrayName[ 10] ArrayNamel0]42=| ArrayName[9]™t*] 진행됩니다. ArrayNameL 10]

은 없습니다.

배열의 BS 지나 AS 저장할 경우        ;

YS Ao] 원소에 저장할 때 컴파일러는 각 값을 그 원소의 크기와 첨자의 개
수에 따라 어디에 저장할지를 계산합니다. 가령, 여섯 번째 원소인 1008&04515|에

을 저장하도록 요구를 했다고 합시다. 컴파일러는 변위의 aoa 원소의
크기(를 곱합니다. 다음에는 그 곱한 Ws 배열의 첫 번째 위치부터 시작
하여 그만큼의 위치로 이동을 하여 주어진 AS 저장합니다.

만일 여러분이 LongArray[50] 위치에 값을 저장한다면 컴파일러는 그 항이 프로그
램에서 존재하는지 안하는지 검사를 안합니다. 단지 그 배열의 처음 위치에서 얼
마나 먼 곳에 gS 저장해야하는지 - 여기서는 200 바이트 - 계산하고 그 곳을
찾아가 그냥 저장해버립니다. 모든 자료가 저장될 수가 있습니다. 이 새로운 He
저장하면 사실 어떤 일이 일어날지 모릅니다. So] 좋으면 여러분의 프로그램은
그 즉시 깨져 버릴 수 있습니다. 운이 없으면 프로그램의 아주 뒷부분에 가서 예
상 못한 결과를 가져올 것입니다. 그리고 그 때는 어디에서 오류가 나는지 한참
찾아야 할 것입니다.

컴파일러는 마치 집을 떠나 다른 집을 찾아가는 장님과도 같습니다. 그는 첫 번
째 집 MainStreet{O]}2 떠납니다. 여러분이 그에게 6번째 집을 찾으라고 하면 그는



===== PAGE 339 =====
제11일 배열 ee 337

속으로 계산합니다. “앞으로 5번째 집을 더 가야한다. 각 집은 큰 보폭으로 4걸음
이다. 따라서 나는 20걸음을 더 걸어야 한다.” 그리곤 걸어갑니다. 만일 여러분이
MainStreet[100]}-&- 찾아가라고 하면 장님은 400걸음을 가야한다는 것을 계산합니
다. 실제 집은 25개밖에 없다는 것을 알지 못하고 그는 400걸음을 걷습니다. 한참
후 그는 차도에 들어설지도 모릅니다. 그를 어디로 보낼지 여러분은 주의를 기울
여야 합니다.

[리스트 11.2]의 프로그램이 배열의 BS 지난 경우 어떤 일이 일어나는지 보여줌
니다.

이 프로그램을 실랭시키지 QML - 여러분의 시스템을 파괴할지 모릅니다.

[리스트 11.2] 배열의 BS 지나 BS 저장하는 경오

나게

2: // [리스트 11.21 배열의 BS 지나 WS 저장하는 경우

Se //

Ae

5: #include <iostream.h>

6: int main()

a at

8:   // sentinels

9:   long sentinelOneL[3];

10: long TargetArray[25]; // array to fill

11: long sentinelTwoLl3J;

Nae

13: for (int i=0; i<3; i++)

14:     sentinelOneLil = sentinelTwoLil] = 0;

hoe

16: for (i=0; i<25; i++)

17%     TargetArrayLil = 0;

18:

19: cout << "Test 1: \n"; // test current values (should be 0)
20: cout << "TargetArray[O]: " << TargetArray[l0] << "\n";
21: cout << "TargetArray[24]: " << TargetArrayl24] << "\n\n";
225

23: for (1 = 0; i<3; i++)

24: 세

25%     cout << "sentinelOneL" << i << "J: "

26:     cout << sentinelOneLil << "\n";

ars     cout << "sentinelTwoL" << i << "J: "

283     cout << sentinel Twolil<< "\n";


===== PAGE 340 =====
338 ee 제2주

292 +

505

31: cout << "\nAssigning..."7

32: for (1 = 0; i<=25; i++)

33:     TargetArrayLil = 20;    업어 든 ayelzbl 많으.

34:

35: cout << "\nTest 2: \n";

36: cout << "TargetArrayLO]: " << TargetArrayLO] << "\n";
37: cout << "TargetArray[24]: " << TargetArray[24] << "\n";
38: cout << "TargetArray[25]: " << TargetArrayL[25] << "\n\n";
39: for (i = 0; i<3; it+)

40: ¢f

“13     cout << "sentinelOneL" << i << "J: "7
42:     cout << sentinelOneLil<< "\n";

43:     cout << "sentinelTwoL" << i << "J: ";
44:     cout << sentinelTwoLil<< "\n";

45: _ㅠ

46:

473   return 0;

48:}

결 1h Test 1:

TargetArrayL0OJ1: 0
TargetArrayLl24]: 0

SentinelOneL01:
SentinelTwoLl0J:
SentinelOneL1]:
SentinelTwoLl1]:
SentinelOneL[2]:
SentinelTwoL2]:

oo o Oo oc ©

Assinging...

Test 2:
TargetArrayL0J]: 20
TargetArrayLl24]: 20
TargetArrayl25]: 20

SentinelOneL01: 20
SentinelTwoLl0J:
SentinelOneL[1]:
SentinelTwol11]:
SentinelOneL2]:
SentinelTwoLl2J]:

ㅇ20000



===== PAGE 341 =====
제11일 배열 ee 339

: 분석 9, 11번 줄은 TargetAray 주변을 돌아다니며 파수꾼 역할을 하는 3개의 정
Tes 갖는 두 태터 배열을 갖습니다. 각 "ae 0   으로 초기화됩니다. 메

모리가 TargetArayS] 끝을 넘어가면 960086의 값이 변할 것 같습니다. 어떤 컴파
일러는 메모리에서 억순으로 저장되고 다른 컴파일러는 정순으로 저장됩니다. 그

eA] sentinel-S TargetArray 양쪽에 선언합니다.

19-29번 SoA] TestlS 통해 560086의 값을 확인해 봅시다. 33번 줄에서
7008아408》의 멤버가 모두 20으로 초기화되었습니다. 그런데 TargetArray2] 변위가
25까지 설정되었고 TargetAray[25]= 선언하지 않았습니다.

35-38번 줄에서 1690라는 이름으로 TargetAmay®] BSS 출력합니다. 다행히
TargetArray[25]2]_ 값이 아무런 이상 없이 출력되었습니다. 그러나 9600060006와
86000611\0의 값을 출력하여보면 960006070|이의 값이 변하였음을 알 수 있습니
다. 이를 어떻게 해석할 수 있는가 하면 TargetAmayS] 25번째 원소가 바로
56000611\0의 OHA] 원소와 같은 메모리를 사용한다고 할 수 있습니다
TargetArray[25] 172] 원소가 접근되면 AAZE sntinelTwoo] A 번째 원소가 A
근되는 것입니다.

이러한 버그는 찾기가 몸시 어렵습니다. 왜냐하면 sentinelTwo2] 원소가 프로그램
에서 전혀 쓰지도 않았는데 바뀌었기 때문입니다.

여기서 9600061의 상수로 3을 썼고 18080.408의 개수로 25를 사용하였는데 이는
상수로 정의하여 쓸 수 있습니다. 그렇게 하면 한번 바꿀 때 모두 일일이 쫓아다
니며 바꿀 필요가 없습니다.

솔타리 말뚝 오류

배열의 BS 넘어 값을 다루는 것은 하도 흔한 오류라 아예 그 이름이 붙어 있습
니다. 울타리 말뚝 오류라 합니다. 이는 다음의 문제에서 나옵니다. 한 단위의 울
타리를 막는데 1개의 말뚝이 필요하다면 10개의 울타리를 치는데 몇 개의 말뚝ㅇ
필요합니까? 대부분 10이라고 하겠지만 실은 11입니다. 그림을 봅시다.

1  2  3  4  2  7  2 ~  1

1번          2번         3번          4번         5번         6번          7번          8번         9번         10번

~

@
o

[그림 11.2] 솔타리 말뚝 오류


===== PAGE 342 =====
340 ㅎㅇ 제주

이 한 개의 차이가 프로그래머의 세계에서 종종 일어납니다. 아주 흔히 여러분
25개의 원소를 가진 배열이 24까지 세어지는 것을 봅시다. 0부터 세어지기 때
입니다.(프로그래머는 종종 왜 건물에 0번째 충이 없는지 ESS 합니다. 실제
몇 프로그래머는 5충에 도달하기 위해 4층 번호 판을 누른 경우도 있습니다:)

bid aa rlo

어떤 프로그래머는 ArrayNamelOS 0번째 원소라 합니다. 이런 습관에 물들면 안
습니다. AvrayName[0]°] 0번째 원소라면 ArrayName(1]2 몇 번째 BAe? 첫
째인가? 만일 그러하다면 ArrayName(24] HAS 보면 이를 24번째 원소라 할 것
가? 아닙니다, 분명 25번째 원소입니다. 따라서 ArrayName(O]2 0번째 변위라 말하는
것이 옮고 이는 첫 번째 원소라 하는 것이 옮습니다.

배열 초기화

여러분은 정수형이나 문자형 같은 내장된 Bo] 간단한 배열은 선언시 초기화를
할 수 있습니다. 배열의 이름 뒤에 =표시를 하고 섬표로 분리된 WES 중괄호로
막아서 초기값을 지정할 수 있습니다. 한번 봅시다

int IntegerArrayL51] = { 10, 20, 30, 40, 503;

IntegerArray=S 5개의 정수형을 가지도록 하였습니다. IntegerArray[0]°] 10을 저장
하였고 IntegerArray[1]o] 20을 저장하였고 나머지도 그런 식으로 하였습니다.
여러분이 만일 배열의 크기를 적지 않았다면 처음 초기화 값들을 저장할 수
정도의 크기로 배열이 잡힙니다. 따라서

int IntegerArrayLl] = { 10, 20, 30, 40, 50};

라고 쓰면 처음에 잡았던 배열과 같은 크기가 잡힙니다.

여러분이 배열의 크기를 알고 싶다면 컴파일러에게 요구할 수 있습니다. 예를 들면

const USHORT IntegerArrayLength
IntegerArrayLength = sizeof (IntegerArray) / sizeof (IntegerArrayLl0])

3
ttlo

는 상수 USHORT 변수 IntegerArrayLengthS 다음 값으로 설정합니다. 전체 배열
의 크기를 각 배열의 한 원소의 값으로 나눔니다. 그 Ke 배열에 있는 멤버의
숫자입니다.



===== PAGE 343 =====
제11일 배열 ee 341

int IntegerArray[5] = (10, 20, 30, 40, 50, 60} ;

는 틀립니다. 왜냐하면 5개의 배열을 만들고 6개의 값으로 초기화하였기 때문입
니다. 그러나 다음은 됩니다.

int 101696『4『ㄷ80753 = { 10, 20};

나머지 초기화되지 않은 PRS 값을 보장할 수 없습니다만 실제 표준안에서는 0
으로 초기화됩니다. 배열 Yo] 초기화되지 않으면 0으로 설정됩니다.

00     컴파일러가 로기화된 배열의 크기를 설정토록 합시다.
DONT 배열 크기를 지난 곳에 WAS 하지 Beh.

00 변수에서 그랬듯이 배열 이름은 의미를 가진 것을 주도록 합시다.
DO 배열의 첫 번째 원소는 변위 0임을 기억합시다.

변수 선언
배열은 적절한 변수명을 가질 수 있습니다. 단 같은 범위 WI 같은 변수명이
나 같은 배열명하고 ae 않으면 됩니다. 따라서 여러분은 1000치라는 배열
명과 0`08이라는 변수명을 같이 가질 수는 없습니다.

배열의 차원을 상수형이나 나열형으로 SF 있습니다. [리스트 11.3|을 봅시다.

[리스트 11.3] 배열에서 상수형과 나열형

1; // [리스트 11.33 HS 상수형과 rag

Ze 77

33

4: #include <iostream.h>

5: int main()

6: 1

Gi    enum WeekDays { Sun, Mon, Tue, Wed, Thu, Fri, Sat, DaysInWeek };
8:

5    int ArrayWeek[DaysInWeek] = { 10, 20, 30, 40, 50, 60, 70};
10%

Tie   cout << "The value at Tuesday is: " << ArrayWeek[Tuel];

125   return 0;

132 +



===== PAGE 344 =====
342 ee R24

24 lh  The Value at Tuesday is: 30

분석  TH 줄에서 \6602856라는 나열형을 만들었습니다. 8개의 WAS 가지고 있
습니다. Sune OF} 같고 DaysinWeek= 7과 같습니다.

11번 줄에서 나열형의 상수 Tues AY WIS 지정하는 상수로 썼습니다. Tue
는 2이고 따라서 배열의 세 번째 원소가 되며 ArrayWeek(2}2] go] 전달되어 11
번 줄에서 출력됩니다.

배열

배열을 선언하기 위해서는 저장되는 자료의 BS 먼저 MAT 배열의 이름을 Such, 첨자
를 객체의 개수와 함께 써줍니다.
예제 1

int MyIntegerArrayl90];

예제 2
Long * ArrayOfPointersToLongl[1001];

배열의 멤버에 접근하기 위해 첨자 ANAS SUC.

예제 1
int theNinethInteger = MyIntegerArrayL8];

예제 2
Long * pLong = ArrayOfPointersToLongL81];

배열은 (부터 시작되고 크기 nel 배열은 0부터 0-1까지 있습니다.

랙체의 배열

어떠한 객체도 - 내장된 것이든 사용자가 만든 것이든 - 배열에 저장될 수 있습
니다. 배열을 선언할 때 컴파일러에게 객체의 형을 알려주고, 공간을 잡을 수 있
도록 객체의 크기를 알려줍니다. 컴파일러는 클래스              를
저장하는데 열만큼의 여유가 필요한지를 알아닙니다.
는 기본 생성자를 가져 배열이 정의될 때 객체가 만

_ 배열에 있는 멤버 자료에 접근할 때 두 단계의 과정이 필요합니다. 인덱
연산자([])를 사용하여 배열상의 WS 구별해내고 멤버            |

로 =

  os



===== PAGE 345 =====
AS 배열

ee 343

특정 멤버 변수를 찾아갑니다. [리스트 11.4가 어떻게 5개의 CAT 배열

지 보여줍니다.

[리스트 11.4] Axo) 배열 만들기

1: // [리스트 11.4] 객체의 배열 만들기
2
3: #include <iostreams.h>
4:
5: class CAT
6: 《
7: public:
8:    CAT() { itsAge = 1; itsWeight=5; } // 기본 생성자
ie   “CATC) (30   // 소멸작
10:   int GetAge() const { return itsAge; }
V1   int GetWeight() const { return itsWeight; }
12:   void SetAge(int age) { itsAge = age; }
13:
14: private:
15   int itsAge;
16:   int itsWeight;
Tk 33
18:
19: int main()
20: £
21:   CAT Litter(51;
22:   int 1;
25:   for (i= OF 1< 5) 1++)
24:     LitterLil.SetAge(2*i +1);
25:
26: for (1 = 0; 1 <5; J++)
ar:   i
28:     cout << "cat #" << 7#1<< "2 1
29:     cout << LitterLil.GetAge() << endl;
SO:   a:            Sou 시 애도
3015    return 0; (ter th) ” Sy
328 3
결과 cat #1: 1
cat #2: 3
cat #3: 5
cat #4: 7
cat #5: 9


===== PAGE 346 =====
344 ee 제2주

분석  5-17번 줄에서 CAT SAAS 선언하였습니다. CAT 클래스는 CAT 객체가

^” Was 선언되도록 기본 생성자를 갖습니다. 만일 다른 생성자를 만든다면
컴파일러가 제공하는 기본 생성자가 만들어지지 않으므로 여러분은 여러분 자신
의 것을 만들어야 합니다.
처음의 for 순환문(23-24)에서 각각 5개의 CATS] 나이를 설정하였습니다. 두 번째
의 {@문에서(26-27) 각 배열의 멤버 WS 접근한 뒤 GetAgeOS 호출하였습니다.
각 CATS] GetAge() 메쏘드는 배열 1410601] 다음에 점 연산자(.)를 쓰고 멤버 함수
를 씀으로써 멤버에 접근합니다.

다차원 HH23(Multidimensional Array)
일차원 이상의 배열을 갖는 것이 가능합니다. 각 차원은 배열의 첨자로 표현됩니
다. 따라서 2차원 배열은 2개의 첨자를 갖습니다. 3차원 wae 3개의 첨자를
습니다. 배열은 몇 차원이라도 가질 수 있는데 실제 여러분이 만드는 배열은
개 일차원이거나 이차원입니다.

Zw

이차원 배열의 좋은 예는 AA 판입니다. 한 차원이 8개의 S 다른 차원은 8개의
칸을 대표합니다. [그림 11.3]이 이를 설명합니다.

[그림 11.3] 체스 판과 이차원 배열

SQUAREZHE 이름의 클래스를 가지고 있다고 합시다. 80000라는 이름의 배열은
다음과 같이 됩니다.


===== PAGE 347 =====
제11일 배열 ee 345

SQUARE Board[81[8];

물론 이를 일차원 배열로 해도 됩니다.

SQUARE 800『0ㄷ643;

하지만 이는 현실 세계의 이차원 배열을 정확히 표현시키지 못합니다. 게임이 시

작하면 왕이 첫째 줄 4번째 칸에 위치하게 됩니다. 0부터 시작하면 위치가 다음
과 같습니다.

Board(0J([3];

물론, 첫 번째 첨자가 줄에 해당되고 두 번째 첨자가 칸에 해당된다는 전제하입
니다. 전체 판에서의 위치가 [그림 11.3|에 있습니다.

다차원 배열 초기화

다차원 배열도 초기화할 수 있습니다. 값들의 목록을 각 배열의 윈소에 차례로
저장하면 됩니다. 마지막 첨자항의 원소부터 초기화하다 원소가 다 차면 앞선 원
AS 변화시킨 뒤 또 채워 나갑니다. 만일

int theArray[51[3]

가 있다면 처음 세 개의 원소가 theAmay[oZ 들어갑니다. 다음 세 개의 값이
06408>[1]로 들어가고 계속 그렇게 됩니다.

이를 다음과 같이 초기화할 수도 있습니다.

int theArray[51[3] = { 1, 2, 3/4, 5 6/7; 8, 9/10, 101 , 112, 14, 15
ry;

분별을 쉽게 하기 위해 각 초기화를 중괄호로 집단화시킬 수 있습니다.

int theArray[51(3] = {{ 1, 2, 3},
C4, 5, 00,
{ 7, 8, -9F
{10,1123
£13,145153) 3

컴가일러는 안의 중괄호는 무시합니다. 우리가 볼 때 각 숫자들이 어떻게 배분되
는지를 쉽게 보여주는 셈입니다.

각 값들은 중괄호에 관계없이 AE 분리되어야 합니다. 전체 초기화 집합들은
SBE 안에서 이루어져야 하고 반드시 세미콜론으로 끝나야 합니다.


===== PAGE 348 =====
346 eo 제2주

[리스트 11.5]에서 2차원 배열을 만들었습니다. A 차원은 0부터 4까지의 수의 집
합이고 두 번째 차원은 첫 번째 차원의 값의 두 배입니다.

[리스트 11.5] 다차원 배열 만들기

1: #include <iostream.h>

2: int main()

Si

4    int SomeArrayL[51[2] = { {0,0}, {1,2}, {2,4}, {3,6}, {4,813};
be    for Cint 1 = 0; i<5; i++)

6       for (int j = 0; j<2; jt+)

7       {                                          °

8:        cout << "SomeArrayL" << i << "JE" << j << "J: "7
9:

:        cout << SomeArrayLilLjl<< endl;
10:     }
11:
12:   return 0;
132 3

결과   SomeArrayLOJCOJ:

SomeArrayLOJ(11:
SomeArrayL11LOJ:
SomeArrayL11([1]:
SomeArrayL2JC0l:
SomeArrayL2J([1]:
SomeArrayL31LOJ:
SomeArrayLl3J([11]:
SomeArrayLl41]L01:
SomeArrayLl41([11]:

ORAWRFNN — OO

4번 줄에서 SomeArayS 2차원 배열로 선언하였습니다. 첫 번째 차원은 5개
의 정수로 구성되었습니다. 두 번째 AAS 2개의 정수로 되어 있습니다.
이것은 [그림 11.4에서처럼 5×2의 격자 모양을 만듭니다.

(a
ee

[그림 11.4]                =                         ㄷ
5x2 배열               Cc                           ‘ge

HHS (5) (2)



===== PAGE 349 =====
제11일 배열 ee 347

0. 바깥 0문은 첫 번째 차원을 순환시킴니
.각                  한되면서 내부 10@문은 역시 두 번째 차원을 순후
시킴니다. 이  age  출력 부분에서 증명되는데 9006403710[0| 다음에
900064000101[1이 읍니다. 첫 wal 차원은 두 번째 차원이 차면 중가되고 그러떤
두 번째 차원은 0부터 다시 시작합니다.

a)
빈

yy

[포

x

a

rie,

fo

nN

oO

Hy x2

메모리에 관하여

여러분이 배열을 선언하면, 여러분은 컴파일러에게 어느 정도 크기의 객체를
안에 넣을 것인지를 정확히 일 sh 컴파일러는 그만큼의 메모리를 eee
놓는데 그후 여러분이 그 메모리를 안 써도 마찬가지입니다. 그런데 이 과정은
여러분이 열마큼 크기의 객체를 사용할 것인지를 안다면 사실 문제될 것이 하나

도 없습니다. AS 들어, 체스 판은 60개의 사각이 필요하고 CATE 한 마리에서

gd 마리 사이의 새끼고양이를 ede 등입니다. 그런데 프로그램을 하다보니
여러분이 열마큼 크기의 AAS Baw 하는지 정확히  모른다면 이는 낭패요, 여
러분은 다른 자료 구조를 사용해야 합니다.

이 책에서는 배열에 대한 포인터를 살펴봅니다. 즉, 자유 기억
배열입니다. 그리고 다른 형태도 살펴봅니다. 다른 큰 용량의 기
자료 TEE 이 AS WAS 벗어난 문제입니다. 프로그래머에거
가지 문제는 항상 배울 것이 넘쳐 있다는 것과 항상 읽을 책이 a

다. 경사 났습니다.

 그 2 of
on: !구

fo 호 \ 오
rir 본 0! 기
>     om
mt = [1
& sn cfr er

Te

포입터 HHQa(Array of Pointer)
여태껏 논의된 배열은 그들의 멤버를 스택에 저장합니다. 통상 스택 메모리는 용

량이 작고 자유 기억 BAS 용량이 엄청 Fy. 각 개체는 자유 기억 공간에
저장을 하고 그 포인터를 배열 안의 객체에 저장하는 것이 가능합니다. 이렇게
하면 스택 메모리를 상당히 A + 있습니다. [리스트 11.6|은 [리스트 11.4]의

프로그램을 변형한 것으로 모든 객체를 자유 기억 공간에 저장합니다. 이 프로그
램이 다룰 수 있는 큰 메모리를 말하기 위해 배열이 5에서 500으로 늘어났습
다. 그리고 이름이 110@에서 FamilyS 바뀌었습니다.


===== PAGE 350 =====
348 ee 제2주

[리스트 11.6] 배열을 자유 기억 공간에 저장하기

1: // [리스트 11.63 배열을 자유 기억 공간에 저장하기
Ze
3: #include <iostream.h>
As
5: class CAT
6: {
7: public:
8:    CAT() { itsAge = 1; itsWeight=5; } // 기본 gt
9:    “CATO! (0
10%   int GetAge() const { return itsAge; }
11%   int GetWeight() const { return itsWeight; }
2:   void SetAge(int age) { itsAge = age; }
13:
14: private:
158   int itsAge;
16:   int itsWeight;
178 oe
18:
19: int main)
203 «
21: CAT * Family[5001; & tome Fila   UNE 오조
eck   int 17
aon   CAT * pCat;
24:    for Ci = Os 7 < 5005 144)
in                              ~ Chom 9106
26:       Cat = new CAT;
27:      pCat->SetAge(2*i +1);                Nome = New  cher Uo}
A   ; FamilyCil = pCat;                     Anti rao} heise)
50%                                                   "
31; for (1 = 0; i < 500; i++)                owe Ci emew cher Eve)
S2:   {
335      Gout << “Cat #! << 141 <6 "Ee":
34:      cout << FamilyLiJ->GetAge() << aa  nome
35%   )
56%   return 0;
308 2
24 Dh  Cat #1: 1
Cat #2: 3
Cat #3: 5

Cat #499: 997
Cat #500: 999



===== PAGE 351 =====
제11일 배열 ee 349

분석  CATS] 객체가 5-17번 줄에서 선언되었고 이는 [리스트 11.4]와 동일합니다.
- 이번에는 21번 줄에서 Family 이름으로 배열이 선언되었고 이는 500개의
CAT 객체의 포인터를 저장할 수 있게 되어 있습니다.
초기화하는 순환문에서(24-29번 줄) 500개의 new CAT 객체가 자유 기억 공간 상
에 만들어졌고 각각의 나이는 인덱스의 두 Zo 1을 더한 값으로 설정되었습니
다. 따라서 첫 번째 CATS 1로 설정되고 두 번째 CATS 3, 세 번째 CATS 5로
되었습니다. 마지막으로 포인터가 배열에 저장되었습니다.
배열은 포인터를 가지도록 선언되었기 때문에 - 포인터를 소환한 값이 아니라 -
포인터가 배열에 저장되었습니다.
두 번째 순환문(31-32)은 각 값을 출력합니다. 포인터는 인덱스 Family[i]J= 사용하
여 접근됩니다. 그 주소는 GetAge() 메쏘드에 접근되기 위하여 사용됩니다.
이 예제에서 Family 배열과 그를 가리키는 모든 포인터는 스택에 저장되지만, 500
개의 0&5는 자유 기억 AA 저장됩니다.

자유 기억 공간에 배열 선언하기
전체 MSS 자유 기억 공간에 집어넣을 수 있습니다. 00#라는 예약어를 사용하

고 첨자 연산자를 사용합니다. 결과는 자유 기억 공간의 배열을 가지고 있는 포
인터가 반환됩니다. 예를 들면

CAT * Family = new 647[5003 고

이는 Family7} 500개의 CAT 배열의 첫 번째를 포인터하도록 선언합니다. 다른 말
로 바꾸면 Family 800011이을 포인트 - FAS 갖고 있는 - 한다는 것입니다.

00

이러한 방식으로 Family 사용하면 Family®] 각 ayo] 접근하기 위해 포인터
계산을 할 수 있다는 것입니다. qs 들면

CAT * Family = new 04765003 ;

CAT *pCat = Family;// pCat°| FamilyS 포인트

pCat->SetAge(10);// FamilyLOl$ 10으로
pCattt+;// 『3011>[17로 이동
pCat->SetAge(20);// Familyl1]& 20으로 절정
위의 예제는 500개의 CAT 배열을 news 선언하고 포인터는 배열의 첫 시작 부
포인터 하게 합니다. 그 포인터를 사용하면 처음 CATO] 다음 CATS 가리
있도록 포인터를 증가시킬 수 있고 그후 두 번째 584800가 호출되어 쓰일
>

습니다.

yn eft
xo, 4 "0


===== PAGE 352 =====
350 ee 제2주

배열을 가리키는 포인터와 포인터가 저장된 배열

다음 세 개의 선언을 유심히 살펴봅시다.
objet Dov

14: Cat FamilyOne[500]1;
네가 560 커

2: CAT * FamilyTwol5001];

터를 저장하는 배열입니다. 8001171ㅠ60는 500개의 CAT 배열의 ASS 가리키는
포인터입니다.

이 세 개의 코드의 차이점이 각 배열이 동작하는 것을 서로 다르게 합니다. 놀라
운 것은 FamilyThrees= FamilyOne2] 변종인데 FamilyTwoSh= AK 다르다는 것입
니다.

여기서 포인터는 배열과 어떻게 연관이 되는가 하는 예민한 주제가 하나 발생합
니다. 세 번째에서 FamilyThreet= 배열에 대한 포인터(배열을 가리키는 포인터)입
니다. 다시 말하면 FamilyThreeo] 들어 있는 주소는 그 MS A 항목의 주소와
같습니다. 이는 FamilyOne= 마찬가지입니다.

포인터와 배열명
0++에서 배열 이름은 실제는 그 배열의 A 번째 원소의 상수형 포인터입니다. 따
라서 다음 선언에서
CAT 『801ㄴ/ㄷ5037    Soomiln 논 여러 .

3: CAT * FamilyThree = new 66416ㄷ5003;
FamilyOne*= 500개의 CATS} 배열입니다. FamilyTwo 500742] 0&1에 대한 포인

00001는 &Family[0]¢] 대한 포인터인데 배열 80000의 첫 번째 원소의 주소를 가
아지”

리킴니다.
배열 이름을 상수형 포인터로 쓰는 것은 맞습니다. 그 역도 맞습니다. 따라서
Family + 4는 Family[4]o] 접근하는 올바른 방법 중 하나입니다.

컴파일러는 여러분이 포인터를 추가하고 증가, 감소할 때마다 필요한 계산을 다
해줍니다. Family + 4라고 하면 FamilyS 지나서 4 바이트에 접근한다는 것이 oF
니라 4 개의 객체를 지나서 접근한다는 것입니다. 각 객체가 4 바이트이면 Family
+ 4는 16 바이트입니다. 각 객체가 CATS = 4 바이트를 가진 4 개의 long 멘버
변수와 2 바이트를 가진 2 개의 shot Wry 변수를 각각 가지고 있다면 각 CATE
20 바이트이고 Family 처음 배열을 80 바이트 지나야 합니다.


===== PAGE 353 =====
제11일 배열 ee 351

[리스트 11.7|이 자유 기억 공간에 MAL 선언하고 사용하는 예를 보여줍니다.

[리스트 11.7] newS 사응하여 배열 만들기

1: // CRIAE 11.7] newS 사용하여 배열 만들기

25

3: #include <iostream.h>

6:

5: class CAT

ou ¢

ts public:

8:    CAT() { itsAge = 1; itsWeight=5; } // 기본 생성자
9:    “CATOE                    // 237}

10:   int GetAge() const { return itsAge; }
11:   int GetWeight() const { return itsWeight; }
ze   void SetAge(int age) { itsAge = age; }

14: private:

1291   int itsAge;
16%   int itsWeight;
ifs }s

192 CAT £2 “CATO

20: +

21:   // cout << "Destructor called!\n";
22: }

24: int main()
251

26: CAT * Family = new CATE500]; CATS 것번매는 가려

27:   int i;
28:   CAT * pCat;
29%    for (i = 0; i < 500; i++)

S50:   {

S15      pCat = new CAT;

Se:      pCat->SetAge(2*i +1);

33:      FamilyLil = *pcat; 2h.

34:   >

35:

56:    for (i = 0; i < 500; I++)

Sf:   {)

38:      cout. << "Cat _#" << i+1 << " "3
39:      cout << FamilyLil.GetAge() << endl;
40:   }

41:

42:   delete [] Family;

기
c


===== PAGE 354 =====
352 ee 제2주

43:
44:    return 0;
45: }

결과 Cat #1: 1
Cat #2: 5
Cat #3: 5

Cat #499: 997
Cat #500: 999

불샐 260 SL Family WAS 선언하였는데 이는 500개의 047 개체입니다. 전

제 WAL new 0471500|을 사용하여 자유 기억 공간에 만들어졌습니다. 배

열에 추가되는 각 CAT 객체는 자유 기억 공간에 만들어집니다.31번 줄) 그런데

이번에는 포인터가 배열에 들어가지 않았습니다. 객체 그 자체가 들어갑니다. 이
배열은 포인터의 배열이 아니라 CATS] 배열입니다.

자유 기억 공간의 배열 지우기

Family 자유 기억 공간의 배열을 가리키는 포인터입니다. 33번 줄에서 포인터
pcato] 참조되고 CAT 객체 그 자체가 배열에 대입되었습니다.(배열이 자유 기억
공간에 있으므로 가능합니다.) 그런데 다음 순환에서 pCato] 다시 사용됐습니다.
여기에서 047 객체를 가리키는 포인터는 없어지고 메모리 누출 가능성이 있지
않을까요?

080014를 삭제할 때 할당된 모든 메모리를 삭제하지 않는다면 = 문제가 발생합
니다. 컴파일러는 배열 안의 모든 객체를 지우고 할당된 메모

억 공간으로 되돌려 Baud.
et met

이를 증명해 보기 위해 배열의 크기를 10 정도로 줄여 봅시다(26, 29, 36 줄)
21번 줄의 출력 BRS 주석문으로 막아버립시다. 44번 So] 도달하면 wae 삭
제되고 각 CAT 소멸자가 호출됩니다.

new 사용하여 자유 기억 공간에 항목들을 만들면 여러분은 항상 0000를 사용하

여 그 항목을 삭제해야 합니다. 비 a new <클래스>[크기] 문을 사용하여 배열

을 만들면 단지 0886 | ]를 사용하여 그 배열을 삭제하고 메모리 ARS 해방시킬
수 있습니다. YBSE 컴파일러에게 이 배열이 지워질 것이라고 알립니다.

N



===== PAGE 355 =====
제11일 배열 ee 353

대괄호를 빼버리면 배열의 첫 번째 객체만 지워집니다. 42번 So] 대괄호를 없애
보면 알 수 있습니다. 21번 줄의 소멸자 부분의 출력을 실행시키면 단지 하나의
CAT 객체만 삭제된다는 것을 알 수 있을 것입니다. 이때 메모리 누출이 일어나

00 SR] 배열은 0부터 -!로 번로화된다는 사실을 기억합시다.
DONT 배열을 지나 읽거나 쓰지 eh,

DONT 포인터 배열과 배열을 가리키는 포인터를 론돈하지 gpjcy,
DO 가능라면 HAS 가리키는 포인터로 배열을 사용합시다.

char 배열(문자 배열)
문자열은 문자들의 일련의 나열입니다. 여태껏 여러분이 보아왔던 문자열은 cout
문장 등에서 사용된 이름 없는 문자열입니다.
cout << "hello world.\n" ;
Cro] 문자열은 널 문자로 끝나는 문자의 배열입니다. 다른 배열에서와 같은
방법으로 TASS 선언하고 초기화할 수 있습니다. 예를 들면
char GreetingL[J =
{ oH fel of Fe 대 그 60 ' “i ‘wi, “ot, bls eee "a, 10 버거운
마지막 문자 We 널 문자입니다. 많은 C+ 함수로 하여금 문자열의 끝임을
게 합니다. 비록 이 문자 단위의 작업이 잘 돌아가지만, 입력이 쉽지 않고 오류
발생시킬 확률이 많습니다. 0++은 위 부분의 코드를 간편히 할 수 있는 방법

제공합니다.

char GreetingL] = "Hello World"
이 구문에서 두 가지를 주목해야 합니다.
Be 중괄호에 의해 둘러싸인 MEY 의해 분리되는 홀따옴표가 아니라, 겹따옴표로 싸이고 쉼

Se
도 없고 중괄호도 없이 쓰입니다.

를 널 문자를 끝에 안 넣어줘도 됩니다. 컴파일러가 알아서 해줍니다.

때6 ml ue

변이

Hello \000는 12바이트입니다. Hello7} 5바이트이고 빈 공간이 한 개 있고 World
가 5바이트이며 널 문자가 한 바이트입니다.
로


===== PAGE 356 =====
354 ee 제2주

여러분은 또한 초기화되지 않은 문자 배열을 만들 수 있습니다. 다른 모
과 마찬가지로 미리 있는 메모리 공간보다 더 많은 자료를 넣어서는 안됩

[리스트 11.8]은 초기화하지 않은 버퍼의 사용 예를 보여줍니다.

[리스트 11.8] 배열 채우기

// [리스트 11.83 배열 채우기

#include <iostream.h>

{

1

2

3

4:

5: int main
6

7    char bufferl80];
8

:    cout << "Enter the string: ";
os    cin >> buffer;

10:   cout << "Here's buffer: " << buffer << endl;
1718    return 0;
1235) 5

결과  Enter the string: Hello World

Here's the buffer: Hello

AY 78] 줄에서 버퍼가 80개의 문자를 가질

가의 문자와 한 개의 널문자를 가질 정도로 충분
8번 줄에서 사용자는 문자열을 입력하라는 명령을 받고 이
번 줄에서 버퍼로 저장됩니다. 문자열을 쓴 뒤 널 문자를
cing] 역할입니다.

(a
nas

[JAE 1188|에는 두 가지의 문제가 있습니다. 하나는 사용자가 79개 이상의 문
자를 쓸 경우인데 cine] 버퍼의 BS 지나 입력을 하게 됩니다. 둘재는 사용자가
공백문자를 입력할 경우인데 cine 이를 문자열의 끝으로 생각을 하고 버퍼에 쓰

기를 중지하는 것입니다.
이 문제를 풀기 위해 여러분은 cing] 특별한 머

cin.getQ= 3개의 매개 변수를 가집니다.
myer 할 버퍼

를 입력해야 할 최대 문자 수

mute 중료시키는 $2 둔자,

선언되었습니다. 이는 79
ㅣ 큼

글자가 9

호출해야 합니다.


===== PAGE 357 =====
제11일 배열 ee 355

[리스트 11.9] 배열 채우기

11의가 이 사용법을 보여줍니다.

// 79자리까지 록은 개행 문자까지 얻음

1: // [리스트 11.97 배열 채우기

ze

3: #include <iostream.h>

4:

5: int main()

6: 4%

te    char bufferl80];

8:    cout << "Enter the string: ";
ois    cin.get(buffer, 79);

10%   cout << "Here's buffer: " << buffer << endl;
hte   return 0;

12% 개

겔과 Enter the string: Hello World

Here's the buffer: Hello World

분석  9번 줄에서 cine] 메쏘드 gets

불렀습니다. 7번 줄에 4

선언된 버퍼가 첫 번

째 인자로 전달되었습니다. 두 번째 인자가 입력될 최대 문자수입니다.  이

자를 넣어줄 필요는 없습니다.

우 종료 널 문자를 남기고 79문자입니다. 기본값 개행 문자가 있으므로 종료
}

cin 여러 비슷한 함수들은 스트림에 대해 좀더 깊게 다룬 후 “전처리계”를 다루
°

는 17일째 날에 공부할 것입니다.

strcpy() 2} strncpy()

Cte C 라이브러리 함수들로부터 문자열을

많은 함수들 중 복사를
50009()는

11.10|이 이를 보여줍니다.

[리스트 11.10] strepy() 쓰기

FE 함수들을 이어 받았습니다.

하는 함수가 두 개 있습니다. 5000>0와 5000080입니다.
전체 USS 하나의 문자열로부터 다른

문자열로 복사합니다. [리스트

#include <iostream.h>
#include <string.h>
int main()

{

FWN =


===== PAGE 358 =====
356 ee 제2주

CON WW

Ais
126
105 가

char String1[] = "No man is an island";
char String2(801;

strcpy(String2,String1);
cout << "String1: " << String1 << endl;

cout << "String2: " << String2 << endl;
return 0;

a IE String1: No man is an island
String2: No man is an island

Bay ald 가잎 STRING.H7} 2번 줄에 포함되어 있습니다. 이

파일은 strepy) 함

수의 원형을 보여줍니다. 940090는 두 개의 문자 MAS AY - 복사의
대상처와 근원처입니다. 만일 근원처 문자열이 대상처 문자열보다 더 크다면

strepyO 버퍼의 BS 지나 복사를 하게 될 것입니다.

이를 막기 위해 표준 라이브러리 BE stmepyO= 가지고 있습니다. 이 함수는
이우 에 우우 ie OL ,

복사될 문자의 개수도 가지고 있습니다. 9000000는 처음 널 문자를 만날 때까지

복사하거나 지정된 최대 문자만큼 복사를 합니다.

[리스트 11.11] strncpy) 사용법을 보여줍니다.

1: #include <iostream.h>
2: #include <string.h>
3: int main
ae <
52    const int MaxLength = 80;
6:    char String1L[] = "No man is an island";
Cs    char String2[MaxLengtht+1];
8:
Oe
10%   strncpy(String2,String1 MaxLength) ;
Te
123   cout << "String1: " << String1 << endl;
13%   cout << "String2: " << String2 << endl;
14:   return 0;
156 가
4 1h String1: No man is an island

String2: No man is an island


===== PAGE 359 =====
제11일 배열 ee 357

we Sy 10번 줄에서 strepy07} stmepyS 부르도록 바뀌었습니다. 이 함수는 세 번

째에 인자를 하나 더 받는데 복사할 문자의 최대 개수입니다. 버퍼 String?

는 최대 Maxlength + 1을 취할 수 있도록 되어 있습니다. 1을 더한 이유는 널 문

자를 가지기 위함입니다. 이 a AHS strepyOu} stencpyO7} 문자열 다음에 자동
적으로 붙입니다.

문자열 클래스(9109 Class)

대부분의 CH 컴파일러는 자료 연산을 위한 많은 클래스들
이브러리들을 가지고 있습니다.

CHe UE 끝나는 문자열과 9000`0같은 라이브러리 함수들을 0로부터 물려받았
습니다. 그러나 이러한 함수들은 객체 지향 구조로 통합되지 않았습니다. 문자열
클래스들은 자료들을 연산할 캡슬화된 자료 집합과 함수들을 제공하고 또 문자열
클래스의 클라이언트들로부터 자료들을 은폐하기 위한 접근연산자 함수들을 제공
합니다.

만일, 여러분의 컴파일러가 문자열 클래스를 제공하지 않으면 여러분은 자신의
것을 만들어 써야 합니다. 이번 장의 나머지 부분은 문자열 클래스의 설계와 구
현으로 이루어집니다.

최소한 문자열 Gast 문자 배열의 한계를 극복은 해야 합니다. 모든 배열과
마찬가지로 문자 배열은 정적입니다. 여러분은 그 자료가 얼마나 큰지 설정해야
합니다. 여러분이 프로그램에서 그란큼을 안 쓰더라도 메모리는 차지합니다. 배열
의 BS 지나 사용하는 것은 위험하기 짝이 없습니다.

좋은 문자열 클래스는 필요한 만큼의 메모리를 자기가 할당하고, 정확히 그만큼

을 가지고 있습니다.

[리스트 11.12]가 문자열 클래스의 첫 번째 학습 대상을 제공하여 줍니다.

thlo

포함한 클래스 라

[리스트 11.12] 문자열 클래스 사웅하기

// [리스트 11.127 문자열 클래스 사용하기

#include <iostream.h>        oe ny    제이

#include <string.h>

// 문자열 클래스
class String

NOU RWD =
… er ee … …ㅁ…………



===== PAGE 360 =====
358 ee Hla

3s: <
9: public:
10:  // 생성자 및 소멸자

11:  VStringQ);                                          (  )
12:   Vstring(const char *const);   Stn ing (, OS  veh       sot  ail
13   Jstring(const String &);                          ‘

14:    “String <) ;

153

16:    11-32 연산자

17{    char & operatorLl](unsigned short offset);

18:    char operatorL](unsigned short offset) const;

19:    String operator+(const String&);

20:    void operatort=(const String&);

211    String & operator= (const String &);

eee

23;    // 일민 절근자

24:    unsigned short GetLen()const { return itsLen; }

258    const char * GetString() const { return itsString; }

26%

27: private:

28: “tring (unsigned short); // 전용 Wat
298    char * itsString;

50:    unsigned short itsLen;

S412 oF

S2i

33: // 0바이트의 문자열 생성하는 NE 생성자
34: String::StringQ

555 4

36%   itsString = new charl1];

Ste   itsString[0OJ] = '\0';

38:   itsLen=0;

39: 3}

40:

41: // ip kee ally 생성자

42: // 필요한 만큼의 길이의 문자열을 만드는
43: ,// 클래스 메쏘드에 의해서만 사용됨

44NString::String(unsigned short len? =         AR  ath 2 i

45: ¢                      0           ‘      > waa
46:   itsString = new charLlen+1]; —                      a  2 (08
Ark   for (unsigned short i = 0; i<=len; i++)         seeder i

48:      itsStringli] = '\0';

49:   itsLen=len;                             “

50: +

54

52: // 문자 배열을 문자열로 변환함
53: String::String(const char * const cString)
54: £



===== PAGE 361 =====
제11일 배열

ee 359

55
56:
57%
581
59
60:
6e
62:
63:
64:
65:
66:
67:
68:
69:
70:
71:
(2:
13:
74:
15:
76:
tt:
78:
198
80:
81:
82:
83%
84:
85:
86:
87:
88:
89:
90:
91:
92:
93:
94:
95;
96:
97:
98:
99:

100:
101:

itsLen = strlen(cString);
itsString = new charLitsLen+1];
for (unsigned short i = 0; i<itsLen; i++)
itsStringLil = cStringLil;
itsStringLitsLenJ='\0';
}

// 복사 생성자
String::String (const String & rhs)
{
itsLen=rhs.GetLen();
itsString = new charLitsLen+1];
for (unsigned short i = 0; i<itsLen;it+)
itsStringli] = rhslil;
itsStringLitsLen] = '\0';
3

// SB, 메모리 FET
Stritig: = String ()
£
delete [CJ itsString;
itsLen = 0;
}

// 대입 연산자, 기존 메모리 방출함
// 그리고 문자열과 US 복사
String& String: 10062010「=(00051 String & rhs)
{
if (this == &rhs)
return *this;
delete [4 itsString;
itsLen=rhs.GetLen();
itsString = new charLitsLen+1];
for (unsigned short i = 0; i<itsLen;i++)
itsStringlil = rhslil;
itsStringLitsLen] = '\O';
return *this;

// 비상수 변위 SAP tT
// 문자의 참조작 반환하여
// 나중에 바꿀 수 있게 함
char & String::operatorL](unsigned short offset)
sf

if (offset > itsLen)

return itsStringLlitsLen-1];
else


===== PAGE 362 =====
360 ee 제2주

102:
103:
104:
105:
106:
107:
108:
109:
T10:
171
(12:
1138
114:
TUS
116:
1175
118:
110
120:
T2168
Tee:
Tes:
124:
125:
126:
1274
128:
1298
130:
1513
1328
133:
1368
1356
156%
AST:
138:
1395
140:
141:
142:
143:
144:
145:
146:
147:
148:

return itsStringLoffsetd;
}

// 상수 Wal 사용되는
// 상수 AA 연산작
char String::operatorL](unsigned short offset) const
ne
if (offset > itsLen)
return itsStringLitsLen-1];
else
return itsStringLoffset];
}

// 현재의 문자열에 rhsB 주가하여
// 새로운 문자열을 만들
String String::operator+(const String& rhs)
ti
unsigned short totalLen = itsLen + rhs.GetLen();
String temp(totalLen);
for (unsigned short i = 0; i<itsLen; i++)
tempLil] = itsStringLlil;
for (unsigned short j = 0; j<rhs.GetLenQ); j++, it+)
tempLCil = rhsLljJ;
tempCtotalLenJ='\0';
return temp;
}

// 반환이 없는 현재의 문자열 바꿈

void String::operatort=(const String& rhs)
t
unsigned short rhsLen = rhs.GetLen();
unsigned short totalLen = itsLen + rhsLen;
String temp(totalLen);
for (unsigned short i = 0; i<itsLen; i++)
tempLil] = itsStringlil;
for (unsigned short j = 0; j<rhs.GetLen(Q); j++, it+)
tempLCil = rhsLi-itsLen];
tempCtotalLenJ='\0';
*this = temp;
}
int main()
a8
2
String s1("initial test"); wate Stringed 변랐 NaN.
cout << "S1:\t" << s1.GetString(@ << endl;
char * temp = "Hello World";



===== PAGE 363 =====
제11일 배열 ee 3061

149:   s1 = temp;

150:   cout << "S1:\t" << s1.GetString() << endl;
1512

152°   char tempTwol20];

153%   strcpy(tempTwo,";nice to be here!");

154:   s1 += tempTwo;

155%   cout << "TempTwo:\t" << tempTwo << endl;
156:   cout << "S1:\t" << s1.GetString() << endl;
157:

1506,   cout << "S104]:\t" << 61643 << endl;

159:   Sil4d="x"s

160:   cout << "S1:\t" << s1.GetString() << endl;
161:

162:   cout << "$1[999]:\t" << s1[999] << endl;
163:

164:   String s2(" Another string");

165:   String 's3;

166:   s3 = s1t+s2;

167:   cout << "S3:\t" << s3.GetString() << endl;
168:

169:   String s4;

170:   s4 = "Why does this work?";

A718   cout << "S4:\t" << s4.GetString() << endl;
17028   return 0;

1728 0

결과 ot       initial test

Hello world
TempTwo:   > nice to be here!

Stic         Hello World; nice to be here!

STE4I:     0

S13         Hellx World; nice to be here!

$1£999]:   !

S35:         Hello World; nice to be here! Another string
S4:         Why does this work?

불셀 7- 3! 번 쿨에서 간단한 9078 SAAS 선언하였습니다. 줄 11 - 132 37)
~ 、 의 생성자를 가집니다. 기본 생성자와 복사 생성자, 그리고 0에서와 같이
널로 끝나는 문자열을 가지는 생성자입니다. Sting 클래스는 첨자 연산자(0), 덧

셈 연산자(1), 덧셈 후 대입 연산자=)를 중첩하여 가지고 있습니다. 첨자 연산자

는 두 번 중첩되어 있습니다. 하나는 문자형을 반환하는 상수 함수이고 다른 하

는 문자형의 참조자를 반환하는 비상수형 함수입니다.
오오오 이아 ce re et 으으으 이 오그


===== PAGE 364 =====
362 ee 제2주

비상수형 함수는 다음과 같은 문장에서 쓰입니다.
SomeStringL4] = '\x';

이는 1598 줄에서 보여집니다. 이는 문자열의 A 문자들을 직접 접근하도록 ㅎ

여줍니다. 문자에 대한 참조자가 반환되는데 이는 호출한 함수가 연산을 할

있도록 하여줍니다.

}수형 Sting 객체가 접근될 때 사용되는데 63번 줄의 복사연산자가 구

같은 경우입니다. 058]가 접근됨을 주목합시다. thst const String &로

습니다. 비상수형 멤버 함수를 써서 이 객체에 접근하는 것은 문법에
따라서 참조 연산자는 상수 접근자로 중첨되어야 합니다.

4y 2

oot
rlo
om
+

2

rx (인 0%
r2 nt >
고
ry

ye
에

{A
Go
피>   오
도) 의
aw
avy
x

반환되는 객체가 크다면 여러분은 반환값을 상수형 참조자로 하고 싶을 것입니
다. 여기서는 문자형은 1바이트이므로 그렇게 할 필요는 없습니다.
기본 생성자가 33 - 39번 줄에 구현되어 있습니다. 길이가 od 문자열을 생성합니
다. 이는 String 클래스가 마지막 BS 포함시키지 않은 길이를 나타나게 하는 개
넘을 갖고 있습니다. 기본 문자열은 단지 종료 널 문자만을 가지고 있습니다.

i OT pean 이 이시이 아아아 ON NO Nit Oe

aN, tie

사연산자가 63 - 70번 줄에 구현되어 있습니다. 이는 기존의 존재하는 문자열의
와                        L

이와 같은 문자열을 설정합니다. 단 널 문자를 넣기 위해 하나를 더합니다. 기
존의 문자열을 새로운 문자열로 복사합니다. 그리고 새로운 문자열을 널로 ey
니다.

53 - 60번 줄에서는 C 방식의 문자열을 취하는 생성자를 구현합니다. 이 생성자
는 복사 생성자와 비슷합니다. 이미 존재하는 문자열의 길이는 기존의 표준 라이
브러리 함수 9060()을 호출하여 구합니다.

28번 줄에서 다른 생성자 90108000이 전용 멤버 함수로 선언되었습니다. 이는 이
클래스의 설계자의 의도인데 어떠한 클라이언트 클래스도 임의의 길이의 Strings
만들지 못하게 하려는 의도입니다. 이 생성자는 Strings 내부에서 만들 때 도와
주기 위한 것인데 예를 들면 136번 SoA += 연산자에 의해 요구됩니다. 연산자
+=가 밑부분에서 다루어질 때 잘 설명될 것입니다.

String(unsigned short) 생성자는 그 배열의 각 WAS NULLS 채옵니다. 따라서
for 순환문은 1460 대신 i<-len& 검사하여 봅시다.

73 - 77번 줄의 소멸자는 클래스가 가진 문자열을 삭제합니다. 삭제 연산자를 호
출할 때 대괄호를 포함시키는 것을 잊지 WG. 그래야만 각 배열의 모든 멤버
가 삭제됩니다.


===== PAGE 365 =====
제11일 배열 ee 363

입 연산자는 첫 번째로 오른쪽 항이 왼쪽 항과 같은지를 먼저
면 현재의 문자열은 삭제되고, 새로운 문자열이 만들어지교 대
참조자가 반환되어 다음의 기능이 일어나게 해줍니다.

String1 = String2 = String3 ;

변위 연산자가 두 번 중첩되었습니다. 범위 검사가 동시에 일어납니다. 만일 사용
자가 배열의 SS 지나 접근을 하려면 마지막 문자060 - 1에 있는)가 반환됩니다.

- 127번 줄은 문자 연결 연산자로 덧셈 연산자를 구현하였습니다. 다음과 같
이은   수 있어 편합니다.

String3 = String1 + String2 ;

이는 두 개의 다른 문자열을 연결하여 50003으로 되게 하여줍니다. 이를 만들

위해 덧셈 함수는 두 개의 문자열의 길이를 더하여 임시 문자열 temps 만듭

다. 정수형을 가지는 private 생성자를 부른 뒤 널로 채워진 문자열을 만듭니다.

다음 널들은 두 개의 문자열의 내용으로 채위집니다. 왼편 문자열이 먼저 복사되
(this) 오른쪽 문자열009)이 붙여집니다.

처음의 for 순환문은 왼편의 문자열을 세고 각 BAS 새로운 문자열에 붙입니다.
두 번째 순환문은 오른쪽을 셉니다.

계속 증가하지만 FE ths 문자열을 새로 세어갑니다.
덧셈 연산자는 temp 문자열을 값으로 반환하는데 대입   nae  BHo] 있는

Stringlo] 대입됩니다. += 연산자는 이미 있는 문자열에 동작합니다. suring) +=
String? 문장의 왼쪽 YS 말합니다. 포인터 덧셈 연산자와 비슷하게 작동하는데,
단 하나 140번 줄에 tempzto] 현재의 문자열에 대입된다는 점이 제외됩니다.(*06

= temp)

검사합니다. 다
신 복사됩니다.

om 4 =

v4

Wee SG

녀

143 - 173줄의 main) 함수는 이 SAAS 테스트 프로그램으로 활용됩니다. 145
번 줄에서 널로 끝나는 (와 같은 형태의 생성자를 사용하는 9008 객체를 만듭니
다. 146번 줄은 066902080라는 접근자 PES 사용하여 YRS 출력합니다. 148번
~ 또 다른 C 형태의 문자열을 만듭니다. 149번 Se 대입 연산자를 검사하고
50번 줄에서 결과를 출력합니다.

152번 SS 세 번째의 C 형태의 문자열 16001\0를 만들고 153번 SoA} strepyS
불러 버퍼를 24006 to be 1686!라는 문자들로 채움니다. 154번 SO += 연산자를 호
출하고 기존의 문자열 91에 10001\0를 연결합니다. 156번 줄에서 출력합니다.


===== PAGE 366 =====
364 ee 제2주

158번 줄에서 slo] 있는 4번째의 문자가 접근되었고 출력되었습니다. 159번 줄에
서 새로운 값이 대입되었습니다. 이는 다시 비상수형 변위 연산자([ ])를 호출합니
다. 160번 줄에서 결과를 출력하는데 이는 실제로 we 값을 보여줍니다.

162번 줄은 문자 배열의 끝을 지나 접근하려고 하는데 맨 처음 설계한대로 마지
막 문자열이 반환됩니다.

64 - 165번 줄에서 추가로 두 개의 String AAS 생성합니다. 166번 줄에서 덧셈
연산자를 사용합니다. 167번 줄에서 결과를 출력합니다.

169번 줄은 54라는 새로운 Swing 객체를 만듭니다. 170번 줄에서 대입 연산자를

호출하였습니다. 171번 Se 결과를 출력합니다. 여기서 다음과 같은 의문이 제기
될지도 모른다. “21번 졸에서 분명 대입 연산자는 상수형 Shing 참조자를 AAS
록 정의되었는데 여기서 0 형태의 문자열을 전달받았습니다. 맞는지".

AVS 이렇습니다. 컴파일러는 Strings 기대했는데 문자 HSS 받았습니다. 따
라서 컴파일러는 주어진 Aw Strings 만들 수 YEAS 검사합니다. 12번 |S
에서 여러분은 문자 배열로부터 Stings 생성하는 생성자를 선언하였습니다. 컴
파일러는 문자 배열로부터 임시 90108을 만들고 대입 연산자에 이를 전달합니다.
이를 비명시적 형 변환이라 합니다. 여러분이 문자 배열을 취하는 생성자의 선언
은 하지 않고 구현만 한다면 이 대입식은 컴파일러 오류를 발생시킬 것입니다.

연결 리스트(니060 List)Ot CHE 725 (Structure)

배열은 커다란 컨테이너와 같습니다. Be 용량을 가지지만 그 크기는 고정되어
야 합니다. 여러분이 사용하는 양에 비해 너무나도 큰 컨테이너를 취한다면 여러
분은 용량에 있어 손해를 볼 것입니다. 그 반대로 너무 적은 컨테이너를 취한다
면 내용물이 넘쳐 큰 Seo] 일어날 것입니다.

하는            스트0.0060 1490를 사용하는 것입니다. 연결
조그만 컨테이너들을 필요한 만큼 peu 쓰는 AS 구조입니다, 이
자신의 하나의 객체를 - 예를      , CAT = Rectangle - 보유하
AMS 포인트하는 객체를 만들도록 해줍니다. 여러분 각자가

를 만들고 그들을 하나로 필요한 만큼 묶는 것입니다.

각각의 컨테이너는 노드04006라 불립니다. 연결 리스트에서 첫 번째 노드는 헤더
노드는 테일(180)이라 불립니다.



===== PAGE 367 =====
제11일 배열 ee 365

그

리스트는 3가지의 기본 형태를 가지고 있습니다. 간단한 것부터 복잡한 것으로

나가봅시다.

Met 연결[91791/ linked)

WM 쌍방향 948 (Doubled linked)

BH ==|(Tree)
단 방향 연결 리스트에서 각 노드는 다음 LES 포인트합니다. 그전 BHO 노
드는 포인트하지 않습니다. 특정 노드를 찾기 위하여 여러분은 꼭대기로부터 하
나씩 SES 뒤집니다. 마치 보물찾기와 ASS 노드는 의자 밑에 있다!

=

pA

I>
|o
m
위
rf
바버
au)
|»
10
cr
으
a

로 말입니다.) 쌍 방향             앞뿐만 아니라 뒤에서부터도 찾을
Tl 해줌너다, 블리 ee Le 곡강하 구주입니다, ae 노드는
두 개 아니면 세 개의 방향으로 추적할 수 있습니다. [그림 svt 이 세 가지
연결 리스트를 보여줍니다.

[그림 11.5]                단방향연결

Data                    Data                    Data                    Data
연결 리스트
o—                    o—"                     o—"                     + 0
쌍방향연결
Ss     a
;            Data                    Data                    Data                    Data
o<+—+—-                 는                  Me                  [~ @
o—                       o—                       o—                       .——> ©
Trees
Data
ㆍ     e
Data                             Data
Ze   |  Sy                         .  |  eS
Data            Data            Data            Data

Q
Q

Data

ae]
a<T


===== PAGE 368 =====
* Hoek Cook ( >>
(seek © ) 3

366 ee 제2주

컴퓨터 학자들은 더욱 복잡하고 명료한 자료 구조들을 만들었는데 각각은 노드들
을 연결하는 빵법에 따라 다릅니다. [리스트 11.131은 단순 연결 리스트를 어떻게
만

[리스트 11.13] 연결 리스트를 구현합시다.

// CAE 11.13] 연결 FASS 구련합시다.
//

#include <iostream.h>

// 리스트에 추가되는 객체
class CAT
£
public:
CAT() { itsAge = 1;}
CATCint age): itsAge(age) t}
“CAT O43;
int GetAge() const { return itsAge; }
: private:
int itsAge;

CONDUFWYD

a ee ee ee ee eo}
nDnUPWN | OO

|
|
들고 사용하는지 보여줍니다.
2 가

~ as
600

: // 리스트를 다룸

: class Node

s 1

: public:
Node (CAT*);

“Node(Q);

void SetNext(Node * node) { itsNext = node; }

Node * GetNext() const { return itsNext; }

CAT * GetCat() const { return itsCat; }

void Insert(Node *);

void Display();

: private:

CAT xitsCat;

Node * itsNext;

WWWNYONYNNNNNNNYDY -
mM] 02 6 60 기 AU RFWN — OO

oa

WWW
ui ews

: Node: :Node(CAT* pCat):
itsCat(pCat),
itsNext (0)

WNWWN
CON BO

2 t)

a WN
oO 0

: Node: :~Node()


===== PAGE 369 =====
제11일 배열 ee 367

41:
42:
45:
44:
45%
46:
4(3
48:
49:
DUE
Die
523
aS)
54:
55:
D6:
EY ér
58:
Dos
60:
618
62:
63:
64:
65:
66:
67:
68:
69:
COS
11
28
135
74
(a8
76:
te
(8:
19%
80:
81:
82:
83:
84:
Gon
86:
87:

£
cout << "Deleting node...\n";
delete itsCat;
itsCat = 0;
delete itsNext;
itsNext = 0;

// RRKKKRKKKKE RRA KERRIER 고 KER KR 세 세 세 세 세 세 슈슈 슈 세 기 나
// 삽입
// 나이에 의해 cat& 정렬
// 알고리즘 : 마지막 줄이면 cats 추가
// 아닌 경우 : 새로운 cat] 현재보다
// 나아가 많고 다음보다 어리면 현재 것 뒤에 삽입,
// 아닌 경우 ; 다음 것이 sey 삽입할
[| RRKKEKKKRE KERR EKER KEKE KKK REAR K
void Node::Insert (Node* newNode)
{

if (!itsNext)

itsNext = newNode;

else
{

int NextCatsAge = itsNext->GetCat()->GetAge(); Next, Nede

int NewAge = newNode->GetCat()->GetAge();  Ab]
int ThisNodeAge = itsCat->GetAge();        eo rede
현재 [6006
if ( NewAge > ThisNodeAge && NewAge < NextCatsAge )
{
newNode->SetNext (itsNext);
itsNext = newNode;
}
else
itsNext->Insert (newNode) ;

void Node::Display()
aa
if (itsCat->GetAge() > 0)
{
cout << "My cat is ";
cout << itsCat->GetAge() <<" years old\n";
}
if (itsNext)
itsNext->Display();


===== PAGE 370 =====
368 ee 제2주

88: int main()

89: {

90:

91:   Node *pNode = 0;

92:   CAT * pCat = new CAT(O);
93:   int age;

94:

95:   Node *pHead = new Node(pCat);
96:

97:   while (1)

98:   x.

99:      cout << "New Cat's age? (0 to quit):
100:      cin >> age;

101:      if (lage)

102:        break;

103:     pCat = new CAT(age);
104:     pNode = new Node(pCat);
105:     pHead->Insert (pNode) ;
106: }

107: pHead->Display();

108: delete pHead;

109: cout << "Exiting...\n\n";
110: return 0;

1118 개

New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
New Cat's age? (0 to quit):
My Cat is 1 years old

My Cat is 2 years old

My Cat is 3 years old

My Cat is 5 years old

My Cat is 7 years old

My Cat is 9 years old
Deleting node...

Deleting node...

Deleting node...

Deleting node...

Deleting node...

Deleting node...

Deleting node...
EXating.-..

OMUNN WSO =



===== PAGE 371 =====
제11일 배열 ee 369

분석 7 - 16번 줄에서 간단하게 변형된 CAT 클래스를 선언하였습니다. 기본 생

성자는 멤버 변수 16486를 1로 설정하였고, 또 a 생성자는 정수를 받아
들여 16486를 그 정수값으로 초기화합니다.

- 32번 SE 8006라는 클래스를 선언합니다. Node: 리스트에서 CAT 객체를
—_ 고안되었습니다. 일반적으로 여러분은 NodeS CatList 클래스 안에 은폐할
수 있습니다. 여기서는 은폐하지 않았는데 이는 연결 리스트가 어떻게 동작하는
지 보여주기 위함입니다.
리스트 안에 어떠한 객체도 가질 수 있는 좀더 일반적인 NodeS 만드는 것이 가
능합니다. 14번째 학습 날에 배울 것입니다.
pe 생성자는 CAT AAS 포인트하는 생성자를 가집니다. 복사 생성자와 대입

연산자는 공간을 아끼기 위해 잠시 빼버렸습니다. 실제로는 포함되어야 합니다.

세 개의 접근자 함수가 정의되었습니다. 9604640는 매개 변수로 전달된 Node 이
AS 포인트하는 19%06파라는 멤버 변수를 설정합니다. 06메640와 060(2800는 wl

버 변수들을 반환합니다. 0604640와 0000800는 각각 상수형으로 cee
Node 4S 바꾸지 않기 때문입니다.

Insert()7} 클래스에서 가장 강력한 멤버 함수입니다. 05600는 연결 리스트를 유
하고 NodeS-S 각각의 CATS] 가리키는 Yolo] 근거하여 삽입합니다.
프로그램은 88번 줄부터 시작합니다. 포인터 pNode7} 만들어지고 0으로 초기화되

었습니다. CAT 객체가 만들어지고 나이가 0으로 초기화되었는데 리스트의 헤드

를 가리키는 포인터가 항상 처음에 있도록 확인하려는 것입니다.

번 줄부터 사용자는 나이를 입력시키게 되어 있습니다. 사용자가 0을 입력하면
더 이상 CATS 만들어지지 않는다는 신호가 됩니다. 그 외의 다른 모든 값에 대
해서는 CATS] 103번 줄에서 만들어지게 되어 있습니다. 그리고 15486가 주어진
ULE 설정됩니다. 104번 줄에서 각각의 04에 대해 Node 객체가 만들어집니다.
CAT3} Node7} 만들어진 후 105번 줄에서 리스트의 처음의 Nodet= 새로 생성된
NodeS 입력하도록 되어집니다.

프로그램에서는 어떻게 Node7} 삽입되고 어떻게 리스트가 유지되는지 모릅니다.

전적으로 Node 객체가 알아서 처리합니다.

105600)를 호출하면 프로그램의 실행이 59번으로 넘어갑니다. 항상 Inset
—pHeadS 먼저 호출합니다.

x


===== PAGE 372 =====
370 ee 제2주

59번 줄에서 처음 new Node 추가가 실패하기 때문에 pHeadt= 새로운 NodeS 포
인트하도록 설정됩니다. 출력에서는 16486를 1로 설정된 CATS 가진 노드가 됩
니다.

두 번째의 CAT 객체가 itsAgeS 9로 설정시키며, pHead7} 다시 호출됩니다. 이번
에는 itsNext7} Zo] 아닙니다. 따라서 61 - 74까지의 else 문장이 호출됩니다.

세 개의 지역 변수 - NextCatsAge, NewAge, This NodeAge - 7} 다음의 값들로 채
워집니다.

현재의 Node 나이 - pHead CATS] 나이는 0입니다.
새로운 노드에 의해 보유된 CATS] 나이 - 여기서는 9입니다.
다음 노드에 의해 보유된 CAT 객체의 나이 - 여기서는 1

67번 줄의 WHE 다음과 같이 다시 쓸 수 있습니다.

if ( newNode->GetCat()->GetAge() > itsCat->GetAge() && \\
newNode->GetCat()->GetAge() < itsNext->GetCat()->GetAge() )

이렇게 하면 세 개의 임시변수를 줄일 수 있습니다. 하지만 읽기가 힘들고 혼란
스럽습니다. 대부분의 0++은 이런 프로그램을 버그가 많고 찾기도 힘들기 때문에
싫어합니다.

새로운 CATS] 나이가 현재의 CATS] 나이보다 많고 그리고 다음의 CATS] 나이
보다 적으면 새로운 CATS 나이는 현재의 노드 다음에 넣어집니다. 이 경우 if
문장이 참이 됩니다. 새로운 노드는 현재의 노드가 가리키는 포인트 자리를 갖고
현재의 노드는 새로운 SES 가리키게 됩니다. [그림 WLS 봅시다.

이 검사가 실패하면, 이 자리엔 노드를 집어넣을 적절한 자리가 아닌 셉이 됩니
이때엔 리스트에서 다음 Eo} 대해 105600가 호출됩니다. 지금 106000를 호
출하는 A Insert(\o] 대한 자기 SSO) 끝나지 않는 한 반환되지 않습니다. 따
라서 계속적인 호출이 스택에 쌓이게 됩니다. 만일 리스트가 너무 길어지면 스택
을 날려버리고 프로그램은 파괴됩니다. 이렇게 깊은 스택을 갖지 않도록 하는 방
이 있긴 하지만 이 책의 범위를 벗어납니다.
일단 사용자가 CAT AAS 추가하는 것이 끝나면 처음 노드 pHeadol] 대해
men 호출됩니다. 현재의 노드가 CATS 포인트하면 CATS] 객체의 나이가
력됩니다. 그리고 현재의 노드는 다음 노드를 가리키기 때문에 Display 다음
의 ES 부릅니다.

마지막으로 786800에 대해 delete7} 불려집니다. 소멸자는 다음 노드에 대한 포인
ES 삭제하기 때문에 다음 노드들이 계속 호출됩니다. 전체 리스트가 불려지고

무 -

ㅇ

hag


===== PAGE 373 =====
제11일 배열 ee 371

각 NodeS 줄여가며 160#의 메모리를 방출합니다. 마지막 노드는 멤버
itsNexttS (으로 설정하고 08666가 그 포인터                 에
deleteS 호출하는 것이 가능한데 이는

m                     CAT      |                                   CAT
헤드              |  ^96=0                노드                Age = 1                 ==

노ㄷ  pCAT 7                       pCAT 07                       pCAT 07
pNext e                     > | pNext e                     > | pNext 0          >
Before                                                새로운 노드        CAL
=e                                                          로운 노드         Age =3  |
pCAT 7
pNext e—;————__» 0
CAT
ee                   ㅣ
Age =9
헤드                                                                       06 가 -
호                                                                  pNext e—+—_———_» @
pNext
After

[그림 11.6] 노드 Ay

클래스 배열(사[0+ Class)

여러분 자신의 배열을 사용하는 것이 내장된 배열을 사용하는 것보다 이점이 많
습니다. 처음 AAS 사람들이 배열의 BS 지나 조회하는 것을 막을 수 있습
니다. 또한 여러분의 클래스 배열의 크기를 변동적으로 만들 수 있습니다. a 처

음에는 하나의 WHS 가질 수 있는데 프로그램의 과정중 그
습니다.

정렬할 수 있습니다. 수많은 배열의 변종들이 있는데

oO

i
fo
a
2
S)
a.
fo}
@
(®)
om
@
으
=)
크
42
dz
-포
mn
=
ot
mul
au
&
sed
피>
ale
it

APA (Dictionary) : 한 쌍의 짝으로 구성되는데 하나의 값은 다른 값을 검색하기 위한 키
OLE 쓰임니다.


===== PAGE 374 =====
372

eo 제2주

MAF 배열|60056 array) : 인덱스들이 여러 개의 집합으로 제공됩니다. 하지만 배열에 추
Te 값들만 메모리를 사용하게 되어 있습니다. warns 실제로 SparseArray[5] 또는
SparseArray[200]& 사용할 수 있지만 메모리는 상대적으로 적게 할당됩니다.

BM 모임체|800| : 정렬되지 않아 무작위로 검색되는 집합

2

인덱스 연산자([])를 중첨시킴으로써 연결 리스트를 정렬된 덩어리로 만들 수 있
습니다. ois  것을 배제하면 덩어리를 0 만들 수 있습니다. 리스트의 각
객체들이 짝으로 구성된 값을 가지게 하면 연결 리스트를 사전이나 분산 배열로
만들 수 있습니다.

오늘 여러분은 0+에서 배열을 만드는 YS 배웠습니다. Wee 고정된 길이의,
모든 같은 형을 지닌 객체들의 덩어리입니다.

배열은 끝 검사를 하지 않기 때문에 배열의 BS 지나 읽거나 쓰는 것은 BAB

때로는 일을 저지릅니다. 배열 0부터 시작하는데 흔한 오류는

열에 저장하는 것입니다.

배열은 일차원 또는 다차원으로 될
형을 가지거나 기본 생성자를 가진

수 있습니다. 각각 배열의 멤버들은 내장된
클래스의 객체라면 초기화될 수 있습니다.

배열과 그 내용은 자유 기억 공간 혹은 스택에 aaa 수 있습니다. 자유 기억
공간 상의 WAL 2)-2 deletes 호출할 때 [ ]을 넣는 것을 잊지 Yc.

배열 이름은 배열의 첫 번째 원소에 대한 상수 포인터입니다. 포인터와 배열은
배열의 다음 요수를 찾기 위해 포인터 연산을 합니다

컴파일시 알 수 없는 분량의 덩어리를 다룰 수 있는 연결 리스트를 만들 수 있습
니다. 연결 리스트에서 여러분은 여러 개의 그리고 복잡한 자료 구조를 가질 수
있습니다.

문자열은 문자들의 배열입니다. 0++은 문자 배열을 다루는 여러 도구들을 지원하
는데 배열을 겹따옴표를 사용한 문자열로 초기화할 수 있습니다

Q 24개의 멤버를 가진 배열에 25개의 AAS 집어넣으면 어떤 일이 발생합니까?
A 다른 메모리에 저장하는 셈인데 잠재적으로 프로그램에 재앙을 초래할 것입니다.


===== PAGE 375 =====
제11일 배열 ee 373

Q 초기화되지 않은 배열 원소 안에는 무엇이 있습니까?

A 처음 만들어진 메모리엔 별 것이 다 들어가 있습니다. 새로운 Be 저장하지 않고
이 메모리를 쓰면 알 수 없는 일이 발생합니다.

Q 배열들을 섞어 쓸 수 있습니까?

A 간단한 배열에서 더 사용하여 새로운 큰 배열을 사용할 수 있습니다. 배열
가지고 FARES BAGS 혼합하기 위해 내장된 함수를 쓸 수 있는데 예를 들
streat 9] ch.

Q HWSO] 잘 동작되는데 AW 리스트를 사용하는 이유는?

AWS 고정된 크기를 가져야 합니다. 연결 리스트는 AM) 그 크기를 맘대로 조
정할 수 있습니다.

좀더 좋은 배열 클래스를 사용할 수 있음에도 불구하고 내장된 배열을 써야 하는 이유
대

A 내장된 배열이 사용하기 쉽고 빠릅니다.
Q ENA 클래스는 문자열의 USS 보유하기 위해 char "를 사용해야 합니까?
A 아닙니다. 설계자가 생각하기에 좋은 대로 자유 기억 공간을 쓸 수 있습니다.

을
=]
a

이 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가
를 확인해 보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어
있습니다. 부록 Do] 있는 HS 보기 전에 각 물음에 대답을 할 수 있도록 노력하
고, 다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다

I. SomeArray(25)2| 첫 번째와 마지막 번째의 원소는 무엇입니까?
2 다중 HSS 어떻게 선언합니까?

3% 2번 질문의 다중배열을 초기화하십시오.

4 배열 SomeArray(10) [5)[20)에는 몇 개의 원소가 있습니까?

$. 연결 리스트에 저장할 수 있는 원소의 최대 개수는 몇 개입니까?
수 있습니까?

& 연결 리스트에서 첨자를 쓸
어

7. “Brad is a nice 94?'에서 마지막 문자는 무엇입니까?


===== PAGE 376 =====
374 ee 제2주

연습 문제

1. 세목 놓기(한사람은 동그라미를 다른 사람은 ×표를 그려나가는 오목 비슷한 놀이)
만드는 이차 배열을 선언하십시오.

2 1번에서 만든 배열을 모두 0으로 초기화하는 코드를 작성하십시오.

3. unsigned short 정수형을 갖는 노드의 클래스를 선언하시오.

4 버그잡기

unsigned short SomeArray(51([4];
for (int i = 0; i<4; i++)
for (int j = 0; j<5; j++)
SomeArrayLlilLjJ = itj;
$ㆍ 버그잡기
unsigned short SomeArray(51(4];
for (int i = 0; i<=5; i++)
for (int j = 0; j<=4; j++)
SomeArrayLiJLjJ = 0;

rel
no


===== PAGE 377 =====


===== PAGE 378 =====
376 ee 제주

서

=|
Cc

탐구하고 인식하고 또 각 개념 사이의 관계를 만들어 내는 것이 인간 지능의 기
본적인 한 단면입니다. 우리는 사물의 상호 작용하는 원리를 이해하고 설명하기
위해 AS 구조0160000), 매트릭스008001069), Y]EA (network) 등 여러 개념을 만
듭니다. 0+은 상속의 계충이라는 개념을 사용합니다. 오늘 여러분이 배울 것은
다음과 같습니다.

를 상속이란 무엇인가

wey 하나의 클래스로부터 다른 클래스를 파생해 Were

를 보호 접근자|0:06060 000655란 무엇이며 어떻게 사용하는가

를 가상 tt (virtual 10001071란 무엇인가?

A}z(inheritance)OlEt 무엇인가?

상

vie 도대체 무엇입니까? 여러분이 강아지를 불 때 여러분은 어떠한 관점으로 봅
니까? 생물학자는 상호 작용하는 유기체의 EMS 보고, 물리학자는 원자와 운
동력을 볼 것이며, ean 개 과를 생각할 것입니다.

아마도 우리가 관심을 갖게 되는 것은 마지막 문장일 것입니다. 개는 개 과의 일
종이고 개 과는 포유동물 ie 분류학자는 세상에 살아있는 모든 생명체를 류,
종, 족 등으로 usu

이러한 계층 PAE 소위 한 Sis a’ THE ACE 표현됩니다. WE 개 과의
한 종류(6 OIG. 우리는 이러한 관계를 세상 어디서나 BF 있습니다 도요
타는 차의 한 종류입니다. 차는 운송 기구의 한 종류입니다. 선데(시럽, 과일 등
ge 아이스크림의 일좋)는 후식의 한 종류이고 He 식사의 한 종류입니다. ㆍ

여기서 한 종류(6 get 무엇을 말합니까? 이는 한 분화된 AS 뜻합니다. 자동
차란 운송 기구의 한 분화된 사물을 뜻합니다.

|

i} I}Ad(inheritance and Derivation)

개에 있어서 상속이란 개가 자동적으로 포유류의 모든 SIS 가지는 것을 말합
니다. 개는 포유류이기 때문에 움직이고 공기를 들이마십니다. 모든 포유류는 포
유류의 정의에 의해 움직이고 공기를 들이마십니다. 그런데 We 짓고, 꼬리를 혼


===== PAGE 379 =====
제12일 상속 ee 377

드는 개

넘들을 더하였습니다. 우리는 또 한편 개를 사냥개와 애완견으로 분류합
니다. 애완

eu                         ㅇ      A

견은 또 요크셔와 단디-던마운트 등의 애완견으로 분류합니다.
요크셔는 애완견의 일종이고 따라서 이는 개의 일종이며 따라서 포유류고 동물이
며 결국은 생물의 일종입니다. 이 AS 구조가 [리스트 12.11에 나타나 있습니다.

[그림 12.1]
동물의 계중 구조                              동물

VAN

포유류                                  파충류

2

말                    개

cas

사냥개                                       애완견

21

요크                                 캐런

SES 를래스토무터 가쟁된(6059 다른 SARS 정의하게 함으로써 2)
러한 관계를 표현할 수 있게 합니다. 파생이란 “한 종류”를 뜻합니다. 여러분은
Mammalo]@ 클래스로부터 Doge 클래스를 파생시킬 수 있습니다. 여러분은 개가
움직인다는 내용을 명시적(6000050으로 기술할 필요가 없는데 이는 개가
080000[(포유류)로부터 상속되었기 때문입니다.

새로운 파생(0606) |존의 클래스에 새로운 기능을 추가한 새로운 클래스를 원래 클래스에
용어 서 파생되었다고 합니다. 먼저의 클래스를 베이스 클래스(6696 0656)라고 합니다.

개 클래스가 포유류 클래스로부터 파생되었다면 포유류 클래스는 개 클래스의 베
이스 클래스입니다. 파생된 클래스는 그의 베이스 Saag 하위 ip arta
라고 합니다. 개라는 것은 포유류에 몇몇 기능을 추가한 것이고 개 클래스

유류 클래스에 특정 메쏘드나 자료들을 더한 것입니다.


===== PAGE 380 =====
378 ee 제2주

일반적으로 베이스 클래스는 하나 이상의 파생 클래스를 가지고 있습니다. 개와
|                      모

마찬가지로 고양이가 있고 말이 있는데, 이 모두가 포유류이고

스로부터 파생되었습니

동물의 왕국

파생과 상속에 대한 논의를 좀더 효율적으로 하기 위해 이번 장에서는 동물들을
대표하는 많은 클래스의 관계들에 대해 초점을 맞출 것입니다. 여러분은 어린애
들의 게임 - 동물농장 - 을 설계한다고 생각하면 될 것입니다

2,

c

젠가는 여러분은 동물농장의 BE SESS 만들어 낼 것입니다. 말이 있겠고
, 개, 고양이, 양 등이 있습니다. 여러분들은 이러한 클래스에 대해 메쏘드를 만
어 어린애들이 기대하는 바 대로 행동하게 될 것입니다. 하지만 당분간 여러분
일단 간단한 00파라는 문장으로부터 시작합니다
방법은 이 함수가 호출된다는 것을 보여주기만 하고 나머지 기능은 다음에 완
합니다. 이번 장에서 예제로 주어진 SES 좀더 현실적으로 만들려고 조급해
필요는 없습니다
구문
래스를 선언하면 그 클래스가 “ler 파생했는지를 클래스 이름 * #=
쓰고 파생의 A(public HE 기타 등등)을 쓴 뒤 베이스 클래스명을 쓰면 됩니
다음이 그 예입니다.

lass Dog : public Mammal

파생형에 대해서는 이 장의 마지막에 설명될 것입니다. HES publicKhS 씀시다.

베이스 클래스는 이미 선언되어 있어야 합니다. 그렇지 않으면 컴파일러 오류가
납니다. [리스트 12.1]은 \0000081로부터 파생되는 Dog 클래스를 보여줍니다.

[리스트 12.1] 간단한 상속

에 내 은 에 00

// [리스트 12.13 간단한 상속

#include <iostream.h>
enum BREED { YORKIE, CAIRN, DANDIE, SHETLAND, DOBERMAN, LAB 가오

class Mammal


===== PAGE 381 =====
제12월 상속

ee 379

Th
8:
=

10:
115
122
152
14:
1D:
16:
Vs
18:
19:
20:
215
22:
25%
24:
25:
26:
27:
28:
29:
30:
51:
32:
53:
S45
358
56%
371
38:
39:
40:
41:
42:
43:
44:
455
46:
47:

{

public:

// 생성작 및 소멸자
Mammal();
“Mammal ();

A127}

int GetAge()const;
void SetAge(int);

int GetWeight() const;
void SetWeight(int);

// 다른 메쏘드
void Speak();
void Sleep();

protected:
int itsAge;
int itsWeight;
3;

class Dog : public Mammal
{
public:

// 생성자 및 소멸자
Dog();
“DogQ);

// 접큰작
BREED GetBreed() const;
void SetBreed(BREED);

// 따른 메쏘드
// WagTail();
// BegForFood();

protected:
BREED itsBreed;
3;

이 프로그램은 줄력이 없습니다. 왜냐하면 클래스의 선언
다. 하지만 살펴볼 것은 많습니다.

ㅁ

ㅜ

nu


===== PAGE 382 =====
380 ee 제주

ㆍ 불셀 ㅇ- 278 중에서 Mammalo] 선언되었습니다. 이는 예제인데 Mammals 다른
클래스로부터 파생된 것은 아닙니다. 사실 현실 세계에서는 Mammal 동물

로부터 파생된 것이고 이는 포유류는 동물의 일종이라는 의미입니다. 0++에서는
여러분은 단지 주어진 객체에 대해 일부의 정보만을 표현할 수 있습니다. 현실 세

구조는 쓸만한 자료 들 중 일부만을 표현한 것입니다. 좋은 설계라는 것은 현실을
충실히 반영하는 부분 중 여러분이 BAS 갖는 영역만을 표현하는 것입니다.

AS FAS 어디선가 시작하는 HO] 있어야 합니다. 이 프로그램에서는 포유
에서 시작하였습니다. 이 때문에 좀더 높은 클래스에서 표현되는 변수들은 여
에 나타나 있지 않습니다. 예를 들어, 사실 모든 짐승은 나이를 가지고 있고 중량
을 가지기 때문에 이러한 속성을 가진 동물로부터 파생됩니다. 이 때문에 이 속
성이 포유류 클래스에서 나타납니다.

프로그램을 다루기 쉽고 간단히 하기 위해 단지 여섯 개의 메쏘드만이 Mammal
클래스에 저장되었습니다. 4개의 접근 연산자와 Speak), 910970입니다.

29번 줄에서 보듯이 개 클래스는 포유류 클래스로부터 상속되었습니다. 각 개 객
AE 세 개의 멤버 변수를 가집니다. 16486, itsWeight, 1698[660입니다. 개에 대한
클래스 선언에는 16486와 itsWeight 멤버 변수를 가지지 않습니다. 개 객체는 이
를 포유류 클래스로부터 상속받습니다. 또 복사연산자와 생성자, 소멸자도 상속받

으리라 기대합니다.

2
7
4

ad

*j-2-(private) it (protected)

[리스트 12.1]9] 24, 45번 줄에서 새로운 접근자 예약어 protected7} 도입되었습니
다. 앞에선 클래스 자료는 전용(00\800으로 선언되었습니다. 그러나 전용 멤버는
파생 클래스에서는 유효하지가 않습니다. 물론 여러분은 16486와 19\68를 범
용으로 만들 수 있습니다. 하지만 바람직하지 않습니다. 다른 클래스가 마음대로
접근하는 것이 별로 내키지 않습니다.

여러분이 원하는 것은 이 ARS) 이 클래스로부터 파생된 클래스에만 유효하게
하는 것입니다. 이에 의해 고안된 개념이 BS (protected YT. 보호 자료 멤버
와 함수들은 파생된 클래스에서 유효하지만 다른 클래스에게는 AOE 간주됨
니다.

따라서 세 가지의 접근자 명세서가 있습니다. 범용(00040)과 WS (protected), 전용
(00180)입니다. 만일 함수가 여러분의 클래스의 객체를 가지고 있다면 그 함수는



===== PAGE 383 =====
제12일 상속 ce 381

모든 범용 멤버 자료와 함수들을 접근할 수 있습니다. 멤버 함수는 그 자신의 클
래스의 모든 전용 자료 WMS 함수들을 가질 수 있고 자신을 파생시킨 클래스의
모든 보호 자료 멤버와 함수를 접근할 수 있습니다.

따라서 함수 Dog::WagTail()<- itsBreed 및 Mammal 클래스의 보호 자료를 접근할

수 있습니다.

다른 클래스가 Mammals} Dog 사이에 있을 hole 들어 가축이라는 클래스
8 클래스는 역시 Mammal 클래스의 보호 Ys 접근할 수 있습니다. 물론 이

들 클래스 모두 범용 상속을 하였을 경우를 가정합니다. 전용 상속에 대해서는

15일에 좀더 이야기할 것입니다.

[리스트 12.2]는 어떻게 208형의 객체를 만들고 그 Bo] 자료와 함수를 접근하는

지 보여줍니다.

[리스트 12.2] 파생 AA 사응하기

// [리스트 12.27 파생 객체 사용하기

#include <iostream.h>
enum BREED { YORKIE, CAIRN, DANDIE, SHETLAND, DOBERMAN, LAB };

class Mammal
{
: public:
9:    // 생성자
102   Mammal ():itsAge(2), itsWeight(5){}
V1   “Mammal () {}
12:
13: // 접근자
14:   int GetAge()const { return itsAge; }
155   void SetAge(int age) { itsAge = age; }
16:   int GetWeight() const { return itsWeight; }
1   void SetWeight(int weight) { itsWeight = weight; }
18:
19:   // 다른 메쏘드
20:   void Speak() const { cout << "Mammal sound! \n"; }
21:   void Sleep() const { cout << "shhh. I'm sleeping.\n"; }
22:
23%
24: protected:
2540   int itsAge;
26:   int itsWeight;
ace Fe

1
2
3
Le
5s
6:
7
8


===== PAGE 384 =====
382 ee 제2주

28:

29: class Dog : public Mammal

30: ¢

51: public:

525

53%   // Sagat

34:   Dog():itsBreed(YORKIE) {}

55:   “Dog () {}

36:

37:   // 접근자

38:   BREED GetBreed() const { return itsBreed; }

359:   void SetBreed(BREED breed) { itsBreed = breed; }
40:

41:    // 다른 메쏘드

42:   void WagTail() { cout << "Tail wagging...\n"; }
43:   void BegForFood() { cout << "Begging for food...\n"; }
44:

45: private:

46:   BREED itsBreed;

47s 33

48:

49: int main(Q)

502 ¢

Bile   Dog fido;

D2:   fido.Speak();

53:   fido.WagTail();

54:   cout << "Fido is " << fido.GetAge() << " years old\n";
Do    return 0;

56: 3

렬    Mammal sound!
Tail wagging...
Fido is 2 years old

= 4 6-27번 줄에서 Mammalo] 선언되었습니다.(모든 PSS 공간을 절약하기

위해 10106으로 확장되었습니다. 29 - 47번 줄에서 Dog 클래스가 Mammal

의 파생 클래스로 선언되었습니다. 따라서 이 선언으로 인하여 Doge 나이와 무
A, 종족을 가지게 되었습니다.

51번 줄에서 Dog 800가 선언되었습니다. 800는 140008의 모든 속성을 이어받았

고 208의 속성도 이어받았습니다. 따라서 800는 \381810도 사용할 줄 알지만
Speak(), 916600도 할 줄 압니다.


===== PAGE 385 =====
제12일 상속 ee 383

생성자와 소멸자
0208의 객체는 Mammal} 객체입니다. 이것이 아까 말한 “한 종류"라는 관계의 본
질입니다. 800가 생성되었을 때 그 Mammals 만들 때의 베이스 생성자가 먼저
호출되고 다음에 Dogs] 생성자가 호출되어 Dog 객체의 생성을 마칩니다.
800에게 매개 변수를 안 주었기 때문에 각각 기본 생성자가 호출됩니다. 800는
각각의 생성자가 생기기 전에는 존재하지 않는데 이는      부분과 Dogs] 부
분이 먼저 생성되어야 한다는 것을 뜻합니다. 따라서 각각의 생성자가 호출되어
야 합니다.
fido7} 삭제될 때 먼저 Dog®] 소멸자가 호출되고  음에 100의 Mammal 부분으
소멸자가 호출됩니다. 각각의 소멸자는 800에서의 자신의 BS 제거하게 됩니
다. [리스트 123]9] 예를 보여줍니다.

[리스트 12.3] 생성자와 ABT 호줄

// [리스트 12.37 생성자와 소멸자 호출

#include <iostream.h>
enum BREED { YORKIE, CAIRN, DANDIE, SHETLAND, DOBERMAN, LAB };

class Mammal

{

public:

9:    // 생성자 및 소멸작
10:   Mammal ();

11:   “Mammal ();

1S   // 접근자

14:   int GetAge() const { return itsAge; }

(5%   void SetAge(int age) { itsAge = age; }

16:   int GetWeight() const { return itsWeight; }

17   void SetWeight(int weight) { itsWeight = weight; }

198    //다른 메쏘드
20:   void Speak() const { cout << "Mammal sound! \n"; }
21:   void Sleep() const { cout << "shhh. I'm sleeping.\n"; }

22:

23:

24: protected:
25:   int itsAge;

263   int itsWeight;


===== PAGE 386 =====
384 ee 제2주

Cal he
26:
298
30:
31:
$2:
55:
34:
55:
36:
378
38:
39:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50%
D1:
52
D5
54:
55
56:
57%
58:
59:
60:
61%
625
65:
64:
65:
66:
67:
68:
69:
(05
1?
Tara
(3?

J;

class Dog : public Mammal

£

public:

// 생성자 및 소멸자

Dog();
“Dog();

AY Cua]
BREED GetBreed() const { return itsBreed; }
void SetBreed(BREED breed) { itsBreed = breed; }

// 다른 메쏘드
void WagTail() { cout << "Tail wagging...\n"; }

void BegForFood() { cout << "begging for food...\n";

private:

>;

BREED itsBreed;

Mammal::Mammal():

itsAge(1),
itsWeight (5)
ng
cout << "Mammal constructor...\n";

Mammal ::~Mammal ()

c

cout << "Mammal destructor...\n";

Dog::Dog():

itsBreed(YORKIE)
{

cout << "Dog constructor...\n";
}

Dog::~Dog()

<

}

cout << "Dog destructor...\n";

int main()

{

Dog fido;

}



===== PAGE 387 =====
제12일 상속 ee 385

C4:   fido.Speak();

(5:   fido.WagTail();

163   cout << "Fido is " << fido.GetAge() << " years old\n";
(ae   return 0;

(eo: )

결과   Mammal constructor...

Dog constructor...
Mammal sound!

Tail wagging...

Fido is 1 years old
Dog destructor...
Mammal destructor...

분석  [리스트 12.3]은 [리스트 12.2]와 비슷합니다. 단 생성자와 소멸자가 호출될

때마다 출력합니다. Mammal 생성자가 호출되고 Dogs] 생성자가 불립니다.

이제서야 Dog7} 존재하고 그 메쏘드가 호출될 수 있습니다. 800가 영역을 벗어나
면 008의 소멸자가 호출되고 \14008의 소멸자가 뒤따라 호출됩니다.

베이스 생성자에게 인수 전달하기
1800081의 생성자에게 특정 나이를 지니도록 생성자를 중첩시킬 수 있
리고 208의 생성자에게 종족을 가질 수 있도록 역시 중첩시킬 수 8
Al 나이와 무게 매개 변수를 \00008의 원하는 생성자에게 전달할
만일 Dog 나이를 초기화하고 싶지만 Mammal? 초기화하기 싫을

Pa

[리스트 12.4] 파생 클래스에서 생성자 중첩

// [리스트 12.47 파생 클래스에서 생성자 중첩

#include <iostream.h>
enum BREED { YORKIE, CAIRN, DANDIE, SHETLAND, DOBERMAN, LAB 3};

class Mammal
{

NOU RWD =
… … 00 00 er er re


===== PAGE 388 =====
386 ee R24

8: public:

9:    // 생성자 및 소멸작

10:   Mammal () ;

118   Mammal (int age);

128   “Mammal ();

os

14:   // 접근자

15:   int GetAge() const { return itsAge; }

16:   void SetAge(int age) { itsAge = age; }

Ate   int GetWeight() const { return itsWeight; }

18:   void SetWeight(int weight) { itsWeight = weight; }
19s

20:    // 다른 메쏘드

el:   void Speak() const { cout << "Mammal sound!\n"; }
22:   void Sleep() const { cout << "shhh. I'm sleeping.\n"; }
23:

24:

25: protected:

26:   int itsAge;

er:   int itsWeight;

28: 3;

292

30: class Dog : public Mammal

ale +

32: public:

35%

34:  // 생성자 및 소멸자

555   Dog();

36:   Dog(int age);

St:   Dog(int age, int weight);

58:   Dog(int age, BREED breed);

39:   Dog(int age, int weight, BREED breed);

40:   “Dog;

a Le

42:   // 접근자

43:   BREED GetBreed() const { return itsBreed; }

44:   void SetBreed(BREED breed) { itsBreed = breed; }
45:

46:    // 다른 메쏘드

47:   void WagTail() { cout << "Tail wagging...\n"; }
48:   void BegForFood() { cout << "begging for food...\n"; }
49:

50: private:

513   BREED itsBreed;

522 25

55%

54: Mammal::Mammal():


===== PAGE 389 =====
제12일 상속

ee 387

Do:
56:
50
58:
595
60:
Ole
62:
63:
64:
65:
66:
67:
68:
69:
70:
(1:
2:
(3:
74:
(a:
16:
tC
78:
198
80:
81:
82:
85:
84:
85:
86:
87:
88:
89:
90:
91:
92:
93:
94:
95:
96:
978
98:
99:

100:
101:

itsAge(1),
itsWeight (5)
A
cout << "Mammal constructor...\n";
as

Mammal::Mammal (int age):
itsAge(age),
itsWeight (5)
£
cout << "Mammal (int) constructor...\n";
2

Mammal::~Mammal ()
.

cout << "Mammal destructor...\n";
}

Dog::Dog():
Mammal (),
itsBreed(YORKIE)
1
cout << "Dog constructor...\n";
가

Dog: :Dog(int age):
Mammal (age),
itsBreed(YORKIE)
{
cout << "Dog(int) constructor...\n";
}

Dog::Dog(int age, int weight):
Mammal (age),
itsBreed(YORKIE)
{
itsWeight = weight;
cout << "Dog(int, int) constructor...\n";
3

Dog::Dog(int age, int weight, BREED breed):
Mammal (age),
ItsBreed (breed)
{
itsWeight = weight;

cout << "Dog(int, int, BREED) constructor...\n":

}


===== PAGE 390 =====
388 ee 제2주

102:

103: Dog::Dog(int age, BREED breed):
104:   Mammal (age),

105:   itsBreed(breed)

106:   {

107:      cout << "Dog(int, BREED) constructor...\n";
108:   }

109:

110: Dog::~Dog()

1112 +

1125   cout << "Dog destructor...\n";

11352 3

114: int main(Q)

1158 £

116:   Dog fido;

1178   Dog rover (5);

118:   Dog buster (6,8);

119:   Dog yorkie (3,YORKIE);

120,   Dog dobbie (4,20,008ㄷ때041) ;

121%   fido.Speak();

122:   rover .WagTail();

123:   cout << "Yorkie is " << yorkie.GetAge() << " years old\n";
124:    cout << "Dobbie weighs ";

125   cout << dobbie.GetWeight() << " pounds\n";
126:   return 0;

1272 +

줄력은 각각 분석 과정에서 언급이 쉽도록 번로가 붙여졌습니다.

: Mammal constructor...

: Dog constructor...

: Mammal (int) constructor...

: Dog(int) constructor...

: Mammal (int) constructor...
Dog(int, int) constructor...
Mammal (int) constructor...
Dog(int, BREED) constructor...
9: Mammal (int) constructor...

10: Dog(int, int, BREED) constructor...
11: Mammal sound!

12: Tail wagging...

13: Yorkie is 3 years old

(ust

CONDU FWD


===== PAGE 391 =====
제12일 상속 ee 389

14: Dobbie weighs 20 pounds
15: Dog destructor...
16: Mammal destructor...
17: Dog destructor...
18: Mammal destrustor...
19: Dog destructor...
20: Mammal destrustor...
21: Dog destructor...
22: Mammal destrustor...
23: Dog destructor...
24: Mammal destrustor...

불셀 !리스트 12.41에서 Mammale} 생성자가 11번 줄에서 Mammale] 나이 정수형
^” 을 가지도록 중첩되었습니다. 61 - 66번 줄에서 15486는 생성자에게 전달된
ROLE 초기화되었고 16\619는 5로 초기화되었습니다.

Dog 35 - 39번 줄에서 다섯 개의 생성자로 중첩되었습니다. A wae 기본 생
성자이고 두 번째는 Mammal 생성자와 똑같이 나이를 취합니다. 세 번째는 나이
와 무게를 취하며, 네 번째는 나이와 종족, 다섯 번째는 나이, 무게, 종족을 취합
니다.

74번 ye Dog?| 기본 생성자가 Mammal?] 기본 생성자를 호출함을 주목

엄밀히 말하면 이럴 BLE 없지만 이는 매개 WSS 취하지 않는 베이
를 너트 |킨다는 IES 문서화했다고 보면 됩니다. 베이스 생성자는 어떤
도 호출될 수 있지만 이렇게 하면 여러분의 의도를 분명하게 할 수 있습니다.

수형을 가지는 Dog 생성자의 구현은 80 - 85번 줄에 있습니다. 초기화 단계인
- 82번 줄에서 Doge 매개 WES 사용하여 베이스 클래스를 초기화하고 그
종족을 초기화합니다.

다른 008의 생성자가 87 - 93번 줄에 있습니다. 두 개의 매개 변수를 갖
다. 다시 베이스 클래스를 적절한 생성자를 호출함으로써 초기화하는데  이번
무게를 베이스 클래스의 w= itsWeighto] 저장합니다. 여기서 베이스 클래스
수에게 초기화 WS 줄 수가 없는데 이는 Mammalo] 이 매개 변수를 가지는 생
자를 갖지 않았기 때문입니다. 여러분은 이를 008의_생성자의 몸체에서 해야 합
니다.

나머지 생성자 부분이 어떻게 동작하는지 확인을 합시다. 무엇이 초기화되고 무
엇이 생성자의 본체에서 초기화되는지 살펴봅시다. 출력은 이 분석에서 사용될
수 있도록 번호가 붙여졌습니다. 처음 두 So] 출력은 800의 선언을 기본 생성자
를 사용하여 보여줄 때 나타납니다.

여

로 Jy
ae 땐

생성자
우에

od

81

tA

Zk

a
피

6
ot fh fr 등

|


===== PAGE 392 =====
390 ee 24%

3, 4번 SS rover 것이고, 5, OH SS buster 것입니다. SSE Mammal 생성자는
하나의 정수형을 가지는 생성자이고, Dog 생성자는 두 개의 정수형을 지니는 생

성자입니다,

결국 모든 객체가 만들어지고 사용됐으며 나중에 끝납니다. 각 객체가 삭제될 때
마다, 처음 Dog 소멸자가 호출되고 Mammal 소멸자가 호출됩니다. 전부 다섯 번
입니다.

함수 재생(006『10109 Function)

Dog 객체는 Mammal 클래스 안의 모든 멤버 함수들을 접근할 수 있으며 Dog 클
래스가 추가한 \881310같은 다른 멤버 함수도 접근할 수 있습니다. 또 한편 베이
스 클래스 함수를 재생할 수 있습니다. 함수를 재생한다는 것은 베이스 클래스 함수
의 구현을 파생 클래스에 한다는 것입니다. 파생 클래스의 Aas 만들 때 원했던
함수가 호출됩니다.        pyereidns
새로운 WAS WAx(overriding method) == 클래스가 베이스 클래스의 B
웅어 은 반환형과 원형부(5190846) 가지는 함수를 만들면서 새로운 구련을 할
1    그 메쏘드를 재생한다고 합니다.

(signature)7} 일치해야 합니다. 원형부는 Bre] 반환형을 제외한 함수의 원형을
말하는 데, 즉 매개 변수의 이름과 매개 변수 목록, 그리고 만일 상수형이 쓰였다
면 상수형까지 포함한 것을 말합니다.
새로운 BHsH(signature) 함수의 원령
SO] 합니다. 단 원령부는 반환형을 =

[리스트 12.5]는 Dog 클래스가 100001의 메쏘드 SpeakOS 재생시키면 어떤 일이

발생하는지를 보여줍니다. 공간을 절약하기 위해 접근자 함수들은 이 클래스에서

제외시켰습니다.

[리스트 12.5] 파생 클래스에서 베이스 클래스의 메쏘드를 재생시킬 때

// [리스트 12.57 파생 클래스에서 베이스 클래스의 MES 재생시킬 떼

il

2:

3: #include <iostream.h>

4: enum BREED { YORKIE, CAIRN, DANDIE, SHETLAND, DOBERMAN, LAB +}


===== PAGE 393 =====
제12일 상속

ee 391

CON OW

xo

111
128
13%
14:
1952
16:
17
18:
19%
20:
21%
222
23°
24:
25:
26:
205
28:
29%
30:
ott
52:
233.
54%
55%
56!
Sf:
30:
39:
40:
41:
42:
43:
44:
45%
46:
47:

class Mammal

<

public:
// Oo" 및 스멸자
Mammal() { cout << "Mammal constructor...\n"; }
“Mammal() { cout << "Mammal destructor...\n"; }

// 다른 메쏘드
void Speak()const { cout << "Mammal sound!\n"; }
void Sleep()const { cout << "shhh. I'm sleeping.\n"; }

protected:
int itsAge;
int itsWeight;
3;

class Dog : public Mammal
{
public:

// 생성자 및 소멸자
Dog(){ cout << "Dog constructor...\n"; }
“DogQ{ cout << "Dog destructor...\n"; }

// 다른 메쏘드

void WagTail() { cout << "tail wagging...\n"; }

void BegForFood() { cout << "begging for Toods«=\n" > +
void Speak()const { cout << "Woof!\n"; }

private:
BREED itsBreed;
3;

int main()

af
Mammal bigAnimal;
Dog fido;
bigAnimal.Speak();
fido.Speak();
return 0;



===== PAGE 394 =====
392 ee 제2주

결과    Mammal constructor...

Mammal constructor...
Dog constructor...
Mammal sound!

Woof!

Dog destructor...
Mammal destructor...
Mammal destructor...

분석 34번 줄에서 Dog FAAE Speak) MAES 재생시켰고 506800가 SSS
Wr} Wools 말하도록 하였습니다.

42번 4°] Mammal 객체 bigAnimalo] 생성되었을 때 Mammal 생성자가 호출되어
출력됩니다. 43번 줄의 Dog 객체 800가 만들어질 때 다음 두 줄의 출력이 일어납
니다. 여기서 Mammal 생성자와 Dog 생성자가 호출됩니다.
44번 줄에서 Mammal 객체가 500860를 부르고, 45번 줄에서 ㅁ08가 자신의
9768160)를 부릅니다. 출력을 보면 올바르게 호출되었음을 알 수 있습니다. 마지막
으로 두 개의 객체가 범위를 벗어나고 소멸자가 각각 호출되었습니다.

4 (overloading)=t+ 재생(0610108)
두 개의 말이 비슷하고 hei YS 합니다. ARES 중첩한다면 같은 이름을
가지고 메쏘드를 만든다는 것인데 대신 다른 원형부를 지닙니다. 재생을 한다면
파생 클래스에서 베이스 클래스와 같은 이름, 같은 원형부를 가진 메쏘드를 만든
는 것을 뜻합니다

|

베이스 클래스 메쏘드의 은폐
위의 예제에서 Doge] 클래스 메쏘드 506860는 베이스 클래스의 메쏘드를 은폐합
니다. 이것이 바로 원하는 것이었습니다. 하지만 원하지 않는 결과를 얻을 수도
있습니다. 만일 Mammalo] 메쏘드 Move)S 가지고 이것이 여러 개로 중첩되었을
때, 그리고 Dogo] 그 메쏘드를 재생하였을 때 2008는 Mammal’) 그 이름을 가지
는 모든 중첩된 메쏘드를 은폐할 것입니다.
만일, 540001이 Move()S 세 가지 메쏘드로 중첩하였고 - 매개 변수가 없는 것, 정
수형 매개 변수를 갖는 것, 정수형과 WHS 매개 변수로 갖는 것 - Dog7} Move()
를 매개 변수 없는 것으로 재생하였을 때 Dog AAS 사용하여 나머지 두 개의 메
RES 접근하는 것은 어렵습니다. [리스트 12.6]이 이 문제점을 보여줍니다.


===== PAGE 395 =====
제12일 상속 ee 393

[리스트 12.6] 메쏘드 은페(1009 method)

1: // C2|AE 12.6] 은폐 메쏘드(10109 method)
2

3: #include <iostream.h>

4:

5: class Mammal

6: <¢

7: public:

8:    void Move() const { cout << "Mammal move one step\n"; }
9:    void Move(int distance) const

10:   ne

9 캐틀      cout << "Mammal move ";

128      cout << distance <<"steps.\n";

10   }

14: protected:

128   int itsAge;

16:   int itsWeight;

108 2)

18:

19: class Dog : public Mammal

20: {

21: public:

22: // 함수를 은페한다고 경고 밭을 수도 있습니다.
241   void Move() const { cout << "Dog move 5 steps.\n"; }
24: }

25

26: int main()

Zr t

28:   Mammal bigAnimal;

294   Dog fido;

30:   bigAnimal.Move();

ot   bigAnimal.Move(2);

2328   fido.Move();

53%   // fido.Move(10);

34:   return 0;

55% 3

Mammal move one step
Mammal move 2 steps
Dog move 5 steps

이 클래스들에서 불필요한 RES 자료들은 제거되었습니다. 8, 9번 줄에
서 Mammal 클래스는 중첩된 Move() 메쏘드를 선언하였습니다. 23번 줄에서


===== PAGE 396 =====
394 ee 제2주

Dog: Move 매개 변수 없이 재생시켰습니다. 그리고 30 - 32번 줄에서 호출
되었고 출력이 이 결과들을 반영하였습니다.

33번 SL - 주석화되어 없어졌는데 컴파일러 오류가 발생하기 때문입니다. Dog
클래스가 매개 변수 없는 Move) 함수를 재생하지 않았다면 Dog FASE
Move(int)' 호출할 수 있었지만 한번 재생하면 여러 개의 매개 변수를 갖는 중첩
되었던 함수들을 못쓰게 됩니다. 이는 옛날에 여러분이 배운 생성자 관련된 부분
과 비슷합니다. 여러분이 생성자를 만들면 컴파일러는 더 이상 기본 생성자를 만
들지 않는 것과 비슷하죠(기억이 안 나면 그 부분을 복습해야죠.)

oe

여러분이 베이스 SAAS 재생하려할 때 예약어 0008를 잊은 채 은폐하는 것은
흔한 오류입니다. const 원형부이고 이를 빠뜨리면 원형부가 바뀌고, 재생하는

것이 아니라 은폐하는 결과를 불러일으킴니다.

재생(006[『10109)과 은폐(110410ㅁ9) :
다음 절에서 가상 메쏘드가 서술됩니다. 가상 메쏘드를 재생하면 다형성이 지원됩니다. -
은폐를 하면 다형성이 파괴됩니다. 곧 배울 것입니다.

베이스 메쏘드 호줄
여러분이 베이스 메쏘드를 재생하더라도 메쏘드의 이름을 완전하게 다 써주면 사
용이 가능합니다. 즉, 베이스 이름을 주고 두 개의 콜론을 주고 메쏘드 이름을 주
면 됩니다. 예를 들면, \4800001::540\6()입니다.
[리스트 12.6|의 33번 SS 다음으로 바꾸고 컴파일해서 돌리면 다른 결과가 나
오죠.

328    fido.Mammal::Move(10);

{nu
of
re

이는 Mammal WARES 아주 공공연하게 호출합니다. [리스트 12.7|이 이

[리스트 12.7] 재생된 메쏘드로부터 베이스 메쏘드를 호출하기

1; // [리스트 12.73 재생된 메쏘드로부터 베이스 메쏘드를  호출하기
28
3: #include <iostream.h>
4:
5

: class Mammal


===== PAGE 397 =====
제12일 상속 ee 395

62 £

7: public:

8:    void Move() const { cout << "Mammal move one step\n"; }
0”    void Move(int distance) const
10:   {

Vs     cout << "Mammal move ";
126      cout << distance <<"steps.\n";
Si   Br

14:

15: protected:

16:   int itsAge;

Wee   int itsWeight;

181 +;

19%

20: class Dog : public Mammal

21: ¢

22: public:

23    void Move() const;

24:

258

26:

27: void class Dog :: Move() const
26: £

29%   cout << "In dog move...\n";
SU:   Mammal :: Move(3);

311 +

32

33: int main()

54: ¢

555   Mammal bigAnimal;

562   Dog fido;

sre   bigAnimal .Move(2);

38:   fido.Mammal::Move(6) ;

59?   return 0;

403 2

Mammal move 2 steps.
Mammal move 6 steps.

EBAY 35%) 중에서 Mammal® 객체 bigAnimalo] 만들어지고 36번 줄에서 Dog’
~All 800가 만들어졌습니다. 37번 줄에서 메쏘드가 Mammals] Move)= 호

ny

<< {4

로
다

하였고 이는 정수형을 취합니다.

그래머는 Dog 객체에 대해 4006000를 사용하기를 원했지만 문제가 있었
Dogi= Move) 재생하였지만 중첨하지는

았고 정수형을 취하

re >

것

도버
rir

rlo


===== PAGE 398 =====
396

ee 세2주

들지 않았습니다. 이 HAE 명시적으로 38번 줄에서 베이스 클래스의 메쏘드를
호출, 사용하여 해결하였습니다.

증된 클래스를 파생하여 기능을 확장시켜 봅시다.

21
00 파생 클래스에서 베이스 클래스의 메쏘드를 재생하여 함수의 기능을 변화시
켜 봅시다
DONT #4 원형부를 바꾸어 베이스 클래스 함수를 은페시키지 atl

가상 메쏘드(\|[481| Method)

이번 장에서 Dog 객체는 \080008의 한 종류라는 AS 무척이나 강조ㅎ 하였습니다.
여태껏은 Dog 클래스가 베이스 클래스의 속성(자료)과 기능(메쏘드)을 상속받았다

는 점만을 의미하였습니다. 그런데 C++] “한 종류”라는 것은 더욱 깊고 심오
한 뜻을 가지고 있습니다.

ay ret 원합니다. eas
Mammal* pMammal = new Dog;
가 가능합니다.

이는 새로운 208 객체를
Mammal 가리키는 포인터에 치환합니
4800081의 한 종류이기 때문입니다.

=

힙에 만들고 그 객체의 포인터를 반환하여 이를
좋습니다. 왜냐하면 Dogz

이것이 바로 LBA (polymorphism)2] 본질입니다. 예를 들면 여러분은 아주 여러 다른
창들을 만들 수 있습니다. 예를 들어, 대화용 상자, 위 아래로 움직이는 창, 목록 상자,
기타 SES 만든 뒤 그 각각에 0*@4()라는 메쏘드를 줄 수 있습니다. 창에 대한 포인
터를 만들어, 그 포인터에 대화 상자를 저장할 수도 있고, 아니면 다른 파생된 형을 저
장할 수 있습니다. 여러분은 실행시 포인터가 가리키는 형에 관계없이 drawl) 메쏘드
를 SSE 수 있습니다. 그때마다 해당 창에 부여했던, 의도랬던 정확한 drat 로

출됩니다.


===== PAGE 399 =====
제12일 상속 ee 397

그 다음에 여러분은 이 포인터를 사용하여 Mammals} 어떠한 메쏘드도 호출할
수 있습니다. 여러분이 하고 싶은 것은 2080에서 재생된 메쏘드가 자신의 함수
를 호졸할 수 있도록 하는 것입니다. 가상 함수가 이를 가능케 하여줍니다. [리스
트 12.8|은 이것이 어떻게 동작하고 비가상 함수에서는 어떤 일이 일어나는지 보
여줍니다

[리스트 12.8] 가상 메쏘드 사응하기

// 리스트 12.8] 가상 메쏘드.사용회기

#include <iostream.h>

{
public:
Mammal ():itsAge(1) { cout << "Mammal constructor....\n"7 +

9:    “Mammal() { cout << "Mammal destructor...\n"; }
10:   void Move() const { cout << "Mammal move one step\n"; }
te:   virtual void Speak() const { cout << "Mammal speak! \n"; }
12: protected:
135   int itsAge;

1
Ze
3
4:
5: class Mammal
6:
7
8:

14:

1b 2;

16:

17: class Dog : public Mammal

162 {

19: public:

20:   Dog() { cout << "Dog CONSLMUCTOF ..=\n" 7 >
215   “Dog() { cout << "Dog déstructors;...\n" > }

22:   void WagTail() { cout << "Wagging Tail...\n"; }
23:   void Speak()const { cout << "Woof! \n"; }

24:   void Move()const { cout << "Dog moves 5 steps....\n"; }
28 고

265

27: int main()

28: {

29:

30:   Mammal *pDog = new Dog;

SW   pDog->Move();

325   pDog->Speak();

53:

34:   return Q;

55: 3



===== PAGE 400 =====
398 ee 제2주

re     Mammal constructor...
Dog Constructor...
Mammal move one step
Woof!
Dog destructor...
Mammal destructor...

불셀 el 좋에서 Mammal’ 가상 WE - Speak) - 을 제공하였습니다. 이 클
래스의 설계자는 따라서 이 클래스가 다른 클래스의 베이스 클래스형으로
될 수 있도록 하였습니다. 파생 클래스는 이 함수가 재생되기를 원할 것입니다.
30번 줄에서 Mammalol) 대한 포인터 pDog7} 만들어졌고 여기에 새로운 Dog 객체
의 FAT} 들어갔습니다. Dog Mammalo] 한 종류이기 때문에 이는 맞는 문법입
니다. ceo] 포인터는 Move0S 호출하였습니다. 컴파일러는 pDogo] 단지
Mammal@}= 것을 알기 때문에 \10\60를 찾기 위해 Mammal 뒤집니다.

32번 줄에서 포인터는 다음에 SpeakOS sigue (Spakoe 743171 때문에

이것은 마법에 가깜습니다. SRE ETE Mammal 포인터를 가지고 She 것으로
가리키는 포인터 배열을 가지고 있다면 각각은 Mammal] 부클래스(000069들
포인트할 것이고 여러분은 차례로 원하는 함수를 정확히 호출할 것입니다. [리
ERIS 봅시다. oy ovorriiing  주는 virtue & 선언 .

1 lo fo

[리스트 12.9] 다중 가상 BA(Multiple virtual function) 7t 차례로 호출되는 예

: // 리스트 12.93 다중 가상 SE CMul tiple virtual function) *} 차례로 호출되는 예

#include <iostream.h>

1

2

3

4:

5: class Mammal
6: {

7: public:

8:    Mammal():itsAge(1) { }

Re    “Mammal() { }

10:   virtual void Speak() const { cout << "Mammal speak!\n"; 가
11: protected:

122   int itsAge;

13: 3;

14:

15: class Dog : public Mammal

16: ¢

172 public:

18:   void Speak()const { cout << "Woof!\n"; }


===== PAGE 401 =====
제12일 상속

ee 399

19%
20:
21:
228
23:
24:
232
26:
2:
28:
29:
30:
S1
32:
55:
34:
358
56;
3/7:
38:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
515
523
538
54:
55
56:
até
58:
59:
60:
61:
62:
65:
64:
65:

};

class Cat : public Mammal
인
public:
void Speak()const { cout << "Meow! \n"; }
3;

class Horse : public Mammal
{
public:
void Speak() const { cout << "Winnie!\n"; }
3;

class Pig : public Mammal
t
public:
void Speak()const { cout << "Oink! \n"; }
3;

int main()
{
Mammal* theArray([5];
Mammal* ptr;
int choice;
for Cint i = 0; i<5; i++)

{
cout << "(1)dog (2)cat (3)horse (4)pig: mS
cin >> choice;
switch (choice)
d:
case 1: ptr = new Dog;
break;
case 2: ptr = new Cat;
break;
case 3: ptr = new Horse;
break;
case 4: ptr = new Pig;
break;
default: ptr = new Mammal;
break;
}
theArraylil = ptr;
}

for (1=0;1<5;i++)


===== PAGE 402 =====
400 ee 제2주

66:     theArrayLil->SpeakQ ;
67:   return 0;
68: }

결과  (1)dog (2)031 (3)horse (4)pig:

(1)dog (2)cat (3)horse (4)pig:
(1)dog (2) cat (3)horse (4)pig:
(1)dog (2)cat (3)horse (4)pig:
(1)dog (2) cat (3)horse (4)pig:
Woof!

Meow!

Winnie!

Oink!

Mammal speak!

wu 드 에 002

각 클래스의 간단한 기능만을 보여주기 위해 불필요한 FES 벗겨버린 이
프로그램은 가상 함수의 BIS 보여줍니다. Ul 개의 클래스 Dog, Cat,
Horse, Pig 모두 480008!로부터 파생되었습니다.

00
de

1031 줄에서 Mammal®} SpeakQ7} 가상 함수로 선언되었습니다. 18, 25, 32, 38H
줄에서 4개의 파생 SHAT} Speak] 구현을 재생시켰습니다. 사용자는 어떤 객
AS 만들 것인지 요구하는 프롬프트를 보게 됩니다. 46번 줄과 64번 줄에 거쳐
포인터가 배열에 저장됩니다.

컴파일 시에는 어떤 객체가 만들어질 것인지 알지 Be] 때문에 어떤 Speak()t 불
려질지 모릅니다. ptr= 이  는 실행시 그 범위를 부역받게 됩니다. 이를 동적 바인
EI (dynamic binding) =      H HBEOIE!(pyn-time binding) l2t 하는데 이는 정적 바인딩
(static binding) HE 컴파일 ‘sel #1 (complle-time binding) 2} 반대말입니다,

Fe are as
a
ㅜ

2 다
에

가상 함수는 어떻게 동작하는가?
08 같은 파생 객체가 만들어졌을 때 베이스 클래스에 대한 생성자가 먼저 호출
되고 다음에 파생 클래스에 대한 생성자가 호출됩니다. [그림 12.2]에서 Dog 객체
가 만들어진 후 어떻게 되는지를 보여줍니다. 기억 장소 안에서 객체의 Mammal
부분에 Dog 부분에 연결되어 있습니다.

넌

aK"

“


===== PAGE 403 =====
제12일 상속 co 401
[그림 12.2]
Dog *4AI7t 만들어지   Mammal Part 부분     Mammal
a 나서
Dog Object
Dog

개체에서 가상 함수가 만들어지면 객체는 그 황수를 항상 추적해야 합니다. 많은
컴파일러들은 가상 함수 Blo]! (virtual function table)S 만드는데 °]S v-tableo]z}
합니다. 여기엔 각각의 가상 함수를 저장하는 곳이 있고, 각 파생된 객체는 가상
테이블의 포인터를 유지하는데(이를 vptr 혹은 -0000@라 합니다.) 이는 그 테이

블을 가리키고 있습니다.

각 객체의 \ㅠ은 v-tableS 가리키는데 이는 각각의 가상 함수를 가리킴니다.(함수
에 대한 포인터는 14일 날 배움니다) 008에서 Mammal 부분이 만들어졌을 때
\00은 v-tableS] 원하는 부분을 가리키도록 초기화됩니다. [그림 12.3]입니다.

[그림 12.3]

VPTR =
Mammal] v—table                                      -
6 Move
v

Mammal                        é Speak

Dog 생성자가 호출되었을 때, 그리고 이 객체의 Dog 부분이 추가되었을 때 160
은 Dog 객체의 재생된 가상 함수를(만일 있다면) 가리키도록 조정됩니다. 이는
[그림 12.4]에 나타납니다.

[그림 12.4]

\017506
0009의 v—table

Mammal                       6 Mammal: Move ( )

6 Dog: Speak ( )

Dog



===== PAGE 404 =====
402 ee 제2주

Mammal? 가리키는 포인터가 사용되었을 때 \0은 객체의 실제 Bol 의거하여
원하는 함수를 가리키도록 되어 있습니다. 따라서 506060가 호출되었을 때 원하
는 함수가 불럽니다.

없는 것을 얻을 순 없다

만일, Dog 객체가 Mammalel) 없는 WagTail 메쏘드를 가졌다면 Mammals 가리
키는 포인터가 그 메쏘드를 접근할 수 있도록 할 FE 없습니다.0008를 가리키도
록 형 변환 하기 전엔 말입니다.) \881010은 가상 함수가 아니고, Mammal]
객체가 아니므로 이에 도달할 수 없습니다.

Mammal-& Dog 포인터로 바꿀 수 있는 WHO] 있지만 여러분은 \881810을 호출
하는 더 좋은 방법을 가질 수 있습니다. CHS 명시적인 형 변환의 오류 가능성
이 많아 사실 싫어합니다. 이 주제는 내일 다중 상속이 다루어질 때 깊이 논의될
것입니다. 그리고 20일날 템플릿이 이야기될 때 또 다루어집니다.

또 하나

가상 함수는 단지 포인터와 참조자에만 작용합니다. 객체를 값으로 전달하면 가
상 함수가 호출되게 할 수 없습니다. [리스트 WIS 한번 봅시다.

[리스트 12.10] 2t 전달 방식에서 자료의 분할

// [리스트 12.107 값 전달 방식에서 자료의 분할

#include <iostream.h>

1
2
3
4:
5: enum BOOL { FALSE, TRUE };
6: class Mammal

cs 4

8: public:

9:    Mammal ():itsAge(1) { }

10:   “Mammal() { }

115   virtual void Speak() const { cout << "Mammal speak!\n"; }
12: protected:

138   int itsAge;

143 가;

133

16: class Dog : public Mammal

17: ¢

18: public:


===== PAGE 405 =====
제12일 상속

403

19:
20:
21:
22:
23:
24:
25°
26:
Zr:
28:
29:
50:
S12
$2:
33:
34:
55:
56:
371
58:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
51%
52:
D355
54:
558
56:
aC:
58:
59°
60:
61%
62:
63:
64:

void Speak()const { cout << "Woof!\n"; }
3;

class Cat : public Mammal
{
public:
void Speak()const { cout << "Meow! \n"; }
3;

void ValueFunction (Mammal) ;
void PtrFunction (Mammal*) ;
void RefFunction (Mammal&) ;

00 my WE “a

int main()
{
Mammal* ptr=0;
int choice;
while (1)
{
BOOL fQuit = FALSE;
cout << "(1)dog (2)cat (O)Quit: ";
cin >> choice;
switch (choice)
{
case 0: fQuit = TRUE;
break;
case 1: ptr = new Dog;
break;
case 2: ptr = new Cat;
break;
default: ptr = new Mammal;
break;
}
if (fQuit)
break;
trFunction(@tp) ;
htrunecien @as
ValueFunction(&ptp) ;
}
return 0;
}
fn  ~          5 aN
void ValueFunction Gouna) Samaritan)   ar  객체기
《                       unas} 으으 스가
Mammal Value. Speak ();
}

xe,    wow

ol

we   Ba

~ 1


===== PAGE 406 =====
404 ee 제2주

65: void PtrFunction (Mammal * pMammal)
66: f

67:   pMammal->Speak();

68: }

69:

70: void RefFunction (Mammal & rMammal)
718"                           나

(2:   rMammal .Speak () ;

(32 +

겔과  (1)dog (2)cat (O)Quit: 1

Woof

Woof

Mammal Speak!

(1)dog (2)cat (O)Quit: 2
Meow!

Meow!

Mammal Speak!

(1)dog (2) cat (O)Quit: 0

  6-26번 줄에서 Mammal, Dog, Cat 클래스를 간략히 한 버전이 있습니다. 세
개의 함수가 선언되었습니다. PtrFunction(, RefFunction(), '\81400000000(0입

다. 각각은 Mammal} 포인터, 00000의 참조자, Mammal 객체를 상대적으로 가

집니다. 이 세 개의 함수는 같은 일을 하는데 각각 50600 WES 호출함니다.

(lg
2

프로그램은 사용자에게 Dogs} CaF 선택할 것을 요구하고, 사용자의 선택에 적
절한 형에 대한 포인터를 44 - 49번 줄에서 호출합니다.
태

력에서 사용자는 Dogs 선택하였습니다. Dog 객체가 44번 Fol
간에 만들어집니다. 그리고 각각의 포인터, 참조자, we] 세 개의

포인터와 참조자는 모두 가상 함수를 호출합니다. 그리고 008>500000 멤버 함수
XK

N
—

로 전담됩니다. 함수는 Mammal 객체를 원합니다. 컴파일러
1008의 객체를 Mammal 부분으로 나누어 나갑니다. ©} Mammal 976000가
출되는데 위의 Seo] 사용자 선택 후 셋째 줄에 나타납니다.       :

이 ABS Cat 객체에 대해서도 비슷한 결과를 출력합니다.

『'

rote
‘04
bl
re,
et
als
개
10

[이
lr



===== PAGE 407 =====
제12일 상속 ce 405

가상 ABAL(Virtual Destructor)

파생된 객체에 대한 포인터가 삭제되면 어떤 일이 일어날까요? 소멸자가 가상이 .
면 파생 클래스의 소멸자가 호출됩니다.

파생 클래스의 소멸자는 자동적으로 베이스 클래스의 소멸자를 호출하기 때문에
전 객체는 올바르게 삭제됩니다.

가상 복사 생성자(10481 Copy Constructor)

앞서 말했듯이 생성자는 가상이 될 수 없습니다. 그럼에도 불구하고 여러분의 =
로그램은 이미 만들어진 파생 객체의 복사본을 베이스 객체로 포인터를 사용하여
전달하고픈 때가 있을 수 있습니다. 이 때에는 베이스 클래스에서 Cloned 메쏘드

스는 10060 AES 재생하기 때문에 파생 클래스의 복사본이
트 12.11]을 봅시다.

[리스트 12.11] 가상 복사 생성자

// [리스트 12.117 가상 복사 생성자
#include <iostream.h>

1

2

3

4:

5: class Mammal
6:

』

8

{
public:
Mammal ():itsAge(1) { cout << "Mammal constructor...\n"; }
9:    “Mammal() { cout << "Mammal destructor...\n"; }
10:   Mammal (const Mammal & rhs);
14   virtual void Speak() const { cout << "Mammal speak!\n"; }
12: virtual Mammal* Clone() { return new Mammal(*this); } // 가상 메쏘드

13:   int GetAge()const { return itsAge; }

14: protected:

15:   int itsAge;

16: 3:

173

18: Mammal::Mammal (const Mammal & rhs): itsAge(rhs.GetAge())
19: <

20:   cout << "Mammal Copy Constructor...\n";

212 3

22:


===== PAGE 408 =====
406 ㅇㅇ 제주

23: class Dog : public Mammal

242 ¢

252 public:

26:   Dog() { cout << "Dog constructor...\n"; }
ar:   “~Dog() { cout << "Dog destructor...\n"; }
28:   Dog(const Dog & rhs);

29:   void Speak()const { cout << "Woof!\n"; }
30:   virtual Mammal* Clone() { return new Dog(*this); }
S1¢ 35

52:

33: Dog::Dog(const Dog & rhs):

|
|
34: Mammal (rhs)
|

55: £

36:   cout << "Dog copy constructor...\n";

371 +

38:

39: class Cat : public Mammal

40: {

41: public:                                                     \
42:   Cat() { cout << "Cat constructor...\n"; }                  :
43:   “Cat() { cout << "Cat destructor...\n"; }

44:   Cat (const Cat &);

452   void Speak()const { cout << "Meow!\n"; }
46:   virtual Mammal* Clone() { return new Cat(*this); }
47% FE

48:

49: Catz::Cat(const Cat & rhs):

50: Mammal (rhs)

51: <

526   cout << "Cat copy constructor...\n";

53: J

54:

55: enum ANIMALS { MAMMAL, DOG, CAT};

56: const int NumAnimalTypes = 3;

57: int mainQ

58: 1

59:   Mammal *theArrayCNumAnimalTypesl;

60:   Mammal* ptr;

61:   int choice;

62:   for (int i = 0; i<NumAnimalTypes; i++)
63:   af

64:      cout << "(1)dog (2) cat (3)Mammal: ";
65:      cin >> choice;

66:      switch (choice)

67:     {

68:        case DOG: ptr = new Dog;


===== PAGE 409 =====
제12일 상속 ee 407

69:
702
(ake
728
(3:
74:
75、【
162
Ce
78:
(9
80:
81:
822
83:
84:
85:
86:

break;
case CAT: ptr = new Cat;
break;
default: ptr = new Mammal;
break;
}
theArrayLil = ptr;
}
Mammal *OtherArrayCNumAnimalTypes]J;
for (i=0;1<NumAnimal Types; it+)
{
theArrayLil->Speak();
OtherArraylil] = theArrayLil->Clone();
}
for (i=0;i<NumAnimal Types; i++)
OtherArrayLil->Speak();
return 0;

결과

불섹

1: (1)dog (2)03+ (3)Mammal: 1

2: Mammal CONT UBIO xx
5:3) dog=¢           mre

4: (1)dog (2)cat (3)Mammal: 2

5: Mammal constructor...

6: Ca             ty

7: (1)dog (2)cat_     mal: 3

8: Mammal constructor..\

9: Woof!    et

10: Mammal Copy constructor...
11: Dog copy constructor...
12: Meow!

13: Mammal Copy constructor..
14: Cat copy constructor...
15: Mammal speak!

16: Mammal constructor...

17: Woof!

18: Meow!

19: Mammal speak!

[리스트 1212 앞선 예제와 매우 비슷합니다. 단 Mammal 클래스에
010060이라는 새로운 가상 메쏘드가 추가되었습니다. 이 메쏘드는 복사 생

AAS 호출하여 새로운 Mamma 객체를 가리키는 포인터를 돌려주는데 그 포인
터에는 그 자신(*008)을 const 참조자로 전달합니다.
아래아 ee a 애마


===== PAGE 410 =====
408 ce 제?주

1008와 Cat= 각각 CloneQS 재생하고 각각 ABS 초기화하며 그 자신의 복사본
을 자신의 복사 생성자에 전달합니다. CloneQ7} 가상이므로 81번 줄에 보여지듯
이 가상 복사 생성자를 만듭니다.

프로그램은 사용자에게 개, 고양이, 포유류 중에 하나 선택할 것을 원합니다. 그
들은 62 - 74번 줄에서 만들어집니다. 각각의 포인터가 75번 줄의 배열에 저장이
됩니다.

프로그램이 HSS 따라 반복할 때 각각의 객체는 80, 81번 줄에서 그 자신의
Speak()} Clone) 메쏘드를 차례로 호출합니다. Clone) 호출의 결과는 객체에
대한 복사본의 포인터인데 81번 줄에서 배열에 저장됩니다.

출력의 첫 번째 줄에서 프로그램은 사용자에게 프롬프트를 내고 사용자는 le 입
력하여 AS 선택하였습니다. Mammals} Dogs] 생성자가 호출됩니다. 이는 4 - 8
번 줄에서 고양이와 포유류에게도 반복됩니다.

9번 줄에서 첫 번째 객체 208에 대해 Speak7} 호출됩니다. 가상 Speak) 메쏘드
가 호출되고 “\008"가 출력됩니다. Clone) 함수가 다음에 불리고 이는 역시 가

이므로 208의 Clone()7} 호출되는데 이는 Mammal 생성자와 208의 복사 생성자
부릅니
이런 식으로 고양이(12 - 14)와 포유류(15 - 10)에 대해 반복됩니다. 마지막으로
각 배열이 반복되고 각각의 9060060가 호출됩니다.

때 %&

두

가상 메쏘드를 사용하는 대가
가상 메쏘드의 객체는 vtableS 유지해야 하기 때문에 가상 메쏘드를 가지는 부
담이 있습니다. 파생 클래스를 가지지 않는 아주 작은 클래스라면 가상 메쏘드를
가질 아무 이유가 없습니다.
단 여러분이 어떠한 메쏘드를 가상으로 선언한다면 ㅠ1086에 대해 그만큼의 대
를 지불해야 합니다.(비록 상대적으로 아주 적은 메모리 HHO] 있지만) 이 점
A 여러분은 소멸자도 가상이길 원하고, 더 나아가 다른 모든 메쏘드가 가상이
길 원하는 충동을 느낄 지도 모릅니다. 가상이 아넌 것을 잘 살펴봅시다. 그리고
그들이 왜 가상이 아닌지를 잘 이해해 봅시다.

일
카
에


===== PAGE 411 =====
제12일 상속 ee 409

Q&A

DO     클래스로부터 파생할 때 가상 메쏘드를 사용합시다.
00     여러분의 메쏘드가 가상이면 가상 소멸자를 사용합시다.
DON'T 생성자를 가상으로 하지 맘시다.

오늘 여러분은 By 클래스가 어떻게 베이스 클래스로부터 상속하는지 알아보았
습니다. 이번 장에서 일반적인 범용 상속과 가상 함수를 enim 클래스
는 모든 일반 및 보호 자료와 함수를 베이스 클래스로부터 상속합니다.

보호된 접근 방식은 파생 클래스 모두에게 범용으로 쓰이고 전용은 다른 객체에

게 쓰입니다. 파생 클래스는 그의 베이스 클래스의 전용 자료나 함수를 접근할

생성자는 생성자의 몸체부가 사용되기 전에 초기화될 수 있습니다. 베이스 생성
자가 호출되고 매개 변수가 베이스 클래스에 전달되는 것이 바로 이 때입니다.

베이스 클래스의 함수들은 파생 클래스에서 재생될 수 있습니다. 베이스 클래스
의 함수가 가상이면, 그리고 객체가 포인터나 참조자에 의해 접근된다면 파생 클
래스의 함수가 포인트 된 객체의 형으로 AMA 불려집니다.

베이스 클래스의 메쏘드는 베이스 클래스 이름과 두 개의 콜론 다음에 함수
명시적으로 적어서 부를 수 있습니다. 예를 들어, Dog®] 4807081로부터 상속
다면 Mammal} \8160는 Mammal::Wak0)= 호출될 수 있습니다.

가상 메쏘드의 클래스에서 소멸자는 대부분 항상 가상으로 만들어져야 합니다.
가상 소멸자는 객체의 SY 부분이 포인터 상에 delete 사용할 때 삭제되는
것을 보장합니다. 생성자는 가상이 될 수 없습니다. 가상 복사 생성자는 복사 생
성자를 호출하는 가상 멤버 함수를 만드는 방법에 의해 효율적으로 만들어질 수

니다.

Ba
4

O°:

렀으
tl}

Q 상속되는 멤버와 SHE 차례로 아래 계층으로 전달됩니까? 가령 개는 포유류로부터
상속되고, 포유류는 동물로부터 상속될 때 개는 동물의 함수와 자료를 상속받습니까?


===== PAGE 412 =====
410 ee 제2주

A a. 파생이 계속되면서 파생 클래스는 계속 위 계층들의 함수와 자료 BES 상속
받습니다.

@ 위의 에이서 SRT] SHEL SG Masia 개는 어떤 함수를 가집니까? 원래

수입니까, 재생된 함수입니까?

쇼 개가 포유류를 상속받는다면 포유류가 가진 함수를 갖습니다. 재생 함수를 갖습니다.

Q 파생 클래스는 범용 베이스 함수를 전용으로 만들 수 있습니까?

A 가능합니다. 그리고 이때는 모든 아래 계층에게 전용으로 남습니다.

Q 왜 모든 클래스 함수를 가상으로 만들지 않습니까?

A 가상 함수를 만들면 viableS 만드는 경비가 있습니다. 그 후부터는 경비가 사소하
게 됩니다. 많은 0++ 프로그래머는 함수 하나가 가상이면 다른 것도 가상이어야 한
다고 느낌니다. 다른 프로그래머는 이 점에 반대합니다. 가상이 되려면 그만한 이유
가 있어야 합니다.

Q 50170『410)이라는 함수가 베이스 클래스에서 가상이고 하나의 정수형 또는 두 개의
정수형을 갖도록 중첩되었고, 그리고 파생 클래스에서 하나의 정수형을 갖도록 재생되
었습니다. 파생 객체를 가리키는 포인터가 두 개의 정수형 형태의 합수를 호출하면 oF
떤 것이 호출됩니까?

A 하나의 정수형을 갖는 형태의 재생이 베이스 클래스의 함수를 은폐하기 때문에 컴
파일러 오류가 발생합니다.

연구

이 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가
확인해 보는 퀴즈들과 배운 것을 시험해 볼 수 있는 연습 BASS 구성되어 있
습니다. 부록 Do] 있는 답을 보기 전에 각 물음에 대답을 할 수 있도록 노력하
고, 다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다.

-| of

그
I>

1. v-tableo|2t 무엇입니까?

2 가상 소멸자란 무엇입니까?

3B 가상 생성자의 AAS 어떻게 합니까?
4 가상 복사 생성자는 어떻게 만듭니까?


===== PAGE 413 =====
제12일 상속 ee 411

$. 함수를 재생시킨 베이스 클래스에서 베이스 멤버 함수를 어떻게 호출합니까?

& 함수를 재생시키지 않은 베이스 클래스에서 베이스 멤버 함수를 어떻게 호출합니까?

7. 만일 베이스 클래스가 함수를 가상으로 선언하고 파생 클래스가 그 클래스를 재생할 때
111481이라는 단어를 쓰지 않는다면 다음 계층이 이를 상속할 때 가상이 됩니까?

8. ㅁ0「ㅁㅇ0[60[60라는 예약어는 언제 쓰입니까?

연습 문제

, 정수형 매개 ASS 취하고 4010형을 반환하는 가상 함수를 선언하십시오.

클래스 Squares 선언하는데 『60[80016로부터 파생되게 하십시오.

3. 예제 2에서 Rectangle= 두 개의(길이와 넓이) 매개 변수를 갖고, Square= 길이 하
나만을 매개 변수로 가질 때 5048[6를 위한 생성자 초기화를 보이십시오.

4 위의 Square 클래스를 위한 가상 복사 생성자를 만들어 봅시다.

§. 버그잡기
void SomeFunction (Shape) ;

Shape * pRect = new Rectangle;
SomeFunction(*pRect);

6 버그잡기

class Shape()
a
public:
Shape();
virtual ~Shape();
virtual Shape(const Shape&);
3;


===== PAGE 414 =====
수|어 가는 페이지입니다



===== PAGE 415 =====


===== PAGE 416 =====
414 ee 제2주

서

=

어제 여러분은 어떻게 파생 클래스에서 가상 함수들을 사용하는지 알아보있습니
다. 이것이 Gage] 기본적인 기초입니다. 즉, 원하는 파생 클래스의 개체들을
실행시 베이스 클래스 포인터와 연결하는 능력입니다. 오늘 배울 것은 다음과 같
습니다.

를 다중 상속이란 무엇이고 어떻게 쓰는가

를 가상 상속이란 무엇인가?

추상 자료형이란 무엇인가
를 순수 가상 참수란 무엇인가:

여러분은 동물클래스를 가지고 SRS 하여왔고 SES 조류와 포유류의 두 부류
로 나눌 수 있었습니다. 조류는 멤버 함수로 8ㅁ50를 가집니다. BATE Horses
포함해 여러 종류로 나 수 있습니다. Horse: Whinny()} 0801070라는 멤버 함
수를 가질 수 했습니다

갑자기 여러분은 ?680949(그리스 신화에 나오는 날아다니는 말)라는 객체가 필요
하다는 것을 알게 됐다고 해봅시다. 말과 ZH] 중간입니다. 268854는 000
Whinny(), 080000를 가질 수 있습니다. 단 하나의 상속성만 갖는다면 여러분
곤란해질 것입니다.

여러분은 ?688945를 조류로 취급할 수 있습니다. 그러나 그런 경우엔 Whinny)}
080000를 사용할 수 없습니다. 또 말로 만들 수 있습니다. 이 경우 역시 ㅁ50를

사용할 수 없습니다.

여러분의 A 번째 해결 WAS FlyOS Pegasus 안으로 복사한 뒤 말로부터

Pegasus 까생시키는 것입니다. 이는 80를 두 군데서 갖는다는 단점만

조류와 Pegasus) 그런 대로 쓸만합니다. 그런데 한 쪽의 850를 바꾸면
FOS 바꿔야 합니다. 물론 몇 달      년 후 여러분의 코드를 유지
러 오는 개발자도 그것을 알아야 합니다.

ㄴㄴ               =
또는 몇          들

=

얼마 안 있어 여러분은 곧 또 새로운 문제점을 가지게 됩니다. 여러분이
의 목록과 조류 객체 목록을 가지고 싶습니다. 여러분은 06900 객 aa
록에 등록하고 싶어합니다. 그러나 Pegasus7} 말이라면 여러분은 조류 항
을 수가 없습니다.

제외하
다른 쪽
보수하
말 객체
양쪽 목
목에 넣


===== PAGE 417 =====
제13일 다형성 ee 415

여러분은 한 쌍의 잠재적인 해결 방식을 가지고 있습니다. 말 메쏘드 021000를
Move()= 바꿀 수가 있고 그리고 40060를 여러분의 Pegasus 객체가 ㅁ0를 할
수 있도록 Pegasus 안에 중첩시키면 됩니다. 그리고 MoveQ=S 말 안에 021000를
할 수 있도록 중첩시키면 됩니다. 아마 Pegaus= 짧은 거리는 달리고 먼 거리는
날아야겠다는 판단을 내릴 정도로 현명할 것입니다.

Pegasus: :Move(Llong distance)

sf

if (distance > VeryFar)

fly(distance);

else

gallop(distance) ;
}
그런데 이는 한계가 있습니다. 어떤 SF Pegasus= 짧은 거리를 날고 싶은 때가 있
을 것이고 먼 거리를 한번 달려보고 싶은 때가 있을 것입니다. 여러분의 또 다른
해결 방법은 050를 말에게 가져다 놓는 일일 것입니다. 이는 [리스트 13.1]에 있
는데 여기서의 문제는 대부분의 말은 날 수가 없다는 것이고 따라서 이 방법은
말이 Pegasus7} 아닌 때에는 무용지물이 된다는 것입니다.

oH 뭐 좀 좋은 수 없을까요.

[리스트 13.1] 만일 말이 날 수 있다면.…

1: // [리스트 13.1] 만일 말이 날 수 있다면. . .

28 fy

S$:

4: #include <iostream.h>

De

6: class Horse

fe 4

8: public:

9:    void Gallop(){ cout << "Galloping...\n"; }

10:    virtual void Fly() { cout << "Horses can't fly<\n" =}
112 private:

12:   int itsAge;

153 }』

14:

15: class Pegasus : public Horse

162 £

17: public:

18:   virtual void Fly { cout << "I can fly! I can fly! I can fly! \n"s 3
19% 33

nN
oO


===== PAGE 418 =====
416 ee 제2주

21: const int NumberHorses = 5;
22: int main()
23: {
24:   Horse* RanchENumberHorses];
20%   Horse* pHorse;
26°   int choice;
271   for (int i=0; i<NumberHorses; i++)
28:   {
201      cout << "(1)Horse (2)Pegasus: ";
50:      cin >> choice;
51%      if (choice == 2)
$2        pHorse = new Pegasus;
33:     else
34:        pHorse = new Horse;
55%      RanchLil] = pHorse;
$6   }
Br:   cout << “"\n";
58:   for (i=0; i<NumberHorses; i++)
59:   {
40:     RanchLil->Fly();
41:      delete RanchLil;
42:   uy
43%   return 0;
44: }
(1) Horse (2)Pegasus:

all

(Ad
12

In le
= 0 °°
내 비크

oe
ty

(1
(1
(1
O

)Horse (2)Pegasus:
)Horse (2)Pegasus:
Horse (2)Pegasus:
)Horse (2)Pegasus:

aN = Nh =

Horses can't fly.
I can fly! I can fly! I can fly!
Horses can't fly.
I can fly! I can fly! I can fly!
Horses can't fly.

ㅇ

=

™
|

rr

|

프로그램은 분명 돌기는 돕니다. 단 Horse7} FyOS 가져야 한다는 단점

있습니다. 10번 줄에서 FlyQ7} Horse Al 제공되었습니다. 실제 세계에서
분명 오류 또는 실패작입니다. 18번 줄에서 Pegasus 클래스는 Fly) 메쏘

os

생합니다.

의 Horse 포인터의 WAS, 원하는 050 메쏘드가 실행시 2066와 Pegasus
잘 묶어 호출하였는지 알기 위해 사용되었습니다.


===== PAGE 419 =====
제13일 다형성 ee 417

상승(0060130118 Upward)
이러한 경우 필요로 하는 함수를 하나 상위 클래스 계충으로 상승시키는 것이 일
반적인 해법이 될 수 있습니다. 이때 많은 함수에서 베이스 클래스로 상승되는
발생시킴니다. 이런 경우 베이스 es 일부의 파생 클래스에서 조차
는 것을 모든 함수의 이름 Yoo] 잡아놓는 MAIS 가지고 있습니다. 이것은

Cro] 심각한 경우이고 이런 때 베이스 클래스는 방대하고 따분한 것이 될 것

일반적으로 공통되는 기능은 각 클래스의 상호 교류 과정에 BBS 끼치지 않는
범위 내에서 상위 클래스 계층으로 상승시키기를 원할 것입니다. 다시 말하면 만
일 공통되는 베이스 클래스(예를 들어, 말과 조류는 둘 다 동물이고)를 가지는 두
개의 클래스가 공통되는 기능(예를 들어, 둘 다 먹는다라는 기능)을 가진다면 여
러분은 그 먹는다는 기능을 베이스 클래스로 올려버리고 가상 함수를 만들면 된
다는 것입니다

여러분이 피할 것                                      들

은 단지 몇 개의 파생 클래스에서만 쓰는 접속 부분을(예를
A

=
어, Fyeh= 2S 상승시켜서는 안된다는 것입니다.

형 변환 하향(635008 Down)
일단 어렵더라도 원리를 설명하고 보기를 통해 이야기하겠습니다.
단일 상속을 하는 경    vl 이 문제 HAS 위한 또 하나의 접근 방식은 Ay(
Pegasus 안에 넣어두고, 포인터가 Pegasus 객체를 포인트 할 때마다 불러 사용하
는 것입니다. 이렇게 하려면 여러분은 여러분의 포인터가 실제 어떤 형을 가리키
는지 알게 할 필요가 있습니다. 이를 ㆍ실행시 B 서술000 Time Type
Identification: RTTI)’e} 합니다. #171를 사용하는 것은 최근 0++에 있어 공식적으
로 사용되는 추세입니다.
여러분의 컴파일러가 RIMS 지원하지 않
(enumerated type)-& 반환하는 메쏘드를 oly

RM Nes 여러분의 클래스에 넣을 때 주의합시다. 이 기능을 사용하는 것은 다소
뒤떨어진 설계 중 하나입니다. 가상 함수, 템플릿, 다중 상속을 대신 사용할 수 있습


===== PAGE 420 =====
418 ee 제2주

Ay0S 호출하기 위해 여러분은   peel 형 변환해야 합니다. 4, 포인터가
orseS 가리키지 않고 『680545를     키도록 형 변환해야 합니다. 제 형 변환
3}3#(casting down)°]2} 하는데, Horse 객체를 형 변환해 좀더 파생된 형으로 내려
보내기 때문입니다.

CHe 오늘날 공식적으로 MEL dynamiccat 연산자라는 것을 사용하여 형 변
환_하향을 지원합니다. 여러분의 컴파일러에서는 아직 지원이 안될 수 있으므
컴파일시 오류가 발생하더라도 이런 것이 있구나 하고 지나가면 됩니다.

Horse 같은 베이스 클래스를 가리키는 포인터를 가지고 있고, 이 포인터에
ㅁ688505같은 파생 SAAS 가리키는 포인터를 대입하면 여러분은 Hore 포인터를
다형성 있게 사용할 수 있습니다. 만일 여러분이 ?688505 객체에 도달하고 싶으
wi, Pegasus 포인터를 만든 뒤 dynamic_cast 연산자를 사용하여 형 변환합니다.

실행시 베이스 포인터가 검사됩니다. 변환이 적절하다면 26806 포인터가 사용될
수 있고, 변환이 적절치 않다면 Pegasus AAS 가질 수 없으며 새로운 포인터는
널로 채워집니다. [리스트 13.218 봅시다.

[리스트 13.2] 9 변환

// [리스트 13.2]
// 실행식 dynamic_cast 사용

1
2
3
4: #include <iostream.h>

5: enum TYPE { HORSE, PEGASUS };
6

7

8

class Horse
은
9: public:
10:   void Gallop(){ cout << "Galloping...\n"; }
112
12: private:
132   int itsAge;
145 D3
15%
16: class Pegasus : public Horse
178 <
18: public:
19%
20: virtual void Fly() { cout << "I can fly! I can fly! I can fly!\n"; }
21 2;
22%
23: const int NumberHorses = 5;
24: int main()



===== PAGE 421 =====
제13일 다형성 ee 419

258 £
26:   Horse* RanchCNumberHorses];
ate   Horse* pHorse;

28:   int choice, i;

29:   for (int i=0; i<NumberHorses; i++)
30:   £

318     cout << "(1)Horse (2)Pegasus: ";
52:      cin >> choice;

53:      if (choice == 2)

34:        pHorse = new Pegasus;

So:     else

56:        pHorse = new Horse;

ST:      RanchLil = pHorse;

53:   }

39:   cout << "\n"s

40:   for (i=0; i<NumberHorses; i++)

41:   {

42:      Pegasus *pPeg = dynamic_cast<Pegasus *> (RanchLil);
45%      if (pPeg)

44:         pPeg->Fly();

45:      else

46:         cout << "Just a horse\n";
4a:

48:      delete RanchLil;

49:   +

50:   return 0;

a1 J

결과  (1)Horse (2)Pegasus:

(1)Horse (2)Pegasus:
(1)Horse (2)Pegasus:
(1)Horse (2)Pegasus:
(1)Horse (2)Pegasus:

= nN 2a nw =

Just a horse
I can fly! I can fly! I can fly!
Just a horse
I can fly! I can fly! I can fly!
Just a horse

€  이 방법도 돌기는 돕니다. AyOE 8066 바깥으로 빠져 나왔습니다. 그리고

Horse 객체에서는 불려지지 않습니다. ze] a Pegasus 객체에서 호출될 때
명시적으로 형 변환을 합니다. 24066는 FyOS 가지지 않습니다. 따라서 포인터가
PegasusS 가리키도록 형 변환을 시켜야 합니다.

(a


===== PAGE 422 =====
420 ㅇㅇ 제?주

Pegasus 객체를 형 변환 할 필요를 “Ara 여러분의 설계에 무언가 잘못이 있
는 이야기 입니다 이 프로그램은 분명 가상 함수의 FAAS 손상시키는데, 왜
냐하면 실행시의 Bo] 의존하여 형 변환을 해야 하기 때문입니다.
두 개의 SS (List) 넣기
이 방식에 있어 또 다른 문제는 2688505를 18006형으로 선언했다는 것입니다. 따

라서 PegasusS 800형에 등록시키지 못했습니다. 여러분
는 대가를 치르거나, 포인터를 형 변환 하향했는데 =

은 07(0를 8006에 집어넣
다 만족스런 결과를 못 얻

었습니다.
단일 상속을 하는 경우의 마지막 선택이 있습니다. Fly, Whinny(), Gallop) 모
= Bird, ㅁ016의 공통의 베이스 클래스인 Animale] 넣는 것입니다. A, 말의 ae

을 가지는 대신 하나의 동물이라는 통합된 모양을
적거리는 것이 wast 됐다 하면 무조건 몽땅 아주
입니다.

그와 반대로 메쏘드를 각 필요로 하는
법 말이죠. 이보다 더 ue

수 없습니다.

갖습니다. 이래도 됩니다. 걸리
높은 계충으로 올려보내는 것

객체에 넣을 수 있습니다. 형 변환하는 방

DO     공통 기능 부분을 상속 WSN 윗부분으로 올립시다

DONT 상호 접속 부분을 상속 WS 윗부분으로 올리지 WAT

DO    실행시 객체형에 형 변환 사용을 피합시다. - 가상 메쏘드, 템플릿, 다중 상
a2. BA 다
Aa, =   ㆍ

DON'T 파생 클래스로 형 변환하여 하량시키는 것을 피합시다.

다중 2dss(Multiple Inheritance)

Ol

tolet 합니다. 하나 sa 클래스로부터 파생하기 위해 각 베ㅇ
쉼표로 분리합니다. [리스
하는 예를 보여줍니다. 그 다음 프로그램

(2  *   ofN

|나 이상의 베이스 클래스에서 sy 클래스를 WEE 것이 가능합니다. 이를 다

클래

트 13.31이 et 1810로부터 Pegasus= 파생시켜 al
은 Pegasuss 양쪽 목록에 등록합니다.


===== PAGE 423 =====
제13일 다형성 eo 421

[리스트 13.3] 다중 상속

1: // [리스트 13.37 다중 상속

25 //

3:

4: #include <iostream.h>

Die

6: class Horse

2 £

8: public:

Os    Horse() { cout << "Horse constructor... "; }

10:   virtual ~Horse() { cout << "Horse destructor... ee
11    virtual void Whinny() const { cout << "Whinny!... 트릴 값
12: private:

AS   int itsAge;

148 3:

155

16: class Bird

17: 4%

18: public:

19s   Bird() { cout << "Bird constructor... "; }

20:   virtual ~Bird() { cout << "Bird destructor... Wis 가
21:   virtual void Chirp() const { cout << "Chirp... "; }
222   virtual void Fly() const

25;   {

24:      cout << "I can fly! I can fly! I can fly! ";
25%   }

26: private:

208   int itsWeight;

285 +5

29:

30: class Pegasus : public Horse, public Bird

S12 4

32: public:

35:   void Chirp() const { Whinny(); }

34    Pegasus() { cout << "Pegasus constructor... "; }
55%   “Pegasus() { cout << "Pegasus destructor... "; }
56; 3;

St:

38: const int MagicNumber = 2;

39: int main()

40: {

41:   Horse* Ranch[MagicNumber];

42:   Bird* Aviary[MagicNumber];

43:   Horse * pHorse;

44:   Bird * pBird;


===== PAGE 424 =====
422 ee 제2주
45%   int choice;
46:   for (int i1=0; i<MagicNumber; i++)
47:   {
48:      cout << "\n(1)Horse (2)Pegasus: ";
49:      cin >> choice;                            _1안 wy <i
50:     if (choice == 2)                ote | Vit
51:        pHorse = new Pegasus; Mate
525     else
355        pHorse = new Horse;
D4:      RanchLil = pHorse;
555   }
56:   for (i=0; i<MagicNumber; i++)
56:   {
58:      cout << "\n(1)Bird (2)Pegasus: ";
59:      cin >> choice;
60:      if (choice == 2)
61:        pBird = new Pegasus;
62:      else
63:        pBird = new Bird;
64:      AviaryLil = pBird;
65:   }
66:
67:   cout << "\n";
68:   for (i=0; i<MagicNumber; i++)
69:   {
70:      cout << “\nRanchL”™ << 1 << "J: "|;
rahe     RanchLil->Whinny () ;
irae      delete RanchLil;
(38   }
(4:
(28   for (i=0; i<MagicNumber; i++)
76:   {
(ti      cout << "\nAviaryL" << i << "Ji";
78:     Aviarylil->Chirp(;
(9%     AviaryLil->FlyQ;
80:      delete AviaryLil;
81:   B
82:   return 0;
85: 7}

(1)Horse (2)Pegasus: 1

Horse constructor...

(1)Horse (2)Pegasus: 2

Horse constructor... Bird constructor...Pegasus constructor


===== PAGE 425 =====
제13일 다형성 ee 423

a

ae

(1)Bird (2)Pegasus; 1

Bird constructor...
(1)Bird (2)Pegasus:
Horse constructor...

RanchCOJ: Whinny!...
Ranchl1]: Whinny!...

destructor...

AviarylOJ: Chirp...

destructor...

Aviary[1J]: Whinny!...
Pegasus destructor.
AviaryLOJ: Chirp...

destructor: s:

Aviary([1]: Whinny!...
Pegasus destructor.

6 - 1441 줄에서 Horse
력하고, Whinny)= “Whinny!”Z}_ 단어를

16 - 28번 줄에서 Bird 클래스가 선언되고

개의 메쏘드가 있는데 2070과 850입니다. 각각은 자기를 나타내
합니다. 실제 프로그램에서 이 부분은 예를            3

-Bird destructor.

-Bird destructor..

2
-Bird constructor...

»Pegasus constructor

Horse destructor...
Pegasus destructor..Bird destructor...Horse

I can fly! I can fly! I can fly! Bird
I can fly! I can fly! I can fly!
..Horse destructor...

I can fly! I can fly! I can fly! Bird

I can fly! I can fly! I can fly!
-Horse destructor...

클래스가 선언되었고, 생성자와 소멸자
출력합니다.

생성자와 소멸자가 만들어집니다. 두
렵

rr
et
on
tho
ni

는 문장을 출
들어 스피커를 사용해 소리를 내거나

동화상을 내보낼 수도 있습니다.

마지막으로 30 - 36번 줄에서 Pegasus 클래스가 선언되었습니다. Horse2} 210로부
터 파생되었습니다. Pegasus= Chip0S 재생시켜 \[100)0를 부르는데 이

Whinny()= 8066로부터 상속되었습니다.
TT ~ ~

두 개의 목록이 만들어집니다. 41번 줄에서 HorseS 가리키는 #80애와 42번 줄에
서 BirdS 가리키는 AviaryYUth. 46 - 55번 줄에서 Horses} Pegasus7} Rancho]
저장되고 56 - 6531 줄에서 Bird2} Pegasus= Aviaryol] 저장됩니다.

Bird 포인터와 Horse 포인터 양쪽에 가상 메쏘드를 사용하여 Pegasus7} 올바로 동
작되게 하였습니다. 즉, 78번 줄에서 Aviary 배열의 멤버가 자기가 각각 가리키는
객체의 00070를 호출하였습니다. 800는 이를 가상 메쏘드로 하였고 따라서 각각
원하는 것이 호출됩니다.

매번 Pegasus 객체가 만들어지고, 그 Pegasus©] 810와 Horse 부분이 출력에 나타
납니다. 868854가 삭제될 때 각각의 HorseS} Bird 부분이 삭제되는데 소멸자를 가
상으로 만들어 이런 일이 가능합니다.


===== PAGE 426 =====
424 ee 제2주

하는 베이스 클래스의 이름들을
예제 1

class Pegasus :
예제 2

class Schnoodle :

심표로 분리하여 적습니다.

클래스 이름 뒤에 콜론을

하고, 원

public Horse, public Bird

public Schnauzer, public Poodle

다중 상속 WAS 각 부분들
Pegasus 객체가 메모리에 만들어질
됩니다. [그림 13.1]을 봅시다.

13

}

ge

NI
Le 때 ot slo

oN 오 mith o&

Ss rh

©:

[그림 13.1]
다중 상속을 받은
24H

이야깃거리가 다중 베이스 클래스를 가진 객
같은 이름의 가상 함수나 가상 자료를 가진
받을 때 어떤 일이 일어납니까? 다중 베이스 클래스 생성자는 어떻게 초기화
까? 여러 개의 다중 베이스 클래스가 똑같은 클래스로부터 %
문제가 발생할까요? 다음부터 계속
}속이 이루어지는지 알아볼 것입니다.

때 양쪽 베이스 클래스가 268096를 구성하게

yao] 대해 생김니다. 예를 들면
두 개의 베이스 클래스로부터

속된 것이라면

하여 이 문제를 연구할 것이고 어떻게 다

Horse

Bird

Pegasus

다중 상속된 MAAS 생성자

Pegasus7} 8ㅁ0156와 810로부터 shi

가지는 새섯자를 가지며 Pe
[리스트 13.4]를 봅시다.

고 각각의 베이스 클래스

는 각각의 새성자르 3     Pa



===== PAGE 427 =====
제13일 다형성 ee 425

[리스트 13.4] 다중 생성자

// [리스트 13.47 다중 생성자

//

#include <iostream.h>

typedef int HANDS;

enum COLOR { Red, Green, Blue, Yellow, White, Black, Brown };
enum BOOL { FALSE, TRUE };

CONABDUFW PED =

class Horse

{
: public:
Horse(COLOR color, HANDS height);
virtual ~Horse() { cout << "Horse destructor...\n"; }
virtual void Whinny()const { cout << "Whinny!... sae
virtual HANDS GetHeight() const { return itsHeight; }
virtual COLOR GetColor() const { return TtsColors }
: private:
HANDS itsHeight;
COLOR itsColor;

3 3 RP eS RS mS = S| a= =O
SOON AU RFWNH =| OO

oe

Nm Mw
- =

: Horse::Horse(COLOR color, HANDS height):
itsColor(color),itsHeight (height)
{

6090 60 00
~ WP

cout << "Horse constructor...\n";

6090 mM MY
NOW
Y

: class Bird

s 4

: public:

Bird(COLOR color, BOOL migrates);

virtual “Bird() {cout << "Bird destructor...\n"; }
virtual void Chirp(Q) const { cout << "Chirp... 보가
virtual void Fly()const

ne

NWWNWWWG WG 60 PO
ur 에 2 | 2 OO C

cout << "I can fly! I can fly! I can fly! ";

Ww
^

}
virtual COLOR GetColor()const { return itsColor; }
virtual BOOL GetMigration() const { return itsMigration; }

a WNW WS
Oo Oo oN

: private:

41:   COLOR itsColor;
42:   BOOL itsMigration;
45: 33

44:


===== PAGE 428 =====
426 ee R24

AD:
46:
47:
48:
49:
50:
31:
523
53:
54:
551
56:
Dts
58:
59%
60:
61:
62:
63:
64:
652
66:
67:
68:
69:
70:
rake
2:
(358
Cae
(5s
168
(ts
78:
79:
80:
81:
82:
83:
84:
85:
86:
87:
88:
89:
90:

Bird::Bird(COLOR color, BOOL migrates):
itsColor(color), itsMigration(migrates)
“6
cout << "Bird constructor...\n";

class Pegasus : public Horse, public Bird
본
public:
void Chirp()const { Whinny(); +
Pegasus(COLOR, HANDS, BOOL, long);
“Pegasus() 1 cout << "Pegasus destructor...\n";}
virtual long GetNumberBelievers() const
{
return itsNumberBelievers;

private:
long itsNumberBelievers;
3;

Pegasus: : Pegasus (

COLOR aColor,

HANDS height,

BOOL migrates,

Long NumBeLlieve):
Horse(aColor, height),
Bird(aColor, migrates),
itsNumberBelievers (NumBelieve)
{

cout << "Pegasus constructor...\n";
}

int main®
{
Pegasus *pPeg = new Pegasus(Red, 5, TRUE, 1:0) 주
pPeg->Fly();
pPeg->Whinny();
cout << "\nYour Pegasus is " << pPeg->GetHeightQ;
cout << " hands tall and ";
if (pPeg->GetMigration())
cout << "does migrate.";
else
cout << "does migrate.";
cout << "\nA total of " << pPeg->GetNumberBelievers();
cout << " people believe it exists.\n";



===== PAGE 429 =====
제13일 다형성 ee 427

918   delete pPeg;
92:   return 0;
93:3

24 Dh   Horse constructor.

Bird constructor.

Pegasus comenraier

I can fly! I can fly! I can fly! Whinny

Your Pegasus is 5 hands tall and does migrate.
A total of 10 people believe it exists.
Pegasus destructor...

Bird destructor...

Horse destructor...

(ra

AY 8 - 19번째 줄에서 Howse 클래스가 선언되었습니다. 생성자는 두 개의 매개
변수를 가지는데 5, 6번 줄에서 선언된 나열형을 사용하였습니다. 21 -25번
줄의 생성자에 대한 구현은 각 멤버 변수를 초기화하고 문장을 출력하였습니다.

27 - 43번 줄에서 Bird 클래스가 선언되었고 그 생성자의 구현이 45 - 49번 줄에
걸쳐 있습니다. Bird 클래스는 두 개의 매개 변수를 갖습니다. 재미있게도 10066
생성자는 색깔을 가지고 있으며 800 생성자 또한 깃털 색을 지니고 있습니다.
이는 다음 보기에서 보겠지만 #68854가 AAS 가지도록 할 때 문제를 발생시킴
니다.

Pegasus 클래스 그 자신은 51 - 64번 줄에 선언이 되어 있습니다. 또 그 생성자는
66 - 72번 줄에 있습니다. Pegasus AAS] ASE 세 개의 BAS 가지고 있습
니다. 첫째, Horse 생성자가 색깔과 키를 가지고 초기화되었습니다. 다음 Bird 생
성자가 색깔과 나열형을 가지고 때 마지막으로 Pegasus 멤버 변수
itsNumberBelievers7} 초기화되었습니다. 모든 것이 이루어 진   후 Pegasus 생성자의
몸체가 호출됩니다.

main) 부분에서 Pegasus 포인터가 만들어지고 각 베이스 객체의 함수들을 접근합
니다.

모호성 해결(44060184156 Resolution)
[리스트 13.4]에서 Horse 클래스와 Bird 클래스는 06(00100 메쏘드를 같이 가지고
있습니다. 여러분은 Pegasus 보고 AAS 밝히라고 요구할 때가 있습니다. 이때
문제가 발생합니다. Pegasus 8100와 Horse 양쪽으로부터 상속되었습니다. 둘 다


===== PAGE 430 =====
428 ee 제2주

색깔을 가지고 있습니다. 둘 다 같은 이름과 사용법을 가지고 있습니다. 이때 컴
파일러로서는 소위 모호성(40001840/이라는 것을 가지게 되는데 이는 여러분이
해결해 줘야 합니다.

여러분이 단순히

COLOR currentColor = pPeg->GetColor();

라고 쓴다면 다음과 같은 컴파일러 오류가 납니다.

Member is ambiguous: 'Horse::GetColor' and 'Bird::GetColor'

이런 때 여러분은 명시적으로 여러분이 쓰고자 하는 함수를 지정함으로써 BEY
을 피할 수 있습니다. 봅시다.

COLOR currentColor = pPeg->Horse::GetColor();

아무 때라도 여러분이 어떤 클래스의 Wy 함수(또는 ABS 쓸 것인가를 밝혀
ok 할 때 베이스 클래스 이름을 베이스 클래스의 함수나 자료 앞에 붙임으로써
이를 해결할 수 있습니다.

Pegasus7} 이 함수를 재생한다면 문제는 간단해집니다. 568050의 멤버 함수 안에
쓰면 됩니다.

virtual COLOR GetColor()const { return Horse::itsColor; }

이렇게 하면 Pegasus 클래스의 클라이언트에서 발생하는 문제들을 은폐하고, 어떤
베이스 클래스로부터 색깔을 상속받는지의 문제를 캡슬화시킴니다. 클라이언트들
은 물론 다음과 같이 씀으로써 아직도 자유로이 프로그램을 만들 수 있습니다.

COLOR currentColor = pPeg->Bird::GetColor();

공유된 베이스 Bel A(Shared Base (8159)로부터 상속
Bird} Horse7} 같은 베이스 클래스 - 예를 들어, Animal - 로부터 상속받는다면
어떤 문제가 발생할까요? [그림 13기에서 이를 도식화하였습니다.


===== PAGE 431 =====
제13일 다형성 ee 429

[그림 13.2]
SSA 베이스 클래스

Animal

Horse

Animal

Bird

Pegasus

그림에서는 두 개의 베이스 SHA 있습니다. 같이 공유된 베이스 클래스에서
함수나 자료가 호출될 때 또 모호성(41088400이 발생합니다. 예를 들어, Animal
이 16486를 멤버 변수로 또 0044800를 멤버 함수로 선언할 때, 그리고 여러분이

pPeg->GetAgeS 호출할 때 이는 Horse= 통

요 아니면 800를 통
면서 이 모호성을 극복해 봅시다.

[리스트 13.5] 공통되는 베이스 클래스

해 거쳐온 0666800를 부르는 것인가

통해 AAS 0064860를 호출하는 것입니까? [리스트 13.5]를 보

1: // [리스트 13.5] SESE 베이스 클래스

an //

3: #include <iostream.h>

4:

5: typedef int HANDS;

6: enum COLOR { Red, Green, Blue, Yellow, White, Black, Brown } 5
7: enum BOOL { FALSE, TRUE };

8:

9: class Animal // horseS} bird] 대한 공통 베이스

40: ¢

17: publ ice:

12:   Animal (int);

13%   virtual ~Animal() { cout << "Animal destructor...\n"; }
14:   virtual int GetAge() const { return itsAge; }

15%   virtual void SetAge(int age) { itsAge = age; }

16: private:

17:   int itsAge;

182 He


===== PAGE 432 =====
430 ee 제2주

19:
20: Animal::Animal(int age):
21:   itsAge (age)

22:   {

25:      cout << "Animal constructor...\n";
24:   +

258

26: class Horse : public Animal

are 1

28: public:

29:   Horse(COLOR color, HANDS height, int age);

30:   virtual ~Horse() { cout << "Horse destructor...\n"; }
312   virtual void Whinny()const { cout << "Whinny!... "7; }
52:   virtual HANDS GetHeight() const { return itsHeight; }
35:   virtual COLOR GetColor() const { return itsColor; }
34: protected:

$5:   HANDS itsHeight;

36:   COLOR itsColor;

371 +5

38:

39: Horse::Horse(COLOR color, HANDS height, int age):

40:   Animal (age),

41:   itsColor(color),itsHeight (height)

42:   {

43:      cout << "Horse constructor...\n";
44:   }

45:

46: class Bird : public Animal

472 £

48: public:

49:   Bird(COLOR color, BOOL migrates, int age);
50:   virtual ~Bird@) {cout << "Bird destructor...\n"; }

512   virtual void Chirp()const { cout << "Chirp... "; }

a2:   virtual void Fly const

53:      { cout << "I can fly! I can fly! I can fly! "; }

54:   virtual COLOR GetColor()const { return itsColor; }

D5   virtual BOOL GetMigration() const { return itsMigration; }

56: protected:

57s   COLOR itsColor;

58:   BOOL itsMigration;

59: 고

60:

61: Bird::Bird(COLOR color, BOOL migrates, int age):
62:   Animal (age),

63:   itsColor(color), itsMigration(migrates)

64:   {


===== PAGE 433 =====
제13일 다형성 ee 431

65:      cout << "Bird constructor...\n";
66:   }
67:
68: class Pegasus : public Horse, public Bird
69: {
70: public:
C1:   void Chirp()const { Whinny(); }
tes   Pegasus(COLOR, HANDS, BOOL, Long, int);
Cae   “Pegasus() {cout << "Pegasus destructor...\n";}
(4   virtual long GetNumberBelievers() const
Tae      { return itsNumberBelievers; }
(6:   virtual COLOR GetColor()const { return Horse::itsColor; }
TAGE   virtual int GetAge() const { return Horse: :GetAge(); }
78: private:
79: long itsNumberBelievers;
80% 3
81:
82: Pegasus: :Pegasus(
83:   COLOR aColor,
84:   HANDS height,
85%   BOOL migrates,
86:   long NumBelieve,
87:   int age):
88: Horse(aColor, height,age),
89: Bird(aColor, migrates,age),
90: itsNumberBelievers(NumBelieve)
91:2 ¢
92:   cout << "Pegasus constructor...\n";
9355 +
94:
95: int main()
96: ¢
97:   Pegasus *pPeg = new Pegasus(Red, 5, TRUE, 10, 2);
98:   int age = pPeg->GetAge();
99:   cout << "This pegasus is " << age << " years old.\n";
100: delete pPeg;
101: return 0;
102: F
결과   1: Animal constructor...
2: Horse constructor...
3: Animal constructor...
4: Bird constructor...
5: Pegasus constructor...


===== PAGE 434 =====
432 eo 제?주

This pegasus is 2 years old.
Pegasus destructor...

* Bird destructor. «.

: Animal destructor...

: Horse destructor...

: Animal destructor...

그 =ㄷㅇㅇ

— <초

분석  이 예제에는 흥미 있습니다. Animal 클래스가 9 - 18번 So] 선언되었습니다.
Animal? 하나의 멤버 변수 16486와 접근자 966&860를 가지고 있습니다.

26번 줄에서 Horse 클래스가 40004로부터 파생되었습니다. 8006 wate 세번
째의 매개 변수 ageS 베이스 클래스 ^40000로 보냄니다. Horse   스는
GetAgeQS 재생시키지 않고 상속받습니다.

46번 줄에서 800는 ^0008로부터 파생되도록 선언되었습니다. Bird 생성자 역시
나이를 취하고 베이스 Saaz Animals 초기화하는데 사용됩니다.

Pegasus*= Bird9} Horse 양쪽으로 상속을 받는데 따라서 Animale] 상속성을 다 가
지고 있습니다. tele) Pepe ala | at Gea 호출하려면 모 ie
니다.

TPA 줄에서 이 문제가 해결됩니다. Pegasus 객체가 어떤 계통을 타고 상속된 것
AS 알리는 666&860를 재생하여 선언합니다.

은 두 가지 이유에서 필요합니다. 이번 경우 같이 어떤 베이스
클래스를 타고 pane 모호성을 없애기 위함이거나 Se 어떤 작업 후 그 함수
를 좀더 딴 작업을 위해 베이스 클래스에 남겨놓을 목적으로 사용할 때입니다.
종종 여러분은 작업을 한 뒤 계통을 연결하기를 원할지 모르고 혹은 계통을 연결
한 뒤 베이스 클래스 함수가 반환될 때 작업을 진행할지 모릅니다.

Pegasus 생성자는 다섯 개의 매개 변수를 취합니다. 색깔, 키, 이주 여부, 믿는 사
람 수, 나이 등입니다. 88번 줄에서 생성자는 Pegasus©] 색깔, 7], 나이 등을 Horse
부분을 이용합니다. 89번 줄에서 생성자는 2688908의 색깔, 이주 여부, 나이를
Bird 부분을 이용해 초기화합니다. 마지막으로 OW 줄에서 믿는 사람 숫자를 초
기화합니다.
88번 줄에서의 Horse 부분의 생성자 SSS 39번 Fol] 있습니다. Horse 생성자는
age Animal 부분을 이용합니다. 다음엔 Horse 부분의 itsColorS} itsHeight?] 두
개의 멤버 변수로 초기화합니다.


===== PAGE 435 =====
제13일 다형성 ee 433

89번 줄의 800 부분의 생성자 호출은 61번 줄에 구현된 것을 사용합니다. 여기서
도 286는 Animal 부분을 사용합니다.

보다시피 2688508의 색깔은 HorseS} 800의 양쪽 BRS 다 사용하였습니다. 또 나
이 부분도 Animal 베이스로 한 Horse] 15486와 Animal? 베이스로 한 800의
itsAgeS 사용하였습니다.

가상 상속(10481 Inheritance)
[리스트 13.5]에서 2688545의 클래스는 베이스 클래스의 어느 부분을 사용할 Aol

가를 서술하여 모호성을 탈피하였습니다. 대부분의 경우 어느 계통을 사용할 것
인가는 임의적입니다. 7] Horses} Bink: 같은 조상을 가지고 있기 PES

니타,

0++에서 여러분은 같은 베이스 클래스의 두 개의 복사본을 원하기보다는([그림
13.2]) [그림 13.31과 같이 단일 공통 클래스를 원

[그림 13.3]
다이아몬드형의 상속

Animal

Horse                       Bird

Pegasus

eft Animal Horses} 800에 대한 가상 베이스 클래스로 만듬으로써 이를
이룰 수 있습니다. Animal 클래스는 전혀 변하지 않습니다. Horsey} Bird Hale:
가 각각의 선언에서 10088이라는 말을 사용할 때 변화가 일어납니다. 그리고
질적인 변화는 2688545에서 일어납니다.

보통 클래스의 생성자는 단지 그 자신의 변수와 베이스 클래스를 초기화합니다.
가상적으로 상속된 베이스 클래스는 예외입니다. 가상 상속은 가장 최근에 파생


===== PAGE 436 =====
434 ee 제2주

yy tl

클래스로 27) uc. Animale Horse9} Bird= 초기화되지 51 Pegasus 2]
으로 초기화됩니다. Horses} Bird= AnimalS 각자의 생성자로 초기화해야 합니
하지만 이 초기화는 2688545가 만들어지면 무시될 것입니다.

대
[리스트 13.6|은 [리스트 BIS 가상 상속의 이점을 활용하여 다시 작성하였습니다.

[리스트 13.6] 가상 상속의 예

1: // [리스트 13.67 가상 상속의 예

~

3: #include <iostream.h>

4:

5: typedef int HANDS;

6: enum COLOR { Red, Green, Blue, Yellow, White, Black, Brown } ;
7: enum BOOL { FALSE, TRUE };

8:

9: class Animal // HorseSt Bird 대한 공통 베이스

A0: £

11: public:

lige   Animal (int);

135   virtual ~Animal() { cout << "Animal destructor...\n"; }
145   virtual int GetAge() const { return itsAge; }

15   virtual void SetAge(int age) { itsAge = age; }

16: private:

Ae   int itsAge;

188 35

191

20: Animal::Animal (int age):

21: itsAge(age)                                            =."
22: ¢                                of Sri
23:     cout << "Animal constructor...\n";      > .NY Ayer
24: }                                     :

25:                                      뉴트

26: class Horse : virtual public Animal

272 <

28: public:

29:   Horse(COLOR color, HANDS height, int age);

30%   virtual ~Horse() { cout << "Horse destructor...\n"; }
S1:   virtual void Whinny()const { cout << "Whinny!... "; }
Set   virtual HANDS GetHeight() const { return itsHeight; }
33:   virtual COLOR GetColor() const { return itsColor; }

34: protected:

59:   HANDS itsHeight;

56:   COLOR itsColor;

37: 33

(시
co


===== PAGE 437 =====
제13일 다형성 ee 435

59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
501
571 【
Dee
535
54:
5D
26:
50s
58:
59%
60:
61:
62:
65:
64:
65:
66:
60s
68:
69:
(05
Cle
72:
73;
74:
(ay
76:
OC
(83
(95
80:
ol:
82:
83:
84:
85:

Horse::Horse(COLOR color, HANDS height, int age):
Animal (age),
itsColor(color),itsHeight (height)

{
cout << "Horse constructor...\n";
}

class Bird : virtual public Animal
{
public:
Bird(COLOR color, BOOL migrates, int age);
virtual ~Bird() {cout << "Bird destructor...\n"; }
virtual void Chirp()const { cout << "Chirp... "; }
virtual void Fly() const { cout << "I can fly! I can fly! I can fly! "; }
virtual COLOR GetColor()const { return itsColor; }
virtual BOOL GetMigration() const { return itsMigration; }

protected:
COLOR itsColor;
BOOL itsMigration;
3;

Bird::Bird(COLOR color, BOOL migrates, int age):
Animal (age),
itsColor(color), itsMigration(migrates)
{
cout << "Bird constructor...\n";

class Pegasus : public Horse, public Bird
£
public:
void Chirp()const { Whinny(); }
Pegasus(COLOR, HANDS, BOOL, long, int);
“Pegasus() {cout << "Pegasus destructor...\n";}
virtual long GetNumberBelievers() const { return itsNumberBelievers; }
virtual COLOR GetColor()const { return Horse::itsColor; }

private:
long itsNumberBelievers;
3;

Pegasus: : Pegasus (
COLOR aColor,
HANDS height,
BOOL migrates,
long NumBelieve,


===== PAGE 438 =====
436 ee 제2주

86:    int age):

07:   Horse(aColor, height,age),

88:    Bird(aColor, migrates,age),
89:    Animal (age*2),

90:    itsNumberBelievers(NumBel ieve)

91%   {

92:     cout << "Pegasus constructor...\n";
95:   }

94:

95: int main()

96: £

97:   Pegasus *pPeg = new Pegasus(Red, 5, TRUE, 10, 2);
98:   int age = pPeg->GetAge();

995   cout << "This pegasus is " << age <<" years old.\n";
100: delete pPeg;

101: return 0;

102: }

24 Dh  Animal constructor...

Horse constructor...

Bird constructor...

Pegasus constructor...

This pegasus is 4 years old.
Pegasus destructor...

Bird destructor...

Horse destructor...

Animal destructor...

EN AY 2641 중에서 Hones 가상적으로 Animale] 상속되도록 선언되었습니다.
~ 46번 줄에서 Bird 같은 ANS 하였습니다. 800와 Horse] 생성자는 계속
Animal 객체를 초기화함을 주목합시다.

Pegasus HorseS} Bird 양쪽으로부터 상속됩니다. 그리고 Animale] 대한 가장 최
근의 파생 객체로서 40000을 역시 초기화합니다. 호출되는 것은 Pegasus®] 초기
3+] Bird2} 8066의 Animalo] 대한 초기화는 무시됩니다. 값 2가 전달되고 Horse
와 Bird= 그 ZS Animal 전달하는데 Pegasus7} 그 값을 2배를 해버립니다. 결
과는 4가 되어 99번 So] 해당하는 출력에서 나타납니다.

Pegasus GetAge)S 호출할 때 더 이상의 모호성은 없습니다. 이 FFs Animal
로부터 상속받아 문제가 없습니다. Pegasus 060001000를 호출하면서 모호성을
아직 지니는데 이는 4000081에는 없고 양쪽의 베이스 클래스에는    니다.

why

9)


===== PAGE 439 =====
제13일 다형성 ㅎㅎ 437

가상 상속의 클래스 선언
파생 클래스가 단지 공통 베이스 클래스 중 하나만을 사용하고자 할 때, 중간의 클래스를
원하는 베이스 클래스로부터 가상적으로 상속받도록 합니다.
예제 1
class Horse : virtual public Animal

class Bird : virtual public Animal
class Pegasus : public Horse, public Bird

예제 2

class Schnazer : virtual public Dog
class Poodle : virtual public Dog
class Schnoodle : public Schnazer, public Poodle

다중 상속의 문제점들

중 상속이 단일 상속에 비해 더 많은 이점들을 제공하지만 많은 c+ 프로그래
들은 이를 사용하기를 싫어합니다. 그들이 들먹이는 문제는 아직 많은 컴파일
가 이를 지원 안하고, 따라서 디버깅이 어렵고, 또 다중 상속으로 만들어진 대
부분들은 다중 상속 없이도 돌게 할 수 있다는 것입니다.

이는 근거가 있는 말이고, 따라서 여러분은 복잡하고 불필요한 것을 여
로그램에 넣지 않으려는 명분으로 삼길 원할 것입니다. 사실 몇몇 디버
중 상속을 iat 아주 심한 고생을 합니다. 그리고 Be 설계사들

00 새로운 클래스가 하나 이상의 베이스 클래스로부터 geo 여러 특징들을
필요로 할 때 다중 상속을 사용합시다.

on 2
OG    대부분의 파생 클래스가 공통된 베이스 클래스에서 나올 때 가상 상속을 사
용랍시타.
oS
DO    PE MIA 클래스를 사용할 때 파생 클래스로부터 공통 베이스 클래스를
i te es 가
초기환합시다.

DONT 단일 상속으로 가능한 문제에 다중 상속을 사용하지 gpyey,



===== PAGE 440 =====
438 ee 제2주

혼합(10) 그리고 만능 클래스
다중 상속과 단일 상속의 중간부를 치고 나가는 방법에 혼합00000) 방법이 있습
니다. 여러분은 여러분의 Horse 클래스가 Animals} ㅁ215000006로부터 파생되게 할
수 있습니다. 016040006은 화면에 몇몇 객체를 나열하는 몇 가지 메쏘드를 추가
하였습니다.

새로운 (훈합(41<-10) 클래스| 혼합 Se 만능 클래스는 자료를 약간 Se 주가하지 않은 제

기능 클래스는 다른 클래스와 마찬가지로 파생 클래스 들로 섞여있는데 파생 클
래스 들이 상속을 받도록 선언되었습니다. 그러나 다른 클래스와의 차이점은 기
능 클래스는 자료가 아주 적거나 없다는 것입니다. 물론 이는 임의적인 구분법입
니다. 파생 클래스를 복잡하게 하지 않고 몇 개의 추가 기능을 뒤섞는 것입니다.

이렇게 하면 몇몇 디버거들에게는 복잡한 다중 상속을 사용하지 않고 VS 쉽게
Poe 합니다. 또 기본적인 베이스 BAAS 접근하는 데 있어서 모호성도 적
을 것 같습니다.

*   2,

들면, Horse Animaly} 1049018/806로부터 상속되었는데 Displayable? 자료
가지고 있지 않습니다. Animale 원래의 그 모습 그대로이고 따라서 Horsec
Animal 222-5] 상속받았지만 80066의 함수는 이제 양쪽으로부터 받을 수 있습니다.

티네 개 ~ -=

ㆍ혼합08×10'이라는 단어는 써머빌과 메사추세츠의 아이스크림 가게로부터 유래
되었는데 캔디와 케이크가 섞여 기본 아이스크림이 되었습니다. 이는 SCOOPSE}
는 객체 지향 프로그램 언어를 가지고 작업을 하는 프로그래머들이 여름 휴가를
취하곤 하던 그곳에서 유래된 듯합니다.

추상 Tte% (Abstract Data Type)

종종 여러분은 같은 계충의 클래스들을 같이 만들 수 있습니다. 예를 들면

Rectangles} (37016을 파생시키는 58806라는 클래스를 만들    있습니        형

으로부터 정사각형이라는 SAAS 만드는데 이는 직사각형의 특정한 일부분입

니다.

각각의 파생된 클래스들은 2000\0와 GetAreaQeh= ARES 재생시킬 것입니다.

[리스트 13.7]은 98806 SAAS FAR 모습과 거기서 파생된 Circle, Rectangle 클
스를 보여줍니다.


===== PAGE 441 =====
제13일 다형성 ee 439

[리스트 13.7] Shape 클래스

// [리스트 1353.73 Shape 클래스

#include <iostream.h>

1
2
3
4:
5: enum BOOL { FALSE, TRUE };
6:
7: class Shape

&: +

9: public:

10:   Shape () {}

V1:   “Shape (){}

12: virtual long GetArea() { return -1; } // 오류

iss   virtual long GetPerim() { return -1; }

14s   virtual void Draw() {}

15: private:

162 가,

10"

18: class Circle : public Shape

19: <

20: public:

211   Circle(int radius):itsRadius(radius) {}

22:   “Circle(){}

23:   long GetArea() { return 3 * itsRadius * itsRadius; }

24:   long GetPerim() { return 9 * itsRadius; }

20%   void Draw();

26: private:

ar:   int itsRadius;

28%   int itsCircumference;

29> Fy

30:

31: void Circle::Draw()

S28 -<

55:    cout << "Circle drawing routine here!\n";

54: }

55:

56:

37: class Rectangle : public Shape

38: <€

59: public:

40:   Rectangle(int len, int width):

41:   itsLength(len), itsWidth(width) {}

42:   “Rectangle(){}

441   virtual long GetArea() { return itsLength * itsWidth; }

44:   virtual long GetPerim() {return 2*itsLength + 2*itsWidth; }
45:   virtual int GetLength() { return itsLength; }


===== PAGE 442 =====
440 ce 제주

46:   virtual int GetWidth() { return itsWidth; }
47:   virtual void Draw();

48: private:

49:   int itsWidth;

50:   int itsLength;

Sle oy

52:

53: void Rectangle::Draw()

54: £

D8   for (int i = 0; i<itsLength; i++)
56:   {

571      for (int 1 = 0; j<itsWidth; jt+)
Dot         cout << "x";

59:

60:      cout << "\n'"s

61:   개

62: 고

63%

64: class Square : public Rectangle

65: £

66: public:

6s   Square(int len);

68:   Square(int len, int width);

69:   “Square () {}

10:   long GetPerim() {return 4 * GetLength() ;}
718 2)

(2:

73: Square::Square(int Len, int wath) ;

74:   Rectangle(len,len)

058 <3

76:

77: Square::Square(int len, int width):
18:   Rectangle(len,width)

(9%

80: {

81:     if (GetLength() != GetWidth())
82:       cout << "Error, not a square... a Rectangle??\n";
Boe 2

84:

85: int main®

86: {

87:   int choice;

88:  BOOL fQuit = FALSE;

89:   Shape * sp;

90:

91:   while (1)

92:5   {


===== PAGE 443 =====
제13일 다형성 ee 441

93:
94:
95:
96:
97:
98:
99:

100:
1012
102:
105:
104:
105:
106:
107:
108:
109:
110:
111:
1125
113%
114:

cout << "(1)Circle (2)Rectangle (3)Square (0) Quit: ms
cin >> choice;

switch (choice)

내
case 1: sp = new Circle(5);
break;
case 2: sp = new Rectangle(4,6);
break;
case 3: sp = new Square(5);
break;
default: fQuit = TRUE;
break;
}
if (fQuit)
break;
sp->Draw();
cout << "\n";
}
return 0;

}

(1)Circle (2)Rectangle (3)Square (O)Quit: 2
x XK X xX
xx xX x MX
XN XK RK
XxX «XX X
(1)Circle (2)Rectangle (3)Square (O)Quit: 3

Xx eX x
xX xX xx &
Xk XX K
MX XX K
XK X OK
(1)Circle (2)Rectangle (3)Square (O)Quit: 0

를 100한다는 것은 무엇을 뜻합니까? 모양(58009/의 형(원, 사각형 Be 그
수 있지만 추상으로서의 모양(94808은 그려질 수 없습니다.

Circle 54006로부터 파생되었고 세 개의 가상 메쏘드를 재생하였습니다. ‘virtual’
이라는 단어를 붙일 필요가 없습니다. 왜냐하면 상속의 일부분이기 때문입니다.


===== PAGE 444 =====
442 ee 제2주

그렇다고 미리 그렇게 하여 손해볼 건 없는데 43, 44, 47번 줄의 Rectangle 클래스
에서 보여줍니다.

Square= Rectangle@3-E] 파생되었고 00606000을 재생하였고 #6080806에 있는
나머지 메쏘드를 상속받았습니다.

사용자가 Shape BAS 실제로 사용하려는 것은 귀찮은 일이고, 아예 불가능하게
만드는 것이 바람직한 것처럼 보이기도 합니다. Shape 클래스는 자이으파티 파
생된 클래스에게 인터페이스만 제공하기 위해 존재합니다. 이것이, 추상 자료형입

니다. 이를 121(066040 data type) = 합니다.
새로운        령은 객체(0706 같은 WS 나타낸다기 보다는 개념(91606 같은
응어    탁낼니다. oe ADTE 항상 다른 클래스들에 대해 베이스 클래스이고
|      ;

순수 가상 &4(Pure Virtual Function)

CHe 순수 가상 함수라는 것으로 추상 자료형의 표준을 지원합니다. 가상 함수
를 0으로 초기화함으로써 순수 가상 함수로 됩니다,

virtual void Draw() = 0;
하나 이상의 순수 가상 함수
인스턴스(실체화)하는 것은 좋
여러분의 클래스에 순수함수
가지를 알립니다.

1, 이 클래스에 객체는 만

ㅅ

2 = 순수 가상 함수는 재생

를 가진 클래스를 401라하고 ADT?) 클래스 객체를
지 않습니다. 이렇게 하면 컴파일러 오류가 납니다.
집어넣는 것은 여러분의 클래스의 사용자에게 두

가     “ft   al

ADT#¥ =} 파생된 어떠한 SHAE 순수 가상 함수를 상속하고 객체를 실체화하
는 방법은 오직 순수 가상 함수의 재생을 통해서 입니다. 만일 Rectangle7} Shape
로부터 상속하였고 Shaper} 세 개의 순수 가상 함수를 가졌다면 80000966는 이
세 개를 재생해야 하거나 그 자신도 407가 되어야 합니다. [리스트 13.8]은 91806
가 ADT} 되도록 다시 구성하였습니다. 공간을 절약하기 위해 [리스트 13.719
나머지 BES 다시 작성하지 않았습니다. [리스트 13-719] 7 - 16번 줄의 Shape
선언부를 [리스트 13.8]로 바꾸고 프로그램을 다시 실행시켜 봅시다.


===== PAGE 445 =====
제13일 다형성 ee 443

[리스트 13.8] 추상 자료형

1: class Shape

22 에

3: public:

4    Shape (){}

be    “Shape (){}

6:   virtual long GetArea(
7:

8

9:

1

virtual long GetPerim
virtual void Draw()
private:
Os 가조

24 Df  (1)Circle (2)Rectangle (3)Square (0)Quit:

XXX XXX
X XXX XX
XX X X X X       x
XX XX XX

(1)Circle (2)Rectangle (3)Square (0) Quit:

XX XXX
XX X X X
xX XX X X
XXX XX
XX X X X

(1)Circle (2)Rectangle (3)Square (0)Quit:

앞에서 보았듯이 프로그램이 전혀 바뀌지 않았습니다. 단 하나의 차이점은

a
iz

2

3

0

Shape 클래스의 객체를 WEE 것이 불가능해졌습니다.

eee

추상 자료형
클래스 선언부에 하나 이상의 순수 가상 함수

예제

class Shape
{

virtual void Draw() = 0 ;// 순수 가상

를 포함시켜 추상 자료형 클래스를 선언합니
다. 함수 선언부 뒤에 = OS 써서 순수 가상 함수임을 선언합니다.

BA
함수



===== PAGE 446 =====
444 ee 제2주

순수 가상 함수의 구현
원래 추상화된 베이스 클래스에서의 순수 가상 함수
하면 어떤 객체도 만들어질 수 없기 때문이고

는 구현될 수 없습니다. 왜냐
따라서 구현할 필요가 없으며,

ADTE 그 자신으로부터 파생되는 객체와의 인터페이스에 대한 정의로만 Fes

하기 때문입니다.

하지만 순수 가상 함수에 구현을 하는 것은 가능합니
된 객체에 의해 호출될 수 있는데, 아마 모든

을 부여하기 위함일 것입니다. [리스트 13이는 [리스트

재생된 함수들에게
13.7]을 다시 만들

다. 함수

는 412로부터 파생
공통적인

기능
는데

을 위해 베이스 클래스 함수에 연

것이며, 여러분은 베이스 클

이번에는 Shape ADTE. 하였고 순수 가상 함수 200\0를 구현하였습니다. 0006
클래스는 108\0를 재생하였고, 추가적인 기능

결되었습니다

이 예에서 추가적인 기능은 간단한 BAS 출력하는

래스가 공유된 그리기 기능을 제공한다는 것을 생

파생 클래스가 사용할 윈도우를 설정

[리스트 13.9] 순수 가상 함수의 구현

각하긴 어렵지 않을

하는 것입니다.

것입니다.

// [리스트 13.91 순수 가상 힘
#include <iostream.h>
enum BOOL { FALSE, TRUE };

class Shape

{

public:
Shape () {}
“Shape () {}
virtual long GetArea() = 0;
virtual long GetPerim()= 0
virtual void Draw() = 0;

: private:

가

2 ¢

CONAOU FWD —
ㅁㅁ ㅁㅁ ee oe ㅋㄷㅋㄷ oe

ee a ee ok ab ak SO
NOU 은 에 0 | OF §
en ee … oe oon

—
co

void Shape

600 060 =
- oO 0

: }          yer rar Orroroo eee ™"v

NN
WM

: class Circle : public Shape

cout << "Abstract drawing mechanism! \n";


===== PAGE 447 =====
제13일 다형성 ee 445

24: 1.

25: public:

26:   CircleCint radius) :itsRadius (radius) {}

20:   “Circle() {}

28:   long GetArea() { return 3 * itsRadius * itsRadius; }
29:   long GetPerim() { return 9 * itsRadius; }

30:   void Draw();

31: private:

32:   int itsRadius;

55:   int itsCircumference;

34: 3;

55%

36: void Circle::Draw()

Sf: £

38:   cout << "Circle drawing routine here!\n";

39%   Shape::Draw();

405 3             Ly avy 44

42:

43: class Rectangle : public Shape

44: {

45: public:

46:   Rectangle(int len, int width):

47:   itsLength(len), itsWidth(width) {}

48:   “Rectangle(){}

49:   long GetArea() { return itsLength * itsWidth; }
50:   long GetPerim() {return 2*itsLength + 2*itsWidth; }
515   virtual int GetLength() { return itsLength; }
525   virtual int GetWidth() { return itsWidth; }

a3   void Draw();

54: private:

55:   int itsWidth;

56:   int itsLength;

5/5 33

58:

59: void Rectangle: :Draw()

60: 1

61:   for (int i = 0; i<itsLength; i++)
62:   {

63:      for (int j = 0; j<itsWidth; j++)
64:        cout << "KK "3

65:

66:      cout << "\n";

67: }                         :
(08 +

(1:


===== PAGE 448 =====
446 ee He

721
73:
74:
122
76:
(고
78:
192
80:
81:
82:
85:
84:
85:
86:
30:
88:
89:
90:
91:
92:
93:
94:
95:
96:
or?
98:
99:

100:
101:
102:
103:
104:
105:
106:
107:
108:
109:
110:
111
V125
113%
114:
115:
116%
11¢:
118:

class Square :

af

public:
Square(int len);
Square(int len, int width);
“Square(){}
Long GetPerim() {return 4 * GetLength() ;}

Dd;

public Rectangle

Square::Square(int len):
Rectangle(len,len)

tt

Square::Square(int len, int width):
Rectangle(len,width)

{

}

if (GetLength() != GetWidth())
cout << "Error, not a square... a Rectangle??\n";

int main()

{

int choice;
BOOL fQuit = FALSE;
Shape * sp;

while (1)

nf

cout << "(1)Circle (2)Rectangle (3)Square (O)Quit: ";

cin >> choice;

switch (choice)

{
case 1: sp
break;
case 2: sp
break;
case 3: sp
break;

new Circle(5);
new Rectangle(4,6);

new Square(5);

default: fQuit = TRUE;

break;
B
if (fQuit)
break;

sp->Draw();
~” 0”


===== PAGE 449 =====
제13일 다형성 ee 447

119:     cout << "\n";
120: 3}

121: return 0;

122: 3

결과  (1)Circle (2)Rectangle (3)Square (O)Quit: 2
Xx XX XXX

XxX xX MX
XxX XX XX

xxx KK X

Abstract drawing mechanism!

(1)Circle (2)Rectangle (3)Square (O0)Quit: 3

XX XXX
X X X X X
Xx XXX X
XX X XK X
XX XXX

Abstract drawing mechanism!
(1)Circle (2)Rectangle (3)Square (O)Quit: 0

7 - 10번 줄에서 추상 자료형 Shapo7} 선언
가 가상 함수로 선언되었습니다. 이는 반드시 필요한 것은 baie 어떤

함수 하나라도 순수 가상으로 선언되었

ㆍ GetArea()9} 0606800 메쏘드는 구현되지 않았지만 06020440는 구현되었습니다.

Circle>} Rectangle= = 다 GetDrawOS 재생하였습니다. 그리고 둘 다 베이스 메

쏘드까지 연결되었는데 이는 베이스 클래스에서의 기능을 공유하는 이점을 가집

니다.

(aa
i

추상의 복합 W4(Complex Hierarchies of Abstraction)
때로 여러분은 하나의 41로부터 다른 ADTS 파생시킬 수 있습니다. 여러분은
파생된 순수 가상 함수는 순수하지 않게, 그리고 나머지는 그대로 순수 가상 함
수로 할 수 있습니다.
Animal 클래스를 만들 때 8060, Sleep, Move(), ReproduceQS 모두 순수 가상 함
수로 만들 수 있습니다. 아마 Animal SPE] 포유류와 FS sea 수 있을
oe

포유류를 이런 방식으로 만든 후 oz] Mammal::Reproduce()= 비순수로 만들

고, Eat(), Sleep0, MoveQ%= 순수 가상 함수로 만들 수 있습니다.


===== PAGE 450 =====
448 ee 제2주

포유류로부터 여러분은 WS 만든 후, Dog= 재생을 하고 세 개의 남아있는 순
가상 함수를 구현하여 208형의 AAS 만들 수 있습니다.

클래스 설계자로서 여러분은 어떠한 400081이나 Mammal& 인스턴스될 수
들었지만, 모든 Mammal® 제공된 #600000060 메쏘드를 재생하지 않고 상

수 있습니다.                :

[리스트 13.10|이 이 클래스의 구현을 보여줍니다.

[리스트 13.10] 하나의 401로부터 파생된 ADT

: // [리스트 13.103 하나의 407로부터 파생된 ADT
ase
: #include <iostream.h>

: enum COLOR { Red, Green, Blue, Yellow, White, Black, Brown } ;
enum BOOL { FALSE, TRUE 3;

CONDOU FWD —

class Animal

9: £

10: public:

11   Animal (int);

42%   virtual ~Animal() { cout << "Animal destructor...\n"; }
13%   virtual int GetAge() const { return itsAge; }
14:   virtual void SetAge(int age) { itsAge = age; }
IDE   virtual void Sleep() const = 0;

16%   virtual void Eat() const = 0;

17:   virtual void Reproduce() const = 0;

18:   virtual void Move() const = 0;   AT

19:   virtual void Speak() const = 0;

20: private:

21:   int itsAge;

22: 3}

25%

24: Animal::Animal (int age):

25: itsAge(age)

26: {

27:   cout << "Animal constructor...\n";
28: }

29%

30: class Mammal : public Animal

Bs x

32: public:

55   Mammal (int age) :Animal(age) { cout << "Mammal constructor...\n";}

34:   “~Mammal() { cout << "Mammal destructor...\n";}


===== PAGE 451 =====
제13일 다형성 ee 449

55    virtual void Reproduce() const { cout << "Mammal reproduction depicted...\n"; }

56: };

37:

38: class Fish : public Animal

359: £

40: public:

41:   Fish(int age) :Animal(age){ cout << "Fish constructor...\n";}
42:   virtual ~Fish() {cout << "Fish destructor...\n"; }

43:   virtual void Sleep() const { cout << "fish snoring...\n"; }

44:   virtual void Eat() const { cout << "fish feeding...\n"; }

45:   virtual void Reproduce() const { cout << "fish Laying eggs...\n"; }
46:   virtual void Move() const { cout << "fish swimming...\n"; }

47:   virtual void Speak() const { }

48:

492 }:

50:

51: class Horse : public Mammal

522 £

53: public:

54:   Horse(int age, COLOR color ):

55%   Mammal (age), itsColor(color) { cout << "Horse constructor...\n"; }
56:   virtual ~Horse() { cout << "Horse destructor...\n"; }

57:   virtual void Speak() const { cout << "Whinny!... \n"; }

58:   virtual COLOR GetItsColor() const { return itsColor; }

59:   virtual void Sleep() const { cout << "Horse snoring...\n"; }
60:   virtual void Eat() const { cout << "Horse feeding...\n"; }
61:   virtual void Move() const { cout << "Horse running...\n";}
62:

63: protected:
64:   COLOR itsColor;

65: +5

66:

67: class Dog : public Mammal

68: £

69: public:

102    Dog(int age, COLOR color ):

Ms   Mammal Cage), itsColor(color) { cout << "Dog constructor...\n"; }

f2:   virtual ~Dog() { cout << "Dog destructor...\n"; }

(3:   virtual void Speak()const { cout << "Whoof!...\n"; }

7481   virtual void Sleep() const { cout << "Dog snoring...\n"; }

(52   virtual void Eat() const { cout << "Dog eating...\n"; }

16:   virtual void Move() const { cout << "Dog running...\n"; }

77: virtual void Reproduce() const { cout << "Dogs reproducing...\n"; }
78:

79: protected:

80:   COLOR itsColor;

812 3;


===== PAGE 452 =====
450 ee Rae

82:

83: int main()

84: {

85:   Animal *pAnimal=0;

86:   int choice;

87:   BOOL fQuit = FALSE;

88:

89: while (1)

90% <":

91:    cout << "(1)Dog (2)Horse (3) Fish (O)Quit: ";
92:     cin >> choice;

93:

94:     switch (choice)

95:     {

96:      case 1: pAnimal = new Dog(5,Brown) ;
90:      break;

98:       case 2: pAnimal = new Horse(4,Black);
99:      break;

100:    case 3: pAnimal = new Fish (5);
101:    break;
102:    default: fQuit = TRUE;

103:    break;

104:    }

105:    if (fQuit)

106:       break;

107:

108:     pAnimal->Speak();
109:     pAnimal->Eat();
110:     pAnimal->Reproduce();
Tit:     pAnimal->Move();
112:     pAnimal->Sleep();
113:     delete pAnimal;
114:     cout << "\n";
1155   가

116:

117: return 0;

118:

119% 3

결과  (1)009 (2)Horse (3)Bird (O)Quit: 1
Animal constructor...
Mammal constructor...
Dog constructor...
Whoof!...
Dog eating...


===== PAGE 453 =====
제13일 다형성 ee 451

Dog Reproducing...
Dog running...

Dog snoring...

Dog destructor...
Mammal destructor...
Animal destructor...

(1)Dog (2)Horse (3)Bird (O)Quit: 0

8 - 228 줄에서 추상 자료형 Animalo] 선언되었습니다. Animale 비순수
가상 접근자를 가지는데 이는 Animal 객체에 의해 공유됩니다. 다섯 개의
순수 가상 함수 916600, 88060, Reproduce(), Move(), 506800을 가집니다.

Animal-2- Mammal-2 파생하고 이는 30 - 36번 So] 있는데 추가된 자료가 없습니
다. 그러나 ReproduceQS 재생하는데 모든 포유류에 대해 공통되는 형식을 제공
합니다. Fish= ReproduceQS 재생해야 합니다. 왜냐하면 버애는 400081로부터 파
생되고 포유류의 reproduction] 이점을 취할 수 없기 때문입니다.

Fish, Horse, 1208은 모두 남아있는 순수 가상 함수를 재생하였는데 따라서 그들의
BS 가진 객체들은 인스턴스0090008)될 수 있습니다.

프로그램의 몸체에서 Animal 포인터는 각각의 파생된 객체들을 포인트하도록 사
용되었습니다. 가상 메쏘드가 호출되었고 AYA 포인터를 묶는 방식이 채택되었
으며 파생된 클래스에서 올바른 메쏘드가 호출되었습니다.

000히이나 Mammal? 인스턴스하는 것은 오류를 발생합니다. 왜냐하면 둘 다 추
상 자료형이기 때문입니다.

(aa
=

어떤 Yo] 주상인가?
하나의 프로그램에서 Animale 추상이고 다른 프로그램에서는 아닙니다. 무엇을
가지고 추상인지 아넌지를 판단할까?

이에 대한 Be 실질 세계에 의해 oa  게이 아니라 여러분의 ot 서
382 Animale SY 지료형으로 할 수 i 지만 00는 WANE 인스턴스하는 클
래스로 될 수 있습니다.

한편 개집을 짓는다면 여러분은 Dogs 추상 자료형으로 할 수 있고, 개의 인스턴
AS 만들 수 있습니다. 추상의 각 단계는 여러분의 형을 잘 구별할 필요에 의해
는 함수입니다.

a |
4

=


===== PAGE 454 =====
452 ㅇㅇ 제2주

DO    여러 개의 관계된 클래스의 공통된 기능을 제공하?| 위해 주상 자료령을 사

용합시다.
po       든 순수 가상 함수를 중복합시다
DO 중복되어야 할 모든 함수를 순수 가상으로 만듭시다
DONT 추상 자료형의 WME 인스턴스하지 Bet.

O&A

Q 기능 AS(percolating functionality 40\810)이란 FAS 의미합니까?
공통의 베이스 클래스로 끌어올리는 AS 뜻합니다. 하나 이상의
공유하면 공통 베이스 클래스를 찾는 것이 바람직합니다.

오비
AS
a
sc,

ileal
ot
주
~
re
10
Hu
xz
고
rir
yay
트여
olf
ty
Aw)
cs

 실행시 형 서술 HHO! Ot SE 이유는?

A 큰 프로그램에서 switch 문장은 크고 유지하기 어려운 점이 있습니다. 가상 함수의
요점은 가상 테이블을 만드는 것에 있습니다.

Q 형 변환이 왜 안 좋습니까?

A 형을 안정되게 한다면 형 wee 나쁘진 않습 다 어떤 객체가 특정형이어야 한다
     진 않습니다. 형 변환은 0++에서
| 피하는 이유  나체 어러분이 객체에 대해 실

그램이 뭔가 잘못됐다는 것입

|
후
4)
SG
fot
rye

ttl
= oe
=
-
riot
2,

니다.
Q 애 모든 합수를 가상으로 만들지 않는지?
A 가상 함수는 가상테이블에 의해 유지되는데 이는 실행시 프로그램의 크기와 수행성

에 부담이 됩니다. 여러분의 클래스가 매우 작고 하부 클래스가 없다면 어떤 함수
도 가상으로 만들지 be 것입니다.


===== PAGE 455 =====
제13일 다형성 ee 453

Q MW 소멸자는 가상으로 만드는지?

A 항상 여러분의 클래스가 하부 클래스가 될 수 있다고 생각하고, 베이스 클래스에
대한 포인터가 하부 클래스의 객체를 접근하기 위해 사용될 수 있다고 생각합시다.
우선 여러분이 어떤 함수를 가상으로 만들었다면 소멸자는 가상으로 만듭시다.

Q 왜 추상 자료형을 만드는지. 왜 비추상형으로 만들지 않고 그 형으로 만드는 것을 피하
지 않습니까?

A 에서 많은 개념들은 컴파일러가 OFS 잡게 하는데 있습니다. 따라서 여러분은
AYA) 오류를 줄여야 합니다. 클래스를 추상으로 만들어(순수 가상 함수를 주고)
컴파일러로 하여금 그 추상 자료형으로 만들면 OFS 발생시키게 합니다.

연구

이 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가

를 확인해 보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어
있습니다 부록 0에 있는 담을 보기 전에 각 물음에 대답할 수 있도록 노력하고,
다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다.

퀴즈

1. 형 변환 하향(6851 00\00)은 무엇입니까?

2 v-ptro|Zt?
3. ia 사각형이 직선 변과 둥근 모서리를 town  RoundRect= Rectangle=t Circle
부터 상속받고, 또 동시에 ShapeS te} 상속받습니다. RoundRectS 만들 때 얼마

. 많은 Shape7} 만들어집니까?

4 110156와 Bird7} public 가상 SSS 사용하여 Animale He, 상속받을 때 생성자가
Animal 생성자를 초기화해야 합니까? 만일 『698545가 Horse? ㅁ|[0로부터 상속받
을 때 어떻게 Animal 생성자를 초기화합니까?

$ㆍ vehicles 추상 자료형으로 만드는 클래스를 선언하십시오.

@ 베이스 클래스가 ADTO|D 세 개의 순수 가상 함수를 갖는다면 파생 클래스에서 몇 개
의 재생을 가져야 합니까?

P

연습 문제
1. Rocket? Airplane2 4H 상속받는 클래스 46[018116을 선
2 101M 기술된 JetPlaneQe Se ASHE 747에 대해 선언하십시오.


===== PAGE 456 =====
454 ee 제2주

3 \/하)016로부터 파생된 CarZ} 6806를 갖는 프로그램을 만드십시오. Vehicles 두 개의
8

순수 가상 함수를 갖는 ADTI} 되도록 하십시오. 단 BusSt Car= ^01가 아니게 하십
시오

4.14   enol 발전하여 하이 ADT7} 되도록 하고 08[로부터 SportsCarSt CoupeS
만드십시오. Car 클래스에서 Vehicleoll 있는 순수 가상 함수 중 하나를 구현하고 이것

을 ule  수로 만들어 봅시다.



===== PAGE 457 =====


===== PAGE 458 =====
456 ee 제2주

서문

g        2
공합니다. 지금까지 여러분은 전역 변수, 지역 변수, 변수를 가리키는 포인터, 클
래스 멤버 변수들을 만드는 YS 보았습니다. 오늘 여러분이 배울 내용은 다음과

같습니다.

i
nt
4)
tuft
-구
mL
그
rir
Hel
pica
md
at
wz
tll
=
x
kJ
_오
아모
=
iT]
Hu
a
of
tl
ie ㅁ
mi

=
~~

정적 멤버 Tt=(Static Member Data)

지금까지 여러분은 각 객체에 있는 자료들을 그 객체에 대해서 유일하며 클래스

내에서 다른 객체들 사이에 공유되지 않는 것으로 생각해 왔습니다. 예를 들면,

여러분이 다섯 개의 Cat 객체를 가지고 있다고 합시다. - 자신의 나이, 무게, 기타

등등 - 그 객체의 나이는 다른 객체의 나이에 영향을 미치지 않습니다.

그러나 여러분은 자료들의 AGS 추적하고 싶은 때가 생길 것입니다. 예를 들

특정의 클래스에 대해 얼마나 많은 객체들이 여러분의 프로그램에서 만들어졌
입

지 알고 싶은 때가 있고, 또 아직도 남아있는 객체들은 몇 개인가 하는 등

변
리오
~

도

하나입니다. [리스트 14.1은 Cat 객체를 정적 자료 멤버 HowManyCace 선언하
였습니다, 이 WHE 얼마나 많은 car 객체가 만들어졌는지 추적합니다. 이는
적변수 80\0400`0#를 증가시킴에 의해 이루어지는데 생성자가 생길 때마다
가시키고 소멸자가 생길 때마다 하나씩 감소시킴니다.

[리스트 14.1] 정적 멤버 자료

1: 7/ [키스트 14.11 정적 멤버 자료
2:


===== PAGE 459 =====
제14일 특수 클래스와 함수들

ee 457

CONWU EW

WM:
12%
15:
14:
152
163
Ve
18%
19%
20:
215
222
25:
24:
29%
26:
27:
28:
29%
50:
31:
32:
$5:
34:
SDs
56:
50:
368:
59:

#include <iostream.h>

class Cat

<

public:
Cat(int age):itsAge(age){HowManyCats++; }
virtual ~Cat() { HowManyCats--; }
virtual int GetAge() { return itsAge; }
virtual void SetAge(int age) { itsAge = age; }
static int HowManyCats;

private:
int itsAge;

3;
int Cat::HowManyCats = 0;

int main()
t
const int MaxCats = 5;
Cat *CatHouse[MaxCats];
for (int i = 0; i<MaxCats; i++)
CatHouseLil = new Cat(it2);

for (i = 0; i<MaxCats; i++)

af
cout << "There are ";
cout << Cat::HowManyCats;   ERY Bz
cout << " cats left!\n";
cout << "Deleting the one which is ";
cout << CatHouseLil->GetAge();
cout <<" years old\n";
delete CatHouseLil;
CatHouseLil = 0;
0
return 0;

There are 5 cats left!
Deleting the one which is 2 years old
There are 4 cats left!
Deleting the one which is 3 years old
There are 3 cats left!
Deleting the one which is 4 years old


===== PAGE 460 =====
458 ee 제2주

There are 2 cats left!
Deleting the one which is 5 years old
There are 1 cats left!
Deleting the one which is 6 years old

way > - 17번 줄에서 간단한 Cat 클래스가 선언되었습니다. 128 줄에서
HowManyCats7} 정수형의 정적 멤버 변수로 선언되었습니다.

80\40000의 선언은 일반 정수형으로만 선언되지 않았습니다. 자유 기억 공간
이 별도로 설정되지 않습니다. 비정적 멤버 변수와 달리 Cat 객체를 인스턴스하
면서 자유 기억 공간이 설정되지 않습니다. 왜냐하면 HowManyCate 객체 안에
있지 않기 때문입니다. 따라서 19번 줄에서 변수가 정의되고 추기화되었습니다.

래스 안에서 정적 멤버 변수를 정의하지 않는 오류를 범할 때가 종종 있습
이런 일이 바로 여러분에게 일어나지 않도록 주의합시다. 물론 이런 오류를
생시키면 링커는 다음과 같은 오류를 발생시킬 것입니다.

세
=
타
HE
os

undefined symbol Cat::HowManyCats

여러분은 15&686에 대해 이렇게 할 BRE 없습니다. 왜냐하면 16486는 비정적 멤
버 변수이고 여러분이 매번 Cat 객체를 만들 때마다 정의되기 때문입니다. 여기
서는 26번 줄에서 이루어졌습니다.

Cato] 생성자는 정적 멤버 변수를 8번 SA 증가시켰고 9번 줄의 소멸자에서
감소시켰습니다. 따라서 어느 때라도 HowManyCats= 소멸되지 않은 Cato] 객체
수를 항상 가지고 있습니다.

21 - 40번의 프로그램에서 다섯 개의 Cas 인스턴스했고 각각을 배열에 넣었습
니다. 다섯 개의 생성자를 호출하고 HowManyCats= 처음의 0에서부터 다섯 번
증가가 일어났습니다.

그리고 프로그램은 현재의 ca 포인터를 삭제하기 전 MSS 순환하면서
HowManyCats= 출력합니다. 출력은 처음의 시작 ge] 5이고(이는 다섯 개가 생
성되었다는 뜻) 각 순환이 실행될 때마다 Cato] 하나씩 작아진다는 것을 보여줌
니다.

fowManyCasts 법융이고 1600이 의해 Aa eae Ad Fw Ae

은 이 변수를 이렇게 드러낼 필요는 없습니다. 여러분이 Cato] 인스턴스를 통해
접근하려면 다른 멤버 변수와 같이 전용으로 놓고 범용 접근자 ARES 제공하
는 것이 바람직합니다. 또 다른 한편으로 이 자료를 Cat AAS 유효하지 않게
하고 직접 접근하려면, 여러분은 두 개의 선택을 할 수 있습니다. [리스트 14.2]에


===== PAGE 461 =====
제14일 특수 클래스와 함수들 ㅎㅎ 459

서와 같이 범용으로 하거나 아니면 이번 장의 후반에 나오듯이 정적 멤버 함수를
제공합니다.

[리스트 14.2] 정적 멤버 HAS 객체 없이 접근하는 법

// 『리스트 14.21 정적 멤버 SAB 객체 없이 접근하

rir

=a)
=]

#include <iostream.h>

{

public:

9:

1

2

3

4:

5: class Cat
6:

7

8

CatCint age): itsAge(age) {HowManyCatst+; }

:    virtual ~“Cat() { HowManyCats--; }
10:   virtual int GetAge() { return itsAge; }
13   virtual void SetAge(int age) { itsAge = age; }
12:   static int HowManyCats;

13:

14: private:

15:   int itsAge;

16:

17: 33

18:

19: int Cat::HowManyCats = 0;

20:

21: void TelepathicFunction();
22:

23: int main()

24: £

25%   const int MaxCats = 5;

26:   Cat *CatHouse[MaxCats];

27:   for Cint i = 0; i<MaxCats; i++)
28:   af

29:      CatHouseLil] = new Cat(i);
50:     TelepathicFunction();
31:   +

52:

55°   for ( 1 = 0; i<MaxCats; i++)
54:   a

35:      delete CatHouseLlil;

36:     TelepathicFunction();
57%   D

58:   return 0;

59: +

40:

41: void TelepathicFunction()   번동 eer}


===== PAGE 462 =====
460

ee 제2주

겔과   There are

4231 <

43: cout << "There are ";

44: cout << Cat::HowManyCats << " cats alive\n";
45% >

cats alive

1
There are 2 cats alive
There are 3 cats alive
There are 4 cats alive
There are 5 cats alive
There are 4 cats alive
There are 3 cats alive
There are 2 cats alive
There are 1 cats alive
There are 0 cats alive

분석  [리스트 14.2]는 새로운 함수 TelepathicFunction()-S 추가시킨 점만 빼고 [리
=>

AE 14.1]과 GS 바가 없습니다. 이 함수는 Cat 객체를
객체를 매개 Wee 가지지도 않았는데 HowManyCatsS 멤버
있었습니다. 다시 한번 강조하건만 이 멤버 변수는 어느 특정 객체에도 있지 않
고 클래스 전반에 걸쳐 있으며 범용이면 프로그램 내의 아무 함수에서나 접근할
수 있습니다.

이 범용 멤버 변수를 다르게 만드는 방법의 하나는 전용으로 만드는
이렇게 하면 여러분은 멤버 함수를 통해 이를 접근할 수 있지만 그 클래스를 유
효하게 하는 객체를 가져야 합니다. [리스트 14.31을 봅시다. 정적 멤버 변수에 대
한 또 다른 선택이 [리스트 14.31을 분석한 후에 설명됩니다.

에

[리스트 14.3] 비정적 멤버 BAS 사응하여 정적 멤버 변수에 접근하기

1: // [리스트 14.3] 비정적 멤버 함수를 사용하여 정적 멤버 변수에 접근하기
fae

3: #include <iostream.h>

4:

5: class Cat                                                          ~
68 4

7: publics

8:    Cat(int age): itsAge(age) {HowManyCatstt+,; Bi

92    virtual ~Cat() { HowManyCats--; +

10:   virtual int GetAge() { return itsAge; }

11   virtual void SetAge(int age) { itsAge = age; 2

12:

virtual int GetHowMany ¢    return HowManyCats;

S&T      Tye


===== PAGE 463 =====
제14일 특수 클래스와      ee 461

0%
41>
min

1S
14:
15%
16:
ive
18:
19:
20:
218
228
Zor
24:
251
26:
Ze
28:
295
50;
318
52°
55%
34:
35.
361
of
38:
59%
40:
41:

private:  28,

int itsAge;

static int HowManyCats;
+; eee

int Cat::HowManyCats = 0;

int main()
{
const int MaxCats = 5;
Cat *CatHouse[MaxCats];
for (int i = 0; i<MaxCats; i++)
CatHouseLil = new Cat(i+2);

for (i = 0; i<MaxCats; i++)

ne
cout << "There are ";
cout << CatHouseli]->GetHowMany();
cout << '" cats left!\n";
cout << "Deleting the one which is ";
cout << CatHouseLil->GetAge()+2;
cout << '" years old\n";
delete CatHouseLil;
CatHouseLil = 0;

}

return 0;

}

100
ie

There are 5 cats left!
Deleting the one which is 2 years old
There are 4 cats left!
Deleting the one which is 3 years old
There are 3 cats left!
Deleting the one which is 4 years old
There are 2 cats left!
Deleting the one which is 5 years old
There are 1 cats left!
Deleting the one which is 6 years old

17번 줄에서 정적 멤버 변수 HowManyCats7} 전용 접근자를 가지도록 선언
되었습니다. 이 변수에 비정적 멤버 함수를 가지고 (전의 예제의

TelepathicFunction) 접근을 할 수 없습니다.


===== PAGE 464 =====
462 ㅇㅇ 제주

변수가 비록 정적으로 선언되었지만 아직은 클래스의 범위 내에 있습니다. 어떤
클래스 함수라도(예를 들면, GetHowMany) 이에 접근할 수 있습니다. 마치 ay
함수는 어떠한 멤버 변수라도 접근할 수 있듯이 말입니다. 하지만 GetHowMany(

DONT 정적 멤버 변수를 하나의 WHE 위한 자료 보관용으로 사용하지 Bret.
정전멘
on nD
MASE 클래스의 모든 객체 사이에서 공유됩니다.

정적 멤버 StA(Static Member Function)

정적 멤버 Ge 정적 멤버 변수와 비슷합니다. 단지 개체 내에서만 존재하는
것이 아니라 클래스의 범위 내예서 존제합니다 따라서 그 클래스의 객체 없이도

호출될 수 있습니다. [리스트 14.4에 있습니다.

[리스트 14.4] 정적 멤버 함수

// [리스트 14.43 정적 멤버 함수
#include <iostream.h>

1

2

3

4s

5: class Cat
6:

iti

8

t
public:
:    Cat(int age):itsAge(age){HowManyCats++; }
9:    virtual ~Cat() { HowManyCats--; }

10%   virtual int GetAge() { return itsAge; }

11:   virtual void SetAge(int age) { itsAge = age; }
13: private:

14:   int itsAge;

155   static int HowManyCats;

16: Je

tt:


===== PAGE 465 =====
463

18: int Cat::HowManyCats = OF
19:
20: void TelepathicFunction();
215
22: int main()
233
248   const int MaxCats = 5;
25°   Cat *CatHouse[MaxCats];
26:   for (int i = 0; i<MaxCats; i++)
20:   {
28:      CatHouseLil] = new Cat(i);
29:     TelepathicFunction();
3058   }
S12
Se:    for ( 1 = O; i<MaxCats; i++)
338   £
SKE      delete CatHouseLil;
55°     TelepathicFunction();
36:   }
Sti   return 0;
38: 3}
39:
40: void TelepathicFunction()
415 £
42:   cout << "There are" << Cat: :GetHowMany() << " cats alive\n";
43: 3                  a
ing  There are 1 cats alive
There are 2 cats alive
There are 3 cats alive
There are 4 cats alive
There are 5 cats alive
There are 4 cats alive
There are 3 cats alive
There are 2 cats alive
There are 1 cats alive
There are 0 cats alive

(rag

정적 멤버 변수 HowManyCats7} 15번 줄의 Cato] 선언부에서 범용 접근자

를 가지도록 선언되었습니다. 범용 접근 함수 GetHowMany(7} 12번 줄에서

범용이면서 정적 멤버 함수로 선언되었습니다.

GetHowManyQS 범용이므로 어떤 함수에 의해서도 접근될 수 있습니다. 또 정적
「       ae      i ee

멤버 함수이므로 SSS 위해 CatYo] 객체를 가질 이유가 없습니다.


===== PAGE 466 =====
464 ee R24

42번 줄에서 함수 TelepathicFunction(}°] Cat 객체를 접근함이 없이 범용 정적 접
aye 접근할 수 있습니다. 물론 여러분은 다른 접근 함수처럼 mainO 안에서 유

효한 Cat 객체에 GetHowMany0S 호

ah

hed

4y fe
xo,

xo

tly
ef
Ea)

여러분은 정적 멤버 함수를 마치 일반 멤버 함수처럼 클래스의 객체 상에서 호출하여 접근
4   브르

oh
>
zo
피>
때
fa
fob
rlo
2
모
rt
rlo
mu
고
\>
ia
고
고
으
ol
ilo
Oly
AC
oh
+)
Pal
2
I
In
.보
고
gO
oO

class Cat
4
public:
staric int GetHowMany() { return HowManyCats; +
private:
static int HowManyCats;
3;
int Cat::HowManyCats = 0;

void main()

a
int howMany;
CAT theCat;// define a cat
howMany = theCat.GetHowManyQ;// access through an object
howMany gears tel 7 7 access without an object
}                                         Nee



===== PAGE 467 =====
제14일 특수 클래스와 함수들 ㅇㅇ 465

이 방법은 매우 유용합니다. 이는 여러분의 입력 내용에 따라 마음대로 함수를
호출할 수 있습니다.

함수에 대해 단 하나의 까다로운 YRS 포인트되는 객체에 대한 형입니다. 파형
을 포인트하는 포인터는 정수형을 가리키고 Yo] 대한 포인터는 해당 반환형과
원형부를 지닌 함수를 포인트합니다.

re
[오
-ㅁ
=z
x

long (*funcPtr) (int);

라고 했으면 funcPtre 정수형 매개 변수와 1008를 반환

40006 QI) BR) BAO, AGS AGT Ue 경우 다 Peay
높은 때가 먼저 함수명에_달라붙기 때문입니다. 만일 괄호

정수형을 가지고 1008형 포인터를 반환하는 함수의 선언으로 간주될 것입니다.

(여기서 공백 문자는 의미가 없습니다.)

다음의 두 개의 선언을 살펴봅시다.
Un

long * /Function WP ;
tong (*funcPtr) (int) ;

Al 번째의 80000000은 정수형을 가지고[008형의 변수의 포인터를 반환하는 함수
대

입니다. 두.번째의 funcPtre 정수형을 가지고    영 변수를 반환하는 함수어

포인터 함수의 선언은 반환값과 매개 변수를 집어넣는(물론 매개 변수가 있는 경
우에만 넣습니다.) BSS 가집니다. [리스트 14.5]를 살펴봅시다.

a

[리스트 14.5) Bt 포인터

// [리스트 14.5] 함수 포인터

#include <iostream.h>

void Cube (1018, int&);
void Swap (int& int &);

: void GetVals(int&, int&);
9: void PrintVals(int, int);
10: enum BOOL { FALSE, TRUE };
a
12: int main()

158 ¢

1

2

3

4:

5: void Square (int&,int&);
6:

7

8


===== PAGE 468 =====
466 ec 제2주

14:   void (* pFunc) (int &, int &);
15:   BOOL fQuit = FALSE;

16:

17:   int valOne=1, val Two=2;

18:   int choice;

19: while (fQuit == FALSE)

20:   {

218      cout << "(0)Quit (1)Change Values (2)Square (3)Cube (4)Swap: ";
22:      cin >> choice;

235%      switch (choice)

24:     {

25        case 1: pFunc = GetVals; break;
26%        case 2: pFunc = Square; break;
27:        case 3: pFunc = Cube; break;
28:        case 4: pFunc = Swap; break;
295        default: fQuit = TRUE; break;
30:     }

31:

32:     if (fQuit)

33:        break;

34:

55:      PrintVals(valOne, valTwo);

36:      pFunc(valOne, v

3(:      PrintVals(valOne, valTwo);

358:   y

39:   return 0;

40: }

41:

42: void PrintVals(int x, int y)

435: {

44: cout << "x: " << x <<" ys " << y << endl;
45: +

46:

47: void Square (int & rX, int & rY)

48: {

49: rX *= 7X;

50: ryY *= ry;

51: 2

52:

53: void Cube (int & rX, int & rY)
54: {

52°) Ant tmp;

56:

57: tmp = rX;

58: rX *= 7X;

59: rX =rX * tmp;



===== PAGE 469 =====
60:
61:
62:
63:
64:
65:
66:
67:
68:
69:
(0%
18
721
73%
74:
tas
16:
(C:
78:
19:
80:

tmp = rY;

rY *= rY;

rY =rY * tmp;
}

void SwapCint & rX, int & ry)
{

int temp;

temp = rX;

CX = FY?

rY = temp;

}

void GetVals (int & rValOne, int & rValTwo)
{

cout << "New value for ValOne: ";

cin >> rValOne;

cout << "New value for ValTwo: ";

cin >> rValTwo;

B:

(naa

1444

하는

(O)Quit (1)아3096 Values (22)650420『6 (3)Cube
xt 2

New value for ValOne: 2

New value for ValTwo: 3

Xx 2 Yes

(O)Quit (1) Change Values (2)Square (3)Cube
xi2 ye 3

x: 8 ye 27

(O)Quit (1)Change Values (2)Square (3) Cube
X28 ye 27

x: 64 y: 729

(O)Quit (1) Change Values (2) Square (3)Cube
x: 64 y: 729

x: 729 >: 64

(O)Quit (1)Change Values (2)Square (3)060066 (4) Swap:

(4) Swap:

(4) Swap:

(4) Swap:

(4) Swap:

0

5-84 줄에서 4개의 함수가 선언되었는데, 각각 같은 반환형과 원형부를 가
지는데, 전부 1000값을 반환하고 두 개의 정수형 참조자를 가집니다.

줄에서 pFunc= 두 개의 정수형 BAAS 매개 변수로 가지고 100를 반환

조
황수를 가리키는 포인터로 선언이 되었습니다. 앞의 4개의 합
용

+= pFunc

에 의해 포인트될 + 있습니다. 사용자는 계속적으로 함수를 선택하고 pFunc7}


===== PAGE 470 =====
한 현재의 go] 출력되

on
\o
Hu
muh
of
rit,
ate;
+o

. 35 - 37H 줄에서 두 개의 정수에 대
가 불려지며 값들이 다시 출력됩니다.

2
그
es
Hel
[으
모

는 함수 이름 대신 함수에 대한 포인터가 사용된다는 점을 제외하고는

함수 포인터에 치환할 때는 함수 이름만을 매개 변수 없이

Long (*pFuncOne) (int, int)
Long SomeFunction (int, int)
pFuncOne = SomeFunction;
pFuncOne(5, 7)

함수 포인터를 사용하는 이유

여러분은 [리스트 use 함수 포인터를 사용하지 않고 쓸 수도 있습니다. 하지
끄

x
만 함수 포인터를 RE 것이 맘대로 할 수 있고 또 프로그램이 명확하게 됩니다.

[리스트 14.6|은 함수 원형과 정의를 [리스트 14.5]와 같이 쓰지만 프로그램의 몸
개         °.

제부분에서는 함수 포인터를 쓰지 않습니다. 이 두 개의 예제의 차이점을 잘 살
봅

이 프로그램을 컴파일하려면 [리스트 14.5]의 41-79번 SS 55번 줄 다음에 가져다 놓
습니다.

[리스트 14.6] [리스트 14.5] 프로그램을 함수 포인터 없이 다시 작성한 예제

1; // [리스트 14.63 [리스트 14.57 프로그램을 함수 포인터 없이 다시 작성한 예제
2: // [리스트 14.53의 PrintVals, Square, Cube, Swap, GetVals 함수 본체는 생략
3: #include <iostream.h>


===== PAGE 471 =====
제14일 특수 클래스와 함수들 ee 469
4:
5: void Square (int&,int&);
6: void Cube (1018, int&);
7: void Swap (1018, int &);
8: void GetVals(int&, int&);
9: void PrintVals(int, int);
10: enum BOOL { FALSE, TRUE };
118
12: int main()
131 6
14:   BOOL fQuit = FALSE;
15:   int valOne=1, valTwo=2;
16:   int choice;
178   while (fQuit == FALSE)
18:   {
195     cout << "(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: ";
20:      cin >> choice;
21:      switch (choice)
22:      {
25°         case 1:
24:          PrintVals(valOne, valTwo);
25:          GetVals(valOne, valTwo);
26:          PrintVals(valOne, valTwo);
27:          break;
28:
29:        case 2:
50:          PrintVals(valOne, valTwo);
313          Square(valOne, valTwo);
S22          PrintVals(valOne, valTwo);
35:          break;
34:
351        case 3:
36:          PrintVals(valOne, valTwo);
ot?          Cube(valOne, valTwo);
38:          PrintVals(valOne, valTwo);
39:          break;
40:
41:        case 4:
42:          PrintVals(valOne, valTwo);
43:          Swap(valOne, valTwo);
44:          PrintVals(valOne, valTwo);
45:          break;
46:
47:        default :
48:           fQuit = TRUE;

49:           break;


===== PAGE 472 =====
470 ee Haz

50:     }

D1:

D2:      if (fQuit)
535        break;
54:   }

55: return 0;

56: 3

겔과 (O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 1
xe 1 oye 2
New value for ValOne: 2
New value for ValTwo: 3
x22 yes 3
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 3
xi2 yi 5
xe 8 yz 27
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 2
x: 8 y: 27
xr 64 ys 729
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 4
x: 64 ys: 729
x: 729 ys 64
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 0

이 함수의 구현은 [리스트 14.5|와 같으므로 빠졌습니다. 보다시피 결과는

같습니다. 그러나 함수의 SAE 27줄에서 38줄로 확장되었습니다.
PrintVals(o] 대한 SO] 각 0856문에서 반복되어야 합니다.

(a
iz

PrintValsQte-& whilett2] 꼭대기와 밑부분에 각각 넣고 싶은 ee  생기겠지만

0856문을 빠져나가는 경우에도 200[8150를 호출하게 되므로 정답이 아닙니다.

코드 량이 늘고 또 같은 것을 여러 번 호

어졌습니다. 여기서는 단지 어떻게 함수 포인터가

위함입니다. 실제 프로그램 세계에서 함수 포인터를 쓰는 것은 이점이 많습니다.
See en =

함수 포인터는 재생되는 코드 량을 엄청 Se 것이고 프로  wea 더욱 깔끔히

게 해주며 함수 테이블을 만들어 놓고 실행할 때ㅁ

니다.



===== PAGE 473 =====
간단한 호출
여러분 맘대로 이지만, 함수 포인터는 참조될 필요가 없습니다. 따라서, 만일 pFunc7t 함
수 포인터이고 정수형 매개 HES 취하고 1070형을 반환한다면, 여러분은 해당되는 함수
를 pFuncS 다음의 두 가지 HHS 써서 함수를 호출할 수 있습니다.

pFunc(x);

(xpFunc) (x);
두 개는 서로 같습니다. 전자는 후자의 간단한 표현입니다.

정수형에 대한 배열을 선언하듯이 여러분은 반환값과 원형부가 똑같은 함수들의
배열을 만들 수 있습니다. [리스트 1472 [리스트 US 배열을 다시 사용하여
작성하였습니다

이 프로그램을 컴파일하려면 [리스트 14.5]의 41-79번 SS 38번 줄 Sec (FE 놓
습니다

[리스트 14.7] 함수 포인터의 배열을 사응한 of

// [리스트 14.71 함수 포인터의 배열을 사용한 에
// (®|AE 14.5]9| PrintVals, Square, Cube, Swap, GetVals 함수 본체는 생략
#include <iostream.h>

1

2

3

4:

5: void Square (int&,int&);
6: void Cube (1018, int&);

7: void Swap (1018, int &);
8: void GetVals(int&, int&);
9: void PrintVals(int, int);
10: enum BOOL { FALSE, TRUE };
11:

12: int main()

1s: ¢

14:   int valOne=1, valTwo=2;
15:   int choice;

16:   const MaxArray = 5;

17:   void (*pFuncArray[MaxArray]) (int&, int&);
18:


===== PAGE 474 =====
472 ee 제2주

193   for (int 1=0;i1<MaxArray;i++)

20:   {
Zl:      cout << "(1)Change Values (2)Square (3)Cube (4)Swap: ";
22:      cin >> choice;
25:      switch (choice)
24:      {
2a:        case 1:pFuncArrayLil = GetVals; break;
26:        case 2:pFuncArrayLil = Square; break;
2s        case 3:pFuncArrayLil = Cube; break;
28:        case 4:pFuncArrayLil = Swap; break;
29:        default:pFuncArrayLlil = 0;
30:     }
51%   3
52%
55:   for (i=0;1<MaxArray; i++)
34:   {
So:      if ( pFuncArrayLil] == 0 )
363        continue;
Sts     pFuncArrayLil(val0ne,valTwo);
38:     PrintVals(valOne,valTwo) ;
59:   }
40: return 0;
41: }
a    (1) Change Values (2)Square (3)Cube (4) Swap:

(1) Change Values (2)Square (3)Cube (4) Swap:
(1)Change Values (2)Square (3)Cube (4)Swap:
(1)Change Values (2)Square (3)Cube (4) Swap:
(1)Change Values (2)Square (3)Cube (4)Swap:
New Value for ValOne: 2

New Value for ValOne: 3

xe 2083

Say: 9

: 64 y: 729

: 729 y: 64

: 531441 y: 4096

불셀 다시 한 번 한수의 구현 부분은 지면 절약을 위해 일부러 빠뜨렸습니다. 17
번 줄에서 pFuncArray7} voids 반환하고 두 개의 정수형 참조자를 취하는
5 개의 함수 포인터 배열로 선언되었습니다.
19 - 31번 줄에서 사용자들은 원하는 함수를 선택하고 각 배열의 We 적절한
함수의 포인터를 받습니다. 33-39번 줄에서 각 함수가 차례로 호출되고 결과가 각
각 출력됩니다.

6890 에 에 00 =

x «x >×>×


===== PAGE 475 =====
제14일 특수 클래스와 He ee 473

함수 포인터를 다른 함수에 전달하는 방법
더 포인터(또는 그런 식의 배열)는 다른 함수에 ASS 수 있는데, 이때에도 =
는 원하는 대로 동작합니다.

선택된 함수 포인터를 2800 바깥의 다른 함수로 전
 호출하고 값을 ag  수 있습니다. [리스트 14.8]의 변형된 모습

주의
이 프로그램을 컴파일하려면 [리스트 14.5]의 41-79번 줄을 44번 줄 다음에 가저다 놓

[리스트 14.8] 함수 포입터를 함수의 매개 AAS 전달하는 방법

// [리스트 14.8] 함수 포인터를 함수의 매개 HAR 전달하는 방법
// [리스트 14. 5]2} Square, Cube, Swap, GetVals 함수 본체
#include <iostream.h>

생략

rir

void Square (int&,int&);

void Cube (1018, int&);

void Swap (1018, int &);

void GetVals(int& int&);

void PrintVals(void (*)(int& int&),int&, int&);
10: enum BOOL { FALSE, TRUE };

VAs

12: int main(Q)

133. +

14:   int valOne=1, val Two=2;

15%   int choice;

16:   BOOL fQuit = FALSE;

1

183   void (*pFunc) Cint&, int&);

19:

20:   while (fQuit == FALSE)

21%   x

22:      cout << "(Q)Quit (1)Change Values (2)Square (3)Cube (4)Swap: ";
238      cin >> choice;

24:      switch (choice)

2591     {

26:        case 1:pFunc = GetVals; break;
C03        case 2:pFunc = Square; break;
20%        case 3:pFunc = Cube; break;

CONOU RP WD =
… … …ㅁ…… …… 0… … …… …

Se)


===== PAGE 476 =====
474 66 제2주

29:        case 4:pFunc = Swap; break;

30:        default:fQuit = TRUE; break;

31:     }

52:      if (fQuit == TRUE)

33:        break;

34:      PrintVals (une) valOne, valTwo);
SD!   가

36:

37: return 0;

38: }

59:

40: void PrintVals( void (*pFunc) (int&, int&),int& x, int& y)
412 ¢

42: cout << "x: "<< x << "yr " << y << endl;
43:   pFunc(x,y);

44:    cout << "xs "<< x <<“ ys " << y << endl;
45: }

겔과  (O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 1
xi1 yie
New value for ValOne: 2
New value for ValTwo: 3
xi2 ys
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 3
Xe 2 yes
x: 8 y: 27
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 2
Xx? 8 ye 27
x64 15729
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 4
x964 ys 729
x:2729 y:64
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 0

18번 줄에서 pFunct= voidgS 반환하고 두 개의 정수형 참조자를 취하는
함수에 대한 포인터로 선언되었습니다. 9번 Sold PrintVals= 3 개의 매개
취하는 함수로 선언되었습니다. A 번째 매개 변수는 700형을 반환하고

수형 참조자 매개 변수를 취하는 함수에 대한 포인터이고, 두 번째 변
와 세 번째 인수는 정수형 참조자입니다. 사용자는 선택할 함수를 정하고 34번
에서 PrintVals7} 호출됩니다.

위 도사라고 자처하는 CH 프로그래머를 찾아가 다음 So] 무엇을 의미하는지
봅시다.

(ag
iz

고 >
vo

md ky oN Sy St 포

“2


===== PAGE 477 =====
제14일 특수 클래스와 함수들 ee 475

ra pavers, ae a 사용.

이 선언은 여러분이 잘 사용 안하면서 필요할 땐 책에서 찾아보는, 그러나 정작
필요한 곳에서는 여러분의 코드량을 확 줄여주는 아주 드문 종류의 선언입니다.

void (id, 1049 FEE 잘 봐권야 하는 따분한 구문입니다 tate  이
단히 하기 위해 62608문을 쓸
의 정수형 참조자를 취하는 함수 포인터의 형으로 선언하는 가 [리스트
찌아 고

14.이는 [리스트 14.8]을 17260하문을 써서 다시 작성한 것 입니다.

|

[리스트 14.9] 함수 BHO 가독성을 높이기 HoH typedefS 사응한 of

// [리스트 14.91 함수 포인터의 가독성을 높이기 위해 typedet 사용한 예
// [리스트 14.5]의 Square, Cube, Swap, GetVals 함수 본체는 생략
#include <iostream.h>

void Square (int&,int&);

void Cube (int&, int&);

void Swap (int&, int &);

void GetVals(int&, int&);
typedef void (*VPF) (1018, 1018) ; \/
10: void PrintVals(VPF,int&, 1018);
11: enum BOOL { FALSE, TRUE };

12:

13: int main()

14: {

155   int valOne=1, valTwo=2;

16:   int choice;

17   BOOL fQuit = FALSE;

CONDWU FWD =
… … 00 00 00 00 00 ㅣㅁ…

‘Oo

18:

20: ‘

216   while (fQuit == FALSE)

225   nf

23:      cout << "(O)Quit (1)Change Values (2)Square (3)Cube (4) Swap: ";
24:      cin >> choice?

252      switch (choice)

26:      {

er:        case 1:pFunc = GetVals; break;
28:        case 2:pFunc = Square; break;
29:        case 3:pFunc = Cube; break;


===== PAGE 478 =====
476 ee 제2주

30:        case 4:pFunc = Swap; break;

B15        default:fQuit = TRUE; break;

52:      }

333      if (fQuit == TRUE)

34:        break;

351      PrintVals ( pFunc, valOne, valTwo);
36:   Bs

37: return 0;

38: 3

598

40: void PrintVals( VPF pFunc,int& x, int& >)
418 세

42:    cout << "x: "<< x << "yi " << y << endl;
43:   pFunc(x,y);

44:    cout << "x: " << x <<" ys " << y << endl;
45: }

24 Di  (O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 1
x 1 ys"
New value for ValOne: 2
New value for ValTwo: 3
xe 2 s
(O)Quit (1) Change Values (2)Square (3)Cube (4)Swap: 3
Xe 2 y¥2 Ss
Ki B yt 27
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 2
xe 8 ys 27
xs 64 ye 729
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 4
x: 64 y: 729
x 729 ys 64
(O)Quit (1)Change Values (2)Square (3)Cube (4)Swap: 0

ox
i

= ai  9번 SoA] typedef7} 사용되었는데, VPFS 1010형을 반환하고 두 개의
형 참조자를 매개 변수로 취하는 함수로 선언하였습니다.
10번 줄에서 200[8150는 세 개의 매개 변수를 취하는데 VPFS} 두 개의 정수형
참조자를 갖습니다. 19번 줄에서 pFunc= \0"형으로 선언되었습니다.
일단 빼형이 정의된 후, pFuncs} PrintVals) 선언이 훨씬 말끔해졌습니다. 보다
시피 출력은 같습니다.


===== PAGE 479 =====
멤버 함수에 대한 포인터

여태까지의 포인터, 여러분이 만든 모든 함수 포인터는 일반적인 형의 포인터, 즉
비클래스 함수입니다. 클래스 wey 함수의 포인터를 만드는 것도 가능합니다.
멤버 함수 포인터를 만드

클래스 이름과 범위 연산자(::)를 사용합니다. 따라서 만일 pFunc7} 1010형을

단                 연
반환하고 두 개의 정수형을 취하는 Shape 클래스의 why 함수 포인터가 되려면,
선언은 다음과 같이 됩니다.

void (Shape::*pFunc) (int, Tint)?

멤버 함수 포인터는 함수 포인터와 같은 방식으로 사용합니다. 단 호출 시마다
정확한 클래스의 객체를 필요로 합니다.

[리스트 14.10|은 멤버 함수 포인터의 사용법을 보여줍니다.

[리스트 14.10] 멤버 함수에 대한 포인터

// [리스트 14.10] 멤버 함수에 대한 포인터

#include <iostream.h>

class Mammal

nf

: public:

9:    Mammal ():itsAge(1) { }

10:   ~Mammal() { 3

118   virtual void Speak() const = 0;
12:   virtual void Move() const = 0;
13: protected:

14:   int itsAge;

1

2

3

ae

5: enum BOOL {FALSE, TRUE};
6:

7

8

ㆍ Vhs de

165

17: class Dog : public Mammal

18: £

19: public:

205   void Speak()const { cout << "Woof!\n"; }

21s   void Move() const { cout << "Walking to heel...\n"; }
225 33                                                   '
25°

24:

25: class Cat : public Mammal



===== PAGE 480 =====
478 eo 제2주

268

271 public:

28:   void Speak()const { cout << "Meow!\n"; }
29:   void Move() const { cout << "slinking...\n"; }
30: 3;

312

52%

33: class Horse : public Mammal

34:-¢

35: public:

36%   void Speak()const { cout << "Winnie! \n"; }
37,   void Move() const { cout << "Galloping...\n"; }
38, +:

59°

40:

41: int main®

42: ¢

435:   void (Mammal::*pFunc)() const =0;

44:   Mammal* ptr =0;

45%   int Animal;

46:   int Method;

47:   BOOL fQuit = FALSE;

48:

49:   while (fQuit == FALSE)

50:   {

bit      cout << "(O)Quit (1)dog (2)cat (3)horse: ";
52:      cin >> Animal;

53%      switch (Animal)

54:      {

55:        case 1: ptr = new Dog; break;

56:        case 2: ptr = new Cat; break;

573        case 3: ptr = new Horse; break;

58:        default: fQuit = TRUE; break;

59%      }

60:      if (fQuit)

61:        break;

62:

63:     cout << "(1)Speak (2)Move: ";

64:      cin >> Method;

65%      switch (Method)

66:      {

Of:        case 1: pFunc = Mammal::Speak; break;
68:        default: pFunc = Mammal::Move; break;
69:      }

(0%

112      (ptr->*pFunc) ;


===== PAGE 481 =====
제14일 특수 클래스와 함수들 ee 479

(22      delete ptr;
13%   3

ae   return 0;

751 고

겔과  (Q)Quit (1)Dog (2)Cat (3)Horse: 1
(1)Speak (2)Move: 1
Woof!
(Q)Quit (1)Dog (2)Cat (3)Horse: 2
(1) Speak (2)Move: 1             :
Meow!
(Q)Quit (1)Dog (2)Cat (3)Horse: 3
(1)Speak (2)Move: 2
Galloping...
(Q)Quit (1)Dog (2)Cat (3)Horse: 0

4  6-15번 줄에서 추상 자료형 Mammalo] 두 개의 순수 가상 w= Speak()34}

Move) 써서 선언되었습니다. Mammal? 다시 각각 976400와 Move()=
재생하는 208, Cat, Horse! 클래스로 분류되었습니다.

55-57번 줄에서 구동 프로그램 0800은 사용자에게 어떤 Bo] SHS 만    “ll
지 선택하게 하고, Animale] 대한 새로운 하위 클래스가 자유 기억 장소에 만들
어져 28000에 할당됩니다.

사용자는 어떤 메쏘드를 호출할지를 선택하게 되고, 메쏘드는 포인터 pFuncel] 할
당됩니다. 71번 줄에서 선택된 메쏘드가 만들어진 객체에 의해 선택되는데, 객체
에 접근하기 위해 00 포인터를 사용하고 또 함수에 접근하기 위해 prunes 사용
합니다.

마지막으로 72번 줄에서 [에 대해 해당 LS 자유 기억 공간에 되돌려주기
위해 delete7} 호출됩니다. pFunco] 대해서는 06606를 호출할 필요가 없는데, 왜냐
하면 이는 코드에 대한 포인터이지 자유 기억 공간 상의 객체가 아니기 때문입니
다. 이렇게 하면 컴파일러 오류가 남니다.

00

만들  것인

더

멤버 함수 포인터에 대한 배열
함수 포인터와 같이 멤버 함수 포인터도 배열에 저장될 수 있습니다.

배열은 각 멤버 함수의 주소로 초기화될 수 있고 각 배열의 변위에 의해 호출됩
니다. [리스트 14.111이 이 기술들을 보여줍니다.



===== PAGE 482 =====
480 ee 제2주

[리스트 14.11] 멤버 함수 포인터의 배열

// CRAE 14.111 멤버 함수 포인터의 배열

#include <iostream.h>

4
2
3
4:
5: enum BOOL {FALSE, TRUE};
6
7: class Dog

Se t

9: public:

10:   void Speak()const { cout << "Woof!\n"; 개

118   void Move() const { cout << "Walking to heel...\n";

12:   void Eat) const { cout << "Gobbling food...\n"; +

152   void Growl() const { cout << "Grrrrr\n"; +

14:   void Whimper() const { cout << "Whining noises...\n"; }

ied   void RolLOver() const { cout << "Rolling over...\n"; +

16: void PlayDead() const { cout << "Is this the end of Little Caeser?\n"; }
1733)

18:

19: typedef void (Dog::*PDF) (const ;

20: int main

218 <

22:   const int MaxFuncs = 7;

23:   PDF DogFunctions[MaxFuncs] =

24:   { Dog::Speak,

20:     Dog: :Move,

26:     Dog: :Eat,

2c     Dog::Growl,

28:     Dog::Whimper,
29:     Dog::RollOver,
30:      Dog::PlayDead };
S15

32:   Dog* pDog =0;
595:   int Method;
54?   BOOL fQuit = FALSE;

35:

36:   while (!fQuit)

Sts   본

38¢      cout << "(O)Quit (1)Speak (2)Move (3)Eat (4)Growl";
59:      cout <<" (5)Whimper (6)RoLL Over (7)Play Dead: ";
40:      cin >> Method;

aie      if (Method == 0)

42:      {

43:        fQuit = TRUE;

44:        break;


===== PAGE 483 =====
제14일 특수 클래스와 함수들 ㅎㅇ 481

|
18

45:     }
46:     else
47:      {
48:        pDog = new Dog;
49:        (pDog->*DogFunct ions[Method-1]) () ;
50:        delete pDog;
51:     0
52:   +
53: return 0;
D4: 2
a   (O)Quit (1)Speak (2)Move (3)Eat (4)Growl (5)Whimper (6)RoLL over

(7)Play Dead: 1

Woof!

(O)Quit (1)Speak (2)Move (3)Eat (4)Growl (5)Whimper (6)RoLL over
(7)Play Dead: 4

Grrrr

(O)Quit (1)Speak (2)Move (3)Eat (4)Growl (5)Whimper (6)RoLL over
(7)Play Dead: 7

Is this the end of Little Caeser?

(O)Quit (1)Speak (2)Move (3)Eat (4)Growl (5)Whimper (6)RoLL over
(7)Play Dead: 0

7 - 17H 줄에서 Dog 클래스가 선언되었고, 같은 형을 반환하고, 같은 사용
을 가진 7개의 멤버 함수가 만들어졌습니다. 19번 Solr] typedef7} PDE

매개 Wee 없고 반환값도 없는 그리고 상수형인 Dog 멤버 함수 포인터로
언시켰습니다.

- 30번 줄에서 DogFunctions7} 7개의 멤버 함수를 가지고 각각의 함수 주소로
eee
38, 39번 줄에서 사용자는 메쏘드를 선택합니다. Quits 선택하지 않는 한 새로운
Doge] 힙에 만들어지고 원하는 메쏘드가 49번 So] 배열 상에 호출됩니다. 여기
또 C++ 도사에게 물어볼 좋은 예제가 하나 생겼습니다.

rx fe

be

r

(pDog->*DogFunct ion[Method-11]) ();
——ahahe_eo oo See”

이것은 또 또 다른 비법인데, 여러분이 wy 함수로부터 만들어진 테이블을 필요로
할 때 여러분의 프로그램을 훨씬 이해하기 쉽고 읽기 쉽게 만들 것입니다.



===== PAGE 484 =====
482 ee 제2주

dD
DON'T 아주 간단한 방법이 있을 때 멤버 함수 포인터는 사용하지 ate.

요와

오늘 학습에서 정적 멤버 변수를 만드는 법을 배웠습니다. 각 클래스는 (각 객체
가 아니라) 그 정적 멤버 변수의 인스턴스를 가지고 있습니다. 이 멤버 변수에 클
래스의 객체를 만들지 않고도, 이름을 완전하게 주면 접근을 할 수 있습니다. 몰
론 정적 We 범용 접근자로 선언되어 있어야 합니다

정적

왜냐하면 정적 멤버 변수는 각 객체의 부분이 아니며 메모리를 할당받지 않고,

멤버 변수는 클래스의 인스턴스에 관계없이 계산기로 사용될 수 있습

무

또 클래스의 바깥 부분에서 정의되고 초기화되어야 하기 때문입니다.

정적

래스의 특정 객체 부분 없이 접근되며 정적 wy 자료에 접근할 수 있습니다.
적 멤버 함수는 비정적 멤버 자료를 접근할 때 쓰일 수 없는데, 왜냐하면 005

N
로

멤버 함수는 정적 멤버 변수와 같은 방식으로 클래스의 한 부분입니다.

d

tl om! 때

인터가 없기 때문입니다.

정적

기 때문
const= this 포인터가 0009[임을 나타내는 멤버 함수

멤버 함수는 this 포인터를 안 가지기 때문에 conte 만들 수 없습니다.

에
입니다.

함수 포인터와 멤버 함수 포인터의 선언 및 사용법도 배웠습니다. 이 포인터들에
대한 배열 및 함수에 전달하는 방법도 배웠습니다.

함수 포인터와 멤버 함수 포인터는 실행시 선택될 수 있는 함수의 테이블을 만드
는데 사용될 수 있습니다. 이렇게 하면 포인터 없이 사용할 때보다 훨씬 여러분
의 프로그램에 SERS 부여할 수 있습니다

전역 자료를 쓸 수 있는데 정적 자료를 사용하는 이유는 무엇입니까?
클래스

스 내의 범위에서 쓸 수 있습니다. 따라서 정적 자료는 단지 클래

스의 객체를 통해서만 유용합니다. 범용이면 클래스명을 사용한 명시적 호출을 통


===== PAGE 485 =====
제14일 특수 클래스와 함수들 eo 483

해 사용 가능하며 혹은 정적 멤버 함수를 사용하여 가능합니다. 정적 자료는 클
스형에 맞춰져야 하는데, 제한된 접근과 강형이라는 점 때문에 전역 변수보다 안전
합니다.

전역 함수를 사용할 수 있는데 정적 멤버 함수를 사용하는 이유는 무엇입니까?

A 정적 멤버 함수는 클래스 내에서 사용할 수 있습니다. 따라서 클래스의 객체를 사
용하여 호출되거나 혹은 명시적으로 명확하게 사용(186944006:0000000443006())해야
합니다.

Q 함수 포인터 혹은 멤버 함수 포인터를 사용하는 AS 흔합니까?

A 아닙니다. 특정한 용도로 사용

경

로그램조차 쓰지 않는

연구

이 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가
를 확인해 보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어
있습니다. 부록 De 있는 답을 보기 전에 각 물음에 대답할 수 있도록 노력하고,
다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다.

퀴즈

1 정적 We 변수는 전용으로 될 수 있습니까?
2. 정적 멤버 변수를 선언하여 봄시다
3. 정적 ae] 함수를 선언하여 봄시다

4 10170형을 반환하고 하나의 정수형 매개 변수를 취하는 함수 포인터를 선언하여 봅시다.
5. 4번의 함수를 Car 클래스 멤버 BS 가리키는 포인터로 고쳐 봅시다.
6 5번의 정의를 10개의 포인터 배열로 확장하여 봄시다.

연습 문제

1. 하나의 멤버 변수와 하나의 정적 멤버 변수를 가지는 클래스를 선언하는 짧은 프로그램
을 작성하십시오. 생성자가 멤버 변수를 초기화하고 정적 멤버 변수를 증가시키도록 하
십시오. 소멸자가 멤버 변수를 감소시키도록 하십시오.

로그램을 사용하여 3개의 객체를 만들고 각각의 멤버 변수와 정적 멤버 변수를
한 프로그램을 작성하십시오. 다음

iz
력           프
변수에 대한 SHS 조사하십시오.

24
각각의 객체를 소멸시키고 정적 멤버



===== PAGE 486 =====
484 ee 제2주

3. 2번 연습의 프로그램을 정적 멤버 변수를 접근하는 정적 멤버 함수를 사용하여 수정하십
시오. 정적 멤버 변수를 전용으로 선언하십시오.

4. 3번 연습에서 비정적 멤버 변수를 접근하는 멤버 함수 포인터를 작성하십시오. 그리고
그 자료의 값을 출력하는 포인터를 사용하십시오.

5. 전번 문제에서 클래스에 두 개 이상의 멤버 변수를 추가하십시오. 이 Hes 얻는 접근
자 함수를 만들고 모든 멤버 함수에게 같은 값과 사용법을 주도록 하십시오. 이 함수들
에 접근하기 위해 멤버 함수 포인터를 사용하십시오.


===== PAGE 487 =====


===== PAGE 488 =====
486 eo 제2주

연결 리스트를 사용, 가상 함수, 순수 가상 함수, 함수 재생, 다형성, 범용 상속,
함수 중첩, 무한 순환, 포인터들, 참조자들 그리고 기타 등등입니다

이 프로그램의 주된 목적은 연결 리스트를 작성하는 것입니다. 이 리스트의 노드
들은 공장에서 쓰일 각 부분들을 가지고 있습니다. 비록 이러한 것이 이 프로그
램의 최종본은 아니지만 비교적 상당한 자료 구조의 좋은 예를 보여줍니다. 전
코드 량은 300줄 정도입니다. 출력 뒤에 나오는 BAS 읽기 전 여러분 스스로
이 코드들을 분석하여 봅시다.

[리스트 02.1] 둘째 주 복습 목록

0:  fj 고 고고고 KKK KKK KEKE KEKE KERR KKK RRERERRERERERRRKKEE
42 U1

2: // Title: 둘째 주 복습 프로그램

Se fi

4: // File: Week2

pe 7

6: // Description: 연결 리스트 WR 프로그램

te 7

8: // Classes: PART - part 번호와 S= part

9: //             에 대한 정보 가짐

108 7/

11: // PartNode - PartsList*] 노드

1282 77

13: // PartsList - 각 부분의 연결 리스트에 대한 동작 원리 제공
0448 a

15: // Author: Jesse Liberty (jl)

165 //

17: // Developed: 486/66 32mb RAM MVC 1.5

188 77

19: // Target: Platform independent

205 7/

21: // Rev History: 9/94 - First release (jl)

222 f7

23: // KKK KKK 소소소소수 소소수 소수소소 수소소 소수소 소소소 소소수 소소소 소소소 소소소 소소소 소소조 소소소 조수 조여
24:

25: #include <iostream.h>

26:

27: typedef unsigned long ULONG;

28: typedef unsigned short USHORT;

nN
Se)


===== PAGE 489 =====
제2주 끝내면서 ee 487

30:
S18
32:
$5:
34:
333
56:
37:
38:
59:
40:
41:
425
43:
44:
45:
46:
47:
48:
49:
50:
at!
525
53:
546
D5
56:
571
561
59:
60:
61:
62:
63:
64:
655
66:
67:
68:
69:
708
71s
728
73:
Th:
Tae

// KeeKKKKKKKKKEKKK Part BE xxaxkxkeee

// 주상 베이스 클래스 부분
class Part
4
public: |
Part():itsPartNumber(1) {}
Part(ULONG PartNumber) :itsPartNumber (PartNumber) {}
virtual ~Part(){};
ULONG GetPartNumber() const { return itsPartNumber; }
virtual void Display() const =0; // must be overridden
private:
ULONG itsPartNumber;
3;

// 파생 클래스를 연결할 수 있
// 순수 가상 함수의 구현
void Part::Display() const
{

cout << "\nPart Number: " << itsPartNumber << endl;
}

rir

[[ RRRKEREKEKKKKR Car Part KKKKKEKKKKKKK

class CarPart : public Part
{
public:
CarPart():itsModel Year (94) {}
CarPart(USHORT year, ULONG partNumber) ;
virtual void Display() const
{
Part::Display(); cout << "Model Year: ";
cout << itsModelYear << endl;
}
private:
USHORT itsModelYear;
>

CarPart::CarPart(USHORT year, ULONG partNumber):
itsModelYear (year),
Part (partNumber)

{}

// RRKKKKKKEKKKKKK ATrPlane Part KEKKKKKKKKKEKK



===== PAGE 490 =====
488 ㅇㅇ 제?주

16%
tC:
78:
(9:
80:
81:
82:
83:
84:
85:
86:
87:
88:
89:
90:
912
925
95:
94:
95%
96:
o7:
98:
99:
100:
1011
102:
103:
104:
105:
106:
107:
108:
109:
110:
11
1123
1133
114:
1155
116:
117:
118:
1193
120:
121:

class AirPlanePart : public Part
{
public:
AirPlanePart():itsEngineNumber (1) {};
AirPlanePart(USHORT EngineNumber, ULONG PartNumber) ;
virtual void Display() const
{
Part::Display(); cout << "Engine No.: ";
cout << itsEngineNumber << endl;
}
private:
USHORT itsEngineNumber;
3;

AirPlanePart::AirPlanePart(USHORT EngineNumber, ULONG PartNumber):
itsEngineNumber (EngineNumber),
Part (PartNumber )

G8,

if KKKKKKKKKKKKKEEK Part Node KKKKKKKEKKEEKE
class PartNode
건
public:
PartNode (Part*);
“PartNode ();
void SetNext(PartNode * node) { itsNext = node; }
PartNode * GetNext() const;
Part * GetPart() const;
private:
Part *itsPart;
PartNode * itsNext;
+;

// PartNode 구현

PartNode::PartNode(Part* pPart):
itsPart(pPart),
itsNext (0)

{}

PartNode::~PartNode()
{
delete itsPart;
itsPart = 0;
delete itsNext;


===== PAGE 491 =====
제2주 끝내면서 ee 489

122%
123%
124:
125:
126:
1272
128:
129:
130:
1515
1328
1338
134:
135:
136:
1350:
138:
159%
140:
141:
142:
143:
144:
145:
146:
147,
148:
149:
150:
15.18
152:
1535
154:
155%
156:
157
1588
159:
160:
161%
162:
165:

164

165:
166:
167:

itsNext = 0;
3

// 다음 PartNode%t 없는 경우 널 반환
PartNode * partNode::GetNext() const
{

return itsNext;
Be

Part * PartNode::GetPart() const
{
if (itsPart)
return itsPart;
else
return NULL; //error

// KRKRKREKKEKKEKKKK Part LIST KKKKKKKKKKKKE
class PartsList
{
public:
PartsList();
“PartsList();
// 복사 생성자와 등치 Att 필요함
Part* Find(ULONG & position, ULONG PartNumber) const;
ULONG GetCount() const { return itsCount; }
Part* GetFirst() const;
static PartsList& GetGlobalPartsList()
{
return GlobalPartsList;
B
void Insert(Part *);
void Insert(void (Part::*f)()const) const;
Part* operator[L](ULONG) const;
Private:
PartNode * pHead;
ULONG itsCount;
static PartsList GlobalPartsList;
3;

PartsList PartsList::GlobalPartsList;

// Lists 구현

PartsLists:PartsList@ :
pHead(0),



===== PAGE 492 =====
490 ee 제?주

168:
169:
170:
1715
172:
1768
174
1758
176:
1708
178:
179:
180:
181:
182:
183:
184:
185:
186:
187:
188:
189:
190:
1907
192:
193:
194:
195%
196:
197%
198:
199:
200:
201:
202:
203%
204:
205:
206:
207:
208:
209:
210%
27s
20128
213%

itsCount (0)
{}

PartsList::” PartsList()
{

delete pHead;
+

Part* PartsList::GetFirst() const
{
if (pHead)
return pHead->GetPart();
else
return NULL; // 오류 잡음

Part * PartsList::operatorL](ULONG offSet) const
-
PartNode*x pNode = pHead;

if (!pHead)
return NULL; // 여기서 오류 잡음

if (offSet > itsCount)
return NULL; // error

for (ULONG i=0;i<offSet; i++)
pNode = pNode->GetNext();

return pNode->Getpart();
}

Part* PartsList::Find(ULONG & position, ULONG PartNumber) const
t
PartNode * pNode = 0;
for (pNode = pHead, position = 0;
pNode!=NULL;
pNode = pNode->GetNext(), positiontt)
{
if (pNode->GetPart()->GetPartNumber() == PartNumber)
break;
}
if (pNode == NULL)
return NULL;
else
return pNode->GetPart();


===== PAGE 493 =====
제2주 끝내면서 ee 491

214%
215:

가

216: void PartsList::Iterate(void (Part::*func)() const) const

217:
218:
219:
220:
224%
222:
223;
224:
225%
226:
227:
228:
2295
250:
231%
252:
233:
254:
255%
236:
257:
238:
259:
240:
241:
242:
243:
244:
245%
246:
247:
248:
249:
250:
251:
252%
255%
254:
255%
256:
2575
258:
259:

{

}

if (!pHead)
return;
PartNode* pNode = pHead;
do
(pNode->GetPart()->*func) ();
while (pNode = pNode->GetNext());

void PartsList::Insert(Part* pPart)

{

PartNode * pNode = new PartNode(pPart) ;
PartNode * pCurrent = pHead;
PartNode * pNext = 0;

ULONG New = pPart->GetPartNumber ();
ULONG Next = 0;
itsCountt+;

if (!pHead)

{
pHead = pNode;
return;

}

// 11630보다 작으면
// 이 부분이 색로운 1630로 됨
if (pHead->GetPart()->GetPartNumber() > New)
t
pNode->SetNext (pHead) ;
pHead = pNode;
FETUEN,
}

for (33)
{
// 다음이 없으면 이 새로운 부분을 붙임
if (!pCurrent->GetNext())
t
pCurrent->SetNext (pNode) ;
return;


===== PAGE 494 =====
492 ee 제2주
260:      // 의 APO] 있으면 oll See
261%      // 아닐 경우 다음으로 감
262:      pNext = pCurrent->GetNext();
263:      Next = pNext->GetPart()->GetpartNumber ();
264:      if (Next > New)
2655      {
266:        pCurrent->SetNext (pNode) ;
2612        pNode->Setnext (pNext) ;
268:        return;
269:      a
270%      pCurrent = pNext;
Zrii
Zs +}
205+
274: int main)
Aron <
2(6:   PartsList pl = PartsList::GetGlobalPartsList();
VA A he    Part * pPart = 0;
278:   ULONG PartNumber;
279:   USHORT value;
280:   ULONG choice;
281:
282:   while (1)
283:
284:      cout << "(O)Quit (1)Car (2)Plane: ";
26)"      cin >> choice;
286:
287:     if (!'choice)
288:        break;
289:
290:      cout << "New PartNumber?: ";
291%      cin >> PartNumber;
292:
293:      if (choice == 1)
294:      af
29a:        cout << "Model Year? ";
296:        cin >> value;
297:        pPart = new CarPart(value,PartNumber) ;
298:      가
299:     else
300:     ne
301%        cout << "Engine Number? ";
302:        cin >> value;
3035:        pPart = new AirPlanePart (value,PartNumber) ;
304:     }                                     "

305:


===== PAGE 495 =====
제2주 끝내면서 ee 493

306:      pl.Insert(pPart);

307:   3

308:   void (Part::*pFunc) ()const = Part::Display;
309:   pl.Iterate(pFunc) ;

310: return 0;

311: 3

결과  (O)Quit (1)Car (2)Plane: 1
New PartNumber?: 2837
Model Year? 90
(O)Quit (1)Car (2)Plane: 2
New PartNumber?: 378
Engine Number 4938
(O)Quit (1)Car (2)Plane: 1
New PartNumber?: 4499
Model Year? 94
(O)Quit (1)Car (2)Plane: 1
New PartNumber?: 3000
Model Year? 93
(O)Quit (1)Car (2)Plane: 0

Part Number: 378
Engine No. 4938

Part Number: 2837
Model Year : 90

Part Number: 3000
Model Year: 93

Part Number 4499
Model Year: 94

a  2 주의 복습에서는 Part 객체에 대한 AA 리스트를 구현하여 봅시다. 연결
리스트는 동적인 자료 구조로 마치 배열 같지만 객체가 증가, 감소됨에 따
라 크기가 조정됩니다.
이 연결 리스트는 클래스 Pant] 객체를 가지도록 설계됐는데, 이 Part 각 Part
번호를 가진 임의의 객체에 대한 베이스 클래스로 작용하는 추상 자료형입니다.
에 에서는 Part= CarPart2} AirplanePat=. 다시 분류됩니다.

(ag

클래스 Part 34 - 44H So] 선언되었고 부분 번호와 BA 접근자로 이루어져
있습니다. oop 이 클래스는 각 부분에 대한 다른 중요한 정보를 가지게 할 수도
있습니다. Part 추상 자료형이고 순수 가상 함수 Display(Qol) 의해 나타납니다.


===== PAGE 496 =====
494 ee 제2주

48-51번 줄에서 Display07} 구현이 됩니다. 설계자의 의도는 파생 클래스가 그 자

신의 Display) 메쏘드를 만들도록 하는 것인데 또한 이 메쏘드에도 AA] 될 수

있게 하였습니다.

55 - 67번 줄 및 77 - 89번 줄에서 간단한 파생 클래스 08와 AirPlanePart7}
만들어졌습니다. 각각 AAR Display) 메쏘드를 가지고 있는데 실제 베이스 클래

22] Display) 메쏘드와 연결되어 있습니다.

0004006는 Part 클래스와 PartsList 클래스의 인터페이스로 작동합니다. 부분에 대
한 포인터를 가지며 또한 리스트에서 다음 노드를 가리킴니다. 단 하나의 메쏘드
는 다음 노드를 얻고 설정하며, 그리고 현재 가리키는 Pats 반환하는 것입니다.
이 리스트의 기발한 점은 아마도 nel 이 있을 것인데, 그 선언이 140 - 160번
에 있습니다. 00091491는 리스트의 A 번째 원소(08680)를 가리키고 있고, 다른 메
쏘드들을 리스트를 하나씩 뒤져 접근하기 ~ pHead= 사용합니다. 하나씩 뒤진
다는 것은 말 그대로 하나의 노드를 물어본 뒤 다음 노드를 뒤지는데 끝이
를 가진 노드가 나올 때까지 뒤집니다.

AL 번째와 마지막 번째를 접
근할 수 있는 훌륭한 방식을 ett 혹은 클라이언트가 쉽게 리스트를 뒤질
수 있는 순환 객체를 제공합니다.

PartsList= 그럼에도 불구하고 알파벳 순서로 리스트 된 매우 흥미 있는 메쏘드를
제공합니다. 이것은 매우 좋은 생각이고 함수를 찾기 쉽게 해줍니다.

터00(0는 PartNumber?} ULONGS 취합니다. PartNumberol] 대응하는 부분이 찾아지
면 Parto] 대한 포인터를 반환하고 리스트의 그 부분의 위치에다 01.0840형으로
채움니다. 만일 PartNumber7} 없다면 NULLS 반환하고 위치는 의미가 없어집니
다. 00000000는 리스트의 원소의 개수를 반환합니다. 8009118는 이 숫자를 멤버
변수 19000꼬로 저장하는데 이는 리스트를 하나씩 뒤져 계산할 수도 있습니다.
060969[0는 리스트의 처음 Panto] 대한 포인터를 반환하고 리스트가 비었으면
NULL& 반환합니다.

어

GetGlobalPartsListQ3= 정적 멤버 변수 00000009148의 참조자를  ik
이 이 클래스의 정적 MABAMUC. PartsListS 가진 B       은
GlobalPartsList$ 가지고 있는데 물론 G= PartsListtS 만드는 것은  터  에레 이
러한 개념의 HAS Parte] 생성자를 모든 부분이 0000810009148상에서 만들어지
도록 수정할 것입니다.

= 프로
< 프로


===== PAGE 497 =====
제2주 끝내면서 ee 495

10960는 Partol] 대한 포인터를 가지고 PartNode= 만들어 PartNumber 순으로 리스
트에 추가합니다. 1600는 8#00에 대한 멤버 함수 포인터를 가지는데 매개 변수는
없고 1010형을 반환하며 0009형입니다. 4600는 리스트에 있는 모든 Pant 객체에
대해 멤버 함수를 호출합니다. 예제에서는 21901800에 호출하였는데 이는 가상 함
수이고 따라서 AYA) Part 객체가 호출되는 각 경우에 따라서 적당한 Display()
메쏘드가 호출될 것입니다.

연산자 [ ]는 변위가 주어지면 8ㅁ에 직접 접근할 수 있도
위 검사가 이루어지는데 리스트가 NULLO}AU 변위가 리
요구하면 오류로 NULLS 반환합니다.

실제 프로그램에서는 이 함수에 대한 주석이 클래스 선언에 쓰여 있습니다.

TS 프로그램은 274 - 311에 있습니다. 2009149[ 포인터가 266번 줄에 선언되었고
GlobalPartsList 초기화되었습니다. GlobalPartsList 그 자체는 162번 Zo} 선언되
었습니다. 정적 멤버 변수의 선언이 정의내리지 않는 한 이러한 과정이 필요합니
다. 정의는 클래스의 선언 밖에서 이루어져야 합니다.

282번 줄에서 307번 줄까지 사용자는 자동차 부분 혹은 비행기 부분을 선택하게
됩니다. 선택에 의거하여 올바른 go] 요구되고 필요한 부분이 만들어집니다. 306
번 줄에서 만들어진 부분이 리스트에 삽입됩니다.

PartsList©] Insert() 메쏘드의 구현이 226 - 272번 So] 있습니다. 처음 부분의 번
가 입력되었을 때(2837) 그 ASS 가진 080와 모델 연도 900] 만들어지
LinkedList::Insert() = 전달됩니다.

Ss 합니다. 기본적인 범
조            을

트 크기보다 큰 곳

EL fot

22841 줄에서 새로운 PartNode7} 그 Partol] 만들어지고 변수 New7} 그 부분의 번
호로 초기화됩니다. 234번 줄에서 #009119의 1900때가 증가합니다.

236번 줄의 08680의 NULL@14] 여부가 검사되고 참으로 판결납니다. 여기가 처음
노드이므로 pHead7} 0임은 참입니다. 238번 줄에서 pHead= 새로운 노드를 가리
키도록 설정되고 이 함수가 반환됩니다.

사용자는 두 번째 부분을 입력합니다. 이번에는 비행기 부분의 부분 번호 378과
엔진 번호 4938을 입력합니다. 다시 SH PartsList::Insert()7+} 호출되고 pNode7} 새
로운 노드로 초기화됩니다. 정적 멤버 변수 1900빠는 22 증가하고 pHead7} 검
사됩니다. 08680는 바로 전에 치환되었으므로 Yo] 아니고 검사는 거짓으로 판명
납니다.



===== PAGE 498 =====
496

eo 제2주

244번 줄에서 08600에 의해 부분 번호 28370] 현재 부분의 번호 378과 비교됩니
다. 새로운 값이 전의 28680에 의한 값보다 작으므로 새로운 것이 새로운 헤드의
포인터가 됩니다. 그리고 244번의 검사는 참이 됩니다.

246번 줄에서 새로  로운 노드는 pHeado] 의해 지난 최근에 포인트됐던 노드를 가리
킴니다. 주의할 것은 이것은 새로운 노드가 08600 그 AAS 가리키는 것이 아니
라, pHead7} 가리 키던   노드를 가리키는 것입니다. 247번 줄에서 08600는 새로운

SES 가리키도록 설정됩니다.

순환의 세 번째 부분에서 사용자는 자동차에 대해 4499를 입력하였고 모델 연도

94를 입력하였습니다. 1900따가 하나 증가하고 이번에 입력한 HSE pHead7}
가리키는 번호보다 작지 않습니다. 따라서 251에서 시작하는 for 순환문으로 들어
갑니다.

28680에 의해 포인트되는 값은 378입니다. 두 번째 노드에 의해 가리키는 Re
2837입니다. 현재 값은 4499입니다. 00000 포인터는 286800와 똑같은 LES
리키고 따라서 다음 값이 없는데, 두 번째 노드를 가리키며 따라서 254번 줄의
검사는 실패합니다.

N
=~

pCurent 포인터는 다음 SES 포인트하도록 설정되고 따라서 순환은 반복됩니
다. 이번에는 다음 것이 없으므로 254 = 줄의 검사가 성공하고 따라서 현재의 &
드는 256번 줄의 새로운 노드를 포인트하도록 되고 삽입이 끝납니다.

네 번째로 부분 번호 30000] 입력됩니다. 이는 바로 전 과정과 비슷하게 움직이
는데, 이번에는 현재의 노드가 2837을 포인트하고, 다음 노드가 4499이므로 264번
줄의 Ake 참이 되며 새로운 노드는 자리를 찾아가 들어앉습니다.

마지막 사용자가 OS 입력하고 287번 줄에서 참이 되며 \4160)문을 빠져나갑니
다. 308번 줄에서 멤버 함수 DisplayO7} 멤버 함수 포인터 00000에 치환됩니다.
실제 프로그램에서는 사용자의 선택에 의해 동적으로 치환이 됩니다.

멤버 함수 SOlE|E PartsList::Iterate) 메쏘드로 전달됩니다. 216번 SoA] Iterate()
메쏘드는 리스트가 비어 있지 않다는 사실을 압니다. 그러면 221-223번 줄에서 리
AES) 각각의 Pat7} 멤버 함수 포인터를 사용하여 호출됩니다. 각각의 #ㅁ에 대
한 AAS DisplayO7} 출력에서 보듯이 호출이 됩니다.


===== PAGE 499 =====
> 셋째 주의 학습 목표

CHS 배우기 시작한지 어느새 Sl 주 학습을 끝냈습니다. 지금쯤이면 여러분은 캡술화라든가 Se 다형성 등
의 좀더 고급화된 AA 지향 프로그래밍에 대애 진숙아게 느껴질 것입니다.

마지막 주는 고금 상속에 대애 논의아면서 시작합니다. 16일패에 CASS 스트림에 대애 깊이 HS 것이며 17
일깨는 전저리계의 고급 기능들을 배울 것입니다. 18일꺼 날은 프로그램 언어의 문법에 초점을 맞추기보다는 객
세 지향적인 SAT 설계에 대애 SHOE 새로운 SHO] 될 것입니다. 19일깨는 템플릿을 공부아고, 20일째에
예외 SIS 공부할 것이며, 21M 마지막 날에는 어디서도 다루어지지 않았던 나매지 주제들에 HOH 공부할
이며 나아가 (;++의 도사가 되는 다음 과정에 대애 논의가 있을 예정입니다.



===== PAGE 500 =====


===== PAGE 501 =====
500 ee BF

1 2t(Containment)
지난 예제에서 보았듯이 클래스의 멤버 자료가 다른 클래스의 객체를 포함하는
것이 가능합니다. C+ 프로그래머들은 바깥 클래스가 내부 클래스를 포함하고 있
다고 말합니다. 따라서 Employee 클래스는 문자열 2x|Employee 이름에 사용)와
448(Employee 봉급에 사용) 그리고 기타 SS 포함합니다.
은 불완전하지만 그래도 유용한 String FAAS 설명합니다.
이 예제는 아무런 출력도 내지 않지만 나중의 예제에서 쓰일 것입니다.

[리스트 15.1] 91100 클래스

1: #include <iostream.h>

2: #include <string.h>

3

4   class String

aE

6: public:

7     // constructors

8     String();

9's    String(const char *const);

10:   String(const String &);

Ve   “StringQ;

12;

13%   // overloaded operators

14:   char & operatorLIi(int offset);

138   char operatorLl(int offset) const;
16:   String operator+(const String&);
17:   void operator+=(const String&);

13:   String & operator= (const String &);
19%


===== PAGE 502 =====
제15일 고

fu

상속 기

oir

ee 501

20:
21
22:
255
24:
25:
26%
20:
28:
29:
30:
S18
32:
53.
34:
$5:
56:
St
58%
59:
40:
41:
4e:
43°
44:
ADs
46:
47:
48:
49:
50:
515
528
53%
54:
55
56%
575
38:
59:
60:
61:
62:
63%
64:
65:

// General accessors

int GetLen()const { return itsLen; }

const char * GetString() const { return itsString; }
// static int ConstructorCount;

private:
String (int); //private constructor
char * itsString;
unsigned short itsLen;

>;

// 0빠이트 문자열을 만드는 기본 생성자
String::String()

t

itsString = new char[1];

itsString[0O] = "VO! s

itsLen=0;

// cout << "\tDefault string constructor\n";
Lf ConstructorCount++;

}

// 필효한 만큼의 길이의 새로운 문자열을
// 만드는 클래스 연산자에 의해 사용되는
// 전용 생성자

String::StringCint Len)

t

itsString = new charClen+1];
for (int i =0; i<=len; i++)
itsStringli] = NOUS
itsLen=len;
// cout << "\tString(int) constructor\n";
// ConstructorCount+t;

// 문자 배열을 문자열로 바꿈
String::String(const char * const cString)
£
itsLen = strlen(cString);
itsString = new charLitsLen+1];
for Cint 1 = 0; i<itsLen; i++)
itsStringLlil = cStringLlil;
itsStringLitsLen]="\0';
// cout << "\tString(char*) constructor\n";
ae ConstructorCount++;
}


===== PAGE 503 =====
502 ee 제3주

66:
67:
68:
69:
(02
(15
(2:
(3:
(4s
(ae
76:
UC
(8:
(2
80:
81:
82:
83:
84:
85:
86:
87:
88:
89:
90:
918
92:
95:
94:
955
96:
97:
98:
99%

100:
101:
102:
103:
104:
105:
106:
107:
108:
109:
110:
1115

/
5
{,

38

/
5

}

/
/
5
{

/ 복사 생성자
tring::String (const String & rhs)

itsLen=rhs.GetLen(Q);
itsString = new charLitsLent+1];
for (int i = 0; i<itsLen;it+)
itsStringlil = rhslil;
itsStringLitsLen] = '\0';
// cout << "\tString(String&) constructor\n";
// ConstructorCounttt;

/ 순멸자, 할당된 메모리 반납
타1095 66709 ©

delete [J] itsString;
itsLen = 0;
// cout << "\tString destructor\n";

/ 등지 연산자. 메모리 방줄하고
/ 문자열과 길이를 복사
tring& String: :operator=(const String & rhs)

if (this == &rhs)
return *this;
delete [] itsString;
itsLen=rhs.GetLen();
itsString = new charLitsLent1];
for (int i = 0; i<itsLen;it+)
itsStringLlil = rhslil;
itsStringLitsLen] = '\0';
return *this;
// cout << "\tString operator=\n";
가

Ai 비상수 변위 연산자
// 참조자를 반환
// 나중에 값을 바꿀 수 있게 함
char & String::operatorL](int offset)
£
if (offset > itsLen)
return itsStringLitsLen-11];
else
return itsStringLloffset];


===== PAGE 504 =====
제15일 고급 상속 기능 ee 503

11250

113:

114: // 상수 객체에 사용되는

115: // 상수 변위 연산자

116: char String::operatorL](int offset) const

117: €

118:   if (offset > itsLen)

119%      return itsStringLitsLen-1];
120:   else

121:      return itsStringLoffset];
122: }

123:

124: // 현재의 BASS rhs] 추가하여
125: // 새로운 문자열 만듬
126:,String::operator+(const String& rhs)

pee {
128:   int totalLen = itsLen + rhs.GetLen();

129: = String temp(totalLen+1);
130:   int 1, j;
1315   for Cint i = 0; i<itsLen; i++)

132:      templil = itsStringLil;
133:   for (int j =0; j<rhs.GetLen(); j++, i++)
134:      templil = rhsljJ;

135:   tempCtotalLenJ='\0';

136:   return temp;

137: }

138:

139: // 련재의 문자열 바꿈

140: void String: :operator+=(const String& rhs)

141: 1
142:   unsigned short rhsLen = rhs.GetLen();
143:   unsigned short totalLen = itsLen + rhsLen;

144:   String temp(totalLent1) ;
145:   for Cint i = 0; i<itsLen; i++)

146:      tempCil = itsStringLil;
147:   for (int j = 0; j<rhs.GetLen(); j++, i++)
148:      tempCid = rhslj];

149:   temp[totalLenJ='\0';

150:   *this = temp;

1515 3

152:

1552 // Ant String::ConstructorCount = 0;



===== PAGE 505 =====
504

ee 제3주

ey 번지 학승한 [리스트 11. 121에서 보여준 것과 비슷한 String 클래스를 보여
줍니다. 크게 다른 점은 생성자와 다른 몇몇 함수들이 자신이 사용됨을 나

타내는 출력문을 가진다는 것인데 현재는 주석문으로 막았습니다. 나중의 예제에

서 사용될 것입니다.

23번 줄에서 정적 멤버 변수 ConstructorCount7} 선언되었고 153번 줄에서 초기화

되었습니다. 이 변수는 각각 문자열 생성자에서 증가합니다. 이 부분의 모두가 주

석으로 막았습니다. 나중의 예에서 쓰일 것입니다.

[리스트 152]는 3개의 문자열 객체를 포함하는 Employee FAAS 기술하였습니
다. 여러 개의 문장들이 주석으로 막혔습니다. 나중의 예에서 다시 쓰일 것입니다.

[리스트 15.2] 600!0166 클래스와 구동 프로그램

1   class Employee

2: 4

5

4: public:

De    Employee();

6     Employee(char *, char *, char *, long);
7     “Employee();

8     Employee(const Employee&) ;

9:    Employee & operator= (const Employee &);
40%

173   const String & GetFirstName() const
12:      { return itsFirstName; }

15%   const String & GetLastName() const { return itsLastName; B
14:   const String & GetAddress() const { return itsAddress; }

15   Long GetSalary() const { return itsSalary; +
16:

17、   void SetFirstName(const String & fName)

18:      { itsFirstName = fName; }

19:   void SetLastName(const String & LName)

20:      { itsLastName = LName; +

21:   void SetAddress(const String & address)

225      { itsAddress = address; }

253   void SetSalary(long salary) { itsSalary = salary; }
24: private:

25:   String itsFirstName;

26:   String itsLastName;

art   String itsAddress;

28:   long itsSalary;

29: 33

30:


===== PAGE 506 =====
제15일 고급 상속 기능 ㅇㅇ

에

505

51:
325
55%
34:
35°
36:
Ste
38:
59%
40:
41:
42%
43:
44:
45:
46:
47:
48:
49:
30
D1
226
Dos
54:
Dit
56:
Bi
58:
59:
60:
61:
62:
63:
64:
65:
66:
67:
68:
69:
70:
71s
23
(Se
14:
75"
765

Employee: :Employee():
itsFirstName(""),
itsLastName(""),
itsAddress(""),
itsSalary (0)

{}

Employee::Employee(char * firstName, char * lastName,
char * address, long salary):
itsFirstName(firstName),
itsLastName(lastName),
itsAddress(address),
itsSalary(salary)

CP

Employee: :Employee(const Employee & rhs):
itsFirstName(rhs.GetFirstName()),
itsLastName(rhs.GetLastName()),
itsAddress(rhs.GetAddress()),
itsSalary(rhs.GetSalary())

CP}

Employee::~Employee() {}

Employee & Employee: :operator= (const Employee & rhs)
{
if (this == &rhs)
return *this;

itsFirstName = rhs.GetFirstName() ;
itsLastName = rhs.GetLastName();
itsAddress = rhs.GetAddress();
itsSalary = rhs.GetSalary();

return *this;
}

int main()
{
Employee Edie("Jane","Doe","1461 Shore Parkway", 20000);
Edie.SetSalary (50000) ;
String LastName("Levine");
Edie.SetLastName(LastName) ;
Edie.SetFirstName("Edythe") ;

cout << "Name: ";


===== PAGE 507 =====
506 ee ABs

Ws    cout << Edie.GetFirstName().GetStringQ;

78:    cout <<" "<< EmptoyeeOne.GetLastName().GetStringQ;
798    cout << ".\nAddress: ";  ne.

80:    cout << Edie.GetAddress().GetString(;

81:    cout << ".\nSalary: ";

82:    cout << Edie.GetSalary(;

83: return 0;

84: +}

[리스트 15.1]의 예제 BES STRINGHPPAt 불리는 파일에 저장합시다. 그리고 50109
클래스가 필요로 할 때마다 #000406문을 써서 이를 포함시킬 수 있습니다. 예를 들어,
[리스트 15.2]의 초기 부분에 include String.hppS 주가합니다. 이렇게 하면 려러분의
프로그램에 90100 클래스가 추가될 것입니다.

겔과 Name: Edythe Levine.

Address: 1461 Shore Parkway.
Salary: 50000

분석  [리스트 152] Employee 클래스를 보여주는데 3개의 문자열 개체를 가집
때     니다. 즉, itsFirstName, itsLastName, 15&007695입니다.

70번 줄에서 Employee 객체가 만들어지고 4개의 값들이 Employee 객체를 초기화
하기 위해 전달되었습니다. 71번 줄에서 Employee 접근함수 56698800가 상수값
50000을 가지고 호출되었습니다. 실제 프로그램에서는 이를 동적인 AAAI 입

력하는) 또는 상수로 정할 수 있습니다.

72번 줄에서 문자열이 만들어지고 ++의 문자열 상수로 초기화되었습니다. 이 문
자열 객체는 73번 줄에서 964.050480060의 매개 변수로 사용되었습니다.

74번 줄에서 Employee 함수 SetFirstNameQ°] 다른 상수 문자열을 가지고 호
었습니다. 그러나 여러분이 조금만 주의를 기울인다면 Employees, 인수로
을 취하는 SetFirstNameQ?7H= BS 가지지 않는다는 것을 알 것
SetFirstName)= 상수형 문자열 참조자를 필요로 합니다.

컴파일러는 이를 잘 분석하여 상수형 문자열을 문자열로 만듭니다. [리스트 15.4
의 9번 줄에서 이미 말하였기 때문입니다.

Ad
주 때
ne $e,

ro

로

니


===== PAGE 508 =====
세15일 고급 상속 기능 ee 507

포함된 클래스의 멤버에 접근
Employee 객체는 String) 멤버 변수에 접근하는 특정의 접근자를 가지지 as
다. Employee 객체인 Edie7} 그 자신의 itsFirstName 멘버 변수의 멤버 WS itsLen
에 접근하려면 컴파일러 오류가 발생합니다. 그러나 큰 부담이 되지는 않습니다.
접근자 함수는 90008 클래스에 대해 인터페이스를 제공합니다. Employee 클래스
는 자세한 구현에 대해 걱정할 필요가 없습니다.

포환된 멤버에 대한 접근 걸러내기(6009)
String 클래스는 연산자 +를 제공합니다. Employee 클래스의 설계자는 모든 문
열 접근자(예를 들어 00040040000)가 상수형 참조자를 반환하게 하도록 선언함
으로써 Employee 객체에 대해 호출된 연산자 +o] 대한 접근을 막았습니다. 연
자 +는 상수 함수가 아니고 될 수도 없기 때문에(자기를 부른 객체를 바꿈) 다음
과 같이 쓰면 컴파일러 오류가 발생합니다.

String buffer = Edie.GetFirstName() + Edie.GetLastName() ;
GetFirstName()2- 상수형 문자열을 반환하는데 여러분은 상수형 객체에 대해
자 +를 호출할 수 없습니다. 이를 수정하기 위해 GotkinstName-S 비상수형

‥                                   SS NSA ee a
Saud.

const String & GetFristName() const { return itsFirstName; }

String & GetFirstName() { return itsFirstName; }

ERE 더 이상 상수형이 아니고 멤버 함수 그 자신도 더 이상 상수형이 아님

반
니다. 반환값만 바꾸는 것은 함수명을 중첩하기에는 충분하지 않습니다. 그 함수
의성

포함의 대가
Employee 클래스는 문자열 객체가 만들어질 때마다 혹은 Employee 복사본이 만들
어질 때마다 그만한 대가를 지불해야 한다는 것에 주목해야 합니다.
[리스트 15.1]의 38, 51, 63, 75, 84, 100번 줄의 cout 문장의 주석을 떼어버려 얼마
나 자주 이것이 일어나는지 보기로 합시다. [리스트 15.3]의 구동 프로그램을 다
시 작성하여 어디에서 객체가 만들어지는지 출력해 보기로 합시다.



===== PAGE 509 =====
508 ee ABA

pre 0.  e
이 예제를 험파일하려면
1, [리스트 15.1]의 38, 51, 63, 75, 84, 100의 주석을 Aw Fh.
2. [리스트 15.2]를 편집합니다. 64-84번 SS 없애고 [리스트 15.3]의 예제로 치환합
비마.
3, 앞서 이야ㄱ| 한대로 ttinclude 50^09.100를 주가합니다.

[리스트 15.3] 포함된 클래스 생성자

1    int main®

2   {

3      cout << "Creating Edie...\n";

4:     Employee Edie("Jane","Doe","1461 Shore Parkway", 20000) ;
>t     Edie.SetSalary(20000) ;

6:     cout << "Calling SetFirstName with char sven NN

7      Edie.SetFirstName("Edythe");

8      cout << "Creating temporary string LastName...\n";

9     String LastName("Levine");

10:    Edie.SetLastName (LastName) ;

ies

12%    cout << "Name: ";

15%    cout << Edie.GetFirstName() .GetString(;

14:    cout <<" " << Edie.GetLastName().GetStringQ;
198    cout << ".\nAddress: ";

168    cout << Edie.GetAddress().GetStringQ;

12    cout << ".\nSalary: " ;
18%    cout << Edie.GetSalary();

19    cout << endl;
20:   return 0;
211 +

: Creating Edie...

String(char*) constructor
String(char*) constructor
String(char*) constructor
: Calling SetFirstName with char *...
String(char*) constructor
String destructor

: Creating tempory string LastName...
String(char*) constructor
: Name: Edythe Levine.

FWD =

oD aANaAUY

=<


===== PAGE 510 =====
11: Address: 1461 Shore Parkway.
12: Salary: 20000

13%         String destructor
14:         String destructor
115:         String destructor
16:         String destructor

~

분석 [리스트 15.3]은 [리스트 15.1], [리스트 15.2]와 같은 클래스 선언을 사용ㅎ
였습니다. 단 000문장은 FAS 떼어 버렸습니다. [리스트 15.3]의 출력은
분석을 쉽게 하기 위해 번호를 붙였습니다.
리스트 15.3]의 3번 줄에서 Creating Edie... S 출력시켰고 출력의 1번 So] 나타났
습니다. 4번 줄에서 Employee2] 객체 806가 4개의 매개 변수를 가지고 생성됩니
다. 출력은 90008에 대한 생성자가 기대한대로 3번 호출됨을 보여줍니다.

_

번 줄에 Edie.SetFirstName("Edythe”)7} 3)
출    » TH 문장에 있듯이 문자열 “805706”로부터 임시 문자

이 생기게 합니다. 단 치환이 일어나면 즉시 소멸됩니다.

9번 줄에서 프로그램의 몸체 부분에서 문자열 객체가 만들어집니다. 여기서 프로

그래머는 앞 문장에서 컴파일러가 비명시적으로 행한 일을 명시적으로 해버립니

다. 이번에는 출력 9번 줄에서 생성자가 생기는 것은 보지만 소멸자는 보지 못합

니다. 이 객체는 함수 끝의 영역을 벗어나기 전까지 소멸되지 않습니다.

출력의 13 - 16번 줄에서 Employee 객체가 범위를 벗어나 소멸됨에 따라

Employee 객체의 문자열이 소멸되었습니다. 그리고 9번 줄에서 생성된 LastName

문자열 역시 범위를 벗어나면서 소멸되었습니다.

uy
8 도

값에 의한 복사
[리스트 15.3]에서 하나의 Employee 객체가 만들어질 때 5개의 생성자가 호출되는
aS 보았습니다. [리스트 15.4]는 구동 프로그램(00416 program) 부분을 다시 작성
하였습니다. 이번에는 Seo] 사용되지 않고 정적 멤버 변수 문자열
ConstructorCount7} 사용되었습니다.

[리스트 15.1]은 매번 문자열 생성자가 호출될 때마다 000904000ㅠ0002가 증가하는
것을 보여주었습니다. [리스트 15.4]의 구동 프로그램은 출력문을 호출하고
Employee 객체를 전달하는데 ASW 참조자로, 두 번째는 값으로 전달합니다.
ConstructorCount= Employee7} 매개 변수로 전달될 때마다 얼마나 많은 문자열
객체가 생성되는지 추적합니다.


===== PAGE 511 =====
510 ee 제3주

이 예제를 컴파일하려면
1. 121 예제의 23, 39, 52, 64, 76, 153번 줄의 주석을
2. 15.2의 68-84번 SS 없애고 [리스트 15.4]의

3. 앞서 말했듯이 90109.007를 포함시킴니다.

태제합니다:

[리스트 15.4] 2 전달

1: void PrintFunc(Employee) ;

2: void rPrintFunc(const Employee&) ;

5

4: int main(

br

6:    Employee Edie("Jane","Doe","1461 Shore Parkway", 20000) ;
te    Edie.SetSalary (20000) ;

8:    Edie.SetFirstName("Edythe");

9:    String LastName("Levine");

10:   Edie.SetLastName(LastName) ;

11:

12:    cout << "Constructor count: ";

132   cout << String::ConstructorCount << endl;
14:   rPrintFunc (Edie) ;

135    cout << "Constructor count: ";

16:   cout << String::ConstructorCount << endl;
1/도   PrintFunc (Edie);

18:    cout << "Constructor count: ";

195   cout << String::ConstructorCount << endl;
20:   return 0;

eve 3

22: void PrintFunc (Employee Edie)

238 tt

24:

25%    cout << "Name: ";

26%    cout << Edie.GetFirstName().GetString(;
27:    cout <<" " << Edie.GetLastName().GetString(;
28:    cout << ".\nAddress: ";

29%    cout << Edie.GetAddress().GetString(;
50:    cout << ".\nSalary: " ;

31%    cout << Edie.GetSalary();

32:    cout << endl;

33:

WNW
ue
gt


===== PAGE 512 =====
제15일 고급 상속 기능 eo 9511

36: void rPrintFunc (const Employee& Edie)

37 4
38:    cout << "Name: ";
39%    cout << Edie.GetFirstName().GetString();

40:    cout <<" " << Edie.GetLastName().GetString();
41:    cout << ".\nAddress: ";
42:    cout << Edie.GetAddress().GetString();

43:    cout << ".\nSalary: " ;
44:    cout << Edie.GetSalary();
45:    cout << endl;

46: }

결    Sring(char*) constructor
Sring(char*) constructor
Sring(char*) constructor
Sring(char*) constructor
String destructor
Sring(char*) constructor

Constructor Count: 5
Name: Edythe Levine.
Address: 1461 Shore Parkway.
Salary: 20000
Constructor Count: 5
Sring(String&) constructor
Sring(String&) constructor
Sring(String&) constructor
Name: Edythe Levine.
Address: 1461 Shore Parkway.
Salary: 20000
Sring destructor
Sring destructor
Sring destructor
Constructor Count: 8
Sring destructor
Sring destructor
Sring destructor
Sring destructor

하나의 Employee 객체를 만들에 따라 ae 문자열 객체가 만들어짐을 보
여줍니다. Employee 객체가 PrintFune() 9]  참조자로 전달될 때 추가적인

09009 aie TENA GRY 추가적인 문자열 객체는 앞 만들어집니

hase 모두 참조자로 전달됩니다)

(ald
Jz


===== PAGE 513 =====
512 ee 제3주

14번 줄에서 Employee 객체는 값으로 202004000에 전달되고 EmployeeS| 복사본
이 만들어지고 따라서 3개의 문자열 객체가 만들어집니다.(복사 생성자를 호출하
므로)

상속/포함, 대리(06!69해100) HA 구현

때때로 클래스는 다른 클래스의 속성으로 표현되고자 합니다. 예를 들면 여
이 Parts- Catalog 클래스를 만드는 과제를 받았다고 생각해 봅시다. 요구받
격서에서 PartsCatalogt= 각 0따의 모임체입니다. 각 pate 고유번호를 가지
습니다. PartsCatalog= 중복된 HSS 허용하지 않고 각 pat WSS 통해서
을 원합니다.

째 주 복습에서 여러분은 연결 리스트.00601490를 만들었습니다. 연결 리스트
매우 잘 검사가 되었고, 충분히 이해되었으므로 여러분은 2808080108를 설계
만드는 것이 아니라 이미 완성된 연결 리스트의 기법을 써서 작성하고 싶

At

개 32 ㅋ1 00

ro 00

m 4c fr &
나 내
d

드
*

이런 때 여러분은 yes PartsCatalog 클래스를 만들고 ©] PartsCatalog 클래스에
다 연결 리스트를 포함시킬 수 있습니다. 이때 2009080108는 연결 리스트의 구현
을 (자신의 포함해 버린) 연결 리스트 객체를 사용하여 대리0066886)할 수 있습
니다

이 과제를 해결하는 다른 방법은 20008108를 연결 리스트로부터 파생되게 만들

고 따라서 연결 리스트의 속성은 상속받습니다. 그러나 범용 상속은 “한 종류06
9)”라는 관계를 가져야 하고 이때 여러분은 PartsCatalog7+ 연결 리스트의 “한 종
eee 대한 의문을 제기해야 합니다.
PartsCatalog7} 연결 리스트의 한 종류인지 아닌지에 대한 질문에 답하는 방
LinkedList7} 베이스 클래스이고 PartsCatalog= 파생 클래스임을 가정해 보는 것이
고 이렇게 되면 다음 질문들을 하는 것이 가능합니다.
1. 파생 클래스에 있어서 안되는 것이 베이스 클래스에 있는지 질문합니다. 예를 SH, a
결 리스트 베이스 클래스에 PartsCatalog 클래스가 가져서는 안되는 BTS 가지고 A

지 않습니까? 만일 그러하다면 범용 상속이 불필요하지요.

a 520 |

2. 여러분이 만들려고 하는 클래스가 하나 이상의 베이스를 가지지 않았는지 SES 합니
다. 예를 SH PartsCatalog7} 각각의 객체에서 두 개의 연결 리스트를 필요로 하지

않는지요? 만일 그러하다면 여러분은 거의 확실히 포함을 써야 합니다.



===== PAGE 514 =====
제15일 고급 상속 기능 co 513

러분이 가상 함수 혹은 보호 멤버 접근자의 이점을 가지기 위해 베이스 클래스로부터
       }              일 그러하다면 여러분은 전용 혹은 범용의 상

ce Lo

lta}
Ao
이
요
따
트레
n
po

이 질문의 답변에 기초하여 여러분은 범용 상속(“한 종류” 관계)이나 전용 상속

혹은 포함의 하나를 사용합니다.
새로운 포함됨(000181060) 다른 클래스의 멤버로 선언된 객체

용어. 를 대리(061698407) 특정 기능을 FYE 위해 포함된 클래스의 aye 사용하
는 |

Ke A

@ “201M + (Implemented in terms of)” 하나의 클래스를 다른 클래스의

기능성 위에서 만드는 것 - 단, 범용 상속을 사용 안함

C{z](Delegation)
SH PartsCatalogS 연결 리스트([106601490로부터 파생시키지 않을까요? PartsCatalog
는 연결 리스트가 아닌데 왜냐하면 연결 리스트는 정렬된 모임체이고 각 모임체의
멤버는 반복될 수 있습니다.(집합은 반복이 안됩니다.) PartsCatalogi= 정렬되지 않
은 유일한 항들을 가지고 있습니다. PansCatalog?} 5번 찌 wha part 번호 5가 아

분명히 『009148로부터 범용으로 상속받는 것이 가능하고, 따라서 105600와 변위
연산자([])를 맘에 맞게 재생하는 것이 가능하지만 여기서는 차라리 PartsList 클래
스의 본질을 바꾸었습니다. 대신 여러분은 변위 연산자가 없고, 중복을 허락하지
읍                              + 연산자를 정의하는 ?019080108를 만들

이를 만들기 위한 첫 번째 작업은 '포함'입니다. PartsCatalog= 포함된 LinkedList
의 목록 관리자를 대리할 것입니다. [리스트 15.9]를 살펴봅시다.

[리스트 15.5] 포함된 연결 리스트를 대리함

#include <iostream.h>

typedef unsigned long ULONG;
typedef unsigned short USHORT;

[| RRRRRKKKKERKKKHEK Part KKEKKKEKERK

NOU RW 020 = OC


===== PAGE 515 =====
514 ee 제3주

10:
q15
12:
13:
14:
158
16:
At:
18:
19%
20:
212
22:
25:
24:
25%
26:
er:
28:
29:
50:
313
32:
345
34:
355
36:
Sh
38:
39:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
518
52:
53%
543

// part 대한 추상 베이스 클래스

class Part

{

public:
Part():itsPartNumber(1) {}
Part(ULONG PartNumber):
itsPartNumber (PartNumber) {}
virtual ~Part( {};
ULONG GetPartNumber() const

{ return itsPartNumber; }

he Display() const =0; // must be overridden

private:
ULONG itsPartNumber;

3;

// 순수 가상 함수의 구현
// 파생 클래스를 연결하게 함
void Part::Display( const
{
cout << "\nPart Number: " << itsPartNumber << endl;

}

// KeRKKKKKKKKKKERK Car Part KKKKKKKKEE

class CarPart : public Part
A:
public:
CarPart():itsModelYear (94) {}
CarPart(USHORT year, ULONG partNumber) ;
virtual void Display const
{
Part::DisplayQ;
cout << "Model Year: “;
cout << itsModelYear << endl;
a
private:
USHORT itsModelYear;
3;

CarPart::CarPart(USHORT year, ULONG partNumber):
jtsModelYear (year),
Part (partNumber)

{}

// RRKKKKEKKEREREKKERKR Airplane Part #kKKKKEKKKKER


===== PAGE 516 =====
제15일 고

fu

상

db

Als ee 515

552
56:
af:
58:
D9:
60:
61%
62:
63:
64:
65:
66:
Of:
68:
69:
70%
1:
t2e
38
74:
158
76:
(C3
(8:
(CF
80:
81:
82:
83:
84:
85:
86:
87:
88:
89:
90:
91:
92:
93:
94:
95%
96:
97:
98:
98:
100:
101:

class AirplanePart : public Part
{
public:
AirplanePart():itsEngineNumber (1) {};
AirplanePart
C(USHORT EngineNumber, ULONG PartNumber) ;
virtual void Display() const
nf
Part::Display();
cout << "Engine No.: ";
cout << itsEngineNumber << endl;
+
private:
USHORT itsEngineNumber;
};

AirplanePart::AirplanePart
CUSHORT EngineNumber, ULONG PartNumber):
itsEngineNumber (EngineNumber) ,
Part (PartNumber)

{}

[| RRKKKKKKKKKKKKEKKEKK Part NOdEG KXKKKKKKKKKKKK
class PartNode
{
public:
PartNode (Part*);
“PartNode();
void SetNext(PartNode * node)
{itsNext = node; }
PartNode * GetNext() const;
Part * GetPart() const;
private:
Part *itsPart;
PartNode * itsNext;
Me
// Part Node ~H#

PartNode::PartNode(Part* pPart):
itsPart(pPart),
itsNext (0)

1):

PartNode: :~PartNode()
{
delete itsPart;
itsPart = 0;


===== PAGE 517 =====
516 ㅇㅇ 제주

102:
103;
104:
105:
106:
107:
108:
109:
110:
As
1128:
1132
114:
1158
116:
aires
118:
119:
120:
21:
1229
1233
124:
125:
1206:
1278
128:
129:
130:
1351:
132%
13353
134:
1358
136:
1373
138:
139:
140:
141:
142:
143:
144:
145:
146:
147:
148:

delete itsNext;
itsNext = 0;
Bs

// “tS PartNode"t 없는 경우 널 반환
PartNode * partNode::GetNext() const
{

return itsNext;

Part * PartNode::GetPart() const
{
if (itsPart)
return itsPart;
else
return NULL; //error

// KRRKEKRKKKKEEKRKERERK Part LIST KXKKKKAKKKKEKE
class PartsList
ai
public:
PartsList();
“PartsListQ;
// 복사 생성자와 등치 연산자 필요
void Iterate(void (Part::*f) (const) const;
Part* Find(ULONG & position, ULONG PartNumber)
Part* GetFirst () const;
void Insert(Part *);
Part* operatorL] (ULONG) const;
ULONG GetCount() const { return itsCount; }
static PartsList& GetGlobalPartsList@
£
return GlobalPartsList;
3
private:
PartNode * pHead;
ULONG itsCount;
static PartsList GlobalPartsList;
3;

PartsList PartsList::GlobalPartsList;

PartsList::PartsList(:

const;


===== PAGE 518 =====
제15일 고급 상속 기능 ee 517

149:
150:
151
152:
155:
154:
1555
156:
157%
158:
1598
160:
161:
162:
163:
164:
165:
166:
167:
168:
169:
170:
1718
172:
173s
1745
17593
176:
1:
178:
179:
180:
181%
182:
183:
184:
185:
186:
187:
188:
189:
190:
191s
192°
193%
194:
195:

pHead(0),
itsCount (0)
{}

PartsList::~PartsList()
af

delete pHead;
}

Part* PartsList::GetFirst() const
£
if (pHead)
return pHead->GetPart();
else
return NULL; // 오류 잡음

Part * PartsList::operatorL[](ULONG offSet) const
£

PartNode* pNode = pHead;

if (!pHead)
return NULL; // 여기서 오류 잡음

if (offSet > itsCount)
return NULL; // error

for (ULONG i=O;i<offSet; i++)
pNode = pNode->GetNext();

return pNode->Getpart();
}

Part* PartsList::Find(
ULONG & position,
ULONG PartNumber) const

{
PartNode * pNode = 0;
for (pNode = pHead, position = 0;
pNode!=NULL;
pNode = pNode->GetNext(), positiont+)
{
if (pNode->GetPart()->GetPartNumber() == PartNumber)
break;
}

if (pNode == NULL)
return NULL;


===== PAGE 519 =====
518 ee 제3주

196:   else

197:      return pNode->GetPart();

198: }

1995

200: void PartsList::Iterate(void (Part::*func) ()const) const
201: ¢

202:   if (!pHead)

205:     return;

204:   PartNode* pNode = pHead;

205:   do

206:     (pNode->GetPart()->*func) O;
207:   while (pNode = pNode->GetNext());
208: }

209:

210: void PartsList::Insert(Part* pPart)
2113 ¢

212:   PartNode * pNode = new PartNode(pPart) ;
2132   PartNode * pCurrent = pHead;

214:   PartNode * pNext = 0;

215:

216:   ULONG New = pPart->GetPartNumber ();
210:    ULONG Next = 0;

218:   itsCountt+;

219:

220:   if (!pHead)

2211   1

222:      pHead = pNode;
225:     return;

224:   }

225%

2265   // head} 작으면
227:  // 이 부분이 새로운 1620로 됨
ees:   if (pHead->GetPart()->GetPartNumber() > New)

229:   £

230:     pNode->SetNext (pHead) ;

2318      pHead = pNode;

25e:     return;

233:   }

234:

255:   for Cee)

236:   {

237:      // 다음이 없으면 이 새로운 부분을 붙임
2588     if ('pCurrent->GetNext())
239:     {

240:        pCurrent->SetNext (pNode) ;
241:          return;

242:     +


===== PAGE 520 =====
제15일 고급 상속 기능 ee 519

243%
244:
245:
246:
247:
248:
249:
2508
Zoe
252%
255%
254:
2558
256:
200
258:
259:
260:
261:
262:
263:
264:
265:
266:
267:
268:
269:
270:
erie
eer
2051
274:
275:
276:
217%
278:
2901
280:
281:
282:
263:
284:
285%
286:
287:
288:
289:

// 의 식이에 있으면 역기에 살입학고
// Ve) 경우 다음으로 감
pNext = pCurrent->GetNext();
Next = pNext->GetPart()->GetpartNumber () ;
if (Next > New)
{
pCurrent->SetNext (pNode) ;
pNode->Setnext (pNext) ;
return;
}
pCurrent = pNext;

class PartsCatalog

ti

public:

void Insert(Part *);

ULONG Exists(ULONG PartNumber) ;

Part * Get(int PartNumber) ;

operator+(const PartsCatalog &);

void ShowALl() { thePartsList.Iterate(Part::Display); }

private:

a

PartsList thePartsList;

void PartsCaltalog::Insert(Part * newPart)

{

ULONG partNumber = newPart->GetpartNumber ();
ULONG offset;

if (!thePartsList.Find(offset, partNumber) )

thePartsList.Insert(newPart);
else
a
cout << partNumber << " was the ";
switch (offset)
{
case 0: cout << "first "; break;
case 1: cout << "second "; break;
case 2: cout << "third "; break;
default: cout << offsett1 << "th";


===== PAGE 521 =====
520 66 제주

290:      cout << "entry.Rejected!\n";

291:   3

2925 2

293:

294: ULONG PartsCatalog::Exists(ULONG PartNumber)
295° £

296:   ULONG offset;

298   thePartsList.Find(offset,PartNumber) ;
298:   return offset;

299: }

300:

301: Part * PartsCatalog::Get(int PartNumber)
302: £

303:   ULONG offset;

304:   Part * thePart = thePartsList.Find(offset, PartNumber) ;
305:   return thePart;

306: }

307:

308:

309: int main()

5105 <

31181   PartsCatalog pc;

Size    Part * pPart = 0;

313:   ULONG PartNumber;

314:   USHORT value;

515%   ULONG choice;

3516:

S172   while (1)

318:   {

5198      cout << "(O)Quit (1)Car (2)Plane: ";
320:      cin >> choice;

9212

$228      if ('choice)

3235:        break;

324:

$25:      cout << "New PartNumber?: ";

526%      cin >> PartNumber;

Sere

328:      if (choice == 1)

529:     {

550%         cout << "Model Year?: ";

551:        cin >> value;

332%        pPart = new CarPart(value,PartNumber) ;
3553:     }

334:     else

350!     {

336:         cout << "Engine Number?: ";


===== PAGE 522 =====
제15일 고급 상속 기능

ee 521

S57:
338:
339:
341:
5415
542:
343:
344:

cin >> value;
pPart = new AirPlanePart(value,PartNumber) ;
B
pc.Insert(pPart);
B
pc.ShowALl();
return 0;
}

결과

a

PartsCataloge}i= 새로운 클래스가 260 - 2708) 줄에 모

Lu

< PartsListS

(O)Quit (1)Car (2)Plane:
New Part Number?: 1234
Model Year?: 94

(O)Quit (1)Car (2)Plane: 1
New Part Number?: 4434
Model Year?: 93

(O)Quit (1)Car (2)Plane: 1
New Part Number?: 1234
Model Year?: 94

1234 was the first entry. Rejected!
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 2345
Model Year?: 93

(O)Quit (1)Car (2)Plane: 0

Part number: 1234
Model Year: 94

Part number: 2345
Model Year: 93

Part number: 4434
Model Year: 93

[리스트 15.5]는 2째 주 복습의 Part, PartNode, PartsList 클래스에 대한 인터

수기 자시

PartsList 관점에서 구현되었습니다.

PartsCatalog®] 클라이언트는 『009119에 직접 접근하지 않습니다. 인터페이스

PartsCatalogS 통해서이고 그에 따라 『7009149는 동적으로 변합니다. 예를 들면

만들어졌습니다. PartsCatalog
자료 멤버로 가지는데 목록 관리를 대리합니다. PartsCataloge

and
uU

PartsCatalog::Insert() 메쏘드는 7809149(에서의 중복된 엔트리를 허용 ve 습니다.


===== PAGE 523 =====
522

eo 제3주

PartsCatalog::Insert()°] 구현은 272번 줄에서 시작합니다. 매개 변수로 전달된 Part
& jtsPartNumber 멤버 변수의 값을 요구받습니다. 이 값은 8809119의 8000 메쏘
Eo] 주어지고, 일치하는 값이 없으면 그 번호가 입력됩니다. 같은 go] 있으면
오류 문장이 출력됩니다.

PartsCatalog*= 『009149[인 멤버 변수에 InsetS 직접 호출함으로써 실질적인 입력
을 합니다. 이러한 실질적인 입력 구조, 연결 리스트의 유지, 연결 리스트의 탐색
및 검색 등이 PartsCatalog®}] 멤버인 포함된 PartsListoll 의해 유지됩니다.
PartsCatalog7} 이러한 부분의 코드를 만들 필요는 없습니다. 단지 잘 정의된 인터
페이스의 이점을 활용하면 됩니다.

이 부분이 바로 +에서의 재사용06058)의 핵심이 됩니다. 『200908101108는 PartsList
의 코드를 재사용할 수 있습니다. PartsCatalogs] 설계자는 000906(의 자세한 부분
의 PAS 몰라도 됩니다. 0009149((클래스의 선언)와의 인터페이스는 PartsCatalog

클래스의 설계자에 의해 필요로 하는 모든 정보를 제공합니다.

전응 상속(61026 Inheritance)

PartsCatalog7} 만일 140660149의(물론 여기에서는 없었습니다.) 보호 멤버를 접근
할 Bork 있었다면, 혹은 Linkedlisto] 메쏘드를 중복할 필요가 있었다면
PartsCatalog= 『009178[로부터 상속받아야 합니다.

PartsCatalog*= 『80091719[의 객체가 아니므로 또 여러분은 ?009149의 함수 기능들
PartsCatalog®] 클라이언트들에게 노출시키고 싶지 않으므로 여러분은 전용 상속
쓸 필요가 있습니다.

전용 상속에서 먼저 알아야 할 것은 모든 베이스 멤버 변수와 함수들은 실제 베
이스에서의 접근 수준에 관계없이 전용으로 선언된 것처럼 취급된다는 것입니다.
따라서 PartsCatalog®] 멤버 함수가 아닌 모든 함수에 있어서 200918로부터 상속
된 모든 함수는 접근 불가능합니다. 이는 심각한 문제입니다. 전용 상속은 상속을
위한 인터페이스를 가지지 않습니다.

PartsCatalog 클래스의 사용자들에게 PartsListt= 보이지 않습니다. 그 인터페이스 어
느 것도 유효하지 않습니다. 어떠한 메쏘드도 호출할 수 없습니다. 하지만
PartsCatalog 메쏘드는 호출할 수 있습니다. 그리고 그 메쏘드는 모든 1400601256는
접근할 수 있는데, 왜냐하면 그들은 모두 140660178로부터 파생되었기 때문입니다.


===== PAGE 524 =====
제15일 고급 상속 기능 ce 523

여기서 중요한 것은 0008080108는 PartsList7} 아니라는 것인데 범용 상속에 포함
되어 있습니다. 이는 PartsListeH= 관점에서 구현되었는데 포함의 경우와 마찬가
지입니다. 전용 상속이 편합니다.

[리스트 15.6]은 PartsCatalog= PartsList2 PE] 전용으로 파생된 클래스로 다시 작
성하여 만든 예제입니다.

에 북사래야 합- 다.

[리스트 15.6] HS 상속

1: // CRIAE 15.6] 전용 상속

2: // PartsCatalog 다시 작성

38 //

4:

a

6:

7: class PartsCatalog : private PartsList
8: {

9: public:

10:   void Insert(Part *);

113   ULONG Exists(ULONG PartNumber) ;

12:   Part * Get(int PartNumber);

137   operator+(const PartsCatalog &);

14:   void ShowALL() { Iterate(Part::Display); }
15: private:

16: 35

18: void PartsCatalog::Insert(Part * newPart)

193 £

208   ULONG partNumber = newPart->GetPartNumber() ;
21s   ULONG offset;

22%

25:   if (!Find(offset, partNumber))

24:     PartsList::Insert(newPart) ;

258   else

26:   £

208      cout << partNumber << " was the ";
28:      switch (offset)

29:      {

50:        case Q: cout << "first "; break;


===== PAGE 525 =====
524 ee 제3주

idle
$2:
55:
34:
35:
36:
Sts
38:
59:
40:
4&1:
42:
43:
44:
45:
46:
47:
48:
49:
50:
515
525
535°
54:
Doe
56:
Dts
58:
Dg:
60:
61:
62:
63:
64:
65?
66:
67:
68:
69:
10%
718
tes
(3:
(4%
153
(6:
C3

case 1: cout << "second "; break;

case 2: cout << "third "; break;

default: cout << offsett1 << "th ";
해

cout << "entry. Rejected!\n";
가

ULONG PartsCatalog::Exists(ULONG PartNumber)
t

ULONG offset;

Find(offset,PartNumber) ;

return offset;
3

Part * PartsCatalog::Get(int PartNumber)
{

ULONG offset;

return (Find(offset, PartNumber));

int main(Q)

a
PartsCatalog pc;
Part * pPart = 0;
ULONG PartNumber;
USHORT value;
ULONG choice;

while (1)

38
cout << "(O0)Quit (1)Car (2)Plane: ";
cin >> choice;

if (!choice)
break;

cout << "New PartNumber?: ";
cin >> PartNumber;

if (choice == 1)
{

cout << "Model Year?: ";

cin >> value;

pPart = new CarPart(value,PartNumber) ;
가


===== PAGE 526 =====
제15일 고급 상속 기능 ee 525

78:     else

198      {

80:         cout << "Engine Number?: ";

81:        cin >> value;

82:        pPart = new AirPlanePart(value,PartNumber) ;
83:      Bs

84:     pc.Insert(pPart);

85°   }

86:   pc.ShowALl();
87: return 0;
88: }

겔과 (O)Quit (1)Car (2)Plane: 1
New Part Number?: 1234

Model Year?: 94
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 4434
Model Year?: 93
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 1234
Model Year?: 94
1234 was the first entry. Rejected!
|                      (O)Quit (1)Car (2)Plane: 1
|                     New Part Number?: 2345
|                     Model Year?: 93
(O)Quit (1)Car (2)Plane: 0

Part number: 1234
Model Year: 94

Part number: 2345
Model Year: 93

Part number: 4434
Model Year: 93

분석  [리스트 15.6|은 28008080108로의 변화된 인터페이스 부분만을 보여주고 구동 프로
7 그람을 다시 작성하였습니다. 다른 클래스와의 인터페이스는 [리스트 155|와 다른
부분이 없습니다.
[리스트 15.6] TH 줄에서 PartsCatalog= PartList22E} 전    전용으로 파생되었음을 선

언합니다. PartsCatalog2}2] 인터페ㅇ ]스부는 [리스트 15.5]와 바뀌지 않았습니다. 물
= HS Partlist 객체를 멘버 자료로 필요로 하지 않습니다.


===== PAGE 527 =====
526 ㅇㅇ 제주

PartsCatalog2] 9500\4110함수는 『009119의 IterateQS 호출하는데, 4000060의 범용
인터페이스 역할을 하는 PartShowAllQ 클래스의 멤버 함수를 가리킴니다.

ShowAll0&- 16000의 범용 인터페이스로 동작하는데 올바른 정보를 제공

하고 한

편 클라이언트 클래스로부터 100060를 직접 호출하지 못하게 합니다. 비록
PartsList= 다른 함수들은 100660로 전달될 수 있게 하지만 280050800108만은 안되

게 합니다.

Insert() 함수도 역시 upYrch, 23번 SS 봅시다. 8000가 직접 호출되는데

베이스 클래스로부터 상속받았기 때문입니다. 24번 줄의 Inset) 호출은
되어야 하는데 그렇지 않으면 무한 반복합니다.

간단히 말해 PartsCatalog w= 7} PartsList 메쏘드를 호출하기

2

oN elt

i

a A

원할 때 직접

행해야 합니다. 단 하나의 예외 AS} PartsCatalog7} 메쏘드를 중복하고 PartsList
버전이 필요할 때인데 이때에는 함수명이 충분히 써져야 합니다.

하지만,
직접 접

DO     파생된 객체가 베이스 클래스의 “st 종류"일 때 전용 상속을 사용하시오.

Do    다른 클래스의 함수 기능을 대리하고 싶을 때 포함을 사용하시오. 단 그의
보호 멤버를 접근할 필요는 없습니다

DO     다른 클래스의 용어로 구현할 필요가 있을 때 그리고 베이스 클래스의 보호
멤버를 접근할 필요가 있을 때 전용 상속을 사용하시오

DON'T 하나 이상의 베이스 클래스를 사용할 필요가 있을 때 전용 GSS 사용하지
Bcf 포함을 사용해야 합니다. WB 들면, PartsCatalog tt 두 개의
『31+5Ｌ:하를 BRE 한다면 전용 TSE 쓰면 안됩니다

DON'T 베이스 클래스의 멤버가 파생 클래스의 클라이언트에게 유료해서는 안되며
전용 상속을. 쓰지 SMF

프랜드 클래스(『「!1600 Class)

종종 여러분은 클래스들을 같이, 하나의 집합으로 만들 때도 있습니다. as 들
©}, PartNode3} PartsList7} 긴밀하게 상호 연관되어 있다면, 8809148&[가 PartNode 2]


===== PAGE 528 =====
제15일 고급 상속 기능 ee 527

Part 포인터인 itsPanS 직접 읽을 수 있다면 매우 편리할 것입니다.

접
여러분은 16000를 범용이나 보호형으로 만들기를 원하지 않는데, 왜냐하면 168
는 PartNodeS] 상세한 구호     으로 하고 싶기 때문입니다. 그러나 이를
PartsListo]] 노출시키고 싶습니다.

ret
i
은비 a
op |o

여러분이 전용 멤버 자료나 함수를 다른 클래스에 노출시키고 싶으면 여러분은
그 클래스를 0000로 선언하면 됩니다. 이렇게 하면 여러분의 클래스의 인터페이

됩   ;
Nese Ss 쁘
를 프랜드 클래스를 포함하도록 합니다.

|»

일단 PartNode7} PartsLitS 프랜드 클래스로 Ass ParsListo] 관련된 모든
28009006의 멤버 자료나 함수는 모두 범용이 됩니다.

이 프랜드라는 관계는 전달되지 않습니다. 마치 당신이 나의 친구이고 홍길동이
당신의 ATA 때 내가 반드시 홍길동의 친구는 아닌 것처럼 말입니다. 프랜드의
관계는 상속되지 않습니다. 다시 한 번 예를 들면 당신이 나의 친구라 나의 비밀
을 모두 말한다고 당신의 아이들과 나의  비밀을 공유하지 않는 것과 같습니다.

마지막으로 프랜드라는 관계는 교환되지 않습니다. 클래스 vps 클래스 yp]
프랜드가 되게 한다고 하여 클래스 '나`가 클래스 po] 프랜드로 되는 것은 아
Bud. 당신이 나에게 모든 비밀을 말한다고 하여 내가 나의 모든 비밀을 당신
에게 말할 Bee 없습니다.

[리스트 15.71은 [리스트 15.6|으로부터의 예제를 프랜드 관계를 적용하여 다시 작
성하였습니다. 여기서 2009119[를 280040086의 프랜드로 하였습니다. 그렇다고 하여
PartNode7} 『?8009149(의 프랜드로 되는 것은 아닙니다.

[리스트 15.7] 프랜드 클래스의 예제

O: #include <iostream.h>

1:

2: typedef unsigned long ULONG;
3: typedef unsigned short USHORT;
4:

53

6:   [| RRKKKKKKKKEKKKEKKK Part KKKKKKKKKKK
(3

8: // part] 대한 추상 베이스 클래스
9: class Part

10: <

112 public:

12:    Part():itsPartNumber(1) {}

135    Part(ULONG PartNumber):


===== PAGE 529 =====
528 ee AB

14:
132
16:
10
18:
19:
20:
212
222
23:
24:
25:
26:
ar:
28:
295
30:
31,
32:
33:
34:
553
505
Sis
$8:
39:
40:
41:
42:
43:
44:
45:
46:
4(3
48:
49:
50,
51:
52:
535
54:
55
56:
EAH
58!
59:

itsPartNumber (Par tNumber) {}

virtual ~Part(){};

ULONG GetPartNumber() const

{ return itsPartNumber; }

virtual void Display() const =0; // must be overridden
private:

ULONG itsPartNumber;
>

// 순수 가상 함수의 구련
// 파생 클래스를 연결
void Part::Displ
“e

cout << "\nPart Number: " << itsPartNumber << endl;

// KRRRKKREKKEKKEEK Car Part KxRKKKKKKK

class CarPart : public Part

{
public:
CarPart():itsModelYear (94) {}
CarPart(USHORT year, ULONG partNumber) ;
virtual void Display const
{
Part::DisplayQ;
cout << "Model Year: “;
cout << itsModelYear << endl;
}
private:
USHORT itsModelYear;
Ly

CarPart::CarPart(USHORT year, ULONG partNumber):
itsModelYear(year),
Part (partNumber )

[에

// KRREKKKERKKEKKKKKKER Airplane Part *xKKKKKKKKAKK

class AirplanePart : public Part

6:

public:
AirplanePart():itsEngineNumber (1) {};
AirplanePart


===== PAGE 530 =====
세15일 고급 상속 7

ee 529

60:
61:
62:
65%
64:
65%
66:
6f:
68:
69:
70:
Tl:
es
(3:
(4:
(58
76:
0:
78:
09:
80:
812
82:
83:
84:
85:
86:
87%
88:
89:
90:
91:
92:
93:
94:
95:
96:
97%
98:
98:

100:
101:
102:
103:
104:
105:

CUSHORT EngineNumber, ULONG PartNumber) ;
virtual void Display() const
{
Part::Display();
cout << "Engine No.: ";
cout << itsEngineNumber << endl;
}          :
private:
USHORT itsEngineNumber;
3;

AirplanePart::AirplanePart
CUSHORT EngineNumber, ULONG PartNumber):
i tsEngineNumber (EngineNumber) ,
Part (PartNumber)
4}
[| KRKKKKKRRKEKKKKKRKKKK Part Node xkkKKKKKKKKKEK
class PartNode
af
public:
friend class PartsList;
PartNode (Partx) ;
“PartNode();
void SetNext(PartNode * node)
C{itsNext = node; }
PartNode * GetNext() const;
part * GetPart() const;
private:
Part *itsPart;
PartNode * itsNext;
3;
// Part Node ~H#

PartNode::PartNode(Part* pPart):
itsPart(pPart),
itsNext (0)

(3

PartNode::~PartNode()
aE
delete itsPart;
itsPart = 0;
delete itsNext;
itsNext = 0;


===== PAGE 531 =====
530 ee 제3주

106:
107:
108:
109:
110:
1118
1125
1192
1145
1155
1408
1172
118:
AS:
120:
Aas
A228
123%
124:
125%
126:
Ter:
128:
129
1308
1318
132:
1338
134:
(35:
136:
1378
138:
159%
140:
141%
142:
143:
144:
145:
146:
147:
148:
149:
150:
1515

// 다음 PartNode"t 없는 경우 널 반환
PartNode * partNode::GetNext() const
{

return itsNext;

Part * PartNode::GetPart() const
t
if (itsPart)
return itsPart;
else
return NULL; //error

Ji KKKKKKKEKKEKKEKEREEER Part LIST KEKKKKKKKKKKKE
class PartsList
{
public:
PartsList();
“PartsListQ);
// 복사 생성자와 SF] 연산자 필요
void Iterate(void (Part::*f) (const) const;
Part* Find(ULONG & position, ULONG PartNumber) const;
Part* GetFirst () const;
void Insert(Part *);
Part* operatorL[] (ULONG) const;
ULONG GetCount() const { return itsCount; }
static PartsList& GetGlobalPartsList()
{
return GlobalPartsList;
}
private:
PartNode * pHead;
ULONG itsCount;
static PartsList GlobalPartsList;
3;

PartsList PartsList::GlobalPartsList;

PartsList::PartsList():
pHead(0),
itsCount (0)

i}


===== PAGE 532 =====
세15일 고

qu
oz
db
=
olr

15208
1538
154:
155¢
156:
1572
158:
159:
160:
161:
162:
165:
164:
165:
166:
167:
168:
169:
170:
171s
1728
1066
174:
1733
1768
Wit:
1078:
179:
180:
181:
182:
183:
184:
185:
186:
1878
188:
189:
190:
191:
192:
193%
194:
195%
196:
197:

PartsList::~PartsList()
{

delete pHead;
}

Part* PartsList::GetFirst() const
{
if (pHead)
return pHead->itsPart;
else
return NULL; // 오류 잡음

Part * PartsList::operatorLJ(ULONG offSet) const
{
PartNode* pNode = pHead;

if ('!pHead)
return NULL; // 여기서 오류 잡음

if (offSet > itsCount)
return NULL; // error

for (ULONG i=0;i<offSet; i++)
pNode = pNode->GetNext();

return pNode->Getpart();
+

Part* PartsList::Find(
ULONG & position,
ULONG PartNumber) const

PartNode * pNode = 0;
for (pNode = pHead, position = 0;
pNode!=NULL;
pNode = pNode->GetNext(), positiont+)
a

if (pNode->GetPart()->GetPartNumber() == PartNumber)

break;
0,
if (pNode == NULL)
return NULL;
else
return pNode->GetPart();


===== PAGE 533 =====
532 ee 제3주

198: }

199:

200: void PartsList::Iterate(void (Part::*func) ()const) const
2012 <

202:   if (!pHead)

203:     return;

204:   PartNode* pNode = pHead;

205:   do

206:      (pNode->GetPart ()->*func) ();
2075   while (pNode = pNode->GetNext());
208: }

209:

210: void PartsList::Insert(Part* pPart)
116 «

ele:   PartNode * pNode = new PartNode(pPart) ;
2156   PartNode * pCurrent = pHead;

214s   PartNode * pNext = 0;

215%

216%   ULONG New = pPart->GetPartNumber ();
2173    ULONG Next = 0;

218:   itsCounttt;

219:

220:   if (!pHead)

224   {

222:      pHead = pNode;

225:     return;

224:   }

225

226:   // headS*} 작으면

227:  // 이 부분이 새로운 1680로 됨

220   if (pHead->itsPart->GetPartNumber() > New)
229:   {

230:      pNode->itsNext = pHead;

251%      pHead = pNode;

252:     return;

253:   By

234:

255%   for 072

236:   £

237:      // 다음이 없으면 이 새로운 부분을 붙임
2583     if (!pCurrent->itsNext)

239:     {

240:        pCurrent->itsNext = pNode;
241:          return;

242:      }

243:


===== PAGE 534 =====
제15일 고급 상속 기능 ee 533

244:
245:
246:
247:
248:
249:
250:
251%
252°
253:
254:
255%
256:
257%
258:
209%
260:
261:
262:
263:
264:
26a.
266:
267:
268:
269:
2708
erie
272:
273:
274:
2755
2766
207:
278:
279:
280:
281:
282:
285:
284:
2851
286:
28:
288:
289:

// 이 사이에 있으면 여기에 삽일하고

// 아닐 경우 다음으로 감

pNext = pCurrent->itsNext;

Next = pNext->itsPart()->GetpartNumber ();

if (Next > New)

t
pCurrent->itsNext = pNode;
pNode->itsNext = pNext;
return;

a}

pCurrent = pNext;

class PartsCatalog : private PartsList
{
public:
void Insert(Part *);
ULONG Exists(ULONG PartNumber) ;
Part * Get(int PartNumber) ;
operator+(const PartsCatalog &);
void ShowALL() ¢ thePartsList.Iterate(Part::Display); }
private:
3;

void PartsCaltalog::Insert(Part * newPart)

{
ULONG partNumber = newPart->GetpartNumber () ;
ULONG offset;

if (!Find(offset, partNumber) )

PartsList::Insert(newPart) ;
else
5
cout << partNumber << " was the ";
switch (offset)
af
case 0: cout << "first "; break;
case 1: cout << "second "; break;
case 2: cout << "third "; break;
default: cout << offset+1 << "th";


===== PAGE 535 =====
5034 ee ABs

290:
294:
292:
293:
294:
295:
296:
29s
298:
299:
300:
$01:
302:
303:
304:
505%
306:
S073
308:
309:
310:
311":
37128
513%
S145
S15
316:
Sif:
318:
319%
320:
3212
322:
325:
324:
525:
326:
$275
328:
529:
550:
S51:
3352:
333:
3345
335:

가

cout << "entry.Rejected!\n";

ULONG PartsCatalog::Exists(ULONG PartNumber)

{

+

ULONG offset;
thePartsList.Find(offset,PartNumber) ;
return offset;

Part * PartsCatalog::Get(int PartNumber)

{

ULONG offset;

return (Find(offset, PartNumber));

int main()

{

PartsCatalog pc;
Part * pPart = 0;
ULONG PartNumber;
USHORT value;
ULONG choice;

while (1)

xf

cout << "(O)Quit (1)Car (2)Plane: ";
cin >> choice;

if (!choice)
break;

cout << "New PartNumber?: ";
cin >> PartNumber;

if (choice == 1)
본
cout << "Model Year?: ";
cin >> value;
pPart = new CarPart(value,PartNumber) ;
3
else
{


===== PAGE 536 =====
제15일 고급 상속 기능 ee 535

336:         cout << "Engine Number?: ";

557:        cin >> value;

338:        pPart = new AirPlanePart(value,PartNumber) ;
559%      }

541:   pc.Insert(pPart);

341:   }

342:   pc.ShowALl();
343: return 0;
344: }

결과 (O)Quit (1)Car (2)Plane: 1
New Part Number?: 1234
Model Year?: 94
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 4434
Model Year?: 93
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 1234
Model Year?: 94
1234 was the first entry. Rejected!
(O)Quit (1)Car (2)Plane: 1
New Part Number?: 2345
Model Year?: 93
(O)Quit (1)Car (2)Plane: 0

Part number: 1234
Model Year: 94

Part number: 2345
Model Year: 93

Part number: 4434
Model Year: 93

80번 줄에서 PartsListt= PartNode 클래스의 프랜드로 선언되었습니다.
= AM] 범용 부분에서 선언되었는데 문장의 의미를 바꾸지 않는다
래스 선언부의 아무 곳에나 선언될 수 있습니다. 이 문장으로 인해 모든 전
버 ASS 함수들이 0809148[ 클래스의 모든 멤버 함수에게 유효합니다.
SS SS ae ee
158번 줄에서 멤버 함수 0604000의 구현이 이 변화를 반영하였습니다
pHead->GetPartS 반환하는 대신 이 함수는 08680->1680@라고 써서 전용 wy} 자
를 반환할 수 있습니다. 비슷하게 18000 함수는 pNode->SetNext(pHead)2}31 2%
는 대신에 pNode->itsNext = pHeadz} 썼습니다.

(rad

a
&

ne 때 me


===== PAGE 537 =====
ee 제3주

사실 이는 사소한 변화이고 『009119[를 『20084006의 프랜드로 선언하는 충분한 이
유는 없지만 a] oko} friends] 예를 보여주는 의미는 있습니다.
리아 아이바 a OD

랜드 클래스의 선언은 매우 주의하여 사용해야 합니다. 만일 두 개의 클래스가

복잡하게 Aa) 있고, 하나의 클래스가 다른 클래스를 아주 자주 접근한다면 이러
한 선언을 할 충분한 이유가 있습니다. 하지만 아껴서 사용합시다. 전용 접근 메
쏘드를 쓰는 것이 쉬울 경우가 많습니다. 그리고 그렇게 하는 것이 다시 컴파일

를 RE          경
=   ㄴ          ㅇ
하지 않고 클래스를 쓸 수 있게 합니다.

++의 전문가들은 =

랜드 선언이 때때로 객체 지향 프로그래밍에 있어서 중요한 요소
인 Waste 저래한다고 합니ㄷ
A

|다. 사실대로 말하면, 말도 안되는 소리입니다. 프랜드 선
프랜드 부분을 선언합니다. 그리고 전용 파생과 마찬가지로
다.

언은 클래스 인터페이

gt
의
Wests 저해하지 않습니

|나의 클래스에 대한 접근권을 허용하는 다른 클래스의 프랜
ㅁ      |     =

히
드로 만듭니다. 여기서 당신을 나의 프랜드라고 선언할 수 있지만, 이것0

class PartNodef
public:
friend class PartList;// PartListS PartNode2| 프랜드로 되게

e+e.
3;

mey= StA(Friend Function)

+9 접근을 전체 클래스에 적용시키지 않고 해당
에 국한시킴니다. 여러분은 이를 전체의 클래스를
하나의 클래스의 멤버 함수를 프랜드로 선언하여

이번에는 여러분은 이런
래스의 하나 혹은 두 개의
프랜드로 선언하는 것이 ㅇ

uly

이건 아니건 프랜드 합수로 AMS 수 있습니다.


===== PAGE 538 =====
제15일 고급 상속 기능 ee 537

프랜드 함수와 연산자 중접(00600 Overloading)

[리스트 15.1은 연산자 +를 재생하는 Suing 클래스를 제공하였습니다. 또 상수
} 포인터를 취하는 생성자를 제공하였는데, 문자열 객체가 0 형태로 만들어지

니다. 이렇게 하면 여러분은 문자열을 만들고 거기다 0 형태

ae 고
에
SS
ae,
70h
을
x2 0
ty

그러나 여러분이 할 수 없었던 AS 0 형태의 문자열을 만
써서 거기다 붙이는 것입니다. 즉,
char cStringL[] = {"Hello"};

String sString("World");
String sStringTwo = cString + sString ; // 오류

rn
Aq
An
x
ne
a
mY
mur

C 형태의 문자열은 재생된 연산자 +를 제공해 주지 않습니다. 10일째 이야기했듯
이. 090008 + sString? 이야기할 때 ojo) Ae 호출하는 것은
050108.006080[0『+(690108)입니다. 여러분은 억제 C 형태의 AAAS operator+()
를 호출할 수 없으므로 이는 컴파일러 오류를 발생시킴니다.

이런 문제는 9078안에 프랜드 함수를 선언하여 = 수 있는데 두 개의 문자열 객

ㅇ
하고 두 개의 문자열 객체를 ALBEE operators 호출하여 문자열 객체로 va
ㅇ

—

이 예제를 컴파일 하려면 [리스트 15.1]의 33번부터 123번 Se [리스트 15.8]의 33번
줄 뒤로 복사하시오.

[리스트 15.8] 프랜드의 020하아+

// [리스트 15.87 프랜드의 6ㅎ66『ㅠ810ㅠ+

1

2:

3: #include <iostream.h>
4: #include <string.h>


===== PAGE 539 =====
938 ee 제3주

Dt

6: // 문자열 클래스
7: class String
8: f

9: public:

10:   // constructors
108   String);

12:   String(const char *const);
13:   String(const String &);
4:   string);

155

16:   // overloaded operators

17%   char & operatorL](int offset);

18:   char operatorL](int offset) const;

19%   String operator+(const String&);

20:   friend String operator+(const String&, const String&);
21%   void operatort+=(const String&);

22:   String & operator= (const String &);

25s

24:   // General accessors

25:   int GetLen()const { return itsLen; }

26:   const char * GetString() const { return itsString; 3
20:

28: private:
29:   String (int); //private constructor
30:   char * itsString;

312   unsigned short itsLen;
32: JF
33:

34: // NBS BASES rhs 주가하여

35: // NEE BIS 생성

36: String String::operator+(const String& rhs)
37: ¢

58:   int totalLen = itsLen + rhs.GetLen();

39:   String temp(totalLen+1);

40:   for (int i = 0; i<itsLen; i++)

AN:      tempLil = itsStringlil;
42:   for (int 1 = 0; j<rhs.GetLen(Q); j++, i++)
43:      tempLil = rhsljl;
44:   tempLtotalLenJ='\0';
45:   return temp;
46: }
47:

48: // 새로운 문자열을 rhs 추가하여
49: // 새로운 문자열 만들
50: String operator+(const String& lhs, const String& rhs)


===== PAGE 540 =====
세15일 고급 상속 기능 ee 539

ale €

525   int totalLen = Lhs.GetLen() + rhs.GetLen();
535   String temp(totalLent1);

54:   for (int i = 0; i<lhs.GetLen(); i++)

Doe      tempCil = lhsCil;

56:   for (int j = 0; j<rhs.GetLen(); j++, i++)
Divs      tempLi] = rhs[jJ;

58:   temp[totalLen]='\0';

595   return temp;

60: }

61:

62: int main()

652 £

64:   String s1("String One ");

65:   String s2("String Two ");

66:    char *c1 = { "C-String One " Be

67:   String s3;

68:   String s4;

69:   String s5;

70:

Tie   cout << "st: " << s1.GetString() << endl;
(22   cout << '"s2: " << s2.GetString() << endl;
(ele    cout << "cl: " << 61 << endl;

74:    s3 = 61 + 52;

755   cout << '"s3: " << s3.GetString() << endl;
16:    54 = 651 + 01;

70   cout << 641 " << s4.GetString() << endl;
78:   65 =c1+s1;

19%   cout << '"s5: " << s5.GetString() << endl;
80: return 0;

812 3

(aa

TE 51: String One
s2: String Two
c1: C-String One
s3: String One String Two
s4: String One C-String One
s5: C-String One String Two

operator+S 제외한 BE 문자열 메쏘드는 [리스트 15.1]과 다를 바가 없는데
따라서 이 부분은 제외하였습니다. 20번 줄에서 새로운 operator+7} 두 개의
상수 문자열 참조자를 취하며 문자열을 반환하도록 재생되었는데 이는 프랜드 함
수로 선언되었습니다.



===== PAGE 541 =====
540 ee ABs

이 operator+t= 어떤 클래스의 멤버 함수도 아닙니다. Serings} 클래스 내에서 프랜
드로 선언되었으므로 다른 함수원형은 불필요합니다.

50 - 60에 거쳐 operator} 구현이 이루어졌습니다. 앞의 operator+s} 비슷한데 단
지 두 개의 문자열을 취하고 범용 접근자 메쏘드들을 통해 접근된다는 점이 다릅
니다.

구동 프로그램은 78번 줄에서 이 함수의 사용법을 보여주는데 operatort Bo] C 형
태의 문자열에서 호출됩니다.

프랜드 함수
friend 예약어를 사용하고 함수의 완전한 명세를 사용하여 함수를 프랜드로 선언합니다.
함수를 프랜드로 선언한다고 하여 this a 접근하는 프랜드 함수가 주어지는 AS
아니고 전용과 보호 멤버 자료 및 함수어       접근하는 권한을 줍니다.
예제 :
class PartNode
&
friend void PartsList::Insert(Part *); // 다른 클래스의 멤버
// 함수를 프랜드로 만들
friend int SomeFunction();    // 전역 함수를 SHES 만들
3;

삽입 연산자!06600100 Operator) 중첩
이제 여러분은 마지막으로 90008 클래스에 00를 적용할 시간이 되었습니다. 지
금까지 여러분은 문자열을 출력할 때 다음과 같이 썼습니다.
cout << theString.GetString(;
이제 어느 정도 도사 경지에 이르렀으니 이런 식으로 써야 합니다.
cout << theString;

dig 쓰기 위해 여러분은 operator<<NS 중복해야 합니다. 18일째에 여러분은
모든 입출력 스트림을 가지고 작업을 하는 입출력에 대해 공부할 것입니다. 당분

간 [리스트 15.9]2] 예제를 보고 어떻게 operator<<7} 프랜드 함수를 사용하여 재
생되는지 살펴봅시다.


===== PAGE 542 =====
제15일 고          ee 541

qu

상속 7

에

[리스트 15.9] operator<<() 중복

1: #include <iostream.h>

2: #include <string.h>

3:

4: class String

as t

6: public:

(e    // constructors

Se    String ();

9:    String(const char *const);

10:   String(const Sting &);

alae   “String();

123

135:   // overloaded operators

14:   char & operatorL](int offset);

3 (yk   char operatorL[](int offset) const;

16%   String operatort+(const String&);

a WA   void operator+=(const String&);

18:   String & operator= (const String &);

19:   friend ostream& operator<<( ostream& theStream,String& theString);
20:   // General accessors

21%   int GetLen()const { return itsLen; }

22:   const char * GetString() const { return itsString; }
23:   // static int ConstructorCount;

24:

25: private:

26:   String (int); // private constructor

27:   char * itsString;

28:   unsigned short itsLen;

29:

50: }

512

32: ostream& operator<<( ostream& theStream,String& theString)
553 £

34:    theStream << theString.GetString();
358    return theStream;

56: }

37: int main()

358: <

359:    String theString("Hello world.");
40:    cout << theString;

41: return 0;
42: }



===== PAGE 543 =====
542 ee 제3주

겔과  Hello world.

분섹 ^   지면을 절약하기 위해 Strings] 메쏘드는 빼버렸는데 바로 전 예제와 다를
바가 없습니다. 19번 줄에서 operator<<t= ostream 참조자, String 참조자를

취하고 ostream FAAS 반환하는 프랜드 함수로 선언되었습니다. 이는 90008의
멤버 함수가 아님을 주의하십시오. 060600의 참조자를 반환하는데 따라서
operator<<°] SHS 연결할 수 있게 합니다. 즉,
cout << "myAge: " << itsAge <<" year.";
입니다. 32 - 3681 줄에서 프랜드 함수의 구현이 이루어졌습니다. 이 모든 것이
BAAS 060600에 제공하는 세세한 FAS 은폐하는 것이고 또 그래야만 합니
다. 18일째 00000101>>와 이 연산자의 재생에 대해 공부할 것입니다.

오늘은 포함된 객체에서 어떻게 함수기능을 대리할 것인가를 배웠습니다. 또 하
를 포함이나 전용 상속을 사용하여 다른 클래스의 관점에 의한 구현

2 1°

나의 클래스를

방법을 보있습니다. 포함은 새로운 클래스는 포합된 클래스의 Bed 멤버에 대
한 접근 권한을 가지지 않는다는 ial 제한적이며 포함된 객체의 멤버 함수를

중복할 수 없습니다. 포함은 전용 상속보다 사용이 간편한데, 가능할 때마다 사용
되어야 합니다.

야 합니다

여러분은 또 어떻게 프랜드 함수나 프랜드 클래스를 사용하는지를 배웠습니다
프랜드 함수를 사용하여 연산자들을 재생하는 것을 배웠고 새로운 클래스가 마치
내장된 클래스가 그러하듯 cous 사용하는 것을 보았습니다.

범용 상속은 “한 종류“, 포함은 “하나를 가진"이고 또 전용 상속은 * - 의 용어로
구현된"이라는 표현들을 갖습니다. “대리"라는 관계는 포함이나 전용 상속을 통해
표현           좀더

1 일반적입니다.

O&A
Q "한 종류"와 “Ue 가진”과 “ - 의 관점으로 구현된”이라는 용어를 구별하는 것이 왜
중요한가요?
A 0++의 요점은 잘 설계된 객체 지향 언어 프로그램을 만드는 것입니다. 이 WAS
즉석에서 잘 구현하는 것은 여러분이 만들려고 하는 것을 보다 현실에 가깝게 설계


===== PAGE 544 =====
제15일 고급 상속 기능 ee 543

하는데 도움을
본

줍니다. 더 나아가 이해심 있게 잘 설계된 프로그램은 나중에 코드
에도 그대로 반영됩

aud.

A 현대 프로그래밍에 대한 도전은 복잡성을 극복하는 것입니다. 블랙박스를 많
들          드의 자세한 부분에 신경 쓰지 않아도 되고, 복잡성을
수 있습니다. 포함된 클래스는 그 자세한 사항을 은폐합니다. 전용 상속은 4

왜 모든 클래스를 그들이 사용하는 클래스의 프랜드로 만들지 않습니까?
A

하나의 클래스를 다른 클래스의 프랜드로 만드는 것은 자세한 사항을 드러내고 a
숄화를 AAG. 이상적인 것은 가능한 한 많은 상세한 부분을 다른 클래스로
브

©
ue

함수가 중첩된다면 각각을 프랜드로 만들 필요가 있습니까?
A 그렇다. 여러분이 함수를 재생하고 그들을 다른 클래스에 대한 프랜드로 만
접근을 허용하고자 하는 각각의 형태에 대해 friends 선언해야 합니다.

띠0
Bh
rh

여러분이 얼마나 잘 이해하였는가
수 있는 연습 문제들로 구성되어
음에 대답을 할 수 있도록 노력하

ㆍ 한 SHAE 관계를 만들어 봅시다.
% 하나를 가진"이라는 관계를 만들어 봅시다.
3. 포함과 대리의 차이점은 무엇입니까?

% Dog0| 80\의 프랜드라면 BoyE 060의 프랜드입니까?

8. Dog0| 80의 프랜드이고 16010『가 009으로부터 파생됐다면 Terrier= 80\의 프랜
드입니까?


===== PAGE 545 =====
544 ee 제3주

9. 009이 Boy2| 프랜드이고 Boy Horse2| 프랜드일 때 000은 |10[56의 프랜드입니
까?
10. 프랜드 함수의 MAS 어디에 나타나야 합니까?

연습 문제
1, 문자열 aol 자료 WHS 포함하는 클래스, AnimalS 선언하십시오.
2 배열인 BoundedArray 클래스를 선언하십시오.
3 배열의 용어로 선언된 클래스 SetS 선언하십시오.
4 (리스트 15.11)의 OS operator))S 가진 String 클래스를 사용하여 수정하십시오.
$ 버그잡기

1:#include < iostream.h>
zclass Animal;

2
3
4:
5: void setValue(Animal&, int);
6:
7
8

zclass Animal
0006
10: public:
11   int GetWeight()const { return itsWeight; }
12: int GetAge() const { return itsAge; +
13:private:
14: int itsWeight;
15: int itsAge;
16:3;
Ave
18:void setValue(Animal& theAnimal, int theWeight)
19:
20: friend class Animal;
21: thdAnimal.itsWeight = theWeight;
222)
25:
24:int main()
2524
26: Animal peppy;
27: setValue(peppy,5);
28: return 0;
29:3

6 5H 문제를 컴파일되도록 수정하십시오.


===== PAGE 546 =====
IP

제15일 고급 상속 기능 ee 545

ne

7 버그잡기

1:#include < iostream.h>

:class Animal;

2
3
4:
5: void setValue(Animal&, int);
6:void setValue(Animal&, int, int);

8

8:class Animal

ae

10: friend void setValue(Animal&, int);

11:private:

12: int itsWeight;

13: int itsAge;

T4233

132

16:void setValue(Animal& theAnimal, int theWeight)

Tsk

18: theAnimal.itsWeight = theWeight;

191)

20:

ale

22:void setValue(Animal& theAnimal, int theWeight, int theAge)
23524

24: theAnimal.itsWeight = theWeight;

25: theAnimal.itsAge = theAge;

26:3

20%

28: int main()

293

30: Animal peppy;

31: setValue(peppy,5);

32: setValue(peppy,7,9);

33: return 0;

348}

8. 7번 문제의 잘못을 수정하여 컴파일되도록 하십시오.


===== PAGE 547 =====
가는 페이지입니다



===== PAGE 548 =====
Al



===== PAGE 549 =====
548 ce 제3주

충분한 이해 없이도, 화면에 SAS 하기 위해 coutS 사용하였
력받기 위해 00을 사용하였습니다. LSS 다음을 배옵니다.

스트림(5『680))에 대한 개괄

0++은 자체의 언어 안에 화면이나 파일에 ARS 쓰는 방법, 혹은 =
로 읽어들이는 We 가지지는 않습니다. 하지만 이 부분은 Ct

로, CHS 이 입출력 부분을 jostream 라이브러리에 가지고 있습니다.

입출력을 자체 언어 속이 아니라 라이브러리로 가지는 것은 언어가 “플랫폼에 독
립적"으로 되게 하는 이점이 있습니다. 다시 말하면 여러분은         만
들고 다시 선 위크스테이션에서 컴파일한 뒤 실행시킬 수 있습니다. 컴파일러 제
조자는 올바른 라이브러리를 제공하기만 하면, 모든 것이 잘 돌아갑

+
So,
제

라이브러리라는 것은 추가적인 함수기능을 제공하기 위해 여러분의 프로그램에 연결
되어 있는 OB) 파일들입니다. 코드 재사용의 가장 기본적인 형태인데 고대 프로그래
머들이 자기 무덤 벽에다 oat 1을 새기기 시작한 이래 계속 우리 Ae Wes 있습
니다.

iain selene
ostream 클래스는 여러분의 프로그램으로부터 화면으로의 자료의 SES 한 바이

EA 계속 이어지는 자료의 흐름으로 간주합니다. 스트림의 목적지가 여러분으

파일이건 혹은 화면이건 간에 그 근원지는 대개 여러분의 프로그램의 특정 부분

입니다. 스트림이 보존된다는                           =

자료변수로 부어지는 AS 의미합
모

pM
yt
~ ft
NX
NY
ta
이
도
더
×
4
xy
°
Hu
S|
호
i)

스트림의 하나의 기본적인 BRE 자료들을 왔다 갔다 하게 하는 문제를 캡슬화
하는 것입니다. 일단 스트림이 만들어지면 여러분의 프로그램은 스트림을 가지고


===== PAGE 550 =====
제16일 스트림 ee 549

일하고, 스트림은 2H 자세한 부분을 처리합니다. [리스트 16.1이 이에 대한

Keyboard

Monitor

[그림 16.1] AEBS 통한 캡슬화

버퍼화(84001119)

디스크에 쓰는 것은(혹은 범위를 줄여 화면에 쓰는 것은) 매우 비용이 많이 Su
다. 자료를 디스크에 쓰거나 디스크로부터 읽는 것은 상대적으로 시간이 많이 걸
리고, 일반적으로 프로그램을 실행시킬 때 디스크에 입출력 동안에는 프로그램이
잠시 정지됩니다.

이 문제를 풀기 위해 스트림은 버퍼화를 합니다. 자료는 스트림 속으로 쓰여지는
데 곧바로 디스크에 쓰여지는 것이 아닙니다. 대신 스트림의 버퍼가 채워지고 버
퍼가 가득 차면 그때 한번에 디스크에 저장됩니다.

그럼에서 물이 물통의 꼭대기를 향해 떨어지고, BS 점점 가득 차는데 Bo]
바깥으로 흘러나가지는 않습니다. [그림 16.2]가 이것입니다.

물(자료)이 꼭대기에 차게 되면 수도는 잠기고 배수통이 열리면서 물이 한꺼번에
eb) 나갑니다. [그림 16.31입니다. 다시 버퍼가 비게 되면 밑바닥의 배수통
이 닫히고 수도가 다시 열리면서 또 다른 So] 버퍼 탱크로 흘러 들어옵니다. [그
림 16.4]입니다.

가끔 여러분은 물통이 가득 차기도 전에 물통을 비울 때가 있습니다. 이

방줄(6006 flush)°] 2 부릅니다. [그림 16.5]입니다.

5 a

NAL

보

때


===== PAGE 551 =====
550 ee ABF

[그림 16.2)
버퍼 채우기

[그림 16.3]
버퍼 비우기



===== PAGE 552 =====
제16일 스트림 ee 551

[그림 16.4]
버퍼를 다시 채움

[그림 16.5]
버퍼 방출



===== PAGE 553 =====
502 ee AB

스트림과 버퍼
여러분이 예상할 수 있듯이 0++은 스트림과 버퍼를 구현할 때 객체 지향적인 관
Pa ch ee A 간간 그분 ee
WH sreambul 클래스는 버퍼를 다루고 그 멤버 함수는 버퍼를 채우고, 비우고, 방출하고 그 외
조작하는 WES 제공합니다.
Bl ics SAL 스트림 SHAS 입출력하는 베이스 클래스입니다. ios 클래스는 streambut 4
체를 멤버 변수로 가집니다.
BB |91607과 ostream’ 105로부터 파생되었고, 입출력 스트림의 과정을 특히 처리합니다.
Bl iostream SAHA+ istream#t ostream 클래스의 두 개로부터 파생되었고 입출력 메쏘드를 제

공합니다.

rt

WH [51607 SHAE 파일로부터의 입출력을 제공합니다.

표준 입줄력 24HKI(Standard !/0 Object)
1094630을 포함하는 C++ 프로그램이 시작되면 4개의 객체가 생성되고 초기화됩
니다.

jostream 클래스 라이브러리는 컴파일러에 의해 자동으로 여러분의 프로그램에 주가됩
니다. 여러분이 해야 할 모든 것은 여러분의 프로그램 처음에 적절한 |
넣는 것입니다.

류 장치로 보내는 것을 다룹니다. 이것은

,]     지만 7     파일로 재지정|{6016060|되는 We] BEY
~ 애써 애가”



===== PAGE 554 =====
제16일 스트림 ee 553

재지정((601160100)

ie] 표준 장치는 다른 장치로 재지정될 수 있습니다. 표준 오류는 종종
로, 표준 입출력은 운영 시스템의 명령을 사용하여 파일로 파이프됩니다.

일

가

새로운 재지정(6601『60!1100), 파이프(『10109) 재지정은 WHS 기본장치에서 다른 장치

$0

cin&

로 전환하는 것을 말합니다. 005와 UNXOIM 재지정은 입력 재지정(<)과 출력 재지
정(>)이 있습니다.

파이프는 프로그램의 출력을 다른 프로그램의 입력으로 재지정하는 것을 말합니다.

0ㅁ05에서 재지정은 입력 재지정(<)과 출력 재지정(>)이 있습니다. 080%에서는
더 발전된 재지정 기능이 있지만 기본개념은 같습니다. 화면으로 의도된 출력을
파일에 쓰거나 다른 프로그램으로 파이프합니다. 입력은 키보드가 아니라 파일로
부터 추출될 수도 있습니다.

재지정은 1060600보다는 운영체제의 명령에 더 가깝습니다. 0++은 4개의 표준 장
치에 대한 접근 방식을 제공합니다. 이를 사용하는 것은 여러분 맘대로 입니다.

사응한 입력
범용 객체 00은 입력에 대해 책임지며 여러분이 iosteamhS 포함하면 유용하게
사용할 수 있습니다. 앞 예제들에서 여러분은 자료를 여러분의 프로그램의 변수
a  넣기 위해 재생된 추출 연산자(>>)(60180000 operator)S 사용하였습니다. 이것
은 어떻게 동작할까요? 기억하겠지만 PRS 다음과 같습니다.
int someVariable;

cout << "Enter a number: ";
cin >> someVariable;

범용 객체 cout 다음에 설명될 것입니다. 당분간은 cin >> someVariable;ol] 신경
을 쏟읍시다. cine 무엇이라 생각하십니까?

객체입니다. 왜냐하면 여러분의 프로그램에서 정의하지 않았기

문입니다. 여러분은 앞의 경험에서 cine] 추출 adore 중복했고 그 결과

는 쓰여지는 어떤 자료이건 그 자신의 버퍼에서 지역 변수 someVariablea) 넣는

yy
ro
ie
aes

of

장 명료하지 않은 AS 00이 추출 연산자를 아주 다양한 매개 변수를 가지고
생되었다는 것인데 그 중엔 int& short& long&, double&, float& char&, char*

코


===== PAGE 555 =====
554 ee 제3주

등등이 있습니다. cin >> someVariableS 사용할 때 someVariableo] 접근됩니다. 위
의 예제에서 90006\84840[6은 정수이고 따라서 다음의 함수가 호출됩니다.

istream & operator>> (int 6)
rewrrrmwmeree worn

매개 변수가 참조자로 전달되었으므로 추출 연산자

있습니다. [리스트 16.1]을 봅시다.

[리스트 16.1] 여러 FB 자료영을 CHE cin

rir

원

래

의

변

~
수

00

건

림
a

=
수

1: // [리스트 16.17 여러 종류의 자료형을 TRE cin
2:

3: #include <iostream.h>

4:

5: int main(

6:

A    int myInt;

8:    long myLong;

9:    double myDouble;

10:   float myFloat;

118   unsigned int myUnsigned;

126

13:    cout << "int: ";

14:   cin >> myInt;

155    cout << "Long: ";

16%   cin >> myLong;

17:    cout << "Double: ";

18:   cin >> myDouble;

198    Gout << "Float: ";

20:   cin >> myFloat;

218    cout << "Unsigned: ";

22:   cin >> myUnsigned;

23:

245   cout << "\n\nInt:\t" << myInt << endl;
20%   cout << "Long:\t" << myLong << endl;
26:   cout << "Double:\t" << myDouble << endl;
2s   cout << "Float: \t" << myFloat << endl;
28:   cout << "Unsigned:\t" << myUnsigned << endl;
29: return 0;

308 +

Wh int: 2

Long: 70000
Double: 987654321


===== PAGE 556 =====
제10일 스트림 ee 555

Float: 3.33
Unsigned: 25
Inte      2
Long:     70000
Double:   9.87654e+08
Float:    $255
Unsigned: 25
분석 7-11번 줄에서 각종의 변수가 선언되었습니다. 13-22번 Sopa] 사용자는 이
- 변수들에 값을 대입하고 결과가 24.28 줄에서 cours 사용하여 출력되었
습니다
출력은 변수들이 올바른 SH] 변수들에 집어넣어진다는 것을 입증하고 프로그
Ho] 여러분이 의도한 대로 동작한다는 것을 보여줍니다.
문자열
cine 또 문자 포인터(000 인수를 다룹니다. 따라서 여러분은 문자 버퍼를 만들
고 그 버퍼를 채우기 위해 cine 사용합니다. 예를 들면, 다음과 같이 쓸 수 었습

니다.

char (10404306[ㅁ503;
cout << "Enter your name: ";
cin >> YourName;

여러분이 JesseS 입력하면 변수 YourName-e- 이 이 로 로 로 Ode 채워집
니다. 마지막 문자는 4011입니다. 00 자동적으로 Bee NOLL 괄법니다
따라서 여러분은 문자 길이 이외에 널 문자를 넣을 공간을 하나 더 추가해야 합
니다. 널은 '문자열의 끝'이라는 표시를 표준 라이브러리 함수에게 알려주는데 21
일째에 공부합니다.

문자열의 문제
결국 00은 동작이 되었고 여러분은 여러분의 완전한 이름을 문자열에 넣었
SRE 것입니다. cine 공백 문자를 분리자로 간주합니다. cine 빈칸이나 개행
문자를 보았을 때 매개 변수의 입력이 끝났다고 간주하고 그곳에 WS 넣습니다.
[리스트 16218 봅시다.


===== PAGE 557 =====
556 ee 제3주

[리스트 16.2] 하나 이상의 문자를 cin 쓰기

1: // [리스트 16.27 하나 이상의 문자를 617에 쓰기

2%

3: #include <iostream.h>

a:

5: int maind

6: ¢

:    char YourNameL50];

8:    cout << "Your first name: ";

9:    cin >> YourName;

102   cout << "Here it is: " << YourName << endl;
115   cout << "Your entire name: ";

122   cin >> YourName;

AS:   cout << "Here it is: " << YourName << endl;
14: return 0;

152 +

겔과 Your first name: Jesse

Here it is: Jesse
Your entire name: Jesse Liberty
Here it is: Jesse

=I

H

1

불셀 Te SAA 사용자의 WAS 받기 위한 문자 배열이 만들어졌습니다. 8번
개                                         ~  럼

줄에서 사용자는 하나의 이름을 입력하고 그 이름은 출력에서 보는 것처

|르게 입력이 됩니다.
Ie 줄에서 사용자는 다시 입력을 하는데 이번에는 전체 이름을 다 넣었습니다.

cine. 이 입력을 다 읽은 뒤 그 이름 사이에 공백 문자가 있음을 알고 첫 번째
단어 다음에 널을 넣고 입력을 마칩니다. 이는 사용자가 원했던 바가 아닙니다.
왜 이런 식으로 되는지 이해하기 위해 [리스트 16.3]을 봅니다.

[리스트 16.3] 다중 입력

1
(4
3
4:
5
6:
7
8
9

// [리스트 16.31 다중 입력
#include <iostream.h>

int main()

{
int myInt;
long myLong;
double myDouble;


===== PAGE 558 =====
제16일 스트림 ee 557

10:   float myFloat;
1:   unsigned int myUnsigned;
12:   char myWord[50];
1S
14:   cout << "int: ";
15:   cin >> myInt;
162   cout << "Long: ";
As   cin >> myLong;
18:   cout << "Double: ";
19%   cin >> myDouble;
20:   COUL.<S "Floats >;
21:   cin >> myFloat;
Ze:   cout << "Word: ";
235°   cin >> myWord;
24:   cout << "Unsigned: ";
25:   cin >> myUnsigned;
26:
er:   cout << "\n\nInt:\t" << myInt << endl;
28:   cout << "Long:\t" << myLong << endl;
29:   cout << "Double:\t" << myDouble << endl;
30:   cout << "Float:\t" << myFloat << endl;
a1:   cout << "Word: \t" << myWord << endl;
325   cout << "Unsigned:\t" << myUnsigned << endl;
55:
34:   cout << "\n\nInt, Long, Double, Float, Word, Unsigned: ";
35:   cin >> myInt >> myLong >> myDouble >> myFloat >> myWord >> myUnsigned;
562
3:   cout << "\n\nInt:\t" << myInt << endl;
38:   cout << "Long:\t" << myLong << endl;
59:   cout << "Double:\t" << myDouble << endl;
40:   cout << "Float:\t" << myFloat << endl;
41:   cout << "Word: \t" << myWord << endl;
4281   cout << "Unsigned:\t" << myUnsigned << endl;
43: return 0;
44: }
결과  ints 2
Long: 30303
Double: 393939397834
Flodite 3235

Word: Hello
Unsigned: 85


===== PAGE 559 =====
558 ce 제주

Int:                            2

Long:                           30303
Double:                         3.93939e+11
Float:                          3233

Word:                           Hello
Unsigned:                       85

Int, Long, Double, Float, Word, Unsigned: 3 304938 393847473 6.66

bye -2

Int:                            3

Long:                           304938
Double:                         3.93847e+08
Float:                          6.66

Word:                           bye
Unsigned:                       65534

100

셀 다시 한번 여러 개의 변수가 만들어집니다. 이번에는 문자 배열이 포함되어
있습니다. 사용자가 입력을 하고 출력이 충실하게 됩니다.

34번 줄에서 사용자는 입력을 합니다. 각 입력어는 Bra 저장됩니다. ane
력시 각 단어를 입력 변수에: 맞는 입력으로 간주하고 다중 YAS 받습니다.
일 cinco] 전체의 입력을 하나의 형으로 하여 변수에의 입력으로 간주한다면 이렇
게 여러 개를 입력하는 것이 불가능합니다.

35번 줄에서 요구된 마지막 객체는 unsigned 정수형이지만 사용자는 -2를 입력하
였습니다. cin& unsigned 정수형으로 간주하기 때문에 -2의 비트 형태는 unsigned
정수형으로 간주되고 004으로 출력될 때는 65534로 출력됩니다. 40918000 65534는
910060의 -2입니다.

이번 장의 마지막에서 다중 단어를
는지 볼 것입니다. 지금으로선 다음
문자열 연결을 처리합니까?”

이뽀   ‘a,  ro

전체 문자열을 어떻게 버퍼로 저장하

포함한
의 의문이 일어납니다. “어떻게 추출 연산자가

밴

istream 객체 참조자를 반환하는 operator>>
cin2} 반환값은 10680 객체에 대한 참조자입니다. 00 그 자체가 10680 객체 이므
로 추출 연산자의 반환값은 다음 추출의 입력이 될 수 있습니다.
int VarOne, varTwo, varThree;

cout << "Enter three numbers: "
cin >> VarOne >> varTwo >> varThree;


===== PAGE 560 =====
제16일 스트림 ee 559

여기서 cin >> VarOne >> varTwo >> 1\0711066를 만들면 처음의 추출이 계산됩니
다. (cin >> VarOne ) 반환값은 CHE istrream 객체이고 그 객체의 추출 연산자는

vatTwo 변수를 취합니다. 마치 아래와 같습니다.

(Ccin >> VarOne) >> varTwo) >> varThree;

이 기법은 후에 cous 배울 때 보게 됩니다.

의 또 다른 멤버 함수

operator>> 재생에 추가하여 00은 다른 여러 개의 멤버 함수를 가집니다. 이 멤버
함수들은 입력에 대한 더 훌륭한 통제가 필요할 때 사용됩니다.

단일 문자 입력
노자 참조자를 취하는 0000106>>는 표준 입력으로부터 하나의 문자를 받을 때 ap
용됩니다. 멤버 함수 ce 하나의 문자를 얻을 때 사용되는데 두 가지 방법으
로 사용됩니다. 800는 반환값을 사용하는 경우가 있는데 이때에는 매개 변수가
없고, 또 다른 경우는 문자의 참조자를 사용합니다.

get()S 매개 변수 없이 사용하는 법

는 것입니다. 이때에는 문자의

로 반환하고, 과일의 ga) 도달하면 EOF(end of file) 반환합니다. 매개 변수
없이 쓰는 방법은 잘 안 쓰임니다 여러 개를 입력할 때 880를 연결해서 쓰는
것이 불가능한데 왜냐하면 반환값이 1090600이 아니기 때문입니다. 따라서 다음
은 동작하지 않습니다.

cin.get() >> myVarOne >> myVarTwo;           Ti

자 OFS
a7 ㄴㅋㅁ

(cin.get() >> 100780000)의 반환값은 1060600이 아니라 정수형입니다. 사용 예가
[리스트 164]에 있습니다.

of

[리스트 16.4] 매개 변수 없이 00[0를 사응하는 법

// [리스트 16.47 매개 변     수 없이 get 사용하는 법
#include Stostresinch>

int main()
{
char ch;

AOU rWD =


===== PAGE 561 =====
560 co 제주

iC    while ( (ch = cin.get()) != EOF)
8:    {

9:       cout << "ch: " << ch << endl;
10:   }

aie   cout << "\nDone!\n";

V2:   return 0;

133 +

이 프로그램을 끝내려면 키보드에서 파일 끝이라는 표시를 보내야 합니다. 006에서는

441+2이고 4141%엑석는 6804+ㅁ입니다.
지지 사직

결과  Hello

ens i
ch:e
ch: L
chs! t
chs ©
ch:
World
ch: W
chs 0
che r
chs Ｌ
chi d
ch:
Cotrl=z)
Done!
분석 6번 줄에서 지역 변수가 선언되었습니다. while 순환문에서 07.880으로부터
==

받은 입력을 애에 저장하고 문자가 8야가 아니면 SAS 합니다. 하지만
이 SAS 마지막 So] 읽혀질 때까지 버퍼에 저장됩니다. 일단 8야를 만나면

(0008에서는 000+2이고 080%에서는 001+0ㅁ입니다.) 순환문이 끝납니다.
주의할 것은 모든 iostreamo] 880 MAS 지원하는 것은 아니라는 것입니다.

get] 입력으로 문자가 전달되었을 때 그 문자는 입력 스트림의 다음 문자로 al
워집니다. 반환값은 1090680 객체이며 이런 형태의 860는 [리스트 16.5]처럼 연결

될 수 있습니다.


===== PAGE 562 =====
제10일 스트림 ㅇㅇ 561

[리스트 16.5] 매개 HAS HIE get()

1: // [리스트 16.5] 매개 HAS 가지는 get)
2: #include 개가

3

4: int main()

De it

6     char-a, b, c;

if

8:    cout << "Enter three letters: ";
98

10:   cin.get(a).get(b).get(c);

Vs

V2?   cout << "a: " << a << "\nb: " << 6 << ""\nc: "<< c << endl;
13   return 0;

14: }

겔과  Enter three letters: one

분석  번 줄에서 세 개의 문자 변수가 만들어집니다. 10번 줄에서 02.800이 A

번 호출됩니다. 처음에는 00.800)가 호출됩니다. 처음의 글자를 8에 저장하

고 00을

반환한 뒤 이것이 끝나면 00.800)을 호출하고 다음 문자를 po] 저장합

니다. 마지막에는 00.8800)가 호출되고 입력값은 co) 저장됩니다.

00.8660)는 00으로 계산이 되므로 여러분은 다음같이 쓸 수 있습니다.

cin.get(a) >> 6;

7A] cin.get(a)= 00으로 계산이 되므로 두 번째 구는 cin >> 로 됩니다.

00
00

DON'T

공백 문자를 건너될 때 SS 연산자(>>)를 사용합시다.

nu
공백 문자를 포람하여 모든 문자를 살펴볼 필요가 있으면 매개 변수 없는

=.
eB
변수 없는 oct GHATS AE BA 다소 불명확합니다.



===== PAGE 563 =====
562 ee 제3주

표준 입력으로부터 문자열을 받아들이는 법
문자 배열을 채우기 위해 추출 연산자가 사용될 수
멤버 함수를 사용해서 가능합니다.

있는데 880과 8601060라는

860의 마지막 형태는 3개의 매개 WES 가집니다. 첫째 매개 변수는 문자 배열

에 대한 포인터이고 두 번째 매개 변수는 읽어들일 문자의 최대 개수에 하나를

더한 값이고 마지막 매개 변수는 종료 문자입니다.

만일, 여러분이 두 번째 매개 변수로 20을 써넣었다면 880는 19개의 BAS 읽고
문자열의 널 종료값으로 끝낼 것입니다. 그리고 이는 첫 번째 매개 변수에 저장
됩니다. 세 번째 매개 변수인 종료 문자는 기본값이 개행 문자000입니다.

만일 문자의 최대 개수만큼이 읽어지기 전에 종료 문자를

종료 문자는 버퍼에 남아 있습니다.
[리스트 16.6|에서 이를 살펴봅시다.

[리스트 16.6] 문자 HAS 가지고 0010 사응하기

만나면 nullo] 쓰여지고

1: // [리스트 16.6] 문자 배열을 MAID get O 사용하기
2: #include <iostream.h>

3

4: int main(

a 고

6:    char stringOne[256];

te    char stringTwol256];

8:

9s    cout << "Enter string one: ";

10:   cin.get(stringOne,256) ;

A418   cout << "stringOne: " << stringOne << endl;
128

15:   cout << "Enter string two: ";

14:   cin >> stringTwo;

15:   cout << "StringTwo: " << stringTwo << endl;
16:   return 0;

lite +

Enter string one: Now is the time
String One: Now is the time

Enter string two: For all good
String Two: For


===== PAGE 564 =====
제16일 스트림 ㅇㅇ 563

EBAY ㅇ 7번 줄에서 두 개의 문자 Wo] 만들어졌습니다. 9번 줄에서 사용자는
문자열을 입력하고 10번 줄에서 00880이 호출됩니다. 첫 번째 매개 변수
는 채위야 할 버퍼이고 두 번째 매개 변수는 880이 받아들일 문자의 최대 개수
더하기 일의 값입니다.0배이 들어갈 자리) 세 번째 매개 변수의 기본값은 개행
문자입니다.

사용자는 “Now is the time”S 입력합니다. 사용자가 BAS 개행 문자로 끝냈으
므로 그 CBS stringOne= 들어가고 뒤따라 NULLS] 들어갑니다.

사용자는 13번 줄에서 또 문자열을 입력하고 이번에는 추출 연산자가 사용됩니
다. 추출 연산자가 처음의 공백 문자까지의 모든 문자를 받아들이므로 NULLZ
끝나는 1@마는 문자열이 두 번째 문자열에 저장되는데 이는 물론 의도하지 않았
던 것입니다.

이 문제를 푸는 또 다른 방법은 800160인데 [리스트 16.7]에 있습니다.
이

[리스트 16.7] getline() 사웅하기

// 리스트 16.73 getline) 삭용하기
#include <iostream.h>

1

2

3

4: int main()

Birt

6    char stringOne[256];
ié     char stringTwol256];
8:    char stringThree[256];

98

10:    cout << "Enter string one: ";

te   cin.getline(stringOne,256) ;

12:   cout << "stringOne: " << stringOne << endl;

134

16:    cout << "Enter string two: ";

15905   cin >> stringTwo;

16%   cout << "stringTwo: " << stringTwo << endl;

ws

185    cout << "Enter string three: ";

19%   cin.getline(stringThree,256) ;

205   cout << "stringThree: " << stringThree << endl;
21   return 0;

228 +



===== PAGE 565 =====
564

eo 제3주

겔     Enter string one: one two three

(a

문자)를 가집니다. 이 버전의 880는 문자

stringOne: one two three

Enter string two: four five six

String two: four

Enter string three: stringThree: five six

셀  이 예제는 아주 자세히 살펴보아야 합니다. 놀랄 만한 So] 있습니다. 68H
줄에서 세 개의 문자 배열이 선언되었습니다.
10번 줄에서 사용자는 문자열을 입력하고 이 문자열을 860060에 의해 읽혀집니
다. get 같이 8601060은 버퍼와 최대 문자 ATS 취합니다. 단 880과는 달
종료 개행 문자는 읽혀진 뒤 버려집니다. 800에서는 종료 개행 문자가 버려지지
나 eo
14번 줄에서 사용자는 다시 YAS 하고 이번에는 추출 연산자가 사용됩니다. 사
용자는 104 five 9를 입력하고 A 번째 글자 10ㅁ가 9000810에 입력됩니다. =
이어 Enter string three7} 출력되고 8601060이 다시 호출됩니다. 876 six 아직 입
력버퍼에 남았고 곧바로 AY 문자까지 읽혀집니다. 8001060는 E42! stringThree
7} 20번 줄에서 출력이 됩니다.
사용자는 세 번째 문자열을 WAS 겨를
호출은 15번 줄의 추출 연산자를 호출한
해 채워지기 때문입니다.

추출 연산자는 처음 공백 문자가 나올 때까지 읽어들인 뒤 문자 배열에 단어를
넣습

데 왜냐하면 두 번째의 800060

없는
입력 버퍼에 남아 있던 문자열에 의

의
호
후

자의 값을 반환합니다. 두 번째 버전은 하나의 문자 참조자를 취하고
참조자에 의한 60600 객체를 반환합니다.      =

마지막 Waal Geox 문자 배열, 취하는 문자의 개수, 종료 문자(기본값 MY
최대 문자 개수보다 하나 작은 문자
읽어들이거나 혹은 종료 문자        까지 읽어들입니다. 880이 종료 문자
만나면 종료 문자를 입력 버퍼에 남기고 입력을 중지합니다.

8601060도 역시 세 개의 매개 변수를 취합니다. 채울 버퍼, WAS 문자의 개수보
다 하나 큰 숫자, 그리고 종료 문자입니다. gets} SAV getline 종료 EAS
버려버립니다.

[멤버 함수 880이 중첩봅니다. 첫 번째 버전이 서는 베개 wee 취하지 않고 받
들인 문              두

rir

furl 00
0
더,
ay,
au

=a


===== PAGE 566 =====
제16일 스트림 ㅎㅎ 565

cin.ignore() 사응하기

종종 여러분은 줄의 끝801)이나 파일 끝8009을 입력할 때까지 줄에 문자가 있
는 것을 버리고 싶은 때가 있을 것입니다. 180000라는 멤버 함수가 이 목적에 사
용됩니다. 1800060는 두 개의 매개 변수를 가지는데 하나는 무시해야할 최대의 문
자 개수와 또 하나는 종료 문자입니다. 만일 100006(80,"0'이라고 입력하면 may
문자를 만날 때까지 80개의 문자는 버려집니다. 개행 문자가 다음으로 버려지고
ignore 끝납니다. 예제를 봅시다.

[리스트 16.8] ignore() 사응 off

// 리스트 16.831 ignore() 사용 예
#include <iostream.h>

1

2

3

4: int main()

aft

6:    char stringOne[255];
7     char stringTwol255];
8

9:    cout << "Enter string one: ";

10:   cin.get(stringOne,255) ;

112   cout << "String one:" << stringOne << endl;
12:

13:   cout << "Enter string two: ";

14:   cin.getline(stringTwo,255) ;
158   cout << "String two: " << stringTwo << endl;

16:

re   cout << "\n\nNow try again...\n";

18:

ee   cout << "Enter string one: ";

20:   cin.get(stringOne,255);

2:   cout << "String one: " << stringOne<< endl;
228

235:    cin.ignore(255,'\n');    Batter   Cleary
24:

20%    cout << "Enter string two: ";

26:   cin.getline(stringTwo,255);

ere   cout << "String two: " << stringTwo<< endl;
28:   return 0;

29: }



===== PAGE 567 =====
566 ee 제3주

결 1 fh Enter string one: once upon a time
String one: once upon a time
Enter string two: String two:

Now try again...

Enter string one: once upon a time
String one: once upon a time

Enter string two: there was a
String two: there was a

(aa

By < 7번 중에서 두 개의 문자 배열이 만들어집니다. 9번 줄에서 사용자는
Once upon a 0006라 입력하고 EntrS 입력합니다. 10번 줄에서 get()°] 이
BAS 읽는데 사용됩니다. get stringOneS 채우고 개행 문자를 만나 끝나는데
MY 문자는 버퍼에 그대로 seuc.
13번 줄에서 사용자는 다시 입력을 합니다. 하지만 14번 줄의 8601060에서는 이미
버퍼에 있는 개행 문자를 보고 즉시 끝나버립니다. 따라서 사용자는 글을 입력할
겨를이 없습니다.
19번 줄에서 사용자는 다시 처음에 입력한 문장을 입력합니다. 이번에는 23번 줄
에서 180060가 사용되고 개행 문자를 먹어 AGC. 따라서 26번 줄에서 다시
8601060이 사용될 때 버퍼는 깨끗이 비어있고 사용자는 다음 SS 입력할 수 있
습니다.

peek()2+ putback()
입력 객체 cine 간단한 두 개의 메쏘드를 더 가지고 있습니다. 보기만 할 뿐 다.
음 문자를 추출하지는 않는     는 함수와 입력 스트림에 문자를 삽입하는

putbackOYUG. 예제를 봅시다.

"|

[리스트 16.9] 666(0와 putback()

// [리스트 16.93 066(()와 putback©
#include <iostream.h>

int main()
:
char ch;
cout << "enter a phrase: ";
while (cin.get(ch) )
£

~ 60 기 AU FWD


===== PAGE 568 =====
제16일 스트림 ee 567

10:      if (ch == '!')

11:        cin.putback('$');

12s     else

13%        cout << ch;

14:      while (cin.peek() == '#')
152        cin.ignore(1,'#');

16:   +

17:   return 0;

13: >

결과  enter a phrase: Now! is#the!time#for! fun#!
NowSistheStimefor$fun$

AY <번 중에서 문자형 변수 애가 선언되고 TH 줄에서 사용자는 문장을 BS
니다. 이 프로그램의 목적은 느낌표(!)를 달러 기호(9)로 바꾸고 수

를 제거하는데 있습니다.

이 프로그램은 파일 끝을 만날 때까지 순환합니다(00880는 파일 끝에서 og 반

환합니다:) 현재의 문자가 느낌표이면 버려지고 입력 버퍼로 $ 기호가 집어넣어집

니다. 그리고 OSS 읽습니다. 현재의 문자가 느낌표가 아니면 출력이 됩니다.
음 문자가 살펴지고 샵60 문자가 나타나면 제거됩니다.

이렇게 하는 것이 효율적인 것은 아닙니다(그리고 처음에 샵문자는 발견을 못합니다)

단지 이 메쏘드가 어떻게 동작하는지 예를 보인 것뿐입니다. 좀 불명확하긴 한데 실제

어떻게 쓸 것인지 걱정하지는 We. 일단 기억해 두면 조만간 쓸 일이 생길 것입니다

peekQ)SF putback()2 문자열 또는 다른 TRESS 분리하는 떼 쓰이는데, ye 들면
컴파일러를 만들 떼 쓰입니다.

(aa

iad
a,
ker
a

be

cout= 출력
문자열, 정수, 그 외 다른 PRES 화면에 eat 때 삽입 연산자(<<)와 함
께 cout 사용하였습니다. 자료를 규격화하고 칸을 정열하며 숫자 자료를 십진범
과 16진법으로 표현하는 것이 키능합니다. 이번 is 이러한 AS 배움니다.


===== PAGE 569 =====
568 ec 제3주

줄력할 산줄물을 방줄함(49)
여러분은 이미 endo) 출력 visi 모두 VERE 보있습니다. 8는.698으 sha

함수 .44940를 호출하는데 이는 버퍼에 있는 모든 ARS 방출합니다. 여러분
flush) 메쏘드를, 00980 멤버 메쏘드를 호출하거나 혹은 아래와 같이 xo za

flush) WARES 직접 사용할 수도 있습니다.
cout << flush

이는 여러분이 버퍼가 비어있음을 확신하고 USS 화면에 출력할 때 편하게 사
용할 수 있습니다.

관련된 함수
Te 연산자가 sal 및 getline} 어우러져 사용할 수 있듯이 삽입 연산자는
Put) 후 함수는 하나의 문자를 출력 장치에 쓸 때 사용합니다. 240는 0560600 참조
자를 "자를 반환하기 때문에 여러분은 240를 삽입 연산자 쓰듯이 사용할 수 있습니다.
예제를 봅시다.

[리스트 16.10] put() ASH

1: // [리스트 16.103 64+() 사용법
2: #include <iostream.h>
oe
4: int main®
88 &
6:    cout.put('H').put('e').put('L").put¢'l') putC'o").putC'\n');
te    return 0;
88 +
겔과  Hello
분석 6번 줄은 이렇게 BUC. coutput(H’)= HS 화면에 출력하고 004 객체를

반환합니다. 그러면 다음이 남습니다.

cout.-put('e').put('l').put('l').put('o').put('\n');

6가 쓰여지고 THE] = cout.put(l’)...o] 남습니다. 이 과정이 반복되고 각 문자가
쓰여지며 마지막 문자(002`)가 쓰여질 때까지 cout 객체가 반환됩니다.


===== PAGE 570 =====
제16일 스트림 ee 569

walle  삽입 연산자와 비슷한더

ㅣ 단지 함수에게 최대 출력할 문자 개수를 알리
는 값을 매개 변수로 갖습니다. [리스트

16.11]을 봅시다.

[리스트 16.11] write.) 사응법

// 리스트 16.113 write() 사용법
#include <iostream.h>
#include <string.h>

int main()
<
char One[] = "One if by land";

- 60 60 기 WAU KFWYD =
© =) se we ce 0s ce ce a8 a6

= =
ny =
os …

int fullLength = strlen(One);
int tooShort = fullLength -4;
int tooLong = fullLength + 6;

a a
uu ews
… … …

cout.write(One,fullLength) << "\n";
cout.write(One,tooShort) << "\n";
cout.write(One,tooLong) << "\n";
return 0;

—_— — — «2d
co CON O
ac ss se oe
ro)

결과 One if by Land

One if by
One if by land i?!

여러분의 컴퓨터에서는 마지막 줄의 내용이 다를지도 모릅니다.

분석  TH 줄에서 문자 배열이 만들어집니다. 11번 줄에서 정수형 10116080가 문
이    자 배열의 크기로 설정되고 12-13번 줄에서 005800와 tooLong7} 각각 설정

됩니다.

니
15번 줄에서 writeQS 사용하여 문자 배열이 출력되는데 원래 문장의 길이로 출
력이 됩니다.

16번 줄에서는 출력되는 길이가 4가 모자라게 되는데 출력도 그대로 됩니다.


===== PAGE 571 =====
570 ee 제3주

ITA 줄에서 출력되는 길이가 원래 길이의 6 글자가 늘어나게 됩니다. 따라서 메
모리의 6개의 글자가 추가로 출력됩니다. 원래 문자열의 마지막은 널 문자이고
나머지 5개의 글자는 아무 값이나 출력됩니다.

2Tt(Manipulator), 플래그(『139),
124 39J=JO|(Formatting Instruction)

출력 스트림은 많은 상태 SAIS 가지고 있는데, 어떤 기수(십진법 혹은 십육진
법)를 쓸지를 결정하고, 얼마나 필드를 넓게 벌어질 것인지와, 각 필드를 채울 문
자를 결정합니다. 각 상태 플러그는 각 비트가 의미를 가지는 바이트로 구성되어
있습니다. 비트를 이러한 식으로 연산하는 방법에 대해서는 21일째 봅니다. 각
ostream2] 플래그는 멤버 함수와 조종자를 사용하여 설정될 수 있습니다.

cout.width)S 사용하는 법
여러분의 출력의 기본 넓이는 숫자, 문자 혹은 출력 버퍼의 문자열들을 출력할
만큼 충분한 공간입니다. 이 넓이를 \0010를 사용하여 바꿀 수 있습니다. \10010
는 멤버 함수이므로 000 객체에 의해 호출되어야 합니다. 바로 Hes] 출력 필드
만 바꾸고 다음은 기본 넓이 값으로 wp yd. [리스트 16.12]를 봅시다.

[리스트 16.12] 줄력의 WOE 조정하는 법

1: // [리스트 16.127 BHI 넓이를 조    정하는 법
2: #include <iostream.h>

bie

4: int main®

Ds

6:    cout << ""Start 2°,

vs    cout.width(25);

Se    cout << 123 << "< End\n";

9:

10:   cout << "Start >";

ba Be   cout.width(25);

(2:   cout << 123<< "< Next >";
13%   cout << 456 << "< End\n";
14:

190   cout << "Start 2",

16:   cout.width(4);

17   cout << 123456 << "< End\n";


===== PAGE 572 =====
제16일 스트림 ee 571

18:
19:2   return 0;
20: }

24 Df  Start >                123< End

Start >                  123< Next >456<End
Start >123456< End

a  6-84 줄의 처음의 SAS 7TH 줄에서 넓이가 25로 설정된 필드에 132 2
력합니다. A 번째 출력 줄에서 나타납니다.

출력의 두 번째 줄은 넓이가 25로 설정된 같은 필드에 123을 출력하고 다음에

456을 출력합니다. 4562 기본 넓이 값으로 출력되었습니다. 앞서 말했듯이

\1000()는 바로 다음의 출력 부분만 효과를 가집니다.

마지막 출력에서 나타난 것은 출력의 넓이보다 적게 설정된 Woe 필요한 만큼

의 넓이를 설정하는 것과 같은 효과를 지닙니다.

이 See Eee

aa

채울 문자의 설정

위에서 WYK] 보통 cout \000를 호출할 때 빈 필드를 공간으로 aed.
종종 메쏘드는 각 필드를 다른 문자로 채우고 싶은 때가 있을 것입니다. 이렇게
하기 위해 810을 호출하여 매개 변수로 채우고 싶은 문자를 전달할 수 있습니다.

[리스트 16.13]을 봅시다.

[리스트 16.13] fill) 사응하기

1: // 리스트 16.13] FillO 사용하기
2%

3: #include <iostream.h>

4:

5: int main()

6s 고

te    cout << "Start >"

8:    cout.width(25);

9    cout << 123 << "< End\n";
10:

g BEE

12:   Gout << “Start a"

Si   cout.width(25);

14:   cout. TI ULUC’s? =

158   cout << 123 << "< End\n">


===== PAGE 573 =====
572 ee 제3주

16:   return 0;
Iv: +

결과  Start >                    123< End
Start KRKKKKKKKKKKKKEEKEKEKKEK 1 23< End
붙석 7 - 9번 줄에서는 위의 예를 반복하였습니다. 줄 12-15에서도 이 기

복하였는데, 이번에는 14번 줄에서 채우는 문자가 BRS 설정되었고 이는
출력에 반영되었습니다.

설정 플래그(66 Flag)
jostream 객체는 플래그를 사용하여 객체의 상태를 추적하고 있습니다. 여러분은

이 플래그를 set 호출하여 설정할 수 있고 하나 이상의 미리 정의된 나열형

상수를 전달할 수 있습니다.
ge

새로운 .상태(61616) WHE 그 객체의 일부 록은 전부가 어떤 조건을 표시할 때 이를 상태
웅이 를 가지고 있다고 하는데 그 상태는 프로그램의 중간에 ta 수 있어야 합니다.

예를 들면, 여러분은 소수점 밑의 0들을 지니게 할 수도 있고 잘라 버릴 수도 있
습니다.(따라서 20.00이 20으로 절삭되지 않게 할 수 있습니다.) 0이 따라오게 하

71 setf(ios::showpoint)S 사용하면 됩니다.

나열형화된 상수가 1094600 클래스009)에 정의되어 있고 이는 충분한 명세와 함
Al 호출됩니다. 즉, 106: 플러그 이름의 BALA ios::showpoint7} 이 예입니다.
ios::showposS 사용하여 양수 앞에 +기호를 넣을 수 있습니다. 출력을 ios: lef,
ios::right, ios::intemalS-& 사용하여 정렬할 수 있습니다.

마지막으로 숫자의 기수를 106::060(십진법), 105::006(8진법), 106:06%(16진법)를 사용
하여 표현할 수 있습니다. 이 SATE 삼< 연산자 속에 연결될 수 있습니다.
[리스트 16.14]를 봅시다. 또한 [리스트 16.14]는 58\라는 조종자를 보여주는데 넓
이를 설정하면서 삽입 연산자에 연결될 수 있습니다.

[리스트 16.14] set) Ate

1: // [리스트 16.143 56[+7()를 사용
2: #include <iostream.h>

3: #include <iomanip.h>
4:


===== PAGE 574 =====
제16일 스트림 ce 573

5: int main()

6: <《

때    const int number = 185;

8:    cout << "The number is " << number << endl;

9°

AUS   cout << "The number is " << hex << number << endl;
11:

121   cout.setf(ios::showbase) ;

13%   cout << "The number is " << hex << number << endl;
14:

15%   cout << "The number is ";
16%   cout.width(10);
V7   cout << hex << number << endl;

18:

19:   cout << "The number is ";

20:   cout.width(10);

oe   cout.setfCios::left);

2ee   cout << hex << number << endl;
or

24:   cout << "The number is ";

Zo:   cout.width(10);

26:    cout.setf(ios::internal);     양쪽 La

are   cout << hex << number << endl;

28:

29%   cout << "The number is: " << setw(10) << hex << number << endl;
30:   return 0;

Sis 2

24}  The number is 185
The        is b9

number
The number is Oxb9
The number 15     Oxb9
The number is Oxb9
The number is Ox     b9
The number is Ox     b9
= ai  TH 줄에서 상수 int number7} 1852 초기화되었습니다. 8번 줄에 출력되었

습니다. 10번 줄에서 다시 출력되었는데 조종자 hex7} 연결되었고 이는 16
진수인 6906=11; 11*16+9=185)로 출력되었습니다.

12번 줄에서 showbase7} 설정되었습니다. 이는 모든 16    6진수 앞에 7} 붙도록  하
출력도    도 그렇게 되었습니다. 16번 줄에서 넓  넓이가 10으로 설정되고 Zo] 오른쪽
으로 밀렀습니다. 20번 줄에서 넓이가 다시 10으로 되었고 이번에는  정열이 왼쪽
으로 이루어졌는데 숫자는 다시 왼쪽으로 밀렸습니다.

|8


===== PAGE 575 =====
574 ee 제3주

25번 줄에서 다시 넓이가 10으로 되었고 이번에는 정열이 양쪽으로 이루어졌습니
다. 그래서 Ox: 왼쪽, WE 오른쪽으로 이루어졌습니다.

N

ele

막으로 29 줄에서 AA AA} setwOo] 넓이를 10으로 설정하였고 그대로
력되었습

니다.

2
oa
BR

\ 푸

스트림과 printf) 함수

대부분의 CHE 또 0의 표준 입출력 라이브러리 함수를 제공하는데 00000도 포
함이 됩니다. 비록 printf7} 000보다 사용하기는 편하지만 별로 바람직하진 않습

니다.
00000는 형의 안정성을 제공하진 않습니다. 따라서 정수형을 문자형으로 무심코
출력하    그 반대로 하라는 등의 Was 내릴 수 있습니다. = prntfoe

래스를 지원하지 않습니다. 따라서 여러분의 클래스 자료를 출력시키지 못합니다.
각 클래스의 ys 하나씩 20040에 주어져야 합니다.

한편 printf 규격화000080100)를 손쉽게 하는데 printf) 안에 맘대로 써넣을 수
있기 때문입니다. 00000는 나름대로의 사용법을 가지고 있기 때문에 아직 많이

애용됩니다. 이번 항에서는 70000를 살펴봅시다.
printfOS 사용하기 위해 헤더 파일로 STDIONS 포함시키는 것을 잊으면 안됩니

다. 간단한 형태로 print 첫 번째 매개 변수로 규격 문자열을 취하고 남은 매

개 변수에 일련의 값들을 취합니다.

규격 문자열은 쌍따옴표로 묶인 텍스트와 변환 상술자(600ㅁ60100 specifier)S 가집
니다. 변환 상술자는 반드시 퍼센트 기호(%)로 시작되어야 합니다. [표 16.1 일
반적인 변환 상술자가 있습니다

[표 16.1] 일반적인 변환 상술자

상술자               사용

825                    문자열

%d                    정수형

%|                       1009 정수형
%10                      long 정수형

%f                           float



===== PAGE 576 =====
제16일 스트림 ee 575

각 변환 상술자는 넓이를 나타내는 상술자와 정밀도(0009100)를 나타내는 상술
를 가집니다. 000형으로 표현되는 소수의 윈쪽은 총 길이를 나타나고 오른쪽은
float 나타나게 할 수 있는 정밀도를 표현합니다. 따라서 %50는 다섯 글자 넓
의 정수형을 나타내고, %15.9는 15길이 넓이의 80&형을  gee sy acdc a7
의 숫자는 정수형 부분의 길이입니다.

[리스트 16.15] printf) 출력하기

: #include <stdio.h>

: int main()

of

printf("%s","hello world\n") ;

1
2
3
4
D2
6    char *phrase = "Hello again!\n";
?    printf("%s\n",phrase) ;

3

9:    int x =5;

10: printf("%d\n",x);

112
12: char *phraseTwo = "Here's some values: uy
13: char *phraseThree = " and also these: mr

14: int y =7,2 5 35;

15: long longVar = 98456;

16: float floatVar = 8.8;

10%

18: printf("%s %d Xd %s Xd #f\n" ,phraseTwo,y,z,phraseThree, longVar,floatVar) ;
19%

20: char *phraseFour = "Formatted: "

21: printf("%s 250 %10d “10.5f\n",phraseFour,y,z,floatVar);

22: return 0;

25: 3

결과  hello world

Hello again!

5

Here's some values: 7 35 and also these: 98456 8.800000

Formatted:    7       35    8.800000
EBAY 431 중의 처음 20000 문장에서는 se 사용하였습니다. printfe = 단어
Of 상따옴표, 변환 상술자(여기서는 %9) 및 변환 상술자 안에 넣을 값이 있

습니다.


===== PAGE 577 =====
576 ee 제3주

Gz 문자열임을 나타내고 이 경우에 문자열의 RS “hello \000^입니다.

두 번째의 00000 문장은 첫 번째와 비슷한데 여기서는 문자열 대신 char 포인터
가 사용되었습니다.

10번 So] 세 번째의 20040에서는 정수 변환 상술자를 사용하였는데, 그 정수는
변수 xo] 들어 있는 go] 됩니다. 18번째 SS] 네 번째의 20000 문장은 다소 복
잡합니다. 여기에는 여섯 개의 값이 연결되어 있습니다. 각 변환 상술자가 공급되
고 변수가 제공되는데 ARS 분리됩니다.

마지막으로 21번째 줄에서 넓이와 정밀도를 나타내는 규격화된 상술자가 사용되
었습니다. 보다시피 조종자보다 사용이 편합니다.

앞서 말했듯이 20000의 약점은 형 검사가 없고 00040는 특정 클래스의 프랜드
나 멤버 함수로 선언될 수가 없다는 것입니다. 따라서 여러분이 다양한 멤버 자
료를 출력하려면 여러분은 70000를 명시적으로 작성해야 합니다.

파일의 입력과 줄력

10
다녀
ro
MS
br
10
로 0
Gi,
1
시
Hu
-ㅁ
때
x,
fru
(uu
rm
2;
mun
ac)
KI
if
fou,
rh
2,
tN
pa 일
1>
ay
Hu
ay
Jt

i

Hen] 단일한 WAS 사용합니다. 어떤 BPE 여러분은 F2
산자 및 관련된 함수나 조종자를 사용하면 됩니다. 파일을 열고

ifstreamz} ofstream2}] 객체를 사용하는데 이제부터 설명하려 합

Oo

Ht 2 tl {>
rlo (수

ofstream
니다. l= iostreaam 객체로부터 파생되었습니다. 파일에 AAA 여러분은 먼저
ofstream 객체를 만들고 여러분의 디스크의 특정 _파일과 연결지어야 합니다.
ofstream 객체를 사용하려면 먼저 여러분의 프로그램에 6068014를 포함시켜야 합
니다.

tstreamht iostreamhS 포함하므로 1660^68깨를 따로 포함할 필요가 없습니다.


===== PAGE 578 =====
제16일 스트림 ee 577

AWS 나타내는 상태

1050680 객체는 여러분의 입력과 출력 AVS 알리는 플래그를 가지고 있습니
불린 함수 eof), 60800, 1110, 80000를 사용하여 이 플래그를 먼저 검사할 수 있습
니다. 60[0는 1050600 객체가 EOFS 만나면 jc 반환합니다. 0800는 여러분이
TH) 않은 MS 시도하려면 참값을 반환하고, 5800가 참이거나 연산이
실패하면 1010 BPE 참을 반환합니다. Tee   로 good) 이 세 개의 함수가
거짓이면 참을 반환합니다.

문

> 때

ie

입줄력을 위한 파일 열기

myfile.cpp= ofstream 객체로 열기 위해 ofstream 객체의 인스턴스를 선언하고 매
개 변수로 파일 이름을 전달합니다. ㆍ 다인 3m

ofstream fout("myfile.cpp");

이 파일을 입력용으로 열기 위한 AS 같은 방식인데 단지 150600을 사용합니다.
ifstream fin("myfile.cpp");       다윈 입력

fout= cout, fin 00과 비슷합니다.
TL qc
ope 파일스트림 함수는 00560입니다. 여러분이 읽기용이나 쓰기용, 읽고 동시
쓰기용으로 열어놓은 파일은 입출력을 마친 뒤 00600로 닫아야 합니다. 이렇
~ 『 파일이 깨지거나 디스크에 저장한 파일이 없어지지 않습니다.

트림 객체가 일단 파일과 연결되면 다른 스트림 객체처럼 쓰일 수 있습니다

[리스 스트 16.16]을 봅시다.

nak:

[리스트 16.16] 읽기와 쓰기응으로 파일을 열기

1: #include <fstream.h>

2: int main()

3: £

4:    char fileName[80];

5    char buffer[255]; // 입력용
6:    cout << "File name: ";

7    cin >> fileName;

8

9:    ofstream fout(fileName); // M2

10:   fout << "This line written directly to the file...\n";
We   cout << "Enter text for the file: ";
12:   Cin.ignore(1,"\n'); // 파일명 뒤의 개행 문자를 없앰

13: cin.getline(buffer,255); // 사용자 입력받음

드



===== PAGE 579 =====
578 ee 제3주

14:   fout << buffer << "\n"; // 파일에 씀

15:  fout.closeQ); // 파일을 닫고 다시 열기를 기다림
165

17: ifstream fin(fileName); // 읽기 위해 다시 S
18°   cout << "Here's the contents of the file:\n";

19:   char ch;
20:   while (fin.get(ch))

212      cout << ch;

22:

23:   cout << "\n***xEnd of file contents.***\n";
24:

25:   fin.close();
26:   return 0;
20) 》

결과  File name: test1
Enter text for the file: This text is written to the file!
Here's the contents of the file:
This Line written directly to the file...
This text is written to the file!

*kkxEnd of file contents.***

분석 4번 줄에서 비퍼가 파일 이름을 저장하기 위해 마련되었고 5번 줄에서 사
용자의 VAS 위해 버퍼가 만들어졌습니다. 사용자는 6번 줄에서 파일 이
름을 입력하고 이는 fileName 버퍼에 저장됩니다. 9번 줄에서 ofstream 객체 [04이
만들어지는  는데 이는 새로운 파일명과 연결이 됩니다. 이는 파일을 열고 만일 파일
이 존재하면 그 내용은 지워집니다.
10번 줄에서 텍스트의 문자열이 직접 파일에 쓰여집니다. IA 줄에서 사용자는
입력을 합니다. 사용자가 입력에서 파일명을 입력할 때 같이 입력된 개행 문자는
12번 줄에서 없어지고 따라서 파일명은 13번 줄에서 600@에 저장됩니다. 이 입
력은 14번 줄에서 개행 문자와 함께 입력이 되고 파일은 15번 줄에서 닫힙니다.

ITA 줄에서 파일이 다시 열리고 이번에는 읽기 전용으로 열리는데, 20과 21번
Zo) 한번에 한 문자씩 Yala.

파일 열기에서 ofstream 객체의 기본 작동을 변화시키는 법

파일을 열 때의 기본 작동은, 만일 파일이 없어 새로 만들고 있으면 안의 내용을
지우는 것입니다. 이러한 기본 ASS 원하지 않는다면 여러분은 여러분의



===== PAGE 580 =====
제16일 스트림 ee 579

ofstream 객체의 생성자에 명시적으로 두 번째의 인수를 줄 수 있습니다. 다음이
것들입니다.
Mi ics:opp - 존재하는 파일 끝에서부터 내용을 써나갑니다. add ol Lx)
를 10506 ㆍ 파일의 끝에 AAU, 그러나 자료의 어느 RYE 쓸 수가 있습니다.
Bl ios:ttrunc -  기본값입니다. 존재하는 파일이 있으면 내용을 자릅니다.
 ios::nocreate - 파일이 없으면 열기 Sato) 실패합니다

I ios::noreplace - 이미 파일이 존재하면 열기 동작이 실패합니다.

app 800600의 약자이고, ate at 600의 약자이며, trunct truncate2} 약자입니다.
[리스트 16.17]은 [리스트 16.162] 파일을 다시 열어 그 끝에 YRS 덧붙이는 것
입니다.

[리스트 16.17] 파일 끝에 덧붙이기

1: #include <fstream.h>

2: int mainQ) // 오류시 1 반환

3: ¢      .

4:    char fileName[80];

Bi    char buffer(l255];

6:    cout << "Please re-enter the file name: ";
이    cin >> fileName;

8

9:    ifstream fin(fileName) ;

10:   11 (1110)

115   {

125      cout << "Current file contents:\n";

13:      char ch;

14:      while (fin.get(ch))

15:        cout << ch;

16:      cout << "\n***End of file contents.***\n";
a Ae   J

18:   fin.close();

ADs

20%   cout << "\nOpening " << fileName <<" in append mode...\n";
212

ee:   ofstream fout(fileName,ios::app);

25:   if (!fout)

24:   {

25%      cout << "Unable to open " << fileName << " for appending.\n";
26:     return(1);

27%   }

28:


===== PAGE 581 =====
580 ce

제3주

29:
30:
31:
Lys
53:
345
55:
562
S(:
38:
39:
40:
41:
42:
43:
44:
45:
46:
47:
48:

cout << "\nEnter text for the file: ";
cin.ignore(1,'\n');
cin.getline(buffer,255);
fout << buffer << "\n";
fout.close();
fin.open(fileName); // 존재하는 fin 객체에 할당
if (!fin)
{
cout << "Unable to open " << fileName <<" for reading.\n";
return(1);
}
cout << "\nHere's the contents of the file:\n";
char ch;
while (fin.get(ch))
cout << ch;
cout << "\n***End of file contents.***\n";
fin.close();
return 0;
0

결과

(rag
2

 cet

Please re-enter the file name: test1
Current file contents:

This Line written directly to the file...
This text is written to the file!

*kkEnd of file contents.***

Opening test1 in append mode...

Enter text for the file: More text for the file!
Here's the contents of the file:

This Line written directly to the file...

This text is written to the file!

More text for the file!

*kxEnd of file contents.***

사용자는 다시 파일명을 넣습니다. 이번에는 9번 줄에서 입력 파일 스트림
객체가 만들어졌습니다. 10번 줄에서 열기가 실험되고 이미 파일이 존재하
내용이 12 - 16번 줄에서 출력이 됩니다. 1(87)는 1000.80000)의 동의어입


===== PAGE 582 =====
제16일 스트림 ee 581

입력 파일이 닫히고 같은 파일이 다시 열립니다. 이번에는 덧붙임 방식으로 22번
줄에서 열립니다. 이번 열기에서도 파일이 제대로 열렸는지 검사됩니다. 1(!10040
는 100401010)과 같은 검사입니다. 사용자는 텍스트를 입력하고 파일이 다시 33
번 줄에서 닫힙니다.

마지막으로 [리스트 16.16|에서와 같이 파일이 읽기 전용으로 열립니다. 하지만
이번에는 fine] 다시 선언될 필요가 없습니다. 같은 파일명이 다시 할당되었습니
다. 다시 368 줄에서 파일이 제대로 열렸는지 검사가 되고 아무 이상이 없다면
파일 내용이 출력된 후 파일이 닫힙니다.

DO     파일을 열 때마다 정확히 열렸는지 확인합시다.

00     존재학는 }60^68/과 ofstream 객체를 다시 사용합시다.
00      다 사용한 tstream 객체는 닫아버립시다.
DON'T  0/이나 cout 닫거나 재할당하지 opsy cy,

이진 파일과 텍스트 파일(8108 versus Text File)

특정 운영체제, 예를 들어 DOS 같은 경우에는 이진 파일과 텍스트 ae 구별
합니다. 이름에서 알 수 있듯이 텍스트 파일은 모든 것을 텍스트로 저장합니다

즉, 54.325는 숫자형의 BAAS, '4', , '3', '2', 5” )로 저장합니다. 이는 비효
#40121 하지만 DOS 녀래가 간단한 프로그램으로 Me) 수 있다는 장점
이 있습니다.

시스템이 텍스트와 이진 파일간의 구별을 쉽게 하기 위해 C++& ios: :00080라는
플래그를 le 제공합니다. 많은 시스템에서는 이 플래그가 무시되는데, 이는 모든 자
료가 이진 형태로 저장이 되기 때문입니다. 심지어 어떤 시스템에서는 109::61080
라는 플래그는 틀린 것이고 컴파일조차 안됩니다.

이진 파일은 정수형 및 문자열뿐만 아니라 전체 자료 구조도 저장합니다. 모
자료들을 150680의 write) 메쏘드를 사용하여 한번에 입력할 수 있습니다.

write)=S 사용하면 6800를 사용하여 다시 자료를 읽어들일 수 있습니다. A 함수
는 문자에 대한 포인터를 원하는데, 여러분의 클래스의 주소를 문자 포인터로 형
변환하여 사용할 수 있습니다.

pH

[on


===== PAGE 583 =====
582 ee

제3주

각 함수의 두 번째 인수는
할 수 있습니다 쓰여지는 것은

히는

쓰여지는 문자의 크기를 넣어야 하는데 9200[0를 사용
메쏘드가 아니라 자료임을 잊지 Bal. 또한 읽

것도 자료입니다. [리스트 16.18]을 보기로 합시다.

[리스트 16.18] 클래스를 파일에 쓰기

1
2
3
4
98
6
df
8

9:

10:
11:
128
13:
14:
15%
16:
173
18:
19:
20:
218:
22:
25°
24:
25:
26%
ot
28:
29.:
30:
318
32:
5352
34:
358
36:
Si:
38:
39:

: #include <fstream.h>

: class Animal
2 4

public:

Animal (int weight, long days) :itsWeight (weight) , itsNumberDaysAl ive(days) {}

“Animal () {}

int GetWeight()const { return itsWeight; }
void SetWeight(int weight) { itsWeight = weight; }

Long GetDaysAlive()const 1 return itsNumberDaysALlive; }
void SetDaysAlive(long days) ¢ itsNumberDaysALlive = days; +

private:

int itsWeight;

Long itsNumberDaysAlive;
3;

int main

{
char fileNameLl801];
char buffer[255];

cout << "Please enter the file name: ";

cin >> fileName;

ofstream fout(fileName,ios::binary);

if (!fout)

{
cout << "Unable to open " << fileName <<" for writing.\n";
return(1);

Animal Bear (50,100);
fout.write((char*) &Bear,sizeof Bear);
fout.close();

ifstream fin(fileName,ios::binary);


===== PAGE 584 =====
제16일 스트림 ce 583

40:   at Cl find

41:   {

42:      cout << "Unable to open " << fileName << " for reading.\n";
43:     return(1) ;

44:   }

45:                        .

46:   Animal BearTwo(1,1);

47:

48:   cout << "BearTwo weight: " << BearTwo.GetWeight() << endl;
49:   cout << "BearTwo days: " << BearTwo.GetDaysAlive() << endl;
502

Die   fin.read((char*) &BearTwo, sizeof BearTwo);

a2:

53:   cout << "BearTwo weight: " << BearTwo.GetWeight() << endl;
54:   cout << "BearTwo days: " << BearTwo.GetDaysAlive() << endl;
5D:   fin.close();

56:   return 0;

are }

겔과  Please enter the file name: Animals
BearTwo weight: 1
BearTwo days: 1
BearTwo weight: 50
BearTwo days: 100

분석  3-18번 줄에서 간단한 Animal 클래스가 선언되었습니다. 22-32번 줄에서 파
일이 만들어지고 이진 양식으로 출력되기 위해 열립니다. 50이라는 무게를
가지고 100일의 나이를 가진 동물이 34번 줄에서 만들어지고 35번 줄에서 그 자
료들이 파일에 써집니다.
37번 줄에서 파일이 닫히고 39번 줄에서 이진 양식의 읽기 형태로 다시 열립니
다. 46번 줄에서 두 번째의 동물이 생기는데 무게는 1이고 나이는 하루입니다. 51
번 줄에서 파일로부터 자료가 새로운 동물 객체에게 daa 옮겨지는데 기존의
자료를 대체하고 새로운 자료가 들어가 차지합니다.

명령어줄 프로세싱(30101013110-Ｌㄴ1116 라보
DOSU UNIX 같은 많은 운영체제에^                   프로그램의 매개
변수를 전달할 수 있게 합니다. 이러한 것을 니케  줄 te 부르는데 빈칸에

의해 구분됩니다.

고
tI
if
a
rs
[원
고


===== PAGE 585 =====
584 ㅇㅇ 제주

SomeProgram Param1 Param2 Param3

이 매개 변수들은 0000으로 직접 전달됩니다. 그런데 mange 두 개의 매개 변
수를 가집니다.

첫 번째는 명령어줄에서 gate @ ate Age 가지는  정수형 계산기입니

다. 프로그램 그 자체도 하나로 계산되므로 모든 프로그램은 적어도 하나의 매개
Wee 가집니다. 위의 예제 프로그램은 4개의 매개 변수를 가집니다.(프로그램
명과 나머지 3개의 매개 변수)

00009 gist 번째의 매개 변수는 포인터 문자열의 배열입니다. 배열명은
배열의 첫 번째 원소의 상수형 포인터이므로 여러분은 이 인수를 문자형 포인터
의 포인터로 혹은 ~  배열의 포인터로 혹은 문자형 배열의 배열로 선언할 수
있습니다.

전형적으로는 첫 번째 CFE argc(argument 00400로 이름지워지는데 여러분 맘대
로 이름을 바꿔도 됩니다. 두 번째 1FYS argv(argument vector)= 잘 쓰는데 다
른 이름으로 바꿔도 상관없습니다.

&080에 여러분이 원하는 만큼의 매개 변수를 받았는지 검사한 후 08\에 접근하는
것이 일반적인 방법 중 하나입니다. argv} e 프로그램명이고, 08111은 프로그램
에 대한 첫 번째 매개 변수인데 보통 문자열입니다. 여러분의 프로그램이 인수로
두 개의 SAS 가지면 이 SASL 문자열로 전달되는데 나중에 필요에 따라 숫
자형으로 바꿀 필요가 있습니다. 19일째 어떻게 표준 라이브러리를 사용하여 바
꾸는지 보여줄 것입니다. [리스트 16.19|는 명령어줄 인수 전달 방법의 예를 보여
줍니다.

[리스트 16.19] 명령어줄 인수

1: #include <iostream.h>

2: int main(int argc, char **argv)

3:

4s    cout << "Received " << argc << " arguments...\n";
DE    for Cint i=0; i<argc; i++)

6     cout << “argument " << i <<": " << argvLil << endl;
7     return 0;

8: +

결과  TestProgram Teach Yourself C++ In 21 Days
Received 7 arguments...


===== PAGE 586 =====
제10일 스트림 ee 585

argument 0: TestProgram.exe
argument 1: Teach

argument 2: Yourself
argument 3: C++

argument 4: In

argument 5: 21

argument 6: Days

(aa

가지는 정수형과 명령어줄의 각 단어의 포인터를 가지

다. 각자의 프로그래밍 취향에 따라 쓰면 됩니다. 각 배열의 변위는 각각의 문

열을 접근하기 위해 쓰입니다.

4번 줄에서 argc 명령어줄의 인수 ASS 출력하기 위해 사용되었습니다.
그램 명까지 하여 7이 됩니다.

A main 두 개의 매개 WES 가집니다. 480라는 명령어줄의 인수 7

프로

5, 6번 줄에서 각 명령어줄 인수들이 출력됩니다. 문자열의 배열을 각각 찾아갈

때 cout] 널로 끝나는 문자열이 전달됩니다.

명령어줄 인수의 좀더 일반적인 사용법은 [리스트 16.18|의 파일명을 명령어

서 받아들이는 방법으로 바꾸는 것입니다. 이 예제에서는 바뀌지 않은 클래
언은 포함하지 않았습니다.

[리스트 16.20] 명령어줄 사응법

줄어

=

A ㅅ
= at

1: #include <fstream.h>

2: int main(int argc, char *argvLl])

S: <¢

4:    if (argc != 2)

5    a

6:       cout << "Usage: " << argv[0] << " <filename>" << endl;
ts      return(1);

8:    +

o:

108   ofstream fout(argv[1],ios::binary);

Wale   if (!fout)

121   {

AS:      cout << "Unable to open " << argv[1] <<" for writing.\n";
14:     return(1);

er   +

16%

17:   Animal Bear(50,100) ;


===== PAGE 587 =====
506 ec AB

18   fout.write((char*) &Bear,sizeof Bear);

19s

20:   fout.close();

218

22:   ifstream fin(argvL[11],ios::binary);

23:   Tf GC! Fin)

24:   £

258      cout << "Unable to open " << 89614 << " for reading.\n";
26:     return(1);

er:   }

28:

29s   Animal BearTwo(1,1);

50:

31:   cout << "BearTwo weight: " << BearTwo.GetWeight() << endl;
522   cout << "BearTwo days: " << BearTwo.GetDaysAlive( << endl;
55:

54:   fin.read((char*) &BearTwo, sizeof BearTwo);

55:

36:   cout << "BearTwo weight: " << BearTwo.GetWeight@ << endl;
Sr?   cout << "BearTwo days: " << BearTwo.GetDaysAlive() << endl;
58:   finwcloset):;

39:   return 0;

40: }

24 Dh  BearTwo weight: 1
BearTwo days: 1
BearTwo weight: 50
BearTwo days: 100

Animal9] 클래스 선언은 [리스트 16.18|과 Soh 여기서는 빼버렸습니다.
그런데 이번에는 사용자에게 파일명을 입력하라고 요청하는 대신에 명령어
중 입력 YAS 사용하였습니다. 2번 줄에서 maine] 두 개의 매개 변수를 가지
도록 선언되었는데 각각 인수의 개수를 가지는 변수와 명령어줄의 각 인수 문자
열의 포인터를 배열 윈소로 갖는 포인터입니다.

그르

(aa

4 - 8번 줄에서 프로그램은 전
사용자가 HUBS 전달하지 않

를 확인합니다.(2개입니다.) 만일
장이 다음과 깥이 나옵니다.
Usage TestProgram <filename>
그리고 프로그램이 끝납니다. 프로그램에 내장되어 있는 파일명보다 008이을 사
용하는 것이 파일명을 자유로이 갖게 하고 또 위의 사용법 문장을 내보낼 수 있

어 좋습니다.


===== PAGE 588 =====
제16일 스트림 ee 587

lod 줄에서 전달된 파일을 이진 파일로 엽니다. 파일명을 지역 임시 버퍼에 저
장해야 할 이유가 없습니다. 481111을 접근함으로써 해결됩니다.

이 기법이 22번 줄에서 사용되었는데 같은 파일이 입력용으로 다시 열렸고, 13과
25번 줄에서는 파일 열기가 실패했을 때 오류 문장을 출력하면서 다시 사용됩니다.

오늘은 스트림과 전역 객체 004, 00을 배웠습니다. 154680과 ostream 객 체의 목적
은 여러 구동 장치에 쓸 때와 입출력에 버퍼 할 때 캡슬화를 위해 사용됩니다.
각 프로그램에 의해 만들어지는 4개의 표준 스트  객체가 있습니다. 004, cin,
cert, clog7} 그것들인데 각각은 많은 운영체제에 의해 재지정될 수 있습니다.
160680 객체인 cine YAS 위해 사용되는데 일반적인 사용법은 추출  연산자(>>)
를 재생하는 AMC. ostream 객체 004는 SYS 위해 쓰이는데 흔한 사용법은
삽입 연산자(<<)를 재생하여 쓰는 것입니다.

각 객체는 몇 개의 멤버 함수들을 가지고 있습니다. get(), 040 둥이 그것입니다.
각 메쏘드의 일반적인 형태는 스트림 객체의 참조자를 반환하므로 각 연산자와
함수를 연결하기가 쉽습니다.

스트림 Male 나    oe 사용하여 리피  제주)  oe 이 조종자들은 규격

본

일 입출력은 60600 클래스를 사용하여  is  수 있는데 60600은 스트림 클래
스로부터 파생된 것입니다. 정상적인 삽입 및 추출 연산자를 지원하는 것 외에,
이 객체들은 대용량의 이진 객체를 정열하고 검색하기 위해 0800, writeQS 가집

니다.

Q&A

Q 삽입 및 추출 연산자를 언제 쓸 것인가를 어떻게 압니까? 또 stream 클래스의 각 멤
of 함수를 언제 쓸 것인지 어떻게 압니까?
A 일반적으로 Aq 및 추출 연산자를 사용하는 것은 쉽고 또한 선호됩니다. 그런데
비정상적인 상황에서는 이 연산자들이 제역할을 못할 때가 있습니다.(단어 문자열
못 읽어들임) 이런 땐 다른 함수를 syd.


===== PAGE 589 =====
388 ce 제3주

Q cerrZ clog2| 차이점은 무엇입니까?

A 000은 버퍼화되지 않습니다. 000에 쓰이는 것은 + 출력됩니다. 이것은 오류들이
화면에 나타나게 할 때 좋습니다. 그러나 이를
과부하가 걸립니다. 008는 출력에 버퍼를 제공하므로   더욱 효율적입니다.

Q printf()7} 잘 동작하는데 왜 스트림이 필요합니까?

스 20000는 C++9] 강형 시스템을 충분히 지원하지 못합니다. 따라서 사용자가 정의한
클래스를 지원 못합니다.

Q 언제 putback()S 사용합니까?

A 읽기 연산자가 문자가 유효한지 아닌지를 결정하는데 쓰이기도 하지만 다른 읽

연산자는 BAS 버퍼에 넣기도 합니다. 파일을 파싱(08008)할 때 많이 ered
예를 들면 0++의 컴파일러 프로그램은 2000060을 S 확률이 높습니다.

Q 1910016()는 언제 쓰입니까?

A 보통 gett) 다음에 쓰입니다. 800는 종료 문자열을 YA] 남기므로 get 다음에
ignore(1, "\n’)°] 자주 쓰입니다. 이것도 파싱할 때 많이 쓰입니다.

| 나의 동료가 C++ 프로그램에서 010()를 자주 쓰는데 그래도 좋습니까?
그렇습니다. 편리함이 있긴 있습니다. 단 형의 안정성은 보장 못합니다.

연구

°

ㅣ 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가
를 확인해보는 퀴즈들과, 배운 것을 시험해         연습 문제들로 구성되어
있습니다. 부록 Do] 있는 답을 보기 전에 각 물음에 대답할 수 있도록 노력하고,

장으로 넘어가기 전에 FS 충분히 이해하도록 합시다.

그
1
의

rir

퀴즈

1, 삽입 연산자란 무엇            을 합니까?

2 추출 연산자란 무엇이며 어떤 역할을 합니까?

3 cin.get()2} 세 가지형은 무엇이고 각각의 차이점을 말해봅시다.

4 cin.read()2t cin.getline2| 차이점은 무엇입니까?
$ㆍ 삽입 연산자를 사용하여 long 정수형을 출력할 때 기본 폭은 얼마입니까?
6 삽입 연산자의 반환값은?


===== PAGE 590 =====
제16일 스트림 ㅎㅎ 589

7 ofstream 객체의 생성자는 어떤 매개 HS 취합니까?

8. ios::ate UTE FAS 합니까?

연습 문제

1. 4개의 EF iostream 객체(00, cout, cerr, 이09)에 출력하는 프로그램을 작성하십

시오.

2% 사용자로부터 성명을 입력받고 화면에 출력하는 프로그램을 작성하십시오.

3.

4.

ae: |                   | — |
[리스트 16.98 같은 일을 하는 프로그램으로 바꾸어 작성하되 putback()Lt
ignore()S 사용하지 BAIct.
HAIRS 매개 변수로 받아들이고 읽기 전용으로

피                     =|
파일의 모든 문자를 읽고 나서 알파벳, 숫자, 구두점만을 화면에 출력한 뒤 파일을 닫는


===== PAGE 591 =====
ce

ce



===== PAGE 592 =====
ff                              =

ANIA



===== PAGE 593 =====
592 ee 제3주

서문
지금까지 여러분은 CH 프로그램을 만들었습
해 해석되어 여러분의 프로그램이 됩니다. 그런데 컴파일러가 295171 전 전처
리계라는 것이 먼저 실행합니다. 이는 조건부 컴파일이라는 기회를 부여합니다.
오늘 여러분이 배울 내용은 다음과 같습니다.
를 조건부 컴파일이란 무엇이며 어떻게 하는가?
를 전처리게에서 사용하는 매크로는 어떻게 작성하는가《
를 버그를 잡기 위해 어떻게 전처리게를 쓰는가

니다. 이 프로그램은 컴파일러에 의

접저리계와 컴파일러(060「0066550『 and Compiler)

매번 컴파일러를 돌릴 때마다 전처리계가 먼저 수행됩니다. 전처리계는 전처리계
명령어를 먼저 찾습니다. pall 명령어는 샵 7 SHH 시작합니다. 이 명령어
의 역할은 원시 코드를 텍스트로 바꾸는 역할을 합니다. 결과는 새로운 원시 코
드가 되는데 여러분은 보지를 못하지만 컴파일러로 하여금 여러분이 볼 수 있는
형태로 저장시킬 수 있는 명령은 내릴 수 있습니다.

컴파일러는 여러분의 원시 코드를 읽지는 않습니다. 컴파일러는 전처리계의 출력
BO 읽고 그 출력물을 컴파일합니다. 여러분은 이미 #00006 지시자(076006)의
AMS 이미 살펴보았습니다. 이는 전처리계로 하여금 해당하는 파일을 찾아 원
시 코드의 그 위치에 넣도록 합니다. 마치 여러분이 원시 코드에 입력하여 넣은
처럼 하고 나중에 컴파일러가 컴파일할 때 포함된 파일이 그 자리에 있도록 합

중간 '애티0800900 『0100)의 보기

모든 _컴파일러는 여러분     통합 개발 SAUDE : integrated development
environment) 상태로 있게 ay 3 혹은 라인 명령어  ils    환경에 있게 할 수 있으
며, 각각 컴파일러에게 중간 파일을 저장하도록 명령을 내릴 수 있습니다. 이 중
간 파일을 보고 싶으면 여러분의 컴파일러 안내서를 보     고 명령을 내려봅시다.


===== PAGE 594 =====
세17일 전처리계 ee 593

#define 지시자 사응하기

#define 지시자는 문자열 치환 명령

thlo

내립니다.
#define BIG 512

전처리계로 하여금 810이라는 문자열만 나오면 5122 바꾸게 합니다. ES BIG
는 여러분의 원시 코드에서 512로 we ESS 문자열, 상수, 혹은 사용 가능
한 다른 글자들의 집합이 있는 RA 사용될 수 있는 문자열입니다.) 여러분이
로그램에서 다음과 같이 썼다면

#defind BIG 512;
int myArrayL[BIG];

전처리계에 의해 형성된 중간 파일에는 다음과 같이 써집니다.
int myArray[512];

여기서 #Hdefine 지시자 문장이 없어졌음을 주의합시다. 전처리계 문장은 모두 없

어집니다. 마지막 코드에서는 전혀 나타나지 않습니다.

lq

#define 지시자를 사용한 상수 정의
66806 지시자를 쓰는 한가지 이유는 ASE 치환화기 위해서입니다. 사실 이는
별로 좋은 생각이 아닙니다. #06006 지시자는 단지 치환만 하지 BS 검사하지
않습니다. 상수 AYA) 말하였지만 define 지시자를 사용하는 것보다 const 예약
OR ee SOF FROETTSOO

어를 사용하는 것이 좋은 이유가 많습니다.

겸사응으로 #define 지시자 사응
#define 지시자를 사용하는 두 번째는 단지 어떤 특정의 문자열이 정의되었다는
것을 선언하기 위함입니다.

de fine (816)

이라고 하여놓고 나중에 BIG] 정의되었는지 아닌지에 따라 프로그램을 달리 나
가게 할 수 있습니다. 이때 각각 쓰는 전처리계 명령어가 #00라와 #0008입니다.
양쪽 다 모두 블록이 끝나기 전에(마감 중괄호를 만나기 전에) dendifay 의해 닫
혀야 합니다.

Hifdeft= 검사하고자 호
여러분은 다음과 같이

의되어 있으면 참이 됩니다. 따라서



===== PAGE 595 =====
594 ee 제3주

#ifdef DEBUG
cout << "Debug defined";
#endif

전처리계가 tildes 만나면 미리 만들어 놓은 테이블을 se] 06809가 있는지
살펴봅니다. 있다면 Be] 되고 다음의 #660나 *0008를 만나기 전에 있는 모든 문
A 중간 파일에 Sc}. 거짓으로 판명되면 #ifdef DEBUGS} 8600 사이에 있는
모든 문장들이 애초의 원시 코드에 없었던 것처럼 됩니다.

8006 40 의 elas] 역입니다. #ifndef= 여태껏 검사하고자 하는 문자열이
정의되어 있지 않아야 참이 됩니다.

#else 전처리계 지시자
충분히 생각할 수 있겠지만 Hilder 혹은 sindets} 6000 사이에 #060가 을 수 있
습니다. [리스트 17.11을 봅시다.

[리스트 17.1] #define 지시자 사응

1: #define DemoVersoin
2: #define DOS VERSION 5
3: #include <iostream.h>
4:

D5

6: int mainQ)

f: €

8:

9: cout << "Checking on the definitions of DemoVersion, DOS VERSION and
WINDOWS VERSION...\n";

10:

11: #ifdef DemoVersion

12:   cout << "DemoVersion defined.\n";

13: #else

14:   cout << "DemoVersion not defined.\n";
15: #endif

16:

17: #ifndef DOS VERSION

18:   cout << "DOS VERSION not defined!\n";

19: #else

20:   cout << "DOS VERSION defined as: " << DOS VERSION << endl;
21: #endif

22:

23: #ifdef WINDOWS VERSION

24:   cout << "WINDOWS VERSION defined! \n";


===== PAGE 596 =====
제17일 전저리계 ee 595

25: #else

26:   cout << "WINDOWS VERSION was not defined.\n";
27: #endif

20:

295   cout << "Done.\n";

30:   return 0;

30:}

겔과 Checking on the definitions of DemoVersion, DOS VERSION and
WINDOWS VERSION...

DemoVersion defined

DOS VERSION defined as: 5
WINDOWS VERSION was not defined.
Done.

(rag

섹  1,  2번 줄에서  10600\659100과 DOS_VERSION°S] 정의되었는데
DOS_VERSION?- 문자열 5로 정의되었습니다. 11번 줄에서 DemoVersion]
검사되었는데 DemoVersion®] 정의되어 있으므로 참이 되고 12번 줄이 출력됩니다.

17번 줄에서 DOS_VERSION©] 정의 안되어 있는지 검사합니다. DOS_VERSION-2-
정의가 되어 있으므로, 이 부분은 거짓이 되고 실행문은 20번 줄로 뛰어갑니다.
여기서 문자열 5 DOS_VERSIONS.2 치환되고 이는 컴파일러에 의해 볼 수 있
습니다.

cout << "DOS VERSION defined as: " << 5 << endl;

처음의 DOS_VERSION<- 치환이 안되었는데 왜냐하면 이는 쌍따옴표로 둘러싸였
기 때문입니다. 두 번째의 DOS_VERSION 치환이 되어 마치 여러분이 5를 입력
한 것처럼 컴파일러가 인식하게 됩니다.

마지막으로 2H 줄에서 프로그램은 WINDOWS_VERSIONS Ate} I] ch.
WINDOWS_ VERSIONS 정의하지 않았고 따라서 26번 줄이 출력됩니다.

포함(|0어45100) 및 포함 AAI Inclusion Guard)

여러분은 프로젝트를 할 때 여러 개의 다른 파일들로 만드는 경우가 많습니다.
때로는 여러 개의 각각의 클래스가 그 자신의 클래스를 선언한 헤더 파일(4008)
및 클래스 메쏘드를 설정한 원시 코드가 담긴 CPPS 각각 가진 디렉토리
들을 결합할 것입니다.


===== PAGE 597 =====
596 ㅇㅇ 제3주

여러분의 main) 함수는 .CPP 파일 안에 있고 모든 CPP 파일은 OB) 파일로 A
파일 되고 다음에는 링커에 의해 하나의 프로그램으로 됩니다.

여러분의 프로그램은 다른 많은 클래스를 사용하기 때문에 많은 헤더 파일들이
각각의 파일에 포함되어야 합니다. 한편 헤더 파일 각각도 다른 헤더 파일을 포
함할 때가 많습니다. 예를 들어, 파생된 클래스 선언을 가진 헤더 파일은 자신의
베이스 클래스를 가진 파일을 포함해야 합니다.

를 들면 Animalo] ANIMAL.HPPo] 있다고 합시다. 200.80#에 있는 Dog 클래
= Animal 클래스로부터 파생되는데 ㅅ04441.10#를 포함해야 합니다. 아니면
Animal 222) 파생될 수가 없습니다. Cat 헤더 파일은 같은 이유로 ANIMAL.HPP
를 포함해야 합니다.

만일, 여러분이 Catz} DogS 같이 사용하는 ARES 만든다면 여러분
ci car 이 ace li cra

ANIMALHPPS 두 번 포함하게 되는 위험성이 있습니다. 이는 컴파일 오류를

생시키므로 클래스를(40008) 두 번 선언하는 것은 비록 선언이 같다고 하더라

좋지 않습니다. 이 문제는 포함되었는지를 검사하는 문장을 다음과 같이 작성

여 해결할 수 있습니다.

#ifndef ANIMAL HPP

#define ANIMAL_HPP

. . // 모든 파일을 여기에 넣음
#6007+

| &

El at ro

이렇게 하면 여러분이 ANIMAL_HPPS 정의하지 않았다면 지금 정의하게 됩니다.
#defineS} #endif 사이에 원하는 전체 파일을 넣습니다.

여러분의 프로그램이 처음 이 부분을 포함하였으면 전처리계는 첫째 줄을 읽고
참으로 판명합니다. 즉, 여러분이 아직 ANIMAL_HPPS 정의하지 않았다는 뜻입
니다. 그러면 계속 진행하여 \00006 안의 전체 BUS 정의하고 포함합니다.

여러분 프로그램이 두 번째로 이 HRS 만나게 된다면 전처리계는 첫째 줄을 거
짓으로 판명 내립니다. ANIMAL HPPS 정의되어 있습니다. 이런 경우 다음의

대부분 정의된 파일 이름을 대문자로 쓰고 점()을 밑줄 문자(.)로 바꾸어 쓰지만
정의된 파일(4404441.800)의 실제 이릅은 별로 중요하지 않습니다. 단지 개념상



===== PAGE 598 =====
제17일 전처리계 ee 597

al
att
2
tt
ww
oz
poe
a
rir
>코
Tle
is
1:3
2
2

습니다. 때때로 여러분의 디버깅 시간을 줄여 줌

라인 명령어 환경에서 정의하는 방법
대부분의 C++ 컴파일러는 여러분에게 #06806의 값을 라인 명령어 환경에서 정의
|             하게 하거나 혹은 통합 개발 환경에서 혹은 양쪽에서 사용할 수 있게 해줍니다.
따라서 [리스트 17.1의 1-2번 SS 빼고 명령어 줄에서  DemoVersion,
|                BetaTestBersion 등을 넣을 수 있습니다.

특정의 디버깅 SES #ifdef DEBUGS} #endif 사이에 넣을 수 차  이렇게
하면 최종 버전에서는 여러분의 디버깅 코드가 컴파일시 원시 코드에서 쉽게 없

어지게 할 수 있습니다.

#undef 사용하기
AANA
‘58 이름을 정의한 뒤 취소하고 싶으면 [리스트 7a  | hoaets) 1894404

[리스트 17.2] #undef 사응법

1: #define DemoVersion

2: #define DOS VERSION 5

3: #include <iostreams.h>

4:

Dt

6: int main()

ce 그

8:

9: cout << "Checking on the definitions of DemoVersion, DOS VERSION and

WINDOWS VERSION...\n";

10:

11: #ifdef DemoVersion

12s   cout << "DemoVersion defined.\n";

13: #else

14:   cout << "DemoVersion not defined.\n";
15: #endif

16:

17: #ifndef DOS VERSION
18:   cout << "DOS VERSION not defined!\n";


===== PAGE 599 =====
598 ee 제3주

19:
20:
21:
225
23:
24:
25%
26:
27:
28:
29:
50:
31:
32:
55%
34:
353
36:
Ste
38:
59:
40:
41:
42:
45%
44:
45:
46:
CS
48:
49:
50:
S12

#else
cout << "DOS VERSION defined as: " << DOS VERSION << endl;
#endif

#ifdef WINDOWS VERSION

cout << "WINDOWS VERSION defined! \n";
#else

cout << "WINDOWS VERSION was not defined.\n";
#endif

#undef DOS VERSION

#ifdef DemoVersion

cout << "DemoVersion defined.\n";
#else

cout << "DemoVersion not defined.\n";
#endif

#ifndef DOS VERSION

cout << "DOS VERSION not defined!\n";
#else

cout << "DOS VERSION defined as: " << DOS VERSION << endl;
#endif

#ifdef WINDOWS VERSION

cout << "WINDOWS VERSION defined! \n";
#else

cout << "WINDOWS VERSION was not defined.\n";
#endif

cout << "Done.\n";
return 0;
}

결과

Checking on the definitions of  DemoVersion, DOS VERSION  and
WINDOWS VERSION...

DemoVersion defined.

DOS VERSION defined as: 5

WINDOWS VERSION was not defined.

DemoVersion defined.

DOS VERSION not defined!

WINDOWS VERSION was not defined.

Done.



===== PAGE 600 =====
제17일 전처리계 ee 599

분석 [리스트 17.2]는 #undef DOS_VERSIONS] 호출된 29번 줄까지는 [리스트

17.1]과 같습니다. 이렇게 하면 DOS_VERSIONO]Z#= 용어가 다른 정의를

하지 않고도 무효로 됩니다. 예제의 나머지는 단지 출력을 되풀이합니다.

DemoVersionz} \184120\_\144910씨은 처음에 했던 대로 되지만 DOS_VERSION

BARS 나중에 참이 됩니다. 두 번째 경우의 DOS_VERSIONS 정의되지 않은 것
으로 됩니다.

AHS 컴파일(000에0081 Compilation)
#061006과 #ifdef, Helse, #ifndef 등을 잘 섞어 쓰면 여러분이 정의한 것에 따라 =
로그램이 다르게 컴파일됩니다. 이렇게 하면 하나의 원시 코드로 여러 개의 엔진

또 다른 일반적인 사용은 06008가 있느냐 없느냐에 따른 조건부 컴파일을 하게
할 수 있다는 것인데 나중에 보게 됩니다.

DO 여러분의 코드로 동시에 여러 개의 버전을 만들 땐 조건부 컴파일을 합시다.

DONT 조건부 컴파일을 너무 복잡하게 만들지 Beet,

bo    HundetS 가능한 한 많이 써서 여러분의 코드가 '정의라는 미로'에 빠지지
말게 att

00 포함 검사를 자주 합시다.

매크로 함수(0400 Function)
06806 지시자는 매크로 함수를 만들 때 사용됩니다. 매크로 Y= #00606를 A}
용하여 만든 기호인데 마치 다른 함수처럼 인수를 가집니다. 전처리계는 주어진
인수에 따라 치환 문자열을 치환하여 버립니다. 예를 들어, TWICES 다음과 같
이 정의했다 합시다.
#define TWICE(x) ( (x) * 2)
그때

TWICE(4)


===== PAGE 601 =====
600 ec 제3주

을 하면 1\108(4)는 없어지고 8이 대체됩니다. 만일 4를 넣으면 전처리계는 ( (4)
* 2 )으로 대체할 것입니다. 이 Ae 결국 8로 계산됩니다.

매크로 함수는 하나 이상의 매개 변수를 가질 수 있고 각 매개 변수는 매크로 함
수에서 반복적으로 사용될 수 있습니다.

#define MAX(x,y) ( (x) > (72 ? (x) : Gy) 2
#define MIN(x,y) ( (x) < (y) ? () : Cy) )

매크로 함수 정의에서 매크로 이름 바로 뒤에 빈칸 없이 시작 중괄호가 와야 합
니다. 전처리계는 컴파일러와 달리 공백에 민감합니다. 만일 다음과 같이 14%와

(xy) 사이에 SYS 넣고

#06+106 MAX (x,y) ( (x) > Cy) ? Gd) : (yD
MAXS 다음과 같이 사용한다면

10【×=ㅋ5, >= 7, z
2 = MAX(x,y)

중간 파일은 다음과 같이 만들어집니다.

int X=(5 >, y= 70, ZF
z= (yy) € GO > &) 7 GO f(y) 2 Gay)

이렇게 되면 매크로 함수를 수행시키는 것이 아니라 단지 문자열 치환만 일어나
Al 됩니다. MAX (xy) ( 00 > 00 ? 00 : 07 )로 되고 그 뒤에 665)가 또 붙게
됩니다. MAX} (xy) 사이에 공백이 없어야

int x=5,yY=7, Z
z=7;

이 됩니다.

왜 괄호들이 필요한가?
여러분은 왜 위의 매크로 함수에 괄호가 많은지 의아해 할 것입니다. 전처리계는
인수가 괄호에 둘러싸여야 한다는 강제 규정을 가지진 않습니다. 그러나 괄호는
여러분이 생각지도 ee 부작용으로부터 프로그램을 보호하여 줍니다. 예를 들어,
MAXS 다음과 같이 정의했다 합시다.

#define MAX(x,y) x >y ? 1



===== PAGE 602 =====
제17일 전처리계 ee 601

5와 7이라는 값이 전달되었을 때 정상적으로 작동할 것입니다. 하지만 좀더 복잡
한 수식을 전달하면 [리스트 17.3]과 같이 전혀 다른 결과가 발생합니다.

[리스트 17.3] 매크로 함수에서 괄호 사응

1: // [리스트 17.37 매크로 함수에서 괄호 사용
2: #include <iostream.h>
Se
4: #define CUBE(a) ( (a) * (a) * (a) )
5: #define THREE(a) at axa
6:
7: int main()
8: {
9%   long x = 5;
10: long > = CUBE(x);
11: long z = THREE(x);
12s
13: cout << "y: " << y << endl;
14: cout << "z: " << z << endl;
1532
16: longa=5,b=7;
17: y = CUBE(atb);
18:  z = THREE(atb);
19%
20: cout << "y: " << y << endl;
21: cout << "z: " << z << endl;
22: return 0;
25: +}
결과 y: 125
Ze 125
y: 1728
Ze 82

4번 줄에서 매크로 CUBE7} 정의되었고 인수 x7} 사용 시마다 괄호에 넣
져 있습니다. 5번 줄의 THREE 정의는 괄호 없이 사용되었습니다.

이 매크로 함수들을 처음 사용할 때, 값 5가 매개 변수로 주어졌고 두 개의 매크
로 함수가 다 잘 동작됩니다. 0088(5)는 ( (5) * (5) * (5) )로 확장되고 125가 됩
니다. THREE(S)= 5 * 5 * 5로 되고 역시 125로 됩니다.

(a
개

두 MAS] 16-18번 줄에서 매개 변수는 5 + 7입니다. 이 경우 0088(5+7)은


===== PAGE 603 =====
602

66 제주

( (5+7) * (5+7) * (5+7) )

이 되고

( (12) (12) * (12) 2

가 되어 반환값은 1,7280] 됩니다. THREE(S+7)2
5+7*5+7>*×5+ 7

이 되고 곱셈이 덧셈보다 연산순위가 BOBS
5+(7%*5)+(7%5) +7

이 되어

5+ (35) 주 (55) + 7

은 82로 계산됩니다.

매크로와 함수 및 BS=l(Template)

매크로 함수는 0++에서 4 가지 SAS 가집니다. 첫째는 매          혼
이 오는데 매크로는 한 줄에 정의되어야 하기 때문입니다. 그 줄을 역사선 문자
(VS 써서 확장시킬 수 있지만 매우 큰 경우 다루기가 어렵습니다.

둘째 문제는 매크로 함수는 사용시 확장됩니다. 이는 만일 매크로 함수가 100번
TEMA 치환은 100번 일어나는데 함수 호출의 경우 한 번 일어나고 호출된다
는 점이 다릅니다. 물론 함수 호출이 부하가 크므로 매크로 함수가 FES 빠릅

y
I
on
4o
&

1
i

a

중 단위로 치환이 일어난다는 것은 세 번째 문제를 일으키는데 컴파일러에 의한
중간 코드에는 매크로 함수가 없다는 것이고 이는 디버그할 때 어려움을 줍니다.
마지막 문제점은 매우 Puch 매크로 함수는 형을 보장 못합니다. 어떤 인수라도
매크로 함수에 쓸 수 있다는 편의점이 있긴 하지만 이는 강형인 0++의 속성을
저해함니다. 템플릿은 이 문제들을 해결하는데 19일날 보게 될 것입니다.

확장 StA(inline Function)

종종 매크로 함수 대신 확장 함수(0006 functions 선언하는 것이 가능합니다. 예
를 들어, [리스트 17.4]는 CUBE 함수를 만드는데 [리스트 17.3]의 CUBES 같은
일을 하지만 Yo] 안정성(006-8066)을 보장합니다.


===== PAGE 604 =====
세17일 전저리게 ee 603

[리스트 17.4] 매크로 함수 대신 확장 함수의 사응

#include <iostream.h>

inline unsigned long Square(unsigned long a) { return a * a; }
inline unsigned long Cube(unsigned long a)
{ return a*a* aj; }
int main()
{
unsigned long x=1 ;
for (35)
{
cout << "Enter a number (0 to quit): ";
Cin o> xs
if (x == 0)
break;
cout << "You entered: " << x;
cout << ".. Square(" << x <<i")= Us
cout << Square(x);
cout <<". Cube(™ << x <K x <<"): ";
cout << Cube(x) << "." << endl;
3
return 0;

1 가

Enter a number (0 to quit): 1

You entered: 1. Square(1): 1. Cube(1): 1.
Enter a number (0 to quit): 2

You entered: 2. Square(2): 4. Cube(2): 8.
Enter a number (0 to quit): 3

You entered: 3. Square(3): 9. Cube(3): 27.
Enter a number (0 to quit): 4

You entered: 4. Square(4): 16. Cube(4): 64
Enter a number (0 to quit): 5

You entered: 5. Square(5): 25. Cube(5): 125
Enter a number (0 to quit): 6

You entered: 6. Square(6): 36. Cube(6): 216
Enter a number (0 to quit): 0

=    두 개의 확장 함수001106 function) Square(), CubeQ7} 21°15)
다. 각각 확장형으로 선언이 되었고 따라서 매크로 함수와 같이 호출

확장되고 함수를 호출하는 PSE 없습니다.


===== PAGE 605 =====
604 ee 제3주

16번 줄에서 함수 Square7} 함수 Cubes 같은 방식으로 호출됩니다. 이들은 확장
함수이므로 이렇게 쓰여진 것과 같습니다.

16: cout << ". Square(" << x << "Jr "KK KEK KN, CubeC" << x << "):

리브 사운과는 것이 permgmee. TY

사이즈 4
“ cen Manipulation)

#define WRITESTRING(x) cout << #x
라고 한 뒤
WRITESTRING(This is a string);

라고 하면 전처리계는 이렇게 BUC.

cout << "This is a string";

Thisis a string] cout] PLES 겹따옴표로 둘러 쌓였습니다.

문자열 94:8 (Concatenation)

da 연선자는 여러분으로 하여금 하나 이상의 단어를 Hol 하나의 새로운 단
어로 만듭니다. 이 새로운 단어는 클래스 이름, 변수명, 배열에서의 변위, 혹은 어
디서든 일련의 글자들의 연속이 나타날 수 있는 모든 곳에 사용될 수 있는 토큰

이 됩니다.


===== PAGE 606 =====
제17일 전처리계 ee 605

당분간 5개의 함수 fOnePrint, fTwoPrint, fThreePrint, fFourPrint, fFivePrint'= 가정합
시다. 다음과 같이 선언할 수 있습니다.

#define fPRINT(x) + ## x ## Print

fTwoPrintS 만들기 위해 fPRINT(Two)S 사용하고 fThreePrint$ 만들기 위해
fPrint(Three)S 사용합니다.

2주 A 공부의 결론에서 20018 클래스가 만들어졌습니다. 이 BSS Gz] List
의 객체만 다룰 수 있었습니다. 이 목록이 잘 동작한다고 가정하고 이제 여러분

객
은 동물, 자동차, 컴퓨터, 기타의 SSS 만들고 싶다 합시다.

근 방식은 AnimalList, CarList, ComputerList 등을 만들고 적절한 곳에서
코드를 자르고 붙이는 것입니다. 이는 순식간에 악몽이 될 것입니다. 왜냐하면 한
이 모든 곳으로 번질 것이기 때문입니다.

다른 방식은 매크로 함수를 사용하여 연결 연산자를 쓰는 것입니다. 예를 봅시다.

#define Listof(Type) class Type##List \
<\
public: \
Type##List(){} \
private: \
int itsLength; \
3;

사실 이 예제는 좀 희박한 예인데 그럼에도 불구하고 개넘상으로 모
쏘드와 자료는 갖고 있습니다. 여러분이 AnimalListS 만들고 싶으면

Listof (Animal)

이라고 하면 AnimalList2] 선언이 만들어집니다. 여기에도 약간의 문제가 있는데
이는 19일째 날에 템플릿에서 공부할 것입니다.

내장 OlA=(Predefined Macro)

많은 컴파일러들이 유용한 매크로를 내장시켜 놓았습니다. _DATE_, _TIME_,
_LINE_, _FILE_$°] 그것입니다. 각 이름은 두 개의 WS 문자(_)로 둘러 쌓

여 있는데 여러분이 만드는 이름과 충돌하는 것을 피하기 위함입니

전처리계는 이들을 만나면 적절한 ABS 합니다. _ 0414 _ 는 현재의 날짜로 바
꾸고 _TIME_= 현재의 시간, _LINE_, _FILE_© 현재 원시 코드의 줄 번호



===== PAGE 607 =====
606 ㅇㅇ 제3주

와 파일 이름으로 ¥
닙니다. 여러분이(_ :
램이 컴파일된 날짜가
Nee ee ee

이들은 전처리게에서 바뀌며 실행시 바뀌는 것이 아
._ 를 졸리시기펀 Bae 놀러가 eo
옵니다. 디버깅할 때 매우 편합니다.

assert()

많은 컴파일러가 assert) HALS 제공합니다. 매개 변수가 참이면 assent 참을
돌려주고, 매개 변수가 거짓인 경우 어떤 코드 BRS 실행합니다. 많은 컴파일러
WA AS 프로그램을 중단하고, 다른 컴파일러는 예외 사항을 실행합니다.
예외 사항은 20일째 배움니다.

assert()2} 강력한 특징 중 하나는 DEBUG7} 정의되지 않은 BHA 전처리계는
assert() 부분을 코드에 넣지 않는다는 것입니다. 이는 프로그램 개발시 유용하고
마지막으로 프로그램이 완성된 후에 DEBUGS 빼어 버리면 프로그램 부하라든지

코드 량의 증가가 없어집니다. 컴파일러가 제공하는 055000보다는 여러분 자신의
assert) 만들 수 있습니다. [리스트 ITS 간단한 86600 매크로를 보여줍니다.

[리스트 17.5] 간단한 35500) 매크로

1: // [리스트 17.53 assert

2: #define DEBUG

3: #include <iostream.h>

4:

5: #ifndef DEBUG

6:    #define ASSERT(x)

7: #else

8:    #define ASSERT(x) \

9:       if <! (x)) \

10;      { \

114        cout << "ERROR!! Assert " << #x <<" failed\n"; \
12:       cout << "on Line " << _LINE_ << NAF
458        cout <<" in file " << FILE << NaN
14:     }

15: #endif

168

17%

18: int main

192 3

20:    int x = 5;

21   cout << "First assert: \n";

223   ASSERT (x==5);



===== PAGE 608 =====
제17일 전처리계 ee 607

23:   cout << "\nSecond assert: \n";
24:   ASSERT(x != 5);

255   cout << "\nDone.\n";

26:   return 0;

26: }

겔과  First assert:

Second assert:

ERROR!! Assert x!=5 failed
on Line 24

in file test1704.cpp

Done.

불셀 ?번 좋에서 DEBUG} 정의되었습니다. 이것은 컴파일시 명령어 줄
128에서 이루어지고 따라서 여러분은 이 WSS 죽였다 살렸다 할 수

니다. 8 - 15번 줄에서 assert) 매크로가 정의됩니다. 대개 이 부분이 헤더 파일
ASSERT.HPPo}] 정의되어 있는데 따라서 여러분은 이 BRS 구현할 때 헤더 파
일만 포함시키면 됩니다.
5번 줄에서 DEBUG7} 검사되었습니다. 정의되어 있지 HOw assert 아무런 코
드도 생성하지 않습니다. 정의되어 있다면 8-14번 So} 기능이 적용됩니다.
assert() 그 자체는 하나의 긴 문장으로 7줄의 원시 SES 잡아먹습니다. ow 줄
에서 매개 변수로 값이 전달되고 검사됩니다. 거짓이면 11-13번 So] 블려지고 오
류 USS 출력합니다. 참값이 전달되면 아무 일도 않습니다.

수 YO sor
tly flo

assert() 가지고 디버깅하기
프로그램을 할 때 여러분은 마음속 깊은 곳에 이것은 맞는다라고 간주해 버
경우가 많습니다. 즉, 함수가 어떤 값을 당연히 갖는다고 생각하고 또
터가 참이라고 생각하는 등입니다. 여            Z
에서는 그렇지 않은 것이 버그의 본질입니다. qs 들어,
하다고 생각했는데 프로그램이 깨지는 경우입니다. 89600
를 코드 안에 정기적으로 넣어주기만 한다면 버

로 포인터를
달할 때 포인터가 유효한지를 assenQS 확인합시다. 코드 안에서 변수의 특정 값
에 의존하게 되는 경우 일단 assez 확인하여 봅시다.


===== PAGE 609 =====
608 ㅇㅇ ABS

assert 자주 써도 손해가 없습니다. DEBUGS] BIS 취소하면 코드에서 아예
없어집니다. 게다가 좋은 도큐먼트가 되어 나중에 특정 시기에 여러분이 생각하
는 것이 SARS 갖는지 확인할 때 좋은 효과를 발휘합니다.

assert()2} 예외 Ate+S(Exceptions)
20일째 되는 날 오류 ZAS 다루기 위해 예외 사항들에 대해 공부할 것입니다.
889600는 실행 시의 OHS 다루기 위해 만들어진 것이 아니라는 것을 알아야 합
니다. 예를 들면, 잘못된 자료, 메모리 부족, a 수 없는 파일 등등입니다. 65000
단지 프로그래밍 오류만을 잡기 위해 만들어졌습니다. 즉, 88000가 SAS 하
여러분의 코드 상에 오류가 있는 것입니다.

이는 치명적인데, 왜냐하면 여러분이 여러분의 고객에게 실행 코드를 올려놓으
assert) 없어진 상태이기 때문입니다. AYA) LHS assert] 의존할 수 WF
다. assert 이미 거기에 없기 때문입니다.

899610를 메모리 할당후의 반환값을 검사하는데 쓰는 것이 일반적인 오류입니다.

re ci

S, [본

00

Animal *pCat = new Cat;

Assert(pCat);// 틀린 용법

pCat->SomeFunction() ;

이는 고전적인 오류입니다. 프로그램을 검사할 때마다 프로그래머의 메모리는 충
분하고 따라서 asset SHS 않습니다. 단지 검사할 때마다 부하를 잡아먹습
니다. 다음 이 프로그램이 열악한 환경을 가진 고객의 컴퓨터에 실행 파일만 을
라가게 됩니다. 이때에는 25000가 빠진 상태입니다. 환경이 열악하여 new7} 실패
하고 포인터로 널이 반환됩니다. 하지만 이때에는 89600가 없는 상태이므로 =
로그램은 다음줄 pCat->SomeFunction(o] 와서 부서지게 됩니다.

메모리 할당시 NULLS] 반환되는 것은 오류가 아니라 예외 사항입니다. 이러한
경우로부터 벗어나야만 합니다. 기억합시다. 26800가 정의되어 있지 않으면
889600는 없어집니다. 예외 사항의 자세한 부분은 20일째에서 공부합시다.

부작응(5106 Effect)
855600가 없어진 후 버그가 생기는 것도 흔한 일 중 하나입니다. 이는 프로그램
중 assert) 혹은 단지 HIS 잡기 위해 만든 코드에서 의도하지 않게 만든 부작

용 때문입니다. 예를 들면,


===== PAGE 610 =====
제17일 전처리계 ee 609

ASSERT( x = 5 )

에서 실제는 x == 5를 검사하려다 이런 오류를 만든 것입니다.

예를 들어, 이 4998070문을 쓰기 전 *를 0으로 설정하는 함수를 호출했다고 합
시다. 위의 4558010에서 여러분은 x7} 5와 깥은지를 검사했다고 생각했지만 실
제는 *에다 5를 대입하였습니다. 검사는 참으로 됩니다. 왜냐하면 x = SE *를 5
로 설정하고 5값을 반환하는데 5는 참으로 판단되기 때문입니다.
이렇게 하고 나면 프로그램은 잘 돌아갑니다. 여러분의 프로그램을
터에 설치하고 나면 디버그는 없어집니다. 그때에는 *가 0으로 설정
로 프로그램에서 탈이 납니다.

나중에 연락을 받고 와서 디버그를 실행시키면 프로그램은 또 잘 돌아갑니다.

프로그램시 부작용에 주의합시다. 디버그를 VAs 때에만 오류가 발생하면 디버
그 부분을 잘 살펴보도록 합시다.

델리
ox
고
10

클래스의 SHA (Invariants)

대부분의 클래스는 클래스의 멤버 함수가 끝날 때마다 참이 되어야 하는 특정 조
들을 가집니다. 이 클래스의 불변성은 여러분 클래스의 필수 부분입니다. 예를
어봅시다. CIRCLE 객체는 반경이 0이면 안됩니다. ANIMAL 객체의 나이는 0보
고 100보다 작아야 합니다.

조건들이 참인 경우에만 AMS 반환하는 110808060 메쏘드를 선언하는 것은
HW 유용합니다. 여러분은 956000808060)를 모든 클래스 메쏘드의 시작에 넣
을 수 있습니다. 예외 사항은 00808060가 여러분의 생성자가 실행되기 전이나
소멸자의 실행이 끝난 후 참값을 반환하지 않는다는 것입니다. [리스트 17.6|에서
Invariants)S 보기로 합시다.

묘 때
테

d

[리스트 17.6] Invariants() 사응법

#define DEBUG

#define SHOW INVARIANTS
#include <iostream.h>
#include <string.h>

#ifndef DEBUG

#define ASSERT(x)
#else

#define ASSERT(x) \

CONBDUFWD | OO


===== PAGE 611 =====
610 ee ABE

9:       if (1 GOD 호

10:      aN

115         cout << "ERROR!! Assert " << #x <<" failed\n"; \
12:        cout << "on 1106" << _LINE_ << "\n"s \

13:         cout <<" in file " << _FILE_ << "\n"; \

14:      a

15: #endif

16:

17:

18: const int FALSE = 0;
19: const int TRUE = 1;
20: typedef int BOOL;

218

22:

23: class String

248 4

252 public:

26: ㅣ /7 생성자 및 소멸자

(alg    String;

28:    String(const char *const);

29:    String(const String &);

30:    “String;

512

32:    char & 006『2010『ㅁ(101 offset);

$5:    char operatorL](int offset) const;
34:

$5!    String & operator= (const String &);
36:    int GetLen() const { return itsLen; }
37:    const char * GetString() const { return itsString; +
38:    BOOL Invariants() const;

$9:

40: private:

41:    String (int); // 전용 생성작

42:    char * itsString;

43:    // unsigned short itsLen;

44:    int itsLen;

456 J}

46:

47: |// 널 문자열을 반드는 기본 생성자
48: String::String®

49: ¢£

50    itsString = new charl1];
a1;    itsStringLO] = '\0';

52:    itsLen=0;

55:    ASSERT(Invariants());
54: +



===== PAGE 612 =====
제17일 전처리계

ee

611

55
56:
at:
501
59:
60:
61:
62:
63:
64:
65:
66:
67:
68:
69:
102
(1%
fa:
75%
142
(5s
76:
(Ade
78:
195
80:
81:
82:
83:
84:
853
86:
87:
88:
89:
90:
91:
92:
93%
94:
95%
96:
Or
98:
99:

//

// 전용 생성작

//

String::String(int len)
{

itsString = new charLlent1];
for (int i = 0; i<=len; i++)
itsStringlil = '\0';
itsLen=len;
ASSERT(Invariants());

// 문자 WAS 문자열로 바꿈     '
String::String(const char * const cString)
{
itsLen = strlen(cString);
itsString = new charLitsLen+1];
for (int i = 0; i<itsLen; i++)
itsStringlil = cStringLlil;
itsStringLitsLenJ='\0';
ASSERT(Invariants());

// 복사 생성작
String::String (const String & rhs)
{
itsLen=rhs.GetLen();
itsString = new charLitsLent1];
for (int 1 = 0; i<itsLen;i++)
itsStringlil = rhsCil;
itsStringLitsLen] = '\0O';
ASSERT(Invariants());

// 소멸자, SHE 메모리를 해제함

Stping?: String (0

{
ASSERT(Invariants());
delete [4 itsString;
itsLen = 0;

// 등지 연산자

io  pal

fi

100: String String::operator=(const String & rhs)


===== PAGE 613 =====
612 ce HBS

1015 +

102:   ASSERT(Invariants());

103:   if (this == &rhs)

104:      return *this;

105:   delete [] itsString;

106:   itsLen=rhs.GetLen();

107   itsString = new charLitsLen+1];
108:   for (int i = 0; i<itsLen;it+)
109:      itsStringLil = rhsLlil;

110:   itsStringLitsLen] = '\0';

111   ASSERT(Invariants());

112:   return *this;

113: 2

114:

115: // 비장수 변위 Atte

116: // 8 수 있도록 문자의 참조자를

117: // 반환

118: char & String::operatorL](int offset)
1192 +

120:    ASSERT(Invariants());

1218    char retVal;

122:    if (offset > itsLen)

1255      retVal = itsStringLitsLen-11];
124:    else

12D      retVal = itsStringLoffset];
126:    ASSERT(Invariants());

127:    return retVal;

128: }

129: // 상수 변위 연산자

150: //

131: char String::operatorL](int offset) const
132:

135:    ASSERT(Invariants());

134:    char retVal;

135:    if (offset > itsLen)

1562      retVal = itsStringLitsLen-1];
137:    else ~

138:      retVal = itsStringLoffset];
139:    ASSERT(Invariants());

140:    return retVal;

1412 가

142: BOOL String::Invariants]

145: {

144: #ifdef SHOW INVARIANTS

145:    cout << " String OK ";

146: #endif



===== PAGE 614 =====
세17일 전처리계

ee 613

147:
148:
149:
150:
19
152%
1535
(54:
155%
1568
157%
158:
159%
160:
161:
162:
163:
164:
165):
166:
167:
168:
169:
170
VOU
1021
VS
174:
1758
176:
(Cs
178:
A719:
180:
1811
182:
183:
184:
185%
186:
187:
188:
189:
190:
191:
192:

return ( (itsLen && itsString) |!
(litsLen && !itsString) );
}
class Animal
{i
public:
Animal(): itsAge(1), itsName("John Q. Animal")
{ ASSERT (Invariants() ); }
Animal (int, const String&);
“Animal (){}
int GetAge() £ ASSERT(Invariants()); return itsAge;}
void SetAge(int Age)
{
ASSERT(Invariants());
itsAge = Age;
ASSERT(Invariants());
}
String& GetName()
{i
ASSERT(Invariants());
return itsName;
}
void SetName(const String& name)
4:
ASSERT(Invariants());
itsName = name;
ASSERT (Invariants());
}
BOOL Invariants();
Private:
int itsAge;
String itsName;
3;

Animal::Animal(int age, const String& name):
itsAge(age),
itsName (name)
{
ASSERT(Invariants());
1:

BOOL Animal::Invariants()

¢

#ifdef  SHOW INVARIANTS
cout << '" Animal OK ";

#endif


===== PAGE 615 =====
614 ee 제3주

193:    return (itsAge > 0 && itsName.GetLen());

194: }

195:

196: int main()

197: 4

198:    Animal sparky(5,"Sparky");

199:    cout << "\n" << sparky.GetName().GetString@ <<" is ";
200:    cout << sparky.GetAge() << years old.";

201:    sparky.SetAge(8);

202:    cout << "\n" << sparky.GetName().GetStringQ) << "is ";
205:    cout << sparky.GetAge() <<" years old.";

204:    return 0;

205: +

과  String OK String OK String OK String OK String OK

String OK String OK String OK Animal OK Animal OK
Sparky is Animal OK 5 years old. Animal OK Animal OK
Animal OK Sparky is Animal OK 8 years old. String OK

셀 5 - 15번 좋에서 assert) 매크로가 정의되었습니다. DEBUG7t 정의되었다면
assert()7} FALSE 때 오류 문장을 출력할 것입니다.

(aa

38번 줄에서 String 클래스 멤버 B= Invariants()7} 선언되었고 142 - 149번 줄에
서 정의되었습니다. 생성자가 48 - 54번 줄에서 선언되었고 53번 줄에서 객체가
생성된 후 적절한 생성이 이루어졌는지 알기 위해 Invariants()7} 호출되었습니다.

이와 같은 형태가 다른 생성자들에서도 반복되고 소멸자의 경우 객체를 깨뜨릴
때 100808060를 호출합니다. 다른 클래스의 함수들도 특정 동작을 하기 전과 반
환하기 전 10080806()를 호출합니다. 이러한 방법들이 0++의 기본 원칙들을 지키
는 것입니다. 멤버 함수와 생성자, 소멸자들은 유효한 상황에서 작업해야 합니다.
175번 줄에서 Animal 클래스는 그 자신의 100808060 메쏘드를 선언하였고 188 -
194번 So] 구현되었습니다. 10106 함수가 InvariantsOS 호출하는 154, 157, 160,

162번 줄을 주목합시다.

중간값(|마0110 Value) 234
는 방법 외에 여러분은 포인터, 변수,
문자열의 현재 값을 출력해 보는 것을 원할 수 있습니다. 여러분의 프로그램에서
각 과정에서의 가정들을 검사하는 것은 매우 유효한 방법 중 하나입니다. 예제를
한번 봅시다.

i


===== PAGE 616 =====
세17일 전처리계 ee 6015

[리스트 17.7] DEBUG 양식에서 값을 SHOE 것

// [리스트 17.71 06806 양식에서 값을 즐력하는 것
#include <iostream.h>
#define DEBUG

#ifndef DEBUG
#define PRINT(x)
#else          ‘
#define PRINT(x) \
cout << #x << ":\t" << x << endl;
: #endif

그 9 600 4 BAU FWP =
CG es cs os se Se se Ss as ie

= =
N =
a.

: enum BOOL { FALSE, TRUE } ;

a ~
WN

: int main()
sf

~
ww ok
nu
…‥…

int x = Ss
long y = 738981;
PRINT(x);
for (int i = 0; i < x; i++)
{
PRINT(i);
}

NNNNDND = = =
FWNMH = OO ON

PRINT (y);
PRINTC("Hi.");
int *px = &x;
PRINT(px);
PRINT (px);
return 0;

NNN NM PKL PY
oO CO CON 0 녀
vy

결과

Sei ed 때 제 wee. 가 SS
~ 에 650 | OW

:          73898
"AAAs     Hi
px:         0x2100 ( 다른 값을 받을 수 있습니다. )

*DX:       5


===== PAGE 617 =====
616 ㅇㅇ 제주

불셀 5 - el 줄의 매크로는 주어진 마개 변수의 현재 we
^” 주어진 첫 번째 것은 매개 변수의 문자열화된

2 cout: 콜론과 탭문자를 출력하는 “WS 받습니다. 세 번째로 004는 매개
변수 xo} 값을 받고 600의 값을 받아 개행 문자를 출력하고 버퍼를 비옵니다.

디버그 수준(00648 Level)

크고 복잡한 프로젝트에서 단순히 00008를 만들었다 지웠다 하는 것보다
실적인 통제 방법을 원합니다. 여러분은 디버그의 수준을 정하여 어떤 수
크로를 ~  안할 것인지를 검사할 수 있습니다.

수준을 정의하기 위해 #efine DEBUG 뒤에 숫자를 FUch 어떤 숫자를 써도 좋
지만 보통 HIGH, MEDIUM, LOW, NONES 가집니다. [리스트 17.8]은 [리스트
17.6]을 변화시킨 것인데 여기에서 이들의 사용법을 보여줍니다. 다른 클래스 메
RE Ob Invariants 지면상 제외시켰습니다. 하지만 다른 YS [리스트 17.6|과
같습니다.

이 프로그램을 첨파일하려면 [리스트 17.6]의 43-136번 SS 64와 oe 줄 사이에 복
사하시오.

[리스트 17.8] DEBUGO 수준

0: enum LEVEL { NONE, LOW, MEDIUM, HIGH };
1: const int FALSE = 0;

2: const int TRUE = 1;

3: typedef int BOOL;

4:

5:  #define DEBUGLEVEL HIGH

6:

7:  #include <iostream.h>

8: #include <string.h>

9:

10: #if DEBUGLEVEL < LOW // MEDIUM 혹은 HIGH®|°°F 함
113    #define ASSERT(x)

12: #else

132    #define ASSERT(x) \

14:     if (16802 XN


===== PAGE 618 =====
세17일 전처리계 ee

617

15<
16:
1271
18:
19:
20:
21%
22:
29;
24:
25%
26:
27%
28:
29:
30:
31:
32:
55%
34:
25:
36:
Ss
38:
391
40:
41:
42:
43:
44:
45:
46:
4:
48:
49:
50:
516
52:
5S
54:
553
56:
a0:
53:
DoF
60:

{ \
cout << "ERROR!! Assert " << #x <<" failed\n"; \
cout << " on Line.” <9 LINE | << "An"; X
cout <<" in file " Si RELE: < jp <N
}
#endif

#if DEBUGLEVEL < MEDIUM
#define EVAL(x)
#else
#define EVAL(x) \
cout << #x << "i\t" << x << endl;
#endif

#if DEBUGLEVEL < HIGH
#define PRINT(x)
#else
#define PRINT(x) \
cout << x << endl;
#endif

class String
{
public:
// 생성자 및 소멸자
String();
String(const char *const);
String(const String &);

“String();

char & operatorLlCint offset);
char operatorl](int offset) const;

String & operator= (const String &);
int GetLen()const { return itsLen; }
const char * GetString() const

{ return itsString; }
BOOL Invariants() const;

private:
String (int); // MB 생성자
char * itsString;
unsigned short itsLen;

3;


===== PAGE 619 =====
618 ee 제3주

61: BOOL String::Invariants() const

62: ¢{

65:    PRINT("(String Invariants Checked)");
64:    return ( (BOOL) (itsLen && itsString) 11
65:       (!itsLen && !itsString) );

66: }

67:

68: class Animal

69: {

70: public:

(1s    Animal():itsAge(1),itsName("John Q@. Animal")
72:      {ASSERT (Invariants());}

(52

(4:    Animal (int, const String&);

Tor    “Animal () {}

(6:

(ti    int GetAge()

18:    {

79:      ASSERT(Invariants());

80:      return itsAge;

81:    Be

82:

85:    void SetAge(int Age)

84:    {

85:      ASSERT(Invariants());

86:       itsAge = Age;

875      ASSERT(Invariants());

88:    }

89:    String& GetName()

90:    {

91      ASSERT(Invariants());

92:      return itsName;

93:    }

94:

95:    void SetName(const String& name);
96:    {

97:      ASSERT(Invariants());

98:       itsName = name;

99:      ASSERT(Invariants());

100:   내

101:

102:   BOOL Invariants();
103: private:

104: int itsAge;

105: String itsName;
1063 23



===== PAGE 620 =====
제17일 전처리계 ee 619

107:

108: BOOL Animal::Invariants()

109% £

110:   PRINT("(Animal Invariants Checked)");
1118   return CitsAge > 0 88 itsName.GetLen());
1126 }

113:

114: int main()

115,"

1108   const int AGE = 5;

108    EVAL(AGE) ;

118:    Animal sparky (AGE,"Sparky") ;

119:    cout << “\n'""<< sparky.GetName().GetString();
120:    cout << "is 대

1216    cout << sparky.GetAge() <<" years old.";

1221    sparky.SetAge(8);
123:    cout << "\n" << sparky.GetName().GetString();
124"    cout << " 16
1258    cout << sparky.GetAge() <<" years old.";
126:    return 0;
127% D
a i    AGE:                            5
(String Invariants Checked)

(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)
(String Invariants Checked)

Sparky is (Animal Invariants Checked)

5 Years old. (Animal Invariants Checked)
(Animal Invariants Checked)

(Animal Invariants Checked)

Sparky is (Animal Invariants Checked)
8 years old. (String Invariants Checked)
(String Invariants Checked)


===== PAGE 621 =====
620 ㅎㅇ 제주

// DEBUG LEVEL = MEDIUM? = 하고 다시 실행시킴
AGE:                        5

Sparky is 5 years old.

Sparky is 8 years old.

분석  10 - 20번 줄에서 DEBUGLEVEL°] LOW#t} 낮으면(즉 NONE®]%) assert()

매크로의 기능을 벗겨버립니다. 어떠한 형태의 디버그 형태가 존재하기만

하면 499800는 동작합니다. 23번 줄에서 DEBUGLEVEL©] MEDIUM#t} 작기만

하면 EVAL 기능이 없어지도록 하였습니다. 즉, DEBUGLEVEL7} 8000이거나
Ｌ0\이면 8741.이 작동을 안합니다.

마지막으로 29-34번 줄에서 DEBUGLEVEL®] 11008보다 작으면 PRINT 매크로가
기능 못하도록 선언되었습니다. J, PRINTE 110로 되어있을 때에만 사용됩니다.
PRINTS: 100808060 RES 사용하여 HAS 출력합니다. 117번 줄에서 현재의
나이를 계산하기 위해 EVAL] 사용되었습니다.

DO     매크로 이름에 대문자를 쓰도록 합시다. 이는 권장 사랑인메 이렇게 하지 않
으면 다른 프로그래머들이 혼동합니다.
DON'T 매

크로가 부작용을 낳지 않도록 합시다. ASS 증가시키거나 매크로 안에서
값을 치환하지 않도록 합시다.
DO     매크로 함수에서 인수는 괄호로 FSH.

요약

ese 전처리계를 잘 다루는 법을 배웠습니다. 매번 컴파일러를 돌릴 때마다 먼
저 전처리계가 수행되어 전처리계 지시자들00006, #ifdef 등)을 변환시킴니다.

전처리계는 텍스트 치환을 하며, 매크로를 사용하면 좀더 복잡해 a 수 있습니다.
fifdet, #else, #ifndef 등을 사용하여 조건부 컴파일할 수 있는데 이 조건에서는 이
gal 컴파일되게 하고 저 조건에서는 저렇게 컴파일되게 합니다. 이렇게 하면 프
로그램이 하나 이상의 엔진에서 가동할 수 있게 합니다. 또 종종 디버그 정보를
포함하게 합니다.


===== PAGE 622 =====
제17일 전처리계 ee 621

매크로 함수는 컴파일시 매크로로 전달된 인수에 기반 하여 복잡한 텍스트 치환
이 일어나게 합니다. 각 인수에 괄호를 넣는 것이 올바른 치환이 일어나게 하는
데 필수 조건이 됩니다.

매크로 함수와 전처리계는 0보다는 0++에서 덜 중요합니다. 0++은 상수 변수,
템플릿 등 전처리계보다 윌등한 대안물들을 제공하는 기능이 있기 때문입니다.

Q&A

Q C++OME 전쳐리계보다 월등한 기능들을 제공하는데도 전쳐리계가 아직 쓰이는 이
유는 무엇입니까?

A 먼저 CHE CHA 나왔으므로 (에서 중요한 것은 모두 갖고 있습니다. 두 번찌로
CHa} 아직 빈번히 쓰이는 전처리계 기능(포함 감시자 기능) Bo

Q Qe! 함수를 쓸 수 있는데도 매크로 함수를 쓰는 이유는 무엇입니까?

A 매크로 함수는 줄에서 확장이 일어나는데 같은 명령을 비슷하게 여러 번 반복 입력
해야 하는 경우에 사용됩니다. 템

Q 88 함수와 매크로 중 어떤 것을 쓸 것인가를 어떻게 압니까?

A 대부분 별로 문제가 되지 않습니다. 간단한 것을 쓰도록 합시다. 그런데 매크로는
문자 치환, 문자 열화 기능 및 연결 기능을 제공합니다. 함수에는 이런 기능이 없슴
니다.

Q 디버그 하는 동안 중간값을 출력시키는 전처리계에 대안물은 무엇이 있습니까?

A 디버그 안에 추적 문장을 넣는 것입니다. 자세한 사항은 컴파일러나 디버그 문서를
보도록 합시다.

있습니다. 부록 Dol 있는 답을 보기 전에 각
고                         |

, 다음 장으로 넘어가기 전에 답을 Site


===== PAGE 623 =====
622 eo 제3주

퀴즈
1. 포함 감시자란 무엇입니까?
2 전처리계의 결과를 알 수 있는 중간 파일을 여러분의 컴파일러에게 만들도록 하는 방법
은 무엇입니까?
3. #defind debug 0과 #undef debug 차이점을 말하시오.
4 4개의 내장 매크로를 말하십시오.
5 왜 생성자의 Ad 번째 Boll invariants S 쓰지 못합니까?

연습 문제
1. STRING. HAE 헤더 파일에 포함 감시자문을 작성하십시오.
2 assert()S 다음과 같이 작성하십시오. 디버그 수준 2에서는 오류 문장, 파
호를 출력하고, 디버그 수준 1에서는 오류 문장만을      0          것
않도록 하십시오.
3. debug7} 정의되어 있는지를 검사하고 매개 변수로 전달된 BS 프린트하는 DPrintet
는 매크로를 작성하십시오.

4 오류 문장을 출력하는 함수를 작성하십시오. 오류가 발생한 줄 번호와 함수명을 나타내
야 하고  이주     개는 인수로 전달되어야 합니다.

§. 오류가 발생한 함수의 파일명과 줄 HSS 어떻게 Sorry?

6. 4번 문제로부터 OF 함수를 사용하는 3566「【()를 작성하고 O| assert() 매크로를 호출
하는 구동 프로그램을 작성하십시오.



===== PAGE 624 =====


===== PAGE 625 =====
624 ㅇㅇ 제3주

서문

C++9] 문법에 초점을 맞추다가, 어떻게

흔한 일입니다. 오늘은 다음을 wer.
를 걱체 지향의 관점에서 문제를 분석하는 법
를 거제 지향의 관점에서 설계하기

를 재사용성과 확장성을 고려한 설계

개발 주기(06061000161[ Cycle)

많은 책들에서 개발 주기에 관해 이야기하였습니다. 어떤 사람은 “폭포 방식
(waterfall 1060100)”의 개발 주기 BAS 이야기하였습니다. 그에 따르면 설계자는
프로그램이 무엇을 해야하는지를 결정해야 하고 구성하는 사람은 어떻게 프로그
램이 구성되며 어떤 클래스가 사용되어야 하는지 SS 만들어야 합니다. 그리고
프로그래머는 설계자와 구성한 사람의 의도대로 프로그램을 구현합니다. 설계와
구조가 나오면 거의 끝난 것입니다. 프로그래머가 해야하는 모든 일은 필요한 기
능성만 구현하면 되는 것이었습니다.

Aro] 잘 돌아간다고 하더라도 좋은 프로그램을 Wie 다소 뒤떨
어진 방식입니다. 프로그래머가 일을 진행하는 과정에는 여지까지 해온 것과 앞
으로 남아있는 일 사이의 자연적이고도 또한 필연적인 피드백66606800 과정이
있게 마련입니다. 이것이 사실이라면 좋은 C++ 프로그램은 코드에 들어가기 바로
전까지의 아주 자세한 부분까지 설계가 되어야 하고, 또 전 개발 주기를 거쳐 설
계가 변하지 않는다는 것은 거짓이 됩니다.

설계되어야 하는 양은 프로그래밍이 시작하기 바로 전 단계까지 Bro] 크기와
같습니다. 여러 프로그래머가 몇 달에 거쳐 작업해야 하는 고도의 복잡한 노력은
한 명의 프로그래머가 하루에 짜야하는 간단하고 단순한 유틸리티보다 훨씬 잘
계산된 구조가 필요합니다.

이번 장에서는 몇 년간에 거쳐 확장되고 기등

하는 매우 크고 복잡
Heads 설계에 관해 초점을 맞출             프로
ee                   해

로그래머들은 아

ot om a ae 2;

ste
‘

설계가 되었습니다.

We 확장할 수 있도



===== PAGE 626 =====
제18일 객체 지향 분석과 설계 ce 62

5

che 장에서는 객체 지향의 관점이서 설계의 문재들을 살펴볼 것입니다. 이번
의 목적은 분석의 과정을 재검토하고 설계물을 구현할 수 있도록 CH 문장을

경보 시스템 시뮬레이션

시뮬레이션이란 실제 AAS Bis Saas 것입니다. lees 하는
러 가지 이유가 있는데 훌륭한 설계자는 설계자가 해결하고자 하는 문제를 시
레이션이 얼마나 잘 대담해줄 수 있는지에 대한 충분한 이해가 있어야 합니다.
출발하는 시점에서 이런 문제를 살펴봅시다. 한 가옥에서의 경보 시스템을 시뮬
레이션하도록 요청을 받았다고 해봅시다. 이 가옥은 가운데 홀이 있고 4개의
실이 주변에 있으며 깔끔한 지하실과 집 밑에 차고가 있다고 합시다.

아래 층에는 다음처럼 창문이 있습니다. 부억에 3개가 있고, 주방에 4개가 있

2 o&

여
=

17

침

으며

반침실에 1개, 거실과 안방에 각각 개가 있으며 문 옆에 조그만 창이 있습니다.

4개의 침실은 이충에 있고 각각 2개의 창문이 있는데 단 큰 침실에는 4개의 창
있습니다. 욕실이 2개 있고 각각에 1개의 창이 있습니다. 마지막으로 지하실에

이 가옥에 들어가는 것은 보통 현관을 통해서입니다. 부억에는 비스듬한 유
이 있고 차고에는 차가 SUS 수 있는 두 개 짜리 Bo] 있으며 지하실로 통하
ㅣ 있습니다. 뒤뜰에 지하실로 통하는 문이 역시 하나 있습니다.

문과 창문에 경보 장치가 되어 있습니다. 각 전화기와 침대 옆에 경보 단
습니다. 마당에도 경보 장치가 있는데 조그만 동물들에 의해 파헤쳐지지

경보 장치는 또한 화재나 연기 탐지기 및 스프링 쿨러 시스템에도 연결되어 있
니다. 경보 시스템 그 자체는 연중 계속 돌아가고 자체 발전기가 있으며 방화
치가 되어 있습니다.

창이

4

단주

않
6

ee
=)
장


===== PAGE 627 =====
626 ㅇㅇ ABS

예비 설계
이제 물어볼 차례입니다. “이 시뮬레이션은 어떤 문제에 대답을 하는가?” 예를 들
어, 시뮬레이션이 이런 질문에 답하면 됩니다. “감지기가 부서진지 얼마만에 사람
들이 알게 하나?” 혹은 “경찰에게 걸리지 않고 창문의 경보 장치를 제거하는 방
법은 없을까?”

JA] 시스템의 어떤 부분을 프로그램으

]니다. 일단 이해가 되면 프로그램을

무엇이 Wael it?
이 문제에 일단 접근하는 방법은 사용자 인터페이스 FES 일단 젖혀놓는 것이
고 단지 문제의 영역에 대해서만 초점을 맞추는 것입니다. 객체 지향 설계에
첫 접근은 여러분이 시뮬레이션하고자 하는 객체의 목록
체가 무엇을 알아야 하고 FAS 해야 하는지를 살펴보는 것입니다.
새로운 문제 AA(problem space) 문제들의 집합이고 여러분의 프로그램이 다루고자 하는
응어 주제입니다. 해결 YA(solution 50866)은 이 문제들에 대한 해결책의 집합입니다.

예를 들어, 분명히 여러분은 여러 종류의 감지기를 가지고 있습니다. 중앙 경보
장치, 경보 단추, 접촉 탐지 전선, 전화기 등입니다. 더 AAS 하게 되면 여러분
해

은 아마 방, 마루, 주인이나 경찰 같은 일련의 사람들에 대해서도 시뮬레이션8
봐야 합니다.

감지기는 일단 움직이는 것을 탐지하는 것과, 접촉 탐지 전선, 소리 탐지기, 연기
탐지기 등으로 나눌 수 있습니다. 이 모든 것이 탐지기의 일종인데 개별 탐지기
를 나누는 것은 의미가 크게 없습니다. 좋은

ee Be 망이기이너다

로서, 탐지기 클래스는 모든 SH] 탐지기와의 인터페이스를 제공하고 각각
의 파생형은 각각의 FAS 제공합니다. 다양한 감지기의 클라이언트들은 구체적
으로 어떤 감지기인지에 관계없이 사용하고 그 실제의 형에 의거하여 올바르게
작동합니다.

좋은 ADTS 만들기 위해 감지기가 무엇을 하는지에 대한(어떻게 하는지가 아니
oh 충분한 이해가 있어야 함니다. 예를 들어, 감지기는 누가 건드려야 올리는가
아니면 자기가 옴직이는 물체를 알아    지합니까? Fe AS 받아야 울리는가,

x 때


===== PAGE 628 =====
제18일 객체 지향 SAD 설계 ee 627

아니면 전선이 끊어져야 SAE}, 아니면 특정 부분이 녹아야 올립니까? 아마
어떤 감지기는 디지털 식이고(경보 상태이거나 아니면 비경보 상태) 어떤 것은
아날로그 식입니다.(현재의 온도는 몇 도이다.) 추상 자료형과의 인터페이스는 모
= 추상 클래스의 예상되는 요구들을 다룰 수 있도록 완벽해야 합니다.

다른 Was
AAS 계속됩니다. 각 사항에 부응할 수 있는 여러 클래스들을 검증해야 합니다.
예를 들어, 기록을 하려면 타이머가 있어야 합니다. 그러면 타이머가 각 감지기를
살펴볼 것인가 아니면 각 감지기가 자동적으로 보고서를 작성할 것입니까?

사용자는 감지기를 잠시 중지하고 SASS 설정해야 하며 따라서 특정의 옵션
설정용 단말 장치도 필요합니다. 경보 프로그램 그 자체를 위한 독립된 대상도
필요합니다.

클래스란 무엇인가?
이 문제를 풀기 위해 여러분의 클래스를 설계해야 합니다. qs 들어, 여러분은
이미 96050[의 파생 클래스로 HeatSensorS 만들었을지도 모릅니다. 감지기가 주기
적으로 보고를 하려면 1106@로부터 다중 상속을 통한 파생을 해야 할지도 모릅니
다. 혹은 자체의 멤버 변수로 타이머를 가져야 할지도 모릅니다.
열 감지기는 CurrentTemp()} 9601600114010를 멤버 함수로 가질 것이고 베이스
클래스인 96050『로부터 SoundAlam(°]Z@H= 함수를 상속할 것입니다.

객체 지향 설계에서의 주요 논점은 캡슬화입니다. 여러분은 경보 장치가
0001600를 설정할 수 있는 설계를 생각할 수 있습니다. 경보 시스템은 현재의
온도를 묻고 이를 최대 LES} 비교하여 너무 뜨겁다고 판단되면 경보를 울립니
다. 어떤 이는 이것이 캡슬화를 해친다고 말합니다. 즉, 경보 장치는 온도 분석의
자세한 사항을 알 필요가 없고 이는 86050090에 있으면 된다는 주장입니다.

여러분이 동조를 하건 말건 이것이 문제 분석을 하는 동안 내려야 할 결정의 하
나입니다. 이 BAS 계속하기 위해 단지 감지기와 기록 객체만이 어떻게 감지기
의 활동이 기록되는지를 알아야 하고 경보라는 객체는 알아서는 안된다고 주장을

룰 수 있어야 합니다.

좋은 캡슬화는 각 클래스가 응집성6000000을 가지면서 완전한 자기 담당성
(responsibilities)>] 의해 판단됩니다. 다른 클래스는 같은 담당성을 가져서는 안됨

re


===== PAGE 629 =====
HeatSensor7} ReportAlam() 함수를 가져야 합니까? 모든 감지기는 ABS 울릴 능
력이 필요할 AMYch. ReportAlarm()°] 56050의 가상 메쏘드가 되어야 하고
Sensor 추상 베이스 클래스이어야 한다는 것은 좋은 생각입니다. HeatSensor=
Sensor2] 좀더 일반적인 #6000418000 메쏘드에 연결되고, 중복된 함수가 자세한
부분을 채워 주어야 합니다.

경보는 어떻게 보고되는가?
여러분의 감지기가 경보 상태(2000000)를 알리면, 객체에게 많은 정보를 주어야
록을 합니다. 여러분은 0000000 클
여러 개의 측정치를 취합니다. 측
고

또는 간단한 정수값 정도를 가

qr 고 2 cfr 수
thlo
4)
1
xo,
uy

=>
poy
ex
af
ox,
고
때
1>
miu
a
mun
mu
을

때
ar
ro
aw
rs)

매우 잘 설계된 시스템은 중간의 조정 담당자를 가질 필요가 없습니다. 감지기는
모두 잘 독립적으로 메시지 객체를 주고받으며 매개 변수를 설정하고, 읽고, 집안
을 살펴봅니다. 잘못된 것이 있으면 경보 객체가 만들어지는데 문제를 기록하고
(기록 객체에게 문서를 전달하거나 해서) 적절한 행동을 취합니다.


===== PAGE 630 =====
제18일 객제 지향 SAD 설계 oe 629

사권 @2'=(Event Loop)
이와 BE 사건 위주의 시스템을 시뮬레이션하기 위해 여러분의 프로그램은 사건
환

순환문을 만들 필요가 있습니다.

이는 1\00160)과 같은 무한 순환인데 운영체제로부터 메시지를 받고(마우스나 키
보드로부터의 동작) 이를 하나씩 분기하여, 종료 상태가 될 때까지 순환문을 돕니

다. 예제를 봅시다.

[리스트 18.1] 간단한 사건 순환문

// CHAE 18.17 간단한 사건 순환문
#include <iostream.h>

1

2

3

[Ae

5: class Condition
6

7

8

{
public:
:    Condition() { }
9:    virtual ~“Condition() {}
10:   virtual void Log() = 0;
de ds
V2
13: class Normal : public Condition
148 £
128 public:

168   Normal() { Log(); }
176   virtual ~“Normal() {}
18%   virtual void Log() { cout << "Logging normal conditions...\n"; }

192 35

20:

21: class Error : public Condition
22: 31

25: public:

24:   Error(): {Log() 3}

25%   virtual “Error() {}

26:   virtual void Log() { cout << "Logging error! \n" =: 3
278 +9

28:

29: class Alarm : public Condition

308 €

31° public:

32!   Alarm ();

55%   virtual “~Alarm() {}

34:   virtual void Warn() { cout << "Warning!\n"; }


===== PAGE 631 =====
630 ee 제3주

352
36:
37:
38:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
D1:
525
a5:
54:
55.
56:
57%
58:
59:
60:
61:
62:
63:
64:
65:
66:
67:
68:
69:
10:
71:
(28
(35
74:
753
162
CC
78:
7193
80:

virtual void Log() { cout << "General Alarm log\n"; }
virtual void CallQ = 0;

3;

Alarm: :Alarm()

{
Log();
Warn();
}
class FireAlarm : public Alarm
{
public:
FireAlarm() {Log() 7};
virtual ~FireAlarm() (0
virtual void Call() { cout << "Calling Fire Dept.!\n"; }
virtual void Log() { cout << "Logging fire call.\n"; }
3;

int main()
{
int input;
int okay = 1;
Condition * pCondition;
while (okay)
{
cout << "(O)Quit (1)Normal (2)Fire: ";
Cin >> input;
okay = input;
switch (input)
{
case 0: break;
case 1:
pCondition = new Normal;
delete pCondition;
break;
case 2:
pCondition = new FireAlarm;
delete pCondition;
break;
default:
pCondition = new Error;
delete pCondition;
okay = 0;
break;



===== PAGE 632 =====
제18일 객체 지향 SAD 설계 oe 631

81:    +
82:     return 0;
S25 }

겔과  (O)Quit (1)Normal (2)Fire: 1

Logging normal condition...
(O)Quit (1)Normal (2)Fire: 2
General Alarm log

Warning!

Logging fire call.

(O)Quit (1)Normal (2)Fire: 0

AY SOBA 단순한 순환문이 만들어졌는데 정상 통지와 화재 통지를 받아
시뮬레이션하는 입력을 받습니다. 이 통지의 영향은 단지 상태 객체를 만드
는 것인데 그 생성자가 여러 멤버 함수를 부릅니다.

생성자로부터 가상멤버 함수를 호출하면 여러분이 객체에 대한 생성자의 순서를
미리 알고 있지 않은 경우에 혼동이 올 수 있습니다. 예를 들어, 72번 줄에서
FireAlarm 객체가 만들어지면 생성자의 순서는 Condition, Alarm, FireAlarm 순으로
호줄됩니다. Alam 생성자는 Logs 호출하면 비록 Ｌ080가 가상으로 선언되었다
해도 호출되는 것은 시400의 1080이지 『0641400의 Ｌ080가 아닙니다. 왜냐하면
Alam2] 생성자가 실행될 때 FireAlarme) 객체는 없기 때문입니다. 나중에
FireAlarme] 쟁성되면 그 생성자가 1080를 다시 호출합니다. 그리고 이번에는
FireAlarm::Log()7} 호출됩니다.

aa

땅

우편 AIAH(PostMaster)

객체 지향 EAS 해 볼 수 있는 또 다른 문제 하나를 풀어봅시다. 여러분이 이
제 막 「숲웨어'라는 소프트웨어 회사에 고용되었고, 거기서 새로운 소프트웨어 =
JES 시작하면서, 여러분의 프로그램을 구현하기 위해 몇몇 cH 프로그래머
용했다고 합시다. ㆍ신상품 Ws) 부사장인 '김버거'라는 사람이 여러분의
. 김버거는 여러분에게 새로운 우편 시스템을 설계하고 만들기를 원합
. 우편 시스템은 여러 개의 서로 관계가 없는 전자메일 제공자로부터 전자우
읽어들이는 유틸리티입니다. 잠재적인 DAS 하나 이상의 전자메일 - 나우
나 유니텔, 천리안, 하이텔의(이상 가나다 순) E-mail, Interchange, CompuServe,
Prodigy, America Online, Delphi, Internet Mail, Lotus Notes, AppleMail, CC:Mail 등
- 을 이용하는 직장인들입니다.

내
10

qr fst 드때 fu

f tle de ae s
ro
cH


===== PAGE 633 =====
632 ee 제3주

에 전화거는 법과 각 전자메일에 접속하는 WS 실행시킴니
지를 가져와서 그것을 단일한 양식으로 여러분에게 제공하
객은 편지를 재구성하거나 BIS 쓰고 혹은 내용을 더 추가하여 보

전 2탄이 이미 예상되고
12 사용자로 하여금 제
Ls 하는것 둥의 거능이 추가티었습

있습니다. 즉, 우편 시스템에 인
스템 및 동의어, 반의어

-ㅇ
rst
ma
1%
ot
6
tr
MY,
rr
do
st
ead
\y
oe
Se,
oN
Mt
a
2  x

jo 건
as
ri
2,
>

7) 기능까지 갖게 하는    ohne

또 다른 기능이 이야기되는데 여기에는 AUS 다루는 것뿐만 아니라 논쟁할 수
있는 토론 그룹의 기능이 그것입니다. CompuServeS] 1000088라든지 Internet 2]
Newsgroups 등입니다. '숲웨어' SAKE 우편 시스템에 상당한 기대를 갖고 있는
데 여러분은 철저한 스케줄에 쫓기고 있으며 대신 예산은 무한대로 쓸 수가 있
습니다.

생가은 여러 번, 결정은 한번에

여러분이 사무실과 사무 도구들을 정리하고 나서 처음 요구하는 것은 그 우편 시
스템에 대한 정확한 BIS 요구하는 것입니다. 시장을 분석한 후 여러분은 그
개발품이 GUS] 플랫폼에서 만들어져야겠다고 Ags 내렸고 그래서 DOS,
UNIX, 매킨토시, 윈도우 NT, 08/2 중 하나를 고르려고 합니다.

김버거와의 여러 차례에 걸친 힘든 회의를 하고 나서 ee 특정 플랫폼을 고

르기가 몸시 어렵다는 것을 알게 됩니다. 따라서 여러분은 개발품의 전방 부분 -

사용자 인터페이스 - 후방 부분 - 통신과 데이터베이스 - 8 분리하려고 합니다.

일을 빨리 진행시키기 위해 우선 DOS 버전을 먼저 만들고 Win32, Mac, UNIX,

05/2의 순으로 하려고 합니다. 이 간단할 결정은 여러분의 프로젝트에 엄청난 결
터페이스를
H

°

과를 가져오는데, 즉 여러분은 메모     관리하고, 다양한 사용자 인터페이스
가지고 SAL 데이터베이스를 다루는 클래스 라이브러리 함수 또는 일반의 라이
브러리 함수들을 필요로 하게 됩니다.

Ab

we  사람인데, 따라서 그는 여러분에게 다른 ens meee
AAS 할 것을 요구하였습니다. 이제 분석하기 시작합시다.

ee =
Le
ts
ne,



===== PAGE 634 =====
제18일 객제 지향 분석과 설계 ee 633

분열시킨 뒤 정복하라
풀어야 할 문제가 한 둘이 아니라는 것은 뻔한 일입니다. 프로젝트를 다음의 하
부 프로젝트로 분리합니다.
Lei: SAS 통한 전자메일 제공자에게 ASAE 기능, 혹은 YEO 연결하는 기능
2 데이터베이스 : 자료를 저장하고 디스크로부터 검색하는 기능

3 전자메일 : 다양한 규격의 전자메일을 읽고 이를 각 다른 시스템에 새로이 작성하는 방법

Or.

4 편집 : 편지를 만들고 다룰 + 있는 품질 좋은 에디터 제작

$ 플랫폼 : 다양한 플랫폼(005, 매킨토시 등)에서 제공되는 다양한 사용자 인터페이스

6 확장성 : 성능 향상을 위한 계획

7. 조직과 스케줄링 : 여러 개발자들을 관리하고 각 코드를 결합시킴니다. 각 그룹은 시간
계획을 작성하고 그에 따라 적절히 움직입니다. 부관리자와 판매자들은 언제 이 제품이
나올 것인지를 알고 있어야 합니다.

여러분은 이 개의 부분을 다루고 조직하고 시간 계획을 작성할 중간 관리자를
고용합니다. 또 분석과 설계를 하고 또 다른 나머지 부분을 다룰 중간 개발자를

고용합니다. 이 중간 개발자는 다음의 팀을 만듭니다.

Leva : 전화 걸기, oEY SAS 담당. 패킷과 스트림, 비트들을 다룹니다.

2 메시지 규격화 팀 : 일반 전자메일 제공자의 규격에서 우편 시스템의 표준 규격으로 전
환 및 반대의 과정을 담당하는 팀.

3 메시지 편집 : 이 GE 각 플랫폼의 산출물에 대한 전체적인 사용자 인터페이스를 담당
합니다. 전방 부분과 후방 부분 사이의 인터페이스를 효율적으로 시키고 2} 플랫폼간의
이식시 코드 중복을 없애는 것이 이들의 책임입니다.

메시지 규려화

통신과 사용자 인터페이스는 뒤로 미루고 메시지 규격에 먼저 초점
합니다. 먼저 무엇을 해야하는지 충분히 이해해야 합니다. 여러분이
는 정보가 무엇인지를 이해하기 전까지는 정보를 어떻게 출력할 것인 기. 또는 ar
격화하여 출력하는 것이 가능한지에 대한 걱정이 있기도 합니다.

그런데 여러 메일 메시지 제공 회사의 규격을 살펴본 결과 EH 많다는 것을
알게 됩니다. 각각 발신인, 수신인, 작성 일자가 있습니다. 대부분 제목과 부제가
있으며 본문이 있는데 본문 부분은 간단한 텍스트로 구성이 되는 부분과 규격화
된 텍스트, 또는 그래픽, 심지어 음성 등등의 본문 부분이 있습니다. 각각의 메일

 alo
rs
x
ON,


===== PAGE 635 =====
634 ee 제3주

첨부 기능이 있어 일반 텍스트 다음에 프로그램 코드라든가 또는 다른 파일을
첨부하여 보낼 수 있습니다.

여러분은 각 메시지를 하나의 표준 형태로 규격화하는 것이 가능하다는 것을 알
게 됩니다. 하나의 레코드 규격으로 저장하고 디스크로부터 입출력하면 됩니다.
또한 헤더 부분(발신자, 수신자, 날짜, 제목 등) 몸체 부분과 ac 때때로

my   i

사용자들은 편지 제목만 보고 BES 안 볼 수도 있습니다. 또 BES HFA! al
더부분만 다운로드받는 경우도 있습니다. 하지만 1차 버전에서는 비록 BES A
용자에게 보여주지 않더라고 일단 전체 편지를 디스크에서 다 가져오는 것으로

합니다.

조기 클래스 설계

우편 시스템의 메시지를 분석한 결과 Message 클래스가 필요하다는 것을 =A
됩니다. 이 프로그램을 비메일의 메시지로 확장할 것을 고려하여 여러분
1685886라는 추상 베이스로부터 EmailMessageS 파생시킴니다. 0 _
터 PostMasterMessage, InterchangeMessage, CISMessage, ProdigyMessage’s-& 파생시
킴니다.

메일 메시지를 다루는 프로그램에서 Message: 적절한 객체가 되지만 복잡한 시
스템에서 필요한 모든 객체를 찾아낸다는 것이 사실 객체 지향 프로그래밍의 가
장 큰 문제이기도 합니다. 때때로 기본적으로 만들어 놓은 객체가 문제를 해결하
ea Heise 합니다. 사실 적절한 ANE 찾는 과정이 매우 어럽고 긴 시간

을 요구할 수 있는 경우가 대부분입니다.

3무 걱정하지 Yc. 대부분의 설계자들이 처음부터 잘하는 것이 절대 아님니
aide 좋게 하려면 문제점을 과장되게 서술합니다. 프로젝트를 기술할 때
든 명사 부분과 동사를 그대로 다 나열합니다. 명사 부분은 객체를 만드는 좋

재료 감임니다 동사 부분은 이 객체에 대한 대쏘드가 되고 혹은 개체가 될
수도 있습니다. 이렇게 무조건 다 적어놓는 것은 잘못된 것이 있다해도 좋은 출
발을 하고 있다는 증거가 됩니다.

 3 Al 지원 쉬워집니다. 여기서 질문이 발생합니다. “메시지의 헤더 부분의 클래
부분과 분리되어야 합니까?” 이렇게 한다면 여러분은 평행한 계층 구
가져 야 합니다. 예를 들어, CompuServeBody?} CompuServeHeaderS 가져야
분도 다 이렇게 나뉘어야 합니다.

 년

au
ofa

oh [>
a ae

aN
:



===== PAGE 636 =====
세18일 객체 지향 SAT 설계 eo 635

평행한 계층 구조는 잘못된 설계라는 경고로 알면 됩니다. 하나의 Aso] 일련의
객체를 평행하게 갖는 것과 이 객체들이 짝지어지는 일련의 부분들을 갖는 것은
객체 지향에 있어 오류가 되기 십상입니다. 이들을 항상 같이 유지 보수하고 동
기화시키는 것은 부하가 FUG. 이른바 고전적인 유지 보수 방법이 됩니다.

사실 왕도는 없습니다. 따라서 이렇게 평행한 계층 구조를 갖는 것이 특정 문제
를 푸는데 효율적이 될 수도 있긴 합니다. 그렇지만 ine 식으로 설계가 진행된
다면 다시 고려해 볼 필요가 있습니다. 다른 해결책이 있을 것입니다.

것
이제까지 BAS] 전자메일 제공자로부터의 메시지를 몸체와 헤더로 분리할 필
요는 없습니다. 많은 자료들이 뒤엉킬 수 있고 이는 여러분의 계층 구조에 그대
로 적나라하게 나타납니다.

이 과업을 잠깐만 더 생각해 봐도 각 메시지의 특성을 모두 나열하는 것은 기능
과 자료 저장의 적절한 추상 수준을 정하는데도 필요합니다 각 객제의 Hae
나열하는 것은 자료 Ws 찾고 다른 객체와의 주고받는 부분들을 그리는 과정
에서도 좋은 안내가 됩니다.

me 메시지는 AA 필요가 있습니다. 사용자의 전화번호나 취미 사항 등도 그
습니다. 저장 기능이 계층상에 나타나야 합니다. 메일 메시지가 반드시 베이스
ean 포함되어야 하는지?

순종 7lF(Rooted Hierarchies) it 잡종 A=
(Non—Rooted Hierarchies)

ASE 상속하는 방법에는 크게 보아 두 가지로 나닙니다. 하나의 BES 근본
(Root) 클래스를 가지고 계속 상속받는 방식과, 또 다른 SUE 한 개 이상의 계
충으로부터 aertte 경우입니다. 단일의 클래스 AS 상속 방식의 이점은 다중

상속을 피할 수 있다는 것이고 불리한 AL 수많은 구현물들이 베이스 클래스에
끼여든다는 것이다
새로운 FY 클래스들이 공통 조상(0011101 ancestor)S 공유하는 경우 순종이라고 하고, 잡종
SO 계증이란 공통의 베이스 클래스를 공유하지 않는 경우를 말합니다

여러분의 생산물은 많은 플랫폼에서 개발될 것이고, 또 다중 상속은 복잡한데다
모든 플랫폼에서 지원된다고 보 = 수 없으므로, 여러분이 결정할 첫 번째는 순
종 계충과 단일 상속을 갖도록 하는 것입니다. 하지만 나중에 다중 상속이 필요
할 경우가 발생할지도 모르므로 다중 상속을 만들 자리를 미리 상술하고 또 다중


===== PAGE 637 =====
636 ee 제3주

aeons E7189 대한 AAS 미리 고려를 하여 나중에 전체 설계를 망치지

모든 수군    클래스는 로 시작하게 하여 어떤 클래스가 여러분이 만든
것이 라이브러리에서 온 것인지를 쉽게 구별하게 합니다. 21일째에

Seis ia 개넘을 구현할 이름 YA(name space)ol] 대해 배우는데 당분간은

그냥 진도를 나갑시다.

순종 클래스000! 0059)는 200060라 합니다. 여러분이 만드는 모든 클

로부터 내려갑니다. pObject: 상대적으로 단순하게 합니다. 모든 항

나는 자료들만 공유합니다.

°

이 AS 구조의 꼭대기에 올 수 WE ASS pStoredt} pWired7} 될 수 aie
pStored 객체는 여러 경우에 디스크에 저장되는 객체입니다. | pWired 객체는
go] yEdo 전달되는 객체입니다. 여러분의 모든 객체는 디스크에 저장된
필요가 있으므로 이 SS AS] 꼭대기에 올려보낼 필요가 있고 또 모든 BW
으로 보내는 모든 객체는 저장이 되어야 하지만 모든 저장된 객체가 모두 BO
로 가는 AS 아니므로 2\160를 0510760로부터 파생하는 것은 의미가 있습니다.
각각의 파생 클래스는 그 베이스 클래스로부터 정보(자료)와 기능(메쏘드)을 가지
며 추가하여 다른 기능들을 갖습니다. 2\100는 다양한 메쏘드를 갖는데 이들은
모두 Bas 연관되는 기능입니다.

BE Eq 전송 sin 저장이 되어야 하거나 혹은 저장된 객체는 모두 ASS
수 있어야 하거나 혹은 이 두 개의 문장이 다 틀릴 수 있습니다. 단지 몇몇의 전
송되는 객체만 저장되고. 그리고 저장되는 객체 중 몇몇만 전송되면 다중 상속을
사용해야만 하거나 혹은 문제점 주위를 빈둥거리며 다녀야 합니다. 이러한 잠재
적인 몸쓸 기능은 상속될 수 있는데, AS 들어 저장 객체로부터 전송 객체가 나
오고 전송된 자료가 저장은 안되고 저장하는 메쏘드가 아무 것도 하지 않거나 오
류를 발생시킬 수 있습니다

분명히 저장되는 객체 전
은 사항입니다. 전송 io
[그림 18.1]과 같습니다.

dese 것은 아닙니다. AE 들면, 사용자의 취미
저장이 됩니다. 따라서 여러분의 계층 구

도  쿠


===== PAGE 638 =====
제18일 객제 지향 분석과 설계 ㅇㅇ 637

[그림 18.1]
초기의 AF 구조                             pObject

pStored

pWired                                               pPreferences    |                                  pProvider Info |

pMessage

인터페이스 설계

이 설계의 단계에 있어 중요한 것은 나중의 구현 부분과 연관지어서 생각하면 안
된다는 것이 아주 중요합니다. 여러분의 BE 정열을 클래스간의 깨끗한 인터페
이스의 설계에 맞추고 어떤 자료와 메쏘드가 필요한 것인지 그림을 그리는데 초
점을 맞춤시다.

각각의 파생 클래스를 만들기 전에 베이스 클래스에 대한 정형화된 이해를 가지
는 것이 필요합니다. 따라서 일단 pObject, pStored, pWiredo] 초점을 맞춤시다.

순종 클래스(600600는 단지 여러분의 시스템에서 모두 공통되는 자료와 메쏘드
를 가져야만 합니다. 모든 객체는 가령 단일의 인식 번호를 가질 수 있습니다. 이
런 경우 pIDS 만들고 이를 2040000의 멤버로 합니다. 그전에 ALS 해야 합니
다. “저장되지 않고 전송되지 않는 객체도 이 HSS 가져야 합니까?” 또 다음 질
문이 나옵니다. “저장은 되지 않지만 이 계층 구조에 일부분인 객체가 있습니까?”
당분간 분리된 pObjectS 가정하는 것이 좋을지도 모릅니다. 여러분은 pAddress
객체의 모임체인  bate 생각할 수 있고 niger 자신을 저장은 못하지만
각각이    한 인식    Pik  갖게 하는 도구가 있을 수 있습니다. pIDS pObjecto}

oO

Of"

O°

:
at

일단은 다음 형태를 가진다는 AS 의미합니다.

class pObject

+

public:
pObject();
“pObject();


===== PAGE 639 =====
638 ce 제주

010 GetID() const;
void SetID(Q);
private:
pID itsID;
}

이 클래스의 선언에서 살펴볼 것이 많습니다. 먼저 이 클래스는 어디에서 파
것이 아닙니다. 이것은 순종 클래        동

니다. 06000) 같은 메쏘드에서 조차도(실제 필요한데) 없

셋째 const WET} 상술되어 있습니다. 구현이 아니라 인터페이스의 부분입니다.
마지막으로 000라는 새로운 Bo] 포함되었습니다. pIDS unsigned 1008등으로 A}
용하지 않고 새로운 Yow 하여 여러분의 설계에 융통성을 더해주었습니다.

unsigned longo] 불필요하거나 HEX unsigned 1008만으로 크기가 모자라 더 늘
때 202만 수정하면 됩니다. 이 FAS 단지 pID7} 사용되는 곳에만 영향을 미
니다. 프로그램의 모든 부분을 쫓아다닐 필요가 없습니다.

분간 typedefS 사용하여 pIDS 01.0440로 사용하는데 01.0씨06는 40518060 long
로 합시다. 그런데 이 선언은 어디에서 합니까?

ES 프로그래밍할 때 각 파일에 대한 전반적인 기준이 필요합니다. 이
로젝트 수행시 여러분이 지켜야 할 표준 접근 WAS, 각 클래스는 헤더 파일
에 나타나야 하고 그 구현 BRS 해당 파일에 cCPPH 확장한 파일에 있어야 합
. 따라서 여러분은 OBJECT.HPPS} OBJECT.CPPS 가져야 합니다. pMessageS
하고 구현할 때 MSG.HPPS} MSG.CPPS 각각 가져야 합니다.

m at 4s

|o off

도
ro 도

^

구입을 할 것인가 록은 작성을 할 것인가? 프로그램 설계 단계에서 나타나는 문제는
어느 부분을 구입하고 어느 SBS 여러분이 직접 작성할 껏이냐 입니다. 이미 존재하
는 상용화된 라이브러리 함수를 구입하여 문제들을 HAL 수 있습니다. 하지만 가격
과 비기술적인 부분들이 고려되어야 합니다

상용 라이브러리 함수를 구입하는 것은 이점이 많습니다. 그떼 여러분은 특정 프로그
램에 정열을 쏟을 수 있고 부자적인 HS 구입을 통해 래결을 합니다. (++을 사용
하는데 직접 필요하지 않은 라이브러리 함수들을 구입할 수도 있는메 이런 것이 기본
적인 기능성을 가지고 여러분에게 도움을 준다면 여러분이 제시간에 업무를 완료하는

그
In
Ho
pa
it
>코
re
FE
pa


===== PAGE 640 =====
제18일 객제 지향 분석과 설계 ee 639

원형 2   9 8 90308탠은

하는 것은 잘못입니다. 어긋난 문제로 인해 곤란을 겪을 수 수 있는 . 프로그램의
HES 작성하기 전 모든 클래스를 만들고 그들 간의 인터페이스를 끝내놓는 것
은 ASS 향한 첫걸음이 됩니다

원형을 만들어 보려는 여러 가지 이유가 있습니다. 여러분 생각의 핵심을 빠르게
그리고 대충 만들어 보는 것입니다. 여러 종류의 다른 원형들이 각각의 필요에
따라 사용될 수 있습니다.

인터페이스에 대한 설계 원형물은 잠재적인 사용자들과 함께 여러분의 산출물의
외양과 느낌을 검사할 기회를 줍니다.

기능에 대한 원형물은 최종적인 사용자 인터페이스를 가지지는 않지만 사용자로
하여금 여러 Ee  기능 실험을 하게 해줍니다. 예를 들면, 메시지에 응답하거나
파일을 첨부시켜 전송해 보는 등입니다.

마지막으로 구조에 대한 원형물은 조그만 프로그램 Was 개발할 기회를 주고

얼마나 쉽게 그 ee   a 수 있는7 He a   [기 위해 설계됩니다.
원형의 목적을 분명히 해야 합니다. 사용자 인터페이스를 살펴보았는가? 기능성
이 충분히 Bese! 최종 Ube EME SHS 구성하였는가! 구조이

대한 원형물은 잘 만들었는데 인터페이스에 대한 MISS 형편없지 않은가 sq

고

80/80의 법칙
Gol 있어 좋은 설계의 원칙이 있습니다. 80%의 사람들이 808의 시간을 투
여해 만들고 싶은 PRS 설계하고 나머지 20% FRE 선경 쓰지 말라는 것입니
. 주변적인 부분들은 조만간 요구되겠지만, 일단 여러분 설계의 Be 80/80에

여

=                                      스

때, 세련 되지 anda 하나의 대표적인   ae 선택하여 거기에 초점을 맞추
고 비슷한 것들의 설계와 구현은 나중으로 미룹니다.


===== PAGE 641 =====
640 ec A3%

또 다른 법칙이 있습니다. 90/20 법칙입니다. 프로그램의 처음 20%를 PEE 전체의
80% 시간이 소비되어 나머지 80%의 프로그램에 또 80%의 시간이 소비됩니다.

PostMasterMessage 클래스 설계

이러한 것들을 염두에 FAA) PostMasterMessagel] 몰두하기로 합시다. 이 클래스

가 가장 여러분의 직접 통제하에 있는 클래스입니다.

인터페이스 부분에 있어서 PostMasterMessaget= 다른 메시지형들과 같이 이야기될
필요가 있을 것입니다. 여러분은 다른 메시지 제공자와 그 메시지의 규격 상술서
를 얻기 위해 긴밀하게 일할 수 있어야 합니다. 하지만 당분간은 그들의 서비스를
이용할 때 여러분에게 오는 AS 보고 대략 추측하여 사용하기로 합니다.

어떤 경우든 WE PostMasterMessage= 편지 전송인과 수령인, 날짜와 제목, 그리
고 본문과 첨부 파일(없는 경우도 많지만)이 있을 것입니다. 따라서 각각에 접근
하기 위한 접근 메쏘드가 필요하고 첨부 파일 및 메시지의 크기를 보고할 메쏘드
도 필요합니다.

어떤 서비스는 각 폰트에 명령 기호,
정하는 규격 명령어를 가진 텍스트일

없는 ALE 있습니다. 여러분의 클래스에서는 ㅇ
스트로 변환하는 변환 메쏘드를 가질 수 있어야 하고 혹은 5S] PostMaster at
격으로 바꿀 수 있어야 합니다.

기, 속성(볼드체 혹은 이탤럭체) SS 설
ZE        2H

a
et
ty
Sou,
jin Ad
Jf
0
\m
fur
ne
=
ayy

응응 프로그램 인터페이스

응용 프로그램 인터페이스(60]는 서비스를 사용하는 일련의 안내서와 과정의 A
합입니다. 많은 메일 제공자들이 여러분에게 APIS 제공하는데 따라서 206044096『
메일은 각 메일의 고급 기능(규격화된 메일 HS 사용할 수 있습니다. 2050448566[
도 역시 자신의 APIS 출판해야 다른 제공자들도 미래에 206004896와 같이 일할
계획을 세울 수 있습니다.

여러분의 PostMasterMessage 클래스는 잘 설계된 범용 인터페이스를 가져야 하고
PostMaster2} APIS] BAe . 변환함수가 SB 것입니다. [리스트  18.2]는
PostMasterMessage®] 인터페이스가 이런 식으로 된다는 aS 보여줍니다.


===== PAGE 642 =====
제18일 객체 지향 SAT 설계 ㅎㅎ 641

[리스트 18.2] PostMasterMessageQ] 인터페이스
1: class PostMasterMessage : public MailMessage
20

3: public:

43    PostMasterMessage();

5:    PostMasterMessage(

6:    pAddress Sender,

ts    pAddress Recipient,

8:    pString Subject,

9:    pDate creationDate);

102

Ve   // 생성자들

12:  // 복사 생성자 포함에 유의

Key   Lf

14: // 다양한 규격들의 생성자 지님

155   //

16:   “PostMasterMessage();

It:   pAddress& GetSender() const;

18:   void SetSender(pAddress&) ;

19: // 다른 멤버 접근자

205

21    // 연산자 메쏘드

22: // PostMaster 메시지를 다른 규격으로
23%   // 바꿈

24:

25: private:

26:   pAddress itsSender;

27:   pAddress itsRecipient;

28:   pString itsSubject;

29:   pDate itsCreationDate;

508   pDate itsLastModDate;

313   pDate itsReceiptDate;

52:   pDate itsFirstReadDate;

55%   pDate itsLastReadDate;

S42 32

Ah 3:
분석 PostMasterMessage 클래스는 MailMessage@ 425] 파생됩니다. 많은 생성자

기능을 가집니다.

이 제공되고 다른 메일 메시지의 형으로부터 PostMasterMessage= 생성하는


===== PAGE 643 =====
642

많은 접근 메쏘드가 다양한 자료 및 하나의 메시지를 다른 메시지로 변환하는 a

산자들을 War 설정하는 역할을 할 것입니다. 이 메시지들을 디스크에 정렬하고,
통신 회선으로부터 읽으며 따라서 접근자 메쏘드가 이 목적에 적합하게 사용되어
야 합니다.

대 그룹에서의 프로그래밍

이 예비 구조만으로도 어떻게 여러 개발 그룹들이 작업을 진행할지를 잘 나타냄
니다. 통신 그룹은 통신 후방 부분에서 메시지 규격화 그룹과 상호 이야기하면서
작업을 진행할 수 있습니다.

메시지 규격화 그룹은 Message 클래스와 의사 ASS 통해 자료들을 디스크에 OF
떻게 입출력해야 할 지에 전력 투구할 수 있습니다. 이 디스크와의 인터페이스가
잘 설정이 되면 통신 계충과의 인터페이스를 만들 수 있습니다.

메시지 편집 그룹은 Message 클래스에 대한 자세한 정보를 가지고 메시지 편집기
를 만들고 싶은 유혹에 빠지지만 이는 아주 나쁜 설계 오류입니다. 메시지 편집
그룹은 사실 메시지의 내부 구조에 대해 아주 조금만 알 따름이죠.

설계에서 기타 고려 사항들

프로젝트가 계속 진행되면서 여러분은 계속적으로 기본 설계에서 Poad 사항
들을 만나게 될 것입니다. 어떤 클래스에 일련의 기능성(혹은 자료들)을 넣을 것
인가? 메시지 클래스가 이 기능을 가져야 하는가 아니면 주소 클래스가 이 기능
을 가져야 하는가? 에디터가 이 정보를 가져야 하는가 아니면 메시지가 가져야
하는가?

여러분의 클래스는 od 필요가 있다'라고 하는 기본 전제에서 판단해야 합니다.
실제 필요한 이상의 자료를 가지면 안됩니다.

설계시 판단

프로그램을 진행하면서 많은 설계상의 이슈를 접하게 됩니다. 각각은 다양한 범
위의 좀더 전역적인 질문들을 가지고 있습니다. “이것은 무엇을 하게 할 것인
가“, “이것이 어떤 작용을 하게 할 것인가



===== PAGE 644 =====
제18일 객체 지향 분석과 설계 ce 643

러분의 구현은 끝나지 않게 됩니다. 계속 작업을 함에

것인데 여러분은 여러분의 설계를
가져야 합니다. 코드에 들어가기 전 여러분이 하고자
야               중간

하는 것을 확실히 알고  합니다. 소프트웨어가 중간에 죽어버리는 가장 큰
이유는 무엇이 만들어질 것인가에 대하여 사전에 충분한 합의가 없었다는 ag
니다.

판단, 판단
설계 과정이 어떤가를 알기 위해 이 질문을 봅시다. “메뉴 위에 무엇이 있습니
까?” 우편 시스템에서는 처음의 선택 사항은 “새로운 메일 메시지”일 것입니다.
이는 즉각 다른 설계 ARS 불러일으킬 것입니다. 사용자가 New 14685886를 선택
했을 때 무엇이 일어날 것입니까? 편집기를 미려:  만들어준 다음 메일 메시지를
보여줄 것인가 아니면 새로운 메일 메시지를 만든 다음 편집기를 만들 것입니까?

여러분이 만든 명령어는 “새로운 메일 메시지“이므로 새로운 메일 메시지를 먼저
만든 다음, 다음 일을 하는 것이 올바른 순서일 것입니다. 그런데 사용자가 메시
지를 작성한 다음 CANCELS 선택하면 어떤 결과가 날 것입니까? 이런 땐 먼저
편집기를 만들고 편집기가 새로운 메시지를 만들게 하는 것이 맞을 것입니다.
이러한 접근 방식의 문제점은 메시지를 만드는 것하고 메시지를 Base 것하고
편집기가 각기 다른게 동작해야 한다는 것인데, 메시지가 먼저 만들어지면 다음
에 편집기에게 넘겨주는 것으로 되고 이때까지는 일련의 코드가 필요합니다. 다
음부터는 이미 존재하는 메시지를 편집하는 것입니다.

내  만들어지려면 누가 만듭니까? 메뉴의 명령어 코드가 만듭니까? 그렇다
면 메뉴가 메시지에게 그 자신을 편집하라고 합니까? 그러면 이는 메시지의 생성
자 메쏘드의 영역이 될 것입니다.

메시지의 생성자가 이 ail 하게 하는 것이 언뜻 보았을 때 맞는 A 같습니다.
메시지를 만들 때마다 편집을 원할 것입니다. 그럼에도 불구하고 이는 좋은 개념
이 아닙니다. 먼저 전제7 | 틀릴 수 있습니다. 여러분은 조그만 메시지(운영자에게

오류 사항을 적는 메시지)를 만들어 보낼 수 있는데 이는 편집기 안에 들어가지
않습니다. BAS 더 중요한 문제인데 생성자의 역할은 객체를 만드는 것이지 그
이상이나 그 이하가 되어서는 안됩니다. 메일 메시지가 만들어지면 생성자의 일
이 끝납니다. 편집기의 역할을 생성자에 넣으면 생성자의 역할에 혼동이 오고 메
일 메시지가 편집기에서 실패하기 쉽게 만듭니다.


===== PAGE 645 =====
644

66 제3주

모
로

>보
rlo

편집기 메쏘드가 다른 클래스, 즉 편집기를 호출하고 여기서 또 생

성자가 호출됩니다. 편집기는 메시지에 대한 베이스 클래스가 아니고 메시지 안
에 있는 것도 아닙니다. 메시지의 생성자가 편집기의 생성자에 의존한다는 것은
좋지 않습니다.

마지막으로 메시지가 성공적으로 만들어지지 않으면 편집기를 호출하고 싶지 않
을 것입니다. 그럼에도 불구하고 성공적으로 만들어지는 것이 시나리오에 잡혀
있고 편집기를 호출하는 것에 의존하게 됩니다. 여러분은 51695886::8010를 호출하

%                               ]니다.

. 여러
기 전 메시지의 생성자로부터 빠져나가고 싶을 것입

00 설계를 통해 자연히 나오는 객체를 주시합시다

DO 문제 영역에 대한 인식이 확산될수록 재설계하는 것을 주저하지 Mt.
DON'T 필요한 것 이외의 정보들을 클래스 사이에 공유하지 많시다

00 ++의 다령성의 이점을 활용합시다

구동 프로그램(매106 Program)S 가지고 작업

응어

설계 사항의 ASS AYRE 데에는 작업의 초기 부분에서 구동 프로그램을 만
들어 보는 것도 하나의 방법일 것입니다. 예를 들어, 우편 시스템의 구동 프로그
램은 일단 몇 개의 간단한 메뉴를 보여주는 데에서 시작할 수 있습니다. 먼저
PostMasterMessageS 만들고 연산하고 몇몇 설계 사항을 실행해 봅니다.

새로운 구동 프로그램 구동 프로그램은 다른 함수들을 한 번 보여주고 Wr] 위해 존재
니

— 느    A
하는  함수입

[리스트 18.3] PostMasterMessage®] 정의에 대한 좋은 예제이고 간단한 구동 =
로그램을 보여줍니다.

[리스트 18.3] PostMasterMessageOl 대한 구동 프로그램

#include <iostream.h>
#include <string.h>

typedef unsigned long pDate;
enum SERVICE

나 6 Er =


===== PAGE 646 =====
제18일 객체 지향 SAD 설계 oe 645

6:    { PostMaster, Interchange, CompuServe, Prodigy, AOL, Internet };
7: class String
8:

{
9: public:
10:  // 생성자 및 소멸자
11   String();
1020   String(const char *const);
Ws:   String(const String &);
14:   “String;
15:

16:    // 재생 연산자
10s   char & operator[](int offset);

18:   char operatorLl](int offset) const;

19:   String operator+(const String&);

20:   void operatort=(const String&);

Z21¢   String & operator= (const String &);

22:   friend ostream& operator<<

253     ( ostream& theStream,String& theString);
24:   // 일반 접근자

25:   int GetLen()const { return itsLen; }

26:   const char * GetString() const { return itsString; }
2s   // static int ConstructorCount;

28: private:

29: String (int); // 전용 생성자

50:   char * itsString;

512   unsigned short itsLen;

52:

5355 33

34:

35: // 2 생성자

36: String::String()

S57: <

38:   itsString = new charl1];
39:   itsStringlO] = '\O';

40:   itsLen=0;

41:   // cout << "\tDefault string constructor\n";
42%   // ConstructorCount++;

43: 3

44:

453 //

46: // 전용 생성자

AC: 17

48: String::String(int len)

49: ¢

50:   itsString = new charLlen+t1];

a1.    for (int i = 0; i<=len; i++)


===== PAGE 647 =====
646 ce

제3주

528
55:
54:
55:
56:
DT:
58:
59:
60:
61:
62%
65%
64:
65:3
66:
67:
68:
69:
(02
71:
(2:
(33
(4:
OE
168
77:
(8:
79:
80:
81:
82:
85:
84:
853
86:
87:
88:
89%
90:
OT:
92:
95:
94:
95%
96:
97:

itsString£1] = "\0";
itsLen=Len;
// cout << "\tString(int) constructor\n";
// ConstructorCounttt;
자

// 문자 배열을 문자열로 바꿈
String::String(const char * const cString)
{

itsLen = strlen(cString);

itsString = new char(itsLent1];
for (int i = 0; i<itsLen; i++)
itsStringLil = cStringlil;
itsStringLitsLenJ='\0';
// cout << "\tString(char*) constructor\n";
// ConstructorCounttt;
}
// Set

String::String (const String & rhs)
{
itsLen=rhs.GetLenQ;
itsString = new charLitsLent1];
for (int i = 0; i<itsLen;it+)
itsStringli] = rhslil;
itsStringLitsLen] = '\0';

// cout << "\tString(String&) constructor\n";

// ConstructorCounttt;

// 소멸자
String::~String ()
{
delete [J itsString;
itsLen = 0;
// cout << "\tString destructor\n";

// 데일 연신작
HE:
String& String::operator=(const String & rhs)
{

if (this == &rhs)

return *this;
delete [] itsString;
itsLen=rhs.GetLen();



===== PAGE 648 =====
제18일 객체 지향 분석과 설계 ㅇㅇ 647

98:
99:

100:
101:
102:
103:
104:
105:
106:
107:
108:
109:
1102
1111
1128
113
1148
115:
116:
117
118:
119:
120:
1217
122:
123%
124:
125%
126:
127%
128:
129%
130:
T3 12
1328
135:
134:
135:
136:
1375
138:
139:
140:
141:
142:
143:

itsString = new charLitsLent1];

for (int i = 0; i<itsLen;it+)
itsStringlil = rhsLlil;

itsStringLitsLen] = '\0';

return *this;

// cout << "\tString operator=\n";

}

//

//' 비상수 변위 연산작

//

char & String::operatorLl](int offset)
{

if (offset > itsLen)

return itsStringLlitsLen-1];
else

return itsStringloffsetl;

}

// 상수 변위 연산자

//

char String::operatorL](int offset) const
{

if (offset > itsLen)

return itsStringLitsLen-1];
else

return itsStringlLoffset];

// 새로운 문작열 생성
//
String String::operator+(const String& rhs)
{
int totalLen = itsLen + rhs.GetLen();
String temp(totalLen);
for (int 1 = 0; i<itsLen; i++)
tempCil = itsStringLlil;
for (int j = 0; j<rhs.GetLen(); j++, i++)
tempCil = rhsljl;
tempCtotalLenlJ='\0';
return temp;
}

// eh Bs
void String::operator+=(const String& rhs)
{


===== PAGE 649 =====
648 ec 제3주

144:   unsigned short rhsLen = rhs.GetLen();

145:   unsigned short totalLen = itsLen + rhsLen;
146:   String temp(totalLen);

147:   for (int 1 = 0; i<itsLen; i++)

148:      1600613 = itsStringlil;

149:   for (int j = 0; j<rhs.GetLen(); j++, i++)
150:      tempLil] = rhsLi-itsLen];

151:   tempLtotalLenJ='\0';

152%   *this = temp;

1548 개

154:

155: // int String::ConstructorCount = 0;

156:

157: ostream& operator<<( ostream& theStream,String& theString)
1582 <

159%   theStream << theString.GetString();

160:   return theStream;

1615 ¥

162:

163: class pAddress

164: {

165: public:

166:   pAddress(SERVICE theService,

167:   const String& theAddress,

168:   const String& theDisplay):

169:   itsService(theService),

170:   itsAddressString(theAddress),

1712   itsDisplayString(theDisplay)

(fe:   {}

174,   // pAddress(String, String);

174:   // pAddress();

1758   // pAddress (const pAddress&);

176:   “pAddress(){}

177: friend ostream& operator<<( ostream& theStream, pAddress& theAddress) ;
178:   String& GetDisplayString() { return itsDisplayString; }
179: private:

180:   SERVICE itsService;

181:   String itsAddressString;

182:   String itsDisplayString;

Too. 17;

184:

185: ostream& operator<<( ostream& theStream, pAddress& theAddress)
186: {

187:   theStream << theAddress.GetDisplayString();
188:   return theStream;

189: }


===== PAGE 650 =====
A182 객제 지향 SAD 설계 ㅎㅎ 649

190:
191:
192:
193;
194:
195:
196:
1971
198:
199:
200:
201:
202:
203:
204:
205=
- 206:
207:
208:
209:
210:
211:
212:
213:
214:
215:
2168
2173
218:
2198
220:
2c:
222:
225:
224:
225%
226:
2278
228:
229:
230:
2505
232:
2335
234:
2355:

class PostMassage
{
public:
// PostMasterMessage();

PostMasterMessage(const pAddress& Sender,
const pAddress& Recipient,
const String& Subjcet,
const pDate& creationDate);

// 다른 생성자들

// 복사 생성자를 포함해야 함
//

// 다양힌 규격의 생성작 포함
//
“PostMasterMessage(){}

void Edit(); // invokes editor on this message

const pAddress& GetSender() const { return itsSender; }

const pAddress& GetRecipient() const { return itsRecipient; }
const String& GetSubject() const { return itsSubject; }

// void SetSender (pAddress& );

// 다른 멤버 접근자

if
// 연산자 메쏘드 및 변환 루틴
//

ln

포함

private:
pAddress itsSender;
pAddress itsRecipient;
String itsSubject;
pDate itsCreationDate;
pDate itsLastModDate;
pDate itsReceiptDate;
pDate itsFirstReadDate;
pDate itsLastReadDate;

3;

PostMasterMessage: :PostMasterMessage(
const pAddress& Sender,
const pAddress& Recipient,
const String& Subject,
const pDate& creationDate):


===== PAGE 651 =====
650 ee 제3주

256:   itsSender (Sender),

2575   itsRecipient (Recipient),

258:   itsSubject(Subject),

239:   itsCreationDate(creationDate),

240:   itsLastModDate(creationDate),

241:   itsFirstReadDate(0),

242:   itsLastReadDate(0)

243:   {

244:      cout << "Post Master Message created. \n";

245:   Bs

246:

247: void PostMasterMessage: :Edit()

248: {

249:   cout << "PostMasterMessage edit function called\n";

250: }

251:

252:

253: int main()

254: £

255:  pAddress Sender (PostMaster, "jlibertya@PostMaster", "Jesse Leberty");
256: pAddress Recipient (PostMaster, "slLibertyaPostMaster","Stacey Liberty");
257: PostMasterMessage PostMasterMessage (Sender, Recipient, "Saying Hello",0);
258:   cout << "Message review... \n";

2592   cout << "From:\t\t" << PostMasterMessage.GetSender() << endl;
260:   cout << "To:\t\t" << PostMasterMessage.GetRecipient() << endl;
261:   cout << "Subject:\t" << PostMasterMessage.GetSubject() << endl;
262:   return 0;

263: |}

결과  Post Master Message created.

Message review...

From:             Jesse Liberty
To:               Stacey Liberty
Subject:          Saying Hello

분석  4번 줄의 270066는 unsigned 1008형의 17060라입니다. 날짜들을 long 정수형으로
저장하는 것은 드문 일입니다. 왜냐하면 날짜는 어떤 특정일(예를 들어 1900
년 1월 1일 0시)을 기준으로 하여 그때부터의 초를 가지고 계산하는 경우가 많기
때문입니다. 여기서 JAWS pDateS 진짜 클래스로 저장하고 싶을 것입니다.
5번 줄에서 나열형 상수 SERVICE} 정의되었는데 어떤 종류의 주소(우편 시스
템, CompuServe 등)를 가져야 하는지에 대한 주소 객체를 추적하기
니다.


===== PAGE 652 =====
세18일 객제 지향 SAD 설계 ㅇㅇ 651

- 161번 줄에서 String] 대한 인터페이스와 구현을 작성하였는데 앞부분의 장
들에서와 같은 부분이 많습니다. 90008 클래스는 많은 멤버 변수들이 메시지 클
래스에서 사용되게 하고, 또 많은 클래스들이 메시지에 의해 사용되게 하고 따라
서 여러분의 프로그램에서 중심이 됩니다. 완전하고 SRS String 클래스는 여러
분의 메시지 클래스를 완전하게 만드는데 기본이 됩니다.

- 183번 줄에서 pAddress 클래스가 선언되었습니다. 여기서는 이 Sar} 기

  |능 부분만 나타냈습니다. 여러분의 프로그램이 좀더 잘 이해되면 a
은 Fuel eto Aelch o] Ade Be Alaa 기본적인 요소들을 표
as       J

출력하는 문자열과 서비스를 위한 내부적으로 배달할 문자열을 계속 보유하는 것

이 pAddress 객체의 임무입니다. 단 하나의 pAddress 객체가 필요한지에 대한 질
문이 있을 수 있습니다. ae 각 서티스형에 대한 하부   클래스가 될 지에 대한
AEE 있습니다.      시브

191 - 229번 줄까지는 PostMasterMessage 클래스에 대한 인터페이스입니다. 이

별한 는 이 클래스는 상속 부분이 없지만 얼마 안 있어 이 부분을 상
계충에 넣어야 할 것입니다. 이를 MessageB HE] 상속되게 재설계할 때 몇몇
버 변수들은 베이스 클래스로 들어가게 될 것이고 다른 멤버 함수들은 베이스
래스 메쏘드에 중복될 것입니다.

때 o,f} 40

그 다양한 생성자, 접근자 함수 및 다른 멤버 함수들은 이 클래스에게 다양한 기
등성을 부여할 것입니다. 이 “ae 보여주는 것은 여러분  의 간단한 구동 프로그
램을 만들어 여러분의 가정들을 몇 가지를 검사할 때 여러분의 클래스가 100%
완벽한 것이 될 필요는 없다는 ag 보여줍니다.

247 - 2502 8010 함수가 있는데 편집기가 필요한 곳에 집어넣어지면 이 기능이
충분히 동작하는 것을 보여줍니다.

253 - 263번 줄에서 구동 프로그램을 보여줍니다. 이 프로그램은 단지 접근자 함
수와 operator<<2] 중복 이외에 아무 것도 하지 않습니다. 그럼에도 불구하고 여
러분에게 PostMasterMessageS: 가지고 실험하는 시작점을 보여주고 또 여기의 클
래스들을 수정하고 영향을 검사하는 구조를 제공합니다.


===== PAGE 653 =====
652 ee 제3주

ose 많은 0++의 FE 원소들을 결합하고 이를 객체 지향 분석, 설계, 프로
그래밍에 적용하는 것을 보았습니다.  i 주기는 깨끗한 분석에서 설계로 넘어
가고 거기서 완성을 향해 달려가는 그런 선형적인 과정이 아닙니다. 차리리 돌고
도는 과정입니다. 물론 첫 번째 단계는 분석입니다. 이 분석의 결과를 가지고 각
설계의 전초적인 베이스를 만들어 나갑니다.

예비 설계가 끝나면 프로그래밍이 시작될 수 있지만 프로그래밍 단계에서 분석과
설계로 계속적인 피드백이 일어납니다. 프로그래밍에서 검사와 디버그가 시작됩
니다. 주기는 계속 지속되고 적절한 시기에 컴퓨터에 올라가기 전까지는 끝나는
점이 보이질 않습니다.

객체 지향의 관점에서 문제를 분석할 때 문제들이 골치 아프게 작용하는 부
객체를 예비 설계하는 부분일 것입니다. 설계자는 계속 프로세서들을 관찰
가능할 때마다 객체를 캡슬화해야 합니다.

클래스의 계층 구조가 설계되어야 하고 각각의 상호 작용 부분의 순종 관계가 성
림되어야 합니다. 예비 설계는 완료되는 것을 의미하는 것이 아니고 설계가 완성
되어 가면서 객체간의 기능성이 완성되어 감을 의미합니다.

(A

oO
, =
}고

ol

객체 지향의 근본 목적은 가능한 한 많은 자료들과 FAS 은폐하고 분리된 객체
들을 만드는 것인데 각각은 정밀하고도 잘 정의된 인터페이스가 있어야 합니다.
여러분의 객체의 클라이언트들은 각 구현 부분들이 어떻게 작동하고 있는지 자세
히 보지 않아도 되게 해야 합니다.

Q&A
(객체 지향 분석과 설계는 다른 접근 방식에 비해 무엇이 근본적으로 다릅니까?
A 객체 지향 기법이 도입되기 전에는 분석가와 프로그래머는 프로그램을 자료를 가공
하는 함수로 생각했습니다. 객체 지향 언어는 통합된 자료와 함수를 하나의 분리된,
정보(자료)와 기능(함수)을 가진 단위로 봅니다. 순차적인 프로그램은 그와 다르게
함수 및 그 함수가 자료에 동작하는 과정에 초점을 Be. 파스칼과 ( 프로그램
들은 순차적인 함수와 자료의 모임체이고 +은 클래스의 모임체입니다.

Q Bal 지향 프로그래밍은 프로그램상의 SASS 모두 해결하는 해결사입니까?


===== PAGE 654 =====
세18일 객제 지향 분석과 설계 ㅇㅇ 653

A 아닙니다. 그렇게 고안된 것은 아닙니다. 그러나 크고 복잡한 객체 지향 분석과 설
계 프로그래밍은 프로그래머로 하여금 엄청난 복잡성을 다룰 수 있는 가능한 도구

들을 지원합니다.
Q C++2 완벽한 객체 지향 언어입니까?

A (++은 다른 객체 지향 언어와 비교해 수많은 이점과 단점이 있는데 다른 언어에
비해 장점이 하나 있습니다. 지구상에서 단 하나의 가장 흔하게 쓰이는 객체 지향
언어라는 것입니다. 사실 다른 객체 지향 언어로 설계하느라 기진맥진한 프로그래
머들이 무조건 CHS 선택하진 않습니다. 단지 좋은 곳이 있으면 그리로 갑니다.
1990년대에는 좋은 Ko] 0++이었습니다. 그만한 이유가 있습니다. 그럴만한 이유가
많다는 것은 Creo] 제공하는 것이 많다는 것입니다.

Q 어디서 객체 지향 분석과 설계를 좀더 배울까요?
 21일째 좀더 제안을 할 것입니다. 단 본인의 견해로는 수많은 객체 지향 분석서와
설계서가 있습니다. 다음을 추천합니다.

Object-Oriented Analysis and Design with Applications by Grady
Booch (2nd Edition).

Published by Benjamin/Cummings Publishing Company, Inc.,
ISDN:0-8053-5340-2

Object-Oriented Modeling and Design by Rumbaugh, Blaha, Premerlani,
Eddy and Lorenson.

Published by Prentice-Hall, ISBN 0-13-629841-9.

다

나 토구 chee 으아 아그 950066 고픈 마던
PCSAl 서

비스 일원으로 가입하는 것        슴니다.

5 "

를 여러분이 얼마나 잘 이해하였는가
a 수 있는 연습 문제들로 ras
Biol 대담을 할 수 있도록 노력하

록 합^

있도

할 수
1c.



===== PAGE 655 =====
654 ee 제3주

3. 개발 주기의 각 단계는 무엇입니까?

종 계층이란 무엇입니까?

§ 구동 프로그램이란 무엇입니까?
6 캡슬화란 무엇입니까?

연습  =

보도를 가지고 시뮬레이션한다고 합시다. 적
절한 nee inn 교통 신호의 시간을 결정하는 것이 목적입니다.

이 시뮬레이션에서 어떤 객체가 모델화되어야 하겠습니까? 어떤 클래스가 시뮬레이션되
어야 하겠습니까?

1번 질문이 뉴욕의 교외에서 일어났다고 해봅시다. 한국인으로서는 낮선 곳인데 3 종류
의 운전자들이 있습니다. 내국인으로서 통과 신호등이 들어오면 교차로를 통과하는 운
자이고, SWS 여행자로서 매우 조심스럽게 SAS 하며, 마지막으로 택시기사인데 탑
승객의 눈치를 살펴가며 마구 운전하는 사람입니다.
한편 뉴욕에는 두 종류의 보행자가 있습니다. 내국인으로 자기 기분 내키는 대로 횡단보
ES 건너는 사람이고 SMS 여행자로 통과 신호만 있을 때 건너는 사람입니다.
이러한 고려 사항들은 SAS 어떻게 바꿀까요?

글
기조
of
Hu
jo
OM
Hu
jo
EJ
a
oi
EJ
> 에
jr
for
=
1  i

frat

3% 그룹 스케줄을 설계하라는 요청을 받았습니다. 프로그램은 각 개인간과 그룹별로 모임을

정해야 하고 한정된 회의실을 예약해야 합니다. 기본 하부 시스템을 상술하십시오.
4 3번 문제의 회의실 예약 부분의 클래스의 설계와 인터페이스를 보이도록 하십시오.



===== PAGE 656 =====
n=

배



===== PAGE 657 =====
656 ce AB

때

은 전처리계에서 연결 연산자(600086608000 000080100)들 사용하여
을 만들기 위해 das 사용하는 we 공부하였습니다 ase
템플릿에 의해 고쳐지는 많은 문제점들을 가지고 있습니다.

Ei/=5)(Template)OlEt 무엇입ㄴ|까?

2번째 주 학습의 뒷부분에서 8009149 객체를 만드는 법과 88008080108를 만들
위해 이 객체를 사용하는 법에 대해 공부하였습니다. 여러분이 고양이의 목록을
만들기 위해 PartsList AAS 만들려고 한다면 다음과 같은 BAIS 안게 됩니다.
PartsList}= 단지 #0에 대해서만 안다는 것입니다.

2,
et

제를 풀기 위해 List 베이스 클래스를 만들고 여기서부터 2009146[와 CatsList
파생시켜야 합니다. Sol} PartsListo] WHS 자르고 붙여서 CatsList
만들어야 했습니다. 3째 주에 여러분이 Car 객체에 대한 SSS 다든지
했을 때 여러분은 새로운 클래스를 만들어야 했고, 여기서 또 자르고 붙이기

로 으
\» |y

때 님 때 때

의
으
rt
로
요

간 이는 좋은 방법이 절대 아닙니다. 계속해서 149 클래스 및
스가 확장되어야 합니다. 하나에서의 변화가 관련된 모든 클래스
로 번지는 것은 그야말로 Oh! my God. 입니다.

17 일 째에서 매개 변수화된 목록들을 사용하는 방법이 간략히 보여졌습니다. -
이 매크로와 이름   변절 방식(08016 000081608000)을 통해 couch 비록 매크로가
자르고 붙이는 JY] 많은 부분을 절약은 해 주지만 하나의 HS 단점이 있습
다. 대부분의 전처리계에 있는 기능이 그렇지만 형의 안정성(076-908을 보장 못

한다는 것입니다.



===== PAGE 658 =====
제19일 템플릿 ee 657

템플릿은 (++에서 매개 변수화된 SSS 만드는 좋은 RES 제공합니다. |
릿은 프로그래밍 언어에 있어서 통합된 부분이고 형의 안정성을 보장하며 융통
까지 가지고 있습니다.

매개 변수화된 형
플릿은 일련의 형태를 상술하는 목록을 만들기보다는 컴파일러에게 특정 형의
——_—ew—“owS oo 이이
록을 만드는 법을 가르쳐줍니다. 2009119는 각 Parte] 대한 목록이고 CatList=
CaS) 목록입니다. 다른 점흔 목록에서 대상에 대한 형태들입니다. 템플릿을 가지
목록에 있는 대상의 형태들이 클래스 정의시 매개 변수로 될 수 있습니다.

모든 Crt 상의 라이브러리의 구성은 배열 클래스로 이루어져 있습니다. 1496에서
보았듯이 하나의 배열 클래스를 여기서는 정수형, 다른 곳에서는 000016형, 혹은
AnimalsS] 배열로 만드는 것은 그야말로 BAA Yr. 템플릿은 매개 변수화된 배
열 클래스를 만들도록 하여주고 그 다음에 각 배열의 인스턴스들이 어떤 Bo] 객

체를 가질지를 상세하게 서술합니다.

새로운 인스턴스화(10618008400), 매개 변수화된 템플릿 템플릿으로부터 특수한 형태을
용어 만드는 것을 인스턴스화한다고 하는데 각각 개별적인 클래스들을 해당 템플릿의 인
스턴스라 부릅니다

템플릿 정의
다음과 깥이 써서 매개 변수화된 Array 객체(배열에 대한 템플릿)를 선언합니다.

1: template <class 1>// 템플릿과 매개 변수를 선언하고
2: class Array// 매개 변수화 되는 클래스

Se +

4° public:

5: Array();

6: // 완전한 클래스 선언 부
?

ss =    느

A

인 가고

예 약어 templateo] 템플릿 클래스 선언 및 정의의 시작 부분에 쓰여졌습니다. 템
플릿의 매개 변수가 예약어 template 다음에 옵니다. 매개 변수는 각 인스턴스에
따라 we 것입니다. |S 들면, 앞서 보여준 배열 템플릿에서 배열에 저장된 a



===== PAGE 659 =====
658 ee 제3주

체의 Qo] ua 것입니다. 어떤 인스턴스는 정수형 배열로 저장되고 다른 것
Animals 9] 배열로 저장이 됩니다.

이 예제에서는 예약어 class7} 사용되고 뒤따라 서술자 1가 사용되었습니다. 0055
는 예약어는 이 매개 변수가 형이라는 의미입니다. 서술자 TE 매개 변수화된
참조하기 위해 템플릿의 나머지 정의 부분에 사용되었습니다. 어떤 인스턴
Tt 나타나는 굿을 모두 정수형으로 바꼴 것이고 또 어떤 TEE 08형으로
바꿀 것입니다.

성수형과 08형으로 매개 변수화되는 배열 클래스를 선언하려면 이렇게 씀니다.

rlo

|» oft
(3 ° 이

Array<int> anIntArray;
Array<Cat> aCatArray;

Hal] anIntArray= 정수형 배열입니다. AA aCatArray= 0806형의 배열입니다. 쓰
자 하는 곳에서는 어디서나 Amay<int>S 쓸 수 있습니다 - 함수의 반환값으로
혹은 함수에 대한 매개 Wee 등등입니다. [리스트 19.11은 배열 템플릿의 완전
선언을 보여줍니다.

~ jo WH 로

[리스트 19.1]은 완전한 프로그램은 아닙니다.

[리스트 19.1] 배열 클래스의 템플릿

1: // [리스트 19.1] 배열 클래스의 템플릿

2: #include 여러개.

3: const int DefaultSize = 10;

4:

5: template <class T>

6: class Array

te: +"

8: public:

9:   // constructors

102   Array(int itsSize = DefaultSize);
41;   Array(const Array &rhs);

12:   “Array() { delete [CJ] pType; }

15°

14: // 연산작

152   Array& operator=(const Array&);
16:   T& operatorLI(int offset) { return pTypeLoffsetl; }

—
N



===== PAGE 660 =====
제19일 템플릿 ee 659

18:  // 접근자

19:   int getSize() { return itsSize; }
20%
21: private:

ee:   T *pType;
250   int itsSize;
24% Je

켈꽤 282 없습니다. 완성된 프로그램이 아닙니다.

분석  템플릿의 정의가 “ 줄에 예약어 template 및 뒤따라 나온 매개 변수와 같
~~    이 ai 이경     매 개 변수는 cgi class }] ~ 형으로 상술되었고

부터 템플릿의 선언이 끝나는 24번 줄까지의 선언부는 일반 다른 클래스의
와 같습니다. 단 하나의 차이점은 객체의 Bo] 일반적으로 나타나는 곳이
면 서술자 1가 대신 사용된다는 것입니다. 예를 들어, 000000[는 배열의 객체를
가리키는 참조자를 반환하는 것으로 기대되는데 실제 1에 대한 참조자를 반환하
도록 선언되었습니다.

6번 줄
H
선언부

|

정수배열의 인스턴스가 선언되었을 때 그 배열에 제공된 00800는 정수형에 대
한 참조 디즈 반환  베린 것입니다. Animal 배열의 인스턴스가 선언되었으면 Animalo|

고

|S = 0060010『=는 ^401081에 대한 참조자를 반환할 것입니다.

이름을 사용하여
클래스의 AMMA) Aray7} 더 이상의 표현 없이 사용되었습니다. 프로그램의 어
떤 곳에서도 이 클래스는 408%<1>로 참조될 것입니다. AS 들어, 클래스 AM
생성자를 만들지 않으면 여러분은 다음과 같이 작성해야 합니다.
template <class T>

Array<T>::Array(Cint size):
itsSize = size

{
pType = new TLCsizel;
for (int 1 =0; i< size ; i++)

pTypeLil = 0;
}



===== PAGE 661 =====
이 코드 부분의 첫 번째 줄의 선언부는 형을 식별하였습니다.(0066 77 템플릿의
이름은 Array<T>°] a. 8-H Array(int 9126)입니다.

이 함수의 나머지 BRS 비템플릿 함수와 같습니다. 클래스와 함수를 템플릿에
넣기 전에 클래스와 함수를 단순한 선언으로 동작하게 하는 것이 일반적인 방법
입니다.

템플릿의 구현
템플릿 클래스 배열의 완전한 FAS 복사 A414} operator=
합니다. [리스트 19.2]가 템플릿 클래스를 4
합니다.

구식 컴파일러는 이 템플릿을 지원 않습니다. 그러나 템플릿은 현존하는 ++의
분입니다. 모든 주요 컴파일러 공급자들은 다음 버전에서 템플릿을 지원하기로 하
|다. 여러분의 컴파일러가 템플릿을 지원하지 않으면 굳이 컴파일을 하려하지 at
HS 읽어본 뒤 나중에 좋은 컴파일러를 구입한 뒤 실럼해봅시다.

ki 32 wo we
내 %묘

rz 2

[리스트 19.2] HBS) 배열의 구현

#include <iostream.h>

const int DefaultSize = 10;

1
2
3
4:
5: // 단순한 Animal 클래스 선언
6   Wy)

7

8: class Animal
a: ££
10: public:

118    407108ㄴ(61012);

12    40708);
13%    “Animal() {}
14:    int GetWeight() const { return itsWeight; }

156    void Display() const { cout << itsWeight; }
16: private:

106    int itsWeight;

18! 3

19%



===== PAGE 662 =====
제19일 템플릿 oe 661

20:
215
22:
232
24:
255
26:
ere
28:
29:
30:
ols
32:
55:
34:
355
36:
378
58:
39:
40:
41:
42:
45:
44:
45:
46:
47:
48:
49:
50:
1s
de:
535
54:
558
56:
57:
58:
D9
60:
61:
62:
65:
64:
65:

Animal::AnimalCint weight);
itsWeight (weight)
{}

Animal::Animal():
itsWeight (0)
{}

template <class T> // 템플릿 및 매개 변수 선언
class Array        // 클래스가 매개 변수화 됨

{

public:

// 생성자
Array(int itsSize = DefaultSize);
Array(const Array &rhs);

“Array() { delete [] pType; }

// ary

Array& operator=(const Array&);

T& operatorL](int offSet) { return pTypeLoffSet]; }

const T& operatorL[](int offSet) const { return pTypeLoffSet]; }

// 점콘자
int GetSize() const { return itsSize; }

private:
T *pType;
int itsSize;
3;

//

-|4

a B
a8

rr

11 생성자 FH
template <class T>
Array<T>::Array(Cint size = DefaultSize);
itsSize(size)
{

pType = new T(size);

for (int i = 0; i<size; i++)

pTypeLil] = 0;

// 복사 생성자
template <class T>
Array<T>::Array(const Array &rhs)


===== PAGE 663 =====
662 eo AB

66:
67:
68:
69:
70:
(12
les
(3:
74:
tos
76:
Tt?
78:
(9:
80:
81:
Se
83:
84:
85:
86:
87:
88:
89:
90:
O15
92:
93:
94:
95:
96:
Or:
98:
99:

100:
101:
102:
103:
104:
105
106:
107:
108:
109:
110:
1111

itsSize = rhs.GetSize();

pType = new TLitsSizel;

for (int i = 0; i<itsSize; i++)
pTypeLil = rhslil;

// operator=
template <class T>
Array<T>& Array<T>::operator=(const Array &rhs)

{

}

if (this == &rhs)
return *this;

delete [3 pType;

itsSize = rhs.GetSize();

pType = new TLitsSizel;

for (int i = 0; i<itsSize; i++)
pTypeLil = rhslil;

return *this;

// 구동 프로그램

{

int main®         penne (Ae

AY ASA
Array<int>) theArray;
Array<Animal> theZoo;
Animal *pAnimal;

// WSS 채움
for (int i = 0; i < theArray.GetSize(); itt)
{
theArrayLil = i*2;
pAnimal = new Animal (i*3);
theZooLil] = *pAnimal;
ay

// 배열의 내용 출력
for (int j = 0; j < theArray.GetSizeQ; jtt+)
{
cout << "theArrayL" << j << "J:\t" << theArrayLjlJ << "\t\t";
cout << "theZooL" << j << "J:\t";
theZooLj].Display(;
cout << endl;
I

// 할당된 메모리 주소 반환



===== PAGE 664 =====
제19일 템플릿 ec 663

We:   for (int k = 0; k < theArray.GetSize(); k++)

113:     delete &theZooL[k];
114:   return Q;
115: }

겔과  theArrayLO]:      0        theZooL[0]:      0
theArray[1]:      2        theZooL[1]:       3
theArrayL[2]:      4        theZooL[2]:       6
theArrayL[3]:      6       theZooL[3]:      9
theArrayL4]:      8        theZooL4]:       12
theArrayL[5]:      10      theZooL[5]:      15
theArrayLl6]:       12        theZooL6]:       18
theArray([7]:      14       theZoo[7]:       21
theArrayL[8]:      16      theZooL[8]:      24
theArrayL[9]:      18       theZooL9]:       2

불샐 ＊- 26번 SS 간단한 Animal 클래스를 제공하였는데 배열에 추가될 사용자
정의형의 객체가 되기 위해 이곳에 만들어졌습니

29번 SL 다음이 MEME 것과 그 탭플릿에 대한 매개 변수가 형이라는 것
그리고 TR 되었다는 것을 나타냈습니다. Amay 클래스는 보여지는 바와 같이 두
개의 생성자를 가지고 있는데 그중 첫 번째는 see 취하고 상수형 정수
DefaultSizeS 기본으로 갖습니다. 치환과 변위 연산자가 선언되었는데 후에 const
와 비 const 선언되었습니다. 단 하나의 접근자는 0851260인데 배열의 크기를
반환합니다.

여러분은 좀더 완전한 인터페이스를 생각할 수 있는데 여기에 제공된 Amy 프로
그램은 그렇지 않습니다. 최소한 원소를 제거하고 배열을 확장하고 배열에 저장
하는 그러한 연산자들이 필요합니다.

전용 자료는 배열의 크기와 메모리에 있는 배열 객체의 포인터로 구성되어 있습

x

배열 객체를 여러분의 함수에 전달하고자 하면 여러분은 배열의 특정 인스턴스를
하고 템플릿 자체를 전달하여서는 안됩니다. 따라서 SomeFunction()°]
매개 변수로 정수형 배열을 취하면 이렇게 쓸 수 있습니다.

void SomeFunction(Array<int>&) ;// 정상


===== PAGE 665 =====
664 ee 제3주

하지만 이렇게 쓰면 안됩니다.

void SomeFunction(Array<T>&) ;// 오류
7&가 무엇인지 알 길이 없습니다. = 이렇게 써도 안됩니다.
void SomeFunction(Array&) ;// 오류

클래스 Amay7} 없습니다. 단지 템플릿과 인스턴스

좀더 일반적인 접근을 시도하기 위해, 함수 템플릿을 선언해야.함니다.

뿌
어브
피>
트레
aw

template <class T>
void MyTemplateFunction(Array<T>&) ;// 정상

여기서 함수 MyTemplateFunction)o] 맨 윗줄의 선언에 의해 템플릿 함수로 Aas
었습니다. 템플릿 함수는 다른 함수와 마찬가지로 어떤 이름도 가질 수 있습니다.
템플릿 함수는 템플릿의 인스턴스를 취할 수 있고, 추가로 매개 변수화된 형태를
가질 수 있습니다. 다음이 예입니다.

template <class T>
void MyOtherFunction(Array<T>&, Array<int>&) ;// 정상

이 함수는 두 개의 MAS 취합니다. 매개 WEB arrays} 정수형의 20입니다.
전자는 어떤 객체의 배열도 될 수 있지만 후자는 정수형의 배열이어야 합니다.

템플리과 프랜드

2. 일반적인 템플릿 프랜드 클래스 혹은 함수
3. 형 상술화한 템플릿 프랜드 클래스 혹은 함수

비템플릿 프랜드 클래스와 함수

어떤 클래스 혹은 함수를 여러분 템플릿 클래스의 프랜드로 ade 수 있습니다.
각 클래스의 인스턴스는 프랜드를 마치 프랜드의 선언이 그 특정 인스턴스에 만
soa 것처럼 적절하게 다룰 것입니다. [리스트 193|은 간단한 프랜드 함수

1000060를 Array SAAS] 템플릿 정의에 추가하였고 구동 프로그램이 Intrude()



===== PAGE 666 =====
세19일 템플릿 ee 665

호출하였습니다. 프랜드이기 때문에 IntrudeQE 4784의 전용 자료를 접근할 수 있
습니다. 이는 템플릿 함수가 아니므로 정수형의 Anayo] 호출될 수 있습니다.

[리스트 19.3]을 사용하기 위해 [리스트 19.2]의 ㅣ - 26번 줄을 이 예제의 po 줄 다음
에 쓰고 [리스트 19.2]의 51-86번 줄을 37번 다음에 복삭하시오.

[리스트 19.3] 비템플릿 프랜드 함수

1: // [리스트 19.37 비템플릿 프랜드 함수
2

3: template <class T>

4: class Array

52 4

6: public:

7     // constructors

8:    Array(int itsSize = DefaultSize);
91    Array(const Array &rhs);

10%   “Array() { delete [J pType; }
V1:

12   // operators

1365   Array& operator=(const Array&);

14:   T& operatorLI (int of fSet) { return pTypeLoffSetl; }

15:   const T& operatorLJ](int offSet) const { return pTypelLoffSet]; }
16:

178   // accessors

18:   int GetSize() const { return itsSize; }
193

20:  // 프랜드 함수

218   friend void Intrude(Array<int>) ;

cee

23: private:

24:   T *pType;

2”   int itsSize;

2600 +5

er:

28: // 프랜드 함수

293 //

30: void Intrude(Array<int> theArray)

$1: ¢

Sez   cout << "\n*** Intrude ***\n";

338   for (int 1 =ㅋ02 1 < theArray.itsSize; 1++)

348      cout << "i: " << theArray.pTypeLil << endl;


===== PAGE 667 =====
666 ce AB

55:   cout << "\n";

56: 3

Sr:

38: // PE 프로그램

39: int main

40: {

41:   Array<int> theArray;

42%   Array<Animal> theZoo;

43:   Animal *pAnimal;

44:

45: // WSS 채움

46:   for (int i = 0; i < theArray-GetSize(Q); it+)
47:   {

48:      theArrayLil = i*2;

49:      pAnimal = new Animal (i*3);

503      theZooLi] = *pAnimal;

1s   }

52:

53:  // 배열의 내용 출력

54:   for (int j = 0; 1 < theArray.GetSizeQ; j++)
55:   {

362     cout << "“theZooL" << j << "1:\t";

De     theZooLjJ.DisplayQ;

506:      cout << endl;

595   }

60:   cout << "Now use the friend function to 7
61:   cout << "find the members of Array<int>";
62:   Intrude(theArray) ;

64:  // 메모리 반환

65:   for (int k = 0; k < theArray.GetSize(); k++)
66:     delete &theZooLlk];

67:

68:   cout << "\n\nDone.\n";

692   return 0;

701 3

결고

theZooL01]:           0
theZooL1]:           5
theZooL[2]:           6
theZooL[31:           9
theZooL[4]:           12
theZooL[51]:           15
theZooL6]:           18

theZooL7]:           21



===== PAGE 668 =====
제19일 템플릿 ee 667

theZooL[8]:           24
theZooLl9]:           27

Now use the friend function to find the members of Array<int>
xxx Intrude **x

nN OO

= 8

: 10
2 12
: 14
: 16
: 18

Ce Ce Pe 자 자 가 가
… … …… …"

Done.

분석 이 배열 템플릿의 선언은 프랜

다. 이 선언은 배열의 모든 인
턴스

하고 또 IntrudeQ=E 배열 인스턴

= 함수 1000060를 포함하도록 확장되었습니
스턴스가 10ㅁ0060를 프랜드 함수로 생각하게
13 멤버 자료와 함수에 접근할 수 있습니다.
33번 줄에서 1000060는 159126에 직접 접근하고 34번 Solr] pType] 직접 접근
합니다. 이 멤버들에 대한 사용들은 배열 클래스가 이 자료에 대한 범용 접근자
를 제공하므로 불필요하지만 프랜드 함수가 템플릿과 함께 선언되는 것을 보여주
기 위해 예제로 보여줬습니다.

은
[세

일반 템플릿 프랜드 클래스/함수
amy GAA 출릭    ane 추가하는 것은 도움이 될 것입니다. 하나의 접근
ㅅ           는 것

이지만 이는 amayS 템플릿으
로 만드는 ㅇ

fut
|이
4
nz,
ro,
aes
AG)

정작 필요한 AS 모든 208》의 형에서 동작하는 삽입 연산자입니다.
ostream& operator<< (ostream& Array<T>&);

이것이 동작하게 만들기 Sal operator<<S 템플릿 함수로 만들어야 합니다.
template <class T> ostream& operator<< Costream&, Array<T>&)

이제 operator<< 템플릿 함수이고 여러분은 단지 구현만 하면 됩니다. [리스트
19.4]는 이 선언을 포함하도록 200》를 확장하였고 006000[<<를 위한 구현을 제공
하였습니다.


===== PAGE 669 =====
668 ㅇㅇ 제주

이 예제를 컴파일하| 위해 [리스트 19.2]의 8-26번 SS 3번과 4번 사이에 oo abe os
시다. 그리고 [리스트 19.2]의 51-86을 37과 38번 사이에 넣읍시다.

[리스트 19.4] operator ostream 사응하기

#include <iostream.h>

const int DefaultSize = 10;

1

2

3

4:

5: template <class T>
6: class Array

7

8

{
public:
os    // constructors
10:   Array(int itsSize = DefaultSize);
118   Array(const Array &rhs);
128   “~Array() { delete [4 pType; }
15:
14:   // operators
15%   Array& operator=(const Array&);

16:   T& operatorLi(int offSet) 1 return pTypeLoffSetl; }
173   const T& operatorL[](int offSet) const { return pTypeLoffSetl; }

18%

1\9=   // accessors

20%   int GetSize() const { return itsSize; }
21:

22:    template <class T> friend ostream& operator<< (ostream&, Array<T>&);
25:

24: private:

25°   T *pType;

26:   int itsSize;

205 0;

28:

29: template <class T>

30: ostream& operator<< (ostream& output, Array<T>& theArray)
31: £

522   for (int i = 0; i<theArray.GetSize(); i++)

53:   output << "[" << i << "J" << theArrayLlil << endl;

54: }

36: enum BOOL { FALSE, TRUE};

38: int main(Q)



===== PAGE 670 =====
제19일 템플릿 ee 669

39: 4

40:  BOOL Stop = FALSE; // #3f2 flag

41:   int offset, value;

42:   Array<int> theArray;

43:

44:   while (!Stop)

45:   af

46:      cout << "Enter an offset (0-9) and a value. (-1 to stop): ";
47:      cin >> offset >> value;

48:

49:      11 Coffset <0)

50:        break;

51

52:      if (offset > 9)

55)      {

54:        cout << "***Please use values between 0 and 9.***\n";
55%        continue;

56:      }

Df:

58:      theArrayLoffset] = value;

59:

60:

612   cout << "\nHere's the entire array:\n";

62:   cout << theArray << endl;
63:   return 0;
64: }

re Wy Enter an offset (0-9) and a value. (-1 to stop): 1 10
Enter an offset (0-9) and a value. (-1 to stop): 2 20
Enter an offset (0-9) and a value. (-1 to stop): 3 30
Enter an offset (0-9) and a value. (-1 to stop): 4 40
Enter an offset (0-9) and a value. (-1 to stop): 5 50
Enter an offset (0-9) and a value. (-1 to stop): 6 60
Enter an offset (0-9) and a value. (-1 to stop): 7 70
Enter an offset (0-9) and a value. (-1 to stop): 8 80
Enter an offset (0-9) and a value. (-1 to stop): 9 90
Enter an offset (0-9) and a value. (-1 to stop): 10 10
*xx*PlLease use values between 0 and 9. ***

~

Enter an offset (0-9) and a value. (-1 to stop): -1 -1
Here's the entire array:

[01 0

C1] 10

[2] 20

[3] 30


===== PAGE 671 =====
670 ee 제3주

[4] 40
[5] 50
[6] 60
{71 70
[8] 80
[9] 90

분석 22번 줄에서 함수 BSA operator<<()o] Amay 클래스 템플릿의 프랜드로

선언되었습니다. 006010<<0는 템플릿 함수로 구현되었으므로 이 매개 변수

화된 배열형의 모든 인스턴스들은 자동으로 000800<<(를 가질 것입니다. 이 A

산자에 대한 FAS 29번 So] 있습니다. 배열의 모든 Wyse] 차례로 호출됩니

다. 배열에 저장된 모든 형의 객체에게 정의된 078010<<가 있어야만 동작을 합
니다.

형이 서술된 템플릿 프랜드 클래스/함수
[리스트 1941에서 보여준 삽입 연산자가 비록 동작은 하지만 아직 충분한 것은
아님니다. 22번 줄에서의 프랜드 연산자의 선언은 템플릿을 선언하였으므로 00)
의 모든 인스턴스와 배열을 취하는 모든 삽입 연산자에 동작할 것입니다.
[리스트 194|에 보여진 삽입 연산자 템플릿은 삽입 연산자 00000[<<의 모든 인

스

형이건 400081형이건 0#이건 따지지 않습니다. Animals] 삽입 연산자를 정수형
Array9] 삽입 연산자의 프랜드로 하는 것은 의미가 없습니다.

원하는 것은 정수형의 4080에 대한 삽입 연산자를 정수형 클래스의 프랜드로 하
는 것이고 400181의 Array] 삽입 연산자를 animal 인스턴스의 ^478》의 프랜드가

이를 달성하기 위해 [리스트 19.4]9] 22번 줄의 삽입 연산자의 선언부를 수정하여
template <Class 1>를 지움니다. 22번 SS 아래와 같이 바꿈니다.

friend ostream& operator<< (ostream&, Array<T>&);

이는 ANS 4000의 템플릿에서 선언합니다. 따라서 정수형에 대한 operatore<t=
정수형에 대한 배열을 가져야 동작할 것입니다.



===== PAGE 672 =====
제19일 템플릿 ee 671

템플릿의 항목들을 다른 형에서 하듯이 다룰 수 있습니다. 참조자나 gow 하여
매개 변수로 전달할 수 있고 함수의 반환값으로 하듯이 반환값으로 사용할 수 있

는 값이나 참조자로 반환할 수 있습니다. [리스트 195 템플릿의 객
AZ 전달하는 예를 보여줍니다.

[리스트 19.5] BAO 앞뒤로 HES ANS 전달하기

#include <iostream.h>

const int DefaultSize = 10;

class Animal
{
: public:
9:    // constructors
4102   Animal (int);
ES   Animal ();

1

2

3

4:

5: // 배열에 추가될 클래스
6:

7

8

121   “Animal ();
15H
14:   // accessors

155   int GetWeight() const { return itsWeight; }
16:   void SetWeight(int theWeight) { itsWeight = theWeight; }
1068

18:   // friend operators

19:   friend ostream& operator<< (ostream&, const Animal&);
20:

21: private:

22:   int itsWeight;

252 +8

24:

25: // extraction operator for printing animals
26: ostream& operator<<

2rs    Costream& theStream, const Animal& theAnimal);
28: {

29:    theStream << theAnimal.GetWeight();

$0:    return theStream;

S12 }

326

33: Animal::Animal (int weight):
34: itsWeight (weight)
55: <


===== PAGE 673 =====
672 ㅇㅇ 제주

36:
Sf:
58%
59°
40:
41:
42:
43:
44:
45:
46:
Ars
48:
49:
50:
oT:
52:
22.
541
53:
30%
af:
58:
395
60:
Ole
62:
65%
64:
65:
66:
OF:
68:
69:
708
1s
les
(3:
14:
fey
162
1G:
78:
79:
80:
812

// cout << "Animal Cint)\n";
a

Animal::Animal():
itsWeight (0)
£

// cout << "AnimalQ\n";

Animal::~Animal()

{

// cout << "Destroyed an animal...\n";
Es

template <class T> // 템플릿과 매개 변수 선언
class Array        // 클래스가 매개 변수화됨
€
public:
Array(int itsSize = DefaultSize);
Array(const Array &rhs);
“Array() { delete [] pType; }

Array& operator=(const Array&);
T& operator[li(int offSet) { return pTypeLoffSetl; }
const T& operatorL[l](int offSet) const
{ return pTypeLoffSet]; }
int GetSize() const { return itsSize; }

// friend function

friend ostream& operator<< (ostream&, const Array<T>&);
private:

T *pType;

int itsSize;
3;

template <class T>
ostream& operator<< (ostream& output, const Array<T>& theArray)
{
for (int i = 0; i<theArray.GetSize(); i++)
output << "[" << i << "J" << theArrayLil << endl;
return output;

void IntFillFunction(Array<int>& theArray) ;
void Animal Fill Funtion(Array<Animal>& theArray) ;
enum BOOL { FALSE, TRUE};



===== PAGE 674 =====
제19일 템플릿 oe

673

82:
83:
84:
85:
86:
87:
88:
89:
90:
915
928
93:
94:
95%
96:
972
98:
99:

100:
101:
102:
103:
104:
1052
106:
107:
108:
109:
110:
A115
112:
(1S:
114:
1154
116"
Te
118:
1195
120:
121%
122:
123:
124:
125°

int main()

{

Array<int> intArray;

Array<Animal> animalArray;
IntFillFunction(intArray) ;

Animal Fill Function(animalArray) ;

cout << "intArray...\n" << intArray;

cout << "\nanimalArray...\n" << animalArray << endl;
return 0;

void IntFillFunction(Array<int>& theArray)

4

BOOL Stop = FALSE;
int offset, value;
while (!Stop)

{

cout << "Enter an offset (0-9) ";
cout << "and a value. (-1 to stop): ";
cin >> offset >> value;
if (offset < 0)

break;
if (offset > 9)
{

cout << "*x*xPlease use values between 0 and 9.kkk\N";

continue;
3
theArrayLoffset] = value;

void Animal Fill Function(Array<Animal>& theArray)

{

Animal * pAnimal;
for Cint i = 0; i<theArray.GetSize(); i++)

{

pAnimal = new Animal;
pAnimal->SetWeight(i*100) ;
theArrayLil = *pAnimal;
delete pAnimal;



===== PAGE 675 =====
674 ee 제3주

결 1 bs 6Enter an offset (0-9) and a value. (-1 to stop): 1 10
Enter an offset (0-9) and a value. (-1 to stop): 2 20
Enter an offset (0-9) and a value. (-1 to stop): 3 30
Enter an offset (0-9) and a value. (-1 to stop): 4 40
Enter an offset (0-9) and a value. (-1 to stop): 5 50
Enter an offset (0-9) and a value. (-1 to stop): 6 60
Enter an offset (0-9) and a value. (-1 to stop): 7 70
Enter an offset (0-9) and a value. (-1 to stop): 8 80
Enter an offset (0-9) and a value. (-1 to stop): 9 90
Enter an offset (0-9) and a value. (-1 to stop): 10 10

*xxPlease use values between 0 and 9. ***
Enter an offset (0-9) and a value. (-1 to stop): -1 -1

intArray...
[03 0
[1] 10
[2] 20
[3] 30
[4] 40
E53] 50
[6] 60
[7] 70
[8] 80
[9] 90

animalArray...
CO] 0
[1] 100
[2] 200
[3] 300
[4] 400
[5] 500
[6] 600
[71 700
[8] 800
[9] 900

불샐 Array 클래스의 구현은 지면상 제외하였습니다. Animal 클래스가 623번 줄에
서 선언되었습니다. 단순하게 만든 클래스이지만 자체의 삽입 연산자(<<)를
Animal 출력하도록 제공하였습니다. 출력은 Animale] 현재 무게를 출력합니다.
Animal 기본 생성자가 있습니다. 이는 필요한데, 왜냐하면 여러분이 객체를 배
열에 추가할 때 객체의 기본 생성자가 객체를 만들기 위해 사용되기 때문입니다.
보겠지만 약간의 다른 점이 있습니다.



===== PAGE 676 =====
제19일 템플릿 ee 675

79번 줄에서 함수 10041000000000이 선언되었습니다. 원형에서 보듯이 이 함수는
정수형 WSS 취합니다. 이는 템플릿 함수가 아닙니다. 0011800081000은 단지
하나의 배열형을 원합니다. 즉, 정수형 배열입니다. 비슷하게 sow 줄에서
AnimalFillFunction()°] Animal?) ArayS 취하도록 선언되었습니다.

이 함수들의 구현이 서로 다른데 이는 함수형의 배열을 채우는 것은 440006의
배열을 채우는 것과 같은 방식으로 수행되지 않기 때문입니다.

특수 함수들

[리스트 19.5]에서 Animale] 생성자와 소멸자의 출력문을 주석으로 막으면
Animals] 대한 기대하지 않았던 생성자와 소멸자가 있다는 것을 알게 됩니다.

배열에 객체가 추가되면 객체의 기본 생성자가 호출됩니다. Amay 생성자는 [리스
트 19.2}9} 59, 60번 줄에서와 같이 배열의 각 멤버에 0값을 할당하기 시작합니다.
someAnimal = (Animal) 0; 라고 쓰면 Animalol] 대해 기본 연산자 operator=S 호출
합니다. 임시 Animal 객체가 정수를 취하는 생성자를 사용하여 만들어집니다. 이
임시 객체는 등치 연산자의 오른쪽 값으로 사용되고 소멸됩니다.

이는 시간 낭비인데, 왜냐하면 Animal 객체가 이미 적절하게 초기화되었기 때문입
니다. 그렇다고 하여 이를 제거할 수는 없는데 정수들이 자동적으로 0의 값으로
초기화되었기 때문입니다. 이의 해결 방법은 템플릿으로 하여금 400081에게 이 생
AAS 사용하지 맡고 특수한 Animals] 생성자를 사용하도록 하게 하는 것입니다.
Animal 클래스에 대한 명시적인 구현을 제공할 수 있는데 [리스트 19.6|이 이것입
니다.

[리스트 19.6] 특수 템플릿 구현

1   #include <iostream.h>

2:
3: const int DefaultSize = 3;
4

5: // 배열에 추가될 클래스들
6   class Animal

i "

8: public:

9      // constructors
105    AnimalCint);

11     Animal();


===== PAGE 677 =====
676 ㅇㅇ 제주

12:    “Animal ();

AS:

14:    // accessors

156    int GetWeight() const { return itsWeight; }

16:    void SetWeight(int theWeight) { itsWeight = theWeight; }
Wee

18¢    // friend operators

19:    friend ostream& operator<< (ostream&, const Animal&);
20:

21: private:

221    int itsWeight;

25, Fe

24:

25: // extraction operator
26: ostream& operator<< (ostream& theStream, const Animal& theAnimal);

An

26:    theStream << theAnimal.GetWeight();
(he    return theStream;

3018 +

Sit

32: Animal::Animal (int weight):
33: itsWeight (weight)

34: ¢

55°    cout << "animal (int) ";
36: }

S03

38: Animal::Animal(Q:
39: itsWeight (0)

40: <

41:    cout << "animal() ";

42: }

43:

44: Animal::”~Animal()

452 <

46:    cout << "Destroyed an animal...";
4/7: >

48:

49: template <class T>
50: class Array

516 1

521 public:

531    // constructors

54:    Array(int itsSize = DefaultSize);
013)    Array(const Array &rhs);

56:    “Array() { delete [] pType; }

5s



===== PAGE 678 =====
제19일 템플릿 ee 677

58:
59
60:
61%
62:
63:
64:
65%
66:
67:
68:
69:
70:
1:
128
(38
(43
(58
16:
771
78:
79:
80:
813
82:
83:
84:
85:
86:
87:
88:
89:
90:
91:
925
93:
94:
95:
96:
971
98:
99:

100:
101:
102:
103%

// operators

Array& operator=(const Array&);

T& operator(CiCint of fSet) { return pTypeLoffSet]; }

const T& operator[]Cint offSet) const { return pTypeLoffSetJ; }

// accessors
int GetSize() const { return itsSize; }

// friend function
friend ostream& operator<< Costream&, const Array<T>&);

private:
T *pType;
int itsSize;
3;

template <class T>
Array<T>::Array(int size = DefaultSize):
itsSize(size)
{
pType = new TEsizel;
for (int i = 0; i<size; i++)
pTypeLil = (1T)0;

template <class T>
Array<T>& Array<T>::operator=(const Array &rhs)
{
if (this == &rhs)
return *this;
delete [3 pType;
itsSize = rhs.GetSize();
pType = new TLitsSizel;
for (int i = 0; i<itsSize; i++)
pTypelil = rhslil;

template <class T>
Array<T>::Array(const Array &rhs)
{
itsSize = rhs.GetSize();
pType = new TCitsSize);
for (int i = 0; i<itsSize; i++)
pTypeLlil = rhslil;


===== PAGE 679 =====
678 ee AB

104:
105:
106:
107:
108:
109:
110:
ys bi Fr
112:
1156
114:
1158
116%
17s
118
119%
120:
121%
122:
123:
124:
1250
126:
127:
128:
129:
150:
1312
152:
133:
134:
135:
136:
VS
138:
139:
140:
141:
142:
1435
144:
145:
146:
147:
148:
149:

template <class T>
ostream& operator<< (ostream& output, const Array<T>& theArray)
{
for (int i = 0; i<theArray.GetSize(); i++)
output << "L" << i << "J" << theArrayLlil << endl;
return output;

Array<Animal>::Array(int AnimalArraySize):
itsSize(AnimalArraySize)
Ke
pType = new T(AnimalArraySize);
}

void IntFillFunction(Array<int>& theArray);
void Animal Fill Funtion(Array<Animal>& theArray);
enum BOOL { FALSE, TRUE};

int main()
{
Array<int> intArray;
Array<Animal> animalArray;
IntFillFunction(intArray) ;
Animal FillFunction(animalArray);
cout << "intArray...\n" << intArray;
cout << "\nanimalArray...\n" << animalArray << endl;
return 0;

void IntFillFunction(Array<int>& theArray)
{
BOOL Stop = FALSE;
int offset, value;
while (!Stop)
{
cout << "Enter an offset (0-9) and a value. (-1 to stop): ";
cin >> offset >> value;
if (offset < 0)
break;
if (offset > 9)
ne
cout << "***PLease use values between 0 and 9.*x**\n";
continue;


===== PAGE 680 =====
제19일 템플릿 ee 679

150:      }

151s      theArrayLoffset] = value;

152:   0

1532 3

154:

155<

156: void AnimalFillFunction(Array<Animal>& theArray)
Vole £

158:    Animal * pAnimal;
159s    for (int i = 0; i<theArray.GetSize(); i++)
160:    {
161:      pAnimal = new Animal (i*10);
162:      theArrayLil = *pAnimal;
163:      delete pAnimal;
164:    a:
165: }
분석을 쉽게 하기 위해 SA ASS 붙였습니다. 여러분의 플력에서는 번호가 of 나
타납니다.
결과      1: animal() animal() animal() Enter an offset (0-9) and a value.

(41 to stop): 0 0

2: Enter an offset (0-9) and a value. (-1 to Stopi< 1 1

3: Enter an offset (0-9) and 8 value. (-1 to Stop) + 2 2

4: Enter an offset (0-9) and a value. (-1 to stop): 33

5: Enter an offset (0-9) and a value. (-1 to stop): -1 -1

6: animal(int) Destoryed an animal... animal (int) Destoryed an

animal...animal(int) Destoryed an animal...initArray...

7. [0] 0

38 011 4

이 [202

10:

11: animal array...

12: [07] 0

132 [1] 10

14: [2] 20

152

16: Destoryed an animal...Destoryedananimal...Destoryedananimal...
4 WY de
<<< 두 번째 수행 >>>

18: 바소 Destroyed an animal.

19: animal(int) Destroyed an animal...


===== PAGE 681 =====
680 ㅎㅇ 제3주

20: 30108ㄴ(101) Destroyed an animal..

21: Enter an offset (0-9) and a value. (-1 to stop): 00
22: Enter an offset (0-9) and a value. (-1 to stop): 1 1
23: Enter an offset (0-9) and a value. (-1 to stop): 2 2
24: Enter an offset (0-9) and a value. (-1 to stop): 3 3
25: animal (int)

26: Destoryed an animal...

27: animal (int)

28: Destoryed an animal...

29: animal (int)

30: Destoryed an animal...

Ss IM tA ay cc»

32: [01 0

331 E12 1

34: [234 2

36: animal array...
37: [01 0
38: [11 10
Sye=Ee 20

41: Destoryed an animal...
42: Destoryed an animal...
43: Destoryed an animal...

aa

석  [리스트 19.6]|은 임시 Animal 객체의 생성과 소멸을 볼 수 있도록 클래스들
을 다시 만들었습니다. SBS 간단히 하기 위해 DefaultSizeS 3으로 SY
습니다.

32 - 47의 Animal 생성자와 소멸자는 그들이 언제 호출되는지를 알리기 위해 4
각 문장을 출력합니다

74 - 81번 SoA] array 생성자의 템플릿이 선언되었습니다. 114 - 118번 줄에서
^70101의 Array 위한 특수 생성자가 보여졌습니다. 이 특수 생성자에서 기본 생
성자가 각각의 동물에 대한 초기값을 설정하도록 하였고 명시적인 대입은 없었습
니다.

이 프로그램이 처음 수행될 때 Sao] AS 설정이 보여졌습니다. 출력의 AH
째 줄은 세 개의 기본 생성자가 MSS 만들면서 호출됨을 보였습니다. 사용자는
4개의 숫자를 입력하고 이는 각각의 정수 배열로 들어갑니다.

실행은 AnimalFillFunction0 2° = 뛰어갑니다. 161번 줄에서 힙에 임시 Animale] 만
들어졌고 162번 줄에서 배열상의 Animal 객체를 수정하기 위해 그 값이 사용되었



===== PAGE 682 =====
세19일 템플릿 ee 681

습니다. 163번 SA 임시 Animalo] 소멸되었습니다. 이런 과정이 각 배열의 각
멤버에 대해 되풀이되었고 출력의 6번 줄에서 출력됩니다.

프로그램의 마지막에서 배열이 소멸되었고 각각의 소멸자가 호출되었을 때 그들
의 객체도 역시 소멸됩니다. 이것은 출력의 16번 줄에서 보여졌습니다.

출력의 두 번째 과정 (18 - 43)에서는 프로그램의 114 - 118번 So] 있는 문자 생
성자의 배열의 특수 구현 부분이 주석으로 막혔습니다. 프로그램이 다시 수행될
때 74 - 81번 줄에 있는 템플릿 생성자가 Animal 배열이 생성되면서 다시 수행됩
니다.

이렇게 하면 임시 Animale) 객체가 배열의 각 멤버에 대해 호출이 되고(79 - 80
번 줄) 출력의 18 - 20번 So] 나타납니다.

두 개의 수행 과정의 출력은 Segue,

정적 멤버와 템플릿
deve 정적 자료 WME 선언될 수 있습니다. 템플릿의 각 인스턴스화된 것은
그 자신의 정적 자료 집합을 가지는데 클래스형에 대해 하나씩입니다. 말하자면
정적 WAS Array 클래스에 추가하면(예를 들어 얼마나 많은 배열이 만들어졌는
지를 세는 증감기) 각 형에 대해 이 WAS 가집니다. SHE Animals] 모든 배열
에 대해 또 다른 것은 정수형의 모든 배열에 대해서 입니다. [리스트 19.71은 정
적 WS 추가했고 Amy 클래스에 정적 함수를 추가합니다.

[리스트 19.7] 템플리과 함께 정적 멤버 자료와 정적 멤버 BAS Soe of

1: #include <iostream.h>

2s

3: template <class T>

4: class Array

be 이

6: public:

te    // constructors

8:    ArrayCint itsSize = DefaultSize);
oF    Array(const Array &rhs);

10:   “Array() { delete [] pType; itsNumberArrays--; }
ie

12:   // operators

13%   Array& operator=(const Array&);
14:   T& operatorLi (int of fSet) { return pTypeLoffSet]; }
15:   const T& operator[I(int offSet) const { return pTypeLoffSet]; }


===== PAGE 683 =====
682 ee AB

16:

173   // accessors

18:   int GetSize() const { return itsSize; }

193   static int GetNumberArrays() { return itsNumberArrays; }
208

21:   // friend function

2e%   friend ostream& operator<< (ostream&, const Array<T>&);
25%

24: private:

(se%r   T *pType;

26:   int itsSize;

20   static int itsNumberArrays;

28: 3;

29:

30: template <class T>

31: int Array<T>::itsNumberArrays = 0;

021

33: template <class T>

34: Array<T>::Array(int size = DefaultSize):

35: itsSize(size)

562 {

371    pType = new TLsizel;

38:    for (int i = 0; i<size; i++)
59%      pTypeLil = (1)0;

40:    itsNumberArraystt;

6,

42:

43: template <class T>
44: Array<T>& Array<T>::operator=(const Array &rhs)

45: ¢
46:   if (this == &rhs)
47s      return *this;

48:   delete [3 pType;

49:   itsSize = rhs.GetSize();

50:   pType = new TLitsSizel;

Sit   for (int i = 0; i<tisSize; i++)
by Ne      pTypeLil = rhsLlid;

5S: >

54%

55: template <class T>

56: Array<T>::Array(const Array &rhs)
57 at

58:   itsSize = rhs.GetSize();

59:   pType = new TLitsSizel;

60:   for (int i = 0; i<itsSize; itt)
6133      pTypelil = rhslil;



===== PAGE 684 =====
제19일 템플릿 ee 683

62:
O35:
64:
65:
66:
67:
68:
69:
708
711
(ee
13%
74:
(os
76:
“rs
78:
“98
80:
81
828
83:
84:
85:
86:
87:
88:
89:
90:
913
92:
93:
94:
955
96:
OF:
98:
99:

100:
1018
11025
103:
104:
105:

itsNumberArrays+t+;
가

template <class T>
ostream& operator<< (ostream& output, const Array<T>& theArray)
x
for (int i =0; i<theArray.GetSize(); i++)
output << "[" << i << "]_" << theArrayLil] << endl;
return output;
}

Array<Animal>::Array(int AnimalArraySize):
itsSize(AnimalArraySize)
nf
pType = new TCAnimalArraySizel;
itsNumberArrays+tt;
Ps

int main()
(

cout << Array<int>::GetNumberArrays() <<" integer arrays\n";
cout << Array<Animal>::GetNumberArrays();

cout <<" animal arrays\n\n";

Array<int> intArray;

Array<Animal> animalArray;

cout << intArray.GetNumberArrays() << " integer arrays\n";
cout << animalArray.GetNumberArrays();

cout <<" animal arrays\n\n";

Array<int> *pIntArray = new Array<int>;

cout << Array<int>::GetNumberArrays() << " integer arrays\n";
cout << Array<Animal>::GetNumberArrays();

cout <<" animal arrays\n\n";

delete pIntArray;

cout << Array<int>::GetNumberArrays() <<" integer arrays\n";
cout << Array<Animal>::GetNumberArrays();

cout <<" animal arrays\n\n";

return 0;

}



===== PAGE 685 =====
684 ee 제3주

겔과 0 integer arrays
0

animal arrays

1 integer arrays
1 animal arrays

2 integer arrays
1 animal arrays

1 integer arrays
1 animal arrays

분석  Animal 클래스의 ANS 지면상 생략하였습니다. 27번 줄에서 408“ 클래스
는 정적 변수 jtsNumberAmays= 추가하였고, 이 ABE ASHE 19번 |S
에서 정적 범용 접근자 GetNumberArrays()7} 추가되었습니다.
정적 자료의 초기화는 완전한 템플릿으로 만들어졌고 이는 30 - 31번 줄에서 보
여졌습니다. Array] 생성자와 소멸자는 각각의 순간에 얼마나 많은 배열이 만들
어졌는지 추적하기 위해 수정되었습니다.

정적 멤버에 접근하는 것은 다른 클래스의 정적 wu] 접근하는 것과 같습니다.
이미 존재하는 객체에 대해 똑같이 할 수 있는데 이는 91 - 92번 줄에 보여졌습
니다. 혹은 85 - 86번 줄처럼 완전한 클래스 BAS 사용하여 할 수 있습니다. 이
정적 자료에 접근할 때 배열의 특수형을 사용해야만 합니다. 각 형에 대해 하나
의 변수가 있습니다.

EAS 만들고 사용하는 WS 배웠습니다. 템플릿은 0++에서 매개 변수
만들기 위해 내장된 기능입니다. 매개 변수에 의거하여 동작을 바꾸는
될 때 전달됩니다. 이렇게 하면 코드를 안전하고 효율성 있게 재



===== PAGE 686 =====
제19일 HEX ee 685

에 마한 2 8의에서 매개 변수화되는 % ee wate 템플릿에 대한 각 인

클래스는 세 개의 형의 프랜드 BSS 선언할 수 있습니다. 비 템플릿, 일
반 템플릿, 형 명세한 템플릿입니다. 템플릿은 정적 자료 멤버를 ade 수 있는데
이는 템플릿의 각 인스턴스가 그 자신의 정적 자료의 집합을 가질 수 있습니다.

실제형에 근거하여 템플릿 함수의 SAS 특수하게 하려면 특정형에 템플릿 함수
를 중복할 수 있습니다. 이는 멤버 합수에도 같이 작용합니다.

Q WAZ} 있는데 템플릿을 쓰는 이유는?
A 템플릿은 형에 대해 안정성을 제공하는 내장된 기능입니다.
템플릿 함수의 매개 변수화된 형과 일반 함수의 매개 변수와의 차이점은 무엇입니까?

A 일반 함수는 동작시킬 수 있는 매개 변수를 취합니다. 템플릿의 함수는 함수에 대
한 특정 매개 tel Be 매개 변수화할 수 있도록 합니다, 즉, 함수의 형의 배열
을 전달하고 탬플릿의 인스턴스에 의해 결정된 Be 가질 수 있습니다.

Q HAZ} 있는데 템플릿을 가지고 고생을 하는 이유는?

A 템플릿은 언어에 통합된 부분이지만 매크로는 아닙니다. 템플릿은 ye 보장하고
매크로는 아닙니다.

(언제 템플릿을 쓰고 언제 상속을 합니까?

A 여러분의 클래스가 행하는 사항의 VS 제외한 모든 동작이 바뀌지 않을 때 템플릿
을 사용합니다. 여러분이 클래스를 복사해 하나 이상의 wy] 형만을 바꾼다든지

 일반 템플릿 프랜드 클래스를 사용할 때는 언제입니까?
A 형과 관계없이 각 인스턴스는 이 클래스 혹은 함수의 프랜드로 사용할 수 있습니다.
Q 언제 형이 상술된 템플릿 프랜드 클래스나 함수를 사용합니까?

A 두 개의 클래스 사이에 일대일 관계를 설립하기를 원할 때입니다. qs 들면
array<int>+= iterator<Animal>°] 아니라 iterator<int>2} 대응해야 합니다.


===== PAGE 687 =====
686 ㅇㅇ 제주

연구
이 연구란에서는 이번 장에서 다루어진 주제를 여러분이 얼마나 잘 이해하였는가

를 확인해보는 퀴즈들과, 배운 것을 시험해 볼 수 있는 연습 문제들로 구성되어
므               로

있습니다. 부록 0에 있는 SE 보기 전에 각 물음에 MS 할 수 있도록 노력하
고, 다음 장으로 넘어가기 전에 답을 충분히 이해하도록 합시다
퀴즈
Ｌ 템플릿과 매크로의 차이점은?
2. 템플릿의 매개 변수와 함수의 매개 변수의 차이점은 무엇입니까?
3. 형명세 템플릿 프랜드 클래스와 일반 템플릿 프랜드 클래스의 차이점은?
# 하나의 템플릿의 인스턴스에 특정 SAS 제공하고 다른 인스턴스에는 제공하지 않는 것
이 가능합니까?
S. 하나의 정적 AS 템플릿 클래스 정의에 넣어둘 때 얼마나 많은 정적 변수를 만들 수

있습니까?

연습 문제

1. 이 클래스 목록에 기반하여 템플릿을 만드시오.

class List
{

public:

List():head(0), tail(0), theCount(0) {}
virtual “ListQ;

void insert( int value );

void append( int value );

int is_present( int value ) const;

int is_empty() const { return head==0; }

int count() const { return theCount; }
private:

class ListCell

£

public:
ListCell(int value, ListCell *cell = 0):val(value), next(cell){}
int val;

ListCell *next;
3;



===== PAGE 688 =====
제19일 템플릿 ee 687

ListCell *head;

ListCell *tail;

int theCount;
3;

2 ㄴ16[(비템플릿형) 클래스 버전에 대한 PHS 작성하시오.
3% 구현에 대한 템플릿 HAS 작성하십시오

4 문자열, Cat, 정수형의 세 개의 목록 AAS 선언하십시오.
$ 버그잡기

List<cat> Cat_List;

Cat Felix;
CatList.append( Felix );
cout << "Felix is " <<

( Cat_List.is present( Felix) )2?"": "not" << "present\n";
6 Listol] 대한 프랜드 operator==S 선언하십시오
% Listo] 대해 프랜드 연산자 ==를 구현하십시오
8. 두 개의 WES 서로 바꾸는 swapoll 대한 템플릿 함수를 구현하십시오



===== PAGE 689 =====


===== PAGE 690 =====
예외 ASHI 오류 처,


===== PAGE 691 =====
690 ee 제3주

서

책     들은 여러분에게 예를 보여주기 위해 작성된 aa  지금까지
는 오류들은 다루지 않았고 이는 A 장의 주제로부터 벗어나지 않기 위함이었습
다               그램의 세계에서는 오류 조건들을 고려해야 ai

me) 사항'이란 eter are

를 어떻게 예외 사항을 사용하며, 어떤 주제들이 기다리고 있을까
를 예외 사항 계층을 어떻게 wee

를 어떻게 예외 사항 들을 오류 처리 방식에 사용할 것인가

를 디버거란 무엇입니까?

버그, 오류, 실수, 프로그램에 녹이 & 때(2006 Rot)

모든 프로그램들은 WIS 가지고 있습니다. 프로그램이 커질수록 WIE 더욱
많아집니다. 마지막에 이 버그들은 고쳐지고 최종 버전이 생기게 되는 것입니다.
이것이 사실이라고 해서 버그가 없는 프로그램을 만드는 것이 프로그램에 있어
최고의 목표는 아닙니다.

소프트웨어 업계에서 큰 프로그램은 당연히 버그도 많고 불안정합니다. 크나큰
프로그램에 있어 가장 큰 지출은 검사와 오류 수정에 따르는 지출입니다. 적은
비용에 안정되고 좋은 프로그램을 만드는 사람이야말로 소프트웨어 업계에 혁명

을 불러일으킬 것입니다.

프로그램을 괴롭히는 수많은 종류의 버그들이 있습니다. 첫 번째는 논리상의
류에서 나오는 버그임니다. 프로그램이 여러분이 요구하는 것을 겉      o|
기는 하지만 알고리즘이 적절하지가 않습니다. 두 번째는 구문입니다. 잘
현과 함수 혹은 틀린 구조를 사용합니다. 이 두 가지가 가장 흔한 오류이
분의 프로그래머들이 찾느라 고생하는 오류들입니다.

많은 연구와 경험들을 토대로 볼 때 개발과정을 지난 뒤 오류를 찾는 것은
은 대가를 치뤄야 합니다. 대가를 적게 치루려면 미리 피해야 합니다. 다음으
가장 적게 대가를 치르는 방법은 컴파일러가 가리킬 때 처리하는 것입니다. 표
0++에서는 컴파일러가 컴파일시 많은 오류 메시지를 출력하게 하고 있습니다.



===== PAGE 692 =====
제20일 예외 사항과 오류 저리 ee 691

오

rlo

wilt 는
112
>

뜨
at
ca
ry
|
Hu

ia
of

수행할 il 나타나는 오류들은 그렇지 않

문상의 오류보다 MA 큰 문제는 기대하지 않았던 동작에 대한 무대책
가령 여러분의 프로그램이 사용자들이 정수를 입력하면 잘 수행을 하나
 임력하면 깨지는 경우입니다. 또는 메모리가 부족하거나 플로피 디스크의
디스크 드라이버에 없거나 혹은 wyo] 끊겼을 때 프로그램이 다운되는 경우 등
입니다.

이들과 전쟁을 벌이기 위해 많은 프로그래머들이 방탄 조끼 같은 프로그램을
들려고 합니다. 이 방탄 조끼 프로그램은 컴파일 실행 이후 괴곽한 pret
의 오류를 미리 사전에 방지한 프로그램이란 뜻입니다.

프로그래머가 코드에서 구문상의 APS 만들어 생긴 오류와 문제를 잘못 인식하
고 푸는 방법을 오해한데서 생긴 논리상의 오류 및 비정상적이나 예상은 할 수

있는 문제인 예외 사항들과 구분해야 합니다.

Ao 279 다 | Oo 게

되 과
—a

x
fu

예외 AFSH(Exception)
17일날 공부하였듯이 프로그래머들은 아주 강력한 컴파일러를 사용하고 one
잡기 위해 assetS 사용하여 조사합니다. AWS 다시 검사하고 논리오류를 찾기
고 검사에 지쳐버립니다.

그러나 예외 사항은 다릅니다. 예외 사항이 나타나는 환경은 줄일 수 없습니다.
미리 대비를 할 수는 있습니다. 여러분의 사용자는 때때로 메모리 부족을 일으킬
수 있고 이때 여러분이 할 수 있는 질문은 BAS 할 것인가 입니다. dese

은 선택이 있습니다.

1, 프로그램이 다운되게 뇌돕니다

2 실상을 알리고 조용히 종료합니다

3. ANS 알리고 사용자로 하여금 장애를 제거하게 한 | 계속 진행하게 합니다
4. 종합적인 USS 취한 후 사용자를 괴롭히지 말고 계속 진행합니다

(++은 예외 사항 처리를 위해 형의 안정성 보장 및 실행시 잘 나타나지는 않지
만 프로그램 수행중 예상할 수 있는 비정상적인 조건들에 대한 종합적인 방식을

제공합니다.


===== PAGE 693 =====
692 ce 제주

‘eA 프로그램(6606 #0[)'이라는 말에 대해
슨 프로그램도 잘 일어나는 현상입니다. 이는 프로그래머의 태만에 의해

해도 몇 개월 뒤 점차 새롭고 이상한 버그들이 나타납니다. 사실 여러분이
Ww

Jo] 떨어지는 경우를 말합니다. 처음에 잘 짜여진 버그 없는 프로그램

이라
취할

은 단지 다시 그 코드로 돌아가 어디가

뜻입         동안 코드를 만져
생소한 것이 될 것입니다. 4       Al 이렇게 코드를 꼬이게 짜고 재앙만 초

예외 AFY(Exception)

C++o]A] 예외 사항이란, 문제가 BYR 코드로부
부분으로 전달되는 객체입니다. 예외 사항의 형태는
를 다루어야 할지, 사용자에게 다시 되돌려지는 내

예외 사항의 배후에 있는 개념은 다음과 같습니다.

를 자원의 할당|메모리 할당, 파일에 접근 제한 겉기]은 프로그램의 매우 낮은 단계에서 이

루어집니다.

m ego) 실패하거나, 메모리 할당이 불가하거나, 또는 파일 접근흘 막을 수 없는 경우 행
해야 할 논리 순서는 사용자와 상호 BRS 통해 이루어지므로 프로그램의 높은 단계에
Af 이루어집니다

B 에의 사항은 자원을 할당하는 코드로부터 오류 ANS 다룰 수 있는 코드에까지 직접 통
로를 제공합니다. 만일 중간 사이에 위치할 수 있는 기능 단계가 있다면, 메모리 할당을
초기화할 수 있는 기회가 주어지겠지만 단지 오류 사항을 전달하기만 하는 코드는 별로
필요하지 않습니다



===== PAGE 694 =====
제20일 예외 사항과 오류 저리 ee 693

에외 사항은 어떻게 사용되는가

ty 블록은 문제를 가질만한 코드 PRS 둘러싸기 위해 만들어집니다.

try
{
SomeDangerousFunction() ;
3
catch BSL ty 블록에서 나타난 예외 사항을 다루는 BES 가집니다
try
1
SomeDangerousFunction();
}
catch(OutOfMemory)
{i
// 특정 조치를 취함
가
catch(FileNotFound)
{
// 또 다른 조치를 AT
}

2 예외 사항이 발생되면 이를 잡
화하거나 사용자에게 적절한 안내를 합니다. (리스트 20.1)에서 나타남

으
af
[o)
= Se
rir
(0)
20
2
2)
=
nua
Hu
tulo
[모
nn
kK
ok
nf
-
Ho

초기

mf
ae
무

새로운 예외 사항, 및 catch 블록
종이   예외 사항 : 문제 사항에 대한 YRS 전달하는데 사용되는 객체
try 블록 : 예외 사항이 일어날 만한 곳을 중괄호로 묶은 블록

catch BS : try 블록 TS] 곧바로 나와 예외 사항을 처리하는 블록

예외 사항이 나타났을 때 프로그램의 통제는 현재의 try 블
즉시 갑니다.

0

에서 catch 블록으로


===== PAGE 695 =====
694 ee 제3주

몇몇 오래된 컴파일러는 이를 지원하지 않습니다. 그러나 예외 사항은 현재의 표준
++의 일부분입니다. 이를 지원하지 않았던 대부분의 주요 컴파일러 공급자들은 다음
버전에 이를 포함하기로 하였습니다. 옛날 버전을 가졌다면 이를 Uae 수는 없지

[리스트 20.1] 예외 사항의 발생

#include <iostream.h>

const int DefaultSize = 10;

{
public:
// 생성작
Array(int itsSize = DefaultSize);
9:   Array(const Array &rhs);
10: “Array() { delete [CJ] pType;}
1106
12   if 원신자
ls   Array& operator=(const Array&);
14:   int& operatorL](int offSet);

0
1
2
Se
4: class Array
5
6
7
8

15%   const int& operator[l(int offSet) const;

16%

17:    // 접근자

18:   int GetitsSize() const { return itsSize; }

193%

20:   // friend function

21:   friend ostream& operator<< (ostream&, const Array&);
Zee

23: class xBoundary 10; // 예외 사항 클래스 정의
24: private:

25%   int *pType;

26:   int itsSize;

208 20)

28:

29:

30: Array::Array(int size):

31: itsSize(size)

32:
55%    pType = new intLCsizel;
S54:    for (int i = 0; i<size; i++)

35:       pTypeLil = 0;



===== PAGE 696 =====
제20일 예외 사항과 오류 저리 ee 695

36: }

378

38:

39: Array& Array::operator=(const Array &rhs)
40: {

42:    if (this == &rhs)

43:      return *this;

44:    delete [] pType;

451    itsSize = rhs.GetitsSize();

46:    pType = new intLitsSizel;

al:    for (int i = 0; i<itsSize; i++)
48:       pTypelil = rhsLlil;

49: }

50%

51: Array::Array(const Array &rhs)

52: 1

Doe    itsSize = rhs.GetitsSize();

54:    pType = new intLitsSizel;

35    for (int i = 0; i<itsSize; i++)
56:      pTypelil = rhslil;

571 7}

58:

59:

60: int& Array::operatorll(int offSet)
61: 《

62:    int size = GetitsSize();

63%    if CoffSet >= 0 && offSet < GetitsSize())
64:      return pTypeLoffSetJ;

65:    throw xBoundary();

66:    return pTypel0O]; // 156 &

of: 3

68:

69:

70: const int& Array::operatorL](int offSet) const
1s £

272:    int mysize = GetitsSize();

(55    if (01156 >= 0 && offSet < GetitsSize())
74:      return pTypeLoffSetI;

C5    throw xBoundary();

76:    return pTypeLO]; // msc 용

(7: F

(8:

79: ostream& operator<< (ostream& output, const Array& theArray)
80: {

81:    for (int i = 0; i<theArray.GetitsSize(); i++)

82:       output << "[" << i << "]_" << theArrayLil << endl;


===== PAGE 697 =====
696 ec 제3주

83:    return output;

84: }

85:

86: int main()

872 £

88:    Array intArray(20);

89:    try

90:    £

941:       for (int j = 0; j< 100; j++)

92:      {[

93:         intArrayLljl] = j;

94:         cout << "intArrayL" << j << "J okay..." << endl;

95%      }

96:    >

90:    catch (Array::xBoundary)

98:    {

99:      cout << "Unable to process your input!\n";

100:   }

101:   cout << "Done.\n";

102:   return 0;

103% | >

결과   intArrayLO] okay...

intArrayLl1] okay...
intArrayL2] okay...
intArrayLl3] okay...
intArrayLl4] okay...
intArrayL[5] okay...
intArrayl6] okay...
intArrayL7] okay...
intArrayLl81] okay...
intArrayL9] okay...
intArrayL10] okay...
intArrayLl111] okay...
intArray[12] okay...
intArrayl13] okay...
intArray[14] okay...
intArray[15] okay...
intArrayL£16] okay...
intArrayL[17] okay...
intArray[18] okay...
intArrayL19] okay...

Unable to process your input!

Done.



===== PAGE 698 =====
제20일 예외 사항과 오류 저리 oe 697

불샐 [ZALES 19잎 날의 템플릿이 기본을 둔 간단한 Amy 클래스를 제공
~ 합니다. 23번 줄에서 새로운 클래스가 포함됩니다.

이 새로운 클래스는 보기에는 예외 사항으로 분류되지 않았습니다. 다른 클래스

와 마찬가지입니다. 이 클래스는 간단합니다. ASE 없고 메쏘드도 없습니다. 그

럼에도 불구하고 클래스는 클래스입니다.

사실 메쏘드가 없다는  ate os 것인데 왜냐하면 컴파일러가 생성자, 소멸자, 복

를 자동으로 제공하기 때문입니다. 따라서 이미

지만 자료는 없습니다.

Array A] 선언하는 것은 두 개의 클래스를 we 기능을 합니다. 15일날 이야기하
웃이 Array= xBoundaryol] 특별한 접근자가 없고 또 xBoundary Array 멤버에

의 특별한 접근자가 없습니다.

60 - 66번 줄 및 70 - 77번 줄에서 변위 연산자가 요청된 변위를 살펴보기 위해
수정되었고 이것이 WAS 벗어나면 예외 사항으로 xBoundary SAAS 일으킴니
다. xBoundary 생성자의 006 호출과 나열형 상수의 사용을 구별하기 위해 중괄호
가 사용되었습니다. 마이크로소프트에서는 선언과 일치시키기 위해 retun(}7]]
는 정수 FAVS 제공하였습니다. 물론 OF 줄에서 예외 사항이 발생하여 66번
줄에 도달하지 않더라고 말입니다.
89번 줄에서 예약어 try7} wy 블록의 시작을 알리고 96번 줄에서 끝났습니다. 이
록에서 88번 줄에서 선언이 된 배열에 100개의 정수가 추가되었습니다.

97번 줄에서 xBoundary 예외 사항을 잡기 위한 catch 블록이 선언되었습니다.
86 - 103의 구동 프로그램에서 배열의 각 멤버를 초기화하는 부분이 try 블록 안
에 선언되었습니다. 91번 줄의 ]가 20으로 증가할 때 변위 20의 멤버가 접근되려
하고 이는 63번 줄에서 오류를 발생시키고 00600104[]는 65번 줄에서 xBoundary 예
S| 사항을 불러일으킴니다.

램의 SAS 97번 줄의 catch 블록으로 가고 예외 사항이 감지되고 처리됩
4 0 기 더     ae 출력합니다. 프로그램의 흐름은 100번 S2] catch B
의 끝

te 드 i

}니다.

버


===== PAGE 699 =====
698 ec 제3주

try 블록과 catch 블록

try 블록 - try SSS 문장의 집합이 라는 예약어로 시작되고 시작 중괄호로 열린 뒤
마감 중괄호로 끝남니다
예제
try
{
Function();
3;
catch 블록 - 일련의 문장이 catch 시작한 뒤 괄호 안에 예외 사항의 종류가 나오고
시작 중괄호 마감 중괄호로 끝납니다.
예제
try
인
Function();
3;
catch (OutOfMemory)
4
// 조치가 행레짐
+

록을 어디에 사용하는지는 간단한 문제는 아닙니다. 어떤 동작이 예외 사항
불러일으킬지는 분명하지가 on 다음 문제는 어디에 예외 사항을 설정
하는가 입니다. 메모리가 할당되는 모든 곳에서 메모리 예외 사항을 호출하고
기도 할 것입니다. 하지만 예외 ABS 잡는 KE 사용자와 인터페이스하는 부
입니다.

eae

try 22 catch S59] aia
try

Ac

언제 ty 블록을 시도할지는 자원을 할당하는 곳을 살펴봅시다. 또 범위를 검사하
는 곳, 잘못될 가능성이 있는 입력 부분 SS 살펴봅시다

예외 사항 잡기((하아108 Exception)
어떻게 동작하는지 봅시다. 예외 사항이 일어났을 때 호출 et stack)o] 살펴
집니다. 호출 스택은 하나의 프로그램 부분에서 다른 함수를 호출하였을 때 만들
어지는 함수의 목록입니다.



===== PAGE 700 =====
제20일 예외 사항과 오류 저리 ee 699

호출 스택은 실행 과정을 주적합니다. 2800이 Animal::GetFavoriteFood) = 호출하고
GetFavoriteFood()= _Animal::LookUpPreferences()= 호출하고 이는 fstream::operator>>()
= 호출한다 할 때 이 모두가 호출 스택에 잡힙니다. 자기 호출의 경우는 호출
스택에 매우 많이 잡힙니다.

예외 사항은 마감 중괄호를 만날 때 호출 스택에 저장이 됩니다. 스택이 되플릴
때 스택 상에 있는 각 지역 객체의 소멸자들이 호출되고 객체는 소멸됩니다

하나의 ty 블록 다음에 하나 이상의 catch 블록이 옵니다. 예외 사항이 하나의
cach 문장과 일치하면 그 문정들이 AWTS 의미합니다. 일치하는 부분이 없으
면 스택은 계속 풀려집니다.

구동 프로그램이 끝나도록 예외 사항이 잡히질 않으면 내장된 예외 사항 처리
로그램이 호출되어 프로그램을 끝냄니다. 예외 사항이 스택에서 풀리는 것은
일한 과정임을 알아야 합니다. 진행이 되면서 스택이 풀리고 스택 상의 객체
소멸됩니다. 뒤로 돌아가는 것은 없고 일단 예외 사항이 다루어지면 프로그램
0 블록 뒤의 해당 예외 사항을 다루는 catch 문장을 시작합니다.

ro rir fe

따라서 [리스트 20.1]에서 실행은 101번 줄에서 재개됩니다. 4, wy 블록 후
×83000080/를 다루는 catch 블록 다음입니다. 예외 사항이 나타났을 때 프로그램의
pee  atch 블록 다음으로 가지 예외 사항이 일어난 다음 줄로 가지 않음을 명

하나 이상의 63대문

하나 이상의 ZA] 예외 사항을 일으킬 수 었습니다. 이 경우 마치 switch 문장
과 같이 하나 이상의 catch 블록이 YAS 수 있습니다. enna 같은 문장이
“catch everything - 나머지 모든 예외 사항을 잡아라”입니다. 이는 catch(..) 형태로
지정됩니다. [리스트 20.2]를 봅시다.

[리스트 20.2] 다중 예외 사항

0: #include <iostream.h>

We

2: const int DefaultSize = 10;
3s

4: class Array

5: ¢

6: public:

Ce

// 생성자


===== PAGE 701 =====
700 ee 제3주

8:

10:
1%
12:
132
14:
15%
165
i WA
185
19
20:
212
22:
25%
24:
25:
26:
ers
28:
29:
30:
St:
32:
345
34:
35:
56:
37%
38:
39:
40:
41:
42:
43:
44:
ASS
46:
47:
48:
49:
50:
318
528
53%

Array(int itsSize = DefaultSize);
Array(const Array &rhs);
“~Array() { delete [] pType;}

// 연산작

Array& operator=(const Array&);

int& operatorL](int offSet);

const int& operatorL](int offSet) const;

// 접몬작
int GetitsSize() const { return itsSize; }
// 프랜드 함수

friend ostream& operator<< (ostream&, const Array&);

// 예외 사항 클래스 정의
class xBoundary {};
class xTooBig {};
class xTooSmall{};
class xZero {};
class xNegative {};
private:
int *pType;
int itsSize;
3;

int& Array::operatorLi(int offSet)
{
int size = GetitsSizeQ);
if CoffSet >= 0 && of fSet < GetitsSize()
return pTypeLoffSet];
throw xBoundary();
return pTypeLO]; // msc &

const int& Array::operatorlL](int offSet) const
{
int mysize = GetitsSizeQ;
if (offSet >= 0 && offSet < GetitsSizeQ)
return pTypeLoffSetJ;
throw xBoundary();

return pTypel0J;   // 056 &



===== PAGE 702 =====
제20일 예외 사항과 오류 저리 ee 701

54:
55: Array::Array(Cint size):
56: itsSize(size)

578) 4

58:   if (size == 0)

598      throw xZero();

60:   if (size < 10)

61:      throw xTooSmall();

62:   if (size > 30000)

63%      throw xTooBig();

64:   if (size < 1)

65:      throw xNegative();

66:

67:   pType = new intLsizel;

68:   for (int i = 0; i<size; i++)
69:      pTypeLil] = 0;

70: }

1:

2s

(3:

74: int main()

(oe £

76:

tts   try

(8:   a

79:     Array intArray(0);

80:      for (int j = 0; j< 100; j++)
81:      {

82:        intArrayLj] = j;

83:        cout << "intArrayL" << j << '"] okay..." << endl;
84:      }

85:   0]

86:   catch (Array::xBoundary)

87:   {

88:      cout << "Unable to process your input!\n";
89:   }

90:   catch (Array::xTooBig)

915   {

92:      cout << "This array is too big..." << endl;
93:   }

94:   catch (Array::xTooSmall)

95:   {

96:      cout << "This array is too small..." << endl;
97:   +

98:   catch (Array::xZero)
99%   {



===== PAGE 703 =====
702 ee 제3주

100:     cout << "You asked for an array of zero objects!" << endl;
1012 +

(02: icateh Cs.)

1032 i

104:     cout << "Something went wrong, but I've no idea what!" << endl;
105-2 i}

106: cout << "Done.\n";
108: return 0;
109:}

결과  You Asked for an array of zero object!

Done.
분석  모든 Amay)] 메쏘드의 구현(생성자를 제외하고)은 [리스트 20.1]과 같으므
로 제외되었습니다.

24 - 27번 줄에서 4개의 클래스 - xTooBig, xTooSmall, xZero, xNegative - 가
어졌습니다. 55 - 70의 생성자에서 생성자로 전달된 크기가 검사되었습니다.
크거나, 작거나, 0이거나, 음수이면 예외 사항이 발생됩니다.

try 블록 다음의 catch 블록이 각 조건을 포함하도록 바뀌었는데 단 음수인 경
는 102번 줄의 0000(_)에서 잡히게 되어 있습니다.

배열의 여러 크기 BS 주어 이를 시도하여 봅시다. -5를 주면 xNegative7} 호출
되리라 기대하는데 실제는 size < 10의 생성자 부분에서 먼저 걸립니다. 이를 수
정하기 위해 60 및 61번 SS 649} 65로 바꿈시다.

또 (들
so aun

4o

oO] 사항 계중 구조
예외 사항도 클래스이므로 그들은 파생이 가능합니다. xSieS 만든 뒤 여기로부
터 xZero, xTooSmall, xTooBig, xNegativeS 만들 수 있습니다. 따라서 어떤 함수들
은 xSize 오류에 잡힐 수 있고 다른 함수들은 ×9126에 잡힐 수 있습니다. [리스트

20.3]을 봅시다.

[리스트 20.3] 클래스 계충과 예외 사항

0: #include <iostream.h>

16

2: const int DefaultSize = 10;
3:

4

class Array



===== PAGE 704 =====
제20일 예외 사항과 오류 처리 ee 703

CON OW

118
12:
133
14:
15¢
16:
Ve:
18:
Ge
20:
ale
22
25%
24:
25%
26:
are
28:
29%
50:
Ss
2321
55%
34:
35
36:
Sr
38:
59%
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:

{
public:
// 생성자
Array(int itsSize = DefaultSize);
Array(const Array &rhs);
“Array() { delete [] pType;}

// 연산자

Array& operator=(const Array&);

int& operatorLl(int of fSet);

const int& operatorL](int offSet) const;

// Oa"
int GetitsSize() const { return itsSize; }

// 프랜드 함수
friend ostream& operator<< Costream&, const Array&);

// 예외 사항 클래스 정의
class xBoundary {};
class xTooBig : public xSize {};
class xTooSmall : public xSize {};
class xZero : public xTooSmall {};
class xNegative : public xSize ts
private:
int *pType;
int itsSize;
3;

int& Array::operatorL](int offSet)

{
int size = GetitsSize();
if (01156 >= 0 && offSet < GetitsSize())
return pTypeLoffSetJ;
throw xBoundary();
return pTypeLO]; // msc £
+

const int& Array::operatorLl(int offSet) const
6
int mysize = GetitsSize();
if (07156 >= 0 && offSet < GetitsSize())
return pTypeLoffSetI;
throw xBoundary();


===== PAGE 705 =====
704 ee 제주

511
5005
528
54:
555
562
a8
58:
Dos
60:
61:
62:
63:
64:
65:
66:
60:
68:
69:
708
1s
te:
(3:
74:
38
16:
Cle
182
192
80:
81%
82:
83:
84:
85:
86:
87:
88:
89:
90:
91:
92:
95:
94:
955
96:

return 01>706ㅁ023;   // Msc 용

Array::Array(int size):
itsSize(size)
《:
if (size == 0)
throw xZero();
if (size < 10)
throw xTooSmall();
if (size > 30000)
throw xTooBig();
if (size < 1)
throw xNegative();

pType = new intLCsizel;
for (int 1 = 0; i<size; i++)
pTypeLil = 0;

int mainQ
{

try
{
Array intArray(0);
for (int j = 0; j< 100; j++)
{
intArrayljl] = j;
cout << "intArrayL" << j << "J okay..." << endl;

가
catch (Array::xBoundary)
{
cout << "Unable to process your input!\n";
}
catch (Array: :xTooBig)
{
cout << "This array is too big..." << endl;
}
catch (Array::xTooSmall)
{
cout << "This array is too small..." << endl;



===== PAGE 706 =====
제20일 예외 사항과 오류 저리 ee 705

97°   a

98:   catch (Array::xZero)

99:   {

100:     cout << "You asked for an array of zero objects!" << endl;
1012 +

102: (catch ¢....)

1038 <

104:     cout << "Something went wrong, but I've no idea what!" << endl;
105: }

106: cout << "Done.\n";
108: return 0;
109:}

결과  This array is too small...

Done.

EM AM 주요한 번화는 25 - 28번 줄입니다. 클래스의 계층 구조가 있습니다. 클래스
a    xTooBig, xTooSmall, xNegative7} ×5126로부터 파생되었고 xZero%= xTooSmall
로부터 파생되었습니다.

Array7} 크기 0으로 만들어졌는데 이것은 FAS 의미합니까? 잘못된 예외 사항
은 잡히게 마련입니다. catch 블록을 자세히 살펴보면 xZero 예외 사항을 살펴보
기 전 <[005001을 살펴봅니다. xZero 객체가 발생되고 xZerot= 《1005041의 한

종류이기 때문에 *[00500에 의해 잡힙니다. 일단 잡히면 다른 처리기를 통과하
지 못하기 때문에 <260는 영원히 호출되지 않습니다.

이의 해결 방법은 처리기를 잘 배열하는 것인데 특수한 처리기를 먼저 놓고 그 다
음을 나중에 놓습니다. 이 예에서는 <2600와 <10050001을 바꾸어 놓아야 합니다.

i"

띠

예외 사항의 자료와 예외 사항 랙체 작명법

종종 여러
는지 이상
여러분은

고 그 자료를 읽을 수 있

| 알맞게 대응하기 위해 어떤 형태의 예외 사항이 발생되었
싶을 것입니다. 예외 사항의 클래스는 다른 클래스와 같습니다.
제공할 수 있고 생성자에서 그 ABE 초기화할 수 있
니다. [리스트 2044에서 이를 보여줍니다.

2 tio AL
O40 lo
EI fo

a5   ful

[리스트 20.4] 예외 AY 랙체를 통해 자료 얻기

0: #include <iostream.h>
1:


===== PAGE 707 =====
706 ce

제3주

CONOU HW DY

118
128
13:
14:
15%
16:
17:
18:
19:
20:
21:
22:
2s:
24:
25%
26:
27:
28:
29:
$0:
$1
3258
33:
54:
35:
36:
Sr:
38:
3905
40:
41:
42:
43:
44:
45:
46:
47:

const int DefaultSize = 10;

class Array

publics

// 생성자

Array(int itsSize = DefaultSize);
Array(const Array &rhs);

“Array() { delete [4 pType;}

// 원산작

Array& operator=(const Array&);

int& operator[l](int offSet);

const int& operatorLl](int offSet) const;

// 접근자
int GetitsSize() const { return itsSize; }

// 프랜드 함수
friend ostream& operator<< (ostream&, const Array&);

// 예외 사항 클래스 정의
class xBoundary {};
class xSize
{
public:
xSize(int size):itsSize(size) {}
“xSize(){}
int GetSize() { return itsSize; }
private:
int itsSize;
3;

class xTooBig : public xSize
{
public:
xTooBig(int size) :xSize(size) {}
3;

class xTooSmall : public xSize
t
public:
xTooSmall (int size) :xSize(size) {}
3;

class xZero : public xTooSmall


===== PAGE 708 =====
제20일 예외 사항과 오류 저리 ee 707

48:
49:
50:
at:
52:
55:
54:
55:
56:
av:
58:
59:
60:
61:
62:2
635:
64:
65%
66:
67:
68:
69:
70:
1s
2:
73:
74:
135
76:
VCs
78:
79:
80:
813
82:
83:
84:
85:
86:
87:
88:
89°
90:
918
92:
93:

{
public:

xZeroCint size) :xTooSmall (size) {}
i;

class xNegative : public xSize
{
public:
xNegative(int size):xSize(size) {}
3;

private:
int *pType;
int itsSize;
3;

Array::Array(int size):
itsSize(size)
{
if (size == 0)
throw xZero(size);
if (size > 30000)
throw xTooBig(size);
if (size <1)
throw xNegative(size);
if (size < 10)
throw xTooSmall (size);

pType = new intLCsizel];
for (int i = 0; i<size; i++)
pTypeLil] = 0;

int& Array::operatorL](int offSet)
HC
int size = GetitsSize();
if CoffSet >= 0 && offSet < GetitsSize())
return pTypeLoffSet];
throw xBoundary();
return pTypeL0];   // MSC &
}

const int& Array::operatorLll(int offSet) const
{



===== PAGE 709 =====
708 ㅇㅇ 제주

94:    int mysize = GetitsSize();

95:    if (offSet >= 0 && offSet < GetitsSize())

96:      return pTypeLoffSet];

or:    throw xBoundary();

98:    return pTypeLOJ;   // Msc 용

99: +

100:

101: int main()

102: 호

103:

104:    try

105:    {

106:      Array intArray(9);

107:       for (int j = 0; j< 100; j++)

108:      {

109%         intArrayljl] = j;

110:         cout << "intArrayL" << j << "J okay..." << endl;
V1:      }

112:    }

1138    catch (Array::xBoundary)

1143    5

115:       cout << "Unable to process your input!\n";

116:    a

117:   catch (Array::xZero theException)

118:   {

119:      cout << "You asked for an array of zero objects!" << endl;
1205      cout << "Received " << theException.GetSize() << endl;
1212   0

122:   catch (Array::xTooBig theException)

1238

124:      cout << "This array is too big..." << endl;

125s      cout << "Received " << theException.GetSize() << endl;
126:   D

127%   catch (Array::xTooSmall theException)

128:   {

129:      cout << "This array is too small..." << endl;

130:      cout << "Received " << theException.GetSize() << endl;
131:   }

132:   catch (.«.)

1338:   {

134:      cout << "Something went wrong, but I've no idea what!" << endl;
155%   버

136:   cout << "Done.\n";
137 e   return 0;
1388 |)



===== PAGE 710 =====
세20일 예외 사항과 오류 저리 ee 709

겔과  This array is too small...
Received 9
Done.

분석  ×5126의 선언이 32번 줄에서 멤버 변수 195126를 가지도록 수정되었고, 30번

- 줄에서 멤버 함수 009080를 가지도록 바뀌었습니다. 추가하여 28번 줄에
서 정수형을 가지고 멤버 변수를 초기화하는 생성자가 추가되었습니다.

초기화하고 아무 일도 안하는 생성자를

선언하였습니다. a9) 선언은 a 따라서 지면을 절약하기 위해 신지

113 - 135의 catch 블록이 이름을 갖도록

자료를 접근하도록 이 객체를 사용하였습

정되었고(468%060000) 169126에 저장된
다.

드 4

예외 사랑을 만들 때 예외 사항이 발생했다라는 사실을 명심합시다. 무엇인가가 잘못
된 것이고 따라서 여러분의 예외 사항 안에서 이 같은 문제가 = 발생하지 않도록 주
의합시다. 여러분이 OutOf{Memory 예외 사항을 만들면 그 생성자에서 = 메모리를 할
당하지 않도록 합시다.

각각의 catch 블록이 출력 메시지를 내보내는 것은 따분       . 이 일은 객
체에 속하는 것인데 객체는 어떤 Yo] 객체이고 어떤 Ye 받는지를 압니다. [리
스트 25 가상 BEES 사용하여 예외 사항이 올바른 일을 하도록 하여 이 문
제에 대해 좀더 객체 지향적인 접근 방식을 취합니다.

lo    rou
ne,
ro,
ay
토해

ye

[리스트 20.5] 예외 사항에서 잠조자를 전달하고 가상 BAS 사응함

#include <iostream.h>

const int DefaultSize = 10;

0

1

2

3:

4: class Array
a: 섹

6: public:

7    // 생성자

8:    Array(int itsSize = DefaultSize);
93    Array(const Array &rhs);

10:   “Array() { delete [] pType;}

118

125  // 연산자


===== PAGE 711 =====
710 ee ABS

13%

150

Se:
33%
34:
35.
36:
Sf:
38:
39:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
D1
525
538
54:
532
56:
af
58:

Array& operator=(const Array&);
int& operatorLl](int offSet);
const int& operatorLI](int offSet) const;

// aS
int GetitsSize() const { return itsSize; }

// SHE 함수

friend ostream& operator<< (ostream&, const Array&);

// 예외 사항 클래스 정의
class xBoundary {};
class xSize
{
public:
xSize(int size):itsSize(size) {}
“xSize() {}
virtual int GetSize() { return itsSize; }
virtual void PrintError()
{
cout << "Size error. Received: ";
cout << itsSize << endl;
}
private:
int itsSize;
};

class xTooBig : public xSize
{
public:
xTooBig(int size) :xSize(size) {}
virtual void PrintError()
{
cout << "Too big! Received: ";
cout << xSize::itsSize << endl;
}
3;

class xTooSmall : public xSize
{
public:
xTooSmall (int size) :xSize(size) {}
virtual void PrintError()
{
cout << "Too small! Received: ";
cout << xSize::itsSize << endl;



===== PAGE 712 =====
제20일 예외 사항과 오류 저리 ee 711

59:
60:
61:
62:
63:
64:
65::
66:
67:
68:
69:
70:
“13
72:
(3:
74:
ton
(6:
Cl:
78:
19:
80:
81%
82:
83:
84:
854
86:
87:
88:
89:
90:
91:
92:
95:
94:
956
96:
90:
98:
99:

100:
101:
1023
103:
104:

}
03:

class xZero : public xTooSmall
{
public:
xZero(int size) :xTooSmall (size) {}
virtual void PrintError()
a6
cout << "Zero! Received: ";
cout << xSize::itsSize << endl;
}
3;

class xNegative : public xSize
{
public:
xNegative(int size):xSize(size){}
virtual void PrintError()
+t
cout << "Negative! Received: ";
cout << xSize::itsSize << endl;
}
3;

private:
int *pType;
int itsSize;
3;

Array::Array(int size):
itsSize(size)
£
if (size == 0)
throw xZero(size);
if (size > 30000)
throw xTooBig(size);
if (size <1)
throw xNegative(size);
if (size < 10)
throw xTooSmall (size);

pType = new intLsizel;
for (int i = 0; i<size; i++)
pTypeLil = 0;


===== PAGE 713 =====
712 ee 제3주

105:
106:
107:
108:
109:
110:
111:
1126
113:
114s
1153
116:
TUL
118:
119:
120:
21s
1223
125%
124:
125%
126:
120:
128:
129:
130%
1351:
W522
133:
134:
1355:
136:
150%
138:
139:
140:
141:
142:
143:
144:
145:
146:
147:
148:
149:
150:

int& Array::operatorL](int offSet)

{
int size = GetitsSize();
if (offSet >= 0 && offSet < GetitsSize())
return pTypeLoffSetJ;
throw xBoundary();
return pTypeLO]; // MSC 용
가
const 1018 Array::operatorL](int offSet) const

{
int mysize = GetitsSizeQ;
if CoffSet >= 0 && offSet < GetitsSize())
return pTypeLoffSetl;
throw xBoundary();
return pTypeL0J;   // msc &

int main()
{

try
{
Array intArray(9);
for (int j = 0; j< 100; j++)
{
intArrayLljl] = j;
cout << "intArrayL" << j << "J okay..." << endl;

}
catch (Array::xBoundary)
AE
cout << "Unable to process your input!\n";
}
catch (Array::xSize& theException)
ai
theException.PrintError();
}
Catch (= =
{
cout << "Something went wrong!\n";
}
cout << "Done.\n";



===== PAGE 714 =====
제20일 예외 사항과 오류 처리 ee 713

151:   return 0;
1528 J

겔과  Too small! Received 9

Done.

분석 [리스트 20.5]는 ×5126에서 가상 메쏘드를 선언하였습니다. 이 메쏘드는
1000300[0로 오류 문장을 출력하고 클래스의 실제 크기를 출력합니다. 이
는 각각의 파생 클래스에서 중복됩니다.
142번 줄에서 예외 사항 객체가 AAAS 선언되었습니다. 800080000가 객체에
대한 FAAS 호출되었을 때 다형성이 200080000의 올바른 버전이 호출되도록
합니다. 코드가 깨끗해지고 이해하기 쉬워지며 유지 보수가 쉽게 됩니다.

예외 사앙과 HBS
템플릿을 가지고 일하는 예외 사항을 만들 때 여러분
릿의 각 인스턴스에 예외 사항을 만들 수
언된 예외 사항 클래스를 사용할

+
See?
ry
Ey
* i
ies
> 껄
고 ro
S 때
나 0
Pa
mt 26 wl
= 0
도
ny,
=z
eS
Ps

[리스트 20.6] 예외 사항을 HSS D 같이 사응

1: #include <iostream.h>

21

3: const int DefaultSize = 10;

4: class xBoundary {};

Die

6: template <class T>

7: class Array

8: 6

9: public:

10:    // 생성자

We    Array(int itsSize = DefaultSize);
12:    Array(const Array &rhs);

13?    “Array(Q) { delete [] pType;}

14:

15:    // 연산자

16%    Array& operator=(const Array<T>&);
1:    T& operatorLi(int offSet);

18:    const T& operatorL[](int offSet) const;


===== PAGE 715 =====
714 ee 제3주

198
20%
21
22:
25%
24%
25
26:
27:
28:
29:
30:
51:
$22
53:
34:
55%
368
St:
38:
39
40:
Als
42:
43:
44:
45:
46:
47:
48:
49:
DU:
a1¢
52:
95%
54:
508
56:
57:3
58:
59s
60:
61%
62:
635:
64:

ff 접근작
int GetitsSize() const { return itsSize; }

// 프랜드 함수
friend ostream& operator<< (ostream&, const Array<T>&);

// 예외 사랑 클래스 정의
class xSize {};

private:
int *pType;
int itsSize;
};

template <class T>
Array<T>::Array(int size):
itsSize(size)
af
if (size <10 || size > 30000)
throw xSizeQ);
pType = new TLsizel;
for (int i = 0; i<size; i++)
pTypeLil = 0;

template <class T>
Array<T>& Array<T>::operator=(const Array<T> &rhs)
{
if (this == &rhs)
return *this;
delete [03 pType;
itsSize = rhs.GetitsSizeQ;
pType = new TLitsSizel;
for (int i = 0; i<itsSize; i++)
pTypeLil = rhslid;
Bs
template <class T>
Array<T>::Array(const Array<T> &rhs)
{
itsSize = rhs.GetitsSizeQ;
pType = new TLitsSizel;
for (int 1 = 0; i<itsSize; i++)
pTypeLil = rhslid;



===== PAGE 716 =====
제20일 예외 사항과 오류 저리 ee 715

65%
66:
67:
68:
69:
70:
ate
ler
738
74:
21
76%
778
783
hue
80:
81:
82:
83:
84:
85:
86:
87:
88:
89:
90:
918
92:
9S:
94:
95:
96:
97:
98:
99:

100:
101:
102:
103:
104:
1.05%
106:
107:
108:
109:
1108

template <class T>
T& Array<T>::operatorLi(int of fSet)
{
int size = GetitsSize();
if (CoffSet >= 0 && offSet < GetitsSize())
return pTypeLoffSet];
throw xBoundary();
}

template <class T>
const T& Array<T>::operatorL[l](int of fSet) const
{
int mysize = GetitsSize();
if (offSet >= 0 && offSet < GetitsSize())
return pTypeLoffSet];
throw xBoundary();
J

template <class T>
ostream& operator<< (ostream& output, const Array<T>& theArray)
{
for (int i = 0; i<theArray.GetitsSize(); i++)
output << "[" << i << 03 " << theArrayLi] << endl;
return output;
}

int main()
{

try
af
Array<int> intArray(9);
for (int j = 0; j< 100; j++)
+
intArraylj] = j;
cout << "intArrayL" << j << "J okay..." << endl;
as
개
catch (xBoundary)
€
cout << "Unable to process your input! \n";
}
catch (Array<int>::xSize)
{


===== PAGE 717 =====
716 ee AB

11413      cout << "Bad Size!\n";
1122   01

113:

114:   cout << "Done.\n";

115: return 0;

116: +}

24 il Bad Size!

Done.

불셀 저유의 이의 사항인 xBiunday7} 4번 oA 팀플릿의 바깥에서 선언되었습
니다. 두 번째의 예외 사항 xSize7} 템플릿의 내부에서 선언이 되었습니다.

xBoundary2} 예외 사항은 템플릿 클래스에 엄매이지 않고 인스턴스화된 4085에
기반 하여 호출되어야 합니다. 두 개의 catch 블록의 구문 차이를 볼 것입니다.
105줄은 catch(xBoundary)= 보여주고 109번 Be catch(Array<int>::xSize)z} 되어
있습니다. 후자는 정수형 배열의 인스턴스에 Ame} 있습니다.

오류가 없는 예외 사항

0++의 도사들이 일과 후 사이버 스페이스라는 가상 맥주 집에 모였을 때 예외
사항들이 일반적인 조건에서도 쓰일 수 있는지에 대한 이야기를 하고 있었습니
다. 한쪽의 주장은 속성상 예외 사항은 예상할 수 있지만 이름 그대로 프로그래
머들이 예상할 수 있는 예외 사항의 환경에 쓰여야 하고 이는 정상적인 코드의
부분에 쓰여서는 안된다고 하였습니다.

른 쪽 주장은 다음과 같습니다. 예외 사항이 메모리의 누출 없이 여러 단계의
함수를 통해 매우 강력하고 좋은 방식을 제공합니다. 흔한 예는 다음과 같습니다.
사용자가 001 환경에서 행동을 요청합니다. 요청을 잡는 코드의 부분은 다이얼로
그의 관리자에게 멤버 함수를 호출해야 하고, 이는 요청을 처리하는 프로세스를
차례로 호출하며, 다음에는 어떤 대화 상자를 사용할지를 결정하는 SES 호출
하고, 다음에는 대화 상자를 그리는 SES 호출하고, 마지막으로 사용자의 입력
을 처리하는 SES 요청합니다. 만일 사용자가 ASS 하면 SEE 맨 처음의
메쏘드를 호출해야 하고 여기서 원래의 요청이 다루어집니다.

이를 해결하는 방식의 하나는 sy SSS 원래의 호출에 넣고 예외 사항으로
CancelDialog 넣는데 이는 사용자가 취소 단추를 누를 때 처리기에 의해 불리어



===== PAGE 718 =====
제20일 예외 사항과 오류 저리 ㅇㅇ 717

집니다. 이것이 안전하고 효율적인 방법입니다. 하지만 취소 단추를 누르는 것은
일반적인 환경이지 예외 사항은 아닙니다.

이는 종종 신념에 관련된 논쟁인데 그래도 요점적인 질문을 만들 수 있습니다.
에의 사항의 사용이 SES 이래하기에 쉽거나 어럽게 만듭니가 오류나 메모리
누출을 만드는 위험성 등이 있지나 않는지요? 이 코드를 유지 보수하다 쉽거나
어렵게 하지 않습니까? 이러한 결정들이 다른 문제들과 마찬가지로 분석을 요구
하는데 하나의 답은 없지만 올바른 답은 있을 것입니다.

버그와 디버깅

17일째에서 asset 사용하여 실행시 버그를 확인하는 YS 보았는데 ese 실
행시 문제를 잡기 위해 예외 사항을 사용하는 것을 봅시다. 버그를 공격하기 위
한 뛰어난 무기인 디버거입니다.

최근의 모든 개발 환경들은 강력한 디버거를 가지고 있습니다. 디버거의 기본 개
넘은 이렇습니다. 디버거를 수행합니다. 이는 여러분의 원시 코드를 올립니다. 그
리고 여러분은 디버거 안에서 프로그램을 AMM yc. 이렇게 하면 여러분의
프로그램이 실행되면서 그 코드를 볼 수 있습니다.

= 컴파일러는 특정 기호를 주거나 뒤 컴파일을 할 수 있습니다. 이 기호를
으면 실행시 실행 부분과 원시 코드 사이의 BS 하게 합니다. 디버거는 원
코드의 특정 위치와 프로그램의 다음 동작을 연결합니다.

단위에서 기동되는 디버거는 이 작업을 즐겁게 해줍니다. 디버거를 올리
Aes] 모든 원시 코드를 통해 읽고 이를 화면에 보여줍니다. 각 함수의 호
AVA 밝아 나갈 수 있습니다.

의 디버거에서 원시 코드와 각 실행문의 결과를 보기 위한 출력 사이를 오
{습니다. 더 나아가 각 변수의 현재 상태를 볼 수도 있고 복잡한 자료 구
있으며 클래스의 각 멤버 자료도 볼 수 있습니다. 또 각 포인터 및 메
위치의 ke 볼 수 있습니다. 여러분은 또 몇몇 SH] 통제를 행할 수 있는
기점 설정, 경계점 설정, 메모리 보기, 어셈블러 코드 보기가 그것입니다.

at
년
roy

=,

UN (묘 (조
fou,
[묘

ito   은
[월 .모
쪽

0

fd PN oN a
4
one x0 Fs

© eo

데

= 1/4 (Breakpoint)

분기점은 더버기이게 내리는 특정 줄의 코드의 실행 준비가 되면 =e
지시키    명령입니다. 이는 문제가 되는 So] 도달할 때까지 방해받지 않고


===== PAGE 719 =====
718 ee 제3주

로그램을 실행시킬 때 사용됩니다. 미묘한 줄의 전후에서 특정 변수값을 보거나
분석을 할 수 있게 합니다.

경계점(\하아 Point)
특정 변수의 BS 보여주게 하거나 변수가 입출력되었을 때 멈추게 할 수 있습니
다. 경계점은 이 점들을 설정할 수 있고 프로그램을 실행시키면서 변수값을 바꿀
수 있습니다.

메모리 살펴보기

실제 메모리에 있는 값을 보는 것도 중요합니다. 현대의 디버거는 실제 변수의
값을 보게 ila 문자열은 문자들로 1008형은 그 길이대로 BA 합니다. 어떤
0++은 클래스를 그대로 보게 하고 006를 포함하여 각 멤버 변수의 현재 eS 보
게 합니다.

어셈블러
원시 코드를 통해 읽는 것이 WIS 잡는 데 필요한 i 이지만 이것이 실패할
땐 때로는 a 원시 코드에서 생성되는 suds He 것도 필요  합니다. 메모리
의 레지스터, 플래그 등 깊이 들어갈 필요가 있습니다.
디버거 사용법을 익힙시다. 버그와의 전쟁에서 가장 강력한 무기가 됩니다. 실행
버그는 잡기가 힘들고 없애기가 힘듭니다. 좋은 디버거가 이를 해결합니다. 비록
쉽지는 않지만 대부분을 찾게 해줍니다.

오늘은 어떻게 예외 사항을 만들고 사용하는지 배웠습니다. 예외 사항은 만들어
지고 또한 예외 환경이나 오  오류가 일어나는 부분에서 실행 프로그램이 처리하지
못하는 부분을 다루는 객체입니다. 프로그램의 다른 부분인 호출 스택의 위 부분
에서 예외 사항을 잡고 적절한 행위를 가하는 catch BSS 구현합시다.

예외 사항은 일반적인 사용자가 만든 객체이고, 값이나 참조자로 전달될 수 있습
니다. 자료나 메쏘드를 가질 수 있고 catch BSS 그 예외 사항을 다루기 위해
자료를 사용할 수 있습니다.



===== PAGE 720 =====
제20일 예외 사항과 오류 저리 ee 719

Q&A

다중 cath SS 만들 수 있지만 한번 000 블록과 일치되면 처리가 된 것으로
간주하고 다음의 catch 블록으로 가지 않습니다. 0001 블록의 적절한 순서를 정
하는 것은 중요합니다. 이렇게 하여 S4 catch 블록이 먼저 검사되게 할 수 있

이번 장에서는 디버거의 근본을 살펴보았습니다. 경계점, 분기점 SS 살펴보았는
데 이 도구는 특정부분에서 무결점이 되도록 도와줍니다. 그리고 프로그램의 실
행되는 과정에서 각 변수의 RS 알 수 YAS 해줍니다.

Q 예외 사항을 만든 이유는 무엇입니까? 왜 오류가 발생한 곳에서 처리하지 않습니까?

A 각 코드의 다른 곳에서 같은 오류가 날 수 있습니다. 예외 사항은 오류의 중앙화를
피합니다. 추가하여 각 오류가 발생하는 곳이 OHS 처리하기에 가장 적합한 곳은
아닙니다.

Q 왜 객체를 만듭니까? 왜 오류 코드를 전달하지 않습니까?

A 개체가 오류 코드보다 음통성이 있고 강력합니다. 더 많은 gus 전달하고 각 생
성과 소멸시 생성자/소멸자 도구를 사용할 수 있는데 이는 예외 사항을 적절히 처
리하게 할 수 있습니다.

Q 비오류 조건에서 예외 사항을 사용하지 않아야 하는 이유가 있습니까? 비 예외 사항
조건이 존재할 때 지난 코드로 돌아가는 급행 열차를 타는 것이 편하지 않습니까?

A 맞습니다. 몇몇의 CH 프로그램들은 그 목적으로도 사용합니다. 단지 위험성의 예
외 사항은 스텍이 풀려 WR] 개체들이 자유기억 공간에 남게 될 때 메모리 누출
이 일어난다는 것입니다. 주의 깊게 프로그램을 만들면 이를 피할 수 있습니다. 그
렇지 않으면 이는 개인적인 취향의 문제입니다. 다른 프로그래머들은 예외 사항은
속성상 정상적인 조건에서는 사용하면 안된다고 합니다.

Q try 블록이 예외 사항을 만드는 곳에서 예외 사항이 잡혀야 합니까?

A 아닙니다. 호출 스택의 아무 곳에서나 잡을 수 있습니다.

Q coutL} 조건부 컴파일(#1106+)을 사용할 수 있는데 디버거를 사용하는 이유는?

fu

A 디버거는 여러분의 코드를 하나씩 살펴가고 값들을 살펴보고 할 때 여러분의 코드
를 수정하지 않고 살펴보는 강력한 도구를 제공합니다.


===== PAGE 721 =====
720 ee AB

연구

2

연구란에서는 이번 장에서 다루어진 주제를 여러

FL 8 mle

, 다음 장으로 넘어가기 전에 SS 충분히 이해하도록 합시다.

퀴즈

1. 예외 사항이란?
2 try 블록이란 무엇입니까?

3. catch 문장이란 무

4 예외 사항은 어떤 정보를 가질 수 있습니까?
5. 언제 예외 객체가 만들어집니까?

6. 예외 ATES 값으로 전달합니까 Hare 전달합니까?

무엇입니까?

7. catch 블록은 베이스 클래스를 보려면 파생된 예외 ASS 잡습니까?

8. 두 개의 catch 문장이 있는데 하나는 베이스이며 하나는 파생입니다. 무
합니까?

9 catch(...)= 무엇을 의미합니까?

to. 무엇이 분기점입니까?

연습 문제
. try 블록, catch 문장, 단순한 예외 사항을 만들어 봅시다.
2. 1Ho] 답을 변형하십시오. 예외 사항에 eS 넣고 접근자 함수를 넣고 0
록에서 사용하여 봅시다.
3. 2번 문제를 예외 사항의 계층 PRES 갖도록 수정하십
베이스 객체를 사용하여 수정하십시오.

시오. catch 블록을

4 3번의 문제를 3단계의 함수 SSS 가지도록 수정하십시오..
5. 버그잡기
class xOutOfMemory

ae
public:

ei
ful
d
a)
로
시
으
의,
ol
32.

a
확인해보는 퀴즈들과, 배운 AS 시험해 볼 수 있는 = dé 문제들
습니다. 부록 Do] 있는 답을 보기 전에 각 물음에 대답을 할 수 있

엇이 먼저와야

파생 객체와

xOutOfMemory( const Strings& message ) : itsMsg( message 210

~xOutOfMemory () {}

virtual const String& Message(){ return itsMsg };
private:



===== PAGE 722 =====
제20일 예외 사항과 오류 저리 ee 721

String itsMsg;

int main()
1
tryf
char *var = new char;
if ( var == 0 )
throw xOutOfMemory();

}
catch( xOutOfMemory& theException )
{
cout << theException.Message() << "\n";
}
return 0;


===== PAGE 723 =====
삐
르
ol
K
0
=
=]

도
|

| 어기



===== PAGE 724 =====


===== PAGE 725 =====
724 ㅇㅇ 제3주

서문

이제 여러분은 3주간에 걸친 0++의 강도 높은 과정을 막 마치려 하는 중입니다.

좋을                    ++에 대한 자신감이 생길 것입니
서는 좀더 배워야 할 일이 있습니다.
보충하고 앞으로 계속 공부해야 할

oN y

이번 장에서는 그 pe 과정에서 빠진 것을
사항을 정할 것입니다.
ee 다음을 배움니다.
 표준 라이브러리란 무엇인가?
Bone] 비트를 연산하고 플래그로 사용하는 법
BM (을 효율적으로 사용하기 위해 다음에 배워야 할 과정은 무엇인가

표준 라이브러리(53008[0 Library)

모든 0++의 구현에는 표준 라이브러리가 있고 또한 추가로 일반 라이브러리 함
수도 있습니다. 라이브러리란 여러분의 코드에 링크될 수 있는 함수의 집합을 의
미합니다. 이미 여러분은 여러 개의 표준 라이브러리 함수들과 클래스들을 보았
는데 대부분은 ostream 라이브러리였습니다.

라이브러리를 사용하기 위해 여러분은 일반적으로 여러분의 원시 코드 안에 헤더
파일을 포함해야 하는데 이미 앞부분에서 \00406 <iostreamh>S 사용한 예를 많
이 보았을 것입니다. 각 괄호는 컴파일러에게 여러분의 컴파일러의 표준 라이브
러리의 헤더 파일이 있는 디렉토리를 찾아보라는 뜻입니다.

Fe 라이브러리들이 있는데 파일을 연산하는 것부터 날짜와 시간을 수학 함
설정하는 것까지 있습니다. 오늘은 지금까지의 과정 중에서 배우지 않았던
라이브러리와 클래스 중 자주 쓰이는 것들을 배워봅니다.

뼈 +

Jou
수많
로
Sz.
~.

문자열(95\100) 라이브러리 함수

가장 흔히 쓰이는 라이브러리 함수는 아마도 문자열에 관련된 라이브러리 함수일
것인데 90600이 가장 자주 쓰일 것입니다. 90000은 널로 끝나는 문자열의 길이
를 반환합니다. 예를 봅시다.



===== PAGE 726 =====
Aaa 다음은 FAS 할 것인가? ee 725

[리스트 21.1] strlen()

1: #include <iostream.h>

2: #include <string.h>

3

4: int main()

58 <:

6:    char buffer[80];

2     00

8     {

95       cout << "Enter a string up to 80 characters: ue
10:     cin.getline(buffer,80) ;

415      cout << "Your string is " << strlen(buffer);
12;      cout << " characters long." << endl;

13%   } while (strlen(buffer));
14:   cout << "\nDone." << endl;
15%   return 0;

163)

결과  Enter a string up to 80 characters: This sentence has 31 characters
Your string is 31 characters long.
Enter a string up to 80 characters: This sentense no verb
Your string is 21 characters long.
Enter a string up to 80 characters:
Your string is 0 characters long.

Done.

6번 줄에서 버퍼가 만들어지고, 9번 줄에서 사용자는 문자열을 입력합니다.
사용자가 입력하면 입력된 문자의 개수가 11번 좋에서 출릭됩니다.

00...00416()의 검사 부분의 문장 while(strlen(buffer) S 주목합시 다. strlenQ-<- 버퍼가
비어 있으면 0을 반환하는데, 0은 거짓으로 되므로 버퍼에 문자가 있는 한 while

AA

(rag
dz

strcpy()2} strncpy()

두 WAZ 가장 많이 사용되는 SFE strepyOele] 하나의 문자열을 다른 곳으로
복사항니다. 이 © Was] GE 에 AE 의미가 많이 elated, a
하면 공급자나 사용자가 만든 문자열 클래스에서 문자열 연산을 잘하기 때문입니
2 ee 대입 연산자나 복사 생성자를 지원해야 하
는데 이는 strepyOS 사용하여 구현되는 경우가 많습니다. 예제를 봅시다.


===== PAGE 727 =====
726 ㅎㅇ 제주

[리스트 21.2] strepy 사응하기

1: #include <iostream.h>
2: #include <string.h>
31
4: int main®
be
6:    char stringOnel80];
C2    char stringTwoLl80];
3:
9:    stringOneL0J='\0';
10:   stringTwoL0J='\0';
V1:
2:   cout << "String One: " << stringOne << endl;
15%   cout << "String Two: " << stringTwo << endl;
14:
15:    cout << "Enter a string: ";
16:   cin.getline(stringOne,80) ;
Av:
18:   cout << "\nString One: " << stringOne << endl;
19:5   cout << "String Two: " << stringTwo << endl;
20:
215   cout << "copying..." << endl;
22°   strcpy(stringTwo,stringOne) ;
253
24:   cout << "\nString One: " << stringOne << endl;
25%   cout << "String Two: " << stringTwo << endl;
26:   cout << "\nDone." << endl;
at:   return 0;
28: 그
String One:

String Two:
Enter a string: Test of strcpy()

String One: Test of strcpy(
String Two:

copying...

String One: Test of strcpy(
String Two: Test of strcpy(

Done.



===== PAGE 728 =====
Mas 다음은 FAS 할 것인가? ee 727

분석  두 개의 C 형태의 널로 끝나는 문자열이 6, TH 줄에서 선언되었습니다. 9,

10번 줄에서 빈 문자열로 초기화되었고 그 값은 12, 13번 줄에서 출력되었

습니다. 사용자가 문자열을 입력하고 결과가 9008006에 저장되었습니다. 두 개의

문자열이 다시 출력되는데 단지 9008006만이 내용을 가졌습니다. strcpy()7} 다시
호출되고 90108006이 904081\0로 복사됩니다.

5000>0의 구문은 “두 번째의 매개 변수를 A 번째의 매개 변수에 복사하라”라고
읽힙니다. A 번째의 매개 변수가 두 번째 문자열의 길이를 수요하지 못할 정도
로 작으면 어떻게 될까요? 이를 해결하는 예제가 바로 [리스트 21.3]입니다.

[리스트 21.3] strncpy() 사응

#include <iostream.h>
#include <string.h>

1

2

3

4: int main()

ae ft

6:    char stringOne[80];
7     char stringTwoL10];
8:    char stringThreeL101];

92

10:   stringOneLOJ='\0';

TA   stringTwoL0J='\0';

12:   stringThreeLOJ='\0';

13:

14:   cout << "String One: " << stringOne << endl;

158   cout << "String Two: " << stringTwo << endl;

16%   cout << "String Three: " << stringThree << endl;
Wf:

18%    cout << "Enter a long string: ";

19   cin.getline(stringOne,80) ;

20:   strcpy(stringThree,stringOne) ;

216   //  strcpy(stringTwo,stringOne) ;

22:

2355   cout << "\nString One: " << stringOne << endl;
24:   cout << "String Two: " << stringTwo << endl;

256   cout << "String Three: " << stringThree << endl;
26%

te   strncpy(stringTwo,stringOne,9) ;

28:

29:   cout << "\nString One: " << stringOne << endl;
$0:   cout << "String Two: " << stringTwo << endl;

302   cout << "String Three: " << stringThree << endl;
S2¢



===== PAGE 729 =====
728 ee ABS

53:   stringTwoL9J='\0';

34:

55:   cout << "\nString One: " << stringOne << endl;
56:   cout << "String Two: " << stringTwo << endl;

St:   cout << "String Three: " << stringThree << endl;
38:   cout << "\nDone." << endl;

39: return 0;

40: }

a    String One:

String Two:
String Three:
Enter a long string: Now is the time for all...

String One: Now is the time for all...
String Two:
String Three: Now is the time for a ies

String One: Now is the time for all...
String Two: Now is th tii
String Three: Now is the time for all...

String One: Now is the time for all...
String Two: Now is th
String Three: Now is the time for 내

0006.

BY ose 좋에서 세 개의 버퍼가 선언이 되었습니다. 다른 버퍼들이 80의 걸이
를 갖는 반면 5008740는 단지 10개의 BAS 갖도록 선언되었습니다. 10 -
12번 줄에서 0의 길이로 초기화된 뒤 14 - low 줄에서 Sele] 되었습니다.
사용자가 문장을 입력을 하고 20번 줄에서 세 번째 문자열에 복사되었습니다. 21
줄은 주석으로 막혔습니다. 이 문자열을 50008140에 복사하면 프로그램의 예
분을 건드려 프로그램이 중지될지도 모릅니다.
함수 500000는 ALS] 매개 변수에 의해 포인트되는 주소를 복사하는데 충
간이 있는지는 조사하지 않고 그냥 복사합니다.

(a

oe (쏘

de 뻐
AN po AN [위 때
6 【

공
표준 라이브러리 함수들은 좀더 안전한 함수 90007)0를 제공하는데 특정한 7 air
sin Ht

의 문자를 대상이 되는 문자열에 복사합니다. stmepy2] 중간에 있는 매개 변
은 numbers 의미합니다. 이러한 개넘이 표준 라이브러리 전반에 걸쳐 사용됩니다.



===== PAGE 730 =====
제21일 다음은 FAS 할 것인가? ㅇㅇ 729

27번 줄에서 0008000의 처음 9개의 문자가 5008140에 복사되고 결과가 출력됨

니다. stmpy 복사된 문자열의 BS 널로 막지 않으므로 결과는 의도된 바대

로 되지 않습니다. 50000는 복사된 문자열을 QE 끝나게 하지만 stmepy= 그
렇지 않습니다.

33번 줄에서 BS 첨가하였고 문자열이 마지막으로 출력되었습니다.

strcat()=} strncat()

strepy()2} stmepy(Qol] 관계된 함수가 streat()7} 80200860입니다. 처음의 함수는

하다(60008660088)라는 뜻의 가운데 부분의 cat 이름을 BASU. 즉, 두 번째 매
개 변수의 문자열을 A 번째 매개 변수의 문자열 끝에 연결하라는 뜻입니다.
stmeat()-2 짐작할 수 있겠지만 처음의 개의 문자를 다른 문자열에 붙이는 것입
니다. 리스트를 봅시다.

[리스트 21.4] 91『08[(0과 strncat()

1: #include <iostream.h>

2: #include <string.h>

3:

4:

5: int main()

6: 4

(3    char stringOne[255];

3:    char stringTwol255];

9%

10   stringOneLOJ='\0';

Ve   stringTwoL0J='\0';

V2

13%    cout << "Enter a string: ";

14:   cin.getline(stringOne,80) ;

158

16:    cout << "Enter a second string: ";

aire   cin.getline(stringTwo,80) ;

18:

19:   cout << "String One: " << stringOne << endl;
20%   cout << "String Two: " << stringTwo << endl;
21%

22:   strcat(stringOne," 별

235%   strncat(stringOne,stringTwo,10) ;

245

25%   cout << "String One: " << stringOne << endl;


===== PAGE 731 =====
730 ee 제3주
26:   cout << "String Two: " << stringTwo << endl;
et?
28:    return 0;
29: }

(Aa

24 il}  Enter a string: Oh beautiful

Enter a second string: for spacious skies for amber waves of grain

String One: Oh beautiful
String Two: for spacious skies for amber waves of grain

String One: Oh beautiful for spacio
String Two: for spacious skies fir amber waves of grain

Ay 7, 88 SAM 두 개의 문자 배열이 만들어졌고 사용자는 두 개의 문자열을
입력하는데 둘 다 배열에 들어갑니다.

22번 줄에서 94148006 끝에 빈칸이 1개 Ao) 되고 23번 줄에서는 9000810의
처음 10개의 문자가 4008006에 연결되고 결과가 25, 26번 줄에서 출력됩니다.

다른 문자열 함수들

문자열 라이브러리는 다른 함수들을 제공하는데 문자열에서 특정 문자나 토큰을
찾아내는 GEE 있습니다. 문자열에 있는 AL 또는 특수 단어를 찾아내려면 여
러분이 필요로 하는 함수가 문자열 라이브러리에 이미 존재하는지 찾아봅시다.

시간과 날짜 관련 함수

시간에 관련된 라이브러리들도 현재의 시간과 날짜의 근사치를 알아내고, 날짜와
시간을 비교하는 여러 개의 함수들을 제공합니다.

이 라이브러리의 중심은 구조체 인데 이는 초, 분, 시간, 일, 월을 나타내는 숫
자(1월이 0임), 1900년 이후의 년도 FS 나타내는 숫자, 요일을 나타내는 숫자(일
요일이 0임), 년도 중 AA 임을 나타내는 숫자(0365), 서머타임을 알리는 나열
형 값(어떤 시스템에서는 이 BRL 지원이 안됩니다)의 9개의 정수형으로 구성
이 됩니다.

몇 개의 날짜용 함수는 변수 time BS 사용하거나 이 형의 WES 포인트합니
다. 이 형을 mao) 자료 PAE 변환하는 GEE 있습니다.



===== PAGE 732 =====
Aas 다음은 FAS 할 것인가? ee 731

© 라이브러리는 0000를 제공하는데 006.에 대한 포인터를 취한 뒤 현재의
aoe 채옵니다. 또 00060라는 것을 제공하는데 날짜가 이미 채워진 time tS
매개 변수로 취한 뒤 출력을 할 + 있는 4901형 문자열을 반환합니다. 시간에
관련되어 출력을 좀더 조정하려면 006. 변수를 10618060에 2  전달하면 되는데 그
러면 tm 구조체의 포인터를 반환합니다. 예제를 봅시다.

[리스트 21.5] ctime() 사웅법

1: #include <time.h>

2: #include <iostream.h>

3

4: int main()

58 (¢

6:    time_t currentTime;

vs

8:     // 현재 시간을 가져와 출력

9:    time (&currentTime); // fill now with the current time
10:   cout << "It is now" << ctime(&currentTime) << endl;
118

12:   struct tm * ptm= Localtime(&currentTime) ;

15:

14:   cout << "Today is " << ((ptm->tm_mon) +1) << "7";

15:   cout << ptm->tm_mday << "/";

16%   cout << ptm->tm_year << endl;

17:

18:   cout << "\nDone.";

19: return 0;

20: 3

It is now Tue Jul 19 11:14:27 1998

(uz
쁘

Today is 7/19/98

Done.

분석 6번 줄에서 000ㅠ60[00006이 07006의 형으로 선언되었습니다. 이 변수의 주
가 표준 라이브러리 0060에 전달되었고 변수  CurrentTime°] 현재의 eto}
시간으로 설정되었습니다. 이 변수의 주소가 ctimenz 전달되는데 이번에는
&5011형의 문자열로 반환되어 10번 줄에서 출력됩니다.


===== PAGE 733 =====
732

eo AB

CurrentTime2] 427} ©] Ho]= localtime()°] = 라이브러리 함수로 전달이 되고
의 주소가 반환되는데 OE ptm 지역 변수의 초기화값으로 됩니다. 이 구조체
의 멤버 자료는 현재의 달, 일, 년도를 출력하기 위해 사용됩니다.

stdlib

stdib= 다른 라이브러리 함수에 맞지 않는 함수들의 집합체입니다. 간단한 4

산술 함수, 정렬 함수(빠른 정렬 함수 중 하나인 66000 포함) 및 ASCH 텍스트

정수, long, float 등으로 변환하는 프로그램 등이 있습니다.

posi 있는 함수들 중 자주 쓰이는 AL atoi(), 1080 그리고 &010에 관련된 함
들입니다. 4010는 ^901를 정수형으로 변환합니다. 상수 문자 변수라는

alae 취한 뒤 정수형으로 바꿔 반환합니다. das 봅시다.

[리스트 21.6] ato) 및 관련된 BAS 사응

1: #include <stdlib.h>

2: #include <iostream.h>

3

4: int main®

5s

6:    char buffer([80];

7     cout << "Enter a number: ";

8:    cin >> buffer;

9:

10:   int number;

115   // number = buffer; compile error
123   number = atoi(buffer);

13:   cout << "Here's the number: " << number << endl;
14:

15%   // int sum = buffer + 5;
16:   int sum = atoi(buffer) + 5;

A   cout << "Here's sum: " << sum << endl;
18: return 0;
19: 3

Ai & Enter a nymber: 9

Here's the number: 9
Here's sum: 14



===== PAGE 734 =====
제21일 USS 무엇을 할 것인가? ㅇㅇ 733

AH oe] 줄에서 80문자의 버퍼가 할당되고 7번 줄에서 사용자는 숫자를 입력합
니다. 입력은 텍스트로 간주되어 버퍼에 저장됩니다.

10번 줄에서 정수형 변수 number7} 선언되었고 11번 줄에서 프로그램은 버퍼의

내용을 정수형 변수에 저장하려 합니다. 이는 컴파일러 오류를 발생하므로 주석

으로 막아버렸습니다.

12번 줄에서 표준 라이브러리 함수 4010를 호출한 뒤 버퍼를 매개 변수로 전달

하여 이 문제를 해결하였습니다. 반환값은 텍스트 문자열의 정수형 값이고 이는

정수형 변수에 저장된 뒤 13번 줄에서 출력되었습니다.

15번 줄에서 새로운 정수형 변수 sume] 선언되었고 정수형 상수 5를 버퍼에 더

한 결과를 대입하려 하였습니다. 이 역시 오류가 발생하고 010를 호출하여 해결

하려 하였습니다.

어떤 컴파일러에서는 표준 변환을(610()같은 함수) WARS 처리합니다. ome 내부
과정은 잘 몰라도 됩니다. 자세한 사항은 컴파일러 매뉴얼을 참조합시다.

(ig

qsort()

때로는 표나 배열을 정렬하고 싶은 때가 있습니다. 6000가 아주 빠르고 쉬운 방
We 제공합니다. 65000 사용에 있어 어려운 부분은 전달해야 할 구조체를 설정
하는 문제입니다.

05000는 4개의 인수를 가집니다. ASS 정렬하고자 하는 표의 시작 포인터이고
(배열명을 넣어도 됩니다.) 두 번째는 표의 원소의 개수, 세 번째는 각 Mad a
기, 네 번째는 비교하는 함수의 포인터입니다.

비교하는 함수는 정수형을 반환해야 하는데 매개 변수로 두 개의 상수형 100 포
인터를 취합니다. void 포인터는 0++에서는 자주 쓰이지 않는데 형 검사를 감소
시키기 때문이지만 어떤 Yo] 사항도 포인트할 수 있다는 이점이 있습니다. 여러
분의 05000 함수를 SHA 템플릿을 쓰는 것도 고려할 만합니다. 예제를 봅시다.

2

[리스트 21.7] qsort()

1: /* qsort example */
2:


===== PAGE 735 =====
734 ee ABs

3: #include <iostream.h>

4: #include <stdlib.h>

58

6: // 050「에 의해 요구되는 60『+400101의 형태
7: int sortFunction( const void *intOne, const void *intTwo);
8:

9: const int TableSize = 10; // 배열 크기

10:

11: int main(void)

12: ¢

155   int table(TableSize);

14:

15; // HIBS 값으로 체움
16:   for (int i = 0; i<TableSize; i++)

1:   {

18:      cout << "Enter a number: ";
19:      cin >> tableLil;

20:   2,

ene   cout << "\n";

(a

23:   // sort the values

26%   qsort((void *)table, TableSize, sizeof(table[01), sortFunction) ;
25:

26: // 결과 Be

et:   for (i = 0; i < TableSize; i++)

28:      cout << "Table [" << i << "]: " << tableLi] << endl;
29:

30:   cout << "Done." << endl;

S51:   return 0;

31: 3

32:

33: int sortFunction( const void *a, const void *b)

54: {

55%   int intOne = *(Cint*)a);

562   int intTwo = *(Cint*)b);

37:   if CintOne < intTwo)

ㅣ

38:      return -1;

59%   if (intOne == intTwo)
40:      return 0;

41:   return 1;

42: }

켈    Enter a number: 2
Enter a number: 9


===== PAGE 736 =====
제21일 다음은 SAS 할 것인가? ee 735

number: 12
Enter a number: 873
Enter a number: 0

Enter a
a
a

Enter a number: 45
a
a
a
a

Enter a number: 93
Enter a number: 2
Enter a number: 66
Enter a number: 1

TableLOJ]: 0
Table[1]: 1
Table[2]: 2
Table[3]: 2
Tablel4]: 9
Table[5]: 12
Tablel6]: 45
TableL[7]: 66
Table[8]: 93
TableL91]: 873
Done.

wey A 줄에서 표준 라이브러리 헤더 부분이 포함되었는데 이는 05000를 위해
La    필요합니다. TH 줄에서 함수 80000008000이 선언되고 4개의 매개 변수를
필요로 합니다.

13번 줄에서 선언된 배열이 사용자에 의해 16 - 20번 줄에서 입력되었습니다.
08000가 24번 줄에서 호출되었고 표의 MAGS 100*로 형 변환하였습니다.

80000000000라는 매개 변수가 06000로 전달되었습니다. 즉, 5000000008이라는 함
수의 포인터가 66000의 매개 변수로 APS 것입니다.

일단 05000가 실행이 되면 상수형 void 포인터 as} 를 각 배열의 값으로 Agu
다. 첫 번째 값이 두 번째 값보다 작으면 비교 함수는 -1을 반환합니다. 같으면 0
을 반환하고 첫 번째 값이 두 번째 값보다 크면 비교 Fee 1을 반환합니다. 33
- 42의 90000000000에서 나타났습니다.

다른 라이브러리 함수

여러분의 C+ 컴파일러는 많은 다른 라이브러리 함수들을 제공하는데 그들 중에
는 여러분이 여태껏 써왔던 표준 입출력 라이브러리와 스트림 라이브러리 함수가
습니다. 여러분의 컴파일러와 함께 온 안내서를 탐구하여 이 라이브러리 함수
이 무엇을 제공하는지 살펴봅시다.

Hin so ff


===== PAGE 737 =====
736 ㅇㅇ 제주

비트 SiAKBit Twiddling)
여러분의 객체 상태를 추적하기 위해 플래그를 설정할 때가 있습니다.
이를 사용자가 정의한 나열형을 가지고 할 수도 있지만 플래그가 많으면 그리고
저장 크기가 문제된다면 이 개별적인 VES 플래그로 사용하는 것이 편할 AY
다.
든 비트는 8비트를 가지고 있고 따라서 4바이트의 길이는 32비트의 독립된 플
그를 가지고 있습니다. 비트는 그 Fo} 1이 되면 설정됐다라고(680 하고 0이 되
지워졌다고(4680 합니다.68과 060는 명사로도 쓰이고 동사로도 쓰입니다.)
때 값을 변화시킴으로 설정과 지움을 할 수 있지만 이는 따분한 일입니다.

참고

부록 (에서 이진과 16진 연산을 다루었습니다.

iG,

an

0++은 각각의 비트에 작용하는 비트 연산자를 제공합니다. 이는 논리 연산자와
비슷해 보이지만 다릅니다. 따라서 초보 프로그래머들은 혼동할 수도 있습니다.
비트 연산자가 [표 21.1]에 있습니다.

[표 21.1] 비트 엽삽자

기후                            연산자

&                               AND

|                                OR

2                         배타적인 OR

~                      보수(6010ㅁ01610601)

비트 연산자 AND
AND 연산자(&)는 논리 AND 연산자와(&&) 달리 &가 한 개입니다. 두 a 비트
를 480하면, 만일 두 개의 비트가 다 1이면 결과는 1이고 그 이외에는 모두 0입
니다. 두 개의 비트가 모두 설정되어 있을 때에만 1이 됩니다.



===== PAGE 738 =====
Alaa 다음은 무엇을 할 것인가? ee 737

비트 연산자 OR

두 번째의 연산자는 080)입니다. 역시 |가 한 개이고, 논리 OR

은 두 개의 |를
가집니다. 두 개의 HES 08하면 두 개 중 하나라도 설정된 경우는 1

이: 됩니다,

배타적 비트 OR 연산자
세 번째는 배타적 OR 연산자입니다. 두 개의 비트가 다를 때 1로 됩니다.

보수 연산자(6000610070 연산자)
보수 연산자는 설정되어 있는 BE WEE 지우고, 지워져 있는 모든 비트는 설

BYU. 가령 현재의 값이 1010 0011이면 보수의 결과는 0101 1100입니다.

비트 설정(6004108 Bits)

특정 HES 설정하거나 지우고 싶을 때 masking 연산자를 사용합니다. 4바이트
플래그를 가지고 있고, 8번 비트를 TRUEZ 설정하고 싶을 때 128의 값으로 OR
8-2

를 하면 됩니다. 왜냐하면 1282 이진으로 1000 0000이기 때문입니다. 현재의 yy
트 Ke] 무엇이든 128로 ORS 하면 이 8번째를 설정하고 다른 곳에는 전혀 영향
을 안 미칩니다. 가령 현재의 값이 1010 0110 0010 0110이고 이를 128로 08#하면
이렇게 됩니다.
9 8765 4321

1010 0110 0010 0110         // 8번 비트가 0임
| 0000 0000 1000 0000        // 128

1010 0110 1010 0110         // 8번이 설정될

몇 가지 살펴볼 것이 있습니다. 첫째 비트는 오른쪽에서 왼쪽으로 세어집니다. 둘
Al 128은 8번째 비트만 제외하고 나머지는 모두 0입니다. 세 번째 처음의 1010
0110 0010 0110은 OR 연산자에 의해 8번째 비트 부분만 바뀌고 나머지는 그대로
입니다. 8번째가 이미 설정이 되었다면 바뀌지 않고 남아 있습니다.


===== PAGE 739 =====
738 66 제3주

비트 초기화

8번째 비트를 지우려면 128의 보수로 ANDS 하면

WES 지우고 나머지 모는

BES 설정하면 됩니다. 다음에 ANDS 하면

됩니다. 128의 보수는 8번째
원래

은 변함이 없고 단지 8번째 비트가 0으로 wc

1010 0110 1010 0110
& 1111 1111 0111 1111

1010 0110 0010 0110

이를 충분히 이해하려면 =
쓰고 그렇지 않으면 무조건
같습니다.

비트 H}271|(Flipping Bits)

연산을 해봅시다. 두 개가 다 1이면
입니다. 답을 비교하면 8번째만 지워지고 나머지는

// 8번 327 1일
// -128

// 8번이 지워짐

답에다 1이라

마지막으로 8번째 비트를 바꾸고자 합니다. 128로 배타적인 ORS 하면 됩니다.

1010 0110 1010 0110
^ 0000 0000 1000 0000
1010 0110 0010 0110
^ 0000 0000 1000 0000

1010 0110 1010 0110

// Rte
// 128

// 8번이 PFE
// 128

// 원 위치 됨

DO     OR 원산자를 사공하여 비트를 절정합시더.
DO     AND 연산자를 사용하여 비트를 로기화합시다.
DO     배타 ORS 사용하여 비트를 바꿀시다.

비트 ZX (Bit field)

6개나 8개의 바이트를 저장해서 사용해야 연

가 많습니다. 그런데 여러분이 사용하는 클래스나 구조체가 일련

을 가진다면 이들에게

모든 바이트가 다 사용되거나 혹은
산이 되는 경

의 나열형 변

비트 필드를 사용하게 할 수 있습니다.

우
수를 사용하거나 혹은 변수들이 매우 작은
사용



===== PAGE 740 =====
제21일 다음은 무엇을 할 것인가? ee 739

표준 C++ 자료형을 사용하여 여러분이 사용할 수 있는 가장 작은 문자형인데 1
바이트를 사용합니다. 종종 정수형을 사용하는데 이는 보통 4바이트를 사용합니
다. 비트 BES 사용하면 문자형 변수에 8개의 WS 저장할 수 있고 1008형에서
는 32개를 사용할 수 있습니다.

이제 비트 BES 사용하는 WS 봅시다. 비트 PEE 클래스의 멤버와 같이 이
름지어지고 접근될 수 있습니다. 그 형들은 항상 unsigned 정수형으로 선언됩니다.
비트 필드 이름 다음에 콜론을 쓰고 숫자를 Such 숫자는 컴파일러에게 얼마나
많은 비트가 이 변수에 할당될 것인지를 알려주는 명령입니다. 1이라고 쓰면 비
트는 0 혹은 1을 표현할 수 있습니다. 2를 쓰면 0 1, 2, 3의 총 4개의 BL 쓸 수
있습니다. 3은 개의 WS 의미합니다. 부록 0에서 이진수를 살펴볼 것입니다.
[리스트 21.8]을 봅시다.

[리스트 21.8] 비트 필드 사웅하기

#include <iostream.h>
#include <string.h>

0

1

2

3: enum STATUS { FullTime, PartTime } ;

4: enum GRADLEVEL { UnderGrad, Grad } ;

5: enum HOUSING { Dorm, OffCampus };

6: enum FOODPLAN (< OneMeal, AllMeals, WeekEnds, NoMeals };
7

8

class student
92 고
10: public:
ATs    student():
125    myStatus(FullTime),
1231    myGradLevel (UnderGrad),

14:    myHousing(Dorm),
15%    myFoodPlan(NoMeals)
AG?    {}

1G    “student () {}
18:    STATUS GetStatus();
19:    void SetStatus (STATUS) ;

20:    unsigned GetPlan() { return myFoodPlan; }
21:

22: private:

23:    unsigned myStatus : 1;

24:    unsigned myGradLevel: 1

25:    unsigned myHousing: 1;

26:    unsigned myFoodPLan : 2;

27. 33



===== PAGE 741 =====
740 eo 제3주

28:
29:
30:
315
$2:
53:
34:
55:
56:
SC:
38:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
5
521
53:
54:
55:
56:
57:
58:
598
60:
61:
62:
63:
64:
65:
66:
Ot:
68:
69:
70:
13

STATUS student: :GetStatus()
£
if (myStatus)
return FullTime;
else
return PartTime;

}
void student::SetStatus(STATUS theStatus)
xe
myStatus = theStatus;
}
int main()
{

student Jim;

if (Jim.GetStatus()== PartTime)

cout << "Jim is part time" << endl;
else

cout << "Jim is full time" << endl;

Jim.SetStatus(PartTime) ;
if (Jim.GetStatus()

cout << "Jim is part time" << endl;
else

cout << "Jim is full time" << endl;

cout << "Jim is on the" ;

char Plan[80J;
switch (Jim.GetPlan())

{
case OneMeal: strcpy(Plan,"One meal"); break;
case AllMeals: strcpy(Plan,"ALL meals"); break;
case WeekEnds: strcpy(Plan,"Weekend meals"); break;
case NoMeals: strcpy(Plan,"No Meals") ;break;
default : cout << "Something bad went wrong!\n"; break;
}
cout << Plan << " food plan." << endl;
return 0;



===== PAGE 742 =====
제21일 다음은 FAS 할 것인가? ee 741

겔과  Jim is part time

Jim is full time
Jim is on the No Meals food plan.

3 - 6번 줄에서 B 개의 US) 정의되었습니다. 이들은 학생 클래스 ot
에 비트 필드의 가능한 값들을 정의합니다.
학생 클래스는 8 - 27번 So] 선언되었습니다. 키드  음의 비트는 학생의 상태를 나타
냄니다.(전일제인지 파트타임인지) 두 번째 비트는 대학생인지 아닌지를 나타내고
세 번째 비트는 학생이 기숙사에 있는지 아닌지를 네 번째 비트는 4가지의 가능
한 식사 계획을 Gepaud.
클래스의 메쏘드는 다른 클래스와 같은 방식으로 사용되었고 비트 필드라는 사실
이 아무런 다른 gs 나타내지 않습니다.
멤버 함수 0066900480는 불린 HES 읽어 나열형을 반환하는데 반드시 필요하지
는 않습니다. 비트 필드를 직접 반환하도록 고칠 수 있습니다. 컴파일러가 변환을
담당합니다.
이를 증명하기 위해 0069000450를 다음으로 바꾸어 봅시다.

STATUS student: :GetStatus()

return myStatus;
B
프로그램의 기능에는 아무런 변화가 없습니다. 단지 코드를 읽을 때 명료성이 있
는가 없는가이며 컴파일러는 중요하지 않습니다. 46번 줄의 코드는 상태를 검사
하고 의미있는 메시지를 출력합니다. 이렇게 쓰고 싶을 것입니다.

cout << "Jim is " << Jim.GetStatus() << endl;

그러면 이렇게 출력할 것입니다.

Jim is 0

컴파일러는 나열형의 상수 PartTimes 텍스트로 SAS 방법을 가지고 있지 VF
니다.

61번 줄에서 프로그램은 식단 ADS switch 문장으로 처리하고 각각에 따라 버퍼

에 메시지를 넣으며 69번 줄에서 출력합니다. switchze 다음과 같이 쓰일 수 있
었습니다.


===== PAGE 743 =====
742 eo 제3주

case 0; strcpy(Plan,"One meal"); break;

case 1: strcpy(Plan,"ALL meals"); break;

case 2: strcpy(Plan,"Weekend meals"); break;

case 3: strcpy(Plan,"No Meals"); break;

비트 필드를 사용할 때 가장 중요한 Ae 클래스의 클라이언트들은 자료 저장 방
식에 신경을 쓸 필요가 없다는 것입니다. 비트 필드는 전용이므로 나중에 바꿀
수 있고 인터페이스는 바꿀 필요가 없습니다.

= Ail(Style)

이 책의 어디에선가 이야기했지만 코딩할 때 어떤 방식을 선택하든 크게 문제가
없지만 일단 정하면 정해진 일정한 코딩 WIS 가지는 것이 중요합니다. 일정한
방식을 가지면 코드의 특정 부분에서 어떻게 한 것인지 짐작할 수 있을 뿐 아니
a 나중에 알아보기 쉽게 해줍니다.

다음의 안내는 다소 임의적입니다. 이는 과거 저자가 작업해온 방식인데 비교적
잘 진행되었습니다. 여러분은 쉽게 여러분의 것을 만들 수 있는데 여기의 예제들
이 도움이 될 것입니다.

에머슨0808500이 말하였습니다. “서투른 일관성은 옹졸한 표시이다.” 하지만 코
드에 있어 일관성은 매우 중요합니다. 일단 마음을 정하고 그 후에는 신의 말씀

x

을 따르십시오.

들여쓰기(|0060!"08)
Bo} 크기는 4의 공간을 가지게 합니다. 여러분의 편집기에서 Bs 4의 크기로
BABA.

중괄호 정렬
중괄호를 어떻게 정렬할 것인가가 0 및 0++의 프로그래머 사이의 가장 큰 논쟁
이었습니다. Bele 이렇게 생각합니다.

mI

[을 이루는 SUSE 수직으로 만나야 합니다.
언이나 정의에 속하는 바깥쪽의 중괄호 짝은 그 가장 왼쪽에 있어야 합니다. 안의
한번 들여쓰기가 이루어져야 합니다. 다른 중괄호의 짝은

[줍니다.

mk
ot
le:

BA plo me

에:



===== PAGE 744 =====
제21일 다음은 무엇을 할 것인가? ㅇㅇ 743

Mie SES 중괄호와 같은 Soy 나타나지 않게 합니다. 예를 들

L

if ( condition == true )

{
j =k;
SomeFunction();
}
m++:

ie

i 줄의 처리

줄의 넓이는 화면 안에 나타나는 길이로 합니다. 한 줄에서 끝나야지 그렇지 않으
면 어지럽습니다. 어절 수 없이 So] 잘릴 때는 다음 Se 한번 들여쓰기를 합니
다. 또 적당한 부분에서 잘리도록 합니다. 중간에 연산자가 있는 경우 sls 끝에

경우 윗줄 끝

그대로 있게 합니다. 그래야 다음 줄에 무엇인가 온다는 것을 쉽게 짐작합니다.

CHAS CHAS] 함수보다 코드 wa 짧아지는 경향이 있습니다. 그래도 옛
날 말씀에도 있듯이 한 함수의 줄 수는 가능한 더욱 짧게 하십시오

switche 정렬
8\4애에서의 들여쓰기는 다음과 같이 합시다.

switch(variable)
no
case ValueOne:
ActionOne();
break;
case ValueTwo:
ActionTwo();
break;
default:
assert("bad Action");
break;
}

pal 코드 HAE

기 쉽게 하기 위해 몇 가지 원칙들이 있습니다. 읽기 AMok 유지 보수


===== PAGE 745 =====
744 eo HBF

를 읽기 쉼도록 하기 위해 공백 문자를 활용합시다.
조

를 극체와 배열은 어떤 것인가를 참조합니다. 객체 참조자 사이에 공백을 넣지 WAL .

>,[]]

연산과 누비 있으므로 사이에 공간을 넣지 BASH 연산체와 먼 곳에 공

& sizeof 둥입니다.
BM AeA E 양끝에 SHS 넣읍시다.

+=/%×<…<=-ㄴ&1,6&11, = 둥이 있습니다.
| 우
Bw 쉼프와 세미콜론 다음에 공백을 넣고 전에 넣지는 BAG.
| |

를 에약어} 같은 경우|는 공백 문자로 분리합시다: } (a = bl
를 주석의 몸체는 //로부터 공백으로 분리합시다.
를 포인터나 참조자는 형 이름에다 붙여쓰고 변수명에 붙이지는 WA.

char* foo;
int& theInt;

아래와 같이 하지는 BAICt.
char *foo;
int &theInt;

를 하나 이상의 변수를 같은 줄에 넣지 맘시다.

상술자 작명법

가지 기준이 있습니다.

를 상술자 이름은 Use 알릴 수 있도록 충분히 길어야 합니다.

약이나 단촉을 사용하지 맘시다.

를 작명에 시간을 쏟읍시다.
가리 eel ae 하지 BITE CHE 강형 언어이므로 변수명에 형을 집어넣을 이
가 없습니다. 사용자 정의형|클래스|에 있어 형가리         ‘

인터 앞의 p, 참조자 앞의 (, 클래스 멤버 변수 앞의 는 붙여 써 주도록 합시다.
ES 읽기 쉽게 하거나 사용법이 아주 자명한 경우에만 BU.

범

위에 비례합니다.

ul

| |
a3
Tle
[표
on
tle
th     ne)

변수명의 길이는 그



===== PAGE 746 =====
제21일 USS FAS 할 것인가? ㅇㅇ 745

0 각각의 변수명은 서로 혼동되지 않도록 해야 합니다.

를 SAE) RS 동사이거나 동사-명사구이어야 합니다. Search|), Resell),
FindParagraphl), ShowCursorl) 등입니다. 변수명은 주로 추상 명사이며 또 하나의 명사가 붙
을 수 있습니다. 6007, state, windSpeed, windowHeight, 불린 변수명은 적절하게 합니다.
windowlconized, filelsSOpen 둥입니다.

이름에 철자 붙이기와 대문자 붙이기

이름에 철자 붙이기와 대문자 붙이기는 여러분의 프로그램 방식에 있어 간과되어
서는 안됩니다.

를 어떤 언어에서는 모두 대문자로 쓰고 의미를 분리할 때 밑줄 문자를 쓴 경우도 있었습니
다. SOURCE_FILE_TEMPLET. 그런데 0++에서는 그렇지 않습니다. 단 상수이거나 템플릿은
그렇게 합니다.

를 다른 상술자는 혼

typedef, 구조체  on 비티 시작합니다. 자료 멤버나 지역 멤버들은 소문자로
합니다.

를 나열형 상수들은 0007의 축약 의미로 약간의 소문자로 시작합니다.

enum TextStyle

a
tsPlain,
tsBold,
tsItalic,
tsUnderscore,
3;

주석은 프로그램을 훨씬 이해하기 쉽게 합니다. 하나의 프로그램을 가지고 며칠,
w

몇 달을 쉬는 경우가 있습니다. 이런 경우 나중에 특정 코드가 무엇을 하는지 왜
이 부분을 포함하였는지 모를 때가 있습니다. 프로그램에 대한 이해의 문제는 다
= 사람이 여러분의 코드를 IS 때 발생합니다. 주석은 일관성을 가지고 적용되
어야 하고 노력            3

Moser /* … */ CH] //
a

주석이 프로그램에 대한 자세한 주석보다 효과가 있습니다. 부가 가치를 창출
해야지 단지 BES 다시 서술하는 것은 의미가 적습니다.

4

ntt;// n& 하나 증가함


===== PAGE 747 =====
746 ee 제3주

이는 별로 의미가 없습
합니까《 sage 무엇입

느
정들을 기술합시다. “n°           al
가 말입니다. 복잡한 논리에 있어서는 각 부분에 있어서의 조건들을 기술합

를 사용하지 BAS 너무 자세하게 적는다는 것이 나중에 보면 좋은 것이 됩니다.

를 빈줄을 잘 활웅합시다. 문장들을 논리적인 그룹으로 나눔시다.

(Access)
프로그램에 접근하는 것도 일관성이 있어야 합니다.
MY public, 00706, protected FS 사용하도록 합시다. 기본값에 의존하지 맘시다.
를 범응 멤버를 먼저 쓰고 다음에 보호 멤버, 전용 멤버 순으로 합시다. 메쏘드 다음에 자료
멤버를 Balch

를 생성자를 먼저 쓰고 소멸자

[=]
시다. 접근자 함수를 가능하면 같은 그룹으

. 재생 메쏘드를 각각 같은 이름으로 ASH
묶어 BAS.
를 한 그룹에서는 메쏘드 이름과 변수명을 알파벳순으로 정리를 합시다. 00006에서 파일명
을 알파벳순으로 정렬합시다.
를 중복에 있어 virtual 예약어가 조건부일지라도 가
}|실을 환기시켜주고 따라서 선언이 일관성 있게

떠
off
=

ie
=

Ht

Se

클래스 정의
메쏘드의 정의를 선언과 같은 순으로 합시다. 찾기가 쉽습니다.
함수를 정의할 때 반환형과 수식자를 전 줄에 ATS 하여 함수명과 클래스명이
좌측에 BES 합시다. 함수명을 찾기 쉽게 해줍니다.

include 파일
포함되어야 할 파일은 헤더 파일에 넣읍시다. 가장 소규모의 바람직한 헤더 파일
은 클래스와 그로부터 파생된 파일들을 위한 헤더 파일입니다. 여러분이 만드는
또 다른 10006 FAIS 선언되는 클래스의 멤버 객체들을 위한 파일입니다.
include 파일을 헤더 파일에서 빠뜨리지 BA. 왜냐하면 이를 포함하는 cpp 파
일은 afd includes 가져야 하기 때문입니다.

to

tho



===== PAGE 748 =====
제21일 다음

벼
2

것인가? ee 747

assert()
855600)를 맘껏 사용합시다. 오류를 찾는데 ESS 주고 또한 프로그램을 보는 사
람으로 하여금 전제 조건을 알게 합니다. 프로그래머의 생각을 알게 합니다.

const
적절한 곳에 const 사용합시다. 매개 변수, 변수, 메쏘드 등에 사용합니다. 하나
의 메쏘드에 상수형과 비상수형의 버전을 각각 요구하는 때가 있습니다. 명시적으
로 상수형을 비상수형으로 Fe doe 형 변환을 할 때 조심합시다. - 이렇게 하
는 수밖에 없는 경우가 많습니다 - 할 수 없이 이럴 때에는 주석을 달아 놓읍시다.

다음 단계
++을 가지고 349 동안 열심히 공부하였습니다. 이제 여러분은 상당한 0++ 프
로그래머가 되었으리라 생각합니다. 그러나 아직 끝은 아닙니다. 아직 배울 것은
많고 전문가가 되기 위해서는 훌륭한 CH 프로그래머에게서 배울 것이 많습니다.
asl 각가의 부분에서 Be AES Deed 이는 전부 Bela 7 개인적인  경험
과 의견에서 좋다고 생각되는 것들입니다. 각 부분에 we 책을 추천하였는데 구
입하기 전에 다른 사람의 의견도 구하여 봅시다.

어디에서 도움과 중고를 구할 것인가?
(+ 프로그래머로서 여러분이 제일 먼저 해야 할 일은 온라인으로 서비스되는
CH 토론그룹에 참가하는 것입니다. 이 단체들에 가입하면 수많은 c++ 프로그래
머들과 만날 수 있으면 여러분의 질문에 대답을 주고, 충고를 하며 여러분의 기
발한 생각에 WIS 달아 줄 것입니다.
저자는 인터넷의 F221 (comp.lang.ct+, 00000.1008.0++.000004660)에서도 활발히
참여하고 있는데 이런 곳에서 좋은 정보와 ESL 얻으리라 봅니다.
또한 여러분들은 C++ 사용자 소그룹을 발견할 수 있을 것입니다. 많은 도시나 학
교에서 프로그래머들을 만나고 생각을 교환할 수 있을 것입니다.

좀더 읽어야 할 책
다음 책을 사서 71S 바랍니다.


===== PAGE 749 =====
748 oe 제3주

Meyers, Scott. Effective C++ (ISBN: 0-2-1-56364-9). Addison-Wesley
Publishing, 1993

이 AS 저자가 읽은 책 중 가장 유용한 책인데 구입하여 3번이나 읽었습니다.

잡지

위의 ASS 읽고 또 더 YE 것이 앞으로 여러분이 C+ 프로그램에 접근하는데
매우 중요한 부분이 될 aoe 그런데 여러분의 기술을 신장할 더 많은 부분

이 있습니다. 0++에 관련된 좋은 잡지를 구독합시다. 본인의 개인적인 생각으로
는 SIGS 출판사의 C+ 200 좋을 것입니다. 모든 주제가 유용한 제목으로 포
장되어 있습니다. 잘 MoE. 오늘 별로 중요하지 않은 것이 내일 HI 중요
한 것이 될 것입니다.

C++ Report SIGS 출판사에서 얻을 수 있는데 =A P.O. Box 2031, Langhore,
PA 19047-9700 입니다. 저는 그 잡지사와 관계는 없습니다,(저는 다른 2개의 출판
사에서 일합니다) 하지만 0++에는 그 잡지가 좋습니다.

직접 연락을 원할 때

이 책에 대해 하고 싶은 Bol 제안, 혹은 좋은 생각은 항상 즐거운 마음으로
들을 준비가 되어 있습니다. SEY] jliberty@zdi.ziffcom2= E-MAILS 띄우시
거나 혹은 인터넷 웹 사이트 \'\\.11060“8590010165.000으로 연락 바랍니다. 반갑게
맞이하겠습니다,

i
습니다

DONT 코드만 읽지 It He 배우는 좋은 방법은 (++을 작성하는 것입니다.
00 좋은 C++ 잡지를 읽고 그룹에 가입합시

분은 CH 컴파일러에 있는 표준 라이브러리 함수들이 일상적인 작업을
을 보았습니다. 90000, strlen) 및 관련 함수들이 널로 끝나는 문자열을



===== PAGE 750 =====
제21일 다음은 FAS 할 것인가? ee 749

Q&A

다루는데 쓰입니다. 이런 것들이 여러분이 만든 문자열 클래스를 직접 연산할 수
는 없지만 여러분의 클래스를 구현하는데 기본적인 기능들을 제공합니다.
날짜와 시간 함수들이 시간 구조체를 연산하고 얻는데 ESS 줍니다. 여러분의
시스템 시간을 구하고 접근하거나, 혹은 여러분이 만든 시간 및 날짜 관련 객체
를 연산하는데 도움을 줍니다.

또한 각 개별적인 ~ 설정하고 검사하는 법 및 클래스 멤버에 제한된 개수의
비트를 할당하는 법을 배웠습니다.
마지막으로 C++ 방식이 이야기되었고 앞으로의 공부에 필요한 자원이 소개되었
습니다.

Q 표준 라이브러리들이 + +의 컴파일러에 있는 이유는? 또 표준 라이브러리들이 쓰이
는 때는 언제입니까?

A Co} 동질성을 갖추기 위해 있습니다. 그들의 형은 보장받지 못하고 사용자가 만든
클래스와 잘 어울려져 작업되지 않습니다. 따라서 사용이 제한됩니다. 종종 여러분

은 모든 특정 기능이 0++에서도 특정 라이브러리 함수로 제공되기를 바람니다. 이
때쯤이면 (의 라이브러리 함수들은 별로 도움이 안 될 것입니다.

Q 정수형 대신에 비트 구조체를 사용하는 이유는 무엇이니까?

A 객체의 크기가 문제일 때 사용합니다. 제한된 메모리 혹은 통신 소프트웨어에서 작
업할 때 이 구조체에 의해 제공된 절약된 부분이 여러분의 산출물에 중요한 요소가

된다는 것을 알게 될 것입니다.
 프로그램을 작성하는 문체가 중요한 이유는?
A 프로그래머들은 그들의 프로그램 제작 습관에 매우 없매입니다. 이런 방식의 코딩
에 익숙해져 있다면

if (ComeCondition){
// 문장

ro

}// B

이를 버리기는 어렵습니다. 새로운 문체는 틀
한번 온라인 통신 서비스에 접속을 하여 올바
수천만 가지의 대답이 자기가 제일이라고 우기
보게 될 것입니다.

a)
ta
©,
EI
rot
애

(a5


===== PAGE 751 =====
750 ㅎㅇ 제주

Q 다음에는 어떤 것을 읽어야 합니까?

A 어려운 질문입니다. 좀더 기본적인 것을 원한다면 다른 입문서를 읽어보도록 합시
다. 여러분의 Aas 갈고 Foe Scott Meyer2] Effective 0++을 구해 읽어봅시다.
객체 지향 기술을 향상시키려면 객체 지향 설계와 분석에 관한 AS AES 합시
다. 마지막으로 윈도우나 맥에서 작성하고 싶으면 플랫폼에 관한 입문서를 ALS

합시다. 얼마 안 있어 그 ASS 다 읽어야 할 것입니다.

A 그렇습니다. 여러분은 0++에 대해 배웠지만 사실은 일부분입니다. lod 전 만 해도
한사람이 이것 저것을 아는 것이 수웠습니다. 오늘날은 그것이 아닙니다. 여러분은
따라갈 수가 없습니다. 또한 노력을 해도 세상이 변합니다. 꾸준히 독서를 합시다.
최근에 바 것을 따라갈 수 있도록 노력을 합시다. 잡지와 온라인 서비스를 이용
합시다.

ay

Pm

에

1. strcpy()St 6[『000()의 차이는?

2 ctime()0| 하는 일은?

3. ^601| 문자열을 1000형으로 바꾸는 함수는?
4 보수 연산자의 ASS 무엇입니까?

5. ORZt 배타적 OR(Exclusive 야3)의 차이는?
6 &와 &&의 차이는?

Je iA ||의 차이는?

연습 문제
1. 20바이트의 SAAS 10바이트의 문자열로 복사되게 하는 프로그램을 작성하십시오. 남
는 것은 자릅니다.
2 94년 7월 28일부터 현재의 날짜를 알리는 프로그램을 작성하십시오.
3. 26개의 플래그(3ㄱ로 이름 붙여짐 )를
를 치게 하십시오. 비트를 설정하고 읽게 하여

하십시오.
4. 두 개의 SAS 덧셈 연산자(+ )를 사용하지 않고 더하는 프로그램을 작성하십시오.

비트 연산자를 TS



===== PAGE 752 =====


===== PAGE 753 =====
752 ee 제3주

아래의 프로그램은 지난 3주 동안 어렵게 공
니다. 셋째 주에서의 복습에서는 템플릿을 기반

법         은 AY
한 연결 리스트를 예외 사항

rm, -ㅁ
16 (에
때 님
피|
™,

한
과 함께 다룹니다. 자세히 살펴봅시다. 충분히 이해하였으면 이제 진짜 CH 프로
그래머입니다.

[리스트 R3.1] 셋째 주 복습 목록

OMAN 에 내 든 에 52 — ㅇㅇ
ㆍ …… …… ……… …×… … …… … …‥…

[ [RRR RRR KERR RRR RR 세가 규소 고 규소 고 규소 나 고 ERE RK

//

// Title: 셋째 주 복습 프로그램
ii

// File: Week3

//

// 서술 : 템플릿을 WHE 한 연결 리스트
// 및 예외 ^

lie

// Classes: PART - part 번호 및

// part 관련된 다른 정로 (개

//  6ㅁ6「+의 실랭시 령울 SAE 연산자
// _ operator<< 를 '가지는 목록에 | 대한
//    예제 class U.

Mae        ：

//

// Node - List2| 노드

//

// List - 템플릿을 기반으로 한 list
//    연결 리스트의 메커니즘 구련

Ii

Lf

// Author: Jesse Liberty (jl)

//

// Developed: Pentium 200 Pro. 128MB RAM MVC 5.0
//

// Target: Platform independent

//

// Rev History: 9/94 - First release (jl)

//          4/97 - Updated (j1)

// KAKI KIKI KIKI KI RIKKI IKI KARR KARIERRE RRR KERR

#include <iostream.h>

// 예외 사항 클래스
class Exception {};
class OutOfMemory : public Exception{};



===== PAGE 754 =====
제3주 끝내면서 ee 753

37:
38:
59:
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
Dit
52:
53%
54:
55
56:
57s
58:
59:
60:
61:
62:
63:
64:
65:
66:
67:
68:
69:
70:
(is
fe
Te
74:
251
76:
aes
78:
092
80:
81:
82:

class NullNode : public Exception{};
class EmptyList : public Exception {};
class BoundsError : public Exception {};

// KRKRKKKKKKERKKEE Part KXKKKEKKKKKKK

// 각 부분에 대한 추상 베이스 클래스

class Part

{

public:
Part():itsObjectNumber(1) {}
Part(ULONG ObjcetNumber) :itsObjectNumber (ObjectNumber) {}
virtual ~Part(){};
ULONG GetObjectNumber() const { return itsObjectNumber; }
virtual void Display() const =0; // 중복되어야 St

private:
int itsObjectNumber;

};

// 순수 가상 함수 구련

// 파생 클레스 연결 기능
void Part::Display() const
{
cout << "\nPart Number: " << itsObjectNumber << endl;
y

// BE part 객체에석 operator<< FEE
// 전용 data 접근하지 않으므로 프랜드일 필요는 없음
// 필요로 되는 다령성을 사용하는 019018>( BB
// thePart®| 실제 형에 근간 하여 중복을 원하지만
// 6++이 지원 안함
ostream& operator<<( ostream& theStream,Part& thePart)
{
thePart.Display(); // 가상
return theStream;
}

// *×**×*×*×**×**×*×****** Car Part KkKKKEKKK
class CarPart : public Part
{
public:
CarPart():itsModelYear (94) {}
CarPart(USHORT year, ULONG partNumber) ;
USHORT GetModelYear() const { return itsModelYear; }
virtual void Display() const;


===== PAGE 755 =====
754 ee 제3주

835:
84:
85:
86:
Sr
88:
Soe
90:
91%
92:
93:
94:
95:
96:
978
98:
99:

100:
101:
102:
103:
104:
1055
106:
107:
108:
109:
1105
110:
112:
11135
1148
1152
116:
Tt:
118:
119
120:
1218
122:
123%
124:
125¢
126:
127:
1285

private:
int itsModelYear;
3;

CarPart::CarPart(int year, int partNumber):
itsModelYear (year),
Part (partNumber )

{}

virtual void CarPart::Display() const;
{
Part::DisplayQ;
cout << "Model Year: " << itsModelYear << endl;

// xKekKKKKKKKKKK AirPlane Part ***kkk*
class AirPlanePart : public Part
{
public:
AirPlanePart():itsEngineNumber (1) {3};
AirPlanePart(USHORT EngineNumber, ULONG PartNumber) ;
virtual void Display() const;
int GetEngineNumber()const { return itsEngineNumber; }
private:
int itsEngineNuber;
3;

AirPlanePart::AirPlanePart(int EngineNumber, int PartNumber);
ijtsEngineNumber (EngineNumber),
Part (PartNumber )

{}

virtual void AirPlanePart::Display() const
{

Part::DisplayQ;

cout << "Engine No.: " << itsEngineNumber << endl;
}

// List 클래스 선언
template <class T>
class List;

// KRRRKKKKKKKKKKKKKK NODE KKKKKKKKKKKKK
더   x   A  Lo
// List 추가될 수 있는 일반 노드

10 RRR KEKE KKK ER EKRE REE RRR ER REREERER



===== PAGE 756 =====
제3주 끝내면서

ee 755

1295
130:
131
1525
133:
134:
135%
1356:
1348
138:
139
140:
141:
142:
143:
144:
145:
146:
147:
148:
149:
150%
15.
152%
15S:
154:
155:
156:
157 、【
158%
159:
160:
161:
162:
165:
164:
165:
166:
167:
168:
169:
170:
1208
V2:
175%
1748

template <class T>
class Node
{
public:
friend class List<T>;
Node (T*);
“Node();
void SetNext(Node * node) { itsNext = node; }
Node * GetNext() const;
T * GetObject() const;
private:
T* itsObject;
Node * itsNext;
3;

// Node 구현

template <class T>

Node<T>: :Node(T* pOjbect):
itsObject(pOjbect),
itsNext(Q),

{}

template <class T>

Node<T>: : ~Node()

{
delete <class T>
itsObject = 0;
delete itsNext;
itsNext = 0;

// 다음 노드가 BOA NULL 반환
template <class T>
Node<T> * Node<T>::GetNext() const
{

return itsNext;
}

template <class T>
T * Node<T>::GetObject() const
{
if (itsObject)
return itsObject;
else
throw NullNode();


===== PAGE 757 =====
756 ce 제주

115s
176:
1778
1788
179:
180:
101:
182:
185:
184:
185
186:
187:
188:
189:
190:
191:
192:
193s
194:
195:
196:
1975
198:
199:
200:
201:
202:
203%
204:
205:
206:
207:
208:
209:
210:
242
212:
2133
214:
215:
216:
eles
218%
219:
220:

// RRRRKKKRRKEKREKKEEK LIST RRKKKKKKEKKR
// 일반 List template
// 어떤 객체와도 작용
// KRKRRKRKEKR ERR KR ERE RRR 소고 소계 고 고 고 스고 고 고 고 곤 소곤
template <class T>
class List
public:
ListQ);
“LISt Os

Tx Find(int & position, int ObjectNumber) const;

Tx GetFirst const;

void Insert(T *);

T* operatorLi(int) const;

int GetCount() const { return itsCount; }
private:

Node<T> * pHead;

int    itsCount;
3;

// 리스트 구현

template <class T>

ㄴ01562 sListQ =
pHead(0),
itsCount (0)

{}

template <class T>
Lisit<t>!s List©O
{

delete pHead;
}

template <class T>
Tx List<T>::GetFirst(@ const
{
if (pHead)
return pHead->itsObject;
else
throw EmptyList();

template <class T>



===== PAGE 758 =====
제주 끝내면서 ee 757

221: T * List<T>::operatorL](int offSet) const

2225 1

223:   Node<T>* pNode = pHead;
224:

220%   if (!pHead)

226:      throw EmptyList();

227』

228:   if (offSet > itsCount)
229:      throw BoundsError();
230%

2312   for (int i=O;i<offSet; i++)
232      pNode = pNode->itsNext;
233:

234:   return pNode->itsObject;
235: }

236:

237: // 단일 AB (id) B 리스트의 객체를 찾아감

238: template <class T>

239: Te List<T>::Find(int & position, int ObjectNumber) const
240: {

241:    Node<T> * pNode = 0;

242:   for (pNode = pHead, position = 0;

243:     pNode!=NULL;

244:   pNode = pNode->itsNext, position+t)
24581   {

246:      if (pNode->itsObject->GetObjectNumber() == ObjectNumber)
247:      break;

248:   Bs

249:   if (pNode == NULL)

250:      return NULL;

25 le   else

252:      return pNode->itsObject;

2538 >

254:

255: // 객체 번호가 유일하면 삽입

256: template <class T>

257: void List<T>::Insert(T* pObject)

258: <

259:   Node<T> * pNode = new Node<T>(pObject);
260:   Node<T> * pCurrent = pHead;

261:    Node<T> * pNext = 0;

262:

263:   int New = pObject->GetObjectNumber();
264:    int Next = 0;

265%   itsCount++;

266:


===== PAGE 759 =====
758 ee ABs

267:
268:
269:
200:
271%
2(2:
203%
274:
275":
276:
277
278:
279:
280:
281:
282:
283:
284:
285:
286:
287:
288:
289:
290:
291:
292:
293:
294:
2955
296:
297:
298:
299:
300:
301:
302:
303:
304:
305:
306:
3507:
308:
309:
310:
S118
312:

if (!pHead)

{
pHead = pNode;
return;

}

// WEY 헤드보다 작으면
// 새로운 AED
if (pHead->itsObject->GetObjectNumber () > New)
{
pNode->itsNext = pHead;
pHead = pNode;
return;

for C33)
i
// 다음이 없으면 추가
if (!pCurrent->itsNext)
{
pCurrent->itsNext = pNode;
return;
}

// 사이에 있으면 주가

// 아니면 다음으로 감

pNext = pCurrent->itsNext;

Next = pNext->itsObject->GetObjectNumber () ;

if (Next > New)

{
pCurrent->itsNext = pNode;
pNode->itsNext = pNext;
return;

3

pCurrent = pNext;

int main)

a

List<Part> theList;
int choice;

int ObjectNumber;
int value;

Part * pPart;



===== PAGE 760 =====
제3주 끝내면서 ee 759

313%
314:
3155
316:
317:
318:
319:
320:
32181
522:
525:
324:
325%
326:
Sec:
328:
$29:
330:
S512
S32:
333:
334:
535:
336:
557%
358:
339:
341:
341:
342:
343:
344:
345:
346:
347:
348:
349:
S50
551:
352:
353%
354:
3523
356:
557:
358:

while (1)

{
cout << "(O)Quit (1)Car (2)Plane: ";
cin >> choice;

if (!choice)
break;

cout << "New ObjectNumber?: ";
cin >> ObjectNumber;

if (choice == 1)
{
cout << "Model Year?:";
cin >> value;
try
‘C
pPart = new CarPart(value,O0bjectNumber) ;
}
catch (OutOfMemory)
{
cout << "Not enough memory; Exiting..." << endl;
return 1;
}
}
else
{
cout << "Engine Number?";
cin >> value;

try
a
pPart = new AirPlanePart(value,0bjectNumber) ;
}
catch (OutOfMemory)
{
cout << "Not enough memory; Exiting..." << endl;
return 1;
}
try
(
theList.Insert(pPart) ;
I
catch (Nul LNode)
{

cout << "The List is broken, and the node is null!" << endl;


===== PAGE 761 =====
760 ee 제3주

359:
360:
361:
362:
363:
364:
365:
366:
367:
368:
369:
$70:
CY Atty
372:
373:
374:
3791
376:
S(T:
378:
579%
380:
381:
382:
383:
384:
385:
386:
387:
388: }

return 1;

a

catch (EmptyList)

본
cout << "The List is empty!" << endl;
return 1;

try
{
for (int i = 0; i < theList.GetCount(); i++)
cout << "(theListlil);
a
catch (NullNode)
본
cout << "The List is broken, and the node is null!" << endl;
return 1;
3
catch (EmptyList)
{
cout << "The List is empty!" << endl;
return 1;
}
catch (BoundsError)
{
cout << "Tried to read beyond the end of the list!" << endl;
return 1;
3
return 0;

결과  (O)Quit (1)Car (2)Plane: 1
New PartNumber?: 2837

Model Year? 90

(O)Quit (1)Car (2)Plane: 2
New PartNumber?: 378
Engine Number? 4938

(O)Quit (1)Car (2)Plane: 1
New PartNumber?: 4499
Model Year? 94

(O)Quit (1)Car (2)Plane: 1



===== PAGE 762 =====
제3주 BUA ee 761

New PartNumber?: 3000
Model Year? 93

(O)Quit (1)Car (2)Plane: 0

Part Number: 378
Engine No. 4938

Part Number: 2837
Model Year: 90

Part Number: 3000
Model Year: 93

Part Number 4499
Model Year: 94

불셀 3) 복습에서는 2주째 프로그럼을 수정하여 PHS 추가하고 ostream
과 예외 사항을 다루었습니다. 출력은 동일합니다.

35 - 39 줄에서 몇 개의 예외 클래스가 선언되었습니다. 이 프로그램에 의해 보여
진 몇몇 초보적인 예외 사항 처리에서는 자료나 메쏘드가 필요하지 않습니다.
catch 문장의 플래그로 작용하는데 매우 간단한 경고를 출력하고 빠져나갑니다.
좀더 좋은 프로그램에서는 이 예외 사항들을 참조자로 전달하고 문제를 해결하기

위해 예외 사항에서 자료나 BBS 만들어낼 것입니다.

44번 줄에서 추상 베이스 클래스 #가 2째 주 복습과 똑같이 선언되었습니다.
단하나 흥미있는 변화는 비클래스 멤버 006800<<(인데 69 - 73번 줄에 선언되었
습니다. 이는 Part] 멤버도 아니고 프랜드도 아닙니다. 인수의 하나로 Pat 참조
자를 취합니다.

올바른 operator<<7} car part 3-2 airplane part 중 어떤 것이 전달되느냐에 의해
호출되기를 바라는 마음에 006000<<가 CarPart2} AirPlanePart= 가지기를 원할
것입니다. 그러나 프로그램이 에 대한 포인터를 전달하고 CarPart}
AirPlaneParto]] 대한 포인터를 전달하지는 않으므로 0++은 Bro] 대한 인수의 A
제 형에 의거하여 올바른 함수를 호출해야 할 것입니다. 이를 역변화
(00008808008)라 하는데 0++에서는 제공되지 않습니다.

+에서 다형성을 구현하는 두 가지 방법이 있습니다. 함수 다형성과 변수 다형성
입니다. 함수 다형성은 여기에서 다루지 않았는데, 왜냐하면 모든 경우에 있어 같
은 사용법을 사용해야 하기 때문입니다. J, Parte] 대한 참조자를 취해야 합니다.


===== PAGE 763 =====
762 ee 제3주

가상 함수도 여기서 사용하지 않았는데 07000<<이 Part} 멤버 함수가 아니 기
때문입니다. cout << thePatS 호출하기를 원하기 때문에 operator<<= Parto} 멤버
함수로 할 수 없습니다.

이는 실제의 ZS] cout.operator<<(Part&) = 이루어지고 cout Part?) 참조자를
취하는 006010<<의 HAS 가지지 않습니다.

이 한계를 극복하려면 3주의 프로그램은 #의 BAAS 취하는 006010<<를 가
져야 합니다. 이는 다음에 DisplayOS 호출해야 하는데 이는 가상 멤버 함수이고
따라서 올바른 버전이 호출됩니다.

129 - 142번 줄에서 Node7} 템플릿으로 정의되었습니다. 2주 째의 복습 프로그램
에서의 Nodes} 똑같은 BES 구현합니다. 그러나 이번의 80006는 Part 객체에 I
매여 있지는 않습니다. 실제 모든 객체형의 Node7} 됩니다.

예외 사항이 174번 줄에서 발생됩니다.

181 - 196번 줄에서 일반적인 List 템플릿이 정의되었습니다. 이 List 클래스
일한 식별 숫자를 가지는 어떤 객체의 노드도 가질 수 있고 이를 순차적으
열 하여 가지고 있습니다. List 함수의 AAS 예외 사항을 검사하고 필요할 때
예외 사항을 YO AU.

306 - 388번 줄에서 구동 프로그램이 두 가지 Yo] Pat 객체를 만드는데 각 개체
의 값을 표준 스트림 구조를 사용하여 출력합니다.



===== PAGE 764 =====


===== PAGE 765 =====
764 eo 부록

선순위(ㅁ「66606006) 프로그램이 정해
하나의 연산자가 다른 연산자에 비해 우선

Alf

은 순위의 연산자가 낮은 순위으
=a
oH

ㅣ 됩니다. 아래 그림에서

r&
(o7

등급 이름                         연산자
범위 연산자(66006 resolution)
2      멤버 선택, 첨자,                      -). 0)
함수 호출,                                  ()
후치 증가와 감소                        ++ --
3      sizeof, 전치 증가와 감소                  he =
보수, 300, not, 단항 -, 단항 +,           주 |
소환자 주소 계산, new, new(), delete     =
delete), 8 H#,sizeof()               & *
()
4       포인터에 대한 멤버 선택                   그
5      곱셈, Leal, 나머지 연산                */%
6      덧셈, we                           +=
7       비트 이동                              <《< >
8       부등 관계                             ({=))=
9      등치, 부등치                        == |=
10      비트곱                               &
11      비트 배타적 합                       ^
12      비트합                              ㅣ
13      논리곱                               &&
14      논리합                              i

15

HH
[보
2
a
>
~2



===== PAGE 766 =====
순위 ee 765

16

throw

<1

Ol

throw

쉼표

12
18



===== PAGE 767 =====


===== PAGE 768 =====
_Apperid

B

C++ 에의어


===== PAGE 769 =====
768 ce 부록

서문

배약어들은 (+ 언어에 의히컴파원터가 사용하기 위해 만들어진 것입니다, 에야
어와 같은 이름을 가진 클래스나 변수 혹은 함수명 SS 만들 수 없습니다. 여기
에 있는 예약어 목록은 일과벳 순서로 나열한 것이며 어떤 예약어들은 여러분이
사용하는 컴파일러에 안 맞을 수도 있습니다. 따라서 여러분이 사용할 때 조금
달라질 수도 있습니다.

auto
break
case
catch
char
class
const
continue
default
delete
do
double
else
enum
extern
float
for
friend
goto

if

int

long
mutable
new
operator
private
protected
public
register
return
short
signed
sizeof
static
struct
switch



===== PAGE 770 =====
부록 86 C++ 예약어 ee 769

template
this
throw
typedef
union
unsigned
virtual
void
volatile
while


===== PAGE 771 =====
는 패이지입니다



===== PAGE 772 =====
Appe

이진법과 16진법



===== PAGE 773 =====
772 ce 부록

서

그 기초가 없으면

랫동안 기초적인 대수학을 배웠을 텐데 이 PRS
즉시 “백사십오"라고

오랫동안                      ㅣ
이해하기 힘들지도 모릅니다. 145란 숫자를 보면 여러분

H
부분
으
| ay

Hu

이진법과 16진법을 이해한다면 여러분은 1458 다시 살펴보게 되고 이를 숫자
는 것이 아니라 숫자의 코드로 보게 됩니다.

단 간단히 시작하여 봅시다. “3”과 “숫자 Al” 사이의 AAS 살펴봅시다. 3이라
글자는 종이 위에 쓴 것이고 숫자 AS 개념입니다.

차이점은 “3”이 “three”, “I”, “***", 등으로 표현될 수 있지만 전부 같은 개념
을 Yehyuc.

rr ue

은

10진법에서 여러분들은 0 1, 2, 3, 4, 5,
다. 그러면 여기서 숫자 십을 어떻게 프현합니까)
어떤 이는 십을 표현하기 위해     gx                            =
1011011를 사용하여 그 개념을 나타낼 수 있습니다 로마인들은 XS 사용하였습
니다. 우리가 쓰는 아람식에서는 값을 표현하기 위해 숫자들의 AAS 이용합니
다. 맨 오른쪽의 위치는 “일자리” 숫자를 나타내고 두 번째는 “십자리”를 나타냄
니다. 따라서 숫자 ASE 15로 나타내지고 이 의미는 10이 한 개 있고 1이 5개
있는 것을 yepyuc.

이를 일반화시키면 다음의 법칙이 나타납니다.

1. 십진법은 숫자 0 - 9를 사용합니다.

2 각각의 항은 10의 꼽으로 늘어납니다.: 1, 10, 100

3. 세 번째 항이 100이면 두 개의 숫자로 만들 수 있는 가장 큰 수는 99입니다. 일반화시
A 개의 함으로 여러분은 (부터 (10" - 1)까지 만들 수 있습니다. 따라서 3개의 함으
로 여러분은 0 - 999까지 만들 수 있습니다.

다른 7|A5 (Other Bases)

십진법을 쓰는 것은 우연이 아닙니다. 우리는 10개의 손가락을 가지고 있기 때문

다른 기수를 사용할 수 있습니다. 10진법에서 나타나는 법



===== PAGE 774 =====
부록 6 이진법과 16진법 ce 773

1. 8진법에서 사용하는 숫자는 0 - 7 입니다.
2 각 항은 8의 곱씩 SOIC}: 1, 8, 64
3. 개의 항으로 여러분은 (8" - 1)개의 AAS 나타낼 수 있습니다.

각각의 기수로 쓰여진 숫자들을 구분하기 위해 기수를 숫자 오른쪽에 첨자시킴니
다. 10진법으로 15는 1570으로 쓰고 “십진법 일 오”로 읽습니다.

따라서 SoS 8진법으로 나타내면 178이 됩니다. 이는 “gay 일 aro] 됩니다.
또는 이를 십오라고 읽기도 합니다.

왜 17이 됩니까? 이는 한 개의 8과 7개의 1을 Gey ch. 한 개의 gx 7개의 1
은 십진법으로 15와 같습니다.

KKKKK    KKKKK
KKKKK

일반적인 경향은 두 개의 묶음으로 만듭니다. 10개의 묶음과 남은 5개의 Reg
니다. 십진법으로 15입니다. 이를 다음으로 만들 수 었습니다.

KKKK     KRKKKKKK
kKeKK

8개의 별표와 7개의 별표입니다. 이는 17,로 나타낼 수 있습니다.

기수에  내하여

HLS 십진법으로 15로 표현하고 9진법으로는 16, 7진법으로는 21;로 나타냄니다. 7진
법에서는 8이란 숫자가 없습니다. 십진법으로 15를 표현하기 위해 두 개의 7과 한 개의
lo] 필요합니다.

이 과정을 어떻게 일반화할 것입니까? 기수 10을 기수 7로 바꾸려면 항에 대해
생각해야 합니다. 7진법에서는 각 항은 십진법으로 하여 일, 칠, 사십구, 삼백사십
삼 등으로 나갑니다. 이는 7의 0승, 7의 1승, 7의 2승, 7의 3승으로 표현합니다.
테이블을 만들면 다음과 같습니다.

ASS 나타냄니다. 두 번째 SS 7의 곱을 나타냄니다. 세
십진범으로 나타낸 수입니다


===== PAGE 775 =====
7진법으로 나타내려면 몇 개의 과정이 필요합니다. 먼저 숫자를 살펴보
씀것인지 살펴봅니다. 숫자가 200이라면 4번째 항은 0이고(343이
러분은 4번째 항은 생각 안해도 됩니다.
는지 알기 위해 200을 49로 나눔니다. 값은 4이고 따
라서 4를 세 번째 항에 넣고 나머지 4를 봅니다. 4에는 7이 없습니다. 따라서 7의
항에는 0을 써넣습니다. 1의 항에는 남은 4를 넣습니다. 따라서 답은 404입니다.

968을 6진법으로 바꾸어 봅시다.

5          4          3          2         1
6         6°         6°         6'        6"
1296 216       36        6        1

968에는 1296이 들어갈 수 없습니다. 따라서 5번째 항의 값은 0입니다. 968을 216
으로 나누면 4가 남고 나머지는 104입니다. 4번째 BE 4입니다. 104를 36으로 나
누면 2이고 나머지는 32입니다. 3번째 BL 2입니다. 32를 6으로 나누면 Ho] 5이
고 나머지는 2입니다. 따라서 답은 4252/입니다.

2]       4       3       2       1
6°      6      6      6!      6°
1296 216     36      6       1
0       4       2       5       2
이를 10진법으로 다시 바꾸려면 각각을 곱합니다.
4 * 216 = 864
2* 36 = 72
5*6 = 30
2*1 =2
968

| #14 (binary)

이진법이 진수법을 배우는 궁극적인 목적입니다. 2진법에는 단지 2개의 수가 있
습니다. oF 1입니다. 4 항은 다음과 같습니다.
8 7 6 5 4 3 2 1
2 020 020 020 2 2 2 2
128 64 32 16 8 4 2 1

Ez 이> of

88을 2진법으로 바꾸면 1282 안되므로 8번째 항은 0입니다. 88에는 한 개의 64
가 있으므로 7항은 1이고 24가 나머지입니다. 24에는 32가 없으므로 6번째 항도



===== PAGE 776 =====
부록 ¢ 이진법과 16진법 ㅇㅇ 775

a 24에는 하나의 16이 들어가므로 5번째 항은 1이고 나머지는 8입니다. 하
8에 들어감으로 4번째 항은 1이고 나머지는 없습니다. 따라서 나머지

2
ra
Le
ㅇ
=
fos)

1 1 0 0 0

이 ke 검증하기 위해 거꾸로 변환해 봅시다.

1 * 64 = 64
1 * 16 = 16
1*8 = 8

88

왜 이진법을 쓰는가?
2진수는 컴파일러가 표현하고자 하는 체계와 아주 맞아떨어집니다. 사실 컴파일
러는 문자나 숫자, 명령, 프로그램 등에 대해 모릅니다. 그 내부의 핵심에는 회로
가 있을 따름이고 그 표시 방법은 전압이 얼마나 높으냐, 낮으냐 입니다.

위해 기술자는 이를 상대값으로 다루지 않습니다.
“아주 적은 전압, 약간의 전압, 좀 센 전압, 큰 adh” 등으로 다루지 않는다는
뜻입니다. 단지 이항으로 나눔니다. 즉, “충분한 전압과 그렇지 않은 전압"입니다.
이를 바꾸어 보면 “그렇다 와 그렇지 않다"로 나눌 수 있습니다. 이는 YESS} NO
이며 다시 표현하면 1과 0으로 생각할 수 있습니다. 개념상 1은 YES, 0은 NO#
나타낼 수 있습니다. 수많은 OF 1로 모든 회로에 참과 ARS 나타낼 수 있으며
이를 가지고 전압이 있다와 gow VENUE. 모든 컴파일러가 아는 것   있다
=1과 없다=0입니다.

2
대 옷
ats
전
ro
4a
Ac
o tle
ris
ti
as)
ae

rlo 님

비트(610, 바이트(66), -|(nybble)

1과 O22 참과 거짓의 체계가 만들어지면 80084 digits(BITS)7} 매우 중요해집니
다. 옛날의 컴퓨터들은 한번에 8비트 AAs 전송이 가능했고 따라서 8비트를 사
용한 코드를 작성하는 것이 자연스러운 것이었습니다. 이를 바이트라 불렀습니다.

1바이트의 반(4비트)을 니블이라 부릅니다.


===== PAGE 777 =====
776 ee

40
dil

8개의 이진수로 ia 다른 값을 표현할 수 있습니다. 4 항을 살펴보면 알 수
있습니다. 8비트의 모든 값이 1로 되어 있으면 We 255로 됩니다. 아무 것도 A
정되어 있지 않으면(모든 비트가 0) 값은 0입니다. 0부터 255까지의 256개의 표현
방법이 나옵니다.

(란 무엇입니까?
2의 10승은 1024이고 이는 대강 10의 3승하고(1.000) 비슷합니다. 이런 우연의 일
치는 너무 좋아서 그냥 놓치기가 아까웠습니다. 많은 컴퓨터 박사들이 2의 10승
을 1 혹은 1킬로바이트라 하는데 이는 10진법에서 1000을 킬로라고 하는 것과

슷하게 1024 * 102401,048.576)는 백만과 가깝고 따라서 IM 혹은 1메가 바이트
i" 불립니다. 또 1024 메가바이트는 1기가 바이트라 불립니다.

이진수
컴퓨터는 모든 것을 oF 12 암호화합니다. 기계 명령어는 모두 Os} 1의 연결로
이루어지고 기본 회로에 의해 해석됩니다. 임의의 1과 0의 집함들이 컴퓨터 학자

에 의해 SAS 바뀌는데 이 숫자들이 무슨 본질적인 의미를 가진다고 착각하

어, 띠이의 80X6 칩셋은 1001 0101을 명령으로 해석합니다. 여러분은 분명
49로 해석하는데 이는 아무런 의미가 없습니다.
로 숫자는 명령이고 때로는 값이 되고 때로는 그냥 코드입니다. 중요한 표준
드는 4901입니다. 4901에서 모든 문자와 기호는 7자리의 이진 WOE
니다. 예를 들어, 소문자 8는 0110 0001입니다. 이는 숫자가 아닙니다. BS
은 이를 97로 생각할 수도 있습니다. 사람들이 ASCH 코드에서 ‘aS 97로
니다. 사실은 97의 이진 표현 01100001은 문자 '@'로 암호화되고 97은 사람
이 생각하는 값입니다.

00!
뉴 alr

이진수는 읽기가 어려우므로 비슷한 값을 표현하는 Yao] 찾아졌습니다. 이진수
상당한 계산을 요구합니다. 그러나 이진수를 16진수로



===== PAGE 778 =====
FEC 이진법과 67 ee 777

이를 이해하기 위해 여러분은 먼저 16진수를 이해해야 합니다. 16진수에는 16개
의 글자가 쓰입니다 즉 0 4 2, 3, 4 5 6 7, 8 9. A,B, CD, EB F 입니다. 뒤의
OAS] 문자는 임의적인데 ABE] 『까지가 키보드에서 사용되기 쉬워 선택되었습
니다. 16진수의 테이블은 다음과 같습니다.

4    3    2   1

16 16" 16! 16°

4096 256 16  1

16진수를 심진수로 바꾸려면 곱하면 됩니다. PCE 다음과 같습니다.

F * 256 = 15 * 256 = 3840

8*16 =     |  128
C*# 12126 1ㄷ12
3980

(를 이진으로 바꾸는 법은 10진법으로 바꾼 뒤 이를 2진법으로 바꾸는 것입니다.

F* 16 = 15 * 16 = 240
C* 1=12%* 1= 12
252

252를 이진수로 바꾸는 도표입니다.

항              9              8               이             6               5             4            5             2               1
승              28             2"             26            25              34           23           22           2!              20
a              256          128          64           32             16          8             4             2               1

2562 없습니다.

128% 나누어 124 남음
642 나누어 60 남음
32로 나누어 28 남음
16으로 나누어 12 남음
8로 나누어 4 남음

4로 나누면 나머지 없음

따라서 답은 1111 1100 입니다.
이렇게 하고 보니 여러분이 16진수의 수를 4자리의 집합으로 다루면 변환이 아주
쉽게 일어남을 알 수 있습니다. 오른쪽 부분은 1100입니다. 십진수로 12이고 16진
수로 (입니다.


===== PAGE 779 =====
778 eo 부록

수로 #입니다. 따라서 다음과 같이

왼쪽 BRS 1111이고
됩니다.

1111 1100
E   6

십진수로 15이며 16진

이 두 개의 16진수를 같이 쓰면 POV 되고 이는 1111 1100이 됩니다. 이 기법은
항상 맞습니다. 이제 임의의 2진수를 4개로 나눈 뒤 이를 16진수로 쉽게 바꿀 수
있습니다. 여기 아주 복잡한 수가 있습니다.

1011 0001 1101 0111

Zt 항의 값은 1 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384,

32768 입니다.

1* 15       1

1*2 =        2

1*4=        4

0*8=         0

1*16 =      16

0*32 =       0

1* 64 =      64

1 * 128 =      128

1* 256 =     256

0* 512 =     0

0 * 1024 =     0

0 * 2048 =     0

1* 4096 =    4,096

1 * 8192 =    8,192

0 * 16384 =     0

1 * 32768 =     32,768

총계           45,527
이를 16진수로 바꾸려면 16진수 도표가 필요합니다.
65535    4096 256 161

45,527에는 65,535가 없습니다. 따라서 처음
니다. 나머지는

항은 4096입니다. 11개의 4096이 있습
471이고 여기에는 한 개의 256이 있고 나머지는 215입니다. 215에

는 13개의 16이 있고(208) 나머지는 7입니다. 따라서 16진수로 8117입니다.

검산을 하면

sled
=



===== PAGE 780 =====
부록 6 이진법과 16진법 ee 779

B(11) * 4096 = 45,056

1 * 256=      256
D(13) * 16= 208

7 * 1=         7

= >         45,527

이제 간단한 방법으로 연산해 봅시다. 1011000111010111을 각각 4개의 그룹으로
나누어 봅시다. 1011 0001 1101 0111입니다. 각 4개를 다음엔 16진수로 바꾸어 봅

1011 =
1*1= 1
1*2= 2
O*4= 0
1%8= 8
=      11
16진수    B
0001 =
1*※1= 1
0*2= 0
O*4= 0
O*8= 0
중 >    1
16314   1
1101 =

1* 14    1
O*2= 0
1*4h= 4
1*8= 8
총계     13
16진수    0
0111 =
1*1= 1
1*2ㅋ= 2
1*4= 4
0*8= 0
롱계     7
16414   7


===== PAGE 781 =====
다
a
oll
K
re)
=
=

그
i

| 어가



===== PAGE 782 =====


===== PAGE 783 =====
782 ee 부록

1일째

퀴즈

1. 인터프리터는 원시 코드를 읽어 프로그램으로 변환하여 프로그램의 코드와 명령들을 즉시
동작으로 yBUch 컴파일러는 원시 코드를 실행 프로그램으로 바꾸고 나중에 수행을 합니

다.

각 컴파일러마다 다릅니다. 도움말을 참고하도록 합시다.

링커의 역할은 컴파일된 코드들을 컴파일러가 제공하는 라이브러리 및 다른 코드들과 연결

하는 것입니다. 링커는 여러분의 조각된 프로그램을 하나로 묶습니다.

A

wf
ob gu
SW

ro

4.

i
In

입력, 컴파일, 링크, 검사, 반복

연습 문제
1. 두 개의 정수형 변수를 초기화하고 그 HS 출력함
z 컴파일러 안내서를 봅시다.
3. 1001400마는 단어 앞에 # 기호를 넣어야 합니다.
4 Hello Worlds 출력하고 SS sect.

22) Mii

퀴즈

L 컴파일러를 수행할 때마다 전처리계가 먼저 수행됩니다. 여러분의 원시 BEB 읽고 여러분
이 요청한 include HIS 가져오고 다른 잡다한 VS 합니다. 전처리계는 18일짜에 자세
히 설명이 됩니다.       |

2. main()2 여러분의 프로그램이 실행될 때마다 자동적으로 호출됩니다.

3. C++ 형태의 주석인 //는 그 문장의 끝까지 주석으로 처리하고, C 형태의 주석인 /* ...
we 는 그 안의 부분만 주석으로 처리합니다. 후자는 각각이 MS 이루어야 합니다.

그렇습니다. C++ 형태의 주석이 C 형태의 주석 안에 들어갈 수 있습니다. 그 역도 참인

벌어 단 0+ + 형태의 주석은 한 줄로 끝내는 것에 유의합시다.

S.C 형태의 주석을 사용하면 됩니다. C++ 형태의 FAS 사용하려면 각 줄마다 //를 사용
하여야 합니다.



===== PAGE 784 =====
FED 해답편 ee 783

연습 문제

1.

5.

6.
7.

: #include <iostream.h>

: void main()

Aa

cout << "I love C++\n";
return 0;

int main() { return 0; }
AH 줄에서 TASS 감싸는 앞 쌍따옴표가 빠졌습니다.

#include <iostream.h>
main()

cout << “Is there a bug here?”;

1:
2:
32
4                                ,
5: }

ㅇ (02t
re
+>
rir
Ho
rn
ox
4>
flu
ad

Nu 0m
Olt
El
4r
om
b>
+>
[건
0g!
re
4>
rir
n>
>
00
2
ort
Ol
rr
고
-ㅁ
on
[건
no
™

unsigned7} 의미하
정수형은 2바이트이고 1079형은 4바이트입
기호 상수는 그 지

다시 재정의될 수 있습니다.
2

의미입니다. 대부분의 컴퓨터에서 short

i

as
2
으
lu
0
Hu
mz
02
ior
m Oo
A
므
HR
시
fol
o>
+>
rr
to

원시 코드의 다른 Rol
const= 형이 있고 컴파일러가 그 변수를 사용할 때 AAS 합니다. 그리고 전처리계에 의
이 없으므로 이름이 디버거에서 잡힐 수 있습니다.

명은 그 변수가 무엇인지 이름만 SS 압니다. 나쁜 변수명은 정보가 없습니다.
myAget PeopleOnTheBus= 좋은 이름이고 <, prndi= 별로 ot 좋은 이름입니다.
102

rok
02
ok

aa

olf
rlo
fe
4>

8. 좋습니다.

6. 쓸 수 없습니다.


===== PAGE 785 =====
784 66 부록
맞기는 하지만 좋지 않은 이름입니다.
0. 좋습니다.
@. 맞기는 하지만 좋지 않은 이름입니다.

연습 문제
1. a. unsigned short int
b.
C.
d.
2 2.
C:

unsigned long int, unsigned float
unsigned double

unsigned short integer

myAgeb. backYardArea
StarsInGalaxyd. averageRainFall
3. const float P| = 3.14159;

4. float myPi = PI:

4일째

L 반환값을 가지는 문장

, 12

4. 1
5 myAge :
6. 14

41,a:39,b: 41



===== PAGE 786 =====
부록 0 해답편 ee 785

연습 문제

1.
17 (x > y)
= >
else   I-¥> XM =
yY=X;
eH AH: 20,     10,     50
@ 3: «a? 20  6 10  8: 10
13번 SE 대입문이지 등치 연산이 아닙니다
§ 5번 줄이 a-bS col] 대입합니다. cE 0이고 [는 거짓이 되며 따라서 아무것도 출력이 없

은          것입니다. 정의는 그 함수를 정의하는 것입니다. 원형은 세미
콜론으로 끝나고 정의는 그러면 안됩니다. MAS 예약어 inlineS 가질 수 있고 매개 변수
에 대한 기본값을 가질 수 있지만 정의는 안됩니다. MAS 매개 변수의 이름을 가질 필요
가 없지만 정의는 가져야 합니다.
2 아닙니다. 모든 매개 변수는 위치에 의해 식별되지 이름에 의해 되는 것이 아닙니다.
3. voids 반환하게 합니다.
4 기본값으로 정수형을 반환합니다.

$ 특정 블록으로 전달되거나 블록 안에서만(보통은 함수) 사용되는 변수입니다. 블록 안에서
6. 지역 변수       변수가 나타나고 생명을 가지는 위치를 HEU ch. 일반적으로 한 쌍의

합니다. ++에서는 매우 Seu

|
접근할 때 필요
을       HES 거의 쓰지 않게 됩니다.

다. 일단 정적 클래스 변수를 만 변
9. 같은 이름을 가지나 매개 변수의 형과 개수에서 구별이 되는 함수들을 사용할 수 있는 기능
을 말합니다.

객체들을 그 상이성에 관계하지 않고 다
래스의 파생 기능과 가상 함수 기능을 사

음
i  i


===== PAGE 787 =====
786 eo 부록

연습 문제

1.

unsigned Long int Perimeter(unsigned short int, unsigned short int);

2.

unsigned long int Perimeter(unsigned short int length, unsigned short

1

nt width)

{

return 2*length + 2*width;

>

3

4.
5.

\010형으로 선언되어 값을 반환할 수 없습니다. myFuncdl ints 전달하는

를 전달하여야 합니다.

ey 뼈
좋기는

한데 함수 정의 부분에 세미콜론이 있습니다.

것이 아니라 x

short int Divider(unsigned short int valOne, unsigned short int valTwo)
{

#

typedef unsigned short int USHORT;

t
8

1

af

if (valTwo == 0)
return -1;
else
return valOne / valTwo;

include <iostream.h>

ypedef unsigned long int ULONG;
hort int divider (
unsigned short int valone,
unsigned short int valtwo);
nt main()

USHORT one, two;
short int answer;

cout << "Enter two numbers.\n Number one:

cin >> one;
cout << "Number two: ";
cin >> two;
answer = Divider(one, two);
if (answer > -1)
cout << "Answer: " << answer;
else

cout << "Error, can't divide by zero!";

return 0;



===== PAGE 788 =====
부록 0 해답편 ㅇㅇ 787

7.

#include <iostream.h>
typedef unsigned long ULONG
typedef unsigned long int ULONG;
ULONG GetPower (USHORT n, USHORT power);
int main()
{
USHORT number, power;
ULONG answer;
cout << "Enter a number: ";
cin >> number;
cout << "To what power? ";
cin >> power;
answer = GetPower (number, power);

cout << number << "to the " << power << "th power is " << answer << endl;
return Q;

ULONG GetPower (USHORT n, USHORT power)
{
if (power == 1)
return n;
else
return (n * GetPower(n, power-1));

6일째

퀴즈

S

7.

점 연산자는 점(.)입니다. 클래스의 WHS 접근하는데 사용됩니다.

정의할 때 메모리가 준비됩니다. 선언에는 메모리가 할당되지 않습니다.
MAS 인터페이스입니다. 클래스의 클라이언트에게 클래스와 어떻게 상호 작용할 것인지
려줍니다. 클래스의 PHS 저장된 멤버 함수입니다. 대부분 CPP 파일에 저장됩니다.

용 자료 멤버는 클래스의 클라이언트로부터 접근이 가능하고 AS Wee 해당 클래스의
멤버 함수에 의해서만 접근이 가능합니다.

ne Ww ¢

건
Hu
rr
n=
00
으
mia,

>
rae}
cS
ES
2
min
[것

야0
jo 0
Hu

[무

|
KI
ia

>

Hu

2

DE

야0

[건

ru

ney


===== PAGE 789 =====
788 eo 부록

8 클래스 MAS 마감 SBS 다음에 세미콜론으로 끝납니다. 함수 AAS 그렇지 않습니다.
9. void Cat::Meow()
10. 클래스를 초기화하기 위해 생성자가 호출됩니다.

연습 문제

1.

class Employee

{
int Age;
int YearsOfService;
int Salary;

3;

2.

class Employee

{

public:
int GetAge() const;
void SetAge(int age);
int GetYearsOfService() const;
void SetYearsOfService(int years);
int GetSalary() const;
void SetSalary(int salary);

private:
int Age;
int YearsOfService;
int Salary;

3;

3.

main()

{
Employee John;
Employee Sally;
John.SetAge (30) ;
John.SetYearsOfService(5);
John.SetSalary (50000) ;

Sally.SetAge(32);
Sally.SetYearsOfService(8);
Sally.SetSalary (40000) ;



===== PAGE 790 =====
부록 0 해답편 ee 789

cout << "At AcmeSexist company, John and Sally have the same jobs \n";
cout << "John is " << John.GetAge() << " years old and he has been with";
cout << "the firm for " << John.GetYearsOfService << " years.\n";

cout << "John earns $" << John.GetSalary << " dollars per year.\n\n";
cout << "Sally, on the other hand is " << Sally.GetAge() <<" years old and
cout << "been with the company " << Sally.GetYearsOfService;

cout <<" years. Yet Sally only makes $" << Sally.GetSalary();

cout << " dollars per year! Something here is unfair."; return OF

4.

float Employee: :GetRoundedThousands() const
{

return Salary % 1000;
}

5.

class Employee
€
public:
Employee(int age, int yearsOfService, int salary);
int GetAge()const;
void SetAge(int age);
int GetYearsOfService()const;
void SetYearsOfService(int years);
int GetSalary()const;
void SetSalary(int salary);
private:
int Age;
int YearsOfService;
int Salary;
3;

6 클래스 AAS 세미콜론으로 끝나야 합니다.

7 SEA GetAgeQE 전용입니다. 기억합시다. 모든 클래스 멤버는 다른 말이 없으면 전용

입니다.
8. itsStatione 전용이므로 직접 접근할 수 없습니다.
클래스에서 SetStation()S    할
16651[81101이 MAX} 없으므로 초기화할 수 ga

Lt 4
tel



===== PAGE 791 =====
790 ee 부록

7일째

퀴즈
1. 쉼표로 분리하여 초기화합니다.
for (x = 0, y = 10; x < 100; x++, y++)

2 goto: 원시 코드의 아무 BOS 갑니다. 따라서 이해하기가 어렵고 유지, 보수가 어렵습니

다.
3. 가능합니다. 초기화 후 조건이 ARO for 순환문의 몸체가 실행이 되지 않습니다. 예를
봅시다.

for (int x = 100; x < 100; x++)

4 가능합니다. 어떤 순환문도 다른 순환문 안에서 SHO] 가능합니다.
§ 다음에 끝나지 않는 for Zz \/1116문을 만들었습니다.
for 6052
x
// 끝나지 않은 fork
}
while(1)
5
// 끝나지 않는 whilee
가

6 프로그램이 중지되지 않으므로, 보통 컴퓨터를 UCVt 다시 켜야 합니다.

cc
연습 문제
1. 100
2.
for Cint i = 0; i< 10; it+)
{
for ( int j = 0; j< 10; j++)
cout << "0";
cout << "\n";

3.
for (int x = 100; x <= 200; x += 2)



===== PAGE 792 =====
7

8일째

int x = 100;
while (x <= 200)
XS 25

int x = 100;
do
t
×+= 27
} while (x <= 200);

counter 증가하지 않고 따라서 whileZo] 끝나지 않습니다.

순환문 뒤에 세미콜론이 있으므로 몸체가 실행되지 않습니다. 만일 이것이 의도된 과정이라
면 값을 출력하는 것은 의미가 없습니다.

counter7} 100으로 초기화되었습니다. 그런데 검사 조건에서는 counter7} 10보다 작은
경우를 검사하므로 따라서 몸체는 실행되지 않습니다. 첫 번째 줄이 counter = 5;로 yA
다면 순환문이 정수형의 가장 작은 수를 지나 다른 수로 될 때까지는 순환문이 끝나지 않습
니다. 정수형은 기본값으로 양/음수 값을 가지므로 원하지 않는 결과가 발생할 수 있습니다.
case 0에서 break7} 필요합니다. 그렇지 않다면 주석에서 밑으로 가라고 할 것입니다.

주소 연산자(&)가 쓰입니다.

조회 연산자(*)가 사용됩니다.

다른 변수의 주소를 가지는 변수입니다.

포인터에 저장된 주소는 다른 변수의 주소입니다. 그 주소에 저장된 값은 임의의 값이 될
수 있습니다. 간접 지정 연산자(*)는 그 주소에 저장된 값을 돌려주는데 그 poss 쪼인터

「

const int * ptrOne= prtOneo| 상수 정수형을 가리키는 포인터임을 선언합니다. 이 정
T= 포인터를 사용하여 바꿀 수 없습니다.

int “ const ptrTwoE ptrTwo7} 정수형을 가리키는 상수 포인터임을 LpEpHL|c} 일단
초기화되면 포인터에 저장된 주소값을 바꿀 수 없습니다.



===== PAGE 793 =====
792 ee HE

연습 문제
ha: 정수형을 가리키는 포인터를 선언합니다.
6 : 정수형 변수를 선언합니다.
6 : 정수형 포인터를 선언한 뒤 다른 변수의 주소로 초기화합니다.
2 unsigned short *pAge = &yourAge:
3. *pAge = 50:
4.

int theInteger;
int *pInteger = &theInteger;
*pInteger = 5;

pint 초기화되었어야 합니다. 중요한 것은 초기화가 안되어 어느 적절한 주소를 가리키지
=  므로 메모리 상의 아무 곳이나 가리키고 있다는 것입니다. 따라서 9를 그 아무 곳에 저
장하는 것은 버그입니다.

6. 버그잡기
아마 프로그래머는 OB pVar7t 가리키는 주소에 저장하려 했을 것입니다. 불행히 9는
pVar 값에 저장이 되었습니다. * 가 없기 때문입니다. pVaroll 값이 할당되어 있다면 재앙
을 초래합니다.

9일째

퀴즈

L 참조자는 객체에 대한 새 별칭이고, 포인터는 주소를 가지는 변수입니다. 참조자는 널값을
가질 수 없으며 대입이 안됩니다.

2. 포인트되는 값을 다시 할당할 때나 포인터가 널일 때 사용합니다.

3. 널 포인터

4. 상수형 객체에 대한 참조자를 줄인 말입니다.

5. 잠조자에 의해 전달하는 것은 지역적인 복사를 하지 않습니다. 복사는 참조자를 전달할 때
생김니다.

연습 문제
1.

int main()
{



===== PAGE 794 =====
부록 0 해답편 ㅎㅎ 793

2.

int varOne;
int& rVar =
int* pVar =
rVar = 5;
*pVar = 7;
return 0;

varOne;
&varOne;

int main()
af
int varOne;
const int * const pVar =
varOne=6;
*pVar = 7;
int varTwo;
pVar = &varTwo;
return 0;

&varOne;

vy

3% STS 객체에 값을 할당할 수 없습니다. 상수형 포인터에 값을 재할당할 수 없습니다.
4

5.

6.

int main()

£
int * pVar;
*pVar = 9;
return 0;

int main()
{
int VarOne;
int * pVar = &varOne;
*pVar = 9;
return 07;

#include <iostream.h>

int FuncOne();
int main()
{

int * lLocalVar = FunOne();


===== PAGE 795 =====
794 eo 부록

7.

9.

cout << "the value of localVar is: " << * lLocalVar << endl;
return 0;

int FunOne()

ie
int * pVar = new int (5);
return *pVar;

#include <iostream.h>

int FuncOne();

int main®)

t
int theInt = FunOne();
cout << "the value of pInt back in main is: " << theInt << endl;
return 0;

int FunOne()

6
int * pVar = new int (5);
cout << "the value of *pVar is: " << *pVar << endl;
delete pVar

}

MakeCat2 자유 기억 공간에서 만들어진 CATS 반환합니다. 이 메모리를 놓아
없고 따라서 메모리 누출이 일어납니다.

해
0뚜
re
2

1: #include <iostream.h>

28

3: class CAT

4: {

5: public:

6:    CATCint age) { itsAge = age; }
(고    “CAT(){}

8:    int GetAge() const { return itsAge;}
9: private:

10:   int itsAge;

118 +3

12s

13: CAT * MakeCat(int age);
14: int main()
15: <



===== PAGE 796 =====
부록 0 해답편 ee 795

16:    int age = 7;

17%   CAT * Boots = MakeCat (age);

18:   cout << "Boots is " << Boots->GetAge() <<" years old\n";
19:   delete Boots;

208   return 0;

215 0

22: CAT * MakeCat(int age)

252 -¢

24:   return new CAT(age);

258 고

10일째

퀴즈

1

의 형이나 개수에서 차이가 납니다.
% 정의는 메모리를 할당하여 놓는 반면 선언은 아닙니다. 대부분의 경우에 선언하면서 정의합
니다. 예외의 경우는 클래스 선언, 함수 원형, typedef 문장에서 일어납니다.
3 객체의 임시 복사가 만들어질 때입니다. 객체가 값으로 전달될 때 항상 일어납니다.
4.7 객체가 소멸될 때 소멸자가 호출됩니다. 이는 객체가 범위를 벗어나거나 그 객체를 포인
트하는 포인터에 delete AMS 하였을 때 일어납니다.

입 연산자는 이미 존재하는 객체에 대해 만들어지고 복사 연산자는 새로운 것을 하나 만

니다.

중접된 멤버 함수는 같은 OSS 공유하는 클래스 안에 있는 함수입니다. 하지만 매개 변수
신

n
qn 2

6. 자기 객체 그 자신을 “rele 포인터로 모든 멤버 함수에 감추어져 있습니다.
7 전치 연산자는 매개 변수가 없습니다. 후치 연산자는 하나의 정수형 매개 변수를 취하는데
컴파일러에게 sa] 위한 신호입니다.

8. 할 수 없습니다. 어떠한 연산자도 내장형으로 중첩할 수 없습니다.
있는
|

% 안됩니다. 여러분의 코드를 읽는 사람이 쉽게 이해할 수 있는 방식으로 중첩되어야 합니다.

10. 없습니다. 생성자 및 소멸자와 마찬가지로 반환값을 가지지 않습니다.

연습 문제
1.

class SimpleCircle
{


===== PAGE 797 =====
796 eo 부록

public:
SimpleCircle();
“SimpleCircle();
void SetRadius(int);
int GetRadius();

private:
int itsRadius;

3;

2.

SimpleCircle::SimpleCircle():
itsRadius(5);
{}

3

SimpleCircle::SimpleCircle(int radius):
itsRadius(radius);
{}

SimpleCircle SimpleCircle::operator++()
{

++itsRadius;

return *this;
}

SimpleCircle SimpleCircle::operatortt Cint)
{

itsRadiustt+;

return *this;

class SimpleCircle
xf
public:
SimpleCircle();
SimpleCircle(int);
“~SimpleCircle(Q);
void SetRadius(int);
int GetRadius();
SimpleCircle operatort+();
SimpleCircle operator+t(int);
private:
int *itsRadius;
3;



===== PAGE 798 =====
부록 0 해답편 ee 797

7.

SimpleCircle::SimpleCircle()
{ itsRadius = new int(5); }

SimpleCircle::SimpleCircle(int radius)
{ itsRadius = new int(radius); }

SimpleCircle SimpleCircle::operatort++()
{

(*itsRadius)++;

return *this;
0

SimpleCircle SimpleCircle::operator++(int)
{

(*itsRadius) ++;

return *this;
}

SimpleCircle::SimpleCircle(const SimpleCircle & rhs)
t

int val = rhs.GetRadius();

itsRadius = new int(val);

SimpleCircle& SimpleCircle::operator=(const SimpleCircle & rhs)
t
if (this == &rhs)
return *this;
*itsRadius = rhs.GetRadius();

#include <iostream.h>

class SimpleCircle

{

public:
// 생성자
SimpleCircle();
SimpleCircleCint);
SimpleCircle(const SimpleCircle &);
“SimpleCircle() {}


===== PAGE 799 =====
798 ee BE

/7 접근작 함수
void SetRadius(int);
int GetRadius()const;

// operators

SimpleCircle operatortt();

SimpleCircle operatort+(int);

SimpleCircle& operator=(const SimpleCircle &);

private:
int *itsRadius;
3;

SimpleCircle::SimpleCircle()
{ itsRadius = new int(5); }

SimpleCircle::SimpleCircle(int radius)
{ itsRadius = new int(radius); }

SimpleCircle::SimpleCircle(const SimpleCircle & rhs)
{

int val = rhs.GetRadius();

itsRadius = new int(val);
가
SimpleCircle& SimpleCircle::operator=(const SimpleCircle & rhs)
{

if (this == &rhs)

return *this;
*itsRadius = rhs.GetRadius();
return *this;

SimpleCircle SimpleCircle::operator++t()
{

(xitsRadius) ++;

return *this;

SimpleCircle SimpleCircle::operatort++ (int)
{
(xitsRadius) ++;
return *this;
}
int SimpleCircle::GetRadius() const
{
return *itsRadius;



===== PAGE 800 =====
FED 애답편 ee 799

}

int main()

{
SimpleCircle CircleOne, CircleTwo(9);
CircleOnet+;
++CircleTwo;
cout << "CircleOne: " << CircleOne.GetRadius() << endl;
cout << "CircleTwo: " << CircleTwo.GetRadius() << endl;
CircleOne = CircleTwo;
cout << "CircleOne: " << CircleOne.GetRadius() << endl;
cout << "CircleTwo: " << CircleTwo.GetRadius() << endl;
return 0;

}

9 rhs7} this* 같은지 검사하여야 합니다.

10. operator +7} 연산체 중 하나를 HBC}. 합계를 가지고 새로운 VeryShortS 만들어야

합니다. 다음을 봅시다.

VeryShort VeryShort::operator+ (const VeryShort& rhs)
ne

return VeryShort(itsVal + rhs.GetItsVal());
}

11일째

퀴즈

I. SomeArray(0), SomeArray(24)

2 2 차원에 대해 첨자 집합을 만듭니다. 예를 들면, SomeArray(2)(3) (2 3차원 배
니다. 처음 AAS 2개의 ALS 가지고, 두 번째 차원은 3개, 3번째 차원은 2개의 원
가집니다.

3 SomeArray(2) (3) (2) = { { {1,2}, {3,4}, {5,6} }, { {7,8}, {9,10}, {11,12}

410 * 5 * 20 = 1,000

fe= Te}
=
AS
pal 즐

) hs

$ 고정된 개수가 없습니다. 여러분의 컴퓨터가 얼만큼의 메모리를 가졌냐에 달려 있습니다.

6 여러분의 클래스가 연결 YASS 가지고 첨자 연산자를 SHS 때 첨자 기호를 사용할 수

있습니다.

AA
7 널 문자


===== PAGE 801 =====
800 ee FE

연습 문제
1. int GameBoard(3) (3);
2 int GameBoard(3)(3) = { {0,0,0}, {0,0,0}, {0,0,0} }
3.

class Node

{

public:
Node ();
Node (int);
void SetNext(Node * node) { itsNext = node; }
Node * GetNext() const { return itsNext; }
unsigned short int GetVal() const { return itsVal; }
void Insert(Node *);
void Display();

private:
unsigned short int itsVal;
Node * itsNext;

};

4. 배열이 5*4 배열입니다. 그런데 코드에서는 4 * 52 초기화하였습니다.
6 | < 5 대신 ㅣ (= 5B 사용하였습니다. 이렇게 하면 |가 5, )가 4일 때 실행하는데
SomeArray(5) [4)와 같은 원소는 없습니다.

12일째

퀴즈

L v-table 혹은 가상 함수 테이블은 + +에서 컴파일러가 가상 함수를 다루는 방식에 사
되는 테이블입니다. 이 테이블은 모든 가상 함수의 주소 목록을 가지고 실행시 포인트하
객체의 형에 의거하여 적절한 함수를 호출합니다.

2. 임의의 클래스의 소멸자는 가상으로 선언될 수 있습니다. 포인터가 삭제되었을 때 객체의
실행형이 접근되고 적절한 파생 소멸자가 호출됩니다.

3. 가상 생성자란 없습니다.

4. 여러분의 클래스에 가상 메쏘드를 만들면서 그 자체가 복사 생성자를 호출합니다.

§. Base: :FunctionName():

rir 00

6. FunctionName():
7. 그렇습니다. 가상성은 상속이 됩니다.

8. 전용 멤버는 파생된 객체의 멤버 함수에 의해 접근될 수 있습니다.



===== PAGE 802 =====
부록 0 EH ee 801

연습 문제

1.
virtual void SomeFunction(int);
2.
class Square : public Rectangle
(35
3.
Square::Square(int Length):
Rectangle(length, length) {}
4.
class Square
af
public:
7200
virtual Square * clone() const { return new Square(*this); }
ip hee
3;

$ 아마도 없는 것 같습니다. SomeFunctionS Shape 객체를 기대하였습니다. Rectangle
을 잘게 쪼개어 Shape 전달하였습니다. 여러분이 Rectangle #2E 필요로 하지 않는
한, 이는 잘 될 것입니다. 여러분이 RectangleS 필요로 하면 SomeFunctionS Shape
에 대한 참조자나 포인터를 가지도록 바꾸어야 합니다.

& 복사 생성자를 가상으로 선언할 수 없습니다.
13일째

퀴즈

1. 다운캐스트(캐스트다운)이란 베이스 클래스에 대한 포인터가 파생 클래스에 대한 포인터처
럼 다루어지는 것을 말합니다.

2 v-ptr 혹은 가상 함수 포인터란 가상 함수의 세세한 구현을 말합니다. 가상 함수의 클래스
에서 각 객체는 v-ptrS 가지고 있는데 해당 클래스에 대한 가상 함수의 테이블을 포인트
합니다.

3. 만일 아무 클래스도 예약어 1[48!을 사용하여 상속되지 않았다면 두 개의 511806가 만들
어집니다. 하나는 Rectangle 위해 다른 하나는 Shape 위해서 입니다. 두 개의 클래
스에 virtual] 사용되었다면 단지 하나의 공유된 Shape7t 만들어집니다.


===== PAGE 803 =====
802 ee FE

4. Horse2t Bird S 다 그들의 베이스 클래스 AnimalS 각각의 생성자 안에서 초기화합니
다. ㅁ608545도 역시 그러는데 Pegasus7} 만들어질 때 HorseS} Bird2| Animaloll 대
한 초기화가 무시됩니다.

5.

class Vehicle
{

virtual void Move() = 0;
}

6 여러분이 클래스를 비추상형으로 만들지 않는 한 아무것도 중복되지 않는데 이 경우 Al 개
모두가 중복되어야 합니다.

연습 문제
1.

class JetPlane : public Rocket, public Airplane;

class 747 : public JetPlane;

3.
class Vehicle
{
virtual void Move() = 0;
virtual void Haul() = 0;
3;

class Car : public Vehicle
{
virtual void Move();
virtual void Haul();
};

class Bus : public Vehicle
ae
virtual void Move();
virtual void Haul();
3;

class Vehicle
{
virtual void Move() = 0;



===== PAGE 804 =====
부록 ㅁ 해답편 ee 803

virtual void Haul() = 0;
};

class Car:
{
virtual void Move();

public Vehicle

J;

class Bus :
{

public Vehicle

virtual void Move();
virtual void Haul();
};

class SportsCar :
af

public Car

virtual void Haul();
3;

class Coupe :
t

public Car

virtual void Haul();
3;

14일째

퀴즈

1,

그렇습니다. 정적 멤버 변수
루어집니다. 전용이면 단지 멤버 힘
멤버 함수에 의해서

전근된

접근됩니다.

static int itsStatic;

static int SomeFunction();

long (* function) (int);

다른 경우와 마찬가지로 다
더 일반적으로 말하면 정적


===== PAGE 805 =====
804 ee 부록

5.

Long (* Car::function) (int);

6.
(long (* Car::function) (int) theArray[10];

class myClass
{
public:
myClass();
“myClass();
private:
int itsMember;
static int itsStatic;

CONAOU FWD —
seen ee ee ee oe ne oe

= 0
oO
os

a7

=
=
o.

myClass::myClass():
itsMember (1)
{

6 5. =
WM

itsStatictt;

-_- — —
NOU
eee oe

ro)

myClass::~myClass()
{
itsStatic==;

— 기
‘oO 00

nm Mm
- oO
vw

nm mM
WN
ae …

int myClass::itsStatic = 0;

int main()
{ return 0; }

6090 0602
ue

#include <iostream.h>

class myClass

{

public:
myClass();
“myClass();
void ShowMember ();

CONBDU FWD =
…… ee ee ee ee ……"



===== PAGE 806 =====
부록 0 해답편 ee 805

9:     void ShowStatic();
10: private:

10    int itsMember;

123    static int itsStatic;
135% 3;

14:

15: myClass::myClass():
16: itsMember (1)

1s <£

18:    itsStatict+;

192 >}

20%

21: myClass::~myClass()
22: {

23:    itsStatic--;

24:    cout << "In destructor. ItsStatic: " << itsStatic << endl;
251 }

26:

27: void myClass::ShowMember ()
208 <

29:    cout << "itsMember: " << itsMember << endl;
30: }

ST

32: void myClass::ShowStatic()
55:

34:    cout << "itsStatic: " << itsStatic << endl;
35: 개

36: int myClass::itsStatic = 0;
S73

38: int main()

59: £

40:    myClass obj1;

41:    o0bj1.ShowMember ();

42:    obj1.ShowStatic();

43:

44:    myClass obj2;

45:    obj2.ShowMember ();

46:    obj2.ShowStatic();

47:

48:    myClass 0013;

49:    0bj3.ShowMember ();
50:    obj3.ShowStatic();
18    return 0;

52:


===== PAGE 807 =====
806 ee 부록
3.
1:  #include <iostream.h>
a
3: class myClass
6: 1
5: public:
6:     myClass();
ie     “myClass();
8:     void ShowMember ();
9:     static int GetStatic();
10: private:
wake    int itsMember;
12:    static int 1tsStatic;
13: 33
14:
15: myClass::myClass():
16: itsMember (1)
fife <
18:    itsStatictt+;
193 +}
20:
21: myClass::~myClass()
228 +
235%    itsStatic--;
24:    cout << "In destructor. ItsStatic: " << itsStatic << endl;
25: +
26:
27: void myClass::ShowMember ()
28: ¢{
29:    cout << " itsMember: " << itsMember << endl;
30: 7}
34%
32: int myClass::itsStatic = 0;
33:
34: void myClass::GetStatic(
35: +
36:    return itsStatic;
Sf: 3}
38:
39: int main()
40: {
41:    myClass obj1;
42:    obj1.ShowMember () ;
43:    cout << "Static: " << myClass::GetStatic( << endl;
44:
45:    myClass obj2;



===== PAGE 808 =====
부록 ㅁ HEH ee 807

46:
47:
48:
49:
50:
511
52s
531

CONAU FWD =
… ne oe oe … ee …

RP RP RP eS eS eS m= om m2 Oo
OCONDAU FWD SO :
os es se ose os os se ose oe as

NNW DMN DY DY DY WH PF PEP Pw
NV = 2 6 60 기 AU 도 에 00 =

WNW
나

Ww
n

nN
oO
so …

WN
WN
on ee ee …

obj2.ShowMember ();
cout << "Static: " << myClass::GetStatic() << endl;

myClass obj3;

obj3.ShowMember();

cout << "Static: " << myClass::GetStatic() << endl;
return 0;

#include <iostream.h>

class myClass
{
public:
myClass();
“myClass();
void ShowMember ();
static int GetStatic();
private:
int itsMember;
static int itsStatic;
3;

myClass::myClass():
itsMember (1)
{
itsStatictt;
}

myClass::~myClass()
t

itsStatic--;

cout << "In destructor. ItsStatic: " << itsStatic << endl;
}

void myClass::ShowMember ()
4:

cout << "itsMember: " << itsMember << endl;
}

int myClass::itsStatic = 0;
int myClass::GetStatic()

£

return itsStatic;


===== PAGE 809 =====
808 ee FE
375 +}
58:
39: int main()
40: ¢
Als    void (myClass::*PMF) ();
42:
43:    PMF=myClass::ShowMember ;
44:
45:    myClass obj1;
46:    (obj1.*PMF) ();
47:    cout << "Static: " << myClass::GetStatic() << endl;
48:
49:    myClass obj2;
50:    (obj2.*PMF)();
51:    cout << "Static: " << myClass::GetStatic() << endl;
528
55:    myClass obj3;
54:    (obj3.*PMF)();
55%    cout << "Static: " << myClass::GetStatic( << endl;
56:    return 0;
57: >}
5.
1:  #include <iostream.h>
28
3: class myClass
és of
52 public:
6:     myClass();
t:     “myClass();
8:     void ShowMember ();
Oe     void ShowSecond();
10:    void ShowThird();
as    static int GetStatic();
12: private:
15s    int itsMember;
14:    int itsSecond;
15%:    int itsThird;
162    static int itsStatic();
17. Fe
18:
19: myClass::myClass():
205    itsMember (1),
212    itsSecond(2),
22:    itsThird(3)



===== PAGE 810 =====
=D HEH ee 809

24:
225
26:
203
28:
293
30:
S51:
S25
335
34:
55:
36:
37:
38:
598
40:
41:
42:
43:
44:
45:
46:
47:
48:
49:
50:
512
522
538
543
De
56:
Da:
Doe
59:
60:
61:
62:
65:
64:
651
66:
67%
68:
69:

1tsStatictt:
}

myClass::~myClass()
{

TtsStatic-=5

cout << "In destructor. ItsStatic: " << itsStatic << endl;
}

void myClass::ShowMember ()
{

cout <<" itsMember: " << itsMember << endl;
}

void myClass::ShowSecond()
{

cout << " itsSecond: " << itsSecond << endl;
+

void myClass::ShowThird()
€
cout <<" itsThird: " << itsThird << endl;
}
int myClass::itsStatic = 0;

int myClass::GetStatic()
£

return itsStatic;
}

int main()
{
void (myClass::*PMF) ();

myClass obj1;

PMF=myClass::ShowMember;

(obj1.*PMF)();

PMF=myClass::ShowSecond;

(obj1.*PMF)();

PMF=myClass::ShowThird;

(obj1.*PMF)();

cout <<" Static: " << myClass::GetStatic() << endl;

myClass obj2;
PMF=myClass::ShowMember;
(obj2.*PMF)();


===== PAGE 811 =====
810 ee FS

70%    PMF=myClass::ShowSecond;
(13    (obj2.*PMF) ();

(2:    PMF=myClass::ShowThird;
(32    (obj2.*PMF) ();

14:    cout << "St
(on

atic: " << myClass::GetStatic() << endl;

(6:    myClass obj3;

(ts    PMF=myClass:

78:    (obj3.*PMF)

73:    PMF=myCLlass:

80:    (obj3.*PMF)

81:    PMF=myCLlass:

82:    (obj3.*PMF)
83:    cout << * St
84:    return 0;
85: }

15일째

퀴즈
1 범용 상속에서 만들어짐
2 포함에서 일어납니다. 즉
3. 포함은 하나의 클래스가

BAS 위해 하나의 클래스가 다른

에 의해 수행됩니다.
4 대리는 어떤 목적을 위해
로 구현됐습니다.'라는 것
$ 프랜드 함수란 여러분의
fe}

입니다.

6 프랜드 클래스란 모든 멤버 함수가 여러분

말합니다.
7 아닙니다. 프랜드
8 아닙니다. 프랜드

뿌 뽀
고 + 고

내   lr 타

9. 아닙니다. 프랜
10. 클래스 선언의 아무 곳어
ㅁ

r
10
rH
=

: ShowMember ;
C) 3
: ShowSecond;
3
:ShowThird;
O«

atic: " << myClass::GetStatic() << endl;

하나의 클래스가 다른 형의 객체를 AHS 가집니다.
다른 형의 객체인 자료 멤버를 가지는 것을 말합니다.
클래스를 사용하는 개념을 말합니다. 대리

|용하는 개념을 Bo

하나의 클래스가 다른 클래스를 A
현을      는 말합니다.

다른 클래스의 구현을 상속받

클래스의 전용과 범용 멤버에 접근할 권

li

fk

전달되지 않습니다.

|서나 나타납니다. AAS public:, protected:,

의 클래스의 프랜드 함수이도록 선언

대리는 어떤

W 조조 Ts
= 종종 포함

하고 -의 용어

[을 가지도록 선언된 함수

된 클래스를

private:2| 접



===== PAGE 812 =====
FSD 애답편 ee 811

연습 문제

class Animal;
{
private:
String itsName;
+;

2.

class boundedArray : public Array
{
LT ams

3

class Set : private Array
{
IT wae

1: #include <iostream.h>

2: #include <string.h>

5:

4: class String

a3 <

6: public:

ts   // 생성자

8:   String();

9:   String(const char *const);

10: String(const String &);

11: “String();

128

13: // overloaded operators

14: char & operator[I](int offset);

15: char operator[Ci(int offset) const;
16: String operator+(const String&) ;
17: void operatort=(const String&);

18: String & operator= (const String &);
19: friend ostream& operator<<( ostream& theStream, String& theString)
20: friend istream& operator>>( istream& theStream, String& theString)
21: // 일반 접큰자

22: int GetLen()const { return itsLen; }


===== PAGE 813 =====
012 66 부록

5.

6.

23: const char * GetString() const { return itsString; }
24:

20%

26:private:

27: String (int); // private 생성작

28: char * itsString;

29: unsigned short itsLen;

30:

3110;

328

33:ostream& operator<<( ostream& theStream, String& theString)
34:¢

35: theStream << theString.GetString(;

36: return theStream;

378 +

358:

39:istream& operator>>( istream& theStream, String& theString)
40:

41:  theStream >> theString.GetString();

42: return theStream;

43: }

44:

45:int main()

46:

47: String theString("Hello world.");

48: cout << theString;

49: return 0;

50:3
friend AHS 함수 안에 넣을 수 없습니다. 함수는 클래스 안에 프랜드가 되도록 선언하여
야 합니다.

: #include <iostream.h>
: class Animal;

1

2

3

4:

5: void setValue(Animal& , int);
6:

7

8

: class Animal
Oo: ¢
10:public:
11: friend void setValue(Animal&, int);
12: int GetWeight()const { return itsWeight; }
13: int GetAge() const { return itsAge; }



===== PAGE 814 =====
FED 해답편 ee 813

14:private:

15: int itsWeight;

16: int itsAge;

UW ARB a

18:

19:void setValue(Animal& theAnimal, int theWeight)
20:f¢

21: theAnimal.itsWeight = theWeight;
22°)

23:

24:void main()

256

26: Animal peppy;

27: setValue(peppy,5);

28: return 0;

292)

함수 SetValue(Animal&, int)7} friend 선언되었으나 중첩된 함수 SetValue
(&2010781&, int, 101)는 friend 선언되지 않았습니다.

: #include <iostream.h>

: class Animal;

1
2
3
4:
5: void setValue(Animal& , int);
6: void setValue(Animal& ,int,int); // 여기에 변화가 있음
rd
8: class Animal

9: <

10: friend void setValue(Animal&, int);

11: friend void setValue(Animal&,int,int
12:private:

13: int itsWeight;

14: int itsAge;

1523

17:void setValue(Animal& theAnimal, int theWeight)
1851

19: theAnimal.itsWeight = theWeight;

20820

23:void setValue(Animal& theAnimal, int theWeight, int theAge)
24:¢
25: theAnimal.itsWeight = theWeight;


===== PAGE 815 =====
814 ee 부록

26: theAnimal.itsAge = theAge;
art 개

28:

29:void main()

30 ¢

31: Animal peppy;

32: setValue(peppy,5);

33: setValue(peppy,7,9);

34: return 0;

35817

16일째

퀴즈

1. 삽입 연산자(<<)란 ostream 객체의 멤버 연산자이고 출력 장치에 쓸 때 사용됩니다.

2, 추출 연산자(>>)는 istream 객체의 멤버 연산자이고 프로그램의 변수에 입력할 때 사용합
니다.

3. 첫 번째 형은 매개 변수 없이 사용하는 것입니다. 이는 찾아진 문자의 값을 반환하고 파일
끝에서는 EOFS 반환합니다.
두 번째 형은 매개 변수로 문자 참조자를 가지는 것으로 그 참조자는 입력 스트림의 다음
문자로 채워집니다. 반환값은 165[『[6817 객체입니다.
세 번째 형은 배열, 얻어질 문자의 최대 개수, 종료 문자 세 개를 취합니다. 이 형태의
get()= 최대 문자의 개수보다 하나 작은 문자를 배열에 채우는데 그 전에 종료 문자를 만
나면 거기서 HSLIch 어떤 APS YS 마지막에 채우고 종료 문자는 버퍼에 Sh74BUCh.

4 cin.read() 이진 자료 PAS 읽는데 AASS|D getline()= istream2 버퍼로부터 읽는
데 사용됩니다.

5. 전체 개수를 출력할 정도로 충분한 폭

6. istream 객체의 참조자

. 열려질 파일명

8 jos::ate= 파일의 끝에 옮겨 놓습니다. 그러나 여러분은 자료의 아무 곳에 쓸 수 있습니다.

연습 문제
1.

1: #include <iostream.h>
2: int main()
수 §



===== PAGE 816 =====
부록 ㅁ 해답편 ee 815

= 그 92 60 4 AU &

6 0 …
ss …"

Oo CONDU FWD =
… ae … … ee oe

CONBDOUPFPWDY =
. ee oe  oe "ㆍ

00 [0 10 [0 — 5 SP SP -ㅡ5 -ㅡ5 a= = -ㅡ3 -ㅡ3 Oo
WNP 2 6 60 이 에 녀 에 에 60 SB 2 이
… 9 9 0 0 … 0 = 0 …… …… … …=… ㆍ

= Sf
: #include <iostream.h>

~

ING x

cout << "Enter a number: ";

cin >> x;

cout << "You entered: " << x << endl;
cerr << "Uh oh, this to cerr!" << endl;
clog << "Uh oh, this to clog!" << endl;
return 0;

: #include <iostream.h>
: int main()
는 ¢

char nameL80];

cout << "Enter your full name: ";
cin.getline(name,80) ;

cout << "\nYou entered: " << name << endl;
return 0;

리스트

: int main()
it

char ch;
cout << "enter a phrase: ";
while ( cin.get(ch) )
{
switch (ch)
t
case '!':
cout << "“$"5
break;
case '#':
break;
default:
cout << ch;
break;
}
4;
return 0;


===== PAGE 817 =====
816 ee 부록

4.
1: #include <fstream.h>
2: enum BOOL { FALSE, TRUE };
3:
4: int main(int argc, charetargv) // 에러 시 1& 반환함.
bs <
6:
(ge   if (arge != 2)
8:   {
oO:      cout << "Usage: argvL[0] <infile>\n";
10:     return(1);
112   }
125
13:  // 입력 스트림을 Se
14: ifstream fin (argv£1],ios::binary);
15: 1) Cltin)
16: ¢<
10     cout << "Unable to open " << 89613 << " for reading.\n";
18:     return(1);
195. }
20:
213 char ch;
22: while ( fin.get(ch))
23°     if ((ch > 32 && ch < 127) || ch == "\n' | | ch == '\n')
24:        cout << ch;

25: fin.close();
26: return 0;
27: I

: #include <fstream.h>

: int main(int argc, char**argv)

= £

for Cint ctr = arge; ctr ;.ctr-)
cout << argvEctr] <<" ";
return 0;

CONAOUFWD
en …… ee a8   ae



===== PAGE 818 =====
부록 ㅁ HEH ee 817

17일째

퀴즈

1. 헤더 파일이 프로그램에 한 번 이상 포함되는 것을 막는데 사용되는 것입니다.

2 O| SAE 여러분이 사용하는 컴파일러 사용법을 보고 여러분이 각각 답해야 합니다.

3. #define debug 0은 debug@t= 용어를 0이 되도록 정의합니다. 06600라는 단어가 나
타나는 곳이면 모두 0으로 바뀌어 집니다. #undef debug= 모든 00600의 정의를 gic
니다. 프로그램에서 debug7} 발견되는 모든 곳이 변화가 없이 그대로 있게 됩니다.

4. 0416, TIME_, _FILE_, LINE __

$ 여러분의 생성자의 역할은 객체를 만드는 것입니다. Saya invariant 객체가 다 만들어
지기 전에는 있어서는 안됩니다. web invariant()2| 사용은 생성자가 완성되기 전까지는
거짓이 됩니다.

연습 문제
1,

#ifndef STRING H
#define STRING H

#endif
2.

#include <iostream.h>

1

2

3: #ifndef DEBUG

4: #define ASSERT(x)
5: #elif DEBUG ==

6: #define ASSERT(x) \
7

8

if G! GODr\
:    tN
a:       cout << "ERROR!! Assert " << #x <<" failed\n"; \
10:   0

11: #elif DEBUG ==
12: #define ASSERT(x) \
135%    if C! GO) \

145   {\

153     cout << "ERROR!! Assert " << #x <<" failed\n"; \
16:      cout << "on line " SS _ LINE. 2<< \ri"7 *\,

Ts      cout <<" in file " < 가 티드 << "\n" 이

18:   Bg

19: #endif


===== PAGE 819 =====
818 eo 부록

#ifndef DEBUG

#define DPRINT(string)

#else

#define DPRINT(STRING) cout << #STRING ;
#endif

: #include <iostream.h>

: void ErrorFunc(
int LineNumber,
const char * FileName)

cout << "An error occurred in file ";
cout << FileName;

cout <<" at Line "

cout << LineNumber << endl;

PB SP OANA UM 은 에 02 =
a

=O0O8
oo ee

: // ErrorFuncS *2|*p| 위한 구동 프로그램

int main(Q)

= 고

cout << "An error occurs on next Line!";
ErrorFunc( LINE , FILE );

return 0;

NOU FWD
ee …‥  oe ㆍ

: #include <iostream.h>
: H#define DEBUG // 오류 처리를 동작시킴

: #ifndef DEBUG
#define ASSERT(x)
#else
: #define ASSERT(X) \
if (§ (80) \
{ \
ErrorFunc( LINE , FILE _); \

CONAU FWD —
on …" oe

=a 8 ~ 0
nm 2
on ee one

}

13: #endif

14:

15: void ErrorFunc(int LineNumber, const char * FileName)



===== PAGE 820 =====
부록 0 애답편 ee 019

168 고

VWs   cout << "An error occurred in file ";
183   cout << FileName;

195   cout << " at Line ";

20:   cout << LineNumber << endl;

21: +

2:

23: // ErrorFuncS 실행하기 위한 구동 프로그램
24: int main()

25:

26:   int x = 5;

el:   ASSERT(x >= 5); // 오류가 아님

28:   x = 3;

29: ASSERT(x >= 5); // 2 FF!

30:   return 0;

이 경우 _LINE_, _ FILE 527} assert() 매크로에서 SSE + 있고 올바른 SH
줄 것입니다. (29H B) 이는 왜냐하면 3566[[() 매크로가 SSE] 곳에서 먼저 확장되기
입니다. 따라서 이 프로그램은 main()o| 다음과 같이 작성된 것처럼 작동합니다.

1: // ErrorFuncS Pes] 위한 구동 프로그램

2: int main()

38 4

4s   int x = 5;

5:   if Cf Gc >= 5)) CErrorFune( LINE...,. ..FILE, ) 7}
6:   x = 3;

7    if (! (x >= 5)) {ErrorFunc(_ LINE, FILE _);}
8:   return 0;

9: 2

18일째

퀴즈
1. EAL 언어는 자료와 분리된 함수에 초점이 맞춰져 있습니다. 객체 지향 프로그래밍은 자료
와 기능을 하나의 객체에 잡아넣고 그 객체 사이에서 상호 작용하게 합니다.
BAU 구동 PAS 행동이 여러분의 키보드나 마우스의 시뮬레이션의 형태로 반응한다는 A}
실에서 구별됩니다.
3. 분석, 설계, 코딩, 검사, 프로그래밍, 각 단계로의 피드백 단계를 포함합니다.
4 순종 계층((00[60 hierarchy)S 프로그램의 모든 Bayar} 하나의 베이스 클래스로부터

직, 간접으로 파생되는 경우를 말합니다.


===== PAGE 821 =====
820 ee FE

$. 현재 여러분이 프로그래밍 하는 객체와 함수를 실행시키는 함수입니다.
6 캡술화는 모든 클래스와 기능을 하나의 구체적인 실체로 묶는 특성을 말합니다.

연습 문제
Ｌ 자동차, 오토바이, 트럭, 자전거, 보행자, 비상 운송 도구 모두가 교차로를 이용합니다. 또
신호등이 있습니다.
도로 면이 시뮬레이션에 포함됩니까? 물론 도로 면의 상태가 교통에 영향을 미치기는 하지
만 처음 설계에서는 이 부분을 뒤로 미룹시다.
첫 번째의 객체는 교차로 그 자체일 것입니다. 교차로 객체는 각 방향으로 신호에 따라 x
나기를 기다리는 차의 목록과 횡단보도를 지나기를 기다리는 사람들의 목록을 가지고 있을
입니다. 얼마나 많은 차와 사람들이 교차로를 지나는지를 선택할 메쏘드를 가지고 있을
입니다.
단 하나의 교차로가 있으므로 Ct 하나의 객체만 인스턴스화 되는 것을 생각할 것입니다.(정
적 메쏘드와 보호 접근자를 생각합시다.)
사람과 차들은 모두 교차로의 클라이언트입니다. 각각 여러 개의 특성들을 공유합니다. 언제
고 나타나 임의의 숫자가 됩니다. 전부 신호를 기다립니다. (물론 각각 다른 Royal) 이를 보
면 보행자와 차에 대해 공통의 베이스 클래스를 가질 수 있다고 생각할 수 있습니다.
클래스는 다음을 포함하여야 합니다.

class Entity; // 인터섹션의 클라이언트

// the root of class Vehicle : Entity ...;

all cars, trucks, bicycles and emergency vehicles.
class pedestrian: Entity...; // 모든 사람의 루트
class Car : public Vehicle...;

class Truck : public Vehicle...;

class Motorcycle : public Vehicle...;

class Bicycle : public Vehicle...;

class Emergency Vehicle : public Vehicle...;

class Intersection; // 지나기를 기다리는 차와 사람의 BES 가짐

2 여기에 대한 합리적인 시작점은 문제에 의해 만들어진 모델의 파생 객체를 만드는 것입니다.

class Local 680『 : public Car...;

class Tourist_Car : public Car...;

class Taxi : public Car...;

class Local Pedestrian : public Pedestrian...;
class Tourist Pedestrian : public pedestrian...;
class Boston Bicycle : public Bicycle...;

~

것
것

가상 메쏘드를 사용하여 각각의 클래스는 자신의 명세를 만족시키는 일반 SAS 수정하여
of 합니다. 예를 들면, 뉴욕의 SAE 여행자에 비해 적색 신호에 대해 다르게 행동할 수
있는데 그럼에도 불구하고 일반적인 동작을 상속받습니다.



===== PAGE 822 =====
부록 0 해답편 ee 821

3. 이 프로젝트에서는 두 개의 분명한 문제가 작성되어야 합니다. 사용자가 수행하는 클라이언
트 기계 부분이고 다른 기계에서 수행되는 서버 부분입니다. 추가로 클라이언트 기계에서는
시스템 운영자가 새로운 사람과 방을 추가할 수 있는 운영 요소를 가지고 있습니다.
이를 서버/클라이언트 모델로 구현하기로 했다면 클라이언트는 사용자로부터 ele 받고

이를 서버기계에 요청합니다. 서버 기계는 요청에 응답하여 결과를 반송합니다. 이 모델에서
는 많은 sol 동시에 ole 조정할 수 있습니다.

클라이언트 부분에서는 운영자 모듈에 추가하여 두 개의 중요한 하부시스템이 있습니다. A}
용자 인터페이스 부분이고 SAAAR 부분입니다. 서버 FRE 세 개의 주요 ste 시스템
이 있습니다. 통신과 스케줄링, 편지 인터페이스 부분인데 편지 부분은 스케줄에 변경이 생
기면 사용자에게 알려주기 위한 것입니다.

4 미팅은 일정 시간 동안 HS 예약하는 사람들의 그룹으로 한정합시다. 예약자는 특정 방이
나 특정 시간을 요구합니다. 그러나 스케줄러는 얼마 동안 미팅이 지속되고 누가 사용할지
를 요구합니다.

객체는 시스템의 사용자와 회의실을 포함합니다. 달력과 특정 사건에 관련되어 알려진 모든
AS WSS class MeetingS 만들도록 합시다.
이 클래스의 원형은 다음과 같습니다.

class Calendar Class; // forward 소환자

class Meeting;        // forward 소환자

class Configuration

{

public:
Configuration();
“Configuration();
Meeting Schedule( ListOfPerson&, Delta Time duration );
Meeting Schedule( ListOfPerson&, Delta Time duration, Time );
Meeting Schedule( ListOfPerson&, Delta Time duration, Room );
ListOfPerson& People(); // 범용 Ha
ListOfRoom& Rooms();    // BRS 범용 접근자
ListOfRoom rooms;
ListOfPerson people;

3;

typedef Long Room_ID;

class Room

n

{
public:
Room( String name, Room_ID id, int capacity,
String directions =" ", String description="" );
“Room();
Calendar Class Calendar();
protected:

Calendar Class calendar;


===== PAGE 823 =====
822 ee 부

dil

int capacity;
Room_ID id;
String name;
String directions; // 방이 어디에 있는가?
String description;
3;
typedef long Person_ID;
class Person
{
public:
Person( String name, Person_ID id );
“Person();
Calendar Class Calendar(); //  meetingeS 추가하| 위한 접근 포인트
protected:
Calendar Class calendar;
Person 10 id;
String name;
3;
class Calendar Class
{
public:
Calendar Class();
“Calendar Class();

void Add( const Meeting& ); // calendar] meetingeS 추가함

void Delete( const Meeting& );

Meeting* Lookup( Time );    // 주어진 시간에 meetinge®] 있는지
// 살펴봄

Block( Time, Duration, String reason="" );
// 시간을 BY...
protected:
OrderedListOfMeeting meetings;
3;
class Meeting
{
public:
Meeting( ListOfPerson&, Room room,
Time when, Duration duration, String purpose =" '" );
“Meeting();
protected:
ListOfPerson people;
Room room;
Time when;
Duration duration;



===== PAGE 824 =====
부록 2 애답편 ee 823

String purpose;

19일째

퀴즈
1. 템플릿은 C+ +에서 USE 것이고 Soll 대해 안전합니다. ASE 전처리계에 의해 만들
어지고 형에 대해 안정성을 보장 못합니다.
2% 템플릿의 매개 변수는 템플릿의 각각의 형에 대해 인스턴스를 만듭니다. 만일 여러분이 6개
의 템플릿 인스턴스를 만들었다면 6개의 다른 클래스나 함수가 만들어집니다. 함수에 대한
매개 변수는 함수에 대한 동작이나 자료를 HHSLCH, 그러나 단지 하나의 함수가 만들어집

니다.
3 일반적인 템플릿 프랜드 함수는 매개 변수화된 클래스의 각 형에 대해 하나의 함수를 만듭
니다. 형 명세 함수는 매개 변수화 된 클래스의 각 인스턴스에 대해 형 명세된 인스턴스를

만듭니다.

4 가능합니다. 특정 인스턴스에 대하여 특정한 함수를 만드는 것이 가능합니다. Array<t)
SomeFunction()ol] 추가하여 각 정수형 배열의 SAS 바꾸도록 Array<int)::SomeFu
만드는 것이 가능합니다.

§ 클래스의 각 인스턴스에 하나씩 만듭니다.

Ol

연습 문제
1. 이 템플릿을 구현하는 한가지 방법입니다.
template <class Type>

class List
{

public:
List():head(0), tail(0), theCount(0) { }
virtual “List();

void insert( Type value );

void append( Type value );

int is_present( Type value ) const;

int is_empty() const { return head == 0; }
int count() const { return theCount; }

private:


===== PAGE 825 =====
824 ee 부록

class ListCell

{

public:
ListCell (Type value, ListCell *cell = 0):val(value), next(cell){}
Type val;
ListCell *next;

3;

ListCell *head;
ListCell *tail;
int theCount;

3;
2.
void List::insert(int value)
%
ListCell *pt = new ListCell( value, head );
assert (pt != 0);
// tail& 처리하기 위해 이 줄이 들어감
if ( head == 0 ) tail = pt;
head = pt;
theCount+t;
J
void List::append( int value )
{
ListCell *pt = new ListCell( value );
if ( head == 0 )
head = pt;
else
tail->next = pt;
tail = pt;
theCountt+t;
}
int List::is_present( int value ) const
nf
if ( head == 0) return 0;
if ( head->val == value |} tail->val == value )
return 1;

ListCell *pt = head->next;
for (; pt '= tail; pt = pt->next)



===== PAGE 826 =====
부록 0 해답편 ee 825

3

if ( pt->val == value )
return 1;

return 0;
P

template <class Type>
List<Type>::~List(
{

ListCell *pt = head;

while ( pt )

{
ListCell *tmp = pt;
pt = pt->next;
delete tmp;

ts

head = tail = 0;

}

template <class Type>

void List<Type>::insert(Type value)

£
ListCell *pt = new ListCell( value, head )
assert (pt != 0);

// taile 처리하기 위해 이 줄이 들어감
if (head == 0 ) tail = pt;

head = pt;
theCountt+;

template <class Type>
void List<Type>::append( Type value )
£
ListCell *pt = new ListCell( value );
if ( head == 0 )
head = pt;
else
tail->nest = pt;

tail = pt;
theCount++;


===== PAGE 827 =====
826 ee 부록

template <class Type>
int List<Type>::is_present( Type value ) const

£
if ( head == 0 ) return 0;
if ( head->val == value |} tail->val == value )
return 1;
ListCell *pt = head->next;
for (; pt != tail; pt = pt->next)
if ( pt->val == value )
return 1;
return 0;
}
4.

List<String> string list;
List<Cat> Cat_List;
List<int> int_List;

§. Cat= 정의된 operator==S 가지지 않습니다. Listoll WE(is_present) 값을 비교하는
모든 연산자는 컴파일러 오류를 발생시킬 것입니다. 이 위험을 줄이기 위해 복사할 수 있는
주석을 어떤 연산이 정의되어야 하는지를 시작하는 템플릿 정의 앞에 넣습니다.

6.

friend int operator==( const Type& Lhs, const Type& rhs 3

7.
template <class Type>
int List<Type>::operator==( const Type& Lhs, const Type& rhs )
{
// 먼저 길이를 비교함
if ( 나타 60040 != rhs.theCount )
return 0; // Lengths differ

ths. head;
rhs.head;

ListCell *lh
ListCell *rh

for(; th != 0; 나 = Lh.next, rh = rh.next )
if ( lh.value != rh.value )
return 0;

return 1; // 다르지 않으면 반드시 일치됨
}



===== PAGE 828 =====
FED HEH ee 827

// swap 템플릿

// 할당을 가져야 하며 복사 생성자가 정의됨.
template <class Type>

void swap( Type& Lhs, Type& rhs)

sf
Type temp( lhs );
나요 = rhs;
rhs = temp;

}

20일째

퀴즈

1. 예약어 throws 사용한 결과 만들어지는 객체입니다. 예외 사항을 알리기 위한 신호인데
그 형을 다루는 AS catch 문장의 호출 스택으로 전달됩니다.

2 try 블록이란 예외를 발생시킬 우려가 있는 문장의 집합입니다.

% catch ESE 그가 다루는 예외형의 사용법을 가지고 있습니다. try 블록에 뒤따라오며 try
블록 내에서 발생하는 예외의 수령자로 동작됩니다.

 객체이므로 사용자가 만든 클래스가 가지는 모든 정보를 가질 수 있습니다.

§. 예약어 throws 부를 때 사용됩니다.

6 일반적으로 예외 객체는 BAAS 전달됩니다. 예외 객체의 SS 바꾸고 싶지 않으면
const 참조자로 전달하면 됩니다.

% 예외 객체를 AAAS 전달하면 그렇습니다.

8. catch ESE 원시 코드에서 나타난 SACHS 살펴집니다. 먼저의 사용법이 일치하는
catch 문장이 사용됩니다.

% catch(....= 모든 형의 모든 예외에 일치됩니다.

10. 디버거가 프로그램 내에서 수행을 중지하는 점입니다.

연습 문제
1.

#include <iostream.h>
class OutOfMemory {};
int main()
af

try


===== PAGE 829 =====
828 ee

브
부록

int *myInt = new int;
if (myInt == 0)
throw OutOfMemory();

}
catch (OutOfMemory)
ne

cout << "Unable to allocate memory! \n";
}
return 0;

#include <iostream.h>
#include <stdio.h>
#include <string.h>
class OutOfMemory
{
public:
OutOfMemory(char *);
char * GetString() { return itsString; }
private:
char * itsString;
3;

OutOfMemory::OutOfMemory(char * theType)

itsString = new char[80];
char warningL1] = "Out Of Memory! Can't allocate room for: ";
strncpy(itsString,warning,60) ;
strncat(itsString,theType,19);

}

int main()

iG
try
{

int *myInt = new int;
if (myInt == 0)
throw OutOfMemory("int");
By
catch (OutOfMemory& theException)
{
cout << theException.GetString();



===== PAGE 830 =====
return 0;
}
3.
1: #include <iostream.h>
ar
3: // Abstract exception data type
4: class Exception
5: 6 Ot
6: public:
ts     Exception() {}
8:     virtual ~Exception(){}
9:     virtual void PrintError() = 0;
10% de
Ts
12: // Derived class to handle memory problems.
13: // Note no allocation of memory in this class!
14: class OutOfMemory : public Exception
{시 £
16: public:
17:    OutOfMemory(){}
18:    “OutOfMemory(){}
19%    virtual void PrintError();
20: private:
ene
22:
23: void OutOfMemory::PrintError()
243 £
Ze    cout << "Out of Memory! !\n";
26% 3
20%
28: // bad numberS 다루기 위해 파생된 클래스
29: class RangeError : public Exception
50: ¢£
31: public:
S25    RangeError (unsigned Long number) {badNumber = number ;}
53:    “RangeError(){}
34:    virtual void PrintError();
35%    virtual unsigned long GetNumber() { return badNumber; }
36:     virtual void SetNumber(unsigned long number) {badNumber = number
37: private:
38:    unsigned long badNumber;
39: J;
40:
41: void RangeError::PrintError()

{


===== PAGE 831 =====
830 eo 부록

AS:    cout << "Number out of range. You used " << GetNumber() << "!!\n";
44: }
45:
46: void MyFunction(); // function prototype
47:
48: int main()
49: {
50:    try
a1    {
525     MyFunction();
538     +
54:     // Only one catch required, use virtual functions to do the
555     // right thing.
56:     catch (Exception& theException)
ei     {
58:       theException.PrintError();
59:     }
60:     return 0;
61: +
62:
63: void MyFunction()
64: {
65:     unsigned int *myInt = new unsigned int;
66:     long testNumber;
67:     if (myInt == 0)
68:       throw OutOfMemory();
69:     cout << "Enter an int: ";
70:     cin >> testNumber;
1:     // this weird test should be replaced by a series
(2:     // of tests to complain about bad user input
(32     if (testNumber > 3768 |; testNumber < 0)
(4:       throw RangeError(testNumber) ;
(5:
16:     *myInt = testNumber;
(le     cout << "Ok. myInt: " << *myInt;
(4     delete myInt;
792 =F
4.
1:  #include <iostream.h>
2:
3:  // Abstract exception data type
4: class Exception
S27
63 public:
t     Exception() {}



===== PAGE 832 =====
= ㅠㅠㅠㅠㅠㅠ ㅠㅠㅠ 조후

FSD EH ee 831

8:     virtual ~Exception(){}

9:     virtual void PrintError() = 0;
10: 3

1318

12: // Derived class to handle memory problems.
13: // Note no allocation of memory in this class!
14: class OutOfMemory : public Exception

15: 에

16: public:

a    OutOfMemory() {}

18:    “OutOfMemory(){}

193    virtual void PrintError();
20: private:

21: 3

22:

23: void OutOfMemory::PrintError()
24: {《

7a    cout << "Out of Memory! !\n";
26: }

a oe

28: // Derived class to handle bad numbers
29: class RangeError : public Exception

305 {

31: public:

328    《80906『『0「(040519060 Long 04066『)1(683084066『 = number ;}

33:    “RangeError(){}

545    virtual void PrintError();

SD:    virtual unsigned Long GetNumber() { return badNumber; }

36:    virtual void SetNumber (unsigned Long number) {badNumber = number
37: private:

38:    unsigned long badNumber;

59: 33

40:

41: void RangeError::PrintError()

a2: {

43:    cout << "Number out of range. You used " << GetNumber() << "!!\n";
44: }

45:

46: // func. prototypes

47: void MyFunction();

48: unsigned int * FunctionTwo();

49: void FunctionThree(unsigned int *);

50:
51: int main()
522 £

53:    try


===== PAGE 833 =====
832 ee FS
54:    1
55.     MyFunction();
56:     +
57:     // Only one catch required, use virtual functions to do the
58:     // right thing.
59:     catch (Exception& theException)
60:    {
61s       theException.PrintError();
62:     7
63:     return 0;
64: }
65: unsigned int * FunctionTwo()
66: ，《
67:     unsigned int *myInt = new unsigned int;
68:     if (myInt == 0)
69:       throw OutOfMemory();
70:     return myInt;
v12 .
Lae
3
74: void MyFunction()
758 <<
TOE     unsigned int *myInt = FunctionTwo();
Cl
(8:     FunctionThree(myInt);
(92     cout << "Ok. myInt: " << *myInt;
80:     delete myInt;
812 3}
82:
83: void FunctionThree(unsigned int *ptr)
84: ¢{
85:     long testNumber;
86:     cout << "Enter an int: ";
87?     cin >> testNumber;
88:     // this weird test should be replaced by a series
89:     // of tests to complain about bad user input
90:     if (testNumber > 3768 || testNumber < 0)
91:        throw RangeError(testNumber) ;
92:     *ptr = testNumber;
95:

class xOutOfMemory
{
public:
xOutOfMemory( const Strings& message ) : itsMsg( message ){}



===== PAGE 834 =====
부록 0 해답편 ee 833

~xOutOfMemory() {}

virtual const String& Message(){ return itsMsg };
private:

String itsMsg;

int main()
{
try
{
char *var = new char;
if ( var == 0 )
throw xOutOfMemory();
}
catch( xOutOfMemory& theException )
{
cout << theException.Message() << "\n";
3
return 0;
}

“out of memory’S 다루는 과정에서 xOutOfMemory 생성자에 의해 string 객체가 만
니다. 이 예외 사항은 메모리가 모자랄 때 발생하므로, 예외사항에서 또 메모리를 요구하면
실패합니다.

이 AAS 같은 예외사항에서 호출하므로, 예외 사항이 또 호출되고 이는 프로그램이 박살날
때까지 무한 순환을 SUCH. 이 stringo| 절실히 필요하다면, 여러분은 프로그램을 시작하
기 전 정적 Huo] 공간을 할당할 수 있습니다. 그리고 예외 사항이 발생할 때마다 이를 at
용합니다.

21일째

퀴즈

1. strspytchat” destination, char* source)= sourceS destinationc= 복사하고 널
= destinationo] 붙입니다. destinationS sources 복사받을 수 있을 만큼 커야 합니

다. 그렇지 않으면 배열을 지나 복사합니다.
strncpy(char* destination, char* source, int howmany)= howmany?!#2| 바이
트만큼 604[06에서 destination©= SAS 하는데 널은 붙이지 않습니다.

2. etiorigiies time_t HFS 취하여 현재의 AZ ASCIl 문자열로 반환합니다. time 변

는 time()O] 그 FAS 전달하여 채워집니다.
3. atol()


===== PAGE 835 =====
834 ee 부록

4 숫자 안의 모든 HES 보수화합니다.
& ORE 둘 중 하나가 참이면 참을 반환합니다. 배타적 ORE 하나만 참일 때 첨
다. 두 개 다 참일 땐 거짓입니다.
6 &는 비트곱 연산자이고 &&E 논리곱 연산자입니다.
연

7 |는 비트합 연산자이고 ||는 논리합

연습 문제
1.

: #include <iostream.h>
: #include <string.h>

1
2
Bs
4: int main(Q)

56 <

6:   char bigString[21] = "12345678901234567890";
7    char smallStringl10];

8%   strncpy(smallString,bigString,9);

9:   smal lStringL9J='\0';

10: cout << "BigString: " << bigString << endl;
11: cout << "smallString: " << smallString << endl;
12: return 0;

13:3
2.
1: #include <iostream.h>
2: #include <time.h>
St
4: int main(Q)
as <
6:   time_t currentTime;
4    struct tm *timeStruct;
8    time(&currentTime) ;
9s   timeStruct = localtime(&currentTime) ;
10:

11: cout << timeStruct->tm_mon+1 << oy ale
12: cout << tiemStruct->tm_mday << "/";
13: cout << timeStruct->tm_year <<" ";
14: return 0;

158가

#include <ctype.h>
#include <iostream.h>



===== PAGE 836 =====
SSD 애답편 ee 835

class Bits

i

public:
enum { BITS PER_INT = 16 };
Bits( int cnt );
virtual ~Bits();

void clear();
void set( int position );
void reset( int position );
int is_set( int position );
private:
unsigned int * bits;
int count;
int Ints_Needed;
3;

class AlphaBits : private Bits
Xt
public:
AlphaBits() : Bits( 26 ){}
“AlphaBits(){}

void clear() { Bits::clear(); }
void set( char );
void reset( char );
int is_set( char );
3;

Bits :: Bits( int cnt ) : count( cnt )

{
1065 Needed = count / BITS PER_INT;
// 나러지가 있으면, 배열에 하나의 멤버가 머 필요
if ( 0 != count % BITS PER_INT )

Ints Needed++;

// 모든 비트를 가질 수 있는 정수형 배열 생성함
bits = new unsigned intL 1015 Needed J;
clear();

}

Bits <2 “Brts:©)
{
delete [J] bits;



===== PAGE 837 =====
836 eo 부록

void Bits :: clear()

{

// 비트를 깨끗이 함
for ( int i = 0; i < Ints Needed; 1++ )
61156 iJ =

void Bits :: set( int position )

// 설정할 비트를 찾음
int Int_Number = position / BITS PER_INT;
int Bit_Number = position % BITS PER_INT,;

// create mask with that one bit set
unsigned int mask = 1 << Bit_Number;

// 비트 A 설정
61156 Int_Number J] {= mask;

// 비트 깨끗이 함

void Bits :: reset( int position )

내

가

int Int_Number = position / BITS PER_INT,;
int Bit_Number = position % BITS PER_INT;

unsigned int mask = ~( 1 << Bit_Number );
bits Int_Number J] & mask;

void Bits :: is_set( int position )

if

}

int Int_Number = position / BITS PER INT;
int Bit Number = position % BITS PER _. INT;

unsigned int mask = 1 << Bit_Number;

return (0 != ( bits£ Int_Number ] & mask ) );

void AlphaBits :: set( char 5 )

{

// SAB 문자가 알파벳 문자인지를 Tol st
// 만일 그렇다면 소문자로 PE ‘a's asciitte MFT
// 처음 시작값 (< ㅎ= 0, 6 =1 )으로 만든 뒤 그 비트로 설정함
if ( isalpha( s ) )

Bits :: set( tolower( s ) - 'a' );



===== PAGE 838 =====
void AlphaBits :: reset( char s )
36

if ( isalpha(s ) )

Bits :: reset( tolower(s ) - 'a' );
}
int AlphaBits :: is set( chars )
(                =
if ( isalpha(s ) )
return Bits :: is set( tolower( 5 ) - 'a' );
else
return 0;
}
int main()
{

AlphaBits letters;
char buffer(512];

for Cys)

{
cout << "\nPlease type a word (0 to quit): ";
cin >> buffer;

// 비트 설정
for ( char *s = buffer; *s; 5+7+ )
letters.set( *s );

// B48 출력
cout << "The letters used were: ";
for ( char c = 'a'; c <= 'z"; ctt )
if ( letters.is set(c) )
cout << ¢ << Wt:
cout << "\n';

// 28 42> 함
letters.clear();
}
return 0;
}

4

#include <iostream.h>

unsigned int add( unsigned int lhs, unsigned int rhs )
a6
unsigned int result, carry;

while (1 )

{
result = Lhs * rhs;
carry = lhs & rhs;
if ( carry ==0 )


===== PAGE 839 =====
838 ee 부록
break;
Lhs = carry << 1;
rhs = result;
3;

return result;

int main()
{
unsigned Long a, b;
for Ces)
nf
cout << "Enter two numbers. (0 to stop): ";
cin >> a->> b;

if (la && !b)
break;
cout <<a << "+" << b << "=" << add(a,b) << endl;
가
return 0;



===== PAGE 840 =====
CD-ROM AIL |



===== PAGE 841 =====
840 co 부록

이 책에 포함된 CD-ROMAE 다음과 같이 C++ 프로그래밍을 배우는 a 필요한
프로그램과 원시 코드가 들어 있습니다.
HB Borland International 사의 상응 801070 C++ 컴파일러 - 006, 윈도우용

BY 단원을 공부하기 전, 후에 시행해 볼 수 있는 평가 시험 - 이를 통해 해당 Cee 복

7
습할 필요가 있는지 알 수 있습니다.
를 교재에 있는 원시 코드의 파일들 - 입력하는데 소요되는 시간을 절약해 줍니다

CD-ROMS 사응하기 위해 필요한 시스템 사양
컴파일러를 사용하는데 다음과 같은 사항이 필요합니다.
HH Intel 80386/SX 혹은 그 이상의 IBM PC 호환 기종으로 80486 이상을 추천함
mm MBS} 확장 메모리를 가진 DOS 3.31 이상 버전

를 윈도우 프로그래밍을 위해 버전 3.0 이상의 Microsoft Windows2} 2MB 이상의 확장 메모
리가 필요함[4\/8 추천]

BVGA 이상의 해상도
HH CDROM 드라이버
충분한 하드 더스크 용량
를 마우스나 유사한 기구
평가 시험을 보기 위해 다음이 필요합니다.
W IBM PC 호환 기종으로 1386 이상|1486을 추천함|
HI Microsoft DOS 5.0 이상
Hl Microsoft Windows 3.x 이상
 4MB RAM(SMBS 추천함
BH 256 color 디스플레| HE
를 2배속 CDROM ©2t°]H(CDROM2 = 수행시)



===== PAGE 842 =====
부록 ㄷ CD-ROM 사용법 ee 841

CD-ROM 사응하기

윈도우 3.1 메뉴 프로그램에서
1. CD-ROMS CD-ROM 드라이버에 삽입
2 파일 혹은 프로그램 관리자로부터 파일 메뉴의 실행을 선택
3. (driver)\setup.exeS 입력하고 <ㄷ0[6[>를 누릅니다. 여기서 <driver)=  여러분의
CD-ROMS| 드라이버를 가리키는 문자입니다. 예를 들어, 여러분의 CD-ROMO] 0: 드
라이버라면 D:\setup.exeS 입력하고 (Enter)S 누릅니다. 여기부터 Interactivest
메뉴 프로그램이 열립니다. 단지 안내 메뉴를 따라 온라인 화면 명령을 따라 가십시오.

윈도우 95 메뉴 프로그램에서
1. CD-ROMS CD-ROM 드라이버에 삽입
2% 윈도우 95 데스크탑에서 내 컴퓨터 항목을 더블클릭
3. CD-ROM 아이콘을 더블클릭
4 인스톨 프로그램을 수행하기 위해 SETUP.EXE 아이콘을 더블클릭. 여기부터
Interactivest 메뉴 프로그램이 열립니다. 단지 안내 메뉴를 따라 온라인 화면 명령을
따라 가십시오.

윈도우 Ht 인스톨되어 있는 컴퓨터에 AutoPlay 기능이 설정되어 있으면 cp-Rom 드라이버
에 디스크를 넣자마자 7S 2S SETUP.EXEt 수행됩니다.

Borland C++ 3.1 인스

Borland C++ 3.1에는 자동으로 INSTALL 프로그램이 따라옵니다. 파일 압축 기법
이 사용되었으며, 파일을 인스톨하기 위해서는 이 프로그램을 사용합니다. 단순히
파일들을 여러분의 하드 디스크로 BAS FE 없습니다. INSTALLS] 자동으로
복사해 주고 압축된 파일을 복원합니다. 참고로 인스톨 디스크의 README 파일
에 공급되는 파일 목록이 있습니다.

Borland 사의 라이선스와 제한된 사용 권한에 관한 동의서가 있는데 알아두실 필
요가 있습니다. 이 부록 뒷부분에 있는 동의서 HRS 읽어보십시오.



===== PAGE 843 =====
842 ee 부록

Borland International 사와 직접 연락하여 기술 자문을 구하지 마십시오, 기술 자문을 위해
서는 이 책 뒷부분에 있는 Macmillan 기술 지원부 ASS 참조하십시오.

DOS 3.31 이상에서 인스톨하기
DOS 3.31 이상 AoA] Borland 0++을 인스톨하려면 다음 단계를 취하십시오.

1. CD-ROM CD-ROM 드라이버에 삽입

2. d:\bce31\install& 입력(여러분의 CD-ROM 드라이버가 0:가 아니면 해당 드라이버

입력)

3. 화면에 나타나는 BAS 따라감
인스톨이 끝나면 800800 C++ 파일들을 가진 경로가 만들어집니다.
c:\borlandc\bin 또는 이에 해당되는 BES 여러분의 AUTOEXECBAT 파일의 시
스템 AZo] 집어넣어야 합니다. 이래야 6008000가 컴파일러를 가진 경로로 인식
됩니다. 만일 여러분이 이 컴파일러를 다른 경로나 다른 드라이버에 넣었다면 이

에 UES 조정하십시오. 정보가 더 필요하시면 eco] 시스템 안내서를 참조하십
시오.

윈도우 3.× 이상에서 인스톨하기
윈도우 3x 이상 버전에서 Borland C++-S 인스톨하려면 다음 GAS

sy
Of
ON
rial
ey
bo

1. CD-ROMS CD-ROM 드라이버에 삽입
2. 프로그램 관리자에서 파일 | 실행 선택
3. 0:\6631\406181을 입력(00-ㅁ014 드라이버가 0:가 아니면 해당 드라이버 입력)
4. OKS 선택

$. 화면에 나타나는 명령을 따라간다.

So] 끝나면 80000 (++이라는 프로그램 그룹을 만드는데 이 안에 모든 관

스놀                                  =
된 도구들과 안내 파일들을 가진 아이콘이 생성됩니다.

fe eo

윈도우 95 이상에서 인스톨하기
윈도우 95 이상 버전에서 Borland 0++을 인스톨하려면 다음 단계를 취하십시오.
1. CD-ROMS CD-ROM 드라이버에 삽입

2. 시작 메뉴에서 시행 선택



===== PAGE 844 =====
부록 E CD-ROM 사용법 ee 843

3- d:\be31\install @A(CD-ROM 드라이버가 d:7} 아니면 해당 드라이버 입력)

4 OKS 선택

§. 화면에 나타나는 HAS 따라감
인스톨이 EUW Borland (++이라는 프로그램 그룹을 만드는데 이 안에 모든 관
련된 도구들과 안내 파일들을 가진 아이콘이 생성됩니다.

Borland C++ 수행하기

1005에서 Borland (++을 인스톨한 뒤, Borland C++2] bin 경로로 바꾸십시오.
를 입력하고 <Enter>S 누르십시오. 이렇게 하면 통합 개발 BAdntegrated

Development Environment)°] 열립니다.

윈도우 3.15} 95에서는 Borland C++ 3.1 그룹에서 Borland C++-2 선택하십시오.

혹은 Borland (++의 bin 경로에서 bew.exeS 선택하기 위해 파일 관리자를 사용할

수 있습니다.

윈도우 95 이상 버전에서는 시작 메뉴에서 프로그램 | Borland C++ 3.1 | Borland

C++ 선택합니다. 혹은 Borland C++ \bin 경로에서 60\.6%6를 선택하기 위해 윈

도우 탐색기를 사용할 수 있습니다.

Borland C++ 3.1슬 가지고 프로그램 컴파일하기
각 통합 개발 환경은 메뉴 안에서 컴파일 옵션을 제공합니다. 추가로 여러분은
DOS 명령어에서 컴파일할 수도 있습니다. 컴파일하려면 다음을 입력하십시오.
bec <파일명>
여기서 <파일명>은 여러분의 컴파일하려는 파일의 이름입니다.
여러분이 Bad command or filename 오류 메시지를 받았다면 40708%80.847에서
PATH 부분을 검사하여 0\0008000\00(여러분이 컴파일러를 이 경로에 인스톨하였
다는 가정 하에) 경로가 있는지 확인해야 합니다.

평가 시험 부분

평가 시험 부분은 각 단원에 대한 여러분의 지식을 검사하는 프로그램들입니다.
은 3개의 구조로 이루어져 있습니다.



===== PAGE 845 =====
844 ee

40
dil

자체 평가 부분 : 보통 이 부분이 먼저 치러집니다. 이 평가는 특정 주제에서
여러분이 어느 부분이 강하고 약한지에 대한 감을 주기 위해 꾸며졌습니다.
답안을 통해 즉시 Bolo] 가능합니다. 맞았으면 다음 문제로 가십시오. 틀렸으
교재 중에서 어느 단원을 더 공부해야 할지 가르쳐 주며, 다시 시도할 기
드립니다.

단원 마무리 시험 : 각 GAS 읽은 후 해당 단원의 내용 중에서 간단한 테스
트를 할 수 있는 기회를 드립니다. 즉시 해답을 통해 확인할 수 있습니다.
마스터 시험 : 이 부분이 중요합니다. 여기에 여러분이 모든 것을 알았다는
을 증명하기 위한 여러 개의 자체 평가 시험 문제가 있습니다.

Sou (모
때

ya

{4

어

모든 시험 문제는 사지선다형입니다. 각 답은 a 8, 6 dz 되어 있습니다. 다른 말
이 없으면 답은 한 개입니다.

자체 시험 소프트웨어 인스톨
윈도우 탐색기의 CDROM] 직접 소프트웨어를 실행할 수 있으며 5600 프로그
램을 수행해도 됩니다. 소프트웨어는 18라는 경로에 있습니다.

자체 시험 시작
자체 시험 소프트웨어는 CDROMAA] 직접 수행이 가능하므로 여러분의 하드 디
스크에 어떤 파일도 인스톨할 필요가 없습니다. 여러분은 그저 간단한 시작 과정
만 따라가다 보면 소프트웨어가 매우 쉽다는 것을 알게 됩니다.
윈도우 3.1과 95 이하 버전에서는 다음 단계를 따르십시오.
1, 프로그램 관리자의 파일 메뉴에서 실행을 선택
2 d:\CTB 입력(여러분의 CD-ROM 드라이버가 0:가 아니면 해당 드라이버 입력)
4. OKS 선택
$ㆍ 화면에 나타나는 BAS 따라감
윈도우 95 이상에서는 다음 GAS 따르십시오.
시작 메뉴에서 실행을 선택
ㆍ d:\CTB 입력(여러분의 CD-ROM 드라이버가 0:가 아니면 해당 드라이버 입력)
4. OKS 선택
§. 화면에 나타나는 BAS 따라감



===== PAGE 846 =====
부록 E CD-ROM 사용법 ee 845

CD-ROM 문제는 무작위로 문제들을 ASL 새로운 문제 그룹을 선택하려면 중간에 종
료하고 다시 시작해야 합니다. 시작 메뉴에서 다시 시작하면 새로운 문제들이 다시 나타남

eet

Macmillan Computer Publishing, USA 라이선스 동의서

이 패키지의 CD-ROMS 이 부록 Eo] 기술된 소프트웨어를 포함합니다. 이 패키
지를 SOU 여러분은 다음과 같은 사항에 동의하는 것이 됩니다.

이 소프트웨어는 판권 소유가 있으며 모든 권한은 출핀 판사 및 라이선스를 맺은 당
사자에게 귀속되어 있습니다. 여러분은 이 소프트웨어를 단일 컴퓨터에서 사용할
수 있는 권한을 갖습니다. 이 소프트웨어는 단지 백업용으로 복사가 가능합니다.
다른 목적으로 이 소프트웨어를 복사하는 것은 다음과 같은 미국 법률을 어기는
것이 됩니다.

THIS SOFTWARE IS SOLD AS IS, WITHOUT WARRANTY OF ANY KIND, EITHER

EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.

출판사나 라이선스 계약자, 공급자 및 판매자는 이 소프트웨어를 사용하다 발생
된 손해에 대해 책임이 없습니다.

이 디스크의 모든 내용 및 소프트웨어의 컴파일 본은 판권 소유가 되어 있으며
미국 법률에 의해 보호를 받습니다. 이 디스크의 각 프로그램은 저자와 소유자에
의해 판권 소유가 되어 있습니다. 각 소프트웨어는 사용 허가를 받아야 하며 제
한을 받습니다. 각 프로그램을 사용하려면 사용 허가를 받고 요구 사항에 따라야
합니다. 라이선스에 동의하지 않으시면 프로그램을 사용하지 마시기 바랍니다.

BORLAND 제품에 대한 사응 동의서 및 한정 보중

중요 - 주의 깊게 읽으세요.
이 사용 동의서/한정 보증문은 위 서술된(80814040에 의해 제공된 소프트웨어,
미디어 및 이에 수반되는 온라인 혹은 출력된 안내서) 소프트웨어 산출물(소
웨어)에 대한 여러분(개인 혹은

i 2

단체 구매자)과 이 소프트웨어를 여러분께 제



===== PAGE 847 =====
846 ee 부록

출판사 및 Borland Intemational, 00간의, 법적 합의문(라이선스합의)으로 이루어집
니다.

BY INSTALLING, COPYING, OR OTHERWISE USING THE SOFTWARE, YOU AGREE
TO BE BOUND BY ALL OF THE TERMS AND CONDITIONS OF THE LICENSE
AGREEMENT.

여러분이 이 소프트웨어의 원래 구입자이며 이 사용 동의서의 각 구절과 조건에
동의하지 않으면 이 소프트웨어를 구입한 곳에서 즉시 반품하시기 바랍니다.

이 사용 동의서의 각 구절과 조건에 동의하시면, 800800는 이 소프트웨어를 교육
적 목적에 의해서만 아래에 기술된 방식으로 사용할 권한을 드리며, 이 소프트웨
어에 의해 제작된 SBE] 대한 권한을 인정하지 않습니다.

이 소프트웨어는 800800 및 그 공급자에 의해 판권 소유법 및 국제 판권법에 ：
해 겨레 pret 따라서 여러분은 이 소프트웨어를 다른 판권 소유 인정된 물

(예를       , 책)과 같이 취급하여야 합니다. 단 백업 목적으로만 이 소프트 alos
ee 이 소프트웨어를 하드 디스크로 SANA 수 있습니다.

여러분이 백업 이외의 다른 목적으로 BABS 가지지 않는다면 여러분은 소프트
웨어와 HAS 영구히 가질 수 있습니다. 단, 사용 동의서에 서술한 대로 버러
임대, 대여, 복사, 수정, 2차 라이선스, 전자 우편에 의한 소프트웨어의 송
금지됩니다. 여러분은 소프트웨어의 소스 코드 형태로 800800 및 그 우아

권한을 인정하므로 동의 없이 소프트웨어를 수정하거나 디컴파일, 디어셈블
것이 금지됩니다.

이 소프트웨어는 미 통상국 FAS 준수하며, 800000가 깐매한 국가에서 사용할
목적으로 만들어졌습니다.

완 오 > Ae

rr : ii rlo

사용이 위험한 경우

이 소프트웨어는 오류에 대한 충분한 검중이 이루어지지 Beton, 위험한 환경 -
예를 들어 핵실험, 항공, 통신 시스템, 항공 제어, 의료 시스템, 국방 시스템 -
만일 오류시 즉각적인 사상, WA, 중요한 물리적, Waa eds 입히는 환경 하
에서 사용되도록 고안되지는 않았습니다.

wae

이 in 합의문은 Borland] 공식 권한을 가진 부서와 당사자간의 사인이 이
Jo] 의해서만 수정 가능합니다. 이 문건의 일부가 무효 또는 준수될

은



===== PAGE 848 =====
부록 E CD-ROM 사용법 ee 847

수 없다고 해도 나머지 부분은 유효하며 준수될 수 있습니다. 만일 일부분이 초
기 목적에 부합하지 않는다 해도 나머지는 유효합니다.

이 라이선스 합의문은 USA California 주의 법에 의해 만들어지고 해석됩니다.
이 합의문은 여러분에게 특정 법률적 권한을 부여합니다. 이 조항들은 주, 국가간

변동이 가능합니다.

기술 지원

여러분의 컴퓨터 및 0.9, 제 3의 응용 프로그램에서의 문제점은 도와드릴 수 없
습니다. 이 책이나 00#080에서의 문제점은 도와드립니다. 860000에 문제가 발
생하면 Macmillan Technical Supporto] 연락하십시오.

Borland International 사와 직접 연락하여 기술 자문을 구하지 마십시오.

Internet E-mail

문제 발생시 Macmillan Technical Support 전화 (317) 581 - 3833 혹은 E-mail
support@mep.com®]] 의뢰하십시오.

여러분이 Compuserve, America Online, Prodigy 가입자인 경우 그 서비스를 통해
E-mail°] 가능합니다.

우편
Macmillan Computer Publishing
Support Department

201 West 103rd Street
Indianapolis, IN 46290

전화
(317) 581-3833
(800) 858-7674

DHA
ae

(317) 817-7488



===== PAGE 849 =====
848 ee 부록

온라인 접

http://www.mcp.com

Borland C++2 예외 ZH, RMS 지원하지 않습니다.

가



===== PAGE 850 =====
찾아보기 ee 849

#define 593
#else 594
#undef 597

ADT 442

ANSI 표준 30

ASCII 문자 집합 59
Abstract Data Type 438
Access 746

Array 334

Array Element 335
argc(argument count) 584
argument 50
argv(argument vector) 584
arity 321

assert() 606

assignment operator 81
atoi() 732

Bag 372

Binary Operator 320
Bit Twiddling 736
Bit field 738
Breakpoint 717
break 187

buffer flush 549

찾아보기

Casting Down 417
Code Rot 692
Complement 연산자 737
Concatenation 604
Conditional Compilation 599
Conditional Operator 102
Constant 69
Constructor 160
Containment 500
Conversion Operator 327
Copy Constructor 301
catch B= 693, 698
cerr 552

char 배열 353

character 57

cin 552, 553
cin.ignore() 565

clog 552

close.) 577
compile-time binding 400
const 71

const Reference 280
const this 포인터 251
const 멤버 함수 164
const 포인터 248

continue 187

conversion specifier 574
cout 44, 552, 567



===== PAGE 851 =====
850 ee 찾아보기

cout.width() 570
ctimeQ) 731

Dangling Pointer 246
Declaring 109

Default Parameter 125
Defining the Function 112
Definition 109

Delegation 513

Derivation 376

Destructor 160
Development Environment 31
Dictionary 371

Doubled linked 365

deep copy 301
dereference 228

derive 377

direct recursion 133
do...while  191

dynamic binding 400

Expression 79
element 334
else 92

Flag 570

Flipping Bits 738
Formatting Instruction 570
Free Store 234

Friend Class 526

Friend Function 536
Function Prototype 109
Function polymorphism 128

fillQ 571

for 196

fstream 클래스 552
function 108

Global Variable 116
get) 559

getline) 563

goto 182

IDE 592
Implemented in terms of 513
Inclusion Guard 595
Indentation Style 92
Indenting 742
Instantiation 657
Invariants() 609

if 89

indirect recursion 133
indirection 228
inheritance 376
inline 131

106 클래스 552
ios::app 579

ios::ate 579
ios::binary 581
ios::nocreate 579
ios::noreplace 579

ios::trunc 579



===== PAGE 852 =====
찾아보기 ee 851

iostream 라이브러리 548
isa 376

istream 552

1080 732

Looping 182
literal constant 70
logical AND 99
logical NOT 100
logical OR 99

Macro Function 599
Manipulator 570
Memory Leak 238
Mix-in 클래스 438
Mixin 438

Multiple Inheritance 420
masking 연산자 737
member-wise copy 301

Nesting Parentheses 87
Node 364
new 235

Operator 81
Ordered Collection 371

Overload 292
Overloading Function 128

Overriding Function 390
ofstream 576
operator>> 558
ostream 552

overriding method 390

Percolating Upward 417
Piping 553

Predefined Macro 605
Prefix Operator 308
Private Inheritance 522
Pure Virtual Function 442
parameter 50

peek) 566
polymorphism 396
popped 139

printf) 574

problem space 626
protected 380

pushed 139

putback() 566

RAM 56

Recursion 133
Redirection 553
Relational Precedence 100
Return Value 123
reference 256

run-time binding 400



===== PAGE 853 =====
Set 371

Set Flag 572

Side Effect 608
Signed 58

Singly linked 365
Sparse array 372
Standard Library 724
Statement 78

Static Member Data 456
Static Member Function 462
Stray Pointer 246
Stream 548

String Class 357
Structure 176

Style 742

shallow copy 301
signature 390
solution space 626
state 572

static binding 400
stdlib 732

streat() 729

strepy() 355, 725
streambuf 클래스 552
strncat() 729
strncpy() 355, 725
subscript 334
switch 205
8\1001문 정렬 743

symbolic constant 70

Tail 364
Ternary Operator 102

Tree 365
this 244

try 블록 693, 698
typedef 64

Unary Operator 316
Unsigned 58

Virtual Copy Constructor 405

_ Virtual Destructor 405

Virtual Inheritance 433
Virtual Method 396
y-table 401

virtual function table 401

Watch Point 718
Whitespace 78
while 184

가상 메쏘드 396
가상 복사 생성자 405
가상 상속 433

가상 소멸자 405
가상 함수 테이블 401
간접 지정 228

간접 지정 연산자 228



===== PAGE 854 =====
찾아보기 ee 853

간접 호출 133
}소 연산자 84
개발 주기 33
개발 환경 31
객체 지향 프로그래밍 26
객체 초기화 300
경계점 718
공백 문자 78, 79
관계 연산자 88
계 연산자 우선순위 100
점에서 구현 513
동 프로그램 644
구조적 프로그래밍 26
구조체 176
규격 명령어 570
기본 매개 변수 125
im  상수 70
긴 줄의 처리 743
은 복사 301

oN

at

문민

기 뿌뿌

낙타식 표기 61
내장 매크로 605
널 문장 78

널 참조자 262

널 포인터 227

누드 364

다중 상속 420
다차원 배열 344

대소문자의 구별 61
대입 연산자 81, 322
동적 바인딩 400
들여쓰기 92, 742
디버그 수준 616

seis ce un cninathesa's’ova iy sa whv eben eaENURUNTEAVa¥is9 (2)
라이브러리 548

레지스터 138

BA 33

초기 0a COS BBOOE LR eee SPECS ER ScneR (oO)
매개 변수

매개 시이 템플릿 657
매크로 함수 599
메모리 누출 238
메모리 번지 56
메모리 할당 57
메쏘드 148
메쏘드 은폐 393
메쏘드의 재생 390
멤버 변수 147
멤버 함수 148
멤버 함수 중첩 292
임체 372

호성 때 427

jak

Ad   ie   td

xX

Ad Ad 5 An Ad

od,
~
2



===== PAGE 855 =====
854 ㅎㅎ 찾아보기

문제 영역 626
문체 742

반환값 123

배열 334

배열 원소 335

배열 초기화 340

배열의 원소 334
배타적 비트 OR 연산자 737
버퍼 방출 549

버퍼화 549

범용 151

범용 접근자 메쏘드 154
범위 연산자(::) 477
베이스 클래스 377
변수 56

변수 선언 341

변환 상술자 _574
보수 연산자 737
Holy 155

보호 자료 멤버 380
복사 생성자 272, 301
복합ㅠ 94

부작용 608

분기점 717

배열 372
바꾸기 738
설정 737

연산 736
연산자 AND 736
E 연산자 OR 737
비트 초기화 738
비트 필드 738

프프프프프리
m im im im jm re

사건 구동 방식 27
사전 371

삼항 연산자 102
삽입 연산자 540, 567
상속 376

상속성 29

상수 69

상수 나열령 71

상수형 참조자 280
상승 417

상태 572

생성자 160
생성자 중첩 298
설정 플래그 572
소멸자 160

수식문 79

수학 연산자 81
순수 가상 함수 442
순종 AS 635
순차적 프로그래밍 2
순환문 182

스택 138, 139
스택 포인터 140
스트림 548

실행 바인덩 400
쌍방향 연결 365



===== PAGE 856 =====
찾아보기 ee 855

연산자 중첩 305, 316, 320
예약어 61

오른쪽 값 81

올림 초기화 65
와일드 포인터 227
왼쪽 값 81
운영체제 138

워드프로세서 31
원시 파일 32

원형부 390
이스케이프 문자 69
이진 파일 581
이항 연산자 320
인수 50
인스턴스화 657
인터페이스 165
입력 재지정(<) 553

자기 호출 133
자료 멤버 147
자료 은닉 28

자유 기억 공간 234
자유 기억 장소 138
잡종 계층 635
재사용성 29

재지정 553

전역 공간 138
전역 변수 116

전용 상속 522

전용성 155

전처리계 43, 592
전치 연산자 84, 308
접근 746

정렬 모임체 371

정적 멤버 자료 456
정적 멤버 함수 462, 464
정적 바인딩 400
조건 연산자 102

조건부 컴파일 599
조종자 570

조회 연산자 228
주석 745

주석문 46

주소 연산자(@&) 225
중괄호 정렬 742
중첩 괄호 87

SA 생성자 298
중첩된 순환문 201
증가 연산자 84
증가 함수 307

지역 변수 114

직접 호출 133

집합 371

이게개지게 (%)
참조자 256

첨자 334

추상 자료형 438

주상화 단계 137

추출 연산자 558

출력 문자 69

출력 재지정(>) 553

dtl aaea vance ore ye Manion Ue aner ences (4)
es} 28

컴파일 32

컴파일 바인딩 400
AE YS 138
클라이언트 147



===== PAGE 857 =====
856 eo 찾아보기

EAL 256
테일 364
텍스트 문자열 43
텍스트 파일 581
텍스트 편집기 31

트리 365

파생 376, 377

파이프 553

포인터 224

포인터 배열 347

포함 500

포함 감시자 595
라이브러리 724

= 함수 536, 540
그램 25
플래그 570
플랜드 클래스 536
한

함수 다형성 128
함수 선언 109
함수 실행 113
함수 원형 109, 112
함수 인자 120
함수 재생 390
함수 정의 109, 112
함수 중첩 128
함수 포인터 468
항의 개수 321
해결 영역 626

0 【오 off

:형가리식 표기법 61

헤더 364
형 변환 연산자 327
형 변환 하향 417

확장 함수 131
후치 연산자 84
힙 234



===== PAGE 858 =====
/

/

a WY 지향 설계, 프로그래밍,
분석을 배움니다.
프로그램 작성 및 소스 고드의
컴파일, 실행 파일을 강력하고
빠르게민들 수 있습니다.

a 새로운 ANS| 표준과
프로그램에서 ANSI 표준의
의미를 알게 합니다.

BA, 비열, 변수, 포인터를

통애 고닌도의 프로그래망을

가능히게 합니다
여러분 프로그램의 Yas
상속성과 디형성을 통해

확장시키는 HE 일게 됩니다.
프로그램 SANE 통에
CHO 특징을 완전히

fae

소화하기 BIEL,
 모든 ANSI 표준 G+ Bulg

러로 동작할 수 있습니다.

호

Category : Programming
Covers : C++

SAMS

PUBLISHING

이 책은 객체 지향 프로그램의 설계 및 SMS 가르쳐줍니다. 프로그램 내부의

책                       및 분
흐름 및 메모리 관리, 컴파일, 디버깅을 포함한 SE 기본 개념을 이해시켜 드립
니다. 한 걸음 더 나아가 이 MS 21일간 자습할 수 있도록 하였습니다. 각 개념 '
들을 이해하기 쉬운 주제들로 분류하여 나누었으며, 각 리스트 코드를 통해 실력 |
을 배양하도록 하였습니다. 리스트 AEE 충분히 보완되고 수정되었으며 ANSI |
표준에 맞도록 컴파일하여 시험되었습니다.

|

|

= Liberty Associates, 100.의 회장인데 여기메서는 그는 객체 지|

프로그래밍에 대한 사이트를 통해 교육 및 모니터링, 컨설팅, 프로그래밍 사업!
하고 있습니다. Jesse AT&T, Xerox, PBS 사에서 걸출한 소프트웨어 aut
지니어 및 설계자로 이름을 날렸으며, 한때 시티 은행 개발부 부사장이었습니다.
그는 프로그래밍 및 객체 지향 분석, 설계에 관해 6권의 AS 썼으며, 그의 웹 Ap!
이트는 0ㅁ://\00.11061/25600165.000입니다.        :          :              :

|

010 ook

g t=

1!!!

ISBN 89-7627-465-2

정보문회시

~ http://www. infopub.co.kr

