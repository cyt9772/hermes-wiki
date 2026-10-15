---
source_url: /home/yutae/work/pdf/20261015/프로그래밍/비주얼베이직6_입문.pdf
ingested: 2026-10-15
sha256: 3d19ecc0293b55e3d64410c971d9b3fee3bfb41b564fa9e32f1bc2a8072858c4
---
# NEW 비주얼베이직 6 입문 (raw source)


> **Warning:** scan-only PDF. OCR'd via tesseract 5.5.3 (kor+eng, 300dpi); some English tokens garbled — cross-check the original PDF when interpreting. 원서는 일본어 원서(Hayashi Haruhiko, SoftBank)의 한국어 번역(Youngjin.com, 1999/2002).
## Book metadata
- **title:** NEW 비주얼 베이직 6입문 — 프로그래밍 업어 마스터 시리즈 (New Visual Basic Nyumon Beginner Hen)
- **author:** HARUHIKO HAYASHI (하야시 하루히코)
- **original:** SoftBank Publishing (JP), 1998
- **publisher (KR):** 영진닷컴 (Youngjin.com, 영진출판사), 1999 first edition, 2002 reissue
- **ISBN:** 89-314-1287-8
- **pages:** 357 (scanned)
- **source file:** raw/books/vb6-introduction.pdf (local only, git-ignored)
## 장 (chapter) structure
| # | topic | rough book pages |
|---|-------|------|
| 1 | Visual Basic 의 기본 지식을 알아보자 (클래스와 인스턴스) | ~20-57 |
| 2 | 어떻게 Visual Basic 프로그램을 만들 것인가? | ~58-86 |
| 3 | Visual Basic 6의 기본 조작 (IDE, 컴파일과 디버그, 프로젝트 관리) | ~87-154 |
| 4 | 변수 (기본 데이터형, 배열, Variant, 사용자 정의형) | ~155-162 |
| 5 | 연산자 | ~163-170 |
| 6 | 제어문 (If, Select Case, For, While, Do, GOTO) | ~171-182 |
| 7 | 프로시저 작성 (Sub/함수, 파라미터) | ~183-194 |
| 8 | 컨트롤의 사용 | ~195-249 |
| 9 | (API 등) | ~250-280 |
| 10 | 그래픽의 처리 | ~302-320 |
| 11 | 재미있는 프로그램 | ~321-333 |
| 12 | 파일 처리 함수 (순차/랜덤 액세스) | ~334-357 |
## OCR text (all 357 pages)


===== PAGE 1 =====
NEW
비주얼베이직

0) 르
[= |

뜨

2Stl.com GHETIED [eaux

영진출판사가 '영진닷컴'으로 새롭게 출발합니다. TEL.(02)794-9000 FAX.(02)794-4200   aoe


===== PAGE 2 =====
프로그래밍 업어 마스터 시리즈 New 비주얼 베이지 6

SHIN VISUAL BASIC NYUMON BEGINNER HEN

by HARUHIKO HAYASHI

Copyright © 1998 by HARUHIKO HAYASHI

Original Japanese edition published by SOFTBANK PUBLISHING, INC.,
Tokyo

Korean translation rights arranged with SOFTBANK PUBLISHING,
INC. through Eric Yang Agency

Korean Translation Copyright © 1999 by YOUNGJIN.COM

Copyright ©2002 by Youngjin.com

1623-10 Seocho-dong Seocho-gu
Seoul, 137-878

Korea
All rights reserved. First edition Printed 1999. Printed in Korea
ISBN 89-314-1287-8

이 AS 무단복사, 복제, 전재하는 AS 저작권법에 저촉됩니다.

* Microsoft Microsoft Corp.2] 등록상표입니다.

*\1000\8는 Microsoft 0072.의 등록

상표입니다.

* Visual Basic: Microsoft Crop.2] 등록상표입니다.

이외의 상표는 각 회사의 등록상표입니다.

저 자 : HARUHIKO HAYASHI
기 획 : 영진기획팀
1 9: Wa, 깐동명

’



===== PAGE 3 =====
fa
모

m@ 들어가기 앞서서

윈도우 시대가 되자 컴퓨터의 기능이 비약적으로 발전했다. 특히 윈도우 95
의 등장 이래 컴퓨터의 기능은 상상을 초월할 정도로 많아졌다. 단지 마우스를
클럭하는 것에 그치지 않고 더블 클릭, 드래그, 오른쪽 클릭 등 또 그 조작의 위
A, 조작 형태의 차이까지 혼란스러울 정도로 조작 방법이 다양해졌다. 또 화면
상에도 변화가 있어 아이콘과 도구 모음, 버튼, 여러 가지 다이얼로그 박스와
Indicator, status bar 등으로 화면이 F 차게 되었다. 이와 같이 복잡한 조작
을 가능하게 하기 위해서는 그것을 실현할 고도의 기능을 갖고 있는 윈도우용
프로그래밍 언어가 필요하다. 마이크로소프트 Visual Basic® 그 대표적인 언

어이다,

지금까지의 MS-DOS$ 프로그램 언어는 본질적으로 어떤 대상을 처리하는
기능만을 갖고 있었다. 가능한 프로그램에 대한 조작 표시는 키보드에서만 할 뿐
이었다. 이에 비해 Visual 88810은 다음의 2가지 기능으로 구성된다.

3
무엇

랜

처리할까(계산)+어떻게 ZALA[ZI7KIntertace)

1;

어떻게 조작시킬까 라는 기능이 소위 윈도우다운 애플리케이션을 실
. LAS 하기 위해서 Visual 88810은 여러 가지 부품을 갖고 있다. 그
면 버튼과 AES 표시하기 위한 박스이다. 이 같은 부품을 모아
sual 28810의 프로그램이다. 또 그 부품이 제 기능을 다하게 하기
 이벤트 드리븐 방식이라는 프로그래밍 방법을 취한다.

ea
람 애

네요 (건

:

그
들
Vi

  nu {ru

fe}

39 of rat

원  버  rlo

이처럼 Visual Basic2 S42] MS-DOSS 언어와는 크게 다르다. 이 기능
은 AAS 포함한 내용은 아니다. 그 때문에 Visual 88810의 초보자에게 설명
하는 경우가 많다. 윈도우 조작은 표면적인 지식만으로 끝나지만 Visual
Basic? 프로그래밍 언어이다. 따라서 Visual Basics 공부해 나가는 것은 표
면적으로는 끝나지 않으므로 깊숙이 이해해야 한다.


===== PAGE 4 =====
이지를 넘게 되어 초심자용이라고 말하기가 어렵기 때문에 이 책은 다음과 같은
방침으로 설명한다.

금부터 Visual Basic 배우고 있는 초심자에게 필요한 지식을 정리해 제
시하고 실제 샘플 프로그램을 보여 준다. 초심자에게 필요한 항목을
체계적으로 보여 졸 것이다.

이 책은 Visual Basic 6.0에 대해서 그 기능과 용법을 설명한다. Visual
Basic V 6,02 마이크로소프트사의 Visual Basic, Visual C++, Visual J++
을 총합한 34 Visual Studio 6.0으로 버전업과 동시에 개정된 것이다 종래의
Visual Basic 버전 5.0에 대해 여러 가지 기능이 추가되었지만 사용자가 보는
개발 환경 부분에 대해서는 거의 차이가 없다. 즉 개발 환경면에서 화면 레이아
웃과 컨트롤의 취급, 코드의 입력 방법 등이 같다. 실제 사용의 차이에 대해 보고
적절한 설명과 샘플 프로그램의 추가 등으로 보다 처리하기 쉽도록 서술했다.

이 책과 Visual BasicS 학습하고 싶은 독자가 하나가 될 때, 좋은 성과를 a
{다.

°

2. 스
=e i

>


===== PAGE 5 =====
 Visual 80510의 기본 지식을 알아보자 ……… 15

1.1 Visual Basic2] 특징 SSE ns EST GAs aa SaaS RT I encale cri cearenneiarmeernpnnanennor 16
epee Bee fs -………여~~너서여셔셔며애적6애져래/허90학야지버에지지자여 17
THANE seevesteneneonnesenessunoacvennasnaevsant pies seneeanneuaennaesenes ina tevestusrenentirenentarenseaereuasueueventents 17
다 -!스[이므로 어0000000000000000000000000000000000000000070000000000000000000000000000070000000000000000000077 18
SAI OBE 애서.오오오 이 시은오오오온오온은우 으오으오스 18
alee ee 19
이벤트와 이벤트 프로시저 ㆍ…아아아아아아아사아애서어어사어이어이이이비사이이기시아시기사이이시이사새사애새사애아어 20
최초로 실행되는 프로시저 ㆍ……아아아아아아서아아아애어아새아져사어어이이이기새아사어이기사새사새사애사애사자사사어 20
프로시저와 BY ……아아아아아아아아아아아아아셔새사사시시비새사사사사이새사이이이새사어어이이이새아이이세새새새새새아어 21
클래스와 인스턴스란 ceeeeecereeeeeeeeeeseteeetesseeeeeeeeesesseeeereseeeeseseesesteeestneeeeeneeeserteeernes 22
Bl EOS OOOO OOOOOOOEOOOOOOOOOOOOOOOSS 23
컨트롤이란 eS 23
BA SEE SESOSOOSESOOOESOOOS OOOO OOEOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO 24
개체의 관계| nessereresceeeeeesessseeeeeseesteeesnsctssesessentessennasesesnnenesnereseneengeassonensersacasssnenenenes 24
Visual 88916에서 프로그램을 작성하는 순서 ㆍ………아아아아아아바아아바아아아아바아아아아아아바아아아아아 24
1.3 코드 작성에 SERGE OY ectsgczeacerwevarsseozaveuns as saurenasconan onepeaertiaennatctimns nave taanaesnnagn 으으으 으오오오 으으으 은 26
주석 seeereteeeeeeseeseesetseteetseesetsstsssesessessessessessesssteseesesesssssessesseresteeneeteeteetestestentensees 26
복수 명령문 cas cecsesseeseesssesesesevesseessescseesscsssenenevsssvsssssensnssavassenenenenssseseneseneeserenenenenengs 26
문장을 복수 행으로 분할 oeeeeesecsescseeeeessssseneeecsesesssssesesessssssseenenessssssesenenesssseasecaenees 26
진수의 ey 9S SSESE SESS CESOES CSO OSSOOOOOOOEOSEOSOOOEOSOOOOOOOOSOOROOOOOOS 27
대문자와 소문자의 구별 cee e cece eee eee ete e eee e tees tees eeeeeetee testes sieettretteeenteeesteesnereneees 27
으는니뿔시느0000000000000000000000008600009 28
1.4 학습 방법 Amicon ant aw seep mE TEEPE omTe ne sierernce esr 29

2.1 직접 프로그램을 만들어 보자 ………-……………ㄴ여리 32
2.2 Visual Basic 실행하기 See Oe cence etorcnsinarneaieemeectecr cenit are eee 32
D3 Ol] 제목 불이기| ecteeeeseeenccrencctescascenesesormnnaveorennsacornranazescrsnersonnanvernveasessiessavtssce saan nesvausntbaaiasotaen 35

24 컨트롤 배치하기 Smee fa 1 이해키지케기00벼애여겨여티며배재기캐자 con See Tz ME eREE THESES CARTS EES 36


===== PAGE 6 =====
CONTENTS

285 이벤트 SEU A A CRF | oxeesccerecerrereree reer rte eaoeo nee eT 39
2.6 프로크램의 ABW creer ences ecrcant emenimimaimantiataee oe 41
ag, be a an een atone neat 42
2.8 새로운 프로그램 작성하기 ……………………………………………………………………………… 45
2.9 저장된 파일 블러무기 rcccesesscrssnsenvesnaroerccinnessen cin anaes 47
2.10 실재 TEC exer) FEET] cece eeecsseseessessneessssnneessssnncessnnneccesnnnsecesnnnneecsnnnaeseannneecnnnnaeeestey 49
yee Ds en 51

2.12 실행 파일의 실행

3.1 Visual Basic2| 시작 66668 veaaien ESO RERSEUSENRSSARE CONOR EASA S AUR EIT RURT THANE SEE
3.2 Visual Basic2| 화면 구성 회분 오규개태겨재떼에역져데회에배해더 개셔려래야애매아재예개기퇴거아에여어기기기이이의
3.3 Visual 88510의 화면 레이아웃
3.4 메뉴 바와 도그 모음  A EASES Nh TST WA tsa ian antg eR eranehad Geneeeonsaetnenes 63
도구 모음 EEE OESOEOSEOSEOOOEOSEO OSS OSEOSSSOOSOOSEOOE OOOO OOOOSOOOSEOOOOOOSOOOOOOOOOOOOON 76
3.5 애플리케이션의 조작 순서  irra here EERT NRK ORONO SEOURET 79
컨트를 배치하기 en 79
자이 컬블00000000000000000000000000000000000000000000000000000000002 79
활성화하기 cvvceesseeeeeeeseeseeeeeeeeeteeteeeseesssessseseeseesseesssesessesessessseseseessseeessesesesssesesseesnes 79
컨트롤 이동과 크기 변경 cvreceesceeseeseessesscesseeseeesesseesssesesesessesssessesseeseesseeseesseeseeesenseenes 81
컨트롤 제거하기 EEE EEE 81
BSAA  eeceueeenteaenems cere rernerze seer wettiaeeacenectisiseeeecemoremeer prememncgarettaceae 81
개 제의 YAY wevseessesercsessessssesessssescsoscsssececscscsensosnencsesncncnsnensassesersencacnensnssenensnenessssenens 82
속성의 항목 설정 …‥………아아아아 82
FE TAT 00000 84
코드 입력 화면 eeeeeeeeeeeeeeeseeeestsesteeessseeeseeeseesesseesseseseessesessecssessseeeeseaesseessseeesseenseeenes 84
개체와 이벤트를 선택한다 ㆍ……9999999999990090000600404090040909606006960090064000000004 85
이벤트 프로시저명과 코드 QYEY  eeeeeseeeseeseesseeeesseeseesseeseeesessesssesseeseesseessesseenesenrenseeaeens 85
프로시저 코드의 연속 표시와 분해 표시 ……이99990 87
지모부부재피으으으 재이재이으으섹이이 노이 2 이 이이 89


===== PAGE 7 =====
CONTENTS

neo. 구성원 자동 Es mi i nu Wana awa’ N Ta NTN a WR aN Ula hSDN a STEERS 91
작은 창에서의 능숙한 선택 방법 BO CC ence CO ter ae Cone oe cece eee ice ero C cre 92
PORE FEA)  <asreusten tyres e vee eau eaneneennst ems manraenien ine masiaco kamen sts 93
패가 변수 점보의 Sp eres ected ras eeratecarae eer e ec ayettarne aeacoqarsenarsevoraneas esses 93
단어를 잃어버렸을 패의 .지원 SEA) -v-eoeewensssteescnzennns erssorsneettnaeiennentnainaavecstuwcasecs 95
주서 블록 기능: cee 태이 95
3.6 애플리케이션의 실행과 디버그 eee ccc eesssssssssssssssssssssssssssssssseecssssecsssececceeeeeeceeeeeees 97
OURS AO| SS] APM ienesccdecscrracrsrarnernacareerreniivers ene nner et EREA He 97
순차 컴파일과 완전 컴파일 …-…………-ㅠ이시이 98
터비 그융의 화면 2: en ee eee ee 99
be A ee ee ee 101
아00 문으로 정지하기 ……………………~                            이이 ate ee 102
중단점을 설정하라
디버그용 윈도우의 여러 가지 종류       elon           104
Co Ea a 105
직접 실행 창의 구성 ……ㄴ아아        107
간략한 조사석의 ASR …-…ㄴ…-ㄴ……ㄴ~~아여여        107
Deboug. Print 추신 108
EATS AYRE nnseeeeeeeee nese nsesssseseeeettecennssssennentneectnntnnnnsseenngnnnnntssuunnenseeneneennssannnsecennnnenenesaey 109
DG Cis, eee 110
임의의 행까지 실행. cocceecestersceremvcanessercanscciseessseesenannanapstsawavencsenemnennnenemee 111
커서 위치를 실행 이전으로 되돌리기 ………………………………………%%%%%%%%%%%……………… 111
Ce? [보기 | 여새여벼자셔체비녀저제여쳐지석연벼녀치티져터재제타 111
AIBA TEED] AG AISI sacsccscnacqnnncanccvecnnnnnanancentnrnaneestnpnngnralsnncnm sewicersetVaneninysese cen coosicencuenenosys 113
3.7 프로젝트와 환경 관리 ……………………………………………………………………………………… 116
때 로젝트의 SE eneresserreenemtenc nace e ioraniesmniaeenarenmene 116
프로젝트 작성/불러오기/저장 ……ㄴ니이 121
WSIS 추가/제거/보존 ………ㄴ…-…ㅋ…ㅋㄴ~…~려새아여시 121

BBO] 신규 작성 ……~~처겨여래                                                                                             “sees 122


===== PAGE 8 =====
CONTENTS

사용자 정의 컨트롤 도구 상자에 추가/삭제 cscs eeccee estes eeeseeeetteeeeennteesensenrseeseesensey 122
Visual 88616의 환경 옵션 설정 eect tts eee teeter secrete teesiteeeeeerieeenerrneenaerneasacensenenanysays 123
BBA re) 9) 127
3.8 a MO) my we 128
텍스트의 삭제와 이동 그리고 == 0 MEE 130
드래그에 의한 = AS =i) = 131
[빈인인언인의인이처 트에에세0/070.29.70.700006 131
문자열의 검색과 바꾸기  ………아아아아아바바아사아아아아아아아아아어애새새사사아아시이새새사이이새새새사사사아아아 131
코드 에디터의 a 도움말 …….아아아아아아아아아아아아아아아아아새자사지이시이새새사서사사사사버어서서서서서서사아 132
폼과 코드의 인쇄 …………아아아아아아마바아바사사사바바바바바바바아사사사바타타바바바바아아사사자자자아바아바아아아아 133
3.9 도움말의 사용 ……………나어어아에아아새새가새사사새아가서아지아이999사사사사아사사아사사아사 135
Chapter 4       변수
4.1 an Da Ac
묵시적 선
형 선언 문자
명시적인
명시적인
변수 이름
변수의 통
4.2 배열의 A cee

4.3 동적 배열 기능

4.4 기본 데이터형

4.5 문자열형(61090)  가 이이 151

4.6 통화형(64『『60ㅇ\) ee ee 152

4,7 HtO|Ea(Byte)

4.8 H2s(Boolean) sa seep ae ace se eee on gE ccnp em EAT aT den en Th Sea crenia eee A 153

PE eB) | ee ce ee ee Meee 153

QUE Ce) ———— 으으으 으으 으으 9 154
I) OG cxcenmescntonsr sirstxmnsnenelianmannhstase ie ens be AE 154
응할에 의한 주소 설정 ……아사아아바바사아바사아바바바사아사사사아바사아아마아아이이어이이아어아아어새아사어에 154

개체형의 반대 설정 sssseesesesescescessessees sean ssuseussuseisenssnenisesansenvoneecssasesacanneteensanesiersennes 155


===== PAGE 9 =====
CONTENTS

Nothing2| 설정과 개체 설정 ‥……아아아아아아아아아아아이이에이이어이9이119이사이이시9이시아이시이 155
NewOl] 의한 새로운 모듈의 생성 ceeceseeeseseeeeeetssessesseseeessesseeseesseseessesseesesssasseasserness 155
4. 11 FEBS Variant) vce sinner nmmmamninasneesnmmemrmmcema ements 157
가변형 선언과 값의 대입 --seeeeseceesseeesesseeseeseseesstseesssesseeesssssesssseesseseseesesseasesssseeeeenees 157
0 이으르그는 리00008 158
Empty2t=} lsEmpty 함수 ee EEESOOEEESEOSS 158
NUIZEDH ISNUI] eseeceeereeeceeeeereeeeeeneneeeeenenssensneeentenettesseneoeaesetdastesntenrssensnnnentateneseees 159
4112 사용자 정의형(구조체) rerun crenrecsencensipsiceomctseerntcnstoninimenennemomeersbanstn 159
4.13 Crist 정수(기호 정수) …………………~아거아가개사새90000 160

Chapter  5         연산자  (inert tot ee ter eer oi eon _    163

Chapter 6     세 이분] ee eee 171
6.1 Visual Basic®| 제어문 sccictenansemnn tanner naneemamnnn 172
UF ee acca crerceesent ere erat ase eens nessreeccrarce eect gee eonesooe esters erent ceptor 172
63) Select Case 물 = 에에 em ere snereenireesssereroeeim enor ri om munnessteesots 173
6 4 FOr Se eerste teens aad anon anes 175
G5 WHS: ccc WN eee anasecece rel ceces rarenrctarencncrevencirata cope reers ogee to uassuansesiczeeceenenecas 176

6.6 Do...Loop=


===== PAGE 10 =====
CONTENTS

6.7 GOTO SET 라벨 …………………………………………에아에에에에에에아아에아아메에아마메에아메아아메에에아메아마메에아메에에아에에아아아 178
6.8 Stop 문
6.9 Exit 2
6.10 End =

6. 1] WEA Reece ree een actenccen rarer rte rensuiran aurea Tessa Toerteegeravai lvoe eevey earsr a Te aemeeeeceeedt 180
6.12 그 외의 제어문(ㅎ1|, Go Sub, On) arr pelea a pave gue ean nee esta eh aya oneeatendior ss 181
Chapter 7     프로시저 작성  =ㅋㅁㅋ88 0818.54.19.88.0.0116188.1880888.8.88.8.881880.0581610.60416180누0881 183
7.1 Visual Basic2| 프로시저 여기 아대 두 이 이브 으으 해이 비이 SE 184
7.2 Sub 프로시저 Insctitevloeansusenamnanpasaeseivenessinwin wt amassblin sin 으으으 vat bile Rera ye eee Race U aN CNA ELIA Taaeaaes 184
Sub 프로시저 정의 weecseeccesssseesseeeseeesseceseeesnsesssesssssesseeseersaeesnnesssesseeesseeeasecnsessaeeees 184

오바 TEAL] BeB  ctteeettcccecnseeseresseeenscessenssneesneeneenecneanmsestentsetsesseassanesevanasenenecesces 185

HEOTASOL ANOS. senniccnnndncsnnnnnen enenonsnnnanivesiintssisvse tansuniner veawna nes Sus eblbies sc eenanaaneuuguageeagiE 186

7.3 함수 프로시저 EVA Sai Ae eco A aha s AT Ad costo c nt pm ee amet earannmennieeemeneeeattoneanannsewescasuneans 186
함수 프로시저의 정의 crveeecseeereeerseesseseseceneensescessetsssessseessesentesseesssesseressesenaseeseeesees 186

함수. 프로시져 호출 ㅣ …이시이이이이이이00610 0 187

7.4 프로시저의 신규 작성과 삭제 Dae ard Bae Ch eocrerc pacicacr a eho gC Une on one 대이 eee Sea CEL 188
이벤트 :프로시저와 제너럴 프로세서 nvcrenreerenerenenneneroneneemennavstauanamnnmvscaveneiansineniieseey 188

새로운 제너럴 프로시저를 작성 ㆍ………아아99999아이아아애이 188

기존의 프로시저 편집 에디터 불러우|  ceeeeeeeeeeseeeeeteseeceseeseseseseenenseeneaeseneeneneneeenenenes 189

불필요한" 프로 시[저의 ALA] seetesnstcevncrcovenrsannnnnnnmeenesenantanensstcananaseedishecaenanwveveneiiveviiaens 189

7.5 인수를 넘겨 주는 방법 showers Dunes St TOE oe ape Mal age Aen ca ek Pan aeevmecucaveanemederneneesnee 190
참조에 의한 호출 sseeeesscesecsseesiesesessssoessessneesereseeracseserceesseccecesnceesseensepensseneansseenensen 190

값에 의한 SE cesdstsenroendenncnesssseansenneennrrnnnsntnansennrsdanesenves se nevonasicuubusniovieetwnsruweteteNs 191

식에 의한 Sp 범겨주기 a ancannnanvvncansnsnasnaumenvesnseerteamnees seis sent eene que anu RNR ENENER 192

사용자 정의형 넘겨주기 ee ec re 193

비열 념겨주기. sestaeeerenteeneaaeseraescessneencresnnnesrseernannnnnnemennnsspvansabhstectiias saceasnlsoet.veldveaiaarons 194
Chapter 8     컨트롤의 사용 a 195
8.1 기본 컨트롤 보기 SEEDED Yer cto onc Saco oR RE a eR PERS RR ELIOT eee CPE Le Stee 196
8.2 (Form) sin sive enacts tracer icv ara ee aE en gp RUIOU TAAL ETHRHLGUGB Uc neaneranenesese 198

10)


===== PAGE 11 =====
CONTENTS

Ce ee 으으으 에우 202
설명 610668912614361662044내이0너누46.이시스161서러지티가가어치지9하느조사리지져기여다져자태1채시제차 203
8.5 라벨(Ｌ3661) ee een 206
규정 아아아 inne ne oie 이벤베베베베베 바이 사서 으2 206
a 207
8.6 텍스트 박스(16×<[6ㅁ0×) cracenee cheer ceeetenecteaes senes ann certtercncbv voce ster teal enszer Meavvaeocerrstecetcecestes 209
ee이아 209
설명 digibloaia yan Vso e' ph WIEN U.A pS lei aaininl pte dinc ob NAN Dae HAiMalNG alba wis o's sais eles ulcsiei auc ae uaa nen eG spas esenekaspaesevaseinseens 210
8.7 0|0|X\(Image) Se ee 아아아 아아 213
아다 000000000000000000000000000700000020000007077 213
PJD] sessesrsnssenssevenrecsnsvasnsnssensnstonensvenadasienadeesserssai aU Ne SNRSAEAAA Races svasatnenneeceass 214
8.8 픽처 4tA(PictureBox) ad RS apie bvt ay wetiigu iPcoyp ld raguceb casilocscu rear zaypans edn eevy ESET TANTS ERISSTECIIES 218
TEAL veeceetttteeeeetteeeeesseeeessseeseesseseessneesessseccesssessenesssesseseeeeeseeecsseeeensraeeeesnaeeeesaeeees 218
SAY scsi AC i nh tiadeomeinetannsas 219
8.9 프레임(『『「3106) iA le 으으으 이오아이어온 으으 아이이 이오 이 223
보지 새시 00090 000 223
설명 Upp hn da enkan Caeet peaeets seuss aekteleu seme mienaopaeane pia bamatnisencamaienGeh yak caaes-taeanh ee -mie~eaeene-msierscsenen 224
8.10 체크 HA(CHECKBOX) n-ne tnntnnttninninninninnniiuniiansensieis 225
ae 225
설명 Seis lRtale Rie alee es Sie ese ig ac op ye enerehen naman cin ate cmhasbpnapnnhatesninsh<demteniersneninecseeemrseeenenarese 226
8.11 옵션 RECO Bitty) ence ncn ssecentzcsesvssnraonnsvnsnnanennnasasnznvnreoeserevnnnbsosennensntin 229
a 229
설명 Seana Ris SS See Sis eae wy ou mieten 애가 me ramadan ad aunt e tae GAaeaRnw son cale nen enpaacemeneativamse 230
S12 리스트 BA(LIstBOx) cccerstcacrs nce nner naniamaninnne cinemas 232
이이다 이아다다000000000000000000000000000070 232
ID ex ceceonane sce tinsesecnacstznenaneengenonopenns songnenmonnnananensnensamicsnesnenenyensiessaat 233
8.13 콤보 4tA(ComboBox) sieuseseeveneNsSTis TERT ae CEREURLEIIN ASRS UTRONNTET TREE TERESI SENT REIRUR TRUE aRERNEES 238
이 ee 238
aD nasa eer sm iii Sco ere 239

11


===== PAGE 12 =====
CONTENTS

규정 rte e eee ee errr rrr eeeeerereetnrneeeeeeeetnnnieeteeeeersennenneeeeeenes 242
RAD cenvereseneryaseis suns rseeorg nce ean uasneps a reer era 243
8.15 수직 스크롤 바(\/6아이182[) Ge ee ee ee 246
TEAL ctetteetetnseeenttseesneteeeeetteseeeseeestseecesensesenessetsesseeseeseeeerseaeessiateeenieteeneateeseaeeeenes 246
PACS nronancarntanonanonsabh venvsssiensitiweanswanencnsueoverciuandvis vvresins gon vounseeeee nee ene a nEyEae ENR 246
8.16 타이머(] 16) << eeorecw re ereeecrmmenmemr ee 247
FEA rete etter et ee eee terrasse treeeetrteeseriseeeseneeestnseeesineeeeeniteereneeeenieeeeete 247
STS pesto rc ors crc ge ocr ate an 이 | 247
8.1/ 드라이브 :리쓰트 밤쓰 이에 00이0이아에에에이이이으매에데에매이에이이 1. 249
규정 EEE 249
PAT ee ee 0000 이이. 250
8.18 디렉토리 리스트 BA(DirListBox) seems nacmenneemmanmnnnmience 251
가점: seers es sth cms cnmm eevee cava es Sette caren tas sncncr mm oemenmomnaney 251
SE ee ac dis eee OS oc eee a Pcl a ee 252
8.19 파일 리스트 BA(FIISLISTBOX) esses ccmssenrmuvanaraesnssecescseeceeeam 253
는 으드애0550000000000000000000000000000000000000000000000020000070 253
2ST oe rip PE CT cet le a OE 254
8.20 제이프(81966)  onveervsseesssserssssesseessessssesessssesssessnsessnsanesusnecnaseruaneqssseesennecnnunnqeneevanses 257
TER rete teeter teeta 0000000000000000000000000000000000000000000000000000000 257
AQTE scar scaracdeninarcen esnsnesigansqnaiigaatets tonenenata sii piiease wri wsir cau aoseviree Stan acinteorcas ames 257
8.21 라인(106) ……………………………녀니이이이이이이이이이이이이이이미에이에예에에에에이 259
be 0S eee 259
설명 nisineinein einen a casting Women wiapin-tnin ale seisia winiainneanginin win aiKn an 0(sTeb Ae ane We We HS AD NST Naa aaa Nats We Nele eNO T UNAS UNS 259
CVO ㄷ컨테이너(()|Ｌ Se ee 261
baie S eee 261
PEE sasmearonanetns anranahgedsgesnatzmnanesiea ¥en anus la ea ary otenitc nandvedv ome anne rR aS 262
8.23 데이터[0313) Sao agp Ceasar oe naron ey pea ReHRE RpSaeE aLE LRG ac coenaceereneosn menaeeearvannpgamneereanecane 270
STOEL eeesay asuicseshn Seats ceceraer Sues Gene ta See ec ace-n conaee ceoaoee en enntasarneranenee omnes Pera eee 270
HA 2 xen sscalverst ansaetnanasrenardinnstoesrannsthashenvoxestoiinctniuitivasus . Puta ostinsucnecer waiocenarneanys 271
8.24 메뉴(\4/6114)  Sasa NN ex eU RIS eee eae enmnnn ARNE SER IR IOTTAOONEEH 리이매 272
is Se 212
BADE ancinactaneasvonnsasaamranntnanevtennsryn ceneraii 1scdSioR 니니 273


===== PAGE 13 =====
CONTENTS

  그 의 기본 용법 …아아에에에아에에애에메아에에아아아 279

9.1 MSQGBOxOl] 의한 정보 표시 …………………거거거거거거개가가사가가가게가가사서사사사사사에사사사새사사아새애아아아아: 280

9.2 InputBoxOl 의한 입력 ee 283

913 품 크기와 컨트를 크기의 be er 286

9.4 Printer 개체 Se eee, ee | a 291

916 마우스, 이벤트와 키| 이벤트 secretion nrescnainemrimensidnicninnceummsivermtinibareincaeet 296

이 어서섭서000000000000000000000000000000006 296

비이어언서0000000000000000어9999600000 296

DragDrop ash Saba slnea nana sol awrarNioarlaNnicastarlekiounie NWA RAINS KK ROD HiSAieSCONAGlsiOnamtmAaeneineiemeiae mmeAle 297

DragOver Galea Rye Na aiden BGI ie Manas HAE SER EUR Sala apo NUNES NNR oUNsnaCOMaUaRTI REA MUNNTNKINND ONAN 297

KeyDown /KeyUp     Hin Pan AEA Hn EDN RIG Apna sie dld eR SESH KS ENA SCHORR UNA RIT OIE STEGER  297

KeyPress FS CT Gece oat tigi abn pre SESE nase 7 GC EM ePIC OPHIR oe ct DOr Lacon Orme oar ieeranry oe ME 299

MOoUSEDOWN/MOUSCUD  ……0아아아사아사바사사사바바사아아자아이이아이이이이아이아사사아사사새사아새사새사사사 300

터00861\06 어어아아애서아아애아아어어이이애아비이이이시사이기사시비사시사시사이새이사시이어애아사새새사사새사사아새사 300

Chapter 10     그래픽의 저리 ee 305

ORE, 와 단위 ee ee ete. 306

10.2 SCreer 개체 cnn csesccccesssseessceessseessesesnsssnnnesssensssanssssssssssnsssesensssnssnsssesssnsssnesssscesssnneseseeeenen 307

10.3 AHO] 지정 ee Ee er Oe eee er 308

Long 정수 지정 EE 308

이업블크는0000000000000000으어00909900000006 308

0@0800아 k=! ES 309

짜넣기 정수 …아아아아아아아아서사서새사사사시이새사아이사새새새사이이사사새사이이새새새사사사이사새사사이세새서새사새아자 309

10.4 그래픽컬 컨트롤 …………………………여49040 310

10.5 크래픽처리에 유용한 ANIA cesccceccomnnnmstanssenneepmunanerercavaernncsianiinemines 311
10.6 컨트롤의 이동

Left/Top 속성의 9 0 = Sa 312

1646 8s |e 312

PACH [SE savcvecssectescnernnenncsnnssnsesneensgoncennennsossnsnsnsbanssensanssensonisoeessensersbedesssstnenisennsss 312

10-7 픽처 바꾸기 배아 61611 인빙니11281※18116164126(8161.81664616바1614비16114 312

10 8 크래픽 메서트 ac ner csceynrnsnvcasnasonsnerconnterenernanenennenmaeseosae bhi eth ata 316


===== PAGE 14 =====
CONTENTS

11.3 트리 are ee ws wr Was SE rca er 오이어히치으으아여디져애제매며태매미며제게매지에 327
11.4 평행선의 회전 Sie ea EERIE AR TAGs i Seen err ere remeron ereatareoowemecs 329
11.5 구의 표시 오브 Rocca Gogg han unc i ROC ts RTE dE RCEN RET ec ma LENCE OS Hae Ce 이이소은 으으 331
11.6 입체 문자 표시 00 으으으 으으으으으 으으이으으 Wale als YEW Ea URN eae Eu Stet CEU OGRA ROLE RUSTE NSO os 336
12.1 파일 액세스에 대해서 …………………………………………………………………………… 340
12.2 파일 액세스의 종류 span eae na aly vee Ue Otc SEY TIE en gee onsen pene alenexyrayFEmareaatnasnenns 341
12.3 파일 처리용 함수와 명령문 ……………………………………………………………ㅇ…ㅇ…………. 341
12.4 순차 액세스 …………………………………………………………ㅇ…ㅇ……………………………………………………… 343
파월 열기 ㅣ ~여아나이어이여이서지16106 dees uuneceeeconecnnesseenepennnensnnenene 343

파일 ELD] eaesecineenmtaeaesnvcea ee eiicacrean tacanra new nenoeinanrsananatiorvat-onanienenenasnncaseueucanisassieneseanineas 343

데이터 '읽그  serereeenenscnenacensensonemmsieswsaeauitan anemvananancaneversssvaenmneae del svedsiana Seen ayreTay IE 344

파일 es esenevnsavwscnesecscasasuseaewscensevainn sunteneusentey suena sd bteepesueetaectaseeeeteneresereresesesnenenees 345

12.5 랜덤 액세스 ………………………………………………………………………………………………………. 347
레 코드 정의  ………애여사 347

파일 SYD] wxeewecsetecesessussesesosedeserseesensnsayens veg evaeedaaseaueavareedaseccstsonrcronnneensaneeenseseetenen® 347

레코드 읽기 area 0a ces eminem netnee beni ein en et ecnraasnnscdincli sro mesisnnnined dik Helan eaTaalnee 348

레 고트 BAG) cererenorcnexseonar se. nn-sccyas cite or ratan an searassseateeyesueshcnueetemeereaernaen 348

레 큐드 BET}. srcesesecoeserccsseossccscessovssntosevewedeedseneneasavavvandaeessetevesssheossastesesoreceenensennes 348

CYR 싸지. sesveeeerecenstes seemecepsen cose ensearteccgsencrencatennecadernatetaccenerernnane ce sermecernonseaces 349

12.6 바이너리 액세스 …………………………………………………………………………………………………………………… 351
바이너리 QI <evwessenseseseesscencovevesnatvntnveosunvenenanenetnasnnasesieiveeneeaaanteseeearsaseoncnenesennene 352

OYE) SIF]  serssececezsessacetcencetasaiwie stincenmerencnenesieoraceenenetnan caneeenansiinnceaaeusienniceensaaisona 352

바이너리 액세스의 내용 처리 a er Te er eo eer 352

내부 EY esereescasneerener sve raneenneneueneeneemrass exeneeaeeaas mean naenniomeiasasdavareatecreeneranscesenenetae 353

일 | NOE] a: memes sence cccatertnstite se at ener oesnnsne sence arenas dernon nner doundisia sath sateen nase aio 354

인덱스  isa le WW Wid ald 6d WSU al NNER GR WAGG Inve S'S Slne Sin mnie a eins neaieinainieiels.asia:ns Rosiswniauewnais nnsaanedewveue’ead 356


===== PAGE 15 =====
CHAPTER

Visual Basic 의
기본 AAS 알아보자

이 장에서는 우선, Visual BasicO| 갖고 있는 다양한
지식에 대해서 알아보기로 하고 정리된 자세한 설명은 다음 장부터 살펴
보기로 하겠다. 이 장에서는 또 이후의 ABS 위해서 필요한 7
용어와 기본적인 지식에 대해서 명확히 기술한다.



===== PAGE 16 =====
Chapter1 Visual Basic 의 기본 지식을 알아보자

Visual Basic 은 종래의 148-1008 Quick Basic 과는 완전히 다른 프로그램 언어이다.
언어라고 말하기보다는 프로그램 개발 환경이라는 것이 적절하며 형태는 다음과 같이 구성되

어 있다.

| 프로그래밍 언어 ㅣ
+
도우 사용자 인터페이스 개발 툴 |

110

또한 작성된 애플리케이션은 다음과 같이 구성된다.

| 개 체 | + | 이벤트프로시저 ㅣ

2

Visual Basic 2 종전의48-1008시대의) 베이직이라는 개념을 초월하여 대단ㅎ
의 프로그램 개발 환경이 되고 있다. Visual Basic 2] 특징은 다음과 같다.

@ 『010이라는 토대가 되는 창에 버튼과 텍스트 박스 등의 HESS 배치하여 화면을 만든다.
@ 479] 컨트롤에 대응한 이벤트 프로시저에 실제 처리 USS 기술한다.

@ 각 컨트롤에 속성을 설정함으로써 세밀한 제어가 가능하다.

@ 각 컨트롤은 메서드라는 BAS 통하여 동작시킨다.

@ 외부 애플리케이션과 데이터를 주고받는 기능이 준비되어 있다.

@ 외부 데이터베이스와의 관련 처리를 행하는 기능이 준비되어 있다.

@ 다양한 디버그 기능을 갖는다.

로
이
Sz
Js
IN
16
Obi
Ei
we
Hu
AY
프
ull
bs
>으
aia

@ 그 외에 윈도우에서 운용하기 위한 유용한



===== PAGE 17 =====
1.2 프로그램 구조에 대하여

Visual 88810 은 이벤트 프로시저 SS 직접 만든다는 AS 제외하면 마치 HSS 쌓아 올
el 것처럼 AA Odjec)S 이용하여 프로그램을 작성한다. 이 장에서는 프로그램 구조에 관
한 중요한 항목에 대해서 설명한다.

-DOS | 상에서 za 사용하는 mage 화면에서 HES 표시하고 이것을
인가 작동된다. 이러한 처리를 하고 싶은 경우에는 다음과 같은 작업을 필요로

>오

(2) HES 그래픽으로 표시하는 프로그램 작성

(6) 버튼에 OSS 붙이거나 AS 입히는 프로그램 작성
(0) 버튼이 눌러졌는지를 검출하는 프로

(0) 버튼 클릭에 따른 작동 프로그램 작
(                          작송

6) 마우스 작동 및 체크 프로그램

rl

rim

이와 같이 여러 가지 데이터(이름과 색)와 프로그램 AES 작성해야 한다.

개체는 이 프로그램과 데이터를 조합 하나의 단위로서 이용할 수 있도록 한 것이다. 예를
들면 명령 버튼이라는 개체를 지정하면 명령 버튼과 프로그램이 전부 준비된다.

개체라는 말의 사용 범위는 광범위하다. 예를 들면 애플리케이션 전체가 하나의 개체이고
그 안에 있는 Form & 개체이다. 또 Form 상에 배치되어 있는 명령 버튼 등도 각각 개체이
다. 개체는 다른 개체를 포함할 수도 있다.

예를 들면 나사와 못은 단순한 것이다. 그것을 사용하여 무엇을 할지는 목공(프로그래머)이
결정한다. 나사와 못이 목공을 대신해 줄 수는 없는 법이다.

이것에 대해 TV 개체이다. 그 안에는 사물이 있고 그 사물을 동작시키기 위한 기능을 내장
하고 있다. TV 전원과 채널과 음량이라는 속성을 지정하면 그것만으로도 움직인다.

개체는 프로그램을 작성하는 부품이다.
NOTE

17


===== PAGE 18 =====
_콜렉션이란

Visual Basic 에서 사용되고 있는 여러 가지 기체 중에서 같
다. 예를 SH Forms 콜렉션은 애플리케이션에서 방향을 제 시하고
한 것이다. 또 Printers SAAS 시스템에서 사용할 수
프린터 개체는 평상시 사용되는 하나의
0 있는 콜렉션은

다. 이것에 비해
Visual Basic 에

Chapter1 Visual Basic2| 기본 지식을 알아보자

고
32   i
je
cS
mm
0
tho
so
m=)
rol:

Ju
있는 모
프린

대응하는 개체에 자를 붙이기로 되어 있으므로

Forms

Form
Control                             Controls
Printer                             Printers

종류의 개체의 모임이다.

속성이란

Make 그 활용 범위를 넓히기 위해서 속

이름 색

성을 자세히 4

면 개체의 예로서 TVS 생각하면 그 속성은 다음과 같다.

18

표시 HA

속성을 가지고 있다. 속성이 없으면 그 개체는 특
작업에서만 사용할 수 있다. 속성은 개체의 적용 범위를 넓혀 주는 것이다. 예를 들면 명령 버
Eo 다음과 같은 많은 속성

성 항목을 가지고

벌정하는 것으로 자신의 요구에 맞춰서 화면과 활동을 결정할 수 있다. 예를 들


===== PAGE 19 =====
1.2 프로그램 구조에 대하여

전 원      on “ㆍ 전원을 Zc}

채 님       1 vee HS 1로 한다

a5       5 owe 음량을 적당히
색채               속성       속성값

속성의 값은 화면 레이아웃을 할 때 속성 창에서 설정할 수 있지만 프로그램 코드 안에서도
다음과 같이 설정할 수 있다.

Wile] AAS ARS 것은 속성이다. 속성 창은 그    Sg Was B28 + 있다.
그러나 이와는 별도로 개체를 조작해야 할 필요가 YS 경우 그 역할을 하는 것이 매서드

개체를
(Method)o|¢}, 예를 들면 개체의 이동은 중요한 메서드이다.
메서드의 예로

매서드

개체

위의 내용을 구체적으로 설명하면 Forml lH: FS (100,200)9} 위치로 이동시키라는
지시는 다음과 같다.

Form1, Move 100,200

iil 매서드는 어떠한 SAS 하는 것이다.
NOTE

19


===== PAGE 20 =====
Chapter1 Visual Basic2| 기본 지식을 알아보자

_이벤트와 이벤트 프로시저 _       —
Visual Basic 4] 2-190] 확인 가능한 외부의 동작을 이번트라고

ot
=
요
ru
rule
re

마우스 클릭
마우스 드래그

키보드 입력

이 대표적인 이벤트이다. 또 타이머로 발생하는 이벤트도 있다. Visual 88816 은 개체마다 이
벤트가 발생하면 이에 대응하는 프로그램으로 점프하는 장치를 가지고 있다. 그 대응하는 프
로그램을 이벤트 프로시저라고 하며 이벤트 프로시저는 정의 부분이 준비되어 있어서 내용(프

로그램 코드)만 사용자가 작성한다.
예를 들면 명령 버튼을 클릭하였을 경우 이벤트 프로시저는 다음처럼 된다.
이 프로그램 코드는

-버튼이 눌러지면 무엇을 할까

2
를 결

전

성힌

(고

ee

다

Private Sub Commandl_Click() ‘H#0| 클릭되었을 때 실행되는 이벤트 프로시저

(HES 클릭할 때에 동작하는 SAIS 사용자가 직접 작성)

~

End Sub                   이벤트 프로시저의 B

기 이벤트는 무언가가 일어났는지를 검출하는 것이다.
NOTE

 최초로 실행되는 프로시저

이벤트 프로시저는 애플리케이션이 실행되고 있을 때 사용자의 조작에 ola  실행된다. 그러면
최초로 실행되는 프로시저는 어떤 것일까. Visual 88800 애플리케이션을 실행하면 우선 SS 읽

어 들이지만 최초 동작으로 다음 프로시저를 실행한다.

Private Sub Form_Load()
(사용자가 적성)

End Sub

20


===== PAGE 21 =====
1.2 프로그램 구조에 대하여

이 프로시저는 여러 가지 속성의 초기 설정과 폼들을 메모리에 올리고, 사용하는 변수의 초
기 ABS 한다. Form 11080 는 최초에 실행되는 프로시저이다.

프로시저와 명령문          0"

프로시저는 프로그램 코드 집합으로 실행할 때에는: 한 개의 단위로 치리된다 종래의 베이
직에서는 서브루턴이나 함수라는 이름이 사용되어 왔지만 16481 88810은 프로시저라는 이
름으로 사용된다. Visual 88810의 프로시저는 다음과 같다.

6 AIA   Joos US 되돌리지 않는다(서브루틴)
일반적 프로시저 ]ㆍㆍㆍ애플리케이션 전체에 공통되는 코드 작성

이벤트 프로시저 |ㆍㆍ 이벤트 발생시 실행되는 코드 작성

이 프로시저 작성에는 명령문이 사용된다. 프로시저는 사용자 자신이 작성한 코드의 집합

이다, 171 대해 SBE AAS Beate 최소의 Geld, BEM 여러 가지 조작

과 선언, 정의 등을 기술한 최소 단위의 구문이 명령문이며 Visual Basic ol] 처음부터 준비되
는 기능이다. 다음과 같은 것이 명령문의 예이다.

A=100

Dim B

If A=100 Then X=200
Print A

ott
Ad
‘lo
rh
ooh
2,
Ol
ae
SE
|=
다
pons

이 기본이지만 아래와 같이 복수로 쓰기도 한다. 이러한

A = 100 : PRINTA

21


===== PAGE 22 =====
22

Chapter 1

| 클래스와 인스턴스란

Visual Basic 의 기본 지식을 알아보자

Visual Basic S 저음 시작하는 ARS      몰라도 크게 상관은
래스 및 인스턴스라는 중요한 기능이 있다. 클래스는 개체의 기능
예를 보면 도구 상자 위에 HAS] 있는 그림은 클래스를 표현하고 있다.
예를 들면

는 [명령 버튼:이라는 클래스를 표현하고 있다. 이 클래스를
채로 드래그하면 버튼 그림이 나타난다. 이 복사된 버튼 그림
서 실제로 복사하여 배치한 버튼이 개체가 된다.

클래스는 처음에 누군가가 프로그래밍한 소스 프로그램을 같이 사용할 목적으로 공개한 것
이라고 생각된다. 예를 들어 말하면 클래스는 설계도와 같은 것으로 살아 있는 것은 아니다.
클래스의 인스턴스를 작성하면 그것이 개체라는 살아 있는 AS 실제로 동작을 하는 것이 되
는 것이다. 복사된 것이므로 당연히 그 개체는 근원이 되는 클래스 YAS 이어받고 있다. 또
클래스를 모은 클래스 라이브러리는 판매 대상이 되지만 개체 라이브러리는 판매되지 않는다

인스턴스(복사) 작성
SSSR ESSE S SRS

0|21< Visual BasicOll            이것을 AASAUA Visual Basiclh &
준비되어 있다(스스로 만드는 AS 가              프로그래빙한다

Olr



===== PAGE 23 =====
1.2 프로그램 구조에 대하여

만일 여러분이 혼자서 팩스의 양식을 작성한다고 가정하자. ‘HAS 포함해서 00장 보냄
니다" 라는 문장을 HES 작성하고 점선을 굿는다. 이 원본 양식은 보통 바인더 파일에 보존
해 둔다. 그리고 팩스를 보낼 필요가 있을 때가 클래스에 해당한다. 그리고 복사(인스턴스),
실제로 사용하는 팩스 양식은 개체가 된다.

개  클래스 [원본 코드]에서 인스턴스는 원본 코드를 복사한 것이다.

Visual Basic}] 프로그램을 작성할 경우에 먼저 화면에 새로운 AS 만들고 이 위에 명
령 버튼을 배치해야 한다고 가정하면 이 토대가 되는 YS 폼이라 한다. 다이얼로그 박스도 폼
의 하나이다. 쉽게 풀이하면 Visual Basico} 작성한 애플리케이션을 실행하였을 때 처음

에 나타나는 창이 폼이다.

 im, Form!

— |

Visual Basic ZZ 182 폼 위에 컨트롤을 배치하는 것부터 시작한다. 컨트롤

에서 익숙한 시각적 요소라 할 수 있다. 즉 마우스로 조작하거나 문자열로 표시, 입력하는
없어서는 안되는 도구이다. 컨트롤은 주로 다음과 같은 역할을 한다.

(a) 사용자로부터의 입력을 검출
(6) 애플리케이션에 정보를 표시

텍스트 박스, 명령 버튼, 리스트 박스 등을 컨트롤이라 하며 모두 윈도우를 조작할 때 잘 알

아두어야 한다.
테스트 바ㅅ
3S OS
명령 버튼
리스트 박스

23


===== PAGE 24 =====
24

Chapter 1

Visual Basic 2| 기본 지식을 알아보자

ee  을 입력하려면 a       ie 사용하야 한다, WOES 가의 AE 박스가 배치되어
도 실제로는 하나의 텍스트 박스에만 입력된다. 이처럼 입력할 수 있는 개체의 상태를
‘EAB 가지고 있대 a    vec, uualos EAAg 갖고 dled ※시가 나타난다, 에

들                             으면 커서가 나타나고 어떤 윈도우가 포커스를 갖고

~,

개체와 그 구성 요소의 관계를 표로 나타낸다면 다음과 같다.

표 1-3
클래스 |p sesh 작성
+
콜렉션 |              속성   *ㆍ 속성 설정
그
HAS [fe 표준 동작
Z       이벤트
:      프로시저 | re 실질적인 작동
화면상에     각각의 개체 행동과
배치해 프로그램을 동작을 규정한다
구성한다

Visual ㅁ88510 에서 프로그램을 작성하는 순서

Visual Basic 4] 프로그램을 작성하는 순서를 일반적인 베이직과 비교하면 다음  과 같다.



===== PAGE 25 =====
1.2 프로그램 구조에 대하여

일반적인 베이직

모든 절차는 오로지 프로그래밍에 의존한다.

(1) 폼(창)에 개체(컨트롤)를 배치한다.
@ 개체의 속성을 속성 창에 설정한다.
(3) 이벤트 프로시저의 코드를 작성한다.

만일 ]을 누르면 “Hello, Quick Basic” 이라고 표시하고 OS 누르면 종료하는 프로그램
을 MS-DOS # Quick 88810으로 작성하면 다음과 같다.

CLS                                      ‘StH 클리어
PRINT *1:인사말 2:종료                          `가이드 표시
20
AS = INKEY$                              ‘| 문자 입력
IF AS = “1” THEN PRINT “Hello, Quick Basic”   1]이라면 표시
IF A$ = “2” THEN END                      ‘eH 종료
LOOP

Visual Basic A= '숫자 1 을 누른다면' 이라는 식의 애매 모호한 조작 방법을 취하지
않고 각각의 AS HES 배치해서 다음과 같이 설계한다.

(1 폼을 만든다.

(0) 그 쯤안에 버튼1 과 버튼2 를 배치한다.

(3) 버튼1 에 "인사", 버튼2 에 “종료"를 표시한다.
(0) 버튼1 의 이벤트 프로시저를 작성한다(인사 표시).
© 버튼2 의 이벤트 프로시저를 작성한다(종료).

이 프로그램을 실행시키면 언제라도 사용자의 조작이 일어나는 것을 감시하고 그 조작이
일어나면 처리를 한다, 즉 이 프로그램은

(3) 뭔가 작동이 일어나면

06) 뭔가 처리를 한다
라는 식으로 처리를 한다. 이와 같은 방식의 BATA Event-driven Programming(At
상 중심 프로그래밍) 이라고 부른다.

25


===== PAGE 26 =====
Chapter1 Visual Basic 2| 기본 지식을 알아보자

여기에서는 (8)를 이벤트라 불린다. 예를 들면 HES

클릭하거나 키를 누르면 이벤트가
발생하고 그것에 대응하는 이벤트 처리 프로그램이 실제로 작동

한다. Visual Basic 에서는

이것을 이벤트 프로시저` 라고 부른다. 이벤트와 이벤트 ZEA) AE Visual Basic 2] 기본
이 되는 것이다. 이것이 Visual Basic 의 프로그램 방법이다.

Visual 38810에서 코드를 작성할 때 프로그램 기술을 편리하게 해 주는 몇 가지 지켜야 할
사항으로 다음과 같은 것들이 있으므로 꼭 외워두어야 한다.

Visual Basic 의 주석(2000046010은 단일 따옴표(')를 사용한다. 한 행 중에 ''' 이하는

무시된다.
A = 100 '초기 설정문         도중에 (')를 쓰면 이후는 주석이 된다
작성일 5월 23일          앞에 (')를 두면 행 전체가 주석이 된다

 복수 명령문
Visual Basic 은 한 행에 하나의 HAS 쓰는 것이 기본이지만 콜론(:)으로 구분지어 한
행에 복수의 문장을 쓸 수 있다.

A = 100                      한 Yo] 한 문종
A = 100 : B=200 : 0=300      한 행에 복수의 문

 문장을 복수 행으로 분할
IFES 출력문에서 한 행이 너무 긴 경우 그냥 입력해도 좋지만 화면에서 벗어날 수 있
으므로 귀잖더라도 스크롤 조작을 해야 한다   이정  af 행 끝에 행 단결 문자 「공백 문자+
  」를 를 사용해서 분할할 수 있

26


===== PAGE 27 =====
A="aaa” & “bbb”   한 행에 썼다
2="“83828" _         행 단결 문자를 사용했다
&” bbb”

B="aa _          의 경우는 불가능하다. 공백 입력 가능 장소에서 BS
a” & “bbb”

C=100 +_
200

수를 사용할 때에는 다음처럼 한다.

255              이것은 일반적인 10 진수 =
&0377             8진수로 표기한 255. “&O"S 붙인다
&HFF              16 친수로 포기한 255," +

t\r
a

16 진수 표기 등의 경우에 뒤에 % 을 붙이면 ‘Long’ 의 값이 된다. 이것은 부호가 없
에서 사용할 경우에 매우 중요하다.

A = &H8000       A #2-327682 된다
B = &H8000&      B We 327682 된다
C = &H8100       C 값은-32512로 된다
D = &H8100&      D #2 330242 된다

 대문자와 소문자의 구별

Visual 88810은 대문자와 소문자를 구별할 수 없다. 예를 들면

같은 것이 되어 버린다. 단지 Visual 88810의 편집기는 선언시 사용한 문자로 자동

Dim Data As Integer

라고 선언하면 이하의 코드 부분에서 “DATA”, “data” 10818 로 입력해도, "10818 로 통일
된다. 즉 Visual Basic 1] 사용자는 다음처럼 하는 것이 보통이다.

27


===== PAGE 28 =====
Visual Basic 의 기본 지식을 알아보자

-시작이 되는 단어의 첫 자는 대문자로 한다

예를 들어 “yourdata’7} 아니라 “YourData’= 인식된다. 이것에 의해 (언어 류에
“7040 data’ 로 하지 않아도 알기 쉬운 명칭이 된다. 또 첫 글자를 대문자로 하여 프로그래밍
할 때 다음의 반응을 봄으로써 바른 변수명을 확인할 수 있다.

“yourdata”"= 입력 — “‘YourData”’= 변화
이것은 대단히 편리하다.
한국어 사용

Visual Basic 2 변수명과 프로시저명에 한국어를 사용할 수 있다. 한국어를 사용하면 =
로그램이 알기 쉽게 된다. 예를 들면 다음의 이미지 프로그램을 보자.

Dim 금액 As Integer, 단가 As Integer
Dim #243 As Integer, 개수 As Integer

If 재고가 있는(부품번호) Then
금액 = 단가 * 개수
출하처리를 한다

End If

Private Function 재고가 9J+(nbr As Integer) As Boolean
(무엇인가 기술)
End Function

Private Sub 출하처리를 한다()

(무엇인가 기술)
End Sub

단지 컨트롤, 폼, 클래스 및 표준 모듈의 이름에는 한국어는 사용할 수 없다. 초보자는 혼란
스러움을 피하기 위해서 「변수명과 프로시저명에서 한국어 사용 가능」이라고만 기억해 두자.

28


===== PAGE 29 =====
1.4

oh
따

Visual 88886은 「간단히 윈도우용 야플리케이션을 작성 가능』하게 해 주지만 내용을 개
발하는 것은 쉽지 않다. 그러나 기초가 제대로 되어 있어야만 한다. 따라서 이 책은 입문자
가 충분한 기초 AAS 효율적으로 익힐 수 있도록 다음과 같은 구성으로 학습 방법을 제시

~
하고 있

a

# 제1장 LA Visual Basic 2| 기본 지식을 알아보자.

Visual 88810을 이해하기 위해서는 우선 Visual 828810의 일련 AAS 간략히 체험하는
것이 효과적이다. 처음부터 마지막까지 대충 체험해 보면 이후의 학          을
인가」를 파악하기 쉬워진다. 이 장은 사전 지식없이 대강 owe
득하는 것이 가능하다.

# 제2장 어떻게 Visual 88510 프로그램을 만들 것인가?
# 제3장 Visual Basic 2| 기본 조작

이 두 장은 「사용 방법」에 대한 내용이며 Visual Basic 같은 개발 환경을 갖는 시스템의
경우는 그 개발 환경 자체의 사용 방법을 충분히 이해할 필요가 있다. 최근    애플리케이션은 온
라인 도움말 전성기로 만족스런 페이퍼 매뉴얼이 첨부되어 있지 않은 경향이 있다. 이 장은 기
본적인 용법을 자세히 설명하고 있으므로 이 장을 읽는 것만으로, 「\16481 88816의 조작」에

대해서는 충분히 이해할 수 있다.

@ 제4장 변수의 선언과 데이터형
@ 제5장 연산자

# 제6장 제어문

# 제7장 프로시저 작성

이 네 개의 장은 Visual 88810이라는 언어의 문법을 설명한다. Visual 88810의 문법도
온라인 도움말로 보든지 페이퍼 매뉴얼을 구입해야 한다. Visual 88810의 문법은 종래의
BASIC 보다 기능이 강화되었으므로 익숙하지 않은 구문도 나와 있다. 이 장에서는 이것만 알

29


===== PAGE 30 =====
Chapter 1 Visual Basic 2| 기본 지식을 알아보자

간단               4 문범에 대해서는
7 프로그래밍을 만들고 싶은 독자는 이 92 넘기고 Bae ao

다 찾아봐도 상관없다. 또 0] AS WAZ 하는 경우는 이 AGS 집에서 학습하도록 지도할

@ ABS 컨트롤의 사용
# 제9장 그 외 기본 용법

이 두 개의 장은 이 책의 핵심이 되는 것이다. Visual 88810을 실행하면 표시되는 표준 Al
트롤의 기본적인 용법을 전부 설명한다. 이 me AEST 사용해도 애플리케이션을 완벽히 개
발할 수 있다. 각각의 설명은 전부 같은 방식으로 간략한 설명과 샘플 프로그램을 제시하고 있
다. 이 샘플 프로그램을 변경하는 방식으로 자신이 직접 프로그램을 작성해 보면 좋을 것이다.

@ AOS 그래픽의 처리
@ 제11장 재미있는 프로그램

이 두 개의 장에서는 그래픽 처리의 방법에 대해서 설명하고 있다. Visual Basic 2] 그래픽
처리에서는 단지 ALS AY 라는 SAS 외견상 나타내기 위해서 그림자처럼 활동하는 기능
 많다. 그것들에 대해서 설명하고 있다. 또 잠시 쉬어가기 위해서 그래픽을 사용한 재미있

프로그램을 5 개 소개하고 있다. 상당히 짧은 프로그램이므로 자신이 좋아하는 출력의 비
올로 코드를 입력해 그림 화면을 즐겨 보자.

# 제12장 파일 처리

aot

A
주 들

이 책의 마지막은 본격적인 프로그램에서는 빠질 수 없는 파일 입출력 처리로 시퀸스, a
덤, 바이너리의 각 액세스 방식에 대해서 설명한다. 파일 처리 자체는 플러스 4(알파)의 기능
이므로, Visual Basic 9] 다른 기능을 마스터하고 그 다음 순서로 읽어 나가자.

0

때

이상의 구성은 많은 고민 끝에 순서

을 것이다. 단지 문법만은 별개이

정한 것이다. 가능한 이 순서로 읽어 나가는 것이 좋
법 부분은 필요할 때마다 페이지를 보기로 하자.

도
Ad 개

sof


===== PAGE 31 =====
= CHAPTER

어떻게 Visual Basic
프로그램을 만들 것인가?

이 장에서는 Visual Basic 프로그램 개발 방법에 대하여 간단히
개한다. Visual Basic 에 대하여 상세한 지식은 0

로 화면에 표시된 순서에 따라 편히 읽어 보기로 하자.
Visual Basic 의 실행과 컴파일, 저장 등의 일련의 AAS 책
체험하게 될 것이다.



===== PAGE 32 =====
Chapter 2 어떻게 Visual ㅁ52510 프로그램을 만들 것인가?

Visual Basic 22142 일반 베이직 프로그래밍 방법과 크게 다르다. 이것은 16481
28810과 일반 베이직의 차이라고 하기보다 “MS-DOS 프로그램과 윈도우용 프로그램의
작성 방법의 차이"라고 말할 수 있다. 여기에서는 AE Visual 88810 프로그래밍은 어떻게
만드는지를 화면의 예로 표시하기로 한다. 이 장에서는 눈으로 보는 것만으로도 충분하다. 자
세한 것은 뒤에서 정리하여 설명할 것이므로 7pH yy] 읽어 내려 가 보자.

여기에서 작성하는 것은 「인사 프로그램」으로 실행하면 그림 3-1의 화면이 된다.

제목 tle  wi

을 넣는다

로

「시작』」버튼을 클릭하면 616,             「종료」버튼을 클릭하면
Visual Basic 이 출력된다                 종료된다

Visual 88810 프로그램을 작성하기 위해서는 먼저 Visual Basic 개발 환경을 실행해야 한
다. 실행하는 방법은 윈도우상에서 일반 애플리케이션을 실행하는 것과 같다. Visual Basic
을 설치하면 시작 메뉴에 등록되므로 실행 방법에 대하여 알아보기로 하자.


===== PAGE 33 =====
2.2 Visual Basic 실행하기

33


===== PAGE 34 =====
Chapter 2 어떻게 Visual Basic 프로그램을 만들 것인가?

Ser 심자                                                속성 창
도구 모음

Be 프로그램의 기본적인 크기가 된다.           폼 레이아웃 창
이 크기는 네변을 드래그하여 조정할 수 있다.

주) 실행 화면에서 0+0]6011-[01101001171이라고 하는 윈도우가 표시되는 때에는 그 창의 최대화 버튼을 클
릭하면 위 화면과 같이 작업창이 커진다,

여기를 클릭하면 위 화면이 된다. 화면 설정 방법에 대해서는
Visual Basic 의 기본 24KCHAPTER 3/)에서 설명한다.

34


===== PAGE 35 =====
2.3 폼에 제목 붙이기

폼은 작성하는 프로그램의 윈도우가 되며 자신이 좋아하는 크기로 변경할 수 있다. 폼의 제
BO 기본으로 “Forml” = 되어 있지만 변경이 가능하다. 제목 표시줄의 제목을 “최초의 프
록그램"으로 별경할다

(1) 여기를 클릭하고 4

프로그램' 이라고 입력한다

[10

여기에 마우스
드래크히면 폼의 크기2

포인트를 올려놓고      제목 표시줄의 속성명
| 변경된다.         “Caption” 0|C}

35


===== PAGE 36 =====
“WDisabledPicture (3)
E           i            (없음)
(없음)

(2) ㅅ&점부터 ㅁ8점까지 드래그하면 명령 버튼이 나타난다
버튼명은 표준으로 6000003001로 되어 있다
두 번째 명령 HES 배치하면 command27} 된다

36



===== PAGE 37 =====
2.4 HES 배치하기

ㅁ 2 Project! (Projectl)
3 폼

는
ommand! CommandButton

OOueM@>r ie

® 제목이 변경되었다

© S$ Projecti (Project!)
oS
& Fort (Formty
ommand2 CommandButton    4

command2 & 변한다(그 버른의 속성

배치할 THRICE command                         = FF
zl

2
=
스         4    즌 으
변경할 수 있다) 시작 버른을 클

oF ~

co

릭하면 다시 commandl°?l 된다

37



===== PAGE 38 =====
L_ 6 배치히고 싶은 RS 드래그해서 텍스트

peg  Ac
박스를 배치한다. 이 Ato “Textt”

raid

x      |
이라고 표시되어 있다

©
요
시
00
0
Ju
Ol!
Q
OH
.-3
10
Hl
ie
nun
EI
0
4
rif
그

| [Multiline     False

OLEDragMode 0-45

|                                              :                                 OLEDropMode 0-2
§                           P:    dChar

|                                                 위                            {RightToLeft    False
|                             a       가라는 60018065 0-88
(                   디                 |18010068
|                       9) “Text” 이 삭제되었다                     rats     2
‘ag

38


===== PAGE 39 =====
2.5 이벤트 프로시저 만들기

컨트롤 배치가 끝나면 컨트롤을 클릭했을 때에 처리시키고 싶은 일을 작성한다. 그 방법은
코드 에디터에서 이벤트 프로시저를 작성한다(그림 2-11~2-13).

(1) 전 화면에서 시작 버튼을 더블 클
버튼의 이벤트 프로시저 작성 화면이 나타난다.

[데아

jo Sub Command1_Click()
nd Sub

Causesvaldatio True
Default               False
DisabledPicture (없음)
DownPicture (없음)
Dragicon      (없음)

은 문자 입력 위치를 나타내는 커서이다

@ 프로시저의 처음과 마지막 HE 자동으로 나타나므로
이 내부에 이벤트 프로시저를 입력한다

39


===== PAGE 40 =====
40

Chapter 2 어떻게 Visual ㅁ28610 프로그램을 만들 것인가?

Private Sub 000060012011다()

Text!.Text = “Hello, Visual Basic”
End Sub

@ 입력이 끝났으면 이 버튼을 누르

ce T—

고 앞의 폼 화면으로 돌아간다

863 더     ~ㅋ…ㅋㅜㅠ××*…ㅠ“ㅠㅠ ㅋㅎ…ㅠㅠㅠ …*＊ㅠㄴㄴ
Lee ee 수 에 에 루비 차 가 개

방법으로 종료 HES 더블 클릭하여 이
그램의 종료 지시이기: 때문에 ‘End’ ala 22

10  =

1

호그

Private Sub Command _Click()
Text!.Text = “Hello, ¥isual Basic”

Private Sub Command2_C1 ick( )
End
End Sub

auses Validatio True
Default       False
DisabledPicture (없음)
DownPicture (없음)
Dragicon



===== PAGE 41 =====
2.6 프로그램의 실행

Private Sub Command!_Click( }
Text1.Text = “Hello, Yisual Basic”

41


===== PAGE 42 =====
Chapter 2 어떻게 Visual ㅁ58510 프로그램을 만들 것인가?

ae 경우 두 $91 ae Aaa 필요가 있다,

그림 2-15 O44 그림 2-18까지는 참고를 위하여 먼저 폼 파일의 저장 방법을 보여 주

음으로 프로젝트 파일의 저장 방법을 보여 준다. 먼저 프             장해도 상관없다.

Visual Basic? 폼 저장의 필요 여부를 판단해서 만일 필요하다면 폼 파일의 저장 화면이 자
으로 나타난다.

2-10

42


===== PAGE 43 =====
2.7 파일 저장

(2 보관하기에 적절

(3) ‘aisatu.frm’ 이라는
입력한다.

한

Appearance

AutoRedraw

1-30
False
(@ eHe000000Fe” ,



===== PAGE 44 =====
milo
ye
nun
>쪼
[은
니
도

Chapter 2 어떻게 Visual Basic ZB

Project! (Project!)
15

Gl sHeoo0000F
2- 크기 조정 74%
2 Ao] 프로그 yt
True
True           %
13-불사펜

회

6

(2) 여기를 클릭해서 저장

44


===== PAGE 45 =====
2.8 새로운 프로그램 작성하기

계속해서 다른 프로그램을 작성하고 싶을 때에는 개발 환경을 전부 지우고 거기에 새로운
프로젝트를 지정한다(그림 3-19~그림 3-21).

False
=]

[>
%
해:

더 &He000000Fé
2 - 크기 조정 기

HA 프로그램

True          |
True          iq
13-8 [5
0 - 단색       x

45


===== PAGE 46 =====
46

Chapter 2 어떻게 Visual 52510 프로그램을 만

fun

Project! (aisatu.vbp)
S442
BF

최초의

True

True

13 - 복사 펜
0 - 단색

Api
jAutoRedraw
BackColor

ControlBox
DrawMode
DrawStyle

= @ 새로운

화면이 나타나며 여기서부터 프로그램을 작성한다



===== PAGE 47 =====
2.9 저장된 파일 불러오기

이전에 작성한 파일을 불러와서 프로그램 수정 등을 할 때는 프로젝트 파일을 불러온다. 여
기에서는 앞에서 작성한 41880 HAUS 불러 보자(그림 3-22~그림 2-28).

| [BorderStyle
| {Caption

| {ClipControls
_ |ContralBox
| |DrawMode

| {DrawStyle

주) 최근 Agel Mee! OTOL 등록되어 있다면 OTS. 클릭하면
그 mag 열 4 있다. 등록되어 있을 때는 OR! 방법이 간단하지
만 여기에서는 표준적인 방법을 제시한다

47


===== PAGE 48 =====
Chapter 2 어떻게 Visual ㅁ53610 프로그램을 만들 것인가?

@ 불러올 Wes 더블 클릭한다

Appearance
AutoRedraw

Private Sub Command1_Click( )
Text!.Text = “Hello, Yisual Basic”
End Sub

Private Sub Command2_Click( )
End
End Sub
orm!

48



===== PAGE 49 =====
2.10 실행 파일(.6×6) 만들기

@ 여기를 클릭한다

최초의  Eade.
True
True

— © 폼이 표시되었다

완성된 프로그램을 실행 파일 (exe) 만들면 개발 후

환경을 실행한 상태가 아니더라도 윈
도우상에서 보통 애플리케이션으로서 실행할 수 있다(그림 2-

-26~크림 2-27).

49


===== PAGE 50 =====
Chapter 2 어떻게 Visual ㅁ08610 프로그램을 만들 것인가

ance

1® 여기를 클릭한다

Vb6
Visdata

False

2 - 크기 조정 7
최초의 프로그램
True

True

13 - SA}

50


===== PAGE 51 =====
2.11 Visual Basic 종료하기

프로그램 작성이 끝났다면 Visual Basic 개발 환경을 종료시킨다. 종료 방법은 보통 윈도
우 조작과 같다(그림 2-28).

그림 2

(1) 여기를 클릭하면 종료된다
[파일-)]-[종료(>)]를 사용해도 된다

orm (Form))

8 Project! (aisatu. vbp)
Bas

2 - 크기 조정 기
최초의 프로그램
True

True

13 - SAt

0 - 단색

@ 저장하지 않은 경우에는
이 화면이 출력된다

51



===== PAGE 52 =====
만

nin
ws
ro
NX
ACY

실행 파일을 윈도우 탐색기 등에서 선택해 실행할 수 있다. 또 윈도우의 표준 조작에서 시
작 메뉴로 등록하는 것도 가능하다(그림 3-29).

에               CJ            Vohelp. srg
= CQ Program Files                                                  Medaka
{3 폰트          ~
Qi Accessories ©
@ ©) Adobe

Vbaexeb.lib
Vbdatavw tb,
Vbext. srg

ci

(1) 2-11에서 저장한 파일을 찾아서 더블 클릭한다
@ 실행되었다

52


===== PAGE 53 =====
Jud
1 CHAPTER

Visual Basic
기본 조작

Visual BasicS 처음 시작하면 프로그램을 만들기 위한 Visual
83910만의 개발 환경이 나타난다. 이 장에서는 독자 여러분이 윈도우
환경에 익숙하다는 전제하에서 프로그래밍에 대해 AHS 한다.

=

=
독자 여러분에게 윈도우 환경에서의 SAS 보다 첩게 이해시키기 위

os

하여 CHAPTER 2의 「어떻게 Visual ㅁ88910 프로그램을 9

o

를 가지고 설명을 하므로 복습하는 기분으로 결ㅋ=

ol    [에
fel

=

것인7

i=
노르 시  if



===== PAGE 54 =====
i

Chapter 3 Visual Basic2| 기본

Visual

Visual Basic 바르게 인스톨하면 메뉴 시스템 안에 등록된다. WES 이 중에서 Visual
Basic 6.0이라는 항목을 클릭해서  1 윈도우 탐색기에서 실행 파일을 더블 클릭해
도 실행된다. 실행 파일의 HAE 인스톨시 지정한 위치에 따라 다소 차이가 있다. 예를 들면
다음과 같다.

C:\Program Files\Microsoft Visual Studio\Vb98\Vb6.exe
C:\Program Files\Vb98\Vb6.exe

또 실행 파일 아이콘을 데스크탑에 복사하면 아래와 같은 Vb] 바로 가기 아이콘이 만들어진다.

&

VbB

위의 Vb6 의 바로 가기 아이콘을 더블 클릭해도 된다(그림 3-1, 1H 3-2)

54|


===== PAGE 55 =====
3.1 Visual Basic2| 시작

크림 3-2

 새 파일을 작성할 때에는 이긋에서 프로그램의 타입을 선택한다
ActiveX 인터넷의 브라우저 수식 등의 기능을 갖는다

 이미 작성되어 있는 프로그램을 수정할 때에는 이 HS 클릭한다
기존 파일 불러오기이며 [파일[-)] - [프로젝트 열기(2)!와 같다

이미 작성한 프로그램 중에서 최근 사용한 파일은 이 Holl
등록되어 있어 쉽게 선택할 수 있다. 여기에 파일명이 있으
면 활씬 편리하다. 즉 여기에 등록되어 있는 리스트는 파일
메뉴에서 표시되는 파일명 리스트와 동일하다

ee   =  |
{      ActiveX EXE ActiveX DLL ActiveX VB    VB 마벌사 | ||
| 998 Ave   “   Bey ES ERY

수           “$       4

EL    Be    추가 기능 Activex SM Activex 문서 OHM

이곳을 클릭하여 표시가 나타나면 다음에 Visual BasicS
실행하면 화면에 새 프로젝트 대화 AA} 표시되지 않는다.
프로젝트 대화 상자를 다시 표시하기 위해선 [도구]-[옵션]-
[환경] 탭을 사용한다

보통 작성하는 프로그램은 "표준 EXE’ S 클릭하여 사용하며
Visual Basico 실행하였을 경우 반전 상태로 나타난다

55


===== PAGE 56 =====
Chapter 3 Visual Basic2| 기본 조작

Visual BasicS 실행시켜 가장 먼저 나타나는 화면의 네 모서리를 드래그해서 화면상에서
최적의 크기로 만들어 보자. Visual Basic 화면은 그림 3-3처럼 구성되어 있다(주:실행 화면
에서 Projectl—Form1(Form)°|24}= 새로운 창이 표시되면 그 창의 최대화 HE mS 클릭한

— 도브

다. 그림 3-3과 같은 화면이 된다(2장의 3-2 Visual Basic®] 실행 참조))

그림 3-3

도구 모음
메뉴 바

Clipcontrols  i
| ControlBox

=z 모선리를 드래그하여
윈도우를 크게 한다
폼 레이아웃 창

도구 상자

메뉴 바
Visual 88810에서 애플리케이션을 개발하기 위하여 필요한 모든 기능이 있다.

도구 모음

메뉴 바에서 사용 빈도가 높은 항목을 아이콘화하여 모아 놓은 곳이다. 이 아이콘을 클릭하면
해당 메뉴를 선택한 것과 같게 처리된다.

56


===== PAGE 57 =====
3.3 Visual Basic 2| 화면 레이아웃

도구 상자
Visual Basic 의 표준 컨트롤로서 폼 상에 표시하여 사용한다.

폼

만일 폼의 크기를 변경하지 않는다면
하여 나타나는 창의 크기는 동일이다

프로젝트 탐색기
작성하고 있는 프로그램이 어떠한 모듈(파일)로 구성되어 있는지 표시해 준다. 최소의 프로그램
은 파일 BES 하나 가지고 있다. ZBAE* Visual 828810의 프로그램 전체를 설명하는 것이
고 애플리케이션은 프로젝트 하나에 해당된다.

속성 창
현재 편집중인 개체(폼과 ALS 버튼 So] Visual 8880에서 준비되어 있는 속성을 제시해 준다.

폼 레이아웃 창
폼이 화면상에서 어떻게 배치되는가를 확인하는 것이다(그림 3-8 참조).

가

Visual Basic 화면은 자신이 작업하기 쉽도록 다음처럼 화면을 변경할 수 있다.

@ Visual Basic 작업화면 전체를 최대/자유/최소 크기로 변경할 수 있다.
ㅇ

@ 가능한 한 폼을 크    —_    ay le 수 있도록 레이아웃 할 수 있다.

# 도구 상자 크기와 장        바꿀 수 있거나 사라지게 할 수 있다

@ 프로젝트 탐색기,  i ‘az 폼 레이아웃 창의 크기와 HAS 변경하거나 삭제할 수 있다.
@ 각각의 HS 도킹형이나 비 도킹형으로 변경할 수 있디   dpe  은 복수의 창이 fete 있

내   고
02! 0
00
Hi
2
zo om
 0
! 0
ow
명 .
10

고, 개별로 이동할 수 없다. Visual BasicS 실행하
로 하면 창을 뿔뿔이 배치할 수 있다. 예를 들면 도구 에
업에 방해가 되지 않은 곳에 보낼 수 있어 폼의 작업 영

에 붙이는 방   법과 마찬가지로 너나   내 위치에 붙일 수 있다

57


===== PAGE 58 =====
Chapter 3 Visual Basic®| 기본 조작

을             }을 최대화시키면 당연히 넓어지지만 작업성이 떨어지는 면이 있다. 이
|유는 장에서 oe 이동할 때에 특별한 버튼 조작과 키 조작이 필요하기 때문이다.

해 두면 각각의 창의 일부를 보여 주어 그 창의 아래 부분을 클릭하는 것
으로도 간단히 윈도우를 전환할 수 있다. 프로그래밍 중에 코드 에디터와 폼 SAS 빈번히 왕
래하기 때문에 전환의 용이성을 확보하는 쪽이 유리하다. 다음처럼 창을 구성하면 편리하다.

@ 폼 레이아웃 창을 감추어 두었다가 보고 싶을 때마다 나타나게 한다.
@ 간단한 프로그램인 경우라면 프로젝트 탐색기도 감추어 둔다.

@ 속성 창은 항상 오른쪽에 위치시킨다. 단지 SS 가능한 좁게 해서 폼 레이아웃 SS 위해서
비워 둔다.

지금부터 그림 3-4에서 그림 3-9까지의 TAS 이용하여 Visual Basic 화면 레이아웃 조
작 방법을 알아보기로 하자.

그림 3-4

|
|

ORS 클릭한 상태에서 드래그하면 도구 상자 위치가 변경된다. 작업

창 중앙에 가까이 가져가면 독립형 창이 되고(설정 화면 8), 화면의

네 곳의 가장자리까지 드래그하면 그 위치에 도킹한다(설정 화면 <)
여기를 클릭하면 설정 화면 D 타입으로 옮겨진다

ㅣ
여기를 상하로

드래그하면 비
율이 변경된다 [409
i       Peeve ele

Form
True

여기를 왼쪽으로 드래그          ae
하면 도구 상자 좁아진다 드래그하면 창이 |
좁아진다

Ｌㄴ 여기를 아래로 끝까지      여기를 상하로 드래그
드래그해서 가능한 한      하면 비율이 변경한다
화면을 크게 한다

58


===== PAGE 59 =====
3.3 Visual Basic2| 화면 레이아웃

56 Project! (Project!)

‘orm

Appearance     1-30
_{AutoRedraw — False
BackColor       Gj sH8000000F:
. [BorderStyle     2 - 크기 조정
Be Captior        Form!
{ClipControls 1146
ControlBox     True
DrawMode        13 - 복사 펜
Drawstyle      0 - 단색

59



===== PAGE 60 =====
60

Chapter 3 Visual Basic2| 기본 조작

그림 3-/

— @ 이 HES 클릭하면 설정화면 ㄷ가 된다

@ 이 버튼 또는

@ 이 HES 클릭하면 설
정 화면 A= 돌아간다

|. | Private Sub Command! “Click()
Text!.Text = “Hello, Yisual Basic”
End Sub

Private Sub Command2_Click( )
=      End
End Sub

ee ee 즈제제즈즈제
ee eee eee ee ee ee eee

화면에 현재 S 위치와
크기를 나타낸다

(1) 폼과 코드가 동시에 표시된다.
(효과를 알기 쉽게 하기 위해서 먼저 만들었던 86804.006를 읽어 보았다)



===== PAGE 61 =====
3.3. Visual Basic2| 화면 레이아웃

@ 스크롤 바를 조작해서 제목 표시줄의 오른
쪽 끝 부분에 있는 복원 버튼을 클릭하면
설정화면 [로 되돌아간다. 사실 이 조작은
제목 표시줄을 더블 클릭하는 것이 더욱

Private Sub Command2_Click( )
End
End Sub

| ㅣ 티티 그

® 가능한 최대 크기가 된다. 단지 표시는 이
창안으로 스크롤 장소가 표시된다. 이것은
설정 화면 AQ 작성 폼(여기에서는
Form1)2| 최대화 HES 클릭해도 같다

@ 여기를 보면 폼
이 최대로 되었
다는 것을 알
수 있다

56 00601 (aisatu,vbp)
aa &
5 Formt (aisatu.frm)

False

‘Gi sHe0o0000Fe
2 - 크기 조정 7.
:최초의 프로그램 개
True
True
13-복사펜 ©

'0 - 단색      회

더

여기를 통해서도 폼
의 크기가 최대로
되었다는 것을 알
수 있다

61


===== PAGE 62 =====
Chapter 3 Visual Basic2| 기본 조작

어느 정도 프로그램의 골격이
나온다면 속성 창은 가능한
좁게 한다.

프로그램 작성이 익숙해지면 새로운
컨트롤을 배치하는 일은 없어지므로
도구 상자 전체를 감추어 두게 된다

폼 레이아웃 창은 감추어 둔다. 항상 띄 -ㅡ
As 정도로의 사용 가치는 없다.

보기 메뉴의 폼 레이아웃 창을 이용하여
다시 나타나게 할 수 있다

62


===== PAGE 63 =====
3.4 메뉴 바와 도구 모음

뉴 바에 집약되어 있어서 파일의 저장과 불러오기도 이 메
뉴 항목에서 지정한다. 메뉴 바 중에서도 사용 빈도가 높은 기능은 버튼 형태로 도구 모음에
표시되어 있다. 메뉴 바 앞에 표시되어 있는 그림은 도구 모음에 아이콘으로 표시되어 있다는
것을 의미하고, 뒤에 있는 "0800+@"로 표시되어 있는 문자는 단축키를 표시한 것이다. 메뉴
바 앞에 그림은 있으나 표준 상태의 도구 모음에 표시되지 않는 경우는 [디버그], [폼 편집기],
[편집] 도구 상자에 버튼이 표시되어 있다. 메뉴 내용은 상황에 따라 변화하는 경우가 있으며
다음의 EEL 메뉴 바에서 각 도구 모음의 위치를 설명한 것이다,

Visual Basic 의 편집 기능은

—  CH    |
때   폼 편집기 |

sal
il

ral
ies

\

[파일)]-[새 프로젝트(4)] (CHIH)
새로운 프로젝트를 작성한다

 [파일『)]-[프로젝트 열기(0)] (CH+0)
저장되어 있는 프로젝트를 불러온다.

[파일(『「)]-[프로젝트 471D)]
새로운 프로젝트를 추가 작성한다.
[파일(『「)]-[프로젝트 제거()]             4
현재 프로젝트를 프로젝트 그룹으로부터 제거한다 |
(저장은 되어진다).                                      |
=                 @ [D(F)}H{ZeaWe AAV)
현재: ZBAE(vbp 파일)와 프로젝트에 포함된 폼/1412[폼/표준/클래스 BSS 저장한다. |

63


===== PAGE 64 =====
64|

Chapter 3 Visual Basic 의 기본 조작

[파일『)]-[프로젝트를 다른 이름으로 저장(6)]
작업중인 프로젝트(.002 파일)를 새로운 이름으로 저장한다
[파일(『)]-[『0「01 저장(6)] ((여01+[9])
현재 선택되어 있는 폼/표준/클래수 BES 저장한다. Form27} 선택되어 있다면
[Form2 2] 저장(8)]이라고 표시된다.
[파일(『)]-[『0[0711을 다른 이름으로 저장(4)]
현재 선택되어 있는 폼/표준/클래스 모듈을 새로운 이름으로 저장한다.
[파일(『)]-[선택 영역 저장(Ｌ)]
선택된 항목의 릴레이션(06181100) AAS 보존한다(데이터베이스 디자인으로 사용한다).
[파일(『)]-[변경 스크립트 저장(1)]
SQL 명령문을 sql 파일로 해서 보존한다(데이터베이스 디자인과 테이블 디자이너로
사용한다).
즐 [파일(6)]-[인쇄(2)] ((여0+06])
폼과 코드를 laste}.
Dy [파일(『)]-[인쇄 설정(/)]
기본으로 선택되어 있는 프린터의 기능을 설정한다.
[파일(『)]-[마이6여1.6>6 만들기(()]
실행 파일(.6※6)을 만든다.
[파일(『)]-[프로젝트 그룹 만들기(3)]
프로젝트마다 개별 실행 파일을 작성한다.

[파일(-)]-[종료(×)] (A+)

마이크로소프트 16481 88816 을 종료한다.

/ Beet \

Bi [편집(6)]-[실행 AA(U)] ([여01+121)

마지막으로 편집했던 내용에서 전 상태로 돌아간다(20 회분의 문자 편집 조작까지 유효).
 [편집(6)]-[재실행(『)]

[실행 취소]명령하였던 내용으로 원상 복귀한다.



===== PAGE 65 =====
3.4 메뉴 바와 도구 모음

W [편집(6)]-[잘라내기(1)] ([여+0)
선택한 컨트롤과 문자열을 제거해서 SARE 저장한다.
&) [편집(5)]-[복사(-)] ((01+(61)
선택한 컨트롤과 문자열을 클립보드에 복사한다.
 [편집(6)]-[붙여넣기(2)] (c+)
클립보드에 저장된 내용을 커서가 있는 위치에 삽입한다.
[편집(6)]-[연결하여 붙여넣기()]
DDE (다이나믹 데이터 익스체인지) 소스로의 연결선

[편집(6)]-[삭제(2)] (Ded)

현재 선택되어 있는 컨트롤, 문자열, 또는 조사식을 삭
제한다.

[편집(6)]-[데이터베이스로부터 테이블을 제거(8)]

데이터베이스로부터 선택된 테이블을 삭제한다(데이터

[편집(6)]-[전체 선택(4)] ([여01|+시)
코드 화면의 전제 ES 선택한다.

[편집(6)]-[전체 열 선택(4)]
입력 소스 윈도우의 모든 SS 선택(쿼리-디자이너로 사용한다).

[편집(6)]-[테이블(8)]
[기본 키 SAM) [열 FAO) [열 삭제08)]
데이터베이스의 테이블 조작을 행한다(테이블 디자이너, 데이터베이스 디자이너로 사용한다).

—— ee ee

 [편집(6)]-[찾기『)] ((여+)

문자열을 검색한다.

[편집(6)]-[다음 찾기(4)] (09 다음 6001+09)
문자열 검색을 반복한다.

[편집(6)]-[바꾸기(6)] ((Ci)+(H))

문자열을 새로운 문자열로 교체한다.

65


===== PAGE 66 =====
Chapter 3 Visual Basic 의 기본 조작

© [편집(6]-[들여쓰기()] 096
선틱되어 있는 8] TALS 다음의(오른쪽) 템 IH 이등한다.

re
st
fay
og
jo
jf
> 논
10
alu >
Ho
Je,
ie
=f
os 8
jo =
eal’
[는
x»
oe
off
esl
awl

6 [편집(6)]-[속성/메서드 sett] ((여01+미)
지정한 개체로 사용 가능한 속성과 메서드의 목록을 표시한다.
:                    S)] ((어01+[6000+미])
지정한 속성에 사용 가능한 상수 SSS #시한다.

@
rH
ital
11)
as
ox
4
0
=o

개체와 속성 등의 ERS 쉽게 표시한다.                                         |
es 이  집(6)]-[매개 변수 정보(\/)] (Cre) +Shif} +1)
수에 필요한 파라미터를 표시한다.
ㄱ: [편집(6)]-[단어 채우기(\/)] ([여01+16000)
스펠링을 잘 모를 때 적절한 단어를 표시한다
[편집(6)]-[행으로 가기(3)]
[맨 AS (F)) [맨 마지막(Ｌ)] [다음(×)] [이전(4) ][행(\)] [새 행04)]
쿼리 디자이너와 뷰 디자이너로 사용한다. 쿼리 조작 결과가 표시되어 있을 때 그
마지막 등의 행으로 점프한다.

피(안내 ve     로 정 ee sees                                      :

/ 보기00) 메뉴 .     “a

| ㅁ [보기/)]-[코드(0)] 6

현재 폼/표준/클래스 모듈의 코
SH [보기(/)]-[개체(8)] ((여0+61)

현재 선택되어 있는 개체0~00)를 표시해준다.

; a
ont
tio
AA
Ho
eal

00


===== PAGE 67 =====
3.4 메뉴 바와 도구 모음

[보기(/)]-[정의(2)] (600+6)
커서 위치의 프로시저와 변수를 정의하고 있는 부분에
점프한다.
[보기(\/)]-[이전 위치04)] (001+508+12)
전에 편집해있던 위치로 커서를 되돌린다. [정의00)메뉴에서
크게 점프하는 등에 편리, 누를 때마다 이전의 위치 돌아간다.
랭 [보기(/)]-[개체 찾아보기(0)] (@)
개체 창을 띄운다.
22 [보기(/)]-[직접 실행 창()] (예0+6)
직집 실행 창을 띄운다.
OB [보기(/)]-[지역 창(6)]
지역 창을 띄운다.
 [보기(/)]-[조사식 창7)]
조사식 창을 표시한다.
@ [보기(/)]-[호출 ACK) (A+)
호출했던 기록을 표시한다. 브레이크 BES} 경우에만 유효하다.

프로젝트 탐색기를 띄운다.
& [보기(/)]-[속성 SW)] (64)
속성 창을 띄운다.
료 [보기(/)]-[폼 레이아웃 SF)
폼 레이아웃 창을 띄운다.
[보기(/)]-[속성 페이지(3)] (6001+541)
사용자가 작성한 속성 페이지를 받아들인다.
[보기(/)]-[테이블(5)]
[열 속성()] [열 이름] [7](K)] [이름만으로04)] [사용자 정의(\)]
다이어그램 내에서의 테이블 표시 방법(예 : 열 이름을 표시할까)을 지정한다(데이터베 |
이즈, 쿼러, Tr 더자이너로 APB ey),                                                      '

67


===== PAGE 68 =====
68|

Chapter 3 Visual Basic 2| 기본 조

[보기(\/)]-[확대/축소(2)]

[200%] [150%] [100%] [75%] [25%] [10%] [선택 영역(8)]

다이어그램을 확대 또는 축소시킨다.
[보기('/)]-[창 표시(4)]

[다이어그램(2)] [표 형태(3)] [8@Ｌ(8)] [결과(2)]

지정한 창(여러 가지 결과 표시 틀)의 표시/비 표시를 지정한다.

® [27|\(V)H&t 상자(>)]

도구 상자를 표시힌다.

[17\(V)]-[Data View 창 (V)]

데이터소스로의 접속을 행하거나 그 상태를 나타내는 데이터 F AS 띄운다.
[보기(()]-[색상표(Ｌ)]

컬러 팔레트를 띄운다.

[보기(\)1-[도구 2S(L)]

[디버그] [편집] [폼 편집기] [표준] [사용자 정의(2)]

도구 모음 표시 항목을 설정한다.

[보기(/)]-[비주얼 구성 요소 관리자]

액티브 도큐먼트와 COMA 등 여러 가지 컴포넌트를 관리하는 비주얼 구성 요소 관
리자를 실행시킨다.

/ 프로젝트) 메뉴  \

|       S [ZEAE(P)-1S 추가『)]

현재 프로젝트에 새로운 폼을 추가한다.
 의 [프로젝트(-04미 폼 37H)

현재 프로젝트에 새로운 1402[폼을 추가한다,
 [프로젝트(0)]-[모듈 추가04)]

현재 프로젝트에 모듈을 추가한다.
  [프로젝트()]-[클래스 모듈 추가(0)]

현재 프로젝트에 클래스 모듈을 추가하다.



===== PAGE 69 =====
3.4 메뉴 바와 도구 모음

  [프로젝트(ㅁ0)]-[사용자 정의 컨트롤 47KU)]
현재 프로젝트에 새로운 MDS 추가한다.
 [프로젝트(0)]-[속성 페이지 47KP)]
현재 프로젝트에 속성 페이지를 추가한다.
'@[프로젝트(0)]-[사용자 정의 문서 추가(0)]
현재 프로젝트에 사용자 문서를 추가한다.
[프로젝트(ㅁ)]-[마111 Page 추가]
IE 4.0으로 사용할 수 있는 Dynamic 1101Ｌ페이지를 추가한다(이하 4 개 항목은 모두
ActiveX 디자이너이다).
[프로젝트(0)]-[ㅁ0813 Report 추가]
데이터베이스 Report S 만들어 W= Data Report 개체를 추가한다.
[프로젝트(0)]-[\/66001365 추가]
웹 처리를 행하는 WebClass WAS 추가한다.
[2241 (P)]-{Microsoft UserConnection 추가]
데이터베이스와의 AAS 설정한다.
[프로젝트(0)]-[기타 ActiveX 디자이너]
[Data Environment]
현재 프로젝트에 파일을 추가한다. 이 파일은 다른 프로젝트와 공용하는 파일이 된다.
[프로젝트(0)]-[파일 추가(4)] ((Cti+())
기타 프로젝트에서 사용하고자 하는 파일을 추가한다.
[프로젝트(2)]-[『01「011 Ml74(R)]
현재 선택되어 있는 항목을 제거한다. “Forml” HHS 선택되어 있는 항목 이름이 된다.
@ [프로젝트(ㅁ2)]-[참조(|)]
참조 가능한 라이브러리 파일을 지정한다.
[프로젝트(0)]-[구성 요소(0)] (C+)
새로운 구성요소(컨트롤 등)을 지정해서 도구 모음에 표시한다.
[프로젝트(0)]-[마이6011 속성(6)]
완성하는 프로그램용 속성 정보를 지정한다. 버전 번호와 컴파일 방법 SS 지정할 수 있다.

69


===== PAGE 70 =====
70

Chapter 3 Visual Basic 의 기본 조작

형식(0) 메뉴

A

[3

fu

복수의 a
른쪽 끝에서 정렬, 모눈에 맞추는 등의 지정을 할 수 있다.

ee 37|2(M)]

SOLIS 모는에 (0)
위치 맞출 것인지를 지정한다.

식(2)]-[맞춤(4)]

컨트롤 맞춤법을 설정한다. 좌측 끝에서 정렬하거나 오

의 AES 크지들 같게 한다.

디버그(2) 메뉴

\

현재의 프로시저 안에 남아
로 되돌아온다.

있는 HES 한번에 실행하여 누락되어 호출된

& [디버그(0)]-
한 행씩 sae
Ge [디버그(2)]-[프로시저 단위 실행(0)] haa
현재 루틴을 한 행씩 실행한다. 다른 프로시저를 불러 |
냈을 때는 그 전체를 한번에 실행해서 현재 루턴의 다 :
음 행에서 멈춘다.                                  :
© [디버그(2)]-[프로시저 나가기(0)] (Cad   +600+태) =)



===== PAGE 71 =====
3.4 메뉴 바와 도구 모음

[디버그(0)]-[커서까지 실행()] (C+)
커서가 있는 행의 앞에까지 실행하고 정지한다.
[디버그(0)]-[조사식 추가(4)]
변수값 등을 알기 위한 조사식을 입력한다.
[디버그(0)]-{조사식 편집(ㅁ)] (C+)
입력되어 있는 조사식을 편집한다.
에 [디버그(0)]-[간략한 조사식(0)] (G+)
반전 선택 지정한 변수와 속성의 값를 미리 표시한다.
©) [디버그(0)1-[중단점 설정/해제()] (@)
ANT 있는 행의 SIAL 설정 또는 해제한다.
[디버그(0)]-[모든 중단점 지우기(0)] ((여+6808+9)
프로젝트 내에서 설정되어 있는 BE 중단점을 해제한다.
[디버그(0)]-[다음 문 설정04)](800+09)
다음 실행하는 임의의 행을 지정한다. 실행 순서를 앞으로 되돌려서 지정 할 수도 있다. |
[디버그(2)1-[다음 문 표시00]
중단 모드에 있을 때 다음에 실행되는 명령문을 커서로 표시한다.

/ wR 호

 (ABRHANS)] (6)             :
He Berge 실행한다. 실행을 시작하였다가 중단 |
을 하면 [계속(0)]이 표시되고 이것은 중단된 실행을 재 |
AALS 기능이다.                                       :
6) (주:[시작(6)] 버튼과 겸용)
지 장소부터 다시 시작한다.
[ARIMA 컴파일 후 시작(『)] ((여0+9)
프로그램을 일단 완전히 컴파일하고 나서 실행한다.
| [실행(%)]-[중단(<)] (01+894)
실행중인 프로그램을 일시 정지한다.

mu
oat
2
i
7}
x 은

Pa


===== PAGE 72 =====
 00803 Visual Basic 2| 기본 조작

 [실행()]-[종료(6)]
프로그램 실행을 종료한다.
[실행()]-[다시 시작()](0+6)
프로그램을 처음부터 실행한다. 중단 BOS 되어 있을 때 사용한다.

 쿼리) 메뉴 \
Ss (ARH YHA)

[쿼리(4)]-[<136016 A) BE] SE BS 선택(6)]

[쿼리(4)]-[<13016 B) 2H 모든 HS 선택(6)]

이들 메뉴에는 마이크로소프트 116481 Database Tools 의 하나인 쿼리 디자이너에 대
한 내용이다. “디자이너"는 갑자기 코드를 기술하는 BSS 덜기 위해서 개발 환경 상에
서 비주얼 디자인용 윈도우를 제공하는 것이다, 쿼리 디자이너는 데이터베이스로의 문
의를 행하는 SQL VBS 작성하기 위한 비주얼 툴로 그것을 사용하기 위한 메뉴가 여기
에 집합되어 있다. 예를 들면 [실행08)]은 입력한 SQL 명령을 실행하고 그 쿼리 결과를
표시한다. [결과 지우기(0)]는 그 결과 표시 영역을 지우기한다. 본 책은 쿼리에 대해서
는 설명하지 않는다.

72


===== PAGE 73 =====
3.4 메뉴 바와 도구 모음

[다이어그램(| )]-[선택된 테이블 크기 자동 조정(2)]

이들 메뉴는 Microsoft Visual Database Tools 의 하나인 데이터베이스 디자이너에
대한 것이다. 데이터베이스 디자이너는 데이터베이스의 구조를 작성하고 그 개체를 작
A, 수정, 제거한 것이다. 작성 중 프로그램과는 관계없이 데이터베이스에 직접 Asal
서 테이블 내용과 테이블간의 연결 표시를 행하기 때문에 시각적으로 편집 작업을 할 수
있다. 이 테이블 내용과 연결을 표시한 것을 다이어그램이라 한다. 예를 들면 새 텍스트
주석(4)은 다이어그램에 명령을 붙일 수 있다. 관계 테이블 추가(4)에서는 키로 관련지
어진 테이블을 추가할 수 있다. 본 AS 다이어그램에 대해서는 설명하지 않는다

[도구(1)1-[프로시저 추가0ㅁ)]
새로운 프로시저와 함수의 작은 모형을 코드 화면에 추가한다. 예
를 들면 다음과 같은 모형이 삽입된다.

73


===== PAGE 74 =====
Chapter 3 Visual Basic 2| 기본 조작

[도구(1)1-[프로시저 특성(4)]

프로시저마다의 SYS 설정하다.

[도구()]-[메뉴 편집기04)](여+)

메뉴 편집기가 실행된다.

[도구)]-[옵션(0)]

Visual Basic 개발 환경 속성을 설정한다. 편집, 서식, 일반, 도킹, 환경, 고급 설정을
지정할 수 있다.

[도구(1)]-[게시(0)]

Component Manager (발행 위저드)를 실행한다. 이것은 [추가 기능(&)]-|추가 기능 |
관리자]로 지정된 항목이다. 컴포넌트 저장과 취득에 A-BSEE Repository Database |

의 컴포넌트 Wee 돕는다.                                            :

/ 추가 기능) 메뉴 \

|    과          [추가 기능(&)]-[비주얼 데이터 관리자(\/)]            |
데이터 관리자인 VisDataS 실행한다. Access, 20886, |
FoxPro, Paradox, Excel, Text File, ODBC 등의 데이

추가 7IS(A)H#7t 기능 관리자(4)]
추가 기능 관리자 SHH] Visual Basic 개발 환경의 확       le      을 Agel, 7} 7s |
의 종류와 로드 WHS 지정할 수 있다. 여기에서 nek 내용은       [도구(2)] 메뉴 또는 이 |
메뉴 [추가 기능 관리자(4)]에 추가 표시된다.

[창(//)]-[수직 바둑판식 HH S(C)]
코드 에디터와 개체 창을 좌우로 배열한다.

74


===== PAGE 75 =====
3.4 메뉴 바와 도구 모음

BW) I-AA! 배열(<)]
코드 에디터와 개체 AS 겹쳐서 표시한다.

[창(//)]-[아이콘 정렬(4)]

코드 에디터와 개체 창을 최소화할 때 그 아이콘은 화면 아래에서 정렬한다.
[AU(W)IH1 Projecti-FormS (Form)]

사용하고 있는 폼과 코드의 리스트가 표시된다. 여기에서 지정한 BO 액티브하게 된다.
즉 메뉴 표시 항목은 변화한다.

/ 도움말) 메뉴 \
Qs                    [도움말(1)]-[목차(ㅇ)]
Visual 88810의 도움말을 실행하고 목차 YS 이용한다.
[도움말(1)]-[색인(|)]                                   q
Visual Basic] 도움말을 실행하고 키워드 탭을 이용한다. |
[도움말(|1)]-[검색(6)]
Visual 28810의 도움말을 실행하고 검색 AS 이용한다.
[도움말(1)]-[기술 지원 도움말(1)]
기술 지원 서비스 관계의 도움말을 실행시킨다.
[[S2(H)]-[Web 에 있는 Microsoft 정보(\)]
인터넷의 웹 메뉴를 표시한다. 이 메뉴를 선택하면 그대로 웹 페이지에 접속된다.
[=23H(H)]H MicroSoft Visual Basic 정보(4)
Al, 저작권 사용 가능한 메모리량

해



===== PAGE 76 =====
Chapter 3 Visual Basic 의 기본 조작

도구 모음
메뉴 항목 중 중요한 것은 도구 모음에 배치되어 있다. 다음에 제시하는 표준 Et 모음의
기능에 대하여 알아보자(표 3-1) . 그것 이외의 툴 바(표 3-2~표 3-4)는 [보기(4)]-[도구
모음(1)] 메뉴 설정에 의해 표시된다.

표준 도구 모음

9@96@006960060000600600000060000606

복사

붙여넣기

문자열을 검색하다

HAS Hoe 되돌리다
실행 취소하기 전으로 돌아간다
프로그램의 실행시작

실행을 중단

실행을 종료

프로젝트 탐색기를 표시한다
속성 ae 표시한다

폼 레이아웃 창을 표시한다
오브젝트 브라우저를 표시
도구 상자를 표시한다

Data View 창을 표시한다
VCMS 표시

[파일(『)]-[프로젝트 추가(0)]

[프로젝트(ㅁ0)]-[폼 추가(『)]

[도구(1)]-[메뉴 편집기(\4)]((01+[6])
[파일(『)]-[프로젝트 열기(2)]((여00|+@))
[파일(『ㄷ)]-[프로젝트 저장(\/)]

[편집(ㄷ)]-[잘라내기(1)](|여1+[0)

[편집(ㄷ)]-[복사(ㅇ0)]((901+(0))

[편집(6)]-[붙여넣기(ㅁ)]((001+[이)
[4 A(E)]-[ 27 |(F)]( (eta) +(F))

[편집(ㄷ)]-[실행 취소(4)](|예1|+[2])

[편집(ㄷ)]-[재실행(ㅁ)]

[실행(68)]-[시작(5)](66)

[실행(68)]-[중단(<)]([(0]+66@00)

[실행()]-[종료(6)]

[보기(\/)]-[프로젝트 탐색기(『ㅁ)]((601+[8])
[보기(()]-[속성 창(\)](64)

[보기(/)]-[폼 레이아웃 창(『)]

[보기(\/)]-[개체 찾아보기(2)](2)

[보기(\)1-[도구상자(×/]
[H17|(V)]-[Data View 창(\/)]

[보기(/)]-[비주얼 구성 요소 관리자]



===== PAGE 77 =====
Mo
은

8@6909006000090900090000

SSS 11 10 ㅣ eR Ree

기능

속성/메서드의 보기

상수의 보기

요약 정보

파라미터 도움말

단어 채우기

BOI]

내어쓰기

중단점를 설정/해제

주석 248 자동으로 ag
주석 블럭을 자동으로 해제
책갈피의 설정/해제

다음 책갈피로 이동

전 책갈피로 이동

모든 책갈피를 해제

3.4 메뉴 바와 도구 모음

베뉴와 단죽기

[편집(6)1-[속성/메서드 목록("1)]((01+[미)

[편집(ㄷ)]-[상수 목록(6)]((여01|+601+미)

[편집(6)]-[요약 정보(@)]1(여1+[1])

[편집(6)]-[매개 변수 정보(/)]((여01+6001+[1])
[편집(6)]-[단어 채우기(\/)]([여01|+68099)

[편집(ㄷ)]-[들여쓰기(|)](706))

(AA (E)]-[L4 0147 |(O)] (Shift {Tab))

[디버그(『0)]-[중단점 설정/해제(1)](09)

[편집(6)]-[책갈피(83)]-[책갈피 설정/해제(1)]
[편집(ㄷ)]-[책갈피(8)]-[다음 책갈피(4)]
[편집(6)]-[책갈피(3)]-[이전 책갈피(ㅁ)]
[편집(6)]-[책갈피(3)]-[모든 책갈피 지우기(ㅇ)]

77


===== PAGE 78 =====
Chapter 3 Visual Basic 2| 기본 조작

디버그 도구 모음

© |      프로그램을 실행 시작          [실행()]-[시작(5)](5)

@         실행을 중단                  [실행()]-[중단(<)]([여0]|+6600)

@ I       실행을 송료                [#e(R)]-[SS(E)]

@ &      중단점을 설정/해제            [디버그(2)]-[중단점 설정/해제(1 )](9)

©        한 닫계씩 코드 실행           [디버그(2)]-[한 단계씩 코드 실행 (|)](68)
@         속성을 실행한다              [디버그(2)]-[프로시저 단위 Se4(O)](Ghitl+ fal)
®EB    프로시저를 나간다            [디버그(2)|-[프로시저 나가기(/)](여01+[01+ Fa) )
 a     지역 창을 표시              [보기(/)]-[지역 창(6)]

© &      직접 실행 창을 표시          [보기(\/)]-[직접 실행 창(|)]((001+(61)

© B      ANA 창을 표시             [보기(/)]-[조사식 창(1)]

00 @      간략한 조사식                 [디버그(2)]-[간략한 조사식(0)](0때+)
© B      프로시저 불러내 OSS 표시     [보기(\/)]-[호출 스택(<)]((001+Ｌ)

폼 편집기 도구 모음

S)
S
(©)

대응

(01-[만앞으로

00 &      개체를 맨 앞으로 이동          [SAHA         727 (BCC) +9)
20      개체를 맨 뒷면으로 이동       [형식(2)]-[순서(2)]-[맨뒤로(5)]([여0]+ 00)
@ &      개체의 위치를 정리한다         !행심(())-|맞줌(1

On -      AAS 폼 중앙에 배치          [형식(60)|=[폼의 가운데((.)]

© &      개제의 크기를 정리한다         [형식(2)]-[같은 크기로(\/)]

© &      컨트롤 잠그는 기능            [형식(9)| [접드몰 잠그기()|

78


===== PAGE 79 =====
3.5 애플리케이션의 조작 순서

Visual Basic A] 야플리케이션을 작성할 때에는 다음 순서를 기본적으로 취한다.
각각에 대한 설명을 하나씩 살펴보도록 하자.

| 대응한 이벤트 프로시저와 그 이외의 코드를 기술한다.

ES 메지하기

Pot

배치하기

애플리케이션의 작성은 먼저 폼 위에 컨트롤을 배치하는 것부터 시작한다.
배치 기본은 간단한 것으로 그림 3-10과 같이하면 된다.

활성화하기

폼 상에 몇 개의 ASSO] 배치되었을 때 이것을 편집
번에 하나밖에 되지 않는다. 작업할 컨트롤을 클릭하면
이 SA] er},

할 수 있는 것은(활성화 되어 있다) 한
활성화되고 그림 3-11처럼 8곳에 점

79


===== PAGE 80 =====
80

Chapter 3 Visual Basic 2| 기본 조작

에서 드래그한다.

@ 컨트롤 버튼이 나타난다

od

tae |

Projecti  (Project!
더 Fermi Form!)

DownPicture(2tS)

Dragicon

(없음)



===== PAGE 81 =====
3.5 애플리케이션의 조작 순서

수

LH Vict 그            CeO nares Nese fascias ee    ie        S
활성화된 컨트롬의 크기를 변경하거나 장소를 이동할 수 있다. 크기의 WBS che 5 20 마
크에 마우스 커서를 위치시킨 후 드래그하고 이동은 버튼 내부에 마우스 AAS 이동한 후 드래
그 한대(그럼 3-120!.

ak

ou

AS feel |

여기에 마우스 AMS 맞추면 포인트가
변한다. 화살표 방향으로 드래그하면
크기 변경이 된다

마우스 AMS 내부에 위치시킨 후 드래그하면 이동할 수 있다

N
N
(03

aS

10

때

|ㅇ

0

자적인 기능과 SAS 가지고 있으며 그 기능과 SAS 결정하기 위한
속성이 있다. 속성의 AAS 프로그램 중에서도 할 수 있지만 버튼 이름처럼 설정같이 결정
는 것은 속성 창에서 설정하는 것이 보통이다.

81


===== PAGE 82 =====
Chapter 3 Visual Basic 의 기본 조작

체의 설정

폼에 배치되어 있는 컨트롤은 각각의 속성을 갖고 있으며 애서 a  에 표시된다( =
3-14) all 원하는 컨트롤을                        fol] 표시된다. 또 속
자체의 윗 부분에 있는 개체 선

mi
Ol
[묘
by
ot
41°,
=
of
2
bo
i
_
ou

{Commandt CommandBiutton

a   ‘ommandbuttan
Form! Form
Text! TextBox

개체 선택 박스에서
지정할 수 있다

속성 보기

여기를 클릭ㅎ
Command1 속성
이 표시된다

여기를 클릭하면 Command2
속성이 eae 다

SARS 설정할 때는 먼저 그 항목 BS 클릭해서 반전 표시를 나타나게 한다(그림 3-15),
이때 입력 타입에 파라 버튼 등이 표시된다. 다음에 제시하는 입력 타입을 살펴보도록 하자.

vega     릭하여 리스트에서 속성값을 선택한다.

파일의 선택/다이얼로그 박스로부터 선택
HES 클릭하여 파일을 선택하거나 다이얼로그 박스 중에서 원하는 항목을 선택한다.

82



===== PAGE 83 =====
3.5 애플리케이션의 조작 순서

:
a
밴
Hu
Wwe
on
oh
ial

pees val cation True

efault                 rele

isabledPicture (없음
ownPicture        i é

능마다 그룹으로 분류되어 표시된다

안을
B=

아무런 버튼이 나타나지
때는 문자를 직접 입력한ㄷ
00 '
이 버튼이 표시되면 클릭하여
리스트 속에서 선택한다(주)

pels

= 이 버튼이 표시되면 클릭하여
의기 파일 선택과 다이얼로그 버튼
ㆍ 에서 선택을 한다

83


===== PAGE 84 =====
Chapter 3 Visual Basic 2| 기본 조작

| 코드 작성

컨트롤 배치가 끝났다면 실제로 실행하게 하는 일은 이벤트 프로시저에서 작성한다. 여기
에서는 예제로 간단한 스톱 워치를 만들어 보자(그림 3-16). 세 개의 컨트롤을 배치하여 표
3-5에 제시한 속성을 설정한다. 여기에 기술한 이외의 속성은 표준값을 그대로 사용한다.

(Form)                  Caption        “스톱워치”
명령 버튼1(60000ㅁㅁ98ㅁ01)        ‘Caption        “Start/Stop”
명령 버튼 20(00070ㅁ08002)        Caption        "종료"
텍스트 박스(16×%11)             Text           (S44)

이벤트 프로시저를 작성할 때에는 원하는 폼 또는 컨트롤을 더블 클릭한다. 그러면 코드 에

디터가 표시된다. 여기에서는 아직 프로그램 내용에 대해서는 생각하지 않아도 괜찮다.

00004

© ‘Start/Stop 을 클릭하면 “측정 시작"이라고 표시하고 측정 시작
9 다시 한번 더 클릭하면 “경과"라고 표시하고 측정 중지
@ 종료 를 클릭하면 프로그램 종료

84


===== PAGE 85 =====
3.5 애플리케이션의 조작 순서

컨트롤을 더블 클릭해서 코드 에디터가 표시되면 그 컨트롤의 이벤트 프로시저에 커서가
놓여진다. 예를 들면 최초의 명령 버튼을 더블 클릭하면

Private Sub Command1_Click()

이라는 프로시저에 커서가 깜박인다. 또 코드 에디터에서 다른 이벤트 프로시저와 다른 개
체를 선택할 수도 있다. 코드 에디터에는 다음의 리스트 박스가 있으므로 여기에서 선택한다

다른 개체(폼과 컨트롤)를 선택한다

이벤트 박스 선택

현재 개체에서 기술하고 싶은 이벤트에 대한 프로시저를 선택한다

예를 들면 클릭 AAs 하고 싶은 때에는 “0110"을 선택, 키 누르기를 기술하고 싶
은 때는 “KeyPress’S 선택한다

이벤트 프로시저명과 코드 입력

작성된 이벤트 프로시저명은 자동적으로 결정됩니다. 명령어는
개체이름_이벤트이름(필요하다면 인수 배열)"
이 된다. 예를 들면 명령 버튼을 클릭하면 이벤트 프로시저의 디폴트 이름은
Command1_Click()

이다. 개체 이름은 표준으로 결정되어 있기 때문에 보통 사용자가 명령하는 일은 없다(변경도
가능 다음의 NOTE 참조) 예를 들면 명령 HES 3개 배치하면 순서대로 Commandl,
Command2, Command3°| 된다. 이벤트 프로시저의 Al 행과 끝 YS 준비되어 있기 때문
에 그 사이에 필요한 코드를 입력해 간다(그림 3-17).

이 단순한 샘플 프로그램에서는 필요하지 않지만 이벤트 프로시저로부터 배열되는 일반적
인 제너럴 프로시저(소위 서브루턴)가 필요할 때에는 그것도 기술한다(7장의 프로시저의 신
규작성과 제거에서 새로운 제너럴 프로시저의 작성을 참조).

85


===== PAGE 86 =====
『

Ke

Chapter 3 Visual Basic 2| 기본

화면1 개체를 선택

GotFocus
<eyDown
pevp ree
ey
MouseDown
여기를 클릭해서 다른        1005
개체를 선택할 수도 있
다. [2000008002;를 선                           여기를 클릭하면 폼
하면 HFHIC.              트            화면으로 되돌아간다

Private Sub Command!_Click()
Static Stwach

Static Tm

If Stwach = False Then
Tm = Timer

Text1. Tent = “측정시작“

se
eke Text = Timer - Tm & “ABD”

End

seach = Not Stwch

End Sub

여기에 프로그램 BCS 기술한다. A
끝 행은 처음부터 표시되어 있다

. |DisabledPictu (없음)
DownPicture (없음)
(없음)
0 - 수동
True

is «5 «x ㅋㅋ ㄴㄴ ㅋㅋ ㅋㅋ & =

주) 똑같이 Command? Click()$ 기술한다. 왼성한 프로그램 코드는 그림 3-190] 된다.

86


===== PAGE 87 =====
3.5 애플리케이션의 조작 순서

ff] 25° 0182 변경하려면 Name Sas 변경한다. 이것은 속성 SOMME (이름)이라는 BBE 사용한
Nore] 다. 예를 들면 Command! 명령 버튼을 클릭해서 표시된 속성 창에서 아래와 같이 변경하면
이틀

이하의 프로시저명은 처음의 Commandt_Click()0| 아니고, CmdABC_Click( JAH 된다.

a

코드 에디터에서는 작성중   인 소스 프로그램을 표시하는 방법은 아래와 같이 두 가지 방법
이 있다(그림 3-18,그림 3-19).

(a) 한번에 하나의 BEAMS 구분하여 표시한다.
(6) 복수의 프로시저를 화면상에 연속해서 표시한다.

예를 들면 Command2 를 클릭했을 때 (3)에서는 Command?2_Click()°]2He 프로시저만
이 표시되지만 (6)의 경우는 다른 프로시저도 전부 표시된 상태에서 Command? 0110()에
커서가 맞춰진다. 이 방법은 [도구(1)] 메뉴에서 설정할 수 있다.

(8)를 보면 알겠지만 프로그램이 커지면 다른 프로시저로 이동하는 것이 부담스럽다. 만약
화면이 분해 표시가 되어 있다면 다음에 제시하는 설정을 하여 연속 표시로 하는 것이 필요하
다. 또 동시에 각 프로시저 사이를 가로 일직선으로 구간을 나누는 기능이 준비되어 있는데 이
것도 메뉴로 설정하는 것이 가능하다

코드를 연속 표시로 한다 : 다음의 SSS \/표시한다.
[도구(1)]-[옵션(2)]-[편집]-[윈도우 설정]-[| |전체를 모듈 보기를 7) 23° 2(M)]

코드에 Linge a :  sen ori 표시한다.
[도구(1)1-[옴션(0)|-[편집]-           설정]-|| ｌ프로시저 HEAP)

87


===== PAGE 88 =====
Chapter 3 Visual Basic 의 기본 조작

모든 코드가 표시되어 Command2_Click()2| 코드 부분에 커서가 맞춰져 있다.
른 프로시저로 이동하기 쉽다

Private Sub Command! _Click()
Static Stwach
Static Tm
if Stwach = False Then
Ta = Timer
Pe Text = "축정시작"

아아. Text = Timer - 108 "초경과"
if

3)

Stech = Not Stwch
End Sub

Private Sub Command2_Cl ick()
ni
End Subj

jue fo [

Vea" gs
{ws}

ie)

하나의 프로시저만 표시된다. Command_Click() ZBAIA 등에 이동하는 것이 귀찮다.
AMS 맞춰서 Shift] 를 누루는 또 다른 기술 조작이 필요하게 된다

betvate Sub Command2_Cl ick()
End Sud

88



===== PAGE 89 =====
3.5 야플리케이션의 조작 순서

Visual Basic? 코드 입력 중에 문장 에러를 체크한다. 이것은 입력중인 행에서 커서가 벗
어난 경우에 실행된다. 이 기능에 의해 컴파일하기 전에 단순한 에러(키워드의 실수와 구간 구
분 기호 실수 She 미리 방지할 수 있다.

문장 에러가 없다면 16081 Basic Se 코드를 내부 형식으로 변환시킨다. 이 시점에서 키워드
등은 계속 올바르게 변환되므로 문제되지 않는다는 것을 눈으로 확인할 수 있다. 예를 들면 에
러가 없으면 {07 167"라고 변환된다. 이 자동 구문 체크 기능은 기본적으로 유효하지만 만
약 이 기능을 무효로 하고 싶은 때에는 아래의 '자동 구문 검사(<) 앞에 VS 표시한다.

[도구(1)]-[옵션(2)]-[편집]-[코드 설정]-[[|자동 구문 검사(<)]

ES 작성중이라면 코드 에디터에서 여기저기에 커서를 이동시킨다. 그때

많은 코                                                                            특정 장
소로 간단하고 빨리 이동할 수 있다면 편리하다. 이 기능을 처리하기 위해서는 다음과 같은 메
뉴를 사용한다

그러나 실제로 이것을 실행할 때에는 편집 도구 모음을 불러와 사용하는 편이 훨씬 편리하
다. 프로그램이 커질수록 이 기능의 사용 빈도는 높아진다. 필수 기능이라고 말해도 좋다(작
은 프로그램일 때는 불필요). 전용 편집 도구 모음을 표시할 때에는 WHET 모음
(1)]-[편집]을 선택한다. 사용 방법은 그림 3-20 의 SHAS 보자.

89


===== PAGE 90 =====
Chapter 3 Visual Basic 의 기본 조작

@ 이것이 젝갈피 표시이다

Private Sub 00006001-011다()
아하 대
atic Tm                              =
If Stwach = False Then *“ 여기를 3행이라 st
m= Tim                              i
ett! Text = "축정시작" &----- 여기를 6   행이라 한다

껄 0 Text = Timer - Ta & "초경과"
\f

End
Stwch = Not Stwch
End Sub

Private Sub Command2_Click( )
End @

= ~ㅎ          총                        i
여기를 6행이라  한다       Appearance | - 30
BackColor (@ &H800000(
(se      False
Start/Stop
|   ausesVald  da True
Default       False
DisabledPictu (없음)
DownPicture (없음)

End Sub

‘WDragicon      (없음)
DragMode 0 - 수동

|60800160                         a
|Font
Height

® 6행에 AMS 두고 여기를 클릭하면 b 행에 책갈피 | | L © 모든 책갈피를 제거한다
가 나타난다. 다시 한번 클릭하면 책갈피가 삭제된다     . @ 이것을 클릭하면 커서가
@ 이것을 클릭하면 커서가 다음 wm} 전 책갈피가 있는 행(예:

있는 행(예:6행)으로 점프한다               행)으로 점프한다

| Py 입력 지원 기능

Visual Basic? 코드를 입력할 때에 지원 기능을 발휘한다. 예를 들면 코드 중에서 속성
을 설정하고 싶지만 무엇을 쓰면 좋을지 망설인다든지 생각이 잘 나지 않아 매뉴얼을 보지
않으면 항목을 잘 모른다는지 그 문자가 불명확한 경우가 있다. 이러한 때에 Visual Basic 은
성원 자동 목록이라는 작은 입력 지원 창이 나타나 제시한다. 그 뒤는 입력 지원 창에서 Al
택만 하면 된다.

속성 및 페서드의 구성원 자동 목록 표시.                  |
여기에서는 명령 버튼 Command! 관해 기술하는 경우를 예로 설명한다. 예를 들어 다
음과 같이 입력한 경우

90


===== PAGE 91 =====
3.5 애플리케이션의 조작 순서

Command1.Caption= 완료”
Command1 .Height=500
Commnd1.Visible=False

oh

우선 속성과 BALES] 입력 지원이다. 이것은 피리어드(.)의 오른쪽에 쓰는 것을 지원해 주
는 것이다. 신규 입력 때는 자동으로 지원된다.

Commandl,7}4] 입력하면 자동으로 구성원 자동 BS (Appearance, BackColor 등)이
작은 창에 표시된다. 그 중에서 원하는 항목을 더블 클릭(또는 항목을 반전시켜서 탭이나 A

터를 누른다)하면 그것이 커서 위치에 삽입된다. 또 이미

Command1.Caption ~

ito
보

라고 입력되어 있을 때 피리어드의 오른쪽(여기에서는 “Caption” 부분)을 변경하고 싶
에는 다음과 같은 방법으로 구성원 자동 목록을 표시할 수 있다.

© 피리어드의 오른쪽("개체명”의 오른쪽)에 커

서를 맞춘다
@ [편집06)1-[속성/메서드 목록080]0600+ )을 클릭한

za
릭한다.

작은 창은 사라진다. 이에 개의치 않

작은 창에서 선택이 불필요한 경우에는 BIS 누르면 작
한 때)에 작은 창은 자동으로 사라진다.

고 Mes ASS 적절한 타이밍('=' 와 EARS 입력

상수의 구성원 자동 목록 표시

커서가 "개체명.속성명="의 우측에 위치가 맞춰져 있을 때

을          8 가능한 상수 목록을 표시한다. 또 신규 입력 때는 “="까지 입
력하면 자동 표시된다. 예를 들어 다음과 같이 입력하면 자동으로 구성원 자동 목록(참, 거짓)

command1.visible =

ole! 적은 창이 자동으로 나타나는 Zl "과잉 BaF Olek 느낄 때어는 [도구1-[옵센(0)|-[편짐[-
[코드 설정]-[! :구성원 자동 목록(Ｌ)]을 표시하면 기능이 정지한다. 이때도 수동으로 작은 창 표시는 행
해진다.

91


===== PAGE 92 =====
Chapter 3 Visual Basic 의 기본 조작

까지 입력하면 이 작은 창이 나타난다
00008001,

Top
로 UseMaskColor
e@ Value
때 Visible
es Whats ThisHelpID
eS! Width
=@ ZOrder

목록에서 선택한 내용이 삽입된다

00008001.\1610616

"=”까지|입력하면 이 작은 창이 나타난다
Command! Visible =|    [

|      7 목록에서 선택한 False 가 삽입되다

00008001.\151016 = False

에 AMS 맞춰

수정할 때는 “"의 우측
론 메뉴 선택도 좋다)

의
)를 느르  =
Command! Visible = False _   Ci) +) re 누른다(물론
이 작은 창이 나타난다

[ams

es Top

eg UseMaskColor
00! Value

fey   만   19081010 |
es W

= ZOrder

| "-:"의 우측에 AMS 맞춰 800+6800+미를 누르면
Command!.¥isible =
calle

이 작은 창이 나타난다

> -

구성원 자동 목록인 작은 창에서 세로 스크롤 바를 사용해 원
활용 방법이 아니다. 만약 구성원 자동 목록의 첫 문자 정도는 알
한 것처럼 해 보는 것도 좋은 방법이 된다.

00) “000084001.”까지 입력한다 ->작은 창 표시

@ "라고 입력한다 — ”'로부터 시작하는 첫 구성원 자동 목록이 표시된다.
(8) 라고 입력한다 — “visible”o] 반전 표시된다

@ fablS 누른다 — 항목이 삽입되고 작은 Ae 사라진다.

92


===== PAGE 93 =====
3.5 애플리케이션의 조작 순서

어느 첫 문자를 입력했을 때 해당 항목이 정확하게 표시되는 것은 유사 항목이 몇 개 있느
냐에 따라 달라진다. Visual Basic 속성 이름 SS 긴 것이 많기 때문에 “Al 문자를 입력해
나가다가 곧 정확한 구성원 자동 목록이 표시되면 098을 누른다.”라고 기억해 두면 좋다.

요약 정보 표시

개체 속성과 변수 등에 대해 간단한 문법 설명

해 준다. 예를 들면

ttlo

dt = Asc(ss)
에서 '& 에 커서를 위치시키고
[편집(ㅁ)]-[요약 정보(3)]((여0+00)
라는 메뉴를 선택하면
Asc(String As String)As Integer

라고 표시된다. 또, “88 에 AAS 위치시켰을 때 “Local ss As String” 이라고 표시된다. 자
동 요약 표시에서는 “dt=Asc(ss)"S 입력할 예정으로

dt=asc (

까지 입력하면 아래와 같이 그 문법이 표시된다.

Asc(String As String)As Integer

2) 매개 변수 정보의 표시 _

함수에 Bae 인수 = 인수 Aue 표시해 준다. 예를 들면

Dim ss As String,dt As Integer
dt=Val (ss)

라고 기술되어 있을 때 괄호 안의 “ss” ol] AAS 위치시키고
[편집(6)]-[매개 변수 정보(\/)]((여0+6001+ㅁ10)

를 선택하면 다음과 같이 표시된다.

93


===== PAGE 94 =====
94

Chapter 3 Visual Basic 2| 기본

조작

Val(String As String)As Double

요약 정보와 매개 변수 정보는 표시 기능이 같기 때문에 SHO] Awel7| 쉽다.

커서가 지시하고 있을

쓰크
요약 정보
매개 변수 정보

크
ak

단어의 문법을 표시

단어를 열 때까지 인수라고 보

때 다음과 같은 차이가 있다.

위에서 보여준 차이는 다음 예에서 명확히 알 수 있다

|

Asc(Mid(ss, 2)

Asc( String As String) As \nteger |

Asc =

Asc(Mid(ss, 2))

EH
[= |

[매2

10
뻐
쓰

Mid( String, Start As Long. (Length) |

“MO AMS 맞춘다
7019 를

re
+
on
bs
Hu
이

표시
함수

Mid’ 를
표시한다



===== PAGE 95 =====
단어를    끝까지 모를 때 준비되어 있 있는 29] 워드 중 올바른 단어를 표시해 준다. 예를 들면,
“BorderStyle”°|@#}= 단어를 모를 때에는 "60"까지 입력해서

[편집(6)]-[단어 채우기(\/)]([더01+ 6999)

를 선택(실제로는 Ctrl+Space7} 편리)하면 “60 "로 시작하는 단어가 나타난다. 원하는 항목
을 더블 클릭하여 선택할 수 있다. 스펠링이 하나밖에 없을 때에는 그 단어가 커서 위치에 들

ru

를 누르면 화면에는 “Caption” 2 Hpac}, 단어 채우기의 편리한 점은
텍스트로서 처리되는 것으로 만약 문법이 4S) 때에는 앞에서 설명한 요
하므로 걱정할 필요가 없다. 그러나 이 기능은 아래와 같이 문법과는 관계 없이 사용할 수
있어서 편리하다.

이

5

ss="BorderStyle 의 사용 예"

ack 프로그램을 작성하다보면 시행 착오로 어떤 복수 행을 일시적으로 주석을 달고 싶
은 경우가 있다. 불필요한 행이라고 인정되면 그 행을 삭제하면 좋겠지만 확실치 않을 때에는
우선 주석을 달아두었다가 MSS 조사해 보는 경우라든지 고생해서 작성한 프로그램 부분이
므로 삭제해 버리기에는 어딘가 재이용의 가능성이 있을 것 같아 주석으로 설정해서 그 소스

행의 보존을 하고 싶은 때도 있다.

Visual Basic Ht: 이와 같은 작업을 간단히 행하기 위해 지정 행을 한번에 주석으로 만들
어 주는 기능이 있다(그림 3-22), 이 조작을 하는 경우에는 책갈피 기능을 사용하는 때와 마
찬가지로

[보기(/)]-[도구 모음(1)]-[편집]

에 /표시ㅎ

음을 나타내 보자.

1
UH

95


===== PAGE 96 =====
96

Chapter 3 Visual Basic 2| 기본 조작

Private Sub Command1_Cl ick()
Static Stweh

Stwch = Not Stwch
14 Sub

Private Sub Command2_C1ick()
End
End Sub

Private Sub Command!_Click( )
Static Stweh
Static Ta
lf Stwch = False Then
Tm = Timer
Text!.Text = “BMA 3"

se
Text!.Text = Timer - Tm &@ “A 겸과“
End If

Stwch = Not Stweh

Sub

End

이 ㅣ | Sana nn is” 로 보오 이 로 eas ag aa

|
dt
0

[      = 설정] HES 2회 사용하면 이중 주석 마크7
반대로 [주석 블록 해제] HES 누르면 마크가 한 개씩
은 [이미 주석 행이다]라는 것과 그렇지 않은 HS 통째
는 조작을 가능하게 한다.

 63 이것을 클릭하면 각 행의 좌측
끝에 주석 마크가 자동으로 설정
된다. 한번 더 선택하여 이것을
클릭하면 이중 주석 행이 된다

2 Se ee      — © 원하는 행을 반전 표시시킨

주지도 ee           후 클릭하면 좌측 끝 주석 마
분에서 세로로 드래그)                  | 삭제된

ommandBut.

Pia  Cn a

ts



===== PAGE 97 =====
3.6 애플리케이션의 실행과 디버그

작성한 프로그램을 실행하여 바르게 작동하는지를 판단해야 한다. 그 확인 작업을 쉽게 하
기 위하여 Visual Basic ol] 충분히 익숙해질 필요가 있다. 따라서 지금부터 실행 방법과 여러
가지 디버그 기능에 대해서 알아보자.

애플리케이션의 실행

작성한 애플리케이션을 실행할 때 다음과 같이 조작한다(그림 3-23).

프로그램 실행 시

방법1 : [실행02)]-[시작(9)]을 클
방법2 : 를
방법3 : 9S 클릭
프로그램 중단(일시 정지)
방법1 : [실행(8)]-[중단(<)]을 클릭
방법2 : (Ctri}+ Break 를 누른다
방법3 : PS 클릭
일시 정지한 프로그램에서 재실행
방법1 : [실행08)]-[계속(2)]을 클릭
방법2 : 5 를 누른다([시작]과 겸용)
방법3 : BS 클릭([시작]과 겸용)
중단된 en 처음부터 실행
방법1 : [실행08)]-[다시 ASRS 클
빙법2: ae 누른
프로그램 종료
방법1 : [실행08)]-[종료(0)]을 클릭
방법2 : is 클
방법 3 : 프로그램 자제의 종료 PHS 사용

97


===== PAGE 98 =====
98

Chapter 3 Visual Basic 의 기본

i

@ 일시 정지할 때에는 이것을 클릭한다

@ 실행을 종료시킬 때는 이것을 클릭한다
|

애플리케이션에 종료 버튼이 아직 설정
되어 있지 않아도 디버그 중이리면 여기

를 클릭하면 멈춘다

VK Oe

Private Sub Command1_Click()

Static Stwch

Static Tm

If Stwch = False Then
Tm = Timer        ：
Text!.Text = “373 jem

Private Sub Command2_Cl ick
End
End Sub

© 이 #2 디버그용 ㄴ- @ 이 버튼을 클릭
조작에 사용한다

el

|면 프로그램이 작동한다

순자 컴파일과 완전 컴파일

작은 프로그램의 경우 시작 버튼을 클릭하면 곧 실행하는 것처럼 보이지만 실은 Visual
Basic 프로그램은 보이지 않은 Loy 다음과 같은 처리를 하고 <

|  프로그램을 컴파일 |

|      프로그램을 실행      |



===== PAGE 99 =====
3.6 애플리케이션의 실행과 디버그

이처럼 보이지 않게 프로그램을 컴파일하여 실행한다. 이 방식에서는 프로그램이 큰 경우
시작 버튼을 눌렀을 때 컴파일 완료까지 잠시 기다려야 하는 결점이 있다. 이것을 피하기 위
해 Visual Basic HAE 순차 컴파일이라는 방법이 있다. 이것은

[도구(1)]-[옵션(0)]-[일반]-[컴파일]-[| 」요청할 때 컴파일(ㅁ)]

에 \/ 표시의 유무로 알 수 있다(없앨 수도 있다). 순차 컴파일은 필요에 따라 부분적인 컴파
일을 한다. 따라서 아무리 큰 프로그램이라도 먼저 최소한 필요한 부분만 컴파일해서 곧 실행
시킨다. 보통

[도구(1)]-[옵션(0)]-[일반]-[컴파일]-[| |백그라운드 컴파일(<)]

에도 V EAR 설정해 두면 개발 환경에서의 빈 시간(사용자가 키 입력 등의 작업을 완전히
행하고 있지 않은 때 BS 사용해서 컴파일된다. 이와 같은 고도의 처리가 이루어지기 위해
보통은 사용자가 컴파일 갖고서 초조해 하는 일은 없다.

그러나 프로그램에 의해서(01. 서버 작성 등) 순차 컴파일에서 바르게 작동하지 않는 일
도 있다. 그때는 위의 v 표시를 빼고

[실행(『)]-[전체 컴파일 후 시작(『「)] ([여1+티 )

메뉴를 사용해서 실행을 시작한다. 후자는 일시적으로 완전 컴파일을 행한다.

Ea 디버그융의 화면 설

작성한 프로그램을 디버그하였을 때 화면 구성을 약간 변형하는 것이 편리하다. Visual
Basic 환경을 화면 가득히 해 두면 아래와 같이 잘못된 결과가 나타난다.
0 정지하면
@ 코드 에디터가 표시된다. 그러면
@ 폼 화면이 뒤에 숨겨져 보이지 않게 된다

폼 화면과 코드 에디터를 동시에 표시시키는 것은 시행 착오를 계산하여 Visual Basic 환
경을 작게 설정해 둔다(그림 3-24).

99


===== PAGE 100 =====
Chapter 3 Visual Basic 의 기본 조작

[아바 el peeeeneleet ick()
tat

State tm
If Stych = = le Then
To
Text. tere = "BUNA
Else
Text!.Text © Timer - Ta 회"    초 경과"
End
Stwch = Not Stwch
00 Sub.

Private Sud Command2_Click()
0

pee SUA 자동적으로 사라진다

면포 개        MOOS

화면이 표시된다. 이것은 디버그용 창이며 사동으로 표시된다. 불필요한 때에
닫기 버튼을     전 재실행할 때에 [보기(/)|-[직접 실
AMICCMHE)S 선택한다

og!

100


===== PAGE 101 =====
3.6 야플리케이션의 실행과 디버그

. 실행 시작한 프로그램은 다음 방법으로 중단시킬 수 있다. 중단 코드가 들어갈 때는 변수의
값을 표시하는 등의 디버그 조작을 할 수 있다

am
se

OF OF of oF Of 0
따 th of Ge of of

: 프로그램 안에 Stop HS 넣는다
: 중단점을 설정한다

: 조사식을 설정한다

: [실행 e200) 을 클릭한다
: (Ctrl) + Break 를 누른

: 에러가 발생할 때,

oOo = 0 NM —

특정 행에서 정지시켜 자세한 BES 얻고 싶을 때에는 방법1이나 빙
a =e 서 ere 싶을 때에는   방법 8을 사용한다. 방법 4와 방법

시지가 표시되면서 자동으로 정지된다
일단 중단한 프로그램에 대해서 새로운 중단점 SS 설정하여 다시 연속 실행시키고 싶을
때에는 다음과 같이 하면 재개된다.

프로그램 계속 실행

방법1 ㅣ Eo 크크

ow   .       cee
방법2 : 를 누른
방범 3 : [실행02)]-[계속(0)]을 클릭

또 지금까지의 실행 과정을 무시하고 ASHE] 실행하고 싶을 때에는 다음과 같이 조작한
다. 물론 종료하고 다시 시작해도 상관없다.

시작02)}을 클릭

101


===== PAGE 102 =====
Chapter 3 Visual Basic 2| 기본 조작

Stop 문으로 정지하기

임의 행에서 정지하기 위한 가장 알기 쉬운 HHS 그 행에 Stop ES 입력하는 것이다. 여
기에서는 예제로서 그림 3-25 프로그램을 제시해 보았다.

Private Sub Command1_Click()
Dim D As Integer, Wk As Integer
Dim Mul As Integer, Add As Integer
Mul = 1: Add = 0
For D = 1 To 5
Add = Add + D
Mul = Mul * D

Wk = D * 10
Wk = D * 100
Wk = D * 1000
Stop            여기서 Stop
Next
Textl.Text = 회 & Add & “44=" & Mul
End Sub

이 프로그램을 실행하면 프로그램은 정지하고 그림 3-269] 직접 실행 창이 나타난다. 직
접 실행 Abo AE Print S 사용함으로써 변수의 값을 HAS 수 있다.
또한 Print = 간단하고 손쉽게 기술하는 “? 도 사용할 수 있다.

여기에서는 간단한 Stop BS 사용했지만,

If D = 3 Then Stop           ‘D7t 3 이라면 Stop

102


===== PAGE 103 =====
3.6 애플리케이션의 실행과 디버그

® 정지한 위치에 화살표와 노란샌 반전이 표시된다

| Private Sub Commandt_Click()
주     010 D As Integer, Wk As Integer
Dim Mul A jatesers Add As Integer

10
'여기서 Stop
“St=" & Add 8 "책=" & Mul

Next
Text!.Text =
End Sub

Private Sub Command2_Cl ick( )
End

End Sub

Print Hd 2| 값 값을 표시해라
"adh vk @— HHA add of wk l 값 HS 표시해라
       OE 프린트와 같은 기능.

임의의 행에 중단점을 설정하면 stop 문과 같이 정지시킬 수 있다(그림 3-27). 특정 행에서 여러
정지하며 디버그 할 때에는 stop 문이 편리하지만 Ee 여기까지 실행시켜. 보자"라는 것처
럼 순서를 일시 정지시켜서 디버그를 할 때에는 중단점의 사용이 편리하다. 중단점은 실행 전 혹은
중단 모드에 있는 코드 에디터에서 다음처럼 설정한다. 중단점의 설정은 방법 30] 훨씬 편리하다.

[또

벼
tt

방법1 : 임의 행에 ANS 놓고 WS 누르면 설정되어 반전 표시로
한번 더 BS 누루면 제거된다.

방법2 : [디버그2)]-[중단점 설정/해제(1)]를 사용한다.
[디버그 도구 모음]의 해당 아이콘도 좋다.

방법 3 : 코드 에디터의 좌측 여백을 클릭하면 설정/해제가 된다.
이 방법이 간단하다.

중단점 전체 해제
[디버그2)]-[모든 중단점 지우기(2)]((여0|+600+09])로 전체 해제가 된다.

103


===== PAGE 104 =====
Chapter 3 Visual Basic 2| 기본 조작

Private Sub Command! Click()

Dim 0 As Integer, Wk As Integer

Dim Mul As Integer, Add As Integer

Mul = 1; Add = 0

For 0 = 1 105
=

Mul

Wk = D * 1000

Next
Text!.Text = “St=" & Add & 7책=" & Mul
End Sub.

Private Sub Command2_Cl ick()
n
End Sub

Ad
정된 중단점에서 프로그램이

(2) 실행중에 설
중단되고 | 화살표가 나타나며 코드        이것을 클릭하면 이 작은
가 노란색으로 반전되어 나타난다              창은 닫을 수 있다
[보기(/)]-[지역 SSIS 선택해서 AIS SS 표시하고 있다.
|   현재 유효한 변수값이 자동 표시된다(다음에 설명)

 디버그용 윈도우의 여러 가지 종류

Visual Basic2 효과적인 디버그를 위하여 다음의 AS 준비해 두고 [보기(\)] 메뉴에서
표시할 수 있다. 그 동안 직접 실행 창과 지역 창은 앞에서 그림으로 보여 주었지만 조사식 창
에 대해서는 다음에서 알아보도록 하자. 각각의 AS 닫는 방법으로는 창의 상단 오른쪽에 있
는 닫기 버튼을 클릭하면 된다.

직접  실행  차
Oo

사용자가 키 입력하는 것에 의해 변수의 값 표시/설정 SS 한다. 또한 뒤에서 익힐
Debug.Print 문의 출력이 나타난
지역 창

현재 액티브 프로시저 내에서 사용되고 있는 변수값 등을 (사용자가 지정할 필요 없
이) 자동으로 표시한다.

104


===== PAGE 105 =====
3.6 애플리케이션의 실행과 디버그

차
=
조사식으로 지정한 변수값을 표시하는 창이다.

| . 조사식에서 잠조와 중단하기

중단할 때마다 Print 문을 입력하는 것은 의외로 귀찮다. 바로 이러한 때 조사식을 사용하
면, 중단할 때마다 어떤 변수 값이 자동으로 표시되어 편리하다.
조사식은 다음 3종류로 설정할 수 있다.

)

이라면 중단하라(예 : D=4)

중단하라(예 : aa

설정2와 설정3은 ZAR] 자체가 중단 처리를 하며 설정1은 몇 개의 별도 원인으로 중단
되었을 때 이에 대한 식의 값도 자동으로 표시하라고 지정한다. 조사식을 설정할 때에는 다음
과 같이 한다.
[디버그(20)]-[조사식 7K A)]

새로운 식을 설정한다. 두 개의 AS 설정할 때에는 이 메뉴를 2회 지정한다.

[디버그 (0)]-[조사식 편집(ㄷ)](801+0)
eo] 끝난 조사식을 변경한다. 표시되어 있는 조사식 창에서 변경하고 싶은 ge 마우스로 클
릭하여 반전행이 되면 이 메뉴를 선택한다.

[디버그(2)]-[간략한 2A}4|(Q)] (Chit +)
반전으로 선택된 변수와 속성의 값을 표시한다

Delete

입력을 마친 조사식을 삭제한다. 표시되어 있는 ZAM) 창에서 식을 마우스로 클릭해서 6008를
누르면 삭제된다(그림 3-28 조사식의 사용-1).

nh

번

A] 창에서 마우스 오른쪽 HES 클릭하면 추가/편집/삭제 등의 바로 가기 메뉴가 표시되어 메뉴 선택을
할 수 있어 편리하다.

k

조사식 설정은 코드 에디터 상에서 조사하고 싶은 변수에 커서를 맞추고 메뉴를 선택하기만 하면 된

근 ATL

다(그림 3-28). 다음 그림은 조사식을 설정한 예로 실행 결과는 다음에서 다룰 예정이다.

105


===== PAGE 106 =====
Chapter 3 Visual Basic 의 기본 조작

화면1 조사식의 설정
0) 변수 Muldl| AMS 맞춰 둔다

For 0 = 1 105
Add = Add + D
Mul = Mul + 0

Wk = D + 1000
Next
Text!,Text = “St=" @ Add
Sub,

End

Private Sub Command2_Cl ick( )
ni
End Sub

@ 이 메뉴를

(1) 같은 모양으로 변수ㅁ에 커서를
마츠

맞춰서 메뉴를 선택. 이 BPE ㅁ
만 자동으로 설정되기 때문에

을    . 이 SRE "DAI 값이 4가
된다면 중단하라 는 것이대

106


===== PAGE 107 =====
3.6 애플리케이션의 실행과 디버그

직접 실행 창의 구성은 앞에서 AVM 조사식을 ABS 그림 3-292 알아보도록 하자.

Private Sub Command!_Click()
Dim 0 As Integer, Wk As Integer
Dim Mul As Integer, Add As Integer
Mul = 1: Add = 0
For D= 1 105

Add = Add + 0
Mul = Mul + 0
Wk = 0 + 10
Wk = D+ 100
Wk = D+ 1000

Next
Text!.Text = "St=" 8 Add & "책=" & Mul
End Sub

Private Sub Command2_Cl ick()
End
End Sub

현재 값이 표시된다

변수 형태가
표서된다
a dq} mul
4 6

Boolean           ‘orm, Command!
Integer           Form 1,Command1!_C

변수의 프로시저명이 표시된다. 이하의 표시는
"Form1,Commandt_ Click’ 이라고 되어 있다
(1) 자동으로 조사식 창이 표시된다
L_ (3) 참으로 되어 있기 때문에 이 D=42h=
조건으로 중단한 것을 알 수 있다
L_ @ 이미 변수 MulZto] 표시되어 있다
L_ © 여기를 좌우로 드래그하면 2개의 A 비율을 변경할 수 있다
ㄴ 66) 스스로 변수0와 MulS 표시하여 보았다.

절히 여기저기의 변수(식) 값을 알고 싶을 때에는 그림 3-30 처럼 조작하는 인
하다. HE 변수 이름 위에 마우스 버튼을 설치해도 변수값을 표시할 수 있다.

107


===== PAGE 108 =====
  Chapter 3 Visual Basic 2| 기본 조작

화면1 간략한 조사식의 사용

@ 이 '400"에 커서를 맞

Hy!
므

Private Sub Command! _Click()
Dim D As Integer, Wk As Integer
Dim Mul As Integer, Add As Integer |
Mul = 1: Add = 0
For O= 1 10 5
Add = Add + D
Mul = Mul + 0
Wk =O * 10
Wk = 0 + 100
Wk = D + 1000

Next                      ~
Wiilexti.Text = "t=" & Add & “4=" &
End. Sub

Private Sub Command2_Ci ick( )

ni
End Sub

(01) 이 중단점으로 중단시켰다

® 값이 표시된다
화면2 마우스 HES “Add © 필요하면 이것을 클릭하면 조사식으로
위에 위치시켰다         서 미리 등장되기 때문에 편리

Private Sub Command1_Click( )             >)
Dim 0 As Integer, Wk As Integer
Dim Mul As Integer, Add As Integer
Mul = 1: Add = 0

For D=105
Add = 200 + 0
Mul [Add = 15] 0
Wk = 0 * 10

Wk = 0 * 100
Wk = D + 1000
Next
ar : oe = “St=" & Add & “4{=" & Mul
nd Su
ss                                    ee

.Print 를 사용

다이나믹한 변수 값을 알고 싶을 때에는 Debug. Print 7} 편리하다(그림 3-31)
임의의 위치에 아래의 USS 입력하면 그 변수값이 실행되어 창에 표시된다.

Debug.Print Add

108


===== PAGE 109 =====
3.6 애플리케이션의 실행과 디버그

이때 프로그램은 멈추지 않고 실행된다. 잘 사용하면 어떤 변수값의 변화 과정이 표시될 수
있기 때문에 디버그 정보 수집으로서 대단히 유용하여 전문가가 좋아하는 기능이다. 간단히

Print Add

라고 입력하였을 때에는 보통 기본이 되는 폼 상에 (쓰레기처럼) 표시된다. Visual Basic ol
서는 직접 실행 창에 표시된다.

화면1
© 이곳에 입력하였다. 어차피 디버그용이므로 눈에 띄도록 쓰면 좋다

Private Sub 000060012011하()
010 0 As Integer, Wk As Integer
Qim Mul As Integer, Add As Integer
Mul = 1: Add = 0
For D = 1 To

5
Add = Add + 0
Debue.Print “eager? hdd  — fy 22

Wk = D + 100
¥k = D + 1000

Next
Text!.Text = “St=" & Add & "책=" & Mul
End Sub.

Private Sub Command2_C1! ick( )
미
End Sub

1 00 에베 as i ha i Mi i se i 으

Ea 단계별 실행

프로그램을 한 행씩 정지시키고 실행할 때에는 단계별로 실행해 나간다.

한 단계씩 실행
[디버그02)1-[한 단계씩 코드 실행0)]08)을 클릭한다

프로시저 단위 실행
[디버그(2)]-[프로시저 단위 실행(2)](@008+8)을 클릭한다.

109


===== PAGE 110 =====
Chapter 3 Visual Basic 의 기본 조작

프로시저 나가기
[디버그(2)]-[프로시저 나가기()]([더1+0때+ )을 조작한다.

프로시저 나가기는 중간에 실행 중인 프로시저가 있으면 프로시저를 최후까지 한번에 실행해서 불러내
고 원래대로 돌아간다. 한 단계씩 실행과 프로시저 단위 실행은 프로시저 호출하기가 있었다면 동작이 달
라진다. 프로시저 불러내기가 없다면 어느쪽이라도 같은 동작이다. TA 3-329] 예를 보도록 하자.

60090 214 등지의 성덩응 리스

1 Private Sub Command1_Click()

2      Dim D1 As Integer, D2 As Integer

3     Debug.Print "Start"

4     21 = 100

5     D2 = 200

6     Dout Dl, D2              '이하의 프로시저 Dout 호출하기
7      Print “End"

8 End Sub

9 Private Sub Dout(A As Integer, B As Integer)

10     Debug.Print A+B
a1     Debug.Print A - B
12     Debug.Print A * B
13 Debug Print A /ㅁ
14 End Sub

[}거하거사거하거아거아게아게 }게가게하게사거7}8|

프로시저 단위로 실행의 흐름
LW 의 의

| (Py 임의의 행부터 실행

단계별 실행은 한 행씩 처리를 해 나가지만 때로는 전혀 다른 행을 단계별로 실행 확인을
하고 싶을 때가 있다. 그런 경우에는 다음처럼 한다.
다음에 실행할 행을 설정하다

O 다음에 실행시키고 싶은 행에 AAS 맞춘다.

@ [디버그02)1-[다음 문 설정0)](601+89)을 선택한다.

110


===== PAGE 111 =====
3.6 애플리케이션의 실행과 디버그

예를 들면 단계별로 실행하고 있어서 현재 19행을 나타내는 화살표가 있다고 하고 여기에
서 28 번째에 AAS 두고 [여0|+[9 를 누르면 28행을 실행하기 위한 표준 완료가 된다. 이후
언제나 한 단계씩 실행과 프로시저 bile 실행 지시를 한다. 이렇게 하면 12~27행은 실행되

지 않는 것에 주의해야 한다. 이 기능은 프로그램 흐름을 볼 수 없다.
임의의 행부터 실행은 “어떤 프로그램 부분이 기능을 집중적으로 테스트한다' 라는 목적으

로 사용한다. 12~87행도 실행해서 28행으로 나아가고 싶을 때에는 다음 기능을 사용한다

임의의 행까지 실행

중에 있는 행까지는 한번에 처리를 진행하고 싶다고 1000번을 반복하는 루
면 빠져 나올 수 없는 일이 생기고 만다. 이런 때에는 다음처럼 하면

임의의 행까지 한번에 실행한다
@ 처리를    은 마지막 행에 커서를 위치시킨다.
@ [디버그(0)1-[커서까지 실행0)] (00+8)을 선택한다.

커서 ANE 실행 이전으로 되돌리기

단계별로 실행 중인 상태에서 다른 부분의 SES 확인하기 위하여 화면을 스크롤하게 되
면 단계별로 실행 중에 있던 행으로 되돌리기 어렵게 된다. 이런 경우는 다음 방법으로 간단

히 커서를 되돌릴 수 있다.

단계별 실행 자 eee

a 호출 스택 보기

어떤 프로시저가 실행되고 있을 때 어디서부터 호출되어 졌는가를 확인하고자 할 때 호출
택

111


===== PAGE 112 =====
Chapter 3 Visual ㅁ2610의 기본 조작

Private Sub Command1_Click()
SubPrg1
End Sub                            이것을 불러낸다

Private Sub SubPrgl1() <—_]
SubPrg2        BP Se aap see
End Sub                           더불어 이것을 불러낸다
Private Sub SubPrg2() 개]
Print "abc"
stop       <             여기에서 중단
End Sub

all

이 단계에서 중단했다

Private Sub Command!_Click()
SubPrg1

600 Sub
Private pus SubPrai()
Sub

14 6840
ae sp Perea
aly

End  ar

) 원하는 BRA
저를 선택하여
반전시켜 클릭
하면 그.프로
시저의 코드
화면으로 옮긴
다(프로시저명
Project! Form! Command! Click                      을 더블 클릭
해도 좋다)

= Commandi_Click()O|Ct
arya                 |

112


===== PAGE 113 =====
3.6 애플리케이션의 실행과 디버그

a 실행 파일 작성과 실행

동작이 올바르게 확인된 프로그램은 컴파일해서 실행 파일을 작성한다. 일단 실행 파일을

만들면 SAE Visual 88810을 실행하지 않아도 윈도우 상의 보통 애플리케이션과 같
은 방법으로 실행할 수 있다.

실행 파일을 작성하다
[파일)]-[ㅁ70)1601.686만들기(《)]를 선택해서 실행 파일명을 ¢

ro,
1.
후

더.

“Project.exe’ 의 부분에는 그때 작성하고 있는 프로젝트 파일명이 들어간다. 보통은 이 조작
만으로도 상관없지만 본격적인 프로그램을  an 때에는 버전    | us 들어가게 할 수도 있다.
여기에서는 전에 보여 줬던 스탑워치 프로그램을 컴파일 해 보자(그림 3-34).

a

필요로 한다. 그러나 프로그램을 개발한 사람은 자기 컴퓨터로 실행할 때 자동으로 설정되어 있기 때문에
이상없이 실행할 수 있다. 상대가 같은 Visual Basic 개발 환경을 인스톨하고 있을 때에는 실행 파일만
을 건네면 좋다. 그렇지 않을 때에는 실행 파일에 첨가하여 필요한 라이브러리를 배포할 필요가 있다. 이
처리를 적절히 행하기 위해서 Visual Basicdll= 셋업 프로그램(배포용 디스크)을 작성하는 기능(애플리
케이션. 셋업. 위저드)이 준비되어 있다.

Al  사실 여기서 작성한 실행 파일만으로는 실행할 수 없다. 실행에는 런 타임 라이브러리라는 별개의 파일을
NOTE

화면1 실행 파일 작성

113



===== PAGE 114 =====
114

Chapter 3 Visual ㅁ2510의 기본 조작

정보에서 버전 탭을 클릭하면 볼 수
해 보았다

있다. 예로서
'\/6「1,2.3을 지정

을 넣어 보았다. 표준은
Stwch7} SQ7} 있으므로, 그
대로 해도 좋다

미세 때때           (3) 이것을 클릭하면
컴파일 시작
@ Sse 지정하고 싶을
때에는 여기를 클릭
 작성하고 싶은 실행 파일명을 입력한다
화면 3 [프로젝트(2)]-[프로젝트 SAE] 메뉴로 SAS 지정하다
버전 HSS 지정한다. 이 정보는 실행 파일의 등록 제품명을 넣는다. 예로서 이름

파일명

애플리케이션 아이콘을 지
정한다. 단순한 프로그램은
『0071밖에 없다. 복수의
폼을 이용하는 프로그램의
경우 어느 폼의 아이콘을
EXEMS 아이콘(그 애플
리케이션의 얼굴이 되는 Of

이콘)으로 할지 선택한다:
=                             2S 기술한다 eA
Ol 섬며을 |    았다 ALB
XE URIs 작성할 때마다 리배전 es          고사 아오 이시기



===== PAGE 115 =====
3.6 애플리케이션의 실행과 디버그

99-06-27 오후

98-06-25 오전
98-06-24 오전 12
98-07-22 오전 12,

(1) 윈도우 탐색기에서 Stwch.exe
를 마우스의 우측 버튼을 클릭

해서 [등록 정보]를 선택한다

@ 버

[것
[쪼
[10
eed
모
[에
다

=]
on

@ 설정한 내용이
표시되어 있다

Ouolur Amo

115


===== PAGE 116 =====
Chapter 3 Visual Basic2| 기본 조작

Visual 28810에서는 작성한 애플리케이션은 프로젝트라는 단위로 관리한다. 하나의 프로젝
트가 하나의 애플리케이션을 표현한다. 여기에서는 프로젝트의 구성과 그것을 취급하는 방법,
사용자 정의 컨트롤의 추가 BAT Visual Basic 환경의 변경 방법에 대해서 살펴보도록 하자.

| (py 프로젝트의 구성

프로젝트 파일에는 사용하고 있는 파일 이름과 개체의 보기 그리고 환경에 관한 정보가 포
함된다. 프로젝트 파일은 단순한 텍스트 파일이다. 참고로 Stwch.vbp 파일 내용을 그림 3-
835에 제시했다.

속성의 본체 부분은 보통 frm 파일에 보관된다. 작은 애플리케이션은 frm 파일만으로 7

술할 수 있다. ESS 위해 Stweh.frm 파일을 그림 3-36에 제시했다.

코드 창의 리스트 박스 중에서

(General)

Command1l

Textl
과 같이 코드를 입력하는 개체를 선택하였고 이것은 편집 작업의 편의를 위하여 저장하였지
만 결국 같은 곳에 입력되었다는 ASS 수 있다. 또한 속성 AA 설정한 내용도
Stweh.frmF 기록되어 있는 것을 알 수 있다. 즉 속성 AS 이용하여 SYS 설정해도 코드
로 속성을 설정한 것과 같은 것으로 이해하면 쉽다.

116


===== PAGE 117 =====
3.7 DEAE} 환경 관리

Form=stop. frm

Reference=*\G{00020430-0000-0000-c000-000000000046}
#2. O#0#..\..\..\WINDOWS\SYSTEM\STDOLE2.T? LB#OLE Automation

IconForm="Form1"

Startup="Form1"

HelpFile=""

Title="ABAUz|"

ExeName32="stwch. exe"

Command32=""

Name="Project1"

HelpContextID="0"

CompatibleMode="0"

MajorVer=1

MinorVer=2

RevisionVer=4

AutoIncrementVer=1

ServerSupportFiles=0

VersionComments="A2|zx|"

VersionCompanyName=" 영진 "

VersionFileDescription="ZIHtSt 스톱워치"

76ㅁ8101106092107806081166=" 스톱워치"

CompilationType=0

OptimizationType=0

FavorPentiumPro (tm) =0

CodeViewDebugInfo=0

NoAliasing=0

BoundsCheck=0

OverflowCheck=0

F1PointCheck=0

FDIVCheck=0

UnroundedFP=0

StartMode=0

Unattended=0

Retained=0

ThreadPerObject=0

MaxNumberOfThreads=1

117


===== PAGE 118 =====
Chapter 3 Visual Basic2| 기본 조작

VERSION 5.00
Begin VB.Form Forml

Caption               =     "스톱워치"
ClientHeight    =   1455
ClientLeft      =   60
ClientTop       =   345
ClientWidth     =   4680
LinkTopic       =   "Form"
ScaleHeight     =   1455
ScaleWidth      =   4680
StartUpPosition = 3 (Windows 기본값)
Begin VB.CommandButton Command2
Caption         = 종료"
Height          =   375
Left            =   2520
TabIndex        =   2
Top             =   720
Width           = 1815
End
Begin VB.CommandButton Command1
Caption         =   "Start/Stop”
Height          =   375
Left            = 240
TabIndex        =   1
Top             =   720
Width           = i215
End
Begin VB.TextBox Textl
Height          =   375
Left            = 240
TabIndex        =   0
Text            =   "Text1i"
Top             =   240
Width           =   4095
End

End

Attribute VB_Name = "Forml1"
Attribute VB_GlobalNameSpace = False
Attribute VB_Creatable = False
Attribute VB _Predeclaredid = True

118


===== PAGE 119 =====
3.7 프로젝트와 환경 관리

Attribute VB_Exposed = False
Private Sub Command1_Click()
Static Stwch
Slatic IM
If Stwch = False Then
T™ = Timer
Text1.Text
Else
Text1.Text = Timer - T™ & " 경과"
End If
Stwch = Not Stwch
End Sub

"측정시작"

Private Sub Command2_Click()
End
End Sub

폼 2S( frm)
애플리케이션의 주체가 되는 것으로 폼 위에 배치한 컨트롤과 속성에 관한 정보 또는 이벤트 프
로시저 등 드 속성 본체가 포함된다.

표준 23( bas)

폼 모듈에 포함되지 않는 프로그램 코드가 들어오는 ALE 사용자 BAS, 정수, 변수, 제너럴
클래스모듈(.019)

독자적으로 AAS 작성할 때에 사용하는 BEE 스스로 코드를 기술한다. 성격은 폼과 같지만
화면에 표시되는 인터페이스는 같지 않다.

리소스 파일(.169)

프로그램 코드에 집어 넣지 않는 독립 데이터를 Vole 파일이다. 예를 들면 같은 동작으로
화면 표시만 다른 한글 버전과 영문 버전의 프로그램을 작성하는 경우 해당 문자열(일본어와 영

어)을 리소스 파일로 관리하면 야플리케이션 본체를 한 개로 할 수 있다.

준 컨트롤
Visual Basico] 표준으로 준비되어 있는 컨트롤이다. 이 컨트롤은 도구 상자 위에 항상 표시되
어 잃다:

119


===== PAGE 120 =====
Chapter 3 Visual Basic] 기본 조작

OLE 사용자 정의 컨트롤(.06×0의 삽입 가능한 개체
표준 컨트롤 이외의 특수한 컨트롤로 별개 파일로 제공된다. 서드 파티로부터 발매되는 일도 gl
다. OLE 사용자 정의 컨트롤(0030은 OLE 기술을 사용하는 컨트롤이다. 삽입 가능한 개체는
엑셀의 위크시트처럼 다른 애플리케이션으로부터 제공되는 개체이다. 이 HAL 도구 상자에
추가하거나 삭제할 수 있다.

VBX 사용자 정의 컨트롤(./6>)
OLE 사용자 정의 컨트롤과 같은 것이지만 16481 Basic] 16 비트로만 사용할 수 있다. 이전
의 Visual 88810으로 사용되고 있던 것이다.

14 3-372 Visual Basic 애플리케이션의 프로젝트 구성을 FSS 한 것이다.

설정
이벤트 프로시저 Cee rece eerevevece입력
LS 컨트롤 배지 we secede wee ane ses aw ssa eon배치
속성 Ce Cee se See er ……설정
이벤트 프로시저 ㆍ*…ㅇ…ㅇㄴㅇ …*입력
= 컨트롤ㅁ 배치………ㄴㅇㄴㄴㅇㄴㄴ,ㄴ,,ㄴㄴㄴ, ㄴ……ㄴㄴㄴ×ㄴㄴㄴㄴ…ㄴㄴㄴㄴㅇㅇ배치
속성 _ ×……ㄴ………………0……………………………*설정
|벤트 프로시저 ㆍ‥…ㅇㅁㄴㅇ입력
| 표준 모듈(.689)      ㅣ
제너럴 프로시서 ㅣ] *……ㅠㆍ …ㅇㅇㅇㅇ…ㅇㅇㄴ…ㅇㅇ ㅇㅇ입력

폼 모듈에 포함되지 않은 코드(변수형 지정 등). ‥…‥ㆍ입력

표준 He    A

AA I         일(.  res)              |  CSS CMOS K TNR ES ROE DRED필요하다면

에.

| OLE 87t 정의 HES ocx)2| 삽입 가능한 개체 ㅣㆍ‥…‥ 필요하다면
=  VBX4t 24 정의 AE S( vpx)       |해ㅎㅠㄴ<ㅜ~필요하다면

프로젝트 파일(./60)은 Visual Basic] 한참 이전(버전 4보다 이전)의 버전에서는 확장자가 .008(였지
“wote| 만 Make 파일의 흐름에 해당하는 것으로 새 버전에서는 사용하지 않는다.

120|


===== PAGE 121 =====
3.7 프로젝트와 환경 관리

한 개의 야플리케이션은 한 개의 프로젝트 파일을 갖고 있다. 애플리케이션을 작성하는 것
은 프로젝트 파일을 새로 작성하거나, 기존의 것을 읽거나(열기), 그것을 저장한다.

프로젝트 파일은

- 애플리케이션은 00라는 파일로 구성되어 있다.

는 정보를 갖거나 그 구체적인 프로그램 파일은 또 다른 방법으로 저장한다(다음 항). 프로
젝트를 불러오면 거기에 입력되어 있는 모든 파일이 준비된다.

현재 이름으로 프로젝트를 덮어 써서 보존하다.
[파일0)]-[프로젝트 저장(\/)]을 선택한다.

새로운 이름을    -_ 프로젝트를 저장한다.
[파일0"]-[프로젝트를 다른 이름으로 저장08)]을 선택한다.
py 파일을 주가/제거/보존
프로젝트로 지정된 파일(위에서 설명했던 frmy} basta 등)을 실제로 처리하며 이 파일
처리는 디스크 사이에서 읽혀진 것 이외의 처리 형태로서는
현재 프로젝트 파일에 추가(등록), 제거(삭제)할까

가 있다. 즉 제거라고 하여도 프로젝트 파일에 등록되어 있는 않은 상태로 제거하는 것은 디스크
에서 삭제되지 않는다.

때 현재 프로젝트 태 추가한다.
[파일(0)]-[프로젝트 추가()]를 선택한다.

121


===== PAGE 122 =====
Chapter 3 Visual Basic2| 기본 조작

프로젝트를 현재 프로젝트 그룹으로부터 제거한다.
[파일0)]-[프로젝트 AARIS 선택한다.

현재 이름으로 파일을 덮어 써서 보존한다.
[파일0")]-[7672001의 저장(8)]을 선택한다.

편집중인 파일의 선택 영역을 텍스트 파일로 저장한다.
[편집(01-[파일 삽입0.1을 Hea

Visual 88510은 작성하는 애플리케이션을 프로젝트 그룹이라는 단위로 관리한다. 초보자가 작성하는 프
Non| 로그램은 프로젝트 그룹 속에 프로젝트 파일이 한 개, 그 속에 B= 한 개로 구성되어 있는 것이 보통이다.
하지만 규모가 큰 애플리케이션에는 한 개의 프로젝트 파일 속에 폼을 복수로 넣어서 구성하는 일이 많다.

[oi 모듈의 신규 작성

내 모듈의 프로그램 작성 과정에서 자동으로 한 개(067201이라는 이름으로)가 준비된다.

작       Se 폼 모듈만으로 끝날 수도 있지만 필요에 따라 모듈이 많아질 수도 있다.
새로운 모듈이라면 다음의 방법으로 처리한다.
폼 DSS 현재의 프로젝트에 추가한다.

[프로젝트(2)]-[폼 추가0")]를 선택한다.

=
=]
oH
i
“4

_ ZEAE O 추가한다.
때 02    폼 추가(1)]를 선택한다.

표준 모듈을 현재의 재개 추가한다.
-[모듈 추가(1/)]를 선택한다.

ne
ish

o=
호
월
ae
2"

\r

om 4
in ©
SS
A,
1c,
(el
ffl
ie
of
띠ㅇ
-뿌
ox
ca
+>
yo
도

122|


===== PAGE 123 =====
3.7 프로젝트와 환경 관리

Visual 88800에서는 의외로 많은 사용자 정의 컨트롤이 준비되어 있다..그 컨트롤을 사용할 때
에는 목적의 컨트롤이 도구 상자에 표시되어 있는 상태가 되어야 한다. 그 조작은 다음과 같다.

사용자 정의 28 도구 상자에 추가한다.
[프로젝트00)]-[구성 요소(0)]를 클릭하면 다이어그램 박스가 표시된다.
[컨트롤] 탬 a 희망 컨트롤에 \표시한다.
확인 버튼을 클릭한다.

사용자 정의 HESS 도구 상자로부터 삭제한다.
[프로젝트(2)]-[구성 요소(0)]를 클릭한다.
상기의 추가와 같은 SNS 표시를 지우고 확인 HES 클릭하면 삭제된다.

화면1 리치 텍스트 박스를 추가한다                     화면2 도구 상자에 리치 텍스
(1) [프로젝트(2)]-[구성 요소(0)]를 클릭한다                 트 박스가 추가되었다

) Microsoft Hierarchical FlexGrid Control 6, a]
(| Microsoft HTML Object Library

(_] Microsoft Internet Controls

1 Microsoft NetShow Player

Co) Mi       Office Web Ci           9.0

(-] Microsoft Outlook Express 5,0 Type Libre *
(] Microsoft RemoteData Control 6,0         ||
vi

[] Microsoft Sysinfo Control 6,0

_ 1) Microsoft Tabbed Dialog Control 6,0
[Microsoft Windows Common Controls 5,
) Microsoft Windows Common Controls 6,
1 Microsoft Windows Common Controls-2

@ 이것을 클릭해서 표시를 한다

Visual 80510의 환경 옵션 설정

Visual Basic®| 프로그램 개발 환경에는 많은 옵션이 있다. 초보자는 이 옵션에 관해서 있는 그대
로 사용하는 것이 좋지만 숙달이 되면 옵션 설정을 하여 보다 쉬운 환경어서 프로그래밍할 수 있다.
옵션 설정은 [노구(1-[옵션(0)(에서 한다. 각 항목에 대해서는 그림 3-390] 잘 설명되어 있다.

123


===== PAGE 124 =====
124

_ 00803 Visual Basic] 기본 조작

화면1 [편집기] 탭

—— 코딩시 함수와 함수의 매개 정보를 표시한다

변수의 선언 없이 사용을 허락하지 않는다

een $ be =

프로시저간에 노란선을 넣어 알기 쉽게 한다
전체 프로그램을 보기 표시를 한다

코드 에디터에서 반전 표시한 텍스트를 드래
그 조작으로 이동할 수 있도록 한다

화면2 [편집기 형식] 탭
코드의 종류마다 컬러를 넣을 때 지정

나나

선택 영역의 색을 지정한다
문자의 색을 지정한다

박스에 나타난다

— 문을 완성하기 위해 을 찍으면 메소드/프로퍼티 등의 정보가 나타난다

코드를 한 행 삽입할 때마다 자동 구문 ASS 행한다

한 행의 글자 아래에 맞춰서
자동으로 들여쓰기 한다

탭의 간격을 설정

코드의 서체를 지정한다

코드의 서체 크기를 지정한다
좌측 끝에 책갈피와 중단
점을 표시하며 스페이스로
확보한다. 그것은 표시 없
이 하면 디버그가 불편하다

AS 끝에 표시되는 마크의

So (ee



===== PAGE 125 =====
3.7 MEMES} 환경 관리

화면3 [일반] 탭

— HES 배치를 그리드에 맞춘다
 그리드의 간격을 설정한다
폼 위에 그리드를 표시한다

프로젝트 탐색기에서 프로젝트를 닫았을 때에(프로젝트명의
좌측[-}을 클릭해서[+]로 한다) 이동해서 폼 창과 코드 에디
터도 닫을 것인가에 대해 지정

—— 도구 아이콘에 마우스 커서가 위치하면

나타나는 버튼 명 표시 기능을 설정

화면4 [도킹] 탭

 각각의 BS Visual Basic 환경의 본체 윈도우
와 일체화할 것인가에 대해 지정

예를 들면 [도구 상자]를 v 없이 하면 항상 독립
형 창이 되고 어디라도 배치할 수 있게 된다

ey
| 교
| 그
|:
ja

125



===== PAGE 126 =====
hapter 3 Visual Basic2| 기본 조작

화면5 [환경] 탭

 소스 프로그램에 수정을 가하고 프로그램 AHS 하였을 때 그 소스 프로그램의
저장 여부에 대해 먼저 지정한다.
그것은 실행할 때 과부하에 대한 AAS 안전하게 하는 의미가 있다. Visual Basic
을 실행할 때 오류에 대한 HAAS 표시하고 \/16481 Basic HSS 모두 강제 종료
시키면서 AA 프로그램이 버려지는 SPS 방지하는데 유익하다
—lAi 프로젝트]라는 창을 열지 않고 표준 EXES 작성하도록 한다
Visual 885616을 실행할 때 또는 [파일[-)]-[새 프로젝트()]를 선택할 때 [새 =
로젝트]라는 창을 열도록 지정하여 실행시에 [aoe 이 대화 SAS 표시 안
HUIS V 표시 했을 때 이곳을 설정하면 다시 표시하도록 한다
x

기존의 컴포넌트와 코드를 새로
운 프로젝트로 다시 이용할 수
있게 하기 위해서 [새 프로젝트]
라는 창에 표시시키는 정보를
지정한다. 이 BBS 아래의
특별 폴더에 보관하고 있다

[AH 프로젝트] 창에 표시한다. 이것을 끝내면 [AH 프로젝트] 화
면의 표시 HS 줄여서 기본적인 항목만이 된다

화면6 [고급] 탭

 엑셀 화면같이 한번에 복수 문서(스프레드 시트 등)를 열 수 있는 \/0(멀티 도큐먼트
인터페이식)가 아닌 62)(싱글 도큐먼트 인터페이스)용의 Visual Basic HBO 한다.
보통의 경우에는 VEE Bee 하지 않는다

 어떤 파일(예를 들면 frm)o| 몇 개의 프로젝트로 공유되고 있던 경우 그 파일 내용

을 변경할 때 영향을 주는 다른 프로젝트도 적절히 처리될지의 여부를 찾도록 한다

프로젝트의 로드를 백 그라운드로 행하고 최초의 화면을 가능한 빨리 표시하도록 한다
ad                                        지

~ HIMLZ©& 기술에 notepad,
ees 사용하도록 설정하고
있다

126


===== PAGE 127 =====
3.7 프로젝트와 환경 관리

작성이 끝난 어떤 프로그램을 복사해서 방법을 강구하고 새로운 프로그램을 만들고 싶을
경우 기존의 베이직 프로그램이라면

tstprgl.bas—tstprg2.bas

라고 복사하고 새로운 tstprg2 basehs 프로그램이 만들어지는 방법을 강구해 완전히 다
프로그램으로 발전시킬 수 있다

이와 같은 처리를 할 때 16081 828810에서 주의할 점이 있다. Visual 88810에서는 프로젝
트 파일이라는 소스 파일이 따로따로 관리된다는 점이다. 예를 들면 단순한 예로서 [3{0181
이라는 프로그램은 아래와 같이 구성된다.

(tu

tstprg1.vbp
tstprg1.frm

이 프로그램을 복사할 때에는 다음 조작이 필요하다

@ Visual 88810을 실행해서 tstprgl& 읽는다
® [파일0)]-[((6[0181.170을 다른 이름으로 저장]을 사용해서 tstprg2.frm& 만든다.
(3) [파일")]-[프로젝트를 다른 이름으로 저장]을 AVS} tstprg2. vbpS 만든다.

이처럼 .vbp 파일과 frm 파일을 모두 새로운 이름의 파일로 저장하는 것이 필요하다. 어
느쪽이든지 한쪽만 복사하는 것으로는 잘 될 수 없다. vbp 파일만 새로운 파일로 복사해도
시작한 이상은 바르게 동작하는 것처럼 보이나 다음 단계로 동작하는 것에 지나지 않는
올바른 복사 프로그램의 관계
독립한 두 개의 프로그램
         (catprai. fm)

Q2| 작업을 하지 않았던 복사 프로그램의 관계

tstprg1.vbp         tstprg1.frm]-::::-이 HAYS 공유하고 있다

tstprg2.vbp }       tstprg2.frm| ----:- 이 TAS 존재하지 않는다

127


===== PAGE 128 =====
Chapter 3 Visual Basic 2| 기본 조작

이처럼 vp 파일은 어느 frm 파일을 사용하고 있는지의 정보를 가지고 있다. @의 조작
으로 이 정보도 바르게 지정된다. O~O2] 사용법을 잊지 않고 복수의 frm 파일과 bas 파
일을 사용하고 있는 때에는 전부 복사해야 한다. 만일 어떤 파일을 공유해서 사용하고 싶을 경
우에는 해당 파일의 복사는 필요하지 않다.

실제로 애플리케이션의 개발에 있어서 각종 컨트롤 배치가 끝난 이후에는 거의 대부분으
작업을 코드 에디터에서 하게 되므로 코드 에디터의 사용에 익숙해지는 것이 중요하다. 여기
에서는 코드 에디터에서의 여러 가지 조작을 정리한 표3-8을 보도록 하자.

|

3-6 |

=              한 문자씩 좌측 이동
=              한 문자씩 우측 이동
| 때              한 줄씩 위로 이동
w             한 줄씩 아래 이동
(Cir) +)           다음 프로시저를 표시
~(en+00          하나 앞의 BEAMS 표시
(e+)          하나 오른쪽 단어로 이동
_(er)+3          하나 왼쪽 단어로 이동
            행 끝에 이동
[여1+60의        모듈의 맨 뒤로 이동
0009            행의 맨 앞으로 이동
(Cirl) + ome)        모듈의 맨 앞줄 왼쪽 Boe 이동
고            프로시저의 맨 앞줄/맨 ASS 찾아가며 앞으로 이동
            프로시저의 맨 앞줄/맨 ASS 찾아가며 다음으로 이동
(Cini) + (iE)        프로시저의 맨 앞줄을 찾아가며 앞으로 이동
_ (Cia) + Caz)        프로시저의 맨 앞줄을 찾아가며 다음으로 이동
_ (er)+          커서 위치를 개체 YAS 이동
_ (e+)          커서 위치에 있는 프로시저의 정의한 부분으로 이동

(Cir) + hit) +2     코드 WOM 점프 전의 커서 위치로 돌아간다.

128


===== PAGE 129 =====
3.8 코드 에디터의 사용법

          좌측 문자를 삭제

(Ctrl) + (Back Space)      커서 AAA 앞의 HHS 삭제    :

Delete)            한 문자 또는 선택되어 있는 SASS 삭제(보존하지 않는다)
_[Cit} + 6009        AA 위치의 뒷 단어를 삭제

            커서 위치에서 줄 바꿈

             삽입 모드의 On/Off

Tab)             ts # 위지로 이동

Shift} + (Tab)        전 탭 위치로 돌아간다(들여쓰기를 삭제)
“(ee (Sarees) 클림보드로 복사

(Ctr!) +(N}         현재 라인 앞으로 공백 라인을 삽입

(Cir) +[0}          반복(전으로 돌아간 AS 전으로 돌아간다)

[여01+[/(6001+100) 붙이기(클립보드로부터)
_ (em) +X)([C (Chi)+ined) 자르기(클릭보드에 보존)

| 에         현재 AS 삭제(클립보드에 저장)
+[21

_ (Ci)            바로 앞의 편집 작업을 앞으로 되돌린다.
es
키
(Fl              상황(커서 위치)에 대한 도움말을 표시
(F2)               개체 브라우저를 표시
(F3)               커서가 있는 위치에서 아래로 검색한다.
- Grif + 3          커서가 있는 위치에서 위로 검색한다.
(F4)               속성 창 표시
(Shiff) + [F4]          속성 페이지 표시
실행 개서(중단 모드의 경우는 실행 중단)
(Cin) +65          컴파일 후에 실행
(Shift) + 55         OH 앞부터 재실행
                코드 창 표시
_Ghif} +{7)           = A 표시
               한 단계씩 코드 실행
__ (Cini) +(e}          커서까지 실행
 600+         프로시저 단위 실행
(F9)              중단점의 설정과 해제
(Ctrl) + (Shift) + [F9)      모든 중단점의 설정과 해제
_ (Cir) +(F9)           [디버그]-[다음 2 설정(44)]
601 + F9)        AMA BS 연다(중단 모드시)
(Alt) +(Q)         Visual BasicS 종료한다

129


===== PAGE 130 =====
130

Chapter 3 Visual Basic2| 기본 조작

(Alt) + [F4)          Visual BasicS 종료한다
(Cir) +0)           실행을 중지
(Ctrl) +A)          Be 텍스트 선태
(Cin) +)          파일의 추가
(Cir) +(5)          파일을 보존
(Ctrl) +[F)          검색
(Ctr) +6)          직접 실행 창을 연다(중단 SEA)
_(ca)+          치환한다         2
~ (em) +0          프로시저의 호출 이력이 표시(중단 SEA)
(Cir) + (N)          신규 프로젝트를 작성
. (eri)          프로젝트를 열기
. (cra) +F)          인쇄하다 _ _
~ (Cr) +R)          프로젝트 탐색기를 표시
__ (Cin) +)           조사식을 표시
_ fen) +)         속성/메서드의 보기 표시
(Ctrl) + Shit} + (J)      정수의 보기를 표시
_ {ei} +1)          RF Bao FA
(Ctrl) + Shift] + (1)     파라미터 힌트를 표시
_ (Cir) + (Alt) +(A)     입력 후보를 표시

3] 텍스트의 삭제와 이동 그리고 복사
코드 중에 있는 텍스트를 처리하고 싶을 때에는

메뉴를 사용할 수도 있다
삭제1
O 해당 텍스트 부분을 드래그해서 반전시켜 둔다.

삭제2 (삭제한 텍 재테 클립보드로 보존)
Ho.

© 해당 텍스트 GES 드래그해서 반전시켜 둔다.
@ (801 +를 누른다.

이동
(1) 해당 텍스트 부분을 드래그해서 반전시켜 둔다.
@ (여0 + WS 누른

(3) 목적 위치에 AAS 를 둔
@ (601+1|를 누른다.

다음처럼

한다. 이 중 키 조작은 [편집(0)]


===== PAGE 131 =====
3.8 코드 에디터의 사용법

복사
O 해당 텍스트 BRS 드래그해서 반전시켜 둔다.
(2) (mM+OS 누른다.

@ 목적 위치에 커서를 둔다.
@ CH+MS 누른다.

드래그에 의한 텍스트 이동_             =     a
텍스트 이동은 전에 기술한 바처럼 (+H, | eee 더 sa ‘alsloy Visual
Basic? 드래그&드롭으로 이동시킬 AE 있으며 조작은 다음과 같다.

이 기능은 BEALE 유효하지만 다음 설정으로 PAS 수도 있다.

[도구(1)]-[옵션(20)]-[편집기]-[ㅁ텍스트 끌어서 놓기(2)]

Undo/Redo..                 '
AES 질못해서 삭제하는 So] BSL 원래대로 ESS + 있다. 편집 머뉴에서 되돌리
기를 이용하면 되며 전으로 되돌아갔던 것을 다시 되돌리는 기능이 있다.

다시 되돌리기
(Ctrl) +(Z)

_o) 문자열의 검색과 바꾸기
텍스트를 검색 또는 바꾸기할 때에는 다음 메뉴를 사용한다(그림 3-40).

[편집(6)]-[찾기(「-)]((여+)
[             [바꾸기(6)](여+)

131


===== PAGE 132 =====
Visual Basic 2| 기본 조작

먼저 마우스를 올려 놓은 부분의 텍스트가 반전되어 나타나면 그것이 찾을 내용이고 바꾸기 전의 문
자열이다. 바꾸기는 찾기 창에서 모두 바꾸기를 추가된 것으로서 검색 창에서 바꾸기03 배튼을 클릭

하면 바꾸기 창으로 이동할 수 있다. 같은 문자열의 재탐색은 88((아래로), 6008+0|(위로)이 편리하다.

;       | 선택

찾을 내용 입력                 찾을 내용에 입력했던 문자열을 cha
찾기 실행
찾기를 중지하고 다이얼로그
박스를 닫는다
»                                   [바꾸기] 다이얼로그 박스에 이동한다
탐색 방향을 아래로 또는 위로의 설정
|                   대표 기호를 사용하여 찾기
대소문자를 구별하여 찾기
단어 전체가 일치하는 문자열만 찾기
프로젝트 내의 선택 범위에 포함된 코드 찾기
ㄴㄴ 프로젝트 내의  든 모듈 찾기
ㄴ 현재의 모듈 찾기
현재의 프로시저 찾기

|씩 확인 18 하면서 바꾸키
! 작업 없이 전체 바꾸기

렸고 두 . 에 디 터 위 동월 ae
코드를 입력 중에 입력이 끝난 키워드 BAS 알고 싶어지면 그 키워드에 ANS 위치시키
고(어느 문자라도 좋다) AS 누른다. 그러면 해당하는 도움말이 표시된다.

Do While A < 10
0 여기에 ANS 맞춰서 『|을 누르면 Do 문의 도움말을 표시

132|


===== PAGE 133 =====
3.8 코드 에디터의 사용법

작성중인 폼과 AES [파일00)]-   인시) 메뉴를     를 이용하여 프린터로 인쇄할 수 있다. [인쇄]
다이얼로그 박스가 표시되므로 항목을 설정해서 확인 HES 클릭한다(그림 3-41~그림 3-43)

Forml ~ 1
VERSION 5.00
Begin VB.Form Forml
Caption                   =       "스톱워치"
ClientHeight    주 0195
ClientLeft       =) 60
ClientTop        = 345
_ClientWidth        = 4680
LinkTopic        =    "Form"
ScaleHeight      = 3195
ScaleWidth       = 4680
StartUpPosition = 3           'Window 의 계정값
Begin VB.TextBox Text1
Height           = 855
Left             = 360
TabIndex         Sere

133


===== PAGE 134 =====
134

Chapter 3 Visual Basic2| 기본 조작

Top                                       =         240
Width                                 = 3975

End

Begin VB.CommandButton Command2
Caption                        =         "종료"
Height                              = 495
Left            =   2520
TabIndex                     =        a
Top                =    2400
Width                                 = 3815

End

Begin VB.CommandButton Command1
Caption                           =          "Start/Geop”
Height                              = . 495
Left              =    360
TabIndex                     eet 8)
op                                  =        2400
Width                             =        1815

End

End
Forml - 1

Private Sub Command1_Click ( )
Static Stwch
Static Tm
If Stwch = False Then
Tm = Timer

Textl.Text = "측정시작"
Else
Textl.Text = Timer - Tm & "Zit"
End If
Stwch = Not Stwch
End Sub
Private Sub Command2_Click( )
:    End
End Sub


===== PAGE 135 =====
3.9 도움말의 사용

Visual 88810에서 프로그램밍할 때에는   다수의 컨
이러한 기능은 대단히 많으므로 전부를 7

정리하는 것도 곤란하다. 보다 필요한 정보는  는 온라인 도
하다면 이 도움말로 정보를 얻게 된다.

Visual 88810의 도움말이 마이크로소프트 ASS] 도움말과 크게 다른 ae        전
거대한 111101Ｌ형식으로 되어 있다는 점이다. 버전 6.0부터는 개발환경 이외의 도움말 뷰
사용한다. 도움말이 별도의 창으로 표시되어 개발 티티 pi   [때 이용이
하다. 도움말 뷰어는 a Basic 개발 환경의 [도움말03) ]-[목차(2)], (E22
0)], [도움말08)]-[검색(8)]에서 실행된다. 일단 Age 애견 그 지시는 도움말 뷰어 중
있는 메뉴에서 표시해 be

도움말 뷰어는 왼쪽 창에 모든 목차가 표시되며 항목을 더블 설명이 오른쪽 창에
표시된다. 또 설명 본문 중의 색깔 있는(밑에 밑줄이 그어져 있음) 항목을 클릭하면 그 항목으

로 이동하거나 이동하기 전의 위치로 돌아갈 수 있다. 이와 Z 20]   이동하면 목차(왼쪽 창)와 설
명(오른쪽 창)이 일치하지 않게 된다. 이때 도움말 뷰어의 [보기(/)]-[동기(Ｌ)]를 선택하면 현
재 설명하고 있는 내 해당하는 목차 HES MLS 반전한다.

도움말 중 어디에 무엇이 작성되어 있는지는 목차에서 여기저기의 FSS 열고 어느 정도
스스로 체험에 의하는 수밖에 없다. 여기에서는 도움말 참조의 예로서 “명령 버튼 컨트롤의
082400 속성을 조사한다"라는 조작 순서를 제시하니 참조해 보자.

화면1 도움말 메뉴를 선택

© 이 메뉴를 클릭한다

135


===== PAGE 136 =====
136

Chapter 3

Visual Basic 2} 기본 조작

HH2 목차와 설명 표시

{oli

— 6 목차가 표시된다. 책을 더블 클릭하면 중간 목차
가 표시된다. 이때 책은 열린          |

@
모으
°
모

J
Olt
ra
I> £
0%

을 클릭하면 메서드 보기를 표시하다
이것을 클릭하면 이벤트 보기를
나타낸다

프로세스의 시작, 중단, 종료 시 CommandButton HESS 사용합니다.
CommandButtonO| 선택된 경우 눌러진 상태로 표시됩니다. 그래서 누름 단
추라고도 부릅니다.

이     MSDN Library 들매가기

8 @ Visual Studio Scho! 설명서
ㅁ @ Visual Basic 온라인 도움말
Visual Basic 시작 페미지
Visual Basic 설명서 OHH
Visual Basic 6,02] 새로운 기능
Visual Basic 6.0시작하기          - | | CommandButton
Visual Basic 사용                   4

, | 참고

CommandButton 컨트롤에 텍스트들 표시하려면 Caption SAS 설정하십

= 4] 시오. ORAS 눌러 CommandButtonS 선택할 수 있습니다. <Enter>71Z
i] CheckBox HES       i       놀러 WES 선택하려면 0618배! SAS True= 설정하고 <ㄷ666>키를 눌러 단
=] ComboBox 컨트롤       :     추를 선택하려면 CommandButton2| Cancel 448 True= 설정합니다.
2]

2) Data AES
iz) DirListBox 컨트롤
2

＊ = ㆍ

al
L@ Command Button 컨트롤의 설명이 표시되었다

[로부터 이 항목을 찾으며 더블 클릭한다. 어디에 어
떤 항목이 있을까 하는 시행 ASS 거치면서 기억한다

미        3(Col         Button 컨         양             매밍
Appearance 속성                      Visual Basic 참조
BackColor, ForeColor 속성                    Visual Basic 참조
Cancel 속성                                  Visual Basic 참조



===== PAGE 137 =====
3.9 도움말의 사용

piesa enema            al 예제 Ashes
© Q) MSDN Library Visual Studio 6,0

MSDN Library #017471                        ＊ 폼 —FormO|U+ MDIForm 개체의      표시즐에 나타나는 SASS 결
Visual studio | 22H! 설명서                      정합니다. Sol 최소화되면 문지열은 Sous

밑에 나타납니다.
인

6 0 rhea                      + 컨트롤 ㅡ 컨트롤미니 컨트롤 옆에 나타나는 SNS 결정합니다.

5    seer ate eee 기능              ㆍ MenuLine 개체 — Menu 컨트롤미나 Menultems 컬렉션 개체즐 나

& @ Visual Basic 6,0 시작하기          4           pal IS ii ile

ae ee                  Menu 컨트롤은 실행 Sede Caption S42 대개 2171/47] 겸용입니
다, 그러나 MenuLine 기      갈미 Visual BasicO| 추가 기능에 나타내고 SS
하는 메뉴의 Caption 읽기 전용입니다.

2) ComboBox          『
의 CommandButton 컨트롤
(2) Data 컨트:               ;
(&) DirListBox 컨트롤

i) DriveListBox HES

is) FileListBox 컨트

if) Frama AE

도
fc CheckBox 컨트롤       °
N

이것을 클릭하면 이 Santi 4 aA  성을 2 2H 컨트롤 보기가
전부 역으로 표시된다.
주) 여러 가지의 HES Caption 속성을 갖고 있다.

화면5 사용 예가 표시된다

© Caption 속성의 프로그래밍 예가 표시된다

해서는 000008001으로 명          omman   suc
MSDN Library Visual Studio 6,0                                                              a
MSDN Library 들머가기                       품의 선      Seth BSS SOD <PHalS 누르고 AAS 선택합니
Visual Studio 22}2! 설명서
ㅁ QQ Visual Basic 온라인 도움말                 teas ae Cope eee Maye
eta Bese 시형 OA              If Conmand! Caption = "선택" Then
Visual Basic 설명서 OHH                                                 확인"

Visual Basic 6.0의 새로운 기능 |          Command! Caption

Else
Command! .Caption = "선택"
If

End
End Sub

Visual Basic 6,0 시작하기
Visual Basic 사용
조

Qa &
0 @ Mo 참조
ㅁ 00 컨트롤 참조
6 Que 컨트롤

137



===== PAGE 138 =====
Chapter 3 Visual Basic2| 기본 조작

화면6 색인으로 찾는다

(1) 이것을 클릭하면 키워드 검색 화면이 된다.

@ “Captions 입력하면 © 목적 도움말이 표시된다

＊ 폼 -【0『미미나 버마『00 개체의 제목 표시졸메 나타나는 SASS 결
정합니다. 폼미 최소화되면 문자열은     마미콘밀메 나타납니다.

* 컨트롤 ㅡ 컨트롤미나 컨트롤 Sol 나타나는 SASS 결정합니다.

＊ MenuLine 개체 —Menu 컨트롤미나 Menultems 컬렉션 개체를 나
타내는 SASS 결정합니다,

{Caption 609 ine propel
| command button groups
| common buttons

lorms
| labels                         :
‘| specifying access 1805 for
-|__storing to tabi

les with optior                     =                    S
:               Ee Caption 40004 개체)                   Windows ay
tutorial          | Caption 속성(8300 개체)             Windows 컨트

nal  ON Statement      Caption $4(DataGrid 컨트롤. Column 개.,  DataGrid dee

ie      very 1) Caption 44(DEDesigner 확장성)    Visual Basic 참조

{caption       A TT
1001   hangi           176 컨트:       sual Basic 잠소

a ng Ee elds

Caption 속성                                 Visual Basic 참조

@ 항목이 표시된다. 이것을 더블 클릭하면

© ‘Caption’ 에 관련된 항목이 표시된다.
이것을 더블 클릭하면

터도움말 사용하기
코드 입력 화면에서는 We 상황 의존의 도움말을 사용할 수 있다. 예를 들면

command1 .Caption="A|2t"

을 할 때 "캡션" 문자 어딘가에 커서를 맞춰서 HS 누르면 키워드 '캡션"의 도움말이 표시된다.

138


===== PAGE 139 =====
3.9 도움말의 사용

화면7 전체 문자 AMS 한다

@ 이처럼 입력하고
(1) 이것을 클릭하면 검색 화면이 된다

© 목적 도움말이 표시된다.
호환성” 부분이 강조되어 표시된다

버전 28 사용 시기
참교

| Visual Basic= 소프트웨머 PA 요소를 확장하는 동안 하위 버전 호:
지하기 위한 두가지 메커니즘을 제공합니다, 바로 버전 099 7  능가
| Implements 기능입니다.

ㅣ Visual carey 버전       기능은 미전의 HAS 사용하며 | 컴파밀된 ae  그
Sot 함께 하위 버전 호환성   뮤지하는데 필요한 구성 요소를 확장하는 한 방법
Such. petites   설] 대화 상자의 [구성 요소] SIO 위치해 있는 버전 i= =H
Bp 상자는 3가지 옵션  2 갖고 있습니다.

* BSS 38         즐 컴파일할 HOCH MSS 클래스의 10와 새로운 ㆍ
버스 io 포함왼 새로론 HH 라미브러리정보가 샘섬윌니다. 구
“                       |         성 요소의 버전 사미메는 마무런 관련미 없으며 한 버전에 맞게 컴파일된
나비 Berea”          |          프로그램은 다름 버전메 사용할 수 없습니다.

프로젝트       구성 요소즐 컴파일할 때마다 형식 라미브러리

가 보존되므로 테스트 프로젝트는 구성 요소 프로젝트메 대한 함조들 뮤
지할 수 있습니다. 미전 HAS 모든 클래스 1ㅁ가 보존됩니  He   민터페미
ae 버전과 Ola 미진 호환성되지 많는 클래스 일 경우

모

때도

|

pm OI Sa Oo COOL EMS SLM MOL leo!

@ 이것을 클릭하면           @ "호환성"이라는 문자열을 포함한 텍스트 명이
나타난다.
이것을 더블 클릭하면

139


===== PAGE 140 =====
140

' Chapter 3 Visual Basic 2| 기본 조작

화면8 즐겨찾기에 등

버전 사용 시기

Visual Basic= 소프트웨머 구성 요소즐 확장하는 동안 하위 버전 seas 유
eckBox 컨트                                 | 지하기 위한 두가지 메커니즘을 AS  합니다. 바로 버전
Function 컨트롤(0013 Report 디자미너)                    Implements 기능입니다.

버전 BE

Visual Basic’2| 버전        기들은 미전의 HAS 사용하며 컴파밀된 프로그
램과 함께 하위 버전          유지하는데 필요한 구성 요소'     를 팍장하는 한방법 |
니다. [프로젝트 속성] 대화 상자의 [구성 요소] Soil 위치해 있는 fect}  a
뽑! 상자는 3가지 SUS 갖고 있습니다,                                        i
4

- eee   없음: 구성 요소즐 컴파일할 때마다 새로운 SHAS! 10와 MSS
미스 10가 포함된 새로운 형식 라미브러리 정보가 생성됩니다. 구   4
성 요소의 버전 사미메는 마무런 관련미 없으며 한 버전메 맞게 컴파일된

프로그램은 다음 버전에 사용활 수 없습니다.                                『

a
SENS 0 구성 245 Roe E MOI! 형식 clolwaiel 식벌자
스트 프로찍트는 구성 요소 프로찍트에 대한 참조좋 S ㅠ
김홈 수 있습니다 O14 eel Se 클래스 ot 보존임니다 인터비미스
IDE 미전 버전과 더 미상 미진 호환성되지 않는 클래스 일 Swe 변경
다

a
a

ES

om

om

@ 현재 도움말 항목이 표시되고 있다              @ 이것을 클릭한디

© 여기에 등록된다. 이 후의 항목을 더블 클릭하면
언제라도 도움말을 볼 수 있다



===== PAGE 141 =====
NOTE

3.9 도움말의 사용

도움말 항목을 발견하는 요점

신형 도움말은 가끔 찾고 싶은 FSS 제대로 찾지 못하는 일이 있다. 아래에 Visual Basic 버전 6.0 의

최초 판을 근거로 하여 항목 검색 포인터 몇 가지를 적어 보았다.

(1) 개발 환경 메뉴를 알고 싶을 때 [메뉴]에서 찾아도 발견되지 않는 경우가 있다. 이러한 용어는 메뉴 에
디터 등의 SSO] 해당되므로 개발 환경의 사용 방법에서 보여지지 않는 문제가 있어 개별 항목으로
찾는 방법밖에 없다. 만일 [편집(6))에 대한 내용을 알고 싶은데 목차 탭에서 보이지 않는 seal 키
워드 탭을 사용하여 “WAS 입력하여 찾아도 발견되지 않는다. 정답은 '[편집]"이다. 이것으로 찾으
면 [편집] 메뉴 커맨드라는 항목이 발견된다. 이처럼 보기 전에 HS "[ )"로 둘러싸인 형식으로 등
장되는 일이 많다. 예를 들면 지역 창을 알고 싶다면 "[지역]"으로 검색하면 발견된다.

(2) 표준 컨트롤의 도움말은 [목차] 탭으
[Visual Basic 온라인 도움말]-[참조]-[컨트롤 참조]-[내부 컨트롤]

로 정리되어 있다. 그러나 빠져 있는 것도 있다. 예를 들면 [OLE 컨테이너]는 없다. 그것으로 키워드
BS 사용하는 것이지만 여기에서도 항목 지정에 생각을 요구한다. 우선 “OLE OAH 잘 발견되지 않
는다. 다음에 "ㅇ0.ㄷ컨테이너"로도 발견되지 않는다. 정답은 "0ㄷ컨테이너"이다. “OLE” 후에 공백이
한 개 필요하다. 이처럼

-두 개 이상의 단어로된 용어의 경우에는 Apolo] 공백을 넣으면 발견되는 a 많다.

ㅎㅎ
라는 것을 알아두면 좋다. 같은 경우로 만약 체크 박스 AEST 옵션 배튼 컨트롤을 키워드 use 검
색하고 싶은 때에는 반각 공백을 두 개 넣어서 체크 박스 컨트롤, 옵션 배튼 컨트롤로 하지 않으면 발

견되지 않는다.

(3) 마찬가지로 데이터 컨트롤도 목치에는 없다. 이것도 키워드 탭의 AME 지지만 생각할 필요가 있다. 이

Lone =

AS 데이터 예로는 안되고 SHS 사용한 데이터 컨트롤에서도 발견되지 않는다. 정답은 영문자를 사

소비 oe

용해 반각 SHS 넣은 데이터 컨트롤이다. 이처럼 영문자로 찾지 않으면 발견되지 않는 항목도 있다.

(4) Visual Basic2 폼 AMIS 속성과 이벤트를 갖고 있다. 그 폼의 일을 조사하고 싶어도 목차 탭에서

는 발견되지 않는다. 거기에서 키워드 탭을 사용하는 것이지만 어떤 항목 이름으로 할지 몰라 많이 헤
맨다. SHE 영문자를 사용하고 SYS 넣은 “폼 오브젝트"이다.

7 to

(5) [목차(0)]-[색인()]은 별개이다. 키워드로 적절히 찾은 항목은 목차 탭으로부터 표시되지 않은 특별
텍스트인 경우가 있다. 이때는 [동기] HE 기능이 무시된다.

141


===== PAGE 142 =====
ll
CHAPTER

면수의 선언과 데이터형

이 장에서는 Visual Basic 2| 변수에 대해서 살펴볼 것이다. 기본적
할독에서무터 개체형, ee 배열 기능, 가변형이라는 — 시

ㅅ     lo)
도 상관없다. Set Zt New ec 7 능은 필요할 때 다시 반복해서 읽으면
된다. 처음이라는 SHS 갖지 말고 가벼운 마음으로 이 장을 시작해 보



===== PAGE 143 =====
144

_ Chapter 4

변수의 선언과 데이터형

Visual Basic 2 종래의 베이직으로 사용되던 데이터형을 그대로 사용하고 있으며 몇 개의
새로운 데이터형이 추가되었다. 그 중에서 가변형(0/8118200은 강력한 데이터형이라 할 수 있다.

가변형은 종래의 기본적인 모든 데이터형을 다룰 수 있는 범용 데이터형이다. 프로그래밍
할 때 가변형을 사용하는 것은 편리하지만 메모리를 많이 사용하고 처리 시간이 많이 걸린다
는 단점이 있다. 만약 애플리케이션 크기를 작게 할 필요가 있거나 처리 속도를 높일 필요가

있는 프로그램에서는 데이터형을 확실히 지정하여야 한다.
먼저 큰 프로그램을 작성할 때 데이터형을 확실히 지정하는 것이 입력 내용을 알기 쉽게 한

다. 가변형은 이러한 장점을 살려야 할 때 사용하는 것이 좋다.
Visual Basic 9] 데이터형을 정리하면 그림 4-1처럼 된다.

Integer     g
Long       &
Single      !
Double     #

Currency @

String              $

Byte

Boolean

Date

Object

Lo LL

Variant
= 사용자정의 형

- 고 고 고 고 고 고 고 가 개 0.

종래의 베이직에서는 변수의 선언은 불필요했다. 이것을 묵시적 선언이라 한다. 예를

ful
re


===== PAGE 144 =====
a=100

과 같이 입력할 수 있다. 변수 8가 나타나는 시점에서 자동으로 변수 a7} 선언되는 것으로 처
리되었다. 이것은 편리한 반면 프로그램 품질 저하로 연결된다. 예를 들어 아래와 같은 내용
이 있다고 가정하자.

A0=100      변수명 40(에이, BS AS
20=00+200 틀려서 4(/(에미, 모)로 입력되어 있다.
PRINT AO                              :

이것의 SAS “300"0] 아니라 “100”이 된다. 이런 종류의 잘못된 BAS 곤란하다.
Visual Basic = 종래의 묵시적 선언도 허락하지만 “변수는 선                           것
을 권장한다.

ee
el)
or >

종래의 베이직에서는 변수의 선언 없이 사용된 데이터형을 지시하기 위해서 형 선언 문자
를 ABO} Visual Basic HAE 이러한 기능이 그대로 사용된다. 그러나 16481 Basic
에서는 “변수는 선언 없이 사용하는 것이 바람직하며, 범용 데이터형인 가변형이 있다.”라는
두 가지 이유로 형 선언 문자가 사용되는 일이 적지 않게 되었다. 형 선언 문자는 표 4-1처럼

되어 있다.

예 : A%=100
= 42 ecm som 0
형 선언    의미
나 26   :   변수 ^ 는 101696「(정수형)이다.
VATS         변수 AS ㄴ009(장정수형)이다.
~ 지        변수ㅅ는 910016(단정도부동소수정형)이다.
V A#      변수&는 ㅁ046016(배정도부동소수정형)이다.
Y A@       HAA Currency(S sts) 0|ct}
V_A$          변수 는 String(@AtSs)olct
A         HAAS Variant(7tHS)olct 형 선언 SAS 생략하면 가변형이
된다

145


===== PAGE 145 =====
146

Chapter 4

변수의 선언과 데이터형

Dim A As Integer                        Integer 3 변수2를 선언
Dim 단가 As Integer                      한글도 사용한다

Dim B As Integer,C As Integer,D As Long 변수8, c, pS 선언

Dim Datal As Variant                     가변형 HA patal S 선언
Dim Data2                             가변형 변수 Data2S 선언

줄이기 위해서 묵시적인 변수 선언을 금지할 수 있다. 명시적인 변수
없이 변수가 사용되는 때에는 Bal’ op] 설정한다. 그것에 폼 모듈
등의 선언 섹션에서 Option Explicit e}a1 입력한다. 또 [도구(1)]-
변수 es  2=H(R)] lV Ve 표시하면 신규 작성하는 모든 모듈의 변수

<7:
인
그
Ley

ia tle
떠0
1
SL
> =
of   Hi ¢
LJ] mn (오 :

변수명은 다음과 같은 규칙으로 붙여진다.

영문자 또는 2바이트 문자(한자 등)로 시작된다.

#@ 피리어드(.)와 형 선언 문자(%,$,!,@.&)는 사용할 수 없다.

# 255 문자 이내(반각 상당)에서 붙인다.

@ 영문의 대문자와 ASAE 같이 취급된다. “08131 과 “ㅁ041^1" 등의 혼란이 있어도 선언 시
에 입력한 변수명으로 통일된다.


===== PAGE 146 =====
변수의 통용 범위                  !                          :

변수는 어느 범위까지 ash  지에 대해서는 정해져 있다. 그 통용 범위를 자세히 지정하
기 위해서 Dim k= 몇 개의 선언자가 있다(그림 4-9). 여기에서는 21끄선언자의 의미에 대
해 다시 설명한다.

— 프로시저 내에서의 선언 ==ㅠ= ㅁ1ㅠ    |
ee  Static   |
느기 모듈 내에서의 선언 }   {Dim

때   Private     }
|  Public    ㅣ

프로시저 내에서 선언하는 경우

Dim Datal As Integer

* Datal 2 프로시저 내에서만 사용된
* Datal& 그 프로시저가 실행하는 동안만 존재하는 변수이다

Static Datal As Integer              정적변

aie

* Datal2 그 프로시저 내에서만 통용된다
* Datal2 그 프로시저가 실행되고 있지 않을 때에도(애플리케이션이 종료할 때까지) 계속 값
을 갖고 있다

모듈의 선언 섹션에서 선언하는 경우

Dim Datal As Integer

* Datal? 그 모듈 내(모든 프로시저)에서 유효

Private Datal As Integer

* Datal? 그 모듈 내(모든 프로시저)에서 유효

147


===== PAGE 147 =====
「   Chapter 4

148

변수의 선언과 데이터형

*이 AD Private 1010 은 같은 의미가 된다.

* Datal? 다른 모듈의 모든 프로시저에서도 유효하다
*애플리케이션내의 모든 프로시저에서 사용할 수 있는 변수이다

같은 이름의 변수는 식별이 가능하다면 어느 곳에서도 사용할 수 있다. AS 들면 프로시저
AS} 프로시저 중에서 같은 변수 명을 사용해도 전혀 문제가 없다. 또 모듈로 선언되고 있는
변수와 같은 이름을 프로시저 내에서 사용할 수 있다. 이때는 프로시저 내에서의 선언이 우선
한다(그림 4-3).

Public Dt                모듈의 선언 섹션에서 마를 선언

프로시저1

16811의 미가 유효

이 프로시저 내에서만 유효한 Kosuu
76511의 며에 대입

76811의 KosuuQl] 대입

이 프로시저 내에서만 유료한 Kosuu
모듈에 선언된 며에 대입
76812의 KosuuOll 대입



===== PAGE 148 =====
4.2 배열의 선언

ALS Static] 여부를 지정하지만 SSO] 선언 섹션에서 선언하는 경우는 oF
변수가 된다. 또 프로

기능상으로 모든 변수가 6316과 같은 정적 변수

프로시저 내에서의 변수 선
Nom] & 프로시저에서도 사용이

시저의 첫째 줄에

Sc 사아 나 Oe

가능하다는

Static Sub Myproc(1)

과 같이 StaticS 붙이면 그 프로시저 내의 로컬 변수는 |S StaticOe 취급된다
기 참조)

(7장의 7-2 서브 프로시저 불

를 보자.

에 제시한 선언의 예

명을 여러 개 사용할 때에는 배열 선언을 한다. 다음

같은 변수
Dim A(10) As Integer
이것은 4(0)~4&(10) 11개의 RAS ZH Integer 배열이다. Visual Basic HAS 표준으
로 0부터 시작된다. 단
Option Base 1
하면 1부터 시작한다. 이것은 4(1)~4ㅅ(10)까 ” " 개 요소를 갖는다
음 열은 8(3)~808)까지 유효한

이라는 명령문을 입력

Visual Basic A= 범위 지정 배열도 선언할 수 있다. 다음

~ eee

배열이다.
Dim B(3 To 8) As Integer
또,
Dim 0(10)
는 형의 이름이 없으므로 가변형 배열이다. 가변형 배열에서는

149


===== PAGE 149 =====
Chapter 4

변수의 선언과 데이터형

C(0)=123
C(1)="abcde"

와 같이 다른 데이터를 대입할 수 있다.

음은 정적 변수의 배열을 선언한다.

Ls

Static D(10) As Integer

프로시저의 내에서가 아닌 모듈 선언 섹션으로 S24] 4 PublicS 사용하여 선언하면 =
로그램 구성 파월 중 모든 프로서저에서 사용할 수 있다:

이

Public E(10) As Integer

음은 다차원 배열의 선언이다. 800,0)-9.9)까지 사용할 수 있다.

Dim F(9,9) As Integer

150|

Dim G() As Integer            HISSGS 선언해 둔다.

ReDim G(10)                       배열을 6(0)-06(10)으로 DAA 선언한다.
배열 데이터는 초기화된다.
:                                 (수식형-(0,문자 배열-" “,가변형-6[00!/로 된다.)
ReDim Preserve G(20)           다시 배열을 G(O)-G(20)2= 바꿔 선언한다.

배열 데이터 6(0)-6(10)의 값을 계속 유지한다.
N = 10                         프로그램 중에서 변수 의 어떤 값을 설정했다고 한다,
ReDim G(N)                       G(0)}-G(N)S 선언


===== PAGE 150 =====
4.5 문자열형(50009)

Visual Basic 에서 사용

SEA 9]느
할 수 있는

기본적인 데이터형과 그것이 메모리에 차지하는 바이트

(Byte) 그리고 값의 표현 WHE 다음에 제시한 표4-2와 같다

Integer              % | 정수형                              2                 —32768 ~ 32767
Long     & | 정수형       4    ~2147483648 ~ 2147483647
Single                   |          단정도                                  4                   —3,402823E38 ~—1.401298E-45 (부가)
부동 소수점형                                     1.4012985-45^~3.402823538 (정가)
Double                # | Hae                                  8                   —1,79769313486232E308 ~
부동 소수점형                                    -4.94065645841247ㄷ-324 (부가)
=                                          4,94065645841247E-324 ~~
1.79769313486232E308 (정가)
Currency           @ |통화형                                  8                   —922337203685477,5808 ~
922337203685477.5807
String                $ |문자열형               문자 바이트 수 | 0^~~208(32비트 시스템)
(가변 개정)                                   0^~65400바이트(16비트 시스템)
Byte                            Bytes                           1                0~ 255
Boolean                       Boolean &                    2                 4 (True) SE 744! (False)
Date           Date &          8      서기100년1월1일^~/서기9999 년12월31일
Object                          Object &                        4                 임의의 개체 참조

문자열형(6109)

문자 HAS 가변과 고정 두 가지의 타입이 있다. 가변 쪽의 조작은 간단하지만 고정 쪽이

처리 효과가 뛰어나다.

0) Dim Sst As String
@ Dim Ss2 As String * 50

151


===== PAGE 151 =====
Chapter4 변수의 선언과 데이터형

가변의 경우는 문자열의 크기를 신경쓰지 않고 대입할 수 있지만 고정의 경우는 지정한 길이
(이 예에서는 50바이트)의 문자열을 취급한다. 대입된 문자열이 50바이트에
는 남은 부분에 공백 문자가 채워지고 50바이트를 넘은

이처럼 불필요한 공백 문자가 있으면 문자열의 비교가 바르게 행해지지 않는 등 불편이 있

으므로 "18481 Basic WH 공백 문자 삭제 함수가 준비되어 있다.

Sir= Oris) =문자열 61의 맨 앞에 있는 SUS 삭제해서 str 들어간다
도 =[지00(61)문자열 61의 맨 뒤에 있는 SUS 삭제해서 str 들어간다
= Trim(S!) 0 …아문자열 61의 양쪽 SUS 삭제해서 [로 들어간다

Oo               ral Eee
차가 있을 수 있으므로 정확성이 특히 중요하게 shah    금전의 계산 등에 쏘기 위하여 고정  -
점형이 사용된다. 통화형은 15행의 정수부분+4행의 소수부분 으로 표현된다. 다음은 그 예이다
Dim I As Integer, C As Currency, D As Double
I = 100 / 3               :33 으로 된다
2 = 100 / 3                (33.3333 으로 된다
D = 100 / 3                133 .3333333333333 으로 된다.

바이트형은 0~255까지 밖에 기억할 수 없는 1바이트 정수형이다. 사용 YS Integer

Dim B As Byte
B=100

처럼 사용한다. 바이트형은 바이너리 데이터의 파일 처리에 적합하다. 또 만약 0~255까지의
값으로 괜찮은 데이터라면
152


===== PAGE 152 =====
4.9 날짜형(0816)

Dim Dt(100) As Byte

로 사용하는 편이 메모리를 적게 할 수 있다. 그러나(언어 같은 일반적인 1바이트 단
자처리에는 적합하지 않다. Visual 88810에서의 문자열은 독자적인 관리 방식을 갖고 있으므

인
fo
Ol
el

로 바이트형과 문자열형과의 사이에서 상호 처리를 하는 데에는 테크닉과 F9I7

부울형은 참과 거짓이라는 두 값을 갖는 변수이다. 어떤 AS 유/무, 0ㅁ0/01[, 참/거짓 등
에 표현할 때 사용한다. AA® Integer 변수의 값을 나누어 사용하여 진위 BAS 해도 상관
없지만 부울형을 사용한 쪽이 프로그램을 쉽게 알 수 있다.

부울형은 내부에서 참을 -1, AAS 0으로 표현하고 있다. S Visual Basic HAE 0이 거짓이

- — —v—eSEre       SON     a       _            ‘1            ar
고 0을 제외한 숫자는 참이다. 정수형 변수에 대입할 때에도 이 값이 사용된다. S 부울형의 내부
HAL Integer 2} 같은 2바이트이므로 메모리 절약이 된다든지 처리가 빨라진다는 장점은 없다.

다음 예의 A= -1, BE 100°] 된다.

Dim Flg As Boolean
Dim A As Integer,B As Integer

Flg = True
A = Flg                                      Az -1(잠)이 된다
If Flg = True Then B = 100 Else B = 200         Be 1000| 된다

Visual Basic H= 날짜와 시각을 되돌리는 함수가 있어서 리턴값을 저장하기 위해 날짜형
변수를 사용한다. 다음의 예를 보자.

Dim Today As Date
Today = Now                 '현재의 날짜와 시각을 취득
Print Today               ‘24 예 98/10/29 11:22:34

153


===== PAGE 153 =====
154

Chapter 4

변수의 선

언과 데이터형

개체형의 선언

개체형 변수는    ee FAS 기억해 긴 개체의 214  을 짧은  이름으로 지정할 수 있도록
하거나 같은 변수명으로 복수의 엄의 개체를 새로 바꿔가면서 조작할 수 있도록 하는 장점이

있다. 개제형에는 2 총칭 개체형과 고유 개처형으로 분류할 수 있다.

다음 4개가 있으며 이 변수에서 어떠한 개체가 사용될지 실행할 때까지 잘 모를 때 사용한
다.

Din A 26 Object = 01 SAS 임의의 개체를 SAS 수 있다.
Din AAG 데키 이이변수^는 임의의 폼을 참조할 수 있다.
Dim AAR Control = 별수 는 임의의 HESS 참조할 수 있다.
Dim 2 As 00010659 =변수 ^ 는 임의의 |/미폼을 침조할 수 있다

고유 개체형

사용하는 개체의 SRS 사전에 알고 있을 _ 특정 개체의 SRS 지정한다. 고유 개체가 자
BOF 체크하거나 코드의 실행 속도가 높고 또 읽기 쉽다는 이점도 있다
Dim A 26 Vester변수&는 텍스트 박스만을 참조할 수 있다
Dim A As CommandButton 00000 이변수 ^&는 명령 버튼만을 참조할 수 있다
Set Ol 의한 주소  rn
개체형 변수으  ines                               한다. 다음에는 명령 버튼에

Dim A As CommandButton       개제 변수 설정

Set A = Command            ‘Command! 버튼의 추소를 설정
A.Caption = "실행"            ‘Commandi.Caption= 실행" a} 같음


===== PAGE 154 =====
4.10 개체형(20160

다큐먼트 인터페이스) 폼이라 한다:

한 개의 폼 중에 SAO] Ho] 있도록 애플리케이션 PAR 했을 때 부모와 같은 형태인 폼을 MDE]

개체형의 반대 설정
어떤 변수가 특정 개체형인지에 대하여 알고 싶으면 다음처럼 한다.

(60995 ata is Object Then

(저리)

End If

예 : If TypeOf MyControl Is CommandButton Then ~

Nothing 의 설정과 개체 설정
프로그램의 흐름 속에서 개체 변수와 실제 개체의 관

[토로 해

AAS 해제하는 것이 충분히
하지 않은 채로 읽는 것을 방지하기 위해 좋을 때가 있다. 이런 경우에
사용한다. 일단 Nothing 으로 하면 Set A] 유효한 개체로 연결
를 사용할 수 없다.

rN

비
는 키워드 Nothing 을
하지 않으면 그 개제의 변수

Set MyObject = Nothing

개체 변수가 Nothing 여부에 대한 판정은 다음처럼

Lu

[위
ag

If MyObject Is Nothing Then

New Ol] 의한 이매 모듈의 생성

Sot 명령문의 외관상 기능은 이미 있는 BES 별도의 이름으로 사용할 수 oe 하는 것 외
of 이미 있는 모듈을 다시 한 개를 복사하여서 조작하는 WHS 있다. 그것에는 New FES
사용한. 전자에서는 BAO] 한 개 그태로이지만 ALAS wo] Ber TIRE 인스

턴스가 생성된다라고 표현한다). New ANS 때 또는 86[과 동시에 사용한다.

155



===== PAGE 155 =====
_ Chapter 4

156

변수의 선언과 데이터형

New 사용 예1 : 선언할 때 사용

Dim x As New Forml      새로운 Formis 생성해서 변수×에 AMAIA 수 있다
X. Show               새로운 FormiS 표시한다

New 사용 예2 : setz} 함께 사용

Dim y As Form           개체 변수선언
Set y = New Forml      새로운 Formis 생성하여 에 연결시킬 수 있다
y. Show                 새로운 Form1S 표시한다

Elana

New 9H 의한 인스턴스 생성의 예이다. 폼 위에 명령 버튼을 한 개 배치하여 이 버튼을 클
하면 새로운 폼이 생성된다. 이 프로그램은 지켜보는 것만으로 상관없지만 후에 기술하는
로그래밍 방법을 기억하려면 주의해서 살펴보자.

158  fe

정

Ib

zo Ox
미ㅇ  미호

kl
In

Private Sub Command1_Click()

Dim y As Form                   개제 변수 선언

Set y = New Forml                 Form19| 복사본을 만든다
y.Caption = "복사했던 Form1"      복사된 쪽의 CaptionS 설정
y. Show                      새로운 SS 표시한다

y.Move y.Left + 500, y.Top + 500 볼 수 있도록 새 SS 비켜 놓는다
End Sub

동작의 확인
(0) 실행 aml Command1 bic 클릭하면 두 개의 폼이 표시된다.


===== PAGE 156 =====
4.11_가변형(30800

@ 이 폼이 생성된다

선언과 값의 대입

형은 범용 데이터형이므로 고정 문자열형과 사용자 정의형 이외의 기본 데이터 형을
킬 수 있다. 가변형에는 %와 HAS 형 선언 문자는 없다. 데이터형을 생략할 때에는 가
라 인정된다. 변수를 ANS 때 “As Variant” = 생략할 수 있다.

Dim A As Variant       가변호
Dim B                  가변호

02! og
rz

7
j2 (2

i

가변형에는 기본 데이터형 이외에 Empty 값, Null#, 에러값, Nothing 이라는 특별값을
넣어둘 수 있다.

가변형 변수에 값의 대입은 기본 데이터형을 사용할 때와 같으며 자동으로 적절한 메모리
영역이 확보된다. 정수값을 대입하고 Bye 문자열을 대입해도 상관없다 .대입한 값을 문맥
중에서 적절히 판단하여 처리한다. oS 들

T£ Dt = 100 Then

에서 까는 수치값으로서 처리된다.

Dim B                가변형 HAB
B = 1234                   AAS 대입
Print B                     정수 출력

B = "abcde"               문자열을 대입
Print B                    문자열 출력

157


===== PAGE 157 =====
008016『4 변수의 선언과 데이터형

Vartype 함수
가변형 변수를 사용하고 있다면 지금 어떤 BQ] 데이터가 들어가고 있을까 알고 싶을 때가
있다. 그때에는 Vartype HS 사용한다(표 4-3)

B = 1234

C = VarType (B)             ‘C= 2(Integer)7} 된다
B = "abcde"

C = VarType (2)              ‘c= 8(String)O| 된다

정수          값       변수의 형

시 vboEmpty        0         Empty #t(O| 초기화)

/ _NeNull          1         Null 값(무효인 2t)

vbinteger       2         83 (Integer)
vbLong        3        장 A+ (Long)
vbSingle         4          단정도 부동소수점형(510016)
voDouble         5           배정도 4HSA4AAS (Double)
vbCurrency           6                 S5}S (Currency)
vbDate                   7                   = MS (Date)
vbString        8         문자열 & (String)
vbObject        9         OLE LEH O|M 개체
vbError         10        Ol] 44 Zt (Error)
vbBoolean      11        Boolean & (Boolean)
vbVariant        12        버라이언트 & (Variant) 의 배열
vbDataObject    13        H}OLE2E|0|M 개체
vbByte          17         바이트 @ (Byte)

- vbArray      8192    배열

주1: 정수는 Visual 80810내에서 정의되어 있으며 되돌아온 yp 대신에 사용할 수 있다
AQ: 바열의 경우는 WE TES 나타낸 Yo 가산된 2턴 같이 된다
주 3 : 여를 EM integer 배열은 8194(2+8192)가 2턴 같이 된다

Empty ata} IsEmpty 함수
SAY 데이터는 선언되면 최초의 값으로 00] 되고 문자배열 데이터는 “ ”이 된다. 한편 가

변형 변수가 선언된 채로 아무 것도 대입되지 않을 때에는 특별 값인 Empty 값을 갖는다. 가
변형 변수가 82ㅁ01》일지 YSZ) Vartype 함수의 되돌아온 값으로도 알 수 있지만 ew
럼 IsEmpty 함수를 사용할 수 있다.

If IsEmpty(A) Then ...      HA 7t Empty et

158



===== PAGE 158 =====
4.12 사용자 정의형(구조체)

El

4, Empty 값을 갖는 가변형 변수는 편의상 숫자 연산 중에서는 0, 문자 연산 중에서는“
"로서 취급된다.

Dim A As Integer
Dim B As String

Dim V

A=V                     ‘AS BE 0이 된다

B=V                    ‘BQ| 값은 “ol 된다
NUII 값과 IsNull

가변형 변수는 의지적으로 대입하는 것에 의해 Null MS 갖고 판정할 수 있다. 다음처럼
사용한다.

Dim A                     `가변형 변수 선언

A=Null                   ‘Null 을 Hel

If IsNull(A) Then ...       변수 &가 Null 0] 2}

여기에서 Null 그 변수에 유효한 데이터가 들어가 있지 않다라는 의미를 갖는 특별한 묵
인 데이터이다. 예를 들면 표 계산 소프트웨어에서는 임의의 셀이

() 숫자 또는 문자열이 들어가 있
(3) 공백 문자열“ ”이 들어가 있다
(3) 아무것도 들어가 있지 않다

를 갖는다. 미 입력 데이터 (3)을 표현하는 것이 *411값이다. 가변형
하면 그 값을 갖는다. Nulla 대입을 하지 않으면 Null gS 갖는 응
수의 Empty M2 자동으로 초기 설정되지만 일단 삭제되면 두 번 다시 Empty @&

» tr

SL om

flo 구 때 쪼
lo rir

NF
rir oft
ne,
rlo
ED
a

DAA 유저가 독자적인 데이터형을 작성할 수 있다. 사용자

으 즈
=
정의형의 정의 부분은 표준 모듈 안에서 기술한다.

159



===== PAGE 159 =====
Chapter4 변수의 선언과 데이터형
표준 모듈 안에서 사용자 설정

Type Golf                  Sie 관러히는 형
Name    As String         이름
61160 As Integer      경적~연수
Handicap As Integer        핸디

End Type

프로시저 S04 활용

Dim Player As Golf           골프형 변수

Player.Name = "영진 출판"     이름을 넣는다.

Player.Keiken = 10         경험 연수를 넣는다

Player.Handicap = 15        핸디캡을 넣는다.

Print Player.Name        =

Print Player.Keiken          | 출력한다

Print Player.Handicap     —

사용자 정의형은 배열로 할 수도 있고 그 변수값을 일괄 복사할 수도 있다.

Dim Player As Golf

Dim Sensyu(10) As Golf       배열 선언

Sensyu(1).Name = "영진 출판" 이름을 넣는다

Sensyu(2) = Sensyu(1)        일괄 복사

Player = Sensyu(5)           일괄 복사

Visual 88816에서 Const 명령문을 사용하여 4

는 기호 정 정수를 AA 정하는 기능으로 프로그램

If A > 217 Then

If A > MaxData Then

160

24 a4 기 하기 Tahal “eet ae



===== PAGE 160 =====
4.13 Const 정수(기호 정수)

는 Ho] 기술한 의지를 알 수 있다. 그리고 어디에서 Max 데이터에 27S 선언해 두면 좋
것이다. 또 같은 값이 몇 번이나 프로그램 속에 있고 그것을 일괄 변경하고 싶은 경우 Const’
라면 선언 부분 한 행의 변경으로 끝내 버린다. Const 정수는 다음처럼 선언한다.

4 ro

Const MaxData = 217 0MaxData 2172 한다
Const Jikan = 60 * 60 ……연산자도 사용할 수 있다
Const Aisatu = "Hello" ---문자열도 사용할 수 있다

Const 정수는 BHO] 변수와 마찬가지로 참조할 수 있다. 단지 정수이므로 프로그램 중에
148※×10868=100이라는 대입 처리는 할 수 없다. 또 Const 정수도 필요하다면 통용 범위를 지
정할 수 있으며 방법은 다음과 같다.

특정의 프로시저내에서 유효한 정수
… 그 프로시저내에서 BES 선언한다.
폼내의 모든 프로시저내에서 유효한 정수
… 그 폼 모듈의 선언 섹션으로 ASS 선언한다(당연히 표준

내

),

복수 폼 구조로 할 때 애플리케이션 전체에서 유효한 id’
- 표준 모듈의 선언 섹션에서 PublicS 붙인 ASS 선언한다.
예 : Public Const Pai=3,14157

E Visual Basic: 처음부터 준비된 정수인 편입 정수도 있다. 예를 들면 먼저
0971906의 되돌아온 값을 표현하기 위해 소개한 편입 정수를 사용해서

A = vbLong

라고 하면 A) 값은 30] 된다

i aegis 폼이 한 .애미며 오조 해 코드는 그것에 대응하는 폼 모듈(.[[70)에 저장된다. 큰 프로그
을 사용하는 것이 된다. 이 때 모든 모듈에서 공통으로 사용하기 위

t ee 프로시저는: 표준 모듈(확장자 .686;로 저장된다. 표준 모듈을 추가하는 SHS [MDI 폼 추가
()]-[모듈 추가(\/)]를 클릭하면 준비된다.

모듈의 선언 섹션에서라고 하면 딱딱하지만 요컨대 폼 모듈과 표준 모듈의 코드 잃기 화면으로 옮겨 뭔
Nore| 가를 한다는 것이 된다. 모듈의 선언 섹션을 열려면 다음처럼 한다.

(1 화면 우측 위쪽에 있는 프로젝트 탐색기에서 폼 모듈(107), 표준 모듈(666:의 아무거나 선택
@ 코드 HES

클릭

m

161


===== PAGE 161 =====
|
CHAPTER

연산자

—

이 장에서는 Visual BasicOl] 준비되어 있

는 연산자에 대해서 설명한
다. Visual BasicOl= Like, 16같은 고도의 연산자와 60, Imp 같은
익숙한 연산자도 있다. 잘 사용하면 강력일 232. SAG ASS a

드러나지 않는 연산자는 무시해도 팬질타.



===== PAGE 162 =====
Chapter5 연산자

Visual 828810의 연산자에는 표5-1과 같은 것이 있다. 처음부터 이것들 APS 기억할 필
KE 없다. 특수한 용도인 것도 있으나 기억하지 않아도 프로그래밍에 곤란한 일은 없다. 우
선 기본이 되는 것만 기억해 두고 특수한 것은 필요한 상황에 따라 기억해 나가자.

산술 연산자        산술 연산을 행한다      ^^=/ㅅ-+10

비교 연산자       비교를 행한다          lf A> 5 Then ...

논리 연산자       논리 연산을 행한다      lf A) 6 And B > 7 Then...
문자열 연결 AAA BAS AAS 행한다 StrO = Stri & Str2

"Visual Basic 9] 산술 연산자에는 다음의 것이 있다.

5-2 네어이 의

연산자 설명

시      지수승 V            (ee Ps      0 32 가 Bette 2" 2°22)
os       곱하기 ~            Ae 5      = 157} 된다

/       나누기 Vv           4ㅋ972      — 4.5가 된다

\     q4 나누기 V     Rees    — 40| 된다

Mod    나머지               A=Q9Mod2 1이 된다

호    가산           A= 6 +2    — 70| 된다

si      감산                 Rea 2      — 30| 된다

=      딴항 마이너스 연산자 A ㅋ23        = -3이 된다

164


===== PAGE 163 =====
5.3 비교 연산자

처럼 사용한다. 그러나 Visual 88810에서는 가변형 변수 vi, v2, v3 이 있을 때,
vl=v2+v3

라고 하면 수치 가산인지 문자열 연결인지 애매모호하게 된다. 이를 방지하기 위해 Visual

Basic A= 문자 배열 연결 연산자 &가 있어 문자열 ABS 의미가 확실해진다. 즉 가변형

Aol] + 연산자는 다음처럼 판단될 때 사용한다.

가변형 변수 모음에서 +계산을 할 때에는 내부 처리 형식이 수치 모음이라면 가산을 하고
문자열 모음이라면 문자열 연결, 틀리다면 형이 일치하지 않는다는 에러가 된다,

다음의 기술은 좋은 힌트가 될지도 모른다(변수ㅅ, BCE 가변형)

디               el

Ae “ii

Be 2205

CS=A+Bo vece "111222"가 된다-문자열 AA

CROASB 아아C= 333이된다.-수값0이 있으므로 수치 처리가 행해진다

'-' 연산자는 마이너스 값을 보여 주는 단항 연산자에도 사용한다. 한편 +는 플러스 값을
나타내는 단항 연산자는 아니다. 편집 화면에서 일부러 “A = A + +5"라고 입력하면 뒤의 +
는 에디터에 의해 삭제된다.

비교 연산자는 두 개의 연산자의 대소 관계와 등식 관계를 판정해서 정수와 허수값을

언
것이다(표 5-3), 정수와 허수값의 관계가 올바르면 참(수치 값의 표현이라면 -1), 바르지
다면 거짓(수치 값의 표현이라면 0)이 된다. Like 연산자와 Is 연산자는 다음 항목에서 설
하기로 한다.

of G2 cir

165


===== PAGE 164 =====
166

Chapter5 연산자

〈          작다                | A<B Then...

=         작거나 같다           | 4 < 8 then...

>          크다                A > 80 00160...

=         크거나 같다            | A= 6 Then ...

<          같지 않다             lf A <) B Then ...

=          같다                 84 = 68 60

Like       문자열의. 패턴이 일치함 lf FileA Like “* "dar  Then ...
is”        개체 변수 비교         If MyObj1 16 MyObj2 Then ...

Like 연산자

Liket: 특수한 패턴 지정 문자와 일치 여부를 비교하는 것이다. 용법은 다음과 같으며 문
자열이 지정한 패턴과 일치하는지를 판단한다.

If 문자열 Like 패턴 Then

패턴 지정은 다음과 같이 한다

pes: 배스 이여

패턴 지정 문자

?              임의의 한 문자

본                임의의 복수 문자

#               임의의 숫자 한 문지(0 9)

[charlist]        Charlisto| 지정했던 문자 중 어떤 한 문자
[!charlist]       charlistol 지정했던 문자 이외의 어떤 한 문자

Al) 영문 반가 문자와 한자가 SPH 한 문자로 판단된다. 단지 #는 반각 문자만이 일치한다.
42) *[A-EPELLSI ‘A’ ~ 2 까지의 아무거나 한 문자를 의미한다.
48) Option Compare 명령문어서 일치하는 문자를 설정할 수 있다.

Option Compare BinaryS 지정한 경우
If A Like “[A-C]” Then ...
ㅡ이것은 ‘A’ BC 와 비교된다.


===== PAGE 165 =====
Option Compare TextS 지정한 경우
If A Like “[A-C]” Then ...
이것은 44 a, B, b, C,c, A, a, B, b, C, c%} 비교된다.
즉 대문자/소문자, 전각/반각은 구별하지 않는다

입력 예 : If "aXc" Like 『2206" Then § -----참이 된다
If "2국6 Like "a?ce" Then wees참이 된다
If 16020" Like "a?c" Then 00000거짓이 된다
If "aBBBa" Like "ata" Then 22참이 된다
If "myfile.bas" Like "*.bas" Then ……참이 된다
If "D" Like "(A-E]" Then 2 owes참이 된다
If "D" Like "(!A-E]" Then 00000거짓이 된다
Tf "D" Like "(E-Z]" Then 2 2 2 ow거첫이 되다
If "abFgh" Like "ab[A-Z]gh" Then =참이 된다
08622" Like "a#a" Then 00009참이 된다
If "aba" Like "a#a" Then 2 ow거짓이 된다
If "BATPRROGRAM" Like "B?T*" Then ---:참이 된다
If "PATPRROGRAM" Like "B?T*" Then ---거짓이 된다

산자는 두 개의 개체 변수가 같은 개체를 지시하고 있는지를 조사한다. 양쪽
은 개체를 지정하고 있을 때에는 참이 된다. 이것은 0언어라면 단순한 포인트 비교

있는 것이다. 입력은 다음과 같이 한다.

If A 16 B Then ...

입력 에: Dim Obl As CommandButton
명령 버튼

고
건
flu
ba
디오
[에
+>
30
rr
re
>
(0)
=

Dim Ob2 As CommandButton

명령 버튼 개체를 기억할 +
Set Obl = 0000086001 명령 버튼 개체를 Commanc
Set Ob2 = Command1                 같은
If Obl Is Ob2 Then A = 1 Else A =    4

30

rir

묘
7
oO
12)
02

ㄱ
==
1

lo 010
os
2 [

bo
>
으
1ㅁ
Hu
>
0
호
iil
어

%닌

167


===== PAGE 166 =====
Chapter5 연산자

문자열 연결 연산자를 표 5-5에 나타낸다

HEI
(27
on

re
[수
>
미소
0묘
요

&        문자열을 연결한다        A = “ABC” & “def”
a         문자열을 연결한다        A = “ABC’ + “def”

예
Not        부정            lf Not C Then
And        논리합          lf AYB And C)D Then
Or         논리곱          lf 426 Or C)D Then
Xor        배타적 논리곱     lf AXB Xor C)D Then
Eqv       논리 등식        lf AYB Eqv C)D Then
Imp        논리 포함        lf AYB Imp C)D Then
논리 처리

논리 연산자는 정수와 허수의 값을 부정하거나 복수의 조건을 맞추는 것이다. 이 중에는
Not, And, 이 많이 사용된다. 세 가지의 연산자의 우위 순서가 높은 편이므로 기억해 두
는 것이 좋다. 각 연산자의 의미는 표 5-75} 같으며 다음과 같이 입력한다.

168


===== PAGE 167 =====
내 58 /

Not 연산자       식이 거짓이면 결과는 참

And 연산자      양쪽 모두 참이면 결과는 참

아연산자         한쪽이 참 또는 양쪽 모두 참이면 결과는 참

×0「연산자        한쪽이 참이면 결과는 참

60*연산자        양쪽 모두 참 또는 양쪽 모두 거짓일 때 결과는 참

100연산자        식1이 A 식2가 거짓일 때만 결과는 거짓

(이것은 식1이 식2를 암시적으로 포함한다라는 논리 연산)

논리 연산자는 비트 처리에도 사용된다 5-8), 이때는 아래와 같이 입력하여 수치값 A
와 수치값 BS 비트마다 And 처리한 결과를 (:에 넣는다.

C=AandB

대응하는 두 개의 비트에 대한 비트 연산 처리를 정리하면 다음의 표와 같다.

데이터 1 의 값                    Ob 1                       OOFF
메이터간의 값              08 | 06 제                OFFO
And                     9 09 0 1                OOFO
Or                       OFS Pee a                0
Xor                      0 10010                OFOF
Eqv                     30 001                FOFO
Imp                      182 0600 의                FFFO

169


===== PAGE 168 =====
Chapter5 연산자

하나의 식에서 복수의 연산자가 사용될 때에는 처리 순서가 결정되

“"1+2*8”이라면 “2*8”이 먼저 계산된다. 이와 같은 eS 우선
“(01+2)048”이라면 “1+2”가 먼저 계산된다, 이처럼 “( )”는 우선 순위를
한다. 또 다른 연산자가 함께 사용되고 있을 때에는 산술 연산자, 비교 연산자, 논리 연산자의
순서로 평가된다. 비교 연산자의 각 연산자의 우선 순위는 모두 같다. 따라서 식에서 복수의
비교 연산자가 지정되어 있는 경우 나타나는 순서대로 왼쪽에서 오른쪽으로 평가된다. 산술

연산자 및 논리 연산자는 표 5-9에 나타나는 순서로 평가된다.

산술 연산자         6                            우선순위 (높음)
\
Mod
Bee
&
비교 연산자         = <> < © > )= Like Is
논리 연산자        Not
And
Or
Xor
Eqv                               y
Imp                          우선 #4 (ks)

주) 같은 우선 순위의 연산자가 사용된다면 왼쪽에서 ORO} AMZ 평가된다(예를 들면 10/205" 9] 결과는 25

=

170


===== PAGE 169 =====
제어문

CHAPTER

이 장에서는 프로그램의 흐름을 바꾸는 제어문에 대해서 알아보기로

yee  BasicOl=

ce  무

 있다. 또 제어
|

, 6010 등은 가능한 사용하지 않는 편0

새롭고 편리한 제어문이 추가되어 있으므로 알

게 프로그램을 작성할 수 있다. 특히 00^Ｌ_000문은 강력한 SHS
문의 추가에 맞춰서 종래의 GoSub~Return,

좋은 문장이라고 여겨진다.



===== PAGE 170 =====
Chapter6 제어문

Visual Basic2

프로그램을 기본적으로 입력, 출력, 계산(과 대입)으로 Azle  하지만: 제어문은 그 의도한 순서
의 흐름을 바꾸는 역    ae 한다. Visual Basico] 준비되어 있는 제어문은 다음과 같다.

If Then Else             Do Until ~ Loop            On GoTo
Select Case              Do Loop ~ While            Stop
For Next                 Do Loop ~ Until            Call
While Wend               GoSub ~ Return             GoTo
Do While ~ Loop          On GoSub                   End

Exit Do; Exit For, Exit: Function, Rxit) Sub

If 문의 기본적인 동작은 조건에 근거한 두 방향으로 나누어진다. 또한 한 행으로 완결하는
If 문과 복수 행에 걸친 블록 Ｌ Bo] 있다,

      if 조건식 Then #1 Else 문2

:조건식이 참이면 문1을 실행한다. 거짓이면 HIS 실행한다
ㆍ Else 이하는 생략할 수 있다
ㆍ문1과 문2는 문 전체에서 한 행 이내로 해야 한다

       If 조건식 Then

문!

Else

Ad
NS)

End If

ㆍ 조건식이 참이면 문1을 실행한다. 거짓이면 BOS 실행하다
ㆍ 문1과 BIE 복수 행에 걸쳐서 쓸 수 있다
ㆍ Hse SH: 불필요하면 생략할 수 있지만 ‘End If 는 생략할 수 없다

172


===== PAGE 171 =====
If 조건식 ] Then
zl

Elself £0442 Then
#2

Elself 조건식ㅁ Then

=n
Else

=x
End If

*ㆍ만약 조건식1이 참이면 문1은 실행한다
그렇지 않고 조건식2가 Hol TIS 실행한다

그렇지 않고 조건식 no] 참이면 Ens 실행한다

그렇지 않으면 문*를 실행한다
+ Elselfte 필요한 만큼 쓸 수 있다

다음 예에서는, BS] 값은 555로 된다

6.3 Select Case 문

A=4
If A < 3 Then
B = 333
ElseIf A < 5 Then
B = 555
Else
B = 999
End Lf

적합한 Case SAS 실행한다. 프로그램이 다방향으

로 나누어질 때 If 문보다 깔 깔끔한 입력

173


===== PAGE 172 =====
Chapter6 제어문

(서식)      Select Case HAE 식

Case #1
문1

Case 식2
문2

Case 식ㅁ
=n
Case Else
zx
End Select

* 테스트 식에는
:식에는

테스트 식과 일치시키고

식을 평가하여 값이 어떤 값과 일치하면 그 블록으로 점프하여 처리한다

ㆍ 어떤 식에도 일치하지 않을
* Case Else= 불필요하면 생략할 수

ㆍ 0886식에는 다음과 같은 입력 방법이 있다

는

수식 또는 문자열 식을 입력한다
싶은 식을

입력한다

exe 실행한다
있다

Case 2 00000 이다 테스트 식의 값이 2라면
Case 3 To 5           … 3~52}H
Case 3,6,8 ……3.6.8이라면
Case Is < 5           …5미만이라면
Case 1 To 4, 6,8,9 «+복합 지정
Case "TV"            :문자열이 “TV 라면
Case "TV","RD" weve문자열이 “TV"L “RD” 2}
다음의 예에서는 AS] 값은 2314가 된다
A= 0
Yor Ｌㅋ=] 06 10
Select Case I
Case 2
A=A+ 10      한 번 실행한다
Case 3 06 5
A=A + 100           세 HH Alsi otc}
Case Is >= 9
A = A + 1000          = HH 실행한다
Case Else
A=A+1            '네 번 실행한다
End Select
Next

174


===== PAGE 173 =====
6.4 Fo #

Next 루프 변수

+ 루프 변수의 값이 초기값 ~ 최종값 사이에 루프 처리를 반복한다.
+ 루프때마다 같은 증가분만큼 증가한다.
ㆍ “Step 1 의 루프는 8[67구조를 생략할 수 있다.

A=0

For 1 = 1 To 10
A =A. + 1

Next

다음의 예에서는, AS 값은 55가 된다.
For 88애를 사용하면 배열과 콜렉션의 모든 요소에 대해 처리할 수 있다. 이것은 요소수

For Each 245 대입하는 변수 In 컬렉션 이후는 배열 변수

Next

Dim dt(10) As Integer, i As Integer, sum As Integer

Dim x
For 1 = 1 09 10
601). =a
Next
For Each x In dt             배열 0[의 BE 요소
sum = sum + x
Next
Debug.Print sum             '힙계값은 55
For Each x In Printers       ‘Printers 컬렉션의 모든 요소
Debug.Print x.DeviceName ‘0/2 가능한 프린터 이름을 모두 표시
Next

175


===== PAGE 174 =====
176

Chapter6 제어문

기  임의의 조건으로 For SS 종료시키고 싶을 때에는
NOTE     If 조건 Then Exit For

ari ge ele aT:            _
를 사용한다.  For....Next= 0681(상자) 구조로 할 수 있다.

os

While ...\600 는 부정 회수의

While ...Wenc

ise bb 문이다, While #2 조건을
그 결과가 참이라면 루프 처리를 한다. While 문의 조건식은 다음의 루프를 실행할 지에 대

먼저 판정해서

한 여부이고 식이 처음부터 거짓인 경우어 aie   번도 행하지 않는다. 문 중에서는 다음 루프
를 계속 판정하기 위하여 AAAS] 값을 변경하는 기술을 하는 것이 보통이다. S| Visual
28810에는 보다 고기능 422A] Do,..Loop it 사용하는 것이 훨씬 편리하다.

      while 조건식

므

~
Wend
ㆍ조건식이 BY 때 루프 처리를 반복한다
ㆍ조건식이 처음부터 거짓인 때는 문을 한 번도 실행하지 않는다

조건이 참인 때 또는 조건이 거짓이 될 때까지 처리를 반복한다. Do... Loop tS 사용하면 전

판정, 후판정과 사이 루프와 도달 루프도 자유 자재로 기술할 수 있고 루프 탈출도 할 수 있다.

     전판정/사이 루프
Do While 조건식

Loop



===== PAGE 175 =====
6.3 Do...Loop=

Ajo] 참인 동안 지금 행한 루프를 반복한다
식이 처음부터 거짓이라면 이 문은 한 번도 실행되지 않는다

조건
조건

Do Until 조건식
Loop

*조건식이 Zo] 될 때까지 다음의 루프 처리를 한

*조건식이 처음부터 참이라면 이 HS 한 번도 실행되지 않는다
1 While 조건식

+ BAA] 참인 동안 지금 행한 루프를 반복한다

*조건식이 처음부터 거짓이라도 이 문은 최저 1회는 심행된다

Do
oe Until 조건식
+ £240] 참이 될 때까지 지금 행한 루프를 반복한다
*조건식이 ASHE 참이라도 이 HE 최저 1회는 실행된다

다음 예에서는 어떤 것이라도 AS] 값이 1~4로 변화하고 BE 10이 된다.

60)    A=1: B= 0
Do While A< 5
그 = 3 +tA
A=A+1
Loop

®    A=1: B=0
Do Until A = 5
B=B+A
A=A+rt+1

Loop

177


===== PAGE 176 =====
Chapter6 제어문

@@)    A =-1:'B = 0
Do

B=B+HaA

A=A++1

®   A= 1: B= 0
Do

B= BA

A=A+1

Loop Until A = 5

임의의 조건에서 Do. .Loop#S 종료시키고 싶을 때에는,

lf ZH Then Exit Do

를 사용한다.
While 구와 Until 구는 생략할 수 있으며 이런 경우는 무한 루프가 되므로 6 00와 같이 사용하는 것
이 좋다.

Do

if 조건 Then Exit 20

Loop
Do .....LoopZ22 Nest(AtA}) PAS

nh
+>
32
i

Visual BasicOl= GoTo 문도 있다. 지정한 라벨까지 점프한다. GoTo 문은 프로그램을
어렵게 만들므로 별로 사용하지 않는다. 단지 프로그램 중에 특정한 장소에서 특정한 장소
지 일시적으로 8ㅁ7시키고 싶을 때에 사용하면 편리하다. 그러나 특별한 경우를 제외하고는
사용하지 않는 것이 좋다.

178


===== PAGE 177 =====
6.9 Exit =

   GoTo 라벨
+ Golo SS 대응하는 라벨의 쓰여진 위치에 제어를 이동시킨다.

GoTo Asoko -

Asoko: <q | apa 행의 앞에서 입력하고 가장 뒤에 “을 붙인다

*라벨은 같은 프로시저에서 해야만 한다.

“Stop 문을 실행하면 프로그램은 일시적으로 정지한다. 그 후 시작 루프가 되므로 Met Do
와 같이 사용된다.

Stop                  4104이 행에서 일시 중단한다
ding 조건 Then SCOP tates조건이 참이면 일시 중단한다

Exit= 프로시저와 Loop 제어로부터 탈출할 때에 사용한다.

Exit Do             Do..Lloop= 탈출한다

Exit For           For. .Next SES 탈출한다

Exit Sub            Sub BRAINS 탈출하여 호출 쪽으로 돌아간다
Exit Function        Function 프로시저를 탈출하여 호출 쪽으로 돌아간다
Exit Property        Property 프로시저를 탈출하여 호출 쪽으로 돌아간다

179


===== PAGE 178 =====
Chapter6 제어문

End: 각각의 기술 단위(프로시저와 블록)의 a 뒤에 입력하고 그 기술 단위가 종료하는
것을 나타낸다.

End                   프로그램을 종료시킨다

End Function           Function 프로시저를 종료시킨다
End If                           킨타

End Property                   로시저를 종료시킨다
End Select                       문을 종료시킨다

End Sub                Sub 프로시저를 종료시킨다

End Type                사용자 정의의 tye SS 종료시킨다
End With                 With 문을 종료시킨다

With HS 프로그램 기술을 간단히 하는 효과가 있어서 같은 개체명을 연속적으로 사용할

입력1:    Command1.Caption = 실행”
Command1.Enabled = True
Command1.Visible = True

입력2:     With Command1

.Caption = “실행”

-Enabled = True

-Visible = True
End With

180


===== PAGE 179 =====
6.12 그 외의 제어문(01, GoSub, On)

SA 베이직에서는 이하의 제어문도 자주 사용되었다. Visual 88810에서는 최신 제어
구조가 준비되어 이 문은 사용하지 않는다. 이것들은 과거의 베이직의 흔적으로 남아 있을 뿐

이다.
Call                   프로시저를 불러낸다
GoSub ~ Return        프로시저 내에 기술된 서브루틴을 불러낸다
On GoSub               식의 값에 의한 Gosub
On GoTo                 식의 값에 의한 GoTo

181


===== PAGE 180 =====
CHAPTER

프로시저 작성

이 장에서는 프로시저의 작성 방법에 대해서 알아보기로 한다. 종래의
ㅁ88610에는 서브루틴과 함수라는 루틴이 있었다. Visual ㅁ88810에서는
이것들을 정리한 AS 프로시저라고 부른다. 프로시저 중에는 Sub 프로
시저와 Function 프로시저가 중요하다. 자주 들어 보면 알겠지만 이벤
트 프로시저는 기능 구분상 Sub 프로시저의 하나이다.



===== PAGE 181 =====
Chapter7 프로시저 작성

트
해 주었다. 그러나 명령 버튼을 눌렀을 때 일을 시키는 구체적인 지시는 사용자가 프로시저 내
에 입력한다. 프로시저에는 아래와 같은 것들이 있다
806 프로시저            abs 되돌리지| 않는다(서브 루틴)
Function 프로시저         Gs 되돌린다
Property 프로시저      독자적인 프로퍼티를 작성한다

이 중에서 중요한 것은 Sub 프로시저와 Function 프로시저이다. Property 프로시저는
독자적인 프로시저를 작성할 때에 사용하며 표준 기능만으로도 문제가 되지 않을 경우에는 사
용하지 QFEc} Property BBAAE 특별한 용도에만 사용되며 이 책에서는 다루지 않는다.

Sub 프로시저의 정의
Sub 프로시저는 다음처럼 입력한다.

      [PrivatelPublic] [Static] Sub 프로시제(인수 나엘

End Sub

* Private/Public® & 중에서 하나만 붙인다. 생략하면 Public >] 된다

Private Sub Abc()     Private &
Public Sub Abc()      Public &
Sub Abc ()                  Public &

*단, 이벤트 프로시저는 16081 Basic 환경에서는 ES = Private 7} 추가된다

184


===== PAGE 182 =====
7.2 Sub 프로시저

Private Sub Command1_Click()

* Privates 붙이면 Sub 프로시저를 AMS 모듈 내에서만 참조할 수 있는 프로시저가 된다

*PublicS 붙이면 모든 모듈 내의 모든 프로시저로부터 참조할 수 있는 프로시저가 된다

* StaticS 붙이면 81 프로시저 Yo 선언된 로컬 변수가 모든 정적 변수가 된다. 변수 선
언이므로 818110은 지정할 필요가 없다

Private Static Sub Aaa()
Static Sub Bbb()

ㆍ인수는 데이터형과 변수명은 동시에 괄호 안에 쓴다
Sub Tst1()                             인수 없음
Sub Tst1(A As Integer)                 S817}
Sub Tst1(A As Integer, B As Integer)   인수2개
Sub Tst1(A, 2)                      형 지정이 없으면 영문

Sub 프로시저 호출                                 ;
Sub 프로시저를 호출하는 방법은 다음과 같다. Sub 프로시저를 호출할 때 보통 인수는 그
대로 쓴다. 7.5 인수를 넘겨 주는 방법에서 기술한 것처럼 인수는 “( )"로 둘러싸이면 특별한

의미가 되므로 주의하자.

Sub 프로시저명 [실인수 부르기]

ㆍ인수의 유)무는 다음처럼 기술한다

testl                          인수
A
A

test2 A,B                인

원주, 원 면적을 나타낸 프로그램을 다음의 프로그래밍에서 알아보자.

Private Sub Commandi_Click()

En_data 10                      '인수10으로 En_ datas 실행
End Sub
Sub En_data(R As Double)             ‘Cle RE Doubles

Dim C As Double                 AS HA 선언

Dim S As Double

C= 2 * 3.14159 = &             '원주의 계산

S=R *R * 3.14159              '원 면적의 계산

185


===== PAGE 183 =====
Chapter7 프로시저 작성

Print "반경"; R; 『 원주 a"; 이; "면적 ="; §
End Sub

Sub 프로시저 SSS 종래의 Basico] 남아 있는 CallZS 사용할 수도 있지만 위에 기술한 방법을 많
이 사용하다. Call EE 사용하면 다음과 같다.

Call En_data(10)           ‘Call Fn data= 실행

BA =v 에서 데이터 주고받기를 할 때 인수를 사용한다. 이때
반인수라고 부른다. 그것은 1 ao] 전달되는지 잘
로시저를 호출하는 측에서는 실제 데이터를 기술한 것

En_data 10                   “2194-10
En_data Dt                     '실인수 Dt
Sub En_data(R As Double)      ‘BrOlz R
End Sub

함수 프로시저의 정의

함수 프로시저는 다음처럼 기술한다

i

      [PrivatelPublic] [Static] Function 프로시저명 (인수 나열) [As 형]

본체 기술
프로시져 명=값                이것이 되돌린 같이 된다

End Function

186


===== PAGE 184 =====
* Private, Public, Static 용법은 Sub 프로시저와 같음
:인수 배열의 기술은 Sub 프로시저와 같음
:되돌린 값의 형은 48데이터 형으로 지정된다

Function Tstfunc1(A, B) As Integer     Integer S2| 값을 리턴한다
Function Tstfunc2(A, 2) As Long       1009형의 값을 리턴한다
Function Tstfunc3(A, B) As String     문자열형을 리턴한다
Function Tstfunc4 (A, B)              생략하면 SESS 리턴한다

ㆍ되돌린 값의 AVS 함수 명의 대입으로 이루어진다
Function Tstfuncl(A, B) As Integer

Tst funcl=X                     `이것에 리턴 값이 된다
End Function

함수 프로시저 호출
함수 프로시저는 다음처럼 호출하면 인수 배열을 “O'S 둘러싸는 것만 주의하자.

     매=함수 프로시저명(실인수 배열)

ㆍ 함수 프로시저는 공식 안에서 이루어진다. 즉 좌변의 함수에 뭔가를 대입하면 형과 문 등
의 조건식으로 사용된다

다음에 제시한 직각삼각형의 변의 길이를 바꾸는 프로그램을 보자(실제의 예를 제시한다).

Private Sub Command1_Click()

Dim X
X= Syahen(10, 10)      함수 불러오기
print X                ‘XE 14142122 핀다:
End Sub
Function Syahen(A, B)       ‘E|Sel Zt 인수에도 Variant
Dim ㅇ                   로컬 변수
@v=Ger (8 ^ 2402)    =
Syahen = C             `이것으로 되돌린 값이 된다.

End Function

187


===== PAGE 185 =====
Chapter7 프로시저 작성

이벤트 프로시저와 제너럴 프로시저
Visual Basic 의 프로시저는 Sub 와 Function 2] 구별 외에 또 다른 것이 있으며 그것은
다음과 같다.

또는 AEST 1대1로 대응하고 있는 프로시저로서 명령 HES 클릭할 때 동작
t

ㅎ
au

mule” of

6 ~  ㅋㅋ

이벤트 프로시저로부터 여러 번 불려지는 공통의 코드가 필요할 때가 있다. 그 공통
코드를 기술한 것이 제너럴 프로시저이다. 제너럴 프로시저라고 하면 뭔가 특별한
것저럼 들리지만 그 의미는 SSO 프로시전라는 것으로 예전의 일반 SSO 506 무
틴에 해당한다. 제너럴 프로시저는 이벤트 프로시저와는 달라서 다른 프로시저로부
El 호줄되지 않는 한 설행하는 일은 없다

새로운 제너럴 프로시저를 작성

이벤트 프로시저는 템플릿이 처음부터 준비되어 있으므로 해당 컨트롤을 더블
우     느

음처럼 조작한다.

(3) 무엇이라도 좋으므로 프로시저 편집 화면으로 해 둔다
© [삽입()]-[프로시저2)]을 클릭한다

(3) [이름04)] 텍스트 버튼에 프로시저명을 넣는다

© SHAE 모양임)에서“"3106”나 “Function” SS 하나

ru

AV OK

때

클릭한다

이것에서 지정한 이름의 프로시저 편집 화면이 표시된다.

il  이 메뉴 조작을 하지 않아도 임의의 프로시저 편집 화면으로 새로운 행에
NOTE     Private Sub Abc()

로 입력해 엔터를 누르면 그 순간에

  188|


===== PAGE 186 =====
7.4 프로시저의 신규 작성과 삭제

Private Sub Abc()
End Sub

라는 새로운 프로시저의 템플릿을 표시하므로 훨씬 간편하다.

폼 화면에서 임의의 컨트롤을 더블 클릭하면 편집 에디터로 이동하고 바탕을 더블 클릭하
면 폼의 프로시저 편집 에디터로 이동한다.

또 편집 화면에 뭔가가 있을 때에는 그 에디터 상부에 있는 드롭다운 메뉴로 개체명(예를 들

5s
면 Commandl)>} 이벤트명(예를 들면 Click)S 지정하면 해당 함수(예를 들면 Command,
Click())= 커서가 이동한다.

0 | Private Sub 00006001.011대()
Static Stwch
Static 대
If Stweh =  ~ 일 Then

TH = Tim
antl Text “=   "측정시작”
주 .70산 = Timer - 개 6 "초 경과"

600
;     Stwch = Not Stweh
End Sub.

Private Sub Command2_Click()
End

id Sub

@ 해당하는

프로시저에 커서가 이동한다

 불필요한 프로시저의 삭제                           —                   :

만약 어떤 프로시저가 불필요하다면 삭제할 필요가 있다. 불필요한 프로시저의 기술 부분
을 키 KA} PRG} 6009) 또는 마우스 조작으로 삭제하기만 하면 된다. Visual Basico] 프로
그램에서는 단지 에디터에서 입력되어 있는 문자열에 지나지 않으므로 그 문자열을 지우면 해
당하는 프로시저가 삭제된다.

189


===== PAGE 187 =====
Chapter7 프로시저 작성

참조에 의한 호출

Visual Basic2] 프로시저(81프로시저도 함수 프로시저도 같음)로 인수를 전달할 때
조에 의한 호출(2311 by 16[676ㅁ06)과 값에 의한 호출이 있다. Visual 88810은 표준으
조에 의한 SSS 사용한다. 이 방법은 어느 변수형과 배염을 사용해도 같은 크기(4바이
데이터를   같은 AQ 시간으로 전송     Ay, 61느 장점이 있다.

송알 T MUO
참조에 의한 호출은 호출한 함수 내
르

10 Hu clr
6 om! | od

주소를 건네 주고 프로시저 측에서는 그 받은

번수으                                   =
주소를 통해 목적의 값을 취함으로써 이루어진다. 또 BHAA 측에서 그 변수를 대입하면 같
은 FAS 참조하고 있으므로 불러내는 측의 변수값도 변한다(그림 7-2). 이것은 Sub 프로시
저에서도 인수를 사용해서 값을 되돌릴 수 있다는 것을 의미한다. 따라서 거꾸로 생각하면 보
통은 프로시저 측에서는 인수로 되어 있는 변수의 같을 변경하는 것을 기다린다는 것이 된다.
다음에 참조에 의한 호출 예를 보자
Private Sub Command1_Click()
Dim A As Integer
A = 123
116 "AL 81 즈
subtstl A              '변수4를 사용해서 참조 불러오기
Princ) 22 Si! oA
End Sub
Sub subtst1(X As Integer)
X=X*2              AX ZS 변경한다.
Print 게츠 조
End Sub

음은 이 프로그램의 실행 결과이다
Al = 123             Sosa
X = 246               프로시저
22 = 246              호출측 출

190


===== PAGE 188 =====
oa
[을
:
맑
:

크림 7-2
A=123               1000H A (=H A)O] 123을 대입
subtst1 A
10008 넘겨준다
                1000번지 |
+
Sub subtst1(X As Integer)                       # (246)
X=Xx2                                     :      ㆍ
ead Sub                       1000번지에 있는 1016961값을 2배로 한다

값에 의한 호출
호출측의 값이 변경할 수 있다는 것은 그 프로시저의 독립성이 낮다는 의미도 된다. 보통의
프로그램에서는 관계없지만 다시 호출하려는 프로그램에서는 문제가 될 수 있다.
Visual Basic] 값에 의한 호출(2811 by value)& 할 수 있다(그림 7-3). 인수값을
되돌리기 하면 그 변수를 복사하여 프로시저에 넘겨 준다. 프로시저 안에서는 넘겨받은 변
의 값을 변경해도 원래의 변수와는 관계가 없어진다(이것을 독립성이 높다고 한다). 값에
SSS 프로시저의 반 인수 선언에

를 붙인다. 다음은 값에 의한 호출의 예이다

=
벼스
Li Fi
의

Private Sub Command1_Click()
Dim A As Integer
A = 123
Princ “Ar =A
subtst2 A                   ‘HAAS 사용하여 참조 불러오기
Print "22 ="; 조
End Sub

Sub subtst2 (ByVal X As Integer)    ‘ByValS 붙인다.
Keone               변수×의 값을 변경한다.
22 1706 "에우; x

End Sub

191


===== PAGE 189 =====
Chapter7 프로시저 작성

= 123              호출측의 331
= 246:              프로시저의 출력
22 = 123              호출측의 출력3. ae 변하고 있지 않다.
그림 / 3
|           A=123
|          SubESt2 A

AS] 값을 복사하여 12322 넘겨준다.                  |

|                          +

Sub subtst2 (ByVal X As Integer)
X=Xx2 호출측의 A+ AS 관계없다.

End Sub

ByVal 2] 대응 키워드로서 참조에 의한 SSS 규제하는 ByRef7t 있다. 그러나 생략하면 ByRef 라고 간
주되므로 보통은 사용하는 일이 없다.

.식에 의한 값 넘겨주기

참조에 의한 호출인 프로시저에서도 인수로서 변수 아닌 식을 넘
fe}

의한 SSS 할 수 있다. 예를 들어 100이나 &+10이라는 식의 경우는 인수를 표현하는 주소
가 없으므로 값 넘겨주기로 여긴다. 또 변수만인 인수의 경우도 그것을 “()"로 둘러싸면 특별

히 식으로 인정된다.

전에 보여 주었던 참조에 의한 불러내기 4] subtstl& 값으로 불러내는 예를 보도록 하자.

SUBESEL 즈이 아사변수 aS 사용하여 AAO] 의한 호출(보통의 방법)
subtstl 200 = 재100이라는| 값에 의한 호출

subtstl 2+10 = …아2+10이라는 값에 의한 호출

subtstl (2) teAQ| 값에 의한 호출

보통은 인수를 "()"로 둘러싸지 않는다. 이것    을 함수 프로시저와 혼동해서
가 건네기가 되므로 주의하자. 함수 "()"부일 때와 Sub 프로시저로의 지
차이가 있으므로 구분할 수 있도록 익숙해지면 좋다.

subtstl (A)906 호출할 때에는 ‘( 의 좌측에 공백이 들어간다
B=functstl(A) 22함수 호출할 때에는 、('의 좌측에 공백이 들어간다

192


===== PAGE 190 =====
a
[은
땅

리턴 값을 얻기 위해 입력된 Sub 프로시저에서 인수에 "( )"를 붙이면 다음과 같이 부조화가 되므로 주
Note] 의해야 한다. 작동은 하지만 어디가 잘못되었는지 알지 못하는 경우도 있다.
sameproc sss문자열 변수 631에서 리턴 값을 얻을 + 있다
someproc (ssl) tes이렇게 하여도 SAS 하지만 값이 전달 되므로 문자열 변수
891의 리턴 값은 되지 않는다.

함수 프로시저의 불러오기도 기본적으로 사용된다. 값에 의한 SSA 때에는 ByvalS 사용한다. 또 참조
nore] 에 의한 SSS 기술된 함수에 대해 Alo] 의한 값을 전달할 때에는 다음처럼 입력한다.

2 = functstl(A) 00000 마마이것은 참조 넘겨주기가 된다.
2 = functstl((A)) 9s이렇게 하면 값 넘겨주기가 된다

사용자 정의형 넘겨주기
사용자 정의형의 인수를 건네는 경우도 특별한 조작이 아니다. Integer 1008이라는 키
워드 대신에 정의한 형의 이름을 사용하면 좋다. HLL 전에 언급한 골프형을 사용한 예를 보

도록 하자.

Type Golf                   ‘Sy Hee
Name As String             ‘OS
Keiken As Integer        ‘aa 년수
Handicap As Integer       핸디

End Type

그럼 /-4

Dim Player As Golf ㆍㆍㆍㆍㆍ 001『형 변수

Subtst3 Player
1 001*형 변수를 넘겨

다.

Ay

Sub Subtst3(A As Golf)

End Sub

193


===== PAGE 191 =====
Chapter7 프로시저 작성

붙인다. 프로시저에서 배열의

LBound (배열명, 차원)
배열의 인덱스 번호의 최소값을 바꾼다. 보통은 배열의 인덱스 최소값(기저)은 0이므로 이 함수
를 사용하지 않아도 된다. 차원을 생략하면 1

UBound (배열명. 차원)
배열의 인덱스 번호의 최대값을 바꾼다.

LBound/UBound?] 리턴 값을 조사한 예이다

Dim A(20), N
Dim B(0 To 10, 2 To 4)

= LBound(A, 1)                       ‘NS

N
N = LBound (A)               ‘N&O       생략하여도1)
N = LBound(B, 1)             ‘N20
N = LBound(B, 2)              ‘N22
N = UBound(A, 1)              ‘N20
N = UBound (A)                 ‘N220      (생략하여도1)
N = UBound(B, 1)              ‘N#10
N = UBound(B, 2)              ‘N=4

Private Sub Command1_Click()
Dim A(3) As Integer
(0) = 10: A(1) = 20: A@) = 30: A(3) = 40:

Print alladd(A\())               `배열&에서 불러오기. SSE 100으로 된다.
End Sub
Function Alladd(A() As Integer)    ‘IntegerHiS Sas 인수화한다

Dim I, Sum                지역 변수

Sum = 0                     '제로 클리어

For I = LBound(A) To UBound(A) ‘j=0 To 37} 22

Sum = Sum + A(I)            가신
Next
Alladd = Sum                ‘ae a 설정

End Function

194


===== PAGE 192 =====
컨트롤의

이 장에서는 Visual BasicS 실행하였
기본적인 컨트롤에 대해서 모두 설명호

ㄱㄱ CHAPTER

사용

을 경
명한다. Vis

우 도구 상자에 표시된
ual BasicS 활용한다는

것은 컨트롤을 제대로 사용한다는 것과 같다. 모든 컨트롤에 대해서 샘

플프로그램을 제시했으므

Mm

내용을 다루고 있으므로

로 비교해가며 익혀가자. 이 장은 가장 중요한

충분히 읽어서 사용 방

방법을 마스터해 보자.



===== PAGE 193 =====
196

Chapter 8

컨트롤의 사용

이미 설명했듯이 Visual BasieS 구성하는 것은 개체라는 단위이다. 개체에는
있다. 야플리케이션 전체가 하나의 개체이고
등도 하나의 개체이다.

가 포함되는 일이
폼 위에 배치된 명령 버튼

이 장에서 설명하는 것은 AEBSF
기 쉬운 개체라 할 수 있다. 한편 SE 컨트롤

이 장에서 설명하는 컨트롤은 그럼 8-1
에 SY} Ao] 표시된 기본 컨트롤로서 사용
로그램

하여 여러 가지의 프로

그림 8-1

보도롬 하자. 이것
도가 많아 중요하다. 이러한 기본 컨트롤을 사용

[프  j

= 개체
a. Wey 있는 폼도 개제이며 그

은 하나의 처리 단위로서 정리되어 있어 다루
과 같은 조작으로 다룰 수 있다,

은 Visual 88810을 실행할

iz

포인터

라벨(86060

프레임『「3106)

체크 #LA(CheckBox)
콤보 박스(2000608ㅁ800
수평 스크롤 4KHScrollBar)
타이머(11060)

디렉토리 리스트 YtA(DirListBox)
셰이프(31306)
0|0|A\(image)

OLE 컨테이너(2_ㅁ)

픽처 YtA(PictureBox)

텍스트 박스(161ㅁ80)

명령 4=(CommandButton)

옵션 버튼(26100ㅁ8400)

리스트 박스(16420)

수직 스크롤 4kKVScrollBar)
드라이브 리스트 YtA(DriveListBox)
파일 리스트 YtA(FileListBox)

선(106)

데이터[0813)

메뉴 편집기(도구 모음에 있는 HESS
[도구(1)1]-[메뉴편집기(\/)] 지정과 같음)



===== PAGE 194 =====
NOTE

8.1 기본 컨트롤 보기

Visual 28810에는 이것 이외에 고도의 기능 컨트롤이 많이 준비되어 있다.

이 장의 마지막에는 메뉴 작성에 대해서 설명한다. 메뉴는 애플리케이션의 위에 표시되므
로 좀더 본격적인 프로그램을 만들고 싶다면 꼭 사용하여야 한다.

=

샘플 프로그램에 대해서

다음 샘플 프로그램부터는 .160 파일을 사용하고 있다(.60ㅁ와 .\71도 같음). 이러한 파일들의 대부분은
Visual ㅁ88910에 부속되어 있다. Visual Basic2 인스톨할 때 이 파일 사용 OFS 선택해 주어야 하며
어느 폴더를 사용할 것인지에 대하여 사용자가 임의로 설정할 수 있다. 하지만 어떠한 방법으로 Visual
BasicS 인스톨한 경우도 그 중에

\icons
\bitmaps
\metafile
라는 폴더가 있어 여러 가지 화면 라이브러리가 포함된다.
예를 들면 다음에 있을지도 모른다.
C:\Program Files\Microsoft Visual Studio\Common\Graphics\Icons

\Computer\w95mbx01.ico
C:\Program Files\VB6\Common\Graphics\lcons\Computer\w95mbx01.ico

197


===== PAGE 195 =====
Chapter8 HE=9| 사용

메뉴 바 아이콘                                  속성 창
폼 표시
ix Form!                                                             T     ef
13 -복사펜
"0 - 단색
=          2                                           HelpC    10 0
오른쪽 속성 창에 제시한 속성 이외에도 다음의 것이           ee 이00
eyPreview   alse
Left     “0
있어 코드 중에서 사용할 수 있다.                                   LinkMode 0
LinkTopic   Form
| {MaxButton   True
5                            ;                               : MDIChild    False
ActiveControl          FontSize                            |MinButton 7148
Mouselcon (SiS)
Controls                FontStrikethru
Count                    FontUnderline
CurrentX                hDC
CurrentY                hWnd
FontBold                Image
FontItalic                               StartUpObject
FontName

이것 이외에 속성 창의 (이름)과 같은 Name 449°] 있다. 이름은 어느 컨트롤에도 있으나
찌82086에 대해서는 생략된다.

198


===== PAGE 196 =====
8.2 &(Form)

Click
DbIClick
Deactivate

DragOver
GotFocus
initialize
eyDown
eyPress
eyUp
LinkClose
준비되어 있는 메서드
200                   Point                 ScaleYy
Circle               PopupMenu            SetFocus
Cls                   Print                 Show
Hide                  PrintForm            TextHeight
Line                  PSet                         TextWidth
Move                  Refresh              WhatsThisMode
OLEDrag              Scale                 ZOrder

PaintPicture                 Scalex

= sas 여러 가지 age 배치하는 7} 되는 것으로 애플리케ㅇ Vag 4
관계되는 윈도우(또는 다이얼로그 박스)가 된다. 폼의 속성을 설정하면 위치, 크기, 색상 등을

결정하거나 크기를 변경할 수 있다. 폼은 작은 S(MDI 작은 폼)을 가질 수 있다.

나 컨트롤과 같이  a 메서드를 갖고 있고 From 1.0830는 실행할 때 폼을 클

릭하면 무슨 처리를 할지 혹은 폼의 위치와 크기를 변경하는 SCE 작성할 수 있다.

폼의 중요한 이벤트 프로  시 저에는   Kom _Load7} 있다, Form Load: 실행할 때 제일 4
음 불러진 프로시저이다. 폼을 더블 클릭하면 1000 1.080의 코드 에디터가 출력된다.

폼의 중요 속성은 표 8-1에 제시한 바와 같다.

199


===== PAGE 197 =====
200

Chapter 8

컨트롤의 사용

기능
BorderStyle     O~d            BANe| AAS 정한다
ControlBox      True / False      컨트롤 메뉴 바를 표시/비 표시
Caption         텍스트           폼의 제목 표시 문자열
MaxButton       True # False      최대화 HE 유효/무효
MinButton       True / False      최소화 HE 유효/무효
WindowState    0 - HE          실행시에 보통 창을 표시

1 - 최소화       실행시에 작업 표시 줄에 표시

2 - 죄대화       실행시에 최대 화면 표시
Icon           (아이콘)          화면 왼쪽 위에 표시하는 아이콘을 지정
Name          텍스트           폼 식별 SS 설정한다

#2 BorderStyle $32 설정하여 경
Button/MinButton 2] 값을 연동해서 변경하

0-없음           틀이 없다
ㅣ 고정(설수)         창의 크기를 고정한다

최대화 최소화 버튼을 표시할 수 있다
2 가변            장의 크기를 변경 Its

최대화 최소화 버튼을 표시할 수 있다
3-고정 다이얼로그 창의 크기를 고정한다.
최대화 최소화 버튼을 표시할 수 없
요

4-고정 를 원도우 컨트롤 메뉴 YAS 표시하지 않는다
타이틀명과 미니사이즈의 닫는 버튼만을 표시
5-를 윈도우        컨트롤 메뉴 박스를 표시하지 않는다

타이틀명과 미니사이즈의 닫는 버튼만을 표시
실행하였을 때 타이틀 바에 표시되지 않는다
네 변의 드래그로 큰기를 변경할 수 있다



===== PAGE 198 =====
8.3 포인트

화면2 [ControlBox]0l] False= 했다

화면3 [MaxButton]S False= 했다

화면4 Icon\graphics\icons\fregs\Figskor.ico= 했다

포                 니라 Visual Basic 환경 내에서의 여러 가지 조작을 한다. 포인트
Eo 컨트롤 HES 클릭하여 모양을 변경하여 포인트로 되돌리는 등에 사용한다.

인트는 컨트롤이 아

201


===== PAGE 199 =====
Chapter8 HE=9| 사용

명령 버튼 아이콘

폼 표시

속성 창에 제시된 속성 이외에도 다음의 것이 있으며
코드 내에서 사용할 수 있

Container            FontUnderline

FontBold             ForeColor

FontItalic           hwnd

FontName             Parent

FontSize             Value

FontStrikethru

준비되어 있는 이벤트

Command!
True
False

테다

ragDrop
DragOver
GotFocus
eyDown
es

Nereus
MouseDown
MouseMave

MouseUp
OLECompleteDrag

202



===== PAGE 200 =====
8.4 명령 Y=(CommandButton)

준비되어 있는 메서드

Drag                                       Refresh                              ShowwhatsThis
Move                                   SetFocus                         ZOrder
OLEDrag

처리를 시작하거나 중단 또는 종료시킬 때 사용되고 또한 복수
우 선택도 할 수 있다.

튼은 점선 사각 틀로 둘러싸여져 있다. 이 상태로 00해를 누르면 클

098에 의한 포커스 이동
TabStop 속성을 True® 하면 090으로 포커스를 이동하고 다음 버튼에 점선 사각 틀이 표시

폼 상에 명령 버튼이 복수이고 BAAS 갖지 않은 상태로 Hels 누르면 Default= 설정된 버
Eo] 선택된다. 이것은 2603411 속성을 'ㅠ06로 설정한다.

를 누를 때에 언제라도 선택되는 버튼으로 03006! 속성을 Truck 설정한다. 디폴트 취소
HES Caption 속성(즉 버튼의 제목)을 “취소"라고 설정하는 것이 보통이다.

속성 기능은 표 8-3] 정리해 제시한다.

AS
Cancel    True/False (scl 디폴트 취소 버튼 선택
하나의 명령 버튼만이 True= 된다

Default    True/False BHAS 갖지 않았을 때에 Gee 디폴트 버튼 선택
한 개의 명령 버튼만이 True= 된다
TapStop True/False  0098으로 포커스가 이동할지를 설정
주) 0011061과 26[01411는 여러 버튼 중 하나만이 True 된다. 즉 아무거나 하나를 1146로 하면 다른 버튼
은 자동으로 『0186가 된다.

203


===== PAGE 201 =====
Chapter8 컨트롤의 사용

떠풀턴로트램

명령 버튼의 기능을 확인하는 프로그램이다. ied, Be), 096의 클릭도 판단한다.

속성 설정

개체           sa           aa
Command1         Cancel           False
Caption          "Nomal"
Default          False
TabStop          True
Command2         Cancel           False
Caption          "Default"
Default          True
TabStop          True
Command3         Cancel           True
Caption          "Escape"
Default          False
TabStop          False
Text1            TabStop         False
코드

Private Sub Command1_Click()
Text1l.Text = "NORM"
End Sub

Private Sub Command2_Click()
Textl.Text = "DEF"
End Sub

Private Sub Command3_Click()
Textl.Text = "ESC"
End Sub

Private Sub Text1_Click()

Textl.Text = ""
End Sub

204


===== PAGE 202 =====
8.4 명령 버튼(0100018110ㅁ2400)

동작의 확인                .
0 Normal, Default, Escape FES 클릭하면 “NORM”, “DEF”, "08@^라고 표시된다.
(3) 텍스트 YAS 클릭하면 내용이 지워진다.
@ 텍스트 박스가 선택상태로 \해를 누르면 “DEP S 표시된다.

@ (sc]S 누르면 “ESC” 7} 표시된다.
© ffab)S 누르면 Normal, 1006}3411 버튼으로 포커스가 옮겨진다.

“NOTE

이 장의 샘플 프로그램에서는 가능한 한 간단한 예를 보여 주기 위해서 종료 WES 사용하지 않았다. 종
료시키려면 실행중인 애플리케이션 화면 우측 위의 ad HES 클릭하거나 디버그용 도구 모음에 있는 종
료 HES 클릭한다. 본래의 애플리케이션 APS 독자적인 종료 HES 폼 Aol 배치하거나 [종료] 메뉴를
준비하는 것이 보통이다. 종료 버튼의 실례에 대해서는 2장에서 작성한 인사 프로그램을 참조하도록 하자.

205


===== PAGE 203 =====
Chapter 8

206

컨트롤의 사용

라벨 아이콘                                     속성 창
= 표시                                       jLabell Label

‘Labell

0- 왼쪽 맞출
1-39

오른쪽 속                                                 것이
있으며 코드
Container                       FontSize
DataChanged                   FontStrikethru
FontBold                         FontUnderline
FontItalic                      Parent
FontName

준비되어 있는 이벤트

MouseMove
louseUp

2895
False

준비되어 있는 메서드
Drag                                 LinkSend                         ShowwhatsThis
LinkExecute                   Move                                  ZOrder
LinkPoke                            OLEDrag
LinkRequest                     Refresh



===== PAGE 204 =====
8.5 라벨(306)

라벨은 Caption 속성에 AACE 텍스트를 BAH 기능만을 가지고 있으며 애플리케이션
실행시에 사용자가 입력하여 변경할 수는 없다. 입력하여 변경하고 싶을 때에는 텍스트 박스
를 사용한다.

라벨은 틀 BAS 할 수도 있지만 보통은 문자열만 Sol] 표시한다. 이를 위해 작업의 경과
를 설명하거나, 텍스트 박스와 Ze Caption SAS 갖지 않는 컨트롤의 제목 BAS 위해서
사용된다.

AutoSize SAS '7146로 하면 표시하는 문자열에 따라서 크기가 변경된다. 또
WordWrap 속성을 True = 해 주면 문자열이 긴 경우 vs   ~ 후 위 아래 방향으로 문
에 적합하게 라벨의 크기를 자동으로 조절해 준다. 이 7                면 짧은 BAGS 복수 행
으로 표시 시킬 수     있다  또 ened 속성에서 S %   }태름 설정할 수 수 있다.

이 속성으

AutoSize    True/False HAO 맞춰서 자동으로 라벨의 크기가 변경

된다
BorderStyle 0 - 없음      Be 없고 문자만이 표시된다
베레 의서      움 파인 형태의 틀이 표시된다

WordWrap _True/False 단어 복수 HS 허용하거나 하지 않는다

음은 복수 행 표시의 예이다. WordWarp 속성을 True = 해 두자.

예1 : Caption 속성 문자열 “TRUE AND FALSE”

FALSE    <= ‘FALSE 다음
행이 되었다. 이것

ia  4
[때
ry 끼
og
10
Hu
On”
k
ee
iia

예2 : Caption 속성 문자열 “TRUE    AND    FALSE”

TRUE
AND     <— Sts 많이 널어 다음 행으로 보내기를 했다. 이것으로 원
FALSE        하는 대로 SA 행 표시를 할 수 있다

207


===== PAGE 205 =====
208

Chapter 8

컨트롤의 사용

Keele

복수 행의 표시와 BorderStyleS 실선으로 한

—&
때
고
>
rch
a

속성 설정
Labell     Caption           "EO! 사용 방법"
BorderStyle        0 -|없음
WordWrap          False
Label2    Caption           "이것은 복수행 표의 gy"
BorderStyle        0 없음
WordWrap          True
Label3    Caption           "OIS2 BorderStyle WHOS 했다."
BorderStyle       1-44
WordWrap          False
코드
없음
동작의 확인
(1) 텍스트 표시 결과를 확인한다



===== PAGE 206 =====
8.6 텍스트 YtA(TextBox)

텍스트 박스 아이콘           .                     속성 창

폼 표시

~

Container                       FontUnderline
DataChanged                   hwnd

FontBold                         Parent
FontItalic                      SelLength
FontName                          SelStart
FontSize                         SelText
FontStrikethru

준비되어 있는 이벤트

209


===== PAGE 207 =====
210

Chapter 8

컨트롤의 사용

준비되어 있는 메서드

Drag                      LinkSend                 SetFocus
LinkExecute             Move                      ShowwhatsThis
LinkPoke                 OLEDrag                  ZOrder
LinkRequest             Refresh
 설명                   |
텍스트의 입력과 표시를 하는 것으로 많이 사용되는 텍스트 박스의 표시는 Text 속성 외에
도 프로그램에서도 할 수 있다. 프로그램에서 표시할 경우는 다음과 같다.

Text1.Text = "abc"

또 실행시에는 텍스트 박스에 한 문자를 입력할 때마다 문자열이 Text 속성에 넣어 둔다.

텍스트 박스에서 중요한   이벤트  에  Change 2} KeyPress 7} 있 fo} fe) 으며 0018086는 텍 텍스트 박
스의 내용이 변경되면(뭔가 입력하면) 작동된다. 또 Keypress: 한 문자를 입력할 때마다 작
동되고 이때 입력한 문자 BES KeyAscii ol] 저장된다. 이때 KeyPress 이벤트 프로시저 중
에서 "《67&8011=0"라고 기술하면 입력이 없었던 것으로 할 수 있다. 이것은 어떤 문자를 입
력 금지하는 효과가 발생한다.

MultiLine 속성을 True = 하면 입력한 문자열이 오른쪽 끝에 위치하면 자동으로 SS 바
꾸어서 복수 행 표시가 된다. 이 때 ore 자동적으로 실행된다. 또 0@를 임비하면
AXA 줄 바꿈을 한다. 또 이때 코드 기술을 복수 행으로 표시할 때에는

Text1l.Text = "최초 행"& Chr(13) & Chr(10) & "다음 aq”

이라고 한다. 다시 SS 바꾸고자 할 때에는 복귀와 S 바꿈이라는 두 개의 지정이 필요하다.

MultiLine 속성을 18186 로 하면 입력한 문자열이 우측 끝에 위치하면 자동으로 가로로 스
크롤이 되고 빈 곳까지 한 행을 표시한다. 스크롤로 볼 수 없었던 문자열은 지워질 수 없고 더

, 너로 커서를 이동하면 표시된다. 또 한 행을 표시할 때에는 60@를 누르면 삐- 소리가 울리
며 이때 다시 입력할 수 있다.

ㅇ0)
^
ScrollBar 속성을 사용하면 스크롤 바 HAS 할 수 있다. 설정은

0 - 없음
1 - 수평
2 - 수직
3 - 양쪽


===== PAGE 208 =====
8.6 텍스트 YtA(TextBox)

중에서 선택한다. 스크롤 바 표시를 할 호. MultiLine & 을 True= 해 둔다. 4 수평 스크
바를 생성시킬 때에는                         =e                   Al 상태가 된다.

Locked $42 True = 하면 문자열      을 임력해 변경할 수     없는(표시하는 것만) 텍스트
스가 된다.                 |

텍스트 박스로 문자열 입력과 복사 처리를 한다.

니풀버로틴램

속성 설정

때

프

개체            속성               설정
Text           MultiLine          False
     ScrollBars         6 - 없음
Text2           MultiLine          False
ScroliBars          0 - 없음
Text3           MultiLine          False
ScrollBars         0 - RS
Text4           MultiLine          True
ScrollBars          2 - 수직
Commandi       Caption             "복자 34"
코드

BASS 1-4로 복사
Private Sub Text1_Change()

Text4.Text = Text1.Text
End Sub

'경고음을 제거한다.
Private Sub Textl_KeyPress(KeyAscii As Integer)
If KeyAscii = 13 Then KeyAscii = 0   '경고음 제거
End Sub
부터 문자열을 2-4로 복사, 숫자 입력을 무효로 한다.
Private Sub Text2_KeyPress (KeyAscii As Integer)
If KeyAscii = 13 Then
KeyAscii = 0        '경고음 제거
Text4.Text = Text2.Text
ElseIf Asc("0") <= KeyAscii And KeyAscii <= Asc("9") Then
KeyAscii = 0        '숫자이면
Beep
End If

211


===== PAGE 209 =====
Chapter8 컨트롤의 사용

End Sub

 포커스 이동
Private Sub Text3_KeyPress(KeyAscii As Integer)
If KeyAscii = 13 Then                    |

KeyAscii = 0         '경고음 제거
Command1 . SetFocus     '포커스 명령 버튼으로 이동
End If             :
End Sub

‘BASS 3-42 SA
Private Sub Command1_Click()

Text4.Text = Text3.Text
End Sub

동작의 확인
© [Texti]o] 입력하면 Text4 로 복사된다.
@ [Text2]o] 입력하고 뼈빼를 눌렀을 때 Text4 로 복사된다.
@ [Text2] A= 수직 입력은 할 수 없다(경고음이 울린다).
@ [Text3]o] 입력해서 뻐해를 누르면 복사 34 버튼에 포커스가 이동한다(틀 표시된다.)
여기서 한번 더 Ente] S 누르면 문자열이 3-+4 로 복사된다.
© 복사 34 버튼을 클릭하면 언제나 BAS] 83-4 로 복사된다.
© [Text4= 수직 스크롤 바가 표시되었다. 점점 BS 바꿔가며 메뉴가 표시된다.

212


===== PAGE 210 =====
8.7 이미지!00306@)

규정

이미지 아이콘                                      속성 창

image! Image                   |

3           Cen

Container                        Parent                                        |        |  Whats ThisHeloc
|             WWidtl
DataChanged

준비되어 있는 이벤트

준비되어 있는 메서드
Drag                                 OLEDrag                           ShowwhatsThis
Move                                 Refresh                           ZOrder

213



===== PAGE 211 =====
Chapter8 컨트롤의 사용

건     SEE a

이피지는 그림 bmp, :  ico, .wmnf 등)을 표시하는 컨트롤로 011 이벤트를 갖고 있으므로
명령 버튼처럼 표시된 그림을 수보 처리할 수 있다.
이미지 컨트롤의 선택 영역과 로드하는 그림의 크기가 다른 BPE Stretch 속성을 사용해서

컨트롤 크기에 맞춘다

Stretch = True        그림을 7
롤 크기를 그림의 크기에 맞춘다

Stretch = False                 컨트

라고 설정할 수 있다. 그림을 컨트롤 크기에 맞추어 처리하면 전 화면의 가로와 세로의 비율

도 변하므로 주의해야 한다. Stretch 저리가 귀찮을 때는 다음에 설명하는 픽처 박스를 사용
는 것이 훨씬 편리하다.

이미지 컨트롤은 픽처 박스 컨트롤보다 메모리 사용이 작고 속도가 빠르지만 그 반면에 기
능이 한정되어 있다.
그림 파일의 설정 방법

이미지 컨트롤에 그림 파일의 지정하는 방법에는 다음 세 가지가 있다.
(1 ) 디자인시 설 설정

설계할 때 속성 창에 2106076 속성값으로 파일명을 지정한다.
(2) 함수로 로드

실행할 때 LoadPicture HS 사용해서 다음처럼 설정한다.

Imagel.Picture = LoadPicture (“파일명”)

(3) SAt

실행할 때 이미 있는 그림 정보를 아래와 같은 방법으로 복사한다.

Image2.Picture = Imagel.Picture

그림 파일 삭제

표시되어 있는 그림을 삭제할 때에는 LoadPicture HES 인수 없이 사용한다.

다음처럼 기술하면 삭제된다.

Imagel.Picture = LoadPicture()

이미지 HESS HEAR 사용

이미지 AES? Click MES 갖고 있으므로 아이콘을 표시해서 명령 버튼처럼 사용할

다. 단지 명령 버튼처럼 눌러진 상태로 할 수 없으므로 30006781716 속성으로 경계선
정한다. 이 44 MouseDown, MouseUp 이벤트 내에서 기술한다.

ju +>
me *o

uo
ㅜ

녀

214


===== PAGE 212 =====
8.7 O|O/Al(image)

BorderStyle = 0 - 없음
BorderStyle = 1 - 실선

[니풀녀로틴램

Stretch=True(Sol] 맞춘다)와 Stretch=False( 13] 맞춘다)의 예와 이미지 컨트롤에
BES 이미지를 명령 버튼처럼 사용하는 oS 표시한다. 실제에서 이 기능은 화면상에 일례
로 복수 이미지를 배열하여 도구 모음처럼 사용하면 좋다.

속성 설정

Image         Stretch      True
Image2         Stretch      False
Image3         Stretch      False
Picture       ico HAS 지정한다
Command     Caption     '틀에 마추기"
Command2     Caption      ‘130 OF 7)"
코드

' .606 파일을 이미지1에 로드한다
Private Sub Command1_Click()

Imagel.Picture = LoadPicture("c:\mydata\house.bmp")
End Sub

'.bmp 파일을 Image2 o| 로드한다

Private Sub Command2_Click()                     :
Image2.Picture = LoadPicture("c:\mydata\house.bmp")

End Sub

‘Imagel 과 Image2 SB 지운다
Private Sub Image3_Click()
Imagel.Picture = LoadPicture("")
Image2.Picture = LoadPicture("")
End Sub
'마우스로 클릭(누른 상태)의 경우 SS 표시한다
Private Sub Image3_MouseDown (Button As Integer, Shift As_
integer, X As Single, Y As Single)
Image3.BorderStyle = 1
End Sub

215



===== PAGE 213 =====
Chapter8 컨트롤의 사용

'마우스 버튼을 놓으면 틀을 제거한다
Private Sub Image3_MouseUp(Button As Integer, Shift As_
integer, X As Single, Y As Single)
Image3 .BorderStyle = 0
End Sub

주) LoadPicture 에서 지정하는 bmp 그립은 사용자 자신의 디스크의 파일에서 지정해야 한다.

동작의 확인
(0) "“틀에 맞추기"”라는 HES 클릭하면 이미지1의 그림이 표시된다.
(3) So] 맞춰지기 위하여 그림이 세로로 넓혀져 있다.
@ “AA 맞추기"라는 HES 클릭하면 이미지2의 그림이 표시된다.
® 그림에 맞춰지게 하기 위하여 초기의 사이즈보다 크게 되어 있다.
© 이미지 3DYS 클릭하면 그림이 사라진다.

216


===== PAGE 214 =====
8.7 0|O|Al(Image)

EERE core vgect

화면1 디자인시의 이미지 크기

럼          Image27} 커졌다

세로로 늘어

ae

그
화면3 103063을 클릭해서 삭제

217


===== PAGE 215 =====
Chapter8 컨트롤의 사용

픽처 박스 아이콘                                 속성 창

폼 표시

Appearance ㅣ-30
AutoRedraw False
AutoSize
‘{BackColor
BorderStyle 1
CausesValidati 1046
‘{ClipControls = True
_ (DataField

| DataFormat
DataMember

| {DataSource
{Draglcon

Container                       FontSize

CurrentX                            FontStrikethru                                                      ro
CurrentYy                                  FontUnderline                                                                     를 &H8000001¢
DataChanged                HDC                                                 ight     겨
FontBold                            hwnd

FontItalic                       Image

FontName                            Parent

218


===== PAGE 216 =====
8.8 픽처 박스(기어+6ㅁ80)

준비되어 있는 메서드

Circle                             Move                                  Scalex

Cls                                    OLEDrag                           ScaleYy

Drag                                 PaintPicture                 SetFocus

Line                                  Point                                ShowwhatsThis
LinkExecute                   Print                               TextHeight
LinkPoke                         PSet                                 TextWidth
LinkRequest                   Refresh                           ZOrder
LinkSend                         Scale

=  ae SESS Se aR CS ne noennserereEe moteacir coor oer em

픽처 박스는 그림과 문자를 표시하는 것으로 이미지 AEST} 비슷하지만 그림 표시 이외
에 Circle 4} Line 메서드를 이용하여 간단한 도형을 작성하거나 22171 메서드로 문자를 표시
하는 부가 기능이 있다.

표시된 그림이 설정된 영역보다 클 때에는 초과한 부분은 표시되지 않으며 AutoSize 속성
을 1706로 설정하면 표시하는 그림의 크기에 맞춰서 컨트롤의 크기가 자동으로 변경된다.

픽처 박스 컨트롤의 내부에 다른 컨트롤을 배치하거나 텍스트 박스, 라벨, 이미지, 옵션 버
=, 체크 박스 SS 배치할 수 있다. TASS 컨테이너화되었으므로 배치한 컨트롤은 픽처 박
AS 이동하면 일괄적으로 이동한다. 또 배치된 옵션 HES 그룹화되었으므로 폼 상에서 별
개의 옵션 버튼과 구별할 수 있다.
픽처 박스의 표시

픽처 박스로 데이터 표시는 다음처럼 한다.
(0 그림(.100, .bmp, .wmf) 파일의 표시

방법 ㅣ: 디자인시 Picture 속성에 파일을 지정

방법2 : 코드에 다음처럼 기술

Picturel.Picture = 1402021002ㅇ(“파일명”)
@ 그림                                                                                                              .
Circle +} Line 메서드를 사용한다.

08) 텍스트 SF

Print 메서드를 사용한다. 문자 $12) CurrentX. CurrentY 속성을 사용한다. 이 위치 결정
단위에는 twipS 사용한다(다음에 나오는 Note 참조).

219


===== PAGE 217 =====
220

Chapter 8

컨트롤의 사용

픽처 박스 제거
픽처 박스 내를 제거할 때에는 다음처럼 한다. 우선 그림 파일의 삭제는 다음과 같이 한다.

Picturel.Picture = LoadPicture()

이때에는 제작 그림의 데이터와 문자도 동시에 사라진다. 또 Circle 등의 제작 그림과 Print of
의한 문자 표시는 아래의 입력한 방법으로 지운다.

Picture.Cls

AutoRedraw Oll 의해 다시 그림 그리기

폼과 픽처 박스는 AutoRedraw 속성을 갖고 있다. AutoRedraw 를 True 로 하면 자동으로 다
시 그림을 그린다. 예를 들면 01706, Cls, Line, Print, PSet 2] 그래픽 메서드에서 그려진 데이
터가 있다고 가정하자. 실행할 때에는 MEPS 최소화하고 또 앞으로 복원할 경우, 혹은 실행할
때 다른 윈도우를 일단 위에 겹쳐서 또 다른 곳으로 옮겨서 볼러올 때,

AutoRedraw7} True?®] 경우 그림이 재현된다
AutoRedraw7} False®] 경우 -그림은 없어진다

는 동작이 된다. 이것은 AutoRedraw 7} TrueY 때 그림을 메모리에 저장하며, 19186 일 때는
그림을 그린 것만으로 되어 있기 때문에 그림은 사라진다.

AutoRedrawt 실행할 때 새로 바꿀 수도 있다. 이것은 자동 그림 그리기 속성과 함께 018메
서드에 영향을 주는 것으로 다음 예처럼 작용한다.

Picturel.AutoRedraw = True
Picturel.Print "True 이 다 "        |
Picturel.AutoRedraw = False
Picturel.Print "False 이 다"       |
Picturel.Cls

이 프로그램을 실행하면 “1746이다"는 지워지지 않는다(애경의 UHRA 취급된다). 즉,

AutoRedraw & False = 해서 018 를 실행하면 1706 일 때에 출력된 그림은 지워지지 않는다는
것이다. 이것은 048를 두 종류로 나누어 사용할 수 있는 것을 말한다.


===== PAGE 218 =====
8.8 픽처 YtA(PictureBox)

샘|그프더그닌

속성 설정
개체            속성              설정
Picture        BorderStyle        1 - Aa
AutoSize          False
AutoRedraw       True
Command}      Caption           "화상"
Command2      Caption           ` 원-그럼"
Command3      Caption           "텍스트"
코드

Private Sub Command1_Click()
Picturel.Picture = LoadPicture("c:\mydata\picture.bmp")
End Sub

Private Sub Command2_Click()
Picturel.Picture = LoadPicture()      (그림 체개
For 1 = 100 60 500 86600 100          :
Picturel.circte (2000, 1000), 1 (HS 그림
Next
End Sub

Private Sub Command3_Click()
Picturel.Picture = LoadPicture()      Cah 제거
Picturel.CurrentX = 1000                       '로케이드
Picturel.CurrentY = 500

Picturel.Print "오늘은"            문자열 출력
End Sub
동작의 확인

© 화상 HES 클릭하면 그림이 표시된다.
© 원 그림 HES 클릭하면 동심원이 그려진다.
@ 텍스트 HES 클릭하면 문자열이 표시된다.

Visual Basic & age ‘wip 이라는   단위로 표현한다. Picturet, CurrentX=10002 가로로 1000twip
Nore} 이라는 의미이다. ttwip2 프린터 폰트의 크기의 단위인 1포인트의 1/20 이다. £ icme= 567twip,1 2!
RIE 1440twip 이 된다. twipS 좌표에 관한 t 설명    은 좌표와 단위를 보자.

221


===== PAGE 219 =====
222

Chapter 8

컨트롤의 사용

화면1 그림을 표시



===== PAGE 220 =====
8.9 프레임(『13006)

IH
=

2
=
으
메
Jb
0x
ow

우측에 있는 속성 창의 속성 이외에 다음의 것들이 있
으며 코드 내에서 사용할 수 있다.

Container                       FontStrikethru                                                   |                          |
|                               480                        |
FontBold                         FontUnderline                                   Mouselcon (1)                   |
,                                                         MousePointer (0 - 기본값          |
FontItalic                        hWnd                                                           0                       없음
FontName                          Parent
FontSize

준비되어 있는 이벤트

대디
|                                                    DbIClick

MouseUp

ECompleteDrag
EDragDrop

EDragOver
EGiveFeedback
ESetData

|으으은은

~] Naenccianausaccadlboinneaaaeiat Thong’

준비되어 있는 메서드
Drag                                  OLEDrag                      ShowwhatsThis
Move                                  Refresh                      zZOrder

223


===== PAGE 221 =====
 Chapter8 컨트롤의 사용

프레임을 배치하면 So] 틀이 표시된다. 프레임은 그 영역에 다른 여러 가지 컨트롤을 배치

해서 하나의 그룹으로서 다루는 데 사용된다. 이처럼 그룹화해서 한 개의 관리 단위로 하는 기
능을 콘테이너라고 한다.

면 네 개 중에 하나를 선택하는 옵션이 두 개 필요할 때 폼에 옵션 버튼 8개를 배치
8개 중에서 하나만 선택할 수 있으므로 우리가 원하는 기 능을 얻을 수 없다.
옵션

트 8
을 두 개 배치하고 프레임안에 각각
A
as

프레임 프로그램 예는 옵션 버튼의 항을

때

조하자.

컨트롤을 그룹으로 묶어서 한 개의 관리 단위로서 취급  하는 기능을 .컨테이너라 부른다. Bae 컨테이
너 기능을 갖는다. 컨테이너를 이동하면 내부의 컨트롤도 이동하고 컨테이너를 삭제하면 내부 컨트롤도
삭제된다.

@

224


===== PAGE 222 =====
8.10 체크 #tA(CheckBox)

체크 박스 아이콘                                  속성 창
폼 표시
DownPicture 0. a8
_        _                                     Dragl       (23)
속성은 우측에 제시한 이외에도 다음의 것이 있으며 ： [03040 — Os
_                                      (True
이것들은 코드 내에서 사용할 수 있다.                         |         !
Container             FontSize
DataChanged           FontStrikethru
FontBold              FontUnderline
FontItalic            hwnd
FontName              Parent

준비되어 있는 이벤트

LostFocus

MouseDown
MouseMove
MouseUp
OLECompleteDra

준비되어 있는 메서드

Drag                                     Refresh                        ShowwhatsThis
Move                                  SetFocus                    ZOrder
OLEDrag

225


===== PAGE 223 =====
226

_ Chapter 8

컨트롤의 사용

설명

체크 박스는 0ㅁ이나 Off S 이용하여 기능의 활성화를 설정하는 것으로 체크 박스를 클릭
하여 표시를 하면 그 기능이 활성화된다.

체크 YAS 그룹화해서 배열하는 것도 많이 사용되며 체크 박스는 옵션 박스와 다르고 각
Zt On/Off 2 자유로이 설정할 수도 있으며 전부 Onl =e 설정할 수도 있다.

체크 박스 설정값은 VALUE 속성을 사용한다.

Value = 0      박스가 공백이다.
Value = 1      박스에 V HAZ} 있다.
Value = 2      기본 설정의 회색 표시이다.

Value 2] 값으로 0 또는 1을 많이 사용한다. 2는 프로그램이 특별 의미를 갖게 하고 싶을
때에 사용하고 보통 조건부 선택을 나타내고 싶을 때 사용한다. 이것을 유용하게 사용한 예
는 Windows 2} 제어판의 [프로그램 추가/삭제]의 [윈도우 설치] BS 선택하면 자세히 알 수
있다.

Value 9] 판정은 다음과 같이한다. ㆍ

If Check1.Value = 1 Then

i표시 없게 처리
End If

Hae ela

속성 설정

개체              속성              설정

76×%11             Caption         "샘플 문자"
Check]          Caption         "볼드체 (&B)'
Check2      Caption      `이탤릭체 (&1)"
Check3         Caption         "2S (&U)"



===== PAGE 224 =====
8.10

코드

체크 박스((}16아80>)

'볼드제의 설정
Private Sub Check1_Click()

_ Tf Checkl Value = 1 Then     ' 제크가 있으면

Textl.Font.Bold = True  ''볼드체에 on
Else 그렇지 않으면
Textl.Font.Bold = False 볼드제에 off
End If
End Sub
'이탤릭체의 설정
Private Sub Check2_Click()
If Check2.Value = 1 Then
Textil .Font.italic = True
Else
Textl.Font.Italic = False
End If
End Sub
'밑줄의 설정
Private Sub Check3_Click()
If Check3.Value = 1 Then
Text1.Font.Underline = True
Else
Text1.Font.Underline = False
End if
End Sub
동작의 확인
© [볼드체(3)]의 체크 YAS 클릭하면 FH] 표시된다.
@ [이탤릭체([)]의 체크 박스를 클릭하면 이탤릭체로 변한다
@ [밑줄(0)]의 1   박스를 클릭하면 밑줄 표시로 된다
@ 복수 항목을 선택할 수 있다.
© @n+8 g        me 것과 [볼드체08)]의 체크 YAS 클릭하는 것은

세스키에 대해 서는 다음 Notes 참조.

같다. 이외에도 같은 액

227


===== PAGE 225 =====
Chapter8 컨트롤의 사용

명령 WET 체크 박스 등 Caption SYS 갖고 있는 컨트롤에서는 액세스키를 설정하는 것은 윈도우 화
면에서 자주 사용된다. 앞에서 예를 들었지만 액세스의 ABS 비교적 간단하다. Caption 속성에

&+영문자

를 기술하는 것만으로 자동으로 SAS 발휘하여 BOS 한 문자가 밑줄이 그어져 표시된다. 그리고
[401+[밑줄 붙은 영문키]를 누르면 클릭한 것과 같게 된다. 앞의 항목의 (+160<(1 체크 박스를 모델로 해
A 다음의 OS 제시한다. 액세스키 표시 "()"는 없어도 좋지만 붙이는 것이 관례이다.

aE 8=5
Captionaa    표시           설정
고딕체          고딕체         액세스 키 무효
고딕체(8)         고딕체(8)       (Be Gest 문자 표시
고딕체(&8)        고딕체(8)        (AN)+B) 7} 유효
고딕체&6         고딕체        [400+8]가 유효
고딕체(8010) 고딕체(3010) _—“AW+ 87} 유효

228


===== PAGE 226 =====
8.11 옵션 HE(OptionButton)

AAS
|             LL

8은 옆의 속성 창에서 보여진 내용 이외에 다음의
것이 있으며 코드 내에서 사용할 수 있다.

Container                       FontStrikethru                                                                            |
FontBold                         FontUnderline                                             on     a Sag               |
FontItalic                     hwnd                                            |           Li               보르                 |
FontName                          Parent                                        |         Right!            False                   |
FontSize                                                                                                                                  |

준비되어 있는 이벤트

MouseDown                                                                                                            i                                                                                                         |
MouseMove                                                                                                             |
ㅣ                                                    Mouse

준비되어 있는 메서드

Drag                                 Refresh                      ShowwhatsThis
Move                                  SetFocus                    ZOrder
OLEDrag

229


===== PAGE 227 =====
Chapter8 컨트롤의 사용

옵션 WES 복수의      튼 중에서 하나의 버튼만을 선택할 수 있다. 복수의 옵션 버튼을   배
치하고 한 개의 그룹으로서 사용한다. 그러나 항목이 한 개로 단순히 TAS On/Off =H 사용
할 때는 체크 박스가 편리하다. 즉 옵션 버튼은 프레임과 픽처 박스를 먼저 설정하여 그 위에
배치해서 사용하면 된다. 하나의 프레임과 픽처 박스 내에 배치된 옵션 버튼이 하나의 그룹이
된다. 이 경우 프레임과 픽처박스는 콘테이너로서의 역할도 갖는다. 예를 들면 프레임을 이동
하면 옵션 버튼도 함께 이동한다.

ES 위에 직접 배치할 수도 있고 이 APE 직접 배치인 옵션 버튼만으로 하나의 그룹이
된다. 옵션 버튼이 선택되면 그 Value 속성은 True7t 된다. 이것을 판정하여 처리한다.

RGBe 색을 지정하는 함수이다. 서식은
NOTE

RGB(red, green, blue)

|

2 red, green, blue 의 색상 GES 0~255 의 값으로 지정한다. 이 함수의 되돌린 값은 색의 RGBZt
을 나타내는 Long’ 정수로 속성 창의 『0760010「에 그 값이 표시되어 있다. 이외에 색 지정에는
0080010「함수를 사용하는 HAS 간단해서 자주 이용된다.

Agha

[시 Ae] 옵션 버튼에서 색을 선택한다. 「색상 변경 실행, 버튼을 클릭하면 텍스트의
표시색이 변경된다.

=

개체          속성        설정            비고
Textt         Text           "샘플 문자"

ForeColor     검정색으로 처리    최초의 색이 된다

_ Framet       Caption       "색상 선택"

061001      Caption       "black"

Value        True            최초로 선택되어 있다
Option2      Caption       "red"

Value        False           H| 선택
Option3      Caption       "green’

Value False           비 선택
Option4      Caption       "6146"

Value        False           비 선택

230


===== PAGE 228 =====
8.11 옵션 버튼(2610708ㅁ8내00)

코드

Private Sub Command1_Click()
If Option1l.Value = True Then
Text1.ForeColor = RGB(0, 0, 0)   "black
ElseIf Option2.Value = True Then
Text1.ForeColor = RGB(255, 0, 0) ‘red
ElseIf Option3.Value = True Then
Text1.ForeColor = RGB(0, 255, 0) ‘green
ElseIf Option4.Value = True Then
Text1.ForeColor = RGB(0, 0, 255) ‘blue
End If
End Sub

231


===== PAGE 229 =====
232

Chapter 8

컨트롤의 사용

fox]
것이 있으며 코드 내에서 사용할 수 있다.

의 속성 창에서 보여진 내용 이외에 다음의

Container
DataChanged
FontBold
FontItalic
FontName
FontSize
FontStrikethru
FontUnderline

ListCount
ListIndex
NewIndex
Parent
SelCount
Selected
Text
TopIndex

0649
ItemCheck
eyDown
eyPress

KeyUj

ieee

MouseDown
iMouseMove

Jb



===== PAGE 230 =====
8.12 리스트 ¥tA(ListBox)

준비되어 있는 메서드

AddItem                           OLEDrag                      SetFocus
Clear                               Refresh                      ShowwhatsThis
Drag                                 RemoveItem               zZOrder

Move

SEA 사용자가한 개 또는 HE 선택할 수 2

로 스크롤 바가 나타난다.

고
i.

리시트 박스로의 항목 추가는 40016 메서드를 사용해서

List1.AddItem 한국"
Listl.AddItem 미국”

처럼 한다. 또 삭제할 때에는 Removeltem 메서드를 사용한다. 리스트 박스에 한하지 않고

Visual 88810에서는 리스트에 항목 추가를 하고 싶을 때에는 4001[60을 그리고 항목 삭제를
하고 싶을 때에는 Removeltem S 사용하는 것이 보통이다.

다음에 제시하는 애플리케이션을 실행시키고 리스트 박스에 항목을 추가하거나 삭제할 때의 예
AS 보자. 또 현재 선택되어 있는 Text 속성에서 알 수 있

List1.addItem 스페인", 0

현재 리스트 박스의 선두에 스페인을 추가
List1.AddItem “스페인”

현재 리스트 박스의 베이 나타나 있는 항목 앞에 스페인을 추가(0이 선두)
List1.addItem “스페인”

Sorted 속성이 [706 일 때 적절한 위치에 배열된다

Sorted 속성이 False 일 때는 마지막에 배치된다
List1.RemoveItem 2

현재 리스트 박스의 두 번째에 표시되어 있는 항목을 삭제(0이 선두)
List1.Clear

든 항목을 삭제

List1.Text

현재 선택되어 있는 텍스트   설정한다

rufa
aM
iin
J
flo

by
©:

233


===== PAGE 231 =====
 Chapter8 컨트롤의 사용

항목의 자동 바꿀 배열

항목은 입력한 순서로 표시되지만 80060 속성을 TrueH 하면 오름차순으로 배열되어 표시

된다,

가로 스크롤 바 설정

설정하는 항목수가 리스트 박스 크기보다 클 때에는 세로 스크롤 바가 나타나는 것이 표준이다.
스크롤 바 표시는 Columns 속성에서 설정할 수 있다. 예를 들면 표시하는 항목 이름이 짧은 예는

한 행에 복수 항목 표시를 하게 하는 것이 편리하다.

Columns=0      표준 세로 스크롤 바
Columns=1     한 행에 한 항목 표시 세로 스크롤 바
Columns=2     한 행에 = 항목 표시 세로 스크롤 바

그 의의 속   속성 중에서 이용하는 것은 다음과 같다

ㅁ

Text         현재 반전 표시되고 있는 문자열을 얻는다
ListCount     등록되어 있는 모든 항목 수보다 1 작은 값
선두를 0 번째로 계산하기 때문이다
List Index     현재 채택되어 있는 항목 HSS 리턴 또는 설정한다(선두가 0)
Selected     현재 채택되어 QI=AlS True/FalseQ= 나타낸다
list          현재 유무에 관계없이 지정한 번호의 BAAS 얻는다

ol]: 현재 채택되어 있는 항목을 디버그용으로 표시된다.
DeBug PrintList1.Text
2: 전 항목을 디버그용으로 표시한다.

For i = 0 To List1.ListCount -1
Debug. Print List1.List (i)
Next

예3 : 채택되어 있는 항목을 삭제한다. 1

For i = Listl.ListCount -1 To 0 Step -1

If Listl.Selected(i) = True Then List1.RemoveItem i
Next

234


===== PAGE 232 =====
8.12 리스트 YtA\(ListBox)

예4 : 채택되어 있는 항목을 삭제한다. 3

n = List1.ListIndex
List1.RemoveItem n

예5 : 2번째 항목을 선택(반전 표시)한다.

List1.ListIndex = 2

복수의 항목을 삭제할 때에는, 한 개 삭제할 때마다 배열희 번호가 바뀌므로 주의하자.

NOTE    List1.Removeltem 1 1번째를 삭제. 그 후 배열 번호가 변한다
List1.RemoveItem 1 새로운 1번째를 삭제

라고 하면 정의 1, 2번째의 항목을 삭제한다. 또

List1.Removeltem 1 1번째를 삭제. 그 후 배열 번호가 wf Pict
List1.Removeltem 2 새로운 2번째를 삭제(전에 3번째)

라고 하면 정의 1, 3번째 항목을 삭제한다. 또
List1.Removeltem 2 2번째를 삭제. 그 후 배열 번호가 y-Hc}
List1.Removeltem 1 새로운 1번째를 삭제(전에 1번째)

라고 뒤부터 처리한 쪽이 배열 변경 영향을 받지 않고 안전하다.

[니플[니로틴램
리스트 박스는 국명이 표시되어 있으며 어느 하나를 선택하면 선택된 국가의 수도가 표시
된다.

fi  이 장의 메뉴 항목에서도 리스트 박스를 사용한 샘플 프로그램이 있으므로 그쪽도 참고로 하자.
NOTE

속성 설정

개체                    스스                 설정
| 1611            Columns          0

Sorted           True
Text1           Text              (공백)
Command         Caption               "수도 표시"

235



===== PAGE 233 =====
236

Chapter8 컨트롤의 사용

Private Sub Form_Load()
Listl.AddItem "한국"
List1.Additem "일본"
Listl.AddItem "미곡"
Listl.AddItem "프랑스"
Listl AddItem "영국"
Listl.AddItem "독일"
Listl.AddItem "중국"

End Sub

Private Sub Command1_Click()
Tf Listlitext = * Sia "other
Texti.Text = "Aja"
ElseIf List] Texe = "Gl Then
Text1.Text = "동경"
ElseIf Listi.Text = "미곡" Then
Text1.Text = "워싱턴"
ElseIf Listl.Text = "프랑스" Then
Text! Text = 파리"
ElseIf List1.Text   "영국" Then
Textl.Text = "HG"
ElseIf List1.Text =
Text1.Text = "베를린"
ElseIf List1.Text =
Text1.Text = "북경"
End If
End Sub

동작의 확인
© 실행 화면에 자동으로 세로 스크롤 바가 출현한다.
@ PBL 오름차순으로 정리되어 리스트 박스에 표시된다.
@ 항목이 많으므로 스크롤 바가 자동으로 표시된다.
@ 리스트 박스의 항목을 클릭하면 반전 표시된다.
© 수도 표시 HES 클릭하면 텍스트 박스에 수도가 표시된다.

      = 은.  f  PTT



===== PAGE 234 =====
8.12 리스트 ¥tA(ListBox)

시인 카로 ASS 바가 된다

oa!
ik
뻐

면 한번에 가로-두

Le

선택할 때 곧 수

Commandi_Click 0| 아니라 Listi_Click 이벤트 프로시저에 직접 기술하면 리스트를

도를 표시시킬 수 있다. Commandt_Click2 삭제하고 다음처럼 기술한다.
‘Command1 0] 없는2181로 기술

NOTE
Private Sub List1_Click()

TE Listl. Text = "Qt" Then
Text1l.Text = "동경"

(이하 같음)

End If
End Sub

237


===== PAGE 235 =====
238

Chapter8 컨트롤의 사용

폼 표시

도 0%

의 속성 창에서 보여진
드 내에서 사용할 수 있

다.

내용 이외에 다음의

Container
DataChanged
FontBold
FontItalic
FontName
FontSize
FontStrikethru
FontUnderline
hwnd

ListCount
ListIndex
NewIndex
Parent
SelLength
SelStart
SelText
TopIndex

Lombal

ombo    ombobBox

ee

hc

Whats ThisHelpiC 0

“Width

2535

준비되어 있는 이벤트



===== PAGE 236 =====
준비되어 있는 메서드

8.13 콤보 4tA(ComboBox)

AddItem                 OLEDrag              SetFocus
Clear                    Refresh             ShowwhatsThis
Drag                     RemoveItem          ZOrder
Move
설명
콤보 박스(별명 : 드롭다운 리스트 박스)는 선택할 수 있는 수가 많은 때에 특정한 하나의
항목을 선택하기 위하여 사용된다. 버튼을 클릭해서 표시된 리스트 중에서 한 개를 클릭
선택한다. 리스트 항목이 많은 때에는 세로 스크롤 바가 나타난다.
콤보 박스는 텍스트 박스와 리스트 박스의 기능을 가지고 있다. 즉 리스트 중에서 선택할
수도 있고 MES 누르지 않고 직접 텍스트를 입력할 수도 있다. 이것은 선택할 수 있는 항
목 중에서 선택한다. 만약 적당한 항목이 없다면 스스로 입력해야 한다
콤보 박스에 항목 추가/삭제의 방법 및 선택되어 있는 항목의 처리 방법 등은 리스트 박스
와 같다.
콤보 박스는 세 개의 표시 형식을 갖고 있다. 그 APS Style 속성에서 하고 Style=2Z
하면 선택밖에 할 수 없는 콤보 박스가 된다. 이것은 사용자의 입력을 받기보다는 이미 리스
Bal 데이터 중에서 하나를 선택하게 할 때 유용하다
Style - 드롭다운 콤보(디폴트)
M@ 버튼의 표시                    있음
보통 표시틀                et dat BAL HE 클리으로 리스트퓨현
항목의 편집                        가능
Style 1 - 표준 콤보
¥ 버튼의 표시                    없음
보통 표시들                 설정한 복수행에 리스트를 항시 표시
버튼의 표시                       가능

style 2 - 드롭다운 리스트
항목의 표시
다른 것은 드롭다운 콤보와 같음

nat
a
rf
2
[무

239


===== PAGE 237 =====
Chapter8 HES9| 사용

|
|
|

Hazes

콤보 박스에 국명을 선택하여 [수도 표시] MES 클릭하면 수도가 표시된다. 선택 항목이
없을 때에는 스스로 국명을 aes     고 대응되어 있지 않은 국명의 경우에는 등록되어 있
지 않다고 표시된다.                                          |

속성 설정

6006001        Style          0 - 드롭다운 콤보
Sorted         False

Text1           Text            (공백)

Command       Caption         "수도 표시"

비

Private Sub Form_Load()
Combol.AddItem "일본"     ‘2
Combo1.AddItem "중국"
Combo1.AddItem "한국"
Combol.AddItem "미국"

Combol .AddItem "영국"
Combo1.AddItem "프랑스"
Combo1.AddItem "독일"
Combo1.AddItem "캐나다"
Combo1.AddItem "스페인"

|>
.. Sa Msilll
09
JH
lz
ot

Combo1.Text = "한국"     '최초의 표시 리스트

보01701 . Show           '폼을 표시(40ㅁ참조)

Combo1.SetFocus        'Combol 에 폼 BEA] 포커스를 준다
End Sub

Private Sub Command1_Click()
TE -Combol .Téext 8 "let then

Text1.Text = "동경"
Elself Combol.Text = "중국" Then
Text1.Text = "북경"

240


===== PAGE 238 =====
8.13 콤보 4tA(ComboBox)

Elself Combol.Text = "한국" Then
Textl Text = "A[S"

Elself Combo1.Text = "미국" Then
Textl.Text = "워싱턴"

Elself Combol.Text = "영국 Then
Text1.Text = "HO"

Elself Combol.Text = "프랑스" Then
Textl Text - "파르"

Elself Combol.Text = "독일" Then
Text1.Text = "베를린"

Elself Combo1l.Text = "캐나다" Then
Text1.Text = "오타와"

Elself Combol.Text = "스페인" Then
Textl.Text = "마드리드"

Elself Combol.Text = "이탈리아" Then
Text1.Text = "로마"

Else
Text1.Text = "등록되어 있지 않

00

(0 최초 항목인 “한국"이 표시되고 포커스가 이동되어 있다.
@ Ml HES 클릭하면 리스트가 표시된다.
@ 항목수가 많으므로 세로 스크롤 바가 자동 표시되어 있다.
인지 항목을 클릭 선택하고, [수도 표시]를 클릭하면 수도가 표시된다.
© 텍스트 박스에 직접 “이탈리이"라고 입력하고, [수도 ENS 클릭하면 수도가 표시된다(이
제

241



===== PAGE 239 =====
242

Chapter 8

이 프로그램 중에서

Form. Show
Combo1. SetFocus

라는 두행은 없어도 좋다. 이 샘플의 ASS 알기만 하면, 없는 편이 AES SetFocus= 애플리케이
션 실행시에 최초의 포커스를 Combo ol 주기 위해 사용하고 있다. 그런데 SE Form_Load 가 실행 완
료된 직후에 표시된다. 표시하지 않은 폼에서 콤보에 대해 SetFocus 실행하면 에러가 된다. 거기서 OF
직 Form_Load= 종료하고 있지 않지만 이 시점에서 먼저 SS 표시한다라는 SAO Show 메서드를
기술하고 있다.

수평 스크롤 바나

규정

수평 스크롤 바 아이콘                           속성 창
폼 표시
|
|                ㅁ
때                                    |         태미   나
속성은 옆의 속성 창에서 보여진 내용 이외에 다음의 | amet Tae
것이 있으며 코드 내에서 사용할 수 있다.                    |        Tue
Container           Parent
hind                                         |



===== PAGE 240 =====
8.14 수평 스크롤 HKHScrollBar)

준비되어 있는 메서드
Drag                Refresh          ShowwhatsThis
Move                SetFocus         ZOrder

J. 설명

수평 및 수직 스크롤 바는 어떤 정보 범위 중에서 현재 위치를 표시하거나 설정하는 데 사용
한다. 예를 들면 라디오의 볼륨처럼 어떤 범위 내에서 연속적으로 변하는 값을 표시/설정하는데
편리하다. 또 윈도우의 미디어 플레이어에서는 재생 경과 시간을 표시하는 데 사용되고 있다.
수평 스크롤 바를 사용할 때에는 표 8-6의 속성이 중요하다.

표 8-6

속성            기능

Max           위치 표시가 우측끝(최대)에 VS 때의 값을 설정한다

Min            위치 표시가 좌측끝(최소)에 있을 HA 값을 설정한다

SmaliChange    화살표 표시 WES 232 때 이동량을 설정한다

LargeChange   위치 표시와 화살표 표시 버튼의 사이를 클릭할 때 이동량을
설정한다

Value          현재 위치의 값을 취득한다. SE 지정한 값에 해당하는 위치에
위치 표시를 이동한다

예를 들면 0~100범위의 수평 스크롤 바를 설정해서 최초의 위치 BAS 30으로 할 때에

는 다음처럼 한다.

Hscroll1.Max = 100
Hscrolli.Min = 0
Hscroll1.Value = 30

또 프로그램을 실행 후에 위치값을 변수 ㅁ에 입력할 때에는
n=Scrol11.Value

로 한다. 좌우 화살표 표시 HES 클릭할 때의 수평 스크롤 바의 이동 길이는 SmallChange=
설정한다. 보통 이 값은 1로 한다. 화살표 버튼과 현재 위치 표시 사이를 클릭할 때 수평 스크롤
바의 이동 길이는 LargeChange@ 설정한다. HES 이 값은 10등으로 하고 크게 이동한다.

띠플법로빈림
수평 스크롤 바에서 설정한 적, 녹, 청의 8원색에서 텍스트의 색을 표시한다.

243


===== PAGE 241 =====
244

Chapter 8

컨트롤의 사용

속성 설정
개체       속성        설정               비고
86611      Caption                        Ad 모델" 공백은 위치 AAS 위함
BorderStyle    1 - aa            틀 표시
BackColor     백               최초의. 배경색
Label2      Caption           0        255"          공백은 위치 AAS 위함
Label3    Caption       "red"              표제
Label4    Caption       "green’
Label5    Caption       "plue"
Labelé Caption       "255"              값 표시
Label7    Caption       255,
Label8    Caption       1255:
HScroll1. Max          255               4\CH at (red)
Min           0                 최소값
Value         255               최초의 핸들 위치
LargeChange 10               104 이동
HScroll2. Max          255               (green)
Min           0
Value         265
LargeChange 10
HScroll3. Max          255               (blue)
Min           0
Value         255
LargeChange’ 10
코드

Private Sub HScroll11_Change ()
Label6.Caption = HScroll1.Value
Labell.BackColor = RGB(HScroll1l.Value, HScroll2.Value, HScroll13.Value)

End Sub

Private Sub HScrol1l2_Change()
Label7.Caption = HScrol12.Value
Labell.BackColor = RGB(HScroll1.Value, HScroll2.Value, HScrol113.Value)

End Sub

Private Sub HScrol13_Change()
Label8.Caption = HScrol113.Value
Labell.BackColor = RGB(HScroll1.Value, HScroll2.Value, HScroll13.Value)

End Sub


===== PAGE 242 =====
8.14 수평 스크롤 바160001830

동작의 확인
(1 세 개의 위치 표시를 이동시키면 창 배경색이 해당 색으로 변한다.
@ 각 스크롤 바가 지지하고있는 값이 우측에 표시된다.
(8) 좌우 화살표 버튼을 클릭하면 하나씩 증감한다.
(4 현재 위치 표시와 화살표 버튼 사이를 클릭하면 10씩 증감한다.

245


===== PAGE 243 =====
컨트롤의 사용

Chapter 8

그저

수직 스크롤 바 아이콘

|

= 표시

(없음)
0 - 기본값

속성 창에서 보여진 내용 이외에 다음의

False
1

Tabindex           0

ㅇ   옆     ㅇㅇ ㅇ
것이 있으며 코드 내에서 사용할 수 있다.                               =
Container            Parent
hwnd
준비되어 있는 이벤트
준비되어 있는 메서드
Drag                 Refresh           ShowwhatsThis
Move                 SetFocus          zOrder

 설명

나

수직 스크롤 바는 수평 스크롤 바와 같은 기능으로 어떤 정보 범위 중에서 현재 위치를
타내거나 설정하는 데 사용한다. 세로 방향으로 길게 배치되어 있는 이 컨트롤은 폼 상의
이아웃에 맞춰서 수평/수직 스크롤 바를 분리 사용한다. 수직 스크롤 바에 대한 ABS 수
스크롤 바(807011880)를 참조하면 된다.

러
평

246


===== PAGE 244 =====
8.16 타이머(117060

타이머 아이콘                                             속성 창

폼 표시

속성은 위의 속성 창에서 보여진 내용 이외에 다음의 것이 있으며 코드 내에서 사용할 수
있다.

Parent

준비되어 있는 이벤트

                                            Teena

준비되어 있는 메서드
없음

cholo 14 zie) ait wot alg 발생시킨다. 에

를 들면 달리는 개를 표현하
는 분할 애니메이션을 몇 개 준비해서 타이머 컨트롤을 사용하여 일정 시간(예를 들면 0.5초)
마다 애니메이션 이미지를 새로 바꿔서 표시하면 그 개는 언제까지나 계속 달린다

타이머 컨트롤은 실행시에는 표시되지 않는
타이머 컨트롤의 SYS 표 8-7의 두 가지가 중요하다.

247


===== PAGE 245 =====
Chapter8 컨트롤의 사용

속설        qs
Interval     이벤트 발생의 간격을 설정하다. 단위는 ms
Enable     타이머 이벤트를 유효/무효(이벤트가 발생하지 않는다)로 한다

ㅠ46에서 유효. 『156@에서는 무효가 된다

띠플느로램 -
좌측에서부터 문자가 흘러가게 하고 타이머를 사용하여 타이밍을 처리하고 있다. 픽처의
새로 바꿈 항목(9장)에서도 타이머를 사용한 프로그램이 있다.

xz
속성 설정

개체           속성            설정          비고
Labell         BackColor      백
BorderStyle     1 - Ala
11061         Enabled        True
Interval        500          500미리의 이벤트 발생
Command        Caption            "청지,계속"
코드

Private Sub Command1_Click()
Static f As Boolean
Tf £ Then
Timerl1.Enabled = True   '타이머 유효
Else
Timerl.Enabled = False 타이머 =
End If
f = Not 도
End Sub

때

Private Sub Timerl_Timer ()
Static ct As Integer
Dim sl, s2

|                       Ck = cE + i

81 = "여러분 안녕하세요."
s2 = Mid(sl, ct) & Left(sli, ct - 1)   『들
Label1.Caption = 82
TE Ct. > 13 94160 06 = 0

End Sub

AO
ot
ule}
A>
[뿌
mel
Pal

0 실행하면 문자열이 점점 좌측으로 흘러가듯이 표시된다.
© 정지/계속 HES 클릭하면 문자가 정지/계속된다.

0

어

248



===== PAGE 246 =====
(9) 디자인할 때에는 타이머 아이콘을 볼 수 있지만 실행하면 사라진다.

화면1

디자인시의 화면

드라이브 리스트 아이콘

Jb
Oz
0엔

폼 표시

속성은 오른쪽에 표시되어 있는 것 이외에 다음과 같

은 것이 있다. 이들 코드 중에서 사용할 수 있다.

Container                FontUnderline

Drive                     hwnd

FontBold                 List

FontItalic              ListCount

FontName                 List Index

FontSize                 Parent

FontStrikethru         TopIndex

i

Causes Validatic Tru

e
Ss

249


===== PAGE 247 =====
Chapter8 컨트롤의 사용

ragDrop
Drag Over
GotFocus
eyDown
가 fess

100
OLECompleteDrag
OLEDrag ie
OLEDragOve!
OLEGiveFeedback

준비되어 있는 메서드

Drag                                 Refresh                      ShowwhatsThis
Move                                  SetFocus                    zOrder
OLEDrag

os

드라이브 JAE 박스는 선택 가능한 AS 드라이브 리스트를 표시합니다. 실행시 사용
자는 를 단추를 클릭해 표시되는 리스트 중에서 희망하는 드라이브를 선택할 수 있습니다. 선
Drive 속성에서 알 수 있습니다.

드라이브 리스트 박스는 디렉토리 리스트 박스 및 파일 리스트 박스와 연동하여 사용하는
것이 일반적인 것입니다. 이들 세 가지 리스트 박스를 활용하는 것에 따라

A 드라이브 8 디렉토리 ㅇ파일
로 지정하는 것이 가능하게 됩니다.

드라이브 리스트 박스의 구체적인 설명은 [파일 리스트 박스] 항목을 참고해 주세요.

[드라이브 리스트 박스]+[디렉토리 리스트 박스]+[파일 리스트 박스]에서 특정 파일을 선택하는 방법은 «A

Note] WHE 윈도우 3.1 형식이다. 현재의 윈도우 95/98에서와 같이 윈도우 탐색기가 있다. 이 창 안에서 드
라이브도 디렉토리도 Wate 선택할 수 있다. Common 다이얼로그 HESS [Microsoft Common
Dialog (00[01]을 추가하면 사용할 수 있다.

250


===== PAGE 248 =====
8.18 디렉토리 리스트 박스(21119120>

디렉토리 리스트 박스 아이콘                      속성 창
폼 표시
peau Files
속성은 옆에서 제시한 것 이외에도 다음과 같은 것이
있으며 코드 내에서 사용할 수 있다.                                                  |
ㅣ
Container             FontUnderline
Drive                 hwnd
FontBold              List
FontItalic            ListCount
FontName              ListIndex
FontSize              Parent
FontStrikethru       TopIndex
준비되어 있는 이벤트
ra
0000
GotFocus
eyDown
eyPress
00006
MouseDown
MouseMove
MouseUp

251



===== PAGE 249 =====
Chapter8 컨트롤의 사용

준비되어 있는 메서드

Drag                                 Refresh                      ShowwhatsThis
Move                  ：                   SetFocus                      ZOrder
OLEDrag

디렉토리 리스트 박스는 현재 Evol] 디렉도리를 계층  738 표시해 준다. 사용자는
그중 임의의 디렉토리를 선택할 수 있다. 선택한 디렉토리 명은 Path 속성에서 알 수 있다.
디렉토리 AES] 88471 많을 때에는 스크롤 바가 표시된다.

이브 리스트 박 바스 및 및 파일 리스트 박스와 같이 사용하는 것이
박스의 구체적인 내용을 파일 리스트 박스의 항을 참조하자.

252


===== PAGE 250 =====
8.19 파일 리스트 ¥tA(FileListBox)

i           ee
(archive

| {BackColor
_|CausesValidatio
{Draglcon

옆에서 제시한 것 이외에도 다음의 것이 있다,
코드 내에서 사용할 수 있다.

Container                       hWnd

FontBold                            List

FontItalic                      ListCount

FontName                          ListIndex                                                                                      |
FontSize                            Parent                                            |                         -…
FontStrikethru           Path                                    — Winsted         |       |
FontUnderline                      TopIndex

준비되어 있는 이벤트

BoiCick
ragDro
Bragover
GotFocus
eyDown
eyPress

louseDown
MouseMove
louse

253



===== PAGE 251 =====
Chapter8 HE=9| 사용

준비되어 있는 메서드

Drag                                     Refresh                        ShowwhatsThis
Move                                  SetFocus                    ZOrder
OLEDrag

As 박스는 현재 Calelo] 있는 mage 표시한다. BA 그 중에서 임의의

리스트 빅
파일을 선택할 수 있다. 선택한 파일명은 Filename 속성에서 알 수 있다.
라이브 리스트 박스와 디렉토리 리스트 박스를 연동해서 사용하는 것이
본             츠느

보통이다. 이 세 개의 리스트 박스를 잘 짜맞추는 것에 의해

A 드라이브의 ㅁ디렉토리의 파일.

이라는 지정이 가능하다. 러스트 박스의 연동은 간단하다. 다음의 결정된 문구를 이용해 보자. 각
각의 리스트 박스의 이름을 271761, 2171, Filel 2}i1 하자.

Private Sub Drivel_Change()

Dirl.Path = Drivel.Drive    '드라이브 AS pirl do] 연동시킨다
End Sub.                           |
Private Sub Dirl_Change()

Filel.Path = Dirl.Path      '디렉토리 AHS #1161에 연동시킨다
End Sub                             |

실제로 파일을 선택할 때에는 다음 4개의 속성이 중요하다.

Drivel.Drive      선택되어 있는 드라이브 명을 설정/취득
(드라이브 보기가 표시되어 있다)

Dirl.Path         선택되어 있는 패스 BS 설정/취득
(디렉토리 보기가 표시되어 있다)

Filel.Path        선택되어 있는 패스 명을 설정/취득

(파일 보기가 표시되어 있다)
Filel.Filename   선택되어 있는 파일명을 취득

전체 패스명의 취득
선택한 파일의 전체 BHA(Full Path) (“C:\mydata\ak.txt” 의 형식 이름)은 기본적으로는
myname=Falel.Path & Filel.Filename
254


===== PAGE 252 =====
8.19 파일 리스트 YtA(FileListBox)

로 얻을 수 있다. 단지 2801 가 800[디렉토리의 장소는 1161.28 의 내용이 “:”처럼 Fea’
가 없다)스스로 VS 붙여 줄 필요는 없다. 다음 예를 보고 실제에 사용되는 샘플 프로그램을 살펴
보자.

예1 : Root 디렉토리에 있는 파일명 취득

Filel.Path7} "c:", Filel.filenameS "abc.txt"= 한다.

myname = Filel.Path & "\" & Filel.filename
(021)       (\)      (abc tet) = G: \abe txt

예2 : 일반 폴더에 있는 파일명 취득

Filel.Path7} "c:\mydata\", .Filel.FilenameO| "xyz.txt"= 한다.

myname = Filel.Path & Filel.filename
(Ci: \mydata\) (xyz.txt)           — c:\mydata\xyz.txt

파일 패턴의 지정
파일 리스트 박스에 표시시키는 파일의 패턴을 지정할 수 있으며 Pattern 속성을 사용하여 다
음처럼 하면 된다. 복수의 타입이 있을 때에는 「 로 구분한다.

Pattern *.*               모든 파일명을 표시
Pattern *.ico               ico 파일명만을 표시
Pattern *.ico;*.bmp     ico, bmp 파일을 표시

디플 녀로빌렘
드라이브 리스트 박스, 디렉토리 리스트 박스, 파일 리스트 박스를 사용하여 ico, bmp 파일
의 그림을 픽처 박스에 표시한다. 또 선택된 파일명을 라벨 컨트롤을 사용해 표시한다.

속성 설정
개체              속성       설정
Picture      BackColor       BH
File1             Pattern              * iCO;*,omp
Labelt     — Caption         (없음)

주) 07061과 Dirlg 표준 그대로 사용한다.

코드

Private Sub Drivel_Change()
Dirl.Path = Drivel.Drive    'Dirl 에 연동된다

255


===== PAGE 253 =====
Chapter8 컨트롤의 사용

End Sub

Private Sub Dirl_change()
Filel.Path = Dirl.Path

End Sub

Private Sub Filel_Click()
Tf Right (Filel.Path, 1) < > "\"|Then ‘Root 7} 없을 A
p$ = Filel.Path & "\" & Filel.filename
Else ='Root 폴더의 경우
p$ = Filel.Path & Filel.filename

End If
Picturel.Picture = LoadPicture(p$)    「'파일을 로드한다
Label1l.Caption = p$         ‘Full Path 표시한다
End Sub
동작의 확인

® 드라이브 리스트 박스에서 드라이브를 선택할 수 있다.
@ 선택한 드라이브의 디렉토리 구성이 표시된다.

(9 디렉토리 리스트 박스에서 디렉토리를 선택할 수 있다.
(4 선택한 디렉토리 파일 구성이 표시된다.
© 파일 리스트 박스에서 희망 파일을 선택할 수 있다.
© 파일 리스트 박스에는 .100, .bmp 파일명만이 표시된다.
© 8개의 리스트 박스는 연동하고 있다.
 선택한 파일이 픽처 박스에 표시된다.
(9 선택한 파일의 패스명이 화면 아래의 라벨 속에 표시된다.

|
| © 선택한 디렉토리를 더블 클릭하면 파일 리스트 박스에 파일
|    이 나타난다    !         ie       :                          |

|

6) 선택한 bmp 가 표시되었다

|       4 선택된 패스가 표시된다. 여기에 [라벨] HESS 배치하고 있다

| @ 선택한 파일을 더블 클릭하면 그림이 표시된다

256


===== PAGE 254 =====
8.20 셰이프(91206)

세이프(5

셰이프 아이콘                                                        속성 창

폼 표시

속성은 옆에서 제시한 것 이외에도 다음의 것이 있으
며 이것들은 코드 내에서 사용할 수

fo}
^

Container           ForeColor
Parent

준비되어 있는 이

fe)
없음

f=
\m

준비되어 있는 메서드

Move                Refresh     zOrder

가타
셰이프는 폼 내에 사각형, 정사각형,

정원, 타원을 그릴 때에 사용하며 각은

둥글게 만들 수
있다. 셰이프는 SS 장식하는 데 사용되며 셰이프 컨트롤 조작과 기능은 라인 컨트롤과 같다.

ㅇ
BorderStyle, BorderWidth, DrawMode 등의 기본적인 기능은 라인의 항목을 참조

바란다.

;
Ol

7]

257


===== PAGE 255 =====
Chapter8 컨트롤의 사용

셰이프 컨트롤에서 그리는 도형은 Shape 속성에서 결정할 수 있다. 이때 FillStyle 속성에
서 그린 도형의 바탕색, 사선 등을 지정할 수 있으며 처리에 사용하는 AS \11060107 속성에
서 지정한다. Shape YH FillStyle 2} 규정에 대해 살펴보자.

Shape                    0 - 사각형
1 - 정사각형
2 - 타원형
3- Uy

4 - 둥근 사각형
5 - 둥근 정사각형

Fillstyle           0 - 단색
~ 투명
2- 수평신
3 - 수직선
4 - 상향 대각선
5 - 하향 대각선
6 - 교차
7 - 대각선 교차

셰이프는 이벤트를 가지고 있지 않으므로 셰이프 자체가 처리시키는 것이 아니다. 셰이프
컨트롤에서 형태을 그리고 내부에 명령 HES 배치할 AL 있지만 단지 겹쳐져서 배치되어
있을 뿐이다. 셰이프 컨트롤 자체는 컨테이너로서 사용할 수는 없다. 디자인할 때 셰이프를 이
동해도 명령 버튼은 움직이지 않는다.

258


===== PAGE 256 =====
8.21 라인(106)

라인 아이콘                                      속성 창
폼 표시

속성은 옆에서 제시한 것 이외에 다음과 같은 것이 있
으며 이것들은 코드 내에서 사용할 수 있다.

Container              Parent

으
없음

준비되어 있는 메서드

Refresh                                 ZOrder

라인은 디자인할 때 폼에 직선(수평, 수직, EUS 그을 때에 사용한다. Gels] 폼과 픽처
박스는 Line 메서드를 가지고 있으므로 이것을 사용해서 AAS 그을 수도 있다. 실제로는 라
인 컨트롤 쪽이 드래그 작업으로 실행 착오도 바로 잡아가며 그을 수 있으므로 편리하다.
Line 메서드는 프로그램 실행 과정에서 동적으로 AS 그린다.

259


===== PAGE 257 =====
_ 008016『8 컨트롤의 사용

린 AAS AutoRedraw 속성이 13186 로 되어 있어도, 언제라도 내용

라인 컨트롤은 폼, 픽처 박스, 프레임 내에 AAS 그릴 수 있다. 실행시에 ※1, X2, 1,
?2의 SYS 설정하는 것에 의해서 AAS 이동시킬 수    전 그러나 Move 메서드는 없다.
은 BorderWidth 속성에서 설정한다. 또 나 속성은 개체마다 의미가
다르다. 라인    컨트롤에서 다음의 의미를 갖는다.
이 중 23~5는 BorderWidth7} 1일 때만 유효하고 다른 경우는 실선이 된다. 또 라인의
경우는 6도 겉보기는 실선과 같아진다.

개

BorderStyle                 명
색(경계의 중심선이 개체의 외형선과 일치)

시

x de

0H
lie
Qi
3
4 - 대시-점
5 - 대시-점-점
6 - 내부 단색(경계의 중심선이 개체의 외형선과 일치)
DrawMode 속성을 사용하면 그리기 BES 지정할 수 있다. 이것은 배경색과 es
처리 방법을 결정하는 것이다. |S SH Minvert)A= 라인이 교차한 부분은 배경식
전한 색으로 한다.
당연한 얘기지만 라인은   ns     ES 갖고 있지 않으므로 그것 자체가 뭔가 처리의 동기를 만
드는 것은 아니다. 단지 그냥 표시될 뿐이다.

『
ie   수동
r= Jo,

260


===== PAGE 258 =====
8.22 OLE 컨테이너(0ㄴㅁ)

속성은 옆에 제시한 것 이외에도 다음의 것들이 있으

ou
OAS

Patel EZ

코드 내에서 사용할 수 있다.

J}
ot

Action
AppIsRunning
Container
Data
DataChanged
DataText
FileNumber
ForeColor
Format

hwnd
lpOleObject
Object

ObjectAcceptFormats
ObjectAcceptFormatsCount
ObjectGetFormats
ObjectGetFormatsCount
ObjectVerbFlags
ObjectVerbs
ObjectVerbsCount
OLEType

Parent

PasteOK

Picture

0-35
2 0 106    |
- 105        |

0 - 기본값         |

OLEDropAllowec False
2

‘True                    |

"120
0 - AS
0

Tue

261


===== PAGE 259 =====
_ 0118016『8 컨트롤의 사용

준비되어 있는 이벤트

MouseMove
jousel

준비되어 있는 메서드

Close                                   FetchVerbs                              SaveToFile
Copy                                                InsertObjDlg                                 SaveToOlelFile
CreateEmbed                   Move                                       SetFocus
CreateLink                     Paste                                     ShowwhatsThis
Delete                              PasteSpecialDlg                 Update

DoVerb                             ReadFromFile                       ZOrder

Drag                                 Refresh

설명                    ete

OLE 컨테이너 AES? 스스로 AAS Visual 88810 애플리케이션 중에서 다른 애프리케

이션의 개체를 이용      a 있도록 한다. S 사용자가 AAS Visual Basic 애플리케이션 중에
서 Execl J} Word 등을 사용할 수 있다.

OLE 컨테이너 컨트롤은 폼 위에 다른 애플리케이션 데이터를 삽입 가능한 프레스 HES
작성한다. 쉽게 설명하면 다른 애플리케이션 데이터의 AAS 제공하는 것이다.

예를 들면 Sol] OLE 컨테이너를 배치했다고 하자. 그러면 사각의 Sol] 빈 공간만이 표
된다. 그리고 [개체 삽입] 다이얼로그 박스가 나타나며 여기에서 [개체의 종류]
MicroSoft Excel 워크시트를 선택했다고 하자. 그러면 OLE 컨테이너 컨트롤용으로 만들
어진 빈 공간에 엑셀용 영역과 임시 그리드가 표시된다. 그리고 이 애플리케이션을 실행시
키면 작성한 프로그램 중에서 Excel S 사용할 수 있게 된다. 이것은 마치 윈도우에서 OLE
고받기를 하고 있는 것과 비슷하다. 예를 들면 Word 의 화면에 엑셀 데이터

0 fu >

OLE 컨테이너에서는 채우기와 렁크라는 두 가지 방법이 있어 다른 애플리케이션의 데이
터(218 MAS 조작할 수 있다. 채우기에서 작성한 데이터는 그 애플리케이션 자체가 갖고
있으므로 데이터를 보존하거나 읽어 내려가는 루턴을 사용할 필요가 있다. 링크의 경우는 데
이터를 작성한 애플리케이션                    데이터를 저장/불러오기를 한다.

262



===== PAGE 260 =====
8.22 OLE 컨테이너(2.ㅁ)

이전의 Visual 88810에서는 같은 종류로 OLE | ]언트 컨트롤이 있었다. 그것의 기능
을 보다 강화시킨 것이 OLE 컨테이너 컨트롤이라 할 수 있다(상호 호환성   이 있다).

OLE 컨테이너에는 수많은 속성이 있고 또 OLEFH: 개념에 대해서 종합적인 지식이 필요
하므로 본격적으로 사용하는 것은 처음 시작하는 사람에게는 부담이 되기 때문에 앞으로 제
공하는 OLE 컨테이너의 최소 기능을 AAS 수 있는 샘플과 자주 사용하는 주요 메서드의 기
익히 도록 하자.

SaveToFile           01ㄷ컨테이너 내에 있는 데이터를 디스크에 저장한다
LoadFromFile           디스크로부터 0ㄷ컨테이너에 데이터를 읽는다
DoVerb           설정한 외부 애플리케이션을 기동한다

Close                 실행 중에 있는 외부 애플리케이션을 종료시킨다

Aiea

이해를 돕기 위해 단순한 사용 예를 보면서 익혀 보자. 폼 상에 OLE 컨테이너 AEBS 실
행하여 OLE 컨테이너 컨트롤을 더블 클릭하는 것에서 시작된다. 단지 이때 창의 크기를 적
점히 변경하거나 흑은 경우에 따라서는 MOLE 72S AEE 여러가지 dae 필요
로 한다. 따라서 그런 부담을 줄이고자 여기에서는 외부 야플리케이션을 별개의 창으로 실행
하는 방법을 제시한다. 전용 버튼을 클릭하면 이벤트가 불려지고 편집 에디터가 나타난다.

속성 설정

개체                 속성                  설정
Commandt         Caption         a
Command2         Caption             ‘OLE 편집"
Command3       _Caption             비로 은
Command4      Caption        "저장"

주) Formol 011을 설정하고 [오브적트 삽입] SNOW [그림판 파일 ]을선택한다.

Lk

코드

Private Sub Command1_Click()     '열기
Dim FileNum As Integer
FileNum = FreeFile
Open "c:\mydata\oletstl.ole" For Binary As #FileNum
OLE1.ReadFromFile FileNum

263


===== PAGE 261 =====
Chapter8 컨트롤의 사용

Close #FileNum

End Sub
Private Sub Command2_Click()     ‘OLE 편집
OLE1.Doverb -2             '외부 애플리케이션(이 경우 그림판)을 실행
End Sub
Private Sub Command3_Click()     'OLES &
OLE1.Close
End Sub
Private Sub Command4_Click()     「저장

Dim FileNum As Integer

FileNum = FreeFile

Open "c:\mydata\oletst1l.ole" For Binary As #FileNum
OLE1.SaveToFile FileNum

Close #FileNum

End Sub

동작의 확인
© 실행해서 OLE BAS 클릭하면 [이벤트|라는 별개의 창 화면이 되고 그림을 그릴 수 있다
© 그림을 그리면 그 그림이 약간 늦게 OLE 컨테이너 박스에 표시된다

(8) OLE 종료를 클릭하면 그림판이 종료한다.
(4 저장 HES 클릭하면 저장된다.
(6) 다음에 실행할 때 열기 HES 클릭하면 읽을 수 있다.

264


===== PAGE 262 =====
그릴 6 19

8.22 OLE 컨테이너(0@ㄴㅁ

화면1 컨트롤 배치와 개체 삽입
(1) 이 OLE 컨테이너 HESS 배치하면

여러 가ㅅ

화면3 개체 편집 종료의 보통" 화면

 애플리케이션에서 화

er
Bh

@ 이것을 선택하여 이벤트를 실행하기 위한

면으로 돌아간다. 그림도 표시되어 있다

| 설정이 자동으로 행해진다

(7) 이것에 그림을 그리면

265


===== PAGE 263 =====
266

Chapter 8

컨트롤의 사용

ME IE] 2

이번에는 별도의 창에서 표시되는 것이 아니고 외부 애플리케이션을 자신의 창으로 넣
방법을 익혀 보자. 이 처리를 하는 경우는 2개의 SS 사용하면 스타트로 간다. 이 두 개의
중에서 하나는 MDI(Multi Document Interface) °]2@}31 하고 엑셀처럼 토대가 되는 큰
창으로부터 절대로 나올 수 없는 작은 폼의 형식을 하고 있다. 본 책에서는 MDIS 설명은
지 않으므로 만족할 때까지 참조로서만 보자. MDI 폼은 다음처럼 작성한다.

i
~
=
TI
포
ral
하

© 평상시에 기동하면 2S Form1°] 있다.
(3) (224 E(P)|-(MDIS 모듈의 추가(1)]를 클릭
— MDIForml °|@}3! 하는 폼이 작성된다.
(3) Form! 2] 화면으로서, Form1 2] 속성 창에서
— MDIChild=True 라고 한다(이것은 보통은 MDChild = False = 되어 있다.)

이상의 조작에서 MDIForm1& 부모 폼, Form1& 자식 폼이 된다.

6

떠

이 프로그램의 용법은 전에 나온 샘플 프로그램1과 같다. 단지 외부 야플리케이션의 기동
LE 컨테이너를 더블 클릭으로 할 수 있도록 한다(보통 형식에서도 가능).

rlo
oO

속성 (MDI Form1)
없음
속성 설정(『0「01)

개체                           속성                설정

Command]       Caption 열기
Command2             Caption            "OLE 종료"
Command3            Canton = |        `저장"

주) Forml ol 01트을 설정하고 [개체의 삽입 ] 화면에서 [그림판]을 선택한다.

코트

Private Sub Form_Load()

Forml.Height = 3600        !지시 품의 ㅋ기 초성
Forml.Width = 4665

End Sub

Private Sub Command1_Click()     |



===== PAGE 264 =====
8.22 OLE 컨테이너(0ㄴㅁ)

Dim FileNum As Integer

FileNum = FreeFile

Open "c:\mydata\oletstl.ole" For Binary As #FileNum
OLE1.ReadFromFile FileNum

Close #FileNum

End Sub

Private Sub Command2_Click()     os
Close.Close

End Sub

Private Sub Command3_Click()     저질

Dim FileNum As Integer
FileNum = FreeFile
Open "c:\mydata\oletstl.ole" For Binary As #FileNum
OLE1.ReadFromFile FileNum
Close #FileNum
End Sub

주) 이상의 프로그램은 Form 12] HOI}, 책의 예에서는 MDIForml]ol 관한 프로그램은 없다.

동작의 확인
© 기동해서 01.8컨테이너를 더블 클릭하며 [그림판]과 일체화된 화면이 되고 그림을 그릴 수
있다.

267


===== PAGE 265 =====
Chapter8 컨트롤의 A

00

@ 마이

@ 01 ㄷ컨테이너를 배치

[그림판]도 설정해 둔다

268


===== PAGE 266 =====
8.22 OLE 컨테이너(2ㄴㅁ)

개

© 친 폼에 [페인트] 메뉴와 툴 박스가`표시되어 있다

@ 이것을 클릭하면 그림 종료

(0) 자 폼은 그대로 그림 화면이 된다
여기에 그림을 그린다

화면4 원래 화면으로 돌아간다

© 애플리케이션 화면으로 돌아간다. 그림도 표시되고 있다

269



===== PAGE 267 =====
Chapter8 컨트롤의 사용

규정          이

데이터 아이콘                                             속성

폼 표시

속성은 옆에 제시한 것 이외에도 다음의 것들이 있으
며 이것들은 코드 내에서 사용할 수 있다.
Database               FontStrikethru
FontBold               FontUnderline
FontItalic             Parent
FontName               Recordset
FontSize

준비되어 있는 이벤트

ragUrop
DragOver

or
louseDown

7

juseUp
ErompleOrag
EDragDrop
EUragUver
EGiveFeedback
ESetData
LEStartDra:

[SSSSooz
Hors

| -30          1
디 &Hs00000058 |

10 -처음으로 미 |

준비되어 있는 메서드

Drag                                 Refresh                     UpdateRecord
Move                                  ShowwhatsThis          ZOrder
OLEDrag                           UpdateControls

270



===== PAGE 268 =====
8.23 데이터(0012)

설명

데이터 컨트롤은 기존의 데이터베이스의 정보를 폼에서 이용하기 위하여 사용되며 Visual
28810에서 데이터 처리를 하고 싶은 경우 Fo] 여러 가지 컨트롤을 배치해서 각각의 속성을
작성해야 한다.

또한 그 외에 처리하고 싶은 데이터를 디스크로부터 YAY 저장하거나 하는 절차도 필요하
다. 그러나 데이터가 데이터베이스처럼 복잡한 형식을 가지고 있을 때에는 읽기가 어렵다.

데이터 컨트롤은 바로 이와 같은 처리를 간단하게 해 준다. 데이터 컨트롤을 배치하고 다른
컨트롤과 연동하도록 설정하면 데이터 엑세스는 대단히 간단해진다. 사용자는 그 데이터를 어
떻게 처리할지에 대해 프로그램 기술에 전념할 수 있게 된다. 이처럼 데이터 컨트롤은 기존의
데이터베이스의 데이터를 표시, 추가, 수정, 삭제하는 수단을 제공하는 것이다.

데이터 컨트롤에서 사용하는 데이터베이스의 타입은 00ㅁㅁ6어 속성에서 Access, dBASE,
Excel, FoxPro, Lotus, Paradox, Text= 지정한다.

DatabaseName 속성은 처리하는 데이터베이스 파일명을 지정하고 RecordSource 속성
은 데이터베이스 내의 테이블을 지정한다.
그 후 폼 상에 불러들였던 데이터를 표시하는 텍스트 박스 등을 배치하여 처리하는 방법도
기술된다.
음은 데이터 컨트롤과 연결할 수 있는 컨트롤의 예이다

체크박스 (CheckBox)              콤보 박스 (200020ㅁ80※×)
이미지 (Image)                   OLE 컨테이너 (OLE)
벨 (Label)                    DB 2|AE (DBList)
픽쳐 박스 (PictureBox)            DB 콤보 (08000020)
텍스트박스 (TextBox)                DB 그리드 (28210)

리스트 tA (ListBox)

예를 들면 폼 상에 데이터 AESS 배치하고 DB 그리드라는 표 계산 컨트롤을 배치한다
(이것은 [프로젝트(82)]-|[구성 요소(0)|를 이용하여 도구 상자에 추가한다). 그리고 양쪽을 관
ㅇ

련짓는다. 또 데이터 AE=S2] Connect 속성에서 Excel 데이터 형식을 지정한다. 그 외 몇
개의 AAS 종료하면 작성한 속성에서 Excel 데이터 표 계산의 처리가 가능하게 된다. 이 관
계를 그림 8-18에 정리해 보았다

271


===== PAGE 269 =====
272

Chapter 8

(3)

컨트롤의 사용

| 데이터 베이스 파일 ㅣ 디스트 상에 있는 액세스, 디베이스 엑센 So} 데이터 형식
| 데이터 액세스
데이터 공급

ㅣ 데이터 HES} 06 그리드 컨트롤 ㅣ

—>| ㅣ 이미지 aes |

— | 텍스트 박스 컨트롤 |

—> i    기타     ㅣ
데이터 컨트롤의 처리는 초보자에게는 너무 어려우므로 본 책에서는 더 이상 bite

않는다. 많은 양의 데이터를
롤에 대해서 몰라도 곤란한

LULU

처리하는 본격적인 프로그램을 만드는
일은 없을 것이라고 본다.

사람 이외는 데이터 컨

메뉴(4600)

개체(메뉴 윈도우의 항목)

속성                  메뉴 항목

Caption                  2444 (P)

Checked                 AS (C)

Enabled                  유효 (6)
HelpContextID             도움말 HeAS WS (H)
Index                    인덱스 (×%)

Name                    이름 (M)
NegotiatePosition                     ARI (O)

ShortCut                      단축키 (6)

Visible                                   HA\(V)



===== PAGE 270 =====
8.24 메뉴(\4/604)

mz

명

윈도우 애플리케이션에서 메뉴 바의 작성은 메뉴 편집기에서 한다. 메뉴는 메뉴 타이틀, 서
브 메뉴 타이틀, 구분선, 체크 기능 등으로 구성된다. 메뉴 타이틀은 4단계까지의 계충을 가
질 수 있다. 하나의 메뉴 항목마다 화면상에서 다음과 같은 설정을 한다(그림 8-19참조).

매뉴 에디터의 기동
[도구(1)]-[메뉴 편집기0/)]를 클릭한다.

메뉴 에디터의 항목
[캡션(6)] : Caption
메뉴 타이틀을 입력한다. “:”의 So] 기술하고 WE “Caption” = 속성 이름이다. 코드
에서 설정한 때 이 이름을 사용한다. 이곳에 “ ”를 입력하면 구분 Ao] 표시된다.
다음처럼 하면 액세스키를 설정할 수 있다 메뉴 바 항목에는 [씨11+액세스키로 그 항목
이 반전 표시된다. 또 드롭다운 메뉴의 경우는 액세스키를 누르면 그 항목 선택이 된다.
인쇄(&『)                    입
민쇄(2)                      |

모비

3 18
mye 40H

=

it

메뉴를 선택할 때 직접 실행되는 것이 아니므로 일단 다이얼로그 박스가 표시되는 프
로그램 AVS 할 때에는 흔히 메뉴 항목의 문자열 뒤에 “...”을 붙인다. 예를 들면

“파일 열기(0)..."
라는 캡션 명으로 한다.

[이름(\4)] : Name

코드 중에서 메뉴 항목에서 액세스할 때에 사용하는 식별 명(컨트롤 명)을 입력한다.

HelpFile 속성을 At
Bes 가리키기 위한 고

273


===== PAGE 271 =====
Chapter 8

컨트롤의 사용

[네고시에이터 위치(60)] : negotiateposition
0ㅁ690119160051101 속성을 선택한다. 이 속성에서 컨테이너 폼 내에 메뉴를 표시
및 그 방법을 설정한다.             |

[제크(611 : Check               |

메뉴 항목의 좌측에 체크 마크을 붙인다. 이것으로 메뉴 커맨드를 On/OnfAsde A
정할 수 있다.                      |

[유효(6)] : Enabled

이 체크 YAS 꺼두면 메뉴 항목이 SS HOS 표시되고 사용할 수 없다는 것을 나타낸
다. 실제로는 이 항목을 상황에 따라서 실행시에 설정한다.

[표시(/)] : Visible
HAS 하면 메뉴 SSS 메뉴로 표사하벼 V7t 있는 것이 HEROIC, 이 SSR 실
HAO] 상황에 따라서 메뉴 항목의 표시 자체가 필요/불필요의 경우로 설정된다.

[원도우 리스트(00)] : WindowList _
이 체크 YAS V 표시하면 현재 열려 있는 작은 폼 보기를 메뉴 컨트롤로 표시한다.

tr
A
[꾸

디자인할 때 현재 선택되어 있는 메    계를 변경한다, 메뉴는 4단계까지 작성할 수

있다.                                                          |

같은 레벨의 메뉴 단계 내에서 현재 선택되어 있는 항목을 상하로 이동한다.

[다음으로(비)]

선택 항목을 다음 sow 이동한다. 실제로는 이 항목을 상황에 따라서 실행시에 설
정한다.

현재 선택된 Bo] 위로 1행 삽입한다.

[삭제(1)]
현재 선택된 줄을 삭제한다.

ih
ee

Hl

me
ont
00
et
ot
fell

|고 메뉴 에디터를 닫는다.

274



===== PAGE 272 =====
8.24 메뉴(4604)

설정을 포기하고 메뉴 에디터를 닫는다.

메뉴 편집기 항목 설정 예
메뉴 편집기에 의한 실제의 설정 예를 제시한다. 이 설정 예는 뒤에 있는 샘플 프로그램에서 사
용완다,

인덱스 단축 키 Al 크      H| 고
a (ar)                       mnuFile
- + -AlFE(&N)         mnuFileltem       0
…‥…:ㆍ불러오기(&0)... ㅣ mnuFileltem           1
‥…-저장(&9)            mnuFileltem           2
=               mnuFileltem      3                   HAS 넣는다
-- BE (8X)                    mnuFileltem               4
설정 (&S)                       mnuSettei
‥문자 A4(&C)      mnuSetteiltem     0
~Ha (&B)               mnuSetteiCol         0                    Vv
DeeatZt (&R)        mnuSetteiCol     1           V
eee파랑 (&L)                  mnuSetteiCol           2                        V
SuesAY (&G)                mnuSetteiCol          3                      Vv
eee                     mnuSetteiltem      1       Z                구분선을 넣는다
‥ㆍ볼드체(&8)           mnuSetteiltem       2 | (Ci)+(B)) Vv
ㆍ 이탤릭체(&|)           mnuSetteiltem         3      [여01+0]

FHS PREGA C14 AE 작성한 LS GEG PR OP) RO 마뉴 AAT
를 기입할 때어는 필요가 없다.

AQ) 이 표에서는 [.….]은 계층 1단계를 나타낸다. 이것은 — -로 조정한다.

주 3) [도움말 텍스트 ][네고시에이터 위치 19 A Tee 리스트 ]는 표준 그대로이다,

4) [이름 ]은적당한 것이 좋지만 YOU "000를 붙이는 추세다.

플로 램
앞의 메뉴 설정 예를 실제로 사용한 프로그램을 제시한다. 디스크 상에서 파일을 읽고 리스트 박
스에 표시한다. 그 데이터를 추가/삭제해서 저장한다. 이때 문자색과 문자 스타일을 설정할 수 있다.

속성 설정

Text                         Text                          “추가항목"
Commandi          Caption           Sa Jf
Command2          Caption            “삭제”

주) 리스트 은 표준 그대로 사용한다.

275


===== PAGE 273 =====
Chapter8 컨트롤의 사용

el

Private Sub Form_Load()
List1.Font.Bold = False
List1.Font.Italic = False
mnuSetteiltem(2) .Checked = False
mnuSetteiltem(3) .Checked = False
mnuSetteiCol_Click (0)

End Sub

Private Sub Command1_Click()
List1.AddItem Text1.Text
List1.SetFocus

End Sub

Private Sub Command2_Click()
Dim i As Integer

'초기에 설정한타

'볼드체 제거

'이탤릭체 제거

'볼드체 메뉴에 표시를 한다

'이탤릭체 메뉴에 표시를 한다
'검정색으로 설정

!16×<[|을 추가

‘List AMS 되돌린다

‘BES 항목 제거

For i = Listl.ListCount - 1 To 0 Step -1

If Listl.Selected(i) = True Then List1.RemoveItem i
Next
List1.SetFocus                         ‘Listi@ AAS 되돌린다
End Sub

Private Sub mnuFileItem_Click(Index As
Dim buf As String

Select Case Index
Case 0
List1.Clear
Case 1
List1.Clear
Open "c:\mydata\teldt.txt" For
Do While Not EOF(1)
Line Input #1, buf
List1.AddItem buf
Loop
Close #1
Case 2
Open "c:\mydata\teldt.txt" For
For i = 0 To LIstl ListCoumt -
Print #1, List1.List(i)
Next
Close #1
Case 3   ,

Case 4
End
. End Select
End Sub

276

Integer)

'새로 만들기

'리스트 박스 Clear

'열기

'리스트 HA Clear
Input As #1

'파일 마지막으로 Loop

'리스트 박스에 추가표시 한다

'파일을 닫는다

Ae

Output As #1     '파일열기

1

'리스트를 한 행씩 저장

'파일을 닫는다

구분선

'아무것되 하지 않으면 코드 불필요



===== PAGE 274 =====
8.24 메뉴(\/604)

Private Sub mnuSetteiCol_Click(Index As Integer)

Select Case Index

Case 0                            '검정
List1.ForeColor = RGB(O, 0, 0)
Case 1                           eae
List1.ForeColor = RGB(255, 0, 0)
Case 2                            '파랑
List1.ForeColor = RGB(0, 0, 255)
Case 3                              '녹색
List1.ForeColor = RGB(0, 255, 0)
End Select
For i = 0 To 3
mnuSetteiCol (i) .Checked = False ‘A/S 표시 제거
Next
mnuSetteiCol (Index) .Checked = True ‘Aja 표시 부여
End Sub
Private Sub mnuSetteiItem_Click(Index As Integer)

Select Case Index

Case 0                       문자색/코드 불필요

Case 1                            '구분선/코드 불필요

Case 2                            '볼드체
mnuSetteiltem(2) . 아16아60 = Not mnuSetteilItem(2) .Checked
List1.Font.Bold = Not List1.Font.Bold

Case 3                            '이탤릭체

mnuSetteiltem(3) .Checked = Not mnuSetteiItem(3) .Checked
List1.Font.Italic = Not List1.Font.Italic

End Select
End Sub
0 메뉴 바 항목을 클릭하면 드롭다운 리스트가 표시된다.
© 하위 메뉴가 있을 때에는 》마크가 붙는다.

© [볼드체]와 [이탤릭체]는 체크 표시 가 On/Off 된다.

@ 색 BRL 4개 중 하나만이 \있게 된다.

© BEAM [이탤릭체]는 단축키가 표시된다. 이 단축키를 누르면 직접 메뉴를 선택할 수

© 텍스트 박스에 입력하고 추가를 클릭하면 리스트 박스에 추가된다.

O AAS 클릭하면 현재 선택되어 있는 항목이 제거된다.

 [파일("]-[열기(0)]-[저장(8)]으로 파일 읽기/쓰기를 한다.

© [파일001-[신규 작성0)|로 리스트 박스를 제거한다.
0 [파일0"1-[종료001로 이 프로그램을 종료한다.

는 ADS 누르면 [파일08")이 반전 선택된다.

@ 이후 떠, Ge 메뉴 선택할 수 있다.

@ 메뉴 항목의 끝머리에 있는 문자 키 입력으로 선택할 수

있다.
277


===== PAGE 275 =====
278

Chapter 8

컨트롤의 사용

그림 8-19

화면1 메뉴 에디터를 편집중인 화면
[도구(1)]-[메뉴 편집기(1)]를 선택한다

이 EO] 여러 가지 설정할 —
수 있는 속성을 여기에 입력해
간다

메뉴 구성을 표시한 리스트 박
A 여기에서 항목을 선택하면 -ㄱ
위의 설정 화면에 표시된다. 또

— ㅡ로 메뉴의 깊이를 변경할
수 있다

화면2 디자인할 때의 화면

설정한 메뉴

리스트 박스

화면4 [【설정(6)]을 열다
있을 때에는 마크가 붙는다

하위 메뉴가

[그

화면3 실행해서 [파일(『-)] 메뉴를 열다
새로운 데이터를 보존한다. 이름과 SHS 추가했다

[불러오기(0);로 잃은 데이터

체크 마크가 표시되어 있다

고딕체 파랑색으로 표시되어 있다



===== PAGE 276 =====
apa

그 의 기본 용법

여기에서는 지금까지의 설명하지 않았던 중요한 기능에 대해서 살펴
보자. Visual 88610은 단지 화면에 표시하는 것은 간단하지만 그 단계
를 넘어서 정리를 하려고 하면 그 순간 복잡한 기능을 학습할 필요가 있

도 꼭 기억해 두고 싶은 기본 기법에

다. 따라서 이 장에서는 그 중에서도 꼭
대해서 살펴보자.


===== PAGE 277 =====
280

Chapter9 그 외 기본 용법

애플리케이션 중에서 메시지를 표시하거나 사용자가 입력을 하기 위해서는 적당한 컨트롤
을 배치하는 것이 기본이다. 그러나 이것 이외에 대화 상자를 사용하는 방법도 있다. 대화 상
자는 필요할 때에 화면상에 나타났다가 역할이 끝나면 사라진다. 이 대화 상자는 BS] 레이아
웃에 묶이지 않고 자유스럽게 사용할 수 있다. 또 대화상자는 스스로 설계도 가능하고 정의된
대화 상자를 사용할 수도 있다. 정의한 대화 상자에는 MsgBox} InputBox7} 있다. 우선
MsgBox] 대해서 알아보기로 하자.

부

148880는 에러 경고와 주의 등의 짧은 메시지를 표시하는 데 사용하고 보조 기능으로서
는 예, 아니요 등의 선택 입력 기능이 있다. 118880×는 함수이며 AALS 다음과 같다.

MsgBox (Prompt [, button] [, title] [, helpfile, context!)

promt 대화 상자의 메시지로 출력되는 문자열로 최대 길이는 1024자이다.

buttons 표시한 HES] 종류와 개수, 사용하는 아이콘의 스타일 SO 표 9-1의 정수 또는 값
으로 설정한다. 생략하면 OOKH ERO] 된다. 각 그룹에서 한 } 개밖에 설정할 순 없
지만 다른 그룹의 설정과 동시에 지정할 수 있다. 그 경우는 각 그룹으로부터 값을
하나씩 선택해서 가산한 합계액을 지정한다. 이것은 논리 연산자를 사용해서

vbYesNo Or vbquestion or vbDefaultButton2

처럼 지정하는 것이 간단하고 정확하다.
title fs} 상자의 제목 표시줄에 표시할 BASS 지정한다. 생략하면 애플리케이션 명
이 표시된다.
helpfile 대화 상자에 상황 의존의 도움말을 설정하기 위하여 사용하는 도움말 파일의 이름
이다. helpfileS 지정한 A$ Context 지정할 필요가 있다.
context 도움말 토픽에 지정한 컨텍스트 번호(도움말 정보의 번호)를 나타낸다.



===== PAGE 278 =====
9.1 MsgBox] 의한 정보 표시

점 수   가 내 은

그룹 1    vbOKOnly             0 | OK HES 표시
vbOKCancel            1| OK, AA HES 표시
vbAbortRetrylgnore     2| Stop, MAS, 무시 HES 표시
vbYesNoCancel         3 | 예, 아니오 AA HES 표시
vbYesNo             4 | 예, 아니오 HES 표시
vbRetryCancel         5 | MAH 취소 WES 표시
그룹 2    vbCritical             16 | SCH 메시지 아이콘을 표시
vb Question           32 | 질의 경고 아이콘을 표시
vbExclamation         48 | 메시지 경고 아이콘을 표시
vbInformation         64 | 메시지 정보 아이콘을 표시
그룹 3   vbDefaultButton1       0 | 첫번째 버튼이 초기값이다
vbDefaultButton2     256 | = 번째 버튼이 초기값이다
vbDefaultButton3     512 | 세 번째 버튼이 초기값이다
그룹 4    vbApplicationModal     0 | 애플리케이션 모달로 한다

\4/69ㅁ80×를 종료하지 않고 현재의 어

플리케이션으로는 돌아가지 않는다

다른 애플리케이션으로 이동

vbSystemModal     4096 | 시스템 모달로 한다

MsgBoxS 종료하지 않고 어떤 애플

리케이션으로도 돌아가지 않는다

주1) helpfile, contextS 지정할 때 떼으로 도움말 토픽을 참조할 수 있다. 이 경우에는 도움말 HEE 표시
된다.

AQ) 취소 버튼이 표시되어 있는데 휘도 같은 기능이 된다.

주3) 표준 버튼 지정을 하면 그 버튼이 파선표시가 되고, 60빼를 클릭하면 선택 THO] 된다.

ZA) 그룹 2의 지정에 OH 경고음도 4종류로 변화한다.

선택된 버튼에 의해 표 9-29] gto] 리턴된다. 정수명을 사용해도 SA.

4A
0 oy =

as «                               HA                                     =

확인                 |                     vbOK
취소                2                    vbCancel
중단                3                    vbAbort
AHA|               4                    vbRetry
무시                5                    vblgnore
예                                  6                                     vbYes
아니오                    ie                            vbNo

음 지정에서 MsgBoxS 표시한다.

281


===== PAGE 279 =====
Chapter9 그 외 기본 용법

디풀변로빌렘

vbYesNo                     예, 아니오 HES 표시한다
vbQustion                   서로 의논한 메시지 아이콘을 표시한다
vbDefaultButton2            아니오 HES 표준 버튼으로 한다
"C:\Window\help\dialer.hlp" 의 컨텍스트 번호1000을 헬프로 한다

또 리턴 값을 판정해서 예가 선택되면 다음의 MsgBox S 표시한다. 즉 여기에서 사용하고
있는 ESTE 윈도우 시스템에 있는 것을 BMS BEST 내용은 본 프로그램과는 관계
가 없다.

속성 설정
개체                       속성                   설정

Commandt           Caption    |          “MsgBox-Test'

코드

Private Sub Command1_Click()
Msg = "다음의 MsgBox 표시합니까 (F1SSeh’
Btn = vbYesNo Or vbQuestion Or vbDefaultButton2   “HE Ol 정의
Or VbMsgBoxHelpButton

Title = "MsgBox 2| 테스트"                      타이틀을 붙인다
Help = "c:\windows\help\dialer.HLP"             ‘esa 파일
Ctxt = 1000                                 컨텍스트 번호
Ret = MsgBox(Msg, Btn, Title, Help, Ctxt)
If Ret = vbYes Then                            ‘(js 선택한 경우
Ret = MsgBox("[OJ7} 선택되었다." , "\4/60ㅁ0×테스트 2")
End Tf
End Sub
동작의 확인

(0 실행해서 MsgBox-Test HES 클릭하면 MsgBox 7} 표시된다.
(2) 11을 누르면 도움말이 표시된다.
(3) 예를 클릭하면 다음 MsgBox 7} 표시된다.

282


===== PAGE 280 =====
9.2 _1004[20×에 의한 입력

화면1 실행 화면                화면2 \69ㅁ0×168!를 클릭하면
1011                            새롭게 다음 창이 나타난다

=a]

화면3 이것이 표준 버튼이므로    화면4 예를 클릭하면 이
점선이 붙여져 있다              화면이 표시된다

대화 상자에는 정형 대화 상자와 비정형 대화 상자 2종류가 있다. 정형 대화 상자는 대화 상자를 닫지 OL
으면 다른 윈도우로 이동할 수 없으나 비정형 대화 상자는 그 SHAS 표시한 채 다른 부분에 처리를 S
길 수 있다. 어떤 폼에서 다른 폼을 부를 때 정형/비정형은 다음처럼 지정한다.

Form1. Show 1 ………정형으로 된다
Form1, Show 0 ………비정형으로 된다(0은 생략 가능)

(String) == Variant °]4 InputBox= 함수이다. 1404+80*의 함수는 다음과 같다.

283


===== PAGE 281 =====
Chapter9 그 외 기본 용법

      InputBox(Promptl, titlell, defultll, xposll, yposll, helpfile, context)

propmpt            대화 상자의 메시지를 표현하는 문자열

title              대화 상자의 제목 표시줄에 표시할 문자열을 지정하며 생략하면 애플리케
이션.이름이 지정된다.

default            처음 텍스트 박스에 계정값으로 표시될 문자열로서 생략하면 공백이 된다.

xpos              화면의 좌측 끝부터 대화 상자의 좌측 끝까지의 수평 방향의 Ae|(twiptt
위)이며 생략하면 ※방향이 화면 중앙에 배치된다.

Ypos            화면 상단부터 대화 상자의 위치까지의 수직 방향의 거리([\17단위)이며
생략하면 ?방향이 화면 위쪽 끝부터 1/32] 위치에 배치된다.

helpfile           대화 상자에 상황 의존의 도움말을 설정하기 위하여 사용하는 도움말 파일

의 이름으로 1610[116을 지정한 경우는 Context 지정할 필요가 있다.
이 설정을 하면 자동으로 도움말 버튼이 표시된다.
context           도움말 토픽에 지정한 컨텍스트 HSS 나타낸다.

     확인 버튼이 선택 또는 68@가 눌려지면 텍스트 박스의 USS 되돌린다.
|        취소 버튼이 선택되면 빈 문자열(" ")을 되돌린다.

.|플[니로트|램

화면 중앙부에 InputBoxS 표시한다. 입력이 공백 문자열이나 취소 HES] Selo] 아니라
면 계속해서 화면 좌측 AHF] InputBoxS 표시한다.
또 리턴 BS 판정하고 취소 버튼의 Seo] 아니라면 다시 InputBoxS 표시한다.

A
속성 설정

개체             촉성                   설정
Command1                                    Caption                    [                                   "TInputBox-Test"
코드

Private Sub Command1_Click()
Msg = 아무런 글자나 입력을 하여 주세요"

Title = "InputBox2| 테스트"         ‘EUS = 붙인다
Ret = InputBox(Msg, Title, "1")      AS Ge 1
Tf Ret < “" Then               입력되어 있으며 취소 HES 클

1)
있으
릭하지 않으면

284


===== PAGE 282 =====
9.2 InputBoxol] 의한 입력

Title = "InputBox2| H/AE2"      '계정값을 앞에서 입력한 값으로 한
         다. 표시 위치를(200,200)으로 한다.
Ret = InputBox(Msg, Title, Ret, 200, 200)
End If
End Sub

동작의 확인
@ 실행하여서 InputBox—-Test=2 클릭하면 ㅁ04[80가 표시된다.
@ 취소 HES 클릭하거나 입력이 “ "라면 종료한다.
(3) 뭔가 입력하면 +S InputBox7} 좌측 위에 표시된다.
@ 이때의 계정 값은 전의 입력 값이 된다.

화면1 실행 화면

[그

화면2 InputBox—TestS 클릭했다

계정 값의 10] 표시되어 있다(여기서 1234 "라고
입력해서 엔터키를 누르거나 확인을 클릭)

화면3 바르게 입력하면 이번은 화면 좌측 위에 다음 InputBox7} 표시된다

전의 입력값이 표시되고 있다

285


===== PAGE 283 =====
Chapter9 그 외 기본 용법

Visual 88810 프로그램을 실행중에 네 변의 가장자리를 드래그하면 폼 크기를 변경할 수
있다. 그러나 그 위에 배치된   컨트롤 크기는 변경되지 않으므로 균형이 맞지 않는다. 그것을
해결하는 WHS 윈도우의 “Peau” of “그림판” 처럼 작업 영역과 AS 연동하여 크기 변형
이 가능하게 한다.

작업 SAS 가능한 크게 하고 싶을 때 사용자가 직접 기교적인 코드를 입력하며 방법은 다
음과 같다.

한다

Form Resize()S 사용
폼의 크기를 변경하면 For
에서 필요한 크기를 조정할

Resize()ZH= 이벤트가 발생하므로 Form ㅁ68126( )에서 속성 중

01503. .
수 있게 입력(다음 항)을 한다.

크기의 재 계산
폼 크기를 마우스로 변경하면

Form1 .Width
Forml .Height

는 속성이 변한다. 이 변화를 반영시킨 것이 컨트롤(예를 SH Text!) 속성이다.
Text1.top             Form 2} 상단에서의 거리

Text1.Left            For 2| 좌측 끝에서의 거리

Text1.Width            Text19| 가로 =

Text1.Height           Text19| 세로 =

를                    19-3), 이것에 연동하여 크기를 변경한다. 실제로는 폼 크기, 제목 표시
줄의 두께와 상하 프레임의 두께를 빼야 한다.

픽저 박스 컨트롤의 패러   HASH 경우는 AutoRedraw= '[07146로 하고 크기 변경이 될 때
마다 자동으로 다시 그림을 그리도록 한다. 그렇지 않으면 원래 그림이 없어질 수도 있으므로 조
심해야 한다.

286


===== PAGE 284 =====
9.3 폼 크기와 컨트롤 크기의 연동

|                                                 Form1.Width
|            <                                                                                                     -
|                                                                                                                             4
                                                      Text1.Top
|
|
|                  Text1.Left
|                                                                     Text1                         Text1.Height         Form1.Height
Text1.Width
\
최소화 버튼

크기 연동 변경에서 주의할 것은 윈도우에 표준 wy (AAS) HES 클릭할 때의 처리이다. =
HES Sas+H Resize() 이벤트가 발생한다. 그러나 최소화되고 있는 폼은  이동과 크기를 변
할 수 없으므로 이것을 행하면 실행할 때 에러가 발생한다. 이를 막으려면 168126() 이벤트 be
서 다음과 같이 입력하면 된다.

If WindowState = 1 Then Exit Sub 0012

48
에
b>
[01
ㅁ
In
모
[모
2!
tu
에
a
52
rr
모

\1000\8【846는 윈도우의 표시 AHS 설정/취득하는 것이다.

WindowState          0 - Normal (Al 값)
1 - 최소화
2 - 최대화

띠플녀로티램티

폼 상에 텍스트 박스와 두 개의 명령 버튼, 한 개의 라벨이 있다. 폼을 변경하면 텍스트 박
스가 연동되어 크기가 변경된다. 명령 버튼과 라벨의 크기는 변하지 않지만 적절한 위치로 이

동한다.

287


===== PAGE 285 =====
Chapter9 그 외 기본 용법

속성 설정

1611       MultiLine        True
Label      BoderStyle      1 - 실선
Caption            "텍스트 YAS 폼과 연동해서 크기를 변경한다"
Command1 Caption         "OK"
Command2 Caption         "Cancel"
코드

Private Sub Form_Load()

Text1.Text = "1234567890ABCDEFGHIJKLMNOPORSTUVWXYZ
abcdefghijklmnopgrstuvwxyz"
End Sub

Private Sub Form_Resize()
If WindowState = 1 Then Exit Sub 최소화 버튼

Tf Forml.Width < 5535 Then        '이것보다 가로 크기를 작게 하지 않음.
Forml.Width = 5535: Exit Sub

End If

If Forml.Height < 1815 Then    | ： '이것보다 세로 크기를 작게 하지 않음.
Forml.Height = 1815: Exit Sub

End If

Text1.Width = Forml.Width - 1440 ‘Text192| 가로 폭의 변경

Textl.Height = Forml.Height - 960 ‘Text1°| 높이 변경

Command1l.Left = Forml.Width - 240 - 975 ‘Command12| 가로 위치 변경
Command2.Left = Forml.Width - 240 - 975 ‘Command2Q| 가로 위치 변경
Label1l.Top = Forml.Height - 735   ‘Label1 2} 세로 높이 HA

End Sub

Private Sub Command1_Click()
End

End Sub

Private Sub Command2_Click()
End

End Sub

주) 수같인 1440, 960, 240, 975, 735 디자인할 따의 각종 Width, Top, Left HS 토대로 얻은 것

동작의 확인
© 연동해서 네 WS 드래그하면,
@ 텍스트 박스는 그 크기를 바꿀 수 있다.
© 명령 버튼은 항상 화면 위에 놓인다.

288


===== PAGE 286 =====
9.3 폼 크기와 컨트롤 크기의 연동

@ 라벨은 항상 화면 아래에 놓인다.
© 폼은 디자인할 때의 크기보다 작게 되는 일은 없다.
© 최소화, 최대화 버튼에도 바르게 대응한다

bedefghijkimnoparstuywxyz]

화면2 네변을 드래그 하여 사이즈 변경한다

띠플더로틴램터

그림이 표시되고 있는 폼 크기를 변경하는 예이다.
속성 설정

Picturel                                               BackColor

rot
ies

코드

Private Sub Form_Load()

Picturel.Picture = LoadPicture("c:\mydata\ship.bmp")
End Sub

Private Sub Form_Resize()

If WindowState = 1 Then Exit Sub      '최소화

If Forml.Width < 5535 Then           '최소 가로 크기
Forml .Width = 5535: Exit Sub

End If

289


===== PAGE 287 =====
Chapter9 그 외 기본 용법

If Forml.Height < 1815 Then          최소 세로 크기
Forml.Height = 1815: Exit Sub
End If
Picturel.Width = Forml.Width - 400    가로폭 HA
Picturel.Height = Forml.Height + 600 =0| 변경
Exit Sub
End Sub

화면2 크지가 변경되었다

290



===== PAGE 288 =====
9.4 Printer 개체

애플리케이션 중에서 데이터를 인쇄할 때 Printer 개체를 사용한다. 종래의 퀵 베이직 등
에서는 인쇄가 한 BY 단위의 시리얼 출력이었다. Visual 28810의 Printer 개체에 의한 출력
은 보통의 윈도우에 의한 인쇄와 같이 페이지 단위로 인쇄된다.

애플리케이션의 화면상에 있는 텍스트와 도형을 인쇄하는 것만이 아니라 코드를 기술해서
직접 프린트할 문서, 선 그럼을 프린터할 수도 있다. 한 페이지 분의 출력이 끝나면 EndDoc
메서드를 실행함으로써 인쇄가 된다.

Sas           기능

ColorMode       컬러나 흑백 중에서 어떤 것으로 인쇄할 것인지를 설정
Copies          인쇄 부수를 설정

CurrentX        다음에 행하는 출력의 수평 좌표를 설정
CurrentY        다음에 행하는 출력의 수직 HHS 설정
DeviceName     프린터 드라이브가 서포트하는 디바이스를 변경
DrawMode       그림 출력의 Ws 설정

DrawStyle        그리는 선의 종류를 설정

DrawWidth       그러는 선의 크기를 설정

DriverName      프린터 드라이버 SS 설정

Duplex          양면 인쇄를 행할지 말지를 설정

FillColor         도형 내부의 색칠할 색을 설정

FillStyle         도형 내부의 색칠 패턴을 설정

Font            폰트 WAS 결정

FontBold         볼드체를 설정

FontCount        이용 가능한 HES 변경

『0ㅁ01118110         이탤릭체를 설정

FontName        사용하는 폰트를 설정

Fonts           이용 가능한 폰트의 이름을 변경

FontSize          폰트 크기를 설정

FontStrikethru    취소선을 AA

FontTransparent 문자의 HANS 투명하게 할 것인지를 결정
FontUnderline     밑줄을 설정

ForeColor        HAMS 설정

hDC           이 개체용의 HSS 바꾼다

291


===== PAGE 289 =====
Chapter9 그 외 기본 용법

속성명           =

Height           개제의 높이를 설정

Orientation        인쇄방향을 세로/가로로 설정

Page       현재 페이지 HeS 변경

PaperBin        BASS 지정해서 그것을 미정 취급으로 한다
PaperSize        용지 크기를 설정

Port            프린터에 SAIS 때 HE BS 변경

PrintQuality      프린터의 해상도를 나타내는 값을 설정         2
ScaleHeight      개체의 수직 방향의 SOLS 설정

ScaleLetft        개체의 좌측 끝의 수평 좌표를 설정

ScaleMode      개체의 좌표계의 단위를 설정

‘ScaleTop        개체의 위쪽 끝의 수직 ABS 설정

ScaleWidth       개제의 수평 방항의 높이를 설정

TrackDefault      윈도우의 제어판에서 프린터 AMS 반영할 AAS 설정
TwipsPerPixelX  Halol| 수평 방향의 HAS twipS 바꾼다
TwipsPerPixelY 7Ha]0| 수직 방향의 BAIS twip+S 바꾼다
Width            개체의 SS 설정

ZOOM        인쇄 결과의 확대와 BAS 백분율로 설정

메서드      기능

Circle      원 타원 원주를 oad.

EndDoc    Printer 개체에 보낸 데이터를 실제로 프린터에 SS 지시
KillDoc     현재 실행되고 있는 인쇄 화면을 곧바로 종료

Line         Mit 사직형을 그럼

NewPage 현재 페이지를 종료하고,다음 페이지로 넘어간다
PaintPicture 그래픽 m2! omp, .mnf, .emf, ico, .dib)\S 그린다

_Print        문자를 출력
PSet        점을 출력
Scale      좌표계를 정의
Scalex     폭의 C1912 ScaleMode 속성의 설정에서 다른 것으로 변환
80816     높이의 단위를 ScaleMode 속성의 설정에서 다른 것으로 변환

TextHeight 현재 폰트에서 SASS. 인쇄할 때의 높이를 바꾼다
TextWidth Sal 폰트에서 문자열을 인쇄할 때의 폭을 바꾼다

Printer 개체의 사용 방법
Printer 개체는 위에 나타낸 것처럼 많은 기능을 가지고 있으며 그 중에서 중요한 기능을 구체
적으로 알아보자.

printer .EndDoc

292



===== PAGE 290 =====
9.4 Printer 개체 4

프린터에 출력한 데이터는 프린터 버퍼에서 자동으로 인쇄되지만 작은 데이터인 경우에는 버퍼
를 이용하지 않는다. 이럴 때 프로그램에서 Solo] 출력하라고 지시하는 명령이다.

용지 방향을 세로로 하면 화면은 가로가 된다.

출력할 문자를 굴럼체로 한다. 이 ES 지정은 윈도우의 SE 지정 화면에 나오는 SES 사
용한다.

Picturel 2] 그림을 (10,20)의 위치에 출력한다.

293


===== PAGE 291 =====
Chapter9 그 외 기본 용법

샘[]프더그는

기본적인 인쇄방법을 모델로 제시한다.

속성 설정

개체          속성            설정
6000013001     Caption         “인쇄”
Picture       Picture          .omp 파일을 설정한다
Text1         Text           “Text! 문자"
프로그램 코드

Private Sub Command1_Click()
Dim i As Integer

Printer.ScaleMode = 6    HAs 밀리미터로 함.
Printer.Orientation = 1            용지를 세로로 한다. 가로는 2
Printer.FontName = "굴림체"         '굴림체로 한다
217ㅁㄴ62 . Print                    한 줄씩 줄 바꿈
For i = 8 To 18 Step 2
Printer.FontSize = i           "문자 크기를 변경하여 인쇄
Printer.Print "인쇄 Demo 프로그램"
Next                        |
Printer.FontSize = 14              ‘EA Sle 14
Printer.FontName = "바탕체"         '바탕체로 한다.
Printer.Line (0, 35)-(80, 100), |, B WalS 사각으로 둘러싼다.
Printer.CurrentX = 10             '다음의 BA 출력 위치×
Printer.Currenty = 40              '다음의 문자 출력 위치
Printer.Print 761 . 06           '텍스트 박스의 문자 출력
Printer.PaintPicture Picturel, 10, 65 픽처 박스의 내용 출력
For i = 20 To 2 Step -2             OSH 출력
Printer.Circle (50, 70), i
Next
Printer. EndDoc                   인쇄 자동 개시
End Sub

(1 실행하여 인쇄 HES 클릭하면 소정의 인쇄가 행해진다.

294


===== PAGE 292 =====
9.4 Printer 개체

[으으
ee
2
3
[회

로그램

인쇄 0600 프로그램

인쇄 0600 프로그램
인쇄 0600 = =
인쇄 0600 프로그램

}
|

Text 1 문자

295


===== PAGE 293 =====
Chapter9 그 외 기본 용법

Visual 28810 애플리케이션에서는 마우스 이벤트와 키 이벤트는 중요한 사용자 인터페이

스이다. 다음에 그 규정들을 정리하여 제시한 구문 중에 “Object” 부분에는 컨트롤 명과 폼
명이 들어간다(예 : Commandl_Click( )).

또 보동의 neil 는 컨트롤을 사용하지만 컨트롤 배열 사용은 많지 않다. 그때에는
구문의 인수인 “Index As Integer” 를 사용한다.  ale : 들면   다음에 제시하는 011에서는

Private Sub Object ()                        컨트롤의 경우
Private Sub Object_Click(Index As Integer)   컨트롤 배열의 경우

이 된다. 배열이므로 그 요소를 as ㅣ 위하여 Index 7} 필요하다. 실제로 보통의 프로그램
에서는 컨트롤 배열을 ise      은 거의 없으므로 사용자가 보는 것은 앞의 서식이다. 여기
에서는 쉽게 알기 위해 (Index      -1008902 생략한 서식을 제시한다.

Click

Private Sub object_Click()

사용자가 개체 상에서 마우스 HES 클릭할 때에 발생한다. 그외 특별한 조작으로 발생할
수도 있다.

_DbIClick
      Private Sub object DbiClick

사용자가 개체 상에서 마우스 HES 더블 클릭할 때에 발생한다.

296



===== PAGE 294 =====
9.5 마우스 이벤트와 키 이벤트

2} DragDrop |

      Private Sub object DragDrop (Source As Control, X As Single, Y As Single)

Source C= 되어 있는 컨트롤의 이름
X,Y      드래그 앞에 놓인 마우스 HES] 수평/수직 위치
컨트롤을 FES 컨트롤 위에서 드래그 & 드롭하였을 때(조작 예시점) 발생한다.

DragOver ©

Private Sub object DragOver(Source As Control, X As Single, Y As Single, State As Integer)

Source 드래그 되어 있는 컨트롤의 이름
X,Y 드래그 앞에 놓인 마우스 버튼의 수평/수직 위치
state 소스 컨트롤과 목적 폼 또는 컨트롤의 위치 관계를 제시하는 값

0-소스는 목적의 범위 내에 들어갔다
1-소스는 목적의 범위밖에 나왔다
2-소스는 HAS 이동하고 있

드래그와 드롭 조작의 진행 중에 발생한다. 이때 마우스 버튼이 위치하고 있는 개체에 의해

a

Private Sub object_KeyDown(KeyCode As Integer, Shift As Integer)

KeyCode 눌러진 키의 코드, 특수 키의 경우는 BTS 사용하면 좋다.
 . 에 i vbKey(Fl) vbKeyHome(Home)
Shift 쉬프트 키 상태. 키의 상태는 제대로 분배되어 있으므로 중복 지정을 할 수 있다.
예를 들면 이 값이 6 이라면 [401와 (0이 눌러져 있다.

15

297


===== PAGE 295 =====
Chapter9 그 외 기본 용법

사용자가 키를 눌렀을 때나 그렇지 않을 때에 포커스를 갖고 있는 개체에서 발생한다. 이
두 개의 이벤트는 키가 눌러진 때와 그렇지 않은 양쪽의 타ㅇ iy  에서 처리할 때 편리하다.
이 이벤트는 BSS] 문자 키뿐만이 아니라 펑션 키와 쉬프트 키도 검출한다. 펑션 키 등의

we 정수를 사용하면 쉽게 알수 있지만 직접 해 보면 어느 값이 Bora] 알고 있으므로
수 값을 직접 써도 상관없다

인수 Shift 에서 Shift (Cm) (AW) 상태를 알 수 있다. 예를 들면 60때만이 눌러져 있는 것은
If Shift = 1 Then     0가 눌러져 있다

으로 알 수 있다. 값은 그 위치에 해당하는 2진수이다.

또 KeyDown/KeyUp2# 입력되는 <670006와 다음에 설명하는 KeyPress = 입력하
는 <6748001는 저리하는 값이 다른 것이 있으므로 주의해야 한다.

670006는 키보드로부터 읽는 때의 키 번호가 들어간다. KeyAsccii HE 그것은 48001
코드로 변한된 것도 들어온다. JS 들면 그 차이는 다음을 보면 알 수 있다.

: 키보드가 소문자 입력 모드로 되어 있을때

AS 눌렀다 : ( 8 를 입력할 예정)
KeyDown 2| 이벤트의 KeyCode= - 65
KeyPress 의 이벤트의 KeyAscii= — 97

Shi+A)S 눌렀다 : (A'S YAS 예정)
KeyDown 2| 이벤트의 KeyCode= — 65
KeyPress 의 이벤트의 *6/28011는 — 65

KeyCode = 입력된 키 번호는 키보드에 배치된 ㅅ키의 고유 번호(65)이다. 이 HSE FZ
트 키를 누르거나 누르지 않아도 고정되어 있다. 그러나 <6748011는 그것을 문자 코드(여기
에서는 소문자 8 )에 변환한 것이 들어오므로 소문자 를 나타내는 97이 들어오는 것이다.

이와 같은 처리를 하므로 문자 코드를 갖지 않는 펑션키 등은 <67『7688이벤트로 처리할

Es 수 없다.
이 이벤트에서 처리할 수 있는 문자의 값은 도움말에서 KeyCode 설정을 보면 알 수 있다.
중요한 값은 다음과 같다.

298


===== PAGE 296 =====
9.5 마우스 이벤트와 키 이벤트

정수          값         정수          이 9]

vbKeyBack     Ox8 6688    vbKeyLeft      0x25 8

vbKeyTab      Ox9    vbKeyUp      026 (|

vbKeyReturn    OxD    vbKeyRight     Ox2/ 6

vbKeyShift      Ox10 600    vbKeyDown    0x28. OW

vbKeyControl      Oxi! (0       vbKeyA            65       A (Ascii T= 2} 같음)
vbKeyPause    0x13    vbKeyZ       90    (Z)

vbKeyCapital      Ox14       voKeyO           48      ©) (Ascii Z=2} 같음)
vbKeyEscape    Ox1B _ [Esc]    voKey9       57    (9)

vboKeySpace    Ox20    vbKeyF1       Ox70 {ri

vbKeyPageUp   0x21    vbKeyF12      Ox7B
vbKeyPageDown 0x22   vbKeyNumpadO Ox60 ©

vbKeyEnd      Ox23    vbKeyNumpad9 Ox69 9)

vbKeyHome     Ox24 0009    vbKeyMultiply   Ox6A  &)

voKeyPrint    Ox2A   vbKeyAdd    Ox6B

vbKeylinsert   Ox2D   vbKeySeparator Ox6C

voKeyDelete    OX2E 6009    voKeySubtract Ox6D ㅁ

vbKeyHelp     Ox2F ff     vbKeyDecimal   OxGE  L)

vbKeyNumlock  Ox90 (ia    vbKeyDivide    Ox6F

KeyPress

Private Sub Object_KeyPress(KeyAscii As Integer)
KeyAscii         눌러진 키의 Ascii FE

Ascii 문자가 입력될 때에 포커스를 갖고 있는 개체에 발생한다. 작성한 이벤트 프로시저
중에서 KeyAscii HS 변경하면 다른 문자를 입력했다고 할 수 있다. 또 675801는 0으로
하면 입력하지 않았다라고 할 수 있다. 예를 들면

If KeyAscii<&H30 Or &H39<KeyAscii Then KeyAscii=&H30

으로하면 숫자 이외의 문자가 입력될 때 강제로 '0 을 입력값으로 변경된다.
KeyPress 이벤트는 펑션 키와 600를 검출할 수 없다. 단지 Ascii 문자만을 처리하고 A
을 때 사용하는 편이 좋다.

299


===== PAGE 297 =====
Chapter9 그 외 기본 용법

"Private Sub object MouseDown(Bution As Integer, Shift As Integer, X As Single, Y As Single)

Private Sub object MouseUp(Button As Integer, Shift As Integer, X As Single, Y As Single)

Button]: 버튼의 조작 여부를 나타낸 값

15           2   1  0
LL 608
meee 010:

Shift 쉬프트 키 상태. 용법은 KeyDown 9S] 이벤트와 동일
고       마우스 커서(목적상의)의 현재 위치

이 두 개의 이벤트는 마우스
현재 버튼의 종류를 구별할 수

냉             트는
별할 수 있다(3110, Dblclick ope aA  구별할 수 없다). 또 (Shift)
, (Chi), (Ait) 등의 보조키를

합하여 사용할 수 있다.

-MouseMove |

Private Sub object_MouseMove(Button As Integer,
Shift As Integer, X As Single, Y As Single)

Button 어느 버튼이 조작될까를 나타내는 값
Shift 쉬프트 키 상태. KeyDown 이벤트와 동일
x,Y     마우스 버튼의 현재 위치

이 이벤트는 사용자가 ㅁ Leia! ile  있을 때에 연속적으로 발생한다. 현재 마우스 버
튼이 통과하고 있는 개체에서 검출된다. 예를 들어 마우스 버튼 상에서 움직이고 있는 순간
경고음이 울린다.

Private Sub Command1_MouseMove 12592 As Integer, Shift As Integer,
X As Single, Y As Single)

Beep
End Sub

300


===== PAGE 298 =====
9.5 마우스 이벤트와 키 이벤트

EES

속성 지정

개체                =                 지정
Picture            Autoredraw           True
BackColor            흰색으로 한다.
코드
Dim DrawFlg As Integer                Ae 곡선 그리기
Dim LineFlg As Integer                 '직선/사각/색상 채운 사각형
Dim ColCode As Integer                   '색지정

Dim x1 As Integer, yl As Integer

Private Sub Form_Load()                HAS 초기 설정
MLS ley Se
LineFlg = 1
ColCode = 1

End Sub

Private Sub Form_MouseDown(Button As Integer, Shift As Integer, X As
Single, Y As Single)             i
Forml.Print "F1:4!M F2:A}Zt F3:MAPZ! 0-9a-F:AHA| A”
Forml.Print "click: drag: A} GM YS click:F1-3 펑션키로 그리기
Forml.Print "dblclick: 삭제"
End Sub
Private Sub Form_MouseUp(Button As Integer, Shift As Integer, X As
Single, Y As Single)

Forml.Cls                          ‘& 삭제
Picturel.SetFocus                  '픽처 박스에 포커스 이동
End Sub
Private Sub Picturel_Db1Click()        .
Picturel.Cls                        픽처 박스 삭제
End Sub                                        :
Private Sub Picturel_KeyDown (KeyCode As Integer, Shift As Integer)
If KeyCode = vbKeyF1l Then             WA 키
LineFlg = 1             '직선 크리기 지정
ElseIf KeyCode = vbKeyF2 Then
LineFlg = 2                      사각형 그리기 지성

301


===== PAGE 299 =====
Chapter9 그 외 기본 용법

ElseIf KeyCode = vbKeyF3 Then

LineFlg = 3                    `사각형 내에 색상 그리기 지정
End If
End Sub
Private Sub Picturel_KeyPress(KeyAscii As Integer) ‘! 지정
If &H30 <= KeyAscii And KeyAscii <= &H37 Then     ‘0-9

ColCode = KeyAscii - &H30
ElseIf &H41 <= KeyAscii And KeyAscii <= &H46 Then ㅅㄷ
ColCode = KeyAscii - &H41 + 10                  :
ElseIf &H61 <= KeyAscii And KeyAscii <= &H66 Then a-—f{
ColCode   KeyAscii - &H61 + 10
End If
End Sub
Private Sub Picturel_MouseDown (Button As Integer, Shift As Integer,_
X As Single, Y As Single)
If Button = 1 Then      왼쪽 HY
DrawFlg = 1
Picturel.PSet (X, Y), QBColor(ColCode)
ElseIf Button = 2 Then 오른쪽 버튼 클릭. Fi-F3S 이용한 그림

fim

클릭. 점 그리고 난 후 자유선의 시작점

Tf x1 = -1 Then                  '첫번째 오른쪽 버튼 클릭
1 ~ Se ay                  시작점 저장
Picturel.PSet (X, Y), QBColor(ColCode)      시작점 그리기

Else                           '두 번째 오른쪽 버튼 클릭
If LineFlg = 1 Then              ALA

Picturel.Line (x1, yl)-(X, Y), QBColor(ColCode)
ElseIf LineFlg = 2 Then          `사각
Picturel.Line (x1, 171) -(※, Y), QBColor(ColCode), B
Else                          정사각형
Picturel.Line (xl, 71) -(※, Y), QBColor(ColCode), BF
End If
elo) bey = = 1
End Tt
End If
-End Sub

Private Sub Picturel_MouseMove (Button As Integer, Shift As Integer,_
X As Single, Y As Single)
If DrawFlg Then
Picturel.Line -(X, Y), QBColor(ColCode) 드래그 중 선 그리기
End If
End Sub

Private Sub Picturel_MouseUp(Button As Integer, Shift As Integer, X_
As Single, Y As Single)

302


===== PAGE 300 =====
9.5 마우스 이벤트와 키 이벤트

DrawFlg = 0       MR 그리기 종료
End Sub

동작의 확인
(1 폼에서 마우스 왼쪽 버튼을 누르고 있는 사이에만 도움말이 나타나고 떼면 다시 사라진다.
@ fi, 64, HS 누르면 직선, 사각, 사각 색칠 지정이 된다(그림은 OA 행한다).
(3) OA (인의 7], AIA HS 누르면 QBColor(0)~QBCOLOR(15)2} 색 지정이 된다.
그림 그릴 때는 모두 이 색이 반영된다.
(4) 픽처 박스 내에서 클릭하여 점을 찍는다.
(6) 픽처 박스 내에서 드래그하면 자유선을 그린다.
(6) 오른쪽 버튼을 클릭하여 2점을 연결하는 그림을 그린다.

그럼 9 7

303


===== PAGE 301 =====
‘CHAPTER

개발 툴인 Visual BasicOllA
. 이 장에서는 두 가지 중요한
필요한 지식을 정리하여 소개

MS-DOSet 다른 cere Held
는 그래픽의 처리 SHS Ole

샘플 프로그램을 이용하여 그리
하므로 완벽하게 소화하여보자.


===== PAGE 302 =====
Chapter 10 그래픽의 처리

좌표계와 단위

Visual 28810은 [\)2이라는 SHS 사용한다. Itwipe 1포인트(프린터 폰트의 크기를 나
타내는 단위)의 1/20이고, lem= 567twip, 1인치는 1440[\이다. 이 APE ScaleMode +
성에서 변경할 수 있다. 아직 익숙하지 않으므로 이해하기 쉬운 단위로 변경하는 것이 좋다.

ScaleMode   0- 사용자 정의
1 - twip(C|S&)

2 - Point 0 00000 매매20 twipdll 해당

3 - Pixel 4 £2 2 아아HES 1 dotS} 동일

4 - Character 00900문자 단위 가로 120twip 세로 240twipd| 해당
5 - 1200 00000 아라72포인트, 1440 ㅁ012에 해당

6 - mm

7 = oa

좌표는 그 컨트롤이 배치되어 있는 콘테이너 상의 위치이다. 명령 버튼이 배치되어 있을 때
명령 버튼의 위치는 다음과 같다. 폼의 좌측 우측 Ze (0,0)이 된다.

me

「
l

스케일 체계의 사용자 정의
스케일 체계는 사용자가 정의할 수 있다. 이것을 사용하면 폼의 중
전체를 640×400이나 500×300등이라는 임의의 Dotto} 할 수

앙을 (0,0)으로 하거나

ㅇ
있
XA

a

306



===== PAGE 303 =====
10.2 Screen 개체

이것들의 값을 AMSA ScaleModet 자동으로 0°] 된다.

object .ScaleLeft          좌측 끝의 수평 ABS 설정(표준으로는 0)
object .ScaleTop           위 끝 수평 좌표를 설정(표순으로는 0)
object .ScaleHeight        화면의 수직방면 논리 좌표를 설정
object, ScaleWidth         화면의 수평방면 논리 좌표를 설정

다음 폼화면을 640×400100에 임의로 Ast aS 보자.

Forml.ScaleLeft = 0
Forml.ScaleTop = 0
Forml.ScaleHeight = 400
Forml.ScaleWidth = 640

컨트롤 배치의 토대가 되는 S 자체의 위치는 화면 위의 x, 》값으로 표현된다. 그
린이라는 Eq Screen 개체에서 표현한다. Screen 개체는 표 10-1과 같은 SYS
0)

ActiveControl     액티브한 컨트롤을 바꾼다

ActiveForm       액티브한 SS 바꾼다

FontCount       AS 가능한 폰트의 48 바꾼다

Fonts           지정 인덱스 번호의 폰트명을 바꾼다

Height           화면의 높이를 바꾼다

Mouselcon       ASA 점의의 마우스 아이콘을 정의

MousePointer     특정 위치에서 표현되는 마우스 포인트의 종류를 설정

TwipsPerPixelX  _ 한 픽셀당 ×방향 1/10수를 바꾼다

TwipsPerPixelY 한 픽셀당 방향 twip 수를 바꾼다
Width            화면의 폭을 바꾼다

307


===== PAGE 304 =====
Chapter 10 그래픽의 처리

예를 들면 폼을 네 개로 나눈 화면의 오른쪽 아래 부분에 표시할 때에는 다음처럼 한다.

Private Sub Form_Load()
Forml.Top = Screen.Height / 2
Forml.Left = Screen.Width / 2
End Sub

색의 지정에는 다음 4가지 방법이 있다

Ｌ009형 정수 지정

색의 지정은 1008값으로 한다. 1008형 정수의 색은 적/녹/청을 8칸씩 지정한다. 각색은
OO~ FF 표시한다(주 : 마지막 '@& 은 Long 형이라는 것을 나타내기 위하여 사용하고 있
다. 이것은 일시에 편집기에서 삭제되는 것이다). 다음의 aS 보자.

Forml.Backcolor = &HFF0000    청
&Hbbggrr& | &H0000008 |검정
AAA

&HFF00006 |i} 2}

파랑 녹색 빨강
&HOOFFOO& |=A#
&HOOOOFFE |빨강
&HFFFFFFE |흰색

1

RGB 함수
RGBEE Long 정수 지정의 색상 값을 다른 표현으로 하여 다음처럼 지정한다. 각색
상은 0~255로 지정한다.

RGBired, green, blue)

308


===== PAGE 305 =====
10.3 색의 지정

List1.ForeColor = RGB(0, 0, 0)   ‘aA
List). ForeColor = RGB(255,.0, 0) _ 빨강
List1.ForeColor = RGB(0, 0, 255) _ 파랑
List1.ForeColor = RGB(0, 255, 0) 녹색

1

오기 아자시 이이 이이매            매매
종래의 Quick 88810류의 0~15색상 번호에 의한 색 지정이다(표 10-2).

QBColor (색번호)

Forml .BackColor = QBColor(7)

0          검정             8           회색

1           파랑            9            밝은 청색
2           녹색             10            밝은 녹색
3          청록             11           "밝은 청록
4          빨강             12           밝은 빨강
5           자홍             13            밝은 자흥
6           노랑             14            밝은 노랑
7          백색            15           밝은 흰색

다음은 @800107함수의 기술 예이다.

: 특별한 ae 메해서는 적절한 수   같이. 지정된 컬러 변    수의 정수 가준  준비되어 있으므로 이것
을 사용할 수도 있다(표 10-3). 보통의 AS SHXXXXXXSH 표현되지만, &LH80000002.
로부터의 연결 번호에서 시작하는 특별 컬러 시스템도 준비되어 있다(표 10-4).

309


===== PAGE 306 =====
Chapter 10 그래픽의 처리

# 10=3

vbBlack                     &HOOO0000                    검정

vbRed                         &HOOOOFF                      빨강
vbGreen              &HOOFFOO              2
vbYellow                 &HOOFFFF |!               노랑
vbBlue                       &HFFOOOO __                  파랑
voMagenta                 &HFEFOOFF                  자홍
vbCyan                &HFFFFOO               a=
vboWhite                 사변              흰색

정수                      a                       내용

vbScrollBars         &H80000000        스크롤 바의 색상
vbDesktop          &H80000001        데스크 탑의 색상
vbActiveTitleBar     &H80000002       활성 타이틀 바의 색상
vbInactiveTitleBar

&H80000003 |

비 활성 타이틀 바의 색상

Visual 828810에서는 폼 위에 도형을 그리기 위해 다음 3개의 컨트롤을 준비하고 있다. 이
것을 사용하면 기술할 필요 없이 마우스로 기본적인 도형을 작성해서 배치할 수 있다. 이것들
에 대한 상세한 설명에 대해서는 8장 컨트롤을 보도록 하자(195페이지).

이미지 컨트롤         12(9.omp, .ico, wmf 등)을 표시한다
라인 컨트롤          폼 내에 직선(수평, 직선, 칠)을 그린다
az          XR

셰이프

310


===== PAGE 307 =====
106 컨트롤의 이동

Visual Basic] 그래픽을 처리할 때에는 속성/메서드가 유용하다. 사용하는 컨트롤에서
다음의 속성/메서드가 준비되어 있다면 그래픽 처리를 할 수 있다.

표 0-5 ii    용

이름          설명

AutoSize      픽처 박스의 AutoSizeS True® 하면 픽처 박스의 크기는 그림
의 크기에 맞게 자동으로 StH ect

Stretch        이미지 HESS 선택 AAT 로드하는 그림의 크기가 다른 경우
의 AAS 결정한다
Stretch=True      그림을 컨트롤 크기에 맞춘다
Stretch=False      HES 크기를 1219] 크기에 및춘다

[66106     폼의 왼쪽 위 끝(0.0) 지점부터의 거리를 결정하고 컨트롤의 폼

위에서의 배치를 설정한다.

Height/ Width 컨트롤과 폼의 높이와 폭을 결정한다

Move        AEST 품의 위치를 이동한다. Leta Tops 개별로 기정하여
장소로 이동하는 대신에 사용할 수 있다.

Align         픽처 박스 또는 데이터 HESS = 상하 ASD 어느 WOE
에 맞춘다

AutoRedraw Sit 픽처 박스에 준비되어 있다. AutoRedrawS 참으로 해
2 AS22 다시 그림을  그린다. 예를 들면 윈도우 위에 다른

를 겹쳐서 또 볼 수 있도록 할 때 AutoRedraw7} 참인

우는 '그림이 재현된다

때

ow re 4n

AES Left/Top 속성 값을 코드 중에서 짧은 시간
용하면 이동시킬 수 있다. 이미지 컨트롤과 픽처 박스 컨트롤을 실행시켜 표시된 그림을 이동

하여 보인다.

변경하지만 혹은 Move 메서드를 A}

311


===== PAGE 308 =====
312

Chapter 10 그래픽의 처리

Left/Top 속성의 사용

다음과 같이 명령 HES 클릭할 패마다 픽처 박스 그림이 우측 아래로(우측
100twip#)) 이동한다.

아래로

Private Sub Command1_Click()
Picturel.Left = Picturel.Left + 100
Picturel.Top = Picturel.Top + 100

End Sub

Move 메서드
Left/Top S42
AES 사용하여 잔

i

사용하면 이동에 대한 잔상이

Yo] 단계적으로 보이게 된다. 이것
AS 없애고 이동을 할 수 있다. 다음처럼 하면 명령

Private Sub Command2_Click()
Picturel.Move Picturel.Left + 100, Picturel.Top + 100

End Sub

절대 이동

Move 메서드의 예는

예1 :   Picturel.Left = 1000
Picturel.Top = 1500

2:  Picturel.Move 1000,1500

현재 위치보다 100twip# 오른쪽
다음처럼 하면 어떤 특정 장소로 이동을 한다. 이것

= (1000,1500)9] 위치로 이동하고

아래로 상대적으로 이동하고 있으
있다.

나

픽처 박스에 표시되어 있

마다 새로운 그림을 읽고 표시히

AN
a
요
0
ful
ra


===== PAGE 309 =====
10.7 픽처 바꾸기

Picturel.Picture = LoadPicture( 파일명")
Imagel.Picture = LoadPicture ( 파일명" )

로 한다. 그러나 이 방법은 읽는데 시간이 많이 필요로 하므로 그림을 빠르게 바꾸고자 할 때
에는 적절하지 않다. 예를 들면 날개를 펼친 나비의 그림과 날개를 접은 나비의 그림을 빨리
바꾼다면 날고 있는 듯이 보이게 된다. 이와 같은 경우에는 미리 모든 그림을 읽고 실행시에
바꿔 표시하는 방법을 사용한다. 보통 나중에 표시할 그림은 이미지 컨트롤에 읽어 두고 픽처
박스에 전송한다. 예를 들면 두 개의 이미지 박스에 미리 그림을 읽어 두면(디자인 시에 가능)
다음의 코드에서 그림을 바꾸어 준다.

If 조건 Then
Picturel.Picture = Imagel.Picture
Else
Picturel.Picture
End If

띠플터로틴램

폼에서 싱글싱글 웃는 그림이 이동하고 가장자리에 위치하면 방향 전환
Qld 모습과 생글생글 웃는 얼굴로 변경된다. 이동의 타이밍은 타이머 컨

Image2 .Picture

속성 설정

개체             속성                      설정

Command       Caption                   “Alay

Timer1           Interval                   1

Imagel           Picture                    130602.160설정한다.
Visible                    False

Image2          Picture                    130601.100을 설정한다.
Visible                    False

Picture1          BorderStyle                90 ~ 없음
Picture                    없음 (주)

주) Picturel.Picture 는 “(없음 ) 이지만 디자인할 때에는 [140601.100를 일단 잃고 사이즈를 빠듯하게 조정
해 둔다. 그 SCY OR 되돌아간다.

코드

Private Houkou As Integer
Private Const LftUp = 1
Private Const RgtUp = 2
Private Const RgtDn = 3

313


===== PAGE 310 =====
Chapter 10 그래픽의 처리

Private Const LftDn = 4

Private Sub Command1_Click()
If Command1.Caption = "시작" Then

Command1.Caption = "정지"
Timerl.Enabled = True       '타이머 유효(이동 시작)
Houkou = Int(4 * Rnd + 1)    '최초의 이동 방향
Else
Command1.Caption = "시작"
Timerl.Enabled = False       타이머 무효
End If
End Sub

Private Sub Form_Load()
Picturel.Picture = Imagel.Picture 최초의 웃는 마크를 설정
Timerl.Enabled = False
End Sub
Private Sub Timerl1_Timer ()
Dim OldHoukou
Static ImgFlg
OldHoukou = Houkou
Select Case Houkou
Case LftUp                    '왼쪽 ACOs 이동
Picturel.Move Picturel.Left - 20, Picturel.Top - 20
If Picturel.Left <= 0 Then

Houkou = RgtUp           좌측 끝이면 우측 상단으로 방향 전환
ElseIf Picturel.Top <= 0 Then
Houkou = LftDn          상단 끝이면 좌측 하단으로 방향 전환
End 10
Case RgtUp                    Ss 상단으로 이동

Picturel.Move Picturel.Left + 20, Picturel.Top = 20
If Picturel.Left >= (Forml.Width - Picturel.Width - 100) Then

Houkou = LftUp          우측 끝이면 좌측 하단으로 방향 전환
ElseIf Picturel.Top <= 0 Then
Houkou = RgtDn          하단 끝이면 우측 상단으로 방향 전환
End if
Case RgtDn                  ‘Se 하단으로 이동

Picturel.Move Picturel.Left + 20, Picturel.Top + 20
If Picturel.Left >= (Forml.Width - Picturel.Width - 100) Then

Houkou = LftDn          우측 끝이면 좌측 하단으로 방향 전환
ElseIf Picturel.Top >= (Forml.Height - Picturel.Height - 400) Then
Houkou = RgtUp          하단 끝이면 우측 상단으로 방향 전환
End If
Case LftDn                    f= 하단으로 이동

죄
Picturel.Move Picturel.Left - 20,
If Picturel.Left <= 0 Then   Bia

Picturel.Top + 20

끝이면 우측 하단으로 방향 전환

=


===== PAGE 311 =====
10.7) 픽처 바꾸기

ElseIf Picturel.Top >= (Forml.Height - Picturel.Height - 400) Then
Houkou = LétUp . '한단:끝이면 좌측 상단으로 방향 전환

- 200 861606                      =
_ If OldHoukou <> Houkou Then      `방향 전환이면 변경한다.

IngFlg = Not IngFlg
If ImgFlg Then
Picturel. Picture = Image2.Picture

_ SoS 얼굴
Else      인
ㆍ Picture
End If
End Sub

sture  = Imagel.Picture

동작의 확인
© 실행해서 시작 버튼을 클릭하면 스마일 마크가 이동한다.
(9) 시작 HES 정지 버튼으로 이름이 변한다.

화면1 디자인 화면

여기에 픽처 박스가 있다. 경계를        이것을 클릭하면 마크가
없음 으로 해 두므로 잘 모른다                    움직이기 시작한다

실행시에 타이머와 이미지
HESS 보이지 않게 된다

315


===== PAGE 312 =====
316

아18016『10 그래픽의 처리

품과 픽처 박스는

i eas ee

Cis

메서드           :

PSet

ge:     린트에 의한 출력을 제거한다
지정 위치에 점을 찍

그 내부에 간단한 그래픽을 그릴 수 있으며 메서느는 표 10-6과 같다.

는다            !

Point            지정된 점에 대한 RGBS 반환 .
Line             선, 사각형을 그린다          |
Circle             원 ,타원, 원호를 그린다

PaintPicture_

임의의 위치에 그래:

z| 파일의 그림을 그린다

Print

문자열을 출력한다

다음에 나타낸 그래픽 메서드의 기술

주) Step 2 상대 지정할 때에 사용한다

형식의 예를 보자.

이 메서드들을 사용할 때에는 다음의 속성이 유용하다.

object .DrawWidth

[= size]

그리는 선의 크기를 설정(|-32767) 지정 값은 1

Object .DrawStyle [= number]


===== PAGE 313 =====
- 이점 쇄선(대시-점-점)
5- AMES)

6- 내부 단색

10.8 그래픽 메서드

Object .DrawMode [= number]
그래픽의 외관을 AA
| _

흐

=

2 - 쉬이 Marge Pen ows15번의 반전색
3 - 1489 시이 1760 2펜의 반전색과 배경색에 공통색으로 출력
4—-—Not Copy 060 0000 에19번의 반전색
5-Mask PenNot 2펜과 표시색의 반전색에 공통색으로 출력
6 - 10060 ts표시색을 반전시켜 출력
00펜과 표시색의 어느쪽인가에 포함되어 있는 색을 조합하여 출력
8-Not Mask Pens9번의 반전색
Q9-Mask Pen 으아펜과 표시색에 공통색 출력
10 - 비이 Xor Pen7번의 반전색
0 _표시색과 펜의 반전색을 조합하여 출력
12-Marge NotPen 2화면에 그려지지 않는다
18 - 0007 1060 싸여(계정값 『01600!아로 지정한 색으로 출력
14 - 48096 Pen Not 2펜의 색과 표시색의 반전색을 조합하여 출력
15 - Marge Pen펜의 색과 표시색을 조합하여 출력
16 - 백
Object .FillColor [= number]
색칠에 사용하는 색을 설정.  a   값은 0(흑).색은 RGB 함수와 QBColor 함수로 AZ, FillStyle0| 기
본 값인 1(투명)에 설정되어 있는 경우에는 110010/의 설정은 무효
Object .Fillstyle [= number]
원과 사각을 색칠할 때의 패턴을 설정
0- 색칠
+ 투명
2- 가로선
3- 세로선
파선(좌측 위-우측 아래)
5- 파선(좌측 아래-우측 위)
6- 대각선
~ 그물

317


===== PAGE 314 =====
Chapter 10 그래픽의 처리

띠풀터로트램

Cls, PSet, Line, Circle, Print2] 사용 예를 나타낸다. 폼을 클릭하면 그릴 수 있다.

JP

3a

없

정

Do

코드

Private Sub Form_Click()
Dim I As Integer, col As Integer

Cls
ScaleMode = 3                       '단위를 픽셀로 한다.
DrawWidth = 1                      선의 #7|8 1로 한다
For I = 5 To 50 Step 3
col = (col + 1) Mod 15
Circle (50, 50), I, QBColor(col)    ‘AS 그린다.
Next
For I = 0 To 50 Step 3               사각형을 16색으로 그린다.

col = (col + 1) Mod 15        |
Line (200 - I, 50 - I)-(200 + I, 50 + TI), QBColor(col), B

Next 1
ForeColor = QBColor (4)               사각형을 16색으로 그린다.
FontSize = 24                       폰트 사이즈
FontItalic = True                   이탤릭체로 한다.
CurrentX = 0
Currenty = 120
Print "그래픽 Demo"            |
DrawWidth = 3                       선의 H7/S 3으로 한다.
For X = 10 To 240 Step 10
PSet (X, 160), QBColor (4)         ANOS 그린다
Next
Exit Sub
End Sub

주) 이 프로그램에서는 개체 명이 생략되어 있다. OWE 들면 FontSizet “Forml.FontSize = 24"로 된다,
개체를 생략하면 현재 액티브로 되어 있는 것이 지정된다. 이 LBA Form Clickol 유료하게 될 때어는
확실히 Form 1이 액티브되므로 이것으로 괜찮다(『01171.“을 넣어도 졸다).


===== PAGE 315 =====
10.8 그래픽 메서드

동작의 확인
@ 실행하면 아무것도 없는 폼이다.
© 폼을 클릭하면 그림이 나타난다.

319


===== PAGE 316 =====
CHAPTER

Ee
—
$2
rr
ic
al!
|
1늬

그래픽 기능을 사용하여 재미있는 화면 표시를 해 보ㅅ
으로 기본적인 AAS 하고 그것을 프로그래밍으로
릴 수 있다. 만약 손으로 그린다면 대단한 끝기2
에서는 짧은 순간에 할 수 VC, ZEISS Ac

게 가능한지 생각

Lo ean |

Ol!
ra
oa
me
S
HI
=
Hu
Olt
a



===== PAGE 317 =====
322

Chapter 11

재미있는 프로그램

몇 개의 원을 조금
않도록 그림자 처리를 뻐
우선 가상의 가장 큰 원을 한 개 그리고 원 주위에

씩 단위를 달리하며 그리고 원이 겹쳐진

부분이 보의지

중심을 둔 작은 원을 차례로 그리면 다

음과 같다.
이 그림을 응용하면 가상의 큰 원을 우측으로 작은 원이 $9] 그러가면서 큰 원의 반경을
작게 한다. 이렇게 하면 입체감을 갖는 Melo} 같은 그림을 그릴 수 있다.
Picture. FillStyle=0              ‘ANAL 지정
Picture.FillColor=(255,255,255) 흰색 지정

0_
을 설정한다.

Magzbla

재미있는 그림의 프로그램을 다음에 제시한다.

속성 설정

개체                   속성                     설정
Command}           Caption                재미있는 그림
Picture           BackColor         흰색



===== PAGE 318 =====
fu
In

Private Sub Command1_Click()

Const x0 = 1500, yO = 2000
Const RAD = 3.14159 / 180

Dim x As Integer, y As Integer
Dim deg As Single

Dim r_dai

Dim r_syo

Dim sft As Integer

Picturel.Cls
sit = 0: y = 1000
© dai > 1000: vr syo = 600
Picturel.FillStyle = 0
Picturel .FillColor = RGB(255, 255, 255)
For deg = 0 To 360 * 3 Step 3

x = © dai * Cos(deg * RAD)

ll

VY = >, 991 ^ Sin(deg * RAD)
x = x + x0 + SEL: SEL = sft + 10
y-yt yO

Picturel.Circle (x, y), r_syo, RGB(0, 0, 0)
If deg > 360 * 2 Then r_syo = r_syo * 0.98

Next

End Sub

크림 11-1

>

(Crm,
S  (AB

구불구불
최초의 큰원 중심
작은 원 중심
각도

큰 원의 반경
작은 원의 반경
오른쪽으로 회전
'색칠하기

(호 AH

ae

'작은 원 중심 결정

323


===== PAGE 319 =====
324

Chapter 11

재미있는 프로그램

재귀(086) 프로그램의 샘플로서 유명한 힐베르트 곡선은 다음과 같은 방법으로 그림을 그
린다. 우선 다음의 힐베르트 곡선을 보자.

나         ㄴ  -90}
H1                                     H2

Ae] 그림 중에서 왼쪽의 그림 HLS 힐베르트 Fao] 기본 247 Sie 것으로 이것을 위
(HHO 9] 힐베르트 곡선이라고 한다. 오른쪽의 82는 더 복잡한 것으로 이것을 위수:
#029] 힐베르트 곡선이라고 한다.

1이 힐베르트 곡선의 기본 요소이다. So] H29] 도형을 보면 이 그림이 파선 부분만
을 생각하면 HLT} 같은 구성이 되어 있다. 그 HLS 그리는 도중에 작은 4 개의 H1S 적당히
회전시커서 그림 그린다. 여기에서 22를 보면 기본 요소 HIE 좌측 회전의 ㅅ패턴과 우측
회전의 BAH] 있다. 이것들의 그림 그리기 SAE 다음과 같다.

ATH 그리기 순서

-90도 회전해서 길이 LS] 직선을 표시
+90도 회전해서 길이 Ｌ의 직선을 표시
+90도 회전해서 길이 Lo] 직선을 표시

-90도 회전한다


===== PAGE 320 =====
—_
~
nD
nt
=
i
JH
Ps

BoyH 그리기 순서

+90도 회전해서 길이 Ｌ의 직선을 표시
-90도 회전해서 길이 Ｌ의 직선을 표시
-90도 회전해서 길이 Ｌ의 직선을 표시
+90 & 회전한다

지금 이것들의 동작을 A, 8, 90, -90, 1이라는 번호로 표현하고 ㅁ2(전체로부터 본 ㅅ패턴)

oS

의 그리기 순서는 다음과 같다. 12 "길이1의 AMS 표시"라는 동작을 나타낸다.

A: -90, A, 1

+90, A, 1
A, +90, 1
B, -90

샘덕피커 1
이 원리로 작성한 위수(00806의 힐베르트 BAS 다음에 제시한다. 이 수를 크게 하면 보
다 자세히 그림을 그릴 수 있다.

|

A
속성 설정

개체             숙적               설정

Commandt        Caption            "힐베르트 곡선"

Picture          BackColor         흰색

코드

Private Sub Command1_Click()                   `힐베르트
Const size = 4096                       ‘12! 전체 크기
Dim ct As Integer, lenn As Integer
Dim x As Integer, y As Integer
Dim d As Integer                          진행 방항

Picturel.Cls
(ol wala 0)

325


===== PAGE 321 =====
326

Chapter 11 재미있는 프로그램

lenn = size / (2 ^ ct)                  선의 길이
x = size - size / (2 ^ (ct +1))) 직선 크림 자리 값을 다음 다음으로 지정

Vas 9326 / (2 ^ 066 + 101

a= 270

drawA ct - 1, x, y, d, lenn            '교릴 시직
End Sub

Private Sub drawA(ct As Integer, x As Integer, y As Integer, ByVal d_
As Integer, lenn As Integer)

If ct < 0 Then Exit Sub
d=d- 90: drawB ct - 1, x, y, da, lenn: drawhine x, y, d, lenn
요 = 0 + 90: drawA ct - 1, x, y, d, lenn: drawLine x, y, d, lenn
drawA ct - 1, x, y, d, lenn: d = d + 90: drawLine x, y,; d, lenn
GrawB ct + 1,..x;-yv, 이, 20001; 이 = 4d - 90

End Sub

Private Sub drawB(ct As Integer, x As Integer, y As Integer, ByVal d_
As Integer, lenn As Integer)

If ct < 0 Then Exit Sub
d= d+ 90: drawA ct - 1, x,y, 6, lenn: drawline x, y,.d, lenn
a= d ~ 90: drawB ct — 1,2, y, d, lenn: drawline x; y) da, Jenn
drawB ct - 1, x, y, 0, lenn: d = 4 - 90: drawhine x, y, dg, lenn
GrawA ct - 1, x, y, dad, lenn: d =d + 90

End Sub

Private Sub drawLine(x As Integer, y As Integer, d As Integer, lenn_
As Integer)

Dim oldx As Integer, oldy As Integer

If d < 0 Then d = d + 360
If d >= 360 Then d = d - 360
oldx = "x: oldy = y

Select Case d
Case 0: x = x + lemn
Case 90: y = y - lenn
Case 180: x = x - lenn
Case 270: y = y + lenn
End Select

Picturel.Line (oldx, oldy)-(x, y), RGB(0O, 0, 0)
End Sub


===== PAGE 322 =====
11.3 트리

그림 11 3

힐베르트 곡선과 마찬가지로 리턴 콜을 사용한 동일 패턴 반복 그림 화면이다. 다음의 그림
을 보자.

우선 나무 가지인 aS 그린 다음에 가지 8 로부터 분리된 가지를 그린다. 다음에 가지 cS
"새로운 가지 @"라 생각하고 거기서부터 분리된 가지 0와 가지 6로 그 위에 가지 £2} 가지 g
를 그린다. 이 같은 가지 분리 그림을 모든 '가지' 에 대하여 한다. 그러면 울창하고 번성한 독
특한 나무가 프로그램 내에 그려진다.

327



===== PAGE 323 =====
Chapter 11 재미있는 프로그램

Agha

다음에 프로그램을 제시한다.

속성 설정
개체                   속성                     설정
Command           Caption                 “Tree”
Picture          BackColor         흰색

Const XSIZE = 5000, YSIZE = 4000, LENGTH = 1000
Const RAD = 3.14159 / 180

Private Sub Command1_Click()                ' TREE
Dim n As Integer, m As Integer
Dim i As Integer, j As Integer
Dim lenn As Single
Dim th As Single, thl As Single, th2 As Single
Dim kaido As Single                  '가지의 시작을 결정한다.
Dim x As Single, y As Single
Picturel.Cls
rege               가지 AB 각도를 180/4=45도로 한다.
kaido = 180 /n

= 91028 / 2eiy = 16028 / 3          '최초의 가지 분기점의 위치
lenn = LENGTH                        '가지의 길이

th = 180 / 2         JERIQ] HOLI7E 방향을 결정한다:
Picturel.Line (x, YSIZE)-(x, YSIZE - y) 최초의 줄기 표시

tree x, y, lenn, th, kaido
End Sub

Private Sub tree(x As Single, y As Single, ByVal lenn As Single, th_
As Single, kaido As Single)

Dim x1 As Single, x2 As Single

Dim yl As Single, y2 As Single

Dim thl As Single, th2 As Single

If lenn <= LENGTH / 15 Then Exit Sub

lenn = lenn * 0.75                   다음의 가지가 짧게 된다:
thl = th - kaido                    OSs 가지의 각도

th2 = th + kaido                    '윈쪽 가지의 각도

xl = x + 1600 * Cos(thl * RAD)         가지 선의 위치

yl = y + 1600 * Sin(thl * RAD)

328


===== PAGE 324 =====
11.4 평행선의 회전

x2 = x + lenn * Cos(th2 * RAD)
y2 = y + lenn * Sin(th2 * RAD)

Picturel.Line (x, YSIZE - y)-(xl, YSIZE - yl)       "오른쪽 가지

tree x1, yl, lenn, th1, kaido         오른쪽 가지 NS 그린다.

Picturel.Line (x, YSIZE - y)-(x2, YSIZE - 22) -      "왼쪽 가지

tree x2, y2, lenn, th2, 12100         ‘QI 가지 MS 그린다.
End Sub

평행선을 희전시키면서 반복한 그림으로 복잡한 모양의 원을 그릴 수 있다. 이 원은 두 개의
수값ㅁ과 ms 지정하는 것으로 그 모양이 변한다. 그림 11-6에 그림 그리기 원리를 나타낸다.

A 그림은 기본형이다. 원 주위에 시작점과 종점을 갖는 평행선을 (2-1)번 Mey, 이 파선의
Ue 실제로는 표시하지 않는다. BAGS 90도 각도를 붙여서 일조의 평행선을 Mey, 결국
(0-]1)번의 평행선이 mES 끌어 당겨서 빠지는 것이다. 그림 Cems 4 로 한 것이다. 회전
각도는 180/피도로 된다. DIGS mS 10으로 한 것이다. ㅁ을 크게 하면 동심원이 증가하
고, m& 크게 하면 원이 명료하게 되는 경향이 있지만, 그 모양 패턴이 재미있는 변화를 한다.

329


===== PAGE 325 =====
Chapter 11 재미있는 프로그램

1 noe een See oe el eo

NC
기

AY
= Os:

A (n=5)              6 (n=5, m=2)            C (n=5, m=4)           D (n=5, m=10)

띠플터로트램

다음에 프로그램을 제시한다. nt mo] 값은 텍스트 박스로부터 입력할 수 있도

4

Ol
EJ
32,
된

속성 설정

개체             속성              설정
Command       Caption           평행선 회전'
Picture          BackColor BA
Text1            Text              -
Text2            Text              eZ

=
Private Sub Commandl_Click() 평행선 회전

Dim n As Integer, m As Integer

Dim i As Integer, j As Integer

Const lenn = 1500, PAI = 3.14159

Dim th As Single, thl As Single, th2 As Single
Dim x1 As Integer, x2 As Integer

Dim yl As Integer, y2 As Integer

Picturel.Cls

n = Val (Text1.Text)

m = Val (Text2.Text)

11 ㅁ0 = 2106 m < 2 Then Beit Sub)

For i = 0 fo m — 1       각도 회전을 msl 한다.

80 3 = 1 20 ㅁ- 1 ‘n-1 평행직선을 끌어당긴다.

th = 3 < (PAT / ㅁ)
thi  4 * (PAL / m) = th
th2   a (PAL / 0) th

1

330



===== PAGE 326 =====
11.5 구의 표시

xl = 068(다1) * 1609 + 2000
yi = Sin(thl) * denn + 2000
x2 = Cos({th2) * lenn + 2000
y2 = Sin(th2) * lenn + 2000
Picturel.Line (xl, yl)-(x2, y2)
Next
Next

End Sub
주) “the~"9] 식은 본래는 “thsj * (PTI/180) * (180/n/' AES 갖고 있다.

|

|

원을 입체적으로 표시하면 구가 된다 .원은 ※성분과 》성분만을 표시한 것이지만 구의 경우는 2

분을 생각해야 한다. 즉 3차원의 TAS 취급하는 것이다. 이 경우 원래의 물체는 3차원이지만

| 상태의 화면은 2차원이므로 2 성분을 성분과 성분으로 반영시켜서 무리하게 2차원으로 투
시킬 필요가 있다. 그 방법으로서 이론적으로는 주측 투영, —   투영, 투시 도법 등이 있다.

여기에서는 구라는 특수한 그림 즉, 어느 방법으로 보아도          구인 그림이므로 그밖의 프

로그램으로 간단한 방법으로 그려 보자, 지구를 Telepanel  00   pas 간단하다. 우선 그

림 11-8 을 살펴보자.

성
HA
3

331


===== PAGE 327 =====
Chapter 11 재미있는 프로그램

그림 11-8
|            Yea
Xa
09          |
A               B              Cc

쇼그림처럼 XY 평면 위에 가상의 반원을 생각하고 그 원주 상에 A pl, p2,...p99 자리를
잡는다. 이것은 지구의 위도에 해당한다. 여기에서 축을 중심으로 일 회 회전하고 그것을 정
가로로부터 보면 그림 8가 된다. 더구나 그림 Bol 대해서 축을 앞쪽으로 30도 넘어뜨리
면, 그림 (처럼 된다

이 그림에 경도를 나타내는 세로 선을 넣으면 구의 그림이 된다.

이 그림은 음영 처리를 하고 있지 않은 지구 모양 같은 그림이다. 본래 북극이 보이고 있고
남극은 숨겨 있는 그림틀이지만 보이도록 하면 역으로도 볼 수 있다.
속성 설정

개체                속성                  설정

22 <
Command       Caption         ae
Picture          BackColor      | 흰색
코드
Const HANKEI = 2000                         원의 반경
Const XBASE = 2200, YBASE = 2200             '원의 중심
Const RAD = 3.14159 / 180
Private Sub Command1_Click()       |            ‘St
Dim x As Double, y As Double, z As Double
Dim x2 As Double, y2 As Double
Dim degZ As Double                       2지원(×-\면) 회선 각도
Dim degY As Double                      ‘BAIA (x-z HH) 회전 각도

332


===== PAGE 328 =====
11.5 구의 표시

Picture1.Cls
:가로선
For 0692 = -90 To 90 Step 10             “위도
x = HANKEI * Cos(degZ * RAD)
y = HANKEI ^ Sin(degZ ^ RAD)
For degY = 0 To 360
x2 =x ^ Cos (degy %, RAD)
Z =x * Sin(deqy * RAD)
V2 =¥ < Cos (30 ^ 529) + 2 ^ Cos (60) * RAD)
Picturel.PSet (XBASE + x2, YBASE + y2) 위도 표시
Next
Next

0"

10도씩으로

[이
프

‘AEA
For degY = 0 To 180 Step 10              ‘AGS 10도씩으로
For degZ = -90 To 270
x = HANKEI * Cos(degZ * RAD)
y = HANKEI * Sin(degZ * RAD)
“2 = x * Cos(degy * RAD)
z = x * Sin(degY * RAD)           축의 회전이 0일때
72 = y " 008(30." RAD) + 81?0086(60 ^ RAD)
Picturel.PSet (XBASE + x2, YBASE + 72) 경도 표시
Next
Next
End Sub

|
ro
a

주) ×와/는 XY BRIS 위치. ×2 는 \/축 회전을 반영시킨 것.2는 yee 성분, VE VSS 앞으로 30도 돌린
Wo 바영시키 거
스크 ㄴㅇ Ls A

그럼 11-9

333



===== PAGE 329 =====
334

Chapter 11

재미있는 프로그램

같은 그림을 음영 처리한 것이다. 음영 처리에는 MAX - MIN'YI 내부를 백색으로 칠하

기 등의 간단한 방법이 있지만 표시되는 그림에 의해 방법도 달라진다. 일반적으로      그림이 위

에서부터 아래로 왼쪽에서부터 오른쪽으로 진행하는 경우의 음영 처리는 간단하다. 이 지구

의 HALE Pset 42157} 되돌려지므로 단순한 음영 처리 방법은 어렵고   어떻게 해서라도

그림 순서를 분석하고 그것에 대한 대응 방법을 얻을 순 없다. 여기에서는 다음처럼 처리한다.
횡선(위도) 그림

SAA, BS 동시에 찍도록 프로그램을 고친다. 우선
그릴다(기존의 DHS 지운다) 그 후 두 캐의 점 ㅅ

A, 8ㅁ사이에 백색으로 선을
BS 검은색으로 찍는다.

종선(경도) 그림

'그린다/그리지 BEC Ate 플래그를 준비한다. 찍을 만한 점이 외주 상에 온다면
거기서부터 뒤쪽으로 회전하여가는 타이밍으로 “그린다/그리지 Beco] 플래그를
반전시킨다. 다시 외주상에 온다면 거기서부터 표면으로 나오는 타이밍으로 “그린다
/그리지 BEC S| 플래그를 반전시킨다. 점(×%,)가 「 외주상에 있을까 어떨까는 "
+ = 으로 판정할 수 Uc 은 HS 반경).

실제 프로그램으로 콘트롤의 배치는 동일하므로 코드만을 나타낸다.

코드
Const HANKEI = 2000#                     '원의 반경
Const XBASE = 2200, YBASE = 2200           “Aol BA
Const RAD = 3.14159 / 180
Const R2 = 2000# * 1999                 '반경*반경보다 조금 작은 것
Private Sub Command1_Click()               ‘SH 처리의 >

Dim x As Double, y As Double, z As Double
Dim x2 As Double, y2 As Double

Dim 0692 As Double                     '2차원(×-\면) 회전 각도
Dim degY As Double                      3 차원(×%-2면) 회전 각도
Dim draw As Integer, insideFlg As Integer

Picturel.Cls

'횡선

For 0692 = 90 To -90 Step -10          WES 10도씩으로 한다

= HANKEI * 0068 (0692 * RAD)
y = HANKEI * Sin(degZ * RAD)
For degY = -90 To 90 Step 0.5       주) 참조
x2 = x * Cos(degY * RAD)
2 =x * Sin(degyY ^ RAD)


===== PAGE 330 =====
11.5 구의 표시

y2 = y * Cos(30) * RAD) + z ^ Cos(60 * RAD)
If degZ >= -50 Then
Picturel.Line (XBASE - x2, y2 + YBASE)-(XBASE + x2,

y2 + YBASE), QBColor (15)        `흰색으로 제거
End If
Picturel.PSet (XBASE + x2, YBASE + y2)      위도 표시
Picturel.PSet (XBASE - x2, YBASE + y2)      ‘OG 표시
Next
Next
ae ot
For degY = 0 To 180 Step 10            '경도를 10도씩으로 한다
draw = True: insideFlg = True
For degZ = -90 To 270 Step 0.5      주 참조

x = HANKEI * 068 (0692 * RAD)
y = HANKEI ^ Sin(degZ * RAD)
x2 = «-* Cos (degy ^ RAD)
Z = x *-Sin(degy * RAD)
y2 = y ^ Cos(30 ^ RAD) + 2 * Cos(60 * RAD)
Tf (x27 x2 4 ye * y2) >= R2 Then
If insideFlg = True Then draw = Not draw
insideFlg = False
Else
insideFlg = True
End If
If draw = True Or insideFlg = False Then
Picturel.PSet (x2 + XBASE, y2 + YBASE) A&HA|
End If
Next
Next
End Sub

주) AHS. 확실히 SFI] 위해 “For degY=-90 To 90"이 아니라, “For degY= -90 To 90 Step 0.5"으
로 하고 있다.

그림 11-10



===== PAGE 331 =====
336

Chapter 11 재미있는 프로그램

입제 문자 표시

입체 문자 폰트를 ARSE 것은 아니고 임의의 문자열을 프로그램 처리하는 것으로 입체
문자로 표시한다. 입체 BALE 보통 좌측 위쪽부터 빛이 비추고 있다고 가정하고 처리한다. 이

을 하기 위해서는 문자 자체의 좌측 위쪽에 흰색 표시 부분을 문자 자체의 우측 하단부에 검
색으로 표시하면 좋다. 다음의 프로그램을 보짜.

텍스트 박스에 입력한 문자를 픽쳐 박스에 표시하.
자 부분을 그리고 난 후 마지막에 문자 부분을 쓴다.

CurrentY = 문자 위치를 결정한다.

것
정

밝은 부분을 그린다

Picturel.CurrentX = x - 20 : Picturel.CurrentY = y - 20

그림자 #28 그린다

Picturel Currentx = x + 20 ; Picturel Currenty — y + 20

문자를 그린다

Picturel.CurrentX = x :Picturel.CurrentY = y

…플 ooh

입체 문자 표시 프로그램을 보자.

속성 설정
Commandt       Caption          |  "입체문자)
76×11             Text                S
Picture                             표준대로



===== PAGE 332 =====
11.6

입체 문자 표시

코드
Private Sub Command1_Click()
Dim x As Integer, y As Integer 프시위치
x = 200: 꼬 - 200
Picturel.Cls
Picturel.Font.Name = "굴림체"
Picturel.Font.Size = 72
Picturel.CurrentX = x - 20: Picturel.CurrentY = y - 20
Picturel.ForeColor = QBColor (15)      ‘Bre 흰색
Picturel.Print Text1.Text
Picturel.CurrentX = x + 20: Picturel.CurrentY = y + 20
Picturel.ForeColor = QBColor(0)       as 그림자
Picturel.Print Text1.Text
Picturel.CurrentX = x: Picturel.CurrentY = y
Picturel.ForeColor = QBColor (12)      ‘AAW 문자
Picturel.Print Text1.Text

End Sub

337


===== PAGE 333 =====
a fal

CHAPTER

파일 처리 함수

Visual Basic2| 파일 처리에는 순차, 랜덤, 바이너리의 세 가지 Bt
법이 있다. 바이너리 처리는 한 문자 단위로 하는 것으로 바이너리 단위
의 입출력 명령문도 준비되어 있다. 보통은 순차 파일들을 사용하면 종
래의 지식으로 간단하게 WS 처리할 수 있다. 또 Visual 88910에서

는 컨트롤 자체가 파일 입출력 기능을 갖고 있는 것도 있다.


===== PAGE 334 =====
Chapter 12 파일 처리 함수

파일 액세스에 다

여기에서는 Visual 88810의 파일 처리 방법에 대해서 살펴보자. 보통 프로그래밍 언어에
A) 파일을 처리하기 위해서는 파일 처리 함수를 사용해야 한다는 점이 Visual 나 조금

차이가 있다. Visual 88810에는 기능이 충실한 컨트롤이 있으며 속에는 파일 입출

가진 컨트롤까지 있다. 구체적으로는 데이터 컨트롤을 의미한다. 이 컨트롤과 연결 ae
롤을 병용하면 PES 한 SE 표시하지 않아도 데이터베이스 파일의 읽기와 쓰기가 가능하
다. 또 리치 텍스트 컨트롤에서는

RichTextBoxl.LoadFile “U}2!/H" ,rtfRTF           이지
RichTextBoxl.SaveFile 파일명" ,ㅠㄴㄷ[ㅁ8           쓰기

에서 한번에 1080와 SaveS 해 준다. 이처럼 컨트롤이 가진 파일 읽기 기능을 사용한 방법도
지만 데이터를 한 행씩 읽을지 어떤 위치에 어떤 데이터만을 읽는 치리를 하기 위해서는 보

있
S 파일 처리 함수를 사용한다.

340


===== PAGE 335 =====
12.3 파일 처리

00
8

Visual Basic2] 파일 처리에는 다음의 세 가지 형태가 있다.

랜덤 액세스는 같은 길이의 데이터를 읽기 SAS 한다. 데이터는 바이너리 gee
저장되고 불러오기는 선두부터가 아니라 임의의 위치에서도(즉, 랜덤에서)읽을 수 있

바이너리 액세스

바이너리 핵세스에서든  텍스트 데이터만이 아니라, 값 등 여러 가지 종류의 데이터
파일을 저장할 수 있다 ne 데이터가 어떻게 파일에 저장되고 있는지를 프로
그램이 이해해 두지 않으면 바른 입출력을 할 수 없다.

파일 Has 함수와

Visual 28810에서는 파일 처리용으로 표 12-1의 BES 준비하고 있다. grb 각각 순차
HAAS), 랜덤 AANA), 바이너리 액세스(82)로 사용 가능을 의미한다.

341


===== PAGE 336 =====
342

_ Chapter 12

파일 처리 함수

표 12-1

구분       이를          기능

srb        Dir            파일명과 디렉토리명을 반환한다

srb        ChDir          현재의 디렉토리를 변경한다

sro       MkDir         새로운 디렉토리를 만든다

srb        RmDir         디렉토리를 삭제한다

srb       ChDrive       현재의 드라이브를 변경한다

srb       CurDir         현재 드라이브의 PathS 반환한다

srb        FileCopy       파일을 복사한다

srb        GetAttr         .파일/디렉토리의 속성을 반환한다

sro       SetAttr        파일의 속성을 Hast

srb       FileDateTime    파일 잭성 AAS 바꾼다

srb       Kill           티스크로부터 파일명  명을 삭제한다

srb        Name          파일명/디렉토리명    을 변경한다

srb       FreeFile       사용 개능한(이직 미사용) 파일 번호를 바꾼다

srb        FileLen         파일 크기를 바이트 단위로 지정

srb        LOF           파일의 길이를 바이트 단위로 바꾼다

srb       EOF          파일의 |마지막 인지의 여부

srb       Seek          읽기/쓰기 위치를 설정한다

srb        Loc            열려있는 파일의 현재 위치를 반환한다

srb      Lock        파일을 잠그기한다(다른 프로세스로부터의 OH
세스 금지)

srb        UnLock         파일 잼그기를 삭제한다

sro        Reset           모든 파일을 닫는다

srb          Open             파일을 연다

Sr       Close         파일을 닫는다

8            Write #           데이터를 Commas} 이중 인용 부로 가공해서 읽는다

8          Input #         Write#= 쓴 데이터를 읽는다

8          Print #         데이터를 텍스트로서 쓴다

6          Line Input #     한 행 단위로 읽는다

rb        Put           지정 기록번호/바이트 위치에 쓴다

rb        Get           지정 기록번호/바이트 위치로부터 읽는다

sb         Input()          지정한 수의 BAS 읽는다

sb         InputB()        지정한 바이트 수의 BAS 읽는다

주) 106나8는 문자열을 바이너리 데이터로서 취급한 때에 사용


===== PAGE 337 =====
12.4 순차 액세스

순차 파일은 기본적으로는 문자가 줄줄 들어가 있는 파일이다. Print#, Input#o| 행 단
위의 쓰기/읽기를 하는 것이 기본 용법이다.

Write#, Input#& 사용하면 쓸 때에 특별한 가공을 하는 것에 의해 수값을 직접 쓰거나
타입이 다른 복수의 변수에서 읽기를 할 수 있다.

파일 열기
                                    Input

Open 2!" For Output  | As #n [Len = 버퍼사이즈]
00600

Input 파일로부터 문자열을 읽는다.

Output - 파일에 문자열을 쓴다.

Append 파일에 문자열을 추가 쓰기를 한다.

#n          사용하는 파일 WSS 지정. 숫자로 # 처럼 기술해도 좋고 Integer Y 변수를 사용해서
#PileNbr 13 기술해도 좋다. 이 Ae 이후의 입출력에서 특정 파일을 위해서 사용한다.

ten 데이터 전송용의 버퍼의 용량을 지정한다(보통은 생략한다).

파일 닫기
  Close 파일 번호

Close 랜덤 액세스에서도 바이너리 액세스에서도 용법은 같다. 이후

음은 Close 2] 사용 예이다

1°,
ner,
oft
ro
ox
“at
에

Close #1 00009 1, 파일을
Close #1, #3 ©9941     는    다
Close            ㆍ오픈되어 있는 전체 파일을 닫는다

343


===== PAGE 338 =====
Chapter 12 파일 처리 함수

Print #n, 한 행 출력 리스트 출력 리스트로 표시된 한 행분의 데이터를 쓴다

Line Input #n, 변수            파일로부터 한 행씩 읽고 변수에 넣는다
Write #n, 출력 리스트           출력리스트로 표시된 데이터를 Comma 구분으로 쓴다
Input #n, 변수명 리스트        파일로부터 읽고 변수에 넣는다
Input (문자수, #n)       지정 문자 수만 읽는다
예 : Print #1, "SSS" 00000]한 행 출력
Print #1, "S52", ste출력하고 줄바꿈하지 않음
Print #1, .!직업트 ; Tab ; "OlAf" | ---.--탭으로 구분하여 출력
Print #1, Tab(20); "오늘은! = ……20항목부터 출력
Print #1, Spc(3); "오늘은"; = ……공백3문자 나중에 출력
Print #1, 2 | 에여공백 라인을 출력
Print #1, Textl.Text ©2020 000 wr텍스트 박스의 내용 전체를 출력한다
Line Input #1, MyStr 00000한 SH 읽어 mystrol] 넣기
Write #n, "단가", 3000 아다문자와 정수를 출력
Write #2, 00000 1 아따공백 라인을 출력
Input #m, MyStr, Kakaku 00000문자와 수치를 변수에 입력
MyStr = Input(10, #1) | 마마10문자를 읽어 mystrol| 넣기

Print#2} Line Input#, \11[#과 Input#® 대조되어 사용된다.
Print#AS 출력 데이터는 기본적으로 행의 텍스트로서 그대로 쓰인다. 이것에 의해
Write#o| Ee 출력은 구분되어 작성된다. 예를 들면

Print #n, ,"ABCD":1234
Print #n,"EFGH",5678

의 쓰기 데이터는 다음과 같다. 여기에서 WritevoH 의한 특별 데이터는 InputkS 사용하면
바르게 인식되어 읽혀진다.

344


===== PAGE 339 =====
Write#2| 읽기 전용 데이터

문자열은 이중 인용       수치는 이중 인용
부호로 둘러쌓인다      부호없는 문자가 된다

구별하기 위해 컴머가 들어간다     개항

파일의 끝을 조사하기 위해서 다음의 함수가 있다.

： 2080일 번회

파일의 끝에 도달해 있으면 True

파일 AAS 읽는 BLS 이 함수를 사용해서 다음처럼 한다.

띠플법로빈램
간단한 프로그램 예이다. 쓰기 HES 클릭하면 파일에 데이터를 쓴다. 읽기 버튼을 클릭
|면 읽기를 하고 데이터를 리스트 박스에

el

더

>

| 0%
Th
on

Fo] 리스트 박스와 명령 버튼 두 개를 바치하여 다음의 속성 설정을 한다.

주) 리스트 1은 표준 그대로 사용한다

345


===== PAGE 340 =====
oo
+

Chapter 12 파일 처리

코는

Private Sub Command1_Click()
Open "c:\mydata\sfile.dt" For Output As #1 파일 열기
Print #1, "선두행"            |
Print #1, ‘1234567890"        |
Print #1, "abcdefghij"      |
Print #1, "ABCDEFGHIJ"
Print #1, "가나다라마바사0"
Print #1, "최종행"
Close #1                     fo
End Sub                            |

no
또
end

Private Sub Command2_Click()
Dim MyStr As String            |
List1.Clear               ㅣ   "리스트 HAO] 내용

을 삭제한다.
Open "c:\mydata\sfile.dt" For Input As #1
Do While Not EOF(1)           | '파일의. 가장 마지막에서 Loop
Line Input #1, MyStr
Listl.AddItem MyStr       | ‘BIAS 빅스에 추가 트시한다
Loop                        |
Close #1
End Sub

346


===== PAGE 341 =====
12.5 랜덤 액세스

랜덤 액세스용 파일은 동일한 길이의 데이
이터의 보관되어있는 위치를 알 수 있다. 이
를 기록하면 좋다.

를              고 있어서 번째 데
단위가 되는 동일한 길이의 데이터 정보

레코드 정의

레코드는 단일 혹은 복수의 변수로 구성된다. 복수의 변수를 사용할 때에는 사용자 정의형
으로서 지정한다. 예를 들면 이름과 AB] 있는 260802마는 FEBS 다음과 같다. 레코
드로 자용하는                         § 길이 문자열이라고 한다.

Type Person                ‘Persona 정의
Namae As String * 20
Nenrei As Integer

End Type

Dim Meibo As Person          ‘Person & 변수 Meibo Ml

파일 열기
      open 파일명 [For Random] As #n Len = 레코드 길이

mm 사용하는 파일번호
ten 레코드의 길이를 설

ㆍ “For Random” 사용하는 파일 번호
어그

:레코드의 AoE Lente Ca 다음처럼 기술한다.

Dim Meibo As Person          Person 변수 Meibo 선언
Dim RecLen As Integer        '길이 S22 변수

RecLen = Len(Meibo)           레코드의 길이를 구함

Open "mydata.dt" For Random As #1 Len = RecLen =|
Open "mydata.dt" For Random As #1 Len = Len(Meibo)

347



===== PAGE 342 =====
Chapter 12 파일 처리 함수

치에 데이터를 작성

“지정 레코드

위
* 레코드 번호를 생략하면 다음의 위치에서 작성

1부터 시작

*레코드 번호

    Get #n, [레코드 번호], 변수명
*지정 레코드 위치의 데이터를 읽는다
*레코드 번호를 생략하면 다음의 위치로에서 읽는다
음은 Put» Get > 사용 예입니다.
Put #1, RecNbr, Meibo  「[60140「에 표시된 위치에 !(6160데이터를 저장한다

Put #1, , Meibo       ‘THS 위치에 작성한다
Get #1, RecNbr, Meibo   ‘RecNbr mio} 레크드를 6160 에 읽어 들인다

레코드 바꿔 쓰기 _ a
어떤 레코드 USS 바꿔 쓸 때에는 다음처럼 한다

Get #1, RecNbr, Meibo 필요한 레코드를 읽어 들인다

|

40160  변수            수정한다)

Put #1, RecNbr, Meibo 원 위치에서 ne 장한다

yl 액세스 파일의 끝에 새로운 TER 추가하는 경우는 현자의 총 레코드 수에 1을 더하
고 그 레코드 위치에 쓴다. 총 레코드 수는 파일 a7 ea  레코드 3712 나눈 OE 다음의
LastRec= $ 레코드 수를 관리하는 12668@형 변수로 작성하여 사용자가 관리한다.

본. ,

348



===== PAGE 343 =====
12.5 랜덤 액세스

LastRec = LOF(n) W Len(Meibo)     총 레코드 48 구한다
LastRec = LastRec + 1        43 더한다
Put #1, LastRec, Meibo      '그곳에서 읽어 들여서 추가한다

LOF 함수는 지정한 파일의 길이를 바이트 단위로 바꾼다. 서식은 다음과 같다.
    10따일번회

+ QE 시에 사용한 파일 번호를 사용해서 지정한다

레코드 삭제                        되

ig AL 특정 ATES 삭제하는 기능은 없다. 단지 Mol +> 없게 되어도 총
다면 모두 공백 문자(혹은 값이를 레코드에 쓰면 된다. 그러나 이것에서는 데이터 영역은 그
대로 남아 있다. 완전한 레코드를 삭제는 파일 AS 파일 BS 복사하는 과정어서 필요 없는
레코드를 버리도록(복사하지않도록) 한다. 이 때는 원래의 파일을 삭제하기 위하여 kill 명령
문과 파일명을 WASP 위하여 Name BALL 사용한다,

떠플법로트램

랜덤 액세스의 프로그램 예로 레코드
고 표시한다; 치가 데ㅇ |터와 레코드 번

fa

번호를 deals 읽기 vee 클릭하면 데이터를 a
c= 입력해서 쓰기 HES 클릭하면 데이터를
이 프로

이 프로그램의 이름                 한다.          AAS 보통의 소스 파일 7ㅁ01116. frm 5I 외
에 표준 모듈 — basS 사용한다. 표준 모듈은 [프로젝트(2)]-[모듈 S7KMIMNA 추가
한다.
속성 설정

폼에 리스트 박스와 명령 버튼 3 개, 라벨 3개 ,텍스트 박스 3개를 배치하고 다음의 속성을 설
정한다.

Commandi       Caption            Poe
Command2       Caption           “쓰기 `
Command3       Caption            ‘Sz’
Labelt                Caption                 aac 번호
Label2           Caption            “이름”
Label3               Caption                 “He”

349


===== PAGE 344 =====
350

Chapter 12

no!
+

파일 처리

코드 rndfile.bas

Type Person                =
Namae As String * 20     |
Nenrei As Integer        | | 내용:
End Type
Global Meibo As Person       |
Global LastRec As Integer   a

코드 randfile.frm

Private Sub Form_Load()
Open "c:\mydata\rfile.dt" For Random As #1 Len = Len(Meibo) = @7

LastRec = LOF(1) W Len(Meibo)         레코드 AS 구한다
End Sub
Private Sub Command1_Click()                      :
If Val (Text1.Text) < 1 Or Val(Textl.Text) > LastRec       신규 데이터인가
Textl.Text = LastRec + 1          ‘Al 데이터
Text2.Text = 신규"
Text3 Text = ""
Else
Get #1, Val(Text1.Text), Meibo    기존 데이터 읽어 들이기
Text2.Text = Meibo.Namae          텍스트 박스에 표시
Text3.Text = Meibo.Nenrei
End If
End Sub
Private Sub Command2_Click()                쓰기
Meibo.Namae = Text2.Text              '데이터를 레            |=

Meibo.Nenrei = Val (Text3.Text)
Tf Val (Text1.Text) < 1 Or Val(Text1.Text) > LastRec Then 추기는 어디에
LastRec = LastRec + 1

Put #1, LastRec, Meibo           주가 쓰기
Text1.Text = LastRec             '새로운 레코드 번호 표시
Else
Put #1, Val (Text1.Text), Meibo    기존 데이터 바꿔 쓰기
End If
End Sub
Private Sub Command3_Click()
Close #1
End
End Sub


===== PAGE 345 =====
12.6 바이너리 액세스

동작의 확인
(1 코드 번호를 입력해서 읽기 HES 클릭하면 그 레코드의 내용이 읽혀져서 표시된다.

(3) 레코도 번호가 1-LastRec 의 범위에 없었다면 신설추가 파일로서 추가용 레코드 WSS

표시하고 이름란에 신설이라고 표시한다.

@ 쓰기 HES 클릭하면 표시되어 있는 레코

드 번호에 쓴다.
@ 종료 HES 클릭하면 파일을 닫고 프로그램을 종

료한다.

크럼 12 -2

바이너리 액세스는 순차 액세스처럼 앞에서부터 데이터를 읽어 가는 방법이다. 그러나 데
이터는 모두 바이트로 관리되므로(순차 파일에서는 수값도 문자열로서 보관된다.) 상급자는
유연한 파일 조작을 할 수 있으며 가변길이 문자도 보존할 수 있다. 파일 크기도 다른 방식보
다 적게 되고 지정한 바이트부터 읽기도 가능하다. 그러나 수준 낮은 기능만이라면 초보자에

게 말할 수 없다. 입문자는 아직 순차 파일 다음으로 필요하다면 랜덤 액세스 파일을 사용하
면 충분하다.

“Hi  바이너리 데이터를 처리할 때에는 바이트형 배열을 사용하면 안전하다.
NOTE

351


===== PAGE 346 =====
Chapter 12 파일 처리 함수

바이너리 열기
      Open 파일명 oe Binary As #n

wn -사용하는 파일 번호

a)

데이터 읽기                 베커

     Put #n, [바이트 위치], 변수명

ㆍ 지정 바이트 위치에 데이터를 쓴다.
ㆍ 바이트 위치를 생략하면 다음의 위치에 쓴다.

* 바이트 위치는 1부터 시작한다.
     Get #n, [바이트 위치], 변수명
*ㆍ지정 바이트 위치의 데이터를 쓴다.

ㆍ 바이트 위치를 생략하면 다음의 위치부터 읽는다.
ㆍ읽는 데이터의 구분은 변수 타입으로 판정된다.

Input (24}4s,#n)
:지정 문자수만 읽는다.

다음과 같이 사용 방법을 표시한다.

Put #1, BPos, MyStr         ‘Pos 나타내는 바이트 위치에 MyStr 데이터를 쓴다
Put #1, , MyStr          다음 위치에 Act

Get #1, BPos, MyStr        BPosH{O|E 째의 데이터를 MyStr ol], 읽는다

MyStr = Input(10, #1)      10문자 읽기 MyStrol] 넣는다

바이너리 액세스의 내용 저리

바이너리 액세스와 보통의 순차 액세스의 차이를 살펴보자.

352



===== PAGE 347 =====
12.6 바이너리 액세스

내부 표현
바이너리 액세스와 순차 익세스에서는 내용 HERO] 다르다. 다음 oS 보자.

순차 쓰기와 보관 데이터

Dim ss As String

Open "c:\mydata\sss.dt" For Output As #1
ss = "ABC"

Print #1, ss

Print #1, ss

Close #1

‘A’ "B' 'C’ CR BF 'A' "B' 'C' CR LF

저장 데이터=*| 41 | 42 . 43 | op oa 41 42 43 | 0ㅁ 0a

바이너리 읽기와 보관 데이터

Dim ss As String

Open "c:\mydata\bbb.dt" For Binary As #1
ss = “ABC”

Put #1), 38

Put 1, , 86

12 TB' tc! tar rBliige

저장 데이터=*| 41 | 42 | 43 | 41 | 42 | 43

저장 데이터 중 “41 42 49”은 문자 ‘A’, 'B’, '@ 의 데이터이다. “OD OA" E 복개 BAS
나타내는 FEE 이것은 문자열의 구분의 의미도 갖는다. 또 값은 다음처럼 보관된다.

바이너리 쓰기(값)

Dim ss As String

Dim ii As Integer

Dim bb As Byte

Open "c:\mydata\bbb.dt" For Binary As #1
ss = "ABC"

353


===== PAGE 348 =====
Chapter 12 파일 처리 함수

ii = 260
bb = 18
Put #1, , ss
Put tl, ; 12

Put #1, , bb
Put #1, , ss
Close #1

260
"Al 12! 16 18 'A' 'B' 160!

저장 데이터-*| 41 | 42 43) 04 01 12 | 41 42 43

이 데이터에서 “04 01”은 12168@형 값 260 을, 이어진 “12"는 바이트형 값 18 을 나타낸
다. 즉 시퀸스 파일의 경우의 값을 쓰는 방법은 데이터의 읽기를 참조하도록 하자.

읽기 데이터 폭               |

바이너리 처리에서는 보관되어 있는 데이터의 폭을 자동으로 판단해서 읽어간다. 값 변수
의 경우는 적절한 바이트 수 (바이트형이라면 1바이트, 10668@『형이라면 2바이트)만 읽을 수
있다. 고정 길이 자열 변수의 경우에는 그 선언시의 길이만 읽을 수 있다. 가변 문자열일 때는

현재 그 변수에 보관되어 있는 문자수만 AS 수 있다. 다음에서 그 읽는 예를 보자.

Dim ssi As String
Dim ss2 As String * 5
Dim ii As Integer, bb As Byte

ssl = "123"                '이것으로 3바이트 읽기라고 표시한다
Get #1, , ssi             SHEO|E 원기

Gat 11. 362              '652가5문자 폭 고정장에서 5바이트 읽기
Gop 101, , 31              101696「[형에서 2바이트 읽기

Get #1, , bb              '816형에서 1바이트 읽기

354


===== PAGE 349 =====
호/숫
Vi FEAL 이아아아사아아애사아아새사사아아아사아아에어 226
Cee 168
IN. osteamnems eenescvnconalrectireatitten antl ohoanedtenteen 164
Se oat ere peer Sr res eraser ere 164
어디에 164
를 cesteteceseeseaseetseeeseeseeensenessenessenenessenens 164
ee ee 164, 168
5 Behera eesrueeanes 어이 164
Bar carn SUR rence bar pecmrsqoe ct oar RODE ren era ar 166
(se eseseteeeeeeeeeteeeeeeeenetesseneenenesenesaeneney 166
잘: 이이 166
[gg ㅣ 이기여개매매매대대이이 119
이빈이러리00066668908 214
GIG ceseeeetanenameeeermeennes 이이 119
AYO Seeeeneeeeeeeeeaseeeenened ereesevonsneesenenens At
fT <Seeesnsu care at Seactacetaomipnnonnas 42, 116, 119
OQ: 여니 197, 214
SGN Bert od a ennrny ne etrntsmnstnn inlet SEAR CATES 120
FOR seatnnseiser aieustnaeemmeeeeeneerear 119
VDD cestessesetteereteeseeeeeeneeeeseneesessessess 42
립상었이인 120
WEA 0 에이미 214
0 166
6 ㅣ 니이 166
JE seereeeeseseeeesesseseeeneeeseseseneneneereetetaeiey 166
16 RIA 아아아아아아아아아애새새사아이아아이이이에아아아 27
GRA 아아아아아애아아이이이세아이에아애아이이이사아아사 27

기에 의한 호출 |…여~나새어에기이시개개-가 191

pe 17
개제 의 설정 ee ee 82
개체 LO) = ae 85
개체형 ……아아아아사사사사아아사사사사사사아아아아아아 154
구조체 ee 159
그래픽컬 컨트롤 ㆍ…아아아아아아아아아아사아아아아 310
기미 anenrteaaceseerc meena 267
기호 Se 160

날짜형 ………아아아아아아사아사아아사아아아아아아아아아 153
NB] EE ceeeeeeeeeseseseesrevessesesenseeeeeseeenenenees 168
논리 등식 …아아아아아아아아아아아아아아사아아아아아 168
논리: 연산자 coeeeesesesesnseseseserersensneneneeees 168
병리 처리 eee 168
SB] 포함 여여여어아애새어아새이이이어이어새에 168
EIST scscnaneanndpnnennnenirnsnnmnnnksnnanmnsnnkiiaka 168

다이어그램() 메뉴 ………아아아아아아아아아아아아아 73
단어 채우기 …‥…아아아아아사사사사바사아바사아아아아이 95
단정도 아아아아아아아아서서사아사머서사아바마아사아아이 151
데이터 오배 0 이러 0000.00 00000 270
데이터 읽기  …에아아아아아아아아사아아아아 344, 352
도구 모음 ㆍ…아아아아아아아바아아바아아바아아아아아아다 56
무구 ALT} saanescorssvesnssenernsssnvenenereemnanes 57
(oes g ger | oem eee eee er 78
fees ol Se 135
TESS) 메뉴 weeseceeeeseeeeseeseeeeneneneeeenes 75
도킹 탭 ㆍ아아어아아아어아서사사아아어사사아아아아아아 125



===== PAGE 350 =====
Index

도킹형 아어아아아아사서서사아아애서아사아아서서아아아어 57
디렉토리 리스트 박스 cere etter rere 251
CJT cecesteseeseseeeresssetsnnereeneeenessees 63, 97
디버그 도구 모음  Se A eesRae esi Roan CaN SNRE 78
디버그(2) 메뉴 seseeseeeseseeeeeeesenesareneeenees 70
디폴트 au yura a aoa walncbcaNis ae bib Sloineienatarain ace nisiniaie eis 203
ed a aS ㆍ…아아아아아아아아아아아아아아아아아이 203
캐
Fel = 206
BIOL asnsnntansncemesraranresnecasconnecarerceneanvensen 259
PH 액세스. ……~…내애비 341, 347
레코드 바꿔 AAD] …에여여어여여애이이애여여매애매에 348
레코드 삭제 ……아아마아아바사아마바아사아아아아아 349
레코드 읽기  initiates sniaiaiv on in ent ol ae Sonne Hate aR 348
레코드 정의  ee ee 347
레코드 AD} -nseeeevssessnesenanesvsononeeonnsnenss 348
리소스 파일 vsvevsesssveosososseeseseenssenscnanns 119
리스트 박스 …아아아아바아아아아아아아아아아아아아 232
매
마우스 이벤트  ……아아아아아사아아사아마아아아아아 296
매개 변수 정보  Ce ee 93
메뉴 cescesseeseesteseesessesesesseeeersessesseeneenees 72.
메뉴 바 ceseceseseeseeeereceeseeeeeeenseneneneeensenenes 56
메서뜨 ㆍ…아아아아사사사아아아아타타타아아이이이이이이아 19
명령  = ee 202
명령문  …아아아아아아아바바사아아마아사아아아마아아아이 21
명시적인 변수 선언 요구  Gs ani gnbieleneaiicee sien, 146
명시적인 선언  ………아아아아아마아아아사아아아아아 146
모듈으 신규 작성 0000900009000000000000000000000.0 122

무시저 선언. ee eae 144
문자열 연결. 거~거어거-여에에여연에내에새 168
모사 es ee 151

=
oe) ……여에아여역게매서아여나데이사에이1: 131
바이너리 GHIA. ………여여애애제세에세어 341, 351
바이너리 열2| ㅣ 여이며에타베재애새애며새매키재시이 352
바이트형 ……아어아아아아아사사아아아사사아아아사사아아 152
반인수 이서바버6.828이01216.81421011661616816.0101066166010히61614 186
배열 넘겨주기 …아아아아아아아사사아사아아아아아이 194
배열의 선언. -nn-sneseessacsssnneenesnennnctnenntons 149
S| So 151
배타적 BIE. 재애여여여셔에네애새서제에대대테이제 168
변수의 선언  oo Ce 144
변수의 통용 범위 ee 147
변수 이름의 IR) cxeecncecennmnnennaneurrerwennss 146
부기(\) 메튜 wnesaonencesessronnesavonnnunencnnnn 66
복수 명령문 lef aeigaies ain my etmrn'asornineo'aioesaioisle'elaelstsiniefte 26
UA FAI ncmcrneen nnn emaiennin 151
부울형 …아아아아아사사아아아아아아아아아아아아아아아아 153
부정 고부가 21160 168
비 도킹형 ㆍ……아애아아아여아사아아아사사아아아사아아아아 57
비교 연산자  Aas eael ea natn na a Hiejpuiaere ioe sine eaten oe 165
비트 처리 ㆍ여아아아아여아여어사아이이어이이이이아아 169

[새
사용자 정의 권트롤 …이여에시려시재배매에채내내 122
APE) BIOS 애에머새메메여셔셔니애너아서애 193
산술: 연산자] 여여 164
상수 목록 so 9 625s la arsiavalovsaava/oisuarotaro!ate tubo stsialatvioinin:eiainie:ei6ie 91

357


===== PAGE 351 =====
BEREBESSLSESES   SR EBRR   SRe
04 000:  떠 : i i  : a 뿌    op 1   <    : ㅠ 40
OH} 60 :  HI  10  : mr Ul : , HO    oT = :  시 Jo    : aS
rr 5 mo mv on eR I gy KO et   soi gin   에 해 내
wWoRPAC~ Tse awe ww oe wo   HEennmna   w) wl 피
| eee   RO 10 RK RP FE +   i
6009 [8 쓰노 의도옥이오    =
eB G7 Seeoneseeek   PSELIYSSLRLBRSA
오우 이 이 은    ㅠㅠ &        =) : 아
Mf bob bo: mom 은 은 은      세 : 기    고
Wii ot tot 펜메모코: :  x0     의 : aa    Bo:
wh PP oor uf mm <) qu ERE JE   ese i oO 해 : |: om oS
rn Pe ee 해 머   S2Qiqgwani tao yg
a a WH edo my oe   aneRe 2 RF wy wo wo 핀
= AS OO WO XO WO KT HO KK i ot 10 ied    TiN UU one es <I
x      = oR 4 <r <r <r <r <b <P O<H <H <M Py nar
0
을                      Oo

… 336

358|


===== PAGE 352 =====
키  이벤트   asia ele MWe Alo lareie ule Vibes Aca ele ptarala\e SIS NUANCE O's 296
El

타이머  tn sinie ecaso pi olmniaie sie aieleSisiewiciesiarsle'e Rian s amie saistacaies 247

텍스트 박스  ROCCE ICO COICO ROCCE PO TOCR) 209

통화형 PO er CLO Der Cana cOr Ont Cerne 151. 152

트리 EEE  327

일 끝 ㅣ: ㆍ아아아아아아아아어이이이아이이아어이이가아아에 345
파일 탈구 ee ee 343
파일 리스트 박스. eet rterrcocmecsnnrcinns 253
파월 OW AYAS sn assronerecanneaenntarnnannevennevente 340
파월 열기 c-cstencnecoreneannconnewnenracsunenessen 343
파일 패턴  TAR RERRE A cardia en Roehm 255
TOI) 메뉴 sxrxsenanenasonanasaneonsiricsosanenes 63
THA] ㆍ sonsesssnbeasseaeassonesmnereevenmoenreeansactscn 63
편집 도구 모음 …아아아아아아아아아아아아아아아아에 77
ENA 2 내이 124
편집기 BY xarevnsseesuneonsnseavenesersnecsniios 124
편집(6) 메뉴  siaiein aleiaiewpisisincn.eaie'sls nin nalacewiandibln evina'eie 08 64
평행선의 회전 ceaisien neneessenamansiacesseeveineneines 329
TUOlE: ssacssssnaneeesecavacsannereieard aascemecans 201
TEJA sesseesseenenavvnsatensenseonsaenssseentenssons 24

표준 도구 모음 eee 76
표준 모듈 ㅣ …아아아아아아사아아아아아아이이아아아아아 119
표준 | =e == a Ce 119

ZS EXE ceeeeessceeessneeeetesseneesssreneeoeenenaaee 55
프레임 veeeceeeseeteseeeseeeesseeteseesensetseeenens 223
프로시저 ㅣ ……아아아아어이에어이이아이에 21, 184
프로시저의 ALA). winecrenencrnntinntenstoninne 189
프로젝트 ee eee 116
프로젝트 복사 ceeeeeceeeeeseeeteeeeseetetenenaes 127
프로젝트 속성 EE 114
프로젝트 탐색기 wsnassnssecremerrenaeccrmsarwne 57
프로젝트의 구성 ㆍ……아아아아아아아아아아아아아아 120
프로젝트(2) 메뉴  ……여아아아아아아아아아아아아이 68
ee 218
픽처 박스 제거 ‥…아아어아아아아아아어아아아아아아 220

[캐

한국어 APS ……이이니새0000 28
일쑤 프랭시서 | 에세메마에 이이이 이 186
형 AN 문사 ㆍ새애새너내재재새새어새데져제제이새지재 145
SAO) 메뉴  Baisieia Sloe gees Rap wale wan eonn@eN sites eas 70
호출 스택 ……여아아아아이이아아이이이아이이이이사이이사 114
화면 레이아웃 ㅠ브여매셔에여애메이이치체시이어 57
화경, 관리 scarerscuteentynrcenserrerwermminanenes 116
힐베르트 곡선 …‥……아아아아아아아아사아아아아아아아 324

359


===== PAGE 353 =====
360

Index

개

개

ACCESS /아아아아아아아아아애아아아아아아아에아애아어 오서
Nos 1\V/-), GREE 55
F’Nele|| (211 REE 233
ANC cocceceereee etter terete te tetaeeeeeaeeesennes 168
And 연산자  ee ee ee 169
ASCII 문자 …아아아아아아아아아아어아아이아아아아아에 299
AutoRedraw 속성 ………아아아아사사사사아사사사 220
AutoSize 4 속성 Pe ee ee ee 207
매
ㅁ0600168[7 cerceeerceeeeeeeeeeeeteseeeeeeseteseeeeseeees 153
Boolean 형  ……0아아바사사사마사사사사사사아사아아아 151
BorderStyle 속 속성 EE 207
BorderStyle 속성값 ㆍ…아아아아아아아아아아아아 200
로 이으티로이오으으오도도 192
ONY (= eee 152
Bytes 라스 으으으 으으으 은 으으으 으으으 으으으 이 151
ByVal FA fo) a 191
a |
(0 | Ee 181
Call by reference errs 190
Calll by 변46 ----+srerreeesereneenseneneesennes 191
CANCE) ceeccceerreetereeeesteteteteteaeeeneeeeeaaees 203
Cancel 속성 ………아아아바사사사사사마사바아나나아 203
어(어어호0000000000000000000006006 219
CICK 아아아아아아애아애아이아이이이이기아아이이어아아아 296
Click 이벤트 …아아아아아아아사아아아사아아아아아나 214
CIOS 아여아아이어 343

대 _

Columns 속 속성 00000000000000000000000000=0.=0000000 234
ent Ce 271
Const 정수  wd en oinie Ainileainse oiaigesiticies eines nieinin eldlelae eats 160
Currency  0…0000000000000000000000000000.009.00.00 151, 152
CurrentX  sone nsiatiesGhiacieweew eta usle cetera eeee 219
CurrentY 속성  000000000000000000000000000000000099 219

베어 ㅣ 애거겨애개겨추니내재개 270
DatabaseName 속성 ……아아아아아아아아아아아 271
Dale:  ersters rescenesrencnmeesernmenerereics 153
Date 형  ……아아아아아사새서사사사사사아어아사사서사어 151
DB 그리뜨  …여아아아아아아아아아이애아이아아아아아아 271
DB 리스트 …여에애애애애겨아아아여어여서여여여새아에 271
DB 콤보 …아아아아아아사아아이이이아아사새새사애아아아 271
OBASE | 이아애억에개어가99 on
DDICHICK 아아아아아아아여아아아이이이사시이아에아아 296
Debug.Print severities 108
Default s-tsrersseneeceen ences 203
Default 속성 ……에에아아아아마아아아아사아사아아이 203
DIrLISIBOX «sesso ee seer 251
미이천트이어 는 지0060066 176
DGUBIG: r-2tte-oreeneneecnncsircteeenecisresesnaadl 151
키이이르(이이 00000 297
미(이이이이 이로0000 297
DrawMode 234g vsrsrrsessseeteeseeteeeees 260

Empty 값과 IsEmpty 함수 6.69544946바64454 158
Enable  6 :o:0p-wie)a:e:n nine wista wee eieiw eiucerpa eininin sie esnincn imines 248
End =I  Siecemtesiate aetna Etre ce eae rae 180


===== PAGE 354 =====
Index

EndDoc 메서드 ……아아아아아사사사사사사마아아아 291        Ta] (CA cee 248
EOF  1 WORGaalalh ase oleh owe Ses NWislkns Nieeea eee seems 345        Is 연산자 요비디지이디바11001110.0.5.5010.18.120.421916010.0 167
Eqv Sine Wein WE wis is\a)s Weiss ea el Weieewinwrnun la nines taremiereeriaceme's 168
EqQu HAR ssssessesseetstessessesssessssssecees 169    K |
Event-driven Programming oss 25
Ege) -nininnssvasancisananomnwansaadionernreanseate 262         KeyDOWn srrrreerrrsessesteeeseeceecesescescesnecs 297
면서 SS. ncncannevaumennsimecnomnesennmamemacceoen 179        KeyPreSS vrrrrerteeeeteseetseeeerenscre 210, 299
KeyUp  SO NRET Hesln vais wane es Neue cele sie naneeees enn 297
대
내
Filename 속성 rea aN aS cian a wie wlerninia/ainiecaiereiaieiacaiacece 254
SNCs 속성 om emencamiierantercien 258        LargeChange srs 243
FillStyle 속성  eer 258      LBound scajere nia Zoee 6 ieee ome MWR OO AlCNRERMO AA RNS MRO 194
For 분 아아아아아사아아아사사아아새사사아아사사아아사어 175         LIKE 연산자 …애애개새세셔새새사여여이기기매이아 166
Forms 콜렉션 이 18        Line  eisieieee aueihieecweisio at aap ou Geek alsa USNR ENE eeews 259
Faith ssamemcecnrmeremeeesanennreenceremvenn 271        Le TAs sostetiessencerescesrinereeremiony 259
Line 메서드 . …아아아사아바사사사사사바사사사아라사 219
G                                                  ListCount Bsa Sin eee Niele wa sre. S Tablets once emn' ein Klara wise mail 234
ListIndex  saya avons wider ote nie lniwa o erainiv eine eipigcn niece eeiei® 234
GoSub  a5 ase cfu Sian Sins Wao oeipietetniolnininleinie Ais ermonrecaslesisiks 181        LoadPicture 함수  aa eaieneusee a alesis wnaerae eens 214
Golo 문과 fal =| 178         LoadPicture() ……     psdiayencnanereeseeeanunseres                   220
Locked 속성 00161 이자버티 비기피이으1조 211
TH                                               Long  PC Cee OCC ee a oe 151
Lotus  aepis WRUNG TRAD USER ET WH ener ae Man ENN Reet N 271
HScrollBar  eC OTe ee 242
HTMLiZ& Sipin o la Win Wiaiala Siedler ORS ee S Ree AR ede ele 126   '
(Mi
|                                                   Max wi Re nae Laer Wa aCe wrerw eceseleca\ 0 ai ule aw nte arm atelevio en Homme) Pee 243
o                                              MDI Se Bsa Wg wsiaia slau l0iAli red ib 'e'e tine wie mieinia/siaiaininie/aie aigiaialear aie 126
  a “        — ee 272
50000 가 169         Min a:aigincale a:n-nieloie:vinin ain erniniaiaisipicinisaipia'n ea ces @ealele ewe siiena'e 243
InputBox  ware teitieaeiaioie clok'y atae cau a eS sieieemM eine ats 283       MOUuseDOWN rrr ala, 300
MouseMove  Pe eC COO re 300
Integer  미지이지테디티지터16116. 151

361


===== PAGE 355 =====
362

내

co |

MouseUp   BECO COCTR Or CCE ORES er  300

MouseUp  이벤트 a RAR QI sSeis ip nee omieinises emanes 214
MsgBox    OC OO ee ere CeO 280
MultiLine  속성  Pe ey 으으으 er 210

negotiateposition 속성 sisinioiaie :8/bieleininalenece #ieieceie'e 274
New Ween e eee e cece e teens nee eeeeeeeneneeeesseseeeeseeeees 155
Not  (Syaa(HiWia Sain inloin ern ejainis wis oin/ninia als SA SCaTOELE aS Sloeisle me eisiels 168
et 연신 자 axe ce crercesreaierrmmearremmmns 169
Nothing 00000000000000000000000000000000000000000000 155
NUII 값과 IsNull    00000000000000.000000000000000000 159

이 0000” 154
0616이 형 | 아아아아아바사사사사사사아사사사사사아아아 151
QUE seescesawaceisnacorccensnagneeaneannnnteeas tenons 261
OLE 사용자 정의 컨트롤 ㅣ. ………아아아아아아 120
OLE 컨테이너 | …아에아아아아마아아아아아아아아에에 261
(pM ee ore reece 181
(0) 0) =) 9 RR 343
OP 아이어 02000 168
(0) 연산자 EEE 169

|

가즈  ceeeceteeceteet ete ee eee ee este eee ee eee ee eee eee es 102
Print 메서드  minim man Za ne asad inininse-wlaTacnisnions Rin Realy 219
Printer 개체  a aK 6a ain Tu 4 @ cn lin'o espn yores[ag ALIN RIRINIOAR 291
Printers 콜렉션  = 10112 18
Private  caediniou saw sult WU Sealsinisies Ae S GW ieewevanir esa eans 184
PUDIIC crrttttet tt tet eet e sent e eee ee ee eee eee ee eee ees 184

cel |
QBColor 함수 바기오 309

R | |
RecordSource 속성  sfalnresoin [6 aie WS ulNaaNas Lerma 271
Redo  Se OO ee en ore re 131
Removeltem  메서드   05 ain 1a alae faiu wisn laibtalalereiataioialeia’s 233
RGB  in| sinipcnininiol' pin: wjein'spiaibin/alols evn 'hieiaraneis-civts\nieaiawieiviblvinislonne 230
RGB 함수  iefsTs FrsiaZee s/n 0inlela/nfniolosalale/Aioie/¥ ocaieixinipcnlew ain's'yiezeiu 308

Paradox anreo Wino 668/aln 46a WinTurubaraiGsalore-SiSiuiG'wielplw/alece aiaTuiNie's 271
Path 속성 onan sh aang WML anor 252
Picture 속성 000000000000000000000000000000000000009 214
Picture.Cls  RC te ee eer ae) 220
Picture1.Picture 000000000000000000 220

BSCAIEMOdG 속성 ……아………아사아아아에에에에 306
Screen Zia) 박애타새베이에에데대서대셔새재애=서인 307
SceraliBar 쪽섬ㅣ| 1배매매애여재새네이이시시재 210
GP| ㅣ 이시애 126
Select Case 분 -etarentecetceenerane 173
ISveifevoi(sto [ tpaseSorcaer sect sacem oonepetcecsoeecn ar 234
est gee rpms Reson er eres 154
SHAD verses eee teeeeeeeeeteeeneeeteeeeey 257
(Shape 속성 ㆍ…아아아아아아아아사아아아아아아아아아 258
Single 아아사아아아아아아사아사아아아아사아아아어아아이 151
SmallChange 아아아아아아사사아아아아아사아아아이 248
Stop Se '아아아아사아사아사아사아아사아아아아아 102, 179


===== PAGE 356 =====
Index

Stretch 속성 ……ㅇㅇㄴㄴㄴㅇㅇㄴㅁㄴㅇㅁㅁㅁㅁㄴㅁㄷㅁㅁㅇㅁㅁㅁㅇㄴㅇㄷㅇㅁㅁㄴㄷㄴㅇㅇㄴㅇㅇㄷㅇㄷㄷ0ㅇ0.0 214
String  Se ee ee 151
Sub 프로시저  00000000.000.00000000ㅋㅁㅇ0ㄴㅇㅁㅇㄴ…ㄷㅋㄷㄷㄷ 184         Xor  ㅇ…00ㄴ00000000000000000009000000000000000000000 168
Sub 프로시저 호출 01000@이느디지지10100 185        Xor 연산자 PO COC eee 169
개
TapStop  000000000900000000ㄷㄴ000000000000000.0.0.0.00.00.0 203
Timer aoe koi nia a aie Stnininc nin ni6le wine's nln ara:nie'sininiacwreiee 247
내
UBound cor rer er es 194
Undo  ee ee 131
VE
Value éruissavernaralaveuniece’ wale biAinieierne wieipie alainlaia/sinie-siraiae.ales.eaie 243
Value 속성  이00019001000000000000000000000.09100.0 230
Variant  ……0000000000000000000000000000000000000000000 157
Vartype 함수  SSPEG RAMEE AUT RENEE NS aMEN ER 158
VBX 사용자 정의 컨트롤 ㅣ ……아아아사사아사아 120
Visual 88610의 환경 옵션 설정 ………… 123
VScrollBar  Sessa ganeninakne keverwmuctoad wanes: 246
m7 |
While ..Wend 2 Annis ais bialele aiaieia d sioinieralRigiatnieeaeataless 176
With 문  EnextiodncaManeienadesnesoicanpaneteeteswenns 180
Word  eee COC Oo erty Oe 262
WordWrap 속성  00000000000000000000000000000=000 207

363


===== PAGE 357 =====
프로그래밍 언어 마스터 시리즈 New 비주얼 베이직 6

1판1쇄 발행 1999년 9월 30일
1판6쇄 발행 2002년 9월 25일

저 자
HARUHIKO HAYASHI
발행인
이 문 칠
발행처
(주)영진닷컴
주 소

서울 서초구 서초동 1623-10 (우)137-878

대표전화 1588ㅡ0789

대표팩스 (02) 2105—2200

문의전화 (02) 2105-2010

문의팩스 (02) 2105—2203

등   록 1987. 11. 5. 제 03-00095호

값그그.(00() 원
© 1999., 2002. (주)영진닷컴 ISBN 89-314-1287-8
(본 누적쿠폰을 오려서 엽서에 붙여주세요.)

프로그래밍 업어 마스터 시리즈 New 비주얼 베이직 6

9"788  1

ISBN 89-314-1287-8

http://www.youngjin.com

※ 내용 I= http://www.youngjin.com2= 해주시기 바랍니다.

