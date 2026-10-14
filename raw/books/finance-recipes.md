---
source_url: /Down/전자책/금융공학레시피.pdf
ingested: 2026-10-15
sha256: 22a75b8ab95308063a1d45464b2f0f433f47ed45013011c4ab6055ee087a4e55
---

# 파이썬을 활용한 금융공학 레시피 — raw source

> **Warning:** scan-only PDF. OCR'd via tesseract (kor+eng, 300dpi); occasional garbled tokens — cross-check the original PDF when interpreting.

## Book metadata
- **Title:** 파이썬을 활용한 금융공학 레시피 (Financial Engineering Recipes with Python)
- **Author:** 김용환 (지음), 감수: 장민자, 노태협
- **Publisher:** 한빛미디어 (Hannbit Media)
- **Year:** 2018 (초판 1쇄 2018-06-14)
- **ISBN:** 979-11-6224-082-3
- **Pages (OCR):** 400
- **Example source:** https://github.com/finterstellar/download

_OCR text follows verbatim (page markers preserved)._



===== PAGE 1 =====
}쟁의 코딩 물렁증과
}쟁의 2S Suse
0 NOE  .…
공학 사이다 ©

킴용환 지음                                               of | 」
장민자, 노태협 감수



===== PAGE 2 =====
파이썬을 활용한 금융공학 레시피

문과생의 코딩 울렁증과 이과생의 SS 울렁증을 한 방에 HS 금융공학 사이다

초판1쇄발행 2018년 6월 14
초판 44 WY 20214 2월 19일

자은이 김용환 / 감수자 장민자. 노태협 / 베타리더 이기성 / 펴낸이 김태헌

DER 한빛미디어(주) / 주소 서울시 서대문구 연희로2길 62 한빛미디어(주) [1 출판부

전화 02-325-5544 / BA 02-336-7124

등록 1999년 6월 24일 제10-1779호 / ISBN 979-11-6224-082-3 93000

총괄 전정아 / 책임편집 홍성신 / 기획 박지영 / 편집 이상복 / 교정 정안나 / 진행 김대현

디자인 표지 내지 최연희 / 전산편집 백자선

영업 김형진. 김진불. 조유미 / 마케팅 Hs. SSA 조수현. OBS 고광일 / 제작 박성우, 김정우

이 책에 대한 의견이나 오탈자 및 잘못된 내용에 대한 수정 정보는 한빛미디어(주)의 홈페이지나 아래 이메일로
알려주십시오. 잘못된 책은 구입하신 서점에서 교환해드립니다. 책값은 뒤표지에 표시되어 있습니다.
한빛미디어 홈페이지 www.hanbit.co.kr / 이메일 ask@hanbit.co.kr

Published by Hanbit Media, Inc. Printed in Korea
Copyright © 2018 2#! & Hanbit Media, Inc.

이 책의 저작권은 김용환과 한빛미디어(주)에 있습니다.

저작권법에 의해 보호를 받는 저작물이므로 무단 복제 및 무단 전재를 금합니다.

자금 하지 않으면 할 수 없는 일이 있습니다.
책으로 펴내고 싶은 아이디어나 HTH OS (writer@hanbit.co.kr)= 보내주세요.
한빛미디어(주)는 여러분의 소중한 경험과 자식을 기다리고 있습니다.



===== PAGE 3 =====
문과생의 코딩 울렁증과
이과생의 SS 울렁증을
SO NOB os
금융공학 사이다 ©

*

킴용환 지음                                                 a all 0 |
IX}, 노태엽 감수

oy
ㅁ

Hs 힌빛민딘이

^”


===== PAGE 4 =====
지은이 ㆍ감수자 소개

지은이 감용환 finterstellar@naver.com

SK 0&0에서 프로그래머로 사회생활을 시작했으나 금융권에 있는 친구들이 더 우아하게 살
면서도 높은 ASS 받는다는 사실에 분개해 한국거래소로 이직, 지금까지 15년 이상 금융과
ITS] AANA 활동하고 있다. 연세대학교 산업공학과를 거쳐 캘리포니아대학교 어바인에서
MBAS 취득했다.

감수자 장민자 CFA

한국투자공사(610) 창립 멤버로 국부펀드 운용 시스템을 설계했고, 현재 투자오퍼레이션팀
에서 주식 및 채권 파트 백오피스를 책임지고 있다. 삼성515 금융부문 역임.

감수자 노태협 교수

덕성여자대학교 경영학과에서 차세대 금융 인재를 가르치고 있으며, 경영학과 rr
107 분야에서 활발한 연구를 진행 중이다.

00

용합한



===== PAGE 5 =====
추천사

융합의 시대, 하나의 전문 지식만으로는 부족하다. 금융과 [1가 결합한 금융공학이야말로 4차
산업혁명 시대를 준비하는 최고의 무기가 될 것이다.

안상환 (한국거래소 부이사장)

이제 IT 없는 FES 상상하기 어려워졌고, 금융과 ITS] 접점에는 금융공학이 있다. 이 책을
통해 더 많은 사람이 금융공학에 흥미를 느끼게 되길 바란다.

신재룡 (코스콤 전무, 한국거래소 8』/ CO)

금융공학 프로그래밍을 배우고 싶은 경상계열 출신의 눈높이에 딱 맞는 금융공학 입문서.

이화수 (한국증권금융 팀장, 서울대학교 경제학과)

금융과 11, 두 마리 토끼를 동시에 잡을 수 있는 책. 금융 1 융합 인재가 되고 싶은 모든 이에
게 추천합니다.

김찬현 (한국수출입은행 부부장. KAIST 전산과)

경제지 기자들도 어려워하는 파생상품을 가장 쉽게 알려주는 명강사가 쓴 금융공학 책! 빅데
이터와 파이썬은 덤.

SES (매경이코노미 증권팀장 / 매일경제 기자)

금융업계로 진출하고 싶은 학생이라면 꼭 알아야 할 내용이 모두 담겨 있는 단 한 권의 필독서.

안재준 (연세대학교 투자공학과 교수)


===== PAGE 6 =====
지은이의 말

리베로, 수비수이면서 공격에도 적극 가담하며 경기를 리드하는 핵심 포지션을 뜻하는 축구
용어입니다. 대학 AAS 시간에 교수님께서 산업 현장에서 산업공학자의 역할이라고 설명해
주신 용어였죠. 금융산업에서 금융공학자의 역할 역시 리베로와 같습니다. 다른 말로는 용합
인재. 멀티플레이어라고도 합니다. WE, 제도, 상품 개발, 시스템 설계 등 다양한 역할을 수
행해서 그렇습니다.

거래소에서 금융공학을 하고 있으니 금융공학을 잘 모르는 많은 사람들이 제 ASS SS
다. 경영인지 인지. 경영학 석사라 경영 ASS 맞긴 하지만 ITS 배우지는 않았습니다. st
지만 현업 부서 사람들은 모델링을 위해 코딩하는 BSS 보고 AS 17 전공자로 오해합니다.
반대로 17 부서 사람들은 제가 시장이나 제도 등을 분석할 때 MBAz} 이런 걸 할 수 있구냐'
생각합니다. 멀티플레이어, 아무 일이나 다 할 수 있다고 여겨지다 보니 새로 개척하는 신규
사업, 해결사가 필요한 분야 등의 에 자주 투입되었죠. 보수적인 금융기관의 퀸트가 겪어온
현실입니다. 하지만 이제 금융 공기업들도 금융공학의 중요성을 인식하고 관련학과 SAYS
채용하기 시작했습니다.

글로벌 금융시장에서 치열하게 경쟁하는 국내외 대형 증권사들은 벌써부터 금융공학의 중요
성에 대해 제대로 인지하고 금융공학자들로 구성된 조직을 만들어 BE 트레이딩, 41 등 금융
공학 기반의 비즈니스를 육성하고 있습니다. 이들 회사에서는 이미 이러한 비즈니스가 가시적
인 성과를 내는 수준에 이르렀고, 이러한 성과는 더 많은 금융공학자에 대한 수요로 나타나고
있지요.

5

4차 산업혁명의 SAS 금융공학자의 역할을 진화시키고 있습니다. 지금까지의 융합 인재는
한 Hol] 두 가지 이상의 업무를 = execution) Bok 했다면, 앞으로의 금융공학자는 판단
(06019107)을 위주로 하고 업무 수행은 Al] 맡기는 시대가 되는 것입니다. AS 기반으로
한 4차 산업혁명이 지식 노동자들을 퇴출시킨다고 하지만, 융합 지식을 갖추고 복합적인 사고



===== PAGE 7 =====
를 하는 FSS ALS 디자인하고 41에게 일을 시킬 수 있는 사람이 될 수 있습니다. 실
제로 지금까지 금융산업에서 ALS 이끌어온 그룹도 금융공학자입니다.

지금까지 금융공학을 공부하면서 수없이 많은 관련 AAS 읽었습니다. 하지만 한 번도 쉽게
쓰여진 책을 읽어보지는 못했습니다. 한정된 지면에 금융, 통계학, 공학 등 여러 분야의 전문
지식을 쏟아내기가 쉽지 않기 때문이죠. 그래서 저는 세상에서 가장 쉬운 금융공학 책을 쓰고
싶었습니다. 쉬운 레시피로 세상 사람들을 주방으로 불러들인 <집밥 백선생>처럼, 간단한 엑
셀과 파이썬 실습으로 SAS 금융공학의 AAS 안내하려고 합니다. 금융공학에 새롭게 관
심을 갖게 된 사람이 이 AS 읽고 “of, 할 만하구나"라고 말한다면 글쓴이로서 더없이 보람찰
것입니다.

인생 Al 책을 쓰면서 그동안의 커리어를 정리해봤습니다. 첫 직장에서 시작한 Ｌ, 거래소에서
의 첫 업무 인덱스, 카투사 출신이라고 떠맡은 해외 사업과 해외 기업 상장 유치, 구조화 상품
인 ELW, ETF 시장을 관리하며 시작한 BE, 대한민국 모든 증권거래를 처리하는 매매 시스
템 EXTURE+ 구축 등 다양한 US 했습니다. 앞으로 어떤 일을 하게 될지 저도 궁금하네요.
다만, 금융공학을 확보해두었으니 더 재미있는 일을 할 수 있을 거라는 기대감만은 확실합니
다. 독자 여러분도 이 책을 통해 언젠가 이러한 마음을 느낄 수 있으면 좋겠습니다.

처음 원고를 쓸 때 인터넷을 통한 시세 데이터 수집은 구글 파이낸스를 이용했지만, 2018년
초 구글이 해당 서비스를 중지해 데이터 소스를 구글과 네이버로 수정했습니다. 이러한 일은
빅데이터 수집 과정에서 흔히 발생하는 일이며, 혹시 출판 이후에 유사한 일이 발생하면 이 책
의 공식 웹사이트인 1『+0://0376.0246『「.000/+1016「516110『 를 통해 다른 방법을 안내해
드리겠습니다. 기타 문의 및 건의 사항은 106「516113「003\6「.ㅇ01으로 보내주세요.

금융공학을 접하고 본격적으로 재미를 붙이도록 도와주신 거래소 선후배이자 증권상품부 동

료인 김영, 이근영, PFE, MES, 김영인 님, AS 감수해주신 한국투자공사 장민자 책임


===== PAGE 8 =====
님, 덕성여자대학교 노태협 교수님, 베타리딩을 맡아준 이기성 님에게 감사드립니다. 무엇보
다 주경야독하며 BBWS 마칠 수 있도록 아낌없이 지원해준 아내, 야빠와 놀고 싶어도 FH 참
아준 아이들에게 감사합니다. 그리고 항상 응원해주시는 어머니, 아버지, 장모님, 장인어른께
감사합니다.

2018년 5월
김용환


===== PAGE 9 =====
이 책에 대하여

코딩 교재? NO!

금융공학에서 프로그래밍은 본질이 아닌 도구입니다. 금융공학자가 최고의 프로그래머가 될
필요는 없지요. 그럼에도 금융공학자는 프로그래밍을 할 수 있어야 합니다. 하지만 프로그래
밍 초보자에게는 코딩 기초 교재조차도 쉽사리 읽히지 않는 넘사벽으로 느껴지는 것이 일반적
인 현실입니다. 그렇게 쉽다고들 하는 파이썬도 마찬가지로, 언어 버전도 2 x9} 3.×가 있고,
프로그래머의 기호에 따라 선호하는 개발 환경이 다르고 설치 방법도 제각각입니다. 다양한
방법을 다 따라가려고 하다 보면 코딩은 시작도 못 해보고 환경 구성에서 막혀 진도를 나갈 수
없습니다. 큰맘 먹고 구입한 두꺼운 코딩 교재는 50페이지까지만 펼쳐보고 책장 구석으로 처
박혀버리기 일쑤지요.

필요한 만큼만 배우고 바로 활용하기

그래서 준비했습니다. 이 책은 어려운 이론서가 아닙니다. '딱 필요한 만큼만 배워서 바로 활
용하기'를 BES 합니다. FEE, 코딩도 여러 배경과 다양한 이론이 있고, 사람마다 선호하
는 이론도, 활용 방법도 다릅니다. 이를 모두 고려하다 보면 진도가 안 나갑니다. 이에 현재
시점에서 금융권에서 가장 일반적으로 활용되는 이론을 설명하고(수학적 SAE 어려우니 넘어갑
니다), 엑셀로 실습해보고, 연습한 내용을 파이썬으로 구현하기 위해 필요한 코딩 기술을 익힙
니다. 마지막으로 이론과 실습으로 숙지한 내용을 토대로 파이썬을 이용해 실제 금융시장 gl
이터로 모델을 만들어봅니다.

빅데이터 활용
금융공학은 데이터 EAS 통해 솔루션을 찾습니다. 이 과정에서 주가 데이터와 같이 깔끔하


===== PAGE 10 =====
게 BAS 데이터도 이용하지만, 뉴스. 기업공시와 같이 So] 정해지지 않은 비정형 데이터
도 이용하게 됩니다. 비정형 데이터를 수집하고 분석하려면 금융공학자는 빅데이터 기법과 친
숙해져야 합니다. 이 책에서는 자연어 처리와 같은 고급 빅데이터 기술은 사용하지 않지만 주
가 데이터 수집 등을 위해 빅데이터 기법을 활용합니다. 코딩 기술 부분에서 빅데이터와 데이
터 과학에 필요한 코딩 기술을 익혀보세요.

실습 환경

이 책을 집필할 때는 윈도우 10 운영체제를 사용했지만, 다른 버전의 윈도우나 맥에서도 이
책 내용을 실습하는 데 문제는 없습니다. 엑셀은 윈도우용 엑셀 2013을 사용했는데. 버전이
다르면 메뉴의 위치 등이 다를 수 있습니다. 파이썬은 3.6 HAS 사용합니다. 3.x 버전의 파
이썬은 모두 사용 가능하지만, 2.x 버전과는 호환되지 않습니다. 3.x 버전이라면 맥에서도 동
일하게 사용이 가능합니다.

기본 웹 브라우저는 구글이 만든 크롬을 사용합니다. 크롬은 운영체제와 상관없이 동일한 사용
환경을 제공한다는 장점이 있으며, 데이터 수집을 용이하게 하는 XPath 등의 기능을 제공해 편
리합니다. 아직 크롬을 사용해보지 않은 분이라면 꼭 사용해보기를 권장합니다. 크롬 브라우저
를 설치하려면 검색엔진에서 ae oe 검색하거나 ||【【ㅁ5: //ww.google.com/chrome/ ol]
접속해서 다운로드할 수 있습니다.

책에서 실습에 사용한 파일은 이 책의 공식 웹사이트인 http: //book. finterstellar.com
또는 깃허브 저장소 https://github.com/finterstellar/download 에서 다운로드할 수
있습니다.

10


===== PAGE 11 =====
CONTENTS

지은이ㆍ감수자 AP coreeeeecsessecccrceccccceececssseesseecsscscsnssnesecseescseseccsnsnscnsssecseessssersnasssssssscsncesesessssnacssenseeceseseessesenee 4
ZEA Afrveveeesececccecsecersseessecsecencceeeceeseeceneneecesensenssssscenessesssesessecsanecceccasesereneaccssenssaasaasuasusacacesssccssessscseceesssnceeesesse 5
지온이의 Dfeeeennerereeeesevesevcceccccerccccecssscnsssnsnccssscscsssnvernscosscsssnsensneneaceecsseeseassocsseveccasensesnes scenes acsesncesencccseesecasssesens 6
이 책에 CHEPOY-----+---e22eeenenrerececreccseccecesccnsccceesesssenneoccccesccessesensanecceesessserecensccesseccecsesensssecoscnnscaceenenescessenccscessnnce 9

Port] 준비하기

Chapter 1  금융공학이란?

1 By |  금융상품의 진화……ㅇㄴㄴㄴㅇㄴㄴ0ㄴ00000000000000000004000000000000000000000000000000000000000*000000000<00000<00000000040<ㄴ000000009000 23
은행10000000009000000000000009000900000000000*0000000000000000000<0<<00000000*<ㄴ000000000000000000<00<000000000-000009000000000000000< 23
보험000000900000000000000000000040000000000000000000090000000000000000000000900000000000000000000000090000004400904000000000000000000 24
주식eee een eereceseeesnsnensccsesnassesenesecseseeeeesseeeeeseeeseeeeeeseen teeeeee eee seeesenseessaessasecsessecseesssesescecccesees 24
파생상품ㄴㄴ000000000ㄴ900090090016000090000900000시시시00니니0009000000000000090000190000000900000000909000900990990001400009001000 25
구조화 상품ㄴㅇㅇ0000000000000000000000000000000600000000ㄴ000000000000000<00000000000000000000000000000000000000000000000ㄴ400<000000 25
1.2 금융공학 = 금융 + 모델링 oeeeeeeeeeeeecsecseeeeeeeseeseessessnsensesansanseseeescssseseceessseesersnassensessceserscsesees 27
1.3 금융공학자 FT ADA peceeseceeeeceeneeeceeereneseenesecrsnessseeseesseesssersseessenssssssnsesessenseseeasnneceerensess 27
Chapter 2 돈의 시간 FAI
2.1 미래가치('/) 계산Meee ee seen ne eeeseaeeeneeeenesassnennsesseeessesseseeesseesesseseneseeesess essere eeseeesnssassenecesseeseeses 29
2.2 현재가치(2\/) 계산…ㅇㄴㄴ09090000000900000000000000090090005000000000000000000000900000000000090000090090000009099000000009090910 30
2.3 금융공학과 돈의 AIZWIR] ceeeeseeeeeeeeecteeeeeeesesecneesesteneneessereasnassesecseseneeeseeeseessessseerseereacenseeenes 30
Chapter 3  파이썬  설치
3.1 아나콘다로 한 방에 DALY | c-evseeecccessseessceecccencecssscnnscsessscecseceesenseseeseeeesnsessascnarscseressesesseenees 31

11


===== PAGE 12 =====
——

CONTENTS
3.2 주피터 노트북으로 파이썬 명령 실행 ene eneeeeeeeeceseeeeceesescnsscntecnsetncnescesstarssssensnersnsecssnansnsnenseees 38
QS Pa UINO Prd oer) ereetenteeecete vad varetesctccaccereucceseceareccyeuqeansecssvececectsctueensensercsrccecegecusnecenecte 41
3.4 노트북을 이용한 실습 진행 방법 vnneneen cece eceesccnesnecncesenecsecnsavenssncsnccnscnssnscnsnseanssesassncsnecnscoesnees 45

port 주식과 지수

Chapter 4  주식;  7 124,  지수

CAS) SYNE AS pw cow rocco no p:yececry nec 1 cobke cee LOL cea EXT EERE CECE eee 51
BLO WSO AVAL Ae ANT MDE poco corer eet tooo 51
MIVA TM 티빔리0때 마이07300006사00006 20000core eee 52
FICH ZO] AS CHET] CHSO! PAHT ELLA <eeecescseecsecceccnecsccsscccnscssccasccsscensccsecssesssecssessscssess 53
BRNO TEI acy 세는, 0700012100000911.0.040009000000 01000000700000070000사0 53

AF FE al Ol Petgd See ca CHAFOM eS scesecssNiscaseedersscescsntssascesssecccorscbersansasteraesesssrassnssensccasce 54

4.3 주가지수: 관심종목 그룹 전체를 대표하는 FIA Reveceescsecnesseesessnesnecsecsssesscsessecsssssteasssesscencane 56
주가지수의 종류: 종합지수, 대표지수, 섹터지수, 테마자수 등……………….……%%여아아 57
KIS AN BH: CEO ZEA BAI yg, AIT IESOH WPA soccceecseccsecsecssecsssccnscosscnscssscsscssncssscsnsscsessnesees 57
LON 7 FROM ED POs acne eateteaetetpestu ti veneatesesPestsssestnesrcsseticerassystssciprocccatectssscsioacsécsscassusveccses 58
KOSPIPA ISON KOSI OOOEK sec fescl esentistasus pbeeeytacaescdgeolere toarassastas, sbscacetteavectseccsoseate-« 59
ESIC AEH seers Ex SEAT OSO IPR entered ect aressecse aap csisacscotsnsragligesestsicnscsdssepiscassnsce 59
KOSPI2000| KOSP} 전체를 대변한다(파레토 법칙)………………………………아아다아아아아아에아아아아아아아아 60

1 저슨시이 서난디법트프사까때0100040304000000000000000000001200700000070770 00000 60
SSPEOO SSK OSPIOOOER EASE cal rl Peseereten tarovtarsusbanureessertonstecettescestrtsypstiactssnstosacsélscescs 60
SUSU EWR bray oramaica pry eriey ty “rn eecr err tes COEDPD SECRETS Eee 62
SRDS SAK OS PID OOK 50] lb earemreantesnsrcttostes cas ousthesasecseeheensdscy cas cceeedebsysGssesesesecs 64
R? ° 추세선의 품질000000000000000000900000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 65

12



===== PAGE 13 =====
Chapter 5 주식 엑셀 실습

Pe ee ee G3
6.3 S&P5002} KOGPI2009] 상판판계를 일이보는 희궤뽀석………………………………. 70
주네선 그래프.그리기 이 28
irra ene Fe ee by
anne Gig 81
잃지별 주가 elgg mene tee oo nee ee =
자시 heme fo ae IAN cai etaniee cilities chara ee eA
Sg i eee eee 86

Chapter 6 코딩 기술: 파이썬 기초

Go 함수…아아아아이이이시이 89
6.2 외부 모듈 Af eveereeseeeceseeeseesenenessssesetnessesenseassssssssnensesssetasserenecsensnssnensssenseassanssocessasassneess 91
6.3 빅데이터의 시작 뷰티플 수프 oeeeeecescesescscsscssesnsensnecsnsensenecenscsanscsscnscnersnsssanscsensensesssessesscess 93

Chapter 7 금융공학 모델링

7.1 S&P500 vs. KOSPIQOO H]iiless:-++s+esessesseesesesserensescenssanesssssessencassenseeserencenssasensenasncennserenss 99
네이버에서 KOSPI200 지수 SIS HTML 페이지 크롤링) …………아아아아아아사아아아자아아아애사아서 100
데이터 추출 기능을 함수로 만들기……………레나이이마시 자사시아새세이 이 sneer 113
네이버에서 해외 지수 4ERJSP (ISON 파일 크롤링)…‥…………아아아아아아아이아자아자자자자자자어사자 118
데이터프레임으로 여러 딕셔너리를 테이블 하나로 합치기|…………….…따여9아이이새서어 129

13


===== PAGE 14 =====
Le 라이 스기

Nam ay ee

CONTENTS

SOS (EE [Sr 3 Sob [ae ee eee one 134
CURRIE YS prs cccocecrs 00000 coos ys ESSER 00 137
SRO TEC OE Toa tees tee anes taycencneceretecescaceae vets ath 소00000.000000000000000000700 140
네이버에서 한국 10대 기업 데이터 수잡하기|……‥……………어이9이이이이이이이시이이기이기사시거이가사사 140
DR) AD SEY D prove traces eee 니시 5 OSE oe 148
자수 Abe ecseceeceseencecceceseesnnscnscsseseesescesensersnsesesecesccssssessensesssssncnesssasssesensssesssassessessseesers 152
US SA SAD boss asp comer mab eeton notre oD Coc oe 155
KOBE DOO [Fabs sore caccu cen repinn voces ononsypaeenend eric ere-cocan ¢Eoeno Yer eee eee 156
Chapter 8  선물의  개념

즈거금민{잇으면거래가러버리지!차은오모000이아여0이아아다사다이아이사이이이아이이아이아아아시 167
레버리지에.대한:안전장차; 알알정산과 마진를 ………………………………아다아아아아다아아이00아이아다 168
(그 써는 띠(카은차가 아미070007 0 110000500077071770000001070000070070000000007007000 169
VA 써는 ton A fool | tar cee aA aI Ces aseesaasSha te ccroonc sansa la asdssoceccgctansvensneracetacseaseeessereeses 170
예측이 맞는 경우: 상승장에 매수 포지션을 취한 경우………‥………….아이아아이이아아아아아아 171
예측과 다른 경우: 상승장에 매도 포지션을 취한 경우…………………….“%아아아아아아아 172
EUS Peat OMT eeetaa tase ataa carpe tace tan akan cacedet Jar cancrcanccksshisasescssusrspssrapsscsecseossesessocectessssoees 173
계산은 나중에: 이자 O]O]s--eeeenenecnssssnsenecsecnscnrensrncnecnvcssensssssaccuccesnssnecnscnssoscsssesssessssessessess 173
확보한 자산에 대한 권리는 아직 미보유: 배당은 못 받음………ㅇ“아이나 173
선물 이론가 계산: 이익과 손해를 반영 ………………아아999999999999999999이99099 173

14



===== PAGE 15 =====
8.6 선물 관련 용어Heer eeeeneanee aren setaneeeueeneeseeneeenessaeH eee sess ee ssesnaesss esses enuseseuesessteesunsesnesesssenssssenees 174

fe) 0.5 ol S Cece 174
베이시스 wossserreeeeeteeeeeeeeeeeeeesenneeeeeeeeeteeneeseseneetecscscecscaceesesesesseseesesaneseceeeretenseaceesceseesensens 175
롤오버999이이이이이이시시시시이이이0000이시시이시시시기기시기기시이이기이이이기이기시끼000000000000000000000000000090090000000000000000000000000000000000000ㄴ 175

Chapter 9 선물 엑셀 실습
9.1 K5 선물 이론가 ARSeee eee eee ene een eeeeee eee eee eens ee eens senses nesses ess seeesesesaseseeeesssetesseeseesseseesessenescesces 177
9.2 KOSPI200 선물 포지션 손익 Meee nee e eres eee nse reeseees senses essa ese Heeeeees sees EEeEseeeseE eS EESESsEseeeneeeseseseseees 182
9.3 마잔콜 발생 여부000000000000000000000000000000000000000000000ㄴ00000000000000400000000000000019909000000000000000000990000000 185

chapter 10 코딩 기술: 반복되는 데이터

10.1 .반복되는 데이터는 넘파이 EGE scnnesnsensecneconeenscsonensecnsconscndsoneesnsennssnsconessusesrsonsssnnctuseuaee 191
나으 Mie, 000130030030000100020000[202700000000 7700.90 카이 000 00000000 73006 6000 000 192
배열 모양 HZIS|T fp-enneeceeeceeecnscessccnsccnsccnnccnsccoscesnsseneconscenvsecnseesvosensssnesecnacsneennosesnuscensss 193
배열의 스칼라 연산………………………………아아아아 안이 어아소아이보온라자이에아인인이 194
바열의 벡터 LAL -n--cnscnscnssssecnscnecsnsconecsnecnccnesreconeconsenessnesoasonessussnascnnscnnsensseanengennstosss0ssc 196
행끼리, 열끼리 Ab eceveccnsccssccescrsscnnscenscsnsccnsccnsscencenecsnecsauesonaquascanecsnsscassenncesesseascenassess 196
배열에서 특정 데이터 HOLQI | -veeeeeescvsccnscnsccsccneccsccnsecnecsscsnccsusconscnsscnsenessnzequssnecenscnesensens198
10.2 데이터베이스 PRI BHCLA.--0s--cacceccsscnecosescosstnetsccuseversssnseoucoscunececsaseustuscuscsscasrnccrsancenses 199
사리즈여에아아에에에아아이에다에터아여더이이아이리런으이아어은이안이 리이아애이인 이 eaceeee ane aera 200
데이터프레임 AYAYsasaaseneeoeecnscosecessnscsnssayeacecnscnasevecousesscousenscousceuccusvesnenstnnsonsencteasenecostesse 204
데이터프래임'조회……%…아바앙데라새랭안은아안어러앤언룬이안애안언안연운오온애에선 로 eaten205
미아 [그토팍고 [파브리 (히[크스레 는00000202000000047.00000000. 7600.07 00000. 67700 6 207
데이터프레임 3 5 ge208
데이터프레임에서 데이터 빼기:…%…사에아아애이6이6아레애0만인사라인마어디아애연안 애러인신산인쟁이 211
데이터프레임 YOST [lig tes) <n cacesscescscnestscusstsceeasnee Omens destalesneentMMeteetecte feneeearaniemied213

15


===== PAGE 16 =====
=

~ -

eas ee 쑤

CONTENTS
Chapter 11 금융공학 mee)

SHE) OSE OT) STO] E> ona ne cee ena EO ER eo216

S29 YS DS [Ol Bay} orecomen comb semarecoy ease mo po Ree216

(SOIT To raves sites eu one LLnL eo CTE cb eo 218

보급형 DAIS 이용한 선물 이론가 Pb eeneeececeecceceecceceeneecesceeesceseesesceressescseesensnssesteaseeseecees 220

11.2 WTI 선물가격을 이용한 롤오버 비용 FifAbe--eseseceseeceeeeceseereccnsceesescseseeescasseeeeatsensestneeetaees 221

엑셀에서 WI 현물. 최근월물, 차근월물 데이터 읽어오기…………………………%아아아이222

CPUS QTE GL PSEIO © Bay poceeonecos ie cece OS erent ECO eee223

RUT MOET PRON EE He MONE MISES | cxerneeravenstestctecetcr cesta segs ctscesscatcsstyssussesscestesevenees 225

POTENT bal QUIN [SU Ge 풀때아0061000000710004070000007010000070001011002000000000000226

BOLT RAO @ [CE 2 ern um oie pe 227

Chapter 12 BM 거래의 개념

1 2.1  권리에 대한 계약×~000000000000000000000000000000000000000000000000000000000000000000000000000000000000000040060000000000233

12.2 SMO] FR --ece-neeeeeecceeeeeeeeccencecesscccscncececeesessssccnssscesnssersusensacersnessnsesssssencssscsssesseeseeneas 235

시간이 지나면 가능성은 사라진다: 시간가치| coeeseeeceeceeseeeetseteeneeesesseerceneessersescnrsesteassnsesseese 236

BT AWATMANGOLNART RAH P| Meceseeteritetssearescerensesttessorecccthasscscleschegenccucaccsceaseenscesceesenssesoess236

옵션의 가차: 내재가치 + 시간가치 -oneeneeeseeesessenrceccenceonercsnncncsncrenscersestensncsessescssscassessensess 236

12 3 변동성0600000000000000000000000000000000000000000000000000000000000000000900040000000000900000000000000040000000000000000000000 238
12.4 옵션의 특장: Svs. 풋-0000000000000000000000000000000000000000000000900000000000000000000000000000000600000000000000000004 239
옵션 매수 AIM eserseeeseescereessesececsssescesessrsesersersecsecnsessseasesessersersseneeseessessestossaeseeceasenseas 239

옵션 매도 포지션…………………아아이99999999909999이이이이이이이이이이이이이이이이이이00000000000000000000000000004 241
1 2.5  다양한 옵션 상품400600900000000000000000000000000000000900000000000000000000000000000004000406000000000000000600000000000 242

16


===== PAGE 17 =====
다양한 가격………아아아아아사아이이이9999이이어서242

매달 DED |nscasaccecenseasesseqeneaseutotucnectevoscccesacgstvcusey<sessasenuparived te vatraiite ayer aeataa aan an243
EL Woessesssesocsssesvsasccecsscescorespesvecensvavenssescrobeacenoa ¥scsael 1 d7ythtter titaeen ane nen aaa nna244
미국형 옵션 0 JAW SSM Seer a lasesecescecasnccseacetescovaru sevedsu=ozsuseseitevensveer=eaasenty atta seen maa244
12.6 옵션 이론가: 블랙-술즈 HEI) cece vsecesazeasascnenustsessussusescasoseysacapsetsitoarsitep essesse= =o meee245
12.7 옵션 그릭스: 어려워 보이는 옵션 용어…………………………-………0레애아어이 이이이246
멜타……어여애에아에예에아데에아아미테테테에어어태태게태시테이애”246
Zi pprecevsesseccoscsssccsesacchoutcsoctvoscdeeucsshessbeantee’ssecdhaceheteed Mints dette taste ttgiet 가스247
Pep Ss sesaecscsescescocscscscneatosousestectoucdensouteserevcasesndvasesrsectaunenaattcareeteset: 이거게이 eon248
Eff [oeceecsashececasusososcaccscveeesresevensncavercoseccsessatessusesceescucescacopsseareetet=esetts tet este eae249
Bi iapeovnesesiat sascsesssvenssceseanseaeqecesceuceostnaasecsccocseneerageesteapedtemnase tuosefe res aaa aCTee Tee249
Chapter 13 옵션 엑셀 실습
13.1 액셀로 구현하는 블랙-술즈 모형…………………-010…아이아아아아이이사안시이 이이 02000 250
AM Mat THON ees rc sececncatescesasasscvacedzoce as cetaagny ant thecte~cnctael ike zss<cacerocsnt nets ete250
옵션가격 구성요소 NE fevreceseseeeeseceecscsssceesccseescscsersscnsnssescssenscesenssnensneacesnssensnenessnesenges251
1222: 올읍션가격으래프크리기………………………00 af tcc ce256
13.3 그래프로 보는 멜타와 Zh fe-eeoseneenseosenvsenesnecnseucenseosenecnsecsecuesuecetechaqhsteususeuacesssachstescudueses263
SVC War) bei (la) a Speen ETT creer cen conic ue cra eceertnree ee268
1315 그래프로 보는 b] Seen EPR ETCH crores cette cen eaten tsa es 271

Chapter 14 코딩 기술: 시각화

14.1 그래프 그리기 끝판왕 HsRey...........Siievesileeaauesat Rape SORT a eae 274
OWES] 라이브러리 호출 및 노트북 사용 세팅…ㄴ아아274
그래프 그리기으에에다아아타에다아아아애데애아이랑라란레새래랜론앤이대어이인에래에새대언언안안안어앤인서연기애이세275
그래프 모양 ASAE] | ae oenencnnsccnccsscasucccsnstsaseeacasant sbacceeaanastnrccatcasal sexerssensstehreenatanneracaenees280

17


===== PAGE 18 =====
me mp

CONTENTS
제목, ZS 이름. 범례 삽입…ㄴ99999 282
여러 개의 그래프를 모아서 HOPS |e-evesesecseeesesecesececseesseneeenesesecessenesecnsncsccusncsesssneneesecsess 287
14.2 CBRERREI TD} 팬더스의 ORf----n---ceeeceneseencnenevensseenensucncnsssseensnsncnececessencsusscocscenssnencesneseasenees 289
POF TM KET 7 | teaesaceec rhecoyenesvezsuccssnecyssesaseyostestauatsns ieveqesedeseueseslscciecosereresccarsesterecers 290
데이터의 분포를 나타내는 히스토그램…………… 이아 293
영역형 그래프………/304.9은0769.729079290000530110010000802 00700 02070 아차산 다사아주 아아사 293
통계치를 그래프와 함께 보여줄 때는 박스 그래프‥………‥…ㅇ“아아295
관계를 표시할 때는 APSA anne nceccnnnseneceaecsenovevossasssacnesnesenssarsecosasnsopnessencssencacoeasscsesacorsssoee 296
SSD ate IF eee vcen senor csenencnnsnsacsntacvasnovssessncncecssvnecscnceusesnrnenvsasacncacsesncosnesssavacseessatiee 297

Chapter 15 금융공학 모델링

45.1 WOPHOR 구련하는 블랙-술즈 BY ness escseceensenccnerecnensensenscussncnccnscassucsessucnecnersecsesecsesse 301
NO oN Gd erecta cr aecennas cnn asec ts cavessexactsenrntoinsoasseeiacartessccescssesestsenesoseoesnes 301
PbeSea 7 | PUA eae esa ed cme esesaseces cheser esse vefivicscbatutaraccavasasssarbacranstarerststeascacuacsecereneceksuse: 302
BEAH BX BPYANS O/RSE BSMI}Z§ FST] cneneenenececevenesscencnssnssncsassecsscncssccecscsesncenesesees 303
기초자산 및 행사가격.변화에 따른 몰읍션가격 변화…ㅇ………………………………=……………~…9909999999090099304

(BAT OWES GSA bee pee eae tie Ue OEE ee oe 306
INDE | SUG] SS | ST etre ore ey preteen repens TeOreOtY EEE EE eee 306
Fa ey Pod LOMA Mirage cchcecna tact cnesdedecuosnsnscedealobibsocsessspetatsessishicscdseasars<sse~sstscssseoveresoavesess 308
SEUSS | S| SE frre to vrei rece ERO POOLEY SOP ee ee 312

TBS} SHE STIVS ST SRY beacon recent ts Crete oor OEE PPTL eee314
TYEE SS Bee +n emo yrrcrro 0 areas Stee CO TEED TET eo314
견지 그르 SL aU aaa are Soca ane Nese CATE Ltbicesotcsacestascsccusseecuscecsactreccacsts;envecsaccesceses 315
STEEL SBE SE Bhs cs nine crercorreonr icetebtet te ei Per POL 317
EE DAN SET ER os vireny Getrerccrse cane rr eres rr POET 기거1어이가0 319

18


===== PAGE 19 =====
pat 펀드와 구조화 상품

chapter 16 펀드와 구조화 상품 개념과 설계

16. 7 구조화상품…………………에애가에익어마지”325
16:2.구조화 상품 BOY ssscsectowsonssssczaocenescntos,tacyncnqsyerumesteaantenak sul ncaa Jeanine emt mean326
액티브 ys 패시브 «seaside -svesncesctsnndsonscusnnasconcenterasseabitelOPecotuatcoiicane aetna tea326
알파 vs. 베타

Chapter 17 펀드 엑셀 실습
17.1 K5 펀드 구조화Renee eee n eee eeeeeeseeeeeeeneeeeseeeneeeeeseeeeeeseeeeeenneeseeeseneaeneanssansnnaaeeesnantnnanssanenassnee333
17.2 K5 Hc 운용 eee eeeeeneneeeeneeeeeseceueneeeeeesenseesesesusesesseuseneeseesessnssenssassessnssaessesesssasssessaseseneees336

chapter 18 코딩 기술: 데이터 수집 및 가공

19


===== PAGE 20 =====
해

CONTENTS

문자열의 시작을 검사하는 match veereesesesesseeeeseesesesessneeneeneeneneeeneereneensenennsenennesnesneensenseess
문자열 내에 패턴이 있는자를 검사하는 96870 …'…'아이아아아어사아재사사사사새사사사어
모두 다 찾으려면 fia] ---e-eeeeeeeeeeseeeeneeeseeseeteseseeeeseeenenenesnsneenesssnsevensnseneeseecanenennensaneness
문자열을 분해하는 621…………애여저아아아아이지아아이지이이이이이이이이이이아사사사사사사사사사
여러 음절 중 원하는 패턴이 들어 있는 음절 찾기
특정 문자를 바꿔주는 sub voesesseceeseseesesseeesesecsssnececeneeenntenssssncenenseescnscnscnsansnscnecnceneenseneess
패턴 정의하기……………………이이이아아아이아아어아아아 서요 00000 00000
18.2 데이터 BaAlfeseeoeseseceeeneseseneceeeseeeseensessnensscsenensecarecensnsncssnsnsesessessesenensassssesncaresssresnensesecs
18.3 핸드폰 번호 검색 n-ne esececececeseseseseeesrsnsseresssenescssesnssssnsnssssssneesscecansesssssossesesasssscessnseeneess
18.4 간편식을 이용한 패턴 정의…ㄴ이

Chapter 19 금융공학 모델링

(Os) GEG 더 LEGA Sho otter se reuse yee n oro creer 00000 이00000

PaReSO) UD QI D Peahesscezercntscrsssrdsscnscsesecnsssneccrsecoveconsennscensatasercasgenccernsvossecnascsnsscssecsnnee rss
19.2 K10 HE 구성을 위한 사전 준비
아어 COs 2H gl cae sm eetren er statecssececuthesfracnscteernecracerescasscasendscnecoeQareccoasensecasenuscnscsnsse

AAG) ah WSs coe ro 아아 아지게에어 385
Raueay Vo 기이 에 기어이 에이 이 500
NO SEBEL} ro cnn ee 이0 301
OCI) oo coer oii ese 개기거 395
PAGER Roe ee eect dal te emi ee on



===== PAGE 21 =====
Tl

PA

5
의



===== PAGE 22 =====
시간가치

돈의

r2

A”

re
weal

|

Chapter 3



===== PAGE 23 =====
금융의 발전은 금융상품의 진화를 이끌었고, 금융상품 진화의 중심에는 금융공학이 있었습니
다. 금융공학에 들어가기 전에 은행, 보험 등 전통 금융상품부터 구조화 상품까지 금융상품 전
반의 특징을 살펴보도록 하겠습니다.

1.1 금융상품의 진화

0
=
&
flo
iu
N
in
x
00
의
Sh»
oN
k
,
110

Ni

= eG,
4x
구내
i
ue
Aw.
lr
ㅁ
(10
ott
bal
00
jo
a
때
is
a
비

=
ㄴㄴ

ox:

은행에서 학자금대출, 주택자금대출 등 ES 빌리면 개인에게는 초기에 큰 SAAS 현금
흐름이 발생하고, 약정한 기간 동안 지속적으로 작은 마이너스(-) 현금흐름이 발생합니다. 반
면 은행에는 초기에 큰 마이너스가 발생하고 이후에 지속적인 플러스가 발생하게 되지요. 그
은행의 대출상품은 누가 만들까요? 당연히 은행입니다. 개인은 여러 금융기관이 만들어놓
은 대출상품 중에서 선택을 할 뿐이지요. 은행은 향후 이자율이 어떻게 변할지, 다른 금융기관
은 이자율을 어느 수준으로 결정할지, 은행의 현재 현금흐름은 어떻게 되는지 SS 고려해서
은행에 이익이 되면서도 다른 금융기관과 비교해 경쟁력 있는 대출상품을 설계합니다.

of


===== PAGE 24 =====
보험

보혐은 Bro 지속적인 마이너스 현금흐름을 발생시키지만, wes] 경우에 큰 플러스 현금
흐름이 발생하는 금융상품입니다. 보험 nee 설계하는 사람을 계리사라고 하는데, 계리사는
이자율 변화, 보험사 투자 포트폴리오 변화와 더불어 손해율(보험이 지급될 확률)을 함께 고려
해 보험상품을 설계합니다. 생명보험을 판매하는 보험설계사는 항상 내년이 되면 보험금이 올
라갈 테니 빨리 가입하라고 하지요? 이는 비단 상술이 아니라 실제로 그렇습니다. 평균수명이
늘어나면서 병원비를 지불해야 할 상황이 더 많이 생기니 손해율이 높아져서 그런 것이지요.

주식

그럼 주식은 어떨까요? 주식은 은행 대출이나 보험과 같은 고정된 현금흐름에 대한 약속이 없
습니다. 주식은 빌리거나 가입하는 것이 아니라 사서 소유하는 것입니다. 주식을 산다는 것은
그 기업을 산다는 것과 같은 뜻입니다. 내가 산 주식을 발행한 기업이 성장하면 내 주식의 가
격도 올라가고. 쇠퇴하면 주식가격도 하락하게 됩니다. 그럼 주식의 가격은 누가 정할까요?
대출은 은행이, 보협은 보험사가 정하지만 주식가격은 증권사가 정하지 않습니다. 주식가격
은 다수의 투자자, 즉 시장이 결정합니다. 주가가 올라갈 것이라고 예상하는 사람은 주식을 사
고, 반대로 주가가 떨어질 것이라고 생각하는 사람은 주식을 팔지요. 더 많은 사람이 배팅하는
방향으로 주가는 움직이게 됩니다.

그래서 주식시장의 투자자는 은행 같은 전통 금융시장 소비자보다 더 어려워졌습니다. 전통
금융시장 소비자는 정해진 틀 안에서만 움직여야 했으므로 많은 고민이 필요하지 않았습니다.
내가 정해진 이자를 부담할 능력이 되는지만 판단하면 대출을 받을지를 결정할 수 있었습니
다. 하지만 주석시장의 소비자인 Salat 두자하려는 기업이 앞으로 AAP, 다른 투자자
들은 어떻게 움직일지, 주식 투자의 수익률이 은행 예금의 수익률보다 높을지 등을 모두 고려
하야 합니다.

반대로 주식시장에서 공급자와 비슷한 역할을 하는 증권사는 어떨까요? 가격을 결정할 권한
이 없으니 그냥 주식 매매 수수료만 받으면서 앉아 있을까요? 예전에는 그랬습니다. 더 많은
기업을 상장시키고 투자자들이 더 많이 주식을 사고팔게 하면서 늘어나는 수수료 수입으로 증
권사가 커나갔죠. 하지만 증권사 간 경쟁이 심화되면서 수수료는 점점 내려가고, 심지어 '계좌
개설하면 평생 수수료 무료'라고 광고하는 증권사도 출현하는 등 수수료에서 나오는 수입은

24  1부 준비하기


===== PAGE 25 =====
점점 줄어들고 있습니다. 이제 증권사는 더 많은 고민을 하지 않을 수 없습니다.

증권업계의 고민은 새로운 금융상품을 만들었습니다. 수수료가 늘어날 수 있도록 투자 자금이
부족한 투자자에게는 자기 자본 이상의 AAS 할 수 있도록 마진거래를 제공합니다. 은행이
ES 빌려주는 대출 ANAS 제공하듯, 증권사는 주식을 빌려주는 대차 서비스를 만들어 공
ut (short selling)'S 할 수 있게 했습니다.

파생상품

돈에 대한 열망과 창의력의 결합은 파생상품을 만들었습니다. 선물, 옵션으로 미래 가치를 가
지고 거래를 시작한 것입니다. 현재의 기업 가치도 서로 다르게 판단하며 거래하는 상황에
서 미래의 기업 가치를 판단하는 일은 얼마나 어려울까요? 그래서 선물, 옵션의 밸류에이션
(valuation), 즉 가치 산정 방법을 두고 많은 연구가 시작됐습니다. 특히 옵션은 매 순간 가치
가 달라지고 고려할 요소가 많아 여러 밸류에이션 모델이 나왔습니다. 여러 모델 중 가장 사용
하기 편리하고 대중적인 모델이 그 유명한 블랙-숄즈 BA (Black-Scholes model) YUtt,

블랙-숄즈 모형의 출현으로 옵션 밸류에이션이 대중화됐고, 이제 사람들은 더 많은 것을 원
하게 되었습니다. 선물, 옵션을 이용해 HBS 헤지[16086)^하는 YAS 생각해냈을 뿐 아니
라, 더 큰 레버리지(16467286ㅇ)”를 일으키는 방법까지 깨달았습니다. 한 걸음 더 나아가 주식,
선물, SAS 섞어 자신이 필요한 수익률을 안정적으로 달성하는 WHS 고안해냈습니다. yt
야흐로 금융업계에 금융공학이라는 새로운 Hop} 출현하게 된 것입니다. 이제 금융업계는 금
융공학자, 즉 BE (quant)S 채용하기 시작합니다.

구조화 상품
금융공하은 주식, 선물, SAS 넘나들며 다양한 금융상품을 만들기 시작했습니다. 주식, 선
물, 옵션 등 여러 금융상품을 섞어서 만든 새로운 금융상품을 구조화 상품이라고 합니다. 구조

1 주식을 보유하고 있지 않지만 빌려서 파는 거래. 주가 하락을 예상할 때 실행합니다. 가격이 높을 때 증권사에서 SAS 빌려서 시장에 내다
팔고, 가격이 낮아지면 시장에서 FAS 사서 증권사에 주식을 갖는 방법으로 차익을 실현합니다.

2 가격 하락 등으로 발생할 위험을 방어하는 거래를 말합니다. 주식 1억 원어치를 매수한 투자자가 주가 하락 시 발생할 손실을 방어하기 위
해 같은 가격에 선물 1억 원어치를 매도하는 것을 예로 들 수 있습니다. 물론 위험이 없어지는 만큼 수익의 기회도 같이 사라집니다.

3 고수익을 위해 자산 규모 이상의 거래를 하는 것을 말합니다. 대출을 받아 아파트를 사는 거래, 증거금만 납입하고 10배 이상 규모의 파생
상품을 매매하는 거래 등을 예로 들 수 있습니다.

1장 금융공학이란? 25


===== PAGE 26 =====
화 AS 원래 특정한 수익률을 확보하려고 하는 기업 고객을 위해 출시되었지요. 2008년에
유명했던 키코(61ㅇ)*가 대표적인 예인데, 수출입을 많이 하는 기업 고객의 환위험을 헤지
하기 위해 만든 상품입니다.

키코는 좋은 목적으로 설계된 상품이라 WARE 구간 내에서는 원하는 현금흐름을 달성하
지만 파생상품이기 때문에 특정 YAS 벗어나면 큰 위험에 노출됩니다. 예를 들어 BHO]
1000~1200원 사이에서 움직이는 경우 환율을 1100원으로 고정해 수출입 기업의 기대 수
익률을 안정되게 할 수 있지만, 1200원 초과(0ㅁ0아-10) 또는 1000원 미만(ㅁ0이-040)인
경우에는 오히려 손해를 보는 구조를 갖습니다. 키코 사태 발생 이전에는 오랜 기간 환율이
1000~1200원 구간 내에서 움직여왔기 때문에 많은 기업이 안심하고 키코에 가입했지요. 하
지만 미국발 금융 위기가 촉발한 환율 SSS 키코 가입자에게 큰 EAS 초래하고 말았습니
다.

21세기 들어 구조화 ASS 중국, 인도, 베트남 등 해외 HES 수익률 급등에 힘입어 개인 고
객에게도 급격히 퍼져나가기 시작합니다. 초창기 펀드는 높은 수수료를 내고 펀드매니저에게
돈을 맡기면 펀드매니저가 개인 역량에 따라 운용하는 형태가 많았습니다. 하지만 펀드매니
저의 역량에 의존하는 기존 펀드보다 특정 인덱스를 지정해 유사한 수익률을 보장하는 형태인
인덱스 펀드의 수익률이 더 좋다는 기사가 언론에 자주 노출되며 인덱스 WES] 인기가 점점
높아집니다. 또한 인덱스 펀드는 기존 펀드보다 수수료가 훨씬 저렴해 장기 투자자에게 메리
트가 더 AAIB. 여기에 거래소는 자산운용사와 손잡고 주식처럼 간편하게 거래할 수 있으면
서도 수수료는 훨씬 저렴한 상장지수 펀드(81,. exchange-traded [400 )를 만듭니다. 바야
흐로 모든 사람을 위한 구조화 상품 시대가 시작된 것입니다.

구조화 상품 시장의 성장으로 금융업계는 더 많은 퀸트가 필요해졌습니다. 이전에는 증권사와
자산운용사로 대표되는 금융투자회사가 BES] 주 수요층이었습니다. 하지만 파생상품과 구
조화 상품을 이용해 자산을 굴리는 운용 YH] 인기를 더해가며 은행, 보험과 같은 전통 금융
업계도 금융공학자가 필요하게 됩니다.

4 knock-in, 14700<-0011의 약자로, 환율이 일정 구간 내에서 변동하면 미리 약정한 환율을 보장하는 금융상품. 반면, 구간 밖으로 나가면
더 큰 손실이 발생합니다.

26  1부 준비하기


===== PAGE 27 =====
1 .2 금융공학 = 금융 + 모델링
검색엔진에서 금융공학을 찾아보면 ^수학을 이용해 금융시장을 분석하는 학문이라고 정의하
는 것을 볼 수 있습니다. 한 예는 다음과 같습니다.

8-34 (financial engineering): 수학적 방법론을 이용해 금융시장을 분석하거나 투자처
를 결정하는 학문 분야로 HE(finance) 7} Se(engineering)2] 합성어이다. 각종 경제 ㆍ

금융 데이터를 SASS 이용해 가공하고, 여기에 근거해서 어디에 투자할지 결정한다. |
정교한 수학적 방법론을 이용해 새로운 금융상품을 만들거나 컴퓨터 프로그램으로 작성해
미래를 예측하기도 한다. (경제용어사전, 한경닷컴)

금융시장에는 엄청나게 많은 데이터가 있습니다. 주가, 이자율, 성장률, 배당, 인플레이션 등
일일이 나열하기 어려운 수준이지요. 이렇게 많은 데이터를 분석하려면 컴퓨터를 이용할 수밖
에 없겠지요? 그래서 금융공학자는 컴퓨터를 잘 다뤄야 합니다. 금융공학의 본질에 컴퓨터가
들어 있지는 않지만, 금융공학이라는 단어를 들으면 컴퓨터가 떠오르는 이유가 이 때문입니다.

|

it

금융공학은 데이터 분석에서 끝나지 않습니다. 상품을 설계하고, HAS 측정하고, 투자
을 결정하는 등 데이터 BAS 통해 필요한 솔루션을 찾아야 합니다. 금융공학이 제시한
AS 다른 사람들이 이해하고 활용할 수 있어야 하므로 일반인이 이해하기 쉬운 형태로 만
어야 합니다. 즉, 모델링을 해서 제공해야 한다는 뜻이지요. 그래서 금융공학자는 프로그래
을 해서 모델을 만듭니다.

is}
he 때

of

1.3 금융공학자 ~ IT 전문가

금융공학자는 IT 전문가와는 다릅니다. IT 전문가가 생산자라면 금융공학자는 설계자입니다.
금융공학자는 데이터 BAS 통해 SHAS 찾고 모델을 만듭니다. 금융공학자는 필요한 데이
터가 무엇인지, 그 데이터를 어디에서 구하는지, 어떻게 분석하는지 알아야 합니다. 또한 데
이터 BAS 위한 방법을 숙지하고 프로그래밍을 통해 모델을 구현할 수 있어야 합니다. 금융
공학자에게는 뛰어난 프로그래밍 기술이 요구되지 않습니다. 필요한 모델을 정확히 구현할 수
만 있으면 됩니다. 그 이후 과정은 1 전문가에게 맡기면 되지요.

IT 전문가는 금융공학자가 제시한 모델을 상용 시스템으로 생산해내는 역할을 합니다. iT 전

1장 금융공학이란? 27


===== PAGE 28 =====
문가의 관심사는 모델을 만드는 것이 아니라 제공된 모델을 얼마나 효율적인 시스템으로 구현
해내느냐에 있습니다. 그래서 IT 전문가는 어떤 기술이 더 높은 성능을 발휘하는지, 해킹으로
부터 안전한지, 유지 보수가 수월한지, 비용 대비 효율적인지 등을 알아야 합니다. 17 전문가
는 금융공학자가 관심 갖지 않는 하드웨어, 네트워크, 데이터베이스, 보안 등의 영역을 담당
합니다. 조금 더 뛰어난 17 전문가라면 금융공학자가 만는 모델을 튜닝해 성능을 개선할 수 있
겠지요.

28  1부 준비하기



===== PAGE 29 =====
돈의 시간가지

금융공학을 공부하기 위해 많은 선수 지식이 필요하지는 않지만 꼭 알아야 하는 개념이 있습
니다. 바로 돈의 시간가치(02076 value of 2ㅁ0ㅁ6)입니다. 10년 전의 1억 원, 현재의 1억 원,
10년 후의 1억 원은 다 가치가 다르지요. 이렇게 시간에 따라 돈의 가치가 달라지는 것을 돈의
시간가치라고 합니다.

현재가치는 PV (present value), 미래가치는 FV (future 3146)라고 합니다. 과거의 가치는
큰 의미가 없어 별도의 용어가 없네요. 금융 활동은 HS 빌려주고 돌려받는(또는 빌리고 갖는

일련의 행위가 포함되며, 이 과정에서 이자를 매개로 한 돈의 시간가치가 고려되어야 합니다.

2.1 미래가치[『\/] 계산

은행 상품을 예시로 보겠습니다. 1년 만
기 AFL] 이자율이 10%라고 하면, 지
a 10000원을 예금에 넣으면 1년 후에
11000원을 돌려받습니다. 현금흐름.
나타내면 지금 대비 -10000원, 1년 후
+11000원이 됩니다. 이 예금상품의 현
금흐름을 그려보면 다음과 같습니다.

11000

현재

ft
rh
4h

—10000

2S 돈의 시간가치 29


===== PAGE 30 =====
그러면 1년 후 받게 될 돈은 어떻게 계산할까요? 1년 후에는 저축한 원금에 이자를 덧붙여 받
게 됩니다. 원금은 10000원이고. 이자는 10000>×%10%인 1000원이니 SS 합해서 11000원을
받습니다. 수식으로 나타내면 10000×(1+0.1). 즉 미래가치=현재가치×(1+이자율)입니다.

2.2 현재가치[[『'\/] 계산

그러면 반대로 1년 후에 10000원을 받                             10000

으려면 지금 얼마를 예금에 넣어야 할까                     —
2? 미래가치를 구하는 것과 반대로 계              현재

산을 하면 되겠지요. 미래가치를 구할 때        :        로   =         1년 후

는 현재가치에 (1+이자율)을 꼽해주었           |          :
으니, 현재가치를 구할 때는 (1+이자            -9091
율)로 나뉘줍니다. 수식으로 나타내면

Ba7l= Geek 입니다. 1년 후에 10000원을 받으려면 지금 9091원을 저축해야 하는
것이지요.

2.3 금융공학과 돈의 시간가치

금융상품 밸류에이션의 기본 컨셉은 돈의 시간가치를 인정하는 것부터 시작합니다. 선물, 옵
A, 구조화 상품 등 다양한 금융상품의 밸류에이션은 금융상품을 `지금 사서 미래까지 보유하
는 AB '미래에 사기로 약속하고 그동안 현금으로 이자소득을 얻는 것이 동일한 가치를 갖는

는 전제하에 시작합니다.

30  1부 준비하기


===== PAGE 31 =====
파이썬 설치

3.1 아타콘다로 한 방에 끝내기

파이썬을 설치할 시간이 왔습니다. 사실 파이썬 언어 설치부터 125 설치, 코딩에 필요한 라이
브러리 설치 등 고려할 것이 많습니다. 하지만 이 모든 DAS 한 방에 해결해주는 패키지가
있는데, 바로 아나콘다(40200002)입니다. 아나콘다는 파이썬 개발을 위한 통합적인 환경을
무료로 제공합니다.

아나콘다 공식 웹사이트 다운로드 페이지인 https: //www. anaconda. com/download/ 에
접속합니다. 어떤 HAS 설치할지를 결정해야 합니다. 현재는 = 버전인 2.*와 신 버전인 3.×
가 공존하고 있으나, 대부분 3.x7} 대세가 될 것이라고 얘기하고 있습니다. 이 책에서는 집필

시점인 2018년 5월 기준으로 가장 최신 버전인 3.6을 사용하겠습니다. 다음은 다운로드 페이
지의 화면입니다.

3장 파이썬 설치 _ 31


===== PAGE 32 =====
(대여 채에대 ㅋ 1

€  CB TE bron wee seconde com sommes     :                                           ㅎ 6

Download Anaconda Distribution

Version 5.0.11 5

Download For + | G ^

High Performance Distrbuton                         Package Management                              Portal to Deta Science
Eesty rated 1000+ Gola science               Manage packages. dependencies               Uncover insights in your dota ond
polos                                  8nd exrvronments with Conda                    Create interective visualizations

Gl wrsom   @ maxcos   4S unn                                    |

그런데 3.6 HAS 받으려고 스크롤을 내려보니 다시 운영체제가 64비트인지 32비트인지에
따라 다른 설치 파일을 다운로드해야 하네요. 내 운영체제가 둘 중 어떤 것인지 확인해서 적합
한 버전을 골라 다운로드합니다.

¢
O cores ewe
Anaconds Gout  Documernstor    Contact    7
O ANACONDA.                     What Anaconda? Predicts Sippot Communty About Reouces SM
Biwinters GG racos | tenn

Anaconda 5.0.1 For Windows Installer

Python 3.6 version "                Python 2.7 version ~

은 0000
서거 Gmme rote OS 벅고                            (4.08 Comes renaier 200 MR
22.08 Gates rome 16 보그                                        2m Gans rete tM

때기 오데
게재 te oat Python 고우 의 coher Python vermoes
tie to instal ANACONDA

Get Started
BB
의
시                                pee to Ute 스어 ose Meawigetor                 Pech ages 레시 개 In Anaconce

32 14 준비하기


===== PAGE 33 =====
운영체제 64비트/32비트 확인

윈도우 10 사용자는 자신의 운영체제가 64비트인지 32비트인지 다음과 같이 확인할 수 있

습니다.

OD UEP) 키를 누르면 나타나는 시작 메뉴 중 설정 아이콘을 클릭합니다.

Chrome

Conexant

Drive File Stream

Groove 음악

INC Ainternst

9 &

@ Windows AA 화면에서 시스템 아이콘을 클릭합니다.

=       Sse   =   $$$

EE   기

므 | & @ «A

천한        네트회그 Reus       ve  ¥
22     Pree  .     vance

: =                       의                       “후                       ®                       (7                          |

AN         시간 월 OO         AB          Sew
Mk S7m 오      8   wh     vi   WR MEL    게이터 Bw?          |
e                     S160                      |

NG 정보         cas 될 보안           a4

3장 파이썬 설치


===== PAGE 34 =====
os                                 정보
[exer                            =] Pc7t 모니터핑되고 보호됩니다.                                               pee or
© mois BA 영지

ae

as@                  © sma 잇 네트워크 vo
Windows # 보다    수위
= 디스플레이               © 디바이스 성능 잇 상대                            ~
'                                      © 연 및 브라우저 nse                          피드백 보내기
i                 O wexae
[                                        Windows 내에 에서 AY 저번 암조
;                 O 전은외졸전
ㅁ 베터리
디바이스 사양
ns Kad             디바이스 OB Gam
프로세서    intel) <여0139 17-6500 CPU @ 2. S0GH:
@ auxec                     pase
o 504g              SNE RAM  0008 (7 87GB usable)

a 00000

So Kane 포시
NAG Se    SEES EE SEE Peo

:                             x 6603                             :          디즈
t 5                                                                                 uot feuc.
|         ie hod    ^, (arcs oie 47 |
O ue                      |

：

|                                                                               Windows 사양
에디션        Vandows 10 Pro
버전          1709
OSes           16208.192

AB 키 변경 또는 Wado ME 업그레이드
서비스에 적8 다는 Miccosoh 서비스 AG 위기

) 주아어  나타나는
6 0”

다운이 완료되면 브라우저 상태표시줄 등에서 다운로드한 파일을 클릭하거나 탐색기를 열어
다운로드 폴더에 저장된 설치 파일을 더블클릭해서 설치를 시작합니다. Next YES 눌러서
설치를 시작합니다. 다음 그림처럼 사용권 동의 화면이 나오면 149166 버튼을 누릅니다.

34  1부 준비하기



===== PAGE 35 =====
O Anaconda3 5.0.1 (64-bit) Setup                              =              x

License Agreemert
ANACONDA        freee the license terms before installing Anaconda3 5.0.1

Press Page Down to see the rest of the agreement.

See ee Se SSE ES Se                                 ^

[Anaconda End User License Agreement

Copyright 2015, Anaconda, Inc.
‘All rights reserved under the 3-dause BSD License:

Redistribution and use in source and binary forms, with or without modification, are
permitted provided that the following conditions are met:

If you accept the terms of the agreement, dick I Agree to continue. You must accept the
agreement to install Anaconda3 5.0. 1 (64-bit).

Anaconda, Inc

| <Back | 1498 ] | cancel |

사용자 범위 설정을 위해 '너만 쓸래, 같이 쓸래?를 물어보는 화면이 나옵니다. 공용 pcs 관
리하는 관리자가 아닌 이상 권장 사항대로 Just 516'를 선택하고 (Next) 버튼을 누릅니다.

‘> Anaconda3 5.0.1 (64-bit) Setup                             -             x

Select Installation Type

ANACONDA    Please select the type of installation you would like to perform for
Anaconda3 5.0.1 (64-bit).

Install for:

@pust Me (recommended)|
OA Users (requires admin privieges)

Anaconda, Inc.

다음은 설치 SS 결정하는 단계입니다. 어느 폴더에 설치하든 실질적인 영향은 없습니다.

으

여기에서는 기본값 위치대로 (:\056「5\사용자명\&03000033에 설치하겠습니다. 사용자명은

3장 파이썬 설치 _ 35


===== PAGE 36 =====
|                 각자의 환경에 따라 다른데 한글일 경우 오류가 날 수 있습니다. 경로에 한글이 있다면 다른
경로를 지정하는 게 좋습니다. BES 지정한 다음 Next 버튼을 클릭합니다.

O Anaconda3 5.0.1 (64-bit) Setup                               =              x

Choose Install Location
0) ANACONDA Choose the folder in which to install Anaconda3 5.0.1 (642).

Bee ea ee ee OL Det Hl 데토 To instal in a different
folder, dick Browse and select another folder. Chck Next to continue.

Space requred: 2.468
Space avaiable: 70.6G5

Araconss, Ine

__< Beck [net >] cancel |

시스템 환경변수에 ee 실지 폴더를 주가할지 여부와 아나콘다를 파이썬 코덩용 기본
IDES 사용할지 여부를 선택하는 화면이 나옵니다. 아무것도 변경하지 않고 Install HSS
클릭하면 본격적으로 say 시작됩니다.

xia

O Anaconda3 5.0.1 (64-bit) Setup                                =              x
Advanced installation Options
®) ANACONDA a        how       da integrates with Wind:

                    Advanced Optons

(Add Anaconda to my PATH environment variable

Not recommended. Instead, open Anaconda with the Windows Start
menu and select “Anaconda (6400. This “add to PATH” option makes
00650 Breton) ean = software, but may

9 you to uns

iRegster Anaconda as my defauit Python 3.6

This wil allow other programs, such as Python Tools for Vieual Studio

Arcenysheedens Masel and MSI binary packages, to automatcaly
detect Anaconda as the primary Python 3.6 on the system.

Anaconda, Inc

 <66 [rst] cance

36  1부 준비하기



===== PAGE 37 =====
설치 완료까지 시간이 꽤 소요됩니다. 설치가 완료되고 Next HES 누르면 설치 종료 화면
이 나옵니다. 체크 YAS 모두 해제하고 Finish HES 눌러 설치를 종료합니다.

O Anaconda3 5.0.1 (64-bit) Setup                            =

Thanks for installing Anaconda3!

©)          Anaconda is the most popular Python data scence platform.
ANACONDA       bat hee Soca rere packages, projects and environments

[] 6300 more about Anaconda Cloud

eS] 0

설치가 종료된 후 윈도우 시작 메뉴를 보면 아나콘다가 설치된 것을 확인할 + 있습니다. 드디

어 파이썬 코딩 환경 구성이 끝났습니다.

을  Anaconda3 (64-bit)
Anaconda Navigator
Anaconda Prompt
Jupyter Notebook

Reset Spyder Settings

Spyder

3장 파이썬 설치 _ 37


===== PAGE 38 =====
3.2 주피터 노트북으로 파이썬 명령 실행

파이썬 명령에 즉각 반응하는 주피터 LES (upyter Notebook) 이용해보겠습니다. 윈도
우 시작 메뉴에서 “Anaconda %4\18310ㅠ를 클릭해서 아나콘다 내비게이터를 실행합니다. 첫
실행 시에는 다소 시간이 걸립니다. 환영 화면이 뜨면 건너됩니다. 내비게이터에는 다음과 |
이 7개의 블록이 있는데(버전에 따라 개수는 다를 수 있습니다), 우리는 붉은색으로 표시된 주피터
노트북을 사용할 것입니다.

O 서에애차                                                              -  ㅁ  ×
oe
oO ANACONDA NAVIGATOR                                                                                                       E===
bad              on rect       … Cannes                                 Petrewr
|  기                      호               ?               [그              [그
ㆍ
7                                y                               Lf
2                                 —
Brew            ©            어떠             ~
i Prajects (eta)                                        ~—                      _                     bo]
a We          jupytertad:         08         “04000         spyder
전 나네             ㅎㅇ              seo              ant              ane
그     ~                     PrQt Our 대이 bupperts nine 1녕예이이.    nen tlc PYUNen Develogment
7  (         어부 repeat Bie (OMG D teed On Oe  notebook emirenment. Lt end rem   proper matting    totes          U   Ot with
SR Commurty       태지 betebeot and Architecture.  mam readable Cock while Geicrbing the | Nighighting, graphical caltigs, and more.  advanced editing, interactive testing,
Gata anatcis,                                                                                             Gebvaging ond introupection features
—                  —;                  a                  ;    =
호               [그               ?
geet            ceanged             nitude
owe              aan              100
때                           Gata mining framework. A set of tegrated tools Cerigned to hee
Hes Copere (ee tenateps 메 다예 ane   이네 rinualzation and dats anaitls for  you be more productive with  inchates 19
데어 Bing        among related 이내에    novice and expert Interacthe wortflows    이네 and notebooks
with 0 urge toca
treme
ey             [=]            [=
|
yess?

ㅣ 노트북 블록에 있는 Launch) HES 클릭해 주피터 노트북

후
으으           ㅣ 을 실행합니다. 노트북을 실행하면 웹 브라우저가 열리며 다
~               ㅣ Sa} 같은 화면이 나옵니다.
notebook            ：

5.0.0
Web-based, interactive computing        '
notebook environment. Editandrun
human-readable docs while describing the |
data analysis.

!
|
|

38  1부 준비하기


===== PAGE 39 =====
/ S Home           x\   ‘
S | O tocathose.0282/100

jupyter

© Favertes
O 어리
© 6
DB © OneDrive - Univernity of California - irvine
DO © 에
GO Saved Games
© O Searches

UO CO Videos

13 days ago
13 days a90
13 days a90

13 days 009
13 07300
13 days 090
13 days 290

초기 화면에는 사용자 폴더(:\056「5\사용자명\)가 기본으로 표시됩니다. ASS 위해
『10600라는 폴더를 만들겠습니다. 실습을 하면서 사용할 파일들을 모두 저장할 폴더입니다.

화면 오른쪽 상단에 있는 New HES 클릭하고 드롭다운 메뉴 S Folder 를 클릭합니다.

스어              x

SO texsihosrasueyree

= jupyter

OD 0

BD © OneDrive - University of Caltomia - ining
© © Pxtures

© © Saved Games

O © Searches

CG © Videos

13 days age
13 days ago
13 Gays age
J hours age
13 days ago
13 days ago
13 days apo
1) days ago

3% 파이썬 설치

39


===== PAGE 40 =====
이제 폴더 목록에 방금 REE untitled Folder 폴더가 표시된 것을 볼 수 있습니다.

eee      =                                                  르스 a
o—      > =

€ SO weatecrsatimes   a   =    205 5      =     wii

|     = yepyter                                                   19094

|

：      tin  Se || 1<3에기

;      See teva © pete actions on Dem                                       Upest New CS

|      rey  ~ =                                       heme Laut Mocties +

：       8 ODte=                                            13 days ap

/       BS sce?                                               en hour 000

|       S Stes                                               13 0 ap

:       S Coen                                                   6 cays age

：       8 Canc                                               a Gay ap

:       S Diem                                               Dhowrs age
S Drewes                                               Dep op
S&S 2                                                 13 aap age
2 Cun                                                 Deapep
BS eee et se Cats ee                                       Shows 290
을 Oa                                              Deep oe

H       SD wetter                                                13 0 0

：       고 은 에                                               Days a

| 을 (2 weeetaee                                                    “= |
:       & 은                                                13 9760
'

폴더 이름을 변경하기 위해 Untitled 『0106「에 체크하고 왼쪽 상단에 있는 Rename 버튼
을 클릭합니다.

으   a                 ‘               re       2   0
- (< 9        re    :    a         wt
= jupyter                                                   Logout

tn   로   Cotes

Eo                         mt mee

-)-s                                      hare = Last Mocied @
6 ORGea                                                    13 days ago
© 0 Acca                                                    hous 0
8 OCraa                                                  13 days ago
들 2 대                                                     6 days ago
© © Oscars                                                  acy oe
© OC Omen                                               그치 ego
O Ofercts                                                     13 days ago
Y 0                                                      13 days ago
을 0mm                                                   13 days 090
DD Cneleen | 래벼매니 Cotter - bein                                        Shours ago
S OF                                                  13 cays age
© © Seed Gomes                                                1307
들 0 tee:                                                  13 doy og
2 ete                                               3 mintee oge
S Oma                                                   Dap ee

40 1% 준비하기



===== PAGE 41 =====
팝업 창이 뜨면 폴더 이름을 『10600로 바꾸고 파란색 Rename HES 클릭합니다.

home               x

<      CS | 020 lecathost£8282/treet                                                                                                                          wl

Rename directory

Enter 0 new directory name

Untitled Folder2] 이름이 FinEng= 바뀌었을 것입니다. 이제 FinEng SS 클릭해서 S
더 안으로 들어갑니다. 아무 내용이 없는 빈 폴더입니다.

”   =  ㅁ   ×
> Finkng!        ad

<   S | O locathost£6SE/rree/FinEng                                =     —         8 '.

= jupyter                                                                        Logout

Files   Running   Chssters

Select Rems to perform actions on them                                      Upeesc News OS

ㆍ ti! FinEng                                                             Name+ Last Mocted

o                                                         seconds 200

Notedook Ist empty

이제 파이썬 프로그래밍을 위한 준비가 끝났습니다.

3.3 첫 파이썬 프로그래밍
Al 파이썬 프로그래밍을 위해 새 노트북 파일을 만들어보겠습니다. 앞에서 했던 것과 마찬가
지로 오른쪽 상단 New HES 클릭한 다음, Pythons 를 클릭합니다."

xz

1 아나콘다의 버전에 따라 Python 3 CHA! Python [00008 root]2} Python [default]7} 보일 수도 있는데, 이 책의 HSS 위해서는 S
중 어떤 걸 선택해도 무방합니다.

3장 파이썬 설치 41


===== PAGE 42 =====
소아 a 오오노                                                                             벅    =
4 =                  네트                 ass         To __
¢   CSO kcalhostssssrree/FinEngt                           도             ee     ao!
은 Jupyter                                                                             Logout
Files   Roneing   Chusters
Select Rems to perform actions on them.                                               Upioad [New=] c
나
=a                                                        [그
=                                                                  | Omer            |
Notebook Est empty                       Text Fite
| Folder
Terminals Unavailable
host ESSE ree/Finings                                                                            el

브라우저에 새 탭이 열리면서 빈 노트북 화면이 나타납니다.

ae                              2

 TRI Ss \      Z                  J
<  CS O kecaihosreses  books/FinEng/Unotied spynb?kerne!_name=python3                  :
J Jupyter Untitled Last checkpoint « few seconds 200 (

Fie Edt View insert. Cel Kemel Widgets Help.

B+ x 2B + HMC Com   , a

노트북 파일의 이름을 지정하기 위해 노트북 제목을 클릭합니다. 지정한 노트북 제목은 파일
명으로도 사용됩니다.

--~-   SOR _   ae                                       v   =
~   7
29960 00000 8 oN       ~ 로

. C|O locathost868/notebooks/fanEng/ Unstled ipyob Tkarnal naman python?                 —  7   7

= jupyter [Untitied) ic»    @ few seconds ago (  사아 |    ur Bs 7   Co) Logout

Fie Edt View inset Cel Kernel Widgets Help

BSB +x 20268 * + WH BC Coss  vii
| Ini { Jz 1

42 1% 준비하기



===== PAGE 43 =====
입력창이 나타나면 UntitledS 11로 바꾸고 Rename 버튼을 클릭합니다.

Ci  fo) Sree ipynb?kernel_name=python3

Rename Notebook

Enter a new notebook name

| umm

파일명이 His Ube 것을 확인할 수 있습니다.

FinEng/          x isi             x}
va      - =e                 \

S . O locathost8283/notebooks/FinEng/Hiipynb

= jupyter [Hips Checkpoint 5 minutes ago (sutosaved)                                                                    &  Logout
File     Edit     View     Insert     Cel     Kernel     Widgets     Help                                                    Trusted       | Python 3 O
a + *« @ 60 & + WH BC Code          ” o

|  In [ ]: 1

이제 노트북에서 코딩을 하고 ATES 확인하는 방법을 알아보겠습니다.

다음 그림에서 빨간색이 코드를 입력을 하는 부분이고, 파란색이 결과를 보는 부분입니다. 앞
으로 이 공간을 워크스페이스(70ㅁ<6ㅁ0206)라고 부르겠습니다. 일반적으로 프로그래밍에 이
용되는 각종 DEL 코딩을 하고 800 VES 누르면 디버거와 컴파일러가 실행되며 별도의
창에 결과가 표시되지만, 노트북은 별도의 컴파일을 수행하지 않고 A(cell) 단위로 바로 결
과를 확인할 수 있어서 사용이 편리합니다. 빨간색 Alo] BES 입력한 & [Shift ]+[Enter |S
누르면 아래 파란색 부분에 결과가 나타날 것입니다.

3장 파이썬 설치 43


===== PAGE 44 =====
c O tecatont sist rotebocks Fring Merb     더       a                         w
= jupyter Hi ust co    12 mimess oye                               vos
Fle Edt Vew bet Cel Kemel Widgets Help                  Trusted  16003 O
5 ¢ > @B + + HM MC Cor    ㆍ 2

|  Inf ]:  1

처음 설치했다면 빨간색 셀에 줄번호가 보이지 않을 테니 줄번호가 보이도록 설정을 바꿔봅시
다. 메뉴에서 View > Toggle Line Numbers 를 클릭하면 줄번호가 나타나거나 사라집니다.

’                        = 66 2
              [1 0
= jupyter Hi Last Checkpoint 14 minutes ogo (autoaaved)                              & coo
Flo Eat View meet Cel Kernei Wide = Help           Trated | Pythea 3 O
B+ 3 — Togge Header   1 C Cos   2

이제 워크스페이스의 빨간색 부분에 print ('st0|' )라고 입력하고 [Shift ]+ [Enter |S
봅시다. 파란색 영역에 하이라고 결과가 출력되는 것을 볼 수 있습니다. 너무 Seek, 첫
파이썬 코덩이 끝났습니다. 또한 학습을 위한 환경 세팅도 완료됐습니다.

2 구 버전의 주피터 노트북에는 이 메뉴가 없으므로 내비게이터에서 주피터 LESS 업데이트해주세요. 혹은 [0 1+[ |. Ｌ|을 순서대
누르면 셀 단위로 줄번호를 표시할 수 있습니다.

44  1부 준비하기



===== PAGE 45 =====
ar                        세                                                      v    -   q
c 스스          아가 로        :

= = jupyter   Hi Last Checkpoint: 23 minutes ago (unsaved changes)                                                      「 개  Logout

Fie Edt View insert Cel Kermel Widgets Help          Trusted # | Python} O

SB +x 의 6 + WH BC Code  ” os

In [1]: print(‘@}o]")

하이

In [ ]:

3.4 -ESs 이용한 실습 진행 방법

북을 이용해 AGS 할 때는 각 YEJo] 맨 앞부분부터 순차적으로 실습을 진행해야 합니
다. 앞에서 나온 코드의 결과를 뒤쪽에 나오는 코드로 사용하는 경우가 많기 때문에 앞부분을
건너뛰면 결과가 나오지 않을 수 있습니다. 또한 순차적으로 진행하더라도 한 번에 진행해야
만 하는 경우도 있습니다. 메모리에 들어 있는 앞부분 코드의 Azo] 필요한 뒷부분 코드가
있기 때문입니다. 따라서 실습을 진행하다 중단하고 다시 시작할 때는 맨 위 코드부터 다시 실
행을 하고 이후 실습을 계속해야 하는 경우가 생길 겁니다.

코드를 모두 다시 실행하려면 첫 셀부터 모두 (Shift ]+[Enter |S 눌러 수동으로 실행할 수도
있지만, 메뉴에서 Kemel > Restart & Run All HES 누르면 전체 AS 일괄로 다시 실행할
수도 있습니다.

09
— 14076 Hi Last Checkpoint 3 minutes ago (autosaved)                                       ^ pase
File Edt View insert Cell Kemel Widgets = Help                Trusted | Python 3 O
65 + *« @ B& + & MH BB interrupt     3
| Restart
|        :
Restart & Clear Outp
Reconnect
하이      Shutdown
In [ ]:   1        |  Change kernel    ㆍ

3장 파이썬 설치 45



===== PAGE 46 =====
이 책의 파이썬 소스는 깃허브를 통해 제공합니다. 깃허브의 파이썬 노트북 코드를 보면 각 챔
터의 실습 코드가 각각 하나의 파일에 담겨 있는데, 이는 앞에서부터 순차적으로 진행해야 하
기 때문에 그렇습니다. 실습 코드를 실행할 때는 첫 셀부터 실행하며 진행하기 바랍니다.

46  1부 준비하기



===== PAGE 47 =====
4차 산업혁명과 금융산업

바야흐로 4차 산업혁명 시대입니다. 정부는 2017년 대통령 직속 4차산업혁명위원회
를 설치하고 4차 산업화의 경쟁에서 대한민국이 뒤쳐지지 않도록 독려하고 있습니다.

4차 산업혁명을 알아보기 전에 먼저 산업혁명의 역사에 대해 간략히 살펴보겠습니다.
최초의 산업혁명은 18세기 영국에서 일어났습니다. 제임스 와트가 발명한 증기기관으
로 이전에는 인간의 힘으로 할 수 없던 일을 기계를 이용해 처리하게 되며 생산 방식에
서 혁명을 이루었고, 기차, 증기선 등 장거리 교통수단이 생겨나 원료와 제품의 이동이
쉬워지면서 물류라는 개념도 탄생했습니다.

2차 산업혁명은 19세기 후반 미국에서 시작됐습니다. 전기 발명으로 본격적인 산업화
가 시작된 것이죠. 무엇보다 생산 방식이 크게 바뀌었습니다. 벨트컨베이어와 분업으
로 대표되는 대량생산 시대가 열린 것입니다. 대량생산을 통해 생산원가는 크게 낮아
지고, 많은 사람들이 산업화의 혜택을 누리게 되었죠. 제너럴 일렉트릭(68)은 전기와
전구로 미국의 밤을 밝혔고, 포드는 미국에 마이카 시대를 열었으며, Melo] (Carrier
Corporation = 에어컨을 보급해 미국 서부를 살기 좋은 KOS 만들었지요.

3차 산업혁명은 20세기 후반 인터넷이 탄생하며 일어났습니다. 컴퓨터가 보급되고 모
두가 인터넷을 통해 정보를 습득할 수 있는 세상이 된 것이죠. 제한된 소수가 정보를 독
점하던 시대에서 모든 사람이 정보를 공유하는 시대가 되었습니다. 동네 공인중개소만
알던 아파트값을 인터넷을 통해 다른 지역 사람들도 알 수 있게 되었고, 증권사 객장에
나가야만 볼 수 있던 주식 시세를 집에서도 볼 수 있게 된 것입니다. 정보의 불균형이 심
했던 취업시장 역시 변화했습니다. 1990년대 말까지만 해도 인기 있는 기업은 특정 대
학교에만 입사 지원서를 보내주었고 이를 받은 사람만 그 회사에 지원할 수 있었답니다.

4차 산업혁명은 이제 막 시작됐습니다. 인공지능, 빅데이터 등 융합 기술을 기반으로
산업 전반을 지능화하는 것입니다. 3차 산업혁명이 정보의 공유를 가져왔다면, 4차 산
업혁명은 지능의 공유를 가져옵니다. 3차 산업혁명 시대에는 공유된 주가 데이터를 읽
고 투자 의사 결정을 하는 주체가 사람이었지만, 4차 산업혁명으로 인간의 개입 없이
기계가 스스로 데이터를 읽고 판단을 합니다. 관련 지식을 갖춘 자만이 할 수 있었던

3장 파이썬 설치

47


===== PAGE 48 =====
48

일을 기계가 대신함으로써 과거의 산업혁명과는 달리 화이트칼라의 직업도 기계가 대
체할 수 있게 되었습니다.

대표적 화이트칼라 직군인 금융산업 역시 4차 산업혁명의 영향을 많이 받고 있습니다.
고객의 투자 BARS 분석해 투자상품을 권유하는 인공지능인 로보어드바이저(80120-
advisor), 신문 기사나 SNS 키워드에 많이 언급된 단어를 중심으로 투자 SSS 선정
하는 감성 분석(66001016ㅁㄴㄷ30ㅁ21515)은 이미 금융업계에서 유명합니다. 기존의 HE
트레이딩 기법에 인공지능을 접목해 컴퓨터가 스스로 알고리즘을 진화시키도록 하려
는 시도 또한 활발합니다.

골드만삭스 08ㅇ 로이드 블랭크페인은 2015년 “골드만삭스는 11 회사"라고 선언했고,
이미 직원 비중의 30%가량을 17 부서 인력으로 채웠습니다. 빅데이터와 자연어 처리
기술을 보유한 인공지능 Ase (Kensho)S 도입해 투자 관련 자료 수집과 리포트 작성
에 이용하면서 금융권에서도 고급 직군에 속하던 애널리스트를 대체했고, 고객 주문을
처리하던 딜링룸 직원 600명도 프로그램 관리자 2명으로 대체했습니다. 골드만삭스뿐
만 아니라 대부분의 금융기관들이 4차 산업혁명 기술 도입을 위한 경쟁에 뛰어들었습
니다.

안타깝게도 국내 금융권에는 골드만삭스와 같은 혁신적 변화의 조짐은 아직 보이지 않
습니다. 심지어 트렌드에 둔감한 구세대들은 인공지능이라는 용어 때문에 4차 산업혁
명을 인정하지 않기도 합니다. 이는 인공지능이라는 개념이 오래전부터 여러 17 분야
에서 오용되고 있었기 때문이지요. 인공지능이라는 WAS 1930년대에 생겼지만 기술
적 한계로 성장이 ASU. 1980년대부터 전산 장비가 발달하고, 2000년대에 신경
모형 WAS 인공지능에 도입하면서 인공지능 기술은 본격적인 성장을 시작했습니다.
하지만 20여 년 전부터 소위 있어 보이고자 하는 사람들이 인공지능이라는 말을 사용
했는데, 그 당시 사용한 인공지능이란 단어는 지금과는 개념이 다릅니다. 현대의 인공
지능은 인간의 개입 없이 스스로 학습하고 진화하는 시스템을 말하는 반면, 과거의 인
SASS 스스로 학습하는 것이 아니라 인간이 미리 정해놓은 패턴에 따라 반복적인
일을 자동화한 시스템인 것이지요. 우리나라 금융계에도 빨리 변화의 바람이 불어 4차
산업혁명 시대에 뒤쳐지지 않으면 좋겠습니다.

1부 준비하기



===== PAGE 49 =====


===== PAGE 50 =====


===== PAGE 51 =====
=  ^                                                     Chapter &
주식, 가격, 지수

4.1 주식과 가격

주식의 가격은 어떻게 정해질까요? 내가 사고 싶은 종목이 지금 비싼지 싼지 어떻게 알 수 있
을까요? 이런 궁금증은 주식시장이 생기기 전부터, 돈에 관심 있는 모두가 알고 싶어 하는 주
제입니다. 주식의 적정 가격만 정확히 알 수 있다면 주식시장에서 ES 버는 건 식은 죽 먹기
일 테니까요. 아쉽게도 이 질문에 답을 할 수 있는 AMS 아직 아무도 없습니다. 다만, ES
좋는 많은 사람의 노력으로 주식의 가치를 평가하는 다양한 밸류에이션 모델이 나와 있을 뿐
입니다. 여기에서는 주식의 가격이 왜 중요한지, 금융공학에서는 어떻게 밸류에이션을 하는지
알아보겠습니다.

wr

주식가격은 기업의 과거, 현재, 미래를 반영

주식가격은 기업의 과거, 현재, WAS 반영한 종합 분석의 산물입니다. ake 삼성전자(종목코
드: 005930) 종목의 2016년 1월 초부터 2017년 12월 말까지의 주가 그래프를 보겠습니다.

|

4장 주식. 가격, 지수 51


===== PAGE 52 =====
eee ee ee eee

90 서하

|

2750000 +
2250000 +

2016-04 2016-07 2016-10 2017-01 2017-04 2017-07 _—.2017-10

201714 마지막 날 삼성전자의 주가는 254만 8000원이었습니다. 그럼 이 시점의 삼성전자 주
가는 싼 것일까요, 비싼 것일까요? 2016년 1월보다 아주 많이 올랐다고 할 수 있나요? 반도체
경기 호황과 경쟁사 부진을 감안하면 오히려 덜 오른 것은 아닐까요? 이런 질문에 답을 찾기
위해 많은 사람이 기본적 분석, 기술적 분석 등 다양한 분석을 합니다.

금융권에서 애널리스트(40231550)라는 직업을 들어봤을 겁니다. 애널리스트는 금융권에서 of
주 잘나가는 직업 중 하나로, 하는 일은 바로 주식 가치를 산정하는 것입니다. 애널리스트는
기업 실사, 미래 전망, 경쟁사 분석, CEO 인터뷰 등을 통해 다양한 BAS 하고, 향후 주가 예
측을 위한 밸류에이션을 시행해 목표 주가를 산정하고 분석 보고서를 발간합니다. 이 모든 노
력은 결국 현재 주가가 적절한지 판단하기 위한 활동입니다.

싸면 매수, 비싸면 매도

여러 BAS 통해 현재 주가가 싸다고 생각하면 주식을 사고, 비싸다고 생각하면 주식을 팔면
되겠죠. 트레이딩 용어로 바꾸어 얘기하면 전자는 롱 포지션, 후자는 se 포지션에 배팅을 하는
것입니다.

여기서 롱078)은 매수(501), 또는 포지션(잔고)이 플러스인(보유) 상태를 말하고, 반대로
숫(911070)은 OW (sell), 또는 포지션이 마이너스인(빚진) 상태를 말합니다. 이렇게 서로 다른
판단을 하는 사람들이 거래소에 모여 거래가 이루어지고, 주가는 더 많은 사람이 배팅하는 방

lo flo

52  2부 주식과 지수


===== PAGE 53 =====
향으로 움직이게 되지요.

기대 수준이 서로 다르기 때문에 거래가 발생

주가를 산정하는 데 사용되는 과정과 지표는 다양합니다. 또한 같은 지표를 사용한다고 해도
실적을 어떤 방식으로 산식에 반영하는가에 따라 결과는 달라집니다. 그래서 사람들이 적정
주가를 서로 다르게 판단하게 되고, 그 결과가 매매로 나타나는 것입니다. 사람들이 모두 동우
한 예측을 한다면 거래 자체가 일어나지 않겠죠? 모두가 지금 주식이 싸다고 생각하면 롱 포
지션으로만 배팅이 몰리고 그러면 주식을 팔려는 사람이 없을 테니 매매가 이루어지지 않을
테니까요.

밸류에이션: 적정 주가 산출

애널리스트는 특정 종목의 주가를 평가하기 위해 경영전략, 시장 동향, 경쟁사 동향 등 기업
활동을 심층 분석하고 다양한 밸류에이션 방법을 적용해 목표 주가를 산정합니다. 애널리스트
가 사용하는 밸류에이션 방법을 보면 종목마다 그 방법이 다른데, 이는 항상 성립하는 밸류에
이션 방법은 없다는 증거입니다.

주가 평가에 사용되는 밸류에이션 모델은 배당할인 모형((>ㅁ0"), 고든(302000)의 성장률
모형, CAPM, FV/EBITDA, PER, EPS, PBR 등 재무 비율을 이용한 상대비교 모형 등 다양
합니다. 이들에 대한 BBS 각 종목에 대한 BAT 함께 다루어져야 하고, 금융공학보다는 투
Are (investment bank) 분야에서 더 관심을 갖는 주제이므로 이 책에서는 다루지 않습니
다.

물론 금융공학에서도 밸류에이션을 합니다. 금융공학의 여러 분야 중 WE 트레이딩 분야가
밸류에이션에 특히 관심이 많습니다. 적정 가격을 찾아야 트레이딩을 할 수 있기 때문입니다.
전통적인 밸류에이션 모델은 종목 하나하나를 심층 분석하고 기업 활동이 주가에 미치는 영향
을 예측하며 적정 주가를 찾는 반면, 금융공학은 종목 하나하나를 분석하기보다 유사한 다수
종목의 주가를 관찰해 주가를 형성하는 규칙을 찾아내고 이를 바탕으로 적정 주가를 찾습니
다. 금융공학이 통계학에 뿌리를 두고 있어서입니다.

4장 주식, 가격, 지수 53


===== PAGE 54 =====
4.2 주가 비교의 ABS: dla! 대상의 표준화

주가 비교를 위해 삼성전자와의 비교 대상을 찾아보겠습니다. 다음은 반도체라는 공통점이 있

ㄴㄴ

는 하이닉스, 그리고 전자라는 공통점이 있는 16전자의 2016년 1월부터 2017년 12월까
지의 주가 그래프입니다.

| — 5\하이닉스

2016-04

2016-07

2016-10 2017-01 2017-04  2017-07  2017-10

110000

— Ｌ6전자

2016-04

2016-07

2016-10 2017-01 2017-04  2017-07  2017-10

2016% 1월 대비 201741 12월에는 어느 SHO} 더 많이 올랐을까요? 달리 표현하자면, 어느
종목이 더 수익률이 높았을까요? 그래프가 따로파로 있어서 눈대중으로 파악하기 어려우니

54

2부 주식과 지수


===== PAGE 55 =====
그래프를 겹쳐서 볼까요?

3000000

— $\하이닉스 |

2500000ㄱ7

2000000 -+

1500000 +

5000007------------ “+ a pt pee SEE seneofeseescnescesooe  보오,   —et pal ae A 6060. SER FEE.

2016-04 2016-07 2016-10 2017-01. «2017-04  2017-07  2017-10

프를 합쳐놓으니 삼성전자 주가가 올라간 AS 눈에 띄지만 sKspo|YAS} LG 전자가 움
직이는 모습은 보이지 않죠? 주가 수준을 감안하지 않고 단순히 그래프만 합쳐놓았기 때문입
니다. 어느 종목이 더 수익률이 높은지 쉽게 비교하려면 비교 대상들의 주가를 같은 기준으로
통일한 후 비교해야 합니다. 이를 지수화(1006×108)라고 부릅니다.

지수는 비교 대상 가격을 기준일 가격으로 나누고 기준가를 곱해서 계산합니다.

Price, (Ara 주가)
Price, (7|EU 주가)

×기준가

가격지수 =

우선 기준일을 2016년의 첫 거래일인 1월 4일로 잡고, 기준가는 100으로 설정하겠습니다.

으(하이닉스

2015-12-30               30,346                    1,232,071               53,377
2016-01-04               29,754                    1,178,290              52,087
2016-01-05       30,198         1,181,224      53,873

위 표를 참고해 삼성전자의 19 49 S71 1,178, 2008S 기준으로 19 5일의 가격지수를
계산해보겠습니다.

4장 주식, 가격. 지수. 55


===== PAGE 56 =====
“4               0)
Price, 100 = 1,181,224

=                x 100 =100.25
Price,                1,178,290

삼성전자 가격지수 =

너무 간단해서 서운할지도 모르겠습니다만, 여기서부터가 금융공학의 시작입니다. 금융공학
의 주요 관심사인 주식, 지수, 거시경제지표 SS 비교 분석하기 위해서는 서로 다른 스케일의
가격 정보를 지수화하는 과정이 필요합니다. 이 개념은 뒤에 AWS 주가지수 산출, 펀드 가격
산정 등에 동일하게 적용됩니다. 그럼 세 종목의 주가를 지수화하여 비교한 그래프를 보겠습
니다.

| — 하이닉스
— 삼성전자

2501

200 5

150 5

100 +

2016-04 2016-07 2016-10 2017-01 2017-04 2017-07. 2017-10

세 종목 중 5\하이닉스의 상승폭이 가장 Aa), LG AAV} 가장 작았다는 것을 한눈에 ot
slenich 2 또한 Y=} 눈금을 통해 9하이닉스는 2016년 1월 대비 약 250%, 삼성전자는 OF
210%, 16 전자는 약 200% 상승했음을 알 수 있습니다.

이렇게 가격대가 서로 다른 금융상품들은 지수화를 통해 비교 가능성을 높일 수 있습니다.

4.3 주가지수: 관심종목 그룹 MAS 대표하는 가격지수
먼저 지수의 사전적 정의를 한번 본 다음. 이어서 다양한 지수에 대해 살펴보겠습니다.

56  2부 주식과 지수


===== PAGE 57 =====
Z| (index) 구체적인 숫자 자체의 크기보다는 시간의 흐름에 따라 수량이나 가격 등 해
당 수치가 어떻게 변화되었는지를 쉽게 파악할 수 있도록 만든 것으로 통상 비교의 기준이
되는 시점(기준 시점)을 100으로 하여 산출한다. (「통계용어ㆍ지표의 이해』 통계청, 2015)

주가지수의 종류: 종합지수, 대표지수, 섹터지수, 테마지수 등

지수화를 통해 파악하고자 하는 대상의 가치가 어떻게 변화했는지 쉽게 알 수 있습니다. 주가
지수도 마찬가지로 관찰하고자 하는 SHS] 주가를 모아서 만드는데, 지수 디자인 컨셉에 따
라 종합지수, 대표지수, 섹터지수, 테마지수 등 종류가 다양합니다. 여기에서 말하는 '파악하
고자 하는 WAS 구성종목이라고 부릅니다.

먼저 종합지수는 KOSPI 지수, KOSDAQ 지수 등 증권시장에 포함된 종목 전체가 관찰 대
상이며, 국가 전체 경제 규모 변동을 반영하는 지표로도 사용합니다. 대표지수는 KOSPI200
지수, KOSDAQ150 지수 등 각 시장 내 대표 종목들로만 구성한 지수입니다. 섹터지수는
KOSPI 금융, KOSPI 헬스케어 등과 같이 유사 ASS 영위하는 기업들만을 그 구성종목으로
합니다. 테마지수는 배당률이 높은 종목들만을 모아서 만드는데 예를 들어 (0571고배당50

등 특정 테마에 어울리는 종목들을 골라서 만듭니다.

지수 산출 방법: 다우존스 방식 ys, 시가총액 방식

지수를 산출하는 방법은 크게 구성종목 주가의 평균을 이용해 산출하는 ESA (Dow
Jones) 빵식과 구성종목 시가총액(주가×상장주식 수)의 합계를 이용해 산출하는 시가총액 방
식의 두 가지로 LPYUCh, 다음 ES 보면 이해가 빠를 것입니다.

1.000               1,000,000            1,000,000,000                 1,000             1,000,000,000
2,000                1,000,000            2,000,000,000                  2,000             2,000,000,000
1,000,000                       1,000            1,000,000,000          1,000,000             1,000,000,000
500                2,000,000            1,000,000,000                     500             1,000,000,000
1,000                       1,000                   1,000,000                 1,000                    1,000,000

지수 반영                                                       200,900           5,001 000,000

4장 주식, 가격, 지수 57


===== PAGE 58 =====
상장 AAS 증권시장을 통해 자본을 조달하는데, 기업이 조달한 자본의 규모는 개념적으로
열마짜리 주식(주가)을 얼마나 많이(상장주식 수) 팔았는지를 보고 판단합니다. 종목 4, <, D
는 주가가 서로 다르지만 시가종액(주가×상장주식 수)이 같으므로 기업 규모가 비슷할 AY
니다. 특히 C 종목은 주가가 100만 원이나 되지만 상장주식 수가 적으므로 주가가 2000원인
8 종목보다 기업 규모는 작을 것으로 판단할 수 있습니다.

다우존스 방식에서는 구성종목들의 주가의 평균값을 지수 산출에 사용합니다. 기업의 규모보
다는 시장에서 거래되는 주식의 가격에 초점을 맞춘 것이지요. 반면 시가총액 방식은 시가총
액의 합을 지수 산출에 사용합니다. 시장의 가격보다는 기업의 규모에 주안을 두는 것입니다.

유동 시가총액 방식
대부분의 지수는 시가총액 방식으로 산출하며, 다우존스 방식은 잘 쓰지 않는 편입니다. 우리
나라의 KOSPI 지수도 과거에는 다우존스 방식으로 산출했으나 지금은 시가총액 방식으로 Ab

출하고 있습니다.

요즈음 인기리에 개발되는 지수는 시가총액 방식에 약간의 변형이 가해진 형태인데, 유동
을 반영한 시가총액 방식입니다. KOSPI200 지수가 이렇게 산출되는데, 시가총액을 구할
(주가 ×상장주식 수)가 아닌 (주가×유동주식 수)로 구하는 것입니다. 유동주식이란 실제로
거래소 시장에서 유통되는 주식을 말합니다.

ind
때0

|

어
ue
프

발행주식, 상장주식, 유동주식 용어 정리

* 발행주식: 기업에서 자금 ASS 위해 발행한 주식. 발행주식 수는 재무제표에서 찾아볼 수 있습니다.

* SUA! 발행주식 중 거래소 시장에 상장한 주식.

* 유동주식: 유통이 Of 되는 주식을 제외한 거래소 시장에서 실제로 유통되는 주식. 유통이 안 되는 주식의
예로는 최대 주주 및 그 친인책(특수관계인), 우리사주조합, 자사주. 정부 등이 ASS 지분 등이 있습니다.

이렇게 지수를 산출하는 이유는 지수를 이용한 금융상품을 만들어 운용할 때 운용이 용이하도
= 하기 위해서입니다. 예를 들어 ㅅ기업이 발행한 주식 100만 주 중 유동주식이 50만 주밖에
되지 않는다고 생각해보죠. 지수가 100만 주를 기준으로 움직인다면 펀드매니저들이 100만
주에 해당하는 SSS 확보하기 위해 50만 주를 가지고 BBS 해야겠죠? 이 경우 시장가격이

58  2부 주식과 지수



===== PAGE 59 =====
왜곡될 수 있고(경제학의 수요-공급 곡선 개념을 떠올려보세요. 공급보다 수요가 많아지면 가격이 올라
갑니다), 펀드매니저도 물량 확보가 어려울 수 있습니다. 다시 말해, 해당 지수를 기초로 한 상
BS 운용하기 어렵다는 뜻이지요. 그래서 지수사업자는 지수를 개발할 때 유동비율을 반영한
시가총액 방식을 애용합니다.

여기서 지수사업자란, 지수를 개발해서 발표하는 기관을 말합니다. 우리나라의 경우 한국거래
AT} 직접 지수사업을 하고 있고, 매일경제, 에프앤가이드(8ㅁㅠㅇ4106) 등도 지수사업을 합니
다. 국제적으로 유명한 지수사업자로는 모건스탠리캐피털인터내셔널(51601), 파이낸셜타임
스스톡익스체인지(『188), 스탠더드앤드푸어스(6&2) So] 있습니다.

KOSPI 지수와 KOSPI200 지수는 다르다

KOSPI 지수는 KOSPI 시장에 상장되어 있는 보통주 전체(2018년 1월 기준 769종목)를 구성
종목으로 합니다. 상장 기업의 경제 규모와 직접적으로 관련이 없는 우선주, 외국증권(ㄷㅁ),
펀드 등은 제외합니다. 반면 KOSP1200 지수는 각 산업군별로 규모(시가총액)가 큰 SSS 뽑
는 방식으로서 KOSPI 시장의 상위 200개 종목으로 구성됩니다. 두 지수가 담고 있는 SSO]
다르기 때문에 지수도 당연히 다르게 산출되겠지요.

™ KOSPI200      ™@ KOSPI200 제외

시가충액(억 원 | :

0%               20%              40%              60%              80%             100%

대한민국 대표 GAIA KOSPI 지수

KOSPI200 지수는 유동주식 수를 사용하는 반면, KOSPI 지수는 상장주식 수를 사용합니다.
시장에서 형성된 가격은 유동주식뿐 아니라 발행주식 수 전체를 반영하기 때문에 대한민국 전
반의 경제지표를 나타내는 지표로는 종합지수인 KOSPI 지수가 더 적합합니다. 따라서 GDP,
실업률 등 거시경제지표와 시장 규모 변동을 비교할 때는 KOSPI 지수를 사용하는 것이 더 바
람직합니다.

4장 주식, 가격 지수 59


===== PAGE 60 =====
KOSPI12000| KOSP! 전체를 대변한다(파레토 법칙)

KOSPI 지수와 KOSP1200 지수는 분명히 다르지만, 두 지수는 상당히 유사하게 움직입니다.
8:2의 법칙으로 유명한 파레토 법칙은 지수에도 역시 적용됩니다. 상위 20%의 종목이 지수
전체의 움직임을 좌우하기 때문입니다. 결국 거시경제지표와의 비교, 해외 지수와의 비교 시
데이터를 구하기 수월한 KOSP1200 지수를 사용해도 별문제가 되지 않는다는 얘기지요. 더욱
이 미국같이 거래소가 여러 개 있는 나라는 국가 경제 규모를 대표하는 종합지수가 딱히 없기
때문에 많은 사람이 S&P500 지수를 미국 대표지수로 이용합니다.

4.4 지수 6. 시수: 회귀분석

앞에서 금융공학은 유사한 다수 종목의 주가를 관찰해 주가를 형성하는 규칙을 찾아내고 이를
바탕으로 적정 주가를 찾는 일이라고 소개했습니다. 규칙을 찾아내는 방법 중 가장 대표적인 예
가 회귀분석인데, 여기에서는 5&0500과 KOSPI200 지수를 비교하며 규칙을 찾아보겠습니다.

S&P500 vs. KOSPI200 지수 비교 1

금융공학, 아니 금융이 추구하는 것은 공정한 가격을 찾아내는 것이며, 이를 위해 해외 증시와
비교하는 방법이 애용됩니다. 국제적으로 증시 흐름이 크게 다르지 않고, 특히 미국. 중국 등
우리나라에 크게 영향을 주는 시장의 지수는 증시 참고 자료로 항상 사용됩니다. 금융 관련 기
사, 애널리스트 리포트 등에서는 ASA, 디커플링'이라는 용어로 국가 간 증시 SSO] 동조
화 또는 탈동조화 현상을 표현하기도 act  그런 차원에서 S&P5002} KOSPI200-2 유사한
종목이라고 할 수도 있겠습니다.

그럼 2016년 초부터 2017년 말까지 두 지수의 움직임을 한번 보겠습니다.

1 금융에서 국가 간 ABS(coupling/ le 한 국가의 경제가 다른 국가의 경제에 큰 SHS 미쳐 유사하게 움직이는 SHAS 뜻합니다. 미국
증시가 상승하면 다음 날 한국 SALE 상승하는 것이 대표적입니다. 디커플링(0600410100)은 그 반대 의미입니다.

60 2부 주식과 지수


===== PAGE 61 =====
— kospi200 |
2) rem SOD
2000 4-5; 2G ai |woseessessaceoesIee|아가: .
gk 데이
1000 sates cc eae 10 Ee SS Ee 06
Pe isin Zale 8) a ioe ae 0 이

2016-04 2016-07 2016-10 2017-01 2017-04 2017-07 2017-10

위 그림에서 & 수 있듯이 S&P5OO 지수는 2000대이고 KOSPI200 지수는 200~300대로 스
케일이 달라 시각적으로 변화를 파악하기 어렵습니다. 앞에서 배운 대로 지수화 작업이 필요
하겠죠. 지수화를 하고 다시 그려보겠습니다.

--- (0501200

1208 -

110 5

100 yA

90 +

2016-04 2016-07 2016-10 2017-01.  2017-04  2017-07 ~—«2017-10

위 그림을 보니 2016년 초부터 2017 4월까지는 두 나라 증시가 상당히 비슷하게 움직이다
가 4월 말부터 한국 증시가 점프한 모습이 보이네요. 문재인 대통령 취임으로 한국 증시의 펀
더멘털이 좋아졌다는 분석이 많이 나왔던 시기입니다. 그럼 두 나라 증시는 얼마나 유사하

4장 주식, 가격, 지수 61


===== PAGE 62 =====
A] 움직이고 있을까요? 이를 알아보기 위해 날짜는 과감히 생략하고 %축은 56&8500, 축은
KOSP12002 = 이루어진 새로운 그래프를 그려보겠습니다. 이런 그래프를 산포도라고 하는데
※축과 축의 상관관계를 파악해 두 변수 간의 관련성을 파악하기 좋은 그래프 형식입니다.

|    at
ep?
Ss
130 5      10    ~    고 우기
“ot
8                  2
Sinan               FO eee Deere
~
;      : fhe: |
1104 -  nee  fh. 그
1001 waay
23
90     100    110     120     130
S&P500

이 그래프를 보면 둘이 상당히 유사하게 움직인 것처럼 보이네요. 눈으로 볼 때 그렇게 보이긴
하지만. 우리는 금융공학을 공부하고 있으니 얼마나 그럴싸한지를 수치로 표현할 줄 알아야
합니다. 이럴 때 바로 회귀분석을 이용합니다.

회귀분석

회귀분석(768「055100 4001\515)이란 둘 또는 그 이상의 변수 사이의 관계를 분석할 때 널리
쓰이는 통계적 방법입니다. 책마다 사람마다 표현은 조금씩 다르지만 결국 두 변수 사이의 관
계를 나타내는 SAAS 찾아내는 것이 회귀분석의 목표입니다. 추세선은 ZIAl(y = ax +b)
뿐 아니라 다항식 곡선(1= ax’ + bx? + + 0), 삼각함수( yp =asinx+bcosx+c) 등 필요
에 따라 다양한 형태일 수 있습니다. 여기에서는 가장 이해하기 쉬운 직선 형태의 추세선을 찾
아보겠습니다. 여기에서는 과정은 생략하고 회귀분석의 결과로 구한 추세선을 먼저 보겠습니
다.

62  2부 주식과 지수


===== PAGE 63 =====
1401

1301

100 +

90               100              110              120              130
S&P500

우리가 찾고자 하는 것이 바로 저 빨간색 추세선입니다. 이 빨간 ALS 어떻게 구할 수 있을까
요? 컴퓨터는 임의의 추세선을 그려가며 추세선과 각 하늘색 점 간의 거리의 합이 최소인 추
세선을 찾아나가는 방식으로 회귀분석을 수행합니다. 수학적으로 이 과정을 고민하지는 않아
도 됩니다. 컴퓨터가 알아서 해주니까요. 로직만 알고 있으면 귀찮고 복잡한 작업은 컴퓨터에
Al 시키고 결과만 이용하면 됩니다. 회귀분석을 컴퓨터한테 시키는 방법을 곧이어 엑셀과 파
이썬 Belo] 살펴볼 것입니다.

직선 추세선의 공식은 중학교에서 배운 1차함수 ”=ㅇ+ 입니다. 여기서 a= 기울기, b=
＊절편이라고 합니다(기억을 잘 떠올려보기 바랍니다). 기울기가 1이면 정확히 x7} 변하는 양만큼
yi WchS ola, IC} SH x7} 변하는 Akt ys 데[글 SoS MSS SUE.
여기서 분석한 S&P50024+ KOSPI2002] 관계에서 기울기는 1.29, *절편은 -28.23으로 나왔
습니다. 즉 y=1.29x-28.23 입니다. 5&0500보다 KOSPI200°] 더 큰 폭으로 변화한다고
판단할 수 있겠죠?

참고로 통계학 책에서는 추세선 공식에 오차(6)를 함께 표현해줍니다. 오차는 식이 틀릴 수도
있으니 허용 AAS 나타내는 의미이나, 이 AS 통계학을 공부하는 Ao] 아니므로 이를 고려
하지 않겠습니다.

4장 주식, 가격 지수 63


===== PAGE 64 =====
S&P500 vs. KOSPI200 지수 비교 2

앞에서 최근 2년간의 지수를 비교했다면, 이번에는 좀 긴 기간을 관찰해보겠습니다. 리먼 브
라더스발 금융 위기가 발생한 2008년부터 2017년 말까지 기간입니다. 지수화 과정은 익숙해
졌을 테니 이제부터는 지수화 이후 단계부터 진행합니다.

1801 KOSPI200 | nanan feeeceeeereeefeceeneeeeeeecEEaEEEEE SEER EE EEE

j—— S&P500 |

160 +

100  Of EE SS Se, See

2009 2010 2011 2012 2013 2014 2015 2016 2017

앞에서는 두 지수의 움직임이 상당히 유사해 보였는데, 이 그래프를 보니 꼭 그렇지는 않은 것
같습니다. 산포도를 그려보겠습니다.

140

1201

100

KOSPI200

64 2% 주식과 지수



===== PAGE 65 =====
2016년 이후 데이터에 비하면 분포가 상당히 넓게 퍼져 있고, 직선의 모양과는 거리가 yy
다. 회귀분석을 해보면 어떨까요?

140 4

120 4

분포가 넓어 그림이 예쁘지는 않지만 그래도 컴퓨터는 충실히 회귀분석을 완수했습니다. 추세

선의 기울기 a=0.33, 절편 b= 66.43 입니다. 이 BES 두 지수 간에 연관이 높다고 볼 수
있을까요?

R* : 추세선의 품질

S&P500Z} KOSPI200°] 비교 기간에 따라 추세선이 달라지는 것을 확인했습니다. 이번어
+27} KOSPI2007} KOSPI 간의 추세선을 그려보겠습니다. 당연한 결과겠지민
에는 상관관계가 아주 높을 텐데 그걸 확인하려고 그리는 것은 아니고, 앞에서 수행한
의 회귀분석과 비교하기 위해서입니다. 2008년 1월부터 2017년 12월 말까지 (0511 지수와
KOSPI200 지수 간의 상관관계를 보겠습니다.

4장 주식. 가격 지수 65


===== PAGE 66 =====
140 5

120 7

그래프에서 확인할 수 있듯 KOSPI 지수와 KOSPI200 지수는 상관관계가 매우 높습니다. 수
치로 확인해보면 기울기는 1.02, 절편은 -0.08입니다.

그럼 이 세 번의 회귀분석 중 어떤 추세선이 가장 품질이 높을까요? 당연히 HOS 보면 마지
막에 수행한 것임을 알 수 있습니다. 하지만 이를 수치로 확인할 HE 없을까요? 이럴 때 이
용하는 수치가 바로 "입니다. SAAS 하면 *값이 함께 출력되는데, 이 값은 추세선
의 품질을 나타내는 점수입니다. oF] 1 사이 값이 나오는데, 1에 가까울수록 품질, 더 정확
히는 상관관계가 높습니다. 각 회귀분석에서 나온 #”값은 6&8500-62581200(2016~2017
년)이 0.92, S&P500—KOSPI1200 (2008~2017'4)°] 0.52, KOSPI-KOSPI200(2008~2017
년)이 0.97입니다. 즉, KOSPIS} KOSPI200 간의 추세선이 가장 품질이 높다는 의미입니다.

참고로 통계학에서는 RS 결정계수라고 합니다. R27} 무엇인지 알고 봐도 참 어려운 말을
갖다 붙였구나 하는 생각이 듭니다.

증권시장에서 공정한 가격을 찾기 위해 수행하는 여러 방법 중, 회귀분석을 통해 연관도가 높
은 벤치마크(비교의 기준) 지수를 찾는 것은 기본적이면서도 추가 데이터 분석의 기반이 되는
중요한 작업입니다.

66  2뿌 주식과 지수



===== PAGE 67 =====
이제 마이크로소프트 엑셀을 이용해 지금까지 배운 WSS 실습해보겠습니다. 이 책에서는 윈

도우용 엑셀 2013 버전을 기준으로 설명합니다. 버전이 달라도 실습에는 아무 지장이 없으나,
메뉴 위치 등은 다를 수 있습니다.

5.1 S&P500 vs. KOSPI200 비교
이 책의 웹사이트 또는 깃허브 저장소 https://github.com/finterstellar/download
에 접속해서 실습 파일을 모두 다운로드합니다. 먼저 05.1. S&P5@0-KOSP1I200@ (기초데이터) .

×15× 파일부터 열어보겠습니다.


===== PAGE 68 =====
S&P5007} KOSPI200 그래프 함께 그리기

2_S&PSOO-KOSPI200 치대 ~ Excet                 706-0 x

수석 데이터 검도 87                        Yong Whoan Kim-M16 +
jie ==—Bo & fePeston => Sy af
=     ae Si re     =  ——— BHaa-  aan ~ | 더 oe =
- 2-2- H- Seeee B- 멍-% BS Gyane- Bax- o- 35,7 Bh?

    28    n RABY ㅠ 스타일     편집     ^

|                      이 파일에는 2008년 1월부터 2017년 12월까지의 5&8500과 KOSPI200 지수가 담겨 있습니
다. 데이터가 들어 있는 아무 셀이나 선택한 후 |여0 ]+| | |를 누르면 가장 마지막 셀로 이동
{                           합니다. 2017-12-29까지의 지수가 들어 있는 것을 확인할 수 있습니다.

엑셀에서 데이터를 빠르게 살펴보기

ㅣ               * [Ctr |S 누르고 회살표를 누르면 데이터 블록의 가장 끝댄(처음 또는 마지막)으로 이동합니다.
* | Shift |를 누르고 화살표를 누르면 여러 셀을 다중으로 선택할 수 있습니다.
+ (Ctrl |과| 61111 |를 동시에 누르고 화살표로 이동하면 간단히 행/열을 일괄 선택할 수 있습니다.

이제 지수 그래프를 그러보겠습니다.

03 데이터가 들어 있는 아무 셀이나 선택한 후 [Ct] +[A]S 눌러 전체 AS 선택합니다.

68  2뿌 주식과 지수



===== PAGE 69 =====
HE 아이콘을 선택합니다.

@ 다음 그림처럼 상단 삽입 탭에서 AEs

mao 2:
을. 페이지 레이아웃

주식  데이터  검로  보기
com   (그               '  as           ㆍ  ㆍ          treo ~
  i?     |  Oo lea 2   @eco ㅣ ih    xT ey | Ee fe Be f
피벗  주전   표   그림 온라인 0    @내염 - ㅣ 주전      L  MADE ACMS YF 228 iP
테이를 피벗 aoe        그림 a+”     “| 자르 | 2자원 RENS             00
일러스트레이션 주가 기능                      스파크라인
단조    =  [Kv fa     ~ ~

2_S&PSO0-KOSPI200 xlsx - Excel

썸은선형

이 자르의 기능

ㆍ 시간(년, 월, 일) 또는 항목에 따른
주세를 보여줍니다

다음 BPO 사용
ㆍ 항목의 순서가 중요합니다.
ㆍ 데이터 요소가 많습니다.

Perr

는  다른 : eae REM

® 다음과 같이 지수 추이를 나타내는 그래프가 삽입되었을

것입니다.

MG 951 cs     2_SE&PSOO-KOSPI200 xlsx - Excel       지트 도구                  ? 8-= ㅁ x
PM a 상이 soma ox 데이터. 절도. 보기 Re 서식                 Yong Whoan Kim-MI6 =
= lise              =     =           =      -         본
파트 요소. 빠른 RED   ~             Z       —— 5 we 데이터 자트중 xe
Ry BOS                                     전환 선택 ESOS
자르 레이아웃                   자트 스타일                   데이터   종류: 위지     ^
RR. ©   x v fe                                                    ~
A      8     c     D    [0 테어 새기 그 (0 해 푸니     !     )    ke    L    M =!
1           S&PS00 | KOSPI200                                                            =
2 | 2008-01-02  1447.16   2353
3 2008-01-03  1447.16  234.67
4 2008-01-04  1411.63  235.77
5 2008-01-07  1416.18   231
6 2008-01-08  1390.19  23034                         +
7 2008-01-09] 140913 23253             차트 제목             ae
6 2008-01-10  1420.33  229.47| ~                       PZ
9 2008-01-11  1401.02  22441 =
10 2008-01-14|  141625   22281] 200                              Vi
11 2008-01-15   1380.95   220.91] 66
12 2008-01-16   13732   215.87} s0c0
13 2008-01-17   1333.25   21883} xo
14 2008-01-18   1325.19   219.87,   —_                         062.
15 2008-01-21| 1325.19   28080 oo 5 PF oF DP 세 QP OP
16 2008-01-22   13105   2055 gt ot ot
17 2008-01-23   1338.6   207.23
18 2008-01-24    1352.07     211.2                Tr rh eta
19 2008-01-25| 1330.61    215.06
20 2008-01-28   1353.96   206.52
21 2008-01-29      13623      208.8
22 2008-01-30   1355.81   2035                                          =
Ten   | 애서 | 0                            i (이                        0
5장 주식 엑셀 실습 69


===== PAGE 70 =====
2개 이상의 주가 비교를 위한 지수화 작업

8&0500에 비해 KOSPI200 지수의 값이 작아 KOSPI2002] 움직임이 잘 관찰되지 않습니다.
두 그래프를 함께 비교하기 위하여 두 지수를 2008-01-02의 지수를 기준(100)으로 하는 새
로운 지수로 바꾸겠습니다.

Ba"

@D, E 열에 새로운 지수를 만들기 위해 D1, E1 셀에 각각 s&P500, (>521200이라고
제목(헤더)을 달아줍니다:

@ S&P500 지수를 새로 만들기 위해 D2 셀에 =82/8$2*100이라고 수식을 입력합니다. 셀
의 줄번호/열번호 앞에 $를 붙이면 해당 행/열을 고정한다는 뜻입니다.

4|       ^               8              Cc       > Re

11 |         S&P500 | KOSPI200.1 S$&P500 |KOSPI200
2008-01-02      1447.16       eS | i)
3 | 2008-01-03     1447.16     234.6

Eas

() KOSPI200 지수 변환을 위해 D2 셀에서 [Ctri]+[C]S 눌러 BAS 하고 82 셀에서
[Ctra] +[V]S 눌러 붙여넣기합니다.

@ 마지막 행인 2017-12-929까지 수식을 채우기 위해 그림과 같이 D22} 82 셀을 선택하
고, 선택한 영역의 오른쪽 아래 있는 Aol] 마우스를 가져가 포인터 모양이 땐에서 +로
바뀌면 더블클릭합니다.

022    1 1: |, fe || =82/652110

4    A      8B. | le EE
1 |           S&P500 | KOSPI200

2008-01-02 | 1447.16      235.3]
/3 | 2008-01-03     1447.16     234.67
Ea 2NNR.01-0A       441162 ___72ㄷ77

© 다음 그림처럼 마지막 행까지 수식이 잘 채워진 것을 확인할 수 있습니다.

70 2% 주식과 지수



===== PAGE 71 =====
MH 15- @- =                   2_S&P500-KOSP1200 J
홈 ： 삽입 펙이지레이아웃 +4 데이터 Ae 보기
주 esas 이브 이가 가 ==Bo- 1 fee
불여기 , | 가 2 ~ 머- 소-가- W- SSesee B-|S
클립보드 ㅠ         글꼴         os      맞춤      te
| 62593 | : | Ea  AM fe | -<2593/629100
P= Al      B _ | c | oO (FRE fF
2575, 2017-12-04   2639.44   328.77 182.3876 139.7238
2576| 2017-12-05   2629.57   329.61 181.7055 140.0807
2577| 2017-12-06   2629.27   324.52 181.6848 137.9176
2578| 2017-12-07   2636.98   323.59 182.2176 137.5223
2579, 2017-12-08 |    2651.5    324.68 183.2209 137.9856
2580) 2017-12-11   2659.99   325.09 183.8076 138.1598
2581 2017-12-12 | 2664.11    324.07 184.0923 137.7263
2582. 2017-12-13   2662.85   326.18 184.0052 138.623
2583) 2017-12-14   2652.01   324.74 183.2562 138.011
2584) 2017-12-15   2675.81   326.23 184.9008 138.6443
2585 2017-12-18 | 2690.16    326.6 185.8924 138.8015
2586 2017-12-19] 2681.47    326.76 185.2919 138.8695
2587| 2017-12-20] 2679.25    325.79 185.1385 138.4573
2588, 2017-12-21   2684.57   319.72 185.5061 135.8776
2589 2017-12-22   2683.34   321.21 185.4211 136.5108
2590 2017-12-26    2680.5   318.89 185.2249 135.5249
2591 2017-12-27] 2682.62   320.25 185.3713 136.1028
2592 2017-12-28   2687.54   324.74 185.7113 138.011
： = 2017-12-29   2673.61    324.74 184.7487| 138.011]
2594|                                    [|
2595)
2596)
Pan   | sheett |  @
(238
이 데이터로 다시 차트를 그릴 것입니다.
0 마지막 셀인 £25930] 선택된 상태에서 [6108 1+[…]를 한 번 눌러 02593도 함께 선택
합니다.
(3) 두 Ao] 모두 선택된 상태에서 [041]+| 601 |+|[ ㅣ JS 눌러 맨 위 열까지 선택합니다.
(3) 이제 새로 변환한 지수인 D, ESO] 선택된 상태입니다. 앞에서 한 것처럼 차트를 삽입

해 새로운 그래

프를 그립니다. 결과는 다음과 같을 것입니다.

71


===== PAGE 72 =====
erage meee Se aR mea

OB ®&- 20 =      2_S&PSOO-KOSPI200 xisx - Excel         차트 도구
톰 2x 페이지 레이아웃 수색 데이터 we 보기 디자인 MA

wt  빠른 4a}      a      a     000             ea | =  ne oe
추가 레이아옥- ㆍ Oe     a          2      Sa     Pe OO
RE qos                                                      자르 스타일                                                       데이터
「   ^    8     (a    D    E    TG . a) sf
1 __|_s&Psoo | KOSPI200 1 S&PS00 |KOSPI200,              |
2 2008-01-02    1447.16      2353     100     100
3 2008-01-03    1447.16     234.67     100 99,73226
4 | 2008-01-04   1411.63   235.77] 97.54485 100.1997
5 2008-01-07    1416.18       231| 97.85926 98.17255             ;
6 | 2008-01-08     1390.19      230
7 2008-01-09] 1409.13    232                 차트 제목                 Iba
8 2008-01-10    1420.33    229 200                                             4
9 | 2008-01-11    1401.02    224 19                                            co
10 2008-01-14   1416.25   222i sen
11 | 2008-01-15    1380.95    220 120
12 2008-01-16    1373.2   210 뜨
13 2008-01-17    1333.25     218 6
14 2008-01-18    1325.19     219 4
15 2008-01-21] 1325.19      2 쓰
16 _2008-01-22    1310.5   cof) CORRE SRSRGRRESS STARR RAE SSR SS     |
17 2008-01-23    1338.6   207                소이 aes SS SS      |
18 _2008-01-24| 1352.07    21             Bee, cae
19 | 2008-01-25   1330.61    215.06] 91.94629 91.39822
20 | 2008-01-28    1353.96    206.52] 93.5598 87.76881
21 2008-01-29 |    13623      208.8] 94.1361 8873778
22. 2008-01-30| 1355.81    203.5| 93.68764 86.48534
Seren sheet!                                          ae
cae

두 그래프가 비교 가능한 수준으로 그려진 AS 볼 수 있습니다. 그런데 ※축에 날짜가 들어가
있지 않아 조금 이상해 보입니다. 차트를 그릴 때 날짜 열은 데이터로 선택하지 않았기 때문입
니다. ※축에 날짜를 표시해보겠습니다.

(07 ※축을 마우스로 선택한 후 오른클릭을 하면 나오는 팝업 메뉴 중 데이터선택 메뉴를 클
릭합니다

72 2 주식과 지수


===== PAGE 73 =====
=

5.06" 91.94629 91.39822 —

231 97.85926 9817255

차트 제목

삭제02)
스타일여 맞게 다시 BA

보조 눈금선 주가04)
SAAB

1 ㄷㄱ AICEOO O07 760014

@ '데이터 원본 선택'이라는 창이 새로 열립니다. '가로(항목) S 레이블에 있는

이콘을 클릭합니다.

데이터 원본 선택

자르 데이터 BHC): | Ssheett$D$1:$€$2593

BS ADO

 eam |, 27 행/열 saw | ~

가로(항목) 죽 ASO

범례

주가) |

62 편집@ |

× AIA

S&PS00
KOSPI200

i
Y

ene 셀/빈 셀00

[owe] | <

」

죽 레이블
룩 레이블 범위):

?   x

[is] eas

ae]

"데이터 원본 ey 창이 닫히면서 '축 레이블' 창이 열립니다.

5장 주식 엑셀 실습

73


===== PAGE 74 =====
@ 이제 날짜 셀 전체를 선택해야 합니다. 앞에서 한 것처럼 ^42를 먼저 선택하고
+| 804 1|+| | |를 눌러 날짜 셀 전체를 선택합니다. 선택한 뒤 `축 레이블 범위'에
=sheet1!$A$2:$A$25930]z2}31 표시되면 제대로 한 것입니다.

Ae                 수타
BAe BHA):

[Erenssosssossg) 66] wei es

[ 9 ] | |

6) 확인을 누르고 '데이터 원본 선택" 창에서도 확인 을 누르면 다음과 같이 차트에서 xs
에 날짜가 정상적으로 표시된 것을 확인할 수 있습니다.

차트 제목
200
180
160
140
120
100
80
60
40
20
0
oi   >  ay + $ $ +
Sul gt ae ‘in oe ee > > ~
ra £ SS 고 200  Se) oy) eh SN
126 26602":  샤 + 4 $
——SEP500 ———KOSP1200

이렇게 차트로 보면 2008년 9월 미국 금융 위기로 S&P5002} KOSPI200 지수가 폭락했다가
다시 상승하는 추세를 볼 수 있습니다. 그래프의 크기, 위치 등 디자인도 원하는 대로 조절할

수 있는데, 그래프를 선택하면 상단에 디자인 탭이 활성화되며 디자인 관련 기능을 사용할 수
있으니 참고하세요.

2_S&PS00-KOSP1200 xisx - Excel                    AE 도구
페이지 레이아웃     수식     데이터     검토     보기     디자인     서식
3         --                 —)      ~           = =:
주               ;
색 변경  we       Mar af     oe   ; 10“ a            ~ ]
추가 레이아웃    "       —    re eee er ne 0000 | 기
bent bbe                                                   자트 스타일

74  2부 주식과 지수



===== PAGE 75 =====
5.2 회귀분석을
이번에는

화되어 있지 않은 엑셀의 고급

© 엑셀의 상

위한

기능을

}단 메뉴에서 파일 ， 옵션 메뉴를

엑셀 환경 설점
회귀분석을 실습해보겠습니다. 엑셀에서 회귀분석을 하려면 엑셀 기본 설치 시 활성
먼저 활성화해야 합니다.

를 차례로 선택합니다.

@ 다음과 같이 Excel 옵션' 창이 열리면 왼쪽 메뉴에서 추가 기능 을 선택합니다. 화면 제

일 아래에 있는 '관리'에서 “Excel 추가 기능'이 선택된 상태에서 이동 HES

So 느로
otal

릅니다.

6606 을션                                                                                                                                    nb
열반                    fe Microsoft Office 주가 기능를 보고 관리합니다.                                                                    |
수식                                                                                                                                                  |
연어 교정                주가 기능
저장                       이를 ~                                               위지                                                플로           ^
연어                      활성 응용 프로그램 수가 기능                                                                                        더
ae                            분석 도구                                                      C#_ffice#Office 1 St#LibrarywAnalysisWANALYS32XLL Excel 주가 기능  |
=                         분석 S>-vBA                                        Ct_icewOffice | S#UbraryWAnalysis#ATPVBAEN XLAM | Excel 주가 기눔
리본 사용자 지정             유로화 도구                                                (\. 1050 Officer#Office 1 SwLibrary#EUROTOOLXLAM = Excel 주가 기동

R71 주가 기능                                C¥#_OfficetOffice 1 SitLibrary#SOLVERWSOLVERXLAM = Excel 주가 기눈
빠른 실형 도구 모음                                                                                                                  ‘|

MAAR oe       비훨성 응용 프로그램 주가 기능                                                                                       |

0.                  Actions Pane 3                                                                                        04 RES     4

| sor ey                       wR 00440)                                                     C:¥_n Filest#microsof sharedwSmart Tag#MOFLOUL 들작              A

|                                  날짜 (환국어 WR 인식자)                                  C:#_lest#microsoft sharedwSmart Tag#KSTRECOG OU SR              "

ㅣ                              사람 이를 (한국어 사람 이를 인식자)                     C¥_lest#microsoft sharedWSmart 739\<5706000.0 ㅣ: 동작            |

|                                 시간 (ERY 시간 연식자)                                  C¥#_les#microsoft sharedwSmart TagHKSTRECOGOLL SR              ”

|                               전파 번표 (한국어 전파 번호 인식자)                     C#_lest#microsoft sharedSmart 1391<5105000.01Ｌ 동작

|                  주소 (환국어 주소 인식자)                  C#_lestimicrosoft sharedWSmart TagWKSTRECOGOU SRR

|

|                           문서 관련 주가 ie

|                              BA BE #7 718 28

주가 기울: 분석 도구
게시자: Microsoft Corporation
=ng Ens 정보 없음                                                                                           |
|                              위지:       (C:#Program Files              Rt OfficewOffice!S                       S32 XLt                                  ㅣ
|                                                                                                                                                       |
|                               설명:       BA 및 연지니어림 BAS GE 분석 SPH 제공합니다.                                                            |
|                             =             eee SRS -:                a>                 내             |
|                                                                                                                                                       |
|                            Baa: [660 주가기능 |] | 이동@1- |                                                                               |

|                                                                                                                                                       ㅣ

  [Vas]
Ss        느 &                          으                y,                     츠          Wo =          스 Oo)            으
(3) `추가 기능' 창이 열리면 다음 그림과 같이 엑셀에 추가 기능을 추가할 수 있습니다. 우선

'분석 도구'만 추가하면 회귀분석을 할 수 있습니다. 나머지 기능은 필요에 따라 선택하

세요. '분석 도구'에 체크하고 확인 을 누릅니다.

5장주식 엑셀실습 75


===== PAGE 76 =====
i.

96 PETS

ier

;                 주가 기능            ?7 ※×
!                                                    사용 가능한 추가 기능(4):
:                                  -   a
HE ee)      [도
넌유로화 도구          me
|                                              더해 찾기 주가 기능
찾아보기@)ㅡ…
자등화00)…

분석 도구

통계 및 엔지니어링 BAS 데이터 분석 도구를
제공합니다.

회귀분석을 위한 엑셀 추가 기능 설치가 완료되었습니다.

이제 엑셀로 회귀분석을 할 수 있습니다.
0) 상단 메뉴에서 데이터 ， 데이터 분석 을 차례로 클릭합니다.

M8%:-ec-:     2.SBPS00-KOSPI200 xisx - Excel      자드 도구                 ? 8 - 8 ×
를 상업 . 페이지레이아옷 수식 결로 보기 디자연 서식                    ‘Yong Whoan Kim-M16 -
a    Py, Ses    기 ie  Y 개 지우기    < se nr     et     is -     cs   yen
Bm 데이터 ake Bias    "  am  ge CONS |, Heme 항목 재거        석~ | @iAgay ㆍ 3
가페오기 교절- Qeseu;* ~    Yas   나누기 SWI 유효성 검사 - eB    ves
ae                    정렬 더 될더                           데이터 도구                      eRe. 분석
mse tix YY fr
ade. SNe eel 69900 ORD     Erode AF     6   H    I    1 가 엘자     L    _M
1}          S&PSOO |                                                    [+
2 _2008-01-02     1447.16                              차트 제목                              =
3 2008-01-03] 1447.16,                              12
4 2008-01-04  1411.63                                “<=
|         i”                                            }
5 2008-01-07| 1416.18! ml                               ly]
6 2008.01-08| — 1390.19)
7 2008-07-09] 1409.3) ed
8 2008-01-10    142033) 3?
Jy                   9 "2008-01-11|  140102| 19
4                        10 2008-01-14   141625, «©
14                     11 _2008-01-15   138095| “%
회
.
iy.
i

76 2 주식과 지수



===== PAGE 77 =====
@ '통계 데이터 분석' 창이 열리면 회귀 분석' 메뉴를 선택하고 Se

[은
ttlo
af
때
a
a

$A 데이터 분석                                      ?      ×
분석 도구(&
의                                  -
Le  As
£2)

등분산 가정 두집단
|분산 가정 두집단                        !
: 평균에 대한 두집단

(3) `회귀 247 창이 열리면 YS 입력 BST} KOSP1200 데이터 범위를, XS 입력 범위'에
s&P500 데이터 WAS 입력합니다. 이 메뉴에서는 [Ct] HES 이용한 선택 기능이
작동하지 않으므로 마우스로 선택하거나 범위를 키보드로 직접 쳐서 입력합니다. 입력
이 완료되면 확인 버튼을 클릭해 회귀분석을 시작합니다.

회귀 분석                                                 ?
입력
VS 입력 visio:           |56525652593 Es      도
처소 |
X& 입력 범위00:           |50525052593 Es]      OBE
| 도움말) |

x

확인

[| 이름표)              [| 상수에 0을 사용(0)
[신뢰 수준@6         195 _ |1%

플력 옵션

( 출력 범위(0):              부 폴스 Be
© 새로운 워크시트(8):       eae:            =
(- 새로운 Be 2

잔차

Cate)                            CL 잔차도(@)
(Be 잔차)                    DO 선적합도0)

정규 확률
[ 정규 확률도04)

@ 엑셀이 회귀분석을 수행하고 다음과 같이 BAS 돌려줍니다.

5장주식 엑셀실습 77


===== PAGE 78 =====
ee ee

@Q@%-c-s:               2_SRPSOO-KOSPI200 alsa - Excel                706 - 56 x
8     삽입     BAT BS     수식     데이터     걸도     보기                                                                    Yong Whoan Kim-M16 =

소오 시 |
a                                       5                   "|G ys    7

69072 ava: G- 으-크- 맥- eemen S- 만-% wa @ucas- Bax- | 이 우리 22%

furs «     글들      년   ze   5» BABY nn sey    r    eu    ^

a   ~ tix YY fe 229s                                 v

Ai A  j  8    CEN pp t0s 2)  E  812  i  (Fe  H  {  1  oS

122 85

2

3    회귀분석 sav

4 48 상관계수     0.722257477
5
6 조정된결정계수  0.521471175

7 표준 오차        10.66044355

6 Bao           2592

9 ‘

10 분산 분석

11                      자유도        제급한       제급 평근        『비         유의한 【
12 회귀                    1  320991.8105 320991.8105 2824511858          0
13 잔차                 2590  _294340.697  113.6450568

14 계                  2591  615332.5075

계수        표준 오차      1 동계링         『-값        하위 95%     상위 95%     하위 95.0% 상위 95.0%
0.731135751 90.85957242            0 6499701196  67.8643514 64.99701196 67.8643514
0   0321715963   0.39606904   03217154631   (easel,

Wai   TE             q   ,

위 회귀분석 결과를 해석해봅시다. 두 지수 간의 추세선 식에서 기울기는 x12] 계수로 표시된
0.33이고, 절편은 66.43입니다. 즉, 추세선의 방정식은 = 0.33~+ 66.43 입니다. "(결정
계수)는 0.52로, 이 추세선의 EAS UEP AU ch

추세선 그래프 그리기

추세선 그래프를 그리기 위해 두 지수의 그래프를 새로 그려보겠습니다. 앞에서는 aoa 그
래프로 지수를 표현했지만, 이번에는 분산형 그래프로 두 지수 간의 상관관계를 표현해보겠습
니다.

DD, E 열의 데이터를 선택한 뒤 그래프를 그리기 위해 삽입 > 분산형 을 선택합니다.

78  2부 주식과 지수



===== PAGE 79 =====
rx i] BH 6- @-:                    2_S&P500-KOSPI200 xlsx - Excel

홈 MOM oie 4 IE
nia    ro)   |          10208 |              by Be &-       |               |
  © (EGS Gyo ess | ale ay im
피벗 주전     ag 온라인 이    bea >| 조리 os      피벗자르 Ase = en gw
테이블 피벗 EGO] gE        그림 a+”         xe DD         인           00

표        | 일러스트레이션 주가 기능                           :파크라인
62593        11× < fll | =02593/60525100 00        nS  \J  고 ae
세보 2      B     G                          ae 아게!
1            s&Ps00 | KosPI200 | S&P           “i
2 | 2008-01-02| 1447.16                '         8 | 고란
3 | 2008-01-03   1447.16                 거품형 -  값 집합 또는 데이터 we 두 개
4 | 2008-01-04   1411.63                  | 이상 비크합니다.
5 | 2008-01-07| 1416.18                  Ss | waste *
6 | 2008-01-08   1390.19                   지으 제
7 | 2008-01-09    1409.13                     : 다로 Roem 서로 다른 즉정감를
8 | 2008-01-10    1420.33                         GEHSUICE
9 | 2008-01-11     1401.02                                 on          porn

완성된 그래프 위의 아무 점이나 선택하고 오른클릭한 후 추써선추가 메뉴를

클릭합니다.

[
iy                         KOSP1I200
160                                        S|
「
|                    -  로  aa
|
F 120                     -
              2 a AAG “Kospize ~|
ey                  재우기 은곽선
-                    a
!                   삭제2) |   [
ee                 (4G) 스타일에 맞게 다시 Esa
Nee |                               ll ASE 증류 변경00…
' 60                 ace 데이터 선택
| 40 |
「   ㅣ
ㅣ
|   |                                      |
!  0      50     100     150     200 |

추세선 그래프가 일단 그려지고, 오른쪽에 추세선 관련 메뉴가 표시됩니다. 아래쪽에서
4A} & 차트에 표시'와 #-제곱 WS 차트에 표시 를 선택하면 추세선과 함께 방정식과
R? Zo] 차트에 표시됩니다.

5장 주식 엑셀 실습 79


===== PAGE 80 =====
김에 개제

Rss 1 1× Y fe                                                                                                    ~
= ah      an   '    as r                                                                   ™*x
2 2008-01-02  14

3 2008-01-03   4 10

4 2008-01-04  14

5 _2008-01-07   14 se

6 2008-01-08  13
7 2008-01-09  1a

8 2008-01-10  14

9 2008-01-11   14

10 2008-01-14   16”

11 2008-01-15] 13

12 2008-01-16   1“

13 2008-01-17   13

14 2008-01-18   13 =

15 2008-01-21   13                                                       :

16 2008-01-22    1 2                                                     -

17 2008-01-23    1                                   |

¥ 003 01. 24   3 »                                  |      + AEB)       선형 000601200)

19 _2008-01-                                          |

20/ 2008-01-28] 13                                 |     ae

1 2008-01-29   }

3 2008-01-30   13  는      2      =      12094.     알으로)      00   구간

23 _2008.01-31   137855   207.77 9525899 8830004                     뒤도@)        00    구간

24 2008-02-01   1395.42   209.08 96.42472 8885578                     BBS)        aa.

25 2008-02-04   1380.82   21623 9541585 91.89545

26 2008-02-05] 133664 21691 9236297 9218445                     hth eet)

77 7000.07. | 3226 46   71ㄴㅁㄴ 01ㅅ004 0710446                ~   VRAS 같을 REA BAIR       때
< 0?   Sheev  sheet?              oo       ae     >

@ 추세선이 눈에 잘 띄지 않는다면 디자인 메뉴에서 색, 두께를 바꿔봅시다. 다음 그림은
예시입니다.

자트 5     111× v fe                                     i                                                      ~
4    A      8      ¢c      D     E     F     6     Hf]

1. | sac     aa      .     _ 추세선 서식           Aik
2 2008-01-02| 14                KOSPi200                    Sian
3 2008-01-03] 14 1                               i)
4 2008-01-04] 14                                      [o] 2 Wi
5 2008-01-07] 14 ss
6 2008-01-08   13                                        시저
7 2008-01-09   느 이                                           S800
8 2008-01-10] 14                                       *실선의
9 . 2008-01-71   14                                               선선
10 2008-01-14] 14 ™                                             구노 =
11 2008-01-15) 13                                    -   -
12 2008-01-16   1                               CTs)
13. 2008-01-17| 13                                             2c!
14 2008-01-18] 13 w
15 2008-01-21   3                                     두게
16 2008-01-22     1 46                                                |        Be BHO              |x |
17 2008-01-23   1                                |
16. 2008-01-24] 13                                 GN BAD          x
19 2008-01-25) 13                                             을 모양 Ea       {ae -
20 2008-01-28   13                                     연결점 ERY        원형 ㆍ
이 eae 이 29      투     [것             ^            100            150           200             화살표 더리 유청)            | rie
23 2008-01-31]  137855    207.77 95.25899 6830004                 {     Hee 더리 크기(99        를*
24 2008-02-01   1395.42   209.06 9642472 8885678
25° 2008-02-04] 138022 21623 -95.41585 9189545                      가주       me
26 2008-02-05] 133664    21691 9236297 9218445                          화살표 꼬리 크기00)         를.
77 20a?   7ㄱㅋㅋ   71601 01004 OF 10446               -

Ee    Sheet2 | sheet    ®           i 1이   :     >

실습을 마친 결과 예시 파일은 05.3. S&P5@0-KOSPI200 (실습결과 ) .×15×입니다.

80 24 주식과 지수


===== PAGE 81 =====
5.4 K5 지수 산출

이제 조금 수준을 높여보겠습니다. A, B,C, D,  5개의 종목으로 구성된 5 ASS 산출하
겠습니다. 여기서 만든 KS 지수 데이터셋은 향후 선물 및 펀드를 살펴볼 때도 계속해서 사용
하게 됩니다.

5 지수 산출은 미리 준비된 데이터 없이 빈 엑셀 파일에서 시작합니다. Ay 엑셀 파일을 하나
만들고 파일명을 05.4. KS Index.xlsx™ 저장합니다.

종목 기본정보 만들기
지수 산출을 위해 필요한 주식의 기본정보를 생성하겠습니다.

OAE 이름에서 오른클릭을 하면 나오는 팝업 메뉴에서 이를 바꾸키 를 클릭해서 시트 이
름을 `종목 기본정보'로 바꿔줍니다.

8 4

9 |

10

11

12                    |                   |
13 |                   |@] 코드 S710
14                    (ER 시트 See
15 |    랩 AR         ㆍ
16)                      | 8771
Bs                      | 모든시트선택61 |

4 >   | SS 71E3= yw

@ 1열에는 종목명, 2열에는 상장주식 수, 3열에는 유동비율을 입력하겠습니다. 그림과 같
이 입력합니다. 종목명이 들어 있는 행은 색을 변경해서 제목 느낌을 줬습니다.

2 | 상장주식수

유동비율             75%                90%               82%                88%                50%

5장 주식 엑셀 실습 81


===== PAGE 82 =====
Sent REE ee ae 가

a ee ag te re mr 이

상장주식 수와 유동비율, 주가 수준의 차이에 따라 종목 하나하나가 지수에 얼마나 많은 영향

을 미치는지 보기 위하여 각 종목 정보별로 차이를 둔 것입니다. 이 책 그대로 따라서 입력해
도 되고 원한다면 다른 수치를 입력해도 무관합니다.

현실에서는 종목명과 상장주식 수는 상장 기업이 정하고, 유동비율은 거래소가 공시 정보 등

을 참고해 실제 유통되는 주식 수를 파악하여 수시로 조정합니다.

일자별 주가 만들기
주가는 예측할 수 없는 방향으로 매일매일 변하죠. 마치 실제 데이터처럼 주가가 매일 랜덤으
로 변화하도록 데이터셋을 만들어보겠습니다.
OA 시트를 만들고 시트 이름을 '일자별 주가"로 wey,
@ YAS A 열에 입력할 것입니다. ar 셀에 '일자"라고 입력합니다.
종목 기본정보' 시트에서 종목명을 복사해서 B1~F1 셀에 붙여넣기합니다.

| BS 기본정보 | 일자별 주가 | ©

0) 42에 1을 입력합니다. 물론 실제 날짜를 입력해도 좋지만 주가와 지수에 좀 더 집중하
기 위해 첫째 날, 둘째 날, 셋째 날 개념으로 1, 2, 3 식으로 숫자를 넣겠습니다.

© 1년간의 데이터 생성을 위해, 다음엔 43, ^4에 2, 3을 입력합니다.

© 이제 A2~A4S 선택한 상태에서 오른쪽 아래 생기는 점에
마우스를 갖다 대면 포인터 모양이 때에서 += BAU CH.

82 2% 주식과 지수



===== PAGE 83 =====
© 그 상태에서 마우스를 클릭한 채 드래그해서 253행까지 끌어내리면 252일까지 날짜 데
이터가 채워집니다. 보통 금융공학에서는 1년을 250일 정도로 잡는데, 이는 1년 중 주
말과 공휴일을 제외한 트레이딩 데이의 날짜 수에 해당합니다. 이 책에서는 분기별 선물
옵션 만기 등을 처리하기 위하여 계산 편의상 1년을 4의 배수인 252일로 잡겠습니다.

® 시작일 주가 ASS 위해 B2~F2 셀에 10000, 20000, 30000, 100000, 10000002] 값
을 넣습니다.

@ 이제 랜덤으로 주가가 변하도록 설정하겠습니다. 83 WS 선택한 다음, 수식에
=RANDBETWEEN (B2*@.97, 62*1.033 )이라고 입력합니다.

83   +t | ~ 6 -ranoseTween(s2°0.97, 82°1.033) |

R
시: =

^전자

:    Baa ㅣ coz! ㅣ 0화학  엔터
{  110,000 20000 30000 100000 . 1.000.000
| ] 10097!
3

RANDBETWEEN 함수

* 엑셀의 RANDBETWEEN(X, y) 함수는 ×와 \ 사이에서 랜덤한 값을 출력하는 함수입니다.

* B2~F2 아래에 있는 값들은 랜덤하게 생성되기 때문에 책에 인쇄된 값과는 다르게 보이는 것이 정상입
니다.

* 여기에서는 하한값에 0.097, 상한값에 1.033을 곱해 당일 주가가 전일보다 -3%에서 +3.3% 사이에서
움직이게 세팅했습니다. 화폐 SSS 지속적으로 증가해웠고, 실제로 주가는 우상향 추세이기에 \에 조금
높은 값을 주었습니다.

5장주식 엑셀실습 83


===== PAGE 84 =====
00 B3 AS 선택하고 오른쪽 아래 생기는 점에 마우스를 갖다 대면 포인터 모양이 때에서
+로 바꿔니다. 그 상태에서 마우스를 클릭한 A 드래그해서 『3 셀까지 수식을 복사해서
넣습니다.

00 252일까지 주가를 채우겠습니다. B3~F3 AS 선택한 후 오른쪽 아래 생기는 점에 마
우스를 갖다 대면 포인터 모양이 땐에서 += BPAUCH.

09 이 상태에서 마우스를 더블클릭하면 252일까지 자동으로 데이터가 채워집니다.

K5 지수 만들기
KOSPI200& 만드는 방법과 동일한 유동 시가총액 방식을 이용해 5 지수를 만들겠습니다.
기본 공식은 다음과 같습니다.

a _ 비교 시점 시가총액 .,

기준 시점 시가총액 1

(시가총액= 주가×상장주식 수×유동비율 )
지수 산출을 위한 사전 작업으로 일자별 시가총액을 계산합니다.
0 새 ASS 만들고 이름을 '일자별 시가총약'으로 바꿔줍니다.
© A 행에 일자(41), $29 (B1~F1), 합계(01), 지수(811)를 입력합니다.
@ 42에 1을 입력합니다. 일자는 일자별 주가 시트에서와 마찬가지로 첫째 날, 둘째 날 개
념으로 1, 2, 3, …의 숫자를 넣겠습니다.
@ 1년간의 데이터 생성을 위해 43, Adel 2, 3을 입력합니다.
6) 42~44를 함께 선택한 후 오른쪽 아래 생기는 점에 마우스를 갖다 대면 포인터 모양이
Sol] +2 UHC}, 그 상태에서 마우스를 클릭한 채 드래그해서 253행까지 끌어내

84  2부 주식과 지수


===== PAGE 85 =====
Le

52일까지 날짜 데이터가 채워집니다.

© AFA] 1일 차 시가총액을 계산합니다. 22 셀을 선택해 수식에 =" 일자별 주가'!82*'
기본정보' !8$2*' 종목 기본정보' !893을 입력합니다. 시가총액은 (주가×상장주식
수×유등비율로 계산하는데 주가는 “일자별 주개: 시트에, AA] 수와 유등비율은
종목 기본정보" 시트에 들어 있으므로 이를 참조해서 계산한 것입니다.

가

«> | 종목 기본정보 | 일자별 주가 | 일자별 시가종역 | ©        : 김6=

택하고 상단 메뉴에서 자동 합계 버튼인 | 버튼을 클릭하거나, |] 버튼
클릭 후 팝업 메뉴에서 메뉴를 클릭하면 G2 셀에 1일 차의 KS
지수 구성종목 전체의 시가총액이 계산되어 나옵니다(62 Aol] =SUM (82:【『2)라는 수
식이 자동으로 입력됩니다).

태니: ~               2KS_Indexxisx - Excel                2 60
SSR 2 ue 페이지려이아웃 . 수식 go BS 보기           __Yoog Whoan Kin-M16, =
7      =               ㅣ       녁         Ape | Sle a  ㆍ
을 * fears      11 -j47|/=Blao- |e |=    Dimi  0     =    -
J  fa -           -  -    ㅣ        j   TH. ue     }-      ㆍ
아아아 어느 으아 오이 aye | 으으 ates | See wa een
ae        던요    a~ | =   = ts    3 3   Besee- | 63 서식 -    영근
gave <       글꼴 으으으 ator te    28    6) BABA ol See     셀 i 숫자게수이   ^
82       09270 fe |) BE 주가'182"'중목 기본징보'1652"'중목 기본정보'1853              | 39200
죄소같0
AOA   8     c     D     E     『      6   ib
=                              기타 BSH

(9) 지수 AALS 위해 H2 셀을 선택하고 수식 =62/6$2*100을 입력합니다.

ate, = [-)

F          |            G
엔터                        합계                    1+ 벨르
)00,000,000       1,245,000,000,000             100  |

5장 주식 엑셀 실습 85


===== PAGE 86 =====
00 지수를 소수점 둘째 자리까지 표시하기 위해 홈 탭 아래 표시형식 섹션의 .000 아이

콘을 두 번 클릭합니다.

= 조건부 서식- ㅣ Eewa - | > ~ zr
G- %  fy 표 서식 -  , 8 삭제 - | 90 - dhe

=    00 셜 스타일 ~ ae 10

|
a BABA ㅠ 스타일      | By   a

mrs ~ 세! =62/0$2*100

@ 252일까지 지수를 채우는 것은 이제 익숙할 겁니다. B2~H2S 함께 선택한 후 오른쪽
아래 생기는 진이 PAG 갖다 대던 포인터 모양이 Gaya += 바낌니다. 이 상태에
서 마우스를 더블클릭하면 252일까지 자동으로 데이터가 채워집니다.

지수 그래프 그리기
생성된 지수를 그래프로 그려보겠습니다.
© 지수 데이터가 들어 있는 42~11253 셀을 선택합니다.
3) 상단 메뉴의 삽입 YS 선택한 후 WSHH 아이콘을 선택합니다. 다음과 같이 지수 그

래프가 그려집니다.
@M8o-° =          eae a 7 2  7”  a2) mie 80 x
om Bue ㅣ 페이지레이아웃. 수식 데이터 ae 모기 ~      Yong Whoan Kim-M16 -

버 i 터우 ace | ie 가우 a iy   ae
au   a Ware aue-  | 주전 5    피버 까르 MOMMY | ef  | 율라이서 ya OPE 리스트 기표
aoe ae aoe       AS            자르 2a Se                        00                            tary

cane) fF   ” ergo  _ 스파크라인 ot  EES ^ | |}
VE 22 ^  |  i    F    !     6     ~ 서  ae

밀자
2 1 _75,000,000,000  90.000000.000 49 ny pene     )00 500,000,000,000  1.245.000000.000 | 100.00   leg
3.  2 75,337,500,000  91,782,000.000 49 ㅣ        7200 513.914.500.000  1,270,761,520,000       pet
4 3 73.147.500000  90.616.500000 49. KY        900 525,984,000,000 _1,276,232,640,000
S| 4 73,260,000,000  88.632(     .        |          359,000,000
6  5 73,372,500,000  88.375.5      는 다른 국은션령자트041 짝             152,940,000
7 6 74032.500000 90.873, 11500                              )03.420.000
8  7 75757.500000  92.880(                          140.820.000
900 6 74340000000 93946                          108,920,000
10 00 9 76,102,500,000 91,651, 205.00                           {62,340,000
개 10 74,212,500,000 93,596,   Ny                    ‘31,100,000
2 11 0 75112.900.000 __ 959896 °°                              195.820.000.

86  <부 주식과 지수


===== PAGE 87 =====
@ 그래프의 축이 0부터 시작되어 지수의 움직임이 두드러져 보이지 않습니다. 지수 움직
임을 눈에 띄게 표현하기 위하여 YS AHS 80으로 바꾸겠습니다. 그래프의 yao
선택하고 오른클릭을 하면 나오는 팝업 메뉴 중 축 서식 을 선택합니다.

M@aeo-c -
를 22

페이지 려이아옷

2KS_indexxisx - Excet
x 수식

4
1

2 | 1 75,000,000,000
3 2  76,792,500,000
4| 3 76,650,000,000
5| 4 75,262,500,000
6 5 75.285000000
7} 6 77.385000.000
8 7 _75,240,000,000
9 8 _76,005,000,000
10' 9 77,640,000,000
11: 10 77,002,500,000
12} 11 74,925,000,000
13. 12 76,117,500,000
14. 13 _75,780,000,000
1S! 14 73,867,500,000
16 15 74,302,500,000
17  16 74,932,500,000
19 17 74.730.000.000
19. 18 75.495.000.000
2  19 75,352,500,000

88,510,500,000
88,695,000,000

io ke    중독 기본정보 ㅣ 일자별 주가 | 영자별 시가중역 |

자르 도구

 결로       . 디자인 : 서식

데이터     보기       시 08 s

eee NA LAN NK

자르 스타일

- WE 데이터 AREER 자르
전환 선택 | 변경 | 이동
중류 ㅣ 위지

데이터

492,000,000,000  88,000,000.000 500.000.000.000
506,924,000,000  88,732,160,000 492,050,500,000  1.254.850.160,000 100.79
사은          40,000 _487,558,000,000 _1,241,547,540,000      99,72
= MEQ ㅋ -                                 140,000 = 101.14
재우기 용곽션        ㅡ제목                  363,300,000 101.47
「                                                                                               )14“ 0,000          99.83
AAD                                               17££70,000      99.31
3 스타일여 앗게 다시 설정(4)   pee ae  16: 0,000     99.23
y FEO                                               120,380,000 101.20

때 SOE BUD

145,340,000 104.37
330,560,000 103.12
|23,580,000  103.62
345,000,000 104.78
HSASERSRSAAREA 185940000 105.17
「         )       1000 517.883.000.000  1.284.321.380.000  103.16
512.254.000.000  96.858.080.000 524,333,500,000  1.297.451,080.000 104.21
103.43

507,120.600,000  96,.548,320.000 519,968,500,000

1,287,685, 120,000

3

|
ㅣ
|

6 오른쪽에 나타나는 `축 서삭'에서 ‘BABES 선택하여 값을 80으로 바꾸고 [Enter] S +

릅니다.

|                                           =
【                 ㅁ         ;         E                  Es]
eS          6증권          화학          eq) | 죽 서식                       ~
000,000 492,000,000,000  88,000,000,000 | 500,000,     숙 옵션 ＊ ㅣ텍스트 옵선
000,000 506,924,000,000  88,732,160,000  492,050,5              해
500,000 498,002.400,000 _89,872,640,000 _487,558,¢     Oo 2
(
9                           차트 제목                 4554                            시
5 20000                            경계                 | |
¢                                 최소값 다시 설정 | |

180.00                                                                 a Te
C                                                 죄대갖     | 2000 |  자동
5160.00                                         Sa            |
(                                                단위          …             |
( 140.00                                    주      | 200   E ㅣ  자동     |
6. 12000                                            보조      140 os      |
ㄷ                                                                 ——          |
1100.00                                           가로 죽 교자
                                            Lie) AEE/O)

5장 주식 엑셀 실습 87


===== PAGE 88 =====
© 다음과 같이 지수의 움직임이 잘 보이는 그래프로 바뀌었습니다.

차트 제목

180.00

140.00

100.00

지금까지 가상의 5개 종목으로 구성된 KS 지수를 만들어보았습니다. 우리가 주가를 랜덤으로
움직이도록 설정해놓았기 때문에 주가와 지수, 그래프 모양은 항상 다르게 나옵니다. 책처럼
나오지 않는 것이 정상입니다.

실습을 마친 결과 예시 파일은 05.4. KS Index (실습결과-데이터고정) .×15×입니다.

88  2부 주식과 지수


===== PAGE 89 =====
려   DY                                 Chapter 6

여기에서는 금융공학 파이썬 모델링에 필요한 파이썬 기초 SYS 익혀보겠습니다. 프로그래
밍 언어도 한국어, 영어, 중국어와 같은 언어인지라 같은 의미를 전달하는 데에 서로 다른 다
양한 HAS 사용할 수 있습니다. 이 WL 초보자들이 쉽게 파이썬을 익힐 수 있도록 가장 파
이썬다운 기본 방범을 안내합니다. 학창 시절 공부한 영문법 책으로 비유하자면, '기본영어'나
'종합영어'가 아닌 '기초영어"라고 할 수 있겠네요.

아직 프로그래밍을 한 번도 경혐해보지 못한 분이라면 책 마지막 부분 부록에 있는 파이썬 기
본 문법을 먼저 읽어보기 바랍니다.

}

0

«1
(function = 특정한 기능을 수행하는 공장 같은 것입니다. 중고등학교 때 배운 함수와
개넘이 같습니다. f(x) =ㅜ+1 이라는 함수가 있을 때, 이 함수에 어떤 값을 넣으면 1을 더해
서 돌려주는 기능을 수행합니다. 이와 동일한 개념이 프로그래밍에서도 적용되며, 이러한 함
수를 만드는 법을 살펴볼 것입니다. 물론 함수를 만들어서 한 번만 쓰고 말 것이라면 굳이 함
수로 만들 필요가 없겠죠? 함수는 동일한 기능을 여러 번 사용할 경우에 쓰는 것이 효과적입
니다.

함수는 06*라는 명령어로 생성합니다.

a
LET

i

63 코딩 기술: 파이썬 고 89


===== PAGE 90 =====
def 함수명(인수, 인수, ...):
# 함수 기능
return 반환값

J (x)=x4+1 2h 함수. 즉 어떤 수를 주면 거기에 1을 더하는 함수를 만들어보겠습니다.

1 def f(x):
2     y=x+1 ##x= 함수를 호줄받을 때 AALS 인수이다
3     return y

Out

코드를 처음 입력해보는 독자를 위해 부연하겠습니다. 위의 HEE 1~3행까지 한 줄마다 하
나의 명령을 입력하고 [60@71를 처서 다음 줄로 이동하고, 전체를 다 입력했으면 (Shit]+
[enter] S 눌러 지금까지 입력한 코드 전체를 실행한다는 의미입니다. SAS 대신 04『이라
표시한 마지막 행은 셀을 실행했을 때 출력되는 결과를 뜻합니다. 위 코드는 함수를 정의하
기만 했을 뿐 실제로 출력할 내용은 없으므로 출력 결과가 비어 있습니다.

그럼 함수를 정의했으니 한번 실행해볼까요?

개

1 (1)  # 함수를 호출하고 1을 인수로 전달해 AAs 달라고 요청한다
Out 2

./ ㅇ」 를 떠올려봅시다. 같은 함수를 두 번 호출하는 것이지요. 프로그래밍으로도 가능합니다.

1 f(f(1)) # fof
Out 3

함수보다 2 개념으로 SeA(class)7} 있고, 클래스보다 더 큰 개념으로 모듈(0200416)이
있습니다. 모듈은 파이썬 프로그램 단위로 생성됩니다. 즉, {116.0\라는 파일이 +116이라는
모듈이 됩니다. file.py 프로그램 내에 여러 개의 클래스가 있을 수 있고, 클래스 내에는 oF
러 개의 함수가 있을 수 있습니다.

90 2% 주식과 지수


===== PAGE 91 =====
6.2 외부 모듈 사용

파이썬은 금융분석, 빅데이터, 머신러닝을 위한 가장 쉽고 강력한 언어라고 알려져 있습니다.
이러한 분야에서 파이썬이 각광을 받게 된 가장 큰 이유는 데이터의 수집과 분석을 위해 여러
개발자가 만들어서 공유한 풍부한 라이브러리가 있기 때문입니다. eo] Az] (library) 여
러 개의 3S (module) = 구성되고, 모듈 내에는 다시 여러 개의 클래스와 함수가 들어 있습
니다. 외부 라이브러리의 기능을 사용하려면 우선 필요한 라이브러리를 설치하고, 그 라이브
러리 중 원하는 함수가 들어 있는 모듈을 호출(임포트)해야 합니다.

우리는 아나콘다를 사용하기 때문에 라이브러리의 설치와 관리를 쉽게 할 수 있습니다. 아나
콘다가 알아서 라이브러리 간의 의존 관계를 관리하고 설치할 라이브러리의 버전을 관리해주
기 때문입니다. 라이브러리의 설치도 아나콘다 내비게이터에 있는 Environments 메뉴를 선
택한 후 클릭 몇 번만으로 쉽게 할 수 있습니다.

다음 그림은 Environments 를 클릭해서 들어간 모습입니다. 화면을 열면 현재 설치된 라이브
러리 목록이 나옵니다.

© Anaconda Navigator                                                                                                                                    = ㅁ8 ×
| Ue

©) ANACONDA NAVIGATOR                                                                     Sin ta Anaconda Cine]
aia      a Ss    | (Oat) …--6922200
@ 다예      pus         >       Nome     ㄱㅠ Oescripcon                        Vervon  i
@ Lora jar be. CO                                   aro
GB Projects eta)                         a    6     a                         제
A Learning                           1 anxenes    °                                sar
2K Community                          =        Ors                             =
2 anaconda project CO) Reproducible, executable project Grectories                 ono
1G asicryeto    © AA! pares ond vertatizer                       e220
© Qawos     © Abstract syntax tee fer python wth inference sappert              res)
2 이어     O Community devvioped python leary fer astronomy              202
Tl badet      O veins           python                280
떠나    °                                1
come                          dedoorssmnis. O                                tae
Deretoger Blog                                  2           On                =~                       =
irene                          @ buney     © Utter representation of arrays of boolean -¢ extension            oar

상단 드롭다운 메뉴를 이용하면 설치가 et Sl (Not installed) FS 업데이트
(Upgradable) 라이브러리를 쉽게 검색하고 설치할 수 있습니다.

N
or
(원

6장 코딩 기술: 파이썬 기초 91


===== PAGE 92 =====
Installed                         ¥
7 Installed

Not installed
Upgradable
Selected                   |

All

아나콘다를 사용하지 않는 경우에는 여러 가지 모듈 간의 상호 의존성 때문에 충돌이 날 수 2)
으니 주의가 필요합니다. 아나콘다 대신 ㅁ깨라는 파이썬 라이브러리 관리 프로그램을 이용할
수도 있지만, 이 책에서는 설명하지 않습니다.

외부 BSS 가져올 때는 import SSS BAS 이용하는데, 몇 가지 변형이 있습니다.

모듈이 여러 개 들어 있는 라이브러리에서 특정 모듈만을 호출(임포트)할 WE import 라이브
러리명. 모듈명을 사용합니다. 모듈에 있는 특정 함수만을 호출할 GE from 모듈명 1700「 함
수명을 사용합니다. 컴퓨터 메모리를 효율적으로 사용하기 위해, 즉 불필요한 1100「+를 최소
화하기 위해서입니다. 또한 긴 BSS 줄여서 부르기 위해 asS 사용하기도 합니다.

import 054  # bs42}= 외부 OSS 가져온다

# urllibe}= 라이브러리 내의 request 모듈에 있는 urlopen 함수를 가져온다
from urllib.request import urlopen

a nN fF W N =

import pandas as pd   # ride 모율을 00라는 a= 기거 0

Out

92 2% 주식과 지수



===== PAGE 93 =====
6.3 빅데이터의 시작 뷰티플 수프

뷰티플 + (Beautiful 5040)는 인터넷상에서 데이터를 수집할 때 유용하게 사용되는 파이
썬 패키지입니다. 211"4Ｌ이나 XML® 작성된 파일을 가져오고(6411), Us 451 (navigate
and search), 분석하는([62756) 기능을 담고 있습니다.

여기에서는 뷰티플 수프의 여러 기능 중에서 우리에게 필요한 기능을 알아보겠습니다. 이번
절에서 배운 내용은 다음 장에서 실제 웹사이트 데이터를 가져올 때 기초가 됩니다.

크롬 브라우저를 열어 http://book. finterstellar.com/sample.htmlo] 접속합니다.
실습을 위해 필자가 제작한 아주 간단한 예제 사이트입니다. 이 사이트에 있는 내용을 Hols
니 4명의 팀원 이름을 보여주고 있네요.

<     (G} KO) book.finterstellar.com/sample.htm!          tr |  :

The Office

In my office, there are four officers, YW, JK, YJ and KS .

웹 페이지 빈 곳에 마우스를 가져가 오른클릭하면 페이지소스보기 메뉴가 있습니다. 또는 이
기능의 단축키인 [Ctr] +0) S 이용할 수도 있습니다(크롬 브라우저 기준).

              스고                 v      =f x
/ 더 “The Office           x \e
Ss      Cc |  1@ book-finterstellar. 6004580003으 html             wo:
~ 레테  —  a
‘The Office              | $1208)                   Alte 2S 화살표
SLE            시 오른쪽 화살표
In my office, th      r
y        ere {    새로고짐(6)                      Ctrl+R
| 다른 이를으로 저장(4)…             Ctrl+s
인쇄(0)                          00
USO.
한국어(으)로 번역)
페이지 소스 보기0/)                    Ctrl+u
BAIN)                      Ctrl+Shitt+!

6장 코딩 기술: 파이썬 기초 93


===== PAGE 94 =====
다음과 같이 HTML 원문이 보입니다.

<html><head><title>The Office</title></head>

<body>

<p class="title”><b>The Office</b></p>

<p class="story">In my office, there are four officers,
<a href="http://example.com/YW" class="member">YW</a>,

<a href="http://example.com/JK” class="member">JK</a>,

<a href="http://example.com/YJ" class="member">YJ</a> and
<a href="http://example.com/KS" class="member">KS</a>

- </p>

<p class="story">...</p>

HIML 코드가 출력이 되긴 하지만 헤더 부분이 B 붙어 나와서 보기 편하지는 않습니다. 이
예제에서는 의도적으로 보기 안 좋게 만들었지만, 실제로 대부분의 웹 페이지들이 깔끔한 모
양으로 보기 좋게 코드가 정리되어 나오지는 않습니다. 뷰티플 수프를 이용해 보기 좋게 만들
어봅시다.

분석을 위해 우선 HTML AA BES 복사해서 110ㄴ00<라는 변수에 저장합니다.

html_doc = """

<htmb<head><title>The Office</title></head>

<body>

<p class="title"><b>The Office</b></p>

<p class="story">In my office, there are four officers,
<a href="http://example.com/YW" class="member">YW</a>,

<a href="http://example.com/JK" class="member">JK</a>,

<a href="http://example.com/YJ" class="member">YJ</a> and
<a href="http://example.com/KS" class="member">KS</a>

- </p>

wo won ou 은 WN

Ke
YP ©

<p class="story">...</p>

»
oN

Out

이제 뷰티플 수프의 함수를 호출해야 하는데 뷰티플 수프 함수는 654라는 라이브러리에 들어

있으므로 654를 먼저 부르고 그 안에 들어 있는 뷰티플 수프(패키지명 863411415040)를 가

94  2부 주식과 지수


===== PAGE 95 =====
져와야 합니다.

1 from bs4 import BeautifulSoup

Out

고 뷰티플 수프 함수를 이용해 html_doc-S 44 (parsing) a4] 500이라는 변수에 저장
합니다. 뷰티플 수프가 파싱을 할 때는 HTML 코드를 분석해서 코드 안에 담겨 있는 태그별로
서브 변수를 만들어 내용을 저장해놓습니다. 따라서 사용자는 소스 내에 있는 태그 단위로 정

1 soup = BeautifulSoup(html_doc, ‘html.parser')
# 뷰티플 수프 항수를 이용해 html_docS 해석해서 soupO| 저장

out
태그가 눈에 잘 HO] = prettify 함수를 이용해 HTML SES 태그 단위별로 줄바꿈을 해
서 보여줍니다.

1 print(soup.prettify())

Out <html>

<head>

<title>
The Office

</title>

</head>

<body>

<p class="title">
<b>
The Office
</b>

</p>

<p class="story">
In my office, there are four officers,
<a class="member" href="http://example.com/YW">
YW
</a>

?

63 코딩 기술: 파이썬 기조 95


===== PAGE 96 =====
<a class="member™  으르 “http: WEA com/JK" >
JK
</a>

<a class="member" href="http://example.com/YJ">
YJ
</a>
and
<a class="member" href="http://example.com/KS">
KS
</a>

</p>
<p class="story”>
</p>

</body>

</htmb>

이제 소스 FES 보고 내가 가져오고 싶은 정보가 어떤 태그에 들어 있는지 찾아봅시다.
태그는 <태그명>처럼 AA 안에 들어가 있습니다. 예를 들어 문서의 ASS
<title>The Office</title> 부분이 문서 제목인데, <『1【16>이라는 태그로 감싸져 있습ㄴ
다. <title HIS 가져와서 내용만 뽑아보겠습니다.

1  soup. title  _ # title Has 통째로 가져옴
Out <title>The CECE Eley

태그 소스까지 필요한 게 아니므로 텍스트만 가져오려면 16×\ WES Sc.

1 soup.title.text # title 태그 내용을 추출
Out ‘The Office’

이제 본문으로 들어가서 팀원들의 o|S (yw, JK, YJ. KS)S 뽑아보겠습니다. 화면과 HTML

AAS BY 팀원들의 이름은 하이퍼링크 처리가 되어 <a> 태그로 둘러쌓여 있다는 특징이 있
습니다. 그래서 우선 <a 태그를 중심으로 공략해보겠습니다.

96 2 주식과 지수


===== PAGE 97 =====
1  ‘soup. a #a 태그를 ENS FHS

Out <a class="member" href=" 1004 //001010: com/Yw" >YW</a>

팀원은 4명인데 첫 번째 팀원만 나왔네요. 4명을 한 번에 불러오려면 find_allL& 써야 합니
다. 100_311('태그' ) 명령은 소스 코드 내에서 해당 태그를 모두 찾아 리스트에 넣어서 돌
려주는 기능을 합니다.

1  soup.find_all(‘a')   # a 태그를 모두 가저음

Qut [<a class="member" href="http://example. com/YW' Syuc/a>,
<a class="member" href="http://example.com/JK">JK</a>,
<a class="member" href="http://example.com/YJ">YJ</a>,
<a Class="mesber of href=" 그 1041 YC Made IAS BS

이제 태그를 제외한 팀원들의 이름만 뽑으려고 합니다. 결과가 리스트 형태이기 때문에 앞에
서 ABBY soup. find_all('a').textBE 값을 찾을 수 없습니다. 실행 결과에서 생략하
는 부분은 로 표시했습니다.

1 soup. find_all(‘a’).text

000
AttributeError                   Traceback (most recent call last)
<ipython-input-12-243f@feb02af> in <module>()

----> 1 soup.find_all(‘a').text

nee

AttributeError: ResultSet ~~

ic 다음 코드처럼 리스트를 다루는 방법을 이용해야 합니다. 세 번째 팀원 이름을 가져오려
리스트명[2]라고 입력해야 합니다. 파이썬은 숫자를 0부터 카운트하기 때문에 세 번째 팀원
이 ie] 저장됩니다. 부록 &.3절을 참고하세요.

1  5040ㆍ 7100. allC a (2) |

Qut <a class="member" href=" Ae (eran. comes 51340

리스트 내의 데이터를 하나하나 읽어서 그 안에서 데이터 WS 찾아오는 방식이지요. 10「를

6장 코딩 기술: 파이썬 기초 97



===== PAGE 98 =====
이용해서 리스트 내용을 하나씩 읽어내면서 앞에서 했던 대로 texts USS 읽어옵니다.

1 member = soup. find_all(‘a')
2 for m in member:
3              print(m. text)

Out YW
JK
YJ

이상의 내용은 깃허브 저장소 06. Beautifulsoup.ipynb 파일에 담겨 있습니다. 이후에도
이 책의 파이썬 실습은 주피터 노트북을 이용하며, 노트북 파일은 모두 깃허브에 들어 있으므
로 파일명을 따로 표시하지 않습니다.

뷰티플 수프 라이브러리에 대한 더 자세한 내용은 공식 웹사이트를 참고하기 바랍니다. 문서
페이지는 https: //www. crummy .com/software/BeautifulSoup/bs4/doc/ 입니다.

사실 이렇게 데이터를 수집하려면 HTML 문법을 어느 정도 알아야 수월합니다. 아래는
HTML 코드의 기본 구조 예시입니다.

<html>
<head>
<titloBA A]S</title>
<scripb 4 페이지를 컨트롤하기 위한 스크립트 프로그램 </50ㅠ10
</head>
<body>
<a href="SA SACS 웹 페이지로 연결할 + 있는 하이퍼링크</2>
<0>문단</6>
<01\>블록</01\>
<6>볼드체</6>
<table> j0|=
<tr HO} B92} 행
<td S: 테이블 데이터가 실제로 기록되는 부분</『0>
</tp
</table>
</body>
</html>

98 2% 주식과 지수



===== PAGE 99 =====
태  a 22                           Chapter 7
Bees    F Ice!

os =

처음에 안내했듯, 이 책에서는 각 BES] 코딩 ASS 한 파일에서 진행합니다. 앞의 코드부터
순차적으로 실행해야 정상적으로 결과가 나오니 꼭 앞에서부터 진행하기 바랍니다. 실습 중
간에 주피터 노트북을 ACH} 다시 진행해야 한다면 우선 상단 메뉴에서 Kernel > Restart &
Run All HES 눌러 전체 셀을 일괄 실행해서 앞부분 SAAS 메모리에 저장한 후 진행하
기 바랍니다.

먼저 이번 BEA] ASS 진행할 노트북 파일을 만듭니다.

7.1 S&P500 vs. KOSPI200 비교
여기에서는 우리나라 대표 포털 사이트인 네이버와 다음에서 과거 주가 데이터를 수집
(scraping) SHA] 그래프를 224451 (plotting) 회귀분석까지 해보겠습니다. 처음에는 구글 파
이낸스에서 데이터를 수집해 AS 썼으나, 2018년부터 구글이 데이터 수집을 위한 시세 데이
터 제공을 막아서 편집 과정에서 국내 사이트로 변경했음을 밝힙니다. 야후 파이낸스도 시세
Sali 제공하는데, 미국이나 유럽 시장 데이터는 잘 정리되어 있지만 한국 시장 데이터는
는 SSE 많고 중간중간 빠진 데이터도 많이 발견되는 등 신뢰도가 낮아 사용하기 곤란합
i 네이버와 다음은 국내 증시 데이터를 빠뜨리지 않고 제공해주긴 하지만, 금융정보 코너
가 깔끔하게 정비되어 있지는 않습니다. 국내 지수, 해외 지수, 개별 SES 각각 다른 WSO
로 제공하기 때문에 데이터를 수집하는 프로그램도 각각 만들어야 하는 단점이 있습니다. 그

7장 금융공학 모델링 99


===== PAGE 100 =====
럼에도 불구하고 금융공학에서는 데이터의 신뢰도가 중요하기 때문에 우리 책에서는 국내 포
털 사이트를 이용하기로 합니다. KOSPI200 지수는 네이버에서, S&P500 지수는 다음에서 수
집하겠습니다.

네이버에서 KOSPI200 지수 수집하기(『11\4Ｌ 페이지 크롤링)
프로그래밍에 들어가기 전에 우리가 데이터를 수집해올 네이버 페이지를 보겠습니다. 크롬 브
라우저를 열어 http: //finance.naver.com/sise/sise_index.nhn?code=KP1200 에 접

속합니다.

KOSP1200 지수 정보가 나옵니다. 화면 중앙에는 KOSPI200 지수 그래프가 나오고 바로 아
래는 최종거래일의 시간별 시세가, 그 아래에 일별 시세가 나옵니다. 우리가 수집할 정보는 빨
간색으로 표시한 '일별시세'입니다(사이트의 레이아웃은 집필 시점과 달라질 수 있습니다).

Bee RUB BNE YEE BS 투자전랙 뉴스  )/7금융 추천중목
TRIM 전지콜시시스템 (RAST 공매도 총합 포털 LRSM OO 동계시뇨 ㆍ [뉴스] '가상회해' 논린 [뉴스] 글로벌 경제 리모트
국내증시        25> Sas) Farsley, FARO                                     외근조의     lv STOCK
ㅣ 주요시짜정보         | 코스피200                                                     EE] 201803. worn    Atal      2,461,000 a
코스피 코스닥 of   noes   ==   =  = ae    =     TS:
ae 포보스          leaw)ua fou] @amzo     314.61 -심희증쪽수          1                              |
es eg        Be               전얼대비      2079 상승종목수      18
ts mm 284         as                    등역률        40.25% 티의즈목수          0 |
pial Load       |    그                 장중최고       3316.92 OTB RE        ”
we vo 99      }     “>                     Bena         34 VME          13
상한가 eI             이                      2740         959 거래랄 8      111255 |
26 aa              hus       fut.      62984       VSL 기래대금   4.972.189 |
7a os au   '         ue  2    14                                         |
OLNEY
와국인때격 et    Ama                                                                  Ste]
브로그륨젝에홍성:        세결시각      Amt       Ayo}      변농래선주)     가례량      NEE
00268                                                       @ 금호티이어    4615 2
<n        meee        ㅇㅇ        as         nos         ses       O NAVER        792,000 2
eee               주자         mse        a uo           °          1          aia       Dolls         650 v
warms             as        a2        a uo          °         1009         41a      © 비이오리더스    2,100 ¢
poe a                                                          6 셀트리온     309.900 ㅜㅠ
ro                mu?        mS        a uD          °         0p         au
on             msaz           a uo               0              [000             000         WY 많이 본 뉘스
ㅣ 두지자보호             ne         542        au          °         1         area
Baek                                                                                            “AL 매수 1A '셀드리운 에
meUNS%                         123 4 5 6 7 8 9 10 디요ㆍ MY»                   ㆍ [추간증시전양]%시 wae
AU DYSS                                                                                                                       ㆍ [추간증시전망] SOR 고스
Ll sen                                                         ㆍ널위기 증시에 "과열 검보 증
ㅣ조건갑석                 oe         세결기         선알리         ows        MAD eh)       AAS 8      , 한국거래소, PAIN Ala

100 2% 주식과 지수


===== PAGE 101 =====
필요한 정보만을 추려내야 AA 분석이 쉬워지기 때문에 일별시세 부분만 추려내봅시다. 일별
시세 테이블 위에 마우스를 가져가 오른클릭을 하면 나오는 프레임 소스 보기 를 클릭합니다.

12 3 4 5 6 7 8 9 10 다음 WY »
일별시세 (                 ~       ns         ae
뒤로(8)                       씨+왼쪽 화살표         1                ,    =
거래량 진주)        거래대금 인.
날짜        앞으로)               시+오름쪽 화살표         =             ot
20180330       새로고침(0)                        Ctrl+R         111256            3472.10
20180329                                                        8366            51797
mam |     다른 이름으로 ABA)...               CtrleS           3.00             5620918
인쇄(6)                           Ctrl+P
20180327       ASO...                                         nD            ATPASES
스- 구드        한국어(으)로 번역()                                  whee             33092
IR                                                       101615            5,380,087
| Holz] 소스 보기00)                  +
|   프레임 소스 보기0/)                       > 맨뒤 나
Saal    프레임 새로고침)
—         | MAKN)                       Ctrl +Shift+t
GAY~      TAT       2717마    rare        Sy . 거래대금(딱인)? 시기총액억)^
삼성전자           2,461,000       a 9000     037%        154.921         30107       319,52

새 창이 열리면서 AA BE} 나옵니다. 이제 뷰티플 수프를 이용해서 AA 코드를 해석하고
분석을 시작해봅시다.
선 데이터를 뽑아낼 데이터가 들어 있는 웹 페이지의 주소를 확보해야 합니다. 웹 페이지의

우선
주소는 소스 보기 주소에서 view-source: 를 제외한 나머지 부분입니다.

[2] view-sourcesfinance.nav. X 0000)

(G} © view-sourceffinance.naver.com/sise/sise_index_day.nhn?code=KP1200|      고 @e:

_>

enx~oeoceun =

<himl lang="ko*>

9| <head>

10| <meta ht tp-equiv="Content-Type” content="text/html: charset=euc-kr “>
1} <(1116>네이버 SS</title>

12| <link rel="stylesheet” type="text/css” href="http://t        ©, com/cs            1   1    4*>
13| <link rel="stylesheet” type="text/css” href="   it    2                    i   1     >

14) <link rel="stylesheet” type="text/css* href="htto://tinance naver_com/css/ layout css?20 18032 1054224 *>

15| <link rel="stylesheet” type="text/css” href="httn://tinance, naver, com/css/main, css?20 18032 1054224">

16| <link rel="stylesheet” type="text/css” href="http://t                          1        >
17| <link rel="stylesheet” type="text/css* href="   :           t             3         1    4">

18| <link rel="stylesheet” type="text/css” href="htto://tinance, naver .000/665/1\01 10.6657020160321054224">
19| </head>
20 | <body>                                                                      ㅠ

7장 금융공학 모델링 101


===== PAGE 102 =====
주소창에 있는 화면 주소에서 view-source: FHS 지운 나머지 부분, 즉 http://
finance.naver.com/sise/sise_index_day.nhn?code=KP1200°] 일별시세 테이블의

103&.입니다. 주소창에 이 URLS 입력하고 [Enter JS 눌러서 화면을 확인합니다.

v     a     oO     x
O) 네이버 금융             x \ Wa
€7G4  fo) finance.naver.com/sise/sise_index_day.nhn?code=KP1200     * GB a
일벌시세
날짜            체결가              전일비               등락율              거래량 천추.            AeCHAR Ash
20500        31461          a07         +027%            111256           4,472,189
2A       3322         a 201        +6R            83,676           5,117,417
Doss       31181         ㅠ 953         “143%            $3,400           5,620,918
25082       31639        a 14        +05           85599          47468
2AM       3149         a 297        +0795            81668           4329.24
20802      31242       ㅠ 1990       237%         101,615         590,087
123 4 567 8 9 10 Ce 맨뒤 나

네이버 화면상에는 '체결가라고 표시되어 있지만, 이 부분이 종가입니다. 우리가 필요한 데이터
는 날짜와 종가이므로 이 돌을 골라내서 뽑아내는 것을 목표로 소스 분석을 시작해보겠습니다.
데이터가 어디까지 들어 있는지 확인하기 위해 화면 하단 페이지 내비게이션의 맨뒤 버튼을
눌러서 마지막 데이터를 확인합니다.

v     =     ㅁ     x
[고 네이버 금융              x
€      ‘G)  QJ finance.naver.com/sise/sise_index_day.nhn?code=KPI200&page=506 | xr Ge
일별시세

닐짜                    제결가                     전일비                      등락률                    거래량 서주;                  거래대금 만
20800       17898       v12       077%         12811         4,590,668
AEHOLO        18030         ㅠ 057         0329           191222          4A
20000         18087          a 265         +LI%           26313           460953
20001       17a        ㅠ 109        0619         20632         5,522,148
NGO OF        17991         a 110        +E          188,541          S360 812
ZOOL         17881          a oR         +0 27%           158041           4,161,549

맨앞 이전 501 502 503 504 505 506

102 2% 주식과 지수



===== PAGE 103 =====
페이지를 이동하니 URL 0396라는 인수가 따라붙은 것이 보입니다. 네이버에서는 0296
인수 뒤에 따라붙은 페이지 HSS 변경하는 방식으로 일별시세 정보가 움직이는 것을 확
인했으니, 이제 일별시세 URLS Te ak an
마10ㅁ?0006=종목코드&0806=페이지번           것을 알았습니다.

네이버에서는 KOSPI200 지수의 종목코드를 (『1Ｌ200이라고 정의하네요. 종목코드를 1106×_
cd 변수에 저장합니다. 페이지 번호는 1부터 시작해봅시다.

ry

index_cd = 'KPI20@'

2 pagen=1

3  naver_index = 'http://finance.naver.com/sise/sise_index_day.nhn?code=' + index_cd +
‘&page=' + str(page_n)

Out

수집할 페이지 주소를 naver_index 변수에 담았습니다. 0『1116.「60465+에 Y= urlopen
SPE 인터넷에서 소스 코드를 FIVE 기능을 합니다. 이제 URLS 알고 있으니 파이썬으
로 해당 URLY 소스 코드를 FOlSH| source 변수에 담아보겠습니다.

from urllib.request import urlopen

N

source = urlopen(naver_index) .read()

Ww

source

Out b' 아이아스 오오오 iene" ko" aS \pcheads Viceeta Sheep: equiv=" Content-Type"  content=" "text/
html; charset=euc-kr">\n<title>\xb3\xd7\xc@ \xcc\xb9\xf6 \xb1\xdd\xc@\xb6</title>\
n<link rel="stylesheet" type="text/css"href="http://finance.naver.com/css/newstock.
€SS?20180321054224">\n<link rel="stylesheet" type="text/css" href="http://finance.naver.
com/css/common.css?20180321054224"> ~~

소스 SES 출력해보니 너무 복잡해서 읽을 수가 없습니다. 뷰터플 수프를 이용해 태그별로
분류하겠습니다.

AW. prettify()E 소스를 태그별로 보기 좋게 정돈하는 기능입니다. BeautifulSoup7}
들어 있는 654 라이브러리를 호출하고, 그다음 뷰티플 +H] 함수를 이용해 504「ㅇ6를 해석합
니다.

7장 asst 모델링 103


===== PAGE 104 =====
1 import 054
2  _ Source = bs4. BeautifulSoup(source, ‘bal")

Out

prettify() 함수를 이용해 보기 좋게 줄력해봅니다.

1 print(source.prettify())

Out <html lang="ko">
<head>
<meta content="text/html; charset=utf-8" http-equiv="Content-Type"/>
<title>
네이버 금융

~

이 많은 소스 코드 중 어디를 HK 우리가 원하는 데이터를 뽑을 수 있을까요? 네이버 화면
으로 다시 돌아가서, 우리가 Hook 할 데이터를 봅니다. 날짜와 지수를 추출해야 합니다. 네
이버는 지수를 '체결가'라는 필드에 Pouezlst, 이 데이터가 해당 날짜의 종가지수입니다. 이
데이터가 정확하게 어느 부분에 있는지 알아보는 방법이 있습니다. 날짜 위에 마우스를 가져
가 오른클릭을 하고 나오는 메뉴 중 검사 를 클릭합니다. 이 책에서는 날짜가 2018.04.03으로
나오지만(이 부분을 집필한 날짜입니다) 실습할 때는 여러분이 실습하는 날짜에 해당하는 데이터
가 화면에 표출되므로 날짜가 다른 것이 당연합니다.

일빌시세
날짜         제걸가          전일비          등락률
pv Tit ee ae ee En)       oA by AL
206002, 뒤로(8)                    시나왼쪽 화살표
mann 앞으로)              Alt+ OBS 화살표
새로고침(6)                        Ctrl+R
2018.03.29
20680325     다른 이름으로 HAYA)...               Ctrl+s
201860327     인쇄(0)                            Ctrl+P
| 전승(0…
한국어(으)로 HAM                            다임
페이지 소스 보기0/)                  Ctri+U
BAN)                       Ctrl+Shift+!

104 2% 주식과 지수



===== PAGE 105 =====
화면 오른쪽

에 소스 코드가 나타나며 마우스가 가리키고

있는 부분에 해당하는 코드가 선택될

것입니다. 다음 그림에서 파란색으로 음영 처리된 부분입니다. 화면이 다음 그림처럼 나오지

2       르 >1으       도     =)             -   :       =
않는다면 화면 사이즈를 키우고 오른쪽 화면에서 붉은색으로 표시된 Elements YS 클릭한
후 스크롤바를 위아래로 움직여보세요.

|:    =    Oo    x
Gyo 금융           x      기
<     (GO) finance.naver.com/sise/sise_index_day.nhn?code=KPI200&page... 고. Be:
0 00   Elements | Console Sources Network »          : xX
일빈시세              기 기뢰 고기    .  그 / 2 23. 56205
ecu         ><h4 class="top_ tlt" style="text-align: left; ">~</h4>         +
아레 체결가        Vctable summary="O 시세표:날짜에 따른 체결가 전일비 등릭률 거래
랑 거래대금 ASS 제공합니다." 66110200108="0" cellspacing="0"
313.38        class="type_1">
2180       31400           <caption> 2! BM Al All</caption>
> <colgroup>.</colgroup>
2018.03.30                31461                        v <tbody>
> <tr>_</tr>
>
2018.03.29              31382                       번 ins ee
2018.03.28     31181                date”™)2018.04.03</td
i                            <td class="number_1">313.38</td>
cag       see             > <td class="rate_down” style="padding-right:35px;">~</td>
> <td class="number_1">_.</td>
1 2           <td class="number_1" style="padding-right:4@px;">132,269 |
html  “body  “div.box _type_m  table.type_1 tbody tr | tdidate |            |
Styles Event Listeners DOM Breakpoints Properties Accessibility
Filter          shov .cls ry ~                 =
element.style {                  별
}
table newstock.css?20_.0321054224:496
-type_1 td.date {
padding-right: 8px;
color: HJ#999;
font:> 100× tahoma;
text-align: center;
}
table newstock.css?20..0321054224:489
a                -type_1 td {                        f
4    |          »   height: 22px;              ~ | Filter         O Showall ~

필요한 데이터 중 날짜는 <0 class="date">2018.04.03</td>ol] 들어 있습니다. 같은 방
법으로 4월 3일 종가인 313.38 위에서 오른클릭을 하면 <td class="number_1">313.38</
td>ol] 종가가 들어 있는 것을 확인할 수 있습니다.

7장 금융공학 모델링 105


===== PAGE 106 =====
O) 네이버 금융            ×
<  c  (0) finance. naver.com/sise/sise_ index _day.nhn?code=  =KPI200&page...  *¥i Be:
R  G] Elements Console Sources   Neork   »            : x
일별시세                      ~ 62 CIESS$ OCOxZ_t ype 7     -                                   고

> <h4 class="top tlt" style="text-align:left;">..</h4>

Bs mmoee 363-22 |     Yctable sumary="Q! 시세표:날짜에 따른 체결가 전일비 등락률 거래
량 거래대금 정보를 제공합니다." cellpadding="0" cellspacing="0
Dis   만.      class="type_1”>

<caption> @ BAIAll</caption>

2018.0402       314.00
> <colgroup>.</colgroup>
21830       31461           Vv <tbody>
> <tr>_</tr>
> <tr> </tr>
20160129       31382            ¥ctr>
2180828       31181                <td class="date">2018.04.03</td>
td      number _1°5313.38/td
a         as             > <td class="rate_down" style="padding-right: 35px; ">..</td>
> <td class="number_1">~</td>
1 2            <td class="number_1” style="padding-right:4@px;">132, 269

ㅜㅠ
ee ES         —      =       ——
html body div.box_type_m table.type_1 tbody tr  | td.number_1 [ji

“Styles | Event Listeners DOM Breakpoints Properties Accessibility

Filter         thov .cls Sry,
element.style {                  i
}

table newstock.css?20..0321054224:494

-type_1 td.number_1 {
padding-right: 25px;
color: M#666;
font:> lipx tahoma;
text-align: right;

table newstock.css?20..0321654224 : 489
-type_1 td {
a          »   height: 22px;              ~ | Filter         GO Showall ㅜ

우리가 필요한 데이터는 모두 <td> 태그에 들어 있는 것을 그 뷰티플 수프를 이용ㅎ
서 <td> 태그를 찾아 안에 들어 있는 데이터를 뽑아내는 것
적으로 <td> 태그 분석을 시작하기 전에 우선 <td> 태그가

“a

1 td = source.find_all(‘td')
2  len(td)_   # 00의 개수 확인

Out 54

<td> 태그를 모두 골라서 tae 변수에 저장했습니다. 앞서 find_all 함수는 찾아낸 데이
터를 리스트 형태로 저장한다고 소개했습니다. td 리스트의 데이터 개수를 확인하는 명령어

106 2% 주식과 지수


===== PAGE 107 =====
인 Len 2 데이터 개수를 확인하니 54개가 나왔습니다. 화면에 있는 <td> 태그의 개수가 54

개라는 뜻입니다. 일일이 눈으로 확인하기에는 데이터가 너무 많죠.

데이터를 대량으로 제공하는 사이트에서 원하는 데이터의 위치를 찾아낼 때는 XPath 주소를
이용하면 편리합니다. xPath(XML Path 12084286ㅇ)란 웹사이트 또는 XML 문서에 있는 Zt

ZAAZ
주소를

항목의                                    조합한 경로 형태로 표현하는 언어입니다.
크롬 브라우저에서 데이터의 XPathS 확인하는 방법입니다.

우측에서 음영으로 선택된 부분에 마우스를 갖다 댄 후

문서에 포함된 태그를

0) 스크린 우

 오른클릭을 하면 나오는 메뉴 S (Copy 를

@ Copy XPath 를 클릭합니다.

선택 후

PN | 네이버 금융           x A
은     (02  fo} finance. naver.com/sise/sise_ index day. nhn?code= KPI200&page..  _  Ge:
te  0]    Elements Console   Sources   Network   »            이 bx
일별시세                  -    이기지고기 CEESS VON ypeu 0                     ——
><h4 class="top tlt" style="text-align:left;” 0020          =
 Se 체결가        Vctable sumary="Qe! 시세표:날짜에 따른 체결가 전일비 등락률 거래
2 거래대금 정보를 제공힙니다." cellpadding="0" cellspacing="0"
313.38          class="type_1">
노아        31400             <caption> @  AlAil</caption>
> <colgroup>..</colgroup>
2018.03.30               31461                       V <tbody>
> <tro_</tr>
a                          > <tro</tr>
2018.03.29        313.82             wate
2018.03.28        31181
<td clas           .
Add attribute
20900       goss              <td clas                      g-right :35px;">~</td>
><td clas      Edit attribute
1 2              하는거     Edit as HTML         -right:4@px;">132,269 |
html body  div.box_                          td.date
4            먹        Delete element             | tddate |
Styles Event Listeners |                  a
'                  Copy                   »          Cut element
Filter
Copy element
element.style {      |      Hide element                 PY
}                           |                                           Paste element
|       Force state           >
table newstock.css?2
-type_l td.date { |    Break on        » |    Copy outerHTML
padding-right: 802                 ㅣ
Copy selector
color: H#999;       Expand recursively
font: > 10px tahome                          Copy XPath
text-align:  center    Collapse children
|
5        ‘
Rabie                >4        croll into view
stype_1 td {       |     Focus                        Zz
1 6            »   height: 22px;                때             ©) Showall ㅜ

73 금융공학 모델링 107


===== PAGE 108 =====
복사한 XPathS 확인해봅시다. 노트북 화면으로 돌아가서  +(VJS 누르면 복사해둔
XPath 주소가 나타납니다.

/html/body/div/table[1]/tbody/tr[3]/td[1]

앞에서부터 슬래시 단위로 huml—body—div—table (A 번째)-ㅠ(세 HA) td (4d 번째)를 차
례로 찾아가라는 뜻입니다. %ㅁ0201상의 1600\는 실제 코드상에 있는 것이 아니라 여기에서
부터 테이블의 내용이 시작된다고 표시해주는 것이므로 0800\를 제외한 나머지를 찾으며 따
라가보면 원하는 데이터에 도달하게 됩니다. 찾아가는 방법은 찾는 값이 하나일 경우에는
1100(태그명), 여러 개일 경우에는 7100_811(태그명 )[순서]를 이용합니다. 주의할 BS
XPath} 파이썬이 숫자 세는 방식이 달라 BzrSa 수 있다는 것입니다. %8301는 숫자를 1부
터 세지만 파이썬은 숫자를 0부터 세기 때문에 XPath 수에서 -1을 해줘야 합니다. 위 XPath
를 파이썬 코드로 표현해보겠습니다.

1 # /html/body/div/table[1]/tbody/tr[3]/td[1]
2 source.find_all('table')(@]. find os tr’ 12). find_all('‘td')[@]

Out <td class="date">2018.04.03</td>

<td class="date">A|4H class 이름을

a 이름을 붙인 td 태그는 아래와 같이
이름을 지정해서 Bord 수도 있는데, 이렇게 할 경           앞에 붙는 태그를 생략할 수 있어서
유용합니다.

1 d = source.find_all(‘td', 61355 ='date')[@].text
2900

Out '2018.04.03'

원하는 데이터를 찾기는 했는데, 네이버가 지정해놓은 날짜 형식은 파이썬의 날짜 형식과 다
릅니다. 파이썬이 날짜로 인식할 수 있도록 형식을 바꿔줍니다. 점(. )으로 구분된 년, 월, 일
을 분리하고, 이를 436Ｌ1006 라이브러리를 이용해 date 형식으로 바꿔줍니다.

datetime 라이브러리를 이용하기 위해 먼저 43161106 라이브러리를 [라는 이름으로 호출

408 2% 주식과 지수



===== PAGE 109 =====
합니다.

1 import datetime as at

Out

이제 BAS. split (FEAL) 함수를 이용해 구분자를 기준으로 BASS 년, 월, 일로 분해
합니다. 분해한 문자열은 0『.0216(년, 월, 일) BPS 이용해 날짜 형식으로 바꿔서 this_
date 함수에 저장합니다.

yyyy = 106(0.50111('.')[0])

mm = int(d.split('.')[1])

dd = int(d.split('.')[2])
this_date= dt.date(yyyy, mm, dd)
this_date

Out datetime. s-date(2018,  4,  가

Oo 은 WN

날짜 형식으로 Ube this_date 값을 확인할 수 있습니다.

읽어온 날짜 정보를 036 형식으로 바꿀 일이 계속 생기므로 이 WSS 함수로 정의해줍니다.
eee date_format )으로 하겠습니다.

1 def date_format(d):

2      d = str(d).replace('-', '.')
3       yyyy = int(d.split('.')[@])
4      mm = int(d.split('.')[1])

5      dd = int(d.split('.')[2])
6

7

8

this_date= dt.date(yyyy, mm, dd)

return this_date

Out

2행에 보면 0 = 늘보 45009  = uf 추가되어 있는데, 이는 날짜 구분자가 .가
아닌 -로 되어 있을 경우 . 로 변환해주는               . 문자열.「601866('ㅅ', '8' ) 함수

7장 금융공학 모델링 109


===== PAGE 110 =====
는 문자열 ‘A'S B'S 바꿔주는 기능을 하지요. 이렇게 하면 3~5행에서 수행하는 .를 기준으
로 년, 월, 일 데이터를 를 분리하는 기능을 공유할 수 있게 됩니다. 7행에서는 0.0816 가

일) 함수를 이용해 date 형식의 BAS 저장하고 8행에서는 저장한 날짜를 함수 수행의 Ast
값으로 돌려줍니다.

이번에는 지수를 가져올 차례입니다. 해당 일자의 종가지수를 가져와야 하지요. 앞에서 했
던 것과 같은 방법으로 종가를 가리키는 XPathS 구해보면 /html/body/div/table[1]/
16000/ㅠ[3]/10[2]입니다. 종가를 가져올 때는 받아온 데이터를 숫자로 인식하도록 처리하
기 위해 숫자에서 천의 자리를 표시하는 쉼표(, )를 제거하는 작업이 필요합니다. 쉼표 제거에
도 4A) replace() 함수를 이용합니다.

1 this_close = source. find_all('tr')[2].find_all(‘td')[1].text
2 this_close = this_close.replace(’,', '') # 쉼표(,) 제거

3 this_close = float(this_close)
4

this_close

<td class="number_1">313.38</td> 역시 간단하게 다음 코드처럼 나타낼 수 있습니다.

1 p = source.find_all(‘td', class_='number_1')[@].text

간단한 코드를 이용하여 페이지에 있는 모든 날짜와 가격을 불러오겠습니다.

1 dates = source.find_all(‘td', class_='date’)
2 prices = source.find_all(‘td', class_='number_1')

Out

데이터 개수를 확인해봅니다. 우선 날짜 개수입니다.

110 2부 주식과 지수



===== PAGE 111 =====
1 len(dates)

Out 6

지수의 개수도 6개일까요?

1 len(prices)

Out 24

24개로 왜 더 많을까요? 크롬 브라우저로 돌아가 소스 코드를 살펴보면 답을 알 수 있습니다.

CR 은] | 태여바제 Console Sources Network»      i x
일별시새                                                                   f      V<tGody>                                   -
| 7200 1721
wat          새결가           전일비           ae          eae          거애대글                reid
votre
20300        31336        yon        2%          122          SADR               <td Class="date™>2018.04,03«/td>
ze        400        v 061        AIM           ae          429087               <td class="number_1">313,38</td>
matd    ="rate_doun™    …     태지 35px; ">=
am        31463        207        025          noses          4a25 64    ㅣ          Fp rome  rate_     style«" padding-right. 35px
|            td class="number_1” 시
3BR        a 201        ~           BOs          12417 peep errs style-"padding-right:40p«;">
suet        vas        19355          aD          S093    |           <td class="number_1” style="padding-right:3ep«; ">
206여가       33671       als       ae         an        OK   |         $,453,352</te>

</tr>
재기
Pctroic/te>

123 45 67 6 9 10 다음 SH»

소스 FES BH <td class="number_1"> 코드가 47] 보이는 것을 확인할 수 있습니다. 마
우스로 각 태그들을 가리켜보면 '체결가', '등락률', '거래량', Adda 칼럼이 모두 같은 태그
를 사용하고 있네요. 우리는 이 4개의 값 중 첫 번째 값만 필요하므로 0, 4, 8, … 등 4의 배수
로 나타나는 값들만 추출하기로 합니다.

이제 테이블의 날짜를 한 줄씩 순환하며 날짜와 종가지수를 주출해봅시다

1      for n in range(len(dates)):  # dates 개수만큼 반복

2          this_date = dates[n].text # 번째 dates Zt 추출

3         this_date = date_format(this_date) # 날짜 형식으로 변환
4

5          this_close = prices[n*4].text

6         #0, 4, 8 ... & 4의 배수에 해당하는 종가지수 추출

7         this_close = this_close.replace(',', '') # 쉼표(,) 제거
8         this_close = float(this_close) # 숫자 형식으로 변환

9         this_close

7장 금융공학 모델링 111


===== PAGE 112 =====
10
11       print (this. date, this 5 1056) ^   # # 걸갓값 출력

Out    2018-04-03 313.38
2018-04-82 314.0
2018-03-30 314.61
2018-03-29 313.82
2018-83-28 311.81
2018-03-27 316.34

현재 페이지에서 날짜와 종가지수 SSS 완료했습니다. 이제 다음 페이지, 그 다음 페이지에
서 반복해서 추출할 차례입니다. 페이지를 하나씩 넘겨가며 추출을 하다가 마지막 페이지에
도달하면 더 이상 다음 페이지로 넘어가지 못하도록 해야겠죠? 이를 위해 마지막 페이지가 어
디인지 알아보겠습니다. 화면 아래쪽 페이지 내비게이션 부분을 주목해봅시다. 페이지 번호
맨 오른쪽에 맨뒤 라는 버튼이 보이지요? 이 버튼에서 정보를 추출하겠습니다. 맨뒤 버튼 위

에서 오른클릭을 하면 나타나는 메뉴에서 검사 버튼을 눌러 [피2이이 있는 곳의 HES 살펴봅
니다.

[융 GJ Elements Console Sources »        : ^
3                                        > <td>_</td>                           ~
전일비       등릭들       거래량치주:            hp hang
>» <tdo_</td>
J                          » <td>_</td>
4       “LSP
7          tae)         13000             > <td>_</td>
ㅠ on        02%           125,560               > <td class="pgR"></td>
wv 061        019           81690              Y<td class="pgRR">
> 3 href©"/sise/sise index day:nhn?
code=KPI200&8page=506 >_< /a
a 07        B%            110524                  </td>
</tr>
aren                         ,                </tbody>                                    「
ㅠ 43        “LAP                          </table>
<!--- 페이지 네비게이션 B--->
</div>
5 6 7 8 9 10 다음: MWR | < //임빙시시 -->                          >

마지막 페이지 주소를 가리키는 하이퍼링크 <3> HIE <td class="pgRR"> 태그입니다. 그
러면 다음과 같이 하이퍼링크 주소를 HOLS 수 있겠네요.

1 paging = source.find(‘td', class_='pgRR').find(‘a')['href']
2 paging

Out ‘/sise/sise_index_day.nhn?code=KP12@0&page=506 '

412 2% 주식과 지수



===== PAGE 113 =====
oP 하이퍼링크 주소에서 페이지 번호인 506만 추출하기 위해 aS 기준으로 문자열을 잘
라내 뒷부분만 가져옵니다. 페이지 번호는 실행 시점에 따라 달라집니다. 시간이 흘러갈수록 데
이터가 많아져서 페이지가 늘어나기 때문이지요. 숫자가 5060] 아니라고 난처해하지 마세요.

1 paging = paging.split('&')(1]
2 paging

Out ‘page=506'

많이 줄어들었죠? 이제 =을 기준으로 한 번 더 잘라내면 페이지 번호만 남겠네요.

1 paging = paging.split('=")[1]
2 paging

Out ‘506’

이제 뽑아온 페이지 번호를 숫자 형식으로 바꿔주면 끝입니다. 지금까지 내용을 종합해 마지
막 페이지 번호를 뽑는 과정을 정리해봅니다.

last_page = 504「66.1100('10', class_='pgRR').find('a')[‘href‘]
last_page = last_page.split(‘&')[1]

last_page = last_page.split(‘=")(1]

Pm WN BR

last_page = int(last_page)

Out

기

[

i

데이터 추출 기능을 함수로
앞서 함수를 소개할 때 같은 기능을 반복적으로 수행해야 할 경우 유용하다고 했습니다. 현
재 페이지에서 데이터를 추출하는 작업을 페이지마다 반복해야 하기 때문에 함수로 만들
어서 활용해봅시다. 지금까지 공부한 내용을 참고해서 함수를 만들겠습니다. 함수 이름은

historical_index_naver ()2}31 하겠습니다.

7장 금융공학 모델링 113


===== PAGE 114 =====
1 def historical_index_naver(index_cd, page_n=1, last_page=@):
3     naver_index = ‘http://finance.naver.com/sise/sise_index_day.nhn?code=' + index_cd +
“&page=" + str(page_n)
4
5     source = urlopen(naver_index).read() # 지정한 페이지에서 코드 읽기
6     source = bs4.BeautifulSoup(source, ‘Lonl') # 뷰티플 수프로 태그별로 코드 분류
7
8     dates = source.find_all(‘td', 01355_='0216') # <td 01355="021[6">태그에서 날짜 수집
9     prices = source.find_all('td', class ="number_1') # <td class="number_1">EHO//A{ 지
수 수집
10
11     for n in range(len(dates)):
12
B            if dates[n].text.split('.')[@].isdigit():
14
15             # 날짜 처리
16             this_date = dates[n].text
17             this_date= date_format(this_date)
18
19             # 종가 처리
20            this_close = prices[n*4].text # prices 중 종가지수인 0, 4, 8... HRY 데이터 추
줄
21            this_close = this_close.replace(',', '')
22             this_close = float(this_close)
23
24           # 딕셔너리에 저장
25           historical_prices[this_date] = this_close
26
27      # 페이지 내비게이션
28      if last_page = 0:
29         last_page = source.find('td', class_='pgRR').find(‘a')[‘href']
30         # 마지막 페이지 주소 RB
31         last_page = last_page.split('&')[1] # & 5/2] page=506 부분 추출
32         last_page = last_page.split('=")[1] # '=' 뒤의 페이지 번호만 &
33         last_page = int(last_page) # 숫자형 변수로 변환
34

35      # 다음 페이지 SB

114 2부 주식과 지수



===== PAGE 115 =====
36     if page_n < last_page:

37         page_n = page_n+1

38       historical_index_naver(index_cd, start_date, end_date, page_n, last_page)
39

40      return historical_prices
Out

앞부분은 다 익숙한데 36~38행은 좀 LIL? 36행에서 현재 페이지 번호가 마지막 페이지
번호보다 작으면, 37행에서 페이지 번호를 하나 올려준 뒤 38행에서 동일한 함수를 새로운 페
이지 번호를 이용해 다시 호출합니다. 재귀함수라고 하는데, 지금처럼 함수 내에서 자기 자신
을 다시 호출하는 경우를 말합니다.

[Shift ]+[Enter |S 누르면 함수가 생성됩니다. 11510「1031ㄴ1006×_ㅁ02\6「(지수코드라고
함수를 실행하면 네이버가 보관하고 있는 해당 지수의 일별시세 AAS 추출해오는 함수가 완
성됐습니다. 네이버는 KOSP1200 지수를 2006년 1월부터 제공하므로 위 함수를 실행하면 그
때부터 오늘 날짜까지의 일별지수를 수집할 수 있습니다.

그런데 살짝 아쉬운 점이 있습니다. 2006년부터의 데이터가 필요한 것이 아니라 2018년 데
이터만 필요하다면 모든 데이터를 추출하는 것은 시간 낭비지요. 네, 그래서 날짜를 지정해서
추출하는 함수를 만들고 싶습니다. 어떻게 하면 될까요? 함수에서 시작 날짜와 마지막 날짜를
입력시켜 데이터 Ses 제어해보겠습니다.

1 def historical_index_naver(index_cd, start_date='', end_date='', page_n=1, last_page=@):

함수 선언부에서 start_date2} end_dateS 입력하도록 추가해줍니다. 사용자가 데이터를
빼놓아도 에러가 발생하지 않도록 초깃값을 지정해줍니다. 여기에서는 데이터 처리가 편하도
록 공백(' ' )으로 지정했습니다.

if start_date: # start_date7} 있으면

start_date = date_format(start_date) # date ZIHOS 변환
else: # 없으면

start_date = dt.date.today() # 오늘 날짜를 지정

if end_date:

nN DO WU 6 W

73 금융공학 모델링 115


===== PAGE 116 =====
8          600 036 = date_format(end_date)
else:

10                 end_date = dt.date.today()

start_dateS 받아오지 못하면 SAS 할당해주기 때문에 3행 1+문에서 값이 있는지 검사
하고, UchA start_dateS date MMOS 변환하고, 없다면 오늘 날짜를 지정합니다. 600_
date 역시 마찬가지로 처리해줍니다. 이제 start_date2} end_date 사이에서만 데이터를 저
장하도록 처리합니다. 뒤에서 전체 코드를 살펴볼 텐데 먼저 알아둘 일부 코드만 살펴보겠습
니다.

29           if this_date <= end_date and this_date >= start_date:
30             # 5[2/【 03[6와 600 0316 사이에서 데이터 저장

31                 # 증가 처리

39           elif this_date < start_date:

40           # start_date 이전이면 항수 종료

41                             return historical_prices

29행에서 this_date7} 600_032+6보다 o]Alo|D start_date'c} 이후에서만 아래 나오는
데이터 처리 HES 실행하도록 조건을 줍니다. 39행에서는 this_date7} 513「『_0216보다
전이면 함수 실행 자체를 SHOES returnS 실행합니다. 이렇게 start_dateol] 도달하자
마자 함수 실행을 종료해버리면 추가적인 데이터 탐색을 하지 않고 효율적으로 데이터를 수집
할 수 있습니다.

이제 날짜 탐색 기능을 추가한 전체 함수를 보겠습니다.

def historical_index_naver(index_cd, start_date="', end_date='', page_n=1, last_page=@):

if start_date: # start_date7} 있으면

start_date = date_format(start_date) # date ZO 변환
else: # 없으면

start_date = dt.date.today() # 오늘 날짜를 지정
if end_date:

end_date = date_format(end_date)

on DO WU FF WY RP

116 25 주식과 지수


===== PAGE 117 =====
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
32

33
34
35
36
37
38
39
40
41
42
43

else:
end_date = dt.date.today()

naver_index = ‘http://finance.naver.com/sise/sise_index_day.nhn?code=' + index_cd +
‘&page=' + str(page_n)

source = urlopen(naver_index).read() # 지정한 페이지에서 코드 읽기

source = bs4.BeautifulSoup(source, ‘lxml') # 뷰티플 수프로 때그별로 코드 분류

dates = source.find_all('td', class_='date') # <td class="date">EHTO/A] 날짜 수집

prices = source.find_all(‘'td', class_='number_1') # <td class="number_1">EHOj/AJ 지

수 수집

for n in range(len(dates)):
if dates[n].text.split('.')[@].isdigit():
# 날짜 처리
this_date = dates[n].text
this_date= date_format(this_date)
if this_date <= end_date and this_date >= start_date:
# start_date2} end_date 사이에서 데이터 저장
# 종가 처리

this_close = prices[n*4].text # prices 중 종가지수인 0, 4, 8... HA 데이

this_close = this_close.replace(',', '')

this_close = float(this_close)

# 딕셔너리에 저장
historical_prices[this_date] = this_close

elif this_date < start_date:
# start_date 이전이면 함수 Se

return historical_prices

# 페이지 내비게이션

7장 금융공학 모델링 117


===== PAGE 118 =====
44      if last_page = 0:

45         last_page = source.find(‘td', class_='pgRR').find('a')['href']
46        # 마지막페이지 FA 추줄
47         last_page = last_page.split(’&')[1] # & 뒤의 page=506 부분 추출
48        last_page = last_page.split(‘=")[1] # '=' 뒤의 페이지 번호만 추출
49         last_page = int(last_page) # 숫자형 변수로 변환
50

51      # 다음 페이지 호출
52     if page_n < last_page:
53         page_n = page _n+1
54       historical_index_naver(index_cd, start_date, end_date, page_n, last_page)
55

56      return historical_prices
Out

4S 만들기만 하고 아직 호출하지 않았기 때문에 ARLES 없습니다. 이제 함수가 잘 작동
하는지 함수를 호출해서 확인해보겠습니다.

1 index_cd = 'KPI2@0'

2 historical_prices = dict()

3  historical_index_naver(index_cd, '2018-4-1', '2018-4-4')
4  emustordcalepcices

Out  idatetine! date(2018,  4,  2):  314.0,
datetime.date(2018, 4, 3): 313.38,
datetime.date(2018, 4, 4): 308. sa

지정한 날짜인 201814 4월 1일부터 4월 4일 사이의 KOSPI200 일자별지수 데이터가 잘 추출
되었습니다. 2018년 4월 1일은 일요일이므로 데이터가 없는 것은 정상입니다.

네이버에서 해외 지수 수집하기(0504 파일 크롤링)

2018년 10월부터 다음([>8410)이 금융정보 크롤링을 막아놓았습니다. 이 책 1쇄에서는 다양
한 기법을 익힐 수 있도록 네이버와 다음 크롤링을 모두 제공했는데, 아쉽지만 다음은 그만두
고 네이버에 집중해야겠습니다. 대신, 앞서 공부했던 HTML 페이지 크롤링이 아닌 JSON 파
일 크롤링 방식을 공부해보겠습니다.

118 2% 주식과 지수



===== PAGE 119 =====
우선 네이버에서 해외 지수를 제공하는 사이트를 찾습니다. 금융 섹션 중 *해외증시' 메뉴에 들
어가면 여러 나라의 지수가 나와 있고 그중 하나를 선택하면 다음 그림과 같이 선택한 지수의
그래프와 일자별 시세가 나옵니다.

머 sar 500 네이버 ag  x +                     siege Aoi tas

< > & hittps//finance.naver.com/world/sise nhn?symbol=SPI@SPXx

*
그유                                a
NAVER 금융                         '                                                           ><}

B88 j%RUBA «6B AIR 6S OM UA  )/7곰옹＊추선중목

(BUS) 전자금시시스텔 ＊ ㆍ[한국거레스] SAS 중한 포털 -(MSSU) 100대 틀제지료 ㆍ[뉴스) 글로벌 검제 리포트 + (SU) Ags 저숙하도록 siege

S&P 500 5869 o@   2039.01.14 16:48 현지시간 기준 ㅣ 10M 지연

2 582 61                UY 2,596.26        DV? 2,589.32          52% 42 2,940 91           =
;
전일대비 V13.65 (-0.53%)         시가 2.500 31         지가 2.570.41            52주의지 2.346.58          그 i
ayn Di 14 | 3년 SY | 10년:     봉사 일정 | 주몽 | 일정:
자개       aeuy
te ected)                                                                                       pact          거래소          90039 & Poor's Corp
Indes
기준통화                   usp
겨래시간                23.30-05 00
(eau) 서머타일 22 30~05 00
inoue
5
DA 24458 (12/78)            Lan
pee
011.                                                                                      !
16715 16010  1626  woe  11700  Wi6 1/23  ww 1207  1274  Waar 12909 | 에/어  own         POUL A
일일 시시
일자          an         전일대외           시가            교가           지가           wase       max SHOCK
2019.01.14       2,582.61           + 12.65          2,580.31          2,589.32          2,570.41           ae      Hee Be
2010.01.11       2,596.26           v0.38          2,588.11          2,596.27          2,577.40          찬국전역      34,800      2100 =
2019.01.10       2,596.64           A118          2,573.51           2,597.82          2,562.02           weed     rete CEN.        3

이번에도 주식 시세 수집 때와 같이 프레임 BAS 시도하기 위해 날짜 위에 마우스를 옮기고
오른클릭 후 나오는 팝업 메뉴에서 검사 를 선택합니다.

일별 시녀
ww          a          uc           치가            고가            지가
carat         rere         2580.91         2,599.32         2,570.41                                                 -
-   |  BAO              <버%       en      ~                        리스트" collpadding~ ne: 난어
2019.91                                   1         x            S77.                                             r
GooaleW At 201901.14 WAS)                                                                      sean! Re
POON eysaey                         제    6872.51           2,597.82           2,562.02                     > «colgroups.«/colgrovp?
내   베  ㅣ                                                          c                                          ‘© thead i /thead>
19.0
=                        a                   2,595.92           2568.09                     + <tbody>                       é
‘         100                                                                                   <i> DOE HARE MA >
2019.01 08       초고          aii             u         259.0         2547.6                    Veter Class-"polmt_on ~>
2019.01.07        2.0             ww.            2S35.61             2,566.16            2524.56           =               00000                :
7019.01.04      2531.4         26405         24740         2,538.07         2443         pas vey Seen Se Ee     bts        abe    =~
ter Event Lnteners DOM Brestgents Properties Accessibilty
201907.07       2789           6204          2,491.92           2490.14           240.96          음음      ne
titer            tnee 30 +, 으
7019.01.02      2510.03         ans        2.476%        2,519.49        2467.47        oT
2018 1271        2.06.85           2111           2,498.94           2,909.24           2,462.82           ,

저어 finance. cosl2e!
ws2.th_status2_t2 tbody td toed (

background position:® -ige -29pa;
)

12345 67 8 9 0 GB

73 금융공학 모델링 119


===== PAGE 120 =====
코드 분석을 위해 검사 화면을 띄워두고 화면 하단의 페이지 번호를 눌러봅시다. 그런데 주소
창에 보이는 08에 아무런 변화가 없습니다. 다른 페이지로 넘어가도 URLS] 그대로 유지되
다니, 어떻게 된 일일까요? 네, 해외 지수 페이지는 주식 페이지와 다른 방식으로 데이터를 전
달하고 있습니다. 주식 페이지에서는 과거 시세를 보여줄 때 각각 새로운 웹 페이지에서 데이
터를 제공해줬는데, 해외 지수 페이지는 동일한 웹 페이지를 유지한 상태에서 데이터만 새로
불러와 표시해주고 있습니다. 웹사이트 운영자 입장에서는 페이지 전체를 다시 만들 필요가
없이 데이터만 바꿔주면 되니 효율적으로 서버 자원을 활용하는 방법입니다. 하지만 우리 크
롤러는 새로운 방법을 배워야 하는 상황이 되었네요.

웹사이트 전체 들은 유지하면서 안 보이는 구석에서 데이터를 불러오고 일부 데이터를 바뀌
주는 기법을 구사할 때 프로그래머는 자바스크립트라는 언어를 이용합니다. 웹 페이지가 자
바스크립트를 이용해 서버에 데이터를 요청하면, 서버는 150이라는 파일 형태에 데이터를
금아 웹 페이지에 전송하고, 자바스크립트가 받아온 JSON 데이터를 해석해 웹 페이지에 뿌르
주는 방식이죠. 우리는 이 JSON 데이터를 찾아 크롤링을 해보겠습니다. JSON 데이터가 어떤
형태로 오는지 찾기 위해 다음 그림과 같이 오른쪽 검사 화면에서 86800 메뉴로 들어가봄
니다.

더 sar xo dom ee      x +                                                                   re?
© > C  & hips finance naver com/eorld/sse nin yymbol “SPLQSPA                                      xy 2 :
aya                                * TG) Bements Conmcle Sources Network Performance | 가   :
wi      2      rua       Ft)       고자     OO VO Wee BN 22 00000501500 | 0 Presevetog 10 Dos
2019.04     2.582 61        rue        2,580.31        2,589.32      {ee te ata ums
(08 5 055 tg Meda Foot Doc WS Mantest Other
2596.26       v0.38      2,568.11       2,596.27    |      ed      are      ae      mt      roars
Lt       ate      257351       24782
Aw       e20%      2500.0      2562
25441       aman      2B       257TIR
2580               aun               2535.61               2.46.16
2534       터떼      2.       2,598.07
247.89          vena          2491.92          2470.14                              Sat ey ee
2,510.03                 230              2926.96               2519.09                             Perform a request of hit Ctrl + R to record the reload
28S             anu            24984            2509.4

이 상태에서 일별 시세 화면에서 다른 페이지 HES 누르면 다음 그림과 같이 오른쪽 화
면에 wor L\dDayListJson.nhn?symbol=SPlI@SPX&fdtc=0&page=6 식으로 클릭할 때
마다 줄이 하나씩 늘어나는 것을 볼 수 있습니다. 그렇습니다. 페이지 번호를 클릭하면
\01「1003Ｌㄴ1512500.0ㅁ10이라는 파일이 실행되면서 JSON 데이터가 호출된다는 뜻입니다.

120 2% 주식과 지수


===== PAGE 121 =====
€ >
월껄 시녀
외지
2018.10
2016.10 20
2018 10 26
2038.10.25
2018.10.24
20161023
2018.10.22
2018.10.19
2018.10.18

2018.10.17

CI sar sco: 네이버 38

x +

C a https//inance.naver.com/world/ise nhin symbol» SPI@SPX

출가
2,682.63
2,641.25
2,658.69
2,705.57
2,656.10
2,740.04
2,755.88
2,767.78
2,768.78

2,007.21

wus
ate
vine
488
aoa
"Hs
ㅋ…15 19
ㅋ11.90

vio
04)

vor

$72) 314151617 8is

Lo 아사자 INS

시가
2,640.68
2,682.65
2,667.86
2.67458
2,737.87
2,721.03
2,773.94
2773.6
2,202.00

2,811.67

2.972.238
2,722.70
2,742.59
2,753.59
2,778.4
2,797.77
2,806.04

281634

10 UG.

… 대 6] Gements

|

= .ㅁ0

x* ㅁ= @:
00900. Sources [Network] Pevtormance | 가 후

‥ㆍ680 BY QQ View 애즈 12 Group by tame 14 Preserve tog ㅣ.) Omable
fitter          (2 Hide data URts
엽서 15 css img Mess Fort Doc WS Mantest Other
200     aX oe     oC 에     00 ws     이
Sta. Type inmatcr 520 Time 배에에        ㆍ
200 xh indo 73 341 제
200 패소 jpndami 73. 이   ㅣ
200 wy = indo 78 100-            1
200 sw tem 77. 53             ㅣ
200 or mim 79. 22.

JSON 데이터를 호출하는 전체 URLS 복사하려면 클릭할 때마다 생겨나는 줄 위에서 오른클
릭을 해서 나타나는 팝업 메뉴에서 Copy > Copy link address 를 클릭합니다.

{lJ sap 500 네이 38        x +                                                                                         -    ㅁ    x
<           Cc      & https //finance. naver.com/world/sise nha ?symbo! = SPIQSPX                                                                                                   w      Ss      e
erat 시세                                                                                                              * [| 6] Bemerts Console Sources     _Networt Performance»         a
자          Br          선일대리           시가            교가        © 656 VQ Ven SX 6 000바에 8          | Deabte |
foter                                    hese ante
2,923.43                 vile               2,923.80               2,931.42
| Com nom                      09
2,924.59                  010.61                  2,926.29                  2,937.06           | x08        】                       뒤                                                    여여 sateee
2,913.98                      roo                   2,910.03                    2,920.53                    €                          Gt isomnar ented
4                         5                         ~                                                                                                                        [ < 기
2,914.00                      2803                    2,911.65                    2,927.22                                                 om                               기 =r
2,905.97                       7959                    2,916.93                    2,931.15         을 Name                                                                           Copy response                            ~
wordDaylisuso.              f       —
2,915.56          v3.81         2,921.75         2,923.95      =               ;
은 | wonddaytisuse..    Block request domain         Copy at PowerShell
1                   2,919.37                 ¥ 10.20                2,921.83                2,923.79            — wortsOayustso Replay XHR                         Copy as fetch
wortsDaytistiso —                                             Copy as CURL (cred)
2,929.67          vio         2,936.76         2,940.91       =     ay        Save as HAA with content
2,930.75                                                                        _ woreOaytsuso— Copy as cURL (bash
,                        2280                 2,919.73                  2,934.80             | worleDayUstso. 200 ate        AP Oh Ts seep
18.09.19          2,907.95                 ale               2,906.69               2,912.6           LiwondDeytisto- 200 ww ppdom TI) ca, 개 의 fetch
Copy all as CURL (cred)
12345 678 9 0 Ge
a                  ㆍ                                                                      Copy a8 as CURL (bash)
om          ay      구게                                  ㆍ 70903 1 5.4 KB transferred                        Loans sit se Mh

SARE URLS
SPI@SPX&fdtc=0&page=39J UC. 이 URLS

https://finance.naver.com/world/worldDayListJson.nhn?symbol=
브라우저 주소창에 넣고 실행시키면 SS 결과
얻은 ISON 형태의 데이터가 브라우저에 표시됩니다. 총 10개네요.

7장 금융공학 모델링 121


===== PAGE 122 =====
6                                                         -      x
Cy sar 550 네이버 38     XD brpey/tinance nsvercomwor 제아                            a

€ > C a hitps//finance naver.com/workd/workdDayListison nhin?symbel =SPI@SPXEfdtc= O&page=3     xr 2 @

UC sy" "S18  syed": ~20181213". "oven" : 2558.7. “hich”: 2570.18. * low": 2637. 27.  “clos”: 2650.54. “dif f~:-0.53,  6  -0.02.“001":2364352580) .

"6" SP 169 107 1120181212" "0007": 2658 .23. “hich”: 2685. 44. * low"! 2650.28. "clos":2651 .07. “dif f"' 14. 23 ."rate”  £0.54, "evol":2473051770} .
(Cave SIPC oa "20181211". 개  $2884.44. “high” 2674.35." 10"12621.3."0109"12636 .78."01((":-0.94.       @":1-0.04.“0701":235456343아 .
("syed") "SP 109 “60907 :120181210" . “oven”: 2530.85. “high”: 2647.51.” low" 125863.23.7<10671 12637 .72.7101119 14 .64. “rate®  0.18, "avol": 2521728990} .

(i syeb" "SP 169." 120181207" . “cnen™: 2591.26. “hich”: 2708 54," low": 2623.14. “cl os": 2633 .08. “dif f*:-62.87."rate*:-2.33."avol”: 2607989520} .
("syn") "SP 1609 ." xyad™! "20181206" , 10007": 2653.51, "high": 2685.15." 1007 2521.53. "0106"! 2695 95, “dif f*:-4.11,"rate": -0.15. “ovol": 3220645160} .
("6 “95169 .* ya”: “2018 1208" . “cen”: 2762. 43, "high": 2765 .93.7 low": 2697.18. "clos": 2700.06. "dif f*:-90.31, "rate" *-3.24."evol”: 2990888250} .
"696" 1 "SP 16S." xynd™: “20181203" . “coen*: 2750.5, “high”: 2800.18." 1007 12773 .38."clos*: 2790.37. "dif f":30,2, "rate: 1.08, "gvo!": 2752398030} .
{syr! "SPIES, * yd": "20181130" , “ooen”: 2737.75, “high” :2760.83." low" :2732.76. “clos”: 2760.17, "dif f*:22.41 “rate”: 0 82,"9vol”* 3061710890} .
{syeb" = "SP 1G.“ xyed™:°20181123" . “coe”: 2736 .97. “high”: 2753.75.° low" :2722.94. "clos": 2737.76. "dif f*:-6.03. "rate": -O 22, "avol”: 2102760320} ]

데이터를 찾아오는 데 성공했으니 이제 이 JSON 파일을 크롤링하는 단계로 넘어가보겠습니다.
우선 크롤링에 필요한 PSS 호출합니다. 0\Ｌ에서 소스를 읽어오는 1110, 읽어온 JSON
파일을 해석하기 위한 json, 크롤링한 데이터를 담기 위한 WejA(pandas)S 호출합니다(팬
더스에 대해서는 다음 장에서 설명합니다).

1 import pandas as pd

2 from urllib.request import urlopen

3 import json # 해외지수는 json HES HSE
Out

아까 가져온 URLS 보면 물음표(?) 뒤에 따라붙는 인수 중 지수코드를 나타내는 5/0001과
페이지 번호를 나타내는 pages 바꿔가며 JSONS 호출하는 것을 알 수 있습니다. 우리도 이
부분을 크롤링을 하기 위해 이 두 인수를 변수화합니다.

1 symbol = ‘NII@NI225'
2 page = 1

Out

ㅇ

ㅣ 두 BS 주소에 포함시킨 후 10060 ( ) 함수를 이용해 URLS 호출해 JSON 데이터를
불러오고, 1500. 1080 ( ) 함수를 이용해 JSON 데이터를 해석해 data 변수에 저장합니다.

-

url = ‘https://finance.naver.com/world/worldDayListJson.nhn?symbol=' +symbol+'&fdtc=@&pag
e='+str(page)

nN

raw = urlopen(url)
data = json. load(raw)

122 2% 주식과 지수


===== PAGE 123 =====
Out

BAe 데이터를 확인해봅시다. Bee JSON 데이터는 03132 변수에 리스트 형태로 저장되어
있습니다. 03+3[0]으로 리스트의 A 번째 데이터를 확인해볼까요?

1 0212[0]

Out {'‘symb': 'NII@NI225',

‘open’: 20264.82,
‘high’: 20571.28,
‘Low’: 20204.43,

‘diff’: 195.59,
‘rate’: 0.96,

"gvol': 80694300}

이번에는 첫 번째 데이터 중 우리가 필요한 부분만을 뽑아보죠. 날짜와 종가가 필요한데, a
터를 잘 살펴보니 'xymd' ol] 날짜가, ‘clos' ol] 종가가 들어 있는 것이 보입니다. 이 두 부분
추출해봅니다. 우선 날짜입니다.

>

1 data[@]['xymd']
Out ‘20190115'

의번에는 송가입너다:

1 data[@][‘clos']
Out 20555.29

이제 한 페이지에 있는 SF SS 4] 데이터 중 날짜와 종가만 뽑아 딕셔너리에 저장해보겠습니다.

d = dict()

for n in range(len(data)):
date = pd.to_datetime(data[n]['xymd']).date()
price = float(data[n][‘clos'‘])

> WN RP

7장 금융공학 모델링 123


===== PAGE 124 =====
5                    미 0316] = price
6            00050):

Out    {datetime. date(2019,  1, 15): 20555.29, datetime. date(2019,  1, 1):  20359.7, datetime.
date(2019, 1, 10): 20163.8, datetime.date(2019, 1, 9): 20427.06, datetime. date(2019, 1,
8): 20204.04, datetime.date(2019, 1, 7): 20038.97, datetime.date(2019, 1, 4): 19561.96,
datetime.date(2018, 12, 28): 20014.77, datetime.date(2018, 12, 27): 20077.62, datetime.
date(2018, 12, 26): 19327.06}

1행에서는 빈 딕셔너리를 선언합니다. 2행에서는 데이터 개수만큼 순환하면서 처리할
수 있도록 선언하고, 3행은 각 행의 SAS, 4행은 종가를 추출합니다. 3행에서 00.10_
datetime() 함수는 가져온 데이터를 날짜 형태로 바꿔주는 함수입니다. 5행에서는 {날짜 :
종가} 형태로 딕셔너리에 저장합니다.

지금까지 한 내용을 함수로 만들어봅니다. 함수 이름은 (630_1500( )으로 하고 크롤링한 데
이터를 저장할 딕셔너리 0, 지수코드 59000,  기 번호 pageS 전달받아 크롤링을 수행하
고, 크롤링이 완료된 딕셔너리 dS 반환하는 함수입니다.

1     def read_json(d, symbol, page=1):

2        url = ‘https://finance.naver.com/world/worldDayListJson.nhn?symbol=" +symbol+'
&fdtc=@&page='+str (page)

3          raw = urlopen(url)

4         data = json. load(raw)

5

6          for n in range(len(data)):

7              date = pd.to_datetime(data[n]['xymd']).date()

8             price = float(data[n][‘clos*])

9            d[date] = price

10

11        if len(data) == 10:

12            page += 1

13          read_json(d, symbol, page)

14

15        return (d)

Out

1행의 함수 선언부에서 0296=1이라고 표현한 AS 페이지 번호가 입력되지 않으면 기본값으

124 2부 주식과 지수



===== PAGE 125 =====
로 페이지 번호 1을 사용한다는 뜻입니다. 11행에서는 이 페이지에서 불러들인 데이터가 10
개인지를 확인합니다. 페이지에서 불러들인 데이터가 10개 미만이라면 이 페이지가 마지막
페이지라는 뜻이기 때문에, 데이터가 10개면 이후에서 다음 페이지를 또 불러오고, 그렇지 않
으면 더 이상 다음 페이지로 진행하지 않도록 처리하기 위해서지요.

이제 이 함수를 실행해봅시다. 함수를 실행해서 결과를 담을 566165를 만들고 (historical_
index) 실제로 함수를 호출해 이 시리즈에 담습니다(시리즈에 대해선 10장에서 설명합니다).

1 historical_index = pd.Series()
2 historical_index = read_json(historical_index, symbol, page)

Out

이제 결과를 확인해보면 원하는 대로 일본 Nikkei 225 지수를 수집했습니다.

1 historical_index.head(3)

Out 2019-01-15    20555.29
2019-01-11    20359 .70
2019-01-10    20163.80
dtype: float64

이제 여러 SSS 한꺼번에 수집해보죠. 먼저 수집할 지수의 SES 딕셔너리에 담습니다.

1       indices = {

2           "SPI@SPX' : ‘S&P 500’,

3       "NAS@NDX' : ‘Nasdaq 100',
4           "NII@NI225' : ‘Nikkei 225'
5     }

Out

해외 지수의 AEE 웹사이트상에서 확인할 수 있는데, 화면 위쪽의 지수 이름 옆에 작은 글씨
또는 URL 마지막 부분에 있습니다. 다음 그림에서 빨간색으로 표시된 부분입니다.

7장 금융공학 모델링 125


===== PAGE 126 =====
=   ㅁ   x
TI sar sco 네이버 ㅎㅎ     x Ey betpsyfirance nseencomyacts x | +
© + Cf https //financenaver.com’world/sise nhn?symbelf SPIOSPX]                                 xy 2 @:

BBS RUB GB ANB BS 투자전략 뉴스  )/07금융 추천증목

MAGS OMB AU ＊ ㆍ(한국거려수) SHS 중한 포털 ＊[한국은령) 100대 BANS [HA] 글로벌 겹세 리포르 - (Bt) 사람둘이 지스하도록 sey
S&P 500=지 이근 MB 20191 4 ees MTZ 기은     2m
2,582.61                UU 2,596.26        고가 2,589.32          525 UD 2.940.91
HUES! VW 13.65(-053%)        시가 2,580.31         저가 2,570.41           52주치퍼 2,346.58         소스

딕셔너리에 담아놓은 해외 지수들을 한꺼번에 불러오겠습니다.

1 historical_indices = dict()

2 for key, value in indices.items():

3     print (key, value)

4      s = dict()

5     5 = read_json(s, key, 1)

6     historical_indices[value] = s

7 prices_df = pd.DataFrame(historical_indices)

Out

1행에서 결과를 담을 딕셔너리를 선언하고, 2행에서 딕셔너리를 순환하도록 한 후 앞에서 만
le read_json() 함수를 호출해 결과를 담는 식입니다. 이제 결과를 확인해봅시다.

1  prices_ df. tail(3)

Out             S&P 500 Nasdaq 100 Nikkei 225

2019-01-11 2596.26       6601.40      20359.70

2019-01-14 2582.61      6541.04           Nan

2019-01-15       Nan           Nan     20555.29

1월 15일에 미국 지수들이 NaN 값으로 나타나는 것은 개장 전에 데이터를 추출해서 그렇습
다. 한국과 미국의 시차 때문이라고 이해하면 됩니다. 1월 14일은 일본 증시 휴장일이고요.

ㅇ1제 날짜를 지정해주는 부분을 구현해보겠습니다. 7.1절에서 만들었던 date_format() 함
수를 업그레이드 할 건데, 날짜를 받아와서 파이썬이 사용하는 실제 날짜 형식으로 바꿔서 돌

426 2% 주식과 지수



===== PAGE 127 =====
려주는

기능에 추가해, 날짜에 공백이 들어오면 오늘 날짜를 반환하는 기능을 구현하겠습니

다. 오늘 날짜를 지정하는 이유는, 딱히 날짜가 지정되지 않으면 오늘 날짜를 기준으로 데이터
를 수집하도록 처리하기 위해서입니다.

1 def date_format(d=''):

2      yy @ [Ee Mg

3          this_date = pd.to_datetime(d) .date()

4      else:

5         this_date = pd.Timestamp.today().date() # 오늘 날짜를 지정
6      return (this_date)

Out

이제 날짜 처리 부분까지 추가한 해외 지수를 크롤링하는 전체 함수를 만듭니다. 함수 이름은

index_

global ()= 정하고, 결과를 담을 딕셔너리 0, 지수코드 5/0001Ｌ, 시작 SH start_

date, 끝 날짜 670_02+6, 페이지 번호 pageS 입력으로 받는 함수입니다.

on DUN fF WN

10
11
12
13
14
15
16
17
18

def index_global(d, symbol, start_date='', end_date='', page=1):

end_date = date_format(end_date)
if start_date = '':
start_date = end_date - pd.DateOffset(months=1)

start_date = date_format(start_date)

url = 'https://finance.naver.com/world/worldDayListJson.nhn?symbol=' +symbol+'
&fdtc=0&page='+str (page)

raw = urlopen(url)

data = json. load(raw)

if len(data) > 0:

for n in range(len(data)):
date = pd.to_datetime(data[n]['xymd']).date()

if date <= end_date and date >= start_date:
# start_date2} end_date 사이에서 떼이터 저장

7장 금융공학 모델링 127


===== PAGE 128 =====
index_global(d, symbol, start_date, 600 0216, page)

19                  # 종가 처리

20                price = float(data[n][‘clos'])
21                # 덕셔너리에 저장

22               이 0316] = price

23            elif date < start_date:

24            # start_date O/HO/F 항수 종료
25               return (d)

26

27        if len(data) == 10:

28            page += 1

29

30

31     return (0)

Out

3행에서는 끝 SAS date_format ) 함수에 넣어 날짜 BHOS 바꿔줍니다. 만일 끝 날짜
가 지정되지 않으면 오늘 날짜를 끝 날짜로 합니다. 4행에서는 시작 날짜가 있는지 체크하고,
만일 시작 날짜가 없다면 5행에서 시작 날짜를 끝 날짜보다 한 달 앞으로 지정합니다. 이하 부
분은 앞에서 살펴본 (680_1507 ( ) 함수와 동일합니다.

이제 함수를 실행시켜보겠습니다. 시작 날짜는 2019년 1월 1일, 끝 날짜는 2019년 3월 31일
로 지정합니다. 그런데 이 SS 작성한 시점이 1월 15일 저녁이라 3월 31일이 아닌 현재까지
존재하는 데이터만 수집될 겁니다. 없는 데이터를 Hols FE 없는 노릇이니까요.

Out

16 NOU WN Ph

historical_indices = dict()

start_date = ‘2019-01-01’

end_date = '2019-@3-31'

for key, value in indices.items():
s = dict()
5 = index_global(s, key, start_date)
historical_indices[value] = s

prices_df = pd.DataFrame(historical_indices)

결과를 확인해봅니다.

428 2부 주식과 지수



===== PAGE 129 =====
1 prices_df

Out                    S&P 500 Nasdaq 100 Nikkei 225
2019-01-02 2510.03     6360.87         Nan
2019-01-03 2447.89     6147.13         NaN
2019-01-04 2531.94     6422.67  19561.96
2019-@1-07 2549.69     6488.25  20038.97
2019-01-e8 2574.41     6551.85  20204.04
2019-01-09 2584.96     6600.69  20427.06
2019-01-10 2596.64     6620.94  20163.80
2019-01-11 2596.26     6601.40  20359.70
2019-01-14 2582.61     6541.04         Nati
2019-01-15      Nati         NaN  20555.29

의도한 대로 해외 지수가 깔끔하게 크롤링되었습니다. 1월 2일 및 3일에 Nikkei 225 지수가
NaNO 표시된 것은 일본 증시가 1월 4일부터 개장해서입니다.

데이터프레임으로 여러 딕셔너리를 테이블 하나로 합치기
이제 S&P5002+ KOSPI200 지수의 2017년 1월 1일부터 현재까지 데이터를 뽑아서 각각
60500, (0501200이라는 딕셔너리에 저장하도록 하겠습니다. 우선 KOSPI200 지수부터 합니다.

1 index_cd = 'KPI2@@'
2 historical_prices = dict()
3  kospi2@@ = historical_index_naver(index_cd, '2017-1-1', '2017-12-31')

Out

Oo} Ho S&PS00 지수를 가져옵니다.

1      index_cd = 'SPI@SPX'

2       historical_prices = dict()

3     50500 = index_global(historical_prices, index_cd, ‘2@17-1-1', '2017-12-31')
Out

두 지수의 데이터를 구하긴 했는데 50500, (<0501200이라는 서로 다른 통(딕셔너리)에 담겨 있

7장 금융공학 모델링 129


===== PAGE 130 =====
는 상태입니다. 엑셀 실습에서 했던 것처럼 두 데이터가 한 통에 같이 담겨 있으면 작업하기가
수월할 텐데 말이지요. 그래서 파이썬을 엑셀처럼 만들어주는 팬더스를 또 사용하겠습니다.

먼저 위에서 생성한 두 딕셔너리를 tmpek= 하나의 임시 딕셔너리로 합쳐서 모양을 보겠습니다.

1 tmp = {'S&P500' : 50500, '(0501200' : (0501200 }
2 tmp

Out {'KOSPI200': {datetime.date(2017, 1, 2): 260.36,
datetime.date(2017, 1, 3): 262.97,
datetime.date(2017, 1, 4): 263.12,
datetime.date(2017, 12, 28): 324.74},
*"S&P500': {datetime.date(2017, 1, 3): 2257.83,
datetime.date(2017, 1, 4): 2270.75,
datetime.date(2017, 1, 5): 2269.0,

~

datetime.date(2017, 12, 29): 2673.61}}

{'KOSP1200': {kospi200 딕셔너리}, 'S&P500': {50500 딕셔너리} } 형태로 두 딕셔너리가
하나의 딕셔너리로 합쳐진 것이 보이죠?

새로 만들어진 딕셔너리를 마치 엑셀처럼 사용하고 싶다면 어떻게 할까요? 이를 위해 팬더스
라이브러리를 가져와보도록 하죠.

1 import pandas as pd

Out

팬더스 라이브러리에서 데이터를 엑셀처럼 사용할 수 있게 해주는 BME pd. DataFrame ( )
입니다. 이 함수를 이용해서 tmp 딕셔너리를 엑셀 스프레드시트 형태의 데이터프레임으로 바
꾸겠습니다. 바꾼 데이터프레임(스프레드시트)은 0+라는 변수에 저장합니다.

1 df = pd.DataFrame(tmp)
2 df.sort_index(inplace=True)
3 df

430 2% 주식과 지수



===== PAGE 131 =====
Out                    KOSPI 200 S&P 500
2017-01-02 260.36 !     Nan}

2017-01-03      262.97 2257.83
2017-01-04              263.12 2270.75
2017-01-05            261.98 2269.00
2017-01-06            263.20 2276.98
2017-01-09            263.74 2268.90
2017-01-10      263.73 2268.90
2017-01-11      268.15 2275.32
2017-01-12            269.95 227044
2017-01-13      267.91 227464

2017-01-16         266.15 [9]

((0501200과 50500 딕셔너리가 아라는 스프레드시트에 보기 좋게 저장되었네요. 그런데 Nan
이라는 처음 보는 값이 보입니다. 이는 데이터가 없다는 뜻입니다. 아마도 2017년 1월 2일과
1월 16일은 미국 증권시장 휴장일이 아닐까 생각됩니다. 다른 나라의 데이터를 비교하다 보
면 나라마다 서로 공휴일이 달라서 데이터가 빠지는 경우가 SGU. 이를 처리하는 가장 쉬
운 방법은 빠진 날짜를 제거하는 것이지만 절대 추천하지 않습니다. 존재하는 데이터를 없애면
데이터의 SSO] 단절되어 왜곡되기도 하고 데이터의 신뢰도에 악영향을 미치기 때문입니다.

금융에서는 매도 가격과 매수 가격이 맞아떨어져 거래가 체결되면 시세가 바뀌는데, 거래가
체결되기 전까지는 이전 체결 가격을 시세로 인정합니다. 온종일 거래가 없다면 전일 종가가
그날의 시세로 연장되는 것이지요. 위 표에서 1월 16일은 1월 15일 지수를 연장하면 되겠네
요. 그러면 1월 2일은 어떻게 할까요? 당연히 2016년 12월 30일의 지수를 가져와야겠지만
12월 30일도 데이터가 없다면 이야기가 달라집니다. 계속 하루씩 더 당기는 노가다를 지속하
는 것은 프로그래머의 자세가 아니죠. 아쉽지만 그냥 1월 3일 지수를 당겨옵니다.

이렇게 빠진 데이터를 채우는 것을 수학에서는 보간이라고 합니다. 데이터프레임은 보간을 위
한 몇 가지 방법을 제공하는데, 금융 데이터 처리를 위해 여기에서 사용하는 보간을 위한 방
Yl DataFrame. fillna(method='ffill' ) 또는 DataFrame.fillna(method='bfill' )
입니다. ffill& ‘forward fill, 4 앞의 데이터로 뒤의 구멍을 채우라는 뜻이고, bfille
‘backward fill’, 즉 뒤의 데이터로 앞 구멍을 채우라는 뜻입니다. 이를 이용해 코딩을 해보면

7장 금융공학 모델링 131


===== PAGE 132 =====
다음과 같이 됩니다.

1      df = df.fillna(method='ffill')

2      if df.isnull().values.any():

3          df = df.fillna(method='bfill')
4      df

Out               KOSPI200 S&P 500

2017-01-02       260.36 2257.83
2017-0103 262.97 2257.83
2017-01-04       263.12 2270.75
2017-01-05       261.98 2269.00
2017-01-06           263.20 227698
2017-01-09           263.74 2268.90
2017-01-10       263.73 2268.90
2017-01-11      268.15 2275.32
2017-01-12       269.95 2270.44
2017-01-13           267.91 2274.64

2017-01-16        266.15 227464

2047 04 47        67 77.    2287 20.

1월 2일에는 1월 3일 데이터가, 19 16일에는 1월 13S 데이터가 채워진 것을 볼 수 있습니다.

이제 데이터 처리를 위한 모든 준비가 완료되었으니 필요한 전체 데이터를 다시 받아봅시다.
지금까지는 데이터를 가져오는 시간을 아끼려고 2017년 데이터만 가지고 ASS 진행했지만,
우리가 보고 싶은 데이터는 금융 위기 직전인 2008년 1월 1일부터의 데이터입니다. 데이터를
가져오는 데 시간이 좀 걸리겠지만 한 번만 받아오면 되니까 잠깐 참고 기다립시다. 워크스페
이스 앞에 10[12]처럼 워크스페이스 번호가 나오는데, 프로그램이 실행 중일 때는 번호가 *
표시로 바뀌면서 10[*]처럼 BPAUCH, * 표시가 다시 숫자로 바뀌면 실행이 완료된 것입니다.

KOSPI200 지수를 가져옵니다.

1 index_cd = 'KPI200'
2 historical_prices = dict()
3  kospi20@ = historical_index_naver(index_cd, '20@8-1-1', '2017-12-31')

Out

132 25 주식과 지수



===== PAGE 133 =====
이번에는 S&P500 지수를 가져옵니다.

index_cd = '50610506※×'
historical_prices = dict()

3       50500 = index_global(historical_prices, index_cd, '2008-1-1' ,   12017- 12- 31° )
Out
각 지수 딕셔너리를 합칩니다.

1  tmp = = Aly S&P500"  3 50500, "KOSPI200"    : 60501200

딕셔너리를 데이터프레임으로 변환합니다.

1 df = pd.DataFrame(tmp)

Out

구명 채우기를 실행합니다.

1 df = df.fillna(method='ffill')
2 = df.isnull().values.any():
3       df = df; Tilia Cocthode bfill')

최종 ATS 확인해봅시다. 그런데 20084 12 1일부터 현재까지의 데이터를 다 S BRE 없
겠죠? 여기에서는 데이터 앞단의 일부만 확인해보겠습니다. 이럴 uf DataFrame.head ()
라고 명령하면 앞에서부터 5줄만 출력해줍니다(앞에서는 인수로 3을 넣어 3개만 출력했습니다).
반대로 tail )이라고 하면 뒤에서부터 5줄을 출력합니다.

1 df.head()

73 금융공학 모델링 133


===== PAGE 134 =====
Out                       KOSPI 200 S&P 500
2008.01.02 23530 1447.16
2008.01.03 234.67 1447.16
2008-01-04 235.77 1411.63
2008-01-07 231.00 ㆍ 1416.18
2008-01-08 230.34 1390.19

축하합니다. 지금 막 금융 빅데이터와 금융 머신러닝의 시작점이자 가장 손이 많이가고 번거
로운 과정인 데이터 스크레이핑을 성공적으로 완성했습니다.

MBSA 0/Seq 그래프 그리기

이번에는 앞에서 만들어둔 S&P5002} KOSPI200 지수 데이터를 가지고 그래프를 그려보
겠습니다. 파이썬에서 사용할 수 있는 그래프 라이브러리는 여러 가지가 있지만 MSRA
(matplotlib)°] 가장 널리 쓰이고 있습니다. WSeHol] 대해서는 4부에서 상세하게 AVS
예정입니다.

우선 RSS OLE 07010 BSS [나라는 이름으로 가져옵니다.

1 import matplotlib.pyplot as plt
2 ‘%matplotlib inline
MSKAS 그래프를 이미지 파일로 만들어서 화면에 뿌려주는데, 따로 설정해놓지 않으면 별
도의 화면을 열어서 ABS 확인해야 해서 여간 번거로운 게 아닙니다. 노트북을 사용할 때
는 2행에 있는 명령어 USS 삽입하면 노트북 워크스페이스상의 결과 화면에 그래프가 함께
뿌려지도록 지정할 수 있습니다.

ㅁ나라는 이름으로 Sele pyplot 모들을 이용해 그래프의 크기 조절, 그래프로 나타낼 데이
터 지정, 범례 위치 지정, 그리드 출력을 합니다. 여기에서는 우리가 만든 함수를 이용해 수집
해온 S&P500 지수와 KOSPI200 지수를 그래프로 그리겠습니다.

134 2부 주식과 지수


===== PAGE 135 =====
1 plt.figure(figsize=(10, 5)) # 크기 조절
2 ㅁ나-010【(아['560500'])  ＊ G/O/E{ 선택
3 plt.plot(df['KOSPI2@0' ])
4 plt.legend(loc=@) # 범례 위치 지정
5 plt.grid(True, color='@.7', linestyle=':', linewidth=1)  # 그리드 설정
Out        a
2500 4 —— KOSPI200
2000
1500
1000
500
SYS ooo               es te |
0  2008  2009  2010  2011  2012  2013  2014  2015  2016  2017  2018

엑셀 실습 때와 마찬가지로 5&82500에 비해 KOSPI200 지수의 값이 작아서 KOSPI2002] 움
직임은 잘 보이지 않네요. KOSPI2002} S&P500 모두 이미 지수이지만 비교 가능성을 위해
다시 한 번 지수화 작업을 해줍니다. 지수화는 다음 식을 참고하세요.

비교 시점 가격(지수)
기준 시점 가격(지수)

지수 =                           ×100

1월 1일은 공휴일이므로 기준 시점은 2008년 1월 2일로 합니다. 그러려면 전체 데이터를
2008년 1월 2일 자 데이터로 나뉘야 합니다. 데이터프레임(0+)에서 특정 일자의 데이터
를 뽑아내는 WHS 리스트 사용법과 유사한데, 데이터를 선택할 때 Male 아니라 레이블
로도 선택할 수 있다는 점에서 훨씬 수월합니다. 리스트에서 다섯 번째 데이터를 뽑아내려
면 [15[4]라고 지정한 것과 유사하게 데이터프레임에서는 03【라「8006.1100[4]라고 하
면 됩니다. 순서 대신 날짜로 지정하려면 DataFrame. loc[*'S4' ]라고 하면 됩니다. 10<는

'1002000`을, iloc ‘index 10023000“을 줄인 표현입니다.

1 df.ilocle] # 인덱스(위치)로 지정

Out (0501 200   235.30
580 500      1447.16
Name: 2008-01-02, 01106: float64

7장 금융공학 모델링 135


===== PAGE 136 =====
1 df.loc{dt.date(2008, 1, 2)] # 값(날짜)으로 지정
Out KOSPI 200   235.30
S&P 500      1447.16
Name: 2@@8-@1-02, dtype: float64

이 방법을 이용해 20084 19 2일을 기준으로 지수화한 그래프를 다시 그려보겠습니다.

plt.figure(figsize=(16, 5))

plt.plot(df["S&P500'] / df['S&P5@0'].loc[dt.date(20@8, 1, 2)] * 100)
plt.plot(df[‘KOSPI268'] / df['KOSPI20@'].loc[dt.date(2008, 1, 2)] * 100)
plt. Llegend(loc=@)

on ^ WN

plt.grid(True, color='@.7', linestyle=":', Linewidth=1)

Out

— S&PS0O

1807 —_ xosp200

160

140

120

100

40

2008     2009     2010     2011     2012     2013     2014     2015     2016     2017     2018

이제 KOSP12002] 움직임이 한눈에 들어옵니다. 이번에는 전체 데이터(07)에서 2016년 1월
1 일부터의 움직임만을 주려서 보려 합니다. 추려낸 데이터는 지수화시커 0_「3110_2016_ㅁ004
에 담겠습니다. 데이터프레임.100[시작:끝]으로 데이터프레임의 일부만 조회할 수 있습니다.

1 df_ratio_2016_now = df.loc[{dt.date(2016, 1, 1):] / df.loc[dt.date(2016, 1, 4)] * 100
2 df_ratio_2016_now.head(3)

Out                        KOSPI200 S&P 500

2016-01-04 100.000000 100000000
2016-01-05 100639304 100201226
2016-01-06 99987214 98887045

136 2% 주식과 지수


===== PAGE 137 =====
2016년 이후의 지수가 2016년 최초 거래일인 1월 4일을 기준으로 새롭게 지수화되어 07_
ratio_2016_nowol] 담긴 것을 확인할 수 있습니다.

추려낸 데이터로 새롭게 그래프를 그려보겠습니다.

1 plt.figure(figsize=(10, 5))
2 plt.plot(df_ratio_2016_now[ 'S&P5@0'])
3 plt.plot(df_ratio_2016_now[ 'KOSP1200' ])
4 plt.legend(loc=@)
5 plt.grid(True, color='0.7', linestyle=':', linewidth=1)
Out
— S&P500
160 KOSPI200
130
120
110
100
50
2015-12   2016-03   2016-06   2016-09   2016-12   2017-03   2017-06   2017-09   2017-12
=    =

이번에는 회귀분석을 이용해 두 지수의 상관관계를 분석해보겠습니다. 회귀분석에 들어가기

전에

두 지수를 가지고 ABEE (scattered ㅁ1!0)를 그려보겠습니다.

nn & WN KF

plt.figure(figsize=(5, 5))
plt.scatter(df_ratio_2016_now[ 'S&P500'], df_ratio_2016_now['KOSPI200'], marker='.')

plt.grid(True, color='@.7', linestyle=':', Linewidth=1)
plt.xlabel('S&P500' )

plt.ylabel( ‘KOSPI200' )

73 금융공학 모델링 137


===== PAGE 138 =====
Out

a3
40                                                              r “S&S
he        3
a=            Bes
i
       &
gheF-
F
no                   fb. ㆍ
100             aK  A
a
a
0           100          130          120          130
5500

회귀분석을 위해서는 <163「0.110623「_0ㅁ0061ㄴＬ 내의 LinearRegression 라이브러리를 사용
j                      합니다. 벡터화된 데이터 처리를 위해 넘파이(44018) 모듈도 함께 사용됩니다. 넘파이는 3
|                         부에서 소개하겠습니다.
{                                    0) 우선 numpy2} LinearRegression 라이브러리를 호출합니다.
@ S&P500 지수가 KOSP12009F] 미치는 BARS 보려는 분석이므로, 2 KOsSP1200°] 주가
는 분석이기 때문에 ×값인 SB Y= (independent variable) += S&P500 지수를,
값인 종속변수(061060ㅁ060ㄷ\23112116)에는 KOSPI200 지수를 넣습니다.
@ LinearRegression BBS ㅁ행 1열 벡터를 입력받기 때문에 지수 데이터를 (2, 1) 모
양으로 변경합니다. Array.reshape(-1, 1)= 벡터 형태를 바꿀 수 있습니다.
@ LinearRegression9] fit 명령어로 회귀분석을 시행합니다.
(6) 회귀분석 Sale! 기울기는 ‘Slope’, 》절편은 ‘Intercept’, #"값은 '『^2'라는 키
에 저장한 딕셔너리를 반환합니다.

import numpy as np
from sklearn.linear_model import LinearRegression

x = df_ratio_2016_now['S&P500']
y = df_ratio_2016_now['KOSP1200"]

# 171 칼럼 np.array2 변환
independent_var = np.array(x).reshape(-1, 1)

on 6 UN FF WN

138 2% 주식과 지수



===== PAGE 139 =====
9 dependent_var = np.array(y).reshape(-1, 1)

10

11 # Linear Regression

12 regr = LinearRegression()

13 ~regr.fit(independent_var, dependent_var)

14

15 result = {'Slope’:regr.coef_[@,0], ‘Intercept':regr.intercept_[@], ‘R*2':regr.
score(independent_var, dependent_var) }

16 result

Out {'Intercept': -28.225304749250498,
"R®2': @.92106589000891268,
"Slope’: 1.2880855621471596}

회귀분석이 완료되었습니다. 기울기는 1.29, *절편은 -28.23, RE 0.92입니다.

이 추세선을 그래프로 그려봅니다.

1 plt.figure(figsize=(5,5))
2 plt.scatter(independent_var, dependent_var, marker='.', color="skyblue')
3  plt.plot(independent_var, regr.predict(independent_var), color='r', lLinewidth=3)
4 plt.grid(True, color='@.7', linestyle=":', Linewidth=1)
5 plt.xlabel('S&P500' )
6 plt.ylabel(*KOSPI200' )
Out |    7

추세선이 보기 좋게 나오네요. 엑셀 실습에서 봤던 바로 그 모습입니다.

7장 금융공학 모델링 139


===== PAGE 140 =====
지금까지 인터넷에서 주식이나 지수의 종가를 추출하고, 그래프로 그려서 비교해보고, 상관관

그
pas

계를 분석하는 등 금융공학에서 많이 사용하는 패턴 BAS 해보았습니다. 수고하셨습니다.

7.2 K10 지수 산

이번에는 KOSPI200A1 4 한국 10대 기업의 주가를 이용해서 10 지수를 만들어보겠습니다.
금융 이론과 엑셀 ASS 통해 익숙해진 내용입니다만. 10 지수를 만들기 위해 필요한 것들
은 구성종목 각각의 과거 시세(종가) 및 날짜, 상장주식 수, 유동비율 등이 있습니다. 이러한
데이터들은 데이터 스크레이핑을 통해 구해오도록 하겠습니다.

네이버에서 한국 10대 기업 데이터 수집하기

이번에는 네이버에서 데이터를 수집해보도록 하겠습니다. 먼저 상장주식 수와 유동비율입
니다. 필요한 데이터가 들어 있는 화면을 찾는 것이 첫 과정입니다. 웹 AWS 통해 http: //
companyinfo.stock.naver.com/v1/company/c1010001.aspx?cmp_cd=005930 에서
삼성전자의 기업 정보 데이터를 발견했습니다. 다음 그림에서 빨간색으로 표시되어 있는 부분
입니다. 상장주식 수를 구하려고 하는데 화면에는 발행주식 수라고 표시되어 있네요. 엄밀히
구분하면 다른 용어이지만 네이버에서는 발행주식 수와 상장주식 수를 같은 개념으로 사용한
듯합니다. 다른 곳에서 찾아본 상장주식 수와 같은 수치로 나와 있습니다.

삼성전자 & $ 005930  %ㅠ599 05065 «KOSH AJIT \65: 반도체왼반도체장비
타55.421  60530.427 0 9.20 ㅣ 업롱『07.58 0001.64 ㆍ -선금비당수익률 1.7196            결산기 : 12월
FPR 진월자 보통주 SESSA ERS ㆍ헨금래당수역료 쇠근 고신 수정마<(신금)/ Dun 보통주 수정주기
P PBR PE ESS 수청주기 / 최근결산 BPs     ㆍ WACS WISE th 11096 Clasatcation Standard, modified by WISE
P PER 린이 (- 전 ME SSO 같미 (~)연 AWM eA S| 의미합니다
시세 및 주주현황                        [기준:2018.05.16]
주가/전입더비/수익료          49,8508 / +6508 /+13259 주가/상대수익월                    Haa
nm                                          (기
52605 최고/최저                         57,5208 / 4.2208       ia                                            on
액면가                                             1008       Ee                                        siete
19                                        5000
거래탕/거러더금                                          15.918.700주 / 7,923.5 8               bed                                                                                ed
[                                        200
시가출역                                     3,200,033 4 8       「                                        8000
2                                        mono
52주베타                                            65        °                                        2S.000
WUFAS/R Belo                                              {=<
eee eye     oe      °
— 삼성전자 — \6050대비(자) — 전기전자대비(좌)
수익률 Gwaveay     09796 +1.7396/-10.6794 +7.99%    Bray

140 2% 주식과 지수



===== PAGE 141 =====
화면을 찾았으면 이제 데이터 스크레이핑을 위해 필요한 라이브러리를 호출합니다.

1 import 054
2 from urllib.request import urlopen

Out

위에서 찾아낸 URLS 변수에 담아 스크레이핑을 준비합니다.

1 url_float = ‘http://companyinfo.stock.naver.com/v1/company/c10100@1.aspx?cmp_cd=@05930'
2 # Floating ratio from Naver

3  url_float

Out ‘http://companyinfo.stock.naver.com/v1/company/c1@10001.aspx?cmp_cd=805930'

1 source = urlopen(url_float).read()
2 soup = bs4.BeautifulSoup(source, ‘lxml')

Out

앞선 실습에서 했던 것과 같이 XPathS 이용해서 원하는 BRS 뽑아보도록 합니다. of, 그런
데 큰 문제가 있네요. 네이버가 마우스 오른클릭을 하지 못하도록 막아놓았습니다. 이런 경우
에는 어떻게 할까요? 조금 번거롭지만 방법은 있습니다.

© 화면을 조금 늘려보면 가장자리에 내용이 없는 하얀 여백이 생기고 그 부분에 마우스를

가져간 후 오른클릭을 해서 BAR 메뉴를 SS (EE [6떠]+| 6101+| | |)하면 화면 오
른쪽에 XPath 조회를 위한 화면이 나옵니다.

/weowisee 7st x \ Ga

c  © compamynto stock. naver.com/v1/company/<1010001 agulcneSanp c= 0059 308imenuTypextiock               eit  oS!
ATER 7TAQ | 제무분석. FRNH | Des Theta Reee     ane
MASA @ 이 09930 = 이제이 이더 BADN wos EL ebes Te                       이 영역에서 오른클릭
주  wma  pms  cies  리거  vasveciins       aun ee
AN SEU eSS OTSA /이20218   ㆍ현기해알수약용 OS Ro OTOMKN a) DUN BSS OTSA                        .
fon REGNGS SESN/DSNS EOS _swmce wexninach chumeann Seroen meatal puree          a20)          ance Cul
PATHE IE 언거수이4 ORO Bees BOBO                                                    "
알으로07          이은주 Gea
시세 일 주주선황              [기푼.2008093)                                     4228@
PYsRaee      eset) senjnes PYeASNS             goon    ne cigoe NEw.        티제
™                        *                             .
52905 Most             V8 (48    aa                       oon      can                  wi?
a2                        1908         2077.02    SA ax      feo.
UBER + S108          =             버
nayoaas           sa / DES     rom   rns yn a=      eae eam
sloth                  ae
a4                           139652008        아어 PAS             ad        NAN 소스 wiv)              met
2700                                                       나      aA              Cortera
cen         a am

|

7장 금융공학 모델링 141


===== PAGE 142 =====
@ 소스 코드 부분에서 마우스를 움직이면 소스에 해당하는 화면 Yolo] 음영으로 표시되
며 이 소스가 어느 부분을 표시하는 화면인지 알 수 있습니다. 우리가 찾으려는 '발행주
식수/유통비율' 정보는 화면 왼쪽에서 다음 부분에 있습니다.

시세 및 주주현황                           [기준:2018.05.16]
주가전일대비/수익즐         49,850원 / +650원 / +1.32%
52000 최고서:                                      57,520원 / 44,2208
액면가                  1                                            1008
ABE               15,918 7005 / 792388
wee         3,200,033 8
MESNG/R Bue                     |   6,419,324,700% / 72.78%
2320              52.74%
수익률 38413           DST] +1.7356/ -10.63%/ +7.48%
+ 수정주개(차트포힙), BSS 기준, + 52주베티: 주간수익률 기준

@ 오른쪽에 표시되는 소스에서 이 부분이 어디인지를 찾아야 합니다. 오른쪽 소스 코드가
표시된 부분에서 [041]+[ㄷ를 누르면 다음 그림과 같이 검색창이 나타나는데, 이곳에
우리가 찾을 정보를 입력하면 됩니다.

CR 6] ㅣ Blements Console Sources » 41) 은 Xx

< 10 TYPE bred PUBLIC * ine bedi HTML 4.01
Transitional //iN" “http: //ser.ws.org/TR/html4/loose.dtd~
pe chtm] lawgeko style) mae js Fakiiox 00000
canvas _Canvastext _webgl | mo-touch geolocation postressage
hashch    history draganddrop
websockets rgba hsla eultipledgs backgroundsize
borderimage borderradius boxshadow textshadow opacity
cssanimations      1     Cssgradients cssreflections
csstransforms csstransforms3d csstransitions fontface
generatedcontent video audio localstorage sessionstorage
webworkers applicationcache svg inlinesvg smil
000 = 0                    =

> chead>_</head>
» <body oncontextmenu-"return false™>—</body>
</html>

find by string, selector, or XPath                ~~} Cancel
Styles Computed Event l     DOM Break     »
Filter                    다며 .cls +) =

elerent.style {

}

@ 왼쪽에서 '6,419,324.700주 / 72.78% S 드래그하고 복사해서 오른쪽 검색창에 붙여넣
기합니다. 붙여넣기하자마자 검색창 위에 해당 코드가 검색될 것입니다. 노란색으로 표
시된 부분이 바로 우리가 찾고자 하는 부분의 코드입니다.

142 2 주식과 지수



===== PAGE 143 =====
대 GC) Etements  Console Sources Network Performance»   A1p ix
ae   I    Pctro</tr>  ae eae  0 a  ~
> <tr>_</tr>
> <tr>-</tr>
> <tr></tr>
v<tr>
<th scope="row™ class="txt™> WU t42/f Sule    |
</th>
<td class="num"™>

</td>
</tr>
> <tr>_</tr>

| ice  Jee Le ee tof t[~ 00 0000

® 이제 해당 코드 위에 마우스를 놓고 오른클릭을 한 후 나타나는 팝업 메뉴 중 Copy
> Copy XPath 메뉴를 차례로 클릭합니다.

두 0 Elements Console Sources Network Performance »  41 : x
Ph <troic/tr>   2"  겼
> <tr>-</tr>
> <tr></tr>
Ph ctrou</tr>

v«tr>
<th scope="row™ class="txt" > WUt44/2 Sls     al
</th>
-*                    Add attribute
Edit as HTML                                                              S
의 그        ScTB11_ tbody 00
|6,419,324,700% / 72.                            90000 사레 점 |
본                                            5            '     t
Styles Event Li                              st
Filter                         Hide element
Paste element
element.style {         Force state         >
»                             Break on             »       Copy outerHTML

table.gtHead th, t

th, table. gHeadd3                        |     Copy selector
table.gHead®l td,      Expand recursively
.                XPath
height: 25px;       Collapse children
padding-top:
padding-bottom         Scroll into view
Si hed ake

© 노트북으로 돌아와 워크스페이스상에서 [Ct] +(V]S 눌러 복사해온 XPath 주소를 확
인해봅니다. XPath 주소는 //*[010="61811"]/1『000//ㅠ[7]/1입니다. 파이썬 코드
로 작성해봅니다. tbody 빼고, ㅠ[7]과 a 여러 데이터가 들어 있는 리스트로 나타
난 PMS find alle, 10처럼 하나만 있는 것은 finds! 잡아냄니다. 파이썬은 카운트
를 0부터 시작하니까 ㅠ[7]은 find_all(‘tr' )[6]으로 잡아옵니다.

1  soup. find(id=" cTB11" '2- find alc tr’ )(6). td. text

Out ‘\r\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t128, 386, 494주 / 72. 78x\r\n\t\t\t\t\t\t\e\t\e\e\t\
t\t\t'

7장 금융공학 모델링 143


===== PAGE 144 =====
@ 뽑아내려는 데이터가 정확히 나왔습니다! 그런데 \r, \n, \t 같은 것들은 보기가 aul
요. 뽑아낸 문자열을 임시로 \깨라는 변수에 넣고 tmp. replace )로 없애줍니다.

1 tmp = soup. find(id='cTB11').find_all(‘tr’)[6].td.text
2 tmp = tmp.replace('\r', ‘')

3 tmp = tmp.replace('\n', ‘')

4 tmp = tmp.replace('\t', '')

5

Out ‘6,419,324, 7005: / 72.78%"

© 훨씬 깔끔해졌지만 아직 데이터로 가치를 발휘하기에는 조금 부족합니다. 상장주식 수
와 유동비율을 따로 잘라서 각자 변수로 넣어주어야 데이터로 활용이 가능합니다. 이를
위해 두 값 사이에 있는 슬래시 (/ )를 기준으로 데이터를 분리합니다.

(9) 문자열을 분리하거나, 추출할 때는 re 라이브러리를 사용하면 편리합니다. 「6에 대한
자세한 공부는 18장에서 하기로 하고, 여기에서는 우선 re BSS 호출하겠습니다.

Ue    import re

Out

@re.split() 함수를 이용해 문자열을 / 기준으로 분리합니다.

1 tmp = re.split('/', tmp)

Out  ale 6,419,324, thong 0   72.78%' mi

@ tmp 리스트에 잘려진 문자열이 저장되어 있습니다. 2} 문자열을 확인해봅니다.

1 tape]
Out ‘6,419,324, ,700주 1

@® 44-24] += outstanding 변수에 정수형(10) 데이터로 넣고, 유동비율은
floating 변수에 2-4 (float) 데이터로 넣어주면 좋을 것 같습니다. 이를 위해
100[0]에서는 숫자만 추출합니다.

144 2% 주식과 지수


===== PAGE 145 =====
1 outstanding = tmp[@].replace(',', '')

2 outstanding = outstanding.replace('=', '')
3 outstanding = outstanding.replace(' ', '')
4  ne

Out '6419324700'

09 tmp[1] WAS 소수를 표현하기 위해 숫자.숫자 형태로 추출하고 % 기호를 없애줍니다.

floating = tmp[1].replace(' ', '')

floating = floating.replace('%', '')
3  flosting

Out '72.78'

@ 이제 추출한 데이터를 정수형, 소수형으로 변환해서 저장하면 완료됩니다. 두 변수값을
둘러싼 ' '가 사라지고 숫자형 변수로 바뀌었음을 확인할 수 있습니다(노트북에서는 문
자형 변수를 ' '로 둘러싸 출력합니다).

1 outstanding = int(outstanding)

2  pours tanding

Out 6419324700

1 floating = float(floating)
2  floating

Out 72.78

이제 지금까지 작성한 SAS 바탕으로 상장주식 수와 유동비율을 구하는 함수를 만들겠습니다.

1 구성종목 기본정보
2 def stock_info(stock_cd):

3      url_float = 'http://companyinfo.stock.naver.com/v1/company/c1010001.aspx?cmp_cd=' +
stock_cd

4      source = urlopen(url_float).read()

5      soup = bs4.BeautifulSoup(source, 'Lxml')

6

7      tmp = soup. find(id='cTB11').find_all('tr’)[6].td.text

7장 금융공학 모델링 145


===== PAGE 146 =====
10
11
12

14

16
17
18
19
20
21
22

tmp =
tmp =
tmp =

tmp.replace(‘\r', ‘')
tmp.replace('\n', ‘')
tmp.replace('\t', *')

tmp = re.split('/', tmp)

outstanding = tmp[@].replace(‘,', '')
outstanding = outstanding.replace('=', ‘')

outstanding = outstanding.replace(' ', '')

outstanding = int(outstanding)

floating = tmp[1].replace(' ', '')

floating = floating.replace('%', '')

floating = float(floating)

name = soup. find(id='pArea’).find(‘div’).find('‘div').find(‘tr').find(‘td').

find(‘span').text

k1@_outstanding[stock_cd] = outstanding
k1@_floating[stock_cd] = floating
k1@_name[stock_cd] = name

이번에는 K10 지수 구성종목을 지정하고 k10_component 리스트에 저장합니다. KOSPI 시
장 상장종목 중 시가총액 기준 상위 10개 종목입니다.

wo Ont DMN FF WN

sy
2

한국거래소 시가총액 상위 10종목 (2019년1월 기준)

005930
000660
668276
005380
207948
051910
005490
635420
017676

상성전자
하이닉스
셀트리온

현대차

상성바이오로직스
16화학

POSCO

NAVER

텔레콤

146 2% 주식과 지수



===== PAGE 147 =====
12 015760 한국전력

13 0170
14 k10_component = ['005930', '000660', '068270', '005380', '207940',\
15                   *@51910', '005490', '@35420', '017670', '015760']

함수를 호출해서 과거 시세를 받아올 차례입니다. 0『문을 이용해서 k10_component 리스트
내의 종목들을 순환하며 함수를 호출합니다. 상장주식 수, 유동비율  으으 € Fe S444
인 k1@_outstanding, k10_floating, k1@_nameS 초기화한 후 함수를 호출합니다.

1 k1@_outstanding = dict() # 딕셔너리 초기화

2 k1@_floating = dict()

3  k10_name = dict()

4 for stock_cd in k1@_component: # SSS 하나씩 순환하면서
5

stock_info(stock_cd) # stock_info #43 호출

Aslzy°] 담긴 k1@_outstanding (444 수)을 출력해봅니다.

1 k1@_outstanding

Out {'005930': 5969782550,
'000660': 728002365,
'068270': 127948184,
'005380': 213668187,
'207940': 66165000,
'051910': 70592343,
'005490': 87186835,
'035420': 164813395,
'017670': 80745711,
'015760': 641964077}

(10 _+102109(유동비율)도 마찬가지로 결과가 잘 나올 것입니다.

7장 금융공학 모델링 147


===== PAGE 148 =====
과거 주가 구하기

이제 10 각 구성종목의 과거 주가를 구해야 합니다. 주식의 일자별 시세는 네이버에서 수집
합니다. 이미 7.1절에서 KOSPI20 지수의 일자별 시세를 수집하면서 비슷한 작업을 했으니
이번에는 완성된 코드를 먼저 보고 달라진 부분만 확인하기로 합니다.

먼저 주식의 일자별 시세 수집을 위한 화면을 찾습니다. 화면은 다음 그림과 같고, uRLS
http: //finance.naver.com/item/sise_day .0110?0006=005930 입니다.

「                                                               v        -       ㅁ        x
O 네이버 ae             x 앤트
<  C @ finance.naver.com/item/sise_day. nhn?code=005930                    * Ge
일빌시새
날짜              중가              전일비               시가                 고가                저가             거래량

2018.09 09               2,460,000              a 40,000              2,413,000              2,472,000              2,410,000             197,548
DBO.        2,420,000       v 17,000        2,400,000        2,429,000        2,370,000       250,654
2018.64.05          2,437,000         a 91,000          2,370,000          2,469,000          2,367,000         264,912
2018.04.04              2,446,000            v 60,000             2,408,000             2,413,000             2,346,000           247,684
2018.04.03              2,406,000            ㅠ 21,000             2,394,000             2,407,000             2,364,000           255,365
2018.04.62                2,427,000              y 34,00              2,450,000              2,461,000              2,425,000             142,313
2018.03.30          2,461,000          a 9,000         2,454,000         2,495,000         2,454,000        155,542
2016.03.29              2,452,000            4 17,000             2,435,000             2,478,000             2,416,000           201,340
2018.03.28              2,435,000            ㅠ 64,000             2,455,000            2,455,000            2,417,000           303,189
2018.03.27        2,499,000       ㅠ 15,000       2,516,000       2,523,000       2,454,000      237,480

날짜 위에서 오른클릭을 하고 AAS 눌러서 소스 PES 확인하면 Yay} <td align=
“center”><span class='tah 010 gray03'></span></td> 태그에 쌓여 있습니다. <+[0>에
특별한 01855가 붙어 있지 않으므로 <5080>의 class= 이용해 추출해봅시다.

dates = source.find_all('span', class_="tah p10 gray@3')

종가 부분의 소스 SES BH <td class="num"></td= 쌓여 있습니다. 다음처럼 추출할
수 있네요.

prices = source.find_all(‘td', class_='num')

148 2 주식과 지수



===== PAGE 149 =====
을 파악했으니 본격적으로 시작해봅니다. 우선 날짜 처리와 데이터
러리를 호출합니다.

1 import datetime as dt

2 import pandas as pd

Out

이제 일자별 주가를 추출하는 함수 historical_stock_naver (SS

짜)를 만듭니다. 7.1절에서 작성한 date_format ) 함수를 재사용합니다.

tw
in
p25
바시
is
#
때
nf

1 def historical_stock_naver(stock_cd, start_date="", end_date='', page_n=1, last_page=@):
2

3     if start_date: # start_date7} 있으면

4         start_date = date_format(start_date) # date ZOOS 변환

5      else: # 없으면

6         start_date = dt.date.today() # 오늘 날짜를 지정

7      if end_date: # end_date7} 없으면

8         end_date = date_format(end_date) # date ZWOS 변환

9      else: # end_date7} 있으면

10         end_date = dt.date.today() # 오늘 3S end_date= 지정

11

12      naver_stock = ‘http: //finance.naver.com/item/sise_day.nhn? code=' + stock_cd +

‘&page=" + str(page_n)

13

14      source = urlopen(naver_stock).read()

15      source = bs4.BeautifulSoup(source, ‘Lxml')

16

17      dates = source.find_all('span', class_='tah 010 gray@3') # 날짜 수집
18     prices = source.find_all(‘td', class ='num') # 증가 수집

19
20     for n in range(len(dates)):
21

22        if len(dates) > 0:
23

7장 금융공학 모델링 149


===== PAGE 150 =====
24                       ㅎ 날짜 처리

25             this_date = dates[n].text
26             this_date = date_format(this_date)
27
28            if this_date <= end_date and this_date >= start_date:
29            # start_date2} end_date 사이에서 데이터 저장
30                 # 종가 처리
31                this_close = prices[n*6].text
32               this_close = this_close.replace(',', '')
33                this_close = float(this_close)
34
35              # 딕셔너리에 저장
36               historical_prices[this_date] = this_close
37
38            elif this_date < start_date:
39            # start_date 이전이면 함수 종료
40               return historical_prices
41
42      # 페이지 내비게이션
43     if last_page = 0:
44         last_page = source.find_all('table')[1].find('td', class_='pgRR').find(‘a')
['href’]
45         last_page = last_page.split('&')[1]
46         last_page = last_page.split('=')[1]
47          last_page = float(last_page)
48
49      # 다음 페이지 호출
50     if page_n < last_page:
51          page_n = page_n + 1
52       historical_stock_naver(stock_cd, start_date, end_date, page_n, last_page)
53
54      return historical_prices
Out

이번에는 함수를 호출해서 과거 시세를 받아올 차례입니다. forks 이용해서 k10_
component 리스트 내의 종목들을 순환하며 함수를 호출합니다.

150 25 주식과 지수


===== PAGE 151 =====
wo 6 이 DN FW NY =

k1@_historical_prices = dict()
for stock_cd in k1@_component:

historical_prices = dict()
start_date = '2017-1-1'
end_date = '2017-12-31'

historical_stock_naver(stock_cd, start_date, end_date)

k1@_historical_prices[stock_cd] = historical_prices

107] 642] 과거 데이터 전체가 k1@_historical_prices 딕셔너리에 담겼습니다. 지수 4
성을 위한 각종 AALS 편하게 할 수 있도록 딕셔너리를 (10 111510「1031_0ㅁㄷ166라는 이름의
데이터프레임으로 변환합니다.

1 k1@_historical_price = pd.DataFrame(k10_historical_prices)

Out

2 k1@_historical_price.sort_index(axis=1, inplace=True)

데이터에 구멍이 있을 수 있으니 보간 작업을 하고 k10S 출력해봅니다.

Out

k1@_historical_price = k1@_historical_price.fillna(method='ffill') # ffill2 구멍을 채우

고

if k1@_historical_price.isnull().values.any(): # 그래도 구멍이 남아 있으면
k1@_historical_price = k1@_historical_price.fillna(method="bfill')  # bfill@ 채워라

k1@_historical_price.head(3)

00660     0053380     005490       05930 015760     017670     035420     @s51910     068270     207940

2017-@1-@2 45800.0 150000.0 260500.0 1805000.0 43900.0 225500.0 777000.0 253000.0 108200.0 156500.0

2017-01-03 47250.0 153000.0 256000.0 1824000.0 44100.0 223000.0 767000.0 262000.0 106600.0 158000.0

2017-01-04 46500.0 154000.0 254500.0 1808000.0 43900.0 223000.0 810000.0 268500.0 106100.0 154500.0

7장 금융공학 모델링 151



===== PAGE 152 =====
~ |

이 시점에서 챙겨야 할 것이 있습니다. 삼성전자가 2018년 5월 4일부로 1/50 액면분할을
실시해 그날부터 주가는 이전의 1/50로 감소하고, 동시에 주식 수는 50배로 증가했습니다.
시가총액 =주가 × 주식 수이기 때문에 전체 시가총액에는 영향이 없지요. 하지만 우리는 인
터넷에서 무료로 구할 수 있는 데이터를 수집해 사용하기 때문에, 주식 수는 50배 증가된 현
재 데이터를 사용하지만, 주가는 1/50 감소 이전의 과거 데이터를 사용하는 셈이 됩니다. 따
라서 별도의 조치 없이 시가총액을 단순 계산하면 시가총액이 50배 높게 계산됩니다.

따라서 과거 주가를 50으로 나뉘 수정주가(20145660 [0ㅁㅇㅇ)를 구하는 FAS 추가해, 이를 이
용해 시가총액을 계산해야 합니다.

1 k10_historical_price['@05930'] = k1@_historical_price['@@5930'] / 50 # 삼성전자 액면분
할에 따른 수정주가 계산
2 k1@_historical_price. peau)

Out    |                  000660     005380     605490 | 005930| 015760     617670     035420     @51910     068270      207940

| 2017-61-02 45800.0 150000.0 260500.0 |36100.0] 43900.0 225500.0 777000.0 253000.0 108200.0 156500.0 |

| 2017-01-03 47250.0 153000.0 256000.0|36480.0| 44100.0 223000.0 767000.0 262000.0 106600.0 158000.0 |

| 2017-01-84 46500.6 154000.0 254500.0 |36160.0] 43900.0 223000.0 810000.0 268500.0 106100.0 154500.0

43/3741 (005930) 2] 주가가 앞에서 확인한 값보다 1/502 감소된 것을 sels
융회사에서도 시장에서 형성된 가격 ASS 표시하는 단순주가와 주식 수 변경
다시 계산한 수정주가를 구분해 사용하고 있으며, 야후 등 일부 사이트에서는
께 수정주가를 제공하기도 합니다.

지수 산출
지수를 산출하기 전에 수식을 다시 한번 살펴보겠습니다.

지수 = 비교 시점 시가총액

기준 시점 시가총액

(시가총액=주가×상장주식 수×유동비율 )

152 2부 주식과 지수


===== PAGE 153 =====
시가총액을 먼저 구해봅니다. 시가총액을 구하기 위해 10 각 종목별 상장주식 수×유동비
율 값을 구합니다. 앞에서 구해놓은 상장주식 -F (Outstanding), 유동비율(미023008), 주가
(Price), 633 (Name) 등의 칼럼을 가져와 임시(00) 딕셔너리에 저장한 후 (10_1070라
는 데이터프레임으로 만들어줍니다. 주가는 기준일자 주가를 사용하기로 합니다.

1 tmp = {‘Outstanding'
: k1@_floating,\

N

3

4

5
Out

‘Floating’

: k1@_outstanding,\

‘Price’ : k1@_historical_price.iloc[@],\
‘Name’ : k1@_name}

k10_info = pd.DataFrame(tmp)

금융에서 보통 AI7KEA (market capitalization) S 말할 때는 '주가×상장주식 수를 의미
합니다. 하지만 지수를 만들 때는 유동비율을 반영한 AI7EEA (market capitalization with
floating ratio)-& 이용하므로 두 가지 시가총액을 모두 구하겠습니다. 데이터프레임 칼럼을
통째로 불러와서 연산을 수행하고, Azle) 시가총액은 Market Cap 칼럼에, 유동시가총
액은 f Market Cap 칼럼에 저장합니다. 유동비율은 백분율로 나타낸 값이므로 계산을 위해
0.01을 곱해줍니다.

1 k10_info['f Market Cap'] = k10_info[‘Outstanding'] * k1@_info['Floating'] * k10_

info['Price'] * 0.01

k1@_info[ ‘Market Cap'] = k1@_info[‘Outstanding'] * k1@_info['Price'] * 0.01
k1@_info.head(3)

Out                    Outstanding Floating        Price                  Name f Market Cap      Market Cap
000660      728002365        73.89 45800.0           하이닉스 2.463678e+13 3.334251e+11
005380     213668187      66.33 150000.0             현대차 «=2.125892e+13 3.205023e+11
005490      87186835      79.60 260500.0             POSCO 1.807889e+13 2.271217e+11
005930    5969782550       78.75    36100.0           SSMAL 1.697135e+14 2.155092e+12
015760     641964077      48.86 43900.0           한국전력 1.376983e+13 2.818222e+11
017670      80745711      62.23 225500.0          델레큼 1.133094e+13 1.820816e+11
035420     164813395      78.70 777000.0             NAVER 1.007832e+14 1.280600e+12
951910      70592343      64.28 253000.0            ㄴ6화학 -1.148032e+13 1.785986e+11
068270       127948184        66.35 108200.0              셀트리온 9.185490e+12 1.384399e+11
2067940      66165000      24.76 156500.0 삼성바이오로직스 2,563854e+12 1.035482e+11

7장 금융공학 모델링 153


===== PAGE 154 =====
이번에는 일자별로 시가총액을 구합니다. AAR 종목별 일자별 시가총액은 k10_
historical_mc 데이터프레임에 저장하겠습니다.

1 k1@_historical_mc = k1@_historical_price * k1@_info['Outstanding'] * k10_info['Floating']
* 6.01

2 k1@_historical_mc.head(3)

Out                     600660          @e5380          eos490          005930          015760          017670

2027 2-463678e+33 2.125892e+13 1.807869e+13 1.697135e+14 1.376983e+13 1.1330940+13

ae 2.541676e+13 2.168409e+13 1.776658e+13 1.714999e+14 1.383257e+13 1.120532e+13

2027- 27501332€+23 2.182562e+13 1.766248er13 1.69995Ser14 1.376983e+13 1.120532e+13

지수 구성종목 각각의 시가총액을 모두 더해 K10 지수의 일자별 시가총액을 구합니다.

<떼이터프레임>.500() 은 각 열의 합 (세로 방향)
<떼이터프레임>.500(2×15=1) 은 각 행의 합 (가로 방향)

eee

| 0 & WN BP

k1@_historical_mc.sum(axis=1) # 일자별 시가층액 합

Out 2017-01-02        3.828017e+14
2017-01-03         3.844182e+14
2017-01-04           3.882579e+14
2017-01-85           3.830483e+14

~

10 지수의 일자별 시가종액을 10 데이터프레임에 저장하고, 현재가를 이용해 시가총액을
구해 10 데이터프레임에 추가합니다.

1 (10 = pd.DataFrame() # k10 데이터프레임 초기화

2 k1@['K10 Market Cap'] = k1@_historical_mc.sum(axis=1)
# 일자별 시가층액 AS

3  k10.head(3)

154 2% 주식과 지수



===== PAGE 155 =====
Out               206 Market Cap

2017-01-02    3.828017e+14
2017-01-03    3.844182e+14

2017-01-04    3.882579e+14

마지막 과정으로 201714 1월 2일 시가총액을 기준으로 K10 ASS 산출합니다. 산출한 지수
는 10 데이터프레임 내에 K10 칼럼에 저장합니다.

1 k10['K10'] = k10['K10 Market Cap'] / k10['K10 Market Cap'](@] * 100
2 k10.head(3)

Out                K10 Market Cap         K1e

2017-01-82    3.828017e+14 100.000000

2017-01-03    3.844182e+14 100.422277

2017-01-04    3.882579e+14 101.425324

지금까지 과거와 현재의 유동시가총액을 구하고 시가총액을 이용해 지수를 만들어보았습니다.

지수 그래프 그리기

10 지수 그래프를 그려봅시다. 우선 그래프 BS WSRUS 호출합니다.

1 import matplotlib.pyplot as plt
2  peratplotlib’ inline

Out

앞에서 구한 K10 지수를 그래프로 그립니다.

plt.figure(figsize=(10, 5))

plt.plot(k10['K10"])

plt. legend(loc=@)

plt.grid(True, color="0.7', linestyle=":', linewidth=1)

| -& WN PR

7장 금융공학 모델링 155


===== PAGE 156 =====
ont tes

140 5

130 4

120 4

no 4

100                                                                                                                                :

2017-01            2017-03             2017-05             2017-07             2017-09             2017-11             2018-01

KOSPI2002} 비교

우리가 만든 10 지수가 실제 KOSPI200 지수와 얼마나 비슷한지 그래프로 비교해봅시다.
비교를 위해 같은 기간의 KOSPI200 지수를 가져오겠습니다. 지수를 AS 때는 7.1절에서
만들어둔 historical_index_naver (지수코드, 시작 날짜, 끝 날짜) 함수를 사용합니다. 함
수를 이용해 BUS 지수 데이터는 <(0501200 딕셔너리에 저장합니다.

1 def historical_index_naver(index_cd, start_date="', end_date='', page_n=1, last_page=@) :
2
3      index_cd = index.cd # 인덱스 코드
4      page _n=pagen # 페이지 HS
5
6      if start_date: # start_date7} 있으면
7          Start_date = date_format(start_date) # date RWC? 변환
8      else: # 없으면
9          Start_date = dt.date.today() # OS 날짜를 지정
10      if not end_date: # end _date7} 없으면
11          end_date = dt.date.today() # 오늘 날짜를 end_date@ 지정
12      else: # end_date7} 있으면
13          end_date = date_format(end_date) # date 포멋으로 변환
14

156 2% 주식과 지수



===== PAGE 157 =====
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
32
33
34

35
36
37
38
39
40
41
42
43

45
46

47

49

naver_index ='http://finance.naver.com/sise/sise_index_day.nhn?code=" + index_cd +
‘&page="' + str(page_n)

source = urlopen(naver_index).read() # 지정한 페이지에서 코드 읽기
source = bs4.BeautifulSoup(source, ‘lxml') # 뷰티플 수프로 태그별로 코드 분류
dates = source.find_all('td', class_='date’) # <td 01255="021[6">태그에서 날짜 수집
prices = source.find_all('td', class_='number_1') # <td 61255="00006/_1">해그에서 지
수 수집
for n in range(len(dates)):
if dates[(n].text.split('.')[@].isdigit(Q):
# 날짜 처리
this_date = dates[n].text
this_date= date_format(this_date)
if this_date <= end_date and this_date >= start_date:
# start_date2} end_date 사이에서 데이터 저장
# 종가 처리
this_close = prices[n*4].text # prices 중 종가지수인 0, 4, 8... 번째 데이
터 추출
this_close = this_close.replace(',', '')
this_close = float(this_close)
# SA{L{2/0/ 저장
historical_prices[this_date] = this_close
elif this_date < start_date:
# start_date 이진이면 함수 종료
return historical_prices
# 페이지 내비게이션
if last_page = 0:
last_page = source.find(‘td', class_='pgRR').find('a')['href']
# 마지막 패이지 주소 추출
last_page = last_page.split('&')[1]  # & 뒤의 page=506 부분 추출

7장 금융공학 모델링 157


===== PAGE 158 =====
50         last_page = last_page.split(’=")[1] # = 뒤의 페이지 번호만 추출

51         last_page = int(last_page) # 숫자형 변수로 변환

52

53      # 다음 페이지 호출

54     if page_n < last_page:

55         Ppage_n = page n+i1

56       historical_index_naver(index_cd, start_date, end_date, page_n, last_page)
57

58      return historical_prices

Out

이제 함수를 호출해서 KOSPI200 지수를 추출해옵니다.

1 historical_prices = dict() # 딕셔너리 초기화
2 (0501200 = historical_index_naver('KP1200', '2017-1-1', ‘2017-12-31')
3 kospi20e
Out {datetime.date(2017, 1, 2): 260.36,
datetime.date(2017, 1, 3): 262.97,
datetime.date(2017, 1, 4): 263.12,

그래프를 그리기 위하여 (0501200 딕셔너리를 k200 데이터프레임으로 변환합니다.

1 (200 = pd.DataFrame({'K200' : kospi200})
2 k200.head(3)

Out                                  K200

2017-01-02 260.36
2017-01-03 262.97
2017-01-04 263.12

K10 지수가 KOSPI200 지수와 얼마나 비슷하게 움직이는지 비교하기 위해 10과
KOSPI200 지수를 함께 그려봅니다.

158 2뿌 주식과 지수


===== PAGE 159 =====
plt.figure(figsize=(10, 5))
plt.plot(k10[‘K10'] / k10[‘K10'][@] * 100)
plt.plot(k200['K200'] / k20@['K200'][@] * 100)
plt. legend(loc=0)

plt.grid(True, color='@.7', linestyle=':', lLinewidth=1)

Out | 150

OU 은 WN

=. K10
— 200

140 +

130

120 4

110

100

2017-01            2017-03            2017-05            2017-07             2017-09            2017-11            2018-01

KOSPI200 지수보다 10 종목이 훨씬 가파르게 상승한 AS 볼 수 있습니다. 한국
10개 종목이 상위 200개 종목보다 더 많이 올랐다, 즉 주식시장 상승을 주도했다는
프가 보여주고 있네요.

지금까지 한국 증시 10대 종목의 2017년 1년간의 시세를 수집해서 데이터프레임에 저장하고,
이를 이용해 10 지수를 산출해서 그래프를 그리고, KOSPI200 지수와 비교하며 금융공학의

주요 관심사인 지수 산출 과정을 실습해봤습니다.

7장 금융공학 모델링 159


===== PAGE 160 =====
블록체인과 금융산업

블록체인0510001010)은 데이터를 모아놓은 '블록'을 '체인'처럼 연결해 공유하면서
데이터의 무결성을 보장하는 새로운 개념의 보안 기술입니다. 지금은 블록체인 기술을
이용해 만들어진 비트코인이 유명세를 타면서 마치 금융상품인 것처럼 포장되어 세상
에 알려져 있지만 블록체인 자체는 금융이 아니라 기술을 지칭합니다. 실제로 블록체

인은 금융뿐 아니라 물류, 제조 등 다양한 분야에서 활발하게 연구되고 있습니다.

블록체인 기술의 핵심은 공유입니다. 블록체인을 분산원장기술(ㅁㅠＬ1, distributed
ledger technology )°]@} 부르기도 하는 이유이지요. 블록체인 개발 이전까지 데이터
는 관리자에 의해 중앙집중식으로 저장되고 관리되었으며, 관리자는 정보력의 우위를
이용해 우월적 지위를 누리고 있었습니다. 하지만 블록체인 세계에서 데이터는 관리자
에게 집중되지 않고 네트워크상의 모든 사람에게 공유되기 때문에 우월적 지위를 누릴
수 있는 위치 자체가 사라지겠지요.

관리자도 없는데 블록체인은 어떻게 데이터의 무결성을 보장할 수 있을까요? © 데이
터 입력, 변경 등으로 새로운 데이터가 블록에 입력되면 © 블록체인 내부 알고리즘이
네트워크상의 모든 노드(컴퓨터)에 이를 전파하고 © 과반수 이상의 노드가 새로운 데
이터가 정상적인 경로로 입력됐다는 응답을 주면 © 블록은 새로운 데이터를 수용하게
됩니다. 이렇게 왕정이 아닌 민주주의식으로 네트워크가 운영되는 방식이 블록체인이
추구하는 데이터 세상인 것입니다.

블록체인이 꿈꾸는 이상향은 기존 금융산업의 구조와 정면으로 배치됩니다. 금융산업
은 기본적으로 규제 산업입니다. 지금은 라이선스를 가진 금융회사가 규제의 보호 아
래 소비자를 상대로 손쉽게 돈을 벌고 있지만, 블록체인 네트워크에는 규제도 라이선
스도 존재하지 않기 때문입니다.

이를 쉽게 이해하기 위해 현재 우리나라에서 주식을 거래하는 과정을 살펴볼까요? 주
식을 사고 싶은 투자자 &가 있다고 합시다. ㅅ는 증권회사에 가서 계좌를 개설하고 매
수 주문을 합니다. 증권회사가 소비자가 제출한 주문을 거래소로 전달하면 거래소는
여러 소비자가 제출한 매수, 매도 주문을 모아 매매를 성사시키고 그 결과를 증권회사

160 2% 주식과 지수



===== PAGE 161 =====
와 한국예탁결제원(<612)으로 전달해줍니다. 증권회사는 소비자의 계좌에 거래 결과
를 기록하고, 한국예탁결제원이 주식 명의자 이름을 매도자에서 AB 변경하면 거래가
종료됩니다. 거래 과정에 소비자가 직접 참여할 기회는 없는 것이지요.

이 과정을 블록체인으로 처리하면 어떻게 될까요? 주식을 사고 싶은 투자자 AE 증권
회사에 갈 필요 없이 직접 블록체인 네트워크에 참여해 거래 상대방을 찾아 거래를 하
면 됩니다. 이론적으로 증권회사, 거래소, 한국예탁결제원이 더 이상 필요하지 않게 됩
니다. 하지만 블록체인 시대가 되어도 여전히 모든 투자자가 블록체인 네트워크에 직
A 참여할 정도로 기술력을 갖추지는 못하기 때문에 투자자들을 도와줄 증권사는 필요
할 것입니다. 비트코인의 유행과 함께 우후죽순처럼 생겨난 암호화폐거래소가 바로 주
식시장에서 증권사의 역할을 하는 것입니다. 그렇다면 거래소나 한국예탁결제원은 없
어질까요? 이들 역시 이론적으로는 필요가 없지만 거래에 수반되는 각종 위험 관리를
하는 중재자로 남아 있을 수 있습니다. 하지만 위상이 크게 떨어질 수 밖에 없겠죠.

그러면 블록체인을 이용한 금융의 장점은 무엇일까요? 지금까지는 주식거래 과정에서
증권사, 거래소, 한국예탁결제원에 수수료를 지불해야 했지만 블록체인 네트워크에서
는 이곳에 수수료를 낼 필요가 없어집니다. 저렴한 수수료가 블록체인을 이용한 금융
거래의 최대 장점인 것이죠.

금융권에서 블록체인이 가장 먼저 도입되고 있는 SAS 송금입니다. 한국에 있는 아
빠가 스웨텐에서 유학하는 딸에게 생활비를 보내는 경우를 봅시다. © 한국에 있는 시
중 은행에서 원화를 달러로 환전하고, (3) 한국의 은행에 수수료를 내고 달러를 스웨덴
으로 BUC 한국의 은행과 스웨덴의 은행은 직접 거래가 안 되어 인터뱅크라 불리
는 은행 간 송금 전문 SBS 이용해야 합니다. @ 인터뱅크 수수료를 내고 한국의 은
행에서 스웨덴의 은행으로 SHS 송금합니다. © 스웨덴 은행에 수수료를 내고 입금
처리를 합니다. © 스웨덴 은행에 환전 수수료를 내고 달러를 스웨덴 크로나화로 환전
합니다.

반면 이 거래를 블록체인으로 한다면 (1 원화를 지불하고 비트코인을 삽니다. (3) 비트
코인 네트워크를 이용해 스웨덴의 딸에게 송금을 합니다. © 비트코인을 지불하고 스

7장 금융공학 모델링

161


===== PAGE 162 =====
웨덴 크로나화를 삽니다. 현재의 은행을 이용해 송금하면 다섯 차례 수수료를 지불해
야 하지만, 블록체인을 통해 송금하면 세 차례만 수수료가 발생합니다. 비트코인이 이
상적으로 세상에 정착한다면 0, @ 단계의 수수료조차도 발생하지 않겠죠. 블록체인
기술은 송금 수수료를 챙기던 많은 금융기관을 퇴출시킬 것입니다.

이처럼 블록체인 기술은 금융권에 엄청난 파급효과를 초래할 것으로 예상됩니다. 그래
서 기득권을 가진 글로벌 금융기관들은 경쟁적으로 블록체인 기술 연구에 매진하고 있

습니다. 블록체인 때문에 퇴출되는 것이 아니라 새로운 블록체인 네트워크를 만들고,
이 네트워크를 운영하는 신진 세력으로 성장하고 싶어서입니다.

블록체인 사업은 페이스북이나 카카오와 같은 플랫폼 사업입니다. 다수의 사용자를 확
Bet 메인 플랫폼이 되면 다양한 서비스를 추가하며 엄청난 영향력을 발휘할 수 있게
되지요. 메신저 사용자 기반을 바탕으로 게임, 웹툰, 쇼핑, 미디어 등 다양한 영역으로
사업을 확장하고 있는 카카오를 떠올려보세요. 플랫폼 사업은 처음에 진입하기는 어렵
지만 한번 자리 잡으면 독점 효과를 누리며 수많은 이윤 ASO} 기회가 생기게 됩니다.
글로벌 금융기관이 블록체인 기술에 뛰어드는 이유도 이와 같지요.

162 2부주식과 지수



===== PAGE 163 =====


===== PAGE 164 =====
Chapter8 선물의 개념
Chapter9 선물 엑셀 실습
ChopterlO 코딩 기술: 반복되는 데이터

Chopterll 금융공학 모델링



===== PAGE 165 =====
을   Lie a                          Chapter 8
선물의 개념

8.1 선물이란?

선물거래란 선물(%#0)이라는 한자어 그대로 미래에 필요한 상품을 미리 거래하는 것입니다.
따라서 거래를 할 때(거래일) 바로 상품이 넘어가지 않고 약속한 날짜(만기일)가 되어야 상품
이 넘어갑니다. 당연히 돈도 물건을 받는 날 지급하며, 계약 시점에는 약간의 보증금만 주고받
을 뿐입니다.

한 번도 보지 못한 상대방과 보증금만 걸고 맺은 계약이 실제로 이행될 거라고 어떻게 믿을 수
있을까요? 계약할 때는 유리할 것으로 예상하고 추진했지만, 막상 만기가 다가와보니 불리해
졌다면 계약을 파기하고 싶어지는 것은 인간이라면 당연한 심리겠지요. 그래서 선물, 옵션 등
파생상품 거래에서는 거래 상대방의 신용이 매우 중요합니다. 만일 거래소가 보증하는 거래라
면, 거래 상대방의 신용 위험은 거래소가 보증해줍니다. 하지만 거래소 밖 장외시장에서 일어
나는 거래는 거래 당사자끼리 알아서 방어막을 설치해야 합니다. 그래서 똑같은 거래도 거래
소 안에서 일어나는지, 밖에서 일어나는지에 따라 이름을 달리 붙입니다. 거래소가 보증하는
거래를 선물거래, 그렇지 않으면 선도거래라고 합니다.

그럼 선도거래의 예를 보겠습니다.

“유전 재벌 만수르는 계속 떨어지는 원유 가격이 걱정이다. 앞으로도 지금처럼 돈을 물 쓰듯
쓰고 싶지만 자꾸만 발전하는 셰일가스 기술에 신경이 쓰인다. 프리미어리그 축구단 하나 산
것으로는 만족할 수 없어 내년 6월에는 메이저리그 야구단을 하나 사고 싶은데, 원유 가격이

8장 선물의 개념 165



===== PAGE 166 =====
지금 수준인 배럴당 $50는 유지해야 살 수 있을 것 같다. 마침 만수르는 원유 가격이 올라갈
까 봐 걱정하는 정유 재벌 구도일과 내년 6월에 지금 가격인 배럴당 $50에 원유 100만 배럴
을 매매하기로 계약을 체결한다.”

위 계약은 원유 선도 계약입니다. 만수르는 선물 매도자, 구도일은 선물 매수자입니다. 기초
자산은 원유이고, 만기는 내년 6월, 정산 가격은 50입니다. 만일 내년 6월에 원유 가격이
$60로 올라가면 롱 BAAS 취한 구도일은 $60짜리를 $50에 사게 되어 배럴당 $10, 종
$10,000,000(=$10 x 1,000,000)2] 이익을 얻습니다. 반대로 만수르는 그만큼의 손해를 봅니다.

거래소도 비슷한 계약을 할 수 있는 ASS 제공합니다. 원유 가격을 기초자산으로 하는 선물
상품인데, 가장 유명한 것은 미국 거래소인 시카고상품거래소(6848)에 있는 서부 텍사스 중

질유(\71. West Texas Intermediate) 선물상품입니다. 만수르도 구도일도 직접 선도 계약
을 하는 대신 시카고상품거래소에서 서부 텍사스 중질유로 비슷한 계약을 하면 거래 상대방과
위험 없이 편하게 거래할 수 있겠지요. 하지만 ASS 개인투자자를 고려해 표준화된 거
래만을 제공하기 때문에 거래 물량이 BAU 특이한 AAS 원하면 선도거래를 선택하기도 합
니다.

8.2 선물거래의 특징

시작부터 매도할 수 있다

앞의 예시 거래에서 만수르는 유전을 들고 매도를 시작했지만, 팔 물건이 아무것도 없는 사람
도 거래 시작부터 매도를 할 수 있습니다. 주식시장과 같은 일반적인 현물시장에서는 주식(상
품)을 갖고 있어야 팔 수 있는 것과는 다른 개념입니다. 공매도 같은 특수한 거래는 제외하고
말이지요. 처음 선물시장에서 거래를 시작하는 사람도 주가 하락을 예상한다면 선물 se 포지
션을 취하면서 거래를 시작할 수 있습니다.

선물에는 승수(074101>110ㅁ)라는 개념이 있습니다. 선물 1계약당 가격을 결정하는 것인데, 일
종의 거래 단위라고 생각하면 됩니다. 기초자산 지수에 승수를 곱하면 선물 1계약의 가격이


===== PAGE 167 =====
됩니다. KOSPI200 선물은 승수가 25만 원인데, 지수가 300인 경우 선물 1계약의 가격은
7,500만 원(=300 ×250,000원×1계약)이 됩니다.

선물 가격=기초 자산 지수(가격)× 승수×계약

+

8

승수만 변경해가면서 동일한 기초자산을 가지고 여러 가지 선물상
국거래소에는 KOSPI200 선물 이외에 미니 코스피 선물이라는 상
KOSPI200 선물과 동일하게 KOSPI200 지수를 기초로 해서 만든 상품이지만 승수를 5만
으로 해서 선물 계약당 금액을 낮춰놓은 것이 특징입니다. 지수가 300인 경우 미니 코스피 선
= 1계약의 가격은 1500만 원(300×50,000원)이 되는 것이지요. KOSPI200 선물의 가격이
워낙 높아서 개인투자자들이 매매하기 쉽지 않다는 AS 보완하기 위해 낮은 금액의 상품을
만든 것입니다. 삼성전자는 주가가 200만 원을 훌 넘는 귀족주가 되면서 소액투자자의 투자
가 어려워지자 주식가격을 1/50로 낮추는 액면분할을 해서 주가 수준을 기존의 1/50로 낮추
었습니다. 거래 가격을 낮추면 더 많은 투자자가 거래할 수 있게 되고, 이에 따라 주식의 수요
가 높아져 주가가 더 상승하기를 바란 것이겠죠. 미니 코스피 ASE 비슷한 셈입니다. 승수는
상품마다 다르게 정해지는데, 2018년 2월 기준 한국거래소에서 거래되는 대표적 지수선물 상

품들의 ore 다음과 같습니다.

을 만들 수 있습니다.
도 있는데, 이 상

띠

ㅇ oh

oH
때

lq
re

c

KOSPI200 “3/341                       250! 원
미니 코스피 선물/옵션                     5만원
KOSPI200 변동성 지수 선물/옵션         25만원

이처럼 파생상품은 동일한 기초자산이라도 승수만 바꾸면 다양한 상품이 나올 수 있습니다.

증거금만 있으면 거래 가능: 레버리지 효과

선물 계약은 기본적으로 후불입니다. 즉, 만기 시점 또는 계약의 청산 시점에 정산을 하는 것
입니다. 하지만 불특정 다수 간의 거래에 따른 부도 위험에 대비해 계약 시점에 보증금 성격의
증거금을 부과합니다. 증거금은 상품에 따라 비율이 다른데, KOSPI200 지수선물의 위탁증거
Bee 7.5%입니다. KOSPI200 지수가 300인 경우, KOSPI200 선물 1계약에 해당하는 증거

8장 선물의 7d 167


===== PAGE 168 =====
금은 5,625.000원(=지수×계약 수×승수×증거금율=300 x 1 x 250,000 ×7.5%)입니다. 투자
자는 5.625.000원만 있으면 7.500만 원어치 ASS 거래할 수 있게 됩니다. 이렇게 상대적으
로 적은 자본으로 큰 규모의 매매를 하는 AS 레버리지(16067248ㅇ)라고 합니다. 투자자는 레
버리지를 이용해서 보유한 자산 대비 큰 손익을 취할 수 있게 됩니다. 증거금율은 거래소가 정
하며, 시장 상황에 따라 수시로 변경됩니다. 시장의 가격 변동이 심해 위험이 높아질 것으로
예상되면 증거금을 높이고, 반대의 경우 낮추게 됩니다. 2017년 10월에는 1주일 이상의 긴
추석 연휴로 가격변동성이 커질 위험이 있어 연휴 전에 미리 증거금율을 일시적으로 높이기도
했습니다. 해외 거래소의 경우에도 증거금은 보통 3~15% 수준입니다.

레버리지에 대한 안전장치: 일일정산과 마진콜

투자자뿐 아니라 투자자와 거래하는 상대방도 7.5% 보증금만 내고 거래를 합니다.
격 변동이 커서 상대방이 납입한 7.5%의 증거금보다 많은 돈을 날리고 파산하면 나는 이익금
을 어더에서 받을까요? 나와 거래한 상대방이 계약을 이행하지 않을 위험을 거래상대방 위험
이라고 합니다. 거래소가 보증하는 선물거래는 거래상대방 위험을 방지하기 위하여 일일정산
을 합니다. 만기일에만 정산하는 것이 아니라 매일 정산을 하는 것이죠.

=

a

런ㄷ
ro

||

오늘 KOSPI200 선물을 지수가 300일 때 1계약 매수했는데 장 마감 시 지수가 3012 끝났다
고 하면 지수의 차이인 1포인트만큼 이익을 보게 되지요. 이익금 25만 원(=1×250,000원)은
계좌에 플러스가 됩니다. 매도를 한 사람은 반대로 계좌에서 25만 Slo] 마이너스가 되겠지요.

위탁증거금인 계약 금액의 7.5%만 계좌에 넣고 거래를 시작한 사람이 돈을 잃고 잃고 잃다가
계좌가 8-5-0] 되면 거래 상대방은 어떻게 될까요? 거래소는 이러한 사태가 발생하지 않도록
유지증거금 제도를 운영합니다. KOSPI200 선물의 유지증거금율은 5%인데, 증거금이 선물
A :                내려가면 투자자에게 위탁증거금만큼인 7.5%에 맞추도록 돈을 추
[로 남부하게 하는 제도입니다. 만일 투자자가 추가 납부하지 않으면 거래소는 임의로 투자
자의 포지션을 청산합니다.

168 3부 선물


===== PAGE 169 =====
8.3 선물의 가치

다음은 행사가가 300인 KOSPI200 선물을 매수한 경우 수익률 그래프입니다. 선물은 지수의

움직임과 상관없이 행사가로 매매하기로 약속한 상품이므로, 행사가인 300을 기준으로 지수가
300보다 높으면 (지수 - 행사가)만큼 수익이 나고, 300보다 낮으면 그만큼 손해가 발생합니다.

200          225          250          275           300          325           350          375          400
KOSPI200

다음은 정반대 모양의 선물 매도 포지션 수익률 그래프입니다. 지수가 행사가보다 낮은 경
에도 행사가에 매도를 하기 때문에 (행사가 - 지수)만큼 수익이 발생합니다. 여기에서는 지
가 300보다 낮으면 수익을, 300보다 높으면 손실을 입게 됩니다.

Bs a EY 느 0

+ 4

8S 선물의 개념 169



===== PAGE 170 =====
ee |
1 -

x

1 A 리0나

SS

.그비시태채회

100

75

-25

-50

-75

-100

225   250

300
0501200

350

400

따라서 기초자산(지수) 가격이 올라갈

수익을 창출하게 됩니다.

8.4 선물거래 사례

Ths KOSPI200 선물에 투자한 뒤 가격 변동에 따른 거래 사례입니다. KOSP1200 선물

A oe 매수, 하락할 것

@의며마또하는 진략으로

종목 정보대로 승수는 25만 원이고, 1계약을 거래한 것으로 가정하겠습니다.

75,000,000                              —}| 5,625,000} 5,625,000} 5,625,000
1               302 | 75,500,000              500,000} 3,775,000; 6,125,000} 5,125,000
306 | 76,500,000           1,000,000 | 3,825,000} 7,125,000} 4,125,000
3               310 | 77,500,000           1,000,000 | 3,875,000} 8,125,000
170 3부 선물



===== PAGE 171 =====
예측이 맞는 경우: 상승장에 매수 포지션을 취한 경우
Day 0: 지수 300 시점의 계약 금액 7,500만 원의 7.5%(위탁증거금율)인 5,626,000 212 계좌
에 납입하고 선물을 매수.

매수 잔고 = 5,626,000원(위탁증거금)
Day 1: 지수가 302에 마감. 50만 원의 이익 발생. 잔고 66,125,000원.
매수 잔고 = 5,626,000(잔고) + 500,000(차액) = 6,125,000원
Day 2: 지수가 306에 마감. 100만 원의 이익 발생. 잔고 7. 125,000원.

매수 잔고 = 6,125,000(잔고) + 1,000,000(차액) = 7,125,000원

+

Day 3: 지수가 310°] 마감. 1008+ 원의 이익 발생. 잔고 8,125,000원.

매수 잔고 = 7,125,000(잔고) + 1,000,000(차액) = 8,125,000원

+

20

15

10

수익
ㅇ=

-10

-15

-20

280             285             290             295              300              305              310             315             320
KOSPI200

8장 선물의 개념 171



===== PAGE 172 =====
예측과 다른 경우: 상승장에 매도 포지션을 취한 경우
Day 0: 지수 300 시점의 계약 금액 7,500만 원의 7.5%(위탁증거금율)인 5,626.000원을 계좌
에 납입하고 선물을 매도.

매도 잔고 = 5,626,000원(위탁증거금)

~

Day 1: 지수가 302에 마감. SORE 원의 손해 발생. 잔고 5.125,000원.
매도 잔고 = 5,626,000(잔고) - 500,000(차액) = 5,125,000원
Day 2: 지수가 306에 마감. 100만 원의 손해 발생. 잔고 4,125,000원.
매도 잔고 = 6,125,000(잔고) - 1,000,000(차액) = 4,125,000원

Day 3(마진콜 발생): 지수가 310에 마감. 100만 원의 손해 발생. 잔고는 3.125.000원. 잔고
가 계약 금액 7,750만 원의 5%(유지증거금)인 3,875,000원 미만이므로
2,687.500원 추가 납입 필요(계약 금액의 7.5%를 채울 수 있도록).

매도 잔고 = 7,125,000(잔고) - 1,000,000(차액) = 3,125,000원

20

15

10

-15

-20

280          285          290          295          300          305          310          315          320
KOSPI200

172 3부 선물



===== PAGE 173 =====
8.5 선물 이론가

파생상품 밸류에이션은 파생상품을 보유하고 있을 때와 보유하고 있지 않을 때의 손익을 따져
서 결정합니다. 선물도 마찬가지인데, 앞서 나온 선물 손익 그래프에서 봤듯이 만기 수익 구조
가 주식처럼 단순해서 밸류에이션 방법도 간단합니다. 선물 계약을 체결하고 만기가 되어 상
품을 인도받을 때까지 손익을 따지면 됩니다.

계산은 나중에: 이자 이익

선물을 매수하면 계약에 따라 기초자산을 확보하게 되지만, SS 후불로 계약 이행 시점에 지
급합니다. 금융 용어로 설명하면 포트폴리오상의 포지션에는 잡히지만 돈은 지불하지 않은 상
태가 됩니다. 그러므로 계약 시점부터 정산 계약 이행 시점까지의 이자 비용(금융 비용)을 아
낄 수 있습니다.

확보한 자산에 대한 권리는 아직 미보유: 배당은 못 받음
반면 확보한 자산은 아직 내 것이 아닌 상태라 배당에 관한 권리는 없습니다. 배당은 현재 시
점에 자산을 소유하고 있는 사람에게 가기 때문입니다.

선물 이론가 계산: 이익과 손해를 반영

선물 이론가 = 기초자산 가격 + 금융(이자) 비용 - 배당 수입

이 AWS 파생상품 관련 계산에 주로 쓰이는 연속복리이자율(00ㅁㅁㅁ4045 compounded

interest rate )-& 이용해서 표현하면 다음과 같습니다.

ine Ser ok

(F: 선물가격, S: 현물가격, r: 이자율, 0: 배당률, (: 잔존만기)

갑자기 지수함수가 나와 당황할 수 있으니 이자율 계산 관련 내용을 살짝 정리해보겠습니다.

8S 선물의 개념 173


===== PAGE 174 =====
여러 가지 이자율

증권회사 또는 선물회사에서는 투자자들에게 선물 이론가 계산 방법을 더 쉽게 알려주기 위해
연속복리이자을 대신 단순이자율을 사용하기도 합니다. 이 경우 공식은 다음과 같습니다.

=외나(6-00등|

(F: 선물가격, 6: 현물가격, r: 이자율, 0: 배당률, /: 잔존만기)

8.6 선물 관련 용어

미결제약정

선물시장 참여자의 상당수는 레버리지를 이용한 투기거래(6[ㅁ060414000)를 목적으로 단시간
에 매도와 매수를 완료해서 포지션을 0으로 만들고 당일 거래를 마감합니다. 반면, 주 소득원
은 다른 시장이지만 선물거래로 위험에 대비하고자 하는 헤지 거래자도 있는데, 이들이 선물
시장에서 보유하고 있는 계약은 다른 시장에서 보유한 계약의 위험 헤지를 위한 수단이기 때
문에 다른 시장 포지션이 남아 있는 동안 계속 보유하게 됩니다. 이렇게 장 마감 시까지 청산

=

174 3488


===== PAGE 175 =====
되지 않고 다음 날로 넘어가는 계약을 9) Aer (outstanding) °]e}a1 부릅니다.

베이시스

선물가격과 현물가격의 차이를 베이시스([52515)라고 합니다. KOSPI200 선물의 베이시스는
KOSPI1200 선물가격에서 KOSPI200 지수를 WH 값입니다.

베이시스 = 선물가격 - 현물가격

베이시스가 플러스(+)인 경우, 즉 선물가격이 현물가격보다 높으면 콘탱고(60ㅁㄷㅁㅁ80)라고
하고, 반대의 경우를 백워데이션(15200\7270423007)이라고 합니다. 일반적인 경우 선물가격이
현물가격보다 더 높은데, 그 이유는 앞서 선물 이론가 SANA BHO] 선물가격은 현물가격

에 이자 비용이 추가되기 때문이지요.

Aho} ABH (arbitrage) S 하려는 사람들은     ea tle     on  선물 베이시스를 항상 주시하
고 있다가 베이시스 수준이 정상 범위를 벗어나는 순간을 포착해 거래를 하기 때문입니다.

:

롤오비
펀드매니저나 실제로 현물이 필요한 사람은 기간이 긴 ABS 가져가야 하는 경우가 SU
ch 예를 들어 WTI 원유선물 WES 운용하는 펀드매니저는 편드수익률이 원유 가격을 따라

가도록 펀드를 운용해야 하죠. 이를 위해 실제로 원유를 사서 보유하는 방법이 가장 확실하지
만, 아무리 기관투자자라고 해도 원유를 보관하기 어렵고 보관 비용도 만만치 않습니다. 그래
서 현물 보유 대신 선물을 보유하는 것을 더 선호하지요. 선물은 보관 비용이 들지 않고, 증
금만으로 원유를 확보할 수 있어 거래 비용도 훨씬 적게 드는 장점이 있습니다.

하지만 선물을 이용한 포지션 유지의 최대 난제는 만기가 많이 남은 장기물은 유동성이 낮다
는 것입니다. 유동성이 낮다는 Be 거래가 잘 되지 않는다는 뜻입니다. 아래 표는 2018년 2
월 2일 기준 한국거래소에서 거래되는 KOSPI200 선물의 가격과 당일 거래량 ae
거래량 SS 보면 최근월물(만기가 가장 가까운 선물)인 3월물에만 거래가 집중되어 있음을 확인
할 수 있습니다. 심지어 2019년 만기 선물들은 가격이 형성조차 되지 않고  있습니다 장기물
은 정당한 가격이 형성되기 어렵다는 뜻입니다.

8장 선물의 개념 175


===== PAGE 176 =====
코스피200 F 201803                334.15               186,574
BATMI200 F 201806               335.10              453
BATI200 F 201809            335.40           6
ANMI200 F 201812               336.90              3

코스피200 201906             0.00                0
코스피200『 201912        0.00         0
코스피200 202012            0.00               0

장기로 포지션을 가져가야 하는 펀드매니저라면 이런 상황에 어떻게 HES 운용할까요? 보
통 최근월물 위주로 포지션을 운용하다가, 만기 시점에 포지션을 정리하고 차근월물로 보유
종목을 교체합니다. 예를 들면, 2018년 2월에는 2018년 3월물을 보유하고 있다가, 3월 선물
만기일(3월 둘째 주 목요일)이 오면 3월물을 매도하고 2018년 6월물을 매수하는 것입니다. 이
를 롤오버(701106ㅁ)라고 합니다.

그런데 대부분의 경우 롤오버를 할 때 최근월물 매도 가격보다 차근월물 매수가격이 높습
다. 위의 표에서 2018년 3월 만기 선물은 334.15에 마감하지만 2018년 6월 만기 ASS] 가격
은 335.10인 경우이지요. 대개 선물이 현물보다 가격이 높다고 앞서 언급한 것 기억하시죠?
선물상품은 이자 비용 때문에 차근월물 가격이 최근월물 가격보다 높은 것이 일반적입니다.
그렇다면 롤오버를 하면 3월물을 334.15에 팔고 6월물을 335.10에 사야 하므로 1계약당 0.95
포인트씩 SHS 보게 되겠네요. 이렇게 롤오버가 계속되면서 손해를 보는 것을 롤오버 리스
크라고 합니다.

176 3부 선물



===== PAGE 177 =====
Chapter 9
I    oii  R al] |  y & =
엑셀 실습

[z
no

9.1 K5 선물 이론가 산출

5장 엑셀 실습 시간에 만든 KS 지수를 기초로 만든 선물상품 KS ASS 만들어보겠습니다.
파생상품 가격은 기초자산 가격에 연동해 움직이므로 KS 선물 이론가를 계산할 수 있으
물가격이 이론가와 다른 경우에 차익거래를 할 수 있겠죠? 여기에서는 엑셀을 이용해 KS 선
물의 이론가를 계산해보겠습니다.

5.4절에서 만든 엑셀 파일인 05.4. KS 1006×.×15*×를 다시 사용하겠습니다. 파일을 열고 화
면 하단에 있는 @ YES 클릭해 새 시트를 만들고 이름을 '선물로 BUC, 이를 09.1. KS

『44『65.×15×라는 새로

fo
0)
:
이
Sas
도
af
ats,

C                 3. KS Futures.xisx - Excel                7030-65 ×
ee Monae FH 데이터 BS 보기                               :                                           “Yong Whoan Kim-MIS ^.
~ 10829 ㆍ[ett |= Me 20 고 22 [ee 으으
Be   |           a     "| (따가     wy [| PRAN- AND cg eg
02 , [247 a-|B-|Q2-A-|R- | FSB eHL|S- | yg   Mesew- |Bxa- | e- ga- nae
@uys ㄷ!     ai       。    28    ㅠ BABA ㅠ   스타일    Fob   편집      ^
jaa XX he                             |                      v
A      8   gCe ep Of Ae 아이오 ery    삽입0     [새는 - freed le: Re nae Ces ee ME
KR 삭저(이
2                                   이를 BPI
                                   이동/복사040
때                                  & 코드 보기)
& 시트 보호
6                                   - “aM     >
7 |                                           © 40
8                                   e771
9
sa)  ~ 그 ee   atl   x  책                                      Me
| BS 기본정보 ㅣ 일자별 주가 ㅣ 일자별 시가중역 | sheets ,



===== PAGE 178 =====
sparta

선물 이론가 산출을 위해 '일자별 시가총약 시트에 있는 일자와 지수를 사용하면 되지만 한 화
면에서 한눈에 보면서 진행하기 위해 일자와 지수 데이터를 옮겨오겠습니다. 우선 '선물' 시트
Ato] 일자, Bio 지수라고 제목을 만듭니다.
00 42, 43에 1, 2를 각각 입력하고 두 셀을 함께 선택한 후 오른쪽 하단의 점에 마우스를
갖다 대면 포인터 모양이 choy += VHYYCH, 그 상태에서 마우스를 클릭한 ay 드래
그해서 253행까지 끌어내리면 252일까지 날짜가 채워집니다.

4
z

@ 지수를 가져오기 위해 B2 셀을 선택하고, =를 입력하면 엑셀은 수식을 입력받기 위한
대기 상태로 변합니다.

| PI  _- ax fe

|

0

@ 그 상태에서 “일자별 시가총액" AES 선택하고 112 셀에 있는 1일 차 지수 데이터
택하고 키를 누릅니다.

1     "ELK 0 fe | RHE AES 0000
트        F     |     6

tu
c

ㅁ화학           엔터             압게           시수

28 88,000,000,000 500,000,000,000 1,245,000,000,000
100.19

87,576,720,000 513,542,000,000 _—_1,247,383,720,000
25 425 760 000 510954 S00 000 1.941 477 SEN NNO 11 22 |

@ '선물' 시트의 82 셀에 12) 차 지수가 입력됐습니다. 82를 다시 선택하고 박스 오른쪽
하단의 AS 더블클릭해서 252일까지 지수를 모두 채옵니다. 입력된 지수의 자릿수를
소수점 이하 두 자리로 맞춰줍니다.

© 이번에는 선물 이론가를 산출합니다. C1 셀에 '선물이론가(1분기)'를 입력합니다.

178 3부 선물



===== PAGE 179 =====
100.00
100.19
101.32
102.12

>
PWN

선물 이론가 계산을 수식으로 구현하기 위하여 우선 선물 이론가 공식을 다시 봅니다.

jpe Seo

(F: 선물가격, 6: 현물가격, r: 이자율, 0: 배당률, (: 잔존만기)

선물가격 는 구해야 할 값이고, 지금 가지고 있는 데이터는 현물가격(지수) 와 잔존만기(일
자) [가 있네요. 이자율 과 배당률 4가 필요한데, 이 값들은 현재 시장에서 통용되고 있는
치를 이용하겠습니다. 배당률은 누구에게나 동일하게 적용되므로 KOSPI2002] 평균 배당:
1.5%를 이용합니다. 이자율을 살펴보겠습니다. 2018년 2월 기준 국고채 금리는 2.25%, 회사
ay 금리는 2.79%입니다. 그런데 우리가 정부나 회사가 아니니 이 같은 저금리로 자금 조달을
하는 것은 불가능하죠. 은행 대출 금리를 살펴보면 가장 낮다고 알려진 인터넷 은행의 신용대
출 금리가 연 3.19%입니다.

지금까지 나열한 정보들을 종합해서 이자율은 3.19%로 하면 될 것 같습니다. 그런데 하나 더
고려할 사항이 있습니다. 돈을 빌려서 투자한다면 가장 낮은 대출 금리로 잡는 것이 맞겠지만,
이미 보유한 자금으로 투자한다면 어떻게 할까요? 이자율을 0%로 할까요? 아니죠. 우리는 지
금 금융공학을 공부하고 있잖아요. 금융에서는 돈을 놀리지 않는다고 전제합니다. 다시 말해,
가지고 있는 자산으로 투자하는 경우라도 선물에 투자하지 않으면 다른 상품에 투자할 것으로
여긴다는 뜻입니다. 고등학교 경제 시간에 배웠던 기회비용과 동일한 의미입니다. 그리고 이
때 비교되는 다른 상품은 무위험이자율(019-ㅡ[ㅇㅇ interest rate)-& 제공하는 국채입니다. 회
사채만 하더라도 회사가 망하면 채권 회수를 할 수 없기 때문에 위험비용을 수반합니다. 그래
서 금융에서는 일반적으로 자본비용을 얘기할 때 무위험이자율을 이용합니다.

여기에서도 국고채 금리인 2.25%를 이용하겠습니다. 이자율과 배당률을 F1~G2 셀에 입력합
니다.

i

+}

때

9장 선물 엑셀 실습 179


===== PAGE 180 =====
만기일은 하드코딩으로 수식에 직접 넣어도 무방하지만 편의를 위해 셀로 만들었습니다. 앞의
그림과 같이 배당률 아래쪽 『3~04 셀에 입력합니다.

이제 선물 이론가를 계산합니다. 먼저 1분기 만기인 선물 이론가 수식 WAS 위해 2 셀
을 선택합니다. 수식창에 위 SAS 엑셀 수식으로 나타낸 =82*6>×『(($06$1-$6$2)*
( ($6$3-A2)/252) )S 입력합니다. 수식에서 ($6$3-A2)/252) 부분은 잔존만기인 [인데,
1분기 만기일(63일)에서 현재일을 WM 값을 1년인 252일로 나뉘줍니다.

| pr      2 | < OW fe | -22-E@((ss1-s6s2)*(($6$3-A2)/252))

4A   B              D CE    F  ;  G

1                           TEM 2.259)
1| 100.00 [$G$3-A2)/252))      BEES 150%)

3 | 2. 10019            반기(1분기]   63

4 | 3 10132       :     만기(2분    126,

C2e 선택한 후 박스 오른쪽 하단 AS 더블클릭해서 데이터를 ASU. 252일까지 선물 이
론가가 채워진 모습을 확인할 수 있습니다.

여기서 관심을 가질 만한 포인트가 있습니다. 이 선물은 63일이 만기일이므로 64일 이후의 데
이터는 필요가 없습니다. 삭제하는 것이 맞지만, 공부를 위해 잠깐 살펴본 후 삭제하겠습니
다. 만기일 전(1~62일)까지는 선물가격이 지수보다 높습니다. 만기일(63일)로 다가갈수록 선
물가격은 지수에 가까워지고, 만기일에는 선물가격과 지수가 같아지게 됩니다. 만기일 이후
(64일~)에는 선물가격이 오히려 낮아집니다.

180 3부 선물



===== PAGE 181 =====
지수 | 선물이론가(분기)

59 | 58 113.71     113.72
60} 59 114.04     114.05
61| 60 115.03      115.04
62| 61 113.42     113.42
:       <

65

66| 65 111.53 >   111.53
67| 66 111.51      111.50
68} 67 113.31     113.30
69| 68 112.95     112.93

금융 이론을 공부할 때 소개했듯 ASS 만기일에 SS 지불하고 상품을 받는 구조입니다. 따
라서 선물 롱 포지션 보유자는 만기 전에는 이자율만큼 이득을 보기 때문에 선물가격이 지수
보다 높게 나오는 것입니다. 만기일 전후의 가격 변화를 확인했으면 64일 이후의 데이터는 삭
제합니다.

같은 방법으로 2분기 선물 이론가를 산출합니다. 2분기 선물 이론가 FAS =B2*EXP
( ($6$1-$6$2 )* ( ($6$4-A2 )/252) )입니다. 2분기는 126일까지의 데이터만 남기고 127일
부터 Alec,

prowl EK OM fe [ =82"exr((s651-s652)*((sa34-a2)/252))| |

배당를
만기(1분기) |
=
만기(2분기)

잔존만기가 길수록 이자에서 오는 이익이 높으므로 선물 이론가는 당연히 2분기가 더 높게 계
산됩니다.

9장 선물 엑셀 실습 181


===== PAGE 182 =====
LS
>
fa)
ㅁ

디다

2        1 100.00                   100.18                    100.37
3        2 100.19                   100.37                    100.56
4        3 101.32                   101.50                    101.69
5        4 102.12                   102.30                    102.49
6        5 103.17                   103.35                    103.55

일반적인 경우는 아니지만 이자율이 마이너스(-)가 되거나 배당률보다 낮아지는 경우에는 선
물가격이 현물가격보다 낮아질 수도 있겠네요. 실험 삼아 이자율을 -2.25%로 바꿔봅니다.

일자 ㅣ 지수 ㅣ 선물이론가(1분기) | 선물이론가(2분기) 를 oats

배당률

만기(1분기)

만기(2분기)

선물가격이 지수보다 낮아지는 것을 볼 수 있습니다.

실습을 마친 결과 예시 파일은 09.1. 5 Futures (실습결과-데이터고정 ) .×15×입니다.

9.2 KOSPI200 선물 포지션 손익
이번에는 엑셀을 이용해 KOSP1200 선물 투자 시 매수와 매도 각각의 포지션에 대해 손익
계산해보도록 하겠습니다. 손익 계산과 더불어 마진콜 상황에 대해서도 파악해봅니다.

tuo

분석 대상 선물상품은 2017년 124 만기인 KOSPI200 선물(2017년 12월물)입니다. 네이버,
구글 등 포털 사이트는 주식, 지수, ETF 등 대표 금융상품의 시세는 제공하지만 선물, 옵션과
같은 전문 상품의 시세는 제공하지 않고, 제공한다 해도 모든 월물의 시세가 아닌 최근월물(만
기가 가장 가까운 선물) 시세만 제공하기 때문에 데이터 2S2i (crawling)-S 통해 얻기가 어렵
습니다. 아쉽지만 선물 일자별 시세는 본 책의 웹사이트에서 09.2 (05061200 F 201712.x1sx
파일을 다운로드하거나 한국거래소 웹사이트(11『[ㅁ://\41.「×.00.「『)에서 다운로드하기

바랍니다.

182 3부 선물



===== PAGE 183 =====
본격적인 손익 AALS 시작하기 전에 선물 손익 AALS 위한 정보를 세팅합니다. KOSPI200
선물 SHE 25만 원, 개시증거금율은 7.5%, 유지증거금율은 5%입니다. 손익을 명확히 확인
하기 위해 1계약만 거래한다고 가정합니다. 이 내용을 <1~Ｌ4 셀에 기록합니다.

선물가격 지수

4 | 2017/09/04 | 305.6 | 304.19
5 | 2017/09/05 | 304.85 | 304.06

첫 거래를 9월 1일 종가로 거래하고, 개시증거금만 납입한다고 가정합니다. 따라서 첫 날에는
매수 매도 모두 손익이 0입니다. 잔고는 매수 매도 모두 개시증거금(선물가격×계약 수×승수
×증거금율)입니다. 엑셀 수식으로 나타내면 =83*11*Ｌ2*.3입니다.

^          j        B        ‘gets         D                                          F                   G
1                                                                                          매                                               매
2017/09/01 | 308.4 | 307.78            0| 5,782,500            0| 5,782,500
4 | 2017/09/04 | 305.6 | 304.19

슷자가 길어 천 단위 쉼표가 보여야 읽기 쉽습니다. 쉼표가 보이지 않는다면 셀 표시 형식이
숫자 형식으로 지정되지 않아서입니다. 그럴 때는 셀을 선택한 후 오른클릭을 해서 나타나는
팝업 메뉴 중 셀서식 메뉴를 선택한 후, '범주에서 AAS 누르면 오른쪽에 나타나는 화면에
서 다음 그림과 같이 '1000단위 구분 기호(.) AES 선택해줍니다.

9장 선물 엑셀 실습 183



===== PAGE 184 =====
v

일반적인 숫자를 나타내는 데 사용됩니다. 통화 및 회계 표시 형식에는 화폐 가지에

a 서식
   28 글끌 테두리 재우기 ws
BRO:
일반              ~| 보기
동화                   5,782,500
회                      Pepe.           =
=     seneeo: 10 [위
시간                          단        7
aoe              [1000 단위 구분 7150) ASOD |
분수                  음수04):
지수                   (1,234)
——                 (1,234)
기타                    1.234
사용자 지정
-1.234
숫자 서식은
대한 특수 서식이 있습니다.

Lea

az |

둘째 날입니다. 선물가격은 첫째 S 308.44] 305.62 = 하락했습니다. SS 잡은 투자자는
손해를 BAUR, 손해 금액은 (308.4 - 305.6)×계약 수×승수입니다. 반대로 +S 잡은 투

자자는 롱 포지션에서 손해 본

니다.

만큼 수익이 납니다. 수식은 롱과 반대인 (305.6 - 308.4)×계
약 수×승수입니다. 엑셀로 표현하면 다음 그림과 같습니다. 계약 수를 나타내는 Ｌ1 셀과 '승
42S 나타내는 12 셀은 셋째 날 이후로 확장시키는 경우에도 고정시켜야 하므로 $를 붙여줍

ㅋ 2017/09/01 |

Pr   | : | % S_ fe | -(5s-83y*us1%1s2_ |

0 5,782,500    0 5,782,500
2017/09/04 | 305.6 | 304.19 |'LS1*LS2_ |    700,000

5 | 2017/09/05 | 304.85 | 304.06

184 3448



===== PAGE 185 =====
| Px     “11K OY fe | -063-0949015152 ]

일자 | 선뮬가격!| 지주

3 | 2017/09/01| 308.4 | 307.78    0 5,782,500    0 5,782,500

2017/09/04| 305.6 ｜304.19 | -700,000 _  |

잔고는 어떻게 변했을까요? 잔고 계산은 더 단순합니다. 첫째 날 잔고에 둘째 날 손익을 더해
주면 됩니다.

fe ㅋㄷ

일자. [선뮬가격|| 지수
3 | 2017/09/01           308.4 | 307.78                            01 5,782,500                           0 5,782,500
2017/09/04 | 305.6 | 304.19 | -700,000 |=E3+D4               700,000 6,482,500

EVE 434      Ansar      2A4 ae

여기까지 끝냈으면 D4~G4 셀을 선택한 후 오른쪽 하단의 점을 더블클릭해서 데이터를 끝까
지 채옵니다.

3 | 2017/09/01 | 3084 | 307.78
2017/09/04 | 305.6 | 304.19

§ | 2017/09/05 | 304.85 | 304.06
2017/09/08      304 2      3203218

9.3 마진콜 발생 여부

이제 마진콜을 당하게 되는 경우를 체크해보겠습니다. 마진콜은 잔고가 유지증거금 미만으로
내려가는 경우 발생합니다. 유지증거금을 계산하기 위하여 자리를 확보합니다. 유지증거금율
이 5%이므로 유지증거금은 선물가격×계약 수×승수×유지증거금율(5%)로 계산합니다.

H3 셀에 엑셀 수식으로 =83*[$1*|.$2*[$4라고 입력합니다. 그다음 연속 데이터 채우기로 마

9장 선물 엑셀 실습 185


===== PAGE 186 =====
지막 행까지 데이터를 채워줍니다.

4             A            :          8                 ㅇ                  ㅁ                       E            i          F                      6

ub

2                                                                                                                        승수
2017/09/01 | 3084 | 307.78          0} 5,782,500          0} 5,782,500 } *L$2*L$4          개시증거금

4 | 2017/09/04 | 305.6 | 301.19 | -700,000| 5,082.500 | 700,000} 6,482,500

이제 잔고가 유지증거금 이하로 떨어지면 잔고 do] 붉은 HAV} 되도록 세팅합니다. 이는 조
건부 서식을 이용합니다. 3 셀을 선택한 후 상단 메뉴에서 조건부서식 버튼을 클릭하고 계속
되는 팝업 메뉴에서 셀 강조 규칙 , 보다 작음 을 차례로 클릭합니다.

Oa led oly           3.2 KOSPI200 MH OY 실슴가 (2H 오드] - Brcel            706 -=- c x
은 ee 페이지력이아웃 F4 데이터 Ye By                 0000 Yong Whoan Kim-nv6 7
 개개 wean _—___[n =) 4)"                  0,
가 St ee a | 편집      a
Co Eaeae Eo                      이                       ~
MA        B      c      D           Kea G8 강의 사이에 잇음00 데이터 악대) > |            저
1                       0
2                                            fe 같음@0-               Fs 색조(59        '
2017/09/01 | 3084 | 307.78    0 | 5,782.50
4 | 2017/09/04 | 3056 | 30419 | -700,000 5082.50 (fa) "a= SRm-         FEjo1rueo >
5 | 2017/09/05 | 30485 | 304.06 | -187,500 4,895,00
6 2017/09/06 | 3043 | 30318 | -137,500 4757.50 [may 발성 WRW-       aie Som
7 | 2017/09/07 | 3081 | 30697| 950,000 5,707,50                BARA +
8 | 2017/09/08 | 30835 |30743| 62500 5,770,00 |를| 9 2M-        © ea4@
9 (2017/09/11 | 3115 [30983] 787,500 655750  , sayy       1750
10. 2017709/12 | 31145 1310.42 | -12.500. 6545.00       sees          OPAL 5 no     -
it   | 와서   ®                       (hE Se      - “^ 0
0 -   +   + 100

조건부 HAS 설정하는 창이 나타납니다. 왼쪽 칸에 비교 대상 셀을 지정할 수 있습니다. 유
지증거금과 ADS 비교해야 하므로 =13라고 입력합니다. 일자마다 그날그날의 잔고와 유지
증거금을 비교해야 하므로 $를 붙이지 않아야 함에 주의하세요.

보다 작음                                                                                                    ~
다음 값보다 작은 셀의 서식 지정:
66                                      Jes] 적용할 서식: HEE 벅스트가 있는 연한 짤강재우기 |

186 3부 선물

으으


===== PAGE 187 =====
ae tis 1008

확인을 눌러 조

까지 셀에 입력한 내용을 다른 셀로 확대 set 때는 셀 선택 후 오른쪽
릭을 했었습니다. 그런데 서식을 복사할 때는 오
른쪽 하단 점에서 오른클

오른클릭한다는

건부 서식을 적용해도 화면에는 아무
지중거큼보다 많기 때문이죠. 이제 적용한 조건부 서식을 전체 날짜로 확대 적용합니다. 지금

경우와 달리 이번에는

릭을 한 %

변화가 없습니다. 첫째 날은

잔고가 유

하단 점에서 더블클

클릭을 해야 합니다. 53 AS 선택한 후 오

FeHoH | Se 마지막 행까지 끌어내립니다. 보통의

것에 주의하세요. 마우스를 놓으면 팝업 메뉴가 나타나

는데 이때 서식만 채우기 를 클릭하면 조건부 서식이 열 전체에 적용됩니다.

3 =     vl 4 | Si of  fe | =B3*L 1°L2"L3            3        z   gi   고    Ps
4    Ac     B            D               F       G       H    lJ
58| 2017/11/27 | 329.25 | 329.53 |-1,587,500 | 10,995,000 “ERO  50000, 4,115,625
69 | 2017/11/28 | 331.05 | 330.99 | 450,000] 11,445,000   ~   니그 때    4,138,125
60| 2017/11/29 | 331.05 | 330.68      0] 11,445,000    2     :      4,138,125
61| 2017/11/30 | 325.6 | 325.25 |-1,362,500 | 10,082, 500 [a 서식만재우기 —    - ] 4.070.000
62| 2017/12/01 | 325.2 | 324.78 | -100,000 | 9,982,500   서식 없이 재우기(0)   4,065,000
63/ 2017/12/04 | 328.35 | 328.77] 787,500] 10,770,000     단위 BLD     4,104,375
64| 2017/12/05 | 329.95 | 329.61 | 400,000] 11,170,000            22       4,124,375
65| 2017/12/06] 325 | 324.52 |-1,237,500] 9,932,500     c     5     4,062,500
66| 2017/12/07 | 324.05 | 323.59 | -237,500 | 9,695,000     다우         4,050,625
67| 2017/12/08 | 324.75 | 324.68| 175,000] 9,870,000    igh        4,059,375
68| 2017/12/11 | 324.85 | 325.09   25,000} 9,895,000   「            4,060,625
69) 2017/12/12] 323.8 | 324.07 | -262,500] 9,632,500       4,047,500
7 | 2017/12/13 | 3262 | 326.18] 600,000| 10,232,500 *= **71©        4,077,500
71 | 2017/12/14 | 327.65 | 324.74] 362,500} 10,595,000              4,095,625
72

73

. > | shen | @                                   대들     a

GSE 동일하게 조건부 서식을 적용합니다.

9장 선물 엑셀 실습 187



===== PAGE 188 =====
4             A                       8                  c                   ㅁ                        E            j           F                                                    H

1                                                                                                                                        ㅣ                                                                         ㅣ

2                                                                                                                                                                                  =
3 | 2017/09/01 | 3084 | 307.78                       0| 5,782,500                       0} 5,782,500 | 3,855,000
4 | 2017/09/04 | 305.6 | 304.19} -700,000 | 5,082,500} 700,000} 6,482,500} 3,820,000
§ | 2017/09/05 | 304.85 | 304.06 | -187,500} 4,895,000} 187,500} 6,670,000} 3,810,625
6 | 2017/09/06 | 3043 | 303.18 | -137,500 | 4,757,500] 137,500} 6,807,500 | 3,803,750
7 | 2017/09/07 | 308.1         306.97 | 950,000} 5,707,500 | -950,000 | 5,857,500 | 3,851,250
8 | 2017/09/08 | 308.35 | 307.43         62,500 | 5,770,000       -62,500 | 5,795,000 | 3,854,375

2017/09/11 | 311.5 | 309.83 | 787,500 | 6,557,500 | -787,500 } 5,007,500 | 3,893,750
10 | 2017/09/12 | 311.45 | 310.42    -12,500 | 6,545,000     12,500 | 5,020,000 | 3,893,125
11. 2017/09/13 | 310.85     310    -150,000 | 6,395,000 | 150,000 | 5,170,000 | 3,885,625
12| 2017/09/14 | 313.6 | 312.52 | 687,500| 7,082,500 | -687,500 | 4,482,500 | 3,920,000
13, 2017/09/15 ㅣ 314.55 | 313.69 | 237,500| 7,320,000 | -237,500 | 4,245,000 | 3,931,875

14. 2017/09/18 | 320.05 | 318.93 | 1,375,000 | 8,695,000 |-1,375,000                                         4,000,625
15| 2017/09/19 | 3194 | 31851 | -162,500| 8,532,500] 162,500               3,992,500
16 | 2017/09/20 | 319.15 | 31848            -62,500 | 8,470,000             62,500                                         3,989,375
17 | 2017/09/21 | 3194 | 31825              62,500 | 8,532,500 | -62,500                                         3,992,500
18 | 2017/09/22 | 317.1 | 316.71 | -575,000| 7,957,500} 575,000                                         3,963,750
19) 2017/09/25 | 317.15 | 3164      12,500 | 7,970,000} -12,500               3,964,375

20 | 2017/09/26 | 315.15 | 314.29 | -500,000| 7,470,000} 500,000} 4,095,000 | 3,939,375

9월 18일부터 25일까지의 셀이 붉은색으로 변했습니다. 데이터를 보면 해당 일자에는 잔고가
유지증거금 미만임을 확인할 수 있습니다. 이 기간 동안에는 매도 포지션만 마진콜이 발생했
네요. 지수가 꾸준히 오르면서 매수에는 이익이 누적됐지만 매도는 손실이 계속되면서 마진콜
이 발생한 사례입니다

마진콜이 발생하면 개시증거금만큼 잔고를 ASO AMS 지속할 수 있습니다. 그렇지 못하
면 거래소가 임의로 반대매매를 시행하기 때문입니다. 마진콜이 발생한 날 개시증거금을 채우
기 위해 셀 하나를 추가해 개시증거금을 계산합니다. 11 셀에 개시증거금 칼럼을 만들고 개시
증거금을 계산합니다. 13 셀에 수식 =B3*L$1*L$2*L$3-S 입력합니다.

 x vo  Se | =63*$1*1$2*1Ｌ$켜 a     nee    aa zone
G         H               i       도
!                                 | 250.000
782,500 | 3,855,000 |1*L$2*L$3          =A 9      4
482,500 | 3,820,000                 증거금을     5.0%|

188 348


===== PAGE 189 =====
연속 데이터 채우기를 이용해 마지막 날까지 데이터를 채우고, 마진콜이 발생한 날인 9월 18
일로 이동합니다. 9월 18일에 마진콜이 발생해서 잔고를 개시증거금만큼 채워 넣는다면 of
19일에는 개시증거금에서부터 거래를 시작하게 됩니다. 이 USS 엑셀 수식에 반영해줍니
다. 9월 19일 잔고인 615 AS 선택하고 수식을 바꿔줍니다. 이번 수식은 약간 복잡합니다.
전일 잔고가 유지증거금 이상이면 '전일 잔고+손익'으로 잔고를 계산하고, 전일 잔고가 유지
증거금 미만이면 '개시증거금+손익'으로 계산하도록 해야 합니다. 조건부로 계산이 달라지기
때문에 를 이용합니다. 615 셀에 수식 =IF (G14>=H14, 614, 114) + FISS 입력합니다.
이 수식은 614가 H14 이상이면 전일 잔고인 614를, 그렇지 않으면 개시증거금인 114를 A
택한 뒤 손익을 더한다는 의미입니다.

feo  더 - Y fe | =패(614>마14, G14, 114)+F15
A   =   ㅣ   F            H   |   I

1                        !              =

12| 7,082,500 | -687,500| 4,482,500 | 3,920,000 | _ 5,880,000
iB  7,320,000 | -237,500| 4,245,000 3,931,875 | 5,897,813
8,695,000 |-1,375,000 | _ 2,870,000 | 4,000,625] _ 6,000,938
a 8,532,500 | 162,500] 114)+F15 | 3,992,500| 5,988,750

연속 데이터 채우기로 마지막 날까지 수식을 채워줍니다.

9장 선물 엑셀 실습 189


===== PAGE 190 =====
4
1
2
12 2017/09/14 | 313.6 | 31252 | 687,500} 7,082,500 | -687,500 | 4,482,500 | 3,920,000   5,880,000
43) 2017/09/15 |} 314.55 | 313.69 | 237,500] 7,320,000} -237,500| 4,245,000 | 3,931,875   5,897,813
기                                              :
15

2017/09/18 | 320.05 _| 318.93 | 1,375,000 | 8,695,000 |-1,375,000      4,000,625 | _ 6,000,938
2017/09/19 | 3194 | 31851 | -162,500] 8532,500| 162,500| 6,163,438 | 3,992,500] 5,988,750
46 | 2017/09/20 | 319.15 | 31848] -62,500| 8,470,000| _62,500| 6,225,938 | 3,989,375 | 5,984,063
17| 2017/09/21| 3194 [31825] 62,500| 8532,500| -62,500| 6,163,438| 3,992,500] 5,988,750
18| 2017/09/22 | 317.1_| 316.71 | -575,000| 7,957,500| 575,000| 6,738,438 | 3,963,750| 5,945,625
19 | 2017/09/25 | 317.15 | 3164 | 12,500| 7,970,.000| -12,500| 6725,938| 3,964,375 | 5,946,563
20| 2017/09/26 |_315.15 | 31429| -500,000| 7,470,000| 500,000] 7,225,938 | 3,939,375 | 5,909,063
21| 2017/09/27 | 314.75 | 31382| -100,000| 7,370,000| 100,000| 7,325,938 | 3,934,375 | 5,901,563
22 2017/09/28 | 31495 |31385| 50,000] 7,420,.000| -50,000| 7,275,938 | 3.936875 | 5,905,313
23 2017/09/29 | 317.65 | 31627 | 675,000| 8,095,000 | -675,000| 6,600,938 | 3,970,625 | 5,955,938 |
24| 2017/10/10 | 3235 _| 322.49 | 1,462,500| 9,557,500 |-1,462,500 | 5,138,438 | 4,043,750 | 6,065,625
25| 2017/10/11 | 3266 | 326.12 | 775,000| 10,332,500| -775,000| 4,363,438 | 4,082,500 | 6,123,750
26| 2017/10/12 | 329 | 328.11 | 600,000 | 10,932,500 | -600,000 | ay7e3438| 4,112,500] 6,168,750
27 | 2017/10/13 | 328.65 | 327.35] -87,500| 10,845,000| _87,500| 6,256,250| 4,108,125| 6,162,188
28 | 2017/10/16 | 32885 | 327.82] 50,000] 10,895,000| -50,000| 6,206,250] 4,110,625] 6,165,938
23/ 2017/10/17 | 329.15 | 32851| 75,000] 10970,000| -75,000] 6,131,250] 4,114375| 6,171,563
30/ 2017/10/18 | 3292 | 3284 | 12500 | 10,982,500] -12,500| 6118750] 4,115,000] 6,172,500
31
32
33
3
35
36
37
38
39

2

2017/10/19 | 327.45 | 326.47 | -437,500 | 10,545,000} 437,500| 6,556,250] 4,093,125] 6,139,688
2017/10/20 | 329.6 | 32889} 537,500} 11,082,500 | -537,500| 6,018,750} 4,120,000| 6,180,000
2017/10/23 | 3304 | 329.45} 200,000 | 11,282,500} -200,000| 5,818,750} 4,130,000    6,195,000
2017/10/24 | 329.9 | 328.96 | -125,000| 11,157,500 | 125,000} 5,943,750| 4,123,750    6,185,625
2017/10/25 | 330.1 | 329.31              50,000 | 11,207,500 | -50,000 | 5,893,750 | 4,126,250 | _ 6,189,375 |
2017/10/26 | 327.1 | 326.99 | -750,000| 10,457,500 | 750,000} 6,643,750| 4,088,750| 6,133,125
2017/10/27 | 330.2 | 329.23 | 775,000} 11,232,500 | -775,000} 5,868,750| 4,127,500    6,191,250
2017/10/30 | 330.8 | 330.38 | 150,000} 11,382,500 | -150,000 | 5,718,750} 4,135,000} 6,202,500
2017/10/31 | 3344 | 333.57 | 900,000 | 12,282,500 | -900,000} 4,818,750} 4,180,000] 6,270,000
| 40| 2017/1 1/01 | 339.9 | 338.76 | 1,375,000 | 13,657,500 |-1,375,000 | 3,443,750 | 4,248,750| 6,373,125
41. 2017/11/02 | 338.4 | 337.53 | -375,000} 13,282,500| 375,000| 6,748,125 | 4,230,000] 6,345,000
42) 2017/11/03 | 339.7 | 338.83 | 325,000} 13,607,500| -325,000| 6,423,125| 4,246,250    6,369,375
43) 2017/11/06 | 337.5    3374 | -550,000 | 13,057,500} 550,000} 6,973,125| 4,218,750} 6,328,125

전체 기간 중 9월 182, 10% 12%, 119 1일 총 3번 마진콜이 발생해 증거금을 채위놓은 것
을 확인할 수 있습니다.

지금까지 2017년 12월 만기인 KOSP1200 선물의 2017년 9월부터 만기일까지 포지션별 손익
을 계산하고 마진콜이 발생하는지를 체크해봤습니다.

190 3부 선물



===== PAGE 191 =====
ie 기          Chapter 10
코딩 기술: 반복되는 데이터

10.1 반복되는 데이터는 넘파이 배열로
프로그래밍을 할 때 유사한 형태의 데이터 여러 NS 동일한 방식으로 처리해야 할 때가 RS
니다. 반복적인 일을 하는 경우가 대표적이지요. 이럴 때 유용한 데이터 구조가 MS (array)

일자별 주가를 처리하는 경우를 생각해봅시다. 1월 1일부터 1월 31일까지의 종가를 메모리
에 저장해두고 프로그래밍을 하는 경우, HSS 사용하지 않는다면 각 날짜별로 데이터를 처
리해야 해 여간 불편하지 않을 수 없습니다. 1월의 영업일이 20일이라면 각 날짜마다 하나
씩의 총 20개의 변수를 선언하고, 변수마다 일일이 주가를 입력해야 하며(예: 00101=1000,
00102=1010, …, 00131=1100), 필요할 때마다 또 각각의 날짜에 있는 값을 일일이 불러오
는 일을 20번씩 반복해야 하기 때문이지요. 하지만 배열을 사용한다면 1월 1일부터 31일까지
의 주가를 1개의 배열변수에 넣어서 처리(예: d=[1000, 1010, …, 11001])하기 때문에 20번
이 아니라 한 번에 처리할 수 있게 됩니다.

파이썬이 제공하는 기본 array 함수로도 배열을 처리할 수 있지만 대부분 ape] (NumPy)7t
제공하는 다차원 배열을 이용합니다. 넘파이가 제공하는 다차원 배열은 성능 측면에서 우수할
뿐 아니라 기능 또한 배열에 그치지 않고, 선형대수, 난수 발생기, 푸리에 변환 등 여러 가지
추가적인 기능을 제공하기 때문입니다. 여기에서는 넘파이를 이용해 다차원 배열을 다루는 기
술과 선형대수의 핵심인 벡터 연산법을 알아보겠습니다.

10장 코딩 기술: 반복되는 데이터 191



===== PAGE 192 =====
배열 만들기
넘파이 라이브러리를 사용하기 위해서는 SA numpyS 호출해야 합니다. 넘파이는 워낙 대중
적으로 쓰이는 라이브러리라 대부분의 개발자들이 매라고 줄여서 호출합니다.

1 import numpy as np

Out

넘파이가 제공하는 VSS ndarraye}a 부르며, 하나의 배열에는 같은 종류의 데이터만을 담
을 수 있습니다. WSS 만들 HE np.array()S 사용하는데 괄호 안에 실제 배열 데이터가
들어갑니다. HSS 1차원부터 ㅁ차원까지 제한 없이 만들 수 있는데, 차원별로 []를 이용해
구분합니다. 차원의 개념은 엑셀을 떠올려보면 쉽습니다. 1차원 WSS 엑셀에서 한 줄(행 =
는 열)만 이용하는 경우이고, 2차원 배열은 스프레드시트를 모두 이용(행과 AS 동시에 이용)하
는 것입니다. 하나의 엑셀 파일 내에서 시트를 여러 개 만들 수 있죠? 3차원은 이렇게 여러 개
의 시트를 사용하는 엑셀이라고 이해하면 됩니다.

1차원, 2차원, 3차원 배열을 각각 만들어보겠습니다. 1차원 배열이라도 ( ) 속에 [JS 붙여서
배열을 선언하지 않으면 에러가 발생하니 주의하세요.

1 #1차원 array 만들기
2 al = np.array((1,2,3])
3  print(a1)

Out [1 2 3]

1 ＊ 2차원 array: 이중 [[ J]
3 print(a2)

Out [[1 2 3]
[4 5 6]]

1 # 3차원 070: 3중 [[C JJ]
2 a3 = np.array([((1,2,3], [4,5,.6]], [[1,2,3], [4,5,6]]])
3 print(a3)

192 3부 선물


===== PAGE 193 =====
out [023]
[4 5 6]]

[[1 2 3]
[4 5 6]]]

배열 모양 변경하기

넘파이를 이용하면 배열의 모양도 쉽게 바꿀 수 있습니다. (15×1) MSS (1×15), (3 ×5)
등 원소의 개수만 맞춰주면 원하는대로 자유롭게 바꿀 수 있습니다.

(1×15) HSS (3x5) WSS 모양을 바꿔보겠습니다.

먼저 (1×15) 배열을 만들기 위해 넘파이 함수인 03096 ( ) 함수를 사용합니다. 00.0「ㅁ8096
(시작 번호, 끝 번호, 간격)라고 명령하면 203096() 함수는 시작 번호부터 시작해 간격만큼
건너뛰며 끝 번호 직전까지 일정한 간격으로 숫자를 돌려줍니다. 00.0「ㅁ80096 (2, 8, 2)라고
하면 2, 4, OS 돌려주는 것이지요. 시작 번호와 간격을 생략하면 0부터 시작해서 1씩 올라가
며 숫자를 돌려줍니다.

1 ㅇㅋ= np.arange(15)    # 0부터 15 직전까지 1씩 건너뛰어 숫자를 배열한다
2 print(c)
006801005052 3 4 5 6 7 8 9 10 11 12 13 14]

배열 모양을 변경할 때는 배열명.「651306(행, 열) 함수를 사용합니다.

1 c=c.reshape(3, 5)
2 print(c)

Out [[@ 1 2 3 4]
[5 67 8 9]
[10 11 12 13 14]]

1차원 배열이 (3x5) 모양의 2차원 배열로 바뀌었습니다.

이번에는 1차원 배열을 만들고 3차원 배열로 바꾸어보겠습니다.

10장 코딩 기술: 반복되는 데이터 193


===== PAGE 194 =====
1 d=np.arange(®, 100, 5)
2  02090

Out [0 5 10 15 20 25 30 35 40 45 50 55 60 65 70 75 80 85 90 95]

1 d=d-.reshape(2, 2, 5)
2900

Out array (TLL. 5, 10, 15, 201,
[25, 30, 35, 40, 45]],

[[50, 55, 60, 65, 70],
175: 80, 85, 90, 95]]])

배열의 스칼라 연산

배열은 배열 모양 그대로 단순 사칙연산인 스칼라 연산을 수행할 수도 있고, 벡터 연산을 수행
할 수도 있습니다. 고등학교 수학 시간에 벡터와 스칼라를 배웠던 적이 있을 겁니다. 스칼라는
그냥 일반적인 숫자로, 초등학교에서 배운 사칙연산을 합니다. 다만 같은 위치에 있는 숫자끼
리 연산을 한다는 차이가 있습니다. 그럼 스칼라 연산부터 배워봅시다.

1 # nd operation

2 nl=np.array([[1, @], # (2x2) 배열 만들기
3            [0, 1}])

4 n2=np.array({[1, 2],

5

[3, 4]])

1 01172 # 덧셈: 같은 위치의 BA7|e! 더한다

Out Braye 2],
[3, 5]])

1 01-72 # Ba: 같은 위치의 원소끼리 SICH
Out array([[ 0, -2],
[-3, -3]])

194 3부 선물


===== PAGE 195 =====
1 01502 # SY: 같은 위치의 원소끼2/ 곰한다 (행렬 연산이 아닌, 스칼라 연산임)

Out array([[1, 0],
[0, 4]])

1 01/02 # Lee: 같은 위치의 원소끼리 나눈다
Out array({[[ 1. , @. J],
[Ose 0225111)

1 02/01 # OCB 나누면 경고 에시지와 항께 무한대가 나온다

Out 20020([[ 1., inf],
01016. ~4°)))

배열에 대해 처음 소개할 때, 배열의 장점을 얘기하면서 배열 내의 데이터 전체를 한꺼번에 처
리할 수 있다고 했었죠. 스칼라 연산의 다른 형태로 배열 전체에 같은 연산을 일괄적으로 적용
할 수 있습니다. 즉, <배열> + 1을 하면 배열 내 각각의 원소에 1씩 더해진다는 뜻입니다. 예제
를 보겠습니다.

1 nisl # 배열 원소 각각에 1씩 더한다

Out array({(2, 1],
(1, 2]])

1 ㅁ1-1 # 배열 원소 각각에서 14) SICH

Out array({{ 0, -1],
[-1, @]])

1 onl*2 # 배열 원소 각각에 24 공한다

Out array({(2, 0],
[0, 2]])

1 01 / 2 # 배열 원소 각각을 2로 나눈다

Out array([[ 0.5, 0. ],
[0: , @.5]])

앞서 파이썬 실습에서 KOSPI2002} S&P500 데이터들을 지수화하기 위해 일자별 지수를 기

10장 코딩 기술: 반복되는 데이터 195


===== PAGE 196 =====
준 지수로 나누고 100씩 곱하는 프로그램을 작성했습니다. 그때 사용한 방법이 지금 우리가
다루는 배열의 스칼라 연산입니다.

배열의 벡터 연산
이번에는 벡터 연산을 해보겠습니다. 벡터를 오랜만에 접하는 분을 위해 벡터의 곱셈 방법을
잠깐 복습하겠습니다.

벡터의 곱셈
(28h (°                       032 g| af + 8)
ce + (ean    cf +dh

앞의 행렬에서 BS, 뒤의 행렬에서 SS 가져와 순서대로 곱한 후 더해주는 것입니다. 기억이
되살아났다면 벡터 연산을 해봅시다. 벡터 곱셈 연산을 위해서는 00Ｌ( ) 함수를 이용합니다.

1 np.dot(n1, 02)  # # ni. 11. dot (n2) 2} 같은 표현

Out array({[1, 2],
(3, 4]])

 1 ni.dot(n2) # 행렬 연산
Out array({[1, 2],
[3, 4]])

스칼라는 크기만 중요시하는 데 비해, 벡터는 방향과 크기가 모두 중요합니다. 그래서 다항 방

정식을 풀 때 요긴하게 쓰이지요. 이 책에서 다루지는 않지만, 머신러닝 프로그래밍을 할 때
파이썬이 인기가 높은 데는 벡터 연산을 쉽게 할 수 있게 해주는 넘파이의 공이 Suc}.

행끼리, 열끼리 연산

배열에서는 종종 행끼리 또는 열끼리 연산을 해야 할 필요가 있습니다. 일자별 주가 데이터에
서 최고가, 최저가, 평균가 등을 뽑는 경우가 그렇습니다. 넘파이는 이를 위해 한 줄 연산 기

196 3부 선물


===== PAGE 197 =====
능을 제공합니다. 한 줄 AAS 할 때는 축(3×15)을 지정해야 하는데, 열끼리 연산은 315=0,
행끼리 연산은 3%15ㅋ로 지정을 합니다.

1 # 배열 내 연산
2 03 = np.arange(12).reshape(3,4) _ ＊ @~112/ 배열을 만들고, (3*4)배열로 변환
3  pare (ns)

Out [[@ 1 2  3]
04566. 7]
[8 910 Jas

1 n3.sum(axis=@)  10 열( 합계

Out gurey(Ci2, 15, 18) 40

1 n3. sum(axis= 1) # HC) 합계

Out array([ 6, 22, 38])

ins: max(axis= 1) # 2 행( DOA, 최댓값

Out THON 85757110)

1 n3. ‘mean (axis= 0)   # 각 열( )의 평균값
7.]

Out array([ 4., 5., 6.,

축을 지정하지 않으면 한 줄 연산을 하지 않고 전체 원소에 대해 연산을 합니다.
1 print(n3.max()) # 최댓값
2 print(n3.min()) # 2#/#zt
3 print(n3.sum()) # 전체 합
4 print(n3.mean()) # 평균값
5 print(n3.std()) # 표준편차
6 print(n3.var()) # 분산
7 print(n3.cumsum()) # 2+ 원소의 누적 St
8 print(n3.cumprod()) # 각 원소의 누적 곱

10장 코딩 기술: 반복되는 데이터 197


===== PAGE 198 =====
Out 11

5.5

3.45205252953
|                        11.9166666667
:          [0 1 3 6 10 15 21 28 36 45 55 66]
|           [000000000000]

넘파이가 제공하는 연산의 종류는 다음과 같습니다.

Sis | 으으

max                  최댓값
min                  ES AG
a                               sum                  합계
mean                평균
std                  표준편차
var                  분산
cumsum            A 원소부터 해당 원소까지 누적 합
cumprod           첫 원소부터 해당 원소까지 누적 곱

배열에서 특정 데이터 뽑아오기

배열에서 일부 데이터를 뽑아와야 할 때는 슬라이싱(11008) 기능을 사용합니다. 파이썬 기
본 문법에서 리스트 내 데이터 슬라이싱을 하는 것과 동일한 방법인데, 다만 차원이 늘어났을
뿐입니다. 주의할 BS 첫 번째 데이터가 1이 아니라 0에서부터 시작한다는 것입니다. 즉, 슬
라이싱 주소 1은 두 번째 데이터를 가리킴니다.

renner

1 v=np.array({{11, 12, 13, 14, 15],
ot                 2            (21, 22, 23, 24, 25],
+                 3            [31, 32, 33, 34, 35],
4                  4            [41, 42, 43, 44, 45]])
|                Out
5
:

198 3248

|



===== PAGE 199 =====
1 # 83770에서 GIO/E{ 뽑아보기
2 vii, 2] # 2 3열 HOLES 추출

Out 23

ees YCLIC2))   # 이  2/와 같은 표현
Out 23

1 [:, 1] # 전체 행, 2열 900/터 추

Out eifey (12> 22 32; 4232

1 v(i:3, 1] # 2~3행, 2열 GIO/E] 추출

Out     array([22,_   32])

1 vil, :] #284, 전체 절 500/터 추출

Out array((21, 2250235024; re

지금까지 넘파이의 기본 사용법을 알아봤습니다. 더 자세한 내용을 알고 싶은 분은 공식 웹사
이트 10: //ww.numpy.org 를 참고하세요.

10.2 데이터베이스 YFAI= 팬더스

넘파이와 더불어 파이썬을 이용한 데이터 분석에서 빠지지 않는 라이브러리가 팬더스
(pandas) Ue}, 넘파이에서는 하나의 배열에 동일한 형태의 데이터만 담을 수 있지만, 팬더
스는 하나의 데이터프레임에 다양한 데이터를 집어넣고 쓸 수 있다는 차이가 있습니다.

또한 팬더스에서는 인덱스를 이용해 데이터를 조작할 수 있다는 장점이 있습니다. 일자별 주
가를 가져올 때,넘파이를 이용하는 경우와 팬더스를 이용하는 경우를 비교해봅시다. 12월 1
일부터 12월 31일까지의 주가를 넣어두고 12월 5일의 주가를 가져올 때, 넘파이에서는 12월

5일이 다섯 번째 날임을 이용해 array[4]2] 형태로 불러와야 하지만, 팬더스에서는 몇 번째
날인지 별도로 계산할 필요 없이 날짜를 인덱스로 설정해두고 데이터프레임['1205'1의 형태
로 불러올 수 있습니다.

10장 코딩 기술: 반복되는 데이터 199


===== PAGE 200 =====
팬더스를 이용하면 파이썬의 자료 구조를 엑셀의 스프레드시트와 같은 형태로 만들어 대용량
데이터를 쉽게 처리할 수 있습니다. 그뿐 아니라 팬더스는 스프레드시트 형태의 데이터를 데
이터베이스처럼 사용할 수 있게 해서, 사용자는 넘파이에서와 같이 특정 열이나 행의 데이터
를 쉽게 뽑아내서 사용할 수 있습니다.

팬더스로 1차원 데이터를 처리할 때는 시리즈(66065)를, 2차원 데이터를 처리할 때는 데이
=A] A (DataFrame)S 사용합니다. 금융 데이터를 처리하는 BPS 예로 들면, 1개 종목의
일자별 시세를 담아놓을 때는 시리즈로 충분하지만, 2종목 이상의 일자별 AVIS 담으려면 al
이터프레임을 사용해야 합니다.

시리즈

1차원 데이터, 즉 한 열(줄)만 있는 데이터를 처리할 때는 시리즈를 사용합니다. 물론 1차원
데이터만 다루는 경우에도 데이터프레임을 써도 되긴 하지만, 성능을 위해 시리즈를 사용합니
다. 꼭 필요한 것만 배우자는 우리 책의 컨셉에 따르면 데이터프레임만 배워도 충분하긴 합니
다만, 데이터프레임으로 가는 과정에 시리즈가 있으니 잠깐 둘러보고 가겠습니다.

시리즈나 데이터프레임을 사용하기 Fei pandas 라이브러리를 가져옵니다. 020085는 파이
썬에서 자주 쓰이는 라이브러리로 대부분의 프로그래머들이 00라고 줄여서 사용합니다.

1     import pandas as 00 # pandas 라이브러리를 00 이름으로 호출

Out

1개 종목의 주가를 담을 시리즈를 생성하기에 앞서 주가를 담은 리스트를 생성하겠습니다.

1     prices = [1000, 1010, 1020] # 주가를 담아놓은 리스트 생성

Out

Ae

200 348


===== PAGE 201 =====
pd.date_range(‘AlZt 날짜', '끝 날짜', 06「1005=날짜 수, 「60='주기')
둘 중 하나 지정            생략 가능

* 시작 날짜와 끝 날짜 또는 시작 날짜와 날짜 수(06ㄷ1005);를 쌍으로 지정해야 합니다.
주기(『「60)는 'ㅁ'(매일) '\'(매주) 'M' (DHS!) 등으로 지정. 생략 시 기본값은 'ㅁ'입니다.

date_rangeS 이용해 3일간의 날짜를 생성해 dateseh= 변수에 담습니다.

1 dates = 00.0216_「2006('20181201' , periods=3) # date_range 함수를 이용해 날짜 생성
2 dates

Out   DatetimeIndex([ "2 2018-12-01', '2018-12-@2', ‘2018-12-03'], dtype='datetime64[ns]',
pean D' )

시작 날짜를 2018년 18128, 끝 날짜를 1월 31, 주기를 '\' 로 지정하면 2018년 19194
터 시작해 1월 31일까지의 일주일 단위의 날짜를 돌려줍니다.

1 pd.date_range('20180101', '20180131',  freq=' Ww ye

Out DatetimeIndex(['2018-@1-@1', '2018-01-08', ‘2018-@1-15',
*2018-@1-22', '2018-@1-29'],
005 4519티00994000598 A Here W-SUN' a

o}Ho]= datesol] 저장한 날짜에 pricesol] 저장한 가격을 매치하여 시리즈를 생성합니다.
날짜를 인덱스로 하고 주가를 값으로 하는 시리즈(666165)는 다음과 같이 생성합니다. 5를
대문자로 쓰는 것에 주의하세요.

1 5 =pd.Series(prices, index=dates) # 주가를 데이터로, 날짜를 인덱스로 하는 시리즈 생성
2  5

Out 2018-12-01    1000
2018-12-02    1010
2018-12-03    1020

Epes  D,  ctype:  int64

그렇다면, 날짜를 지정하지 않고 값만 지정해 시리즈를 만들면 어떻게 될까요?

10장 코딩 기술: 반복되는 데이터 204


===== PAGE 202 =====
1 s2=pd.Series(prices) # 인덱스를 지정하지 않은 시리즈

252

Out @        1000

1        1010

2        1020
ope    int64

인덱스에 0부터 자동으로 숫자 일련번호가 매겨져 시리즈가 생성됩니다.

시리즈에 데이터를 추가할 때는 시리즈명[인덱스]=값의 형태로 지정합니다. 숫자로
가 매겨진 그 52에 네 번째 데이터를 추가해보겠습니다.

we
aN
[또

1 52[3] = 1030 # 시리즈에 데이터 추가

2552
Out 0         1000
1         1010
2         1020
3         1030

dtype: 10164

이번에는 날짜로 인덱스가 매겨진 시리즈 sol] 데이터를 추가합니다. 인덱스가 날짜 형식으로
지정되어 있으므로 추가할 때도 날짜 형식으로 인덱스를 지정해줍니다. 날짜 형식으로 인덱스
를 지정하기 위하여 0320025 함수인 pd.to_datetime ()-& 이용합니다.

프로그래밍을 할 때 사람이 보는 모양만 날짜처럼 보이는 것과 파이썬이 날짜로 인식하는 것
과는 큰 차이가 있습니다. 숫자를 예로 SOMA, 문자 BAl (str) Oe 되어 있는 '123'과 숫
자 형식(101)으로 되어 있는 123은 파이썬이 다르게 취급하게 됩니다. 문자 형식끼리 더하면
'123'+'123'='123123'이 되지만, 숫자 형식끼리 더하면 123+123=246이 되기 때문입니다.

1 print('123' + '123')
2 print(123 + 123)

Out 123123
246

202 34 선물


===== PAGE 203 =====
GAS 날짜 SAI (datetime) oS 저장하면 날짜 사이의 연산, 즉 며칠 전후. 날짜 간 차
이 SS 계산하는 것이 가능해집니다. 나중에 날짜 연산을 하기 수월하도록 날짜는 00.10_
datetime () 함수를 이용해 날짜 형식으로 지정해서 입력해줍니다.
pd.to_datetime( ' 날짜' )
날짜 모양으로 입력 (예 2018-01-01. 20180101 등)

* 문자 형식(5Ｌ「)의 날짜를 날짜 형식(0316ㄴ106)으로 변환

시리즈 5에 12월 4일의 주가 1030원을 추가하고, 추가된 5 AAS 출력해봅니다.

1    s[pd. to_datetime('2018-12-04')] = 1030 # 인덱스를 이용한 데이터 추가
2    Ss

Out 2018-12-01   1000
2018-12-02   1010
2018-12-03   1020
2018-12-04   1030
Freq: D, dtype: int64

시리즈도 리스트나 배열처럼 특정 데이터를 골라서 Bohs 수 있습니다.

00121? 배일 스타일로 데이터 추출, 위치가 20|므로 SEN 데이터가 다용 _

Out 1020

리스트와 HSS 데이터를 뽑을 때 위치(인덱스 숫자)만을 이용해야 했지만 시리즈는 레이블
(인덱스 이름)을 이용할 수 있습니다.

1     5['2018-12-03']  # 인덱스를 이용한 (이터 추출
Out 1020

108 코딩 기술: 반복되는 데이터 +203


===== PAGE 204 =====
데이터프레임 생성

데이터프레임은 2차원 배열입니다. 여러 종목, 여러 날짜의 시세를 한 번에 저장할 수 있습니
다. 데이터프레임을 만들 때는 딕셔너리를 만들어서 데이터프레임으로 변환하는 방법, 데이터
ZAMS 직접 만드는 방법, 시리즈를 데이터프레임으로 변환하는 방법 등 여러 가지가 있습
니다. 여기에서는 &전자, BES}, CHE 세 종목의 시세 데이터를 데이터프레임에 넣고 071이
라고 이름을 붙입니다. 우선 0ㅁ1665 덕셔너리를 만들고 나서, 딕셔너리를 데이터프레임으로
변환합니다. prices 덕셔너리는 각 종목의 OSS 키로, AVIS 담은 리스트를 값으로 하는
형태로 생성합니다.

1 prices = {‘AMA}' : [1000, 1010, 1020], # '종목명' : 1시세7
2         '8화학' : [2000, 2010, 2020],
3         '금융' : [3000, 3010, 30201}
4 dfi1=pd.DataFrame(prices) # 딕셔너리를 데이터프레임으로 변환
5 071

Out    AMA Bae Cas

0 1000 2000 3000
1 1010 2010 3010
2 1020 2020 3020

세 종목의 시세 정보를 담은 데이터프레임이 생성됐습니다. 하지만 인덱스를 별도로 지정하지
않아 0, 1, 2로 자동 지정 되어버렸네요. 일자별 시세답게 인덱스를 날짜로 지정해서 데이터
프레임을 만들어봅니다. 인덱스에 사용할 날짜는 앞에서 만들어둔 0365 리스트를 이용합니
다. 인덱스를 지정할 때는 데이터프레임() 안에 1106×%=[인덱스]를 추가합니다. 날짜 인덱스

가 있는 새로운 데이터프레임은 0+2로 지정합니다.

1 df2 = pd.DataFrame(prices, index=dates) # 인덱스가 있는 떼이터프레임
2 02

Out                    AMA} Bae Cas

2018-12-01 1000 2000 3000
2018-12-02 1010 2010 3010
2018-12-03 1020 2020 3020

204  3부 선물


===== PAGE 205 =====
데이터프레임 조회
데이터프레임에 저장된 데이터를 조회하는 방법은 리스트, 시리즈 등과 유사합니다. 다만 2차
원 데이터를 다루고 있으므로 행과 SS 따로따로 지정해주어야 합니다. 또한 시리즈에서와
같이 이름으로 데이터를 조작할 수 있다는 기능이 추가됩니다. 위치번호로 데이터프레임을 조
회하는 방법입니다.
데이터프레임.1100[줄번호, SHS]
열번호는 생략 가능. 생략하면 열 전체 선택

* 위치번호를 이용해 데이터프레임을 조회

리스트처럼 위치번호를 이용해 데이터프레임을 조회해봅니다.

1 df2.ilocfo] # 184 선택

Out AIA}       1000

8화학         2000
cas         3000

Name: 2018-12-01 00:00:00, 01106: 10164

행을 선택하려면 열을 우선 지정한 후 행을 지정합니다. 열 지정 방법은 리스트에서와 동일합
니다.

1 df2.iloc[:, 0] #134, 열 전체 선택

Out 2018-12-01   1000
2018-12-02   1010
2018-12-03   1028
Freq: D, Name: AMA}, dtype: 10164

1 df2.iloc{®, 0] # 134, 18 선택

Out 1000

|
|

팬더스의 멋진 기능인 레이블(121501)로 데이터 선택하기를 해보겠습니다.

10장 코딩 기술: 반복되는 데이터 205


===== PAGE 206 =====
데이터프레임.100['행 레이블, '열 레이블']
열 레이블은 생략 가능, 생략하면 열 전체 선택

* 레이블을 이용해 데이터프레임을 조회

령어가 1106에서 106로, [] 안에 넣어주는 매개변수가 숫자에서 문자로 veel 것을 제외하
사용법은 똑같습니다.

명
고

1 df2.loc[{'2018-12-01'] _ ＊ 134 선택
Out Aziz}   1000
8화학 2000
(금융 3000

Name: 2018-12-01 00:00:00, dtype: 10164

1 df2.loc[:, ‘AMAt'] #184, 열 전체 선택

Out 2018-12-01   1000
2018-12-02   1010
2018-12-03   1020
Freq: 0, Name: AZZ}, dtype: 10164

1 df2.loc['2018-12-01', '/전자'] # 184, 19) 선택

Out 1000

데이터프레임은 데이터 조작의 편의를 위해 레이블로 열 AAS 뽑아서 리스트로 반환하는 기
능을 제공합니다.

1 아2['4전자'] ee 선택

Out 2018-12-01   1000
2018-12-02   1010
2018-12-03   1020
Freq: D, Name: AAA}, dtype: 10164

1 0[2.4전자 # 072 '/4전자') 와 동일

206  3부 선물


===== PAGE 207 =====
out  2018-12-01   1000
2018-12-02    1010
2018-12-03    1020
ied:  D, Name: 전자; (9430  int64

1 072['전자']['2018-12-01'] # 열 선택 후 BY 선택

Out 1000

1 df2.loc{:, '/전자']['2018-12-01'] ㆍ # 072( '4전자'7( '2016-12-01'7 와 동일한 표현

Out 1000

데이터프레임에 데이터 추가

세 종목의 2018년 12월 1일부터 3일까지 일자별 시세가 생성되었습니다. 데이터프레임에 새
운 종목을 추가하려면 어떻게 할까요? 데이터프레임[ '종목명'] = [시세]처럼 지정해서 추

가할 수 있습니다.

1 072['0엔터'] = [4000, 4010, 4020]  # 데이터프레임에 열 추가
2 df2

Out         AMX} BSS Cas ㅁ엔터
2018-12-01 1000 2000 3000 4000
2018-12-02 1010 2010 3010 4010
2018-12-03 1020 2020 3020 4020

데이터프레임에 종목을 추가할 때 이미 만들어둔 시리즈를 이용할 수도 있습니다. 데이터프레
임[ ols") = 시리즈와 같이 지정합니다. 앞의 시리즈 예제에서 만들어두었던 시리즈 5를
이용해 8텔레콤 시세를 추가하겠습니다. 5에 저장된 값 중 072의 인덱스에 해당하는 값들만
선택되어 072에 저장됩니다.

1 072['6텔레콤'] = ㅎ # 시리즈에서 데이터프레임 열 추가
2 012

10장 코딩 기술: 반복되는 데이터 207


===== PAGE 208 =====
Out        AMA Bee cag OCH ECAE

2018-12-01 1000 2000 3000 4000          1000
2018-12-02 1010 2010 3010 4010     1010
2018-12-03 1020 2020 3020 4020          1020

데이터프레임 확장
시리즈를 이용해 데이터를 추가할 때 인덱스에 없는 값도 추가하려면 60008 기능을 이용합

oe

니다. 앞서 소개한 방법은 기존 데이터프레임에 데이터를 추가하는 방식이었던 반면, concat
을 사용하는 방법은 데이터프레임을 확장하는 방법이라고 이해하면 됩니다.

pd.concat(A, 8, axis=1)
합쳐질 데이터프레임 합치는 방향 OS sy, 12 열>)

* 데이터프레임을 병합
우리가 계속 만지고 있는 df22} 앞서 만들어둔 시리즈인 6를 병합하여 0+2에 담아보겠습니다.
종목명을 『수프트로 지정해 병합하며, SSS 추가하는 방향으로 합하기 때문에 So] 확장되
는 방향인 axis=1= 지정합니다.

우선 시리즈 5의 이름을 '『소프트'로 지정합니다.

1 s.name = 소프트 '

2025

Out 2018-12-01   1000
2018-12-82   1010
2018-12-03   1020
2018-12-04   1030
Freq: D, Name: 『소프트, dtype: int64

이제 072에다가 시리즈 5를 병합합니다.

208  3부 선물


===== PAGE 209 =====
1 df2 = pd.concat({df2, 5], axis=1)

2 df2

Cue      AMZ} Balt CBS OWE ESAZ FAHE
2018-12-01 1000.0 2000.0 3000.0 4000.0 1000.0  1000
2018-12-02 10100 2010.0   3010.0 4010.0      1010.0        1010
2018-12-03 1020.0 2020.0 3020 0 4020.0      1020.0        1020
2018-12-04  NaN  NaN  NaN  NaN  NaN  1030

이번에는 12% 7일에 129 1일보다 시세가 60원씩 오른 AS 데이터프레임에 추가하려고 합

니다. 12월 7일의 시세를 간단히 만들려면 12월 1일의 AAS 가져와서 60원씩 더해주면 되
겠네요. 데이터프레임 연산을 통해 간단히 처리할 수 있습니다.

© 0+2에서 12월 1일 자 시세를 추출해서 073에 저장하고,
@ 60원씩 더합니다.
© 073에 12월 7일이라고 레이블을 지정한 후,
(@) 072에 YS 추가해주면 됩니다.
행을 추가할 때는 데이터프레임.8200600(추가할 데이터프레임 )을 이용합니다.

df3 = df2.iloc{e] #@

df3 = df3

df3

Out ㅅ전자
8화학
금융
[엔터
텔레콤

FADE

+ 60

2060.8
3060.8
4060.0

# @

1
2
3 df3.name = pd.to_datetime(' 20181207" )  # @
4

1060.0

1060.0
1060.0

Name: 2018-12-07 00:00:00, dtype: float64

1 df2 = df2.append(df3) # @

2 012

10

zt

코딩

기술: 반복되는 데이터 209



===== PAGE 210 =====
AMA BES Cas OMA EGG 소프트
2018-12-01 1000.0 2000.0 3000.0 40000 1000.0 1000.0
2018-12-02 1010.0 2010.0 30100 40100 10100 1010.0
2018-12-03 1020.0 2020.0 3020.0 40200 10200 1020.0
2018-12-04        NaN        NaN        NaN        NaN           NaN 1030.0
2018-12-07 1060.0 2060.0 3060.0 4060.0 10600 1060.0

Out

129 6일의 시세는 122 1일보다 50원씩 올랐다고 합시다. 앞에서와 같은 방법으로 추가할
수 있습니다.

1 df3 = 0【2.11060[0] + 50 #@, (2)

2 df3.name = pd.to_datetime('20181206') #@
3 df2 = df2.append(df3) #@

4 df2

Out

^전자 BEI CHS DWH EEAG 【소프트
2018-12-01 1000.0 2000.0 3000.0 4000.0 1000.0 1000.0
2018-12-02 1010.0 2010.0 30100 40100 1010.0 1010.0
2018-12-03 1020.0 2020.0 3020.0 4020.0 1020.0 1020.0
2018-12-04        NaN NaN        NaN        NaN           NaN 1030.0
2018-12-07 1060.0 2060.0 3060.0 4060.0 1060.0 1060.0
2018-12-06 1050.0 2050.0 3050.0 4050.0 1050.0 1050.0

124 62 자 시세까지 저장해놓고 보니 날짜가 역전되어 있네요. 124 7일이 6일보다 앞에 있
으니 보기에 좋지 않습니다. 게다가 이렇게 LEE 위치번호로 데이터를 뽑을 때 문제가 생기
겠네요. 날짜순으로 다시 정렬하면 좋겠습니다. 데이터프레임 인덱스를 재정렬하려면 50「+_…
indexS 사용합니다.

210 3부 선물


===== PAGE 211 =====
데이터프레임.50「『_1006×(2×15=0, ascending=True)
axis=O2 Wwe} axis12 SYS _7ㅠ46(기본값)이면 오름차순, 생략 가능

* 데이터프레임의 인덱스를 재정렬

0+2를 날짜 오름차순으로 재정렬하겠습니다.

1 df2 = df2.sort_index(axis=@) # 날짜순으로 인덱스 재정렬
2 df2

Out

AMA Ba CHS OWE ESAG FARE
2018-12-01 1000.0 2000.0 3000.0 40000 10000 1000.0
2018-12-02 10100 20100 30100 40100 10100 1010.0
2018-12-03 1020.0 2020.0 30200 40200 10200 1020.0
2018-42-04       NaN       NaN       NaN       NaN         NaN = 1030.0
2018-42-06 1050.0 2050.0 30500 40500 1050.0 1050.0
2018-12-07 1060.0 2060.0 3060.0 40600 10600 1060.0

df27} 날짜 순서대로 정렬되었습니다.

데이터프레임에서 데이터 빼기
데이터를 추가하고 정렬하는 AUS 해봤으니 이제 빼볼까요? 데이터프레임에서 데이터를 B
때는 drop 명령을 사용합니다.
데이터프레임.0000(18661, axis=0)
BY 행/열의 인덱스명 = qxis=1 0/1 열 삭제, 기본값은 346=ㅇ
* 데이터프레임에서 행 또는 열 삭제

빼내기 예제 실습 시에는 ARS 저장하지 않겠습니다. 실습하면서 데이터를 다 빼버리면

추가적인 실습을 할 재료가 남지 않으니까요.

볼

012에서 12월 6일의 데이터를 빼보겠습니다. 눈으로 보는 인덱스 값은 2018-12-06이지

10장 코딩 기술: 반복되는 데이터 211


===== PAGE 212 =====
만 파이썬 내부에 저장된 값은 날짜 BA} (datetime)2] 2018년 12월 6일입니다. 그래서 그
냥 drop ('2018-12-06' )이라고 하면 에러가 발생하니 꼭 날짜 형식인 pd.to_datetime
('2018-12-06' )처럼 지정해줘야 합니다. 삭제한 데이터프레임을 저장하지 않으므로 현재
BRIA 삭제된 것처럼 보이나 072에 삭제한 결과가 저장되지 않음에 주의하세요.

1 df2.drop(pd.to_datetime('2018-12-06'))  # 8¥ 삭제

Out      스전자 Bae Cas OWE ECAR FATE
2018-12-01 1000.0 2000.0 3000.0 4000.0  1000.0 1000.0
2018-12-02 1010.0 2010.0 3010.0 4010.0  1010.0 1010.0
2018-12-03 1020.0 2020.0 3020.0 4020.0  1020.0 1020.0

2018-12-04  NaN  NaN  NaN  NaN   NaN 1030.0
2018-12-07 1060.0 2060.0 3060.0 4060.0 1060.0 1060.0

12월 62 자 데이터를 빼냈습니다. 이번에는 12월 2일과 62) 자 데이터를 동시에 삭제해보겠
습니다.

1 012.0000([00.10.02161106('2018-12-02'), pd. to_datetime('2018-12-06')])   # 여러 SH 삭제
Out

스전자 Beret CHS DWH ESAZ FATE
2018-12-01 1000.0 2000.0 3000.0 4000.0 10000 10000
2018-12-03 1020.0 2020.0 30200 40200 10200 1020.0
2018-12-04        NaN        NaN        NaN        NaN           NaN 1030.0
2018-12-07 1060.0 2060.0 3060.0 4060.0 1060.0 1060.0

이번에는 일자별(행)이 아닌 종목별(열) 데이터를 삭제해봅시다.

1 df2.drop(‘D%E{', axis=1) # 열 삭제

Out       AMA} Beet CHS EWE FADE
2018-12-01 1000.0 2000.0 30000 10000 10000
2018-12-02 1010.0 2010.0 30100 10100 10100
2018-12-03 1020.0 2020.0 3020.0 10200 10200
2018-1204 NaN NaN NaN NaN 10300
2018-12-06 1050.0 2050.0 3050.0 1050.0 1050.0
2018-12-07 1060.0 2060.0 3060.0 1060.0 10600

212 3부 선물


===== PAGE 213 =====
1  072.0000(['<금융', '6텔레콤'], axis=1) # 여러 열 삭제
Out

AMA BSH DME, FARE
2018-12-01 1000.0 20000 40000 10000
2018-12-02 1010.0 20100 40100 1010.0
2018-12-03 1020.0 2020.0 40200 10200
2018-1204 NaN NaN NaN 1030.0
2018-12-06 1050.0 20500 40500 10500
2018-12-07 1060.0 20600 4060.0 10600

데이터프레임 구멍 메우기(보간법)

지금까지 진행하면서 데이터프레임에 있는 34이라는 값이 눈에 거슬렸을 텐데 오래 참고 기
다리셨습니다. NanS 데이터가 없다는 HOB, 엑셀의 N/ag} 같은 표현입니다. 즉 12월 4일
에는 『소프트를 제외한 다른 종목들은 시세 정보가 없다는 뜻이지요.

이런 구멍 난 데이터를 없앨 땐 데이터프레임.0ㅁ0002 ( ), 다른 값으로 메울 땐 데이터프레
임.711108 ( ) 명령을 사용합니다.

데이터프레임.0170002()
* 데이터프레임에서 NaNo| 포함된 행 삭제

데이터프레임.000008( )를 수행하면 Nan 값이 포함된 BS 지워버립니다.

1 df2.dropna() # NaN 제거

AMA BRS (금융 OWE ESAS FAZE
2018-12-01 1000.0 2000.0 3000.0 4000.0 10000 10000
2018-12-02 1010.0 2010.0 3010.0 40100 10100 1010.0
2018-12-03 1020.0 20200 3020.0 4020.0 10200 10200
2018-12-06 1050.0 2050.0 3050.0 40500 10500 10500
2018-12-07 1060.0 2060.0 3060.0 40600 10600 10600

108 코딩 기술: 반복되는 데이터 213


===== PAGE 214 =====
NaNO] 있던 12월 4일 자 데이터가 모두 지워졌습니다. 심지어 『소프트는 값이 있었는데도 말
이지요. 있는 데이터마저 지워버리는 것은 데이터를 소중히 하는 데이터 과학자에게는 가슴
아픈 일이지요. 그래서 보통 다른 값으로 대체합니다.

데이터프레임.『111083(대체값 또는 방법)
0, 1 등 US 지정하면 해당 값으로, method=ffill/bfillLo|s 앞/뒤 값으로 변경

* 데이터프레임에서 NaN 값을 다른 값으로 대체

데이터프레임.11102 ()S 이용해서31 값을 0으로 바꿔보겠습니다.

1 df2.fillna(®) # NaANS 0으로 바꿈

Out
AMA, BSS CBS 0ㅁ엔터 ㄷ델레롬 소프트

2018-12-01 1000.0 2000.0 30000 40000 10000 1000.0
2018-12-02 10100 20100 30100 40100 10100 1010.0
2018-12-03 10200 20200 30200 40200 10200 10200
2018-12-04          00          00          0.0          0.0             00 1030.0
2018-12-06 1050.0 2050.0 3050.0 40500 10500 1050.0
2018-12-07 1060.0 2060.0 3060.0 40600 10600 10600

NaNO] 모두 0으로 바뀌었죠? 그런데 시세가 이렇게 SsbA 그래프가 금융 데이터 분석
을 정상적으로 수행할 수 없습니다. 주가는 추가적인 거래가 일어나지 않으면 전일 가격이 그대
로 유지됩니다. 그래서 주식 데이터의 빈칸을 채울 땐 『『111 (forward (111 )을 이용합니다.

1 df2.fillna(method="ffill') # /09//을 앞의 값으로 채움

Out
ASA} BER CHS OCH ESAS [소프트

2018-12-01 10000 20000 30000 40000 10000 1000.0
2018-12-02 10100 20100 30100 40100 10100 1010.0
2018-12-03 1020.0 20200 30200 40200 10200 10200
2018-12-04 10200 20200 30200 40200 10200 1030.0
2018-12-06 1050.0 20500 30500 40500 10500 1050.0
2018-12-07 1060.0 20600 30600 40600 10600 1060.0

214 3448


===== PAGE 215 =====
AZIZ} 12월 4일의 Nano] 12월 3일 값인 1020원으로 바 것을 확인할 수 있습니다. 주가 데
이터가 아니고 뒤에 오는 데이터가 더 중요한 경우에는 역방향인 07111 (backward 1111 )을
사용합니다.

1 df2.fillna(method="bfill') # NaNS 뒤의 값으로 채움

he      AMA 화학 cas ㅁ엔터 EAS 다소프트

2018-12-01 1000.0 2000.0 3000.0 4000.0 10000 1000.0
2018-12-02 10100 20100 30100 40100 10100 1010.0
2018-12-03 1020.0 2020.0 3020.0 4020.0 1020.0 1020.0
2018-12-04 1050.0 2050.0 3050.0 40500 1050.0 1030.0
2018-12-06 1050.0 2050.0 3050.0 4050.0 1050.0 1050.0
2018-12-07 1060.0 2060.0 3060.0 4060.0 10600 10600

AIA} 122) 429] Nano] 12%) 6S 값인 1050원으로 변경되었습니다.

지금까지 팬더스를 이용해 데이터를 정리하고 처리하기 위한 기능을 살펴보았습니다.

10장 코딩 기술: 반복되는 데이터 215


===== PAGE 216 =====
11.1 KOSPI200 선물 이론가 산출

지금까지 공부한 선물 이론과 파이썬 코딩 기술을 바탕으로 KOSPI200 선물 이론가를 산출하
고 실제 선물가격과 비교해보겠습니다. 이론가 산출에 필요한 데이터는 앞서 엑셀 실습에서
이용했던 09.2 KOSP1200 F 201712.×15*이며, 팬더스를 이용해 엑셀 파일에서 데이터를 읽
어와 데이터프레임에 저장해두고 사용하는 방법도 공부합니다.

엑셀에서 데이터 읽어오기
우선 데이터가 들어 있는 엑셀 파일을 살펴봅니다. 일자별로 선물가격과 지수가 들어 있습니다.

4    eee 베버 네  De eee SRE eG [시
1 a 선물가격 | 저수

2017/09/01 | 308.4 | 307.78
3 | 2017/09/04 | 305.6 | 304.19
4 | 2017/09/05 | 304.85 | 304.06
5 | 2017/09/06 | 304.3 | 303.18
6 | 2017/09/07 | 308.1 | 306.97
7
8
9

2017/09/08 | 308.35 | 307.43
2017/09/11 | 311.5 | 309.83

2017/09/12 | 311.45 | 310.42

216 3부 선물



===== PAGE 217 =====
엑셀에서 데이터를 읽어오고 저장하는 기능은 팬더스를 이용합니다. 또한 고급 수학 계산을
위해 넘파이를 이용합니다. 노트북에서 팬더스와 넘파이 라이브러리를 호출합니다.

1 import pandas as pd
2 import numpy as np

Out

엑셀 파일에서 데이터를 읽어올 w= pd. read_excel ()-& 사용합니다.

00.「630_6×661Ｌ(엑셀 파일명, 시트명, 1006×_001=칼럼명)
(시트명은 생략 가능, 생략 시 1번 시트)          (칼럼명도 생략 가능, 생략하면 0. 1, 2, …로 인덱싱)

* 엑셀 파일에서 데이터를 불러와 팬더스 데이터프레임을 생성

* 엑셀 파일이 파이썬 노트북 파일과 다른 폴더에 있다면 경로명을 파일명 앞에 붙여야 합니다(예: ' . ./엑셀/9 .2
KOSPI200 F 201712.×15×').

데이터가 들어 있는 AEE Sheet1°]a2 일자를 기준으로 데이터가 들어 있으므로 시트명은
'Sheet1' & 지정하고 1706×_001='일자'라고 지정해서 데이터를 불러옵니다. BAe 데이
터는 데이터프레임 dfol 저장합니다.

1 df = pd.read_excel('@9.2 KOSPI200 F 201712.xlsx', ‘Sheet1', 1006×_001='일자')
2 df.head()

Out         선물가격 지수
일자

2017/09/01        308.40 307.78
2017/09/04        305.60 304.19
2017/09/05        304.85 304.06
2017/09/06    304.30 303.18
2017/09/07        308.10 306.97

여기에서는 다루지 않지만 엑셀에 데이터를 저장할 wh pd. to_excel (M4 파일명, AES)
을 사용합니다. pd.to_excel() 사용법을 알고 싶은 BS 노트북 화면에서 help (pd. to_

11장 금융공학 모델링 217



===== PAGE 218 =====
excel) o|2}31 입력하고 [Shift]+[Enter]S 눌러 실행하면 나오는 매뉴얼을 참고해 사용법
을 배워보기 바랍니다.

불러온 데이터를 정상적으로 이용하려면 인덱스 칼럼이 날짜 형식으로 지정되어 있어야 합니
다. 인덱스 칼럼 데이터의 형식을 확인해봅니다.

1    __type(df.  index)

Out  pees core. indexes. base. Index

엑셀에서 SAS 일자는 파이썬에서 날짜 형식이 아닌 문자 형식으로 인식된 상태입니다. 날
짜 형식으로 변환을 해줘야 잔존만기 계산을 할 수 있습니다. 일자는 df] 인덱스
df.indexS 불러와서 날짜 형태로 변환해주는 00.10_0361106( ) 함수에 넣어 변환한 뒤
0+.1006×에 다시 저장해줍니다.

1 df.index = pd.to_datetime(df.index)
Out

이제 다시 인덱스 칼럼 데이터 형식을 확인해봅니다.

1    type(df.  index)

Out  80085 core. indexes.datetimes.DatetimeIndex

인덱스 칼럼이 날짜 형식으로 저장된 것을 확인할 수 있습니다.

선물 이론가 산출
이제 이론가 산출을 위해 선물 이론가 공식을 다시 한번 살펴보겠습니다.

F cc Sela)!

(F: 선물가격, 6: 현물가격, /: 이자율, 0: 배당률, : 잔존만기)

218 3부 선물



===== PAGE 219 =====
잔존만기는 최종거래일(만기일)까지 남은 날짜 수를 의미하는데, 1년이 남았으면 잔존만기를
1로 계산합니다. 금융공학에서는 1년을 보통 250일 정도로 계산하고, 이 책에서는 계산 편의
를 위해 252일로 정했었습니다. 따라서 남은 날짜 수를 252로 나누면 잔존만기가 나옵니다.
수식으로 하면 G7 Sole) 이 됩니다.

파이썬으로 두 날짜 사이에 며칠이 있는지 계산할 때는 (날짜2 - 날짜1) .035를 이용합니
다. 그런데 이 방법은 주말을 포함한 날짜를 결과로 보여줍니다. 우리가 1년을 365일이 아
닌 252일로 잡은 근거는 휴일에는 거래가 없기 때문이지요. 따라서 daysS 이용하면 안 됩
니다. 공휴일을 제외한 영업일만을 계산하려면 넘파이가 제공하는 ㅁ0ㅁ.045027_ㄷ040(날짜
1, 날짜2)를 이용해야 합니다. 이를 이용해 잔존만기를 파이썬 코드로 나타내보겠습니다. 만
기일자를 , 기준일자를 tO, 잔존만기를 +라고 하면 + = np.busday_count (t@.date(),
T.date()) / 252가 됩니다.

자연지수는 00.6×0 ( )를 이용합니다. 6 -""는 00ㅁ.6×0ㅁ((「-0 )*【)라고 코딩합니다. 지금까
지 내용을 종합해서 선물 이론가를 산출하는 함수를 만들어보겠습니다.

1 def futures_price (5, r, 0, 1, 10):

2     t = np.busday_count(t@.date(), T.date()) / 252
3      F = S * np.exp((r-d)*t)
4     return F

Out

위에서 작성한 함수를 이용해 KOSPI200 선물 이론가를 계산해보겠습니다. 해당 ASS
2017년 12월 만기 상품으로 만기일은 2017년 12월 14일입니다. 이자율과 배당률은 앞서 사
용했던 것과 동일하게 2.25%, 1.5%를 이용합니다.

T = pd.to_datetime('2017-12-14') # 최종거래일
r= @.0225 # 이자율
d=0.015 # HSS
for n in (df.index):
t@=n
5 =df.loc{n, '지수']
F = futures_price (5, r, 0, 1, 10) # 함수를 호출해 선물 이론가를 받아와 Foy 저장
f = '{:,.2f}'.format(F)  # 이론가 숫자 포매팅

on DUN fF WN PK

11장 금융공학 모델링 219



===== PAGE 220 =====
9     df. troll  AUiadgh ue =f # 'O/27H' 칼럼에 값 추가

위 코드에서 8행을 보면 '{: , .21} ' .70ㅁ02 )라는 코드가 보입니다. 이 코드는 정수 부분

은 천의 자리마다 쉼표(, )를 추가해 가독성을 높이고 소수점 아래는 두 자리까지만 표시하도

록 포매팅하는 부분입니다. 정확한 숫자를 다 보고 싶다면 별도의 포매팅이 필요하지 않지만,
른 숫자들과 모양을 맞춰주기 위해서는 통일성 있는 포매팅이 필요합니다.

보급형 공식을 이용한 선물 이론가 계산
이번에는 연속복리이자율이 아닌 단리 개념의 보급형 공식을 이용한 이론가 계산입니다. 우선
공식을 살펴보겠습니다.

F=S|1+(r    -d)x x4

(F: 선물가격, S: 현물가격, r: 이자율, 0: 배당률, t: 잔존만기)

단순형에서는 더 쉽게 이해하기 위해 1년을 252일이 아닌 365일로 합니다.

1 def S_futures_price (5, r, 0, 1, 10):

2     t = (1 - t@).days / 365  # 잔존만기 계산
4     return F

Out

연속복리이자율과의 차이점은 날짜 계산입니다. 365일을 기준으로 잡았기 때문에 주말까지
포함한 날짜 AALS 해야 합니다. 따라서 (날짜2- 날짜1) days 를 이용합니다.

이 함수를 이용해 선물 이론가를 산출해봅니다.

1 T = pd.to_datetime('2017-12-14') # 최종거래일
2 r=0.0225 # 지율

220 3# 선물


===== PAGE 221 =====
3 0=0.015 # Hohe

4 for ㅁ in (df.index):

5      t@=n

6     5 = df.loc{n, '지수']

7     F = S futures_price (5, r, 0, T, t0) # 함수를 호출해 선물 이론가를 받아와 Fol 저장
8      f = '{:,.2f}'.format(F) # 이론가 숫자 포애팅

9     0『.106[0, '이론가2'] =f ＊ '이론가2' 칼렁에 값 추가

Out
이제 두 공식을 이용해 계산한 선물 이론가를 확인해봅시다.
al hy                      dk  자아 00
Out                ar

선물가격 AS 이론가1 이론가2

2077-09-01        308.40 307.78 30846 308.44
2017-09-04 305.60 30419 30485 304.82
207-2005 30485 304.06 30471 30468
2077-09-06 304.30 303.18 30382 303.80

2037 05-07 308.10 306.97 307.61 307.59

—_—

선물가격은 실제 거래된 해당 일자의 선물 종가이고, 이론가1은 연속이자율을, 이론가2는 단
순이자율을 이용해 계산한 이론가입니다.

지금까지 KOSPI1200 지수를 기초자산으로 하는 선물 이론가를 계산하고, 실제 KOSPI200 선
물가격과 비교해보았습니다. 이제 선물 모델링을 할 수 있겠죠?

11.2 WTI 선물가격을 이용한 롤오버 비용 계산
선물 이론을 배우면서 롤오버의 의미와 롤오버 리스크에 대해 알아보았습니다. 여기에서는 롤
오버 비용이 손익에 미치는 영향이 얼마나 큰지 서부 텍사스 SAR WD 선물가격을 바탕

으로 모델링해보며 알아보겠습니다.

원유 가격은 2014년 중반만 해도 배럴당 100달러를 넘어서며 고가 행진을 계속하다 2014년

11장 금융공학 모델링 221


===== PAGE 222 =====
부터 2016년까지 급락하며 많은 투자자에게 SAS 안겨준 대표적인 상품입니다. 여기에서는
2010년부터 2017년까지 서부 텍사스 중질유 현물에 투자했을 경우와 선물에 FARMS 경우
의 손익이 어떻게 될지를 비교해보며 롤오버 비용에 대해 알아보겠습니다. 롤오버 비용 계산
을 위해 서부 텍사스 중질유 ASO] 최근월물(76010 ㅁ10ㅁ01)과 차근월물(6600ㅁ0 month) 가
AS 이용합니다. 서부 텍사스 중질유 현물과 선물가격은 엑셀 파일로 제공합니다.

참고로 이번 실습에 사용할 데이터는 고가의 금융정보 제공 매체인 블룸버그(81001015018)
에서 다운받았음을 밝힙니다. 블룸버그는 월 사용료만 수백만 원이 넘는 고가의 정보 매체로
대부분의 금융회사가 국내외 금융정보 2318 위해 사용하고 있습니다. 금융회사에서 일하거
나 경영대학원에서 MBA 공부를 하게 되면 블룸버그를 접할 기회가 생기게 될 것입니다.

ZB, 차근월물 용어 정리
* 37S: 만기를 앞두고 있는 선물. 영어로는 00 month, lead month, first 70101 등으로 표현.
* 차근월물: 다음 주기에 만기가 도래할 선물. 영어로는 second month= 표현.

* KOSPI200 선물의 경우 분기별로 만기가 도래해 3, 6, 9, 12월에 만기가 있는데, 지금이 1월 1일이라
면 3월 만기 선물이 최근월물, 6월 만기 선물은 차근월물이 됩니다. 반면, 서부 텍사스 중질유 선물의 경
우 매달 만기가 도래하기 때문에 지금이 1 월 1일이라면 1월 만기 선물이 최근월물, 2월 만기 선물이 차
근월물이 됩니다.

엑셀에서 WTI 현물, 최근월물, 차근월물 데이터 읽어오기

먼저 엑셀 파일을 준비합니다. 책의 웹사이트에서 다운로드한 11.2 \11.×15× 파일을 열어보
H ‘Spot 시트에는 \71 지수(현물가격), Front 시트에는 최근월물 가격, ‘Second’ 시트에는
차근월물 가격이 담겨 있는 것을 확인할 수 있습니다.

앞의 실습에서와 같이 엑셀에서 데이터를 읽어오고 저장하는 기능은 팬더스를 이용합니다. 또
한 NaN 데이터 처리를 위해 넘파이를 이용합니다.

1 import pandas as pd
2 import numpy as np

Out

222 3부 선물


===== PAGE 223 =====
pd.read_excel()-& 이용해 엑셀 파일의 각 시트에서 데이터를 불러오고 03【6를 인덱스로
하여 데이터프레임인 01. 02, 073에 저장합니다.

1 001 = pd.read_excel(‘'11.2 WTI.xlsx', ‘Spot’, index_col='Date')

2 df2 = pd.read_excel('11.2 WTI.xlsx', ‘Front’, index_col='Date’)

3 df3 = pd.read_excel('11.2 apie  "Second', index_col='Date')
Out

df1, df2, 073를 하나의 데이터프레임으로 합쳐 새로운 데이터프레임인 0『에 저장하고
df.tail() 명령어로 dfoll 3개의 데이터프레임이 잘 합쳐졌는지 확인합니다.

1 df = pd.concat([{df1, 072, 073], axis=1)
72 (hic 1190

Out                             Spot Front Second
Date

2010-01-08 82.75 82.75         83.30
2010-01-07 8266 82.66    83.19
2010-07-06 83.18 83.18    83.75
2010-01-05 8177 81.77    82.41
2070-01-04 8151 81.51     82.12

20104 14 4일부터 데이터가 들
Second 칼럼에 저장되어 있는 것을 확인할 수 있습니다. 데이터에 구멍이 난 Lo] 있을 수 있
멍

으니 11108 ( ) 명령을 이용해 구멍을 메우는 보간법을 시행합니다.

가

1 df = df.fillna(method='ffill') # 앞의 에이터를 가져와 NaN ZS 덮어송
2 df =df. falta Gethode! bfill') # $/2/ 떼이터를 가져와 NaN 값을 Boj

Out

엑셀에서 WTI 만기일 정보 읽어오기
롤오버는 유동성(필요한 만큼 차근월물을 확보할 수 있는지 여부)과 가격(유동성이 높아져 차근월물 가

11장 금융공학 모델링 223


===== PAGE 224 =====
Ao] 합리적인지 여부)을 고려해 대체로 만기일에 가까워지면 시행합니다. 2010년부터 2017년
까지 만기일에 롤오버를 시행하기 위해 만기일 정보가 필요합니다. 만기일 정보는 같은 엑셀
파일 내에 ‘Expiry’ 시트에 들어 있습니다. 앞 절에서와 같은 방식으로 wil 선물 만기일 정보
를 가져와 df_eol] 저장합니다. 만기일 정보는 딱히 인덱스가 필요하지는 않습니다.

1 df_e = pd.read_excel('11.2 WTI.xlsx', ‘Expiry’)
2 df_e[{120:125]

보바                    Ticker           Month LastTrade Last Price
120 CLG10 2017-02-10 01/20/10           77.62
121 CLH10 2017-03-10       02/22/10           80.16
122 CLJ10 2017-04-10 03/22/10           81.25
123 CLK10 2017-05-10 04/20/10           83.45
124 CLM10 2017-06-10 05/20/10           68.01

월별로 구분되어 있는 선물상품과 최종거래일 정보가 들어 있습니다. 이 중에서 우리가 필요
한 AHS Last 1「306 열입니다. 0 _6에서 Last Trade Ul 추출해서 보겠습니다.

1 # 만기일 추출
2 df_e['Last Trade'].head()

Out @          01/20/00

1 = 02/22/00
2 03/21/00
3 04/19/00
4 05/22/00

Name: Last Trade, dtype: object

최종거래일이 잘 표시되긴 하지만 06406: objectH 되어 있는 AS 보니 날짜 형식은 아닙
니다. 데이터 처리 시 편의성을 위해 날짜 형식으로 wy} (to_datetime 함수 사용) 시리즈에
저장하겠습니다. 새로운 시리즈 이름은 6<011「*로 합니다.

1 # 추출한 만기일 정보를 시리즈에 저장
2 expiry = pd.Series(pd.to_datetime(df_e['’Last Trade']))
3 expiry.head()

224  3부 선물


===== PAGE 225 =====
2000-01-20

1 2000-02-22
2 2000-03-21
3 2000-04-19
4 2000-05-22

Name: Last Trade, dtype: datetime64[ns]

expiry] 최종거래일 정보가 datetimes4 SY = 저장됐습니다.

시세 데이터프레임에 최종거래일 표시하기

롤오버는 최종거래일에 최근월물을 팔고 차근월물을 사서 포지션을 유지하는 거래를 Be
다. 롤오버를 하지 않으면 최근월물은 WIS 맞이하고 포지션이 자동으로 정리되면서 잔고는
0으로 변하게 되지요. 최근월물을 팔고 차근월물을 사는 거래는 최종거래일에 일어나기 때문
에 시세 데이터에 최종거래일을 표시해주어야 합니다. 우선 0+에 최종거래일을 표시할 칼럼
을 추가하겠습니다. 이름은 만기를 뜻하는 ExpiryS 하고, 아직 데이터가 WOES Nan 값을
입력합니다. Nan 값을 만드는 데는 넘파이 기능인 np.nanS 사용합니다.

1 df['Expiry'] = np.nan
2 df.head()

Out

Spot Front Second Expiry
Date

2017-12-28 5984 59.84         59.87         NaN
2017-12-27 59.64 59.64         59.69         NaN
2017-12-26 59.97 59.97         60.00        NaN
2017-12-22 58.42 58.47         58.54         NaN
2017-12-21 58.33 58.36         58.40        NaN

이제 최종거래일에는 Expiry 칼럼의 WS 1로 표시해서 최종거래일을 구분하겠습니다. O df
에서 순차적으로 Date 칼럼의 WS 읽어서 © 앞에서 만들어두었던 expiry 시리즈에서 찾아
보고 해당 Date 값이 존재하면 최종거래일이 맞으니 ® Expiryoll 1이라고 표시합니다.

Date 값은 df 데이터프레임의 인덱스로 사용되고 있으니, Date 값을 가져올 WHE df. 1006×를

11장 금융공학 모델링 225


===== PAGE 226 =====
가져오면 됩니다. SAAS expiry 시리즈의 값이므로 600ㅠ1「\.'31465로 불러옵니다.

1 # Trading day 중 만기일 찾아서 표시하기

2 ford 10 df.index: # DatezgtS 하나씩 읽어와서

3      if d in pd.to_datetime(expiry.values): # expiryOl] 같은 값이 있으면
4        df.loc{d].Expiry = 1 # Expiry 열에 1이라고 표시

5  df[5: 101   # df 테이블 일부를 표시해서 데이터 확인

Spot Front Second Expiry
Date

2017-12-20 5802 58.09    58.13    NaN
2017-12-19 57.46 57.46    57.56     1.0
2017-12-18 57.16 57.16    57.22    NaN
2017-12-15 57.30 57.30          57.33          NaN
2017-12-14 57.04 57.04        57.08        NaN

최종거래일이 1.02 = 표시되어 있음을 확인할 수 있습니다.

손익 계산: 현물에 투자했을 경우

ENS 현재가격에서 매수가격을 빼서 계산할 수 있습니다. 우리는 2010년의 Al 거래일인
2010 1월 4일에 서부 텍사스 중질유를 매수하고, 지금 시점에서 손익을 계산합니다. 따라
서 현재가격에서 2010년 1월 4일 가격을 빼주면 됩니다.

현물은 만기라는 개념 없이 팔지 않으면 계속 들고 가는 상품이므로 단순하게 (현재가 - 매입가)
로 계산합니다.

1 # 현물에 투자했다면             ce)

2 / 손익 = 현재가격 - 초기가격 MK ~

3  price_now = float(df['2017-12-28' ]['Spot’])      SS 현재가격
4 price_before = Sh erie eee ae     # HS 최초가격
5 profit = (price_now - price_before) * 1000

6 print('#2| (현재가격 - 초기가격) : ', ‘{:,.2F}'.format(profit))

Out 손익 (현재가격 - 초기가격) : -21,670.00

226 3부 선물


===== PAGE 227 =====
손익 계산: 선물에 투자했을 경우

서부 텍사스 중질유 ASS 매달 만기가 있으므로 매달 롤오버를 합니다. 이때마다 발생하는
롤오버 비용이 손익에 반영되어야 합니다. 롤오버 비용은 최근월물을 팔고 차근월물을 매입하
는 가격이므로 560000 값을 지불하고 Front ZS 받는 계산, S Second-FrontS 해줍니다.

# 선물에 투자했다면
# 현재가격 - 초기가격 - 롤오버 비용
「011_.046「_005【_800 = 0” # 롤오버 비용 누적값 초기화
for 0 in df.index: # df 일자별로 순환하며
if (df.loc{d].Expiry = 1):  ＊ 최종거래일이면 롤오버 계산 시작
# 롤오버 비용 = 차근월울 가격 - 최근월울 가격
roll_over_cost = df.loc[d].Second - df.loc{d].Front # 롤오버 비용

roll_over_cost_acc = roll_over_cost_acc + roll_over_cost # 누적값

2 니 DN fF WN PB

9
10 print(' a 롤오버 ne:       4 Se  =formetrollig over_cost_acc))

Out   a 기 비용 : : 40.68

이제 롤오버 비용 누적값을 반영해서 서부 텍사스 중질유 선물 ENS 계산해봅니다.

price_now = float(df['2017-12-28']['Front']) # 선물 현재가
price_before = float(df['2010-01-04'][‘Front']) # AS 2/27}
profit = (price_now - price_before - roll_over_cost_acc) * 1000 # AS 현재가-선물 최초
가 - 롤오버 HS 누적값
4  Brine’   Vial eu, 5  me ; dy  sfocmat (profit):

Out  ar 손익 -62,350.00

현물에 투자했을 때보다 선물에 투자했을 때 더 큰 손해가 났습니다. 선물은 레버리지 효과,
차익거래, 헤지 효과 등 다양한 장점이 많은 상품이지만 장기간 보유하면 현물보다 더 큰 손해
를 입을 수 있습니다. 그래서 선물에 투자할 때는 현물보다 더 신중하게 투자해야 합니다.

지금까지 선물의 개념과 금융 이론을 공부하고, 엑셀 실습을 통해 SHR 이론을 느껴보고, 파

이썬을 이용해 모델링을 해보았습니다. 수고 많으셨습니다.

11장 금융공학 모델링 227


===== PAGE 228 =====
블롬체인 vs. 암호화페

앞에서 블록체인은 소수가 정보를 독점하는 불균형을 해소하고, 기존 금융산업에 지불
하던 수수료를 획기적으로 줄여주는 새로운 네트워크라고 소개했습니다. 그런 차원에
A 지금의 암호화폐거래소는 기형적입니다. 암호화폐 거래에는 실제 거래소와 예탁결
제원이라는 존재가 없음에도 암호화폐거래소 단독으로 너무나 높은 수수료를 챙기고
있는 현실입니다. 암호화폐 거래 수수료가 주식 거래 수수료보다 훨씬 높습니다. 비단
수수료만이 문제가 아닙니다. 가끔 발생하는 암호화폐거래소 해킹 사건, 암호화폐 시
세 조종 등 암호화폐를 둘러싼 의혹이 끊이지 않습니다.

비트코인 확산에 아주 큰 기여를 한 '실크로드라는 온라인 상거래 사이트가 있습니다.
마약, 무기 등 불법 거래에 야용되던 사이트인데 자금 추적을 피하기 위해 비트코인을
결제에 이용하면서 이슈가 됐죠. 물론 AALS! 폐쇄 이후에도 비트코인은 활발하게
쓰이고 있기는 합니다. 20164 여름, 우리나라 주요 금융회사 웹사이트를 공격한 해커
는 비트코인을 요구하며 응하지 않으면 재공격을 하겠다고 협박하기도 했죠. 비트코인
의 익명성은 이렇게 범죄, 자금 세탁, 탈세 등에 요긴하게 활용됩니다.

주식은 거래소뿐 아니라 금융감독원, 정부 등 공적인 기관에서 관리해 큰 잡음 없이 거
래되지만, 암호화폐는 정식 금융 거래가 아니기 때문에 이를 관리할 주체가 없을뿐더
러 블록체인이라는 사상 자체가 중앙집중적 관리와 맞지 않아 계속 문제가 벌어지고
있습니다. 암호화폐의 이런 부작용이 무정부 상태의 규제 없는 금융이 얼마나 위험할
수 있는지를 잘 보여주고 있습니다.

정부 등 기득권 세력과 기술 기반의 혁신주의자의 대결 구도로 비추어지는 비트코인
에 대한 논란은 지금도 끊이지 않고 있습니다. 2018년 1월 ]186에서는 이를 주제로
유시민 작가 대 김진화 대표의 BES 진행했습니다. 비트코인을 비판하는 입장의 유
시민 작가는 비트코인이 경제적 가치가 없다는 사실에 기반해 논리를 펼쳐갔고, 비트
코인 옹호론자인 김진화 대표는 4차 산업혁명 시대에 블록체인 기술을 성장시키기 위
해 비트코인을 육성해야 한다고 주장했습니다. 아쉽게도 두 주장 다 허점을 보여주었
습니다. 유시민 작가의 주장대로라면 경제적 가치가 없는 신용파산스압(01275, 0601

228 3부 선물


===== PAGE 229 =====
default 5\30)과 같은 상품 역시 금융상품으로 인정받기 힘듭니다. 김진화 대표의 블
록체인 기술 육성을 위해 비트코인 활성화가 필요하다는 주장은 허점을 논하기 전에
근거가 없습니다. 비트코인 거래소들이 번 돈이 블록체인 기술 개발에 사용된다는 A
결 그리는 어디에도 없으며, 비트코인은 블록체인을 이용한 하나의 상품일 뿐 비트코

인이 블록체인은 아니니까요.

비트코인을 둘

Ee

싼 잡음은 비단 우리나라만은 일은 아닙니다. 미국 정부는 실크로드
창업자를 종신형에 처하고 비트코인을 몰수해서 경매에 부쳤습니다. 그런데 비트코인
옹호자들은 비트코인이 악용되었다는 사실보다는 정부가 비트코인을 경매에 부쳤다는
사실에 더 주목했습니다. 정부가 비트코인의 가치를 인정했고 시세를 만들어줬다고 생
각한 것입니다. 한때 블록체인을 육성하겠다고 국가적으로 비트코인 거래를 권장했던
일본 역시 지금은 분위기가 달라졌습니다. 2017년까지만 해도 도쿄 시내 곳곳에 비트
코인으로 결제할 수 있는 상점들이 즐비했지만, 비트코인 거래소 해킹 사건 등으로 비
트코인에 대한 신뢰가 떨어지고 비트코인 가격 변동성이 높아지자 상점들이 자발적으

로 비트코인 결제를 거부하기 시작했습니다.

중요한 점은 블록체인과 암호화폐를 혼돈하지 말아야 한다는 것입니다. 블록체인 기
So 그 자체로 효용 가치가 충분하고 세상을 바꿀 정도의 파급효과를 지니고 있습니
다. 블록체인 기술에 대해 관심을 갖고 연구 개발에 힘써야 하는 것은 우리의 과제이지
만, 그렇다고 꼭 비트코인을 활성화해야 하는 것은 아닙니다. 비트코인에 들어간 자금
이 블록체인 연구에 쓰인다는 증거도 없습니다. 주식을 사면 해당 회사에 투자하는 것
이지만, 비트코인을 산다고 해도 블록체인에 투자하는 것은 아니라는 뜻입니다. 금융
HITE 전혀 모르면서 비트코인에 투자하는 친구들에게 종종 듣는 질문 중 하나는 리
플이 비트코인보다 기술적으로 뛰어나다는데 리플에 투자해야 하느냐는 것입니다. 암
호화폐끼리의 비교에 대한 질문이지요. 리플이 기술적으로 뛰어나다 한들 리플 소유자
에게 무슨 도움이 될까요? 비트코인 가격이 오르고 리플 가격이 오르는 것은 단지 다
= 사람이 그 코인을 더 높은 가격에 사주기 때문이지 코인이 소유자에게 배당이나 다

른 가치를 주지 않습니다.

기득권 세력으로 분류되는 거래소를 비롯한 금융기관은 블록체인 기술을 수용하면

11장 금융공학 모델링 299



===== PAGE 230 =====
서도 관리 기능을 유지할 수 있는 중도형 블록체인인 프라이빗 블록체인(ㅁㅁ\8ㄷ
blockchain)o] 많은 관심을 두고 있습니다. 프라이빗 블록체인은 데이터를 분산시킨
다는 차원에서 기존의 퍼블릭 블록체인(6413110 blockchain)} 같지만, 정보의 분산
범위와 조회 권한을 통제할 수 있도록 만들어지기 때문에 블록체인이라도 관리가 가능
하다는 장점이 있습니다. SRE 아니라 물류, 제조 등 산업 곳곳에서 적극적으로 연구
하는 기술은 대부분 프라이빗 블록체인인데, 자본을 들여 기술을 개발하는 주체는 항
상 그 기술을 소유하고 관리하길 원하기 때문입니다. 해외 거래소나 예탁결제원, 중앙
은행과 같은 금융기관은 프라이빗 블록체인 도입을 위한 프로젝트를 추진하며 적극적
으로 대응하고 있고, 글로벌 은행들은 자체적으로 또는 몇몇 은행이 연합해 국가 간 자

금 이체에 프라이빗 블록체인을 도입하는 프로젝트를 추진하고 있습니다.

rl

|

한국블록체인협회 진대제 회장의 언론 인터뷰를 소개하며 글

tuo

마무리하겠습니다.

“암호화폐와 블록체인이 건전하게 성장하는 생태계를 만들고자 한다. 먼저 투자자의 이
NS 증진시킬 필요가 있다. 코인을 발행하는 사람, 채굴하는 사람, 이를 사용하거나 거
래하는 사람들이 어떤 연관성을 갖고 움직이는지를 알게 해줘야 한다. 현재 이 구성원
들은 거의 연관성이 없다. 즉 코인 거래 수수료는 블록체인 기술과 무관한 거래소가 가
져간다. 암호화폐 발행처는 알고리즘 기반으로 새 코인을 만들 뿐 책임이 없다. 암호화
폐를 발행한 재단이 암호화폐공개(10ㅇ)를 하는 것과 이를 토대로 블록체인 기업이 태
동할 것이라는 건 막연한 기대에 불과하다. 실제 벌어진 상황이 아니므로 앞으로 그 코
인 위에서 기술력을 갖춘 회사가 성장할 것이라 믿는 건 무모하다. 회원사의 협조를 통해
이런 부분을 알려 나갈 계획이다. 그렇게 되면 좋은 스타트업은 더욱 성장하게 될 것이
다. (…) 지금은 ICOS 하거나 거래소를 운영하는 곳만 ES 번다. 투자자들이 보상받
는 건 거래 가격이 상승했을 때 가능하다. 앞으로는 투자자가 어떤 코인을 투자할지 사
전에 판단할 수 있게 하고 투자처에서 성공을 거두면 수익을 보장받을 수 있게 해야 한

다. 충분히 가능하다.” (「주간조선, 2496호)

230 3부 선물



===== PAGE 231 =====


===== PAGE 232 =====
Chapter 12 옵션 거래의 개념
Chapter 13 옵션 엑셀 실습
Chapter 14 코딩 기술: 시각화

Chapter 15 금융공학 모델링



===== PAGE 233 =====
Chapter 12

옵션 거래의 개념

대부분으  a 책은 주로 옵션을 다룹니다. 주식과 선물은 너무 쉬워서 다루지 않고, 구조
화 상품은 너무 복잡해 다루기 어렵기 때문입니다. 옵션만으로도 내용이 방대하고, 이해가 쉽
지 않아 이재  넘는 두꺼운 금융공학 책들도 옵션만 전적으로 다루기도 합니다. 옵션가격을
추정하는 방법만 해도 가장 대표적인 블랙-슬즈 모형을 비롯해 유한차분법. 몬테카를로 시뮬
레이션 등 다양한 방법이 있고 하나하나가 이해하기 수월하지 않아 전달해야 할 내용이 많기
문입니다.
이 책에서는 먼저 옵션의 기본 개념을 소개한 후, 옵션의 기본이면서도 가장 중요한 이론인
랙-슬즈 방정식을 이용해 옵션가격을 계산하고, 블랙-솔즈 방정식을 기반으로 도출되는 그
릭스를 살펴봅니다.

브
=

12.1 권리에 대한 계약

금융공학 전문가가 아닌 일반 투자자가 가장 이해하기 어려워하는 금융상품이 옵션입니다.
그 이유는 주식이나 선물과는 달리 ASS 대상으로 거래하는 것이 아니라 금융상품을 거래할-
'권리"를 거래하는 것이기 때문입니다. 옵션은 약간의 돈을 내고 주식 매매를 예약해두었다는
뜻입니다.

먼저 현물, 선물, 옵션의 개념을 간단한 예를 가지고 이해해봅시다. 현물거래는 편의점에서

12장 옵션 거래의 개념 233


===== PAGE 234 =====
돈을 내고 상품을 구매하는 것처럼 우리 일상에서 일어나는 대부분의 상거래로, 현재 시점에
물건을 사고파는 행위입니다.

선물거래를 이해하기 위해서 부동산 거래를 떠올려봅시다. 아파트를 매수하기 위해 부동산에
서 1월에 매도자와 계약을 하고 계약금 10%를 지불한 후, 잔금일인 3월에 남은 잔금 90%를
치르고 등기 이전을 하면 드디어 아파트가 내 것이 됩니다. 이 거래는 아파트를 기초자산으로
1월에 선물 매매를 하고 만기인 3월에 실물을 인수받는 부동산이 선물거래입니다.

옵션거래를 이해하기 위해서 크리스마스 파터를 위해 예약금 10만 원을 내고 레스토랑을 예
약하는 행위를 생각해봅시다. 예약자가 지불한 10만 원은 레스토랑의 사용 권리를 사기 위한
대가이며, 예약자가 사정이 생겨 파티를 할 수 없게 된다면 10만 원을 포기하고 예약을 취소

수 있습니다. 하지만 레스토랑은 예약금을 받았기 때문에 크리스마스에 레스토랑을 예약자
에게 제공할 의무를 지게 됩니다. 이 거래는 매수자는 예약자, 매도자는 레스토랑, 기초자산
은 레스토랑 사용권, 만기는 크리스마스가 되는 옵션거래입니다.

세 계약에서 수반되는 의무관계만 뽑아서 보면 각각의 특징을 더 잘 파악할 수 있습니다. 현물
거래는 현재 시점에 모든 거래가 끝나기 때문에 매수자나 매도자에게 남은 의무 같은 개념이
없습니다. 하지만 선물거래는 계약 시점과 잔금 시점이 다른 만큼 잔금 시점까지 실제 거래를
이행해야 하는 약속이 생기며, 매수자와 매도자 모두 계약을 이행할 의무가 있습니다. 반면 옵
션거래인 레스토랑 예약은 손님(매수자)이 일방적으로 예약 취소가 가능하고, 예약 취소 시 예
약금만 포기하면 됩니다.

주식과 선물, 옵션 상품의 특징을 간단히 정리해보겠습니다.

사프
=

온셔
금선

가격              현재 가격              현재 가격              합의한 가격 (행사가)
이행 시기      지금            미래            미래
개념              매매                   계약                  예약
매수자: ㅇ             매수자: ×
의무            해당 없음                                  ag
매도자: ㅇ             매도자: ㅇ

옵션에서 합의한 가격은 아래 옵션 전광판에서 보이는 여러 가격대의 옵션 중에서 선택한 행
사가를 의미합니다.

234 4부 옵션



===== PAGE 235 =====
_ 지수 현재가 전일비   AHS       증목명      현재가    대비    등락을   ARS wWOAA sass 미결증감 ^
코스피200  | 32329, ㅜ 372      101.936 || 코스피200『 201803    323,50 ?    4.40      -1.34    323.737      +0.21      265,055      +749
코스피 | 2491.75: ¥ 33,64     442.349 || A200 F 201806    324.65 ¥   4.15     -1.26      694     +13      19.728       -43v
[그미니션물옵션          만기휠  (coro Oey   vo                                                       읍션항목 Jif     ¥     즈의
[=                        #384                               A         (-뻐:                          풋 옵션                          ㅣ
AMS     Iv      세타     델타    려월대비.   현재가 ㅣ 행사가 |(판산지수) 현재가 -전일대비    델타     세타      Vv     ARS
i       1    50,98 |       0        0               0.01| 377.50 | (2.909,57) |    50.40        0 -1,0000 +0017!        0        0
3   49.03      0      0    0.01| 375.00 | (2890.30) |   5155 a 470 -1,0000  *0.0169      0     141
2     4702         0         0         0      0.01| 372.50 | (2.871.03) |     45.40         0  -1.0090 -00168         0         0
1     45.00        0         0         0      0,01 | 370.00 | (2.851,77)      42.90         0 -1,0000 -0,0167        0        0
1     42.95        0         0         0      0.01} 367.50 | (2,832,50) |    40,40         0 -1,0000 +0,0166        0        0
105   40.88       0       0       0     0.01| 365.00 | (2.013.23) |    3790       0  -1 0000 +0.0165      0       0
111      38.79         0          0          0       0.01| 362.50 | (2 79396) |     35.40          0 -1,0000 +00164         0         0
73    36.67       0       0       0     0,01 | 360.00 | (2774.69) |    36.65 ㅅ 39  -1.0000 -00163    53.64      14
1.503      34.52          0          0          0       0.01| 357.50 | (2.755.42) |     30.45          0. -1.0000 -+0.0162          0          0
8.238     32.35        0        0        0      0.01 | 355,00 | (2,736.15)     27.35        0 -1,0000 -0,0160        0        0
10,568     30.14         0          0          0       0.01} 352.50 | (2716.69) |      7,6          0  -1.0000 +0.0159         0         0
9.054    27.92       0       0       0     0.01| 350.00 | (2.697.62)    26.25 a 3,75 -1,0000 ㆍ0.0158      0      %
24.177    25.65       0        ov 001      0.01 | 347,50 | (2.678.35) |    360 42 3.35  -1.0000 ㆍ0.0157       0       10
50.540     23,34         0         ov 002      0.01 | 345,00 | (2,659.08) |     21.00 42 33 -1,0000 -0015%        0       109
95.593    22.69       0       ov 003     0.02] 342,50  (2.63981) |    1910 4 335 -1,0000, -+0.0155       0     289
162.271     21,20 -0.0002 +0.000!1 v 006      0,03} 340,00 | (2.620,54) |     16.65 a2 395 -0.9999 +0015!     15.56      473
232.387    1989 -0.0015 +0.0008 v O14     0.05} 337.50 | (2,601.27)     1440 4 410, -0.9992) +00137    26.70    5.487
384.847    18,32 -0.0074 -0.0046 v 0350    0,08} 335,00 | (2582.00) |   11.95 42 400  -0.9954 00078   24.07    1562
368,098    17,58 -0.0268 +00200 v 055     0,17} 332,50 | (2.562. 74) |     940 42 367 -09600 -00118    19.25    2.222
422.624     16,64 -0.0723 +0.0673 ¥ 1,00      0.34] 330,00 | (2543.47)      7.21 4 339 -09327 -0.0573     19,52     9.157
377,941     15.70 -0.1436 +0.1749' ㅜㅠ 1.68      0.67] 327.50 | (2,524.20) |     502 4 259 -08251) -01288     17,62    22.559
263,361     15,15 -0.2091    0.3559 Vo 245      1,33} 325.00 | (2504.93)      320 4 18 -06441 -01945     16,84    62.981
134,570,    15.41, -0.2224 +0,5795;¥ 3.07      253] 322,50 | (2.485, 66) |     188 a2 115 -04205 -02078     16.90 193.215
18,669, 15,58 -01729 0.7809 ㅜㅠ 357 4.18| 320,00 | (2.466.39)| 1045 A 06S = -0.2191 -0.15865 17.45 336,524

12.2 옵션의 가치
증권사 직원 ㅅ는 1년 후

Ar
좋은 레스토랑을 10만 원을 내고

약해두었습니다

연히 예약한 날짜가 서울세계불꽃축제일로 결정되었습니다. 여의도 주변 음식점에는 좋은
ㆍ. 직원 A7} 예약해둔 레스토랑 주인은 RES 붙여 장사할 수 있는 대박 기회를 놓
처버렸습니다. 반면 예약자 ㅅ는 이벤트를 준비하는 누군가에게 RES 받고 예약을 넘길 수
도 있겠습니다. 옵션의 가격이 올라간 것입니다.
불꽃 축제 행사 계획이 나왔습니다. 레스토랑 건물 앞쪽으로 불꽃 축제 행사 무대가 설치되는

데, 레스토랑 창문을 다 가리도록 설계되었다고 합니다. 불꽃놀이 인파 때문에 길만 막히고 불
꽃놀이는 즐기지도 못하는 상황이 된 것이지요. 게다가 애초에 생각했던 한강 전망조차 즐기
지 못하게 되었네요. 옵션가격이 급락했습니다.

그러던 중 ㅅ가 회사에서 해외 지사 발령을 받게 되었습니다. 그런데 발령일이 결혼식 날짜 이
전이군요. 결혼식을 앞당겨야겠습니다. 결국 옵션을 행사하지 못하게 되어버렸습니다.

12장 옵션 거래의 개념 235


===== PAGE 236 =====
시간이 지나면 가능성은 사라진다: 시간가치

레스토랑을 1년 전에 예약하다 보니 1년이라는 긴 시간 동안 여러 가지 Yo] 예약의 가치를
변동시키고 있습니다. 계약(예약)일로부터 만기(행사)일까지 기간이 길수록 계약의 가치를 변
동시킬 수 있는 사건이 발생할 가능성이 높습니다. 그리고 시간이 갈수록 이러한 가능성은 줄
어들지요. 옵션가격이 점프할 수 있는 가능성의 시간, 이것이 바로 옵션에서 얘기하는 시간가
치입니다. 당연히 시간가치는 시간이 지날수록 줄어들고, 만기가 되면 사라집니다.

ITM, ATM, OTM: 내재가치

내재가치는 시간가치와 대비되는 개념으로, 지금 현재가 만기라고 가정하면 옵션의 가치가 얼
마나 되는지를 따지는 것입니다. 가능성의 가치를 쪽 빼고 팩트만 보는 것이지요. 최초 예약을
했을 때는 10만 원의 가치가 있는 예약을 10만 원을 내고 확보했으니 내재가치는 0원이 됩니
다. 불꽃 축제 행사가 결정되었을 때는 예약의 가치가 10만 원보다 올라가기 때문에 내재가치
는 플러스(+)로 올라갑니다. 반대로 행사 무대 설치가 결정되었을 때에는 내재가치가 마이너
스(- )로 내려가게 됩니다.

내재가치가 0인 시점을 옵션 용어로는 등가격(4734, 41 the 2010ㅁ6\)이라고 부르고, 기초자
산의 가격이 권리 행사 가격이랑 같다고 이해합니다. 내재가치가 플러스(+)인 경우는 내가격
(ITM, in the money)°]#}3! 하는데, 기초자산의 가격이 권리 행사 구간 내에 있다는 뜻입니
다. 반대로 내재가치가 마이너스( - )인 경우는 2|7}4 (OTM, out of the 2ㅁ0ㅁ6\)인데, 기초
자산의 가격이 권리 행사 구간 밖에 있다는 뜻입니다.

옵션의 가치: 내재가치 + 시간가치
옵션의 값은 내재가치와 시간가치를 합한 값입니다. 다음 옵션가격 그래프로 이해해보겠습
니다.

236 4부옵션


===== PAGE 237 =====
| 옵션가격 |
3011 내재가치 |

~
20                 OTM                              22

BE 471A (Call Price)

300                 310                                        330                                        350
7|2%t4t(Underlying)

위 그래프는 행사가 330인 KOSPI200 콜옵션가격 곡선입니다. 행사가격(행사가)이 330인
SSS 지수가 330보다 높으면 가치가 있는 옵션, 330과 같거나 낮으면 가치가 없는 옵션
이 이비 예를 들어 만기 시 지수가 340이라고 하면, 매수자는 권리를 행사해서 340짜리를
330에 살 수 있게 되어 계약당 10만큼의 이익을 얻습니다. 여기서 말하는 가치(이익)가 바로
내재가치입니다.

그래프에서 붉은색 AS 옵션의 가격, 파란색은 내재가치입니다. 행사가가 330이므로 330보
다 오른쪽은 플러스, 즉 내가격 구간이고, 왼쪽은 마이너스, 즉 외가격 구간입니다. 파란색 A
으로 표시된 330는 등가격인 ATMO] 됩니다. 그래프에서 보듯이 등가격과 외가격 구간에는
내재가치가 없습니다.

내재가치가 없는 구간이라도 옵션가격은 0이 아닌데, 이유는 남은 시간 동안 시장 상황이 변
동해서 가격이 올라갈 가능성이 있고, 옵션 투자자들은 이 가능성에 가치를 부여하기 때문입
니다. 이것이 바로 시간가치입니다. 위 그래프에서 빨간색 그래프와 파란색 그래프 사이가 시
간가치 부분입니다.

12장 옵션 거래의 개념 237


===== PAGE 238 =====
12.3 변동성

시장 상황의 변동으로 인한 가능성의 크기를 옵션에서는 변동성(ㅠ012041165)이라고 부르는데,
옵션가격 결정에 아주 중요한 SAS 합니다. 변동성이 커지면, 즉 가능성이 높아지면 시간가
치(다음 그래프의 초록색 영역)가 커져서 옵션가격이 올라가기 때문입니다.

다음은 다른 조건은 모두 동일하고 변동성만 10%와 30%로 차이가 날 때의 옵션가격 그래프
입니다. 변동성이 높아질 때 옵션가격이 확 올라가는데, 그 차이가 모두 시간가치의 변화에 기
인한 것임을 확인할 수 있습니다.

콜옵션 가격

$

N
“

8

~
uw

콜옵션 가격 (Call Price)

그
ㅇ

200                                                                                340
기초자산 가격 (Underlying)

앞의 그래프에서 보듯 변동성이 10%일 때 등가격 옵션가격은 8(기초자산 가격(※×값)이 330일
때 빨간 그래프의 ?값) 정도입니다.

238 4부 옵션


===== PAGE 239 =====
콜옵션 가격

ㅎ

w
uw

$

nN

8

=

몰옵션 7+4 (Call Price)

10

320
기초자산 가격 (Underlying)

fu

변동성이 30%로 올라가니 등가격 옵션가격은 22.5로 많이 올라갔네요. 변동성 상승에 따른
시간가치의 증가를 확인할 수 있는 부분입니다.

12.4 옵션의 특징: 3 vs.

옵션에는 현물과 선물에는 없는 콜옵션과 풋옵션이라는 구분이 있습니다. 콜은 만기 시 살 수
있는 권리, 풋은 만기 시 팔 수 있는 BIS 말합니다. 이는 옵션이 현물이나 선물보다 복잡하
Al 보이는 이유 중 하나인데, 현 시점의 포지션은 매도/매수, 만기 시점의 포지션은 콜/풋으로
구분해서 콜 매수(1008 call), 콜 매도(6110ㅁ call), 풋 매수(1008 put), 풋 매도(510ㅁ put)
의 총 4포지션이 만들어집니다.

옵션 매수 포지션

을 매수한 포지션(콜 매수, 풋 매수)은 프리미엄을 지불하고 옵션(권리)를 구매한 측입니
다. 따라서 유리한 경우에는 권리를 행사하고 불리할 경우에는 권리를 포기할 수 있습니다. 콜
매수는 싸게 살 권리이기 때문에 현물가격이 행사가를 초과할 경우 수익이 발생하고, 풋 매수
는 비싸게 팔 권리이므로 현물가격이 행사가보다 낮을 때 수익이 발생합니다.

12장 옵션 거래의 개념 239


===== PAGE 240 =====
행사가가 315인 KOSPI200 옵션의 4개 포지션 각각의 그래프를 보겠습니다. 모든 그래프에
서 XS 현물가격을, YSS ENS 나타내며, 옵션 프리미엄은 3이라고 가정합니다.

콜 매수 (Call Long)
124
104
87
67
or
q 44
27
07
-24
300       305       310       315       320       325       330
KOSPI200

행사가에 살 권리를 매수한 것입니다. 앞의 그래프에서 현물가격이 325인 경우에도 = 매수
자는 315에 살 권리가 있어 계약당 10의 이익이 발생하며, 프리미엄 3을 차감하면 이익은 7입
니다.                                                                                  오기

풋 매수 (Put Long)

300          305          310          315          320          325          330
KOSPI200

행사가에 팔 권리를 매수한 것입니다. 앞의 그래프에서 현물가격이 305인 경우에도 풋 매수

때

240 4부 옵션



===== PAGE 241 =====
자는 315에 팔 권리가 있어 계약당 10의 이익이 발생하며, 프리미엄 3을 차감하면 이익은 7입
니다.

옵션 매도 포지션
반대로 매도 포지션(콜 매도, 풋 매도)은 프리미엄을 받고 옵션(권리)를 판매한 입장이기에 권
리를 보유한 매수자가 요구할 경우 의무를 이행해야만 합니다. 매수 포지션과는 반대로 권리
는 없고 의무에 대한 책임만 있기 때문에 엄청난 위혐을 감수해야 하는 포지션입니다. 콜 매도
는 싸게 팔 의무이기 때문에 현물가격이 행사가를 초과할 경우 손해가 발생하고, 풋 매도는 비
싸게 살 의무이므로 현물가격이 행사가보다 낮을 때 손해가 발생합니다.
그러면 왜 권리는 없고 의무만 있는 매도 포지션을 잡으려 할까요? 그 이유는 바로 프리미엄
수익 때문입니다. 옵션을 매매할 때 매수자는 매도자에게 프리미엄을 지불하게 되는데, 매도
포지션을 취하는 측은 이 프리미엄으로 안정적인 수익을 올리기 위해 혹시나 발생할지 모르는
위험을 감수하는 것입니다. 옵션 매도자가 엄청난 손실을 당하는 경우는 자주 일어나지 않기
문입니다. 한 계약에 천 원씩 받지만 당첨자에게는 큰 돈을 지불하는 복권 발행자를 생각하
면 이해하는 데 도움이 될 것입니다. 복권 당첨자에게 어마어마한 당첨금을 지불하지만 하나
에 천 원씩 받는 복권 판매 수입이 훨씬 크다는 사실, 알고 계시죠?

콜 Oh (Call Short)

27

0;

-24

or -44
uy

-87

-10/

-124

300       305       310        315        320        325       330
KOSPI200

행사가에 살 의무를 매도한 것입니다. 앞의 그래프에서 현물가격이 325인 경우에도 콜 매도

12장 옵션 거래의 개념 241


===== PAGE 242 =====
자는 315에 팔 의무가 있어 계약당 10의 손해가 발생하며, 프리미엄 3을 더하면 손해는 7입니
다. 하지만 현물가격이 318 미만인 전 구간에서는 프리미엄 이익을 얻습니다.

풋 매도 (Put Short)

300              305              310              315              320              325              330
KOSPI200

행사가에 팔 의무를 매도한 것입니다. 앞의 그래프에서 현물가격이 305인 경우에도 풋 매도
자는 315에 살 의무가 있어 계약당 10의 손해가 발생하며, 프리미엄 3을 더하면 손해는 7입니
다. 하지만 현물가격이 312 초과인 전 구간에서는 프리미엄 이익을 얻습니다.

eee

12.5 다양한 옵션 상품

다양한 가격
앞에서 잠깐 소개한 옵션 전광판을 떠올려봅시다. 선물은 상품 종류벌로 한 개의 상품만

Qh
지만, 옵션은 같은 종류의 상품이라도 행사가별로 상품이 다양하게 있습니다. 다음 전광판은
2018년 2월 만기인 KOSPI1200 옵션 상품의 메뉴판 일부를 캡처한 것입니다.

ㅎㅇ)

242 4부 옵션



===== PAGE 243 =====
SADE (환산지수) 현재가
377.50  (2.909.57) |  50.40
375.00  (2.090.30) |  51.55
372.50  (2.071.03) | 45,40
370,00 (2851.77), 42,90
367.50 (2.832,50)| 40,40
365,00 (2.813,23)| 37,90
362.50 (2,793.96) | 35.40
360,00 (2,774.69) 36.85
357.50 (2.755,42)| 30,45
355,00  (2.736.15) 27,95

352.50 (2716,89)| 7.05
350,00 (2697.62) 26,25
347.50 (2678.35) 23,60
345.00 (2.659,08) 21,00
342,50 (2.633.81)| 19.10
340.00 (2.62054)  16.65

337,50 (2601.27), 14.40
335.00 (2,582.00) 11.95
332,50 (2,562.74) |  9.40
330.00  (2.543.47) .  7.21
327.50 (2,524.20).  5,02
325.00  (2.504.93)   3,20
322.50 (2,485,665) |  1,88
320,00 (2,466.39)   1.04

초자산의 동일한 만기 상품이지만 행사가별로 서로 다
있음을 볼 수 있습니다. KOSPIZ0 BAS 2.5포인트 단위로 상

=                 고
품이 상장되고, 투자자는 다양한 행사가의 옵션 중에서 본인이 원하는 수익 구조(627-00)를

매달 만기

앞에서 같은 달이라도 행사가에 따라 수없이 많은 상품이 있다는 것을 보았습니다만 그걸로
Bo] 아닙니다. 옵션거래는 선택의 So] 더 넓습니다. 한국거래소에서 거래되는 옵션은 매달
(매달 둘째 주 목요일) 만기가 있습니다. 즉, 1, 2, 3월 매달 서로 다른 상품이 있는 것이지요. 분
기별(3, 6. 9, 12월의 둘째 주 목요일)로 상품이 있는 선물보다 훨씬 다양한 상품이 구비되어 있
는 셈입니다.

매달 "개의 행사가격별로, 콜/풋(×2)별로, 12개월(×12)별로 상품이 있으니 옵션 종류별
연간 총 1 ×2×12개의 상품이 거래되는 것입니다. 선물이 분기별로 한 개씩, 연간 총 4개의
상품만 있는 것과 대비되죠.

Hu

123 옵션 거래의 74 243


===== PAGE 244 =====
ELW
선물에서 소개한 $4 (multiplienS 떠올려봅시다. 옵션도 똑같은 개념으로 승수가 있습니
다. KOSPI200 옵션은 승수가 25만 원이고, 미니선물과 같이 승수가 5만 원인 미니옵션도 한

—_ ree

국거래소 파생상품 시장에서 거래되고 이 지수가 316일때 행사가격이
(os latte bak

3159] 콜옵션의 7} 240] 4.73이라고 하면 KOSPI200 SAS 1,182,500 A (=4.73 x 250,000),
미니옵션은 236.500원(=4.73×50.000)이 됩니다.

미니옵션의 개념에서 한 발짝 더 나아가 소매용 옵션상품인 ELW (equity linked \80800)라
는 것이 있는데요, 미니옵션보다 승수를 더 낮게 책정해서 100원대로 단가를 맞춰놓은 옵션입
니다. KOSPI200 ㅁ81\라면 승수를 100으로 해서 옵션가격이 473원(=4.73 x 100)이 되는 것
입니다. ELW 소매용 상품이기에 소비자를 위한 안전장치를 추가해두었는데요, 바로 매수
포지션만 가능하다는 것입니다. ELW 시장에서 투자자는 콜 매수, 풋 매수의 두 가지 포지션
만 취할 수 있고, 매도는 기관인 12 (liquidity provider)7} 전담합니다.

미국형 옵션, 이색 옵션

지금까지 소개한 옵션은 단순한 구조의 유럽형 옵션입니다. 유럽형 옵션과 대비되는 개념의
ol (exotic) 옵션들이 있는데요, 이색 옵션들은 수익 구조가 복잡합니다. 살짝 alzra 수 있
으니 단순한 옵션이 아직 깔끔하게 이해가 되지 않았다면 읽지 말고 넘어가시기를 추천합니
다.

039 (American) 옵션은 만기 전 아무 때나 권리를 행사할 수 있습니다. 유럼형 옵션이 만
기 시에만 권리 행사가 가능한 것과 대비되지요. 따라서 미국형 옵션의 소유자는 더 많은 권리
를 소유하고 있는 셈이니 당연히 옵션가격은 더 높게 산정되어야겠지요.

이색 옵션인 조기 종료형 옵션은 목표 가격을 설정해놓고 만기 전 아무 때라도 기초자산 가격
이 목표 가격에 도달하면 조기에 종료되는 옵션입니다. 0501200 조기 종료 콜옵션(목표가:
330, 행사가: 320, 만기: 2018 12월)을 KOSPI200} 3152 때 구매했다면 2018년 12월 만기
전에 KOSP1200°] 330 이상 올라가면 조기 종료가 되어 330에 권리 행사를 하고, 그렇지 않

으면 2018년 12월에 단순한 옵션처럼 320에 권리 행사가 되는 방식입니다.

244 4부 옵션



===== PAGE 245 =====
12.6 옵션 이론가: 블랙-슬즈 방정식

옵션에 관심이 있는 사람이라면 블랙-솔즈 방정식이라는 맡은 한 번쯤 eS 정도로

랙-솔즈 방정식은 옵션 세계에서 바이블 같은 공식입니다. 블랙-슬즈 방정식을 eae a
정은 꽤 어려운 개념을 이해해야 하므로 쉽지 않지만, 단순히 공식을 사용하기만 하는 것은 어
렵지 않습니다. 우선 공식을 소개합니다.

옵션가격                      C(#)=S,N(d,)- Ke" N(d;)
때 = Ke" N(-d,)-S,N(-d,)

2
Ineo Sr
d, =

oVT
2
In Star S lr
d, =d, -ovT =

So: 기초자산 7}A (stock price at time 0)

K: A}}A (strike price)

T: 잔존만기(연율로 SH} (time to maturity)

r: 이자율(연속복리)(00ㅁㅁㅁ40451\ compounded risk-free rate)

0: 기초자산 49 (volatility)

N(x): 표준정규분포의 누적분포함수(04104120\ㅇ probability distribution for a standard
normal distribution)

복잡해 보이는 공식이지만 한번 프로그래밍을 해놓으면 AAS 컴퓨터가 하기 때문에 사용은
간단함니다. 콜옵션은 wef (기초자산 가격)-(앵사가격)민 |격)만큼의 수익을 얻습니다. 블랙-숄즈
모형에서 콜옵션의 가격인 C=SN(d,)—-Ke"N(d,) 중 N(d,), ^(0, )는 옵션이 행사
될 기댓값을 나타냄니다. 블랙-숄즈 모형에서 앞부분 57“(< )는 '기초자산의 기댓값이고, 뒷
부분 46”//(0,)는   Ke" 가 행사가격의 현재가치이므로 '행사가격의 기댓값의 현재가치.
eo.          —

RGAE BHA 반대의 포지션이므로 만기에 (행사가격-기초자산 가격)만큼의 수익을 4

=   =

ees,

128 옵션 거래의 7S 245


===== PAGE 246 =====
현합니다. 따라서 콜옵션의 가격과 반대로 계산합니다. 위 블랙-숄즈 모형을 보면 co} 『 공
식이 반대로 표현된 것을 알 수 있습니다.

이항 모형, 몬테카를로 시뮬레이션 등 다른 모형은 앞으로 주가가 어떻게 움직일지를 표본에
서 무작위로 선택해 옵션가격을 계산하는 BIS 수백 회 이상 반복(많이 반복할수록 신뢰도가
높음)하는 방식으로 옵션가격을 산출하는 반면, 블랙-솔즈 모형은 주가는 로그 정규분포를 따
른다고 가정하고 한 번에 계산해내기 때문에 계산 속도가 빠르고 컴퓨팅 파워가 적게 소모됩
니다. 블랙-숄즈 모형보다 ARS 조금 떨어지지만 더 다양한 상품에 적용할 수 있는 모형인
유한차분법도 널리 사용되고 있습니다.

12.7 SS 그릭스: 어려워 보이는 옵션 용어
읍션 관련 이론이 복잡하고 모두 외국에서 들어오다 보니 옵션 업계 종사자들 역시 소위 전문
용어를 사용합니다. 가장 대표적인 것은 그릭스(6ㅠ60}65, 그리스 문자)인데 옵션가격을 결정하

a    *

는 각 요인들이 변할 때 옵션가격은 얼마나 변하는지를 나타내는 민감도이며, 옵션 포지션으
위험도를 판단할 때 사용됩니다. 그릭스에 대한 상세한 설명은 옵션을 어렵다고 여기게 할 수
있으므로 간단히 소개만 하도록 하겠습니다. 처음 읽을 때부터 이해하지 않아도 괜찮습니다.

원래 어려운 내용이니까요.

델타(&)는 기초자산 가격(5) 변동 대비 옵션가격의 변동입니다. 델타가 0.5라면 기초자산 가
격이 1% 변동할 때, 옵션가격은 0.5% 변동한다는 것을 의미합니다. 블랙-숄즈 방정식을 sez
편미분해서 구합니다.

mag -|  A(call) = N(d,)
dS |A(put)=N(d,)-1
콜옵션 매수 포지션의 경우 0부터 1 사이의 값으로 나타나는데, 내가격일수록 1에 가깝고 외
가격일수록 0에 가까운 값을 갖습니다. 다시 말해, 행사 가능성이 높을수록 기초자산 가격 변
동과 비슷한 만큼 옵선가격이 움직이고, 행사 가능성이 낮을수록 기초자산 가격 변동에 비해
옵션가격 변동은 둔감하다는 뜻이지요.

246 4부 옵션



===== PAGE 247 =====
- ~”

콜옵션의 델타

=                     <
^.

0.6000

0.4000    SY

를 ㅡ^
SSRBLSBSRBLSSRABLG
ESE Ce Oc 은 은 도 일 a 월 5 중
이 예 05 05 05 05 02 02 02 002 02 02 MYM 02 02 02

행사가가 315인 KOSPI200 옵션의 기초자산 가격이 315일 경우(등

입니다. KOSPI1200 지수가 1만큼 올라가면, 콜옵션가격이 0.59만큼

감마(1')는 기초자산 가격(5) 변동 대비 델타의 WSS ech 델타를 SB 편미분해서

구합니다.
120 (0()
252 80427
Ni(x)=—e*”
^ 428
등가격 근처에서 가장 큰 값을 가집니다. 행사가격 근처에서는 기초
옴션가격 변화 속도가 더 빠르다는 뜻이지요.

een er 가기짜가 이개

초자산 가격의 변화에 따라

12장 옵션 거래의 개념 247


===== PAGE 248 =====
감마
0.0045
0.0040              ~
           as            NG
0.0020
0.0015     vA                  IN
0.0010 —f—                     SS
0.0005
Bo Sa te ie ENS Se
2SSSsSs5esssRsgss

2h,

세타(6)는 AZT) 경과 대비 옵션가격의 변동운입니다. 블랙-숄즈 방정식을 7로 편미분해
서 구합니다.

22
S,N'(d,)o

aT

다음 그래프에서 보이듯 7가 0에 가까울수록 즉, 만기가 가까워질수록 세타는 가파르게 떨어
집니다.

6(00//)=-                   rKe"" N(d,)

©( put) =-                  +rKe’ N(-d,)

Theta
SEBSSESLSRASRBRLBRL{8RSS

껴 켜 여 켜 여 여 예 져 며 _ㅡ=

0
0
0
0
0
0
0
0
0
0

(10.00)                         i
(20.00)

(30,00)                                                                                                   나
(40.00)

(50.00) -
(60.00)
(70.00)
(80.00)

248 4484



===== PAGE 249 =====
i             (   pe
HHO = 기초자산 변동성(0) 대비 옵션가격의 ASRS UePMUch 블랙-숄즈 방정식을
로 편미분해서 구합니다.

vega = gee S,VTN'(d,)
do

1

727

크래프에서 볼 수 있듯이 변동성이 낮을수록 옵션가격의 민감도가 높습니다.

2
—x°/2
e

N'(x) =

Vega
82.000

81.000

때 < 0 ~

79.000

78.000                                                                2
77.000
76,000
75,000
74,000
73,000

로(6)는 이자율(/) 변동 대비 옵션가격의 변동율을 Ue 블랙-숄즈 방정식을 /로 a
미분해서 구합니다.

oe dC -|  rho(call) = KTe “TN (d,)

=e   rho( put) =—KTe"" N(-d,)

이자율 변동은 자주 일어나는 일이 아니라 실제 트레이딩에서는 거의 사용되지는 않는 지표입
니다. 그래프도 생략하겠습니다.

12장 옵션 거래의 개념 249


===== PAGE 250 =====
13.1 WHS 구현하는 블랙-숄즈 모형

새 엑셀 파일 준비
이번 시간에는 블랙-숄즈 방정식을 이용해 옵션 이론가를 계산하는 과정을 엑셀로 구현해보
ASU 먼저 바탕화면이나 윈도우 메뉴에 있는 엑셀 아이콘을 더블클릭해서 새 파일을 만
듭니다.

작업을 할 시트 이름을 기본값인 ‘Sheet1']4] ‘Option 기본'으로 바꿈니다.

--] _9064400- |
rs 8 프
아라 a  시트 SS (P)_.        5
---           24M           >

1 승기         1
102     숨기기 취소(2).     ]

[         ㅣ 모든 시트 MES)
오그

250 4부옵션



===== PAGE 251 =====
옵션가격 구성요소 세팅
옵션 이론가를 산출하기 위한 사전 준비 작업으로 옵션가격의 구성요소를 세팅합니다. 우선
옵션가격을 어떻게 산출하는지, 그리고 이를 구성하는 RAE 무엇인지 다시 한번 살펴봅니다.

옵션가격
|  C(#)=S,N (d,)- Ke"? N(d,)

P(=) = Ke" N(-d,)—S,N (-d,)

2
in Sb(r4 Sr
d, =

oVT

2
"꽃[/-을 |
d, =d,-oVT =

So: 기초자산 가격

K: 행사가격

T: 잔존만기(연율로 환산)

r: 이자율(연속복리)

0: 기초자산 변동성

N(x): 표준정규분포의 누적분포함수

12.6절에서 봤던 블랙-숄즈 공식입니다. 콜과 HE 모두 동일한 구성요소를 갖고 있네요. 기초
자산 가격(5), 행사가격), BERIT), 무위험이자율), 변동성(0)이 주어져야 옵션가
AS 구할 수 있습니다. 그럼 이 값들을 엑셀 파일에 세팅해봅니다.

때 : [Ix + fe | =neTworKDAYs(B2,€2)/252 | -

B                Cc        eee 비
재일        만기일 | 잔존만2
-@7-@1 | 2019-03-21

A
행사가격

330

연
2018

F
변동성

10.00%

;     E
_ 이자을 」

행사가격은 315, 현재일은 2018년 7월 1일, 만기일은 2019년 3월 21일, 이자율은 2%, 변동
성은 10%을 입력합니다. 잔존만기는 현재일과 만기일 사이의 날짜를 계산해 연율로 환산해

13장 옵션 엑셀실습 251

—


===== PAGE 252 =====
야 합니다. 주말에는 증권시장이 열리지 않으므로 여기에서는 주말을 제외한 252일을 1년으
로 하기로 약속했었지요. 따라서 우리가 해야 할 일은 주말을 제외한 날짜를 세어 252로 나뉘
주면 됩니다. 엑셀에서 주말을 제외한 날짜를 계산할 때는 =NETWORKDAYS (날짜1,날짜2) 함
수를 사용합니다. 따라서 잔존만기가 들어가는 D2 AS 앞의 그림처럼 =NETWORKDAYS (82,
C2) / 2527} 됩니다.

여기까지 해놓고 보니 하나 빠진 것이 있네요. 바로 기초자산 가격입니다. 기초자산 가격이 변
함에 따라 옵션가격이 어떻게 변하는지 알아보기 위해 기초자산 가격은 변동시켜가며 옵션가
격을 계산해보려고 우선 빼놓았죠. 그럼 기초자산 가격을 변동시켜가며 옵션가격을 계산하도
록 나머지 정보를 세팅해봅시다.

^                                      c                  D         |         3                   F
oH                     ^       0             ㆍ       Oo                   .               ()        Oo            HH

4
20
2         330        2018-07-01| 2019-03-21           0.75        2.00%          10.00%
3
4

^4부터 84까지의 셀에 앞의 그림처럼 입력합니다. 현물가격이 변하는 BAS 300544] 3007+
지로 잡기 위하여 AS 셀에 300, AG 셀에 301을 입력합니다. 그리고 360까지 데이터를 채우
기 위해 45, AG AS 함께 선택한 후 오른쪽 하단에 나타나는 포인터 모양이 땐에서 +로 바뀌
면 마우스를 클릭한 상태로 드래그하여 465 셀까지 쪽 끌어내려줍니다. 엑셀의 연속 데이터
채우기 기능을 이용하는 것이죠.                                  2

In —+ ( +     }r

oO

이제 85 셀에 01 수식을 입력할 차례입니다. a, =ㅡ-- 2) ota 자연로그00)는
oO

IN() OS, 제곱(”)은 ^2로, 제곱근(/)은 SORT ( )로 표현합니다. 엑셀 수식으로 나타내면 = (

LN (A5/A$2) + (E$2+F$2°2*0.5)*D$2 ) / ( F$2* SQRT (D$2 ) )입니다.

252 4484



===== PAGE 253 =====
10000 ~ | eae \ fe | =( 네(65/052) + (e$2+F$2°2"@.5)*0S2_) / ( F$2" SORT(OS2) )|
G        H
300/-( LN(AS/AS2) + (ES24F$2%2"0.5)"D$2 ) / ( F$2™ SQRT(DS2) )

6       301

7s       302

in| 순은 2
                       K       2               :
이번에는 C5 셀에 0,를 입력합니다. d, =d,—oNT =       이므로 간단하게
oO

위에서 계산해놓은 0,을 이용합니다. 엑셀 수식으로 나타내면 = 85 - F$2 * 5001 (D$2) U4
다.

10008 ㅋ 1: OK OM fe || - 05 - 『52 = soRT(Ds2) |

내재가치 | 시간가치

01, 0, 입력을 완료했으면 이제 콜옵션 이론가 CH 계산할 차례입니다. C= SN(d,)—
Ke 7/(0,)에서 N(x) 표준정규분포의 누적밀도 함수, 즉 평균이 0이고 표준편차가
1인 표준정규분포의 -ㅇ부터 *까지 누적 분포값을 EH YU ch, 엑셀 수식으로는 NORM.
5.0151( )로 나타내고, 다음 그림과 같이 엑셀 상단의 수식 〉 기타함수 〉 통계 메뉴에서 찾
을 수 있습니다.

13장 옵션 엑셀 실습 253


===== PAGE 254 =====
4.2.1 Option St
이터       토     보기

검
               3 3 이를정의 | 올=잠조되는 쓸 추적 Bsa 표시
= yi pao          MM og BTM      | of 잠조하는 BSN ㆍ 오류 검사
+       .                       | 관리자 [3 선택 영역에서 만들기 Go 연결선 제거 ~   Ge) 수식 계샌
1.5.0157(85, TRUE) - 4921 0 S2Q@ > — norminv         |
a 해 르기 TF2OQ » | NORMS DIST       Ss        :        시
16 S20 >       NORM.S.INV                  =       ;      =H
3        10.00% I =#3Q>     PEARSON       a  a
표주 전그 누전 부포가을 구한니다
WM 20) 0) ㅣ  percentneexc! 평균이 0이고 표준 편자가 1인 정규
| 대재각지 | 지긴기저느               0. | 무포를의미합니다         ^
it                                PERCENTRANKES @ 자세히

이를 엑셀 수식으로 나타내면 = 45 * NORM.S.DIST (BS, TRUE) - A$2 * EXP (-E$2*D$2) *
NORM.S.DIST (C5, TRUE) Uc.

| < SM _ fe | = 45 * norn.s.orst(85, TRUE) - BS2°EXP(-£$2°032)"NORN.S.DIST(C5, TRUE) |

=          |
0.88 1-    @.97 |= AS * NORM

이제 현물가격이 3008 때 콜옵션의 가격을 구했습니다.

콜옵션가격을 구했으니 내재가치도 구해봅시다. 내재가치는 만기 시 옵션 보유자가 얻는 수
익입니다. 다시 말해 우리가 블랙-숄즈 모형을 이용해서 구하는 이론가는 만기 이전에 옵션
을 매매할 때 사용하는 가격이고, 내재가치는 만기 시점에 옵션 보유자가 얻게 되는 수익을 의
미합니다. 만기 시 현물(기초자산)가격이 행사가격보다 높으면 옵션 보유자는 기초자산을 행
사가격에 살 수 있으므로 (현물가격)-(행사가격)만큼의 수익을 얻게 되고, 현물가격이 행사가
격보다 낮으면 옵션 보유자는 권리를 포기하므로 수익은 00] 됩니다. 이를 수식으로 나타내면
Max, 현물가격-행사가격)이 됩니다. 이 식을 85 oll 삽입합니다.

clr

lo

254 4480



===== PAGE 255 =====
-veooxue 0 | KOM fe | 98060. 25-52) | |

c | ㅁ  at F

4) ^

-

내재가치 | 시간가치

id: kes

시간가치는 남은 시간 동안 현물가격이 변동해서 옵션가격이 올라갈 수 있는 가능성의 가치,

=

즉 옵션가격과 내재가치의 차이를 의미합니다. 수식으로 나타내면 간단히 (옵션가격)-(내재

가치)가 됩니다. 다음 그림과 같이 『5 Boll 이 수식을 입력합니다.

세         8    ㅣ    G         D         E    . ope

지금까지 구한 값을 현물가격 변화 범위 전체에 적용할 차례입니다. 연속 데이터 채우기를 st

기 위하여 85부터 『5까지의 셀을 한꺼번에 선택합니다. 선택 범위 오른쪽

점에 마우스를 올려놓고 더블클릭합니다.

아래에 나타나는

| es eee S|   G      H

F52* 5007(052) )

330      2018-07-61 | 2019-03-21

01                         | 내재가치 ㅣ 시간가치

현물가격          [        |
ee} -    0.88 |-    0.97 |     2.58 —        cy    2.58

대      1 | A fe | =( uncassas2y + (€52+F$2°2"0.5)*D$2 ) / (
A   A      Bee     6 수세해제. DE      ies
BAIS || 현재일    만기일 」 잔존만기 ㅣ 이자율    변동송

이제 현물가격 360까지 데이터가 채워진 것을 확인할 수 있습니다. 진도를
라면 865 셀까지 데이터가 채워졌을 것입니다.

잘 따라가는 중이

13장 옵션 엑셀 실습 255


===== PAGE 256 =====
13.2 콜옵션가격 그래프 그리기

이제 현물가격의 변화에 따른 옵션가격의 변화를 그래프로 그려봅니다. 그래프를 그리기 위해
14부터 『65까지 셀 전체를 선택합니다. 우선 sw 선택한 후 (Shit) S 누른 상태에서 [|
키를 두 번 눌러 『4까지 일괄 선택한 후 [01]+[61081+| | |를 누르면 865까지 한 번에 선택
이 됩니다. 앞에서 설명한 엑셀의 [Shirt], [00] 버튼을 이용한 방법입니다.

이렇게 선택한 상태에서 상단의 © 삽입 메뉴를 클릭하면 그림, 차트 So} 삽입에 사용되는 메
뉴가 나타납니다. 나타나는 메뉴 SO ASME 를 선택한 후 팝업 메뉴에서 © ASME 아
이콘을 클릭합니다.

삐 던 S-    =
ita: eee
피벗  주전

*
로 ~
표 AW 온라인 도령 51720441스크린샷 gua - | 주전     a
테이를 피벗 테이블        그릴 1       7

자트
표                        일러스트려이션            | 추가 기능          |

피버 그른 !꺼으선현 S 승

Vv
|. ~ by    스파크라인

느무 70:              7
| Heme             ¥
이 자트의 기능:

“AHH, 월, 일) 뜨는 BsHoj 따른

| 주세를 SHSLC.

7                         -                                 0                       | 다음 경우에 사용:

i                            -                                    @         :                  *항목의 순서가 중요합니다
7                       :                              0       98 | lie 다름 ㆍ데이터 요소가 많습니다.
2      303- 0.77 - 0.86     3.19        0    3.19         =
9         304 - 0,73 -_0.62       3.42          @      3.42

2.58             0       2.58 |                                차트 제목
2.77          @      2.77
40.00
2.98          0      2.98
3.19          0      00 를
3.42          °      3.42 | 30.00
3.66          @      3.66 | 25.00
3.91          @      | |
4.17          0      4.17
4.45          0      4.45 | 19.00
4.73          0      4.73    10.00
5.03          ®      5.03    5.00
5.35          0      5.35       :
5.67          UD      2:67,         1 3 5 7 9 11131517 19212325 2729313335 37 394143454749515355575961
6.01          @      6.01
6.37          0      6.37                  HAA AE
6.73             e       6.73                                  —                                        :

256 4484


===== PAGE 257 =====
그래프는 예쁘게 나왔는데 XS 수치가 이상하네요. ×축에는 옵션가격 계산의 기준이 되는 기
초자산 가격인 현물가격이 들어가야 하는데 말이죠. ※축을 바꿔주는 작업을 해야겠습니다.
우선 그래프에서 XH 데이터를 선택합니다. 그리고 XS 위에서 오른클릭을 합니다. 나타나는
팝업 메뉴 중 데이터 선택 을 클릭합니다.

|
차트 제목               삭제)
40.00                                            SJ 스타일에 맞게 다시 Baa)
| 35.00                                   가 Zao
| 30.00                               때 자른 Ss 2am
| 25.00                           때 데이터 선택도       |
(20.00                                   다
| 1500                                —
10.00                                                 FSss 주가000
5.00                                       보조 Sad 추가0』)
-                                de SAAD
hh 3 5 7 9 1113151719212325272931333537394143a997sy>1355597590"
비이 0=내재가지. -=-시간가겨 2: Pre     ae
ts                              =                       mam (HE SS) a -|
AZ SR \————

차트 데이터를 선택하는 '데이터 원본 선택' 창이 Frc}. 화면의 왼쪽은 그래프로 그려질 데이
터의 값, 오른쪽은 ※축의 값입니다. 우리는 XS 값을 바꿔야 하니 화면의 오른쪽에 관심을 가
져봅시다. 엑셀이 임의로 설정해둔 기본값인 1, 2, 3, …으로 된 값을 현물가격으로 바꾸기 위

해 가로(항목)축 레이블'에 있는 편집 버튼을 눌러줍니다.

데이터 원본 선택                                                                     로 02
AE 데이터 Be): |=506651!9094555569              less]

범례 항목(게열)(5)                                FESS) 즉 려이클(0

naw | Geto) ×42466 x || Geo]
iio - -      |
WM 내재가지
BM 시간가지

띠 띠 띠 띠 띠
uh WH ww

ㅣ 슬겨진 쓸/빈 sD     취소

13장 옵션 엑셀 실습 257


===== PAGE 258 =====
편집 버튼을 누르면 열려 있던 창이 닫히고 새로운 작은 Aol S 레이블' 창이 열립니다. 축
레이블 범위에서 커서가 Wao XS 값으로 사용할 데이터를 받아들일 준비를 하고 있습
니다.

죽 레이블                                ?      x
| 을 레이블 BA):

126 | 범위 선택
[ 90 |] | *소 |

이 상태에서 ASE] ^465까지의 셀을 선택하고 확인 HES 눌러줍니다.

= 레이블                  ?   x

때 레이블 범위(&):

[=SheetiISass:sases 범위 선택
Lae], a |

= 레이블 창이 닫히면서 아까 사라졌던 '데이터 원본 선택' 창이 열립니다.

데이터 원본 선택                                                     ?     x

ALE 데이터 범위(2): | =Sheet1!SAS4:$AS65,Sheet!$D$4:$FS65                  a

범례 항목(계열)(5)
3 주가@) ㅣ 편집@) | >×제거0 | ㆍ |v
wc
    내재가지
M 시간가치

. 6겨진 설/빈 Be)

1, 2, 3, …으로 되어 있던 ※축 Zo] 300, 301, 302, …‥로 변한 것을 확인할 수 있습니다. 이
제 확인 버튼을 눌러 새로 입력한 ×축 값을 차트에 적용합니다.

258 4부 옵션



===== PAGE 259 =====
차트 제목

40.00
| 35.00

25.00
! 20.00
15.00
10.00

5.00

500 303 306 309 312 315 318 321 324 327 330 333 336 339 342 345 348 351 354 357 360     |

—c ---내재가지 ㅡ--시간가지

ㄴ--  -—  -        -  —   —  —  —  $=  그  에

X=} 값이                                 확
차 있어 보기에 좋지 않습니다. XH 값을
을 클릭해 선택한 상태에서 오른클릭한

후 팝업 메뉴에서 축서식 메뉴를

현물가격 값으로 vba 것을 확인할 수 있습니다. 그런데 값들이 너무 Beet 들어
5단위로 표시해서 보기 좋게 만들어봅시다. XS ek

클릭합니다.

차트 RE «ao
40.00                                   Gy] 스타일에 맞게 다시 SSA
35.00                                  가 _글꼴)…
30.00                                   Wh +E 종류 SSW.
go 00                                 (Gh 데이터 선택6@…
, 20.00                                   일 33     in
15.00
“ane                                           주 눈금선 주가04)
5.00                                            보조 눈금선 주가(4)
———
4 ily 죽서식060
00 303 306 309 312 315 318 321 324 327 330 333 336 559 342 343 398 551 359 337 SOY,
eC ====내재가치
!      4                                  ai   Way  '가로 (항목) a.  a=
| 재우기 윤곽선 -…

오른쪽에 *축 서식을 지정하는 화면이 나타납니다.

13장 옵션 엑셀 실습 259


===== PAGE 260 =====
'축 서식" 편집 화면에서 레이블 메뉴를 클릭해 펼칩니다. '레이블 사이에 들어갈 간격'에서 '간
격 단위 지정'을 선택하고 값을 5라고 입력한 후 [Enter] S 누릅니다. %축이 300, 305, 310,
…으로 바뀌며 보기 좋아집니다.

이제는 옵션거래에서 생성되는 부가가치인 시간가치에 집중해봅시다. 같은 차트 내에서 시간
가치는 기초자산 가격 변화에 따라 어떻게 변하는지 관찰하기 위해서입니다.

시간가치 그래프를 선택한 후 오른클릭을 하면 나타나는 팝업 메뉴에서 계열 차트 종류 변경 을
선택합니다.

260 4454



===== PAGE 261 =====
차트 제목

~

2 we
(AAS "시간가지 -
재우기 윤곽선ㄴ-----

300 305 310 315

—_—C

320 325 330 [Aaa
Jf 데이터 As
(3 38 희전@&
데이터 레이블 주가6@)     >
주세선 주가@)
We 데이터 계열 ANH.

ㅡ--내재가지

다음과 그림과 Yo] AE 종류 변경" 창이 나타납니다. 창 아래쪽에 붉은 색으로 표시한 부분

을 보면 각각의 그래프마다 종류를 지정할 수 있게 되어 있습니다.

?   x
(a) he.
=        te Wee 0
뻐 서로
kx Age         사용자 지정 조합
@ 원령       |
= 가로 막대형                 차트 제목
A 영역형         sass
ke 분산형         30.00
lad 주식형
@ 표면혈        15.00
1000
*K 방사형         5600
he 0 |      : 2  3065  310  215  330  325  Lo  35  330  “Ss  350  mS  Ww
—c¢ -ㅡ--내제가치 ㅡ--시간가지
데이터 ASN 대한 자르 SRG os 선택합니다:
CC 두. 으으 1  자르 SF 중류             보조 욱 ㅅ
ac            ‘yeay      fH a
8 내재가지        ee ㅁ
ㅣ 시간가지          mene GQ 이
 aa
134 옵션 엑셀 실습

261


===== PAGE 262 =====
자이

이 중 시간가치 그래프만 기존의 '꺼은선형'에서 '영역형'으로 바꿔줍니다.

~

AE 증류 변경                                           2 pe
SURE 모든 자트
in 죄근에 사용한 항목          |
mi 서식 파일        때 i 000
[때 세로 막대형   tet eee ---ㅡ=
2 mene        사용자 지정 조합      nd 세로 막대형             “I
ae                 well IBA IAA
는 가로 Sree
4000
A 영역형         35.00             E 가로 막대형
je Bares         a                    a
lai FAS         rae                    = Ca
Cees         eR              x mene
wk SNe        500 =       가 SS
—<t 내 3   사 7000
~ /
데이터 계열여 대한 자트 중류와 a PA, ｜^,^
계열 이름          mE      ee            R
fc             연아
8 내재가지
vv
1 시간가지 ae.
Tee 으으
전체 차트 중 시간가치 그래프만 다음 그림처럼 영역형으로 바뀌 것을 볼 수 있습니다.

——

8

차트 제목

8 &
88

8

10.00

8

=
|
|
|

262 4부 옵션



===== PAGE 263 =====
마무리로 차트 제목을 바꿔주고, 각 그래프의 색깔을 보기 편하게 바꾸어주면 좋겠습니다. 차
트 데코레이션은 굳이 금융공학 책에서 다룰 내용은 아니기에 독자에게 맡김니다.

콜옵션 이론가격

|                   m=            |
|| 40.00
「 35.00
|| 30.00                                   |
|| 25.00                                   |
|) 2000
| 150
| 10.00

5.00

300 305 310 315 320 325 330 335 340 345 350 355 360
09 시간가지 ===ㅇ a LAE

이상으로 엑셀을 이용해 옵션 이론가를 산출하고 그래프를 그러보는 시간을 마치겠습니다.

13.3 그래프로 보는 델타와 감마

이번 Belo AS 앞서 살펴본 옵션 그릭스 값들을 엑셀을 이용해서 계산하고 그래프를 그려보
며 그릭스에 대한 감을 느껴봅시다. 바로 앞에서 실습했던 블랙-숄즈 이론가를 산출한 a
을 기반으로 시작해보겠습니다.

델타와 감마를 계산하기 위해 새로운 시트를 만들고 o]=2 ‘Delta ㅎ200102'라고 바꿔줍니다.

| Option 기본 | Delta Gamma

\-)

앞 AJE|OIA] 만들었던 엑셀을 활용하기 위해 ‘Option 기본" ALES] AI~FS BES 다음 그림

과 같이 복사해서 ‘Delta Gamma’ 시트에 붙여줍니다.

13장 옵션 엑셀 실습 263


===== PAGE 264 =====
301 _ -  ARS -  0.93   2.77     aA   2.277

그릭스 중 현물가격 변화에 따라 변화하는 값인 델타와 감마의 변화를 관찰하기 위해 E4S
10610 로, 84를 ‘Gamma’ 바꿔줍니다.

잔존만기가 ASS 그래프의 SHO] 더 눈에 띄게 변하기 때문에 잔존만기를 좀 짧게 바꾸
고 싶습니다. 현재일은 2018-08-01로, 만기일은 12월 옵션 만기일인 2018-12-13로 바꿔
줍니다. 현물가격 변동 범위를 행사가격을 기준으로 앞뒤 50포인트씩으로 넓게 잡기 위해 AS
셀을 280으로 바꿔줍니다.

변동송

이자율

2.49 -

65 셀에 델타를 계산하는 수식을 입력합니다. 콜옵션의 델타 계산식은 4(00/)=^(4,)입
니다. N(x) 엑셀이 함수로 제공하고, dS Bs 셀에서 이미 계산해놓았으므로 간단히 계
산할 수 있습니다. 이를 엑셀 수식으로 나타내면 =NORM.S.DIST (BS, 1046)입니다.

PI    - : ® AS _ fe | -nonn.s.orst(85, TRUE)|



===== PAGE 265 =====
FS 셀에 감마를 계산하는 수식을 입력합니다. 감마를 구하는 식은 P= 일 이고, 여기에서는

(1) =-금-ㅇ입니다. 이 식을 엑셀 수식으로 나타내면 = ( EXP (-1* 85^2 * 0.5)
/27

/ SORT(2* PI()) ) / (45 * 『92ㅋ5007 (052) )입니다.

er XY fel ㆍ < EXP( -1 * 8542 * 0.5) / SQRT(2 * PI()) ) / (AS * F$2 * SQRT(DS2) I}

G     H     I

이제 연속 데이터 채우기를 이용해 현물가격 BAS 3807) 늘려줍니다. 연속 데이터 채우
기는 AS~FSS 한꺼번에 선택하고 오른쪽 하단에 나타나는 BS 클릭한 상태에서 드래그하여
105행까지 내리면 됩니다.

wm 앵사가격

x.

a

4 Belem     01        02        6

| 5       2801-    2.49 -    2.56     0.03 _
6

a

이제 그래프로 그려볼 차례입니다. 델타와 감마 그래프를 그려보기 전에 우선 비교 기준인
콜옵션 이론가 그래프를 그려봅니다. 다른 그래프와 한꺼번에 그리면 눈에 잘 띄지 않아서
D4~D105 셀만 선택해 그려줍니다. 그래프를 그리는 자세한 방법은 바로 앞 Belial 설명
했으므로 생략합니다.

13장 옵션 엑셀 실습 265


===== PAGE 266 =====
260 290 300 310 320 330 340 350 360 370 380

셀만 선택해서 그려줍니다.

H      _ es 010 0 |
고
2                                                                                    (c
3
4
5                                                                                                 ~
6         281                2.50       0.04       8.01     @.e012                                   é
7]        262|-  2.38 - 2.44       0.05       0.01     0.0013 70.00
8 |       283|- «2.32 - 2.38       0.06       0.01     0.0015 20.00
9        284|- 2.26 - 2.33       0.07       0.01     0.0017 3000
10 |      2s5|- 2.21 |- 2227     0.08     0.01    0.0020
11        286|- 2.15 - 2.21       0.10       0.02 | 0.0022                                 =
12        287|- 2.10 - 2.16       @.12       6.02     0.0025        스이 350. 510 550 360 570 380
13 |       288|- 2.04 - 2.10       0.13       0.02     0.0026 |
24      289|- 1.98 - 2.05     0.16     0.02    0.0031               Delta
15 |      290|- 1.93 - 1.99     0.18     0.03 | 0.0035 166
16,        291]-1.87 - 1.93       0.21       0.03 | 0.0038
27.      292|-   1.82 -   1.88     6.24     0.03    6.0042 080
18        293/- «1.76 - — 1.82       2.28       0.03 | 0.0046 660
19        294|- 1.71 - 1.77      0.32       0.04 |  0.0051'
20      295|- 1.65 -  1.71     0.37     0.05 | 0.0056 090
21      296|- «1.60 -  1.66     0.42     0.06    0.0261 | 920
22,        297|/- 1.54 - 1.61       0.48       0.06 | 0.0066 |
23     298|- 1.49 - 1.55     0.54     0.07    e.c071,
24.       1692 20 9 이어      Of       0.08 | 0.0077     280 290 300 310 320 330 340 350 360 370 380

이번에는 감마 그래프를 그립니다.

266 4부 옵션



===== PAGE 267 =====
：                 『           6       내          I          3
만기일    잔존만기    이자율
2018-12-13        5        :          10.00%                         6
, 6000
TT                 2                           [Gamma …~
280|-       .49 -     rE            :                     0.0010 060
281|-      44 -     2:           :                   8.0312
282|-      >          22           iM                   e.0013 70-0
283|-     2.32 |-     22            인                     0.0015 2000
284|-     2.26 -     2.            :                     0.0017 3000
285|-     2          2.           '                   0.0020
286|-     2.15 -      20            :                     @.0022
rome    621"    =         :                은       280 290 300 310 320 330 340 350 360 370 380
288       2.04 -     22           :                   0.0028
289|-   1.98 -   2.       fe             0.0031              Delta
290] -    1.93 -    1 뻔        A              8.2035 309
291|-   1.87 -   a5       9             0.0038
292|-     1.82 -     a;           1                   0.0042 080
293       1.76 -     1.           r                   0.0246 660
294       1.71 -     1.77        0.32        0.04      0.0051
295|-     1.65        1.71        0.37        6.05      e.eass 00
296|-    1.60 -    1.66     0.42     0.26    0.0061 020
297|-   1.54 -    1.61     0.48     0.06    0.2066
298|-   1.49 -   1.55     0.54     0.07    0.0071
299|- 1.43 - __1.50       e.61       2.08     steazz 200 790 900) 510 520. eae
300}-     1.38        1.44        0.69        0.08      0.0083 ：
301       1.33 -     1.39        0.78        0.09      0.0089                    Gamma
302|-     1.27 |=     1.34       0.88       9.10     @:6895 | .
303       1.22 -     1.28        0.98        @.11      0.0101
304|-     1.17, |-     1.23        1.10        @.12      @.0187 166
305]-     1.11 -     1.18        1.23        @.13      @.0113
305]-     1.06 -     1.12        1.37        @.14      0.0120 . go 100
307]-     1.@1 -     1.07        1.52        @.16      @.0126
308       0.96 -     1.02        1.68        6.17      @.0132 66050
389|-     0.98 -     0.97        1.86        0.18      0.0138
310       0.85 -     0.91        2.04        0.20      0.0144      5
311       6.88 -     @.86        2.25        @.21      @.0158         280 290 300 310 320 330 340 350 360 370 360
312      @.75_ -    @.81       2.47       0.23     9.9156

옵션 이론가와 델타, 감마 그래프를 동시에 놓고 비교해봅니다. 행사가격인 330 근처에서 델
타 그래프가 가파르게 상승하는 것을 볼 수 있습니다. 또한 감마 역시 행사가격 근처에서 가장
높습니다.

중학교에서 배운 거리, 속도, 가속도를 떠올려보면 이 세 그래프의 관계를 이해하기 쉽습니
다. 옵션가격의 1차 미분값인 델타는 옵션가격이 변화하는 속도입니다. 현물가격이 올라갈수
록 옵션가격이 올라가는 속도가 빠르고, 그 속도는 행사가격 근처에서 가장 빠르다는 것을 a
타 그래프가 보여줍니다. 옵션가격의 2차 미분값. 즉 델타의 1차 미분값인 감마는 델타 그래
프가 시사하는 바를 확실히 보여줍니다. 옵션가격 변화의 가속도를 보여주는 델타 그래프가
행사가격 근처에서 볼록하게 LOF 있는 모양은 이 부분에서 가속도가 가장 크다는 것을 의미
하지요.

13장 옵션 엑셀 실습 267


===== PAGE 268 =====
1 EERE | oh

13.4 그래프로 보는 세타

이번에는 시간 변화에 따른 옵션가격의 변화를 보여주는 세타입니다. 우선 ‘Theta’eH= 이름
의 새로운 시트를 만듭니다.

| Option 기본 | DeltaGamma | Theta    @
TE Te

이제 옵션 기본정보를 세팅해봅시다. 시간 변화에 따른 옵션가격의 변화를 보기 위해서는 시
간이 변동해야 합니다. 앞에서 실습했던 델타와 감마는 시간은 고정된 상태에서 현물가격이
변동했다면, 이번에는 현물가격을 고정하고 시간을 변동해야 합니다. 따라서 현물가격을 위
기본정보로 올리고 아래쪽 표에 잔존만기를 넣습니다. 위쪽에 적어놓은 잔존만기는 아무
할이 없습니다. 여기에서는 입력하지 않아도 무방하지만 다음 차례인 베가를 위해 남거두었
니다.

쓴
=<
a4

스
=)

행사가격 ㅣ 현물가격 ㅣ 잔존만기 ㅣ 이자율

1년간의 옵션가격 변화를 살펴보기 위해 AS 셀에 1을 입력하고 점차 줄여보겠습니다. 기본
세팅값이 달라졌으므로 01, 02, Cc 역시 다시 계산해야 합니다.

01인 BS 셀에는 =( LN (B$2/A$2) + (D$2+E$2*2*0.5)*A5 ) / ( E$2* 5081 (45) )을 입
력합니다.

268 4부옵션

ET ST


===== PAGE 269 =====
02인 C5 셀에는 = 85 - E$2 * 5081 (45 )을 입력합니다.

0 a    x V~ ^ | 66969 0

8     620
현물가격   잔존반기 .

행사가격 |

4                     i
1.001    @.2803 P= BS - E$2 *

콜옵션 이론가인 D5 셀에는 =B$2 * NORM.S.DIST (BS, TRUE) - A$2*EXP (-D$2*A5 )*NORM.
S.DIST (C5, TRUE)-& 입력합니다.

PI           2] > ~ Sac 652 * NORM.S.DIST(8S, TRUE) - AS2*EXP(-D$2"AS)*NORM.S.DIST(CS, TRUE)}

F      G   6  H

oe
1.0a1    0.2803 |    0.1803 = 852 * NORM

트디어 세타의 차례입니다. 콜옵션의 세타를 계산하는 수식은 o= SAVE _ cer (a)
입니다. 이를 엑셀 수식으로 나타내면 = -1* ( 6$2* ( EXP( -1* 85^2* 0.5) / 5001 (2 *
PI()) ) * E$2 ) / (2* 5081 (45) ) - 052 * A$2 * EXP( -1* 052 * AS ) * NORM.S.DIST

(C5, TRUE) SUCH.

= Bas te  --1 ( B$2 * ( 60( v1 852 © 0.5) / SQRT(2 © PI()) ) * 592 ) / (2 1 SQRT(AS) |
- 052 * 452 * EXP( -1* 052 * AS ) * NORM.S.DIST(CS, TRUE)

1.00!       0.2803 |

이제 잔존만기를 줄여가봅시다. AG 셀에 0.98을 입력하고 AS~AG WS 함께 선택한 후 연속
데이터 채우기를 이용해 만기가 0인 ^55까지 데이터를 ABUCt.

13장 옵션 엑셀실습 269



===== PAGE 270 =====
B5~ESS 함께 선택한 후 연속 데이터 채우기 기능을 이용해 855까지 데이터를 모두 채옵니다.
55행을 봅시다. 데이터가 이상하네요?

B              |              <              i              D              |               E              i
9.2493                           @.2352                           2.4847  -                     49.17
#DIV/0! ” #pIv/e! ” #pIv/e! ” #DIVv/e!

분모에 들어 있는 잔존만기가 0°] 되어 계산 불가능 에러가 생긴 것입니다. 이 BAS 해결하
기 위해 455 셀 값을 0 대신 0.001로 바꿔줍니다.

「          ^          i          B          1                      i          D          1           E          i

2.2493,      A 2352      2 4847 =     49.17
5      0.00   0.9647    0.9616    1.1000 -   136.59 |

A5SS 0.001 바꾸었지만 여전히 A55 셀에는 0으로 표시가 됩니다. 하지만 855~ㅁ55에 있
던 에러는 사라졌네요. 이제 세타 값을 그래프로 그려보겠습니다.
F      G      H      z

뽀                           ~

$ |     1.08   ©.2803    0.1603   17.1606 |-   10.05

6     0.98   0.2781    0.1791   16.9590 |-   10.11             Theta

7     0.96   0.2758    8.1779   16.7561 |-   10.18

8    0.94   0.2736   0.1766   16.5517 |-   10.25     1               oF   0.00
9     0.92   0.2713    0.1754   16.3460 |-   10.33 | -2000

10     0.90   0.2691    0.1742   16.1387 |-   10.40

12   0.88  0.2668  0.1730  15.9299 |-  10.48 | -40.00

12)     0.86   0.2645    0.1717   15.7195 |-   10.56

13     0.84   0.2621    0.1705   15.5074 |- 10.64 |

14     0.82   0.2598    0.1692   15.2937 |-   10.73 | -so09

15     0.8   0.2574    0.1680   15.0781 |-   10.82

16    0.78  0.2551   0.1667  14.8607 |-  10.92 | -10000

17)     0.76   0.2527    0.1655   14.6415 |-   11.01

18    0.74  0.2502   0.1642  14,4202 |-  3154190|| 220.00

19    0.72  0.2478   0.1629  14.1969 |-  421-22 | 500

20     0.70   0.2453    ©.1617   13.9714 |-   11.33

270 4부 옵션


===== PAGE 271 =====
13.5 그래프로 보는 베가
이번에는 베가를 구해보겠습니다. 베가 작업용 새 시트를 만듭니다.

| Option 기본 | DeltaGamma | Theta | Vega |   @

옵션 기본정보를 세팅합니다. 베가는 변동성이 변할 때 옵션가격의 변화를 보는 것이므로 아
래 표에는 변동성을 넣어줍니다. 44 셀에 `변동성*을, 854 셀에 7682 를 입력합니다.

변동성이 변하는 구간을 1~100%까지 움직여보기 위해서 AS 셀에 1%, AG Aol] 2%를 입력하
고 연속 데이터 채우기를 이용해서 100%까지 입력해줍니다.

01, 02, C 값을 계산하기 위한 수식을 입력해줍니다. 01은 =( LN (B$2/A$2) + (D$2+A6%2*
@.5)*C$2 ) / ( AG* 5081 (C$2) )입니다.

SUM     - 1 | × oO fe | =CLN(BS2/A82) + (DS2+A54240.5)*CS2 ) / (AS* SQRT(CS2) )
4    ^        8        ㄷ        ㅁ        E       6    i    G

1   행사가격   현물가격    잔존만기    이자을     변동성

2 :   330   |   329   ㅣ     0.38 | 2.00% | 10.00%

3

4 Ai |.    01        02        Cc       Vega

EY         @%|RT(C$2)_)

6        1%

13S 옵션 엑셀 실습 271


===== PAGE 272 =====
02는 = 85 - AS * SORT (6$2 )입니다.

콜옵션가격인 CE = 8$2 * NORM.S.DIST(B5, TRUE) - A$2*EXP (-D$2*C$2)*
NORM.S.DIST (C5, TRUE) 9Uct.

PI       ~ ×  fe |  = B$2 * NORM.S.DIST(B5, TRUE) -
AS2*EXP (-D$2*C$2)*NORM.S.DIST(C5, TRUE)

이제 베가 수식을 입력할 차례입니다. 베가를 구하는 AS 다시 한번 보겠습니다.

dC      ;
Yi) == S.VTN'(d,)

엑셀 수식으로 나타내면 =B$2 * SQRT(C$2) * ( EXP( -1 * 85^2 * 0.5) / SORT(2* PI()) )
입니다.

272 4부 옵션



===== PAGE 273 =====
이제 BS~ES 셀을 한꺼번에 선택해서 연속 데이터 채우기로 100%까지의 베가 값을 구합니
다. 베가 그래프를 그리기 위해 E4~E104 셀을 선택한 후 삽입 〉 치트 를 눌러 AOA 그래프

를 추가합니다.

5 |     1%    0.75 @.7485679 1.7972636   61.25

Gil      2%    @.38 ©.3696308 2.50361¢2   75.78                 Vega

7 |      3%    @.26 @.2412504 3.2786857    78.73 | 68200

8 |     4%   @.20 ©.1755@91 4.0721589   79.81

9 |      5%    0.17 0.1348235 4.8731038    90232 9000

10 |     6%   0.14 0.1066657 5.6777891   80.59 78.00

11     7%   @.13 @.0856667 6.4845954   80.76 ©) 2609

12     8%   @.12 @.069142 7.2927051   82.86

13 |     9%   @.11   @.0556 8.1016589   88:93) || 7400

14 |    10%   0.11 _ 0.044146 8.9111777   80.97 7200

15 |    11%   0.10 0.0342106 9.7210806   81-81 |

Be)     노식    DoH CAE hey TREE MENS    ES      1% 11% 21% 31% 41% 51% 61% 71% 81% 91%

90    13%   0.10 @.0174935 11.341582   81.04     ：    i   :  = oN
14%    @.10 _0.0102613_12.152027:    81.05 |

실습을 마친 결과 예시 파일은 13. Option 6「665.×15×입니다.

지금까지 금융공학에서 가장 유명한 모델인 블랙-숄즈 방정식을 엑셀 기본 기능만으로 구현
하고, 그중에서도 어렵다고 하는 그릭스 값들을 산출하고 그래프로 그려서 모양을 살펴보며
기초자산 가격, 잔존만기, 변동성이 변함에 따라 옵션가격에 어떻게 영향을 미치는지 살펴보

았습니다.

13장 옵션 엑셀 실습 273


===== PAGE 274 =====
14.1 그래프 그리기 끝판왕 WES

파이썬에서는 RSLA (matplotlib) 라이브러리를 활용해 다양한 그래프를 그릴 수 있습니
다. 특히 그래프 전문 라이브러리인 WSS A] 데이터 전문 라이브러리인 팬더스와 결합하면
복잡한 모양의 그래프도 간단히 그려낼 수 있습니다. 이번 챔터에서는 WSRAS 사용해 다
양한 그래프를 그려보는 방법을 알아보겠습니다.

WESz 라이브러리 호출 및 노트북 사용 세팅

RELAIS 사용하기 위해서는 항상 그렇듯이 라이브러리를 호출해야 합니다. 그런데, 우리가
코딩하는 노트북 환경에서는 하나 더 해줘야 할 일이 있습니다. 그래프를 결과 화면으로 출력
하라는 명령을 추가해야 합니다.

1 import matplotlib.pyplot as plt
2 ‘%matplotlib inline

Out

2행의 %matplotlib inline 4°] 바로 그것인데, WSRYS 라인 Apolo] 출력하겠다는
의미입니다. 이 작업을 해주지 않으면 그래프가 어디에 나타나는지 찾아보기 어렵게 됩니다.

274 4부 옵션

ST


===== PAGE 275 =====
노트북이 아닌 다른 환경에서 코딩을 하면 ~~.0\라고 BES 저장하게 되는데 ~~~. py 코드

를 실행하면 새로운 창이 뜨면서 그래프가 보입니다.

그래프 그리기
이제 그래프를 출력하는 명령어인 0나.ㅁ10\( )를 입력해봅니다.

1 plt.plot()

0060크림[15.1.1:1

0.04 +
0.02 +
0.00 +
0,02 4
-0.04 +
-0.04        -0.02         0.00          0.02          0.04

내용이 들어 있지 않은 빈 그래프 틀만 출력되었네요.

이번에는 그래프 틀의 사이즈를 조절해보겠습니다. SS 건드릴 HE plt.figure()S 이용
하는데, 사이즈 AAS plt. figure (figsize=(x, y))= 합니다. 사이즈 AAS 별도로 Sf
Al 않은 기본 사이즈는 6×4입니다.

1 plt.figure(figsize=(10, 5))  # 그래프 ZaI7/ 설정
2 plt.plot()

14장 코딩 기술: 시각화 275


===== PAGE 276 =====
대 eee

Out

0.04 +

0.02 4

0.00 +

-0.02 4

-0.04                    -0.02                     0.00                      0.02                      0.04

사이즈가 10 ×5인 틀이 출력됐습니다.

이제 그래프에 내용을 넣어봅시다. 그래프에 들어갈 값을 임의의 값으로 채우기 위해 넘파이
를 사용하겠습니다. 우선 넘파이 라이브러리를 호출합니다.

1. import numpy as np

Out

그래프의 ※축은 102] 간격으로 100부터 300까지로 정합니다. S 100, 110, 120, …저럼 표
현되며, 총 20개의 값을 갖습니다. 넘파이 함수로 나타내면 10.0728096 (100, 300, 10) U4
다.

np.arange(start, end, interval)
(생략 가능, 기본값 0)     (생략 가능, 기본값 1)

* 시작과 끝 AIS 일정한 간격으로 채운 배열을 반환합니다.

축은 표준정규분포를 따르는 임의의 값으로 합니다. 표준정규분포를 따르는 \값은 평균이
0, 표준편차가 1인 분포상에서 임의의 값이 할당됩니다.

276 4부옵션



===== PAGE 277 =====
np.random. randn(n)
(발생시킬 난수의 개수)
* 표준정규분포 NO, 1)를 따르는 난수를 개 반환합니다.
* 00.0280000.ㅁ200(0/은 특정 분포를 따르지 않는 난수를 반환하므로, SS 구분해야 합니다.

축의 값을 지정할 때 XSL] 값과 같은 개수만큼 지정해야 합니다. ×의 개수와 yo] 개수가 같
지 않으면 파이썬은 에러 메시지를 반환합니다. 그러므로 *값으로 발생시킬 난수의 개수는 ×
의 개수만큼인 20으로 지정합니다.

1 x = np.arange(10@, 300, 10)
2 y = np.random. randn(20)
3 plt.plot(x, y)    #x, yS 지정해서 그래프 그리기

Out     20

1.574

0.0 +

-0.5 5

—1.0 5

100     125     150     175     200     225     250     275

※축은 100부터 300774], 축은 -2부터 2까지로 표시된 그래프가 출력되었습니다.

XS} 값은 생략할 수 있는데, XS WS 지정하지 않고 축의 값만을 지정해준다면 그래프는
다음 그림과 같이 0부터 시작해서 20개의 값을 출력하게 됩니다.

14장 코딩 기술: 시각화 277


===== PAGE 278 =====
1 plt.plot(y)    # ^죽을 지정하지 않고 그래프 그리기

Out         2.0

1.55

1.0 4

0.5 5

0.0 5

-0.5ㅋ

-1.0ㅋ

=—1'5 5

-2.0

oO 206 SO 75 000 wo 5800 453

이전의 그래프와 달리 X= 값이 0부터 20까지 표시된 것을 확인할 수 있습니다.

이번에는 틀 사이즈를 (10, 5)로 조절하고 위 그래프를 그려보겠습니다.

1 plt.figure(figsize=(10, 5))    # 그래프 사이즈 지정
2 plt.plot(x, y)

Out           2.0                                                                                                                                                                                     ㅣ

154

1.0 4

055

0.04

100            125            150            175            200            225            250            275

그래프를 그릴 때마다 S A}o|ZS plt. figure (figsize=(10, 5 ) )처럼 지정하기가 귀찮
으면 미리 설정해놓는 방법도 있습니다. 「ㄷ라는 파라미터를 미리 세팅해놓으면 프로그램 전
체에 해당 파라미터값이 적용되기 때문에 편리합니다.

278 4484



===== PAGE 279 =====
1 plt.rcParams['figure.figsize'] = (10, 5)    # 그래프 사이즈 지정

Out

rcParams& 이용해서 세팅할 수 있는 파라미터는 약 300714] 정도로 엄청 많습니다. 이들 값

들을 알고 싶으면 plt.rcParams 명령어를 입력하면 됩니다.

1 plt.rcParams

Out RcParams({‘_internal.classic_mode’: False,
‘agg.path.chunksize’: 9,
‘animation.avconv_args': [],
‘animation.avconv_path': ‘avconv',
‘animation.bitrate'’: -1,

이제 별도의 사이즈 지정 없이 rcParamsollAl 지정한 값을 적용해 바로 그래프를 출력해보겠

습니다.

1 plt.plot(x, y)

Out           2.0

a LS

1.04

0.5 -

0.05

-0.54

-1.04

—1,5

204

125          150         175         200         225         250         275

14% 코딩 기술: 시각화 279


===== PAGE 280 =====
그래프 모양 설정하기

그래프 모양도 바꿀 수 있습니다. plt.plot () 안에 속성값으로 지정할 수 있는데, 그래프의
색상, 선 모양 SS 지정해주면 원하는 모양으로 upc}, 색상은 6010「='색상', Al 모양은
11065Ｌ716='선 모양', 데이터 AS 표시하는 DYE marker='HA| 모양' SOs 지정합니
다. plt.plot (x, y, color='red', 110651916=' --' , marker='0') 형태로 말이지요.

색상은 레드, 블루, 스카이블루 등 일상에서 사용하는 표현으로 지정하며, 레드, 블루, 그린,
블랙의 기본색은 「, 5. 9, 로 짧게 나타낼 수 있습니다.

ㄷ                   cyan
‘m'                          magenta
yellow
black
‘w'                          white

마커에도 여러 가지 모양이 있는데 대표적인 ASS 다음과 같습니다. 더 많은 마커 모
양을 알고 싶다면 Wee 공식 웹사이트의 마커 모양을 안내하는 페이지인 https: //
matplotlib.org/api/markers_api.html& 참고하세요.

280 4484


===== PAGE 281 =====
a

으
rie

@
ne
Is
dt

Oy
NS
ns
ont

og

그
모
‘on
SJ

x
HI
Ole
N

uD)                  다이아몬드

그럼 색깔은 빨강, 모양은 점선, 마커는 원으로 지정해 같은 그래프를 다시 그려보겠습니다.

1 plt.plot(x, y, color='r', linestyle='--", marker='o0')
2 #plt.plot(x, y, '/0--')도 같은 표현

Out     2.0

1.57
1.04                /

0.51 @     #

100            125             150            175            200            225            250            275

귀차니즘에 빠진 프로그래머들을 위해 자주 사용하는 색상과 Al 모양, 마커 모양 등을 조합해
짧게 축약형으로 나타낼 수도 있는데 위 그래프의 BP plt.plot (x y, '「0--' )로 나타낼
수 있습니다. 이 책에서는 코드를 읽기 AES 축약형을 사용하지는 않겠습니다.

위에서 설명한 속성들 이외에도 마커 사이즈(0206「5126=' 숫자' ), 마커 색(03ㅁ61866
6010「='색상' ), 마커 경계색(0206「60960010ㄷ=' 색상' ), 투명도(31018=' 0~1 사이 소수'

등 여러 가지 속성을 지정해 그래프를 꾸밀 수 있습니다.

14장 코딩 기술: 시각화 281



===== PAGE 282 =====
제목, 축 이름, 범례 삽입
그래프의 ASS 넣어봅니다. ASS 넣을 때는 ZH] plt.title '제목' )과 같이 지정할
수 있습니다. 앞에서 언급한 속성들과 함께 제목을 추가한 그래프를 그려보겠습니다.

1 plt.plot(x, y, color='m', linestyle=":', marker='*', markersize='20' )
2  fae title(’ 제목' )   # 따로 살정하지 않으면 한글이 Li =e)

|
|

0.04 5 :   i : E f *

100      125      150      175      200      225      250      275

|

색상은 자주색(22800), 41 모양은 점, 마커는 별 모양, 마커 사이즈는 20으로 지정했고, 그
래프 ABS 한글로 AS Oe 지정해 그래프를 그렸습니다. 그래프는 예쁘게 잘 나왔는데 제
목이 깨졌네요. WSS] 기본 폰트가 영어 전용 폰트라서 한글이 깨진 것입니다. 그래프에
서 한글을 사용할 수 있도록 한글 폰트로 바꿔줘야 합니다.

S12 rcParamsS 이용해 프로그램 내내 % 이용할 수 있게 설정할 수도 있고, 노트북의 한
셀마다 설정할 수도 있습니다. 우선 rcParamsS 이용해 한글 폰트를 사용할 수 있게 세팅해
봅시다.

1 # 그래프에서 한글 사용 세팅

2 plt.rcParams['font.family'] = ‘Malgun Gothic’
3 plt.rcParams['font.size'] = 12
4

plt.rcParams[ ‘axes.unicode_minus'] = False

282 4부옵션



===== PAGE 283 =====
ㅜ

2행의 plt.rcParams['font.family'] = '폰트명'에서 사용할 SES 지정하는데, 이때 한
글 폰트를 지정해주어야 합니다. 여기에서는 eae 폰트를 지정했습니다. 만일 opie 4
퓨터에 맑은고딕 폰트가 없거나, 다른 SES 사용하고 싶다면 WSEHO] 사용할 수 있는 폰
트에는 어떤 것들이 있는지 조회해볼 수 있습니다.

1 / WBRZ 사용할 수 있는 폰트 리스트 조회
2 from matplotlib import font_manager

3 set(sorted({f.name for f in font_manager.fontManager.ttflist]))

Out ~~
"Nanum Brush Script’,
“Nanum Pen Script’,
‘NanumBarunGothic' ,
"NanumBarunpen’ ,
"NanumGothic',
‘NanumMyeongjo' ,
"NanumSquare’ ,
‘NanumSquareRound' ,

—s

폰트명'에 넣어주면 됩니다. 필자의 경우 네이버에서 PRS 배포하는 '나눔글꼴 모음'을 설치
해 나눔 폰트들이 많이 보입니다.

이렇게 해서 나오는 폰트 목록에서 원하는 SES 찾아 plt.rcParams[' font. family'] = '

이제 한글 세팅을 했으니 그래프를 다시 그려봅니다.

1 plt.plot(x, 1, color='m', linestyle=':', marker='*', markersize='20')

2 plt.title('aj=')

148 코딩 기술: 시각화 283



===== PAGE 284 =====
Out                                                                제목

20 5

05 4    * i i *    i   Ei   x  x.
004    Vi  * :   *    : *   :
054     *    |  별     E

100        125        150        175        200        225        250        275

한글 제목이 잘 들어가 있는 모습을 확인할 + 있습니다.

이번에는 그래프에 그리드를 추가해 더 읽기 쉬운 그래프로 만들어보겠습니다. 6 나.
grid (True) = 간단히 할 수 있습니다.

1 plt.plot(x, y, color='m', linestyle=':', marker='*', markersize='20')
2 plt.title('aJ2', size=29)
3 plt.grid(True)

Ce                                       제목

201-     ——      a 12 [+

104          :  4          시 taf
0.04—}- —}-}-  > :    x te
7G See > ae —- dco a 고"

100           125           150           175           200           225           250           275

-1.0

앞에서 한글 세팅 방법이 두 가지가 있다고 했습니다. 지금까지 알아본 방법이 프로그램 전체

284 4부 옵션


===== PAGE 285 =====
1
ㅇ

에 반영되
다. 이 방법
서 저장한 딕셔너리

방법

|

a 낼

|었다면, 이번에는
한글 폰트를 딕셔너리에 저장하고, 제목

를 호출하는 방식입니다. ie | 등
폰트가 PCO] 없다면 한글이 깨져 보일 것입니다. 원

, 축 레이블 등 한글을 ees

노트북의 한 셀에만 적용되는 방법을 사용해보겠습니

뷰는의

1 font_title = { '720115':

"Nanum Brush Script’, ‘color’: ‘black’, ‘weight’: ‘bold’, ‘size’:

40}
2 font_label = {'family’: 'Nanum Pen Script’, ‘color’: ‘black', ‘weight’: ‘regular’, ‘size’:
25}
3
4 plt.plot(x, y, color='m', linestyle=':', marker='*', markersize='20')
5 plt.title('A]S', fontdict=font_title)   # AS 지정
6 plt.xlabel('X2i(SHHA+)', fontdict=font_label)   # XS AS
7 plt.ylabel('Y2t(S44H=)', fontdict=font_label)   # YS 제목
8 plt.grid(True)
Out
져요
:                       me |
|        *
$ 1.07—|      ry   |  rs       i |    “      J   *
주  |    > ¢     :  6       ‘ 고        4
1.0   |               ;  *          *            *
co) (ia a    |= a ae       “Sah 25    개        :
|               *
100    125    150    175    200    225    250    275
XU (L4§u24)

1행과 2행은 제목과 = 레이

ZN" 5 61126:

블에 각각 사용할 폰
리 내부를 살펴보면 딕셔너리명 = {'family': '폰트
크기} 형태로 지정하고 있음을 알 수 있습니다. 여기에서 주의해야 할 점은 시
명을 지정하면 에러

스템에 저장된 폰트만 사용할 수 있다는 사실입니다.

메시지와 함께 기본 폰
다.

u
ZEel GE 전용 폰트로

트를 딕셔너리로 저장한

트로 자동으로 전환되어 한글이 다시 깨질

명', ‘color’: '색깔', ‘weight’:

저장되지 않은 폰트

14장 코딩 기술: 시각화

부분입니다. 딕셔너

a

285



===== PAGE 286 =====
행은 제목을 지정하고 폰트를 701+_ +1116 딕셔너리로 지정한 부분이고, 6행은 ×축 레이블
지정하고 HES font_label&, 7행은 YS 레이블을 지정한 부분입니다.

UW

ttlo

이번에는 그래프를 하나 더 추가해보겠습니다. 그래프가 두 개이니 각 그래프가 무엇인지 표

시할 수 있도록 꼬리표를 달아줘야 합니다. 그래프에서 꼬리표는 범례라고 합니다. 범례를 다
는 BPH plt.plot() 안에 18661='레이블'과 같이 붙여줍니다. 범례를 표시하는 위치는
pit. legend (106='위치' )로 나타내는데, 컴퓨터에게 알아서 가장 좋은 위치에 나타내라고
할 때는 위치를 best 지정합니다.

plt.plot(x, y, color='m', linestyle=':', marker='*', markersize='20', 13661='그래프1')

plt.plot(x, y+1, color="orange’, linestyle='-', label='12}2£2')

1
2
3
4 plt.title('Al=', fontdict=font_title)  # 제목 지정

5 plt.xlabel('X2i(SH4+)', fontdict=font_label)   # XE 제목
6 0ㅁ나./13061('값(종속변수)', fontdict=font_label) # YS 제목
7 plt.grid(True)

8  0056 pose CLC best’ on

100           125           150          175          200          225          250          275

|                                ×값(독립변수)

1행과 2행이 그래프를 그리고 범례를 붙여준 행이라면, 8행은 범례를 표시할 위치를 지정한
부분입니다.

286 4454


===== PAGE 287 =====
여러 개의 그래프를 모아서 보여주기

이번에는 여러 개의 그래프를 모아서 보여주는 방법을 살펴봅니다. 여러 그래프를 한 Hol] 모
으기 위해서는 Aul7]el figures +19에 할당한 후, +19의 Zt 자리에 240_540010Ｌ( )을 At
용해 각각의 그래프를 추가하는 방식을 사용합니다.

1
2      여러 개의 그래프 모아서 보여주기
4 fig = plt.figure(figsize=(16, 10))    # 그래프 사이즈를 지정하고 719에 할당
5
6 # Subplot 지정: add_subplot(#, 열, 순서)
7 3×1 = fig.add_subplot(2, 3, 1)    # 284 3S fig 중 AA 자리를 ax10 할당
8 axl.plot(x, y)  # ax1O/ plot() 그리기
9
10 ax2 = fig.add_subplot(2, 3, 2) # 284 32 fig 충 SA 자리를 ax2o 할당
11 ax2.hist(y)  # ax20 hist() 그리기
12
13 ax3 = fig.add_subplot(2, 3, 3) # 284 3열 fig 중 셋째 자리를 ax3o/ 할당
14 ax3.scatter(x, y)   # ax30/ scatter() 그리기
15
16 ax4 = fig.add_subplot(2, 3, 4)    # 284 3S fig 중 넷째 자리를 ax4o 할당
17 ax4.plot(x, y, color='r', linestyle="--')   # ax40i] plot() 그리기
Out                        Fi
i                    as                    a)
is                    PA                    19          a
1                    25                    10           oh.
os             \     =                  os}.   ㆍ         i
a a             15                 629    ㆍ  $   ere
os                    18                    2s    ㆍ
-10                    os                    “10        -    ㆍ     %
wo   150   200   20      Md                      wo   ™   200   ~~
20
is
10
os
00
as
10            '
100   190   200   20

14장 코딩 기술: 시각화 287



===== PAGE 288 =====
4행에서 그래프의 Au7/el plt.figure()S 10에 할당합니다. 7행의 fig.add_
subplot (2, 3, 1)은 4행이 지정한 Aul7|7} 2행 3열로 나누어질 것임을 선언한 후, 그중 Al
번째 자리를 3×1에 할당한 것입니다. 8행에서는 361에 plot )을 그린 것입니다. 방식
으로 둘째부터 넷째 자리까지를 채워 넣었습니다. 다섯 번째와 여섯 번째는 따로 그래프를 지
정하지 않아 빈칸으로 남아 있습니다.

이번에는 다른 방법으로 표현해보겠습니다. 이번 방법은 Aul7|S +10에 할당하는 동시에
3×65에도 할당을 하는데, axes= Ax7]2! figure 안에 들어 있는 각각의 그래프 하나씩
을 가리킴니다. 719, axes = plt.subplots(n, ㅁ)이라고 하면 figure AqI7] 안에 na m
열의 subplots 넣을 것이며, 각 subplotSs 3×65에 할당한다는 뜻입니다. 이렇게 하면
3×65[행, 열]은 각 5640010+을 가리키는 배열이 됩니다.

여러 개의 그래프 모아서 보여주기 2

fig, axes = plt.subplots(2, 3, figsize=(16, 10))    # SubplotS 지정하는 또다른 방법

axes[@, @].plot(y)
axes[@, 1].hist(y)
axes[@, 2].scatter(x, y)
axes[1, @]-plot(y, ‘g--')

Out

CODD & A w YH (년

°     s     10    15                                     100    150    200    250
oO                          19
20
os                          os
us             rf
19               Hi           06                          06
H
os               |
i                                       04
00             i        of
Lae
te
a                v          02                          02
10                i
00                          co

°        s        10       15               oo     02      04      oe     os      10     00     02     o4     06     os      109

288 4454


===== PAGE 289 =====
4행은 figures 2행 3열로 나누어 각 subplot-& 3×65에 할당하는 부분입니다. 6행부터 9행
까지는 할당된 23×65[행, 열] 각각에 그래프를 그리는 부분입니다.

먼저 소개한 방법과는 그래프가 할당되지 않은 부분이 공백으로 나오느냐, 빈 그래프로 나오
느냐의 차이도 있습니다.

14.2 HERB Tt 팬더스의 만남
맺플롯립과 팬더스가 만나면 복잡한 그래프를 쉽게 그려낼 수 있는 막강한 파워를 발휘합니
다. ASS 위해 우선 팬더스를 불러옵니다.

1  import Pandas a as 5 pd

Out
금융공학 책이니 주가 데이터와 비슷한 그래프를 만들어봅시다. 1개월간 3개 종목의 주가 al
이터를 임의로 생성합니다. 임의의 값을 지정하는 것은 앞에서와 마찬가지로 표준정규분포에
해당하는 난수 값인 00ㅁ.「『80000.『23000 (개수 ) 함수를 이용합니다.

N(1000, 100)인 정규분포를 따르는 WY 주가 생성
201814 9월 1일부터 30일 동안의 날짜로 인덱스 생성
갈럼명을 기업명으로 설정

df = pd.DataFrame(np.random.randn(30, 3)*100 + 1000,
index=pd.date eee ae periods=30, freq='D'),
6014005=['천리마마트', '히드라마트', '터렛마트'])
df.plot.line() # 팬더스와 함께 그러낸 기본 차드

wo Ont DN 은 WYN RP

148 코딩 기술: 시각화 289



===== PAGE 290 =====
Out

moo}

1000 +

— 천리마마트

60001 _ _ 허드라마트
— 터렛마트
03             10             17             24
Sep
2018

>

6행은 평균이 1000, 표준편차가 100인 난수를 발생시키는 부분입니다. 30일간 3종목의 난수
매트릭스이므로 00.「80000.「3000 (30, 3 )으로 지정해줍니다. 7행은 2018년 9월 1일부

30일간의 날짜 데이터를 생성해서 0+의 인덱스로 지정한 부분입니다. 8행은 각 종목으
을 지정한 부분입니다. 9행에서는 생성한 데이터프레임을 선 그래프로 표시하는 명령
합니다.

c

IN

ce
Jo
의
ol

o

a
+
oot

막대 그래프 그리기
이번에는 9월 1일부터 5일까지의 데이터를 추출해서 막대그래프로 그려봅니다. 막대그래프
를 그릴 We df.plot.bar ()S 이용합니다.

x. ! df[:5].plot.bar()

290 4% 옵션


===== PAGE 291 =====
4001

2003

mee 천리마마트
」 000 히드라마트

mam 터렛마드

1111

2018-09-01 00:00:00

2018-09-02 00:00:00
2018-09-03 00:00:00
2018-09-04 00:00:00
2018-09-05 00:00:00

크래프는 잘 나왔는데, XS

|
|
|

표시하고 싶습니다. 인덱스

|
|
|
|
|

인 날짜 부분이 보기에 거슬리네요. 시간 부분은 잘라내고 날짜만
를 가져온 후 날짜 부분만 추출해서 XS 값으로 지정해줍니다.

1 df[{:5].plot.bar(x=df[:5].index.date)

Out
699 천리마마트
10001 Sam 히드라마트
mmm 터렛마드
800 +
600 4
400 4
200 +
03
5             8             8              3             8
8              8             g              8             8
Rg             을             R              Rg             R
이번에는 막대그래프를 쌓아서 표현해봅니다. 쌓인 막대그래프는 합계 값이 중요한 데이터를

14장 코딩 기술: 시각화 291



===== PAGE 292 =====
표시할 때 유용합니다. 막대를 쌓으려면 .010.680『( )에 인수로 513060=1ㅠ「046를 넣어줍
니다.

1 df[{:5].plot.bar(x=df[:5].index.date, stacked=True)
Out

3000 4

me 천리마마트
ma 히드라마드
25001                                           ma 터렛마트

2000 +
1500 4
1000 +
500 +
02

02
03

2018-09-01
2018-09
2018-09

2018-09-04
2018-09-05

1 df[:5].plot.barh(x=df[:5].index.date, stacked=True)

Out

699 천리마마트
Gam 히드라마트
mmm 더렛마트

2018-09-05

2018-09-04

2018-09-03

2018-09-02

2018-09-01

0                500              1000             1500             2000             2500              3000

292 4부옵션



===== PAGE 293 =====
데이터의 분포를 나타내는 히스토그램

어느 영역에 데이터가 많이 분포하는지를 나타내는 그래프를 히스토그램이라고 합니다. WS
롯립에서는 0『.010ㄷ.1115Ｌ( )로 그립니다. 히스토그램을 그릴 때는 구간의 사이즈를 지정해
주어야 컴퓨터가 구간을 사이즈에 따라 나누고 해당 구간에 소속된 데이터 개수를 헤아릴 수
있습니다. 구간 사이즈는 0105=사이즈 값으로 지정합니다.

1 df.plot.hist(bins=2@, grid= True, alpha=0.5) # bins = 볼록 사이즈

Out                                |                              |

51           '                                mmm 전리마마트 -

Frequency

여기에서는 alpha 값을 지정했는데, alpha7} 1이면 완전 불투명하고 작아질수록 투명해지며
0이면 완전 투명하게 됩니다. 히스토그램에서는 개수가 합쳐져서 보여지므로 투명도를 1보다
작게 지정했습니다.

영역형 그래프

선 그래프는 데이터 하나하나의 움직임을 나타내는 데 강점이 있다면, 영역형 그래프는 여러
데이터의 누적값 움직임을 나타내는 데 좋습니다. 예를 들면, A 그래프로 일정 기간 각 종목
의 주가를 표시하면 눈에 잘 띄지만, 영역형 그래프는 일정 기간 세 종목 주가 누적값의 움직
임을 한눈에 파악하는 데 도움이 됩니다. 실제로 여러 종목 주가의 누적값을 구할 일은 별로
없지만, 거래 대금 합계 등 지수를 산출하는 과정에서 영역형 그래프가 도움이 됩니다. 영역형
그래프를 그릴 w= df.plot.area()=@ 표시해주고, 값을 누적시키려면 9680<60=1ㅁ46라고

인수를 전달합니다.

14장 코딩 기술: 시각화 293



===== PAGE 294 =====
|

1 df.plot.area(stacked=True)

Out

669 천리마마트
Ge 히드라마트

원그래프는 특정 시점의 데이터 값 크기를 비교할 때 좋습니다. 다음 그림은 9월 1일 각 종
목의 주가를 비교해놓은 원그래프입니다. 특정 일자의 시가총액을 비교할 때 도움이 됩니다.
df.plot.pie()# 그리며 autopct='%.2F' 인수를 전달하면 파이썬이 자동으로 각 값의 비
율을 계산해서 그래프에 표시해줍니다. '%.2+'는 비율을 소수점 둘째 자리까지 표시하라는

의미입니다.

1 df.iloc[@].plot.pie(figsize=(6, 6), autopct='%.2f')

Out

천리마마트

와

2d{p-09-01 0:00.00

=
[=]
=
m

터렛마트

294 4부 옵션


===== PAGE 295 =====
ih) EE |

데이터 값이 어떤 모양으로 분포되어 있는지를 알아보기 위해서는 밀도 그래프를 그릴
수 있습니다. df.plot.kde()=S 그리는데 여기에서 (06는 핵밀도추정(6061 density
estimation) 2] 약자입니다.

1 df.plot.kde()

Out
0.004 +                                               — 전리마마트
~;                                                  — 히드라마트
— quoe

0.003 4

&

= 0.002

8
0.001 4
0.000 4

600     700     800     900     1000    1100    1200    1300    1400

SAAS 그래프와 함께 보여줄 때는 박스 그래프

주가를 표현할 때 종종 사용되는 그래프 중에 박스 그래프가 있습니다. 박스 그래프 자체는 S
계치를 내포하고 있는데, VAS] 맨 위에서부터 각각의 가로줄이 최댓값, 상위 25%값, 중간
값, 하위 25%값, 최숫값을 표시합니다.

=

Se ee SICHZE
상위25%값
중간값
하위25%값
= Le      최소값

14장 코딩 기술: 시각화 295


===== PAGE 296 =====
박스 그래프를 그릴 oe df.plot.box()S 이용합니다.

1  df. plot. box()                                                                           |

WOT ee    =  :  -                     |

Out      1200

1150                                                                                                                                                                          "
1100
1050

1000
950
900
850
x                                                                                      ath                                                  os

전리마마트                        히드라마트                          터렛마트

관계를 표시할 때는 산포도

×값과 VSO] 관계를 알아보는 그래프를 그릴 때는 산포도를 이용합니다. 회귀분석을 할 때
사용했던 그래프가 산포도인데, 각 데이터마다 ×축의 값과 *축의 값을 각각 찾아 점을 찍
가면서 ※축과 *축이 어떤 관계가 있는지를 알아보는 데 도움이 됩니다. 회귀분석은 이렇게
찾아낸 BAS 추세선으로 만들어가는 것이지요.

후

1 df. plot.scatter(x='6|Ce2}O}E’, 1='천리마마트', figsize=(5, 5))

Out

296 4부 옵션


===== PAGE 297 =====
14.3 3D 그래프 그리기
이번에는 있어 보이는 그래프의 끝판왕 3D 그래프입니다. 3D 그래프를 그릴 때는 WSSA
의 추가 기능인 mplot3dS 이용하는데, 통상 다음과 같이 라이브러리를 호출합니다.

1 from mpl_toolkits.mplot3d import Axes3D

Out

앞에서 그렸던 마트 삼총사의 그래프를 3ㅁ로 그려보겠습니다. 4 종목의 주가를 막대 형태의
크래프로 표시하고 3DE 표시합니다. ×축은 기간, 축은 SS, 2축은 가격을 나타내도록 =
리겠습니다. 31 막대그래프를 그릴 때에는 Xe, 높이값(2값), 데이터 구분값(*값)과 함께,
어느 방향으로 데이터를 움직이며 그래프를 그릴지 지정해주어야 합니다. ax.bar (Xz, Za

Yat, zdir=" eet" )처럼 지정합니다.

1 fig = plt.figure(figsize=(8, 6)) # 그래프 를 설정해 710라고 지정
ax = fig.add_subplot(111, projection='3d') # 710를 1행 1열로 지정하고, 서으플롯을 삽입한
후 해당 서브플롯을 3*라고 지정
for 2, n in 210([1, 2, 3], df.columns): # 증목(칼렁)마다 순환
left = df[n].index # X# (xz)
height = df[n].values # 2값 (#0/Z)
25 = 2 # YS (GIO/E] 구분)
ax.bar(left, height, zs, zdir="y', alpha=@.8) # 3D 막대그래프 그리기

N

wo Ont ou fk WW

ax.set_xlabel("SHMt') # XZ O/B 삽입
10 ax.set_ylabel('SS3') # Y2 O/B 삽입
11 ax.set_zlabel('7}24') # Z2 이름 삽입
12

13 ax.legend(df.columns) # Hej] 삽입

148 코딩 기술: 시각화 297



===== PAGE 298 =====
Out
699 천리마마트
mas 히드라마트
000 더렛마트
1200

‘T 1000
7 800
600 A
400
‘T 200

2018-09-01          ——
2018-09-08
201

1행에서는 그래프 사이즈를 포함한 그래프 전체 SS AMAA 10에 할당합니다. 2행에서
110에 서브플롯을 지정하는데, 0060660008 30' an 명시해서 3D 그래프를 그릴 것임
선언합니다. 그리고 지정한 서브플롯을 , axel] 할! 할당합니다.

3~7행은 막대그래프를 하나씩 그리는 부분입니다. 파이썬은 RANE 구분해서 그래프를 그

릴 수는 있지만 문자를 기준으로 그래프를 그리지는 못합니다. 그래서 220 ([1, 2, 3],
0『.0014005 )을 이용해 각 종목에 임의의 숫자 1, 2, 3을 부여해서 이름과 묶어줍니다.

for 2, nin zip([1, 2, 3], df.columns)S 이용해 각 종목을 순환하며, 16 = df[n].
1006×에서 ×축 값을, height = df[n].valueso]A] 2축 값을 지정한 후 3<.0623「 (left,
height, zs, zdir="y', alpha=0.8)S 통해 막대그래프를 그립니다. 여기에서 31.0113=0.8
은 그래프를 반투명하게 그리라는 부가 정보입니다. 1은 완전 불투명하게 그려지고, 0은 완전
투명하게 그려집니다.

9~11행은 각 축의 OSS 삽입하는 부분이고, 마지막 13행은 범례 정보를 표시하는 부분인
니다. 같은 정보임에도 불구하고 31 그래프로 보니 느낌이 많이 다르죠? 뭔가 좀 더 있어 보
인다고 할까요.

이번에는   제 경반음  그려보겠습니다. 3D 막대그래프가 2차원 데이터를 모아서 3차원으로

298 4부 옵션


===== PAGE 299 =====
만든 것이라면, 입체 평면은 처음부터 3차원으로 그림을 그리게 됩니다. 또한 선이 아니라 면
그리는 것이기 때문에 각 축의 값이 이전과 같이 1×1 형태의 한 점이 아니라 2×2 매트릭
형태로 입력되어야 합니다.

uw

fed.
el

A

예를 들어, ×축의 점이 (1, 2, 3), 축의 점이 (4, 5. 6), 2축은 z=x+ "인 경우 이 ASS
그대로 입력하면 파이썬은 ((1.4.5), (2.5.7), (3.6.9))에 AS 찍고 연결하여 하나의 AS
듭니다. 입체 평면을 만들기 위해서는 (((1.4), (1.5), (1.60)0), ((2.4), (2.5), (2.60)), ((3.4),
(3.5), (3.6)) oll 해당하는 매트릭스 전체의 Moll 대해 2값을 계산하고 이들을 연결해야 합니
다. 그래서 입체 BAS 그릴 때에는 xX, 값을 매트릭스 형태로 넣어줘야 합니다.

입체 BAS 그리기 전에 우선 평면에 사용할 컬러맵을 호출합니다. 컬러맵은 WeeHe] 미
리 여러 가지 색 조합을 만들어두어 사용자가 쉽게 사용할 수 있도록 만든 편의 기능입니다.
matplotlib 라이브러리에 있는 cm 클래스를 가져옵니다.

co

1 from matplotlib import cm

Out

이제 입체 평면을 그려볼 차례입니다. 4행에서는 ×축의 범위를 0부터 20까지로 지정합니다.
5행에서는 축의 BPS -10부터 10까지로 지정합니다. 6행의 X, = np.meshgrid (Xx, Y)
는 ※, 의 범위를 섞어서 매트릭스 형태의 범위로 반환하는 과정입니다. 7행에서는 ※, 매
트릭스 각각에 대해 2값을 계산합니다.                                                       |

9행이 실제로 입체 BAS 그리는 부분입니다. 3<.010『_54「[2306 (×, Y, 2)만 입력하면 입
체 평면이 그려지고, 나머지 부분은 데코레이션입니다. 0080=00.54006「에서 평면의 Ay
깔 톤을 지정했고, linewidth=12 평면 위에 그려지는 선분의 FAS, alpha=0.82 평면
의 투명도를 지정합니다. 이어서 surf = ax.plot_surface(X, Y, 2, cmap=cm.summer,
linewidth=1, alpha=0.8 )이라고 입력하여 입체 평면을 54「+에 할당합니다. 할당하지 않아
도 그래프는 그려지지만, 뒤에서 컬러바를 표시할 때 BAT} 컬러바를 연결하기 위해 하는 작
업입니다.

|름을 지정하는 부분이며, 13행에서는 Figo 들어 있는 컬러바를 가져

10~12행은 각 축의 이름을
연결해 화면에 표시해줍니다.

와서 surf 평면과

14장 코딩 기술: 시각화 299



===== PAGE 300 =====
1     fig = plt.figure(figsize=(8, 6)) # 그래프 를 설정해 110라고 지정

2      ax = 19 .902(0「01600【100='30') # figs 1행 1열로 지정하고, 서브플롯을 삽임한 후 해당 서브플
롯을 라고 지정 |] 606 plot

3

4      X = np.arange(®, 20) # X% 범위 지정

5      Y = np.arange(-10, 10) # YS 범위 지정

6     X, Y = np.meshgrid(X, Y) #X, YS 매트릭스로 변환

7      2 = np.sqrt(v**2 +X) # 매트릭스 2} 점마다 2값 계산

8

9     surf = ax.plot_surface(X, Y, 2, cmap=cm.summer, 1106010타=1, alpha=0.8) # 입체 평면 그리

기 및 surfol] 할당
10     ax.set_xlabel('X') # X# 이름 지정
11     ax.set_ylabel('Y') # YS 이름 지정
12     ax.set_zlabel('Z') # 2축 이름 지정
13     fig. Cae IKGuRY  shrink=@.5,  shespects 2)   # 컬러바 BA]

Out

어떤가요? 3D 그래프라 더 있어 보이지 않나요?

지금까지 WEYL 이용해 다양한 그래프를 그리는 방법을 알아봤습니다. 그래프는 많은 데
이터를 시각적으로 나타내서 데이터의 SYS 한눈에 파악하기 HES 만드는 데 그 목적이
있습니다. 데이터 과학에서는 그래프를 잘 그리는 것이 매우 중요하죠. 비단 데이터 과학뿐 아
니라 금융공학에서도 여러 금융상품을 합성해서 신종 금융상품을 만드는 과정에서 손익 분석,
리스크 분석 등을 위해 그래프를 잘 그리는 것은 필수입니다. 금융공학자라면 그래프를 그리
는 방법은 꼭 숙지하고 있어야 하는 기술이죠.

300 4부 옵션


===== PAGE 301 =====
15.1 파이썬으로 구

블랙-슬즈 모형 리뷰
이제 파이썬을 이용해 Baa 모형을 구현하고 옵션가격 및 그릭스 그래프를 그러보겠습
니다. 코딩을 시작하기 전에 먼저 블랙-숄즈 방정식을 복습해봅시다.

C()=5S,N(d,)— Ke" N(d,)
Fe = Ke" N(-d,)- SoN (-d,)

2
inSeefre lr
d, =_

“    oNT

In Se afr—Sr
K       2

oVT

블랙-숄즈 방정식에 표준정규분포, 제곱근, 로그, 지수함수 Sol 포함된 것을 볼 수 있습니
다. 코딩을 시작하면서 블랙-숄즈 방정식에 포함된 연산을 수행하는 데 필요한 라이브러리를
호출합니다.

d, =d,-ovT =

15장 금융공학 모델링 301


===== PAGE 302 =====
from scipy import stats

import numpy as np

import pandas as pd

import matplotlib.pyplot as plt
qustplotle inline

wu & WN RP

Out
1행은 5010 라이브러리를 사용한다는 뜻입니다. 사이파이(60187)는 과학, 통계 관련 기능을
제공합니다. 블랙-숄즈 방정식에 있는 표준정규분포를 구현하는 데 이용합니다.

2행은 배열 형태의 데이터 처리를 위한 넘파이인데, 넘파이의 강력한 기능은 제곱근, 로그 등
고급수학 연산 기능을 함께 제공합니다.
3행은 데이터 처리를 위한 팬더스, 4~5열은 그래프를 그려내기 위한 Weed duct.

잔존만기 계산
먼저 잔존만기를 계산하는 함수를 만듭니다. 이미 소개했듯이 정규 거래소에서 거래되는 금
융상품은 거래가 일어나지 않는 공휴일을 제외한 252일을 1년으로 합니다. 잔존만기는 1년을
3} 채우면 1이고, 만기에 가까워질수록 0으로 다가갑니다.

1 def (106_.10.02141115(10, 1, y=252):

2      10 = pd.to_datetime(t@)
3      T = pd.to_datetime(T)
4     return ( np.busday_count(t®@, 1) / y )
Out
18-2 time_to_maturity 함수를 선언하고 기준일인 tog} 만기일인 TS 인수로 받습니다. 1

AS 252일로 하면 /=252로 기본값을 세팅해놓아 따로 인수를 전달하지 않아도 무방하지만,
년을 365일 또는 다른 숫자로 바꾸고 싶으면 1년을 며칠로 정할지 인수로 함께 지정합니다.

2~3행은 전달받은 인수인 10, TS pd.to_datetime() 함수를 이용해 날짜 형식으로 바꾸
어줍니다. 4행은 잔존만기 값을 계산해서 돌려주는데, 기준일(10)과 만기일(1) 사이의 평일

302 4부 옵션


===== PAGE 303 =====
(\6616031)만을 카운트하기 위해 np.busday_count (t0, T)S 사용하며, 이를 1년 기준 날
짜 수인 로 나누어줍니다.

실제로 time_to_maturity () 함수를 이용해 잔존만기 값을 구해보겠습니다.

그  time_to _maturity(’ 2018- = 1',    '2018- ‘12- 14° )

Out @.38492063492063494

기준일(【0)로 2018-8-1을, 만기일(1)로 2018-12-148 전달해 함수를 호출해보니 결과가
앞의 그림과 같이 출력됩니다.

이제 본격적으로 블랙-숄즈 방정식을 계산하는 함수를 구현해봅니다. 1행은 6311_.0「ㅁ1066 ( )
수를                                 FER] (ttm), 이자율(『), 변동성

|
OF
(~
re
에
에
ky
N
fh
N
x
es
NX
SN)
jy a
a
oot
~
주
NX
Ny
ahs
ae
주

(sigma) 2] 5가지 인수를 받아옵니다.

2~3행은 01, 02를 계산하는 수식입니다. 넘파이 라이브러리에서 가져온 로그(109), 제곱근
(sqrt) 함수를 이용합니다. 02는 4행에 있는 주석처럼 작성해도 동일합니다.

5행은 옵션가격을 계산하는 부분입니다. 표준정규분포의 누적밀도 함수인 N(d,) 계산을 위해
사이파이 라이브러리에서 가져온 9635.00「0ㅁ.007 (01, 0.0, 1.0 )과 같이 작성합니다.

6행은 계산한 옵션가격을 돌려주는 부분입니다.

1 def call_price(S, K, ttm, r, sigma):

2     01 = ( np.log(S / K) + (r + sigma**2 * 0.5) * ttm ) / ( sigma * np.sqrt(ttm) )

3     d2 = ( np.log(S / K) + (r - sigma**2 * @.5) * ttm ) / ( sigma * np.sqrt(ttm) )

4     #td2 = 01 - sigma * sqrt(ttm) 도 같은 수식

5     val = ( 5 * stats.norm.cdf(d1, 0.0, 1.0) ) - K * np.exp( -r * ttm ) * stats.nom.
cdf(d2, @.@, 1.0)

6      return val

154 금융공학 모델링 303



===== PAGE 304 =====
이제 블랙-숄즈 방정식을 이용한 콜옵션가격 계산 함수를 완성했으니 함수를 호출할 때 입력
할 정보인 잔존만기, 이자율, 변동성 값을 ASU.

ttm = time_to_maturity(‘'2018-9-1', '2018-12-14')
r = 0.025

wn pe
4.
3
1
@
더

로
이 값들을 이용해서 6ㅎ11_01「166( ) 함수를 호출합니다. call_price (기초자산, 행사가, 잔
존만기, 이자율, 변동성)의 순서로 입력합니다. 여기에서는 기초자산 가격과 행사가를 모두

—

350으로 입력해봅니다.

1 call_price(350, 350, ttm, r, sigma)

Out 12.631163296464337

옵션가격이 12.63원으로 계산된 AS 확인합니다.

기초자산 및 행사가격 변화에 따른 콜옵션가격 변화
이번에는 기초자산 가격이 변할 때 옵션가격은 어떻게 변하는지를 살펴보기 위하여 5에 변화

때
4
[무기
띠
EG;
id

Amtts 저장하기 위한 덕셔너리를 생성합니다. 242 기초자산 가격 구간을 AAS
데, np.arange (200, 400, 10 )으로 기초자산이 200~400 사이에서 10만큼씩 증가하는,
[200, 210, 220, …, 390]의 배열 구간을 정의한 것입니다. 파이썬에서 구간을 지정하면 앞

의 숫자는 포함하고 뒤의 숫자는 포함하지 않는다는 것은 H 기억하고 있어야 합니다.

ot
lo

19 4 a

1 call_space = dict()

2 S =np.arange(200@, 400, 10)

3 fors 10 5:

4      call_space[s] = call_price(s, 300, ttm, r, sigma)
5

call_space

304 4454


===== PAGE 305 =====
Out {200: 1.82298654176895556-06,
210: 3.72433252296185826-05,
220: 0.00048482193450108749,

—

390: 92. AGT

기초자산 가격은 200~400까지 변하고, 행사가격은 3002) 경우 옵션가격이 어떻게 변하는지
구했습니다.

이번에는 기초자산 가격도 변하고, 행사가격도 변하는 경우를 살펴보겠습니다.

명

2행은 행사가격 구간을 250~350으로, 3행은 기초자산 가격 구간을 200~400으로 정의합니

다.

appa 250~350 구간을 순환하며 5~8행을 반복 실행하도록 설정합니다. 5행
은 각 행사가격에서 사용할 옵션가격 구간을 저장할 딕셔너리를 선언합니다. 6행에서는 행사

이 < AEE DE 0 FS ALU. 7행은 행사가격이 (, 기

초자산 가격이 6일 경우 콜옵션가격을 구하        single_space 딕셔너리에 저장합니다.

oH

[00

f
ia

8행에서는 행사가격 (에 대한 콜옵션가격을 저장한 딕셔너리인 single_spaceS We|~ 시
리즈 형태로 바꾸어 6ㅎ11_508086 딕셔너리의 열에 저장합니다. 9행에서는 완성된 6011 _
space 딕셔너리를 출력합니다.

call_space = dict()
K = np.arange(25@, 350, 10)
5 = np.arange(2@0, 400, 10)
for k in K:
single_space = dict()
for s inS:
single_space[s] = call_price(s, k, ttm, r, sigma)

call_space[k] = pd.Series(single_space)

oO On DN F&F WN BR

call_space

15S 금융공학 모델링 305



===== PAGE 306 =====
Out    (250:    200          0.022213

210              0.135833

220              0.579058
dtype: float64,

260: 200           0.004304
210              @.033756

220              @.180484

—

dtype: float64,

348: 200           1.901492e-10
210       9.308611e-09

220          2.761759e-07

—

dtype: float64}

ARS 잘 출력되긴 했는데, 가독성이 많이 떨어지네요. 이럴 때 유용한 것이 데이터프레임
이죠. 한번 써먹어보겠습니다. 60311_50206를 데이터프레임으로 바꿔서 df_call_spaceo]
저장합니다.

1 df_call_space = pd.DataFrame(call_space)
2 df_call_space

Out       250   260   270   280   290   300    310    320    330    340
200 0.022213 0.004304  0000730 0.000110  0000015  0000002 2051670207 2137537e-08 2078843209  19014926-10
710 0.135833 0.033756 0.007326  0.001405 0.000241 0.000037 5.257695e05 6833560007 8245959008 9 30861109
220° 0579058 «= 0.180484 = 0.049127 0.011791 0.002521 0.000485 8.458891e 05 1355684205 200528506 275175907
230 1825802 «0.697475 0.233416  0068909 0.018095 0.004264 9096275204 1.771610e04 3175612205 5.278307e-05
240 © 4.488751  2051631 0.826690 0.294930 0.093641 0.026655 6855433203 1.605359e-03 3.449005e04 6 247559005

표로 만들어놓고 BU 훨씬 보기 좋아졌네요. 하지만 여전히 부족합니다. 역시 그림이 제일 보
기 좋죠.

15.2 2847/14 그래프 그리기

행사가별 옵션가격 그래프
그래프로 그려보겠습니다. 우선 그래프에서 한글을 사용하기 위해 다음 부분을 추가합니다.

306 4부 옵션


===== PAGE 307 =====
1 ＊ 그래프에서 한글 사용 새팅

2 plt.rcParams['font.family'] = ‘Malgun Gothic’
3 plt.rcParams['font.size'] = 12

4 plt.rcParams[‘axes.unicode_minus’] = False

Out

이제 본격적으로 그래프를 그려보겠습니다.

1행에서 그래프 SS 설정해 [19에 할당합니다. 2행은 『10에 서브플롯을 삽입하고 서브플롯
을 axl] 할당합니다. 3~5행은 각각 행사가격이 200, 300, 310인 경우의 그래프를 3×에 그려
줍니다. 6~7행은 그래프에 축 SS 달아주고, 8행에서 그래프 제목을 달아줍니다. 마지막
으로 9행에서는 범례를 표시할 위치를 지정해줍니다.

fig = plt.figure()

ax = fig.add_subplot(1,1,1)
ax.plot(df_call_space[29@], label="k=290')
ax.plot(df_call_space[3@@], label="k=300')
ax.plot(df_call_space[310@], label="k=310')
ax.set_xlabel('7|AfAt(Underlying) ')
ax.set_ylabel('S3M7}2 (Call Price)')
ax.set_title('SAH7F HX 옵션가격')

ax. Legend(loc='best')

|, 090 69 NH OH 도 09 60 PB

1001 —— k=290
— k=300

Out                      행사가별 옵션가격              |
804 —— k=310                           |

60 +

|
|
|
40 4

284712 (Call Price)

204                                               |
|

200" W225" 250 2058 300i S250 SONNETS  |
기조자산(00060109)

15장 금융공학 모델링 307



===== PAGE 308 =====
그래프가 그려졌습니다. 행사가격이 낮아질수록 콜옵션의 가격이 높아지는 것을 확인할 수 있
습니다. 행사가격이 낮아질수록 SAS 행사할 확률이 높아지기 때문에 그렇습니다.

콜옵션가격 곡

이제 옵션가격을 31 곡면으로 그려보고 싶습니다. 앞에서 만들어 사용했던 0011_0「166( )
함수는 한 점의 값을 입력받고 해당 콜옵션가격을 반환합니다. 그래서 기초자산 가격과 행사
가격이 변하는 구간의 값을 구할 때는 *아를 이용해 한 점씩 순환하며 콜옵션가격을 한 한
eb 구하고 합쳐서 데이터프레임으로 만들었습니다. 아주 번거로운 일이었습니다. 이번에는 +
간으로 한꺼번에 지정해서 해보겠습니다.

앞에서 for 순환문으로 St st 했던 AS for 없이 원샷으로 해봅니다.

1 5 =np.arange(200, 400, 10)

2 call -Price(S,  300,  ttm,  r, sigma)

Out array([ 1.82298654e-06,
4.26409479e-03,
4.44383483e-01,
6.12900719e+00,
2.47864402e+01,
5.24250191e+01,

3.72433252e-05,

2.66557720e-02,
1.27688176e+00,
1.08267114e+01,
3.34483906e+01,
6.22826058e+01,

4.84821935e-04,
1.23806417e-01,
3.03251898e+00,
1.71254243e+01,
4.27536972e+@1,
7.22257937e+@1,

8.22048147e+01, 9.21976056e+01])

앗, 결과가 똑같이 나오네요. 쉽게 할 수 있는 걸
가격도 같이 움직여보겠습니다.

먼 길 돌아서 왔네요. 그러면 이번에는 행사

K = np.arange(25@, 350, 10)
5 = np.arange(200, 400, 10)
call_price(S, K, ttm, r, sigma)

Out

ValueError                        Traceback (most recent call last)

—

ValueError: operands could not be broadcast together with shapes (20,) (10,)

복잡한 에러 vA] Z|7} AS 나오는데 중요한 AS 맨 아래 나와 있습니다. (와 5의 원소 개

308 4부 옵션


===== PAGE 309 =====
수가 달라서 발생한 에러였

습니다. 에러가 나지 않도록 5와 (의 개수를 맞춰보겠습니다. (의

간격을 10에서 5로 줄여서 와 5 모두 20개씩의 데이터 AES 만들어줍니다.

K
S

np.arange(25@, 350, 5)
np.arange(20@, 400, 10)

call -Price(S,  0 ttm; see

Out  가 2.221314346-02,

4.100561946-01,
2.527835876+00,
8.094294326+00,
1.746252776+01,
2.964290426+01,

6.892030346-02,
8.268902646-01,
3.944955256+00,
1.08267114e+01,
2.12748025e+01,
3.410909006+01,

1.804837186-01,

1.508220086+00,
5.796508036+00,
1.396361096+01,
2.535066746+01,
3.871266296+01,

4.342312926+01, 4. So NY,

5

2, 이제 에러가 나지 않네요. 이 데이터로 31 입체 BAS 그려봅니다. 우선 3D 그래프를 그
리기 위한 라이브러리를 호출합니다.

1 from mpl_toolkits.mplot3d import Axes3D

2  From matplot lib import cm

Out

이제 K, SS 모두 20개씩으로 맞춘 데이터를 가지고 입체 BAS 그려봅니다.

^
1

np.arange(25@, 350, 5)
np.arange(2@0, 400, 10)

wn
1

1

call_price(S, K, ttm, r, sigma)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

o ON DOD NT FF WN

surf = ax.plot_surface(S, K, Z, cmap=cm.summer,

rR
=

linewidth=1, antialiased=True, alpha=0.8)

PrP PR
N BP

ax.set_xlabel('7| XZ AfAt(Under lying) ')

15장 금융공학 모델링 309



===== PAGE 310 =====
Out

13 ax.set_ylabel(' {$A}7} 24 (Strkie)')
14 ax.set_zlabel('$M7}24 (Call Price)')
15 ax.set_title( BEM 가격 곡면을 그리고

16

17 fig.colorbar(surf, shrink=0.5, aspect=5)

싶었으나…')

콜옵션 가격

곡면을 그리고 싶었으나.…

숭                  1.0
2
a
3              0.8
Le               0.6
~
Ay
04
au
0.2
0.0

평면이 그러지지 않았네요. (와 5 값을 매트릭스로 입력하지 않아서 평면을 그러내지
입니다. 그럼 평면이 아닌 선으로는 그릴 수
을 그리도록 고쳐봅니다.

있을까요? 평면을 그리는 부분인 9~10행

5

N
1

fig = plt.figure()
= fig.add_subplot(111, projection='3d')

K = np.arange(25@, 358, 5)
np.arange(20@, 400, 10)

call_price(S, K, ttm, r, sigma)

11 ax.set_xlabel(' 7] 2}4t(Underlying) ')
12 ax.set_ylabel(' $4A}7}24 (Strkie)')

310 4부 옵션

surf = ax.plot(S, K, 2, linewidth=5, antialiased=True, alpha=0.8)


===== PAGE 311 =====
—

13 ax.set_zlabel(' SSM 7+74 (Call Price) 0
14 ax.set_title('SSM 가격 선분밖에 못그림')

Out

콜옵션 가격 선분밖에 못그림

|

&

w
o

nN
[=]
괄옵션가격(0211 Price)

=
ㅇ

200               Z
225
50
PR xBI5 300 a
“Underlying 29° 375

9행에서 ax.plot )으로 AS 그려내도록 명령했더니 예쁜 선이 나왔습니다. 매트릭스
가 아닌 점으로 값을 주면 이렇게 와 5가 함께 움직여서 선분밖에 그리지 못하게 되는 것
입니다. 이중 for 순환문으로 BE 값에 대해 BES te 순환시키며 값을 가져오듯 5
와 KS 매트릭스로 만들기 위해서는 00.0ㅁ6509「10( )를 사용해야 합니다. 3행에 (<, 5 =
np.meshgrid(K, 5 )를 추가해봅시다. 그리고 선을 면으로 바꾸기 위해 OBS] ax.plot )을

ax.plot_surface () = 바꿔줍니다.

1   = np.arange(250, 350, 5)

2 S = np.arange(200, 400, 10)

3 K, S=np.meshgrid(K, S) # 매트릭스 만들기

4 2Z=call_price(S, K, ttm, r, sigma)

5

6 fig = plt.figureQ

7 ax = fig.add_subplot(111, projection='3d')

8

9 surf = ax.plot_surface(S, K, Z, cmap=cm.summer,
10                  linewidth=1, antialiased=True, alpha=0.8)
11

12 ax.set_xlabel('7|ZAt4t (Underlying) ')

15장 금융공학 모델링 311



===== PAGE 312 =====
ee ee ee ee

13 ax.set_ylabel(' 84A}7}24 (Strkie) ')

14 ax.set_zlabel('3AM7}2 (Call Price)')
15 ax.set_title(ZEM 가격 곡면')

16

17 fig.colorbar(surf, shrink=0.5, aspect=5)

Out
콜옵션 가

격 곡면

120
100

ㅎ 88

콜옵션가격 곡면이 그려졌습니다. 기초자산 가격이 높을수록 콜옵션가격은 높아지고, 행사가

SF TEE)

격이 낮을수록 콜옵션가격이 높아지는 USS 확인할 수 있습니다.

풋옵션가격 곡면 그리기
이번에는 풋옵션가격 곡면을 그려볼까요? 풋옵션가격 공식을 복슴해봅니다.

[\(Ge))= Ke" N(-d,)- S,N (—d,)

SAS 이용해 풋옵션가격을 구하는 함수 put_price )를 만듭니다.

1 def put_price(S, K, ttm, r, sigma):

2     01 = ( np.log(S / K) + (r + sigma**2 * 0.5) * ttm ) / ( sigma * np.sqrt(ttm) )
3     02 = ( np.log(S / K) + (r - sigma**2 * 0.5) * ttm ) / ( sigma * np.sqrt(ttm) )
4     val = K * np.exp( -r * ttm ) * stats.norm.cdf(-d2, @.0, 1.0) - ( 5 * stats.norm.

cdf(-d1, 0.0, 1.0) )

312 4484


===== PAGE 313 =====
return val

이제 풋옵션가격 곡면을 그려봅니다.

Cy Ty) SS ey MF 2s ) WW te

PPP RP RP RP PR
Ou fk WN RP 으

17

K = np.arange(250, 350, 5)

5 = np.arange(200, 400, 10)

K, S = np.meshgrid(K, 5)

Z = put_price(S, K, ttm, r, sigma)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

surf = ax.plot_surface(S, K, Z, cmap=cm.winter,
linewidth=1, antialiased=True, alpha=@.8)

ax.set_xlabel(' 7| ZApAt(Under lying) ')
ax.set_ylabel(' 8 A}7}24 (Strkie) ' )
ax.set_zlabel(' 2 @M7+4 (Put Price)')
ax.set_title((#SM 가격 곡면')

fig.colorbar(surf, shrink=0.5, aspect=5)

Out

풋옵션 가격 곡면

15장 금융공학 모델링 313

——=



===== PAGE 314 =====
콜옵션 곡면과는 반대로 기초자산 가격이 낮을수록, 행사가격이 높을수록 풋옵션가격이 높아
지는 것을 확인할 수 있습니다.

15.3 BM 그릭스 그래프 그리기

콜옵션 델타 그래프
이번에는 콜옵션의 델타를 구하는 함수를 만들어보겠습니다. 델타 공식은 다음과 같습니다.

We “a   A(call) = N(d,)
| ea).

이 중 콜옵션의 델타를 구하는 Brel call_delta()S 작성합니다.

1 def call_delta(S, K, ttm, r, sigma):

2     01 = ( np.log(S / K) + (r + sigma**2 * 0.5) * ttm ) / ( sigma * np.sqrt(ttm) )
3     val = stats.nomm.cdf(d1, @.0, 1.0)
4      return val

Out

콜옵션 델타를 곡면으로 그려보겠습니다. 델타는 기초자산 가격 변화에 따른 콜옴션가격의 변

화율이므로 잔존만기, 이자율, 변동성 등 다른 변수들은 고정합니다.

K = np.arange(30@, 350, 5)

S = np.arange(20@, 400, 10)

K, S = np.meshgrid(K, S)

Z = call_delta(S, K, 0.38, 0.02, 0.30)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

o On DOD ON FP WN -

surf = ax.plot_surface(S, <, Z, cmap=cm.coolwamn,

linewidth=1, antialiased=True, alpha=0.8)

rary
>

ie

314 445


===== PAGE 315 =====
11
12
13
14
15

ax.set_xlabel('7|Z Aft (Underlying) ')
ax.set_ylabel(' $4 A}7} 24 (Strkie) ')
ax.set_zlabel(' HE}(Delta) ' )
ax.set_title(’HEt 3H')

16
17 fig.colorbar(surf, shrink=0.5, aspect=5)

Out

델타 곡면
오우

| |
eit Lys
|                      2
Cy
a     0.6
a
mu
04
0.2

|

엑셀에서 본 그래프와 비슷한 모양의 그래프가 나왔네요. 기초자산 가격이 높아질수록 1에 가

까워지는 그래프입니다.

감마 그래프

이번에는 감마 그래프를 그려봅니다. 우선 감마 공식을 복습합니다.

감마 함수를 정의하기 전에 우선 N’(x) 를 구해야 할 필요가 있겠네요. 00×(×)로 Bers 만

15장 금융공학 모델링 315



===== PAGE 316 =====
들어봅니다.

1 def ndx(x):
2     return ( np.exp( -1 * x**2 * 6.5 ) / np.sqrt(2 * np.pi) )

Out

감마는 콜과 풋의 공식이 동일해서 따로 구분자 없이 gamma () 함수로 정의합니다.

1 def gamma(S, K, ttm, r, sigma):

2     01 = ( np.log(S / K) + (r + sigma**2 * 6.5) * ttm) / ( sigma * np.sqrt(ttm) )
3     val = ( ndx(d1) ) / ( 5 * sigma * np.sqrt(ttm) )
4      return val

Out

^
1

00.28「2096(300, 305)
00.2「2096(200, 400, 10)

K, 5 = np.meshgrid(K, 5)

Z = gamma(S, K, 0.38, 0.02, 0.30)

wn
1

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d‘)

ow On DN 은 WDN RP

surf = ax.plot_surface(S, K, Z, cmap=cm.summer,

ray
i}

linewidth=1, antialiased=True, alpha=0.8)

ee
N PB

ax.set_xlabel('7| ZA}AF(Underlying) ')
ax.set_ylabel(' SA}7}24 (Strkie)')
ax.set_zlabel(' 감마(63002) ' )
ax.set_title('Z{o} 곡면')

2 82 PP
aon 6 WwW

|e
Ni

fig.colorbar(surf, shrink=@.5, aspect=5)

316 4488



===== PAGE 317 =====
| 0.007
0.006
0.005
0.004
0.003

등가격 주변에서 높은 값을 나타내는 감마 그래프의 형태를 확인합니다.

4N

콜옵션 세타 그래프
시간가치 크기인 세타를 살펴봅니다. 공식은 다음과 같습니다.

‘Cd
©(call) = Se -76 N(d,)

SN'(d)o ,

O( put) =-    Sie

rKe"" N(-d,)

이 중 콜옵션에 대한 AEH call_theta() 함수로 나타내봅니다.

1 def call_theta(S, K, ttm, r, sigma):
2      di = ( np.log(S / K) + (r + sigma**2 * 0.5) * ttm ) / ( sigma * np.sqrt(ttm) )
3      02 = ( np.log(S / K) + (r - sigma**2 * 0.5) * ttm) / ( sigma * np.sqrt(ttm) )
4      val = -1 * ( ( 5 * ndx(d1) * sigma ) / ( 2 * np.sqrt(ttm)) ) - r* K* np.exp(-r*ttm)
* stats.norm.cdf(d2, 0.0, 1.0)
5       return val
Out

153 금융공학 모델링

317



===== PAGE 318 =====
그래프로 그려보겠습니다. 세타만의 특이한 점은 잔존만기가 점점 0에 가까워지면서 그래프
가 변하는 BSS 보여주기 위해 XS 값이 양수(+)에서 0으로 거꾸로 흘러가게 만들어야 한
다는 것입니다.

T = np.arange(1.0@, 0.0, -0.01)

5 = np.arange(35@, 355)

T, S = np.meshgrid(T, S)

Z = call_theta(S, 350, 1, 0.02, 0.30)

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

ow ON DH F&F WN

surf = ax.plot_surface(T, S, Z, cmap=cm. Summer,

rary
as)

linewidth=1, antialiased=True, alpha=0.8)

3 RP
N 0

ax.set_xlabel('2+29F7| (Time to Maturity) ' )
ax.set_ylabel(' 7] A}At (Underlying) ')

ax.Set_zlabel(‘ AJE}(Theta)')

ax.invert_xaxis() # X#S 1부더 0의 순서로 거꾸로 출력
ax.set_title('AJE} 곡면')

PPP PP BP
on DN Bh WW

!
|

fig.colorbar(surf, shrink=@.5, aspect=5)

Out

AEE 곡면

318 4484


===== PAGE 319 =====
것을 볼 수 있습니다.

베가 그래프
베가는 변동성의 변화에 따른 옵션가격의 변화를 나타낸 것입니다. 우선 공식을 복습해봅니다.

vega = ee S,VTN'(d,)
do

—

N (x)=     ene

V2x

베가는 콜과 풋의 구분이 없어 4698 ( )로 함수를 정의합니다.

1 def vega(S, K, ttm, r, sigma):

2     01 = ( np.log(S / K) + (r + sigma**2 * @.5) * ttm ) / ( sigma * np.sqrt(ttm) )
3     02 = ( np.log(S / K) + (r - sigma**2 * @.5) * ttm ) / ( sigma * np.sqrt(ttm) )
4      val = ( 5 * np.sqrt(ttm) * ndx(d1) )

5

return val

Out

그래프로 그려보면 다음과 같습니다.

1 V = np.arange(@.@5, 0.95, 0.01)

2 5 =np.arange(358, 352)

3 V, 5 = np.meshgrid(V, 5)

4 Z = vega(S, 350, 0.38, 6.02, V)

5

6 fig = plt.figure()

7 ax = fig.add_subplot(111, projection='3d')

8

9 surf = ax.plot_surface(V, S, Z, cmap=cm.spring,

10                         linewidth=1, antialiased=True, alpha=@.8)

15S 금융공학 모델링 319



===== PAGE 320 =====
11

12 ax.set_xlabel('H=4 (Volatility) ')

13 ax.set_ylabel('7|ZA}4t(Underlying)')

14 ax.set_zlabel(‘4]7}(Vega)')

15 ax.set_title('H|7} =H")

16

17 ‘fig. colorear (Sul tee shrink=@.5, arse)

Out
베가 곡면

Sor 080

cA           85.0
“78408

Stes 9        84.5
830N             84.0

82.5
820               GEIS
82.5

02      —
feo"          ~  2502 0

변동성이 아주 낮은(10% 미만) 구간에서 베가가 급격히 올라가고, 변동성이 증가함에 따라 베
가가 점점 감소하는 것을 볼 수 있습니다.

지금까지 옵션이란 무엇인지 알아보고, 옵션의 특징  . 음션가적을 dete tie 공부했습니
다. SAS 금융공학의 핵심이자 주인공이며, 거의 대부분의 금융공학 서적이 옵션을 소개하
는 데 지면의 대부분을 Cole 만큼 큼융공학에서 옵션이 차지하는 비중이 큼니다. 그릭
비롯해 어려워 보이는 단어가 많았죠? 옵션은 그래프 없이 이해하기가 거의 불가능할 정도로
어려운 개념이므로 많이 이해하지 못했어도 낙심하지 마세요. 다들 그런 과정을 거치거든요.

이해하는 데 어려움이 없었기를 바랍니다.

320 4부 옵션



===== PAGE 321 =====
찰나의 싸움 HFT

2010년 이후 글로벌 금융시장은 HFT (high-frequency trading)7} 장악하기 시작했
습니다. 영어로는 41ㅠ라는 일관된 용어를 쓰는데, 이전에 국내에서는 영어 직역에 충
실한 기자들이 고주파 매매라고 번역하기도 했습니다. 최근에는 고빈도 매매라고 주로
번역됩니다.

HFTS] 기본은 남보다 빨리 거래소로 SES 쏘는 것부터 시작됩니다. 시세 변화를 먼
저 포착하고, 다른 사람보다 먼저 주문을 낚아채 늦게 오는 사람한테 더 비싼 가격에
되파는 것이 HFT7} 수익을 내는 방식이지요. 주가지수를 기반으로 가격이 변동하는
선물상품을 생각해봅시다. KOSPI200 지수는 2초에 한 번씩 산출되어 발표되고, 투자
자들은 새롭게 발표된 지수를 기준으로 선물에 배팅을 시작합니다. KOSPI200 지수를
산출하는 방법을 알고 있는 HFT 트레이더라면 거래소가 지수를 발표하기 전에 지수를
먼저 산출할 수 있을 것입니다. 그러면 다른 투자자가 지수 발표 후 배팅을 시작하기
전에 먼저 주문을 내서 선물을 확보할 수 있겠지요. 그러고 나서 늦게 들어오는 투자자
들에게 조금 더 비싼 값에 되팔면 됩니다.

현재 지수가 300이고, 선물가격이 302라고 가정해봅시다. 2초 후에 발표될 지수가
301이라는 것을 먼저 계산한 HET 트레이더는 선물가격이 303으로 올라갈 것을 예상
해서 302에 나온 선물을 모두 사들인 후 303에 매도합니다. 낚시를 할 때 물고기가 오
는 길을 미리 파악해서 그물을 치고 기다리고 있다가 그물을 거두어들이는 것과 비슷
한 셈이지요.

지수가 2초마다 발표되는데 그 사이에 어떻게 그런 일이 가능하냐구요? 금융공학을
알고 17 기술을 이용할 자금만 있다면 충분히 가능한 일입니다. 한국시리즈 야구표 예
매도 1초만 늦게 접속하면 원하는 자리를 찾기가 어려운데, 어마어마한 돈이 걸려 있
는 금융시장은 오죽할까요? 현대의 초고속 통신망과 거래소의 고성능 매매 체결 시스
템은 초고속으로 쏟아내는 HET 트레이더의 주문을 무리 없이 수용할 수 있습니다. Al
수들 사이에서는 마이크로초(0.000001초) 단위의 차이로 수익의 희비가 엇갈리고 있
는 것이 현실입니다.

15장 금융공학 모델링

321



===== PAGE 322 =====
그럼 HFTS 주식시장에 나쁜 존재일까요? 「『라이어스 ATS] se, US, 등의 작가
마이클 루이스는 그의 저서 『플래시 보이스』]에서 HFTS] 민낮을 고발했습니다. HFT
트레이더는 남보다 먼저 움직여서 1틱(선물의 경우 0.05)의 마진을 얻는 무위험 거래를
합니다. 선물 1계약을 차익거래 한다면 거래 한 번으로 12,500원(=0.05×250,000원)
을 duc. 거래량이 많아지면 차익은 더 많아지겠죠. 조금 늦게 들어온 일반 투자
자는 같은 상품을 매수하기 위해 그만큼의 돈을 더 지불해야 합니다. 결국 거래 비용이
늘어나게 되어 시장에 전체적으로 나쁜 영향을 초래하는 것입니다.

그러면 왜 현대 금융 시스템은 807가 가능한 거래 환경을 제공할까요? 사실 처음에는
HFTS] 단점보다는 장점이 부각됐습니다. 금융공학으로 무장한 817 트레이더는 일반
투자자들은 잘 발견하지 못하는 새로운 기회를 먼저 발견하고 FES 제출함으로써 이
상품이 Eo] 되는 상품이다라는 시그널을 일반 투자자에게 주었습니다. 일반 투자자는
어려운 금융 공부를 하지 않아도 거라량이 급증하는 상품만을 찾아 다니면서 투자할
수 있으니 누이 좋고 매부 좋은 일이었지요.

주문을 처리하고 매매를 시켜주는 증권사와 거래소는 HPT 트레이더의 ake 거래로
더 많은 수입을 올릴 수 있었습니다. 그래서 증권사는 서로 HPT 트레이더를 유치하
기 위해 자사의 초고속 주문회선을 HET 트레이더에게 전용으로 임대해주고 수수료도
까아주는 경쟁을 하기도 했지요. 2011년 우리나라 증권시장에서 이슈였던 ELwW 초단
타 투자자(스캘퍼) 특혜 제공 사건이 바로 이 사례입니다. 결국 법원에서 무죄 판결을
받기는 했지만 증권사가 초단타 투자자들에게 전용선을 임대해주는 것이 문제가 되어
ELW 시장 전체가 나쁜 시장이라고 손가락질 받는 사건이 있었지요.

법원의 판결처럼 METS 불법이 아닙니다. 많이 공부하고 더 투자해서 높은 수익을

리는 것이니까요. 다만 시장 전체의 거래 비용을 높인다는 치명적인 단점을 극복할
있을지가 관건이지요.

> 0

322 4부 옵션


===== PAGE 323 =====


===== PAGE 324 =====
가공

및

|

집

A?
TT &

1:

이터

술: 더

Li

7



===== PAGE 325 =====
Chapter 16

= 4 fo

=
2
1

조하 At

메

fon)

~

, ETF, ETN, ELW, ELS 이런 용어를 많이 들어보셨다면 당신은 이미 21세기형
조화 ABE (structured ㅁㅁ0040[)에 익숙해진 것입니다. 주식, 채권, 선물, 옵
상품이라고 한다면, 구조화 상품은 기본 상품들을 조합하여 새로운 수익 HAS
만들어낸 상품입니다. 20세기에도 구조화 상품은 있었지만 기업을 상대하는 기관투자자들의
전유물이어서 개인투자자에게는 참여의 기회가 거의 없었습니다.

ro
ic
[>
ct
1

0
ㅁ
0)
ㅇㅇ
ofa
ro
4)

rere
oir
010
N
re

2147] 들어 거래소와 금융기관은 개인투자자의 투자 기회 확대를 위해 상품의 복잡도를 S
이고, 위험을 제한하며, 개인투자자가 접근하기 쉽게 각종 금융 ASS 정비해 개인투자자용
구조화 상품을 출시하게 됩니다. 이러한 상품의 가장 중요한 특징은 개인투자자가 거래하기
쉬워야 한다는 점인데, 이를 위해 거래 단위를 잘게 쪼개서 증권화하고 거래소에 상장시켜 일
반 주식처럼 거래할 수 있도록 합니다.

상품명     풀 네임                       거래 장소
 6    | Exchange Traded Fund          | 거래소
ETN | Exchange TradedNote HRA

ELW | EquityLinked Warrant ss
“ELS | Equity Linked Securities     | Bent

mish ort  Derivatives Linked Securities   |  증권사      |
ELD | EquityLinkedDepost. = | 은령:

16장 펀드와 구조화 상품 개념과 설계 325


===== PAGE 326 =====
액티브 vs. 패시브

벤치마크 지수 이상의 수익률을 목표로 삼고 그때그때 펀드매니저의 판단에 따라 다양한 운
방법을 선택하는 HES 액티브 WE (active fund), 벤치마크 지수를 기준으로 운용 ups
사전에 정의하고 정해진 수익률을 따라가도록 설계해 펀드매니저의 개입 없이 자동으로 운
하는 HES 패시브 WE (passive 14700 )라고 합니다.

:

알파 vs. 베타

금융상품을 운용할 때 비교 대상보다 높은 수익을 추구하는 것을 알파(<), 비교 대상의 수익
률과 유사한 패턴의 수익을 추구하는 것을 베타(6)라고 합니다. 플러스 알파라는 말을 생각해
보면 느낌이 옵니다. 주로 액티브 펀드는 알파, 패시브 펀드는 베타를 추구합니다.

패시브 펀드 중 특정 지수(인덱스, index)S 따라가도록 설계된 펀드를

다. 인덱스 펀드는 KOSPI200 대비 X% 초과수익 또는 (>5171200만큼의 수익을 내겠다고 광
고를 하며 투자자를 모집합니다. 여기에서 KOSP1200 지수를 벤치마크(기준점, benchmark)
라고 합니다. 벤치마크는 주로 주가지수를 선정하는데, 여러 지수를 섞어 새로운 지수
(customized benchmark index)S 만들어서 벤치마크로 삼기도 합니다.

326 54 펀드와 구조화 상품


===== PAGE 327 =====
16.3 펀드의 2, ETF
펀드 중에서 특별히 거래소에 상장되어 거래되는 BSS 817라고 하며, exchange-traded
fund2] 약자입니다.

낮은 수수료

ETFS BES] 꽂이라고 부르는 이유는     ce 가지가 있지만 무엇보다도 수수료가 싸다는 점이
ETFS] 가장 큰 장점입니다. ETFS] 수수료는 대부분 연 1% 미만으로 일반 펀드보다 훨씬 낮
습니다. 어떻게 이렇게 낮은 수수료가 가능할까요? ETFE 대부분 인덱스 펀드로, 설계만 잘
해놓으면 운용하는 데 큰 수고가 들지 않기 때문에 액티브 펀드보다는 수수료가 저렴할 수 있
습니다. 그리고 무엇보다 거래소에 상장된 상품이어서 투자자들이 접근하기 쉽기 때문에 박리
다매로 충분한 수익을 올릴 수 있으며, 별도의 판매 수수료를 지불하지 않아도 되는 이점이 A
습니다.

실시간 매매

ETF7} 아닌 일반 HES 은행이나 증권사 등에서 거래하면 당일 종가로 거래됩니다. 자산운
용사가 당일 장 중     주 주문을 모아서 장 마감 시 한꺼번에 반영하기 때문이죠. 그래서
투자자는 자신이 생각했던 가격에 거래를 할 수가 없습니다. 장 마감 시점에 가격이 어떻게 변
할지는 주문하는 시점에는 알 수가 없으니까요. 심지어 해외 펀드는 일주일 후 종가로 거래되
기도 합니다. 도저히 내 자산이 얼마에 거래되는지 알 수 없는 상황이지요.

하지만 ETFE 거래소에서 일반 주식처럼 거래할 수 있어서 시장에서 거래되는 가격에 바
로 매매할 수 있습니다. 게다가 거래소는 ETFS] 유동성을 보장하기 위하여 [『(유동성 공급자、
liquidity provider)2H= 장치를 만들어났습니다. 인기가 없는 종목들은 SUAS 지정하여
강제로 매도 매수 주문을 내도록 하는 것입니다.

ETF7} 담고 있는 총자산(주식, 채권. 현금 등)가치를 AUM (asset under management)°]2#}32
하며, 이를 총 펀드 좌수로 나뉘서 한 좌당 가치를 계산한 것을 순자산가지, NAV(net asset

16장 펀드와 구조화 상품 개념과 설계 327

emer



===== PAGE 328 =====
8146)라고 합니다. ETF 내에 주식이 800억 원, 채권이 100억 원, 현금이 100억 원이 들어
있다면 AUMS 1천억 원이 되는 것이지요.

이 ETF7} 1천만 주로 나뉘어 있다면 1주당 가격은 1천억 원 1천만 주 = 1만 원이 되는데,
이렇게 1주당 NAVS 계산한 값이 거래의 기준이 되는 기준가가 되며 매일 장 마감 이후
산해서 발표합니다. 하지만 투자자들을 위해 거래가 진행되고 있는 A 중에도 NAV 추정치를
발표하는데 이를 iNAV (inferred net asset value)z}a! 합니다. 즉 iNAVE 펀드가 담고
는 자산 가격을 평가해서 펀드 1주당 가격을 실시간으로 산출한 값입니다. 참고로 펀드에서
주' 대신 '좌라는 표현을 사용합니다. 1천만 주는 1천만 좌라고 부릅니다.

=

que

flr 32

괴리율

ETFS 주식처럼 거래되기 때문에 투자 열기가 과열되거나 저평가될 수도 있습니다. 투자 열
기가 과열되었다는 뜻은 ETFS 수요가 많아져서 가격이 정상 이상으로 올라간다는 뜻입니다.
거래소는 투자자들이 ETFS 적정한 가격에 매매할 수 있도록 정상 가격을 알려주고 있습니
다. ETFS] 정상 가격은 NAVS 표현하고, 괴리율은 시장에서 매매되는 ETF 가격과 NAVY
차이를 비율로 나타낸 것입니다. 운용사가 관리를 잘하는 좋은 81『일수록 괴리율이 작습니다.

16.4 펀드 설계 및 운용
펀드를 설계하고 운용하는 방법을 간단히 살펴보겠습니다.
© 벤치마크 선택: 복제하고자 하는 지수를 선택합니다.
@ 펀드 스타일 결정: 지수형, 리버리지형(2배, 3배), 인버스형(-1배, -2배) 초과수익형
(커버드 콜) 등
@ 펀드 구조화: 원하는 수익률을 달성하기 위해 필요한 운용 방식을 결정합니다.
@ 편입종목 및 비중 결정: 벤치마크 지수의 구성종목 비중대로 펀드에 편입할 종목을 결정
합니다.
© 투자자 모집: WES 광고하고 투자자를 모집해 펀드 자산을 확정합니다.

© 펀드 설정: 펀드 자산으로 편입종목을 비중대로 매입합니다.

328 5부 HOS 구조화 상품


===== PAGE 329 =====
© 리밸런싱: 투자자금이 늘고 줄어들에 대응하여 편입한 주식을 매수 또는 매도합니다.
 펀드 환매: 투자자가 펀드를 해지하면 들고 있던 주식을 매도해 투자자에게 수익을 돌
줍니
펀드가 지수 수익률을 복제하려면 어떻게 해야 할까요? 펀드 자금으로 지수가 구성된 것과 동
일한 비율로 AAS 매입해놓으면 각각의 주식가격의 등락과 관계없이 펀드는 지수 수익률을
그대로 따라갈 수 있습니다. 따라서 지수형 ETRE 벤치마크 지수의 구성종목 편입비중대로
주식을 매수하기만 하면 되기 때문에 설계도 매우 간단합니다.

=

A, B, C, D, E 57] 종목으로 구성된 *5라는 지수가 있고, Zt 종목의 41S] 40%, 30%, 20%,
5%, 5%라면 KSS 추종하는 5 ETFE AS 40%. BS 30%, CS 20%, DS 5%, ES 5% 매입
해놓으면 되는 것입니다.

다만 자산운용사가 실제로 BES 운용할 때에는 비용이 들어가기 때문에 자산을 모두 주식
매입에 사용할 수는 없습니다. 자산의 99% 정도만 주식 매입에 사용하고 1%는 투자자가 환매
를 신청하는 등 이벤트에 대응하기 위하여 현금으로 보유합니다. 현존하는 펀드 중 가장 완벽
하게 지수를 복제했다고 유명한 SPDR S&P500 8177 '(종목명: SPY, NYSE 상장)조차도 현금을
0.09%를 보유하고 있습니다. 이러한 차이는 펀드 수익률과 지수 수익률에 오차가 발생하는
원인이 되는데, 이러한 오차를 `추적오차율'이라고 부릅니다.

5 ETF7} 투자자들에게 100억 US 모집했다면, 펀드매니저는 위에서 설계한 대로 4, B,C,
D, E 종목을 40억, 30억, 20억, 5억, 5억 원씩 매수합니다. 이 과정을 '설정'이라고 합니다.
다음 날 각 주식의 가격이 변동해 A, 8, C, D, ES] 편입비중이 40%, 25%, 20%, 10%, 5%로
변했다면 펀드매니저는 이에 따라 포트폴리오를 조정합니다. 하지만 펀드 자금 규모에 WS]
없다면 펀드매니저는 아무것도 하지 않아도 됩니다. 어제 매수해놓은 주식가격이 변동해 펀
드 내 주식 규모는 자동으로 40억, 25억, 20억, 10억, 5억 원으로 바뀌기 때문입니다. 하지만
펀드에 100억 원이 추가로 들어왔다면, 펀드매니저는 새로 추가된 100억 원으로 40억, 25°,
20억, 10억, 5억 원씩 매수해 편입비중을 맞춰줍니다.

반대로 투자자가 펀드에서 자금을 인출하는 경우를 봅니다. 투자자가 50억 원 환매를 신청하

1 State Street Global Advisory7} 발행하고 `56에서 거래되는 S&P500S 기초로 하는 ETFS 펀드 자산을 모두 주식으로 보유하
고 있는 것으로 유명한 세계 최대의 펀드입니다. https: //us.spdrs.com/etf/spdr-sp-500-etf-SPY 참고.

16장 펀드와 구조화 상품 개념과 설계 329


===== PAGE 330 =====
면, 펀드매니저는 각 주식을 편입비중만큼씩 매도하기 위해 20억, 12.5억, 10억, 5억, 2.5억
원씩 매도해서 현금 50억 원을 확보해 투자자에게 돌려줍니다.

엑셀 실습 BAA) 실제로 지수형 ETFS 설계하고 설정, 환매하는 과정을 실습해보겠습니다.

16.5 레버리지 ETFS! 설계

우리나라에 상장된 레버리지 ETRE 지수 수익률의 2배의 수익률 달성을 목표로 하는 ETF
입니다. 펀드 자금으로 주식만 매수한다면 달성이 불가능한 수익률이지요. 그래서 레버리지
ETFS 파생상품을 함께 이용합니다. 앞선 PENA] 소개했듯이 파생상품은 거래 규모의 일부
인 증거금만 있으면 거래를 할 수 있기 때문입니다.

KOSPI200& 2배로 추적하는 ETFS] 자금이 100억 원이라면, 90억 원으로 KOSPI200 비중
만큼의 주식 또는 지수형 ETFS 매수해서 지수를 0.9배만큼 추적합니다. 남은 10억 원으로
KOSP1200 ASS 1.1배만큼 매수합니다. KOSP1200 선물의 증거금율이 7.5%이기 때문에
8.25억 Woe 선물 포지션을 취할 수 있습니다. 주식에서 나온 0.9배와 선물에서 나온 1.1배
를 더하면 2배의 수익률이 완성됩니다.

해외 거래소에 상장되어 있는 3배, 4배 등 다른 배수의 레버리지 상품도 같은 방식으로 만
어낼 수 있겠지요.

uf

fl

16.6 ELS, DLS, ELD 설계

파생결합증권이라고 이름 BS ELS, DLS, ELD 등은 모두 비슷한 BHO] 구조화 상품인데 어
떤 자산에 투자하느냐, 어느 금융기관에서 취급하느냐에 따른 차이가 있습니다. ELS (equity—
linked security) 주식, 지수 등 현물자산에 투자하는 상품으로 증권사에서 취급합니다.
DLS (derivatives-linked security)= 파생상품에 투자하는 상품이며 역시 증권사가 취급합
니다. ELD(equity-linked deposit)= ELS2} 똑같이 현물자산에 투자하는 상품인데 예금
(0670051[)이라고 불리는 만큼 은행에서 취급합니다. 그럼 이 파생결합증권 중 가장 대표적인
원금보장형 815 상품을 알아보겠습니다.

원금보장형 515는 원금의 대부분(00%이상)을 채권에 투자해 만기 시 원금 100%를 확보하고,

330 5부 펀드와 구조화 싱품



===== PAGE 331 =====
차액을 옵션에 투자해 초과수익을 추구하는 금융상품입니다. 다음 그림처럼 채권에서 나오는
이자로 ELS 원금을 채울 VSS 채권에 투자하고, 나머지 금액으로 리스크를 지는 것입니다.

간단한 ELS 상품의 oS 보겠습니다. 기초자산 수익률이 110~130%인 경우 ELSE 0~20%
만큼의 이자를 제공하고, 기초자산 수익률이 110%에 못 미치면 원금 보장, 130%를 초과하면

20%의 이자를 주는 원금보장형 콜 스프레드(6111 spread)@ ELSE 다음과 같은 수익 곡선을

보이게 됩니다.

ELS return
uw

80          90         100         110         120         130         140         150
0501 200 return

어떻게 하면 이런 수익률을 돌려주는 ELSS 설계할 수 있을까요? ELSS 총 1004 원 모집했
다고 하면 원금의 95%인 95억 원으로 이자율이 5%인 채권을 매수해서 원금 100억 WS 확보
합니다. 그리고 남은 5억 원으로 다음과 같이 콜옵션 매도와 콜옵션 매수를 동시에 취하면 됩
니다. 행사가 110인 콜옵션(초록색)을 매수하고, 동시에 행사가 130인 콜옵션(파란색)을 매도
합니다. 두 콜옵션의 그래프를 더하면 빨간색의 ELS 수익률이 만들어집니다.

16장 펀드와 구조화 상품 개념과 설계 331


===== PAGE 332 =====
25
20
15
10

ELS return
uv

80       90      100      110      120      130      140      150
KOSPI 200 return

332 5부 펀드와 구조화 상품



===== PAGE 333 =====
i=

ㆍ   ines

wg As.                               Chapter 17
퍼드 에셀 A

17.1 K5 펀드 구조화

이번 AEWALE 우리가 만든 KS 인덱스를 이용해 KS HES 구성하고 운용하는 방법을 A
셀을 통해 실습해보겠습니다. 먼저 9.1절에서 만든 KS 인덱스가 저장되어 있는 엑셀 파일을
불러와서 새 시트를 만들고 시트 이름을 WES 바꿔주는 것으로 준비를 시작합니다. 이를
17.1. (5 『400.×15×라는 새로운 이름으로 저장합니다.

| | SS 기본정보 | 일자별 주가 | 일자별 시가종액 | 선물 | 편드 |   9)   |

일자별로 각 종목을 펀드에 나태 담아야 할지 편입비중을 계산해보겠습니다. 제목 행을 다
음 그림과 같이 만들어주고 연속데이터 채우기 기능을 이용해 일자를 252일까지 ABU.

1 |      |            떠 인
2 |

|

}   fe)
APS 추종하는 펀드에서 각 종목의 편입비중은 EST TET 으로 구합니다 지수

의 시가총액과 각 종목의 시가총액은 이미 일자별 시가총액' 시트에서 =P OSS 이 값을
사용합니다. 엑셀 수식으로 나타내면 ='일자별 시가총액' !82/ 일자별 시가총액' !$62입니다.

17장 펀드 엑셀 실습 333


===== PAGE 334 =====
여가 저브

B3 셀에 이 수식을 입력합니다. 지수 전체의 시가총액 ALS 고정하기 위해 6 앞에 $ HAS
붙여놓았습니다.

 일자별 시가종액'!82/'일자별 시가총액'!$62

B3 셀을 복사해 63~+3까지 붙여넣습니다. B3~F3S 선택한 후 오른쪽 아래의 점을 더블클
릭해 연속 데이터 채우기를 이용해 252일까지 데이터를 AUC.

이번에는 지수를 가져옵니다. 제목 행에 '지수를 추가하고 '일자별 시가총액' 시트에서 구해놓
은 지수를 그대로 가져옵니다.

sa    ~ | × vv eh "SAS 시가종액'12

1 6.02% 7.23% 39.52% 7.07% 40.16% 100.00}

B3~G3S 일괄 선택하고 연속 데이터 채우기 기능을 이용해 252일까지 데이터를 ABU ct.
이제 기초공사는 완료되었습니다.

이제부터 본격적으로 펀드 부분입니다. 펀드는 폐쇄형 펀드와 개방형 펀드가 있는데, 폐쇄형
펀드는 최초 설정 이후 약속된 기간 동안 자금이 주가로 유입되거나 빠져나가지 않는 펀드이

334 5부 펀드와 구조화 상품



===== PAGE 335 =====
ee lll

Weaidon}
설정좌수 ㅣ Stns
1,000,000               -      1,000,000

[ 5)*50000 | 100,000 1,100,000

추가 설정, 환매의 최소 단위인 CUE 5만 좌로 정합니다. 0좌부터 25만 좌 사이의 5만 좌 단
위의 임의의 값을 주기 위하여 114 셀에 SRANOBETWEEN (0,5 )*50000를 입력합니다. 환매도
마찬가지로 0좌부터 25만 좌 사이의 5만 좌 단위의 임의의 BS 주기로 하지만, 총 좌수 이
상의 환매는 불가능하므로 총 좌수보다는 작은 값으로 제한하기 위하여 14 셀에 =MIN(I3,
RANDBETWEEN (0,5 )*50000 )를 입력합니다. 전일의 총 좌수에 추가된 설정과 환매된 좌수를
함께 계산해 ]4 셀에 =I3+H4-14S 입력합니다.

(Random)
설정좌수 || SHOWA
1,000,000                   1,000,000

200,000 100,000     1,100,000 |

이 펀드의 기준가는 지수 100을 기준으로 1좌당 1만 원이라고 하겼 겠습니다. 설정좌수가 100

PRLS TL ae          ~? 후

만이고 지수가 100이라면 펀드 전체 AKH(AUM, asset 아사노 013038601600)은 얼마일까
요? (설정좌수)×(기준가) = 1,000,000좌×10,000원 = 10,000,000,000원이 됩니다. 여기

에서 ce) 앞에서 공부했던 INAVE (기준가 )×  eae 구합니다. 지수가 100°]
으으 FT

17장펀드 엑셀 실습 335



===== PAGE 336 =====
면 iNAVE 10,000원이고, 지수가 110이면 iNAV7} 11,000원이 됩니다.

iNAV2} AUMS 구하기 위해 K~L SS 세팅하고 (3 셀에 =10000*G3/6$3 수식을 입력해
iNAVS, L3 ol] =93*3을 입력하고 252일까지 연속 데이터를 Aue.

1: 6 | =10000103/053 |

(Random)

SEES eames EES

17.2 |[<5 펀드 운용

펀드 자금을 모았으면 이제 펀드 자금으로 주식을 매입할 차례입니다. 전체 자산인 AUMS
가지고 4. 8, C, 2. E 종목을 얼만큼씩 사야 할까요? 물론 제일 처음에 구한 각 종목의 비중
만큼 사야 합니다. 주의할 점은 시가총액 기준으로 해당 비중만큼 사는 것이므로 주식 수는 별
도로 계산해주어야 한다는 것입니다. 따라서 해당 비중의 시가총액을 주가로 나누어 주식 수
를 구해야 합니다. 주가는 '일자별 주가" 시트에 들어 있습니다. 일자별 주가 시트에서 같은 날

짜의 종목 주가를 가져와 시가총액 비중을 나뉘줍니다.

각 날짜마다의 구성종목 AAS 위해 M~Q 열에 일자별 매매 내역` 칸을 만들고 각 SBS 할
당합니다. 그리고 M3 Aol] 수식 =$L3*B3/' 일자별 주가' !82를 입력합니다.

엔터

[Enter]S 누르면 계산 결과가 소수점 둘째 자리까지 나오는데, 지금까지와는 다르게 여기에
서는 BY 버튼을 눌러 소수점을 없애줘야 합니다. 주식은 소수점 단위로 살 수 없으니까요.
M3 셀을 복사해서 <23까지 채워줍니다.

336 5부 펀드와 구조화 상품

이


===== PAGE 337 =====
일자별 매매 내역을 완성했으면, 당일의 매매 내역이 반영된 주식 잔고를 계산합니다. R~V
열에 A) 잔고 코너를 만들고 각 SSS 할당합니다. 아직은 첫날이라 1일 차 매매 내역만
반영하면 됩니다. M~Q AS 그대로 복사해오기 위해 R3 셀에 =43를 입력한 후 \3 셀까지
복사합니다.

첫째 날의 주식 잔고가 채워졌습니다.

둘째 날부터는 조금 다릅니다. 첫째 날은 AUM 전액을 매수해야 했다면, 둘째 날부터는 차액
만큼만 매매를 하게 됩니다. 따라서 새로운 40)4을 기준으로 전체 주식 잔고를 계산한 후 oF
제 잔고를 차감하고 남은 만큼 주식을 매수하면 됩니다. 이를 수식으로 입력하면 =$14*84/'

~

일자별 주가' !83-펀드!063이 됩니다.

17장 펀드 엑셀 실습 337



===== PAGE 338 =====
rene

ete wi 9

  [  00924

일자별  주가 183-펀드!03|  |

일자별 매매내역
AAT     6건설     <증권     ㅁ와학     엔터
10,000,000,000 60,241 36,145 131,727 7,068 4016 |
|__11,021,060,980 |펀드63 | 3,614  13.173 707     402

ㅜㅜ

앞의 그림을 보면 둘째 날 지수(6열)가 빠져 98.17이 되어 144ㅅ\(열)는 9,817원으로 Yo
졌지만, 10만 주의 추가 설정이 발생([1~1열)해 408^(Ｌ열)은 오히려 높아진 것을 볼 수 있습
니다. 따라서 늘어난 자산 규모만큼 주식을 추가 매입해야 하는 상황입니다. 새로운 AUMS
기준으로 각 종목의 주식 잔고를 계산하고, 전일 잔고와의 차이만큼을 매매합니다.

주식 ASE 전일의 주식 잔고에 당일자의 매매 내역을 더해주면 됩니다. ra 셀에 수식
=8#34444을 입력합니다.

Xo _ fe [=r]

^전자    6건설      증      ㅁ화학    엔터
60.241  36,145 _ 131,727    7,068    4,016 |
|  66,265 | 39,759 144900 7,775 4,418 —

이제 M4~v4 셀을 한꺼번에 선택해서 252일까지 채워주면 펀드 모델은 완성됩니다.
AGS 마친 결과 예시 파일은 17.1. KS Fund (실습결과-데이터고정) .×15×입니다.

지금까지 엑셀을 이용해 K5 펀드 모델을 만들어보며 인덱스를 기반으로 Wes 구성하고 운
용하는 방법을 실습했습니다.

338 5¥ 펀드와 구조화 상품



===== PAGE 339 =====
18.1 문자열 WHS 찾아주는 re

인터넷에서 자료를 수집하고 사용자의 용도에 맞추어 스크랩하는 일은 금융공학, 빅데이터,
머신러닝 등 파이썬 프로그래밍을 할 때 빼놓을 수 없는 과정입니다. 수집한 자료에서 원하는
부분만을 골라내서 정제된 데이터로 만들 때 유용한 라이브러리가 「6입니다. 비단 파이썬뿐
아니라 C, 자바 등 일반적인 프로그래밍 언어에서 SEALS 문자열 조작에 쓰이는 정규 표
@A] (regular expression)°]2H= 것이 정의되어 있는데, WAS 정의해서 문자열을 분석하
는 작업에 사용됩니다. 여기에서는 re 라이브러리를 이용해서 정규 HAAS 사용하는 방법
을 알아보겠습니다.

우선 정규 표현식 모듈 사용을 위해 re 라이브러리를 호출합니다.

1 import re

Out

184 코딩 기술: 데이터 수집 및 가공 339


===== PAGE 340 =====
re 명령어
[에서 사용하는 명령어를 알아봅니다.

eee ㄱㄱ
문자열의 시작이 패턴과 일치하는지 조사합니다.

일치하면 해당 인덱스를. 일치하지 않으면 NoneS 반환합니다.

문자열 전체에서 패턴과 일치하는 부분이 있는지 조사합니다.

일치하는 부분이 있으면 첫 인덱스를, 없으면 NoneS 반환합니다.

문자열에서 패턴과 일치하는 SHS 도두 찾아냄니다.

찾은 부분을 리스트로 반환합니다.

문자열을 구분자 기준으로 자릅니다.

잘라낸 각각의 문자열을 리스트로 반환합니다.

문자열에서 패턴을 찾아 CHIE HBLICL

바꾼 문자열을 반환합니다.

패턴을 미리 해석합니다. 복잡한 패턴을 사전에 정의해놓고 사용하는 경우 코
드 가독성이 높아집니다.

「6.02다(패턴, 문자열)

re.search(HHH, 문자열)

「6.+7100211(패턴, 문자열)

「6.5011(구분자, 문자열)

「6.540(패턴, 대체문자, 문자열)

「6.0000116(패턴)

re.search('BC', '46006' )라고 명령하면 파이썬은 문자열 'ABCDE' 중 'BC'7} 들어 있는
인덱스인 (1, 3)을 반환합니다. Slzte]Z] 않도록 다시 한번 파이썬의 인덱스 규칙을 복습하자
면, 첫 위치는 0으로 시작하고, 앞의 위치는 포함, 뒤의 위치는 불포함입니다. (1, 3)인 경우
두 번째부터 세 번째까지 문자를 Zhe] ct.

문자열의 시작을 검사하는 match
우선 실습을 위한 문자열을 만듭니다.

트는 552 SNS SA TS SAS NS
Out

먼저 문자열 stro] '이사원'으로 시작하는지 검사해봅시다. 여러 방법이 있지만 여기에서는
match 사용하겠습니다.

340 5부 펀드와 구조화 상품


===== PAGE 341 =====
__1 re.match(‘O|APS!', str) # strO/ '이사원'으로 시작되어 인덱스 (0.3)을 반환

Qut <_sre.SRE_Match object; span=(@, 3), match='O|'>

당연히 아니라고 나오겠지만 AGS 위해 문자열이 '오대리'로 시작하는지 검사합니다.

1 「6.08대('오대리', str) # str& '오대리'로 시작되지 않아 반환값이 없음

Out

|
|
|

문자열은 '이사원로 시작하므로 '오대리'로 시작하는지 검사한 결과의 Azle] 나오지 않습
니다.

문자열 내에 패턴이 있는지를 ZAISk= search
searchi= 08대와는 다르게 시작점부터 검사하는 것이 아니고 문자열 전체를 검사합니다.
그리고 해당 패턴이 처음 나타나는 인덱스를 반환합니다.

1 「6.560「대('이사원', str) # 문자열0/ 처음 나오는 인덱스 (0,3/을 반환
Qut <_sre.SRE_Match object; span=(@, 3), match='O|A}?l'>

찾으려는 패턴인 '이사원이 우연히도 문자열 w 앞에 위치하네요. 그래서 (0.3) 값이 반환됐
습니다.

1 re.search('2tH2]', str) # 문자열이 처음 나오는 인덱스 (4,7)을 반환

Qut <_sre.SRE_Match object; span=(4, 7), match='2C}e|'>

즈

08『대로 검사한 때와는 다르게 '오대리' 패턴을 찾아내서 그 인덱스를 반환해줍니다.

모두 다 찾으려면 10011
을 땐 710031을 사용합니다.

18장 코딩 기술: 데이터 수집 및 가공 341

|
|
|



===== PAGE 342 =====
1 re.findall(‘2', str)

Out ['3', '장', '장']

과장. 차장, 부장에 각각 들어 있는 문자 '장'을 모조리 찾았습니다.

문자열을 분해하는 6ㅁ0!

이번에는 '쉼표(, )S 기준으로 각 멤버를 분리해봅시다.

1 words = re.split(',’, str) #,3 기준으로 문자열 분리해서 words 리스트에 당기
2 words

Out ['이사원', '오대리', '구과장', '육차장', '정부장']

분리된 각각의 문자열은 40「05라는 리스트에 담겨 있기 때문에 하나씩 불러내서 쓰기 편하게
됐습니다. 리스트의 두 번째 멤버를 불러와봅니다.

1 words[1]
Out '오대리'

여러 음절 중 원하는 패턴이 들어 있는 음절 찾기

이번에는 words 리스트의 멤버 중에서 '장'이라는 문자가 포함된 멤버만 추려내봅시다. 리스
트의 멤버들을 일일이 점검하기 위해 for 순환문을 이용해 멤버들을 하나씩 순환하며 찾고자
하는 패턴인 '장'이 포함되어 있으면 출력합니다.

1 for w in words:

2     if re.search('2', w): # 장으로 끝나는 BHO 표시
3         print(w)
Out 구과장
육차장
정부장

342 5부 펀드와 구조화 상품


===== PAGE 343 =====
특정 문자를 바꿔주는 sub
문자열에서 원하는 패턴을 찾아서 다른 형태로 바꿀 때는 sud (substitute)S 이용합니다. str
문자열에서 숫자로 읽히는 문자들을 숫자로 바꿔봅니다.

1 str = 「6.500('구', '9', str) # '구'를 숫자로 변화
2 str =re.sub('2', '5', str) # '오'를 숫자로 변환
3 str =re.sub('O|', '2', str) # ‘'O/'3 숫자로 변환
4 str =re.sub('S', '6', str) # '육'을 숫자로 변환
5005

Out  2사원, .5대리, 9과장,6차장,정부징 '

oe 익히는 데 의의를 BIC.

좀 억지스러운 여

패턴 정의하기

reo] 기본 기능을 익혔으니, 패턴을 정의하는 방법을 본격적으로 알아보겠습니다. 지금까지
는 패턴을 정의할 때 '' 속에 하나의 단어(예: 장, 오대리 등)를 넣어 같은 패턴이 있는지를 찾
았습니다. ' '로 정의된 패턴은 정확히 똑같은 문자열의 형태가 존재해야 매칭이 됩니다. 하지
만 SC] 융통성 있게 패턴을 정의할 수도 있습니다. [] 속에 문자를 여러 개 넣으면 이 중 하
나라도 같은 형태가 있다면 HAS 합니다. 실습을 위해 5나에서 숫자를 찾아봅시다. 숫자는
0~9까지의 10개 문자만 정의해주면 되니 ' ' 속에 10개의 숫자를 넣어봅니다.

우선 [] 없이 '' 속에 바로 넣어봅니다.

그  re.findall(' 0123456789" » str)
Out  a

fulo
+
zo,
rir
»
ro
LE

strol] 01234567897} 통째로 패턴으로 인식되기 때문에 같은 문자열을 찾
다. 이번에는 [] 속에 숫자를 넣어보겠습니다.

1 re.findall('[@123456789]', str)
OUG e255 5 95, 56.)

183 코딩 기술: 데이터 수집 및 가공 343

| oa


===== PAGE 344 =====
는 문자 중 하나라도 같

숫자들이 튀어나오네요. 이렇게 [] 속에 문자를 넣어주면 [] 속에 있
있으면 매칭하는. 즉 숫자는 모

은 패턴이 발견되면 찾아줍니다. 위 예제는 0~9 중 아무거나
두 찾는 패턴입니다.

0~9, ^ㅅ~2와 연속된 BAAS 좀 더 편하게 정의하도록 구간 사이에 '-'를 넣어서 간단히 표
현할 수도 있습니다.

1 re.findall(‘[@-9]', str)

Out ['2', '5', '9', '6']

[] 없이 숫자를 다 가져오려면 orS 의미하는 | 기호를 이용할 수도 있습니다.

1 re. -findall(’ 11 2}314151617;819',  _str)

Out lee,   “+5, 9",  6']          =    a
하지만 []이 훨씬 효율적이지요. 그리고 두 개 이상의 문자가 붙어 있다면 의미가 달라집니
다. str 문자열에서 과장, 차장, 부장 직급을 찾아오려면 어떻게 할까요?

1 「6.1100811('과장|차장|부장', str)
Out ['과장',  지정: 부장'1

하지만 여기에 []가 적용되면 결과는 달라집니다.

1  「6.1100011('[과장|차장|부장]', 56)
Out [과', '장', ‘ar, '장', '부', '장']

'과장|차장|부장'이 [] 안에 들어가면서 과, 장, 차, 장, 부, 장이 각각 개별적인 문자열로

되어 결국 (6. 10021 ( ' [과차부장] ' , 5『 )과 동일한 표현이 됩니다.

패턴을 정의할 때 ' ' 속에 []를 적절히 섞어 사용해야 원하는 패턴을 정의할 수 있습니다. At
소하지만 아주 중요한 기술인데, WAS 정의할 때 '' 안에 의도되지 않은 공백을 넣으면 et
됩니다. 공백조차도 패턴으로 인식되어 원하는 AAS 얻지 못할 수도 있습니다. 패턴을 정
의할 때는 띄어쓰기 하지 마세요!

344 5부 펀드와 구조화 상품


===== PAGE 345 =====
18.2 데이터 정제

인터넷에서 수집해온 페이지에서 원하는 데이터를 뽑아내는 데이터 정제를 하기 위해서는 우
선 페이지 내의 문장 전체를 음절별로 분해하고 각 음절에서 원하는 데이터의 패턴과 비교해
매칭되는 데이터를 뽑아내는 작업을 합니다. 여기에서는 5ㅠ을 , 를 기준으로 음절별로 분해
한 후에 원하는 데이터를 뽑아내겠습니다.

우선 str-& 각 음절로 분해해 0ㅁ005라는 리스트에 담습니다.

1 0005 = re.split(',', str) #¢,3 기준으로 문자열 분리해서 0075리스트에 당기

2 04005

Out  CA, , “scl , '9과장', '6차장', '정부장']

5명의 직원 중에 Jo] 숫자로 표시된 멤버를 뽑아봅시다. 0005 리스트를 순환하며 각 음절에
숫자가 포함된 SAS 찾아 출력합니다.

for n in 0405:
if re.search('[@-9]', 0): # 숫자가 포함된 직급만 표시

print(n)
Out 2사원
5대리
9과장
6차장
이번에는 과장 이상 직급의 직원을 뽑아봅시다. 과장 이상 직급에는 다 '장'이 붙는다는 패턴

이 있네요. 0005 리스트를 순환하며 각 음절에 '장'이라는 패턴이 er 음절을 찾아 출력합
니다.

1 for n in nums:
if re.search('2t', 0): # 숫자가 BSE 직급만 표시
3         print(n)
Out 92}
6차장
정부장

18장 코딩 기술: 데이터 수집 및 가공 345



===== PAGE 346 =====
가벼

문자열 내에 동일한 구문이 반복되는 경우, 반복 연산자를 이용해 쉽게 데이터를 찾을 수 있습
니다. 우선 실습을 위한 문자열을 정의합니다.

1 SUS [a B',  "BA', "BAAA', ‘BAAAAA’, ‘CBA’, ‘CBABA', 'CBABABA']

str] 멤버 중에서 '84&'가 포함된 BASS 모두 ZloRslch search 기능을 이용해 str
문자열을 하나씩 검사하며 패턴 '84&'가 있는지 검사합니다.

1 for s in str:
2     if re.search('BA', 5):
3         00063

'84' 가 포함된 문자열을 모두 찾았습니다.

이번에는 '84' 이후 두 개의 문자가 추가되는 '840ㅁ' 형태의 패턴을 찾아봅시다. 정규 표

현식에서 임의의 문자 하나를 표현하는 ~  다. '8&ㅁㅁ'는 임의의 문자 두 개가
들어가니 '84. . '라고 표현해보겠습니

1 for 5 in str:
2     if re.search('BA..', s): # BA
3         print(s)

Out BAAA

CBABABA

'84' 이후 두 개 이상의 문자가 붙은 문자열을 모두 찾았습니다. 이번에는 '8400ㅁㅁ' 를 찾
아봅시다.

346 54 펀드와 구조화 상품


===== PAGE 347 =====
1 for s in str:
2      if re.search('BA...', s):  # BA
3          print(s)

이렇게 임의의 문자로 글자 수를 조절해가며 찾을 수도 있지만. 특정 문자를 정해주고 찾을 수

도 있습니다. 특정 문자를 정하는 경우에는 문자를 지정한 후 *, +, {} SS 이용합니다.

a | = 9재때

+        13] 이상 반복           BA+: BA, BAA, BAAA, -~
?        1회 이하 반복           BA?: B, BA
BA{2,4}: BAA, BAAA, BAAAA
     차라         BA{2}: BAA
{m,n}         회 이상, ㅁ회 이하 반복
BA{2,}: BAA, BAAA, BAAAA, =
BA{,2}: B, BA, BAA

'*' 기호를 실습해봅니다.

for 5 in str:
if re.search('BA*', s): # 8 다음에 4가 0회 이상 반복
3         print(s)

Out

&가 0회 이상 반복이므로 《가 하나도 없는 BE 잡아옵니다. 반면 '+'는 하나라도 있어야 잡아
옵니다.

18장 코딩 기술: 데이터 수집 및 가공 347



===== PAGE 348 =====
1 for 5 in str:
2      if re.search('BA+', 5): # 8 다음에 4가 13] 이상 반복
3          print(s)

Out BA
BAAA
BAAAAA
CBA
CBABA
CBABABA

{m,n} = 반복 횟수를 정해줍니다. 0, 1 중 하나를 생략할 수도 있습니다. 4{2}는 AS 23)
반복, 4{2, }는 AS 2회 이상 반복, AL, 2}는 AS 2회까지 반복한다는 뜻입니다.

1 for s in str:                           >
2 if re.search('BA{2,3}', s):   #6 Che 4가 28] 이상 38] eas
3        print(s)           Do a ee
Out BAAA                                                 Ss
BAAAAA
이번에는 841{3}입니다.

1 for 5 in str:
2      if re.search('BA{3}', s): #8 Che A7} 33] 반복
3          print(s)
Out BAAA
BAAAAA
8 다음 4가 33] 반복되는 '8444'가 포함된 문자열을 모두 찾아옵니다. 그러면 Bay} 통째로
반복되게 패턴을 만들려면 어떻게 할까요? ( )를 이용해서 BAS 묶어주면 됩니다.

1 for 5 in str:

2      if re.search('(BA){3}', 5): # BAS 38] 반복
3         print(s)
Out CBABABA

348 SH 펀드와 구조화 상품


===== PAGE 349 =====
ㅠㅜ >

문자열의 시작과 BS 지정해서 더 효율적으로 검색할 수 있습니다. BA} 들어간 문자열
는 예제를 다시 보겠습니다.

filo
pal

1 for s in str:
2     if re.search('BA’, 5):

3                    print(s)

앞의 예제에서 문자열이 CH 시작되는 아래 세 S 말고 BS 시작되는 것들만 찾아오려면 어떻
게 해야 할까요? 다시 말해 문자열 가운데 아무데서나 패턴을 발견하는 것이 아니고 문자열의
Al 부분에서만 HAS 찾으려면, 우리가 이미 학습한 matchS 사용할 수 있습니다. 하지만 편
의를 위해 패턴 앞  0 로

~
acts

—_

1: for s)inistr:
2      if re.search('*BA', 5): # BA& 시작
3         print(s)

Out BA

BAAA
BAAAAA

패턴 앞에 '^'를 붙이는 대신 searchS matchs 바꿔도 동일한 결과가 나옵니다.                                |

1 fors in str:
2      if re.match('BA', 5): # BAZ 시작
3         print(s)
Out BA
BAAA
BAAAAA

188 코딩 기술: 데이터 수집 및 가공 349


===== PAGE 350 =====
———

그러면 844, BAAAAY 늘어지지 않고 BAR 딱 끝       문자열을 찾으려면 어떻게 할까요? 패
턴의 마지막에 '$'를 붙여주면 문장의 끝에서 다 찾습니다.

1 for 5 in str:
2     if re.search('BA$', s): # BAS 끝남
3         print(s)

마무리하는 기분으로 '^'와 '$' 를 모두 사용해 딱 BARE 찾아봅시다.

1 1어52410 str:

2     if re.search('*BA$', 5): # 84로 시작하고 BAS 끝남
3         print(s)
Out BA

BALLS 타깃으로 한 문자열 검색이었습니다.

18.3 핸드폰 HS 검색

지금까지 내용을 종합해 문자열 중 핸드폰 번호를 골라내는 실습을 해봅시다. 우선 전화번호
리스트를 만들고 전화번호로 매칭할 수 있는 패턴을 미리 정의합니다. 핸드폰 번호 패턴이 복
잡하므로 (6.0000116을 이용해 패턴을 미리 정의하고 01006_08【6에 저장합니다.

ET eee.
… ~

1 phone = ['010-1111-2222' , '01012345678', '010 5555 7777',
2           '0709999-0000', '010.2222~5555', '02-3774-3774']
3  phone_pattern = re.compile('010[-~= \.]?[@-9]{4}[-—= \.]?[0-9]{4}')

Out

핸드폰 번호 패턴을 정의하는 방법입니다.

350 5부 펀드와 구조화 상품


===== PAGE 351 =====
aa

© 핸드폰 인식 번호 010 : 핸드폰 번호는 010으로 시작하므로 패턴을 010으로 시작합니다.

@ 번호 사이 공백 [-~= \.]? :       사이의 기호는 -, ~, =, 공백 등 사람마다 각각 다르
게 입력하므로 가능한 ee 모두 고려합니다. 각 기호는 OR 조건으로 취급되므로 I
속에 넣어줍니다. 공백을 명시적으로 입력하기 위해 ' '를 넣은 것을 주의해주세요.

@ [-~= \.]? : '.,'은 임의의 문자를 의미하는 특수기호라 그냥 넣어주면 파이썬이 제대
로 인식할 수 없습니다. 특수기호를 넣을 때는 '\'를 앞에 병기해서 '\. '처럼 표시합니
다.         ee

@ [w= \. TK QE 08 또는 18) PWR: 경우를 검사합니다. []?는 [] 안의 내용이 0
회 또는 1회 발생할 수 있다는 의미입니다.

© 중간 및 끝 번호 [0-9]{4} : 숫자가 4번 반복된다는 의미입니다.

그럼 phone_pattern& 이용해 핸드폰 WSS 간주되는 번호만 주려봅니다.

1 for p in phone:
2      if phone_pattern.search(p):
3         Beane (p)

Out @10-1111-2222
01012345678
010 5555 7777
@10.2222~5555

총 6개의 전화번호 중 0102S 시작하는 4개가 핸드폰 번호로 인식되었습니다. 이 번호들을
깔끔하게 정리해봅니다.

1 for p in phone:

2      if phone_pattern.search(p):
3        p = re.sub('[*0-9]', '', 0) _＊ 10 도 같은 표현

4        print(p[:3] + ‘-' + p[3:7] + ‘-' + p[7:])

Out @10-1111-2222
010-1234-5678
@10-5555-7777
@10-2222-5555

183 코딩 기술: 데이터 수집 및 가공 354



===== PAGE 352 =====
3행에서 보는 HAS 새롭습니다. [] 안에 ^가 들어갔네요. ' '에 바로 ^가 나타나면 문장의
시작을 Ol) ee ^는 NOTES 의바합니다. [^0-91라고 표시되면 숫자가
아닌 것들을 찾아내는 패턴이지요. 3행에서는 숫자가 아닌 것들을 찾아서 지워버립니다. 대체
문자열 ' '에 공백이 들어가지 않았음에 주의하세요.

18.4 간편식을 O1SSt 패턴 정의
[0-9A-Za-z] = 문자와 숫자를 한꺼번에 정의할 수 있었지요? 파이썬에서는 이렇게 자주 A}
용되는 WAS 미리 정의해서 간편하게 사용할 수 있도록 해두었습니다.

af (0-9)                 숫자

\D [| [70-9]          숫자제외 전체
\w       [A-Za-z0-9]      문자+숫자
\                [“A-Za-z0-9]             문자와 RAS 제외한 전체
\ \s            [ \t\n\rJ              공백 (스페이스, 탭, 엔터 등)
\s              9                         공백 제외 전체
실습을 통해 확인해봅시다.
1 str = ‘ABcd12!@ 가나'
2 print('A} :', re.findall('\d', str))
3 print('4e2X :', re.findall('\D', str))
4 print(’#A} :', re.findall('\w', str))
5 print('#A}X :', re.findall('\w', str))
6 print('S'4 :', re.findall(‘'\s', str))
7

print(’S44x :", re.findall('\s', str))

Ou tsscATe ale a
RARE RIGAG MAB 16270007 1 eN@s,) ope 나]
ATO MAU MBIsacupa du 나 02독 MOT. (바디

PAK: ['!', '@', 6 7

공백 : [' ']

EXC HIMAM BES ACL ACIgmd NDS 니 168 "가! 나]

352 5부 HOS} 구조화 상품



===== PAGE 353 =====
정제 작업은 생선 가시를 발라내듯 귀찮은 작업입니다. 위에 소개

: 한꺼번에 발라내는 것처럼 좀 더 쉽게 문자열을 정제하는 치트키와 캠
18장 코딩 기술: 데이



===== PAGE 354 =====
19.1 대한민국 대표 펀드 따라잡기

의번에는 우리가 이전 AeA] 만든 10 인덱스를 이용해 인덱스 펀드를 만들고 운용하는
모델을 만들어봅시다. 우리가 만드는 펀드는 10 종목을 포트폴리오로 편입하고 벤치마크는
\@501200입니다. 즉, 한국거래소의 상위 10개 종목만 이용해서 KOSPI200 인덱스의 수익

률을 따라가려는 펀드입니다. ^
본격적으로 펀드 AAS 하기 전에 우리나라 대표 펀드인 KODEX2007} TIGER2002] 투
자설명서를 참고해봅시다. KODEX2002] 투자설명서는 삼성자산운용 웹사이트(11105: //
\4\.(006×.ㅇ00)에서, TIGER2002] 투자설명서는 미래에셋자산운용 웹사이트(|11105: //
www. tigeretf.com)]A] 다운받을 수 있습니다. 투자설명서에는 이 펀드를 어떻게 운용하
는지에 대한 방법이 설명되어 있습니다.

펀드의 수익률을 어떻게 할지에 대한 항목인 투자 목적 부분을 살펴봅니다. 두 펀드 모두
KOSPI200 지수의 변동률과 유사하게 운용하는 것을 목적으로 합니다. S KOSPI200 지수
가 움직이는 만큼만 수익을 내겠다는 것입니다. 그럼 어떻게 이런 수익률을 Syst 수 있을까
요? 투자 전략 부분에서 그 방법이 설명되는데, 펀드 자산의 95% 이상을 KOSPI200 지수 구
성종목인 주식을 매수해서 지수 수익률을 달성하는 방법입니다. 물론 주식을 매수할 때 지수
구성 비율만큼 매수해야 정확하게 지수를 추적할 수 있겠지요.

지수 수익률을 복제하는 방법 중 가장 대표적인 두 가지는 지수 구성종목 주식을 그대로 보유

354 5부 펀드와 구조화 상품

Zo


===== PAGE 355 =====
에

Ke 방법과 지수 선물을 보유하는 방법입니다. KODEX200, TIGER200 모두 주식을 보유하
방법으로 수익률을 좋습니다. 자산의 60% 이상을 주식에 투자해야만 하는 주식형 펀드이
때문입니다. 선물로 수익률을 복제하는 파생형 펀드가 되면 자산을 굴리는 방법이 더 다양
해지는 장점이 있는 반면, 자산 모집에 한계가 있습니다. 퇴직연금, RP 같은 안전자산은 파생
자가 불가능하기 때문입니다.

그러면 펀드 포트폴리오를 크게 조정하는 리밸런싱은 언제 일어날까요? 두 회사 모두 투자
설명서에서 지수 구성종목이 바뀌면 정기적인 리밸런싱을 하고, 이외에는 지수 구성종목 AP
장회사가 부도 등으로 문제가 생기는 경우에 한다고 되어 있습니다. 우리나라 200대 기업인
KOSPI200 구성종목은 부도 AM] 적은 것을 감안하면 실제로 1년에 한 번 지수 구성종목이

정기적으로 변경되는 경우에만 리밸런싱을 하는 셈입니다.

|r

7

oft!
(보
1
ni

그럼 KODEX200, TIGER200-& 참고해서 K10 HEY] 투자설명서를 만듭시다.

K10 펀드 투자설명서

° 투자 목표: 펀드의 순자산가치 변동률을 KOSPI200 지수의 변동률과 유사하도록 운용합
니다.

*투자 전략: 투자 BES 추구하며 동시에 금융공학 학습의 용이성을 확보하기 위해
KOSPI200 종목에서 시가총액 기준으로 상위 10개 종목을 선정해 투자함으로써 지수 수
익률을 확보하며 가끔 발생하는 추적오차 현상을 관찰하고 원인을 파악해봅니다.

* 포트폴리오 구성: KOSPI200 상위 10개 종목으로 구성된 10 지수를 산출하고, 펀드 자
At AAS 10 지수 구성대로 주식을 매입하여 운용합니다.

* 포트폴리오 조정: 2017년 1월 2일부터 2017년 12월 28일까지 1년간만 운용하는 HES
별도의 리밸런싱은 없습니다.

펀드는 원래 유명한 지수를 벤치마크로 삼아야 투자자를 모집하기 쉽습니다. 우리가 만든
K10 지수는 개인투자자에게 알려지지 않았으니 10 지수를 벤치마크로 삼으면 투자자에게
어필하기 어렵죠. 그래서 KOSPI200 지수를 벤치마크로 삼습니다. 하지만 실제 운용은 상위
10개 종목인 10 지수를 기준으로 합니다. 간결한 AGS 통해 이해하기 쉽게 운용 기간은

2017년 1년으로 하고 리밸런싱은 하지 않기로 합니다.

19장 금융공학 모델링 355

a


===== PAGE 356 =====
08 20 니.

KODEX2007} TIGER200-< KOSPI200 구성종목 대부분을 매입해서 운용하기 때문에 추적
오차가 거의 발생하지 않습니다. 하지만 우리 HEE 10개 종목만으로 KOSPI200 지수를 따
라가야 하기 때문에 추적오차가 많이 발생할 것으로 예상됩니다. 10개 종목으로 200개 종목
을 얼마나 잘 따라가는지, 추적오차는 얼마나 자주 발생하는지, 그 이유는 무엇인지 살펴봅니다.

실습의 한계 및 가정

펀드 운용을 정밀하게 하려면 고려해야 할 사항이 많습니다. 모든 사항을 다 고려하면 너무 복
잡해져 이해하기 어려울 수 있으니 펀드 운용에 필요한 핵심적인 내용 위주로 실습을 하겠습
니다. 다음은 현실에서는 고려해야 하지만 ASS 위해 단순화하기 위한 가정입니다.

DZS 기간 중 10 구성종목은 변하지 않는다.

negro"

— KOSPIZ00 £29] 정기 변경은 1년에 한 번 일어나기 때문에 현실과 비슷하기도 합
니다.
@ 운용 기간 중 A 구성종목의 유동주식 AL 변하지 않는다.
ㅡ유동주식 수의 변경 역시 자주 일어나지 않습니다.
@ 운용 보수, 주식 매매 수수료. 증권거래세 등 제반 비용은 고려하지 않는다.
ㅡ각종 비용을 포함한 ETFS] 운용 보수는 1% 미만으로 적습니다.
@ 주식에서 받는 배당은 고려하지 않는다.
FAS 보유하면서 받게 되는 배당은 펀드 자산을 증가시킴니다. Oo] 비용을 상쇄하
는 효과가 있습니다.
© 운용 기간 중 이자율은 변하지 않는다.
-한국은행이 분기마다 이자율을 발표하긴 하지만 그 변화는 미미합니다.
© 최초 설정은 100만 AZ 시작하고, 운용 기간 중 50만 좌 이하로 내려가지 않는다.
ETFS} 경우 NAV7} 50억 원 미만이 되면 상장페지가 됩니다. 유사한 기준을 적용해
보고 싶었습니다.
이제 본격적으로 펀드를 만들어보겠습니다.

356 5부 펀드와 구조화 상품


===== PAGE 357 =====
ft

19.2 K10 HE 구성을 위한 사전 준비

펀드를 설계하려면 자료가 필요하겠죠. 벤치마크 지수인 60501200 지수. 운용 기준 지수인
10 지수 그리고 10 지수를 구성하고 있는 종목들의 일별 주가와 주식 수 데이터가 Bae
니다. 이 자료들은 앞서 7장에서 이미 실습한 적이 있으니 가져와서 재사용합니다. 코드 재사
용은 게으름이 아니라 효율의 상징이지요. 이미 학습한 코드이므로 간단한 설명만으로 복습해
봅시다.

데이터 수집과 처리를 위한 라이브러리를 호출합니다.

import datetime as dt
from urllib.request import urlopen
import bs4

import re
import pandas as pd

wu 6 WN

Out

K10 지수 구성종목을 선정합니다. 여기에서는 2018 49 159 주가를 기준으로 시가종액
상위 10개 SHS 선정했습니다. 이 실습과는 별도로 다른 종목으로 지수를 구성하고 싶거나,
종목 수를 늘리거나 줄이고 싶으면 (10_000000601 리스트에 종목코드를 변경해주면 됩니다.
KOSPI200 종목 전체를 대상으로 하는 KODEX200, TIGER200 모델을 만들고 싶으면 리스
Eo] 200개 종목을 넣어주면 됩니다.

한국거래소 시가총액 상위 10중목 (2019년1월 기준)
005930 삼성전자

000660 하이닉스

068270 셀트리온

005380 현대차

207940 삼성바이오로직스

051910 」』6화학

005490 POSCO

035420 NAVER

017670 5(텔래콤

uo On DU 은 WN

PR
Pr ®

198 금융공학 모델링 357



===== PAGE 358 =====
12
13
14
15

Out

015760 한국전력

k1@_component = ['005930', '000660', '068270', '005380', '207940',\
'051910', '005490', '035420', '017670', '015760']

선정한 10개 종목에 대한 기본정보를 가져오는 함수를 정의합니다. 이 함수에서 수집하는 기
본정보는 발행주식 수, 유동비율, 종목명입니다.

Ww

oO Ont DWN 6

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

358

# PYSS 기본정보
def stock_info(stock_cd):

url_float = ‘http://companyinfo.stock.naver.com/v1/company/c1010001.aspx?cimp_cd=" +
stock_cd

source = urlopen(url_float).read()
soup = bs4.BeautifulSoup(source, ‘lxml')

tmp = soup. find(id='cTB11').find_all(‘tr')[6].td.text
tmp = tmp.replace('\r', '')

tmp = tmp.replace('\n', '')

tmp = tmp.replace('\t', ‘')

tmp = re.split('/', tmp)

outstanding = tmp[@].replace(',', '')
outstanding = outstanding.replace('=', '')
outstanding = outstanding.replace(' ', '')

outstanding = int(outstanding)

floating

tmp[1].replace(’ ', '*)
floating = floating.replace('%’, '')
floating = float(floating)

name = soup. find(id="pArea').find('div').find('div').find('tr').find('td').
find('‘span').text

k1@_outstanding[stock_cd] = outstanding # 발행주식 수를 dicto 저장

5부 펀드와 구조화 상품


===== PAGE 359 =====
26      k10_floating[stock_cd] = floating # 유동비율을 010【에 저장
27      k1@_name[stock_cd] = name # 종목명을 dictof 저장

Out

발행주식 수, 유동비율, 종목명을 각각 저장할 딕셔너리를 ANSEL k10_component 리스트
내의 각 SES <2Sbs}4] stock_info 함수를 호출해서 기본정보를 수집해와 저장합니다.

1 k1@_outstanding = dict()
k1@_floating = dict()
k1@_name = dict()

for stock_cd in k1@_component:

2
3
4
5
6            stock_info(stock_cd)

Out

수집해온 K10 구성종목의 종목 정보 k10_info 데이터프레임에 저장하고 확인합니다.

1 4 과거 시세만 반영

2 tmp = {‘Outstanding’ : k10_outstanding,\

3      ‘Floating’ : k1@_floating,\

4      ‘Name’ : k10_name}

5 k1@_info = pd.DataFrame(tmp)

6 k10_info

Out          Floating          Name Outstanding

000660    76.91       하이닉스 728002365
005380       65.44                 현대자      220276479
005490         79.26                   POSCO         87186835
005930      72.78             삼성전자 6419324700
012330      67.12          현대모비스      97343863
028260       48.05              삼성울산      189690043
035420    77.87         NAVER    32962679
051910       64 28                Ｌ6화학       70592343
068270       63 33              쓸르리온      125395903
207940    21.78 삼성바이오로직스    66165000

19장 금융공학 모델링 359



===== PAGE 360 =====
구성종목의 일자별 주가를 가져오는 함수를 가져오겠습니다. 우선 날짜 EMS 정리하는 함수
를 가져옵니다.

1 def date_format(d):

2

3      d = str(d)

4      d = d.replace('/', '-')

5      d = d.replace('.', '-")

6

7      yyyy = int(d.split('-')[@])
8      if yyyy < 50:

9          yyyy = yyyy + 2000

10      elif yyyy >=50 and yyyy < 100:
11          yyyy = yyyy + 1900
12      mm = int(d.split('-")[1])

13      dd = int(d.split(‘-')[2])
14
15     return dt.date(yyyy, mm, dd)

Out

일자별 주가를 수집해오는 함수를 가져옵니다.

def historical_stock_naver(stock_cd, start_date="', end_date='', page_n=1, last_page=0):

1

2

3      if start_date:

4          start_date = date_format(start_date)
5      else:

6          start_date = dt.date.today()

7      if end_date:

8          end_date = date_format(end_date)

9      else:

10          end_date = dt.date.today()

11
12     naver_stock = ‘http://finance.naver.com/item/sise_day.nhn?code=' + stock_cd + ‘&page='

+ str(page_n)
13

360 54% 펀드와 구조화 상품



===== PAGE 361 =====
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
32
33
34
35
36
37
38
39
40
41
42
43

45
46
47
48
49
50

source = urlopen(naver_stock).read()

source = bs4.BeautifulSoup(source, * bal")

dates = source.find_all('span', class_='tah 010 gray@3') # 날짜 수집

prices = source.find_all('td', class_='num') # 증가 수집
for n in range(len(dates)):
if len(dates) > @:

# 날짜 처리
this_date = dates[n].text
this_date = date_format(this_date)

if this_date <= end_date and this_date >= start_date:
# start_date2} end_date 사이에서 GJO/E{ 저장

# 종가 처리

this_close = prices[n*6].text

this_close = this_close.replace(‘,', '')

this_close = float(this_close)

# SAIL{2/Of 저장

historical_prices[this_date] = this_close

elif this_date < start_date:
# start_date 이전이면 항수 =

return historical_prices

# 페이지 내비게이션
if last_page = 0:
last_page = source. find_all(‘table’)[1].find('td', class_="pgRR').find(‘a’)[‘href*]
last_page = last_page.split('&')[1]
last_page = last_page.split(‘=")(1]

last_page = float(last_page)

# 다음 페이지 SB
if page_n < last_page:

19장 금융공학 모델링 361



===== PAGE 362 =====
51          Ppage_n = page_n + 1

52       historical_stock_naver(stock_cd, start_date, end_date, page_n, last_page)
53

54      return historical_prices

Out

이제 k1@_component 422 하나씩 순환하며 historical_stock_naver() 함수를 호출해
운용 대상 기간인 2017년 1월 1일부터 2017년 12월 31일까지의 시세를 수집합니다.

1 k1@_historical_prices = dict()
2
3. for stock_cd in k1@_component:
4
5      historical_prices = dict()
6      start_date = '2017-1-1' # 시작 날짜
7      end_date = '2017-12-31' # © 날짜
8     historical_prices = historical_stock_naver(stock_cd, start_date, end_date)
9
10      k1@_historical_prices[stock_cd] = historical_prices
Out

수집한 AAS 데이터프레임에 저장합니다.

1       k1@_historical_price = pd.DataFrame(k10_historical_prices)
2        k1@_historical_price.sort_index(axis=1, inplace=True)
Out

10종목 모두 한국거래소 상장종목으로 거래일이 동일해 비어 있는 데이터는 없습니다. 하지
만 여러 나라 주식을 섞어 펀드를 구성할 수도 있으므로 데이터의 구멍을 메우는 보간을 시행
합니다.

1 k1@_historical_price = k10_historical_price.fillna(method='ffill')
2 if k1@_historical_price.isnull().values.any():
3      k1@_historical_price = k10_historical_price. fillna(method="bfill')

362 5% 펀드와 구조화 상품

 7S | SS!

natn


===== PAGE 363 =====
4 (10 111510「710621ㄴ0「166.11620(3)

Out                                  000660 085380 085490          05930 015760 017670

035420

e51910       068270        207940

2017-01-02 45800.0 150000.0 260500.0 1805000.0 4390.0 225500.0 777000.0
2017-01-03 47250.0 153000.0 256000.0 1824000.0 44100.0 223000.0 767000.0

2017-01-04 46500.0 154000.0 254500.0 1808000.0 43900.0 223000.0 810000.0

253000.0 108208. 156500.0

262009. 106600.0 158000.0

268500.0 106102.0 154500.0

삼성전자 액면분할을 반영하기 위해 수정주가를 계산합니다.

1 k1@_historical_price['@05930'] = k1@_historical_price[‘005930'] /

에 따른 수정주가 계산
2 k1@_historical_price.head(3)

Out                        000660     005380     005498 085930 615760     017670

035420

esisie          068270           207948

2017-01-02 45800.0 150000.0 260500.0 36100.0 43900.0 225500.0 777000.0
2017-@1-@3 47250.0 153000.0 256000.0 36480.0 44100.0 223000.0 767000.0

2017-01-04 46500.0 154000.0 254500.0 36160.0 43900.0 223000.0 810008.0 268500.0 106100.0 154500.0

253000.0 108200.0 156500.0

262000.0 106600.0 158000.0

이제 수집한 정보를 바탕으로 10 지수를 산출합니다. 지수 산출을 위해 일자별로 각 종목별
시가총액 비중을 구합니다. 0571200과 같은 방식의 유동주식 비율을 반영한 시가총액이 필

요합니다.

1 k1@_historical_mc = k1@_historical_price * k1@_info['Outstanding'] * k1@_info['Floating']

* 0.01
2 k1@_historical_mc.tail(3)

Out

00660                005380                005490                e05930e

015760

017670

2017-
12-26

2017-
12-27

2017-
12-28

3.980615e+13 2.182582e+13 2.356154e+13 2.265980e+14 1.226425e+13

4.039786e+13 2.21801lde+13 2.321454e+13 2.320514e+14 1, 204468e+13

4.115095e413 2.210927e+13 2.307574e+13 2.395733e+14 1.196627e+13

1.396896e+13

1.344135e+13

1. 341623e+13

비중 계산을 위해 전체 종목의 시가종액 합을 구합니다.

1 (10 = pd.DataFrame()
2 k1@['Market Cap'] = k1@_historical_mc.sum(axis=1)

19장 금융공학 모델링 363

—_

fer a


===== PAGE 364 =====
3 k10.head(3)

Out                                        Market Cap

2017-01-02 3.828017e+14
2017-01-03 3.844182e+14

2017-01-04 3.882579e+14

지수 산출을 위한 기준일을 2017년 18 2일로 설정합니다.

1 base_date = dt.date(2017, 1, 2)

Out

일자별 K10 인덱스를 계산합니다.

k1@[‘Index'] = k10['Market Cap'] / k1@['Market Cap' ][base_date] * 100
k10.head(3)

Out                             Market Cap           Index

2017-01-82 3.828017e+14 100.000000
2017-01-03 3.844182e+14 100.422277

2017-01-04 3.882579e+14 101.425324

201714 19 2일을 1002 하는 K10 지수가 생성되었습니다.

산출한 \10 지수와 KOSPI200 지수를 비교해보기 위해 지수 그래프를 그려봅니다. 우선 그
래프를 그리는 데 필요한 라이브러리를 호출하고 주피터 노트북에 그래프가 출력되도록 세팅
합니다.

1 import matplotlib.pyplot as plt
2 %matplotlib inline

Out

그래프에서 한글을 사용할 수 있도록 설정합니다.

364 5부 펀드와 구조화 상품


===== PAGE 365 =====
1      # 그래프에서 한글 사용 세팅

2      plt.rcParams[ ‘font. family'] = ‘'Malgun Gothic’
3      plt.rcParams[ 'font.size'] = 32

4     plt.rcParams[ ‘axes.unicode_minus’ ] = False
Out

그래프 사이즈, 그리드 모양을 설정합니다.

1  plt.rcParams[' figure. figsize’] = (10, 5)

2. plt.rcParams[ ‘grid. linestyle’] = ‘--'

3 plt.rcParams[‘grid.alpha'] = 0.7

4  plt.rcParams[ ‘lines.antialiased’ ] = True
Out

K10 지수 그래프를 그립니다.

1 plt.plot(k10[‘Index'], color="orange’, label="K10")
2 plt. legend(loc=@)
3 plt.grid(True)

‘out [750
140
130
120

| 110

2017-01         2017-03         2017-05         2017-07          2017-09         2017-11         2018-01

o} Ho} KOSPI200 지수를 수집해옵니다. 앞에서 K10 구성종목의 주가를 수집했을 때와 마
찬가지로 7장에서 작성한 코드인 historical_index_naver () 함수를 그대로 재사용하기로

19장 금융공학 모델링 365



===== PAGE 366 =====
합니다. 7장 실습 파일을 열어 historical_index_naver() 함수를 복사해옵니다. 다시 밝
히지만 그대로 가져온 것이니 여러분도 앞에서 작성한 SES 복사해서 사용하기 바랍니다.

1 def historical_index_naver(index_cd, start_date="', 600 _0316='', page_n=1, last_page=@):
2
3      if start_date: # start_dat7} 있으면
4         start_date = date format(start_date) # date HIHOP 변환
5      else: # 없으면
6         start_date = dt.date.today() # 오늘 SHS 지정
7      if end_date:
8          end_date = date_format(end_date)
9      else:
10          end_date = dt.date.today()
11
12     naver_index = ‘http://finance.naver.com/sise/sise_index_day.nhn?code=' + index_cd +
"&page=' + str(page_n)
13
14      source = urlopen(naver_index).read() # 지정한 패이지에서 코드 읽기
15     source = bs4.BeautifulSoup(source, ‘lxml') # 뷰티플 수프로 때그별로 코드 분류
16
17      dates = source.find_all(‘td', class ='02016') # <td class="date">EH TOA] 날짜 수집
18     prices = source.find_all(‘td', class_='number_1') # <td class="number_1">E}| 2Q//A{ 자
수 수집
19
20     for n in range(len(dates)):
21
22         if dates[n].text.split('.')[@].isdigit():
23
24             # 날짜 처리
25             this_date = dates[n].text
26             this_date= date_format(this_date)
27
28             if this_date <= end_date and this_date >= start_date:
29             # start_date2} end_date 사이에서 데이터 저장
30                   # 종가 처리
31                this_close = prices[n*4].text # prices 중 종가지수인 0, 4, 8... 번째 데이
터 추줄

366 SH 펀드와 구조화 상품



===== PAGE 367 =====
32
33
34
35
36
37
38
39
40
41
42
43

45
46
47

49
50
51
52
53
54
55

Out

this_close = this_close.replace(',', '')

this_close = float(this_close)

# 딕셔너리에 저장

historical_prices[this_date] = this_close

elif this_date < start_date:
# start_date 이전이면 항수 종료

return historical_prices

# 페이지 내비게이션

if last_page == 0:
last_page = source.find('td', class_='pgRR').find(‘a')[ ‘href’ ]
# 마지막 패이지 주소 추출
last_page = last_page.split('&')[1] # & 뒤의 page=506 부분 추
last_page = 185『_0296.5011【('=')[1] # = 뒤의 패이지 번호만 추출
135 0296 = int(last_page) # 숫자형 변수로 변환

# 다음 페이지 호줄
if page_n < last_page:
page_n = page 0 + 1
historical_index_naver(index_cd, start_date, end_date, page_n, last_page)

return historical_prices

이 함수를 SSAA 2017 한 해 동안의 KOSPI200 2142S (200 데이터프레임에 담고, a
WEES 확인해봅니다.

0 Fk WN BR

index_cd = ‘KP1200'

historical_prices = dict()

kospi200 = historical_index_naver(index_cd, '2017-1-1', '2017-12-31')
k20@ = pd.DataFrame({'Index' : kospi2@0})

k200.head(3)

198 금융공학 모델링

367



===== PAGE 368 =====
|

Out
Index

2017-01-02 260.36

2017-01-03 262.97
|                                               2017-01-04 263.12

|             2017년 1월 2일 자 KOSPI200 지수는 260.36이네요. 쉽게 비교하기 위하여 10 지수의 기
준값을 <(2501200과 맞춰주면 좋을 것 같습니다. 기준일인 2017년 1월 2일의 (2501200 지
수를 \10에도 맞춰주고, 해당 값을 Adj Index 칼럼에 저장합니다.

1 # 편하게 비교하기 위해 <10 지수를 <0501200과 맞춤 (기준일 기준으로)

2 = (10['401 Index'] = (10[ ‘Market Cap'] / k1@['Market Cap'][base_date] * (200['1006×'][02056_
date]

3 k1@.head(3)

Out              Market Cap     Index Adj Index

2017-01-02 3.828017e+14 100.000000 260.360000
2017-01-03 3.844182e+14 100.422277 261.459441

2017-01-04 3.882579e+14 101.425324 264.070973

기준일인 2017년 18 2일의 두 지수는 260.30으로 같아졌습니다. 비교하기 편해졌네요. 그
럼 두 지수의 그래프를 함께 봅시다.

plt.plot(k10['Adj Index'], 0010「='002096', label='K10')
plt.plot(k20@[‘Index'], color="blue’, Label='KOSP1200')
plt. legend(1loc=@)

plt.grid(True)

> WN PR

368 5% 펀드와 구조화 상품


===== PAGE 369 =====
Out
—— k10

— kOSPi200

360

320
300 +

280 J

260

2017-01         2017-03         2017-05         2017-07          2017-09         2017-11         2018-01

KOSP12002¢} K10°] 수익률이 더 높은 것을 확인할 수 있습니다.

19.3 K10 펀드 설계 및 운용

이제 본격적으로 10 펀드를 만들어봅시다. 우리는 코딩의 효율성을 위해 10개 종목을 한꺼
번에 계산할 건데, 여러 종목을 한꺼번에 처리할 때는 넘파이 배열이 유용합니다. 넘파이 라이
브러리를 호출합니다.

1 import numpy as np

Out

이제 펀드 기본정보를 세팅합니다. 설정과 환매 단위인 CU(creation unit), HE 설정 기준
일, 최초 설정 수량, 펀드가 보유할 현금에 대한 이자인 이자율 BBS 결정합니다.

CU = 50000 # 설정과 환매 단위
base_date = dt.date(2017, 1, 2) # 설정 기준일
volume = 1000000 # 2/2 설정 수량

interest_rate = @.02 # 이자율

Pe WN

Out

19S 금융공학 모델링 369



===== PAGE 370 =====
펀드 운용 기간 중 매일매일 설정과 환매가 일어날 수 있습니다. 설정과 환매가 얼마나 많을지
는 예측 불가하므로 [30001 함수를 이용합니다. 환매의 경우 최소 50만 좌 이상은 유지해주

기 위하여 50만 좌 이상인 경우에만 환매가 일어나도록 조건을 추가해줍니다.
1 def creation_redemption(v):

2     creation = np.random.randint(@, 5) * 00 # @5 사이 임의의 청수 x CU

3      if v>500000: # 50만 2} 이상인 경우에만 환매 발생

4         redemption = np.random.randint(@, 5) * CU

2      6156:

6          redemption = 0

7      volume = v + creation - redemption # 층 좌수 = 기존 좌수 + BA - 환애
8

return(creation, redemption, volume)
Out

np. random. randint ()2] 사용 방법은 다음을 참고합니다.
np.random. randint(A|2t, 2)

(생략 가능. 기본값 0)
* 시작과 끝 사이의 임의의 정수를 반환

매일 주가가 변동함에 따라 zou le 할 주식의 비중이 달라집니다. 데이터프레임의 일괄 계

산 기능을 이용해 일자별 보유 비중을 간편하게 계산해 k1@_stock_ratio] 저장합니다.
1 # 보유 비중 산정
2 k1@_stock_ratio = pd.DataFrame()
3 fors in k1@_info. index:
4

k1@_stock_ratio[s] = k1@_historical_mc[s] / k1@_historical_mc.sum(axis=1)

Out

이제 일자별 보유 비중 변동과 설정 및 환매 수량 변동에 따라 펀드의 포트폴리오가 어떻게 변
하고, 그 결과 펀드의 자산가치가 변하는 과정을 계산하겠습니다.

1~2행에서 일자별 BE 순자산가치는 『400고41 데이터프레임에, 순자산가치 변화는 『400_

370 54% 펀드와 구조화 상품



===== PAGE 371 =====
Chg 데이터프레임에 저장하기 위해 미리 선언합니다.

1 Fund_NAV = pd.DataFrame()
2  Fund_Chg = pd.DataFrame()

4행에서 일자별로 순환하며 계산할 수 있도록 7@『문을 선언합니다.

oh  _for d 3 in | k10_ historical -Price. index:

6~8행에서 포트폴리오 구성에 사용할 일자별 주가와 일자별 비중을 불러와 stock_price,
stock_weightol] 저장합니다.

6     # 포트폴리오 구성용 정보 (당일 주가, 자산 비중)
7      stock_price = np.array(k10_historical_price. loc{d])
8     stock weight = = 00: gel tey lee stock_ratio. ioe

10~17행에서 전일까지의 주식 포트폴리오의 AVS 계산합니다. 종목별 주식 보유량은
stock_holdingso] 저장하는데, 기준일인 1월 2일 이전에는 보유량이 없으므로 stock_
holdingsS 0으로 세팅합니다(13행). 현금 잔고도 물론 0입니다(14행). 기준일 이후에는 전
일까지의 주식 보유 수량에 주가를 곱해서 전체 주식 잔고를 계산하고(16행), 현금 잔고를 더
해주면 펀드 전체의 순자산가치를 구할 수 있습니다(17행).

10      # 기존 주식 포트폴리오 NAV 계산

11     if (0 <= base_date): # 기준일 이진

12         # 최초 주식 포트폴리오 (보유량 0)

13        stock_holdings = np.array([@, 0, 0, 0, 0, 0, 0, 0, 0, 0])
14         NAV_cash=0 ＊ 2/2 현금 보유량

15     else: # 기준일 이후

16         NAV_stock = sum(stock_holdings * stock_price) # 주식 잔고

17         NAV = NAV_stock + NAV_cash # 전체 잔고

19~24행에서는 기준가격을 산정합니다. 비교가 쉽도록 1월 2일의 기준가격을 0501200지

수 * 100으로 맞춰줍니다(22행). 그 이후에는 펀드 전체의 순자산가치를 총 좌수로 나뉘서 구

19장 금융공학 모델링 371

[cea sews

coer


===== PAGE 372 =====
합니다(24행).

19      # 기준가격 산정

20     if (0 <= base_date):

21        # 최초 기준가를 기준일자의 KOSPI 200 지수와 맞춤
22         price = k2@@['Index'][base_date] * 100

23      else:

24          price = NAV / volume

26~368 A= 일자별 설정 및 환매를 반영합니다. 설정 AGS 기존 좌수는 0(28행),
변경된 좌수는 100만 주입니다(29행). 다음 날부터는 앞에서 만들어놓은 0ㅠ6231100_
redemption() 함수를 이용해 임의의 gros 설정 및 환매 수량을 받아와서(31행), 변동 좌
수 = 설정 좌수 - 환매 좌수를 계산합니다(32행). 변동된 좌수를 총 좌수에 반영합니다(34
행). 변동된 좌수에 당일의 펀드 기준가격을 곱해주면 일별로 펀드에 입출금된 자산의 총액이
계산됩니다(36행).

26       # 신규 펀드 설정 및 환매 좌수 계산

27      if (0 = 0356 0216):

28         volume = 0 # 펀드 좌수

29         volume_chg = 1000000 # 첫날 설정액

30      else:

31         vol = creation_redemption(volume) # 설정 및 환매 함수 호출
32         volume_chg = vol[@] - 101[1] # 좌수 변동

33      # 층 펀드 좌수에 반영

34      volume = volume + volume_chg

35     # WC 입줄금액

36      aum_chg = price * volume_chg

38~43행에서는 당일 입출금된 금액만큼 주식을 거래해야 합니다. 종목별로 얼마큼의 금액
을 투자할지를 구한 후 주가로 나누어주면 종목별로 몇 주씩 매매할지 계산되며, Bake
stock_tradeo]] 저장합니다(39행). 당일의 주식 매매 금액 SHS trade_amtol] 저장합니다
(41행). 입출금된 자산 종액에서 주식 매매 금액을 빼면 남은 현금 변동을 구할 수 있습니다
(43행).

372 5부 HOS 구조화 상품


===== PAGE 373 =====
38 # 신규 주식 거래량 계산

39     stock_trade = np.floor( price * volume_chg * stock_weight / stock_price )
40      # 주식 매매 금액

41     trade_amt = sum(stock_trade * stock_price)

42     # 현금 잔고 변동

43      cash_chg = aum_chg - trade_amt

45~48행에서 전일까지의 주식 보유량에 신규 주식 거래량을 더해주면 총 주식 보유량이 됩

니다(46행). 전일까지 보유하고 있던 현금은 이자율만큼 증가합니다(48행).

45      / 층 주식 보유량 = 기 보유량 + 신규 거래량
46      stock_holdings = stock_holdings + stock_trade
47      # 현금 보유량 증가 (0/자용 반영)

48     cash_holdings = np.floor( NAV_cash * np.exp(interest_rate/365) )

50~53행에서 HES] 순자산가치를 업데이트합니다. SUS] 신규 AMES 반영한 SF 주식
보유량에 당일 주가를 곱하면 주식 순자산가치가 나옵니다(51행). 전일까지 보유한 현금 증가
분에 당일의 현금 변동을 더해주면 현금 순자산가치가 됩니다(52행). 이 둘을 합하면 펀드 전

Lo Loe

체의 순자산가치가 됩니다(53행).

50      # NAV 업데이트
51     NAV_stock = sum(stock_holdings * stock_price) # 주식 잔고
52      NAV_cash = cash_holdings + cash_chg # 현금 잔고

53      NAV = NAV_stock + NAV_cash # 진체 잔고

55~65행에서 HES) 일자별 순자산가치를 Fund_NAvel], 일자별 설정 및 환매 좌수 정보를
『400_00에 저장합니다. 일자별 인덱스를 만들기 위해 날짜 정보를 시리즈에 저장합니다(55
행). 데이터프레임에 저장하기 위해 NAV 정보를 dict 형태로 임시 저장하고(58행), 날짜 인
AS 함께 데이터프레임에 저장한 후(59행), 일자별로 누적합니다(60행). 일자별 설정 및

환매 정보 역시 같은 방식으로 저장합니다.

55           date = pd.Series(d)

19S 금융공학 모델링 373

if


===== PAGE 374 =====
56
57
58
59
60
61
62
63

65

지금까지 설명호

# Fund NAV BBS 데이터프레임에 저장

NAV_tmp = {‘Stock' : NAV_stock, ‘Cash’ : NAV_cash, ‘Total’ : NAV,

tmp = pd.DataFrame(NAV_tmp, index=date)
Fund_NAV = Fund_NAV.append(tmp)

# 일자별 설정 및 환매 좌수 BS 데이터프레임에 저장

Chg_tmp = {‘Amount Change’ : aum_chg, ‘Trade Amount’ : trade_amt,
chg}

tmp = pd.DataFrame(Chg_tmp, index=date)
Fund_Chg = Fund_Chg.append(tmp)

} SES 한 번에 모아서 보면 다음과 같습니다.

et

‘Price’ : price}

"Cash Change’ : cash_

374

Fund_NAV
Fund_Chg

pd.DataFrame()
pd.DataFrame()

for 0 in k1@_historical_price. index:

# 포트폴리오 구성용 정보 (당일 주가 / 자산 비중)
stock_price = np.array(k10@_historical_price.loc[d])

stock_weight = np.array(k10_stock_ratio. loc[d])

# 기존 주식 포트폴리오 44 계산

if (0 <= base_date): # 기준일 이진
# 최초 주식 포트폴리오 (보유량 0
stock_holdings = 00.20「「127([0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
NAV_cash=0 # 최초 현금 보유량

6156:     # 기준일 이후
NAV_stock = sum(stock_holdings * stock_price) 주식 잔고
NAV = NAV_stock + NAV_cash # 전체 잔고

# 기준가격 산정

if (0 <= base_date):
# 최초 기준가를 기준일자의 KOSPI 200 지수와 맞춤
price = k20@[‘Index'][base_date] * 100

else:


===== PAGE 375 =====
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39

40
41
42
43

45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60

price = NAV / volume

# 신규 펀드 설정 및 환매 좌수 계산
if (0 = 06356 0216):
volume = 0 # 펀드 좌수
volume_chg = 1000000  /＊ 첫날 설정액
else:
vol = creation_redemption(volume) # 설정 및 환매 함수 호출
volume_chg = vol[@] - vol{1] # 좌수 변동
# 총 펀드 좌수에 반영
volume = volume + volume_chg
# 펀드 입출금액

aum_chg = price * volume_chg

/ 신규 주식 거래량 계산

stock_trade = np.floor( price * volume_chg * stock_weight /
stock_price )

# 주식 매매 금액

trade_amt = sum(stock_trade * stock_price)

# 현금 잔고 변동

cash_chg = aum_chg - trade_amt

# 층 주식 보유량 = 기 보유량 + 신규 Hee
stock_holdings = stock_holdings + stock_trade

# 현금 오유량 증가 (이자율 반영)

cash_holdings = np.floor( NAV_cash * np.exp(interest_rate/365) )

# NAV QYG/O/E

NAV_stock = sum(stock_holdings * stock_price) # 주식 잔고

NAV_cash = cash_holdings + cash_chg # 현금 잔고
오마     ae

사서. 서게                     거여"

“NAV = 40500 + NAVcash # 전체 잔고
date = pd.Series(d)

# Fund NAV 정보를 DataFramOj] 저장

NAV_tmp = {'Stock' : NAV_stock, ‘Cash’ : NAV_cash, ‘Total’ : NAV, ‘Price’ : price}
tmp = pd.DataFrame(NAV_tmp, index=date)

Fund_NAV = Fund_NAV.append(tmp)

19s 금융공학 모델링 375



===== PAGE 376 =====
61

62     # 일자별 설정 및 환매 좌수 정보를 DataFramed] 저장
63      Chg_tmp = {"Amount Change’ : aum_chg, ‘Trade Amount’ : trade_amt, ‘Cash Change’
cash_chg}
64      tmp = pd.DataFrame(Chg_tmp, index=date)
65      Fund_Chg = Fund_Chg.append(tmp)
Out

그럼 이제 K10 HES] 수익률을 그래프로 확인해봅시다. 우선 펀드 수익률 그래프에 일반적
으로 쓰이는 기준일(2017년 1월 2일)부터 현재까지의 수익률을 나타내는 YTD (year to date)
수익률을 보겠습니다. 각 지수 수익률과 펀드의 수익률을 AA Earnings 데이터프레임에
저장하고 그래프로 그립니다.

# 펀드 수익률 vs Al 수익
Earnings = pd.DataFrame()

3  Earnings['K10'] = ( k1@[‘Index'] - k10['Index'][base_date] ) / k1@['Index'][{base_date] *
100

4 ㄷ20「01095[ '(05061200'] = ( k2@@['Index'] - k2@@['Index'][base_date] ) / (200['1006<']1[0056_
date] * 100

5 €arnings['Fund'] = ( Fund_NAV['Price'] - Fund_NAV['Price'][base_date] )/ Fund_NAV['Price’ ]
[base_date] * 100

ax = Earnings.plot(color = ['orange’, ‘blue’, ‘red'])
ax. Legend(loc=@)

ax.set_ylabel('(4-2}#, %)')

ax.grid(True)

onan oO

Out          50

= 110

— Fund

호

2017-01      2017- 03       2017-05       2017-07       2017-09      2017-11       2018-01

376 5% 펀드와 구조화 상품


===== PAGE 377 =====
K10 지수 수익률을 나타내는 주황색 선은 610 펀드 수익률인 빨간 선에 가려져 보이지 않습
니다. 10 펀드의 수익률과 10 지수의 수익률은 거의 일치하고, KOSPI200 수익률보다는
높은 움직임을 보였네요. KOSPI 상위 10개 종목의 주가가 KOSPI200 전체 종목 평균보다 많
이 올랐다는 뜻입니다. 그럼 수익률 말고 기준가와 지수를 비교하면 어떨까요?

TEC) 00 이에 80060 는

Out

당연호

일반적인

# HE 기준가 vs 지수

Indicator = pd.DataFrame()

Indicator['K10'] = k1@['Adj Index']

Indicator[ ‘KOSPI20@'] = k200[ 'Index' ]
Indicator[‘Fund'] = Fund_NAV[ ‘Price’ ]/100

ax = Indicator.plot(color = [‘orange’, ‘blue’, ‘red'])
ax. Legend(loc=@)

ax.set_ylabel('(+218, %)')

ax.grid(True)

2001. to
— KosPi200
—— Fund
360
_ 340
z
+ 320
기
300
280
260
2017-01     2017-03     2017-05     2017-07     2017-09     2017-11     2018-01

애기지만 수익률뿐 아니라 기준가격과 지수 역시 동일한 움직임을 보입니다. 이번에는
주식 차트가 주가와 거래량을 함께 표시하는 것처럼 수익률과 펀드의 Nav AK

치) 변동을 함께 표시해봅니다. NAVE 가독성을 높이기 위하여 억 원 단위로 표시합니다.

oO Ont Dn 제 WN Pp

fig = plt.figure(figsize=(10, 8))

axl = fig.add_subplot(2, 1, 1)

fig.add_subplot(2, 1, 2)

Earnings.plot.line(ax=ax1, color = [‘orange', 'b', ‘r'])
ax1.set_ylabel('(=- 2], %)')

Fund_NAV['Display'] = Fund_NAV[‘Total'] * 0.00000001

Fund_NAV[ ‘Display’ ].plot.area(ax=ax2, stacked=False, sharex=True)
ax2.set_ylabel(‘(NAV, 2{91)')

ax1.grid(True)

ax2

198 금융공학 모델링 377

아마”


===== PAGE 378 =====
10 ax2.grid(True)

Out

— Fund

(UM, %)

10

(AV, @B)
8

2017-01      2017-03       2017-05      2017-07       2017-09      2017-11       2018-01

BEE YTD 수익률도 중요하지만 매일매일의 일간 수익률 역시 중요합니다. 단기 투자자
도 펀드의 목표 수익률을 얻어야 하기 때문이죠. 그래서 이번에는 일간 수익률을 계산해서 그

ame 그려보겠습니다. 일간 pepe, 우으기뜨가저-전랄기또가격 <. 계산됩니다. 전

일기준가격을 구할 때는 전일 날짜의 AVIS 하루씩 뒤로 당기면 되는데, 데이터프레임에서
는 DataFrame.shift (1)= 간단히 뒤로 할 수 있습니다. 만일 반대로 앞으로 당겨야 한다면
DataFrame. shift (-1 )을 하면 되지요.

1 # 일간 수익률

2 fig = plt.figure()

3 ax = fig.add_subplot(1, 1, 1)

4 Daily = pd.DataFrame()

5 Daily['K10'] = (k10[‘Index'] - k10[‘Index'].shift(1))\

6               / k10['Index'].shift(1) * 100

7 Daily['K200'] = (k2@@[‘Index'] - k200['Index'].shift(1))\

8               / k20@['Index'].shift(1) * 100

9 Daily['Fund'] = (Fund_NAV['Price'] - Fund_NAV['Price'].shift(1))\
10               / Fund_NAV['Price'].shift(1) * 100

11 Daily.plot(ax=ax, color = [‘orange’, ‘blue’, ‘red'], alpha=0.7)
12 ax.set_ylabel('(%)')

378 54 펀드와 구조화 상품


===== PAGE 379 =====
13 ax.grid(True)

Out

— 10
331 -ㅡ- 1200
Fund

2017-01       2017-03       2017-05       2017-07       2017-09       2017-11       2018-01

WES] 일간 수익률이 KOSPI2009] 일간 수익률보다 더 큰 FOS 움직이네요. 5월, 9월에는
3% 넘게 상승한 날도 보입니다. 포트폴리오는 분산이 되면 될수록 수익률이 안정적으로 변합
니다. 10개 종목보다는 200개 종목으로 구성한 포트폴리오가 더 안정적이지요. 안정적이란
말이 좋게 들리긴 하지만 반대로 상승폭도 작다는 것을 의미합니다.

이번에는 펀드의 추적오차(\ㅠ20108 ㅇㅁㅁ07『)를 구해봅니다. © 매일매일의 추적오차는

2
펀드 수익률 -지수수익률)

펀드 수익률 - 지수 수익률로, 기간별 추적오차는 20       -
(no. 일 OS 구합니다. 여기에서는 WES] 일간 추적오차를 구하는 것이므로 D9] 식을 이
용합니다.

우리가 만든 펀드의 벤치마크인 KOSPI200 지수와의 추적오차입니다.

# KOSPI200 대비 일간 추적오차융

fig = plt.figure()

ax = fig.add_subplot(1, 1, 1)

Daily['TE200'] = Daily['Fund'] - Daily['K200'] # 추적오차율 = 펀드 수익률 - 지수 수익률
Daily['TE2@@'].plot(ax=ax)

ax.grid(True)

be) 00 (35 (NY 더

19장 금융공학 모델링 379



===== PAGE 380 =====
Out       20

2017-01       2017-03       2017-05       2017-07       2017-09       2017-11       2018-01

대부분의 오차가 +1.0 이내, 최대 41.8 정도만 벌어지는 것을 확인할 수 있습니다. 1071 S
목만으로 200개 종목을 따라감에도 불구하고 추적오차가 크게 벌어지지 않습니다. 10개 종목
<A OAL

만으로도 KOSPI200 HE 운용이 어느 정도는 가능하네요. 그러면 10 지수와의 +
은 어떻게 될까요?

1 # K10 대비 일간 추적오차융
2 fig = plt.figure()
3 ax = fig.add_subplot(1, 1, 1)
4 Daily['TE1@'] = Daily['Fund'] - Daily['K10']
5 Daily['TE1@'].plot(ax=ax)
6 ax.grid(True)
Out   a
0015
0010
0.005
0.000
-0.005
-0.010
-0.015
2017-01    2017-03    2017-05    2017-07    2017-09    2017-11    2018-01

K10 지수와의 추적오차는 최대 +0.02% 아주 미미합니다. 그렇다면 KOSPI200 지수

han

380 54 펀드와 구조화 상품

르츠

적


===== PAGE 381 =====
하기 위해 200개 종목을 거의 다 담는 KODEX200, 710ㅁㅁ200과 같은 펀드는 추적오차가 거
의 발생하지 않는 아주 좋은 BES 것으로 추정됩니다.
참고로 앞의 그래프는 책에 나온 것과 독자의 모델이 다른 Awe 보여줄 것입니다. 펀드를
설계할 WW creation, redemption 수량이 랜덤하게 바뀌도록 구성했는데, 이 때문에 BES
실행할 때마다 펀드 좌수가 달라지게 됩니다. 펀드 좌수가 달라지면 펀드가 보유하고 있는 현
금 등이 달라져서 NAV 값이 미미하지만 변동되는데, 0.001% 단위로 관찰하는 추적오차율에
서는 이 작은 차이가 눈에 SF 있기 때문이지요.

지금까지 10 지수를 만들고 이 지수를 바탕으로 KOSPI200S 추종하는 펀드를 만들고 운용
해보았습니다.
이것으로 이 책을 통해 전달하고 싶은 USS 모두 살펴봤는데, 너무 어렵거나 너무 쉽지는 않
았나요? 책을 읽기 전 금융 지식이나 프로그래밍 지식 수준에 따라 책이 어려웠을 수도, 쉬웠
을 수도 있을 것입니다. 이 책에서 다룬 내용 GEA 증권사, 자산운용사, 은행 같은 금융기관
에서 사원이나 주임급 직원에게 요구하는 수준의 금융공학 지식을 충분히 채울 수 있습니다.
금융권 취업을 준비하는 분이라면 이 책의 내용만 숙지한다면 금융지식을 물어보는 WAS 거
E35] WAS 수 있을 것입니다. 수고 많으셨습니다.

19장 금융공학 모델링 381



===== PAGE 382 =====
플래시 크래시

플래시 Sey) (flash crash) = 주가 하락에 민감하게 반응한 자동 매매 알고리즘이 매
도 물량을 쏟아내 연쇄 반응을 일으키며 시장이 더 급속도로 하락하게 만드는 현상을
말합니다.

지수에 영향을 주는 일부 대형주 주가가 하락하면 지수가 하락하게 됩니다. 그러면 해
당 지수를 추종하는 금융상품이 사용하는 금융공학 기법이 적용된 자동 매매 알고리즘
은 지수 하락 시 추가 손실 방지를 위해 ASHA(stop—loss) 매도 주문을 Yc}, 금
용공학이 더 널리 사용될수록 자동 매도 주문은 늘어나고 결국 시장은 더 빠른 속도로
하락하게 되는 것이지요.

플래시 크래시는 수시로                                      모찌
일어나고 지금까지 많은
사례가 있었지만, 2010년
Sal 미콕에서 발생한 사
래시을 일러는 계기가 "1006           ina           as

습니다. 오후 2A] 30분부

터 10분만에 다우존스 지수가 1000포인트 이상 하락한 것이지요. 이 사건은 최초 한
트레이더의 주문 실수로 지수가 하락한 것으로 시작됐고, 지수 하락에 따른 자동 매매
매도 주문이 급격한 시장 폭락을 초래했다고 알려졌습니다. 하지만 2015년에 런던의
한 트레이더가 이 사건의 범인으로 유죄를 선고받았습니다. 주문 실수가 아니라 플래
시 크래시를 유발할 목적으로 선물 주문을 허위로 낸 사실이 적발된 것입니다.

플래시 크래시는 금융공학이 대중화될수록 충격이 더 커지는데, 그 이유는 두 가지입
니다. 금융공학으로 인한 알고리즘 매매의 증가와 금융공학을 이용한 지수 기반 금융
상품의 규모 증가 1 21세기 최고의 금융상품이라 불리는 ETRE 금융공학이
생산하는 대표적 상품으로, 투자하기 쉽고 수수료가 낮기 때문에 전 세계 투자자들에
게 인기를 한 몸에 받고 있습니다. 지수 상품에 투자된 자산이 많아질수록, 지수 하락
시 알고리즘 매매로 인한 하락 속도는 더 빨라질 수밖에 없는 구조인 것이죠.

382 5부 펀드와 구조화 상품

ㅣ 너도 다]    if

더 으으 1.


===== PAGE 383 =====


===== PAGE 384 =====


===== PAGE 385 =====
A.1 파이썬 기본 문법

이 PRS 프로그래밍을 한 번도 해보지 않은 분을 위해 마련했습니다. 프로그래밍을 해본 분
이라면 건너뛰어도 좋습니다.

프로그래밍을 하려면 우선 작성한 ACS 실행할 수 있어야겠죠? HSS 실행하려면 [Shift]
+(Enter]S 누릅니다. 모든 실습에서 동일하게 적용되므로 코드 입력이 끝나면 꼭 [Shift] +
[Enter] 누르세요.

att 출력
프로그래밍을 하면 결과가 의도한 대로 나오는지 확인해봐야겠지요? ASKS 출력하는 가장

일반적인 방법은 0ㅁ10( ) 함수를 이용하는 것입니다.

숫자를 출력할 때는 ( )에 직접 넣어주면 되고, 문자를 출력할 때는 따옴표( ' '       a, 이
용해 묶어주어야 합니다. 여러 값을 연속해서 출력하려면 AEC )를 이용해 연결해줄
습니다.

rR

print(1)
2          print(‘A’)

부록 파이썬 프로그래밍 기초 385

때 |


===== PAGE 386 =====
18

3   pa, Number:', 1)

코드 입력 끝나고 | 6016 ]+[Enter |S 누르셨죠?

파이썬은 작은따옴표와 큰따옴표를 모두 사용할 수 있습니다. 다만 한 문장 내에서 혼용은 불
가합니다. 이 책에서는 기본으로 작은따옴표를 사용합니다만, 독자의 기호에 따라 큰따옴표로
사용해도 무방합니다.

대소문자 구분
파이썬은 대문자와 소문자를 구분합니다. 《와 at: 서로 다른 변수로 인식하는 것이지요.

a

A=   al

~A
고매 주
수2'
A:'

rE 「뜨

1

2 a=
3 print('A:', A)
4

pent: a:', a)

Out A: 변수1
a: 변수2

들여쓰기
파이썬은 들여쓰기로 문단을 구분합니다. 단일 문단 내에서는 반드시 같은 위치에서 줄을 시
작해야 하며, 이를 어기면 에러가 발생합니다.

1 print(1)
2  print(2)

Out 1
2

386 부록 파이썬 프로그래밍 기초


===== PAGE 387 =====
다음은 들여쓰기 오류로 에러가 발생한 예입니다.

1 print(1)
2     prant@).

Out File "  set etione 1000 -4-ea5ae22bc8ce>", line 2
print(2)

^

IndentationError:  oespected indent

문장의 끝 (줄바꿈)

파이썬은 자바, CO} 같이 문장 끝에 세미콜론(; )을 BAS 필요가 없습니다. 다만 붙여줘도
에러는 나지 않습니다. 문장이 너무 길어져 가독성을 높이기 위해 줄을 바꾸고 싶을 때는 백슬
래시 (\ )를 붙이고 다음 줄로 넘어갑니다.

6 = '문장을 만들어볼까요?'
6 = '긴 문장을 ' + \
'한 줄로 만들어볼까요?'

OF "의 594

주석

AAI (comment)& 코딩에 포함되긴 하지만 파이썬이 해석하지 않는 문자열입니다. 프로그래
밍을 하면서 참고 사항 등을 표시할 때 사용합니다. 주석은 #, ''' ''', """ """로 표시합니
다. 한 줄짜리 주석은 # 뒤에, 여러 줄 주석은 ''' '「'나 """ ""사이에 eet

1 # 이것은 한 줄 주석입니다.
2 p=1 * 0) 줄에서는 여기서부터가 주석입니다.
3

부록 파이썬 프로그래밍 기초 387



===== PAGE 388 =====
상중 따옴표 사이에 들어와도 다 주석입니다.
여러 줄 주석을 입력할 때 사용합니다.

p = 100
주석은 파이썬에 입력되지 않기 때문에 출력되지 않습니다.

11 print(p) #p#S 줄력하는 SSS 2행에 있습니다.

변수의 형식 (자료형)

래밍은 필요한 정보를 컴퓨터에게 알려주며 계산을 시키고 ARGS 돌려받는 과정입

니다. 컴퓨터에게 정보를 알려줄 때는 이름표를 달아서 알려주는데, 이름표를 변수라고 합니
는           변수와 문자형 변수로 구분됩니다.

!

그만
ing
|

oft!

변수 타입: SAS, 문자형

숫자형 변수에는 11, float, complex 등이 있습니다. AE int, AE float, 복소수
는 000016×입니다. 변수가 어떠한 형태로 사용되었는지 확인하려면 type (H+ )이라고 입
력합니다.

숫자형 변수는 꼭 BAS 지켜서 사용해야 합니다. 정수형 변수에 소수를 집어넣으려고 하면
에러가 발생합니다.

fuy(u

type(i)

Out int

변수에 소수를 입력하면 자동으로 소수형 변수로 설정됩니다.

388 부록 파이썬 프로그래밍 기초



===== PAGE 389 =====
2  type(f)

Out float

하지만 정수형으로 이미 선언된
float () 함수를 이용하면 정수형 변수가 강제로 도   변환 auch

i= float(i) # 정수형으로 선언했던 변수를 소수형으로 변환

type(i)
Out float          :        ie      mit         ~         i
금융에서는 사용할 일이 거의 없지미       형 변수도 있습니다

1 c=1+2) 옥소수렁 면수

2   ee)

Out    Salen

문자형 변수는 '' (작은따옴표) 또는 ""(큰따옴표)로 감싸서 전달해야 합니다. 둘 중 어떤 따옴
를 사용해도 상관없습니다. 여러 줄을 넣을 때는 ' ' ' '' '나 """ """ 사이에 넣습니다.

type(s)

Out str

문자형 변수를 출력해봅니다.

1 print(s2)

Out 나도
문자

부록 파이썬 프로그래밍 기조 389


===== PAGE 390 =====
print () 함수를 쓰지 않아도 결갓값이 나오는 경우도 있습니다. 보고 싶은 값이 하나뿐이라
면 굳이 print )를 쓰지 않아도 됩니다. 하지만 0ㅁ10()로 명시적으로 출력해주지 않고 변
수를 여러 개 나열한다면 마지막 변수만 출력되고 이전 것들은 무시됩니다. 따라서 보고 싶은
값의 개수에 따라 print )를 써야만 하는 경우가 있습니다.

A.2 사칙연산
FAS 사칙연산은 더하기 (+), 빼기(- ), 곱하기 (*), 나누기 (/ ), 나머지(%). ASA
(** > So] 있습니다.

1 %=3
2 print(x)

Out 3

1 print(x * 2)

Out 6

1 print(x ** 2) #x*x 도 같은 표현입니다.

Out 9

1 print(x ** 3) # 거듭제꼽은 엑셀에서는 x°3 로 표현됩니다.
Out 27                                       a

문자는 사칙연산 대신 합치기와 자르기가 됩니다. 문자를 합칠 때 +를 사용하고, 문자를 자를
때는 변수 뒤에 [시작 위치(이상):끝 위치(미만 )]을 붙여 사용합니다. 문자의 최초 위치는 0
부터 시작되고, 시작점은 포함, 끝점은 미포함합니다. 각 위치를 나타내는 점이 문자 위를 가
리키는 것이 아니라 문자 사이를 가리킨다고 이해하시면 됩니다. 다음 pythonolek= 문자열
에서 [0:2]라고 하면 OS 『 앞 위치, 2는 \와 t 사이 위치를 가리키므로 ‘py’ 7} 나옵니다. 인
덱스를 생략하면 가장 끝 위치를 나타냄니다.

390 부록 파이썬 프로그래밍 기초



===== PAGE 391 =====
HPHYHE HM © fo |
0190 1260 300 45

1 wi= ‘py’
2 w2 = ‘thon'
3 word=wl+w2 #4 w1i} 02를
4 word

Out   "Python"

합하기

. 1 word[@:2] # OE} 2까지
Out ‘Py’

Out ‘yth'

1  _word(1: ae   # 1부터 4까지

et  word[: 4]   # 처음부터 STEAL

Out ‘Pyth'

1 word[4:] # 4부더 끝까지

Out ‘on'

A.3 고급 자료형

리스트

리스트(119[)는 여러 값을 그룹으로

자형과 문자형이 섞여서 존재

Fi

번에 지정하는 자료형입니다. 리스트 안에는 숫

부록 파이썬 프로그래밍 기초 391



===== PAGE 392 =====
ES te

1 prices = [100, 200, 300, 400, 500]

2 prices

리스트도 문자열과 같은 방식으로 dehy 수 있고, 특정 위치의 값만을 Bora + 있습니다.
주의할 점은 문자 자를 때 보았듯이 파이썬은 최초 위치에 0을 지정하기 때문에 네 번째 값을
뽑아내려면 [3]이라고 지정해야 합니다.

1 prices[@:2]
Out [100, 200]

1 prices[3] #2 번째 값은 00/22 3S 지정하면 | 번째 값이 옵니다.

Out 400

리스트에 값을 추가할 수 있습니다.

1 prices.append(600) # 300600를 할 때는 [JO] 아니라 OS 사용합니다.
2 prices

Out [100, 200, 300, 400, 500, 600]

리스트에 몇 개의 값이 들어 있는지는 161 (리스트 )로 확인합니다.

1 len(prices)

Out 6

리스트에서 값을 빼낼 수도 있습니다.

1 prices.remove(400) # removeS 할 때는 [JO] 아니고 ()를 사용합니다.

2 prices

Out [100, 200, 300, 500, 600]

392 부록 파이썬 프로그래밍 기초


===== PAGE 393 =====
1    _len(prices) |

04 5

한꺼번에 여러 WS 넣으려면 extends 사용합니다. 여러 값을 한 번에 넣기 위해서는 [] 속
에 여러 값을 넣어 리스트를 만든 후 기존 리스트에 추가해줍니다.

1 prices.extend([700, 200]) # 6×<[600를 할 때는 QC 안에 리스트를 넣어줍니다.

2 prices

Out (200, : 200, 300, 500, 600, 700, 200)

1   len(prices) -

Out 7

세트
세트(660)는 수학의 집합과 같습니다. 리스트에서는 그룹 지정에 []를 사용했지만 집합에서

EOS Agere  수학 시간에 공부한 집합의 연산인 합집합, 교집합. 차집합 연산을 할 수
있습니다.

Ae Acs. 06 2, 3. 4) 5}
B= {4, 5, 6, 7, 8}
3 type(A)

Out set

il  A |006 합집합. A. union(B) = 가능

Out 23. 5. 6. 7, 8}

1 A&B # DBs A.intersection(B)= 가능
Out {4, 5}

1 A-B 자집합
Outen) 2703}.

부록 파이썬 프로그래밍 기초 393



===== PAGE 394 =====
i=#-4

T=

FE (uple)S 리스트와 유사하지만 한번 만들어지면 데이터를 추가하거나 변경할 수 없습니
다. 다만 처리 속도에 장점이 있어 파이썬 내부적으로 많이 사용됩니다. 리스트는 [], 세트
{}, 튜플은 OS 사용합니다.

et =: 27 3)
2 type(t)
Out tuple

딕셔너리
딕셔너리(01001ㅁ0ㅁ231)는 사전(단어:뜻)처럼 key: value’ 로 구성되어 있는 자료 구조입니다.
데이터의 추가와 삭제도 가능합니다.

1 d= {'Kim':123, ‘Lee':456}
2  type(d)

Out dict

1 d['Choi'] = 789 # 딕셔너리에 데이터 추가
260

Out {‘Choi': 789, ‘Kim’: 123, ‘Lee’: 456}

1 del 이 'ㄴ66] # 데이터 삭제
2 0

out {'Choi'’: 789, 0": 123} 할:
딕셔너리에 데이터 쌍이 몇 개가 들어 있는지는 160 (딕셔너리 명 )으로 알 수 있습니다. 딕셔

너리는 데이터에 직접 접근하기 쉽습니다. Key: value 쌍을 가져오려면 16605 ( ), 6\만 가
져오려면 keys (), 42106만 가져오려면 431465 ( )를 사용합니다.

394 부록 파이썬 프로그래밍 기초



===== PAGE 395 =====
1: d[{‘Park'] = 134
2 ten)

1 d. items()
Out dict -items((( Kim', 123), (' Choi', 789,  S Park’,  , 1397)

Teds keys()

Out dict -keys(C Kim',  “choi *Park'])

1   d. values()

Out dict vatues((123,, 789, BA)

A.4 반복문

forsee. 정해진 구간을 순차적으로 진행하며 USS 실행합니다. 기본 PRE 다음과 같습
니다. 실행할 내용은 들여쓰기를 합니다. 들여쓰기가 끝나면 *0「가 실행할 내용이 끝남을 의
미합니다. *「문은 SASHA] 사용할 수 있습니다. 다음 구조에서 실행할 내용 부분에 또 다른
foro] 들어갈 수 있다는 의미입니다.

1아문의 구조

for 변수 in 범위:
실행할 내용

다음은 리스트를 공부할 때 만들었던 0ㅁ1665에 있는 값들을 하나씩 출력하는 예제입니다.

1 prices # pricesO 뭐가 담겼는지 확인해봅니다.

Out [100, 200, 300, 500, 600, 700, 200]

부록 파이썬 프로그래밍 기조 395


===== PAGE 396 =====
1 700 ㅁ 10 01665: # pricesO] 담긴 WSS 변수 pol] 할당해서 루프를 돌립니다.
2    EHC 가겨은 | » 0, '입니다.')

Out 가격은 100 입니다.
가격은 200 입니다.
가격은 300 입니다.
가격은 500 입니다.
가격은 600 입니다.
가격은 700 입니다.
가격은 200 입니다.

A.5 제어문

입력된 조건이 참인지 거짓인지 판단하고 결과에 따라 실행을 달리하는 것을 제어라고 하며
1*문이 대표적입니다. 1*문의 FAL 다음과 같습니다. 1*문에서도 실행할 내용은 들여쓰기
를 해야 합니다.

if 조건 1:

조건 1이 HA 때 실행할 내용
elif 조건 2:

조건 2가 참일 때 실행할 내용
6156:

모두 거짓일 때 실행할 내용

elif} 6156는 생략할 수 있습니다. 둘 다 생략된다면 조건 1이 참인 경우에는 내용을 실행하
고 거짓인 경우에는 아무것도 실행하지 않고 지나갑니다.

다음 예제는 가격을 입력받고, 입력받은 가격이 1만 원보다 낮으면 매수, 높으면 매도, 1만 원
이면 SAS 표시하는 1+문입니다.

396 부록 파이썬 프로그래밍 기초



===== PAGE 397 =====
p= int(input(.))  # Feats 입력받아 pol] 저장

2000『()으로 값을 입력받음

inte 입력받은 값을 정수형으로 변환

UF 정수형으로 변환해야 숫자로 인식해서 7문을 통해 대소 비교가 가능

if p < 10000: # 10000원보다 낮으면
00106('매수')

elif p > 10000: # 10000원보다 놓으면
0「10【('매도')

6156:

# 위 조건이 모두 틀리다면

12      print('SH')

wo mont nun fF WN =

PR
en)

Out 11000
11000
매도

부록 파이썬 프로그래밍 기초 397



===== PAGE 398 =====
마이크로웨이브

마이크로웨이브(21070\36)는 말 그대로 극초단파를 말합니다. 가정에서 사용하는
전자레인지도 마이크로웨이브라고 부르는데, 극초단파를 이용해 음식을 익히는 데 이
용하지요. 여기에서 말하는 마이크로웨이브는 금융 용어라기보다는 통신 용어인데, 초
고속 통신을 위한 통신 인프라를 말합니다. 광케이블로 연결하기 힘든 도서 산간 지역
에 통신망을 제공하기 위해 이동통신 회사들이 많이 이용해왔습니다. 우리 주변에서
보이는 마이크로웨이브 시설로는 남산 서울타워에 있는 커다란 안테나, 방송국 옥상에
있는 커다란 안테나 등이 있습니다.

앞에서 소개했듯이 HFTS 위해서는 빠른 통신 속도가 생
명인데, 경쟁자보다 빠른 통신 SES 확보하기 위해 마이
크로웨이브 통신망이 금융업계에 도입되었습니다. 기존의
광통신망은 땅속에 매설되는 방식으로 설치되는데, 길이
구불구불하면 광케이블 역시 구불구불하게 설치됩니다.
반면 마이크로웨이브는 송수신탑을 세우고 초단파를 싸서
통신을 하는 방식입니다. 광케이블이 다음 그림에 있는 파
a 점선처럼 설치된다면, 마이크로웨이브는 빨간 직선처

이용하려고 합니다.

금융권에서 마이크로웨이브는 뉴욕(현물시장인 뉴욕증권거래소(45 )와 나스닥
(NASDAQ) 소재)과 시카고(파생시장인 시카고상품거래소(ㅇ46 )와 시카고옵션거래소
(CBOE) 소재)를 연결하기 위해 이용되기 시작했습니다. 우리가 이 책에서 계속 공부
해온 것처럼 현물시장에서 각 종목의 시세가 결정되고, 이 시세들을 모아 지수를 산출
합니다. 이렇게 산출된 지수는 파생상품 가격 산정의 기준이 되기 때문에 남보다 먼저
지수를 산출해서 주문을 할 수 있으면 HFTS 성공하게 되는 것이지요. 뉴욕에서 산출

398 부록 파이썬 프로그래밍 기초



===== PAGE 399 =====
된 지수를 바탕으로 시카고로 먼저 주문을 하기 위해 마이크로웨이브를 사용하기 시작
한 것입니다.

우리나라는 현물과 선물 모두 한국거래소에서 거래되긴 하지만 정치적인 이유로 현물
은 서울에서, 파생은 부산에서 거래되고 있습니다. 한국 HET 트레이더들은 ETF 거래
에도 마이크로웨이브를 이용합니다. ETF NAV7} 지수를 기준으로 결정되기는 하지
만, 시장에서의 거래는 선물가격에 영향을 많이 받습니다. 81마다 의무적으로 지정

는 Ｌ『?가 호가를 제출할 때 헤지가 용이하도록 지수보다는 지수선물 가격을 참고해
호가를 제출하기 때문이지요. KOSPI200 ee 경우 ETF AAS 할 때마다 헤지를
위해 200개 종목을 매매하는 것보다 KOSPI200 선물을 매매하는 것이 쉽기 때문이죠.
HTF 트레이더는 ㅁ『보다 먼저 호가를 제출해서 LP 호가에서 차익을 남기는 거래를 합
니다. 그래서 부산에서 지수선물 가격이 결정되면 바로 서울로 ETF 호가를 제출하는
HFT 거래를 하도록 마이크로웨이브를 이용합니다.

부록 파이썬 프로그래밍 기초 399



===== PAGE 400 =====
~                  ~        wv
금융             | 빅데이터 |  파이썬  |

= eda 딱 필요한 만큼만 배우고

금융공학에서 프로그래밍은 본질이 아닌 도구입니다. 금융공학자가 최고의 프로그래머가 될 BLE 없지요.
이 책의 모토는 '딱 필요한 만큼만 배워서 바로 활용하기'입니다. 금융권에서 가장 일반적으로 활용ㅇ
선물, 옵션, 펀드 이론을 배우고, 엑셀로 개념을 실습합니다. 이를 토대로 상품을 설계하거나 위험을
투자 전략을 결정하는 등 금융공학 모델링을 실제 파이썬으로 코딩해봅니다. 각 주제에 대해 이 과정
하며 금융공학 입문자가 알아야 할 내용을 확실하게 알려줍니다.

A
g
ed

‘i

바보
[~

는 금융공학 입문서.

생이라면 꼭 알아야 할 내용이 모두 담겨 있는 Ct 한 권의 필독서.

예제 소스 https://github.com/finterstellar/download

데이터 과학 / 데이터 분석

|    93000

9 791162 240823
정가 28,000원 16684 979-11-6224-082-3

