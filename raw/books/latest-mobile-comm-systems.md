---
source_url: /run/media/yutae/Data/최신 이동통신시스템.pdf
title: 최신 이동통신 시스템
subtitle: "MATLAB 실습예제가 풍부한 — 유비쿼터스 모바일 시대의 가이드북 (원서: Simulation and Software Radio for Mobile Communications)"
author: 차종상 · 이종헌 · 강창목 · 왕진철 편역 / Hiroshi Harada · Ramjee Prasad 원저
publisher: 도서출판 그린 (원서 Artech House, 2002, ISBN 1-58053-044-3)
year: 2002 (원서)
pages: 509 (scan)
ingested: 2026-10-18
sha256: 4ee568b8bfdbf9c5b45705fedfa49b97ec5bd31d83704aca2785b95dd7c59f1a
---

# 최신 이동통신 시스템 (raw source)
> **Warning:** scan-only PDF (UPDF, "Scanner System"). OCR'd via tesseract 5.5.3 (kor+eng, 300dpi); Korean/English/numeric tokens occasionally garbled — cross-check original PDF when interpreting (esp. formula numbers, equation symbols, MATLAB code identifiers).
> 원서(EN): Harada & Prasad, *Simulation and software radio for mobile communications*, Artech House 2002.
> 국내 번역본: 차종상 외 3인 편역, 도서출판 그린 (2002~2003 추정).

## 장 (chapter) structure (from OCR'd TOC, pp.5-10)
| # | topic | approx. pages |
|---|-------|---------------|
| 서론 | 이동통신의 역사 및 다양한 시스템의 특징; 시뮬레이션 평가의 필요성 | 3-30 |
| 1 | 이동통신의 역사 (개척기/성장기), 이동통신시스템 분류 | 3-42 |
| 2 | MATLAB 기초 (벡터·행렬·인덱싱), 데이터 생성과 BER, 이동통신용 MATLAB I/O | 36-64 |
| 3 | 디지털 변조 (BPSK/QPSK/직교변조/OQPSK/MSK) + 시뮬레이션 | 65-131 |
| 4 | 채널 모델링 (AWGN/레이리/로레이), 채널 평가 | 131-? |
| 5 | 확산·CDMA (직접/주파수/시간 확산, Chirp, 확산 코드, Gold/직교 Gold), 시뮬레이션 | 266-295 |
| 6 | 다중접속 프로토콜 (비경합/경합, 순수/슬롯 ALOHA, 비경합/슬롯 CSMA), MATLAB 시뮬레이션 | 295-362 |
| 7 | 어레이 안테나·빔포밍, 셀룰러 시스템, 고속 데이터(10.7 MHz), 3G (5.8 GHz) | ~362-? |
| 8-10 | 소프트웨어 정의 무선 (SDR), 소프트웨어 무선 통신시스템, 통합 시뮬레이션 | ?-509 |
| 부록 6A/6C/6J | MATLAB 코드 소스 (전파·채널·BER·ALOHA/CSMA) | 358-364 |

## OCR text (all 509 pages)



===== PAGE 1 =====
차재상 | 이종현 | GAR | SAIN 편역
Hiroshi Harada | Ramjee Prasad 원저



===== PAGE 2 =====
Library of Congress Cataloging-in-Publication Data
Harada, Hiroshi, 1969-
Simulation and software radio for mobile communications / Hiroshi Harada,
Ramee Prasad.
p. cm. — (Artech House universal personal communications series)
Includes bibliographical references and index.
ISBN 1-58053-044-3 (alk. paper)
1. Wireless communication systems—Computer simulation. 2. Cellular telephone
systems—Computer simulation. I. Prasad, Ramjee. II. Title. __ III. Series.

TK5103.2 .H368 2002
621.3845'6—dc21                                                                                                                 2002019677

British Library Cataloguing in Publication Data
Harada, Hiroshi
Simulation and software radio for mobile communications. —
(Artech House universal personal communications series)
1. Wireless communication systems—Evaluation 2. Wireless communication
systems—Computer simulation 3. Mobile communication systems
I. Title II. Prasad, Ramjee
621.3'845

ISBN 1-58053-044-3
Cover design by Igor Valdman

© 2002 Hiroshi Harada and Ramjee Prasad
All rights reserved.

All rights reserved. Printed and bound in the United States of America. No part of this book
may be reproduced or utilized in any form or by any means, electronic or mechanical, including
photocopying, recording, or by any information storage and retrieval system, without permis-
sion in writing from the publisher.

All terms mentioned in this book that are known to be trademarks or service marks have
been appropriately capitalized. Artech House cannot attest to the accuracy of this information.
Use of a term in this book should not be regarded as affecting the validity of any trademark or

service mark.

International Standard Book Number: 1-58053-044-3
Library of Congress Catalog Card Number: 2002019677

10987654321

+ 책은 Hiroshi Harada2} Ramiee Prasad2| ‘Simulation and Software Radio for Mobile
Communications, 에 대하여 대학교수를 중심으로 한 전문가들이 모여 번역하고 재구성하였다.



===== PAGE 3 =====
역자서문

a

@ 본 교재의 필요성 및 집필 동기

a 정보화 사회는 통신 및 방송분야가 상호 접목됨과 동시에 다양한 형태의 시스템들이 이
동통신 기술을 토대로 언제 어디서나 누구와도 멀티미디어의 대용량 정보를 쉽게 공유할 수
있는 유비쿼터스 이동 통신시스템의 형태로 진화해 가고 있는 시대라고 할 수 있다.

이러한 유비쿼터스 모바일 시대에 있어서 관련 직무의 종사자 및 공학도들의 필수적인 기
초지식을 향상시키기 위해서는, 독자들에게 이동통신시스템의 핵심적인 지식들을 쉽고 명확
하게 이해시키고, 교재에 기술된 내용을 다양한 예제기반의 컴퓨터 실습과정을 통해서 완벽
하게 소화시킬 수 있도록 ESS 주는 전공 서적의 SH] 무엇보다도 필요하다고 할 수 있다.

이동통신시스템을 전공하고 현재 대학에서 연구 및 강의를 행하고 있는 본인으로서는 본
역서가 대한민국의 11분야의 종사자 및 관련 전공학생들로 하여금 이동통신시스템분야의 전
문적인 지식에 대한 갈증해소에 매우 큰 도움을 줄 수 있으리라는 확신을 갖고 여러분들의 힘
을 빌어 본 역서를 출판하게 되었다.

@ 본 교재의 구성

본 교재는 총 8장으로 구성되었으며 각 장 별 특징을 간략히 기술하면 다음과 같다.

제 1장에서는 이동통신의 역사 및 다양한 시스템의 특징, 컴퓨터 시뮬레이션에 의한 평가
모델 등에 BUSS 설명하고 있다.

제 2장에서는 본 교재에 수록된 각종 프로그램소스를 이용한 ASS 행하기 위한 기초지식
을 습득하게 하고자 통신용 범용 시뮬레이션 툴인 MATLAB) 관해서 소개하고 그 기초적인
사용법에 관해서 설명하고 있다.


===== PAGE 4 =====
   최신 이동통신시스템

제 3, 4, 5, 6, 7, 8 장에서는 이동통신시스템과 관련된 핵심적인 변복조 및 다중화와 다중접
속기술, 다양한 프로토콜 및 시스템 등에 관해서 상세히 다루고 있으며, 이론적인 설명과 이에
Bad 풍부한 시뮬레이션용 소스들을 제공하고 있다.

@ 본 교재의 특징

본 WAS 특징으로서는 통신분야의 범용 시뮬레이션 툴인 MATLABS] 사용방법과 시뮬
레이션에 관한 기초적인 지식을 제공한 후에 이동통신 분야의 전송기법 및 시스템에 관한 핵
심적인 내용을 기술함과 동시에 다양한 프로그래밍 기법들을 풍부한 예제 소스들과 함께 제
시해준다는 점에 있다. 따라서 본 교재는 이동통신 관련 학과의 수업용 교재로서 유용하게 활
용될 수 있으며, 이동통신관련 직무에 종사하는 실무자와 대학원생 등 연구자들에게도 아주
유용한 자료가 될 것이라 확신하는 바이다.

@ 감사의 글

본 책이 집필되기까지 기술적 조언을 아끼지 않으셨던 각 분야의 전문가들과 책의 산파역
할을 하여준 그린출판사의 윤덕우 사장님, 번역본 완성을 위해 노력해주신 이종현 교수님, 강
장묵 교수님, 왕진천 선생님, 번역된 원고의 오자를 정정해준 서경대학교의 통신시스템 연구
실 학생들 및 관계자 여러분께 진심으로 감사의 말씀을 전한다.

@ 마지막으로
본 책이 출간되기까지 1년여 시간 동안 결에서 묵묵히 도와주고 내조해준 역자 네 사람 모
두의 아내와 가족들, 그리고 하나님께 진심으로 감사의 말씀을 드립니다.

2005년 2월 20일 이른 아침에
역자 대표 차재상 올림

“Be the first, be the best or be different!”
최초가 되어라. 최고가 되어라. 아니면 차별화하여라!
시대를 앞서 나아가는 누리꾼에게 이 책을 바친다.



===== PAGE 5 =====
차례                                                                7y

서론

11 이동톡센의 6 gee ene ee eee et ee 3
1,2 이동통신시스템의 시뮬레이션 평가를 위한 모델의 분류ㅣ …………………………………%……% 7
12 지전대지점 통신 ee eae meenemis  ORen LSMeh” & eMC Pes 17
12 2. 지정 OI Bertier cen penton pees 21
eR eee 다지점봉신 지이나느아아토이 사혀저제데으이지치 24
1 3 0|책의:개설. ………0아아에아에제제에이가세재 르이가에더 이이 26
토지 고문헌 ene oc nenee ee ea rene wee Oe ee SCION 으으으 이 으이지으 29

2 Rit se 1. Sapenennen sere te mineromgenecron WoMES etecrieewt i! Stier STA PO. 7a 42 36
2.2.1 벡터와 행렬의 생성 ceveceeeeercccececensensnsessenesereeeeeeetenensnseenenenesseseseseesseseeseeneesees 36
2.22. 인덱싱과 서브스크립팅 one eneeeccncccncncecscnncesssanssnescchsscanccasseecesetccccescecscsascadguperss 38
2.2.5. 행렬과페터 계산법 . wicerecsn tester estieienteoee-apcheabigelguapse rb epetnccaegees 39

2.2.4 WAAR eerie ereeseedeeieasderiegpe ines henipeaeitunngens 43



===== PAGE 6 =====
최신 이동통신시스템

Cer 두립해산재 오티디이이이이시이 er enn eee oc ae
9.6 BBE ho] Sasercsecacssoncnninnsesvtcsarsntnasavccsovedseccnasaenneeneeusneetnansosnennsenetaenshentaoniczene
DE A Re ossecemnsoetint gosceceveqiosaviesgnsonsnnnvnssdeneearnnsiinenstonseennunsiiaersobeennammn seta
DiS UB 프로그래밍 soereecicepncorinsnsnnensnveconendonteceetonsilinsssantuenenpsteensonbbonensa eres

2.3 데이터 생성과 비트 98 (Bit Error Rate)

2A 이동통선용 MAH IO BO] nncecscrcccscecesnrsccecsecsrcsnsnnnnnssssssssssasscsscseesensenensoesenncuensenne
DAT: RGN SERD  nnnrme dsb enmmessssaeectretbectsgneretencessnontverivescateapeonepndornaownmminleghebie
CR ee meee ee © ert Oren ener Mea terete ater

3.2.1 BPSK 변조방식의 기본 구성 …아아아아아아아아아아아아아아아아아사아아아아아이이이이이이어아사사사세

3.2.2 이론적인 신호의 표기 …에에아에아아아아사아아아아아아이자아이이이이이아아이이이아아아아아아아아아아
3.2.3 컴퓨터 시뮬레이션 프로그램 ㆍ………아아아아아아아아아아아이이이아아미이이아어어아아아어사아아아아아

3.3.1 직교변조방식의 기본 구성 ㆍ………아아아아아아아아아이아아아아이지자이이이이이이사시사이이어사사아아아아
3.3.2 OPSK 변조방식의 기본 구성 ㆍ……아아아아바바바바바바바바바바바아바바아바바아타바아타사아아아아아아
3.3.3 컴퓨터 시뮬레이션 creeeceeteeceseeesnseecsnseescnstensssnensssnensssseesssntensnnsensssasnssnecnsaneees
3.4 OQPSK EST Tr er ss ree coer ster rere er St eer erecta rs
3.41 OQPSK 2} 기본 구성 ceseeeeeeeneteeeeeteteeeneenetetetseaenesensnenenseecansusenesaneneesennenenenys
3.4.2 컴퓨터 시뮬레이션 …아아아아아아아아아아아아여애애여아아아이아아자사아아새아아아아아사새사사아아아아
35 MSK. 000000000000000000000000000000000000 66006
3.5.1 MSK 변조방식의 기본 구성 ㆍ아아아아아아아아아아아아이아아아아아아이이이이시이사사아아아사사아아에
3.5.2 컴퓨터 시율레이션 cneeescssseesteseesccsssnsssestesssssssscnscsssnsnesecessnsssesansnsnnnvesseenssenneese



===== PAGE 7 =====
Contents   Ee

BiG GIMGK-- tsesescsncenthccrcansnnnsspnagantgdnenaitsyilienspincerecansateashapna tities acute tah it. da, aD eagle 127
3.6.1 GMSK 2} 기본 구성 ceveesseeeeensssessscenesnsnsnseenesseneneosssenseessceeeadiceesensenesersnbessenes 127
3.6.2 컴퓨터 시뮬레이션  cvvseeseesesenseecesnessecesneenensanseneastenseeeseeeeestasasansnpenceeesseessaeaeess 129

3.7 QAM. 00000 131
3.7.1 QAME] 기본 구성 vetsesseeesceesessssesssecsnsnctosneenesecapeeensnesnssseassussusanestesenseasensenes 131
3.7.2 컴퓨터 시뮬레이션  eveceseseeeeseeseceeseesesesseessnecsssesetenseenesseseabteasstsnnseesseaesesnaeasees 134

BB Sy Beet sa cscecsnasssccseccctsacecdensqesssssesesezistsaeticeascasesscecfbatbaaaepesscatsaissejaesges ey aapioeen dteaete 137

WAL TIS] creceecsccscecsessncsnnsnveccsresnenssuneescesecssessesensnerscessensesaeedeusacenesaeeausaesnseatsseeneasesaesaetans 138

tee y. eee 139

Pts, Bak ella EO we, (Batis. eerteemeneermemnemmneniopeenserts ter ob ty ne etiorn eb rieey 즈8 194
AS 000 전송기법에 태한 개념 nance scea os cl pvionerto npandoenipainanectnnetld 197

BBE 송선기 구성 ^ :=아여여5어아아내사세에저여애아제자댄저야티다버바지이타아어거데에어게자어메[아아이이 198

4.3 2. 수신기 구성 tea ae cicenttdsnsemncinegricen i acer opens omens 사에메아 201
AA 컴퓨터 시뮬레이션을 통한 OS 3s snerie cities csinen Sissons aegrrtreanse ean nds ienapesrsevtcony 203
4.5 D}QH 심볼-기반 (Pilot Symbol-Aided) OFDM 변조방식 ………………아아아아아아아아아아에 213
BC 결론 wevessssnssasssstaisnread dehitareardqeptbeds sosapesyipsenpiveosaigupidy 아수스 232
@ 참 고문 ceecsssccsrccsceonseenccsccencnencernneesestnessaneennensnsonisentecnssscerdoceoncnassanenscessceansesseessensennnes 233
을 부록 4소| 아아아아아이이이이 234

코드분할다중접속(1044) 기법


===== PAGE 8 =====
ia Eee

5.2 CDMA 키법의 개념 cweeecessecsssscecssscesssseessssensssssessssessnnsensnssenssseessnusessssanssnecesanesssneees 266
5.2.1 직접 APPZ creeeeeeeeeeeeeseseeeeeeteneenenenenseneeneneaeaseneeesanenessansnensnenenenerenneassenenenens 267
5.2.2 주파수 홈핑 ceeeeeeeeeeeceeeeseneseseeenereneeesenenenansnsnansesensnsnsnanenensneesassseceeeseranersenenss 271
5.2.3 시간 홈핑 ceseeseeeeeeeeeeseseetenenenenenterenenenentenensneneeeseensnensacacececensnensasscesenensenensens 275
5.2.4 (Chirp) 확산 스펙트럼 cverrseersreeeesssseeseseneesensenneenenensenesnennssenenenseesnanenenenes 2957
5.2.5 합성(9600) 시스템 ……아아에아아아아아아아아사아아아아아아아아아아아아아사사아사아사사아사사아아아아아 278

53 확산 코드의 생성 eeseessseesssecsseessneesssessssessssessnesnsssssnecssnensnsesanecsssensnecsnecssuecssnensnssnses 279
5.3.1 선형 귀환 전이 레지스터 01068『1660080( shift register)o] 의한 코드 생성 281
5.3.2 0 Ce cea 282
5.3.3 Gold A] QA. vressessessessssssssesseeneeneeseesnesneeneeneennennesnesneenseneeneenesneeneeneenennseneensens 284
5.3.4 직교 Gold A] GA vessesessessesessesesseeseenennensenencenenseneneensensnssnsntsnsneensenensensneenennes 286

5.4 컴퓨터 프로그램을 통한 송신기와 수신기의 구성 wvsvecssescsssecssseennssssneersneensneesnnensness 287

55 BER 성능 cvssesssssesssseesssseessssssssnseneensensnsensssnseneensenessenessscnnsensencensenssacensenseasenseassnneny 293
5.5.1 AWGN 환경에서의 BER 성능 ……아에아아아아아아사아아아사아아아아아사아사아사아사아사여사여사아 293
5.5.2 레일리 환경에서의 BER 성능 ………어아아아아아아아아아아아아아아아아이이이이어아사아아아사사아에 294

eee ee eS Ce | gece ae heeeemenmnnns eine ee eam ne oowre
6.2.1 비경합 (스케즐링) 다중접속 프로토콜 ese eneesteceeceeesecnseneetannennernnnnnsonete
6.2.2 경합(랜덤) 다중접속 프로토콜 ……………아아아아에에에아아아아아아사세아아사에사아에아아
6 3. 캔덤접속 프로토콜 nnn encssscesssccnsescnssecsseesnseestsseccnsebtnsnennecsevnecnvensnssesnvessnassnnseanassanens
6.4 컴퓨터 시뮬레이션에서의 보편적 조건 …………………………아아아에아아아아에아아아아아
641 게키 통신 시 ek pee ee ee mem a 에

6.4.2 시뮬레이션 SAO] PIL 구성. weeeeccceessseeccccnnnsseeneennseeenscsssnsnennnsnsnees



===== PAGE 9 =====
Contents    | x |

6.4.3 주 프로그램 csvrsessssesseneeneessnesnesesseenenseneseenssnsnsencensnsensessnsensnnsassnsanenssasensanenssess 328
6.4.4 부 프로그램의 설명 veesecsseseseesesenesseeeeseseessenennssaneensanenssesssensarsnsensassnsereaeensaes 334
6.5 순수 ALOHA …………아아아아아아아아아애아아이어 335
6.5.1 원 라 아아아아아아아아어어이아어아아이이이이기에 335
6.5.2 시뮬레이션 프로그램 ceveeeesescscseeeseseeseseesesesennensnseesenssssescenseeecsesnseensnenesceneneess 337
6.5.3 시뮬레이션 결과 cveesesessseeseeseseenesesesenesssenssesnssessensessesnssesasassnsnsnsensenensnsecsnsess 339
6.6 슬롯화된 ALOHA wrvsessesseeseesssssessessessessnsseessessenseseensstsnssessesanssnsssssessnssnsanasesensensens 340
6.6.1 원 기 vsseeseseessessessesnsseenesnseessesssssssnsessssenssesnssnsateassnssssnssassnsasensesscensenseserents 340
6.6.2 시뮬레이션 프로그램 sereeeeeescseseseeeeeeseseesescsesesneneeenssssesesnenenssescseensasasssseseeasees 342
6.6.3 시뮬레이션 결과 cveseesesseeseseeessesssesesenssssenesesnsneneecensesescsesnsessssnsnsnesensesensnensnsess 342
6.7 비영속적 CSMA cvvsvsssssseeesssssseesssesneessesssssessssnsessssensnssnsanessansasensessnnencensasensensansanenses 343
6.7.1 원 리 cvvssseeseessseessesnenssnsnsscssssesssevsnsscsssensessnssnssssnnsnsssenssenssusensenensensesusensensenes 343
6.7.2 시뮬레이션 모텔 vvesssseseesessenesesessensnssnenssnenenesssneneseensnssnsnsnsensacsnsnesesnsnssnenseceees 346
6.7.3 시뮬레이션 결과 crecesssseseseseesseeneseecsessseenseseseesnssenensssssensnsasssenseeneneasssscsceneeees 346
6.8 슬롯화된 H]AA SMA cvvesessseessssseesesessscsssnensessssnsenssessnssnssneesesansaesssssnsssseeeeneens 348
6.8.1 QL] cesseseeesseseessseesensnssnecsnssssessssssssnsssecensessnsnssnentasesesasesesssnensasensenecsnesneseaens 348
6.8.2 시뮬레이션 모텔 cvessescssssseseseseeseseenenssesceesesnesnsesseneessesesnsessesssesesesceseseneensees 351
6.8.3 시뮬레이션 결과 cvessesesseeeseeseseenesesessnesesensanencnesntessssnsnsecsssesseensessscesseensnesasens 351
GQ 결 론 crseeesseesesssnseesesessessacessnsansnsssansnssssesssssesscensesansnsessnsnsecsnsnsauensessnsnsacansnegsanensenennes 352
WALT cssessesessessssessssessesnsssnssnsessssssssssnsensncsnsessnsensncssssnsssausansnssnsnsensansanesusesessnsanseesates 353
WEN GA ceesssessesscsssneesesnssessesntensssncsssensaesansnsscsneensensnsenecnsseentenssnsseenssesnsanensenssnssneneansensan 356
# 부록 62 아아아아아사사사사사사아이이이이이이이이이이시이시이이이이이아아어 358
@ 부록 GC esveecscsssssseeseseseesssesnsscsnsanscssssnssssssnsnsesansnsassnsssensnsassnancausnsausnsauansassnansauensaeacensonees 364

7:2 MBA AJA BO] FHS De ASS 알고리즘 ……~…%0…4…%5~5아아타사아아아하아 388
7 3 몽적채널할당 시스템의 시뮬레이션 프로그램 oaeencaseeeneeeteceeseectnsesectnenecensesensesecensiee 391



===== PAGE 10 =====
| « ES

7.3.1 성능측정 eseseeeseesssnsneseesensenennsnsnnonnsseneecenennnnnnnssssscenrenennnnananneneses리수 391
7.3.2 전체 시뮬레이션의 흐름도 cveeseesseeseseneenneeeeeeesesseesneessssneensssnennsenneeeneeneennte 392
7.3.3 셀 레이아웃과 셀-랩핑 기술 ………아아아아바바바바사사라바바사아바바바사사바바바사바바마아사아아아마 394
7.3.4 Al 망(01694) 구성 vvsreecesesseeeeeseeeeeseteeeneeeeessssnseensnessseencnsennencnncnsnensnnensnsannanengy 396
7.3.5 ZO] 트래픽 인자 cvreeesesseseessseeeeseeesesressseensncnesnnnenenssnensenenennencannanennansanansncants 398
7.3.6 전송 조건 crsseeessessneeseseeseensnensnennneeeneessueesnenneeenseennesnasenneennianensanecaasengnannansnnenss 400
7.3.7 Ma, eh) a ma 401
7.3.8 채널체크와 재 할당 이아아아아사아사아사아어사사아어이아이이어사사애사사사사사서사새사아사사사사사사사아세 405
BQ ZY vvrreccseesssecsssssneesnsssneensnennnensnecsnstnnessnessseeneeaneenneenaesessanansonecnsanasenseeegsetes 405
7.4 DCA 알고리즘을 사용한 셀룰러 시스템의 시뮬레이션 결과 vrreeeeresrresereessrseerrseesnee 406
7.4.1 시뮬레이션 = Mc cae 406
7.4.2 0) BAO) BAY cvvsessssssnvsssnnansnssennsssessessessseessenceeeensneneesseeennnnnnnnnanansnsninarenssenet 408
7.5 셀룰러 시스템을 위한 어레이 안테나를 사용한 YS A (beamforming) 기술 ……… 409
7.5.1 CIR 향상 평가를 위한 시뮬레이션 프로그램 ㆍ…………*아아라아사바아아아아아사아아 411
1.5.2 시뮬레이션 결과 cvssssseesecececeeeeeeeeeeesseessnttssesensssseeenensnsusnenenssseeeseesnanssaatnnaes 416
FG 결 론 …아아아아아아아아아사사사사사사아이이이이자아아바아아사아사사사사사사사아사바아사바바배아사사배사사사사사사사사사사사 417
WETS coecseesesseessssessnessnsccnnesssnsensusecsneessnencuneensnnetsneesanecousessusenascsssacanssensctanecgnsacsnsess 418
EAA cesessssesssressneeesssensnnecsnicnnnsesesnecsnauecsunsccnsesensensanstanaasunersanacactecnauanennacennesensnageunseey 419

소프트웨어 무선 통신시스템

(Software Radio Communication Systems)

용어 A] 론 | reseessesseesneesesscescssesnsensssneennenneesneenecnnensnenssensnensaneeenssansnesenseasaneansangranseensngsetns 439
8.2 소프트웨어 무선 통신시스템의 정의 creesssccscesnnesesseessnnneseerssnnansesssssssstersenssnsssseeennens 441
8.2.1 안테나 장치 cesceeeeeseeeeesseseecseessnsesnnsarsstscenensnenssasansnensnscanegeencnsnageananeannanesenences 442
8.2.2 무선주파수 신호처리 장치 (REU) ㆍ……아어어아아사서사아여에아아사새사사사사사사사아사사아아아 442
8.2.3 중간주파수 신호처리 장치 (TEU) svsvressssessessssneeeesseseessnseensnnncescanennensnnennenseges 442

8.2.4 아날로그10-디지털 변환 (ADC) 9} 디지털10아날로그 변환 (DAC) 장치 443
8.2.5 기저대역 신호처리 장치 (880) vvesseeessseceereeeeterseeeessetecsssesernnetencnnensnnneseens 443



===== PAGE 11 =====
Contents     | ai |

8.2.6 전송제어 장지 (TCU) vvmveservnsssecssncscesssocccnsnsscenabesessosensetonseeersoseneccnanessssonssecs 444
8.2.7 입력/출력 (I/O) 처리 장치. 여아아아아아아아아이이아아아미이이이이이이이이사이이이이시이아이이아사어 445
8.2.8 End-+to-End 타이밍 처리 장치 (60 20) cee cece 445

8 3 소프트웨어 무선 통신시스템의 이점 ae cieecseieerig ets cies sctstermig einen 447

8.4 소프트웨어 무선 통신 서스템의 문제점 ceecseeesseecsseecnseecnerssessnseessenssesensessnscssaneessess 448

8.5 소프트웨어 무선 통신시스템의 기술 …………아아아아아아아아아아이이이이이이이사아이이이이이이이이이사아에 450
SSE 직접 AT erst terete ep seeaneeny 데레 아메드 450
8.5.2 샘플링 빵법 ㆍ…아아아아에아아아이미아아아이이이이이이이이아어에에 452
8.5.3 샘플링 레이트 변환 ㆍ…아아에아아아아아이이아아아이이이이이이다 455
8.5.4 DSPH 구조 cesessesesesesessssesneeeessessssseasecsssesesssssasenaeassesesnsnensesesenseseensarneeenenenes 464
8.5.5 인자제어 소프트웨어 무선 기술 crereereeeeeeeteeeeeeeteeeeeeeseeeesensesetseneeessesseeeesnenes 468
8.5.6 다수의 시스템을 위한 동시 신호-처리 방법 ㆍ……여…아아아아아에아이아애사이어애아아여아사 475
8.5.7 소프트웨어 무선 소자 ㆍ…에여여에어아아여아아여아아이아아이이아이이이이이이이이이어이이이이아아아 483

8 6 소프트웨어 무선 통신 시스템 프로젝트 eens ssscsssccssestsvotecsnvesosentennnsesoosnnetapeconnconests 487
8.6.1 미곡 csesesesseseesseeeeseseseeecneseseeeessnseensesecessessseuseecsestessseecsseesenecassasecensanecerenasenee 488
8.6.2 유 럽 아아아아아아아아아아이이이이이이아어 492
8.6.3 일 본 ㆍ에아아아아아아아아아아이아아이이 495

8. 7 소프트웨어 무선 통신시소템의 SESS :…………ㄴ……~너멕아어아나아아아다라디제제재아에아 500
8.7.1 향후의 이동통신에의 응용 …아아아아아에아아이이이아아사이이이이이이이이이이이이이이이사아아아사사아에 500
8.7.2 방송 응용 …아아아아아아아아이이시이아이어 502
8.7.3 사유 네트워크 여아아아사아아사이이이이이시이이이11999 503
87.4 .소프트웨어:꾸선설비의 있슴 방법. …아매에리레네아아 이00 503

88 결론 …거이거가저여여가거더하이아자아아어서어아테아레져에아제제여이기마세이여 기테어 506



===== PAGE 12 =====


===== PAGE 13 =====
이 책은 이동통신시스템에 대한 이해도를 극대화하기 위한 방편으로서, 이동통신 시
스템의 핵심적인 내용을 설명하고, 컴퓨터 시뮬레이션을 활용한 핵심적인 내용 및 시스
템을 구현 및 평가하는 기법을 병행하는 형태를 취하고 있다. 본 장에서는 무선통신 시
스템의 대표격인 이동통신 시스템의 역사를 살펴봄으로써 이동통신 시스템 연구에서
컴퓨터 시뮬레이션에 의한 구현 평가의 이점을 보인다. 또한 컴퓨터 시뮬레이션에 의한
구현 평가의 중요성도 언급된다. 마지막으로 이 책에서 다루는 범위와 컴퓨터 시뮬레이
션에 의한 이동통신 시스템의 구현과정을 보여주는 ISS 제시한다.

BEM) seus 역사

번창하고 있는 이동통신의 발전이 무선통신 역사의 주요 길목을 만들어왔다. 역사적
으로 이동통신 시스템이 표준화될 때 많은 시스템 제안들이 표준화 안에 상정되었다.
이 제안들은 컴퓨터 시물레이션이나 원형 제작에 의해 구현 평가되었고 최종적으로 하
나 혹은 소수의 표준 시스템들이 선택되었다. 표준화된 이동통신 시스템은 많은 중요한
개념들을 포함하고 있기에 이동통신의 역사를 조사하는 것은 최근의 이동통신 시스템
의 주요 사항들을 이해하는 좋은 방법이 된다.


===== PAGE 14 =====
a 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

이동통신의 역사는 세 시기로 범주화 될 수 있다. (1) 개척기 (2) 셀룰러 이전시기 (3)
셀룰러 시기 [1]. 표 1.1은 각 시기의 대표적인 사항을 정리해 놓은 것이다.

#표 1.18 이동통신의 역사

시대                                                      주요 사건

개척기

18608 | James Clark Maxwell] 전자기(5/)파 공리

18808 | Heinrich Rudolf Hertz] 의한 전자기파 존재의 증명

18908 | Gugliemo Marconi] 의한 최초의 무선 사용과 최초의 무선통신 Ss

1905 | Reginald Fessendenol| 의한 무선 링크를 통한 최초의 음성과 음악 신호 전송
A

1912 | 타이타닉의 침몰로 해상에서의 무선통신의 중요성 부각; 다음해에 해상무선전
신 도입

셀룰러 이전시기
1921 |디트로이트경찰국이이농무선필드테스트를행함
1933 | 미국,3040 MHz 영역에서 4개의 채널
1938 | 미국, 정규 서비스를 위한 법규
1940 | 22} 세계대전으로 무선통신 두각
1946 | Bell 시스템에 의해 세인트루이스에 설치된 최초의 상용 이동전화 시스템
1948 | 미국 버지니아 리치몬드에 설치된 최초의 상용 완전자동 이동전화 시스템
19508 | 마이크로파 전화와 통신 링크의 개발                                     |
19608 | 미국에서 자동채널할당 기능을 가진 자동차 무선 시스템의 소개
1970 | 여러 나라에서 사용 이동전화 시스템의 운용 (Al, 미 고속도로의 1억대의 운송
차량, 서독의 “BNetz”)

셀룰러 시기
19808 | 아날로그 셀룰러 시스템의 배치
19908 | 디지털 셀룰러의 배치와 디지털 시스템의 듀얼-모드 운용
2000s | Future public land mobile telecommunication system(FPLMTSs)
/international mobile telecommunications-2000(IMT-2000) /universal mobile
telecommunication systems(UMTS) 2} 멀티미디어 서비스 배치
2010s | 인터넷을 통한 고정점#》-기반 무선광대역통신과 소프트웨어 라디오 가능
20108+ | 광섬유 마이크로셀과 같은 FAS 통한 무선통신 가능



===== PAGE 15 =====
ae 00

개척기에는 무선통신에 대한 많은 기본 연구와 개발이 이루어졌다. 영국에서 1860년
대에 맥스웰에 의해 발표된 전자기파에 대한 공리들, 1880년대에 헤르츠에 의해 이루
어진 이들 전자기파의 존재에 대한 증명, 1890년대 이태리에서 마르코니에 의해 행해
Al 무선전신의 발명과 최초의 시연 등이 이 시기 유럽에서 행해진 주요 사건들이다 [2,
3]. 또한 일본에서는 1986년에 통신부에서 전기기술 연구소의 일부로 무선전신 연구부
서가 설립되고 무선전신을 연구하기 시작했다.

위에서 살펴본 기본 연구와 결과적인 무선전신의 발전으로부터 이동통신 시스템에
무선전신의 응용이 1920년대부터 시작되었다. 셀룰러 이전 시기는 디트로이트 경찰국
이 순찰차에 급한 연락을 보내기 위해 설치한 지상 이동 무선전화기 시스템에 의해 시
작되었으며 그 후, 1932년도에는 뉴욕 경찰국에도 설치되었다 [4]. 이 시스템은 234
의 주파수 대역에서 운용되었다 [4]. 아이러니한 일이지만 2차 세계대전 중에는 전쟁으
로 인해서 전파통신 기술의 급격한 발전이 이뤄졌다.

1946년에 세인트루이스에서 벨 전화연구소에 의해 150-MHz 주파수 대역에서 운용
되는 최초의 상업적인 이동전화 시스템이 구현된다. 시연된 시스템은 수동으로 전화를
교환하는 단순한 아날로그 통신시스템이었다.

그 후 1969년에 양방향 이동통신 시스템이 450-MHz 주파수 대역에서 구현되었다.
이 HAS 시스템에서는 자동적으로 전화 교환이 이루어졌다 [5]. Improved mobile
telephone system (IMTS)°]2} 불린 새로운 시스템이 미국 전역에 설치되었다. 그러나
큰 유효통화범위 영역 때문에 이 시스템은 많은 사용자나 효과적인 유용 주파수 대역의
할당을 처리할 수 없었다.

셀룰러 영역에 대한 개념은 이런 문제를                             을 이용해 해결하고자
개발되었다. 그림 1.1에 셀룰러 영역에 대한 기념     을 보였다. 한 셀룰러 영역의 주파수
채널이 다른 셀룰러 영역에서도 사용된다.

~ 같은 주파수 채널을 사용하는 셀룰러 영역간의 거리는 간섭이 충분히 적을 정

충분히 멀어야 한다. 이러한 새로운 셀룰러 영역에 대한 개념 사용이 셀룰러 시기
자 세 번째 시기를 열었다.

글
es
Sie
16
es
분
in
=
tho



===== PAGE 16 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simufation

Cellular zone

를 그림 1.1 셀룰러 영역 개념

최초의 셀룰러 이동통신 세대는 1980년에서 1990년대에 개발되었다. 이 시기의 연
PAHS (R&D) = 아날로그 셀룰러 통신 시스템에 집중되어 있다. 표 1.2는 이들 아날로
그 셀룰러 통신 시스템을 정리한 것이다.

《표 1.28 아날로그 셀룰러 무선통신 시스템의 정리

시스템                 AMPS           NMT-450       NMT-900          TACS         ETACS

즈        ~

ody ; ~      824-849/              453-457.5/ | 890-915/           890-915/ | 872-905/
869-894               463-467.5 | 463-467.5          935-960        917-950

(MHz)

채널간격 042)        30                    25             12.5*              2.5            2.5

채널의 수              832                   180           1,999              1,000          1,240

ie                      미국, 호주,            유럽            유럽, 중국, | 영국            유럽,
중국, 동남 아시아                     인도, 아프리카                      아프리카



===== PAGE 17 =====
Radicom-        JTACS/
시스템                  C-450             RTMS                                               NTT
|                                 2000      NTACS
450-455.74/          405-455/ | 165,2-168.4/ | 915-925/ | 925-940/
460-465.74 460-465 | 169,8-173 860-870 | 870-855
192.5-199.5/ | 898-901/ | 915-918.5/
주파수 영역                                                                          5                       :
ae Aa                                                         200.5-207.5         843-846 | 860-863.5
ile                                                     215.5-233.5/ | 918,5-922/ | 922-925/
—                                                      207.5-215.5       863.5-867 | 967-870
414.8-418/
424.8-428
12.5               25/12.5* | 25/6,25*
채널간격 (kHz)        10*                  25                                25/12.5* | 6.25*
12.5*      6.25*
256 400/800 | 600/2400
573                  200           560                120/240 | 560
qiJLj o] &
채널의 수                                               640               280           480
256
지역                                     독일, 포르투갈             이탈리아 | 프랑스                        일본                    일본

* 중복이나 “격자” 채널을 사용한 주파수 교차배치; 채널간격은 채널 대역폭의 반

미국에서는 20080060 mobile phone service (484729)라 불리는 아날로그 셀룰러 이
SSA 서비스가 1983년 시카고에서 시작되었다 [6].
다수의 셀룰러 이동통신 서비스가 유럽에서 시작되었다. 노르웨이에서 Nordic
Mobile Telephones (NMT)7} 아날로그 셀룰러 이동통신 시스템 개발에 성공하였다:

NMT-450 [7].

영국에서는 Motorola7} AMPSoel] 기반 한 total access communication system
(TACS)2} 불리는 아날로그 셀룰러 이동통신 시스템을 1984년-1985년에 걸쳐 개발하
였다. 1983%4 ol] = NMT7} NMT-900°] 2} 불리는 74191 NMT-450 서비스를 개시하였

고 C-450, RTMS, Radicom-2000°] 각각 독일, 이탈리아, 프랑스에 소개되었다.

일본에서는 Nippon Telephone and Telegraph (NTT)7} 800-MHz 주파수 대역의 셀
Br] 이동통신 시스템을 개발하고 1979년 12월 도쿄에서 서비스를 시작하였다. 또한


===== PAGE 18 =====
Zy 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

일본의 주파수 운용 계획에 맞게 개선된 1&068인 JTACS7} 198914 7월 소개되었다.

그 후 필요 주파수 대역을 반으로 줄인 Bg (narrowband) TACS (NTACS)7}
1991년 10월부터 서비스 되었다.

지금까지 아날로그 셀룰러 이동통신 시스템의 발전에 대해 언급했다. 그러나 이러한
다양한 시스템들의 비호환성 때문에 로밍이 배제되었다. 이는 사용자가 다른 나라로 이
동했을 때 이동통신 단말기를 바꿔야한다는 의미이다. 게다가 아날로그 셀룰러 이동통
신 시스템은 사용자 수의 증가에 따른 충분한 수요 능력이 부족하고 음성의 질 또한 좋
지 못했다.

이러한 문제점들을 해결하기 위해 디지털 무선전파 개요에 기초한 셀룰러 이동통신
시스템의 연구개발이 시작되었다. 이 새로운 이동통신 시스템이 2세대 이동통신 시스
템으로 알려지게 되고 아날로그 셀룰러 시기는 1세대 이동통신 시스템으로 간주된다.
표1.3은 디지털 셀룰러 무선 시스템을 Bas 것이다.

8《표 1.3ㅅ 디지털 무선 시스템의 정리

GSM
시스템                                                 IS-54                   IS-95                 PDC
|                  DCS-1800
GSM:                                         Tx:869-894;                       Tx:869-894;                Tx:810-826;
ee               Tx:935-960;             Rx:824-849           Rx:824-849        Rx:940-956;
주파수 영역                                                                                                      ‘                :
(IA) Rx/'Tx         Rx:890-915                                                           Tx:1,429-1,453;
:       DCS-1800:                                                     :     -
;                CS-1800                                                   Rx:1,477-1,501
Tx:1,805-1,880;
Rx:1,710-1,785
채널간격 4412)      200                     30                     1.250              25
GSM: 124;            832                 20                1,600
ae oe                       ?                                                    ?
채널 수                DCS-1800:375
GSM: 8               3                    63                3
gure hae
MASSA | Hog 1800:16
다중접속           TDMA/FDMA        TDMA/FDMA       CDMA/FDMA | TDMA/FDMA
이중전신            FDD                  FDD                FDD             FDD
변조                        GMSK                        a / 4DQPSK              BPSK/QPSK        a / 4 DQPSK



===== PAGE 19 =====
음성부호화와    RPE-LTP        VSELP        QCELP      VSELP
속도 (Kbps)                 13                                      7.95                                8                               6.7
1/2                1/2              44413      9/17
채널부호화        Convolutional        Convolutional       다운링크 12     Convolutional
Convolutional
남 아시아      인도네시아     남동 아시아

REL-LTP: regular pulse-exciting longterm predictive coding; VSELP: vector-sum-excited linear

predictive coding; GSM: global system for mobile communication.

국제 로밍이 가능한 900-MHz 주파수 대역을 사용하는 이동통신을 위한 국제 시스템
(0634)이 1992년 유럽에서 서비스되기 시작했다. 1994년에는 1.8-GHz 주파수 대역을
사용하는 개선된 6984인 DCS-1800 서비스가 개시되었다.

북미에서는 1S-54 디지털 셀룰러 통신 시스템이 1989년 표준화되었다. 그 후 표준안
은 아날로그와 디지털 셀쿨러 통신 시스템 간의 양 BES BHHES 수정되어 1993
년에 DAMPS 혹은 18-136이라는 이름으로 소개되었다. 또한 코드분할 다중접속
(CDMA) 기반을 둔 최초의 시스템인 IS-957} 1993년 서비스를 시작하였다.

일본에서는 800-MHz5} 1.5GHz 주파수 대역을 사용하는 디지털 셀룰러 통신 혹은
개인 디지털 셀룰러 (PDC) 시스템이 각각 1993년과 1994년에 서비스를 시작하였다.

위의 디지털 시스템 외에도 새로운 디지털 무선 기술들에 의해 2세대 시스템을 보완
하게 된다. 일본의 76690081 handy-phone systems (PHSs) (이전 PHPs)>} 유럽에서의
digital enhanced (이전 European) cordless telephone (DECT) 그리고 북미의 276650081
access communication services (PACS)7} 그 예이다. 표 1.4는 이들 2세대 보완 시스템
들을 정리한 것이고 607016961616000707401080008, second generation (CT2)2} CT2+S
보여준다. 72에 대한 자세한 내용은 [10, 11]에서 찾을 수 있는데 012+는 캐나다에서
CT29] 공통 인터페이스를 개선한 버전이다.

2세대 이동통신 시스템에서는 유럼과 북미와 같은 몇몇 지역의 공통 표준화가 이루
어져 일부적인 로밍이 가능하게 되었다. 이점은 1세대와 비교해 2세대만이 갖는 특징
이다. 공통 표준화의 도래는 사용자에게 간단한 국제 로밍에 대한 감각을 일깨워주게



===== PAGE 20 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

HH148 디지털 무선 시스템의 정리

시스템                    CT2/CT2+                  DECT                      PHS                     PACS
주파수 영역                 CT2:864-868             1,880-1,990               1,895-1,919           Tx:1,850-1,910
(기지 Rx/Tx, MHz) | CT2+:944-948                                                          Rx:1,930-1,990
채널간격 4412)         100                   1.728                 300                300
채널 수                  40                      10                      77                   96
채널당 사용자 수    1            12           4          8
다중접속                    FDMA                     TDMA/FDMA         TDMA/FDMA | TDMA/FDMA
이중전신                    TDD                        TDD                        TDD                    TDD
변조                            GFSK                       GFSK                       z/4DQPSK | a/4DQPSK
음성부호화와속도 | ADPCM       ADPCM       ADPCM      ADPCM
(Kbps)                       32                            32                            32                        32
채널부호화                 None                       CRC                        CRC                    CRC
지역                      se apie ae                     일본 홍콩 | 미국

되고 전 세계적인 표준화를 요구하게 된다.

1990년-2000년 기간을 거쳐 디지털 신호처리의 혁신으로 무선 통신 뿐만 아니라 유
선통신의 방식도변화되었다. 이 기간 동안 음성, 데이터, 영상 그리고 동영상과 같은 모
든 정보들이 디지털화 되어 인터넷과 같은 전 세계적 네트워크를 통해 전송될 수 있게
되었다. 이동통신 이용자들은 이러한 디지털 데이터들을 이동통신 네트워크를 통해 전
송할 수 있기를 원하게 되었다. 그러나 2세대 이동통신 시스템에서는 데이터 전송 속도
가 제한되어 있어 새로운 고속의 이동통신 시스템의 필요성이 대두되었다. 이러한 목적
을 바탕으로 1995년에 3세대 이동통신 시스템에 대한 연구개발이 시작되었다. 1995년-
2000년 기간에 행해진 연구개발은 두 가지 영역으로 분류된다. (1) 국제 표준화된 이동
성을 갖춘 2세대 고속 디지털 셀룰러 시스템과(2) 국제 표준화된 이동성이 약한 광대역
이동접속 지스템이 그것이다.

첫 번째 영역에서는 IMT-20000] 표준이 되었다. IMT-2000L 고이동성 환경에서

10



===== PAGE 21 =====
SEE                                                           7                           Other mobile
communication

base station

ae.

2 Mbps     { :   | E  ~
multimedia teminal

64~384 Kbps ~8 Kbps              64, 128, and 384 Kbps
PDAterminal mobileterminal multimedia terminal

terete.

를 그림 1.2 = IMT-2000

다. 그림 1.2는 IMT-20000] 대한 개념을 보여주는 그림이다.
CDMA® 기반으로 한 641-2000에서는 3가지 AS 개념들이 표준화되었다.
(1) directsequence CDMA (DSCDMA/)-frequency division duplex (FDD)
(DSCDMA-FDD), (2) multicarrier CDMA (MCCDMA)-FDD (MCCDMA-FDD), 그
리고 (3) direct-sequence CDMA (DSCDMA)+ime division duplex (TDD) (DSCDMA
-TDD). NTT Docomo} Ericsson¢|] 의한 WCDMA $} Qualcomm] 의한 CDMA2000
이 ITU] 제출되었다. 그들의 기본 요구조건들이 ¥ 1.5에 정리되어 Bch. IMT-2000<
코드 전송률(0410 rate)-S 수정하여 국제 로밍이 가능토록 하는 CDMA 기반 시스템을
채택하였다.
게다가 3세대 이동통신 시스템의 데이터 전송률144 6282 54628)이 2세대 시스템
의 전송률(64 Kbps) 보다 훨씬 크기 때문에 사용자들은 음성뿐만 아니라 동영상 기반
통신과 데이터 통신을 이동 단말기를 통해 실현할 수 있게 되었다.
다수의 고속 이동접속 시스템이 표준화되었다 [14]. 이들 시스템의 기본 조건들이
표 1.6] 정리되어 있다. 그림 1.3은 고속 무선접속 AAS 개념도를 보여준다. 표 1.6

11


===== PAGE 22 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

1 1.58 IMT-2000 정리
WCDMA                                         CDMA2000
주파수       2-GHz band                    ©
ae                  1.25/5/10/20-MHz (DSCDMA)                         1.25/5/10/20-MHz (DSCDMA)
2                                                                                                    3.75/5-MHz (MCCDMA)
Sins                 3.84-Mcps (DSCDMA-FDD, DSCDMA-TDD) | 3.84-Mcps (DSCDMA-FDD)
ited                                                                                      3.6864-Mcps (MCCDMA-FDD)
144-Kbps (고이동성 환경)                       @

384-Kbps (저-이동성 환경)
2-Mbps (정적 환경)

8          비동기                                             비동기적 동기 DSCDMA-TDD)
자라온 21 중기 | oo                                                     동기 (MCCDMA-FDD)
교환                    GSM 네트워크                                             ANSF41

《표 1.68 광대역 이동접속 시스템들의 ise

1666602.11 2 GHz      IEEE802.11 5       HiperLAN2          MMAC
GHz
Pee:    2.40-2.4835 GHz             5.150-5.350 GHz       5.150-5.350 GHz       5.150-5.25 GHz
a8                                           5.725-5.825 GHz       5.470-5.725 GHz
ag        CDM                               OFDM                      OFDM                       OFDM
aay        (DBPSK/DQPSK/CCK) | (BPSK/QPSK/16- | (BPSK/QPSK/16- | (BPSK/QPSK/16-
:                                                   QAM/64-QAM)         QAM/64-QAM)          QAM/64-QAM)
채널         CSMA/CA                          CSMA/CA                  Scheduled TDMA | DSA
접속
이중        TDD                                TDD                         TDD                          TDD
전신
1,2 Mbps, DBSK,             6,9 Mbps BPSK        6,9 Mbps BPSK         6,9 Mbps BPSK

데이터     DQSK, 5.5,11 Mbps          12,18 Mbps QPSK_ | 12,18 Mbps QPSK | 12,18 Mbps QPSK
aes     (CCK)                              24,36 Mbps 16-| 27,36 Mbps 16-| 27,36 Mbps 16

QAM                        QAM                         QAM

54 Mbps 64-QAM_ | 54 Mbps 64.QAM       54 Mbps 64-QAM
기관        18808                                IEEE                        ETSI                          ARIB

BRAN                       MMAC

12



===== PAGE 23 =====
개념을 사용함으로써

Office

“                 Wace
Audio SHF and
other band

니
PC, WS 4/ %

그 e%

Millimeter 4. ~156 Mbps

wave     ~   은

eet et

20~30 Mbps

5 GHz band 4
‘oe:

를 그림 13

에 언급된 바와 같이 대부분의 표준화된 시스템들이 10 Mbps 이상의 전송 속도
하였다. 5 GHz 주파수 대역에서 직교 주파수 분할 다중 (OFDM) 기반 고속
시스템은 초당 수십 메가비트 00088618)의 SES 구현할 수 있다. 이러한 이동접
초당 수십 메가비트 의 광대역 데이터 전송률이 유선 네트워크
만 아니라 무선통신 네트위크에서도 가능하게 되었다.

초당 수십 메가비트에서 수백 메가비트의 데이터 전송속도를 구현할 수 있

Optical fiber network

SHF and other band

Base
station

Note PC, PDA
Mobile video telephone

ce

고속 무선 접속 시스템의 개념도

Jp

rr

00
iad

8 + a

무선접

Fg

rN
a
hy

13


===== PAGE 24 =====
최신 이동통신시스템

14

Mobile Communications using MATLAB Simulation

무선접속 시스템들이 새로운 연구개발의 목적이다.

유럽의 Advanced Communication Technologies and Services (ACTS) 프로그램 내
에는 네 가지 European Union-funded R&D £24) E 7} 진행되고 있는데 Magic Wand
[wireless ATM (WATM) network demonstration], ATM _ wireless access
communication system (AWACS), system for advanced mobile broadband
applications (SAMBA), 그리고 멀티미디어 응용 (MEDIAN) 위한 무선 광대역
customer premises local area network (CPN/LAN)°] 그것이다 [14-231.

미국에서는 Bell 연구소의 두 주요 프로젝트들과 Fy] seamless wireless network
(SWAN)=} broadband adaptive homing ATM architecture (BAHAMA) 그리고
WATM network (WATMnet)°] 미국의 Nippon Electric Company (NEC) computer
and communication (C&C) 연구소에서 개발되고 있다 [15-191.

일본 우정국의 communication Research Laboratory (CRL)= 광대역 이동통신 시스
템의 개발로 분주했는데 이 시스템은 10 Mbps 채널 비트 레이트를 갖는 9406 high
frequency (SHF) 대역 (3~10 012)에서 운용되었고, 80 km/hr 차량속도의 교이동성
환경에서 5 Mbps 전송이 가능했다 [25, 26].

게다가 155 Mbps2] 목표 비트 레이트를 갖는 밀리미터 파장 대역의 실내 고속 무선
LAN 또한 연구되었고 [27, 28], 156 54678의 전송률을 ZH= pointtomultipoint 무선
LANO] reservation-based slotted idle signal multiple access (RS-ISMA)°] 2H= 프로토
콜을 이용하여 개발되었다.

고이동성 환경에서 초당 수2ㅁ688618에서 10 Mbps2] 광대역 전송 능력을 필요로 하
는 이동통신 시스템의 대표적인 a] = intelligent transport system (ITS)7} 있다 [30-341.

118에는 다수의 통신 계획이 존재하는데 GPS7} 가장 유명한 응용 예이다. 그러나 최
근에는 060108[660 shortrange communication (DSRC) 시스템의 표준화가 진행되고 있
다. DSRC 시스템은 단거리 (약 302까지)의 vehicletotoadside 통신 시스템을 구현하
기 a} industrial, scientific, medical (ISM) 대역 (5.725-5.875 GHz)-& 사용한다. 그림
1.4-1.6은 각각 DSRC 시스템의 구성도와 응용 그리고 스펙트럼 할당을 보여준다. [311.

DSRCS 구현하기 위해 유럽의 Comité Européen de Normalisation (CEN), 북미의



===== PAGE 25 =====
ITS information and

communication platform
{infrastructure of
information and communication)

satellite portable
telephone, MCA

Roadside on me   Roadside Dene |
(                             (optical fiber)

optical fiber)

 Portable telephone,

ITS information

FM multibroadcasting,
terrestrial digital broadcasting,
\. Satellite broadcasting

Track (for
distribution)

Bus/taxi (for public           Walker
transportation)

를 그림 1.4 DSRC 시스템의 이미지

American Society for Testing and Materials (ASTM)>} IEEE 그리고 일본의 ARIBO}
DSRCS 위한 표준화 HUBS 구성하였다. 데이터 ASS 위해서 Intemational
Telecommunication Union-Radiocommunication (ITU-R) 권고안 M.14532 active}
backscatter 두 가지 방식을 제안하고 있다 [31]. 요구사항은 ¥ 1.7에 보였다. 권고안에
기반하여 몇 가지 응용 안이 고려되구 있다.

$21.78 Hse 0680 시스템
Active                                          Backscatter
기관                          ARIB                              CEN
10 MHz                            is                 중간 데이터 ASS
10.7 MHz (고속 데이터 전송률)
:                            8MHz 이하                    5 MHz (#21 데이터 전송률)
허용 점유 대역폭                   소    Sk
10 MHz (고속 데이터 전송률)
변조방식                        ASK (UL/DL)                     ASK (DL) / PSK (UL)
데이터 부호화             Manchester 코드               FMO (DL) / NRZI (UL)

DL: downlink; UL: uplink

15


===== PAGE 26 =====
최신 이동통신시스템

16

Mobile Communications using MATLAB Simulation

Security        Credit          Bank
office           company Postbank

-  1                                       =       [
Convenience stores                                    i         i                          ‘
Drive-through shops                                                                                            "
Gas station
Traffic info.       ;                               고
Local info.                  >                                         호

Info. for siden

ma)

Automatic check-in

Information shower

eee
Parking

를 그림 1.5 DSRC 시스템의 응용

Frequency                              5,800                                         5.900
(매가
5.725                    ISM band                    5.875
ITU-R                                                          :

Europe
North                                                           5.825
pea

ed a                                         Canada only
Japan

를 그림 1.6 DSRC NAGS 위한 스펙트럼 할당

그림 1.5는 몇 가지 응용 예를 보여준다. 또한 완전이동성 통신 시스템과 준이동통
신 시스템도 고려되고 있다. 본 장의 초기에 언급한 바와 같이 이동통신에 사용되는 접
속 프로토콜뿐만 아니라 많은 변복조 계략도 다수가 존재한다. 그림 1.7은 1, 2, 3세대
이동통신 시스템과 고속, 초고속 무선접속 시스템과 178 간의 관계도이다.

때때로 새로운 시스템의 성능을 예전 시스템의 것과 동일한 환경에서 비교한다. 컴퓨
터 시뮬레이션은 동일 환경에서 서로 다른 시스템들의 성능을 평가하기 위해 사용되는
방법 중 하나이다.



===== PAGE 27 =====
16
101 ~
eae
ㅣ
|
6.             IMT-2000     ITS
= |                       (DSRC)
& |
prs
ZUVnl s|s     )
=   ~ 고   =
은   i] o |] 호
wax   1   o   o
= Hileia                      a
고 titslsi es
= eae )존                   Uitra-
내           떡    High-speed wireless     아너
|                              S           access system                      에
|           2                    access
|           a                    system
ㅣ
ㅣ
RF 112 10               7            =
1k      10k    100k    1M     10M     100M 1G
Supported bit rate (bps)
를 그림 17 이동통신 시스템의 분류

우후 | 이동통신시스템의 시뮬레이션 평가를 위한 모델의 분류

몇몇 무선통신 시스템의 성능은 시제품을 개발하여 필드 테스트를 하는 대신 컴퓨터
시뮬레이션을 통해 평가될 수 있다. 이 AS 디지털 무선통신 시스템의 평가에 집중한
다. 디지털 이동통신 시스템의 전형적 모델들은 다음 세 가지로 분류된다. (1) 지점 대

A\A (point-to-point) 통신 (2) 지점 대 다중지점 (pointtomultipoint) 통신 (3) 다중지점
대 U+S2)4 (multipointtomultipoint) 통신. 1.21-1.2.3은 이들 3가지 Bao] 대해 다
룬다.

1.2.1 지점 대 지점 통신

그림 1.8은 지점 대 지점 통신의 개념을 보여 준다 [35]. 지점 대 지점 통신에서 정보
데이터는 먼저 소스 부호기에 입력된다. 정보 데이터가 아날로그라면 이 부호기에서 디

17


===== PAGE 28 =====
 ~) 최신 이동통신시스템
C

Mobile Communications using MATLAB Sinuiatan

지털화 된다. 디지털화된 데이터의 부피가 크다면 데이터는 B 가지 부호화 기법 중 하
나에 의해 압축된다. Motion Picture Experts Group (MPEG)¥} adaptive differential
code modulation (ADPCM)-<- 동영상과 음성-정보 데이터를 위한 부호화 기법의 IS
이다.

소스 부호화된 디지털 데이터는 가혹한 무선 통신 채널에서 비트 에러 발생을 줄이기
위해 채널 Boj 입력된다 a seis     코드나 BoseChaudhuri-Hocquenghem
(BCH) 코드 혹은 660-90100001 코드 등의 오류 정정 코드 (80ㅇ)와 파일 데이터 삽
입 기법 그리고 무선 전파 특성을 추정하기 위한 프레임 생성들이 대표적인 예들이다.

다음으로 채널 부호화된 디지털 데이터는 디지털 변조기에 입력되고 무선주파수 신
호로 변환된다. AZ 의미는 반송 신호 파형에 포함된 고유 성분을 변화시키는 것을
말한다. 반송 신호는 일반적으로 다음과 같이 쓰여 진다.

S(t) = A(t)exp(2af,t + A(t)                            (1.1)

여기서, A(t), /, 그리고 O(t)S 44 A AS, 무선 반송 주파수 그리고 반송 파
형 신호의 시변 위상이다. 식 (1.1)에는사용자가 값을 변화시킬 수 있는 세 가지 고유 성
분이 존재하는데 이는 진폭, 주파수 그리고 위상이다. 디지털 정보 데이터에 따라 식
(1.1)의 진폭을 변화시키면 진폭 변조 (AM), 주파수를 변화시키면 주파수 변조 (FM),
위상을 변화시키면 위상 변조 (PM)z} 불린다. 변조된 ASS 그림 1.9에 보였다.

밴조 태1 반송 무선 주파수 (RF) 대역뿐만 아니라 낮은 주파수 대역에서도 수행
된다. 어떤 경우에는 디지털 신호 처리가 가능한 매우 낮은 주파수 대역을 사용하기도
한다. 이 주파수 대역이 기저대역이라 불린다. 기저대역이 사용되면 변조 신호를 만들
기 위해 반송 RF 대역으로의 상위변환이 필요하다. 직접적인 변환이 어려운 경우에는
먼저 중간 주파수 (IF) 대역으로 변환한다. 그 후 디지털 변조 신호는 무선주파수 채널
을 통해 수신기에 전송된다.

수신기에서는, 수신된 ASE 디지털 복조기에 입력되고 기저대역 디지털 데이터로
하위 변환된다. ABS 위해서 반송 주파수 대역의 수신 신호가 때 대역으로 변환되고

18



===== PAGE 29 =====
이 신호가 다시 기적대역으로 변환되는 방식이 일반적이다. 그 후 기저대역에서 진폭,
주파수 혹은 위상의 레벨이 각각 AM, FM 그리고 PM 방식에 따라 검출되고 최종적으
로 전송된 디지털 데이터가 복원된다.

다음으로 검출된 디지털 데이터는 채널 복호기에 입력되고 무선 채널에 의해 야기된
다양한 진폭과 위상들이 보상되어 송신기에서 사용된 806가 복호된다. 최종적으로 채
널 복호화된 데이터는 소스 복호기에 입력되고 ase 정보가 복원된다.

이 AS 그럼 1.8에 보인 BAS 고려한다. 그림 1.8에서 음영이 있는 영역의 자세한
내용이 그림 1.10에 나타나 있는데 다음 요소들이 평가되었다.

『비트 오류율 (865)

프레임 오류율 (『6)
패킷 오류율

Transmitter
Input data   »| Source      Channel |] Digital
generator   :  encoder      encoder    | modulator
A
Communication
channel
Receiver          :
Received     Source      Channel |.   Digital     :
data            decoder         decoder | . | demodulator

이 값들은 다음 매개변수들을 변화시켜 평가되었다.

를 그림 1.8 지점 대 지점 통신

19


===== PAGE 30 =====
Zy 최신 이동통신시스템
C               ‘                 A

Mobile Communications using MATLAB Simufation

*페이딩 환경 (ol, 도플러 주파수의 레벨)
az 신호의 레벨

orf" Nw SS

> Amplitude
modulation

(AM)
YL NM A re

modulation

」                               Bi                                   (FM)            1-7
0 i>  Modulator  >                 0                               Ht

| | | | |               3fo | 4fo |2fo | fo |3fo | 2fo
T: Symbol transmission time                                  ™

on

Phase            0                                         t

ae   x 02122 0 | x 272

를 그림 1.9 HA 신호의 Of

몇몇 경우, 그림 1.10에 보인 시뮬레이션 된 디지털 무선통신 시스템으로는 87 대역

북조 기획을 모의실험하기 어렵다. 이는 RF 대역에서의 변조 신호를 표현하

기 위해서는 많은 샘플링 데이터가 필요하기 때문이다. 변조된 신호는 기저대역 주파수
부분과 8 대역 부분에서 다음과 같이 분리된다.

S(t) = A(t) exp(A(t)) x exp(27f,t)                         (1.2)

BE 블럭에서 87 대역 부분을 AAS 수 있고 그림 1.109] BE 구성 블록들을 기저
대역에 기반 한 표현식으로 기술하고 컴퓨터 시뮬레이션에 의해 평가를 수행할 수 있
다. 이런 형태의 시뮬레이션은 등가 저역통과 시스템 하의 시뮬레이션이라고 한다. RF
대역 시스템과 등가 저역통과 시스템 사이의 관계 또한 그림 1.10에 나타나 있다. 등가
저역통과 시스템 하의 컴퓨터 시뮬레이션을 사용하여 지점 대 지점 통신 하에서의 몇몇
데이터 전송 성능을 쉽게 평가할 수 있다.

20



===== PAGE 31 =====
4  Baseband    ee

digtal      6.
4 modulator |

Remove radio
fr   Bs          y part

Communication
channel

io bef RF band
_ {upconverter

_ | converter

를 그림 1.10 이 책의 목표 영역

마지막으로 888, FER 그리고 28#과 같은 몇몇 평가 항들을 얻기 위한 대표적인 흐
름도가 그림 1.10에 표현되어 있다. 일단 랜덤 디지털 정보 데이터가 입력 데이터 생성
기에서 생성된다. 필요하면 이 데이터가 채널 부호기에서 패킷이나 프레임으로 형식화
된다. 다음으로 형식화된 데이터가 기저대역 디지털 변조기에서 변조된다. 그 후 기저
대역 변조 신호가 등가 저역통과 모델에 의해 기술된 무선채널 블록으로 입력된다. 수
신기 블록에서 등가 저역통과 시스템에 의해 표현된 전송 신호는  ee, 디지털 복.
기에서 복조되고 전송 디지털 데이터, 프레임 혹은 패킷이 채널 복호기 블록에서 복원
된다. 최종적으로 복조된 데이터, 프레임 혹은 패킷이 전송된 그것과 비교되고 88,
FER 혹은 28#이 얻어진다.

1.2.2 지점 대 다지점 통신

그림 1.11에 지점 대 다지점 통신의 영상을 보였다. 지점 대 다지점 통신에서 하나의
액세스 포인트 (&0)는 다수의 사용자 단말기 (01)와 통신한다. 일단 사용자는 그들의
정보 데이터를 특정 프로토콜을 사용하여 보낸다. 프로토콜은 APS} 다수의 UTZ] 정
의되어있다. 어떤 경우에는 여러 UTE SE] 온 정보 데이터 Apolo] 충돌이 일어나기도

21


===== PAGE 32 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

한다. 이 충돌을 검출하고 충돌의 수를 세서 전송 데이터의 처리량을 모의실험 한다. 또
한 로부터의 정보 데이터를 전송하는데 걸리는 평균 지연시간도 모의실험 한다.

Access point (AP)

Communication area

Magi 지점 대 다지점 통신

그러나 데이터 충돌이 일어나더라도 수신 신호 레벨들의 차이는 크다. 이런 경우 4『
는 가장 큰 신호 레벨을 가진 데이터를 받는다. 이를 포착효과(68006 effect)z} 부른다
[1]. 여러 간섭 신호 레벨과 888, FER 혹은 PERS] 평가를 위한 데이터가 준비하면 |
착효과 환경 하의 보다 정확한 처리량과 평균 지연시간을 실험할 수 있다.

위에서 살펴본 바와 같이, 이 책에서는 지점 대 다지점 통신에서 다음 항들과 같은 평
가를 주로 다루게 된다.

처리량
eam 지연시간

이 값들은 다음 변수들을 변화시켜 평가된다.

22



===== PAGE 33 =====
= UTS] 수

『제공된 트래픽의 부피
버
=

※포착효과의 레벨

대표적인 흐름도를 그림 1.12에 보였다. 제일 먼저, 각 단말기에서의 데이터 생성 모
del 트래픽 모델, APS] 위치, 01들의 위치 그리고 들의 수가 결정된다. 그리고 프
로그램된 액세스 프로토콜에 하에서 전송 패킷이 APo] 성공적으로 전송되었는지의 여
부에 따라 처리량과 평균 전송지연을 평가한다.

Traffic model                    ¢ Position of access point
¢ Poisson arrival               ¢ Position of user terminal
¢ Number of user terminals

Modeling of communication channel
Wired communication

¢ Ideal communication channe!
Wireless communication

¢ Propagation loss

¢ Shadowing

|                   Access protocol               은아

Packet transmission   | New age)

or retransmission

Decision whether                         Information of

the transmission                             modulation and
packet is successfully                      demodulation schemes
transmitted or not                         (CIR vs. BER, FER, PER)

Failure

Success

|  Measurement of transmission delay

Number of successfully
transmitted packets reaches
required number in the
simulation

The simulation is finished

|  Throughput and transmission delay  |

를 그림 1.12 지점 대 다지점 통신에서 전송 능력을 얻기 위

rol
lok
on
대

23


===== PAGE 34 =====
최신 이동통신시스템

A

24

Mobite Communications using MATLAB Simufation

1.2.3 다지점 대 다지점 통신

그림 1.13은 다지점 대 다지점 통신의 개요도를 보여준다. 다지점 대 다지점 통신에
서는 다수의 APS} 07가 설치되고, 새로운 평가 항으로 호출 저지 (callblocking) 확률
이 평가된다.

호출 저지는 그림 1.13에서 나타낸 셀룰러 " 스템에서 발생한다. 이런 셀룰러 시스템
에서 하나의 셀룰러 영역에서 사용되는 주파수들은 다른 셀룰러 영역에서 다시 사용된
다. 하나의 주파수 대역을 사용함으로써 특정 셀룰러 영역에 위치하는 01에 의해 생성
된 전송 신호가 다른 셀룰러 영역에 존재하는 APS 간섭하는 경우가 존재한다. 호출 저
지를 일으키는 간섭 레벨은 상당히 크다. 다지점 대 다지점 통신의 시뮬레이션 모델을
만들어 호출 저지 확률을 평가할 수 있다.

Interference         chi                ‘i point (AP}

if  User terminal (UT)

Call blocking
occurs

Mid 1.13 다지점 대 다지점 통신

이 확률을 검토하기 위한 대표적 흐름도를 그럼 1.14에 제시한다. 먼저 UTS APS]
위치, UTS 수 그리고 셀룰러 영역의 크기가 결정된다. 동시에 트래픽 모델, 각 단말기
의 데이터 생성 모델이 정의된다.

그 다음에, 주파수 할당 기법과 같은 프로그램된 자원 관리 기법에 하에 특정 셀룰러
영역이 구성되고 원하는 신호 레벨과 그렇지 않은 신호 레벨 간의 비가 모든 4『에서 측
정된다. 이 비는 APS 의 위치, AS ASS] 파워, 안테나의 이득과 패턴 그리고 et



===== PAGE 35 =====
Start

Preparation,
status initialization

Time loop

ㅣ

Finishing call is terminated

Connected call is checked,
if necessary, reallocation

|

New call arrival and
channel assignment

|
Calculation of antenna
gain at access points and
user terminals
|
Calculation of CIR
at each access point

|

IVY

Time loop   ue
|
Output data    ee
0 그림 1.14 다지점 대 다지점 통신에서의 전송 성능을 얻기 위한 SES

테나의 높이와 같은  ee ee
함으로써 호출 저지가 발생할지 결정할 수 있고 최종적으로는 호출 저지 확률을 얻을

수 있다.
이 장의 초기에 밝힌 바와 같이 이 책은 독자로 하여금 컴퓨터 시뮬레이션

Lu

1g 통한 지

25



===== PAGE 36 =====
2) 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

점 대 지점, 지점 대 다지점, 다지점 대 다지점 통신에서의 AS 성능 평가에 대한 이해
를 FES 할 것이다.

1.3 ? 척의 가설

26

이 책은 8개의 장으로 구성되어 있으며, 컴퓨터 시뮬레이션을 활용한 디지털 이동통
신의 전송 성능을 평가하기 위한 모든 필요 요소들을 다룬다. 각 장의 부록과 더불어 책
과 함께 제공되는 CDROMS] 시뮬레이션 프로그램들을 제시하고 있다.

2장에서는 컴퓨터 시뮬레이션을 수행하기 위한 몇 가지 주요 변수에 대해 기술한다.
통신용 범용 시뮬레이션 툴인 MATLABO] 이 책의 주요 SLA 사용된다. 이 때문에 2
장에서는 MATLAB 의 사용법을 우선 기술한다. 다음으로 2.1장은 자주 사용되는 명령
어와 함수들 그리고 ASA 프로그램을 위한 방법들을 정리한다. 또한 모든 통신 시스
템을 평가하기 위해 공통적으로 사용되는 함수를 프로그래밍하기 위한 기법들을 설명
하는데 여기에는 데이터 생성 블록, 레일리 페이딩 (Rayleigh-fading) 채널 블록 그리고
additive white gaussian noise (AWGN) 채널 블록이 해당한다.

3장은 위상 변위 방식 (PSK) 기반한 디지털 무선 전송 AAS] 기본 구성에 대해 설
명하고 AWGN3} 다중경로 레일리 페이덩 채널 환경 하에서 컴퓨터 시뮬레이션을 이용
해 전송 성능을 평가하기 위한 방법을 기술한다. HS C= PSK 기반 디지털 무선 전송
u}4]=-binary PSK (BPSK), quadrature PSK (QPSK), offset QPSK (OQPSK),
minimum shift keying (MSK), gaussian-filtered MSK (GMSK) 그리고 quadrature AM
(QAM)-S 소개하고 컴퓨터 시뮬레이션 프로그램을 통해 그들의 성능을 평가한다.

4장에서는 OFDM 전송 방식의 구성을 제시하는데, 이 방식은 다중경로 페이팅의 간
AS 줄이고 높은 주파수 이용 효율을 유지하면서 광대역 통신을 구현할 수 있다. 또한
4장은 AWGN3} 다중경로 레일리 페이덩 채널 환경 하에서의 AS 성능을 모의실험하
기 위한 방법을 기술한다. 이 성능들은 프로그램된 컴퓨터 시뮬레이션을 통해 구현되고
평가된다.

54 CDMAS] 구성에 대해 제시한다. 다중경로 페이덩과 같은 열악한 전송채널 환



===== PAGE 37 =====
경 하에서도 전송품질이 유지되는 CDMAE 3세대 이동통신 시스템에서 사용된다. 5
장은 또한 AWGN} 다중경로 레일리 페이덩 채널 환경 하에서의 AS 성능을 모의실
험하기 위한 WHS 기술한다. 이러한 전송성능은 MATLABE S19 소스를 이용한
컴퓨터 시뮬레이션을 통해서 구현되고 평가된다.

6장에서는 컴퓨터 시뮬레이션을 통해 다중접속 프로토콜을 가진 지점 대 다지점 통
신 시스템에서의 전송 BSS 평가하는데, 이를 위해 pure ALOHA, slotted ALOHA,
nonpersistent carrier sense multiple access (CSMA) 그리고 9100660 nonpersistent
inhibit sense multiple access (ISMA)2} 같은 다중 접속 프로토콜들을 예로 들어 설명
한다. 6장은 또한 처리량과 평균 지연 ALES 모의실험하기 위한 방법도 기술하는데,
그 성능들은 MATALBE S18 소스에 의한 컴퓨터 시뮬레이션을 통해 평가된다.

7장에서는 셀룰러 원격통신 시스템에 기초한 다지점 대 다지점 통신 시스템의 기본
적인 시뮬레이션 기법을 기술한다. 7장에서는 또한 dynamic channel assignment
(DCA) 312], fixed-channel assignment (FCA) 알고리즘 그리고 적응 안테나를 이
용한 4000016 cellular zone configuration (AZC) 알고리즘에 대해 소개한다. 다음으로
호출 저지 FSS 모의실험하기 위한 기법에 대해 논하는데, 이들 성능 역시 MATALB
프로그램 소스에 이한 컴퓨터 시뮬레이션을 통해 평가된다.

8장에서는 이 책에서 공부한 소프트웨어 프로그래밍 SASS 이용하여 디지털 하
드웨어상태로 응용하는 소프트웨어 무선 |4l(Software Radio Communication) 시스
템에 대해 기술한다. 최근에는 프로그래밍 기반의 디지털하드웨어 기술의 발달에 힘입
어 너411Ｌ40이나 (:언어와 같은 프로그래밍언어소스를 이용하여 이동통신 단말기.등
을 위한 하드웨어의 ASHES digital signal processor (DSP), 1610 ㅠㅁ081807107181016

gate array (FPGA) &< application-specific integrated circuit (ASIC)7|=2} 같은
digital signal processing hardware (DSPH)= 구현이 가능해졌다. 이러한 관점에서 8
장에서 소개하는 소프트웨어 무선 통신은 7장까지 FSB OA 프로그래밍기법들을
실제로 하드웨어적인 응용분아로 확대시켜서 이동통신용 디지털 하드웨어까지도 구
현할 수 있는 지식의 EQS 제시해주고 있다.

또한 8장에서는 소프트웨어 무선 통신의 장점과 앞으로 해결해야할 과제들에 대해

27


===== PAGE 38 =====
21 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

서도 논하고 소프트웨어 무선통신 시스템을 구현하기 위해 개발된 주목할 만한 기술들
에 대해 설명한다. 게다가 2000년까지 발표된 논문에서의 최근의 소프트웨어 무선통신
프로젝트들의 개요를 살펴보고 몇 가지 소프트웨어 무선통신 기반 통신 시스템의 응용
에 대해 설명한다.

28



===== PAGE 39 =====
1) Prasad, R., Universal Wireless Personal Communications, Norwood, MA: Artech House, 1996.
2) Dunlop, U. E., Marconi-The Man and His Wireless, New York: The Macmillan Company, 1937.
3) Jolly, W. P., Marconi, London: Custable, 1972.

4) Jakes, W. C., Microwave Mobile Communications, New York: IEEE Press, 1994.

5) Sampei, S., Applications of Digital Wireless Technologies to Global Wireless
Communications, Upper Saddle River, NJ: Prentice Hall, 1997.

6) Calhoun, G., Digital Cellular Radio, Norwood, MA: Artech House, 1988.

7) Cox, D. C., “Wireless Network Access for Personal Communication,” IEEE Comm. Mag.,
Vol.30, December 1992, pp.96-115.

8) Padgett, J. E., C. G. Gunther, and T. Hattori, “Overview of Wireless Personal
Communications,” IEEE Comm. Mag., Vol.33, January 1995, pp.28-41.

9) Kinoshita, K., M. Kuramoto, and N. Nakajima, “Development of a TDMA Digital Cellular
System Based on Japanese Standards,” Pre. IEEE VTC’91, 1991, pp.642-645.

10) Tuttlebee, W. H. W. (ed.), Cordless Telecommunications in Europe, Berlin: Spinger Verlag,
1990.

11) Tuttlebee, W. H. W., “Cordless Personal Communications,” IEEE Comm. Mag., Vol.30,
December 1992, pp.42-62.

12) Prasad, R., CDMA for Wireless Personal Communications, Norwood, MA: Artech House,
1996.

13) Ojanpera, T., and R. Prasad, Wideband CDMA for Third-Generation Mobile Communications,
Norwwod, MA: Artech House, 1998.

14) van Nee, R., and R. Prasad, OFDM for Wireless Multimedia Communications, Norwood, MA:
Artech House, 2000.

15) Prasad, R., “Wireless Broadband Communications Systems,” IEEE Comm. Mag., Vol.35,
January 1997, p.18.

16) Honcharenko, W., et al., “Broadband Wireless Access,” IEEE Comm. Mag., Vol.35, January
1997, pp.20-26.

17) Correia, L. M., and R. Prasad, “An Overview of Wireless Broadband Communications,” IEEE
Comm. Mag., Vol.35, January 1997, pp.28-33.

29


===== PAGE 40 =====
최신 이동통신시스템

        Mobile Communications using MATLAB Simulation

18) Morinaga, N., M. Nakagawa, and R. Kohno, “New Concepts and Technologies for Achieving
Highly Reliable and High-Capacity Multimedia Wireless Communications Systems,” IEEE
Comm. Mag., Vol.35, January 1997, pp.34-40.

19) da Silva, J. S., et al., “Mobile and Personal Communications: ACTS and Beyond,” Proc. IEEE
PIMRC’97, September 1997.

20) Prisoli, F. D., and R. Velt, “Design of Medium Access Control and Logical Link Control
Functions for ATM Support in the MEDIAN System,” Proc. ACTS Mobile Comm. Summit’97,
October 1997, pp.734-744.

21) Rheinschmitt, R., A. de Haz, and M. Umehinc, “AWACS MAC and LLC Functionality,” Proc.
ACTS Mobile Comm. Summit’97, October 1997, pp.745-750.

22) Aldid, J., et al., “Magic into Reality, Building the WAND Modem,” Proc. ACTS Mobile Comm.
Summit’97, October 1997, pp.734-744.

23) Mikkonen, J., et al., “Emerging Wireless Broadband Networks,” IEEE Comm. Mag., February

1988, pp.112-117.

24) Hase, Y., et al., “R&D Project on Broadband Mobile Communications Using Microwave Band,”
Proc. MDMC’96, July 1996, pp.158-162.

25) Harada, H., and M. Fujise, “Experimental Performance Analysis of OCDM Radio Transmission
System Based on Cyclic Modified M-Sequences for Future Intelligent Transport Systems,”
Proc. IEEE VTC’99 Fall, September 1999, pp.764-767.

26) Harada, H., and M. Fujise, “Field Experiments of a High Mobility and Broadband Mobile
Communication System Based on a New Multicode Transmission Scheme for Future
Intelligent Transport Systems,” Proc. IEEE VTC’2000 Spring, May 1999.

27) Wu, G., et al., “A Wireless ATM-Oriented MAC Protocol for High-Speed Wireless LAN,” Proc.
IEEE PIMRC’97, September 1997, pp.198-203.

28) Wu, G., Y. Hase, and M. Inoue, “An ATM-Based Indoor Milimeter-Wave Wireless LAN for
Multimedia Transmissions” IEICE Trans. Commun., Vol. E83-B, No.8, August 2000, pp.1740-
1252.

29) Wu, G., K. Mukumoto, and A. Fukuda, “Analysis of an Integrated Voice and Data Transmission
System Using Packet Reservation Multiple Access,” IEEE Trans. Veh. Technol., Vol.43, No.2,
May 1994, pp.289-297.

30) Najarian, P. B., “Status Update on ITS Activities in the U.S. and ITS America,” Proc. ITST2000,
October 2000, pp.7-11.

31) Ohyama, S., K. Tachikawa, and M. Sato, “DSRC Standards and ETC Systems Development in
Japan,” Proc. 7th World Congress on Intelligent Transport Systems, Torino, Italy, November
2000.

30


===== PAGE 41 =====
32) Kim, J. M., “ITS Research and Development Activities at ETRI, Korea,” Proc. ITST2000,
October 2000, pp.13-18.

33) Armstrong, L., “New DSRC Standards Under Development for North America,” Proc. 7th
World Congress on Intelligent Transport Systems, Torino, Italy, November 2000.

34) Rokitansky, C., C. Becker, and A. Feld, “DSRC Standardization and Conformance Testing of
DSRC/EFC Equipment,” Proc. 7th World Congress on Intelligent Transport Systems, Torino,
Italy, November 2000.

35) Proakis, J. G., Digital Communications, #rd ed., New York: McGraw-Hill, 1995.

31



===== PAGE 42 =====
See

—



===== PAGE 43 =====
21 1,

MATLAB2I
시뮬레이션 SHAQ 기초적 사용법

이 장에서는 컴퓨터 시뮬레이션을 통해 이동통신 시스템의 전송 성능을 용이하게 평
가하기 위해 필요한 몇 가지 주요 주제들에 대해 논의한다. 본 책은 주로 훌륭한 시뮬레
이션 소프트웨어인 MATLABS 이용한다. 이런 이유로 먼저 2.2장에서는 이 책에서 자
주 사용되는 명령어들을 설명함으로써 MATLAB 사용법에 대한 기본적인 지침을 소
개한다. 또한 이동통신의 연구 및 개발에 있어서 폭넓게 공통적으로 사용되는 필수적인
aS S MATLAB 시뮬레이션 프로그램을 통해 정의한다. 2.3장은 MATLAB 프로그

을 사용한 데이터 생성과 88성능도출의 WAS 설명한다. 2.4장에서는 전송 성능
을 평가하기 위해 사용되는 전형적인 통신 채널에 대해 설명하고 통신 AS 프로그래
밍하기 위한 기법에 대해 기술한다. AWGN 채널과 레일리 페이덩 Ao] 대해서도 a
명된다. 마지막으로 2.5장은 간단한 정리로 이 장을 마무리한다. Appendix 2ㅅ에 본 장
과 관련된 모든 프로그램을 제시하는데 그 내용은 책과 함께 제공되는 0ㅁ2&044에서도
찾아 볼 수 있다.

35


===== PAGE 44 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

| 기본적인 사용법

36

본 책에서는 시뮬레이션을 위해서 MathWorks, Inco] 의해 개발된 컴퓨터 시뮬레
이션용 소프트웨어인 MATLAB[1]-& 사용한다. \ㅅ1Ｌ4ㅅ8이라는 0] matrix
laboratoryS 의미하는데, 일반적으로는 행렬연산을 용이하게 해줌과 동시에 6:언어와
마찬가지로 시뮬레이션 툴로서의 기능도 수행한다. 이 책은 MATLABS 단지 시뮬레
이션용 툴로서 사용하기에, 그 사용법에 대해서는 심도 있게 다루지는 않는다. 보다 자
세한 사용법을 익히려면 MATLAB 지침서[1]를 참고하길 바란다.

2.2.1 벡터와 행렬의 생성

먼저 MATLAB 언어 사용의 용이성을 보여주기 위해 몇 가지 예를 제시한다.
MATLAB 시작하면 작업공간을 보게 될 것이다. 이 작업공간은 명령 줄을 보여준다.

이 명령 So] 직접 명령어를 입력할 수 있다. 몇 개의 벡터와 행렬을 MATLAB 작업
공간에 생성해 보자.

2
1.세개의벡터 w= 1), v= (1 —1 1), s= 7S 만들기 위해, 명령 줄에 다음과 같이 입력하고
4

비슷하게 다음을 입력한다.

oP ive [ab



===== PAGE 45 =====
MATLABS| 시뮬레이션 둘로서의 기초적 사용법 (을

다음과 같이 A|A(setting)st 것이다.

Leon
2,3by3 행렬 A= | 2 1 2) 3 생성하기 위해서는 다음과 같이 입력한다.
Its

>> [2 2 tre, 27) 2 0 시

3. 벡터와 행렬의 2,,와 ㅇ,, 을 교환하는 연산인 전치하기 위해서는 벡터와 행렬의 다음에 “'” 를 입력
하면 된다. \를 전치하기 위해서는 다음과 같이 입력한다.

가가 ad

MATLAB 연산의 결과가 출력된다.

ans =
1
=.
di

AS 전치하기 위해서는 다음과 같이 입력한다.

>> A!
ans =
2      1
2       i       iL
2      2

37


===== PAGE 46 =====
ZY 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation
2.2.2 인텍싱과 서브스크립팅

행렬과 벡터의 하부 항을 얻는 방법을 예를 들어 설명한다. 먼저 다음 행렬을 생성
하자.

m= NH N
= WwW fb

-& > oO
SELB, A 7

>> 865[2 4187.23 4; 1 14}

B=
2    4    8

3    4

1:    1    4

BS] 7행 /열 요소는4471.48에서 2(7, /)로 표현된다. oS So}, 2(2, 3)항
을 얻기 원한다면 다음과 같이 입력한다.
22627 3)

ans =
4

MBNA 72행까지, 2열에서 《4열까지의 항이 필요하면 Bim: 7, 2: 0)과 같이
입력한다. 예를 들어, 1열~2열과 2행~3행까지의 항이 필요하면 다음과 같이 입력한다.
>> 0(Ｌ12.283)
4     8
3
^행에서 7행까지 증가분 a=, 2열에서 0열까지 증가분 로 하부 항을 얻기 위
해서는 2(72: 0: 2, 2: 0: 0)를 실행한다.

>> Bi(is233,42223)

ans: =

38



===== PAGE 47 =====
MATLAB! 시뮬레이션 둘로서의 기초적 se BO

4

myo] 모든 항이나 /열의 모든 항이 필요하면 “:”명령을 이용한다. B(m, :)과
BC, /)와 같이 입력함으로써 각각 mY] 모든 Ys} /모든 항을 얻을 수 있다.
예를 들어, 2 행렬의 3행의 모든 항을 얻기 위해서는 다음과 같이 입력한다.
>> BAS p39

ans =

1       1       4
2 행렬의 2열을 얻기 위해서는 다음과 같이 입력한다.

o> Bt, 2)
ans =

4

3

2.2.3 행렬과 벡터 계산법

이 장에서는 MATLABS 통한 행렬과 벡터의 기본적인 계산법을 소개한다.

(1) 덧셈과 밸셈
행렬의 덧셈과 als 배열에서와 같이 항별로 정의된다. A 행렬과 8 행렬의 덧셈과
lS 다음과 같이 행해진다.

>> X=A+B
x=

39


===== PAGE 48 =====
21  최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

Y=

4

덧셈과 wae 두 행렬이 같은 차원을 가질 때 가능하다. 만약 차원이 다르면 오류가
발생한다.

>> X=Atu

??? Error using ==> +

Matrix dimensions must agree.
>> w=v+s

w=

(2) 벡터 곱과 전치
같은 크기의 행벡터와 열벡터는 곱할 수 있다. 다음은 두 가지 예를 보여준다.

>> xX=Vv*uU
x=
5
>> ASuTV
x=
2    “2     2
=A     1
4    “4     4
(3) 행렬 곱셈

행렬의 Fle 선형 변환의 구성을 반영하고 동시 선형 방정식의 간결한시스템 표현
식이 가능하도록 정의되어 있다. 행렬 곱 0=4*8는 AS] 열의 크기와 BS] 행의 크기가
같거나 둘 중 하나가 스칼라일 때 가능하다. &가ㅁ687이고2가216877이면 그 HCE
m-byno|t}. 다음 두 예는 행렬 곱이 교환가능하지 않음을 보여준다. 즉 4*8와 BALE
보통 같지 않다.

40


===== PAGE 49 =====
MATLABS| 시뮬레이션 툴로서의 기초적 사용법 (OB

>> X=A*B

8    13    28

>> Y=B*A

Y=
18    16    26
12    Id    16
s/     0    Lat

또한, YS] 4 (4, Z=A*A=A’2)2S 다음과 같이 정의된다.

>> Z=A%2
Z =
6     5     나
7
2     5     7

행렬은 오른쪽에 열벡터와, 왼쪽에 행벡터와 곱할 수 있다.

>> x=A*u
x =
8
Ls
itil
>> y=v*B
y=
ds     2     8

(4) 항대항 계산
y* by, 3% by, ay* byl S 얻기 위해서는 “.* ”를 사용하면 된다.

41


===== PAGE 50 =====
Zy 최신 이동통신시스템
tC

Mobile Communications using MATLAB Simulation
>> c=a.*b

c=[a,/b,, a/b, a3/b3,°*, @y/ by) S 얻기 위해서는 다음과 같이 “./*를 사
용하면 된다.

>> c=a./b

또한 ㅇ=[01^01, ax bo, a;"b3,°**, an byl& 얻기 위해서는 Se i 0 사용하면
된다.

>> 0=2.^5ㅁ
다음 두예는 2=[4, 9, 8]와 ㅎ=[4, 3, 4]를 이용하여 위 계산들을 보여준다.

>> a=[4,9,8]

a=
4     9     8
>> b=[4,3,4]
Dy 를
4     3     4
>> 000, =D
c=
16    27    32
>> c=a./b
c=
1     3     2
>> c=a.“b
c=
256         729        4096

이들 AAS 다음 예에서와 같이 행렬에 대해서도 성립한다.

42



===== PAGE 51 =====
MATLABS| 시뮬레이션 둘로서의 기초적 사용법 를

1     L     8
>> C=B./A
Ce
2     2     8
1     6:
a     1
>>. C=A.4B
C=
1    16     E
4     1    16
1     i    16

표 2.1에 MATLAB 산술 연산을 정리하였다.

HH 218 1411Ｌ48의 산술 연산자

+          더하기                                              hes            제곱 승(항대항)
- | 페기                                     (벡터) ' | 전치
= 3          곱하기 (항대항)                                   :              행렬 곱
나누기 (항대항)              행렬 나누기
+    단일 항 플러스              수     행렬 제곱 승
단일 항 마이너스

2.2.4 관계 연산자

MATLAB 표 2.2에 보인 관계 연산자를 지원한다.
이 연산자들은 두 벡터 혹은 행렬의 관계를 결정하는데 각 항들은 관계가 참인 경우
1, 거짓인 경우 0을 갖는다. 다음은 각 관계 연산자들의 효과를 보여준다.

43


===== PAGE 52 =====
\,

최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation

HH 2.28 MATLAB 관계 연산자

<          Less than                                                =         Greater than or equal to
(=         Less than or equal to                              ==        Equal to
>           Greater than                                              ~= | Not equal to

^ Re |e 40.4 7 ey

A=
At    ail    고
1    1    1
자    1    1
eS B= (A 71 10 a 그 714 ee)
B=
1    1    pit
aN    나    자
    pall    1
>> A<B
ans: =
0          0
0     0
1
>> A<=B
ans =
£
0          0
Bl
>> A>B
ans: =
0     0
고
0     ub     0
>> A>=B
ans =
4:     0     A

44



===== PAGE 53 =====
MATLABY| 시뮬레이션 툴로서의 기초적 사용법  10 |

1     at     1
0     il     L
>> A==
ans =
d     0     1
0     0     0
0     0     1
>> A~=B
ans =
0     1     0
1     ai
a     a8     0

2.2.5 논리 연산자

MATLAB 표 2.3의 논리 연산자를 지원한다.

AND 연산자, &는 피연산자 모두가 참일 때 참을 준다. 수식 항에서는

7-00] 아닐 때 참이다. 다음 예는 그 효과를 보여준다.

BE 2.38 MATLABS| 논리 연산자

두 피연산자

&                      AND                        |                         OR                        me

NOT

>> u=(2°0 -120° 0 2]

2  0  1  0  0  2
2. = (2.1.3.0. 20)

2     다     3     0     it     0
>> u&Vv
ans =

ul     0     1     0     0     0

“1° 값을 갖는 Be uv 모두에서 00] 아닌 WS 가짐을 나타낸다.

45


===== PAGE 54 =====
26 최신 이동통신시스템

Mobite Communications using MATLAB Simulation

OR 연산자, | 피연산자 중 하나가 참이거나 둘 모두 참일 때 참이다. OR 연산자는
두 피연산자 둘 모두가 거짓일 때 거짓이다. 수식 항으로는 두 피연산자가 0일 때 거짓
이다. 다음 예는 그 효과를 보여준다.

>> |v.

bh
bh

al    0    £    a

NOT 연산자, ~= 피연산자를 부정한다. 이 연산자는 피연산자가 참이면 A Als, 거
짓이면 참을 준다. 수식 항으로는 0이 아넌 피연산자는 0이 되고, 0인 피연산자는 1이
된다. 다음 예는 그 효과를 보여준다.

2.2.6 BH 제어

MATLAB] = 표 2.4에서 & 수 있는 바와 같이 7개의 흐름 제어 명령어가 존재한다.
이 AA = if, switch, while, for 그리고 6ㅠ68와 같은 5개의 명령어만을 사용한다.

8#표 2.48 MATLABS] 흐름 제어 연산자

if          Else, elseif 2} 함께 사용되어, 논리조건에 따라 일련의 명령을 실행한다.
switch      case, otherwise 9} 함께 사용되어, 논리조건에 따라 다른 일련의 명령을 실행한다.
while     논리조건에 따라 일련의 명령을 무한대로 반복 실행한다.
for        정해진 수만큼 일련의 명령을 반복 실행한다.
break          fort} whileo] 실행을 끝낸다.
try-catch | JY 도중 오류가 검출되면 흐름 조절을 변화시킨다.
return | 실행을 야기한 함수로 되돌아가도록 한다.

46



===== PAGE 55 =====
MATLABS| 시뮬레이션 둘로서의 기초적 사용법 (을

(1) if, else, 그리고 elseif
연산자 는 논리 표현식을 평가하고 표현식의 값에 따라 명령어 그룹을 수행한다. 문
법은 다음과 같다.

if logical_expression
statements

elseif
statements

end

논리 표현식이 참 (1)이면, MATLAB if} end 사이의 BE 명령문을 수행한다. 다
음으로 ond 문 다음부터 수행을 다시 시작한다. 조건식이 거짓 (0)이면,4411.48은
와 600 사이의 모든 명령문을 건너뛰고 000 문 다음부터 수행을 다시 시작한다. 다음은
명령어의 사용 예이다.

[Program]
k=1
if k==1
fprint£ (“0k 107

end

[Result]
Ok

(2) switch
명령어 switche 어떤 변수나 표현식의 값에 따라 특정 명령문을 실행한다. 기본 형
태는 다음과 같다.

switch expression ( scalar or string )
case valuel

statements
case value2

statements

47


===== PAGE 56 =====
ZY 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

otherwise
statements

end
위 명령문 블록은 다음 요소로 이루어져 있다.

Bswitch. 다음에는 평가될 표현식이 뒤따른다.

※수개의 case 그룹. 이 그룹은 표현식이 가질 수 있는 HO] case 다음에, 한 Fo] 표현
된다. 뒤따르는 선에서는 표현식이 그 값을 가질 때 수행할 명령문이 포함된다. 이 명령
HL swithS 포함한 모든 MATLAB 명령문이 사용될 수 있다. 하나의 case_ 다음
6886나 otherwiseS 만나면 끝나게 된다. 표현식과 값이 일치하는 하나의 6856만이 수행
된다.

『선택사항인 otherwise 그룹. 이 그룹은 이전 case 그룹에 의해 다뤄지지 않은 그 외의
표현값의 경우에 수행되는 명령문을 7/42) otherwise 문으로 PY At. otherwise 그룹
은 600 문에서 끝난다.

®End 문.
다음은 90100 문의 사용 예이다.

[Program]
k=1;
switch k
case 1
fprintt ()ie "1s" F \n*};
otherwise
fprinté (Pit is not 1 \n")’;
end

[Result]
LEAs 가

48



===== PAGE 57 =====
MATLABS| 시뮬레이션 둘로서의 기초적 vee PO

예제는 &가 1이면 MATLABS] 스크린에 “16 1”을, 다른 값이면 “It is not 1”을 출
력한다.

(3) while
while 루프는 제어 표현식이 참 (1)인 경우 BATS 반복 수행한다. 문법은 다음과
같다.
while expression
statements
end

U2 while 명령의 사용 예이다. 이 예는 간단한 합을 구하는 예이다.

[Program]
n=1;
while n<100
n=n+1;
end\
fprintfi (“ta \n'7n)-

[Result]
100

(4) for
for 루프는 명령문을 지정된 횟수만큼 수행한다. 문법은 다음과 같다.
for index=start:increment:end

statements

end

증가분의 기본 값은 1이다. 이 값은 음의 값을 포함한 어떤 값으로도 지정할 수 있다.
양의 색인 값인 경우, 색인 값이 ond WS 초과할 때 수행이 중단된다. 음의 증가분에 대
해서는, 색인 go] end 값보다 작을 때 수행을 중단한다. 예를 들면, 다음 예는 1에서

49



===== PAGE 58 =====
최신 이동통신시스템

a

Mobile Communications using MATLAB Sinmuation
100까지의 합을 구한다.

[Program]
total=0;
for n=1:100
total=total+tn;
end
fprinti (4d=\n" , total);

[Result]
5050

2.2.7 기성 함수들

2.2.6장에서 언급된 함수들 외에 많은 MATLAB 호

수들을 사용할 것이다; 이들 함수

에 대해 관심이 있다면 MATLAB 교재들을 참고하기 바란다[1]. 본 장에서는 본 책에서

사용되는 몇몇 중요 함수들에 대해 정리한다. 이들 함수는 표 2.5-2.8에 정리되어 있다.
BH258 이 AUN 사용된 주요 함수들 (1)
명령      적요              설명                  예
abs(-5)=5
=                는 ※의 원소들으
abs         Y=abs(X)        abs(X)= X29] 원소들의 절대값           abs(3+4i)=5
acos(X)           Y=acos(X)                                                                                                                   acos(cos(z))=3.1416
asin(X)     Y=asin(X)        역 삼각함수                              asin(sin(z/2))=1.5708
atan(X) | Y=atan(X)                                                            atan(tan(z/4))=0.7854
                 ceil(X)= ※의 WAS ※보다 크거나 같은 X=[-1.9 0.2 3.4 5.6 7.0]
ceil           Y=ceil(X)                                        ii                       :
가장 가까운 정수로 올림한다.                   ceil(X)=[-1 04 6 7]
_                   a=[1 23 4]
es            ORIG Petey Latholes 1-7)                            conv(a,b)=[10 40 100 160 170
120]

50



===== PAGE 59 =====
MATLABE| 시뮬레이션

둘로서의 기초적 사용번 (를

cos(X)       Y=cos(X)                                                         cos(z/3)=0.5000
sin(X)       Y=sin(X)          삼각함수                                     sin(st/6)=0.5000
tan(X)              Y=tan(X)                                                                                                                  tan(st/4)=1.0000
오류함수 ere 가우시안 분포함수를0| 30
브              브
erf          Y=erf{x)          TELLS                           y=erf(x)
id 2 (7 oP
erf{x) =  ip  J, e                          plot(x,y)
complementary 오류함수  erfe(x)=  [1 30]
으
바구        개        complementary erf(x)2] 값             880
ee      =f:
erfc(x)    He  f£ e       1—erf{x)        plot(x,y)
exp             Y=exp(X)            exp(X)= x2] 각 AAO] eS 준다.            exp(1)=2.7183
a               felose(fid)= 특정 파일이 열려있는 경우 fid=’ parameter.txt’
close
fclose           (fil           ,          이를 닫고 성공한 경우 0S 실패한 경우-1 fopen(fid)
n
ene        을 리턴한다.                             fclose(fid)
2 2.68 이 HOA ASA 주요 함수들 (2)
명령                 적요                                             설명                                                              예
fft         y=fft(x)         fft(x)= 벡터 x2] fast Fourier transform | X=[1 1-1-1-111-1]
(FFT)
:                      .                      fft(x,n)- 00101 FFT                                     fft(ifft(X,8))=
ifft         y=ifft(x)         :
ifft(x)= 벡터 xo] 역 FFT                    [11-1-1-111-1]
ifft(x,n)2 n-point 역 FFT
소수점 이하를 제거하여 ※의 AAS AS | X=(1.9 0.2 3.45.6 7.0
fx      Y-fix(X)      수점 이하를 제거하여 의 USS 정수    [             ]
로 만든다.                                            fix(X)=[-1,0,3,5,7]
-            venir kk enim          X=[-1.9 0.2 3.45.6 7.0]
oor         =TLoor                 ae            |:          사초
아오 로고                 floor(X)=[2 -1 3 5 7]
fopen      fopen            fopen(‘filename’,)permission’)               fid=’ parameter.txt’
(‘filename’) | fopen(‘filename’,’permission’)¢ 특정 모 | fopen(fid,’r’)

드로 파일을 연다.
7°: 읽기 모드

fclose(fid)

51


===== PAGE 60 =====
4    최신 이동통신시스템

Mobile Communications using MATLAB Simuflailion

+”: 읽기와 쓰기 모드

ㆍ\": 존재하는 파일의 Yes 지우거나
새 파일을 만들고 쓰기 모드로 연다.

ㆍ +": 존재하는 파일의 내용을 지우거나
새 파일을 만들고 읽기, 쓰기 BES 연다.
‘a’: 새 파일을 생성하여 SAU 존재하는
파일의 끝에 쓰기, 첨가 모드로 연다.

‘at’: A 파일을 생성하여 SAU 존재하는
파일의 일기, 끝에 쓰기, 첨가 BES 연다.

#2278 이 책에서 사용된

주요 함수들 (3)

명령                  적요                                                   설명                                                              예
fprintf | fprintf(fid, | 행렬스의 데이터를 특정 Mo] 맞게 형식화한다. | a=3
*format’,A,-*:) | -\n newline                                                  b=1.2
-\t horizontal tab                                                   c=0.0003
%d 십진수                                                 fprintf(“%d\t%f\t%
- %e exponential 형식                                     e\t%e\n’,a,b,c)
Hf TAS 형식                                           3 1.2000 3.0000e004
fscanf | fscanf(fid,        특정 파일 80로부터 데이터를 읽고 측정 형태로 fidd=fopen(‘test.txt’);
‘format’,size) | 변환하여 행렬이나 벡터로 리턴한다. 크기는 읍 | fscanf(fidd,’%g’,[1,1]);
fscanf(fid,      션이다.
‘format’)        -n: 열벡터로 개의 원소를 읽는다.
‘inf 파일의 끝까지 읽고 [미는 mbyn 행렬
을 채울 수 있는 수만큼 읽는다.
-%0 십진수
%6.%6%8 부동소수
108        Y=log(X)         X 원소의 자연로그                                    log(exp(1))=1
10810 | Y=logl(X) | X 원소의 상용로그                                        106810(1000)=3.0000
length | y=length(X)      벡터 x2] 길이를 계산                             x=[1,2,3]
length(X)=3
rand       Y=rand(m,n)      균일분포를 갖는 랜덤 mbyn 행렬                    rand(2,3)=0.5828
0.3340 0.5798
0.4235 0.4329
0.7604

52



===== PAGE 61 =====
MATLABS 시뮬레이션 둘로서의 기초적 사용법 FOE

822.88 이 책에서 사용된 주요 함수들 (4)

명령     적요          설명               ol

randn         Y=randn(m,n) | 정규 분포된 랜덤 mbyn 행렬       randn(2,2)=
-0.4326 0.1253 -1.1465
-1.6656 0.2877 1.1909

randperm | p=randperm(n) | 정수 1:2의 랜덤 순열              randperm(6)SMS [3 2 6 4 1 5]일 수
도 있고 1:6의 다른 순열일 수도 있다.

real           X=real(Z)          2 원소의 실수 부분                  real(2+3.*i)=2

rem              rem(x,y)                rem(x,y)=xn.*y 여기서                  rem(5,2)=1

n=fix(x./y) = x./y2] 정수부분

round          Y=round(X)         X AAS 가장 가까운 정수로 반 | X=[-1.9 -0.2 3.4 5.6 7.0]

=F                                      round(X)=[-2 0 3 6 7]
sqrt          Y=sqrt(X)         X 원소의 제곱근                    sqrt(2)=1.4142
sqrt(-2)=1.4142i
sum          Y=sum(X)          벡터 x9] 합을 계산                  X=[1,2,3]
sum(X)=6

2.2.8 ASA 프로그래밍

지금까지는 MATLABS 하나의 해석기 타입의 소프트웨어로 소개했다. 그러나
\1411.48은 C, C++ 혹은 20#1※ㅅ찌과 같은 프로그래밍 언어로 사용될 수도 있다.
프로그램은 주함수와 부수적인 파일들로 이루어지고 ASA 구조를 가진다. 주함수와
부함수의 관계를 그림 2.1에 제시한다. 이 장은 계층적 프로그램의 생성을 예로써 설명
한다.

예제는 다음과 같은 목적을 수행하는 프로그램이다.

53


===== PAGE 62 =====
~

최신 이동통신시스템

한        Mobile Communications using MATLAB Simuation

Main function. m

idata                   iout 10818        iout             idata           iout
“—                  qout     ~       qout            qdata          qout

Subfunction1. m                  Subfunction2.m =) vs"

~   Communication of arguments

Mad 21 주함수와 부함수의 관계

1. 가우시안 랜덤 데이터의 생성
2. value9} disper. 이름 지어진 부함수를 이용한 평균과 분산의 계산

먼저 두 개의 부함수를 정의한다. A 번째 함수는 BTS 계산하기 위한 것이
다. 줘개의 심벌 데이터로 이루어진 데이터 BF indata=[%, 42, 0 ,…, Aw Jol]
대해 평균 ES 다음과 같이 주어진다.

래스

/

MATLAB] (2.1)을 표현하는 부함수를 만들 것이다. 다음과 같은 표기법을 사용

fuction [outputl, output2, *: ] = function_name
input argumentl, input argument2, °":)

(
% start. of files
calculation equation by using input

output variable 1

arguments

output variable 2     calculation equation by using input

54



===== PAGE 63 =====
MATLABS| 시뮬레이션 둘로셔의 기초적 사용법 (을

arguments

% end of files

여기서 “= FAS 나타낸다. G+ function_name.m7} 같은 이름으로 저장되
어야 하는데 “.2”은 MATLAB 함수를 의미한다. 이 함수를 실행하기 위해서는
MATLABS] 현재 디렉토리가 파일이 저장된 디렉토리와 동일하거나 셋업 메뉴를 통
해 MATLAB 경로를 파일이 존재하는 디렉토리로 설정해주어야 한다. 부함수를 만들
기 위한 과정을 평균값을 계산하는 부함수를 만드는 AS 통해 공부해 보자.

먼저, \070080나 MATLAB 편집기와 같은 편집기를 실행해 새로운 파일을 생성한
다. MATLAB 편집기를 사용하고자 한다면 다음과 같이 입력한다.

>> edit

프로그램 2.19] 보인 mvalue.my} 같은 프로그램을 생성해야 한다. 이 프로그램의 경
우 입력 변수와 출력 변수는 모두 하나로 동일하다. 함수에서, 벡터의 모든 항을 더하고
이를 입력 벡터의 크기로 나누어준다. sum 명령어와 16080 명령어의 사용은 2.2.7장에
ㆍ 기술되어 있다. 이들을 이용해 분산과 표준편차를 계산하는 부함수를 구현할 수 있다.

WE] indata=[a,, 08, a3,°°, )/!에 대해 분산과 표준편차는 각각 다음 식으로
얻을 수 있다.

N.

44
2. | ua
V (indata) = + a    -    7,

(2.2)

o(indata) = .{V (indata)                              (2.3)

부함수는 분산과 표준편차를 출력 값으로 갖는다. 분산 값 출력을 48082, 표준

ef

55


===== PAGE 64 =====
ZY  최신 이동통신시스템
C

Mobife Communications using MATLAB Simulation

편차 출력을 98008라고 정의하고 YA OSE indata 벡터를 사용한다. 입력 데이터는

프로그램은 2ㅁ*8106.2과 동일한 디렉토리에 저장되어야 한다. 프로그램 이름을
disper.m° = 저장하라.

지금까지 두 개의 부함수를 만들었다. 다음으로, 주함수를 만들 것이다. 새로운 파일
을 열어 프로그램을 VST mainmo Ss 부함수와 동일한 디렉토리에 저장하라.208010.0
은 프로그램 2.3에 주어졌는데, 여기에서 랜덤 데이터가 자동적으로 생성되고 평균과 분
산이 계산되어진다. 프로그램을 만든 So}, mvalue.m, disper.m 그리고 main.me] 존재
하는 디렉토리에서 ㅁ810.0을 실행하면 다음과 같은 데이더를 얻게 된다.

>> main

meanvalue = 0.522608
dispersion = 0.111834
standard deviation=0.334415

결과로써, 평균과 분산 그리고 표준편차를 주함수에서 사용할 수 있다. 이 책에서는
많은 부함수들을 생성할 것이다. 최종적으로 여러분은 많은 함수 자료들을 얻게 될 것
이다

| 23 | 데이터 생성과 비트 오류율 (611 Error Rate)

시스템 성능을 평가하기 위해 비트 오류율 (BER)S 분석한다. 본 장에서는 비트 오
류 확률을 정의하고 몇 개의 예를 통해 BERS 계산하는 방법을 보인다. 위 예를 사용하
여, 0이나 1로 구성된 165-10 벡터로 구성된 데이터를 생성한다. 벡터 %084는 다음과
같다.

>> txdata=rand(1,10)>0.5

txdata =
ae    0    +    0    1    1    0    0    1:    0

56



===== PAGE 65 =====
MATLABS| 시뮬레이션 툴로서의 기초적 se (을

통신 채널에서 오류가 발생하여 \08001,7)이 0에서 1로 변한다면, 수신 데이터
rxdatat 다음과 같다.

>> rxdata=txdata;
>> rxdata(1,7)=1
rxdata =
1    0    i    0    L    al    gf    0    1    0

>> rxdata(1,9)=0
rxdata =
1    0    a    0    1    나    1    0    0    0

>> nod=length (txdata)
nod =
10

오류의 수를 계산하기 위해서 다음과 같은 과정을 거친다. 먼저, 송신 데이터 \084
를 수신 데이터 ㅠ008로부터 뻔다. 만약 오류가 없다면 000와 같은 크기의 영벡터를 a
Al 된다. 오류가 존재하면, 오류 위치에 “…1”이나 “1*의 값을 갖는 벡터를 얻게 된다. 이
차 벡터 subdata= 다음과 같다.

>> subdata=rxdatatxdata

subdata =
0    0    0    0    0    0    5    0   그    0

subdatao]]A] 볼 수 있는 바와 같이, &%0813의 항이 오류에 의해 0에서 1로 변하면
804608343의 해당 위치의 항이 “1”이 된다. 반면, 오류에 의해 &081의 항이 1에서 OLS

57


===== PAGE 66 =====
최신 이동통신시스템

^.

58

Mobile Communications using MATLAB Simulation

변하면 946080의 해당 항은 “-1”이 된다. subdatas] 각 항의 절대 값을 얻으면 오류 항
의 위치에 “1*을 갖는 벡터를 만들 수 있다.
>> abs (subdata)

ans =
0    0    0    0    0    0    aL    0    48    0

008(600084)의 모든 항을 더함으로써 오류의 pS 구할 수 있다. 각 항의 HS 얻기
위한 MATLAB 명령어는 “900”이다. 오류의 수 206는 다음과 같이 sum 명령어로 구
한다.

>> noe=sum (abs (subdata) )
noe =
Z

결국 206와 200를 써서 비트 오류 확률을 계산할 수 있다. 비트 오류율을 6@로 정의
하면 다음과 같이 206와 000의 비로 나타난다.

>> ber=noe/nod
ber =
0.2000

본 책에서는 이 과정을 통해 BERS 얻을 것이다.

ZB 이동통신용 전송채널의 정의

본 책에서는 백색잡음 (AWGN) 다중경로 페이덩-환경 하에서 시스템 성능에 대해
분석한다. 본 장에서는 AWGN3} 다중경로 페이덩에 대해 설명하고, 이들을 MATLAB
에서 구현하는 방법을 설명하도록 하겠다.



===== PAGE 67 =====
MATLABS| 시뮬레이션 둘로서의 기초적 사용법 (을

2.4.1 AWGN 채널

수신기의 입력단에서 신호의 수학적 모델을 생성하면, ALS 그림 2.2에서와 같이
백색 가우시안 잡음을 첨가함으로써 ATS 오염시키는 걸로 가정 된다 [2]. 송신 신호,
백색 가우시안 잡음, 수신 신호를 각각 $(), nlf), ANS 정의하면, 수신 신호는 다
음과 같이 나타낼 수 있다.

ee

r(t) = s(t) +n(t)                                       (2.4)

- 0 aca” ag

|"

Additive white Gaussian noise

Amplitude                  pdf of power spectrum density                 pdf
:           1                                                    Variance = power
rem
Asad                                                 >
“igs                f          0      Amplitude

를 그림 2.2 AWGN 채널의 예

여기서, 7(7)는 확률밀도함수 (001)를 갖는 AWGN 과정의 AS 함수이고 파워스펀
EWE (power spectral density)= 다음과 같다.

1
®,,(f)= No [W/H2]         as

위 식에서 Ne 상수이고 잡음파워밀도라고 부른다. AWGNS 51411.40에서 시
뮬레이션하기 위해서는 내장함수인 0002을 사용하는데, 이 함수는 각 항이 평균 0과

59


===== PAGE 68 =====
최신 이동통신시스템

60

Mobile Communications using MATLAB Simifation

분산 1의 정규분포를 갖는 랜덤 수나 행렬을 생성한다. AS inphase 채널 (Ｌ채널)과
quadrature-phase 채널 (채널) 데이터 벡터 idata2} 022%에 파워가 1인 AWGN 잡
음을 가산하면, Ｌ채널과 -채널의 출력 데이터 702/과 0024은 다음과 같이 주어진다.

iout(t) = idata(t) + randn(t)
qout(t) = qdata(t) + randn(t)                           (2.6)

시뮬레이션에서는 때때로 잡음 파워를 AS npowe 정의하고 이를 BSP)|A BER
을 계산한다. idataS} qdata= 파워가 아닌 전압이므로 npowS 전압에서 파워로 변
환해야 된다. 변수 27^/을 727000의 근으로 정의한다.

1
attn = —./npow
2                          (2.7)

AZ, npow!| IAS 가진 잡음에 의해 오염된 후의 출력 데이터는 다음과 같다.

iout(t) = idata(t) + attn x randn(t)
qout(t) = qdata(t) + attn x randn(t)                       (2.8)

프로그램 2.4는 디지털 직각 위상 변조방식으로 표현된 입력 데이터에 AWGN 가
산할 수 있다. 입력 데이터로 722%와 022/%를 사용하고 출력 데이터는 7020과 gout
이다. 잡음에 오염된 ASS 만들기 위해 atin, idatad} 4420만을 입력하면 된다.

2.4.2 레일리 Hol? 채널

지상 이동통신의 기지국과 이동국 사이의 경로는 다양한 장애물과 반사물로 특성지
어진다. 예를 들면, 실내 환경은 사무기기와 가구 그리고 실외환경은        2
이 존재한다. 이들은 무선 파형이 기지국에서 이동국으로 전파될 때 수신신호에 많은
영향을 끼치게 된다. 지상 이동통신에서의 무선파 ASS] 기본적 특성이 그림 2.3에 나

ou,



===== PAGE 69 =====
MATLABS| 시뮬레이션 툴로서의 기초적 사용법  101

타나 있다. 기지국에서 송신된 무선파는 모든 방향으로 복사되는데 여기에는 다양한 장

애물에 의해 반사된 반사파, 희절가, 산란파과 기지국에서 이동국으로의 직접파들이

존재한다. 이 경우, 직접, 반사, Bas 산란파들의 경로 길이가 다르기 때문에 이동국

에 도달하는 시간도 각각 다를 것이다. 게다가 입사되는 파동의 위상이 반사 때문에 다

양하다. 결과적으로, 수신기는 다른 위상과 도착 시간을 갖는 여러 파동들로 구성된 중
A

다중경로 전송 환경에서 수신신호는 때때로 증강되거
페이딩인데 수신과의 신호 레벨은 매 순간 변하게 된
환경에서 디지털 무선 신호가 전송될 때 수신신호의
능력을 위해서는 이 다중경로 페이딩을 보상해 줄 수           2
이 장은 다중경로 페이딩의 개념과 이를 시뮬레이션하기 위한 프로그래밍 방법을 설명
한다.

페이딩이 발생하는 구조부터 시작하자 [3, 41. 단일주파수 /,(82/의 연속가가 기지
국에서 전송되었을 때, 그림 2.3에 해당하는 입사각 0, 을 갖는 지연가는 다음과 같이
주어진다.

r, (t) = Refe, 060 j(2af.0)]        (2.9)

여기서 6[]는 복소수에서 실수부분을 나타내는데 n 방향에서 오는 파동의 복소
수 포락선을 얻게 해준다. 또 /는 복소수이다. 6,(?)는 입사파들의 기지국에서부터의
전송경로 길이 7.,,(000)와 이동국의 속도 1020/8) 그리고 파장 102)로 다음 식 (2.10)
과 같이 쓸 수 있다.

22(/. —vtcos@, )  -
A

e, (t) = R, (exp {-                             개 =x, (t)+ jy,

(2.10)
61


===== PAGE 70 =====
2) 최신 이동통신시스템
C        Mobile Communications using MATLAB Simulation

를 그림 2.3 다중경로 채널의 원리

이때 2,과 @,는번째 입사파의 포락선과 위상을 나타낸다. %,(?)과 y, (A= 4
각 e,,(t)2] inphase$} quadrature-phase 성분이다. 번째 입사파는 도플러 효과에 의
해 반송 주파수를 veos 0,,/ 40832)로 전이시키는데 이를 지상 이동통신에서 도플러 전
이라고 부른다 [3, 4]. 이 도플러 전이 f= 입사파가 이동국의 이동방향으로부터 즉

cos 0, = 1의 방향으로부터 발생할 때 최대  v/AS 갖는데 이 Ho] 도플러 전이의
최대 값이 된다. 이동국의 뒤에서 오는 지연파 또한 -7/,』,082)의 주파수 전이를 갖는

이동국에서 수신된 수신파 7(7)가 위에서 언급한 입사파들의 합성이기 때문에 입사
파의 수가죄일 때 수신파는 다음과 같다.

62



===== PAGE 71 =====
MATLABS 시뮬레이션 둘로서의 기초적 사용법 (를

r(t)= 2. (0)

= Re (Se o| exe)
= Re|(x(t) + j(v(t)Xcos 2af,t + j sin 27f,t)|

(2.11)
= x(t) cos 2f,t — y(t)sin 2af,t
여기서 x(t) 7(/)는다음과 같이 주어진다.
x(t) = }' x,
n=1
N
w= Dy)                             (2.12)

x(t)S y(t) EN] 충분히 클 때 평균 0과 분산 oS 갖는 정규화된 랜덤 과정들이

다. x=x(t), 1= vy CH) BAY 조합 확률밀도 d(x, PEGE 식 (2.13)과 같다.

1    x+y?
x,y)=  ex
P(x, y) eae | a? ]

(2.13)
수신파의 진폭과 위상을 사용하여 *(7)를 표현할 수도 있다.
r(t) = R(t) cos(2af,t + 0(t))                          (2.14)
RU) 0(7)는다음과 같이 주어진다.
RQ)=R= x? +y?
O(t) = 6 = tan [y/x]            (2.15)

63



===== PAGE 72 =====
~  최신 이동통신시스템

Mobile Communications using MATLAB Simulation

변수의 ASS 통해, a(x, VE A(R, DZMES VC.

R     R*
R,@)=     exp| -
ics 220" | 쓰|     (2.16)

IRS 0에서 2까지 OR, OS 적분함으로써 확률밀도함수 7(2)을 얻는다.

R     R?
R) = —~exp| -
PIR) o nf x

(2.17)

또한 을 0에서 00까지 (RK, 0)를 적분함으로써 확률밀도함수 2(0)를 얻을 수
있다.

1
PO.                               (2.18)

이 수식들로부터, 포락선 WES 레일리 분포를 따르고 위상 변동은 균등분포를 갖는
다. 다음으로, 레일리 페이딩의 시뮬레이션을 위한 표현식을 찾아보자. 그림 2.3에 보인
바와 같이, 이동국은 FATS 수신하는데 수신 입사가의 입사각은 균일하게 분포되어
있고 입사파들의 FE #&이다. 이런 경우, 등가적인 저역통과 시스템의 복소수 페이딩
변동은 다음과 같다 [3, 41.

r(t) = x(t) + 7 ㆍ)(0)

We a   aaa cof 22" soon]

(2.19)

64



===== PAGE 73 =====
MATLABS| 시뮬레이션 툴로서의 기초적 사용법 (를

여기서 Ny 흘수이고 N.S 다음과 같이 주어진다.

1(
Oe 시끄 2 1                                        (2.20)

이 경우, 다음 관계가 성립한다.

Elx?(0)|= Ely2]= 5
Elx,(0)y,@]=0                                      (2.21)

Al (2.19)의 결과는 프로그램 2.59] 형태를 가진다. 프로그램 2.5에서, 출력 ATES
신기에 의해 형성된 복소수 변조 신호를 입력하고 동등한 저역통과 시스템으로 표현함

2
@                Delayed waves

a

4    Normalized time

—

ott

수

Direct wave

를 그림 24 다중경로 페이딩 채널의 구성

65



===== PAGE 74 =====
최신 이동통신시스템

a

66

Mobile Communications using MATLAB Simulation

Roe 각에 수신신호를 관찰하면 ASS 레일리 BLS, 위상은 균등분포를 가짐이

확하다. 또한 직접파와 지연파의 평균 전기 파워의 고정비가 존재하는 것도 명확하

로 다시 말하면, 다중경로 전송 환경이 시뮬레이션 될 때 단순히 직접파에 비해 지연파

의 상대적인 신호 레벨과 상대적인 지연 시간을 주면 된다. 이 SHES 그림 2.5에 보

였다. 다중경로 페이덩의 시뮬레이션을 위한 프로그램이 프로그램 2.6과 2.6에 AAS
었다.

Start j=0

Input parameters
Input | ch data                              : 10868
100바으라 086                              : 00818
For delayed wave #/            Delayed time                              ‘itau
Signal power of delayed waves __: dlvl
Time resolution                          : tstp
Simulation time in one simulation :nsamp
Shift of input data               Fading counter                             : 07
by delayed time
Fade for the shifted
signal by subfunction            Output data
Output Ich data: iout
Output Och data: gout
j= the number of

delayed wave

end

름도

rol
Jon

를 그림 2.5 레일리 페이딩 채널을 얻기 Ae

프로그램 2.6에서, 시간 해상도, 직접파와 지연파의 상대적 신호레벨, 상대적 지연시
간, 수신기의 의해 형성되고 동등한 저역통과 시스템에서 표현된 복소수 변조신호, 1회

시뮬레이션 루프 시간을 입력한다.

예를 들어, 1회의 시뮬레이션 루프 시간이 50 /&이고 시뮬레이션의 최소 시간해상도
가 0.5 /4인 경우를 생각해 보자. 세 지연파가 직접파에 비해 각각 10 03, 20 03, 25 08
작은 평균 파워를 가지며, 직접파에 비해 1, 1.5, 2.0 ws] 시간 지연을 갖는다고 가정한
다. 이런 경우, 다중경로 Hole 시뮬레이터의 입력 변수는 다음과 같다.

&



===== PAGE 75 =====
MATLABS| 시뮬레이션 둘로서의 기초적 사용법 (를

Estp =20.5.^20.^(000
itau = [0 floor(L.*10.-* 6) /tstp)
floor (165.710.^ (36) (stp)

floor (2.0: *10.. O (6): estes yi 010, 2, aye ate
Givi: =O, =10,° 207-3254
nsamp = 50.*10.%(-6)/tstp = 100;

다음으로, 다중경로 페이덩 시뮬레이터의 연산에 대해 기술한다. 우선, 입력 신호는
입력 매개변수를 이용해 지연된다. 다음으로, 레일리 페이덩이 지연된 신호에 부가된
다. 매개변수의 지연파 집합의 수만큼 이 과정을 반복하고 모두 더한다. 이 결과 다중경
로 레일리 페이덩 출력 신호가 얻어진다.

이 경우 한 가지 문제가 존재한다. 일반적으로 말해서, 레일리의 분포는 각 지연시간
에 대해 독립적이어야 한다. 그러나 이 시뮬레이션에서 모든 전송 경로의 페이덩 파형
들이 하나의 함수에 의해 생성되므로 분포들이 동일하다. 이 특성을 그림 2.6에 보였다.
이런 이유로, 각 지연시간에서의 페이덩을 SHALE 생성하게 해주는 기법이 필요하
게 된다.

독립적인 페이덩 지연시간을 생성하는 다양한 방법이 존재하는데, 여기서는, 페이딩
카운터 기법이 하나의 예로 제시된다. 페이덩 카운터는 1486.0에서와 같이 페이덩 생성
기에 페이덩 생성의 시작시간을 건네준다.

그림 2.62 페이덩 생성기에 의해 AVA 변동 ASS 보여준다. 시뮬레이션에서는
페이덩 생성기를 사용하기 때문에 단지 하나의 페이덩 파형이 존재한다. 모든 직접파와
지연파의 페이덩 생성기가 두 파형에 모두 같은 Holy ALAS 설정하여 동시에 시작
한다면, 모든 페이덩 파형들은 그림 2.6에서와 같이 동일하다. 그러나 그림 2.7에서와
같이 페이덩 카운터를 다르게 설정해 모든 직접파와지연파들이 서로 다른 페이덩 생성
시작시간을 갖는다면 각 전송경로에서 생성된 페이덩의 파형들은 다를 것이다. 이를 통
해, 독립적으로 분포된 레일리 페이덩 환경을 시뮬레이션할 수 있다.

67


===== PAGE 76 =====
월
ZY 최신 이동통신시스템
C        Mobile Communications using MATLAB Simulation

Signal fluctuation
by a fading simulator

Time
Start time to generate a
direct and a delayed wave
7)
Time
(a)
Zk
Time |
(b)
를 그림 26 AAU 지연파를 생성하기 Ast 시작시간이 같은 경우, Hols Asal
이터에 의한/신호 변동: (a) 직접파의 AS HS (6) AAU Als 변동

프로그램 2.6에 29] sefademS 평가하기 위한 프로그램을 프로그램 2.8에 제시한
다. 페이덩 카운터의 시작 값은 이 평가 프로그램에 주어진다. Holy 카운터의 벡터 a
기는 지연파의 지연시간을 나타내는 벡터의 크기 그리고 지연파의 상대적 파워 레벨을
나타내는 벡터의 크기와 동일하다. 카운터를 적절하게 설정함으로써 레일리 페이딩은
독립적으로 형성된다.

68



===== PAGE 77 =====
MATLABY| 시뮬레이션 툴로서의 기초적 사용법

Signal fluctuation
by a fading simulator

Time

Vv

Start time to generate           Start time to generate
a direct wave                     a delayed wave

(a)

를 그림 27 Ag
이터에 st As 변동: (a

jo 모
en!

[요
a=)
mult
0=
Ox
Oli
Be ht
ㅇ

[와
pr
건
^

ie

=
eee
00

(nd

40

페이딩 카운터는 각 시뮬레이션 루프 후에 시뮬레이션 시간에 해당하는 0000 값을
더함으로써 갱신된다. 0.5 /6&의 최소 시간해상도와 50 /4의 관측시간을 갖는 경우에 각
시뮬레이션 루프 후에 100 포인트가 더해진다. 가산된 값을 갱신 시간이라 부른다. 갱

이 같은 경우 그림 2.8(a)9} 갱신 시간이 관측시간보다 큰 경우 그림 2.806)에 페이딩에
의한 시뮬레이션된 신호 레벨을 보여준다.

69


===== PAGE 78 =====
a

최신 이동통신시스템

70

20276 Communications using MATLAB Simulation

Update

time

Observation                                                                               :

time                                                                                    Fading counter
Start point for      for       for        for         for        for           "두

forloop1 10002 10004 10006 10008  loop 10 loop 12
(a)

A
Update _ |
time

Observation
time                                                                                              Fading counter

Start point Startpoint Start point       Start point       Start point
forloop1 for loop 2       for loop 3        for loop 4         for loop 5

를 그림 28 관측 시간과 갱신 시간의 관계:

갱신 시간과 관측시간이 같은 경우, 연속적으로 변하는 신호 레벨 환경에서 전송 성
을 평가할 수 있다. 그러나 많은 시뮬레이
문에

능                          션 루프에 의해 신호 분포가 레일리가 되기
때문에 시뮬레이션된 성능이 안정화되는데 많은 시간이 걸린다. 반면, 갱신 시간이 관
측시                 에는 그럼 2.806)와 같이 적은 수의 시뮬레이션 루프로도 레일리 페

간보다 큰 경우

이덩 하에서의 AS 성능을 평가할 수 있다. 그러나 이 경우 시뮬레이션 결과가 정확하
지 않을 수도 있다. 그러므로 전송 성능을 정확하게 검사할 때에는 갱신 시간을 증가시
켜주는 Al 좋다. 다중경로 페이덩 시뮬레이터는 이후의 논의에서 계속 사용될 것이다.

본 장에서는 이 책에서 사용되는 시뮬레이션 언어인 44411.408을 이동통신시스템의
시뮬레이션을 위해 필요한 기초적인 사용법을 위주로 소개했다. 또한 4^11.48을 이
용하여 이후의 장에서부터 사용되어질 프로그램 함수들을 생성해 보았다. 이 장의 뒤부
터 이어지는 3장의 이동통신 시스템의 시뮬레이션은 2장에서 습득한 지식을 토대로 행
해지게 될 것이다.



===== PAGE 79 =====
MATLABY| 시뮬레이션 SEMI 기초적 사용법  10 |

1) MathWorks Inc., “MATLAB Using MATLAB.”
2) Proakis, J. G., Digital Communications, 3rd ed., New York : McGraw-Hill, 1995.
3) Jakes, W. C., Microwave Mobile Communications, New York: IEEE Press, 1994.

4) Sampei, S., Applications of Digital Wireless Technologies to Global Wireless Communications,
Upper Saddle River, NJ: Prentice Hall, 1997.

71



===== PAGE 80 =====
최신 이동통신시스템

Mobiie Communications using MATLAB Simulation

BE OA

프로그램 2.1

Program 2-1

00

oe

00

calculate average

00

oe

Programmed by H.Harada

oe

function outdata = mvalue(indata)

ZRKEKKKKKKKKKKKKKKKK  Variables KERR KKK KKK KKKKKKKKKKKKKKK

%       indata : Input data

ZR KKK KKK KKK KKK KKK KKK KK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK

outdata=sum (indata) /length (indata) ;
옹 KKKKKKKKKKKKKKK KANG of ELLER RR KKK KKKK KKK KK KKK KK KKK KKK
프로그램 2.2

Program 2-2
disper.m

00 ol?

ae

calculate dispersion and standard deviation

00 00

ole

Programmed by H.Harada

ole

function [sigma2, sigma]=disper (indata)

ZREKKKKKKKK KK KKK KKK  variables  KKK KKKK KKK KKK KKK KKK KKK KKK

% indata : Input data
% sigma2 : dispersion
% signa   : standard deviation

ZR KKK KKK KKK KK KKK KKK KKK KKK KK KKK KKK KKK KEK KK KK KKK KKK KKK KKK

으

% calculate average value
mvalue= sum(indata) /length (indata) ;



===== PAGE 81 =====
% calculate square average
sqmean= sum(indata.*2) /length (indata) ;

% calculate dispersion
sigma2=sqmeanmvalue’2;

% calculate standard deviation
sigma=sqrt (sigma2) ;

x KKKEKKKKKKKKKKKKKKKONG of ELLER RRR K KKK KK KKK KKK KK KKK KK

프로그램 2.3

% Program 2-3

% main.m

%

% calculate mean, dispersion and standard deviation for the vector

data

Programmed by H.Harada

00 00 00

data=rand(1,20);

mvalue2=mvalue (data) ;

[sigma2, sigma]= disper (data) ;

fprintf( 'meanvalue = %f \n',mvalue2);
fprintf( ‘dispersion =. sf 0, 53900 2) 7
fprintf( 'standard deviation=%f \n',sigma) ;

응 RKKKKKKKKKKKKKKKKKKANd OF FLLLEKKKKKKKKKKKKKKKKKKKKKKKK

프로그램 2.4

% Program 2-4

oe

comb.m

oe

Generate additive white gausian noise

00 00

oe

Programmed by H.Harada

oe

function [iout,qout] = comb (idata,qdata,attn)

KKK KK KKK KKKKKKKKKK Variables FEKKKKKKKKKKKKKKKKKKKKEKK

idata : input Ich data
qdata : input Qch data

00 dP 00

73



===== PAGE 82 =====
\

최신 이동통신시스템

74

Mobite Communications using MATLAB Simulation

% iout   output Ich data
% gout   output Och data
% attn : attenuation level caused by Eb/No or C/N

GH HH HK KK KK KK HK KKK RK KK KK KK KK RK KK KK KK

iout = randn(1,length(idata) ) .*attn;
gout = randn(1,length(qdata) ) .*attn;

iout = iout+idata(1:length(idata) );
gout   qout+qdata (1:length (qdata) );

& KKK KKK KR KK KKK KKK KK KONG OF ELLER RRR KKKKKKKKKKKKKKKKKKK

프로그램 2.5
% Program 2-5
% fade.m
%
% Generate Rayleigh fading

ole

% Programmed by H.Harada

function [iout, gout, ramp, rcos, rsin]=fade (idata, qdata,nsamp,tstp, fd,
no, counter, flat)

KKKKKK KKK KKK KKK KKK  variables  KKEKKKKKKK KKK KK KKK KKK KK KKK

00 le

idata : input Ich data
% qdata : input Qch data
% iout   : | output 1206 data
% qout   : output Qch data
% ramp   : Amplitude contaminated by fading
%- rcos   : Cosine value contaminated by fading
옹. FSin   : Cosine value contaminated by fading
% nsamp : Number of samples to be simulated
% tstp   : Minimum time resolution
cage ee |     : maximum doppler frequency
% no     : number of waves in order to generate fading
% counter : fading counter
% flat     : flat fading or not
% (1-flat (only amplitude is fluctuated), 0-nomal

% (phase and amplitude are fluctutated)
SR kK KK KR RK RK KK KK KK

주 fd = 020



===== PAGE 83 =====
860 = 89120 ./=(2.0." (nos tol) yy
% power normalized constant (ich)
80 =. sqrt (1.0 7/:-@.02 4no));
% power normalized constant (qch)
icO = counter;

% fading counter

pai = 3.14159265;
wm = 2.0.*pai.*fd;
n = 4.*no +27

ts = tstp;

wmts = wm.*ts;
paino = pai./no;

xc=zeros (1,nsamp) ;
xs=zeros (1,nsamp) ;
ic=[1:nsamp]+ic0;

for. nn = Ls no
cwn = cos( cos(2.0.*pai.*nn./n).*ic.*wmts );
xc = xc + cos(paino.*nn)).*cwn;
xs = xs + sin(paino.*nn) .*cwn;

end

cwmt = sqrt (2.0) .*cos(ic.*wmts) ;
xc = (2.00*xe-F 00000 300;

xs. = 2.0.%*xs.*as0?

ramp=sqrt (xc.*2+xs.%2) ;
rcos=xc./ramp;
rsin=xs./ramp;

if flat ==
16Uuk.,= sqrti(xc.%24+xs .22).*idata.(lsnsamp) ;
% output signal (ich)
gout = sqrt(xc.*2+xs.%*2) .*qdata (1:nsamp) ;
% output signal (qch)
else
lout = xc.*idata(l:nsamp) - xs.*qdata(1l:nsamp) ;
% output signal (ich)
gout = xs.*idata(l:nsamp) + xc.*qdata(1l:nsamp) ;
% output signal (qch)
end

75



===== PAGE 84 =====
최신 이동통신시스템

76

Mobile Communications using MATLAB Simulation

else

iout=idata;
qout=qdata;

end

| **×**…*××**×ㅠ*×××*×*×*××*6ㅠ01 of ELLER RRR RK KR KK KKK KKK KKK KKK KKK

프로그램 2.6

00

Program 2-6

sefade.m

%
%
% This function generates frequency selecting fading
%

% Programmed by H.Harada

function [iout, qout, ramp, rcos, rsin]=sefade (idata,qdata,itau,dlvl,
th,n0,itn,nl,nsamp,tstp, fd, flat)

ZREKKKKKKKKKKKKKKKK  variables  KEKKKKKKKKKKKKKKKKKKKKKKK

oe

idata

qdata

00

ol?

iout

00

qout

oe

ramp
rcos

00 00

rsin
itau
dlvl
th
nO

00 00 00 00

oe

itn
nl
nsamp
tstp
fd
flat

00 00

00 00

oe

: Maxmum doppler frequency

input Ich data
input Qch data
output Ich data
output Qch data
Amplitude contaminated by fading
Cosine value contaminated by fading
Cosine value contaminated by fading
Delay time for each multipath fading
: Attenuation level for each multipath fading
: Initialized phase for each multipath fading
Number of waves in order to generate each multipath
fading
Fading counter for each multipath fading
: Number of summation for direct and delayed waves
: Total number od symbols

: Mininum time resolution

flat fading or not



===== PAGE 85 =====
% (1-flat (only amplitude is fluctuated) ,0-nomal (phase
%           and amplitude are fluctutated)

ZRKRKKK KKK KKK KK KK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK

iout   zeros (1,nsamp) ;

gout   zeros (1,nsamp) ;
total _attn = 8910. .4.( 2120 |.*% .dlvl<51020)).-
fork = 1 s.ni
atts:= = 10.* (0205 7 91060)
if dlvl(k) >= 40.0
atts = 0.0;
end
theta = th(k) \.*-pi../ 180.0;
[itmp,qtmp] = delay ( idata , qdata , nsamp , itau(k));

{itmp3, qtmp3, ramp, rcos, rsin]   =   fade   (itmp, qtmp,nsamp,
tstp, £d;n0(k) itn (00) , flat)

iout   iout + atts-.*.itmp3 =/ sqrt (total attn) ;

qout = qout + atts..* qtmp3-./ sqrt(totalattn) ;

end

z KKKKKKKKKKKKKKKKKKK KANG of ELLER KKK RK KK KKKKEKKKKKKK KKK

프로그램 2.7
% Program 2-7

oe

delay.m
Gives delay to input signal

00 00 00

Programmed by H.Harada

00

function [iout,qout] = delay( idata, qdata , nsamp , 1061 )

77



===== PAGE 86 =====
\

최신 이동통신시스템

78

Mobile Communications using MATLAB Simulation

ZRRK KKK KKK KK KK KK KKK  variables  KEKEKKKKKKKKKKKKKKKKKKKKKK

%

00

oe

00 00 00

idata input Ich data

qdata input Qch data

iout   output Ich data

gout   output Qch data

nsamp   Number of samples to be simulated
idel   Number of samples to be delayed

ZRKKKKKKKK KKK KKK KKK KK KK KK KK KK KK KK KR KKK KK KK KK KK KK KKK KK KKK

lout=zeros (1,nsamp) ;

qout=zeros (1,nsamp) ;

if-idel ~= 0

iout (1:idel)
qout(l:idel) = zeros(1,idel);

zeros (1, 1061) ;

end

iout (idel+l:nsamp) = idata(1l:nsamp-idel) ;

gout (idel+1:nsamp)

%

qdata(1:nsamp-idel) ;

KKKKKKKKKKKKKKKKKKK KANG Of  ELLER RRR KKKKK KKK KKK KK KKK KK

프로그램 2.8

%

de 0 dP oP oP oP cP oP CP oP

Program 2-8
bpskev.m

Evaluation program of fading counter based BPSK
transmission scheme

This program is one of example simulations

that include fading

As for the explanation, you can check Chapter 3.

Programmed by H.Harada

ZRKEKKKKKK KKK KK KK Preparation part KKKKKKKKKKKKKKKKKKKEKK

%

Time resolution



===== PAGE 87 =====
% In this case, 0.5us is used as an example
tstp = 0.5*1.0e6;

% Symbol rate

% In this case we assume that each sample time is equal
% to 1/(symbol rate).

% In this case 200 kbps is considered.

sr = 1/tstps;

% Arrival time for each multipath normalized by tstp
% In this simulation fourpath Rayleigh fading are

% considered

itau = 10, 2, 3, 41>

oe

Mean power for each multipath normalized by direct wave.
% In this simulation fourpath Rayleigh fading are

% considered.

% This means that the second path is -10dB less than the

% Eirst direct path.

0101 =--[(0 10. 7204, 257;

Number of waves to generate fading for each multipath.
In this simulation fourpath Rayleigh fading are
considered.

In normal case, more than six waves are needed to generate

00 00 00 00 0

Rayleigh fading

% Initial Phase of delayed wave

% In this simulation fourpath Rayleigh fading are
% considered.

thi=[0.0,0.0, 0:..0,.0.:01';

% Number of fading counter to skip (50us/0.5us)
% In this case we assume to skip 50 us

itnd0=100*2;

% Initial value of fading counter

79


===== PAGE 88 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

80

% In this simulation fourpath Rayleigh fading are
% considered.

% Therefore four fading counter are needed.
itnd1l=[1000,2000, 3000, 4000];

% Number of directwave + Number of delayed wave

% In this simulation four-path Rayleigh fading are
% considered

nowl=4;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
fd=200;

% Number of data to simulate one loop
% In this case 100 data are assumed to consider
nd = 100;

oe

You can decide two mode to simulate fading by changing
the variable flat

flat     siiflattading-oer not

% (1-flat (only amplitude is fluctuated) ,0-nomal (phase

00

ole

% and amplitude are fluctutated)
flat =1;

ZRKKKKKK KKK KKK KK KK START CALCULATION KKK KK KK KKKKKKKEKKEKK
nloop = 1000; % Number of simulation loop

noe = 0; % Initial number of errors

nod = 0; % Initial number of transmitted data

for iii=1l:nloop

ZREKKKKKKK KKK KKK KKK Data generation KKEKEKKKKKKKKKKKKKKKKK

data=rand(1,nd)>0.5; % rand: built in function



===== PAGE 89 =====
웅****×*…****×**×*×*×ㅠㅠㅠ BPSK modulation KKEKKKKKKKKKKKKKKKKKEK

datal=data.*2-1; % Change data from 1 or 0 notation
% to +1 or -1 notation

GRAEKKKKKKKKKKKKKKKKKK Fading channel KEKKKKKKKKKKKKKEKKKK

% Generated data are fed into a fading simulator
% In the case of BPSK, only Ich data are fed into
% fading counter
[data6,data7]=sefade(datal,zeros(1,length(datal)),itau,
dlvl1l,th1,n0,itnd1,nowl1, length (datal),tstp, fd, flat);

% Updata fading counter
itndl = itndl+ itnd0;

GREKKKKKKKKKKKKKKKK BPSK Demodulation | 을 소오 수 스고 수 수스 고 소소 수조 오시오
demodata=data6 > 0;
GREKKKKKKKKKKKKK KKK Bit Error Rate (BER) KREKKKKKKKKKKKKK

% count number of instantaneous errors
noe2=sum(abs (data-demodata)); % sum: built in function

% count number of instantaneous transmitted data
nod2=length(data); % length: built in function

fprintf ('$d\t%e\n',iii,noe2/nod2) ;

noe=noe+noe2;
nod=nod+nod2;

end % for iii=1:nloop
ZRHEKKKKKKKKKKKKKKKKKK Output result KKKKKEKKKKKKKKKKKKKKEK

S$ber = noe/nod;
fprintf ('%d\t%d\t%e\n',noe, nod, noe/nod) ;

& KKKKKKKKKKKKK KKK KKK KANG of ELLEOX RR RRR KKK KKK KKK KK KK KKK

81


===== PAGE 90 =====
oe
oe



===== PAGE 91 =====
PSK 기
디지털 변조기

00 서른

반

버
=|

+1과-1 같은 디지털 ALS 무선가를 이용해 전송하는 가장 쉬운 방법은 디지털 정
보 데이터의 정보에 특성에 맞추어서 주파수 의 반송파를 변조하는 것이다. “변조”
의 의미는 정보데이터를 반송 신호과에 Le 행위를 Uae, 이때 반송 ass

조방식별로 반송파에 포함된 특정 성분을 변화시키는 것이다. 반송신호의 가형은
과 같이 쓸 수 있다.

S(t) = 4008122.7+0(0)}                              (3.1)

위 수식에서, A, fo ONE A 반송파신호의 진폭, 중심 주파수, 시변 위상을 나
타낸다. 식 (3.1)에는 사용자가 값을 변경할 수 있는 세 가지 특정 성분이 존재한다. 이
세 가지 성분은 진폭, 주파수, 위상인데 디지털 정보 데이터에 따라(3.1)의 진폭을 변화
시키면 AM 변조방식이라 부른다. (3.1)의 주파수를 변경시키면 FM 변조방식, 위상을
변화시키면 PM 혹은 29 변조방식이라 부른다.

85


===== PAGE 92 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

이 장은 PSK 기반 디지털 통신에 중점을 두고, 송신기와 수신기의 기본 PIS 기술
하고, 이 구성을 컴퓨터 시뮬레이션을 통해 표현하는 방법에 대해 설명한다. 3.2장은
808에 대해 기술한다. 3.3장은 808에 비해 주과수 활용효율을 높여 ASSESS
가시키기 위해 QPSKS 설명한다. QPSKE 시제품을 개발하는 관점에서 보면 공유 대
역폭과 같은 몇 가지 문제점들을 내포하고 있다. 이 문제점들을 해결하기 위해, 3.43.6
장을 통해 OQPSK, MSK, 0149의 세 가지 변조방식을 소개한다. 또한 제한된 대역폭
에서의 광대역 데이터 ASS 실현하기 위한 0414방식을 3.7장에서 소개한다. 각 장에
A 이들 시스템을 컴퓨터 시뮬레이션을 통해 평가할 수 있는 방법에 대해서도 설명한
다. 마지막으로 3.8장은 간단한 정리로 이 장을 마무리한다. 이 장과 관련된 모든 프로
그램은 부록 3& 와 2220\0에서 제시된다.

ea 33

86

.1 BPSK 변조방식의 기본 구성

2
변조방식에서는, 입력 디지털 데이터 0이나 1은 위상 0이나 xz 각각 변환된다.
은 다음과 같다.

SW) = Acos{2af,t+-d,}                  (3.2)

여기서 @,는정보 데이터 수열이다.

그림 3.1은 BPSK 신호 생성기법을 보여준다. 그림 3.1에서와 같이, BPSK 파의 파형
은 양극성 형태의 디지털 정보 데이터에 반송파가 곱해져서 만들어진다. 그러나 주파수
대역폭의 한계 때문에 적당한 펄스쉐이핑 필터를 통해 형태를 제어해줘야 한다. 이런
이유로, BPSK 신호 생성과정에서는 먼저 디지털 데이터가 펄스쉐이핑 필터 회로로 입
2 ©] 51, pulse-shaped 신호는 D/A 변환기에 의해 아날로그 신호로 변환되어 반송 신호
파를 곱해 RF 주파수로 상위 변환되며, 마지막으로 공중으로 전송된다.



===== PAGE 93 =====
psk 기반 디지털 변조기법 (를.

Data | Pulse                       Lit
aint   >) shaping     D/A         BPF    Transmission
| Ae) | fitter                                    signal s(t)

1
|                   Acos2zf,t

(a)
r(t)

|               |
|
Bandpass     BPF   ale 이뻐    와 Decision |.) oe.
| [filter

filter                                                    compensator] | circuit

|
Acos2zf, t              |                                                                                    }

(b)

를 그림 3.1 BPSK 전송방식에서의 (a) 송신기 (6) 수신기

수신기에서는, 수신파는 저역통과필터 BPF)S 통과하여 의사파가 제거된다. 수신
ASE 수신된 무선신호에 RF 반송주파수 신호로 곱하고 대역제한을 행하는 과정을
거쳐서 기저대역으로의 주파수 하향 변환을 행한다. 이 ASE A/D 변화기를 통해 디
지털 샘플 데이터로 변환되고 전송신호가 2880에 의해 복원된다. 0500에서는 심볼
간섭을 제거하기 위해 샘플링된 데이터가 펄스쉐이핑 회로에서 필터링된다. 마지막으
로, 필터링된 샘플 신호에서 동기화 지점이 선택된다. 이 지점에서 신호 레벨이 0보다
크면 수신된 신호는 디지털 데이터 1이, 작으면 0으로 판정 된다.

3.2.2 YEA 신호의 표기

컴퓨터 시뮬레이션 프로그램에 필요한 BPSK 전송방식에 대한 이론적인 지식에 대
해 먼저 알아보자. 전송 디지털 데이터 시퀸스는 다음과 같다.

00= 210.ㆍ aie Liat kT,))     as)

= 2. 000)                      (3.4)

87


===== PAGE 94 =====
21  최신 이동통신시스템
C

Mobife Communications using MATLAB Simulation

여기서 d,(d,: R=1,2,°"), g7(t), 7',는 각각 전송 디지털 데이터, 4 전송 디
지털 데이터의 펄스 형태 그리고 비트 지속시간을 나타낸다. 7`,의 역수가 비트 레이트
이고 a(t 델타 함수이다.

1:t=0
00) =
0 : otherwise                                 (3.5)

87(?)가 직각펄스일때,

7:
tases I,
60이  2    주

0; otherwise  2                                     (3.6)

d, g(t), 0(?) 그리고 4(?)의 BAS 그림 3.2에 보였다. 이 경우, { 2, : =1…
6}=[1.0,1,1,0.0]이고 “0? 데이터는“1”로 변환된다. 그림 3.2의 펄스 형태가 디지털 신
호로 보이지만, 주파수 영역에서 보면, 이 형태는 다른 주파수 채널에 많은 의사 신호를

방사한다.
970 &
othe ee                                            로
2             2

el ee

| ifn ey 1 | | ee 001
0004

Vv

Mid 3.2 2g-(t), ㅇ(?) 그리고 2(7)의 관계

88



===== PAGE 95 =====
psk 기반 디지털 변조기번 0),Ｌ.Ｌ

그림 3.3은 87(?)의 한 예와 °]2] Fourier 전송 값 (2,(7)를 보여준다. 그림 3.3에
보인 바와 같이, |/| 개  영역의 모든 정보를 포함하기 위해 시간 도메인에서 펄스
형태는 sine (= SO) )함수를 가져야만 한다. 이 형태는 그림 3.2와는 다르다. 이 경

우, 의사 신호가 다음 영역에 나타난다.

7:
>
2
Nyquist pulse-frequency axis                                 Nyquist pulse-time axis
1
g                         2         00!
&                       6         [| \
0
0
ch    0   iis         -37,-27,-T, 0 1, 27, 37,
27 Frequency 2s             Time

를 그림 3.3 ¢-(t)2t Fourier 전송값의 예

결국 시간과 주파수 도메인에서 의사 신호의 수를 감소시킬 수 있는 적절한 최적 형
를 가진 필터가 필요하다. 의사 신호의 수를 감소시키기 위해 널리 사용되는 필터는
Nyquist 필터이다. Nyquist 필터의 주파수 응답은 다음과 같이 주어진다 [1].

3   a

0s|f|s

aE lon fle at a) Gs 0-0) . cl] 박은
(1+@)
:              iia

Gy (f) =} co

(3.7)
89



===== PAGE 96 =====
Zé  최신 이동통신시스템

Mobile Communications using MATLAB Simulation

여기서 a= 채널 대역폭을 결정짓는 7010 인자이다.

그림 3.4는 주파수 도메인에서 Gy(F) 4714 도메인에서 임펄스 응답을 보인
다. ee off 인자 a7t 증가함에 따라 주파수 도메인에서 의사신호의 진폭은
fh ah     ~ 2844 증가한다. 반대로, 시간 도메인에서 의사신호의 Ase
lt] > 가  영역에서  감소한다. 이런 연유로 절충적인 01-0# 인자 WS 찾을 수 있다.

1          Nyquist pulse-frequency axis                                   Nyquist pulse shaping-time axis
ig                   ay             a= 0]                  :
vs                  A        a =0.54                                                                        로
3     #      N       3        PN nts he
&            4                      Ne =1 |     >   &             i
/           2      0
[27         도
+   “7     0     후     cue       SI 2T i Be Fi 2h, 37,
3          * Frequency        ,            if                                        Time
(a)                                                                     (b)

를 그림 3.4 Nyquist 필터의 구성: (a) Gy(f) (0) GyA 임펄스 응답

Nyquist 필터의 한 가지 특징은 시간 도메인에서 볼 때 nT, (n= 정수)에서 항상 0
을 갖는다는 점이다. 이런 이유로, 동기 AAS 77;,로 설정하면 이 지점에서는 하나의
심볼은 다른 심볼들을 간섭하지 않는다. ¥]S Nyquist 필터가 여러 유용한 특성을 가지
있지만 최적의 결과를 얻기 위해서 언제, 어디에 사용되어야 하는가 하는 문제가 있
다. 참고문헌 [1]은 AWGN 환경에서 동기 지점을 최대화하기 위한 최적 할당 기법에
대해 논하고 있다.

[1]에는 균일 분포 이득 Gy(f), F 0>(7)=\ 0707), Ge(f)=  게이 을
갖는 송신 및 수신 필터가 제시되어 있는데 @,(/)와 Gag A= 각각 송신기와 수신
기의 주파수 응답이다.

e

90



===== PAGE 97 =====
psk 기반 디지털 waz (를

G,(f)=G,(f)=y7  100,

1            0<|f\< 이이 8
T,
oe  of  ‘fon f\- x(1- =a) 해 <I es

이런 필터는 root) Nyquist 필터라고 불리고, 임펄스 응답 op (4) welt)
음과 같다.

870)=8,(0)

|           4a/T,
= 1 sina = 그} + 1 아즈 cos 2n0 +) Al
os   4at               [,    ae   4at               2;
6,                    2;

(3.9)

Al (3.4)와 (3.6)을 이용해, 데이터의 BPSK ASS 구성할 수 있다. 구성된 신호는 반
송주파수 신호 (예, 0086277,.7)를 Fal 변조되고 공중으로 전송된다. 전송신호는 다음
과 같다.

개

s(t) = d(t) cos 2af.t                   (3.10)

전송신호는 다중경로 페이딩과 AWGNO] 의해 오염되고 수신기에서의 수신신호는
다음과 같다.

70) = |, 4600 6960 -2000+70)                (63.11)

91



===== PAGE 98 =====
최신 이동통신시스템

92

Mobie Communications using MATLAB Simulation

여기서 hc, 2)는시간 /에서의 무선채널의 임펄스 응답이고 2(7)는 수신기 잡음
이타.

수신기에서, 수신신호는 먼저 BPFo 의해 필터링되는데 이 필터는 신호
시할 수 있을 정도로 충분한 통과대역을 가지고 있다고 가정한다. 필터링
송신기와 동일한 주파수를 갖는 반송파로 곱해진다. 그러나 송신기와 수
이의 SAS SAS 427] 워상은 다르다: 그래서 수신기에저의: 받송신호
cos (2af,+ 0{1(7))로 표시되는데 O,(t) = 반송신호의 초기 위상 값이다. 곱해진
호는 다음과 같다.

띠ㅇ

왜
된
소

Bod Ai +

at
그게
시
1
17] ^
쓰
진

i Oe ae fol

r,(t) = r(t) x cos(2af,t + 6, (t))                         (3.12)

여기서 (YEA GANS 주어진다. 간단하게 하기 위해 필터링이 없다고 가정
하면,

     cos@,(t) -—sin@,(t) \( d(t)cos2zf.t
gone rel sinO,(t) cos@,(t) I         0         | ame
=|R(t)d(0)(cos 6, (t) + n, (t))|cos 2af,t +n, (t)               (3.13)
f

R(t) 0(7?)는 각각 무선채널에 의한 ASS 위상의 APA 요동이다. 20(7)는 수신
기 잡음인데 n(t) = R(t)xn,(t)x cos2af,t+ 72>(?)로 주어지고, n,(t) 4 n (thE
각각 /, 주변의 잡음성분과 다른 잡음성분을 의미한다. 다음은 위상 0.(7)의 회전행
렬이다.

cos@,(t) -81ㅁ00,(2)
810 0,(7)  0080,(2)

식 (3.12)를 사용해서 식 (3.11)을 확장할 수 있다. 확장 값으로 LPFS 사용하면



===== PAGE 99 =====
psk 기반 디지털 변조기법 (OE

파수 ASE 제거된다.
0) = 4(R(Qd(O(cosd, (t) +7, (0)))cos 6, 0
eS                      f          :              :                  (3.14)

그후, r,(t)=ISIS 감소시키기 위해 펄스쉐이핑, 필터기반 J Nyquist 필터로 필터
gad.

r,(t) =17,(1) @ gp (0)

= => Rt) cos 6, (t) cos 6, (t)-   yd,

k=-00

(g, (0) @ ge) BS -KT,)) +5 ((c086,()® (0)
= 40000 0, (t) cos A, (t)-  sd,

-(g,(t) @gp(t) @ 5(t-kT,)) +n,(0)

(3.15)

다음으로, 필터링된 신호는 AD 변화기를 동해 샘플링 레이트 Hh (n8 8422

Nyquist 필터의 특성으로부터, t=u- T,/n( 는 정수)일 때 펄스의 최대 값을 얻
수 있다. 그러나 동기화 방법을 고려해야만 한다. 이 장에서는, 동기화 지점을 안다고
‘a 한다. 동기화 지점에서 T, 혹은 매 n 샘플마다 다음을 재 샘플링한다.

93



===== PAGE 100 =====
^  최신 이동통신시스템
C

Mobite Communications using MATLAB Simulation

마지막으로, 재 샘플링한 데이터 ×(/ ) (동기점+ 7ㆍ7) 1=0, 1, 2,…을 얻는다.
다음 문턱치 조건방정식을 사용해 수신데이터가 1인지 0인지 결정할 수 있다.

   1 (r,() > 0)
d, =
0 (r,() <0)                                (3.16)

a, @,를 비교함으로써 BERS 계산할 수 있는데 이 값은 수신기 잡음의 부피에
달려있다. AWGN3} 단일경로 레일리 페이덩 채널에서의 이론적인 BERS 다음과 같
다고 알려져 있다 [13].

1
BER ppsx-awon = sertely E,/N, )                          (3.17)

1       1

BER ppsx-rapinc = 2  = 680
E,/N,                  (3.18)

E,/ N= 비트 당 에너지 ( £,)4 잡음 파워 밀도 NS] 비이다. 2H 3.5% BPSK
의 4\68*과 단일경로 레일리 페이딩 채널에서의 2,/ 7/,(08)과 BERS] 이론적인 관
계를 보여준다.

BPSK-performance of BER

10"

107                                                           Rayleigh theory

BER

10°
AWGN theory
10*
10°
0          5          10         15          20         25         30

E,/N, (dB)

M28 3.5 AWGNa 레일리 페이딩 환경에서의 806 ASBA S| BER 성능 (이론

적 값)

94



===== PAGE 101 =====
3.2.3 컴퓨터 시뮬레이션 프로그램

BPSK 방식의 BER 성능을 측정하기 위해 컴퓨터 시뮬레이션을 사용했다. 여기서 사
용된 모델을 그림 3.6에 제시하고 사용된 세 개의 프로그램을 다음에 보인다. 이 장에서
사용된 모든 함수들은 표 3.1에 정리되어 있다. 프로그램 3.1은 BPSKS 위한 주된 프로
그램으로서 BPSK 시뮬레이션의 과정을 설명하기 위해 이 장에서 사용할 것이다.

프로그램 3.1을 사용하기 전에, 프로그램에서 사용되는 공통 변수들을 설정해줘야
한다.

sr=256000.0; % Symbol rate
ml=1;

oe

Number of modulation levels

br=sr.*ml;   % Bit rate (=symbol rate in this case)

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=3;      % Eb/NO

IPOINT=8;    % Number of oversamples

이 프로그램을 위해 중요한 가정을 해야 한다. 3.2에서 설명되는 바와 같이, 수신기에
서 수신신호를 오버 샘플링한다. 그래서 최소시간단위는 오버샘플링 지속시간과 동일
하다. 즉 aan — be ole.

여러 변수들을 정의한 후에, 2 Nyquist Bo] 필터계수들을 설정해줘야 한다. 필터

계수는 LEA 3,29] hrollfcoef.m 함수를 이용해 계산된다. 마지막 변수를 1이나 0으
로 설정함으로써 각각 송신기나 수신기를 위한 필터를 생성한다. 송신기 필터계수를 생
성하기 위해서 다음과 같이 입력한다.

ixfn=21;     % Number of filter taps

alfs=0.5;    % Rolloff factor
[xh] = hrollfcoef(irfn, IPOINT,sr,alfs,1);

수신기 필터계수를 생성하기 위해서는 다음과 같이 입력한다.

[xh2] = hrollfcoef(irfn, IPOINT,sr,alfs,0);
필터에 대한 정보는 xh} xh2o] 저장된다.

95

Psk 기반 디지털 zz Qe


===== PAGE 102 =====
XN

최신 이동통신시스템

Mobile Communications using MATLAB Simulation

을 정의하기로 하겠다.

Pn tS
=

이하에서는 모든 프로크램에저 SSLE ASSES

% Number of simulation loops

nloop=100;

438

Joyesuedwo)

@OURLIEA 8016
ueew Joj}es0Ue6
asiou ueissneg

404

wnouto

uoisi9eg
9

joyesuadwoa

89044

(19/48084)1844 Burdeys 85100

(181414504641) sayy Buideys asing

39191809
4844
quejeninba)             [nono] _ revenuos]            1018618486
80041    ©  -Juonnjoauo9}               -dny”                  000
jeuueyd                                                                 1
이004                                u                     0

해 사용된 BPSK 전송 시스템의 모델

0 그림 3.6 BER 성능을 계산하기 위

96


===== PAGE 103 =====
Psk 기반 디지털 변조기법 《0)를

noe = 0;       % Number of error data
nod = 0;       % Number of transmitted data
9H 318 이 장에서 사용된 시뮬레이션 함수들의 개요
함수 이름             기능                 입력 데이터               출력
bpsk.m            AWGN3} 단일경로 레일리 | 무                            - BER: bit error rate
(Program 3.1)      페이딩 채널에서의 BER 4                                    성능
bpsk_fadingm | 능을 계산 (828)
(Program 3.2)
hrollcoef.m      입력 심볼과 샘플링 레이트 |ㆍ00: 필터링에 사용할 AS | -xh: 입력 심볼 또는 샘
(Program 3.3)     에 따라 root Nyquist 필터 | 의 수                       플링레이트에 따른 계
의 필터계수를 계산            ipoint: 한 심볼당 샘플의 수 | 수값
-sr: 심볼레이트
-alfs: 롤오프 계수
-nec: 1-송신 인자
0수신 인자
oversamp.m     IPOINT 배의 출력 오버샘 - indata: 입력 시퀸스       -outdata: 오벌샘플링
(Program 3.4) | 플링 데이터                  -nsymb: 입력 A) 22] 심볼 ㅣ 데이터
의수
‘sample: 오버샘플의 수
qpsk.m            AWGN>} 단일경로 레일리 | 무                            - BER: bit error rate
(Program 3.5) | 페이딩 채널에서의 BER 4                                    성능
qpsk_fadingm | 능을 계산 (QPSK)
(Program 3.6)
compconv.m      복소 신호와 BES] 컨볼루 - idata: 입력 채널 데이터     10 필터링된 채널
(Program 3.7) | AS 행함                       -qdata: 입력 채널 데이터 | 데이터
- filter: 필터 탭 계수             gout: 필터링된 채널
데이터
compoversamp.m | IPOINT 배의 오버샘플링 Ｌ | - idata: 입력 채널 데이터     -iout: 오버 샘플렁된 1
(Program 3.8)      Qa 데이터 출력           -qdata: 입력 채널 데이터 | 채널 데이터
ㆍ087006: 입력 A] A229] 심볼 |ㆍ004: 오버 샘플링된
의수                          채널 데이터

‘sample: 오버샘플의 수

97


===== PAGE 104 =====
「      최신 이동통신시스템

Mobile Communications using MATLAB Simulation

#31 (계속)
함수 이름           기능               입력 데이터                  출력
qpskmod.m        QPSK 변조의 변조 - paradata: 병렬 직렬 데이터 | -iout: HAS Ｌ채널 데이터
(Program 3.9)      데이터 출력            080: 병렬의 수                 - gout: 변조된 -채널 데이터
ㆍ00: 심볼의 수
“mil: WZ}
qpskdemod.m                             -idata: 입력 Ｌ채널 데이터       - demodata: 복조 직렬 데이터

(Program 3.10)

QPSK 변조의 복조
렴

데이터 출력

ㆍ00808: 입력 채널 데이터
para: 병렬의 수

ㆍ00: 심볼의 수

“ml: 변조의 수

comb.m              AWGN 부가            -idata: 입력 Ｌ채널 데이터        104: 1 채널 데이터 출력
(Program 2.4)                             -qdata: 입력 채널 데이터 | - gout: Q 채널 데이터 출력
-attn: 19} Q 채널에서의 잡음
As
oqpsk.m                 AWGN3>} 단일경로 | 무                                            - BER: bit error rate 성능
(Program 3.11) | ae] 페이딩 채널
oqpsk_fading.m | 에서의 BER 성능을
(Program 3.12) | 계산 (QPSK)
msk.m                   AWGN3} 단일경로 | 무                                            - BER: bit error rate 성능
(Program 3.13) | ae] 페이딩 채널
msk_fading.m     에서의 BER 성능을
(Program 3.14) | 계산 (MSK)
msk2.m               AWGN3} 단일경로 | 무                                       888: 541 error rate 성능
(Program 3.15) | 레일리 페이딩 채널
00962 fading.m | 에서의 BER 성능을
(Program 3.16) | 계산 (MSK)

oversamp2.m
(Program 3.17)

MSKe|4]_ IPOINT
배의 오버샘플링 I,
Qala 데이터 출력

ins 입력 ALAA
-ntot: 입력 Al AAs] 심볼 수
-sample: 오버샘플의 수

-out: 오버샘플링 데이터

98



===== PAGE 105 =====
psk 기반 디지털 변조기법 (를

표 3.1 (계속)
함수 이름              기능                 입력 데이터               출력
gmsk.m         AWGN3>} 단일경로 레일리 | 무                       -BER: bit error rate
(Program 3.18) | 페이딩 채널에서의 BER 성                              성능
gmsk fadingm | 능을 계산 (0549)
(Program 3.19)
gaussf.m         가우시안 필터의 형성       ㆍ: 필터계수               ‘xh: 입력 심볼 또는
(Program 3.20)           :                   0: 필터링에 사용 BAS | 샘플링 레이트에 따
의수           른계수 값
-ipoint: 심볼당 샘플의 수
- sr: 심볼레이트
-nec: 1-송신 인자
수신 인자
gam16.m        AWGN3>} 단일경로 레일리 | 무                      -BER: bit error rate
(Program 3.21) | 페이딩 채널에서의 BER ¥                                성능
qam16_fading.m | 능을 계산 (16-QAM)
(Program 3.22)
qammod.m       16-QAM 변조의 변조 데이 - paradata: 입력 직렬 데이터 | -iout: BAR La
(Program 3.23) | 터 출력                       - para: 병렬의 수                데이터
ond: 심볼 수                     -qout: 변조된 채널
ml: 변조의 수                  데이터
qamdemod.m     16-QAM 42] 2% 데이 -idata: 입력 채널 데이터     -demodata: #4 4]
(Program 3.24) | 터 출력                       -qdata: 입력 채널 데이터 | 렬 데이터

ㆍ0008: 병렬의 수
“nd: 심볼 수
700: 변조의 수

모든 변수들을 정의한 후에, BERS 얻기 위해 시뮬레이션을 실행할 수 있다. 먼저, 1-
by-nd*ml 벡터의 랜덤 데이터 (0이나 1)를 생성하고 4341이라 부른다. 2.3장에서 데이
터 생성 방법에 대해 설명하였다. 데이터 생성은 단순히 다음 명령을 입력함으로써 이

루어진다.

99


===== PAGE 106 =====
최신 이동통신시스템

Mobile Communications using MATLAB Siniujaiion

data=rand(1,nd)>0.5;

다음으로, 034의 표기를 0과 19] 디지털 데이터에서 -1과 12] 디지털 데이터로 변환
한다. 변환된 데이터는 변수 4381에 저장된다.

datal=data.*2-1;

전송될 데이터를 그림 3.7(2)에 보였다. 데이터는 다음과 ZO] pulse-shape 된다.

(이

BPSK transmission signal

BPSK phaser

0

BPSK transmission oversampled data

가
빵:

1
08
06|
oatt--
o2th------
i:
|   02}---H.-
OA} ---|
06}---
~aah---

BPSK received signal

BPSK transmission data

es
“3333335335 °

를 그림 3.7 시뮬레이션된 순간적인 BPSK 파형: (a) BPSK 전송 데이터 (b) BPSK
전송 오버샘플링된 데이터 (c) BPSK 전송신호 (0) BPSK 수신신호 (6)
BPSK phaser

100


===== PAGE 107 =====
psk 기반 디지털 변조기법 (을

0) 08181을 사용하여 (3.2)에서와 같이 최소지속시간이 1/(sr + IPOINT)
dss 트레인 AS d= 이 400- AT) & 만든다. 다음과
같이 함수 00668800016.0이 임펄스 트레인 JBAS 생성하기 위해 사용된다.

data2 = oversamp( datal, nd, IPOINT) ;

data29) 파형을 그림 3.7(4)에 보인다.
@ 임펄스 트레인 시퀸스를 생성하기 위해, 필터계수 패를 사용해 컨볼루션을 행한
다. 필터링된 데이터는 다음과 같이 주어진다.

data3 = conv(data2,xh) ;
081[33의 파형은 그림 3.7(c)9} 같다.

ASA ASE (저역통과 시스템과 동등한) 무선주파수 SS 통해 전파된다. 수신
기에서, 수신신호는 먼저 AWGNO] 의해 오염된다. 사용된 잡음 함수 comb.me 2.4장
에서 설명되었다. 시뮬레이션에서 이 함수를 사용하면 60 데이터를 입력할 필요가 없
다. 또한 변수 atnS 결정해 주어야 한다.

우리는 E,/ Nj) BERS 관계를 결정하기를 원하는데 이는 2,/ ^/,를 일정하게
유지하면서 302을 변화시켜주어야 함을 의미한다. 변수 atin 다음과 같이 계산된다.
먼저 비트 당 에너지 FS 잡음파워밀도 24;가 정의된다.

spow

= (W-Thbit)                     es
_ npow
N, = ee      (W/Hz)                        (3.20)

o|7]A] spow, npow, 그리고 sre 각각 심볼 당 파워, AS S 잡음파워, 비트 레이

트, 심볼 레이트이다.

식 (3.19)와 (3.20)을 결합하면 다음을 얻는다.

101



===== PAGE 108 =====
ZY  최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

ere spow sr
br npow                              (3.21)
정리하면 다음과 같은 4S 얻는다.
spow sr
npow =           .
br E,/N,                              (3.22)

Ey] No& 데시벨 형식이므로, 식 (3.22)는 다음과 같이 쓸 수 있다.

Spow sr
b      AORN

10 0                         (3.23)

npow =

위 식은 220\를 계산할 수 있음을 의미한다. 이 시뮬레이션에서 0418, data2 그리고
0803는 전압으로 표현되었으므로 잡음 또한 전압으로 표현되어야 한다. 가우시안 잡
음은 ㅠ71[856와 0480780076ㅁ8886에 동일하게 정규 분포되어 있다. 그러므로

[
attn =   = el                             (3.24)

프로그램 3.194, 위 관계를 다음과 같이 표현한다.

spow=sum (data3.*data3) /nd;
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn);

800을 사용하여, A+ 데이터를 AWGN = 오염시킨다.

inoise=randn (1, length (02ㄴ23 ) ) .*attn;

data4=data3+inoise;

102



===== PAGE 109 =====
psk 기반 디지털 변조기 9

이 때, randn(a,b)= 평균 aS} 분산 6를 갖는 가우시안 잡음을 생성하는 내장 GO]
다. 수신신호 4404는 시뮬레이션 초기에 설정된 Al xh2S 갖는 FS Nyquist VBA
터링된다.

data5=conv (data4, xh2) ;

a+ conv.mS 사용하기 위해, 컨볼루션에 의한 160801000)의 시간지연을 복원해야
한다. 각 conv.m2] 시간지연은  pass amen 이다. 우리는 두 개의 600 44S
사용하므로 시간지연은110+1ㅁ00 샘플이다. 그래서 A=] irfnt IPOINT+1 04
dataSS 재샘플링한다. 시작점을 samp1°] 2} 정의한다.

sampl=irfn*IPOINT+1;

필터링된 신호 4405는 오버 샘플링된 신호이고 그림 3.7(0)와 같다. 송신된 신호를
복원하기 위해, 오버 샘플링된 신호로부터 최적 지점들을 선택해야만 한다. 그림 3.7(0)
에 보인 바와 같이 시작점으로부터 매 20147(=8)마다 0305를 재샘플링함으로써 10)
U-1 얻을 수 있다. 재샘플링된 값은 6406에 저장된다. 위 과정에서 송신신호가 복원
되었음을 이해할 수 있다. BMS ASTI] AAS 그림 3.7(6)에 보였다.

data6 = data5(sampl1:8:8*nd+sampl-1) ;

수신신호가 AWGN 의해 오염되었다면, 0806의 값은 1이나 00] 아니고, 이 값이 0
혹은 1인지 결정해줘야 한다. 이 APS 위한 문턱 값은 (3.16)에 의해 주어진다. 다음
조건 함수를 실행하기 위해 사용한다.

demodata=data6 > 0;
각 요소가 0보다 크면 12, 그렇지 않으면 0으로 간주된다.

다음으로 오류의 FS 생각해보자. 이 과정은 2.3장에 기술되어 있다. 이 시뮬레이션
에서, 송신 데이터는 040이고 수신 데이터는 60206이다.

noe2=sum (abs (data-demodata) ) ;

103



===== PAGE 110 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

nod2=length (data) ;
noe=noe+noe2;

nod=nod+nod2;
마지막으로, BERS 다음과 같다.

ber = noe/nod;

레일리 페이덩 환경에서의 시뮬레이션을 위해 프로그램 3.2를 사용한다. 프로그램
3.1과 3.2의 차이는 다음과 같다. 프로그램 3.2에서는 먼저 2.4.2장에서 설명한 페이딩
매개변수들을 설정한다. 이번 경우 단일경로 레일리 페이덩을 생성하고자 한다.

음*>****×*×*×ㅠㅠㅠㅠ Fading initialization KEKKKKKKKKKK

% Time resolution

tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp
itau = [0];

% Mean power for each multipath normal5ized by direct wave.

dlvl = [0];

% Number of waves to generate fading for each multipath.
n0=[6];

% Initial Phase of delayed wave

th1=[0.0];

% Number of fading counter to skip
itnd0=nd* IPOINT*100;

% Initial value of fading counter

itnd1=[1000];

% Number of directwave + Number of delayed wave
nowl=1;

% Maximum Doppler frequency [Hz]

fd=160;

$ flat     : flat fading: or .not

% (1>flat (only amplitude is fluctuated) ,0->nomal

104



===== PAGE 111 =====
psk 기반 디지털 변조기 《0”ㅠ

% (phase and amplitude are fluctutated)
flat =1;

위 매개변수들을 사용하여, 송신된 BPSK 신호 0303는 페이딩 시뮬레이터에 의해
요동친다.

ZRKKKKKKK KKK KK KKK KKK Fading channel KKKKKKKKKKKKKKKEK

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (data3, zeros (1, length (data3) ),itau,dlvl,thl
,n0,itnd1,nowl, length (data3),tstp, fd, flat) ;

% Updata fading counter
itndl = itndl+ itnd0;

다른 함수들은 기본적으로 프로그램 3.1과 동일하다. 프로그램 3.1 (bpsk.m)3} 3.2
(bpsk_fading.m)-& 사용하여 AWGN} 페이딩 환경 하에서의 BER 성능을 평가하기
위해서는 다음과 같이 입력하면 된다.

clear

bpsk

0

oO
ㄴㄴ

clear
bpsk_fading
시뮬레이션된 결과를 그림 3.8에 보였다.
그림 3.8에서와 같이, 시뮬레이션된 결과는 이론적인 ZL} 매우 근사하다. BPSK 방
식은 간단한 구성을 가지고 있다. 888 에 기반 한 몇 가지 변조방식이 보다 높은 주파
수 효율을 위해 제안되어 왔다. 3.3-3.7장은 대표적인 예로 QPSK, OQPSK, MSK,
GMSK 그리고 QAM-& 소개한다.

105



===== PAGE 112 =====
1  최신 이동통신시스템
에                                      A

Mobile Communications using MATLAB Simulation

Performance of QAM
1,00E + 00
BPSK AWGN theory |
                                                                      ㅁ BPSK AWGN              5
— BPSK Rayleigh theory
1.00E — =                                            o BPSK Rayleigh           —
시                                                   BPSK Rayleigh theory
 1.00E - 02
=
ㅣ
PSK AWGN th
1.00E - 03               at              ou
|           가
1.00E - 04 0                   10                   20                   30                  40                  50                 60
E,/N,(dB)

를 그림 3.8 AWGN2 페이딩 환경 하에서 BPSKY| 이론적, 시뮬레이션 BER 성능

| 3.3 | oPsk

3.3.1 직교변조방식의 기본 구성

QPSK 신호는 두 개의 BPSK 신호로 생성된다. 두 ASS 구분하기 위해 두 직교 반
송신호가 사용되는데 하나는 600622/7,?이고 다른 하나는 652ㅁ277,/이다. 두 반송신호
는 한 주기의 영역에서 직교한다.

호 cos 27f,t x sin 2af,t = 0                               (3.25)

이때 TS 반송신호의 주기이고 반송주파수와 다음 WAS 갖는다.

f,=

is
T.

106



===== PAGE 113 =====
Psk 기반 디지털 변조기본 (를

cos2af,t 과 sin2zf,t & 사용하여 QPSK 신호를 다음과 같이 표현할 수 있다.

1                        1          :
s(0) = ed, (eos(2af.1) + Fedo (t)sin(2af.t)        (3.26)

cos 2f,t 7} 반송신호로 사용된 채널은 ㅠㅁ0856 채널 혹은 Icho]z} 불리고, 반송신
호로 sin2f.t 7} 사용된 A'S & quadraturephase 채널 혹은 Qcho]z} 불린다. 그래서
@,(?)과 26(?)는 각각 10과 의 데이터를 나타낸다. 10과 008을 사용하는 변조
방식을 직교변조방식이라 부른다: 기본 구성은 그럼 3.9e] 보였다.

이 시스템에서 입력 디지털 데이터 d,: 4=1, 2,…는 먼저 두 채널 Ich3} Qch] 병
렬 데이터로 변환된다. 각 데이터는 2,(?)과 26(7)로 표현된다. 데이터는 맵핑 회
로 블록을 사용해 할당된다. 그 뒤에, Icho] 할당된 데이터는 Ich] 펄스쉐이핑 필터
를 사용해 필터링된다. ©] pulse shape 41S D/A 변화기에 의해 아날로그로 WSS]
고 cos2af,t 반송신호로 곱해진다. Qcho] 할당된 데이터 역시 펄스쉐이핑 필터로 필
터링된다. 04196794806된 신호는 D/A 변화기에 의해 아날로그로 변환되고 6ㅁ227,.7
반송신호로 곱해진다. 그런 다음 10과 Qch ASE 더해져서 전파된다.

수신기에서, 수신파는 먼저 BPFS 통과하는데 여기서 의사파들이 제거된다. 그 뒤,
PALAIS RF 반송주파수를 곱함으로써 기저대역으로 하위-변환된다. 10과 0208에
각각 606[277.7+ 0,(t)]S sin[22f,t+ 0,(?)]를 사용하는데 여기서 0,(?)는
주파수 소스의 위상잡음이다. 다음으로 10과 Qcho] 모두, 주파수 하향 변환된 ASE
AD 변환기를 통해 디지털로 샘플링되고 이 디지털 데이터는 DSPH= 입력된다.
106에서는 ISIS 제거하기 위해 샘플링된 데이터를 펄스쉐이핑 필터로 필터링한다.
그 뒤 신호는 동기화되고 전송된 디지털 데이터가 복원된다.

3.3.2장에서는 직교변조방식에 기반 한 여러 변조방식에 대해 논한다.

'

×

r

pe

107


===== PAGE 114 =====
TLAB Simisation

ommunications using MA

1“

Mobile

1010
uoisi9aq

Joyesuadwoo
asing

ynoIND

Buiddewaq
ynauid} fsoyesuadwoa
uoisioeq               asing

a/v
(77S2)us

JOylys
85640 7/2

(0°}2:2)s09
an

309

309

1737 us
070 버

Jaylys
85640 2/1

7920500

\/0 1

yng
Buiddeyy

soyesaueb
0160

직교변조방식의 기본적 구성

를 그림 3.9

108


===== PAGE 115 =====
psk 기반 디지털 변조기법 (를

3.3.2 QPSK 변조방식의 기본 구성

QPSKE 기본적으로 그림 3.9에 보인 구성과 QPSK] 특화된 몇 가지 블록들을 사용
하는데 4A (mapping), 디맵핑(0604820108), 펄스쉐이핑(0418668820008)이 그것이다.

맵핑과 디맵핑을 위해서, 그림 3.10에 보인 간단한 회로를 사용한다. 펄스쉐이핑을
위해서는 3.2.2장에서 설명한 = Nyquist BE] S 사용한다. 4\0치과 단일경로 레일리
페이덩 환경 하에서 이론적은 88 값은 [2]에서 제시된 QPSK 전송방식을 갖는다.

76000     Ich data
A
d,       d,
ad
d(t)               Input data                                                                            이            :
A
mar     a). +e  {          $7 at ar or: ar
d, | d,   d, | d,    t
Qch\t)     Qch data
0 7 27. 37 4T ST G77 06              A
d,            d,
>
d, | d,        t
0   ar 4F   07 3
를 그림 3.10 QPSKO 맵핑 회로 Js
]
BER opsx-awon = ~erfo{ E,/N 주
2"                 (3.27)
1|11-    i
BER opsx-rapinc = =               1
2     1+
E,IN,           (3.28)

레일리 페이덩 환경에서의 시물레이션에서, 주파수 회전은 보상된다고 가정한다.

109



===== PAGE 116 =====
ZY 최신 이동통신시스템
C

Mobite Communications using MATLAB Simulation

3.3.35 컴퓨터 시뮬레이션

QPSK] BER 성능을 시뮬레이션하기 위해 사용한 BAS 그림 3.11에 제시한다. 그
림 3.11과 3.6을 비교해보면 직교변조가 BPSK WAS} 어떻게 다른지 알 수 있다. 직교
변조에서는 10과 Qch9] 두 시뮬레이션의 흐름이 존재한다.

om
38     3
és     zs
몰           캐최비
코르            ~
2333    Seis
223%    내
|
을     238s
s22es      pee
      Ha
883s
a
fifa (ells
Z  s  ‘So   5 om =
zs 3         ze
egies      a    es
=   zs =
를
내

를 그림 3.11 BER ASS 시뮬레이션하기 위해 AVS 직교변조방식의 모델

110



===== PAGE 117 =====
Psk 기반 디지털 변조기번 (를

이들 각 흐름의 시뮬레이션은 독립적이고 888의 시뮬레이션과 동일하다. 그래서
시뮬레이션 자체는 이해하기 수월하다. 시뮬레이션 프로그램은 프로그램 3.53.10에
해당한다. 주된 프로그램인 프로그램 3.5에서 먼저 프로그램 전체에서 사용될 공통 변

FES 결정한다.
sr=256000.0; % Symbol rate
ml=2;          % ml:Number of modulation levels
bresr.-.* mis   % Bit rate
nd = 1000;     % Number of symbols that simulates in each loop
ebn0=3;      % Eb/NO
IPOINT=8;    % Number of oversamples

다음으로 Nyquist 필터의 필터계수를 결정한다. 이 과정은 BPSK) 사용된 것
과 동일하다 (3.2.3장 참조).

그 뒤, BPSK4] 3} 같이 프로그램에서 사용될 공통 변수를 정의한다 (3.2.3장 참조).

모든 변수들을 정의한 후에, BERS 얻기 위해 시뮬레이션을 a" 있다. 먼저, 1-
bynd*ml 벡터의 랜덤 데이터 0 혹은 1을 생성하고 0301이라 부

datal=rand(1,nd*ml)>0.5;

전송신호는 그림 3.12(2)에 보인다.

Hels, 벡터 datalS 맵핑 회로에 입력하는데 여기에서 사전 정의된 맵핑을 따라
A 직렬 데이터가 두 채널 10과 0애의 병렬 데이터로 변환된다. 그 뒤
compoversamp.m-<= 사용하여, 두 채널에서의 데이터가 오버 샘플링되고 펄스쉐이핑
필터를 사용할 수 있도록 임펄스 트레인 AAA 입력된다. BAAS 째로 컨볼루션
하여 임펄스 트레인 AAAS 생성한다. 시뮬레이션 프로그램은 다음과 같이 동작한다.

[ich, qch]=qpskmod (datal,1,nd,m1l) ;

{ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ich1,qchl, xh) ;

이 과정에서, compoversamp.m< oversamp.m2] 확장이고, compconv.m-< comv.m

111



===== PAGE 118 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulaiion

의 확장이 된다. 순간 파형 101과 qch1 & 그림 3.1206)와 (0)에 보인 바와 같다.
필터링된 신호는 전파되고 (저역통과 시스템과 동등한) 무선주파수 채널을 통과하
여 수신기에서 수신된다.

\-channel
0

QPSK phaser

QPSK transmission oversampled data(Q)

1

08

06

04

0.2

0
Bry) | ee eer eee
4  -
06
08

-1

QPSK received signal(Q)

_QPSK transmission oversampled data(|)

16 18 2

14

10 12

Time
(a)
OPSK received signal(!)

QPSK transmission data

@ 그림 3.12

112



===== PAGE 119 =====
Psk 기반 디지털 변조기번 On

수신기에서 수신신호는 먼저 4\6쩌에 의해 오염된다. 잡음함수 comb.me 2.4.1장
에서 기술되었다.

E,/ 과 BERS] 관계를 알아보기 위해서는 ,/ ^/,를 상수로 고정하고 402을 변
화시켜보면 된다. A+ attn-2 8828또에서와 동일하게 계산된다 (3.2.3장 참조).

800과 60006.2을 사용해서, 전송 데이터를 AWGN? = 오염시킨다.

{ich3,qch3]= 0000 (1002, 00927 653) ;

Comb.m-< 2.4.1장에 기술하였다. 다음으로, 수신신호 143과 4083은 Nyquist 4
터로 필터링되는데 여기서 수신 데이터는 계수 xh29} 상관된다.

[ich4,qch4]= compconv (ich3,qch3,xh2) ;

ich49} qch42] 파형은 그림 3.12(0), (6)와 같고 위상은 그림 3.12(#와 같다. 3.2.34}
에서 언급된 바와 같이 conv.mS 사용하면 컨볼루션에 의한 시간지연을 복원해줘야 한
다. 한번엔, conv.m= 필터 탭의 길이의 반에 해당하는 지연을 야기한다. 이 경우, 탭의
길이는 (10 *1001341)/2이다. 근 Nyquist 필터를 사용하기 때문에, 600ㅁㅁ은 두 번 사
용된다. 결국 AZIZ) GS irfn* POINT 샌플이고 A] 214 syncpointS 정의할 수 있다.

syncpoint=irfn*IPOINT+1;
다음으로 144와 qch4% IPOINT 레이트로 재샘플링되고 10415와 4085로 변환된다.

ich5=ich4 (syncpoint: IPOINT: length (ich4) );
qch5=qch4 (syncpoint:IPOINT: length (qch4) );

리샘플링된 데이터는 복조 함수로 입력된다.
[demodata]=qpskdemod (ich5,qch5,1,nd,m1) ;

다음으로 오류의 수를 계산한다. 이 과정은 2.3장에 설명되었다. 이 시뮬레이션에서
송신 데이터는 080이고 수신 데이터는 42407이다.

113



===== PAGE 120 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation

noe2=sum (abs (datal-demodata) ) ;
nod2=length (datal) ;
noe=noet+noe2;

nod=nod+nod2;
마지막으로 BERS 다음과 같다.
>> ber = noe/nod;

Performance of QPSK
1.00E + 00                                                          ee eee          ee

— QPSK AWGN (Theory)

o QPSK AWGN (Simulation)
— QPSK Rayleigh (Theory)

© QPSK Rayleigh (Simulation)

ec
님 1.006- 02        i ed a

=
1.00E — 03               eee ee!
=
N\
‘y

에
1.00E — 04                                                 a8                                      :
0                 10               20               30                40                50               60
E/N, (dB)

LOU

1.00E — 01

가역

를 그림 3.13 AWGN 단일경로 레일리 페이딩 환경 하에서의 BER
성능의 이론적 값과 시뮬레이션 값

그림 3.13에 보인 바와 같이, 시뮬레이션 결과는 이론적인 값과 매우 유사하다. 레일
리 페이딩 환경에서의 시뮬레이션을 위해서는 프로그램 3.6을 사용할 수 있는데 이는
프로그램 3.5에 페이딩 매개변수와 시뮬레이터를 첨가한 것이다.

114



===== PAGE 121 =====
Psk 기반 디지털 변조기번 (를

| 3.4 |이23

3.4.1 OQPSKY] 기본 구성

QPSK 전송방식에서 10과 Qch2] 데이터 (27, dg) 다음 네 가지 상태를 갖는다.
A(1,1), B(L,-1), CC1, -1) 그러고 2(1, +1). 모든 7he BASS AG + 있으므로 위상
ASS 그림 3.12(#에서 보인 바와 같다. 그림 3.12(8와 같이, 위상 전이가 때로는 원점
을 통과할 수 있는데 이는 180#의 위상 변화를 의미하고 다른 위상 전이에 비해 스펙트
럼이 퍼지게 될 것이다. 원점통과를 줄이는 한 가지 방법이 028% 의 사용이다.

Mapping circuit (OQPSK)

           Ich data
Input data            ait)
sequence
dk(t)             :
ch data
eS     000)
7000    Ich data
A
ae   Input data              d,  1   8
t                      i tay CaT*
10    d,   a].
어허 띠어 ft       00000 Och data
H          A
T 27 37 4T    7787
0    3747 57 6777 8       Za
0    % | _4,      t

ana | ag AS ae ses A*

0 7 27 37 47 57 67 77 87

를 그림 3.14 OQPSKS 위한 맵핑 회로 함수

OQPSK2] 구성은 QPSKY] 구성과 거의 동일하다. 한 가지 차이점은 맵핑 회로에 있
다. 그림 3.14에 보인 바와 같이, Qoh 신호의 데이터 ASX Ich AS 반 심볼 지연된
것이다. 송신기와 수신기의 구성은 028&와 동일하다 [173]. 이런 이유로 이론적인
BER (3.27)과 (3.28)에 보인 QPSK 의 BER3} 동일하다.

115



===== PAGE 122 =====
ZY 최신 이동통신시스템
        Mobile Communications using MATLAB Simulation

OQPSK 신호를 다음과 같이 나타낼 + 있다 [1-3].

s(t) = 7k _(t)cos(2af,t) + F4o o(t -T, /2)sin(2af,, (t- T, /2))
(3.29)

3.4.2 컴퓨터 시뮬레이션
을 시뮬레이션하기 위해 사용한 모델은 그림 3.11과 프로그램

3.11의 모델과 같다. 언급한 바와 같이, 한 가지 차이점은 맵핑 회로이다. QPSKS 위한

맵핑 회로 명령은 다음과 같다.

H

[ich, qch]=qopskmod (datal,1,nd,ml) ;
[ichl,qch1]=compoversamp (ich, qch, length (ich), IPOINT) ;

{ich2, qch2]=compconv (ich1,qch1, xh) ;
OQPSK>*] 맵핑 회로를 위한 명령은 다음과 같다.

{ich, qch]=qpskmod(datal,1,nd,ml) ;

[ich1, qch1]=compoversamp (ich, qch, length (ich) , IPOINT) ;

ich21=[ichl zeros(1,IPOINT/2) ];
qch21=[zeros(1,IPOINT/2) qchl];
{ich2, qch2]=compconv (ich21,qch21,xh) ;

위에 보인 바와 Zo] 40221은 10221에서 IPOINT/2 지연된다. 이 지연은 펄스쉐이핑

후에 수신기에서 수신신호를 복조하기 위해 조절되어야 한다. QPSKAAE 다음을 Ah

용한다.

syncpoint=irfn*IPOINT+1;
ich5=ich4 (syncpoint:IPOINT: length (ich4) );
qch5=qch4 (syncpoint: IPOINT: length (qch4) ) ;

OQPSKAIA AAS 보상해주기 위해서는 다음을 사용한다.

syncpoint=irfn*IPOINT+1;

116



===== PAGE 123 =====
psk 기반 디지털 변조기법 (를

ich5=ich4 (syncpoint:IPOINT: length (ich4) );
qch5=qch4 (syncpoint+IPOINT/2: IPOINT: length (qch4) ) ;

프로그램 3.119] 명령을 사용함으로써 OQPSK ASS 얻는다. 그림 3.15(3)(6)은 =
로그램 3.11로 AS datal, 10121, 00821, 1014, qch42] 여러 순간 신호를 보여준다.

0009 phaser

OQPSK transmission oversampled data(Q)

1
08
06
04
02
0
2

saap---
06
08
a

OQPSK received signal(Q)

OOQPSK transmission oversampled data(!)

1
08
06
04
02
0
사구
-06
-08

14 16 18

OOQPSK transmission data
0 &
Time
{a)
OQPSK received signal(l)

05} 4-- +

epmyduny

를 그림 3.15 시뮬레이션된 순간 OQPSK 파형 (a) OQPSK 전송 데이터 (60) OQPSK
전송 오버샘플링 데이터) (6) OQPSK 전송 오버샘플링 데이터 (4) (0)
OQPSK 수신신호 (() (60) 0008 수신신호 (Q) (|) OQPSK phaser

117


===== PAGE 124 =====
A

최신 이동통신시스템

118

Mobite Communications using MATLAB Simulation

잡음과 페이덩이 없는 환경에서 ich4 3} qch49] 위상의 AAS 그림 3.15(4에 제시하
고 BER 성능을 그림 3.16에 보였다.

그림 3.15(6)와 (0)는 이 시뮬레이션이 오프셋 QPSKS 생성함을 보여주고, 그림
3.15(0는 OQPSK7} AAS 통과하지 SSS 보여준다. 결국 다른 채널로부터의 의사
주파수가 감소하게 된다. 비록 OQPSK7} 큰 위상 변화를 감소시키는데 유용하지만, 진
폭은 고정되어 있지 않고 요동친다[그럼 3.12H43.15 참조]. ASS 안정화시키는
한 가지 방법이 3.5장에서 기술하는 MSKS] 사용이다.

mee                                  Performance of OOPSK
— OQPSK AWGN theory
98 OOPSK AWGN
— OOPSK Rayleigh theory
1.00E - 01                =                                    © OQPSK Rayleigh
=
c
넘 1.006- 02
그
1,00E — 03
1.00E — 04
0     10    20     30     40    베     ©
E,/N, (dB)

를 그림 3.16 AWGN 단일경로 평탄 레일리 페이딩 환경 하에서 OQPSK 방식의
BER 성능의 이론적 값과 시뮬레이션 값

000 45

3.5.1 MSK 변조방식의 기본 구성

이 전송방식에서,(0088의 진폭은 진폭의 변동을 제거할 수 있도록 가중치가 주
어진다. 가중치 BRE 보통 Ich 데이터에는 606(/27`】)이고 Qch 데이터에는
810 (27 /27`,)이다. 한 가지 변화는 맵핑 회로의 구성이다 (그림 3.17). MSK ASE



===== PAGE 125 =====
PSk 기반 디지털 변조기법 (를.

다음과 같이 나타낼 수 있다 [131].

s(t) = d, (t)cos(at/2T, )cos(2af,t) + d,(t-T, /2)sin(x(t- T, /2)/2T,)
sin(2af,(t -T, /2)) = cos(2af, +b(t)z/2T + 00))

(3.30)

이때, O(t)=—d(t)dg(t)°] 2

| x el
Or le  do(t)=-1         (3.31)

AWGN3} 단일경로 평탄 레일리 페이딩에서 이론적인 비트 oF 확률은 3.273}
(3.28)에 보인 QPSK} 그것과 동일하다.

Mapping circuit (MSK}
ich data
> aie)
Lb                                       cos x27,
input data
ath       2    Qch 4
dit                                    hye                                                     jata
*                                    고                                          — pe 40
sin 53027,

를 그림 3.17 MSKIS 위한 맵핑 회로 함수

3.5.2 컴퓨터 시뮬레이션

MSKS] BER 성능을 시뮬레이션하기 위해 사용된 BAS 그림 3.11과 프로그램
3.13, 3.14에 제시한 모델에 기반한다. 여기서도 한 가지 차이점은 맵핑 회로에 있다.

119



===== PAGE 126 =====
\

최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation
MSKS] 맵핑 회로 명령은 다음과 같다.

[ich, qch]=qpskmod (datal,1,nd/2,2);
smoothl=cos (pi/2* [-1+1./4.* [0:IPOINT-1]]);     SIPOINT     point
filtering

for ii=1:length (ich)
ich2 ( (ii-1) *IPOINT+1:ii*IPOINT) =(-1) ^ (ii-1) *smooth1.*ich (ii) ;
qch2 ( (ii-1) *IPOINT+1:ii*IPOINT) =(-1) * (ii-1) *smooth1.*qch (ii) ;

end

ich21=[ich2 zeros(1,IPOINT/2) ];
qch21=[zeros (1, IPOINT/2) qch2];

위에서와 같이, qoh21-< ich21 0A] IPOINT/2 지연된 신호이다. 수신기에서 수신신
SS 복조하기 위해서는 이 지연을 펄스쉐이핑 후에 조정해주어야 한다. OQPSKS] 일
부로 다음을 사용했다.

syncpoint=irfn*IPOINT+1;
ich5=ich4 (syncpoint: IPOINT: length (ich4) ) ;
qch5=qch4 (syncpoint+IPOINT/2:IPOINT: length (qch4) ) ;

49&에서는 어떤 필터도 사용하지 않기 때문에 다음을 사용한다.
syncpoint=1;

ich5 = ich3(syncpoint+IPOINT/2:IPOINT: length (ich2) ) ;
qch5 = qch3 (syncpoint+IPOINT: IPOINT: length(ich2)+IPOINT /2);

ich5 (2:2:length (ich5) )=1*ich5(2:2:length (ich5) ) ;
qch5 (2:2: length (ich5) )=1*qch5(2:2:length (ich5) );

프로그램 3.133} 3.14에서 이 명령들을 사용함으로써 MSK ASS 얻는다. 그림
3.18(3)(60)는 프로그램 3.11을 통해 얻은 순간 Al S datal, ich, qch, 1015, qchSS 그
있다. 잡음과 페이덩이 없을 때 ichS 9} 6085에 의한 위상을 그림 3.18(8에, BER 성능

120



===== PAGE 127 =====
psk 기반 디지털 변조기법 (를

는 원점
된다.

이 시뮬레이션이 MSKS 생성하고 이 449

ㄴㄴ
uU

그림 3.199] 보였다. 그럼 3.1800

수가 감소

)

즈
~

널로의 의사

채

다. 이런 이유로 다른

을 보여준

oho
wu

ㅣ

A

하

통과

oO
=

으으
wu oD
Sco
uy
<0 70
()                             (2)                            (p)                 K in
Jeuueyd |                        eu                         oul
SIE ESR IR 0 oa   0 06 00 006 00 06    o_o,   eo uw #8 © @-e ow '     se
{   4   a      {   {        H   :   H   내일    ao
tw              Loge          bd        0 a        za
90-           ae                       Fags Gabiay seed A    그어
4   :   H        &
ig                                                  4---2be- = doy       40
ae                                             eee        KS
"월                                            PA:        를   609
v0                                    1 가    90   므
TH oy
90                                                                om ©
1                                                                   =

1065684035\

45.08
C8

f

{

0. . ee
~…ㄴ0

수 aes

Pooper

(D)evep pejdwesseno uoissimsuen YSN

(i)e1ep pajdwesieao uoisswsuen ySW

BJep UoIssiIMsUeN \SW

(Q) (f) MSK phaser

호

A
(ta

A
ta

121



===== PAGE 128 =====
최신 이동통신시스템

a

122

Mobile Communications using MATLAB Simulation

1

10

— MSK1 Rayleigh (theory)
x MSK1 Rayleigh (simulation)
—  MSK1 AWGN (theory)
3% =MSK1 AWGN (simulation) | J

10°F

25

15
67408]

10

를 그림 3.19 ^/4과 단일경로 레일리 페이딩 환경 하에서 MSK 방식의 BER 성능

의 이론적 값과 시뮬레이션 값

위의 논의에서, MSK 구성을 OQPSKS] 구성에서 접근해 갔다. 다른 접근법은 FSK
|반 전송방식에서 출발한다. MSK ASE 연속위상전이를 가진 FSK 신호로 간주되

N

는데 이는 위상의 궤적이 그림 3.18686에서와 같이 부드럽게 연속적으로 분포되어 있기
때문이다. 이 경우의 맵핑 회로의 구성이 그림 3.20에 제시되어있다. 연속위상전이를
가진 FSK 신호는 다음과 같이 기술된다.
Mapping circuit (MSK2)
Ich data
cos Olt)           > ait)
Input data
sequence      alt)
이                ee
F                 » Ach data
sin O(t)           P d,(t)
를 그림 3.20 MSk2s 위한 맵핑 회로 함수 (시뮬레이션 2)



===== PAGE 129 =====
psk 기반 디지털 변조기번 (를

s(t) = 4008(22.7+0(2))                                (3.32)
A(t) = 2ndf [' x(c)dz                            (3.33)
x(t) = 2. 20-/2;)                            ao,
이때 2(7)는직각펄스이다.
i O<tst
BOS :    otherwise                            (3.35)

정수 d,: R= 1이나ㄱ1을 갖는 데이터 A)AHo]Tf. (3.30)에 보인 FSK 신호의 파워
스펙트럼 밀도는 다음과 같다 [21.

S esx GE )  “a
T,
4            m             :            {cos(m 7) — cos(22X yy                1005 때 n)| <1
m(m* —4X*)} 1—2cos(mz)cos(22X) + cos?(mz)
1                                                             m            d                                                      3
an, {6(2X +m) +65(2X —m)}+ eral  {l-cos(mz) cos(22X)}|cos(mz)| =1,m #0

(3.36)

여기서 m=2a/T es 변조 색인이고 X(=F—LIT IS 정규화 주과수이다
MSK 신호의 파워 스펙트럼 밀도는 다음과 같다.

507: 16 fee

7;       m\ 1-167;                     (3.37)

A} (3.36)3} (3.37) 2] HE (3.36) 41 %2= 0.5로 치환하면 서로 같게 된다. 식 (3.32)

123



===== PAGE 130 =====
21 최신 이동통신시스템

Mobile Communications using MATLAB Simuflaiion

에서 (3.34)와 m=0.5S 이용해 MSK 신호를 생성할 수 있다. 그 과정은 다음과 같다.
OPS 데이터 』,를 사용하여 (3.33)으로 주어진 @(7)을다음 결과를 이용해 계산
한다.

O(KT,) - O((k -1)T,) = 2adf  30000

O(KT,) = O((k -1)T,) + 2nAf j Het x(r)dt
= O((k -1)T,) + 22AfT,d,                (-: (3.34))
= O((k -1)T,) + ait                 (m = 2AfT, = 0.5)

(3.38)

(R-1)T < tS kT BANA ORT ,) 7} 연속적으로 0((&-ㅡ-1)7`,)와 연결
되어 있으므로

ie    i.     a, t-(k-Df,
O(t) = O((k -1)T,)+—d, = ar eee            aan
@ 계산된 0(7)을 MSK 신호를 얻기 위해 (3.30)에 입력한다.
분 부호화와 동기 검출이 사용될 때 [13],

BER wsx awon = erfe(y E,/No )                      (3.40)

BER 성능을 시뮬레이션하기 위해 사용된 Bale 다시 그림 3.115} 프로그램 3.15,
3.16에 제시된 모델에 기반한다. 한 가지 차이점은 다시 맵핑 회로에 있고 FSK 기반
MSKS 위한 맵핑 회로 명령은 다음과 같다.

data2=oversamp2 (02ㄴ211 , length (datall1),IPOINT) ;

124



===== PAGE 131 =====
psk 기반 디지털 변조기법 (을

th=zeros (1, length (data2) +1);
ich2=zeros (1, length (data2) +1) ;
qch2=zeros (1, length (data2) +1) ;

for ii=2:length (data2) +1
th (1,ii)=th(1,ii-1)+pi/2*data2.(1 , 11-1) 24a PONT;

end

ich2=cos (th) ;
qch2=sin (th) ;

복조기에서, Ichz} QchE37-E] 2] 수신신호를 복원해야만 한다. 먼저, ich3Z} qch3S
ny 2018마다 재샘플링한다. 그 방법은 0088에서와 동일하다.
syncpoint = 1;

ich5=ich3 (syncpoint:IPOINT: length (ich3) );
qch5=qch3 (syncpoint: IPOINT: length (qch3) );

다음으로105는 qch5 9} 차별적으로 곱해진다.

demoddata2 (1,1)=1;
for k=3:2:nd*ml+1
demoddata2 (1,k)=ich5 (1, k) *qch5 (1,k1) *cos (pi* (k) ) >0;

end

for n=2:2:nd*ml41
demoddata2 (1,n)=ich5 (1,n-1) *qch5 (1,n) *cos (pi* (n) )>0;
end

마지막으로, 다음 과정을 통해 수신신호가 재생성된다.
[demodata] =demoddata2 (1,2:nd*m1+1) ;

프로그램 3.157} 3.16에서 이 BASS 사용하여 MSK ASS 얻는다. 그림 3.212
전송신호 [그림 3.21(3)]와 6(?)의 전이 [그림 3.2106)], 10과 Qch2] 송신신호 [그림
3.21(0)]를 보여준다. 49 의 BER 성능은 그림 3.22와 같다. 그림 3.2106)는 각 심볼 마

125



===== PAGE 132 =====
*

(시뮬레이션 2) (a) AS 데이터 (6) MSK

다. 그림 3.22는 이 시뮬레이션 프로그램이

(9)                     (9)                    (2)
yer            ou                    ewly
해       09           Cis Se aren Mae NSB 300 재해 0
=             '  ㆍ  ㆍ
ete a 애        1 eee eee a eer

S                                      '                   1         그 동    5    1어
8 빼                               시 dees” Meeeae ee | 가        trippy! B Az
Ss                                      ㆍ         '  4      Be kd        doopoe doo 4--- 470 s  x
3                                      7         4          *         개 호           <0
Poe. Ce 14713eae 200. fo          나우 Sw
ee                                        SOE: wae BE        itn 28

ae Mie   EN Sie 5      0 6 CA Me 레마 이 04 100"      rdw
5   e ms                                     벼00000, a    정과  3   HS
&   !                                     1)  4    i.  '                             one
NS  70 8       jeuBis uoissiwsuen 381    H       uoneuen aseyd ySW           6180 uoIssimsue YSW       때 o
> =                                                                     oe
3   N 70ㅁ                                                                 a 세
   더 a                                                                < OF
= a, A                                                                      z
8  ilo? cn)                                                   a
se 4 건                                                                      x
iS   76 OW                                                                     zi
eee 9                                                      7
LS)   Lo 2                                                                     시
a   <
ㆍ fe
S
 ee 수

126



===== PAGE 133 =====
Psk 기반 디지털 변조기본 (를.

10                       '                    7                ome                  ~                    7
-……~ Rayleigh fading theory

% Rayleigh fading (simulation result)
— AWGN theory

++ AWGN (simulation result)

10°             1             j           re            ,            e
0            5           10           15          20           25          30
E,/N, (dB)

@ 28 3.22 AWGNY 단일경로 레일리 페이딩 환경 하에서 MSk2 방식의 BER
성능의 이론적 aa 시뮬레이션 값 (시뮬레이션 2)

MSKE 많은 좋은 특성들을 가지고 있지만, 그림 3.21(6)에 보인 바와 같이 위상전이
에서 최대 전이가 7/2로 제한되어 있어서 변동이 부드럽지 못하다. 요동을 부드럽게
하는 한 가지 방법은 3.6장의 Gaussian MSK (GMSK)= 사용하는 것이다.

GMSK

3.6.1 GMSK9Y] 기본 구성
GMSK+ GSM 이동 전화 시스템에 채용되어 널리 사용되고 있다. GMSK*= MSK
의 확장 버전이다.449&와 같이, GMSKE 그림 3.18(4에서처럼 SS 일정하게 유지한
다. 그러나

419 와는 달리, GMSKE kT ,( &=정수) 지점에서 위상 A] (phase transition) 2
궤적을 부드럽게 유지한다.

GMSK 신호를 생성하기 위해서, 맵핑 회로를 제외하고는 MSKS} 동일한 구성을 사

127


===== PAGE 134 =====
^ 최신 이동통신시스템
C

:    Mobile Communications using MATLAB Similation

용한다. 맵핑 회로의 구성은 그림 3.239] 나타내었다. 입력 데이터는 가우시안 필터로
필터링되어 형태가 안정화된다. 필터링된 ASE FSK 기반 MSK 송신기와 수신기에
입력된다. 주파수 응답은 다음과 같다.

Mapping circuit (GMSK)

~ Ich data
Input data                                                                       cos A(t)                   P a(t)
cme
“ar   — | 00  Fe!
sin 0(t)                   ee “a
를 그림 3.23 GMSKS 위한 맵핑 회로 함수
In2( f )\
G(f) = exp seal
2 \ By                (3.41)
시간 임펄스 응답은 다음과 같다.
22          2        『
t =|/—8     ~~~ ("By jt
g(t)   in? 38 exp  ea  sab") |        (3.42)

위 식에서 2,,4는 308 대역폭이고 필터 o NE 무한시간계수를 가지고 있다. 일
반적인 경우, 가우시안 필터의 특성은 o( 1) 3의 FS 가진 ABA o (HSA
볼루션 취해 알아본다. 컨볼루션 값은 다음과 같다.

227       ta         2
yt) = gQ) Sg, = [ps0 [Sex| - 2 (Bat) far

1               2                                      2
= 리버 ea et— o} + erf 2% (t+ 까|

(3.43)
128



===== PAGE 135 =====
Psk 기반 디지털 변조기법 (를

그림 3.24는 2; 의 변화에 따른 가우시안 필터의 형태 변화를 보여준다. GMSK 전
송의 BER 성능은 다음과 같이 계산된다.

BER ousx_awon (E; / No) = erfe(/B -E,/N, )           (3.44)

Amplitude

077

를 그림 3.24 Boy 변화에 따른 가우시안 필터의 변화

3.6.2 컴퓨터 시뮬레이션

GMSK¢] BER 성능을 시뮬레이션하기 위해 사용된 모델은 그림 3.11에 기반하고
가우시안 필터를 제외하고는 MSKS] 프로그램과 동일하다. 주된 프로그램은 프로그
램 3.18과 3.19이다. GMSKol]A] 변화한 부분은 “HHH New for GMSK ##f’2}51 표시
얻는다, 그림 3.25(2)(0)는 프로그램
그림 3.25(6)에서, BER 성능을 그림 3.26에서 볼 수 있
129



===== PAGE 136 =====
\

최신 이동통신시스템

130

Mobile Communications using MATLAB Simiation

다. 그림 3.26 이 시뮬레이션이 GMSKS 생성함을 보이고, 3.25(6)는 GMSK7} 원점
을 통과하지 않고 진폭이 일정함을 보여준다. 그림 3.25(0)는 위상 전이가 매우
움을 보여준다. 이 시스템이 무선 채널에서 전송률을 높이기 위한 강력한 수단이기는

하지만 다른 방향으로도 생각해 봐야만 한다.

3
3
3
f-     3
eo
st.      =
=
oh     3
=
SE

^:
-1 -08 -06 -04

GMSK transmission signal

GMSK transmission data

"33

04
02
0
02
-04
-06
-08
-1

부드러

를 그림 3.25 시뮬레이션된 순간 GMSK 파형 (a) GMSK 전송 데이터 (6) 가우시안 필

터링 후 GMSK 전송 데이터 (0) GMSK 위상 변화 (0) GMSK 송
(6) GMSK phaser

NA

tz

신호



===== PAGE 137 =====
66( 기반 디지털 변조기본 ㅅ0),Ｌ.

10"                      ㅜ                    T                     T                    T                    T

—— Rayleigh fading theory (BT =0.5)
Rayleigh fading BT = 0.5 (simulation result)

—— AWGN theory (BT = 0.5)

+ AWGN 87=0.5 (simulation result)

0          5          10          15          20          25          30
E,/NJ{dB)

를 그림 3.26 AWGNa} 단일경로 평탄 레일리 페이딩 환경 하에서 GMSK 방식의 BER
성능의 이론적 값과 시뮬레이션 값

3.7장에서는 높은 주파수 활용도를 유지하면서도 전송률을 증가시키는 방식을 소개
한다.

099 cam

3.7.1 QAMY] 기본 구성
QPSK 기반 변조장식에서는 두비트 (285,, Gong): 4=1, 2,…가심볼 시간 T,
동안 전송될 수 있다. 파형은 다음과 같다.

s(t) =d ,(t) cos(27f,t) +d o(t) sin(2f,t)                     (3.45)

이때 d(t) 2 do(t)= 각각 Ichy} 0애의 AS 진폭이다.

131



===== PAGE 138 =====
최신 이동통신시스템

Mobie Communications using MATLAB Simulation

QAM 전송방식에서 과 Qch2] ZL 보다 많은 비트를 사용해 결정된다. 그
림 3.27(3)(0)는 QAM, 16-QAM, 64-QAM, 256-QAM4] constellation S 보여준다.
이 책에서는 22" QAM] 집중한다. 이 이 심볼 시간 동안 22" 비트

(020+17''', 2om+on) = ASU. 이때 가장 중요한 요소는 어떻게 진폭에 전송 비
트를 할당하는냐 하는 문제이다.
a               a
ㅣ               ㅣ
(a)              (b)
a               Q

(이                        (d)
를 22 3.27 Constellation (a) QAM (6) 16-QAM (c) 64-QAM (0) 256-QAM

는 한예로 2 QAM (n=, 2, 3, 4)를 위한 Gray 부호화에 대해 소개한다.

장에서
에는 3단계가 존재한다.

이장
이 방법

Dien 41s 1% Bom +n) 7 Toe 분류한다. 00000 12880; Bom + /)과

&(Gom+ n+1l9°"">  Bom+2n)

132



===== PAGE 139 =====
Psk 기반 디지털 변조기 (를

@ 두 그룹에 다음 두 계산을 행

oo

다

a,(k) = 가 ×28
jal

(3.46)
aig (k) = Yamane) X2"
s    슴 ss                (3.47)
@) 다음 변환 맵을 사용하여
-1  1  0  0  0.4.0  0  Ox O07 Oke 0-0-0 0
pas -3 -1  3  1  O20  0  020-20: 0: 0 0 0 0-0
ee, eee meee Cee 00025 1 3 .30-43)>5~0 0 0000
-15 -13 -9 -11 -1 -3 -7 -5 15 13 9 11 13 7 5
(3.48)

22” QAM (n=1, 2, 3, 4)2] in-phase} quadraturephase 채널의 진폭을 결정할 수
있다.

d,(k) = C(n,a,(k) +1)/ 2? :                  (3.49)

=                 07512

do (k) = C(n,ag(k) +1)  2                         ane

Al (3.45), (3.49), (3.50) 사용하여 Gray 부호화된 22" QAM 신호를 생성할 수 있

다. 또한 역 과정을 통해 ASS 복조하고 전송 데이터를 복원할 수 있다. 4\0씨과 단

일 경로 레일리 페이딩 하에서의 2?” QAM ( n=1, 2, 3, 4)의 이론적인 BERS 다음과
같다고 알려져 있다 [1-31.

3        12               9           12
BER sont anonEs/N)= Zen 26. }-Zeste| 26. |

(3.51)
133


===== PAGE 140 =====
Mobile Communications using MATLAB Siniuiaiion
고             1                   49              1
BER gagam awon (Ey / No) = 그쳐   7 /No | Sar   (E 7 E,/ Ng  |

(3.52)
1                 225 .           4
BER outann (Es!) = Ser |,  85       iv, }-   7048 °     |  260 /N ]
(3.53)

1
V1+5/(2E,/N,)|  (3.54)

Ss
BER j¢gam FADING (E,  IN, = = a

7        1
BER        E,/N,)=—|1-
64QAM_FADING ( »/ No)  |   1+7(E,/No) |   (3.55)

15                     1
BER 9 sqm_FADING (E,/No)= 나 내

J1+85/(4E, =|   (3.56)

레일리 페이덩에서 주파수 회전은 보상되었다고 가정한다.

3.7.22 컴퓨터 시뮬레이션

컴퓨터 시뮬레이션을 통해 22” QAME] BERS 계산했다. 이 장에선 대표적인 예로
n= 2 (16QAM)9] 경우를 다룬다. 사용된 BAS 그림 3.11에 제시되었다. 프로그램
은 프로그램 3.21-3.24이다.
QPSK 모델과의 차이점은 맵핑과 디맵핑에 존재한다. 088에서 YY 희로는 다음
과 같았다.
[ich, qch]=qpskmod (datal,1,nd,m1) ;

[ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
{ich2,qch2]= compconv (ich1,qch1, xh) ;

134



===== PAGE 141 =====
psk 기반 디지털 변조기법 (를

QAMS] 맵핑 회로는 다음과 같다.

[ich, qch] =qammod (datal,1,nd,m1) ;
[ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ich1,qch1, xh) ;

시뮬레이션은 복조과정에서 다른데 QPSKE 다음을 사용하고
{ich, qch]=qpskmod (datal,1,nd,m1l) ;

QAMAAT = 다음을 사용했다.
[ich, qch]=qammod(datal,1,nd,m1l) ;

프로그램 3.21과 3.22] 이들 BAS 변화시킴으로써 16(04)4 신호를 얻었다. 그
림 3.28(2)(6)는 Z}Z datal, 1011, 0001. 1085, qch52] 순간 신호를 보여준다. 잡음과 페
이덩이 없는 환경에서 145와 4085의 위상 AAS 그림 3.28(#에 보였다. 그림 3.29에
보인 바와 같이, 시뮬레이션된 BERS 이론적인 값과 매우 유사하다.

135



===== PAGE 142 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

’    '   '
르기

Tt
{
ee eee ers ery

Time
(이
16-QAM
-0.5

T
'

15

16-QAM transmission oversampled data (0)

1
a.

Time
(e)

fr---B--

16-QAM received signal (Q)

qe---

16-QAM transmission oversampled data (1)

:        z

등          '

을                             Cy Re어도 3

8        3 :

€        |; 이 기      ae

2        기 eaespoofs ks eee Laees

3        je

z        Z|seesTea aera, Saati 8

1        Pd haceye « gape atu hata더
oieeo eee

.        ee eS ee

epnyjdury 1

를 그림 3.28  시뮬레이션된  16-QAM 순간 파형 (a) 16-QAM 전송 데이터 (6) 16-QAM 전
송 오버샘플링 데이터 (I) (6) QAM 전송 오버샘플링 데이터 (0) (0) 16-
OAM 수신신호 () (6) 16-QAM 수신신호 (0) (f) 16-QAM

136



===== PAGE 143 =====
PSk 기반 디지털 변조기번 (를 -

Nh. ~ ~ ~ ~     +          ;     —

— 16-QAM Rayleigh (theory)
a 16-QAM Rayleigh (simulation)
— 16-QAM AWGN (theory)

; eran 베 1

1.00ㄷ- 01                                                 © 16-QAM AWGN (simulation) §
as
c
Gi 1.00E — 02                                =
=
x
어레
1.00E — 03                                           8
글                                 >
{                                   xX
1.00E — 04                     ti                                    =
              0               10               20              30              40              50              60
E,/N, (dB)

를 그림 3.29 AWGNa 단일경로 평탄 레일리 페이딩 환경 하에서 16-QAM 방
식의 BER 성능의 이론적 값과 시뮬레이션 값

| 3.8 es

이 장에서는 6712] PSK 기반 디지털 전송방식 BPSK, QPSK, OQPSK, MSK,
GMSK, 0404에 대해 기술했다. 각 전송방식의 기본 구성과 송ㆍ수신기의 특성에 대해
설명했고 컴퓨터 시뮬레이션으로 평가하는 방법에 대해 설명했다. 이 변조방식들은 모

든 변조 방식들 중에서 가장 기본이 되는 것들이다. 다음 장에서는 이들 변조방식을 사

137


===== PAGE 144 =====
최신 이동통신시스템

C         Mobile Communications using MATLAB Simulaiion

1) Sampei, S., Applications of Digital Wireless Technologies to Global Wireless Communications,
Upper Saddle River, NJ: Prentice Hall, 1997.

2) Prasad, R., Universal Wireless Personal Communications, Noerwood, MA: Artech House, 1996.
3) Proakis, J. G., Digital Communications, 3rd ed., New York : McGraw-Hill, 1995.

138



===== PAGE 145 =====
Treo |

프로그램 3.1
% Program 3-1
% bpsk.m
%
% Simulation program to realize BPSK transmission system
%
% Programmed by H.Harada and T.Yamamura,
%

ZRKKKKKKKK KKK KK KKK Preparation part KKKKKKKKKKKKKKKKKKKK

sr=256000.0; % Symbol rate

ml=1;        % Number of modulation levels

br=sr.*ml;   % Bit rate (=symbol rate in this case)

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=3;      % Eb/NO

IPOINT=8;    % Number of oversamples

Bk OK RK RK RK Filter initialization KKEKKKKKKKKKKKKK

irfn=21;     % Number of filter taps

alfs=0.5;    % Rolloff factor

[xh] = hrollfcoef(irfn, IPOINT,sr,alfs,1);
$Transmitter filter coefficients

[xh2] = hrollfcoef (irfn, IPOINT,sr,alfs,0);
SReceiver filter coefficients

GREKKKKKKKKKKKKK KKK START CALCULATION KEKKKEKKKKKKKKKKKKK
nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod   Os    % Number of transmitted data

ㅣ

for iii=1l:nloop

Bw KR RK KK RK Data generation KKKKK KEKE KKK KKKKKKEKKKK

139



===== PAGE 146 =====
\

최신 이동통신시스템

C        Mobile Communications using MATLAB Simulaiion

data=rand(1,nd)>0.5; % rand: built in function

ZREKKKKKKKKK KKK KKK BPSK Modulation KKKKKKKKKKKKKKKKKKKKK

datal=data.*2-1;
[data2] = oversamp( datal, nd, IPOINT) ;
data3 = conv(data2,xh); % conv: built in function

ZREKKKKKK KKK KK KKK Attenuation Calculation KKKKKKKKKKKKK

spow=sum(data3.*data3) /nd;
attn=0.5*spow*sr/br*10.%* (-ebn0/10) ;
attn=sqrt (attn) ;

ZRKKKKKKK KKK KK KKK KKK Fading Channel ** KK KKKKKKK KKK KK KKK

% Generated data are fed into a fading simulator
% In the case of BPSK, only Ich data are fed into fading counter
%
[ifade, qfade]=sefade (data3, zeros (1, length (data3)),itau,dlvl,th1,n0
,itndl,nowl, length (data3),tstp, fd, flat) ;

% Updata fading counter
Sitndl = itndl+ itnd0;

GxxxxxexKkK* Add White Gaussian Noise (AWGN) ********k*e*

inoise=randn(1,length(data3)).*attn; % randn: built in function
data4=data3+inoise;
data5=conv(data4,xh2); % conv: built in function

sampl=irfn*IPOINT+1;
data6 = data5(sampl:8:8*nd+samp1-1) ;

ZK KR KK KK KK KK KK KK KK BPSK Demodulation KKK KKK KK KK KKK KK KKK

demodata=data6 > 0;

Sk OR RR RK KK RK KR Bit Error Rate (BER) KKKKKKKKKKKKK KKK

noe2=sum(abs (data-demodata)); % sum: built in function
nod2=length(data); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

140



===== PAGE 147 =====
fprintf ('Sd\t%e\n',iii,noe2/nod2) ;
end % for iii=l:nloop

BRR KKK KK RK KK RK KK KK KK Output result KKEKKKKKEKKKKKKK KKK KKK

ber = noe/nod;

fprintf ('Sd\t%d\t%d\t%e\n',ebn0, noe, nod, noe/nod) ;

fid = fopen('BERbpsk.dat','a');

fprintf (fid, 'd\t%e\t%f\tsf\t\n',ebn0,noe/nod, noe, nod) ;
fclose(fid) ;

ZRKKKKKKKKKKKKKKEKK ANd Of File KKKKKKKKKKKKKKKKKKKKKKKK

프로그램 3.2

% Program 3-2
bpsk_fading.m

ae

00 00

Simulation program to realize BPSK transmission system
(under one path fading)

00

ole

00

Programmed by H.Harada and T.Yamamura,

oe

ZK KK KR KK KR RK KR KR KK Preparation part KKEKKKKKKKKKKK KKK KKK

sr=256000.0; % Symbol rate

ml=1;        % Number of modulation levels

br=sr.*ml;   % Bit rate (=symbol rate in this case)

nd = 100;    % Number of symbols that simulates in each loop
ebn0=10;     % Eb/NO

IPOINT=8;    % Number of oversamples

Ze KKK KK KKK RK RR KK Filter initialization KKKEKKKKKKKKKKKK

irfn=21;     % Number of filter taps

alfs=0.5;    % Rolloff factor

[xh] = hrollfcoef(irfn, IPOINT,sr,alfs,1);     STransmitter filter
coefficients

[xh2]   = hrollfcoef(irfn, IPOINT,sr,alfs,0);     SReceiver filter
coefficients

Zk KKK KK KR KK KK Fading initialization *****KKKKKKKKKKK

141



===== PAGE 148 =====
최신 이동통신시스템

Mobie Communications using MATLAB Simulation

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 2-8.

% Time resolution

tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp
% If you would like to simulate under one path fading model, you have
only to set

으

% direct wave.
itau = [0];

% Mean power for each multipath normalized by direct wave.
% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

01371 = [0];

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave

% In this simulation fourpath Rayleigh fading are considered.
th1=[0.0];

% Number of fading counter to skip
itnd0=nd* IPOINT*100;

oe

Initial value of fading counter
In this simulation onepath Rayleigh fading are considered.
Therefore one fading counter are needed.

00 00

itnd1=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered

142



===== PAGE 149 =====
Treo f

nowl=1;

% Maximum Doppler frequency [Hz]

% You can insert your favorite value
fd=160;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1>flat (only amplitude is  fluctuated),0->>nomal(phase and
amplitude are fluctutated)

flat =1;

BRK KK KK KKK KK KK KK RK START CALCULATION KKKKKKKKKKKKKKK KKK
nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop
Zw KR KR KR KK KR RK KK KK KK KK Data generation KREKKKEKKKKKKKKKKKKKKK

data=rand(1,nd)>0.5; % rand: built in function

ZRKKKK KKK KK KK KKK KEK BPSK Modulation KaKKKKK KKK KKK KK KK KKK

datal=data.*2-1;
[data2] = oversamp( datal, nd , IPOINT) ;
data3 = conv(data2,xh); % conv: built in function
ZREKKKKKKKKKKKKK Attenuation Calculation KARR KKK KKK KK KK
spow=sum (data3.*data3) /nd;
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn) ;

ZR KKK KK KKK KKK KK KK KKK Fading Channel **RKKKKKKKKKKKKKKKK

% Generated data are fed into a fading simulator
% In the case of BPSK, only Ich data are fed into fading counter

143



===== PAGE 150 =====
최신 이동통신시스템
Mobile Communications using MATLAB Simulaiion

[ifade, qfade]=sefade (data3, zeros (1, length (data3)),itau,dlvl,th1,n0
,itnd1,nowl1, length (data3),tstp, fd, flat) ;

% Updata fading counter
itndl = itndli+ itnd0;

GRRKKKEAEKK AG White- Gaussian, Noise. (AWGN) .******exenx*

inoise=randn(1,length(ifade)).*attn; % randn: built in function
data4=ifadet+inoise;
data5=conv(data4,xh2); % conv: built in function

sampl=irfn*IPOINT+1;
data6 = data5(samp1:8:8*nd+sampl-1) ;

ZR KKK KKK KK KKK KKK KK BPSK Demodulation KKKKKKKKKKKKKKKEKKK

demodata=data6é > 0;

ZREKKKK KKK KK KKK KK KK Bit Error Rate (BER) KAEKKKKKKKKKKKKK

% count number of instantaneous errors
noe2=sum (abs (data-demodata)); % sum: built in function

% count number of instantaneous transmitted data
nod2=length(data); % length: built in function

noe=noe+noe2;
nod=nod+nod2;

fprintf ('%d\t%e\n', iii,noe2/nod2) ;
end % for iii=1:nloop

ERK KKK KKK KKK KK RK RK KK Output result KKKKKKKKKKKKEKK KKK KKK

ber = noe/nod;

fprintf ('td\t%d\t%d\t%e\n', ebn0, noe, nod, noe/nod) ;

fid = fopen('BERbpskfad.dat','a');

fprintf (fid, 'td\t%e\tsf\tsf\t\n',ebn0,noe/nod, noe, nod) ;
fclose (fid);

ZR KKK KK KKK KK KK KKK end of file KKKKKKKKKEKKKKKKKKK KKK KKK

프로그램 3.3

144



===== PAGE 151 =====
ses, [를

% Program 3-3
hrollfcoef.m

Generate coefficients of Nyquist filter

programmed by H.Harada

function [xh] = hrollfcoef(irfn,ipoint,sr,alfs,ncc)

ZK KK KK RK KK RK KK KK KK  variables  KKKKKKKKKKKKKKKK KKK KKK KKK

% irfn       : Number of symbols to use filtering

% ipoint : Number of samples in one symbol

% sr     : symbol rate

% alfs   : rolloff coeficiense

% nec    : 1 - transmitting filter 0 - receiving filter
옹  ㅠ*×**×ㅠㅠㄴㅠㄴㅠ×ㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㅠㅠㄴㅠㄴㅠㄴㅠㅠㅠㅠ 항행 하강 강가 가가바바가가가바가가가차차바가차차가하하하

xi=zeros (1,irfn*ipointt1) ;
xq=zeros (1,irfn*ipointt+l) ;

point = ipoint;

Cy -= sr ;

tstp.= 1.0../ tres/ ipoints

n= ipoint.. *-ifin;

Mid Son. 2.) eae

subl= 4.0. *: albandg* tre          % 4*alpha*R_s

LOY d= 주회

10058 ㅋ 1 ^ mdz
ym = icon;

if icon == 0.0
xt = (1. 0-alfs+420.*altse/pi)i* tr? 18000)
else

sub2 =16.0.*alfs.*alfs.*ym.*ym./ipoint./ipoint;
if sub2: ~=-1..0
xl=sin (pi* (1.0-alfs) /ipoint*ym) ./pi./(1.0-sub2) ./ym./tstp;
x2=cos (pi* (1.0+alfs) /ipoint*ym) ./pi.*sub1./(1.0-sub2) ;
xt.='xl + 27. 5 bite): plot (Crs Llengthith))., xh)
else % (4alphaRst)*2 = lplot((1:length (xh) ) , xh)
xt                      =                       alts.rir.* (00

145


===== PAGE 152 =====
최신 이동통신시스템

Mobite Communications using MATLAB Simuiaiion

2.0/pi) .*cos (pi/4.0/alfs)+(1.0+2.0./pi) .*sin(pi/4.0/alfs)).:/sqrt (2

-0)F

end %/"1if sub2 += 1.0

end       % if icon == 0.0

if ncc == 0                             % in the case of receiver
xh( i ) = ./ ipoint = </-tt;. -% normalization

elseif ncc == 1 % in the case of transmitter
xh 1 1. Sate. 726          % normalization

else

error('ncc error');
end    % if nec == 0

end % fori=1

5

ZREKKKKKKKKKKKKKKK and of file KKKKKKKKEKEKKKKKKKKKKKKKKK

프로그램 3.4
% Program 3-4
oversamp.m

oe

Insert zero data to input data

00 00 00 00

Programmed by H.Harada

oe

function [out] = oversamp( indata, nsymb , sample)

ZRKKKK KK KKK KKK KK KKK  variables  KKK KE KKK KKK KKKKKKKKKKKKEK
indata : input sequence
nsymb   : Number of symbols

sample : Number of oversample
KKK KKK KKK KK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KK KK KK

00 00 00 00

out=zeros (1,nsymb*sample) ;
out (1:sample:1+sample* (nsymb-1) ) =indata;

ZRRKKKK KK KKK KKK KK KKK end of File KEK KKKKKKKKKKKKKKKKKKKKK
프로그램 3.5

% Program 3-5
gqpsk.m

oe

ode

146



===== PAGE 153 =====
% Simulation program to realize QPSK transmission system
%

% Programmed by H.Harada and T.Yamamura

%

ZK KKK KK KKK KK RK KK Preparation part KKEKKKKKKKKKKKKK KKK KKK

sr=256000.0;> % Symbol rate

ml=2;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,

16QAM:m1=4)

br=sr .* ml; % Bit rate

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=3;      % Eb/NO

IPOINT=8;    % Number of oversamples

ZK KKK KKK KKK KK KK Filter initialization KKKKKKKKKKKKKKKKK

irfn=21;                  % Number of taps

alfs=0.5;                 % Rolloff factor

[xh] = hrollfcoef(irfn,IPOINT,sr,alfs,1);     $Transmitter
coefficients

[xh2]   = hrollfcoef(irfn, IPOINT, sr,alfs, 0);     SReceiver
coefficients

ZK KKK KK KKK KK KK KK START CALCULATION KREKKKKKKKKKEKKKKKKKKK
nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop
LREKKKKKK KKK KK KK KKK Data generation KKK KKK KKK KKK kK KKK KKK
datal=rand(1,nd*ml)>0.5; % rand: built in function

ZK KK KR KK KR RR RR RK QPSK Modulation KKK KK KKK KKK KK KKK

[ich, qch]=qpskmod(datal,1,nd,m1l) ;
[ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ich1,qchl1, xh) ;

filter

filter

147


===== PAGE 154 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

ZREKKKKKK KKK KKK Attenuation Calculation KKKKKKKKKK KKK KKK

spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt(attn); % sqrt: built in function

GRKKKKKK KKK KKK KKK KKK Fading channel KKEKKKKKKKKKKKKKKKKKK

% Generated data are fed into a fading simulator
으

{[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itnd1l,nowl, length (
ich2);tstp; fd, flat}?

% Updata fading counter
Sitndl = itndl+ itnd0;

g*x*ktkeeHK Add White Gaussian Noise (AWGN) ******#x*

[ich3,qch3]= comb (ich2,qch2,attn);% add white gaussian noise
[ich4,qch4]= compconv (ich3,qch3, xh2) ;

syncpoint=irfn*IPOINT+1;
ich5=ich4 (syncpoint: IPOINT:length (ich4) );
qch5=qch4 (syncpoint: IPOINT: length (qch4) ) ;
ZRKKKKKK KKK KKK KKK KK QPSK Demodulation KREKKKKKKKKKKKKKKEK

[demodata]=qpskdemod (ich5,qch5,1,nd,ml1l) ;

ZRKKKKKKKKKKKK KKK Bit Error Rate (BER) KRKKKKKKKKKKKKKKK

noe2=sum (abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf ('Sd\t%e\n',iii,noe2/nod2) ;     %° £printt:: - bug Poe in
function

end % for iii=1:nloop
BK RK kk kk KK Output result KKEKEKKKKKKKKKKKKKKKKKK

ber = noe/nod;

148



===== PAGE 155 =====
fprintf ('sd\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERqpsk.dat','a');

fprintf (fid, 'sd\tse\ts£f\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid) ;

ZRKKKKKKKK KKK KKK KKK end Of File KERR KKKKKKKKKKKKKKKKKKKK

프로그램 3.6
% Program 3-6
% qpsk_fading.m
% Simulation program to realize QPSK transmission system
% (under one path fading)
%

Programmed by H.Harada and T.Yamamura

00 00

ZRRKKKK KKK KKK KK KKK Preparation part KKKKKKKK KKK KKK KKK KKK

sr=256000.0; % Symbol rate

ml=2;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,
16QAM:m1=4)

br=sr .* ml; % Bit rate

nd = 100;    % Number of symbols that simulates in each loop
ebn0=10;     % Eb/NO

IPOINT=8;    % Number of oversamples

ZREKKKKKKKKKKKKKKKK Filter initialization KKKKKKKKKKKKKK

LPin=21>                  % Number of taps

alfs=0.5;                 % Rolloff factor

[xh] =-Hrollfcoeft (izfinTPOINT, sr, alfts,1)>     STransmitter filter
coefficients

[xh2]   = hrollfcoef(irfn, LPOINT, sr,.alfs,'0);     SReceiver filter
coefficients

Gk KK KK KKK KR RK KR Fading initialization KKKKKKKKKKKKK KKK K

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in

149



===== PAGE 156 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

Program 238.
% Time resolution
tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

itau = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

03371 = [0];

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave
% In this simulation fourpath Rayleigh fading are considered.
th1=[0.0];

% Number of fading counter to skip
itnd0=nd* IPOINT*100;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
fd=160;

150



===== PAGE 157 =====
2s ^ 2

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1>flat (only amplitude is  fluctuated),0->nomal(phase and
amplitude are fluctutated)

flat =1;

ZREKKKKKKKKK KK KK KK KKK START CALCULATION KKEKKKKKKKKKKKKKKKK

nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop
ZRKKKKKKKKKKKKKKKK KKK K  Data  generation  KKK KKK KKK KKK KKK KK KKK
datal=rand(1,nd*ml)>0.5; % rand: built in function

BRK KKK KR KR KK KR RR RK KR KK KK QPSK Modulation KKKEKKKKKKKKKKK KKK KKK

{ich, qch]=qpskmod (datal,1,nd,m1l) ;
{ich1,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ich1,qchl1, xh) ;

LRKEKKKKKKKK KKK KKK KKK Attenuation Calculation KKK KKK KKK KK KK
spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt(attn); % sqrt: built in function

ZRAKKK KKK KK KK KK KK KK KKK Fading channel KKKKKKKKKK KK KKK KKK KKK

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itnd1,nowl, length (
Len2), tstp, $4; flac):

% Updata fading counter
itndl = itndl+ itnd0;

G*EKAEHAKAERE Ad White Gaussian: Noise < (AWGN) =e 2s Aner * &*

151



===== PAGE 158 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

[ich3,qch3]= comb (ifade, qfade,attn);% add white gaussian noise
[ich4,qch4]= compconv (ich3, qch3, xh2) ;

syncpoint=irfn*IPOINT+1;
ich5=ich4 (syncpoint: IPOINT: length (ich4) );
qch5=qch4 (syncpoint: IPOINT: length (qch4) );
Zk KKK KK KK KK KK KKK KK KK QPSK Demodulation ㅠㅠㅠ

[demodata]=qpskdemod (ich5,qch5,1,nd,ml1) ;

Zw KKK KKK KK KK KKK KK KK Bit Error Rate (BER) KKKEKKKKKKKKKKKKKKK

noe2=sum (abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noetnoe2;

nod=nod+nod2;

fprintf ('S$d\t%e\n',iii,noe2/nod2) ;     %)¥;:fprintis; built in
function

end % for iii=1:nloop

Zw KK KK KK KK KK KK KK KK KK Output LESULE KERR KKKKKKKKKKKKKKKKKKKK

ber = noe/nod;

fprintf ('Sd\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERqpskfad.dat','a');

fprintf (fid, 'd\t%e\tSf\t%f\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose(fid) ;

ZRKKKKKKKKKKKKKKKKKKK ANd OF File KKKKKKKKKKKKKKKKKKKKKKKKKK

프로그램 3.7
% Program 3-7

ole

compconv.m

Function to perform convolution between signal and filter

AP 00 00

programmed by H.Harada and M.Okita

00 ol?

152



===== PAGE 159 =====
function [iout, qout] = compconv(idata, qdata, filter)

응 RKKKKKKK KKK KKK KKK KKK KKK KR RK KK KK KK RK RR RR RR KR KK KK KK KK KK KK

%    idata          : ich data sequcence
%    qdata          : qch data sequcence
%   filter      : filter tap coefficience

옹  KOR KK KK RK KK KK RK kk kkk kk kk kk kk KK KKK KKK KR KK KK KK KK KKK KK

iout
qout

conv (idata, filter) ;
conv (qdata, filter) ;

ZRKKKKKKKKKKKKKK KK KKK end of file KKKKKKKKKEKKKKKKK KKK KKK KKK

프로그램 3.8
Program 3-8
compoversamp.m

00

oe

Insert zero data to Ich and Qch input data

00 00 00 00

programmed by H.Harada

oe

function [iout,qout] = compoversamp( idata, qdata , nsymb , sample)

KKKEKKKKKKKKK KKK KKK  variables  KKKKKKK KKK KKK KK KKK KK KK KKK

idata : input Ich data
qdata : input Qch data
iout : output Ich data.
qout : output Qch data
nsymb   : Number of burst symbol

sample : Number of oversample
KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KK KKK KK KKK KK KK

AP 00 00 00 00

00 00 00

ilout=zeros (1,nsymb*sample) ;
gqout=zeros (1,nsymb*sample) ;
iout (1:sample:1+sample* (nsymb-1) ) =idata;
gout (1:sample:1+sample* (nsymb-1) )=qdata;

ZREKKKKKKKKK KKK KKK KKK end Of File KKKKKKKKKKKKKKKKKKK KKK KKK

프로그램 3.9
% Program 3-9
% qpskmod.m

153



===== PAGE 160 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

%

% Function to perform QPSK modulation
%

% Programmed by H.Harada

%

function [iout, qout]=qpskmod (paradata, para,nd,m1l)

ZK K KK KKK KK KKK KKK KK  variables  KKEKKKKKKEKKKKKKKKKKKKK KK KK

paradata : input data (parabynd matrix)
iout :output Ich data

gout :output Qch data

para   : Number of paralell channels

nd : Number of data

ml : Number of modulation levels

(QPSK >2 16QAM > 4)

KKRKKKKKKKKKKKKKKKKKK KKK KKK KKK KKK KKK KKK KKK KKK KK KK KK KKK

00 00 00 00 00 00 00 00

m2=ml./2;

paradata2=paradata.*2-1;
count2=0;

for jj=l:nd

isi
isq

zeros (para,1);
zeros (para,1);

for-ii = 1-2 m2

isi    =    isi    a    소노    m2    i   a    )    ae
paradata2 ((1:para),iit+count2) ;

18    =    isq    +    수    m2    고   pind    )    ee
paradata2 ((1l:para) ,m2+iitcount2) ;

end

iout ((1:para),jj)=isi;
gout ((1:para) , jj) =isq;

count2=count2+ml;

end

Zw K KKK KK KK KR KK KK KK KK KK end of file KKEKKKKKKKKKKKKK KKK KKKKKKK

154



===== PAGE 161 =====
2s ^

프로그램 3.10

% Program 3-10

% qpskdemod.m

%

% Function to perform QPSK demodulation
%

% programmed by H.Harada

%

function [demodata]=qpskdemod (idata, qdata, para,nd,m1l)

Bw KK KK KK RK KR RK KK variables KKRKKKKKKEKKKKEKKKKKKK KK KKK

% idata :input Ich data

% qdata :input Qch data

% demodata: demodulated data (parabynd matrix)

% para   : Number of paralell channels

% nd : Number of data

% ml : Number of modulation levels

% (QPSK ->2 16QAM > 4)

옹 *ㅠㅠ×ㅠㄴㅠㄴㅠ＊×ㅠ×ㅠㄴㅠㄴㅠㅠ*＊×ㅠ×＊×ㅠ×ㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㅠ×*×ㅠㄴㅠㄴㅠㅠㄴㅠㄴㅠㄴㅠㅠㅠㅠ 가기 고 가가 고 계가 계가 가 가

demodata=zeros (para,ml1*nd) ;
demodata ((1:para), (1:ml:ml*nd1) )=idata((l:para), (1:nd) ) >=0;
demodata((1l:para), (2:ml:ml*nd) )=qdata((1:para), (1:nd) ) >=0;

Zw KK KK KR KKK KK KR RK KKK RK end of file KKEKKKKKKEKKKKKKKKKKKKKKK KKK

프로그램 3.11

Program 3-11
ogpsk.m

%
%
%
% Simulation program to realize OQPSK transmission system
%
% Programmed by H.Harada and T.Yamamura

%

Ze K KK KR KK KKK RK KK RK RK Preparation part KEKKKKKKKKKKKKK KK KK KKK

sr=256000.0; % Symbol rate

ml=2;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,
16QAM:m1=4)
br=sr.*ml1;   % bit rate

nd = 1000;   % Number of symbols that simulates in each loop

155


===== PAGE 162 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simiflation

ebn0=3;      % Eb/NO
IPOINT=8;    % Number of oversamples

ZK KKK KKK KR KK RK KK RK Filter initialization *****KKKKKKKKKKKK

irfn=21;                  % Number of taps

alfs=0.5;                 % Rolloff factor

{xh} = hrelltcoet (2%in, TPOINT, sr; alfs, 1);     S$Transmitter filter
coefficients

[xh2]   = ‘lhrolifcoef (rin; TPOINT,.sr,;alfts, 0);     sReceiver filter
coefficients

Sk KK KR RK KK Kk kk kk kk START CALCULATION **¥* XX KKKKKKK KKK KKK KKK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1l:nloop
Ze K KK KK RK KR RR KK KK RK KK KK Data generation [시 오존 을 상소 조수 오가 소수소소 소소오 소

datal=rand(1,nd*ml)>0.5; % rand: built in function

ZRKEKKKKKKKKEKKKKKKKKKKK OOQPSK Modulation ** KKK KKKKKKKK KKK KKK

{[ich, qch]=qpskmod (datal,1,nd,ml1l) ;

{ich1, qch1]=compoversamp (ich, qch, length (ich) , IPOINT) ;
ich21=[ichl zeros(1,IPOINT/2) ];
qch21=[zeros(1,IPOINT/2) qchl];

[ich2, qch2]=compconv (ich21,qch21, xh) ;

Zk KK KK KKK KK KK KK KKK Attenuation Calculation KaK KKK KK KKK KK KKK
spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn) ;                     % sqrt: built in- function

SR RR RK KK KR RK KK RR KK RK Fading Channel] *FEKKKKKKKKKKKKKK KKK KK

% Generated data are fed into a fading simulator
%

[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itnd1,nowl, length (

156



===== PAGE 163 =====
1601) ,ㄴ660, fd, flat):

% Updata fading counter
Sitndl = itndl+ itnd0;

BxkkkkkeeKKK* Add White Gaussian Noise (AWGN) ********#ek#«

[ich3,qch3]= comb(ich2,qch2,attn);% add white gaussian noise
[ich4,qch4]= compconv (ich3, qch3, xh2) ;

syncpoint=irfn*IPOINT+1;
ich5=ich4 (syncpoint: IPOINT: length (ich4) ) ;
qch5=qch4 (syncpointt+tIPOINT/2:IPOINT: length (qch4) ) ;

ZREKKKKKKK KKK KK KKK KK OQPSK Demodulation KRKEKKKKKK KKK KK KKK KKK

[demodata] =qpskdemod (ich5, qch5,1,nd,ml1l);

Gk RK RR RR RK KK RK KK Bit Error Rate (BER) KKKKKKKKKKKK KKK KK KKK

noe2=sum (abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf('sd\tte\n',iii,noe2/nod2); % fprintf: built in function
end % for iii=1:nloop

ERK KKK KKK KR KR RR KR KK RK Output 포은 KER KKKKKKKKKKKK KKK KKK KKK

ber = noe/nod;

fprintf('sd\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERogpsk.dat','a');

fprintf (fid, 'sd\t%e\tsf\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid) ;

ZREKKKKKKKKK KKK KKK KKK end of file KKKKKKKKKKKKKKKKKKKKKKKKK

157



===== PAGE 164 =====
\

최신 이동통신시스템

158

02276 Communications using MATLAB Simulation

Ret 3.12

% Program 3-12
ogqpsk_fading.m

Simulation program to realize OQPSK transmission system
(under one path fading)

Programmed by H.Harada and T. Yamamura

00 00 00 00 00 00 de

GRR KK RK KKK KR KK KKK Preparation part KKK KKKKEKKKKKKEK KKK EK

sr=256000.0; % Symbol rate

ml=2;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,
16QAM:ml1=4)

br=sr..* ml; 수 Bit rate

nd = 1000;    % Number of symbols that simulates in each loop
ebn0=10;     % Eb/NO

IPOINT=8;    % Number of oversamples

ZR KKK KK KK KR KR KK KKK Filter initialization KKKKKKKKKKKKKKKK KK

irfn=21;                  % Number of taps

alfs=0.5;                 % Rolloff factor

{xh] = hrollfcoef(irfn, IPOINT,sr,alfs,1);     S$Transmitter filter
coefficients

1321 = hrollfcoef(irfn, IPOINT,sr,alfs,0);     SReceiver filter
coefficients

ZRKKKKKKK KK KKK KK KKK Fading initialization KEK KKKKKKKEKKKKKEKK

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 2-8.

% Time resolution
tstp=1/sr/IPOINT;
% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set



===== PAGE 165 =====
으

응 direct wave.
itau = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

dlvl = [0];

% Number of waves to generate fading for each multipath.
% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

Initial Phase of delayed wave
In this simulation fourpath Rayleigh fading are considered.
th1l=[0.0];

%
%

% Number of fading counter to skip
itnd0=nd*IPOINT;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1l=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

2

% Maximum Doppler frequency [Hz]
% You can insert your favorite value

fd=160;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     + flat, fading or not

%  (l>flat (only amplitude is  fluctuated),0->nomal(phase and
amplitude are fluctutated)

flat =1;

159


===== PAGE 166 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation
Dk KK KK RK RK RR RR RR START CALCULATION KKEKKKKK KKK KKK KKK KKK
nloop=200; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop

LHKKKK KKK KKK KKK KKK KKK Data generation KKKKKKKKKKKKKKKKKKKKK

datal=rand(1,nd*ml)>0.5; % rand: built in function

eK KK KR KK RR RK RR KK KK OQPSK Modulation KKKKKKKKKKKKKKKKEKK

[ich, qch]=qpskmod (datal,1,nd,m1l) ;
[ich1,qch1]=compoversamp (ich, qch, length (ich) , IPOINT) ;
ich21=[ichl zeros(1,IPOINT/2) ] ;
qch21=[zeros(1,IPOINT/2) qchl1];

[ich2, qch2]=compconv (ich21,qch21, xh) ;

ZRKKK KKK KK KK KK KK KK Attenuation Calculation KKKKK KKK KKK KK KKK
spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10);

attn=sqrt(attn); % sqrt: built in function

KKKKKKKKKKKKKKKKKK KEK     ;             KKEKKKKKKKKKK KKK KKK KKK
Fading channe

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itndl1,now1, length (
ich), tstp;fa; flat};

% Updata fading counter
itndl = itndl+ itnd0;

ERKERARES HEX * 200 Whee. Gaussian Noise = (AWGN): ******s <**e™™

[ich3,qch3]= comb (ifade,qfade,attn);% add white gaussian noise
{ich4,qch4]= compconv (ich3,qch3, xh2) ;

syncpoint=irfn*IPOINT+1;

160



===== PAGE 167 =====
ich5=ich4 (syncpoint: IPOINT: length (ich4) );
qch5=qch4 (syncpoint+IPOINT/2:IPOINT: length (qch4) ) ;

Ze KKK KKK KK KK KK KK RK KK OQPSK Demodulation KKEKKKEKKKKKKKKKKKKKK

[demodata]=qpskdemod (ich5, qch5,1,nd,ml) ;

Ze K KK KK KR KK KR KK KK KKK Bit Error Rate (BER) KKEKKKKKKKKKKKKKKKK

noe2=sum(abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf('Sd\t%e\n',iii,noe2/nod2); % fprintf: built in function
end % for iii=1l:nloop

ZK KKK KK KK KKK KKK KK Output 조는 ㅠㅠㅠ

ber = noe/nod;

fprintf ('%d\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERogpskfad.dat','a');

fprintf (fid, 'sd\t%e\tsf\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid);

Zw KKK KR KK RK KK RK KK RK KK end of File KKKKKKKKKKK KKK KK KK KK KK KKK

프로그램 3.13

% Program 3-13

% msk.m

%

% Simulation program to realize MSK transmission system
%

% Programmed by H.Harada and T.Yamamura

%

Zk KKK KK KR RK KR KR KR KK KK KK preparation part KKEKKKKKKKKKKKKKKKKEK

sr=256000.0; % Symbol rate

161



===== PAGE 168 =====
최신 이동통신시스템
Mobile Communications using MATLAB Simutation

ml=1;        % ml:Number of modulation levels

br=sr.*ml;   % Bit rate

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=3;      % Eb/NO

IPOINT=8;    % Number of oversamples

ZREKKKKKKKKKKKKKKKKKK START CALCULATION **** XK KKK KKK KKK KK KK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=l:nloop

Zw KKK KR KKK RK KR KK KK KKK Data generation KKKKKKKKKK KKK KKK KK KK

datal=rand(1,nd)>0.5; % rand: built in function

ZREKKKKKK KKK KKK KKK KKK KK MSK Modulation ******KKKKKKKKKKKKKK

{ich, qch]=qpskmod (datal,1,nd/2,2);
smoothl=cos (pi/2* [-1+1./4.*[0:IPOINT-1]]);     SIPOINT     point
filtering

for ii=1:length (ich)
ich2 ( (ii-1) *IPOINT+1:ii*IPOINT) =(-1) ^ (ii-1) *smooth1.*ich (ii) ;
qch2 ( (ii-1) * [POINT+1:ii*IPOINT) =(-1) ^ (ii-1) *smooth1.*qch (ii);
end

ich21=[ich2 zeros(1,IPOINT/2) ] ;
qch21=[zeros(1,IPOINT/2) qch2];

ZREKKKKK KKK KKK KK RK Attenuation Calculation **** KKK KKKKKK KKK

spow=sum(ich21.*ich21+qch21.*qch21) /nd/2     ㆍ. %-sumt built in
function

attn=0.5*spow*sr/br/2*10.%* (-ebn0/10) ;

attn=sqrt (attn) ;                              % sqrt: built in
function

ZREKKKKKKKKKKKKKK KKK K Fading Channel ** KK KKK KKK KKK KKK KKK KK

162



===== PAGE 169 =====
Treo |

%[ifade, qfade]=sefade2 (data2,qdatal,itau,dlvll,th1,n0,itndl,nowl,1
ength (data2),fftlen2,fstp, fd, flat) ;

EXKAKKKKEKKEX Add White Gaussian Noise (AWGN) *******kkxKexe
[ich3,qch3]= comb (ich21,qch21,attn);% add white gaussian noise
syncpoint=1;

ich5
qch5

ich3 (syncpoint+IPOINT/2:IPOINT:length (ich2) ) ;
qch3 (syncpoint+IPOINT: IPOINT: length (ich2) +IPOINT/2) ;

ich5 (2:2: length (ich5) )=1*ich5 (2:2:length (ich5) ) ;
qch5 (2:2: length (ichS5) ) =1*qch5 (2:2:length(ich5) );

Sk RR KR RK RK KR KK KK K MSK Demodulation KKKKKKKKKKKKKK KKK KKK

[demodata]=qpskdemod (ich5,qch5,1,nd/2,2) ;

Gk KR KR KR RR RR RK KK KK Bit Error Rate (BER) KKKKKKKKKKKK KK KKK KK

noe2=sum(abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf ('sd\t%e\n',iii,noe2/nod2) ;     %.- tprinteé: built. cin
function

end % for iii=1l:nloop
BRK KKK RK RR KR RK RK RR KK KK KK Output result KKK KKK KKK KK KKK KKK KKK

ber = noe/nod;

fprintf ('%d\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERmsk,.dat','a');

fprintf (fid, 'sd\t%e\tsf\ts£\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid) ;

응***×*×*×**×*×ㅠ*×*×ㅠ×*※×*×ㅠ×*※ㅠ×ㅠㅠㅠ end OF ELLE KEK KKKKKKKKKKKKKKKKKKKKKK

프로그램 3.14

% Program 3-14
% msk_fading.m

163



===== PAGE 170 =====
\

최신 이동통신시스템

Mobite Communications using MATLAB Simulation

%

% Simulation program to realize MSK transmission system
% (under one path fading)

%

% Programmed by H.Harada and T. Yamamura

%

RK KK KK KK KK KK KK KK KK KK preparation part KKRKKKKKKKEKKKKKKKKKKK

sr=256000.0; % Symbol rate

ml=1;        % ml:Number of modulation levels

br=sr.*ml;   % Bit rate
%
%
%

nd = 100;      Number of symbols that simulates in each loop
ebn0=10;       Eb/NO
IPOINT=8;      Number of oversamples

Zw KR KK KKK KK KK KK KK KK Fading initialization KKKKKKKKKKKKKK KKK

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in

Program 2-8.
% Time resolution
tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

ttat = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

0171 = [0];

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

164



===== PAGE 171 =====
oa 00

n0=[6];

% Initial Phase of delayed wave
% In this simulation fourpath Rayleigh fading are considered.
th1=[0.0];

% Number of fading counter to skip
itnd0=nd*IPOINT*100;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
fd=320;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1>flat (only amplitude is fluctuated),0>nomal(phase and
amplitude are fluctutated)

flat _=1;

ZREKKKKKKKKKKK KKK KKK START CALCULATION KaKKK KKK KKK KKK KKK KKK
nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop
ZREKKKKK KKK KKK KK KK KK KK Data generation KKKKKKKKKKKKK KKK KK KK

datal=rand(1,nd)>0.5; % rand: built in function

KREKKRRKKKRARKKERKEREERE               +    RAKKAAKKKEKERKKKRRKKKK
MSK Modulation

165


===== PAGE 172 =====
\

최신 이동통신시스템

Mobile Communications using MATLAB Simufaiion

[ich, qch]=qpskmod (datal,1,nd/2,2);
smooth1l=cos (pi/2* [-1+1./4.*[0:IPOINT-1]]);     SIPOINT     point
filtering

for ii=1:length (ich)
ich2 ((ii-1) *IPOINT+1:ii*IPOINT) =(-1) ^ (ii-1) *smooth1.*ich (ii) ;
qch2 ( (ii-1) * IPOINT+1:ii*IPOINT) =(-1) ^ (ii-1) *smooth1.*qch (ii);
end

ich21=[ich2 zeros(1,IPOINT/2) ];
qch21=[zeros(1,IPOINT/2) qch2];

ZREKKKKKKKK KKK KKK Attenuation Calculation KKKKKKKKKKKK KK KKK

spow=sum(ich21.*ich21+qch21.*qch21) /nd/2     727 3-sum2 builtin
function

attn=0.5*spow*sr/br/2*10.%* (-ebn0/10) ;

attn=sqrt (attn) ;                              % sqrt;-burlt in
function

ZRKKKKKKKKKKKKKKKKKKEK Fading Channel ** RRR KKKKKKKKKKKKKKK

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich21, qch21, itau,dlvl,th1,n0,itnd1,nowl, lengt
h(ich21);, tstp,td, flat) +

% Updata fading counter
itndl = itndl+ itnd0;

BRXKKKKKEKKKE Add White Gaussian Noise (AWGN) ********k*xeK*
[ich3,qch3]= comb (ifade,qfade,attn);% add white gaussian noise
syncpoint=1;

ich5
qch5

ich3 (syncpoint+IPOINT/2:IPOINT: length (ich2) ) ;
qch3 (syncpoint+IPOINT: IPOINT: length (ich2) +IPOINT/2) ;

ichS (2:2: length (ich5) )=1*ich5(2:2:length(ich5) ) ;
qch5 (2:2: length (ich5) )=1*qch5 (2:2:length (ich5) ) ;

GREKKK KKK KKK KK KKK KKK MSK Demodulation ** ERK KKK KKKKKK KKK KK KK

166



===== PAGE 173 =====
[demodata]=qpskdemod (ich5,qch5,1,nd/2,2);

ZREKKKKKKKKK KKK KKK Bit Error Rate (BER) KKKKKKKKKKK KKK KKKKK

noe2=sum(abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf ('%d\t%e\n',iii,noe2/nod2) ;     %<—fprintts..zbuilé > in
function

end % for iii=1l:nloop

ZRKEKKKKKKKKKKKKKKKKKK Output LOSULE KERR KKK KKKKKKKKKKKKKKK

ber = noe/nod;

fprintf ('sd\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERmskfad.dat','a');

fprintf (fid, 'sd\t%e\t%£\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function                                     :

fclose (fid) ;

ZRKEKKKKKKKKKKKKKKK KKK end of file KKEKKKKKKKKKKKEKKKKKK KKK KKK

프로그램 3.15
% Program. 3-15
% msk2.m
%
% Simulation program to realize MSK transmission system
%
% Programmed by R.Sawai and H.Harada

oe

ZRKEKKKKKKKKKKKKKK KKK KKK Preparation part KKKKKKKKKKKKKK KKK

sr=256000.0; % Symbol rate

ml=1;        % ml:Number of modulation levels

br=sr.*ml;   % Bit rate

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=5;      % Eb/NO

IPOINT=8;    % Number of oversamples

167



===== PAGE 174 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

Ze KKK KR RK KR KK RK KK RK KK START CALCULATION KKK KKKKKKKKKKKKKK KKK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1l:nloop

BRK KK KKK KKK KK KK KK KK EK Data generation KKK KKKKKKKKKKKKKKKKKK

datal=rand(1,nd*ml)>0.5; % rand: built in function

ZRKKKKKK KK KKK KK KKK KKK MSK Modulation KKKKKKKKKKKKKKKKKKKKKK

datall=2*datal-1;
data2=oversamp2 (datall, length (datall) , IPOINT) ;

th=zeros (1, length (data2) +1) ;
ich2=zeros (1, length (data2) +1) ;
qch2=zeros (1, length (data2) +1) ;

for ii=2:length(data2) +1
th(1,ii)=th(1,ii-1)+pi/2*data2 (1,ii-1) ./IPOINT;
end

ich2=cos (th) ;
qch2=sin (th) ;

B&R RK KR RR Rk eK Attenuation Calculation KKEKKKKKKKKKKKKK

spow=sum(ich2.*ich2+qch2.*qch2)/(nd*IPOINT); % sum: built in
function

attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt(attn); % sqrt: built in function

ZRKKK KKK KK KK KK KK KR KK KK Fading channel KKKKKKKKKKKKKKKK KKK KKK

%[ifade, qfade]=sefade2 (data2,qdatal, itau,dlvll1,th1,n0,itndl1,nowl,1
ength(data2),fftlen2,fstp, fd, flat);

gkkkxekeKEKKEK Add White Gaussian Noise (AWGN) ******x**#**

168



===== PAGE 175 =====
Treo |

[ich3,qch3]= comb (ich2,qch2,attn);% add white gaussian noise
syncpoint = 1;
ich5=ich3 (syncpoint: IPOINT: length (ich3) );
qch5=qch3 (syncpoint : IPOINT: length (qch3) ) ;

ZRKKKKKKKKKKKKKKKKKKK MOK Demodulation KEKKKKKKKKKKKKKKK KKK

demoddata2 (1,1)=1;

for k=3:2:nd*ml+1
demoddata2 (1, k) =ich5 (1,k) *qch5 (1, k1) *cos (pi* (k) ) >0;
end

for n=2:2:nd*ml+1
demoddata2 (1,n)=ich5 (1, ㅁㄱ1 ) *qch5 (1,n) *cos (pi* (n) ) >0;
end

[demodata]=demoddata2 (1,2:nd*m1+1) ;

ZREKKKKKKKKKKKKKKK Bit Error Rate (BER) KKKKKKKK KKK KKK KKK KKK

noe2=sum (abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

. fprintf ('Sd\t%e\n',iii,noe2/nod2) ;     eo teenie; . built. “an
function

end % for iii=1l:nloop

LHEKKKKKKKKKKKKKKKKKKKKK Data ELLOS KERR KKKKKKKKKKKKKK KKK KK

ber = noe/nod;

fprintf ('%d\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERmsk2.dat','a');

fprintf (fid, 'td\t%e\t%f\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid) ;

ZREKKKKKKKKKKKKKKKKKK and of FLL le KERR KKKKKKK KKK KKK KKK KK KKK

169



===== PAGE 176 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

프로그램 3.16

% Program 3-16
msk2_fading.m

Simulation program to realize MSK transmission system
(under one path fading)

Programmed by R.Sawai and H.Harada

00 00 00 00 00 00 00

ZRRKKKK KKK KK KK KKK KKK Preparation part KKKKKKKKKKKKKKKKKKKKK

sr=256000.0; % Symbol rate

ml=1;        % ml:Number of modulation levels

br=sr.*ml;   % Bit rate

nd = 100;    % Number of symbols that simulates in each loop
ebn0=15;     % Eb/NO

IPOINT=8;    % Number of oversamples

ZRKKKKKKKKKK KKK KKK Fading initialization KKKKKKKK KK KKK KKKKK

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 2-8.

% Time resolution
tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

itau = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

divl = [0];

170



===== PAGE 177 =====
% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave
% In this simulation fourpath Rayleigh fading are considered.
th1=[0.0];

% Number of fading counter to skip
itnd0=nd*IPOINT*100;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1=[3000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
fd=320;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (l>Etat  (only amplitude is fluctuated),0->nomal(phase and
amplitude are fluctutated)

flat. =1;

EREKKKKKKKKKKKKKKKKKK START CALCULATION KKK KKKKKKKKKK KKK KKK
nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=l:nloop

ZRKKKKKKKK KKK KKK KKK KKK Data generation KKEKKKKKKKKKKKKKKKKKKK

171


===== PAGE 178 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

datal=rand(1,nd*ml)>0.5; % rand: built in function

ZRKKKKK KKK KKK KK KKK KK KK MSK Modulation KKK KKKKKKKKKKKK KKK KEK

datall=2*datal-1;
data2=oversamp2 (datall, length (data11),IPOINT) ;

th=zeros (1, length (data2) +1) ;
ich2=zeros (1, length (data2) +1) ;
qch2=zeros (1, length (data2) +1) ;

for ii=2:length (data2) +1
th(1,ii)=th(1,ii-1) +pi/2*data2 (1,ii-1) ./IPOINT;

end

ich2=cos (th) ;
qch2=sin (th) ;

ZRKKKKKKKKK KKK KKK Attenuation Calculation KKK KKK KK KKK KK KKK
spow=sum(ich2.*ich2+qch2.*qch2) / (nd* IPOINT) ;   $ sum: built in
function

attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt(attn); % sqrt: built in function

BRK KK KK KR RK KK KKK KKK KK KK Fading channel KKKKKKKKKKK KKK KK KK KKK

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itndl,nowl, length (
ich2), tstp, fa; fidt)-+

% Updata fading counter
itndl = itndi+ itnd0;

ERKKKKKKKKKKK Add White Gaussian Noise (AWGN) KKK KKK KEKE KK
{ich3,qch3]= comb (ifade, qfade,attn);% add white gaussian noise

syncpoint = 1;

ich5=ich3 (syncpoint:IPOINT: length (ich3) ) ;
qch5=qch3 (syncpoint: IPOINT: length (qch3) ) ;

172



===== PAGE 179 =====
Tee |

ZRKK KKK KKK KK KKK KK KKK MSK Demodulation KRKKKEKKKKKKKKKKKKKK KK

demoddata2 (1,1)=1;

for k=3:2:nd*ml+1
demoddata2 (1, k)=ich5 (1,k) *qch5 (1,k1) *cos (pi* (k) )>0;
end

for. n=232:nd*m1+1
demoddata2 (1,n) =ich5 (1,n-1) *qch5 (1, n) *cos (pi* (n) ) >0;
end

[demodata]=demoddata2 (1,2:nd*m1+1) ;

ZREKKKKKKKKKKKKKKK Bit Error Rate (BER) KKEKKKKKKKKKKKKKKKKK

noe2=sum(abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf ('sd\t%e\n',iii,noe2/nod2) ;     . fprint’: = built 32
function

end % for iii=1l:nloop

ZRAEKKKKKKKKKKKKKKKKK KKK Data file KKKKKKKKKKKKKKKKKKKKKK KKK

ber = noe/nod;

fprintf ('%d\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERmsk2fad.dat','a');

fprintf (fid, 'sd\t%e\t%f\tsf\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid);

Zw KKK KK KK KR KK KR RK KK KK end OL tile Ka KKK KKK KKK KKKKK KKK KKK KK

프로그램 3.17
% Program 3-17

2

% oversamp2.m

00

% Function to sample "sample" time

173



===== PAGE 180 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

%
% programmed by H.Harada

ole

function [out] = oversamp2( iin, ntot , sample)

KKK KK KKK KK KK KK KK KK KKK KKK KKK KK KKK KKK KKK KKK KK KKK KK KKKKKK KKK
iin     : input sequence
ntot   : Number of burst symbol

sample : Number of oversample
KKKKKKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KK KKK KKK KKK KKK KKKKKK

00 00 00 00 00

for k=l1:sample
out (k:sample:k+sample* (ntot-1) )=iin;
end

Bk OK RR RK KK KK KK KK KKK End OF FLL KEKKKKKKKKKKKKKKKKKKKKKKK

프로그램 3.18

Program 3-18
gmsk.m

00 00

Simulation program to realize GMSK transmission system

Programmed by R.Sawai and H.Harada

00 00 00 00 00

GK RR RR RK KR KR KK KK Preparation part KKKEKKKKKKKKKKKKKKKKK

sr=256000.0; % Symbol rate

ml=1;        % ml:Number of modulation levels

br=sr.*ml;   % Bit rate

nd = 1000;   % Number of symbols that simulates in each loop
ebn0=5;      % Eb/NO

IPOINT=8;    % Number of oversamples

ZR KR KR RK KR KK KKK KR RK KKK Filter initials 2zation KKEKKKKKKKKKKKKKKKK

irfn=21;                  % Number of taps

B=0.25*sr;

B2=0.6*sr;

[xh]   =   gaussf (6).irtfa; POINT, sr, 1);         STransmitter   filter
coefficients

174



===== PAGE 181 =====
[xh2] =gaussf(B2,irfn,IPOINT,sr,0); %Receiver filter coefficients

ZRKKKKKKKK KKK KK KKK START CALCULATION **¥**RRKKKKKKKKKKKKKKKK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0; . % Number of transmitted data

for iii=l:nloop

ZREKKKKK KKK KKK KK KK KK KK Data generation KKKKKKKKKKKKKK KKK KKK

datal=rand(1,nd.*ml)>0.5; % rand: built in function

ZRKKK KKK KKK KKK KK KK KKK GMSK Modulation ** KK KKKKKKKKKKKKKKKK

datall=2*datal-1;
data2=oversamp (datall, length (datal1l),IPOINT) ;
data3=conv (data2, xh) ;                           % NEW for GMSK

th=zeros (1, length (data3) +1) ;
ich2=zeros (1, length (data3) +1) ;
qch2=zeros (1, length (data3) +1) ;

for ii=2:length(data3) +1
th(1,ii)=th(1,ii-1) +pi/2*data3(1,ii-1) ./IPOINT;

end

ich2=cos (th) ;
qch2=sin (th) ;

BRK KKK KK KK KR KK KKK KK Attenuation Calculation KEKKKKKKKKK KK KKK
spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function

attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn) ;                     %\ sqre: built. in-function
ZRKKKKKKKK KKK KKK KKK KKK Fading channel KKK KK KK KKK KKK KKKKK KKK

%[ifade, qfade]=sefade2 (data2,qdatal, itau,dlvl1,thi,n0,itndl,nowl,1
ength (data2), fftlen2, fstp,fd, flat) ;

Exkkkkee HK Add White Gaussian Noise (AWGN) ******+##HeX

175



===== PAGE 182 =====
9

최신 이동통신시스템

176

Mobite Communications using MATLAB Simulalion

[ich3,qch3]= comb(ich2,qch2,attn);% add white gaussian noise
[ich4,qch4] = compconv(ich3,qch3,xh2) ;

syncpoint =irfn*IPOINT-IPOINT/2+1;
ich5=ich4 (syncpoint: IPOINT: length (ich4) );
qch5=qch4 (syncpoint: IPOINT: length (qch4) ) ;

ZREKKKKKKKK KKK KKKKKK CMSK Demodulation KEKKKKKKKKKKKKK KK KKK

demoddata2 (1,1)=1;

for k=3:2:nd*ml+1
demoddata2 (1, k) =ich5 (1, k) *qch5 (1, k-1) *cos (pi* (k) ) >0
end

for n=2:2:nd*ml+1
demoddata2 (1,n)=ich5 (1,n-1) *qch5 (1,n) *cos (pi* (n) )>0;
end

[demodata]=demoddata2 (1,2:nd*ml1+1) ;

ZK KKK KKK KK KKK KKK KK Bit Error Rate (BER) KKKKKKKKKKKKKKKKEK

noe2=sum(abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noet+noe2;

nod=nod+nod2;

0

fprintf ('S$d\t%e\n',iii,noe2/nod2) ;     6 <fprinct:, ~burle in
function

end % for iii=1:nloop

Bk KK KK KKK KR KR RK KK KK Output result KKK KK KK KKK KKKKKKKKKK KKK KEK

ber = noe/nod;

fprintf ('Sd\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function

fid = fopen('BERgmsk.dat','a');

fouint#ieid Heese ce Ree Le: noe/nod, noe, 내  % 00310 1
built in function



===== PAGE 183 =====
= 0트

fclose (fid) ;

GRR KKK KK KKK KR KKK KR KR KK end of FLL KKK KKKKKKKKK KKK KKK KKK KKK

프로그램 3.19

% Program 3-19
gmsk_fading.m

%

%

% Simulation program to realize GMSK transmission system
% (under one path fading)
%
%
%

Programmed by R.Sawai and H.Harada

Zk KKK KR KR KR KK RK Preparation part KKEKKKKKKKKKKKKKKKK KKK KKK

sr=256000.0; % Symbol rate
ml=1;        % ml:Number of modulation levels
br=sr.*ml;   % Bit rate
nd = 100;    % Number of symbols that simulates in each loop
ebn0=15;     % Eb/NO
%

IPOINT=8;      Number of oversamples

Gk KK KR KK RK KK RK KK KK KK Filter initialization KKKKKKKKKKKK KKK KKK

irfn=21;                  % Number of taps

B=0.25*sr;

B2=0.6*sr;

[xh]   =   gaussf(B,irfn, IPOINT,sr,1);         S$Transmitter   filter
coefficients

[xh2] =gaussf(B2,irfn,IPOINT,sr,0); %Receiver filter coefficients

GRR KKK KK KKK KK KKK Fading initialization KKEKEKKKKKKKKKKKKKKKAKK

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 2-8.

% Time resolution

tstp=1/sr/IPOINT;

177



===== PAGE 184 =====
Ay

최신 이동통신시스템

178

Mobile Communications using MATLAB Sinu#ation

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

itau = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

divl = [0];

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave

% In this simulation fourpath Rayleigh fading are considered.
thl=[0.0];

% Number of fading counter to skip
itnd0=nd*IPOINT*100;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]

% You can insert your favorite value

fd=320;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1>flat (only amplitude is  fluctuated),0>nomal(phase and

amplitude are fluctutated)



===== PAGE 185 =====
flat =1;
Sk KR KR RK Kk kkk kk KK START CALCULATION KKKEKKKKKK KKK KKK 나
nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=l:nloop

ZwKKK KKK KKK KKK KK KK KK KKK Data generation KKKKKKKK KKK KKK KKK KKK

datal=rand(1,nd.*ml)>0.5; % rand: built in function

Sk RR RR KK KR KK KK KK KK KK GMSK Modulation KKKKKKKKKKKKKK KKK KKK

datall=2*datal-1;
data2=oversamp (datall1, length (datall) , IPOINT) ;
data3=conv (data2,xh) ;                           % NEW for GMSK

th=zeros (1, length (data3) +1) ;
ich2=zeros (1, length (data3) +1) ;
qch2=zeros (1, length (data3) +1) ;

for i1i1=2:length (data3) +1
th (1,11) =th(1,ii-1) +pi/2*data3(1,ii-1) ./IPOINT;

end

ich2=cos (th) ;
qch2=sin (th) ;

Zk KK RK KK KK Kk Attenuation Calculation KKK KKKKKKKKKKKKK
spow=sum(ich2.*ich2+qch2.*qch2)/nd; % sum: built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn) ;                     $i sqre: built-in: function

ZREKKKKKKKKKK KKK KK KK Fading Channel ***KKKKKKKKKKKKKKKKKKK

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itnd1,now1, length (
i¢ch2) ,tstp;td, flat}?

179


===== PAGE 186 =====
최신 이동통신시스템

180

Mobile Communications using MATLAB Simulation

% Updata fading counter
itndl = itndl+ itnd0;

ZxkkxkKKKKEKK Add White Gaussian Noise (AWGN) **********xk**
[ich3,qch3]= comb(ifade,qfade,attn);% add white gaussian noise
[ich4,qch4] = compconv (ich3,qch3,xh2) ;

syncpoint =irfn*IPOINT-IPOINT/2+1;
ich5=ich4 (syncpoint: IPOINT: length (ich4) ) ;
qch5=qch4 (syncpoint: IPOINT: length (qch4) ) ;

LEEK KKKKKK KKK KK KKK KKK GMSK Demodulation KKKKKKKKKKKKKKKKKKEK

demoddata2 (1,1)=1;

for k=3:2:nd*mlt+1
demoddata2 (1, k) =ich5 (1, k) *qch5 (1, k-1) *cos (pi* (k) ) >0;
end

for n=2:2:nd*ml+1
demoddata2 (1,n)=ich5 (1,n-1) *qch5 (1,n) *cos (pi* (n) )>0;
end

[demodata]=demoddata2 (1,2:nd*ml+1) ;

LHKKK KKK KK KKK KKK KK Bit Error Rate (BER) KKK KK KK KKKKKKKKKKKKK

noe2=sum (abs (datal-demodata)); % sum: built in function
nod2=length(datal); % length: built in function
noe=noe+noe2;

nod=nod+nod2;

fprintf ('%d\t%e\n',iii,noe2/nod2) ;     도 Fprintt: = 00016 an
function

end % for iii=1:nloop
LKKKKK KKK KK KKK KK KKK KK KK Output result KKK KKKKKKKKK KKK KK KKK K

ber = noe/nod;
fprintf ('$d\t%d\t%d\t%e\n',ebn0,noe,nod,noe/nod); % fprintf: built
in function



===== PAGE 187 =====
Treo |

fid = fopen('BERgmskfad.dat','a"');

fprintf (fid, '$d\t%e\t%f\t%f\t\n',ebn0,noe/nod,noe,nod); % fprintf:
built in function

fclose (fid);

Zk RK RK RR RR KK end of file KKKKKKKKKKKKKKK KKK KKK KK KK

프로그램 3.20

% Program 3-13
gaussf.m

%
%
% Function to form Gaussaian filter
%
%

programmed by H.Harada

function [xh] = gaussf(B,irfn,ipoint,sr,ncc)

SK KI KK KK KI KK KKK KK KKK HK IK KI KKK KE KKK KK KKK KK KKK KKK KK KK KK KK

%    irfn           : Number of symbols to use filtering

%    ipoint         : Number of samples in one symbol

%    sr             : symbol rate

%    B              : filter coeficiense

%    ncc;           : 1 - transmitting filter 0 - receiving filter

Se KR IK I IK IK I I RI I III I I II I FO IOI FOR IK III IKI IOI ek IK
point = ipoint;

tr = sr ;

n-=-ipoint<.* 62207}

mid = (A+ /-2*) 24:4;

fo=B/sqrt (2*log(2));

fori = 1 in

icon = i - mid;
ym = icon;

xt=1°5/2* (ey ft, (8.9 0% 4 Bf ogo) Sy hee Bn pO nt
1/2) /tr) terf (sqrt (2/log (2) ) *pi*B* (ym/ipoint+1/2) /tr));

181



===== PAGE 188 =====
\

최신 이동통신시스템

182

Mobile Communications using MATLAB Simulation

if nec ==                               % in the case of receiver
xh( i f)c= ets;

elseif nec ==                        % in the case of transmitter
xn“) 푸우

else
error (incc"error™)?

end

end

Sk OR RK RRR RK KR KR ROK KK KK end of file KKK KKKKKEKKKEKKKKEKKKKKKKEKK

2248 3.21

% Program 3-21

% qaml16

%

% Simulation program to realize 16QAM transmission system
g

ㅎ

% Programmed by H.Harada and R.Funada

%

ZRKEKKKKKKKKKKK KK KK KKK preparation part KKKKKKKKKEKKKKKKKKKKKK

sr=256000.0; % Symbol rate

ml=4;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,
16QAM:m1=4)

br=sr <* ml; % Bit rate

nd = 1000;    % Number of symbols that simulates in each loop
ebn0=6;      % Eb/NO

IPOINT=8;    % Number of oversamples

ZRKKKK KKK KK KKK KK KK  Filter  initialization     KKKKKKKKKKKKKKKEEEK
irfn=21;                  % Number of taps

alfs=0.5;                 % ROlLOfLL factor

[xh] = hrollfcoef(irfn, IPOINT,sr,alfs,1);     STransmitter filter
coefficients

{xh2]   = hrollfcoef(irfn, IPOINT,sr,alfs,0);     SReceiver filter
coefficients

Zk RR KR RK KKK RK KR KK KK KKK START CALCULATION **** kK KKKKKKKKKKKK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data



===== PAGE 189 =====
nod = 0;    % Number of transmitted data
for iii=1:nloop
ZRKKK KKK KKK KKK KK KKK KKK Data generation KKEKKKKEKKKEKKK KKK KK KKK

datal=rand(1,nd*ml)>0.5;

Zw KK KK RK RK RK KK KKK KKK 16QAM Modulation KKKKKKKKKKKKKKKKKKKK

{ich, qch]=qammod (datal,1,nd,m1l) ;
[ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ichl,qch1, xh) ;

Zw KKK KK RK KR KR KK KK Attenuation Calculation KEKKKKKKKKKKKKKK KKK

spow=sum(ich2.*ich2+qch2.*qch2) /nd;
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn) ;

ZR KR RK KK KK KK Fading Channel **RRKKKKKKKKKKKKKKKKKK

% Generated data are fed into a fading simulator

%
[ifade, qfade]=sefade (ich2,qch2,itau,dlvl,th1,n0,itnd1l,nowl, length (
33062) ,;tstp;fd; flat);

% Updata fading counter
% itndl = itndl+ itnd0;

GtkkexkeKHKKHK Add White Gaussian Noise (AWGN) *****k*eeHKEK

[ich3,qch3]= comb(ich2,qch2,attn);% add white gaussian noise
[ich4,qch4]= compconv (ich3, qch3,xh2) ;

sampl=irfn*IPOINT+t1;
ich5 = ich4(samp1l:IPOINT:length (ich4) ) ;
qch5 = qch4 (sampl:IPOINT: length (ich4) );

Bk KR KR KR RK KK KK KK KK KK 16QAM Demodulation ***KKKKKKKKKKKKKKK

[demodata]=qamdemod(ich5,qch5,1,nd,m1) ;

BRK KK KK KKK KKK KK KK Bit Error Rate (BER) KKKKKKKKKKKKKK KKK KKK

183


===== PAGE 190 =====
최신 이동통신시스템

184

Mobile Communications using MATLAB Simulation

noe2=sum (abs (datal-demodata) ) ;
nod2=length (datal) ;
noe=noe+noe2;

nod=nod+nod2;

fprintf ('S$d\t%e\n',iii,noe2/nod2) ;
end % for iii=1:nloop

ZRKKKKK KKK KKK KK KK KEK Output 조은 KERR KK KKKKKKKKK KKK KK KKK

ber = noe/nod;

fprintf ('Sd\t%d\t%d\t%e\n',ebn0, noe, nod, noe/nod) ;

fid = fopen('BERgqam.dat','a');

fprintf (fid, 'd\t%e\t%f\tsf\t\n',ebn0, noe/nod, noe, nod) ;
fclose (fid);

ZeKKKKKKKKKKKKKKKEKKK and of Tile KREKKKKKKKKKKKKKKKKKKKKKKKK

프로그램 3.22

Program 3-22
90016 fading

00 ol?

Simulation program to realize 16QAM transmission system
(under one path fading)

00 00 00

ae 00

Programmed by H.Harada and R.Funada

ae

Bw KK RK KK RK KK KKK KR preparation part KKK KKK KKKKKKKKKKK KKK

sr=256000.0; % Symbol rate

ml=4;       % ml:Number of modulation levels (BPSK:ml=1, QPSK:ml=2,
16QAM:m1=4)

br=sr .* mL;.% Bit rate

nd = 100;    % Number of symbols that simulates in each loop
ebn0=15;     % Eb/NO

IPOINT=8;    % Number of oversamples

ZREKKKKK KKK KKK KKK KK  Filter  initialization     KKKKKK KK KKK KKK KK
irfn=21;                  % Number of taps

alfs=0.5;                 % Rolloff factor

[xh] = hrollfcoef(irin, 1POINT, sr,alts,..):;     STransmitter filter



===== PAGE 191 =====
seo, 를

coefficients
[xh2]   = hrollfcoef(irfn, IPOINT,sr,alfs,0);     SReceiver filter
coefficients

ZREKKKKKKKKKKKK KK Fading initialization KKK KKKKKKKKKKKKKKEKK

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 28.

% Time resolution
tstp=1/sr/IPOINT;

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

itau = [0];

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

divi. = [0],

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave

% In this simulation fourpath Rayleigh fading are considered.
th1=[0.0];

% Number of fading counter to skip

itnd0=nd* IPOINT*100;

% Initial value of fading counter

% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

185


===== PAGE 192 =====
최신 이동통신시스템

186

Mobile Communications using MATLAB Simulation

itnd1=[1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
fd=160;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1>flat  (only amplitude is  fluctuated),0->nomal(phase and
amplitude are fluctutated)

flat =1;

ZRKKKKKKKK KKK KKK KKK KKK START CALCULATION Ka KKK KKK KKK KKK KKK KK
nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
nod = 0;    % Number of transmitted data

for iii=1:nloop
GK KK KR KR KR Data generation KaAKK KKK KKK KK KKK KK KKK

datal=rand(1,nd*ml)>0.5;

BRK KR KK KK KR RR KK RR KK KK KK 16QAM Modulation **** KK KK KKK KKK KK KK

{ich, qch]=qammod (datal,1,nd,m1l) ;
[ichl,qch1]= compoversamp (ich, qch, length (ich) , IPOINT) ;
[ich2,qch2]= compconv (ichl,qchl1, xh) ;

ERK KKK KKK RK KK KR KKK Attenuation Calculation *** RR KKKKKKKKKKKK

spow=sum (ich2.*ich2+qch2.*qch2) /nd;
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn) ;

ZREKKKKK KKK KKK KK KKK KKK Fading Channel ** KR KKKKKKKKKKKKKKKK



===== PAGE 193 =====
% Generated data are fed into a fading simulator

[ifade, qfade, ramp] =sefade (ich2,qch2,itau,dlvl,th1,n0,itndl,nowl,le
ngth(ich2),tstp, fd, flat);

% Updata fading counter
itndl = itndl+ itnd0;

유********×*×*×*×* Add White Gaussian Noise (AWGN) *****kekk eee
[ich3,qch3]= comb (ifade,qfade,attn);% add white gaussian noise

%****** Compensate the fluctuation of fading by ramp*******

ich3=ich3./ramp(1:length (ramp) ) ;
qch3=qch3./ramp (1:length (ramp) ) ;

{ich4,qch4]= compconv (ich3,qch3, xh2) ;
sampl=irfn*IPOINT+1;

ich5   ich4 (62001: IPOINT: length (ich4) ) ;
qch5   qch4 (samp1:IPOINT: length (ich4) );

ZRKKK KKK KKK KK KK KKK 16QAM Demodulation KKKKKKKKKKKKK KK KKK KKK

[demodata] =qamdemod (ich5,qch5,1,nd,m1l) ;

ZRKKKKKKKK KKK KKK KKK Bit Error Rate (BER) KKEKKKKKKKKKKKKKKKK

noe2=sum (abs (datal-demodata) ) ;
nod2=length (datal) ;
noe=noe+noe2;

nod=nod+nod2;

fprintf ('%d\t%e\n',iii,noe2/nod2) ;
end % for iii=1:nloop

KREKKKREKKRAERECKKAKKRK                   KKK KK KK KKK KKK KKKKKKKKKK
%             &       Output result
ber = noe/nod;

fprintf ('$d\t%d\t%d\t%e\n',ebn0, noe, nod, noe/nod) ;
fid = fopen('BERqamfad.dat','a');

187



===== PAGE 194 =====
최신 이동통신시스템

188

Mobile Communications using MATLAB Simulation

fprintf (fid, 'd\t%e\t%f\ts£f\t\n',ebn0, noe/nod, noe, nod) ;
fclose(fid);

Zw RRR RK KKK KK KK KKK KK KK end of file KKKEKKKKKKKKKKKKKKKKKK KKK

프로그램 3.23
% Program 3-23
% qammod.m
%
% This function is used for Gray coding of 16QAM modulation
%
% programmed by R.Funada and H.Harada
%

function [iout, qout]=qammod (paradata, para,nd,ml)

ZeKKK KKK KKK KKK KKK KK KK KK  variables  KKKKKKKKEKKKKKKKKKKKKKKEKK

% paradata : input data (parabynd matrix)
% iout :output Ich data

% gout :output Qch data

% para   : Number of paralell channels

% nd : Number of data

% ml : Number of modulation levels

oe

(QPSK >2 16QAM > 4)

KKEKKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKKKKKKKKKKKKKK KKK KKK KEK

ole

% The constellation power

k=sqrt (10);
iv=([-3 그 3133

m2=m1/2;
count2=0;

for ii=1 : nd

ㅣ

Lea   zeros (para,1);
isq   zeros (para,1);
for. jjeLt me

if jj <= m2
isi = isi +2.“( m2- jj ).*paradata((l:para),count2+}j3) ;
else



===== PAGE 195 =====
isq = isq +2.*( ml jj ).*paradata((1l:para) ,count2+ jj);
end
end

iout((l:para),ii) = iv(isit1) ./k;
qout ((l:para),ii) =iv(isqt1) ./k;

count2=count2+ml;

end

Zk KR RR KK RK KK KK end OF ELlS KEKKKKKKKKKKKKKKKKK KKK KKK

프로그램 3.24

% Program 3-24
qamdemod.m

%

%

% Function to decode 16QAM modulation
%

% programmed by R.Funada and H.Harada
%

function [demodata]=qamdemod (idata, qdata, para,nd,ml)

ZR KKK KKK KK KK KKK KKK  variables  KKEKKKKKKKKKKKKKKK KKK KK KKK

% idata :input Ich data

% qdata :input Qch data

% demodata: demodulated data (parabynd matrix)

% para   : Number of paralell channels

% nd : Number of data

% ml : Number of modulation levels

% (QPSK ->2 16QAM > 4)

 KKK KKK KKK KKKKKKKKKKKKKKKK KKK KKK KK KK KKK KKK KKK KKK KKK KKK

k=sqrt (10);

idata=idata.*k;
qdata=qdata.*k;
demodata=zeros (para,ml*nd) ;

m2=m1/2;
count2=0;

fori = lind

189


===== PAGE 196 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation

a=1;
b=1;
i_lngth=0;
q_ingth=0;

for jj= 1:m2
Gf jg 으루 개

if demodata((1:para) , jj-1+count2) ==
a=a;
end

if demodata((1:para) ,m2+jj-1+count2) ==1
b=b;
end

i_ingth=i_Ingthti_plrty.*2.%*(m2-jj+1);
q_lngth=q_lngth+q plrty.*2.* (m2-jj+1);
end

if idata((l:para),ii) >= i_lngth
demodata ( (1:para) , jj+count2) =a>=0;
i_plrty=1;
else
demodata ((1:para) ,jj+count2) =a<=0;
i_plrty=1;
end

if qdata((l:para),ii) >= q_lngth
demodata ((1:para) ,m2+jj+count2) =b>=0;
q_plrty=1;
else
demodata ((1:para) ,m2+3j+count2) =b<=0;
q_plrty=1;
end

end % for jj= 1:m2
count2=count2+ml1;

end $% for ii = 3800

BRK KKK KR RK RR RK KR RK KK KK end of File KKKKKKKKKKK KK KKK KKK RK KKK KKK

190



===== PAGE 197 =====
ee



===== PAGE 198 =====
Al SOA SO (OFDM)
전송기법

1 0

2장에서 보인 바와 같이, 이동통신용 무선전송채널은 다중경로 페이덩 환경에 의해
특징지어진다. 달리 표현하면, 수신기에서의 신호는 시선방향의 직접파뿐만 아니라 서
로 다른 시간에 수신기에 도달하는 많은 반사파들을 포함하고 있다. 지연파는 나무, 언
덕, 산, 자동차 그리고 건물과 같은 지형물에 반사된 결과로 나타난다. 이들 반사된 지연
파들이 직접파를 간섭하고 네크워크 성능에 큰 감소를 가져오는 심볼 간 간섭
intersymbol interference (0181)를 야기 시킨다. 무선 네트워크는 이런 불리한 효과들을
최소화하는 방향으로 설계되어야 한다.

최근에는, 유선통신 네크워크에서 가능한 서비스를 이동무선통신 네트워크 사용자
에게 확장하고자하는 시도들이 증가하고 있다. 이러한 시도들은 광대역 이동통신이 가
능하리라는 기대를 증폭시키고 있다. 광대역 멀티미디어 이동통신 시스템에서는 최소
한 초당 수 메가비트의 높은 ASSO] 필수적이다. 그러나 디지털 데이터가 초당 수 메
가비트로 전송되면 지연파의 지연시간은 1 심볼 시간을 초과하게 된다. 지연파가 다른
심볼을 간섭하기 때문에 이 간섭의 효과는 수신신호에서 제거되어야 한다. 이를 위한
몇 가지 방법이 존재한다. 수신기에서 적응 균등화 기법을 사용하는 것은 수신신호를

193



===== PAGE 199 =====
최신 이동통신시스템

| sa 전송기법의 개념

Mobile Communications using MATLAB Simulation

균등화하는 한 가지 방법이다. 그러나 AAA OS 초당 수 메가비트의 균등화를 간단하
고 저가의 하드웨어로 구현하기란 매우 어렵다.

다중경로 Hold 환경을 극복하고 무선 광대역 멀티미디어 통신 시스템 (WBMCS)
을 구현하기 위해서 이 장에서 설명한 OFDM 전송기법을 사용할 수 있다. OFDMS 병
렬 데이터 전송기법에 기반하는데 [133] 이는 다중경로 페이덩의 효과를 감소시키고 복
균등기를 불필요하게 한다. OFDME] 역사에 대해서는 참고문헌 [3]에 잘 기술되
다

OFDM-2: 차세대 방송과 무선랜 (WLAN) 시스템에서 이미 활발하게 사용되고 있다.
예를 들어, 유럽의 ETSI BRAN [4], 미국의 IEEE802.11 [5], 일본의 4818 MMAC [6]
는 이미 차세대 광대역 WLAN 시스템의 물리계층으로써 OFDM 전송기법을 채택하였
다. 표준화 기구에서 몇 가지 통신 시스템들이 이미 컴퓨터 시뮬레이션을 통해 비교되
었다. 이 장은 OFDM 신호의 생성 방법과 OFDM 송신기와 수신기의 구성, 88과 패
킷 오류율(88#) 성능을 컴퓨터 시뮬레이션을 통해 평가하는 WHS 설명한다.

이 장은 다음과 같이 구성되어 있다: 먼저, 병렬 데이터 전송기법에 대한 개념이 4.2
장에 기술되어 있다. 4.3장은 OFDM 전송기법의 개념에 대해 설명하고 OFDM 송수신
기의 구성에 대해 설명한다. 4.4장은 OFDM 신호를 생성하는 WHAT} 컴퓨터 시뮬레이
션으로 OFDM 송수신기를 구성하는 방법을 기술한다. 4.5장은 표준 OFDM 기반
WLAN 시스템에 해당하는 OFDM 시스템 시뮬레이션 방법을 소개한다. 4.6장은 간단
한 정리로 결론을 짓는다. 이 장과 관련된 모든 프로그램은 부록 4^와 0ㅁ2ㅁㅠ\04에 제
공된다.

0 aes
yo, oh

194



===== PAGE 200 =====
직교주파수분할다중 (OFDM) 전송기법   『 §

상 정보를 포함한다. 그림 4.1은 전형적인 다중경로 페이덩의 시간과 주파수 도메인의
임펄스응답을 보여준다. 시간 도메인의 관점에서, 서로 다른 도착시간과 신호파워 그
리고 위상을 가진 많은 신호가 수신기에 도달한다, 반면에 주파수 도메인 관점에서 보
면, 다중경로 페이덩은 특정 주파수들의 증가와 감소로 특징되어진다. 만약 이동수신
이 존재한다면 여러 수신경로의 상대적인 파워레벨과 감쇠는 시간에 따라 변할 것이다.
협대역 신호는 피크와 주파수 응답이 주파수 도메인에서 이동함에 따라 그 품질이 변할
것이다. 또한 신호로써 위상을 사용하는 모든 시스템에 SHS 미칠 위상 응답에도 상
당한 변동이 존재할 것이다.

Channel                                         Channel

impulse                                         impulse

response                                  . fesponse                           ate
Time                               !      Frequency

1 channel
serial                                                                             |        ~,     \
transmission                                                                                             >

transmission 0094    ~ Be

Lal
8 channel |
J

(a)                                                     (b)

M1841 다중경로 페이당의 전형적인 YBA SE: (a) 시간 도메인 (6) 주파수 도메인

195



===== PAGE 201 =====
ZY 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

단일 반송파 직렬 고속 무선 데이터가 다중경로 페이딩 환경에서 전송된 47S 고려
해 보자. 4.1장에서 언급한 바와 같이, 초당 수 메가비트의 속도로 디지털 데이터가 전
송되고 다중경로 페이덩에 의한 지연파의 최대 지연시간이 1/6보다 크다면 지연파들
의 최대 지연시간은 1 심볼 시간보다 크다. 그림 4.1은 지연파의 최대 지연시간이 1 심
볼 시간을 초과할 때 단일 반송파 직렬 고속 무선 데이터 전송기법의 파형을 시간과 스
펙트럼 도메인에서 보여준다. 파형과 스펙트럼 모두 왜곡되어 있으므로 이 왜곡신호를
균등화해줄 필요가 있다. 신호를 균등화하는 한 가지 방법으로 적응 균등화 기법을 사
용할 수 있는데 이는 수신기에서 채널 임펄스응답을 추정하고 수신기에서 수신신호와
추정된 임펄스응답의 공액복소수를 곱해주는 기법이다. 그러나 초당 수 메가비트의 높
은 속도를 갖고 단순하고 저가의 하드웨어를 통해 이 균등화 과정을 수행하기는 어려움
이 따르는데 이는 그림 4.1에 보인 바와 같이 수신 데이터에서 송신 데이터를 복원하면
수신 데이터를 연속적으로 균등화하기 위해서는 다수의 연속적인 ASS 저장해아하
기 때문이다. 이런 이유로 다른 해결법을 모색한다.

주파수 도메인 관점에서 전송신호가 다중경로 페이덩에 영향을 받을 때, 신호의 어떤
PES 발전적인 간섭으로 레벨이 증가하고 다른 부분은 파괴적인 간섭으로 레벨이 감
소하여 때로는 소멸될 수도 있다. 일반적으로 서로 가까운 주파수 대역은 신호 강도에
있어서 같은 ASS] 영향을 받을 것이다. 높은 상관 값을 갖는 주파수 대역폭을 코히어
런트 대역폭이라 부른다 [3]. 협대역 신호에서 ASS 일반적으로 신호의 대역폭이 코
히어런트 대역폭보다 작으면 최소화된다. 그러나 어떤 경우에는 신호가 심각한 감쇠가
될 가능성이 존재한다. 코히어런트 대역폭보다 큰 대역폭을 점유하는 ASE 왜곡되기
쉽지만 다중경로 페이덩의 영향을 받아도 총 수신파워의 변동이 적을 것이다.

다중경로 페이덩 환경이 야기하는 문제점들을 해결하고 광대역 이동통신을 달성하
기 위해서는 여러 채널에서 고속의 전송 데이터를 저속의 병렬 데이터로 변환하는 병렬
전송이 필요하다. 이 데이터들은 하위채널 (61608800619) 간의 구분을 위해서 몇 가지
U}-$3}7|= (multiplexing techniques)°]] 의해 다중 송신된다.

6 『

그림 4.1은 병렬 전송기법의 효과를 보여준다. 주어진 데이터 전송률에 대해, 병렬 전
송 채널이 증가함에 따라 개개의 하위채널이 전달해야할 데이터 전송를은 감소하게 되

196



===== PAGE 202 =====
직교주파수분할다중 (OFDM) 전송기법  10 |

는데 다른 말로 하면 심볼 주기를 연장한다. 결과적으로 지연파의 지연시간은 1 심볼 시
간 이내로 감소된다.

하위 채널 간 RES 위해서, 주파수 분할 OS frequencydivision multiplexing
(FDM)3} 코드 분할 = codedivision multiplex (CDM)°] 자주 사용된다. 어떤 경우
에는 Al 번째 방법을 다중반송파 전송, 두 번째 방법을 다중코드 전송이라 부른다. 그림
4.2는 두 병렬 전송기법의 구성을 보여준다. OFDMS 다중반송파 전송기법이고 가장

효과적이 방법이다.
4.3장은 OFDM 전송에 대한 개념을 기술한다.
este                                                          —
caer                이가 고
Code 1                           Code 1
whey Get ote LY LJ
커야  oi  Code 2         Sum               00002              『/아->
Binary      speed    3                                3                   Binary
high        data      로                                1                   high
speed      tate Se nicer                L—_re—o{ [f+     coed
i Oe!      Code N                    Code N         FE Nop
(a)
| 60                —e—[ Tp |
Freq.1                            Freq.1
eS        >       Be       -—>e-—>| f }거
= 19  ag  ec         Sum        ia    Freq.2             P/S}—>
Binary        si                                    +                   Binary
high        roe     ,                               1                   high
speed      —                                  7       speed
-     —            Freq.N                                       Freg.N                 ~ 매뽀

를 그림 4.2 병렬 전송 시스템: (a) 다중코드 전송기법 (6) 다중반송파 전송기법

ㅣ | OFDM 전송기법에 대한 개념

OFDM 전송시스템의 역사와 원리에 대해서는 우리의 이전 책 [3]을 추천한다. 이 장
에서는 OFDM 전송기법의 개발과 응용에 초점을 맞춘

Ae re

197



===== PAGE 203 =====
Zy  최신 이동통신시스템
c                  4

Mobile Communications using MATLAB Simufation

4.3.1 송신기 구성

그림 4.3(2)는 OFDM 송신기의 구성을 보여준다. 송신기에서, ASHE 고속 데이터
는 AN 개의 하위채널의 병렬 데이터로 변환된다. 그 다음, 각 병렬 하위채널의 전송
데이터는 3장에서 논의된 PSK 기반 변조방식에 의해 변조된다.죄 채널의 직교변조 데
이터 AAA (dy, dj, 4, …, dy_))& 고려하자. 각 d,& 2,= 0, + 70,.의 복소
수이고 0,과 do 은 QPSKAAE {1,1}이고 16(0414에서는 {41,3}이다. 이 변조
데이터가 역 고속 푸리에변환 16096 fast Fourier transform (IFFT) 회로에 입력되고
OFDM 신호가 생성된다. 전송 데이터는 다음과 같이 주어진다.

으> |으>

Guard 도 1600
-—>i time     time [>| FFT

S(t} insertion| S(t) (t)) removal

>

(a)                       (b)
를 그림 4.3 OFDM 무선전송 시스템: (a) 송신기 (6) 수신기

st) = > Yd, ®exp(j2af ¢- kT) f(t- kD)

k=-« i=0

y 'G, (k) + 74, (k) \cos(2af, (t — kT,))+ jsin(2af, (t - kT,))) f ((-KT,)

는

iMs ate

0, (k)cos(2af, (t - KT, ))— dp (k)sin(2af, (t- KT,)) )f ¢-kT,)

ui 20 (k)sin(2af, (t - KT,))+ dp (k) cos(2af,(t- KT,)) )f kT.)
(4.1)
이때 7, OFDM 신호의 심볼 지속시간이고 /, (7=0, 1, 2,…)는 다음과 같이
주어지는 7번째 하위반송파의 주파수이다.
198



===== PAGE 204 =====
직교주파수분할다중 (OFDM) 전송기법   lo |

i
f; =fo 호                       (4.2)
여기서, 7(?)는 4 심볼의 BA 파형이고 다음과 같이 정의된다.
| (07982)
70 oid   (otherwise)                  (4.3)

Real part                     Imaginary part               Ce
>         >  C=1-j:h=0
은 f*. one  8 7 >  C=1+j:f=V7,
NI    eae.

를 그림 4.4 2 하위채널에서 OFDM 전송신호

199



===== PAGE 205 =====
최신 이동통신시스템

200

Mobile Communications using MATLAB Simulation

이제 보호간격(64870 interval)ol] 대해 기술하고자 한다. ISIS} 전송채널 왜곡에 의한
반송파간 간섭-066708106[ interference oa   존재하지 않을 때 OFDMA] 하위 채
널의 직교성은 유지될 수 있고 각 하위채널들은 수신기에서 회로를 이용해 완전하
게 분리될 수 있다. 그러나 Aaa oz 이런 조건들은 구현되기 어렵다. OFDM 신호의
스펙트럼 대역이 강하게 제한되지 않기 때문에 다중경로 페이딩에 의한 왜곡이 각 하위
aide] eV} 인접한 As 퍼지게 만든다. 게다가 aE Aa ADAH 가
진 지연파가 다음 ABS 오염시킨다. 왜곡을 줄이기 위한 간단한 방법으로 심볼 지속
시간 혹은 Washo] $8 SoA + 이다. 그러나 이 Bale 도플러 주과수와 FFT 2
기에 대한 반송가의 안정성 문제로 구현이 어려울 수 있다.
ISIE 제거하는 한 가지 방법은 반복적으로 확장된 보호간격을 생성하는 것인데 [21,
각 OFDM 심볼은 신호 자체의 주기적인 확장이 선행된다. 총 심볼 지속시간은
T a= Tet 7`,가 되고 7',는 보호간격이다. 그림 4.5는 전형적인 보호간격을 보여
준다. 각 심볼은 두 부분으로 구성된다.

Symbol M - » gest              Symbol M                       ) bo   {Symbol M+1

A

x)
Vv

개

Time

4
vv

수 1



===== PAGE 206 =====
aia)

전체 ASE 능동 심볼에 포함되어 있고 이의 마지막 부분은 심볼의 시작 부분에 다

시 반복되고 보호간격이라 블린다. 보호간격이 채널 WASH 혹은 다중경로 지연보

다 큰 경우에 ISI 효과가 AAS 수 있다. 그러나101 또는 26800 페이딩은 여전히 존재

한다. 보호간격과 유효한 심볼 지속시간의 비는 응용 분야에 따라 결정된다. 보호간격

의 삽입은 데이터 HSS 감소시키게 될 것이기 때문에 TABS 7`,/4보다 작다.
보호 간격의 삽입 후에 OFDM 신호는 다음과 같다.

c

기

s(t) = >: >.4.0000024;0-..0/70-..0)

k= i=                                     (4.4)
위 식에서 /“(7)는 다음과 같이 정의된 각 심볼의 변형된 펄스 파형이다.
Pe  io Gd, Sia)
{O-  0 <- Tie              (4.5)

OFDM 신호는 수신기로 전송된다; 그러나 전송된 데이터 $*(《)는 다중경로 페이딩
과 4\0씨에 의해 오염된다. 수신기에서, 수신신호는 다음과 같이 주어진다.

r(t) = |, A(e,t)s(t-r)dr +n)                   (4.6)

이때, ACr, 2)는시간 /에서 FAA SS] 임펄스응답이고 n(t)= 복소수 AWGN?)
다.

4.3.2 수신기 구성

그림 4.3(6)는 OFDM 수신기의 블록도를 보여준다.   수신기에서, 수신신호 7(7)는
신호 왜곡이 거의 없는 충분히 넓은 통과대역을 가진 대역통과 필터에 의해 필터링된다.
직교 검출기가 신호에 적용되는데 신호는 때 대역으로 하위 변환된다. 그 다음, 신호는

201

|교주파수분할다중(야미/) 전송기법 ㅣ).


===== PAGE 207 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

측주기 [iT totais tT tat TIAA 신호의 푸리에 계수를 얻기 위해 FFT 회로에 4
용된다. 번째 OFDM 하위채널의 FFT JES 출력 2,(4)는 다음과 같이 주어진다.

수        1] ple Tai

d, (k= J r@expl- 722, (kT oui) at         a
만약 다중경로 페이딩 환경의 지연파 #,(/8의 특성을 추정할 수 있다면, 수신 데이

터를 다음과 같이 균등화할 수 있다.

(31020                           (4.8)

여기서 *는 공액복소수를 의미한다.

@,와 @(k)= 비교함으로써 BER 성능을 계산할 수 있다. BERS 수신기 잡음의
레벨에 의해 결정된다. OFDM 전송에서 직교성은 유지되고 BER 성능은 각 하위채널
에서의 변조방식에 의해 영향 받는다. 그래서 BPSK7} 사용되면 4\0씨과 단일경로
레일리 페이딩 채널에서 BERS 각각 (3.17)과 (3.18)에 보인 이론치와 같다. 다른 변조
방식의 경우 BER 성능의 변조방식과의 관계를 표 4.1에 나타내었다.

PH 4.18 일반적인 변조방식에서의 BER 성능
이론적인 BER
변조방식
태이                  HUBS Rayleigh 페이딩
1        1
1                                 98 프
BPSK     5 erfel (EN, )                        :     Le
E,/N,
if       oaks
1                                   as
QPSK     00016, 7, )                       ~
2720; 4

202



===== PAGE 208 =====
직교주파수분할다중 (OFDM) 전송기법   rz

3    2      9    2         3      1    |
16-QAM    하기스 시 1 N 스이 고        ==
as    8  | 이채  1] 24  | %  ]    | J1+5/(2E, /N,) |

7   1     49    1       7      1
64QAM | —erfe| /—E,/N, |-——erfc] 기 /N,     rel bv rete IRE
이    24  | (ae  ] 384  | Get  i   24| /1+7/(E,/N,)

15    4      225    [4      15|      1
256QAM | —erfc .|—E,/N, |-     erfe*) ,|—E,/N, || —|1-
ie   64  | 85°  ㅣ 2,048  | 85°  | 64  나

4.4장은 컴퓨터 시뮬레이션을 통한 OFDM 송수신기의 구성에 대해 소개한다.

| 컴퓨터 시뮬레이션을 통한 구성

이 장에서는
계산한다. 시뮬레이션의 블록도는 그림 4.6에 제시한다. 이 장에서 사용된 모든 시뮬레
이션 프로그램은 표 4.

gol

수명           기능               입력 데이터                 출력

ofdm.m        AWGN (프로그램
(Program 4.1) | 4.1)과 단일경로
ofdm_fadingm ㅣ Rayleigh 페이딩 채
(Program 4.2)   널 (프로그램4.2)에

ber: bir error rate 성능

ta

서의 28&성능계산
giins.m             보호 간격 삽입         -idata: 입력 Ｌ채널 AJA            viout: BS 간격이 삽입
(Program 4.3)                                - qdata: 입력 채널 ABA             된 채널 데이터
- fftlen: FFT 포인트 수                        - gout: 보호 간격이 삽입
ㆍ0160: 보호 간격 길이                    된 채널 데이터
nd: 심볼 수

203



===== PAGE 209 =====
최신 이동통신시스템

AQ

Mobile Communications using MATLAB Simulation

표 4.2(계속)

함수명            기능                 입력 데이터                  출력
girem.m              보호 간격 삭제           -idata: 입력 채널 AAA               -iout: 보호 간격이 삭제
(Program 4.4)                                    -qdata: 입력 채널 AAA              된 La 데이터

: 1602: 심 볼당 포인트 수                “gout: 보호 간격이 A}
-gilen: 보호 간격 길이               제된 (채널 데이터
nd: 심볼 수
ofdmda.m                 AWGN3} 단일경로 | 무                                                                - ber: bir error rate 성능
(Program 4.5)        Rayleigh 페이덩 채                                                               ‘per: packet error rate
널에서의 BER 성능                                  성능
계산
cermapping.m        부반송파에 데이터 | 10868: 입력 Ｌ채널 데이터 AAA | -iout: Ｌ채널의 맵핑된
(Program 4.5)        를 설정                       -qdata: 입력 채널 데이터 AAA ㅣ 데이터
00160: IFFT 포인트 수                     - gout: Qa] 9] 맵핑된
“nd: 심볼 수                데이터
erdemapping.m | 반송파로부터 데이 | 1086: 입력 Ｌ채널 데이터 AAA | -iout: Ｌ채널의 디맵핑
(Program 4.7)        터를 분리                   -qdata: 입력 채널 데이터 AAA | 된 데이터
10160: FFT 포인트 수          - gout: Q-a' 9] 디맵핑
ofdmce.m                AWGN} 단일경로 | +                                                            - ber: bir error rate 성능
(Program 4.8)        Rayleigh 페이덩 채                                                               -per: packet error rate
널에서의 BER 성능                               성능
계산
ofdmci.m                  AWGN} 단일경로 | 무                                                                - ber: bir error rate 성능
(Program 4.9)         Rayleigh 페이딩 채                                                               -per: packet error rate
널에서의 BER 성능                               성능
계산
interwave.m          간섭파를 형성             “ci: 반송파와 간섭 파워의 비             -iout: Ｌ채널의 간섭
(Program 4.10)                                    - spow: 반송파의 파워                    - gout: 아채널의 간섭

“mi: 간섭의 변조 레벨
-nsamp: 샘플 수

-tstp: 시간 해상도

ㆍ180108 para: 페이덩 매개변수

204



===== PAGE 210 =====
직교주파수분할다중 (OFDM) 전송기법

이 장에서는 프로그램 4.14.3을 사용한다. 주된 프로그램은 프로그램 4.1이다. 프로
그램 4.1에서는 먼저 주된 프로그램에서 사용할 공통 변수들을 선택한다.

para=128;   %
fftlen=128; %
noc=128;    %
nd=6;       %
ml=2;       %
sr=250000; %
br=sr.*ml; %
gilen=32;   %
ebn0=3;     %

Number

of parallel channel to transmit (points)

FFT length

Number
Number

of carrier

of information OFDM symbol for one loop

Modulation level : QPSK

Symbol

rate

Bit rate per carrier

Length
Eb/NO

of guard interval (points)

그림 4.67} 위 매개변수들에 보인 바와 Zo] 128 하위반송파와 4-ys 심볼 시간
(tstp=1./sr) 그리고 1/4tstp 보호간격을 가진 OFDM 시스템을 시뮬레이션 한다.
다음으로 각 채널에서 QPSK 변조기법을 사용하는 시뮬레이션 변수들을 정의한다.

nloop=100; %
noe=0;      %
nod=0;      %
eop=0;      %
nop=0;      %

Number
Number
Number
Number
Number

of simulation loops
of error data

of transmitted data
of error packet

of transmitted packet

모든 변수를 정의한 후에 BER3} PER 성능을 얻기 위해 시뮬레이션을 수행한다. 먼
저, OF} 1로 구성된 167%13*00*01 벡터의 랜덤 직렬데이터를 생성한다. 이 벡터를

“seldata”2}31 부른다.

seldata=rand(1,para*nd*ml)>0.5;

직렬데이터 벡터 “seldata”3= 병렬데이터 벡터 “paradata”= 변환되는데 이 벡터는
para-by-nd*ml 벡터로 구성되고 QPSK 변조방식을 사용하는 128 하위채널에서 병렬

ASS 가능케 한다.

paradata=reshape (seldata,para,nd*ml) ;

[ich, qch]=qpskmod (paradata, para,nd,ml) ;

205



===== PAGE 211 =====
Mobile Communications using MATLAB Simulation

009)
pied x y x pu x jw

t        (jeuueyo jajjesed iq)        Zsojyesuaduioa | || so}esuadwoa

(019) pu x jw x eved             ｌ              yx pu x jw                         Buipey                 Buipey
수                 ㅣ               4                 H
ㅣ                 1 ]194844020| ㅣ                  4
438 <4Jojesusdwio) ,   uoisiveg fel   gine ql   ae    uoneinpowaq)
jayjesedg
Joyesaueb               1404281800|@
89104                    1881
ueissneg               JaMOod}<€
(jauueyo jajjesedq)                               (ug)
yx pu               YX pu x jw x eved
<                                                    es         (jeuueyp jajjesed/iq)       A
“                                                                I                 yx pux jw               ㅣ             009) pu x jw x 6400
<                                            i                                 .                 4
|               (wajsAs                     !                4               :        ©   |  /
ssedmoj | ,             |            1 ]1948444023| ㅣ
6@)<-  4006240[*      @<—       quajeainba) | ~          we 1     oneinpoy   ; | lenesed| | | Guipoo   - yojesaueb
-o1yauAs    %                japow |.             >                  O}7" = Jjauueyd ie        0160
©                                       jauueyo|                     1                     1008
이084
1101104400
jayjesed |                     eyep
0 | ^                     1이0
101186

=

=

다음과 같이 데이터

ㄴ~

컴퓨터 시뮬레이션
ㄴㄴ

t

ㅎ
4

데이터

==
=

그림 4.7에 보이 것과 같이 구성된다. Ｌ채널과 0

그림 4.8에 보였다. 그 후, 이

가된다.

ee

레임 형태

5 적

~

를 그림 4.6 OFDM 시스템의 BERS 계산하기 위
, ay

시뮬레이션 모델의
Was] 전송 데이터

A

정규화하기 위해 kmod 배

206


===== PAGE 212 =====
직교주파수분할다중(004) 871i Oe

 :1000008000. data

Guard interval

para channel
Frequency

nd symbols

를 그림 4.7 시뮬레이션 모델의 프레임 형태

Transmission data I-channel

0                    20                    40                     60                  80                   100                   120                140
Frequency (subcarrier number)
{a)

Transmission data Q-channel

Amplitude
©
=

가

04h

&
1

&

0             20             40             60              80            100            120           140
Frequency (subcarrier number)
(b)

를 그림 4.8 (a) |채널의 AS 데이터 (6) @채널의 전송 데이터

207



===== PAGE 213 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation

kmod=1/sqrt (2);
ichl=ich.*kmod;
qchl=qch. *kmod;
맵핑 이후에, 이들 주파수 축의 병렬 데이터는 IFFT 회로로 입력된다. 회로에서, 병
렬 데이터는 OFDMS 사용하여 시간 축의 직렬 데이터로 변환된다.

x=ichlt+qchl.*i;

y=ifft (x);      Ser Epes pure in funet ion
ich2=real (y);   % real : built in function
qch2=imag (y) ;   % imag : built in function

입력과 출력은 그림 4.9에 보였다. 다음으로, 보호간격이 ich2S} qch2o] 다중경로 페
이덩에 의해 야기된 ISIS 제거하기 위해 삽입된다.

{ich3,qch3]= giins(ich2,qch2,fftlen,gilen,nd) ;
fftlen2=fftlentgilen;

#0 ——0     마나
#1 —1     1-—
2.—2     하느
2  #61 ——61     6-- 8
‘Ss 62 ——02    e2}-—— £
든 0010    바0=
응 #-64 -ㅡ164 IFFT 64   2
S #-63 ——65     65    =
S #-62 ——66    66   은
오 #*-61-ㅡ67     67} F
uw  ㆍ 자 구내       | 제 빼
ㆍ -ㅡ12   124}
#-3 -ㅡ125    125-ㅡ
#-2 ——126    12 |
#-1—127    127
를 그림 4.9 그림 49 IFFT] 입력과 출력

208



===== PAGE 214 =====
직교주파수분할다중(야마) 전8기본 Oe

이 지점에서, 우리는 84602를 보호간격을 포함한 심볼의 길이로 정의한다. 그 후, 필
터링된 Ase 대기로 전송된다. Ｌ채널과 0-채널의 OFDM 변조 데이터를 그림 4.10에
보였다. 전송된 신호는 무선채널 (저대역통과 시스템과 동등한)을 통해 수신기에 전송
된다.

Transmission signal |-channel

0.15

01 | 고 ih 」       li |

Amplitude

0.1      +
| a

0 100 200 300 400 500 600 700 800 900 1000
Time (sampling number)
(a)

Transmission signal Q-channel

=       bod tht 0!     !

-0.1  +  |    | 기여 T  | |

0100. 200 300 400 500 600 700 800 900 1000
Time (sampling number)

(b)

를 그림 4.10 (a) tye ASUS (b) @채널의 ASH

loli

209



===== PAGE 215 =====
ZY 최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation
수신기에서, PAA SE 먼저 AWGN] 의해 오염된다. 잡음 B= comb.m 함수를
소개한 3.2.3장에서 이미 소개되었다. 이 시뮬레이션에서는 2,/2/,과 BERS] BAS
보여주는 그래프를 생성하기 원한다. 이는 주어진 L,/ Np 따라 “302”을 변화시켜야
함을 의미한다. 변수 “302”은 889에서 사용된 것과 유사한 과정에 의해 계산되었다.
여기서, “spow"= 심볼 당 반송파 당 신호 파워를 의미한다. OFDM 시스템에서
“…00\"”는 병렬 하위반송파의 수를 뜻하는 “para” = 나뉘어져야한다.

8 89003 10811. in function

spow=sum(ich3.*2+qch3.*2) /nd./para;
attn=0.5*spow*sr/br*10.*% (-ebn0/10) ;
attn=sqrt (attn) ;

“attn” 2} comb.m& 사용하여 전송 데이터는 AWGN] 의해 오염된다.
[ich4, qch4]=comb (1013 , qch3, attn) ;
다음으로, FAIAIS ich4 9} qch4q A] 보호간격이 제거된다.
[ich5,qch5]= girem(ich4,qch4,fftlen2,gilen,nd) ;
시간 축의 데이터 “ichS” 2} “qch5”7} FFT 회로에 입력된다. 회로에서, 직렬 데이터
가 주파수 축의 병렬 데이터로 변환된다.

rx=ich5+qch5.*i;

ry=fft (rx) ;       % ft. puritan. function
ich6=real (ry) ;    % real : built in function
qch6=imag (ry) ;    % imag : built in function

변환된 데이터는 각 채널에서 데이터를 비정규화하기 위해 “0000"로 나뉘어 지고
복조 함수로 입력된다.

ich7=ich6./kmod;
qch7=qch6./kmod;
[demodata]=qpskdemod (ich7,qch7,para,nd,ml) ;

210



===== PAGE 216 =====
직교주파수분할다중 (2ㅁㅁ4) 전송기법  4

복조된 데이터는 16%ㅠ000*00*71 벡터로 변환된다. 이 데이터는 “860100801”이라
린다.

demodatal=reshape (demodata,1,para*nd*m1l) ;

부
=

다음으로, 비트 오류의 수를 계산한다. 과정은 2.340] 기술되어 있다. 동시에, 패킷
오류의 수도 계산한다. 이 시뮬레이션에서, 송신 데이터는 “9610312@”로 수신 데이터는
“…%0602008131”로 부른다. 계산은 다음과 같이 수행되었다.

% instantaneous number of error and data

noe2=sum(abs (demodatal-seldata)); % sum : built in function
nod2=length(seldata); % length : built in function

% cumulative the number of error and data in noe and nod
noe=noet+noe2;
nod=nod+nod2;
% calculating PER
if noe2~=0
eop=eopt1;
else
eop=eop;
end
eop;

nop=nopt1;
다음 과정으로 BER} PERS 얻는다.

ber=noe/nod;

per=eop/nop;

메인 프로그램을 실행시킨다,

ofdm

211



===== PAGE 217 =====
ax 이동통신시스템

212

Mobile Communications using MATLAB 5/0776/27707?

1.00E + 00

so oa

5
5
"
5
|
L
ia
5
¥
y
| a
ia

…… BPSK theory

— BPSK 1 path Rayleigh theory

~& QPSK AWGN (no compensation)

-@ OPSK 1 path Rayleigh (perfect compensation)
=#& OPSK 1 path Rayleigh (no compensation)

E,/N, (dB)

를 그림 4.11 BER NS (para=128)

BERS} PERS. 긴 시뮬레이션 후에 얻어진다. BER 성능은 그림 4.11에 보였는데 이

론적인 값과 비교하였다. 시뮬레이션 결과에서 이론적인 값과 비교하여 0.9691-08의
전이가 있었다. 이 전이는 수신신호에서 보호간격 파워를 잘라냄으로써 야기된다. 이
는 다음과 같이 계산된다.

shifted value (dB) = -10log1
(4.9)

gilen ]
fftlen2

이전에 보호간격을 0104으로 보호간격을 포함한 심볼의 길이를 846202로 정의하였
다. 그림 4.11에 단일경로 평탄 레일리 페이딩 하에서 BER 성능을 보였다. 시뮬레이션
oe eee eee
페이딩을 생성하기 위해 다음 매개변수들을 추가하였다.

% Generated data are fed into a fading simulator

[ifade, qfade]=sefade (ich3,qch3,itau,dlvl,th1,n0,itnd1,nowl1,len
gth (ich3)      fd;-flat)?

% Updata fading counter

itndl = itndl+ itnd0;

,tstp,



===== PAGE 218 =====
직교주파수분할다중 (OFDM) 전기 ㅠㅠ

변수 “flat”-S 1이나 0으로 정의함으로써 시뮬레이션을 사용해 페이덩 채널이 자동
적으로 보상될지 그렇지 않을지 결정할 수 있다. 단일경로 레일리 페이덩 하에서의
BER 성능은, 전송 특성에 의해 야기되는 ASH 위상의 변동을 완벽하게 보상할 수 있
다면, 이론적인 값으로부터 0.969-08 전이시킬 수 있다. 그러나 변동 SYS 보상하지
못한다면 데이터를 복원할 수 없다. 실시간으로 전송 특성을 추정하는 것이 중요하다.
한 가지 추정 방법은 그림 4.12에 보인 바와 같이 알고 있는 주기에서 알고 있는 Beal
심볼을 삽입하는 TH BA] S 삽입법이다. 수신기에서 모든 심볼에 대해 채널 특성을
추정할 수 있다.

추정된 전송 특성을 사용해 전송된 데이터를 복원할 수 있다. 4.5장은 이 방법에 대해
자세히 기술한다.

WE) tress 심볼-기반 (Pitot Symbor-Aided) OFDM 변조방식

이 장에서는 페이덩에 의해 생기는 진폭과 위상의 변동을 보상하는 방법에 대해 설명
한다. 이 방법은 ype] Bl 심볼-기반 OFDM 변조방식이라 불린다. 이 방식에서는, Bas
심볼이 그림 4.12에서와 같이 고정된 시간간격에 송신기에서 삽입되고 수신기에서는
HUB ASS 통해 채널 특성을 추정한다. ASS] 레벨이 각 하위반송파 채널과 무관
하기 때문에 알고 있는 시간 주기에 모든 주파수 도메인에서 Belel 반송파를 삽입할
수 있다. 그 다음 추정된 채널 특성을 통해 송신 데이터를 복원할 수 있다. 이 장은 파일
3] 4) S-7) 8 OFDM 변조방식의 구성을 보이고 컴퓨터 시뮬레이션을 통해 BER 성등
을 평가한다.

시뮬레이션의 블록도를 그림 4.6에 나타냈다. 4.4장의 시뮬레이션과 비교해보면 이
시뮬레이션은 보다 실제 상황에 가깝다고 할 수 있다. 이 시뮬레이션에서 = ETSI
BRAN, IEEE 802.11 그리고 ARIB MMAC 프로젝트에서 사용된 OFDM 기반 WLAN
시스템을 사용된다.

213



===== PAGE 219 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

a      a fading
| Jrasing i  V7) Pilot data

ㅣ                               ㅣ      Ee] ‘Information data

Guard interval

4                Ce Re

OS

eZ               4006

로 [그           he |
뜨다 23              C4,
EL.              Fe
~              Z

2                 Aa

Time ms

Mle 412 시뮬레이션 모델의 프레임 형태

D 하위반송파의 수: 52개의 하위반송파가 적용되었고 64-지점 FFT 회로에 의해 생
성된다. 52개의 하위반송파 중 48개가 정보 데이터를 위해 사용된다. 나머지는
위상 잡음을 보상하기 위해 사용된다. 이 시뮬레이션에서, 위상-잡음 환경을 시뮬
레이션하지 않는다. 그래서 모든 52 반송파에 데이터를 입력한다. 그림 4.13은 64
-지점 IFFT 회로의 52 반송파의 주파수 할당을 보여준다.

Null — 0    0-—
1 -ㅡ1    1
2 —42    2
oF encanta      =
S  —      beeen
2 #-26 —126    2 을
들   —27    27 €
= Null—4     r— 은
sii—y~ FT 3
중 Null —4      r-— 5
더   437    37 >
foes. fos
nu
#-2 —62    62
#-1--ㅡ163    6

alg

@ 28 4.13 IFFTO 입력과 출

214



===== PAGE 220 =====
직교주파수분할다중 (OFDM) 전송기법  io |

One frame unit

A

—
>

G

cE [Gi] Data] Gi] Data |이| 088 | GI] Data | GI] Data | GI] Data

를 그림 4.14 시뮬레이션된 OFDM 전송의 프레임 형태

@ 보호 간격: 80076: 지연시간이 AS 길이보다 큰 다중경로 페이덩의 효과를 피
하기 위해서 주기적으로 확장된 신호가 각 OFDM 앞에 삽입되었다. 우리는
800ns2] 보호간격을 사용하였는데 이는 실내 환경뿐만 아니라 실외 마이크로셀
룰라 환경을 위한 OFDM 기반 무선통신 시스템을 고려해야하기 때문이다. %-
GHz 환경에서 800ns2] 간격은 주요 지연파를 다루기에 충분하다. 그림 4.14는
시가  프레임 형태와 각 OFDM 심볼의 구성을 보여준다.

sa 레이트: 샘플링 레이트 (20 MHz)= IFFT 입력 신호의 입력-신호

. 이는 우리가 2054628보다 큰 총 전송률을 달성하기 원하기 때문이다.

이  변조방식: WLAN 환경에서 D8PSK 9} 같은 미분 부호화와 검출기반 변조방식ㅇ

사용된다. 그러나 여러 표준화 위원회에 따라서는, 광대역 데이터 단말기의 사

JU] 환경뿐만 아니라 실외 마이크로 age 환경에서도 가능하다. 이런 이

]내뿐만 아니라 실외 환경에서도 전송 데이터의 SAS 향상시키고 다중경

Blo] Qo] 맞서 강성을 유지하기 위해 사용되는 8289, QPSK, 8PSK, 16-
(00434과 같은 코히어런트 검출기반 변조기법을 논의한다. 이 하위 장
(9409600020)은 (4.4장의 결과와 비교하기 위해) 코히어런트 QPSK 기반 OFDM
시스템을 사용한다.

© FEC: 기본적으로, FECE 컨볼루션 코딩과 #=1/2와 K=7 (R=coding rate,
K=constraint length)2] soft-decision Viterbi 디코덩에 기반 한다. 다른 코덩 레이
트에서는 24000400 컨볼루션 코딩과 600601910ㅁ Viterbi 디코덩을 사용한다.
그러나 이 하위 장은 부호화 방법에 대해서는 논하지 않는다.

© 프레임 형태: 그림 4.14는 시뮬레이션된 OFDM 시스템의 프레임 형태를 보여준

nu

다. 프레입은 두 부분으로 나넌다. 채널추정 (CE) 심볼과 송신 데이터 심볼. 이 장

i)
oz
e   때

A

도와

9
별

오래

30 ob

be 따오
봉 ©

215


===== PAGE 221 =====
Ax 이동통신시스템
Mobile Communications using MATLAB Simutation

216

에서는 하나의 CE 심볼과 6개의 AS 데이터 ABS 하나의 프레임 단위로 사용
한다. CE 심볼에서 BAUS 데이터로부터의 진폭과 위상 편차는 BVA ASS 이
용해 측정된다. 측정된 AS 특성을 기반으로 6개의 OFDM 데이터 심볼의 다중
경로 페이덩에 의해 야기된 진폭과 위상 편차는 보상된다. 이전 장의 결과에 기반
한 부드러운 통신을 위해 다음 과정을 시뮬레이션했다.

ㆍ52-반송파 B]-a} eS] B14] 7] Bt QPSK-OFDM 전송기법

ㆍ52-반송파 BIA] 7] 8 QPSK-OFDM 전송기법

ㆍ52-반송파 파일릿심볼-기반 QPSK-OFDM 전송기법 (AWGN, 단일경로 레일
리 페이덩, 이중경로 레일리 페이딩 하에서의 4,/4^/, 대 BER 혹은 2,/^, 대
PER)

ㆍ52반송파 BIS 심볼-기반 QPSK-OFDM 전송기법 (반송파대-간섭의 비 대
BERZ} PER)

(2) 무선 채널 모델:이 시뮬레이션에서 보통의 단일경로 레일리 페이딩과 이중경로
레일리 페이덩 채널을 사용한다. 이중경로 레일리 Mol” 환경에서, 지연파의 지
연시간은 매우 중요하다. 이 시뮬레이션에서, 보호간격은 80008이다. 그래서 지
연시간은 25028로 지정한다. 또한, 도플러 주파수는 7=50 Hz (3 m/s@5 GHz)
혹은 /2=150 Hz (15 m/s@5 0112)를 사용한다.

시스템 성능을 평가하기 위해, 비트 오류 확률뿐만 아니라 PERE 시뮬레이션했는데
PEROAT 패킷은 한 프레임 단위에 전송되는 데이터의 수로 정의된다. 이 경우, 6개의
OFDM 심볼이 한 심볼 단위에 존재한다. 한 프레임에서 하나 이상의 전송 데이터가 오
류가 나면 패킷 오류가 발생한다.

시뮬레이션 AS 위해 프로그램 4.5에서 4.7까지의 모든 프로그램이 사용되었다. Zz
로그램 4.5에서는 먼저 프로그램 4.1에서 사용한 공통변수를 결정한다.



===== PAGE 222 =====
직교주파수분할다중(04) 전기번 를

para=52;
fftlen=64;
noc=53;
nd=6;
ml=2;
sr=250000;
br=sr.*ml;
gilen=16;
ebn0=3;

00 00 00

00 0 0 0

00 oP 00

Number of parallel channel to transmit (points)
FFT length

Number of carriers

Number of information OFDM symbol for one loop
Modulation level : QPSK

OFDM symbol rate (250 ksyombol/s)

Bit rate per carrier

Length of guard interval (points)

Eb/NO

다음으로 페이덩 변수를 초기화한다.

tstp=1/sr/ (fftlen+gilen) ;

itau=[0];

dlv11=[0];

n0=[6];

thl=[0.0];

itndl=[1000];

nowl=1;

fd=150;
flat=0;

Time resolution

Arrival time for each multipath
normalized by tstp

Mean power for each multipath

normalized by direct wave.

oe 00 oP 0 oP 0

Number of waves to generate
fading n0(1),n0(2)

Initial Phase of delayed wave

00 00

ole

set fading counter

ae

Number of directwave

% + Number of delayed wave

00

Maximum Doppler frequency
% Flat or not (see ofdm fading.m)

itnd0=nd* (fftlen+gilen)*20; % Number of fading counter to skip

시뮬레이션을 위한

nloop=1000;
noe = 0;
nod = 0;
eop=0;
nop=0;

oe 0

00

변수를 정의한다.

Number of simulation loops
Number of error data
Number of transmitted data
Number of error packet

Number of transmitted packet

217


===== PAGE 223 =====
ZY  최신 이동통신시스템

Mobite Communications using MATLAB Simulation

모든 UTS 정의한 후에 BER PER 성능을 얻기 위해 시뮬레이션을 시작한다. 먼
Al, OF} 12] 랜덤 직렬 데이터를 생성하는데 167ㅠㅁ818*ㅁ0” 벡터를 고려하자. 이 데
이터를 “600812”라 부른다.

seridata=rand(1,para*nd*ml) >0 . 5;
“seridata’= 병렬로 전송하기 위해 parabynd*ml= 구성된 “paradata”= 변환된다.

paradata=reshape (seridata, para,nd*m1l) ;

다음으로 YE} paradatae 맵핑희로로 입력된다. 이 희로에서 병렬 데이터는 미리 정
의된 맵핑 방법에 따라 두 채널 Ich} 0애의 병렬 데이터로 변환된다.

[ich, qch]=qpskmod (paradata, para,nd,ml) ;
그 다음, 이 데이터는 정규화하기 위해 다음과 같이 kmod 배 증가된다.

kmod=1/sqrt (2); % sqrt : built in function
ich=ich.*kmod;
qch=qch.*kmod;

주파수 도메인에서 Ich3} 0애의 AS 데이터는 그림 4.13에 보인 형태에 따라 구성
된다. 파형은 그럼 4.15에 보였다.

맵핑 후에, 주파수 축의 병렬 데이터는 + 회로에 입력된다. 이 경우, 64지점 IFFT
회로에 기반 한 OFDM 기법을 사용하여 52 하위반송파 ASS 얻었다. 할당 방법은 그
림 4.13에 보였다.

218



===== PAGE 224 =====
직교주파수분할다중 (OFDM) 전송기법   1 0 |

0.8

Transmission data |-channel
H

7     >

0.6

0.4

0.2

Amplitude

-0.2

-0.4

-06

°      >

-0.8

20 30

40

50   60   70

Frequency (subcarrier number)

(a)

Transmission data Q-channel

08

0.6

0.4

0.2

Amplitude

-0.2

-0.4

-0.6

| 101

i

>6 O90

i

0.8

를 그림 4.15

10

20 30

40

50   60   70

Frequency (subcarrier number)

(b)

(a) FASS] AS 데이터 (0) @채널의 AS 데이터

[1013 , qch1]=crmapping (ich, qch, fftlen,nd) ;

할당 Fol], ich1 2} qch1 2 IFFT 회로에 입력되고 그들의 파형은 OFDM 파형으로 구

성된다.

x=ichl+qchl . ^1.

219


===== PAGE 225 =====
최신 이동통신시스템

220

Mobile Communications using MATLAB Simulation
y=ifft (x);      ta, CEES built-in: function
ich2=real (y) ;   $ real : built in function
qch2=imag (y) ;   % imag : built in function

이들 두 직렬 데이터 ABS 다중경로 페이딩에 의해 야기되는 ISIS 제거하기 위해
각 채널에 삽입된 보호간격을 가지고 있다.

fftlen2=fftlentgilen;
[ich4,qch4]= giins(ich2,qch2, fftlen, gilen, nd) ;

47) A, 4-2] fitlen2S 보호간격을 포함한 심볼의 길이로 정의했다. 필터링된 신

는 대기로 전송된다. 10과 008의 OFDM 변조 데이터는 그림 4.16에 보였다.

신호는 무선채널 (저역통과 시스템과 동등한)을 지나 수신기에 전송된다. 전
SE 먼저 다중경로 페이덩에 의해 오염된다. 시뮬레이션에서 함수에서 “%” 명
사용하였다. 그러나 “%”를 생략하면 레일리 Bo] 환경에서의 88#과 PER
시뮬레이션 할 수 있다.

수신기에서, 수신신호는 4\68*에 의해 오염된다. 잡음함수에 대해서는 이미 3.2.3
장에서 논의하였는데 거기에서 comb.m BFS 사용하였다. 이 시뮬레이션에서, 우리
는 E,/N + BER 사이의 관계를 보여주는 그래프를 얻고 싶었다. 이는 주어진

E,/N ol 따라 “800”을 변화시켜주어야 함을 의미한다. 변수 “302”은 BPSK] A}
용된 것과 유사한 과정을 거쳐 계산되었다. 여기서 “6900\”는 심볼 당 반송파당 신호파
워를 의미한다. OFDMA}, “spow"= 병렬 하위반송파의 수를 나타내는 “0818”로 나
누어줘야 한다.

fo

of of}
이 호 0
(=

thlo 00

&

'

ox,



===== PAGE 226 =====
교주파수분할다중 (OFDM) 전송기법

aa}

Transmission signal |-channel

03
0.2       |
0.1   |       | Poe ie | ey 50 180          +                    “4
Ss 0                                                eS
=
e                       Hl
두 -01                                     DE     '
-0.2    |     【   | |
-0.3
-0.4
0 50 100 150 200 250 300 350 400 450 500
Time (sampling number)
(a)
03                    Transmission signal Q-channel
0.2                 |      |
Ss 0                                :
르
&                                 i
-0.2 ~                  t
-03
-0.4

0 50 100 150 200 250 300 350 400 450 500

Time (sampling number)

(b)

를 그림 4.16 (a) |채널의 전송신호 (6) @채널의 전송신호
spow=sum(ich4.*2+qch4.*2)/nd./para; % |sum : built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn) ;

attn3} comb.m-& 사용하여 전송 데이터는 4\60씨에 의해 오염된다.

[ich5,qch5]=comb (104 , 40114 , attn) ;

221



===== PAGE 227 =====
최신 이동통신시스템

A

222

Mobile Communications using MATLAB Simulation
그 후에, 수신신호1015과 qchS 23] 보호간격을 제거한다.
[ich6,qch6]J= girem(ich5,qch5, fftlen2,gilen,nd) ;

시간 축의 직렬 데이터 “ich6”F} “qch6”%= FFT 회로로 입력된다. 이 회로에서, 직렬
데이터는 주파수 축의 병렬 데이터로 변환된다.

rx=ich6+qch6.*i;

ry=fft (rx) ;   S$} fit. fe burit “in function

ich7=real (ry) ;

qch7=imag (ry) ;

그 결과 우리는 64 채널 SSS 얻게 되는데 이는 회로가 64-지점 FFTS 행하기

때문이다. 그러나 정보는 52 ado] 존재한다. 그러므로 64 채널 출력에서 52 ASS
가져왔다.

[ich8,qch8]=crdemapping (ich7,qch7,fftlen,nd) ;

다음으로 변환된 데이터는 각 채널에서 비정규화를 위해 “kmod” & 나누어지고 BA
함수에 입력된다.
ich9=ich8./kmod;
qch9=qch8 . /kmod;
[demodata]=qpskdemod (ich9,qch9,para,nd,ml) ;
후에, 복조된 데이터는 16\7818*00*2 벡터로 변환된다. 이를 “demodatal”o]
부른다.

demodatal=reshape (demodata,1,para*nd*m1) ;

다음으로 비트 오류의 수를 계산하였다. 그 과정은 2.3장에 기술하였다. 동시에, 패킷
오류의 수도 계산하였다. 이 시뮬레이션에서, 전송 데이터는 “9600818”이고 수신 데이
터는 “demodatal”o] tT}. 계산은 다음과 같이 수행되었다.



===== PAGE 228 =====
직교주파수분할다중(ㅁ04) 전송기법 0깔

noe2=sum(abs (demodatal-seridata)); % sum : built in function
nod2=length(seridata); % length : built in function
% calculating PER
if noe2~=0
eop=eopt+1;
else
eop=eop;
end
e0p;
nop=nop+1;
% calculating BER
noe=noe+noe2;

nod=nod+nod2;
다음 식으로 BERZ} PERS 얻는다.

per=eop/nop;

ber=noe/nod;

ofdmda.m2] 긴 시뮬레이션 후에 BER} PERS 얻었다. BER 성능은 이론치와 비교
하여 그림 4.17에 보였다.

1.006+ 00

?
&
>
?
주
&
>
e
＊
?

+
>

oo   AWGN theory

—— 1 path Rayleigh theory

-& QPSK AWGN (no compensation)

~@- QPSK 1 path Rayleigh (perfect compensation)
~@ QPSK 1 path Rayleigh (no compensation)

1.00E — 01

도
uy 1.006- 02  5

1.006-03 늘

하
g

20
E,/N,{dB)

를 그림 4.17 BER AS (데이터)

223


===== PAGE 229 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

PER 성능은 그림 4.18에 보였다. BER 시뮬레이션 결과에서 이론치로부터 +0.9691-
ABS] 전이가 있었다. 이는 수신신호의 보호간격 파워에 의해 야기된다. 이는 다음과 같

이 계산된다.
:                       il
shifted value (dB) = -10log1       —
fftlen2        (4.10)
1.00E + 00
QPSK Rayleigh       é
1.00E — 01+                                    (perfect compensation)
& 1.00 - 02

1.00E - 03 —

QPSK AWGN

(no compensation)
1.00E — 04                                                                                                           3B

0                   10                    20                   30                   40                    50

E,/N, (dB)

를 그림 4.18 PER 성능 (데이터)

이전에 우리는 보호간격의 길이를 0168으로, 보호간격을 포함한 1 심볼의 길이를
101602로 정의하였다. 그림 4.17에서 단일경로 평탄 레일리 페이딩 하에서의 BER 성능
을 볼 수 있다. 시뮬레이션을 위해, 프로그램 4.5의 페이덩 채널을 위한 프로그램에서
“%” 명령어를 제거하였다. 변수 “flat”-S 1과 0으로 변화시킴으로써 페이덩 ao] 보
상될 수 있는지 여부를 결정할 수 있다. 단일경로 레일리 페이딩 하에서의 BER 성능으
로부터, 페이덩에 의해 야기되는 진폭과 위상의 변동을 완벽하게 보상해줄 수 있다면
이론치로부터 0.9691-08의 전이를 얻을 수 있음을 알 수 있다. 그러나 이 변동을 보상해
줄 수 없다면 데이터를 복원할 수 없다. 전송 특성을 추정하는 한 가지 방법은 Masa

224



===== PAGE 230 =====
직교주파수분할다중 (OFDM) 전송기법   10 |

ES 삽입하는 것인데 이 방법에서는 그림 4.12에서와 같이 알고 있는 Bada 심볼이
알려진 주기에 삽입된다.

수신기에서, 모든 심볼에 대해 채널 특성을 추정할 수 있다. 추정된 전송 특성을 사용
하여 전송된 데이터를 복원할 수 있다. 다음에는 프로그램 4.8에 Bes 데이터 입력 회

BS 추가하는 WH 대해 보일 것이다.

프로그램 4.8에서, 파일 데이터 삽입 프로그램을 추가하여야한다: 프로그램 4.8의
“% CE data generation” 4-2-2 참고하기 바란다. 이 부분에서 Bp Bl 데이터가 구성된
다. 여기에서 Bel 데이터는 랜덤 데이터이고 “ich” ol] RE 삽입된다.

% CE data generation
kndata=zeros (1, fftlen) ;
kndata0=2.* (rand(1,52)>0.5)-1
kndata (2:27) =kndata0 (1:26) ;
kndata (39:64) =kndata0 (27:52) ;
ceich=kndata; % CE:BPSK
ceqch=zeros (1, 64);

데이터는 정보 OFDM 데이터 앞에 시간 도메인에서 입력된다. 프로그램의 “%
— data mapping (DC=0)          “를 참고하기 바란다.

[ichl, qch1]=crmapping (1001, 4004, fftlen,nd) ;
ich2=[ceich.' ichl]; % I-channel transmission data
%

qch2=[ceqch.' qchl];   Qchannel transmission data

구성된 전송 데이터 ich29} qch2S 이용해서 FFTS 수행할 수 있다.

Sa 4084
x=ich2+qch2.*i;
y=ifft (x);
ich3=real (y);
qch3=imag (y) ;

그 다음 주기적인 보호신호가 입력되고 대기로 전송된다. 그 후에, 프로그램 4.5에서

225



===== PAGE 231 =====
a

최신 이동통신시스템

226

Mobile Communications using MATLAB Simutation

언급된 바와 같이 AMA SE 다중경로 페이딩과 AWGNS] 의해 오염된다. 수신기에
서, 입력된 보호간격이 제거된다. 다음으로, 제거된 ASE FFT 회로에 입력된다.

rx=ich6+qch6. *i;
ry=fft (rx);
ich7=real (ry) ;
qch7=imag (ry) ;

8 심볼을 이용해 AS 특성을 추정할 수 있다. “%
CE symbol       “를 참고하기 바란다. 먼저, 수신 후 취해진 데이터 ich72}
0007로부터 HIB 심볼을 추출한다. 이 시뮬레이션에서, whale ABS 그림 4.14에
서와 같이 첫 번째 심볼 시간에 위치한다.

Fading compensation by

% taking CE data out of received data
ce=1;
icel=ich7(:,ce);

qcel=qch7 (:,ce);

동시에, 수신기에서 사용된 Sel 데이터를 준비한다.
% preparation known CE data
ce=1;

ice0=ich2 (:,ce);

qce0=qch2 (:,ce) ;

ie.) | 0 의 ae ea  주어진다.

qcel     0060
1061 ay 1060
0061 로  0060             (4.11)

이때, AT 페이딩 환경의 전이 행렬이고 페이딩이 위상회전과 진폭변동의 함수이기
때문에 다음과 같다.



===== PAGE 232 =====
직교주파수분할다중(0) 전송기보 (를

iv 0
A=
#     iv  |                                (4.12)

페이딩 JAS 보상하기 위해서 모든 수신 데이터를 4 로 곱해줘야 한다. AM!
는 다음과 같다.

eee    1    | iv   4
yiv+qv’ \-w 제                 (4.13)
(4.11)에서 (4.13)까지에서, 2/와 quo] 값은 다음과 같다.

(iceO x icel + qce0 x qcel)

7 주 a
icel + 0061                                    (4.14)

qce0 x icel - ice x qcel)

1
0-- ㅜㅜ (
ajicel + 0061                                    (4.15)

이 시뮬레이션에서, 우리는 매개변수 7/와 que 계산한다.

% calculating reverse rotation

ivereal.( (1/4 iced: 22 +9qc61 542): 6 eee tit qce0)..*(a.cel-
i.*%qeel))3

qv=imag((1./ (igel.“2+qGel. “2)))* taee0 1 oA qce0).* (icel:

t.“qcel)) >;
iv} qué 이용해, 두개의 역 회전행렬은 다음과 같이 만들어진다.

% matrix for reverse rotation
ieqvl=[iv iv iv iv iv iv iv];

geqvl=[qv qv qv qv qv qv qv];
하나의 데이터-프레임 단위가 존재하므로, 하나의 채널 추정 심볼과 6개의 데이터 심

227



===== PAGE 233 =====
A 최신 이동통신시스템
Mobile Communications using MATLAB Simulation

볼이 존재하고 벡터의 길이는 두 매개변수에서 7이다. 벡터를 사용해, 수신신호 107과
0007의 역 회전을 수행한다. 역 회전 데이터는 1002000과 qcompen?| 3? 1017, 00807,
icompen, 40001060,1601, geql 2] 관계는 다음과 같다.

icompen = ich7 x ieqvl - qch7 x geqv1                      (4.16)
qcompen = qch7 x ieqvl + ich7 x qeqv1                  (4.17)

이 시뮬레이션에서 위 RSS 계산했다.

% reverse rotation

icompen=real ((ich7+i.*qch7) .* (ieqvl+i.*qeqvl) );
qcompen=imag ( (ich7+i.*qch7) .* (ieqvlti.*qeqv1l) );
ich7=icompen;

qch7=qcompen;

위상 BAD 데이터로부터 Ble 심볼을 다음과 같이 제거한다.

%

CE symbol removal
ich8=ich7 (:,knd+1:nd+1) ;
qch8=qch7 (:,knd+1:nd+1);

그 후에 사용된 과정은 프로그램 4.5에 기술된 것과 동일하다.

컴퓨터 시뮬레이션에서 위의 위상 보정을 사용하여 BERS} PERS 얻었다. BER 성
능은 이론치와 함께 그림 4.19에 보였다. 단일경로 레일리 페이딩하의 BER 성능으로
부터 페이딩에 의한 진폭과 위상 변동을 보상할 수 있다면 이론치로부터 0.9691-08의
전이를 얻을 수 있다. 그러나 변동을 보상해주지 못하면 데이터를 복원할 수 없다. 반면
에 Eo] 8 기반 OFDM 전송기법에서는 이론치로부터 200의 전이를 얻을 수 있다. 그
림 4.19는 단일경로 페이딩 환경에서 전송특성에 의해 야기되는 ASH 위상변동을 완
벽하게 보상했을 경우의 시뮬레이션된 BER 성능을 보여준다. 이 시뮬레이션을 위해서
는 프로그램 4.8에서 %—Fading compensation by CE symbol- 부분의 “%”를 제거하
면 된다. 완전한 보상의 경우, BER 값은 파일 기반 OFDM 시스템의 것과 동일하다.

228



===== PAGE 234 =====
직교주파수분할다중(00) 전송기보 OE

하면 208의 전이를 의미한다. 이는 우리가 한 프레임 단위의 1/7 파
했기 때문이다. 결과적으로, 입력된 gal 데이터 심볼의 수가 증
은 저하되고 보호간격을 삼입하면 BERS 더 나빠진다.

ay
i El

1.00E + 00

4                                                                                                           7
uy path Rayleigh (no compensation)

~# OPSK 2 path Rayleigh (CE compensation)
-t- OPSK 2 path Rayleigh ISI (CE compensation)

~@-OPSK 1 path Rayleigh

i 1.00 - 02                                                   (CE compensation)
~@ QPSK 1 path Rayleigh
(perfect compensation)
: | QPSK AWGN

1.00 - 03 L        \  {00 compensation)

AWGN  들         1 path Rayleigh theory

theory i
1,      sal                                              L                    11                    일

ae 0                   10                 20                 30                  40                  50

E,/N, (dB)

를 그림 4.19 BER 성능 (00+데이터)

이중경로 패널에서, 파일 기반 OFDM 시스템의 BER 성능은 부분적으로 ©
로 레일리 페이덩에서 지연파의 위치에 의존한다. WS 지연파의 지연시간이 보호
es 짧다면 진폭과 위상의 모든 변동은 Fda ASS 사용해 제거될 수 있고 BER 성

Se 단일경로 레일리 페이딩과 동일하다. 그러나 지연시간이 보호간격보다 크다면
 다음 심볼을 오염시키고 BER 성능은 저하된다. PER 성능은 그림 4.20에 보였다.
그럼 4.20에서 볼 수 있는 바와 같이, PERS 저하된다.

우리는 반송파 대 간섭비 (C1) 2} BER 그리고 0/1와 PERS 컴퓨터 시뮬레이션을 통
해 계산하였다. 이 시뮬레이션에서, 간섭 잡음으로 다른 파일 기반 OFDM 신호를 A}
용하였다. 간섭은 프로그램 4.9를 사용해 첨가되었다. 프로그램 4.10을 사용하여, 파일
3] 7) 8} OFDM 신호를 얻을 수 있는데 신호의 파워는 /1의 값에 의존하고 신호의 데이
터 소스와 오염된 페이덩은 원하는 신호와 그렇지 않은 신호에서 서로 다르다.

229



===== PAGE 235 =====
최신 이동통신시스템

                   Mobile Communications using MATLAB Simutation
1.00E + 00                                                                                                                                [
Ar OPSK 2 path Rayleigh IS!
(CE compensation)
—@- OPSK Rayleigh (CE compensation)
1.00E - 01                          -&- QPSK 2 path Rayleigh
(CE compensation)
& 1.00E - 02
QPSK Rayleigh
(perfect compensation)
1.00E — 03 &
QPSK AWGN (no compensation)
1.00E prs 04              L            11            iL           Din        1            1            11            개           L
0                       10                      20                      30                      40                      50

E,/N, (dB)
를 22 4.20 PER 성능 (00+데이터)

프로그램 4.9는 0/[ 대 BER 그리고 2 대 PERS 계산하기 위한 주된 프로그램이다.
프로그램 4.9에서 우리는 먼저 간섭신호를 위해 몇 가지 변수를 정의한다.

8 interference wave initialization
ci=10;           4 *C/T: ratio

ml2=2;           % modulation level
itau2=[0];

dlv12=[0];

n02=[6];

th2=[0.0];
itnd2=[10000+floor (rand (1) *10) *1000);
now2=1;

fd2=fd;

flat2=0;

itnd02=nd* (fftlentgilen)*300; % Number of fading counter to skip

다음으로, 간섭신호를 위한 페이딩의 매개변수를 1101482081 행렬에 저장한다.

%$% store all parameters in one matrix "fadingpara"

fadingpara=zeros (8, length (itau2) );

230



===== PAGE 236 =====
직교주파수분할다중 (OFDM) 전송기법 fo J

fadingpara(1l,
fadingpara (2,
fadingpara (3,
fadingpara (4,

fadingpara (6,
fadingpara(7,

)
)
)
)
fadingpara(5,:)=itnd2;
)
)
)

fadingpara (8,
fadingpara 행렬을 사용하여, 간섭신호가 생성되고 원하는 신호에 첨가된다.

%$%% interference wave addition

% interference

[iintw, qintw]=interwave (ci, spow,ml2, length (ich4) ,tstp, fadingpa
ra);

itnd2 = itnd2+itnd02;

fadingpara(5,:)=itnd2;

ich4=ich4+iintw;

qch4=qch4+qintw;

Cie} 값을 바꿈으로써 그림 4.215} 4.22] 보인 BERZ} PERS 얻을 수 있다.

1                    T                  T                  개                  | |
-ㅎ- BER, fd = 50 Hz
—- BER, fd = 500 Hz
OTF                                                                                            4
fod
& 00나                         4
0.001                                                                                            4
0.0001                    L                  1                  1                  1
-10                0                 10                20                30                40

CIR (dB)
를 그림 4.21 BER 성능 (ㄷ+데이터)

231



===== PAGE 237 =====
Zy 최신 이동통신시스템
c

Mobile Communications using MATLAB Simufation

—6-— PER, fd = 50 Hz
—8- PER, fd = 500 Hz

O.1F

PER

O.01F

0.001                      1                    i                    1                    1
-10                0                  10                 20                30                 40
CIR (dB)

를 그림 4.22 PER 성능 (6ㄷ+데이터)

000 RS

이 장에서는 병렬 데이터 ASS] 개념과 OFDM 송수신기의 구성에 관한 내용을 기
술하고, OFDM 송수신기를 컴퓨터 시뮬레이션을 통해 구성하는 방법을 설명하였다.
OFDME] 방대한 시뮬레이션 결과에 대해 논하였으며 파일 기반 08184 전송 시스
템을 사용하여 차세대 광대역 WLAN 시스템을 시뮬레이션 하였으며, wpa 기반
OFDM 전송 시스템의 BERY S29] 개선효과를 보이기도 하였다. 이 BS 통해서
OFDMS] 기본원리를 터득한 독자가 만약 OFDM7] 8S] 시제품을 개발한다면 추가적
으로 최적 지점에서 보호간격을 제거하기 위해 OFDM 신호를 위한 동기회로까지도 시
뮬레이션 해야 할 것이다. 또한 다른 변조방식의 시스템과 전송성능을 비교할 때 진폭
과 위상잡음의 비선형성에 대해서도 고려해줘야만 한다.

232



===== PAGE 238 =====
직교주파수분할다중 (OFDM) 전송기법 Bo I

1) Chang, R. W., and R. A. Gibby, "A Theoretical Study of the Performance of an Orthogonal
Multiplexing Data Transmission Scheme," IEEE Trans. Commun., Vol COM-16, No. 4, August
1968, pp.527-540.

2) van Nee, R., R. Prasad, OFDM for Wireless Multimedia Communications, Norwood, MA:
Artech House, 1999.

3) Prasad, R., Universal Wireless Personal Communications, Chapter 10, Norwood, MA: Artech,
1998.

4) http://www.etsi.org/bran/.

5) IEEE802.11, [EEE Standard for Wireless LAN Medium Access Control and Physical Layer
Specifications, November 1997.

6) http://www.arib.or.jp/mmac/e/index.htm.

233



===== PAGE 239 =====
최신 이동통신시스템

234

Mobile Communications using MATLAB Simulation

부록 4ㅅ

프로그램 4.1 0100.07

% Program 4-1

% ofdm.m

%

% Simulation program to realize OFDM transmission system
%

% programmed by T.Yamamura and H.Harada

%

KKK KKKKKKKKKKK KKK KKK         ;        KKK KKK KK KKK KK KKK KKK KKK KKK
%                      preparation part

para=128;   % Number of parallel channel to transmit (points)
fftlen=128; % FFT length

noc=128;    % Number of carrier

nd=6;       % Number of information OFDM symbol for one loop
ml=2;       % Modulation level : QPSK

sr=250000; % Symbol rate

br=sr.*ml; % Bit rate per carrier

gilen=32;   % Length of guard interval (points)

ebn0=3;     % Eb/NO

ZRKEKKKKKKKK KKK KK KK KKK KK KK main loop part KKEKKKKKKKKKKKKKKKKKKK KKK

nloop=100; % Number of simulation loops

noe = 0;    % Number of error data

nod = 0;    % Number of transmitted data
eop=0;      % Number of error packet
nop=0;      % Number of transmitted packet

for iii=1:nloop
ZRKKKK KKK KK KK KKK KK KKK KK KKK transmitter KEKE KKK KKK KEK KKK KKKK KK KKK KK

ZRKKKKK KK KKK KK KR KKK KKK RK KK Data generation KKRKEK KEKE KK KKEKKKKKKKK KKK

seldata=rand(1,para*nd*ml)>0.5; % rand : built in function

GK KK KKK KK KK KK Serial to parallel CONVELSLON KKKKKRKKKKKKKKKKK



===== PAGE 240 =====
paradata=reshape (seldata,para,nd*ml); % reshape : built in function

LRKKKK KKK KKK KKK KK KKK KK KKK QPSK modulation KKK KKKKKKKKKKKEKKKKKKKKK

[ich, qch]=qpskmod (paradata, para,nd,ml) ;
kmod=1/sqrt(2); % sqrt : built in function
ichl=ich.*kmod;

qchl=qch.*kmod;

ZRKKKKKK KKK KK KKK KK KK  IFFT  KKKKKKKKKKKKKKKKKKKKKEKK

x=ichl+qchl .*i;

y=ifft (x);      % ifft : built in function
ich2=real (y) ;   % real : built in function
qch2=imag(y) ;   % imag : built in function

웅***×**×*ㅎ*** Gurad interval insertion ********x**

[ich3,qch3]= giins(ich2,qch2,fftlen,gilen,nd) ;
fftlen2=fftlent+gilen;

웅**ㅅㅎ*×ㅎ*ㅎ*ㅎ*** Attenuation Calculation *********
spow=sum(ich3.*2+qch3.*2)/nd./para; % sum : built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn);

ZRKKK KKK KKK KKK KK KK KKK KK KK   Receiver   KKK KKK KKKKKKKKKKKKKKKKKKKK

kK KKK KKKKKKEKKEKK BWGN addition *******k**

[ich4, qch4]=comb (ich3, qch3, attn) ;
ZRKEKKKKKKKKKKKKKKKK Guard interval removal KKKKKKKKK
[ich5,qch5]= girem(ich4,qch4, fftlen2,gilen,nd) ;

ZRKEKKKKKKKKKKKKK KKK   FFT   KREKEKKKKKKKKKKKKKKK

rx=ich5+qch5.*i;
ry=fft (rx);

00

fli = built-in (00100 00
real : built in function
qch6=imag (ry) ;      % imag : built in function

00

ich6=real (ry);

LHKKKK KKK KKK KK KK KK  demoduration  KKKKKKKKKKKKKKK KKK K

235



===== PAGE 241 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

ich7=ich6./kmod;
qch7=qché6./kmod;
[demodata] =qpskdemod (ich7,qch7, para,nd,m1) ;

ZRREKKKKKKKKKK KK  Parallel to serial conversion  KKKEKKKKKKKKKKKKKK
demodatal=reshape (demodata,1,para*nd*m1) ;
ZRKEKKKKKKKK KKK KKK KKK KK Bit Error Rate (BER) KKKKKKKKK KKK KKK KKK KKK

으

% instantaneous number of error and data

noe2=sum (abs (demodatal-seldata)); % sum: built in function
nod2=length(seldata); % length : built in function

%* cumulative the number of error and data in noe and nod

noe=noet+noe2;
nod=nod+nod2;

% calculating PER

if noe2~=0
eop=eoptl1;
else
eop=eop;
end
eop;
nop=nop+1;

fprintf ('td\t%e\t%d\n',iii,noe2/nod2,eop) ;   %  fprintfl = buidt “in
function

end

Zw KKK RK KK RR RR KKK KK Output result KKaKKKKK KKK KKK KKK KKK KKK KKK KKK

per=eop/nop;
ber=noe/nod;

fprintf ('Sf\te\t%e\tsd\t\n',ebn0,ber, per,nloop) ;
fid = fopen("BERofdm.dat','a');
fprintf (fid, 'Sf\tse\t%e\tsd\t\n',ebn0,ber,per,nloop) ;

236



===== PAGE 242 =====
fclose (fid) ;

ZREKKKKKKKKKKKKKKKKKK end of file KKEKKKKKKEKRKKKKKKKKKKKKKKKKKK

프로그램 4.2  ofdm_fading.m

00

Program 4-2
ofdm_ fading.m

Simulation program to realize OFDM transmission system
(under one path fading)

AP 00 00 00 00

oe

programmed by T.Yamamura and H.Harada

oo

ZRKKK KKK KKK KKK KK KK KK KK EK preparation part KKEKKKKKKKKKKKKKKK 그

para=128;   % Number of parallel channel to transmit (points)
fftlen=128; % FFT length

noc=128;    % Number of carrier

nd=6;       % Number of information OFDM symbol for one loop
ml=2;       % Modulation level : QPSK

sr=250000; % Symbol rate

br=sr.*ml; % Bit rate per carrier

gilen=32;   % Length of guard interval (points)

ebn0=10;    % Eb/NO

GRKKKKKKK KKK KK KKK KKK Fading initialization KKEKKKKKKKKK KKK KK KEKE

% If you use fading function "sefade", you can initialize all of
parameters.

% Otherwise you can comment out the following initialization.

% The detailed explanation of all of valiables are mentioned in
Program 2-8.

% Time resolution

tstp=1/sr/ (fftlent+gilen) ;

% Arrival time for each multipath normalized by tstp

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

itau = [0];

237


===== PAGE 243 =====
최신 이동통신시스템

238

Mobile Communications using MATLAB Simulation

% Mean power for each multipath normalized by direct wave.

% If you would like to simulate under one path fading model, you have
only to set

% direct wave.

01571 = [0];

% Number of waves to generate fading for each multipath.

% In normal case, more than six waves are needed to generate Rayleigh
fading

n0=[6];

% Initial Phase of delayed wave
% In this simulation fourpath Rayleigh fading are considered.
th1i=[0.0];

% Number of fading counter to skip
itnd0=nd* (fftlen+gilen) *10;

% Initial value of fading counter
% In this simulation onepath Rayleigh fading are considered.
% Therefore one fading counter are needed.

itnd1=[(1000];

% Number of directwave + Number of delayed wave
% In this simulation onepath Rayleigh fading are considered
nowl=1;

% Maximum Doppler frequency [Hz]
% You can insert your favorite value
f£d=320;

% You can decide two mode to simulate fading by changing the variable
flat

% flat     : flat fading or not

%  (1->flat  (only amplitude is  fluctuated),0->nomal(phase and
amplitude are fluctutated)

flat =1;

ZRKK KKK KKK KK KIRK KKK KK KKK KK main loop part KKK KKKKKKKKKKKKKK KKK KK KK

nloop=500; % Number of simulation loops



===== PAGE 244 =====
noe = 0;    % Number of error data

nod = 0;    % Number of transmitted data
eop=0;      % Number of error packet
nop=0;      % Number of transmitted packet

for iii=1:nloop

Bk KR KK RK RR RR KR KK RK KK KK KKK  transmitter  KKK KKKKKEKKKKKKKKKKKKKKKKK

Dew KKK RK KR RK RK RK RK RK KK KK Data generation KKEKKKKKKKKEKKKKKKKKKKKKK

seldata=rand(1,para*nd*ml)>0.5; % rand : built in function
ZRKEKKKKKKKKK KKK KK Serial to parallel conversion KKEKKKKKKKKKKKKKKK

paradata=reshape(seldata,para,nd*ml); % reshape : built in function

LRKRKK KKK RK KK KKK KK KK RK KR KK OPSK modulation KKKKKKKKKKKKKKKKKKK KKK

[ich, qch]=qpskmod (paradata,para,nd,ml) ;
kmod=1/sqrt(2); % sqrt : built in function
ichl=ich.*kmod;

qchl=qch.*kmod;

LHKKKKK KKK KK KK KKK KKK  IFFT  KKKKKKKKKKKKKEKKKKKK KK KKK

x=ichlt+qchl.*i;

y=ifft (x);      % sbftt +. built. 10 funceion
ich2=real (y);      real : built in function
qch2=imag(y) ;      imag : built in function

00 00

옹××**~**×*** Gurad interval insertion **********

{ich3,qch3]= giins(ich2,qch2,fftlen, gilen,nd) ;
fftlen2=fftlent+gilen;

Zeca eeete-Attenuation: Calculation: 기우
spow=sum(ich3.*2+qch3.*2)/nd./para; % sum : built in function

attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn) ;

Dkk KK RR KR RK RK KK KK Fading channel KKK KK KKKKKKKKKKKKKKKK

239



===== PAGE 245 =====
최신 이동통신시스템

240

Mobile Communications using MATLAB Simulation

% Generated data are fed into a fading simulator
[ifade, qfade] =sefade (ich3, qch3, itau, dlvl,th1,n0,itnd1,nowl, length (
ich3) ;tstp, fd, flat) ;

% Updata fading counter
itndl = itndl+ itnd0;

GRR KK RR KR RRR RK KR KK KR KK KR KK   Receiver   KKK KE KKK KKK KKKKKKKKKKKKKKK KKK

Sk KR KK RK KR RR KR RK AWGN addition Ke KKK KKK
[ich4,qch4]=comb (ifade, qfade, attn) ;

ZRREKKK KKK KK KK KK KK KK Guard interval removal ******xx**

{ichS5,qch5]= girem(ich4,qch4, fftlen2,gilen,nd) ;

BRK KKK KK RK KK KR RK KR RK   FFT   KKKKKKKKKKKK KKK KKK

rx=ich5+qch5 26

ry=fft (rx) ;         % fft <= “built in function
ich6=real (ry) ;      % real : built in function
qch6=imag (ry) ;      % imag : built in function

Ze K KKK KK KR RK KK KKK  demoduration *** KKK KKKKKKKKKKKKK

ich7=ich6./kmod;
qch7=qch6./kmod;
[demodata]=qpskdemod (ich7,qch7,para,nd,ml1l) ;

ZRKK KKK KK KKK KKK  Parallel to serial conversion  KKK KKK KKK KK KKK KK

demodatal=reshape (demodata,1,para*nd*m1l) ;

ZRKKKKK KKK KKK KK KK KKK KK Bit Error Rate (BER) KKEKKKKKKKKKKK KKK KK KKK

% instantaneous number of error and data
noe2=sum (abs (demodatal-seldata)); % sum: built in function
nod2=length(seldata); % length : built in function

% cumulative the number of error and data in noe and nod
noe=noe+noe2;

nod=nod+nod2;

% calculating PER

if noe2~=0



===== PAGE 246 =====
eop=eopt1;
else

eop=eop;
end

eop;

nop=nop+1;

fprintf ('Sd\t%e\t%d\n',iii,noe2/nod2, eop) ;   %O fpPiNGE S= butt: in
function

end

SRKKKKKKKEKK KKK KKK KK KEK KK Output result KKK KKK KKKKKKKKKKKK KKK KKK KKK

per=eop/nop;
ber=noe/nod;

fprintf ('sf\t%e\tse\tsd\t\n',ebn0, ber, per, nloop) ;

fid = fopen('BERofdmfad.dat','a');

fprintf (fid, 'sf\t%e\t%e\t%d\t\n',ebn0,ber, per, nloop) ;
fclose (fid) ;

LEEK KKKKKK KKK KK KKK KKK end of fite KKK KKK KK KKK KKKKKKKKKK KKK KKK

프로그램 43 _ giins.m
% Function 4-3
giins.m

%
%
% Function to insert guard interval into transmission signal
%
% Programmed by T.Yamamura and H.Harada

%

function [iout,qout]= giins(idata, qdata, fftlen, gilen,nd) ;

Ze KKK KK RK KR KK KK KR KK variables KKK KKK KKK KKK KKK KKKKKKKKKK
% idata    + .-Input:-Ich. data

% qdata    : Input Qch data

% iout     : Output Ich data

% qout     : Output Qch data

% fftlen   : Length of FFT (points)

% gilen    : Length of guard interval (points)

241



===== PAGE 247 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

옹  KKKEKKKKKKKKKKKKKKKKKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KEK

idatal=reshape (idata, fftlen,nd) ;
qdatal=reshape (qdata, fftlen,nd) ;
idata2=[idatal (fftlengilent+1l:fftlen,:); idatal];
qdata2=[qdatal (fftlengilen+l:fftlen,:); qdatal);

iout=reshape (idata2,1, (fftlent+tgilen) *nd) ;
qout=reshape (qdata2,1, (fftlen+gilen) *nd) ;

ZRRKK KKK KK KK KK RK KK RK end of file KEK KKK KKKEKKKKKKKKKKKKKK KK

프로그램 4.4  girem.m
% Function 4-4

% girem.m

%

% Function to remove guard interval from received signal

%

% Programmed by T.Yamamura and H.Harada

%

function [iout,gout]= girem(idata, qdata, fftlen2,gilen,nd);

Hw KK KK RK  variables  KKK KKK KEKKKKK KK KK KKK KK KEKE

% idata       : Input Ich data

% qdata       : Input Qch data

% iout        : Output Ich data

% qout        : Output Qch data

% fftlen2     : Length of FFT (points)

% gilen       : Length of guard interval (points)     1
% nd          : Number of OFDM symbols

옹  KKK KK KKK KK KK KKK KKK KKK KKK KKK KKKKKK KKK KKK KK KKK KKK KK KKK

idata2=reshape (idata, fftlen2,nd) ;
qdata2=reshape (qdata, fftlen2,nd) ;

iout=idata2 (gilenti:fftlen2,:);
gqout=qdata2 (gilen+1:fftlen2,:);

ZREKKKKK KKK KKK KK KK KKK end of file KKKKKKKKKKKKK KKK KKK KKK KK KKK

프로그램 4.5 ofdmda.m
% Program 4-5

242



===== PAGE 248 =====
부록 4A
% ofdmda.m

%

% Simulation program to realize OFDM transmission system

%

% Programmed by T.Yamamura and H.Harada

% Prease refer Program 4-2

%

% GI data GI data ....(data 6symbols)

%

웅웅웅웅웅웅웅웅응융응응응 preparation part %%3%3%33SS%S%SSSSSSS%

para=52;     % Number of parallel channel to transmit (points)
fftlen=64;   % FFT length

noc=53;      % Number of carriers

nd=6;        % Number of information OFDM symbol for one loop
ml=2;        % Modulation level : QPSK

sr=250000;   % OFDM symbol rate (250 ksyombol/s)

br=sr.*ml;   % Bit rate per carrier

gilen=16;    % Length of guard interval (points)

ebn0=3;      % Eb/NO

$%%%%S%SS%S%S%SSSS fading initialization %%%%%%%%%%%

tstp=1/sr/(fftlentgilen); % Time resolution

itau=[0];       % Arrival time for each multipath normalized by tstp
dlv11=[0];      % Mean power for each multipath normalized by direct
wave.

n0=[6];         % Number of waves to generate fading n0(1),n0(2)
th1l=[0.0];      % Initial Phase of delayed wave

itnd1l=[1000];   % set fading counter

nowl=1;         % Number of directwave + Number of delayed wave
fd=150;         % Maximum Doppler frequency

flat=0;         % Flat or not (see ofdm_fading.m)

itnd0=nd* (fftlent+tgilen) *20; % Number of fading counter to skip

Bk KR RK RK RK KK RK Kk KK KK main loop part KKKKK KK KKK KKKK KK KKK KKK KKK

nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data
왕

nod   OF      Number of transmitted data

243



===== PAGE 249 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

eop=0;      % Number of error packet
nop=0;      % Number of transmitted packet
녀

고

LRKKKK KK KK KK RK KKK KK KR RK KKK  transmitter  KKK KE KKK KK KKK KKK KKKKKK KKK KKK

for iii=1:nloop

seridata=rand(1,para*nd*ml)>0.5; % rand : built in function
paradata=reshape(seridata,para,nd*ml); %    reshape : built in
function

%

ml modulation

{ich, qch]=qpskmod (paradata, para,nd,ml) ;
kmod=1/sqrt (2); % sqrt : built in function
ich=ich.*kmod;

qch=qch. *kmod;

data mapping (DC=0) ———

[ich1, qch1]=crmapping (ich, qch, fftlen,nd) ;
오스 스스 21

x=ichi+qchl, *i;

y=ifft (x);      % 그이 시 00116 in function

ich2=real (y);   % -réal.<: built in.function
qch2=imag (y) ;   %. imag, + built in function

%     Gurad interval insertion ———
fftlen2=fftlent+gilen;
{ich4,qch4]= giins(ich2,qch2, fftlen, gilen,nd) ;

%     Attenuation Calculation
spow=sum(ich4.*2+qch4.*%2)/nd./para; % sum : built in function
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;

attn=sqrt (attn) ;

ZREKKKKKK KKK KKK KKK KKK fading channel KKK KK KKK KKK KKK KKKKKKKKKEKKKKK

%If you would like to simulate performance under fading, please
remove "*"

%from the following four sentenses

%[ifade, qfade, ramp, rcos, rsin]=sefade(ich4,qch4,itau,dlvl1,th1,n0,i
tnd1,nowl, length(ich4),tstp, fd, flat);

244



===== PAGE 250 =====
S$itndl = itndl+itnd0; % Updata fading counter
Sich4=ifade;
sqch4=qfade;

SK KK KR RK RK KK RK EK   Receiver   KKK KKK KKK KKK KKK KKK KKKKKKKKKKK
%——— AWGN addition
[ich5, qch5]=comb (10114 , 40114 , attn) ;

%$—1 Path Rayleigh Fading perfect compensation —

%$If you would like to simulate performance under perfect
compensation, please remove "*"

Sfrom the following four sentenses

Sifade2=1./ramp.* (rcos\(1,+)..*ichotrsin (1,3) . 96002) 7
$qfade2=1./ramp.* (-rsin(1,:).*ich5+rcos (1, :|). *qch5) ;

sich5=ifade2;

Sqch5=qfade2;

Guard interval removal ———

[

ich6,qch6]= girem(ich5,qch5, fftlen2,gilen,nd) ;

으으

rx=ich6t+qch6.*i;

ry=fft (rx);   % ££ «> buile-in..ftunction
ich7=real (ry) ;

qch7=imag (ry) ;

%$—————  demoduration
[ich8, qch8]=crdemapping (ich7,qch7, fftlen, nd) ;
ich9=ich8./kmod;

qch9=qch8./kmod;
[demodata]=qpskdemod (ich9, qch9, para,nd,ml) ;

2

%       error calculation ——

demodatal=reshape (demodata,1,para*nd*m1l) ;
noe2=sum (abs (demodatal-seridata)); % sum: built in function
nod2=length(seridata); % length : built in function

% calculating PER
if noe2~=0

eop=eopt1;
else

245



===== PAGE 251 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

eop=eop;
end

eop;

nop=nopt1;

% calculating BER
noe=noe+noe2;

nod=nod+nod2;

fprintf ('%d\t%e\t%d\n',iii,noe2/nod2,eop); % fprintf : built in
function

end

per=eop/nop;
ber=noe/nod;

ZRKKKKKKKK KKK KKK KKK KK KK Output result KKK KKK KKK KKK KKKKKKKKKKKK KKK

fprintf ('Sf\t%e\t%e\ttd\t%d\n',ebn0, ber, per, nloop, fd) ;

fid = fopen('BERofdmda.dat','a');

fprintf (fid, 'sf\t%e\tse\tsd\t%d\t\n',ebn0,ber, per, nloop, fd) ;
fclose(fid);

Sw KK KK IK KK KK enéd“of file KKK KKK KKK KKK KK KKKKKKKKKKEKK

프로그램 4.6 crmapping.m
% Function 4-6
crmapping.m

Function to set data on subcarrier
(DC=0)

00 00 00 00 00

Programmed by T.Yamamura and H.Harada

00 00

function [iout, qout]=crmapping (idata, qdata, fftlen, nd) ;

Zk KK KR KK RK KR RK eK  variables  KEKKKKKKKKKKKKKKKKKKKK KKK

% idata     : Input Ich data

% qdata     : Input Qch data

% iout      : Output Ich data

% qout      : Output Qch data

% fftlen    : Length of FFT (points)

246



===== PAGE 252 =====
옹 nd        : Number of OFDM symbols

& KKK KKK KK KK KKK KK KKK KKK KKK KKK KKK KKK KKK KKK KK KKK KKK KKK KKK

iout=zeros (fftlen,nd) ;
qout=zeros (fftlen,nd) ;

Vout (2:27, :)=idata(1226, ; )
qout (2:27,:)=qdata(1:26,:);
iout (39:64, 2) =idata (27:32 )5)5
qout (39:64, :)=qdata(27:52,:);

Dkk KR RK RK KK RK RK end of £316 KEKKKKKKKKKKKKKKKKKKKKKKEKKEK
프로그램 4.7  crdemapping.m

Function 4-7
crdemapping.m

ae

ae

Function to separate data from the subcarrier
(DC=0)

00 00 00 00

00

MATLAB version
programmed by T.Yamamura

00 ol?

function [iout, qout]=crdemapping (idata, qdata, fftlen, nd) ;

00

KKEKKKKKKKKKKKKKKKK variables KKKKKKKKKKKKKK KKK KKK KKK KK

% idata     : Input Ich data

% qdata     : Input Qch data

% iout      : Output Ich data

% qout      : Output Qch data

% fftlen    : Length of FFT (points)

% nd        : Number of OFDM symbols

옹 **ㅠㅠ＊×ㅠ×ㅠ×ㅠ*×ㅠ*×*×ㅠ×ㅠㅠ×ㅠㄴㅠㅠㄴㅠㅠㄴㅠㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㅠㄴㅠㅠㄴ*×ㅠㄴㅠ×ㅠ×ㅠㅠ×ㅠㅠ×ㅠㅠㄴㅠㅠ×ㅠㅠㄴㅠㅠㅠㄴㅠㅠㄴㅠㅠㄴㅠㅠㅠㅠㅠㄴㅠㅠㄴㅠㅠ×ㅠㅠ×ㄴㅠㄴㅠㅠㄴㅠㅠ×ㅠㅠ×ㅠㅠㅠㅠ

iout(1:26,:) =idatat{2:21,.2
qout: (1:26, :) =qdatat(2:2773) 초
iout (27:52, :)=idata (39:64,:);
qout (27:52, :)=qdata(39:64,:);

ZK KKK KK KKK KK RK KK KK KK end of - £i1e¢6 KKK KK KKK KK KKK KKKKKKKKK KKK KK

247



===== PAGE 253 =====
최신 이동통신시스템

248

Mobile Communications using MATLAB Simulation

프로그램 4.8  ofdmce.m

% Program 4-8

% ofdmce.m

%

% Simulation program to realize OFDM transmission system
%

% Programmed by T.Yamamura and H.Harada

%

% GI CE GI data GI data...(data 6symbols)

% (CE: Chanel estimation symbol, GI Guard interval)

%

ERK KKK KK KK KK KK KK KK KK preparation part KKK KEKKKKKKKKKKKKKKKKKKEK

para=52;    % Number of parallel channel to transmit (points)
fftlen=64; % FFT length

noc=53;     % Number of carriers

nd=6;       % Number of information OFDM symbol for one loop
knd=1;      % Number of known channel estimation (CE) OFDM symbol
ml=2;       % Modulation level : QPSK

sr=250000; % OFDM symbol rate (250 ksyombol/s)

br=sr.*ml; % Bit rate per carrier

gilen=16;   % Length of guard interval (points)

ebn0=3;     % Eb/NO

$SS%%SB%SSSSS%% Fading initialization %%%%%%%%%%%

tstp=1/sr/(fftlen+gilen); % Time resolution

itau=[0];       % Arrival time for each multipath normalized by tstp
dlv1l1=[0];      % Mean power for each multipath normalized by direct
wave.

n0=[6];           Number of waves to generate fading n0(1),n0(2)
thl=[0.0];        Initial Phase of delayed wave

nowl=1;           Number of directwave + Number of delayed wave
fd=150;           Maximum Doppler frequency

flat=0;         % Flat or not (see ofdm_fading.m)

itnd0=nd* (fftlen+gilen) *20; % Number of fading counter to skip

%
%
itnd1=[1000];   % set fading counter
%
%

ZRRKKKKKKK KKK KKKKKKKEKKEKKK Main loop part KKKKKKKKEKKKKKKEKKKKKKKKEK

nloop=1000; % Number of simulation loops



===== PAGE 254 =====
noe = 0;    % Number of error data

nod = 0;    % Number of transmitted data
eop=0;      % Number of error packet
nop=0;      % Number of transmitted packet

ZRKKK KKK KKK KK KKK KK KKK KKK  transmitter  KREKKKKKKKKKKKKKKKKKKKKKKKKK

for iii=1:nloop

seridata=rand(1,para*nd*ml)>0.5; % DC=0

paradata=reshape (seridata,para,nd*ml); %size(51 ~* nd*ml)

%

ml modulation

[ich, qch]=qpskmod (paradata, para,nd,ml) ;
kmod=1/sqrt (2) ;
ich=ich.*kmod;

qch=qch. *kmod;

% CE data generation
kndata=zeros (1,fftlen) ;
kndata0=2.* (rand(1,52)>0.5)-1;
kndata (2:27) =kndata0 (1:26) ;
kndata (39:64) =kndata0 (27:52) ;
ceich=kndata; % CE:BPSK
ceqch=zeros (1, 64);

%      data mapping (DC=0) ———

{ichl, qchl1]=crmapping (ich, qch, fftlen,nd) ;

ich2=[ceich.' ichl]; % I-channel transmission data
qch2=[ceqch.' qchl]; % Qchannel transmission data

ee

x=ich2+qch2.*i;
y=ifft (x);
ich3=real (y) ;
qch3=imag (y) ;

2.
©

Gurad interval insertion

fftlen2=fftlen+gilen;

249


===== PAGE 255 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

[ich4,qch4]= giins (ich3,qch3, fftlen, gilen, nd+1) ;

%—— Attenuation Calculation

spow=sum(ich4.*2+qch4.%*2) /nd./para;
attn=0.5*spow*sr/br*10.% (-ebn0/10) ;
attn=sqrt (attn) ;

ZRRKKKK KKK KKK KK KK KK KKK fading channel KKKKKKKKK KKK KKK KKK KKK KKK KKK
$If you would like to simulate performance under fading, please
remove "*"

from the following four sentenses

%[ifade, qfade, ramp, rcos, rsin]=sefade (ich4,qch4,itau,dlvll1,th1,n0,i
tnd1,nowl, length (ich4),tstp, fd, flat);

Sitndl = itndlt+itnd0; % Updata fading counter

%ich4=ifade;

sqch4=qfade;

응*****×**×*×***×*ㅠㅠㄴㅠㅠㄴㅠㅠ×ㅠ×*×××※   Receiver   KKKKKKKKKK KKK KKK KKK KKK KEKE

%$———— AWGN addition
[ich5, qch5]=comb (ich4,qch4,attn) ;

%—Perfect fading compensation for one path fading —

SIf you would like to simulate performance under perfect
compensation, please remove "*"

from the following four sentenses
%$ifade2=1./ramp.* (rcos(1,:) .*ich5+rsin(1,:) .*qch5);
%qfade2=1./ramp.* (-rsin(1,:) .*ich5+rcos(1,:) .*qch5) ;

%Sich5=ifade2;

sqch5=qfade2;

%—— Guard interval removal ——
[ich6,qch6]= girem(ich5,qch5, fftlen2,gilen,ndt+1) ;

SS 주
rx=ich6+qch6é.*i;
ry=fft (rx);
ich7=real (ry) ;
qch7=imag (ry) ;

Fading compensation by CE symbol ———

250



===== PAGE 256 =====
SIf you would like to simulate performance under CE-based
compensation, please remove "*"

Sin this area

%

% preparation known CE data
%ce=1;

$ice0=ich2(:,ce);
sSqce0=qch2 (:,ce);

% taking CE data out of received data
$icel=ich7(:,ce);
Sqcel=qch7 (:,ce) ;

% calculating reverse rotation
siv=real ((1./(icel.*2+qcel.*2)) .* (ice0+i.*qce0) .* (icel-i.*qcel) );
sqv=imag((1./ (icel.*2+qce1.*2)) .* (ice0+i.*qce0) .* (icel-i.*qcel) );

% matrix for reverse rotation
sieqvl=[iv iv iv iv iv iv iv];
sqeqvl=[qv qv qv qv qv qv qv];

% reverse rotation
sicompen=real ( (ich7+i.*qch7) .* (iteqvl+i.*qeqv1) );
sqcompen=imag ( (ich7+i.*qch7) .* (ieqvl+i.*qeqvl1) );
%ich7=icompen;

$qch7=qcompen;

%—— CE symbol removal

ich8=ich7 (:,knd+1:nd+1) ;
qch8=qch7 (:,knd+1:nd+1) ;

% DC and pilot data removal
[ich9, qch9]=crdemapping (ich8,qch8, fftlen,nd) ;

~ demoduration

ich10=ich9./kmod;
qch10=qch9./kmod;
[demodata]=qpskdemod (ich10,qch10,para,nd,ml) ;

왕        error calculation

251


===== PAGE 257 =====
최신 이동통신시스템

262

Mobile Communications using MATLAB Simufation

demodatal=reshape (demodata,1,para*nd*ml1) ;
noe2=sum (abs (demodatal-seridata) ) ;
nod2=length (seridata) ;

% calculating PER
if noe2~=0
eop=eopt1;
else
eop=eop;
end
eop;
nop=nopt1;

% calculating BER
noe=noetnoe2;
nod=nod+nod2;

fprintf ('%d\t%e\tsd\n',iii,noe2/nod2, eop) ;
end

per=eop/nop;
ber=noe/nod;

ZRKKKEKKKK KKK KK KKK KKK KKK Output result HF HEI HE te Nee HIN Re ki oa de EK eI
fprintf ('Sf\tse\t%e\tsd\t%d\n',ebn0, ber, per, nloop, fd) ;

fid = fopen('BERofdmce.dat','a');
fprintf (fid, 'sf\t%e\t%e\t%d\t\n',ebn0,ber, per, nloop) ;
fclose(fid) ;

ZRKKKKKK KKK KK KKK KK KEK end OF ELLOS KEK EKKKKKKKKKEKKKKKKKKKKEKKKK

프로그램 4.9  ofdmci.m

% Program 4-9
% ofdmci.m
%
%

Simulation program to realize OFDM transmission system
Simulate effect of interfarence noise

00 ol?

ole

Programmed by T.Yamamura and H.Harada



===== PAGE 258 =====
%
% GI CE GI data GI data... (data 6symbols)
%

LaK KKK RK KKK KKK KKK KKK KK KKK preparation part KKK KKK KKKKKKKKKKKKKKK

para=52;      % Number of parallel channel to transmit (points)
fftlen=64;    % FFT length

noc=53;       % Number of carriers

nd=6;         % Number of information OFDM symbol for one loop
knd=1;        % Number of known channel estimation (CE) OFDM symbol
ml=2;         % Modulation level : QPSK

sr=250000;    % OFDM symbol rate (250 ksyombol/s)

br=sr.*ml;    % Bit rate per carrier

gilen=16;     % Length of guard interval (points)

ebn0=1000;    % Eb/NO

4 fading: initialization

tstp=1/sr/(fftlentgilen); % Time resolution

itau=[0];       % Arrival time for each multipath normalized by tstp
dlv1l1=[0];      % Mean power for each multipath normalized by direct
wave.

n0=[6];             % Number of waves to generate fading n0(1),n0(2)
th1i=[0.0];      % Initial Phase of delayed wave

itnd1=[1000];   % set fading counter

nowl=1;         % Number of directwave + Number of delayed wave
fd=150;         % Maximum Doppler frequency

flat=0;         % Flat or not (see ofdm_fading.m)

itnd0=nd* (fftlent+gilen) *10; % Number of fading counter to skip

interference wave initialization

oe

ci=10;           S:C/1I- ratio
ml2=2;           % modulation level

itau2=[0];

dlv12=[0];

n02=[6];

th2=[0.0];
itnd2=[10000+floor (rand(1) *10) *1000];
now2=1;

fd2=fd;

253


===== PAGE 259 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

flat2=0;
itnd02=nd* (fftlen+gilen) *300; % Number of fading counter to skip
%% store all parameters in one matrix "fadingpara"

fadingpara=zeros (8, length (itau2) );
fadingpara(1,:)=itau2;

fadingpara (2,:)=dlvl2;

fadingpara (3,:)=n02;

fadingpara (4,:)=th2;

fadingpara (5,:)=itnd2;
fadingpara (6, :)=now2;
fadingpara(7,:)=fd2;
fadingpara(8,:)=flat2;

Zk KK KR KR KKK KK KKK KK KK KK KK KK main loop part KKK KKKKKKKKKKKKKKKKKKKKKK

nloop=1000; % Number of simulation loops

noe = 0;    % Number of error data

nod = 0;    % Number of transmitted data
eop=0;      % Number of error packet
nop=0;      % Number of transmitted packet

Zk KR KK RK RK RK KK KK KK  transmitter  KK KK KKKKEKKKKKKKEKKKKKKKKKKK

for iii=1:nloop

seldata=rand(1,para*nd*ml)>0.5; % DC=0

paradata=reshape(seldata,para,nd*ml); %size(51 * nd*ml)

%      ml modulation

[ich, qch]=qpskmod (paradata, para,nd,ml) ;
kmod=1/sqrt (2) ;
ich=ich.*kmod;
qch=qch. *kmod;

% CE data generation
kndata=zeros (1, fftlen) ;
kndata0=2.* (rand(1,52)>0.5)-1;
kndata (2:27) =kndata0 (1:26);
kndata (39:64) =kndata0 (27:52) ;
ceich=kndata; % CE:BPSK

254



===== PAGE 260 =====
Treo |

ceqch=zeros (1,64);

%      data mapping (DC=0) ———

[ichl, qchl]=crmapping (ich, qch, fftlen, nd) ;

ich2=[ceich.' ichl]; % I-channel transmission data
qch2=[cegch.' qchl]; % Qchannel transmission data

Ema a ae 2 eS

x=ich2+qch2.*i;
y=ifft (x);
ich3=real (y) ;
qch3=imag (y) ;

%     Gurad interval insertion

fftlen2=fftlentgilen;
[ich4,qch4]= giins(ich3,qch3, fftlen, gilen, nd+1) ;

왕     Attenuation Calculation
spow=sum (ich4.*2+qch4.%*2) /nd./52;
attn=0.5*spow*sr/br*10.%* (-ebn0/10) ;
attn=sqrt (attn) ;

KK KK KK KKK KKK KKKKKKKKKEK     1             KKK KKK KKK KKK KKKKK KKK KKK
ading channe

SI£ you would like to simulate performance under fading, please
remove "*"

from the following four sentenses

[ifade, qfade, ramp, rcos, rsin]=sefade (ich4,qch4,itau,dlvl1,th1,n0,it
ndl1,nowl1, length (ich4),tstp,fd,flat);

itndl = itndlt+titnd0; % Updata fading counter

ich4=ifade;

qch4=qfade;

%%% interference wave addition

% interference

{iintw, gintw]=interwave (ci, spow,ml2, length (ich4),tstp, fadingpara) ;
itnd2 = itnd2+itnd02;

fadingpara(5,:)=itnd2;

ich4=ich4+tiintw;

qch4=qch4+qintw;

255



===== PAGE 261 =====
최신 이동통신시스템

256

Mobile Communications using MATLAB Simufation

Zk KK KKK KR KR RK KR RK KKK   Receiver   KKKKKKKKKKKKKK KKK KKK KKK KKK KKK

%$———— AWGN addition
{[ich5, qch5]=comb (ich4,qch4,attn) ;

%—Perfect fading compensation for one path fading —

SIf you would like to simulate performance under perfect
compensation, please remove "*"

sfrom the following four sentenses

sifade2=1./ramp.* (rcos(1,:).*ich5+rsin(1,:) .*qch5) ;
$qfade2=1./ramp.* (-rsin(1,:) .*ich5+rcos(1,:) .*qch5) ;

S$ich5=ifade2;

sqch5=qfade2;

왕     Guard interval removal ——

[ich6,qch6]= girem(ich5,qch5,fftlen2,gilen,nd+1) ;
ae era 내 6

rx=ich6t+qché.*i;

ry=fft (rx) ;

ich7=real (ry) ;
qch7=imag (ry) ;

%
%
SIf you would like to simulate performance under CE-based
compensation, please remove "*"

$in this area

%

Fading compensation by CE symbol

% preparation known CE data
ce=1;

ice0=ich2(:,ce);

qce0=qch2 (:,ce);

% taking CE data out of received data

icel=ich7 (:,ce);

qcel=qch7 (:,ce) ;

% calculating reverse rotation

iv=real ((1./(icel.*2+qce1.*2)) .* (ice0t+ti.*qce0) .* (icel-i.*qcel) );
qv=imag((1./ (icel.*2+qcel.%*2)) .* (iceO+i.*qce0) .* (icel-i.*qcel) );



===== PAGE 262 =====
% matrix for reverse rotation
ieqvl=[iv iv iv iv iv iv iv];
qeqvl=[qv qv qv qv qv qv qv];

% reverse rotation

icompen=real ( (ich7+i.*qch7) .* (ieqvlti.*qeqv1l) ) /
qcompen=imag ( (ich7+i.*qch7) .* (ieqvl+i.*qeqvl) );
ich7=icompen;

qch7=qcompen;

%—— CE symbol removal

ich8=ich7 (3, knd+1 1000 1) 7
qch8=qch7 (:,knd+1:nd+1) ;

%—— DC and pilot data removal ——

[ich9, qch9]=crdemapping (ich8,qch8, fftlen,nd) ;

%—————_ demoduration

ich10=ich9./kmod;
qch10=qch9./kmod;
[demodata]=qpskdemod(ich10,qch10,para,nd,m1l) ;

érror igatculation -<———

demodatal=reshape (demodata,1,para*nd*m1l) ;
noe2=sum (abs (demodatal-seldata) ) ;
nod2=length (seldata) ;

% calculating PER
if noe2~=0
eop=eop+1;
else
eop=eop;
end
eop;
nop=nop+1;

% calculating BER

noe=noe+noe2;
nod=nod+nod2;

257



===== PAGE 263 =====
최신 이동통신시스템

258

Mobile Communications using MATLAB Simufation

fprintf ('d\t%e\t%d\n',iii,noe2/nod2,eop) ;
end

per=eop/nop;

ber=noe/nod;

ZRKKKKKK KKK KKK KKK KKK KKK Output result KKK KKK KKK KKKKKK KKK KKK KKK KKK
fprintf ('%f\t%e\t%e\tsd\t%d\n',ci,ber,per,nloop, fd) ;
fid = fopen('BERofdmci.dat','a');

fprintf (fid, 'sf\t%e\te\t%d\t%d\n',ci,ber,per,nloop, fd) ;
fclose(fid);

ZRKEKKKKKKKKKK KKK KK KKK end of tile KKK KKK KKK KKK KKKKKEKKKKKKKKKEE

프로그램 4.10 interwave.m

% Function 4-10
% interwave.m

%

% Function to add interference wave

oe

Programmed by T.Yamamura and H.Harada

00 ole

function [iout, qout]=interwave (ci, spow,ml,nsamp, tstp, fadingpara) ;

LEKKKKK KKK KKK KK KK KK  variables  KKK KKKKKKKKKKKKEKKKKKK KKK

%Ci         : Carrier to interference ratio

% spow       : Power of desired signal

% ml         : Modulation level

% nsamp      : Number of samples

% tstp       : Time resolution

% fadingpara : Fading parameter

% iout       : Output Ich signal

% qout       : Output Qch signal

z  KK KKK KK KK KK KK KK KKK KKK KKK KKK KKK KKK KR KK KKK KKK KKK KKK KKK

itau=fadingpara(1,:);
dlvll=fadingpara(2,:);
n0=fadingpara(3,:);
thl=fadingpara(4,:);
itndl=fadingpara(5,:);
nowl=fadingpara (6,:);



===== PAGE 264 =====
fd=fadingpara(7,:);
flat=fadingpara(8,:);

$f 01 < 401

응용옹웅옹옹웅옹웅응옹응응 PLeparation part 웅웅융웅융웅응융웅웅웅웅융옹응응
옹응응 frame format

para=52;

fftlen=64;

noc=53; % the number of carrier

nd=6;    % the number of information sysmbol
knd=1;   % the number of known data symbol

sr=250000; % symbol rate
br=sr.*ml; % bit rate per carrier
gilen=16;   % the length of guard interval

%%% Set CE data load
kndata=zeros (1, fftlen) ;
kndata0=2.* (rand(1,52)>0.5)-1;
kndata (2:27) =kndata0 (1:26) ;
kndata (39:64) =kndata0 (27:52);

옹응응 Simulation start
%$%% fading initialization

SSSSSSSSSSSSSSEESEEEEESSESES CransmMitter SSSSSSSSSSSESSSSFEEEEESEFEF
seridata=rand(1,para*nd*ml)>0.5; % DC=0

paradata=reshape (seridata,para,nd*ml); %size(51 * nd*ml)

%%% ml modulation

[ich, qch]=qpskmod (paradata, para,nd,ml) ;

kmod=1/sqrt (2) ;

ich=ich.*kmod;

qch=qch. *kmod;

% CE modulation

ceich=kndata; % CE:BPSK
ceqch=zeros (1, 64);

%%% data mapping (DC=0)

259



===== PAGE 265 =====
최신 이동통신시스템

260

우

Mobile Communications using MATLAB Simulation

[ich2,qch2]=crmapping (ich, qch, fftlen,nd) ;
% addition of pilot carrier and CE symbol

ich22=[ceich.' ich2]; % I-channel transmission data
qch22=[ceqch.' qch2]; % Qchannel transmission data

66% IFFT

x=ich22+qch22.*i;
VSitii(x);
ich3=real (y) ;
qch3=imag (y) ;

%%% Gurad interval insertion

% guard interval insertion
[ich5,qch5]= giins (ich3,qch3,fftlen,gilen,nd+1) ;

%$%% fading Calculation
[ifade2,qfade2, ramp, rcos, rsin]=sefade (ich5,qch5,itau,dlvll1,thl1,n0,
itndl,nowl, length (ich5),tstp, fd, flat);

$%% C/I reduction
spowintw=sum(ich5.*%2+qch5.%2) / (nd) /52;
rint=spow/spowintw*10% (-ci/10) ;
iout=ifade2.*sqrt (rint) ;
qout=qfade2.*sqrt (rint) ;

else

iout=zeros (1,nsamp) ;
qout=zeros (1,nsamp) ;

end

Sk RK KK RK KK KK KK KK KK end of fi le KREKEKKKKKKKKKEKKKKKKKKKKKKKKK



===== PAGE 266 =====


===== PAGE 267 =====
코드분할다중접속 (ㅇㅁ\4ㅅ^) 기법

| 5.1 |e

CDMA 프로토콜은 다중접속 능력이 주로 코딩에 의해 달성되는 프로토콜로 구성
된다. 02844&에서는 각 사용자에게 자신의 정보신호를 부호화하는데 사용되는 고유의
코드 AAAS 부여한다, 수신기는사용자의 SEAALS 알고 수신신호를 복호하고
원 데이터를 복원한다. 코드신호의 대역폭이 정보신호의 대역폭보다 훨씬 크게 선택되
기 때문에 부호화 과정은 ASS 스펙트럼을 확산하고 이로 인해 확산 AWE spread
“spectrum (SS) 변조라고 알려져 있다. PSs ASE SS 신호라 부르고 CDMA 프로
ESS SS 다중-접속 (SSMA) 프로토콜이라 표기하기도 한다.

SS 통신의 기원은 정확하게 표현하기 어려운데, 이는 현대 SS 통신의 기원을 고해상
도 레이다, 방향검색, 유도, 상관검출, 정합필터, 간섭배제, 재밍회피, 정보이론, 보안통
신 등과 같은 다양한 결과물로부터 찾을 수 있기 때문이다 [1-101.

SS 변조방식은 원래 재밍회피와 낮은 검출확률로 인해 군사용 레이더와 통신에서 사
용되기 위해 개발되었다. 최근에서야 새롭고 저렴한 기술의 개발과 군사용 시장의 감소
로 인해 SS 장비 개발자와 제조자들이 민간부분에의 응용에 관심을 가지기 시작했다.
SS 변조방식으로 분류되기 위해서는 다음 두 조건을 충족시켜야 한다 [9]:

263


===== PAGE 268 =====
최신 이동통신시스템

264

Mobile Communications using MATLAB Simufation

zee 대역폭이 정보 대역폭보다 훨씬 커야 한다.
무선주파수 대역폭은 보내진 정보가 아닌 다른 함수에 의해 결정되어야 한다. 이
ae PM3} 같은 변조기법을 배제시킨다.

85 변조는 정보신호를 보다 큰 대역폭을 가진 전송신호로 전환한다. 이 전환은 데이
터와 무관하고 데이터신호보다 큰 스펙트럼 폭을 가지는 코드신호로 정보신호를 부호
화함으로써 이루어진다. 이 부호화는 원 신호파위를 보다 넓은 대역폭으로 확산시켜 낮
은 파워밀도를 갖게 한다. 전송된 대역폭과 정보 대역폭의 비를 85 시스템의 공정이득
processing gain (ㅠ,라고 부른다.

~

P

geo
2                                   (5.1)

BE 전송 대역폭이고 BL 정보신호의 대역폭이다.

수신기는 원 정보신호를 복원하기 위해 송신기에서 사용된 코드신호의 동기적으로
생성된 모사본과 수신신호를 상관시킨다. 이는 수신기가 데이터 변조에 사용된 코드신

코딩과 확산된 대역폭 때문에 ss 신호는 많은 협대역 Asse 다른 Yas 가지게
된다. 통신 시스템의 관점에서 가장 흥미로운 것들을 다음에서 논한다. 보다 나은 이해
를 위해, 각 성질을 그림과 함께 간단히 설명한다.

fox)

0) 다중접속 능력: 다수의 사용자가 동시에 SS 신후
자가 다른 코드와 적은 상관관계를 a 고 있는 고유의 HES 가지코 있
에 서로를 충분히 구분해낼 수 있다. 수신신호를 특정 사용자의 코드와 상관시키
면 이 사용자의 신호만 대역환원 고 다른 신호
있을 것이다. 그래서 정보 대역폭 내에서 원하는 사용자으
않다면 간섭 파워보다 훨씬 클 것이고 원하는 ASE FSS 1: 있다. gone
능력을 그럼 5.19] 보였다. 그림 5.1()에서, 두 사용자가 그들의 BAS 데이터신

42,
   er



===== PAGE 269 =====
코드분할다중접속 (6044) 기비 OSE

호로부터 SS 신호를 생성한다. 그럼 5.108/에서 두 사용자는 58 ASS 동시에 전
송한다. 수신기에서는 단지 사용자 1의 신호만 “대역환원”된 데이터가 복원된다.

(a)                                     (b)

를 그림 5.1 65 다중 접속의 원리: (3)확산 (6)대역환원

(0) 다중경로 간섭에 대한 Bs: 무선채널에서는 송신기와 수신기 사이에 하나의 경로
만 존재하지 않는다. 반사(와 회절) 때문에 신호는 여러 다른 경로로부터 수신된
다. 다른 경로의 신호들은 모두 송신신호의 복사본이지만 다른 진폭과 위상을 갖
는다. 수신기에서 이들 신호를 더하면 특정 주파수에서는 발전적이 되고 다른 주
파수에서는 퇴행적일 수 있다. 시간 도메인에서, 이는 분산된 ASS 가져온다.
99 변조는 이런 다중경로 간섭을 대항할 수 있다: 그러나 이는 사용된 변조방법에
크게 의존한다. 5.2장에서 다른 변조방식에 기반 한 여러 CDMA 프로토콜을 논
하는데 각 프로토콜에서 다중경로 간섭의 배제가 이루어지는 방법에 대해 논할

것이다.
@ 개인정보보호: 전송신호는 수신기에서 AES 알고 있을 때만 대역환원되고 데이
터가 복원된다.

® 간섭배제: 코드신호를 협대역 신호와 상호상관시키면 협대역 신호의 파워는 확
산되고 정보 대역폭에서 간섭 파워를 감소시킨다. 이는 그림 5.2에 보였다. Ss al
호 (9)는 AAS 간섭 (1)을 수신한다. 수신기에서 SS ASE “대역환원”되고 간섭
ASE 확산되어 대역환원된 신호에 비해 배경잡음으로 보이게 된다.

265


===== PAGE 270 =====
ZY 최신 이동통신시스템

Mobite Communications using MATLAB Simutation

를 그림 5.2 간섭배제

© 재밍회피 능력, 특히 협대역 재밍: 이는 다소 간섭배제와 동일하다. 이 성질은 99
변조를 군사 목적으로 사용하는데 적합하게 만든다.
© 낮은 도청확률 (Ｌ0ㅁ1) 혹은 위장운전: 낮은 파워밀도로 인해 98 신호는 검출이 어

렵다.

85 JES 생성하는 많은 변조방법이 존재한다. 우리는 가장 중요한 몇 가지를 간단
히 논할 것이다.

이 장은 다음과 같이 구성되었다. 먼저, CDMA 기법의 개념에 대해 5.2장에서 기술
한다. 5.3장은 확산 코드를 생성하는 방법을 3개의 대표적인 코드 시퀸스 MAAS,
Gold-A| AZ, 직교 Gold) AZ2AS 소개함으로써 제시한다. 5.4장은 MATLAB 프로그

을 사용한 송수신기의 구성을 논한다. 5.5장은 AWGN 채널과 레일리 페이딩 환경에
서의 BER BSS 보인다. 5.6장은 이 FS 마무리한다. 이 장과 연관된 모든 프로그램
은 부록 5A9} CDROM ES 수 있다.

| CDMA 기법의 개념

SSMA 흑은 CDMA 프로토클은 프로토콜의 개념 흑은 변조방식에 따라 두 가지 다
른 방법으로 분류될 수 있다. A 변째 붙류는 두 그룹의 프로토콜을 주는데 이는 평균
(averaging) 시스템과 회피(370102006) 시스템이다. 평균 시스템은 긴 시
AS 평균화함으로써 WIS 감소시킨다. 회피 시스템은 시간의 많은 부분에서 간섭을
피함으로써 간섭을 줄인다.

변조방식에 따른 CDMA 프로토콜의 분류는 다섯 가지 프로토콜 그룹으로 Ut:

266



===== PAGE 271 =====
코드분할다중접속 (0044) 기 OBE

(ASAAA (DS) EE FASS), Qtr HS (FH), (3)시간홈핑 (TH),
(4)chirp SS, (5)합성 (Hybrid). 이들 4, DSE 평균 SS 프로토콜이고, 합성 프로토콜은
합성방법의 일부로 28가 사용되었는지의 여부에 따라 평균 프로토콜로 분류될 수 있
다. 표 5.1은 두 가지 분류를 보여준다.

5.2.1-5.2.5장은 변조방식에 따른 CDMA 프로토콜을 논한다.

HH 5.18 SSMA 프로토콜의 분류

DS          TH          FH         Chirp       Hybrid
Averaging                  x                                                                                                           x
Avoidance                                        x                       x                       x                       x

5.2.1 직접 ABA

DS-CDMA 프로토콜에서, 변조 정보신호 (데이터신호)는 디지털 코드신호에 의해
직접 변조된다. 데이터신호는 아날로그 혹은 디지털신호일 수 있는데 대부분의 경우
지털이다. 디지털신호의 경우, 데이터 변조는 종종 생략되고 디지털신호가 직접 코드
신호에 의해 곱해지고 결과로 얻은 신호가 광대역 반송파를 변조한다. DS-CDMA 프로
토콜의 이름은 이 직접 곱셈에서 유래한 것이다.

그림 5.3은 DS-CDMA 송신기의 블록도이다. 이진 데이터신호가 RF 반송파를 변조
한다. 변조된 반송파는 코드신호에 의해 다시 변조된다. 코드신호는 많은 (+1이나ㄱ1인)
Oo eee 이드 는 코드 비트로 구성된다. 원하는 신호를 확산하기 위해서, 코드신

의 칩레이트는 정보신호의 칩레이트보다 훨씬 높아야만 한다. 코드 변조를 위해서는
FO 변조방식이 사용될 수 있지만 8『?나나 MSK 같은 PSK 형태가 사용된다. 데이터

ZS 생략하고 코드 변조에 BPSKS 사용하면 그림 5.49} 같은 블록도를 얻는다.

이 송신기로부터 얻어진 DSSS ASS 그림 5.5에 보였다. 그림에서 정보 신호 당 10

코드칩이 전송되어 (코드 칩레이트가 정보 칩레이트의 10배) 공정이득은 10이다. 실제
로 공정이득은 이보다 훨씬 크다.

ga

대

267


===== PAGE 272 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation
Data                  Wideband
6        0000
modulation
Carrier          Code
generator        generator

를 그림 5.3 DSSSMA 송신기의 BES

Binary
data    5         | Wideband
modulator
y
Code          Carrier
generator       generator
를 그림 5.4 +388 DSSS 송신기의 블록도
Data signal

268



===== PAGE 273 =====
Code              >  Data        Sead
demodulator           demodulator
개
Vv
Code           J.                             2
synchronization/ fe       0008               08110
tracking                generator           generator

를 그림 5.6 Dsss 신호의 수신기

신호의 전송 후에, 수신기 (그럼 5.6에서 SF 있는)는 지역적으로 생성된 EAA
늘                  대역환원하기 위해 코히어런트(60860600 복조를 사용한다.
대역환원 작용을 수행하기 위해, 수신기는 신호 확산을 위해 사용될 코드 AAAS 알아
야할 뿐만 아니라 수신신호의 코드와 지역적으로 생성된 SES 동기화시켜야한다. 이
동기화는 수신 시작과 함께 이루어져야하고 모든  아아아 fae 때까지 유지되어야 한
환원 후에, 데이터 변조신호가 생성되고 복조 후에, 원 데이터가 복원될 수 있다.
은 95 신호의 많은 장점에 대해 논한다.  도 관점에서 가장 중요한

것은 다중접속 능력, 다중경로 간섭배제, 협대역 간섭배제, 보안/개인정보 통신, LPIO]
다. 이제 DS-CDMA 경우에서 네 가지 성질에 대해 논할 것이다.

과

D 다중 접속: 다수의 사용자가 동시에 같은 PAS 사용하면, 시간과 주과수에서 중
첩되는 다수의 DSS 존재할것이다. 수신기에서, 코히어런트 복조가 코드 변
조를 제거하기 위해 사용된다. 이 작용은 정보 대역폭에서 원하는 사용자의 파워
를 집중시킨다. 원하는 사용자의 BES} 간섭자의 HES] 상호상관이 작으면, 코

히어런트 ASS 정보 대역폭에서 작은 간섭신호의 파워만을 나타낼 것이다.
@ 다중경로 간섭: 코드 시퀸스가 이상적인 자가-상관함수를 가졌다면, Taal
속시간일 때 상관함수는 [—T., T] 구간의 밖에서 0이다. 이는 원하는 신호

269


===== PAGE 274 =====
2) 최신 이동통신시스템
C

Mobile Communications using MATLA8 Simulation

와 27", 이상 지연된 복사 신호가 수신되었다면 코히어런트 복조가 지연신호를
간섭신호로 취급하고 정보 대역폭에서 이 신호의 작은 파워만을 나타냄을 의미
한다.

@ YOY 간섭: 수신기에서 코히어런트 검출은 수신신호와 지역적으로 생성된 코드
시퀸스의 곱을 포함한다. 그러나 송신기에서 본 바와 같이, 협대역 Ass} 광대역
코드 시퀸스의 곱은 협대역 ASS 스펙트럼을 확산시켜 정보 대역폭에서의 파워
를 공정이득만큼 감소시킨다.

@ LPL DS ASE 항상 전체 신호 스펙트럼을 사용하기 때문에 매우 작은 ey
전송파워를 갖게 될 것이다. 이는 DS ASS 검출하기 어렵게 만든다.

『

rr

i

위에서 AFM YAS 외에도, DSCDMA 프로토콜은 많은 다른 장점(+)과 단점(-)
을 가진다. :

+ 코딩된 신호의 생성이 쉽다. 이는 간단한 곱으로 행해진다.

+ 단지 하나의 반송파 주파수가 생성되어야 하므로, 주파수 합성기 (반송파 생성기)
가 간단하다.

+ 99 신호의 코히어런트 복조가 가능하다.

+ 사용자 간의 동기화가 불필요하다.

- 지역적으로 생성된 코드신호와 수신신호의 동기화를 얻고 유지하기가 어렵다. 동
기화는 칩시간의 몇 분의 일 내에 일어나야한다.

- 정확한 수신을 위해, 지역적으로 생성된 코드 AAAS 수신 코드 시퀸스의 동기
화가 칩시간의 몇 분의 일 내에 일어나야한다. 이는 긴 연속적인 주파수 대역을 이
용할 수 없는 점과 함께 확산 dass 실질적으로 10~20 MHzz 제한한다.

- 기지국에서 가까운 사용자로부터 수신된 파워가 멀리 떨어진 수신자로부터의 파
워보다 훨씬 크다. 사용자가 연속적으로 전체 대역폭으로 전송하기 때문에, 기지
국에 가까운 사용자는 끊임없이 기지국에서 먼 사용자에게 많은 간섭을 생성하게
되고 이는 PALS 불가하게 만든다. 이 근 원 효과는 모든 사용자의 신호가 같은 평

270



===== PAGE 275 =====
코드분할다중접속(0044) 기법 (Re

균 파워로 기지국에 수신되도록 하는 파워제어 알고리듬을 써서 제거할 수 있다.
그러나 파워제어라 불리는 이 제어기법은 구현하기 어렵다.

5.2.2 주파수 39

주파수-홈핑 CDMA (FH_CDMA) 프로토콜에서 변조 정보신호의 반송파 주파수는
일정하지 않고 주기적으로 변화한다. 시간간격 7'동안 반송파 주파수는 동일하게 유
지되지만 각 시간간격 후에 반송파는 다른 1 같은) 주파수로 도약한다. HY seu 은
코드신호에 의해 결정된다. 반송파가 가질 수 있는 주파수 AS 흡셋이라 부른다. F
SS 시스템의 주파수 점유는28-88 시스템과는 다르다.108 시스템은 전송 시에 전체 주
파수 대역을 차지하지만 FH A) ARS YASS] 적은 부분만을 차지하고 이 부분의 위
치는 시간에 따라 다르다.

#쁘시스템이 협 주파수 대역에서 전송하고 있다고 가정하자(그림 5.7 참조). 동일한
시간주기에 전송하는 28 시스템은 신호 파워를 전체 주파수 대역에 확산시켜 이 주파
수 대역에서의 ASS FH 시스템의 파워보다 훨씬 작게 된다. 그러나 FH 시스템
이 시간의 일부분에서만 이 대역을 사용하는 반면 DS 시 소틴은 BE 시간주기 동안 주
파수 대역에서 전송한다. 28-68와 FHSS 시스템의 차이를 그럼 5.7에 보였다.

4

Frequency
cl
+
:
Frequency
--*

oe [주운
PF eS

를 그림 5.7 FHS DS 신호의 시간/주파수 점유

그림 5.8은 FH-SS 송신기와 88 수신기의 블록도를 보여준다. 데이터 신호는 반
송파에 기저대역 몇 가지 변조기법이 Se 사용될 수 있고 어떤 변조방식
이 사용되는지는 주파수 S42] 응용에 중요한 문제가 되지 않는다. 일반적으로, of

af

271



===== PAGE 276 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

로그 신호를 위해서는 IM 변조가, 디지털 ASS 위해서는 FSK 변조가 사용된다. 코

드신호에 의해 제어되는 빠른 주파수 합성기를 사용하여 반송과 주파수는 전송 주과수
로 변환된다
i Baseband |_| Up-        |   |    Down-            Data       Data
modulator    converter          converter       |  demodulator
A
Synchronization
tracking
reine Pl 반청                               ¥
9                          Frequency    Code

synthesizer        generator

를 그림 5.8 FHSS 송수신기의

ful

록도

역과정이 수신기에서 일어난다. 지역적으로 생성된 AAAS 사용하여, 수신신호는
기저대역-변조   let  변환된다. 데이터는 (기저대역) 복조 후에 복원된다. 동기화/
추적 회로는 지역적으로 생성된 반송파의 Bo] 수신 반송파의 B39 패턴과 동기화되
어 신호가 정확하게 대역환원 되도록 한다.

FH-CDMA 프로토콜 Uo}, Sst] 읍핑 레이트에키반한 식별이 이루어진다.
홈의 수가 데이터 레이트보다 크다면 119 (F-FH) CDMA 프로토콜이라 부른다. 이
경우에는, 반송파의 주파수가 한 비트의 전송동안 수차례 변하게 된다. $2] 수가 데이
터 레이트보다 작다면 00\ FH (S-FH) CDMA 프로토콜이라 한다. 이 경우에는, 동일
한 주파수에서 다수의 비트가 전송된다.

하나의 $33 주파수에서 신호의 대역폭은 정보신호의 대역폭뿐만 아니라 FBS
의 형태와 3 주파수에 의존한다. 흡핑 주파수가 정보 대역폭보다 훨씬 작으면 (SFH
경우), 정보 대역폭이 점유 대역폭을 결정하는 주 인자가 된다. 그러나 B38 주파수가
정보 대역폭보다 훨씬 크다면, 홈핑신호의 펄스형태가 Se 주파수에서 점유 대역폭을

6
~

272



===== PAGE 277 =====
코드분할다중접속 (02014) 기법   1 0 |

결정할 것이다. 이 펄스형태가 매우 가파르다면 (급변하는 주파수로 인해 나타난), 주파
FAAS 매우 넓을 것이고 & 주파수의 수를 제한할 것이다. 주파수 Asp} 부드럽다
고 확신하면, 각 홈핑 주파수의 주파수 대역은 주파수 대역폭의 OF 1/27`,배가 되는데
T= 38 TASS 같다. 우리는 주파수 FE 전에 전송 FHS 감소시키고 HB 주파
수가 변했을 때 다시 높여줌으로써 주파수 변화를 부드럽게 만들 수 있다.

DS-CDMA 프로토콜에서와 같이, FHCDMASY] 성질을 다중접속 능력, 다중경로 간
섭배제, 협대역 간섭배제, 도청확률의 관점에서 논할 것이다.

0) 다중접속: FFHS} SFH CDMA 프로토콜이 어떻게 다중접속을 가능하게 하는지

이해하기는 매우 쉽다. FFH SEE SN, 하나의 비트는 다른 주파수 대역에서

ASA. 만약 원하는 사용자가 대부분의 주파수 대역에서 오직 하나의 전송자

라면, 원하는 신호의 수신파워는 간섭 파워보다 훨씬 클 것이고 정확하게 수신될

것이다. SFH 프로토콜에서는, 한 주파수에서 다수의 비트가 전송된다. 만약 다

른 사용자가 동일한 주파수 대역에서 전송할 확률이 상대적으로 낮다면 원하는

사용자는 대부분의 시간에서 정확하게 신호된다. 간섭하는 사용자가 동일한 주

파수 대역에서 전송하는 시간에는 오류-보정 코드가 ASA 데이터를 복원하기
위해 사용된다.

(2) 다중경로 간섭:『+ CDMA 프로토콜에서 한 비트의 전송동안 반송파 주파수가

수차례 변하게 된다. 그래서 특정한 신호 주파수가 많은    반송파 주과수에 변조되

고 전송될 것이다. 다중경로 효과는 다른 반송파 주파수에서 다르다. 결과적으로,

한 반송파 주파수에서 증폭된 신호 주파수는 다른 반송파 주파수에서 감쇄될 것

이다. 수선기에서, 서로 다른 $9 주과수의 응답은 평균되고 다중경로 간섭은 감
소하게 된다. ©] DS-CDMA 시스템의 다중경로 간섭배제만큼 효과적이지는 않
지만 전송을 향상시킨다.

@ 협대역 간섭: 협대역 신호가 SY 주파수 중 하나를 간섭한다고 가정하자. 만약
@7(공정이득)개의 FB 주파수가 존재한다면, 원하는 사용자는(평균적으로) 시
간의 1/G, 퍼센트에 간섭이 존재하는 FY 주파수를 사용할 것이다. 결국 간섭

273



===== PAGE 278 =====
ZY 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

은 @,의 인자로 감소한다.

@ LPI: FH 신호의 도청이 어려운 것은 전송파워가 낮기 때문이다. 전송하는 동안,
연속 전송에서 사용하는 것과 같은 saad 파워를 사용한다. 그러나 신호가 전
송되는 FAST 알려져 있지 않고 특정 주과수에서 전송의 지속시간이 매우 작
다. 그래서 DS 신호보다는 도청이 쉽지만 여전히 도청이 어렵다.

위에서 언급한 성질들 외에도, FHCDMA 프로토콜은 장점(+)과 단점(-)으로 구분

할 수 있는 많은 특성들을 가지고 있다:

+ 동기화가 DS-CDMA#1} 쉽다. FHCDMA] 동기화는 #41212] 수분의 일
내에 이루어져야 한다. 스펙트럼 확산이 높은 By 주파수가 아넌 많은 HAS 이
용해 얻어지기 때문에 홈시간은 DS-CDMA 시스템의 칩시간보다 훨씬 길 것이
다. 그래서 FH-CDMA 시스템은 보다 큰 동기화 오류도 허용한다.

+ @FH A957} 점유할 수 있는 다른 주파수 대역은 연속적일 필요가 없는데 이는
주파수 합성기를 스펙트럼의 다른 부분으로 쉽게 스킴하도록 만들 수 있기 때문
이다. 이 SYS 용이한 동기화와 함께 보다 넓은 SS 대역폭을 가능하게 한다.

+ FHCDMA® 회피 SS 시스템이므로, 다수의 사용자가 동일 주파수 대역에서 동
시에 전송하는 확률이 낮다. 기지국에서 먼 사용자의 전송은 기지국에서 가까운
사용자가 ASAE 다른 주파수로 전송할 가능성이 크기 때문에 기지국에서 수
신할 수 있다. 이런 이유로 FH-CDMAS] 근 원 성능은 28 보다 우수하다.

+ "쁘시스템이 보다 큰 대역폭을 사용할 수 있기 Heal], DS 시스템에 비해 협대역
간섭을 감소시킬 수 있는 가능성이 크다.

- 고성능의 주파수 합성기가 필요하다.

- 주파수 WES 바꿀 때 신호의 갑작스러운 변화는 점유
다. 이를 피하기 위해, 신호는 주파수가 바 때 오프, 온 되어야 한다.

- $3 동안에는 위상관계를 유지하기 어렴기 때문에 코히어런트 복조가 어렵다.

274



===== PAGE 279 =====
코드분할다중접속 (0044) 기법  fo |

5.2.3 Aztex

시간 홈핑 CDMA (TH-CDMA) 프로토콜에서, 데이터 ASE 사용자에게 할당된 코
드에 의해 결정되는 시간간격에서 급격한 격발로 전송된다.

Buffer                                                                                           Buffer
Slow in                                                                                                      Fast in
Data                                                                                                                            Data
ete |                         >     Data                 |        |        Data

modulator                           demodulator
Fast out                                                                                                     Slow out
기

Code                      Carrier                                 Carrier                   Code
generator        ?      generator                             generator               generator

를 그림 5.9 THCDMA 송신기와 THCDMA 수신기의 BEE

시간 축은 프레임으로 나뉘고 각 프레임은 1 시간 슬롯으로 나넌다. 각 프레임동안,
사용자는 MANZE SKS] 하나를 전송할 것이다. MAL 슬롯 중어느 것이 전송될지는
사용자에게 할당된 코드신호에 의해 결정된다. 사용자가 \ 시간 SKS 보내는 대신
하나의 시간 슬롯을 전송하므로 사용자에게 필요한 주파수는 M 인자로 증가한다. TH
CDMA 시스템의 블록도를 그림 5.10에 보였다. 그림 5.10을 그림 5.7과 비교하면, TH
CDMA 프로토콜은 모든시간동안 스펙트럼의 일부분을 사용하는 대신 짧은 기간 동안
전체 광대역 스펙트럼을 사용함을 알 수 있다.

Frequency

Time
를 그림 5.10 THCDMA 프로토콜의 시간주파수 그림

275



===== PAGE 280 =====
rey 최신 이동통신시스템
Mobile Communications using MATLA8 Simutation

이전에 기술된 CDMA 프로토콜과 같은 과정을 거쳐 THCDMAS] 다중접속 능력,
다중경로 간섭배제, 협대역 간섭배제, 도청확률의 성질을 논할 것이다.

0) 다중접속: THSS 신호의 다중접속 능력은 78-89 신호의 것과 같은 방식, 즉, 같은
주파수 대역에서 동시에 전송할 FSS 낮게 하여 얻어진다. THY] 경우, 모든 전
송은 동일한 주파수 대역에서 존재하고 이로써 같은 시간에 하나 이상의 전송이
존재할 확률이 낮다. 이는 다시 서로 다른 사용자에게 다른 코드를 할당함으로써
이룩된다. 만약 다수의 전송이 발생하면, 오류-보정 코드가 원하는 신호가 보정될
수 있도록 한다. 사용자 간에 동기가 존재하면, 할당된 SEE 특정한 슬롯에 하나
이상의 사용자가 전송하지 못하도록 하고 THCDMA 프로토콜은 사용자가 전송
한 슬롯이 고정되지 않고 프레임 단위로 변하는 TOMA 프로토콜로 변화한다.

@ 다중경로 간섭: THCDMA 프로토콜에서, ASE 감소된 시간에 전송된다. 결국
신호전송률은 증가하고 ASS 분산으로 근접한 비트와 중첩되게 한다. 그래서
다중경로 간섭배제에 대해서는 어떤 이득도 없다.

@ 협대역 간섭: THCDMA ASE 감소된 시간에 전송된다. 이 감소는 1/@,와 같
고 @,는 공정이득이다. 수신기에서, 원하는신호의 수신동안 간섭신호만을 수신
한다. 그래서 우리는 단지 시간의 1/@, 퍼센트 동안만 간섭신호를 수신하고 간
섭 파워를 G, 인자로 감소시킨다.

@ LPI: THCDMA®}} 사용자가 전송하는 주파수는 일정하지만 시간은 알 수 없
고 전송 지속시간은 매우 짧다. 특히 다수의 사용자가 전송할 때 전송의 시작과
끝을 그리고 어떤 ASS] 어떤 사용자에게 속하는지 구분하기 위해 도청하기는
어렵다.

aU

로
i=l}
tas

위에서 언급한 특성 외에도, THCDMA 프로토콜은 다음과 같은 장(+), 단(-)점을
가지고 있다.

+ THCDMAS] +42 FHCDMA 프로토콜보다 쉽다.
+ 데이터가 짧은 순간에 높은 파워로 전송되기 때문에 송신기가 피크파워-제한이

276



===== PAGE 281 =====
코드분할다중접속(0044) 기범 를

아닌 평균-파워-제한일 경우에 유용하다.

+ FHCDMAA] 근원 문제는 중요하지 않은데 이는 THCDMA?7} 회피 시스템
이 때문이고 이는 대부분의 시간에서 기지국에서 먼 단말기가 기지국에서 가까
운 전송에 의해 방해받지 않고 전송할 수 있음을 의미한다.

- 코드 동기화는 오랜 시간이 걸리고 수신기가 동기화를 수행해야하는 시간은 짧다.

- 다수의 전송이 발생하면, 많은 데이터 비트가 손실되어 성능 좋은 오류-보정 코드
와 데이터 인터리빙(0[6068008)이 필요하다.

5.2.4 (Chirp) 확산 스펙트럼

첩 SS 시스템이 아직 CDMA 프로토콜로 채택되지 못했지만 간단한 설명이 이 장에
포함되었다. 첩 98 시스템은 반송파의 선형 주파수 변조에 의해 대역폭을 확산시킨다.
이는 그림 5.11에 보였다.

12

<— 0 —>

fl

et

tl           t2

를 그림 5.11 8 변조

=

공정이득 @,는주파수가다양한대역폭 #와주어진 AS 파형의 지속시간 TS] 곱
이다:

G, = BT                                 (5.2)

277


===== PAGE 282 =====
01 최신 이동통신시스템
Mobile Communications using MATLAB Simuiation

5.2.5 tha(Hybrid) 시스템

합성 CDMA 시스템은 위에서 언급된 SS 변조방식의 S 혹은 그 이상의 조합으로 이
루어진 모든 CDMA 시스템을 포함한다. 우리의 논의를 29, FH, TH 변조로 제한하면
4가지 합성 시스템이 존재한다: DS/FH, DS/TH, FH/TH, DS/FH/TH.

합성 시스템의 아이디어는 각 변조방식의 특정 장점들을 결합하자는데 있다. 예를 들
어, AY DS/FH 시스템은 DS 시스템의 반-다중경로 PABFH AAS 좋은 근원
작동 성질을 얻을 수 있다. 물론, 송수신기의 복잡도가 증가하는 단점도 존재한다. 그림
5.12는 결합된 DS/FH CDMA 송신기의 블록도를 보여준다.

Data                                                        Up
converter

Code                       Code                  Frequency
generator                generator           synthesizer

ae

Code clock

를 그림 5.12 합성 DSFH 송신기

데이터 ASE A DS SEATS 사용해 확산된다. SSE 다른 코드 AAA] 따라
두 코드 사이의 수정된 관계를 보

278



===== PAGE 283 =====
코드분할다중접속(0044) 기 OE

MER 확산 코드의 생성

이전에 기술된 CDMA 시스템에서, 코드 AAS 유형 선택은 다중경로 간섭과 다
중사용자 간섭 모두에 대항하는 항목으로 중요하다. 간섭을 극복하기 위해, 몇 가지 조
건이 만족되어야 한다:

코드 생성 함수 집합으로부터 생성된 각 코드 시퀸스는 일정 길이로 주기적이어야
한다.

 코드-생성 함수 집합으로부터 생성된 각 코드 시퀸스는 자신의 시간 전이된 코드
와 구분이 쉬어야 한다.

@ 코드-생성 함수 집합으로부터 생성된 각 코드 시퀸스는 다른 코드 시퀸스와 구분
이 쉬어야 한다.

첫 번째와 두 번째 조건은 실내외 무선 환경에서의 이동통신에서 발생하는 다중경로
전송효과에 있어서 중요한 요인이다. 세 번째 조건은 통신시스템의 다중접속 능력에 있
어 중요하다. 조건 (1)과 (2)를 위한 코드의 식별 WAS 특정하기 위해, 자기상관함수
와 상호상관함수가 각각 사용된다. 자기상관함수는 식별 레벨을 측정하기 위해 사용
되고 다음과 같이 정의된다. :

rye lt)= 29, 040+ㅜ000                           (53)

자기상관함수를 보여주는 MATLAB 함수를 위해 프로그램 5.194] = autocorr.m?]
사용되어야 한다. 이 함수의 인자는 시퀸스의 이름과 코드의 주기의 수이다. 예를 들어,
코드1(7) =, 1,1,-1,-1, = 피의 저키상란함수를 계잔하기 위해서는 다
음 명령을 MATLAB Zo] 입력하면 된다.

>> X= [217 1, sk La 21. 7

>> Rxx=autocorr (X);

279


===== PAGE 284 =====
ZY 최신 이동통신시스템
C

280

Mobile Communications using MATLAB Simulation

이 경우, 우리는 이 장에서 기술될 코드길이 7인 3단계 \시퀸스를 사용한다. 자기상
BRS /=4^ㆍ7'(&=1, 2, 3,…)에서 7이고 다른 점에서는-1이다. 이 BS 계산하기
위해, 상관함수 RS #※로 계산할 수 있다.

>>: RXX

반대로, 상호-상관함수는 서로 다른 코드 AAA ※(7)와 V4) 사이의 상관값이고
다음과 같이 정의된다.

ry (= Tf XOVC+ adr        (5.4)

상호상관함수를 보여주는 MATLAB 함수로 프로그램 5.204] crosscorr.m°] A}
용되어야 한다. 이 함수의 인자는 AAAS] 이름과 코드 주기의 수이다. 예를 들어, 코드
=, 6 1, 도이 as YOO STS TT, Ht Ay 1 의 성호
상관값을 계산하기 위해서는 다음과 같이 MATLAB 창에 입력하면 된다.

22 [1 Laie a 12
o> 그. 007 bs ped al fe
>>, Rxy=crosscorr (X,Y) ;

이 경우, 3단계의 MA AAS} 코드길이 79] BA AAAS 사용한다. 두 코드의 상관
RE 매우 작다. 이 BS 계산하기 위해, 상관함수 Rxy2] HS 계산할 수 있다.

>> Rxy

자기상관과 상호-상관함수를 사용하여 확산 코드가 구현되고 평가된다.

이 장은 확산 HES 예로 세 가지 코드 AAAS 소개한다. (1) M-A) AA (2) Gold 시
A? (3) 직교 Gold 시퀸스. 이 장에서는 이들 BES MATLAB 프로그램을 통해 생성
하는 방법과 생성된 코드의 특성에 대해 설명한다.



===== PAGE 285 =====
코드분할다중접속(0ㅁ044) 기법 ORE

5.3.1 선형 귀환 전이 레지스터 (10637 feedback shift 76919[61)에 의한
코드 생성

코드 EAAAS 생성 하는 몇 몇 가지 방법 이 존재 한다.  한 가지 방법은 귀환 저 전이 레지스 ^
터를 사용하는 방법이고 이 방법은 CDMA 시스템에서 일반적으로 사용되는 방법이다.
전이 레지스터는(1에서 ＊번호로 표시된) 많은 셀로 구성되어 있는데 각 AS 저장단
위로 시계 BAS 제어 하에 출력에 내용을 전달하면서 동시에 입력으로부터 새로운 내

을 읽어 들인다. 귀환 전이 레지스터의 표준적인 구성에서, A me] 입력은 A m-1
의 출력의 함수이고 셀 ＊(전이 레지스터의 마지막 셀)의 출력이 원하는 코드 AAAS
형성한다.

h=1        h,=1             h=1
(1) >} (2)    (3) >) (4) Rey (5)     >

h(x) =X° +X? +1

를 그림 5.13 단일 선형 이진 전이 레지스터

셀 72ㅡ1과 셀 /의 출력을 셀 mo] 입력으로 결합하는 함수는 선형 혹은 비선형 함
수일 수 있다. 이는 우리에게 두 가지 유형의 귀환 전이 레지스터를 준
선형 귀환 전이 레지스터 (413 FSRs)7} 비선형 8888. 두 가지 유형의 차이점은 참고
문헌 [1, 11]에 설명되었다.
이 AS AB FSRsH PE] 생성된 몇 가지 시퀸스에 대해 기술한다.
림 5.13은 단일 선형 이진 전이 레지스터를 보여주는데 이 레지스터는 발생 다항식
Mx) =×"+×“+ 로부터 AAAS 생성할 수 있다. 일반적으로, n AA] 선형 이진
전이 레지스터의 구성은 발생기 다항식으로 기술되는데 이는 /차의 이진 다항식이다.
차수 n& 전이 레지스터의 섹션의 수이다.

h(x) =h,x* +h, 24271 (h, € (0,1})          (5.5)

281



===== PAGE 286 =====
7y  최신 이동통신시스템
C

Mobile Communications using MATLAB Simufation

그림 5.13에서는 Ad) =2° 42°41, th=ho=1, //,。=0이다. 이 전이 레지스터
를 사용함으로써 대부분의 확산 코드 시퀸스가 생성된다.

5.3.2 /[- 시퀸스

\시퀸스는 단일 19로 생성된다. 특별히, 최대 가는 주기 ( /,=3*-1)의 ANA
는 단계 이진 전이 레지스터에 의해 선형 귀환으로 생성된다. MAAS 생성하기
위해, 발생기 다항식는 차의 발생 다항식이어야만 한다. 그래서 주기적인 \시퀸스
의 자기상관함수는 다음과 같이 주어진다.

1        t=OmodN,
7) =
-1/N, _ otherwise                           (5.6)

n#0 mod 42}8, 3가지 값을 갖는 상호상관함수를 갖는 최대길이 AAAS] 쌍이
존재하고 [12], 두 값은 { - (72) , (7) -2}이다. 이때 7(20)은 다음 식과 같다.

나 2 지기 “ntodd
t(n) =           2)/2
142°? n:even                            (5.7)

MAIAAS 생성하기 위한 BEE 프로그램 5.3에서 mseqg. mes 프로그램되었다.
레지스터의 수, 레지스터의 초기 값 귀환 탭의 HA)7} mseq.ms] 인자로 주어졌다. 예
를 들어, 레지스터의 수가 3이고 레지스터의 초기 값이 [1, 1, 1] 그리고 귀환 탭의 위치
가 A 번째와 세 번째 탭인 경우를 가정하자. 발생 다항식은 A(x) =×“+*ㅠ+ 1으로 표
현되고 MAALS 구성하기 위한 진이 레지스터는 그림 5.14에 보였다.

<

Lott

를 그림 5.14 347) MARA

282


===== PAGE 287 =====
코드분할다중접속(6ㅁ044) 기법 ㅠ0)"Ｌ\\

*\시퀸스가 발생 다항식에 의해 생성될 때, 다음 명령이 실행된다.
>> ml=mseq(3, [1,3], [27 171] )

결과로서, 3단계 MAAAIL 1, 1,0, 1, 0, 0]이 벡터로 생성된다. 여기서,0ㅁ960.2은
4번째 인자를 갖는데 이는 출력의 +S 나타낸다. 출력의 수 No] 주어지면, 2 단일-
칩 전이 MAJ AAS 얻게 된다. 예를 들어, 또 다른 3단계 %시퀸스는 다음 명령으로 생
성된다.

>> m2=mseq(3,[2,3},[1,1,11,,3)

이 명령이 실행되면, 세 개의 단일칩 전이 \시퀸스를 얻는다.

m2 =
1   af   1   0
He   1       0
a   0   1   1   1;   0   0

프로그램 5.4에서 mseg.m 함수에서 사용된 shift.mo] 사용자에 의해 주어진 칩의 수
를 전이하는 함수의 하나이다.
프로그램 5.1과 5.2에 S724) autocorr.m} crosscorr.m 함수를 사용해서, 시
B29] 특성이 평가될 수 있다. 먼저, 생성된 코드 시퀸스가 0과 12 구성되므로, 코드
AMAZE 1F 1로 구성되는 코드 시퀸스로 다음 VSS 통해 변환된다.

>> ml=m1*2-1;
>> m2=m2*2-1;

3단계 M-A)al2: ml 2] 자기상관함수는 다음 명령으로 계산된다.
>> autocorr (m1)

결과로 자기상관값[7,-1,-ㄱ1,ㄱ1, lel 얻어진다. 자기상관된 값은 (5.6)을 만족
한다.
다음으로71과ㅠ201,:)의 ASPIRE 다음 명령으로 얻어진다.
283



===== PAGE 288 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

>>. crosscorr (ml; mZ (4527)

결과로, 상호상관값 [3,-1, 3,-1, -1, -5, 3]이 얻어진다. 이 ABE 세 가지 | 즉
[-1, —¢(n), (72) -2]을 갖고(5.7)로부터 7(72)=5이다. 그래서 21과2ㅁ201,:)은
선호되는 쌍의 SYS 갖는다. 《시퀸스의 FE 매우 작다. 표 5.2는 몇 가지 단계의 M-
시퀸스를 AVS 수 있는 귀환 탭의 정보를 보여준다. MA]AAl 기반하여 다른 확산

EAAA7} 구성된다.

#2528 귀환-탭 정보

Number      Period      Number of       Feedback Tap        Number of
of Stage                M-Sequence        (Example)        Preferred Pair
3           7            2        (1,3)(2,3)                    2
4           15            2        (1,4)
가          31            6        (2,5)(2,3,4,5)(1,2,4,5)            3
6          63            6        (1,6)(1,2,5,6)(2,3,5,6)            `

4,7)(1,2,3,7)(2,3,4,7
7        129        18     sy    :   :         6
(1,7)(1,3,6,7)(2,4,6,7)

(2,3,4,8)(3,5,6,8)
8                255                  16                                                       0
(2,5,6,8)(1,3,5,8)

(4,9)(3,4,6,9)(4,5,8,9)
(1,4,8,9)(2,3,5,9)

N

9            511             48

5.3.3 Gold 시퀸스

\시퀸스는 좋은 자기상관 SAIS 가지고 있다. 그러나 함수로 \\시퀸스를 사용하
는 이동통신 시스템의 수는 매우 작다. 이는 동일한 코드 길이와 동일한 상관 특성을 갖
는 \시퀸스의 수가 제한적이기 때문이다. BS 사용자가 서로 통신하는 CDMA A) 2:
템이 구현할 때, 우리는 동일한 상관 값을 갖는 많은 다른 코드를 갖는 시퀸스가 필요하
다. Gold 시퀸스는 그런 시퀸스의 하나이다.

284



===== PAGE 289 =====
코드분할다중접속(6044) 기 ORE

Gold 4) AA Gold] 의해 개발되었다 [13]. 이는 5.3.2장에서 기술한 선호되는 쌍
의 관계를 갖는 두 개의 MA] 4129] exclusive OR (EXOR)= 생성된다. 3단계 전이 레
지스터가 사용된 발생회로를 그림 5.15에 보였다. 발생회로에 의해 생성된 Gold 시퀸
스의 구는 2" + 1이고 [1,11],ㅅ단계 전이 레지스터를 사용할 때 레지스터의 초기 HS
변화시키고 두*《시퀸스를 더함으로써 얻어진다. 두선호되는 쌍의 \《시퀸스로부터 생
성된 Gold 시퀸스에서, 상호상관 RE 세 가지 값을 갖는데 { -1, —t(n), t(n) -2}
가 그것이고 7(70)은 (5.7)에 보였다.

Gold 시퀸스의 생성함수는 프로그램 5.5에 8010860.피에 프로그램하였다. Gold A) 4
스를 생성하기 위해, 두 ASHES] MA|AZAS goldseq.mo] 제시했다. 예를 들
두 \시퀸스로부터 3단계 Gold AAS 생성하기 위해서는 다음 명령을 수행 a

>> ml=mseq(3, [1,3], [1,1,1]);

>> m2=mseq (3, [2,3],[1,1,1]);
>> gl=goldseg(m1,m2)

결과로, 우리는 길이 72] 벡터인 3단계 Gold AAA [00001 1 0]을 얻는다. 초기 H
을 변화시킴으로써, 다른 Gold JAAS 얻을 수 있다. 상호상관 RS 계산하기 위해
= Gold A) 827} 생성되었다.

>> m3=mseq (3, [1,3], 11, 0, 01) ;
>> m4=mseq (3, [2,3], [1, 0, 1] ) ;
>> g2=goldseq(m3,m4)

aa   2 >} 3
san)»
커 1 ee 2   3

+

를 그림 5.15 307 Gold AWA

285



===== PAGE 290 =====
Zy 최신 이동통신시스템

Mobile Communications using MATLAB Simufation

여기서, goldseq m2 3번째 인자를 가졌고 이는 출력의 수를 나타낸다. 출력의 수 WV
이 인자로 주어지면 개의 단일-칩 전이 001 시퀸스를 얻을 수 있다. 예를 들어, 다음
명령이 실행될 때:

>> gl=goldsegq(ml1,m2, 3)
세 개의 단일-칩 전이 Gold A]A27} 얻어진다.

91 =

0         1         0         1          0         0         0
프로그램 5.1과 5.2에 {2724S autocorr.my} crosscorr.m-S 사용하여 M-A] AA]
특성이 평가될 수 있다. 먼저, 3단계 6010 4A gl (1,:)9] 자기상관함수가 다음과 같
이 계산되었다.

>> gl=g1*2-1;
>> autocorr(gl1(1,:))

결과로, 자기상관값 [7, 3, -1, 그, -1, 3]이 얻어진다. 자기상관값은 동기화 지점에서
큰 값이다. 그러나 다른 점에서는 변동된다.
다음으로, 8101,:)과 1(2,:)의 상후상관함수를 다음 명령으로 얻는다.

>> 06008306 (9217 gL 2; 1: ) )

AAS, FSU KCL 3, -1, 8. 1} 3, WS SEG.
이 결과는{ -1, —t(n), t(n) -2}의 HS 취하고 (5.7)에서 t(n) = 3°14.

5.3.4 직교 Gold ABA

Gold JAAS MAI AAS} 비교해 많은 다른 SES 가지고 있다. 그러나 6010 4) 4
ANE 몇 가지 문제점이 존재한다:

286



===== PAGE 291 =====
코드분할다중접속 (CDMA) 기법 lo I

D 03} 19] 비율이 항상 균형을 이루지는 않는다.

(2) 0010 시퀸스의 상호상관 Ho] 동기화된 환경에서 0이 아니다.

@ 코드 길이가 홀수이다. 이 결과, Gold AAAS 생성하기 위해서는 특별한 Be
필요하다.

J
은

위 문제들을 해결하기 위해, Gold A] A Ao} 한 칩이 더해져서 0과 1의 균형을 맞춘다.
이 AAAS 직교 Gold 시퀸스라 한다. 직교 Gold AAAS 상호-상관 he 동기 지점
에서 0이다. 다른 지점에서는, AAAS 특성은 6010 4) AAS 유사하다.

EE] 컴퓨터 프로그램을 통한 송신기와 수신기의 구성

이 장에서는 동기식 DSCDMAS] BERS 얻기 위한 과정을 보인다. 동기식 DS-
CDMAS] 구성은 그림 5.16에 보였다. 동기식 DS-CDMA, 사용자는 정보 데이터
를 확산하기 위해 자신의 AAAS 사용한다.

각 사용자의 단말기에서, 정보 데이터는 Al 번째 변조방식 (aj), QPSK 9} BPSK)oj] 의
해 변조된다. 그 다음, 변조 즈데 이터의 Al 번째 비트는 MA) AAU Gold-A) A A>} 같은
코드 시퀸스를 사용하여 확산된다. 모든 사용자의 확산 데이터는 동시에 기지국에 전송

된다. 기지국은 각 사용자에 할당된 코드 AAAS 수신신호를 상관시켜 각 사용자의
정보 데이터를 검출한다.

시뮬레이션에서, QPSK7} Al 번째 변조방식으로 사용되었다. 주 프로그램은 프로그
램 5.6에 보였고 시뮬레이션 프로그램은 프로그램 5.7-5.11에 보였다. A 번째 변조가
QPSK9}7] 때문에, 시뮬레이션에서 프로그램은 3장에서 논의된 008 프로그램에 기
반한다. 그래서 QPSK $} 동기적 DSCDMA 프로그램에서 공통된 내용은 기술하지 않
는다.

287



===== PAGE 292 =====
최신 이동통신시스템

Mobite Communications using MATLAB Simufation

Transmitter

User1 |

User 2

User N

Code N

Receiver
User 1

Code 1
User 2

Code 2
oy    User N

Code N

를 그림 5.16 동기식 DS-CDMA 시스템

프로그램 5.6에 보인 시뮬레이션에 사용된 주된 프로그램의 인자들은 다음과 같이

정의되었다.
시호   = 256000.0;
ml   = 2;
br   = sr * ml;
nd   = 100;
ebn0 = 3;
irfn   = 21?
IPOINT = 8;
alfs   ee 트라

필터 계수는

[xh}==

oe

{xh2]=

00

288

00 00 00 oP 00 OP

oe

y

QPSK 성능을 평가하는 프로그램에서 보인 바와 같이 정의되었다.

symbol rate

number of modulation levels
bit rate

number of symbol

Eb/No

number of filter taps
number of oversample

roi. 067 factor

hrollfcoef (irfn, IPOINT,sr,alfs,1);
T FILTER FUNCTION
hroiitcoeft (irfin, [POINT;,sr, alfis;0)-;
R FILTER FUNCTION



===== PAGE 293 =====
코드분할다중접속 (6044) 7 OR

086&와 DS-CDMA 프로그램의 차이는 사용자 수와 확산 BES] 생성을 정의하는
인자에 있다. 이 시뮬레이션에서는, 세 가지 유형의 확산 AA 즉, MAlAlA, Gold 시
퀸스, 직교 Gold 시퀸스가 사용되었다. 변수 seg 1, 2, 3으로 변화시켜 코드 AAAS
AGA}. 다음으로, 레지스터의 수를 \시퀸스를 생성하도록 설정한다. 동기적 DS-
00844에서, 서로 다른 사용자에게 할당될 수 있는 코드 시퀸스의 수는 코드 길이와 같
다. 그래서 코드 BAS 길이는 사용자의 수보다 커야한다. 코드 시퀸스를 생성하기
위해, 우리는 레지스터의 수, 귀환 탭의 위치, 레지스터의 초기 값을 설정해야 한다.
Gold 시퀸스와 직교 Gold JAAS 생성하기 위해서는 두 개의 \시퀸스가 필요하다.
그래서 다음 인자가 사용된다.

user = 1?           % number of users
seq   = 1;          % 1:Msequence 2:Gold 3:Orthogonal Gold
stage = 3;             number of stages

ptapl =-(1-3>
ptap2 = [23];
regil=—fi-t tt?

pegi2 = [roe ti     % initial value of register for 2nd

position of taps for lst

position of taps for 2nd

de 00 oP OP

initial value of register for lst

이들 인자를 사용하여 확산 코드가 생성되고 생성된 코드는 변수 0006에 저장된다.
여기서, code 사용자 수와 코드 Al AAS] 길이를 곱한 시퀸스의 행렬이다. &시퀸스
가 함수 mseq.m 2 =, Gold 4] 4127} 함수 8010860.0ㅁ으로 생성된다. 직교 Gold 시퀸스
Gold 시퀸스의 머리나 꼬리에 0 비트의 데이터를 첨가해 생성할 수 있다.

switch seq

case 1                           % Msequence

code = mseq(stage,ptapl, regil,user) ;

case 2                            $ Gold sequence
mi   = mseq(stage,ptapl, regil) ;
m2   = mseq(stage,ptap2,regi2);
code = goldseq(ml,m2,user) ;
case 3                            % Orthogonal Gold sequence
m1   = mseq(stage,ptapl, regil);

289



===== PAGE 294 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

m2

code

mseq (stage, ptap2, regi2) ;

[goldseq(m1,m2,user),zeros(user,1)];

end

생성된 코드 AA27} OF 1로 구성되므로, 프로그램은 이를-1과 1 BPs

Q
Qo
요
0
ll

Code: * <7 ="

Q
paar
@
He
ㅣ

length (code) ;

다음으로, 페이딩 시뮬레이터를 위한 인자가 정의된다. 4806가 0일 때, 시뮬레이션
은 AWGN 채널의 BER 성능을 평가한다. 4806가 1일 때, 시뮬레이션은 레일리 페이딩
환경에서의 BER 성능을 평가한다.

rfade = 0;                       % Rayleigh fading
% O:nothing 1:consider
itau   = [0,8];                   % delay time
divil. ;=.,[0.0;,40.0} 7              % Attenuation level
nod     = a ae                   % number of waves to
% generate fading
thl    = [0.0,0.0];               % initial Phase of
% delayed wave
itndl = [3001,4004];             % set fading counter
nowl   = 2;                       % number of directwave +
% delayed wave
tstp   = 1/ sr / IPOINT / clen; % time resolution
fd     = 160;                     % doppler frequency [Hz]
flat   = 1;                       % flat Rayleigh environment

itndel = nd * IPOINT * clen * 30;

그 다음, 시뮬레이션 루프의 수가 설정된다. 전송 데이터 비트의 수와 오류의 수를 나
타내는 변수가 초기화된다.

nloop = 1000;                     % simulation number of times

290



===== PAGE 295 =====
코드분할다중접속 (CDMA) 기법   io |

noe   = 0;                        % Number of errors
0;

nod   =                           % Number of data

in-phase 채널로 전송되고 QPSK] 의해 직각 위상 변조된 데이터가 AS 데이터를
확산하는데 사용된 코드 AAAS} 곱해진다. 확산 데이터가 오버 샘플되고 70110 필
Bo 의해 필터링되어 통신채널로 전송된다. 여기서, 함수 compoversamp2.m>}
compconv2.m-< 00000ㅠ6[98072.0(프로그램 3.8)과 compconv.m(£=-1%4 3.7)를 개
정한 것이다. 이들 새로운 함수의 입력에 사용되는 형태는 벡터나 행렬에 의존하지 않
는다. 이들 프로그램을 프로그램 5.9와 5.10에 보였다.

data = rand(user,nd*ml) > 0.5;

[ich, qch] = qpskmod(data,user,nd,ml);
% QPSK modulation

{ichl,qch1] = spread(ich,qch, code) ;
% spreading

{ich2,qch2] = compoversamp2 (ich1,qch1,IPOINT) ;
% over sampling

[ich3,qch3] = compconv2 (ich2,qch2, xh) ;

% filter
그림 5.16에 보인 바와 같이, 사용자로부터 송신된 ASE 합성된다.

if user ==                        % transmission
ich4 = ich3;
qch4 = qch3;

else                              %

ich4 = sum(ich3);

ㅣ

qch4   sum(qch3) ;

end

그 다음, 합성된 ASE 레일리 페이딩 채널에 의해 오염된다. 실제로, BE 사용자의
전송신호는 구별되는 레일리 페이덩에 의해 오염된다. 그러나 시뮬레이션에서는 합성
된 신호가 레일리 페이덩에 의해 오염된다.

291



===== PAGE 296 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

if rfade == 0
ich5
qch5

ich4;

qch4;
else
{ich5,qch5] = sefade
(ich4,qch4,itau,dlvll,th1,n0,itnd1,
nowl, length (ich4),tstp,fd, flat) ;
itndl = itndl + itndel;          % fading channel

end

수신기에서, QPSK ASS] 시뮬레이션에서 보인 바와 같이, AWGNO] 수신 데이터
에 첨가된다. 그 다음, 오염된 신호를700[10110# 필터로 필터링한다. 여기서, comb2.m
= attno] 맞게 comb.m(=2249 2.4)를 개정한 것이다. 개정된 프로그램은 프로그램
5.11에 보였다.

spow ~ 8600(206ㄷ90 (1003 022 가 (90093 ;72))- /- nd;

% attenuation Calculation

attn = sqrt(0.5 ^ spow *-sr / br 시 10*(-ebn0/10) )
{ich6,qch6] = comb2(ich5,qch5,attn) ;

% Add White Gaussian Noise (AWGN)

[ich7,qch7] = compconv2 (ich6,qch6, xh2) ;   % filter
sampl-= irfin * LPOINT + 1;

ich8 = ich7(:,sampl:IPOINT: IPOINT*nd*clen+samp1-1) ;
qch8 = qch7(:,sampl:IPOINT: IPOINT*nd*clentsamp1-1) ;

다시 샘플링된 데이터는 모든 사용자의 합성 데이터이다. 합성 데이터를 송신기에서
사용된 확산 코드와 상관시킴으로써 모든 사용자의 ASA 데이터가 검출된다. 상관은
프로그램 5.8에 의해 행해진다.

[ich9 qch9] = despread(ich8,qch8,code); % despreading

상관된 데이터는 QPSK] 의해 복조된다. 그 다음, 모든 사용자에 대해 총 오류의 수
를 계산한다. 마지막으로, BERS] 계산된다.

292



===== PAGE 297 =====
코드분할다중접속 (60144) 기법  fo |

demodata = qpskdemod(ich9,qch9,user,nd,m1l) ;
% QPSK demodulation

noe2 = sum(sum(abs (data-demodata) ) ) ;

nod2 = user * nd * ml;

noe = noe + noe2;

nod = nod + nod2;

IEG cer as

5.5.1 AWGN 환경에서의 BER 성능

프로그램 5.6을 실행하여

>> dscdma

AWGN 환경에서의 동기식 DS-CDMAS] BER 성능을 시뮬레이션하고 그 AWS 그
림 5.17과 5.18에 제시한다.

10°
ㅁ Number of users = 1
+ Number of users = 4
~ Number of users =7
“© AWGN theory
10"
S107                                           4
10°                                                                                            `“.                                          5
해
*
sé
«
1 0^                                                                                                         i       *                1
0                         5                       10                                                20                      25

15
E,/N, (dB)
를 28 5.17 AWGNOIA| MAIBAS 갖는 DSCDMAQY| BER 성능

293



===== PAGE 298 =====
Zy 최신 이동통신시스템

Mobile Communications using MATLAB Simulation

10°                        T           T
ㅁ Number of users =7
~© AWGN theory
10°
;
c,h
45 10°
10°
"3                                     15           20           25

E,/N, (dB)

를 그림 5.18 AWGNOA 직교 Gold AAHAS 갖는 DS-CDMAQY| BER 성능

\시퀸스에서, 동기 지점에서 상호-상관 RL 0이 아니다. 그래서 이 0이 아닌 상관
이 다른 사용자에게 간섭이 된다. 결과적으로, 사용자의 수가 늘어날수록 BERS 저하
된다.

반대로, 직교 Gold 시퀸스에서는 동기 지점에서 사용자간의 상호-상관 WL 0이다.
이는 사용자의 수가 늘어남에 따라 88 의 Zo] 이론적인 값에 근접함을 의미한다.

5.5.2 레일리 환경에서의 BER 성능

레일리 환경에서 동기식 28-2284ㅅ의 BER 성능을 그림 5.19와 5.20에 보였다. M-
시퀸스에서, 사용자의 수가 증가함에 따라 BERS] 저하한다. 이는 코드간의 상호상관
값이 0이 아니고 이것이 간섭이 되기 때문이다. 반면, 직교 Gold 시퀸스에서는, 동기 지
점에서 BES 직교성이 상호상관을 유지한다. 이 결과, 사용자의 수가 증가함에 따라,
BERS 이론치에 근접한다.

294



===== PAGE 299 =====
코드분할다중접속 (6044) 기. Oe

Tt      ㅜㅠ      ㅜㅠ
3

10"              |]            | |            | |            | |

ㅁ Number of users=1
~ Number of users = 4
~ Number of users =7
~® AWGN theory

10

BER

시              2          4          6          8         10        12
E/N, (dB)

를 그림 5.19 레일리 HOS 환경에서 MAJBAS 갖는 DSCOMAY BER 성능

T      tT     58
:

10°            T         =           T
-42- Number of users =7
~@- AWGN theory

BER

8     10    12    14    16    18    20
E,/N, (dB)

ok

16“
Ce ae

를 그림 5.20 레일리 페이딩 환경에서 직교 Gold ABAS 갖는 DSCDMAY BER 성능
295



===== PAGE 300 =====
a

최신 이동통신시스템

Mobile Communications using MATLAB Simulation

| z=

296

이 장에서는 CDMA 시스템의 AS 능력을 평가하기 위해 ASS = B 가지 방법에
대해 논하였으며, 기본적인 0284에 대한 설명이 기술되었다. 또한 대역확산통신용
코드시퀸스로 잘 알려진 세 가지 코드 시퀸스를 소개하고 콜*특성을 분석하였다. 동기
식 DS-CDMA] BER 성능이 컴퓨터 시뮬레이션을 통해 평가되었다. 이 장을 사용해,
독자는 자신만의 코드 A) AAU DS-CDMA 시스템을 디자인할 수 있는 SAS 갖출 수
있게 될 것이다. COMA 제 3세대, 4세대 이동통신 시스템에서의 가장 중요한 시스템
중 하나이다. 저자는 이들 새로운 시스템을 이 장에서 소개한 프로그램을 활용하여 평
가할 수 있을 것으로 기대한다.



===== PAGE 301 =====
코드분할다중접속(6044) 기법 FORT

1) Prasad, R., CDMA for Wireless Personal Communications, Norwood, MA: Artech House,
1996.

2) Special issue on spread-spectrum communication, IEEE Trans. Commun., Vol.COM-30, May
1982.

3) Simon, M. K., et al., “Spread-Spectrum Communications,” Vol.1,ILIII, Comp. Sci., 1985.

4) Scholtz, R. A., “The Spread-Spectrum Concept,” IEEE Trans. Commun., Vol.COM-25, August
1977, pp.748-755.

5) Torrieri, D. J., Principles of Secure Communication Systems, Norwood, MA: Artech House,
1992.

6) Cooper, G. R., and C. D. McGillem, Modern Communication and Spread-Spectrum, New York:
McGraw-Hill, 1986.

7) Glisic, 5. G., and P. A. Leppanen (eds.), Code Division Multiple Access Communications,
Norwell, MA: Kluwer Academic Publishers, 1995.

8) Viterbi, A. J., CDMA Principles of Spread-Spectrum Communications, Reading, MA: Addison-
Wesley, 1995.

9) Dixon, R. C., Spread-Spectrum Systems, New York: John Wiley & Sons, 1984.

10) Viterbi, A. M., and J. Viterbi, “Erlang Capacity of a Power-Controlled CDMA System,” IEEE J.
Selected Areas in Comm., Vol.11, August 1993, pp.892-899.

11) Prasad, R., Universal Wireless Personal Communications, Norwood, MA: Artech House, 1996.
12) Golomb, S. W., Shift Register Sequences, San Francisco, CA: Holden-Day, 1967.

13) Gold, R., “Optimal Binary Sequences for Spread Spectrum Multiplexing,” IEEE Trans. Inf.
Theory, Vol.IT-13, October 1967, pp.619-621.

297


===== PAGE 302 =====
최신 이동통신시스템

298

Mobile Communications using MATLAB Simulation

부록 5ㅅ

프로그램 5.1

Program 5-1
autocorr.m

Autocorrelation function of a sequence

00 00 00 00 00

00

Programmed by M.Okita and H.Harada

oe

function [out] = autocorr(indata, tn)

KKK KKK KK KKK KKK KKK KKK KKK KKK KK KK KKK KKK KKK KK KKK KKK KKK KKK KKK KKK KK KKK

indata : input sequence
tn     : number of period

out    : autocorrelation data
KKK KK KK KK KK KKK KK IKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKKKKKKKK

0 0 00 00 00

oe

tf Nargin:<. 2

tn =k;
end
ln = length (indata) ;
out = zeros(1,ln*tn);

for ii=0:l1n*tn-1
out (iit+l) = sum(indata.*shift (indata,ii,0));
end

LRKKKKKK KKK KKK KK KK KKK KKK End of file KKK KKK KK KKK KK KKK KKKKKKKKEK

프로그램 5.2

% Program 5-2

ole

crosscorr.m

oe

oe

Crosscorrelation function of a sequence

Programmed by M.Okita and H.Harada

00 00 00



===== PAGE 303 =====
Toe 0 |

function [out] = crosscorr(indatal, indata2, tn)

KKK KKK KKK KKK KK KKK KKK KKK KKK KKK KKK KKK KKKKKEKKEKKKKKKKKKKKKKKKKK

indatal : input sequencel
indata2 : input sequence2
tn      : number of period

out     : crosscorrelation data
KKKKKK KKK KKK KKK KKK Kh kkk kkk Kh KKK KKK KKK KKK KKK KK KKK KKK KKK KKK KKK KKK

00 00 00 00 00 00

if-nargin.< 3
tn ly

end
in = length(indatal) ;
out = zeros(1,1ln*tn);

for ii=-0 Sin*tn-1
out (iit+l) = sum(indatal.*shift (indata2,ii,0));
end

HK RR end of fite KAKKKKKKKKKKKK KKK KKK KK KK KK

프로그램 5.3
% Program 5-3
mseq.m

The generation function of Msequence
An example

%

%

%

%

%

%    stg     =
%    taps
%

%

%

%

%

PPR
SS

w

ae

|
NaS Ww

inidata
n    =

Programmed by M.Okita and H.Harada

function [mout] = mseq(stg, taps, inidata, n)

옹  KKKKKKKKKKK KKK KKK KK KK KK KKK KKK KK KK KR KKK KKK KKK KKK KKK KKK KKK 해 강행 가 고 가 가 나
% stg     : Number of stages
% taps    : Position of register feedback

inidata : Initial sequence

299


===== PAGE 304 =====
최신 이동통신시스템

300

Mobite Communications using MATLAB Simulation

Si       : Number of output sequence(It can be omitted)

% mout    : output M sequence
&  KKKKK KKK KKK KK KK KKK KR KKK KKK KK KK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK EK

if nargin < 4
n =-L;
end

mout = zeros(n,2“stq1);
fpos = zeros (stg,1);

fpos(taps) = 1;

for: ii=l:2*stgl

mout(1,ii) = inidata(stg) ;             % storage of the
% output data
num = mod(inidata*fpos, 2) ;            % calculation of the
% feedback data
inidata(2:stg) = inidata(1:stg1);             % one shifts the
% register
inidata (1)     = num;                         % return

% feedback data

end

afin sad
for ii=2:n

mout (3.3, ©)   shite (mout (Lil, 2) -1, 0
end

end

Sk RR KK KKK RK OK KK KK end of fie KKKEKKKKKKKKKKKKKKKKKKKKKK

프로그램 5.4

% Program 5-4
shift.m

oe

ole

Shift the contents of the register.

00 00

oe

Programmed by M.Okita and H.Harada

ae



===== PAGE 305 =====
function [outregi] = shift (inregi, shiftr, shiftu)

옹  *ㅠ*ㄴ*×ㅠ×ㄴㅠㄴㅠ×ㅠㄴㅠ×ㅠㅠㄴㅠ×ㅠ×ㅠㅠㄴ×ㅠㄴㅠㄴㅠㅠ*×ㅠㅠㄴㅠ×ㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㄴㅠㅠㄴㅠㄴㅠㄴㅠㅠ×ㅠ＊×ㅠㄴㅠㄴㅠ＊×ㅠ*ㅠ×ㅠ×ㅠㅠ×ㅠㅠㅠ×ㅠㅠㅠ×ㅠ×ㅠ×ㅠㅠㅠㅠ
% inrege     : Vector or matrix

% shiftr     : The amount of shift to the right.

% shiftu     : The amount of shift to the top.

% outregi    : Register output

&  KKKKK KKK KKK KKK KK KK KK KK KKK KK KK KKK KKK KKK KKK KKK KKK KK KK KKK KKK KKK KKEKK

[h, Vv)    size (inregi) ;
outregi = inregi;

shiftr
shiftu

rem(shiftr,v) ;
rem(shiftu,h) ;

if shiftr > 0

outregi(:,1       :shiftr) = inregi(:,vshiftrt+l:v       3

outregi(:,1+shiftr:v     ) = inregi(:,1         :v-shiftxr);
elseif shiftr < 0

outregi(:,1         :v+tshiftr) = inregi(:,l-shiftr:v      ee

outregi(:,vtshiftr+l:v       ) = inregi(:,1       pa cy ek. oh ay 24

end

inregi = outregi;

1£ shifttu >-0

outregi (1         :h-shiftu,:) = inregi(1l+shiftu:h,     3

outregi (hshiftutl:h,       :) = inregi(1       -Shiftai, <.):7
elseif shiftu < 0

outregi (1       :-shiftu,:) = inregi (h+shiftu+1:h,       ee

outregi (1l-shiftu:h,      :) = inregi(1l         93690 60, 2) 5

end

Zk KK RK RK KOK KKK kk kK kkk kK KK end Of Eile KKK KKKKKKKKKKKKK KK KK KKK

프로그램 5.5
% Program 5-5
goldseq.m

%
%
% The generation function of Gold sequence
%
%

Programmed by M.Okita and H.Harada

301



===== PAGE 306 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

function [gout] = goldseq(ml, m2, n)

KKK KKK KKK KKK KKK KKK KKK KK KK KKK KKK KK KKK KKK KKK KKK KKK KKKKKKKKKKKKK KKK

00 ol?

ml : Msequence 1

m2 : Msequence 2

n : Number of output sequence(It can be omitted)
gout : output Gold sequence

KKK KKK KKK KKK KKK KKK KK KKK KK KKK KK KKK KK KKK KK KKK KKK KKK KKKKK KK KKK KK KKK

00 00 00 00

Licnargin <-3
n-=-1;
end

gout = zeros(n,length (m1) ) /

for ii=l:n
gout (ii,:) = xor(ml,m2);
shift(m2,1,0);

m2
end

ZREKKKKKKKKKKKKKKKKKKKKKKKK ond of fite KKK KKKKKKKKKKKKKKKKKKKKKKK

프로그램 5.6

Program 5-6

00 00

oe

Simulation program to realize DS-CDMA system

00 00

dscdma.m

Programmed by M.Okita and H.Harada

00 00 00

Zk RR KK RR KK KK Preparation part KK KK KKK KKK KKKKKKKKKK KK KKK

sr   = 256000.0;               % symbol rate

ml   = 2;                      % number of modulation levels
br   = sri* mi?                % bit rate

nd   = 100;                    % number of symbol

ebn0O = 3;                      % Eb/No

LRRKKK KKK KKK KKK KKKKKKK Filter initialization KKKKKKKKKKKKKKKKKKKKK

Tein   = 21;                       % number of filter taps

302



===== PAGE 307 =====
IPOINT

alfs
[xh]

[xh2]

8;                       % number of oversample
057                     % roll off factor
hrollfcoef(irfn, IPOINT,sr,alfs,1);       % T FILTER
% FUNCTION
hrollfcoef (irfn, IPOINT,sr,alfs,0);       % R FILTER
% FUNCTION

EREKKKKKKKKKKKKKK Spreading code initialization KKK KKK KKK KKK KKK KKK

user
seq

stage
ptapl

ptap2 =

regil

regi2

L;
1;

37
[42] .7
10 17
Ll. 3 1]?

[3 bees oh

number of users
1:Msequence 2:Gold
3:Orthogonal Gold

number of stages

position of taps for lst
position of taps for 2nd
initial value of register
for ist

initial value of register
for 2nd

00 00 00 00 00 00 00 00 00 00

웅******×*××*×*×※××*××ㅠ Generation of the spreading code Ka K KK KKK KKK KK

switch seq

case

+

code

case

2

ml
m2
code

case
m
m.

i
1
2

code

end
code
clen

% Msequence

= mseq(stage,ptapl, regil, user);

% Gold sequence

= mseq(stage,ptapl, regil) ;
= mseq(stage,ptap2, 26012 ;
= goldseq(ml1,m2,user) ;

% Orthogonal Gold sequence

= mseq(stage,ptapl, regil) ;
= mseq(stage,ptap2, regi2) ;

ㅣ

2098 고 고 347
length (code) ;

[goldseq(m1,m2,user) , zeros (user,1) ];

Bk Rk kK ke kK Fading initialization! KaKKKKKKK KKK KKK KKK KK KK

rfade
itau
01711
7ㅁ0

= 0;

[0,8];
[0.0,40.0];
[6,7];

00 00 00

oe

Rayleigh fading O:nothing 1:consider
delay time

attenuation level

number of waves to generate fading

303


===== PAGE 308 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

thl    = [0.0,0.0];         % initial Phase of delayed wave

itndl = [3001,4004];       % set fading counter

nowl   = 2;                % number of directwave + delayed wave
tstp   = 2/ sr / LPOINT*/“clen?           % time resolution

fd     = 160;                              % doppler frequency [Hz]
flat   = 1;                 % flat Rayleigh environment

itndel = nd * IPOINT * clen * 30;          % number of fading

% counter to skip

ZK KK KKK KK KR KK KK KKK KK kK START CALCULATION **** RRR KKKKKKKKKKKKKK KKK

nloop = 1000;              % simulation number of times
noe   = 0;
nod   = 0;

for ii=1:nloop

ZRKKKKKKKKKKK KKK KKK KKK KK KKK  TrANSMLICter KEKKKKKKKKKKKKKKKKKKKKKKKK

data = rand(user,nd*ml) > 0.5;

[ich, qch] = qpskmod(data,user,nd,ml) ;       S QPSK
% modulation
{ichl,qch1] = spread (ich, qch, code) ;           % spreading
[ich2,qch2] = compoversamp2 (ich1,qch1, IPOINT) ;
% over sampling
[ich3,qch3] = compconv2 (ich2,qch2,xh) ;        % filter
if user == 1                                  % transmission

ich4 = ich3;

qch4 = qch3;
else

ich4

qch4
end

sum (Zens);

ㅣ

sum (00103) ;

SRK Kk RR RK KKK KR KK KK Fading Channel] * *® ® ® ® ® K K

if rfade ==
10685 = ich4;
qch5 = qch4;
else
[ich5,qch5]   =   sefade (ich4,qch4,itau,dlvll1,th1,n0,itndl,

nowl, length(ich4),tstp, fd, flat) ;

304



===== PAGE 309 =====
Toe 를

% fading channel
itndl = itndl + itndel;
end

Bw KKK KR KR RK KR KK RK KK eK  Receiver  KKRKKK KKK KKK KKK KK KKK KKK KKK KKK

spow = sum(rot90(ich3.%2 + gch3.*2))-/| nd;
% attenuation Calculation
attn = sqrt(0.5 * spow * sr / br * 10“K-ebn0/10));

[ich6,qch6] = comb2 (ich5,qch5,attn) ;

% Add White Gaussian Noise (AWGN)
[ich7,qch7] = compconv2 (ich6, qch6, xh2) ;
% filter

sampl = irfn-* LEOINT + 그;
ich8    ich7 (:,sampl:IPOINT: IPOINT*nd*clen+sampl1-1) ;
qch8    qch7 (:, Samp1: IPOINT: IPOINT*nd*clen+samp1-1) ;

ㅣ

[10029 qch9] = despread(ich8,qch8, code) ;
% despreading

demodata = qpskdemod(ich9,qch9,user,nd,ml) ;
% QPSK demodulation

ZRKK KKK KK KKK KKK KK KEK K Bit Error Rate (BER) KKK KKKEKKKKKKKKKKKKKKKK

noe2 = sum(sum(abs (data-demodata) ) );
nod2 = user * nd * ml;

noe = noe + noe2;

nod = nod + nod2;

fprintf ('sd\t%e\n',ii,noe2/nod2) ;

end

Zw KK KR KR RK RK KR KK RK KK kk RK Data EL LO KERR KKK KKK KKK KK KKK KK KKK KK KK

ber = noe / nod;
fprintf ('Sd\t%d\t%d\t%e\n',ebn0, noe, nod, noe/nod) ;
% fprintf: built:in function
fid = fopen('BER.dat','a');
fprintf (fid, 'td\t%e\ts£\ts£\t\n',ebn0, noe/nod, noe, nod) ;

305



===== PAGE 310 =====
최신 이동통신시스템

306

Mobile Communications using MATLAB Simulation

% fprintf: built in function
fclose (fid) ;

Dok KR KK KKK KK RK RK RK RK KK end of file KKK KK KK KKK KKK KKKKKKKKKKKKK

프로그램 5.7

% Program 5-7
spread.m

00

00 ol?

Data spread function

Programmed by M.Okita and H.Harada

00 00 00

function [iout, qout] = spread(idata, qdata, codel)

옹  KKK KKK KK KKK KK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KKK KK KK KK KKK

%   idata   : ich data sequcence

%   qdata   : qch data sequcence

%   iout    : ich output data sequence
%   gout    : qch output data sequence
%   codel    : spread code sequence

%

KOK KK KK KK KI KKK KK KK KK KKK KK KKK KK KK KKK KKK KKK KKK KKK KKK KK KK KKK

switch nargin
ease {-0. ¢21 }
error('lack of input argument');

case 2
codel = qdata;
qdata = idata;
end
{hn,vn] = size(idata);
{he,vc] = size(codel) ;
Li shne >: he
error('lack of spread code sequences') ;
end

iout = zeros (hn,vn*vc) ;
gout = zeros (hn,vn*vc) ;
for ii=1:hn
iout(ii,:) = reshape (rot90 (00061 (ii, : ) , 3) *idata(ii,:),1,vn*vc);



===== PAGE 311 =====
gout (ii,:) = reshape (rot90(codel (ii, :),3)*qdata(ii,:),1,vn*vc);

end

BRK RK RK RR RR RK RK RK RK end of File KERR KKKKKHKKKKKKKKKKKKKKKKKK

프로그램 5.8

% Program

function [iout, gout] = despread(idata, qdata, codel)

a= 8

despread.m
Data despread function

Programmed by M.Okita and H.Harada

KR KKK KKK KKK KK KKK KEK KK KKK KKK KKK KEK KKK KKK KK KE KKKKKKKKK KKK KKK KKK KK KKK

%

%   idata
%   qdata
%   iout
%   qout
%   codel
%

ich data sequcence

qch data sequcence

ich output data sequence

gqch output data sequence
spread code sequence

KKK KKK KKK KKK KEK KKK KKK KK KKK KK KKK KKK KKK KKK KKK KKK KEK KKK KK KK KKK KKK KK

switch nargin

case {0 ,

ie}

error('lack of input argument');

case 2
codel
qdata

end

{hn,vn] =
{he,vc] =

vn   =

iout    =
qout    =

= qdata;
idata;

size(idata);
size (00061) ;

fix (vn/vc);

zeros (hc,vn) ;
zeros (hc, vn);

for ii=l:he
lout (ii,:) = rot90(flipud(rot90 (reshape (idata

(11.

), ve, vn) ) ) *rot90(codeél (그초, ; ) , 3) ) >

307



===== PAGE 312 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

gout (ii,:) = rot90(flipud(rot90 (reshape
(qdata(ii,:))vc, vn).)) *£6t90 (codel (Zi, :).,3))?
end

ZRKKKKK KKK KK KKK KKK KK KKK KKK end of file KKRKKKKKKKKKEKKKKKKK KKK KKK KEK

프로그램 5.9
Program 5-9
compoversamp2.m

oe

Function to sample "sample" time

programmed by H.Harada and M.Okita

de 00000

function [iout,qout] = compoversamp2 (iin, qin, sample)

%  KKK KKK KKK KKK KKK KK KKK KKKKK KK KKK KKK KKK KK KKK KKK KKK KK KK KKK KKK KKK
% iin     : input Ich sequence

% qin     : input Qch sequence

% iout    : ich output data sequence

% qout    : qch output data sequence

%
%

sample : Number of oversamples
KR KKK KKK KKK KKK KK KKK KK KKK KKK KK KKK KEK KKK KKK KEK KKKKKKEKKEKKKKKKKKKKEK

[h,v] = size(iin);

iout = zeros(h,v*sample) ;

qout = zeros(h,v*sample) ;
iout(:,1:sample:1+sample*(v-1)) = iin;
qout (:,1:sample:1+sample*(v-1)) = gin;

ZR KK KR KR KKK KKK RK RK KK RK KK RK KE end of file KKK KKK KKK KKK KKK KK KK KKK KKK

프로그램 5.10

% Program 5-10
compconv2.m

%
%
% Function to perform convolution between signal and filter
%
% Programmed by H.Harada and M.Okita

%

308



===== PAGE 313 =====
부루 ^ 를

function [iout, qout] = compconv2(idata, qdata, filter)

&  KKK KKK KK KKK KK KKK KK KKK KKK KKK KKK KKK KKK KKK KK KKKK KKK KKK KK KKK KKK KKK KEK
%   idata   : ich data sequcence

%   qdata   : qch data sequcence

%   iout    : ich output data sequence

%   gout    : qch output data sequence

%   filter : filter tap coefficience

x  KKK KKK KKK KKK KKK KK KKK KKK KK KKK KKK KKK KKK KKKKKKKKKKKKKKK KKK KKK KKK KK
iout = conv2(idata, filter) ;

qout = conv2 (qdata, filter) ;

ZK KKK KK KKK KK RK KK RK KK KKK KK end of fite KKKKKKKKKKKK KKK KKK KKK KK KKK

프로그램 5.11
% Program 5-11
% comb2.m
%
% Function to add white gaussian noise
%
% Programmed by H.Harada and M.Okita
%

function [iout, qout] = comb2(idata, qdata, attn)

BRK KKK KK KKK KKK RK KR KK  variables  KKK KKK KKK KKKKK KKK KK KK KKK
% idata : input Ich data

% qdata : input Qch data

% iout   output Ich data

% qout   output Qch data

% attn : attenuation level caused by Eb/No or C/N

%

KKK KKK KKK KK KK KKK KKK KKK KKK KKK KKK KKK KKKKKKKKKEKKKKK KKK KKK

v = length (idata) ;

h = length (attn) ;
iout = zeros(h,v);
gout = zeros (h,v);

for ii=l:h
iout (ii,:) = idata + randn(1,v) * attn(ili);
qout (ii,.:)   qdata +“randn(1,v) .* 3ㅎㄴ5ㅁ1320) >
end

i

ZRKKKKKKKKKKKKKKKKKKKKKKKKK and o£ File KKKKKKKK KKK KKK KKK KK KK KK KK

309


===== PAGE 314 =====
a
.

(Multiple Access .
Protocols)



===== PAGE 315 =====
다중접속 프로토콜
(Multiple Access Protocols)

| 6.1 |S

통신 수단에 있어서의 사용자들 간의 Yo] S 규약(프로토콜: #0[0001)이라 한다. At
용자들이 공통된 통신 수단을 사용할 때 다중접속이라 부른다. 그래서 다중접속 프로토
콜은 공통된 매체를 통해 정보의 성공적인 전송을 위한 사용자 간의 합의와 규칙의 집
합이라정의한다. 하나 이상의 독립적인 사용자가 공통된 자원을 사용하거나 접속하면
다중접속 프로토콜이 필요하다. 이런 프로토콜이 존재하지 않으면, 하나 이상의 사용
자가 동시에 자원에 접속을 시도할 때 충돌이 발생한다. 그래서 다중접속 프로토콜은
이러한 SSS 퍼하거나 최소한으로 해결할 수 있어야 한다. 이런 이유로, GSAS 기
Se 네트워크내에 분산된 단말기들 사이에서 제한된 공통 전송 자원을 공유하는 함수
로 정의된다.

이 장에서 논의된 다중접속 프로토콜은 제한된 자원을 공유해야만 하는 통신채널을
이용해서 송수신하는 통신 시스템에서 필수적으로 사용되는 것들이다[1-27]. 이 경우,
자원을 공유해야하는 주된 이유는 송수신기간의 BS (connectivity) S 원활하게 하며,
부족한 자원을 효율적으로 사용하기 위함이다[1]. 모든 사용자에 대해 접속지점에서
공통의 MAS 사용하면, 점-대-점 (0010『10?0100 렁크를 구성하는 네트워크가 존재하

313



===== PAGE 316 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

지만 이들 Ba 중 하나는 동시에 많은 사용자에 의해 공유된다. 그래서 다중화
(multiplexing) 기법이 필요하다. 다중화는 동일한 물리 링크를 통해 다른 정보를 전송
하는 것이다. 표 6.1은 다중접속과 다중화의 차이점을 보여준다.

끄로토콜의 설계는 일발적으로 특정 목표 (환경)를 염두에 두고 행해지고 프로토
의 특성은 설계 목표에 의해 결정된다. 그러나 환경-특수성을 배제하면 좋은 다중접속
프로토콜이 가져야하는 특성들을 다음과 같이 정리할 수 있다:

ru

HE 6.18 다중접속과 다중화의 차이점

다중접속                                            다중화
자원                네크워크                                                    링크
단말기 연결성 | 행렬                                                          점-대(다)점
스위칭 가동 | -7Fe{S3)                                                        #7OSI<2)
(OSI: open systems interconnection)
토폴로지           버스                                                         경로(들)
별
링
나무
제어                   중앙 ee                                                             단말거

0 다중접속 프로토콜의 첫 번째 그리고 가장 중요한 임무는 시스템 내 다수의 사용
자 간에 공통된 전송채널을 공유하는 것이다. 이를 위해, 프로토콜은 사용자들이
특정 TAS 따름으로써 채널에 접속하는 방법을 제어해야 한다. 프로토콜은 A}
용자에게 채널 수용능력의 할당을 제어한다.

@ 프로토콜은 전송 매체가 효과적으로 사용될 수 있도록 할당되어야 한다. 효율은
일반적으로 채널 전송률(470480040과 전송 지연으로 측정된다.

@ 할당은 각 사용자에게 동등해야 한다. 즉, 특정 사용자에게 우선권
로써 각 사용자는 (평균적으로) 동일한 할당을 받아야 한다.

@)프로토콜은 다른 유형의 트래픽 (예: 음성과 데이터)에 융통성을 가져야 한다.

© 프로토콜은 안정적이어야 한다. 이는 시스템이 평형(64041160ㅁ0400) 상태에 있을 때,

tho
2

314


===== PAGE 317 =====
다중접속 neces EO

부하가 증가하면 시스템이 다른 평형점으로 이동해야함을 의미한다. 불안정한 =
로토콜은 부하가 증가하면 시스템이 높은 부하로 표류하고 낮은 전송률을 갖게
한다.
© 프로토콜은 기기 오류와 조건의 변화에 강건해야 한다. 만약 한 사용자가 제대로
운용하지 못할 때 , 이를 나머지 시스템에 가능한 적은 영향을 미쳐야 한다.
이 장은 무선이동 환경에 중점을 둔다. 이런 환경에서는, 프로토콜의 몇몇 특
중할 수 있는데, 특히 조건 변화에 대한 강건성에 집중할 수 있다. 무선이동 환
프로도콜은'다음을 다를 수있어야 환다:

특성에 집

0 숨은 단말기 문제 [두 단말기가 ultra high frequency(UHF) 신호에 불투명한 언
덕, 건물 혹은 다른 물리적 장벽으로 인해 숨겨졌으나 중심 혹은 기지국 영역 내
에 존재];

@ 근원 (nearfar) 효과 (원거리 사용자의 전송이 근거리 사용자의 전송보다 크게
감쇄);

@ 무선채널에서 나타나는 다중경로 페이딩과 새도윙 효과;

@이웃한 ANA 동일한 주파수의 사용으로 인해 야기되는 셀룰라 무선시스템의 동
일채널 간섭 효과

위에서 언급한 많은 프로토콜의 특성은 서로 상충하고 프로토콜의 설계과정에서 타
협이 이루어져야 한다. 타협은 프로토콜의 환경과 특정 사용에 의해 결정된다.

이 장은 무선통신의 몇 가지 전형적인 프로토콜과 컴퓨터 시뮬레이션을 통해 그들의
성능을 평가하는 방법을 소개한다.

이 장은 다음과 같이 구성되었다. 6.2장은 다중접속 프로토콜의 분류에 대해 제시한
다. 몇 가지 랜덤 접속 프로토콜은 6.3장에서 소개한다. 컴퓨터 시뮬레이션의 BBA
조건은 6.4장에 보였다. 6.5-6.8장에서는, 순수 ALOHA(pure ALOHA), 슬롯화 된
ALOHA(slotted ALOHA), 비영속적 CSMA(nonpersistent CSMA), 슬롯화된 비영속
Al ISMA(slotted nonpersistent ISMA)2] 구성과 컴퓨터 시뮬레이션 방법을 소개한다.

315



===== PAGE 318 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

전송률과 전송지연 특성에 대해서도 논의한다. 이 장에 관련된 모든 프로그램은 부록
6C2} 0ㅁ20)4에서 얻을 수 있다.

6.2 | 다중접속 프로토콜의 분류

1970년 (이 장에서 후에 논의될) ALOHA 프로토콜을 시작으로, 많은 다중접속 프로
토콜이 개발되어 왔다. 이들 프로토콜을 분류하는 많은 HHO] 제시되어 Ae [14,16].
이 책에서는 다중접속 프로토콜을 세 가지 주 그룹으로 나눈다(그림 6.1): 비경합 프
토콜, 경합 프로토콜, CDMA 프로토콜.

Multiple access protocols
Contentionless                                                   Contention
(scheduling)                                                      (random access)
CDMA
ors,
Fixed               Demand PureCDMA Hybrid CDMA Repeated       Random
assigned          assigned DS,FH,TH DS/FH             random          access with
|                       TDMA/CDMA access          reservation
FDOMA               Polling token                                         ALOHA,                    Implicit
TDMA            passing                                       s-ALOHA              Explicit

를 그림 61 다중접속 프로토콜의 분류

비경합(혹은 스케줄링) 프로토콜은 사용자의 ASS 스케줄링하여 동시에 두 명 이
상의 사용자가 채널에 접속하는 상황을 피한다. 이는 각 사용자가 전송 수용능력의 부
분에 할당되는 고정된 형태나 전송할 사용자 사이에서만 스케줄링이 발생하는 요청-할
당 형태로 행해진다.
경합(혹은 랜덤접속) 프로토콜에서, 사용자는 다른 사용자가 동시에 전송할 수 있기
316



===== PAGE 319 =====
때문에 충돌이 없을 것이라고 확신할 수 없다. 그래서 이 프로토콜은 충돌이 발생했을
때에 이를 해결하기 위한 다른 방법이 필요하다.

CDMA 프로토콜은 비경합과 경합 어디에도 속하지 않는다. 5장에서 AY sl 바와 같
이, CDMA 두 그룹 사이에 해당한다. 원리적으로, 이것은 다수의 사용자가 동시에 충
돌 없이 전송할 수 있는 비경합 프로토콜이다. 그러나 동시에 전송하는 사용자의 수가
문턱치를 초과하면 경합이 일어난다.

경합 프로토콜은 다시 반복적인 랜덤 프로토콜과 예약 랜덤 프로토콜로 ua 후자
에서, 사용자의 초기 ASS 채널에 접속하기 위해 랜덤-접속을 사용한다. 그러나 일단
채널에 접속하면, 사용자의 전송은 더 이상 전송이 없을 때까지 스케줄링 된다. 프로토
콜의 두 가지 주요 형태는 내시적 예약과 명시적 예약이다. 명시적 예약 프로토콜은 스
케줄링된 시간에 ASS 요청하기 위해 짧은 예약 패킷을 사용한다. 내시적 예약 프로
EBS 예약 패킷의 사용 없이 설계된다.

CDMA 프로토콜은 순수(0426) CDMA $} 49 (hybrid) 010)4ㅅ로 분류된다. 다른 그
룹을 이루는 CDMAS} 비경합과 경합 프로토콜의 하위그룹을 포함해 6개의 부문으로
끝마친다.

6.2.1 비경합 (스케줄링) 다중접속 프로토콜

비경합 다중접속 프로토콜은 모든 사용자의 ASS 스케줄링 함으로써 다수의 사용
자가 동시에 같은 채널에 접속을 시도하는 것을 막는다. 사용자는 스케줄링된 순서대로

ASS 시도해 모든 전송이 성공하도록 한다. 스케줄링은 두 가지 형태를 갖는다:

(1) 고정-할당 스케줄링: 이 VAS] 프로토콜에서, 사용 가능한 채널의 수용능력은 각
사용자의 활동에 관계없이 수용능력의 고정된 부분을 할당받도록 Hdd. 분할은
시간이나 주파수에서 행해전다. 시간 분할은 전송시간이 프레임으로 나뉘고 각
사용자는 각 프레임의 부분을 할당받아 다른 사용자와 중첩되지 않는 TDMA =
로토콜을 가져온다. TOMAS 그럼 6.2(8)에 보였다. 주파수 분할은 채널의 대역
폭이 중첩하지 않는 주파수 대역으로 나뉘고 각 사용자는 고정된 대역을 할당받

317



===== PAGE 320 =====
골 최신 이동통신시스템
Mobite Communications using MATLAB Simulation

는 주파수 분할 SAS (FDMA) 프로토콜을 가져온다. 14 6.2(b)= FPOMAS
보여준다.

@ 요청-할당 스케줄링:사용자는 활동(전송할 것이 있는 경우)하는경우에만허용된
다. 그래서 활동 (준비)하는 사용자는 스케줄링 된 순서대로 전송한다. 요청-할당
스케줄링에서, 집중(6600ㅁ81120) a 와 #AKdistributed) 제어를 구분한다. 집중

제어에서는, 단일 존재가 ASS 스케줄링 한다. 이런 프로토콜의 o]= rolkcall
701178 프로토콜이 있다. 분산 제어에서, 모든 사용자는 스케줄링 과정에 포함되
고 이런 프로토콜은 (06607ㅠ888108 프로토콜이다.

-
아

(a)                                                             (b)

를 그림 6.2 (a) TDMA (b) FDMA

6.2.2 경합 (랜덤) 다중접속 프로토콜

경합 다중접속에서는 전송 스케줄링이 존재하지 않는다. 이는 전송할 준비가 되어있
는 사용자가 언제 다른 사용자 ASS] 간섭 없이 전송할 수 있는  a 대한 정보가 없음
을 의미한다. 사용자는 (채널을 감지하여) 진행 중인 전송에 대해 SFE 그렇지 않을
수도 있으나 다른 준비된 사용자에 대한 정보는 없다: 그래서 다수의 사용자가 동시에
전송을 시작하면 모두 실패할 수 있다. 이런 전송 실패 가능성은 성공적인 전송을 다소
확률적으로 만든다. 랜덤 접속 프로토콜은 다수의 사용자가 동시에 Asa 발생하는경
합을 해결해야 한다.

우리는 경합 다중접속을 두 그룹으로 분류하는데, 반복 랜덤 접속 프로토콜[예: 순

4

318



===== PAGE 321 =====
다중접속 cece 《0료

(py ALOHA, 슬롯화된 (s}ALOHA, CSMA, ISMA 프로토콜]과 예약 랜덤 접속 프로
토콜[예: 예약 ALOHA (rALOHA), 패킷 예약 다중접속 프로토콜(8#\44ㅅ)]이 그것이
다. 전자에서, 사용자가 만드는 모든 전송은 위에서 언급되었다. 모든 전송에서 경합의
가능성이 존재한다. 후자에서는, 사용자는 단지 Al 번째 전송에서 다른 사용자와 충돌
을 피하는 방법을 모른다. 그러나 일단 사용자가 채널에 접속하면 그 사용자의 향후의
전송은 경합이 일어나지 않도록 순서대로 스케줄링 된다. 그래서 성공적인 전송 후에,
채널의 수용능력의 부분이 다른 사용자에게 할당되고 다른 사용자들은 그 수용능력의
사용을 자제하게 된다. 사용자는 전송할 게 없으면 할당된 수용능력을 잃게 된다.

| 런덤 접속 프로토콜

패킷비를 사용하는 SV 위치한 기지국을 갖는 이동단말기 HIS 고려할 수 있다.
랜덤 접속 패킷 통신으로 가장 잘 알려진 방법인 ALOHA [2]는 패킷들의 충돌 문제가
있다. CSMA 프로토콜[3,4]은 높은 수용능력을 제공하지만 그 성능은 “숨겨진 단말기”
문제에 의해 영향 받는다. 중앙 기지국이 이동 단말기로부터의 패킷 SSS 제어하는
세 번째 부분 (ISMA) [5-11]은 데이터 패킷과 숨겨진 단말기의 두 가지 문제의 충돌을
감소시킨다.

억제(2001610 지연 4] (fraction) [5-11]는 ISMAS 사용하는 패킷 통신 시스템의 설계
에 중요한 인자이고 상행 다중접속 채널 (단말기에서 기지국으로)이 이미 사용되고 있
을 때 하행-신호 채널 (기지국에서 단말기로)을 전파함으로써 다른 이동 패킷 전송을 억
제하는데 필요한 패킷의 지속시간의 비로 정의된다.

1884ㅅ는 두 가지 하위 계층으로 분류할 수 있다: 비영속적 19844 프로토콜과 py
AISMA 프로토콜.

이 프로토콜은 완전히 충돌을 피할 수 있을 것으로 보인다; 그러나 두 사용자 간의 전

319



===== PAGE 322 =====
최신 이동통신시스템

320

Mobile Communications using MATLAB Simufation

지연 때문에, 사용자는 다른 ASO] 이미 진행 중일 때 상향 채널이 비어 있다고 간주하
고 전송을 시작할 수 있다.
사용자는 수신국에서의 인지카 없으면 충돌이 SSS 알 수 있
데로 패킷은 후에 임의로 선택된 시간에 전송을 위해 다시 스케줄링 된다.
영속적 프로토콜의 특별한 경우가 1-영속적 ISMA 프로토콜이다. 프로토콜은 사용
자가 상향 채널이 사용되고 있음을 알고 있는 HS 제외하고는 비영속적 19544 프로토
콜과 동일하다. 이 경우, ASE 임의로 선택된 시간에 재스케줄링 되지 않는다. 대신, 사
용자는 채널이 사용되지 않을 때까지 채널을 감시하고 그 후에 즉시 패킷을 전송한다.
결과적으로, 채널이 사용되는 동안 준비된 모든 사용자는 채널이 사용되지 않게 되자
마자 전송할 것이고 이는 성공적인 전송 끝에 충돌의 발생 가 한다.
채널이 사용되는 동안 축적된 패킷의 충돌을 피하기 위해, 축적된 패킷의 전송의 시
작을 랜덤화할 수 있다. 이는 채널이 사용되는 동안 패킷을 생성한 모든 사용자가 채널
이 사용되지 않게 되는 순간 확률 로 전송하도록 함으로써 이루       률
ASS :초( ;는 시스템의 두 사용자간의 최대 전송 지연) 연기할 것이다. :초 후에,

=
ea
운
후
ny

1
>
{a

연기된 단말기는 채널을 다시 감지하고 이전과 동일한 알고리즘을 적용한다.
이 영속적 ISMA 프로토콜로, 채널이 비어 있는 경우 한명 이상의 준비된 사용자가

전송할 FSS 작은 값의 /를 사용하여 아주 작게 만들 수 있다.

비영속적과 ㅠ영속적 ISMA 프로토콜에서, 사용자는 모든 패킷이 ASA 후에 충돌
에 대해 알게 된다. 이 이유는 모든 패킷이 도착한 후에 수신자에게 인지 신호가 보내지
기 때문이다. 충돌이 단지 AS] 시작된 후 전송 지연 내에 발생할 수 있으므로 이 ae
동안 충돌이 발생하면 더 이상의 HAS 보내는 것은 시간 낭비이다. 이런 이유로, 충
을 검출하는 ISMA (ISMACD) 프로토콜이 개발되어 왔다.  = 프로토콜에서, he
자는 전송하는 동안 ABS AS 감시한다. SSS 검출하면, ASS 가능한 빨리 멈춰



===== PAGE 323 =====
다중접속 프로토 FO

EM 컴퓨터 시물레이션에서의 보편적 조건

6.4.1 패킷 통신 시스템의 모델링

이 장에서는 정확하고 효과적인 컴퓨터 시뮬레이션을 행할 때 사용하는 보편적?
정에 대해 정리한다.

re
fe,

(1) 패킷 통신 시스템의 전체 구성
시뮬레이션된 moe 시스템의 구성으로, 그림 6.3에 보인 바와 같이 각 사용자 단

말기는 접속 프로토콜을 사용하여 접속지점에 접속한다.
User terminal 1                                   Packet
transmission
Packet   Arrival        Access |__|
—_——18
generation          fer protocol

User terminal 2

Access

> Buffer | protocol al            Access point
> Access        | A
Buffer
rotocol        cha
User terminal 3         |                                 "

>| Buffer   Access

protocol

User terminal 4

Access
protocol

여여

Communication
channel

를 그림 63 패킷 통신 시스템의 구성

321



===== PAGE 324 =====
최신 이동통신시스템

a

322

Mobile Communications using MATLAB Simulation

(2) 접속단말기

각 사용자 단말기의 성능은 동일하다. 게다가, 각 단말기는 버퍼를 가지고 있다. ZA}
용자 단말기가 전송 HAS 생성할 때 패킷은 버퍼에 저장된다. 그 다음, 저장된 패킷은
버퍼에서 나오는 순서에 따라 전송된다. 즉, YS] firstin and first-out (FIFO) 버퍼이
다. 버퍼회로는 두 가지 유형으로 분류할 수 있다: 무한 메모리를 갖는 버퍼와 유한 메모
리를 갖는 버퍼. 유한 메모리를 사용하는 경우 메모리가 다 차면 사용자 단말기의 패킷
생성이 중단된다. 이를 “콜 차단” (call blocking)°] 2} 한다. 또한, 접속단말기의 수가 제
한되어 있지 않으면, 이런 Bas 무한 콜-자원 (631ㅎ04706) 모델이라 부른다. 반면, 접
속단말기의 수가 제한되는 경우 이를 유한 SAW) 모델이라 부른다. 이론적인 분석에
서, 우리는 때때로 유한 콜-자원 모델을 가정한다.

(3) 통신채널
유선과 무선통신 시스템의 일반적인 차이는 통신채널의 모델링에 있다. 통신채널의
모델링은 다음과 같이 모델링 되어진다.

O 유선통신 시스템에서는 전송 오류가 발생하지 않고 접속지점에서 사용자 단말기
로부터의 신호 파워는 동일하다. 이는 접속 프로토콜을 평가하는데 있어서 가장

 무선통신 시스템에서, 통신채널의 질은 시변한다. 이 장에서, 접속단말기와 접속
지점 사이의 거리와 새도윙에 의해 결정되고 그 사이의 장애물에 의해 야기되는
전송손실이 고려된다. 전송손실과 새도윙은 다음과 같이 모델링 된다:

ㆍ전송손실: 접속지점과 접속단말기 사이의 거리가 증가할수록 수신-가워는

PHU. 이를 전송손실임라 부르고 7-“에'비례하여 Ashes) ves

ch

2에서 52] 값을 갖는다 [28].
MEQ: 전송무선신호는 반사와 회절과 같은 현상에 의해 다수의 경로를 거친
다수의 무선파로 수신된다. 수신파위는 다수의 무선파를 수신함으로써 심하



===== PAGE 325 =====
다중접속 cece FO

게 변동한다. 수십 개 파장에 거친 페이덩의 메디안 RS 작은 스케일에서의
메디안 값이라 부른다. 수십 개의 작은 스케일에 거친 작은 스케일에서의 메디
안 값의 메디안 a 또한 장애물에 의해 변동하고 새도윙이라 불린다. 이 변동
은 표준편차 67 08를 RE 로그 정규 분포를 취함이 알려져 있다.

(4) 패킷 생성
각 접속단말기는 랜덤하고 서로 무관하게 패킷을 생성한다고 가정한다. 그런 패킷 생
성을 2016500 분포라 한다. 다음은 01880 분포의 특성이다.

(1) 독립: Hale] AVS 과거 생성과 독립적이다.

@ 불변성: 패킷의 확률은 시뮬레이션의 각 시간슬롯에서 변화하지 않는다.

(9 FAS: 매우 작은 기간 동안, 두개 이상의 패킷이 생성될 확률은 무시된다. 또한,
생성된 패킷의 7} Poisson 분포를 따르면 패킷이 생성되는 주기는 지수 분포를

따른다.

No collision           Collision occurs        Collision occurs
in whole packet         in some parts of the packet

를 그림 6.4 전송 WAI 충돌

323



===== PAGE 326 =====
최신 이동통신시스템

ray

324

Mobile Communications using MATLAB Simufation

에 의존한다. 그래서 다수의 패킷이 충돌해도 가장 큰 수신 파워를 가진 패킷은 때
로 존속된다. 일반적으로, 이 효과를 캡쳐 효과라 부른다. 반면, 충돌이 발생하지
않아도 통신채널이 나빠서 점속지점에서 수신 파위가 요구되는 파워보다작은 경
우 패킷 전송 오류가 발생한다.

실제 통신 시스템에서, 접속지점이 접속단말기에서 생성된 패킷이 성공적으로 전송
될지 여부를 결정하고 결정의 결과가 접속단말기에 전송된다. 또한, MAAS 오류가
발생하면, 패킷은 접속지점에 약간의 간격 후에 전송된다.

(6) 제공된 트래픽

이 장에서, 접속단말기에서 시간 간격동안 새롭게 생성된 패킷과 재전송된 패킷을 포
함한 패킷의 총 양을 제공된 트래픽이라 부르고 전송 데이터 레이트에 의해 정규화된
제공 트래픽을 (로 쓴다. 전송 데이터 레이트가 (529)이고 T, 610가 전송에 필요
하다면 (는 다음과 같다:

(6.1)
패킷이 생성되지 않으면 G=(o]ch.
(7) 전송률 (throughput)

ES 패킷의 정보량이 Kbps) Tit)! 정의되고 시간단위당 n 패킷이 성공적으로
전송되었다면 Sess} 같다:

R                                                    (6.2)



===== PAGE 327 =====
전송 패킷이 생성되지 않고 모든 전송 패킷이 충돌에 의해 파괴되면 SE 최소값 0이

x
a,
>
thlo
ot
et
pe
i
rf
ae,
ac)
ai
ry
ae
ot
Au
[쏘
a
“2,
rlo
보
wy
so,
a,
0,
207
So,
rf
o
은
삐
oo

속단말                            는 기간과 접속지점과 접속단말기의 거리 그리
고 접속지점에서의 신호처리 시간에 의존한다. 그러나 이 시간은 매우 작다.

(9) 접속 프로토콜의 평가

접속 프로토콜을 평가하는데 사용되는 가장 기본적인 항목은 제공된 트랙픽 Ga
SE 6, 평균 전송지연 Dolch. 이상적인 접속 프로토콜에서, 전송률은 다음과 같이 주
어진다.

s-{t (G<]l)
“Ke (Get)         (6.3)

그러나 그림 6.5에 보인 바와 Bo], SE 가 증가함에 따라 증가한다. 또한, 6가어
떤 문턱치보다 크면 SE (가 증가함에 따라 감소한다. (가 1보다 크면 CE 급격하
게 증가하고 결국 무한대에 이른다. 이상적인 평균 전송지연은 전송 시도에 의해 모든
패킷이 목적지에 완전하게 전송될 수 있도록 스케줄링될 수 있고 스케줄 하는 처리과정
에 시간이 소요되지 않을 때 얻어진다. Kendall] 표기를 사용하면 이 과정은 그림 6.6
에서 보인 바와 같이 4/7071이다.

325


===== PAGE 328 =====
최신 이동통신시스템

Mobiie Communications using MATLAB Simulation

Ideal characteristic

더

Throughput

Actual characteristics

0                                         1
Traffic

를 그림 6.5 트래픽과

Actual
characteristics
~~

Normalized transmission delay

_

전송률의 특송

Lo

M/0/1

Vv

스

fo}

~

326

석인 구성을
2A~

Vv

퓨터 시뮬레이션을 통해 평가하는 과정

그림 6.7에 보였다.
ㅣ뮬레이션에서, 전송손실과 새도윙은 일정하다고 가정한



===== PAGE 329 =====
다중접속 프로토콜 【00”"：

다.성공적으로 ASS 패킷의 수가 요구되는 수와 같아질 때까지 컴퓨터 시뮬레이션은
계속 된다. 또한, 몇 가지 하위 프로그램을 만들고 변화시켜 다수의 접속 프로토콜의 성
능이 평가된다.

Traffic model                           ° Position of access point
Poisson arrival                      ¢ Position of user terminal
¢ Number of user terminal

호

Modeling of communication channel
Wired communication
¢ Ideal communication channel

Wireless communication
¢ Propagation loss
¢ Shadowing

Access protocol

Packet transmission
(new transmission or
retransmission)

Decision whether
the transmission packet
is successfully
transmitted
or not

Failure

Success

Measurement of transmission delay

Number of
successfully transmitted
packets reaches required
number in the
simulation

The simulation is finished

Throughput and transmission delay

를 그림 6.7 컴퓨터 시뮬레이션의 기본적 구성

327



===== PAGE 330 =====
vay 최신 이동통신시스템
Mobite Communications using MATLAB Simulation

6.4.3 주 프로그램

주 프로그램은 프로그램 6.1에 보였다. 프로그램에서는 다음과 같은 과정이 수행된
다. 모든 시뮬레이션 인자는 표 6.2에 정리되었다.

=

826.28 시뮬레이션 인자

변수명                    설명

brate                                                      비트 레이트 (6085)

Srate                                                      심볼 레이트 (608)

plen                                                  패킷 길이 (symbol)

Ttime                                                  패킷 전송 시간 (9)

Dtime                                               정규화된 전송 지연

alfa             전송 지연의 감쇄 고정 값

sigma                                             새노윙의 표준편차 (08)

capture                                                                    캡쳐효과: O:nothing 1:consider

r                            서비스 영역 반경 (m)

bxy                                                                     접속 지점의 위치 (xy,z) (m)

ten                        캡쳐비 (dB)

Mnum                                          접속 단말기의 +

mxy                                            접속 단말기의 위치 (xy,z) 02)

men                                              영역 끝에서 AS) 접속 지점에서의 C/N (08)
Mplen                                             패킷의 길이 (symbol)

Mstate                                          접속 단말기의 상태

mgtime                                               접속 단말기에서 패킷 생성 시간 (66000ㅁ08)
mtime                                         접속 단말기의 상태 변화 시간 (6600ㅁ08)
Mstime                                        접속 단말기의 패킷 전송 시간 (seconds)
G                                        제공된 트래픽

Tint                                              패킷 생성 간격의 71 cH HK (seconds)

Rint                                                          패킷 재전송 간격의 7) Ch Zk (seconds)
Spnum                                            성공적으로 ASA 패킷의 수

80600                                                시뮬레이션이 끝난 패킷의 수

Splen                                                  성공적으로 ASS 패킷의 데이터 (symbol)
Tplen                                                  ASS 시도한 패킷의 데이터 & (symbol)
Wtime                                              전송 지연 시간 (seconds)

328



===== PAGE 331 =====
다중접속 sees ㅠㅠ

. 주 프로그램과 부 프로그램에서 도두 공통으로 사용되는 변수는 메모리를 절약하고 me 실행을 위해 전
of 변수로 정의된다.

global STANDBY TRANSMIT 그 ee PERMIT
global Srate Plen Ttime Dtime

global Mnum Mplen Mstime Mstate

global Tint Rint

global Spnum Splen Tplen Wtime

2, 프로그램에서 사용되는 상수는 보편적으로 정의된다.

STANDBY   = 0;
TRANSMIT   = 1;
COLLISION = 2;
PERMIT    = 3;

3. 각 접속 프로토콜을 위한 부 프로그램의 이름은 배열 구성으로 정의된다. 부 프로그램의 이름을 배열화
라 하고 feval 함수를 사용함으로써 나 80/107문과 비교해 부 프로그램의 이름을 추가하거나 제거하기
act.

protocol = { 'paloha'   ㆍ. % Pure ALOHA       2080. 그
"saloha'      % 슬롯화된 ALOHA     : 2000 = 2
"npcsma'      % np-CSMA          :. 200 = 3
"snpisma'     % Slotted np ISMA   : pno = 4

} ;

4. 시뮬레이션을 위한 인자들이 정의된다. 여기서, ton2 접속지점에서 패킷 오류가 발생하지 않을 때 수신-
파워의 문턱치이다. 107은 접속지점에서 C/N (08로 정의되고 캡쳐 비라고 부른다. mone 접속단말기
의 전송 파워이고 서비스 끝 영역에서 생성된 전송 데이터가 전송 손실을 겪고 접속지점에 도달할 때 접속
지점에서 C/N (08로 정의된다. pno= 과정 (3/에서 보인 배열로부터 색인을 지명하여 접속 프로토콜을
선택한다. 게다가, 시뮬레이션에서 캡져효과를 포함하지 않도록 선택하면, 프로그램은 유선통
신채널 (이상적인 통신채널)에서 시뮬레이션 된다. 또한, 캡쳐효과를 포함하도록 선택하면,
프로그램은 무선통신채널에서 시뮬레이션 된다. 그 다음, 목적지에 성공적으로 전송될 수 있는
패킷의 총 수가 시뮬레이션 프로그램을 멈추는 조건이 되고 이를 spend= 쓴다. 변수 04006
에서, 시뮬레이션 결과가 저장될 파일의 이름은 다음과 같이 나타낸다:

329



===== PAGE 332 =====
최신 이동통신시스템

330

Mobile Communications using MATLAB Simulation

brate   = 512e3;       % bit rate
Srate   = 256e3;       % symbol rate
Plen    = 128;         % length of a packet
Dtime   = 0.01;        % normalized propagation delay
alfa    = 3;           % decline fixed number of
% propagation loss
sigma   = 6;           % standard deviation of shadowing [dB]
% definition of the access point
i       = 100;         % service area radius [m]
bxy     = [07707 hip   % position of the access point
%- (X,y,Z) [ma]
ten     = 10;          % capture ratio [dB]
Mnum    = 100;         % number of the access terminal
men     = 30;          % C/N
pno     = 1;           % protocol number
capture = 0;           % capture effect O:nothing 1:consider
spend   = 10000;       % number of packets that
% simulation is finished
outfile = 'test.dat'; % result output file name

. 과정 4.에서 정의된 인자로부터, 패킷을 목적지에 전송하는 시간과 접속지점에서의 C/No| 계산된다. 접

속지점에서의 C/NZ 계산하기 위해, 접속단말기가 이] 지점에서 WAS 전송한다고 가정한다.

Ttime   Plen / Srate;

mpow

fid = fopen(outfile, 'w');

fprintf (fid, 'Protocol
fprintf (fid, 'Capture

L0™(men/10))-*. sqrt (r“2+bxy (3) *2) alfa;

. 과정 4.에서 정의된 인자는 파일에 저장된다.

= $d\n',pno);

= $da\n',capture) ;

fprintt (fray
fprintf(fid,
Eprintt (hid,
forIntr (fig;

"Normalize delay time       = %f\n',Dtime) ;

"Bit rate (bps)
"Symbol rate (sps)
"Length_of Packet (sbl)

$da\n',brate) ;
sd\n',Srate) ;
sd\n',Plen) ;



===== PAGE 333 =====
다중접속 프로토콜 Fe

fprintf(fid, 'Number of mobile station = %d\n',Mnum) ;
fprintf (210, 'Transmission power (C/N)   = $f\n"',mcn);
fprintf(fid, ‘Capture ratio (dB)         = $f\n',tcn);

fprintf(fid, 'Number of Packet

$d\n', spend) ;

7. BE 접속단말기는 랜덤하게 배열된다. 그 다음, 접속단말기와 접속지점 간의 새도윙이 정규분포를 갖는
랜덤 값으로부터 주어진다.

mxy = position(r,Mnum, 0);       % positioning of the access
terminals

randn('state',sum(100*clock) ) ;   % resetting of the random
table

mrnd = randn(1,Mnum) ;            % decision of the shadowing

8. 시뮬레이션에서 제공된 트래픽은 10 루프의 색인 GS 주어진다. 여기서, 제공된 트래픽의 Ze 접속단말
기의 수보다 적어야 한다. 만약 G7} 접속단말기의 수보다 크면 시뮬레이션은 멈추게 된다.

LOE @510.410.4 sh, 10240.28691             % offered traffic
if G >= Mnum
break

end

9. 패킷의 생성간격의 기대 값이 단말기의 수로부터 계산된다. 그 다음, 패킷 재전송 간격의 기대 값이 생성
간격의 기대 값과 동일하게 설정된다. 실제 시스템에서, 패킷 재전송 간격은 시뮬레이션된 접속 프로토콜
에 의존한다. 예를 들면, 슬롯화된 ALOHAS| 경우, 패킷은 10 시간 슬롯 안에 보내진다. 그러나 패킷재
전송 간격이 특정 영역 내로 고정되어 있으면, 실제 제공된 트래픽은 설정 인자 Goll 따라 다르다. 여기서,
Gol 전송률과 평균 전송지연을 얻는 것이 시뮬레이션 프로그램의 목적 중 하나이다. 그래서 패킷재전
송 간격은 HAS 간격에 사용되는 지수분포를 따라야한다.

Tant
Rint

{I

-Ttime / log(1-G/Mnum) ;          % generation interval

ㅣ

Tint;                           % resending interval
Poissonz} 지수 분포를 사용한 Tint} Rint2| 유도는 부록 64에 보였다.
10. 시뮬레이션에서 사용되는 HS 초기화한다.

Spnum = 0;

331



===== PAGE 334 =====
최신 이동통신시스템

332

Mobile Communications using MATLAB Simufation

ate

12.

13.

14.

15.

Splen = 0;
Tplen = 0;
Wtime = 0;

now_time = feval (char (protocol (pno)),-1);

while 루프의 시뮬레이션 프로그램이 핵심 프로그램이다. 접속 프로토콜은 부 프로그램에서 프로그래밍
된다. 순수 ALOHA, 슬롯화된 ALOHA, np-CSMA, 슬롯화된 npISMAQ] 각각의 자세한 내용은 6.5,
6.6, 6.7, 6.8장에서 각각 설명된다. 기본적인 조작은 다음과 같다. 모든 접속단말기의 상태는 전역변수
Mstatedl| 저장된다. 그 다음, 단말기 조건이 변하는 시간이 리턴된다.

next_time = feval (char (protocol (pno)),now time) ;

접속단말기에서 접속지점으로 성공적으로 전송되는 패킷의 총 수가 정의된 변수 60600보다 크면, Gol
서의 시물레이션은 멈춘다.

if Spnum >= spend
break

end

WAS 접속지점에 전송한 접속단말기가 카운트된다.

idx = find(Mstate==TRANSMIT | Mstate==COLLISION) ;

캡쳐효과를 고려하지 않을 때 접속단말기에서 ASE! 패킷이 접속지점에서 성공적으로 수신되었는지 여
부의 결정은 이곳에서 이루어진다. 과정 (12)에서, 패킷을 전송하는 두개 이상의 단말기가 존재하면, 충돌
이 발생한다. 이 경우, 패킷의 전송이 실패하기 때문에, 데이터 COLLISION] 변수 !/6【816에 저장된다.

if capture ==                        % without capture effect
if length (idx) > 1                % transmission terminals
Mstate (idx) = COLLISION;      % collision occurs
end

캡쳐효과를 고려할 때 접속단말기에서 ASE 패킷이 접속지점에서 성공적으로 수신되었는지 여부의 결
정은 이곳에서 이루어진다. 캡쳐효과에 의해, 최대 수신파워를 갖는 패킷은 접속지점에서 살아남는다. 그
래서 먼저, 접속지점과 패킷을 전송한 접속단말기 간의 거리가 계산된다. 그 다음, 접속단말기로부터 전
송된 모든 패킷에 대해 C/NO| 접속지점에서 계산과 최대 C/NS 갖는 패킷이 선택된다. 그 다음, 선택된
패킷에 대해, 다른 패킷을 잡음으로 간주함으로써 순간적인 C/NO| 다시 계산된다. 계산된 C/NO| 문턱치



===== PAGE 335 =====
다중접속 zece FO

보다 크다면 패킷의 순간적인 데이터는 접속지점에 성공적으로 전송되고 결과는 변수 Mstateol 저장된
다. 반면, 계산된 C/NO| 문턱치보다 낮으면 사용자로부터의 모든 패킷은 접속지점에 전송되지 않고 결과
는 Mstatedl| 저장된다. Mstate7} 패킷 전송동안 TRANSMIT 일 때, 패킷 전송은 성공적으로 끝난
다; 그렇지 않으면, 충돌이 발생한다.

else                                 % with capture effect
if length(idx) > 1
dxy = distance (bxy,mxy(idx,:),1);
pow = mpow * dxy.*-alfa .* 10.%*(sigma/10*mrnd (idx) ) /

[maxp no] = max(pow);
if Mstate(idx(no)) == TRANSMIT
if length(idx) == 1

cn = 10 * logl0(maxp) ;
else
cn = 10 * 1ogl0(maxp/ (sum(pow)-maxp+t1) ) ;
end
Mstate (idx) = COLLISION;
if on >= ben
Mstate (idx(no)) = TRANSMIT;
else
Mstate (idx) = COLLISION;
end
end

end

각 접속단말기의 상태가 변할 때(예, 새로운 패킷이 생성될 때) 시간 카운터가 증가한다.

now_ time = next_time;

. 하나의 G 값에 대한 시뮬레이션이 끝날 때 평균 트래픽, 전송률, B
파일에 저장된다. 여기서, 평균 트래픽은 모든 WAS 전송하는

로 정의된다. 또한, 전송률은 접속지점에서 성공적으로 수신한

간으로 나눈 값으로 정의된다.

균 전송지연과 같은 결과가 표시되고
기간을 총 시뮬레이션 시간으로 나눈 값으
패킷을 전송하는 시간을 총 시뮬레이션 시

traffic = Tplen / Srate / now_time;
ts

theorys (pno, traffic, Dtime) ;

333



===== PAGE 336 =====
최신 이동통신시스템

Mobile Communications using MATLAB Sinufation

fprintf (fid, 'sf\ts£\ts£\tsF\ts£F\tsf\tsf\n',G,now time ...
,Splen/Srate,Tplen/Srate,Wtime, Tint,Rint) ;
fprintf ('G=sf\tS=sf\tTS=sf\n', traffic, Splen/Srate/now time, ts) ;

18. G 인자의 설정에서 SE 시뮬레이션을 마칠 때, 시뮬레이션 AAS 저장하는 파일을 닫고 성능이 표시
된다.

fclose(fid);
graph (outfile) ;

644 부 프로그램의 설명
(1) 접속단말기의 배치를 위한 부 프로그램

부 £214) positionms 프로그램 6.2에 보였다. 입력 인자는 』ㅁ인데 re 셀의
반경이다. 그림 6.8에서와 같이 반경 의 원형구역에ㅁ명의 사용자가 임의로 배치된다.
Alo] 중심은 원점 (0,0)9] 다. BE 사용자의 위치는 달라야 한다. he 각 접속단말기의
높이이다. h-1S 설정할 때, 각 접속단말기의 높이는 1에서 4의 랜덤 HS 갖는다. 모든
사용자의 결정된 위치 정보는 사용 단말기 + by 32] 행렬이 된다.

Access point

User terminal

를 그림 6.8 접속지점과 사용자 단말기의 배치

334



===== PAGE 337 =====
(2) 접속지점과 접속단말기 간의 거리를 계산하는 부 프로그램
부 22718 distancemS 프로그램 6.3에 보였다. 입력 ASE bstn, mstn, 801이다.
sclo] 생략될 때, 901=1이다. 680은 그림 6.8에서 보인 바와 Zo] 접속지점의 위치를
xyz 좌표계를 사용해 나타낸 것이고 mine 접속단말기의 위치를 나타낸 것이다. S
은 801과 660과 mstn 사이의 거리를 곱한 것이다.

(3) 전송률의 이론치 계산을 위한 부 프로그램

부 프로그램 601*8.2을 프로그램 6.4에 보였다. 입력 ASE no, g, 8이다. 20는 선
택값을 나타낸다. no=1,2,3,49) 때, 순수 ALOHA, 슬롯화된 ALOHA, 비영속적
CSMA, 슬롯화된 221884스가 각각 접속 프로토콜로 선택된다. ge 주어진 트래픽이고
ax 정규화된 전송지연이다. AA nos 함께 gas 입력함으로써 이론적인 전송률
이 계산된다.

(4) 시뮬레이션 결과와 이론치를 그림으로 보이기 위한 부 프로그램

부 프로그램 800.0을 프로그램 6.5에 BAC. grapht 제공된 트래픽과 전송률 그
리고 제공된 트래픽과 평균 전송지연의 결과를 표시한다. 입력 인자는 41608006인데 이
는 시뮬레이션 결과를 저장한 파일의 이름을 지칭한다.

Wy 순수 ALOHA

6.5.1 원리

순수 ALOHA 접속단말기가 패킷을 보내고 싶은 데로 전송하는 프로토콜이다. 이
프로토콜은 1970년에 하와이 대학에 의해 제안되었다. 이 프로토콜의 경우, 모든 접속
 단말기는 채널이 사용 중인지 어떤지 관심 두지 않는다. 기본 구성은 그림 6.9와 같다.
각 패킷의 길이가 고정되어 었고 패킷을 전송하기 위한 시간이 7'라면, 패킷은 그림
6.10에서와 같이 다른 패킷이. 7, ㅡ7 에서 + 2 의 27S ASS 식작하지 않으

335



===== PAGE 338 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

면 접속지점에 성공적으로 전송된다. 그래서 제공된 트래픽 (;에서 EF ALOHAS] 전
송률 6는 다음과 같다:

(06.                                     (6.4)

위 수식에서 무한 콜자원 모델이 가정되었고 (=0.5일 때 최대 전송률은 0.184이다.
전송률의 자세한 유도는 부록 68에 제시한다.

Success       Collision         Success     Success
Access      ㅣ       |                    liz     elas
point       1       i    .    ee    {     {       |    |     —~ t
1       |    '    1   1    ㅣ     ㅣ       |]    '
'       1    1    1   1    1     ㅣ       i    1
'       1    1    '   ㅣ    1     ㅣ       1    1
User            a: Ss Se     |       a
terminal 1               '    re    |       |    '      at
1    '   ㅣ    '     :       '    1
Packet        HE Se eee     {       본 아이
(ser     arrival       WHA   |    ree   |
terminal 2       |                |     ot
:                Packer + Retransmission
i                    arrival    with random delay
User                       Wn                |
terminal N                   Pee oe 으아      at
Packet           ee
srival     Retransmission
를 그림 6.9 순수 ALOHA
User
                                            et
terminal 1   t-T          +.            aT
I
|
1
User
terminal 2

Collision
User
terminal 3                                       |                   at

를 그림 610 순수 ALOHA 시스템에서의 패킷의 충돌

¥

4

|
=

336



===== PAGE 339 =====
다중접속 프로토콜 0ㄴㅠ

6.5.2 시뮬레이션 프로그램

부 프로그램 201088.2을 프로그램 6.6에 보였다. 입력 인자는 현재 시간을 나타내는
now_timeo|t}. 출력은 ?0088의 함수를 수행한 후 각 접속단말기의 상태가 변하는 시
간을 UEMHE next_time°]t}. palohaS} 함수는 6개 기능으로 분류할 수 있다. 표 6.3은
시뮬레이션 조건을 보여준다.

HB 6.38 시뮬레이션 조건

r           서비스 영역 반경                                                  100m

bxy:         접속 지점의 높이                                                   5m
Mnum:      단말기의 수                                                100
Srate:        심볼 레이트                                                           256 ksymbol/second
Plen:         패킷 길이                                                            128 symbol

alfa:       거리 감쇄 고정 값                                        3
sigma:       로그정규분포의 표준편차                                        608

men:     영역 끝에서 송신할 때 접속 지점의 CN              30 08

ten:         캡쳐 비                                                               10 08

1. 첫 번째 블록에서, 전역변수와 정적 변수가 정의된다.

global STANDBY TRANSMIT COLLISION
global Srate Plen

global Mnum Mplen Mstate

global Tint Rint

global Spnum Splen Tplen Wtime

persistent mgtime mtime

2. = 번째 블록에서, now_time(O 일 때 모든 접속단말기의 상태가 초기화된다.

if now_time < 0
rand('state',sum(100*clock) );

mgtime         = Tint * log(l-rand(1,Mnum) );

337



===== PAGE 340 =====
최신 이동통신시스템

338

. 다섯 번째 블록에서, 00\_10076에서 패킷
상태

Mobile Communications using MATLAB Simulation

1

mtime            mgtime;
Mstate

Mplen (1:Mnum)

zeros (1,Mnum) ;
Plen;

min (mtime) ;

next_time
return

end

3. 세 번째 블록에서, 패킷 전송이 성공적으로 끝났을 때, SE 단말기에 대해 성공적으로 ASE! 패킷의 +

를 세고 전송지연이 계산되고 새로운 패킷이 생성된 시간이 계산된다. 여기서, 각 단말기에서 새로운 패킷
은 각 채널에서 생성된 패킷이 성공적으로 접속지점에 ASS 때까지 생성되지 않는다.

idx = find(mtime==now_time & Mstate==TRANSMIT) ;
if length(idx) > 0

Spnum          = Spnum + 1;

Splen          = Splen + Mplen (idx);

Wtime          = Wtime + now_time - mgtime (idx) ;
Mstate (idx)    = STANDBY;

mgtime (idx)    = now time - Tint * log(l-rand) ;
mtime (idx)     = mgtime (idx) ;

end

. 네 번째 블록에서, 패킷 ASO] 끝나고 ASO] 실패했을 때, 패킷이 MASSE 시간이 SE 단말기에 대

해 계산된다.

idx = find(mtime==now_time & Mstate==COLLISION) ;
if length(idx) > 0
Mstate (idx)

STANDBY ;
mtime (idx)     = now time - Rint *
log (1l-rand (1, length (idx) ) ) ;

을 전송한 접속단말기가 모든 접속단말기에 대해 찾아진다. 그
다음, 상태가 TRANSMIT BES 변하고, 패킷 MAS 마치기 위한 시간이 계산되고 전송된 패킷의 수가
카문트된다.

idx = find(mtime==now_time) ;



===== PAGE 341 =====
다중접속 프로토콜

if length(idx) > 0

Mstate (idx)    = TRANSMIT;
mtime (idx)     = now _time + Mplen(idx) / Srate;
Tplen         = Tplen + sum(Mplen (idx) ) ;

end

6. 여섯 번째 블록에서, mtime Ce He 최소값을 찾음으로써 각 접속단말기의 상태가 변할 때 가장 가까운
시간인 next_timeo| 결정된다.

next_time = min(mtime) ;

6.5.3 시뮬레이션 결과
주 프로그램 mainms 실행함으로써
>>main

전송률과 평균 전송지연의 성능과 평가가 결정 된다; 시뮬레이션 결과를 그림 6.11과
6.12에 제시한다.

03                                      개 Without capture affect
-@- With capture effect
— Theory
0.25                   OOo                                     케
9                           - oe

Throughput
o
=          은
ou            nN
ra

은
oe
T

0.05}

L       1        L       1       1

0         0.2        0.4        0.6        0.8          1          1.2        1.4        1.6        1.8          2
Offered traffic

를 그림 6.11 순수 ALOHAD 제공된 트래픽과 전송률

339


===== PAGE 342 =====
1  최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

- @ - Without capture effect
--9-- With capture effect
의
2500}-                                                  |
                                                   :
rs
든
= 15마                                         :        |
eo                                         |
=                                       ‘
을 1000                           1              |
                                 rm
Pe ty 아구 Sg eaeq
:                   aoe「   ‘
’                 :  By ee i°qaaeseeeoo:
eg ae    o  0  @……'9"4
& 8 용 OO e "1
0      1     1     1     1     *     ;     :     」
0     0.2    0.4   0.6    08     1     1.2    1.4    16    -P    :
Offered traffic

를 그림 6.12 순수 ALOHA 제공된 트래픽과 평균 지연시간

캡쳐효과가 고려되지 않았을 때, 전송률은 사용자의 수가 100이어도 이론적인 값과
근사하다. 캡쳐효과가 고려될 때 전송률은 캡쳐효과가 고려되지 않았을 때보다 크다.
게다가, 평균 전송지연은 감소한다. 순수 ALOHAY] 경우, 충돌이 자주 발생 한다; 그래
서, 캡쳐효과가 전송률을 증가시킨다.

We secs! ALOHA

6.6.1 원리

순수 ALOHAS] 간단한 수정으로, 즉, 메시지를 두 동기화 펄스 간의 슬롯 시간 내에
전송하고 시간 SRY 시작에서만 시작될 수 있도록 함으로써, SES] 비율을 반으로
감소시킬 수 있다 [29]. 이 프로토콜을 슬롯화된 4ㅁ08스라고 부른다. 구성은 그림
6.13에 보였다. 그림 6.13에서 시간 슬롯 내에 생성된 패킷이 다음 시간 슬롯에서 전송
된다. HAS 접속지점에 성공적으로 전송하기 위해서, 한 시간 슬롯 내에 생성되는 패

340



===== PAGE 343 =====
다중접속 프로들를

논박

ㅇ

——

nf

의 수는 그림 6.14에서와 같이 10] 되어야한다. 한 시간 슬롯 내에 두개 이상의 패킷
생성되면 충돌이 발생한다. 그래서 제공된 트래픽 (에서 슬롯화된 ALOHAS] 전송
S= 다음과 같다:
S = (06 "                                     (6.5)
Slot
 ae        :        :       |
' Success | Collision |         ' Success !
point       ;       :       :     = t
User        eT
terminal 1                  -           1           {           |        ora
Packet        |        |        !       \
arrival                 |        :
User              |             ZZ.                           0
terminal 2    1       i        1       1
H        ' Packet !        때       !
! es      P 에베      |
om        |        |
terminal N                              .         .       +t
Packet                Retransmission
arrival
0 그림 6.13 슬롯화된 ALOHA
나 이마 Success !           ;           :
User      H                   i      |     oo
terminal 1    |   개   i       ㅣ       {       {    at
i Packet {      {      {      {
0     t arrival |     '     }     :
terminal 2    t       t       !                       t
'       ㅣ       ㅣ 4     '       1
|      1      | Packet 1 Collision |
—       :       | arrival }        :
1       '
terminal 3    ‘                                     t
Packet
arrival

를 그림 6.14 슬롯화된 ALOHA 시스템에서 패킷의 충돌

341



===== PAGE 344 =====
골 최신 이동통신시스템

Mobile Communications using MATLAB Simulation

위 수식에서 무산 콜자원 모델이 가정되었고 (*=1일 때 최대 전송률은 0.368이다.
전송률의 자세한 FEE 부록 08에 제시한다.

6.6.2 시뮬레이션 프로그램

부 22714 salohamS 프로그램 6.7에 보였다. 프로그램은 기본적으로 2011048.20과
같다. 그러나 패킷을 전송하는 시간이 시간 슬롯과 동기화 된다.

6.6.3 시뮬레이션 결과

전송률과 평균 전송지연의 시뮬레이션 ANS 그림 6.15와 6.16에 보였다. 6.5.3장에
서와 같이 캡쳐효과의 영향은 현저하다.

yee       3       - | ㅇ Without ca    re effect
Re  A BPO...           60 Wan core act

Throughput

L                            My                            L                            L                           L                          |                            1
0.5            1             15            2            25            3            35            4
Offered traffic

를 그림 615 슬롯화된 ALOHA 제공된 트래픽과 전송률

342



===== PAGE 345 =====
다중전속 프로토콜 EO

1400                 ㅜ-    -
1200 +                                                                 ;
1000                                         ‘

| |                                      더

% 800+                                                ?

등

>                                      오

홈 …                               ee

느                               ys

2 400 F                               oe

ot         iS 90"
200 + ge   : 9 OOF xe
ogo"    6 OO"
0      i     wy

0             05             1              15                            25             3             35             4

2
Offered traffic

를 그림 616 SSH ALOHAD 제공된 트래픽과 평균 지연시간

[| 비영속적 CSMA

6.7.1 8 2

이름은 통신채널에 반송가의 존재 여부가 접속단말기에 의해 감지되는 데서 유래한

다. 반송파 감지를 통해, 각 접속단말기가 그림 6.17에서와 같이 패킷 전송 외에 다른 반
송파를 전송하지 않기 때문에 다른 접속단말기가 패킷을 전송하는지 여부를 판단할 수

ㅜㅜ

통신채널에서 반송파가 감지되면 이 조건을 “608”라고 부르고 그렇지 않으면
“1016”이라 부른다. CSOMAS 반송파 감지의 결과로 패킷 ASS 시작할지 여부를 결정
하는 프로토콜이다. 결과가 “5087”이면 SSS 피하기 위한 조치가 필요하다.

이 장에 제시된 비영속적 CSMAE SES 피하기 위한 프로토콜의 하나이다. 비영속
적 CSMAA, 접속단말기에서 패킷이 생성될 때 접속단말기는 반송파 감지를 시작한
다. 반송파 감지의 결과가 “4016”이면 패킷은 접속지점에 즉각적으로 전송된다. 그러나

343



===== PAGE 346 =====
최신 이동통신시스템

344

Mobile Communications using MATLAB Simulation

반송파 감지의 결과가 “6485”이면 접속단말기는 반송파 감지를 멈추고 잠시 대기한 후
반송파 감지를 다시 시작한다. 대기시간이 높은 전송률을 얻기 위한 중요한 인자이다.
Success                 Collision
Access        |         |                                    pe
point          F         잘           ee,     Ry
!         1           pees     eet
'         1           pot     ae.
1]         1]           {   '     !   그
   Ul      :   i
User                            i  1     and             Sian
terminal 1              '          cm,      > 대
M         y         i  :      H  ;
1         '         내      『
\         \                    Ul
User         es         :        ^      :               mr
terminal 2       ‘  {      :         rs       UF Pane me ener i
|           {         ‥ㆍ       나        \! Retransmission
             4   Waiting .        4          ‘
H                 \             \         i ‘           : ‘
:            \         \           들
User               ‘           '      Wag   ,                   at
terminal N                Bee               ne eae
Carrier                   Retransmission
sense
를 그림 6.17 4844 CSMA
CSMAA, 각 접속단말기가 반송파 감지를 수행해도 패킷의 충돌이 발생한다. 한
가지 이유는 전송지연시간이다. 실제 통신 시스템에서, 접속단말기가 패킷을 전송할
때, 다른 접속단말기는 전송지연시간으로부터 전송을 검출한다. 다른 단말기가 전송지
연시간 동안 MAS 전송하면 그림 6.18에서와 같이 접속지점에서 충돌이 발생한다. 전
송지연시간은 접속단말기 간의 거리에 의존한다. 대부부의 경우, 전송지연시간은 시스

주기로 정규화된 전송지연시간은 각 접속단말기에서 접속지점까지
무선통신 시스템에서, 반송파는

템에서 동일하고
의 패킷 전송에 필요한 시간과 같다고 가정한다. 또한,

때때로 그럼 6.19에서와 같이 접속단말기가 HAS 전송하더라도 어떤 접속단말기들
에서는 감지될 수 없는데 이는 접속단말기 사이에 장애물이 존재하기 때문이다. 이 문

제를 “숨겨진 Hey) hidden terminal” 문제라 부른다.



===== PAGE 347 =====
다중전속 프로토콜 FOR

Success

User        ' ea                          B Bi     7    Ld      *       >t
terminall 고           ‘                 ,      5     ,      ,

is           \                t      7     ?      7,

' ‘            \                ‘       7     ,       ,

i 도           \              t      1)     é      f

t  \           \                               7

ㅣ  호           \                              /
User        <p cat           는                       L    7               t

호            호                           7,
terminal 2    {           {           ;   ;        Ap
\            ry           | 4

eis            A          eC ar   a

|     {           총         ㅣ             4

1     도           \         1               1

1      \           \        1               \
User                           로                                        t
terminal 3

a: Propagation delay

를 그림 6.18 noCSMAOA 패킷의 충돌
Carrier sense is failed

because of long distance
배아 5 gs ee        User
terminal 3                                            terminal 1

Carrier sense is failed
because of obstacles
like bulidings

User
terminal 2

를 그림 6.19 숨겨진 단말기 문제

고

a

|공된 트래픽 에서 비영속적 CSMAS] ASS 6는 다음과 같다:

=          26
G(1+2a)+e                                   (6.6)

345



===== PAGE 348 =====
최신 이동통신시스템

Mobile Communications using MATLA8 Simulation

6.7.2 시뮬레이션 모델

부 2274 npcsmamS 프로그램 6.8에 제시한다. 이 부 프로그램은 기본적으로
281008.0과 같다. npcsma2] 구성은 6.5.2장에서 논의된 5개의 블록으로 나뉘고
0005008와 paloha 간에 서로 다르다. 200808에서, 반송파는 함수 63016796056.02을 A}
용하여 각 접속단말기가 패킷을 보내기 전에 감지된다. 결과가 “1016”이면 패킷은 접속
AALS 전송된다. 결과가 “608*”이면 패킷 재전송 시간이 스케줄링 된다. 모든 접속
단말기에 대해 패킷 전송시간에 대한 모든 정보가 전역변수 Mstimeo] 저장된다.

idx = find(mtime==now_time & Mstate==STANDBY) ;
if length(idx) > 0

Tplen = Tplen + sum(Mplen (idx) );

for ii=1:length (idx)

73 = Adx (aij
if carriersense(jj,now_time) == 0
Mstate (jj) = TRANSMIT;
Mstime (33) = now_time;
mtime(jj) = now time + Mplen(jj) / Srate;
else
mtime (jj) = now_time - Rint ^ log(1l-rand);
end
end
end

다음으로, # ©2728 carriersensemS 프로그램 6.90] 보였다. 이 프로그램에서,
패킷의 전송시간을 나타내는 4490006이 접속단말기 간의 거리에 의존하는 전송지연시
간에 더해진다. 그 다음, 모든 단말기에 대해 반송파가 감지된다. 만약 반송파가 감지되
면, “busy” (768411)로 그렇지 않으면 “idle” (result=0)° = 설정된다.

ㅁ

ㅇ

6.7.3 시뮬레이션 결과
송률과 평균 전송지연의 시뮬레이션 결과를 그림 6.20과 6.21에 보였다. 시뮬레이

ra

346



===== PAGE 349 =====
션에서, 정규화된 전송지연 a 0.01이나 0.10]c}. np-CSMAY] 최대 전송률은 정규화
된 전송지연에 90 a7} 작으면 0ㅠ0514ㅅ의 최대 전송률은 순수 4108보다
높다. 그러나 a7} 크면, 성능은 순수 ALOHA S} 근사하다.

© Without capture effect
--@- With capture effect     [e =0.01]                                       J
0.9 | — theory                      {a=0.01)

ㅁ Without capture effect [a =0.1)
--#- With capture effect    [a=0.1)
-—:- Theory             [a=0.1)

1

10

10°                    10°                   10°
¥          Offered traffic

를 28 6.20 npCSMAY 제공된 트래픽과 전송률

-@- Without capture effect [a = 0.01]                   H                      .
- © With capture effect           [a =0.01]                      |                         :
-@- Without capture effect [a=0.1]             .              J
- + With capture effect       {a=0.1]              t               ;
:             +
을                                                               +*
E                                                              :
s                                                              2
>                                                             :
|                                                            *
o                                                            Py
<c                                                            :
은
© 5007                                                 #            @              기
[                                                        :              :
x)             9
_              가   0
sates                               oo?
ap 니스 에   때 매 # FineseneS: @-
i                                           fouee       1    시 시 시소 소오소
10"                “0                  10                  10°                 10°
Offered traffic

M28 6.21 ㅁㅁ-061/4의 제공된 트래픽과 평균 지연시간

347


===== PAGE 350 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

이는 접속단말기가 반송파를 감지한 후에 패킷을 전송하더라도 다른 접속단말기가
! 전송지연시간동안 HAS 전송하기 때문이다. 결과적으로, 충돌이 발생한다. 또한,
캡쳐효과가 고려되면, ASS MAS 전송한 접속단말기 간의 수신-파워의 차이 때문
에 종종 존속되기도 한다. 그래서 전송률이 증가한다.

가프 | 슬롯화된 비영속적 ISMA

6.8.1 원리

CSMAE 단말기가 다른 사용자의 전송 WSIS ASHES 함으로써 충돌 확률을
감소시킨다. 그러나 CSMAS 두 단말기가 서로 영역밖에 있거나 장애물에 의해 분리

되어 있는 경우에는 충돌을 피할 수 없다. 그러한 두 단말기는 서로 숨겨져 있다고 간주

된다. ISMAE 숨겨진 접속 단말기 문제를 해결하기 위해 제공된 sys] 해법이다.
ISMAY 접속지점으로부터 접속단말기까지 통신채널의 상태를 알림으로써 숨겨진
접속 단말기 문제를 해결하는 시스템이다. 그 개념은 그림 6.22에 보였다.

ISMAI, 접속지점은 접속단말기로부터 패킷을 받고 있을 때는 모든 접속단말기
에 busy ASS 보낸다. 반면, 접속지점은 WAS 받고 있는 않을 Hide 신호를 보낸
다. 각각의 접속단말기가 idle ASS 받으면 각 접속단말기는 MAS 전송할지의 여부
를 결정해야만 한다. 각각의 접속단말기가 6055 ASS 받으면 각 접속단말기의 패킷

348



===== PAGE 351 =====
로비

금지된다. 그래서 이 프로토콜은 1554ㅅ라 불린다. 기본적으로, 숨겨진 단말기
하지 않는 CSMAZ 간주될 수 있다. 그러나 1554ㅅ의 전송지연시간은 모든 접
이 접속지점으로부터의 신호만을 검출하기 때문에 CSMAY] 두 배이고 접
속단말기로부터 패킷을 수신하고 그 다음에 모든 접속단말기에 605 신호
.CSMANA| 접속단말기는 다른 접속단말기로부터의 ASS 감지한다. 다른
기가 전송지연시간동안 AAS 전송하면 그림 6.23에서와 같이 접속지점에서 충
발생한다. 여기서, 정규화된 전송지연시간은 하나의 패킷을 전송하는데 필요한
으로 정규화 된다. 또한, 1654에서, 다운링크는 접속 지점으로부터 접속단말기로
크이고 엽 렁크는 접속단말기로부터 접속지점으로의 링크이다.

wh on slo

aS
qu

Spe She 때
te Ly OP
ec
a oe

my

i
l=

a

때

~

ㅇ

att
é

to,
ol!

Collision

Access point

User
terminal 1

User
terminal 2

d: Propagation delay

를 그림 6.23 ISMAOIA 패킷의 충돌

이 장은 그림 6.24에 보인 슬롯화된 비영속적 ISMA] 중점을 둔다. 이 프로토콜에
서, 엽 Bae 한 패킷의 주기 TH 슬롯화된다. 각 접속단말기가 MAS 생성할 때, a
속단말기는 억제감지를 수행한다. 1016 신호를 받으면, 접속단말기는 다음 시간슬롯어
서 패킷을 전송한다. 반면 busy ASS 받으면, 접속단말기는 전송하지 못하고 임의

그                                       그는                                vs   ]

시작한다. 이 때, 접속지점ㅇ

0 &

=
hk 5 =e

349


===== PAGE 352 =====
최신 이동통신시스템

a

350

Mobile Communications using MATLAB Simulation

접속단말기에 busy UES 전송하는 ANSE busy 슬롯이라 부른다. 접속지점은 모
든 사용자로부터 패킷 수신을 마치면 모든 접속단말기에 패킷을 전송할 다음 시기를 알
려준다. 그러나 접속지점이 어떤 패킷도 수신하지 못하면 접속지점은 단말기에 다음 시
기를 알려준다. 정규화된 ASAAS 4로 취하면, busy SKS (1+ d) TBA Alok
하고1016슬롯은 최소한 27"이상이어야 한다. 제공된 트래픽 에서 슬롯화된 비영속
AISMAS| 전송률 Se 다음과 같다:

트   26“
ltd”                                      (6.7)
전송률은 무한 콜자원 BAS 가정한 이상적인 통신채널에서 얻어진다. 전송률의
자세한 유도는 부록 08에 제시한다.
1016
Busy slot__ |, slot ,|
a | |
Access                              teins              +
point       ,        ets Rear        ty
g\ /@    Merges 8    I\Z
ay,  반     시 기 H  of '  로     '  도
\     \         \
User             p        Glee Te.         수
terminal 1     |     ;  ;      i art     rt     :
Packet |   mans   pea      |    |      i
arrival ;    | 500600 그880800!     gio     ㅣ
1     1         1      7              1
User        !     :         :      2      :         >t
terminal 2     1     i    |    I  |  I     1         1
:        ㅣ     i         1     1     ert 여겨
\     ㅣ         1     ㅣ     at     1      —
1     ㅣ         !     i     boot     1Retransmission
i   1 Waiting 1    i    i  ㅣ    ㅣ
1     1         ㅣ     ㅣ     개     1
User        4    +        +     NY      +         6
terminal N     461  |
에                 Retransmission

d: Propagation delay          Waiting

를 그림 6.24 슬롯화된 비영속적 SMA



===== PAGE 353 =====
다중접속 프로토 FO

6.8.2 시뮬레이션 GE

부 프로그램 940169018.0을 프로그램 6.100] 보였다. 이 프로그램은 기본적으로 프로
그램 6.8에 보인 4005018.2과 같다. 940181008의 구성은 6.5.2장에서 논의한 7개의 블록
분류된다. 첫 번째 블록과 일곱 번째 블록은 2006008와 동일하다.
snpisma2] 다섯 번째 블록에서,20\ _8206에서 HAS 생성하거나 MAS 전송하기
위해 대기하는 접속단말기는 억제감지를 수행한다. 결과가 10416이면,00\_0006은 패킷
을 전송할 다음 시기까지 갱신된다. 결과가 605$이면 다음 억제감지가 수행될 시간이
결정된다.

6.8.3 시뮬레이션 결과
전송률과 평균 전송지연의 시뮬레이션 결과를 그림 6.25와 6.26에 보였다. 시뮬레이

션에서, 정규화된 전송지연 a= 0.02와 0.2이다. 슬롯화된 비영속적 ISMAS] 최대 전
SEE 정규화된 전송지연에 의존한다. 또한 캡쳐효과가 고려되면, AS Wale 종종
도착한 패킷의 수신파위가 서로 다르기 때문에 존속되고 이로 인해 ASHES 증가한다.
1                wry:                 T
Without capture effect (a =0.02)
With capture effect   {a =0.02)
Theory          (a =0.02)

Without capture effect (a =0.2)
With capture effect          (a=0.2)
Theory                         {a =0.2)

—J
o
:
¢a| $e

Throughput

10°                                      10°                                       10°                   .                  10°
Offered traffic

를 그림 6.25 Ske npisMAd 제공된 트래픽과 전송률

351



===== PAGE 354 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

Without capture effect (a = 0.02)
With capture effect {a= 0.02)
Without capture effect (a = 0.2)
With capture effect (a =0.2)

1500  .  가  eT  Sr  ert
+           |    T

e odo

8
rT

Average delay time (packet)

Offered traffic

를 그림 6.26 SEAH npisMaAq 제공된 트래픽과 평균 전송지연

RX 결론

이 FINE 이동통신을 위한 몇 가지 전형적인 프로토콜과 컴퓨터 시물레이션을 통
해 전송률과 평균 전송지연을 평가하는 방법을 소개했다. 논의된 프로그램을 기반으로,

독자는 자신만의 새로운 프로토골을 en 성능음

토콜과 비교해 볼 수 있다.

ot

가하고그 결과를 일반적인 프로

352



===== PAGE 355 =====
sas 프로토콜

1) Prasad, R., CDMA for Wireless Personal Communications, Norwood, MA: Artech House,
1996.

2) Abramson, N., “The ALOHA System-Another Alternative for Computer Communications,”
Proc. Fall Joint Computer Conference (AFIPS), Vol.37, 1970, pp.281-285.

3) Kleinrock, L., and F. A. Tobagi, “Packet Switching in Radio Channels, Part I-Carrier Sense
Multiple Access Nodes and Their Throughput-Delay Characteristics,” IEEE Trans. Comm.,
Vol.23, December 1975, pp.1400-1416.

4) Tobagi, F. A., and Kleinrock, “Packet Switching in Radio Channels: Part II-The Hiddel Terminal
Problem in Carrier Sense Multiple-Access and the Busy Tone Solution,” IEEE Trans. Comm.,
Vol.23, December 1975, pp.1417-1433.

5) Krebs, J., and T. Freeburg, “Multiple and Apparatus for Communicating Variable Length
Messages Between a Primary Station and Remote Stations at a Data Communication System,”
US. Patent No.4519068, 1985.

6) Zdunek, K. J., D. R. Ucci, and J. L. Locicero, “Throughput of NonPersistent Inhibit Sense
Multiple Access with Capture,” Electron. Lett., January 1989, pp.30-32.

7) Prasad, R., and J. C. Amnbak, “Capacity Analysis of NonPersistent Inhibit Sense Multiple
Access in Channels with Multipath Fading and Shadowing,” Proc. 1989 Workshop on Mobile
and Cordless Telephone Communications, IEEE, King’s College, University of London,
September 1989, pp.129-134.

8) Prasad, R., “Throughput Analysis of Non-Persistent Inhibit Sense Multiple Access in Multipath
Fading and Shadowing Channels,” European Trans. on Telecommunications and Related
Technologies, Vol.2, May-June 1991, pp.313-317.

9) Prasad, R., “Performance Analysis of Mobile Packet Radio Networks in Real Channels with
Inhibit Sense Multiple Access,” IEE Proc.-I, Vol.138, No.5, October 1991, pp.458-464.

10) Prasad, R., and C. Y. Liu, “Throughput Analysis of Some Mobile Packet Radio Protocols in
Rician Fading Channels,” IEE Proc.-I, Vol.139, No.3, June 1992, pp.297-302.

11) Widipangestu, I., A. J. ‘t Jong, and R. Prasad, “Capture Probability and Throughput Analysis of
Slotted ALOHA and Unslotted np-ISMA in a Rician/Rayleigh Environment,” IEEE Trans. on
Vehicular Technology, Vol.43, August 1994, pp.457-465.

353



===== PAGE 356 =====
최신 이동통신시스템

354

Mobile Communications using MATLAB Simulation

12) Abramson, N., “The Throughput of Packet Broadcasting Channels,” IEEE Trans. Comm.,
Vol.25, January 1977, pp.117-128.

13) Tanenbaum, A. S., Computer Networks, Englewood Cliffs, NJ: Prentice Hall, 1989.

14) Rom, R., and M. Sidi, Multiple Access Protocols Performance and Analysis, New York:
Springer-Verlag, 1990.

15) Spragins, J. D., J. L. Hammond, and K. Pawlikowski, Telecommunications Protocols and
Design, Reading, MA:Addison-Wesley, 1991.

16) Sunshine, C. A., Computer Network Architecture and Protocols, New York: Plenum Press,
1989.

17) Schwartz, M., ComputerCommunications Network Design and Analysis, Englewood Cliffs,
NJ: Prentice-Hall, 1977.

18) Arnbak, J. C., and W. van Blitterswijk, “Capacity of Slotted ALOHA in Rayleigh-Fading
Channels,” IEEE J. Selected Areas in Comm., Vol. SAC-5, No.2, February 1987, pp.261-269.

19) Tsybakov, B. S., “Survey of USSR Contributions to Random Multiple Access
Communications,” IEEE Trans. Inf. Theory, Vol.IT-31, No.2, March 1985, pp.143-165.

20) Nijhof, J. A. M., R. D. Vossenaar, and R. Prasad, “Stack Algorithm in Mobile Radio Channels,”
Proc. IEEE 44th Vehicular Technology Conference, Stockholm, Sweden, June 1994, pp.1193-
1197.

21) Roberts, L. G., “Dynamic Allocation of Satellite Capacity Through Packet Reservation,” Proc.
National Computer Conference (AFIPS), Vol.42, June 1973, pp.711-716.

22) Crowther, W., et al., “A System for Broadcast Communications: Reservation ALOHA,” Proc.
Sixth Hawaii International Conference on System Sciences, January 1973, pp.371-374.

23) Binder, R., et al., “A Dynamic Packet-Switching System for Satellite Broadcast Channels,”
Proc. IEEE International Conference on Communications, San Francisco, CA, June 1975,
pp.41.1-41.5.

24) Goodman, D. J., and S. X. Wei., “Fast Affecting the Bandwidth Efficiency of Packet
Reservation Multiple Access,” Proc. 39th IEEE Vehicular Technology Conference, San
Francisco, CA, May 1989, pp.292-299.

25) van den Broek, C., D. Sparreboom, and R. Prasad, “Performance Evaluation of Packer
Reservation Multiple Access Protocol Using Steady-State Analysis of a Markov Chain Model,”
Proc. COST 227/231 Workshop, Limerick, Ireland, September 6-10, 1993, pp.454-462.

26) van den Broek, and R. Prasad, “Effect of Capture on the Performance of the PRMA Protocol in
an Indoor Radio Environment with BPSK Modulation,” Proc. IEEE 44th Vehicular Technology
Conference, Stockholm, Sweden, June 1994, pp.1223-1227.



===== PAGE 357 =====
다중접속 프로토콜

27) Prasad, R., and J. C. Ambak, “Enhanced Throughput in Packet Radio Channels with
Shadowing,” Electron. Lett., Vol.24, August 1988, pp.986-988.

28) Kasahara, H., S. Hara, and N. Morinaga, “Modeling and Simulation Analysis of Indoor Packet
Radio Communication Systems,” IEICE Trans. Fundamentals, Vol.J78-A, No.8, August 1995,
pp.947-956.

29) Prasad, R., Universal Wireless Personal Communications, Norwood, MA: Artech House, 1996.

355



===== PAGE 358 =====
1 최신 이동통신시스템
     Mobile Communications using MATLAB Simulation

부록 6ㅅ

생성되는 패킷의 $7} Poisson 분포를 따를 때 단말기가 시간 에 /개의 패킷을 생
성할 확률을 (6ㅅ.1)에 보인다.

80=쁘

(6A.1)

그리고 생성간격은 지수분포가 되기 때문에 생성간격의 기대값은 4 이 된다. 시간
0에서 의 기간 동안 패킷이 생성되지 않을 확률은 다음과 같다:

Py(t)=e™                              (6A.2)
그래서 첫 번째 패킷이 시간 ¢ 후에 생성될 확률은 다음과 같다:

20)0=1-@ ^”                                    (6A.3)

(6&.3)에서 모든 트래픽, 접속단말기의 수, 한 패킷을 전송하는 시간, 패킷 생성간격
의 기대값을 각각 GC, 44 sums 7. , 7 , 으로 표현했고 t= 7', 이고     L
이다. 확률 /(/)는 다음과 같다:

®

@=—2
Agel”            (6A.4)

(AAA, T ine 다음과 같이 구해진다.

356



===== PAGE 359 =====
7  = os     Tid.

별  log| 1- 2
ae        (6A.5)

시뮬레이션에서, 패킷의 생성시간이 필요하다. 이 시간은 에서 (64.6) 2 = 구해
진다.

Tn                                   (6A.6)
마지막으로, 패킷의 생성시간을 구할 수 있다.
t =-T,,, x log(1— x)                                   (6A.7)

위 수식에서 0보다 크고 1보다 작은 균일 랜덤 수가 *로 주어진다.

357



===== PAGE 360 =====
R 최신 이동통신시스템
Mobile Communications using MATLAB Simulation

부록 66

순수 ALOHA, 슬롯화된 ALOHA, 비영속적 CSMA, 슬롯화된 비영속적

6B.1 순수 ALOHA

생성되는 패킷의 수가 Poisson CLS 따른다고 가정했기 때문에 한 단위시간에 생
성되는 패킷 수의 ARS /라고 할 때, 시간 ?동안 7/개의 패킷이 생성될 확률은
(68.1)과 같이 주어진다.

00"

ae                        (6B.1)

한 패킷을 전송하기 위한 시간을 라고 정의하면, 트래픽 는 다음과 같다:
G=Ar                                 (6B.2)

사용자 단말기에서 시간 £9 생성된 BAS 사용자 단말기로부터 접속지점에 성공
적으로 전송한다는 것은 다른 단말기가 시간 7 ㅡ- <에서 ,+ ?까지 어떤 패킷도 전송
하지 않음을 의미한다. 순수 ALOHA 시스템에서는, 단말기에서 패킷이 생성되면 패킷
은 접속지점으로 즉시 전송된다. 그래서 사용자 단말기에서 생성된 HAS 접속지점
에 성공적으로 전송할 확률 2 。, 는 시간 2;동안 어떤 HAE 생성되지 않을 확률과

같다.
-247        0
=          ge     (242)   SOA 290얼

358



===== PAGE 361 =====
전송률 6는 접속지점으로 단위시간 내에 ASHE 패킷 수의 기대값으로 표현된다.
그래서 그 값은 다음과 같이 주어진다.

S=GP.. = (60679                          (68.4)

succ

6B.2 슬롯화된 ALOHA

사용자 단말기에서 생성된 패킷을 접속지점에 성공적으로 전송하기 위해 패킷은 각
시간슬롯에 전송된다. 그래서 사용자 단말기에서 생성된 패킷을 접속지점에 성공적으
로 전송할 확률 7? .,, 는 슬롯화된 408 시스템의 시간슬롯을 rH SAHA cS
안 다른 패킷을 생성하지 않을 확률과 같다.

~ (Ar)?       -47

고 PO Sean A              (6B.5)
그래서 전송률 Se 다음과 같다:
S =GP,,,, =06                          (6B.6)
위의 전송률은 시간슬롯 동안 단지 패킷 하나만을 생성할 확률과 같다.
FY 하버 gm a,
1!                                          (6B.7)

6B.3 비영속적 CSMA

비영속적 08\0ㅅ에서는, 사용자 단말기에서 생성된 패킷은 반송파 감지가 “1016”이
된 후에 접속지점으로 전송된다. CSMA 타이밍을 그림 08.1에 보였다.

359



===== PAGE 362 =====
a

최신 이동통신시스템

360

Mobile Communications using MATLAB Simulation

|
om                     Cycle                   ple                      Cycle

때   Busy period         Idle period} Busy period         Idle period
Be

1             a+Y                             1             a
Terminal 1                                                         |                     ㅣ                           |  —>

a 서          수                            Normalized time

-                                                           a
ia                                                                                           Normalized time
Y

Terminal 2

를 그림 68.1 비영속적 CSMA 타이밍

여기서, “busy” 시간의 시간길이의 기대값을 BE 그리고 “idle” 시간의 시간길이의
기대값을 {로 정의하고 충돌이 일어나지 않고 패킷이 성공적으로 전송되는 시간길이
의 기대값을 (/라고 정의하면 전송률 6는 다음과 같이 주어진다.

re   U
B+I                                (6B.8)

위 수식에서 각 패킷의 길이는 정규화되어 1로 정의되었고 패킷을 전송하기 위한 전
SAAS 4로 정의되었다. 그래서 사용자 단말기에서 시간 《에 생성된 패킷을 사용
자 단말기로부터 접속지점에 성공적으로 전송할 확률은 《,에서 7, + 2까지의 기간 동
안 다른 어떤 패킷도 생성하지 않을 확률과 같다. 그래서 충돌이 일어나지 않고 성공적
으로 패킷을 전송할 시간길이의 기대값 UE 다음과 같다.

U = (676 “^                                 (68.9)

/로 정의된 “idle” 시간의 시간길이의 기대값은 지수분포
음과 같이 주어진다.

fut

따른다. 시간길이는 다



===== PAGE 363 =====
G                                (6B. 10)

tA t+ 4까지의 기간 동안 ASS 마지막 패킷의 AS NS 4+ VY BAS
하고 의 기대값을 라고 정의했을 때, BE 정의된 “busy” 기간의 시간길이의 기
대값은 다음과 같다.

B=1+a+Y¥             (6B.11)
YO] 분포함수가 다음과 같이 주어지기 때문에

F,(y) = Pr{Y < y} = Pr{no arrival occurs in an interval of length a-y}

=e (V6         (y Sa)
(6B.12)
의 기대값 는 다음과 같다.
faor-e%
serrate)            (6B.13)
이들을 정리하면 다음 전송률을 얻는다

i       Ge

G(1+2a)+e                        (6B.14)

68.4 슬롯화된 9S ISMA

그림 68.2로부터, idle 시기의 길이는 최소한 한 시간슬롯이다. idle 기간이 단지 한
슬롯일 때, 이는 1016 기간의 첫 번째 슬롯에 최소한 하나의 수신이 YES 의미한다.

361



===== PAGE 364 =====
최신 이동통신시스템
Mobile Communications using MATLAB Simulation

Unsuccessful transmission

Successful transmission
Terminal 1           Base station Terminal 1 Terminal 2           Base station
——_|
se cs Le NS agian 9 Oeia-----
2 아어                     7\{*                                   H
P
d=-—
Ty
--> Idle
|. 기                       Rais                                        pea 8 Busy
‘.-——                      l4---—  75060

를 그림 68.2 슬롯화된 비영속적 ISMA 패킷 타이밍

슬롯이 되려면 첫 번째 슬롯에 수신이 없고 두 번째 SE 최소한 하나의

기간이 두
수신이 존재해야 한다. 이런 식으로 계산하고 2018501 스케줄링을 고려하면 다음을 얻

는다.

> 개
(68.15)

롯에서 전송이 스케줄 되면
롯에 하나 이상의 수신이 존재

으

Ae 《&전송기간을 포

동일한 슬롯 내에 두개 이상의 패킷이 수신되고 다음 슬
충돌이 발생한다. 만약 &-ㅡ1 전송기간의 각 첫 번째 슬롯
하고 번째 전송기간의 마지막 슬롯에 수신이 없다면, busy 7]
함할 것이다. 그래서 busy 기간은 다음과 같다.

l+d
Boe                                   (6B.16)

ewe



===== PAGE 365 =====
B
U=——P
teas =                    (6B.17)

위 식에서 『,,, 는 성공적인 전송기간의 확률이다. 그 값은 다음과 같다.

_ Pr{single arrival within a slot} _ 4006 1“
“<  Pr{more arrivals within a slot} 1-—e-%           (6B.18)

정리하면 전송률은 다음과 같이 얻을 수 있다.

on ee dGe~*
“el led      (6B.19)

363



===== PAGE 366 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

부록 6ㅇ

프로그램 6.1
% Program 6-1
$ main.m
%
% Packet communication system
%
% MATLAB version
% Programmed by M.Okita
% Checked by H.Harada
%
clear;

% definition of the global variable
global STANDBY TRANSMIT COLLISION PERMIT
global Srate Plen Ttime Dtime
global Mnum Mplen Mstime Mstate
global Tint Rint
global Spnum Splen Tplen Wtime

STANDBY    = 0;              % definition of the fixed number
TRANSMIT   = 1;
COLLISION = 2;
PERMIT    = 3;
% definition of the protocol
protocol = { 'paloha'    Pater     % Pure ALOHA      : pno = 1
"saloha'    re     % Slotted ALOHA   : pno = 2
"npcsma'    ee     % np-CSMA         : 600 .= 3
"snpisma'   se     % Slotted np ISMA : pno = 4

}e

oe

definition of communication channel
bit rate

symbol rate

length of a packet

normalized propagation delay

decline fixed number of propagation

brate = 512e3;
Srate = 256e3;
Plen = 128;
Dtime = 0.01;
alfa = 3;

00 00 00 oP

ole

364



===== PAGE 367 =====
loss

sigma = 6;               %
%

x   = 100;                   %
%

ten = 10;                    %
%

Mnum = 100;                 %

men   = 30;                  %
%

pno     = 1;

capture = 0;

spend   = 10000;

outfile = 'test.dat';

Ttime = Plen / Srate;

mpow = 10%*(mcn/10)

fid = fopen(outfile,'w');

fprintf (fid, 'Protocol
fprintt (fid,
fprintL (fi,
Eprinti (fad,
forintt (iid,
Eprints (fid,
forint sr (fad,
fprintf£ (fad;
fprantf (fid,
fpEInte.(fid,

"Capture

"Normalize delay time

standard deviation of shadowing [dB]

definition of the access point
service area radius [m]
position of the access point
(x,y, 2) [m]

capture ratio [dB]

definition of the access terminals
number of the access terminal

C/N at the access point when
transmitted from area edge

% simulation condition

% protocol number

% capture effect O:nothing
1:consider

%® number of packets that

% simulation is finished

% result output file name

% transmission time of one packet

* sqrti(r*2+bxy (3)%Z) Salsas

% true value of C/N

$d\n',pno) ;
$d\n',capture) ;
$f\n',Dtime) ;

"Bit_rate           (bps) = %d\n',brate) ;
"Symbol rate        (sps) = %d\n',Srate);
"Length_of_ Packet   (651) |= %d\n',Plen) ;
"Number of mobile station = %d\n',Mnum) ;
‘Transmission power (C/N) = %f\n',mcn);
"Capture ratio       (dB) = %f\n',tcn);

"Number of Packet

$d\n',spend) ;

fprint£("\n********* Simulation Start *****4***\n\nh)'s
if capture == 0
fprintf(' %s without capture effect\n\n',char (protocol (pno) ));

else

fprintf(' %s with capture effect\n\n',char (protocol (pno)));

365


===== PAGE 368 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

end
mxy = position(r,Mnum, 0);           % positioning of the
% access terminals
randn ('state',sum(100*clock) ) ;       % resetting of the
% random table
mrnd = randn(1,Mnum) ;                % decision of the shadowing
for 6=102118971 1371.20 2212]          % offered traffic
if G >= Mnum
break
end
Tint = Ttime / log(1-G/Mnum) ;
% expectation value of the packet generation interval
Rint -= Tangy
% expectation value of the packet resending interval
Spnum = 0;
Splen = 0;
Tplen = 0;
Wtime = 0;

now_time = feval (char (protocol (pno) ),~1);
% initialize of the access terminals

while 1
next_time = feval (char (protocol (pno) ),now_time) ;
if Spnum >= spend

break
end
idx = find(Mstate==TRANSMIT | Mstate==COLLISION) ;
if capture ==                      % without capture effect

if length(idx) > 1
Mstate (idx) = COLLISION;   % collision occurs
end
else                               % with capture effect
if length(idx) > 1
dxy = distance (bxy,mxy(idx,:),1);
% calculation of the distance
pow = mpow * dxy.*-alfa .*
10.* (sigma/10*mrnd (idx) ) ;
% calculation of received power

366



===== PAGE 369 =====
end

now_

end

traffic

{maxp no] = max (pow);
if Mstate(idx(no)) == TRANSMIT
if length(idx) == 1
cn = 10 * 1logl0(maxp) ;
else
cn = 10 * 1ogl10(maxp/ (sum (pow) -maxp+1) ) ;
end
Mstate (idx) = COLLISION;
if cn >= tcn
% received power larger than capture ratio
Mstate(idx(no)) = TRANSMIT;
% transmitting success
end
else
Mstate (idx) = COLLISION;
end
end

time = next_time;
% time is advanced until the next state change time

= Tplen / Srate / now_time;

% calculation of the traffic

ts

= theorys(pno,traffic, Dtime) ;

% calculation of the theory value of the throughput

fprintf (fid, 'Sf\tSf\ts£E\tsF\tsf\tsf\tt£\n',G,now time
,Splen/Srate,Tplen/Srate, Wtime, Tint, Rint) ;

fprintf ('G=%f\tS=%f£\tTS=%f\n', traffic, Splen/Srate/now_time,ts) ;

end

fprint£ ('\n********** Simulation End **********\n\n") ;

fclose (fid);

graph (outfile);

SEZSELEEEEEEEEEESSESESS Cnd Of File %%3%%3%S%3SFSSSOSSSSSSSSSSSSS

프로그램 6.2

% Program 6-

% positon.m
2
ㅇ

2

367



===== PAGE 370 =====
최신 이동통신시스템

368

Mobile Cammunicaiions using MATLAB Sinmufation

% Positioning of the access terminals in the area of the radius r.

%
% Input arguments
%   13     : The radius r that an access point is an origin.
%   n     : The number of access terminals.
%   h     >: h=0 > z=0 h=1 > z=1~4
%
% Output argument
%   posxy + (x, ypz)
%
% Programmed by M.Okita
% Checked by H.Harada
%
function [posxy] = position(r, n, h)
ms ="4°* xr;                       % calculation of the number of
% maximum position
ms = ns +24>* sum(txs (sqrt (r%2-(1e ri. 42)))2
if n>ms
error('n exceeds the number of position.');
end
posxy = zeros (n, 3);               % initialize

for ii=l1:n

while 1
xX = round(r*rand) * sign(sin(2*pi*rand) );
% x and y are decided at random
yy = round(r*rand) * sign(cos(2*pi*rand) );

Lf xx*2+yy*2 <= r*2 & (xx~=0 | yy~=0)
% (xx,yy) is not (0,0) in the area
if length (find (posxy(:,1)==xx & posxy(:,2)==yy)) == 0
% (xx,yy) are vacant
break
end
end
end
posxy(ii,{1 2]) = [xx yy];
if h ==
while 1
posxy(ii,3) = round(50*rand) / 10;



===== PAGE 371 =====
if 1 <= posxy(ii,3) & posxy(ii,3) <= 4
break
end
end
end
end

SESEEEESESESEESESSESSSSFE End Of File SBESSSSISSSSEEEESSSESESSSSESESESS

프로그램 6.3
% Program 6-3
distance.m

00 00

The calculation of distance between access point and
access terminal.

Input arguments
bstn : coordinate of access point (x,y,z)
mstn : coordinate of access terminals(x,y,z) (mstn is vector
or matrix)
stp : scale (if stp is omitted, scl=1.))

Output argument
이    : distance

00 00 00 00 AP 00 00 00 00 00 Oo?

oe

Programmed by M.Okita
Checked by H.Harada

00 de

ole

function [d] = distance(bstn, mstn, scl)

if Nargin- < 3                        % stp is omitted
sel<= "1;
end

{v,h] = size(mstn) ;
da       sqrt (sum (rot90 (((repmat (bstn,v,1)-mstn) *scl) .*2)));

oe

SECEEESSEESEEESSSSSSS End OF File BSSSSBTESSSEEEEFESSESSEEBSSESESESS

18
Hu
(J

램 6.4

Program 6-4

oe

oe

theorys.m

369



===== PAGE 372 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

%

% The calculation of the theory value of the throughput
%

% Input arguments

%   no : protocol number         1 : Pure ALOHA

%                                 2 : Slotted ALOHA

%                            3 : npCSMA

%                                 4 : Slotted np-ISMA

%   9   : offered traffic (scalar or vector)

%   a   : normalized propagation delay

%

% Output argument

%   ts : the theory value of the throughput (scalar or vector)
%

% Programmed by M.Okita

% Checked by H.Harada

%

function [ts] = theorys(no,g,a)

switch no

case 그                           % Pure ALOHA
ts = 0. <* exp (-2*q);
case 2                           % Slotted ALOHA
ts =g .* exp(-g);
case 3                           % NonPersistent Carrier Sense

% Multiple Access
ts = 9 .* exp(-atg) ./ (g* (1+2*a) +exp (-a*g) );
case 4                           % Slotted NonPersistent ISMA
ts =a * 9 .* exp(-a*g).../ (l+aexp(-a*g));
end

SSSESESEESSSESSSSSSESS End OF File -웅응옹융융융옹옹옹웅응웅옹옹옹옹웅웅옹옹옹웅옹옹옹옹웅웅응웅

프로그램 6.5
% Program 6-5
% graph.m
%
% The function of drawing the graph of simulation result.
%
% Input argument
%   filename : name of the file which simulation result was stored.
%

370



===== PAGE 373 =====
Output argument
nothing

Programmed by M.Okita
Checked by H.Harada

00 00 00 00 00 00

function graph (filename)

mtitlel = {'Throughput of Pure ALOHA system'
% definition of the title
"Throughput of Slotted ALOHA system!
"Throughput of np CSMA system'
‘Throughput of Slotted np ISMA system'
}
mtitle2 = {'Average Delay time of Pure ALOHA system’...
% definition of the title
"Average Delay time of Slotted ALOHA system'
"Average Delay time of np CSMA system'
"Average Delay time of Slotted ISMA system'

2

fid      = fopen(filename,'r');
nul      = fscant(fid,-ss",2);
protocol = fscanf(fid,'td',1);
nul      = fscanf (fid, '%s',2);
caputre = fscanf(fid,'%d',1);
nul      = fscanfi(fid, 3s"; 2)
dtime    = fscanf (fid,-"%f",1);7
nul      = fscanf (fid, 'ts',2);
brate    = fséant (fid, 'td',1);
nul      = fecanf (fid, "%s', 2);
srate    = fscanf (fid, 'td',1);
nul      = fscanf (fid,'%ts',2);
plen     = fscanf(fid,'%d',1);
nul      = £scant (fia, ts", 고)?
mnum     = fscanf(fid, '%td';,1) >
nul      = fscanf(f£id, ts';,2) ;
men      = fscanf (fid, "sf", 1);
nul      = fscanft (fid) 80 7207
ten      = f£scanf (fid, 'sf",1);
nul      = fscan£ (fid,*ts"; 2);
spend    = fscanft(fid, 'sd";1);

371



===== PAGE 374 =====
최신 이동통신시스템

372

Mobile Communications using MATLAB Simufation

Lax = 0;
while 1

dataO = fscanf(fid,'%f',1);

datal = fscant (£id,“ tf", 1);
data2 = fscanf(fid; 4f'; 1);
data3 = fscanf (fid, "%£",1);
data4 = fscanf(fid,'%f',1);
data5 = fscanf(fid,'%f',1);
data6 = fscanf(fid,'%f',1);
if feof(fid) == 1                      % eof
break
end
idx = 13087 17
tg(idx) = data0;                       % offered traffic
g(idx) = data3 / datal;               % actual offered traffic
s(idx) = data2 / datal;               $ actual throughput
w(idx) = data4 / spend * srate / plen;

end

fclose(fid);

% average delay

ts = theorys (protocol,g,dtime) ;            % calculation of the

if protocol < 3

% throughput

% Pure ALOHA & Slotted ALOHA

plot (9,8, "bes" 75,55; S             % normal graph
legend('result', 'theory',0);           % legend
else                                % npCSMA & Slotted np-ISMA
semilogx.(g; 8, “bos: 0;,-ts;,"r") 7          % semi log graph
if protocol ==                         % legend
legend(strcat('result (a=',num2str(dtime),')'),'theory',0);
else
legend(strcat('result (d=',num2str(dtime),')'),'theory',0);
end

end

title (char (mtitlel (protocol) ),'FontSize',16);

% title

xlabel ('Traffic(Simulation result)','FontSize',14);

% x axis label



===== PAGE 375 =====
ylabel ('Throughput', 'FontSize',14);
% y axis label

figure (2);                    % preparation of the new graph windos
iE protocol < 3               % Pure ALOHA & Slotted ALOHA
plot(g,w, 'bo:');               % normal graph
legend('result');              % legend
else                              % npCSMA & Slotted np-ISMA
semilogx(g,w,'bo:');           % semi log graph
if protocol == 3               % legend
legend(strceat('result (a=',num2str(dtime),')'),0);
else
legend(strceat (‘result (d=',num2str(dtime),')'),0);
end
end
title (char (mtitle2 (protocol) ),'FontSize',16);
% title

xlabel ('Traffic(Simulation result) ', 'FontSize',14);
% x axis label

ylabel('Average Delay time (packet)', 'FontSize',14);
% y axis label

용응옹웅옹웅옹육옹웅옹웅옹웅융응웅웅응웅옹응 End OF Lile %%%%3333%3S%33S%SESSSBSSSSESESS%

프로그램 6.6
% Program 6-6
% paloha.m
%
% Pure ALOHA System
%
% Input argument
% now time : now time but, now_time<0 initializes the access
% terminals
%
% Output argument
% next_time : next state change time
%
% Programmed by M.Okita

Checked by H.Harada

oe

ole

function [next_time] = paloha(now_time)

373



===== PAGE 376 =====
최신 이동통신시스템

ot

Mobile Communications using MATLAB Simufation

global STANDBY TRANSMIT COLLISION                   % definition of
the global variable

global Srate Plen

global Mnum Mplen Mstate

global Tint Rint

global Spnum Splen Tplen Wtime

persistent mgtime mtime        % definition of the static variable
if now_time < 0                % initialize access terminals

rand('state',sum(100*clock));       % resetting of the random
table

mgtime        = Tint * log(l-rand(1,Mnum) ) ;

% packet generation time
mtime         = mgtime;             % packet transmitting time
Mstate        = zeros (1,Mnum) ;

Mplen (1:Mnum)
next_time
return

end

Plen;               % packet length
min (mtime) ;

idx = find(mtime==now_time & Mstate==TRANSMIT) ;

% finding of the terminal which transmission succeeded
if length(idx) > 0

Spnum       = Spnum + 1;

Splen       = Splen + Mplen (idx) ;

Wtime       = Wtime + now_time - mgtime (idx) ;

Mstate (idx) = STANDBY;

mgtime (idx) = now_time - Tint ^ log(l-rand);
% next packet generation time

mtime (idx) = mgtime (idx) ;

% next packet transmitting time
end

idx = find(mtime==now_time & Mstate==COLLISION) ;
% finding of the terminal which transmission failed
if length(idx) > 0
Mstate (idx) = STANDBY;
mtime (idx) = now_time - Rint ^ log(l-rand(1,length (idx) ));
% resending time
end

idx = find (mtime==now_ time) ;

374



===== PAGE 377 =====
5 ㅇ Fig

% finding of the terminal which transmission start
if length(idx) > 0

Mstate (idx) = TRANSMIT;
mtime (idx) = now_time + Mplen(idx) / Srate;
% end time of transmitting
Tplen       = Tplen + sum(Mplen (idx) );
end
next_time = min(mtime) ;                % next state change time

SESEESEEEEESESSESESSEESES End Of File 웅웅응응융융융융융융융융융융융융융웅융융융융융융융융융융융음

프로그램 6.7
% Program 6-7
saloha.m

oe ole

00

Slotted ALOHA System

00 00

Input argument
now_ time : now time   but, now_time<0 initializes the
access terminals

00

oP

Output argument
next_time : next state change time

Programmed by M.Okita
Checked by H.Harada

oP 00 00 00 00 00 00

function [next_time] = saloha(now_time)

global STANDBY TRANSMIT COLLISION
% definition of the global variable
global Srate Plen
global Mnum Mplen Mstate
global Tint Rint
global Spnum Splen Tplen Wtime

persistent mgtime mtime slot
% definition of the static variable

if now_time < 0                       % initialize access terminal
rand('state',sum(100*clock) );           % resetting of the

375



===== PAGE 378 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

% random table

slot          = Plen / Srate;           % slot length
mgtime        = Tint * log(l-rand(1,Mnum) );
% packet generation time
mtime         = (fix(mgtime/slot)+1) * slot;
% packet transmitting time
Mstate        = zeros (1,Mnum) ;
Mplen(1:Mnum) = Plen;                   % packet length

"

next_time       min (mtime) ;
return

end

idx = find(mtime==now_time & Mstate==TRANSMIT) ;     % finding of the
terminal which transmission succeeded
if length(idx) > 0

Spnum       = Spnum + 1;

Splen       = Splen + Mplen (idx);
Wtime       = Wtime + now_time - mgtime (idx) ;
Mstate(idx) = STANDBY;
mgtime (idx) = now_time - Tint * log(l-rand) ;
% next packet generation time
mtime (idx) = (fix(mgtime(idx)/slot)+1) * slot;

% next packet transmitting time
end

idx = find(mtime==now_time & Mstate==COLLISION) ;

% finding of the terminal which transmission failed
if length(idx) > 0

Mstate (idx) = STANDBY;

mtime (idx) = now_time - Rint * log(l-rand(1, length (idx)));
% waiting time
mtime (idx) = (fix (mtime(idx)/slot)+1) * slot;

% resending time
end

idx = find(mtime==now_time) ;

% finding of the terminal which transmission start
if length(idx) > 0

Mstate (idx) = TRANSMIT;

mtime(idx) = now_time + Mplen(idx) / Srate;

% end time of transmitting
mtime (idx)    round (mtime(idx)/slot) * slot;
Tplen         Tplen + sum(Mplen (idx) );

376



===== PAGE 379 =====
end
next_time = min(mtime) ;                 % next state change time
SSSSSSESSSEESSESESSESEES ENA Of File 웅융욱융융응융응융응융응응웅웅응웅웅웅웅웅웅웅웅융웅옹우융웅

프로그램 6.8
% Program 6-8
% npcsma.m

nonpersistent CSMA System
Input argument
now_time : now time but, now time<0 initializes the

access terminals

Output argument         ;
next_time : next state change time

Programmed by M.Okita
Checked by H.Harada

AP 00 00 00 00 00 00 00 00 00 00 00 00

function [next_time] = npcsma(now_time)

global STANDBY TRANSMIT COLLISION

% definition of the global variable
global Srate Plen
global Mnum Mplen Mstime Mstate
global Tint Rint
global Spnum Splen Tplen Wtime

persistent mgtime mtime
% definition of the static variable

if now_time < 0
% initialize access terminals
rand('state',sum(100*clock) );                % resetting of the
% random table
mgtime        = Tint * log(l-rand(1,Mnum) ) ;
% packet generation time

ㅣ

Mstime          zeros(1,Mnum) - inf;

% packet transmitting time

377



===== PAGE 380 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

mtime         = mgtime;              %$ state change time
Mstate        = zeros (1,Mnum) ;
Mplen(1:Mnum) = Plen;

next_time       min (mtime) ;
return

end

idx = find(mtime==now_time & Mstate==TRANSMIT) ;
% finding of the terminal which transmission succeeded
if length(idx) > 0

Spnum       = Spnum + 1;

Splen       = Splen + Mplen(idx);

Wtime       = Wtime + now_time ~ mgtime (idx) ;

Mstate (idx) = STANDBY;

mgtime (idx) = now_time - Tint ^ log(l-rand);
% next packet generation time

mtime (idx) = mgtime (idx) ;

% next packet transmitting time
end

idx = find(mtime==now_time & Mstate==COLLISION) ;
% finding of the terminal which transmission failed
if length(idx) > 0
Mstate (idx)   STANDBY;
mtime (idx)    now time - Rint ^ log(1l-rand(1, length (idx) ));
% resending time

ㅣ

end

idx = find(mtime==now_time & Mstate==STANDBY) ;
% finding of the terminal which carrier sensing
if length(idx) > 0
Tplen = Tplen + sum(Mplen (idx) );
for ii=1: length (idx)
Jer dx (2)
if carriersense(jj,now_time) == 0       % channel is idle
Mstate(jj) = TRANSMIT;
% packet transmitting
Mstime (jj) = now_time;
% start time of transmitting
mtime(jj) = now_time + Mplen(jj) / Srate;
% end time of transmitting
else                            % channel is busy
mtime (jj) = now_time - Rint * log(l-rand);

378



===== PAGE 381 =====
= KO

% waiting time
end
end
end

next_time = min(mtime) ;                % next state change time
SESESSSSESSESESSESSSESFE End Of File 웅웅웅융융옹융육융웅옹응옹웅옹웅옹옹옹웅옹웅옹욱응옹옹응웅웅

프로그램 6.9

Program 6-9

00

carriersense.m

The function of the carrier sense

Input arguments

no       : terminal which carrier sensing

now_time : now time

Output argument
result   7,02 idles Tibusy

Programmed by M.Okita
Checked by H.Harada

oP 00 00 00 00 00 00 dP 00 00 00 00 00 00

function [result] = carriersense(no,now_time)

global Mnum Mstime Ttime Dtime
% definition of the global variable

delay = Dtime * Ttime;
% calculation of the delay time

idx = find((Mstimetdelay)

<=now_time & now_time<=(Mstime+tdelay+tTtime) );

% carrier sense

if length(idx) > 0
result = 1;

carrier is detected
channel is busy

charier can't be detected
channel is idle

00 00

ae

else

oe

result = 0;
end

379



===== PAGE 382 =====
최신 이동통신시스템

380

Mobile Communications using MATLAB Simulation

SSSSTESSESSTSESEEEESEBS ENd Of File SESSSSSSSTESEEEEESEEESEESSSSEBS

프로그램 6.10

%$ Program 6-10
snpisma.m

Slotted nonpersistent ISMA System

00 00 00 00 00

Input argument

now_time : now time   but, now_time<0 initializes the access
terminals

Output argument
next_time : next state change time

Programmed by M.Okita
Checked by H.Harada

dP 00 00 00 00 00 00 00 00

function [next_time] = snpisma(now_time)

global STANDBY TRANSMIT COLLISION PERMIT
% definition of the global variable

global Srate Plen Dtime

global Mnum Mplen Mstime Mstate

global Tint Rint

global Spnum Splen Tplen Wtime

persistent mgtime mtime slot
% definition of the static variable

if now_time < 0                    % initialize access terminals

rand('state',sum(100*clock) );    % resetting of the random table
mgtime        = Tint * log(l-rand(1,Mnum) ) ;

% packet generation time
Mstime        = zeros(1,Mnum) - inf;

% packet transmitting time
mtime         = mgtime;          % inhibit sensing time
Mstate        = zeros (1,Mnum);
Mplen(1:Mnum) = Plen;            % packet length
next_time     = min(mtime) ;      % state change time
slot          = Plen / Srate * Dtime;        % idle slot length
return


===== PAGE 383 =====
end

idx = find(mtime==now_time & Mstate==TRANSMIT) ;

% finding of the terminal which transmission succeeded
if length(idx) > 0

Spnum       = Spnum + 1;

Splen       = Splen + Mplen (idx);
Wtime       = Wtime + now _time - mgtime (idx) ;
Mstate (idx) = STANDBY;
mgtime (idx) = now_time - Tint ^ log(l-rand);
% next packet generation time
mtime (idx) = mgtime (idx);
end

idx = find(mtime==now_time & Mstate==COLLISION) ;
% finding of the terminal which transmission failed
if length(idx) > 0
Mstate (idx) = STANDBY;
mtime (idx) = now_time - Rint * log(lrand(1, length (idx) ));
% resending time
end

idx = find(mtime==now_time & Mstate==STANDBY) ;
% finding of the terminal which inhibit sensing
if length(idx) > 0
Tplen = Tplen + sum(Mplen (idx) );
for ii=1:length (idx)
jj = idx(ii);

if inhibitsense(jj,now_time) == 0        % channel is idle
Mstate (jj) = PERMIT;
[temp1 kk] = max(Mstime) ;

% calculation of the transmitting start time slot
if templ < 0

mtime (jj) = ceil(now_time/slot) * slot;
else

temp1 = templ + Mplen(kk) / Srate;

temp2 = now_time - temp1;

if temp2 < 0

mtime(jj) = templ + slot;
else

mtime(jj) = templ + ceil(temp2/slot) * slot;
end

end

381



===== PAGE 384 =====
최신 이동통신시스템
Mobile Communications using MATLAB Simulation

else                                         % channel is busy
mtime(jj) = now _time - Rint * log(l-rand); % waiting time
end
end
end

idx = find(mtime==now_time & Mstate==PERMIT) ;

% finding the terminal which transmission start
if length(idx) > 0

Mstate (idx)   TRANSMIT;

Mstime (idx)   now_time;

mtime (idx)    now time + Mplen(idx) / Srate;

% end time of transmitting

end

next_time = min(mtime) ;                    % next state change time
웅옹웅응웅옹웅웅웅웅웅웅웅융옹웅웅옹융응웅응응 end of file 웅웅융융융웅옹웅웅웅웅웅웅옹옹웅옹옹웅욱웅옹웅옹웅웅응옹옹응

프로그램 6.11

% Program 6-11
inhibitsense.m

00 de 00

The function of the inhibit sense

00 de

Input arguments
no       : terminal which inhibit sensing
now_time : now time

ae 00

Output argument
inhibit® ..: 0s -idle   1: busy

00 00 00 00 00

Programmed by M.Okita
Checked by H.Harada

00 00

function [inhibit] = inhibitsense(no,now_time)

global Mnum Mstime Ttime Dtime
% definition of the global variable

ㅣ

delay
inhibit

Dtime * Ttime;                % calculation of delay time
0;

il

382



===== PAGE 385 =====
acc KO

idx = find((Mstime+tdelay)<=now_time .

& now_time<=(Mstime+delay+Ttime) ) ;
if length(idx) > 0
idx = find(idx~=no) ;
if length(idx) > 0
inhibit = 1;
end
end

inhibit sensing

except itself
inhibit is detected
channel is busy

SESSSSESSEEESESSEEEEESSESS ENA OF File BESESSESSEESSEESEEEESSSESEFESBS

383



===== PAGE 386 =====


===== PAGE 387 =====
ee ee te

셀룰러 통신시스템

BAM “=

1~6 장에서, 지점 대 AlAl(—pointto-point)Z} 지점 대 CF) 4 (pointto-multipoint)
AS 성능을 다수의 전송방식을 사용하여 평가하였다. 그러나 이동통신시스템에서
기지국은 많은 사용자와 통신한다. 이는 지점 대 지점 ASS 이동통신시스템에서 단지
하나의 기여요인에 지나지 SES 의미한다. 그래서 지점 대 지점 전송의 성능뿐만 of
니라 다중지점 접속방식의 성능을 평가하거나 다수의 독립적인 사용자에 의해 성능이
어떻게 영향 받는지 평가해야 한다. 특별히, 이동통신시스템에서, 높은 주파수 이용 효
율 때문에 셀룰러 통신모델이 흔히 기본적인 접속방식으로 사용된다. 이 장은 실제 At
용되고 있고 높은 시스템 수용능력 (capacity) S 갖는 [1, 2] 셀룰러 통신시스템 모델에
대해 논한다. 시스템 수용능력, 차단확를 혹은 콜의 강제된 종료확률과 같은 전체 시스
템 성능의 평가를 위해 컴퓨터 시뮬레이션의 사용이 필요하다.

셀룰러 시스템에 기반 한 접속방식을 사용하는 한 가지 이점은 이전 장에서 제시된
몇 가지 전송방식과 결합함으로써 진화된 평가를 가능케 한다는데 있다. 사실상, 셀룰
러 시스템 시뮬레이션은 전송파워 제어와 안테나 어레이 기술과 같이 시스템 성능의 근
본적이고 이론적인 분석을 거의 불가능하게 만드는 통신과정의 다른 복잡한 요인과 결

387



===== PAGE 388 =====
a

최신 이동통신시스템

Mobile Communications using MATLAB Simulation

합하여 수행된다.

그래서 본 책에서는 셀룰러 시스템 시뮬레이션의 기본적인 Bas 소개한다. 본 시뮬
레이션에 사용된 몇 가지 기술들은 실제 구현평가에 있어서 필수적이고, 동시에 위에서
언급한 있을법한 상황에 쉽게 적용 가능하다.

셀룰러 통신시스템과 셀간 Zl (intercell interference) 의 기본적인 개념을 7.2장에
서 설명한다. 7.3장에서는, 특정 소프트웨어를 사용하여 셀룰러 시스템의 컴퓨터 시뮬
레이션 Bas 구성하기 위한 몇 가지 주요 기술을 소개한다. 또한, 잘 알려진 채널 할당
방식인 DCAS 이루기 위한 기술을 제시한다. 이 알고리즘을 사용한 시뮬레이션 결과
를 7.4장에 제시한다. 7.5장에서는 어레이 안테나를 사용한 셀룰러 시스템 모델을 기술
한다. 7.6장은 이 장을 결론짓는다. 이 장에 관련된 모든 프로그램은 부록 7ㅅ와 SSA
CD-ROMe] 지시한다.

| 셀룰러 시스템의 개념과 채널할당 알고리즘

388

셀룰러 시스템의 기본적인 개념을 그림 7.1에 보였다. 이 시스템에서, 전체 서비스 영
Ae 다수의 셀이라 불리는 작은 영역으로 분할된다. 각 Ao] 중심에 위치한 기지국은
통화를 시작할 때 셀 내에서 이동 단말기들을 위해 다수의 트래픽 채널을 할당한다. 셀
룰러 시스템의 가장 일반적인 특징 중 하나는 다른 셀들이 충분히 멀리 떨어져 있다면
서로 다른 셀들에서 동일한 트래픽 채널이 동시에 할당될 수 있다는 점이다. 만약 가까
운 셀에서 동일한 채널이 할당되면, 각 셀은 다른 셀에 동일채널 간섭을 야기하고 전송
품질을 저하시킨다. 그러나 같은 채널을 가지는 셀들이 AAS 위치하게 되면, 이 간
섭은 Al 간의 거리에 비례해 약화된다; 전송품질은 이러한 간섭에 의해 저하되지 않고,
전체 시스템의 무선자원은 효과적으로 사용될 수 있다.

그림 7.1에서, 4개의 ASE Ry, Ry, >, ;이고 4명의 사용자는 Ty, Th,

T,, 7:;이다.여기서,사용자 OTS IA Ro 연결되어 있고 4명의 사용자 모두는
동일한 트래픽 채널을 할당 받았다고 가정한다.



===== PAGE 389 =====
셀룰러 동신시스팀 (을

Interference      ch.1

—

: Base station

i : User

Mag 71 셀룰러 시스템 개념

이 가정에 의해, 사용자 Ty ol) 대한 반송파대-잡음+간섭의 비 (0/(4+ 7 ))#,,를
다음과 같이 유도할 수 있다.

$0

1 11000

cnt

3        $i
N+) APd;*10"                    (7.1)

i-l

여기서, <는 경로손실 항목이고, AE 비례계수, PE 사용자 T 9] 전송파워, 4,
는 사용자 7;,와기지국 《,의 거리이다. 또, &는 7:,와 Ry 사이의 새도윙에 의해 of
기된 왜곡인데 (7.1)에서 이 값은 데시벨로 표기된다. (7.1)에서, WA 2,, dy, 4,가
보다 높은 전송품질을 의미하는 보다 높은 C/(N+D 비를 가져옴을 알 수 있다. 그래
A, 예비적인 서비스 SAS 위해 적절한 C/(N+D 비를 달성하기 위해서 몇 가지 채
널할당 알고리즘이 현재의 시스템에서 사용 중이다.

이러한 채널 할당 알고리즘의 두 주요 예로써 FCAS} 004가 있다[3]. 804는 기지
국 당 고정된 채널 할당을 수행하는 알고리즘이다. 804의 예를 그림 7.2에 보였는데,
셀내의 사용자가 다른 셀로부터 최소의 동일채널 WAS 받도록 각 기지국에 4개의 채
널을 할당했다. 반면, ㅁ@4의 경우, 기지국은 시스템의 모든 AWS 조정할 수 있고 간
MAUL 최소화하기 위해 적당한 채널을 동적으로 할당한다.

389


===== PAGE 390 =====
A

최신 이동통신시스템

390

Mobile Communications using MATLAB Simutation

를 그림 7.2 FCA 알고리즘 개념

DCAS] 개념을 그림 7.3에 보였다. DCA 알고리즘듬은 80쇼보다 높은 수용능력을
달성할 수 있고 트래픽의 변동에 보다 유연하게 대처할 수 있는데, 이는 모든 채널의 사
용자의 요구에 따라 적응적으로 할당되기 때문이다.『(스의 경우, 그림 7.3(8)에서와 같
이, 기지국 당 PAS] 수가 고정적으로 제한되어 있기 때문에 셀 내의 두 번째 사용자는
콜 차단을 경험하게 된다. 반면, 그림 7.3(6)에 보인 바와 같이 DCAS] 경우는, 기지국들
은 모두 적응적으로 할당될 수 있는 채널을 공유하고 이로 인해 FCAMA| 발생하는 콜
차단의 발생을 감소시킨다. 그러나 DCAE FCA 비해 간섭측정과 채널 서칭과 같은

(a)       Call blocking

is       Base station                                 —Channel
:          ㅣ
1      User                                            (C77: Not allocated
^ ; Allocated
Cell

를 그림 7.3 DCA 알고리즘 개념: (3) FCA (b) DCA,



===== PAGE 391 =====
73 | 동적채널할당 시스템의 시뮬레이션 프로그램

이 장에서는 DCA 알고리즘을 사용하는 셀룰러 시스템을 구현하기 위한 시뮬레이션
프로그램을 제시한다. 주 프로그램은 프로그램 7.1에, 부 프로그램은 프로그램 7.27.7
에 보였다. 표 7.1은 각 프로그램의 기능을 정리한 것이다.

R718 프로그램 717.79 기능

프로그램      시뮬레이션에서의 이름                       기능
프로그램 7.1 | dcamain.m                        주 프로그램
프로그램 7.2 | basest.m                          각 기지국의 위치를 결정
프로그램 7.3 | wrap.m                             셀-랩핑을 통해 기지국 위치의 관계 결정
프로그램 7.4 | cellmesh.m                             망에 셀을 분포시키고 각 망 좌표에 대한 데이터를 저장
프로그램 7.5 | holdtime.m                          지수적으로 분포된 콜 홀딩시간을 생성
프로그램 7.6 | shadow.m                    로그정규 분포를 갖는 새도윙에 따른 감쇄 생성
프로그램 7.7 | distm                                    거리에 의한 경로손실 생성

7.3.1 성능측정

프로그램에 대한 자세한 Ags 하기 전에, 시뮬레이션에서의 성능측정에 대한 내용
을 기술할 것이다. 여기서는 차단확률과 강제된 종료확률의 두 가지 측정치에 중점을
두도록 한다. 차단확률은 새로운 콜이 7.2장에서 AFM C/(N+ 2) 비 조건을 만족^
키는 적당한 채널을 찾는데 배기 확률로 정의된다. 비록 차단확률이 새로운
콜에 관련된 측정치이지만, 연결된 콜이 C/(N+ 2) 비 조건의 급격한 저하로 끝마치기
전에 차단될 수 있다. 그래서 강제된 종료확률을 연결된 콜이 종료되기 전에 차단될 확
률로 정의한다. 만약 6310401, blocknum, 107060020을 각각 생성된 콜의 수, 차단된 콜
의 수, 강제된 종료 콜의 수로 정의하면, 동일한 OSS 갖는 변수들을 다음 Ao] 보인
시뮬레이션에서 소개한다. 차단확률 PF 강제된 종료확률 는 다음과 같이 주어
진다:

391


===== PAGE 392 =====
2 최신 이동통신시스템

392

Mobile Communications using MATLAB Simulation

_ blocknum
 callnum                                   (7.2)

peu         forcenum
^ cal\num —blocknum                              (7.3)

이 두 가지 성능측정은 셀룰러 시스템의 몇 가지 잠재적인 평가를 가능케 한다.

7.5.2 전체 시뮬레이션의 흐름도

그림 7.4는 전체 시뮬레이션의 흐름도를 보여준다. 시뮬레이션은 세 가지 부분으로
구성 된다: 준비부분, 메인루프부분, 출력부분. 준비부분에서는, 메인루프 시작 전에 셀
레이아웃이나 트래픽 인자와 같이 시뮬레이션에 필요한 몇 가지 정보부분이 소개된다.

(~

Preparation,
status initialization

Time loop

Finishing call is terminated

Connected call is checked,
if necessary, reallocation

New call arrival and
channel assignment

|
L             Time loop             |
End             >

를 그림 7.4 시뮬레이션

rat
ol
ou
0



===== PAGE 393 =====
셀룰러 동신시스템 (을.

메인루프는 준비된 종료시간 “8106600"를 갖는 01486 루프로 활동을 개시한다. 전
체 루프를 통해, 현재 사용자의 상태가 체크되고 필요하면 짧은 시간간격, 주기
“timestep”, 안에 새롭게 설정된다. 몇 가지 상태지표가 연속적으로 행렬 “0860010”에
저장된다. 표 7.2는 행렬 “0660010”의 내용을 보여준다.

aoe

837.28 “userinfo’o] 저장된 정보

a                    저장된 정보
userinfo(:,:,1)                    사용자의 ※좌표
userinfo(:,:,2)                   사용자의 좌표
userinfo(:,:,3)                   사용자의 경로손실 (연결된 경우)
userinfo(:,:,4)                   0:비연결 1:연결
userinfo(:,:,5)                            2 종료시간
userinfo(:,:,6)      할당된 dus (aad 경우)

루프의 모든 시간주기에서, 각사용자는 상태 행렬에 기반하여 콜 시작, 채널 AA, 채
널할당, 채널 재할당, 콜 SEF 같은 여러 이벤트를 야기한다. 시간주기 안에, 다음 이
벤트가 순서대로 고려된다.

0: 이 주기 안에 통화가 종료되면 연결된 사용자의 콜은 종료된다.

여전히 연결된 사용자의 So] 조사된다. 바람직한 간섭조건이 만족되지 못하면
새로운 채널을 찾아 재 할당을 시도한다.

@ 준비된 확률로, 연결되지 않은 사용자가 새로운 콜을 시작하고 간섭조건을 만족
하는 채널을 찾는다.

® (1)로 되돌아간다.

몇 가지 형태의 수치 데이터 또한 모

더

주기에서 측정된다.
마지막으로, 출력부분에서, 메인루프에서 측정되고 저장된 데이터가 출력행렬

|
“check”, 혹은 “check2” 52 “output” 혹은 텍스트 데이터 “data.txt” 형태로 구성된다.

393



===== PAGE 394 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

7.3.3 셀 레이아웃과 셀-랩핑 기술

그림 7.5는 본 책의 시뮬레이션에서 채용된 셀 레이아웃을 보여준다. 시뮬레이션에
서는 19개의 반지름 1인 6각형 셀을 사용했다. 이러한 셀들은 19개 기지국의 위치에 의
해 결정된다. 기지국의 위치는 프로그램 7.2 “08868[.0^으로 결정되고 이 정보는 19×2
행렬 “608861010”에 저장된다. 예를 들어, “baseinfor(5,1)”2} “baseinfor(5,2)’= 각각 5
번째 기지국의 x, y FES 나타낸다. 시뮬레이션에서, 사용자의 규제된 수는 데이터를
취한 19개 셀들에 분산되어 있다.

Y axis in the
simulation

Ceil (19th cell)

Position of base station
(19th base station)

~ Xaxis
in the
simulation

를 그림 7.5 셀 레이아웃

DCA 알고리즘을 사용하는 셀룰러 시스템의 경우, 이웃 셀들로부터의 SUAS 간
섭이 샘플 셀의 성능에 중요한 SHS 미치므로 하나의 샘플 셀뿐만 아니라 이웃 셀들
을 고려해야 한다. 예를 들어, 5번째 AS 1번째, 4번째, 14번째, 15번째, 16번째, 6번째
셀로부터 간섭 받을 수 있다. 2번째 혹은 3번째 셀과 같이 보다 멀리 떨어진 ASE 5번
째 셀과 간섭할 수 있다. 그러나 이러한 간섭은 거리에 의해 무시할 수 있을 정도로 감소

394



===== PAGE 395 =====
셀룰러 동신시스템 “을

된다고 가정하고, 시물레이션에서 바로 이웃한 6개의 AWS 고려한다. 반면, 셀 레ㅇ
아웃의 경계에 위치한 9번째 셀의 경우, 10번째, 2번째, 8번째의 3개의 이웃한 셀이 존
재한다. 이러한 “경계 셀”은 “안에 위치한 셀”과 다른 성능을 갖는데, 예를 들어 9번째
ALS 9번째 셀에 간섭을 야기하는 Alo] 2번째 셀보다 적기 때문에 보다 나은 성능을 갖
는다. 결론적으로, 내부 셀뿐만 아니라 경계 셀까지 고려하면 DCA 성능을 적절하게 평
가하지 못한다.

그래서 이러한 문제를 피하기 위해, 두 가지 해법이 사용될 수 있다. 하나는 그림 7.5
에서 1번째, 2번째, 3번째, 4번째, 5번째, 6번째, 7번째 Aly} 같이 내부 셀만을 취하고
경계 AS 배제하는 것이다. 이러한 내부 ASS 모두 6개의 이웃 셀들로부터 간섭받기
쉽고 DCA 알고리즘의 효과적인 Ves 밝혀줄 것으로 기대된다. 그러나 경계 AS]
출력 데이터에 기여하지 못하기 때문에, 적절히 평균된 데이터를 얻기 위한 전체 셀 al
이아웃을 구성하기 위해서 보다 많은 셀을 필요로 하고 이는 시뮬레이션 로드를 증가
시킨다.

다른 해결법은 셀-랩핑 기술을 사용하는 것이다. 그림 7.6은 이 기술의 WAS 보여준
다. 이 기술에서는, 경계 AS 거의 정반대인 셀 레이아웃에 위치한 경계 셀의 이웃으로
간주된다. 그림 7.6에서, 단지 19개의 음영이 있는 셀만이 실제로 존재하고 다른 셀들은
동일한 FS 갖는 실제 셀의 복제이다. 결과적으로, 9번째 AS 10번째, 2번째, 8번째
셀로부터의 간섭뿐만 아니라 이웃한 위치에서 13번째, 17번째, 14번째 Alo] 복제에 이
한 간섭의 영향도 받게 된다. 이런 가정 하에, 셀 레이아웃 내의 모든 Ae 6개의 이웃을
갖는 “내부에 존재하는 셀”로 간주될 수 있다.

셀 랩핑을 구현하기 위해, 19x19 행렬 wrapinfo7} 프로그램 \ㅠ82.2에서 생성되고
주 프로그램에서 소개된다. 행렬 wapinfoE 셀 랩핑을 포함한 19 셀의 관계를 yas
다. 그래서 예를 들어, wrapinfo(5,:)= 5번째 셀과 특별히 6개의 이웃인 wrapinfo(5,2)
에서 \『801010(5,7)까지의 다른 셀들과의 관계를 저장한다. (프로그램 7.3과 그림 7.6
참조) 이 행렬의 더 자세한 사용은 후에 설명될 것이다.

ad

395



===== PAGE 396 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

| Real cell                | Copy of real cell

를 그림 7.6 #282 기술 개념

7.3.4 셀 B(mesh) 구성

시뮬레이션에서, 사용자 분포는 전체 셀 레이아웃뿐만 아니라 한 셀 내에서 균일하다
고 간주한다. 이러한 조건은 많은 작은 망에 분포한 셀에 의해 구현된다. 그림 7.7은 시
율레이션에서 사용된 하나의 셀과 망들을 보여준다. 프로그램 610688.0이 시뮬레이
션에서 망 생성기 역할을 하고 A 내의 Yo] +S AF cellnumo 2 출력하고 각 망의
위치를 A ASk= cellnumx22] 행렬 meshpositionS 출력한다. 또한 601016918.0의 결

과를 44411408의 명령줄에서 다음과 같이 볼 수 있다:

396



===== PAGE 397 =====
셀룰러 sania (을

Mesh #meshnum

Jr

Fineness
극 Mesh #2

—— Mesh #1

miad77 셀 내에 형성된 망

>>[meshnum meshposition]=cellmesh;

>>plot (meshposition(:,1),meshposition(:,2),’.’)

그림 7.82 이 결과를 보여주는데 여기서 “Fineness"= 망 정밀도를 나타내는 인자이
며 시뮬레이션에서 보통 “Fineness=50" 9° 2 설정된다. 여기서, 이산 망들은 6각형 셀
과 같이 특별한 형태의 영역에 특정 Yo] EBs 할당하기 위해 사용된다. 만약 큰 값
의 “Fineness” S 사용하면, 이러한 이산 망구조는 그림 7.8에서 기대되는 바와 같이 연
속적인 분포 모델에 가까워진다.

시뮬레이션에서, 사용자가 콜을 시작할 때, 1에서 “meshnum” 사이에서 균일하게 변
동하고 사용자를 셀 내의 “meshposition(mesh,:) 위치로 위치시키는 랜덤 변수 “mesh”
를 생성한다. 결과적으로, 각 사용자는 콜 시작 때 셀 내의 “meshnum” 지점들의 특정
]점에 동일한 확률로 분산되고, 셀 내에서 균일한 사용자 분포를 얻게 된다.

N

397



===== PAGE 398 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

T

T        T     =<      2         T        T       1 에      T

ogt Fineness =50

coordinates
=

=A02F
-0사

0.6}

-1 08 -06 -04 -02 0  0.2 0.4 0.6 0.8  1
X coordinates

1         T        T        T        T       = ag      a       T        T        T

ost    Fineness = 30

0.6

0.4F

02

coordinates
=

>9.2+

0.4

0.6 +

08}     i, Sa roe See     1

es 08 -06 -04 -02 0  0.2 0.4 0.6 08  1
X coordinates

를 그림 7.8 4 패턴 oO

7.5.5 콜의 트래픽 인자

각 콜 생성은 각 사용자의 평균 4 = (arrival rate) “lambda” (calls/hour)=
Poisson 과정을 따른다. 이러한 EASES 구현하기 위해서, 랜덤함수 “8040”를 사용

398



===== PAGE 399 =====
셀룰러 통신시스템 FO

하여 모든 시간주기 “00009062"”에서 연결되지 않은 각 사용자를 검사한다. 만약 “rand”
가 “timestep” 동안 평균 도착속도를 나타내는 “Jambda*timestep//3600” 2t} 크지 않

으면, 사용자는 SS 시작한 것으로 간주되고 생성된 콜의 수는 변수 “0801000^으로 세

반면, 모든 시작된 Se 각자의 유지시간을 갖고 시작된 SBS 이 시간 후에 종료된다.
각 콜의 유지시간은 평균 “ht” (초)를 갖는 지수분포를 갖는다. 시뮬레이션에서, 유지
을 함수 “1010020060810)”의 출력으로 얻었는데 이 함수는 평균 “94”의 지수분

는 랜덤 값을 출력한다. 1010020406011)”는 프로그램 “10100106.0^으로 제공되
고 그림 7.9% MATLABL & 측정된 “holdtime(ht)” 출력의 확률밀도함수(001)를 보

또한, 사용자의 수도 중요한 트래픽 인자이다. 독자는 셀 내에 존재하는 사용자의 수
를 설정할 수 있고 이러한 사용자 수의 변동의 효과를 조사할 수 있다. 후에 보이는 시
뮬레이션 결과에서, 변수 “06@로 밝혀지는 셀 당 사용자 수에 따른 DCA 성능을 평가

x 10°

P(x)

0 100 «©6200 Ss 3300's 400 500 600 700 800 900 1000
Call holding time (seconds)

를 그림 7.9 3 유지시간 pdf

399


===== PAGE 400 =====
A

최신 이동통신시스템

400

Mobile Communications using MATLAB Simulation
7.3.6 전송 조건

희망 B}(desired wave) 혹은 간섭파와 무관하게 수신신호의 ARE 시뮬레이션에서
가장 중요한 논점의 shot AGA ASE 거리와 장애물과 같은 요인에 의해 야기
되는 감쇄를 겪게 된다. 본 책에서는 시뮬레이션에 있어서 이러한 감쇄요인으로 경로손
실과 새도윙을 소개하기로 한다.

전송신호가 (7.1)에서와 같이 《의 감쇄항을 갖는 경로손실을 갖는다고 가정하면 시
뮬레이션에서 이는 변수 “alpha” = 제공되고 “alpha=3.5"= 설정된다. 이 경로손실의
AAS 프로그램 “distm’ 2 = 행해진다. 이 프로그램은 함수 “dist(a,b,alpha)”S 제공
하는데 “8”와 “6”는 1×2 행렬이고 각각 두 지점의 좌표를 나타낸다. 그러면,
“dist(a,b,alpha)”2] 값은 이들 두 지점 a, 6간의 경로손실을 계산한다. 이 책에서는 이
함수의 보다 실제적인 사용법을 후에 기술할 것이다.

또한, 새도윙은 (7.1)의 ㅎ,에 해당하는 표준편차 “sigma’S 갖는 로그정규분포
를 갖는다고 가정한다. 이 “sigma” 시뮬레이션에서 “sigma=6.5"= 설정된다.
본 책에서는 또한 “94800\(51808)”의 함수의 출력으로서 새도윙 XS 얻는데 이
TPE 표준편차 “618008”의 로그-정규분포를 갖는 랜덤 변수를 출력한다. 심볼

“shadow(sigma)” 는 프로그램 “400\.4^으로 제공되고 그림 7.10은 MATLABS =
즉정한 “shadow(sigma)” 44 2] pdfS 보여준다.

09

07

05

P(x)

a4

03

02

01

05               1                15               25
Shadowing attenuation

를 그림 7.10 M&A 감쇄의 pdf


===== PAGE 401 =====
셀룰러 통신시스템 (를

7.3.7 Hees
시뮬레이션에서 채널할당과정에 대해 이 장에서 설명한다. 이 과정은 주 프로그램

“…008200210.02”에서 행해진다.
먼저, 콜시작 사용자로부터 기지국으로의 업 링크 파워 강도가 조사된다. 이 파워는
(//으로 주어진다. 이 C/NS 송신기와 수신기 간의 거리가 1일 때 C/NS 나타내
는 시뮬레이션 인자 “cnedge” (decibels)S 사용하여 제시한다. 그림 7.11은 경로손실
만이 고려된 경우의 이들 조건을 보여준다.

Received power

Power (10, cnedge/10)

;                  Rx
x dist (0, X, alpha)
Tx                     ,       Y
Power (10, cnedge/10)
&                        “we
|                                            Power (10, cnedge/10)
ae                     x dist (0, Y, alpha)
————
<7 E cell radius)               가비
<           독          -
*                 +
0 (0,0)                              X (x,0)            U (1,0)           Y (y,0)

를 그림 7.11 경로손실 조건

프로그램에서는, 먼저 사용자 위치와 기지국의 AHS 입력하고 “dist(here,
there,alpha)”= 경로손실 값을 얻고, 그 다음 이 값에 “shadow(sigma)” = 생성된 새도
윙 감쇄를 첨가한다. 다음으로 프로그램에서 “0\86@”"라 부르는 원하는 ASS] 감쇄 값
을 얻는다. “dwave” 값을 사용해 기지국에서 수신한 신호의 C/NS 얻을 수 있다. 이

C/N 은 “00\60(10.0,0ㅁ6086/10.0)”에 해당하고 “en” 변수로 표현된다.
“on? & 계산한 후에, C/(N+ D2] 간섭조건을 만족하는 사용되지 않고 있는 채널을

401



===== PAGE 402 =====
/ : )   최신 이동통신시스템
C

Mobite Communications using MATLAB Simulation

찾는다. 채널서치는 채널번호 “ch’2] 루프에서 행해져서 전체적으로 제공된 수
(“000402”)의 채널이 검사된다. 만약 다른 사용자가 동일한 채널 “ch” ol] 할당되면, 그
사용자로부터의 간섭을 계산한다. “for around=2:7” 루프에서, 변수 “othercell =
wrapinfo(numcell,around)”+= “004100001”번째 셀의 인접 셀과 동등한 AS 의미한다.
또한 이 인접 셀로부터의 간섭신호의 감쇄 HS 계산해야 하는데 이 값의 합은 “dwave”
에서와 같은 방식으로 “uwave”2} 불린다. 그러나 두 좌표행렬 중 하나, 이 경우에는, 행
렬 “there”2 다음과 같이 조금 다르게 제공된다:

>>userposi(1,1:2) = userinfo(othercell,other,1:2);
>>here = baseinfo(numcell,:);
>>there = userposi - baseinfo(othercell,:) °°

+ baseinfo(around,:) + baseinfo(numcell,:);
“dwave” 2] 경우는 다음과 같다:

>>userposi(1,1:2) = userinfo (numcell,numuser,1:2);
>>here = baseinfo(numcell,:);

>>there = userposi;

“uwave”2] 경우, 3개의 추가 항이 존재한다. 이 3개의 항은 셀 랩핑에 의해 야기될 수
있는 계산 오류를 보상하는 FSS 한다.
그림 7.12는 2개의 항을 사용하는 BAYS 보여준다. 그림에서, 15번째 셀의 사용자로
부터 19번째 Alo} 19번째 기지국으로의 간섭이 평가된다. 이 경우, “numvell=19”,
“othercell=15”, “070400=2””이다. (wrap.m 참고) 만약 다음과 같은 3개의 항을 갖는 행
렬 “there”-S 사용하면,
>>userposi(1,1:2) = userinfo(15,other,1:2) ;
>>here = baseinfo(19,:);

>>there = userposi - baseinfo(15,:) °°

+ baseinfo(2,:) + baseinfo(19,:);

402



===== PAGE 403 =====
셀룰러 통신시스팀 (를

| 이 6

uonesusdwod 0/M:
(eydye ‘asauy 8194) 1510 ©
et

(4990) 0010108 8200818]1리비 ㅇ                            (e)
uonejs aseg @

(: 8928430) Ojuleseq-
~ (Z:1 48440 ||8219410) 이비1050

(2:1 18410 ']]0218410)
8         6                                        . 3
(: ‘punoue) ojulaseg >

uonesuadwos/m :
(eydje ‘asa ‘asey) 1510
£

—>            |: 1|8018410) Ojulaseg-
(Z:1 19410 ']160186410) 이비1050

403



===== PAGE 404 =====
Mobile Communications using MATLAB Simulation

그림 7.12(8)에 보인 바와 같이 A 랩핑을 포함한 BEEA “dist(here, there, alpha)”
의 적절한 계산을 얻을 수 있다. 그러나 다음과 같이 3개 항을 무시하면,
>>userposi(1,1:2) = userinfo(15,other,1:2);

>>here = baseinfo(19,:);

>>there = userposi;

그림 7.1206)에 보인 바와 같이 부정확한 경로손실 값을 얻게 된다. 여기서는 간섭을
일으킬 수 있는 모든 사용자로부터 간섭을 계산하고 이를 더해 총 간섭 “dwave”’S 계산
다

다음과 같이 기술되는 </(20+ 7)비 Rye & 계산해야 한다:

rf

Roni a   e

N+I

*      1

SIC +i/€

1

=                                   74

(C/N)'+(C/D)"                 “
(7.2)에서, C/(N+ DE C/N CISA 얻을 수 USS SF 있다. C/N

의 값은 “power(10.0,cnedge/10.0)*dwave” = 제공되고, C/I 0 해
당한다. 이 값을 사용하여, 시뮬레이션에서 </(20+ /)비 “cnirdb” (decibels) 구할
수있다

마지막으로, C/(N+ D7} 간섭조건을 만족하는지, 다시 말해, 이 값이 C/(N+ 7)
문턱치 “cnirth’ c+ 큰지 검 Deas,  C/(N+ 17} 문턱치를 초과하면 콜이 수용되고
사용자에게 채널이 할당된다. 이 경우, 함수 “holdtime()”o] 수행되고 출력이 사용자에
게 콜이 끝나는 시간을 제공하는 콜 유지시간으로 할망된다. 만약 간섭조건이 만족되지
않으면, 그런 Se 차단된다고 간주하고 차단된 콜의 +S 변수 “601000004700^으로 센다.

404



===== PAGE 405 =====
셀룰러 통신시스템

7.3.8 채널체크와 재할당

또한 매 시간주기에 연결된 사용자의 간섭조건을 검사해야하는데, 이 과정은 채널할
당과 비슷한 방법으로 행해지고 각 연결된 사용자에게 할당된 AS C/(N+ D7 검
사된다. 채널의 C/(N+ 2)가 만족되지 않으면, 사용자는 현재 할당된 채널을 풀어주고
채널할당과 같은 방법으로 다른 채널을 찾도록 시도한다.

여기에서, 채널 조건이 만족되지 않으면, 이런 이벤트는 차단으로 간주되지 않고
의 강제된 종료로 간주된다. 그래서, 이런 경우에는, 콜의 강제된 Sire       변
“forcenum” °.= 세어진다.

Ay 때

수7

7.3.9 즐력

마지막으로, 전체 메인루프가 실행된 후에, 축적된 데이터는 계산되어 출력 행렬
“output” 저장된다. 지금까지의 과정을 통해서
“forcenum” 2} 같은 필수적인 수치 변수를 얻었기 때문에 단순히 이전에 정의된 차단확

이미 “callnum”, “blocknum”,

률 P, >t 강제된 on gis (7.2) 9} (7.3)으로 계산한다.

“data.txt” = erst   장된다. 행렬 nee en QO 표 ic 같다.

827.38 “0410니1 의 내용
열                                                           Ws
output(1,:)                            콜의 수
output(2,:)                    차단된 콜의 +
output(3,:)                                          차단확률
output(4,:)                                               강제종료확률

또한 시뮬레이션에서는 다른 출력 행렬 “check” 9} “check2”S 제공한다. 매 시간주
기에서 차단확률과 강제된 종료확률의 현재 HS “0060(”와 “check2”] 각각 저장한

405

fo ㅣ



===== PAGE 406 =====
1  최신 이동통신시스템
G

Mobite Communications using MATLAB Simulation

다. 결과적으로, “check” 2} “check2”= 매 시간주기의 변이 데이터를 주고 프로그램 사
용자는 시뮬레이션의 적절한 루프 길이를 결정할 수 있다.

ZY DcA 알고리즘을 사용한 셀룰러 시스템의 시뮬레이션 결과

이 장에서는 DCAS 사용하는 셀룰러 시스템의 적절한 성능을 평가할 것이다.

7.4.1 시뮬레이션 결과
이전 장에서와 동일한 SAS 사용하여, 시뮬레이션 결과를 평가할 수 있다. 예를 들
면, 사용자 수에 따른 차단확률 성능을 다음과 같은 방식으로 볼 수 있다:
>>semilogy (usernum, output (3 , ; ) )

그럼 7.13은 차단확률 대 사용자 수를 보여준다. 그림에서, “cnedge” [그럼 7.13(3)]
와 “chnum” [그림 7.13(6)]가 인자로 평가되었다. 높은 수신파워와 큰 채널의 수가 낮
은 차단확률을 가져옴을 알 수 있다.

10°
chnum=5
cnirth = 15 (dB)
을
2
Ss
o
5 10'F
Zz tf
3
3                                   cnedge = 15 (dB)
                     cnedge = 20 (dB)
10 돕                     10                     15                    20                    25

Number of users (users/cell)
(a)

406



===== PAGE 407 =====
셀룰러 동신시스팀 (을

10°         a
chnum = 20 (dB)
cnirth = 15 (dB)
2
3                                                              chnum =5
로 10나
=
들                                                          chnum =3
3
a
|
05         10         15         20        25
Number of my (users/cell)
b)

를 그림 7.13 ASS 대 사용자 +: (a) 인자:206006 (6) 인자:아0040

그림 7.14는 “0060《"로 얻은 변이 차단확률을 보여주는데 시뮬레이션의 길이
(‘‘timeend=5000"-& 사용)가 평가에 적절함을 의미한다.

0.5

cnedge = 20 (dB)
chnum =5
cnirth = 15 (08

0.4

으
bo

ett tee em, gett tert eeencas
pga uneteghhe > One Reese pe 시우 ase MeIeeNs

은
2

Blocking probability

0.1

user=5

0                  1000                2000               3000               4000             5000
timenow (seconds)

MI3 7.14 차단확률의 변이 성능

407



===== PAGE 408 =====
글 최신 이동통신시스템
Mobile Communications using MATLAB Simufation

74.2 이론적인 분석

이 장에서는 차단확률의 이론적인 결과를 평가한다. 간단하게 하기 위해, 각 사용자
의 수신파워는 충분히 높아 다른 사용자로부터의 간섭은 무시될 수 있다고 가정한다.
이 가정 하에, 차단확률을 80886['6 loss formula [4]를 사용하여 다음과 같이 나타낼 수

있다:
ee
(vh)’
~. ~ an

s(n-1
a, '   Jom                          (7.5)

i=0

Py -theo ~

여기서, nth st 각각 사용자와 채널의 수이고 ?와 /는 각각 시뮬레이션에서
“lambda” 9} “46에 해당하는 비 연결된 사용자 당 평균 콜 도착속도와 평균 콜 유지시
간을 나타낸다. 그림 7.15는 시뮬레이션 결과와 이론적인 값의 비교를 보여준다. 시뮬
레이션 결과가 이론치와 부합한다고 결론지을 수 있다.

10°                   r                 ㅜ
4 a
zr
2
s
은
a
=
[=
포
8
™ 10°F                                           © Simulation results
q                                                         Theory
10                   i                  ‘                 :                  ‘
5                10                15                20                25               30

Number of users (users/cell)

를 그림 7.15 이론적인 분석

408



===== PAGE 409 =====
셀룰러 통신시스템 (을

| 75 |  셀룰러 시스템을 위한 어레이 안테나를 사용한 YA Deamforming) 기술

빔형성 기술은 공간 도메인에서 주파수 자원의 사용을 최적화하기 위해 이동통신시
스템에서 널리 사용된다 [5]. 기지국에서 이 ISS 구현함으로써, 기지국은 이동국의
위치에 따라 동적으로 지대 (2006)의 GAS 바꿀 수 있다 [6]. 기지국에서 동일채널 간
섭과 원하지 않는 방향으로부터의 지나친 다중경로 페이딩의 수신이 감소하는데 이는
원하는 방향으로 높은 안테나 이득을 주고 원하지 않는 방향으로 낮은 안테나 이득을
줄 수 있기 때문이다. 비슷하게, 이동국의 관점에서 보면, 다른 기지국으로부터의 간섭
신호가 감소한다. 이는 기지국이 원하지 않는 방향으로 신호를 전송하는 것을 피할 수
있기 때문이다. 결과적으로, 서비스의 품질이 기지국과 원하는 이동국 모두에서 향상
된다. 시스템 수용능력 또한 채널-재사용 거리를 짧게 할 수 있기 때문에 증가한다. 자연
적으로, 이동국에서의 빔형성 기술이 더 큰 향상을 위해 필요하다. 원하는 신호 (반
파) 파워와 전체 동일채널 간섭신호 파워의 비 (2000이 이동통신시스템의 수용능력
결정짓는 가장 중요한 인자가 된다. 빔형성 기술은 간섭을 억제할 수 있기 때문에 시
템 수용능력을 향상시키는 강력한 도구이다.

빔형성 제어는 무선통신시스템을 위한 모        속방식에 몇 가지 이점을 제
한다. 이들 시스템에는 FDMA, 시간분   eee     4; (TDMA), CDMA7} 포함된다. 또
:              할다중접속 (80844)가 제한된 주파수 자원 내에서 채널 수용능력을 증가시
키기 위한 방법으로 제안되고 연구되어 왔다. SDMA, 기지국은 각 이동국에 개개
의 빔을 할당할 수 있고 이동국은 셀 내에서 동일한 주파수를 사용하여 기지국과 통신

:

1¥ 00 야

인
2,
re,
Be,
10
oy

[원 off
of

0 0
iy

빔형성 제어의 효과를 평가하기 위한 몇 가지 측정치가 존재하는데 이는 접속방식에
의존한다. 이 장은 모든 방식에 공통된 인자인 CIR] 집중한다. 여기서, CIRO] 이동통
신시스템에 훨씬 많은 영향을 끼치므로 열잡음은 무시한다.

간단하게 하기 위해, 이 장에서는 기지국에서의 업 링크 향상의 평가를 설명한다.
그림 7.16은 빔형성 기술을 사용하는 기지국을 보여준다. 그림 7.16에서, 동일한 주
파수를 사용하고 주파수 재사용 거리 DS 갖는 3개의 셀이 존재한다. 이 거리는 서

409



===== PAGE 410 =====
a 최신 이동통신시스템
Mobite Communications using MATLAB Simulation

비스 모델에서 필요한 서비스 품질을 만족시킬 수 있도록 설정된다. 3개의 기지국
동일한 주파수를 사용하여 각각 By, By, Bo ASS 전송한다고 가정한다.

 : Base station
i  : User

Interference

를 그림 7.16 셀룰러 시스템에서의 기지국에서 빔형성 기술의 사용

2,를 보면, 4,로부터의 원하는 신호의 파워와 My, /4;로부터의 간섬신호의 파워

의 비는 다음과 같이 주어진다
So                Grgo (Prim )                 Gyp0 (ato )                 Gro (P11, )                 Gyo (rvBq )
~ ~ … ^ 0
Ch : -.오        é,   Gyp0 (Pum; )   Gyp9 (ym; )   ACD   Grrr: (Fy )

SARe Oe AO. x0 NO. 1s 28

i=l

(7.6)

410



===== PAGE 411 =====
셀룰러 suse 006

a= 경로손실 항, 4는비례계수, P= MANS 전송파워, d= Mj 2, 사이
의 거리, ㅎ,는 Mj By (7=0,1,2) 사이의 새도윙에 의한 왜곡이다. 기호 Guz,
(Any) By 070/,를 향한 수평 안테나 이득을 나타내고 0,//,는 ㅁ;로부터 44,
의 수평방향이다. 기호 Gye (Oyu, = Bool 0,//,를 향한수직 안테나이득을 나타내고
Oy = 2,로부터 24,의 수직방향이다. 같은 방식으로, Guy (Oue,)= 44,에서 072,
로의 수평 안테나 이득이고 022,는 Bot M; 사이의 수평방향이고 Cyy, (012,)는
44,에서 @,,, 로의 수직 안테나 이득이고 02,는 Bot 44, 사이의 수직방향이다.
02//,와 @,//의 관계를 그림 7.17에 보였다. Oy_, At Oye, 44 (360 - Oxy, Ht

(360 — A yy.) 당한다.

/

vm

um,

B,           O degree
를 그림 7.17 기지국과 이동국의 관계

7.5.1 CIR 향상 평가를 위한 시뮬레이션 프로그램

이 장에서는 셀룰러 시스템에서 빔형성 기술과 어레이 안테나를 사용하여 이동 셀룰
러 시스템에서 얻을 수 있는 CR 향상을 평가하기 위해 시뮬레이션 프로그램을 사용한
다. 주프로그램은 프로그램 7.8에, 부프로그램은 프로그램 7.9-7.11에 aA] ch. 표 7.4
는 각 프로그램의 기능을 정리한 것이다. 그림 7.18(0는 시뮬레이션 모델을 보여준다.
동일한 주파수를 사용하는 19개의 셀이 존재한다고 가정한다. 모든 기지국 간의 거리
는 클러스터의 크기로 정의된다. 그림 7.18) (CE 셀 배치와 클러스터의 크기의 관
계를 보여준다. 여기서 SAS] 셀은 0번이고 주변의 AS 1에서 18번이다.

411



===== PAGE 412 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

R748 프로그램 7.87.11의 기능

프로그램     시뮬레이션에서의 이름               기능
프로그램 7.8          main.m                              주 프로그램
프로그램 7.9         set D.m                        기지국 간의 거리 결정
프로그램 7.10       stationinit.m                    기지국의 위치 결정
프로그램?7.11       antgain.m                      안테나 이득의 특성 결정
프로그램 7.6           shadow.m                            로그정규 PES 갖는 새도윙에 의한 감쇄 생성

(b)

를 그림 7.18 시뮬레이션에서의 셀의 배치: (a)
배치 (6) 클러스터 크기가 7일 때의 셀 배치
때의 셀 배치

프로그램은 중심 기지국에서의 업 링크의 CRE 계산하고 다음 두 가지 경우의 CIR

통계 차이를 출력한다:

D 경우 1: 빔형성 제어가 적용된경우
 경우 2: 빔형성 제어가 적용되지 Se BF
412



===== PAGE 413 =====
셀룰러 통신시스템 를

시뮬레이션 프로그램은 다음과 같다:

@기지국의 위치를 정의한다.
DAA 7(7=0‥…18)에서의 이동국의 위치를 정의한다.
@다음을 계산한다:
ㆍ Ra Ao] 이동국과 목표 』번째 기지국 간의 거리와 각
ㆍ ?번째 셀의 이동국과 중심 기지국 간의 거리와 각
중심 기지국에서의 』번째 AS) 이동국의 방향에 대한 안테나 이득
ㆍ Ral 셀의 이동국에서 중심 기지국 방향에 대한 안테나 이득
*새도윙의 효과
® 44-13} 20] 대한 0표계산

그림 7.19는 시뮬레이션 흐름도를 보여준다. 다음이 주프로그램의 윤곽이다.

(0

Status initialization

Loop

\nitialization of MS's position

[

Calculation of antenna gain
at BS and MS

ㅣ

Calculation of CIR at
centered BS

Loop

수     Statistics (CIR)    2

ㅣ

해               600

를 그림 7.19 시뮬레이션 흐름도

413



===== PAGE 414 =====
최신 이동통신시스템
Mobile Communications using MATLAB Simulation

[status initialization]

먼저, 클러스터의 3717} 인자 와 JS 설정함으로써 결정된다. 여기서, 클러스터
의 크기는 다음 식으로 주억전타:

P+ 41-J                    (7.7)

1=1이고 /=1일 때, 클러스터 크기는 3이다. 다음으로, 클러스터 크기에 기반하
여, 기지국의 배치를 결정한다. 기지국의 높이와 셀의 반경 또한 결정한다. 기지국의 높
이를 0으로 설정하면 매크로셀 모델을 가정할 수 있다.

두 번째로, 기지국(88)과 이동국(548)에서 안테나 이득의 특성을 결정한다. 여기서,
imal AS) 기지국을 BS, 이동국을 MS 정의한다. 이 시뮬레이션에서, 경우 2의
모든 방향 dol] 대해 Gye (d) = Guy (dP) = ㅇ\,.0)= Gyu(d) =0 ( 2=0…18)을
가정한다. 반면, 경우 1에 대해서는 안테나 이득을 특정 값으로 정의한다. 안테나 이득
의 특성을 다음과 같이 근사화할 수 있다고 가정한다.

10log,, 008”(0), -ㅅ/2흐0흐272
re                 otherwise                (7.8)

Grp, (9) = |
방향에 대한 안테나 이득이다. 인자 은 대역폭 0S 결정하는데 사용된다.
고 값의 3 08 이내이다. /은 다음과 같이 결정된다.

xed
이 $2 최
108,,1172

"Tog, 009(0627180)                            (7.9)

식 (7.8)을 사용하여  628. 00,  Guu 00,  Gyp (9),  Gyuf ¢) 2] 특성을 결정 할 수 있
다. 물론, 다른 안테나 특성을 사용하여 CIR 향상을 평가하기 위해 자유롭게 이들을
정할 수도 있다.

414



===== PAGE 415 =====
셀룰러 통신시스팀 PO

[Loop]

각 셀의 이동국의 위치는 임의로 결정된다.

먼저, M, ( 7=0‥…18)의 필요한 전송파워 PS 찾기 위해 4,와 ,의 거리를 계산
한다. PZ 제어함으로써, 파워제어 기술을 구현할 수 있다. 이 파워제어 기술은 CIR
을 향상시키기 위한 효과적인 기술이고 빔 제어와 실제적인 관계가 있다. 이 기술을 사
용하여, 각 이동국은 이동국과 기지국의 거리에 따라 전송파워를 동적으로 제어할 수
있다.

둘째로, 경로손실 4; “를 찾기 위해 중심 BY MS) 거리를 계산한다.

셋째로, MV 목표 #,로의 수평각 O yp 과 수직각 6, 를 계산한다. 경우 1에
서 각 MS SE 에 대해 최고 안테나 이득을 설정한다. 즉, (7.8)에서 보인 바와 같
이 @,/이 #=0에서 최대값을 갖기 때문에, @,,/(0)이 방향 0,』 ( 7=0…18)에서
설정된다. 같은 방식으로, 수직 안테나 이득의 최고 방향 @,,/(0)이 방향 0,, 에 대
해 설정된다. 다음으로, 44, (7=1…18)에서 중심 [로의 수평각 @,, 과 수직각
8 v5, 계산한다. 0, 와 Oye) 차와 0, 와 6,,,의 차가 각각 안테나 이득
Guu np,) + ㅇ,/(0,,,)를계산하는데 사용된다.

은 방식으로, 중심 8,으로부터 44,레대한수평각 Oy 과수직각 0, 를계산
하고 최고안테나 이득 @,,,,(0)과 Gyy,(0) S 설정한다. 다음으로, 중심 (으로부터
44,(7=1…18)에 대한 수평각 @,,,와수직각 O yy, 를계산한다. One 와 0,,,의차
HO yy, AF @,/의 차를 이용해 안테나 이득 @,,,(0,』)와 ㅇ,,,(0,,)를 얻는다.

마지막으로, (7.6)에 기반하여, 중심 기지국에서 경우 1과 경우 2에 대해 업 링크의
CIRS 계산한다.

[statistics (CIR) ]

[Loop] 반복한 후에, 경우 1과 29] CIR 통계가 계산된다.

415



===== PAGE 416 =====
Az 이동통신시스템
Mobile Communications using MATLAB Simulation

7.5.2 시뮬레이션 결과
그림 7.20은 중심 기지국에서의 업 링크의 CIR 향상 AWS 경우 1과 2의 차이를 대
비해 보여준다. 인자는 다음과 같다:

0) I=1, J=1;

@ Grup (d)= (7.8) 의해 정의되고 x=— 100[4B], n= 2.41 ( 0= 60);
@ 모든 방향 0에 대해 Gyp(d) = Guy (d) = Gyu(d) =0;

@)새도윙 9080의 표준편차=0;

© 경로손실 & alpha=3.5;

© 파워제어 비사용;

(2)기지국의 높이는 Ofm] (매크로 셀 가정)

1

ys

ia.
ies
pty UE

J.      ere    4       2.       1      ~      2       4

30 ; 40  50  60  70  80  90  100 110  120
Beamwidth [degree]

Benefit derived by beamforming [dB]
oem NI wet ao Oa @ wo SO

를 그림 7.20 cR 항상

그림 7.20에서, 가로축은 기지국에서의 대역폭을, 세로축은 중심 기지국에서 경우 1
과 2의 CIR 차이를 보여준다. 빔형성 제어의 평균 CIRS 빔형성 제어가 없는 경우에 비
해 8 08의 향상을 보여준다.

자연적으로, 다운링크 향상을 계산하기 위한 프로그램의 WBS 간단하다. 기지국과
이동국의 인자가 대체됨을 주지하라. 또한 한 셀에서 다수의 사용자가 동일한 주파수를

416



===== PAGE 417 =====
셀룰러 통신시스템

0 ㅣ

사용할 수 있도록 프로그램을 변환할 수 있음을 주지하라. 이 경우, 셀 내부 사용자로부
터의 간섭 계산을 고려해야 한다. 프      Ba ag   환할 때, 모델의 활용과 CIR 계산에서
중점을 두는 목표 사용자나 기지국에 대해 주의를 기울여야 한다.

76 |

이 장에서는 다중지점 상황을 고려하여 전체 시스템 성능을 평가하기 위한 접속방식
시뮬레이션에 중점을 두었다. 셀룰러 시스템과 채널할당 알고리즘에 대해 설명한 뒤에,
이러한 시뮬레이션을 수행하는데 필요한 몇 가지 주요 기술과 DCAS 갖는 셀룰러 시
스템을 위한 시뮬레이션 프로그램의 예를 제시하였다. 또한, 어레이 안테나를 갖는
DCAS 소개하고 동적 지대를 형성하는 것의 효과를 기술하였다.

417



===== PAGE 418 =====
최신 이동통신시스템

Mobite Communications using MATLAB Simufation

1) Balston, D. M., and R. C. V. Macario, Cellular Radio Systems, Norwood, MA: Artech House,
1993.

2) Sampei, S., Applications of Digital Wireless Technologies to Global Wireless Commu-
nications, Upper Saddle River, NJ: Prentice Hall, 1997.

3) Gelenbe, E., and G. Pujolle, Introduction to Queueing Networks, New York: John Wiley &
Sons, 1987.

4) Lee, W.C. Y., Mobile Cellular Telecommunications Systems, New York: McGraww Hill, 1989.

5) Godara, L. C., “Applications of Antenna Arrays to Mobile Communications, Part I:
Performance Improvement, Feasibility, and System Considerations,” Proc. of IEEE, Vol.85,
No.8, August 1997, pp.1195-1245.

6) Litva, J., and T. K. Lo, Digital Beamforming in Wireless Communications, Norwood, MA:
Artech House, 1996.

418



===== PAGE 419 =====
프로그램 7.1
% Program: 7-1
%
% dcamain.m
%
% Simulation program to realize DCA algorithm
%
% Programmed by F. Kojima
%

$3%%S%S%S%S%S%S%SSSSSS%S Preparation Part 융융융웅웅융웅웅웅융융웅옹웅웅융웅웅웅웅웅웅웅웅웅웅웅웅

cnedge = 20.0;          CNR on cell edge (dB)

Chirth = 15. 0;          CNIR threshold (dB)

lambda = 6.0;           average call arrival rate (times/hour)
06 ~. 520.0%             average call holding time (second)

timestep = 10;
timeend = 5000;
chnum = 5;

time step of condition check (second)
time length of simulation (second)
number of channels per each base station

00 00 00 00 00 00 00

alpha = 3.5;                    % pass loss factor

sigma = 6.5;                    % standard deviation of shadowing
usernum = [5,10,15,20,25]; % number of users per cell

output = zeros (4,5);            % output matrix

check = zeros (5, floor (timeend/timestep) ) ;

2

% matrix for transient statu

for parameter = 1:5

rand( state’, 5)
randn('state',1);

user = usernum(parameter); t*number of users per cell

baseinfo = zeros(19, 2);

419


===== PAGE 420 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

sbaseinfo(cell #, informations)
SSSSSbaseinfo(:, 1): x coordinates
SSS%cbaseinfo(:, 2): y coordinates

userinfo = zeros(19, user, 15);

Suserinfo(cell #, user #, informations)

S%%tbuserinfo(:, :, 1): x axis

St%%tuserinfo(:, :, 2): y axis

SSsssuserinfo(:, :, 3): attenuation

Sbsssuserinfo(:, :, 4): usage O->non-connected 1->connected
SbS%Suserinfo(:, :, 5): call termination time
SSSSsuserinfo(:, :, 6): allocated channel #

[baseinfo] = basest;
[wrapinfo] = wrap;
{meshnum, meshposition] = cellmesh;

timenow = 0;
blocknum = 0;
forcenum = 0;
callnum = 0;
users = 0; % number of connected users

SSSSSESESSESEEESESSESE Main loop part SSSSSSS¥SBSSSSYSEFSSFEFSEF
while timenow < timeend
callnumold = callnum;

blocknumold = blocknum;
forcenumold   forcenum;

|

Sfinished calls
for numcell = 1:19
for numuser = l:user

if userinfo(numcell, numuser, 4) == 1 &
userinfo(numcell, numuser, 5) < timenow
userinfo(numcell, numuser, 4) = 0;
users = users -l;
end
end

end

420



===== PAGE 421 =====
Sreallocation check
for numcell = 1:19
for numuser = 1l:user
if userinfo(numcell, numuser,4) =
reallo = 0; % flag
cnirdbl = 0.0;
dwave = userinfo(numcell, numuser, 3);
cn = power(10.0, cnedge/10.0) * dwave;
uwave = 0.0;
ch = userinfo(numcell, numuser, 6);
for around = 2:7
othercell = wrapinfo(numcell, around) ;
for other = l:user

ㅣ
oo)

if userinfo(othercell, other, 4) == 1 & userinfo(othercell,
other, 6) == ch
userposi(1,1:2) = userinfo

(othercell, other, 1:2);
here = baseinfo(numcell, :);
there = userposi - baseinfo

(othercell, :) + baseinfo
(around, :) + baseinfo
(numcell, :);

uwave = uwave + dist(here,
there, alpha) *shadow (sigma) ;

end
end
end % around loop
if uwave == 0
cnirdb = 10.0*1log10(cn) ;
else
cnirdb = 10.0*1log10(1/ (uwave/dwavet+1/cn) ) ;
end

if“enirdb<: enirth
reallo = 1;
end

if reallo ==
userinfo(numcell, numuser, 4) = 0;
users = users -1;
succeed = 0;
cnirdb = 0.0;
for ch = 1:chnum

421



===== PAGE 422 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

available = 1;
for other = l:user
if userinfo(numcell, other, 4)
== 1 & userinfo(numcell,
other, 6) == ch
available = 0;
end
end
if available ==
uwave = 0.0;
for around = 2:7

othercell = wrapinfo(numcell, around) ;
for other = l:user
if userinfo(othercell,
other, 4) == 1 &
userinfo (othercell,
other, 6) == ch
userposi(1,1:2) =
userinfo (othercell,
other,* 134)?
here = baseinfo
(numcell, :);
there = userposi - baseinfo(othercell, :) + baseinfo
(around, :) + baseinfo(numcell, :);

uwave = uwave + dist(here, there, alpha) *shadow(sigma) ;

end
end
end % around loop
if uwave ==
cnirdb = 10.0*1log10 (cn);
else

cnirdb = 10.0*1logl10(1/ (uwave/dwavet1/cn) ) ;

end
else
cnirdb = 0.0;
end
if cnirdb >= cnirth
succeed = 1;
users = users + 1;

ㅣ
fay
~

userinfo(numcell, numuser, 4)
userinfo(numcell, numuser, 6) = ch;
break

422



===== PAGE 423 =====
end
end % ch loop
if succeed == 0

forcenum = forcenum + 1;
end

end % reallo ==
end % connected (need to be checked)
end % user loop
end % cell loop

Snew call arrival
for numcell = 1:19
for numuser = l:user
if userinfo(numcell, numuser, 4) == 0 & rand <=
lambda*timestep/3600
callnum = callnum + 1;
mesh = floor (meshnum.*rand) +1;
while mesh > meshnum
mesh = floor (meshnum.*rand) +1;
end
userinfo(numcell, numuser, 1:2) = baseinfo
(numcell, :) + meshposition(mesh, :);
succeed = 0; % flag
cnirdb = 0.0;

userposi(1,1:2) = userinfo(numcell, numuser, 1:2);

here = baseinfo(numcell,:);
there

userposi;

dwave = dist(here, there, alpha) * shadow(sigma) ;

cn = power(10.0, cnedge/10.0) * dwave;
for ch = 1:chnum

available = 1;

for other = l:user

if userinfo(numcell, other, 4) == 1 &
userinfo(numcell, other, 6) == ch
available = 0;
end
end
if available == 1

uwave = 0.0;
for around = 2:7
othercell = wrapinfo(numcell, around) ;

423


===== PAGE 424 =====
최신 이동통신시스템

C        Mobile Communications using MATLAB Simulation

for other = l:user

if userinfo(othercell, other, 4) == 1 & userinfo(othercell,
other, 6) == ch
userposi(1,1:2) = userinfo(othercell, other, 1:2);

here = baseinfo(numcell, :);
there = userposi - baseinfo(othercell, :) + baseinfo
(around, :) + baseinfo
(numcell, :);
uwave = uwave + dist(here, there, alpha) *shadow (sigma) ;

end
end
end % around loop
if uwave == 0
cnirdb = 10.0*log10(cn);
else
cnirdb = 10.0*1lo0g10(1/ (uwave/dwave+1/cn) );
end
else
cnirdb = 0.0;
end

if cnirdb >= cnirth
succeed = 1;
users = users + 1;
userinfo(numcell, numuser, 3)   dwave;
userinfo(numcell, numuser, 4) = 1;
userinfo(numcell, numuser, 5)
timenow + holdtime (ht) ;

qu

userinfo(numcell, numuser, 6) = ch;
break
end
end % ch loop
if succeed == 0
blocknum = blocknum + 1;

end
end % new call
end % user loop
end % cell loop

fprintf ('Sd\t%d\t%d\t%d\t%e\n', parameter, timenow, callnunr-

callnumold, blocknumblocknumold, blocknum/callnum) ;
check (parameter, timenow/timestept1) = blocknum/callnum;
check2 (parameter, timenow/timestep+1) = forcenum/

424



===== PAGE 425 =====
(callnumblocknum) ;

timenow = timenow + timestep;
end %while loop

SSSEEEESESESEESS OUtPUt PALt %44%SSSSSSSSSSSSSSSSSSSSSSSS

output (1,parameter) = callnum;
output (2,parameter) = blocknum;
output (3,parameter) = blocknum/callnum;

output (4,parameter) = forcenum/ (callnumblocknum) ;
end %parameter loop

fid = fopen('data.txt','w');

fprintf (fid, 'UserNumber\t') ;

fprintf (fid, 'tg\t%g\t%g\n', usernum(1,:));
fprintf (fid, 'CallNumber\t') ;

fprintf (fid, 'sq\ttg\teoq\n', output (1, >)
fprintf (fid, 'BlockNumber\t') ;

fprintf (fid, '%g\t%g\t%g\n', output (2,:));
Eprintt£ (fid, 'BloeckingProb. 나)

fprintft (fid, *sq\ttg\tegqin',.. output(3;-:))
fprintf (fid, 'ForcedTerminationProb. \t');
fprintf (fid, 'Sg\t%g\t%g\n', output (4,:));
fclose(fid);

ZREKKKKKKK KKK KKK KKKKKKKKK and of FL LS KEK KKKKKKKKKKK KKK KKK KKK KK

프로그램 7.2
% Program 7-2
%
% basest.m
%
% This function sets positions of the base stations.
%
% Programmed by F. Kojima
% Checked by H.Harada
%
function [out] = basest()
baseinfo(1, 1) = 0.0;
baseinfo(1, 2) = 0.0;

425


===== PAGE 426 =====
최신 이동통신시스템

426

Mobile Communications

baseinfo(2,
baseinfo (2,
baseinfo (3,
baseinfo (3,
baseinfo (4,
baseinfo (4,
baseinfo(5,
baseinfo(5,

1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
1)
2)
10
2)
1)
2)
1)
2)
1)
2)

baseinfo (6,
baseinfo (6,
baseinfo(7,
baseinfo(7,
baseinfo (8,
baseinfo(8,
baseinfo(9,
baseinfo(9,
baseinfo(10,
baseinfo(10,
baseinfo(1l,
baseinfo (11,
baseinfo(12,
baseinfo(12,
baseinfo (13,
baseinfo (13,
baseinfo(14,
baseinfo(14,
baseinfo(15,
baseinfo(15,
baseinfo(16,
baseinfo (16,
baseinfo(17,
baseinfo(17,
baseinfo(18,
baseinfo(18,
baseinfo(19,
baseinfo(19,

out = baseinfo;

Sk KK KR KK KK KKK end of File KKK KKKKKKKKKKKKKKKKKKKEK

using MATLAB Simufation

-0-5"”80 (3.0);
1.5;
“sqrt (33.0);
0.07
“0. 5%sgqrt(3.0).;
“Awe
0:5*sSqrt(3<0) ;
590

sqrt (3...0)-;
<OF
-5*sqrt (3.0);
아오
0;
, 0;
“Sqri(3.0):;
3.0%

“1 -Srsgrt (3.
53

“2. O* sqrt (3s
0.0;

rl. Se Sgqrets.
hae
= -sqrt (3.0);
-3 OF
02.07
733.07
Sqrets .0} 7
“350%

L.S¥ sqrt (3.0);
Seca
27/0¥ sqrt (3.0)?
0.0;
= 1.oesqrt (3.0);
Lay
Sqrie(s.0);
za

0
0
=1
0
3

0);
0);

0);



===== PAGE 427 =====
프로그램 7.3
% Program 7-3
% wrap.m
%
% This function gives informations about cell-wrapping
%
% Programmed by F. Kojima
% Checked by H.Harada
%
function [out] = wrap (inputmat)

inputmat( 1,1:19)   ace
ainputmat:(2,1:19)
67305; LoAt Sls
inputmat ( 3,1:19)
5, Ga 2p 84 F
inputmat( 4,1:19)
15,16;- 6-7}
inputmat( 5,1:19)
Lied, Lol

ㅣ

peice I EA

El piston eile

127337161 ;

10014ㄴㅁㄴ 7, 1119). = [ 7,.8- 627 17 0710.19, 0. 9, 0,

[ 2, <9,10,- 37 lyn Pe Seta es Uh, 10,41, 12, 4535,

[ <3, 10,1112, 47 1peepe eh. 6; 15,19 716,13, 44,

[ 4, 312,13 pi by 07 2, 10, 1 19,1817, 9, -8,

[ 5, 17 4,114,145, 16, 67 de s2p33y 1291385598) £9,

inputmat(6,1219) = 6, 7, 1,5, 16,17; 40043, 0, 2.042, 47147, 15,2), 10,

30 4. 00167

inputmat (_8,1:19)<=: [. 8,14, 9) 2, 77049.45.51 4213.17 10 98.13.36218,

inputmat ( 9,1:19) = [ 9,33717,10, 2;-8, £47 °@72,418,. 6,16 2b, 3; 1,7,

19°15; 251%
inputmat (10,1:19)
1, 4. 8141;
inputmat (11,1:19)
4, 29" Se
inputmat (12,1:19)
14; 5, Ay 2%
inputmat (13,1:19)
8, 5372 Se Le
inputmat (14,1:19)
19,11, 16,- 6) 7
inputmat (15,1:19)

ㅣ

f1l,16,15,19,12;, 3ㅋㅎ30,너, 6) +5, 445

[12744 ,39718,13, 1475 37 OF 167455" 8,

[13,.342729717, 9344, 0, 02, 19, 77

eis Pare rah: ae oral pe Wray ed re Sod > 00. 그 3;

[10,17,16,11, 3,2, 9,28, 18). -6,-5), 15; 29712; 24,

$75:1718,13;,

0001.17, Dy

6;.16,.10,- 4,

44, 245,93 7, 9: Spb gop Sone 2682 60154 0, 2, 7,

0062, Bd


===== PAGE 428 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

2. 3, 10, tae

inputmat(L6, 1:19) -=-{46;-26,<-5715 711, 10,17, 18,7). 17 4,042 8589 el2,
3, 422 Sy xede

inputmat (17-2219): = (17 718,. 6,16, 10,.°9;13;12/;19,. 77 1s 06902 8,
2, 8) 14; 413

inputmat (18,4249). = 3018), 19)49,-:6,17,13,12, 4, 157-- 8): 25x 4 2574610,
9,.14;-.4,-317

inputmat (19,4 39) S97 35, 8, > 7, 18,102,016, 75,245 ee, aye 6,
1 7.132 42 37303

out = inputmat;

ZeeKKKKK end of file ***xxKKKK*

프로그램 7.4
% Program 7-4
%
% cellmesh.m
%
% This function sets meshs in a cell.
%
% Programmed by F. Kojima
% Checked by H.Harada
%
function [meshnum, meshposition] = cellmesh()

Fineness = 50; % parameter for mesh fineness
ka= 1;
3 = 0;
ds = sqrt(3.0) / Fineness;
xmesh = -0.5 * sqrt(3.0);
while xmesh < 0.5 * sqrt(3.0)
smesh =k - 그) tage == 0130 ^ sqrt (5.0);
if xmesh < 0.0
ymin = -xmesh/sqrt (3.0) - ds - 1.0; % lower line of a cell
ymax = xmesh/sqrt (3.0) + 1.0; % upper line of a cell

elseif xmesh == 0.0
ymin = -1.0;
ymax = 1.0;

else

ymin   xmesh/sqrt (3.0) - ds 1.0; % lower line of a cell

428



===== PAGE 429 =====
ymax = -xmesh/sqrt(3.0) + 1.0; % upper line of a cell
end
k= + 그;
ymesh = ymin;
while ymesh < ymax
ymesh = ymesh + ds;
if ymesh > ymax

break
end
je Bet Le
posi(j,1) = xmesh;
posi(j,2) = ymesh;
end
end

meshnum = Jj;
meshposition = posi;

BRR KK KK RK RRR KK RK RK KK KR RK KK end of file KEKKEKKKKKKKKKKK KKK KKK KKK

프로그램 7.5
% Program 7-5
%
% holdtime.m
%
% This function generates holding time
%
% Programmed by F. Kojima
% Checked by H.Harada
%
function [x] = holdtime (ht)

para = rand;
while para >= 1
para = rand;
end
x = ht.* (-log(1-para));

ZREKKKK KKK KR KKK KK KK KR RK KK KK KK end of file KKKKKK KKK RK KK KK KR KK RK KK

프로그램 7.6
% Program 7-6
%

429



===== PAGE 430 =====
최신 이동통신시스템

430

Mobile Communications using MATLAB Simulation

shadow.m

This function generates attenuation of shadowing

00 00 00 00 00

Programmed by F. Kojima
Checked by H.Harada

00 00

function [x] = shadow(sigma)
anoz = randn;
db = sigma * anoz;

x = power(10.0, 0.1*db);

GRRKKKKKEKKKKKKEKKKKKKKKKEKKKK End OF 71106 KEEKKKKKKKKKKKKKKKKKKKKK

프로그램 7.7
% Program 7-7
%
% dist.m
%
% This function generates attenuation due to distance
%
% Programmed by F. Kojima
% Checked by H.Harada
%
function [x] = dist(a,b,alpha)

% a,b: position of two points
% size(a) = size(b) = (1,2)

x   sqrt ( (ab) * (ab)* be

power (x, -1.*alpha) ;

x

ROR KR         i   KK I ke
end o   Lie

프로그램 7.8

$ Program 7-8

%

응 main.m

%

%$ Programmed by A.Kanazawa



===== PAGE 431 =====
% Checked by H.Harada

%

clear

$3%S%%S%SSSSSSSS% Status initialization

LSA;                 % The cluster size is determined from I and
SJ. (n = I*I + J*I + 1300)

J = 2;

r = 100;               % the radius of the cell[m]

h = 0;                 % the height of the BS[m]

D = set_D(I,J,r);

station = stationInit (D);
xbs
ybs = imag(station);

The x axis of the BS
The y axis of the BS

real (station) ;

00 ol?

00

sigma = 6.5;                  standard deviation of shadowing

alpha = 3.5;                  path loss factor

% margin = 0;               % The parameter for power control

00

우

% Characteristics of antenna gain decision for BS

w_HBS = 60;                 [horizontal]: beam width at BS for the
target direction [degree]

{horizontal]: antenna gain at BS for the

opposite direction [dB]

[vertical]: beam width at BS [degree]

00

ole

backg_BS = -100;

00 00 00

w_VBS = 360;
% Characteristics of antenna gain decision for MS

w_HMS = 360;              % [horizontal]: beam width at MS for the
target direction [degree]

{horizontal]: antenna gain at MS for the
opposite direction [dB]

[vertical] :beam width at MS [degree]

oe

backg_ MS = -100;

ole

oe

w_VMS = 360;

oe

if h == 0,                % In the case of macro cell situation,
w_VBS = 360; w_VMS = 360; % the effect of beam tilt becomes less.

end

% Antenna gain calculation of each BS

g_HBS = antgain(w_HBS, backg BS);

g_VBS = antgain(w_VBS, 0);

g_HMS   antgain(w_HMS, backg MS);

431


===== PAGE 432 =====
최신 이동통신시스템

432

Mobile Communications using MATLAB Simulation

g_VMS = antgain(w_VMS, 0);

SSEESSEEEEEEEES LOOP
%$—Initialization of MS positions

N=1000;                       % The number of repeat
for num = 1:N,
Rx = rand(1,19);            % the random values: [0-1]
Ry = rand(1,19);            % the random values: [0-1]
Hs PARES

고 = 브루, Sqre A-r2aza2 Ke Aes

tx = 2*((rand(1,19)>0.5) -0.5);   % the random values: -1 or 1

ty = 2*((rand(1,19)>0.5) -0.5);   % the random values: -1 or 1

~ ee           % The x axis of the MS when we regard the
% position of each BS as (0,0)

y= X=: tye           % The y axis of the MS when we regard the
% position of each BS as (0,0)

x2. = Ztxbs."3        % The x axis of the MS when we regard the
% position of central BS as (0,0)

y2 = ytybs.';        % The y axis of the MS when we regard the
% position of central BS as (0,0)

2 (71) = ere Say

% The complex expression of MS when we regard the position of each BS
% as (0,0)

ENS) = R2P Eye;
% The complex expression of MS when we regard the position of central
% BS as (0,0)

co Moa Geet

abs (z(1,:))3          The distance between BS i and MS i
in horizontal axis

%
%
G29   abs{z (272 y)>        % The distance between central BS
%
%

and MS_i in horizontal axis

d2 = sqrt(d.*%2 + h*2);         The distance

|

25823)   angle(z(1,:));     The angle difference between BS i

and MS 1 [rad]

%
%
phai(2,:)   angle (z(2,:));   % The angle difference between
%
%

central BS and MS i [rad]

deg = phai*180/pi;             the conversion of radian to degree

if h ==0, degH = 90*ones(1,19);



===== PAGE 433 =====
else
phaiH = atan(d(2,:)/h);
% the elevation angle between central BS and MS i
degH = phaiH*180/pi;
% the conversion of radian to degree
end

%——shadowing——
for m = 1:19
g(m) = 10*1log10 (shadow (sigma) ) ;
end
% —— propagation loss —
boss(1,:) = 10:-*:logl0.(d2(1,:: ).. “alpha:
% The propagation loss from MS i to BS i [dB]
Loss(2,:) = 10 * logl0(d2(2,:).*alpha) ;
% The propagation loss from MS i to BS 0 [dB]
Loss max = 10 * 1log10(r.“alpha) ;
% The propagation loss from the cell boundary to BS [dB]

% Free space loss

% wl = 0.1;

% Loss(1,:) = 10 * 1logl10((4*pi*d2(1,:) /wl) }*2);
% The propagation loss from MS i to BS i [dB]

% Loss(2,:) = 10 * logl0(:(4%pi*d2 (2, 00 크나 22).

% The propagation loss from MS 1 to BS 0 [dB]
% Loss max = 10 * logl10((4*pi*r/wl) .*2);
% The propagation loss from the cell boundary to BS [dB]

%——Transmission power level of each MS [dB]

Ptm_0= Loss_max*ones (1,19);    % no power control
% Ptm_0= Loss(1,:) + margin;     % power control (with margin [058] )
*—— Calculation of antenna gain for the target direction

deg B = deg(2,1)-deg(2,:);

% the angle difference between the MS 0 and MS i from central BS
deg M = deg(1,:)-deg(2,:);

% the angle difference between the BS 0 and BS i from MS i

degHBS = mod(round(deg_B),360);
degHMS = mod(round(deg_M), 360) ;
degVBS = round (degH-degH (1) ) ;        % the angle difference in

433



===== PAGE 434 =====
최신 이동통신시스템

434

Mobile Communications using MATLAB Simulation

end

% vertical direction between MSs and central BS
degVMS = degVBS;               % the angle difference in
% vertical direction between MSs and central BS

%—Calculation of CIR at centered BS

sControl

0108 a= Ptm_0(1:19)+g HBS (degHBS(1:19)+1) +
g_VBS (degVBS(1:19)+1) + g_HMS(degHMS(1:19)+1) +
g_VMS (degVMS (1:19) +1)- Loss (2,1:19)-g(1:19);
% Received level at central BS (beam forming)

(6010. 8 510. .^ 20100 s/f 10 );               % dBW
isum_a = sum( CIw_a(2:19));
CIR_a(num) = ClIw_a(1) / isum_a;

%No Control
CIdB_o= Ptm_0(1:19)- Loss (2,1:19)-g(1:19);
% Received level at centered BS (Omni)

CIw o= 10: ^ (0308 © .V/407 95            $ dB > W
isum_o = sum( CIw_o0(2:19));
CIR_o(num) = CIw_o(1) / isum_o;

%—Calculation of CIR under various w_HBS

911. = 17

sfor w_HBS2=30:10:180,

% g HBS2 = antgain(w_HBS2, backg_BS);

% CIdB_a2= Ptm_0(1:19)+g HBS2(degHBS(1:19)+1) +

% g VBS (degVBS(1:19)+1) + g_HMS(degHMS(1:19)+1) +
% g VMS (degVMS (1:19) +1)- Loss (2,1:19)-g(1:19);
% Received level at central BS (beam)
%  Clwiaz2.=.10:.%-t Crdpsae -.:7 20");          % dB W
% ciw_a2 = sum( CIw_a2(2:19));
% CIR_a2(num,ii) = CIw_a2(1) / ciw_a2;
ase i a so
Send

%—statistics

CA
00

10 * log10(sum(CIR_a)/N);
10 * 1logl0(sum(CIR_o) /N);

$—result
CA-CO                                            % Improvement



===== PAGE 435 =====
%—Calculation of CIR under various w_HBS
% CA2= 10 * 1og10(sum(CIR_a2)/N);

% CA2-CO

% plot (30:10:180,CA2-CO)

ZRKEKKKKKKKKKKKKKKK KKK KR KKK KKK End of £ite KKRKKKKKKKKKKKKKKKK KK KKK K

프로그램 7.9

Program 7-9

ole

set_D.m

Programed by A.Kanazawa
Checked by H.Harada

00 00 00 00 00 00

function D = set_D(x,y,R)

% the function to determine the distance between BSs
i R-= sqrt(3) * R;
j R= i-R / sqrt(2);

D2 = 0+03;
fork = 1:x
92 ~ 302 + A ok
end
for-k = ley
D2 =D2+45R+ 4 * j_R

end
D = abs (D2);

ZRKKKKKKKKKKKKKKKKKKKKKKKKKK and of tile KKKEKKKKKKKK KK KKK KKK KKKKEK

프로그램 7.10
% Program 7-10

stationInit.m

Programmed by A.Kanazawa
Checked by H.Harada

435


===== PAGE 436 =====
최신 이동통신시스템

436

Mobile Communications using MATLAB Simufation

function STATION = stationInit (d)
.6 The function to determine the position of BS
STATION = zeros(19,1);

for i = G35
STATION (X*4* 27 *2) *=%det feos fibseps *fF-370) *#*7 2* 1d **= sine
x pis f/f 3.0);
end
for 1 = 나
STATION 자 8, hy 27 FCS (t= 5 90626 20) + 7 자고 ed seen (tT
23. GEO}:

end
ZREKKKKKKKKKKKKKKK KKK KK KK KKK end of ELLER RRR KER KKK KKK KKK KKK KK KK KK

프로그램 7.11
% Program 7-11

antgain.m

ae 00 00 00

Programmed by A.Kanazawa
Checked by H.Harada

oe oe

function gain = antgain(width, back)

theta = [0:359];
gain = zeros(1,360);

if width ~= 360,

n = 16910 (sqrt (1/2) ) ./10g10 (cos (width*pi/360) ) ;
% the coefficient n

gain(1:89) = 10*log10 (cos (theta (1:89) *pi/180) .*n);
$[dB] Antenna gain

gain (272:360) = 10*1log10 (cos (theta (272:360) *pi/180) .“n);
%[dB] Antenna gain

if back ~= 0,    % definition of antenna gain for horizontal
% direction[dB]

back;                     % [dB]

gain(90:271)
end
end

Swe K KK RK KK KK KK KK KR KK KR KK KR KR KK KK  end of  ELLER RRR KKK KKRKKKKKKKKKKKKEKK



===== PAGE 437 =====
통신시스템

(Software



===== PAGE 438 =====
소프트웨어 무선 통신시스템

(Software Radio Communication Systems)

030 서 로

사용자들이 채택할 수 있는 시스템의 수가 증가함에 따라, 다양한 이동통신 시스템
의 공존 필요성이 증가되어 왔다 (예 : GSM, IS-54, 19-136, IS-95, Japanese PDC 혹은
PHS, IMT-2000 시스템). 이는 수많은 에어 인터페이스(44 interface)7} 존재하고 대부
분의 이동전화 사용자들이 여러 개의 이동단말기를 들고 다니고 싶어 하지 않기 때문
이다.

이 책의 독자들은 어떤 통신시스템-무선전송기법이든 다중접속기법이든간에-도
4148이나 C3} 같은 프로그래밍 언어로 AA 수 있음을 이미 알고 있다. 이들 컴
퓨어 시뮬레이션 언어는 298. FPGA, ASIC} 같은 DSPHS 구성하기 위한 소프트웨
어 언어와 깊은 관계가 있다. DSPHS 위한 전형적인 소프트웨어 언어로는 VHDL}
Verilog HDL°| 존재한다. DSPHE 이동통신시스템의 이동단말기와 기지국의 디지털
하드웨어를 구성하는데 사용되어왔다. DSPHE 범용이고 구성은 29" 소프트웨어
(2679)를 다운로덩함으로써 프로그래밍될 수 있다. 이는 사용자가 단지 하나의 단말
기의 DSPH4] 원하는 기본적인 요소를 기술하는 2888를 다운로드할 수 있음을 의미
. 한다. 이 점이 소프트웨어 무선 통신시스템의 기본 개념이다.

439



===== PAGE 439 =====
최신 이동통신시스템

a

440

Mobile Communications using MATLAB Simulation

가까운 미래에 소프트웨어 무선설비의 실현이 완벽하게 완성되면, 이동단말기 제조
ASE 특정 이동통신 소자의 스펙에 무관한 생산품을 만들 수 있을 것이다. 이는 사용
자가 원하는 사업자를 선택할 수 있음을 의미 한다 (예 : 사용자가 한 셀룰러 영역에서
어떤 사업자의 용량이 가득 찬 것을 알게 되면 사용자는 동일한 셀룰러 지역에서 다른
사업자를 선택할 수 있다). 또한 생태학적인 관점에서도 이득이 된다. 소프트웨어 무선
설비는 하드웨어의 GS 줄여 산업 쓰레기를 감소시킨다. 게다가, 제조사의 비용절약
의 관점에서, 게조사는 단말기를 판매하는 대신 이동단말기의 DSPH FAS 위한 소프
트웨어만을 판매하면 된다.

108에 기초한 무선 통신시스템의 연구는 1990년대 초반에 시작되었다. 그러나 초
기의 연구는 재구성 가능한 무선 통신시스템의 관점에서 29『기반 무선 통신시스템을
AES) 않았다. 우리가 알고 있는 바로는, “소프트웨어 무선설비”라는 BOS 처음
사용한 논문은 Mitolao|t} [1]. 4411018는 소프트웨어 무선설비의 기본적이고 기능적인
PAS 기술하였다. 또한, 하나의 원형으로 군사용 무선설비 SPEAKeasy7} 소개되었
U} [2]. SPEAKeasy= 다수의 음성과 데이터 군사용서비스를 사용할 수 있으며 주파수
대역은 2 MHz2 012이다.

궁극적인 통신시스템을 구현하기 위한 대부분의 연구는 (1) DSPHY] 구조, (2) 아날
로그 신호처리 하드웨어, (3) 하드웨어에 소프트웨어를 다운로딩하는 방법, (4) 소프트
웨어 무선설비의 응용 방법에 SAS 두어왔다 [3-7].

이 장은 이 책에서 공부한 소프트웨어 프로그래밍 방법을 독자들이 앞으로의 디지털
하드웨어 구축과 관련된 응용력을 기르게 하기 위한 목적으로써 소프트웨어 통신시스
템을 소개한다. 소프트웨어 무선설비의 개념은 소프트웨어 프로그래밍과 실제 하드웨
어 구현의 가교 역할을 한다. 이 장은 다음과 같이 구성되어 있다: 8.2장에서는 소프트
웨어 무선 통신시스템이 무엇을 의미하는지 정의한다. 8.3장에서는 소프트웨어 무선
통신시스템의 장점을 열거하고 8.4장에서는 실제 시스템의 구현에 있어서의 장벽을 열
AM. 8.5장에서는 소프트웨어 무선 통신시스템의 기술에 대해 기술한다. 8.6장에서
는 현재의 소프트웨어 무선설비 연구에 대해 살펴보고 8.7장에서는 소프트웨어 무선설
비 기반 통신시스템의 앞으로의 응용에 대해 논한다. 8.8장은 이 장을 마무리한다.



===== PAGE 440 =====
8&개

구성을 보여준다. 무선설비는

=

[1]에서의 소프트웨어 무선설비의 기

은
u

3134 8.1

aunjonsjsejyju! UOWWOD

|
asemyos  T |       oS  i:   a.   wos  + |       1068  11   8.  os  1       1068 i   aiemyos  t   B1eMYOS
(000                           (now)                       (gva/90v)        (nal)                    :
yun             (nol)           yun                           yun            yun           (niu) | 홈
Buissaooid            yun             jouoo ft        (0188)   1290     via [< 140480004[         yun
6비140        10비658201이 | uolssiw          yun            pue          ajeipaw       Aduanbayy         yun
048-01-003| |  0/          “| -suedy        *lpueqaseg) |  0/0     | 701             oipey | 호 | euuaquy
(8)              (2)             (9)             (9)             (v)             (이             (2)      더      (i)
를

A

소프트웨어 무선설비의 기본 구성

를 그림 8.1

441


===== PAGE 441 =====
Zy 최신 이동통신시스템
C

Mobile Communications using MATLAB Simufation

(1) 안테나 장치, (2) 무선주파수 신호처리 장치 (RFU), (3) 중간주파수 신호처리 장
치 (IFU), (4) 아날로그10 -디지털 변환 (&10()와 디지털10아날로그 AS (DAC) 장치
(ADC/DAC), (5) 기저대역 신호처리 장치 (BBU), (6) 전송제어 장치 (TCU), (7) 입력/
출력 (VO) 처리 장치 (OU), (8) end-to-end 타이밍 처리 장치 (TPU)°] tt.

각 장치는 자세하게 기술될 것이다.

8.2.1 안테나 장치

하나의 단방향, ASA, 광대역 안테나가 필요한데 이는 다양한 통신시스템에서 At
용될 수 있기 때문이다. 또한, 배열 안테나에 기반한 신호처리 기술은 주변 환경에 따라
소프트웨어 무선설비의 기능을 선택하고 소프트웨어 무선설비 기술을 사용하여 최적
의 알고리즘을 선택할 수 있도록 할수 있다. 이러한 안테나를 스마트 안테나 혹은 소프
트웨어 안테나라고 부른다 [8-10]. 소프트웨어 안테나는 SDMA® 수 있는데 여기에서
안테나는 선택된 사용자의 방향으로 빔을 구성한다. 다중접속은 안테나의 방향을 바꾸
거나 간섭 제거에 의해 구현되는데 여기에서 안테나는 원하는 사용자 방향으로 향하거
나 원하지 않는 사용자나 신호에 0111 pointS 할당한다.

8.2.2 무선주파수 신호처리 장치 (RFU)

송신기의 680에서, 중간주파수 장치 080)나 기저대역 장치 (8800)로부터의 신호
주선주파수 (RF) 대역 ASS 상향변환(40000600되고 증폭되어 안테나 장치로 전
된다. 수신기에서는, 안테나 장치에 의해 수신된 신호는 신호처리에 적합한 상수 레
로 증폭되고 때 대역이나 기저대역으로 직접 하향변환(00\0000600된다. 신호처리
아날로그 희로로 행해진다. RF 증폭기의 선형성이나 효율과 수신기에서 낮은 주파
대역으로의 변환 방법이 주 논점이다.

ofy rr

벨

4y fe

8.2.3 중간주파수 신호처리 장치 (IFU)

이 장치에서, 400/040로부터의 신호는 IF 대역으로 상향 변환되어 증폭되고 수신

442



===== PAGE 442 =====
기의 RFUZ 전달된다.

수신기에서, RFU 장치로부터의 ASE IFUA 신호처리에 적절한 레벨로 증폭되
aLADC/DAC 장치나 기저대역 장치에 적합한 주파수로 직접 하향 변환된다. 수신기에
서 다수의 시스템의 신호가 수신될 때, 원하는 주파수 대역이 필터를 사용해 선택되어
야 한다.

8.2.4 아날로그10 -디지털 변환 (ADC) 디지털[0-아날로그
(DAC) 장치

이 장치에서, 기저대역 장치로부터의 디지털 ASE DACE 사용해 아날로그 신호
로 변환되고 변환된 ASE 보다 높은 주파수 대역 장치 (FUU RFU)& 전달된다. 수

신기에서, FU} RFUE7E]2] ALS ADC] 적합한 레벨로 증폭된다. 안정화된 신
SE ADC 의해 샘플링되고 디지털 ASE 변환된다. 이 장치에서는, 샘플링 방법이
중요한 기술이다. 8.5.2장은 세 가지 중요 샘플링 방법에 대해 설명한다.

8.2.5 기저대역 신호처리 장치 (BBU)

이 장치에서, 데이터는 디지털로 변조되고 수신기의 ADC/DAC 장치로 전달된다. 전
송된 데이터는 400/2ㅁ040 장치로부터 샘플링된 신호와 디지털 신호 처리를 사용해 수
신기에서 복원된다.880의 기본 구성을 그림 8.2에 보였다[2]. 송신기의 880에서, =
레임, 코딩, 맵핑, 변조, 전송필터 블록이 중요 블록이다, 반면, 수신기의 880에서는
수신기 필터, 코드와 심볼 타이밍, 샘플링 레이트 변환 (재샘플), 디맵핑, 복조, 디코딩
블록이 중요 블록이다.
또한, 수신기의 880에서는, 페이딩 2 (equalization) 블록과 원치 않는 신호를 제
거하기 위한 간섭 제거 블록이 존재한다. 대부분의 경우 880는 298 FPGA, ASIC>}
같은 다수의 DSPHS 사용하여 구성된다. 모든 요소 3S Verilog HDLo]4} VHDL
로 씨어진 2688를 사용해 기술되고 컴파일 된다. BBUS] 구성은 DSPSS 변화시킴으

로써 변화시킬 수 있다.

tA

443


===== PAGE 443 =====
777

은근 089 alc 28 ROE

0000 eae ee a ae

eee Coding method |

, and           1
pa a mt i idan size

Output
(ich and
Qch from

input

| coefficient
: 00008 000

Input                          Reto         iS
Ich and                        a Ra                                       =             ee
eh or                    >| correlation} >                       [Denepring od            oo
IF unit)                            ne                               ee  B domoditation                T ach)

UOREINUS FA LLVIN BUISN SUOHBIIUNUIWOD 97907

re

{Slo

re

>
of

ly



===== PAGE 444 =====
8.2.6 전송제어 장치 (TCU)

이 장치에서, BBUS 위한 입력 비트 스트림 BA) 2 media access control (MAC) 계
층(18760)의 전송 프로토콜을 조절함으로써 수신기에서 구성되고, 수신기에서 880로
부터의 검출된 데이터는 MAC 계층의 전송 프로토콜의 데이터 형식에 따라 검사된다.
만약 검출된 데이터에서 비트 오류의 수가 크면 재전송이 요구된다. 이 전송제어에 따
라, 이 장치는 암호문을 다룰 수 있다. 대부분의 경우, TCUS 290브로 구성될 수 있고
모든 요소 BSS DSPSS 사용해 기술될 수 있다. DSPSS 변화시켜, 700는 전송 =

콜을 사용자가 원하는 것으로 구성할 수 있다.

8.2.7 입력/출력 (1/0) 처리 장치

이동국에서, 모든 정보 데이터는 휴대폰, PDA 단말기, 개인용 컴퓨터 등으로부터

모든 수신 데이터는 이들 단말기나 컴퓨터로 되돌아간다. 10와 타이밍은 외부 단말
기와 융통성 있게 연결될 수 있도록 관리된다.

to

Bil

8.2.8 EndtoEnd 타이밍 처리 장치 (TPU)

이 장치는 송신기와 수신기 간의 AS 지연을 제어한다. 예를 들어, 음성의 AS
은 150 ms 이내여야 한다.
부부의 소프트웨어 무선 시스템에서는, 이동통신용 소자를 DSPS 언어로 기술하
는 몇 가지 소프트웨어 프로그램이 DSPHS] 소자를 구성하기 위해 사용된다. 이 소프
트웨어는 특정 시스템의 요구를 만족시킬 수 있도록 쉽게 변환 가능하다. 이런 소프트
웨어 무선 시스템을 완전-다운로드형 (801100\1010807906)소프트웨어 무선 시스템이
부른다. 그럼 8.3은 완전-다운로드형 소프트웨어 무선 시스템의 구성을 보여준다.
시스템은 820, IFU, BBUS 기본 시스템으로 갖는다. 또한, 수신기와 관련된 TX 모듈
과 수신기와 관련된 RK BSS 갖는다.
특정 이동통신 시스템을 완전-다운로드-형 소프트웨어 무선 시스템으로 구현하기 위
해서는 무엇보다 통신 시작 전에 모든 필요한 DSPS7} 880에 다운로드 되어야 한다.

bs
ra

|

445


===== PAGE 445 =====
최신 이동통신시스템

446

Mobile Communications using MATLAB Simulation

프레임 블록, 부호기 블록, 맵핑과 변조 블록, 필터 SS (2H 8.2)S 포함한 2878 블록
이 TX 모듈의 BBU 다운로드 된다. 필터 블록, S37] (equalizer) 블록, 검출기, 복호
기 블록 (그림 8.2)를 포함한 DSPS 블록 HF DSPS= 기술되고 RX 모듈의 880로 다
운로드 된다.

Spare                     To           From         Digital
TX module        RX module          signal
of IFU               of IFU              processing
software
ich      Qch        Ich | Qch

4 Filter Jel Filter I

1 | Modulator | | | Equalizer | ㅣ
010 | |

1 | Frame | [ Detector |

;          tl      i"
|: [Encoder] 1s [Decoder ] +

~ =

Quadrature] ; 1|Quadrature
modulator || '|demodulator

ce

From TX module ToRX module of Fromdatagen. Output data
of baseband unit baseband unit

를 그림 83 완전-다운로드-형 소프트웨어 무선 AAO 구성

소프트웨어가 다운로드 된 후, 구성 검사 프로그램이 실행된다. 그 다음 280가 필요
한 기저대역 변조와 복조 회로를 구성한다. 그 후, 전송 데이터가 TX 모듈의 880에 입
력될 수 있다.

TX 모듈의 880에서, 데이터는 위에서 언급한 DSP BES 사용하여 프레임으로 a
성되어 AS] 5 in-phase 채널 (Ich) z} quadrature-phase 채널 (Qch)2] 두 신호로 변환
된다. 이 신호들은 TX BS FUS 입력된다.

TX 모듈의 FUN, 디지털로 AAS Ich} 002의 ASE D/A 변화기 블록에 의해
디지털에서 아날로그로 변환된다. 이 신호는 때 대역에서 직교변조된 것이고 7% 모듈
의 RFUZ 보내진다. TX 모듈의 00에서 직교변조된 ASE 전송되기 전에 파워제어



===== PAGE 446 =====
부분에 의해 RF 대역으로 상향변환 된다.

RF 신호를 수신하기 위해, 먼저, 수신신호는 RX BSS] RFU] 입력된다. 여기서,
신된 RF 데이터는 대역통과-필터링 되고 의사신호를 제거하고 대역으로 하향변
환 된다. 자동 이득 제어 (AGC) 블록은 하위변환된 신호의 파워를 일정 레벨로 유지한
다. (. oe pe ALS RX 모듈의 FFUS 입력된다.

B39 UA, 000도부터의 수신 ASE An Bt BSS Any Ich3}
(로 분리된다. 그 다음 A/D 변환 블록은 이를 오버샘플
—
모듈의 880에서, 모든 이동 통신 소자 블록은 통신 시작 전에 DSPHE 구현되
고 구성은 테스트 프로그램을 통해 검사된다. 오버샘플링 된 10과 QchE 특화된 방법
으로 필터링되고 등화되고 #※ 모듈의 880에서 필터와 등화기, 복호기 BSS 사용해
검출되고 복호된다.

MEM) 소프트웨어 무선 통신시스템의 이점

완전-다운로드형 소프트웨어 무선설비에서, 시스템음 소프트웨어를 변화시킴으로

써 요구에 따라 변할 수 있다. 말할 필요도 없이, 운영자나 사업자뿐만 아니라 정부나 소
비자에게도 많은 이득이 있

특별히, 상업적인 운영자와 서비스제공자의 이점은 다음과 같다:

2H

01) 글로벌 로밍 서비스;
@ 엽그레이드할 수 있는 단
(3) 단말기의 변화 없이 새로

@)생산품의 리콜 없이 버그 수정
Ouse 소프트웨어 (즉, 이등단말  기뿐만 아니라 다른 전자제품에 인스톨될 수 있
는 무선 Mies cet 이는 이동 사용자뿐만 아니라 다른 기기의 사용자도 소
프트웨어 무선설비 제공자에 접속할 수 있음을 의미한다.

기:
서

다모
=
로우

오행

비스의 추가;



===== PAGE 447 =====
글 최신 이동통신시스템
Mobile Communications using MATLAB Simulation

정부에게는 다음과 같은 이점이 있다:

Dav Ae 글로벌 로밍 서비스를 제공할 수 있다.

QUAI 관점에서, 소프트웨어 무선설비는 하나의 이동단말기만을 필요로 하므
로 하드웨어를 제거한다. 이는 산업 쓰레기의 양이 감소될 수 있음을 의미한다.

@ 무선 법에 근거하여 단말기의 인증이 쉬어야 한다. 궁극적으로, 단지 소프트웨어
만 인증되어야 할 수 있다.

소비자의 이점은 다음과 같다:

01) 무제한 글로벌 로밍;

@ 많은 서비스를 위한 하나의 단말기;

(3) 하드웨어 업그레이드 없이 새로운 서비스의 제공;
© 단말기의 교체 없이 새로운 서비스의 추가;
OAS 리콜 없이 버그 수정.

[| 소프트웨어 무선 통신 시스템의 문제점

8.3장에서 살펴본 바와 같이 소프트웨어 무선설비에는 많은 장점이 존재한다. 그러
나 소프트웨어 무선 기술은 다음과 같은 문제점들을 극복해야만 한다.

0요구되는 이동 통신 구성요소 SSS] 내용이 복잡해짐에 따라 SPH] 다운로드 되
는 소프트웨어의 부피가 증가한다. 이 결과, 다운로드 시간이 증가한다. 또한, 다운
로드 프로그램의 SH] 방해신호에 대한 강성 혹은 페이덩이 WAS BFS
부호화를 위한 과잉 코드가 다운로드 소프트웨어에 추가되어야만 한다[11112].

(9) 요구되는 이동통신 구성요소 블록의 내용이 복잡해짐에 따라 DSPHS| 구성 검사
에 필요한 시간도 증가한다. 이 문제는 구성 검사에 필요한 충분한 시간이 없을 경
우 DSPHS| 작동 특성의 안정성에도 영향을 미친다 [11, 12].

448



===== PAGE 448 =====
@다운로드 된 소프트웨어에서, SS ABM 특유의 기술을 포함한다수의 구성요소
블록이 존재한다(예, 특별한 BSS 위한 최적화 방법이나 계산 알고리즘). 소프
트웨어가 다운로드 될 때 이러한기술이 HST 수 있다. 또한 이러한 기술이 변경
될 가능성도 존재한다 [11, 121.

위에 언급한 문제 이외에도, 소프트웨어 무선설비가 기저대역 장치뿐만 아니라 RF
와 IFUS 제어한다면 다음과 같은 문제가 고려되어야 한다.

OQ 소프트웨어 무선설비를 사용하여, 사용자는 특정 통신시스템을 구현하기 위한
하드웨어의 기본적인 구성요수를 기술하는 소프트웨어만을 다운로드 할 수 있
다. 그러나 다른 주파수 대역에서 작동하는 다수의 통신시스템을 소프트웨어 무
선 기술을 사용해 하나의 이동통신 하드웨어로 통합하면, 이동통신 단말기는 다
수의 안테나 장치, RFU, IFU, ADC/DAC 장치들이 필요하다. 게다가 사용자는
다수의 시스템을 동시에 사용하기를 원할 수 있는데 [13], 이 경우에는 다수의
ADC/DAC 장치, 기저대역 장치, 전송제어 장치, 10처리 장치, end-to-end 타이
밍처리 장치가 준비되어야 한다. 다수의 장치를 관리하기 위한 방법이 고려되어
야만 한다.

@ 다른 주파수 대역에서 작동하는 다수의 통신시스템이 소프트웨어 무선 기술에
의해 하나의 이동통신 하드웨어로 집적되면, 광대역 안테나가 사용되어야 한다.
그러나 안테나의 대역폭은 제한되어 있으므로, 다수의 안테나가 필요하다. 단말
기 내에서 이들 안테나의 배치는 중요한 고려사항이다.

또한, 전체 시스템의 관점에서, 다음 문제들이 발생한다.

0 하나의 소프트웨어 무선 단말기에 어떤 서비스가 집적되어야 하는가? 다중모드
단말기가 각 통신시스템을 이를 위한 특정 4910의 개발과 이들 ASICS 하나의
회로보드에 계획함으로써 쉽게 구현할 수 있다고 하자. 이 경우, 소프트웨어 무선
기술은 필요치 않다. 그래서 소프트웨어 무선 기술은 많은 통신시스템이 필요한

응용분야를 목표로 해야 한다.

449


===== PAGE 449 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

(0) 소프트웨어 무선 기술이 사회적으로 어떻게 그리고 어떤 분아로 인식되어야 하
는가? 소프트웨어 무선 기술은 많은 응용이 존재한다. 이런 응용들이 정리되어야
한다.

(3) 표준화는 어떻게 그리고 어떤 분야에서 정리되어야 하는가? 바이러스나 해커로
부터 어떻게 보호되어야 하는가? 특히, 단말기의 교환 없이 소프트웨어를 200
켜 국제 로밍을 가능케 하는 소프트웨어 무선설비의 기능은, 무선통신^
재구성할 수 있는 바이러스가 포함되는 경우 중대한 위협이 된다. 간단한 예로 송

한,

신기가 수신기와 결합되지 않는 재구성된 단말기가 있다. 또한, 바이러스가 규정
보다 훨썬 높은 레벨로 전송 파워를 변화시켜 전 세계의 모든 무선통신시스템을

정지시킬 수 있다. 참고문헌 [14]는“무선 테러리즘”을 언급한다. 무선 테러리즘

에서, 소프트웨어 무선설비의 모든 사용자는 효과적으로 잠재적인 테러리스트가

된다. 그러한 사고를 방지하기 위해, 표준화가 이뤄져야 한다. 더불어, 소프트웨

어 무선 단말기를 검증할 조직과 무선설비가 개발되어야 한다. 이런 이유로 소프
트웨어 무선설비는 무선법에 새로운 패러다임을 제공한다.

| 소프트웨어 무선 통신시스템의 기술

450

우, 다수의 광대역 안테나와 이들 다른 주파수에 적합한 다수의 RFU} 수신기에 준비
되어야 한다. 그러나 통합된 통신시스템의 주파수 차이가 크지 않다면, 하나의 안테나
가 주파수 대역을 감당할 수 있다. 그러나 800와 80가 그림 8.4(@에서처럼 헤테로다
인 형이라면, 다수의 880가 필요하다. 이 경우, 동일한 주파수 대역에서 새로운 시스템
이 서비스되면 새로운 RFU7} 준비되어야 한다. 결과적으로, 아날로그 희로의 크기가
감소되어야만 한다.



===== PAGE 450 =====
Antenna

를 그림 8.4 직접 변환 방법: (a) 헤테로다인형 구현 (6) 직접-변환형 구현

직접 변환 방법은 이 문제를 해결할 수 있다[15, 16]. 그림 8.4(06)는 기본 구성을 보여
주고, 그럼 8.5는 공정을 보여준다.

먼저, 목표 중심 주파수와 목표 대역폭이 선택된다. 직교 복조기와 허수 배제 필터를
사용하여, 대역폭은 RF 대역에서 기저대역으로 직접 ABS 수 있다. [그림 8.5)

8.5(6)참고.] 그 다음, ADCS 사용해, 수신신호를 목표 대역폭의 두 배로 샘플링한다.
[그림 8.5(0) 참고.] 요구되는 통신시스템을 위해 요구되는 채널은 샘플링된 데이터로
부터 디지털로 필터링 될 수 있고 신호는 기저대역 장치에서 직교 복조기로 복원된다.
직접 변환 방법을 사용하여,&80의 수는 그럼 8.4에 보인 바와 같이 감소될 수 있다. 그
러나 높은 수신^신호-레벨 입력이 목표 대역폭에 들어올 때마다 다이내믹 레인지가 감
소한다. 또한, 빼에서 기저대역으로 변환한 후에 믹서의 비선형성에 의해 야기되는 2
차 왜곡과 de 옵셋에 대한 문제들이 존재한다. 직접 변환에 대해 소프트웨어 무선설비
에 기반 한 통신시스템에 적용하기 위한 기술을 다룬 많은 논문과 시도들이 있었
다.[15-17] 가까운 미래에, 광대역과 다중대역 직접 변환기가 실용화 될 것이다.

0 25
TEES

451


===== PAGE 451 =====
최신 이동통신시스템

Mobite Communications using MATLAB Simulation

ee sen it —                        Adjacent system
' chich? ch3ch4 ch5ch6 ch7ch8

ㆍ (00000

Target center Bing (F,)

XU} Quad. demod.

Ve FS Rechach ch2chi
0
(DC)
U} Analog-to-digital conversion
Digital channel-selection by filter
chi
Ta   1
1
1       >»
7                          호
(00)

를 그림 8.5 직접 변환의 공정

8.5.2 샘플링 방법

소프트웨어 무선 기술로 다중모드 수신기를 구현하기 위해, 샘플링이 RFU, IFU 혹
은 880에서 행해진다. 이 장에서, 이들 샘플링은 각각 8 샘플링, 내 샘플링, 88 샘플
링이라 불린다.

그림 8.6은 이들 샘플링 방법을 보여준다. 88 샘플링의 경우, 모든 계산은 기저대역
신호처리로 사용될 수 있는데 이는 주파수 변환과 다른 필요한 과정이 880와 00의
아날로그 신호처리 ait 끝났기 때문이다.

그러나, 때와 08 샘플링의 경우, 신호처리 섹션의 부담이 증가해서 감소되어야만 한
다 [1820]. 샘플링 방법은 다음과 같이 분류할 수 있다: (1) Nyquist ASA, (2) 오버샘
플링, (3) 언더샘플링.

ot!

452



===== PAGE 452 =====
Antenna
unit

(1) Nyquist 샘플링

샘플링 주파수 /,는 입력신호의 최대주파수보다 두 배 크다. 그림 8.7은 Nyquist 샘
플링 방법을 보여준다. 그러나 이 샘플링 방법은 급격한 감쇄 특성의 안티-앨리어싱 필
터를 필요로 한다.

BW                                                          BW |

ㅣ
|        1

(a)

*        f, + BW/2                                           ate +BW/2         A
~

ㅣ                       =26.+8\/2)                   psig
|    ㅣ     ㅣ
ib)
를 그림 8.7 Nyquist 샘플링: (a) 기저대역 신호 (6) 대역-제한 신호.

—— — =

0
f,. center frequency

~

453



===== PAGE 453 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation
(2) 오버샘플링

샘플링 주파수 fc Nyquist FSO 주파수보다 높다. 그림 8.8은 이 방법을 보여준
다. Nyquist 샘플링과 비교해, 안티-앨리어싱 필터의 절단이 급격할 필요가 없다.
수                                   4               f

< BW                          BW

+
ue
| V
iad
w
=
+
ad

>

al  + BW/2

Mid 88 오버샘플링: (3) 기저대역 신호 (6) 대역제한 신호.

~

3) 언더샘플링

샘플링 주파수 f= Nyquist 샘플링 주파수보다 길다. Nyquist 이론을 사용하여, 샘
플링 주파수가 Nyquist 샘플링 주파수보다 낮으면 앨리어싱이 발생한다. 그러나 이 경
우, RFS} IF ALS 9] 정보 YASS 대역-제한되어 있고 RFS 때 반송신호보다 훨씬 낮
다. 그래서 앨리어싱의 영향은 감소된다. 그러나 샘플링 주파수가 Nyquist 샘플링 주
파수보다 낮으므로, 샘플러의 대역-제한 입력신호와 샘플링 주파수의 관계는 매우 중
요하다. 샘플링 주파수가 AS, 대역-제한된 입력신호의 최저, 최고 주파수가 7, 과 /,
로 정의되면 요구되는 샘플링 주파수는 다음과 같이 주어진다 [20]:

섹       n—l                   (8.1)
여기서 n& 다음 조건을 만족하는 정수이고

454



===== PAGE 454 =====
l<nslf./,-f,)]                            (8.2)

Le |= *의 최대 정수를 의미한다.

언더샘플링을 그림 8.9에 보였다. 주파수 변환은 기저대역 근처의 정보신호가 선택
되었을 때 언더샘플링을 수행함으로써 동시에 행해질 수 있다. 위에 보인 바와 같이, 언
더샘플링은 장점을 가지고 있다.

그러나 (8.1)에 정의된 영역 oy 샘플링 주파수를 유지하기 어렵고, 때때로 클럭
이 지터060의 영향으로 변동한다. 그래서 앨리어싱이 여전히 존재한다. 앨리어싱의
발생을 줄이기 위해 안티-앨리어싱 필터 (AAF)7} 사용된다. 이러한 필터의 개발은 후
에 논할 토픽(10010)이다.

y Pa 1            다      f, + BW/2
BW

<>! ¢, satisfied (8.1)                                   qo
=>

|                 자 서시
T

>;       ~

f

c

Frequency
converted signal

를 그림 8.9 언더샘플링

85.3 샘플링 레이트 변환
른 주과수 대역을 사용하는 다수의 통신시스템이 소프트웨어 무선 기술을 사용해
하나의 이동통신 하드웨어로 통합되면, 그들의 심볼 레이트는 완전히 다르다. 만약 심
볼 레이트가 고정되어 있으면, 심볼 타이밍 오류가 발생한다. 이는 샘플링 레이트를
볼 레이트로 나눈 값이 정수가 아니기 때문이다. 결과적으로, 타이밍 지터나 슬립핑
(slipping)o] BY. 그림 8.10은 샘플링 레이트가수신신호의 심볼레이트의 정수배
인 경우와 정수배가 아닌 경우의 심볼 타이밍을 보여준다.

455



===== PAGE 455 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

Case 1
Integer
times

Case 2       :
Noninteger :
times          :

Sampling duration

※        Symbol timing
wees Optimum symbol timing which is the sampling data closest to the symbol timing
Meg ihe    Sampling timing except for optimum symbol timing

+>

Mie 8.10 샘플링 레이트가 수신신호의 심볼/칩 레이트의 정수배인 경우와 정
배가 아닌 경우의 심볼  ay

00

샘플 레이트 변환은 심볼 타이밍 오류를 방지하기 위해 행해진다. 그림 8.11은 이를
위한 간단한 방법을 HAD [211], 그럼 8.12는 샘플링 레이트 변환 동안의 주파수 스
펙트럼의 전이를 보여준다. 입력신호에 대해, 첫번째 샘플링이 샘플링 레이트 7, 으로
행해진다. x(kT7,): 4= 1, 2,…는 샘플링된 데이터이고 그 스펙트럼은 그림 8.12060)
와 같다. 2(47`,)는 샘플링 레이트 7,로 7(227`..): m=1, 2,…로 변환된다.

KT,                T,
xt) cP xlkT) : xt} 0 nie yit) tills

fe WF,               Ideal                    Lowpass 0 ™h
digital-to-analog                filter
converter

를 그림 8.11 샘플링 레이트 변환 방법

이를 위해, 샘플링 된 데이터는 20&0와 그림 8.12(0)의 전달함수를 갖는 저대역통과
필터를 사용해 아날로그 신호로 재구성되고 아날로스 신호 /(7)가 얻어진다. /(7)의
스펙트럼은 그림 8.12(0)와 같다. 아날로그 신호 7(?)는 레이트 7;,로 재샘플링되고
최종적으로 레이트 변환된 신호 y(mT,): m=1, 2,…를 얻게 된다. 이상적인 DAC
를 사용해 mT): m=1, 2, ~즈무터 ASAE 아날로그 신호 pW“) 스왁트렴은

456



===== PAGE 456 =====
그림 8.12(6)와 같다. 만약 저대역통과 필터의 임펄스 응답이 이상적이라면
y(t) = ×(/)이다. 그러나 디지털 필터의 구성은 시변이고 이상적이지 않다; 그래서
저대역통과 필터 과정에서 허수신호가 완전히 제거되지 않는다. 이런 이유로, 앨리어
싱이 y,(t)2] 스펙트럼에 포함된다. 이 앨리어싱의 BRE 샘플링 레이트 변환의 연구
토픽이다 [21].

00|
+         >f
VT,
(a)
ix      |               ;
~   2: ~
\        f    인 /
1/7,     20,
(b)
|H(f)| 4
J:   \
/     년
Pf     \
=      —   }      =e  > f
ho     ar,
(이
LAU

—> f

@ 그림 8.12 샘플
=

457


===== PAGE 457 =====
최신 이동통신시스템

A

458

Mobile Communications using MATLAB Simulation

샘플링 레이트 변환 기술을 이용해서, 샘플링 AMES 적응적으로 변화시킬 수 있
다. 그러나 샘플링 레이트 변환은 400, DAC, 저대역통과 필터를 포함한 아날로그 회
로에 의해 행해진다. 그래서 소프트웨어 무선설비에 사용되는 시스템의 수가 증가하면
레이트 변환 회로 역할을 하는 다수의 아날로그 소자가 필요하다. 단말기의 크기가 작
아야 하므로 아날로그 회로의 증가는 실용적이지 못하다. 그래서 기저대역 장치에서 고
정된 샘플링 레이트를 갖고 다수의 시스템에 적절한 심볼 타이밍을 찾는 적응 심볼 타
려되어야 한다. 이러한 방법 [22] 중 하나를 다음에 보인다.

신신호를 심볼 레이트로 WIM 비정수 시간 클럭을 갖는 수신신호를 샘

2”
oF,
o&
uk
si

10;
o&
ok,
rlo
> 범

ol,
ro
“4
해
내
전
고
412,
om,
»
ga
0:
때
ot
raul
aw
WW
다녀
oe
=
Bey,
00
ro,
mw
zy
So,
am,
we
\
Ze
prs
2}
BIL
N
SS

이트의 비정수 배의 샘플링 레이트로 샘플링될 때, 4 심볼 타이밍에 가장 가까
샘플 타이밍을 보여주는 최적 심볼 타이밍의 샘플링 WAS (8.3)과(8.4)로 a

lo Ho 때
4y by me
pinged

) =          ~ 06=
x(i) = round $ + O(i   »)                         (83)

O(i) = 든 + O(i -1) - round 응 + O(i- »)

= 는 + O(i -1)-x(i)                 (i21)                    (8.4)

여기서 0(2), C, SH round X)= 4 심볼 타이밍에 대한 최적 샘플링 타이밍의
샘플링 옵셋, 샘플링 레이트, 심볼/칩 레이트, ×의 가장 가까운 정수로의 반올림을 나
타낸다. 0(0)는 첫 번째 심볼 타이밍에 대한 샘플링 옵셋이다. (8.3)과 (8.4)로부터,
x(i) 2] 값은 다음 두 가지 경우로 제한된다:

A=round(C/S)
x(i) =         |  A+1:C/S is lager than round(C/S)

A-—1:C/S is smaller than round(C/S)          (8.5)



===== PAGE 458 =====
명은[22]에 제시되어 있다. 그래서 그림 8.10에 보인 사이클 슬림에 의해 야기되는
밍을 찾고 최적 심볼 타이밍의 샘플링 WAS 갖는 적절한 패턴을 찾기 위해

모든 패턴을 알아야 한다. 그러나 상태 패턴의 총 수는 관측된 심볼의
3 1 기오  이는 기저대역 장치에 많은 부담을 증가시키므로 총 상태 패
}소되어야 한다. 상태 패턴은 세 가지 중요한 특징을 갖는

ㅁ쓰
고 0
<=

re 해
= 을
고

at    4
rok
     10

am +} +f

0) 상태 패턴에서 4 수신의 최대 수 Me 1/|T| 보다 작은 최대 정수이고 TE
오버샘플의 수와 오버샘플의 +S 가장 가까운 정수로 반올림한 값의 차
[ = C/S— 702220( </,5 )]이다.

(2) 4 수신의 최소 수 NS 24보다1 작은 N= /4ㅡ1이다.

(3) B= 상태 패턴에서 반복되지 않는다.

명은 [22]에 존재한다. 이 특징을 사용해, 상태 패턴의 전체 수를 급격하

그림 8.13은 상태 패턴 생성기를 보여준다. 목표 통신시스템의 정보가 A, 2, 44 N
산하기 위해 주어진다. 주어진 정보는 샘플링 레이트, 심볼/칩 레이트, 관측된 심
볼의 수이다. 결과 A, 2, 44, NZ 상태 패턴 생성기로 입력된다.

Number of observation symbols
Sampling rate
Symbol/chip rate
네루 ie                i

c |          8
y  : f                     6     *
A=round(C/S)                                                                                               :

|       10011                            6                8                             |T =C/S — round( C/S)]

A=C/S — round(C/S)
B=A+1:C/S is larger than round(C/S)             M = fioorfaba(1/7))

A-1: C/S is smaller than round(C/S)
[N=M—1|
2 €    게 ^              By        M  4

State pattern generator                                       |

Output device
| Output |                                of state patterns

+
를 그림 8.13 상태 패턴 생성기

459



===== PAGE 459 =====
ZY 최신 이동통신시스템

Mobile Communications using MATLAB Simufation

그림 8.14 상태 패턴 발생기의 SHES 보여준다. 이 생성기에서 사용되는 조건은
다음과 같다:

01) A 수신의 반복은 24보다 크지 않다.
@ #의 이웃은 항상 이다.
@@ 두 2 사이의 4의 반복의 수는 보다 크다.

Input Z, C, S

Calculate
A,B, T,M,N

X={A, B}
Is the length of all
elements of X equal to 2?
NO
Output the

elements of X            Pick up the patterns s
from X

!
|  X=XUfs A}  |

Does {s A} satisfy
the conditions ?

Does {s B} satis
the conditions ?

NO

를 그림 8.14 상태 패턴 생성기의 흐름도

이들 조건은 초기 획득에서 A 번째 샘플링 옵셋 0(0)에 대해 조건
(-0.5 < 0(0) < 0.5)를 포함한다. SHES 과정을 따라 상태 패턴의 수를 줄일 수
있다.

460



===== PAGE 460 =====
심볼 타이밍 아그   기술된 =o 의한 이 상태 패턴에 기반 = ie
8.15는 그 흐름             가 션신호

이밍 추정 블록은 aa aia 파워를 갖는 적절한 상태 패턴을 결정하기 위해 maximum
likelihood 6801048007을 사용한다. 선택된 상태 패턴이 보여주는 샘플링 데이터는 각
복조 블록에 최적 심볼 타이밍의 출력이다. 이 동기화 HHS 심볼 레이트의 정수 혹은
비정수 배의 샘플링 레이트로 샘플링 된 수신 데이터의 최적 심볼 타이밍을 적응적으로
찾는다.

Adaptive symbol timing

synchronization unit
[oe eee1
*,    대                  1
Pulse            |              Synchronization
| shaping        +——>| — timing estimation      sep eee
filter             ㅣ              머006                               ' Each demodulation
                         j                        | block
|                                                  1
!                                                  |
wee            State pattern                  ㅣ
[ 0004010  t  ~          generator block              |
1
Ss a ee「

상태 패턴의 생성의 한 예로, 미래 지능형 전송 시스템을 위한 다중모드와 다중서비
스 시스템으로 통합된 세 개의 시스템 GPS, electric toll collection (ETC), PHSS 고려
해 보자. 표 8.1은 각 시스템의 인자를 보여준다.

E818 시뮬레이션 모델

시스템      주파수            변소          데이터 레이트        대역폭
PHS         1.9-GHz 대역        zt / ADQPSK                    384 Kbps             300 kHz/1 channel
TDMA-TDD
GPS          1.5-GHz 대역         BPSK+                            50 bps                  1.023 MHz
DS-SS
ETC         5.8-GHz               ASK (Manchester code) | 1,000 Kbps           Less than 8 MHz



===== PAGE 461 =====
Rx 이동통신시스템
Mobile Communications using MATLAB Simulation

1S 레이트가 GPS 시스템의 클럭 레이트의 32배일 때 ETC} PHS 신호를 위해
생성된 상태 MAL 다음에 보인다. GPS 시스템의 칩 레이트가 세 가지 시스템의 심볼/
칩 레이트의 가장 큰 값이고 관측된 심볼의 수가 10이므로, ETC ASS 위한 상태 패턴
특성은 다음과 같다

A

(심볼 레이트) = 1,000,000
(샘플링 레이트)= 32,736,000
ㆍ 4 (샘플링 간격 11 = 33

ㆍ 2 (샘플링 간격 22 = 32

ㆍ 7`(샘플링 옵셋)=-0.2640

ㆍ M(AS| 최대 반복 수" =3

ㆍ 2/(ㅅ의 최소 반복 수) = 2

ㆍ (관측 AES F) = 10

상태 패턴은 다음과 같다:

DAAABAAABAA
@AAABAABAAA
@AAABAABAAB
@AABAAABAAA
OAABABABAAB
@®AABAABAAAB
@MAABAABAABA
®ABAAABAAAB
OABAAABAABA
@MABAABAAABA
@MABAABAABAA
®@M®BAAABAAABA

462



===== PAGE 462 =====
08ㅅ4ㅅ484ㅅ4ㅅ804ㅅㅅㅅ
@BAABAAABAA
®BAABAABAAA
@®@BAABAABAAB

PHS 신호의 상태 패턴 특성은 다음과 같다:

* 9(심볼 레이트)= 192,000

* (2(샘플링 레이트)=32,736,000/5 (after decimation of every 5 samples)
z

ㆍ 2 (샘플링
ㆍ 2 (샘플링 간격 22 = 35
플링

N
고

iN
ㅁ쓰

상태 패턴은 다음과 같다:

DBAAAAAAAAB
@BAAAAAAAAA
@ABAAAAAAAA
@AABAAAAAAA
OAAABAAAAAA
O©®AAAABAAAAA
@MAAAAABAAAA
®AAAAAABAAA
@AAAAAAABAA
@MAAAAAAAABA
@AAAAAAAAAB

~ O

463



===== PAGE 463 =====
ZY 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

시뮬레이션 ADS ETCH} PHSS] 총 상태 패턴의 수가 2""패턴에서 각각 163} 11 패
턴으로 감소할 수 있음을 보여준다. Maximum likelihood estimation 기반 한 심볼 타이
8 동기화 방법과 결합한 보다 적은 패턴은 최적 심볼 타이밍이 고정된 샘플링 레이트
하에서 얻어질 수 있음을 의미한다.

더

8.5.4 DSPH 구조

많은 시스템이 혼재한 18에서, 소프트웨어 무선 기술을 사용한 다중모드 소프트웨

무선통신 (MSR) 시스템이 하나의 단말기를 효과적으로 사용할 수 있다. 기본적인
시스템 구성은 완전 다운로드 형이다 (그림 8.3).

이 Ao] 집필되는 동안에도 개개의 소프트웨어 구성요소와 시제품에 대한 MSR A
구가 진행 중이다 (8.6장 참고). 그러나 소프트웨어 무선설비는 하나 이상의 통신시스
템을 동시에 사용하는 경우, 예를 들어 118의 경우, 구현하기가 매우 어렵다. 표 8.2는
일본에서 차량에서 사용되도록 YEP ITS 통신 시스템을 열거한다.

8H 8.28 ITS 시스템에 사용되는 통신시스템

범주                                           제어                                                                                   방종
시스템      GPS      VICS      EIC       라디오       방송       TV       위성
주파수         1.5 GHz       4 대역 | 5.8 GHz | 0.5-0.6 MHz | 76-90         90-222,       11.7-12.0
MHz            470-770       MHz
HHz

변조                BPSK +          LMSK          ASK            AM                      FM               VSB-AM | FM
DS-SS                                                                                               FM              PSK

데이터 레 | 50 bps           16Kbps | 1,024         아날로그           아날로그 ㅣ 아날로그 | 아날로그

이트                                                        Kbps

대역폭     1.023       100kHz | 8 MHz    15           200 kHz | 6 MHz    27 MHz
MHz                                                    kHz/channel

우선순위 |i                     3                  3                 3                        3                  2                  2

464



===== PAGE 464 =====
서비스는 세 가지 분아로 UPa 수 있다 [23]:

Das 운행하는 동안 항상 필요한서비스;
@언제나 꼭 필요한 서비스:
@사용자에 의해 선택되는 서비스:

표 8.2의 시스템에 위 분류 방식에 사용하여 우선권이 주어진다. 178를 위한 소프트
웨어 무선 시스템은 다수의 서비스에 동시에 접속하는 사용자의 필요를 분명히 한다.
미래의 ITS 시스템은 하나 이상의 서비스를 제공할 것이고 이는 다중모드 다중서비스
소프트웨어 무선통신 시스템 040498)이다 [13].

10046&시스템은4개의 하위시스템이 있다[131.신호처리는00489료시스템의 각 하
위시스템의 신호가 디지털이라는 조건 하에 행해진다.

0) 하위시스템 1: BBUS] DSPH7} 소프트웨어 무선통신 시스템의 하드웨어 구성요

를 인스톨함으로써 다수 시스템의 디지털 신호처리를 동시에 수행한다.

}위시스템 2: BBUS] DSPH7} TDM°}U} TDMA 다수 시스템의 디지털 신호
처리를 동시에 수행한다.

@ 하위시스템 3:880의 DSPH7} 코드 분할 다중이나 코드 분할 다중 접속으로 다수
시스템의 디지털 신호처리를 동시에 수행한다.

@) 하위시스템 4: BBUS] DSPH7} 랜덤 접속 프로토콜로 다수 시스템의 디지털 신
호처리를 동시에 수행한다.

[~

아

@

(1)의 송신기와 수신기를 각각 그림 8.16(2)와 8.17(8)에 보였다. 사용자의 특정 요구
를 외부 제어기로부터 전송하는 다수의 DSPH7} 존재한다. 다수의 DSPHE 하나의
DSPHE 집적될 수 있고 하나의 외부 제어기에 이해 제어된다 [13]. 각 디지털 신호처
리 흐름이 분리되어 있으므로, MMSR 시스템은 서비스간 간섭을 야기하지 않는다. 그
러나 다수의 DSPH7} 준비되어야 하고 과잉 신호처리가 존재한다. 결과적으로, 하드웨
어의 크기가 집적된 시스템의 수와 함께 증가한다.

(2)의 송신기와 수신기를 각각 그럼 8.16(6)와 8.17(6)에 보였다. 하나의 DSPH7} 시

465



===== PAGE 465 =====
최신 이동통신시스템

466

Mobile Communications using MATLAB Simulation

간 분할기반다중접속에 의해 통신 시스템들을 위한 신호처리를 수행하는데 이는 하위
]스템 (1)의 문제였던 과잉 신호처리를 제거하기 위함이다. 두 가지 방식의 시간 분할-

|

기반 다중접속 방법이 존재한다: 특정 통신 서비스를 위한 신호처리를 위해 고정된 시
간 슬롯을 할당하는 TOMI} 통신 서비스를 위한 신호처리를 위해 요구에 따라시간 슬
EE 할당하는 TDMA.

스토 a Msc: 토    a ere
sSEGSE 수은 등     =s  그은
주구 을 노가 울기 동구      sass 858
BS$22i 28%    BSSk #88
Ｌ 4

sis] [도

17

Controller’
Controller
(d)

system #N

data for

ode #2! system #2
ㆍ
ㅜ Digital

Code #N

Controller

(c)

Controller!

를 22 8.16 MMSR 시스템의 송신기의 구성 (1/0: time offset, corr: correlator):

(a) 분리형, (6) TOM- 혹은 TDMA-7|#t, (0) CDM- 혹은 CDMA-7|4t, (0)
랜덤 접속형.


===== PAGE 466 =====
Bde) eee
=SE=s   ss
Besase sé
sse2s% 23%
1 주   「       =  g  _&
1    =SE=sSE SE
|        |    Beeeee Sse
|    a.    ㅣ    aszas  av
| |   a>   |     4  4   ㅣ
=|    유즈   1. fell. °   3
주 |    !    {3  |!  <a     ies
E         |   eV   {a    2
의|        |  의 |    a=
|            그
|
        | ieee 2
,   「  a     a  na    2
Eng  g   =    ha SaaS.   ae
sSEGSE 55   esSeges  수은 등
BESG58 Ese    28958... Bad
SSgeee 28:   SEeBSE 288
0               >
= 18            | 고우   |
2   Vv           x  [~]
[=)    a           S  Se
a
중    개
| 로 |      는  ie oan! S
S}| ME 오치  ras
| & |          ‘   3

를 그림 8.17 다중모드 다중서비스 소프트웨어 무선시스템을 위한 MMSR 시스템의

A
o  고
신기의 구성 (1/0: time offset, corr: correlator): (a) 분리형, (6) 다중샘
플기를 갖는 TOM 혹은 7011&기반 SS ASO, (0) 분리된 4/미머 갖는
CDM- 혹은 CDMA-7|#!, (0) 랜덤 접속형.

슬롯 타이밍이 고정되어 있으면 TDMe] 효과적인 MMSR 시스템을 구현할 수 있다.
그러나 집적된 시스템의 수가 증가함에 따라 디지털 신호처리를 위한 시간 슬롯의 수가
증가한다. 또한, 통신 서비스에 우선순위 (3)으로 하나의 시간 슬롯을 할당하면, 시간
SRO 대부분 사용되지 않는다. TOMAS 이 문제를 갖고 있지 않지만 시간 도메인 인
터럼션과 같은 관리 기술이 필요하다.

(3)의 송신기와 수신기를 각각 그림 8.16(0)와 8.17(0)에 보였다. (3)의 28"브의 불필

467



===== PAGE 467 =====
최신 이동통신시스템

A

468

Mobite Communications using MATLAB Simulation

요한 ASA EUS 제거하기 위해 그리고 (2)의 TOMe]} TOMAS] 동기적인 신호처리
를 피하기 위해 각 시스템의 디지털 데이터에 코드가 중첩되는데 이 코드는880의 TX
모듈에서 D/A 변환 전에 22] a1 RX 모듈의 8280에서 A/D 변환 후에 얻어진다. 중첩된
디지털 aoe CDMS 사용해 다중화된다. 특정 서비스를 요청하기 위해, 사용자는
확산 코드를 사용하여 이 서비스의 정보 데이터를 획득한다. 이 경우에 사용된 코드는
암호이거나 확산 코드일 수 있다. 이 시스템의 이점은 코드가 서비스를 결정하는데 있
다. 그러나 코드의 중첩은 클럭 속도가 증가함을 의미한다. 그래서 시스템은 고속 디지
털 신호처리기를 요구한다.

(4)2] 송신기와 수신기를 각각 그림 8.16(0)와 8.17(0)에 보였다. 이 구성은 기본적으
로 TDMAS} TDM 대신 랜덤 접속 프로토콜을 사용한 (2) 응용이다. HS, MMSR AIA
템 (14)를 제외하고도, 시스템 (2)를 송신기 구조로 채택하고 시스템 (3)를 수신기 구조
로 채용한 혼합 시스템을 사용할 수 있다.

54549표은 “다중 시스템”의 집적에 효과적이다. 그러나 소프트웨어 무선 기술에 있
어서는, BBUS] 구성에 대한 새로운 개념을 사용해 보다 효과적으로 만들 수 있다.

8.5.5 인자제어 소프트웨어 무선 기술
일반적인 완전-다운로드 AY AVEO 우선 기술에서; 사용자는 시스템 구성을 변
화시킬 수 있다. 그러나 다음 문제가 발생한다 (8.3장 참고):

D 요구되는 이동통신 구성요소 블록의 내용이 복잡해짐에 oe} DSPHE 다운로드
되는 소프트웨어의 부피가 증가한다.

(60) 요구되는 이동통신 구성요소 블록의 내용이 복잡해짐에 ue} DSPHY] 구성 검사
의 시간도 증가한다.

@ 다운로드 소프트웨어에서, 다수의 구성요소 SHO] 제조사의 노하우와 관련된
다(예, 특정 블록을 위한 최적화 방법 혹은 계산 알고리즘). 이 AAS 소프트웨
어가 다운로드 될 때 유출될 수 있다. 또한, 다른 사람에 의해 변화될 가능성도
존재한다.



===== PAGE 468 =====
소프트웨어 무선 통신시스팀 (를

[11, 12]의 소프트웨어 무선 기술은 단지 TX9} RK 모듈의 280와 관계가 있다. RFU
와 00)는 개별적으로 혹은 집적된 8100 와 IFUS 준비된다. BBUS 그림 8.18에 보였
다. 이미 28빼에서 구현된 송신기의 부호화기, 프레임, 변조기,  이뽀     독과수신겨희
등화기, 검출기, 복호기 블록과 같은 기본적인 이동통신 구성요소 SSS 포함한다. 이

동통신 블록의 기능은 프로그램 할 수 있고 외부  aHeeeRoen 쉽게 변화시
킬 수 있다. 예를 들면 송신기의 디지털 필터의 구성을 변화시키기 위해서는, 사용자는
BBUS] 필터 SS] 단지 필요한 디지털 BE] 계수만을 보낸다. 외부 인자의 사용은
BBUS 다목적 송수신기가 되게 하고 이로 인한 소프트웨어 무선 시스템을 인자제어
소프트웨어 무선 시스템이라 부른다. 그림 8.18는 880의 구성과 인자제어 소프트웨
어 무선설비를 위해 필요한 인자를 보여준다.

To                                      From
TX module                             RX module
of IFunit | Parameters of |F unit

Och    set ree               Ich Qch

4Parameter
controller } |

ee
Se OME NS ARON dente ia inti ne niagara

Ss

총

From data generator                  Output data
를 그림 8.18 인자제어 소프트웨어 무선 기술에서의 864 FA

제안된 시스템은 외부 인자들을 다운로드 해서 구현되는데 인지
시스템의 구현을 위한 작고 중요한 정보들이다. 그래서 중요한 블록은 미리 2600에서
구성되어야 한다. GALLEY 소프트웨어 무선 기술에 비해 안정된 성능을

수 있고 구성 시간도 BAA 수 있다. 또한, 특화된 이동통신 구성소자를 위한
방법과 같은 제조사 노하우를 유출시키지 않는데 이는 적은 부피의 소프트웨어만을

469


===== PAGE 469 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

운로드하기 때문이다. 게다가 DSPHS 다운로드 되는 소프트웨어의 부피가 작으므로
몇 가지 강력한 부호화 방법이 소프트웨어를 다운로드하기 위해 사용될 수 있다. 결과
적으로, 소프트웨어 무선 통신 시스템이 복사나 변경으로부터 안전하다.

인자제어 형의 실험적인 시제품이 개발되어 전송 성능이 평가되었다 [12, 231. 그림
8.19와 8.20은 실험적인 시제품의 시스템 구성과 외형을 보여준다.

a

aa
3  = |[=2
e   Zz        >
   bo        a
Hu) lox =    EZ
ES] jo §       35

nit
TDMA

6 |   CPU  |
u
ADPC

8
[605

680

+            기
D>
De    2     oo   4     o>
=   조   o    a=
& §    a =    222) | 6뜨   ti &
¥     주    수     7
+
「     ^ 쓸        x
=   | | Ee) |
군     zi      5 | 문군    Ge
cc    ac     2 0 뜨    뜨

1.5-1.9
GHz
5.8 GHz

를 그림 819 실험적인 시제품의 시스템 구성.

470


===== PAGE 470 =====
를 그림 8.20 실험적인 시제품의 외형.

시스템 인자는 표 8.3에 정리되어 있다.

』표 8.38 실험적인 NMSA 시스템 인자

서비스                변조              주파수                 데이터 레이트

(서비스 모드)             PHS-1/4DQPSK_ | PHS-1.9GHz__| PHS-384 Kbps (반송파 비트 레이트)

PHS, ETC, GPS          ETC-ASK                   ETC-5.8GHz | ETC-1,024 Kbaud (데이터 레이트)

(사웅자 BE            GPS-BPSK+SS          GPS-1.5GHz | GPS-50 bps (데이터 레이트) : 1.023

BPSK, QPSK,        싸용자 모드-          사용자 모드 ㅣ | Mops (칩 레이트)

2/4 QPSK, GMSK | BPSK, QPSK,             IF 대역               사용가 모드

a/ 4 QPSK, GMSK                            BPSK, QPSK, 2 / 4 QPSK-384 Kbps

(반송파 비트 레이트)
GMSK-270.833 Kbps (반송파 비트
레이트)

실험적인 시제품은 118를 위한 서비스 모델로 세 가지 실제 이동통신 시스템 PHS,
GPS, ETC 시스템을 사용할 수 있다. MMSRE 동시 서비스를 허용한다 (즉, PHS 와
ETC &2 GPSS}ETC). 이는118를 위한 세계 최초의 4449표이다[12, 23]. 또한, 사용
자 모드에서, 사용자는 변조방식을 35449, 7/4QPSK, BPSK, QPSK 중에서 자유롭게
선택할 수 있다. PHSS} GPS 시스템은 088에서 사용되는 주파수(1.5-02대역)와
PHS 주파수(1.9-0대역)가 비슷해 하나의 집적 안테나를 사용한다. 외부 인자는 관

471


===== PAGE 471 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

리 SEEMS 탑재한 LESS 컴퓨터로부터 공급되는데 이 컴퓨터는 실험적인 시
제품과 10BaseT 이더넷 케이블로 연결된다.

그림 8.19의 PHS 시스템을 구현하기 위해, 외부 인자는 SESS 컴퓨터로부터
1088867 이더넷 케이블을 통해 전달되고 CPU 장치에 저장된다. CPU 장치는 인자를
BBU, IFU, RFUo] 전달한다. 비슷한 기술인 688, ETC 시스템에 사용될 수 있다.

다음은 완전-다운로드형 소프트웨어 무선설비와 인자제어 소프트웨어 무선설비의
다운로드 프로그램 부피와 다운로드 시간을 비교한다. 제어된 인자는 변환, FPGA 장
4], DSP°}A} AlteraA}2] FPGAS 사용한다. 첫 번째 결과로, 변환, FPGA, DSP 장치에
서 사용될 수 있는 소프트웨어의 부피가 있다.820ㅅ-기반 장치를 대해, 소프트웨어 부
피가 요구되는 게이트의 수로 표 8.4에 주어졌다.

828.48 실험적인 시제품에서 『『ㅁ6ㅅ^-기반 장치의 소프트웨어 부피

Unit      Conv, Unit                    FPGA Unit (gate)                   FPGA
(gate)                                                             Total
Gate
Device    EPM    EPM   EPM    Ere    EPM    EPM    EPM    EPM     EPM
(Number) | 7064 | 9400 | 7064 | 10K20{ 7128    7128    9400 | 7192    10K250
(1)      (1)     (1)     (1)      (1)      (2)      (2)     (1)     (1)(2)(3)
Max. Gate         1,250       8,000 | 1,250 | 20,000 | 2,500       2,500        8,000 | 3,750 | 250,000x3
사용자 모드 | *1,013 | *2,176                 723    *826   #25920 | F716              8,036
PHS                   *1,013 | *2,176          113 | "2009 #725          13 1] 23520 | £388                                 14,548
GPS                                                                                                                                                                           560                86            547,500 | 548,146
Ete                1,088                                                          1,088
총                         1.013        3,264          113        7,200         725             826          3,080          862         $47,500 | 564,583
목적      TX    RX    PHS/ | (7313) |DSP I/F|DSPI/F |DSPI/F |D S P| GPS
Filter   Filter |IF           TX     TX (413 | RX    I/F RX | Correlator
(1013           (2176,                                                    (725              shared) | (2,520 | (388
shared) | shared)                    shared) | EXT I/F | shared) | shared)
ETC                                            (413)      GPS I/F | EXT
Demod                               (560)    VF
+ETC                                        (388)
VF                                          GPS
(1088)                                       I/F (86)

*몇 가지 시스템의 구현에 공유되는 소프트웨어를 의미한다.

472


===== PAGE 472 =====
DSP-7] 8} 장치에 대해, 소프트웨어 부피가 프로그램 코드의 부피 (byte)= 표 8.5에
주어진다. 표 8.6은 인자제어 소프트웨어 무선 시스템을 위한 사용자 BES] 평균 구성

시간을 보여준다.

#표 8.58 실험적인 시제품에서 각 시스템의 소프트웨어 부피
Device          Conv,&FPGA                        DSP Unit (byte)                         Parameter
Unit (gate)                                                                              (byte)

TX                  RX                 Total

사용자 모드                   8036             13357*             40509*              53866               1660

PHS                           14548              9586*             13340*              22926               1616

GPS                              548146          Not used                  13340*                 13340                        4

ETC                               1088         Not used           Not used                        0                  570

Total                         564583               13857              40509              53866

*몇 가지 시스템의 구현에 공유되는 소프트웨어를 의미한다.

HH 8.68 인자제어 소프트웨어 무선 시스템을 위한 사용자 모드의 평균 구성 시간
BPSK>QPSK                37.5ms | BPSK>GMSK_ | 30.5 ms        QPSK 2/4>QPSK_ | 30 ms
QPSK->BPSK              32.5ms | GMSK>BPSK | 35.35ms {2/4 QPSK>QPSK | 35 ms
BPSK->z / 4 QPSK        32.5ms | QPSK>GMSK | 30 ms          a /4 QPSK>GMSK | 30 ms
z / 4 QPSK->BPSK        35 ms        GMSK>QPSK__ | 40.5 ms       GMSK->2 / 4 QPSK | 35 ms
Full download user mode                      3,410 ms

H 8.4 각 함수 블록과 하드웨어 소자들의 FPGA 게이트 수를 보여준다. (*) 표시된
데이터는 다수의 시스템에 공유된다. 예를 들어, TX 필터 BSS 사용자 BES} PHS
모드에서 SE] 51, FPGAS] 크기는 1.013 게이트이며 EPM7064(1)o] 프로그램 된다.

완전-다운로드 형

소프트웨어 무선설비는 사용자 HE, PHS, GPS, ETC 시스템에 각각

8,036, 14,548, 548,146, 1,088 게이트를 필요로 하고 시제품은 8004 기반 장치에 미
리 프로그램될 564.583 게이트를 펼요로 한다. DSP 장저들 위한 소프드웨어의 무피는

473



===== PAGE 473 =====
최신 이동통신시스템

474

Mobile Communications using MATLAB Simufation

사용자 SLE, PHS, GPS, ETC 시스템에서 표 8.5에 제시된 부피의 도움으로 조사될 수
있다. 시제품에 대해 인자의 부피가 제시됐다. DSP 장치를 위한 소프트웨어만이 다운
로드 된다고 가정하면, 각 시스템의 개별적인 구현을 위해 DSP 장치로 다운로드 되는
모든 DSP 소프트웨어의 경우와 비교해서 시제품은 PHSS] 경우 1/15, 사용자 모드의
경우 1/30 정도의 다운로드만을 필요로 한다. 또한 표 8.5는 288 시스템을 완전-다운로
드형 소프트웨어 무선 시스템으로 구현하기 위해서는 222026 bytes] DSP AXES]
요한 반면 시제품은 모든 시스템을 구현하기 위해 53,866 bytesS 사용함을 밝

은 몇몇 시스템을 위해 과잉 프로그램을 사용하지만 이는 소프트웨어 다
시간을 단축하고 시스템을 재구성할 때 안정적인 성능을 제공한다.

두 가지 소프트웨어 시스템이 HAS 위해 요구되는 260의 크기에 비해, 시제품은
564,583 게이트가 필요하고 완전-다운로드형은 각 시스템에 대해 최대 게이트 수를 필
요로 한다 (688의 경우 이는 548,146 게이트에 해당한다). 다른 말로 하면, 시제품의
FPGAdml 부피는 완전-다운로드형의 1.02 배이다. 반면, DSP 장치에 대해서는, 사용
자 모드를 위한 프로그램이 시제품에서 필요한데 이는 다른 시스템이 이들 프로그램의
몇몇 부분을 사용하기 Wl. AWA 두 소프트웨어 무전 시스템은 사용자 모드 프
로그램을 포함할 수 있는 DSP 구성소자를 필요로 한다.

표 8.6은 사용자 모드의 다운로드 시간을 비교한다. GMSK, 2 / 4QPSK, BPSK,
QPSKS 사용할 수 있다고 가정한다. 시제품의 평균 다운로드 시간은 완전-다운로드-
형의 약 1/100에 해당한다. 또한, 사용자 모드의 구현을 위한 평균 다운로드 시간은 변
조방식과 무관하고 인자제어 소프트웨어 무선 시스템과 거의 동일하다. 이는 사용자
모드의 모든 변조방식이 비슷한 다운로드 소프트웨어를 사용하기 때문이다.

사용자 모드의 경우 실험적인 시제품의 BER 성능을 그림 8.21에 보였다. 모든 시스
템의 이론적인 BER 값 대 ※#,/24,을 포함한다. 이 경우, 모든 시스템에 대해 코히어런
트 검출이 필요하므로 889, QPSK, 7/4QPSKE SUS BER 대 ,/2,을 갖는다.
실험적인 시제품의 BER 성능이 모든 변조방식에 대해 이론적인 BER 성능의 108임이
명확하다.



===== PAGE 474 =====
1                                                   wee

|
—a— QPSK
—8- 1/40PSK
—e- BPSK

0.001                  a ISIN

0 i 2 of a 0000
E/N, (dB)

를 그림 8.21 사용자 SE 경우 실험적인 시제품의 BER 성능

8.5.6 다수의 시스템을 위한 동시 신호처리 방법

하나의 샘플러를 사용하여 모든 목표 시스템에 균등하게 시스템 클럭을 제공하는 공
통 샘플링 처리 방법은 MMSR 시스템의 크기를 줄이는 효과적인 방법이다.

그러나 시스템 클럭 속도는 모든 목표 시스템의 최대 심볼/칩 레이트를 다룰 수 있을
정도로 충분히 커야하므로, 목표 시스템의 심볼 레이트의 차이가 클 때 작은 심볼 레이
트를 갖는 시스템에 대해 과잉 샘플링 처리를 하게 된다.

이 문제를 피하기 위해, 공통 샘플링 과정이 제안되었다[241. 여기서, 시스템 클럭은
목표 시스템의 클럭 속도로 결정되고 모든 목표 시스템에 제공된다. 이 방식은 목표 시
스템의 클럭 속도가 서로 많이 다를 때 시스템 클럭을 감소시킬 수 있어야 한다. 그림
8.22(a)= 두 시스템(&와 B)S] 클럭( 9,와 S,)°] 서로 많이 다를 때( 9 ,>> S,) 제안된

샘플링 과정을 보여준다. Al 할당된 샘플링 클릭은 일정 간격동안 보류되고, 이 시간

동안, 그림 8.22(6)에서처럼 BS] 샘플링이 행해진다. 시스템 A= 샘플링 데이터로 0을
보간020060001809)하게 된다. 이 과정은 목표 시스템의 클럭 SES] 차이가 크더라도 효
과적은 공통 샘플링 처러를 가능케 한다. 이제 이 YAS 다수의 시스템에 적당한 방법
으로,번경서켜.보자.

3     a

th\o

475


===== PAGE 475 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

를 그림 8.22 (a) 제안된 샘플링 방법의 예 (6) 시스템 AS Bol 사용된 샘플링 클럭.

그림 8.23-2 MMSR 시스템에서의 공통

대한 사용자의 요구는 목표 시스템의 SSS 생성하는 블록에 보내진다. 목표 서비스의
수 2 목표서비스의 심볼/칩 레이트 /[=(5,, 52, '…, 5, ㆍ

각 목표 시스템의 샘플링 과정의 최소 보류 간격 Ton 이 개시 그 개
7009 TV mine) 모든 목표 시스템에서 최대 심볼 레이트를 갖는 시스템의 필요
한 오버샘플 수 P[samples/symbol]°] 목표 시스템의 목록에 포함된다. 이 목록은 ^
스템 클럭 할당 장치에 입력된다.

09108                     a       Digital
processing
arts
p                       | Control clock ee)  part
5      Lists of
Carrier   target
=e    systems
를 그림 8.23 (b) 공통 샘플링 처리 방번의 흐름

구성은 그림 8.24에 보였고 모든 목표 시스템의 시스템 클럭 할당 목록

럭 할당 알고리즘에 의해 생성된다. 또한, 시스템 클럭은 직접적으로 시

476



===== PAGE 476 =====
당된 시스템의 총 수를 나타내는 2, 에 의해 결정된다. 마지막으로, 모든 목표 시스
의 각 샘플링 클럭은 샘플링 클럭 발생기에 의해 생성되고 수신 데이터의 각 부분은 멀
티샘플러에 의해 디지털로 오버 샘플링되고 디지털 처리 부분으로 보내진다.

Target system's clock list

Number of target service
Threshold of clock ratio
|              |  Number of oversamples

c
Control clock generator            System clock

를 그림 6.24 시스템 클럭 할당 장치

다음으로, LEAs] 위한 시스템 클럭 할당 알고리즘에 대해 기술한다. 여기서,
마스터-시스템은 샘플링 처리의 최소 보류간격 동안 보다 낮은 심볼/칩 레이트를 갖는
시스템의 샘플링 처리 AS AMS 수 있는 시스템을 나타내고 슬레이브-시스템은 마
스터-시스템의 처리 시간을 홈치는 시스템을 나타낸다.

이 알고리즘에서, /의 S{i=N, 4/ㅡ-1,…, Bol 대해 보다 높은 심볼/칩 레이트
S{J=i-1,--, lhe 다음 할당 방법 순으로 찾아진다,

0마스터^시스템의 처리 시간은 슬레이브-시스템의 처리 시간을 71H] (Cover) ert.
마스터-시스템 7,2] 이후 처리과정에 SHS 미치지 않고 방법 ([)을 이용하기
위해, 슬레이브-시스템 7/,에 대해 충분한 샘플링 클럭이 마스터시스템 2) 최
소 보류 간격 Tring WA 주어져야 한다. 여기서 = /의 번째 심볼/칩 al
JE 6,에 따른 시스템 이름이다. 이는 마스터시스템 19] 심볼/칩 레이트
(S,) 3 슬레이브시스템 17,2] 심볼/칩 레이트 (6,)의 비가 Tring 24 커야

477



===== PAGE 477 =====
^ 최신 이동통신시스템
C

Mobile Communications using MATLAB Simulation

함을 의미한다. 그래서 이 방법 Del 사용될 수 있는지에 대한 추정은 다음과

같다:
~
| % > Tin)                                (8.6)

시스템 클럭 할당 목록 』.은 다음과 같이 생성된다:

여기서 의 각 랭크와 27,( 77,)는 마스터-시스템과 슬레이브-시스템 간의 클래
스를 나타내고 시스템 WE 시스템 1,9) 슬레이브이다. 특별히, Lo] 첫 번째
랭크의 시스템은 시스템 클럭에 직접 할당된 시스템을 보여준다. 그래서 시스템
클럭 C[samples/second]= 최소한 다음을 필요로 한다:

C[ samples / second] = S ,|symbols / second ]× P[ samples / symbol]

심볼 레이트가 서로 많이 다른 (S, >> 6, >> 9) 세 개의 시스템에 대해 시스템
(D)& 사용하는 예를 그림 8.25에 보였다.

478


===== PAGE 478 =====
3
System A   a
1

oO
[=
2
^
>

wn

2
=
s
a
=
”
의

를 그림 8.25  (0))의 al (S,))S,)) 5.)

)마스타시스템의 처리 시간이 다수의 슬레이브-시스템의 처리 시간을 커버한다.
마스터-시스템 /』의 이후 처리과정에 영향을 미치지 않고 방법 (2)을 이용하기

위해, 모든 슬레이브-시스템 ( (토2개 i, IT,) 대해 충분한 샘플링 클럭이 마

479



===== PAGE 479 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simufation

스터시스템 19 최소 보류 간격 Tring 내에 주어져야 한다. 이 경우, 제안된
방식은 마스터-시스템이 모든 슬레이브시스템에 대해 슬레이브 시스템의 최대
심볼/칩 레이트에 의해 결정된 처리 시간을 이용한다. 그래서 (2) 방식이 사용될
수 있는지에 대한 추정은 다음과 같다:

내

여기서 27(=1-7+ 1)은 슬레이브시스템의 +S 나타낸다. 그 다음, 시스템 클
럭 할당 목록 』Ｌ은 다음과 같이 생성된다:

위 식에서 두 번째 랭크의 정보는 하나의 마스터-시스템에 다수의 슬레이브시스
템이 존재함을 의미한다. 이 경우, 시스템 클럭 C[samples/second]= (1))의 경
우와 동일한 계산에 의해 심볼 레이트 6,에 기반해서 결정된다. 세 개의 시스템
에 대해 방식 (@)S 이용하는 예를 그림 8.26에 보였다.

480



===== PAGE 480 =====
a>
ra
e =
3   |
co
ro)
3
eaten~ 2
>> 딱
N
oa ee>>
> oO
—
fo)
ca co
> Kt
2   o
=   E
S   은
=   모
wm   wn

를 그림 2.26 (@)2| al (S,)) S,, 5.)

@)다수의 마스터^시스템의 처리 시간이 슬레이브시스템의 처리 시간을 커버한다.
모든 AEA AR (7, …, Hyp“ ID) 이후의 처리과정에 영향을 주지 않

ㅇ

481


===== PAGE 481 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

고 (@) 방식을 이용하기 위해, 제안된 방식은 각 마스터-시스템 (4, Dye
…, 1°] 슬레이브시스템 24에 필요한 처리 시간을 일정하게 커버하는 방식
을 이용한다. 그래서 모든 마스트시스템 (7, …, Lys HMA 최소 AB
칩 레이트의 시스템 1S 처리 시간을 커버해야 하는데 최소 보류 간격 Tongs
동안 다른 마스터시스템과 균등하게 커버해야 한다. 그래서 이 방식 @)o] 이용
될 수 있는지에 대한 추정식은 다음과 같다:

(s, x t)
|       %| 2 200)                              (8.8)

여기서 (= 7-1+1)은 마스터-시스템의 총 수를 나타낸다. 그 다음, 시스템 클
럭 할당 목록 Lou gs 같이 생성된다:

위 식에서 두 번째 랭크의 정보는 다수의 BPE A] AMO] 하나의 슬레이브-
템에 대해 존재함을 의미한다. 이 경우, 시스템 클럭 C[samples/second]+=
마스터-시스템에서 최대 심볼/칩 레이트 S. 의해 결정되고 모든 마스터-시
Ao] 일정하게 분포된다. 그래서 시스템 클럭 C[samples/second]= 최소한
음과 같아야 한다:

시

년

ALT ole

C[ samples / second] = S,[symbols/ sec ond]x t(= 77 , ) x P[samples / symbol]

세 개의 시스템에 대해 방법 (@)-S 사용하는 예를 그림 8.279] 보였다.

482



===== PAGE 482 =====
를 그림 8.27 (@)9 al (9,, S,)) 5.)

GPS, ETC, PHS, VICS, PDC. 미래 18 서비스를 위한 집적 수신기의 개발의 입장
에서, 제안된 방식의 효율성이 AWGN} 레일이 페이덩 환경에서의 BER 성능으로 컴
퓨터 시뮬레이션을 통해 평가되었다 [24]. 제안된 방식은 AWGN} 레일리 페이딩 환
BAA 충분히 강인함을 보였다.

8.5.7 소프트웨어 무선 소자
이 장에서는 소프트웨어 무선설비를 PASE 세 가지 주요 소자 ADC, DSP, FPGA
에 대해 기술한다.

(1) 아날로그1ㅇ디지털 변환기(600)
ADCE 아날로그 신호와 디지털 신호간의 통로이다. 사용자들은 보다 높은 속도, =
은 해상도, 낮은 가격을 갖는 ADCS 선호한다. 표 8.7은 100 MHz7} 넘는 샘플링 레이
를 RE ADCS 보여준다. 샘플링 레이트는 꾸준히 증가하고 있다. 그림 8.28은 이러
한 경향을 보여 준다 [25]. 2000년 이후로, 4100들은 고속, 고해상도 4100로 기대된다.

483


===== PAGE 483 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

$28.78 주목할만한 ADCO 목록
이름                제조원           해상도 (비트) | 샘플링 레이트
AD9433                        Analog Devices                        12                             105
AD9214                        Analog Devices                        10                             208
AD9410                           Analog Devices                           10                                105
AD9432                        Analog Devices                        12                             200
AD9054A                       Analog Devices                         8                              100
AD9288                        Analog Devices                         8                              100
AD9071                         Analog Devices                        10                             100
TDC1029                     TRW                      6                     100
SPT7760A                       Sig Proc Tech                         8                            1,000
HADC77100                      Sig Proc Tech                          8                              150
CXA1176K                                         Sony                                             8                                         250
CXA1276K                    Sony                       8                     400
1,000,000
100,000        N
,                     ~
을 1000              DOS.
!     SNS
=                                N a  ~~
S                                               N
10                                 Ds   INE
NYA. 기 2003
더 1993
1988
0.1
2     4      6      8     10     12     14     16     18     20
Bit resolution [bit]
를 그림 8.28 ADCI 향후 성능

484



===== PAGE 484 =====
(2) 디지털 신호 처리기(290)

109는 곱셈을 가속화하고 계산을 축적할 수 있는 (MACs) <#ㅁ이다. 주요 이점
소프트웨어 프로그램밍과 BAA. DSPS 구성하기 Ha, C4 어셈블리와 같은 고
컴퓨터 언어가 사용될 수 있다. 필요한 소프트웨어가 저장되어야 하는 메모리 어드레
에서 프로그램을 읽음으로써 소프트웨어를 재구성할 수 있다.

그러나 29『는 처리 속도에 대한 문제를 가지고 있다. 29 프로그램은 일반적
병렬적으로 처리되지 못하고 순차적으로 처리되므로, 처리 시간은 DSPS| 구조에 의
한다.

그림 8.29% DSP 기술에서 기대되는 경향을 보여준다. DSP 처리 속도가 14
Gflops 이상이라면 실시간 이동통신에 사용될 수 있다. 2000년 이후로, DSP 회로에 기
반한 실시간 이동통신 단말기가 가능할 수 있다.

은
~

yh

fs

rh

Floating point                                                                    Fixed point
수                                                                                 A
10 Gflops |                                                                                     {100 6005
TMS320C67x
1 Gflops -—                                                  °                     —{10 GOPS
ㅇ                                 시
에 메야하=                                        ADSP21060_-<                          16008
ㅁ050326 9                                  06『16210
10 Mflops   °                               x  01620                     — 100 MOPS
DSF36001                 ADSP21csp01
1 Mflops _7\6820620                            :               10 MOPS

1990                               1995                              2000

O Floating point DSP
x Fixed point DSP

를 그림 8.29 DSP 향후 성능

(3) Field-Programmable Gate Array(FPGA) [26]
FPGAS 제조 후에 정의될 수 있는 프로그램 할 수 있는
이트의 배열이다. FPGAS 블록의 WSS 구성되고 각 블록은

485



===== PAGE 485 =====
최신 이동통신시스템

486

Mobiie Communications using MATLAB Simutation

있다. ABA FPGA 구조를 그림 8.30에 보였다. FPGA 논리 BEL 일반적으로 7
입력에 대한 lookup tables (LUTs)-& 가지고 있다. 논리 블록의 입력은 LUT 입력이나
flip-flop 입력 포트에 연결되어 있다. LUT 출력은 논리 블록의 출력 YE flipfipo 입
력 포트에 연결된다. 다중화기(2741072168618)를 더함으로써, 입력 신호의 다양한 조합
이 선택될 수 있다.

Logic block

Wire resource

Wire that is actually used

를 그림 8.30 전형적인 FPGA 구조 [26].

LUT static RAM (68.410)을 사용해 구현된다. SRAMdml 모든 어드레스에 데이
터 내용을 설정함으로써 LUTE 4) 4 Boolean 함수라도 구현할 수 있다. LS, flip
4008이 유한 상태 머신의 상태 정보와 같은 데이터를 저장하는데 사용된다. 그림 8.31
은 FPGA 논리 블록의 구조를 보여 Ect [26].

VHDL3} Verilog HDL-& FPGAS 설계하기 위한 프로그래밍 언어들이다. 소프트웨
어는 SRAME] 데이터를 변화시킴으로써 재구성될 수 있다. 29『와 반해, FPGA 고
속 신호처리를 위해 병렬로 설정될 수 있다. 그러나 812Ｌ이나 60108712Ｌ의 프로그
래밍은 목표 소자의 하드웨어 구조에 대한 지식을 필요로 한다.



===== PAGE 486 =====
+
Pp   Hs
0008             버 Flip-flop |
table            a
ld
Mux
e—,
Lookup                    .
+p table              Mux Flip-flop -—
@---
ae
| ~   to
Lookup            Mux-—j Flip-flop -—
table            I
a
Mux Be
re,
Ure ROOkup
table             Mux Flip-flop -—
Ss   |

를 그림 8.31 FPGA 논리 블록 구조의 a [26].

그러한 하드웨어 기술 함수와 (와 같은 고레벨 컴퓨터 언어 간의 변환기에 대한 연
구가 진행 중이다 또한, FPGAS 의제 백말 212 ie  ES 424 한다 [27]. 띠래에는, BE
이동통신 시스템이 단지 FPGAS 사용해 프로그램 될 것이다.

소프트웨어 무선 통신 시스템 프로젝트

이 장에서는 미국, 유럽, 일본에셔 행해지고 있는 SZEMo] 무선 동신 시스템과 관
=

487


===== PAGE 487 =====
최신 이동통신시스템

ray

Mobile Communications using MATLAB Simulation

8.6.1 0] 4

미국에서 소프트웨어 무선설비에 대한 연구와 개발은 군용 통신시스템에서 시작되
었다. 가장 잘 알려진 시스템은 1994년의 “SPEAKeasy” 프로젝트인데 [2], 많은 통신
시스템을 군사용 목적으로 하나의 단말기에 집적한 것이다. 주요 목적은 구별되는 변조
방식을 갖는 단말기 간의 통신에 있었다. 이 개념은 “voice bridge” et 불린다. 시스템 개

념을 그림 8.32에 보였다.

모든 구성요소들은 기능모듈로 배열되고 이들 기능모듈을 관리하기 위해 common
system equipment (CSE)7} 사용된다.

시제품이 개발되었고 표 8.8은 9884ㅅ685*에서 기선 파형 호환성을 보여준다.
SPEAKeasy 프로젝트의 성공 후에, 소프트웨어 무선설비에 대한 연구와 개발이 가
속화 되었다. SDR 포럼과 GloMo 프로젝트를 포함한 많은 프로젝트가 현재 진행 중
이다.

#표 8.88 기선 파형 호환성

파형                      RF 대역                           AlBAIA
STAJ                                                 HF            주파수 도약 데이터와 음성 통소
HF 54] (MIL-STD-188-110A)             HF           멀티레이트 데이터 통신
Automatic Link Establishment (MIL- | HF        자동 셋업과 HF 링크의 모니터링 (채널 스캐닝, 자동
STD-188-141A, App.A)                               응답, Ja 54 분석을 포함)
PACER BOUNCE                                   HF             DAA 아날로그 HF 통소
SINCGARS                                   VHF        주파수 도약 음성과 데이터 통신
HAVEQUICK I/II                         UHF       주파수 도약 음성과 데이터 BA

488



===== PAGE 488 =====
)181180/4400 Jamod 06 |0ㅁ01816 *

1000010400/1911040020 10000 SQ «

je

363 ‘uawdinbe weyshs uowwoD

J9qul        A        ㆍ

82084181비 이

104400 pue 40464101003 이

911816 pue 90401\씨
6416980010

104402 pue Aejdsig 이

1배

1

1044402 Jamog-
Jowuow

Ausedes jauuey)-

ayes eep ajqeue,-
O1pey 16406 *
50161 006 [19 JOWUOW ©
500 01061 80083 «
8010644003ㅇ
UMOPINYS 82841 &

104403

psemuo4 pue yews04-

B1ep/aaio,-
sseudwog(2d)- | | a6puq x2eq/peu-
이버      J3SNVUL-
SIPOUIBIN               uondAsoag-
uondAsou3-
yeuuoy abessay-                     ,
0/| exep 20687         109669010 0300 *
di        4
바시 + Fy bug yoe peu
yomyan-            Anges B]eQ-
aynoy-             peo} weshoug-
eGpug-        queweBeuew Aey-
49NOY «            106960010 Aay e
Bupyiom yausaquj               03903

1484496606418/0004-
Sjauueyo 000히00419
ajdninw 9164584240-
5891009681 0160이10-
149 WOJaAe/M ©
Burt) »
“pow(ea)-
ezyenb3-
4aJajaqul 891033-
peesds(aq)-
JOSS890d WOJBARAA ©
Bujuny-
viaNn-
UoIssaAUOd 0100 ㅇ

wepow

jauueyg-
Joquod 4y- | eduaJaysequl-
980 4u- | Ss0}99)as quy-
AdY/usues| -            ssajdnoy-
40}93}8S21g-           seuuajuy-
16비이비 0          16418 «
du

110
100

Jo

BIB 8.32 SPEAKeasy 시스템 구조와 7

트웨어 무선 포럼(이전 MMITS 포럼) [28]

|어

AXLES

이 199614

멤버들

로젝트의

을 설립하였다. 포럼에서

SPEAKeasy

다: (1) 그림 8.330] 보인

한

해 토의

화 논점에 대

ET

fe)
a

=
ㄴㄴ

489



===== PAGE 489 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

직접모듈 간 혹은 집적모듈과 공통 하부구조 간의 인터페이스에 대한 HES} [2] (2) 소
프트웨어 다운로드 과정과 기술에 대한 ide 포럼은 두 위원회를 갖는다:

기술위원회와 시장위원회. 기술위원회에는 4개의 연구그룹이 존재 한다: (1) 기지국
과 안테나 연구그룹, 2) 다운로트'연구그룹, (3) ASAE API, (4) 모바일 연구그
룹. 전 세계에서 80개 이상의 연구기관과 기업들이 포럼의 멤버로 참여하고 있다.

포럼에서는 기본적인 +4, application programmable interface (API)2] 표기 방법, 소

프트웨어 다운로드에 대한 기술 문서를 발행하고 있다(011: http://www.sdrforum.org).

Module                    Module                    Module

A                            B                            Cc
Stag ate
|                             Module 0                              |
(a)
Module                    Module                    Module
A                            B                             Cc

02 52 FF
L                 Al

Common infrastructure

(b)
@ 22 8.33 SDR BAA 논의된 표준화 논점: (a) PSto SS (6) SStowWA 표준.

(2) GloMo(Global Mobile Information Systems) 프로젝트 [30]

주요 목적은 이동 사용자가 방어 정보 하부구조에서 사용할 수 있는 전체 서비스 영
역에 접속할 수 있도록 하는데 있다. 특별히, 이 프로그램은 무선이동통신의 산발성 연
결 특서에도 불구하고 pry  비디오 서버, 비디오 컨퍼런싱, 화이트 보딩, 이메
일, 음성 통신과 같은 응용환경을 사용할 수 있도록 할 것이다 [311.

이 프로젝트는 127666096 Advanced Research Projects Agency (104 )의 후원으로
미국 내의 많은 대학과 기업으로 구성되어 있다. 표 8.9는 연구 제목과 연구 조직을 열
거한다[301. (URL: http://www.darpa.mil/ito/glomo/index.html.)

490


===== PAGE 490 =====
HZ 8.98 010100의 연구활동

Organization                                         Research Title

BBN Technologies                               Support for distributed real-time multimedia applications
in mobile wireless networks (\MMWN)

BBN Technologies                                             Density and asymmetry adaptive wireless networking

Carnegie Mellon University
Carnegie Mellon University

CTA Incorporated
ITT Aerospace Communications Division

Massachusetts Institute of Technology
(MIT)

Massachusetts Institute of Technology

PLATINUM Technology, Inc.
Raytheon Systems Company
Rutgers University

Rutgers University

Science Applications International
Corporation (SAIC)

SRI International

SRI International
Stanford University
Stanford University

University of Texas at Dallas
University of Calfornia, Berkeley

University of Calfiornia, Los Angeles
(UCLA)

University of California, L\os Angeles

University of California, Los Angeles

(DAWN)

Mobile data access

Pyxis: Middleware for distributed multimedia
programming

Integration of DBS into digital battlefield
High-reliability all-informed voice service
Spectrum wave

Information survivability technology and experiments for
GloMo

Mobile computing support for database applications
Advanced signal processing & networking (ASPEN)

Dataman project-information services for low-powered
wireless mobile clients

NIMBLE: Many-time, many-where communication support
for information systems in highly mobile and wireless
environments

Simulation and evaluation of adaptive mobile large-scale
networks systems (SEAM-LSS)

System engineering, integration (SE&l) and coordination
for GloMo

Advanced secure wireless integrated networks
Low-power distributed mobile networks

Reconfigurable multimode, multiband information transfer
systems

Generic control channel mechanism
Toward a wireless overlay internetworking architecture
Transparent virtual mobile environment (Travler)

Handheld untethered nodes for high performance
wireless network systems

DOMAINS: Design of mobile adaptive networks using
simulation and agent technology ©

491


===== PAGE 491 =====
최신 이동통신시스템

492

Mobile Communications using MATLAB Simufation

표 8.9 (계속)

Organization                                             Research Title

University of California, Santa Cruz          WINGs for the Internet

University of California, Santa Cruz          SPARROW

University of Kansas                                Rapidly deployable radio network (RDRN): phase ||

University of Texas Pan American           Reconfigurable antennas for high-data-rate untethered

nodes

USC Information Sciences Institute         MOSIS: An innovative prototyping service

USC Information Sciences Institute           GloMo university modular packaging system (GUMPS)

Virginia Tech                                   Software radio using reconfigurable computing
8.6.2 #2

유럽에서는, 최초의 소프트웨어 무선설비에 대한 국제 워크숍이 199714 5월 벨기에
의 BSAA, 개최되었다. 워크숍은 Advanced Communications Technologies and
Services (ACTS) 프로그램의 European Commission (EC) DG XIII-Bo} 의해 구성되
었다. ACTSE 다음에 기술된 소프트웨어 무선통신 시스템에 관련된 몇 가지 프로젝트
를 후원한다.

0) Future Radio Wideband Multiple Access Systems (FIRST): FIRSTS] 주된
목적은 GSM 18002} TD-CDMA $} 같은 제2세대와 3세대 이동시스템을 위
능형 다중모드 단말기의 가능성 연구와 시연에 있다. 이 프로젝트는 개념적인 =
문을 포함한다 [34, 35]. GSM 1800과 TD-CDMA 공중 인터페이스의 소프트웨
어 무선 알고리즘을 위한 29『기반 소프트웨어 무선 시연기 또한 개발되었다
[36]. URL 다음과 같다. http://www.era.co.uk/first/First.htm.

(31 Softeare Radio Technologies (SORT): SORT?) 주요 목적은 기능적인 구조와
디지털 신호처리의 정의를 포함해 적응형 무선 접속을 위한 요구조건을 설정하고
안타-앨리어싱 필터와 ADC 그리고 채널화와 샘플레이트 ass
과 WCDMA) 기능 블록으로 구성된 실시간 하드웨어 시연기를 개발하는데 있



===== PAGE 492 =====
다. SORTS] SHE 소프트웨어 공중 인터페이스를 위한 최소한의 표준화 기능을
얻는 것이다. URL http://www.ifn.et.tu-dresden.de/sort/welcome.html°] 다.

(63) Smart Universal Beamforming (SUNBEAM): SUNBEAMS] 주 프로젝트 목적
은 다양한 구조와 소프트웨어 PASS 지원할 수 있을 정도로 충분히 유연한
UMTSS 위한 혁신적인 기지국 배열 처리과정 구조와 알고리즘의 개발에 있다.

= http://www. project-sunbeam.org°]T}. 이에 관련된 EU 프로젝트인 Esprit
프로그램은 소프트웨어 무선통신 시스템과 관련된 프로제트에 중점을 둔다.

® Software Libraries for Advanced Terminal Solutions (SLATS): SLAT2] =
적은 제2세대와 3세대 시스템의 소프트웨어 무선 응용을 위한 (다수의 SASS
위한) 소프트웨어 라이브러리를 개발하는데 있다. 프로젝트는 ㅅ 단계, 라이브러
리 요구조건의 정의와 8 단계, 라이브러리의 개발로 구성된다.

URL & http://www.csem.ch/systemeng/slats°] CH.

© Programmable Multimode Radio for Multimedia Wireless Terminals
(PROMURA): PROMURA 2] 주 3-4] TDMAS} CDMA 3H 9-RF 구조를 지
원할 프로그램할 수 있는 시스템의 시제품의 개발과 BICMOS Bipolar SiGe 기
ZS 사용한 \/8ㅜ8010를 위한 H/W 블록의 개발에 있다.

© Mobile Multimedia Access Using Intelligent Agents (M3A): M3A 프로젝트
는 세 개의 다른 네트워크 (4] : GSM, DAN, HiperLAN)= 함께 혼합하고 하나의
브라우저로 쉽게 작동하도록 만드는데 있다. 이는 05478와 비슷한 서비스를 제
공하고 사용자 반응을 축적하고 이해하도록 할 것이다. 이는 또한 현존하는 시스
템의 네트워크와 단말기 기술을 살펴보고 간결한 단말기를 생산할 수 있는 기술

에 도움을 = 것이다.

이들 프로젝트는 2000년 3월에 종료 되었다. 새로운 ZHAO! Information
Society Technologies (IST) 프로그램이 시작되었다. ISTHE 소프트웨어 무선설비와 관
ad 최소 개의 프로젝트를 가지고 있다. 참고문헌 [331는 이를 알아보기에 매우 유익

하고 표 8.10은 프로젝트의 목록을 보여준다.

493


===== PAGE 493 =====
최신 이동통신시스템

494

Mobile Communications using MATLAB Simufation

BE 8108

TS 프로젝트에서 소프트웨어 무         련된 프로젝트

구직

기술과

rk
tun

CAST

DRIVE

MOBIVAS

PASTORAL

SATURN

SODERA

Aims at laying the foundations for intelligent and adaptable configuration of the
physical layer in wireless communications links, enabling users to access customized
services over networks operating with different radio standards across different
frequency bands. Targets implementation of the protocol stack by proposing a
three-layer (management, procedural, physical) reconfigurable architecture to provide
the interface between the application and the underlying physical layer of the
terminal processing platform; will build a validation platform to assess the operation
of the proposed architecture for the delivery of selected user services

URL: http://cast5.freeserve.co.uk

Aims at developing methods for dynamic frequency allocation and for coexistence of
different radio technologies (dynamic radio) to increase spectrum efficiency and
reach; will develop an IPv6-based multiradio infrastructure to ensure optimized
interworking of cellular and broadcast networks for the provision of adaptive
high-quality multimedia services in vehicular environments

URL: http://www.comnets.rwth-aachen.de/drive

Aims at developing architectural approaches for integrated software platforms and
systems, adaptable to different network services and technologies, that will open
new opportunities for advanced value-added service (VAS) providers, and at
developing innovative and modular network components for seamless and efficient
service provision, enabling downloadable software-defined radio VAS; will combine
wireless technology with CORBA/TINA principles and with sophisticated QoS
mechanisms

URL: http://www.mobivas.ccrle.nec.de

Aims at developing a reconfigurable, real-time platform for third-generation mobile
terminal baseband development, using FPGA devices developed through a new
cosimulation, codesign methodology that allows for an accelerated design cycle; also
looks into downloading applications and protocols over the air for reconfiguration

URL: http://www. ist-pastoral.org

Looks into adaptive/smart antenna techniques, on both the terminal and the base
station, for outdoor (UMTS) and for local/campus area wireless networks (HiperLAN),
aiming to promote high-bit rate wireless services as well as to provide enhanced
location information for location-based services

URL: http://www. ist-saturn.org

Aims at defining and validating the feasibility of the RF architecture best suited for
reconfigurable radio taking into consideration the terminal constrains of low
consumption, low cost, and small form factor, as well as at studying the optimum
partitioning between different technologies (e.g., BICMOS-SiGe, SOI, and
Micro-Machining); advanced PF libraries will be developed to validate this approach

URL: http://www. ist-sodera.org



===== PAGE 494 =====
표 8.10 (계속)

TRUST          Starting from the user requirements from the perspective of the terminal, investigates
enabling technologies such as analog signal processing, adaptive baseband
processing, novel transceiver algorithms, and smart power management; investigates
also system aspects like spectrum sharing techniques, multimode monitoring,
intelligent mode switching, and software download including security issues

URL: http://www ist-trust.org
WIND-FLEX Investigates high-bit rate adaptive modem architecture, configurable in real time, for

indoor single-hop, ad hoc networks, concentrating on algorithms, protocols, and RF/IF
subsystems

URL: hitp://www.stt. fi/ele/research/els/projects/windflex.htm

본                 에 소프트웨어 무선설비에 대한 요구가 최초로 발생하였다. 일
본 정부는 무선 시스템을 위한 소프트웨어 무선설비에 대한 중요성을 인식하였다 [37].
1996년에, 일본 우정국의 지원으로 ARIBO 의해 연구그룹이 조직되고 3년간의 연구
후에 1999년에 마지막 보고서가 발행되었다. 이 연구그룹은 제한된 사람들에게만 개방
되었다. 소프트웨어 무선설비와 기술에 대한 공개논의 를 a institute of Electronics,
Information and Communication Engineers (IEICE)°]] 의해 소프트웨어 무선설비 연
구그룹이 조직되고 1998년 12월부터 APS 계속해 오포 있다 [38]. 다음은 이 두 그룹
의 최근의 활동에 대한 간단한 소개이다.

(0) 44408에서의 소프트웨어 무선설비 연구 조사그룹 [37]: 연구그룹의 활동은 1996년
부터 3년간 계속되었다. 주된 목적은 다중대역, 다중모드, 다중속도 무선 신호를
위한 범용 단말거의 가능성과 불법 다중대역, OSES, 다중속도 무선 신
시와 사찰의 가능성 조사에 있었다. 위의 목적과 함께, 연구그
에 대해 조사하였다: (1) 소프트웨어 무선 수신기에 적합한 소프트웨어 구조, (2)
소프트웨어 무선 수신기의 구성, (3) 소프트웨어 무선 수신기의 응용시장의 향후
경향, (4) 92의 R&D 경향의 조사, (5) SDR 수시기를 위한 표준화 아이템, (6)

소프트웨어 무선 수신기의 평가 방법. 연구그룹은 또한 무선 신호 감시의 시제품

Tu
rlo
3
ra
ri fol
+"
고

N

495



===== PAGE 495 =====
ka 최신 이동통신시스템
Mobile Communications using MATLAB Simutation

을 개발함으로써 소프트웨어 무선 수신기를 구현 평가하였다.

@ IEICENA S| 소프트웨어 무선 연구그룹 [38 ]: 연구그룹의 활동은 1998년 12월부
터이다. 연구그룹은 081 통신학회에 속한다. 다음 주제들이 논의 된다: (1) 소
프트웨어 무선설비의 이론, (2) 소프트웨어와 하드웨어의 기술, (3) 응용들, (4)
APIo} 대한 연구, (5) 표준화, (6) 다른 나라의 활동 조직과의 정보 교환과 협동
[38]. 이 AS 쓰는 시기에, 6개의 기술 모임이 존재한다. 위 주제에 대한 약 60여
편의 논문이 기술위원회에 제공되었다.

또한, 다수의 연구기관과 기업에서 시제품을 내놓았다. 다음은 이들 시제품에 대해
기술한다. 이 정보는 2000년 10월까지 취합되었다.

0) ARIB [18]: ARIB 연구그룹은 1998년과 1999년에 무선 신호 감시를 위한 소프
트웨어 무선 수신기의 시제품을 개발하였다. 1999년도의 시제품의 구성을 표
8.11에 제시하였다. 시제품은 소프트웨어를 변화시켜 복조방식을 바꿀 수 있다.
시제품은 6개의 요소를 갖는 배열 안테나를 사용할 수 있고 multiple signal
classification (MUSIC) 알고리즘을 사용해 요구되는 파의 도래각을 추정하였다
[39]. 또한, A] a] 4$-= directionally constrained minimization of power (DCMP)

알고리즘을 사용해 원치 않는 ASS 억제할 수 있다 [40].

BE 8.118 ARIB 시제품의 시스템 인자 [18]

주파수 대역                                                         27 MHz, 900 MHz, 2GHz
안테나 어레이                     6-성분 원형 어레이

변조 방식                                                         BPSK, GMSK, FM, AM
비트 레이트                                                          8, 16, 32 Kbps

Direction of arrival 추정 알고리즘          MUSIC [39]

간섭파 억제                      DCMP [40]

(2) Communication Research Laboratory (CRL), M.P.T. [12, 23]: CRL-< 1999
년 지능형 교통 시스템을 위한 소프트웨어 무선 송수신기의 AAS S 개발하였다

496



===== PAGE 496 =====
[23]. 시제품의 구성과 외형을 표 8.3과 그림 8.20에 보였다. 시제품은 그림 8.34에
보인 메뉴를 사용하여 세 가지 SE (Japanese PHS, ETC, GPS) = 사용된다. 시제
품은 최초의 지능형 교통 시스템을 위한 시스템이며 #ㅇ기반 관리 소프트웨어를
사용한다. 시제품은 인자제어 소프트웨어 무선설비 [11]와 8.4장에서 기술된
MMSR [13] 개념을 포함한다.

Mild 8.34 관리 소프트웨어의 메뉴 창.

@ NTT: 찌는 1999년에 고급 이동통신 시스템을 위한 소프트웨어 무선 송수신기
의 시제품을 개발하였다 [41, 42]. 시제품의 구성은 표 8.12에 보였다. 시제품은 3-
배열 안테나를 포함하고 RCR STD28 기반 BS (PHS) 프로토콜을 제공한다. |
한, 시제품은 TDMA/TDD$} FDMA/TDD& 통신방식을 변화시킬 수 있고 /
4QPSK 5} 16-QamS] 다중모드로 작동한다. 게다가, 시제품은 ISDN 네트워크와
연결될 수 있다.

BH 8128 NTT 시제품의 시스템 인자 [41, 42]

RF 대역                       2.45 GHz

대역폭                              13 MHz

주파수 변환 방법            Double superheterodyne

IF                                  2/5/39 MHz

RF/IF 시스템의 수         3

접속 프로토콜                 TD MA/TDD FDMA/TDD

변조방식                      ㅠ/4전이 02910, 16044

통신 레이트                  96/384 Kbps

외부 인터페이스            ISDM (기지국) £9, bearer (71191)

497


===== PAGE 497 =====
최신 이동통신시스템

Mobile Communications using MATLAB Simulation

® TOSHIBA: TOSHIBA® 2000년에 고급 이동통신 시스템을 위한 소프트웨어 |
선 송수신기의 시제품을 개발하였다 [17]. 시제품의 구성은 표 8.13에 보였다. 시
제품은 수신기에서 RF 대역에서 기저대역으로의 주파수 변환 방법으로 8.5.4장
의 직접 변환 기술을 채용한다.

#표 8.138 TOSHIBA 시제품의 시스템 인자 [17]

RF 대역                         1.5/1.9 GHz
대역폭                          10 MHz
주파수 변환 방법              직접 변환

변조방식                           최대 384 Kbps
부호화                          ue

© NEC: NECE 19984 무선 신호 감시를 위한 소프트웨어 무선 수신기의 시제품을
개발하였다 [43]. 시제품의 구성은 표 8.14에 보였다. 시제품은 IF 대역에서 기저
대역으로의 주파수 변환 방법으로 8.5.4장의 언더샘플링 기술을 사용한다. 시제
품은 소프트웨어를 변화시킴으로써 AM, FM, MSK, GMSK, BPSK, QPSK,
7/40829, 8PSK, 16-QAM3} 같은 많은 변조방식을 사용할 수 있다. 변조 인식

알고리즘도 포함된다.
HH 8.148 NEC 시제품의 시스템 인자 [43]
HH BEA            AM, FM, FSK, MSK, GMSK, BPSK, QPSK, 2/4QPSK, 8PSK, 16-QAM
AS 레이트          최대 10 Msymbol/second
음성 코덱         32-Kbps ADPCM, CVSD-PM
샘플링 방법          IF undersampling

© Toyo Communication Equipment and Tohoku Electronics Power Company
[44]: Toyo Comm. 19991 지능형 기지국을 위한 소프트웨어 무선 송수신기

의 시제품을 개발하였다 [44]. 시제품의 구성은 표 8.15에 보였다. 시제품은 소프

498



===== PAGE 498 =====
트웨어 다운로드 기술을 가지고 있다. 소프트웨어를 다운로딩 할 때도 시제품은
통신할 수 있다.

8H 8.158 Toyo Comm, 시제품의 시스템 인자 [44]

변조방식              FM, FSK, BPSK, QPSK, 27/4 QPSK
RF 주파수         370-380 MHz
송신기 대역폭           1.25 MHz
수신기 대역폭          650 kHz
ADC                  12 bits/40 MHz
DAC                 12 bits/40 MHz

@ Hitachi Kokusai Electronic Inc. [19 ]: Hitachi Kokusai Electronic Inc. 2000
년에 고급 이동통신 시스템을 위한 소프트웨어 무선 송수신기의 시제품을 개발ㅎ
였다 [19]. 시제품의 구성은 표 8.16에 보였다. 시제품은 주문제작된 DSPHS 가

지고 있고 송신기와 수신기 간에 완전 이중전신 작동으로 사용될 수 있는 FSK,
BPSK, QPSK, 16-QAM, AM, FM, 568와 같은 다양한 변조방식을 지원한다.

』표 8.168 Hitachi Kokusai Electronic Inc, 시제품의 시스템 인자 [19]

변조방식          FSK, BPSK, QPSK, 16-QAM, AM, FM, SSB (USB,LSB)
IF 주파수        455 KHz-100 MHz
전송 속도          50 60664 Kbps

ADC             12 bit/125 Msps 6 bit/30 Msps

DAC            14 bit/125 Msps 16 bit/30 Msps

다름 기업들도 소프트웨어 무선 시스템을 개발하기 시작하였다. 가까운 미래에 보다
많은 시제품을 보기를 기대할 수 있다.

499



===== PAGE 499 =====
최신 이동통신시스템

ray

Mobile Communications using MATLAB Simulation

6 | 소프트웨어 무선 통신시스템의 향후 응용

500

8.7.1 향후의 이동통신에의 응용
(1) 이동통신 단말기

위에서 언급한 바와 같이, 소프트웨어 무선기술 기반 이동동신 단말기는 사용자가
DSPHS| 소프트웨어를 변화시킴으로써 시스템을 선택할 수 있도록 한다. 또한, 사용자
는 자신이 원하는 서비스 사업자를 선택할 수 있다.

이는 하드웨어 생산품과 산업 쓰레기의 수를 줄일 것이다. 이 점에 대해 8.1장에서 언
급하였다. 그러나이를 구현하기 위해서는 소프트웨어 다운로드 시간의 감소와 함께 소
형화와 저 전력 소비 그리고 하드웨어 비용의 감소를 필요로 한다. 또한 효과적인 시스
템 선택 공정이 필요하다.

2) 이동통신 기지국

소프트웨어 무선기술을 갖고 있는 기지국은 새로운 통신시스템의 구현과 버그의 수
정이 쉽다. 또한, 기지국은 페이딩 WHS 위해 하나 이상의 알고리즘을 사용할 수 있다.
게다가 적응형 배열안테나를 사용함으로써 안테나 빔 형태를 소프트웨어로 제어할 수
있다.

이와 같은 응용을 구현하기 위하여, 프로그램을 쉽게 바꿔 다른 구성소자와 연결시
키기 위하여 이동통신 시스템의 구성소자를 구성할 수 있는 프로그래밍 소프트웨어
위한 규칙을 만들어야 한다. 또한, 실시간 전송을 위해 빠른 ADCY 디지털 신호처리
기가 필요하다.

00

(3) 광대역 무선접속 시스템

소프트웨어 무선기술은 기지국과 건물 사이에서 작동하는 광대역 무선접속 시스템
의 유연성을 증가시킨다. 예를 들어, 왜곡 보상기와 간섭 억제기와 같은 소자들을 위해
수프트웨어를 사용할 수 있다, MAYA 또한 변화시길 수 있고 가장 적절한 구성주자
가 선택된다. 적응형 배열안테나의 사용은 소프트웨어를 통해 빔 형태를 제어할 수 있



===== PAGE 500 =====
ES 한다,
이를 위해서, 각 모듈을 소프트웨어로 만드는 규칙이 필요하고 특히 모듈간의 연결에

대한 규칙이 필요하다. 실시간 전송을 위해서 고속 400나 디지털 신호처리기가 필요

(4) ITS

178에서 사용되는 통신시스템을 표 8.29] 보였다. 세 가지 분류로 나누면 다음과 같
다: 통신기반 시스템, 제어-기반 시스템, 방송기반 ALAR. 통신기반 시스템의 대표적
인 a] PDC, PHS, CDMAS 사용하는 디지털 셀룰러가 있다.

CDMA] 기반 한 제3세대 이동통신 시스템인 IMT-2000°] 가까운 미래에 기대된
다. GPS 시스템, VICS 시스템, 레이다가 제어-기반 시스템의 대표적인 예이다. 교통사
고, 도로 장애물, 기상현상과 같은 ARS 제공하는 고급 운행-16919[ highway system
(AHS) ETC 시스템이 차량에 설치될 것이다. 방송기반 시스템의 대표적인 예로는
라디오 방송시스템, 아날로그텔레비전 방송시스템, 위성 방송시스템, 디지털 텔레비
전 시스템이 존재한다.

위에서 언급한 바와 같이, 118에 나타나는 통신시스템의 수는 계속 증가할 것이다.
]는 많은 서비스가 차량의 제한된 공간에서 제공되기 위해 공간 절약과 시스템 구성요
소의 BAC] 중요한 관심사임을 의미한다. 소프트웨어 무선기술은 이들 서비스가 하나

의 작은 단말기로 ASS 수 있는 가능성을 가지고 있다. 그림 8.35는 잠재적인 응용을

ㅇ

소프트웨어 무선기술을 실현하는 PHS 응용 (1)(3)에서와 같다. 175에서, 한 대의
차량에서 사용될 수 있는 서비스의 수는 10가지가 넘는다. 그래서 소프트웨어 무선기

술의 구현이 가능한 빨리 이루어져야 한다.

\

501



===== PAGE 501 =====
Mobite Communications using MATLAB Simulation

00
WE aid! se Peat i, eS                                            010
기시 이 OE Pe Meee ANE AY 0002“i                        or
*＊  룩                                                                                                                      ~  뻐                  a
ee Te Pe        Pea
책                                                                                                           Bal
asengjos payepan                                              개                        마

                        40 Meu peajumop      3
fie.    oo          Jo uonesunuwo) . . , . , A                          (313)                Ss
aE
(ALN ‘War te} 280s pavepdn                                          티미                  wl

PORE DE EMOP        suonediunwwod 히140

4011619 801/485           바이 ance      {(suones!             119이시)                        HI
Bunseopeoig     ed        :                                    uoneys aseg                           <4

00
(AL 910465 '609)                                                                =O
anaes                                          기
mag
[00]
(0000 ZH9-5)                                                              e
Buuajue                                                              -
(ana 사하 euuawe sgg-d me HOZSN  ie                              aiemyos                        a
eipew
8684018          sary  \ 0002-LINI                                    payepdn 10 Mau                            Me
a                                     a           Ws9 ‘90d                                                                        peojumog                                                 ©           oto
SHd ‘Sd9      0                     Ni cea ae ne hunite Ss      lo
na
더      do
7     0
N
iar
00

}

ay

다중모드, 다중표준수

1.

coy
(그

}드웨어에 새로운 서비스를

Ke}

의

uU

진할 수 있다. 이러

바꿈으로써 기
Was =

]

ㅇ
+

=

=

웨어 무선기술은 지상파/기지국/회로변환/케이블 TV 간의 자동변환을 실현
의 세계적

Jo}. 또한, 소프트웨어

=

a

ATE

하기 쉽다. 뿐만 아니라 많은 나라의 표

ㅇ

502



===== PAGE 502 =====
신기는 광대역 안테나와 특정 통신시스템의 구성소자를 기술하는 소프트웨어를 필요
로 하고, 이는 구성소자 간의 연결성이 증가해야 함을 의미한다.

8.7.3 사유 네트워크

최근에는, 많은 사유 네트워크가 교육이나 회사 혹은 통신, ITSY 긴급 상황과 상용
목적으로 존재한다 (그림 8.36). 이러한 네트워크의 현존하는 단말기는 서로 연결성을
가지고 있지 못하다. 소프트웨어 무선설비는 어떠한 사유 네트워크에서도 작동하는 범
용 단말기를 만들 수 있다. 이는 거대한 네트워크가 구성될 수 있음을 의미한다. 가까운
미래에, 이러한 거대 네트워크가 일반적인 공유 네트워크와 대치할 것이다.

For the educational use

를 그림 8.36 AG 네트워크의 소프트웨어 무선설비 응용

8.7.4 소프트웨어 무선설비의 인증 방법
소프트웨어 무선설비의 실제 구현에 있어서 하나의 문제점이 무선 테러리즘이다
[14]. 잠재적인 Bale] 형태를 그림 8.37에 보였다. 어떤 경우에는, 다운로드 된 데이터
가 불법적으로 변화될 수 있거나 컴퓨터 바이러스를 포함하고 있을 수 있다. 변형된 소
프트웨어나 바이러스 소프트웨어에 의해 기지국이 손상되거나 작동을 멈출 수 있다. 또
503



===== PAGE 503 =====
최신 이동통신시스템

Mobite Communications using MATLAB Simulation

한, 이러한 다운로드 소프트웨어의 종류가 송신기와 수신기에서 서로 달라서 그 결과
단말기가 갑자기 높은 파워 신호를 방출할 수 있다. 이러한 무선 테러리즘에 대항하기
위해, 소프트웨어 무선설비에 사용되는 시스템의 새로운 인증 방법이 인증기관에 요구
된다.

The kinds of software are

~
o
본
든
a
e
©
oI
c
o
를
@
a
c
oS
£
3

and receiver.

|

Suddenly high power
signals generate.

Base station is destroyed.
L

=

Virus is stationed in the terminal.

Data are altered.

Downloads failed.

Maid 8.37 무선 테러리즘.

504


===== PAGE 504 =====
인증의 한 예를 그림 8.38에 보였다. 인증 방법은 두 단계를 거친다. 첫 번째 단계에
서, 인증기관에서 다수의 시스템을 구성하는 소프트웨어를 변화시킴으로써 입력 데이

터와 출력 데이터의 관계를 검사한다. 이 경우, 전송 파워, 전송 대역폭, 이웃한 주파수
대역에서의 전기 전력 누수가 각 시스템에서 측정되고 각 나라의 무선 법과 비교함으로
써 평가된다.

nc-혜 |/F

160마           |

i" Standardization
point

oswor frame} oswoH{CodinghoswoH Mapping andhoswoHfUpsample [06009
or              Of | {modulation            or

— WF                  VF                  VFo                     나                      sibs
Transmitter
Correlation
            :       Code timing  be
-bewd PSwoCorrelationSWH ne = | [06
or         or          OF | et | OF
그                         VE                          VF o-{Symbal timing}o 바이
sync

L—_tResampleHosy  emapping andkosyyoH{Decoding
or      ㅣ   or
VF         VF        총
Receiver
(b)

Mle 8.38 소프트웨어 무선장비의 인증 방법: (3)첫번째 단계 (6)두번째 단계.

프트웨어가-잘 동작하면.-인증기관은 SZEMolol] 인증 ASS 부여한다. 인증
점

암호는 268에 소프트웨어를 다운로드하7

505



===== PAGE 505 =====
aR 최신 이동통신시스템
Mobile Communications using MATLAB Simufation

으로 사용된다. 응답확인 동안, 암호가 인증되면 소프트웨어가 메모리로부터 DSPHZ
다운로드 되고 그렇지 않으면 소프트웨어 장비가 경고를 한다. 최악의 경우, 장비는 스
스로 파괴된다. 공개 키 암호기술을 인증 암호로 사용할 수 있다. 또한, 메모리와 DSPH
간의 다운로드 프로토콜이 표준화되어야 하고 인증된 프로토콜을 사용해야 한다.
인증의 두 번째 단계는 소프트웨어 무선설비를 구성하는 BSS 포함한다. 각 구성요
소를 인증하기 위해, 소프트웨어 무선설비의 구성이 변화되어야만 한다. 구성의 한 af
를 그림 8.38(06)에 보였다. 여기서, 스위칭 혹은 인터페이스 모듈이 소프트웨어 무선장
비를 구성하기 위해 기능 모듈 Apolo] 삽입되었다. 이들 스위칭 혹은 인터페이스 모듈
은 DSPH 외부에서 제어될 수 있다. 스위칭 모듈로 각 기능 모듈이 인증된다. 스위칭 혹
은 인터페이스 BSS 인증공정이 ASSES 표준화되어야 한다.

00981 =

이 책에서 공부한 소프트웨어 프로그래밍의 미래 응용 분야 중 하나가 소프트웨어 통
신시스템이다. 소프트웨어 무선설비의 개념은 이 책에서 공부한 소프트웨어 프로그래
밍기법을 토대로 디지털 하드웨어 구현을 할 수 있게 해주는 통신용 프로그래밍능력과
디지털 하드웨어 구현능력의 가교 SSS 한다.

이 장에서는 소프트웨어 무선 통신시스템의 장점과 문제점들에 대해 기술하였다. 소
프트웨어 무선 통신시스템을 구현하기 위한 기술과 향후 응용에 대해서도 또한 논의되
었다. 이 기술은 최근에는 세계적으로 많은 시스템이 존재하고 이러한 시스템이 집적되
어야 하므로 차세대 이동통신 시스템의 성공에 열쇠가 될 것이다. 이 책에서 논의된 이
러한 쟁점들이 시스템을 집적하는데 유용하게 활용될 것이다.

506


===== PAGE 506 =====
1) Mitila, J., “The Software Radio Architecture,” IEEE Commun. Mag., May 1995, pp.26-38.

2) Lackey, R. J., and D. W. Upmal, “SPEAKeasy: The Military Software Radio,” IEEE Commun.
Mag., May 1995, pp.56-61.

3) European Commision DG XIIIB: Proc. of Software Radio Workshop, May 1997.
4) Special Issue on the Globalization of Software Radio, IEEE Commun. Mag., February 1999.

5) Special Issue on Software Radio, IEEE Personal Communications, August 1999.
6) Special Issue on Software and DSP in Radio, IEEE Commun. Mag., August 2000.

7) Special Issue on Software-Defined Radio and Its Technologies, IEICE Trans. on Commun.,
June 2000.

8) Kohno, R., “Structures and Theories of Software Antennas for Software Defined Radio,”
IEICE Trans. Commun., Vol. E83-B, No.6, June 2000, pp.1189-1199.

9) Karasawa, Y., “Algorithm Diversity in a Software Antenna,” IEEE Trans. Commun., Vol. E83-
B, No.6, June 2000, pp.1229-1236.

10) Magnum, C., “Market Opportunities II: The MMITS Forum Market Forecast Study,” Ist
International Software Radio Workshop, Rhodes, Greece, June 1998, pp.15-24.

11) Harada, H., and M. Fujise, “Multimode Software Radio System by Parameter Controlled and
Telecommunication Toolbox Embedded Digital Signal Processing Chipset,” Proc. of 1998
ACTS Mobile Communications Summit, June 1998, pp.115-120.

12) Harada, H., Y. Kamio, and M. Fujise, “Multimode Software Radio System by Parameter
Controlled and Telecommunication Component Block Embedded Digital Signal Processing
Hardware,” IEICE Trans. Commun., Vol. E83-B, No.6, June 2000.

13) Harada, H., “A Proposal of Multimode & Multiservice Software Radio Communication
Systems for Future Intelligent Telecommunication Systems,” Proc. of International
Symposium on Wireless Personal Multimedia Communications (WPMC’99), September 1999,
pp.301-304.

14) Harada, H., “Wireless Terrorism,” Denpa-shinbun newspaper, May 30, 2000.

15) Tsurumi, H., and Y. Suzuki, “Broadband RF Stage Architecture for Software-Defined Radio in
Handheld Terminal Applications,” IEEE Commun. Mag., Vol.37, No.2, February 1999, pp.90-
95.

507


===== PAGE 507 =====
최신 이동통신시스템

508

Mobile Communications using MATLAB Simulation

16) Tsurumi, H., et al., “Broadband and Flexible Receiver Architecture for Software-Defined
Terminal Using Direct Conversion and Low-IF Principle,’ IEICE Trans. Commun., Vol. E83-B,
No.6, June 2000, pp.1246-1253.

17) Yoshida, H., et al., A Software-Defined Radio Using Direct Conversion Principle, Technical
Report of IEICE, SR00-09, April 2000, pp.59-66.

18) Yokoi, T., et al, “Software Receiver Technology and Its Applications,” IEICE Trans. Commun.,
Vol. E38-B, No.6, June 2000, pp.1261-1268.

19) Ide, T., et al., “Development and Evaluation of Software Radio Prototype, IEICE Technical
Report, SRO0-23, October 2000 (in Japanese).

20) Vanghan, R. G., N. L. Scott, and D. R. White, “The Theory of Bandpass Sampling,” IEEE
Trans. Signal Proc., Vol. 39, No.9, September 1991, pp.1973-1984.

21) Henrchel, T., and G. Fettweis, “Sample Rate Conversion for Software Radio,” IEEE Commun.
Mag., Vol.38, No.8, August 2000, pp.142-150.

22) Sawai, R., et al., “An Adaptive Symbol Timing Synchronization Method Multimode &
Multiservice Software Radio Communication System,” IEICE Trans. on Communications, Vol.
E84B, No. 7, July 2001, pp.1885-1896.

23) Harada, H., Y. Kamio, and M. Fujise, A New Multimode and Multiservice Software Radio
Communication System for Future Intelligent Transport Systems, Technical Report of IEICE,
SR99-21, September 1999 (in Japanese)

24) Sawai, R., et al., “A Feasibility of an Adaptive Sampling Processing Method for Software-
Defind Radio,” Proc. of 2001 IEEE Vehicular Technology Conference Spring (VTC2001-
Spring), Rhodes, Greece, May 2001.

25) Walden, R. H., “Performance Trends for Analog-to-Digital Converters,” IEEE Commun. Mag.,
Vol.37, No.2, February 1999, pp.90-95.

26) Cummings, M., and S. Haruyama, “FPGA in the Software Radio,” IEEE Commun. Mag.,
Vol.37, No.2, February 1999, pp.108-112.

27) http://www.altera.com/.
28) http://sdrforum.org.

29) Cummings, M., J. Hoffmeyer, and S. Blust, “Modular Multifunctional Information Transfer
System Forum,” Ist Software Radio Workshop, Brussels, Belgium, May 1997.

30) http://www.darpa.mil/ito/research/glomo/index.html.
31) http://www.darpa.mil/ito/research/glomo/projects.html.

32) Tuttlebee, W., “Software Radio: Developments in Europe,” Ist Internal Software Radio
Workshop, Rhodes, Greece, June 1998, pp.49-61.



===== PAGE 508 =====
33) Pereira, J. M., “Redefining Software (Defined) Radio: Reconfigurable Radio Systems and
Networks,” IEICE Trans. Commun., Vol. E83-B, No.6, June 2000, pp. 1174-1182.

34) Erben, H., and P. Crichton, “Software Radio Architecture for UMTS,” Proc. of 1997 ACTS
Mobile Communications Summit, Aalborg, Denmark, October 1997.

35) Kenington, P. B., D. W. Benett, and R. J. Wilkinson, “RF Transceiver Architectures for
Software Radio Design,” Proc. of 1997 ACTS Mobile Communications Summit, Aalborg,
Denmark, October 1997.

36) Tayler, C., “A DSP System for a Software Radio Testbed,” Proc. of 1997 ACTS Mobile
Communications Summit, Rhodes, Greece, June 1998.

37) Araki, K., “Prehistory of the SDR Studies in Japan-A Role of ARIB Study Group,” IEICE
Trans. Commun., Vol. E83-B, No.6, June 2000, pp.1183-1188.

38) Kohno, R., et al., “Overview of Japanese Activities in Software-Defined Radio,” 12th
Tyrrhenian International Workshop on Digital Communications, Elba, Italy, September 2000.

39) Schmidt, R. O., “Multiple Emitter Location and Signal Parameter Estimation,” IEEE Trans.
Antennas and Propagation, Vol. Ap-34, No.3, March 1986, pp.276-280.

40) Takao, K., M. Fujita, and T. Nishi, “An Adaptive Array Under Directional Constraint,’ IEEE
Trans. Antennas and Propagation, Vol. AP-24, No.5, May 1976, pp.662-669.

41) Uehara, K., et al., Software Radio Base and Personal Station Prototype (1), Technical Report of
IEICE, SR99-10, September 1999, (in Japanese), pp.1-8.

42) Suzuki, Y., et al., “Software Radio Base and Personal Station Prototype,” IEICE Trans.
Commun., Vol E38-B, No.6, June 2000, pp.1261-1268.

43) Ishii, H., T. Yamamoto, and T. Higuchi, Development of Software Radio for Radio Monitoring
System, IEICE Technical Report, RCS98-71, July 1998 (in Japanese).

44) Yokoi, A., et al., Development of Software Radio and Performance Measurement, IEICE
Technical Report, SR99-2, June 1999 (in Japanese).

509


===== PAGE 509 =====
*편역자 소개

차재상                     (현) 서경대학교 정보통신공학과 교수
(chajs@skuniv.ac.kr)         일본 SH (Tohoku) Sta 공학박사(전자공학)
한국전자통신연구원(8140) 이동통신연구소 선임연구원
정보통신연구진흥원, 산업기술평가원, 정보통신부 평
관심분야 : 이동통신, 유무선 홈네트워크, 디지털방송

이종현                  (현) 서경대학교 전자공학과 교수
(chonglee@skuniv.ac.kr)       KAIST 공학박사(전기 및 AAS Sh)

강장묵                 (현) 서경대학교 컴퓨터공학과 겸임교수
(mooknc@paran.com)           고려대학교 공학박사(정보보호) 수료

(주)쌍용정보통신 컨설팅팀 컨설턴트
정보통신부, 한국정보보호진흥원 평가 및 자문위원
관심분야 : 유비쿼터스 컴퓨팅, 0814

Sala                     (&) KAIST 박사과정

(jcwang@sclab.kaist.ac.kr) | 연세대학교 전자공학과 졸업

KAIST 전기 및 전자공학과 석사 및 전자전산학과 박사수료
연구분야 : 검파 및 추정, 영상처리, 통신 및 레이다 신호처리

1&71Ｌ4^8실습예제가 풍부한

최신 이동통신시스템

wy
pu ret

초판 인쇄일 *ㅎ 20054 38 74
초판 발행일 Pp  2005년 3월 12일
편역자 * | 차재상ㆍ이종현ㆍ강장묵ㆍ왕진천
발행처      > 도서출판 그린
발행인     > 윤덕우
출판등록 pb ㅣ 제8-161호(1995. 5. 3.)
주소       > AS) 서대문구 연희동 219-20 (우)120-828
선화      Pm  02)333-2574, 2575
Fax       >  02)333-2561
E-mail     >  greenpress@greenpress.co.kr
Homepage >»       http://www. greenpress,co,kr
정가 : 25,0002!
ISBN : 89-5727-063-9
※ 무단 복제를 금함. 잘못된 책은 바꾸어 드립니다

