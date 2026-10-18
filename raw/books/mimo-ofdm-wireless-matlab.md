---
source_url: /run/media/yutae/Data/MIMO_OFDM_무선통신.pdf
title: MIMO-OFDM 무선통신과 MATLAB
subtitle: MIMO-OFDM Wireless Communications with MATLAB
author: 조융수 · 김재권 · 양원영 공저
publisher: 홍릉과학출판사 (Hongreung Science Publishing, 2008, Copyright 2008)
year: 2008
pages: 728 (scan)
ingested: 2026-10-18
sha256: 2514da74eb3455151697d2999660033a958d9bab3c34b4b52ae7cff56fb0c342
---

# MIMO-OFDM 무선통신과 MATLAB (raw source)
> **Note:** Korean original textbook (NOT a translation — 저자 일동 2008년 7월, 홍릉과학출판사). scan-only PDF (UPDF), OCR'd via tesseract 5.5.3 (kor+eng, 300dpi); equation/formula and MATLAB-code tokens frequently garbled (e.g. "10054668" = 100Mbps) — cross-check original PDF.
> **Distinction:** 조융수 · 김재권 · 양원영, 홍릉과학출판사 2008 — **NOT** related to Harada/Prasad or the latest mobile communication systems (different author, different book).

## 장 (chapter) structure (from OCR'd TOC)
| # | 내용 (topic) |
|---|------|
| 1 | introduction: 3G→IMT-2000/IMT-Advanced (1Gbps nomadic / 100Mbps high-speed mobility) wireless broadband, OFDM fundamentals |
| 2 | SISO channel modeling: Rayleigh/Rician fading, indoor/outdoor channel modeling |
| 3 | MIMO channel modeling: I-METRA, SCM, SCM-E, IEEE 802.11 TGn |
| 4 | OFDM: single/dual-carrier, basic principle, guard band, coded OFDM, OFDMA access, resource allocation, duplexing |
| 5 | OFDM synchronization: symbol timing/carbon/sampling clock offset, estimation techniques, cellular synchronization |
| 6 | channel estimation: overview, comb/comb/Pi structure, training signal estimation, interpolation, decision-directed, DFT, blind, EM, high-speed mobility |
| 7 | PAPR: overview, reduction techniques |
| 8 | inter-cell interference: adjustment/coexistence/elimination |
| 9 | MIMO capacity: eigenvalues, deterministic MIMO channel capacity |
| 10 | (MATLAB simulation integration) |

sha256 placeholder to be replaced


===== PAGE 1 =====


===== PAGE 2 =====
Copyright © 2008 by Hongreung Science Publishing

All rights reserved. No part of this book may be reproduced, stored or transmitted in any
form or by any means, without the prior written permission of the authors or the publisher.
Requests for permission or further information should be addressed to Hongreung Science
Publishing.

Limits of Liability and Disclaimer of Warranty of Software

The authors and publisher of this book have used their best efforts and knowledge in
preparing this book as well as developing the computer programs in it. However, they make
no warranty of any kind, expressed or implied, with regard to the programs or the
documentation contained in this book. Accordingly, they shall not be liable for any incidental
or consequential damages in connection with, or arising out of, the readers’ use of, or
reliance upon, the material in this book.

The reader is expressly warned to consider and adopt all safety precautions that might be
indicated by the activities herein and to avoid all potential hazards. By following the
instructions contained herein, the reader willingly assumes all risks in connection with such
instructions.

MATLAB" and Simulink” are registered trademarks of The MathWorks, Inc. and are used
with permission. The MathWorks does not warrant the accuracy of the text or exercises in
this book. This book’s use or discussion of MATLAB" and Simulink” does not constitute
endorsement or sponsorship by The MathWorks of a particular pedagogical approach or
particular use of the MATLAB” and Simulink”. For MATLAB" and Simulink” product
information, please contact:

The MathWorks, Inc.

3 Apple Hill Drive

Natick, MA 01760-2098, USA

®: 508-647-7000, Fax: 508-647-7001

E-mail: info@mathworks.com

Web: www.mathworks.com



===== PAGE 3 =====
머

멀티미디어 시대를 맞이하여 대용량의 데이터를 고속으로 전송해야 할 필요성이
어 급격히 증대되고 있다. 특히 인터넷을 통한 음성, 비디오, 데이터 통신이 최근
가하고, 셀룰러 통신 시스템이 급속히 보급됨에 따라 이동 중에 사용할 수 있는
무선 광대역 멀티미디어 통신에 대한 기대가 증가하고 있다. 3 세대 이후(66000
IMT-2000)2] IMT-Advanced 시스템에서는 Nomadic 환경에서 1 Gbps, 고속 이동 환경
에서 10054668를 목표로 한다. 이와 같이 무선 채널에서 데이터를 고속으로 전송할 경우
에 무선 채널의 다중경로의 영향으로 인하여 높은 에러율을 갖게 되어 무선채널에 적힌
한 무선접속방식이 요구된다.

Je
rm

OFDM 전송방식은 전체 전송대역을

=
널로 데이터를 동시에 전송하는 방식으
=

may
4)
412
rat
고
」요
내
EI

1
~
mT
Hu
Ac
웹
위
2
BS
4r
2

직
변조와 HAS 각각 IFFTS} FFTS 사용하여

두 08044 심볼 사이에 삽입하여 심볼간
간섭을 AAS 수 있기 때문에 등화기의 구조가 매우 간단해지는 장점이
있                              택되었다. 08014은 DMB} DVB-T 방송 시스
템의 전송 방석으로 사용되며, 고속 무선 LANS] 표준인 IEEE 802.11a9] 전송 방식,
『125/)으로 사용된다. 또한 Mobile \141ㅅ×(와이브로)
의 하향링크 및 상향링크 전송 방식으로 사용되며, 3GPP LTE 시스템의 하향링크 전송
방식으로 채택되었다. 유선망에서도 고속의 데이터 ASS 위하여 OFDMS| 유선 버전에
해당하는 DMT 방식이 ADSL 및 VDSL(Zipper Duplexing) 시스템의 전송 방식으로 사
또는 수신단에 다중 안테나를 사용하여 고속의 데이터를 높은 신뢰
는 MIMO 전송 방식이 최근 활발히 연구되고 있으며 이동/고정
A 통신 시스템의 표준으로 채택되었다. MIMO 전송 방식은 고속 무선 LANG] 표준
IEEE 802.11nz} Mobile WiMAX(2}°]2# 2) 및 3GPP LTE 시스템의 하향링크 및 상항
링크 전송 방식으로 채택되었다.

2
리
Sb»
1°,
× [쏘면
ob
ay
[>
at
412,
KI
AN
ro.
10
Hu
at

Se
|»
ne

ㅇ
보니
of»
ok
티스
fo

r& 40

oa

이와 같이 MIMO-OFDM 방식이 무선 통신 시스템의 전
와 관련된 좋은 책들이 최근 출간되었다. 그러나 대학에서

방식의 주류가 되면서 이
부하는 학생과 산업체에서

ok} of

003



===== PAGE 4 =====
MIMO-OFDM 무선 통신과 MATLAB

실제 개발에 참여하는 엔지니어들이 이 분야의 실제적인 지식과 경험을 습득하는 데에는
어려움이 있다고 느껴 이 AS 저술하게 되었다. 이 책에서는 무선 채널, OFDM 전송 방
식, MIMO 전송 방식의 기본 원리를 엔지니어들이 이해할 수 있도록 가능한 쉽게 기술
하였으며, 실제 MIMO-OFDM 시스템에서의 적용 예를 다양하게 기술하였다. 또한 각 단

원의 주요 내용을 MATLAB 프로그램을 통하여 확인함으로써 개념을 쉼게 이해할 수 있
SS 하였다. 따라서 초보자뿐만 아니라 davis 스스로 다양한 Fal 채널 환정을 7
성하고 여러 전송 방식들을 실제로 테스트하여 그 결과를 분석함으로써 다양한 개넘을
쉽게 이하할 수 있을 것으로 기대된다. 또한 MIMO-OFDMG} 관련된 새로운 VAISS
개발하고 검증하려는 엔지니어들이 이 책에서 제공하는 MATLAB 프로그램을 이용함으

로써 개발에 소요되는 시간을 절약할 수 있을 것으로 기대된다.

이 책의 PART 1에서는 무선 채널 모델링 기법에 대하여 설명하고, MATLAB 프로그
램을 통하여 WSS 확인한다. 1 장에서는 무선 채널 SYOHA large-scale 페이딩 특
성, small-scale 페이딩 특성, 페이딩의 통계적 특성에 대하여 설명한다. Large-scale 페이
딩 모델로서 일반적인 경로 손실 모델, Okumura/Hata 모델, IEEE 802.160 모델에 대하
여 설명한 후, MATLAB 프로그램을 통하여 확인한다. 2 장에서는 옥내/옥외 SISO A
널   나 피피   에 대하여 설명한 후, MATLAB 프로그램을 통하여 확인한다. 옥내 채널

fd
in
ot
is
a3

반적인 옥내 채널 모델링 기법, IEEE 802.11 채널 모델링 기법,

ol”

르    으로   eu
S-V ae    델링 기법, UWB 채널 모델링 기법에 대하여 다룬다. 옥외 채널 모델링 기
법으로는 FWGN 모델링 기법, Jakes 모델링 기법, Ray 기반 모델링 기법, 주파수 선택
적 페이딩 채널 모델링 기법, SU 채널 모델링 기법에 대하여 다룬다. 3 장에서는

MIMO 채널 모델링 기법에 대하여 설명한 후, MATLAB 프로그램을 통하여 확인한다.
통계적 MIMO 모델의 공간 상관과 PAS 모델 등의 기본적인 YRS 설명한 후, 주요
USSMATLAB 프로그램을 사용하여 확인한다. LMETRA MIMO 채널 모델링 기법과
SCM MIMO 채널 모델링 기법을 설명하고, Ray 기반 모델의 공간 상관에 대하여 설명
한다. 마지막으로 SCM-E MIMO 채널 모델과 TERE 802.11 TGn MIMO 채널 모델에서
고려하는 차이점에서 대하여 기술한다.

이 책의 PART 에서는 OFDM 전송 방식에 대하여 설명하고, MATLAB 프로그램을

통하여 USS 확인한다. 4 장에서는 OFDM 기본 원리를 설명한 후, MATLAB 프로그
Ue 통하여 주요 USS 확인한다. 이를 위하여 먼저 단일 반송과 전송 방식과 다중
송파 전송 방식에 대하여 설명한 후, 이 두 방식의 장-단점을 비교한다. OFDMA] om

ra

원리, Coded OFDM 방식, OFDM 다중 접속 기술. 0『0\4에서의 부채널 할당 방식과
부채널 맵핑 방식, OFDM 시스템에서의 Duplexing 기법에 대하여 설명한 후, 주요 부분
에 대하여 MATLAB 프로그램을 통하여 확인한다. 5장에서는 OFDM 시스템에서의 동

004



===== PAGE 5 =====
기화 기법에 대하여 설명한다. OFDM 시스템에서의 심볼 타이밍 옵셋과 반송파 주파수
옵셋의 영향 및 추정 기법에 대하여 설명한 후, MATLAB 프로그램을 통하여 확인한다.

또한 OFDM 시스템에서의 샘플링 클럭 위상과 샘플링 클럭 주파수 옵셋의 영향과 보상
기법에 대하여 설명하고, OFDM 셀룰러 시스템에서의 하향링크 및 상향링크에서의 동기
화 기법에 대하여 설명한다. 6 장에서는 OFDM 시스템에서의 채널 추정 기법에 대하여
설명한다. OFDM 시스템의 채널 추정을 위한 기본적인 기법으로 훈련 신호 기법 (LS
채널 추정 기법, MMSE 채널 추정 기법)과 0609100-0160660 채널 추정 기법, 그리고 채
널 보간 기법에 대하여 설명하고, MATLAB 프로그램을 통하여 확인한다. 또한 최근 연
구가 많이 이루고 있는 DFT 기반 채널 추정 기법, Superimposed ASS 이용한 채널
추정 기법, Blind 채널 추정 기법, Expectation Maximization 채널 추정 기법, 고속 이동
시 채널 추정 기법에 대하여 설명한다. 7 장에서는 PAPR 감쇄 기법의 주요 개념과 널
리 연구되고 있는 PAPR 감쇄 기법에 대하여 설명한다. PAPR 감쇄 기법으로 클리핑과
필터링 기법, PAPR 감쇄 부호, Selective Mapping 기법, Partial Transmit Sequence 기
법, Tone Reservation 기법, Tone Injection 기법, 그리고 3GPP-LTE2] 상향링크 표준인
DFT 확산 (SC-FDMA) 기법에 대하여 설명한다. 8 장에서는 OFDM 셀룰러 시스템에서
의 셀간 간섭 완화 기법으로 셀간 간섭 조정 기법, 셀간 간섭 랜덤화 기법, 셀간 간섭
제거 기법에 대하여 설명한다.

to
2

oi

이 책의 PART 111에서는 MIMO 전송 기법에 대하여 설명하고, MATLAB 프로그램
을 통하여 내용을 확인한다. 9 장에서는 송신부에서 채널 정보가 가응할 때와 가용하지
않을 때의 Deterministic MIMO 채널 용량과 랜덤 MIMO 채널 용량에 대하여 설명한
후, 주요 USS MATLAB 프로그램 “  통하여 eos 10 장에서는 공간 다이버시티
와 시공간 부호화 기법에 대하여 설명한 후, 주요 내용을 MATLAB 프로그램을 통하여
확인한다. 시공간 블록 부호로는 Alamouti 부호, 실수복소 신호 시공간 블록 부호, 그

의 일반적인 시공간 블록 부호에 대해서 다루며, 시공간 trellis 부호의 부호화와 복호
화 기법을 예제와 MATLAB 프로그램을 통하여 살펴본다. 11 장에서는 공간 다중화
MIMO 시스템의 신호검출 기법으로서 선형 검출 기법, 0910 검출 기법, ML 검출 기
법, Sphere Decoding(SD) 기법, QRM-MLD 검출 기법, [80166 ReductionS 활용한 기
법에 대하여 살펴보고, MATLAB 프로그램을 통하여 확인한다. 또한 MIMO 시스템에서
의 Soft Output 발생을 위한 최적/준최적 11# 연산 기법에 대하여 설명한다. 12 장에서

는 다이버시티-다중화 Trade-off 시공간 부호화 기법으로서 Full-diversity Full-rate 시공
블록 부호와 선형 분산 부호에 대하여 설명하고, 주요 Yee MATLAB 프로그램을
하여 확인한다. 13 장에서는 채널 정보를 활용한 송신 기법으로서 송신부에서의 채널
정 방법, Precoding 기법, 안테나 선택 기법에 대하여 설명하고, 주요 yes

ries

Wot 뿌 대

005



===== PAGE 6 =====
MIMO-OFDM 무선 통신과 MATLAB

MATLAB 프로그램을 통하여 확인한다. 14 장에서는 다중 사용자 MIMO 시스템의 상
향/하향 링크 채널 용량과 다중사용자 MIMO 시스템에서의 하향링크 송신 기법에 대하
여 설명하고, MATLAB 프로그램을 통하여 주요 USS 확인한다.

이 책의 PART 14에서는 MIMO-OFDM 무선 통신 시스템에서의 적용 예를 설명한
다. 15 장에서는 IEEE 802.118 규격과 프레임 구조에 대하여 살펴본 후 SimulinkS 통
하여 확인한다. 또한 IEEE 802.117 규격 과 프레임 구조에 대하여 설명한다. 16 장에서
는 DMB3} DVB-T 시스템의 전송방식과 규격에 대하여 살펴본다. 17 장에서는 UWB
시스템에서 사용되는 MB-OFDM 전송 방식의 규격에 대하여 살펴본다. 18 장에서는 와
이브로 시스템에서의 프레임 구조, 부반송파 할당 기법, 하향링크 동기화 기법, 상향링크
제어 채널, 채널 코딩과 H-ARQ, 하향링크 MIMO 기법, MIMO 기법, AAS 기법, MAC
계층에 대하여 설명한다. 19 장에서는 현재까지 진행된 표준화 기고문을 바탕으로 3GPr
LTE 시스템의 하향링크와 상향링크의 프레임 구조, 물리 채널 구조, 기준 신호, 랜덤 엑
세스 절차 및 타이밍 제어, MIMO 기법에 대하여 설명한다.

이 AS 현재까지 진행하였던 MIMO-OFDM 24] 알고리즘 개발 및 FPGA 구현 연구
결과이기 때문에 그동안 무선 채널 모델링, IEEE 802.11a/n, DMB, DVB-T, MB-OFDM,
ADSL, VDSL, 와이브로, 3GPP-LTE 개발에 참여하였던 전원기박사, 박경원박사, 이미현
박사, 김찬규박사, 정혁구박사, 이규인박사, 백종호박사에게 감사드린다. 또한 연구와 개발
의 바쁜 일정 가운데에서도 많은 도움을 준 중앙대학교 전자전기공학부 디지털통신연구실
의 우경수, 위정욱, 김영준, 박창환, 유현일, 고요한, 임태호 박사과정 및 강현진, 장은석,
박종혁,김진민, 김석기, 윤원정 석사과정 대학원생, 그리고 연세대학교 디지털통신연구실
허훈, 우현명 석사과정 대학원생에게 깊은 GAS 드린다. 이 Ao] 내용과 MATLAB =
로그램 전체적인 부분에 걸쳐 그들의 노고가 깃들어 있기에 이 책이 완성될 수 있었다.
마지막으로 이 책을 출간하는 데 물심양면으로 도와주신 홍릉과학출판사 사장님과 실무자

여러분께 감사드린다.

2008년 7월 저자 일동

때 006



===== PAGE 7 =====
GE 무선 채널 see MATLAB / 17

제 1장 무선 채보 특섰 rvvwsvtssenssnsninsennsnnspcessanssrananscncnssycsnnesonnssansnoanvanennsess

1, 1   Large-scale  페 이덩 ieieisinieioeieieieeieistelo'aleteiatieieieteloruto ouiatsvelow'v/dte euressle rere biaterewis-esstorewneiownlansiaweistie glares

144  일반적인 경로 손실 모델 C7 hor scec pac c COS TEC aS TC Ponsnonccoee ac osodonencacooconnesncemecon
1188  Okumura/Hata 모델 POC OT COE ECE ECE OTT De CO Eee)
1.1.3 IEEE 802.16d 모델 ee re ee ee eon

iL 2 Small-scale  페이 덩  ee ee ee eo ee Oe re

1.2.1 시간 지연 확산에 .의한 POPE 영향 ceeeeeceeecsseeeseseeecnneeenneeenneeseneeeenes
1.2.2 도플러 확산에 의한 페이딩 영호

1 8 페이팅의 통계적 특성 ee ee

제2장 SISO 채널 모델링 66 16.010401410.416441446.44북24~46410419149서16100

2.1 Rayleigh 페이딩 채널과 Rician 페이딩 채널 creer

22 옥내 채널 모델링 기법 00000000096사00000000000000000000000000000000000000000000000000000000

9 .9.1 일반적인 옥내 채널 모델링 2 법 eereerrernersemsrercromeereornrasssennarnensens
2.9.9 18008 802.11 채널 모델링 기법 …아아아아아아아바바아타타아아이아이이아이이아아아아아
DDB SHV 채널 모텔링 기법 eessessessestesssssssesseeneeneenrensenncanennsensencnnsenseneesees
224 UWS 채널 모델링 기법 penmeconemmmomenememmnenn

2.3 옥외 채널 모델링 기법 oe eee ee ere errr

2.38.1 FWGN 모델링 기법 지어 Ep antanensinnadeSGsenwasitnn mieentnaersonewennsernumizeaevererenane
2.3.9 Jakes 모델링 기법 cercreceeeeeeeeeeeeseesessessesseeeeeesseeeseeseseseesesseseseees
2.3.3 Ray 기반 모델링 기법 …어어어애애아새사사사아아사시아사시시사시시이이이이이이이이이이이이사

007 0”


===== PAGE 8 =====
MIMO-OFDM 무선 통신과 MATLAB

2.3.4 주파수 선택적 페이딩 채널 모델링 기법 ㆍ……어아아아아아아아아아아아아아아아 99
2.3.5 SUL 채널 모델링 기법 아에아아아아아사사사사타타타이이이이이이아아아아아이이이에사사아아어 104

제 3 4} MIMO 채널 모델링 sa 00020 111
31 통계적 MIMO 모델 SaSus buise evens sunsets wes wreeusseeeress ures eserwesuenreeeseeseseetereeewes 111
3.1.1 공간 상관 ……아어아아아아아아사사어어아사사이어이아사사이아시이이이사어아이사아 115
3.1.9 PAS 모텔 cesceeseeeseesseseesseseeesesteeseeessestseneseeeeteeneeseeteeeeeensessseneseneeneesaes 116

3.2 I-METRA MIMO 채널 모델링 기법 see ee eee eeeeeeneneeneeeeneeeseseaeeseueees 125
3.2.1 상관 기반 MIMO 페이딩 AAS] 통계적 모텔 ………아아아아아아아아아아아 126
3.2.2 상관성 있는 MIMO 페이딩 채널 생성 방법 ………아아아아아아아아아아아아아 130
3.2.3 I-METRA MIMO 채널 모델링 기법 ㆍ어에아아아아아아사사사사사사아아아아아아아아 199
3.9.4 3GPPol] 제안된 MIMO 채널 모텔 ……에에아아아아아사사사아아아아아아아아아아아아아 136

3.3 SCM MIMO 채널 모델링 기법 00000000000000000000000000000000000000000000000000000000 141
3.3.1 SCM 링크 레벨 채널 파라미터 ……에아아아아아아아사아아아아아아아아사아아아사아아아 142
3.3.9 SCM 링크 레벨 채널 모델링 기법 ………아아아아아아아아아아아아아아이아아이이이아아 145
3.3.3 Ray 기반 모델의 공간 상관 ……아어아아아아아사사사아아아사사사아사사사사아아사사사어 147

38.4 SCM-E MIMO 채널 모델 0000000000000000000000000000000000000000000000000000000006090=00 151
3.5 IEEE 802.11 TGn MIMO 채널 모델 seo a 6a Sasa a ARN ANNE UNOS New NEE EN EOS 153

CG 야미/과 MATLAB / 155

제 4 장  OFDM 기초 sees sactaberekeeeeesnss beawisdesceabnaciasesnedousseseetusesancecscueviwencaase ex 157
4.1 단일 반송파 AS 방식과 다중 반송파 전송 방식 ……………… 157

4.1.1 단일 반송파 전송 방식 ㆍ…아아아아아아아아사사아아어아이사사어사이시이이아이이이이기사아아어 157

4.1.2  다중 반송파 전송 방식 | 아아아어아아어서사사어어어아이이어사아어이사사이아이이어사어 162

4.1.3  단일 반송파와 다중 반송파 전송 방식의 비교 eieeteeaecevemeversesesases 173

4.2 OFDM 기본 원리 sinee us we: a:0:seierarolnn aler:nieceteensrene nial siassioiasieieeeieiaiein eninaisigee siemesigeseinncineeeusions 174

4.9.1 08104 변 C= SEES 174

4.2.2 OFDM 보호 구간 ee 182

42.3 OFDM 보호 대역 SC ENERO EERE ER RE NEED 191

4.2.4 OFDM 전송 방식의 BER 특성 CS ee ee Oe ee 193

_ 008



===== PAGE 9 =====
제 5 장

제6장

4.2.5 Water Filling 기법 ee Cero 198

A.2.6 OFDM 파라미터 설정 ……아아아아아아아아아아아이아아이아아이아이이이이이이이아이아아이아아 201

4.0 Coded OFDM PoeU eee er eer errr e creer errr er errr errr rrr rrr errr reer rere ers 203
4.4 OFDM 다중 접속 기술 Lee eee eee eep eee eeeneeaeveneeeeeeeneenseneseeeneeeeaeseesenseeeenns 205
4.5 OFDMAO]A] 2] 자원 할당 Ueessleeereevoreoeeeeensesveeevecsoescocovenconeeseeaesonseeees 207
4.5.1 OFDMAo]A]2] 부채널 할당 방식 | 아아아아아아아어아서사사새사사사아사아아아아아아사 207
4.5.2 OFDMA 부채널 맵핑 방식 …에에아아아아아사아아아이이이이이이이아아이이이아이이이사사아 210

4.6 Duplexing 기법 se eeeeeeeeeeoereeeeesetecerseeseeeseneeeeeceeeereenennesseaeeeerseseonseareesees 912
동기화 기법 ee ee ee ee TE rer ee er 914
5.1 심볼 타이밍 옵셋의 영향 Age NNSKO RAN CUNO MOR DURANT ARNT EN OONU STUNNER NO NUNENNRS ENO IEOINRS 214
5.2 반송파 주파수 옵셋의 영향 olsen EE KORNNN 218
5.2.1 정수배 반송파 주파수 QAO] 영향 ………아아아아아아아아아아아아아아아아아아아 221
5.2.9 소수배 반송파 주파수 옵셋의 영향 …………어아아아아아아아아아아아아아아아아아아 999

5.3 심볼 타이밍 옵셋의 추정 기법 66006 siodinnt velsihen{s\sienisiwersinsis sie clsie seh 993
5.3.1 시간영역 추정 기법 ceseeesecesseseseseseesesessseessssssscesesssseeseesevsecessnsesssees 224
5.3.2 주파수영역 추정 기법 아아아아아아아999999아이이아아아이이이이아아아이아아사 930

5.4 반송파 주파수 옵셋의 추정 기법 60010이이이이. 00101000010010.000.000000100010000000000 932
5.4.1 시간영역 추정 기법 아어어아어아아아아사사사아사사사사어시서서시사이이이이이이사사아아아사사아 232
5.4.2 주파수영역 추정 기법 ES 235

5.5 샘플링 클럭 위상 옵셋의 영향 aeesd se seveceseeeeseeeeeveseedy enews sdeseanedsoneseeees 238
5.6 샘플링 클럭 주파수 옵셋의 영향 ee RO ER Re CO OCR COTO CG 238
5.7  샘플링   클럭 SA 보상 기법 dab uroieasie emenwinriers us ereieaulataresRenesieleleeieiainesesieawenensse 240
5.8 셀룰러 시스템의 동기화 기법 | ia sue peevenssvensusenbuwedesevevensbeusswesoeresuneses 949
5.8.1 CS) oe Mo) Ss 243
5.8.9 상향링크 동기화 기법 EES 246
채널 추정 기법 0.00100000000.90101004.000400014.49040.000.0.09104910시시지이시시시이이이시이이이이0004100000004010090919 249
6.1  채 널 주    정 개요 eee tree eee rere eee eee eee eee eee eee eee ee 249
6.2 a+] al 구조 이00000000000000000000000000000000000000000000000000000000000000000000000000000000 249
6.2.1  블록 구조 cc 250

009


===== PAGE 10 =====
MIMO-OFDM 무선 통신과 MATLAB

62.2 Comb 구조 아어어어어어아어아사사사사아아사사시사시시이이이아시이아사이이사이사이이이이이사아아아아아 250
6.2.3 Lattice 구조 creeseseeeeeeseeeesteeeeseeeteeseneeeeeeseeesteeteresesesesenesenseerens 251

6.3 훈련 신호 기반 채널 추정 기법 vee be eeeeeeaeneen eee eeeneeaeeeneeeseneareeesesseoees 252
6.3.1 LS 채널 추정 기법 …어어어애사사새새새새사사사사사시사사시시시시시시시이새사사사아이아이아아 252
6.3.2 MMSE 채널 주정 기법 sad seaee oaniecadie cones eiees tease seeeesaeavinee see daveseeneieavansoes’s 254

6.4 보간 기법 000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 263
6.4.1 선형 보간 기법 Seedeecueeenaeseverseeedstendsesveseseanvecnsecnesesessecvtoceccnseonesoeessees 263
64,2 DRE 다항식 보간 ZT]  ceseseeseseseeesseeeeseseeeeesseseneeseeseseeseseseeseneesseesenens 264
6.4.3 Cubic Spline 보간 기법 000000070077070077717 264

6.5 Decision—directed 채널 추정 기법 00000000000000000000000000000000000000000.000000 268
6.6 DFT 기반 채널 추정 기법 000000000000000000000000000000000000000000000000000000000000000 269
6,7 Superimposed 신호를 이용한 채널 추정 기법 01000000000000000000000000004 972
6.8 Blind 채널 추정 기법 0000000000000000000000000000000000000000000000000000000000000000000 82974
6.8.1 Bussgang 알고리즘 ee O75
6,8,2 부공간 기반 채널 추정 기법 여어아어아아사서사사아아아어어어어이이이어이이사아아아아 276

6.9 Expectation Maximization 채널 추정 기법 00000 279
6.10 고속 이동 시 채널 주정 기법 0000000000000000000000900000000000000000000000000000000 288
제 7 2} PAPR 감쇄 기법 0106106100.01010000000000100000001010000004000.6604000006910000.00000402400009000 289
7.1 PAPR 개요 eee ee eee eee eee eee eee eee eee eee eee eee ee eee eee eee eee reer 289
7.1.1 PAPR 정의 caeeseeeseaeesonneeecessoessoneseaascnoeneeeneenaenanereaassneescaessenssoesseresenees 991
7.1.9 08044 신호의 ne 297
718 PAPR} 오버샘플링 Sea vebs sues seevewassewrcuesesereequeneaeerneessvseusueNeoneeswerses 301

7.2 PAPR 감쇄 기법 eer rere rere reer ere errr reer ee eee eereee eee ee eee eee eee 306
7.2.1 클리핑과 필터링 기법 ceeeeeeceeeeeeeeeteeeeeeseneetseneeeeeeeeseseeseeeseeesseseseesees 308
7.2.9 PAPR 감쇄 부호 ㆍ어어아아아새사사사사사사사사사사사시이이이기서시이사이이사아기사이이사이사아아 315
7,2.3 Selective Mapping 기법 siasysiawesmasesinenneceniinesieeaiunse:ntinsieWtnsivenmaiennnices aw eiseenele 318
7.2.4 Partial Transmit Sequence 기법 Sas ae CaNTEW NETRA calm UNEN NENG MEE 319
7.2.5 Tone Reservation 기법 deseeeesecssconesccsscessccnsccenesesessesesteestossseoasessees 394
7.2.6 Tone Injection 기법 이여서기개 techy snes {rato 베테 atenes teens Par eteas raewesea erences 326
7.2.7 DFT 확산 (SCHFDMA) 기법 :…아아아아아아아아아아아아아아아이아아이아아아어사사아아 329

010



===== PAGE 11 =====
차 례

제 8장 셀간 간섭 완화 기법 고드사지바라다 거 341

8.1 셀간 간섭 조정 기법 00000000000000000000000000000000000000000000000000000000000000000000000 341

Fos Oo a 341

8.1.2 전력 자원 할당 기법 srsseensefecanesecanesenensecsnansesnonsecnanssanassnanansceqenssssess® 343

8.1.8 BSE 간섭 조정 기법 …아어어아아아아아아아아아아아아아이이이이이이어이어어 345

8.1.4 동적 패킷 할당 dd 346

8. 1.5 HDD 방식 | 아아아아아아바아아아이이이이이이이이에이서 348

8.9 셀간 간섭 랜덤화 기법 …………아바아에아아아아이이아아아이이아이이이아사이이아아사사 350

8.9.1 셀간 간섭의 랜덤화 원리 아에어아아아아아아아사아아아아사사사사아아사이이이이어어이시이 350

8.9.9 Cell—Specific 스크램블링 기법 ……아아아아아아아아아사사아아사아아아아아사에아아 351

8.2.9 Cell—Specific 인터리빙 기법 아아아아아아아아아아아아아사어서서사아어어어새사사사사어 352

8.2.4 주파수 호핑 기법 아아아아아아아사아사사아아이이이이이아이어이이어이이시사시이사어 353

8.9.5 랜덤 부반송파 할당 기법 ……아아아아아아바에아아바아아아이아아아이이아아이이시이이기사사 354

8.3 셀간 간섭 제거 기법 reer eee eee eee 355

8.3.1 Interference Rejection Combining 기법 Fikuvenewseveenseeenecessreerecwens 355

8.3.2 다중 사용자 수신기를 갖는 TDMA 기법 ………아아아아아아에아아에에아아아아 356
GU mimos Matias / 359

제 9 장 MIMO 채널 용량 Pc i er re OC Oo 361

9.1 행렬 기본 이론 차띠티비티베이티비티터이디비티010101010.0:비비비이리디비비이디머이머미버니티어이더이키디비비비비디키비버제티이제티이비키버10서터지이지지0.410.41501524.4 362

9.2 Deterministic MIMO 채널 용량 이아이이09000000000000000000000000000000000000000 362

9.2.1 송신부에 채널 정보가 가용하지 않을 때의 채널 용량 ………… 363

9.2.2 송신부에 채널 정보가 가용할 때의 채널 용량 ………아아아아아아아아아아 366

9.2.3 8100와 MISO 채널 용량 아아아아아에에아아사아아사아아이이이이이이이이이이이에사사어 368

9.3 랜덤 MIMO 채널 용량 Serer ree ee 369

제 10 장 공간 다이버시티와  시공간 부호화 기법 Se EKENRH ESRI VERUSeME CTE SHeNTeTes 379

10.1 공간 다이버시티 oe ee 380

10.1.1 수신 다이버시티 아에어아아아아아사사사사사이어서시이이이사사어어시시이이사이어이이이이이사사에어 381

10.1.8 송신 다이버시티 아아아아아아아아아아아아아아아이아사아이어이이이어이어사이이사사이이시이1시1시사 386

011


===== PAGE 12 =====
MIMO-OFDM 무선 통신과 MATLAB

10 2 시공간 부호화 시스  tsisihwineinsiniee oS neie Ne(0 bn Selge'seee\b'ew besivie We eGUES Wess ee een eawetoseees 387
10.2.1 시공간 부호화 시스템의 개요 로아 Se ne Sec eee eee eee eae Taee eee ee 387
10.2.2 시공간 부호화 시스템의 Pair—wise 오류 확률 ceveeeeeseeeevees 388

10 3  시공간 블록 ro: 0000000000000000000000000000000000000000000000000000000000000000000000000000 391
10.3 1 Aiamoiti 기법 Waseca oespisesiee'ssiaievioeeswanesaeesebiessinesilssavesveeesteapenassearsstanatinns 391
10.3.3  일반적인 ^ 공간 블록 부호화기 Wintissoes ves edeevensesessedeeesvaseiuayavesswonses 396
10,3,3 실수 신호 시공간 BS 노0000000000000000000000000000000000002 397
10.3.4 복소 신호 시공간 블록 도 000000000000000000000000000000072 399
10.3.5 시공간 블록 부호의 복호 ……ㄴ………여여여아여이미애 401

10.4 시공간 Trellis 부호 RRs a EOE EEE TEER a Seen ewer seo eeciaw 405
10.4.1  시공간 Trellis 부호화와 복호화 이아아어서사사아사사사사사사아이이기새아사사아아아 405
10.4.2 시공간 Trellis 부호의 예제 …에에아아아아아아아아사사사사사사아이이이사아아아아아아아 408

제 11 4} 공간 다중화 MIMO 시스템의  신호검출 기법 81601 418

111 1 선형 검출 기법 ioe debe es wehnase ny ssieseaedebuessseeseasesedeedessekesteess denne cawenereenecooens 418

112 OSIC 검출 기법 이0000000000000000000000000000000000000000000000000000000000000000000600000000 419

11.3 ML 검출기법 이이사이00000000000000000000000000000000000000000000000000000000000000000000000000000 424

114 Sphere Decoding 기법 vee eseeceseevcecnasessecsaceseedoeecevesesesbospecsecbeseseseeceees 426

11.5 QRM-MLD 검출기법 sense eee ee nee neeeneneeeeeneeeeneeneeeeeeessaseesaeseesesbenecencesens 436

11,6 Lattice Reduction 활용한 기법 su swan eee eee neever de eeiwNeeNeeseueawesis ees 441
11.6.1 LLL 알고리즘 ceeeeeteesseeceeeesseeeessenseeesssesseeseeseessecsscssecseesseeseeseeenesaees 443
11.6.2 Lattice Reduction 기법의 활용 | 아아어아아아아서서아이이이사이이사이기사이이시이아아아 444

11.7 MIMO 시스템에서의 Soft Output 시사사사아사사아이이사아이이사아이이사아이이사아이아 448
11.7.1 LLR SEG crveseesscecsescsssesseesscessssscsecsssonecesscenssscessseessessesssseeanesnsensesees 448
11.7.2 MIMO 시스템을 위한 최적 ＬＬ 연산 ……아아…아아아아아아아아아아아아아아아 451
11.7.8 준 최적 LLR GAP …아에아아아아아아사사아이이아이이이이이이이이어이이이기사이이아이이아이 451

제12 A 다이버시티-다중화 「ㅜ8060-0 시공간 부호화 기법 ………… 456

12,1 Full—Diversity Full—Rate 시공간 블록 부호 ……아아아아 457
12.1.1 시공간 성상 회전 도 MES 457
12.1.2 Alamouti AES 이용한 시공간 성상 회전 부호 i siaiv snniesisie'cvise'wiai'eis 462

012



===== PAGE 13 =====
12.2 선형 분산 분 후 이이아아이시이 468

12.2.1 Hassibi2k Hochwald2] 기법 …아아아아아아아아아아아아아아아아이이이이이이이에세사아 468

12.2.2 Hearth2} Paulraj 2] As 아아아어어아어어아어어이이사사아이아이사사아아사어아아아아아아 466

제 13 장  채널 정보를 활용한 송신 기법 Leseessnu nun wanVibpKiendoxesnunoaunesadsatcenene 470

13.1 송신부 |서의 채널 추정 er eo 470

13,1,1 Reciprocity FIFE] seseeeeeeseepeeeeeseeesessenessenenecseessenenseneneceeneeeseenenanseneens 471

13.1.3 채널 정보 피드백 방법 ㆍ…아아어어아사서사셔여여어어어서이시시이이어사새사사사사사사사사 472

13,2 Precoding 기법 Oe ee 473

13.2.1 송신단에서 채널 ABS 활용할 APO] 채널 용량 ……………………“ 473

13.2.2 Pre—coded STBC 기법 ……아아아바바아바아사사사아타아아아아아아아아아아아아아아아아아이 476

1322 Pre-—coded 공간 다중화 시스템 메지메090900~00…~ㄴㄴㅋ94010 482

13.3 안테나 선택 기법 0000000000000000000000000000000000000000000000000000000000000000000000000009 494

13.3.1 안테나 선택 기법 적용 시 채널 용량 ……아아아아아아아아바아아아아사아아아아 494

13.3.2 선택 복잡도 감소 기 SE 496

HES tis eS STBCO]A] 2] 최소 오류 확률 아아아 아이오 아아아 이오. 498

제 14 장 다중 사용자 MIMO 기법 cuesSansa bb RIK NANSROTADSW OAD AERETASOAUADANDRRERIC CRED 501
|

                  14.1 다중 사용자 MIMO 시스템 모델 Seicerieye areMersiiesueyewannmNeN wee stcenemwrrsm= 502

14,2 다중 사용자 다이버시티 이이900000000000000000000000000000000000000000000000000000 503

14.3 다중 사용자 MIMO 시스템의 채널 용량 ……아아아에에에아에아아아아아아아 505

14.3.1 다중 사용자 MIMO 시스템의 상향 링크 채널 용량 ……………………“ 505

14.3.9 다중 사용자 MIMO 시스템의 하향 링크 채널 용량 …………………… 507

14.4 다중 사용자 MIMO 하향 링크 송신 기법 ………'아아아아아아아 508

14.4.1 Channel Inversion 기법 b0Cecereccessoeccecseeccseceseescceseoseseeeeseseeseseceeecees 508

14.4.2 Regularized Channel Inversion 기법 Seen aeeeeaaancean aan seeseN saree 510

14.4.3 블록 대각화(8100 Diagonalization) 7] occ 512

013


===== PAGE 14 =====
MIMO-OFDM 무선 통신과 MATLAB

GE imo-orpm 동신시스템 / 517

제 15 장 IEEE 802. 1la/n sanencd Sawuseeussssesesebossinesesecsuiosbseuaseunssevsauaanegnswenseincetns 519
15,1 TEEE 802, 11a cecesctsctreteeeetsessetsetteeteeteeesseteeteessenseensenseeseeeneseseenes 519
15.1.1 IEEE 802, lla 규격 및 기본 블록 ……아어아아아아아아아아아이이이아아아아사 520
15.1.2 IEEE 802.118 성능 분석 seMeendnesevenseetoee sone sewreeseseetusreeeaTeuesnsceaesnenss 527
15.1.3 IEEE 802. 1la 프레임 SEM seseeeeeteeeteeseeeseesesseesseseseeseeeseseessseeseeeees 530
15.1.4 TERE 802, 11a 똥기부 ㆍ에에아아아아아아아아아아이이이이이이이이이이이이이이사사아아이사아이 533
15,1,5 TEBE 802. 11a PLCP cevssesssesscssssssesssessesssssscssssesssecsecssseneseasensenneones 540

15.2 IEEE 802, 1la2} Simulink ccccrrcccresteceeteeeeeeeeeeeeeeeeeeeeeeeeceeneeeeeeeeeeees 544
15.2.1 TEBE 802, 11a 기본 블록 ……아아아아아아아야아아아이이이이이이이이이이이이이이이이이사아 544
15.2.20 TEEE 802.118 채널 추정부 ………아아아아아아아아아아아이이이이이이이이이이이이이이 547
15.2.8 IEEE 802.118 반송파 주파수 옵셋 추정부와 잔류 위상 Sal 추적부

이저0시이의서비 dessus deieeees tid sehssansasessssbuusbedeenenenise 551

SES as ee 00} 0) 0c] 0) ho556
15.3.1 TEEE 802,11 규격 및 기본 블록 ㆍ…아아아아아아아아아아아아아아아아아아아아이 556
15,3,2 IEEE 802.112 프레임 구조 …여어어아아아사사아야사아아이이이아아아아사이이이사아에아에 565

제 16 장  DMB/DVB  시스템 sacemnsdeccsisesensiesasue sane enqeady ena eu cseseheteus vesexaueseicuenas  571
16.1 방송 시스템의 개요 RUAN Dap n WNT NONE REASONED SNR Kae Se E NSE OMENS AR sh es WRerexenxreveTenKa® 571
16,2  DMB 시스템 Won ai oben iWt6 9/0018 eins aisle nti sniei's winiiesaie 6G 0 0d Winie oN b Ne Wle Bid cise pal ewacencewecssesecense 571
16.2.1 DMB 시스템의 개요 cietteeeseeeeeteteeetseseeseeeseeeseeeesesseesessseeeceeerseeseengs 571
16.2.98 DMB 시스템의 전송 방식 ㆍ……아아아아아아아아아사사아아아사사사사사사이이이이애아아아 572
16,2,3 DMB 전송 프레임 구조 ceveesceesceeeeeeeeeeeeeeeseceeeeeeeeseeeeeeesseeseseeeeesaees 575
16.2.4 DMB 물리계층 규격 crreceececeeeeeeeeeeeeeseeseeeseseseesesesesessseecscsessesseeeees 576
16.3 DVB 시스템 ee tre er rrr 583
16,3,1 DVB 시스템의 개 he MOSSES OSSESEEESRESEOOOOOS 583
16,3,2 DVB AJA BS] 전송 방식 ……아아아아아아아아사아아아아아아아애아이이이이어에사사아사아 584
16.3.3 DVB 전송 프레임 구조 Ee 584
16.3.4 DVB 물리계층 규격 …아아아아아아아아아아아아아아이이이이이이이이아이이이이이 586

014


===== PAGE 15 =====
차 례

제 17 A}  MB-OFDM 시스템 sence enon eeene ener ene ereeerenseeeeseee eee eneseasensenseeesenanesenes 593
17.1 UWB 무선 전송 방식 vee eeece nena pec eereeeeeceeeeereeeesencee ees eneneseessaresereeenesees 593
17.2 UWB MB-OFDM 전송 방식의 물리계층 규격 creer 595
10 8 MB-OFDM2] 동기화 절차 0000000000000000000000000000000000000000000000000000000 602

제 18 장  와이브로 시스템 cence ene eee eee voneceecedevensereessensonsessesaecseseeaeeansareasensones 604
18,1 와이브로 시스템 개요 ……여아어어아아아아아사아아아아아어아아아아이사아아어사사아사아사아 604
18.2 와이브로 프레임 구조 ………아아아아아아아아아아이이아이이이이어이어어이이이이이사사이이사 606
18.3 와이브로 부반송파 SHEP ……아아아아에아아아아아아아아아아아아이이이아사사사사이이어시이사 612

18.3.1 하향링크 PUSC vvvesereeseseeseesssessseseessseneeeensssessesesssssesssetsseeesesensssensees 613
18.8.2 하향링크 FUSC  cccsscsecsseevseccessccrsessssscersvsnsessecsnssescesssessssecoesseseseoeceees 617
18,3,3 상향링크 PUSC cevceeesssesssesesssssesesesssseseecsessseseesnesesssessessesneeecesseesaes 618
주주 (6울000000000000000000000000000000000000002 620
18.3.5 상ㆍ하향 링크 자원 할당 |………아아아아아아아아아아아아아아이아아아아이어사아이아야아 621
18.4 와이브로 프리앰블과 하향링크 똥기화 ……………아아아아아아아아아아아아 623
18.5 와이브로 상향링크 제어 채널 eTAsR UNG MNS NCES NNER ERI WsetenESEReKReesevewnes cette 625
18.5.1 레인징 채널 Wen sBAGias cewenSaaG coho s Steesncwusenssvor cou ypeNWadnyenessemsvenswswssienivnnwenaaiinen 625
18.5.2 G@I 2 널 64592 oy PEN SUR T Op US cenwaseareeowascescenwsnsesraaansnersnsanes 터시태져케어 627
18.5.3 ACK / NAK 채널 ee Se ere 630
18.6 와이브로 채널 코딩과 H—ARQ creresesttsesesetetseseeetessseeteeeesenseeeeeeeesees 631
18.6.1 컨볼루셔널 ao Ro) SS 631
18,6,2 컨볼루셔널 Turbo 부호화 ㆍ……여어애아아아아아사사아아이어아이이시이아이시이이이이기사 632
18,6,3 Hybrid ARQ verssrssssesssssesseesesssssessenesesseeneresesssesssesesseneesseeeeesenens 633
18.7 와이브로 MIMOS} I No RR 635
18.7.1 MIMO 하향링크 anuiecieh Rind cuvvaudinitanawveseeneRsemebauns ii eccvereueseanoncrnennee 635
18,7,2 MIMO 상향링크 sees ewan seven bievaseaa yaw aeWeveeswainvaesswuxsamnnnvasecanreeeserereseeaareses 638
18.7.3 추가적인 성능 향상을 위한 MIMO 기법 ceeseeeseseseseeeeeeseeseeeeeeeenees 639
18.7.4 AAS(Adaptive Antenna System) 0아아아아아사아아아아아아이이이아아이이이아아아 643
18.7.5 MIMO8} AAS2O] 비교 아아아아아아아아아아아아아아이이이이아아이아이이이이이이이아이이이사 645
18,8 와이브로 MAC 계층 …아아아아에아아아아자아이이이이이이아아사지이이이이이이이이어사이사사 646
18.8.1 와이브로 MACS] 기본 개요 …아아어에이어아아사사사사어사이이이이아아이이이이아사아 646
18,8,2 MAC 프로토콜 계층 구조 ㆍ……아아아에아아아아아이아이어아어이어아사이아아어 647
015


===== PAGE 16 =====
MIMO-—OFDM 무선 통신과 MATLAB

18,8.3  MAC PDU 구조 Sib sins Sinn Riis wana one VE ee NWUN RWW ES WER YATES EN EANEST SIG RTESONS OUST ORAS OIG 648
18.8.4 MAC 관리 메시지 We 5 Ge SRE RUT GU We SNN CUA INSEINGDINA cast penta cern tauevaveveressTey 650
18.8.5 초기 망 진입 절차 여어어아아아아아아아아사이어아이서이이이이아시이이이이이이이이이이이어어 651
18.8.6 레인징 절차 creeeresssseseeseeeeeeseeseseeetsneeseeseeeeecsssseeesesessessseesesseessenensseeees 653
18.8.7 슬립 모프 ceeeereessseeeeeseeeeeseeesetsessessesstenscsssenssssssecesseeesssscseesnecsenesenees 655
18.8.8 WE DY 절차 아아아아아아아아아이9아사아사이시이시지이시이이이이이이비이이이이이이아와 656
18 8 9 1016 몬트 secscerenceestececrareecoccennerscuereraseeas- snl ae creer detscearneseer ts 658

A] 19 장 SGPP LTE 시스템 …아아아아바아바아바아아아사아아아아아이아이자이이어서새사새사사아와 660
19.1 3GPP LTE 시스템의 개요 SOR seh i tiaemaaloawe sie one ovewwes eg reese eeoaesusiuraumnpacnaiie 660
19.1.1 BGPP LTE 요구 사항 에아아아아아아사아아아아이이시아이어사사이이사아어아어아아아아아아 660
19 1 2 3608 LTB 주요 특징 Swaleawn sea gaSNWNSRTENW de asReETe9usleaTSREOUSURS 사아메서지애매여매게제 661
19.2 3GPP LTE 하향링크 SSRs SAGER CSET EWES Tain wy sac Ue olde 비버리버 662
19.2.1 3GPP LTE 2S] 하향링크 구조 ㆍ아아아아아아아사아아아아이어이이이아이이이아아아이이 662
19.2.2 8GPP LTE 2] 프레임 구조 …아어아아아아아아아아아사사사이아사이이이이어아이이어사아어 663
19.2.3 3GPP LTE] 슬롯 구조 …아어아아사애아사사아사어어어이저사시시이이이사시시아사아아아아 664
19.2.4 3GPP LTE2] 하향링크 물리 채널의 기본 구조 ………아아아아 665
19.9.5 BGPP LTHS} 하향링크 채널 아에아어아아아아사사애사사사어이이아사사사사사사사사사사 666
19.2.6 3GPP LTE] 기준 AlS(Reference Signal) serene 668
19.2.7 3GPP LTE2] 동기 A4l&(Synchronization Signal) ss 672
19,3 3GPP LTE 상향링크 nell oelaa soit aloo Subs wig WW'ROISIN ee s WON EAU SSGGEN SENSOR NOSE IEA 675
19.3.1 30258 LTH OS] 상향링크 구조 ……어아아아어아아사아아아아아아아아아아아아아아아아아아 675
19.3.98 3GPP LTE2] SCHFDMA crrsstssstessssseteesesesseeesseesseseesesssscsseseeseenes 675
19.3.3 3GPP LTES) 상향링크 물리 채널의 기본 쿠조 ccrssessssnsnestsssennes 678
19.9.4 3GPP LTEO] 상향링크 채널 …아어아에아사사사사사사아아이아아아이시사사이이이사사아 678
19.3.5 30628 LTE©] 기준 AlS (Reference Signal) cress 680
19.3.6 30688 LTE 랜덤 엑세스 절차 및 타이밍 제어 ……아아아아아아아아아아아 682
19.4 3GPP LTE 시스템의 MIMO 기법 Sideesdensnescdererecceccanseyerseseusyiereseys 683
19.4.1 Layer 맵핑 ovine wok GUA NE TETSN SADE NT ONG STEEDS RESET ER STING RES GUAE NN VORRA Dine Saree prema aww 683
19.4.2 Precoding 기법 AGHRS CORSUANT RoR divnteaw eas sine oancusnewwaVkbowerenseauvensseuErsETesteSSeeINS 685
19.4.3 CDD 기법 aaa niin ey aN ne RCEE pen dT iycnRy KANN ERUEARKNRASRISAGITURSVATRAGI A tenn onneecenens 687
19.4.4 SFBC 기법 MAAN na RET Ren COEUR REN LOS 688
19.4.5 Virtual MIMO 기법 0000다다터다바베지버저버자라비기2나애10986 688

 참 고문헌 cereeeeseeeetsseeeeeeseseesessssesessssenenesnesseseesersasseereesevsnssssseecscsisnsssseeesseansneeseseesess 690
 찾아보기 SAN RAU Sn WRN CONER NIN ows inn op wine OlGW Cw DSE UUW SSIESSTNT SOW AUN TW RNMIAIY CWA NUIN SVN bab waned einiawa Ous'n 714

016


===== PAGE 17 =====
PART 그

무선 Hig 모델링과
MATLAB

제1장 무선 채널 특성
제2장 5150 채널 모델링

제3장 MIMO 채널 모델링


===== PAGE 18 =====
무선 통신 시스템에서 성능 향상을 제약하는 가장 큰 요인이 무선 채널 환경이다. 무선
채널은 정적이고 예측 가능한 유선 채널과는 달리 매우 불규칙적이며 정확한 분석이 쉽지
않아 무선 통신 시스템 분석 시 가장 어려운 부분 중에 하나로 인식되어 왔다. 최근에 무
선 통신에 대한 급격한 수요 중대와 이동통신 세비스 가입자의 폭발적인 증가로 무선 통
신 시스템의 최적화가 요구되고 있다. 경쟁력 있는 무선 전송 기술의 개발과 효율적인 주

수 사용 연구는 정확한 무선 채널 특성의 파악을 기초로 하고 있다. 무선 통신 채널에서
HOGS 유발하는 메커니즘은 1950~60년대에 HF(High Frequency, 3~30MHz), UHF
(Ultra HF, 300~3000GHz), SHF(Super HF, 3~30GHz) 대역 등에 처음 모델링되었으며,
현재의 무선 채널 HAS 800MHz~2.5GHz 대역에서 광범위한 채널 측정을 통하여 정립
된 것으로, 주로 사용되고 있는 ITU 채널 표준 WAS 제한된 주파수영역에서 SISO
(Single Input Single Output) 채널 모델을 표준으로 제시하고 있다. 또한, 차세대 이동
통신 시스템의 주요 특징인 고속 전송, 주파수의 고효율성 및 다중 안테나 기술의 적용을
위하여 요구되는 다중 안테나 무선 공간 채널 BAS 현재 IEEE 802, METRA 프로젝트,
3GPP/3GPP2, WINNER 프로젝트 등에서 개발 중이다.

페이딩 ABS 넓은 지역을 이동함으로써 발생하는 186-50816 페이딩과 송신단과 수
신단 사이의 공간적인 위치의 작은 변화로 Also] 진폭과 위상이 급격히 변하는
small-scale 페이딩으로 HES 수 있다[1]. 그림 1.1에 나타난 바와 Zo] large-scale 페
이딩은 거리에 따라 수신 신호의 평균 전력이 감쇄하는 APS 나타내는 경로 손실(084
1089)과 수신 신호가 평균 ABS 중심으로 변화하는 BAS 나타내는 91800\108으로 나
누어진다. Small-scale 페이딩은 다중경로 시간 지역 확산에 의하여 채널의 주파수 선택
적/비선택적 특성이 결정되며, 채널의 시간 변화 특성(도플러 확산)에 의하여 페이딩의 속
도가 결정된다.

019


===== PAGE 19 =====
PART 1 _ 무선 채널 모델링과 MATLAB

이동 통신 시스템에서 신호의 전파에 영향을 주는 기본적인 메커니즘은 다음 세 가지가

있다[21.

tAKreflection) : 전파되는 전자기파가 RF 신호의 파장 AW 비하여 상당히 큰 평탄

 표면에 BAA 때 나타난다.

(diffraction) : 송신단과 수신단 사이의 전파 경로가 Ao] 비하여 큰 규모를

IS= 가려졌을 때, 2차의 파동이 장애물의 뒤에서 발생되면서 veh 4

과 수신단 사이에 LOS(line—of-Sight) 경로가 없을 때 RF 에너지의 전달을

Joe, 수신단이 전파가 통과할 수 없는 장애물로 가려져 있더라도

파가 수신단에 이를 수 있기 때문에 이러한 현상을 91800\108이라고도 한다.

- AtEHscattering) : 전파가 크고 불규칙한 면이나 그 크기가 AYE 그 이하의 임의의 면
과 충돌하여 에너지가 전 방향으    때 또는 반사될 때 발생한다. 주로 가로등, 표지판

과 같은 신호의 반사나 산란을 일으키는 HAS 산란자(608060)라고 한다.

|
뜨

「

rok
Fel

|
fol

Wm of clo om py

ue
rh uot of ria

ii

Dy

r

iz
> eo

os
clr

때
Pa
i)

N

|

페이딩 채널의 메커니즘
|
|                                |
넓은 지역에서 이동에                작은 위치 변화로 인한
(t= large-scale 페이딩                  small-scale 페이딩

                            | ㄱ

|               |
ela 따른 수신 평균을 중심으로         다종 경로 시간
력      한 전

“(Path loss)       (Shadowing)             rie          et    딩

22 00

주파수 선택적 주파수 비선택적       시요            pi
기조    cl      a    더
페이딩         페이딩        고속 페이딩    저속 페이닝

그림 1.1 페이딩 채널의 메커니즘

전술한 바와 같이 페이딩 현상은 37] large-scale 페이딩과 small-scale 페이딩으로
분할 수 있다. Large-scale 페이딩(평균 경로 손실, 9%1800\108)과 small-scale 페이딩
를 살펴보면, 그림 1.2에 나타난 바와 같이 거리에 따라 평균 경로 손실이 발생하
수 없는 장애물 등에 가려짐으로 인하여 같은 거리에 있더라도 평균 경
로 변화하는 901800\188 현상이 발생한다. 또한, 산란 성분으로 인하여
shadowing 현상이 발생한 후의 AAS 중심으로 small-scale 페이딩이 발생한다.

【



===== PAGE 20 =====
Received                                                                          Shadowing

Signal
Power [log]

om path            Small-scale
065       1 , fading
LIN      |

Distance [log]
그림 1,2 페이딩 환경에서 large-scale 페이딩과 small-scale 페이딩의 관계

그림 132 이동 전파 응용에 있어서 link budgetS 계산하기 위해 경로 손실을 추정할
때 꼭 감안해야 하는 3 가지 요소들을 나타낸 것이다[3]. 여기서 각 RASS large-scale
페이딩으로 인한 거리의 함수로 표현한 평균 경로 BA, large-scale 페이딩 마진의 변동
(6~10dB), 901011-80816 페이딩 마진의 변동(20~30008)이다. 그림 1.3에서 *※ㅋ1~2%:로
표시된 것은 설계 목표로서 제시된 각각의 확률밀도함수의 끝 부분에 해당하는 확률을 나
타낸다. 즉, 제시된 마진의 양은 페이딩 변화로 인하여 98~99%의 수신 신호 전력을 제공
하는 값에 해당한다.

Tx                      Rx
Power      ㅣ                                              Distance
transmitted
Log-normal
0                                large-scale fading
Large-scale
fading margin
= 1~2%|]                |
Small-scale
fading margin
Power                                                {
received              ~~ 2%

그림 1.3 페이딩 채널에 대한 link budget

021


===== PAGE 21 =====
PART 1 무선 채널 모덜

OER Large-scale  페이딩

자유 공간(006 space) 전파 모델은 송신단과 수신단 사이에 장애물이 존재하지 않는
LOS(Line-of-Sight) 환경에서 수신 신호의 BES 예측하기 위하여 사용되며, 위성 통신
시스템이나 전형적인 LOS 무선 전파 환경에서 가장 널리 사용된다. 다른 대부분의 경로
손실 모델과 같이 송신단과 수신단 사이의 거리 0[00에 대한 함수로 나타낼 수 있다. 대

럽

표적인 8018 자유 공간 방정식에 의한 수신 신호의 ABS 다음과 같이 주어진다[4].
2@@.4?
tS eee ae                      (1.1)
(42) d°L

여기서 ^,와 P, (d)= 각각 송신 전력, 송신단과 수신단 사이 거리 0에서 수신 ABS 나
타낸다. 또한, @. Gy A, LE 각각 송신 안테나 이득, 수신 안테나 이득, whit, 전파
환경과 관련없는 시스템 손실 AL > YS 나타낸다. 시스템 손실 ASE 통신 시스템

: 에서 전송 라인의 감쇄, 필터 SA             sik 시스템 하드웨어의 손실

수신

계수이며, 시스템 하드웨어의 손실                                           %

L

= [2 2

= 떠
[은
a
oe
rb»
ileal
oln
{lo

BS dQ] 자승에 비례하게 감소하는 AS 확인할 수 있다.
Al (1.1)로부터 안테나 이득이 포함된 자유 공간 경로 손실 모델과 안테나 이득이 포함
되지 않은 자유 공간 경로 손실 모델을 유도할 수 있다.
fo     GGA
PL,,(d)[ dB] = 10008 을 |=  owe SS |          (1.2)
P            an
PL(d    =101   — |=-101                          3
-(d)[aB]   oe i)    개 ‘a |          (1.3)

여기서 PLp(d)= 자유 경로 손실을 나타낸다.
그림 1.4는 반송파 주파수 /, = 1.5 08일 때, 거리에 따른 자유 공간 경로 손실을
타낸다. 안테나 이득 와 이 낮아질수록 경로 AIS 커지는 AS 확인할 수 있다.

ㆍ 022



===== PAGE 22 =====
Free Path-loss Model, f = 1500MHz

110         나
—e—G=1,G,=1
100 || ~#— Ge = 1 G = 0.5
—Hi— G, = 0.5, G, = 0.5
S80 pw
3
으
= 70}
a
60 f------++---+--
50
10°        10!        402        103

Distance [m]
그림 1.4 자유 공간 경로 손실 모델

전술한 자유 공간 경로 손실 모델뿐만 아니라 대부분의 경로 손실 모델에서 송신단과
수신단 사이의 거리 0에 따라 91000100010009 평균 수신 전력이 감소한다.
Log-distance 경로 손실 모델은 전술한 자유 공간 경로 손실을 바탕으로 여러 환경에서
경로 손실 지수(0801 loss cement) n& 이용하여 일반화된 경로 손실 모델이며, 다음과
같이 주어진다.

PL,» (d)[ dB] = PL, 4) +10ne{                    (1.4)

여기서 PLzp(d)= log-distance 경로 손실을 나타내며, ds: 기준 Aezl(reference
distance)S 의미한다. 표 1.1에 나타난 바와 같이 경로 손실 지수는 여러 환경에 따라 2에
서부터 6까지의 다양한 값을 갖는다. 예를 들어, 자유 공간에서 7은 2이며, 장애물이 존재
함에 따라 n= 점점 증가한다. 전파 환경에 적합한 기준 거리의 ABS 매우 중요하다. ql
를 들어, 큰 커버리지(>1002)의 셀룰러 시스템에서는 보통 1102의 기준 거리가 사용되지
만, 1102의 셀 반경을 가지는 셀룰러 시스템이나 매우 작은 셀 반경을 가지고 있는 시스템
에서는 각각 100m, 1ㅁ의 기준 거리가 사용된다[5].

023



===== PAGE 23 =====
PART 1 _무선 채널 모델링과 MATLAB

Hii 환경에 따른 경로 손실 지수

Free Space                          2
Urban area cellular radio                2.7 to 3.5
Shadowed urban cellular radio                3 to 5
In building Line—Of-Sight                1.6 to 1,8
Obstructed in building                   4 to 6
Obstructed in factories                  2 to 3

Log-distance Free Path-loss Model, f,= 1500MHz
110

90

80

70

Path loss [dB]

Distance [m]

그림 1.5 Log—distance 경로 손실 모델

는 반송파 주파수 7. = 1.5 07 일 때, Azo 따른 108-01918006 경로 손실을
. 경로 손실 지수 no] 증가할수록 경로 손실이 커지는 것을 확인할 수
신단 사이의 거리가 동일하더라도 수신단의 위치
문어

을 반영한 모델이 log—normal shadowing 모델이며,

024


===== PAGE 24 =====
제1장_무선 채널 특성

PL(d)[aB] = PL(d)+ X,, =Pls(d,)+10nog{ © x,                 (1.5)
0
여기서 X= 02] 표준 편차를 가지고 YE Bato] 02] Gaussian 랜덤 변수이다. 식 (1.5)
는 같은 dS 가지고 있더라도 다른 경로 손실이 발생할 수 있도록 Ay shadowing 효과
가 반영된 것이다.

그림 162 f,=1.5 GHz, ㅇ= 308 , 7 = 3 인 경우의 log—normal shadowing on 경로
손실을 나타낸다. 이 그림에서 나타난 바와 같이 송신단과 수신단 사이의 거리가 동일한

라도 주위 환경에 따라 다른 경로 손실을 갖게 EO} shadowing 효과가 나타난다. =i
1.1(“do_PLgeneral”)2& 프로그램 1.2(“PL_free.m”)2} 1.3 (“PL_logdist_or norm”) 사용하여
자유 공간 경로 손실, log—distance 경로 손실, log—normal shadowing 경로 손실 모델을 도시

하며, 그 실행 결과 얻어진 그래프가 그림 1.4, 1.5, 1.6에 주어져 있다.

Log-normal Path-loss Model, [= 1500MHz, =308,0ㅁ=2

110

100

90

80

70

Path loss [dB]

Distance [m]

그림 1.6 Log-normal shadowing 경로 손실 모델



===== PAGE 25 =====
PART 1 _무선 채널 모델링과 MATLAB

% do_PLgeneral.m
fc=1.5e9; d0=100; sigma=3; distance=[1:2:31].*2;
Gt=[1 10.5], Gr=[1 0.5 0.5]; Exp=[2 3 6];
for k=1:3
y_Free(k,:)=PL_ free(fc,distance, Gt (k) ,Gr(k));
y_logdist (k,:)=PL_logdist_or_norm(fc, distance, d0,Exp(k) ) ;
y_lognorm(k, :)=PL_logdist_or_norm(fc,distance,d0,Exp(1),sigma) ;
end
figure (1)
semilogx (distance, y Free(1,:),'k-o',distance,y Free(2,:),'k-*',distan
ce,y_Free(3,:),'k-s'), grid on, axis([1 1000 40 110]),
title(['Free Path-loss Model, f_c=',num2str(fc/le6é) , 'MHz'])
xlabel('Distance [m]'),ylabel('Path loss [dB] ')
legend('G t=1, 6 r=1','G t=1, G_r=0.5','G t=0.5, G r=0.5',2)
figure (2)
semilogx(distance,y logdist(1,:),'k-o',distance,y logdist(2,:),'k-*',
distance,y logdist(3,:),'k-s'), grid on, axis([1 1000 40 110]),
title(['Log-distance Path-loss Model, f_c=',num2str(fc/le6) , 'MHz'])
xlabel('Distance [m]'), ylabel('Path loss [dB]')
legend('n=2', 'n=3', 'n=6',2)
figure (3)
semilogx (distance, y_lognorm(1,:),'k-o',distance,y lognorm(2,:),'k-*',
distance, y lognorm(3,:),'k-s')
grid on, axis([1 1000 40 110]), legend('path 1','path 2','path 3',2)
title(['Log-normal Path-loss Model, f c=',num2str(fc/le6é) , 'MHz,
', '\sigma=', num2str(sigma), 'dB, n=2'])
xlabel('Distance [m]'),ylabel('Path loss [dB]')

Bl 프로그램 11 일반적인 경로 손실 모델 실행 프로그램

function PL=PL free(fc,d,Gt,Gr)

% Free Space Path Loss Model

% Inputs:

%      fe    : Carrier frequency [Hz]

%      d     : distance between base station and mobile station [m]
%      Gt    : transmitter gain

026


===== PAGE 26 =====
Gr    : receiver gain

Output:

PL    : path loss [dB]
lamda = 3e8/fc; tmp = lamda./(4*pi*d) ;
if nargin>2, tmp = tmp*sqrt (Gt); end

00 oP ol

if nargin>3, tmp = tmp*sqrt (Gr); end
PL = -20*log10(tmp); ¢ “4 (1.2)/(1.3)

Tal 프로그램 12 자유 공간 경로 손실 모델 함수

function PL=PL_ logdist_or_norm(fc,d,d0,n,sigma)

6 Log-distance or Log-normal Shadowing Path Loss Model
%      do    : reference distance [m]

%      n     : path loss exponent

%      sigma : variance [dB]

lamda = 3e8/fc;
PL = -20*log10(lamda/(4*pi*d0)) + 10*n*logl0(d/d0); % “4 (1.4)
if nargin>4, PL = PL + sigma*randn(size(d)); end   * # (1.5)

\

때
ms

ial 프로그램 1.3 Log-distance 또는 log-normal shadowing 경로 손실 모델

RR OOkumura/Hata 모델

Okumura 이동 통신 시스템 환경에서 안테나의 높이와 커버리지 SAS 계산하기 위
하여 경로 손실에 관한 광범위한 ASS 하였다[6]. Okumura BAYS 도심 환경에서 신호
ASS 위하여 가장 널리 이용되는 모델 중에 하나이다. 이 BAS 500MHz>4A}
1500MHz7}2] 대역, 1027에서 10002의 셀 반경, 302에서 1000m2] 기지국 안테나 높이
에 주로 이용될 수 있다. 01040008의 자유 공간 경로 손실 모델 PL, (d)& 다음과 같이

주어진다.

PL yy (d)[dB] = PL, + Aye (1,4) — Gp, — Gr, + Gages

그

여기서 47200, 0)는 매체 감쇄 변수이고, Ge, Gr, = 각각 수신 안테나와 송

나의 이득, Canes 전과 환경에 따른 이득을 나타낸다. 안터
| 안테나의 높이에 관한 이득으로 안테나 패턴과 같은 요소


===== PAGE 27 =====
PART 1 _무선 채널 모델링과 MATLAB

Ayv(f, 0), Gara Okumura7} 실측하여 얻은 그림으로부터 구할 수 있다[6].

Okumura 모델은 현재 가장 널리 사용되는 경로 손실 모델인 Hata 모델의 바탕이 되었
다[7]. Hata= Okumura®] 경험적인 경로 손실 모델을 바탕으로 EAlurban), 교외
(suburban), 개방(0060 area) 환경에 대하여 모델링하였다. 도심 환경의 경로 손실 모델
PL ata, d= 다음과 같이 주어진다.

2 (d)[AB] = 69.55 + 26.16 log f, —13.82log hp, Cy, + (44.9-6.55logh,, Jlogd (1.7)

여기서 반송파 주파수 /,의 단위는 MHzo]a1, 송신단과 수신단 사이의 거리 0와 송신 안
테나의 높이 hy, 의 단위는 각각 km, mole. Cac 수신 안테나의 상관 계수이며, 서비
스 커버리지의 범위에 따라서 2가지로 나뉘어질 수 있다. 작거나 중간 범위의 커버리지를
위한 는 다음과 같이 주어진다.

Cp, =0.8+(1.1log f, -0.7)/ -1.56log 7:                        (1.8)

여기서 는 수신 안테나의 높이이고, 단위는 이다. 또한, 큰 범위의 커버리지를 위한
Capt 반송파 주파수에 따라 2가지로 정의되며 다음과 같이 주어진다.

8.29(log(1.54/p,)) —1.1 if 1S0MHz< f, <200MHz

”                                                                                  (1.9)
3.2(log(11.75h»,)) —4.97 if 200MHz< f, <1500MHz

@ PL yata,sv(d) 4 개방    환경의 경로 손실 모델 2/.6.,,0(0)은

2
PL paras (€LAB] = PL pry, (4) ~ | toe 4   =                             (1.10)
PL jaya 9 (A)[AB] = PL py, (A) — 4.78 (log f.) +18.33log f, — 40.97           (1.11)
프로그램 1.4(“00 PLHata”)= 프로그램 1.5(“PL Hata”) 사용하여 Al(urban, 4]

(1.7)), 교외(646040080, 4] (1.10)), 개방 환경(0060 area, 식 (1.11))의 경로 손실 모델을 도

028


===== PAGE 28 =====
심의 경우가 다른 경우보다 경로 손실이 가장 큰 것을 확인할 수 있다.

110

Hata Path-loss Model, f, = 1500MHz

100 더

—i— urban
—e®— suburban | |}:
—Aé— open area | |}:

H
1
1
1

he

'
4
t
1
‘
oer
a
‘

4
1
|
1
‘

0             1      ) | 1

6 Waimea 주 주
'    1 1
‘
1
1

90 |

Path loss [dB]

60 }------4

80 poe

70 }-------:

차

e      :        MATLAB 프로그램 : Hat

Distance [m]
그림 1.7 Hata 경로 손실 모델

* do PLHata.m

fc=1.5*10°9; htx=30; hrx=2;

distance=[1:2:31] .*2;

y_urban=PL Hata(fc,distance,htx,hrx,'urban') ;
y_suburban=PL Hata(fc,distance,htx,hrx,!suburban') ;
y_open=PL Hata (fc,distance,htx,hrx,'open') ;

semilogx(distance,y_urban,'k-s',distance,y _suburban,'k-o',

distance, y_ open, 'k-*')

grid on, axis([1 1000 40 110]),

title(['Hata PL model, f c=',num2str(fc/1le6) , 'MHz'])
xlabel('Distance [m]'),ylabel('Path loss [dB] ')
legend ('urban','suburban','open area! , 2)

i 프로그램 14 Hata 경로 손실 모델 실행 프로그램

029



===== PAGE 29 =====
PART 1 _무선 채널 모델링과 MATLAB

function PL=PL Hata (fc,d,htx, hrx,Etype)

Etype : environment type('urban', 'suburban', 'open')

% Hata Model

6 Inputs:

%      fc    : carrier frequency [Hz]

6      d     : distance between base station and mobile station [m]
%      htx   : height of transmitter [m]

%      hrx   : height of receiver [m]

% Output:

%      PL    : path loss [dB]

if nargin<5, Etype = 'URBAN'; end

fc=fc/(1e6) ;

if fce>=150&&£c<=200, C_Rx = 8.29*(log10(1.54*hrx))*2 - 1.1;
elseif fc>200, C_Rx = 3.2* (1log10(11.75*hrx))*2 - 4.97;   e 2 (1,9)
else C_Rx = 0.8+(1.1*1l0g10 (fc) -0.7) *hrx-1.56*logl0(fc); % “4 (1.8)
end
PL = 69.55 +26.16*log10(fc) -13.82*1lo0g10 (htx) =G RK ass
+(44.9-6.55*10g10 (htx) ) *log10 (4/1000) ;       * 4 (1.7)
EType = upper (Etype) ;
if EType(1)=='S', PL = PL -2* (log10 (£c/28) )*2 -5.4; % 4 (1.10)
elseif EType(1)=='0'
PL=PL+ (18 .33-4.78*1l0g10 (fc) ) *logl0 (fc) -40.97;     % 4 (1.41)
end

떼

Tel 프로그램 1.5 Hata We 손실 모델

IEEE 802.160 모델

IEEE 802.16d 모델은 log—normal shadowing 경로 손실 DAS 기반으로 하며, 표 1.2
에 나타난 바와 같이 교외 환경에서 송신단과 수신단 사이에 장애물의 밀도(나무의 밀도
로 표시됨)에 따라 Type A, 8, 로 구분된다. 표 1.2에서 ART(Above Roof Top) 지붕
위를 나타내고 BRT(Below Roof 100)는 지붕 아래를 나타낸다. IEEE 802.160 모델은 다
음과 같이 주어진다[8][9][101.

Pl gq 16(4)[ dB] = PL; (dy )+102408,, (=) +Cyr+Cy, — for d>dy           (1.12)
0

030


===== PAGE 30 =====
여기서 dy = 100m, 7 = ㅇ- bhp, +c/hp, S 나타낸다. 또한 a, 0, <의 값은 표 1.3에 주
어져 있다. 송신단 안테나 높이 Ap, = 100에서 80m 사이로 주어진다. 또한, C2} Cy, E
각각 반송파 주파수와 수신 안테나의 상관 계수를 나타낸다. 는 다음과 같이 주어진다.

Cy = 6logio(f, / 2000)                                (1.13)
여기서, 반송파 주파수 /,의 단위는 \0이다. 수신 안테나의 상관 계수 Cy, t= 다음과
같이 두 가지로 주어진다.
_ |-10.8logio(Ag,/2) for Type AandB                 7
| -20logio(Ap, /2) for TypeC                      (1.14)
—10logi) (Ap, /3) for hp, <3m
er =                                                                 (1.15)
—20logio (hp, /3) for hp, >3m

[표 1.2) IEEE 802.160 경로 손실 모델의 형태

“Type Description
Macro-cell suburban, ART to BRT for hilly terrain with moderate—to—
heavy tree densities

oe Macro-cell suburban, ART to BRT for intermediate path—loss condition
ae Macro~cell suburban, ART to BRT for flat terrain with light tree densities

[표 1.3] Type A, B, COl] 따른 파라미터
a                4.6                4                3.6
0,0075         0,0065          0.005
c             12.6            17,1            20

031



===== PAGE 31 =====
PART |_ 3M 채널 모델링과 MATLAB

그림 1.8은 IEEE 802.160 모델에서 반송파 주파수가 20412이고, 송신 안테나의 높이가
300일 때, 수신 안테나의 높이를 변경함에 따른 경로 손실을 나타낸다. 이 그림은 IEEE
802.160 모델의 문제점을 0" 것으로 수신 안테나의 높이가 20에서 10교로 높아짐
에 따라 송신단 안테나와 수신단 안테나의 거리가 1002인 지점에서 불연속점이 발생한
다. 예를 들어, shadowing maiz} 고려되지 않았음에도 불구하고 101m 지점의 경로 손실
보다 99m2] 경로 손실이 약 808정도 큰 것을 알 수 있다. 이러한 BAAS 해결하기 위
하여 새로운 기준 거리((6[666006 distance) 0;가 필요하게 되어 기존의 IEEE 802.160 모
델을 수정한 Modified IEEE 802.16d 모델이 제안되었다[9]. 새로운 기준 거리를 dz A
의하고, 이 값을 구하기 위하여 자유 공간 경로 손실 모델 식 (1.3)을 A (1.12)에 대입하
면 다음과 같이 주어진다.

20108, 뿌 |- 20108, |

[1049 +6, +c      (1.16)
0

따라서, 새로운 기준 거리 @,'은 다음과 같이 정리된다.

|                    (1.17)

d, =d)10 (  =

Al (1.17)& 4} (1.12)에 대입하여 정리하면 다음과 같이 Modified IEEE 802.16d 모델
이 주어진다.

201089 (“22                         for d<d)

PLygo2.16(4 |B] =                                                                                                   (1.18)

20 log), (4 0020 와 Cy+Cp for d> dy
0

프로그램 1.6(“do PLIEEE80216d”)& 프로그램 1.7(“PL_IEEE80216d”)2- 사용하여
IEEE 802.16d 경로 손실 모델(식 (1.12))과 수정된 IEEE 802.160 경로 손실 모델(식
(1.18))을 도시하며, 그 실행 결과 얻어진 그림 1.9를 그림 1.8과 비교하면 \1001060 IEEE
802.160 경로 손실 모델에서는 불연속점이 없어진 것을 확인할 수 있다.

032



===== PAGE 32 =====
IEEE 802.16d Path-loss Model, f. = 2000MHz

1
알스 eesses

Leemra rs

[90] 599이4688

10

10'

10

Distance [m]

[그림 1.8] IEEE 802.160 모델에서

Modifed IEEE 802.16d Path-loss Model, [ = 2000MHz

30m, hp,= 2m

Di

140

[90] sso] Wed

Distance [m]

[그림 1.9] Modified IEEE 802,16d

ee
경로 손실 모델

oe



===== PAGE 33 =====
PART 1 무선 채널 모델링과 MATLAB

% 00 PLIEEE802.16d.m

elf, lc, @lear 311

fc=2*10°9; htx=[30 30]; hrx=[2 10]; distance=[1:1:1000];

y_IEEE16d=zeros (2, length(distance) ) ;

y_MIEEE16d=zeros (2, length (distance) ) ;

for k=1:2
y_IEEE16d(k,:)=PL_IEEE80216d(fc,distance, 'A',htx(k),hrx(k),'atnt');
y_MIEEE16d(k,:)=PL_IEEE80216d(fc,distance, 'A',htx(k),hrx(k),'atnt',
'mod');

end

figure (1)

semilogx (distance, y IEEE16d(1,:),'k:','linewidth',1.5),hold on

semilogx (distance, y IEEE16d(2,:),'k-','linewidth',1.5)

grid on, axis([1 1000 10 150])

title(['IEEE 802.16d Path-loss Model, f£ c=',num2str(fc/1le6) , 'MHz'])

xlabel('Distance (m)'),ylabel('Pathloss (dB) ')

legend('h_{Tx}=30m, h_{Rx}=2m','h_{Tx}=30m, h_{Rx}=10m',2)

figure (2)

semilogx (distance, y MIEEE16d (

semilogx (distance, y MIEEE16d (

grid on, axis([1 1000 10 150])

title(['Modified IEEE 802.16d Path-loss Model,

£ c=',num2str(fc/le6) , 'MHz'))

xlabel('Distance (m)'),ylabel('Pathloss (dB) ')

legend('h_{Tx}=30m, h_{Rx}=2m','h_{Tx}=30m, h_{Rx}=10m',2)

1,:),'k:','linewidth',1.5),hold on
2,:);,'k=',"linewidth', 1.5)

Tg) 프로그램 16 IEEE 802.160 경로 모델 실행 프로그램

function PL=PL_IEEE80216d(fc,d,type, htx,hrx,corr_fact,mod)
IEEE 802.16d model

% Inputs
* fe       : carrier frequency
6 0        : distance between base and terminal
% type      ; selects ‘A’, "B', or *C!
htx       : height of transmitter
hrx       : height of receiver

corr fact: if shadowing exists,
set to 'ATnT' or 'Okumura'. Otherwise, 'NO'

00 oP ol?

응 mod      : set to 'mod' to obtain modified IEEE 802.16d model
6 Output - PL : path loss [dB]
Mod='UNMOD' ;

034



===== PAGE 34 =====
if nargin>6, Mod=upper(mod); end
if nargin==6&&corr fact (1)=='m', Mod='MOD'; corr_fact='NO';
elseif nargin<6, corr fact='NO';
if nargin==5&&hrx(1)=='m', Mod='MOD'; hrx=2;
elseif nargin<5, hrx=2;
if nargin==4&&htx(1)=='m', Mod='MOD'; htx=30;
elseif nargin<4, htx=30;
if nargin==3&&type(1)=='m', Mod='MOD'; type='A';
elseif nargin<3, type='A';
end
end
end
end
30 = 100;
Type = upper(type) ;
if Type~='A'&& Type~='B' &&Type~='C'
disp('Error: The selected type is not supported'); return;
end
switch upper (corr fact)
case 'ATNT',    PL£=6*10g10 (£c/2e9) ;              eS (1,23)
PLh=-10.8*1lo0g10 (hrx/2) ;           % Al
case 'OKUMURA', PL£=6*1log10 (fc/2e9) ;            %
if hrx<=3, PLh=-10*logl10 (hrx/3); % “ (1.15)
else, PLh=-20*1log10 (hrx/3) ;

end
case 'NO',      PL£=0; PLh=0;
end
if Type=='A', a=4.6; b=0.0075; c=12.6;      % A (1.3)

elseif Type=='B', a=4; b=0.0065; c=17.1;
else    a=3.6; b=0.005; c=20;
end
lamda=3e8/fc; gamma=a-b*htx+c/htx; 00 _pr=d0; % 4 (1.12)
if Mod(1)=='M', dO_pr=d0*10*- ((PL£+PLh) /(10*gamma)); end % “ (1.17)
A = 20*1log10(4*pi*d0 pr/lamda) + PLf + PLh;
for k=1:length(d)
if d(k)>d0_pr, PL(k) = A + 10*gamma*log10(d(k) /d0) ;    = + (1.18)
else, PL(k) = 20*1log10(4*pi*d(k) /lamda) ;
end
end

\

ia) De 724 1.7 IEEE 802.160 경로 손실 모델 함수

이 2} large-scale 페이딩 모델로 WINNER 모델 등이 있다[11].



===== PAGE 35 =====
PART 1 _무선 채널 모델링과 MATLAB

1.2 Stor I-scale 페이딩

Small-scale 페이덩은 간단히 페이딩이라고 불리기도 하며, 짧은 시간이나 짧은 거리의
무선 채널을 통하여 수신된 신호 크기의 변동을 나타낸다. 두 개 이상의 파가 약간의 시간
차를 두고 수신 안테나에 도착하면 서로 간섭으로 작용하여 위상이 같으면 신호의 크기를
중가시키고 위상이 서로 반대이면 크기를 감소시키는데, 이러한 다중경로에 의한 영향을
페이딩이라고 정의한다. 서로 다른 경로를 통하여 수신되었기 때문에 다중경로 파
(multi-path \886)라고 불리는 이 ASE 수신 안테나에서 서로 결합되어 크기나 위상을
크게 변화시킨다.

Small-scale 페이딩을 발생시키는 요인은 크게 4가지로 분류될 수 있다.

: 다중경로 전파(00414-ㅁ811 propagation)

널 상의 반사체나 산란체에 의해 다중경로가 발생하게 되고, 다중경로를 통과한 성

들의 랜덤 위상과 크기가 더해져서 신호 강도의 변화를 야기한다.

신기의 속도(0706116 speed)

신기와 수신기의 움직임은 각 다중경로 성분에 따라 다른 도플러 천이를 일으켜 a
덤 주파수 변조가 발생하게 된다. 여기서 도플러 천이는 수신기가 송신기에 접근하는
지 아니면 멀어지는지에 따라 양의 값이나 So] 값을 갖는다.

° 주위 물체의 속도(60660 of surrounding objects)
무선 채널 상에 존재하는 물체가 움직인다면 다중경로 성분들이 도플러 천이를 겪게

a   H

된다. 만약 주위 물체가 수신기보다 빠르게 이동한다면 60811-80886 페이딩을 발생하

는 요인이 된다.

° 신호의 전송 대역폭(『81061001661011 bandwidth of signal)
송신 신호와 채널의 대역폭에 따라 페이딩 현상이 달라진다. 즉, 송신 Also] 대역폭
이 채널의 대역폭보다 작은 경우 주파수 비선택적 페이딩을 겪고, 송신 신호의 대역
폭이 채널의 대역폭보다 큰 경우 주파수 선택적 페이딩을 겪게 된다.

수신기가 이동할 경우 수신된 신호가 겪는 페이딩의 유형은 전송된 신호 및 채널의 특
성에 의존한다. 대역폭, 심볼 주기 등의 신호 파라미터와 mms 지연 확산과 도플러 확산 등
의 채널 파라미터에 따라 다른 유형의 페이딩을 겪게 된다. 무선 채널에서 시간 확산(4006
dispersion)#} 주파수 확산(6604600% dispersion)o]] 따라 다른 유형의 페이딩 채널을 유발

036


===== PAGE 36 =====
중경로 존재 시 지연 확산에 의해 전송 ASL 주파수 비선택적 페이딩 또는 주파수
딩 현상을 겪게 된다. 그림 1.10은 주파수영역에서 채널의 주파수 Veo] 고정

J 특성이 달라지는 현상을 보여준

정우 Ape. 주파수에 따라 다른 크기

|아서 채널 응답의 평탄한 부분에
페이딩을 겪게 a2 송신 신후

고 별
aa

딩을 4A
그림 1.10(8)에서와 같이 무선 채널이 전송 신                       '

며 통과대역 내에서 일정한 이득과 선형 위상 SHS 갖는다면 수신 ASE 주파수 비선

택적 페이덩을 겪게 된다. 여기서 채널의 대

의 지연 확산보다 크다는 AS 의미한다. 송신 신호의 심볼주기 To} 다중경로 채널

h(t ,7)의 지연 확산보다 크면 채널의 지연 확산이 발생하더라도 다음 심볼에 간섭을 주
지 않는다. 즉, 샘플링 주기가 채널의 지연 확산보다 크기 때문에 다음 샘플링 시점에서
aol 다음 Adel IVS 주지 않는다. 주파수 비선택적 페이딩 Ae 채널의 3771
시간에 따라 천천히 변화할 수 있으나, 전송 신호의 대역폭이 채널의 주파수 비선택적 대

역폭에 비하여 매우 작기 때문에 협대역080ㅁ0\6800) 채널로 불리기도 빈다

a(t)      h(t, 7)     y(t)         a(t)      bo    y(t)
7 < Ts          > Ts
a(t)      h(t, 7)      y(t)        z(t)      h(t, 7)      y(t)
0 £     Or    Q err   0125    0   T  026  4690.
X(f)       te       Y(f)        X(f)       H(f)      Y(f)
(a) 주파수 비선택적 페이딩 채널의 예         (b) 주파수 선택적 sols 채널의 예
그림 1.10 다중경로 존재 시 시간 지연 확산에 의한 페이딩 채널 특성

037

00000


===== PAGE 37 =====
PART 1 무선 채널 모델링과 MATLAB

지금까지의 내용을 요약하면, 전송 신호는 다음과 같은 조건하에서 주파수 비선택적 페

이딩을 겪게 된다.
(1.19)

여기서 BsSt To 각각
coherence 대역폭과 rms 4]
전술한 바와 같이 송신 신
일정한 크기의 이득과 선형                면
a 된다. 이러한 경우에 채널의 임펄스 a -
지연 확산을 갖게 된다. 주파수 A     페이덩이

의 대역폭과 심볼 주기를 의미하며, BL} ㅇ,는 채널의

[쏘
oby
(pas
x fe

tof
12 sot

rf

대역폭보다 작은 대역폭 내에서 채널의 주파수 응답이
응답을        신 신호는 주파수 선택적 페이딩을
#8  주기보다 긴 다중경
로에 의해 2771

20
ox

od -

(path
1
Ls

a.m

oe  고, 지연된 다수의 송신 신호가
수 선택적 페이덩은 GEARS) 시간 확산에 의해 발생되며 인접 심볼간 간섭0때%-
Symbol Interference; ISI) 유발한다. 또한, 채널이 주파수영역에서 평탄하지 않고 특정
주파수에서의 크기가 다른 주파수에서의 크기보다 크거나 작기 때문에, '주파수 선택적
(frequency selective) 채널'이란 용어를 사용한다.

그럼 1.10(06)는 주파수 선택적 페이딩 채널의 SYS 보여준다. 이 그림에서 채널의 지
a 확산 가 종신 heals 심볼 주기보다 크기 때문에, 시간영역에서 인접 ASA 간섭이
발생한다. 그리고 주파수영역에서 송신 신호의 스펙트럼 9(/)가 A coherence 대역
% Both 크고 대역 Yoh 주과수에 마라 다른 크기를 가지기 때문에 주과수 선택적
채널이 된다. 주파수 선택적 페이딩 채널은 신호 5(7)의 대역폭이 채널 임펄스 응답의 대
역폭보다 넓기 때문에 광대역041060800) 채널이라고 불리기도 한다.

요약하면, AS ASE 다음과 같은 경우에 주파수 선택적 페이딩을 겪게 된다.

Bo > Be

1.20
1, >,                              (1.20)

변조 방식에 따라 다르기는 하지만, 일반적으로 0, > 0.17,0)8 채널은 주파수 선택적
이라 할 수 있다.

mio
4>

 0386



===== PAGE 38 =====
1.4 PDP2| 표현 예 (ITU-R Pedestrian A 모델)[29]

il                              0                                  0.0

8                             110                                Sl
3                            190                               19,2
4                            410                               -22.8

다중경로 채널의 특성은 종종 PDP(Power Delay Profile)= 사용하여 표현된다. 표 1.4
에 나타난 바와 같이 PDP 기준 시간으로부터 초과 지연 시간에 다중경로 채널을 통하
여 수신된 신호의 평균 전력 분포를 기준 시간의 전력에 대하여 상대 전력으로 나타낸 것
을 의미한다.

여러 다중경로 무선 채널을 비교하고 무선 전송 시스템 설계의 일반적인 가이드 라인의
제시를 위하여 평균 초과 지연(02680 excess delay), rms 지연 확산(0095 delay 901680)과
같은 파라미터 등이 사용된다. 평균 초과 지연 TS PpPS| 1차 모멘트로 다음과 같이 주
어진다.

> at,   > P(e, A
T= k     = k
Ya > 260)

(1.21)

여기서 Tt ＊번째 지연되어 수신된 채널의 지연시간이고, a 와 P(t,) += 각각 <, 에서
의 채널 크기와 전력을 의미한다.
또한 ms 지연 확산 ^, 은 PDP] 2차 중심 모멘트의 제곱근으로 다음과 같이 주어진다.

o, =? -(F)                                         (1.22)
여기서
_ pan DVPee
k   k

= 수 = SAG)               (1.23)

k

|
N

039


===== PAGE 39 =====
PART 1 _무선 채널 모델링과 MATLAB

일반적으로 6004606006 대역폭과 rms 지연 확산은 다음과 같은 BAS 가지고 있다.

Bux                                              (1.24)

I
oO,

상관 값이 0.9 이상인 주파수 dA4Z= coherence 대역폭으로 정의할 경우, coherence
대역폭은 다음과 같이 주어진다.

00                                         (1.25)

상관 값이 0.5 이상인 주파수 대역폭을 000600006 대역폭으로 정의할 경우, coherence
대역폭은 다음과 같이 주어진다.

(1.26)

GRRE 도플러 확산에 의한 페이딩 영향
도플러 확산(00001 spread)o 의해 수신 신호는 고속 페이딩 혹은 저속 페이딩을 a
게된다. 고속 페이딩 채널에서 채널의 임펄스 응답은 심볼 주기 내에서 빠르게 변하기 때
문에 채널의 coherence 시간이 전송 신호의 심볼 주기보다 작다. 이는 도플러 확산에 의하
여 주파수영역에서 확산을 유발하며, 결과적으로 신호의 왜곡을 발생시킨다. 다음과 같은

조건을 만족할 경우 신호는 고속 페이딩을 겪게 된다.

Ts > Te                                           (1.27)
222,
여기서 7,,와 Bp%= 22} coherence 시간과 도플러 확산을 의미한다.
저속 페이딩 채널에서 채널의 임펄스 응답은 기저대역 송신 신호의 변화율보다 매우 느
린 속도로 변한다. 이러한 Bo] AUS 한 심볼 이상의 심볼 주기동안 고정된 채널
(static channel)@ 가정할 수 있다. 이는 주파수영역에서 채널의 도플러 확산이 기저대역

040

58



===== PAGE 40 =====
Shy 아

Wesel
(1.28)
B, >> By
일반적인 000606006 시간과 도플러 확산과의 관계를 살펴보면 다음과 같다
1
=>                                      (1.29)

여기서 /,,는 최대 도플러 천이 주파수이고, By = 2f,, Ch. 상관 값이 0.5 이상인 시간

414-= coherence 시간으로 정의할 경우, coherence 시간은 다음과 같이 주어진다.

9

1627,                                                 (1.30)

T. =
4} (1.29)% Rayleigh 페이딩을 겪는 신호가 매우 천천히 변한다는 가정하에 유도되었
= 식 (1.302 매우 빨리 변한다는 가정하에 유도되었다. 최근 무선 통신에서 가장 널

쓰이는 6004606006 시간은 식 (1.29)와 식 (1.30)의 geometric 100681으로 다음과 같이 주
진다.

a 도

T=
1627,    대

여기서 유의할 것은
에는 관련이 없다는
이 무선 채널이 주파수 선택적인지 주파수 비선택적인지에 대한 어떠한 정보도 제공하지
않는다. 고속 페이딩은 단지 수신단의 움직임에 의하여 발생하는 채널의 변화율에만 의존
하기 때문이다.



===== PAGE 41 =====
PART 1 _무선 채널 모델링과 MATLAB

GW serve 통계적 특성

Clarke 모델은 이동국에 수신된 신호의 Az}4h(Electromagnetic 8010)의 통계적 특성
신호의 산란(60846008)으로부터 형성된다는 것에 착안하여 페이딩 채널을 위한 통계

ZOU

평

bt

BAS 제안하였다[12]. Clarke7} 제안한 BAS 이동국 안테나에 입사된 전자장은 임의
의 반송파 위상, 임의의 도달각을 가진 제개의 평면파(01006 \816)로 구성되며, 각 평면
는 동일한 평균 크기를 갖는다고 가정하였다[12][113][14][15].

EL

x-y plane
^
Vv
T2111 방향으로 vQ| 속도로 이동하는 수신단에 입사되는 평면파
그림 1.11은 2방향으로 ?의 속도로 이동하는 수신단에 입사되는 평면파를 보여준다.

여기서 AoA(Angle—of—Arrival) 0는 ㅎ-4평면에 에 이 각도이다. 수신기가 이동
하기 때문에 이동국에 입사되는 모든 평면파는 도플러 천이되어 동시에 수신기에 도달
한다.

무선 전송 시스템에서 송신단에서 전송한 통과대역(68590800) 신호 x)= 다음과 같
이 주어진다.

H(t) = Re[ 00677 |                                           (1.32)

여기서 a(t) 송신단에서 전송한 71AG baseband) 신호이고, Re [(ㆍ)|는 (ㆍ)의
실수 성분을 의미한다.
식 (1.32)의 통과대역 신호가 무선 WAS 통과하고 도플러 천이를 겪은 후 수신단에 도

착하게 되면 통과대역의 수신 신호 70

042



===== PAGE 42 =====
(1.33)

| = Re [ y(t)e?*" |

7

i=]

o fc 각각

여기서 7는 산란 성분(608460)에 의해 발생하는 최대 전파 경로의 AC, 7
8 번째 전파 경로의 이득, 지연 시간, 도플러 천이를 의미한다. 도플러 천이 /,는 다음과
같이 주어진다.

(1.34)

/, =f, 0086 = 70088

여기서 /,,은 최대 도플러 천이 주파수, 0,는 번째 평면파의 AoAS 나타낸다. 또한 기저

대역 수신 신호 yt) = 다음과 같이 주어진다.

y(t) = 2, Ce "xt —1,)                                                (1.35)
여기서 OM =2a{(f£+4)4-f} 이다.
따라서, ABS 복소 저역통과 임펄스 응답을 가진 선형 A 필터에 의해 다음과 같이
모델링된다.
A= x Ce 6(t-T,)                                              (1.36)
34 주기 Ts

여기서 6(ㆍ)는 Dirac 델타 함수이다. 전파 경로의 지연 차이가 신호의 샘플
보다 매우 작은 경우에는 전파 경로 지연 를 로 간략화할 수 있으며, 이 경우 Al (1.36)

은 다음과 같이 주어진다.

A(t,t) = 3 Ce S(t — 4) = h(t)d(t -2)

i=l

3(07)=1 이라고 가정하면, 식 (1.33)의 통과대역 수신 신호 ID 는 다음과 같이 표현된다.

043



===== PAGE 43 =====
PART 1_ 무선 채널 모델링과 MATLAB

5) =h, (t)cos 2a ft hp(t)sin 2a ft                           (1.38)

여기서 h(t) 2} Mgt) = 각각 H(t) 의 inphase, quadrature 성분이며 다음과 같이 주어진다.
h,(t)= pe, cos @(t)                                               (1.39)
ity = De, sin g(t)                                               (1.40)

여기서 7가 매우 크다면, 중심 극한 Ael(central limit 0160700)에 의해 2, (¢) 2} A(t) =
Gaussian 랜덤 변수로 근사화될 수 있으며, y(t) 7} WSS(Wide-Sense 851100081*)하다는

가정 하에 70) 의 자기 상관(040-00088000은 다음과 같이 주어진다.

Vix (7) = E[WOFC+7)]
= E[h,(t)h,(t+7)|cos 22 fr - E| hg (t)h, G+ 2) |sin 227.7               (1.41)

=), (T)cos2aft—-y, ty 7) sin 227 >

각 경로의 지연과 도플러 천이는 서로 독립적이기 때문에 각 다중경로 채널의 위상은 독
립적이 되고, £7, ㅎ이기 때문에 《(/) 는 (-ㅠ, 7) 구간에서 균일 분포(40000 density)
가 된다. 이러한 SAS 이용하여 Mn, 와 Min, OE 다음과 같이 나타낼 수 있다.

62
Vin, T)= Eno [h, (t)h, (t+ 7)|=— E, [cos 2a fr]
2.    i
(1.42)
=o 기 [ cos (2 f,,rcos@) |
2

Vnny (0)= Exo| hy (ho (t +7) |= 늘고 |9ㅁ0(227,20050)|                       (1.43)

ho

여기서, 0, 2, 다음과 같이 주어진다.

044


===== PAGE 44 =====
제1장_무선 채널 특성

=
6=[6,4,,---,6, |

                                           (1.44)
Q, =E[ a ]+£[ We @) |= LC

Clarke] 2—D isotropic 산란 모델로부터 0에 따른 안테나 이득 ㅇ(0)=1이고 92] 확
률 분포 2(0)=1/2* 일 때, 식 (1.42)와 A} (1.43)은 각각 다음과 같이 유도된다[121.

Yn, (= 3 | 006(0227.70060)2(0)0(0)00

(1.45)
(9)                    Q
=구그 ,005(227,70050)00 = Jo(27f,7)
==    in(2       0)de=0                 1.46
Tat => 1 sin( 1 f,,7 cos 0)d0 =            (1.46)

여기서 4(ㆍ)는 Al 1S 0차 Bessel 함수이다. 위 결과를 이용하여 Al (1.41)은 다음과 같

Vip (T)= Vn, (00005227.2- > 4, Sin 2m fT

Q                                                          (1.47)
= 3 (27 f,,7)cos2a ft

또한 h(t) 9} %0)의 전력 ABE Power Spectrum Density)2 7%,.,(0) 또는
Yio.) 의 Fourier 변환으로서 다음과 같이 주어진다.

Q
; 2     1   !   Ils
Sin, P= Sign, A= F [ Yun «| =) 227, ~) (f/f)                         (1.48)

0                  otherwise

여기서 F[(+ l= (+ ) 2] Fourier 변환을 의미한다. 또한 h(t) 2} 자기 상관과 전력 스펙

트럼은 각각 다음과 같이 정의된다.

045



===== PAGE 45 =====
PART 1 _무선 채널 모델링과 MATLAB

My 0=극시씨0000+20]

(1.49)
=, 00+ 722 (2)
8,,(7)= Sim; (f)+ ISinty (7)                                         (1.50)
A} (1.50)에 주어진 %,,(/) 을 도플러 전력 스펙트럼이라고 정의한다.
)7(2)= Re| 70600" |                                 (1.51)
Re[a]=2"4                      (1.52)
Yan (2) = Yin (2)                                      (1.53)

(1.51)부터 4] (1.53)의 식과 7,,,(=091 성질을 이용하여 통과대역 도플러 전력
스픽트림을 다음 식과 같이 Yeh 수 있다

P

= |f-flsh,

427,       _
Ss(A)=S[Su(S—L)+ 5 (“1 +L)      (4)                (1.54)

0                         otherwise

가 매우 크다면 수신 전력의 변화량을 404에 대한 함수로서 다음과 같이 나타낼 수

S;(f)|df|= “2{4(0) (0) + G(-0) p(-0)}|d6|                        (1.55)

여기서 f=, cosd+ folum |9|는 다음과 같이 주어진다.

11=/,|-9ㅁ000 =) f2 -(7 -— 6.) 100                    (1.56)

046


===== PAGE 46 =====
따라서, 통과대역 도플러 전력 스펙트럼은 404에 대한 함수로서 다음과 같이 나타낼 수
있다.

$0)=-- 2 {0(“02(0)0+0(-07(아
P-(f-f)

(1.57)

한편, Rician 채널 PALS LOS 성분(또는 906041@ 성분)과 NLOS AHX(scattering 성

분)으로 구성되며, AAS] 확률 분포 7(9]는 다음과 같이 주어진다.

= KPO EG AO-4)

(1.58)

여기서 p(@) 2+ @ 는 각각 산란(60806008) 성분의 AoA 확률 HX} specular 성분의
AoAS 나타낸다. K = specular 성분의 전력 c? a} 산란 성분의 전력 20^의 비로 다음고

같이 정의된다.

K=
20°
위 ASS 이용하여 Rician 채널의 자기상관 함수들과 도플러 전력 스펙트럼은
같이 주어진다
1 Q           ※ 요
Voi (1) =p 0 (2A Int) + E008 (28 fn C088)

Q
Viyhy F) = Hsin (2a f,re0s 0)

5,,(/)=             ea (f)+             SZ Saf )
1 Q            1             K

14

0                                                 otherwise

SOF ~ fn 08%) |F|S In

ㅁㄴ

(1.59)

다음과

(1.60)

(1.61)

(1.62)

047



===== PAGE 47 =====
정확한 채널 모델을 생성하기 위해서는 특정 시간에 주어진 환경에서 BA} (reflector)
의 위치, 반사체로부터 수신되는 신호의 전력, 반사체의 이동성 등 모든 반사체(066016000ㅁ0
들의 속성을 알고 있어야 한다. 그러나, 이러한 모든 정보를 수집하는 것은 실제적으로 불
가능하기 때문에 「전형적(5721081)`이거나 ㆍ평균적(3460886)'인 채널 상황을 나타내는 채널
모델이 개발되어 왔다. 본 장에서는 송신 안테나가 1개이고 수신 안테나가 1개인 상황에
서 널리 사용되는 옥내 채널 모델링 기법과 옥외 채널 모델링 기법에 대하여 기술한다.

OCPD Rayleigh 페이딩 채널과 Rician 페이딩 채널

옥내 채널 또는 옥외 채널에 상관없이 일반적인 무선 채널은 그림 2.1에 나타난 바와
같이 NLOS(Non Line—of-Sight) 환경과 LOS(Line—of-Sight) 환경으로 구분할 수 있다.
1장에서 설명한 바와 같이 NLOS 환경에서 수신되는 신호의 확률밀도함수(0706806116
Density Function)= Rayleigh 분포로 유도되며, LOS 환경에서 수신되는 확률밀도함수는
Rician 분포로 유도된다.

확률 변수 에 대하여 Rayleigh 확률밀도함수는 다음과 같이 주어진다.

:

xX 2
200=-ㅜㅇ^                       (2.1)
Oo
여기서 x2] 평균 ABS 20"이다. A} (2.1)2] Rayleigh SSE 4-Fe Gaussian 분포
를 갖는 두 랜덤 변수를 자승하여 합한 후 제곱근은 취하여 새로운 랜덤 변수를 생성할


===== PAGE 48 =====
제2장_ 9150 채널 모델링

이그 scatters

—_     \                                 그    scatters
가       \               —
we                   \                             Line-of-Sight
Sy.                   ~. mobile               SX                      mobile
|     SS           oS receiver             .              호 receiver
transmitter        SON              a              transmitter                              4

4

(a) Rayleigh 페이덩 채널 전파 환경

그림 2.1 Rayleigh 페이딩 채널

이

| Rician 페이딩 채널의 전파 환경

경우 그 랜덤 변수의 분포가 된다. 즉, 각각 /(0,0”) 의 BES 갖는 | 과 랜덤 변수
aS.
꼬들

의 자승의 합은 (chi-square) 분포가 되며, 이 값의 제곱근은 Rayleig

wall 구라                                                 (2.2)

^
도

여기서 x= Al (2.1)에 주어진 Bat 전력인 20? 인 Rayleigh 분포를 갖는다. MATLAB
에 내장된 Gaussian 랜덤 HES 생성하는 함수는 '8000'로서 (0, 1)의 분포를 갖기
때문에 프로그램 작성 시 이를 쉽게 이용하기 위하여 식 (2.2)를 다음과 같이 수정할 수

= 1
있다.
x= 시즈 +25                                       (2.3)
여기서 새로운 변수 23t 2 N(0, 1)의 BBS ie Gaussian 확률 변수이다.
일반적으로 무선 통신 시스템에서 무선 채널은 실                 는 복소
이며 N(0,0° /2) 의 Gaussian

적
수부의 자승의 합이며, 평균 전력
이 0" 인 Rayleigh 분포를 갖게 된다. 이러한 복소 채널은 다음과 같이 모델링된다.

어진다. 이러한 복소 채널에서 실수부와 허수부

개
갖는다. 이 복소 채널 계수의 크기는 실수부와 ㅎ



===== PAGE 49 =====
PART 1 _무선 채널 모델링과 MATLAB

h =z,+j-2z,                             (2.4)

[는다. |씨= / 이라고 한다면 FE 다

여기서 4는 평균 전력이 0”인 Rayleigh BES

음과 같이 Rayleigh BES 갖는다.

나

Rician 페이딩 채널은 그림 2.1에서 나타난 바와 같이 송신한 신호가 반사, 산란, 굴절
존재

등에 의하여 손실되지 않고 직접 수신되는 신호인 LOSI} 존재하는 무선 채널의 경우에
해당한다. 이러한 경우 확률 변수 xo} 대하여 81008 확률밀도함수는 다음과 같이 주어
진다.

(oy        Oo

여기서 (ㆍ )는 수정된 ALE 0% Bessel BES 나타낸다. 또한, ㅇ^은 LOS AHO] A
력을 나타내고, 20^ 은 식 (2.1)에 주어진 Rayleigh 확률밀도함수에서 산란 성분
의 합을 나타낸다. 이 때, 81080 K -18000ㅠ는 식 (1.59)에 주어져 있다. 총 전력이 1인

우에, K 가 0이면 LOS 성분이 존재하지 않기 때문에 크기 BEE Rayleigh 확률밀도함
수를 갖게 되며, & 가 증가할수록 Gaussian 분포에 접근한다. 일반적으로 K 7} -4008

et
ox,
tr
때
(8
모비
ot Ih

Al o|H Rayleigh 재널로 가정하고, K 가 1508 이상이면 Gaussian AYES 가정한다. 채
BS 모델링할 ol] Rician 페이딩은 LOS 환경에서 발생되며 이러한 환경에서는 반사없
이 신호가 도착하기 때문에 일반적으로 첫 번째 탭 채널을 모델링할 때에 적용된다. 그림

2.2는 프로그램 2.1(“00 101 ric 00”)에서 프로그램 2.2(“rayl_model”)2} 프로그램 2.3
(“16 100061”)을 이용하여 생성한 Rayleigh 페이딩 채널과 Rician 페이딩 채널의 확률 분
포를 보여주는데, 이 그림에서 확인할 수 있듯이 이 페이딩 채널은 K 7} -4008일 때
Rayleigh 분포에 근접하며, K 가 1508일 때 Gaussian HES 갖게 된다.

_ 050



===== PAGE 50 =====
제2장 9150 채널 모델링

25          1         T         T         T                   T         ㅜ

—를-- Rayleigh

—@— Rician, K=-40dB
—&— Rician, K=15dB

Occurance
wn

0.5

0         0           1          15         2        2.5         3         3.5         4
x

그림 2.2 Rayleigh 페이딩 채널과 Rician 페이딩 채널의 확률 분포

* do rayl ric _ch.m
N=200000; level=30; K_dB=[-40 15];
rayl_ch=zeros(1,N); rician_ch=zeros(2,N) ;
color=["k"]; lime=['<']; marker=["s', ‘o*|'*']
% Rayleigh model
rayl_ch=rayl model (N) ;
[temp x] =hist (abs(rayl_ch(1,:)),level) ;
plot (x,temp, [color(1) line(1) marker(1)]),hold on
% Rician model
for i=1:length(K_dB) ;
rician_ch(i,:)=ric_model (K_dB(i),N);
[temp x]=hist (abs(rician_ch(i,:)),level);
plot (x,temp, [color(1) line(1) marker (i+1)]);

end
ylabel ('Occurance') ,xlabel('x');
legend('Rayleigh','Rician, K=-40dB','Rician, K=15dB')

fel 프로그램 2.1 Rayleigh 페이딩 채널과 Rician 페이딩 채널 모델 실행 프로그램

051



===== PAGE 51 =====
PART 1 _무선 채널 모델링과 MATLAB

function H=rayl_ model (L)
% Rayleigh Channel Model
%      L : number of channel realizations
%     h : channel vector
H = (randn(1,L)+j*randn(1,L))/sqrt (2) ;
il 프로그램 2.2 Rayleigh 페이딩 채널 모델 함수
function H=ric_model (K_dB,L)
% Rician Channel Model
%     K_dB : K factor [dB]
K = 10*(K_dB/10) ;
H = sqrt (K/(K+1)) + sqrt (1/(K+1))*rayl_model (L) ;
에 프로그램 2.3 Rician 페이딩 채널 모델 함수

6 ~ su 채널 모델링 기법

옥내 채널은 AAS 사무실에서 크게는 쇼핑몰 정도의 환경을 나타내며 일반적으로 사
방이 벽으로 둘러싸여 있는 특징이 있다. 이러한 이유로 옥내 환경에서의 PAS(Power
Azimuth Spectrum)= 균일(0401[0200)하다. 즉, 모든 방향에서 단말기로 동일한 전력을 갖
는 산란(60806008) 재이 Heber 또한, 페데  a 서는 단말의 이동성을 i. i

도 즉정한

따라 다른 채널 값이 4g 수  있기 eo} 이를 전형적 적인 지연 시간과 평균 wag a
는 PDP(Power Delay Profile)= 모델링한다. 정적(66400): 채널이란 시간이나 위치가 주
어지면 그 환경에서 데이터를 전송하는 배서 채널이 변하지 않는 경우를 의미한다.
채널이 시변하는 환경은 단말기가 이동하는 경우 또는 단말기가 이동하지 않더라도 단말

기 주위의 산란 성분(물체나 사람)이 이동하는 : 경우이 발생한다. 다만, 채널의 시변 정도
가 데이터 전송주기에 비해 매우 느려서 데이터를 전송하는 동안에 채널이 변하지 않는다
고 볼 수 있으면 ㆍ준정적 Al 'A(quasi-static 0080061)'이라 정의한다. 많은 경우에 옥내 채

정적 혹은 준정적 wae 가정하고 모델링 한다.

eal
=  =f ~

flo y

052

23


===== PAGE 52 =====
제2장_ 8150 채널 모델링

EAM 임반적인 옥내 채널 Bag 기법

본 절에서는 옥내 채널의 PDP Bae 많이 사용되는 간단한 2-ray 모델과 지수 모델
(exponential 010061)에 대하여 설명한다.

2-ray 모델은 그림 2.3에 나타난 바와 같이 지연 시간이 0인 직접 경로와 ㅎ 시간만큼

지연된 뒤에 입사되는 반사 경로의 두 개의 경로로만 구성되며, 이들 두 경로의 전력은 동
일하다고 가정한다. 첫 번째 경로의 지연을 ,=0라 하고 두 번째 경로의 지연을 <이라
하면 평균 초과 지연(02680 excess delay) 72 T=7,/2 이며, 최대 초과 지연(078×10140
excess delay) <, =7,°|t}. 평균 초과 지연으로부터 얼마나 확산되었는지를 YEE rms
AAS 0, =1,/20|c}. 결과적으로 2-ray Belo] 채널 SYS 단지 두 번째 경로의 지연
시간에 의해서만 결정된다. 2Q-ray 모델은 매우 단순하기 때문에 쉽게 ALS 수 있지만
일반적으로 반사체에 의하여 지연되어 수신된 두 번째 경로의 크기는 지연없이 수신된 A
번째 경로의 크기보다 작기 때문에 실제 무선 환경과 차이가 많이 있다. 2—ray se 단
지 첫 번째 경로가 B+PAlabsorberyol 의하여 가려져 있어 전력의 일부를 손실하고
된 경우에 가능한 모델이다. 그림 2.3(2)는 프로그램 2.4(“plot_2ray exp | -…
로그램 2.2(051 100001”)를 이용하여 얻어진 것으로서, ms 지연 확산이 3008이고, 샘플
링 시간이 1005인 경우에 2-ray DAS 생성한 AWS 보여준다. 이로부터 10000개의 =
시 채널에 대한 평균 전력이 이상적인 Daa 유사함을 알 수 있다.

r

{eI   v3

2-ray model                                                                 Exponential model
ㅜㅠ     -    T      ㅣ      T      T      T                     T      T      T      T   a |    as    ea Ee
—© 1068     |                                      — Ideal
0.6+                          —* Simulation                                       —* Simulation |
T, =T,, = 60726

m

oS
Q
T

=
on
2
-@
은
nn

Channel Power [linear]
os 은 은
6032     wo      기
ㅣ       - 은
| 100빼
Channel Power [linear]
은 은 은
ine)     wo     [개
T         — - “원
1                               =

=
T

S
T

                00000”

0 20 40 60 80 100 120 140    0     60 80 100 120 140
delay [ns]                                                       delay [ns]

(a) 2-ray 모델                             (b) 지수 모델
그림 2.3 2-ray 모델과 지수 모델의 예

=
=

053



===== PAGE 53 =====
PART 1 무선 채널 모델링과 MATLAB

지수 모델은 채널의 평균 전력이 지수적으로 감쇄하는 모델로 2-184 모델보다 실제 옥
내환경에 적합하며, 이 모델의 POPE 다음과 같이 주어진다.

1  —tlty
rie                            (2.7)
여기서 Ta = PDPS 결정짓는 파라미터로서, 지수 BAS] POPE 단지 7,9] 의해서만 A
정된다. 이러한 Blo] 평균 초과 지연은 *=ㅎ가 되며, rms 지연 확산은 O, =7, 7} 되
기 때문에 식 (2.7)에서 Fa 대신에 평균 초과 지연 TU rms 지연 확산 O, 2 대체할 수
있다. 최대 초과 지연 시간 Tn & 다음과 같이 주어진다.

T, =—T, nA                                                       (2.8)

여기서 4 첫 번째 경로의 크기에 비하여 상대적으로 가장 작은 중요한 전력, S 잡음
이 아닌 지연 경로의 크기로 고려할 수 있는 최소 크기를 나타내는 것으로

A= P(Z,,)/ PO)=exp(-,, /T,) B 주어진다. T 대신에 ms 지연 확산 O, 로 대체하고

샘플링 시간 를 고려하면 식 (2.7)의 이산 시간 BIS 다음과 같이 수정된다.

1 pig

여기서 ? 와 “는 각각 샘플링 주기 Tso] 의하여 이산화된 시간 인덱스와 최대 |
을 갖는 마지막 경로의 인덱스를 의미하고, Pow =[%/Ts |e 주어진다. 여기서
(ㆍ)ㅣ 는 (ㆍ)보다 큰 가장 작은 BES 의미한다. 식 (2.9)의 이산 시간 모델의 전체

1   @ (Pmax 0272
(2.10)

22 = =P == Sa

식 (2.10)에서 전체 전력 {을 1B 정규화 하기 위해서는 식 2.9)S 다음과 같이 수
정한다.

_ 054



===== PAGE 54 =====
제2장_6150 채널 모델링

202)=200)6"……,     Dp =0,1, +++, Pray         (2.11)

여기서 2(0)는 전체 ABS 12 정규화하기 위한 A 번째 경로의 전력이며, 2(0)=
1/(2,., ,ㆍ6, )으로 주어진다. 그림 2.306)는 프로그램 2.4(“010( 200 _6×0 00001”)에서
프로그램 2.5(“exp_pdp”)S 이용하여 얻어진 것으로서, mms 지연 확산이 3008이고, 샘플
링 시간이 1008인 경우에 지수 모델을 생성한 결과를 보여준다. 이로부터 10,000개의 순
시 채널에 대한 평균 전력이 이상적인 모델과 유사함을 알 수 있다.

% plot_2ray_exp_model.m

clear, clf
scale=le-9;      6 nano
Ts=10*scale;      % sampling time

t_rms=30*scale; % RMS delay spread

num_ch=10000;     % number of channels

% 2-ray model

pow 2=[0.5 0.5];

delay 2=[0 t_rms*2]/scale;

H_2 = rayl_model (num 01) .'*sqrt (pow_2) ;

avg_pow h 2 = mean(H_2.*conj(H_2));

subplot (221)

stem(delay_2,pow 2,'ko'), hold on, stem(delay_ 2,avg_pow_h 2,'k.');
xlabel('delay [ns]'), ylabel('Channel Power [linear]');
title('2-ray Model');

legend('Ideal','Simulation'); axis([-10 140 0:0.7]);

% exponential model

pow_e=exp_pdp(t_rms,Ts) ;

delay _e=(0:length(pow_e)-1)*Ts/scale;

H_e = rayl_model (num_ch) .'*sqrt (pow_e) ;

avg pow h 6 = mean(H_e.*conj(H_e));

subplot (222)

stem(delay_e,pow_e,'ko'), hold on, stem(delay_e,avg_ pow h e,'k.');
xlabel('delay [ns]'), ylabel('Channel Power [linear]') ;
title ('Exponential Model');
legend('Ideal','Simulation'); axis([-10 140 0 0.7]);

Ta) 프로그램 24 2-ray 모델과 지수 모델 실행 프로그램

055


===== PAGE 55 =====
PART 1 _무선 채널 모델링과 MATLAB

function pdp=exp_pdp(tau_d,Ts,A_dB,norm_flag)
Exponential PDP generator

o Inputs:

%      tau_d     : rms delay spread [sec]

%      Ts        : Sampling time    [sec]

%      A 08      : smallest noticeable power [dB]
%      norm_flag : normalize total power to unit
를 Output:

%      pdp       : PDP vector

if nargin<4, norm flag=1; end    % normalization
if nargin<3, A_dB=-20; end       % 2008 below
sigma_tau=tau_d; A=10*(A_dB/10);

lmax=ceil (-tau_d*log(A) /Ts) ;        % 41 (2.8)

[0

* compute normalization factor for power normalization
if norm_flag
p0=(1-exp(-Ts/sigma_tau) ) /(1-exp(-(lmax+1)*Ts/sigma_tau)); * “ (2.10)
else   p0=1/sigma_tau;
end
% exponential PDP
1=0:lmax; pdp = p0*exp(-1*Ts/sigma_tau); % “ (2.11)

Ta) 프로그램 2.5 지수 모델의 POP 생성 함수

4 IEEE 802.11 채널 모델링 기법

IEEE 802.11 채널 모델은 전력이 지수적으로 감쇄하는 지수 모델(6600060081 model)
을 기반으로 모델링되었으며, 2.4GHz 대 옥내 채널을 모델링하기 위하여 IEEE 802.11b
표준화 그룹에 의하여 정의되었다[36]. PDP7} 지수 모델이기 때문에 앞서 설명한 지수 모
Bs 이용한 채널 모델링 기법과 동일한 방법으로 실행된다. 여기서 채널 임펄스 응답은
임펄스 신호가 입력되었을 경우 FIR(Finite Impulse Response) 필터의 출력을 가정한다.
각 채널 탭은 지수적으로 감소하는 평균 전력 프로파일을 갖는 독립적인 복소 Gaussian
랜덤 변수로 모델링되며, 각 탭의 시간 인덱스는 샘플링 시간의 정수배로 구성된다. 전력

띠

이 0; 인 P 번째 탭은 분산이 0; /2이고 평균이 0인 Gaussian 확률 BES 갖는다. 이
경우 / 번째 채널 임펄스 응답은 다음과 같이 주어진다.

056

00 0 00 022


===== PAGE 56 =====
제2장_ 5150 채널 모델링

h, = 2 +./ㆍ22,      Ply +s Dice                    (2.12)

여기서 219} DE 통계적으로 서로 독립적인 N00; /2) 9] 확률 변수이다. 최대 경로
FS 나타내는 Pm 는 rms 지연 확산 0, 와 샘플링 주기 Ts ol] 의하여 다음과 같이 결정
된다.

Prax ={10-0, /T, |                      (2.13)

가장 작은 전력 PWS 기준으로 최대 초과 지연 시간을 가변적으로 산출하는 지수 모
델과는 달리, IEEE 802.11 모델은 최대 초과 지연 시간을 rms 지연확산의 10배로 고정시
킨다. 이러한 경우에 각 채널 탭의 전력은 다음과 같이 주어진다.

0; =a,e                                                  (2.14)

여기서 은 첫 번째 Bo] 전력을 의미한다. 식 (2.4)에서 확인할 수 있듯이 IEEE
802.11 채널 모델의 AAS 지수함수적으로 감쇄한다. 이 때 첫 번째 Qo] 전력 oo 은 평
균 수신 전력이 1이 되도록 다음과 같은 방법으로 선정된다.

5        1 _ 2 8!%
06 _—_
1 _ @ (Prax 4+1)Ts/0,

(2.15)

IEEE 802.11 채널 모델에서 샘플링 주기 Toe 심볼 주기보다 적어도 1/4정도 작아야
한다. 그림 2.4는 2214 2.6(“plot_ IEEE80211_model”)o]A] 프로그램 2.2(“rayl_ model’)
와 2.7(“ieee802_11_model”)2 이용하여 9, 7} 2508이고, 7,7} 50278인 경우에 대해 생성
한 IEEE 802.11 채널의 평균 전력 및 순시 채널의 주파수 SHS 보여준다. 이 채널은
rms 지연 확산이 비교적 짧기 때문에 주파수영역에서 전력차는 최대 약 SMBS 주파수
선택적 페이딩이 비교적 적다.



===== PAGE 57 =====
PART 1 무선 채널 모델링과 MATLAB

IEEE 802.11 Model, o, =25ns, 16=5005                   Frequency response, o, = 25ns, Ts=50ns
1      ;     ;     ;     ;     1    +     1               10          ;          1          1
0.9+    @                      —© 1068      U             하                                            」
=                          — Simulation
s 0.8F                                             아                                   4
= 0가                              ;      a 4                              3
2 067                                 = 가                           :
Qa
3 0.5+                           4     5 OF                           4
은 0.47                                   7       고 가
을 0하                                   ;       s -아                                   |
fo)                                                   6)
§ 0.27                                   4         -하                                   4
< 0나                               |        하                               |
(a a a a         -10          1          L          Ｌ
비    0    1    2    3    4    5    6    ^          -10        =5         0         5         10
channel tap index, p                                             Frequency [MHz]
(8) 평균 채널 전력                            (b) 주파수 응

그림 2.4 IEEE 802.11 모델

% plot_IEEE80211 model.m

clear, clf

scale=le-9;        % nano

Ts=50*scale;       % sampling time
t_rms=25*scale;    % RMS delay spread
num_ch=10000;      % number of channels
N=128;             % FFT size

pdp=ieee802 11 model (t_rms,Ts) ;

h=zeros (num_ch, length (pdp) ) ;

avg_pow h=zeros(1,length(pdp) ) ;

for k=1:length (pdp)
h(:,k) = rayl_model (num_ch) .'*sqrt (pdp(k) ) ;
avg_pow h(k)= mean(h(:,k).*conj(h(:,k)));

end
H=fft(h(1,:),N);
subplot (221)

stem([0:length(pdp)-1],pdp,'ko'), hold on, stem([0:length(pdp) -1],

avg pow h,'k.');

xlabel('channel tap index, p'),ylabel('Average Channel Power [linear]') ;
title('IEEE 802.11 Model, \sigma_\tau=25ns, T_S=50ns');
legend('Ideal','Simulation'); axis([-1 7 0 1] ) ;

subplot (222)

plot ([-N/2+1:N/2] /N/Ts/10*6,10*10g10 (H.*conj (H)),'k-');
xlabel('Frequency [MHz] ')

ylabel('Channel Power [dB] ')

title('Frequency response, \sigma_\tau=25ns, T_S=50ns') ;

개 프로그램 26 IEEE 802.11 채널 모델 실행 프로그램

058


===== PAGE 58 =====
제2장_8!50 채널 모델링

function 000=1666802 11 model (sigma_t,Ts)

% IEEE 802.11 channel model pdp generator
% Input:

%     sigma_t : RMS delay spread

%     Ts     : sampling time

% Output:

%      pdp      : power delay profile

lmax = ceil(10*sigma_t/Ts); % “ (2.13)
sigma02=(1-exp(-Ts/sigma_t) ) /(1-exp(- (lmax+1)*Ts/sigma_t)); * % (2.15)

2

1=0:lmax; pdp = sigma02*exp(-1*Ts/sigma_t); * 4 (2.14)

Tm) 프로그램 27 IEEE 802.11 채널 모델의 PDP 생성 함수

ORR s-v 채널 모델링 기법

기존의 옥내 채널에 대한 많은 실험 결과를 통하여 채널 경로의 도착 시간은 포아송
(Poisson) =BAJAB 모델링될 수 있음이 확인되었다. Saleh2} Valenzuela= 옥내 채널
환경을 측정한 결과, 옥내 채널의 임펄스 응답이 다수 개의 클러스터로 구성되며 각 클러
스터는 rae 구성되는 것을 발견하고 이를 기반으로 채널 모델링 기법을 제안하였다[37].

Path Magnitude

tS    Overall
\ ‘\. envelope
My;
\       SSA ee
\      se
\ ‘cluster ““s~..
\venvelope     RS
BS          ‘    ><

SS   enw           NS                   i

cluster 0
그림 2.5 S-v 채널 모델

S—V(Saleh—Valenzuela) 채널 모델은 그림 2.5에 나타난 바와 같이 클러스터와 rayS
모델링되며, 각 경로의 도착 시간(60081 time)S 두 개의 포아송 프로세스로 모델링된다.
따라서 S-V 채널 모델은 각 경로의 지연시간이 샘플링 시간 간격(샘플링 시간의 정수배)

059



===== PAGE 59 =====
PART 1 _무선 채널 모델링과 MATLAB

으로 구성되지 않고 임의의 시간 간격으로 배치되는 특징이 있다. 즉, "번째 클러스터의
첫 번째 ray] 도착 시간으로 정의된 클러스터 도착 시간(,,)은 고정된 EAS ㅅ를 갖는
아송 프로세스로 모델링되며, 각 클러스터 내에 도착하는 105는 도착률 AS 갖는

프로세스로 모델링된다. 이러한 경우에 클러스터 도착 시간 간의 BO ray 도착 시간
의 분포는 다음과 같이 지수분포로 주어진다.

mM of 변

P(T,, |Z.) =Aexp[-A(T,, -T,,1)], m>0      (2.16)

P(T,  — ) = Aexp|-A(Z,,., - ne )|.    r>0                      (2.17)

여기서 7, 은 m 번째 클러스터의 A 번째 경로의 도착 시간을 의미하며, <, 은 mw
클러스터 내의 7 번째 185의 도착 시간을 나타낸다. 식 (2.16)과 식 (2.17)에서 # 번째 클
러스터 내 첫 번째 ray] 도착 시간(ㅠ,,)은 "번째 클러스터 도착 시간(7,), 즉
Tm = 7; 으로 정의된다. 또한 를 "번째 클러스터 내의 / 번째 ray} 크기라 하고
0., 를 이의 위상이라 하면 채널의 복소 임펄스 응답은 다음과 같이 표현된다.

Bs)

h(t) =  VY Bc 5(t-T,   -T,,)                    (2.18)

m=0 r=0
여기서 0. & [0, 27] 구간에서 독립적인 균일한 확률 BES 갖는 랜덤 변수이다. 또한
Bm 는 독립적이고 양의 부호를 갖는 랜덤 Ws Rayleigh BES 갖고 다음과 같이 주

어진다.

208 .)=(24/@2.06 ^“                                      (2.19)

여기서 B2, 는 7 번째 클러스터 내의 7 번째 ray] 평균 전력을 의미하며 다음과 같이
주어진다.

a

B= Bye er              (2.20)

__060



===== PAGE 60 =====
제2장_ 6150 채널 모델링

여기서 와 7 각각 지수적으로 감소하는 클러스터와 ray2] 전력 감쇄 시정수(4106
constant)S 나타내며, ^00은 Al 번째 클러스터의 첫 번째 18$의 평균 전력을 나타낸다.
그림 2.5에 나타난 바와 같이 S-V BAS 평균 클러스터 Ao] 식 (2.20)의 6" 에
sel 지수적으로 aati, 2 클러스터 내의 08의 dels A Game] eval ss
지수적으로 감소하는 이중 지수 감쇄 모델(0046016 exponential decay model)°|t}. 첫
번째 클러스터의 첫 번째 ray2] 평균 전력 Ayo 7t 주어지면 나머지 ray2] 평균 전력은 식
(2.20)에서 구할 수 있으며, 각 ray2] 평균 전력이 결정되면 식 (2.19)를 Foto] Rayleigh
포를 갖는 채널 계수의 크기를 구할 수 있다. 경로 손실에 대한 고려가 없는 경우에 첫
제 클러스터 첫번째 의 평균 aie [로 설정하는 것이 일반적인 heels
(2.18)의 채널 임펼스 응답에서 클러스터의 수와 rays} AL 무한 개로 주어지지만
… 의미있는 전력을 갖는 클러스터와 rye 한정되어 있으므로 클러스터의 +S M,
ray2] 수를 로 제한할 수 있다. 또한, log—normal shadow 페이딩 효과를 반영하기 위
하여 log—normal shadow 페이딩의 크기 X S 도입하면 식 (2.18)의 복소 임펄스 SYS
다음과 같이 주어진다.

Ss

c
nu

|

fe Ac

M R    |
AQ) =XDV YB. ne" 5(t-T, - Fm)            (2.21)
m=0 r=0
여기서 의 값은 전력이 아닌 크기로 주어지며 log-normal HES 갖기 때문에
20106810(4)%20(0,0?) 이다. 이 때 Fr log—normal 98800\108의 표준 편차를 나타낸다.

그림 2.6은 프로그램 2.8(“plot_sv_model_ct”)o]*] A=0.023, 2=0.023, 1'=7.4 ,
/=4.3, 0, = 3008인 경우에 대해 프로그램 2.9(“‘sv_model_ct”)S 사용하여 얻어진 9-\
모델링 결과로서, (a) 클러스터 도착 시간 분포 (6) 18$의 도착 시간 분포 (0) 채널의 임펄
A 응답 (0) 1.000번 실행된 채널의 전력 분포를 보여준다. 그림 2.602)와 (6)는 식 (2.16)
과 식 (2.17)에 주어진 클러스터와 28$의 도착 시간에 대하여 확률밀도함수 분포의 해석적
(10681) 결과와 모의실험 결과를 비교하여 보여준다. 그림 2.6(0)로부터 실행된 채널의 전

력 분포는 108-1040100181 shadowing 분포를 따름을 알 수 있다.



===== PAGE 61 =====
PART 1 _무선 채널 모델링과 MATLAB

Distribution of Cluster Arrival Time, A = 0.0233                                 Distribution of Ray Arrival Time

0.025              T             T             T             T
— 1068
— Simulation

T      T      T

r        r
— 1068
— Simulation

P(TmlTm-1)
P(Tr.mlTir-1),m)

1

S

0 50.100. 150 200 250 300     0 05 1 15 2 25 3 85 4 45 5
Tm-Tm-i [ns]                                                                                      Tm-T-» m[ns]
(8) 클러스터 도착 시간 분포                  (b) ray 도착 시간 분포
Generated Channel Impulse Response                                               Log-normal Distribution, t=3dB
0.045             ~    -    >             T  T  1  :
0.4
0.35
0.3
®D
3 0.25
=
i
3 0.2
0.15
0.1
0.05
0               ‘  Da ORE cpa        0   1   1   1
0     ee     80  100  120   =10 -8 -6 =4 =2 0 2 4 6 8 10
delay [ns]                                                               20*log10(X) [dB]
채널의 임펄스 응답                    (a) 채널의 전력 분포

그림 2.6 S-v 채널 모델의 예

8-\ 채널 모델의 MATLAB 프로그램을 실행하는 순서는 다음과 같다.

(1) 클러스터와 「3>의 수 제한 : 클러스터와 ayo] 수가 너무 많으면 모의실험에 많은 시간이
소요되고 너무 적으면 요구되는 채널의 특성을 충분히 반영할 수 없기 때문에 적당한 수
로 식 (2.16)과 식 (2.17)의 클러스터와 의 수를 제한한다. 일반적으로 클러스터의 수
/4 은 10-T 가 적당하며, ray] 수 RE 10-77} 적당하다.

(2) 첫 번째 클러스터의 첫 번째 ray] 평균 전력 결정 : /60(6002)는 식 (2.18)에서 다른
rays) 평균 ABS 결정하는 기준이 된다. 경로 손실이 적용되기도 하지만, 일반적으로

062


===== PAGE 62 =====
제2장_ 9150 채널 모델링

경로 손실 적용없이 ^60ㅋ로 설정한다.

(3) 모델 파라미터 설정 : 클러스터 도착률 ㅅ(Ｌ8300), ray 도착률 4 (lambda), 클러스터 전력
감쇄 시정수 (0800, ray 전력감쇄 시정수 (0800008)를 설정한다. 부가적으로
log—normal shadowing2] 표준편차(9180718 x)? 채널이 108인지 찌Ｌ08인지를 구별하는
파라미터(2108), 그리고 생성하고자하는 AS] 개수) SS 설정한다

(4) 클러스터 도착 시간 계산 : 식 (2.16)과 같은 지수 분포를 가지도록 /7 번째 클러스터 도착

시간 7, 을 생성한다.

(5) Ray 도착 시간 계산 : 식 (2.17)과 같은 지수 BES 가지도록 ray 도착 시간 <, 을 생성
한다.

(6) Ray2| 평균전력 계산 : 식 (2.20)으로부터 m 번째 클러스터 내의 r 번째 의 평균전력
Bin 을 계산한다.

22

(7) 채널의 크기 및 위상 생성 : ray2] 평균전력 FS 이용하여 식 (2.19)의 Rayleigh 분포
를 가지는 채널 이득의 크기 //., 을 BRT 균일한 BES 가지도록 위상을 생성하여
복소 채널 SS 생성한다.

(8) 7m <10ㆍ》 확인 : <, <10ㆍ이면 7 <-7+1로 갱신하고 (6)으로 돌아가서 계속 진행하고,
Tm =10ㆍ/인 경우에는 m 번째 클러스터 내의 ray YYS 종료하고 다음 단계를 진행한다.

(9) 7, <10-T 확인 : 1, <10:1'이면 mem+l, "0 로 갱신하여 (4)로 돌아가 77+1
번째 클러스터의 25 SS 생성하고, T, =10:[`'이면 클러스터 Wray YAS 종료하고 다
음 단계로 넘어간다.

(10) 채널 계수 및 지연 시간 정렬 : 원하는 수만큼의 채널이 모두 생성되면 클러스터 YW ray

의 도착 시간은 생성된 순서에 관계없이 임의적으로 생성되기 때문에 지연 시간에 따라
정렬해야 한다(프로그램 2.9(“9ㅠ 00000! 0[”)의 끝에서 제 5, 6행).

(11) 채널 전력 정규화 및 log—normal shadowing : log—normal shadowing2}] 표준편차 Ox 7}
주어지면 91800\108 페이딩을 적용한다(프로그램 2.9(“41 00081 "의 끝에서 제 2, 3행).

(12) 생성된 채널의 수 확인 : 생성할 ao] 남아 있으면 m0, <-0 로 갱신하고 (4)로
되돌아가 다음 번 채널을 생성한다. 원하는 수만큼의 채널이 생성되면 프로그램을 종료
한다.

063


===== PAGE 63 =====
PART 1 _무선 채널 모델링과 MATLAB

% plot_sv_model ct.m

close all, clear all

Lam=0.0233; lambda=2.5;

Gam=7.4; gamma=4.3;

N=1000; power _nom=1;

std_shdw=3;

E1=02300; t2=070.01¢5;

subplot (221)

p_cluster=Lam*exp(-Lam*t1); %* ideal exponential pdf
h_cluster=exprnd(1/Lam,1,N) ; 6 # of random numbers generated
[n_cluster × cluster] =hist (h_cluster,25); % obtain distribution
plot (t1,p cluster,'k'), hold on,

plot (x_cluster,n_cluster*p cluster (1) /n_cluster(1),'k:');% plotting
legend ('Ideal','Simulation')

title(['Distribution of Cluster Arrival Time, \Lambda=' ,num2str (Lam) ] )
xlabel('T_m-T_{m-1} [ns]'), ylabel('p(T_m|T_{m-1})')

subplot (222)
p_ray=lambda*exp(-lambda*t2); %

h_ray=exprnd(1/lambda,1,1000); % # of random numbers generated

[n_ray x_ray]=hist(h_ray,25); % obtain distribution

plot (t2,p_ray,'k'), hold on,

plot (x_ray,n_ray*p_ray(1)/n_ray(1),'k:'); % plotting
legend('Ideal', 'Simulation')

title(['Distribution of Ray Arrival Time, \lambda=',num2str (lambda) ] )
xlabel ('\tau_{r,m}-\tau_{ (r-1) ,m} [ns] ') ,ylabel ('p(\tau_{r,m}|\tau_{(r-1), m})')
subplot (223)

[h,t,t0,np] = sv_model_ct (Lam, lambda, Gam, gamma,N,power_nom,std_shdw) ;
stem(t(1:np(1),1),abs(h(1:np(1),1)),'ko');

title('Generated Channel Impulse Response')

xlabel('delay [ns]'),ylabel ('Magnitude')

subplot (224)

X=10.*(std_shdw*randn(1,N) ./20) ;

{temp x] =hist (20*log10(X) , 25) ;

plot (x,temp,'k-'), axis([-10 10 0 120])

title(['Log-normal Distribution, \sigma_X=',num2str(std_shdw) ,'dB'])
xlabel ('20*10g10 (X) [dB] ') ,ylabel ('Occasion')

ideal exponential pdf

—

Tal 프로그램 28 S-v 채널 모델 실행 프로그램

064



===== PAGE 64 =====
제2장_ 6150 채널 모델링

function [h,t,t0,np]=sv_model_ct (Lam, lam,Gam,gam,num_ch,b002,sdi,nlos)
S-V channel model

%

6 Inputs

6 Lam     : Cluster arrival rate in GHz (avg # of clusters per nsec)
6 lam     : Ray arrival rate in GHz (avg|# of rays per nsec)

% Gam     : Cluster decay factor (time constant, nsec)

6 gam     : Ray decay factor (time constant, nsec)

% num_ch : number of random realizations to generate

6 nlos    : Flag to specify generation of NLOS channels

6 sdi     : Standard deviation of log-normal shadowing

%            of entire impulse response in dB

% b00     : power of first ray of first cluster

6 Outputs

응   h     : a matrix with num_ch columns, each column having a random
%             realization of channel model (impulse response)

6   t      : time instances (in nsec) of the paths

%             whose signed amplitudes are stored inh

%   to     : arrival time of the first cluster for each realization
%   np     : number of paths for each realization.

if nargin<8, nlos=0; end    % LOS environment

if nargin<7, sdi=0; end    % 008
if nargin<6, nlos=0; sdi=0; b002=1; end
% power of first ray of first cluster
h_len=1000;
for k=1:num_ch    * loop over number of channels
tmp_h = zeros(h_len,1); tmp_t = zeros(h _len,1);
if nlos, Te = exprnd(1/Lam) ;
else     Toe = 0;   % first cluster arrival occurs at time 0
end
to(k) = Te;
path_ix = 0;
while (Tc<10*Gam) % cluster loop
ir=Oir
while (Tr<10*gam) % ray loop
t_val = Tc+Tr; % time of arrival of this ray
bk12 = b002*exp(-Tc/Gam) *exp(-Tr/gam); % ray power, *! (2.20)
r = sqrt (randn*2+randn*2) *sqrt (bk12/2) ;

065



===== PAGE 65 =====
PART 1 _무선 채널 모델링과 MATLAB

h_val=exp(j*2*pi*rand)*r; % uniform phase
path_ix = path_ix+l;       % row index of this ray
tmp_h(path_ix) = h_val; tmp_t(path_ix) = t_val;
Tr = Tr + exprnd(1/Lam) ;
end
Te = Tc + exprnd(1/lam) ;
end
np(k)=path_ix; % number of rays (or paths) for this realization
[sort_tmp_t,sort_ix] = sort(tmp_t(1:np(k))); % in ascending order
t(1:np(k),k) = sort_tmp_t;
h(1:np(k),k) = tmp _h(sort_ix(1:np(k)));
% log-normal shadowing on this realization
fac = 10*(sdi*randn/20) /sqrt (h(1:np(k) ,k) '*h(1:np(k),k));
h(1l:np(k),k) = h(l:np(k),k)*fac; 4 4 (2,21)
end

Tm) 프로그램 2.9 8-\ 채널 모델 St

+

98 Uwe 채널 모델링 기법

AT&T, Intel, Time Domain 등에서 실제 채널을 측정하여 발표한 결과들로부터 광대
역 옥내 채널은 9-\ 채널 모델에서 고려하고 있는 클러스터링 현상이 있으나 8-\ 채널
모델에서 고려한 협대역 옥내 채널과 달리 다중경로의 크기 페이딩이 #8516091 분포보다
는 log-normal 분포나 Nakami 분포에 근접한다는 것을 확인할 수 있다. 이러한 결과를
토대로 90438 UWB 다중경로 모델은 클러스터 도착 신호가 독립적인 108-14ㅁ01008! 페이딩
을 겪도록, 또한 클러스터 내의 ray 도착 ASE 독립적인 108-100170881 페이딩을 ALS
S-V BAS 수정하여 개발되었다[38].

UWB 다중경로 모델의 : 번째 생성된 이산시간 임펄스 응답은 다음과 같이 주어진다.

M R
A(n=X, > Yda,O(t-Ti -7.,,)                                       (2.22)

m=0 r=0

여기서 *:,는 /번째 생성된 채널의 다중경로 이득 계수이며, ㅅ,는 log—normal
shadowing 랜덤 변수를 나타낸다. 또한 7는 7 번째 생성된 MIS 나타내지만 식의 간략
화를 위하여 이후의 표기에서는 77S 삭제한다. 클러스터 및 ray 도착 시간의 BRE

066



===== PAGE 66 =====
제2장_ 9150 채널 모델링

S-V 채널 모델과 동일하게 식 (2.16)과 식 (2.17)의 두 개의 포아송 프로세스로 모델링된

다. UWB 채널 모델은 기존의 5-\ 채널 모델과는 달리 클러스터와 ray7} 서로 독립적인

페이딩을 Au] 각각 log—normal 페이딩을 겪는 것으로 가정한다. 이 경우 채널 계수는
음과 같이 주어진다.

Om = Prm mom                                           (2.23)

여기서 ㅇ6,는 분산이 이 인 7 번째 클러스터의 108-0ㅁ00001 페이딩을 나타내며, ^, 는

분산이 03 인 m 번째 클러스터 내의 번째 의 log—normal 페이딩을 나타낸다. 클러
스터 페이딩과 ray 페이딩이 서로 독립적임을 가정하고 있기 때문에 확률변수

n, © N(0,07) 와 my %70(0.03)는 독립적이다. 또한 ^, 는 반사에 의하여 발생할 수 있
임의의 BA 반전을 반    sas 위하여 추가된 것으로 동일한 확률을 갖는 419] 값을
는다. 식 (2.18)에 주어진 S-V 채널 모델의 채널 계수와 비교할 때 UWB 모델의 채널
AB (0, 271이서 Be  하게 분포하는 Fae] 아니고 단지 - 혹은 의 ahs 가지므
로 채널의 계수는 항상 실수가 된다. 또한, 5-\ 채널 모델에서 Rayleigh 분포인 각 8의

clr

A

pice

크기가, UWB 채널 모델에서는 108-10ㅁ01001 분포인 클러스터, Sn 2 log—normal 분

포우
ray, Bm 의 FOB 표현된다. 식 (2.23)에서 두 log—normal 랜덤 변수의 곱은 또한

+
log—normal 랜덤 변수이기 때문에 채널 계수의 크기 68, = 10 2% of sa ee
log—normal 분포이며, 201og10(¢,, 4...) oc N(Ly moO +03) 이다. 채널 계수의 평균 전력
은 다음과 같이 주어진다.

이 Bn, ‘| =Q,e Te t'”                               (2.24)
여기서 906; 은 Al 번째 클러스터의 A 번째 ray] 평균 ABS 나타낸다. 채널의 크기 분
B(log—normal 분포)의 평균치를 나타내는 /《,,는 다음과 같이 주어진다.

-100(@96)-107,/7-1003 77 (60 +00)0ㅁ00
Bran =           1000)                  20

(2.25)

067



===== PAGE 67 =====
PART 1 _무선 채널 모델링과 MATLAB

Al (2.22)에서 전체 다중경로의 전력에 대한 log—normal shadowing®] 크기를 나타내는
X,= 20logl0(X,) < N(0,o7) S$ 따른다

UWB 채널 모델은 8-\ 채널 모델에서 채널의 SYS 결정짓는 파라미터인 클러스터
EAS A, ray EAS A, 클러스터 감쇄 상수 1', ray 감쇄 상수 7, 전체 다중경로 전력
에 대한 log—normal shadowing2] 표준편차 ㅇ,이외에 클러스터 log—normal 페이딩의
표준편차 이 , ray lognormal 페이딩의 표준편차 ㅇ: 의 파라미터가 추가되어 UWB 환경
을 반영한 AMS 생성한다. 식 (2.22)를 사용하여 최종적으로 모델링된 다중경로 채널
A(t) 는 실수값으로 주어진다. 위 채널 모델에서는 입의의 도착 시간을 갖기 때문에 주파
수 대역이 제한되지 않아 실제 UWB 채널을 사용하는 모의실험을 위해서는 하향변환
(down-—conversion) 및 필터링 SS 통한 적절한 수정이 필요하다.

표 2.1 UWB 채널 파라미터와 모델 특성

Mean excess delay (nsec) (? )       5.05      10,38      14,18
RMS delay (nsec) (9)          5,28      8,03      14,28       25
NPioap                                       28
NP (85%)                                          61,54
ee
A (1/nsec)            0.0233     0.4     0.0667    0.0667
X (1/nsec)             25      O25      01      Pak
vie                    teal        50       14.00      24.00
7                    4.3        6.7        7.9        12
01 (dB)            3.3941    3.3941    3.3941    3.3941
a4 (dB)                  3.3941      3.3941      3.0941      83,3941
a, (dB)
eM SRST) ED SA RE
Mean excess delay (nsec) (T )                   9.         15.9       80,1
rms delay (nsec) (9)            5         8         15        25
NPioas                  12.5       15,3       24,9       41.2
NP (85%)                20.8       33,9       64,7      123 2
Channel energy mean (dB)        -0.4      -0.5       00       0.8
Channel energy std (dB)          2.9        3.1        3.1        207

_068



===== PAGE 68 =====
Impulse response realization

0            20           40           60

Excess delay (nS)
|

ㅇ

i

제2장 5150 채널 모델링

80    100   120    9        30 40 50 60 70 80 90 100
Time (ns)                                                                                   Channel number
「     …   기                        ee   _
(a) 채널 임펄스 응답                     (b) 평균 초과 지연
RMS delay (nS)                                                                        Number of significant paths within 10 dB of peak
16   ;           7   i      7          25   7   ;   7   T   i      1   1
|                    |          zo}. |   |      가 ent a a
0           10          20          30          40          50          60          70          80          90         100                       0           10          20          30          40          50         60          70          80          90         100
Channel number                                                                                     Channel number
=                                        스
(0) RMS 지연확산                 (0) 전력이 1008 이내인 경로 수
Average Power Decay Profile                                             10                                  Channel Eneray
--- Mean
|                                               하                             + £8td. deviation
사
"|                                        |  |      |
;                                    il     |  |
roy
3-30                                   2 aly     LUE A
이
은
고 bis
=< -40                                     —4b         i   V
-하
-50 }--
-하
-60     1!     !     !     !     {        -10   peg gd 100
20   40   60   80   100      0 10 20 30 40 50 60 70 80 90 100
Delay (nsec)

(e) 평균 PDP

Channel number

(f) 채널 에너지

그림 2.7 UWB 채널의 생성 예(0041)

069



===== PAGE 69 =====
PART 1 _무선 채널 모델링과 MATLAB

UWB 채널을 생성하기 위한 모델 파라미터는 채널의 평균 초과 지연, mms 지연 확산
전력이 1008이내인 다중경로의 수, PDP 등이 실제 환경에서 측정된 채널의 결과와 일치
하도록 선정되어야 한다. 표 2.1은 모델링하고자 하는 채널의 특성, 이를 만족시키는
90338 채널 모델의 파라미터, 모델 SAYS 4가지 채널 모델에 대하여 요약하여 보여준다.

표 2.1에서 UWB 채널 모델은 041, CM2, CM3, CM42] 4가지 종류로 주어지며, 이
Bae 거리 및 Ｌ08의 유무에 따라 다르게 구성된다. CM12 0-40거리의 LOS 환경,
CM2%= 0-40 거리의 NLOS 환경, CM3-2 4-10m 거리의 NLOS 환경에서 측정된 채널
특성을 기반으로 하는 모델이다. 또한, CM42] 경우에는 실제 측정된 채널의 특성은 아니
지만 극단적인 NLOS 채널을 모델링하기 위하여 rms 지연 확산을 매우 길게(2508) 모델
파라미터를 인위적으로 설정한 것이다. CMIS 거리도 짧고 LOS 환경이기 때문에 RMS
지연확산이 5.28ns= 채널 모델 중 가장 좋은 채널이며, CM22] 경우에 거리는 0841과 같
으나 NLOSS}40]7] 때문에 mms 지연 확산이 CM12t} = 8.0308이다. CM3= 거리도
비교적 멀고 NLOS 환경이기 때문에 RMS 지연확산이 14.2828로서 상당히 열악한 환경
을 모델링하고 있다.

그림 2.7은 표 2.1의 모델 파라미터를 사용하고 프로그램 2.10을 실행하여 구한 결과를
보여준다. 이 그림은 UWB 채널 모델링 기법으로 모델링된 100개의 0341 채널에 대한
임펄스 응답, 평균 초과 지연, ms 지연 확산, 평균 PDP, 전력이 1008 이내인 경로 수, A
널 에너지 등의 채널 특성을 보여준다. 이 때 샘플링 주기는 167208로 설정되었다. 생성된
채널의 RMS 지연 확산은 508로 Ep 채널 특성의 RMS 지연확산과 거의 일치하며, 또한
초과 지연도 508로 거의 일치하는 것을 확인할 수 있다. 결과적으로 Bags 채널이 실

제 모델링하고자 했던 채널의 특성과 비교하여 정확하게 모델링되었음을 알 수 있다.

9038 UWB 채널 모델을 생성하는 방법은 채널 계수의 크기를 생성하
2

S-V 채널 모델과 동일하기 때문에 2.2.3절의 프로그램에 다음의 절차를 수정

로써 UWB 채널 모델을 생성할 수 있다. 따라서 프로그램 2.11에 수정 또는 추가될 항목만 기

술하기로 한다.

(3) 채널 계수의 log—normal 페이딩 관련 파라미터 추가 : 클러스터 108-4010081 페이딩의
표준편차 1, ray log—normal 페이딩의 표준편차 를 설정한다.

(6-1) 클러스터 100-ㅁ00081 페이딩 계수 생성 : 7 번째 클러스터의 log—normal 페이덩의

070


===== PAGE 70 =====
제2장 6150 채널 모델링

응 UWB_ch.m
clear, clf               |
Ts = 0.167; num_ch=100; randn('state',12); rand('state',12); cm = 1;
[Lam, lam,Gam,gam,nlos,sdi,sdc,sdr] = uwb_sv_params(cm) ;
[h_ct,t_ct,t0,np] = uwb_sv_model_ct(Lam,lam,Gam,gam,num_ch,nlos,sdi,
sdc,sdr) ;
[hN,N] = uwb sv_cnvrt_ct(h_ct,t_ct,np,num_ch,Ts) ;
h = resample(hN,1,N); h = h*N; channel energy = sum(abs(h) .*2);
h_len = size(h,1); t = [0:(h_len-1)]*Ts;
for k=1:num_ch
sq_h = abs(h(:,k)) .*2/channel_energy (k) ;
t_norm= t-t0(k); excess _delay(k) = t_norm*sq_h;
rms_delay(k) = sqrt ((t_norm-excess_delay(k)) .*2*sq_h) ;
temp_h = abs(h(:,k)); threshold_dB = -10;
temp thresh = 10*(threshold_dB/20) *max(temp_h) ;
num_sig paths(k) = sum(temp_h>temp_ thresh) ;
temp_sort = sort (temp _h.*2) ;
cum_energy = cumsum(temp sort (end:-1:1))j;
x = 0.85; index_e = min(find(cum_energy >= x*cum_energy (end) ) ) ;
num_sig e paths(k) = index_e;
end
energy mean = mean(10*log10(channel_ energy) ) ;
energy stddev = std(10*log10(channel energy) ) ;
mean excess delay = mean(excess delay) ;
mean_rms delay = mean(rms_ delay) ;
mean_sig paths = mean(num_sig_ paths) ;
mean sig e paths = mean(num_sig e paths) ;
temp average power = sum(h'.*h') /num_ch;
temp average power = temp average _power/max(temp_average power) ;
average decay profile dB = 10*logl0(temp average power) ;

l@ 프로그램 210 UWB 채널 모델 실행 프로그램

071



===== PAGE 71 =====
PART 1 _무선 채널 모델링과 MATLAB

function [Lam, lam, Gam, gam,nlos,sdi,sdc,sdr] =uwb_sv_params (cm)

% Table 2.1:

tmp = 4.8/sqrt (2) ;

Th2 l= [0.0233 2.5 7.14.3 03 tmp tmp; 0.4 0.55.5 6.7 1 3 tmp tmp;
0.0667 2.1 14.0 7.9 1 3 tmp tmp; 0.0667 2.1 24 12 13 tmp tmp] ;

Lam=Tb2_1(cm,1); lam=Tb2_1(cm,2); Gam=Tb2_1(cm,3); gam=Tb2_ 1(cm,4);

nlos= Tb2_1(cm,5); sdi= Tb2 1(cm,6) ;

sdc= Tb2_1(cm,7); sdr= Tb2_1(cm,8);

 프로그램 211 UWB 채널 모델의 파라미터 설정 함수

function [h,t,t0,np] = uwb_sv_model_ct (Lam, lam,Gam,gam,num_ch,nlos,sdc,
sdr,sdi)
std_L=1/sqrt (2*Lam) ; std_lam=1/sqrt (2*lam) ;
mu_const=(sdce*2+sdr*2) *log(10) /20; h_len=1000;
for k = 1:num_ch
tmp_h = zeros(h_len,1); tmp_t = zeros(h _len,1);

if nlos
Te = (std_L*randn) *2+(std_L*randn) “2;
else    Te = 0%
end
tO (k)   Te; path 1x = 0;

(Tc<10*Gam)
= 0; ln_xi=sdc*randn;
alte (Tr<10*gam)
t_val = (Tc+Tr);
mu = (-10*Tc/Gam-10*Tr/gam) /109 (10) - mu_const;
In_beta = mu + sdr*randn;
pk = 2*round (rand) -
h_val=pk*10*((1n_xi+1ln_beta) /20) ;
path_ix = path_ix +1;
tmp_h(path_ix) = h val;
tmp_t(path_ix) = t_val;
= Tr + (std_lam*randn) *2+(std_lam*randn) *2;

_

end
Te = Tc + (std_L*randn) *2+(std_L*randn) *2;
end
np(k) = path_ix; [sort_tmp_t,sort_ix] = sort (tmp_t(1:np(k)));

ela
t(1:np(k),k) = sort_tmp_t;

hide mp 06) 7  k) = tmp_h(sort_ix(1:np(k)));

fac = 10*(sdi*randn/20) /sqrt (h(1:np(k) ,k) '*h(1:np(k),k));
h(1:np(k),k) = h(1:np(k) ,k)*fac;

end

(i) 프로그램 212 UWB 채널 모델 함수

072


===== PAGE 72 =====
Al2et siso 채널 모델링

function [hN,N] = uwb_sv_cnvrt_ct(h_ct,t,np,num_ch, Ts)
min Nfs = 100; N=2“nextpow2 (max(1,ceil(min_Nfs*Ts) ) ) ;
Nfs = N/Ts; t_max = max(t(:));
h_len=1+floor(t_max*Nfs); hN = zeros(h_len,num_ ch) ;
for k = 1:num_ch

np_k = np(k);

t_Nfs = 1+floor(t(1:np_k,k)*NE£s) ;

for n= 1176 k

hN(t_Nfs(n),k) = AN(t_Nfs(n),k) + h_ct(n,k);
end

end

010
으
=
Se
N
pall
mt
Hu
rE
rok
oli
rr
pot
+s

DSTA 213 UWB 채널 모델에서 연속시간 채널

060 ee

6 FWon 모델링 기법
FWGN(Filtered White Gaussian Noise) 모델은 다양한 도플러 스펙트럼을 표현할 수
있어 가장 널리 사용되는 모델 중의 하나이다. 1.3절에 기술한 Clarke/Gan 모델이 가장 기
본적인 모델이며, 이 때 모플러 필터를 시간영역 또는 주파수영역에서 어떻게 구현하느냐
에 따라 변형된 방법들이 존재한다.
(1) Clarke/Gan 모델
Clarke/Gan 모델은 이동국 주위 Abeh scattering) 성분의 분포가 균일하고 각 Ab
의 전력이 동일하다는 가정하에서 각 도플러 천이에 대한 전력 밀도(도플러 스펙
유도한 Clarke/Gan 이론을 기반으로 Smith7} 고안한 모델이다[39]. 그림 2.8은 Smith7}
고안한 Clarke/Gan MES] 블록도를 보여준다. 주파수영역에서 BA Gaussian FSS 생
성하고 도플러 필터를 통과시켜 각 주파수 성분들이 도플러를 겪게한 후 이를 FFT 시킨
다. 여기서, IFFTS] 출력은 실수 신호가 되어야 하기 때문에, IFFTS] 입력은 반드시
Hermitian 대칭적으로 구성되어야 한다. 최종적으로 실수부와 허수부의 크기를 더해

Rayleigh 분포를 갖는 ASS 생성한다.

073



===== PAGE 73 =====
PART 1 _ 무선 채널 모델링과 MATLAB

Complex                    변태                                             h(t)
Gaussian                                        IFFT
Noise           그
h(t)= hy(t) + jholt)
(+)
28000
Complex                     LA                            ㅠ
Gaussian                                        \FFT
Noise           = 0
그림 2.8 Clarke/Gan 모델의 블록도
Clarke/Gan Model, fn=100[Hz], Ts=50[us]
5           T          T          ㅣ          T          T          ㅣ          T          T          T
0 |                                                                                                     4
-5 be
2
‘3 -10F
z
5 -15-
=
-2아                                                                                                     aI
—25F                                                                                                     |
-30           1          1          1          1          1          1          1          1          1
0        0.05       0.1       0.15       0.2      0.25       0.3       0.35       0.4       0.45       0.5
time [s]
(a) AS} 시간영역 특성
ai 104 Clarke/Gan Model, f,.=100[Hz], Ts=50[us]             ask to: Clarke/Gan Model, fn=100[Hz], Ts=50[us]
4b               로                                 4
3                    i                                    gist
=      |                                                   혼나                                                 |
가                                                                4
|
1 Lf                              |                                |       0.5+                                                                4
0     0.5      1      15      2     25     3     35      = -3    =2    =|      0      1      2     3      4
Occasions                                                  Occasions
(b) 크기 분포                                                (0) 위상 분포

그림 2.9 Clarke/Gan 모델로 생성된 채널의 특성

074



===== PAGE 74 =====
제2장_ 6150 채널 모델링

그림 2.9는 도플러 주파수가 /,, =100Hz°D 샘        기가 Ts=50usY 때,
Clarke/Gan BAS 생성된 주파수 비선택적 페이딩 채널의 시간영역 특성

림 2.9는 (a) 시간에 따른 채널의 크기 변화, (0) 큰기 분포, © 위상 분포
그림으로부터 채널의 크기가 시변 특성을 가지고, 37]= Rayleigh
(uniform) 분포를 갖는 것을 확인할 수 있다. 도플러 주파수가 air
빠르게 변하는데 이러한 경우 고속 페이딩(86 fading) 채널이 된다.

ave
au

N

a
&
도
{0
4
NX
NI

(1) 시간영역에서의 샘플 수(^, )를 결정한다. (프로그램 2.14(“00 『\004”)의 제 3행)

Sy 주파수(/, ) 및 최대 도플러 주파수(7, )를 고려하여 도플러 스펙트럼(45(/) )을

현하기 위한 샘플 Neer )와 IFFT 크기 Nie 를 결정한다. (프로그램 2.15(“FWGN”)
의 제 10, 11행)

(3) IFFT2] 입력을 Hermitian 대칭적으로 구성하기 위해 ^,,ㅠ개 샘플의 실수 Gaussian 잡음

을 생성한 RFPS 취함으로써 주파수영역에서 Neer 7 샘플의 Hermitian 대칭적인
Gaussian 잡음을 생성한다. (프로그램 2.15(“FWGN”)2] 제 13, 15행)

(4) 2224 2.16(“doppler_spectrum”)S 이용하여 ^,,ㅠ 개 샘플의 도플러 스펙트럼(4 9(/ ) )
을 생성한 후, 그 결과를 (3)에서 생성된 실수부와 허수부의 복소 Gaussian 잡음에 각각
곱한다. 도플러 필터의 ASL 주파수영역에서 대칭적이기 때문에, Hermitian 대칭적인
Gaussian 잡음과의 곱한 결과도 Hermitian 대칭적이다. (프로그램 2.15“FWGN”)2] 제
17, 19행)

(5) 실수부와 허수부에 대하여 각각 (22 )개의 BAS 삽입한 후 ^, 크기의 IFFT

를 수행한다. (프로그램 2.15('"\004”)의 제 22, 23, 24행)
(6) 실수부와 허수부를 결합하고 정규화시켜 평균 크기 및 전력이 1인 Rayleigh 페이딩 채널
을 생성한다. (프로그램 2.15FWGN”)2] 제 26, 28, 29행)

응 do_FWGN.m

clear, clf

scale=le-6; % mu

fm=100; % maximum doppler frquency

ts mu=50; ts=ts_mu*scale; % sampling time

fs=1/ts; % sampling frequency

075



===== PAGE 75 =====
PART 1 _무선 채널 모델링과 MATLAB

Nd=1e6; % the number of samples

* obtain the complex fading channel
(h,N££t,Nifft,doppler_coeff] = FWGN(fm, fs,Nd) ;
subplot (211), plot ([1:Nd] *ts,10*1lo0g10 (abs (h) ) )
str=sprintf('Clarke/Gan Model, f m=sd[Hz], T_s=
title(str), axis([0 0.5 -30 5])

subplot (223), hist (abs(h),50), subplot (224), hist (angle (h) , 50)

sd[us]',fm,ts_ mu);

fal 프로그램 214 FWGN 모델 실행 프로그램

function [h,Nfft,Nifft,doppler_coeff] =FWGN (fm, fs,N)
FWGN (Clarke/Gan) Model
Input

fm= maximum doppler frquency

fs= sampling frequency

N = number of samples

00 oP lO ol?

oe

% Output
* h = complex fading channel
Nfft = 2“max(3,nextpow2(2*fm/fs*N)); % Nfft=2*n

Nifft = ceil (Nfft*fs/(2*fm));

% Generate the inependent complex gaussian random process

GI = randn(1,Nfft); GQ = randn(1,Nfft);

© Take FFT of real signal in order to make hermitian symmetric

CGI = ££t (GI);       CGQ = ff£t (GQ);

% Nfft sample doppler spectrum generation

doppler_coeff = doppler _spectrum(fm,Nfft) ;

* Do the filtering of the gaussian random variables here

f_ CGI = CGI.*sqrt (doppler_coeff); £_CGQ = CGQ.*sqrt (doppler coeff) ;

* Adjust sample size to take IFFT by (Nifft-Nfft) sample zero-padding
Filtered_CGI=[f_CGI(1:Nfft/2) zeros(1,Nifft-Nfft) £_CGI (Nf£ft/2+1:Nfft)];
Filtered_CGQ=[f_CGQ(1:Nf£ft/2) zeros(1,Nifft-Nfft) f CGQ(Nfft/2+1:Nfft) ];
hI = ifft(Filtered_CGI); hQ= ifft(Filtered_CGQ) ;

* Take the magnitude squared of the I and Q components and add them
rayEnvelope = sqrt (abs(hI) .*2 + abs(hQ) .*2);

* Compute the root mean squared value and normalize the envelope

rayRMS = sqrt (mean (rayEnvelope(1:N) .*rayEnvelope(1:N)));

h = complex (real (hI (1:N)),-real(hQ(1:N))) /rayRMS;

!

| 프로그램 2.15 FWGN 모델 함수

(

076



===== PAGE 76 =====
제2장_6150 채널 모델링

function y=doppler_spectrum(fd,Nfft)

% fd=maximum doppler frequency

% N€ft=number of frequency domain points

df = 2*fd/Nfft; % frequency spacing

% DC component first

(1) = 0; y(1) = 1.5/(pi*fd) ;

% The other components for one side of the spectrum

for i = 2:Nfft/2,
f£(i)=(i-1)*d£; % frequency indices for polynomial fitting
y({i N££t-i+2]) = 1.5/(pi*fd*sqrt (1- (£ (i) /fd)*2));

end

Fh

% Nyquist frequency applied polynomial fitting using last 3 samples
nFitPoints=3 ; kk=[Nfft/2-nFitPoints:Nfft/2] ;

polyFreg = polyfit (f (kk) ,y(kk) ,nFitPoints) ;

y ((N££t/2)+1) = polyval (polyFreq, f (Nfft/2)+df£) ;

께 프로그램 216 도플러 스펙트럼의 생성 함수

(2) 수정된 주파수영역 FWGN 모델

1000080 모델은 주파수영역에서 효율적으로 도플러 필터를 구현할 수 있는 등 페이
딩 채널을 생성하기 위한 효과적인 방법이지만 를 두 번이나 사용하는 =8  연시
잡도가 큰 단점이 있다. 다양한 변형된 방법들이 존재하는데 본 절에서는 I-METRA
에서 사용하는 방법을 기술한다.

그림 2.10은 도플러 스펙트럼을 생성하는 방법을 보여준다. 그림 2.10(8)에 나타난 바와
같이 정상 샘플링의 경우에 Nyquist 주파수를 중심으로 반복되기 때문에 IFFT 함수가 양
의 주파수 성분만 Ale] etc} (MATLABS] “fit” 함수에 HSH) 이를 폴딩((010108)시켜야
한다. 반면, 그림 2.10(06)에서와 같이 Nos 만큼 오버샘플링할 경우에 도플러 대역폭은
By =2-Nos-f, 이 되며, 70006 변환으로 생성되는 시간영역 전체 Hols 채널의 길이
XL Trading =1/ Mfm 이 되며, 샘플링 WAL At =1/(2ㆍ^, ㆍ/,,) 이 된다. 그림 2.10(0)는
이산 주파수로 주어진 도플러 스펙트럼과 이산 시간으로 주어진 페이딩 ASS 보여준다.
이 때, 도플러 스펙트럼의 간격은 AF, =2-Nos Sn! Neading 2 주어지며, N Fading 은
IFFT 크기이다. 전체 도플러 대역폭 내에 존재하는 이산 주파수 샘플 수는
Ny =n! Mn = N raaing /(2*Nos) 로 주어진다. 이러한 도플러 스펙트럼 생성 방법을 A}



===== PAGE 77 =====
PART 1 _무선 채널 모델링과 MATLAB

— fra            0 ~fim=v/r                                                  9              Fm           200

(8) 정상 샘플링

Bp=2Nosfm                                           Vesa 11 Alig = 1 Bol Meare)

|                               7
1              |    Fourier Transform                              >|

f
0                개           Nosfm                    2Nostm                                            0

At =1/Bpy=1/(2N of.)

(b) 오버샘플링

Af n= ee Nrwding = 2Nosf ml N pading
= Asa riting                                 Drang= 1/ Af, = U(Bp/ 240)  |

           IFFT/FFT                                                 !

ml     lun. =        on

f
0      1                 - 1
Np= = Fin! Af mn =    Npading / (2Nos)

(0) 이산 시간 214
그림 2.10 도플러 스펙트

~

flu   1/Bp=1(2Nosfiny

m)

용할 경우에 주파수영역에서 최대 도플러 주파수를 고려하지 않고 일정 구간("8246 )의
페이딩 신호를 생성할 수 있으며, 시간영역에서 도플러 주파수에 따라 보간하여 사용할
수 있기 때문에 시뮬레이션이 용이한 장점이 있다. 즉, 생성하고자 하는 페이딩 채널의 샘
플 Nrading 과 페이딩 오버샘플링 인자 Nos 를 이용하여 전체 도플러 대역폭 내에 존재하
는 이산 주파수 샘플 수 7, 를 계산하고, 이를 이용하여 최대 도플러 주파수를 고려하지
않고 Nradng 개의 페이딩 채널 ASS 생성하고, 최대 도플러 주파수 /,에 따라 4/를

변화시켜 시뮬레이션에 사용한다.

_ 078



===== PAGE 78 =====
Al2a SISO 채널 모델

여기서 채널응답의 크기는 도플러 스펙트럼으로부터 계산되며, 위상은 임의의 위상을
가정한다. 이러한 경우에 시간영역에서 각 경로의 채널응답은 다음과 같이 주어진다.

N Fading 72그

10000 20140 0222                       (2.26)

k=- N Fading 12

여기서 SU) 이산주파수 *=/740에 의해 주어진 도플러 스펙트럼을 나타내며,
n=t/At* 이산화된 시간을 나타낸다. 또한 % 는 [0, 27) 구간 내에 균일한 분포를 갖
랜덤 변수이다. 이와 같이 도플러 필터에 균일한 AAS 첨가함으로써 08489180 분포으
랜덤 변수를 인가하는 (1800030 모델보다 시간영역에서 유연한 페이딩 곡선을 얻
있다. A] (2.26)에서 균일한 위상 대신에 HA Gaussian 랜덤 변수를 첨가한 경우에
한 페이딩 곡선을 얻기 위하여 저역 통과 필터링이 필요하다.

16 er

r2 4

29)
큰
으
그

인

bn)
ri
4N
fe
of

FWGN 모델에서 도플러 대역폭의 이산 주파수 샘플 수는
Np = Sy! Mn = N rating !(2* Nos) 가 정규화된 최대 도플러 주파수 역할을 수행하므로 도플러

천이 주파수 /, 은 생성된 페이딩 샘플 시간 At =1/ (2-Nos Sy) 을 결정할 때만 사용된다. (프

로그램 2.18(“8480_0 "의 마지막 행)

(1) 페이딩 파라미터 설정 : 페이딩 채널 VIS 위한 의 크기 Neading, 페이딩 오버샘플
링 인자 Nos, 다중경로의 Noam 입력받아 페이딩 파라미터를 설정한다. (프로그램
2.18(“fwgn_ff’)2] 제 16, 18, 20 행)

(2) 도플러 스펙트럼 생성 : 도플러 스펙트럼 타입에 따라 그림 2.10에서와 같은 방식으로 주파

수영역에서 스펙트럼을 생성하고 균일한 분포의 위상을 가한다. (프로그램 2.18(“0080 1")
의 제 21~41행) 도플러 스펙트럼의 타입이 Laplacian?! 경우에는 PAS(Power Azimuth
80600000)의 표준편차 o 2} DoM(Direction—of—Movement)2}+ 100ㅅ(121760000-01-ㅅ0181)
의 차 6가 추가로 입력되어야 한다. (프로그램 2.18(“6080_ 0 "의 제 28행)

(3) 각 경로의 정규화 : IFFT 의하여 생성된 각 경로의 시간영역 페이딩 신호를 평균전력이
1이 되도록 정규화한다. (프로그램 2.18(“8\80 ^”)의 제 42~45행)

079



===== PAGE 79 =====
Modified FW GN in Frequency Domain                                           Modified FW GN in Time Domain

g                                      g
8                                      8
“155                        —— Path 1, fm=100Hz |4        15                        —— Path 1, fr=100Hz |
— Path 2, fm=10Hz                                             —— Path 2, fm=10Hz
-20         ,        |        :        :                 -20
0     0.1     0.2     0.3    0.4     05       0     01     0.2     0.3    0.4    0.5
times [s]                                                         times [s]
(a) 수정된 주파수영역 FWON 채널 모델        (6) 수정된 시간영역 FWGN 채널 모델
그림 2.11 도플러 주파수가 다른 두 경로 채널
최근 보고된 채널환경의 측정결과를 보면, 채널환경에 따라 #4    한 도플러 스펙트럼을
보이며 심지어는 각 경로마다 최대 도플러 주파수 및 도플러 스펙트럼도 달라진다. 이러

한 AS 감안하여 프로그램 2.18(“8080_ "은 각 경로의 도플러 ㄴㄴ, 다를 경우에도
구현 가등하도록 작성되었는데, 이를 위해 각 경로의 최대 도플러 주파수(07 _12)가 함수
의 인수로 제공된다. 각 도플러 주파수는 최대 도플러 주파수로 정규화될 뿐만 아니라 다
Fe 도플러 스펙트럼을 ASS 수 있도록 ZS14 2.19(“DopplerPSD”)= 통해 다양한
스펙트럼 함수가 제공되며, 이 프로그램에 다른 스펙트럼 함수를 추가할 수도 있다.

프로그램 2.17(“00 0  ee  실행 결과 얻어진 그림 2.110)는
N rating =1024 , Nos       경우에 대해 두 경로의 최대 도플러 주파수가 각각 100Hz,
10032이고 그 도플러 peer Classical 모델로 설정된 AYO] 전력을 보여준다.

ㅇ
i“   a

% do_modified_ fwgn fading.m
clear, clf
Nfading=1024; % IFFT size for Npath x Nfading fading matrix

Nfosf=8;      * Fading oversampling factor
Npath=2;      * Number of paths
N=10000;

FadingType= 'class';

fm= [100 10]; % Doppler frequency

subplot (211)

[FadingMatrix ㄴㄴ] = fwgn_ff (Npath, fm,Nfading,Nfosf,FadingType) ;
size (FadingMatrix)

plot ([1:Nf£ading] *t£,10*1log10 (abs (FadingMatrix(1,:))),'k:!),hold on
plot ({1:Nfading] *t£,10*1l0g10 (abs (FadingMatrix(2,:))),'k-')

_ 080



===== PAGE 80 =====
제2장_ 8150 채널 모델링

title(['Modified FWGN in Frequency Domain, Nfading=',
num2str(Nfading) ,',Nfosf=',num2str(Nfosf)]);

xlabel('time[s]'), ylabel('Magnitude[dB]'),legend('Path 1,f m=100Hz',
‘Path 2, £ m=10Hz') ,axis([0 0.5 -20 10])

subplot (212)

[FadingMatrix tf]= fwgn_tf(Npath, fm,N,Nfading,Nfosf, FadingType) ;

plot ([1:N] *t£,10*1lo0g10 (abs (FadingMatrix(1,:))),'k:!), hold on

plot ([1:N] *t£,10*1log10 (abs (FadingMatrix(2,:))),'k-'), hold on
title(['Modified FWGN in Time Domain, Nfading=', num2str(Nfading),

| Nfosf=',numastr(Nfosf),',T s=',num2str(tf),'s']);
xlabel('time[s]'), ylabel('Magnitude[dB]'),legend('Path 1, £ m=100Hz',

‘Path 2, £ m=10Hz'),axis([0 0.5 -20 10])

Tl 프로그램 217 AME 주파수영역과 시간영역 WON 채널 모델 실행 프로그램

function [FadTime,tf]=fwgn_ff (Np, fm_Hz,Nfading,Nfosf,FadingType, varargin)
Fadng generation based on FWGN method in the frequency domain
FadTime= fwgn_ff(Np,fm_Hz,Nfading,Nfosf,FadingType, sigma, phi)

6 Inputs:

% Np        : number of multipaths

6 fm 82     : a vector of max. Doppler frequency of each path [Hz]

% Nfading   : Doppler filter size (IFFT size)

* Nfosf     : oversampling factor of Doppler bandwith

* FadingType: Doppler type, 'laplacian'/'class'/'flat'

% sigma     : angle spread of UE in case of 'laplacian' Doppler type
6 phi       : DoM-AoA in case of 'laplacian' Doppler type

% Output:

6 FadTime   : Np x Nfading, fading time matrix

fmax_Hz= max(fm_Hz) ;

% Doppler frequency spacing respect to maximal Doppler frequency
dfmax= 2*Nfosf*fmax_Hz/Nfading;

* Obtain a funtion corresponding to Doppler spectrum of "FadingType"
ftn_psd= DopplerPSD (FadingType) ;

err_msg= 'The difference between max/min Doppler frequencies is too
large.\n increase the IFFT size';

if isscalar(fm_Hz), fm_Hz= fm _Hz*ones(1,Np); end
if stremp (lower (FadingType(1:3)),'lap') % Laplacian constrained PAS
for i=1:Np

081



===== PAGE 81 =====
PART ｌ 무선 tHe 모델링과 MATLAB

Nd=floor (fm_Hz(i)/dfmax)-1; ¢ Nd=fm_ Hz/dfmax=Nfading/ (2*Nfosf)
if Nd<l, error(err_msg); end
tmp= ftn_psd([-Nd:Nd] /Nd, varargin{1}(i),varargin{2}(i));
tmpz= zeros (1,Nfading-2*Nd+1) ;
FadFreq(i,:)= [tmp(Nd+1:end-1) tmpz tmp(2:Nd)];
end
else % symmetric Doppler spectrum
for i=12Np
Nd= floor (fm_Hz(i) /dfmax) -1;
if Nd<l, error(err_msg); end
tmp= ftn_psd([0:Nd]/Nd); tmpz= zeros(1,Nfading-2*Nd+3) ;
FadFreq(i,:)= [tmp(1:Nd-1) tmpz fliplr(tmp(2:Nd-1))];
end
end
% Add a random phase to the Doppler spectrum
FadFreq = sqrt (FadFreq) .*exp(2*pi*j*rand(Np,Nfading) ) ;
FadTime = ifft (FadFreq,Nfading, 2) ;
FadTime=FadTime. /sqrt (mean (abs (FadTime) .*2,2) *ones(1,size(FadTime, 2) )
); % Normalize to 1
tf=1/(2*fmax_Hz*Nfosf) ; tfading sample time=1/ (Doppler BW*Nfosf)

@ 프로그램 218 수정된 주파수영역 EWEN 채널 모델 함수

function ftn=DopplerPSD (type)
Doppler spectrum funtion for type =

‘flat!     : S(£)=1,  |£0(=£/£m) |< 1
'class'    : S(£)=A/ (sqrt (1-£0.*2)), |£0|<1 (A: a real number)
‘laplacian':

S(£)=1./sqrt (1-£0.*2) .* (exp (-sqrt (2) /sigma*abs (acos (£0) -phi) )
+exp (-sqrt (2) /sigma*abs (2008 (f0) -phi) ) )
with sigma(anglé spread of UE) and phi (=DoM-AoA)
in the case of 'laplacian' Doppler type
‘sui!     : S(£)=0.785*£0.*4-1.72*£0.*24+1, |f£0]<1
'3gpprice' : S(£)=0.41./(2*pi*fm*sqrt (1+1le-9-
(£./fm) .*2))+0.91*delta ftn(£,0.7*fm), |£|<fm
‘dr', S(£)=inline(' (1./sqrt (2*pi*Dsp/2) ) *exp(- ( (£-
Deh) . 2) /Dsp) ',"£', "Dep", 'Dsh') ;
f0 : normalized Doppler frequency defined as f0=f/fm

HAP AP AP 00 AP WP AHP AP _ 00 _ 00 AP HP oP 00 ㅇㅇ

fm: maximum Doppler frequency

062



===== PAGE 82 =====
제2장_ 6150 채널 모델링

switch lower (type (1:2) )

case 'f1', ftn=inline('ones(1,length(f£0))');

case 'cl', ftn=inline('1./sqrt (1+1le-9-f£0.*2)');

case 'la', ftn=inline(' (exp (-sqrt (2) /sigma*abs (2008 (f0) -phi) )+exp
(-sqrt (2) /sigma*abs (acos(£0)+phi))) ./sqrt (1+1e-9-£0.*2)','
£0’, ‘signa’ , 9113 ' ) ;

case 'su', ftn=inline('0.785*f£0.*4-1.72*f£0.*2+1.');

case '3g', ftn=inline('0.41./(2*pi*fm*sqrt (1+1le-9-(£./fm) .*2))+0.91*
delta a  0.7*101「,넷1, 100"),

case 'dr', ftn=inline('(1./sqrt (2*pi*Dsp/2) ) *exp(-((f-Dsh) .“2)/Dsp) '
내 "Dep", "Dsh");

otherwise, error('Unknown Doppler type in DopplerPSD()');

end

수

Olt

를! 프로그램 219 도플러 스펙트럼 생성

0

(3) 시간영역 FWGN 모델
전술한 주파수영역 방식과 달리 시간영역 FWGN BAS 그림 2.12에서는 도플러 스펙
ERO) 주파수 응답에 해당하는 시간영역 필터의 계수를 구한 후 BA Gaussian 랜덤 Al

SS 필터링하는 방식이다. 이러한 시간영역 FWGN BAS 다양한 장점이 있어 상용 페
이딩 채널 시뮬레이터의 생성 방식으로 널리 이용된다.

Complex            0080            Fadi

Gaussian        aaa

Generator

그림 212 시간영역 FWGN 모델의 블록도

주파수영역 FWGN 모델에서는 페이딩 채널의 구간이 WPT 크기인 "^ 과 주파수영
오버샘플링 인자 Nos ol] 의하여 결정되지만, 시간영역 FWGN 모델에서는 도플러 필터
입력인 복소 Gaussian HE AS) 길이에 의하여 결정되는 장점이 있다. 즉, 필터링되
#A Gaussian 랜덤 신호의 수를 증가시킴으로써 시뮬레이션 구간을 확장할 수 el
그러나, FIR 구조를 =  “ 인 경우   a    = a a 길어지면 언산량0

flr to 48

083



===== PAGE 83 =====
PART Ｌ 무선 채널 모델링과 MATLAB

구조의 필터는 안정성을 보장할 수 없기 때문에 FIR 구조의 필터가 많이 사용된다. FIR
구조의 필터를 사용하는 경우 지정된 is ieee llndie   0" 필터링하여 페이딩
채널을 생성하고 이를 사용함으로써 실시간 처리 시 계산량을 감소할 수 있다.

전술한 바와 같이 FWGN 채널 모델링 기법은 1.3절에서 ee 도플러 스펙트럼 이외
에 다양한 도플러 스펙트럼을 쉽게 ASS 수 있다. 가장 널리 사용되는 18891081 모델 외
에 티 도플러 스펙트럼과 18010102 도플러 스펙트럼 So] 있다. Flat 도플러 스펙트럼은
다음과 같이 정의된다.

S(f) «1,             IF ESe                                       (2.27)

또한, Laplacian 도플러 스펙트럼은 다음과 같이 정의된다.

oO

rlo

Oe

on'( J, )+4)}   IIS S,

| exp} -
(YJ                                                (2.28)
여기서 c= PASS) 표준편차를 나타내며, 는 DoMi} DoAL] 차를 의미한다. Laplacian
도플러 스펙트럼은 기존의 Flat LE Classical 도플러 스펙트럼과 달리 이동국의 이동 방
향을 고려할 수 있는 특징이 있다. 위의 도플러 AMSA 최종적으로 정규화 과정을
거치기 때문에 절대적인 크기는 의미가 없고 각 주파수에 따른 전력차가 중요한 요소이다.

주        _ MATLAB 프로그램 : 시간영역 FWGN 채널 모델         2

프로그램 2.20“fwgn tP)2 각 경로의 시간영역 도플러 필터 계수(610를 구해주는 프로그
램 2.21(“gen_filter”)2}] 제 20행에서 프로그램 2. 이 igi   사용하여 주어진 type]
도플러 스펙트럼 함수를 구성함으로써 그림 2.1106)의 결과를 얻는다. 이 때 그 두 번째 입력
ele] fm Hes MYR 넣어좀으로써 각 정로의 최대 도플러 IAS 서로 다르게 설정할
수 있고, 그것이 스칼라로 주어지는 경우에는 모든 경로에 똑같은 최대 도플러 주파수가 설정
된다(제 15행). 다음으로 “860 111@'의 결과로 주어지는 필터 계수를 사용하여 복소 Gaussian
랜덤 ASS 필터링한다(제 19행). 여기서 필터링은 “8101 함수를 사용하여 이루어지는데, 이
001 함수는 FFTS 이용하여 FIR 필터를 구현하는 060480060-800 방식을 프로그래밍한

LS ‘filter’ 2 동일한 결과를 출력하지만 보다 효율적으로 필터링한다.

084


===== PAGE 84 =====
제2장 9150 채널 모델링

function [FadMtx,tf]=fwgn_tf (Np, fm_Hz,N,M,Nfosf,type, varargin)

* fading generation using FWGN with fitering in the time domain

% Inputs:

% Np      : number of multipaths

« fm Hz : a vector of maximum Doppler frequency of each path[Hz]
6 N      : number of independent random realizations

6 M       : length of Doppler filter, i.e, size of IFFT

6 Nfosf : fading oversampling factor

6 type    : doppler spectrum type

용     'flat'=flat, 'class'=calssical, 'sui'=spectrum of SUI channel
%     '3gpprice'=rice spectrum of 3GPP

6 Outputs:

%      FadMtx : Np x N fading matrix

if isscalar(fm_Hz), fm_Hz= fm_Hz*ones(1,Np); end
fmax= max (fm_Hz) ;
path_wgn= sqrt (1/2) *complex(randn(Np,N) ,randn(Np,N)) ;

for p=1:Np
filt=gen_filter(fm_Hz(p),fmax,M,Nfosf,type,varargin{ : } ) ;
path(p,:)=fftfilt (filt, [path wgn(p,:) zeros(1,M)]); %filtering WGN
end

FadMtx= path(:,M/2+1:end-M/2) ;
tf=1/(2*fmax*Nfosf); ¢ fading sample time=1/ (Max. Doppler BW*Nfosf)
FadMtx= FadMtx./sqrt (mean (abs (FadMtx) .*2,2) *ones(1,size(FadMtx,2)));

ll 프로그램 2.20 시간영역 FWGN 채널 모델 함수

function filt=gen_filter(fm_Hz,fmax_Hz,Nfading,Nfosf, 0706 , varargin)
FIR filter weights generation

% Inputs:

%   Nfading : Doppler filter size, i.e, IFFT size

6 Outputs:

%   116    : filter coefficients

% Doppler BW= 2*fm*Nfosf ==> 2*fmax Hz*Nfosf

dfmax= 2*Nfosf*fmax_Hz/Nfading;     % Doppler frequency spacing

6 respect to maximal Doppler frequency

Nd= floor (fm_Hz/dfmax) -1;

if Nd<1, error('The difference between max/min Doppler frequencies is too
large.\n increase the IFFT 8126?! ) ;

end

085 _



===== PAGE 85 =====
PART 1_ FM 채널 모델링과 MATLAB

ftn_psd=DopplerPSD (type) ; *funtion corresponding to Doppler 'type'
switch lower(type(1:2))
case '3g', PSD=ftn_psd([-Nd:Nd] ,Nd) ;
filt=[PSD(Nd+1:end-1) zeros(1,Nfading-2*Nd+1) PSD(2:Nd)];
case 'la', PSD=ftn_psd([-Nd:Nd] /Nd, varargin{:});
filt=[PSD(Nd+1:end-1) zeros(1,Nfading-2*Nd+1) PSD(2:Nd)];
otherwise, PSD=ftn_psd([0:Nd] /Nd) ;
filt=[PSD(1:end-1) zeros (1,Nfading-2*Nd+3)
PSD(end-1:-1:2)]; % constructs a symmetric Doppler spectrum
end
filt=real (ifftshift (ifft (sqrt (filt))));
filt=filt/sqrt (sum(filt.*2));

Tal

fal 프로그램 2.21 FIR 필터 계수 발생

oo
+

Rayleigh 페이딩 ABS 복소 Watt complex sinusoids\S 결합하여 생성할 수 …
여기서 더해지는 정현파의 수는 발생된 채널의 크기에 대한 확률 27} Rayleigh 분
근사화될 수 있도록 충분히 많아야 한다. 또한, 요구되는 도플러 스펙트럼을 정확히 ui
할 수 있도록 정현파 발생기에 가중치가 가해진다. 이 채널 BAS 2.3.1절에서 7] Set
Clarkeo]] 의해 제안된 등방성 산란 1 al(isotropic scattering 10100861)에 기반을 두고 Jakes
가 제안한 채널 모델이다[26]. Jakes 모델은 하드웨어 시뮬레이터를 위해 개발되었으나 구
현이 간단하기 때문에 소프트웨어 시뮬레이션에 널리 이용되고 있다.

그림 2.13은 Jakes DAS] 구현 방법을 나타낸다. 이 BAAS 산란성분의 등방성 연
속체가 공간상에 균일한 방위각으로 도달하는 개의 평면파로 근사화된다. JakesE
^/2 를 홀수로 제한하였으며, 새로운 정수 N, =(N/2-1)/2 를 정의하였다. Jakes 모델은
그림 2.13에 나타난 바와 같이 w, = 287, 의 주파수를 지닌 하나의 복소 발진기에 도플러
천이된 정현파의 주파수 (4, =14, 0050, ) Ny 개의 복소 발진기의 BS 더한 형태로 모델
링 된다. 여기서 6, 는 7 번째 평면파의 도달각을 의미하며, 4=1, 2, …, #, 이다. 결과적
으로 Jakes 로릴어서: 복소 채널은 다음과 같이 표현된다.

E
h(t) =—_——(h     ih
0)    ON, + 7S / (t)+ jhg(t))                      (2.29)

086



===== PAGE 86 =====
제2장 8150 채널 모델링

20080, cos (wy,t)

cos by, 1 008 (wy, it)

20060, cos (wt)

2008 dy cos (0071)
& v2sindy cos (wyt)

2sing, cos (w,t)

OO OC.OO

fm. 008 (27aN,/N) f,,008(27aN,/N) fin

2singN, cos (wy, t)

6
Q
&
그림 213 Jakes 모델의 구현 방법

여기서 &,은 페이딩 채널의 평균 크기를 의미하며, 40) 와 %,(0) 는 다음과 같이 주어
진다.

No
h,(t)=2)°(cos@, cos w,t)+V2 cos@ y cos w,t

es                                                                              (2.30)
h(t) =2>° (sing, cosw,t)+V2 sing y cos w,t

n=l

여기서 Qt Pvt 각각 nwa] 도플러 천이된 정현파의 초기 위상과 최대 도플러 주파수
(//)의 초기 위상을 나타낸다. 페이딩 채널의 위상이 균일한 분포(0011007 distribution)S
가지도록 초기 위상이 설정되어야 하며, 이를 위하여 Jakes= 초기 HAS 설정하는 두 가
지 방법을 제안하였다. 여기서는 두 번째 방법을 이용하여 초기 위상을 다음과 같이 설정
한다[26].

py =0

PET
¢, =ani(N, +),       n=l, 2,-,N,             (00012

087



===== PAGE 87 =====
PART 1 _무선 채널 모델링과 MATLAB

Jakes Model, fy=926Hz, T==1e-006s

Magnitude[dB]

“205     0005 0.01  0.015 0.02 0.025 0.03
times[s]
(a) 채널의 시간영역 특성
Jakes Model, fg=926Hz, T,=1e-006s                                    Jakes Model, fa=926Hz, T,=1e-006s
3000     +     +     ;     -     1        1500     T     T     1     T     1
2500+     rr                 ;           hy     |        ：
20005    |    |               4+ 1000+        m 귀비 Gath 걱
8 150아 8
fa)                                    이                       |
100아                              4    500+                              4
500+                              4
0                                    0
0    0.5    1    15    2    2.5    3     =4 -3   =e  =]   0   1    2   3   4
Magnitude                               Phase[rad]
(b) 크기 BE                         (0) 위상 BE
Autocorrelation, fs=926Hz                                              Doppler Spectrum, fy=926Hz
14    ;   |   ;   '   {   ;      600   도
'       {       |       '       ;       | |— Classical                                                                  sical
14 「         Li tL Simulation                                     — Simulation
10000 00i      0000
을 08 |      ee
은      i              |
ㅎ 06    로---~-            그

nanan

15 2 25 3 35 4 45 “…1 00-06-04-02 0 02 04 06 08 1

은 은
ine}  a

:

|

{

{

|

0   5                          z
delay [s]                   x 10°                                      f/fy
(0) 자기 상관 특성                     (8) 도플러 스펙트럼

그림 2.14 Jakes 모델로 생성된 채널의 특성



===== PAGE 88 =====
체2장_ SISO 채널 모델링

식 (2.30)에서 도플러 천이된 정현파의 주파수는 "는 다음과 같이 다시 쓸 수 있다
w, = 14, 0060, = w, 009(2272 7 N),           n=l, 2,---,N,              (2.32)

도플러 천이된 정현파의 수는 모델링된 Holy 채널의 크기(|40)|)가 Rayleigh 분포에
근사하도록 충분히 많이 설정해야 하는데 일반적으로 ^, =8이면 모델링이 잘 되는 것으

로 알려져 있다.
위와 같은 방법으로 모델링된 Jakes 모델의 특성은 다음과 같다.

2                            2
E| ()|=E                                               (2.34)

E[h(t)| = E,                                                 (2.35)

E| h, (t)hy(t) |=0                                             (2.36)

Al (2.33)에서 식 (2.36)로부터 확인할 수 있듯이, 생성된 채널의 평균 크기는 {이고
채널의 평균 ABS 이다. 또한, 실수부와 허수부의 평균 전력은 각각 22 /2이고, 서로
독립적이다.

그림 2.14는 프로그램 2.22(“00 18169 Flat’)S 실행시켜서 얻어진 것으로서, Jakes 모
델로 생성된 50,000 샘플의 페이딩 채널의 특성, 즉 시간에 따른 크기 변화, 크기 분포, 위

상 분포, 시간영역 상관 특성, 주파수영역 전력 밀도를 보여준다.

* do Jakes Flat.m
clear all, close all
6 initial parameter

£d=926;    * Doppler frequency
Ts=le-6; % Sampling time
M=2*12;

t=[0:M-1]*Ts;

f=[-M/2:M/2-1] / (M*Ts*£d) ;

089


===== PAGE 89 =====
14
fu

31

PART |_ 무선 채널 모델링과 MATLAB

W
이

Ns=50000;
t_state=0;
% channel generation
[h,t_state]=Jakes Flat (fd,Ts,Ns,t_state,1,0);
subplot (311), plot ([1:Ns]*Ts,10*logl0(abs(h))),
title(['Jakes Model, f d=',num2str(fd),'Hz, T_s=',num2str(Ts),'s'])j;
axis([0 0.05 -20 10]), xlabel('time[s]'), ylabel('Magnitude [dB] ')
subplot (323), hist (abs (h) ,50);
title(['Jakes Model, f_d=',num2str(fd),'Hz, T_s=',num2str(Ts),'s']);
xlabel('Magnitude'), ylabel('Occasions')
subplot (324), hist (angle (h) , 50) ;
title(['Jakes Model, f d=',num2str(fd),'Hz, T_s=',num2str(Ts),'s']);
xlabel('Phase[rad]'), ylabel('Occasions')
% Autocorrelation of channel
temp=zeros (2,Ns) ;
for i=1:Ns

for j=1:Ns

temp (1,j-i+1)=temp(1,j-i+1)+conj (h(i)) *h(j);
temp (2,}-i+1)=temp(2,j-1i+1) +1;

end
end
for k=1:M

Simulated_corr(k) =real (temp (1,k) ) /temp(2,k) ;
end
Classical _corr=besselj (0,2*pi*fd*t) ;
% Fourier transform of autocorrelation
Classical _Y=fftshift (fft (Classical_corr) ) ;
Simulated_Y=fftshift (fft (Simulated_corr) ) ;
subplot (325)
plot (t,abs(Classical_corr),'b:', t,abs(Simulated_corr), 'r:')
title(['Autocorrelation, f d=',num2str(fd),'Hz'])
grid on, xlabel('delay \tau [s]'), ylabel('Correlation')
legend('Classical', 'Simulation')
subplot (326)
plot (f£,abs (Classical _Y),'b:', £,abs(Simulated_Y),'r:')
title(['Doppler Spectrum, f d=',num2str(fd),'Hz'])
axis([-1 1 0 600]), xlabel('f/f_d'), ylabel('Magnitude')
legend('Classical', 'Simulation')

Tl 프로그램 222 Jakes 모델 실행 프로그램

090



===== PAGE 90 =====
제2장 6150 채널 모델링

function [h,tf]=Jakes Flat (fd,Ts,Ns,t0,E0,phi_N)

* Inputs:

s fd,Ts,Ns : Doppler frequency, sampling time, number of samples
6 t0, EO : initial time, channel power

6 phi _N    : inital phase of the maximum doppler frequency sinusoid
% Outputs:

* hh, tf    : complex fading vector, current time

if nargin<é, phi N=0;   end

if nargin<5, E0Q=1;       end

if nargin<4, t0=0;      end

NO = 8;               * As suggested by Jakes

N = 4*N0+2;           6 an accurate approximation

wd = 2*pi*fd;         6 maximum doppler frequency [rad]

= t0+[0:Ns-1]*Ts; tf = t(end)+Ts;
coswt=[sqrt (2) *cos(wd*t) ; 2*cos (wd*cos(2*pi/N*[1:NO]')*t)]; % 4 (2.32)
h = E0/sqrt (2*N0+1) *exp(j* [phi 과 pi/(N0+1) *[1:N0]]) *coswt;

\

fm) 프로그램 2.23 Jakes 모델 함수

GR Ray 기반 Bag 기법

Ray 기반 BAS 시간 상관과 공간 상관 사이의 연관성을 고려하여 동시에 구현할 수
있는 장점이 있어 MIMO 채널 모델링에 많이 이용되고 있다[40]. Ray 모델은 5150에서
도 사용될 수 있기 때문에 본 절에서는 Ray 모델의 기본적인 윈리를 설명하고 3장에서
Ray 모델을 MIMO 채널로 확장한다.

Ray 기반의 BAS 기본적으로 Jakes 모델처럼 입사되는 평면파의 합으로 모델링된다.
Ray 기반 모델에서는 그림 2.15에 나타난 바와 같이 단말기 주위에 균일한 간격으로 배치
된 평면파를 고려하지만, 평면파가 균일하게 배치될 필요가 없이 임의의 간격으로 임의의
위치에 배치될 수 있어 다양한 산란(60846008) 환경을 모델링할 수 있다. 이로 인하여
PAS(Power Azimuth Spectrum)7} 균일하지 않으며 도플러 스펙트럼도 Jakes 모델에서
사용한 U-EY(Classical)o] 아닌 주어진 산란 환경에 따라 다양하게 HAS 수 있다.

091



===== PAGE 91 =====
_ 092

PART 1

_ 무선 채널 모델링과 MATLAB

ㅠ azimuth

-x 0 Nea    7 azimuth

Aoi
Broadside
Mean AoA
Endfire
t                                                                                t
Doppler
spectrum

1 Normalized

-1           1 Normalized
frequency                        frequency
(a) Jakes 모델

06) Ray 기반 모델
그림 2.15 Jakes 모델과 Ray 기반 모델의 차이

BS array

8p, AoD                                                                            \
mm 40D WAS array broadside                |    MS array
Ose
‘\                    2                      ‘                                              MS directi
                                                  BS array broadside                          of ae
I

번
=

그림 216 Ray 기반의 MIMO 채널 모델링 기
그림 2.162 30#『에서 MIMO 채널 모델로 사용하는 Ray 기반 SCM(Spatial Channel
Model) 모델링 기법의 ARS 보여준다. MIMO 채널의 경우에 6번째 송신 안테나와 wl

Al 수신 안테나 사이의 7번째 경로의 채널 4,』,(0) 2 다음과 같이 주어진다.

Gos (A xmncatop ) exp(j [ kd, sin (nto ) 때 0. ] x
P         M
h,,,() =   |   oe eo     @ (9, 1.404) exp(jkd, sin (8, 404 ))x
m=1
exp (ik ||v|| cos a  -0  )t)

v

(2.37)


===== PAGE 92 =====
제2장_ 6150 채널 모델링

SISO 채널의 경우에는 공간 상관은 존재하지 않으며 시간 상관만 존재하기 때문에 위
식에서 도플러 스펙트럼만이 의미가 있다. 식 (2.37)의 SCM MIMO 채널 모델에 대해서
는 3장에서 자세히 설명하며, 본 절에서는 Ray 기반 SISO 채널 모델에 대해서만 설명한
다. SISO 채널 BAS 생성하기 위하여 식 (2.37)에서 공간 상관을 형성하는 파라미터들
을 제거하고 108-10ㅁ00011 shadow 페이딩의 크기 Oy, 을 생략하면, SISO 채널 모델 4,(7)
은 다음과 같이 주어진다.

P<    .       .22
h(t)=   ZS (cx0 (10,4) xe00{ 1 Flies (xno -4,))            (2.38)
m=1

여기서 P= 7번째 경로의 전력이고, MS 경로당 AA] subray2] 수이다. 또한, ®,,,,
와 0,,.,/ 는 각각 7번째 경로의 7, 번째 subray2] 랜덤 위상과 수신단에서 수신되는 Al
호의 AoAS 의미한다.

Ray 기반 모델에서는 248에 따라 적절하게 각 subray2] 각도와 전력을 할당함으로써
주어진 PASS 갖는 채널을 생성한다. 각 subray2] 각도와 전력을 할당하는 방법은 SCM
^186에 Motorola7} 제안하여 채택된 동일 전력 subray 방식과 *00히에서 제안한 이산화
된 Laplacian 방식으로 크게 나눌 수 있다. 식 (2.37)과 Al (2.38)은 동일 AA subray 방
AS 사용한 채널 모델이다.

(1) 동일 전력 Subray 방식

동일 AF subray 방식은 각 64018》의 전력을 동일하게 할당하고 subray2] 각도를 비균
일하게 배열함으로써 PASS 구현하는 방식이다. 동일 전력 94618 방식은 VE subrayS|
전력이 동일하기 때문에 쉽게 시공간 상관을 구할 수 있는 장점이 있으며, 모델링 과정에
서도 많은 부분이 단순화되는 장점이 있다. 22 개의 subrayol] 대해서 각 subray2] 각도를
결정하는 방법은 그림 2.17에 나타난 바와 같이 44 개의 94608》에 의하여 나뉘어지는
PAS 상의 면적이 1/ (47+ 1)이 되도록 설정한다. 본 절에서는 48018080 PASS] 경우를
예로 들어 설명한다. 이러한 경우에 두 subray 사이의 WAS 다음과 같이 구할 수 있다.

a,        &    -4210       -12161|  -12161     1
P(O0,0)d0=     6?" d@=--\|e % -e % |=            2.39
J —  Ip                a(M +1)    a



===== PAGE 93 =====
PART 1 무선 채널 모델링과 MATLAB

여기서 2(0, 0)는 평균 AoA7} 0인 Laplacian PASS 나타내며, ㅇ는 rms AS(Angle
Spread)S 나타낸다. 식 (2.39)에서 74 이 홀수이면, 가장 작은 각도의 절대값은 0" 이고
HE subrayo] 대하여 6=1이다. 4 이 짝수이면, 절대값이 가장 작은 두 대칭 각도에 대
해서는 6=2이고 다른 BE subrayol] 대해서는 6=1이다.

Integrated power

Laplacian PAS
in each section

Two sub-ray example

-V26,
oy    로   2,        M
6,,,, [deg] =-—=] In}e * -——— ||, 0<m<— and 6, = 0"   3,
ni Ldeg]  + | .   aol    m<--and 6     (2.40)

여기서 MO] 짝수인 경우에는, 0, =O 초기값으로 하여 가장 작은 각도 0,을 구하고
0, =0“에는 실제 4608가 할당되지 않는다. 반면에 Wo] 홀수인 경우에는, 0, =0“에

단지 하나의 가장 작은 각도의 subray7} 존재하고 대칭 음의 각도에 subray7} 할당된다.

Equal Power Subray : Laplacian o =1°, M=20

1.5
얼 나는@     ' or   4
2             '  1
[이             {
             |
PO on one ane| |    i
0  1  1  i  4    ‘  |  {  '
=5 <4 -8 -2 -I  0  il  2 3 4 5

Angle of Arrival [deg]

그림 2.18 동일 전력 subray 방식에서 옵셋각 할당 방식의 of

_ 094



===== PAGE 94 =====
그림 2.18은 ㅇ=1“이고, M=20% 때 식 (2.40)에 의해 생성된 옵셋각을 나타낸다. 또한
표 2.2는 SCM AYA 사용되는 옵셋각을 보여준다.

~

22 661에서  사용되는 옵셋각

12      10 0894   이주 이이    0 11 5640

8, 4          구0.2826           +0,7064           +4,9447
5, 6         +0,4984           41,2461           +8,7224
1,8         +0,7431          41,8578           +13,0045
9 10         +£1,0257          +2,5642           +17,9492
11, 12         +1,3594          +3,3986          +£23,7899
18, 14         +1,7688          #£4,4220          +30,9538
15, 16         +2,2961          +£0,7403          + 40,1824
LT 18         +3,0389          +£7,5974           +53,1816
19, 20         +4, 3101          +10,7753          +£75,4274

(2) 이산화된 Laplacian 방식

동일 AZ subray2] 경우에 각 subray2] 전력이 동일하고 옵셋각이 비균
이산화된(68000160) Laplacian 방식은 그림 2.19에 나타난 바와 같이 각 전력은 Laplacian
PASS 따르며 평균 AAS SALE 비대칭적인 BAAS 갖는다. 생성 방법은 먼저 평
균 ^04&를 중심으로 [-a, a] 범위에서 6=20/4 의 등간격으로 균일하게 분포되도록
옵셋각을 할당한다. 예를 SO] o =2°, 5°, 35° 경우에 at 각각 10°, 15°, 179°] tf. 다음
으로 [-0.5, 0.5] 범위 내의 임의의 각도가 추가한 후, 각 옵셋각에 subrayS 할당한다. 다
음 식은 이산화된 [80180 방식에서 옵셋각 할당 방법을 보여준다.

주

6, =-a+m-6+¢,    m=0,1---,M-1            (2.41)

여기서 #는 [-0.5, 0.5] 구간에서 균일한 BES 갖는 랜덤 변수이다.

095


===== PAGE 95 =====
PART |_ FM 채널 모델링과 MATLAB

Random
| selection

30 25 6

그림 2.19 이산화된 Laplacian 기법에서 옵셋각 할당 방법

본 절에서는 동일 AS subray 기반의 ray BAS 생성하는 프로그램 2.24(“tya_ fading
165『"에 관해 설명한다. 식 (2.38)에서 확인할 수 있듯이 SISO] 경우에는 단지 이동국 subray
의 옵셋각만 필요하지만, 3장에 기술된 MIMO 채널 모델과 호환성을 유지하기 위하여 기지국
의 파라미터를 설정한다. 만일 이 부분이 필요없다면, “een 10056" 함수에서 기지국 ADE
생성하는 부분을 제거하면 된다.

(1) 페이딩 파라미터 설정 : 프로그램 2.26(“gen_phase”)S 사용하여 채널 지연 확산, 기지국
의 ASS} AoD, 이동국의 ASS AoA, 이동국의 이동 SES 이동 방향을 입력받아 페이딩
파라미터를 설정한다. (2214 2.24(“rya_fading 1680”)의 제 17, 18행)

(2) Subray 전력 및 옵셋각 할당 : 프로그램 2.27(“assignoffset”)S 사용하여 48에 따라 이
동국과 기지국에서 subray2] 옵셋각을 할당한다. 여기서 HE subray2] 전력은 1/M 이며,
채널의 상관 SYS 개선하기 위하여 이동국과 기지국 사이의 subrayS 랜덤하게 짝짓는
다. (프로그램 2.26(“gen_phase”)2}] 19~23행)

(3) 채널 계수 생성 : 프로그램 2.31('87 180108”)을 사용하여 74 개의 subray2] 위상을 결합
함으로써 각 경로의 복소 채널 Ales 생성한다. (프로그램 2.24 (“78 130108 test”)2] 제
22행)

으

* ray_fading test.m

clear, clf

fc=900e6; fs=5e4; speed_kmh=120; Ts=1/fs;
v_ms= speed_kmh/3.6; wl_m= 3e8/fc;

096



===== PAGE 96 =====
제2장_ 68150 채널 모델링

[J

% channel parameters setting: SCM case 2
PDP dB=[0. =1. =9. -10. -15. -20]; t_ns=[0 310 710 1090 1730 2510];

BS theta_LOS deg=0;      MS_theta_LOS deg=0;

BS AS deg=2;                    % Laplacian PAS

BS 200 deg=50*ones (size (PDP_dB) ) ;

119 29 deg=35;                   % for Lapalcian PAS

DoT deg=22.5; MS AoA _deg=67.5*ones(size(PDP_dB)) ;

6 generates phase of a subray

[BS theta_deg,MS theta_deg,BS PHI rad]=gen_phase(BS theta_LOS deg,
BS AS deg,BS AoD deg,MS theta_LOS deg,MS AS deg,MS AoA deg) ;
PDP=dB2w(PDP_dB) ;

% generates coefficients

t= [0:le4-1]*Ts;

h= ray_fading(20,PDP,BS PHI _rad,MS_theta_deg,v_ms,DoT_deg,wl_m,t) ;
plot (t,10*1log10 (abs (h(1,:))))

title(['Ray Channel Model, f c=',num2str(fc),'Hz,T_s=',num2str(Ts),'s']);
xlabel('time[s]'), ylabel ('Magnitude [dB] ')

께! 프로그램 2.24 Ray 기반 채널 모델 실행 프로그램

function theta=equalpower_subray_table(AS deg)
Obtain angle spacing for equal power Laplacian PAS in SCM Text

6 Input:
%   AS deg: angle spread with valid values of 2,5(for BS) ,35(for MS)
% Output:
6   theta : offset angle with M=20
if AS deg==2
theta=[0.0894 0.2826 0.4984 0.7431 1.0257 1.3594 1.7688 2.2961 3.0389

434,00) ;
elseif AS deg==5
theta=[0.2236 0.7064 1.2461 1.8578 2.5642 3.3986 4.4220 5.7403 7.5974
10.7753) ;
elseif AS deg==35
theta=[1.5649 4.9447 8.7224 13.0045 17.9492 23.7899 30.9538 40.1824
53.1816 75.4274];
else error('Not support AS');
end

게 프로그램 225 동일 전력 기반의 subray 위상 옵셋 Look-Up Table

097



===== PAGE 97 =====
모델링과 MATLAB

function [BS_theta_deg,MS theta_deg,BS PHI rad] =
gen_phase(BS_theta_LOS deg,BS AS deg,BS AoD deg,
MS_theta_LOS_deg,MS_ AS deg,MS AoA _deg,M)
Generates phase at BS and MS

oe

« Inputs:

%    BS_theta_LOS deg : AoD of LOS path in degree at BS

%    BS AS deg       : AS of BS in degree

%    BS AoD deg      : AoD of BS in degree

%    MS_theta_LOS deg : AoA of LOS path in degree at MS

%    119 29 deg       : AS of MS in degree

%    MS_AoA deg       : AoA of MS in degree

%    M             : # of subrays

% Outputs:

%    BS theta_deg     : (Npath x M) DoA per path in degree at BS
6    BS PHI rad       : (Npath x M) random phase in degree at BS
%    MS_theta_deg     : (Npath x M) DoA per path in degree at MS

if nargin==6, M=20; end
BS_PHI_rad=2*pi*rand(length(BS AoD_deg),M); % uniform phase
BS_theta_deg=assignoffset (BS_theta_LOS deg+BS AoD_deg,BS AS deg);
MS_theta_deg=assignoffset (MS_theta_LOS deg+MS AoA deg,MS AS deg) ;

% random pairing
index=randperm(M) ; MSl=size(MS_theta_deg,1) ;

for n=1:MS1, MS theta_deg(n,:)= MS theta_deg(n,index); end
Tl 프로그램 2.26 각 ray2| 위상 생성 함수

function theta_AoA_deg=assignoffset (AoA_deg,AS deg)
Assigns AoA/AoD offset to mean AoA/AoD

6 Inputs:

%     AoA _ deg : mean AoA/AoD
%     AS is: angle spread
% Output:              :

theta_AoA deg: AoA deg+offset_deg
offset=equalpower_subray table(AS deg) ;
theta_AoA_deg=zeros (length(AoA_deg) , length(offset)) ;
for n=1:length(AoA_deg)
for m=1:length(offset),
theta_AoA_deg(n, [2*m-1:2*m])= AoA _deg(n)+[offset(m) -offset(m)];
end
end

당

om
+

Te 프로그램 227 Zt ray2| 위상 옵셋

no

096



===== PAGE 98 =====
제2장_6150 채널 모델링

function h=

ray_fading(M,PDP,BS PHI_rad,MS_theta_deg,v_ms,theta_v_deg, lam, t)

h=ray_fading(M,PDP,BS theta_deg,BS PHI|rad,MS theta _deg,v_ms,
theta_v_deg, lam, t)

% Inputs:

%   M         : number of subrays

%   PDP         : 1 x Npath Power at delay

%    BS theta_deg: (Npath x M) DoA per path in degree at BS
% BS PHI rad: (Npath x M) random phase in degree at BS
%    MS _theta_deg: (Npath x M) DoA per path in degree at MS
%   v_ms         : velocity in m/s

%   theta_v_deg : DoT of mobile in degree

%   lam         : wavelength in meter

%   ie         : current time

% Output:

%   h        : length(PDP) x length(t) channel coefficient matrix

MS _theta_rad=deg2rad(MS_ theta_deg); theta_v_rad=deg2rad(theta_v_deg) ;
% generate channel coefficients
for n=1:length (PDP)

tmph=exp(-j*BS PHI rad(n,:)')*ones(size(t)).*
개 ms*cos (MS _theta_rad(n,:)'-theta_v_rad)*t)j;
h(n, :)=sqrt (PDP (n) /M) *sum(tmph) ;
end
 프로그램 228 ray 모델의 페이딩 생성 함수

RR 주파수 선택적 페이딩 채널 모델링 기법
1.2.1절에서 기술한 바와 같이 주파수 선택적 페이딩 채널을 모델링하기 위해서는 다중
경로 채널에 대한 PDP(Power Delay Profile)7} 필요하다. PDPE 다중경로 채널을 통하
여 수신된 신호의 평균 전력 BES 나타내는데, 일반적으로 기준 시간에 수신된 전력어
대하여 초과 지연 시간에서 수신된 상대 전력으로 나타낸다. 표 2.3~2.6은 많은 종류의
PDP 모델 중에서 널리 사용되는 110-#과 COST 207 모델을 보여준다[23][291.

099



===== PAGE 99 =====
PART 1 _무선 채널 모델링과 MATLAB

23 ITU-R 모델의 Power Delay Profile

0       0.0       0.       0.0       0       0.0       0      =o    Classic

1

2     110      =     200     09     310      = 0     800      0.0     Classic
3     190     19 2     800     -4.9     710     -=9.0     8900    12,8 | Classic
4           410          —22.8         1200          -8.0          1090         =10.01 ㅣ 12000. 10 0 | Classic
5                      28300     8     1780    =15.0    WOO. -88 8. Classic
6                      8700    -28.9    2510    -20,0 20000 -16,0 Classic

HE 2.4 COST 207 (Reduced TU, Reduced BU) 모델의 Power Delay Profile

0.0            0.189        gaat           0.0            Cie 이오

1

2         02        0,379       Classic        O73        0,293      Classic
3                     05                  0,239              Classic                 1,0                   0,147               GAUS1
4                     1,6                  0,095               GAUSI1                 1.6                  0,094               GAUSI1
5                      Dee                   0,061               GAUS2                  5,0                   0,185                GAUS2
6                     5 0                  0 087              GAUS2                 6.6                   0,117               GAUS2

= 2.5 COST 207 (TU, BU) 모델의 Power Delay Profile

0.0                  0,092              Classic                 0,                  0.033              Classic

1
2                    0.1                  0115              Classic                0.1                 0.089              Classic
3                     0,3                  0 201               Classic                 0.3                   0,141               Classic
4                     08                  0 127               Classic                 0?                  0.194               4081
5)                   0,8                 0,115              GAUS1 .              1,6                 0,114              GAUSI1
6          Le;         0,074       GAUS1        2.2        0,052       GAUS2
7          | 이        0.046       4081        에        0 035       GAUS2
8                     1.0                  0.074               41081                 5.0                  0,140               GAUS2
9          2.3         0,051       GAUS2        6,0        0,186       GAUS2
10                    831                  0,032              GAUS2                 (2                  0,041              GAUS2
ul         82         0.018       GAUS2        8.1         0,019       GAUS2
19                    8 0                  0,025              GAUS2                100                 0.006              GAUS2

100



===== PAGE 100 =====
제2장_ 68150 채널 모델링

퓨 2.6 COST 207 (RA) 모델의 Power Delay Profile

1                              00                              0.602                             RICE

이                              Ow                               0,241                           Classic
3                              02                              0.096                           Classic
4                                 03                                  0,036                              Classic
5                                   0.4                                    0.018                                Classic
6                                 0.5                                  0,006                              Classic

은 PDP7} 주어질 경우 주파수 선택적 페이딩 채널을 구현하는 방법을 설명한다.

(1) TDL 모델
TDL(Tapped Delay Line) 모델은 다중경로 채널을 구현하기 위하여 널리 사용되는 방
식으로서, TDL 모델의 입력으로 평균전력이 1이며 "+ EPO] 없는 다수 개의 주파수
비선택적 페이딩 생성기의 출력이 사용된다. 이 ASL 채널 모델에 의하여 주어진 각 탭
의 전력과 곱해진 후 그림 2.20에 주어진 TOL 모델의 계수로 사용된다. TOLE

일반적으
로 118 필터로 구현되고, TOL 모델을 통하여 수신된 신호는 다음과 같이 표현된다.

26 기
y(n) = >, h,(n)x(n-d)                                        (2.42)
d=0
a(n-1                        a(n—Np +1)
go         후기    이     Zito
Flat Fading        < 4600. <
generator        * VB       (x)
1
Flat Fading             Lon          h,(n)                      K
generator        Y VB                  9
2
Flat Fading       (lives                                          @
generator      ba J 도                                      별

ri
000= 1 Agla)ale—a)

그림 2.20 TDL 기반의 주파수 선택적 페이딩 채널 모델

101


===== PAGE 101 =====
PART 1 _무선 채널 모델링과 MATLAB

그림 2.20으로부터 알 수 있듯이, TOL BAS 독립적인 주파수 비선택적 폐이딩 생성
기만 있으면 FIR BES 사용하여 쉽게 구현할 수 있다. 그러나, 채널 탭의 지연 시간이
샘플링 주기의 정수배가 되지 않는 경우에는 FIR 필터 FAS 적용하기 쉽지 않다. 다음
절에서는 이와 같이 샘플링 주기의 정수배가 되지 않는 경우에 이를 처리하는 방법에 대

(2) 탭 조정 방법
일반적인 채널 모델의 PPPS 특정한 환경(매크로 셀, 실내 등)에서 측정된 결과를 기
woe 만들어지기 때문에 샘플링 주기의 정수배에서 주어지지 않는 경우가 대부분이
a

다. 이 경우 이산ㅅ^ 본 채널 dee 구현하기 위해서는 불가피하게 ?1#를
야한다. 가장 좋은 방법은 오버샘플링을 충분히 해서 탭 지연이 샘플링 주기의 정수배가
도록 해        AEE 할 경    a  필터의 채널 탭이 너무 길어져 시뮬레이션
이 거의 erate | 될 될 수 있다. 보다 간단하게 구현될 수 있는 방법으로서 탭 보간(62
interpolation), 라운딩 pills 탭 이 resampling) 등의 탭의 전력과 지연 시
간을 조정하는 다양한 방법들이 있다. 본 절에서는 이 중에서 가장 널리 사용되는 라운딩
과 탭 보간 방식을 설명  한다 이와 같은 탭 조정 과정에서 탭 조정 후의 채널 특성, 특히

ms 지연 확산이 탭 조정 전에 비하여 크게 바뀌지 않도록 해야 한다.
문자 243 가장 가까운 샘플링 시간 위치로 이동시키는 방식이다. 이

re
4

OW

muy

경우 각 경로의 전력 및 경로의 수가 변화가 없다는 장점이 있다. 라운딩 방식에 의하여
변경된 지연시간은 cheat 같 같이 주어진다.

= floor(t, / 4 + 0.5)                                (2.43)

여기서 《, 는 데이터의 샘플링 시간을, ty     J
식은 MATLABS] “round” 함수를 이용하여 구현할 수 때 이러한 라운드 방식은 주
진 채널 모델에 비하여 탭 수가 감소는 할 수 있어도 증가되는 경우는
경로 수를 쉽게 판단할 수 있다는 장점이 있다. 라
(2.43)로 미리 라운딩하여 탭 수와 전력을 결정하고
페이딩을 생성하는 사전 처리(006-[[0005908) 방식과
식 (2.43)에 따라 결정된 탭의 위치가 동일한 경로는 결합하는 사후 처리(008『-0000655118)
방식이 있다. 연산량 측면에서 사전 처리 방식이 좋지만, 채널의 특성(006 지연 확산) 측

a
atc)
x
rf
a
69
filo
to,
EP
Oh
고
호

Ho

Ho [A
ot
>!

&
nay
or
ro ㄷ
, ol
=
&
of

102



===== PAGE 102 =====
제2장_6150 채널 모델링

면에서는 사후 처리 방식을 좋을 수 있다. 각 경로마다 도플러 주파수나 스펙트럼 등이 다
를 경우에 사전 처리 방식은 원래의 채널 모델보다 경로의 수가 증가하거나 감소하게 되
면 이를 처리하기  " 매하다. 그러나 사후 처리 YAS 주어진 경로 수만큼 페이딩을 생성
하고 사후에 이를 결합하기 때문에 경로 수의 증감을 처리하기 용이하다.

후          0000    new tap

0     :    2t,   34,   delay

그림 2.21 라운드 방식의 탭 조정 예

탭 보간 방식은 원래의 채널 탭을 두 인접 샘플링 시간 사이에 지연 시간 상의 상대적

인 거리만큼 가중치를 두어 탭을 분배하는 방식이다. 먼저 각 지연 탭의 이산시간 인덱스
와 상대적인 시간차를 구하기 위하여 다음과 같이 지연 시간을 처리한다.

t, = floor(t, /t,)
t=t,/t-t,

여기서 《는 이산화된 지연 인덱스를 a /, 는 4 로부터 떨어진 상대적인 거리를 나
타낸다. 이러한 BTA has          플링 시간 상에 분배하는 WAS 다음과 같다.

h(n) =H, (n) + J1=t,h,(n)                            os)

h(n) = h(n) + Jt,hy()
여기서 ^, 00)는 새로 생성된 채널의 BA 계수를 나타낸다. 4] (2.44)에서 OS 피드
백하는 이유는 하나의 탭이 두 개의 탭으로 분해되기 때문에 인접하는 Bou 샘플링 시
Zt 사이에 하나 이상의 Yo] 존재할 경우에 같은 샘플링 시각에 하나 이상이 SAS 수
있기 때문이다. 그림 2.22는 탭 보간 방식에서 탭 조정의 예를 보여준다. 이 그림에서 2/,
샘플링 시각에는 두 개의 탭에 의하여 SARS 확인할 수 있다. 전력에 대해서 탭 보간을
할 경우에는 다음 식을 사용한다.



===== PAGE 103 =====
_무선 채널 모델링과 MATLAB

new tap

0               [1              27             3t,          delay

그림 2.22 탭 보간 방식의 탭 조정 예

(2.46)

탭 보간 방식 역시 식 (2.46)에 따라 미리 계산된 경로의 전력 및 수만큼 독립적인 페이
Be 생성할 것인가, 아니면 채널 모델에 주어진 경로 수 및 전력에 따라 페이딩을 생성한

후 식 (2.45)에 따라 두 경로의 각 폐이딩을 결합시킬 것인가에 따라 사전 방식과 사후 방
식으로 분류된다.
보간 및 재샘플링 방식에서 연산 속도를 증가시키기 위해서는 페이딩의 보간 과정을

저 수행하고 페이딩 채널 생성 과정을 진행하는 것이 좀 더 이득이 있을 수 있으나, 이
우 lols) 샘플의 증가로 메모리의 사용량이 증가하므로 wales Adel 따라 적절
방식을 선택해야 한다.

먼
경
한

@W sul ws 모델링 기법

SUI(Stanford University Interim) 채널 모델은 1.1.3절에 소개된 전파 환경과 같은 무
선 채널 환경을 위하여 제안된 모델이다. 이러한 전파 환경을 갖는 채널은 다수의 파라미
터 조합이 가능하지만, SUL 채널 모델은 표 2.7에 나타난 바와 같이 다른 파라미터 조합
으로 구성된 6가지 채널로 북미 지역의 전형적인 3가지 지형 타입을 묘사한다[8][101.

표 2.7 지형 타입에 따른 Sul 채널 모델

A                   SUI-5, SUI-6

B                        SUI-3, SUI-4
C                        SUI=l; SUIl=2

104


===== PAGE 104 =====
제2장_ 6150 채널 모델링

표 2.8 SUI 채널 파라미터

Delay [ys]           0/0/0/0/0/0       0,4/0,4/0,4/1,5/4/14      0.9/1,1/0,9/4/10/20
Power (omni ant,) [08]     0/0/0/0/0/0     -15/-12/—-5/-4/-5/-10 -20/-15/-10/-8/-10/—-14
90% K-fact, (omni)       4/2/1/0/0/0          0/0/0/0/0/0           0/0/0/0/0/0
75% K-—fact, (omni)      20/11/7/1/0/0         0/0/0/0/0/0           0/0/0/0/0/0
50% K-fact, (omni)       al all s/ 2/4         Sl a O10           Ted ay
-이189 /-10/-i/— ㅣ -88/ 07, -9e/ -20
Power (30° ant.) [dB]    0/0/0/0/0/0     26 이 려 es    a ae  ae
90% K-fact. (30"  ant.)    16/8/3/1/0/0        pido          cae
75% K-fact, (30° ant.)    72/36/19/5/2
sith ete Gk a   als      0/0/0/0/0/0       0/0/0/0/0/0
:      !                      -/-/-/-/0/0         -/-/-/-/0/0
Doppler [Hz]      0,4/0,2/0,4/0,2/2/0,4 0,3/0,15/0,3/0,15/1,5/0,3 0,5/0,25/0,5/0,25/2,5/0,5
Antenna Correlation                           Penv = 9.7/0.5/0.4/0.3/0.5/0.3
Gain Reduction Factor                          Gap =0/2/3/4/4/4dB
ein             F.,,,, =-0.1771/ -0.3930 / -1.5113 /-1.9218 /-1.5113 /-0.5683qB
Eee aien. 086 이        F,,, =-0.0371 / -0.0768 / -0.3573 / -0.4532 / -0.3573 /-0.1184aB
Terrain Type                                  C/C/B/B/A/A
o, =0.111/ 0.202 / 0.264 /1.257 / 2.842 /5.240 ys
Omni antenna                        K=3, 3/16/0.5/0.2/0,1/0,1(90%)
Overall K                       K=10,4/5,1/1,6/0,6/0.3/0,3 (75%),
=-/-/-/-/1.0/1.0 (50%)
©, = 0.042 / 0.69 / 0.123 / 0.563 /1.276/ 2.3708
30° antenna              K=14,0/6,9/2.2/1,0/0,4/0,4 (90%),
Overall K :                     K=44,2/21,8/7,0/3,2/1,3/1,3 (75%),
K=—/—/-/-/4,2/4,2 (50%)
SUI 채널은 ¥ 2.89] 주어져 있는 파라미터 조합으로 6가지 채널로 구분된다. 501 A
널 모델에서은 040060` 전력밀도함수를 갖는 특별한 도플러 전력 스펙트럼을 사용하며,
다음과 같이 정의된다.
1-1.72 HO    a]
Jo + 0.785 fq fo                     (2.47)

s-{     ;      oat



===== PAGE 105 =====
PART ｌ 무선 채널 모델링과 MATLAB

-126   ;   7   +   T   7   +   、      0
-128                                                 |
-130                                                 {
dB -132                                 -6|------ ero -b-----b-= sohoReape nee Serene, ery Seema ieee |
=164                                 8    로  a   L   t   4
-136                                0) a ee eee그. eae
25 -1.5 -1 -0.5 0 05 1 #15 2 25  4 08 -06 -04 2 0 0.2 04 06 08 1
fo(Hz)                               f/fm(Hz)
(a) 2.5GHz 대역에서 측정된 도플러 PSD          (06) Rounded 도플러 PSD

그림 2.23 Rounded 도플러 PSD

여기서 fo=t/fn 이다. 그림 2.232 2.5GHz 대역에서 측정된 도플러 스펙트럼과
(2.47)에 의해 BALE] rounded 도플러 스펙트럼을 보여준다.

표 2.8에 주어진 SUL 채널 파라미터 중에 Poy, 로 정의된 안테나간 상관 파라미터가

.0

으나 이는 MIMO 환경에 필요한 파라미터이므로 3장에서 설명한다. SUL 채널 모델링 과

정은 그림 2.24에 나타난 바와 같이 생성하고자 하는 AS 파라미터를 설정하고,
(2.47)에 주어진 도플러 스펙트럼을 2.3.1에서 기술한 FWGN 기법을 이용하여 Boles

널을 생성할 수 있다. 마지막으로 보간과 재샘플링을 통하여 설계하고자 하는 무선 전송
H

시스템에 적합한 페이딩 ALS 생성한다. 보간과 재샘플링 방식은 2.3.4절에서 설명한
식을 사용한다.

Setting SUI channel parameter

,

SUI fading channel generation using FWGN with filtering

,

Time interpolation or resampling

a2! 2.24 SUI 채널 모델링 과정

그림 2.25  ¥ 2.80] 주어진 SUI-6 ABS 수정된 FWGN 기법을 수정하여 Holy
HAS 생성한 것이다. 각각 901-6 채널의 POP, 시간에 따른 크기 변화, 생성된 도플
스펙트럼 특성을 나타낸다.

 106

tT]



===== PAGE 106 =====
제2장 68150 채널 모델링

PDP of Channel No.6

r       t      ;

!      H       H      H      H

|      !       '      '      |
따져400000doe

1      i       i      '      i

'      '       !      !      {

!      !       i      H      '

|      ;       |      |      ;

{      i       i      '      !

'      !       |      |      |
… eeee겨레 재테 제제 0

{      ;       1      |      ;

!      i       !      !      !

!      !       {      '      H

|      {       '      {      H

H      i       '      i      H

H      :       H      {      |
| 0000eeee으으000

      :       :      t      :

'      |       !      |      '

H      H       !      |      '

|      H       !      H      !

'      H       i      H      i

!      i       !      {      !
| a튼 020tie eseee 제

      !       {

|      !       i      !      i

!      i       i      {      |

{      i       i      '      '

|      !       H      i      !

i      !       H      !      i
a oe eeeee 제

{      i       1      t      (

'      '       |      '      {

H      H       H      i      :

{      {       |      :      ;

H      '       H      '      '

{      H       !      '      H
0| ee eee Sone!

{      '       1      {      |

:      {       !      i      !

i      i       i      H      {

|      {       H      !      :

!      i       H      {      i

i      !       '      |      :
aea ae ae ae!

'      '       {      1

H      H       '      {      '

H      H       '      {      '

H      H       H      H      '

i      H       '      H      i

!      H       !      '      H
주pounessjesueesa!a~ |

:      {       {      {

i      H       ㅣ      I      !

|      {       !      |      !

H      i       !      H      \

|      !       !      |      :

'      !       !      !      i
SS 가1 eee

‘      i       i      !      {

{      !       {      !      !

|      !       !      !      i

|      {       '      {      i

'      {       !      i      H

!      !       H      i      !
베루 eee ~

{      i       1      !      i

'      '       '      !      [

{      i       H      i      H

|      H              H      {

'      H       H      H      '

>     !     !      !     !

r        '         1         1         1

'      !              !      !

!      !       H      i      !

=      =      So      =

Delay time [ms]
(a) SUI-6 채널의 PDP

Channel No.6

[GP] 18400 |044642

Time [9]

06) SUI-6 채널의 시간영역 크기

=
특성

Simulation
Ideal

hg path

0
Frequency[Hz]

(6) 전력 스펙트럼 (4, )

1

1

0.87
0.6
0.4f
0.2

Simulation

Ideal

hy path
0
Frequency [Hz]

1

1

0.8[
0.6[
0.4
0.2

Simulation
Ideal

h, path
0
Frequency[Hz]

(0) 전력 스펙트럼(^4 )

1

1

a

(0) 전력 스펙트럼 (hf)

그림 225 SUI 채널 모델로



===== PAGE 107 =====
PART ｌ 무선 ale 모델링과 MATLAB

% SUI_channel test.m

clear all,clf;

ch_no=6;

fc=2e9;

fs Hz=10e6;

Nfading=1024; % size of doppler filter

N=10000;

Nfosf=4;

[Delay_us, Power_dB, K factor, Doppler shift_Hz, Ant_corr, Fnorm_dB] =
SUI_ch_param(ch_no) ;

[FadTime tf]=SUI_fading(Power_ dB, K factor, Doppler _shift_Hz, Fnorm_dB,
N, Nfading, Nfosf) ;

의 table=("b", 전, 히토;

subplot (311)

stem(Delay_us,10.* (Power _dB/10)),axis([-1 21 0 1.1])

grid on, xlabel('Delay time [ms]'), ylabel('Channel gain ');

title(['PDP of Channel No.',num2str(ch_no)]);

subplot (312)

for k=1:length(Power_dB)

plot ((0:length(FadTime(k,:))-1)*tf,
20*1log10 (abs (FadTime(k,:))),c_table(k));
hold on
end
grid on, xlabel('Time [s]'), ylabel('Channel Power [dB] ')

title(['Channel No.',num2str(ch_no)]), axis([0 60 -50 10])

legend('Path 1','Path 2','Path 3')

idx _nonz=find (Doppler shift _Hz) ;

FadFreq =ones (length (Doppler shift Hz) ,Nfading) ;

for k=1:length(idx_nonz)
max_dsp=2*Nfosf*max (Doppler shift _Hz) ;
dfmax=max_dsp/Nfading;
% Doppler frequency spacing respect to maximal Doppler frequency
Nd=floor (Doppler shift _Hz(k) /dfmax) -1;
£0 = [-Nd+1:Nd] / (Nd); % frequency vector
f£=£0.*Doppler shift Hz(k);

_ 108



===== PAGE 108 =====
제2장_ 9150 채널 모델링

tmp=0.785*f0.*4 - 1.72*f£0.*2 + 1.0;

hpsd=psd(spectrum.welch, FadTime (idx _nonz(k),:),'Fs',max_dsp,
'SpectrumType', 'twosided') ;

nrom_f=hpsd.Frequencies-mean (hpsd. Frequencies) ;

psd_d=fftshift (hpsd.Data) ;

subplot (3,3,6+k), plot (nrom_f,psd_d,'b', £,tmp,'r')

xlabel ('Frequency[Hz]'), % axis([-1 10 1.1*max([psd_d tmp])])

title(['h_',num2str (idx _nonz(k)),' path']);

end

Tal 프로그램 2.29 SUI 채널 모델 실행 프로그램

function
[Delay _us, Power _dB,K,Doppler_shift_Hz,Ant_corr,Fnorm_dB] =SUI_ch_param

Doppler _shift_Hz: Doppler frequency [Hz]
Ant_corr        : antenna (envelope) correlation coefficient

(ch_no)

% SUI Channel Parameters from Table 2.8

% Inputs:

* ch_no          : channel scenario number

% Ouptuts:

% Delay_us        : tap delay [us]

% Power dB        : power in each tap [dB]

6 K               : Ricean K-factor in linear scale
%

Fnorm_dB        : gain normalization factor [dB]
if ch_no<1||ch_no>6, error('No such a channnel number'); end
Delays= [0 0.4 0.9; 00.4 1.1; 00.4 0.9; 01.5 4; 04 10; 0 14 20];
Powers= [0 -15 -20;0 -12 -15;0 -5 -10;0 -4 -8;0 -5 -10;0 -10 -14];
Ks = (400; 200; 100; 000; 000; 00 0];
Dopplers = [0.4 0.3 0.5; 0.2 0.15 0.25; 0.4 0.3 0.5;

0.2 0.05 0.25% 2 LoS 2.5; 024/0.38 O25] 5
Ant_corrs = [0.7 0.5 0.4 0.3 0.5 0.3];
Fnorms = [-0.1771 -0.393 -1.5113 -1.9218 -1.5113 -0.5683];
Delay _us= Delays(ch_no,:); Power_dB= Powers(ch_no,:); K=Ks(ch_no,:)j;
Doppler shift _Hz= Dopplers(ch_no,:)j;

Ant_corr= Ant_corrs(ch_no); Fnorm_dB= Fnorms(ch_no) ;

]

| 프로그램 2.30 SUI 채널 파라미터 설정 함수

(

109


===== PAGE 109 =====
PART 1 _무선 채널 모델링과 MATLAB

function [FadMtx tf]=SUI_fading(Power_dB, K_factor, Doppler 6141 82,
Fnorm_dB, N, M, Nfosf)
SUI fading generation using FWGN with fitering in frequency domain
FadingMatrixTime=SUI_fading(Power_dB, K_factor,...

Doppler _shift_Hz, Fnorm_dB, N, M, Nfosf)

Inputs:
Power dB          : power in each tap in dB
K_ factor          : Rician K-factor in linear scale

Doppler_shift_Hz : a vector containing maximum Doppler
frequency of each path in Hz

00 AP 00 00 00 ㆍ 00 00 00 00 00 00 00 00 00 ㅇㅇ

Fnorm_dB          : gain normalization factor in dB

N                : # of independent random realizations

M                 : length of Doppler filter, i.e, size of IFFT

Nfosf            : fading oversampling factor

Outputs:

FadMtx           : length(Power dB) x N fading matrix

tt   : fading sample time=1/ (Max. Doppler BW * Nfosf)
Power = 10.* (Power _dB/10) ;   % calculate linear power
82 = Power./(K factor+1) ;    % calculate variance
s=sqrt (s2) ;
m2 = Power.*(K_factor./(K_factor+1)); % calculate constant power
m = sqrt (m2) ;                % calculate constant part
L=length (Power) ;            % # of tabs

fmax= max (Doppler _shift_Hz) ;

tf=1/ (2*fmax*Nfosf) ;

if isscalar (Doppler _shift_Hz),

Doppler_shift_Hz= Doppler _shift_Hz*ones(1,L); end
path _wgn= sqrt (1/2) *complex(randn(L,N),randn(L,N));

for p=1:L
filt=gen_filter(Doppler_shift_Hz(p),fmax,M,Nfosf,'sui');
path(p,:)=fftf£ilt(filt, [path_wgn(p,:) zeros(1,M)]); %filtering WGN
end
FadMtx= path(:,M/2+1:end-M/2) ;
for i=1:L , FadMtx(i,:)=FadMtx(i,:)*s(i)+m(i)*ones(1,N); end

FadMtx = FadMtx * 10*(Fnorm_dB/20) ;

—

ial 프로그램 2.31 SUI 채널 함수

110


===== PAGE 110 =====
장에서는 통계적 MIMO 모델링의 기본 ARS 설명하고, MIMO 모델로 널리 사용
되는 상관 기반(600ㅁ6180400-68560)의 I-METRA 채널과 Ray 기반의 3GPP SCM(Spatial
Channel Model)o] 대하여 설명한다. 상관 기반의 MIMO 채널 모델링 기법은 송수신 안
테나 배열과 수신 안테나 배열의 공간 상관 행렬만 알면 비교적 쉽게 상관성 있는 채널을
생성할 수 있는 장점이 있으나, 도플러 스펙트럼에 의한 시간 상관과 공간 상관이 별개로
생성된다는 단점이 있다. 반면에, Ray 기반의 MIMO 채널 모델링 기법은 주어진 PAS
(Power Azimuth Spectrum)S 갖도록 다수의 RayS 각 영역(30816-0000310)에서 분산시
A 결합함으로써 별도로 도플러 스펙트럼이나 공간 AWS 고려할 필요가 없는 WH] 있
으나, 페이딩 채널 생성을 위한 연산속도가 비교적 느린 단점이 있다. 이외의 MIMO 채널
모델로 SCM-E, IEEE 802.11 TGn, 그리고 유럽의 WINNER 프로젝트에서 이루어진
WINNER I 모델, WINNER II 모델 등이 있다.

ae
~
Ww

=

하나의 안테나를 갖는 시스템에서 채널의 특성을 파악할 때 가장 중요한 요소는 지연
확산(080 spread} 도플러 확산이었다. MIMO 채널에서는 추가적으로 안테나간 상관
AS 결정하는 다중경로 신호의 입사각이 중요한 요소로 작용한다. 고도각(61608000
angle)& 무시하고 단지 방위각(4200401 30816)만 고려하면, 그림 3.1과 같이 42 개로 구성
된 ULA(Uniform Linear ^0850로 수신된 신호 벡터는 식 (3.1)과 같이 표현된다.

y(t) = 2a e(d)xt—7,) + NO                          (3.1)

111


===== PAGE 111 =====
PART 1 _무선 채널 모델링과 MATLAB

building
Base                                         |
station
y, (t) _Y
yy (t) _Y
aft) —Y

house
그림 3.1 간단한 SIMO 무선 채널 환경

여기서 YO= TIVO. WO. VO! 은 MA 안테나로 수신된 ASS 나타낸다. 또
한, &, 7 @ 는 각각 ; 번째 경로의 채널 이득, 지연, AoA(Angle—of—Arrival)S 나타
낸다. 여기서 번째 ABS] ASE 하나의 신호로만 구성된 것이 아니라 @각도를 평균값
으로 하고 주위에 분포되어 있는 수많은 신호의 합으로 주어진다. 0(0) 은 배열 조정 벡터

(array steering vector)S 나타내며, 0(0)=[< (0), (0), …, 0,(0)] 로 정의된다. 각 수
Al 안테나의 조정 엘리먼트, c, (9) & 다음과 같이 주어진다.

 (0) = ft, (0)6 Pr DAlAsing                                             (3.2)

여기서 7,(0)은 m Ha 배열 엘리

[모
Je,

=

복소 Yes} a(complex field pattern)}& 나타

내며, 0 와 AS 각각 엘리먼트간 간격과 파장을 의미한다. 4 (3.1)의 수신신호 y(t
식 (3.3)과 같이 적분형으로 표현할 수 있다.
y(t) = | fe()h(g,7)s(¢— dtd b+ N(1)                   (3.3)

여기서 채널을 나타내는 (0, 은 채널의 ADS(Azimuth—Delay Spread) 함수이다. 순시
PADS(instaneous Power Azimuth—Delay 50600400)는 다음과 같이 주어진다.

(3.4)

~                                            1?

112



===== PAGE 112 =====
MISS MIMO 채널 모델링

평균 PADSE 식 (3.4)의 기대값으로 주어진다.
P(9,7) = E[ Phy (9,7)|                         (3.5)

PAS(Power Azimuth Spectrum, Power Angular Spectrum)-<- PADSS 지연 시간에 관
하여 적분함으로써 구할 수 있고, AS(Azimuth Spread, Angular Spread)+= PAS°] 2%} 중

심 모멘트(660081 moments) 주어지며, 각각 다음 식으로 표현된다.

2.000= ]86.007                        (3.6)

=. @-ay P.@ade                              (3.7)

여기서 평균 AoA @%은 A = [oP, de 2 주어진다. 또한, PDS(Power Delay Spec-
turm)2 PADSS AoA] 대하여 적분함으로써 구할 수 있고, DS(Delay Spread): PDS
의 2차 중심 모멘트로 주어지며, 각각 다음 식으로 표현된다.

P, (2) = 180 2)00                                         (3.8)

0, =) (c- mF P,@de                                (3.9)

여기서 평균 지연 확산, ToS T= ]『>(007으로 계산된다.
^04ㅅ와 지연의 marginal PDF(Probability Density Function)2 각각 다음과 같이 주어
진다.

7,(0)= [7 (9,7 )dt                                        (3.10)

fp(t) = [F.0d                                 (3.11)

여기서 /(0.7) 은 AoA} 지연의 joint PDFS 의미한다.

113


===== PAGE 113 =====
PART 1 무선 채널 모델링과 MATLAB

Clark] 채널 모델은 이동국에서 AOAE 균일한(404000) 확률밀도함수를 가정하
지만, 기지국의 AOA 확률밀도함수는 이와 큰 차이가 있다. 일반적으로 이동국의 공간 상
함수(608081 correlation function)= 1/22] 파장 간격을 갖는 안테나 배열에서 0에 가까
상관을 가지나, 기지국의 경우에는 45에 따라 차이는 있지만 낮은 상관을 위해서 파장
OF 10~40배 정도의 거리가 필요하다. 지연의 확률밀도함수는 일반적으로 지수함수로
근사화된다.

to fo re

unresolvable paths

M, Subrays
Got Abn
ULA

configuration                    a           Resolvable paths

La, To 00]
spacing, af |

                             broadside
oe es
La», T2 $y]
toe rs

La,  Th  6]

(a) 다중 안테나에 수신되는 신호 예

Average
Power ? Po                       PAS                 POF
Py
Gaussian PDF in micro/macro
 P,                                                environments
T% TM ×     delay        01 AoA [deg]          ¢: 404 [deg]
(b) PDS             (c) PAS         (0) AoA2] 확률밀도함수

그림 3.2 다중 안테나에 수신되는 신호의 PDS, PAS, PDF

그림 3.2는 그림 3.1의 수신부를 확대하여 보여준다. 이 그림에서 분해 가능한 경로
(resolvable 2802)는 3개로 구성되어 있으며, 하나의 분해 가능한 경로는 4, 개의 분해할

수 없는 4Ax(unresolvable path= 구성된다. M, 개의 분해할 수 없는 경로는 평균 AoA

를 중심으로 확산되어 입사된다. 44, 개의 분해할 수 없는 경로의 AoA BEE 마이크로
셀 또는 매크로 A 환경에서 일반적으로 Gaussian HES 보인다. 또한, AoA] 따른 전력



===== PAGE 114 =====
제3장_1140 채널 모델링

분포 즉, PASE 셀 환경에 따라 다르지만, 매크로 셀 환경에서는 Laplacian BES
기서 주의해야 할 사실은 AAS} PASS] 분포가 서로 다르다는 것이다. 즉, AoAY
BEE 각 경로의 전력이 고려되지 않은 수신 신호의 입사각만이 고려된 것이며, PASE
수신 ASS] 입사각인 404&에 전력이 고려된 것이다. 마지막으로, PDS 또는 PDP(Power
Delay Profile)o]2} 불리우는 분해가능한 경로의 전력분포는 지수함수의 BES 보인다.

그림 3.3과 같이 0 만큼 떨어진 두 ABSA (omni-directional) 안테나 a2} 6에서 수신
된 두 기저대역 신호 사이에는 7, 만큼의 시간 지연이 발생하게 된다. 이러한 경우에 협대
역 채널을 니케   } 안테나에 수신된 두 기저대역 신호는 다음과 같이 표현된다.

h, =06"120)                               (3.12)
h, = gee! Ft274sin(9)/)  P(@)                          (3.13)

여기서 는 Rayleigh 분포를 가지며, B= [0, 27)에서 균일하게 분포한다. 수식의 간략
화를 위하여 PASS (0) 로 표현한다. 만일 식 (3.12)와 식 (3.13)에서 평균 AoA 가
0“이고 AS ㅇ@,가 0°91 경우.2(6.)=0(0-$@) ), 즉, 배열 안테나의 수직방향으로 각 안
테나에 하나의 646008>만 수신되는 경우에는 두 수신신호 A, 와 %사이에 40&에 의한 시
Zt Al Ho] 발생하지 않으므로 공간 AWS 항상 1이다. 반면, AoA7} 0“이 아니고 48가
0“이 아니면 신호 사이에 시간 지연이 발생하게 되고, 이러한 경우에 두 신호사이의 상관
관계는 다음과 같은 공간 상관 함수에 의하여 결정된다.

ry =dsing,/c

Receive
Antennas

a
그림 3.3 두 전방향성 안테나의 수신 신호



===== PAGE 115 =====
PART 1 _무선 채널 모델링과 MATLAB

p.(d) = Efh,h, |
a j2mdsin(o-h)

=fe 4% P@-)dd                       (3.14)

-

=R..(d)+ j-R,(d)

여기서 평균 AoA 9, = | .02(0)00로 주어지며, PAS P(@)  [P@dg=12
정규화되었음을 가정한다. 또한, 《 (4)는 두 신호의 실수부 사이의 상관값을 나타내며,
R,(d)= /, 의 실수부와 / 의 허수부 사이의 AES 나타낸다. 안테나간 정규화된 거
리를 > =22077로 정의하면 RD) R,(D) = 다음과 같이 정의된다.

R,,.(D) = E[Re(h, )- Re(h, )] =  | cos(Dsin())P(9 — @ Jag                    (3.15)
R,,(D) = E[Re(h, ) - Im(h, )] =  |. 940(/280(0))2(0-0@)00                    (3.16)

식 (3.15)와 식 (3.16)로부터 확인할 수 있듯이 안테나간의 공
PASS] 의존적이다. 특히, PASS] AS7} 작으면 하나의 신호를 구성하는 많은 subraySo]
거의 같은 각도로 각 안테나에 입사되므로 두 신호의 크기는 거의 같아지고 위상만 AoA
에 의하여 차이가 나기 때문에 두 신호의 상관이 커진다. 다중 안테나 시스템에서 안테나
간 상관이 커지면 채널 용량 및 다이버시티 이득이 감소하므로 안테나간 충분한 거리를
두어 상관이 0에 근접하도록 설계해야 한다.

oS
ox
re
rlo
ofl
eu
>
°
>
a

PASE 안테나간의 공간 상관을 결정하는 데 중요한 요소로 작용한다. 『4.5에 의한 공
간 상관을 수학적으로 분석하기 위해서는 실제의 환경에서 발생하는 PAS 분포가 필요하
다. 이를 위하여 실측된 데이터를 기반으로 환경에 따른 여러 종류의 PAS 모델들이 보고
되         표 3.12 대표적인 PAS PASS 요약하여 보여준다.

 116



===== PAGE 116 =====
ASS MIMO 채널 모델링

표 3.1 무선 환경에서의 PAS2| 형태

ㆍ Laplacian

Macrocell
* n-th power of a cosine function
Outdoor        :            ¢ Truncated Gaussian
Microcell          ;        |                       Uniform
* Uniform
Picocell                Almost Uniform

Indoor                                                          Uniform

PASS] BFS 주로 주위의(10081) 산란 성분의 분포에 의하여 결정되는데, H 3.1에 나
타난 바와 같이 이동국의 PAS 지역 산란 성분이 많기 때문에 모든 무선 환경에서 균일
한 전력분포를 보인다. 반면, 기지국의 경우에는 산란 성분이 많은 피코셀 혹은 옥내 환
경에서는 균일한 PASS 가지고, 마이크로셀과 매크로셀 환경에서는 기지국의 지형적 특
성에 따라 다른 PAS BES 가지지만 대부분의 경우에는 AS7} 작은 EAA PASH 관측
된다.

표 3.2는 옥내외 환경에서 측정된 평균 AS 값을 보여준다. 옥내 환경의 경우에는 클러
스터링 효과에 의하여 다수의 클러스터가 관측되는데, 이러한 경우에 다중 클러스터 중
하나의 클러스터에 대한 결과를 보여준다. 표 3.2에 나타난 바와 같이 옥내 환경에서는
AS7} 크며, 옥외 환경의 경우에는 10° 이하로 매우 작음을 알 수 있다.

rit

표 3.2 무선 환경에서의 평균 As

[41]                1000                                                                                                     20~60°
[42]                1800  5~10°

[43]      1800     8°     5°

[44]      1845                 <10°

[45]                1873; 9~15°

[46]                200 9” gis

[47]      2154          10,3°

[48]                2200                                                    =             <ie°) | <0"

[49]                7000                                                                                                     2-96"



===== PAGE 117 =====
PART 1 _무선 채널 모델링과 MATLAB

118

(1) n-th Power of a Cosine Function PAS 모델
Ｌ66에 의해 최초로 제안된 n-th Power of a Cosine Function PAS 모델은 다음과 같이
코사인 함수의 차 전력으로 표현된다[501

20)=은0006), -즈+ =ㄴ0=즈+                 (63.17)
2          2         고

여기서 7은 빔의 폭과 관련된 짝수를 나타내며, 으는 pass 1로 정규화하기 위한 정규
화 요소이다.

그림 3.4는 평균 AoA7} 0*이며, 이 2, 4, 8인 경우의 PASS 보여준다. 이 그림에서
확인할 수 있듯이 MAS [-1/ 2.2/2] o] 존재하며 7이 증가할수록 PAs] ZS 좁아진
다. 이 경우에 공간 상관은 식 (3.17)을 식 (3.15)와 A} (3.16)에 대입하여 다음과 같이 주
어진다.

R,(D)= | cos(D sin(@)) cos" (0-4 100          (3.18)
R,(D)= | sinDsin(o) Sos" (6-4, \do           (3.19)

n-th power of a cosine function PAS, AoA=0[degree]
0.35       -      -      ~      .      ,

      |      |      !      !      |      !      ~ nee

;      |      {      |      ㆍ      ;      |      — n=4
OS) aaa aes ees SY / / a NX a i ed
    -

-100 -80 -60 -40 -20 0 20 40 60 80 100
¢ [degree]

그림 3.4 n-th Power of a Cosine Function PAS



===== PAGE 118 =====
제3장_ MIMO 채널 모델링

앞 식에서 PAS 모델이 코사인 함수의 차 전력으로 표현되기 때문에, 식 (3.18)과 식
(3.19)의 적분식은 풀기 쉽지 않다. 따라서 공간 상관의 분석적인 해는 존재하지 않으며,
수치 해석적으로만 구할 수 있다.

(2) 균일한 PAS 모델

균일한 PAS HAS 지정된 범위의
히, 옥내와 같이 산란 성분이 충분한

다[51].

각도상에서 동일한 전력의 분포를 가지는 모델로 특
환경을 모델링하기에 적합하며, 다음 식으로 주어진
PO)=Q:1, -AG+G SPSAG+ |,              (3.20)

여기서 Ag=vV3o, 22 주어진다. 4] (3.20)에서 정규화 요소 OS 구하기 위하여 식
(3.20)을 적분하여 O oj] 관하여 정리하면 다음과 같이 주어진다.

0=1/(240)                                (3.21)

식 (3.20)을 A] (3.15)와 식 (3.16)에 대입하여 공간 상관을 구하면 다음과 같이 주어
진다.

R,,(D) = J,(D) + 40d) J, (D) cos(2md, ) sin(2mA@) / 2m                   (3.22)
R,(D)= 40d) Joya, (D) sin((2m + 1)d,) sin((2m + 1)Ag) / (2m +1)              (3.23)

여기서 J,0& Al 1S 차 Bessel BPS 의미한다. AS7} 증가할수록
R,(D)=J,(D), R,(D)=0 # 수렴하게 된다.

그림 3.5는 ZU PAS 모델의 PAS 분포와 공간 상관 계수 예를 보여준다. 이 그림으
로부터 49 값이 증가할수록 같은 안테나 간격에서 공간                      9
다. 또한, AS7} 10*인 경우에는 oF 1.74 의 정수배 간격, AS7} 30°°] 4
의 정수배 간격으로 안테나를 배치할 경우에 0에 가까운 상관값을 얻을



===== PAGE 119 =====
PART 1 _무선 채널 모델링과 MATLAB

            Uniform PAS, AoA=0[degree]                                          Uniform PAS, AoA=0[degree]

i   {   | ||| — 46=10[069066]             i    '    i    — AS=10[degres]
16} --[ + /5-301000001        위미 aa et ial iin — AS=20idegree]

하는가      =
Plo) '     pip a

0타+
Or) a + 나가가

0    {    H        {        H    H
-200 -150 -100 -50   0 50 100 150 200
¢ [degree]

(a) PAS

그림 3.5 균일한 Paso] 전력 분

(3) Truncated Gaussian PAS 모델
Truncated Gaussian PAS 모델은 다음과 같이 표현된다[51].

P() = g 노고 -Adt+¢,<@< AG+d,      (3.24)
7220   ：   "

여기서 ot PASS] 표준편차, AGE [-z,2] 이며, 일반적으로 40=*를 사용한다.
Truncated Gaussian PAS 모델을 다음 AS 사용하여 1로 정규화한다.

|. 2(0)400= = [ie  1 00=1                                      (3.25)

여기서 0=20ㆍ/로 치환하여 다시 쓰면 다음과 같다.
so
[i Pe@)dg=E [eat -9-en| 50.) =1                (3.26)

여기서 07(ㆍ)는 오차 함수를 나타내고, 정규화 요소 QE 다음과 같이 주어진다.

120



===== PAGE 120 =====
제3장_\140 채널 모델링

001 52)                         (3.27)
식 (3.15)와 식 (3.16)에 식 (3.24)와 식 (3.27/을 대입하여 다음과 같이 공간 상관을 구
할 수 있다.

R,(D)=J,(D) + oy J, Dye?" cos(2md,)

Re er 26 “042 |-001- 26, - ino)

R, (D) =O Soy. (D)e?? "sin ((2m+1)4,)

그림 3.62 Truncated Gaussian PAS 모델의 PASS} 공간 상관 계수를 보여준다. 이 그
림에 나타난 바와 같이, AS7} 크면 전력이 분포하는 각도가 크기 때문에 같은 안테나 간
0

(3.28)

격에서 공간 상관 계수가 작아지며, AS7} 30*인 경우에는 oF
테나를 배치하면 0에 가까운 상관값을 얻을 수 있다
os      Truncated Gaussian PAS, AoA=0[degree]                                Truncated Gaussian PAS, AoA=0[degree]
|| — AS=10[degree]                                                  — AS=10|degreel
|| ~~ AS=30[degree]                                           —— AS=30[ degree]
Ol eset cas tawcee 개 | 개 게제 제에떼 제때                        |
1.5 Ee! AY ee EY 차        k
Raa
P(9)                                  [Po
1) ee ec oer eee eee
0.5 et ee) ee ee ene 은 eel me: Uf Se a Sa, ea
-150 -100 -50 0 50 100 150                                      6
¢ [degree]
(a) PAS                          (b) 공간 상관 계수

그림 3.6 Truncated Gaussian PAS2| 전력 분포 및 공간 상관 계수

121


===== PAGE 121 =====
PART 1 _무선 채널 모델링과 MATLAB

(4) Truncated Laplacian PAS 모델
매크로 셀이나 마이크로 셀룰러 환경에서 많이 관측되는 101008660 Laplacian PAS 모
ae 다음과 같이 주어진다[51].

P(Q)= g 늘고      -Ad+¢,<¢< AGOt+d       (3.30)
120   ：       laa   "

Truncated Laplacian PAS 모델을 다음 식을 사용하여 1로 정규화한다.

_20-&1

[i Po@de=— fe a

(3.31)
-—— aL Fado    (1-e") = 1

위 식으로부터 정규화 요소 OL 다음과 같이 주어진다.

Q= JK 0790]                      |                         (3.32)

식 (3.15)와 식 (3.16)에 식 (3.30)과 식 (3.32)을 대입하여 다음과 같이 공간 상관을 구

할 수 있다,

R,,.(D) = J,(D) + 40d) J,,,(D) cos(2m@, )

-V2A
[2 +. (2m-snm-a9)-/Bsos2n-a9)/a)|      (3.33)
떼힐  + (270)? ㅣ
oO
R,(D)= 40d) Joya (D)sin((2m +1)9,)
-v2A
대 ge ((2m +1)-sin((2m +1)- Ag) — V2 cos((2m+1)- Ag) / a)      (3.34)



===== PAGE 122 =====
제3장_ 1440 채널 모델링

4     Treated = PAS, AoA=0[degree]                    Truncated Laplacian PAS, AoA=0[degree]
:      {                  —AS=10[dearee]                   H                     = 6=10[06
gree]
8.5 bonnet                        0 Ro=o0l degree]             09                                             — AS=30| degree]
a ee ee ee eee eee eee eee     0.8
0.7
Car a ree ie | ee neta ea
0.6
000) 하나             Ral 05     ———
oe                    {| mt Se
=_—_—_|                  0.3
{                              0.2
0.5
i       7        !            0.1
00 -150 -100 -50 0   50 100 150 200     %
¢ [degree]
(a) PAS

그림 3.7 Truncated Laplacian PASO] 전력 분포 및 공간 상관 계수

그림 3.72 Truncated Laplacian PAS 모델의 PASS} 공간 상관 계수를 보여준다. 공간
상관값이 0.1 이하가 되기 위해서 48가 30*인 경우에는 안테나간 간격이 약 1.34
이상 떨어져 배치되어야 하며, 49가 10°C] 경우에는 안테나간 간격이 of 44 간격 이상
떨어져 배치되어야 한다.

(5) PAS 모델의 표준 편차와 ^8와의 관계

Truncated Gaussian PAS 모델과 Truncated Laplacian PAS 모델에서 ‘Truncated’ 2] 용
어가 ARB EE 이유는 -% 에서 %까지의 범위를 지니는 일반적인 Gaussian/Laplacian 3}
수에서 일부 범위만을 제한하여 사용하기 때문이다. 따라서, Gaussian/Laplacian PAS 모
델의 표준 편차는 ‘Truncated’=]7] 전의 -% 에서 ㅇ까지의 범위를 지니는 일반적인
Gaussian/Laplacian 함수의 표준 편차이며, 다음과 같이 표현할 수 있다.

a= | 0@0-0%0080000                                 (335)

여기서 do = | _08,(6000이다.
반면에, Truncated Gaussian/Laplacian PAS 모델에서 ASE 일반적인 Gaussian/

Laplacian 함수가 - 에서 *까지의 범위로 “170008160'된 후, 각 확산을 의미하므로 다
음과 같이 정의된다.

123


===== PAGE 123 =====
PART 1_ FM 채널 모델링과 MATLAB

0, =\ [0-4 P@do                           6.36)

여기서 =  [ PP,(9)AO 이다. A} (3.35)와 A] (3.36)에서 확인할 수 있듯이 PASS] 표

준 편차와 48의 차이는 적분 범위이다. Truncated Gaussian 『ㅁㅅ8과 Truncated Laplacian
PAS HAS 대칭적이기 때문에 Bato] 0인 PASS 가정하면, PASS] 표준 편차와 AS]
는 다음과 같은 관계가 성립한다.

0" = | 9 P@)do= | 0'80)000+2| 0'8(0)00

(3.37)
=o; +2] 6 P(b)do

AS vs. o of PAS
120                     :     7

— Gaussian PAS |:      '      |
—— Laplacian PAS |             |      !
UA rs ae; aes Vaias ae aaa

'                   1                   !                   '                   i
{                {                {                '                {                ‘
{                '                '                H                ‘                H                1
{                1                {                |                {                1!                {
80}------3Loe eet                Se ee oe ee ee
’                1                ;                |                t
{                i                ;                1                '                :                ‘
{                1                i                                 '

o of PAS

|        {        !        1                1
'        ‘        1        ‘        !        i        4
| a a an een eae) SUn eee Ae ee eee)
40     |
ee ee ee ee

;        t                '
{        {        』;        1                '
'        i        |        i        H                {
{        {        ;        ;        {        :        {

eeee Sees ee eee ee ee ee eee en Eee
i                i        ;        i
i        {        :        :        H        :        1
{        ‘        :        I        :        '

%    10 20 30 40 #50 60 70 80

그림 3.8 PAS 모델의 표준 편차와 ^46와의 관계

그림 3.82 PASS] 표준 BAS} AS BAS 보여준다. 이 그림에서 확인할 수 있듯이
AS7} 305도 이하로 작은 경우에는 PASO] 표준 편차와 거의 같지만, 30보다 커지면 치
이가 발생한다. Laplacian PAS 모델이 Gaussian 모델에 비하여 평균값에서 멀어질수록
빠르게 감소하여 A] (3.37)의 두 번째 항의 영향이 감소하기 때문에 선형 영역으로 근사할
수 있는 범위가 크다

(6) 다중 클러스터
이동국에 지역00081) 산란 성분들이 존재할 뿐만 아니라 인접한 지역에 큰 산란 성
이 존재할 ASO] 서로 다른 도달각과 PASH 갖는 다중 클러스터 신호가 수신된다. 특히

더

~

124



===== PAGE 124 =====
제3장_ 1400 채널 모델링

러스터 신호는 옥내 채널에서 많이 발생하며, 이러한 다중 클러스터 신호의 공간
간 상관 계수의 합으로 표현된다.
는                   Zt Laplacian PAS BAS 보여준다. 그림 3.9(@)에서
Al 번째 클러스터는 AoA7} —60°, AS7} 30°, 크기가 1이며, 두 번째 SAAR AoA7}
10°, 크기가 0.5이다. 그림 3.900)는 두 개의 클러스터로 구성된 수신 신호의
공간 상관 계수를 보여준다. 이 그림으로부터 수신 신호의 공간 상관은 각 클러스터의 공
간 상관 계수를 더한 결과와 같음을 확인할 수 있다.

Laplacian Power Azimuth Spectrum (2 clusters)                  Envelop Correlation Coefficient, | PactiP,, |

— Cluster #1: AoA=-60, AS=30 [degree]
—— Cluster #2: AoA=-60, AS=10 [degree] | |
|

~ i: “et Seine! fale Unter Saieiaiaecees Ria |

(전
아라
fo)

-150 -100 -50  0 50 100 150     0  1   2

[degree]                                  d/d
(a) PAS                             (b) 공간 상관 계수

그림 3.9 Truncated Laplacian PASS| 전력 분포 및 공간 상관 계수 (두 개의 클러스터)

PAS 생성 함수, PAS 모델에 따른 상관 계수 연산 함수 SS] MATLAB 프로그램은 웹
사이트에서 다운로드 가능하다[521.

O22 -metra mimo 채널 모델링 기법

본 절에서는 3.1절에서 설명한 MIMO 채널의 통계적 특성과 다양한 『4에서의 공간
상관을 이용하여 일반적인 MIMO 페이딩 채널을 생성하기 위한 방법을 설명하고, MIMO

pie —

시스템에 널리 사용되는 I-METRA MIMO 채널 모델링 기법에 관하여 설명한다[52].

125



===== PAGE 125 =====
PART 1 _무선 채널 모델링과 MATLAB

상관 기반 MIMO 페이딩 채널의 통계적 모델

그림 3.10에 주어진 74 개의 기지국 안테나와 N 개의 이동국 안테나를 갖는 다중 안테
나 시스템을 고려할 때, 협대역 통계적 MIMO 채널 HE 다음과 같이 표현될 수 있다.

H=0/7A,,0)70°                                  (3.38)

여기서 Ox = 수신 안테나간의 상관관계 행렬을 나타내며, ©, 은 송신 안테나간의 상관
관계 VAS 나타낸다. 또한, ^, 은 상관성이 없는 iid(independent, identically
distributed) Rayleigh 채널을 의미한다. A] (3.38)에 주어진 상관 기반의 MIMO 채널 모
We 기본적으로 송신부와 수신부의 상관행렬이 분리될 수 있음을 가정한다. 이러한 가정
은 송신부와 수신부에서 안테나간 간격이 송신부와 수신부 사이의 거리보다 충분히 작으
면 성립하는데, 실제 무선 통신 환경이 이에 해당한다. 이와 같은 Bao 상관행렬, Op
or 값을 조절함으로써 다양한 MIMO ALS 생성할 수 있다. Og 와 @,이 단위행렬
경우에 완전한 iid 채널을 모델링할 수 있으며, 이외에도 랭크-1 81002 채널, 임의
a9 } Rician 채널 등의 극단적인 경우의 FASE 비교적 쉽게 생성할 수 있다.

ne

©

Mobile Station (MS)                   Base Station (BS)
i                               a y(t)
“ot                                             ‘a 120)
wT | ~ Co

we                               ‘Cot

그림 3.10 MIMO 시스템

이동국과 기지국 사이의 광대역 MIMO 채널은 식 (3.38) 확장하여 TDL(Tapped
Delay Line) 형태로 다음과 같이 구성할 수 있다.

H(z) = >, ^,0(0-2)                                             (3.39)
7=1

126


===== PAGE 126 =====
제3장_\1040 채널 모델링

여기서 He CY 이며, /번째 경로의 복소 채널 이득 BBS 다음과 같이 주어진다.

0)         0)                  0)

Qa,       a By

(2)         (2)                 (1)

a, Ay          ay
A=. 00,                                   (3.40)

(7)         (1)                  00)

Ay, Ayr. 01110 2

여기서 uh 와 m Ba 기지국 안테나와 7번째 이동국 안테나 사이의 1번째 경로의 채널
이득을 나타낸다.

Mobile Station (MS)            Base Station (MS)

s,(t)     ny               VY yy (t)
()      oom     yo(t)
a(t)             mC ys(t)

그림 3.11 하향 링크 MIMO 시스템
그림 3.11에서와 같이 송신 신호가 기지국의 송신 안테나 mF mM. HAL 전송되는 하향

링크의 경우, 다른 두 개의 이동국 안테나 nwt 7;사이의 전력 상관관계는 다음과 같이
주어진다.

‘)                 3.41)

여기서 (x») =(Ebo]- BLxIELy))/ (ER? 1- ERED? I- ADP) 로 정의된다. 식
(3.41)에서 이동국의 안테나간 상관관계는 기지국의 안테나, mF} m, 2] 함수가 아니기
때문에 기지국 안테나에 독립적이라는 것을 알 수 있다. 즉, 송신기와 수신기 사이가 충분
히 떨어져 있는 경우, 기지국의 안테나 간격은 상대적으로 작기 때문에 이동국의 상관엔
영향을 주지 않는다. 이동국이 지역 산란자들에 의해 둘러싸여 있는 환경에서 472 이상
떨어져있는 안테나들은 상관관계가 매우 적다. 그러나 이러한 결과는 이론적인 결과이고,



===== PAGE 127 =====
PART 1 _무선 채널 모델링과 MATLAB

실제에서는 옥내 환경에서도 472 떨어진 안테나 사이에서 상관이 존재한다는 실험 결과
가 종종 보고된다.
이동국에서 안테나간 대칭적 공간 상관 행렬(600101601081 spatial correlation matrix)

다음과 같이 주어진다.

10 i     10 는     … 2 ne
MS  MS    MS

Ris = Pri  Pr  |  Pow                (3.42)
Pm Pra oo Paw

여기서 Ruy 의 대각 성분은 자기 상관임으로 항상 1이다.

이동국은 지역 산란자에 둘러쌓여 있어 안테나간 상관성이 작지만, 기지국의 경우에는
경로손실을 줄이기 위하여 일반적으로 높은 곳에 배치하기 때문에 기지국의 안테나 주위
에는 지역 산란자가 거의 없다. 이러한 이유로 기지국에서 BSE PASE 상대적으로 협
대역 빔폭(66001\1000을 갖는다. 그림 3.12와 같이 이동국 송신 안테나 nyt nyo) 송
신하는 상향링크 MIMO 시스템에서, 다른 두 기지국 안테나 m, 과 /;사이의 전력 상관
AS 다음과 같이 주어진다.

린

2
(1)
Bion

>

‘)                                        (3.43)

여기서 기지국에서의 공간 상관관계는 이동국의 안테나 nol 독립적임을 알 수 있다. 이러
한 가정은 송신기와 수신기가 충분히 떨어져 있을 경우에 이동국의 안테나들이 같은 위치
에 밀집되어 있고 같은 방사 패턴08018040ㅁ pattern) 가지기 때문에 타당하다고 볼 수 있
다. 기지국에서 안테나간 대칭적 공간 상관 행렬(600001001081 spatial correlation matrix)
은 다음과 같이 주어진다.

Pu Ba 때 Pin
BS  BS    BS

R,s =  _  .  나이                (3.44)
Pir 066 10 000

 128



===== PAGE 128 =====
AIS MIMO 채널 모델링

Mobile Station (MS)            Base Station (MS)

YO y, (t)

Yyo(t)

yg(t)

sy(t ) _Y                                   YO

그림 3.12 상향 링크 MIMO 시스템

00000

Mobile Station (MS)            Base Station (MS)

s,(t)        ny                       >  210)
eat} —Y                     re        yo(t)

s(t)                                YY

그림 3.13 송ㆍ수신 안테나간의 상관관계

8170)

여기서 대각 성분은 항상 1이다.

채널 이득 &,를 생성하기 위해서는 송수신 안테나 간 채널의 상관관계에 관한 정보가
필요하다. 그림 3.13에서 나타난 바와 같이 기지국 안테나 m, Fp 이동국 안테나 /,, 기지
국 안테나 my} 이동국 안테나 ny 사이의 두 전송 계수, a 과 al? 의 상관을 다음
과 같이 정의한다.

2
os = (lai,    OL  ㆍ                                               (3.45)
= Prin Pram                                                                  (3.46)

4] (3.45)에 대한 이론적인 해는 존재하지 않으며, 각 경로의 전송 계수 %/; 의 평균 전
력이 같다는 가정하에서 식 (3.46)으로 근사화할 수 있다.

129



===== PAGE 129 =====
PART 1 _무선 채널 모델링과 MATLAB

= MIMO 페이딩 채널 생성 방법

MIMO 채널의 전송계수는 다음 식과 같이 상관성이 없는 벡터에 상관 행
수 있다
(3.47)

[a 경로의 평균 전력을 나타내고, 상관성이 없는 MIMO 페이딩 채널 벡
터 4 = [", 0", …, aviv dae 주어진다. 이 때 0
21= 2, 또는 |, #1, 대하여 (lal?  a2) "= 0이고 평균이 0°] 복소 Gaussian 분
있는 MIMO 페이딩 채널 계수로서 다음과 같이 구성된다.

여기서 가을

은 plaP] =1이며,

갖는다. AE 상관이 9

A

a

qu {ru

(3.48)

000      0) 200 200
[ a 11> 931 °°, Ay, 921 > a |.

>:
II

식 BATA Ce RM" 는 공간 상관 계수를 정의하는 대칭적 맵핑 Bel(eymmetric

mapping matrix) 혹은 상관-성형 BA(correlation—shaping matrix)= 불리며 다음의 과

AS 통하여 생성된다. 식 (3.46)을 이용하여 상관 PIS 구하면 다음과 같다.

{Ry 68 :하향링크         520
(Ry @R, :상향링크           aia

여기서 @ = Kronocker 곱을 나타낸다. 식 (3.49)의 RS 이용하여 루트 전력 상관 행렬

[은 다음과 같이 주어진다.

~  VR, _ for fieldtype                                 6:50)
R,             for complex type

}관 행렬 는 non-singular 하기 때문에 다음과 같이 Cholesky 또는

여기서 루트 전력 싱
써 대칭적 맵핑 행렬 cS 얻을 수 있다.

Square Root 분해함으로

r=cc’                                  (3.51)

 130



===== PAGE 130 =====
AMJSZt MIMO 채널 모델링

여기서 Ce 기지국의 상관 행렬 #,,와 이동국의 상관 행렬 Ryg o] 복소 PAR 주어
지는 경우에 Cholesky 분해를 통하여 얻을 수 있으며, 실수 전력 상관관계 행렬로 주어지

는 Alo Square Root 분해를 통하여 얻을 수 있다.

2.3.5절에서 소개된 SUL 채널은 MIMO 환경에 적합하게 수정될 수 있다. 2.3.5절에서 주어
공간 상관 계수 Pen 은 실수로 주어졌기 때문에 Square Root 분해를 통하여 CS 구할
ㅇ

. 아래의 MATLAB 프로그램을 사용하여 상관성 있는 MIMO 페이딩 채널을 생성할

> 로
5

function hh=channel coeff (nTx,nRx,N,Rtx,Rrx, type)
correlated Rayleigh MIMO channel coefficient

% Inputs:

%      nTx    : number of transmitters

%      nRxb   : number of receivers

%      N       : legnth of channel matrix

%      Rtx    : correlation vector/matrix of Tx

%               e.g.) (10.5), (1 0.570,5/1]

%      Rrx    : correlation vecotor/matrix of Rx

%      type   : correlation type: 'complex' or 'field'
% Outputs:

%      hh      : NMRx x nTx x N correlated channel

ㅎ uncorrelated Rayleigh fading channel, CN(1,0)
h=sqrt (1/2) * (randn (nTx*nRx,N) +}*randn (nTx*nRx,N)) ;

if nargin<4    6 uncorrelated channel
hh=h;
return;
end
if(isvector(Rtx)) Rtx=toeplitz(Rtx); end
if (isvector(Rrx)) Rrx=toeplitz(Rrx); end

으

% narrow band correlation coefficient
if (strcmp (type, 'complex'))

C=chol (kron(Rtx, Rrx)) ';      % complex correlation
else

C=sqrtm(sqrt (kron(Rtx,Rrx))); % power(field) correlation
end

131



===== PAGE 131 =====
PART 1 _무선 채널 모델링과 MATLAB

[0

% apply correlation to channel matrix
hh=zeros (nRx,nTx,N) ;

£6¥ Li=12N
tmp=C*h/( +, 11)
hh(:,:,11)=reshape (tmp,nRx,nTx) ;
end

:를 프로그램 3.1 상관성 있는 MIMO 페이딩 채널 생성 St

+

(09 I-METRA MIMO 채널 모델링 기법

I-METRA(Intelligent Multi-element Transmit and Receive Antennas) MIMO 채널
모델링 기법은 통계적 MIMO 채널 4a\(stochastic MIMO channel model) 사용하여
NokiaS 포함한 5개 회사 및 대학교가 컨소시엄을 구성하여 진행한 프로젝트의 결과물이
다[52]. I-METRA MIMO 채널 모델링 기법은 앞서 설명한 Uniform, Truncated
Gaussian, Truncated Laplacian2] PASS 갖는 단일 또는 다중 클러스터로 수신되는 ULA
(Uniform Linear Array)2] 공간 AES 유도하고, 이를 이용하여 상관성 있는 MIMO 채
널을 생성한다. I-METRA MIMO 채널에서는 174008[660 Gaussian, Truncated Laplacian
PAS 모델을 Gaussian PAS, Laplacian PASS 간략화하여 표기한다.

(1) 채널 모델링 절차

I-METRAO| 의해 제안된 MIMO 채널 모델링은 그림 3.14에 나타난 바와 같이 두 단
계에 걸쳐 이루어진다. AL 번째 단계에서 기지국과 이동국 안테나의 수, 안테나간 간격
클러스터의 수, PAS, AS, AoA SS 입력받아 기지국과 이동국의 상관관계 행렬과 정규
화 요소 SS 구한다. 기지국과 이동국의 상관관계 BSS 이용하여 상향링크 또는 하
링크의 공간 상관관계 행렬을 구한다. 두 번째 단계에서는 공간 상관 행렬로부터 대칭
행렬을 구한 후, 상관관계가 없는 페이딩 Also] 각 경로의 전력과 대칭적 맵핑 행렬
여 상관관계가 있는 채널을 생성한다.

개

Bh

0
al

Ol

[02

es

그림 3.15% 위와 같은 과정으로 이루어지는 MIMO 채널의 기능 BEES 보여준
이 그림에 나타난 바와 같이 미리 정해진 도플러 스펙트럼에 따라 상관성이 없는 Hels
채널이 생성되고, 여기에 공간 상관 맵핑 행렬이 곱해져 상관성이 있는 Hols aso] 생

성된다. 그 후 각 경로의 평균 전력과 지연 특성에 맞게 설계된 FIR = 통과하여 주
어진 21#에 따른 상관관계가 있는 페이딩 채널을 생성한다. 또한, 조정 Px(steering
matrix) 생성하여 안테나의 방사 패턴을 조정할 수 있다.

132


===== PAGE 132 =====
제3장_ MiMO 채널 모델링

number of antenna
antenna spacing
cluster
PAS
AoA, AS

M

:           Phase 1
BS and MS correlation | spatial correlation
matrix

matrix generation

R, Q, sigma
+

Spatial correlation
matrix
R=kron(Res,Rus): down
“R=kron(Res,Rus): UD

Symmetrical mapping
matrix                           Phase 2

Correlation fading
CC'=sart(R)             signal generation

Uncorrelated
<———__ fading signal

a

correlated signal matrix

A=sart(p)Ca

그림 3.14 I-METRA MIMO 채널 모델링 절

Delay Profile

3                     Optional
N MS antennas           CHS                     >                        M BS antennas
Steering matrix                  99091:
00                                                                 Power Profile

Xx                   Spatial correlation                          Ras
*                    mapping matrix

Rus
Fading
Charateristics

그림 3.15 I-METRA MIMO 채널 모델의 기능 블록도

133 _



===== PAGE 133 =====
PART 1 _무선 채널 모델링과 MATLAB

(2) 페이딩 채널 생성 및 도플러 스펙트럼

독립적인 페이딩 생성 방법은 5150 채널 모델에 사용된 다양한 모델링 방식을 이용할
수 있다. 그러나, I-METRA MIMO 채널에서 기본적으로 제공하는 도플러 스펙트럼은
Flat, Classical, Laplacian 등이므로, FWGN 채널 모델링 기법과 같은 다양한 도플러 A

펙트럼을 생성할 수 있는 채널 모델링 기법이 적합하다. 또한, 사용자의 필요에 따라
I-METRA MIMO 채널을 수정하여 다양한 도플러 스펙트럼 모델이 적용된 MIMO 채널
을 생성할 수 있다.

(3) Rician 페이딩

SISO 채널 모델의 Rician 페이딩과 달리 MIMO 채널의 경우에는 안테나간 LOS 경로
의 위상 변화가 발생하기 때문에 이를 반영할 필요가 있다. 그림 3.16에서 보는 바와 같이
LOS7} 존재하는 경우에 직접 수신된 신호와 지연 산란자에 의해 산란되어 수신된 신호의
전력비에 따라 가중치가 가해진 두 행렬의 합으로 Mays 수 있으며, A 번째 경로의
Rician ASS 위한 행렬 HS 다음과 같이 표현된다.

H, = VK JP Hos + 1, 00"                                     (3.52)

여기서 (은 첫 번째 경로의 평균 전력을 나타내며, & 는 LOSS} Rayleigh 항의 전력비
를 나타낸다. 또한, 0768 는 LOS 성분을 나타내며 다음과 같이 정의된다.

1               1

pone sin( AoAp, )                     2220 402.)
‘                 @
0 =e"                .                :                .                                       (3.53)

j2n"®(M—)sin(Aodp,)          j2xB(y-I)sing AoDs,)

(a         é

여기서 도플러 주파수는 fy =veos(a)/A 로 주어지며, 는 그림 3.160] 나타난 바와 같
이 이동국의 이동방향([201:60000-0[-407601606 DoM)z} LOS 성분 사이의 각도를 의미
하고, &00는 Angle—of—DepartureS 의미한다. 8768 은 크기가 1이고 404에 따른 위상

을 원소로 구성된 행렬에 67"? 을 곱하여 구성한다.

134



===== PAGE 134 =====
제3장_ MIMO 채널 모델링

.             scatter                    Direction of motion
j-th          _@_                         of the mobile
multipath _^     ~
^                               &

BS         LOS path
그림 3.46 MIMO 채널 환경에서 Rician 채널의 수신 신호 모델

(4) BA(Steering) 행렬

입사되는 BES] 평균 DoA(Direction—of—Arrival)7} broadside7} 아닐 경우(06=0 )에
두 안테나 사이의 위상차는 90(0) 에 비례하여 발생되며 안테나 방사 패턴에 의한 위상
변화가 발생한다. 여기서 는 DoAS 나타낸다. 현재까지는 상관행렬과 페이딩 신호를
생성하는 방식에 관해서만 기술했기 때문에 이에 대한 고려가 없었으나, Way
(beamforming) 시스템과 같이 안테나간 위상차를 기반으로 빔을 형성하는 경우에는 반드
시 필요하다. AAS} 204의 차이를 요약하면, 40ㅅ는 분해할 수 없는 다중 경로 각각의
입사각을 의미하며, DoAE 이들 404&의 평균 AoAS 의미한다.

그림 3.17은 평균 004에 의한 영향을 보여준다. 그림 3.1700)는 모든 지역 산란자들이
이동국 근처에 위치하고 있어 기지국에 입사되는 BEE Felst DoAS 좁은 입사각을 갖
는 시나리오를 보여준다. 그림 3.1706)는 평균 004에 의한 위상 변화를 보여준다. DoA7}
0°°] 아닌 경우에 인접 안테나에 수신되는 신호는 T= dsin(g)/c WSO] 시간 지연이 발
생하며, 이로 인하여 위상 차이가 발생한다. 그림 3.17에서와 같이 기지국에서의 평균
DoA7} 0“이 아닌 경우(@,, #0"), 상향링크에서 수신되는 ASL 다음과 같이 나타낼 수
있다.

y(0) = W(P,s) [H(2)s(¢ -2007                       (3.54)

여기서 조정 대각 행렬(66008 diagonal matrix)2 다음과 같이 주어진다.

(600 O -- 0
0     eo  0

\(00=| .  ae |.        (3.55)
0     0   Wy) Janay



===== PAGE 135 =====
PART 1 _무선 채널 모델링과 MATLAB

MS antennas

Local                     N-elements

scatter

Mean DoA Broadside

BS antennas ©
ici                ©         Mean DoA            {
Broadside           M-elements      :     \                 Broadside

Mean DoA

BS antennas
M-elements

= dsin(y

기지국에 입사되는 평균 DoA              (b) 평균 204에 따른 위상 변화
그림 3.17 평균 004의 영향

여기서 ,(00 는 입사되는 필드의 평균 004가 라는 가정하에서 첫 번째 안테나에
대한 상대적인 평균 위상 천이를 나타낸다. 안테나간 간격이 d 인 01^에 대하여 \,(@)
는 다음과 같이 주어진다.

(0) = /(0)6 7707000500                                          (3.56)

여기서 7,() 는 번째 안테나의 복소 방사 패턴을 나타낸다. 식 (3.56)은 204에 의
한 안테나간 위상차와 안테나 방사패턴에 의한 위상차가 결합된 형태로 표현된다. 만일
안테나 배열에서 신호들이 통계적으로 독립적(안테나간의 상관이 0)이라면 안테나 사이의
위상 변화가 임의적으로 발생된다. 이러한 경우에는 굳이 평균 DoAS 정의하여 조정 행

을 추가할 필요가 없다.

 3GPPo] 제안된 MIMO 채널 모델

다양한 MIMO 기법들의 성능을 비교ㆍ검증하기 위해서 Lucent—Nokia7} 308##에 제안
한 I-METRA MIMO 채널의 파라미터가 표 3.3에 주어져 있다. Case AE 모든 안테나
사이에 영의 상관을 갖는 주파수 비선택적인 Rayleigh 페이딩 환경을 나타내며, 간단한
참고 모델로 사용된다. Case 8와 Case CE 서로 다른 지연 확산을 갖는 ABA! urban
매크로셀 환경을 모델링하며, 모든 지연 성분이 동일한 AOAS 갖는다. 마지막으로, Case
는 마이크로셀과 bad urban HAS 모델링하며, 각 지연성분들은 서로 다른 AoAS 갖

136



===== PAGE 136 =====
1
2

) Case 8, Case 0의 경우에 모든 지연신호의 AoAE 동일한
) Case DE] 경우에 6개의 다중경로에 따라 다른 AoA} 적용된
는 AoA=312! AoA 갖는

제3장_버40

4£ 3.3 _3060에 제안된 I-METRA MIMO 채널 모델의 파라미터

1                                 4                 |                      6                                         6

es 래이     N/A      ITU Pedestrian A ITU Vehicular A    ITU Pedestrian B
Doppler spectrum —   Classical        Classical         .  Laplacian           Laplacian
20 Speed{km/h)   3/40/120        3/40/120           3/40/120            3/40/120
Topology              N/A                       0. 5Aspacing                      0. 5Aspacing                       0. 5Aspacing
Path #1, Rician,   pore   Koti’ Gag hae eas
N/A                이오              ap acian, AS=            P acian, AS=
/               (Uniform over 360) (Uniform over 360)
Uniform over 360
an                es               5
22.5 (odd paths)
N/A              22.5            67.5 (all path
posses)       /                :              2 tet path)    -67.5 (even paths)
ULA:              ULA:               ULA:
N/A      1) 0,5Aspacing  1) 0,5Aspacing     1) 0,5Aspacing
2) 4.0\spacing 2) 4, OAspacing     2) 4,0Aspacing
. 0    N/A     Laplacian, AS=5 ㆍ Laplacian, AS=10   Laplacian, AS=15
. ~      N/A            20,50”              20,50”        2,-20,10,-8,-3, 31”

다. 이 때, AOAE 200} 508 고려한다.

이
다. 즉, 첫 번째 SLE AoA=2, 여섯 번째 경로
는다. 기본적으로 모든 채널 GL Rayleigh 페이딩을 가정하지만, LOS7+ 존재하는 경우
를 모델링하기 위해서 Case 8와 Case CE 첫 번째 AHS Rician 페이딩으로 선택할 수
있다. 한편, Case 8 는 ITU Pedestrian A, Case C ITU Vehicular A, Case 2는 ITU
Pedestrian B2] PDPS 갖는다.

3£ 3.304] 주어진 MIMO 채널 모델에서 송ㆍ수신 안테나가 각각 4개이고, 안테나 간격
이 0.54 일 때, 기지국과 이동국에서의 복소 상관 계수는 다음과 같다.

(1) Case B

7\A\=-=& Laplacian PAS, AS=5°, AoA =20°, 이동국은 Uniform PAS, AoA = 22.5°

137


===== PAGE 137 =====
모델링과 MATLAB

ㅣ        0.4640+ j0.8499 -0.4802+ j0.7421 _-0.7688- 0.0625
0.4640 — 70.8499    1    0.4640+ j0.8499 —0.4802 + j0.7421
| 9.4802 0.7421 0.4640 — 0.8499     1     0.4640 + j0.8499   ay)
—0.7688 + j0.0625 -0.4802— 0.7421 0.4640 — 70.8499        1
1 -0,3043 0.2203 -0.1812
-0.3043 1 0.3043 0.2203
“| 0.2203 -0.3048 1 = -0.3043           (3.58)
-0.1812 0.2203 -0.3043 1

(2) Case C

7|zA\2-— Laplacian PAS, AS=10°, AoA=20°, °]-=}-2 Laplacian PAS, AS =35°,
AoA = 67.5°91 경우,

ㅣ                  0.4290+ j0.7766  -0.3642+ j0.5472
| 0.4290- 70.7766                  ㅣ                  0.4290 + /70.7766

5S “| 0.3642 — j0.5472 0.4290 j0.7766                  ㅣ
-0.4527+ j0.0521

-0.4527- j0.0521
-0.3642+ j0.5472
0.464+ /0.8499

-0.3642- j0.5472 0.4290 - 70.7766                   1

(3.59)

ㅣ                   -0.6906+ j0.3419 0.4903 — /0.3626
_ | -0.6906 — j0.3419                ㅣ

MS ~

-0.3733+ j0.3450

~0.6906 + 0.3419 0.4903 — 0.3626
0.4903 + 0.3626 0.6906 — j0.3419                  1                  -0.6906+ 70.3419

-0.3733- /0.3450 _ 0.4903+ /0.3626  -0.6906- 0.3419                  1

(3.60)

(3) Case D
기지국은 Laplacian PAS, AS = 15°, AoA = 2°, 0|-5s1-2 Laplacian PAS, AS = 35?이고,

짝수 번째 경로의 AoA =22.5°, 홀수 번째 경로의 40&= -67.5ㅇ인 경우

OTs

1                0.7544+ j0.0829
0.7544 — /0.0829                1

0.4109 + 70.0938
0.7544 + j0.0829

0.2313 + j0.0803 |
0.4109 + 70.0938

BS

0.4109 — 70.0938
| 0.2313 — 70.0803
「           1

0.0819 — 70.4267
~ | -0.0719 = 70.0124
| -0.0863 — 70.0124

 138

0.7544- j0.0829
0.4109 — 70.0938

0.0819 + j0.4267
1
0.0819 — 70.4267
0.0719 — j0.0124

1
0.7544 — /0.0829

0.0719 + 0.0124
0.0819 + j0.4267
1
0.0819 — j0.4267

0.7544 + 70.0829          Pal

1              a
—0.0863 + 70.0124 |
—0.0719 + 70.0124
0.0819 + j0.4267
1

(3.62)



===== PAGE 138 =====
제3장_ 140 채널 모델링

식 (3.57)에서 A] (3.62)을 통하여 알 수 있듯이, 기지국에서의 복소 상관 계수는 AS7}
가장 작은 Case B7} 가장 크며, Case D7} 가장 작다. 반면, 이동국에서의 복소 상관 계수
는 Uniform PASS 갖는 0886 B7} 가장 작다.

그림 3.18에서 그림 3.21은 1-4878#ㅅ에서 제공하는 MATLAB 프로그램을 이용하여
두 개의 송신 안테나와 두 개의 수신 안테나를 갖는 Case 의 하향링크를 모의실험한 결
과이다[52]. 이 때 이동국의 SEE 12007이다. 그림 3.18은 각 안테나 사이의 채널 이
득이 시간에 따라 변화하는 것을 나타낸다. 그림 3.19는 각 안테나 사이에 형성된 채널의
평균 20『(원으로 표시)와 ITU-R Pedestrain ㅅ의 이상적인 2[0『(네모로 표시)를 나타낸
다. 그림 3.20은 각 안테나 사이에 형성된 채널의 지연 경로간 상관관계를 나타낸다. 그
림 3.21은 각 안테나 사이에 형성된 채널의 도플러 스펙트럼을 나타내며, 첫 번째 경로는
K= 608인 Rician 페이딩이기 때문에 Laplacian 도플러 스펙트럼이 형성되고, 다른 경로
는 Classical 도플러 스펙트럼이 형성됨을 알 수 있다.

Tx#1 - Rx#1                                     Tx#1 - Rx#2

'       {       {       '
{       i       {       {
i       1       t       {

10°                                               10° te ea amt mem oman nao =fe.-----4
}       }       H       {
{       \       }       {

10+                                           10
0 0.002 0.004 0.006 0.008 0.01         0 0.002 0.004 0.006 0.008 0.01
Time [s]                                        Time [s]
Tx#2 — Rx#1                                          Tx#2 - Rx#2
10                                      Ce
107}--                                 108
107        !       !       {       !              107       {       {       {       H
0 0.002 0.004 0.006 0.008 0.01         0 0.002 0.004 0.006 0.008 0.01
Time [s]                                       Time [s]

그림 348 2Tx-2Rx Case B 채널의 시간에 따른 크기 변화

139


===== PAGE 139 =====
PART 1 _무선 채널 모델링과 MATLAB

Tx#1 - Rx#1-SumPDP=1.0072                 Tx#1 - Rx#2-SumPDP=0.97593
On           7            T                      Om            :
아흐하나eee                         |
잉-1아----~뽀여세여6
3 ooSe ceean
| croe
=05 | 개 ee@0
“ey           2           3

로                     :
| memo= =주
g-10 }-----------7배부r도배
Ss yn} ----------@------------Screen
3  8
뜨 -20)}------------4------------B__.......--.
2B f-maenen---—{------------9.-.---------
“305          2          3
Tap index                                                 Tap index

그림 3.19 2Tx-2Rx Case B 채널의 정규화된 PDP

Correlation coefficient

eT) pre

ee ee as

Correlation coefficient

1 2 3 4           1 2 3 4
(k-1)*2+1                        (k-1)*2+1                         (k-1)*2+1                        (k-1)*2+1

그림 3.20 2Tx-2Rx Case 8 채널의 각 Bez 상관계수

140


===== PAGE 140 =====
제3장_ MIMO 채널 모델링

0.2

0                  0                       0                       0
—— 0.04            - 002———                —
0.5} |      |       0.02    |       |       0.01     |       |      0.005       |
—             0                 0                 0

Tap hy,                  Tap hi,                  Tap hi,                  Tap hi,

i        :        0.05 —        0.02ㄷㅠㅜ        !        0.01ㄴㅠㅜ        :

0.5| |       |                  |        |        0.01     !        ' 4 0.005       |
a 2 며 002 002 08 0 2

Tap hi},                  Tap hi,                  Tap hs,                 Tap hi,

0.1                        0.02

05| |    |    0.05       | | 001   |    |  ] 0.005
if    |
os 2 & 0002 8 o 2 %& 02
그림 3.21 2Tx-2Rx Case B 채널에서 각 경로의 도플러 스펙트럼

I-METRA MIMO 채널 모델의 MATLAB 프로그램은 웹사이트에서 다운로드 가능하
다[52].

. scm mimo 채널 모델링 기법

3GPP2} 3GPP2°]A4] 공통적으로 요구되는 MIMO 공간 채널 모델의 파라미터 및 기법
을 규정하고 이를 개발하기 위해 양 진영의 두 AHG(Adhoc Group, 애드혹 그룹)가 joint
SCM-AHGS 결성하였으며, 이 SCM-AHGo}] 의하여 개발된 채널 모델이 SCM(Spatial
Channel Model)°]t}[40][53]. SCM 채널 모델은 Ray 기반의 모델로서 2.3.3절에서 설명
한 바와 같이 SISO 채널 모델링으로 사용되기도 하지만, MIMO 채널 모델링에 더욱 장
점이 많은 모델이다. Ray 기반의 MIMO 채널 모델은 222, PAS, 안테나 배열 구조에 기

반을 두고 subray 성분을 SANA 생성하며, 다음과 같은 장점을 갖는다.

MIMO 채널의 통계적 특성을 직접적으로 모델링할 수 있다.

* 시간, 공간, 주파수영역에서의 SAA 특성을 유지시킬 수 있다.

141


===== PAGE 141 =====
PART 1 _무선 채널 모델링과 MATLAB

* 비교적 간단히 실행 가능하다.

ㆍ 다양한 PDPS} 『45에 대하여 유연하게 적용할 수 있다.

ㆍ LOSS} NLOS 채널을 지원할 수 있다.

ㆍ 채널 행렬 Ho] 유효 랭크는 경로 당 subray 의 숫자 Moy 의존한다.

600 SCM 링크 레벨 채널 파라미터

SCM] 규정하고 있는 링크 레벨 채널 모델은 어떤 채널의 스냄샷(6080-5000만을
나타내기 때문에 교정(6811008000)용으로 사용할 것을 추천하며, 시스템 레벨 시뮬레이션
이 궁극적인 목표이다. SCM 링크 레벨 채널 모델과 I-METRA 채널 WAS 거의 유사한
파라미터를 사용한다.

표 3.4는 SCM 링크 레벨 채널 모델의 파라미터를 보여준다. 이 Hol] 나타난 바와 같이
SCM 모델은 3GPP2} 3GPP22] 기존 MIMO 모델을 반영하고 있으며, 안테나 배열 구조
는 기본적으로 ULA(Uniform Linear Array) 가정한다.

기지국의 PAS Laplaican 분포로 다음과 같이 안테나 이득이 곱해진 상태로 정의된다.

_   -V2|0-8|
P(0,0,0)=N,e 060)          (3.63)

여기서 0는 AoD(Angle of Depature)S 의미하며, 0는 AoD 0에서 출발하는 94618*의
출발각을 의미한다. 또한, 는 RMS 각 확산(40816 8507680)을 의미하며, 2(0)는 기지국의
안테나 이득을 나타낸다. N= 정규화 상수를 나타내며 다음과 같이 주어진다.

자06 ㆍ -1210-0|

= ] ㅇ ㆍ 06006,   -2+0ㄴ60ㄴㅋ2+0     (3.64)

-1+0

그
N,

기지국의 경우에 3-섹터 또는 6-섹터의 섹터 안테나를 사용할 수 있기 때문에 그림
3.22에 나타난 바와 같이 PASS 계산함에 있어 안테나 이득이 반영되어야 한다. 기지국
의 안테나 패턴은 다음과 같이 주어진다.

3dB

4o)=-mio | 시 [dB], for -180' < @< -180°      (3.65)

142


===== PAGE 142 =====
제3장_ MIMO 채널 모델링

#34 SCM 링크 레벨 채널 모델의 파라미터
Cc       di
3 ae bee           Case B               Case C           Case D       Case A
지구: ~       Model A, 2, E           Model C         Model B      Model F
PDP           Modified Pedestrian A       Vehicular A       Pedestrian B     ee
1) 4+1(LOS on, K = 6dB)
# of Paths      2) A(LOS off)                    6               6            :
1) 0,0                                               |
로 Inf             0        0,0       0       0.0       0      0110
1) -6.51
:              0       =1,0     310     =0:9     200
Relative             고 2.8 91                        |
Path     Delay    2) -9 7            110      -9 0     710     -489     800
Power     (ns)     1) 98 74
(dB)                 2) -19 >              190       —10,0     1090      -8.0      1200
1) -29,31                  |                     é
: 29 8         410     on)    1730    -08    2300
he                      -20.0 2510 -23.9 3700
Speed (km/h)    : a 120                3, |30, 120       35°80, 120)       3
Topology       Reference 0,5A         Reference 0,5A    Reference 0,5A     N/A
1) LOS on: Fixed AoA for
LOS component, remaining     oe
phwer hs 960: degres      spread of 35    RMS angle spread
cniforer PAS         degrees per path of 35 degrees per
PAS      2) LOS off: PAS soak .    with a Laplacian     path with a      N/A
UE/Mo           Laplacian distribution, RMS    ir see       드니 이
bile             angle spread of 35 degrees ° | P   4 e      eatehu Eon
Station                    por ae            uniform PAS,
DoT
( eee                           0                                      22.5                          ~22.5                  N/A
22.5 (odd
AoA       22.5 (LOS component)                      numbered paths),
(degrees)    67.5 (all other paths)     67.5 (all paths)     -67.5 (even      N/A
numbered paths)
Reference: ULA with
1
도    Topology      0,5A —spacing   or   4, —spacing   or   10A —spacing       Ne
. ig                     Laplacian distribution with RMS angle spread of
Base     PAS                    2 degrees or _ 5 degrees,                    N/A
Skation                           per path depending on AoA/AoD
AoD/AoA              50° for 2° RMS angle spread per path                N/A
(degrees)              20° for 5° RMS angle spread per path
NOTE : *Designators correspond to channel models previously proposed in 3GPP and 3GPP2

ad-hoc groups,

143



===== PAGE 143 =====
PART 1 _무선 채널 모델링과 MATLAB

Total PAS
Laplacian PAS : AoA=22.5°, AS=35°
1.2|-                  /      Antenna Gain : 6.6=70", Am=20dB
.                                            —— Total PAS : PAS x Antenna Gain
1
'S
208
=
fo)
2 0.6
‘a.
0.4}--
0.2[--
나          0          50         100
0 [degree]

그림 3.22 안테나 이득이 반영된 PAS

여기서 Pap 와 4, 2 각각 308 빔폭과 최대 366008000 값을 의미한다. 이러한 경우에
안테나 이득은 0(0)=10"“"""로 정의된다. 3-섹터의 경우에는 0,,,= 70°, A, = 2008로
안테나 이득은 14081이고, 6-섹터의 경우에는 4,,,= 35°, 4,,= 23dBH 안테나 이득은
17081이다.

반면에, 이동국의 PASSE Laplacian 또는 Uniform 모델이 사용되며, 이동국의 안테나
는 이득이 -1001인 전방향성 안테나를 사용하기 때문에 안테나 이득에 대한 고려없이
PAS7} 주어진다. Laplacian 『ㅁ48에 대한 식은 다음과 같이 주어진다.

-v2\0-6|

P(0,0,0)=N,e ° ,  -x+0<0<n+0      (3.66)

여기서 0는 AOAS 의미한다. 이 때 정규화 상수는 다음과 같이 계산된다.

m+0 -/210-0|

그 = fe 더 do =\20(1-e**"")        (3.67)

o -2+0

Uniform 『45에 대한 식은 다음과 같이 주어진다.

144


===== PAGE 144 =====
제3장_ MIMO 채널 모델링

P(0,0,0)=N,,.1,      -30+0<0<V30+0         (3.68)

여기서 정규화 ARSE ON, =1/2V30 로 주어진다.

EP) scm 링크 레벨 채널 모델링 기법
그림 3.23은 Ray 기반의 SCM 링크 레벨 채널 모델의 실행 절차를 보여준다. 먼저 링
크 레벨 모델과 각 채널 모델의 파라미터를 선택하고, 주어진 PASS 갖는 채널을 생성하
기 an 동일 전력 bead 방식 또는 이산화된 Laplacian 방식 중의 하나를 선택하여 Zt
식을 정한다. 선정된 방식에 따라 각 subray2] AoA,
랜덤 ote }을 선택한 호 송신부와 수신부 사이에 각 subrayS 임의의 쌍으로 연결한다. 주
}식에 대해서는 2.3.3절에서 자세히 기술하였으므로
여기서는 설명을 생략한다. 최종적으로 이동국의 이동 속도 및 이동 방향을 입력받아 각
|         sl         3.24 Ray 기반 SCM 모델의 WRS 보여준다.

Al 안테나를 가정할 때, 6 번째 송신 안테나와 u 번째

경로의 HAS 다음과 같이 표현된다.

n—th Path 좋: MBS      Phase dueto | | MS     Phase due to         (3.69)
Poul                   Power                      PAS } | BS Array                 PAS } | MS Array                                ：
여기서 MS 경로당 전체 subray2] 수를 나타낸다. 동일 전력 94618 방식을 사용하는 경

우에 채널은 다음과 같이 주어진다.

Gps (~ ) exp (i Aa, sin a ) a Dn |)
iyagl= =X) Om (Banas) €%P( 50 Oc, ,))               6.70

m=1
에005(6 사개 에  -0)/)

exp(Jk_|

여기서  k=277/ 2 이며,   8, m,Aod Sf  9, m,AoA X= 릭각 번째 경로의 m 번째 subray ©] AoD$}
AoAS 의미한다. 또한, ®,,, 2+ Ot 각각 7번째 경로의 mA subray2] 랜덤 위상과
이동국의 DoT(Direction of 118181)을 의미한다. |네는 속도 벡터의 2007을 의미한다.



===== PAGE 145 =====
PART 1 무선 채널 모델링과 MATLAB

1. Choose LL Model

2. Generates parameters

3. Generates channel
_ coefficients

그림 3.23 SCM 링크 레벨 채널 모델의 실행 절차

06.~400 MS array broadside                 |

\                 as                       \                                              MS direction
ㅣ
ㅣ
1

BS array broadside                          of travel

그림 3.24 Ray 기반 SCM 모델의 개요

146


===== PAGE 146 =====
제3장_ MIMO 채널 모델링

이산화된 Laplacian 방식을 사용하는 경우에는 각 ray] PAS7} 고려되어 다음 식으로

주어진다.

Bs (9, m,AoD ) Gps (6 ) exp 11 810 = ) +, |)

h(t) = JED) Bs  (An. so ) Gus (rm. sox) &XP( Jkd, Sin (8, », 404 ))       (3.71)
©08 (Ayn, tos =; )t)

xexp( jk |v|

으 AlO

마지막으로 LOST} 존재하는 Rician 채널의 경우에는 다음 식으로 주어진다.

Gps Gps (Op) exp  ( jkd,  sin(O,s ))x

he =  le     pelt + J    Gas (us)  ) exp( Jkd, sin(ys) + Pos )X
(3. 22)

exp (jk |p| cos(Oy5 6, )t)

hee, (t) = ahi (t),                                 forn#1

여기서 K 는 Rician factorS 의미한다. 위의 식에 나타난 바와 같이 첫 번째 경로에 하나
의 946085에만 LOS7} 적용되기 때문에 첫 번째 경로 이외에는 A] (3.70) 또는 식 (3.71)
을 그대로 적용할 수 있다.

06668 Ray 기반 Sao) 공간 상관
그림 3.25에 나타난 바와 같이 전형적인 0Ｌㅅ에서 0번째 안테나와 거리 duke 떨어진

| 뜨거

안테나 사이의 상관은 다음과 같이 주어진다.

P(A) = ELA, (OM, wn OI]
ㅅ j2ndsin(@)                      (3.73)
= ㅣ e * P(6)d0

-

안테나 이득에 대한 고려가 없는 Laplacian PAS 경우의 공간 상관에 대
는 식 (3.33)과 식 (3.34)에 주어져 있다. 한편, 각 subraySo] 동일한 전력
에 식 (3.73)은 다음과 같이 간략화 될 수 있다.



===== PAGE 147 =====
PART 1 _ 무선 채널 모델링과 MATLAB

/2009069.6. 0

Pseu (d) =    we                                     (3.74)

Propagation
AoA 0 ,    , Waves,

va    a, “      4      ¥

…ㄴ이Serre Serer) peer) peer
Antenna
spacing, d

그림 3.25 ULA 안테나의 수신 신호

여기서 각 subray2] AoAE 평균 404&를 중심으로 ^4,...0/의 옵셋으로 주어지며,
Ann tor = 9 + Ann, 로 정의된다.

그림 3.262 동일 AA subray 방식을 사용한 경우에 AoA} 안테나간 간격에 따른 공
간 상관값의 변화를 보여준다. 이 그림으로부터 48가 커질수록 상관값이 감소하고, 안터
나간 간격이 넓을수록 상관값은 감소하는 것을 알 수 있다. 또한, 같은 안테나간 간격에서
도 AoA7} £90°9] 경우에는 Zt 안테나가 거   ~ wave-frontS 경험하기 때문에 상관
값이 1에 oh 0*에 근접할수록 상관값이 감소한다. 그림 3.270] 나타난 바와 같이
AoA7} £90°°] 31    were 간격이 272 인 경우에 공간 상관값이 1°] 된다.

만일 이동국이 oles    을 하게 되면, 도플러 지연 확산이 발생하여 채널의 계수가 시간에
따라 변화하게 된다. 그림 3.28은 이동 속도와 DoT] 따른 안테나간 위상차를 보여준다.
이 경우의 시간 AK temporal 000ㅁ13000)을 『ㅁ4ㅅ8로부터 직접 해석적으로 유도하기는 어
렵지만, 동일 A subray?] 경우에는 다음과 같이 유도가 가능하다.

=

걸어

Pre) = Vig EFT) Moun Ol]
1 Z2etlllleos(Oh m.soa~ 8)           (G.75)

=—)Jie     a

여기서 0, 와 |끼는 이동국의 이동방향001)과 이동속도의 크기를 나타낸다. 만일 그림
3.29(6)에 나타난 바와 같이 DoT 6,=90°°] 경우에는 시간 상관과 공간 상관이 다음 식에
서와 같이 동일하게 주어진다.

148



===== PAGE 148 =====
..[p]

Correlation Mag.

1.01
1.005

0.995
0.99
0.985
0.98
0.975
0.97
0,965
0.96

Correlation Mag...[p]

0.2

Pepe m,dod 9.)

whe

d=t|| 1 슨

27/(00=ㅡ

4

M m=1

é

Spatial Correlation Magnitude (spacing d/A=0.5)

—o=

20
5°

은
©

은
a

은
「

60         0          50
Mean AoA [degree]

(a) 404에 따른 공간 AH (d/A =0,5)

Spatial Correlation Magnitude (spacing 0/1 =0.5)

— o=2
—o=5

100     150

-150 -10 -50    0    50    100
Mean AoA [degree]
) AoA] 따른 공간 At (d/A =10)

그림 3.26 AoA} 안테나간 간격에 따른 공간

722090(6, 404)

Correlation Mag...[p]

Correlation Mag...[p]
eeees

제3장_ MIMO 채널 모델링

1 vw j2at\\v||sin(8, mm 404)
—)'e     4
M m=l
(3.76)
SCM (d)

So 은 은 호 돈
Oo 62 f+ Nn DN WD ©

01

ar

은
ie)

O.1}-

Spatial Correlation Magnitude (Mean AoA=20°)

123 4 5 6 7 8 9
Normalized Antenna Spacing, d/A

(b) 0/2에 다른 공간 상관 (06=809)

Spatial Correlation 버지 005 i AoA=67. Py

10

aD

[ee

1     z.    3    4    5    6    7    8    9

10
Normalized Antenna Spacing, d/A
(0) d/Ao] 다른 공간 상관 (0=67.59)
상관
149


===== PAGE 149 =====
PART 1 _무선 채널 모델링과 MATLAB

Propagation
waves
AoA
0=0
Wave
front
[+>
Antenna
spacing, d
(a) 0=0°

그림 3.27 AoA7} 극단적인

Broadside
AoA @

If d is multiple wavelenath/2,
spatial correlation is about 1

AoA 6 = 90°                        Propagation
7                                waves
wane『 |            =                       <—__------
Endfire
Antenna
spacing, d
06) 8=90°
경우의 공간 상관
Propagation
waves

ll v llFeos (6-9

(a) 이동에 따른 안테나간 위상차

Direction of mobile
movement

(b) 안테나간 위상차 (DoT=90°)

그림 3.28 이동 속도와 001에 따른 안테나간 위상차

Temporal Correlation Magnitude (Mean AoA=22.5°, =35°)               Temporal Correlation Magnitude (Mean AoA=67.5°, =35°)
a:                                 — DoT, 0,=0"                  ㄷㄷ Fors             — DoT, 0)=0"
09                                   DoT, 6, =30°     ool -}-----2    :           —       DoT, 0,=309
|       |       |                     — DoT, 0,=60"                  |                                   | | ㅡ- DoT, 0,=60"
08     a      ‘      ~ | - DOL, Oy= 90)       08|-                                    {      == DON, y= 90°}
‘ o7}--                             가     o7}--\s
3                                       {    |      3
0.6;--                                 t    t        0.6} --
등 05}---            descent       아흐 OS)           :
꼬                                            !     3         !
8                                                                                   fo}                            th              {       |
0              {    |    .    !    |    {         0             :    {    :    :
0 05 1 15 2 25 38 385 4 45 5     0 05 1 15 2 25 3 35 4 45 5
Normalized Distance Traveled,                                         Normalized Distance Traveled,
(a) 6=22.5°                                       (b) 0=67,5°
그림 3.29 이동거리에 따른 시간 상관 (AS=35°)

150



===== PAGE 150 =====
제3장_ MIMO 채널 모델링

그림 3.29는 이동거리에 따른 시간 상관의 변화를 보여준다. 이 그림으로부터 0-@, 가
작을 수록 상관값이 증가함을 알 수 있다.

표 3.5는 링크 레벨 채널 모의실험의 결과로 SCM Texto] 주어진 참조 상관치와 비교
하여 보여준다. 표 3.5의 1)은 SCM Texto] 주어진 참조용 상관치이며, 2)는 식 (3.73)을
사용하여 Laplacian PASS 수치 적분한 결과이며, 3)은 식 (3.74)를 근사화한 이산 적분
결과이다. 또한, 4)는 주어진 옵셋각을 사용하여 Ray 기반의 채널 모델링 기법을 통하여
모의실험으로 생성한 채널의 상관 계수이다. 표 3.5로부터 알 수 있듯이 SCM 모델은 동
일한 AAS 갖는 20개의 subray= Laplacian PASS 근사화 하였기 때문에 상관 계수가
큰 경우에는 모의실험 결과와 거의 일치하나 상관 계수가 0.3이하가 되면 참조 상관 계수
와 차이가 커진다.

표 3.5 링크 레벨 SCM MIMO 채널 모델의 모의실험 결과

5            fj                   0,9683 0,4640+0,8499i 0,9676 0,4640+0,8491i 0.9678  — 4652+0,8487i
2 50 (0.9975) =0,7367+0,6725i 0,9975 -0,7390+0,6700i 0,9975 -0,7390+0,6700i 0,9976 -0,7388+0,6703i
B           5 20 (0)B22M 0, 214440, 31581 0.3198 -0,2203+0,2318i 0,1968 -—0,1433+0,1350i 0,2008 -0,1434+0,1406i
8             2 50 (0) 862d 0.8025+0.958. 0.8691 0,7954+0,3350i 0.8530 0,7872+0,3285i 0.8541 0,7801+0,3268i
5 20   > 06000 0,5020 -0,0619+0,0327i 0,0708 -0,0590+0,0391i 0,0655 -0,0529+0,0386i

0,0700 -0,2615—-0,4285i 0,3858 -0,1933-0,3339i 0,3885 -0,1972-0,3347i

M                          -67.5                            0.7771 0,6966-0, 84451  0.7826 -0.6824+0.86971 0.7318 —0,6310+0,3696i

8   0.5    85 22,5 04800 0.08640.494 0.4307 0,0858+0,4312i 0.3426 0,0288+0,3418i 0.3304 0,0227+0,3386i
0.5     35 67,5 00044 0.694840, 8421 0,771 -0,6966+0.3445i 0.7326 -0,6324+0,3697i 0.7313 -0.6810+0.86961

SCM 채널 모델의 MATLAB 프로그램은 웹사이트에서 다운로드 가능하다[54].

(E20 601-ㄷ mimo ae !

5MHz 대역폭으로 제한된 3GPP SCM 모델을 10, 20, 4OMHz 대역폭을 지향하는 무선
전송 기술의 검증에 사용하기 위해서는 대역폭의 확장이 필요하다. 유럽의 WINNER =
로젝트에서는 이를 위하여 기존의 SCM 모델을 확장하여 최대 10054 대역폭을 수용하
고 5012 대역까지 사용 가능한 SCM-E MIMO 채널 Bale 2005년에 발표하였다[55].



===== PAGE 151 =====
PART 1 무선 채널 모델링과 MATLAB

이 Hale B3G(Beyond 30) 시스템 개발을 위한 잠정 모델로서 11600 BBG 채널 모델
이라고 불리기도 한다.
SCM-E 채널 모델을 기존의 SCM 채널 모델과 비교할 때 주요 변경 부분은 다음과 같다.

ㆍ 2GHz 및 5GHz 대역 사용
ㆍ AU 모델로 JEEE 802.11TGn 모델을 사용

ㆍ 실외용 모델로 3GPP SCMS 기초로 하여 확장한 모델을 사용
ㆍ 대역폭은 5~1008/[로 확장

ㆍ 모델 Ul] time—evolution 기능을 추가

* 모든 시나리오에 LOS 고려

* 렁크 레벨 시뮬레이션을 위한 TOL 모델 제시

실외 환경에서 507 이내의 SCM 경로 손실 FAS suburbany} urban 매크로 환경에서
는 COST-Hata 모델을 사용하였고, urban 마이크로 환경에서는 COST-WI(Walfisch—
Ikegami) 모델을 사용한다[56]. SCM—-E 채널의 50132 대역에서 경로 손실은 2011 대역
에서 제시된 경로 손실 모델에서 808의 AAS 고려하였다.

9634에서는 6개의 다중 경로가 정의되어 있는데 각각의 경로는 동일한 지연 시
는 20개의 5080#로 구성된다. 그러나 8084-에서는 대역폭이 확장되면서 주파
도의 변화를 세밀히 표현하기 위하여 midrayS 정의하여 하나의 다중 경로를 구성
개의 subrayS 표 3.6에서와 같이 3 또는 4 종류로 그룹핑하여 서로 다른 지연 시
여한다. 이는 100MHz 대역폭을 갖는 채널 모델의 생성을 위하여 제안되었다.

SCM 모델에서 생성되는 하나의 무선 채널은 앙상블(60800 또는 0702) 내에서 준정
A 채널(04891-96800 0080061)을 가정한다. 즉, 앙상블 내에서는 채널을 생성시키는 파라
미터가 고정되어 있어 이 구간 동안 채널 파라미터의 시간 변화가 허용되지 않는다. 그러
나, SCM-E2] 경우에는 다중 경로를 표현하는 요소인 지연과 공간 정보가 이동국의 속도
에 따라 변화하도록 되어 있다.

wal
ay ee

lo rir a tho

에

「

ㅁㅁ 8 @ Ww

x

4 3.6 SCM-E Midray Power—Delay 파라미터

3                       4
10/20          0 ns        6/20       0 ns
6/20          7 ns        6/20      5.8 ns
4/20         26.5 ns       4/20     13 5 ns

_ 152

4/20       27.6 ns



===== PAGE 152 =====
A3H_ MIMO 채널 모델링

 ㅣ 1666 802.11 Tan MIMO 채널 Se

IEEE 802.11 TGn(High Throughput Task Group) 채널 모델은 2GHz2} 501 대역의

옥내 무선 LAN 시스템의 성능 ASS 위하여 2004년에 발표되었다[571. 이 모델은 9190
와 MIMO 채널의 협대역 경로 손실 및 광대역 특성을 규정하며, 옥내 전파 환경을 6 종류
로 구분하여 Model A~FS 제공한다. 이 채널 모델의 주요 특징을 요약하면 다음과 같다.

ㆍ MIMO 채널 관점 : 상관 BAS 이용한 안테나간의 공간 상관 개념 도입

ㆍ 광대역 채널 관점 : COST259 모델에 근거한 클러스터 개념 도입

IEEE 802.11 TGn MIMO 채널은 I-METRA MIMO 채널에서와 유사하게 각 송ㆍ수
신 안테나간의 페이딩 채널을 주어진 상관 행렬에 따라 확률적으로 생성한다. 코마 광대
역 특성을 나타내는 다중 경로는 복수의 클러스터를 통하여 생성된다. 이 때 클러스터는
전파 환경에서 어느 정도 동질성을 갖는 다중 경로 그룹이라 할 수 있으며, 각 클러스터는

= 지연 시간을 갖고 한 클러스터 내에서는 동일한 AoA AS BS 갖는다고 가정한다.
또 다른 특징으로 특정 지               = 공간 정보를 갖는 다중 경로가 복수(0801
over—lapping)= 존재할 수 있다는 점이다. 이는 측정 데이터를 통한 경험적인 결과에 근
거하며 클러스터 개념으로 이러한 현상을 잘 설명할 수 있다

실내 환경에서 각 세부 모델별로 1606 point 거리 《,, 가 정의되며, 이 거리 내에서는

간의 경로 손실을 가정한다. Break point 거리는 two-ray 모델에서 반사파가 직접
파에 ZS 일으키는 최소 거리를 나타내며, 송ㆍ수신 안테나의 높이와 반송파 주파수에
따라 영향을 받는다. 경로 손실 외에 실내에서 발생되는 94800\ 페이딩은 4, 에 따라 표
ㅣ 주어지고, 경로 손실은 다음 식으로 주어진다.

|

r& a
=
기
&
=
Hu
무리

PL(d)[4B| = PL, (0)                      d<dyp
PL(a)[ dB] = PL; (dgp) + 35logy, (d/dgp)    d>dpp

IEEE 802.11 TGn 채널 모델의 주요 특징 중의 하나인 상관 YAS 이용한 안테나간의
공간 상관 개념은 3.1절과 3.2절에서 설명되었으며, 클러스터 개념은 2.2.3절에서 자세한
설명이 이루어져 본 절에서는 설명을 생략한다.

153


===== PAGE 153 =====
PART 1 _무선 채널 모델링과 MATLAB

표 37 IEEE 802.11 1067 경로 손실 모델 파라미터

‘Aloptional) 0 5
ㅁ

2                3,5                   3                         4
2                3.5                   3                         4
2                3,5                   3                         9)
10              2                3,5                   3                         ㅁ8
20             2                3,5                   3                         6
30             2                3.5                   3                         6

154



===== PAGE 154 =====
part Ul

OFDM} MATLAB

제4장 OFDM 기초
제5장 동기화 기법
제6장 채널 추정 기법

제7장 PAPR 감쇄 기법

제8장 셀간 간섭 완화 기법


===== PAGE 155 =====
f 411 Seow 반송파 전송 방식

01) 단일 반송파 기저대역 통신 시스템
그림 4.1은 한 개의 반송파만을 이용해서 데이터를 전송하는 단일 반송파 전송 방식의
기저대역 통신 시스템을 보여 준다. 송신 필터를 통해 대역 제한된 송신 심볼 0, 은 채널
을 거쳐 수신단에 전달되고 수신 필터를 통과하게 된다. 수신 필터의 출력 신호 HOE

식 (4.1)과 같이 나타낼 수 있다.

AWGN2z(t)
a                          ve Ei    ~        !    y(t)      y(t, )         a,
oy 5 Transmit Filter | «(t) | channel  skh    Receive Filter | y(t  ee   <        Decision 또
grt)           h(t)             0200          ^ 10)             ：
(T : Symbol Duration)

그림 4.1 단일 반송파 기져대역 통신 시스템

270)=0.8,0)*/40)*8,0)0+ㅜ50)                  (4.1)

여기서 40), 870), 8,0), 0), TE 채널, 송신 필터, 수신 필터, 대역 제한된 백색 잡
음, 심볼 주기를 각각 나타낸다. 이 때 시스템의 전체 응답과 등화기에 의해 보상된 신호
식 (4.2)와 식 (4.3)과 같이 주어진다.

200=8,00*400*8,0)                                  (4.2)
V(t) =H) * (0)                    (4.3)
157


===== PAGE 156 =====
PART Il_ OFDM2Z} MATLAB

위 식으로부터 정확한 심볼 타이밍 t,=n7 에서 샘플링된 수신 ASL 다음 식과 같이
주어진다.

yt, = >: 4.27(0-7020)                        (4.4)

이 때 p(t) 다음 식과 같다.
20)=20)*4'0)=8,0)*8,0)=80)                (4.5)

수신단에서 AS 채널에 대한 정보를 정확히 알고 있으며 잡음이 없는 As 가정한
우에는 채널에 의한 신호의 왜곡은 수신단의 등화기에서 완벽하게 보상될 수 있으므
a 신단 사이에는 송수신 필터에 의한 응답만이 존재하게 된다. 송수신 필터의 응답
gt) 그림 4.2에서 볼 수 있는 바와 같이 연속적으로 전송되는 ae Hoo [S(Inter-
Symbol Interference)S 발생시키게 되는데 심볼 주기에 따라 ISIS] 영향은 크게 달라지게
된다. 그림 4.2(8)에서와 같이 송신 심볼의 주기가 긴 경우 송수신 필터의 임펄스 응답에
의한 ISIE 큰 영향을 미치지 않지만, 그림 4.206)에 나타난 바와 같이 송신 심볼의 송신
주기를 짧게 한 경우에는 191가 크게 발생한다. 즉, 단일 반송파 전송 시 데이터 전송률을
높이기 위해서는 심볼 주기를 짧게 해야 하는데 그에 따라 191의 영향이 커지기 때문에 이

를 고려한 송수신 필터의 설계가 필요하다.

Filter Response       a ae                                                   6           시: Sampling Timing

9 TSK.           en:                7, 7": Symbol Duration (7 > 7’)
|          /}           n+1     wt 1
) “ f * 2 |          Time                 nf PKL          Time
Impulse a                                    aad 7      |

그림 4.2 심볼 주기에 따른 isi 발생

(2) 181와 Nyquist Criterion

정확한 심볼 타이밍에서 샘플링되고 등화기에 의해서 보상
(4.6) 과 같이 송신 신호 a, a 인접 심볼에 의한 간섭으로

수신 신호 6,)음 Al

}된
표현될 수 있다.

158


===== PAGE 157 =====
제4장_야미/ 기초

00

y(t.) = > ap’ ((n=n'\T))=a,g(0) + | ‘a  a,g((n—n'JT))        (4.6)
위 식에서 g(0) 이 1이고 4,8(0) 을 제외한 부분, 즉 오른쪽 항이 0이 될 때 151가 발생
하지 않게 되는데 이 AAS Nyquist 00[6000이라고 부른다[69]. 이 AAS 만족시키기

위한 송수신 필터의 임펄스 응답과 주파수 응답은 다음 식과 같이 주어진다.

1.2=7'
시간영역:      g((n-n =o               (4.7)
7? Fourier 변환
Ay         =      ;           1
주파수영역: >] 0(/-4)=7, 1 -+|                       (4.8)

단일 반송파 AS 시스템에서 데이터 AS SES 높이기 위해 심볼 주기를 짧게 하더
라도 송수신 필터의 응답이 Nyquist criterionS 만족하고 정확한 심볼 타이밍에서 신호가
수신되면 IST 없는 데이터 송수신이 가능하다.

Nyquist criterion 만족하는 시간 및 주파수 SHS 갖는 필터를 Nyquist 필터라고 부
르며, 대표적인 Nyquist 필터로 이상적인 저역 통과 필터를 생각해 볼 수 있다. 이상적인
저역 통과 필터의 주파수 SHS 다음 식과 같이 구형파(66000084180) 함수로 표현되고 시
간영역에서 sine 함수가 된다.

1
GA(f)=       고
0,  >                        (4.9)
= 조} 0 ae
2)    27     2 27

위 식에서 TE 심볼 주기, # 은 Nyquist rate, W 는 Nyquist 대역폭으로 정의된다.

이와 같이 저역 통과 필터를 주파수영역에서 대역 제한할 경우 시간영역에서 무한히 긴
임펄스 응답을 발생시키기 때문에 필터 구현 시 복잡도가 크게 증가하게 되어 실제적인
구현을 위해서는 어느 BES 성능 GAS 감수하고 시간 SAS 길이를 제한하여 사용해
oF 한다. 또한 ISI 없이 ASS 수신하기 위해서는 정확한 심볼 타이밍을 찾아야 하지만
잡음이나 타이밍 지터 등에 의한 타이밍 추정 오차는 항상 존재하게 된다. 이상적인



===== PAGE 158 =====
PART ㅁㅁ _ OFDMZ} MATLAB

Nyquist 필터는 이러한 타이밍 오차에 민감하기 때문에 이상적인 저역 통과 필터를 실제
시스템에 적용하기는 쉽지 않다. 이러한 이상적인 저역 통과 필터의 단점을 보완한
Nyquist 필터가 raised cosine 필터이며, raised cosine 필터의 주파수 응답은 다음 식으로
주어진다.
2.                       Ifls
@00= 210 22   “ie   “)))      sine         (4.10)
l+r
0,                    If >   a

Raised cosine 필터는 왜곡 없는 신호 전송에 필요한 최소한의 FAYZNyquist 대역
보다 더 넓은 ASS 사용하게 되는데, 이 때 사용하는 추가적인 대역폭은 70110 factor
/에 의해 결정된다. 그림 4.3(a)2} (6)에 roll-off factor2] 변화에 t= raised cosine 필터
의 시간영역 응답과 주파수영역 응답이 주어져 있다. 이 그림에서 701101【 factor7} 0인 경
우 이상적인 저역 통과 필터가 되며, 70110 factor7} 1 인 경우에는 대역폭이 Nyquist 대
역폭의 2배를 사용하게 되는 것을 알 수 있다.

그림 4.4는 BPSK 신호 전송 4) rolboff factor2] 변화에 따른 eye 0189180을 보여
데, roll-off factor 값이 증가될수록 타이밍 추정 오차에 대한 민감도가 감소함을 알 수
다. 그림 4.3(a)2} (6)에 나타난 바와 Zo] raised cosine 필터는 이상적인 저역 통과 필터
에 비해 추가적인 대역폭을 사용하지만 시간 응답 특성이 이상적인 저역 통과 필터에 yy
해 현저히 빠르게 0으로 수렴하기 때문에 적은 탭 수로 구현이 가능하며 타이밍 오차에
대한 민감도를 크게 낮출 수 있다.

Squareroot raised cosine 필터 역시 실제 통신 시스템에서 많이 사용되는 대역 제한 필
터이다. 904876700[ raised cosine 필터의 주파수 응답은 다음과 같이 주어진다.

|

+o,

=o
Gseec(f) = {reco 2  나], 늦     el fis       (4.11)

l+r
0,                  IF Poe

160



===== PAGE 159 =====
제4장_ 이 기초

1
1
0하                                         4
18
3                                                 3
216                                                     = 06+                                               |
른                                                 E
14                                                     < 04+                                               4
12                                                 0.24                                         J
0                                                  oF
-80 40 -20     0     20     40     60        9      0.2     04     06     08      1      12
Time Index                                                          Frequency
(a) Raised cosine 필터의 임펄스 응답           (06) Raised cosine 필터의 주파수 응
+       +       ;       ;     ==
1.2                                                  1                                  — 0.5
— 「=1
1
0하                                         4
18
8                                                    3B ost
=16                                              =
은                                                 은
Za                                                  두 0사                                            i
12                                                 0.2b                                         i!
0                                                                                   oF
-0.2                                                -02       1       1       1       Ｌ       i
0-40  -0 _ 0     26     Wo 6        ‘0      02 04     06 08      1      12
Time Index                                                                Frequency

(c) Square-root raised cosine 필터의 임펄스 응답 (0) Square-—root raised cosine 필터의 주파수 응

그림 4.3 Raised cosine 필터와 square root raised cosine BE2| 특성

0                               !                    0                               ;                     0
Time                                                              Time                                                              Time

(a) r=0                  (b) r=0.5                 (c) r=1,0

그림 4.4 Roll-off factor2| 변화에 따른 eye diagram

Roll-off factor2] 변화에 t}= squareroot raised cosine 필터의 시간영역 및 주파수영역
특성이 그림 4.3(0)와 (0)에 주어져 있다. 이 그림에서 나타난 바와 Zo] squareroot raised

cosine 필터는 그 자체로 Nyquist criterionS 만족하지 않지만, 송수신단에서 송수신 필

161



===== PAGE 160 =====
PART 1 OFDM2} MATLAB

로 squaretoot raised cosine 필터를 각각 사용할 경우 전체 필터 응답이 Nyquist criterion
을 만족시키게 된다. 또한 송수신 BES] 구조가 동일하기 때문에 수신단에서 844076700[
raised cosine 필터는 정합 필터의 FS 함께 수행하게 된다[70].

(3) 단일 반송파 전송 방식의 한계

현재 많은 통신 시스템에서 고속 데이터 전송의 필요성이 급격히 증대되고 있다. 전 절
에서 설명한 바와 같이 왜곡 없는 데이터 송수신을 위해서는 일정 폭 이상의 주파수 대역
이 필요한데, 이 때 필요한 최소한의 대역폭을 50418 대역폭이라고 부른다. RS 심볼
속도로 정의할 때, Nyquist 대역폭은 2./21로 주어진다[69]. 즉, 1초에 #,개의 ASS
전송하려 할 때 필요한 최소한의 대역폭은 ./2412가 되기 때문에 1122의 대역폭을 사용
하여 달성할 수 있는 최대의 AS SEE 2symbol/sec7} 된다. 따라서 고속의 데이터 전
SS 위해서는 광대역 사용이 필수적이 되며, 단일 반송파 전송 방식에서 고속의 데이터
전송을 위해 심볼 주기를 짧게 한다는 것은 곧 사용하는 대역폭이 넓어진다는 것을 의미
한다. 전 절에서 설명한대로 심볼 주기가 짧아지더라도 Nyquist 00[6000을 만족시킨다면
ISI 없는 데이터 전송이 가능하지만 이는 완벽한 채널 보상을 조건으로 하고 있다. 일반적
으로 심볼의 AS 주기가 짧아질수록 샘플링된 신호의 관점에서 전송 채널의 최대 지연

확산은 상대적으로 길어지는 효과가 나타나 채널에 의한 ISI] 영향이 증가한다. 즉, 전송
채널의 최대 지연 확산 같이 동일할 경우에도 전송 주기가 짧아질수록 샘플링된 Ass

사이의 161는 증가하게 된다. 일반적으로 저속 데이터 AS 시에는 협대역을 사용하기 때
문에 채널이 주파수 비선택적(880) 페이딩 AAS 근사화가 되어 수신단에서 등화기가 필
요 없게 된다. 그러나 고속 데이터 AS 시에는 SAAS 사용하기 때문에 주파수 선택적
채널이 되어 이를 보상하는 등화기의 사용이 필수적이 된다. 고속 데이터 전송이 될수록
채널의 주파수 218s (frequency selectivity)o] 증가하기 때문에 이를 보상하기 위한 수신
단의 등화기 복잡도가 증가하게 된다[1][71]. 특히 등화기는 많은 곱셈기가 필요하고 곱셈
기는 하드웨어 구현 시 복잡도가 크기 때문에 단일 반송파 전송 방식으로 고속의 데이터
ASS 위해서는 등화기 구현 복잡도가 크게 증가하는 단점이 있다.

EWE FS 반송파 전송 방식

01) 다중 반송파 시스템의 기본 구조
다중 반송파 전송 방식은 광대역의 단일 반송파 전송 시 겪게 되는 채널의 주파수 선택

162



===== PAGE 161 =====
Ml4et OFDM 기초

성을 극복하기 위하여 여러 개의 반송파를 사용하여 데이터를 전송하는 방식이다.
반송파 전송방식의 기본적인 개념은 다중 채널 전송 시스템에서 찾아볼 수 있다[72}
[74]. 다중 채널 전송 방식에서는 “a 4.5에 나타난 바와 같이 광대역 신호를 여러 개의
협대역 신호로 분해(0081599)하여 전송하기 때문에 광대역의 주파수 선택적 채널이 협대
역의 주파수 비선택적 채널로 근사화된다.

dy
0

ch

Wideband 639                iseseensonzans
Signal                          |       {      "
x    >| 260) 4             ms Gf)       x
커프 더       Channel    ~ G(f)
+     &       {
ㅇ          Noise         ㅇ
ㅇ                      ㅇ
ㅇ                      ㅇ
Hy (fF               G1 (Ff)
Analysis fiter bank         Synthesis fiter bank

(a) 다중 채널 전송 시스템의 구조

_,| Frequency selective                 ba
Frequency non-selective
$         TT                y,
e                  YN         v4       IN
은                     TT              NN
<x                                               rN
Frequency

06) 다중 채널 전송 시스템의 주파수 특성
그림 4.5 다중 채널 전송 시스템의 구조와 주파수 특성

여기서 A (f= 광대역 ASS 협대역 신호로 분해시커주는 kA 대역통과 필터
이며 @,(/)는 2,.(/)의 정합 필터00810160 래서 나타낸다. 수신단에서는 수
대역 ASS 합성(670016819)하여 송신단에서 전송한 광대역 ASS 복원하게 되는데 협
대역으로 나뉘진 신호가 통과하는 각 eras 독립성이 유지된다면 ICI(Inter—Channel
eee 존재하지 않아 왜곡 없는 데이터 송수신이 가능하다. 각 PASS 통해서
송된 신호는 주파수 비선택적 채널 특성 때문에 수신단에서 각 부채널 별로 복잡도가
단일탭 등화기를 사용하여 채널 보상이 가능하다.

xt
clo ob»

163



===== PAGE 162 =====
PART Ｌ_야미과 MATLAB

위에서 설명한 다중 채널 전송 개념을 적용한 다중 반송파 전송 방식의 기본적인 구조
는 그럼 4.6(8)에 주어져 있다[75]. 여기서 /,는 《번째 부반송파의 주파수, WS 사용되는
부반송파의 개수를 나타낸다. 또한 X[k] St Y [A] / 번째 심볼 구간에서 /,의 부반송프
에 실려 송신된 신호와 수신된 신호를 각각 나타낸다. 이 그림으로부터 다중 반송파 전
방식은 다수의 기저대역 필터와 발진기를 갖는 주파수 분할 다중화 방식임을 알 수 있다.
그럼 4.6(6)는 다중 반송파 전송 방식에서의 전송 신호 스펙트럼의 YS 보여주는데 각 부
반송파를 중심으로 일정 대역을 갖는 부채널로 구성된다. 이 그림에서와 같이 각 Hayy
이 대역 제한 필터에 의해 대역 제한될 경우 FMT(Filtered Multi-Tone) 전송 방식이 되며
이 FMT 전송 방식에 대한 자세한 내용은 4.1.2 (3)절에서 기술한다.

fo
Encoder |}>|                                              바에 ae     . 빼 [0]

fi
X,[1]                                 Baseband                                  Cae               b        Baseband                                y,(1]
—>| Encoder      filter                   5 So                filter | 7) Decoder |

r|

부

ob»

들

Baseband
filter

os
°

Baseband

— >| Encoder +>}     filter

fu- 1
Lb Me pe 펜 00

(a) 기본적인 다중 반송파 시스템의 구조

Power
Spectrum
0 900 ~

The , Frequency
b) 다중 반송파 시스템의 스펙트럼 특성
그림 4.6 다중 반송파 시스템의 구조와 스펙트럼 특성

그
=
>

FMT 방식의 다중 반송파 전송 시스템은 광대역 단일 반송파 전송 시 발생하는 채널의
주파수 선택적 SYS 극복할 수 있지만 사용하는 부반송파의 개수만큼 필터와 발진기를
사용해야 하기 때문에 높은 구현 복잡도를 가질 수 밖에 없다. 또한 부채널간 간섭을 막기
위해서는 대역 제한 특성이 좋은 필터를 사용해야 하고 넓은 대역을
주기도 짧아져야 하기 때문에 부반송파의 수가 많을 경우
게 된다. FMT 방식에서는 이상적인 대역 제한 mis 유
하기 때문에 부채널간 보호 YAS 두어 ICS 방지하기도 하는데 이는 대역폭 aes 감
소시키는 원인이 된다.

164

0 08


===== PAGE 163 =====
제4장_야0 기초

(2) OFDM 전송 방식

OFDM(Orthogonal Frequency Division Multiplexing) 전송 방식 역시 여러 개의 부반
SUS 이용하여 데이터를 전송하게 되는데 전 절에서 설명한 FMT 전송방식과는 다르게
대역 제한 필터를 사용하지 않으며 각 부채널의 전력 스펙트럼이 중첩(006080)되는 특성
을 갖는다. 그림 4.7(0)는 OFDM 전송방식의 개요를 나타낸다. OFDM 방식에서 부채널이
서로 중첩되는 상황에서도 ICI} 발생하지 않는 이유는 각 부반송파간 직교성이 유지되기

문이다. 부반송파간 직교성(00008000880이 유지되기 위해서 그림 4.7(a)o 주어진 *번
째 부반송파 /,는 자기 AALS 제외한 다른 모든 부반송파와 직교하는 성질을 가져야 하
며, 이를 위해서는 심볼 간격이 부반송파 간격과 역수 관계를 이루어야 한다. OFDM] 변
복조 과정은 IDFI/DFTS] 수학적 표현과 동일하기 때문에 다수의 발진기 대신 그림
4.706)에 나타난 바와 같이 IDFT/DFTS 사용하여 구현할 수 있으며, 실제적으로는
IFFT/FFTS 사용하여 효율적으로 구현이 가능하다[76]. OFDM 전송 방식에서 송신 신호
의 주파수 SAS 그림 4.7(0)에 나타난 바와 같이 주파수영역에서 이동된 sinc 함
합으로 볼 수 있다. 이 그림에서 부반송파간 간격이 심볼 간격의 역수일 때 인접 부
위치에서 sine 함수가 모두 영교차 하기 때문에 직교성을 유지할 수 있다. 이러한 OFDM
전송 방식은 FMT 다중 반송파 전송방식처럼 다수의 대역 제한 필터와 발진기를 사용하
지 않으며 보호 대역을 두지 않고도 ICS 방지할 수 있기 때문에 대역폭 효율이 높다.
^109Ｌ과 Zipper 방식의 \109Ｌ에서 사용하는 DMT(Discrete Multi-Tone) 전송 방식 역시
OFDM3} 동일한 구조를 갖는다[77].

그러나 OFDM 방식은 FMT 방식에서와 같이 각 부반송파에 실리는 신호를 대역 제한
시키지 않기 때문에 그림 4.7(0)와 el 나타난 바와 같이 ACI(Adjacent Channel
Interference)7} 크게 발생한다. 9100 함수의 첫 번째 906 1066의 최대 전력 값은 main
1066에 비하여 -13008의 크기로서 상당히 큰 대역 외 방사가 WSs 알 수 있다. 따라서
OFDM 전송방식에서는 ACIS 줄이기 위해 대역 끝 주위의 부반송파에 아무런 데이터를
전송하지 않는 보호 ASS 두어 대역 외 방사를 줄인다. 또한 OFDM 심볼이 채널을 통
과하면서 OFDM 심볼간의 191가 발생하기 때문에 이를 방지하기 위해 보호 구간을 눈다.
일반적인 OFDM 시스템에서는 보호 대역으로 가상 반송파(10481 Carrier; VC)S 사용
하고, 보호 +4702 CP(Cyclic Prefix)S 사용한다[78]. 이러한 보호 대역과 보호 구간은
OFDM 시스템의 대역폭 효율을 감소시킨다. 또한 OFDM 전송 시스템은 부반송파간 직
교성에 의해 각 부채널간 독립성을 유지하기 때문에 주파수 옵셋에 민감하며 이에 의해

일             반

ICI} 발생한다. 일반적으로 단일 반송파 시스템은 타이밍 옵셋에, 다중 반송파 시스템은

165

| 제


===== PAGE 164 =====
PART 1 OFDM2Z} MATLAB

주파수 옵셋에 민감하기 때문에 이를 고려한 동기화 방식이 필요하다. OFDM 전송방식의
기본 이론 및 요소 기술에 대해서는 4.2절부터 자세히 다룬다.

P/S

fo

Channel
&

s/P                           Noise

(a) OFDM 전송 방식의 개요

조시 >| Encoder Ky     |»        |_|                          |        iL [al
ie   |   =                 |      _
Channel
s/P} | O | |P/S}s 0 8 거에 .  106
           Noise           T
- Eee                 덜 _ 털
06) IDFT/DFTS 이용한 OFDM 전송 방식
1k
0.8
8 06+
들 0.사
=
< o.2h                                            |
. 스시             사시
oF                          Ygeecooy
-0.2}                         V

=15    -10    =5     0      5     10
(c) OFDM 전송 방식의 AEA (linear scale)

Power
Spectrum

=5                    5

Frequency
(0) OFDM 전송 방식의 전력 스펙트럼 특성(48)
그림 4.7 OFDM 전송 방식의 구조와 스펙트럼

166


===== PAGE 165 =====
AMl42t OFDM 기초

(3) FMT 전송 방식

그림 4.8(a) 다수의 대역 통과 필터를 이용하는 FMT(Filtered Multi-Tone) 전송 방식
의 송수신 FRE 보여준다. 이 그림에서 X[k] (번째 심볼 시간에서 《번째 부채널로
전송되는 JSS 나타내며, X[k] (W+v) a 오버샘플링되어 *번째 대역 통과 필터

(/)를 통과한다. 여기서 OE 기저대역 필터 /(《)를 Aprototype) 필터로 하며 부
반송파 /,에 따라 달라져 ,(《)6" "로 주어진다. NS 부반송파의 개수, vi 0 혹은 0
정수, 부반송파 간격은 (W+v)/(NT), 샘플       는 (N+v)/T7} 된다. 이 때

다 큰 정수                                 링 속도
Te 심볼의 전송 주기를 나타낸다. 수신단에서는 각 부채널마다 송신 필터의 정합 필터가
AL 필터로 사용되고 수신된 신호는 (+ 0)배 다운샘플링 되어 수신 심볼 [가 된

다. 이 방식에서 대역 통과 필터 (,,(0),/,,(-1))는 실제로 기저대역 필터 뱅크와 발진기
뱅크로 구성되는데 이러한 구조의 구현 방식을 “12160 Realization” 방식이라고 부른다.

mo t w+) po]  so |                  — hb | 들 0
on tivewb >| n@ |[->8    ee "       { ait) 런 0

Noise

QV

wy tote)      hy_,(t) ㄴㄴ                          tay. (tf >| | 짜이

ff        (N+v)/T                                                        (N+v)/T          1/T

(a) FMT 전송 방식의 개요

ㅣ
< =
TT

Power
ectrum
dB)

chk ob no

시구 수가 oc 2

(

Sp
|
2
oO

-9애                                          NW   AN
-001200011'교          0000      '
-60            =i           10                             20             tin             60
…

06) FMT 전송 방식의 전력 스펙트럼 특성

그림 4.8 FMT 전송 방식의 개요와 스펙트럼 특성

167


===== PAGE 166 =====
PART Il_ OFDMZ} MATLAB

이와 같이 FMT 전송 방식은 대역 제한 필터를 사용하여 각 부채널을 분리하기 때문에
그림 4.800)에서 볼 수 있듯이 인접 대역으로의 스펙트럼 누설이 크지 않다. 따라서

06

OFDM 방식에서와 같이 ACIS 감소시키기 위한 보호 대역인 VC SS 사용할 필요가 없
거나 보호대역을 두더라도 OFDM 방식에 비해 매우 적은 비중을 차지한다. 만약 부반송
파 간격과 사용된 필터의 특성이 각 부채널을 완전히 분리시킬 수 있는 조건을 만족하는
경우라면 101가 발생되지 않기 때문에 OFDM 전송 방식에서와 같이 CP 등의 보호 구간
& 두지 않아도 [Slo] 의한 ICI} 발생하지 않는다. 실제적으로 FMT 방식을 채용한 통신
시스템에서는 주파수 효율이나 필터의 복잡도 등을 고려하여 시스템의 성능을 크게 열화

시키지 않는 범위 내에서 ICIS 어느 정도 허용하기도 한다[79].

1) Critical Sampled Case2} Non-critical Sampled Case
심볼 주기와 부반송파 간격이 역수 WAS 성립하여 직교성을 유지하는 OFDM AS
방식과 달리 FMT 전송 방식은 부반송파 간격이 심볼 주기의 역수보다 큰 경우에서도 적
용이 가능하다. FMT 전송 방식에서 심볼 주기와 부반송파 간격이 역수 관계가 성립하는
경우(ㅠ= 0) 를 “critical sampled 0886”라고 부르며, 그렇지 않은 경우(4ㅁ>0) 를 “non-
critical sampled 0856”라고 부른다. 0114081 sampled 0856의 경우 이상적인 대역 제한 필
터를 사용해서 각 PASS 대역 제한시켜야 부채널간 SAS 막을 수 있기 때문에 FMT
전송방식에서는 복잡도나 부채널간 간섭측면에서 non-critical sampled case7} 좀 더 실
용적이다. 그림 4.9는 ㅁ00ㅁ-01104081 sampled 0856의 부채널 스펙트럼 EAS 보여준다. 심
AS 7라고 했을 Wy critical sampled 0856의 부반송파간 간격은 1/7 이 되며 부채
널의 대역폭 역시 1/7' 인 경우에 ICV} 발생하지 않는다. Non-critical sampled 0856의
부반송파간 간격이 1/7' 의 (N+v)/N 배가 되는데, 이 때 은 사용되는 부채널 혹
은 부반송파의 개수를 나타낸다. Non-—critical sampled 0856에서는 부반송파의 간격이

Spectrum               (N+v)/(TN)
i 22 |
(N+0)/T 2(N+v)/T     Frequency

그림 4.9 Non-critical sampled case2| 부채널 스펙트럼



===== PAGE 167 =====
제4장_야미/ 기초

(^"+1)7 배 증가하기 때문에 대역 제한 필터로서 통과대역 Zo] 1/7 인 이상적인 저역
통과 필터를 사용하게 되면 부채널간 vANT) 의 보호 YAS 갖게 된다. 또한 대역 제한
필터로서 Nyquist 대역폭이 1/7' 이고 7011-0 factor7} r °l raised cosine 필터를 사용할
경우 부채널간 간섭이 발생하지 않을 최대의 ?01-01『 factor 다음과 같이 주어진다.

ee 가                (4.12)

전술한 바와 같이 FMT AS 방식에서 부채널간 SR] 어느 정도 허용될 수 있
반송파 간격 사이에 제약 BAe] 없기 때문에 부채널 대역폭,
ㅋ

, 심볼 간격, 필터 특성 등과 관련하여 유연하게 시스템 파라미터를 설계할

더 ne

고:
fir

송피
(|
BK

>
om,

2) Direct RealizationZ} Efficient Realization

그림 4.8에 나타난 바와 같이 “Direct Realization” 방식을 사용하여 FMT 시스템을 4

계할 경우 부채널의 개수가 증가할수록 구현의 복잡도가 크게 증가하게 된다. FMT 전송
방식의 구현 복잡도를 줄일 수 있는 방식으로 “Efficient Realization” 방식이 제안되었으
며, efficient realization 방식에서는 다수의 필터와 발진기를 이용하지 않고 IDFT/DFTS}
poly—phase 필터 YAS 이용해서 FMT 전송 방식을 구현하게 된다. che efficient
realization 방식의 FMT 전송 시스템에 대하여 설명한다.

FMT 전송 방식에 의해 생성된 연속시간 ASS 표시하면 다음과 같다.

co 271

x(th= >, >. -77)                                (4.13)

17=-00 k=0

= \r-r7)      (4.14)

위 식에서 대역 통과 필터 A, ((/+n(N+v))T-I'T)S 식(4.15)와 식(4.16)으로 표현
할 수 있으며 이를 식(4.14)에 대입하여 정리하면 x[n]2 식(4.17)과 같이 IDET



===== PAGE 168 =====
PART I1_ OFDM2Z} MATLAB

(Sr X[k eM eA) op polyphase 필터링 eal Wx, [(/-1")v+n]} 과정

으로 유도될 수 있다. 여기서 Al” 은 poly—phase decompositions] 필터 뱅크의 7 번째
계수 세트를 나타낸다.

ee +v)kl'
h, W277 = 1+    TIT len Omg 15)
N+yv           N+yv

2a        2a        22     2a
JR(I(N+v)+n) —j——(N+v) kl   j—h(I-l') j—kn                   4]
e*      e *     =e 4    6                 (4.16)

var Even  ~ i rT aa ie

=—co k=0
= 황시          ]  rr \S x tee
들 =     +)          "

k=0

(4.17)

= by(I-1')  ae

= = DAIL, [ke a"     a

= 1 he). x,[(I-l')v+n]
['=—00

Al (4.17)에서 v7} 0이 아닌 경우에는 송신 심볼 X[k] ol] 대해 IDFT7} 수행되는 것이
아니라 67`%0"^0-' 의 위상 회전이 발생한 심볼에 대하여 수행되기 때문에 IDFT= 각 심
볼 시간마다 재계산 되어야 하고 그 결과는 ×,[(/-/')7+70]과 같으며, IDFT 출력 샘플은
"가 0인 BPA 비해서 (0 +) 배로 증가해야 함을 알 수 있다. 하지만 IDET 출력의
주기 함수 SAS 이용하면 출력 샘플들의 순환 이동(07041 shift) 및 주기적 확장
(periodic extension) & 통해서 IDFTS] 재계산 및 출력 샘플 수의 증가를 쉽게 처리할 수
있다. 즉, FMT 전송 방식은 IDFTS} poly—phase 필터 YAS 이용하여 효율적으로 구현
이 가능하다. FMT 신호의 복조 과정은 변조 과정의 역순이 되며 2017-171056 정합 필터
링 과정에서 수신 샘플들이 매 심볼 시간마다 순환 이동 및 주기적 확장 과정을 거치게
되고 최종적으로 DITS 통해 송신 심볼을 Bela} 낸다[80]. 이 때 복조된 심볼들은
67" 의 위상 회전이 발생하게 되는데 이는 DFT 입력에서 순환 이동을 통해 간단히
해결할 수 있다.

그림 4.10은 0011081 sampled 0856의 경우(4ㅁ= 0) FMT 전송 ¥}4]°] efficient realization
구현 블록도를 보여준다. 여기서 hi!” & 원형(000[01506) 필터 A(t) 에서 개의 세트로

170



===== PAGE 169 =====
제4장_ OFDM 기초

a                     n?                                                        no                    0
an             no          ln       이          00            20
N/T            N/T
x,(v-1]                                                     ¥,[N—1]
n-»                                                                            eee

1/2'        10006         10606                         1/T'         iff        102"

그림 410 FMT 전송 방식의 efficient realization—critical sampled case

polyphase decomposition’] 계수들 중 "Ha AES 계수로 구성된 필터로서
4((/+77/20)7') 으로 주어진다. 또한 "은 h(t) 의 정합 필터에서 poly—phase decom-

position] "번째 계수 세트를 나타낸다.
Non-critical sampled 0856의 경우 역시 그림 4.11에 나타난 바와 같이 IDFT/DFT2}

poly-phase 필터 YAS 이용하지만 컨트롤 과정은 0704081 sampled case2} 차이가 있다.
송신단의 경우 개의 IDET 출력은 개의 쉬프트 레지스터 세트로 입력되며 각 레지스터
세트에 저장된 값들은 식 (4.18)에 주어진 N+v 72] 세트로 201/-1010856 decomposition
된 계수와 컨볼루션 과정을 거치게 되는데, 첫 번째 레지스터 세트부터 NV 번째 레지스터
세트가 Al 번째 poly—phase 계수 세트부터 NV 번째 poly—phase 계수 세트 까지와 컨볼루
션된 후 N+1 번째부터 N+v+1 번째 poly—phase 계수 AEE 다시 A 번째부터 「
번째까지의 레지스터 세트에 저장된 입력 데이터와 컨볼루션 과정을 거친다. 다음 심볼
시간에서는 이전 심볼 시간에서 마지막으로 컨볼루션 과정을 거쳤던 레지스터 세트의 바
로 다음 세트와 Al 번째 poly—phase 계수 세트를 시작으로 하여 앞서의 과정이 반복되게
된다. 이와 같은 과정을 거치면서 가 0인 경우에 비해서 IDFTS] 출력 샘플이
(N+v)/N 배로 증가하게 되며 순환 이동 역시 필터링 과정에서 함께 진행되게 된다.
수신단의 경우 (%+1)개의 수신 샘플은 개의 쉬프트 레지스터 세트로 입력되며 각
레지스터 세트에 저장된 값들은 A (4.19)에 주어진 개의 세트로 2017-ㅁ1856
0600000051000된 계수와 컨볼루션 과정을 거치게 되는데, 첫 번째 샘플부터 ^ 번째 샘플
까지는 첫 번째 레지스터 세트부터 VN 번째 레지스터 AES 입력되고 나머지 개의 샘
Se 다시 첫 번째부터 『 번째 레지스터 AES 입력된다. 다음 심볼 시간에서는 이전 심
볼 시간에서 마지막 샘플이 입력되었던 레지스터 세트의 바로 다음 레지스터 세트를 시작

171


===== PAGE 170 =====
PART 1 OFDM} MATLAB

Wa                                                       1/@     1/ 27
제미                 (N4+0)/T (N+0)/T            | yo]
소띠                                             |                    Coleg                    =i         EF tu]
Noise                       pet! .
X,Lv-1]
Y,[N-1]
~

{hi}                                                                {91}

{nh}                                                                {gl}

{nlr- 2}                                               {이바

{ay

{aye “~ 0}

그림 4.11 FMT 전송 방식의 efficient realization - non-critical sampled case

이 입력되며 첫 번째 샘플이 입력된 레지스터 세트와 첫 번째 poly—phase

해서 번째 샘플이 입력된 레지스터 AES} NV 번째 2017-111856
션이 진행되게 된다. 이로써 의 입력 WSL 다시 NAN +y) Hy

필터링 과정에서의 순환 이동과 변조된 ASS] 위상 BAS 보상하기
7 입력 샘   \플의 순환 이동도 수행된다.

ae poly—phase 필터의 계수 값은 다음과 같이 주어진다.

10
12,

4»
ean
ne
fold

고

2
10
Safe
= =
a
10
Hu

가벼
   if
nue   a4

de
내
기 으깨
고
08

로
스
rh
계수 세
로감
위한 D
위

172

A =h||1+—"— Ir |, n=0,1,...,N+v—1
/   | ) "      "              내

N     n
=      I+   T |\,n=0,1,...N —-1            ,
2   에그   |  | "                           (619)



===== PAGE 171 =====
제4장_ 0 기초

 단일 반송파와 다중 반송파 전송 방식의 비교

표 4.1은 전 절에서 설명한 단일 반송파 전송 방식과 다중 반송파 전송 방식의 장단점
요약하여 보여준다. 단일 반송파 전송 방식은 주파수 선택적 채널에서 높은 복잡도의

필요로 하기 때문에 저속의 데이터 전송에 적합하며, 고속 데이터 전송을 필요
는 광대역 통신 시스템에서는 다중 반송파 전송 방식이 유리하다. 다중 반송파 전송
2] OFDM 방식과 FMT 방식은 각 부채널을 분리하는 방식에 가장 큰 차이가 있다.
OFDM 방식에서는 부반송파 간격이 심볼 주기의 역수가 되게 설정되어 항상 직교성이 유
지되기 때문에 부채널간 분리를 위하여 필터가 필요하지 않으나 40: 감소를 위하여 VC
등의 보호대역이 필요한 단점이 있다. 반면에 FMT 방식에서는 일반적으로 부반송파 간격

심볼 주기의 역수보다 크게 설정되어 직교성이 유지되지는 않으나 부채널간 분리를 위

©

1c

한 필터를 사용하여 부채널간 간섭을 최소화하고 ACIS 감소시킨다. FMT AS 방식에서
는 부반송파 간격이 증가함에 따라 부채널간 간섭이 감소하고 필터의 복잡도가 감소하는
장점이 있으나 대역폭 효율이 저하되는 단점이 있다. 또한 FMT 전송 방식에서는 OFDM
에서 필수적으로 요구되는 보호 구간(#』)이 사용되지 않는 장점이 있다. 일반적으로 부반
송파 개수가 64개 이상일 경우 OFDM 전송 시스템이, 그 이하일 경우 FMT 전송 방식이

표 4.1 단일 반송파 전

Of

방식과 다중 반송파 전송 방식의 비교

ce

.부반송파 간격                              1/심볼주기         1/심볼주기와 같거나 큼
RC 필터 등의      | eos  RC 필터 등의
일    Nyquist 필터      | es ca ae      Nyquist 필터
BS Bz      필요 없음            필요(08)             필요 없음
으              필요                     fo)
sad      ew 이기게 as
주파수 wa 부반송파 개수가 많을
채널에서 비교적      때 대역폭 효율 높음       작은 ACT 발생
단순한 구조            (64개 이상)
주파수 선택적      부반송파 개수가 적을” 부반송파 개수가 적을
채널에서 높은       때 대역폭 효율 감소, ㆍ 때 대역폭 효율 높음
복잡도의 등화기 필요       = ACI 발생            (64개 이하)

173



===== PAGE 172 =====
PART ㅁㅁ OFDM2} MATLAB

고
12

폭 효을 면에서 유리한 것으로 알려져 있다. FMT 전송방식은 부반송파 수를 가변
}여 전송 SES 쉽게 가변할 수 있기 때문에 SAM(Scalable Adaptive/Advanced
Modulation) 계열로 분류되며 현재 주파수 공용 통신 181#ㅅ1의 전송 방식으로 사용된
다. 이 HOA) RC BEE raised cosine 필터를 의미한다.

다중 반송파 전송방식에는 OFDM 방식과 FMT 방식 외에도 DWMT(Discrete Wavelet
Multi-Tone), OFDM/OQAM-IOTA 등이 있다[811[821.

에

OPP orp 기본 원리

 OFDM 변

(1) 직교성

두 신호 사이의 직교성(000108008115/)은 두 신호의 곱을 ABS 결과가 0이 되는 경우
를 의미한다. 주파수가 177'인 복소 정현파(6007016× sinusoidal wave)2} 주파수가 k/T
인 복소 정현파에 대해 ?** 라면 두 복소 정현파의 곱을 기본 주기(7) 동안 적분하면 그
값이 0°] 된다. 즉, 서로 다른 주파수를 갖는 두 복소 정현파의 기본 주파수(177 )가 같은
경우, 이 복소 정현파들의 기본 주기와 같은 길이를 갖는 시간 제한(4016-110160) 복소
정현파 사이에는 서로 직교성이 성립한다. 이를 수식으로 표현하면 다음과 같다.

1 은 22800        1 pr jowks jams        r a      Lk=7
—| ee Ph =| e Te T dt=—         4 a=                       4.20
T J                   0" ㅣ                                      0, otherwise      (    )

여기서 7와 《는 정수이다. 위 AS O}ALA|ZH(discrete-time)°o 2 HASH 다음과 같다.

나 ㅠㅠ EE    es         7-1 .». (k-i)          _:
AS rng TN ae 개 _  1, k =]                         (4 21)
IN 50                  NS            0, otherwise                 ：

여기서 T/N 는 샘플링 주기를 나타낸다.
식 (4.20)과 식 (4.21)에서 적분 구간이 기본 주기의 정수배가 아닌 경우에

는 직교성이
만족되지 않는다. 이는 복소 정현파와 구형파 윈도우(660308410ㅠ \10001\)의 곱으로 표현

174



===== PAGE 173 =====
제4장_ OFDM 기초

되는 시간 제한된 복소 정현파에서 구형파 윈도우의 길이가 기본 주기의 정수 배와 같지 않
경우에는 구형파 윈도우의 주파수영역 표현인 sinc 함수의 영교차(26600-00089108) 주파

fe)
끈
수 간격과 복소 정현파의 인접 고조파 성분 간의 주파수 간격이 일치하지 않기 때문이다.

A} (4.20)과 식 (4.21에 나타난 바와 같이 서로 다른 주파수를 갖는 두 개의 시간 제한
된 복소 정현파를 동일한 기본 주파수를 갖고 기본 주기에 해당하는 구간 동안 적분할 경
우 두 시간 제한된 복소 정현파는 직교성을 만족한다. 08184에서는 이와 같은 복소 정현
파의 직교성 성질에 기반하여 다중 반송파 전송을 하기 때문에 부반송파 간의 간섭 없이

<

다음과 같이 주파수나 지연 시간이 다른 정현파 신호들과 그에 대한 DPT 수열들이 각각 그
림 4.12(01-86)와 (61-66)에 주어져 있다.

x, (t) = exp(j22t), Re{x,[n] =exp(j22nT, ), 7; =0.1s}                                   (E4.1a)
— X,[k]= DFT, {x, (nT, ), n=0:15}                                                (E4.1b)
x, (t) = exp(j272t), Re{x,[n] = exp(j272nT. ), T. = 0.15}                              (E4.2a)
— X,[k] = DFT, {x,(T,), n= 0:15}                              (E4.2b)
x;(t) = exp(j273(t — 0.1)), Re{x,[”] = exp(j273(n—- DT), 7: = 0.15}              (E4.3a)
— X,[k] = DFT,, {x,(#T7,), n=0:15}                                                  (E4.3b)
X,(t) = exp(j274(t —0.1)), Re{x,[n] = exp(j274(n- DT), 7: = 0.15}              (E4.4a)
— X,[k]= DFT, {x,(T,), 2 = 0:15}                                                  (E4.4b)
x; (t) = exp(j273.9(t)), Re {x.[”] = exp(j273.9nT. ), 7: = 0.15}                     (E4.5a)
— X,[k] = DFT,, {x,(”7,), 2 = 0:15}                                                       (E4.5b)
X,(t) = exp(j274(t — 0)), Re{x,[n] = exp(j(274nT, -2240)), 7: = 0.15}
aiiien fi |   0.1, if 7>0.1184                                                                    (E4.6a)
0.15, else
— X[k] = DFT,, {x,(nT,), 2 = 0:15}                                                 (E4.6b)

프로그램 4.1(orthogonality.m)o}A] x, = {x,(n7,), 2 =0:15} 들간의 직교성을 검사하기 위
해 이 수열(벡터들로 구성된 행렬과 그 전치 행렬의 HS 구하는데, 그 실행 결과는 다음과
같다.

175



===== PAGE 174 =====
PART Ｌ._ OFDM2} MATLAB

>> orthogonality.m

ans =

1.00        -0.00+0.001 0.00-0.001 -0.00-0.00i1 -0.02-0.02i 0.05-0.08i

-0.00-0.00i 1.00       -0.00-0.00i -0.00+0.00i -0.04-0.031 -0.00-0.10i

0.00+0.00i -0.00+0.00i 1.00        0.00+0.00i1 -0.08+0.06i -0.10+0.03i

-0.00+0.001 -0.00-0.00i1 0.00-0.00i1 1.00       -0.46-0.861 -0.94+0.12i

-0.02+0.021 -0.04+0.031 -0.08-0.06i1 -0.46+0.86i 1.00        0.32-0.841

0.04+0.081 -0.004+0.10i -0.10-0.031 -0.95-0.12i 0.33+0.85i1 1.00

이 행렬 중 좌상부 4×4 부분 행렬만 보면 대각 (단위) 행렬인데, 이는 (A/T [rad/s] 2] 정수
배가 되는 주파수를 가진) X,.%).%;,.X, 서로 4)D(orthogonal)s}4, 그 신호들이 지연되더
라도 한 심볼 구간에 대한 값만 수집된다면 지연 시간에 상관없이 직교성이 유지된다는 것을

의미한다. 이와 대조적으로 이 행렬의 제 5행/열과 제 6행/열 의 요소가 모두 영이 아닌 것

은 지피 과 (Qn/T [rad/s] 9] 정수배 아닌 주파수를 가진) 지,%,은 서로 직교하지 않
음을 의미한다. 이러한 직교성 여부는 그림 4.12 (61)-(66)에 주어진 DFT 결과에서도 드러
난다.
Re(x,[n])                         xi [k]
ee             eo a 0 기       20
hs             Pitt           ]
(a1) o- ++ ts Le 1    im     061) 아 |
“Sas 0F-88 4 가 20615       a
Re(x,[n])                         elk
  ¥       도 T  T  T ots T  세
BN      AN     「   제
2 ve 06 086 1 12 14 16 18       es
Re(xsln])                         xaLk]
IF 4       nas  "   " 4      vane   7          20       ;
02 0206 OF A 6 142 180 18      0    :
Re(x,[n])                         X[k]
1 aw         ik "         i x          AN          수         ㅋ                     20
(aa) of i ou Tyw 메바
Gs 00 06 08 1 12 wi 16 18 그     4
ia                         ay
wy    i 개   ff  k   Hi          L
(a5) bi   WV    AD      7    내 J   Ul     (b5) 10
LS ek 12 14 16 18 2    009
Re(xein})    .    .            제
Kas       “yh,      Oy      ro     my     }
26) if \ fot? zt 5 ale |
ae er 1 121216162     aia iad      :
그림 412 여러 가지 주파수를 갖는 정현파들과 그 DFT 수열들

176



===== PAGE 175 =====
제4장_야미/ 기초

4, M%%sX, 9] DPT 결과는 그 신후들이 가진 정보로 볼 수 있는 주파수 성분

2mkIT [rad/s] (k=1, 2,3, 4>을 제대로 나타내고 있는 데 반해, ×;※%, 의 DET 결과는 X5,%, 의

주파수 성분 Wk/T [rad/s] (k=3.9,4)& 제대로 나타내고 있지 않다. 이와 같은 직교성의 파

괴 원인은 피의 경우 피가 Xi KyyXs Xs 의 기본 주파수의 정수배 주파수를 갖지 않기 때문이

며, ※ 의 경우에는 ※ 의 주파수가 찌;%2>%>:3의 기본 주파수의 정수배이지만 FFT 구간에
불연속점을 포함하고 있기 때문이다.

% orthogonality.m
% Plot several sinusoidal signals with different frequencies/phases &
% DFT sequences in order to check their orthogonality
clear, clf
T=1.6; ND=1000; nn=0:ND; ts=0.002; tt=nn*ts; % time interval
Ts = 0.1; M = round(Ts/ts); % Sampling period in continuous/discrete-time
708 = [1:M:ND+1]; tts = (nns-1).*ts; ¢ Sampling indices and times
= [1:4 3.9 4]; tds = [0 0 0.1 0.1 0 0.15]; % Frequencies and delays
K = length(ks) ;

for =
k=ks(i); td=tds(i); x(i,:) = exp(j*2*pi*k* (tt-td) /T) ;
if i==K, x(K,:) = [x(K, [1:700]) x(K-2, [726:end]) x(K-2, [1:25])]; end
subplot (K,2,2*i-1), plot(tt,real(x(i,:)),'!LineWidth',1),
hold on, plot (tt([1 end]),[0 0],'k')
stem(tts,real(x(i,nns)),'.','markersize',5)

end

N = round(T/Ts); xn = x(:,nns(1:N));
xn*xn'/N % check orthogonality

Xk = f£t(xn.').'; kk = 0:N-1;
for 1=12Kk

k=ks(i) + td=tds (i);

subplot (K,2,2*i), stem(kk,abs(Xk(i,:)),'.','markersize',5)
end

ll 프로그램 41 직교성 확인 프로그램

(2) OFDM 변조
0604 시스팀에서는 dal 비트  PSK 또는 QAM 변조하여 데이터 심볼로 변환한
개의 데이터 ABS 직렬/병렬 변환기(50)를 통하여 병렬화한다. 병렬화된 ASE 2



===== PAGE 176 =====
PART I1_ OFDMZ} MATLAB

서로 다른 반송파에 실려 전송된다. S, 한 OFDM 심볼 구간 동안 개의 반송파를 사용
해 NAF 데이터 ASS 병렬로 전송한다. 따라서, Mary 데이터 ASS 사용할 때 한
OFDM 심볼 동안 총 MN 비트가 전송된다. 여기서 한 OFDM 심볼 동안 병렬화된 신호
를 전송하기 위해 ASS 반송파를 부반송파(640080ㅁ160)라 한다.

OFDM 전송 방식에서 각 부반송파는 서로 다른 부반송파와 직교성을 유지하기 때문에
인접 부반송파 대역으로부터의 간섭 AAS 위한 대역 통과 필터가 필요하지 않다. 또한
각 부반송파가 _ 대역이 직교성을 유지하면서 ZA(orthogonal overlap) =|7] 때문
은 다중 반송파 전송이 가능하다. 그림 4.13은 다중 반송파 전송 방식

) \

fo     hi     hi               fn- 1
(a) 대역 통과 필터를 사용하는 경우의 예

70     fi     72               fr-1
(b) 부반송파간 직교하는 경우의 예
그림 4.13 다중 반송파 전송 방식의 스펙트럼 특성

~

OFDM 심볼의 통과대역(00666000) 신호와 기저대역68500800) ASS 연속시간
(continuous-time) 영역에서 나타내면 다음과 같다.

Tym 7=0 k=

<통과대역> Hi =Re 7 vex, 0 게이      (4.22)
<기저대역> x(t) = 9X, [ke        (4.23)

여기서 /, 4, fos Toms 47, fe 은 각각 심볼 인덱스, 부반송파 인덱스, 반송파 주파
를                번
=                 ss

수, 심볼 주기, 부반송파 간격, 《번째 부반송가 주파수

178



===== PAGE 177 =====
M42 OFDM 기초

OFDM 심볼의 & 번째 부반송파를 실려 ASHE 데이터 ASS 의미하고, Ree
복소수의 실수부를 의미한다. ,,(2) 는 다음과 같이 정의된다.

이                                         4.24
0,                  otherwise                                          (       )

¥.O= {* el TET
식 we 주어진 연속시간영역의 기저대역 ASS t=/T,,, +nT,(L, = Tym /N) 에서
샘플링한 경우 기저대역 신호는 이산시간영역에서 다음과 같이 주어진다.

I       j2mkn/N
k=0

Al (4.25)는 N72] PSK 또는 QAM 데이터 심볼에 대한 IDFT(Inverse Discrete
Fourier Transform) 형태가 되며, 실제 구현 시 IFFT(Inverse Fast Fourier Transform) =
구현이 가능하다.

(3) OFDM 복조

OFDM 전송 방식에서 부반송파는 서로 직교하는                    신단에서
기본 주기 동안 적분함으로써 부반송파 간 간섭없이                       할수있
다. OFDM 복조 시 / 번째 OFDM 심볼의 ＊번째 부반송파에 실려 adel 데이터 심볼을
주파수영역에서 표현하면 다음과 같다.

복소 desler] 때문에 수신
전                   조

as
송된 데이터 심볼을 =

HK =—— [nine Reta = =

|. » Ane ' @ inl
;                                             에                                            (4.26)

N-1         "    "
이 이 OO at = XK
sym       i=0

위 식에서 채널과 잡음의 영향은 무시하였다. 그림 4.142 OFDM 변복조의 개념도를
보여 준다.

식 (4.26)에서 7=77, +777;(/; =Ty,/N) 에 샘플링된 기저대역 ASS 주파수영역에
서 표현하면 다음과 같다.

179



===== PAGE 178 =====
PART I1_ OFDM} MATLAB

Bit Stream                  X[k]                                                                                                                                                                 x(k]                  Bit Strear

그림 4.14 OFDM 변복조 개념도

N-1            N

나           j2minIN  -j2n
V[k]=  22000 "=  SLY atte  iT i]     “he j2akn/N

=

(4.27)

1

=

그         a
==        Lee = X[k]

=0 7

3
ㅣ
=

식 (4.27)의 결과로부터 수신된 OFDM 심볼을 DFT (Discrete Fourier Transform) 취함
으로써 송신신호를 복원할 수 있으며, FFT(Fast Fourier 178051000)을 사용하여 고속으로
구현할 수 있음을 알 수 있다.

그림 4.15는 OFDM 통신 시스템의 송신단과 수신단의 블록도를 보여준다. 송신단의 데
이터 소스로부터 생성된 비트 정보는 부호화60000108)와 인터리빙(10[646808)된 후
퍼(0000060에서 PSK/QAM 데이터 심볼로 변환된다. 그 후 데이터 심볼은 직렬/병렬
기를 통해 병렬화되고, FFTS 거친 후 OFDM 심볼로 변조된다. 변조된 OFDM 심
보호 구간 삽입 블록과 윈도윙 블록을 통과한 후 병렬/직렬 변환기를 통해 직렬 신호
Ach. 병렬/직렬 변환기의 출력은 DAC(Digital—to—Analog Converter)S 통과한
통과 필터와 RF 단을 거쳐 채널로 전송된다. 채널로 전송된 OFDM 심볼은 무선 3
통과하여 수신단에 도착한다. AWGN 잡음이 추가된 OFDM 심볼은 수신단에 입력
RF 단을 통해 기저대역으로 천이된 후 ADC(Analog—to—Digital Converter)S 통해 디지
털 신호로 변환된다. 수신단에서는 ADCS 통과한 훈련 신호 또는 OFDM ABS 이용하
： 동기화 BAS 수행한다. ADCS 통과한 OFDM ABS 보호 구간 제거 블록과 직렬/

병렬 변환기를 통과한 후 FFT 통해 OFDM 복조 된다. FFT 이후 각각의 부반송파를 통해
수신된 데이터는 채널에 의하여 크기와 위상이 왜곡되어 있으므로 lel FS 사용하여

the (뜨
flo rot oe

Hu
포

+
고

그

고
미도
오 illo 412

180



===== PAGE 179 =====
제4장_ OFDM 기초

Pilot 90000
and virtual carrier
F                                   Serial to                                                   [>| Paralle to
FEC        Bit        Mapper                      Add          md                  RF
[oa source ff FEC, 너 Interieaver 너0080 0 2 cea ee Ce
md
ㅣ                                  IL                      J         ㅣ                                           [Pan
Bit Strearn                               PSK modulated symbol                                             OFDM signal                            (
channel

Timi  19300                     (
W

demodulator)                                 04

=
i        FEC      Bit deinter          Demapper          Paralle | Channel

| decal 4 Decoding      leaver  4 (QAM demodulator/PSK } 9 sae 더

ㅣ

IL                                                                         J              |                                                          J
Bit Stream                                                QAM/PSK modulated symbol                                        OFOM signal

그림 4.15 OFDM St! 시스템의 송수신단 블록도

채널 추정한 후 등화기를 거쳐 채널 보상이 이루어진다. 채널 등화기를 통과한 데이터 심볼
은 병렬/직렬 변환기를 통해 직렬화된 후 디맵핑(06000008), 디인터리빙(06101006808),
복호화(00000108) YS 통해 정보 비트로 변환된다. 이 그림에서 송신단의 IFFT 이후와
수신단 FFT ale 사이를   aa 하고 그 외의 영역을 주파수영역이라 한다.
OFDM 전송에서는 각 부반송파에 데이터 심볼을 실어 전송하므로 전체 대역을 이용한
의 ole] Abe 각 부반송과 Bol 저속의 데이터 전송이 된다. 수신단에서는
‘abot Gls 데이터 ae] 채널 등화를 수행하기 때문에 Helga eels 저
데이터 전송이 되어 간단한 등화기를 사용하여 ABS 복원할 수 있다. 즉, OFDM 전
에서 각 부반송파는 주파수 비선택적 채널을 경험하기 때문에 단일탭 복소 등화기

al
sb

of tp IS

H(f)

BW          f

그림 4.16 OFDM 전송 방식에서의 주파수 분할

181



===== PAGE 180 =====
PART Ｌ_야미/과 MATLAB

(complex equalizer)S 사용하여 데이터 심볼이 경험한 채널의 YTS 보상할 수 있다
[721[831[841. 이와 같은 단일탭 등화는 IS} 존재하지 않는 상황에서 부반송파 간의 직교
성이 유지되는 경우에만 가능하다. 그림 4.16은 다중경로 채널에서 부반송       z
이 유지되는 경우 OFDM 심볼이 사용하는 광대역 채널의 주파수 응답과 각 부반송파가
사용하는 협대역 채널의 응답을 보여준다. 전체 광대역 채널은 주파수 선택적 채널이지만,

각 부반송파가 겪는 협대역 채널은 주파수 비선택적 채널로 근사화 됨을 알 수 있다.

보
ce
4°

Pay

El 4
ox

무선 ARS 통과한 후 수신된 /번째 OFDM 심볼은 다음과 같이 표현된다
<연속시간영역> vy, (Q=x()*h(O+z,(0= [0059060-200+50)           (4.28)
<이산시간영역 —_y[n] = xn] * hn] +z,[7] = ¥ nfm]xifn—m] + 2 [7]           (4.29)

여기서 xt], vila], 4141, 3.01은 각각 / 번째 OFDM 송신 심볼, OFDM 수신 심
볼, 무선 채널의 임펄스 함수, AWGN 잡음을 나타낸다. *는 컨볼루션 연산을 나타낸다.
식 (4.28)과 식 (4.29)에 나타난 바와 같이 수신된 OFDM ABS 시간영역에서는 송신 심
볼과 무선 채널의 컨볼루션으로 주어지고, 주파수영역에서는 송신한 OFDM 주파수영역
심볼과 무선 채널의 주파수 응답의 곱으로 주어진다. 그림 4.17과 그림 4.18은 연속시간과

WA
7s

이산시간영역에서 채널 임펄스 응답과 주파수 응답의 AS 각각 보여준다. A Ae
볼.

ad

=

°

으
볼에 대해 상수 계수가 곱해진 형태가 되어 현재 심볼이 이전 심볼의 영향을 받지
|

심             않게
된다. 이 채널은 주파수영역에서 coherence 대역폭이 넓은 주파수 비선택적 채널이 된다.
다중경로에 의하여 긴 임펄스 SHS 갖는 채널의 경우에는 시간영역에서 컨볼루션 연산

으로 표현되기 때문에 현재 심볼은 이전 ASS] VES 받게 된다. 이 채널은 주파수영역
에서 coherence 대역폭이 작은 주파수 선택적 채널이 된다.

 182



===== PAGE 181 =====
Tr : maximum excess delay

제4장_야미/ 기조

ty +1                                                  tot tott, tot to+7, 2 tot+t-1
(a) 짧은 임펄스 응답 Al                    06) 긴 임펄스 응답 예
12(7)1= 2000)                                    |H(f l= F(aA(t))

BW

BW                          '

(0) 주파수 비선택적 채널의 주파수 응답 예 (0) 주파수 선택적 채널의 주파수 응답 예

그림 4.17 연속시간 무선 채널의 임펄스/주파수 응답

21011                                 21211             =1
7 : maximum delay spread                          h(n) = Sasi 262)
p=0
                                i           시
ie                                    | 은  1
n
Ny 7671                           Ny Ny t1    ny tp-1
(a) 짧은 채널 임펄스 응답 예               06) 긴 채널 임펄스 응답 예
|A[k]l= FF T(h[n])                                                12[4]1= FFT(h[n])
aa                                  Se,    ~,             oo      “1
\      r ee     Vane    i
ak   H           1
내   i             1
4  '             '
도  i             1
로               1
4               1
we              '
|   |

BW =1/T,

(0 주파수 비선택적 채널의 주파수 응답 예

그림 4.18 이산시

그림 4.19(a)= 보호 구간ㅇ
OFDM 심볼이 다중경로 채널

태그

간 영향을 보여준다. 이 그림에서 7,

반송파 간격의 역수로 주어지며, 수

BW =1/T,

(0) 주파수 선택적 채널의 주파수 응답 예

채널의 임펄스/주파수 응답

신한 OFDM 심볼을 보여주며, 그림 4.1900)는
우 부반송파 별로 다중경로 채널에 의한 심볼
보호 구간을 포함하지 않는 유효 심볼 길이로 부

OFDM 신호의 FFT 주기에 해당한다.

183



===== PAGE 182 =====
PART IL_ OFDMZ} MATLAB

/-th OF DM symbol                  (41)-th OF DM symbol

Te = 1/ Af

(a) 보호 구간이 없는 OFDM 심볼

lh[n]|

to to+ T,

fo

752

/-0 OF DM symbo!      (l+1)-th OF DM symbol |
(b) 부반송파 별 다중경로 채널의 영향
그림 4.19 보호 구간이 없는 OFDM 신호 전송 시 다중 채널에 의한 영향

4.2.1절에서는 설명의 편의상 보호 구간을 무시하여 Tom 1, 으로 표시하였다. FFT 수행
시작점이 다중경로 채널의 첫 번째 Yo} 위치와 oe 가정할 경우, 그림 4.19(6)에 나타
난 바와 같이 다중경로 채널에 의해 지연되어 수신된 신호(점선)는 각각의 부반송파에 대해
1-th OFDM 심볼 부분이 (1+1)-//^ OFDM ae FFT 구간 앞 부분까지 존재하며,
0+ 0 OFDM 심볼 역시 다음 심볼의 FFT 구간 앞 부분까지 a 때문에 OFDM

신호 전송 시 ISIS 발생시켜 OFDM 시스템의 성능을 열화시킨다. OFDM 전송 시 다중경로
ren 의해 발생하는 ISI 문제를 해결하기 위하여 OFDM 심볼에 보호 구간을 삽입한다.

OFDM 보호 구간의 삽입 방식은 크게 두 가지로 구분된다. 첫 번째는 순환 Bicyclic
extension) 이용한 방식이고, 두 번째는 보호 구간에 OF 삽입하는 ZP(Zero Padding)
방식이다. 순환 확장 방식은 OFDM 심볼의 연속성을 유지하도록 보호 구간을 삽입하는

으로 OFDM 심볼에서 보호 구간의 위치에 따라 CP(Cyclic Prefix)2} CS(Cyclic Suffix)
로 구분된다.

184


===== PAGE 183 =====
제4장_ OFDM 기초

0 OF DM symbol                    (/+1)-th OF DM symbol

TG                       Lut

—>

Ln Lat 26

(a) CPS 갖는 OFDM 심볼

Guard                       Effective.
interval               symbol duration

Te
wy          ve
ya                             20       수                                    t
is                       fi isi

(b) CPS 갖는 OFDM 심볼의 시간영역 신호와 주파수영역 신호

ln[n]|
to to+ T,
fo |        i‘                 ~        |        a       =             |                  t
t       :       m2       |      7         (개     !
1          ~ 2             a              ee AT
I, NA      ~      Ke NA     ~      ~
|                          때                     |
                          |
T            Wh               |
|     i                       a                |         | (+1)-h OF DM symbol      |
|          Loy Leet Le       |        '                                |
Eth OF DM symbo!

(0) 부반송파 별 다중경로 채널의 영향
그림 4.20 CPS 갖는 OFDM 신호 전송 시 다중 채널에 의한 영향

185



===== PAGE 184 =====
PART I1_ 야04과 MATLAB

(2) Cyclic Prefix

그림 420) CPZ 갖는 OFDM 심볼을 보여주고, 그림 4.2000)는 CPS 포함한
OFDM 심볼의 시간영역 신호와 주파수영역 ASS 보여주며, 그림 4.20(0) 다중경로 채
널을 통과한 경우 부반송파 별 심볼간의 BS 보여준다. 이 THA Toe 보호 구간
의 길이를 나타낸다. 그림 4.20(0)에서도 그림 4.19(6)에서와 마찬가지로 다중경로 채널에
의해 지연되어 수신된 신호(점선)는 각각의 부반송파에 대해 sh OFDM 심볼 부분이
0+1)-^ OFDM 심볼 구간<,,=1.,+16)의 앞 부분까지 존재하며, ((+1)-@
OFDM 심볼 역시 다음 심볼 구간의 앞 부분까지 존재한다. 하지만 애의 길이를 다중경
로 채널의 최대 지연 시간보다 길게 설정할 경우 ISIE 보호 구간 내에서만 발생한다. 따
라서 7,,,구간에서는 ISI} 발생하지 않으며, 수신단에서 FFTS 첫 번째 경로를 통하여

신된 ALSO] T,,,, 구간에서 취할 경우 191와 ICI7} 발생하지 않게 된다.
그림 4.21은 CP 길이가 채널의 최대 지연 시간보다 짧은 경우로, 이 경우 전 심볼에 의
한 영향이 FFT 윈도우 앞 부분에 포함되어 191가 발생함을 알 할 수 있다.

그림 4.22는 CP 길이가 채널의 최대 지연 시간보다 긴 경우 FFT 시작점에 따른 ISIS}
ICI 발생 유무를 보여준다. 이 그림에서 FFTS] 시작점이 실선으로 표시된 구간 내에 존재
할 경우에는 ISI ICI7} 발생하지 않는다. 이 경우에는 의 시작점이 좌측으로 이동함
에 따라 주파수영역에서 위상회전만 발생되기 때문에 단일탭 등화기로 보상이 가능하다.
결과적으로 CP 길이는 채널의 최대 지연 시간보다 항상 길어야 한다[791.

+>

400[…….

Eth OF DM symbol                           (1)-th OF DM symbol

From
previous
symbol

!            FFT vinden         !       !      FFT Window
그림 4.21 CP 길이가 채널의 최대 지연 시간보다 짧은 경우 심볼 간 영향



===== PAGE 185 =====
제4장_0『0ㅁ0\ 기초

n]l
년        <} FFT Window start point is in this period, there exist 191
| *       ~<— lf FFT Window start point is in this period, there exist no 191 and ICI
5           > FFT Window start point is in this period, there exist ISI and 101
|     i

1—th OF DM symbol         (l+1)—th OF DM symbol

그림 4.22 FFT 시작점 위치 변화에 따른 영향

CP 길이를 채널의 최대 지연 시간보다 길게 설정하고 FETS) 시작 AS 인접 심볼의 영
향을 받지 않은 CP 구간 내로 설정한다면, 수신 ASL 의 순환 확장 특성에 의해 시간
영역에서 송신한 OFDM 심볼과 채널의 임펄스 응답의 순환 컨볼루션(00010 convolution)
이 된다. 이 경우 FFT 이후 주파수영역에서 수신 신호는 다음과 같이 주어진다.

42

Y¥[k]=         thin *xj[n]+z)[n]}e""'™ =     >ap3 h|m]x,[n— m]+ ctl}

n=0                                                                           n=0

-22씨      mi   2. [iJe j2ni(n- “ie  —j2akn/N +Z,[k]

m=0

(4.30)

N ‘20 [0                       n=0
= H,[k]X,[k]+ Z,[k]

위 식에서 Xilk], Vik] / 번째 OFDM 심볼의 《번째 부반송파에 실려 전송된 입력

느리 수신 SS 각각 나타낸다. 또한 2,[4], 2.14]는 《번째 부반송파에서 채널의

응답과 잡음을 각각 나타낸다. 따라서 FFT 이후 주파수영역에서 수신 ASE 각

Seana 입력 심볼과 채널의 주파수 응답의 곱으로 주어진다. 그림 4.230] 나타난 바

와 같이 OFDM 전송 시스템은 위와 같이 CP Als 적절히 선정한 경우 각 부반송파의

채널은 서로 독립적 채널이 되어 주파수 비선택적 채널로 병렬 전송하는 시스템과 등가가
된다.

187


===== PAGE 186 =====
PART Il_ 야미/과 MATLAB

H,{0]       310]

ie
A
=

X,(0]
A(t]                34]

:

X,[1]                   Y,(1]

씨티 *    Zk]

Xk)                                          1013

그림 4.23 OFDM 전송 시스템의 등가 모델

(3) Cyclic Suffix

CS2} CPS} 차이점은 OFDM 심볼 내의
의 위치이다. CPE 순환 확장된 부분이 ASS] 시작 부분에 존재하지만, 68의 경우에는
심볼의 마지막 부분에 존재한다. CSE 상향     과 하향스트림 간의 간섭 방지, 다른 주
파수로의 Sys 위한 보호 구간, 부의 수렴을 위한 We 구간 So] 목적으로 사용된
다. Zipper 방식의 VDSL 시스템에서 CS 사용 예를 설명하면 다음과 같다. Zipper 시스템
에서는 AAS 상향스트림과 하향스트림을 위한 부반송파 그룹으로 나누어 동시에 상향스
트림 신호와 하향스트림 ASS 송수신하는 디지털 duplexing YAS 사용하기 때문에
(#와 CSS 모두 사용한다. 이 때 (구는 다중경로 채널에 의한 191 SS 제거하기 위한
목적으로, CSE 상향스트림 신호와 하향스트림 신호가 동시에 존재할 때 발생하는 상항스

트림과 하향스트림 간의 간섭을 막기 위한 목적으로 사용된다. 따라서 (의 길이는 채널
의 지연 확산을 고려하여 결정되지만, CSO} 길이는 상향스트림의 전송 시간과 하향스트
의 수신 시간의 차이를 고려하여 결정된다.

a

환 확장(00116 extension)°] 의한 보호 구간

i ¢

rr

는

|>
ou

copy                              copy

ㅣ         i                                     Cyclic Suffix

I
th OF OM symbol    HB |    | '(H-1)-th OF DM symbol |     Y

27 iP                                         I, ub                                           27 (ay

Lion = Leet Leet Deg

그림 4.24 CP2} CSS 갖는 OFDM 심볼

188



===== PAGE 187 =====
Ml44t OFDM 기초

그림 4.24 Zipper 방식의 VDSL 시스템에서 사용되는 심볼 구조를 보여준다. 이 그림
에서 Top St Tost CP 길이와 CS 길이를 각각 나타낸다[85]. 여기서 보호 구간의 길이
= Toph Tes2| 합이 된다.

(4) Zero Padding

보호 구간에 OF 삽입하는 ZP 기법은 MB-OFDM(Multi-Band OFDM) 방식을
하는 UWB(Ultra \106-8800) 시스템 등에서 사용된다[86]. 그림 4.25(3)는 ZPS 갖
OFDM 심볼을 보여주며, 그림 4.25(06)는 OFDM 심볼이 다중경로 채널을 통과한 경우 부
반송파 별 다중경로 채널의 SHS 보여준다. 그림 4.25(6)에서도 그림 4.20(0)에서와 같
이 다중경로 채널에 의해 지연되어 수신된 신호(점선)는 각각의 부반송파에 대해 i-th

ㅅ

ofo

tel

1
128이 #야미190009 |200| (1)-th OF DM symbol

=,
=
>    |
개
`
개
es
s
i
+
`
‘            ‘
‘
t
0
————    ~ 구아
/
,
,
+"
개
*
두
，
a
>         .
해
Ss     =e
「
+           +

a gh”

/             ‘
f  ‘     별  ‘        /  \    7
|      +   내    고        「   A
'          ,  /     fly         제  *
|           ~“       별          lao?
’                   '
1         of,    Can    Lem,
2 |               ‘   A
*  (1   a  +  『  도
1        4
y
'
Ｌ

7
-
이
「,
고
/
D
'
'
‘
.
Popes            =
`,
개
내
시

fi

제
0,
=
ef
a      z
~
~

UN

(+1)-th OF OM symbol |

양

개시   Loup

Lem eet Le
Eth OF DM symbol!

10) 부반송파 별 다중경로 채널의 영향
그림 4.25 를 갖는 OFDM 신호 전송 시 다중채널에 의한 영향

189



===== PAGE 188 =====
PART Il_OFDMZ} MATLAB

OFDM 심볼 부분이 (1+1)-th OFDM 심볼 구간(27; om = sup + TG )2] 앞 부분까지 존재하
며, (l+1)-th OFDM 심볼 역시 다음 심볼 구간의 앞 부분까지 존재한다. 2#의 길이를
다중경로 채널의 최대 지연 시간보다 길게 Age 경우에도 보호 구간의 0 삽입에 의해
다중경로 채널을 통과한 OFDM 심볼은 FFT 구간 내에 불연속점을 갖게 되어 부반송파
간 직교성이 파괴되기 때문에 11가 발생한다. 이 때문에 ZPS 사용할 경우에는 수신단에
서 FFT 구간 내에 불연속점이 발생하지 않도록 그림 4.26에서와 같이 다음 심볼의 보호
구간에 해당하는 부분을 현재 심볼의 유효 심볼 시작 부분에 복사하여 더해준다.

0 OF DM symbol    j |   ss         (+1)-th OF DM symbol

copy and add                              copy and add

그림 4.26 가를 갖는 OFDM 심볼에서 연속성 유지 방법

PS 사용할 경우 보호 구간에 0이 삽입되기 때문에 실제 전송 심볼의 길이는 CP 또는
CSS 사용하는 경우에 비해 감소한다. 즉, ZPS 사용할 경우 CPS 사용할 경우에 비해
심볼 전송 시 사용되는 구형파 윈도우의 길이가 짧아지기 때문에 20 사용시 주파수영역
에서의 sine 함수는 CPS 사용할 때에 비해 넓은 영교차(26000-07059108) 주파수를 갖게
된다. 따라서 ZPS 사용할 경우 각 부반송파로 전송되는 스펙트럼의 합으로 주어지는
OFDM 심볼의 전력 스펙트럼081)은 CP 또는 CSE 사용할 때에 비해 작은 대역내
(in-band) 리플을 갖는 동시에 큰 AA S|(out—of-band) 전력을 갖게 된다. 최대 전송 전
Bo] 정해진 상황에서 전력 스펙트럼의 작은 대역내 리플은 그렇지 않은 경우에 비해
전력으로 송신할 수 있음을 의미한다. 따라서 0\8에서와 같이 다른 시스템에 간섭을
소화하기 위하여 전력 스펙트럼 마스크가 작은 값으로 주어진 경우에는 CP 또는 CSS
용하는 것보다 PS 사용하는 것이 효율적이다. 그림 4.27은 64개의 부반송파를 갖
OFDM 심볼에 ZPS 사용하는 경우와 CPS 사용하는 경우의 전력 스펙트럼을 비교하여

lu

~
25

다

 190



===== PAGE 189 =====
제4장_ OFDM 기초

|          with CP
—— Zero padding}

Tees eee eee

| a 글 1) | | ee ee,
eaaendon=                wits       그니 Zero padding

~----4---- MB -4---- 4

-0.8 -0.6 -04 -02 0 02 #04 O06 08      02 #025 O38 035 04 045 05 055 06
normalized frequency                                                                  normalized frequency

그림 4.27 CPS 갖는 OFDM 심볼과 ZPS 갖는 OFDM 심볼의 PSD 비교

보여준다. 우측 그림은 통과대역의 스펙트럼을 확대하여 보여주는데, 이 그림으로부터 ZP
를 사용하는 경우에 대역내 리플이 작고 전력 면에서 효율적임을 알 수 있다.

보호 구간은 다중경로 채널에서 OFDM 심볼 복조 시 부반송파 간 직교성을 유지하고
ISIS 방지하기 위해 필수적이지만, 그에 따른 데이터 전송 효율이 감소하게 된다. 보호
구간을 포함한 OFDM 심볼의 데이터 전송 효율은 Ty 71,ㅠ이 된다.

PE] OOFDM 보호 대역

IFFTS 통해 OFDM 변조된 신호는 시간영역에서 7,,,의 길이를 갖고 크기 1인 구형파
(rectangular) 윈도우가 곱해진 신호로 볼 수 있다. 시간영역에서 구형파 신호는 주파수영
역에서 syne 함수가 되며 syne 함수의 영교차점은 1/7;,, 이 된다. 시간영역에서 곱하기는
주파수영역에서 es 주어지가 때문에 OFDM 신호는 주파수영역에서 각 부반송
파에서 ASS ATS} sync YEO] 컨볼루션으로 주어진다. 0ㅠ의 부반송파의 간격을
1/7;,, 로 설정할 경우에 직교성은 유지되지만 syne YE] 특성 때문에 대역외(041-0[-

6800) 전력이 크게 발생하여 인접 채널에  ead  주는 ACI(Adjacent Channel Inter-

ferenee) 발생한다. 따라서 OFDM 시스템에서는 ACIS] 영향을 감소시키기 위해 주파수
a 보호 대역이 필요하다.

OFDM 전송에서 ACIS 감소시키기 위해 대역통과 필터를 사용하여 대역외 스펙트럼
줄이는 rl 있다. 이 때 41°|(transition) 특성과 통과대역 내의 리플 특성이 우수한

를 사용하면 ACIS 크게 감소시킬 수 있으나, 필터링은 시간영역에서 OFDM 신호와

계수와의 컨볼루션 과정이므로 많은 계산량이 필요하기 때문에 필터의 탭 수를 최소

191



===== PAGE 190 =====
PART 1 _야미/과 MATLAB

화 할 필요가 있다. 따라서 필터를 사용하여 ACIS 감소시키기 위해서는 BAS] 성능과
복잡도를 함께 고려하여 선정되어야 한다. 필터를 사용하는 방법 이외에도 시간영역에서
윈도우를 사용하여 대역외 스펙트럼을 감소시킬 수 있다. 시간영역에서 구형 윈도우 대신
대역외 스펙트럼 감소 특성이 우수한 201660 cosine 윈도우를 곱하여 대역외 스펙트럼을
크게 감소시킬 수 있다. RC(raised cosine) 윈도우를 적용한 1 번째 OFDM ASS 다음
식으로 주어진다.

19

N-1
<통과대역>        x,(t) = Re| RC Gel 9002, Xia Pr 이                                        (4.31)
N-1         ：
<A> x ()=RC(-IT,, ) Xe                                    (4.32)
k=0

위 Alo]A] roll—off7} £21 raised cosine 윈도우와 Y (4) 는 다음 식으로 주어진다.

72201 (t-lT sym)   =     Es <
¥o={°    ee      (4.33)

0,                 otherwise

0.5+0.5cos(s(t+BToym+To)BToym)) (Te +BToym! 2) t<—(T —BT ym! 2)

14 4.282 raised 005106 윈도우를 적용한 OFDM 심볼을 보여준다. Raised cosine 2
도우에서 roll-off 상수의 크기가 증가할수록 천이 부분이 완만해지므로 Aci: 감소하지

만, 유효 보호 구간의 길이는 감소한다.

2,

sym

Te     I          dF 1/Af

=Tot Tay

~
Tyw= BT,                                                            Lp BL

Pe sym

그림 4.28 Raised cosine 윈도우 적용 시 시간영역 OFDM 심볼



===== PAGE 191 =====
Ml42t OFDM 기초

필터링과 윈도우 방식 이외에 AS 대역의 저주파 영역과 고주파 영역, S 대역의 양쪽
부분의 부반송파를 사용하지 않는 가상 반송파(10081 carrier) 방식을 사용할 수 있다. 이
SAS 시간영역에서 별도의 처리가 필요 없기 때문에 구현이 매우 간단하고 쉽게 ACIS
asl + 있으나 Bah) 않은 kesh 인해 대역폭 mol Basha 된다. 가상
반송파 방식을 사용하여 ACHE 감소시킬 경우 전송 효율은 ,,,//# 이 된다. 여기서 w
은 전체 부반송파 수, ^, 는 데이터 ASS 위해 사용하는 부반송파의 AB 나타낸다.
가상 부반송파를 사용할 경우 ACIS] 감소뿐만 아니라 ADCS} 2&0의 저역 통과 필터의
복잡도도 감소시킬 수 있다. ACI 감소를 위하여 가상 부반송파 방식과 윈도우 방식을 a
합하여 사용할 수도 있다.

그림 4.29는 701-0 상수에 따른 1016960 cosine 윈도우의 전력 스펙트럼(60\@
Spectrum Density) 보여준다. 이 그림에서 부반송파는 총 64개 중에서 54개를 사용하였
다. Roll-off 상수가 증가할수록 대역외 스픽트럼의 크기가 감소함을 알 수 있다.

5 06 -04 -02 0 02 04 06 08

그림 4.29 Roll-off 상수에 따른 raised cosine 윈도우의 전력 스펙트럼

Pa OFDM 전송 방식의 BER 특성

AWGN 채널과 Rayleigh 페이딩 채널에서 Mary QAM 신호 전송 시 BAA
(analytic) BERS 다음과 같이 주어진다.

193 |



===== PAGE 192 =====
PART IL_ OFDM2Z} MATLAB

M-I    「  Ee log, M

.                    2°" |. AWGN 채널             4.35
Mlog,M~=(\ 2. M?-1 |      티 Ale            609.

30 |, 3ylog, M/(M*-1)
“  Mlog, M  3ylog, M/(M?-1)+1

| : Rayleigh 페이딩 채널      (4.36)

위 식에서 7, M, O(e)= Eb/N,, 변조 차수, /-함수를 나타낸다. OFDM 전송 방
식에서 가상 반송파를 사용할 경우에는 단일 반송파 전송방식과 다르게 시간영역에서 수
Al 신호에 더해진 AWGN 잡음 양과 주파수영역에서 데이터 심볼이 겪는 잡음 양에 차이
가 발생한다. OFDM 전송 방식에서 BERS 주파수영역에서 계산되므로 주파수영역의
SNR] 실제적으로 의미가 있다. tS OFDM 전송 방식에서 주파수영역의 SNRI} 시
간영역의 SNRY] 관계를 보여주는 식이다.

{

A
fe)

N.
SNR, = (SNR, —10log =z, (dB)                                          (4.37)

위 식에서 SNR,, SNR, 은 시간영역의 SNR, 주파수
aN NA 데이터 ase 위하여 사용된 부
를 나타낸다.

모의실험에서 FFT 크기는 64이고, 이 중 48개의 부반송파는 데이터 전송용으로 나머지는
가상 부반송파로 사용하였다. 입력 ASS 16-QAM 심볼이고, 사용한 채널은 AWGN 채널과
최대 지연 확산이 15 샘플인 다중경로 채널이며, 채널의 각 탭은 &816191 분포를 겪는다. 그
림 4.30은 OFDM 전송방식의 해석적 BER 곡선과 보호 구간 (CP 또는 28)에 따른 BER 곡선

을 보여준다. 그림 4.30()에서 AWGN 채널의 경우에는 채널의 지연 확산이 없으므로 보호
구간이 없더라도 BER 곡선이 AWGNY] 해석적 곡선과 일치하는 것을 SB 수 있다. 또한, 다중
경로 채널의 경우에도 채널의 지연 확산 보다 긴 보호 구간 (16 샘플)을 삽입하여 191를 제거
한 경우에도 BER 곡선이 채널의 해석적 곡선과 일치하는 AS 볼 수 있다. 하지만 그림
4.30(6)에서와 같이 보호 구간이 없거나 채널의 지연 확산 보다 짧은 보호 구간을 갖는 경우
161의 영향에 의해 BER 곡선에 오차 마루가 발생한다.

에
rr (무고

thlo

194



===== PAGE 193 =====
M42 OFDM 기초

=={ ——— AWGN analytic

—— Rayleigh fading analytic
—©— AWGN, No guard interval
---@--- Channel, CP:3
----- Channel, ZP:3

—€— AWGN, No guard interval
=                               ---@-- Channel, CP:16
10°         :         Channel, ZP:16

107         :        !  \    !        i                      10         !        i  \
0

5    10    15    20    25    30    0    5    10    15    20    25    30

EbNO(d8)                                  EbNO(dB)
(a) 181에 의한 영향이 없는 경우           (b) 181에 의한 영향이 존재하는 경우

그림 4.30 다중경로 채널에서 보호 구간에 따른 BER 성능

% OFDM basic.m

clear all

NgType=1; % NgType=1/2 for cyclic prefix/zero padding
if NgType==1, nt='CP'; elseif NgType==2, nt='ZP'; end
Ch=1; % Ch=0/1 for AWGN/multipath channel

if Ch==0, chType='AWGN'; else chType='CH'; end

PowerdB=[0 -8 -17 -21 -25]; % Channel tap power profile 'dB'

Delay=[0 3 5 6 8];          % Channel delay 'sample'

Power=10.* (PowerdB/10) ;     * Channel tap power profile 'linear scale'
Ntap=length (PowerdB) ;      6 Chanel tap number

Lch=Delay (end) +1;           sChannel length

bps=4;        % modulation order=2/4/6 for QPSK/16QAM/64QAM
Nfft=64;       % FFT size
Ng=Nfft/4;    % Ng=0: no guard interval

Lsym=Nfft+Ng; % symbol length
Nvc=Nfft/4; % Nvc=0: no virtual carrier
Nused=Nfft-Nvc;

EbNO=[0:5:30]; %EbNO

N_iter=10;     * number of iterations for each EbNO
Nframe=3;      % number of symbols per frame
sigPow=0;      6 Signal power initialization

195


===== PAGE 194 =====
PART Ｌ _야미/과 MATLAB

for i=0:length (80840)
randn('state',0); rand('state',0); ber2=ber(); % BER initialization
norm=[1 sqrt(2) 0 sqrt(10) 0 sqrt (42)];        % BPSK 4-QAM 16-QAM
for m=1:N_ iter
% TX

bit= randint (1,Nused*Nframe,2“bps); % bit: integer vector
qamSym= gammod (bit, 2*bps,0, 'gray') /norm(bps) ;
if NgType~=2, ofdmSym2=zeros (1,Nframe*Lsym) ;
elseif NgType==2, ofdmSym2= zeros (1,Nframe*Lsym+Ng) ;
6 Extend an OFDM symbol by Ng zeros
end
kk1=[1:Nused/2] ; kk2=[Nused/2+1:Nused]; kk3=1:Nfft; kk4=1:Lsym;
for k=1:Nframe
if Nvc~=0, qamSym2= [0 gamSym(kk2) zeros(1,Nvc-1) gamSym(kk1)];
else     gamSym2= [qamSym(kk2) gamSym(kk1) ] ;
end
ofdmSym(kk3)= ifft (qamSym2) ;
ofdmSym2 (kk4) = guard_interval (Ng,Nfft,NgType, ofdmSym(kk3) ) ;
kk1=kk1+Nused; kk2= kk2+Nused; kk3=kk3+Nfft; kk4=kk4+Lsym;
end
if Ch==0, ofdmSym3= ofdmSym2; % No channel
else % Multipath fading channel
channel=(randn(1,Ntap)+j*randn(1,Ntap))./sqrt (2) ;
channel=sqrt (Power) .*channel;
'cir=zeros(1,Lch) ; cir (Delay+1) =channel;
ofdmSym3=conv (ofdmSym2,cir); % cir: channel impulse response
end
if i==0 % Only to measure the signal power for adding AWGN noise
for k=1:Nframe
kk= 1+ (k-1) *Lsym:k*Lsym;
sigPow = sigPow + ofdmSym3 (kk) *ofdmSym3 (kk) ';
end
continue;
end
% Add AWGN noise
snr=EbN0 (i) +10*10g10 (bps* (Nused/Nfft)); ¢ SNR vs. Eb/NO
noise _mag=sqrt ((10.*(-snr/10))*sigPow/2) ;
ofdmSym3=ofdmSym3+noise_mag* (randn (size (ofdmSym3) ) +] *randn (size (ofdmSym3) ) ) ;

196



===== PAGE 195 =====
제4장_ OFDM 기초

% RX
kk1= (NgType==2) *Ng+[1:Lsym] ; kk2=1:Nfft
kk3=1:Nused; kk4=Nused/2+Nvc+1:Nfft; kk5=(Nvc~=0)+[1:Nused/2] ;
fe ‘Ch==1

cfr= fft([cir zeros(1,Nfft-Lch)]) ;

cfr2(kk3)= [cfr(kk4) cfr(kk5)]; % frequency response function
end

for k=1:Nframe
ofdmSymRx (kk2) = f£t (remove _GI (Ng, Lsym, NgType, ofdmSym3 (kk1) ) ) ;
of dmSymRx2 (kk3) = [ofdmSymRx (kk4) ofdmSymRx (kk5) ] ;
if Ch~=0 % channel equalization
ofdmSymRx2 (kk3) = ofdmSymRx2 (kk3) ./cfr2;
end
kk1=kk1+Lsym; kk2=kk2+Nfft; kk3=kk3+Nused;
kk4=kk4+Nfft; kk5=kk5+Nfft;
end
bit_Rx=qamdemod (ofdmSymRx2*norm(bps) ,2*bps,0, 'gray');
ber2=ber (bit_Rx,bit,bps) ;
end
if i==0, sigPow= sigPow/Lsym/Nframe/N_iter;
else if (ber2<le-6), break; end
end
end

—

ig) 프로그램 4.2 OFDM 변조의 BER 성능 프로그램

% guard_interval.m: add GI

function y = guard_interval (Ng, Nfft,NgType, ofdmSym)

if NgType==1, y=[ofdmSym(Nfft-Ng+1:Nfft) ofdmSym(1:Nfft)];
elseif NgType==2, y=[zeros(1,Ng) ofdmSym(1:Nfft)]; end

2

+ remove GI.m
function y=remove_GI (Ng, Lsym, NgType, ofdmSym)

if Ng~=0
if NgType==1, y=ofdmSym(Ng+1:Lsym); % cyclic prefix
elseif NgType==2                   % cyclic suffix
y=ofdmSym(1:Lsym-Ng) + [ofdmSym(Lsym-Ng+1:Lsym) zeros (1,Lsym-2*Ng) ] ;
end

else, y=ofdmSym; end

197



===== PAGE 196 =====
PART Ｌ_ OFDM2} MATLAB

% ber.m: compute BER
function c_ber=ber(x,x_ref,bps)
persistent e bits; t_bits;
if nargin==0
e bits=0; t_bits=0; c_ber=0;
% e_ bits: # of error bits, t_bits: # of Tx bits, c_ber: cumulative BER
elseif nargin==3
for ii=1:length (x)
6 bits=e_bits+error_check (bitxor (x (ii) ,x_ref(ii)) ,bps) ;
end
t_bits=t_bits+length(x)*bps; c_ber=e bits/t_bits;
end
return;
% error_check

function ecount=error_check(x_xor,bps)
ecount=0;
for ii=0:bps-1, ecount=ecount+bitand(bitshift (x_xor,-ii),1); end

Tal 프로그램 4.3 보호 구간 삽입, 제거, BER 함수

 Water Filling 기법

채널이 시간에 따라 변하거나 이동 환경 하에서는 AMC(Adaptive Modulation and
000108)를 사용하여 시간영역에서 채널에 적합하게 적응적으로 변복조와 부호화를 하는
기법이 CDMA 등의 시스템에서 사용되고 있다. OFDM 방식에서는 이와 같이 시간영역
에서 AMCS 적용하는 것 이외에도 주파수영역에서 AMCS 적용하여 채널 용량을 최대
화할 수 있는 장점이 있다. 즉, OFDM 방식에서는 다중경로 채널에 의해 주파수영역에서
깊은 nullo] 형성된 부채널에 다른 부채널과 동일하게 비트와 전력을 할당1080108)할 경
우 nullo] 형성된 부채널의 오류확률이 크게 증가하여 전체적으로 오차 마루가 발생할 수
있다. OFDM 방식은 다른 전송 방식과 달리 주파수영역에서 ASS 할당하고 검출하므로
주파수영역 SNR] 따라 적응적으로 각 부반송파의 비트 및 전력을 할당하면 위 오차 마
루 BAS 해결할 수 있고 채널 용량(0080061 080800을 최대화 할 수 있다.

OFDM 시스템의 채널 $22 Hartly—Shannon2] 채널 용량 식을 사용하여 다음과 같
이 주어진다.

198



===== PAGE 197 =====
제4장_야미/ 기초

: a 00)                            (4.38)

위 식에서 /, 는 《번째 부반송파를, 0(/, )는 《번째 부반송파의 채널 용량을 나타낸다.

전체 대역이 많은 수의 부반송파로 구성되고, 부반송파의 수가 충분히 커서 각 부채널
Wo] SNRO] 상수로 BAS 경우 CUE gat Be] Raed.

C(f,) = Af log, 1 + any)
여기서 HK], PUK], Nyt k Ma) 부반송파에서 채널의 주파수 응답, 전송 전력, 잡음
의 분산을 각각 나타낸다.

식 (4.38)의 채널 용량을 최대로 하기 위해서는 A] (4.39)에 주어진 부반송파 채널 용량
이 최대가 되도록 각 부반송파에 전력을 할당해야 한다. 이는 각 부반송파의 전송 전력
(PIA])2) 합이 Nivea 와 같다는 조건 하에서 Lagrangian 방법을 사용하여 다음 최적화
문제의 해를 구함으로써 얻을 수 있다.

이 (=O         0

max    ~~ oe     eee)                                             (4.40)

A} (4.40)의 최적화 문제의 해는 다음과 같이 주어진다.

fr |
P[k] = | --            4.41
i ; eal       “"

여기서 ( )" 는 max(x,0) 3 나타내고, AL 각 부반송파에 할당된 전송 전력 PLT 의
합이 가 되도록 선택된다.

그림 4.31은 식 GAS 도식화한 것으로 각 부반송파에서의 SNRo] 따라 전송 전력을
할당함으로 최대의 채널 용량을 달성될 수 있음을 보여준다. 이와 같은 전력 ag 방법을
water filling 기법 또는 water pouring 기법이라고 한다. Water filling 기법을 적용할 경



===== PAGE 198 =====
PART Il_ 야0 과 MATLAB

N,/|ATkIP

1/r -4

subcarrier k

그림 4.31 Water filling 기법을 적용한 경우 부반송파 별 전송 전력 할당

우 각 부반송파에서의 채널 전력에 비례하여 송신 전력을 할당함으로써 채널 용량을 최대
로 만들며, 이 때 NSR(Noise—to—Signal 8800)과 송신전력의 합이 전체 전송 대역 내의
H

부반송파 전력 할당 방식과 마찬가지로 OFDM 전송 방식에서는
sue 상태에 따라 전송 비트와 WIS aioe UI 수 있다[72]. 이와 같은 We

제로 적용하기 위해서는 송신단에서 채널의 SNR 미리 알고 있어야 하기 때문에 송신기
와 수신기 Molo] Ad 정보교환이 SEM 루프를 통하여 사전에 이루어져야 한다. 이러
한 비트 할당 기법은 주로 채널의 특성이 정적인 전화선 채널을 사용하는 DMT(Discrete
\448-1006) 전송 방식에서 먼저 연구되었다. 위 최적화 문제에 대하여 데이터 전송률
평균 전송 전력, 오류 확률의 기준이 있을 때 이들 기준 중에서 어떤 하나 또는 두 가지가
제한되었을 경우 다른 하나 또는 두 가지의 기준을 최적화 또는 준최적화 하는 형태의 알
고리즘이 제안되었다[88]-[911. 예를 들어, 각 부반송파에 할당되는 전력이 동일하고 모든
부반송파에서의 오류확률이 동일하다는 조건하에서 《 번째 부반송파를 통해 전송되는 비
= 수 Ok] S 채널의 SNR 상태에 따라 최적으로 할당할 경우 다음과 같이 주어진다.

모든 부반송파에서 동일하게 된다[87].
전술한 바와 같이 각 부채널 Yo SNRO] 상수로 근사화될 경우 채널 용량을 최대화
하는                                               각 부반송파의
실

(4.42)

b[k] = log, ! + ANS:

여기서 SNR, 는 & Wa 부반송파의 수신 SNR, 1 는 원하는 BERS 얻을 수 있는 이론
적인 SNR} 실제의 SNR 차이(081910)를 나타낸다.

_200



===== PAGE 199 =====
체4장_야0 기초

그림 4.32는 채널의 특성에 따른 비트 할당을 예를 보여준다. 채널의 주파수영역 특성
에 따라 부반송파 별로 비트를 할당한 경우 채널 용량을 최적화 함을 알 수 있다.

Bit/Subcarrier
|
Bit/Subcarrier

Magnitude Response
|

7
그림 4.32 OFDM 시스템에서의 부반송파 별 비트 할당 개요도

wy
=

이동 환    0 사용되는 051014 시스템은 채널의 특성이 시간에 따라 변할 수 있으므
로 최적의 할당 기법을 적용하기 쉽지 않다. 이를 적용하기 위해서는 송신기와 수신기 사
이의 채널 정보   교환이 피드백 루프를 통하여 사전에 이루어져야 하는데 시변 채널에서는
채널 측정 시점과 실제 적용 시점의 시간 차로 채널의 특성이 변할 수 있기 때문이다. 또
한 수신기에서 측정한 채널 정보가 피드백 루프를 통하여 송신기로 전달되어야 하는데 그
정보량이 매우 많을 수 있어 효율적인 제어 채널의 설계가 필요하다. 최근 이동 환경에서
사용되는 OFDM 시스템을 위하여 위의 문제를 해결할 수 있는 알고리즘에 대한 연구가
활발히 이루어지고 있다[92][93].

:

EA OFDM 파라미터 설정

본 절에서는 OFDM 시스템 파라미터를 설정하기 위한 순서 및   나시 설명한다. 일반
적으로 대역폭, 비트 전송률, 무선 채널의 지연 확산의 세 가지 기본 요구 조건은 사전에
주어지기 때문에 이에 적합한 OFDM 파라미터를 선정한다. 가장 에 ii 지연 확산
을 고려하면 보호 구간 길이를 설정한다. 이 때 보호 구간의 길이는 채널의 mms 지연 확산
보다 2배에서 4배 정도 길도록 설정한다. OFDM 시스템에서는 데이터 심볼의 부호율과
데이터 심볼의 변조 차수에 따라 101와 191에 대한 민감도가 달라진다. 예를 들어,
64-QAM3} QAM 신호는 QPSK 신호보다 ICIS} 191에 보다 민감하다. 또한 높은 부호을
의 부호화기를 사용하면 ICI} 161에 대한 WATS 감소시킬 수 있다. 따라서 부호율과
데이터 심볼의 변조 차수에 따른 ICI} ISIS] 민감도를 고려하여 보호 구간의 길이를 설

r

201


===== PAGE 200 =====
PART ㅁ_야미/과 MATLAB

보호 구간의 길이를 정한 후 유효 심
되는 58의 손실을 최소화하는 관점에서는 유효 심볼 구간의 길이가 보호 구간의 길이보
다 클수록 바람직하다. 하지만 유효 심볼 구간의 길이가 증가할수록 부반송파 간의 간격
은 좁아지며 전송 대역내 부반송파의 수가 증가하기 때문에 구현의 복잡도, 위상 잡음 및
주파수 옵셋의 민감도, PAPRo] 증가한다94]-[961. 따라서, 유효 심볼 구간의 길이를 무
한히 길게 할 수 없다. 실제로 OFDM 파라미터를 설정할 때는 유효 심볼 구간(7, )이 적
어도 보호 구간(7; )의 4 배가 되도록 선택하여 보호 구간에 의해 발생하는 SNR 손실이
1 dB 이하가 되도록 한다.
OFDM 시스템에서 직교성을 만족하기 위하여 부반송파 간격은 유효 심볼
역수로 설정한다. 부반송파 간격이 설정된 후에는 요구되는 -3
으로 나누어 부반송파의 수를 결정할 수 있다. 부반송파 수를 결정하는 또

AES 만족시키는 범위 내에서 요구되는 OFDM 심볼당 비
브
부

ru

ce
X»

구간의 길이를 결정한다. 보호 구간에 의해 발생

대한 비트 전송률로 나누어 결정하는 것이다. 각
심볼의 변조 차수와 부호율에 의해 정의된다.

예를 들어, 비트 전송률 20 Mbps, 허용 지연 확산 200 ns, 대역폭 < 15 14432의 요구
조건을 갖는 OFDM 시스템의 파라미터를 설계한다. 위의 조건에서 무선 채널의 지연 확
산은 200 nso] 보호 구간의 길이를 채널의 rms 지연 확산의 4배로 할 때 보호 구간의

길이는 800 ns7} 된다. 유효 심볼 구간(7,,,)은 보호 HAT; )에 의한 SNR 손실이 108
이하가 되도록 보호 구간의 5배로 선택한다. 이 경우 부반송파 WAL 4(/8)의 역수인
250KHz7} 된다. 필요한 부반송파 수는 대역폭, OFDM 심볼당 비트 전송률, 부반송파의
비트 전송률을 고려하여 결정한다. OFDM 심볼당 비트 전송률은 비트 ASS 대한 조
Ast OFDM 심볼 주기를 이용하여 계산하며, 위의 조건하에서는 OFDM 심볼당 전송 비
트 수가 96 비트가 된다. 앞서 AR OFDM 심볼당 비트 전송률을 달성하기 위해서 몇
가지 시나리오를 고려할 수 있다. A 번째는 각 부반송파가 3/4 부호율의 QPSKES 사용하
는 경우이고, 두 번째는 1/2 부호율을 갖는 16-04)4을 사용하는 경우이다. 첫 번째 시나
리오의 경우 각 부반송파를 통해 전송되는 데이터 심볼은 15 비트이다. 따라서 심볼당 96
HES 전송하기 위해서는 64개의 부반송파가 필요하다. 하지만 64개의 부반송파를 사용
할 경우에 필요한 대역폭은 16 MHz(64x250 KHz)7} 되어 요구하는 대역폭을 초과하게
된다. 두 번째 시나리오에서는 각 부반송파를 통해 전송되는 데이터 심볼이 2 비트를 포
함한다. 이 경우 심볼당 96 비트를 전송하기 위해서는 48개의 부반송파가 필요하다. 48개

_ 202



===== PAGE 201 =====
제4장_ 0 기초

의 부반송파를 사용할 경우 필요한 대역폭은 12 MHz(48x250 112/이므로 대역폭 요구
조건(대역폭 < 15 MHz) 만족한다. 따라서 두 번째 시나리오가 위에 주어진 조건에 적
합함을 알 수 있다. IFFVFFT 크기는 64로 하고, 대역의 양쪽 부분 부반송파 16개는 가상
부반송파로 사용한다.

OFDM 파라미터 설정 시 위의 기본 요구 조건 외에 추가적으로 고려할 점들이 있다.
예를 들어, FFTMFFT 구간과 심볼 구간 내에서 샘플 수가 정수가 되어야 한다. 위의 예
에서 부반송파 사이의 직교성을 유지하기 위해서는 170 구간 내에 정확히 64 샘
플이어야 한다. 이를 ile EV RUT )을 16 Mis 설정하면 이 조전을 aE 수
있으나, 이와 같이 할 경우 4.8/8의 심볼 구간(<,,)내에 존재하는 샘플 수는 정수가
되지 않는다. 이러한 ASA GE 과라미터를 약간 변경하여 Ao] 샘플 수에 Get 조
건을 만족할 수 있다. 예를 들어, OFDM ABI 샘플 수를 78로 설정하여 16.25
MHz(78/4.8 18) 2] 샘플링율(1/7: )을 얻을 수 있다. 이제 FFT 구간은 64/16.25 MHz =
3.9385 ys 7+ 되어 보호 구간과 부반송파간 간격은 dys] FFT 구간을 사용할 경우보다
약간 증가하게 된다.

OE coded 야미              |

OFDM 전송 방식을 사용함으로써 다중경로 채널에 의한 심볼 간 간섭을 극복할 수
으나, 특정 부반송파의 감쇄가 심한 경우에는 수신 SNR] 낮아져 그 부반송파로 전송
데이터의 오류 확률이 exter 때문에 전체 88#에서 오차 마루가 발생할 수 있다. 그
4.33은 무선 채널의 주파수 응답 ABA 일부 부반송파에서 감쇄가 심한 페이딩(0662
180108)을 겪는 것을 보여준다. 이 그림에서는 주파수 축에서 감쇄가 심한 페이딩 현상을
보여주나, 시간 축에서도 동일한 페이딩 현상이 발생된다. 본 절에서는 주파수 축에서 발
생하는 페이딩 현상과 극복 방안에 대해서만 기술하나 그 결과는 시간 축에서도 동일하게
적용된다.

rid, 88

'

oe

203


===== PAGE 202 =====
PART Il_ OFDMZ} MATLAB

average SNR

‘ae                 Q         뽀뽀                 =
                      i «a         “~               |
Ss        더                                         더        |

By

required
N

SNR

/

burst error

그림 4.33 주파수 선택적 채널에서 부

[뚜
of
A
Jo
+
Ral
”
Zz
8)

만약 BE 부반송파에 동일
지 않을 최소 SNR 이상이 되               파에서는 최소 9씨보다 낮은 SNRS 갖게
될 수 있다. 이러한 경우 그 부반송파에서 오류가 발생하여 전체 BER 성능이 크게 저하
될 수 있다. OFDM 방식에서는 일반적으로 전방오류정정 부호((070810 error correction
code)S 함께 사용하여 다중경로 채널의 주파수 선택적 페이딩 현상을 효과적으로 극복한
다. 오류정정 부호로는 블록 코드(0100 0006)의 일종인 RS(Reed—Solomon) 코드와 AS
루션 코드가 널리 사용되며, 대역폭 ASS 향상시킨 TCM(Trellis Coded Modulation),
두 개의 서로 다른 부호를 직렬 결합하여 사용하는 60ㅁ08[608160 코드, 터보(02200) 코드,
LDPC 코드 등이 사용된다.

부호화를 ACTH 랜덤 오류가 발생한 경우 정정 능력 범위 내에서 오류를 정정할 수
있지만 오류가 연집으로 발생한 경우에                                들어, 연속된
몇 개의 부반송파에서 오류가 발생하                               는       수
를 초과하게 되어 오류 정정에 실패할 수                                       위
류로 인해 비터비 알고리즘에서 잘못된
연집 오류(6419[ error) 현상을 극복하기 위하여 인터리빙0016068\108) 기법이 사용되며
이 기법을 사용하여 수신단에서 디코딩06000108) 전에 오류를 분산시킨다. 이와 같이 인
터리빙 기법은 연집 오류를 랜덤 오류로 바꾸는 역할을 한다. 인터리빙은 블록 인터리빙
과 컨볼루션 인터리빙의 두 가지 형태가 있으며, 블록 인터리빙에서는 비트 단위와 데이
터 심볼 단위, 그리고 OFDM 심볼 단위의 인터리빙이 모두 가능하다. 인터리빙의 종류
AS 결정하기 위해서는 사용하는 오류정정 Post 무선 채널의 주파수와 시간의 페이
딩 정도, 그리고 인터리빙에 따른 지연을 모두 고려하여야 한다. 그림 4.34는 Eureka—147
기반의 DAB 시스템에서의 사용되는 오류정정 부호(6000866080660 0006)와 인터리빙의 예
를 보여준다.

Lo

re

204


===== PAGE 203 =====
제4장_야ㅁ0\/ 기초

Inner
Data     Outer     Outer         |     Inner
Source | "| Coder | | Interleaver |” | 8 “1 interleaver [>] Mapper

RS(204, 188, t=8) Convolutional punctured All block-based
shortend code interleaving convolutional _ time (bit-wise)
coding     interleaving

correct up to 8 seperate error

a) ee in _ bursts from mother code        symbol           OFDM
4 bytes    inner coding : 1/2, k=7       |}        System
system   C(71, 133)   feguen
AS(255, 239, 8)                                                00)
original code                   pupctuny 8,     0
(permutation)
Inner
Data      Outer       Outer                  Inner
Sink | |060006| | Deinterleaver     becoder | Deinterieaver/* | Demapper

그림 4.34 DAB 시스템에서의 AKSEIE concatenated 부호와 인터리빙의 예

00000 ee ee

방송용이 아닌 셀룰러 이동통신, 무선 LAN 등의 일반적인 통신 시스템에 OFDM 전송
방식을 사용하는 경우에는 다중 접속(0ㅁ1414016 800688)을 위한 7450 필요하다. 단일 반송
파 시스템에서와 마찬가지로 OFDM 시스템의 다중접속기술로는 11044ㅅ(11076-12116107ㅁ
Multiple Access), FDMA(Frequency—Division Multiple Access), ae ee
Multiple Access)7} 있다. 그림 4.35 OFDM 전송 방식과 다중접속기술을 결합한 구조를
보여 주며, OFDM—TDMA, OFDMA(OFDM-FDMA), 저어 벼개어벼패해 애제버은
정의된다[971.

Time OF OM symbols

2
2
는
i
cS)
2
=,
n
>
요
=
®o
>
leg
2
uw

<OFDM-TDMA>        <OFDM-FDMA>        <OFDM-CDMA>
그림 4.35 OFDM 시스템에서의 다중접속기술

205



===== PAGE 204 =====
PART 1 야04과 MATLAB

OFDM-TDMA 방식에서는 각 사용자가 할당된 타임 슬롯 동안 전체 부반송파를 모두
사용하며, 사용자의 요구에 따라 할당하는 심볼 수를 달리하여 자원이 할당된다. OFDMA
에서는 전체 부반송파 중 일부의 부반송파를 할당하며, 사용자의 요구에 따라 할당하는
부반송파 수를 달리하여 자원을 할당한다. OFDM-CDMA 방식에서는 각 사용자가 시간
과 부반송파를 공유하여 사용하고, 각 사용자는 고유의 확산 부호를 통해 구분된다.
OFDM-CDMA 방식은 확산 부호의 AQ Blo] 따라 MC-CDMA, multicarrier
DS-CDMA, MT-CDMA® 구분된다[98]. OFDM—TDMA, OFDM—FDMA, OFDM-—
CDMAA} 지원 가능한 사용자의 수는 각각 타임 슬롯의 수, 부반송파 집합의 수, 확산
코드의 수에 의해 결정된다.

다중 사용자가 OFDM YAS 사용하여 접속할 경우 다중 접속 간섭0441: Multiple
Access Interference)o] 발생할 수 있다. 다중 접속 간섭은 발생 범위에 따라 셀내(00ㅁ8-
cell) 또는 WZHinter—cell) 간섭으로 구분할 수 있는데, OFDM-TDMAU} 0『1004ㅅ에서
는 셀간 간섭만 존재하며, 모든 사용자 또는 모든 기지국이 동일한 부반송파를 이용하는
OFDM-CDMA 방식에서는 셀내 간섭과 셀간 간섭이 모두 존재한다. 각각의 다중 접속
방식에 대하여 간섭 완화 방법을 살펴보면 다음과 같다. OFDM-TDMA 방식에서는 한
사용자가 전체 USS 모두 사용하므로 A 간섭을 완화하기 위해서는 간섭 회피
(interference avoidance) 기법 또는 낮은 주파수 재 AH2E(FRF: frequency reuse factor)
의 셀 구축 기법 등이 필요하다. OFDMA 방식에서는 하나의 셀내의 사용자 들은 서로 다
른 부반송파를 할당 받기 때문에 셀내 간섭은 존재하지 않지만, 서로 다른 기지국 또는 다
셀에 속한 사용자들은 동일한 자원을 사용할 수 있기 때문에 셀간 간섭이 발생할 수
다. OFDMA 방식에서는 간섭 회피 또는 간섭 평균(10160600006 averaging) 기법을 A}
하여 셀간 간섭을 완화할 수 있다. 081084-01084ㅅ에서는 모든 사용자가 또는 전체 부
반송파를 사용하여 송ㆍ수신하고 확산부호를 사용하여 사용자를 구분하기 때문에 확산부
호의 직교성이 파괴되는 경우 셀내 또는 셀간 간섭이 발생할 수 있으며, 다중사용자 검출
(004104-486『 detection) 또는 간섭 평균 기법을 이용하여 간섭을 완화할 수 있다.

OFDM-TDMA 방식에서는 각 사용자가 전체 부반송파를 사용하기 때문에 자원 사용
효율을 고려할 때 크기가 작은 가 적합하며, 셀간 간섭 완화를 위해서는 낮은 주파수
재 AMES 사용하는 셀룰러 시스템 또는 무선 Ｌ4씨과 같이 독립적인 A 환경에 적합하
다. OFDMA A= 전체 부반송파 중 일부의 부반송파를 각 사용자가 사용하기 때문
에 큰 크기의 FFT7} 적합하다. 또한 각 사용자에게 부반송파 할당 시 셀간 간섭을 최소화
하게 부반송파를 할당할 수 있기 때문에 주파수 재 사용률이 1인 셀룰러 시스템에 적합하

of 32 10

206


===== PAGE 205 =====
제4장_(0ㅁㅁ\/ 기초

0
|
|

다. OFDMA 방식에서는 사용자별로 채널 상황이 다르기 때문에 각 high 조
수 USS 할당함으로써 다중사용자 다이버시티(0274104-4660 diversity) 효

xo 터

는 장점이 있더, 그러고

상향링크 전송 시 각 사용자는 사용 가능한 부

}숙파 2 yee
반송파 중 일

에 해당하는 부반송파를 사용하므로 단말의 송신 전력이 제한된 상황에서 부반송파에 할

당된 전력의 증가에 따른
= 사용자가 넓은
diversity) 효과를 얻을

Ax 1]
수 있는

용한 경우 전송방식을 비교한 것이다.

EE 4.2 OFDM 시스템에서의 다중접속

all subcarriers
variable no, of time slots

none
present

interference avoidance
(low FRF)

small FFT size
isolated cell (wireless LAN)

OS 야미/7에서의 자

대역을 통해 데이터를

장점이 있다. 표

기술 비교

subset of subcarriers

variable no, of
subcarriers
|
none
present

interference avoidance
interference averaging
large FFT size
esilular system
multi-user diversity
power concentration

 OFDMA] 부채널 할당 방식

전술한 바와 같이 051084ㅅ에서는 전체 부

당하며, 사용자의 요구에 따라 할당하는 test +8 welts 자원

부
(subchannel) 인접 또는 랜덤하게 분포된 부

is]

“Er eu

뿌
Ea
=
I
a
mun

셀 커버리지 확장 효과가 있다. OFDM-CDMA 방식에서는 모
전송하므로 주파수 다이버시티(6ㅠ604600%
4.2는 OFDM3} 다중접속기술을

을 함께 사

one user/subset of time slots/  multiple users/same time/ all users/same time/

all subcarriers

variable no, of

spreading code
present
present

multi-user detection
interference averaging

inherent frequency
diversity

207



===== PAGE 206 =====
PART I[_OFDM2} MATLAB

1011 10001,
111111111111111 ,
| I  | | ha ani  Ll ㅣ   f
[111 1111 111 11 ,

Random type(cell 8)
그림 4.36 OFDMAO|A2| 자원 할당 방식

택하여 그룹화한 것으로 일반적으로 자원 할당(0604706 81008000)의 최소 단위가 된다.
그럼 4.36에 나타난 바와 같이 부채널은 자원 할당 방식에 따라 크게 블록 타입, Comb 타
입, 랜덤 타입으로 Bee 수 스 있다.

블록 타입으로 구성된 부채널에서는 물리적으로 연속된 부반송파들이 묶여 대역 별로
부채널이 구성되며, 클러스터 타입, Localized 타입, 밴드 타입 FO] 이름으로 불린다. 단말
의 이동성이 작고 안정된 채널 상황에서 주로 사용되며, 각 블록 별로 채널 상황에 적함하
게 AMC(Adaptive Modulation and Coding)S 할 수 있어 4=8(throuput)2 최대화할 수
있다는 장점이 있다. Us| Oe coherence 대역폭 이내로 BSS 구성하고 해당 블록만
채널 추정을 하면 되기 때문에 채널 추정이 간단하다. 블록 타입을 사용할 경우에 다이버
시티를 얻기 위해서는 부반송파를 클러스터 단위로 묶은 뒤 주파수영역에서 호핑을 한다.

Comb 타입으로 구성된 부채널에서는 등간격의 부반송파들로 부채널이 형성되며,
Interleaved 타입으로도 불린다. 하나의 부채널이 전 대역에 퍼져 있기 때문에 다이버시티
이득을 얻을 수 있으나, 인접한 셀에서 comb 타입의 부채널을 사용할 경우에 AZ 간섭이
매우 증가할 수 있어 주파수 재 사용률이 1인 셀룰러 시스템에는 적합하지 않다.

랜덤 타입으로 구성된 부채널에서는 하나의 부채널이 전 대역에 랜덤하게 퍼져있기 때
문에 다이버시티 이득과 간섭의 랜덤화 효과를 얻을 수 Yn}, distributed 타입, 블록 랜
덤 타입 등으로 불린다. 채널 추정을 위해서 전체 대역에 퍼져 있는 WUeS 사용해야 하
는 단점이 있다. 높은 이동성을 갖는 단말에게 적합하며, 인접한 셀간에 충돌이 발생되는
부반송파의 수가 최소가 되도록 랜덤 할당함으로써 주파수 재 사용률이 1인 셀룰러 시스
템에서도 적용 가능하다. 그림 4.36에 주어진 랜덤 타입의 부채널 구조에서 인접한 AA

ke 오
그

208


===== PAGE 207 =====
제4장_야미/ 기초

와 셀 BO] 일부 부반송파에서만 충돌이 발생된 것을 보여준다. 표 4.3은 OFDMA 2
채널의 자원 할당 방식을 비교하여 보여준다.

표 4.3 OFDMAOIA| 부채널의 자원 할당 방식 비교

adjacent subcarriers equidistant subcarriers random subcarriers

frequency hopping     frequency diversity          frequency
required                gain              diversity gain
slow                  fast                   fast
simple                |
whole band            whole band

(coherence BW)

coordination required coordination required interference averaging

그림 4372 랜덤 타입으로 구성된 다이버시티 부채널의 예를 보여 주며, 그림 4.382
블록 타입으로 구성된 밴드-4/40( 부채널의 예를 보여 준다.

icone~ㅣ”ee0000
] | 래 | , | | | | 아따~ beesUea

그림 4.38 블록 타입의 HHo-AMC 부채널

acs

WE-AMC 부채널을 사용할 경우 각 사용자에게 우수한 채널 특성
정하여 SNR} 따라 AMCS 달리함으로써 대역 효율성을 극대화한다.
AQAA 우수한 채널 SAS 갖는 US 선정합으로써 사용자 다이버시티 이
수 있다. 하지만 시간에 따른 채널의 변화가 심한 경우에는 피드백되는 채널 정
화도가 떨어지기 때문에 적응적 자원 할당 자체가 신빙성이 떨어지게 된다. 추가

백 채널 정보를 사용할 수는 있지만 그 만큼 자원의 손실이 발생한다.

ee 2 8

비벼

이 i
re ou
&
~

,

ne

n tA alo
ㅇ pO
N
에

fl

=

pm fr 4
Oo, {o
ot
[rl Je 00

4

209



===== PAGE 208 =====
PART Il_OFDM2} MATLAB

64 QAM
5/6 CC

의

: Subchannels of user A                                   Subchannels of user B

: Channel state of user A                                  : Channel state of user B

그림 4.39 HHS-AMC 부채널 사용 시 사용자 다이버시티 효과

 OFDMA 부채널 맵핑 방식
OFDMA] 부채널 맵핑은 송신할 데이터의 부채널 할당 방식으로 할당 정보의 차수
에 따라 1차원 맵핑과 2차원 맵핑으로 나눌 수 있다. 또한 시간영역 또는 주파수영역의 맵
핑 우선 순위에 따라 7601081 맵핑과 horizontal 맵핑으로 구분할 수 있다[991.

그림 4.40(a)= 1차원 vertical 맵핑에 대한 예를 보인다. 주파수 축을 우선으로 부채널
맵핑하는 방식으로 부채널의 옵셋과 길이가 일반적인 맵핑 정보로 사용된다. 한 타임
롯 내 전 대역의 부채널을 우선하여 사용함으로써 송신단에서의 짧은 전송시간과 수신
을 얻을 수 있지만 순간적으로 높은 전력을 사용해야 하기 때
에 기지국의 하향링크 전송 시 단말의 수신단에서 최대한 빠르게 디코딩을 해야 하는
주로 사용된다. 그림 4.40(06)는 1차원 horizontal 맵핑의 예를
핑하는 방식으로, 1차원 vertical 맵핑에서와 같이

부채널의 옵셋과 길이가 일반적인 맵핑 정보로 사용된다. 최소한의 부채널을 사용하여

타임 슬롯 동안 전송하기 때문에 한 데이터 버스트의 디코딩을 위해서 그 타임 슬
코딩 지연이 존재하는 단점이 있지만, 낮은
을 사용하여 ASS 할 수 있기 때문에 전력 소모가 중요시 되는 단말에서 상향링크
시 유리하다. 그림 4.40(0)는 2차원 맵핑의 예를 보인다. 2차원 맵핑에서는 부채널
(subchannel offset), 사용되는 부채널의 크기(040766 of used subchannels), 심볼
(symbol offset), 사용되는 심볼의 7|(number of used symbols)2] 4개의 파라미터를 사
용하여 1차원 맵핑에 비해 상대적으로 유연한 할당이 가능하다. 하지만 버스트 당 사용되
는 파라미터 개수의 증가로 맵핑 파라미터의 오버헤드가 상대적으로 증가하는 단점이 있

>

N
tho to [쏘 (제 off
oy 야 WY (우선

210



===== PAGE 209 =====
제4장_0『ㅁ0\/ 기초

subchannel
subchannel

1000

OFDM symbol                                                              OFDM symbol
(a) 1차원 vertical 맵핑                  (b) 1차원 40ㅁ20781 맵핑

subchannel

OFDM symbol
(0) 2차원 부채널 맵핑
그림 4.40 OFDMA 부채널 맵핑 방식

다. 일반적으로 2차원 맵핑 방식은 기지국에서 각 딴말에 하향링크 데이터 버스트를 할당
할 경우에 주로 사용된다.

OFDMA 신호의 강건한 ASS 위하여 주파수영역 확산 또는 시간영역 확산 방식을 사
용할 수 있다. 그림 4.4106)는 그림 4.41(8)에 주어진 5개의 부채널을 사용하는 QPSK 1/2
데이터 버스트를 3번 반복하여 15개의 부채널을 사용하는 0286 1/6 데이터 버스트로 주
파수영역으로 확산 한 결과를 보여준다. 이와 같은 방식을 통해 부호율은 저하되지만 주
파수 다이버시티를 얻을 수 있다. 그림 4.41(0)는 그림 4.41(8)를 시간영역에서 확산 하여
15개의 부채널로 확장한 결과를 보여준다. 이와 같은 방식을 통해 시간 다이버시터를 얻
을 수 있다.

211


===== PAGE 210 =====
PART Ｌ_ OFDMZ} MATLAB

QPSK 1/6

subchannel
subchannel

OFDM symbol                                                                   OFDM symbol
(a) 원신호                     (6) 주파수영역으로의 확산
089<1/6|

subchannel

OFDM symbol
(0) 시간영역으로의 확산
그림 4.41 OFDMA 확산 방식

| 416 vuplexing 기법

통신 시스템에서는 상향링크와 하향링크를 구분하기 위한 방식으로 FDD(Frequency
Division Duplexing), TDD(Time Division Duplexing)7} 널리 사용되며, 그 외에 상ㆍ하
향 링크 ASE 동시에 전송하는 21801 Duplexing 방식의 Zipper, TDD2} FDD2] 결합
형태인 HDD(Hybrid Division Duplexing) 등이 존재한다.

FDDE 상향링크와 하향링크에서의 신호 ASS 위해 서로 다른 주파수 대역을 할당하
는 방식으로 일정 보호 대역(64800 6800)에 의해 구분되는 한 쌍의 주파수 대역이 필요하
다. FODD= RF 단의 필터에 의하여 상ㆍ하향 주파수 대역의 크기가 미리 정해지기 때문

에 Bel] 상ㆍ하향 RF 부가 필요하고 FAV] 낮다는 단점이 있다. 그러나 FDDE
full—duplex 방식이기 때문에 지연 시간이 작고 Al 커버리지가 넓어 고속으로 이동하는
단말에 적합하여 셀룰러 시스템에 널리 사용되고 있다.

212



===== PAGE 211 =====
Al42t OFDM 기초

TDDE 각 상ㆍ하향 링크 별로 서로 다른 시간 SRS 할당하고 해당 시간 동안 동일한
주파수 대역을 사용하는 방식으로 각 시간 SRS 보호 시간(64000 0088/에 의해 구분된
다. 700에서는 동시에 상ㆍ하향 ASS 수행할 수 없으나 동적으로 상ㆍ하향 전송 슬롯
의 길이를 조정할 수 있기 때문에 상ㆍ하향 트래픽 량이 다를(050006010) 경우 유연성
(006061460이 높은 장점이 있다. 또한 TOD 상ㆍ하향 링크의 대칭적(500006010) 채널
특성 때문에 MIMO, 스마트 안테나, 링크 적응 기법, pre-compensation 기법 등을 적용
하기가 용이하다. 하지만 상ㆍ하향 링크가 시간에 따라 분리되기 때문에 시간 동기가 정
확히 맞아야 하고, 전파 지연 등에 의해 커버리지 영역 큰 경우에는 적합하지 않으며, 고
속의 이동속도를 지원하기 어렵다는 단점이 있다. 표 4.4는 FDDS} TDDE 비교하여 보여

표 4.4 FDD2} TDD] 비교

2 separate band for each link    :                    「
|      single channel (guard time)
(guard band)

AN

full duplex                  half duplex
low                         high
high (RX filter, etc.)                 low
wide coverage                small coverage
high        |                 10\
low latency                symmetric channel



===== PAGE 212 =====
4장에서 설명한 바와 같이 광대역의 고속 데이터 전송 시에 나타나는 주파수 선택적 채

널에 의한 왜곡을 OFDM 전송 방식에서는 다수의 직교 부반송파를 사용하여 병렬 전송힘
으로써 극복한다. 그러나 이와 같은 OFDM] 장점은 부반송파 사이의 직교성이 유지되는
경우에만 가능하다. 부반송파 사이의 직교성이 파괴되는 경우에는 10101016ㅠ-(1808001
10160616006)에 의하여 OFDM 시스템의 성능이 크게 저하되는데 직교성이 파괴되는 원인
중 하나는 수신단에서 동기화가 이루어지지 않은 경우이다[1]. 본 장에서는 심볼 타이밍 옵
Al(Symbol Timing Offset; 5700)과 반송파 주파수 옵셋(080060 Frequency Offset; CFO)
의 영향을 분석하고 OFDM 시스템에서의 동기화 기법에 대하여 설명한다. 4장에서 기술
한 바와 같이 수신단에서 동기가 이루어지지 않은 경우 이산시간에서 기저대역 신호는 다
음과 같이 주어진다.

N-1
y,[n]= yw itabata| 2728(사00+000 4 [7]                     (5.1)

k=0

여기서 6와 6 는 정규화된 반송파 주파수 BAL AS 타이밍 옵셋을 각각 나타낸다. 4]
(5.1)에서와 같이 동기화가 이루어지지 않은 경우 수신신호는 101와 ISI(Inter—Symbol
Interference)7} 발생하여 부반송파 사이의 직교성이 파괴된다.

OFDM 시스템에서는 변ㆍ복조가 IFFTS} FFTo|) 의해 각각 이루어지기 때문에 수신단
에서 OFDM 심볼의 시작 위치를 찾아내어 동기화를 시켜야 한다. 4장에서 설명한 것 같

214


===== PAGE 213 =====
제5장_동기화 기법

이 OFDM 심볼은 NV 개의 데이터를 IFFTS}o}] 생성되며, 연속된 두 OFDM 심볼 사이에는
ISIS} ICIS 방지하기 위한 CP(Cyclic Prefix)7} 삽입된다. 수신단에서는 N 개의 샘플신호
를 하여 복조가 이루어지기 때문에 샘플의 시작위치를 정확히 일치시켜야 복조가 이
루어진다. 채널과 잡음의 영향을 무시한 상황에서 심볼 타이밍 오차가 OFDM 심볼의 시
작 위치로부터 6 샘플만큼 발생한 경우, 시간영역 수신신호와 주파수영역의 수신신호는

다음과 같은 관계를 보인다.

~

표 5.1 SB 타이밍 옵셋의 영향
y[n]                               x[n+ 이

표 5.1에서 나타난 바와 같이, 수신된 ALSO] 위상은 심볼 타이밍 옵셋과 부반송파 위치에
따라 선형적으로 증가함을 알 수 있다. OFDM 시스템에서는 심볼 타이밍 옵셋에 따른 영
향은 6 의 위치에 따라 다음의 4가지 case 분류할 수 있다. 그림 5.1은 6 에 따라 FFT
시작 위치가 달라지는 4가지 경우를 보여준다.

Tg                                   Law                                 26      .                            Ley
cP                           1- th symbol                            CP                       (1+ 1) - thsymbol
i
Tmax                                 Case |                           |
Case Il                           |
Case Ill                          |
Case IV                          |

그림 5.1 심볼 타이밍 옵셋에 따른 FFT 시작 위치

향을 받지 않는 구간에 위치하는 경우이다. 표 5.1에서 나타낸 바와 같이 이 경우 수신신
SE 심볼 타이밍 옵셋의 크기에 따라 주파수영역에서 다음과 같이 위상 회전된 형태로

나타난다.

215



===== PAGE 214 =====
PART I1_ OFDMZ} MATLAB

1 썬             -jomkin _ 1 8S           joapsin XS 720,              00770).
=ㅜ21010      = 2 지210     Le * "=X[kle
n=0                               p=0

         ™                      5.2
은  5 alee _ ee sin[ #(k—2))]  _ |  for k=p             oe)
=                         sin| 2(k—p)/N |      0 for k#p
여기서 (는 / 번째 심볼의 《 번째 부반송파에서의 수신신호를 나타낸다. 이 경우 FFT

의 시작점이 보호 구간 내에서 이전 심볼의 영향을 받지 않는 부분이므로 191가 발생하지
않으며 부반송파 사이의 직교성이 유지된다. 그림 5.2는 0856 1과 Case 9] 경우 심볼 타
이밍 옵셋에 따른 성상도를 보여준다. 이 그림에 나타난 바와 같이 심볼 타이밍 Saye 위
상 회전을 발생시키며, 이 때 위상 회전량은 부반송파의 인덱스와 옵셋의 크기에
게 된다. 위상 회전은 주파수영역 l-tap 등화기로 쉽게 보상이 가능하므로 성능에 영향

주지 않는다.

Constellation                                              Constellation
1                                                         1                        és        en
ㆍ
러 2°                 ~.
ㆍ                            ,                        .
05                  -                                 0.5                          세
것
i                              [
%
2                                                    2        3
e °                                              a
5                               i
05                                             05     =                          는

6                   od
ee               of
J                         ㆍ        <a”         Case Il
* sTO=0                                       ereien         ° sTo=-3

FFT size = 128                                                    FFT size = 128

ci               05                0               0.5                1                                        1               -0.5                0               0.5                1
Real                                                                                                                                                        Real

그림 5.2 심볼 타이밍 옵셋에 따른 성상도(>-356 |, Case I!)

Case I (1 1)번째 심볼이 / 번째 심볼에 영향을 주고, Case IVE (1+-1)번째 AOI
/ 번째 심볼에 영향을 주기 때문에 이 두 경우 모두 191가 발생하고 / 번째 ABS) 직교성
이 파괴되어 101가 발생한다. Case 14의 경우 FFT 구간 내에 존재하는 신호는 다음과
같다.
x[n+6]                 for 0<n<N-6
ila] = eee  for N-8<n<N-I                 ipa

216



===== PAGE 215 =====
식 (5.3)에서 7 번째 심볼(위 식)을 복조한

써그-6
버1= ne 이 x[ntd]e 72990 =   woX [p]ei27PaN a
N  n=0               =0         n=0
At MSF jan Dn i n(p-k) N=    + sal OW 6)a(k-p 240
=                      sin| ^( k-p )IN |

4, SA 따른 위상회전이 발생하고 aed
서 (1+1)번째 심볼(아래 식)에 의한 영

그림 5.3은 Case III2} Case IV2] 경우

농하므로 이러한
의 경우에는 ICIS} 191의 영향이 심각하므로 이러한
타이밍 동기화가 반드시 수행되어야 한다.

Constellation
ㆍ
1        리      eo    <     =          1-2   =
ㆍ
~ 너너  é    be, -«                   |      년
“호 oo                 틱   e   “
ㆍ
ㆍ               ㆍ        |      . |
05     a  Ee   =                   Teg         05     ee  .°
* 3                  2 |        제   ㆍ
oe                            Cod   |            7 2
D        'e                         ee           ele
Ee 이   °     ~              “e°    H 9   ee amet i
e              ㆍ  ee
:                           ㆍ  oe
ㆍ
ㆍ          '          ㆍ          ㆍ
-0.5                    =                      —      -0.5 ㅣ          =
| 주                      세               ve     ㅣ
oe, ㆍ               vw ©                | *    버버
ㆍ       *      ° | ee
ㆍ
1                       ㆍ       Case Ill
4     g°ee 8     © sTO=-26         1             “1
FFT size = 128       |       ㆍ
=     =          I    zZ           ㅣ     _
1      0.5      0      0.5      f              4      -0.5

결과는 다음과 같이

위상

이.

De

그 2. 아아
n=N

 18    j2np(6-N, in 더

= Wi          6)

Fe  1+1  [ple         pen

Constellation

Real

옵셋에 따른 성상도(2356 Ill, Case IV)

qe -m ㄴㅇ
Case lV

제5장_동기화 기법
주어진다.
R gee,
5.4
N-6 for k=p   C4
#0 100 k#p

이 파괴되어 101가 발생한다. 또한 식 (5.4)에
으로 다음과 같이 191가 발생한다.

(5.5)

우 심볼 타이밍 옵셋에 따른 성상도를 보여준다. 그
림 5.3에서 나타난 바와 같이 심볼 타이밍 옵셋이 0보다 큰 경우
ISI7} 발생하여 성상도가 왜곡되는 것을 볼 수 있다. 이 왜곡은 복

=

회전과 함께 101와
조 이후에 복구가 불가
경우가 발생되지 않도록 심볼 타이밍 동기화를 해야 한다. 특히 Case 1V
상황이 발생되지 않도록 사전에 심볼

e 510=20
FFT size = 128 ||

05

217


===== PAGE 216 =====
PART Il1_ OFDMZ} MATLAB

OLED usm ams 옴셋의 영향

신단의 전송한 기저대역 신호는 발진기(080118601)에서 발생된 반송파 주파수에 의해
통과대역으로 천이040-000\619100)되며, 수신단에서 동일한 반송파 주파수에 의해 기저대
역 신호로 변환(00\04-000\679100)된다. 이 때 수신된 신호에는 반송파와 관련된 왜곡이
포함될 수 있는데 ASS 크게 두 가지 SAS 구분될 수 있다[94]. A 번째는 송신기와
수신기에서 사용하는 발진기의 특성이 안정적이지 못하여 발생되는 위상 잡음(01856
noise) © 주파수가 반송파 주파수 주위에서 시간에 따라 변동하는 것이다. 이와 같은 위
A} 잡음은 평균이 0인 랜덤 프로세스로서 \1606@ 프로세스로 모델링되며 OFDM 시스템
에 영향을 주기 때문에 이에 대해 많은 연구가 이루어져 왔다[100]-[102]. 두 Wale 송
신기의 반송파 주파수(./.)와 수신기의 반송파 주파수(./ '.) 차이에 의해 발생한 주파수
옵셋으로 PAS 신호는 /,,,=./. -/'.의 옵셋을 포함하게 된다. 이와 같은 반송파 주파
수 옵셋이 발생하는 이유는 송신기와 수신기에서 사용하는 발진기가 동일하지 않거나, 단
말의 이동에 따라 도플러 주파수 천이가 발생하기 때문이다. 도플러 주파수는 단말의 이
동속도와 반송파 주파수에 비례하며 다음과 같이 주어진다.

라

c

72 -                                          (5.6)

여기서 favs ㅇ는 각각 도플러 주파수, 단말의 이동속도, 빛의 AES 나타낸다. 표 5.2는
단말의 이동속도와 반송파 주파수에 따라 발생하는 도플러 주파수와 현재 상용화된
OFDM 시스템02508, 3GPP, 와이브로)에서의 정규화된 반송파 주파수 옵셋을 보여준다.

표 5.2 단말의 이동속도와 본   반송피 ft 주파수에 따른 도플러 주파수

3875MHz         1KHz        120km/h       41, 67Hz         0,042
38GPP          2GHz          15kHz        120km/h       222,22Hz        0.0148
와이브로       2,3GHz       9,765KHz      120km/h       295,55Hz        0.0263

표 5.20] 주어진 정규화된 반송파 주파수 옵셋은 다음과 같이 정의된다.

 218



===== PAGE 217 =====
제5장_동기화 기법

여기서 Sopa MEE Et 반송파 주파수 옵셋, 부                            규
화된 반송파 주파수 옵셋, 정수배 반송파 주파수 옵셋, 소수배 반송파 주파수 옵셋을 나타
낸다. 표 5.3에 나타난 바와 같이 반송파 주파수 옵셋이 존재하는 경우 시간영역

BE 송신한 신호 x(n] o] &의 위상회전을 곱한 결과가 되고, 주파수영역의 수신신호는
A

한 신호 X[K] 7} es 이동(68140)한 결과가 된다.

P

표 5.3 반송파 주파수 옵셋의 영향

yin)                       10 시

피시            X[k -€]

Frequency

그림 5.4 반송파 주파수 옵셋에 의한 ic) 발생

OFDM 시스템에서 반송파 주파수 옵셋의 영향을 자세히 설명하기 위해 송신기와 수신
기 사이에 주파수 옴셋만 존재하고 위상 잡음은 없는 경우를 가정한다[100][103]. 시간영
역에서 기저대역 수신신호는 다음과 같이 주어진다.

끼시지시 + 2 [in]                                (5.8)

Mi

=

>
1

0

219


===== PAGE 218 =====
a
<{
pa
ray
<x
=

PART Il_ OFDM

1  1  1  i  '  t    1  '   ^
i  1  1  1  |  1  1  1  내
ee ~… 데레
; « . a Fo a of 을 조노
'  '  1  1  )  1  '  1  1
1  1 {  |  ㅣ  ㅣ  1  1  1  '
'  1  1  ㅣ  |  1  1  t
'  1  '  i  t  1  |
ae a a ee ee oe ae wo
나 donb ab ind
1  1  1  1  t  1  1  1  1
1  1  '  i  1  t  '    '
1  1  1  i  i  '  ㅣ    1
ry te ew |
'
때 = 0 ~ 2 ~  ee | ~ :
imma i aan a a ee en te 거더
1  |  1  i  '  i  1  ㅣ  1
'  )  '  1  1  1  1  ㅣ
1  1  1  1  1  1  )  1  '
1  1  |  i  1  1  1  t  '
ee 제재 케메 제재 es 제제 제 테테 |)
여여 애사 이나 이 은
1  1  1  1  i  !  1  1  '
1  i  i  i  !  1  1  1
1  ㅣ  '  1  1  1  #  1
'  t  1  1  1  ㅣ  '  '
!
tee poe ee ae eee ee ee eee ae)
1  1  '  1  1  1  1  i  t
ri eee 도보 기복
ㅣ  1  을  1  ㅣ  '  '  '  1
'  1  1  !  '  1  1  1  ㅣ
1  1  i  1  '  1  1  1  t
Saleh leteis iietel ate eid Gee ater etal tater at 오모이
i  1  1  1  '  '  1  1  1
1  !  1  1  '  '  1  1  1
1  1  ㅣ  '  1  1  t  1  1
ㅣ  '  ‘  1  1  1  1  1
ㅣ  1  '  1  1  '  1  1  1
NDOODTN KH DOTA =
- ~ ES      of oc s&s
[pel] 020048:히10 06644

3 ead |

주

35

time

=0,1

(a) CFO

tot   은
1 1 1 이 그 로 | 의
1  1  1  1  '  t  1  ㅣ  '
ㅣ  1  t  '  i  1  '  ㅣ  1
ㅣ  1  )  1  '    '  ㅣ
|  “|  1  1    !  ‘   oO
re o-oo. of f    Hi     00
{    i «    !    '
'    1  1    1    1
'    1  1    1    1
1    1  1    1    1
6 츠                Lo
ii      7    7    T     N
ㅣ      1    '
!      '    1    {
H           1    i
ㅣ           ㅣ    '     ^
=           F    ul
;           }    {     띠
'           {    !      2
'           ㅣ    :      E
|      =
Masel          !    L     Lo
i               t     고
| 4             {
1  1             '
tof             {
  i             1
Penocneaebeadom= pom imap ten| tices a =
ㅣ  1  1  1         t
i te 4
1  1  1  1        P
Hn a 그 늬
a |
tiie Siete cae ele 수             wo
t  1  1  1    1  '  ㅣ
1  1  1  '    i  ㅣ  1  '
'  '  1  '    1  ㅣ  '  |
tea 4    1 을 4 4
| 1) | |    ee ee
NQotN-DQOtTAO
= a 수구 오오   Soce

time

=0,3

(b) CFO

35

T    T    T    T    T    T
'    t    1    1    '    1
'    !    '    1    '    i
1    1    i    ㅣ    1    !
ㅣ    i    1    J    ㅣ    1
1    i    1    '    '    1
대 ee ee ae a S
rt    }   1   i   1    02
|    1    ‘    '    '    '
ㅣ    1    '    '    1    1
'    '    (|    1    }    ;
!    i
bala ego hie Sere eae eat acess re)
7    1 4   7   1   1    nN
1    '    '    '    i    1
i    1    '    |    i    i
i    t    '    '        ，'
ㅣ    1    '    '    |    i
ee een eee eee, eee ~ 제타 ee |:
7   c aie |   1   1   7    q
t    ㅣ    1    1    \    1
i    1    i    |    i
ㅣ    1    ㅣ    ㅣ    1    1
ㅣ    ㅣ    1    '    1    1
er!eee hee ee ee aeeney Mee. OE | Ys)
분    1    1    1    i    i    ~
1    H    1
ㅣ    '    '    J    1
1    ㅣ    1    '    ㅣ    1
'    '    1    1    '    ㅣ
a은 Ncaneacnedoneed erst oocu eS
1    q    1    1    i    i    =
'        '    '    1    1
'        1    1    i    ㅣ
{        '    {    i    \
H        {    {    H    H
~ cee: Maine: See ee eee ee wo
1    1    1    !    ㅣ    1
'    '    1    1    i    {
{    1    ㅣ    |:    1    {
ㅣ    1    i    J    |    1
1    1    '        ㅣ    ㅣ    ^
+ 00 예 ㅜㅜ oO  주 후  oo
[091] 3046819]]1ㅁ 85640
ㅠㅠ -ㅠ-ㅠ8
°   |]   '   1   ‘   1   !
ou   ㅣ   '   ㅣ   {   1   {
11   |   4   ‘   -   H   {|
!    =
ro 1a
i
{
{
ㅣ
te)
{                    7180
1                    '
1                    1
ㅣ                    1
'                    ㅣ
호
내                    r   a
i                    '
i                    )
'                    1
i
eee                 ee rere be)
i                    7    ee
'                    !
1                    '
1                    ‘
{ㅣ                    '
i
ban 9 = =r---42
1
'                    i
1                    t
'                    '
---+                    +---10
|                    1
t                 i   1
i                 ㅣ   1
'                 ㅣ   |
1   i             1   '
(=)
+ MN ㅠㅜ OO  연 9? 자

time

1,3

(c) CFO

5.5 반송파 주파수 옵셋에 따

른
=

그림

220


===== PAGE 219 =====
제5장_동기화 기법

\

그림 5.5% 표 5.3과 식 (5.8)에 주어진 반송파 주파수 옵셋에 따른 수신신호의 위상성
분을 시간영역에서 보여준다. 여기서 NS 32, 데이터 심볼은 009로 가정하였고, 잡
이 없는 상황을 가정하였다. 그림 5.5(a)9h (bys 반송파 주파수 옴셋이 0.1와 0.인 경
의 시간영역 신호로 옵셋이 없는 경우의 AS} 비교할 때 시간이 지남에 따라 두 신호의
상 차이가 증가하며 그 때 증가을은 옵셋의 크기에 비례하게 된다. 그림 5.5의 좌측 그
림은 원 신호와 수신된 신호의 위상, 우측 그림은 두 신호 사이의 위상 차를 나타낸다. 그
림 5.5(이는 옵셋이 0.5 이상인 경우로 한 심볼주기 동안에 위상 차이가 *를 초과하게 되
어 phase ambiguity7} 발생한다. 이는 다음에 설명할 옵셋 추정 기법의 추정 범위와 밀접
한 관계가 있다.

음은 반송파 주파수 옵셋을 정수배 반송파 주파수 옵셋과 소수배 반송파 주파수 옵셋

0.
로 분류하여 주파수영역에서 수신신호에 미치는 영향을 설명한다.

oO.
ra
fe)

우

ae

ㅇ

수 옵셋의 영향을 보여준다. 정수배
큼 옴        J

셋이 발생한 것을 의미하기 때

의 반송파 주파수 옵셋은 부반송파 간격의 정수배만
문에 주파수영역에서 수신신호

그림 5.6에 나타난 바와 같이 정수배 반송파 주파수 옵셋이 존재할 경우 주파수영역에
서 순환 이동된 결과가 되어 이를 보상하지 않을 경우 심각한 BER 성능 열화를 발생하지

만 부반송파간의 직교성은 유지되므로 101는 발생하지 않는다.
조10]     =            <     2710]            20160    >               > X,[0—e,]
X,[1] —         l<«— zx,[1]         a, [ie —>|         ~ X,[1— 이
조[01 —>             <x— x,[2]              기 21608 —>             ㄴㄴ 조[2 - 이
N-point                                           N-point
(Transmitter)  :                                   :    (Receiver)
X,[N—2] —           <— x [N—2] 2,[W—2]e?™ 2g           t+ x [lv—2] —2)
X,[N-1] —>         <—2,[N-1] 2,[N—1Je?™ 0           > X[[N—-1]—e1]

그림 5.6 정수배 반송파 주파수 옵셋의 영향

221



===== PAGE 220 =====
PART Il_ OFDMZ} MATLAB

소수배 반송파 주파수 옵셋이 발생하면 4] (5.8)의 수신신호는 FFT 이후 다음과 같이
표현된다[1001

sin 7€

4 k = jme(N-1)/N
ilk] =e    ye

ja ta) 0K) Z08         (5.9)

여기서 LL 소수배 반송파 주파수 옵셋에 의한 ICIS 나타낸다. 식 (5.9)에 나타난 바
와 같이 반송파 주파수 옵셋이 존재할 경우 k 번째 부반송파의 진폭과 위상이 왜곡(첫 번
A 항)되고, 인접 부반송파에 의한 간섭(두 번째 Bo] 발생함을 a 수 있다. 인접 부반송
파에 의한 간섭 LA] 다음과 같이 주어진다.

7/.[4]= 66008 3 Him|X,[m]               sin Z€                 22200
'        스이 1790600-/+6)/00)          (5.10)

m#k

위 식에서 반송파 주파수 옵셋이 존재할 경우 부반송파간의 직교성이 파괴되어 101가
wine 일 알 수 있다. 그림 5.7은 식 (5.9)과 식 (5.10/에 주어진 반송파 주파수 옵셋의 영
+g 살퍼보기 위하여 수신된 3개의 연속적인 OFDM AES 보여준다. 여기서 채널과 잡
음의 GBS Tela] gO, 심볼 타이밍 gato) 없다고 가정하였다. 그림 5.761 나타
난 바와 같이 옵셋의 크기가 작은 경우 식 (5.9/의 첫 번째 항에 따라 진폭과 위상왜곡은
회전하면서 그 크기가 변화하는 AS 알 수 있으며 시간이 지남에 따라 회전이 일정하게
지속되는 것을 확인할 수 있다. 하지만 옵셋의 크기가 증가함에 따라 진폭과 위상왜곡이
증가함과 동시에 식 (5.9)의 두 번째 Bel ICL] 영향이 증가하는 것을 알 수 있다.

모

35         4         05          0         05          1          18 AS         A         05

0
그림 5.7 반송파 주파수 옵셋 존재 시 수신 신호의 성상도


===== PAGE 221 =====
제5장_동기화 기법

function [rxframe] =add_sto(rxframe, iLength, iSTO)

add symbol timing offset

rxframe : received signal

iLength : length of received signal

iSTO    : symbol timing offset

if iSTO>=0, rxframe=[rxframe(iSTO+1:iLength) zeros(1,iSTO)];% advance
else rxframe=[zeros(1,-iSTO) rxframe(1:iLength+iSTO)]; % delay

end

00 A WP Ol?

기

수

에

프로그램 5.1 심볼 타이밍 옵셋 발생

(
1

function y= add_cfo(N_FFT, dDefined_ CFO, iLength, rxframe)

% add carrier frequency offset

% N_FFT = fft_size

% dDefined_ CFO = fractional cfo + integer cfo

i=l:iLength; y = rxframe(i) .*exp(j*2*pi*dDefined_CFO* (i-1) /N_FFT) ;

Il 프로그램 5.2 반송파 주파수 옵셋 발생 함수

OLED 심볼 타이밍 옴셋의 추정 기법;

OFDM 시스템에 심볼 타이밍 옵셋이 발생하면 위상 왜곡 또는 Ist 발생한다. 위상
왜곡만 발생한 경우에는 수신단 등화기로 보상이 가능하지만, 161가 발생한 경우에는 송신
신호를 복원하기 어렵기 때문에 심볼 타이밍의 동기화가 필요하다. 이 절에서 설명하는
심볼 타이밍 동기화란 OFDMS] 심볼 단위로 가 수행되므로 [의 시작 위치를 추정

= OF

하는 것을 의미하며, 5.5절과 5.6절에서 설명하는 샘플링 동기화와는 구별된다. 심볼 타이
밍의 추정 기법은 크게 시간영역 기법과 주파수영역 기법으로 구분되며 본 절에서는 이에
대하여 설명한다.

223


===== PAGE 222 =====
PART 1 _ 야미/과 MATLAB

제

OFDM 심볼 타이밍은 주기적인 시간영역 신호를 이용하여 추정할 수 있다. OFDM 심
Be 개의 ABS 구성된 보호구간(70)과 NA] 샘플로 구성된 유효 데이터 구간
(7.0)으로 구성되어 있다. 보호구간은 유효 데이터 구간에서 뒷부분의 No 7] 샘플고
으     ㅇ

바그

LENS                                        ㅇ

일한 CP(Cyclic 『7603)로 구성되므로 OFDM 심볼은 주기적인 형태를 가지며 이 YAS

이용하여 심볼 동기화를 이룰 수 있다. CPS 이용하는 방식은 별도의 동기용 훈련신호를

사용하지 않으므로 심볼 동기의 추적과정에도 사용될 수 있다. AS 동기화의 다른 방법
<

으로 주기적 구조를 갖는 훈련 (training symbol)S 구성하여 전송한 후 이를 이용하

Aw
심볼 동기를 이루는 방법이 있다.

그림 5.82 CPS 이용하여 심볼 옵셋을
개의 OFDM 심볼이 있을 때 구간 8의 샘플은 구간 B'S] 샘플과 송신 시 598 oe 수신
신호는 다중경로 채널과 잡음에 의해 영향을 받기 때문에 a BS 구간 B'S] 샘플이
동일하지는 않지만 다른 영역의 샘플에 비해 큰 유사성을 갖는다. 그러므로 수신단에서
길이가 Te 이고 서로 Tash 떨어진 두 개의 윈도우 \1과 \2를 구성한 후 윈도우를 이
동하면서 심볼 동기를 찾게 된다.

c
alo
jaa
ee
N

w "
ㅇ

Tg         22       26
| 0 |  (1 - 1) - th symbol   cp    1- th symbol       cP     (1+ 1) - th symbol
A      B      6        BID
‘wt |            | \2 |
Tg    AS sliding window a
그림 5.8 Cyclic prefixE 이용한 AS 동기 시점의 추정 기법

여기서 \1 윈도우의 시작위치가 구간 BO} 시작위치와 일치할 때 \1의 샘플과 \2의 샘
플이 가장 유사하게 되어 두 윈도우 사이의 오차가 최소가 된다. 두 윈도우내의 샘플간의
오차를 비교하여 그 오차가 최소가 되는 순간을 심볼 동기 시점으로 설정할 경우 다음과
같이 주어진다[104].

A        Ng-l+6
5=aremin| » 비가          (5.11)

224



===== PAGE 223 =====
제5장_동기화 기법

Ng-l+6
é= agin} 2, lyf n+il-y, [n+ N +i] |          (5.12)

위와는 다르게 윈도우 \1의 시작위치가 구간 8의 시작위치에 있을 때 두 윈도우 WI
과 \2의 샘플 들은 최대의 상관값을 갖게 되므로 다음의 ML (Maximum Likelihood) 추

정 기법을 사용하여 심볼 동기 시점을 추정할 수 있다.

ae

ER   e{y,| n+ily, 000           (5.13)

= arg max

&>

그러나 식 (5.13)에 주어진 ML 추정 방식은
어 있을 경우 성능이 저하된다. 수신신호로부

추정 기법은 다음과 같이 주어진다[106].

수신된 신호에 반송파 주파수 옵셋이 포함되
부터 log-likelihood 함수를 최대화하는 ML

Ng -l+d

Oy, = argmax 2 aa p)Re{y,[n+i]y;[n+N+i]}-p > ‘i 0+1- sven] (5.14)

여기서 p= SNR/(SNR+1)-& 나타낸다. 위 식에서 상관을 취하는 과정이 많은 계산량을
필요로 하므로 수신신호를 양자화하여 계산량을 감소할 수 있다. 또한 반송파 주파수 옵
셋과 심볼 동기 시점을 동시에 추정하는 ML 추정 기법이 제안되었는데 이 경우 심볼 동

기 시점의 추정은 다음과 같이 이루어진다[107].

by, = arg max {|7[5]| — p [d]}                (5.15)

여기서 (5) 2} @(0) 는 다음과 같이 주어진다.

225


===== PAGE 224 =====
PART Il_OFDM2Z} MATLAB

y[m] =    DE    [n]y, [n+N],
내                                                                (5.16)
SNR

Ls
m|=— , 00  ] [+] ,     P= R41

n=m

A} (5.16)에 나타난 바와 같이 상관의 절대값을 취하기 때문에 반송파 주파수 옵셋 존재

때
시에도 그 영향을 받지 않고 심볼 동기 AGS 추정할 수 있다.

(2) 훈련 신호를 이용한 추정 방식
훈련 ASS 이용한 HAS 훈련 ASS 전송한 후 수신단에서 이에 해당하는 수신신호
를 사용하여 시간영역에서 심볼 동기를 이룬다. 훈련 AES 이용한 WIS 보호 구간을
이용하는 방식에 비해 심볼 동기를 획득하기 위해 훈련 심볼을 전송해야 하기 때문에 2
버헤드가 존재하지만 다중경로 채널의 VES 받지 않는 장점이 있다. 이 방식은 두 개의
동일한 OFDM 훈련심볼을 사용하거나 반복적 구조를 갖는 하나의 OFDM WES 사용하
는 경우에 효율적으로 적용할 수 있다. 시간영역에서 반복되는 훈련신호는 주파수영역에
서 데이터 사이에 OF 삽입하여 발생한다. 그림 5.9는 반복 주기가 2인 하나의 OFDM 심
볼을 사용하는 예를 보여준다.
Tranning symbol          Data symbol
276         1.        기
cp         |         cp
A! 6         C         D                  t
|. 00    — shift

“7.2      N, sliding window

그림 5.9 훈련심볼의 반복적 구조를 이용한 심볼 동기 |

그림 5.9에 나타난 수신신호의 et A, B, DE 구간
방식과 마찬가지로 두 개의 ALPS 형성한 후
기를 이룰 수 있다[108][1091.  aad | 최소 오차를 적용한

off v

쓰 0,
4

é= arg min    >

i=d

(5.17)

y,[n+i]-3, [na]

ML 방식을 적용하면 다음과 같다.

 226



===== PAGE 225 =====
제5장_동기화 기법

2
시 146

 vilei]y; | nA

i=d

5 = argmax                                               (5.18)

2
Nias
5

> y  Pre
120       2

그림 5.9에 표현된 구간 BE 보호구간이므로 이 무간내의 (;-2) 번째 심볼의 영향을 받
지 않는 부분을 심볼의 시작으로 인식해야 하는데 다중경로 채널의 영향으로 최소 오차값
이나 최대 상관값이 C 구간 내에서 발생할 수 있으므로 이를 방지하기 위해 오차값이 특
정 임계치 이하나 상관값이 특정 엄계치 이상인 al 번째 위치에서 심볼 동기를 찾는다. 상
기 설명한 방식은 반송파 주파수 옵셋의 GES 받지 않으며 심볼 동기 AAS 추정할 수
있지만 식 (5.17)과 식 (5.18)에 나타난 바와 같이 윈도우의 크기가 N/2 이므로 Bol 해당
하는 보호구간의 길이만큼 상관값이 평탄한 gh(flat interval)S 갖게 되어 정확한 심볼의
시작위치를 찾기에는 어려움이 있다.

상관값이 평탄한 값을 갖게 되어 정확한 심볼의 AAAS 찾기 어려운 단점을 극복하
기 위해 Minne 보호 구간 길이만큼 상관값을 모두 BES 취해 심볼 동기의 시점을 +
정하는 FAS 제안하였다[103]. 이 방식은 다음과 같이 주어진다.

^

jaggy :  위 soem]      (5.19)

Ne + 1 m=—-Ng +i

여기서 s[n] & 다음과 같다.

N/2=146                                               2

0 01007 [n+ +s]

0

Al (5.19)을 통해 정확한 심볼의 시작점에서 상관값이 최대값을 갖게 된다.
또한 그림 5.10에 we 바와 같이 훈련 심볼의 반복적 구조를 변경하여 심볼 동기 시
점의 추정 오차 범위를 좁힐 수 있다[1031.

5} [n] =

(5.20)

N=14+6

2 y, [n+ il

227



===== PAGE 226 =====
PART 1 OFDM} MATLAB

Tranning symbol                                   Data symbol
Tg                                              Tg

alal-al-a cP

oO
(ge)
ㅁ2

그림 5.10에 나타난 바와 같이 시간영역에서 4번 반복되는 훈련심볼은 3번째와 4번째
주기의 훈련심볼을 변경하여 심볼 동기 시점에서 추정 오차의 범위가 큰 단점을 극복할

nae                           =
수 있다. 그림 5.10] 나타난 심볼 동기 시점의 추정은 다음과 같이 이루어진다.

ys gata on 이 20 ol

(5.21)

See    MATLAB 프로그램 : 심볼 동기 시점의 추정     uae

end
+
(쓰
ne
of
ro

그림 5.11은 시간영역에      신호의 심볼 동기 시점의 추정을 보여준다. 상기
같이 심볼 동기 시점의 추정은 수신신호의 반복되는 패턴을 이용한      수

복되는 주기 0만큼 떨어진 y               는         i
기서 d= CPS 이용하는 경우 FFT size} 동일하며, =
턴의 주기가 된다. 그림 5.11에서 나타난 바와 같이 y[n]
오차를 가지며, 최대의 상관값이 나타난다.

Ps
eS
fot
be
그,
3)

as
my
thlo
bas
42 ph ae
x
로 변 시
&    ~
=   >
도그   os
ue   10
wi   bu
에
——    Ne
7    BY
ne   uot:
| 그 ty
주   x0
월 디존
6 ‘4 요 뚜 py

228

LAT



===== PAGE 227 =====
제5장_동기화 기법

0.25

은

ㅣ
1
1
1
'
1
1
4
4
1
1
{
1

ee ter ere Perera! Wen ee) Bene fen Cee ener ree! eee

2
a

Magnitude

=
—

SS ReneS he ears

OT ee ~

See ee oe       eee ty eee ae

1
‘
1
'
1
1

4
1
1
1
1
1
1
1
1

4
1
1
i
「
1"
'

0 -60 -4                                     80

Sample

그림 5.11 심볼 동기 시점의 추정

function [Esti_STO, dMagnitude] =A _C_CP(rx_sym,N ofdm,N _cp,Nfft)

% STO estimation using correlation
6 rx_sym : received signal

« Nofdm : Nfft +N cp

% N_cp    : CP size

% Nfft    : FFT size

% Esti_STO : STO estimated

dMax_value=0.00000001; Esti_STO=0; mnn=1:N_cp;
cpxTemp= rx_sym(nn+N_ofdm/2+Nfft) *rx_sym(nn+N_ofdm/2)';
dMax_value=abs (cpxTemp) ;
for n=1:N_ofdm
positl= rx_sym(n+N_ofdm/2) '*rx_sym(n+N_ofdm/2+Nfft) ;
posit2= rx_sym(n+N_ofdm/2+N_cp) '*rx_sym(n+N_ofdm/2+Nf£t+N_cp) ;
cpxTemp= cpxTemp-positl+posit2;
dMagnitude(n)= abs (cpxTemp) ;
if dMagnitude (n) >dMax_value
dMax_value=dMagnitude(n); Esti_STO=- (n-1-N_ofdm/2) ;
end

end

(al
{
of
ol
wo
a
(a ce
NI
[또
Jo
oz
mui
on
N
sy
ox
nol
4>

229



===== PAGE 228 =====
PART ㄴ_ 야미과 MATLAB

function [Esti_STO,dMagnitude] =M_E CP(rx_sym,N_ofdm,N_cp,Nfft) ;
* STO estimation using minimum error
Esti_STO=0; dMax_value=1000;
for n=1:N_ofdm
for m=1:N_cp
tmpl=rx_sym(n+N_ofdm/2+m-1) ; tmp2=rx_sym(n+N_ofdm/2+Nfft+m-1) ;
dMagnitude(n)= dMagnitude(n) + abs(tmpl*tmp1) +abs (tmp2*tmp2)
=2*tmp2*tmp1' ;
end
if (dMagnitude (n) <dMax_value)
dMax_value=dMagnitude(n); Esti_STO=-(n-1-N_ofdm/2) ;
end

end

기
[에
4>

Im! 프로그램 5.4 최소 오차 기반의 심볼 동기 추정

 주파수영역 추정 기법
Stel 발생한 경우 FFT 후의 복조신호는 식 (5.2와 같이 주어진다. 심볼 타이밍

상        나타나기 때문에 인접 부반송파간의 위상 차이를 이용
하여 심볼 BAS 추정할 수 있다. 모든 부반송파 k 에 대하여 #2,[4]=4,[4-1]이고,

X[k] 7} 동일할 경우 두 인접 부반송파 사이의 위상차를 이용하여 AS 동기의 시점을
Ze

호     N        Wel           *
b= Mare Sy 317 («-1)                           (5.22)

또한 상호상관 기반의 채널 임펄스 응담을 이용하여 심볼 S719] 시점을 추정할수 있
다[110]. 그림 5.12는 채널 임펄스 SHS 이용한 심볼 동기 추정 기법을 보여준다.

Timing Offset 6                     —e ancy            Timing Offset 6
OFDM 8060 | OFDM Symbol | >                          =       >  | i ‘

Hi
FFT output
FFT Window                                                                      IFFT output                           t

그림 512 채널 임펄스 응답

milo

이용한 심볼 동기 추정 기법

+i

230



===== PAGE 229 =====
제5장_동기화 기법

그림 5.12에 나타난 바와 같이 심볼 타이밍 옵셋이 발생한 수신신호에 훈련심볼을 Bal

서 위상 회전된 주파수영역의 채널을 획득한 뒤 1 연산을 통해 채널 임펄스 응답을 추

정할 수 있다. 이 때 추정한 채널 임펄스 응답은 심볼 타이밍 옵셋에 따라 다음과 같이 시
al

간영역에서 Aol(shift\s 형태로 나타나기 파문에  이를 이용하여 심볼 옵셋을 추정할 수
있다,
N=1
^ [n+6] =<   + [시지 [ke  j2A5KIN ㅡ     pee [x] H,[   [시고 13144
k=0
aS 기 11 사시                                                (5.23)
0

>

6 = arg max (h,[n+6])

그림 5.132 위 기법을 사용하여 추정한 경우에 심볼 타이밍 옵셋에 따른 채널 임펄스
응답의 예를 보여준다.

0.8

|         |         |         | | —esto:0

0.7 위 [+ -  -ㅡㅇㅇ 910: 10
바카
ee
204                                   en

10                - 20        25
sample

그림 5.13 심볼 타이밍 옵셋에 따른 채널 임펄스 응답의 al

이와 같은 주파수영역의 기법을 사용할 경우 정확한 SA WS 추정할 수 있어 미세 심
볼 동기 과정에 사용될 수 있다. 일반적으로 MIS 사용하는 60000 검출 방식의 경우
위상회전 값이 채널 추정치에 포함되므로 등화기에 의해 작은 심볼 타이밍 옵셋은 보상이
가능하다. 그러나 noncoherent 방식의 경우에는 HIRS 사용하지 않고 부반송파간 수신
신호의 위상 차이를 이용하여 송신 심볼을 복원하기 때문에 부반송파 《가 증가함에 따라
선형적으로 위상이 증가하는 심볼 옵셋의 영향을 송신 심볼 복원 전에 보상하여야 한다.

231



===== PAGE 230 =====
PART I1_ OFDMZ} MATLAB

6 3 | 반송파 주파수 emo 추정 기법

반송파 주파수 옵셋의 추정은 심볼 Salo} 추정에서와 마찬가지로 주파수영역과 시간
영역에서 모두 가능하며, 시간영역 추정 기범에는 00010 prefixS 이용하는 방식과 훈련

(1) Cyclic PrefixS 이용한 추정 기법
OFDM 시스템에서 심볼 동기가 이루어져 있
표 5.3에 나타난 바와 같이 시간영역의 수신신호
다. 채널의 영향을 무시할 경우 수신된 OFDM 심
진 신호는 반복되는 신호이기 때문에 수신신호의 Yo} 복소수 ＊'[]와 ylntN]S
fe)

하여 다음과 같이 반송파 주파수 옴셋을 추정할 수 있다.

을 경우 반송파 주파수 Salo] 발생하면
는 송신신호가 위상 회전되는 결과가 된
에

볼에서 cyclic prefix} N 샘플만큼 떨어

rh

1           cs +
6=그떠 > inven]           (5.24)

n=—NgG

위 식에서 잡음의 SES 제거하기 위해 보호 구간 동안에 평균을 취하였다. 식 (5.24)
에서 arg 는 100 0) 로 처리되기 때문에 추정 범위가 - 에서 +*로 주어진다. 즉, 식

(5.24)를 사용하여 추정할 수 있는 반송파 주파수 옵셋의 범위는 161< ao 따라서
OFDM 심볼의 cyclic prefix 이용하여 반송파 주파수 옵셋을 추정할 경우 정수배 반송
파 주파수 BAO 추정할 수 없다.

Weak 주과수 Bato] 0인 경우어는 [41110+4] 실수 값이 되기 때문에 eat 주

0

go] 발생한 경우에만 허수부가 00] 아닌 값을 갖게 된다. 따라서 vilalyin+ N]
의 허수부의 정보를 이용하여 반송파 주파수 옵셋을 추정할 수 있다[111]. 반송파 주파수
옵셋에 따른 오차는 다음과 같이 정의된다.

5 .

ㅇ
7

i<        !
e, = palm [ vil-nly,LN -7]]                                (5.25)

232


===== PAGE 231 =====
여기서 /은 상관 연산을 위한 샘플의 수를 나타낸다. 식 (5.25)에서 오차 6, 는 그림 5
와 같이 sin 함수로 나타나며 기대값은 4[%.]=ㅅ&* 로 근사화된다. 여기서 KE 송신 전력과
채널 전력을 포함한 요소이다. 따라서 정규화된 기대값은 4[%]=ㅎ의 증가함수로 근사화
되므로 &.에 대한 sin 함수 값에 따라 VCOS 조절하여 송신단과 수신단의 반송파 주파
수 동기를 이룰 수 있다. 주파수 지터는 Lol] 반비례하고 ?ＬＬ의 잡음 대역폭에 비례하게
된다. 이 방식의 반송파 주파수 옵셋의 추정 범위는 식 (5.24)에서와 마찬가지로 |6|<0.5
이다. 식 (5.24)에 나타난 &80 을 사용하는 방식은 상관 연산 결과 값의 실수부(60946)과
허수부(906)를 모두 이용하므로 유일한 를 추정할 수 있다. 그러나, 식 (5.25)에 나타난

는 방식은 상관 연산 결과 값의 허수부(626) 값만을 이용하므로 eo] 따른
유일한 를 찾을 수 없다. 따라서 최소 2회의 반복 수행이 필요하다.

반송파 주파수 옵셋의 절대값이 0.5 이상인 경우에는 60016 prefixS 이용한 방식을  "

용할 수 없다. 그러나 초기 동기화 과정에서는 발생할 수 있는 주파수 옵셋의 범위는
적으로 크기 때문에 넓은 범위의 옵셋을 추정할 수 있는 방식이 사용되어야 한다. 추정 범
위를 크게 하기 위해서는 상관을 구하는 두 샘플 사이의 거리를 단축시켜야 하는데 이는
일반적으로 훈련 ASS 사용하여 이루어진다. 예를 들어, OFDM 심볼이 심볼 주기 내에
2번 반복되는 패턴을 가질 때 x(n] a} x[nt+N/2E 동일하므로 [1]과 y[nt+N/2]
곱은 |] ㅇ이 되어 다음과 같이 SAS 추정할 수 있다[108][1091.

=
oln
일반

ㅇ

eas

on

to



===== PAGE 232 =====
PART ㅁ_야미/과 MATLAB

_ e= Late 시 {  y [n]y, [n+ N/ 2}                         (5.26)

n=0

는 |6|<1.0이 된다. 이 결과는 D 번의 반복적인 패턴의 경우로 쉽게 확
=  에서 2) 번 반복되는 패턴은 다음과 같이 주파수영역에서 comb 타
오를 할당하여 발생한다.

4. if k=D-i, for i=0,1,--,(N/D-1)

xUKl=|

otherwise

여기서 Ay 는 M-ary 심볼 중의 하나를 나타낸다. 2)번 반복되는 신호가 수신될 경우 반송
파 주파수 옵셋은 다음과 같이 추정할 수 있다.

é= 스가 시 yi [n]y[nt+N/ 기                                 (5.28)

n=0

~

위 반송파 주파수 옵셋 기법의 추정 범위는 |61<0.50가 된다. 위 기법을 사용할 경우 싱
관을 취하는 과정에서 사용되는 샘플 수가 DLE 감소하기 때문에 MSE 추정 성능이
저하된다. 그림 5.15는 상기 설명한 훈련 ASS] 주기에 따른 반송파 주파수 Sal 추정 기
Wo] MSE 성능과 추정 범위를 보여준다.

CFO
그림 5.15 훈련심볼의 주기에 따른 반송파 주파수 옵셋의 추정 범위와 MSE

234



===== PAGE 233 =====
제5장_동기화 기법

그럼 5.15에 나타난 바와 같이 짧은 주기의 훈련 신호와 긴 주기의 훈련 ASE 추정
범위와 추정 ell] trade-off WAS 보인다. 반복되는 짧은 주기의 훈련 신호에 대하
여 각각 추정 값을 구한 후 그 값들을 평균할 경우 추정 범위를 유지하면서 추정 성능을
향상시킬 수 있다
GRP] 주피수영역 추정 기법
동일한 두 개의 훈련 ASS 연속적으로 전송하는 경우 주파수영역에서 수신된 두 신호
간에는 다음의 관계가 성립한다
Y,[k]=Y¥, [ke                                             (5.29)

위의 성질을 이용하여 다음과 같이 반송파 주파수 옵셋을 추정할 + 있다[112].
e= Stan 226 [k] 10002  (tal)      (5.30)

A] (5.30)에서 tan 7} 2이므로 추정 범위가 0.5 이하로 제한된다. 위 방식의 추정 범

HS 증가하기 위해서는 식 (5.27)과 같이 DO Waste 훈련 ANE Aes Fae
주파수영역에서 0이 아닌 부반송파에 대하여 식 (5.30)을 적용한다. 이 경우 추정 범위가
추정 성능이

Dw 증가하지만 Bae 취하는 샘플의 수가 UD 로 감소허기 때문에 MSE
저하된다. 위 방식은 훈련 심볼을 사용하는 경우에만 적용이 가능하며 데이

볼 이후에 전송이 가능하다.

이와는 다르게 데이터를 전송하면서 miele ES 사용하여 주파수영역에서 정수배 반
송파 주파수 옵셋과 소수배 반송파 주파수 SS 추정하는 기법이 제안되었다[1131. 그
림 5.16은 TUS BS 사용하여 반송파 주파수 옵셋을 획득 WE (acquisition 20006)와 =
Al 모드(0800008 0006)로 구분하여 추정, 보상하는 TAS 보여준다.

그림 5.16에 나타난 바와 같이 획득 모드에서는 정수배 주파수 GIS 포함하여 넓은
범위의 반송파 주파수 옵셋을 추정하며, 추적 모드에서는 미세한 범위의 반송파 주파수
GAL 추정한다. 여기서 정수배 반송파 주파수 Va, &,,는 다음과 같이 추정된다.

205


===== PAGE 234 =====
PART ㅁ_ OFDMZ} MATLAB

y;[n]            memory                                         |
Filtered           ;                  N                                              i       yk]

renee | extraction     ~     N samples                     x)                        FeT unit | 비씨,                   Sena

‘              of OFDM                      of time slot (n)                                                                        7                              not
signal                                                                                                                                  é                    synchronization

blocks                                                              frequency

having                                                                      arnt                             N sub channels                  ee 28005

y(n]                    sync          u+olnll memory                          correction                                                                  이 19 때
subchannels                    N samples              LN                             FFT unit              /      +        00 and (n+D)

of time slot (xD)
Yi+D 시

—-                                                                                     LAG      ^

coarse timing                                                                       —                         -                             자야

ation                                                                  acquisition mode        tracking mode
a | : Maximum searching | : arg(.) operation
S| +arg(.) operation
time domain                                               때 |=                                ：
18] 5006    ¥i lil ec     :
Yi. pblile]      ¥4 p plilseccq!
frequency damain
그림 516 UA 톤을 사용한 반송파 주파수 옵셋의 동기화 과정

=

(¥,.0[ pL]. €]® [pL €]) (Xn0[ PL] 00      (5.31)

@ =    max
7 2n-T., 】 |

sub            j=0

=

여기서 L 은 spelel 톤의 개수, 2[/1는 전체 wea = 중에서 ) 번째 veda 톤의 위
나타낸다. ERX), ,121711와 XlpLi] = 각각 4D) 7 번째 심볼주기의 / 번째 파
톤의 위치에 실린 mele 심볼을 나타내며, 송신 신호의 영향을 제거하기 위하여 포함
었다. 소수배 반송파 주파수 Sal, “은 다음과 같이 추정된다.

Nu

ya af

|
]

=

muy

&,= spot re] (hol [i]s cy ¥ [PLDs 6 |) (Xo LPL] % [Pl ii) (5.32)

sub               y=

득 모드에서는 &,,와 를 추정하고 이 값의 합으로서 반송파 주파수 옵셋을 보상하
A 모드에서는 만을 추정하여 보    ae 이 방식에서 p]sl 톤을 제외한 나머지
반송파에서는 데이터를 전송하므로 WIS SS 사용하여 반송파 주파수 옵셋을 추적하
서 데이터를 전송한다.

로

획
머 주
부반
면

 236



===== PAGE 235 =====
제5장_동기화 기법

function [Esti_CFO]=time_cfo(r_ frame, iM,Nofdm, iWS, 102)

6 time-domain technique

6 r_ frame : received signal

% iM       : number of average symbols for performance improvement
% Nofdm    : symbol duration

6 iWS      : window size

6 iWD      : duration of repetitive pattern

6 D       : number of repetitive patterns

D=Nff£t/iWD; nn=1:iWS;

cpxTemp = 0;

for m=1:iM

cpxTemp= cpxTemp + r_frame(nn+iWD)*r_ frame(nn)'; nn = nn+Nofdm;
end
Esti_CFO=angle (cpxTemp) / (2*pi) *D;

—

BET 5.5 시간영역 반송파 주파수 옵셋 추정

ala
에
>

o oF
function [Esti_FFO]=CFO Moose(r. frame, Nsym, Nfft)
% frequency-domain technique
6 Nsym : number of same training symbols
temp=complex(0.,0.);
for j=1:Nsym
for Wel sNELt
temp=temp+ (rx_sym(j+1,i) *conj (rx_sym(j,i)));
end
end
Esti_FFO=angle (temp) /((2*pi)) ;
il 프로그램 5.6 주파수영역 반송파 주파수 옵셋 추정 함수

237



===== PAGE 236 =====
faa)
<
pi :
ool
<
>
더

샘플링 클럭 위상 옵셋의 영향

PART 1 _야0

=
“Or

이

위상 옵셋

그
클럭

샘플링

럭 위상 옵셋에 대해 설명한다.

프 크
플렁 클

다. 본 절에서는 샘

]

‘ox

렁 지점에서 일정 옵셋을 가지

로 복조 신호에 대해 5.1절에서 설명한 심볼 타이밍 옵셋이 발생

x=

셋과 같이 시간영역에서의 신호 지

+

플링 지점이 최적 샘

새
u

°   =
보는

!

A

J

XK

더

< 커

iL,

&

+3

플렁 클럭 위

Tx samples
Rx samples <>

2H
u

럭 위상 옵셋이 발생

가한다.

bo 중

반송파의 인덱스에 비례ㅎ

회

위

기

파에 발생하

40

a

at

H

이므로
}지만 샘플링 클럭 위상 옵셋의 크기

BA

ㅇ

Sze
=

것이 일반적이다.

=

속도가 일치하지 않는

플링 클럭 주파수 차이로 정의할 수 있다[115]. 그림 5.18은 샘플링

력 주파수 옵셋이 발생

|고 보상하

15

xX

여추

}하

호
|]

심볼 타이밍 옵셋에 비해 상대적으로 매우 작
보면

는 A
에

ㅣ

셋

옵

링 지점이 변화하므로 시간에 따라 샘

sai
g
xz

글

심볼 타이
시
플 구간마다 샘

|기보다는
샘플링 클럭 주파수 옵셋의 영향

+ AW

Ko)

히
도로 주정

238



===== PAGE 237 =====
제5장_동기화 기법

Tx samples <                         ><        ><       >
Rx samples              <>           <>        Jee      위
70              7              가              L       |

플링 클럭 주파수 옵셋은 신호 스펙트럼의 주파수 천이로 인하여 cy} 발생한다. 샘
속도의 차이로 인해 FFT 복조과정에서 부반송파 간격의 크기가 변경되므로 DCS

로 신호의 전체 스펙트럼 Zo] 샘플링 속도의 차이에 의해 증감하게 된다. 이 때 부

9 mule
yz 아 im of pt
[03

반송파의 주파수가 00에서 멀어질수록 ICV} 크게 발생하게 된다. 샘플링 클럭 주파수
옵셋이 발생한 경우의 복조 신호는 다음과 같이 주어진다.
:         jmAk(N-1)

Pk) = YR) Sine A®)      Ts worl          (5.33)

sin(mAk/N) ©

여기서 At (L.-T )7; 를 나타낸다. 위 Ao] 나타난 바와 같이 샘플링 클럭 주파수 옵
셋이 발생한 경우 5.2절에서 기술한 반송파 주파수 옵셋과 같이 부반송파의 진폭과 위상
왜곡이 발생함을 알 수 있다. 30/1씨는 다음의 BAS 갖는 샘플링 클럭 주파수 옵셋에

의한 10[를 나타낸다[1141].

2
vat Zi LAI] = 7 (Ak?                               (5.34)
또한 샘플링 클럭 주파수 옵셋이 부반송파에 미치는 영향은 심볼의 시작 위상에 따라
다르게 나타난다. 샘플링 클럭 주파수 옵셋이 존재할 경우에 샘플링 타이밍 옵셋은 매 심
볼마다 변화하며 1 샘플 삽입 혹은 누락 현상이 주기적으로 반복된다.

239



===== PAGE 238 =====
OFT wes 클럭 ou 보상 기법

샘플링 클럭 보상 기법은 샘플링 클럭의 제어 유무에 따라 동기(50000000009) 샘플링
방식과 ¥}§7|(non-synchronous) 샘플링 방식으로 구분된다[116]. 동기 샘플링 방식은
DPLLE 이용한 샘플링 타이밍 제어 방식으로 아날로그 단에서 보상하는 방식이며, 비동
기 샘플링 방식은 자유 샘플링 후에 디지털 단에서 보상하는 방식을 나타낸다. 그림 5.19
은 동기 샘플링 방식의 기본 블록도를 보여준다.

received                             data _
signal ——> 66          Fell             >

VCXO |€                  디기 에라이                   160

그림 5.19 동기 샘플링 방식의 기본 블록도

그림 5.19에 나타난 바와 같이 동기 샘플링 방식은 FET wpelyl 톤의 위상 회전을 이용하
이 일반적으로 사용되며 추정된 위상 옵셋을

oj 샘플링 클럭 옵셋을 추정하는 방식                                 이용하
여 PLL= 직접 VCXO(Voltage—Controlled Crystal Oscillator)S 제어한다. 최적 샘플링
지점을 계속 갱신하여 정상상태의 샘플링 오류에 의한 왜곡을 줄일 수 있는 장점이 있으나

정상 상태에 도달하는 데 일정한 시간이 소요된다. 또한 VCXOE discrete componento] 4
XO(Crystal Oscillator)o] 비해 가격과 잡음 지터가 높다.

비동기 샘플링 방식에서는 자유 샘플링을 수행하며 디지털 단에서 보상이 이루어지므
로 아날로그 단과의 연동이 필요 없다. 타이밍 오류를 등화기 만을 이용하여 보상할 경우
피드백 루프를 사용하는 방식인 동기 샘플링 방식보다 단순하게 구현이 가능하다. 그러나
이 경우 샘플링 속도가 제어되지 않으므로 샘플링 주파수 옵셋에 민감하게 된다. 따라서
비동기 샘플링 방식에서는 한 심볼 내에서 샘플의 삽입 또는 누락 현상이 발생하여 샘플
skip/duplicateS FFT 입력 전에 수행한다. 주파수영역에서는 FFT 출력 신호에 대해서는
위상 SAS 보상하는 위상 회전기가 사용된다.

그림 5.20은 시간영역 보간기를 사용한 비동기 샘플링 방식의 블록도를 보여준다.

qu

240



===== PAGE 239 =====
제5장_동기화 기법

16086 _,                          Skip/            interpol |.                  <|                        data.
signal                ADC                    Duplicate                   ator                       FFT                      FEQ                                     더
A
Fixed                                                                                                 PF
Xtal                                                                                      DPLL <              160

그림 5.20 ARIS 보간기를 사용한 비동기 샘플링 방식의 gee

그림 5.20에 나타난 바와 같이 샘플 타이밍 옵셋을 보상하기 위해 디지털 components
사용하며 일반적으로 FIR 보간기 필터가 사용된다. 위 방식은 VCXOS 사용하지 않는 장
점이 있지만 시변 필터를 사용하기 때문에 성능 열화가 나타날 수 있다. 성능 열화를 극복
하기 위해 오버샘플링 또는 고차 보간기를 사용할 수 있다.

그림 5.21은 비동기 샘플링 방식의 주파수영역 보상 기법을 보여준다.

Skip, /                                                제                                         data         S.
—»> ADC                  Duplicate                 FFT                    FEQ                                >
Fixed                                                                          a
‘etal                                                DPLL |<          TED



===== PAGE 240 =====
PART ㅁ_0001\4과

o     o   oon        o     a   — ¢ Kr
VCXO(NCO)                    XO
PLL(DPLL)                      FIR interpolation filter
Usage of VCXO is undersirable Performance degration
— higher cost & noise jitter    — Slowly time-varying ICI
than XO                   — Usually, require oversampling or
— discrete component             high-order interpolation filter
* Pilot tone—based             * Discrete time-domain correction
synchronization               ㆍ Hybrid time—domain/frequency—

omain correction

OG 셀룰러 시스템의 동기화 기법

본 절에서는 셀룰러 시스템에서 기지국과 단말간의 하향링크 동기화 기법과 상향령크 동

기화 기법에 대하여 설명한다. TOD 방식의 셀룰러 시스템의 경우에 pila  하향링크
의 대칭 SYS 이용하여 동기화와 채널 추정 등을 수행할 수 있지만, EDD 방식의 셀룰

시스템의 경우에는 상향링크와 하향렁크가 다르기 때문에 각 링크 별로 동   기이 채널 추정
과정이 필요하다. 그림 5.22는 일반적인 셀룰러 시스템에서의 동기화 과정을 보여준다.

Uplink compensation:               Compensated uplink signal                 _Uplink estimation
time, frequency, etc  6       7                     .         4   time, frequency, etc
compensation                                                         estimation

Y
Random access signal
>»

 Downlink sync. channel

Control channel:
uplink sync. info     다

A

Downlink sync:
frame, time, frequency sync. 2
cell seaching

그림 5.22 셀룰러 시스템에서의 셀 탐색 및 동기화 과정

242



===== PAGE 241 =====
제5장_동기화 기법

말을 a 이용하여 프레임 동기화. 심볼 타이밍 동기화, ¥   반송파 주파수 동기화를 수행하
고 단말이 속해있는 셀을 탐색한다. 하향링크 셀 탐색 및 동기화 과정이 완료되면 단말은
랜덤 엑세스 ASS 기지국에 전송한다. us    단말이 전송한 랜덤 엑세스 신호를 사
용하여 심볼 타이밍 옵셋, 반송파 주파수 옵셋, 전력 등을 측정한 후 제어 채널을 통해 상
향링크 동기 정보를 단말에게 전송 sath © 단말은 게지국이 AS 상향링크 동기 AHS

상기 설명한 셀룰러 시스템에서의 동기화 과정 중에서 본 절에서는 하향링크 동기화 과
정에 대해 설명한다. 셀룰러 시스템에서는 초기 동기화를 위해 단말기가 기지국의 ASS
수신하여 시간과 주파수 동기화 및 셀 탐색을 수행한다. 또한, 초기 동기 획득 이후에는
시간과 주파수 옵셋을 추적(480008)하며, 핸드오버(18000160를 위해 인접 셀의 시간, 주
파수 동기화와 셀 탐색을 수행한다. 다중 셀에 대한 고려를 제외하면 하향링크 동기화는
기존의 OFDM 기반 방송 시스템과 버스트(6050 2SJol]4]9} 유사한 점이 많다. OFDM
기반 통신 시스템의 하향링크 동기화 방식은 크게 프리앰블 기반의 동기화 방식과 mpeley
기반의 동기화 방식으로 나눌 수 있다. 방송 시스템의 예로, DMB 시스템에서는 널 심볼
(null symbol) 및 위상 기준 심볼(01866 reference symbol)2- 동기화에 사용하고, DVB-T
와 DVB-H 시스템에서는 HIS 동기화 및 채널 추정을 위하여 사용한다. 버스트 모
Wo) 예로, IEEE 802.118 무선 랜에서는 두 종류의 프리앰블(010ㅁ preamble, long
06000010)을 동기화 및 채널 추정을 위하여 사용한다. 셀룰러 시스템의 예로, 와이브로에
서는 프리앰블을 사용하여 셀 탐색과 하향링크 동기화를 수행하고, 3GPP-LTENAE
PSS(Primary Synchronization Signal)2} SSS(Secondary Synchronization Signal) 채널을
사용하여 셀 탐색과 하향링크 동기화를 수행한다.

프리앰블 설계 시 고려하여야 할 항목은 다음과 같다. 프리앰블을 구성하는 시퀸스는
좋은 자기상관과 상호상관 SYS 가져야 하고 낮은 PAPR SYS 가져야 한다. 낮은
PAPR 특성과 좋은 상관 특성을 갖는 AHA CAZAC 시퀸스, PN ABA, Gold 시퀸
스 등이 있다[117]. 각 시퀸스마다 상관 특성, PAPR 특성, SEE trade-off 관계가 있
으며 각 시스템의 요구사항에 따라 시퀸스를 선택해야 한다. 또한 넓은 범위의 반송파 주

=
=

243



===== PAGE 242 =====
PART 1Ｌ_야미4과 MATLAB

파수 옵셋을 높은 정확도를 갖고 추정할 수 있어야 한다. 5.4절의 반송파 주파수 옵셋의
보상 기법에서 기술한 바와 같이
위가 trade-off 관계가 있기
of 한다. 하드웨어 설계를 고
시 고려해야 할 항목이다.

프리앰블 기반의 동기화 기법에서는 초기 동기화를 수행하는 단말기가 우선 프레임의
Al 부분에 전송되는 프리앰블을 이용하여 프레임의 시작 위치를 검출(68006 066600400)한
다. 프레임의 시작 위치를 ABest 후 OFDM 심볼 타이밍 및 반송파 주파수의 동기화 과
AS 수행한다. 즉, 프레임을 검출한 후, 대략적인 심볼 및 미세 반송파 주파수 동기를 획
득하고 정수배 반송파 주파수 동기화, 셀 탐색, CINR 추정을 수행한다[118]. OFDM 기반
방송 시스템에서는 프레임 검출 또는 FFT 변환 전에 대략적인 심볼 및 반송파 주파수 동
기를 획득하는 경우가 있으나, TDD 기반 셀룰러 시스템에서 이와 같이 할 경우에는 상향
링크 구간에서 신호를 전송하는 단말에 잘못 동기화를 할 수 있기 때문에 일반적으
와 같은 순서로 진행한다. BUR 기반의 동기화 기법에서는 BES] 프리앰블 없이
규칙에 의해 배치된 Tel 신호를 이용하여 프레임 검출, 심볼 타이밍 및 반송파
동기, 셀 탐색, 채널 추정 등의 동기화 과정을 수행한다.

음은 와이브로 시스템의 하향링크 동기화 과정에 대하여 요약하여 설명한다[119]. 그

림 5.23(8)에서와 같이 PUSC ASS 사용하는 경우 각 셀은 3개의 섹터로 구성되며, 제어
심볼과 데이터 심볼에 대해서 섹터 간에 간섭이 발생하지 않도록 섹터 간 주파수 재 사용
Go] 1322 설정되어있다.

그림 5.23(9)는 와이브로 시스템의 각 섹터(세그먼트)에 따른 프리앰블 구조를
다. 그림 5.2306)에 나타난 바와 같이 세그먼트에 따라 다른 부반송파에 프리앰블 시퀸스
가 할당되며 단말은 이를 검출하여 단말이 속한 셀과 세그먼트를 추정할 수 있다. 와이브
로 시스템에서는 서로 다른 114개의 다른 프리앰블 AAAS 사용하여 32개의 셀과 그에

= 3개의 세그먼트를 추정할 수 있다. 와이브로 시스템에서 하향링크 동기화 과정은 1
ASE 구성된 프리앰블을 사용하여 이루어진다. 먼저 시간영역에서 3번 반복되는 프리앰
블 EAS 이용하여 자기 상관을 통해 프레임 검출이 이루어진다. 프레임 AS] 이루어
지면 cyclic prefixS 이용하여 소수배 반송파 주파수 옵셋을 추정한다. 정수배 반송파 주
파수 BAS 이후 셀 탐색, 세그먼트 추정, CINR 추정과 함께 이루어진다. 초기 동
기 획득 모드 후 추적 모드에서는 미세하게 심볼 타이밍 옵셋과 주파수 옵셋을 추적한다.
와이브로 시스템에서 하향링크 동기화 기법에 대한 자세한 USS 18장에 기술한다.

jn 때
Ae oot 이

> od

파

38

244


===== PAGE 243 =====
제5장_동기화 기법

(9) 와이브로 시스템에서의 셀 구조

DC
426                  425
|                1   |               1
ㅇ0ㅇ      | }    ㅇㅇㅇ   {    }  ㅇ0ㅇ }    }  |   000
0   85 86     511 512 513    "937938 1023

‘segment 0  *-seament 1  fseoment 2
(6) 와이브로 시스템의 프리앰블 구조
그림 5.23 와이브로 시스템의 셀 구조와 프리앰블 구조

2. 3GPP LTE 시스템에서의 동기화 기법을 요약한다. 그림 5.24는 3GPP LTE
동기 채널 구조를 보여준다120][121][3211.
3GPP LTE 시스템은 다수의 전송대역(1.25, 2.5, 5, 10, 15, and 20 MHz) 고려하고
있다. 따라서 3GPP LTES| 동기채널은 전체 대역폭 중 1.25MHz 대역에 150의 부반송
파 간격을 갖는 76개의 부반송파를 사용하여 전송되며 PSS(Primary Synchronization
Signal)2} SSS(Secondary Synchronization Signal) 채널로 이루어진다. 3GPP LTE2] 1
프레임은 10개의 서브프레임으로 이루어지며 PSS 와 Sss 은 서브프레임 02} 5번에 두
번에 걸쳐 연속적인 두 OFDM ASH 전송된다. 3GPP Ｌ8시스템에서는 504개의 서로 다
= 셀을 구분하며 3개의 물리계층 IDS} 그에 따른 168개의 물리계층 셀 IDE 이루어진다.

1 frame = 10 ms

1 TTl=1ms
Subframe 0                                          Subframe 5

06009 00062          i a |

이12131408이11231456                     이1121914158이112139141516
fj p-scH [{s-scHt [] s-scH2
그림 5.24 3GPP LTES| 동기 채널 구조

245



===== PAGE 244 =====
PART Ｌ _야미/과 MATLAB

크 동기화의 A 번째 단계로서 단말은 298를 이용하여 Sms 단위로
시간동기를 추정한다. 단말은 PSss  겸출함과 동시에 심볼 동기의 시점과 반송파 주파수
SAS 추정한다. 또한 288에는 고유한 물리계층 IDS 구분할 수 있는 _ a
사용되므로 단말은 물리계층 셀 IDS 찾기 전에 288를 통해 고유한 물리계층        출
한다. 두 번째 단계로서 단말은 988를 이용하여 물리계층 셀 IDS} 프레임 dite 검출
한다. SSSE 위 그림에 나타난 바와 같이 0번째 서브프레임의 9951과 SHA 서브프레임
의 8992로 구성된다. 단말은 (9991, 9982)을 검출함으로써 프레임을 검출할 수 있으며,
(9981, SSS2)2] 조합을 통해 물리계층 셀 내 검출함으로써 하향링크 동기화를 완료한
다. 3GPP LTES] 동기화에 대한 자세한 내용은 19장에서 기술한다.

「뿐
Ny

OFDMA 시스템의 상향링크 동기화는 다수의 단말과 하나의 기지국 사이에 이루어져
『 하기 때문에 하향링크와 달리 기지국이 상향링크 동기 정보를 추정하여 단말에 전송하
폐루프(010860-1002) 방식으로 수행된다. 최초로 Ao] 진입한 단말은 하향링크 동기화
WAYS 수행한 후 자신이 속한 셀의 기지국에 동기화를 이루고 이를 기반으로 기지국과

결을 시도한다. 이러한 상향링크 초기 동기화는 RA(Random Access) 과정에서 수행되
, 이외에도 기지국과의 재 연결 필요한 경우 또는 핸드오버가 필요한 경우에 RA 과
정이 수행된다. 하지만 상향링크       은 다수의 단말이 하나의 OFDMA 심볼에 동시에
ALS 전송하므로 OFDM 방식과 2 Zo ° 심볼 내 von" 직교성 유지를 위해서 다수
의 단말과 기지국간의 심볼 동기가 필요하고, FDDS| 경우에는 추가적으로 주파수 동기가
필요하다. 한 단말의 OFDMA 심볼이 다른 단말들과의 OFDMA 심볼들과 동기가 이루어
지지 않는 경우 그 단말의 심볼은 다른 단말들에게 MAI(Multiple Access Interference) =
작용하며 전체 시스템의 Bes 열화 시키는 주요 원인이 된다. OFDMA 시스템에 처음
접속하려는 각 단말은 상향링크 동기를 획득하지 않은 상태에서 초기 레인징 과정을 수행

제 묘 pe ofr 2

10

Oo}

한다. 그림 5.25는 상향링크 동기를 획득하지 않은 상태의 각 기지국에 신호를 전
송한 경우 기지국 수신기에 다수의 시간 동기가 이루어지지 않은 신호들이 수신되는 것을
보여준다.

그림 5.25에 나타난 바와 같이 각 단말이 OFDMA 형태로 부채널을 전송할 경우 각 단
말의 위치에 따라 기지국에 도달하는 시간이 다르게 된다. 이 경우 기지국 수신단에서 정
확한 시간 동기가 이루어지지 않기 때문에 부반송파간의 직교성이 파괴되어 신호를 복조

_ 246



===== PAGE 245 =====
제5장_동기화 기법

_ 000 symbol    [ES l—th symbol

그림 5.25 OFDMA 기지국에서 수신된 다수의 단말 신호

Copy samples                          Copy samples

|       OFDM symbol period     “|

그림 5.26 Random Access 용 심볼

그림 5.272 초기 레인징 과정에서 그림 5.260] 주어진 RAS ASS 단말에서 전송하
여 상향링크 시간 동기를 획득하는 HIS 보여준다. 그림 5.27에 나타난 바와 같이
OFDM 셀룰러 시스템에 진입하는 단말의 초기 레인징 과정은 다음과 같다.

(1) 전원을 켜거나 또는 핸드오버를 통해 시스템에 접속을 시도하는 단말은 먼저 하향
크 프리앰블을 통해 하향링크 동기를 획득한다. 그리고 하향링크 제어 채널을 통
향링크 전송 파라미터(#ㅅ용 심볼 부호 집합, 부채널 정보, 초기 레인징 시간 Hs 획
득한다. 여기서 《, 는 기지국과 단말 사이의 전파 지연 시간을 나타낸다.
(2) PHS 임의의 RA 심볼 부호를 선택하여 2개의 연속된 OFDMA 심볼 구간 동안에
RA 프리앰블을 반복하여 전송한다.
(3) 기지국은 수신된 각 단말의 RA 심볼을 검출하여 상향링크 ASS 위한 전력 정보,
timing advance 정보 등을 각 단말에게 전송한다. 그
ㅣ

림 5
ua
서 추정한 각 단말의 심볼 동기의 시점으로서, 각 단말에서 상향링크 전송을 위한

ot!



===== PAGE 246 =====
PART IT_ OFDMZ} MATLAB

HED
108)

UE         DL Preamble, t,             S  Slot Time
DL Preamble, 267                        26,    RA Pream    186
AGCH, Timing Sync.Command: —(2t,+4) | pdf          li
2t, +6            time
RA Body                                         RA Body
—6 a
향링크 시간 동기 획득 과정

그림 5.27 OFDM 셀룰러 시스템에서 상향링

timing advance 정보를 나타낸다. 또한 AGCH(Access Grant Channel)-& 통하여 기지
ALS 알려준다.

국에서 단말 프리앰블을 성공적으로 수신하였음을 알

(4) 단말은 하향링크 제어 채널을 통해 시간 동기 및 전력 제어 정보를 수신한 후, 할당된
상향 링크 대역을 사용하여 등록 AAS 수행한다.

앰블을 수신한 기지국은 랜덤 액세스를 시도한 단말의 신호 검출, 시간 동기,

oe 획득한다.

주파수 동기 등

248



===== PAGE 247 =====
0350 12 +

OFDM 시스템에서 송신단의 입력 비트는 PSKU QAM 신호로 변조된 후 IFFTS
쳐 시간영역 신호로 변환되어 무선 채널로 입력된다. 이 때 무선 채널의 영향으로 수신 신
호는 크기와 위상 왜곡이 발생하는데, 이러한 채널 영향을 추정하여 보상해야 송신
호를 복원할 수 있다[126]-[128]. 4장과 5장에서 설명한 바와 같이 OFDM 시스템에서는
직교성(000108000000이 만족되게 FFT 주기와 부반송파 간격이 설정되고, 심볼 타이밍 옵
셋과 반송파 주파수 옵셋이 보상되어 부채널간 간섭이 존재하지 않을 경우
파별로 독립적인 채널로 볼 수 있다. 즉, 각 부반송파 별로 수신된 신호는
sho] go 주어진다. 이 때 송신 ASS 검출하기 sale 각 HANIA 채널 특성을
추정해야 한다. OFDM 시스템에서의 채널 추정은 프리앰블이나 파일릿같이 송신단과 수

신단에서 모두 알고 있는 훈련 ATS 사용하여 수행될 수 있고, 훈련 신호 사이의 채널
보간 기법을 이용하여 추정한다. 또한 훈련 AS} 아닌 데이터 ASS 이용하여 채널을
추정할 수 있으며, 훈련 신호와 데이터 신호를 모두 이용하여 채널을 추정할 수도 있다.
이러한 추정 방법들은 송신단과 수신단 사이의 채널 상태와 채널 추정 성능, 채널 추정 방
법의 연산 복잡도 등을 고려하여 선택된다.

OFDM 시스템에서 채널 추정을 위해 사용되는 HUA 신호는 그 배치에 따라 블록
조, Comb 구조, 80006 구조로 나눌 수 있다1291-[1321.

249



===== PAGE 248 =====
PART I1_ OFDM2Z} MATLAB

 블록 구조

그림 6.1에 나타난 바와 같이 블록 구조는 OFDM 한 심볼에 대하여 전 주파수 대역에
걸쳐 TIA 신호가 존재하고, 시간영역에서 일정한 간격을 두고 BUR 신호가 배치되는
형태를 갖는다. 이 경우 시간 축에서 각 eel 신호 i 채널을 추정하기 위해서는 시
간영역에서 보간 기법이 수행되어야 한다. 블록 구조는 모든 부반송파에 신호가 존재하기
때문에 주파수 선택적(6\604600% selective) 특성이 높은 은 채널에 적합하고, 시간에 따라 빨
리 변하는 채널에는 적합하지 않다. 이 때 Nyquist 샘플링 이론에 의해 splat 신호간의
간격은 다음 AS 만족해야 한다.

8, 주                                            (6.1)

Doppler

여기서 “는 시간 축에서 WAS 신호간의 간격을 나타내고, Sooper 도플러 확산을

나타낸다.

1 OFDM Symbol                 St
|: 101010.101 101010101 101010101 10101010)
@ODDIOC@0OOO0@O0OO00@0000
@OdDIIO@®0OOO0@O0O000@0000
@ODIODO@®@OOO0@®0OO000@0000
>| GBSOOO@®@OOO0@0000@0000
2] @OD|IOO@0OOCO0 80000 @0000
= @OdD|IOO @O0OO00@0O000@0000O
©  ODIO 101010101 101010101 10101010)
쁘   CIO @OOO0@OCC0O0@0C00O0
lex Jelererel Terererel Jererere)
C@OOOC@OQOO0O0C@0000O
(0: 101010101 101010101 10101010)
<)@000000000000000
0@0ㅇ0ㅇㅁ0@0ㅇ0ㅁ0ㅁ000000

=
3
oO

그림 6.1 블록 구조의 Weed 배치

 Comb 구조
그림 6.20] 나타난 바와 같이 Comb 구조는 한 부반송파에 대하여 전 시간영역에 걸쳐
HAA 신호가 존재하고, 주파수영역으로는 일정한 간격을 두고 파일릿이 배치되는 형태
를 갖는다. 그리고 주파수 축에서 각 파일 신호 사이의 채널을 추정하기 위해서는 Fa

250



===== PAGE 249 =====
제6장_채널 추정 기법

tt

1 OFDM Symbol
OODOTOCOOOOCOOOO00O00O0

Frequency
0
@
0)
(
(
O
@
O
oO
O
0
1
O
ie)
O
O
O
O
O
O

@86@000000000900000000000@
Time
그림 6.2 Comb 구조의 DQ 배치

수영역에서 보간 기법이 수행되어야 한다. Comb 구조는 한 부반송파에 대하여 모든 시간
영역에서 신호가 존재하기 때문에 시간에 따라 빨리 변하는 Alo] 적합하고, 주파수 선
택적 특성이 높은 채널에 적합하지 않다. 이 때 Nyquist 샘플링 이론에 의해 mela 신호
간의 간격은 다음 식을 만족해야 한다.

(6.2)

여기서 5, 는 주파수축에서 MIS 신호간의 간격을 나타내고, poe = 채널의 최대 지
연 확산을 나타낸다.

 Lattice 구조
그림 63에 나타난 바와 같이 Lattice FAL 시간 축과 주파수 축에서 aelyl 신호가
일정한 간격을 두고 배치되는 형태를 갖는다. Lattice 구조에서 채널을 추정하기 위해서는
시간영역 보간과 주파수영역 보간을 모두 수행해야 한다. 이 때 Nyquist 샘플링 이론에 의
해 시간 축과 주파수 축에서 HSL 신호간의 간격은 다음 식을 만족해야 한다.
1      1

=. 97S
$5                                  (6.3)

Doppler                             max

lA

251


===== PAGE 250 =====
PART 1 _야미/과 MATLAB

5                          >|

1 OFDM Symbol |

OO  60@000000000@000ㅇ
OODO@OOOOQO0O000@00000
OOBOOOOOOO0O0O@OOO000O
@®ODQOOOCO0@OO0000000
OODOOOOO@OCOOO00000BO
OOAGOO@®OCOOOOOO00SO00O0
@<000000000000000
@0@0@00000000000000000
| Iolo |e (eleleleleley Jelelelelelelelese)
OOQOCOOO@OOOO00000 BO
OOQQVOOSQOOCOOOOOOOSOOO | gs
OOQUSOOQOO00O0OO0B0O0O00O0  "
OOSQVOOOOOOOO@OO0000O
@OQQOOOCO0@OO0000000

Time
그림 6.3 Lattice 구조의 Wed 배치

Frequency
O
Oo

여기서 와 $,는 시간 축과 주파수 축에서 vpolel 신호간의 WAS 나타내고,
06 는 도플러 BARS 나타내며, 는 채널의 최대 지연 확산을 나타낸다.

교
au
ne,
kK
posh
rir
a
i
=
> af
요
=
7
tulo
on
Ol
N
고
Ad

점이 있다. 훈련 신호 기반 채널 추정 기법으로는 19(Ｌ689[ Sas) 채널 er
MMSE(Minimum Mean Square Error) 채널 추정 기법 등이 있다[127]-[130][132][1331.

LS 채널 추정 기법

LS 채널 추정 기법은 수신단에서 사전에 알고 있는 훈련 ASS 이용하여 MIS 추정

하는 기법으로 채널 추정이 가장 간단하여 계산량이 낮은 장점이 있다. OFDM 시스템에
A 수신 ABS 식 (6.4)와 같이 나타낼 때, LS 채널 추정 기법에서의 비용 함수(0061
function) 식 (6.9)와 같이 주어진다.

292



===== PAGE 251 =====
제6장_채널 추정 기법

Y=HX+Z
y=[y[oL yf.lv 4]

매고 0],X [1].--.X LN 14]

Z=(2Z(0],Z[1].---.Z[N-1]              (6.4)
200] 0 ~ 0
은 | 0 401   :
:     ;  0
0 … 0 A[N-]]

J(H)= ll Y-HX |?
= (Y-HX)"(Y-HX)                           (6.5)
= y"y—y* ax—x"A4 y+ xX7a "Ax
여기서 HE 추정된 채널을 나타내고, XE 훈련 신호 벡터, VE 수신 신호 aes
나타낸다. 이 때 4} (6.5)의 비용 함수를 최소로 하는 AS 구하기 위해 비용 함수를 Hol
대하여 gradientS 취하면 다음과 같다.

=—(x#y) +(x#xH) = 0                           (6.6)

따라서 LS 채널 추정 기법으로 추정된 AMS 다음 식으로 주어진다.
트. = ¥                                         (6.7)

OFDM 시스템에서 각 부채널에 대해 수신 ASL 채널과 송신신호의 곱으로 표현이
되기 때문에 식 (6.7은 각 부채널에 대해 다음과 같이 주어진다.

(6.8)

LS 채널 추정 기법은 가장 간단하게 채널을 추정할 수 있다는 장점이 있지만, 채널이
nullo} 빠진 경우 잡음 증폭 효과가 있어 잡음 존재 시 채널 추정 오차가 증가한다는 단점

이 있다. 다음은 LS 채널 추정 기법의 MSE(mean square 6001)를 나타낸다.

253



===== PAGE 252 =====
PART IL_ OFDMZ} MATLAB

MSE,, = 이 ~fi,s) (H -ii,,)| = | (H -x"y)"(H- xy) |
(6.9)

여기서 OF} OFS 각각 잡음 신호와 훈련 신호의 분산을 나타낸다. 식 (6.9)에서 알
수 있듯이 LS 채널 추정 기법의 MSEE 신호대 4-2-4](Signal-to—Noise Ratio; 54448)에
반비례한다.

es
lor

 MMSE 채널 추정 기법
MMSE 채널 추정 기법은 그림 6.4에 나타난 바와 같이 채널 벡터와 입력 벡터의 MSE
를 최소화하는 기법으로, 이 때 채널 추정 벡터는 직교 이론(0001080081 theorem)& 이용
하여 구할 수 있다.

m=

Weight
그림 6.4 MMSE 채널 추정 기법

그림 6.4에서 MMSE 채널 추정을 위한 입력 벡터 HE 식 (6.4)를 사용하여 다음과 같
이 표현될 수 있다.

H =YX! =H+ZX"!                                           (6.10)
직교 이론에 의하면 최소의 MSES 갖은 경우 MMSE 필터의 오차와 입력 값의 곱은

0이 된다. 따라서 그림 6.4에 나타난 MMSE 채널 추정 기법의 가중치는 직교 이론에 의
해 다음과 같이 유도된다.

254


===== PAGE 253 =====
제6장_채널 추정 기법

EleH']=E[(H—H)H' | =E|(H— WH)H' |

=E[HA" ]- 00004.                     (6.11)
= Ryg— WR
=0

여기서 는 오차 WES 나타내고, HE 입력 벡터, HE 가중치가 곱해진 채널 추정
벡터를 나타낸다. 또한 WE 가중치 벡터, Regt 채널 추정 벡터의 자기 분산 행렬
(auto—covariance matrix) 나타낸다. 식 (6.11)에서 입력 벡터 HQ} 오차 의 곱이 00]
되는 가중지 WS 구하면 다음과 같다.

W = RyaRaq                                              (6.12)

여기서 채널 추정 벡터의 자기 분산 YAS 잡음이 포함된 채널 추정값의 자기 분산 행
렬로 다음과 같이 나타낼 수 있다.

Rgg= 8188]
= 비토 (호 ')"1]
= E((H + ZX"')(H+ ZX")"]
= E[HH” + ZX'H” +HX'Z+ZX'(X")"Z")]         (6.13)
= E[HH” ]+ E[ZX"'(xX"')" Z")]

2
0.
= E[HH"]+ =

x

련 신호의 BAS 나타내고, Ｌ는 크기가
Ak Rug 채널 벡터 WS 잡음이 =
8 (cross—covariance 108100※)을 나타낸다. 위
채널 추정 행렬은 다음과 같이 주어진다.

어

여기서 과 oF & 각각 잡음 신호와 훈
NXN 인 단위 행렬을 나타낸다. 또한 식 (
함된 채널 추정 벡터 표사이의 상호 분산
식으로부터 MMSE 채널 추정 기법에 의한

고 오즈

2
ES              02 vax
H= Rag Raq H= Ryg (Rant oD) ‘H           (6.14)

식 (6.14)로부터 원하는 채널 추정 BSS 얻게 되는데 이는 보간 행렬과 채널 추정 값
들의 곱으로 이루어진다. 여기서 보간 행렬은 수신 심볼과 무관하고, 파일릿의 위치와 파



===== PAGE 254 =====
PART I_OFDMZ} MATLAB

수, 추정하고자 하는 채널의 수에 의해 보간 행렬이 결정된다.

분산 행렬 Rg Zt Ruy 2) 원소는 서로 다른 시간과 주파수 간격에 위치한 부
이의 상관값을 나타낸다. 만약 256와 {이 각각 부반송파 인덱스와 OFDM 심볼 인덱스라
고 하면 상관값은 다음과 같이 주어진다.

티4.^/ |=피2, ]=-4100-/1                  (6.15)

여기서 [1 St or Lk] = 각각 시간과 주파수에 대한 상관 함수이다. 지수적으로 감소하
는 다중경로 PDP(Power Delay Profile)o] 대해 7,[4]는 다음과 같이 주어진다.

1

=
maT j2at,, kAf

(6.16)

FF T =   AL 7. 의 역수  이다. 최대 >  플러 주파수 fmax
와 14 스픽트림을 깃는 시간 ao |딩 신호에 대해 시간 상관 함수 LE 다음과 같이

TL = Jo (27 fosax! Tym )                                        (6.17)

2
건
=
fi
ch
을

OA} Bessel 함수이고, Tym OFDM 심볼 주기로 FFT 구간과 보
호 구간의 aan 주어진다. 그림 6.5= 대역폭이 10MHz°|32 OFDM 심볼 주기가
Hel salted 마른 시간 BFE 보여준다.

Age 훈련 SS 사용한 체널 추정 기법의 성능을 살펴본다. 모의실험을 위한 파라
미터는 다음과 같다. 모의실험 시 각 gpelel 사이의 채널 추정 값은 6.4.1절의 선형 보간
구

256



===== PAGE 255 =====
제6장_채널 추정 기법

it

Correlation Lacks in time, BW=10MHz, Ta 115.2us

= 를 =0. 542
—— fmax=1kHz
| | | = frnax=5KH2z

ti ire nt se gc Cec we ho a cn ce Ba to eta med

Symbol index
그림 6.5 채널의 시간 상관 특성 (BW=10MHZ, Toym = 115.2us)

표 6.1 모의실험 파라미터

Cyclic Prefix                    |           128

Pilot spacing                               8
Channel model                        ITU—Pedestrian A
Velocity                               3km/h
Modulation                     16QAM, 64QAM
Pilot pattern                            Comb Type

그림 6.62 LS 채널 추정 기법을 사용하여 채널 추정 후 추정된 채널로 채널 왜곡을 등
화 한 경우의 성상도를 나타내고, 그림 6.72 이 때의 MSE 성능을 나타낸다.

그림 6.6(a)9} (0]는 각각 16044! 변조방식과 64044 변조방식을 사용하였을 때 등화
전의 성상도이고, 그림 6.606)와 (0)는 추정된 AVS 이용하여 등화 한 이후의 성상도를
나타낸다. 그림 6.6(8)와 (0로부터 OFDM 시스템에서 채널 왜곡으로 인해 크기와 위상
성분에서 왜곡이 발생하는 것을 알 수 있으며 이를 보상하지 않을 경우 성능이 크게 저ㅎ
됨을 알 수 있다. 그림 6.606)와 (0)는 LS 채널 추정 기법을 사용하여 WAS 등화 할 경우
크기와 위상 왜곡이 상당히 보상됨을 알 수 있다. 하지만 채널 추정 오차와 잡음에 의해

ar
P -

ot

0

=

257



===== PAGE 256 =====
PART Il_ OFDM2} MATLAB

Constellation after equalization, 16QAM, SNR = 30dB, Ped A, 3km/h

Constellation before equalization, 16QAM. SNR = 3008, Ped A 3km/h
4

1.5                                       1
오오                                                                                  i
3         3                                                                                 i
@          per”      ele   e%e* @                    ~                               ie
Lh 시구 01. | | “0 8 6 >
oe        is                  =                                                |
|. Stag 앨리 | os                                       ;
ee eee PF!    F      지게 ad               *      Sy      »      @.
0       Chg .  이 sens,    ak 투  "       버거 Par al           0
(을                |      ;     :     Hf
.  bisa   os, OS
+     oe.  oe 두               로 |      &      »     wig
*       = <. a:     신오          0.5
2b      ght.   Nae "에                .
!        려 hy  oT. Se ar          ㆍ              ;        -        20        3“        『겨
-4                                                   1.5
4      E      2     4      0      1      2      3      445        1       0.5        0       0.5        1        1.5

(a) 등화 A(16QAM)

Constellation before equalization, 64QAM SNR = 30dB, Ped A 3km/h
4

(b) 등화 #(6QAM)

Constellation after equalization, 64QAM, SNR = 30dB, Ped A 3km/h

1.5          |              [
,           0.카---호 ~ 주 ~ 주
0                               0   *  4  *  레브  주 x.
|                               ee en,
2                    ~ 이 ae 이겨
3              ,  i | 다 이 아래
2   3   2   4   0   1   2   3   4 as    1    36    0    =    1    1.5
) 등화 A(64QAM)                     (0) 등화 #(64QAM)
그림 6.6 LS 채널 추정 기법을 사용한 채널 등화

왜곡이 남아있음을 알 수 있다. 그리고 그림 6.7로부터 MSE7} SNRO| 증가함에 따라 감
소하는 것을 알 수 있으며, 이는 식 (6.9)에서 확인할 수 있다.

그림 6.7은 표 6.1의 모의실험 파라미터를 사용한 경우에 Ｌ5와 MMSE 채널 추정 기법
의 MSE 성능을 나타낸다. MMSE 채널 추정 기법은 추정하고자 하는 채널의 상관 특성
을 미리 알고 있어야 하고 연산 복잡도가 Ｌ8 채널 추정 기법보다 높지만 채널 추정 성능
은 LS 기법에 비해 우수함을 알 수 있다.

258



===== PAGE 257 =====
다음 MATLAB 프로그램 6.1(“CE_main.m”)q4= 부프로그램 6.2(.9 (0ㅁ.0)와 부프로
그램 6.3(“MMSE_CE”)S 사용하여 LS 채널 추정 기법과 MMSE 채널 추정 기법을 실행시키
며, 파라미터 중 하나인 int opt 1 또는 2로 설정함에 따라 (6.4절에 나오는, 그리고 부 프로
그램 6.4(“interpolation”)= 구현된) 선형보간 기법이나 Cubic spline 보간 기법이 적용된다.
MMSE 채널 추정 기법의 함수에서 seal 신호는 매 심볼마다 삽입이 되기 때문에서 식
(6.16)의 주파수 상관 함수만 구하면 된다. 따라서 식 (6.17)의 시간 상관 함수는 1로 하고
MMSE 채널 추정을 위한 가중치를 계산한다.

6 CE main.m

% Channel Estimation with linear/spline interpolation

clear all; close all; clc;

Nfft = 1024; Np = 8; % FFT size and pilot spacing

Nep = Nfft/Np; Nofdm = Nfft+Ncp; % # of pilots and OFDM symbol size
Nsym =2; «© # of symbols

bps = 4; m_ord = 2*bps; % modulation order

v=3; fc=2e9; fd=fc*v*1000/3600/3e8; % velocity and Doppler frequency

259     |



===== PAGE 258 =====
PART Il_ 야미/과 MATLAB

fs=10e6; ts=1/fs; % sampling frequency and sampling period

init_t=0; SNR = 30; snr = 10*(SNR/10); % SNR[dB]

int_opt = 1; % 1/2: linear/spline interpolation

mod_obj = modem.qammod('M',m_ord, 'PhaseOffset',0,'SymbolOrder',
'binary', 'InputType', 'bit');

demod_obj=modem.qamdemod('M',m_ord, 'PhaseOffset',0,'SymbolOrder',...
‘binary', 'OutputType', 'bit', 'DecisionType','hard decision') ;

rand('seed',1); randn('seed',1);

mutipath_jakeschannel ('itu','PEDA',fs,fd,init_t);

for nsym=1:Nsym

pilot = 2*(randn(1,Ncp)>0)-1;   % pilot sequence generation
tx_bit = randint (m_ord* (Nfft-Necp) ,1) ;   % bit generation

Data_sym = modulate(mod_obj, tx_bit).';
Scale = modnorm(Data_sym, 'avpow!,1) ;

Data_sym = Data_sym*Scale; % normalization
li, = 0;   pilot_loe = [];

for k=1:Nfft
if mod(k,Np) ==
Tx_sym(1,k) = pilot (floor (k/Np)+1); pilot_loc = [pilot_loc k];
11 = ii+1;
else       Tx_sym(1,k) = Data_sym(k-ii) ;
end     ：
end
tx_sym = ifft (Tx_sym,Nfft) ;                  응 IFFT
tx_sym = [tx_sym(N£ft-Ncp+1:Nff£t) tx_sym] ;   % add CP
[rx_sym,cir]=mutipath_jakeschannel(tx_sym); % channel pass

ch_length = length(cir); % length of channel impulse response
sig_pow = mean(rx_sym.*conj(rx_sym) ) ;

noise=sqrt (sig _pow/2/snr) * (randn(1,Nofdm) +j*randn(1,Nofdm)); %Noise
rx_sym = rx_sym + noise;                      % add noise (AWGN)
Rx_sym = ff£t (rx_sym(1,Ncp+1:Nofdm) ) ;   6 remove CP and FFT

H_LS = LS _CE(Rx_sym,pilot,pilot_loc,Nfft,Np,int opt); % LS
H_MMSE = MMSE _CE(Rx_sym,pilot,pilot_loc,Nfft,Np,cir,ts,SNR); %MMSE
end

!를 프로그램 6.1 채널 추정 기법의 실행 프로그램

:

260



===== PAGE 259 =====
제6장_채널 추정 기법

function H_LS = LS CE(rx,pilot,pilot_loc,N,Np,int_opt)

% LS channel estimation function

6 Inputs:

%      rx        : received symbol

6      pilot      : pilot symbol

%      pilot_loc : pilot location

%      N         : FFT size

6      Np        : pilot spacing

%      int_opt   : ‘1¢/'2' for ‘linear'/’spline’ interpolation
% Output:

%      LS_out     : estimated channel

k=1:N/Np;

LS est (1,k)= rx(1,pilot_loc(k))./pilot(k); % 4 (6.7) & (6.8)
if int_opt==1, method = 'linear'; else method = 'spline'; end
H_LS = interpolation(LS est,pilot_loc,N,method) ; ¢ linear/spline

Tal

Tal 프로그램 6.2 Ls 채널 추정 함수

function H_MMSE = MMSE CE(rx,pilot,pilot_loc,N,Np,ch_tap,ts, SNR)

% MMSE channel estimation

6 Inputs:

%      rx        : received symbol

%      pilot      : pilot symbol

%      pilot_loc : pilot location

%      N         : FFT size

%      Np        : pilot spacing

%      ch_tap    : channel impulse response
%      ts        : sampling time

%      SNR       : Signal-to-noise ratio[dB]
6 Output:

%      H_ MMSE    : estimated channel

snr = 10*(SNR*0.1);

Ncp=N/Np; % number of pilots

k=1:Necp;

H tild = rx(1,pilot_loc(k))./pilot(k); % “4 (6.17)
k=1:length(ch_tap); k_ts = (k-1)*ts;

tmp = ch_tap.*conj(ch_tap).*k ts;

ch _tap2 = ch_tap*ch_tap';

261



===== PAGE 260 =====
PART 1 야미/과 MATLAB

r = sum(tmp) /ch_tap2;

r2 = tmp*k_ts.'/ch_tap2;

rms = sqrt (r2-r*2); % rms delay
df = 1/(ts*N) ;

j2pi_rms df = j*2*pi*rms*df;

Kl = repmat([0:N-1].',1,Ncp) ;

K2 = repmat ([0:Ncp-1],N,1);

rf = 1./(1+j2pi_rms_df*(K1-K2*Np)); % “4 (6.16)

K3 = repmat ([0:Ncp-1].',1,Ncp) ;

K4 = repmat ([0:Ncp-1] ,Ncp,1);

rf2 = 1./(1+j2pi_rms_df*Np* (K3-K4)); % “ (6.16)

Rhp = ri;

Rpp = rf2 + eye(length(H_tild),length(H_tild))/snr; % “4 (6.13)

H_MMSE = transpose (Rhp*inv(Rpp) *transpose(H tild)); % * (6.14)

tml 프로그램 6.3 MMSE 채널 추정 함수

function [eh_interp] = interpolation(eh,loc_p,Nfft,method)

6 Input:

%      eh      : estimated channel using pilot sequence
6      100 ㅁ : location of pilot sequence

6      NfEt   : FFT size

%      method : ‘linear’/’spline’

6 Output:

%      eh_interp : interpolated channel

if loc p(1)>1
600 = eh(1) - (eh(2) -eh(1))/(loc_p(2)-loc_p(1))*(loc_p(1)-1);
eh = [6580 eh]; loc_p = [1 loc 20] ;
end
if loc_p(end) <Nfft
slope = (eh(end) -eh(end-1) ) /(loc_p(end) -loc_p(end-1) ) ;
eh = [eh eh(end) +slope* (Nfft-loc_p(end))]; loc_p = [loc_p NEfft];
end

if method=='spline', eh_interp=interp1(loc_p,eh, [1:Nfft],'spline') ;

else     eh_interp = interp1(loc_p,eh, [1:Nfft]);
end
i 프로그램 6.4 보간 함수

262



===== PAGE 261 =====
제6장_채널 추정 기법

000 =2 4    | 혜

보간 기법은 BUS 이용하여 채널을 추정한 후에 추정된 채널 aS 사용하여 주파수
영역에서 BIR 톤 간의 채널 또는 시간영역에서 AA 심볼 간의 채널을 추정하기 위
해 수행된다. 보간 기법에는 선형 보간 기법과 2차 다항식(666000-07067 polynomial) 보
간 기법, cubic spline 보간 기법 등이 있다128]-[131][134].

bo

간 기법
YAS 이용하여 추정한 채넬 사이를 직선으로 연결하는 방법으로

6.4.1 선영

간 기법은 프

후

형
7

tr
ce bt

|             2
연결하기 때문

즈
의               기
있다. 그

al

ua 」어
오 (소
에

fe)
중 가장 낮은 계산량을 갖는다. 그리나 선형 보간 기법은 추정한 채널 사이를
때
림 6.

에 TFIBL 사이의 원래 채널이 곡선 형태를 갖는 경우 정확성이
8은 po}s 간의 간격이 4일 때의 선형 보간 기법을 나타낸다.

4 i

Ideal Channel

배가 시  | pt  Estimated Channel
{               |        ,       ]               |               |            (Linear interpolation)

k

그림 6.8 선형 보간 기법 (L=4)

ai

형 보간 기법을 식으로 나타내면 다음과 같다.

Hlk] = H[mL+1) = 2. + | (Hy 41 Hy) 1=0,1,<, £=1         (6.18)

여기서 #[시는 《번째 인덱스에서의 채널 추정값을 나타내고, H,,-2 m 번째 spa 위
치에서의 채널 FAS 나타낸다. 그리고 LS pole 간의 간격을 나타낸다.

263


===== PAGE 262 =====
PART Il1_ OFDMZ} MATLAB

Ry 2차 다항식 보간 기법

구는                                 Estimated Channel

N                                        (Second-order polynomial
는 4              ‘             interpolation)
> k
그림 6.9 2a} 다항식 보간 기법 (L=4)
2차 다항식 보간 기법을 식으로 나타내면 다음과 같다.
a(a-1)                             a(a+l)                  (6.19)

where C_, =        ,C, =-(a-Di@+)), C=    aa. =I L

여기서 Akl 《번째 인덱스에서의 채널 추정값을 나타내고, 2, = AlmL]& mw
Al abled 위치에서의 채널 추정값을 나타낸다. 그리고 LS 파일렀간의 간격을 나타낸다.

EI Cubic Spline 보간 기법

Cubic spline 보간 기법은 FIRS 이용하여 추정한 채널 사이를 여러 개의 소구간으
로 나누고, 각 소구간을 3차 다항식으로 근사화하여 연결하는 방법으로 선형 보간 기법이
나 2차 다항식 보간 기법보다 높은 계산량을 갖는다. 그림 6.10은 wpelal 간의 간격이 4일
때의 cubic spline 보간 기법을 나타낸다.

|

—

264



===== PAGE 263 =====
Estimated Channel
(Cubic spline interpolation)

                                      :        k
(m—1)L             mL               (m+1)L

그림 6.10 Cubic spline 보간 기법 (L=4)

Cubic spline 보간 기법에서 각 소구간 [mL,(m + IL] 에서 구하고자 SHE 채널 값은 다
음과 같이 3차 다항식으로 나타낼 수 있다.

20 =a,, (k—mL)3 +b,, (k—-mL)? +¢,, (k-mL) +d,,, mL < k < (m+1)Lm=1,-", M    (6.20)

여기서 #[시는 소구간에서의 추정된 채널값을 나타내고, H,, = #17141은 번째 파
la 위치에서의 채널 추정값을 나타낸다.

Cubic spline 보간 기법에서 각 소구간에서는 4개의 미지 상수가 존재한다. 따라서 47
개의 소구간에 대해서 414개의 다항식이 필요하다. 이 때 각 미지 상수 (dn, % Com de)
는 다음의 6000081% 00001407을 만족해야 한다.

* Boundary condition

1. #[시는 구간 0,44]에서 연속 함수이다.
2. 1차 도함수 #[/]은 구간 DML OA 연속 함수이다.
2 "[시은 구간 [.44/1에서 연속 함수이다.

각 미지상수는 경계 ZZA(boundary 00001000)에 의해 다음과 같이 구할 수 있다.

'        ;                          ie                   =%        (6.21

여기서 L 은 weal 간의 간격을 나타낸다. 그리고 y,, 은 "의 위치에서의 2차 도함수
"(eS 나타낸다. 식 (6.21)를 식 (6.20)에 대입하여 추정된 채널은 다음과 같이 나타낼

iz
수 있다.



===== PAGE 264 =====
PART ㅁ_ OFDM2Z} MATLAB

ALK] nf | eh Lm “1+ 거는 20 -마

L                          ^
(6.22)
it, (m+1)L—k + He =)
^             L
식 (6.22) 인접 채널과의 관계에 따라 다음과 같이 표현된다.
6  =     _   _
Yo +4%, + = rahe —2Hu +H)                      (6.23)
Al (6.23)을 행렬형태로 나타내면 다음과 같이 표현된다.
고 도    a    a    ：
141000001 %      Byek es
1 4 1 =              Ys           —2H3+H,4
014.      0 0|   "   A, -221+2:
Do:           a _      oo        (6.24)
0000-141 0%,      Hys-2H ys +H yr
0     0         014     Yu-2       Hua-2ives +;
Me                       J] 700      | Hu-2—-2Hwit Hu |
L Yu
Cubic spline 보간 기법은 추정된 채널을 보간하기 위해 3차 다항식을 사용하는데, 이
때 보간에 필요한 미지수의 개수(27)가 다항식의 개수(47- 2)보다 적다. 이 문제를 해결
하기 위해 4801181 spline} parabolic runout spline, cubic runout spline 5°] 이용된다.

Natural splineoJA = 양 끝점에서의 2차 도함수를 0으로 설정한다. 즉, 양 끝점에서 3
차 spline HS 직선으로 간주하는 것이다. A} (6.25)는 4801181 501106에서의 2차 도함수

를 나타낸다.
% =Vu =9                                       (6.25)
Parabolic runout spline? 양 끝점 2  “ 2차 도함수는 일정하다고 가정한다. 4)
(6.26)은 parabolic runout 501106의 2차 도함수를 나타낸다.

_ 266



===== PAGE 265 =====
0.9                       T
!                   —@— Ideal Channel
0.8 }5----B------차  ㅡ*- Estimated Channel
071             ~                                          |
마흔a                                   rae
0.5                                             |
0               5     Index     10              15
oa         Linear interpolation-imaginary, L = 5
0.2 f}---2--2--22-----하나그,
0                       t                      pee --------1
-0.24                             9-0" -*-  —¢— Ideal Channel
04                         H                   —@— Estimated Channel
“0                                                                               “0                     5                     10                    15

Linear interpolation, L = 5

제6장_채널 추정

Linear interpolation-real, L = 5

Index

(a) 선형 보간 기법

Second-order polynomial interpolation, L = 5

-0.5                                                                                               0         Second-order polynomial interpolation-real, L = 5
：                                {                       —@— Ideal Channel
0.811- 가_  ㅡ*-- Estimated Channel
O.7 eee eanen  ee ee
0.6}---         -
085               5     Index     10              15
aa   Second-order polynomial interpolation-imaginary, L=5
2 eee               |                「
0 제비뉘메싸새에세대세새네머즈체데자주저사=주=네재니저==ㄴ=====0=ㄴ=
-0.2-- 0 -- -ㅡ-@- Ideal Channel
Ha                         '                   = Estimated Channel
“0            5    index    10           15
(b) 22} 다항식 보간 기법
05      401 90006 1080000000 1 =     Cubic spline interpolation-real, L= 5
score! euemeeweece.            |                            !                    —@®— Ideal Channel
08posnceeenee--  —?*— Estimated Channel|
아아 a     07 cc
어겨        .              0.6}----         -극                          2
es oe ee                         :      ae
3                                                           056               5              10              15
[sill] leaeeimennenes: tenement |                     |   Index |
Sap    da     Cubic spline interpolation-imaginary, L = 5
FS)                                                            {                 -
매국                           0.2}-            ae        Sse       >
RD pooaean car orerenenbanannnmen gen ana et ammammmatnnn  =        O}------          배우      pang ---------1
주 Ideal 00006  |--------“-1---------#-----]         -0.2                                                  -—@— Ideal Channel
55   —?— Estimated Channel                                                                                              |—#— Estimated Channel
“0               5                              16 | (“045               5              10              15
Index                                                    Index
(c) Cubic spline 보간 기법
그림 6.11 보간 기법에 따른 채널 추정 성능 (L=5)
267



===== PAGE 266 =====
PART 1 _야미/과 MATLAB

70277                                    (6.26)

Cubic runout spline= 양 끝점 근방에서 2차 도함수를 다른 2차 도함수의 선형 연산으
로부터 구한다. 식 (6.27)은 cubic runout 501106의 2차 도함수를 나타낸다.

% = 2% — Vos Vn = 2201 792                            (6.27)

그림 6.11은 ee 간격이 5일 때, 선형 보간 기법과 27} 다항식 보간 기법, cubic
spline 보간 기법에 의한 보간 성능을 나타낸다. 이 때 apelst 위치에서 추정된 채널 값은
HAPS 표현되기 때문에 이를 실수부와 허수부로 나누어 표현하였다.

ONY vecision-directed 채널 추정 기법

DD(Decision—Directed) 채널 추정 기법은 초기 프리앰블 또는 hee  신호를 이용하여
초기 채널 값을 추정한 후, 검출된 데이터 신호를 이용하여 채널의        A\(tracking)

하는 기법이다[135]-[137]. 그림 6.12는 DD AY 추정 기법을 나타낸

re wl
ae
+

.  ue  조시   조시.
—> Femme sip | os | ret |: [ESAT : “/pemod| : | 65 [>

그림 6.12 DD 채널 주정 기법

DD 채널 추정 기법은 크게 두 단계로 구성된다. 첫 번째 단계는 이전 심볼에서 추정된
채널을 이용하여 데이터 심볼을 추정하는 과정이고, 두 번째 단계는 추정된 데이터 심볼
을 이용하여 현재 심볼에서의 채널을 추정하는 과정이다. DD 채널 추정 기법을 식으로
나타내면 다음과 같다.

268



===== PAGE 267 =====
제6장_채널 추정 기법

=      끄시]
Step1: Xi [k]=—
Teel                    (6.28)
Step 2: Ai[k]=—o=+
tep   Hi{k]  YK

여기서 [서는 (번째 심볼에서의 수신 신호를 나타내고, A, [AE -1번째 심볼에
서 추정된 채널을 나타낸다. 그리고 Kk 2, _,[시를 이용하여 [번째 심볼에서 등화
된 신호를 나타낸다. 이 ASS 경판정하여 두 번째 단계에서 최종 채널값 4, _,[시을 추
정하는데 이용한다. 이 때 kt 부반송파 인덱스를 나타낸다. DD 채널 추정 기법은 식
(6.28)과 같이 검출된 ASS 이용하여 채널 갱신이 이루어지기 때문에 검출된 신호에 오
류가 있는 경우 에러 WA error propagation) 효과로 채널 추정 성능이 감소할 수 있다. 또
한 연속한 두 심볼 주기 동안의 채널 변화가 클 때에는 채널 추정 성능이 감소할 수 있다.
이러한 에러 전달 문제를 해결하기 위해 갱신되는 같에 가중치를 적용하는 방법, 인접 부
a

채널간 평균화된 채널 4 A(average channel estimation) 기법을 이용하는 방법 등이 있다.

| 6.6 Smee led ae

DEFT 기반 채널 추정 기법은 6.2절에서 설명한 LS 채널 추정 기법이나 MMSE 채널 추
정 기법 등을 사용하여 일차적으로 BIS 추정한 후에 추정된 채널을 DETS 사용하여
시간영역으로 변환하고 시간영역의 채널 임펄스 응답에서 최대 지연시간 이후의 신호를
제거하여 채널 추정의 VSS 향상시키는 방법이다[138]-[141]. DET 기반 채널 추정 기
법에서 DET 실제 FFTS 사용하여 효율적으로 구현할 수 있다. 그림 6.13은 일차적 채
J 추정으로 Ｌ8 채널 추정 기법을 사용하였을 경우 DET 기반 채널 추정 기법의 개요를
보여준다.

그림 6.13에서 나타낸 바와 같이 LS 채널 추정 기법을 이용하여 일차적으로 추정된 주
파수영역 채널 Ak]: IDFTS 거쳐 시간영역 채널 임펄스 응답으로 변환된다.

[7] = IDFT| alk} =h[n]+2[n], n=0,1,....N-1                           (6.29)



===== PAGE 268 =====
PART Ｌ_야04과 MATLAB

Frequency domain

Frequency domain    ail        Time domain           LL
4000             h [0]      h perl]                 Hpprl0\
tak                                  고                         #……
A(t]                                                     22141
_——
4000                                                 22212]
>             .          .                      —
18         :       ae     h[Z-1] hprrlZ— 비리  ee
Channel        *        =                              fal          :
Estimation                          0- ~                  버
4011                 0                     Hppr(N- 1] »
Yl                                                           -

그림 6.13 마ㄱ 기반 채널 추정 기법

여기서 IDFT{ ㆍ}는 IDET 연산을 나타내는 함수이다. 식 (6.29)의 시간영역 채널 임펄
부와 그 외 나머지 부

ASHE 채널 임펄스 응답의 최대 지연시간 LA) 존재하는 채널부
분으로 구성된 잡음부로 구분할 수 있다.
jn) = a +z[n] ,O0<n = -1                                    630)
z[n]        , otherwise

식 (6.30)에서 잡음부는 잡음 이외에 새로운 정보가 없으므로 이를 제거해서 채널 추정
향상시킬 수 있다. 잡음이 제거된 WAS 다음과 같이 나타낼 수 있다.

AKO
Joe 4%

;   in]   A[n]+z[n] ,0<n<L-1                  nit
77| =                                                                               2
ue                 0           , otherwise                                      ee)

음과 같이 주어

식 (6.31)의 채널 임펄스 응답은 DTS 거쳐 주파수영역으로 변환된 후 등화기 계수를
구하는데 사용된다. 이 때 DFTS 거친 주파수영역에서의 채널 응답은 다

진다.
(6.32)

A ver[k\= DFT {horr (n)}
DFT 기반 채널 추정 기법을 적용하기 위해서는 일차적인 채널 추정이 이루어져야 하

며, 채널 임펄스 응답의 최대 지연시간을 알고 있어야 한다.

270
SN



===== PAGE 269 =====
제6장_채널 추정 기법

표 6.2 모의실험 파라미터

Cyclic Prefix                  |           128
Pilot spacing                                 8
Channel model                         ITU—Pedestrian A
Velocity                                 3km/h
Modulation                               16QAM
Pilot pattern                            Comb Type

LS and OFT—based Channel Estimation

그림 6.14 LS 채널 추정 기법과 DFT 기반 채널 추정 기법의 MSE

Wd 추정 기법과 DET 기반 채널 추정

하여 Ach. WO] REL 과라미터는 표 624] 주어져 있다. 그림 6.14에 나타난

바와 같이 LS 채널 추정 기범만 적용하였을 경우와 비교하여 DET 기반 채널 추정 기법
을 사용하였을 경우 MSE 성능 향상이 크게 이루어짐을 알 수 있다.

본 절에서는 DFT 기반 채널 추정 기법에 대해 MATLAB 프로그램을 사용하여 4

24
다음 프로그램 6.5 DFT 기반 채널 추정 기법의 함수이며, 채널 추정 실행 프로그램?
그램 6.1의

271



===== PAGE 270 =====
PART Ｌ_ OFDM2} MATLAB

H_LS = LS _CE(Rx_sym,pilot,pilot_loc,Nfft,Np,int_opt) ;

H_DFT = DFT_CE(Rx_sym,pilot,pilot_loc_,Nfft,Np,ch_length,int_opt) ;

와 같은 문장을 삼입ㅎ                  수 있다

=

ue

function H_DFT = DFT _CE(rx,pilot,pilot_loc,N,Np,ch_len,int_opt)
DFT-based channel estimation

6 Inputs:

%      rx        : received symbol

%      pilot     : pilot symbol

%      pilot_loc : pilot location

%      N         : FFT size

%      Np       : pilot spacing

%      ch_len   : lenght of the channel impulse response

%      int_opt : ‘1’/'2' for ‘linear'/’spline’ interpolation
6 Output:

DFT out : estimated channel

H_LS = LS CE(rx,pilot,pilot_loc,N,Np,int_opt) ;

DFT time = ifft(H_LS); % 4 (6.29)

H_DFT = fft (DFT time(1:ch len),N); % “% (6.31) & (6.32)

IX

pol

fm! 프로그램 6.5 DFT 기반 채널 추정

ORT superimposed AIDS 이용한 채널 주정 기법

Superimposed 신호를 이용한 채널 추정 기법은 데이터 신호에 sale 신호를 추가하여
전송함으로써 Be 전송에 따른 전송 효율의 감소 없이 채널을 추정할 수 있는 기법이
다[142][143]. 그림 6.15 superimposed 신호의 구성을 보여준다. 전체 송신전력이 1일

때, HAs Also] 0(<1)의 전력을 할당하고 데이터 신호에 1- po] ABS 할당하여
신호를 구성한다.

bie



===== PAGE 271 =====
제6장_채널 추정 기법

그림 6.15 Superimposed 신호

OFDM 시스템에서 / 번째 심볼의 《번째 부반송파에 전송되는 송신신호 ㅅ,[ㅅ]는 데이

개
신호 S[k] 9} w]e 신호 P[K]O| 합으로 표현된다. 이 때 / 번째 심볼의 《번째 부
반송파에서 수신된 심볼은 다음 식으로 주어진다.

¥,[k] = A,[k]X,[k] + Z,[k] = H,[k](S,[k] + BLA]) + 44]                    (6.33)

여기서 YA] 2+ Z[k]= 각각 /
호를 나타낸다. 또한 AA 는 /번
Superimposed 신호를 이용한 채널
을 고려하여 채널이 거의 변하지 않
그 이 44구간 동안 잡음과 데이

번째 부반송파에 수신된 심볼과 잡음 Al
번째 부반송파에서의 채널 값을 나타낸다.

은       coherence 시간 = coherence 대역폭
는 연속된 44 구간을 시간 축이나 주파수 축에서 설정하
호 S,[k] 7} i.i.d(independent, identically distributed)
DET sess alas 파일 신호 [4]가 47
간 동안 동일하다고 가정하면, ME 동안의 채널과 wea ASE 시간영역 또는 주

그

시간영역
000 tem alk] = 1
6.34
주과수영역                     aes
A [k\)= A [k+l] =---=H,[k+M-l=H
P[k])=P[k+l=---=P[k+M-1]=P
연속되는 MSE 동안 수신 신호의 BAS 구하면 다음과 같이 주어진다.

273



===== PAGE 272 =====
PART 1 _ OFDMZ} MATLAB

시간영역
EQ =o YEA =T¥ (Hick al 14 Z oak)
“Vd (H  (Syn Lk]+ Ponl]) + 29)
eal                                            (6.35)
주과수영역
E(u} = 2 ik +m] =+ (Hl + mx, [e+ m+ Zl +m)
~그20 (S,[k +m] + P[k + m]) + Z,[k + m])
~ HP
따라서 채널 추정값은 다음 식을 사용하여 구할 수 있다.
#※= 따지                                        (6.36)
P

Superimposed 신호를 이용한 내 추정 기법은 별도의 splsl ASS 사용하지 않아
전송효율이 증가하지만 Bas ASS 전송하기 위해 추가적인 전력이 필요하며 데이터

호의 평균을 0으로 만들기 위해 많은 신호의 Bato] 필요하다는 단점이 있다. 또한 시
간영역에서 superimposed 신호를 pleat 채널 mal 할 경우 단말의 이동 속도가 증가

=

성능이 열화될 수 있다. eae   eto] 때" 신호를 사용하여 채널 추정을 할
경우 채널의 주파수 선택적 특성이 증가하게 되면 000606006 대역폭이 감소하여 채널 추
저
ㅇ

성능이 열화될 수 있다.

(QO sling 채널 추정 기법

Blind 채널 추정 기법은 채널 추
수신된 신호를 이용하여 채널을 추

AS 위하여 프리앰블이나 weelsl ABS 사용하지 않고
정하기 때문에 채널 추정을 위한 추가적인 오버헤드가 필

_ 274



===== PAGE 273 =====
제6장_채널 추정 기법

요 없다. Blind 채널 추정 기법은 일반적으로 수신 신호와 AGO] 통계적 BAS 이용하며,
단일 반송파 전송방식에서 널리 사용되는 8100 채널 추정 기법으로 84658808 로즈 등
이 있다[144]-[147]. OFDM 시스템에서의 Blind 채널 추정 기법으로 부공간 기반 채널 추

정 기법, eigenvalue decomposition 기법 등이 있다[146][148]-[1501.

ral
계수를 구하고 수신된 4    호를 ‘gable  통과하여 ASS 복원하는 방식을 사용하나,
Blind 채널 추정 기법인 지따 알고리즘은 신호의 통계적 BAS 이용하여 채널 보상
을 위한 Ass 갱신하여 채널 왜곡을 보상한다. 그림 6.16에 나타난 바와 i Bussgang
알고리즘은 일반적으로 LMS(Least Mean Square) 기반의 적응 알고리즘을 사용하여 채
널

Received signal                   iA

yln]           Transversal filter           uln]               Zero-memory            이히
{w,{n]}                              neni i aan
i                                            38

|        (5)

e[n]                pe

위 그림에 나타난 바와 같이 Bussgang 알고리즘은 필터와 비선형 추정기, 최적 적응 알
고리즘으로 구성된다. Bussgang 알고리즘을 적용하기 위해서는 비선형 추정기의 계수를
정해야 하는데, 이 계수를 구하는 방식에 따라 Sato 알고리즘, CMA(Constant Modulus
Algorithm), Godard 알고리즘으로 구분할 수 있다. 표 6.3은 Bussgang 알고리즘에서 사용
되는 비선형 추정기를 보여준다.

단일 반송파 전송방식에서 blind 채널 추정 기법으로 널리 사용되는 80858808 알고리
적용하기 위해서는 이에 적합한 비선형 추정기를 구해야 한다. 그
hy} OFDM 시스템에서 수신 신호는 Gaussian WA 변수이기 때문에 이러한 통계적 특
성을 갖는 Also] 적합한 비선형 추정기를 구하기 쉽지 않아 Bussgang 알고리즘을

OFDM 시스템에 적용하기 어렵다.



===== PAGE 274 =====
PART Ｌ_야미/과 MATLAB

표 6.3 Bussgang 알고리즘의 비선형 추정기

_ [etn]
Sato                                        asgn(u[n])                                          a= Eh]
               E| [ot |
CMA               ufn](1+ R, — lel )          i
E| |x{n]] :
u[n]                              pol              2p-1                           본 [000 |
odar            R     =          R =—    =
Godard      ag  (u{n]|” —|uln]|   )       pa

vinl=»[ r+), i=0,1,....0-1                (6.37)

여기서 yo 수신 ASS 나타내고, TE 송신 ASO 주기, JE 오버샘플링을 통해 생
성된 가상 채널(00481 channel 또는 94001180061)의 수를 나타낸다. 수신된 신호를 오버
샘플링을 함으로써 7 개의 가상 채널이 생성되는데 이는 동일한 송신 신호에 대하여 방정
식의                                                        링 수가

수가 더욱 증가함을 나타낸다. 그림 6.17은 채널의 탭 수 Mo} 3, 오버 샘플
송 신호가 (+1, -1}인 경우의 예를 나타낸다.

때 a

276

으 000 00 0


===== PAGE 275 =====
12  111

X[n—-{1] =-1             X[n+1]/=-1

y[n—2]       yln—1]        yln]        yln +1]       yln +2]       yln+3]

그림 6.17 오배샘플링된 채널의 BS 수신 신호의 예 4 = 3, | = 4, x = (H1,-1}

Ou

ce
=
bo
=z
re
비이
ot,
ria,
4
쓰
(쓰

fu

벡터 표현으로 다시 쓰면 다음과 같다.

y [n] = H'x[n]+z'[n]                                                      (6.38)

여기서 ”[씨와 201 은 각각 번째 샘플의 번째 오버샘플링된 수신 신

나타내고, 지씨 는 7 번째 샘플에서의 송신 SS 나타낸다. 또한, HE
링된 채널을 나타낸다. 식 (6.38)의 각 성분들은 다음과 같이 나타낼 수 있다.

[0]=| 7 00."07-1..2..2"00-^+14] ; 41
200=|200.207-1...200-2+1] ; 41
x(n] =[x{n],x[n -1],....x[n -M—-N +1] ; (+N)x1

hy how hy, 0 + 0           (6.39)
w=| % 7 10 Mo. |p Nx(M +N)
hi =[ AW ky | ; (M+1x1

여기서 은 데이터 샘플의 수를 나타낸다. 4] (6.38)을 벡터 식으로 표현하면 다음과
같다.

277



===== PAGE 276 =====
PART Ｌ_야미/과 MATLAB

y[”] = Hx[n] + 217]
y,=[y[ahy'[nh..y“Unl] 5 200

2 =(2'[A2' Un), '[nl} :  INx1                weal
배구  :  H',....H!"] : INx(M+N)
A} (6.40)에 주어진 수신 신호의 자기 상관 BAS 다음과 같다.
R=E| ylnly"[n] |
= E| (Hx{n] + 2{n])(Hx[n]+ 2001)" |                                   ath

= E| Hx[n]x"[nJH” |+2[2tnz"[n] |
=HR,H" +R,

위 자기상관 행렬을 고유 분해하여 고유치를 구하고, 고유치를 2 gee 정렬하여 나
열하면 다음과 같이 나타낼 수 있다.

Ay 2A, 2 2Ay
A,>o°, t=0,1,..,.M+N-1                            (6.42)
A, =0", t=0,l,...,IN-M-N-1

s,=4q,    ,t=0,1,..,M+N-1
©, =Qyane > £=9,1,...IN-M-N-1

(6.43)

여기서 5, 는 INX1 9] 크기를 갖는 신호 부공간 벡터를 나타내고 g,=[g?.2.8/ ' |

는 INx19] 크기를 갖는 잡음 부공간 벡터를 나타낸다. 신호 부공간 벡터와 잡음 부

벡터의 곱이 0이 되는 직교 성질(000080081 property)oj) 의해 비용 함수를 구하면 다음과
같다.



===== PAGE 277 =====
ae G 는 잡음 부공간으로 구성된 행렬을 나타내고, he 채널 벡터를 나타낸다.
스
T

G, =[G°,G,..,G7], +=0,1..,.IN-M-N-1

e100) 20] … 8614   | 0          0
Gi-| °  elo] = giv~2] 81454 «   0
‘    :     :   =,     :       :    «,    |              (6.45)
0    0 + — gi[0]    ef] -~ g[N-]]
g, € g,[7]
h=[h’,h',..ho TY 37M +1)x1
Al (6.44)의 비용 함수를 만족하는 ABS 다음과 같이 나타낼 수 있다.
h =argminJ (4) =argminh”Gh                                      (6.46)
h          h
Blind 채널 추정 기법은 추가적인 프리앰블 또는 Neo 신호를 사용하지 않아 채널 =
AS 위한 추가적인 오버헤드가 필요하지 않지만, 신호의 상관 등 2차 특성을 이용하기
위해 일반적으로 많은 수의 수신 신호가 필요하다. [토란 추정 Vek 훈련 기반 채널 추

정 기법에 비해 일반적으로 열화되는 경향이 있다.

OBS expectation Maximization 채널 추정 기법

EM 알고리즘은 확률적으로 ML(Maximum Likelihood) ae Searle

방법으로 Se] 분아에 응용이 되고 없다, AoA
정하는 방법에 대하여 설명한다[151]-[156]. EM 알고리즘은 1977년에 제안된 알고리
으로 MAP(Maximum A Posteriori) 확률을 계산하여 사라진 신호(071991408 value)2] 최우
추정(078×1014101 log-likelihood)& 하는 방법이다. EM 알고리즘은 반복과정을 거듭할수록

+
a

279



===== PAGE 278 =====
PART I OFDM#} MATLAB

확률적인 ML 같에 근접하는 장점이 있지만 복잡도가 크고 지역적 최대값에 수렴할 수 있
단점이 있다. ele 과정에서는 계산의 편의를 위해 log-likelihood 함수를 사용한
. 844 알고리즘을           AUS 추정하는 방법은 크게 시간영역 임펄스 sae 추정
하는 방법, 주과수영역 채널 응담을 추정하는 Well 있다 EM 알고리즘은 8-스팀과 Me
Sg 으로 구성이 된다. E-Ae2 ‘expectation’ 의미하고, M—24}-2 ‘maximization’
의미한다. 8-스템에서는 잠재 변수(16601 variable)2] 기대치를 계산하고, 44-스템에서는
주어진 데이터와 『-스템에서 구한 기대치가 부여된 잠재 변수를 이용하여 파라미터를 최
우 추정한다. EM 알고리즘에서는 일정기간 동안 AYO] 변하지 않음을 가정하고, E-AW
과 \4-스템의 반복 과정을 거듬할수록 sea ML 같에 수렴하게 된다.

Al (6.47)과 같이 수신 신호를 3  = 때, 27 와 가 SAS 때 의 확률밀도함수
(probability density 1040001070)는 Gaussian HES 갖는다.

oe

mw  s

8

Y[k]= A[K]X[k]+Z[k], 0<k<SN-1                   (6.47)

식 (6.48)은 HO} X 7} 주어졌을 WYO} 확률밀도함수를 나타낸다.

1     1     2
Y|H,X)=      =   2 - 24            ‘
f(YIHX)=T exp| 3231   [|        (6.48)

(&
f(Y|H)= > ~—        ree? = |Y — HX, f , C: constellation size         (6.49)

여기서 수신된 DHS] 신호 동안 채널이 변하지 SSS 가정하고, 수신 신호와 송신 신

호를 다음과 같이 각각 벡터 형태로 나타낼 수 있다.

Y= [Pal |                                      (6.50)

X=[X',....X? |                           (6.51)

280

  . ;,


===== PAGE 279 =====
EM 알고리즘에서는 를 “incomplete” 034라고 부르는데       =
변수 X 가 숨어있기 때문이다. 그리고 관측변수와 잠재변수를 같이 묶어 (Y,X)# 표시
하고 “complete” 031라고 부른다. tome data SHE ZS 추정하는 AL 어렵기
때문에 가능한 송신 신호의 조합과 수신 신호의 확률 ZS 추정할 수 있는 “complete”
data 형태의 확률분포로 변경하여 확률 값을 498 수 있다. Hee
확률밀도함수를 나타낸다.

“incomplete” data]

D
f(¥|H,X)=[]s(¥4 14,7)           |             (6.52)
d=1

식 (6.52) 연산의 간략화를 위해 log-likelihood 함수를 이용하여 덧셈으로 나타낼 수
있다.

D
log f(Y|H,X)= log f(¥" | H,X“)                         (6.53)
d=1
그리고 “complete” data2) 3-84 4-== log-likelihood 함수를 이용하여 다음과 2

이 나타낼 수 있다.

D

log f(Y,X|H)  0 |x")                  (6.54)

d=|

식 (6.54) 이용하여 WAS 추정하는데, 추정과정은 EAGT} M-AROw 나누어
나타별 수 있다. 8-스템에 의한 과정을 식으로 나타내면 chest 같다.

O(H|H®)=E,{/(¥,X|H)|Y,2@}

21201 f(y! x) 에   (6.55)

ral dal                               f(y" |H”)

E-A82 OC) 함수로 표현되는데, 이는 “complete” data2] log-likelihood 확률밀도
함수인 Al (6.54)을 DH 신호 동안 BRS 구하는 과정이다. 여기서 0(*) 함수의 We
HOA 채널 응답과 오차가 있는 경우 잡음 성분과 채널 추정 오차성분의 Go] 확률 기

281



===== PAGE 280 =====
PART ㅁㅁ OFDM2} MATLAB

대값으로 표현되기 때문에 적은 값을 갖고, A 가 AY 응답과 동일한 경우에 잡음 성
만 남게 되어 최대값을 갖는다.
1-스팁은 식 (6.59)에서 정의한 함수를 AHS 하기 위한 과정으로 A (6.59/의 OC)
함수를 편미분하여 구하게 된다. 그리고 이는 반복계산을 통해 채널이 갱신되는 형태로
표현된다. 따라서 번째 반복에서 구한 채널 AMS 이용하여 /+1번째 반복에서의 채널
HOS 구할 수 있다. 이를 식으로 나타내면 다음과 같다.

Ac

He = argmax O(H | H?)

aS (k" |X,      cD    FL |e,       (6.56)
{sSjxp Ll         dy  obs        |         ]

fal, dai      f(¥4|H”)     i=l al  Ar lz™)

식 (6.56)에서 f(¥"|H,X,) 와 f(Y"|H) = 식 (6.48)과 식 (6.49)를 통해 계산
있다. 식 (6.56)과 같이 EM 채널 추정 기법에서 확률적인 ML 채널 추정은 송신 가
CH 조합의 송신 신호에 대한 확률분포 BS 누적하여 이루어진다. 그러므로 EM
복잡도가 큰 방법이다. EM 알고리즘은 A} (6.55)와 같이 수신된 신호에
합과 채널 값의 곱을 빼주면 잡음 성분만 남게 되고 BSS Gaussian 분
성질을 이용하여 Gaussian 분포에 ae  기대값을 가중치로 사용하여
에 반영한다. 송신되었다고 가정된 신호 조합이 실제 ASS] 신호열일 경우 잡
남게 되어 큰 가중치가 주어진다. 반면에 송신되었다고 가정된 신호조합이 전송
가능성이 적은 신호열일 경우에는 잡음성분과 송신 신호 오차에 따른 성분이 존재
하여 수신 신호와의 거리가 멀어지므로 적은 가중치가 주어진다. EM 채널 추정 기법은
셀간 경계에서의 채널 추정이나 MIMO 시스템에서의 채널 추정과 같이 입력 신호의 정보
가 적게 주어진 상황에서 유용하게 사용될 수 있다.

최근에 EM 채널 추정 기법의 성능을 향상시키거나 계산량을 감소하기 위한 많은 연구
가 이루어지고 있다. DEM 채널 추정 기법은 그 중 하나로써, DD(Decision—Directed) 채
널 추정 기법과 EM 채널 추정 기법의 장점을 결합한 기법이다[153]. DEM 채널 추정 기
은 semi-blind 채널 추정 기법으로 프리앰블 또는 wy 신호를 이용하여 초기 채널
정이 이루어졌음을 가정하고, 초기 추정된 채널 응답과 데이터 신호를 이용하여 채널
3 성능을 향상시키는 채널 추정 기법이다. 기존 EM 기법과 비교하여 DEM 기법은 검
된 신호만을 이용하기 때문에 복잡도가 크게 감소하는 장점이 있다. 그리고 기존 DD

ol
+>

ee
au
ON

cm
oli
IN lo

와 uf   i

A
70°
포
시

신

ras
때
너

oer Pee
rin

10

cir

x2 ot
no Ar
=A

|



===== PAGE 281 =====
제6장_채널 추정 기법

채널 추정 기법의 신호 검출 오류에 따른 오류전달 효과로 채널 추정 성능이 열화될 수
있지만 DEM 채널 추정 기법은 검출된 AS 신뢰도를 이용한 가중치를 사용하여 오류
전달 효과에 의한 성능 열화를 감소시킬 수 있다. 또한 선택적으로 검출된 신호의 신뢰도
를 높이기 위해 채널코딩 복조/변조 블록을 결합할 au 있으며, 잡음 감소 블록을 통과하여
추정된 채널 응답의 정확도를 on 수 있다. MIMO  ‘eels EM 기법 적용 시 하
나의 수신안테나를 이용하여 다중 송신안테나의  Ae 응답을 추정해야 하는 모호성을 검
출된 신호를 이용하는 방법으로 해결하여 추정 성능을 향상   시킬수 수 있다.

OED 24 이동 시 채널 추정 기법

일반적으로 채널 추정은 한 OFDM 심볼 구간 동안 채널의 특성이 변하지 않는다는 가

정하에서 이루어진다. 그러나 고속으로 이동하는 단말의 경우에는 한 OFDM 심볼 구간
내에서 채널이 변할 수 있으며, 특히 OFDM 심볼 길이가 긴 경우에는 그 영향이 크게 나
타난다. 이러한 고속 이동 시 채널 변화는 OFDM 부채널 간의 직교성을 파괴하여 인접
부채널에 영향을 미치는 101(01016-(2180001 Interference)S 발생시킨다. 이 경우에는 수
단에서 단일탭 등화기로 채널을 보상하기 어렵기 때문에 시스템의 성능을 크게 저하시
수 있다. 따라서 고속으로 이동하는 OFDM 이동통신 시스템에서는 채널의 시변 영향
려하여 채널 추정 및 보상이 이루어져야 한다. 본 절에서는 시변 채널에서 발생하는
101의 영향에 대해 살펴본다[157]-[162].

OFDM 시스템에서 송신 심볼은 다음과 같이 정의된다.

   mW (^

KI

N-1
x{n]= > X[k]e?""", N=0,1,---,N-1                           (6.57)

k=0

선 채널이 』개의 독립적인 경로를 갖는다고 가정할 경우 수신신호는 다음과 같이 표

『

[웨
rt
a

vin] = > Ababa -61+버끼
= hylan, ]+ ns 4] +--+ [01400 2, 1+ wh

(6.58)

283


===== PAGE 282 =====
PART Il_OFDMZ} MATLAB

여기서 hints 채널의 임펄스 응답으로서 1 번째 경로의 채널 변화를 나타낸다. 또한,
7 1 번째 경로의 지연시간을 나타내며, 11] 은 AWGNS 나타낸다. 주파수영역에서의
BRAS Yk] 수신신호 10]을 007하여 다음과 같이 주어진다.

11 =   tile pas

mf mh                                                         (6.59)
> X[ mA [k - me?" + Wk], k=0,1,-+-,N-1
i=0

m=0 i

여기서 H[k-m] 2 시변 다중경로 채널 Alnlo] 대한 주파수영역 표현이고, WIL
w{n] 2] 주파수영역 표현으로 다음과 같이 주어진다.

1
H[k —m]= =< alnje mem”
N n=0

1 x2!                                 (6.60)
Wik]=—> wre?"
N n=0
Al (6.59)를 행렬 형태로 표현하면 다음과 같다.
Y=HX+W                             (6.61)
여기서 Y,X,W,H = 다음과 같이 정의된다.
Y =[¥(0], Y(U.--.YIN-H]’
X =[X[0], X[I.--. XIN -U]
W =[W(0]. WU]... W0N
Ao    901 we A=                       60102)
ie  Ao    AQ Awa
Gyo = 9711  이  Qy-1,N-1

식 (6.62)에서 Gin & 다음과 같이 정의된다.

284



===== PAGE 283 =====
Ay im =H,[k-—m]+H[k-m]ev7"" +

                                                     (6.63)
+H, [k-melvr"?'™ | mk =0,1,-**,

N-1

Magnitude

a

를 Alk-m)7} 모두 0이 되므
Oo] 된다. 그러나 채널이 한 심볼
Lk -m] 7} 존재하게 된다. 그 결과 HY
다. 만약 한 OFDM 심볼 주기 동안에 aaa
각 경로의 채널 변화를 작은 기울기를

채널의 특성이

=

rr 8

시

률을 나타내는 상대적 도플러 주파수 변화율
EE        He 직선으로 ais 수
는 주과수영역에서 몰 때이 대부분
eich 즉. 식 (6.62)의 HBA] DC HR
크

고
에    rf

|

[ 즈키

임펄스 &
uo

ㅇ

a

rir

식
밑     갖

ee

=
다

그림 6.18(2)는 도플러 주파수가
볼 구간 동안에 3 경로로 구성된

Jakes 모델을 사용하였다.

값을
We

= % 꼼
rat

각각
이
a

[20

각
mA
5 or

Time variation within a symbol

C 부근에 집중되어 2
게 되고 나머지 대각선 항에서

Hz, 50Hz, 100Hz]°l
one

A] (6.63) 4] mat k 값이 다
만 남게 되고 나머지는 모두

k 값이 다른 경우에도
닌 같을 가질 수 있게
널의 변화가 크지 않을 경우에
형태로 근사화할 수 있다. 즉, 채널의
(4/, ) 을 T,/ fp 로 정의하면,  Mf <0.1
있다. AS 기울기를 갖는 직선의 에너
있기 때문에 식 (6.62)은 간
나타내는 대각 성분과 그 인접 몇 개
멀리 떨어진 항들은 거의 0의 같을 갖

의 아

<

상황에서 한 OFD

채널 변화를 보여준다. 여기서 치

Magnitude response

0.8                                                                                   x              x

ray                                A

——®— 20Hz
—t&— 50Hz
—x— 100Hz

-|—e— 5072
“|—<— 100Hz

Magnitude

0.6 개 기지 ㅎㅎ ae _

se      1@   a a         mee   〉   !   H   '   {   ;
O02           100 200 300 400 500 600 700 800 900                     -200 -150 -100 -50          0           50         100 150 200
Sample                                 Frequency[kHz]
(a) 한 OFDM 심볼 구간 동안의 채널 변화             06) 주파수영역의 크기 응답

그림 6.18 도플러 주파수

변화에 따른 채널 특성



===== PAGE 284 =====
PART Il_ OFDM2} MATLAB

그림 6.180)로부터 한 심볼 구간 내에서 채널의 특성이 선형적으로 변
있으며, 그 기울기는 도플러 주파수가 SIAR 커지는 것을 알수 있다. 그림 61800는
이 정우 주과수영역에서의 크기 응담을 보여준다. 이 그림으로부터 AH
에 집중되어 있으며 DCA 멀리 떨어질수록 크기 같이 감
도플러 주과수가 SSH ICL} 증가하는 것을 알수 있다. 이와 같이 주
시키는 인접 부채널의 수를 라고 할 경우에 식 (6.63)의 a, & 다음과

본

my
의
N
aS
ial
a

a,» =0 for |k-m|>q/2                   (6.64)

즉, 번째 부채널의 좌우 각각 4/2개의 부채널들이 ICS 발생하는 중요한 요소가 되며
나머지 항들은 그 영향이 미약하므로 0으로 근사화할 수 있다. 이 경우 식(6.62)의 WE
다음과 같이 나타낼 수 있다.

90.0 961     Qo 4/2   0         0
Ao  a)      ：               :
                        0
H=| 4,29 7                a   Oy-1-4/2,N-1       (6.65)
0              ：          :
                 Gy-2,n-2  Ay_2.n-1
PO 0 Gy yetegi2 1 Ayer Ava |

위 식으로부터 고속의 이동성을 갖는 OFDM 시스템에서는 채널 왜곡을 단일탬 등화기
로 보상하기 어렵기 때문에 $2] ICE 고려하여 X= HY 가 되어야 한다. 그러나 Wx
ANS 갖는 HBA] 역행렬을 수신단에서 구하는 것은 쉽지 않기 때문에 시변 특성이
아주 크지 않은 경우에는 식 (6.65)를 사용하여 간략화할 수 있다.

식 (6.65)에서 알 수 있듯이 근사화된 H YAS 0이 아닌 원소가 행렬의 대각선과 그
주위에 집중되어 있는 밴드 행렬(6000 matrix) 형태가 되며 그 밴드의 한 쪽 폭은 gi27h
된다. 이 경우 식 (6.65)은 q=N 인 조건하에서 0인 원소가 매우 많은 sparse 행렬이 되므
로 HY 를 계산하기 위해 뻐 의 전체 역행렬을 구하는 것은 매우 비효율이다. 따라서 계
산을 단순화시키기 위해 밴드 행렬을 4-개의 부행렬로 구성된 블록-대각(01006-
diagonal) 행렬로 재구성할 수 있다. 그림 6.19는 행렬의 재구성 방법을 보여준다.

286


===== PAGE 285 =====
0 ! : x Co

iN

2      ~          02
개                           ×
× ×                        a 옷
x[x x   | ____—             _—
x x|x                       ry
L           Nivga2) 4 Xx                        ‘
N-q-l
그림 6.19 블록-대각 행렬로의 변환 방법

그림 6.19의 YAS 통해 뻐 행렬을
있다.

A,        0
                 A,
H=
0                   Ay-tg
Gain         Gant      a      Ga ntq/2       0            aa                  0
Fron Annet                    ic                                               :
;                                                                                          0
A, -  nag/2.n       .                                      “5        Qrigl2yntq
0
An+g-intq-l     Gnsq-intq
[   0       ne     0   Qeeanvg ! Gave nega    Gigante |

따라서 식 (6.61)은 재구성된 HS 이용해서 다시 표현할 수 있다.

Y=HX+W

여기에서 X,Y, We 다음과 같이 정의된다.

대각선 항이 부행렬로 이루어진 Hs 변환시킬 수

(6.66)

(6.67)

287



===== PAGE 286 =====
PART ㅁㅁ OFDMZ} MATLAB

= 지사, |) X,= [Xi Xin tlh Xin tall”
Y =[Y,.¥o-5¥y,] > ¥,= lb ¥intih-.Yin+qll’                (6.68)

W =[W,.Wo- Wy, |W, = In thn + gly

A= yy                                                       (6.69)

여기서 H 은 block—diagonal 행렬이므로 그 역행렬은 각 대각 행렬의 역행렬을 구하
는 것과 같기 때문에 (08) 은 다음과 같이 주어진다.

A)                    0

테그              Ay
(H)'=                                                                (6.70)

우 계산량이 크게 감소된다.

이와 같이 고속 페이딩 채널에서 발생하는 ICI] 영향을 보상하기 위해서는 주파수영역
에서의 채널 SWS 정확히 추정하는 것이 중요하다. 시변 채널을 추정하기 위해서 주
파수영역에서 WIS ES 이용하는 방법, 시간영역에서 wal ABS 이용하는 방법 등
의 많은 연구가 최근까지도 이루어지고 있다[157][160]. 그러나 데이터를 전송하면서 시
변 채널을 추정하는 것은 일반적으로 쉽지 않은 일이기 때문에 앞으로 많은 연구가 필요
한 분야이다. 이 외에도 101의 영향이 상쇄되도록 ATS 전송하는 기법과 같이 채널을 추
정하지 않고 ASS 검출하는 방법 등의 시변 채널에서 데이터 ASS 위한 많은 연구가

이루어지고 있다[161][1621.

288


===== PAGE 287 =====
OFDM 시스템에서는 입력 신호가 많은 독립적인 부반송파에 변조되어 실려 전송되는
데 이들이 같은 위상으로 더해질 때에 시간 영역에서 큰 크기의 신호가 발생하여 최대 전
“(peak power)°] 평균 412(average 00\8601)보다 크게 증가하게 된다. 즉, OFDM 신호는
단일 반송파 전송방식에 비하여 PAPR(Peak-to-Average Power Ratio)©] 증가하는 단점이
있다. 신호의 248 이 증가하게 되면 ADCS} 24ㅅ0의 SQNRS] 저하되며, 송신부 RF 단
의 전력 증폭기의 효율이 감소하게 된다. 특히 PAPRE 송신기의 전력 중폭과 직접 관련
되기 때문에 전력 수급이 Sole 기지국보다는 배터리에 의하여 수명이 결정되는 단말기
의 상향링크 전송 시에 더욱 큰 영향을 주게 된다.

0000 185 00

OFDM 신호는 PAPR7} 크기 때문에 RF 단의 전력 증폭기에 의하여 비선형 왜곡이 발
생할 수 있다. 실제로 모든 입력 신호의 크기에 대하여 선형적인 출력을 갖는 전력 중폭기
는 존재하지 않고, 일반적으로 특정 레벨의 Sas 넘게 되면 증폭기는 포화(640448000)되
어 비선형 왜곡이 발생된다. 이 때 비선형 구간이 시작하는 영역은 그림 7.1에 나타난 바
와 같이 [BO(Input Back—Off)2} OBO(Output Back—Off)°]] 의하여 정의된다[163].

IBO =10log,,(P?* / P,,)                  (7.1)
OBO =10log,. (Pn / Px)                                (7.2)
289


===== PAGE 288 =====
PART [ _ OFDM2} MATLAB

| Pa

OBO

시 pinas      ~
IBO—>41  —
그림 7.1 고출력 증폭기의 입ㆍ출력 특성

이와 같은 고출력 증폭기 Power Amplifier; HPA)2] 비선형 특성은 수신 신호의
성좌도에서 신호의 회전, 감쇄, SA, 뒤틀림 등의 왜꼭을 일으키고, 주파수영역
밖으로 스펙트럼을 방사시킨다. 이러한 고출력 증폭기의 비선형 특성을 나타내는 지표로
서 EVM(Error Vector Magnitude), ACPR(Adjacent Channel Power Ratio), IMD(Inter—
Modulation Distortion) 동이 있다. 대역 밖으로 방사되는 에너지를 나타내는 지표인
로부터 알 수 있듯이 고출력 증폭기의 비선형 특성으로 인하여 자기 대역에서 신호
를 왜곡시킬 뿐만 아니라 다른 대역의 신호에까지 영향을 미치게 된다. 이러한 고출력 증
폭7 0 비선형 ASS 감소하기 위하여 일반적으로 송신 신호의 최대 MAS 제한된다.
의 비선형 왜곡을 피하기 위해서는 모든 입력 신호의 크기가 고출력 증폭기의 선형
| 구간 내에서 존재해야 하는데, OFDM 신호는 많은 부분이 선형 동작 구간 내에서
재하지만 피크 신호가 고출력 증폭기의 선형 동작 구간 외에 종종 존재한다. 넓은 범위
의 선형 동작 구간을 갖는 고출력 증폭기는 크기가 크며 가격이 비싸고 발열이 높기 때문
히 단말기의 송신부에 사용하기에는 어려움이 있다.
으       반송파 전송방식에서는 송신 신호가 PSK, 0444과 같이 분포가 균일
크기가 제한되어 있기 때문에 240#이 작게 나타난다. DS-CDMAS] 신호
의 경우에는 하향링크에서와 같이 다중 사용자의 신호가 더해진 곳에서도 PAPRO] 증가
하는 현상이 발생하나[164], 본 장에서는 다중 반송파를 사용하는 OFDM 신호의 PAPR
에 대해서만 다루도록 한다.

290


===== PAGE 289 =====
제7장_『ㅁ466 감쇄 기법

PAPR 정의

본 절에서는 PAPRI} 이와 유사한 정의에 대하여 설명한다. 그림 7.2는 통과대역
(08896800)에서의 PAM 송신기를 나타내고, 이 중 0480780416 변조기를 수식으로 표시하
면 다음과 같다[1].

V2 cos (27f,t)

이] | Transmit | s(t)

Filter                        (x)

Tok >) Mapper                                  이                                       BF  2
Transmit                                         s(t)

Filter                   (x)

agin]            8 g(t)            t
— V2sin(2rf,t)

그림 7.2 통과대역 PAM 송신기

§(t) =       -kT), = }

SU)= 2 alle Be)     2                    (7.3)

s(t) = V2 Re{(5,(1) + jig) e"”"}                                       (7.4)
여기서 (.)/ 와 Jo 각각 (.) 2] in-phase2} quadrature 성분을 나타내고, 7; 는 샘플링 주

기를 나타낸다[165].

ㆍ PMEPR(Peak-to—Mean Envelop Power Ratio)

PMEPRE: 기저대역의 복소 신호 F(t) 의 포락선에 대해서 최대 전력과 평균 전력의 비
를 나타낸다[165].

0000

1000

PMEPR{3(t)} =                                                             (7.5)

PMEPRE. 기저대역에서 연속시간 신호에 대하여 측정되는 값이며, 실제로 HPA 입력
신호에 대한 측정치는 아니다.

291



===== PAGE 290 =====
PART Il_OFDMiZ} MATLAB

ㆍ PEP(Peak Envelop Power)
PEPE 기저대역의 복소 신호 $(7)의 최대 전력치를 나타낸다[165].

PEP{3(1)} = Max|;(t)'                                   (7.6)

[에

이 때, 일반적으로 맵퍼에서는 변조 지수에 따른 정규화를 수행하기 때문에 맵퍼 출력 신

호의 평균 전력 Ls)? }은 1로 정규화 되었다고 가정할 수 있다. 이러한 경우에
ne PEPS} 같이 Max|s(r)|’ 만으로 정의하기도 한다.

* PAPR(Peak—to—Average Power Ratio)

PAPRE 실제 비선형 왜곡을 발생시키는 고출력 증폭기의 입력 신호 s(t) 에 대하여 |
대 전력과 평균 전력의 비로 정의된다[165]. PAPRS 통과대역에서 변조된 연속시간 신호
전력의 최대치와 평균치의 비로 주어진다.

Max|Re(5(# (S(t    ell! Jer) - Max|s(t)}

디아 ㆍ 18000                 “

PAPR{s(t)}=

* CF(Crest Factor)
CFE 아래와 같이 RFS 기저대역에서 모두 정의되어 있으며, CFE 신호의 전력이 of
닌 크기에 대하여 주어진다[165].

RF condition: CF = /PAPR                                   (7.8)
Baseband condition: CF = PMEPR

이러한 이유로 많은 논문과 기고문에서는 PAPRI} CFS 훈용하여 사용하고 있다. 야는
다음에서 설명하는 CCDF(Complementary Cumulative Distribution Function) 유도하
는 과정에서 수학식을 간단하게 표현할 수 있기 때문에 종종 사용된다.

위에서 정의한 PMEPR, PEP, PAPR, CF 중에서 가장 널리 사용되는 지표는 240#과
(개이다. PSK 변조된 신호가 개의 부반송파를 갖는 OFDM 시스템에서 전송될 경우에
최대 전력은 개의 신호가 동일한 위상으로 더해질 때 발생하며, 이 때 최대 전력은 평

292

0 0 0 0 0



===== PAGE 291 =====
제7장_『ㅁ4066 감쇄 기법

균 전력의 /배가 된다. 만약 신호가 QAM 변조되었다면 이 Be 더욱 커진다. 그러나 실
제로 부반송파의 수 Vo] 증가함에 따라 가장 큰 PAPRO| 나타날 확률은 줄어든다[166].
예를 들어, M—ary PSK OFDM 시스템에서 가장 큰 PAPRE 가질 수 있는 ASE 44”
개 존재한다. 이러한 경우에 가장 큰 PAPRO| 나타날 수 있는 확률은 MP) MY =
이 된다. 만약, W=320]51, QPSKS 사용한다면 그 확률은 8.7×10 °° OFDM 심볼 길
이가 100 us 인 경우 가장 큰 PAPRE 370만년에 한번 나타나게 된다[167]. 이와 같이 위
에서 설명한 신호의 전력에 대한 정의들이 의미 있는 정보로 사용되기 위해서는 값의 분
포가 함께 고려되어야 한다. 이러한 이유로 신호의 전력이 고출력 증폭기의 선형 동작범
위를 넘어설 가능성을 나타내는 전력 분포의 CDF(Cumulative Distribution Function)=
PAPR 관찰에 많이 사용된다. 특히 PAPRAA| 관심이 있는 분포는 특정한 전력 레벨을
넘어서는 확률 분포이기 때문에 CCDE7} 많이 사용된다.

* CCDF(Complementary Cumulative Distribution Function)

OFDM 시스템에서 IFFTS| 입력신호는 QPSK 또는 QAM 등과 같이 크기가 제한되고
균일(04011000)한 분포를 갖지만, N-pointS 갖는 IFFTS] S42 No] 충분히 클 때 실수
Hol 허수부 신호가 중심 극한 정리(660081 limit theorem)°] 의해 각각 Gaussian 분포를
갖게 된다. IFFTS] 출력 신호의 A7|= Rayleigh 분포를 갖게 되고, AHL central
Chi-square 분포를 갖게 된다. 이 경우 Rayleigh 랜덤 변수인 n 번째 샘플의 크기 2, 의

fr, (2)= 2ze*                                        (7.9)
곱셈 법칙에 의하여 CFS] 누적분포함수는 다음과 같이 주어진다.

aN
F,, (z)=P(maxZ, <z)=P(Z,<z):P(Z,<z)--P(Zy1<z)=(I-e*) 0040
PAPR 분석에서는 애가 z 보다 작은 경우의 CDF 보다는 z 보다 클 확률인 CCDF7} 더욱
중요한 지표이기 때문에, Nyquist 샘플링된 하나의 OFDM 심볼에 대하여 애가 = 보다
클 확률인 CCDFE 다음 식과 같이 주어지고[167], 이는 부반송파수 에 대하여 그림
7.3과 같이 나타난다.

293

0000 0 0 00


===== PAGE 292 =====
PART 1 _ OFDM2Z} MATLAB

OM system with N-  ll FFT

10 pistes                   = a
~               ai : 기 tae
a                  Sanaa ENR Simulation

CCDF

10?

4    5

그림 7.3 개의 부반송파를 갖는 OFDM 신호의 CCDF

(0) =P(CF>z)=1-P(CF <z)

=1-F, (2)=1-(1-e*)"

(7.11)

aie geist 않는다. 그 ai 위와 같이 Niquist 샘플링된 ASE aA 연속시간
영역의 최대 값을 항상 포함하지는 않기 때문이다. 그러나 실제로 오버샘플링이 적용된
신호에 대하여 정확하게 최대 전력 분포를 유도하는 것은 쉽지 않기 때문에 van *066와 de
\110는 다음과 같이 간략화된 CDFS 유도하였다[168].

F,(z)=(1-e*)"                              (7.12)

여기서 a 모의실험에 의하여 약 28H 주어지지만, 이론적인 뒷받침이 부족하여 2 NV
의 경우에는 약간의 오차가 발생한다. 프로그램 7.1은 그림 7.3과 같이 개의 부반송파를
가진 OFDM 신호의 CCDF 곡선을 그리는 데 사용된 프로그램이다.

ㆍ 294



===== PAGE 293 =====
제7장_ 『ㅁ456 감쇄 기법

* 0106 _CCDF.m
* Plot CCDF in Fig. 7.3
N = 2.*[6:10]; bits = 2; Nblk = 10*4; z = [2: 0.1: 10];
ecdf_fne = inline('1-((1-exp(-z*2/(2*s2)))*N)', 'N', 's2', 'z');
forn=1: length(N)

for k= 1 ㅎ Nblk

[XI, XQ, Mo, Nsym] = mapper(bits, N(n), 'Y');
xblk(k,:) = ifft (XI+j*XQ,N(n))*sqrt(N(n) ) ;
CFx(k) = PAPR(xblk(k,:));

end
s1=mean (mean (abs (xblk) ) ) /sqrt (pi/2); s2 = s1*2;
for tz = 1: length(z)

ecdf (1,tz) = ccdf_fnc(N(n), s2, 10*((z(tz))/20))
end
for zi = 1: length(z)

cecd£_z(zi) = sum(CFx>z (zi) ) /Nblk;
end

end

igi 프로그램 7.1 OFDM 신호의 CCDF 실행 프로그램

그림 7.4는 단일 반송파를 사용하는 경우에 QPSK 변조된 기저대역 신호와 통과대역
신호의 PAPRS 나타낸다. 4배 오버샘플링된 신호에 대하여 기저대역 신호는 평균 주
최대 전력이 동일하여 PAPR°] 0008이 되 “ 중심 주파수 L=1HZS 사용하고 이상적인
저역 통과 필터를 적용한 경우에 통과대역 ASL oF 308이 된다. 이와 같이 단일 반송파
통신 시스템에서 240#을 정확하게 측정하기 위해서는 SAAS 중심 주파수 LS 고려
해야 한다. 일반적으로 단일 반송파를 사용하는 경우에는 변조 방법에 따라 PAPRO| 같이
예측 가능하며, 그 분포가 많은 부반송파를 사용하는 OFDM 시스템에서와 달리 제한되어
있기 때문에 OFDM 시스템에 비하여 PAPRo} 민감하지 않다. 프로그램 7.2
(“single carrier PAPR.m”)= 그림 7.42} 같이 QPSK 변조된 기저대역 신호와 통과대역
신호의 PAPRE 그리는 데 사용된 프로그램이다.

295



===== PAGE 294 =====
PART 1 _아미/과 MATLAB

OASIS 4 symbols, Ts=1s, Fs=8Hz, L=4, g(n)=u(n)-u(n-Ts)              4  QPSK, 4 symbais, Tels, Fs=8Hz, Lad, fer Hz, a(n) ula) -ult=Ts)

a,  11100  ,;
= TMM   vin fo fll

TU ETT  1 06 1 15  ti

Be
=
in
rw
nw
a
or
wo
ao
~
S(n)
+ 6
~

8600)
=
기
eal
os
|
al
aa
cel
|
20
al
~
스그
as]
ama
—]
nm

PAPR = 3.0108
76 06 1 15 2 25 3 38 4       ist                                                       |
i                                      PAPR = 008                                        ral
을 !                                                       들
[ej                                                         bes
= 0.55                                                    7]       0.5                                                    1
oa a a 1 015 2 25 8854             0 05 1 15 2 25 3 35 4
samples                                                    samples
(a) 기저대역                   (6) 통과대역

그림 7.4 QPSK 변조된 기저대역 신호와 통과대역 신호의 PAPR

% single carrier PAPR.m
6 Plot Fig. 7.4
Ebits = 2; Vbits = [1 [2 : 2 ; 2*Ebits]]; Ts = 1; L = 4; Fe =1;
for tmp_i=1: Ebits+1
bits = Vbits(tmp_i);
Nsym = 1*2*bits;
[inI, inQ, Mo, Nsym] = mapper(bits, Nsym, 'N');
[tmp_out,tmp_outI,tmp_outQ,tmp time] =modul (inI,inQ,Nsym,Ts,16,Fc) ;
[out, outI, outQ, time] = modul(inI, inQ, Nsym, Ts, L, Fc);
[papr_dB(tmp_i), avgP_dB(tmp_i), peakP_dB(tmp_i)] = PAPR(out) ;
[deMi, deMq, detime] = deModul(out, Nsym, Ts, L, Fc);
for tmp j = 1: Nsym
bb _I(L* (tmp _j-1)*2+1:L*tmp_j*2)
bb_Q(L* (tmp_j-1)*2+1:L*tmp_ j*2)
end
papr_dB(tmp_i),avgP_dB(tmp i),peakP_dB(tmp_i)]=PAPR(bb I+j*bb Q);
end

1701 (tmp_j) *ones(1,L*2) ;
inQ(tmp_j) *ones(1,L*2) ;

WW 프로그램 7.2 단일 반송파 신호의 PAPR 분석 프로그램

296



===== PAGE 295 =====
제7장_『ㅁ4^6ㅁ 감쇄 기법

 OFDM 신호의 분포

그림 7.5는 OFDM 시스템의 블록도를 나타내고, 이 그림에서 송신단 IFFT 이후의 이
산시간 영역 신호 xn] 식 (7.13)으로 주어진다.

Input Bit                                      X[k]             z(n]                                         e 02
Sequence                                                 Add                 a(t)
| encoder | |. |: eer |: jie: | os         se
Transmitter                                            5
Receiver                                             —
fat Bit                               7    :    7           =
quence                                     <     3     0 <         :          0100
※… RM                      Nepointi~ - |jau. I
Decoder       jigs      FFT    ‘  pew    5   S/P ;    AD
Y[k]          y(n]                                      eo Pte

그림 7.5 OFDM 시스템의 블록도

x[n]= lee                                          (7.13)

위 식에서와 같이 2171]은 직교하는 NH 다중 부반송파에 X[k] 신호가 실린 후 시간
같

영역에서 더해져 그림 7.6과 같이 나타난다.
rks   liad    AS              02    ㅠㅜ   = ie   —

0
-0.05 -0.04 -0.03 -0.02 -0.01 0 0.01 0.02 0.08 0.04 0.05

=  0.27     T      T      T      T      T      T      T      T      T

0
0.05 -0.04 -0.03 -0.02 -0.01 0 0.01 0.02 0.03 0.04 0.05

T         T         T         T         T         T

은
g
|
은
i

Ix(t)l

2 ¢
o 8

pdf lof Ix(t)

o
a—2

=
fo}
oS
ho
So
[00
은
So
a
So
a
은
N
으
fo}
S
wo
=

fh non as hae           1             1
0.01 0.02 0038 004 005 006 0.07

t                                   Xo
(a) 시간영역 신호                        (6) 확률밀도함수

Site (QPSK, N=8, 16)

ㅣ

297


===== PAGE 296 =====
PART 므_ OFDMZ} MATLAB

그림 7.6(a)2| 00 신호로부터 부반송파의 수 No] 증가함에 따라 240#이 증가하
며,신호의 확률밀도함수는 NO] 증가할 경우 x (2 xo (NE Gaussian HES 따르며,

페

|x(¢)| 는 88510 분포를 따르는 것을 알 수 있다. 이와 같이 OFDM 신호 xHE 넓은 범
위에 걸쳐 분포하기 때문에 고출력 증폭기의 선형 동작 구간 내에서 동작을 시키는 것이
불가능함을 알 수 있다.

프로그램 7.3(“OFDM 818081.0”)은 그림 7.6과 같이 OFDM 시스템의 시간영역 신호와
확률밀도함수를 그리는 데 사용된 프로그램으로서, 연속시간 OFDM 신호와 유사한 결과
를 얻기 위하여 L=16 oe 설정하였다.

% OFDM signal.m

% Plot Fig. 7.6

N= 8; bits = 2% L = 16;

[inI, inQ, Mo, Nsym] = mapper(bits, N, 'Y');
inI(1) = 0; inQ(1) = 0; % DC-subcarrier
time = [0 : 1/N/L :1 - 1/N/L];

for i= 1 +N

if (i<= N/2)

out=ifft ( [zeros (1,i-1),inI(i)+j*inQ(i),zeros(1,N*L-i+1)],N*L) ;
else

out=ifft ( [zeros (1,N*L-N/2+i-N/2-1) , 101 (i)+j*inQ(i) ,zeros(1,N-i)] ,N*L) ;
end

outI(i,:) = real(out); outQ(i,:) = imag(out) ;
end
SoutI = sum(outI); SoutQ = sum(outQ) ;
N = 2°4; time = [0 : 1/N/L :1 - 1/N/L]; Nhist = 1e4;
fork =1 : Nhist
[inI, inQ, Mo, Nsym] = mapper(bits, N, 'Y');
inI(1) = 0; inQ(1) = 0; % DC-subcarrier
fori=1:N

if (i<= N/2)

out=ifft ([zeros(1,i-1),inI(i)+j*inQ(i) ,zeros(1,N*L-i+1)],N*L) ;
else

out=ifft ( [zeros (1,N*L-N/2+i-N/2-1) , 101 (i)+j*inQ(i) , zeros (1,N-i)],N*L) ;
end

298



===== PAGE 297 =====
제7장_ㅁ46 감쇄 기법

outI(i,:) = real(out); outQ(i,:) = imag(out) ;
end
Hout I (N*L* (k-1)4+1:N*L*k) =sum(outI) ;
HoutQ (N*L* (k-1) +1:N*L*k) =sum(outQ) ;
end

Ta) 프로그램 7.3 OFDM 시간영역 신호의 확률분포 분석 프로그램

back-offS 크게 하는 것은 비효율적이라는 것을 알 수 있다. 이라한 관층
제로 OFDM 시스템에서는 적절한 크기 레벨 poor) 클리핑을 하는 방
키기 위해서도 사용된다. 그림 7.7에 나타난 바와 같이 클리핑 레벨을 높

핑 왜곡은 크게 발생하지만 양
= trade-off 관계에 있어 이를 함께 고려한 비트 수 선정이 필요하다.

QPSK, N= 16

05   clipping level 0.5

0.사                                          all
0.3} clipping lefel 0.25                    i
025                                             el
0.1                          TT
0                          et
01                          +4
-0.2                              nbits |
0.95                           quantization |
n bits.
-05                               quantization
n bits.
+4                                    quantization

0

그림 7.7 OFDM 신호의 실수부 분포

그림 7.7은 OFDM 시스템의 시간영역 신호 *()의 APY BES 보여준다. 그림 7.7로
부터 *()의 실수부는 Gaussian 분포를 갖게 됨을 확인할 수 있다. 즉, Wo] 증가함에 따
et 피크 값은 증가하나 피크 값이 나타날 확률은 지수적으로 감소하게 된다. 따라서 가끔
발생하는 피크 값을 왜곡시키지 않고 선형적으로 증폭하기 위해서 고출력 증폭기에서
찰을 바탕으로 실
}법이 종종 사용된
다. 이러한 클리핑 방법은 송신기내 고출력 증폭기와 수진키의 ADC 동작 범위를 제한시
게 설정하면 클리
BASS 발생하지 않지만 양자화 잡음이 증가하고, 클리핑 레벨을 낮게 설정하면 클
자화 잡음이 감소한다. 따라서 클리핑 레벨과 양자화 잡음



===== PAGE 298 =====
PART Ｌ 아미/과 MATLAB

그림 7.8은 N=649) 경우에 ADC 비트 수와 클리핑 레벨에 따른 SQNR 값을 보여준
다. 여기서 SQNR 값은 클리핑 왜곡과 양자화 잡음의 영향을 함께 반영한 값이며, 각 비
트 =o] 대하여 최대 SQNRS 갖는 경       정색으로 표시하였다. 이 그림으로부터 최
대의 클리핑 AWS 사용하는 비트 수에 따라 달라지며, 좌쪽의 Zap} 급한 HHS 클
핑 잡음이 지배적인 SS 주는 부분이고 우측의 Zap} 완만한 부분은 양자화 잡음의

영향이 큰 부분임을 알 수 있다. 비트 수에 따라 최적의 클리핑 레벨이 다르지만 일반적으
로 클리핑 quis 46 로 설정할 BF] 전체적으로 SQNR 값이 높기 때문에 클리핑 왜곡
과 양자화 잡음을 함께 고려하여 클리핑 qs 일반적으로 46 로 설정한다. 프로그램
7.4는 그림 7.8을 얻는 데 사용되었다.

Effect of a N=   64, 7 =0.088102)

= 6bits quantization

'           {           |        —*— =7bits quantization
45 Slee ace  pce  24 ~*  = 8bits quantization
|           |           |        -ㅡ---= Qbits quantization

50

1 (clipping level normalized to ㅇ)
그림 7.8 OFDM 시스템에서 클리핑 레벨에 따른 SQNR

SQNR_with_quantization_clipping.m
Plot Fig. 7.8
N = 64; bits = 6; L = 8; Nblk = 104;
TWL = [6:1:9]; IWL = 1; FWL = TWL - IWL; mu = [2: 0.2: 8]; varx = 0;
for k = 1: Nblk
[XI, XQ, Mo, Nsym] = mapper(bits, N, 'Y');
x = ifft (XI+j*XQ,N) ;
varX = varX + (sqrt (var(real(x))) + sqrt (var(imag(x))))/2;
end

oe oe



===== PAGE 299 =====
HI7Z_PAPR 감쇄 기법

sigma = varX/Nblk; SQNRe = 26208 (16090 (014) , length(mu) ) ; varX = 0;
for f = 1: length(FWL)
for m=1: length(mu)
Tx =0; Te = 0;
for k = 1: NbLk
[XI, XQ, Mo, Nsym] = mapper(bits, N, 'Y');
x = ifft (XI+j*XQ,N); x = x/sigma/mu(m) ;
CxI=fi(real(x), 1, IWL+FWL(f£), FWL(f), 'roundmode', 'round',

‘'overflowmode', 'saturate'); CxI=double(CxI) ;
CxQ=fi(imag(x), 1, IWL+FWL(f), FWL(£), 'roundmode', 'round',
‘overflowmode', 'saturate'); CxQ=double(CxQ) ;
Px=sum(x.*conj(x)); Pe=sum((x- (CxI+j*CxQ) ) .*conj (x- (CxI+j}*CxQ) ) ) ;
Tx = Tx + Px; Te = Te + Pe;
end
SQNRe(f,m) = 10*1log10(Tx/Te) ;
end
end

ia) 프로그램 7.4 OFDM 신호의 클리핑 레벨에 따른 SQNR 분석 프로그램

 『ㅁ40#과 오버샘플링

식 (7.7)에서 주어진 PAPRE 연속시간 영역에서 반송파 주파수 /,로 변조된 통과대역
신호에 대하여 정의된다. 일반적으로 fe 1/ 7;』보다 훨씬 높기 때문에 OFDM 신호에 대
해서는 통과대역에서 측정한 24#과 기저대역에서 측정한 PAPRO] 거의 동일하다[167].
기저대역에서 연속시간 신호에 대해서 240#을 측정할 경우 통과대역에서와 유사하나,
기저대역에서 Niquist 샘플링된 신호 x[nJol 대하여 PAPRS 측정한다면 이는 원래
PAPREC} 일반적으로 낮은 값으로 주어진다[164][169]. 실제로 DACS 포함한 하드웨어
구현 전에 연속시간 신호에 대하여 PAPR 측정을 하기가 쉽지 않기 때문에, 기저대역에서
이산시간 신호 x [n]}S 사용하여 PAPRE 근사적으로 추정할 수 있는 방법이 필요하다.
OFDM 시스템에서 이산시간 영역 신호의 PAPR 값은 24 인 경우에 연속시간 영역 신
호의 840#과 유사하기 때문에 본 절에서는 기저대역에서 오버샘플링하여 PAPRS 측정
하는 방법을 설명한다[164].

그림 7.9는 』배 만큼 정수배 오버샘플링하는 보간기의 블록도를 보여준다[170].

ful



===== PAGE 300 =====
PART Il_ OFDM} MATLAB

                            Anti-  -imaging |
t           4101]
[0]   | |   i Z            LPF           ylm]
0                              Lf,                              Lf,
LG

그림 7.9 HH 보간기의 So

그림 7.9에 나타난 바와 같이 Nyquist BEY [의 신호 사이에 -1개의 0을 Af
입하여 w [/0]을 구성한 후, 이상적인 저역 통과 필터를 통과하는 경우에 이산영역 신호를
다음과 같이 왜곡없이 오버샘플링을 할 수 있다.

= >, Alk]w[m—-k]                         (7.14)
k=-00
x[m/L],     m=0, +L, +22, ...
w[m] =                                    (7.15)
0,         elsewhere
그림 7.107} 그림 7.112 2012에서 샘플링된 ASS 8로 오버샘플링하는 경우

(L=4) 시간 영역과 주파수 영역에서 보간 과정을 나타낸다. 만약 오버샘플링 배수
정수 배를 만족하지 않는 경우에는 보간기와 데시메이터를 결합하여 오버샘플링된 신호
얻을 수 있다. 기저대역에서 이산시간 신호의 2408을 측정하기 위해서 424 을
면 되기 때문에 여기서 데시메이션 과정은 고려하지 않는다.

는
18,

ala

마족
1

1
=

01234567891 12 13 14 15

ylm]

012345678 9 feTi2i31415 ™
그림 710 보간 과정의 시간 영역 BS (L=4)

302



===== PAGE 301 =====
제장 6476 감쇄 기범

120)|          phos들    도.
;         © if         ff         ee
ㆍ                                      ,
Se           Sse!           Na

0 1 2 84 5|6 7 8

Iw(f)| 05 ^ 으으

011 2 3 4 51 6 7+ 6 *
Lf,/2
Oh 세 1 |
0 1 2 383 45167 8“
180) a                      -
0 1 2 3 4 5 6 7 8
그림 7.1 보간 과정의 주파수 영역 표현 (4 =4)

그림 7.5의 OFDM 시스템에서 IFFT 출력 신호에 대하여 Lv 오버샘플링된 이산시간
신호 x'[m] 는 다음과 같이 주어진다.

L-N-1
[m]=—-    pe el e  pen m=0,1,...NL-1
(7.16)
Xk      O<sk<N
0,         elsewhere

여기서 NV, Af, XU: 각각 전체 부반송파 수와 부반송파 간격, 부반송파에 할당된 값
을 나타낸다. 식 (7.10)은 기저대역에서 IFFT 블록에 N(L-1) 749] 0을 패딩한 후 필터
링하여 Lu 오버샘플링된 이산시간 신호 x'[m] 를 구하는 방법을 나타낸다. 이 경

상적인 저역 통과 필터를 사용한 결과와 동일한
ABS 사용할 경우 식 (7.7)의 PAPRE 다음과 같이 재정의된다.

ed

PAPR=    Osm<NL

ai 끼 |

PAPR 측정 과정에서 오버샘플링의 영향을 확인하기 위하여 PAPRo| 적은 신호로 알
려져 있는 CAZAC(Constant Amplitude Zero—Autocorrelation Code) A] 322] 한 부류인

찌|

303



===== PAGE 302 =====
PART Il_OFDMZ} MATLAB

Chu 시퀸스와 IEEE 802.166에 정의된 프리앰블 Also] 대하여 PAPR BAYS 살펴본다.
Chu 시퀸스는 다음과 같이 정의된다[1711].

ink            .
!         N
X,(k)=  때 |            =—_—  Osis N-1, ged(k,N)=1       (7.18)
en             N is odd
Chu 시퀸스는 크기가 19) 복소 신호이고, IFFT 이후에 OF} 19) 값만 존재한다[172]. 따라

서 Chu 시퀸스는 3-408의 낮은 PAPR 값을 갖게 된다.

IFFT(X(k)), k=3, N=16, L=1.4                                   IFFT(X(k)), k=3, N=16, L=1.4

1, PAPRE 008
따는 4.27108

Pod Ee EE 이        0 Of 02 03 04 05 06 07 08 09 1
-0.4 -0.3 -0.2 -0.1 0 O01 02 03 04 05        time(normalized by symbol duration)

그림 712 오버샘플링에 따른 Chu AMAL] PAPR 특성 (N=16, k=3, L=l, 4)

그림 7.12에 나타난 바와 같이 Nyquist 샘플링을 한 BP L=1) IFFT 이후 Chu 시퀸스
는 일정한 크기 값2408#=0008)만 갖지만, 4배 오버샘플링된 경우에 시간영역 신호는 일
정하지 않은 크기?40#=4.27108)를 갖는다. 그러나 과 ko] 따른 Chu 시퀸스의
PAPR 분포는 여전히 랜덤한 신호의 PAPR 보다 낮다. 그림 7.12는 프로그램 7.5를 실행
시켜서 얻어진 결과이다.

oe

PARR_of Chu_sequenc

Plot Fig. 7.12

N= 16; L=4; i = [0 : 1: N-1]'; k = 3; S = exp(j*k*pi/N*(i.*i));
[s, time] = IFFT_Ovs(S,N,1);

oe

_304



===== PAGE 303 =====
제7장_ㅁ46 감쇄 기법

[0001 08, avgP_dB, peakP_dB] = PAPR (s) ;
[09 8, OS time] = IFFT _Ovs(S,N,L); OS_s=OS_s*L;
[OS papr_dB, OS avgP_dB, 09 peakP_dB] = PAPR(OS_s);

ie) 프로그램 7.5 Chu A/HA| PAPR 분석 프로그램

0

그림 7.132 IEEE 802.166에서 사용되는 ani 때 앰블에 대하여 PAPR 특성을 보
여준다[119]. 프리앰블은 송ㆍ수신기에서 미리 알고 있는 시퀸스로서 자기상관, 상호상관,
PAPR 특성이 모두 우수한 AAAS 사용한다. 일반적으로 프리앰블은 데이터보다 높은
전력으로 송신되기 때문에 낮은 PAPR SAYS 프리앰블의 중요한 요건 중에 하나이다.
랜덤하게 생성되는 OFDM 신호는 PAPR 감쇄 기법으로 기저대역에서 7~8dB BEY
PAPRE 갖기 때문에, 미리 설계된 프리앰블의 경우에는 전력 FAQS 고려하여 이보다
낮은 PAPR EAS 필요로 한다. 그림 7.13은 프로그램 7.6(“#ㅅ# 0[ IEEEE802_16e_
preamble”) 실행시켜서 얻어진 결과로서, Nyquist 샘플링된 APs} 오버샘플링된 경
에 대하여 IEEE 802.166에서 사용되는 프리앰블의 PAPR 특성을 보여준다. 이 그림에 나
타난 바와 같이 IEEE 802.166에 주어진 프리앰블의 PAPRE 오버샘플링할 경우 최대
0.408 정도의 차이를 보인다. IEEE 802.16e 프리앰블은 기저대역에서 of 408의 낮은
PAPR 특성을 갖도록 설계된 시퀸스이기 때문에 오버샘플링에 따른 = 차이가 없지만,
일반적인 시퀸스의 경우에는 차이가 커질 수 있으므로 오버샘플링 후의 PAPRE 측정할
필요가 있다. 또한 본 장에서 이루어지는 PAPR 관련 모의실험은 모두 기저대역에서 이
루어지기 때문에 실제 RF 단에서의 840\과는 차이가 있음을 유의해야 한다. 일반적으로

ie

IEEE 802.16e Preamble, L=1.4

65         20 40 60 80 100 120
Preamble index [0~113]

그림 713 IEEE 802.166 프리앰블의 PAPR SA(L=1, 4)

305 _



===== PAGE 304 =====
PART Il_ OFDMZ} MATLAB

고출력 증폭기 입력단에서 신호의 PAPRE RF 단의 필터링 등을 통하여 기저대역에서의
24.08보다 증가하게 된다.

응 PARR_of IEEEE802 166 preamble.m

6 Plot Fig. 7.13

N = 1024; L = 4; Mo = 'BPSK'; N preamble = 114;

papr_nonOS = zeros(N_preamble,1); papr_OS = zeros(N_ preamble, 1) ;

for Pidx = 0 : N preamble-1
X=load(['.\\Wibro-Preamble\\Preamble_sym' num2str(Pidx) '.dat']);
X = X(:,1); X = sign(X); X = moveDC(X);
x_nonOS = IFFT _Ovs(X,N,1); papr_nonOS(Pidx+1) = PAPR(x_non0s) ;
x_OS = IFFT _Ovs(X,N,L); papr_OS(Pidx+1) = PAPR(x_0S) ;

end

fl 프로그램 7.6 IEEE 802.16e 프리앰블의 PARR 분석 프로그램

GEE rare 24 1H

PAPRS 감쇄시키기 위한 기법들은 크게 다음의 네 가지로 분류될 수 있으며, 본 절에
서는 이들 PAPR 감쇄 기법 중에서 많이 사용되는 기법에 대하여 설명한다.

첫 번째는 클리핑(010018)을 통하여 240#을 감소시키는 기법이다. 이 기법에서는
OFDM 신호를 피크0680 또는 그 주변에서 클리핑 또는 비선형적으로 ASS BABA
피크 크기를 감소시키는 간단한 방법이다. 이 경우 클리핑에 의하여 간단하게 피크 크기
감소할 수 있으나 송신 신호의 비선형 왜곡으로 인하여 대역 내ㆍ외에 간섭이 발생하
부반송파간 직교성이 파괴되는 문제점이 있다. 클리핑을 통한 PAPR 감쇄 기법으로
블록 스케일링 기법, 클리핑과 필터링 기법, 피크 윈도윙(668 windowing) 기법[168], 피
크 제거(068 cancellation) 기법, Fourier Projection 기법, Decision-Aided Reconstruction
기법 등이 있다.

두 번째는 부호화를 통한 PAPR 감쇄 기법이다. 이 기법은 전체 OFDM 심볼 중에서 일
부만이 큰 PAPRS 갖기 때문에 OFDMS] PAPR 특성을 이용하여 원하는 레벨 이하의

El 때 EL

[x

306



===== PAGE 305 =====
제7장_『ㅁ406 감쇄 기법

PAPRS 갖는 OFDM 심볼을 생성하는 부호화 기법이다. 이 기법은 클리핑에 의한 비선형
왜곡이 발생하지 않으나, 원하는 PAPR 레벨이 작아질수록 일반적으로 부호율이 낮아진다.
현재까지 부반송파수 NO] 작을 경우에 적합한 PAPR 감쇄 HSE 제안되었으나, No] 증
가할 경우에 체계적으로 부호화와 복호화를 할 수 있는 PAPR 감쇄 부호화 기법은 발견되
지 않았다 168][173]. PAPR 감쇄 부호로 Golay 상보 A)AA(complementary sequence),
Reed Muller 부호, M 시퀸스, Hadamard 부호 Go] 있다.

세 번째는 OFDM 심볼의 입력 시퀸스를 스크램블링(6608000108) AWA 스크램블링
하여 그 중에서 가장 작은 PAPRE 갖는 출력신호를 전송함으로써 높은 PAPRO| 발생할
SS 감소시키는 확률적(07008011500) 기법이다. 클리핑 기법과 PAPR 감쇄 부호 기법
은 OFDM 신호의 PAPR 값을 임계값보다 절대적으로 작게 하는 것이나, 확률적 기법은
PAPRO] 어떤 레벨 이하가 되도록 스크램블링하는 것이 아니라 높은 240의 신호가 발
생할 확률이 최소가 되도록 한다. 이 기법은 대역 밖으로 방출되는 전력이 존재하지 않는
장점이 있지만, 사용하는 부반송파 수에 따라 복잡도가 증가하고, 임의의 부반송파 수에
대하여 특정 레벨 이하의 PAPRS 보장해주지 못하며, 수신기에서 스크램블링 부호에 대
한 정보를 필요로 하기 때문에 주파수 효율을 감소시키는 단점이 있다. 스크램블링을 통
한 PAPR 감쇄 기법으로 스크램블링을 모든 부반송파에 적용하여 위상을 독립적으로 회
전시키는 SLM(Selective Mapping) 기법, 스크램블링을 부반송파 그룹별로 적용하여 위상
을 3S|AIA|7|= PTS(Partial Transmit Sequence) 기법이 있다[186]-[188]. 이 기법들은
PAPRE 감소시키기 위한 PAPR 감쇄 부호의 특수한 경우로 볼 수도 있다. 그러나 스크
램블링 AAS 상보 부호와는 달리 전방 오류 정정과 PAPR GAS 결합하지는 않는다.
위의 SLM 기법과 PTS 기법은 왜곡 없는 PAPR 감쇄 기법 중 이산 파라미터 최적화
(discrete parameter 00010128000)에 속하고, 연속 파라미터 최적화(6000104048 parameter
0001001280020)에는 TR(Tone Reservation) 기법과 11(1006 Injection) 기법이 있다.

네 번째는 송신기에서 IFFT 입력 신호를 DFT 확산하여 PAPRS 감소시키는 방법이
있다. 이 기법은 상향링크 ASA) 단말기에서 PAPRE 단일 반송파 수준으로 감소시킬 수
있어 3GPP LTE2] 상향링크 전송 표준으로 채택되었으며 SC-FDMA(Single Carrier—
1244 )라고 불리운다. 이 외의 PAPR 감쇄 7|'4}° = Pre-distortion 기법[174], Compression
and Expanding 기법 등이 있다.

307


===== PAGE 306 =====
PART 1 _ OFDM2} MATLAB

클리펑과 필터링 기법

|= |

PAPRS 감소시키는 가장 간단한 방법은 송신 신호의 최대크기를 특정 레벨 이하로 4
한시키는 신호의 클리핑이다. 클리핑 기법은 여러 PAPR 감쇄 기법 중에 가장 간단한 빙
법이지만 몇 가지 단점이 있다. A 번째는, 클리핑을 함으로써 OFDM 신호의 크기를 왜곡
시키게 되어 대역내02-6800)에서 일종의 자기 간섭이 발생되어 BER 성능이 저하된다. 두
번째는, 신호의 클리핑은 비선형 왜곡에 해당하므로 대역외(01[-0[-60800) 잡음 형태로
스펙트럼 방출이 증가한다는 것이다. 클리핑에 의한 대역외 잡음은 필터링에 의하여 감소
시킬 수 있으나 클리핑이 이산시간 영역에서 이루어질 경우 클리핑에 의하여 발생하는 고
주파수 성분의 대역외 잡음이 대역내에 간섭을 미치게 된다. 즉, Nyquist 샘플링된 디지
ASS 클리평하게 되면 대역 밖으로 방출된 스펙트럼의 전력이 대역 내로 중첩되는 현상
(aliasing) 야기하여 성능 열화를 발생시킨다. 이 경우 4배 이상의 오버샘플링된 신호에
대해서 이산시간에서 클리핑을 수행하게 되면 대역간 간섭으로 인한 BER 성능의 열화를
극복할 수 있다[169]. 또한, 클리핑은 기저대역 또는 통과대역에서 수행될 수 있는데, 기
저대역에서 수행되는 클리핑 기법은 58#에서 성능 열화가 발생하며, 통과대역에서 수행
되는 클리핑 기법은 스펙트럼을 더욱 퍼지게 한다. 오버샘플링된 OFDM 신호가 저역 통
과 필터를 통과하기 이전에 이산시간 영역에서 클리핑되고 통과대역에서 대역 통과 필터
를 통과하게 된다면 성능 열화는 경감된다. 세 번째는, 대역외로 Yes 스펙트럼을 필터
}게 되면 대역내에서 스펙트럼 리플이 발생하고, 클리핑되었던 피크 ge] 일부가 다시
가하는 현상이 발생한다. 결국, 이와 같은 신호의 비선형적인 왜곡은 BER 성능의 열화
야기하나, 대부분의 OFDM 시스템에서는 채널 부호화를 사용하고 있어 클리핑과 필터
에 의한 성능 열화는 어느 정도 보상된다. 클리핑과 필터링 기법은 더 비교적
단한 조작만으로 PAPRS 감소시킬 수 있고 수신기에서 BRE 하는 추가적인 정보가
문에 주파수 효율이 감소하지 않는 기법이다. 그림 7.14는 클리평과 필터링을 이용
PAPR 감쇄 기법의 블록도를 보여준다.

ru

어

(인 로 2 08 의 oft

X'[m                        X? 1720]                  xe [m]                 X? {k]                 x? [시                xP [m]

시          ㄴ…시         _
Clipping HK} point [| BPE >! point | LPF [> x(t)
FFT          IFFT

tneneenenenoacenseasceeeaerversecevsnensecnserssssseneensesresses Transmitter cccsssssssssseeeseeeseeeeeee                   이아

그림 7.14 클리핑과 필터링 기법의 블록도

Mon


===== PAGE 307 =====
제7장_ㅁ46 감쇄 기법

여기서 Le 오버샘플링 비율을 나타내고, NS 부반송파 수를 나타낸다. 입력 신호
제[서는 식 (7.16)에서와 같이  -1)개의 zero padding? 2 구성된다. 』배 오버샘플
링된 이산시간 영역 신호 xm] = 중심 주파수 /로 변조되어 통과대역에서 x’ [m] zB
표현된다. 이 ASS 클리핑한 신호 x?[m]& Sa} 같이 주어된다.

-4      x’[m]<-A
x? [m]=4x?[m] |x?[m]] <4, 4 >0                   (7.19)
A        x’ [m]> A

이 때, 정규화된 클리핑 레벨 CR(Clipping Ratio)? 다음과 같이 정의된다.

CR=Alo                                         (7.20)

여기서, ㅇ 는 OFDM 신호의 mms 값을 나타낸다. 일반적으로 기저대역에서 o=VN,
통과대역에서 c=VN/22 유도된다. in 들어, CR=1.4% ㅇ보다 308 높은 레벨에

서 클리핑하는 것을 의미한다. 여기서는 주파수 영역에서 대역 통과 필터링을 하였다.
라지막으로 저역 $a} HHS Saket 연쑥시간 Ga 신호 HNL Dae Serie 일
력된다.

클리핑과 필터링에 의한 PAPR 감쇄 기법의 성능을 확인하기 위해서는 다음과 같은 세
가지의 지표를 확인해야 한다[175]. A 번째는, 대역내에서의 리플과 대역외로 방출되는
전력을 전력 ABE A(Power Spectral Density)& 사용하여 확인한다. 두 번째는, CF 또는
ㅁ?ㅅ0#의 분포를 CCDFS 사용하여 확인한다. 세 번째는, 클리핑과 필터링 기법으로 왜곡

신호가 성능에 미치는 VES BERS 사용하여 확인한다. 이 때, 부호화가 적용되지 않

경우와 부호화가 적용된 경우의 BER 성능을 모두 확인한다.

표 7.1은 클리핑과 필터링 기법의 성능을 살펴보기 위하여 모의실험에 사용된 파라미터
예를 보여준다. 주어진 대역폭과 샘플링 주파수를 고려하여 /=8로 설정하였고, 반송파
주파수 /. =2Mhz, 부반송파 수 N=128 을 사용하였다. QPSK 변조된 OFDM 신호에
대하여 약 1.608부터 408까지 변화하며 클리핑하였다.

버   뽀



===== PAGE 308 =====
PART 1 _ 야미/과 MATLAB

표 7.1 클리핑과 필터링 기법의 모의실험에 사용된 파라미터

Bandwidth, BW                 1MHz
Sampling frequency, f, = BW: L              8 MHz
Carrier frequency, f.                   2 MHz
FFT size, V                      128
Number of guard samples (CP)                 32
Modulation order                       QPSK
CR                 0800 12014 0186

그림 7.15는 모의실험에 사용된 equiripple 통과 대역 필터의 시간영역의 임펄스 응답과
주파수 영역의 전력 스펙트럼을 보여준다. 이 그림에 나타난 바와 같이 f= 8MHz, 첫
번째 비통과대역($006800) Zz} 통과대역(08596800) 시작은 각각 1.4\4[2와 1.5MHz, 두
번째 통과대역 끝과 비통과대역 시작은 각각 2.584[와 2.6MHz, 비통과대역 감쇄는 약
40dB°] 되도록 104개의 YS 사용하였다.

-ㅜ

0.2F

은

coefficient value

10 20. 20 40 50 ^ 60 70 80 90 100                거스 가2 금
                                                                                frequency (Hz)                          x 10°
(a) 필터 계수                       06) 주파수 영역 특성

그림 7.15 Equiripple 통과대역 FIR 필터의 예

그림 7.16은 프로그램 7.7(“PDF_of 010060 300 filtered 07124 918001')을 실행시켜서
얻어진 것으로서, 표 7.1의 파라미터를 가지고 클리핑과 필터링을 적용한 결과를 보여준다.
그림 7.14()는 오버샘플링된 기저대역 신호 [^], 그림 7.1406)는 통과대역 신호 x’ [nm],
그림 7.14(0)는 클리핑된 신호 7 [nm], 그림 7.14(0)는 필터링된 신호 Ulm) o] 확률밀도
함수와 전력 스펙트럼을 차례로 보여준다. 이 그림으로부터 OFDM 신호의 확률밀도함수
는 클리핑 전에는 Gaussian HES 취하지만, 클리핑 후에는 클리핑 레벨 이하에만 신호
가 존재하고, 필터링 후에는 클리핑 레벨 밖에 나타나는 신호의 피크 값이 다시 증가하는
확인할 수 있다. 또한, OFDM 신호의 전력 스펙트럼은 클리핑 이후에 대역외 Awe

가하지만, 필터링 이후에는 대역외 스펙트럼이 다시 감소한다는 것을 알 수 있다.

tho
ofN les

0

oe oy
Oj

은



===== PAGE 309 =====
Baseband signal, with CP

AI72t_ PAPR 감쇄

Unclipped passband signal

0.01 0.02

“9.03 -0.02 -0. 2

0
-0.04

04 06 08   1    12                                0.03 0.04
time (nomalized by symbol duration)                                                                           x
a 해여 ：| 0]:     a 매여
g                                                                           더                                                           ‘vom
2 —— 0 ee   3 sme       ied
8                                                                            g
103 4    고
frequéncy (Hz)                      x 10°                                       frequency (Hz)                      x 10°
_                           b) 통고     시호 x’|m|o  확률밀도호 스
전력 스펙트럼
02                   Clipped passband signal, CR=1.2                                           Passband signal after clipping and filtering, CR=1.2
0.15
을 01
0.05|

0
-0.015

-0.01

-0.005     0      0.005     ).)1     0.015

1      2      3

1             0
frequency (Hz)                      x 10°

(0) 클리핑된 신호 v(m] 9] 확률밀도함수와
전력스펙트럼

그림 7.16 클리핑과 필터링 기법

적용시 OFDM

0            1
frequency (Hz)                              x 10°

(0) 필터링된 신호 x [mo] 확률밀도함수와
Se
신호의 확률밀도

424

전력

fe} 전력 스펙트럼 (아=1.2)

응 PDF_of clipped_and_filtered_OFDM signal.m

% Plot Fig. 7.16

CR=1.2; ¢ 4 (7.21), dB scale = 20*1log10 (CR)

bits=2;N=128 ; Ncp=32; fs=1le6 ; L=8;Tsym=1/ (fs/N) ;Ts=1/ (£s*L) ; £c=2e6;
time=[0 : Ts :2*Tsym-Ts]; freq=[0 : fs/(N*2): L*fs-fs/(N*2)]-L*fs/2;
Hd = eugiripple filter fin; Fcoeff = Hd.numerator; Lcoeff =

length(Fcoeff); %

[Xi, Xq, Mo]

= mapper(bits, N, 'Y');

equiripple bandpass filter

Xi(1) = 0; Xq(1)   0;

311



===== PAGE 310 =====
PART ㅁㅁ OFDMZ} MATLAB

x_b=IFFT_Ovs (Xi+}*Xq,N,L) ;

x_b cp=addcp(x_b,Ncp*L) ;

x_b_cp=[zeros (1, (N/2-Ncp)*L), x_b cp, zeros(1,N*L/2)]; toversampling
x _p = upconv_fin(fc,x_b cp,time/Tsym*2) ;

※ 0 ¢ = Cclipping(CR,x p); % 4 (7.22)

X_p_c_f = filtering(Fcoeff,x ㅁ c);

0 0ㄴㅁㄴㅋ16ㄷ(제 p ¢ £);

x_b_c_t = dwconv_fin(fc,x_p_c_ t,time/Tsym*2) ;
mM pet 7.7 클리핑과 필터링 기법 적용시 확률밀도함수와 전력 스펙트럼 분석 프로그램

그림 7.17(8)는 클리핑과 필터링 기법이 적용된 OFDM 신호의 CF(Crest Factor) 2]
CCDFS 보여주는데, CFE 848#과 제곱근 관계에 있기 때문에 (개의 CCDFS PAPR
BEE 해석할 수 있다. 이를 BAS   _  적용하지 않은 원 신호의 PAPRO| 가장 크지
만, 클리핑을 하고 나면 PAPRO| 크게 감소하고, 클리핑과 필터링이 적용되면 240이 다
시 증가함을 알 수 있다. 이 때 0# 값이 작을 수록 PAPR] 낮아짐을 알 수 있다. 그림
7.1706)는 클리핑과 필터링 기법 적용시 BER Ves 보여주는데, 여기서 ‘Ce 클리핑된
ASS, CAPE 클리핑과 필터링이 적용된 신호를 나타낸다. 이 그림으로부터 해석적
(analytic) 결과와 클리핑 Al(unclipped) 신호의 BER 성능은 SUSU, 클리핑된 ASE

CRo| aotael 파라 ise] SAH 알수 있다. 이 aes 주어져 있지 않지만 부호
화기를 적용할 경우에 BER 성능 SSS 어느 정도 극복할 수 있기 때문에 클리핑과 필터
링 기법은 240 감쇄 기법으로 종종 사용된다.

오는

CCDF Suna CR=0.8, 1.0, 1.2, 1.4, 1.6                                Uncoded BER

10°                                                 10° 는

=     00010000
-|—8— clip.
-            90009 & fthering

Analytic
|| —— Unclipped

010개

CCDF F,(Z,)
ㅎ
으
?
>

10°

45 6
Z,(B)                                  EbNo(dB)
(a) PAPR 분포                            (6) BER 성능

그림 7.17 클리핑과 필터링 기법 적용시 PAPR 분포와 BER 성능

312



===== PAGE 311 =====
제7장_『ㅁ466 감쇄 기법

다음 프로그램 7.8(“CCDF_of _clipped_filtered OFDM-signal”)2 그림 7.17을 그리는
데 사용되었다.

% CCDF_of 0110060 filtered OFDM signal.m
% Plot Fig..7.17
SNR = [0 : 1: 10]; % dB
Nblk = 1e4; CR = [0.8 : 0.2: 1.6];
bits = 2; N= 128; Nep = 0; fs = 166; L = 8;
Tsym = 1/(fs/N); Ts = 1/(fs*L); fc = 2e6;
time = [0 : Ts :2*Tsym-Ts] ;
Hd = eugiripple filter fin; Fcoeff = Hd.numerator; Lcoeff =
length (Fcoeff) ;
M = 2*bits;      % alphabet size
if (bits) == 1)   Mo = 'BPSK';
elseif (bits == 2)   Mo = 'QPSK';
else   Mo = [num2str(M) 'QAM']; end
const = gammod([0:M-1] ,M);         % QAM modulation
Mscale = modnorm(const, 'avpow',1); % normalization factor
mdmod = modem.gammod('M', M, 'SymbolOrder', 'Gray','InputType', 'Bit');
mddem = modem.gamdemod('M', M, 'SymbolOrder', 'Gray','OutputType',
'Bit', 'DecisionType','hard decision') ;

Clipped_errCnt = zeros(size(CR));
ClippedFiltered_errCnt = zeros(size(CR)) ;
$ ------------- Iteration with increasing SNR --------------------%
ber = berawgn ([SNR(1) :SNR(end) ] -10*log10 (bits) ,'qam',M) ;
for SNRIdx = 1 : length(SNR)

Unclipped_errCnt = 0;

Clipped _errCnt(:,:) = 0;   ClippedFiltered errCnt(:,:) = 0;

for blk = 1 : Nblk(SNRIdx)

Tx_Xbin = ceil(0.5-rand(bits,N)); % binary squences

Tx_Xig = Mscale * modulate(mdmod, Tx Xbin); % mapper
Tx _Xiq(1) = 0+j*0;   * DC sub-carrier not used

x_b = IFFT _Ovs(Tx_Xiq,N,L)j;

x_b_cp = addcp(x_b,Ncp*L) ;

x_b_cp = [zeros(1, (N/2-Ncp)*L), x_b cp, zeros(1,N*L/2)];
x _p = upconv_fin(fc,x_b cp,time/Tsym*2) ;

313


===== PAGE 312 =====
PART Ｌ_ 야미/과 MATLAB

y_p_n= [x_p(1:(N/2-Nep)*L) awgn(x_p((N/2-Ncp) *L+1: (N/2-Ncp)
*L+(N+Nep)*L),SNR(SNRIdx), 'measured')
x _p((N/2-Nep) *L+ (N+Ncp) *L+1:end) ] ;   % add Noise (AWGN)
y_b_uc_t_W = dwconv_fin(fc,y_p_n,time/Tsym*2) ;
Y_b uc £ W= fft(y_b uc t W);
y_b uct T= ifft([Y_b uc_f W(1:N*L/2), zeros(1,2*N*L-N*L),
Y_b uc _f W(end-N*L/2+1:end)]) ;
y_buct L=y_b uc t T((N/2-Ncp) *L+1: (N/2-Ncp) *L+(N+Nep) *L) ;
y_bluc t = y b uc _t_L(i:leend);
Y_b_uc f = fft(y_b uc_t(Ncp+1:end) ,N)*L;
Y_b_uc_bin = demodulate(mddem, Y_b uc f);
errCnt = biterr(Tx_Xbin(:,2:end),Y_b uc bin(:,2:end));
Unclipped_errCnt = Unclipped_errCnt + errCnt;
for cr = 1 : length(CR)
x _p_c = clipping(CR(cr),x_p);   6 clipping
y_peones= [xp c(1:(N/2-Ncp)*L) awgn(x_p_c((N/2-Ncp) *L+1:
(N/2-Ncp) *L+(N+Ncp) *L),SNR(SNRIdx),'measured')
x _p_c((N/2-Ncp) *L+(N+Ncp)*L+1:end)]; % add Noise (AWGN)
y_b_c t_W = dwconv_fin(fc, y p_ cn, time/Tsym*2) ;
YbcfWe=fft(y bct W);
ybectT = ifft([Y_b c £ W(1:N*L/2), zeros(1,2*N*L-N*L) ,
Y_b c f W(end-N*L/2+1:end)]) ;
ybctLbL=y bc t T((N/2-Nep) *L+1: (N/2-Nep) *L+(N+Ncp) *L) ;
ybet=ybct _L(1:bL:end);
Y_becf = fft(y_b c t(Ncp+l:end) ,N)*L;
Y_b_c bin = demodulate(mddem, Y_b c f);
errCnt     =     biterr (Tx Xbin(:;,2send) , 1 ㅁㄷ c¢ bin(:,2end));
Clipped_errCnt (cr) = Clipped_errCnt (cr) + errCnt;
X_p cf = filtering(Fcoeff,x_p_c);
Xp cl. = 1fFt(x pct);

y_pcfn = [x_p cf(1:(N/2-Ncp)*L) awgn(x_p_cf((N/2-Nep) *L+1:
(N/2-Ncp) *L+(N+Ncp) *L),SNR(SNRIdx),'measured')
x_p_cf ((N/2-Ncp) *L+(N+Ncp) *L+1:end)]; %add Noise (AWGN)

y_b cf t_W = dwconv fin(fc, 7 p cf_n, time/Tsym*2) ;

Ybcf £ W= fft(y_ b cf t_W);

y_b cf t_ T= ifft([Y_b cf 7 W(1:N*L/2), zeros(1,2*N*L-N*L),
Y_b cf f W(end-N*L/2+1:end) ] ) ;

m = ceil (Lcoeff£/2) ;

314



===== PAGE 313 =====
제7장_ㅁ466 감쇄 기법

ybcf t L=y_b cf t_T((N/2-Nep) *L+m: (N/2-Ncp) *L+ (N+Ncp) *L+m-1) ;
y_b cf t= y b cf t _L(1:L:end);

Y_b cf _f = fft(y_b cf _t (Ncpt+l:end) ,N) *L;

Y_b cf bin = demodulate(mddem, Y_b cf f);

errCnt = biterr(Tx_Xbin(:,2:end),Y_b cf bin(:,2:end));
ClippedFiltered_errCnt (cr) =ClippedFiltered_errCnt (cr) +errCnt;

end
end
Unclipped_ber(1,SNRIdx) = Unclipped_ i igprasity (SNRIdx) / (N-1) /bits;
Clipped_ber(:,SNRIdx) = Clipped_errCnt (:,:) /Nb1lk (SNRIdx) ale (N-1) /bits;
ClippedFiltered_ ber(:,SNRIdx) = ClippedFiltered . errCnt (:,:) /Nblk

(SNRIdx) / (N-1) /bits;
end

W 프로그램 7.8 클리핑과 필터링 기법 ASA PAPR 분석 프로그램

 PAPR 감쇄 부호

전체 OFDM 심볼 중에서 일부만이 큰 PAPRS 갖는 OFDM 신호의 특성을 이용하는
호화 기법을 사용하여 PAPRE 감소시킬 수 있다. 즉, 어떤 원하는 레벨 이하의 PAPR
[는 OFDM 심볼만을 생성하는 부호를 사용함으로써 PAPRE 감소시킨다. 물론, 원하
APR 레벨이 작아질수록 얻을 수 있는 부호율은 낮아진다. 참고문헌 [176]에서는 8개
반송파를 갖는 경우 최대 308의 PAPRE 제공하는 3/4 부호율의 부호가 존재함을
참고문헌 [176]에서는 모든 가능한(006) 부호에 대한 막대한 탐색 과정을 통해
구하는데, 불행히도 이 결과는 단지 많은 코드워드6006\010)가 존재한다는 것만
Lali sabia 생성하기 위한 부호화와 복호화에 대한 체계적인 방법의 존
이 부호가 갖는 최대 거리 성질에 관한 USS 제시하지 않았다. 그러나, 이 문헌
에서는 막대한 탐색 과정을 통해 구한 대부분의 부호가 Golay 상보 시퀸스라는 사실을 언
급하였는데, PAPR 감쇄 BSS 생성하는 체계적인 방법을 찾을 수 있는 AS 제시하였
다. Golay 상보 AJAAE 0이 아닌 모든 지연 이동(0613 shift)o] 대해 두 ABZ 사이의
자기상관 함수의 So] 0인 한 쌍의 시퀸스이다[177]. 문헌 [178]에서는 이 부호를 OFDM
신호의 변조에 사용하면 상보 시퀸스의 상관관계 성질로 인하여 PAPRY 308의 작은 값

노새

fe)

Ht 12 rr ilo rs
dr

x2
uu 무

으로 낮출 수 있다고 하였다. LS [179] HAE Golay 시퀸스에 대한 이와 같은 SYS
근거로 하여 0018》 부호의 특정 부집합을 설명하고, PAPR 감소와 전방 오류 정정 능력을
315


===== PAGE 314 =====
PART 1 _ OFDMa} MATLAB

결합한 복호 기법을 제시하였다. Golay AAAS] 성질에 대한 기초적인 연구는 문헌
[180]-[182]에서 찾아볼 수 있는데, 이들 문헌에서는 부호 집합의 크기, 거리 성질,
Reed-Muller 부호에 대한 관계와 많은 세부 사항들을 입증하였다.

음은 상보 A|2(complementary 96046006)의 기본적인 성질을 설명한다. 길이 의
ABA xn] + x[n]°] 다음과 같은 자기상관 함수의 합에 대한 조

Mn] x[n]o] 상보적이라고 할 수 있다.

2 Cae ot eee iI =o                 (7.23)

=0 ,i#0
4} (7.23)의 양변에 Fourier 변환을 적용하면 위의 AUS 다음과 같이 변형된다.

[X[k]? +|X, [x]? =2N                               (7.24)

여기서, [XT 는 x[n] 9] 전력 스펙트럼(081)으로 자기상관 B22] Fourier 변환이
다. 이산 Fourier 변환 X[k] = 다음과 같이 정의된다.

N-1
X[k] = > 지16                                               (7.25)
n=0

여기서, 2; 는 AAA xn] 2] 샘플링 주기이다. 전력 스펙트럼의 최대값은 Al (7.24)에
주어진 스펙트럼 조건에 의해 27/으로 제한된다.

4140.                                            (7.26)

ABA [의 전력이 1이라고 가정하면 식 (7.25)의 평균 전력은 NIE 같기 때문에
X[k] 의 PAPRE 다음과 같이 제한된다.

PAP ratio < = =2 (308)                                          (7.27)

_ 316



===== PAGE 315 =====
제7장_『ㄷ46 감쇄 기법

일반적으로, OFDM 시스템에서 A) AAE IFFTH 입력된다. 그러나 IFFTE FFT 출력
에 SY BALE 취하고 1/#로 크기를 조정하는 것과 같기 때문에, ATS 시퀸스 af]
의 역 Fourier 변환으로 대체한다면 PAPRE 상한값 2로 제한된다. 따라서, 상보 부호를
OFDM ASS 생성하기 위한 입력으로 사용하면 PAPRo| 308를 초과하지 않게 된다. 그
림 7.18은 부호화하지 않은 OFDM 신호와 상보 Boe 변조된 16 부채널 OFDM 신호
크기의 예를 보여준다. 16 부채널 사용시 PAPRE 부호화하지 않은 경우와 비교하여 약
908 감소한다. 여기서 모든 부반송파는 동일한 초기 위상으로 변조하였다.

55
2타
VPAP 2P

1L.5F

0.5F

8. 10 12 14 16      70.24.68 10 12146
Time/T                                  Time/T
(8) 부호화하지 않은 경우의 PAPR            。 06) 상보 코드로 변조된 경우의 PAPR

그림 7.18 상보 Soe 변조된 OFDM 신호의 PAPR

0   2   4   6

부호 집합을 생성하는 방법 중에서 Reed Muller OS 이용한 방법[180]-[182]은 2차
Reed Muller 부호의 1차 지수가 Golay 상보 부호의 EAS 가지므로 상보 AAAS 쉽게
생성할 수 있고 높은 부호율에서도 부호화와 복호화가 간단하다. 전술한 바와 같이 Golay
상보 시퀸스는 항상 PAPRO] 308 이하이다. M A]34A(Maximum-—length 56046006)를 이
용한 YAS m 이 3~10의 값일 때 PAPRO| 5.4~7.3008이고, 부호 길이의 절반 이상의 최
소 AY 거리를 가진다. 여기서 OFDM 심볼의 길이 NS 2"-1이다. 또한 부호화와 복
호화 과정이 매우 간단하고 큰 LUT(Look—Up Table)S 사용하는 것을 피할 수 있다
[183][184]. Hadamard 변환을 이용한 방법은 전력 증가와 부가 정보의 전송없이 oF 208
의 PAPR 감소 성능을 얻을 수 있다. 또한 시스템 복잡도가 증가하지 않고 구현도 용이하
다[185].

317



===== PAGE 316 =====
PART Il1_ OFDM2} MATLAB

“mess Selective Mapping 기법

SLM(Selective Mapping) 기법은 먼저 입력 심볼 시퀸스를 미리 정해진 여러 개의 위
상 AAAS 곱해서 다른 심볼 시퀸스들을 생성한다. 그 후 심볼 ABASS IFFT 하여
OFDM 신호 So 각각의 PAPR 값을 계산하여 가장 작은 PAPR 값을 갖는 OFDM
ASS 선택하여 전송하고 위상 AAAS) 인덱스를 부가 정보(6106 information)= 송신한
다. 그림 7.19는 SLM 기법의 블록도를 보여준다.

=
N-point | x°
Oo   타 |
P=1,              ~
4         ‘             the
Serial        X.| Nepoint |포| ofpm |x
Input Data >} to Xs  S     IFFT [| signal with [7
Parallel     P'      .          the
minimum
2 | 때
—poin
rey 、
po                                 | 가 Necessary:

iaguepeyoaeea sous ane

그림 7.19 Selective Mapping 기법의 블록도

SLM 기법에서는 먼저 입력 심볼 AlBA ※=|지이,시],…,^[^&-1]]와 (개의 위상
ABA PY =[PUP Py, 것 =00, gt e[0,22), OSv<N, lSusUS 곱해서
AGA ※=[4"[0.4"[2].…,4"[4 -1]]" , lsusUs 생성한다. 이 때, ※"는 동일한

를 전송하는 U 개의 독립적인 OFDM 심볼이다. 서로 다른 U 개의 심볼 ALBA x"
IFFTapo} x" =[x"[0] x"UxIN-Il] 를 생성한 후, 생성된 꼬중에서 가장 작은
PAPRE 갖는 심볼 K=x" S 선택하여 전송한다. 여기서 WE 가장 작은 PAPR ZS 갖
는 시퀸스를 생성하기 위해서 사용한 위상 시퀸스의 인덱스를 나타내며 다음과 같이 표현
된다.

ox,

mun

u = arg min( max |x "[2])                             (7.28)

O<usU =: OS SN

수신단에서는 위상 ABAS 곱하여 전송된 신호를 원 ASK 되돌리기 위해서 어떤 위
상 시퀸스 벡터 #*가 송신단에서 사용되었는지 알아야 한다. 이를 위해 가장 간단한 방법
은 부가 정보로서 수신단에 위상 시퀸스의 인덱스 # 를 전송하는 것이다. SLM 기법을 구

318


===== PAGE 317 =====
제7장_『ㅁ4066 감쇄 기법

현하기 위해서는 각 데이터 블록마다 vo] 위상 시퀸스가 곱해지므로 (/개의

14 연

산이 필요하고, 각 hii 블록마다 요구되는 부가 정보의 비트 수 [log,U] 9] 전송이 필
요하다. 여기서 LO) 는 US 넘어서지 않는 가장 작은 정수를 의미한다. 이 부가 정보는
매우 중요하기 ae 에러 발생 시 이를 검출하고 보정하기 위해서 채널 부호화가 필요
하다. SLM 기법의 성능은 위상 AMA) 개수 《/와 위상 시퀸스를 어떻게 설계하는지에
따라 크게 달라지고[189], SLM 기법에 이용되는 위상 시퀸스로는 랜덤 시퀸스, Walsh 시

HA, Golay 시퀸스 등이 있다.

“PPG Partial Transmit Sequence 기법

전 절에서 설명한 SLM 기법에서는 스크램블링을 BE 부반송파에 적용하여 위상을 독
립적으로 회전시키는 반면, PTS(Partial Transmit Sequence) 기법에서는 스크램블링을 부
반송파 그룹별로 적용하여 위상을 회전시킴으로써 구현 복잡도를 감소시킨다[187]. PTS
기법은 먼저 입력 심볼 시퀸스를 서로 결지지 않  않는 입력 심볼 부블록으로 분할하고 각각
의 입력 심볼 부블록을 FFT 한 후 위상 벡터들과 곱하여 더한다. 이 때 위상 벡터를 변
경하면서 가장 낮은 PAPR WS 갖게 하는 최적의 위상 벡터를 선택하고 이에 해당하는
위상 벡터 인덱스를 부가 정보로 수신단에 전송한다. 그림 7.20은 PTS 기법의 블록도를
나타낸다.

x'   N-  ' i  x!           ae
a Oe
Serial             +
Paral LX° [N-point  a  @
%        를
|      ~      a                      .
nput Data    p aon      \FFT             … 5X
into               82
Subblock      '
LX} N-point 보보

IFFT

bi 4           대 제드
으으         _ 1 Necessary:
Optimization     Side information

그림 7.20 Partial Transmit Sequence 기법의 블록도

3219



===== PAGE 318 =====
PART IL_ 야미/과 MATLAB

PIS 기법에서는 우선 한 블록으로 구성된 입력 벡터를 서로 겹치지 않는 부블록 벡터
로 다음과 같이 분할한다.

< 여인 을                                         (7.29)

즉, 입력 데이터 블록 XS 겹치지 않게 분할된 개의 BES ※",ㅠ=1.2,…,/ 로 나
눈다. 여기에서는 표현을 간단하게 하기 위하여 부블록은 인접하여 있고 동일한 크기를
【는다고 가정한다. 위와 같이 나뉘어진 부블록에 위상 회전을 나타내는 가중치
{0 Se v=,2,--, Vi 를 22

R

따

한 후 IFFTS 한 신호 xt 다음과 같이 주어진다.

x= iFeT| 36 x} =e IFFT(X}=> 6" x”                (7.30)

v=l                            =]                                         v=l

<

여기서 ※"의 IFFT] x” S Partial Transmit 56046006라고 부른다.
위상 회전 백터는 x 2] PAPRO| 최소가 되도록 선택한다. 이 때, 위상 회전 가중치는
다음과 같이 주어진다.

>" 12000

v=l

[b',...5” ]= arg min( max
[o!,.-,b”] OSnsN

)                          (7.31)

여기서 argmin(-)2& 송신 데이터 AS 최적화한 최대 전력에 대한 전역적 최소값
(global minimum) 의미한다. 최적의 위상 회전 가중치가 곱해져서 가장 낮은 PAPRE
갖는 심볼은 다음과 같이 표현된다.

i=) 0" 고                                        (7.32)
1

PTS 기법에서는 허용된 위상 회전 가중치의 집합이 d= fe?" [i= 01-7 -H A 때
최적의 위상 회전 가중치의 집합을 찾기 위해서 총 번의 연산이 필요하다. HBS V
의 값이 증가하면 최적의 위상 회전 가중치의 집합을 찾기 위한 계산량은 기하급수적으로
증가한다.

 320



===== PAGE 319 =====
제7장_『ㅁ406 감쇄 기법

가 필요하다. PAPR 감소 성능은 부블록의 개수 「와 허용된 위상 회전 가중치의 개수
Wo] 따라 영향을 받을 뿐 아니라 부블록 분배 방법에 의해서도 영향을 받는다. 부블록
분배 방법에는 인접(2400120600, 인터리브(106646860), 의사 랜덤(6896400-730ㅁ0000) 분배 방
법이 있다. 이 중에 의사 We(pseudo-random) 분배 방법이 가장 좋은 성능을 갖는 것으
로 알려져 있다[190]. PTS 기법은 부반송파의 수와 변조 Bol] 상관없이 적용된다.

전술한 바와 같이 PTS 기법은 부블록의 수가 증가할 때마다 최적의 위상 회전 가중치
의 집합을 찾기 위한 계산량이 기하급수적으로 증가하기 때문에, 이 계산량을 줄이기 위
해서 여러 가지 기법이 제안되었다[191][1921. 참고문헌 [191]에서 제안된 이진 가중치만
을 사용하는 준 최적 조합 알고리즘을 요약하면 다음과 같다.

© 위상 회전 가중치를 {1, -1}로 제한한다.

(3) 입력 데이터 블록을 개의 부블록으로 나누고, 「개의 부블록의 위상 회전 가중치
b=[b',b’,..,b°]S 모두 1로 설정하여 244 을 계산한다.

(3) 두 번째 위상 회전 가중치를 변화하여, 즉 ^ =-1 B 바꾼 후 다시 PAPR' 를 계산한다.

@ 만일 PAPR> PAPR'°|A /^=ㄱ1로 유지하고 아니면 BF? =1로 설정한다.

© 위의 과정을 7=1,2,‥,,/ 에 대해서 수행하여 최적의 위상 회전 가중치를 구한다.

PTS 기법에서 허용된 위상 회전 가중치의 개수가 Weta 할 때 최적의 위상 회전
가중치를 구하려면 W's) 계산량이 필요하지만, 위의 준 최적 조합 알고리즘을 사용하게
되면 성능은 다소 저하되지만 계산량은 ㅣ번으로 줄어든다.

그림 7.212 PTS 기법 사용시 부블록 수의 변화에 따른 240 성능을 보여주는데, 이
로부터 부블록의 개수가 증가함에 따라 PAPR 감소 성능이 WIS 일
MATLAB #7134 7.11(‘“‘compare PTS CCDF”)& 사용한 모의실험으로부터 얻어진 결
과이다. 각 부반송파는 16-044으로 변조되었고, 송신신호는 4배 오버샘플링 되었으며,
50.000개의 랜덤 OFDM 심볼이 이용되었다. 부블록의 개수 가 1, 2, 4, 8, 16개로 변함
에 따라 한 부블록당 부반송파의 개수는 256, 128, 64, 32, 16개로 주어진다. 또한, PT
위상회전 가중치는 프로그램 7.10의 phase factor optimization 부에 의해 위의 준 최적 조
합 알고리즘으로 결정된다.

에

Nn

Bp
Al
적

321

ria



===== PAGE 320 =====
PART ㅁㅁ OFDMZ} MATLAB

CCDF of PAPR (N=256, 16QAM)

=

PR(PAPR>PAPR,)

o
>

109………—a x!
PAPR,[dB]
그림 7.21 PTS 기법에서 부블록 수의 변화에 따른 PAPR 성능

4

function pr=ofdma_papr(N,OS,mod_order,dB_s,dB 1,08 e,MaxIter)

%N        : FFT size(# of total subcarriers)

% OS       : oversampling ratio

% mod_order : 4-> 4QAM, 16 ->16QAM, else -> 64 QAM
% MaxIter : number of iterations

M = N*OS;

bps = log2(mod_order) ;
088 = dB_s:dB i:dB 6; dBcs = dBs+dB i/2;
for iter=1:MaxIter
tx_bits=floor(rand(1,N*bps) *2) ;
mod_sym=QAM mod(tx_bits,bps) ;
[Nr,Nc] =size (mod_sym) ;
zero _pad_sym=zeros (Nr,Nc*OS) ;
for k=1:Nr
zero _pad_sym(k,1:0S:Nc*OS) =mod_sym(k, :) ;
end
ifft_sym=ifft (zero _pad_sym,M) ;
sym _pow=abs (ifft_sym) .*2;
mean_pow (iter) =mean(sym_pow) ; max_pow(iter) =max(sym_pow) ;
end

322



===== PAGE 321 =====
제7장_『40ㅁ 감쇄 기법

PAPR=max pow./mean_pow; PAPR dB=10*1log10(PAPR) ;
count = 0; N_bins = hist (PAPR_dB,dBcs) ;
for i=length(dBs) :-1:1

count = count+N bins(i); pr(i) = count/MaxIter;

end

j@ 프로그램 7.9 OFDM 신호의 PAPR 측정 함수

function pr=PTS papr(N,OS,n_sblk,mod_order,dB_ s,dB i,dB e,MaxIter)

* n_sblk   : Number of sub blocks

M = N*OS;

bps=1log2 (mod_order) ;

dBs=dB_s:dB i:dB e; dBcs=dBs+dB i/2;

for iter=1:MaxIter
temp_papr=zeros(1,length(n_sblk) ) ;
b=ones(1,n_sblk).'; % weight factor
tx_bits=floor(rand(1,N*bps) *2) ;
mod_sym=QAM mod(tx_bits, bps) ;
[Nx,Nc] =size(mod_sym) ;
zero_pad_sym=zeros (Nr,Nc*0OS) ;

for k=1:Nr        % zero padding for oversampling
zero pad_sym(k,1:0S:Nc*OS) =mod_sym(k, :) ;
end
for k=1:n_sblk     6 “4 (7.33) % disjoint subblock mapping

kk= (k-1) *M/n_sblk+1:k*M/n_sblk;
sub_block(k,kk)=zero_pad_sym(1,kk) ;
end
Lift sym = 1fft (sub_block.',M) .1;
for m=l1:n_sblk
for k=l1:n_sblk, temp_a(k,:)=ifft_sym(k,:)*b(k); end
sym_pow= abs(sum(temp_a)) .*2;
temp_papr(m)= max(sym_pow) /mean(sym_pow) ;
if m==1, b(m+1)=-1;
6166

if min(temp papr)<temp_papr(m), b(m)=1;
else b(m)=-1; end
b(m+1)=-1;
end
end

323



===== PAGE 322 =====
PART IL_ 야미/과 MATLAB

for =1:ㅁ 81501, a(k,:)=ifft_sym(k,:)*b(k); end
sym_pow= abs(sum(a,1)) .*2;
mean_pow (iter) =mean(sym_pow) ; max_pow(iter)= max(sym_pow) ;
clear temp_papr
end
PAPR=max_pow./mean_pow; PAPR_dB=10*log10(PAPR) ;
count=0; N_bins=hist (PAPR_dB,dBcs) ;
for i=length(dBs) :-1:1
count=count+N_bins(i); pr(i)=count/MaxIter;
end

0a!
4

ia) 프로그램 7.10 Partial Transmit Sequence

% compare PTS CCDF.m
% Plot Fig. 7.21
OS = 4% N = 256% M = N*OS;
mod_order = 16 ;
V = [1,2,4,8,16]; % number of subblocks
dB s = 0; dB i-=0.1; dBe=12;
088 = dB _s:dB i:dB 6; 0808 = dBs+dB i/2;
MaxIter = 10; % # of transmitted OFDM blocks
ofdm_pr = ofdma_papr(N,0S,mod_order,dB_s,dB_i,dB e,MaxIter) ;
for k = 1:length(Vv)
n_sblk = V(k);
PTS _pr(k,:)=PTS_papr(N,0OS,n_sblk,mod_order,dB_s,dB_ i,dB e,MaxIter) ;
end

_—

i 프로그램 7.11 PTS 기법에서 부블록 개수에 따른 PAPR 분석 프로그램

Ys) Tone Reservation 기법

TR(Tone Reservation)[193] 기법에서는 별도의 PRT(Peak Reduction Tone)= 할당하
고 이 2#7에 적절한 값을 송신하여 시간영역에서 PAPR 감쇄 신호를 생성한다. 즉, PRT
기법에서는 전체 톤을 데이터 ASS 위한 톤과 2#로 구분하여 사용하며, 송신단과 수
신단에서는 미리 PAPR 감소를 위한 2#1의 위치를 알고 있어야 한다. 이 때 PRTE 데이
BS 전송하는 목적으로는 사용되지 않고, PAPR 감소를 위하여 임의의 값을 갖는 심볼을

PRTO] 할당할 수 있다.

324


===== PAGE 323 =====
제7장_『ㅁ406 감쇄 기법

TR 기법에서는 데이터 톤과 001가 중복되지 않고 상호 배타적으로 할당되기 때문에,
데이터 벡터 ※와 PAPR 감쇄 벡터 CH 나뉘어진다. 또한 개의 PRT) 위치를
R= fie vig) 로 정의한다. 여기서 RS 예약된 톤의 수를 나타내며, We 전체 톤의
수를 나타내고, PRT ES =, SSI, 6…으| </ 을 만족한다. RS 의 여집합
으로 정의하면, 입력 ASS 다음과 같이 표현된다.

Clk], keR

지시+더시= ee  ke R

(7.34)

여기서 XTkRS 데이터 심볼을 나타내고, <'[시는 PRTO 할당되는 심볼을 나타낸다. 식
(7.34)는 다음과 같이 다시 쓸 수 있다.

1            ㅣ           |
a     X[nje??™""* ee    C[n]e?™"®                   4.35
ve              we                         (735)

x[n]+c[n] =
CP(Cyclic Prefix)7} 채널 임펄스 응답보다 길다는 가정하에서 수신단 의 출력은
다음과 같이 주어진다.

H{KJC{k]+Z[k], ke R

H[k\(X[k] + C[k]) + Z[k] = teat +Z[k], ke R°

(7.36)

여기서 #[시는 채널 임펄스 응답의 이고, 2|시는 부가 잡음의 이다. TR 기법
에서는 ke “인 위치의 톤의 값만 디코딩하고, ke 인 위치의 8#7의 값은 무시한다.
그림 7.22는 TR 기법의 블록도를 보여준다.



===== PAGE 324 =====
PART 1 _야미과 MATLAB

‘

지이                          #A(0]X [0] + 210]
0                         Alijcti)+ 211]
poi                        >
X(2]  N |                   N   H(2]X[2] + 212]
: |00              DFT | :     ㆍ
0                          H(N-1]C([N-1]+ Z[N-1]
Vo                        ~
0
cll
aie N
ㆍ | IOFT
c([N-1]
_—>

그림 7.22 Tone Reservation 기법의 블록도

TR 기법에서는 데이터 심볼 이외에 PRTS 전송하기 때문에 전력이 증가하고, PRT)
서 데이터를 전송할 수 없기 때문에 데이터 ASB] 감소하는 단점이 있다.

QEXY Tone Injection 기법

TR 기법은 전체 톤의 일부분을 PRTE 예약하고 간단한 송신단 알고리즘을 사용하여
수신단에서 추가적인 복잡도가 없이 PAPRS 감소하는 기법이다. 그러나 PRT7} 사용하
는 톤에 비하여 전체 Eo} 수가 작으면 데이터 전송률이 감소하게 된다. 1(1006
Injection) 기법[193]에서는 데이터 전송율을 감소시키지 않으면서 PAPRS 감소하기 위
하여 TR 기법을 변형한 형태로 볼 수 있다. 그림 7.23은 11 기법의 블록도를 보여준다.

저0]|+ 0001+ 310]

ait                                                                                X(0)+ 20]

X(1]

X|2     N
ㆍ | IDFT

K(1]+ 211] + 24     X(1]+ 24]

+ +

FEQ

DFT

Modulo—D

X([N-1

X(N-1]+ C[N-1]+ Z[N-1]

이 보니                 :                x(t)+c(t)

IDFT

그림 7.23 Tone Injection 기법의 블록도

326



===== PAGE 325 =====
HI7Zt_PAPR 감쇄 기법

TR 기법에서는 PAPR 감쇄 심볼인 CS 데이터 ASS 하지 않는 별도의 8#7에 전송
하였다. 그러나 TI 기법에서는 CS 별도의 톤에 할당하지 않고 데이터를 전송하는 심볼
에 추가하여 전송한다. 이 과정에서 원래 신호의 성상도를 확장된 성상도의 점으로 바꾸
며, 이 때 발생되는 추가적인 자유도로 인하여 240&을 감소할 수 있다. 위 과정을 수식으
로 표현하면 다음과 같다.

N

1   개

2

¥n] = x[n] + c[n]=                X[k] + Clk])e?""™                             (7.37)

여기서 주파수 벡터 C=[Cl],--.CIN-I]] 또는 이와 등가인 시간 영역 시퀸스
e=[c[0],-.c[N-I]] PAPR 감소를 위한 신호이다. 또한 Hn] 은 pAPRo] FAW 신호
를 나타낸다. 수신단에서는 수신된 심볼 #4[4]([4]+1]) 를 복조해야 하기 때문에
[^] 를 효율적으로 제거하는 방법이 필요하다. TR 기법에서는 데이터 Zz} PRT] 위치
가 다르기 때문에 수신된 심볼을 복조하는 데 어려움이 없었으나, TI 기법에서는
Ck] = 214]/2+ 701412 에 의해 ClA] 7} 선택되기 때문에 효율적인 BA 방법이 필요하
다. 여기서 pik] 2} 014]는 PAPRS 최소화하기 위해서 선택된 정수이고, 고정 상수 2
는 송신단과 수신단에서 미리 알고 있는 양의 실수이다. 11 기법에서 적절한 상수 gD
가 선택이 되면, 수신단에서 주파수 영역 등화기위 출력 값인 X[A]+C[k]+Z[k] 또는
X[k]+ p[k]D + q[k]D + 214] 의 실수와 허수 성분의 Modulo—D 연산을 해줌으로써
01] 는 제거될 수 있다. 상수 값 22 ABA 고려할 Ae 다음과 같다. oye 데이터를
M-ary QAM 또는 2"-044에 의해 전송할 때, 74 =2* 는 성상도의 크기를 나타내고 d
는 성상도 점 사이의 최소 거리를 나타낸다. 이 때 상수 DS 사용하는 심볼 C7} BER
성능에 영향을 주지 않도록 하기 위해서는 4074 과 같거나 커야 한다.
그림 7.24는 TI 기법에서 16-QAM 성상도의 확장을 보여준다. 이 그림에서 검정색 심
은 BAS] QAM 심볼을 나타내고, 흰색 ASS 식 (7.38)에 의해 확장된 심볼을 나타

보
=
낸

로

X[k] = X[k]+ Clk] = X[k] + 2412 + jq[k]D                    (7.38)



===== PAGE 326 =====
PART IL_ OFDMZ} MATLAB

AB                                 A7
그림 7.24 Tone Injection on 16-QAM 성상도의 확장

그림 7.25는 16QAM 에서 pLk]=[-1,0,1], 014]=[-1.0.1] 의 경우 생성된 확장된 성

(es

상도를 보여준다. 이 그림으로부터 원래의 16QAM YALE 더 큰 9x16QAM 성상도로
맵핑되며, 송신기는 같은 정보를 싶는 ONS US 하나를 선택할 수 있음을 알 수 있다.
여기서 발생되는 추가적인 자유도에 의해 PAPRS 감소할 수 있다.

Ear 다우1 i es Sa ee1 ie era nd Lg OL1

1    를 ! ㅣ  1 1     ㅣ

1     1 ㅣ     ㅣ ㅣ     1

1006100!: ‘e sje ws !100ㅁ100

‘a Via Vi ia Via Vi 14 Via Vi

‘@ s/@ s: 'e@ wie '

14 Via Vi ia Via Vi

{tes Rein 주아1 02 시게 이이1 (OUR See Sa1

1   =)  1 I   0 281 ㅣ   a)  1

|     ot     1 ㅣ     ㅣ

1001001 10601001 10010 FF:

iA Via Vi  14 Via Vi 14 Via Vi

<<

D

그림 7.25 Stel 16QAM 성상도



===== PAGE 327 =====
제장 ㅁㅁ 감쇄 기법

송신단에서 XA 상수 CIA} 더해진 후 최종적으로 전송되는 신호는 다음과 같다.

X[n] ==> (xT + p[k]D + jq[k\D) e?™'™                             (7.39)

k=0
그림 7.242) 흰색 심볼들이 검정색 심볼들과 같은 정보를 갖고 있으므로 수신단에서 주
영역 등화기(080))의 출력 신호의 실수와 허수 성분에 Modulo-D 연산을 함으로
iv Al (7.38)에서의 CIS 쉽게 AAS 수 있다. 따라서 TI 기법은 부가 정보를 전송할
필요가 없고, 데이터 전송율의 감소도 발생하지 않는 장점이 있다. 그러나 그림 7.24에
타난 바와 같이 2[4]%0이거나 q[k] #00] 4 확장된 성상도의 신호의 전송 때문에 신호 전
력이 증가하는 단점이 있다.

QAR DFT 확산 (SC-FDMA) 기법

OFDMA 시스템에서 IFFT 전단에 확산 코드로서 Walsh-Hadamard 부호 등의 직교
부호 행렬을 사용하는 연구가 많이 이루어져 왔다. 본 절에서는 직교 부호 행렬로서
Fourier 행렬을 사용하는 DFT 확산 기법 또는 SC-FDMA(Single—Carrier FDMA) 기법
에 대하여 설명한다[194].

OFDM 시스템에서 IFFT2] 크기(//)와 동일한 크기를 갖는 DFT 확산 부호를 사용할
우 DFT    oe IFFT 두 os 산이 서로를 iinet aa 단위로 처리하는

N

5 =

ㅣ

Add Guard
Interval

IFFT
P/S

1
a   Fl

Encoder +
Interleaver
iI simplify
Encoder +                     ;                                                                                Add Guard       ;
  Modulation            7

그림 7.26 DFT 확산 부호를 채용한 OFDM 시스템과 단일 반송파 시스템과의 관계

마 [-
Spreading

Modulation



===== PAGE 328 =====
PART ㅁㅁ OFDMZ} MATLAB

OFDMA 시스템에서 단일 사용자가 전체 부반송파를 사용할 경우에는 위와 같은 결과
가 되어 단일 반송파 방식으로 전송하고 수신단에서 주파수 영역 등화를 하는 SC-DFE
(Single-Carrier Decision Feedback Equalization) 방식과 유사하게 된다. 그러나 실제의
OFDMA 시스템에서는 다중 사용자가 일부의 부반송파를 사용하기 때문에 자원 할당 방
Ajo] 따라 다른 결과가 나타난다. OFDMA 전송 방식에서 사용자에게 부반송파를 맵핑하
는 방식에 따라 그림 7.27과 같이 DFDMA(Distributed FDMA)?} LFDMA(Localized
FDMA) 방식으로 나눌 수 있다.

DFT 확산 방식은 상향링크 적용 시에 PAPRS 감쇄하는 장점이 있어 본 절에서도 상
향링크의 단말 관점에서 기술한다[196]. 기지국에서 하향링크로 데이터를 전송할 ae
달리, 단말에서 상향링크로 데이터를 전송할 경우에는 단말기 사용자의 데이터만 전송
다. 따라서 단말기 사용자가 사용하는 부반송파를 제외하고 다른 부반송파는 모두 0으로
채우게 된다. DFDMAA= 입력 데이터의 DFT 출력 값이 전체 00 분산되어 할당
되는 반면, LFDMAA 입력 데이터의 DFT 출력 gto] 연속적인 부반송파에 할당된다.
사용자가 사용하는 부반송파의 개수를 24이라고 하고 00의 부반송파 개수를 이라고
할 때, DFDMA# 확산된 심볼이 //44=0의 등간격에 위치한 부반송파에 맵평이 되면
IFDMA(Interleaved 『12544)라고 정의한다. 여기서 OH 대역폭 확장 인자이다.

X(0]                            [0]                               = ~ X [0]
26108 {                                  Zeros
~
[11
Zeros}:                소이
{                        1
X(2]
X([M-1]
*UM~ 1]                   — +                            Zeros      :
Zeros {    :                                                         :
~ xX[n-1]                   —> X[n- 1]
DFDOMA                                          LFDMA

그림 7.27 OFDMAQ| 부반송파 맵핑 방식 : DFDMASt LEDMA

그림 7.28은 M=4, 0=3, /7=12인 경우의 DFT 확산의 예제를 보여주며, 그림 7.29
는 다중 사용자의 부반송파 할당 YAS 보여준다.



===== PAGE 329 =====
제7장_ㄷ46 감쇄 기법

DFT} X[i]= Sime", M= ‘

m=0

{xT} lolx

N=Q0-M
12=3-4
N>Q-M
12>2-4
N=Q0-M
12=3-4

{X 21007 }     x

{Xorcom}

000     @o[o[o]o]olo]olo)

frequency

그림 7.28 DFT 확산의 예 : IFDMA, DFDMA, LFDMA (1/=4, N=12, O=3)

|] Terminal 1
A Terminal 2
| Terminals

frequency                                                                 frequency

Distributed Mode                                          Localized Mode

그림 7.29 다중 사용자의 부반송파 할당 방법의 예 (사용자 수: 3, M=4, N=12, O=3)

0

그림 7-29는 IFDMA 부반송파 맵핑 방식을 사용한 DET 확산 기법의 송신단 블록도

를 보여준다.
( 1    Xt) 1. 지시    z{n)     |
Encoder +               |     ee ee                  |
Interleaver                                   a              였                                                  |         Add Guard
|     이    LS                 |     Interval

Encoder +                     |              |                ae                   Frequency ㅣ .             Add Guard

18 7.30 DFT 확산 기법을 적용한 OFDMA 상향링크 『ㅁ144)

위 그림에 나타난 바와 같이 입력 데이터 x[m]2 DFT 확산되어 ㅅ[2]로 변환된 후
IFDMA 부반송파로 맵핑이 된다. 이 때 IFFT 입력신호 ㅅ[/]은 다음과 같이 주어진다.

331


===== PAGE 330 =====
PART Il_ 야미/과 MATLAB

9    X[k/Q], k=O-m (0<m<M-1
Stk =  [k/Q] 」  04 (   |     )           7.40)
0, otherwise
N=Q- 이다. IFDMA 부반송파 맵핑을 사용하므로
우 IFFT2] 출력 치7] 은

여기서 0ㄴ&ㄴ//-1이고
n=M-q+m (0Sq5Q0-1,0<m<M-1)2 주어진다. 이 경

다음과 같이 유도된다[1971.

.    :         (=          11%      fan ni
Fm} (= 5Mg-+ my) =  [ke 중 그 > 서씨
k=0             m =0
7   a xime 70 wm a    rae  Ps X[m     en)   (7.41)

따라서 x[n] 2 시간영역에서 원래의 입력 심볼 alm] S 1/0 만큼 스케일링된 성분이
반복되는 형태로 나타난다. 부반송파 맵핑이 / 번째 부반송파(0<7으(2-1)부터 시작되

는 IFDMA 경우의 X[k] = 다음과 같이 주어진다.

0, otherwise
q    NG       o M2 *lm
M-1       1020 Ya          M-1        20    oni

a I   X[m Je”     pay, =, i   X[mJe” =   a 4   7.48)

Q M ie =0                   02  M <>

1] j202
=긍7 -xfm]

Q

경우에는 ov 만큼의 추가적인 위

따라서, / 번째 부반송파부터 맵핑이 되는 18014
상 회전이 발생한다.

fo}

_ 332



===== PAGE 331 =====
제7장_ㅁ46 감쇄 기법

>

LEDMA 부반송파 맵핑 방식을 사용하여 DET SHES 할 경우 송신단에서 IFFT 입력
신호 X[k] 다음과 같이 주어진다.                       |

.   everenct
X[k] =                                                          (7.44)

0, Msk<sN-1

LFDMA 부반송파 WAS 사용하므로 n=O-m+q(0<sqsO-1,0<m<sM-l1)z#
주어진다.

12]=괴00+ 0] 노시 = 2S athe “OM      (7.45)
만약 0=0이면
비= 이 1S ge te SS ee = a       (7.46)
OME          O Mix         Q
만약 4※0이면, XTK]=Satple ” 이므로, 식 (745): 다음과 같이 표현된다.
l= 310m-+g]=2 1-2" |-그호 ㅡ꼬리
Me lee]          (7.47)
1-6 | ¥ 0
exh) 1 atl
QO: x[n]  -    28:     20{ 20, 4 }
M OM

102      sin nf               7.48
wo     «3    i"  |      ane)

333 _



===== PAGE 332 =====
PART I OFDM} MATLAB

{xtmj} [at | eh  ze) | als} |

{0-3 pun}   Lobukebtbobileal (3]e loll 1] (2le(s]
{0300.00} lO ae | a fl | a [ole oe | x bots] | |

Time

3                                         .
*=)iclm.q.p]- 3p] .clm.q,p] : complex weight

p=0

그림 7.31 DFT 확산 방식에서 부반송파 맵핑 방식에 따른 시간영역 심볼의 예

식 (7.46)과 (7.48)에 나타난 바와 같이, 시간 영역에서 LFDMA 신호는 M72] 배수 샘
플 위치의 경우에는 입력 샘플에 Vows 스케일링
입력 샘플에 각각 다른 복소 가중치가 곱해진 시간영
림 7.31은 N=12, M=4, 0=3인 경우에 부반송파 맵핑 방식에 따른 시간 영역 심볼의
예를 보여준다.

그림 7.32는 OFDMA/IFDMA/LFDMA 방식의 PAPR 성능을 비교하여 보여주는데, 이
로부터 DFT 확산 방식의 PAPR 감소 성능이 부반송파 맵핑 방식에 따라 크게 차이가 Qh
음을 알 수 있다. 가령 16-0414의 경우, CCDF 1%의 지점에서 IFDMA= 3.5dB,
LFDMA= 8.3dB, OFDMA+ 10.808 의 ?ㅅ[을 가짐으로써, OFDMA®] 비해 IFDMA
는 약 7.308 낮은, 그리고 LFDMA 약 3.208 낮은 PAPRE 갖는다. 이는 프로그램
7.14(‘compare_DFT_spreading”)S= 통하여 프로그램 7.9(“010018 080「')와 프로그램 7.12
(“ifdma_papr”) 및 프로그램 7.14(“lfdma_papr”)S 실행시킴으로써 얻어진 것이다. 이 모
의실험에서 사용된 변조 방식은 QPSK, 16-QAM, 64-QAMO]31, 오버샘플링은 적용하
지 않았으며, M=64, N=256, 0=4이고, 10,000개의 OFDM 심볼을 사용하였다.

=:                                                                                                                                                                       OFDMA
= LFOMA
—— |FOMA

piss SS} 10° p=

ee              — IFDMA

3

Pr(PAPRDPAPR,)

3

4   6 0                ——                       —
PAPR, [dB]                    PAPR, [dB]                    PAPR, [dB]
QPSK                     16QAM                     64QAM

그림 7.32 DFT 확산 방식의 PAPR 성능 비교 (IFDMA, LFDMA, OFDMA)

334


===== PAGE 333 =====
제7장_ㅁ466 감쇄 기법

function pr = ifdma_papr(N,M,mod_order,dB_s,dB_i,dB e,MaxIter)

웅지, M     : FFT size(# of total subcarriers) & block size
* mod_order: 4 -> 4QAM, 16 ->16QAM, else -> 64 QAM

% MaxIter : number of iterations

Q = N/M;    % spreading factor

bps = log2(mod_order) ;
088 = dB s:dB_ i:dB 6; 0808 = dBs+dB i/2;
for iter=1:MaxIter
tx_bits=floor(rand(1,M*bps) *2) ;
mod_sym=QAM mod(tx_bits,bps) ;
f£t_sym=fft (mod_sym,M) ;
zero fft_temp=[fft_sym(:).'; zeros(Q-1,length(f£ft_sym) )];
wero fit=zero fit temp (1 ) , 「}
ifft sym=ifft (zero fft,N);
sym pow=abs (ifft_sym) .*2;
mean_pow(iter) =mean(sym_pow) ; max_pow(iter) =max(sym_pow) ;
end
PAPR=max_pow./mean_pow; PAPR_dB=10*1log10 (PAPR) ;
N bins = hist (PAPR_dB, dBcs) ;

count = 0;
for i=length(dBs) :-1:1

count = count+N bins(i); pr(i) = count/MaxIter;
end

Tm) 프로그램 7.12 IFDMA2| PAPR 함수

function pr = 1fdma_papr(N,M,mod_order,dB_s,dB_i,dB e,MaxIter)
Q = N/M; bps = log2(mod_order) ;
088 = dB s:dB i:dB 6; dBcs = dBs+dB i/2;
for iter=1:MaxIter
tx_bits=floor(rand(1,M*bps) *2) ;
mod_sym=QAM mod(tx_bits,bps) ;
f£ft_sym=fft (mod_sym,M) ;
zero fft=[f£ft_sym zeros(1,M*(Q-1))]; % subcarrier mapping (LFDMA)
ifft_sym=ifft (zero fft,N) ;
sym_pow=abs (ifft_sym) .*2;

335 _



===== PAGE 334 =====
PART ㅁㅁ OFDMZ} MATLAB

mean_pow (iter) =mean(sym_pow) ; max_pow(iter) =max(sym_pow) ;
end
PAPR=max_pow./mean_pow; PAPR_dB=10*1log10 (PAPR) ;
N_bins = hist (PAPR_dB,dBcs) ;

count = 0;
for i=length(dBs) :-1:1
count = count+N_ bins(i); pr(i) = count/MaxIter;
end
ia) DSH 7.13 LFDMA2| PAPR 함수

% compare DFT spreading.m

6 Plot Fig. 7.32

N=256; M=64; % FFT size and block size

OS = 1; mod_order=16;

08 8=0; 08 1=0.2; dB e=12;

dBs = 08 8:08 1:08 6; 0808 = dBs+dB i/2;    % dB vector
MaxIter=1000; % number of iterations

ofdma_pr = ofdma_papr(N,OS,mod_order,dB_s,dB_i,dB e,MaxIter) ;
lfdma_pr = 1fdma_papr(N,M,mod_order,dB_s,dB_i,dB e,MaxIter) ;
ifdma_pr = ifdma_papr(N,M,mod_order,dB_ s,dB_i,dB e,MaxIter) ;

fa) 프로그램 7.14 |IFDMA/LFDMA/OFDMA 방식의 PAPR 분석 프로그램

터의 특성에 따른 DFT 확산 기법의 PAPR 성능을 비교한다. PAPR 감쇄 방
식       는 필터의 특성에 따라 PAPR 성능이 변화하기 때문에 IFDMAS} LFDMA
부반송파 맵핑 방식에 대하여 PAPR 성능을 살펴본다. 일반적으로 통신시스템에 널리 사
용되는 필터로 701660 cosine YES 이용하여 펄스 쉐이핑(04156 shaping) 하였을 때
roll-off 계수 ao] 따른 Ves 분석한다.

7.33은 @의 변화에 따른 IFDMA/LFDMA 방식의 PAPR 성능을 보여주는데, 이
DMAY] 경우에는 가 OWA 1로 증가할수록 PAPRE 감소하지만 대

수 있다. 이 그림은 22714 7.17(“compare DFT spreading w_psf’)S 통하여 프로그
7.15(“Ifdma_psf’)2} 프로그램 7.17(“ifdma psf’) 실행시킴으로써 얻어진 결과이다.
모의실험에서는 파라미터들이 N=256, M=64, 0=4로 설정되었고, QPSK2} 16-04ㅅ44

= 보떤 때                                                    만 대역외 발
산은 증가하므로 대역외 발산과 PAPRY| 감소 성능이 AZ trade-off 관계에 있는 AS 알
수 있다. 반면, LFDMAS] 경우에는 PAPR 성능이 @ 에 따라 크게 변화하지 않는 AS 알
수                                                                       램

의

336



===== PAGE 335 =====
제7장_『ㄷ466 감쇄 기법

Pr(PAPR>PAPR,)

ie        (solid line) without pulse shapi
PSK    — (solid line) without pulse shaping     16
“                     (dotted line) with pulse shaping              49

그림 7.33 펠터의 특성에 따른 DFT 확산 기법의 PAPR 성능 비교

변조가 사용되었으며, 송신 신호는 8배 오버샘플링 되었고, 50,000개의 OFDM 심볼이 사
용되었다. 또한, IFFT 후에 OFDM 심볼은 시간영역에서 위의 필터를 통과하였다.

음은 한          부반송파 수에 따른 DET 확산 기법의 PAPR 성능을 비교한다.
이 LEDMA®| 경우에 @어 대한 영향보다 AVS 의 비율에 대한 ao] 더 크기 때
에 LEDMA®] 대해서만 모의실험을 하였다. 모의실험에서 64-QAMES 사용하였고, 송
신호에 오버샘플링은 적용하지 않았다. 또한, /=256으로 고정하고, MS 4, 8, 32, 64,
128로 변화하여 0 7} 64, 32, 8, 4, 2로 변화하였다. 50,000개의 OFDM 심볼을 사용하여
모의실험하였다. 그림 7.34로부터 LFDMAS| 경우 Mo] 증가할수록 PAPRO] 증가하는
을 알 수 있다.

결론적으로, IFDMAS} LFDMA= 적용한 SC-FDMA 세 OFDMA#t} 낮은
PAPRE 제공하기 때문에 3GPP LTE 등에서 상향링크 전송기법의 표준으로 사용된다.
위의 결과로부터 IFDMA7} 14114&보다 Ye PAPRE 제공하는 것을 알 수 있지만
IFDMAS ale] 상향링크 자원 할당에 AK LAHSA, well 등)이 있기 때문에 AY
크에 LFDMA7} 주로 적용된다.

fr Ad   in

337


===== PAGE 336 =====
PART 1 OFDMZ} MATLAB

Pr(PAPR>PAPR,)

10°

function pr = lfdma_psf(N,M,mod_order,dB_s,dB i,dB e,MaxIter)

웅지, M     : FFT size (# of total subcarriers) and block size
N_sym=6; % RC filter length
N_os=8;    % oversampling ratio

Q = N/M;   % spreading factor
bps = 1og2(mod_order) ;
088 = dB _s:dB_ i:dB 6; 0808 = dBs+dB i/2;
rhos =:0:0.2:1; % roll-off factor
for i=1:length(rhos)
roll off = rhos (1) ;
psf=rcosfir(roll_off,N sym,N_os,1,'norm')*N_o0s;% RC filter coeff
for iter=1:MaxIter
tx_bits=floor (rand(1,M*bps) *2) ;
mod_sym=QAM_ mod(tx_bits,bps) ;
fft_sym=fft (mod_sym,M) ;
zero fft=[fft_sym zeros(1,M*(Q-1))]; ‘subcarrier mapping (LFDMA)
ifft_sym=ifft (zero fft,N);
ifft_sym_zero_temp=[ifft_sym; zeros (N_os-1,length(ifft_sym))];
ifft_sym_zero=ifft_sym_ zero temp(:).';
psf_out=conv(ifft_sym_zero,psf); « pulse shaping filtering
sym_pow=abs (psf_out) .*2;
mean_pow (iter) =mean(sym_pow) ; max_pow(iter) =max(sym pow) ;

 038



===== PAGE 337 =====
제장 PAPR 감쇄 기법

end
PAPR=max_pow./mean_pow; PAPR_dB=10*log10(PAPR) ;
N_bins = hist (PAPR_dB,dBcs) ;
count = 0,
for m=length(dBs) :-1:1
count = count+N bins(m); pr(i,m) = count/MaxIter;
end
end

ja! 프로그램 715 Raised cosine BES 적용한 LFDMAQ| PAPR 함수

function pr = ifdma_psf(N,M,mod_order,dB_s,dB i,dB e,MaxIter)
N_sym=6;    6 RC filter length

N_os=8;     % oversampling ratio
Q = N/M;    % spreading factor

bps = 1092 (mod_order) ;
088 = dB s:dB i:dB 6; dBcs = dBs+dB i/2;
rhos = [0:0.2:1]; % roll-off factor
for i=1:length(rhos)
roll off = rhos (i);
psf=rcosfir(roll_off,N_sym,N_os,1,'norm')*N os; % RC filter coeff
for iter=1:MaxIter
tx_bits=floor(rand(1,M*bps) *2) ;
mod_sym=QAM mod(tx_bits,bps) ;
f£t_sym=fft (mod_sym,M) ;
zero fft_temp=[fft_sym(:).'; zeros(Q-1,length(fft_sym))];
zero _fft=zero tft (2) , ! ;
ifft_sym=ifft (zero _fft,N);
ifft_sym_zero temp=[ifft_sym; zeros(N_os-1,length(ifft_sym))]j;
ifft_sym_zero=ifft_sym_zero_temp(:).';
psf_out=conv(ifft_sym zero,psf); % pulse shaping filtering
sym_pow=abs (psf_out) .*2;
mean_pow(iter) =mean(sym_pow) ; max_pow(iter) =max(sym_pow) ;
end
PAPR=max_pow./mean_pow; PAPR_dB=10*1log10(PAPR) ;
N_bins = hist (PAPR_dB, dBcs) ;
count = 0;
for m=length(dBs) :-1:1
count = count+N_bins(m); pr(i,m) = count/MaxIter;
end
end

i 프로그램 7.16 Raised cosine BAS 적용한 IFDMAL| PAPR

때
+

339



===== PAGE 338 =====
PART ㅁㅁ OFDM} MATLAB

* compare DFT spreading _w psf.m

N=256; M=64; MaxIter=50000; mod_order=16; dB s=0; dB _i=0.2; dB e=12;
dBs = 08 8108 1108 e; dBcs = dBs+dB i/2;

ifdma_pr = ifdma_papr(N,M,mod_order,dB_s,dB_ i,dB e,MaxIter) ;
lfdma_pr = 1fdma_papr(N,M,mod_order,dB_s,dB i,dB e,MaxIter) ;
ifdma_psf_pr =ifdma_psf(N,M,mod_order,dB_s,dB_i,dB e,MaxIter) ;
lfdma_psf_pr = lfdma_psf(N,M,mod_order,dB_s,dB_i,dB e,MaxIter) ;

‘ml 프로그램 7.17 Roll—off 인자에 따른 IFDMA/LFDMA 방식의 PAPR 분석 프로그램



===== PAGE 339 =====
셀룰러 시스템에 OFDM 전송 방식을 사용할 경우 인접 셀간 간섭이 발생하여 셀 경계
지역에 있는 단말기는 성능이 크게 열화 될 수 있다. 이러한 셀간 간섭을 감소할 수 있는
셀간 간섭 완화 기법(101660611 Interference Mitigation Technique)-2 크게 셀간 간섭 조정
기법(106670611 Interference Coordination Technique), 셀간 간섭 랜덤화 7] ¥\(Intercell
Interference Randomization Technique), 셀간 간섭 제거 기법(01016700611 Interference
Cancellation 160001046)으로 분류할 수 있다.

RNB 주파수 자원 할당 기법

OFDMA 전송방식을 사용하는 셀룰러 시스템을 설계할 경우에 셀간 WAS 줄
하여 여러 형태의 주파수 재사용 방식을 고려할 수 있으며, 다양한 부반송파 할당 방식을
사용할 수 있다. 본 절에서는 이들 방식의 개념과 특성에 대해서 살펴본다. 그림 8.1은
OFDMA 셀룰러 시스템에서 기본적인 주파수 재사용 방식과 부반송파 할당 방식을 보여
준다.

etl shh 주파수 AAS Govt 조금씩 다르나 본 장에서는 영문의 tequeny
reuseS 주파수 재사용률로 정의하고, frequency reuse factor$          수 재사용 계수로 정의
한다. 이 때 주파수 재사용률과 주파수 재사용 계수는        수 관계이 있다. 그림 8.1(8)에서
와 같이 주파수 재사용률이 1일 경우, 한 셀 WoL a 모든 주파수를 사용하기 때문에 가용할
수 있는 대역이 증가하여 대역의 효율성은 증가하나 셀 경계에서 동일 채널에 의한 셀간
간섭 때문에 outage rate7} 증가하게 된다. 반면, 그림 8.1(6)와 (0)와 같이 전체 대역을

fu

341


===== PAGE 340 =====
PART |! _ OFDM2} MATLAB

Cell 1               1

Cell 2

Cell 3

I

Frequency

(8) 주파수 재사용률 = 1

0611

0812        [2]

Cell 3              | |
워--- ~

Frequency

caf fl 8
00808
oo HORE

Frequency

b) 주파수 재사용률 = 3                  (0) 주파수 재사용률 = 3

그림 8.1 OFDMA 셀룰러 시스템에서 주파수 재사용 방식의 Of]

3개의 부대역(6400800)으로 나누고 인접한 셀간에는 서로 다른 부대역을 할당하는 경우,
그림 8.1(8)에 비하여 동일 채널에 의한 간섭은 줄어들지만 가용 대역이 작아져서 대역의
효율성이 감소하게 된다. 이러한 주파수 재사용률과 셀간 간섭을 함께 고려하여 셀 경계
에서의 성능을 향상시킬 수 있는 방법으로서, 전체 부반송파를 다수의 부대역으로 분할하
고 각 셀에서 이 중의 일부 부대역 만을 사용하여 동일 채널 WHS 완화하는
FFR(Fractional Frequency Reuse) 기법들이 제안되었다[198]. 그림 8.2는 OFDMA 셀룰
러 시스템에서 주파수 재사용률 = 3/2, 7/6인 경우의 FFR 기법을 보여준다.

그림 8.2와 같이 FFR 기법을 사용하면 셀간 간섭을 완화하면서 대역의 효율성을 향상
시킬 수 있다. 이 경우 각 AoA] 특정 부대역을 사용하지 않으며 인접한 A 영역에서 이
부대역을 사용하여 인접한 A 영역에서는 부대역이 겹치지 않게 할당한다. 또한, OFDMA
셀룰러 시스템에서는 모든 SAHA 동일한 주파수 재사용률을 사용할 필요가 없고 위치
에 따라서 다른 주파수 재사용률을 사용할 수 있다. 예를 들어, 셀 경계의 영역에서는 셀
간 간섭이 크기 때문에 주파수 재사용률 3을 사용하면서, 셀 중앙의 영역에서는 인접 셀
로부터의 간섭이 적으므로 주파수 재사용 1을 사용하여 인접 셀간 간섭을 완화할 수 있다.

342


===== PAGE 341 =====
Cell 1        [2] 3 |
Cell 2  [1]      [3]
0813  Ree.

Frequency

Frequency

 (8) 주파수 재사용률 = 3/2                  (6) 주파수 재사용률 = 7/6
그림 8.2 OFDMA 셀룰러 시스템에서 FFR 기법의 예

그림 8.3에서 (는 주파수 재사용률 1(셀내)과 3(셀간)을 사용하는 경우, (는 주파수
재사용률 1과 3/2을 사용하는 경우, (0)는 주 수 재사용률 1과 3과 3/2를 혼합하여 사용
하는 경우를 보여준다.

0811
0812 [이   [2]

케이
cas | 0 4

Frequency

Frequency

(0) 주파수 AALS S = 1 + 3 + 3/2
그림 8.3 OFDMA 셀룰러 시스템에서 FFR 기법의 예 (혼합 주파수 재사용률)

8.1.2 전력 자원 할당 기법
OFDMA 셀룰러 시스템에서는 셀간 간섭을 완화하기 위해 각 셀에 할당된 부대역에 전

력을 다르게 할당할 수 있다. 이를 통해 각 셀의 주파수 재사용률은 1을 유지하면서 인접

343


===== PAGE 342 =====
PART Il_ OFDM2} MATLAB

Frequency

(a) 주파수 재사용률 3에 대한 전력 할당      (06) 주파수 재사용률 3/2에 대한 전력 할당
그림 8.4 OFDMA 셀룰러 시스템에서 전력 자원 할당 Of] (부대역의 수: 3개)

셀간 간섭을 완화할 수 있다. 즉, 셀 중심에서 사용하는 부대역은 모든 셀이 낮은 전력으
로 전송하고, 셀 경계에서 사용하는 부대역은 직교하게 할당하여 높은 전력으로 전송함으
로써 데이터: 전송률을 향상시킨다.

그림 8.4(8)는 그림 8.1(6)에 전력 자원을 다르게 할당한 예를 보여준다. 그림 8.106)에
서는 전체 주파수 대역을 3개의 부대역으로 나누어 각 셀에 직교하게 할당하는데 비해,
그럼 8.4(8)에서는 사용되지 않는 나머지 두 부대역에 낮은 전력으로 데이터를 전송함으로
써 전 대역을 활용한다. 즉, 셀 경계에서는 주파수 재사용률 3으로 직교 할당된 부대역을
사용하고, 셀 중심에서는 셀 경계에서 사용하지 않은 부대역을 낮은 전력으로 사용하는
것이다. 그림 8.406)는 그림 82a] 전력 자원을 다르게 할당한 예를 보여준다. 그림
8.4(8)에서와 같이 셀 경계에서 사용하지 않는 부대역을 A 내에서 낮은 전력으로 사용하
여 주파수 재사용률 1을 유지한다.

< Cell type 1
® Cell type 2
@ Cell type 3

18 8.5 OFDMA 셀룰러 시스템에서 전력 자원 할당 예 (부대역의 수: 97H)



===== PAGE 343 =====
그림 8.5는 전체 부대역을 3개 이상으로 나누어 전력 자원을 다르게 할당한 예를 보여
준다[199]. 전체 HAL 9개의 부대역으로 나눈 후, 6개의 부대역은 낮은 전력으로 셀 내
의 사용자가 사용하고, 3개의 부대역은 높은 전력으로 셀 경계의 사용자가 사용하도록 전
력 자원을 할당한다. 이와 같이 AAS 할당함으로써 주파수 재사용률을 1로 유지함과 동
시에 셀간 간섭을 완화할 수 있다.

4\(adaptive interference coordination) 기법은 사용자들의 CQI 정보와
정보를 활용하여 최대한 동적으로 주파수 대역과 전력을 할당하는 기법
FFR(Flexible Fractional Frequency Reuse) 방식이 이 기법에 속한다[2001.

FFFR 방식에서는 각 셀이 우선권을 갖는 자원 AHS 미리 할당한다. 여기서 자원 그

으로 『

ay
US 갖는 자원 그룹은 인접 셀간 직교하도록 할당되어 세그먼트화와 유사한 역할을

한다.
FFFR 방식에서는 한 셀에서 요구되는 자원의 양이 자원 그룹의 크기를 넘지 않을 경우에
는 할당된 그룹에 우선적으로 자원을 할당하며, 요구되는 자원의 양이 이를 넘을 경우에
는 인접 셀의 그룹을 차용한다. 인접 셀의 그룹을 사용할 경우에는 인접 셀의 할당 정보와
사용자의 CA BRS 활용하여 사용할 부대역과 전송 전력의 크기를 결정함으로써 셀간

간섭을 최소화한다.

그럼 8.6은 FFFR 기법의 예를 보여준다. 이 그림의 061-ㅅ에서는 요구되는 자원의 OF
이 할당된 그룹의 크기를 넘어 그룹 ㅅ 대역을 우선적으로 사용하고 추가 자원을 다른 그
룹에서 사용한다. 이 때 낮은 SNRY] 사용자들에게는 그룹 A 대역을 사용하여 강한 전력
으로 송신을 하는 반면, 높은 SNR 사용자들에게는 인접 셀의 그룹을 사용하여 낮은 전력
으로 송신을 한다. 061-)에서는 요구되는 AGS Fo] 할당된 그룹의 크기를 넘지 않기
때문에 그룹 BASS 사용하여 높은 SNRS 갖는 사용자에게는 낮은 전력으로 낮은
SNR2] 사용자들에게는 높은 전력으로 ASS 한다. 즉, 인접 셀의 대역을 사용하지 않는
경우라도 SNR 따라 전력을 다르게 할당하여 AS 전력의 소모를 줄일 수 Yeh. Cell-C
에서는 요구되는 자원의 양이 많아 전 대역을 사용하기 때문에 인접 셀의 부대역을 낮은
전력으로 모두 사용한다.



===== PAGE 344 =====
PART ㄴㄴ OFDMZ} MATLAB

Cell-A

B2 | B3                   01 | C2

——————

weak users                                 good users

Cell-B   A                6865 | C1 | C2 | 63 | C4] C5

ㅎ
0,
=

ser

Cell-C

good users                          weak users

그림 8.6 OFDMA 셀룰러 시스템을 위한 FFFR 방식의 예

 동적 패킷 할당 기법

동적 채널 (dynamic channel allocation) 방식은 인접 셀간 시그널링(618081108)을
통하여 채널 할당 시점에 가용한 주파수 중에서 가장 품질이 좋은 AUS 선택하여 동적
으로 할당하는 방식이다. 기존의 고정 채널 할당 방식(8×60 00800! 411008000)에서는 각
기지국의 무선 자원을 미리 정해진 패턴에 따라 나누어 사용하는 반면, 동적 채널 할당 방
식에서는 기지국이 네트워크 내 사용 가능한 무선 AAS 공유하며 적응적으로 AS 할
당한다. 특히, 셀룰러 환경에서 OFDMA 방식을 사용할 경우 동적 채널 할당 기법과 결합
함으로써 간섭을 최소화하며 주파수 효율을 높일 수 있다. 동적 채널 할당 방식을 구현하
기 위해서는 광범위한 신호측정과 빠른 채널 재할당이 요구되어 기존의 시스템에서는 적
용하기가 쉽지 않았으나, OFDMA 방식에서는 시간과 주파수 축에서 직교한 부채널이 잘
정의되어 있고 OFDMY] 특성상 모든 부채널에서 채널과 간섭신호를 쉽게 측정할 수 있어
적용이 용이하다. 또한 OFDM 시스템은 일반적으로 패킷 모드로 동작하기 때문에 패킷
단위로 동적 채널 할당이 가능하여 높은 대역 효율성을 실현할 수 있다. 이와 같은 기법을

346



===== PAGE 345 =====
DPA 기법은 간섭 센싱(10[6046006006-5609108)과 직교 자원 할당(01800061 segregation),
그리고 staggered 프레임을 기반으로 한다. 간섭 MAS 기지국에서 전송된 BaH SS
해 단말이 채널 SIS 파악하여 기지국으로 전송하는 것을 의미하며 그림 8.79] 3번
so 이름 ABest 직교 자원 Wa 2 기지국이 ALS 시간 Sah Fait sho

x                                           = Ho

Ac
aus
Ol
2
at
nz
&
Bene
에
|ㅇ
고
도
tl\o
et a
2 0무 【
의
ns
-
로 tr
ot
of,
ty
10
ai
oe
oo
oo
으
으
1°

“4, 2b 기지국이 다른 기지국의 AY 이용 상황(간섭 AE AS 파악하여 GE 기
지국이 사용하지 않는(낮은 간섭 신호 레벨) 채널의 순서로 우선순위를 정하여, 우선순우

가 높은 채널 순서로 WIS 할당하는 것이다. Staggered 프레임은 채널 할당 시에 인접
기지국들이 동시에 같은 채널을 선택하는 것을 방지하기 위하여 한 번에 한 기지국만이
채널을 할당할 수 있는 프레임 구조이다.

DPA 기법은 데이터 트래픽의 버스트한 특성에 따라 채널을 동적으로 할당하며, 공간적
으로 트래픽의 분포가 균일하지 않고 트래픽 부하가 심각하게 크지 않을 경우에 좋은 성
을 얻을 수 있다. 셀룰러 시스템과 같은 다중 사용자 환경에서는 간섭의 영향이 실시간
Neighboring BS performs a procedure with staggered time frame                                                                                             )
2. BS broadcasts destination MS
IDs, retum channels, and numbers
of Packets to be delivered
[고 BS assigns channels to all
packets and broadcasts MS IDs,
assigned channels
irs 이는           일 3. MS    all downlink pilots and
strongest BS                 . MS scans     link p
sends st of accenabechennas io                plate xrays 00
J
그림 8.7 DPA 기법의 기본 동작 과정
347


===== PAGE 346 =====
PART I1_OFDMZ} MATLAB

4                                                                    Boi =

                                                          —
a
동
Ww

£5
BS2
Time
그림 8.8 DPA 기법에서의 직교 자원 할당
으로 변화하기 때문에 단말이 할당 받은 AUS 효과적으로 사용할 수 있기 위해서는 A

Yo] 동적 패킷 할당 과정이 신속하고 정확해야 한다. 또한 시간에 따라 변화하는 AYO]
품질과 할당에 따른 오버헤드의 증가를 고려하여 적절한 주기로 재할당 과정을 수행할 필
요가 있다.

DPA 기법에서 채널 할당 절차는 그림 8.7과 같으며, 기지국간에 채널 할당이 시간차를
두고 수행되도록 staggered 프레임 구조를 사용하여 인접한 셀의 서로 다른 단말이 동시
에 같은 WSS 할당 받지 않도록 한다. DPA 기법에서의 동작 절차는 다음과 같다.

(1) 기지국에서 FURS 포함한 an      전송
@ 기준 ASS 수신한 단말이 수신한 HUA 신호를 이용하여 사용 가능한 채널 리스트
를 WE 후 기지국으로 전송

LO
@ 기지국은 단말로부터 전송 받은 채널 리스트를 기반으로 직교 자원 할당을 한 후 각
단말에게 채널을 할당
@ 할당 받은 채널을 통해 단말이 패킷 전송

위 O-@o 해당하는 VAS] 과정을 통해 각 APS 기지국으로부터 사용할 채널을 할
당 받게 되며, 일단 할당 받은 ae 새로운 채널 할당이 수행되기 전까지 패킷 전송에
사용된다.

 HDD 방식

HDD(Hybrid Division Duplex) 방식은 FDD(Frequency Division Duplex) 방식과
TDD(Time Division Duplex) 방식이 결합된 듀플렉싱 방식이다[202]. HDD 방식은 셀

348



===== PAGE 347 =====
Frequency

TDD UL/DL

FDD UL/TDD DL

Guard Time
FI
oo
FDD UL               F2
Time
(a) HDD 방식의 프레임 구조                (b) HDD 방식의 Al 구조

그림 8.9 HDD 방식의 프레임 구조 및 셀 구조

에서 TDD 방식을 사용하고, 셀 간에는 FDD 방식을 결합하여 인접 셀간 간섭을 최소화한
다. TDD 방식은 프레임 길이를 크게 하여 전송 ASS 높이면서도 전송 지연을 줄이고
고속 이동에 효과적으로 Hes    있는 장점이 있다.

그림 8.9(0)는 HDD 방식의 프레임 구조를 나타낸다. HDD 방식에서는 2개의 주파수

HAS 사용하는데, FLS TDD 방식을 위한 대역, 『2는 FDD 방식을 위한 대역을 나타낸
다. 그림 8.906)에서와 같이 HDD 방식에서는 하나의 셀을 안쪽 셀과 바깥쪽 셀로 구분한
다. 안쪽 셀에서는 전형적인 TDD 방식으로 상향)하향링크가 구성되어 있으며, 바깥쪽 셀

otf

에서는 하향링크는 1202 방식, 상향링크는 FDD 방식으로 수행한다. 이와 같은 주
은 안쪽 셀에서 상향링크, 하향링크 자원을 유    연하게 할당함으로써 TDDS 때
수 있으며, 110, RTGS 짧게 하여 TDD 방식의 효율을 증대시킬 수 있다. 또
셀에서 FDD 방식의 상향링크를 활용하여 프레임 길이를 길게 함으로써 ASH
= 얻을 주 있다.

그러나 그림 8.10의 예에 나타난 바와 같이, HDD 방식에서도 인접 셀간 송/수신 전환
시점이 다를 경우 일반적인 TOD 방식에서와 마찬가지로 간섭을 유발할 수 있다. 즉, 891
이 송신하는 데이터 버스트가 852에서 수신되는 경우가 발생하게 되며, 마찬가지로 MS2
가 송신하는 상향링크 데이터 버스트가 인접 셀의 MSA 수신되는 경우가 발생하게 된
다. 이러한 경우, 단말의 위치에 따른 스케줄링을 통하여 인접 셀간 간섭의 조정이 가능하
다[2031.

Ss
스

tho ofp
mS, fu
SW nt ^

06 bh ox mE
jay
ay

Je,
olN

x
rat

iN

349



===== PAGE 348 =====
PART ㅁㅁ OFDMZ} MATLAB

) cat
sk 고 | aa ©

y
eso Pome | (4       Fx        내 0612

0811                        0812                                                        Time
(a) HDD 방식에서 셀간 간섭           (b) HDD 방식에서 비동기시 프레임 구조
그림 8.10 HDD 방식에서 인접 셀간 간섭의 예

Frequency

GE 셀간 간섭 랜덤화 기법

 셀간 간섭의 랜덤화 원리

OFDM 시스템에서 셀내의 동기와 인접 셀간의 동기가 맞추어져 있는 경우, 모든 부반
송파는 직교성을 유지하기 때문에 각 부채널은 독립적으로 표시가 가능하다. 이러한 경
에 각 부채널에서 인접 셀로부터의 간섭신호는 시스템의 성능을 크게 열화시키기 때문에
간섭신호를 랜덤화할 필요가 있다. Cell—specific 인터리버(10[60ㅁ6861) 또는 0011-9060100
스크램블러(604801010)는 인접 셀로부터의 간섭을 랜덤화하여 셀간 간섭을 AWGN
(Additive White Gaussian 페0186)로 근사화한다[2041].

 주파수 영역에서의 OFDM 수신 신호는 식(8.1)과 같이 HAS 수 있다.

pull
fe)
<i

YER) = >. [R]-C[R]- X[K] + 2141                  (8.1)

m=0

여기서 ke 부반송파 인덱스, me 셀 인덱스, Me 인접 셀의 수, CME cell-
8060100 스크램블링 부호를 의미한다. 본 절에서 OFDM 심볼 인덱스는 수식의 간략화를
위하여 생략한다. 또한, CK] X[K] 는 m 번째 셀에서의 신호에 m 번째 셀 부호가
해진 ASS 의미한다. 단말이 서빙 받는 셀 인덱스를 0이라고 할 때, 원하는(0659460) 수

Al 신호와 인접 셀 간섭은 다음과 같이 표현된다.

fl

> oh

350



===== PAGE 349 =====
제8장_셀간 간섭 완화 기

li

Y[k] =H [k]-CO[k]- X[k] + ‘ HH [k]-C [k]: X[k] + Z[K]              (8.2)

m=1

여기서, HOUR) COTR XU] = 0번째 셀의 송신 신호에 스크램블링 부호가 곱해져
저그

채널을 통과한 수신 신호, DOA CMR XMAS 셀 인덱스 0을 제외한 4/-1
m=1

개의 인접 셀로부터 수신된 간섭 ASS 나타낸다. 단말의 수신단에서 역스크램블링 부호

를 수신 신호에 곱할 경우 다음과 같이 주어진다.

YOK] = C® [1714]
=H XU SC fe A -COR X UR 200 =

m=1

식(8.3)에서 CO [/]는 Al 인덱스 0에서 k BA 부반송파 인덱스의 역스크램블링 부호
의미한다. 역스크램블링을 통해 서빙 셀에서 수신된 신호는 AO [A] XOTK] O} 되어
크램블링 부호가 사라지게 되며, 74-1개의 인접 셀로부터 수신된 ASE
CO [k]- A [k]-C Tk] X[k] 가 되어 스크램블링 부호가 두 번 곱해진 형태로 남게
된다. 식(8.3)에서의 간섭 신호를 AWGNS =S 근사화하기 위해서는 간섭 신호 때 Gaussian
HES 가지며, i.i.d.(independent, identically distributed) AAS 만족해ㅇ

X™RE 성상도 상에서 제한된 크기의 균일004000)한 BES
H"[k] = Rayleigh 페이딩 채널 가정 시 Gaussian BES 갖는다. 그러나 ARE
채널의 coherence 대역 내에서는 강한 상관도를 갖기 때문에 부채널간 독립적인 채널로
보기 어렵다. 이 경우 <”"[/]를 통하여 인접 대역간 상관도를 크게 낮출 수 있으며, 스크
램블링 부호는 인접 셀간 간섭을 AWGNL= 화이트닝(\1160108)하는 역

셀에서 송신한 ASE 수신 ASS 역스크램블링하여 얻을 수 있고, 이 때 인접 셀 간섭은

AWGN2 2 근사화가 가능하다.

1> mf

 Cell-Specific ABBEY 기법

Cell-specific ABBAS 유니캐스트04010890 AS 상황에서 인접 셀간 간섭을 화이
Ey 하는 기법이다. 0611-82060100 스크램블링의 원리는 A 절에서 살펴본 바와 같이 인

351 |



===== PAGE 350 =====
PART Il_ OFDM} MATLAB

접 셀이 각자 다른 스크램블링 부호를 송신하는 신호에 곱하
키는 데 있으며, 이 경우에 셀간 간섭에 강           할

블링이 존재하지 않는 경우, 단말기의 복호기는 원하는 Ase      라 인접 셀로부터
신된 신호까지 복호화하기 때문에 성능 열화가 발생한다. 스크램블링 기법은 확산
(spreading) 기법과는 달리 대역을 증가시키지 않지만, 부호기와 함께 사용시에는 부호율
에 따른 확산 이득도 함께 얻을 수 있다. 2H 8.112 cell-specific AABSY 기법의 일
반적인 블록도를 보여준다[205].

nz
eS
es

섭을 화이트닝 시

}

ell—specific 스크

{r
a se
o -꾸
i 6

|>
oe

Cell A

— >} Encoder | 처 Interleaver  (60 >
Scrambling

Cell 8                          Gade

— > Encoder [> Interleaver 0 >
Scrambling

code B

그림 8.11 Cell-specific AB#tS2! 기법

QV Cell-Specific 인터리빙 기법

Cell—specific 인터리빙 기법은 일반적으로 IDMA(Interleaved Division Multiple Access)
기법으로 불린다[206]. IDMA 기법은 단일 사용자 수신기를 VARS 경우, 인접 ale] 간섭
을 화이트닝 시킨다는 관점에서 6011-6060100 스크램블링 기법과 유사하다. 0611-9060180
스크램블링 기법은 각 셀에서 특정한 스크램블링 HSS 사용하여 인접 셀간 간섭을 화이트
닝 시키는 데 반해, IDMA 기법은 각 셀에서 특정한 인터리버를 사용하여 셀간 간섭을 화이
트닝 한다. IDMA 기법에서 수신단에 다중 사용자 수신기를 사용할 경우, 반복적인 복호화
를 통해 간섭을 효과적으로 AAS 수 있으며 6011-8060100 스크램블링에 비해 훨씬 큰 이
득을 얻을 수 있다.

그림 8.12는 하향링크에서 6011-8060180 인터리빙 기법을 적용한 경우를 보여준다. of
기서 단말기 MS1s} MS2%= 각각 기지국 891과 852에 속해 있으며 같은 부채널 대역을
사용한다. 851이 인터리빙 패턴 1을 사용하고, 882가 인터리빙 패턴 2
1451(또는 1452)는 각자 해당 기지국의 인터리버를 사용하여 신호를 복호한다. 단일 사용
자 수신기를 사용하는 경우, 인접 기지국으로부터의 간섭은 4\0취로 근사화된다.

4

352



===== PAGE 351 =====
signal transmitted
by BS2 for MS2

signal transmitted by BS1 for MS1
그림 8.12 Cell-specific 인터리빙 기법

066 주파수 호핑 기법
FH(Frequency Hopping)-OFDMA 기법은 일정한 패턴을 가지고 시간 슬롯에 따라서
HAA 대역이 주파수영역에서 호핑함으로써 주파수 선택적 페이딩 채널에서 버스트 에러
를 극복하거나 주파수 다이버시티 SS 얻는 기법이다[207]. 또한, OFDMA 셀룰러 시
스템에서 셀 마다 다른 패턴을 가지고 호핑할 경우에 셀간 간섭을 평균화시키는 효과를
oj
의

을 수 있다. 이 경우 수신단에서 복호화를 위해서는 한 호핑 패턴을 구성하는 시간 슬롯
데이터를 모두 버퍼링에 해야 하기 때문에 큰 크기의 메모리가 소요되는 단점이 있다.
그림 8.13(0)는 FH-OFDMA 시스템에서 시간 슬롯에 따라서 데이터 버스트가 사용하
는 주파수 대역이 호핑하는 예를 보여준다. 이 그림에서 버스트 Ar 시간 슬롯 3에서 인
접 셀의 간섭을 받게 되나, 다른 시간 슬롯에서는 다른 호핑 패턴에 의해 간섭이 발생하지

channel             channel            channel            channel             channel                f

;  c=}   Ss
/                        ~
/
i
/

Frequency

j
interference
i
i

|     |     |     |     |
V'timesit1  ' timesit1 |! timesiott |! timesiott | timesiot1

>|

(a) 시간 슬롯에 따른 주파수 호핑의 예

그림 8.13 FH-OFDMA 기법의 예



===== PAGE 352 =====
PART 야미 과 MATLAB

알수 있다. 이 정우  수신단에서 복호화를 통하여 버스트로 발생한 인접 셀간

슬롯 5에서와 같이 SYS 한 데이터 버스트가 Way} A
한 피이딩(8680 feding) 빠지게 되어 무선 채널에 의하여 버스트 에라가 발생하는 경우
에도 AAS 랜덤화시킨다. 그림 8.13(0)는 버스트에 따른 주파수 호핑 패턴의 다른 예를
보여준다.

랜덤 부반송파 할당 기법

부반송파 할당 기법에서는 하나의 부채널을 구성하는 부반송파들이 전 대역에 걸
넘하게 퍼져있기 때문에 다이버시티 이득과 간섭의 랜덤화 효과를 얻을 수 있다. a
송파 할당은 Reed-Solomon 부호 등을 사용하여 발생한 랜덤 부반송파 할
라 데이터 부반송파를 전대역에 퍼뜨려 할당하는 방식이다. 셀마   _
을 사용하여 랜덤한 인덱스를 생성하며, 이에 따라 맵핑된 데이터 버스트는 인

부반송파 충돌(00116100)을 최소화한다. 그림 8.14는 OFDMA 셀룰러 시스템에서 랜덤 부
반송파 할당 기법의 예를 보여 준다. 이 그림에서 8개의 인접한 셀을 고려하였으며 셀간에
충돌이 발생한 부반송파를 “0:으로 표시하였다. 여기서는 8개의 셀 중에 어떤 Alo] 인접하
더라도 2개의 부반송파에서만 충돌이 발생하여 셀간 간섭을 최소화하는 예를 보여준다.

2

|

=

re,   (에
에 rim off
또 fe pe
ro N 므

&

CellO 0611 Cell2 _ 061 3 Cell4 Cell5 0616 061 7

Frequency
~

그림 8.14 OFDMA 셀룰러 시스템에서 랜덤 부반송파 할당 기법의 ofl

354



===== PAGE 353 =====
제8장_셀간 간섭 완화 기법

랜덤 부반송파 할당 7) FH-OFDMAS} 비교하여 프레임 단위에서 볼 때에 Bee
유사하나, FH-OFDMAS$} 달리 수신단에서 OFDM 심볼 단위로 복호화가 가능하기 때문
에 버퍼링을 위하여 큰 크기의 메모리가 필요하지 않다는 장점이 있다. 와이브로 시스템
에서 이와 같이 데이터를 랜덤 부반송파에 할당하는 경우를 다이버시티 모드라고 부르고
permutation 10001418에 의해 랜덤 부반송파를 생성한다. 하향링크 PUSC, FUSC,
O-PUSC, 상향링크 2080 등이 이에 해당한다[208]. 와이브로 시스템의 랜덤 부반송파
할당 기법에 대해서는 18장에서 자세히 설명한다.

CP setae 00

00 interference Rejection Combining 기법

수신단에서 다중 안테나를 사용하여 얻을 수 YE 공간적 특성을 이용하여 인접 셀간
간섭의 제거가 가능하다. IRC(Interference Rejection Combining) 기법은 단말에서 다중
안테나를 사용하는 경우, 단말의 안테나에서 수신되는 동일채널 간섭(60-0000061
interference) 상관을 이용하여 인접 셀간 간섭을 제거하는 기법이다. 는 일반적인
MRC(Maximum Ratio Combining)o] 추가적으로 수신 신호의 공간적 BAS 고려하는
개념으로 볼 수 있으며, 이에 따라 수신단에서의 간섭 제거가 가능하다[209]. 즉, IRCE
채널, 잡음, 간섭의 covariance YAS 기반으로 600ㅁ61008 계수를 구하며, 이 경우에 간

섭의 전력뿐만 아니라 간섭의 공간적 0010008까지 고려 가능하다.

Rr,

Tx ]
X(k)—> Transmitter        L 은 AB  Y,(k)

Re,   :    Pg Detector | ¥(k)
| 4
Yy(k)

dio
Noise                                            Recevi M

Adjacent Cell
Interference

그림 8.15 IRC 기법의 개요

355 _



===== PAGE 354 =====
PART _야미/과 MATLAB

그림 8.15에 주어진 M 개의 안테나로 구성된 수신단을 가정할 경우에 각 안테나에 수
신된 신호는 식(8.4)와 같이 정의된다.

Y[k] = H[k]- X[k] + Z[A]
H[k]=[4, [A] 4, [k]--- A, [A]
Z[k]=[Z,[k]Z,[k]---Z yk]
Q= E{Z[k]-Z"[k}}

(8.4)

여기서, ZK = 잡음과 인접 셀의 간섭을 모두 포함하는 벡터이다. QE ZA
상호상관 YALA we]s SS 사용하여 추정한 채널 ga} 수신 ASS] 차이를 이용하여
식 (8.9)와 같이 정의할 수 있다.

0= > (vt —H[k]- X[k])-(¥[]— [A]: Xl)                           (8.5)

k=0

위 식에 나타난 바와 같이 Z[k] 2] 상호 상관 QL coherence 대역폭 내의 K 개 부반
송파에 대하여 평균을 취하여 구할 수 있다. 모든 수신 신호가 동일한
될 경우에 송신 신호의 ML(Maximum Likelihood) = 다음과 같이 주어진다.

~(Y[A]- ALA] X[k   Y[k]-A[k]-X[k
k]=argmax [] xe       ALA) X[K)” 7 (Yd AEAT-XTA])

=argmin 9°(Y [k]- H[k]- X{k]).  Q"(Y[k]- 비시)

OR] 다중 사용자 수신기를 갖는 IDA 기법

셀간 간섭 랜덤화 기법에서 설명한 IDMA 기법에서는 단일 사용자 수신기를 사용하고
AAS 잡음으로 취급한다. 그러나 다중 사용자 수신기를 갖는 IDMA 기법에서는 원하는
신호와 함께 간섭 신호도 복조를 수행하여 원하는 신호에 대한 검출 성능을 향상시킨다
[206]. 특히 다중 사용자 수신기에서 반복적으로 간섭신호를 제거하고 복호화하여 반복

횟수의 증가함에 따라 성능 향상이 이루어진다. 그림 8.16은 다중 사용자 수신기를 갖는
IDMA 기법의 반복적인 간섭 제거 방식의 블록도를 보여준다.

356


===== PAGE 355 =====
제8장_셀간 간섭 완화 기법

80)
y
Decoder 0          To!    <—

기          ㅁ2

Oo
H                           =

                  35 ~-   FFT

                         es
pee 1)                                             Bo

fe}

Decoder M-1               Tae      —
기        TM-1

:
0

그림 8.16 다중 사용자 수신기를 갖는 1044 기법의 반복적 간섭 제거 블록도

그림 8.16에 나타난 바와 같이 반복적 다중 사용자 수신기는 크게 반복적 간섭 제거부

반복적 복호부로 Use} 수신단에 입력된 신호 는 FFTS 통과한 후 다중 사용자 복
조기로 입력된다. 입력된 ASE 다중 사용자 복조기(074104867 0601001418101)를 거친 후
0611-9060100한 역인터리버(※, )와 비트 복호기(0600060)를 통과하게 된다. 복호기를 통
해 복호된 HESS cell—specifics 인터리버(※, )를 거친 후 다시 다중 사용자 복조기로
입력되어 간섭 신호의 제거에 사용된다. 즉, 74개의 복조기 입력 중 서빙 셀에 대한 신호
1개를 제외한 나머지 17-1개는 모두 간섭 신호이므로, 47-1개의 간섭신호를 제거하게
된다. 이 과정을 통해 출력된 신호는 다시 역인터리버를 거치게 되며 복호 후 더욱 신뢰성
있는 신호가 된다.

그림 8.17은 다중 사용자 수신기를 갖는 12044 기법의 반복적 제거 및 복호화 예를 보
여준다. 이 그림에서 A 1의 신호가 원하는 신호이고, 셀 2의 신호가 인접 셀의 간섭이라
고 가정한다. 그림 8.17에서 셀 1에 신뢰도가 저하되는 비트가 존재하는 경우(8), 이를 다
시 부호화(6)와 인터리빙(0) 하여 다중 사용자 복조기에서 그 입력 신호를 제거한다(0). 그
후 A} 2의 인터리빙 sao] 따라 역인터리빙 후 복호화하게 되면 더욱 정확한 셀 2의 비
트열이 BASIC). 여기까지가 1번의 반복이 되며, 이 비트열을 다시 부호화와 인터리빙
을 거친 후 다중 사용자 복조기에서 제거하면 더욱 셀 1에 적합한 신호가 생성된다. 이를
역인터리빙
(6)에서와 ZO} cell-specificg 인터리빙 패턴을 인접 셀에서 사용하지 않는 경우에는 역
인터리빙을 하더라도 같은 패턴으로 인하여 간섭의 랜덤화가 이루어지지 않게 되어 복호
화 시 신뢰도가 저하되는 비트를 얻게 된다.

sor              ：



===== PAGE 356 =====
PART ㄴㄴ OFDMZ} MATLAB

Unreliable information bits
a | | | | 를 | | | | | | | | 1091

Unreliable coded bits

(b) After Re-encoding | | | | 이이 [| 1} | |  | | Cell 1

Unreliable coded bits

(c) After Re-interleaving
(for Cell)                                                                                                                     Cell 1

Unreliable coded bits

(d) After interleaving  [ 로 fen

;                                                                                           Cell 2
cancellation
Unreliable coded bits.
(adjacent, bad for decording)
(6) After De~interleaving
(Non-cell specific)                                                                                              Cell 2
Unreliable coded bits
(distributed, good for decording)
(f) After De-interleaving                                                                                     Cell 2

(Cell specific)

그림 8.17 다중 사용자 수신기를 갖는 IDMA 기법의 반복적 제거 및 복호화 예

358


===== PAGE 357 =====
PART Ii

MIMO2} MATLAB

제 9 장 MIMO 채널 용량

제ｌ10장 공간 다이버시티와 시공간   부호화 기범

제장 공간 다중화 MIMO 시스템의 Al    !호검출 기법

제12장 다이버시티-다중화 Trade-off 시공간 부호화 기법
제13장 채널 PHS 활용한 송신 기법

제14장 다중 사용자 MIMO 기법



===== PAGE 358 =====
다중안테나 기술은 송수신 양단에 다중안테나를 사용함으로써 한정된 주파수 자원 및

신전력을 이용하여 채널 용량을 증대시킨다. 다중 송수신 안테나를 이용하는 레이더 기
, 수중 공간에서의 AU(SONAR) 기술, 무선 통신 시스템의 빔형성(6680000108) 기법
이 예전부터 연구되어 왔으며, 최근 무선 통신 시스템의 용량 증대에 대한 요구가 증가
되면서 이러한 다중안테나 기술 Apo] 관심이 집중되고 있다[210][211].

다중안테나 기술은 각 송신 안테나로부터 독립적인 데이터를 동시에 전송함으로써 고
속으로 데이터를 전송하는 공간 다중화(608081 multiplexing) 기술과 여러 개의 송신 안테
나에서 같은 데이터를 내포하는 ASS 전송하여 송신 다이버시티(ㅠ805011 diversity)S
얻는 전송 다이버시티 기술로 구분된다[211]-[214]. 공간 다중화 기법을 사용했을 때의
채널 용량(0100061 0808016/)은 Shannon2] 채널 용량과 동일하지만, 송신 다이버시티 기
WS 사용한 경우의 채널 용량은 이보다 작게 된다. 페이딩 채널의 영향을 감쇄하여
AWGN 채널과 유사하도록 변형하는 것이 다이버시티 기법의 목표이므로, SISO 비교
할 때 가상 통신 ARS 여러 개 발생하기보다 단일 채널의 페이딩이 AES 한다고 할
수 있다. 따라서, 다이버시티 기법을 사용하면 9190에 비해 채널 용량이 미미하게 증가하
며, 9씨이 높아질수록 공간 다중화 기법 사용시보다 채널 용량이 현격하게 감소한다
[215]. 이러한 두 가지 기술들은 각각 다시 송신기에서 채널 정보의 가용 여부에 따라 개
루프(0000 loop) 방식과 폐루프(00960 loop) 방식으로 나된다.

본 장에서는 MIMO 무선 채널의 용량을 기술한다. 먼저 MIMO 채널 용량 표현에 자주
사용되는 행렬 기본 이론을 알아본다.

oft ty of

361


===== PAGE 359 =====
PART IH_ MIMO} MATLAB

GW ve 212 112

Rank7} ro] 행렬 HE ㅇ"^"?7?의 Svp(Singular Value Decomposition)= 다음과 같
이 주어진다.

H=Uxv"                                          (9.1)

여기서, UEC’ ola, VE ㅇ"이며, U"U=V"VE=I,, L=diag{a,,c,,---,0,},
0,2 6,,, i=1,2,....r-lo]t}. 버 의 SVD 2 eigen-decompositionz} 관련된다.

HH” = QAQ”                  (9.2)

여기서, QW Q=QQ"=Hy,, A=diag{hy,Ays..2y,}, 2,20 이다. 식 (9.1)과 (9.2)의 관계
를 통해, Q=U Oz, 다음의 관계가 성립한다.

4=

1

O7, ifi=1,2,-,r
(9.3)

0,   if i=rtl,--+,ny,

MIMO 채널의 squared Frobenious norm MIMO 채널의 전체 전력이득으로 해석할
수 있고, 채널 용량 표현 식에 자주 쓰이며 다음과 같이 다양한 형태로 표현이 가능하다.

[si = Tec’) =a. | =D

i=l

8. =[i"|, Joao", =Ial, 04

(QP veterministic MIMO 채널 용량

9.1절의 기본 행렬 이론을 사용하여, 다중안테나에 의해 구현되는 채널이 고정되었을
때의 채널 용량을 알아본다. 송수신 신호 관계는 다음과 같이 표현할 수 있다.

362



===== PAGE 360 =====
제9장_ MIMO 채널 용량

Nr          Np
VV           Vv

1X          x          RX
VV                        VV

H

그림 9.1 MIMO 시스템

E
y=   WN. Hx+z                                    (9.5)
T

여기서, ye 6” 는 수신신호 벡터를 나타내고, HE CPN 채널이득 행렬을 나타
내며, xe 6 "는 송신신호 eS 나타낸다. 송신신호의 자기상관 YAS 아래와 같이
정의한다.

R,, =E {xx}                                                  (9.6)

4 송신안테나에서 송신된 신호의 전력을 1이라고 가정할 때 Tr(R,,) =N, 가 성립한
다. 잡음벡터는 2 ㅇㄷ”“^'로 표현되고, 일반적으로 ZMCSCG(Zero Mean Circularly
Symmetric Complex (484891320)이라 가정된다.

 송신부에 채널 정보가 가용하지 않을 때의 채널 용량
Deterministic 채널의 용량은 아래 수식으로 표현된다.
C=maxi(@y)                          (9.7)
여기서, /(3)는 송신벡터의 확률밀도함수를 나타내고, [aye 벡터와 벡터*사이의
mutual informationS 나타낸다. 즉 채널 용량은 송신벡터의 확률밀도함수를 변화시켜 a

을 수 있는 두 벡터 사이의 최대 mutual 10[0008400이다. 두 벡터가 주어질 때 mutual
information® 아래 수식으로 표현된다.

363


===== PAGE 361 =====
PART Il MIMO2} MATLAB

I(x:y)= H(y) - H(y|x)                                  (9.8)

여기서, Hy) yo 차등 EZ 5\(differential entropyyS 나타내고. A(y|) = x 7}
주어졌을 때 *의 AAS 차등 MEL 5 (conditional differential entropy)S 나타낸다. 랜
덤 변수 2와 x7} 독립이기 때문에 아래의 관계가 성립한다.

H(y|x) = H(z)                                                 (9.9)

I(xsy) = H(y)— H(z)                                           (9.10)

A} (9.10)에 의해 표현되는 mutual informations 최대화하기 위해서는 A(z) 가 상수이

므로, 2(*)를 최대화해야 한다. 결론적으로, 는 Gaussian 랜덤 벡터이어야 한다. 이러

할 때 엔트로피는 아래와 같다.

H(y)=log, (det(zeR,, )) bps/Hz                                               (9.11)

H(z) =log,(det(zeN I " )) bps/Hz                                            (9.12)

여기서, R,, =667"]=은 HRA" +, 이다. 식 (9.11)과 식 (9.12)를 식 (9.10)에
대입하면 mutual information /(x;y) 는 아래와 같게 된다[216].

I(xy) = log, det(Iy, + =

Y Meee

HR ,,H") bps/Hz                            (9.13)

따라서 deterministic MIMO 채널 용량은 아래와 같다.

ㄴㄴ                                      E.                H
@ - 6 108.0아(1, + 수 자  HR,” ) bps/Hz                            (9.14)

oe)

송신부에서 채널 정보를 사용할 수 없을 때에는 각 안테나에서 전송되는 신호가 동일한
전력을 갖도록 하는 것이 최선이다.

_ 364



===== PAGE 362 =====
제9장_ MIMO 채널 용량

"                              R,.=1y,                               (9.15)
위의 경우에 채널 용량은 아래와 같다
E      ^”
C=tog det 1, +——— HH |               (9.16)
"  ^,  0

Eigen—decomposition HH” = QAQ” 와 관계식 det(I,, +AB) =det(I,+BA) (AE
6", BEC™™)S 사용하면 위의 채널 용량이 아래와 같이 표현된다.

^                                   E.
C=log, te 1, ae:     040" = log, te 1, + NN, 시

1 @

4)                                                     (9.17)

.                   E
=  > log,   1+—>
i=l              NN,

A] (9.17)을 관찰하면 다중 안테나를 사용하여 rv HS] 가상적인 SISO 채널이 생성되고,
각 SISO 채널의 이득은 이고, 송신전력은 &./4&, 임을 알 수 있다.

채널의 전체 전력이득이 제한되어 있고, 즉,    200 이고, H 2] full rank= 가
한다. N,=N,=N 이면, r=N 이고, 이 때 채널 용량을 최대로 하는 채널 VAS 다음

만쪽한다.

ttlo od

A,=6/N,i=1,2,--,N                    (9.18)

따라서, 채널 행렬이 직교행렬일 때, 채널 용량이 최대가 되고, 9150 채널 용량의 way
가 된다.

HH” =H" H-=1,                                    (9.19)

CE.
=Nlog,| + 으으
18     ce, ve 7                              (9.20)

365



===== PAGE 363 =====
PART If__ MIMO2} MATLAB

Transmitter       Channel            Receiver

==> + pe H 빠
x   ‘|

그림 9.2 송신부에 채널 정보가 가용할 때 modal decomposition 수행

2
y           y

송신부에 채널 정보가 가용할 때의 채널 용량
송신부에서 채널 정보의 활용이 가능할 때 송수신 관계를 그림 9.2에 나타난 바와 같이
분해해서 표현할 수 있다.

jy =  스 0081 0"2 = |스 > x+2             (9.22)
N,             iN

Tr[E{xx”}]=N;                                              (9.23)

결과적으로 그림 9.3에 나타난 바와 같이 가상적인 /개 SISO BYE 분해할 수 있다.

&

그림 9.3 Modal decompositionS 수행해서 얻은 / 개의 가상 채널

366



===== PAGE 364 =====
AOS MIMO 채널 용량

y= a '/ i=1,2,---57.              (9.24)
전체 채널 용량은 그림 9.39] 가상 채널 용량의 합과 같으며 아래 식으로 표현된다.
C=) log,| 1+ㅡ프티,                       2

r

여기서 7, = Ex] } 6=1.2,…,/) 은 번째 송신 안테나의 전력이고 Dy =Ne&

만족해야 한다. 식 (9.25)에서 > =1, 1=1,2,...,7 인 경우가 A] (9.17)임을 알 수 있고, 송

신단에서 채널 정보가 가용하지 않아, 각 안테나에서 동일한 송신전력으로 송신할 때를
용량

의미한다. 전체 전력이 제한되고, 채널 정보가 송신부에 가용할 때, 채널    은 아래와
같다.
C= max  Soe, (1+ Bde Ah 4)                  (9.26)
20 2707 i=l       N,No
최적 전력 할당 해는 water—pouring 기법을 사용해 구할 수 있고, 아래와 같이 표현된다.
pt __   _N-N,    =] ,,,
^ = ,  EA |. i=leyr                  (9.27)
Sy =n,                                              (9.28)

i=]

여기서 WS 상수이고 00, 은 다음과 같이 정의된다.

_| x if x20
=| 0 if x<0                    (9.29)



===== PAGE 365 =====
PART 141 MIMO2} MATLAB

OAS 모드
사용 모드                               \
ye | oe
yr       :
1                      비해     N,N,     N,N,
LU                                          EX      EA,
N,N,     a
N,N,     EX,      a2
Eh,

그림 9.4 Water—pouring 알고리즘의 예

그림 9.4는 water—pouring 기법을 사용한 전
SNR°] 높은 곳에 더 많은 전력을 할당하고 있음

wie “나

력할당 예를 나타낸다. 그림 9.4를 통해
음을 알 수 있다. SNRO] 작은 채널에는
신전력이 할당되지 않고, 이는 사용하지 않는다는 의미이다. 최적 06000108행렬은 다음과
같다.

x= Vx                               (9.30)

송신부의 precoding 이후 각 안테나에서 송신되는 신호 x 2] covariance YAS 아래와
같다.

요미 =VREV"                                                        (9.31)

R® = 01817.) ,… 72}                (9.32)

 SIMO} MISO 채널 용량

SIMO 채널의  배트 hec’**™ r= 그리고 ㅅ크피,이므로 송신부에서 채널
정보의 가용 여부에 상관없이 다음이 성립한다.

Csrmo = rae                             (933)

oO



===== PAGE 366 =====
제9장_ MIMO 채널 용량

만약 || =1, 7=1.2.…,, 이면 fal =, 이므로 다음식이 성립된다.

E.
Oras, nik                          (9.34)

MISO 채널의 경우에는, heC™ojue 7=1이고 ㅅㅋ|비, 이므로 송신부에 채널 정
보가 가용하지 않을 때 채널 용량은 아래와 같다.

Fay
Curso,o1 = log, “ NON, ot                         (9.35)
수식 (9.35)를 관찰하면 SISO 경우와 채널 용량이 동일하다는 것을 알 수 있다. 송신
부에 채널 정보가 가용하면, 모든 ag 그 해당하는 공간모드로 집중할 + 있고, 채널
BS 91540의 채널 용량과 동일하게 된다.
Curts0.ct = x,          4                               (9.36)

GE) we vivo 채널 a9

9.2절에서는 무선 채널이 고정되어 있다고 가정하였으나, 실제 무선채널은 일반적으
불규칙하게 변한다. 채널 행렬 떼가 랜덤 변수라면, 이에 따라 채널 용량도 랜덤 변수가
된다. 자주 사용되는 두 가지 통계적 채널 용량으로 A] (9.37)로 나타내어지는 680016 채
널 용량과 식 (9.38)2] outage 재널 용량이 있다.

369

EE OOS


===== PAGE 367 =====
PART 4 MIMOSt MATLAB

C=E{C}                                                (9.37)

P(CSC,,, )=q%           (9.38)

out .q

도

A] (9.37)로 표현되는 80010 채널 QO 랜덤 채널에 해당하는 채널 용량을 통계적
평균을 취한 값으로서 다시 송신부에서 채널 정보의 가용 여부에 따라 두 가지 채널 용량
이 있다. 송신부에 채널 정보가 가용하지 않을 때 즉 개루프의 경우에는 채널 용량이 아래
와 같다.

"0

_       r         E
C,, =E    ㅣ    1     x.                         9.39
OL   1 og,( V7 N  >}                       (    )

A] (9.38)로 표현되는 채널 SES q% outage 채널 용량이라 하고, 랜덤 변수 C7}
ㅇ0. 보다 작을 확률이 0%임을 의미한다. 그림 9.5는 94#&=10008이고 채널 정보가 송신
부에 가용하지 않을 때의 채널 용량 CDF(Cumulative Distribution 【140001027)로서, 2x2 및
4x4 MIMO 42° ergodic 채널 Sts} outage 채널 BSS 보여주며, 이를 그려 주는
프로그램 9.1(“Ergodic_ Capacity CDF.m’)-2 다음과 같다.

0와우일 Posen pase Pen eeedoeuceaeenes
O64) SR ener ee ee ee ee
_    Ergodic;Capacily"/ ~~;    {    |
의     |    | /써    |    |    !    |    |
-
1     |    ;    |    ;    {    {    |    H
0사가느} eee
|    :    |    {    :        Ny = Np =2
—  N,j=N,=4
02 eee ae                 =
| 보테 으으 이브 22022
:       |         10% ie 090
f    |    |    ~  |    |    |
0         i         1    1    i

2 4 6 8 10 120 14 16 18
Rate (bps/Hz)

그림 9.5 i.i,d(independent identical distributed) Rayleigh 페이딩 채널
(SNR=10aB, 송신부에 채널 정보가 가용하지 않은 경우)

370



===== PAGE 368 =====
제9장_/140 채널 용량

% Ergodic Capacity _CDF.m
clear all, close all
SNR_dB=10; SNR_linear=10.*(SNR_dB/10.) ;
N iter=50000; sq2=sqrt (0.5); grps = ['b:'; 'b-'];
for Iter=1:2
1f Iteér=-1, nT=2; nR=2; % 2x2
else nT=4; nR=4;       % 4x4
end
n=min(nT,nR); I = eye(n);
for iter=1:N iter
H = sq2* (randn(nR,nT)+j*randn(nR,nT) ) ;
C(iter) = 1092 (real (det (I+SNR_linear/nT*H'*H) ) ) ;
end
[PDF,Rate] = hist(C,50);
PDF = PDF/N_iter;
for i=1:50, CDF(Iter,i) = sum(PDF([1:1i])); end
plot (Rate, CDF(Iter,:),grps(Iter,:)); hold on
end
xlabel('Rate (bps/Hz)'); ylabel('CDF')
axis([1 18 0 1] ) ; grid on; set(gca,'fontsize',10);
legend('{\it N Th={\it N_R}=2','{\it N_T}+{\it N R}=4');

i) 프로그램 9.1 Ergodic 채널 용량 실행 프로그램

그림 9.6은 SNR 변화에 w= ergodic 채널 용량을 나타내며, 이를 그려주는 MATLAB

프로그램이 다음 프로그램 9.2(“Ergodic Capacity vs_SNR.m’)°|CH.

371



===== PAGE 369 =====
PART 비 MIMO2} MATLAB

25

—O~ Np=1 Np=1
20-4 —f— Ap=1 Np=2
—&- N,;=2 N,=1

|—— N,=2 Np=2

ee ee ee ee

15       20

10
SNR [08]
그림 9.6 채널 정보가 송신부에 가용하지 않을 때의 90010 채널 용량

% Ergodic Capacity vs SNR.m

clear all, close all

SNR_dB=[0:5:20]; SNR_linear=10.*(SNR_dB/10.) ;
N_iter=1000;

198 Teéra1:5

if Iter==1, nT=1; nR=1; Txt
elseif Iter==2, nT=1; mnR=2; % 1x2
elseif Iter==3, nT=2; mnR=1; % 2x1
elseif Iter==4, nT=2; mnR=2; % 2x2
else nT=4; nR=4;          % 4x4

end
n=min(nT,nR); I = eye(n);
C(Iter,:) = zeros(1,length(SNR_dB)) ;
for iter=1:N_ iter

H = sqrt (0.5) * (randn(nR,nT)+j*randn(nR,nT));

if nR>=nT, HH = H'*H; else HH = H*H'; end

for i=1:length(SNR_dB) srandom channel generation

C(Iter,i) = C(Iter,i) +log2 (real (det (I+SNR_linear (i) /nT*HH) ) ) ;

end
end
end
C = C/N iter;
plot (SNR_dB,C(1,:),'b-o', SNR_dB,C(2,:),'b-<', SNR_GB,C(3,:),'b-s');
hold on, plot (SNR_dB,C(4,:),'b->', SNR_GB,C(5,:),'b-*');

xlabel('SNR [dB]'); ylabel ('bps/Hz') ;

ig! 프로그램 9.2 SNR 변화에 따른 ergodic 채널 용량 실행 프로그램

372

| ^ ＊》《《 ＊ 』7712



===== PAGE 370 =====
HJOzt MIMO 채널 용량

송신부에 채널 정보가 가용할 때 즉 폐루프(00600 1000)의 경우에는 채널 용량이 아래
와 같다.

=07 j=l

Ca =  Slows        yA }                          (9.40)

i=l  i

=F) Does         KPA, ;                                     (9.41)

i=l

그림 9.7은 HA 4x4 MIMO 채널의 경우 채널 정보의 가용 여부에 따른 80010 채널 용량
을 비교하며, 이를 그려 주는 MATLAB 프로그램은 프로그램 9.3 ““OL_CL_Comparison.m”)
과 9.4(“Water_Pouring.m’”)°] TH.

29

-ㅡ@- Channel Unknown
—+ Channel Known

20
15
=
n
용
이 에그
이 202                 |               |
%              5              10             15             20
SNR [08]

그림 9.7 ergodic 채널 용량 (N,; =N, =4)

%OL_CL_Comparison.m
clear all, close all;
SNR_dB=[0:5:20]; SNR_linear=10.*(SNR_dB/10.); rho=0.2;

Rtx= [1           rho       rho*2 rho*3; rho        1           rho rho*2;
rho*2 rho     1        rho;     rho*3. rho*2 rho 1];
Rrx=[1          rho      rho*2 rho*3; rho        1          rho rho*2;
rho*2 rho     1        rho;     rho*3  rho*2 rho 1];

373



===== PAGE 371 =====
PART 1 41140 와 MATLAB

N_Iter=1000;
nT=4; nR=4; n=min(nT,nR); I = eye(n); % 4x4
C_44 OL=zeros(1,length(SNR_dB)); C_44 CL=zeros(1,length(SNR_dB));
for Iter=1:N Iter
Hw = sqrt (0.5)*randn(4,4) + j*sqrt(0.5)*randn (4,4) ;
H = Rrx* (1/2) *Hw*Rtx* (1/2); tmp = H'*H/nT;
for i=1:length(SNR_dB) %random channel generation
C_44 OL(i) = C_44 OL(i)+log2 (det (I+SNR_linear(i)*tmp)); %(9.39)
SV = svd(H'*H); Gamma = Water _Pouring(SV,SNR_linear(i) ,nT) ;
C_44 CL(i) = C 44 CL(i) +
log2 (det (I+SNR_linear (i) /nT*diag (Gamma) *diag(SV))); %(9.41)
end
end
C_44 OL = real(C_44 OL)/N_Iter; C_44 CL = real(C_44 CL)/N Iter;
plot (SNR_dB, C_44 OL,'-o', SNR_GB, C_44 CL,'-<');

i 프로그램 9.3 채널 정보의 가용 여부에 따른 90006 채널 용량 실행 프로그램

function [Gamma] =Water_Pouring(Lamda, 9피묘,27)
Gamma=zeros (1, length (Lamda) ) ;
r=length (Lamda) ;

index=[1:r]; index_temp=index;
p=1;
while pcr

irp=1:r-p+1; temp = sum(1./Lamda(index_temp(irp)));
mu = nT/ (r-p+1) * (1+1/SNR*temp) ;
Gamma (index_temp(irp)) = mu - nT./(SNR*Lamda(index_temp(irp)));
if min (Gamma (index_temp) ) <0
i=find (Gamma==min (Gamma) ) ;
ii=find(index_temp==i) ;
index_temp2=[index_temp([1:ii-1]) index_temp([ii+1:end])];
clear index_temp;
index_temp=index_temp2;
p=ptl;
clear Gamma;

else
p=r;
end

 374



===== PAGE 372 =====
제9장_ MIMO 채널 용량

end

Gamma_t=zeros (1, length (Lamda) ) ;
Gamma_t (index_temp) =Gamma (index_temp) ;
Gamma=Gamma_t;

Tm! 프로그램 9.4 Water—pouring 함수

그림 9.7로부터 SNRO] 높을 때는 송신부에서 채널 정보가 가용해도 큰 이득이 WSS
확인할 수 배서 SNR} 매우 높을 때에는 가장 낮은 모드의 SNR) 높아, 사용되지 않
HE?        , 채널 정보에 따라 각 모드가 할당 받는 AGE 거의 동일하게 BS 의미
다.

MIMO 채널의 러키 르 따른 채널 용량 변화를 알아본다. Deterministic 채널 용량
수식으로부터, SNR] 높을 때 다음 식으로 DAB 할 수 있다.

원

ro cir

E.           A
C= tes log, det(R,.)+log, det ( NN HH; )                             (9.42)

위 수식으로부터 det(R,,) 가 최대가 되기 위해서는 조건 R,=1y 이 만족되어야 함을
알 수 있다. 상관관계가 있는 MIMO 채널을 식 (9.43)과 같이 모델링하면, 해당 채널 용
량은 식 (9.44)와 같이 표현된다.

H=R 7H, RV                        (9.43)
E   1/2     HpH/2
C=log, det| I, +——R!”H,R.H“R               (9.44)
2    Nr  N    r  irene We it
or'T

(9.44)2 부터 N,=N,=N,R, 과 R, 7} full ranko]i2 SNR] 높을 때, 다음의 근사

식 (9.
을 얻는다.

시

E
C=log, aa  <

(a 고"

HH? Jee. det(R,)+log, det(R, )                    (9.45)

식 (9.45) 2} 관계식 (9.46) 3 (9.47) 04] 의해, 상관관계가 있는 때 MIMO 채널 용량이 감

b>
nok
thlo
ue
+>
ro T
co



===== PAGE 373 =====
PART Il MIMO2} MATLAB

det(R        J=[14 _4(R,)                                        (9.46)

log, det(R,) < 0                                           (9.47)

송신 안테나 사이와 수신 안테나 사이에 모두 상관관계가 있을 때 아래 수식으로 표현
는 만큼 용량이 감소된다.

되
log, det(R,,) + log, det(R, )                 (9.48)
Determinant?} eigenvalue2} 관계는 아래와 같다.
0608)=11408)                                                      (9.49)
또한, 산술평균과 기하평균의 관계에 의해 아래 관계가 성립한다.

1

(11 a\¥<+ Lani       (9.50)

위의 두 관계식을 결합하면 아래의 관계를 얻을 수 있다
= igs, det(R) < 0                                                  (9.51)
N
log, det(R) <0                                                        (9.52)

그림 9.82 채널 상관관계에 따른 용량 YAS 나타낸다. 송신단 안테나간에는 식(9.53)
으로 나타난 상관관계가 있고 수신단 안테나간에는 식 (9.                   없
가정하였다. 64#=18008에서 약 3.3 bps/Hz2] 용량이 상관관계에 의해서 감소함을 관찰할
수 있다. 상관관계가 높다는 것은 modal 0600000051001에 의해 표현되는 여러 모드들 중
낮은 SNRE 갖는 모드가 존재할 확률이 높다는 의미이다. 다음 프로그램 9.5 (“8180010
Capacity Correlation.m”)= 그림 9.8을 그려 주는 프로그램이다.

376



===== PAGE 374 =====
제9장_ MIMO 채널 용량

-ㅡ10 4×4 channels
| | correlated 4x4 channels

니나 ow S heme meals

1
ㅣ

0       5       10      15      20
=

그림 9.8 채널 상관관계에 따른 채널 용량 감소

% Ergodic Capacity Correlation.m
% Capacity reduction due to correlation of MIMO channels
clear all, close all;
SNR_dB=[0:5:20]; SNR_linear=10.*(SNR_dB/10.) ;
N_iter=1000;
nT=4; nR=4; n=min(nT,nR); I = eye(n); sq2=sqrt(0.5); % 4x
R=[1 0.76*exp(0.17*pi*j) 0.43*exp(0.35*pi*j) 0.25*exp(0.53*pi*}) ;
0.76*exp(-0.17*pi*j) 1 0.76*exp(0.17*pi*j) 0.43*exp(0.35*pi*j) ;
0.43*exp(-0.35*pi*j) 0.76*exp(-0.17*pi*j) 1 0.76*exp(0.17*pi*j) ;
0.25*exp(-0.53*pi*j) 0.43*exp(-0.35*pi*j) 0.76*exp(-0.17*pi*j) 1);
0 44 iid=zeros(1,length(SNR_dB)); 0 44 corr=zeros (1, length (SNR_dB)) ;
for Iter=1:N_iter
H_iid = sq2* (randn(nR,nT) +j*randn (nR,nT) ) ;
H_ corr = H_iid*R* (1/2);
tmpl = H_iid'*H iid/nT; tmp2 = H_corr'*H corr/nT;
for i=1:length(SNR_dB)
06 44 iid(i) = C_44 iid(i) + 1092 (det (I+SNR_linear (i) *tmp1)) ;
C_44 corr(i) = C_44 corr(i) + 1092 (det (I+SNR_linear (i) *tmp2) ) ;
end
end
0 44 iid = real(C_44 iid) /N_iter;
C_44 corr = real(C_44 corr) /N_iter;
plot (SNR_dB,C_44 iid, SNR_dB,C_44 corr,':');

Tm 프로그램 5 채널 상관관계에 따른 채널 용량 실행 프로그램

377


===== PAGE 375 =====
PART I_ MIMO} MATLAB

1   0.7667"8 0.436/7038 0.25e/°3*

나 _ 0.76e7°""" 1     0.76e/°""" 0.43e/°***             -
-_ 04362 1° 0.766 ~  1      0.76670^               ( :  )

0252.70 0432 03 0.7662 70    i
=k,                                      (9.54)

378



===== PAGE 376 =====
시공간 부호 기법은 여러 개의 송신 안테나를 이용하여 송신 다이버시티 oO] S(diversity
8810)을 얻는 부호화 방법이다. 18000은 최초로 시공간 부호의 개념을 소개했으며, 시공
Zt 부호의 설계 기준으로 10 기준과 determinant 기준을 제시했다[214]. Rank 기준이
부호의 성능에 더 지배적인 GS 준다는 사실을 기반으로, Grimm, Fitz, Krogmeier,
Baro, Bauch, 및 Hansmann2 모의실험을 통해 더 좋은 성능을 달성하는 부호에 대하여

연구하였다[217][218]. 최근에는 91000, Taricco, Biglieri, Byun7} 각자 독립적으로 PEP
의 bound7} 아닌, 정확한 PEPS 010860-1000으로 표현하여 시공간 부호의 성능을 분석
하였다219][2201.

시공간 부호는 크게 시공간 블록 4S (Space-Time Block Code; STBC)2} 시공간
trellis 부호 (Space-Time Trellis Code; STTC)# 분류할 수 있다. 시공간 66118 부호는
대체적으로 더 좋은 Ves 보이지만, 최대 다이버시티 차수를 얻기 위해서는 ML 복호기
(Maximum Likelihood decoder)2] 복잡도가 송신 안테나의 개수와 전송률에 대해 지수적
으로 증가하여, 높은 차수의 변조 기법을 채택함에 있어 제약이 있다.

STBC 분야에서는 Alamouti7} 최초로 2x1 복소 직교 설계(6007016% orthogonal design)
를 이용한 송신 다이버시티 HAS 소개하였고, TarokhS 이를 일반화 하여 직교 설계 이
“(orthogonal design theory) 기반한 직교성을 갖는 시공간 블록 부호를 제안하였다
[213][221]. 시공간 블록 부호는 상대적으로 부호화 이득은 작지만, 최대 다이버시티 차수
를 가지면서 수신기에서 선형 처리만으로 ML 복호를 가능하게 하기 때문에, 수신기의 복
잡도가 낮다는 장점이 있다.

최근에 9650800와 Jafarkhaniz= 시공간 ㅁ6106 부호와 시공간 블록 부호를 결합하여 최대
다이버시티를 만족하면서, 기존의 Alamoutit} Fitz2] 부호보다 더 높은 전송률을 갖는 새
로운 SOSTTC(Super—Orthogonal Space—Time Trellis 0000)를 제시하였다[222]. 기존 시
SU trellis SE 최대 다이버시티 이득과 추가적인 부호화 이득을 얻을 수 있었으나, 최

에
요
rl by

N

379



===== PAGE 377 =====
PART II_ MIMO2} MATLAB

적의 부호 설계 방법이 없었다. 한편, 기존의 직교 AAS 이용한
다이버시티 이득과 간단한 수신기 구조를 얻을 수
다. SOSTTCE 내부 부호로 41404004가 제시한 직교 설
부호를 사용하여, 최대 다이버시티, 최대 전송률을 달성히

을 얻는다.

본 장에서는 다수의 안테나를 통해 얻는 공간 다이버시티의 개념을 먼저 다루고, 시공
간 부호 기법 중 대표적인 시공간 블록 부호와 시공간 0610 부호에 대해 다루고, 모의실
혐을 통해 성능을 확인해 본다.

물이나 지형 등에 의한 영향으로 다

ㅇㅇ

중경             는 수신된 AS AS] 변동하는 Moly 현상을 SAC. 이
와 같은 Hols 현상에 의한 AS 품질의 저하를 방지하기 위해 ee 이용할 수
있다[224][225]. 다이버시티란 2개 이상의 독립된 전파 es 통해 전송된 여러 개의 수
신 신호 중 양호한 신호가 존재할 확률이 높다는 사실을 활용하는 방법이다. 이러한 다이

버시티의 구현 방법에는 다음의 방법들이 있다.

* 공간 다이버시티(60806 diversity) 공간적으로 충분히 분리된 2개 이상의 안테나를
이용하여 송수신하는 방식으로 안테나 간 이격 거리는 104 이상이어야 한다.

¢ 편파 CHO|WAJE|(Polarization diversity) : 수직 푸
방법으로 공간 다이버시티처럼 us 유지할 필요가 없

. Me 다이버시티(1106 diversity) : 충분히 = 시간 간격으로 동일한 QRS 여러 번

sale} 득립적인 피이딩음경혐토록 하는 방식이다

 주파수  ClO|HAIE|(Frequency diversity) : 동시에 서로 다른 둘 이상의 주파수를 사
용하는 방식이다. 주파수간 간격을 충분히 크게 하여 독립적인 페이딩을 겪게 하는 방식
이다.

ㆍ 각도 다이버시티(&00916 diversity) : 지향성이 다른 수신 안테나를 이용하는 방식으로
수신 방향의 So] 넓은 이동국 수신에 적합한 방식이다. Branch 수를 증가시키기 위해
서는 빔 Fo] 좁고 첨예한 지향성을 갖는 수신 안테나가 필요하다.



===== PAGE 378 =====
제10장_공간 다이버시티와 시공간

Frequency                                                        |   Frequency                                                     Frequency

Time

Spatial

PA

Spatial

그림 10,1 시간, 주파수, 공간 다이버시티의 도식적 표현

그림 10.12 시간, 주파수, 공간 다이버시티를 도식적으로 나타낸 것이다. 그림 10.1과
같이 다양한 다이버시티 기법 중 시간 다이버시티 기법과 주파수 다이버시티 기법은 시간
과 주파수의 중복 할당이 필요하여 자원의 활용이 효율적이지 않다. 그러나 공간 다이버시
티는 시간이나 주파수의 추가 할당 없이 향상된 평균 수신 SNRS 얻는다. 공간 다이버시티
성능은 안테나간 간격에 의존하게 되는데 수신 안테나를 공간 상에서 BE 10-202 정도로
서로 이격시켜서, 이격된 안테나로부터 수신되는 신호들은 서로 다른 위상 변화를 겪기 때

Bo] 낮은 상관 관계를 가지며, 이는 두 수신 신호가 통계적으로 서로 독립적이게 되어, 한
신호가 깊은 페이딩에 빠질 때 다른 신호는 깊은 페이딩에 빠질 확률이 적어지므로 결국
se Wied 되면 다중경로 페이딩이 적은 신호를 VE + 있게 된다. 이와 같은 장점
을 지닌 공간 다이버시티 기법에는 수신부에서 다수의 안테나를 사용하는 수신 다이버시티
기범과 송신부어서 HSS) bE 사용하는 송신 다이버시티 기법으로 나눌수 있다.

000 수신 다이버시티

수신 다이버시티 기법은 수신단에 다수의 안테나를 사용하여 다이버시티를 얻는 방식
자 본 절에서는 송신단은 하나의 안테나를 가지고 수신단은 여러 개의 re 가
Al 시스템을 고려하여 설명한다. 즉, 그림 10.2의 SIMO(Single Input Multiple Output) 채
널을 고려한다. 비선택적(0880 페이딩 채널을 가정하면, SIMO 채널을 다음과 같이 표현할

]

=
A
TM

ic

381



===== PAGE 379 =====
PART Il MIMO&t MATLAB

€K | 0

SIMO 채널                      MISO 채널        MIMI |
“| 10.2 a 「 안테나 개수에 따른 채널  "

H=[hhy--hy, |                       (10.1)

여기서 ¥ 2 Nex 크기의 수신 신호 벡터이고, 2 는 써22"}= Nly 의 특성을 가
Al 240800 잡음이다. 이와 같은 수신 다이버시티 기법에서 주로 사용되는 수신부의 Bh
성법에는 SC(Selection Combining), MRC(Maximal Ratio Combining), EGC(Equal Gain
Combing) 등과 같은 기법이 존재한다. SC 기법은 3가지 기법 중 가장 다 기법으로
매 심볼 구간에서 Ne AHS] 수신 안테나 중에서 가장 높은 SNRS 가진 수신 안테나의 A
SS 선택함으로써 다이버시티 이득을 얻는 기법이다. 수신부에서 ^ㅠ개의 독립적인
Rayleigh 페이딩 채널을 가정하고 각 6000애의 평균 944&값인 /,을 계산하면 다음과 같이
구할 수 있다.

=B (in?) 1=1,2,..,Np                   (10.3)

0         0

p=

각 branch2] 순시적 SNR ¥, S 다음과 같이 HAS 수 있다.

.
y, =|" 고 ,f=1,2,...,Np                        (10.4)

0

382



===== PAGE 380 =====
제10장_공간 다이버시티와 시공

위와 같이 구한 각 안테나별 순시적인 SNR 기반으로 수신 a |나를 선택함으로 페
이딩 정도가 최소인 신호를 검출함으로써 수신 다이버시티 ㅇ         수
법은 개의 BE branch] 독립적인 가중치를 적용하는  기법이다 가중치 Re 각
branch2] SNR 값을 이용하여 계산하게 된다. 각 ㅁ800에서 수신하는 신호가 yi, ZF
branch2] 가중치 값을 6라고 할 때 다음 수식의 연산을 수행한다.

Nr
Pune = > GY;                                      (10.5)

i=l

여기서 송신 ASE yy, =hx, +n,,E{|e |? }= 28, 이고 는 Z branch] 잡음 성분
으로 2N,°] 전력 ABE (Power Spectral Density)S 가진다. 그러므로 다음과 같은 형
태로 표현할 수 있다.

Np              Ne
Yure = > Ghx,+ Gn,                                         (10.6)
i=1              i=l

MRC 과정 후 잡음 성분의 전력 스펙트럼은 다음과 같다.

Nr
S,=2N, VIG)                            (10.7)

i=l

또한 순시적인 AS} 전력은 다음과 같다
= 26,                                       (10.8)

이 결과를 바탕으로 여러 branch} 평균 SNR 계산하면 다음과 같다.

Nr
>
N, dIIG|
i=l

(10.9)

Puc

383



===== PAGE 381 =====
PART 11 01140와 MATLAB

Cauchy—schwartz2] 다음 정의에 따라

Nr
2
|a,b,|
i=l]

Ne     Ne
<Dlal 2191                          (10.10)

Z} branch} SNR& G,=h' 이고 정확히 채널 정보를 알고 있다고 가정하면 다음과 같
이 나타낼 수 있다.

Purc =

Ny ‘a

이와 같이 MRC 기법은 86, EGC 기법에 비해 연산량은 크지만 우수한 성능을 보인다.
MRC 기법과 유사한 EGC 기법은 MRC 기법과는 달리 모든 6000애에 동일한 가중치를
적용하는 기법이다. 그러므로 MRC] 비해서 성능면에서는 열화가 발생할 수 있으나 구
현

is

복잡도가 낮다는 장점이 있다. 그림 10.32 Rayleigh 페이딩 채널에서 MRCS} 성능이.

이 결과를 통해 MRC 기법을 통해 성능의 큰 향상을 보임을 확인할 수 있다. 또한 수
안테나의 수가 많을수록 성능이 향상됨을 알 수 있다. 이와 같이 수신 다이버시티 기법
oO.

el,
신
호
L..
=
fo)

384

서

ㅇ
페이덩이 독립적인 Ase 수신단의 다
5             품

해 다이버시티 SS 획득하여 전송

10° =

=—— SISO
—O— MRC (Ny:1, Npi2)

—8— MRC (Ny:1, Np'4)

10°

10 2 4.6 8 10 12 1416 18 20
SNR [08]
그림 10.3 Rayleigh 페이딩 채널에서 MRC 성능



===== PAGE 382 =====
AOS SZ 다이버시티와 시공

oo
=

* MRC_Scheme.m
% Receiver diversity - MRC
clear, clf
packets=4000; frame=130;
BIT=2; % modulation 1/1/3/4 for BPSK/QPSK/16QAM/64QAM
NTx=1; NRx=2; idx = 1; % No. of Tx antenna No. of Rx antenna
EDNO=[0:2:20]; sq_NTx=sqrt (NTx); sq2=sqrt (2) ;
for i_SNR=1:length(EbNO)
SNR=EbNO (i_SNR); sigma=0.5/(10*(SNR/10)); sq_sigma=sqrt (sigma) ;
for p_count=1:packets
symbol data=randint (frame*BIT,NTx) ;
[temp 8 P]=modulator (symbol data.',BIT);
X=temp.'; frlg=length(X) ;   x0=X;
Hr=(randn (frlg,NRx) +) *randn (frlg,NRx) ) /sq2;
H= reshape (Hr, frlg,NRx) ; Habs=sum(abs(H) .*2,2); z1=0;
for i=1:NRx
#(:,,1)=Stim (H(2,4) «*X0, 2) /89 NIX. 2}.
+sq_sigma* (randn(frlg,1)+j*randn(frlg,1));
zl=Z1 + x(:,1) .*¢onj (H(:,1));

end

for m=1:P
d1(:,m)=abs(sum(z1,2)-s(m)).*2+(-1+sum(Habs, 2) ) *abs(s(m))*2;

end

[51111 =min((al),[],2),%  Sld=s(i1)."; Xd=([sid];

templ = X>0; temp2 = Xd>0;
error (p_count) =sum(sum(temp1l~=temp2) ) ;
end
BER(i_ SNR) = sum(error) / (packets*frame*BIT) ;
end% end of FOR loop for SNR
figure, semilogy(EbNO,BER,'b'), axis([EbNO([1 end]) le-6 160] ) ;

im) 프로그램 10.1 Rayleigh 페이딩 채널에서 MRC 기법 실행 프로그램

385



===== PAGE 383 =====
PART 1 )41140와 MATLAB

function [mod_symbols, table, P] =modulator (bits in,modulation)

full_len=length(bits_in); sql0=sqrt (10) ;

if modulation==1        % BPSK modulation
table=exp(j*[0 -pi]); table=table([1 0]+1);
inp=bits_in; mod_symbols=table(inpt+1l); P=2;

elseif modulation==2   % QPSK modulation
table=exp(j*pi/4*[-3 3 1 -1]); table=table([0 1 3 2]+1);
inp=reshape (bits _in,2,full_len/2) ;
mod_symbols=table([2 1]*inp+1); P=4;

elseif modulation==3   6 generates 8—-PSK symbols
table=exp(j*pi/4*[0:7]); table=table([0 13 2 6 7 5 4]+1);
inp=reshape (bits_in,3,full_len/3) ;
mod_symbols=table([4 2 1] *inp+1);

P=¢°
elseif modulation==4   % 16-QAM modulation
m=0;
for k=-3:253
for l=-3:2:3
m=m+1; table (m)=(k+j*1)/sql0; % power normalization
end
end

table=table([0 13245 76121315148 9 11 10] +1) ;
inp=reshape (bits_in,4,full_len/4) ;
mod_symbols=table([8 4 2 1]*inp+1) ;
P=16;    6 16 constellation points

else
error ('Unimplemented modulation');

end

aM
+

im) 프로그램 10.2 BPSK, QPSK, 8-PSK, 16-QAM

 송신 다이버시티

수신 다이버시티 기법은 효과적으로 다이버시티 이득을 얻을 수 있으나 모든 하드웨어
복잡도 및 연산량이 수신부에 집중되어 전력소모가 크다는 단점 때문에 단말기에서는 적
용이 힘들다. 반면, 송신 ome] 기범은 다수의 안테나를 Saeed 설치하여 다이바시
티 이득을                   를 갖는 단말기에서 다이버시티 이득을 얻을 수 있는 기

법이다. 송신 다이버시티 기법을 적용한 시스템은 수신부에서 채널 정보를 필요로 하는

386



===== PAGE 384 =====
10장_공간 다이버시티와 시공간 부호화 기법

시공간 66116 부호(90806-711016 Trellis Codes) 기법과 시공간 블록 부호(60806- Time
Block Codes) 기법, 수신부에서 채널 440] 필요 없는 차등 시공간 부호 기법
(Differential Space-Time Codes) 등이 있다[2251-[2271.

09 ee ee

OPA 시공간 부호화 시스템의 개요

시공간 부호가 적용되는 MIMO 시스템은 그림 10.49} 같다. 송신단에서는 Nr AS]

안테나가 있고, 수신단에서는 개의 안테나가 있으며 7 번째 송신 안테나와 / 번째

Al 안테나간의 경로 이득 hy, 1<is Np, <j < NAYS 서로 독립적인 복소

Gaussian 랜덤 변수라고 가정한다. 또한 이 페이딩 계수들은 7 심볼 구간에는 변화하지

않는 준 AA(quasi-static) 채널이라 가정한다. k 번째 심볼 구간에서 / 번째 수신 안테나
에 수신되는 수신신호 의 복소 기저대역 표현은 다음과 같다.

Yn = Pn, 220 +N,                                 (10.12)

식 (10.12)에서 xa 는 k 번째 심볼 구간에서 i 번째 송신 안테나를 통해 전송된 정규화된

복소 기저대역 신호로서 다음 식 (10.13)을 만족한다.

00

[을                              )
Space-                     Space-
——>| Time                       10 ~
Encoder                     Decoder
그림 10.4 시공간 부호화 MIMO 시스템

387



===== PAGE 385 =====
PART 41 MIMO2} MATLAB

Nr
Dla! =,                                (10.13)
j=l
P= 각 수신 안테나의 Bat SNRS 나타내며 Py, = P/N, ofc, 경로 이득 hy 값과 잡
음 값은 모두 서로 독립적인 BA Gaussian 랜덤 변수들로서 51091 페이딩 채널의
경우 hi 와 의 확률밀도함수는 다음 값과 같이 정의된다.

P(h, ) =<exp(- ^ |)            (10.14)
P(n,)= —exp(- buf)               (10.15)
A} (10.12)의 으로 구성되는 NeXT 행렬 y, //,으로 구성되는 N,XN, 행렬 H,

으로 구성되는 NXT 행렬 x, OB 구성되는 NeXT 행렬 2 을 이용한 행렬식으
로 표현하면 아래 식 (10.16)~(10.17)과 같이 표현할 수 있다.

y =Hx+z                              (10.16)
J,       「 h,      ^     때     hy,  |   x;         Z,
7? |   Mas      ‘2     -     May      2    +   ;                    (10.17)
YNp      | 1    hy >    때    hy wv, |  Xn,       27

GORD) 시공간 부호화 시스템의 231ㅠ-14156 오류 확률

수신단에서 완벽한 채널 정보를 가지고 있는 경우, 수신 신호의 조건부 확률 p(y|H.x)
는 다음 식 (10.18)로 표현된다.

(10.18)

P(y| Hx) =그01 -피(0 4 Hx)(y-./p,,H

al
빼어
z=
—— |
ae

388



===== PAGE 386 =====
제10장_공간 다이버시티와 시공간 부호화 기

따라서 ML 복호기는 각 신호행렬 xop 다해 [0-1060000-10640 |를 계산 이
를 최소로 하는 행렬 ×』,,을 복호하게 된다. ML 복호기의 복호 오류율을 계산한다. 정
확한 복호 오류율의 AALS 어려우므로, 대신 two-word 오류 확률을 계산하면, 행렬 x
가 전송되었을 GML 복호기가 행렬 xB 잘못 복호할 확률 7(ㄴ->ㄴ)은 으-함수를

이용하여 아래 수식과 같이 계산된다.

p(x +x)0{ Sh                        (10.19)

2

여기서 4, 는 ey, Hx 2} Jy, HX 의 Euclidian 거리를 의미한다. 식 (10.19) Chemoff
60000를 이용하여 다음과 같이 나타낼 수 있다.

1

p(x>x)<                   or

14 42(x-x)(x-x)                    a)

위 식 (10.20)에서 |-|4= 행렬의 determinants 의미한다. 4] (10.20)의 우변을 행렬
(x—x)(x-x) 의 eigenvalue ㅅ 값으로 표현하면 아래와 같다.

Nr

p(x>x)s                                   (10.21)

Ni       E wi  -ir
II  7  = (4 (A,,)          (10.22)



===== PAGE 387 =====
PART 1 MIMO2 MATLAB

여기서, vr 과 A, , 는 각각 r= rank{(x- x)(x-x)", 소미: 이며, A, Ay A, 은

행렬 (x—x)(x-x) 의 영이 아닌 DEAS 나타낸다. 따라서 식 (10.21)로 표현되는
two-word 오류 확률을 최소로 하기 위해서는 /값과 ^, 값을 크게 해야 하며, 특히 가능
한 모든 신호 행렬 x,, 에 대한 BL] 같을 아래 수식과 같이 최대로 해야 한다.

v= min rank{(x, -x,)(x, -x,)"|                   (10.23)

이 경우 ^“, 의 다이버시티 이득을 얻으며, >, 를 가정한다면 vs ^, 가 되므로,
v=N, 일 때 시공간 부호가 최대 다이버시티를 갖는다. 최대 다이버시티를 갖는 시공간
부호에서 Aye 아래 수식으로 표현된다.

Np

Ae =|(x, -조(지지 y

(10.24)

N
ol
_
i

호 행렬 ×,, Xo} 대한 의 HAMS 아래 식으로 표현된다.

17

A=min
kel

(x, —x,)(x, —X, )"

(10.25)

다이버시티 이득

Error Probability

SNR [08]
그림 10.5 다이버시티 이득과 부호화 이득의 비교

390



===== PAGE 388 =====
제10장_공간 다이버시티와 시공간 부호화 기법

위 식 (10.25)는 부호화 이득을 나타내며, 부호화 이득을 최대로 하는 것이 시공간 부호
설계의 두 번째 기준이 된다. 지금까지 다룬 다이버시티 이득과 부호화 이득의 9854에 따
른 오류확률 성능에 주는 영향을 그림 10.5를 통해 확인할 수 있다. 그림 10.5로부터 다이
버시티 이득은 BER 성능커브의 기울기와 관련되고, 부호화 이득은 BER 성능곡선의 수평

이동과 관련됨을 관찰할 수 있다[220][228][2291.

3

| 10.3 Me

본 절에서 시공간 BS 부호에 대해 UBT SAGE FA ASS Aled. 먼저
2개의 송신 안테나를 이용하여 송신 다이버시티       21: Alamouti 기법에 대해 알아
본다.

0908 Alamouti 기법

Alamouti= 최초로 2개의 안테나에 대해 복소 직교 AA\(complex orthogonal design)
를 이용한 송신 다이버시티 기법을 제안하였다[213]. 여기서 M-ary 변조 방식을 가정한

다. Alamouti 부호화기에서 두 개의 변조된 심볼 과 S 하나의 블록으로 하여 2개의
송신 안테나를 위한 송신 부호 PAS 아래 식 (10.26)과 같이 구성한다.

고 느

es 「    =|                                                   (10.26)

xX, 저

이와 같은 방식의 Alamouti 기법의 부호화기는 아래 그림 10.63} 같다.

Txt:x'=[2, —25]

0          Modulator          [z, 2,] > :   |                         .
bie                                      fala 오자          Ty2:x?=[2, 2]

|
그림 10.6 Alamouti 기법의 부호화기

391



===== PAGE 389 =====
PART If]_ MIMO2+ MATLAB

Alamouti 부호화기의 출력은 2개의 송신 안테나로부터 2번의 전송 구
두

간
AL 전송 구간 동안 두 심볼 지과 이 송신 안테나 1과 송신 안테나

re,

3
전송된다. 두 번째 AS 구간에서는 — a, TS 송신 안테나 1 로부터 전송하고, 7
송신 안테나 2 로부터 전송한다. 이와 같은 송신 ASS 송신 안테나 별로 묶어

A

아래 식 (10.27) 3} 같다.

Tx1: x! =| x,  -x;' |

indie =|    a" |                                 (10.27)

이와 같은 Alamouti 기법의 부호화된 2개의 전송 심볼은 아래 식 (10.28)의 관계에 있다.

x! (x? ig =x,x, —X, x, =0                           (10.28)

2     2
aa “Fl  ie        0     Jeter 티다 )                (10.29)

2       2
|x,| +|x,|

여기서, Ie 2x2 단위 행렬이다.
수신 안테나가 한 개라고 가정한다면 ML 복호기를 그림 10.7과 같이 나타낼 수 있다.
두 개의 송신 안테나와 한 개의 수신 안테나 사이의 채널 계수 BS 40) 와 &(00라 하

고, 채널 계수값은 다음을 만족한다고 가정한다.

h(th=h(t+T)=h, =|h|e"                (10.30)

h,(t)=h,(t+T)=h, =|h,|e*                   (10.31)

r+T AZ 동안 과 )》,를 수신한다. 수신 ASS 수식으로 표현하면 다음과 같다.

_ 392



===== PAGE 390 =====
간 다이버시티와 시공간 부호화 기

zy                                                2
“2,                                             =
21
<4 ——>
+         hy           +
Channel                      기. Signal
estimation            x           >| combiner
hy                 hy             '              Ty                 Zo
기            「                                 기            「

Maximum likelihood detector

|     |

1                  To

그림 10.7 Alamouti 기법의 ML 복호기

y, =Ax, +hx, +z,                                          (10.32)

y, =h,x, +h,x, +2,                   (10.33)

여기서, 과 >, 는 7와 7+7 시간의 AWGNE 의미한다.

이와 같이 수신된 신호로부터 송신신호를 검출하는 과정에 대해 설명한다. 먼저 채널
페이딩 계수값이 ^ 과 ^ 이고, 수신부에서 채널 정보를 완벽하게 알고 있다고 가정한다.
또한 변조된 성상도의 심볼들은 동일한 확률이라면, A] (10.34)를 이용하여 자승 Euclidian
거리를 계산하여 가장 짧은 거리를 가지는 심볼 벡터를 송신 심볼 벡터로 검출할 수 있다.

2

“01. + y8,) + d?(y,,-hS, + h,&) =|, Hh, —h,%,[° + |p, +48 AF         (10.34)

|

위의 방법

다음 수식으로 표현할 수 있다.

rlo

2
+

[527 fae ]= arg, min(l4l 지씨 —1)(b5    8, [}+ a? (%,,%,) +a? (도호)      (10.35)

393


===== PAGE 391 =====
PART Il_ MIMO2} MATLAB

여기서, ("은 송신 가능한 BE 심볼 벡터 O14) 의 집합이고

X, = +
= hy, -hy,

% = (|) +|Af Ja + An, + lan

% =||씨 기시 x An} + hin,

위 Al (10.37)z} (10.38) 이용해 ML ASS 하게 된다.

Xu. Sa | eRe

음 4] (10.35) At

(10.36)

있다. 먼저, 위 식 (10.36)의 Fb 2 aS

(10.37)

(10.38)

(10.39)

(10.40)

% Alamouti_scheme.m
clear; clf;
frl=130; NumofPackets=4000; NTx=2; NRx=1; BIT=2;
EbNO=[0:2:30]; sq _NTx=sqrt (NTx); sq2=sqrt (2);
for i_SNR=1: length (EbNO)

SNR=EbNO (1 SNR); sigma=0.5/(10*(SNR/10))

for p_count=1:NumofPackets

symbol data=randint (frl*BIT,NTx) ;

394

; Sq_Sigma=sq_ sigma;



===== PAGE 392 =====
제10장_공간 다이버시티와 시공간

tx_bits=symbol data.'; tmp=[];  tmpl=[];

for i=1:NTx
[tmp1,s,P]=modulator(tx_bits(i,:),BIT); tmp=[tmp; tmp1] ;
end
X=tmp.'; x0=X(:,1); xl=X; x2=[-conj\(X(:,2)) conj (X(:,1))];
for n=1:NTx
Hr (n,:,:)=(randn (frl,NTx) +j*randn (frl,NTx) ) /sq2;
end
H=reshape(Hr(n,:,:),frl,NTx); Habs(:,n)=sum(abs(H) .*2,2);
rl = sum(H.*x1,2) /sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1));

r2 = sum(H.*x2,2)/sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1));

21 = r1.*conj(H(:,1)) + conj(r2).*H(;:,2);
22 = r1.*con] (H(?,2)) - con) (r2) .#H(\s,1) +
for m=1<P
tmp = (-1+sum(Habs, 2)) *abs(s(m) ) *2;
di(:,m) = abs(sum(z1, 2) - ae  ^2 + tmp;
d2(:,m) = abs(sum(z2,2)-s(m)).*2 + tmp;
end
[yl,i1)=min(dl,{],2);  sld=s(21).';    clear di
[y2,i2]=min(d2,[],2); s2d=s(i2).';    clear d2
= [sld s2d]; tmpl=X>0; tmp2=Xd>0;
error (p_ count) = sum(sum(tmpl~=tmp2)) ;% for coded
end % end of FOR loop for "p count"
BER(i_SNR) = sum(error) / (NumofPackets*fr1*BIT)
End   6 end of FOR loop for SNR
figure, semilogy(EbNO,BER,'b!), axis([EbNO([1 end]) le-6 160] ) ;
grid on; xlabel('SNR [dB]'); ylabel('BER!);

Ta 프로그램 10.3 Alamouti 기법의 실행 프로그램

그림 10.8은 모의실험을 통해 Alamouti 기법과 앞에서 설명한 MRC 기법의 성능을

ri

2
님

있다고 가정한다. 송신 안테나와 수신 안테나 사이의 페이

rou

10,
flo 40 ot
이

두 때
pe)

} 것이다. 모의실험은 Rayleigh 페이딩 채널을 가정하고, 수신단은 sabi 채널 정보를
딩은 성

. 2x1 Alamouti 기법은 1x2 MRC 기법에 비해 다이버시티 이득은 동일하나, 부호화

낮음을 확인할 수 있다. 두 기법은 다이버시티 차수는 2로 동일하지만 Alamouti 기
송신 AAO] 2개의 송신 안테나에 나누어져 전송되고, MRC 기법은 1개의 송신 안테
전력이 할당되기 때문이다. 2x2 Alamouti 기법과 1x4 MRC 기법은 동일한

395



===== PAGE 393 =====
PART Il MIMOSt MATLAB

crn SISO

}-|—a— Alsmouti (

10% Alamouti (
E-| —k— MRC(1x2)

| -|—A— MRC(1x4)

0      5      10     15 20     25 30

SNR [dB]
그림 10.8 Alamouti 기법의 AS 비교

다이버시티 차수 4를 가지므로 2<1 Alamouti, 1×2 14#0에 비해 향상된 ASS 보임을
알 수 있다. 2x2 Alamouti 기법이 1x4 MRC 기법에 비해 열화된 성능이 보이는 것은 앞
에서 언급한 것과 같이 송신 안테나에서 송신 신호 전력을 2개의 안테나에 나누어 전송하

기 때문이다.

We 간단한 선형 연산을 통해 ML 복호 성능을 달성한다. 이것이 가능한
이유는 2개의 송신 안테나로부터 생성된 신호 사이에 직교성(00008008105)이 성립되기

문이다. 이와 같은 직교 부호 설계 방법을 임의 개수의 송신 안테나 시스템에 적용한 것
이 시공간 블록 부호화기 ($0206-71016 Block Codes)°]t}[214]. 시공간 블록 HSS
통해 47 의 최대 다이버시티를 얻고, 수신 신호의 선형 처리를 통해 간단한 ML BSS
하기 위해서는 Alamouti 기법과 같이 독립적인 부호 설계가 필수적이다.

a5

|.   :                           Space-Time      .    5
nrormation       >! Modulator       >    Block Encoder      :     ：
Data                                            Os             “| Tex

그림 10.9 시공간 블록 부호화기

_ 396



===== PAGE 394 =====
ae

ot

그림 10.9는 시공간 SS 부호화기의 구조를 보여주고 있다. 시공간 블록
전송 행렬 ※는 ^,×27이다. ^, = 송신 cre 개수이고, p= 부호화된 심볼의 한 블
록이 전송되는 데 사용되는 심볼 구간의 수이다. 시공간 블록 부호화기에 입력되는 심볼
의 개수는 《 개라고 하고, 변조된 ASA wy, i= 1] …, KE 77 비트로 이루어진다. 이 경우
시공간 블록 부호화기의 부호율은 다음과 같다.
R=—                             (10.41)
P
시공간 블록 부호의 스펙트럼 효율은 다음과 같다.
r, rmR km
=" I bits/s/H
고 a bile        (10.42)
여기서 4% * 는 비트와 심볼 전송률이고 BE 주파수 대역폭을 나타낸다.
송신 행렬 XY 《개의 변조된 심볼 원소 값인 mo af, 22 ,…,&/ 의 선형 결합은 아래
와 같은 특성을 가져야 한다.
=히지 + bo) +--+ by) 5                  (10.43)
식 (10.43)으로부터 다음 관계가 성립함을 알 수 있다.
14
제 2 > 2,98, =0, 12 j, 0/6비2...24}             (10.44)
t=l
ORR] + 신호 시공간 블록 부호
시공간 블록 부호 기법은 실수 신호 시공간 블록 부호와 복소수 신호 시공간 블록 부호
로 분류할 수 있다. 본 절에서는 실수 신호 시공간 블록 부호 행렬의 설계에 대하여 설명
한다. 송신 안테나의 개수가 ^, =2,4,8 인 경우에 대하여 정사각형의 송신 부호 Yas
고려한다. 이와 같은 BSE 최대 전송율을 가지고 또한 ^, 의 최대 송신 다이버시티를

397 _



===== PAGE 395 =====
PART 4 MIMO2} MATLAB

가진다. 송신 안테나의 수가 4, =2,4,8 인 송신 부호 BAS 아래 식 (10.45)~(10.47)와
같이 주어진다.

x, = |!   =                                       (10.45)

xX, x
% “-%, -% -%
x, Xx     xX, —-Xx
2     1      4       3
x,=                                                       (10.46)
® -& &
5» & —& 4,
% =, -% —-h — = =
> %§* -—% 제 %& & 제 -G
제 & & ~ S| Bee 제
X, —-X, Xx     X = XX. - Xx
4      3     2      1       8     7       6     5
x, =                                                                     (10.47)
4 & 제 & KH -2 = -저
ij %~% 제 &® & § %& 6
By ky 자 차 %& —% & X
[제 Xp 6 5 Xe Ke HH |

이와 같은 부호 행렬의 부호율은 1 YS 알 수 있다. 예를 들어 식 (10.46)의 송신 안테
나 4개를 ane 부호 행렬의 송신 구간 / 는 부호 행렬의 열벡터의 개수가 되므로
fe)

알            송     은 x1, Xp, x3, 저이므로 앞에서 정의한
바드 + i 그러므로 부호율은 아래 식 (10.48)와 같이 1°] 된다.

리로,                      10.48
                  (10.48)

#& 개의 송신 안테나를 가진 경우 최대 BSR #=1로 전송하기 위해서는 송신 구간
의 최소값이 다음과 같아야 한다.

p=min(2“**) 6.010ㅋ0004, 80+20240,    (10.49)

398



===== PAGE 396 =====
제10장_공간 다이버시티와 시공

식 (10.49)를 바탕으로 실수 ASS 이용한 최대 다이버시티와 최대 전송율을 얻기 위
한 4~=3, 5, 6 크기의 직사각형 BAS 다음과 같다.

시 86 8 |[-저

X,=|X, % 기 [제        (10.50)

> 기 ye, -지8 으으

Ke=|%, % 저 = —% Xe 치 %                               (10.51)
X = % % = | —m xX
he Me 세 Me % id, “hy 이

& & -서 & “%& |S & =
Ss & | = ~*~ FR & 3
5              4                1                  2                7                8              5                6
X,=                                                                                                              (10.52)
i %& & F&F > & — «©
때 ee oe,
Xe =X, 자 -6 % (|% x, =X,

SORW] 복소 신호 시공간 블록 부호

복소 신호 x, 32, …, 1S 원소로 가진 47× 복소 송신 행렬 ×, 가 아래 식 (10.53)을
만족하면 부호율이 4/2이고, ^, 의 최대 다이버시티를 갖는 시공간 블록 부호가 된다. 이
와 같은 YY] 예로서 Alamouti 기법은 복소 신호 시공간 블록 부호 기법을 사용하여 2
개의 전송 안테나를 통해 최대 부호을 1과 최대 다이버시티 2를 달성함을 10.3.1에서 보
였다.

41 — Lo

&=|  *

5  1

이와 같은 설계 기준을 이용하여 >=3과 ^>=4인 경우에 부호윤이 1/20] 되는 송
렬을 다음과 같이 표현할 수 있다.

신행

399           |



===== PAGE 397 =====
PART II_ MIMO2} MATLAB

| %& % = 제 F % =~     (10.54)

i hy = -% 지 2 2 =,
x                             *            *              *            x
5 oe                  - & & & *
_ | 2         1           4            3        2         1           4            3
X,=                                             ;          3 5          ‘                                (10.55)

=

A] (10.54), (10.55)의 행렬은 최대 다이버시티 이득을 제공하는 011 rankZAS 만족한
다. 그러나 송신 구간 2=8#이고, 송신 ASS x, 2m, 33, x 이므로 <=4이다. 그러므로 부
호율 #=1/2 가 된다. 높은 부호율을 위해 복잡한 선형 처리를 요구하는 블록 부호 행렬

"             즈                      x
자            af                     시고
_           :             x                    =~
Xhign3 —| 스지              2                     a                      (10.56)
XS  XS  (  x,   x, +X,  i.)   (% +X, +X, -x;)
142 2              2                       2          J
fy             Es                      S|
1       2             2                      /2
By                       “4,
xX      x              >=                     =>
2       1              2                      2
Xena =                                                                                  (10.57)

Al (10.56), (10.57)& 크기가 33} 4인 행렬이며 부호율은 3/4이다.



===== PAGE 398 =====
제10장_공간 다이버시티와 시공간 부호화 기법

위에서 설명한 시공간 블록 부호를 사용한 시스템에서 신호의 복호 방식은 앞에서 설
한 Alamouti 기법과 비슷한 방식으로 복호할 수 있다. 즉, 선형 처리를 통해 간단한 최대
우도 복호를 수행한다.                  간에 j 번째 안테나로부터 수신한 )라고 할 때 다

음과 같이 정의 할 수

위

xo jim >)
ox
>
때

= Yh +n)                                     (10.58)

4} (10.59)에 ML 복호를 적용하면 다음과 같이 전개할 수 있다.

Nr Nr

R => > yh, 6, (i)                                (10.59)

t=1 j=l

여기서 (4) 는 부호 행렬의 * 번째 열의 ×의 BSS 나타낸다.

x, =argmin|R, — x| mia                 (10.60)
XE                      Kl

은 아래 식과 같다.

2

0000007000000000000|오

j=l i=l

(10.61)

;를 복호하기 위한 결정 메트릭은 다음과 같다.

401


===== PAGE 399 =====
PART I MIMO2} MATLAB

2

120“ -24, +yih,, +(x) 7 -(02) Xj +(x) su) em
=

(10.62)
m 3
+{ 1428.55) Jk
j=l i=l
AS 4S 복호하기 위한 결정 메트릭은 다음과 같다.
,                                               2
20  ih  —yih,    vl; +) 3 / -(08) xj -(y{) su) os
을                                                           (10.63)
m 3
+[-12E Sf |x,|
j=l isl
심볼 4S 복호하기 위한 결정 메트릭은 다음과 같다.
es                                                2
=                                                            (10.64)

+[-14 2534. Jot

j=l i=l

STBC Performance (QPSK)                                                       STBC Performance (16QAM)

-6@- SISO-16QAM 0001.60)
10°°b|—— STBC-16QAM (Tx:2, Px)
E]—+— STBC-16QAM (1x3, Rt)

——_STBC-16QAM (Tx, Ret)

0      5      10     15     30° 25     30        0      5      10     15     20     25     30

-@- SISO-OPSK (Tx:1, Rx:1)
10 비-ㅁ4- STBC-OPSK (Tx:2, x1)
—+— STBC-OPSK (1:3, Px:1)
—©—  STBC-OPSK (Tx:4, Pct) |=!

SNR [08]                                                         SNR [08]
(a)                                                                           (b)

그림 10.10 다양한 안테나 개수에 따른 시공간 블록 부호화기 성능 비교

402



===== PAGE 400 =====
제10장_공간 다이버시티와 시공간 부호화 기법

6 STBC 3x4.m
clear; clf;
NTx=3; NRx=4; BIT=2; NumofPackets=4000;
frl=130; EbNO=(0:2:30]; sq_NTx=sqrt (NTX) ;
for i_SNR=1:length (EbNO)
SNR=EbNO(i_ SNR); sigma=0.5/(10*(SNR/10)); sq_sigma=sqrt (sigma) ;
for p_count=1:NumofPackets
symbol data=randint (frl*BIT, 4) ;

tx_bits=symbol_data.'; temp=[];   temp1=[] ;
for i=1:4
{temp1,s,P]=modulator(tx_bits(i,:),BIT); temp=[temp; temp1] ;
end
X=temp.'
% Block signals in the 1—th time slot % Block coding for G3 STBC
x0=X(2, 1) ;      SIX (2238) %
2g yl) == R32) 7 RQ 2EHKe, Is *2\(5,,3) 2x42) 5
3) (9 pd) SK 3) FY, 2058 (1 4) se Be, SSK (a, 20 7
4(:,1)=-X(:,4); x4(:,2)=-X(:,3 ~“   (2 p 8) Sk Cra) 7
ene te 1)» x6=cony] (x2);   x7=conj (x3) ;   x8=conj (x4) ;
for n=1:NTx
Hr(n,:,:)=(randn(frl,NTx) +3*randn(frl,NTx) ) /sqrt (2) ;
end
for n=1:NTx

H = reshape (Hr(n,:,:),frl,NTx); Hc=conj (H) ;

Habs(:,n) = sum(abs(H) .*2,2);
rin=sum(H.*x1,2)/sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1
r2n=sum(H.*x2,2)/sq NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1
(

r3n=sum(H.*x3,2) /sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1

i
di

) ;
i

)                                            ) ;
rén=sum(H.*x6,2) /sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1))j;
)                                            )

)                                              )

r7n=sum(H.*x7,2

i

(                         (                    (    )
(                           (                      (     )
(                           (                      (     )
r4n=sum(H.*x4,2) /sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1)
r5n=sum(H.*x5,2) /sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1)
(                           (                      (     )
(                           (                      (     )
(                           (                      (     )

)
/sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1
r8n=sum(H.*x8,2)/sq_NTx+sq_sigma* (randn(frl,1)+j*randn(frl,1
21 1 = Yin. *He (2,1) + r2n.*He (2,2) + r3n.*He (25.3) 7

21 2 = conj(r5n).*H(:,1) + conj(rén) .*H(:,2) + conj(r7n) .*H(:,3);
Z1(%,m) = 211+ 21 2;

t

403



===== PAGE 401 =====
PART Ill MIMO2} MATLAB

22 1
22 2
22(:,2) = 22 1ㅋ 22 2;

23 1. ㅋ>21ㅁ.*“80 (1 , 3) ~ r3n.*Hc(:,1)-r4n.*He(:,2);
23 2
z3(%,n) = 23 1 + 232;

24 1 = -r2n.*He(:,3) + r3n.*Hc(:,2) - r4n.*Hce(:,1);

rln.*Hc(:,2) - r2n.*He(:,1) + r4n.*Hc(:,3);

1

z4(:,n) = 24 1+ 24 2;
end
for m=1:P
tmp = (-1+sum(Habs,2)) *abs(s(m))*2;
for i=1:4
d(:,m,i) = abs(sum(z(:,:,i),2)-s(m)).*2 + tmp;
end
end
Xd = [1];
for n=1:4, [yn,in]=min(d(:,:,n),[],2); Xd = [Xd s(in).
templ=X>0; temp2=Xd>0;
error (p_ count) = sum(sum(temp1l~=temp2) ) ;
ends end of FOR loop for "p_count"
BER(i_SNR) = sum(error) / (NumofPackets*fr1*BIT) ;
ends end of FOR loop for SNR

conj (r5n).*H(:,2) - 0003 (267) .*H(:,1) + conj(r8n) .*H(:

conj (r5n) .*H(:,3)-conj (r7n) .*H(:,1)-conj(r8n) .

띠 ;

*H (ey 2) 7

24 2 = -conj(rén) .*H(:,3) + conj(r7n) .*H(:,2)- conj(r8n) .*H(:

end

73);

; 0

il 프로그램 10.4 시공간 블록 부호화 기법 실행 프로그램

그림 10.10은 시공간 블록 부호 기법의 모의실험 결과이다. 모의실험은
딩 채널상에서 다양한 개수의 송수신 안테나를 가진 시스템에 시공간 부호 기법을 적용

하

10(00)는 QPSK, (6)는 16QAM2] 변조

이버시터 차수가 커지게 되므로 송신 안테나 수가 많아질수록 성능이
수 있다.

404

~~...)

fo}

Rayleigh 페이

방식을 사용하였
고 다양한 송신 안테나 수에 따른 성능을 나타내며, 송신 안테나 수가 많을수록 송신

WAS 호



===== PAGE 402 =====
제10장_공간 다이버시티와 시공간 부호화 기

 104 422   간 Trellis 부호

즈
of
0 '구
ㅇ i
ne '

오 기법은 수신단에서 간던힌                 식을 통해 최대 다이버
시티 이득을     수 있다. 그러나 시공간 블록 부호 기법을 이용할 때 부호화 이득이 일
반적으   때 본 절에서는 오류 제어 부호(600 control coding), 변조, 송수신 다이버시
티를 동시에 고려하여 설계한 시공간 06118 부호에 대해 설명한다. 시공간 06108 부호는
Tarokh, Seshadri, 및 081060080(에 의해 처음으로 소개되었다[225]. 많은 연구를 통해 시
ot trellis 부호는 부호화 이득과 스펙트럼 효율성, 비선택적(080) 페이딩 채널에서 다이
버시티의 이득을 달성할 수 있음이 확인되었다[229]-[231]. 본 절에서는 M-PSKS 사용
한 AS trellis 코드 설계에 대한 이론을 설명하고 모의실험을 통해 성능을 확인한다.

GOR 시공간 7ㅠㅇ1115 부호화와 복호화

A

Data

Modulator

그림 10.11 시공간 6! 부호화기

시공간 ㅁ61115 부호화기는 06118 구조에 의해 HAS. 본 절에서는 시공간 \ㅎ6115
부호화 M-PSK 변조방식을 이용한 ^, 개의 송신 안테나를 가진 송신부를 가정한다.
그림 10.11은 시공간 06118 부호 시스템의 간략화한 송신부를 나타낸다. 입력 비트는
c= [eet] 정의하고, /시간에 m=log,M 개의 이진 데이터의 그룹을
= 이아 |로 정의한다. 시공간 66115 부호화기를 통해 부호화된 M-PSK 심볼의
신호는 다음 식 (10.65)과 같이 나타낸다.

지디 …포|                         (10.65)

여기서 포 는 시간에 시공간 심볼로서 TS 식 (10.66)과 같다.

elo if                                       (10.66)

t  구구



===== PAGE 403 =====
PART 141 MIMO2} MATLAB

(아나 14

^

(gi.
a_

그림 1012 AlSZt trellis 부호기의 구조

WAS 신호 x,a7,.0x) 는 ^, 개의 송신 안테나를 통해 전송된다.

그림 10.12와 같은 시공간 46118 코드 부호화기의 입력 값은 ,6^,…,@”이고, 개의
feedforword “  레지스터로 구성된다. kel 입력 값인 =(ㅇ0, scp),
k=1,2,..m *번째 쉬프트 레지스터를 통과하고 계수 값과 곱해진다. 모든 레지스터
로부터 곱셈기의 출력값은 Mmodulo 연산이 더해진다. 이런 과정을 통해 출력 값

x=(x',x’,...,.x°") 로 주어진다,

가 가 0 7" al eehtth ening ae, ee )|

| ~ 커 iC. Jeconcil eae spose, )|

8 =
gs
|                                                                                             (10.67)

여기서 gh sk =1,2,...,m, j =1,2,...,V,,7=1,2,...,N, 은 M-PSKZ 변조된 심볼이다. B
호화기의 7 번째 시간, 7 번째 송신 안테나의 출력 값은 × 이고 아래 수식과 같이 연산된다.



===== PAGE 404 =====
:

제10장_공간 다이버시티와 시공간 부호화 기법

VE

= >  28), ci, mod M,i=1,2,...,N,           (10.68)

k=l j=
변조되어 7번째 시간에 전송되는 시공간 ASL 다음 4] (10.69)와 같다.
피=(지0002                     (10.69)

이와 같은 시공간 trellis 코드 부호화기는 메모리가 사용되는데 전체 메모리의 크기는
다음과 같다.

v= >                                         (10.70)
k=1

여기서 v,.4 =1,2,....mt= k 번째 branchS 위한 메모리 크기로 M-PSK 성상도를 위
한 \,값은 다음과 같이 정의된다.

1+-1
y=                                    (10.71)
log, M

ABU trellis 부호화기를 위한 상태는 2'개이다. 개의 곱셈 계수 그룹 AMAL 생
AQABA 부른다. 2개의 송신 안테나를 가진 시공간 6618 부호화기 상위 쉬프트 레지
스터의 입력 이진 수열의 생성 다항식은 다음과 같다.

0(2)=8+60202+0270+620 +                             (10.72)

이와 유사하게 하위 쉬프트 레지스터의 입력 이진 수열의 생성 다항식은 다음 수식과
같다.

@(2)=0+0602+021+020+-        (10.73)

호화기를 위한 feedforward 생성 다항식은 다음과 같이 표현할 수 있다.



===== PAGE 405 =====
PART 4 MIMO2} MATLAB

G;(D)= 2, + gD ++, ,D"                             (10.74)

이와 유사하게 7 번째 송신 안테나의 하위 부호화기를 위한 feedforward 생성 다항식은
다음과 같이 표현할 수 있다.

G) (2)= 8878.27 gs, DP”                              (10.75)
송신 안테나 』로부터 ASHE 부호화된 심볼 수열은 다음과 같은 AAS 수행한다.
x' (D) =c'(D)G/(D)+e° (D)G* (D) mod 4                    (10.76)
이 4] (10.76)은 다음 4] (10.77)과 같은 형태로 다시 나타낼 수 있다.
G!(D)
es  1      1       i
=[c'(D) ¢ oe Al mod 4               (10.77)

ㆍ 00004 A132! Trellis 429] 예제

본 절에서는 시공간 46118 부호 시스템의 이해를 돕기 위해 예를 들어 설명한다. 2742]
송신 안테나를 가지며 4개의 상태를 갖는 시공간 ㅁ6118 부호화된 QPSKI] 신호를 전송하
는 시스템을 가정한다.

'=[(0,2
1(0,2).(2.0)                         (10.78)
* =[(0,1),(1,0)

부호화를 OF trellis PAL 그림 10.13과 같다. Trellis: 4개의 상태로 구성되고, 474
의 입력 데이터 AMAL ¢=(10,01,11,00,01,...) 로 가정하면 시공간 ㅁ6118 부호화기를

통해 생성되는 출력 값은 x =(02,21,13,30,01,...) 이다. 두 개의 안테나를 통해 0

ABE 각각 x' =(0,2,1,3,0,...), x =(2,1,3,0,1...) 이다. A 번째 안테나로부터 전송되
는 신호는 두 번째 안테나로부터 전송되는 신호의 지연된 신호로 지연 다이버시티를 얻을
수 있다:

408



===== PAGE 406 =====
제10장_공간 다이버시티와 시공간 부호화 기법

00/00    01/01     10/02     11/03

00/10    01/11     10/12    11/13

00/20    01/21     10/22    11/23

00/30      01/31        10/32       11/33

그림 10.13 Trellis 구조

시공간 06106 부호의 복호기는 ML BSS Ye Viterbi 알고리즘을 이용한다. Viterbi
알고리즘을 이용하명, branch 메트릭으로 A Euclidian 거리를 사용하여, AA 경로 메
릭을 선택함으로써 복호한다.

(10.79)

이와 같은 생성 다항식을 이용하여 표현한 부호 YAS 유용하고 간단하여 널리 사용되
는 시공간 06108 부호 기법이다. 다양한 연구를 통해 이와 ZS rank, determinant 및
trace 기준을 이용한 유용한 다항식이 제안되었다[232]. 표 10.1은 rank2} determinant 기
ZS 이용한 다양한 송신 안테나 개수에 따른 생성 시퀸스를 정리한 것이다. 표 10.2는
trace 기준을 이용한 다양한 송신 안테나 개수에 따른 생성 시퀸스를 정리한 것이다.

= 10.1 Rank} Determinant 기준을 기초로 한 다양한 안테나 개수에 따른 생성 시퀸스

2'[(0,2) (2,0) ]
QPsk 8   8   [(00) --          :   :
g'[(0.2) (       (0, 2) |
QPSK 4   2   g°[(0.1) S (2,0) |   2
wk 0 20003 (0.42) 600         39
QP           g[(2,0,0) (1.2.0) (2,3,3)]



===== PAGE 407 =====
PART If MIMO2} MATLAB

g'[(0,4) (4,0) ]
8PSK        3         2       g°[(0,2) (2,0) |                            2         9         4

g°[(0.1) (5.0)]
s'[(0.4) (4,4)]

SPSK 4 2: 6 ef (0.2) 42) |    2 3908. 6

"(00 (5.1) (15)]

표 10.2 Trace 기준을 기초로 한 다양한 안테나 개수에 따른 생성 AA

g'[(0,2) (1,0) |

ae   2   #1023) (2.0)]          2   40 10,0
g'[(1,2) (13) (3,2)]

QPSK |   2  #{(2.0) (22) (2,0)]      2   8,0 16.0
g'[(0,2,2,0) (1,2,3,2) |

QPSK 4   3   2((2342) (20,21)       2   - 20.0
g'[(2.4) (3,7)]

8PSK 3  2  g[(4,0) (6,6)]       2 0,686 8,0
g°| (7,2) (0,7) (4,4)]
g'[(2,4,2,2) (3,7,2,4) |

800 4   2 (6044) (6,6,4,0) |      2   - 20,0
s'[(

그림 10.14 시공간 0618 기법을 이용한 모의실험 결과이다. 모의실혐은 2 정적 페
이딩 채널을 이용하였다. (ats 2x1 시스템으로 다이버시티 차수가 2이므로 성능의 기울
기가 모두 비슷하다. States] 수가 많을수록 부호화 이득이 높아지므로 성능이 향상됨을
확인할 수 있다. (6)는 2x2 시스템으로 다이버시티 차수가 4이므로 2×1에 비해 성능이 향
상되는 것을 확인할 수 있다.

 410



===== PAGE 408 =====
제10장_공간 다이버시티와 시공간

=

STTC Performance                                    10°                         STTC Performance

-6- STIC (APSK ASiate, 2x1) |----                         benno
—8~ STIC (4PSK, 8State, 2x1)    foot   toot         ㆍ   i    i    {
-+- 9110 (409<, 16926.20)| -:    4    —           —9— STTC (4PSK, 4State, 2x2)

—#— STTC (4PSK, 32State, 2x1)       |       |       {       !                        -다- 9110 (4PSK, 8State, 2x2)
고        1       1              1]       1       1       {       H       1                    2         i         i         H         i         i         {         i
5s 6 7 8 9 0 11111 o> 02 8 4 65 67, 0
SNR [08]                                          SNR [dB]

(a)                                              (b)

그림 10.14 다양한 statedl] 따른 시공간 6115 부호화기의 성능 비교

응 STTC.m

clear;

frame=1000; Packets=130;   state='4 State 4PSK';

Rx_antennas=2; Tx_antennas=2; zf=3;

[dlt,slt,md] = sttc_stage_modulation(state,Rx_antennas) ;

if md==4 %4PSK
BITS=2;

elseif md==8%8PSK
BITS=3;

elseif md==16%16QAM
BITS=4;

end

SNR=5i2 +15;

for i=1:length (SNR)
source data = data_generation(frame, Packets,md, zf) ;
encoded_data = trellis_encoder(source data,dlt,slt) ;
mod_sig = sttc_modulator(encoded_data,md) ;
[signal,ch_coefs] = channel (mod_sig,SNR(i) ,Rx_antennas) ;
[data_est,state est] = detect (signal, dlt,slt,ch_coefs) ;
[FER_i] = count (source _data,data_est) ;
FER (i) = FER_i;

end

]

| 프로그램 10.5 시공간 6115 부호화기의 실행 프로그램

(

411


===== PAGE 409 =====
PART Il_ MIMO2} MATLAB

2

* sttc_stage_modulation.m
function [dlt,slt,md]=sttc_stage_modulation(state,No_Rx)
switch state
case '4 State 4PSK'
md=4; s=4;
case '8 State 4PSK'
md=4; s=8;
case '16 State 4PSK'
md=4; s=16;
case '32 State _4PSK'
md=4; s=32;
case '8 State 8PSK'
md=8; s=8;
case '16 State 8PSK'
md=8; s=16;
case '32 State 8PSK'
md=8; s=32;
case 'DelayDiv_8PSK'
md=8; s=8;
case '16 State 16qam'
md=16; s=16;
case 'DelayDiv_1éqam'
md=16; s=16;
otherwise
disp('Wrong option !!');
end
base = reshape(1:s,md,s/md)';
slt = repmat (base,md,1) ;
ste bel6é=(.0 O;11 1; 2 2; 9 Sp 4 4515 5; 6 6;23 77 8 8; 8) 9110 Loy
L 21812 72288 7 23734 14, 5 15];
for j = 1:md
Ls] = 1
ak = bitget(1,1); bk

bitget (1,2);

dk = bitget(1,3); ek = bitget(1,4);

switch md

case 4    % 4 PSK

for 1. = 1s
k=i-1;
ak_1 = bitget(k,1);       bk_1 = bitget (k,2) ;
ak_2 = bitget (k,3);       bk_2 = bitget (k,4) ;
ak_3 = bitget(k,5);       bk_3 = bitget(k,6) ;
switch s

412



===== PAGE 410 =====
장_공간 다이버시티와 시공

case 4 %4state_4psk
if No_Rx~=2
dlt(i,j,1) = mod(2*bk_l+ak_1,md) ;srank& determinant
dlt(i,j,2) = mod(2*bk+ak, md) ;
else
dlt(i,j,1) = mod(2*bk_1+ak_1,md) ;
dlt(i,j,2) = mod(2*bk+ak,md) ;

1

end
case 8 %8state 4psk

if No_Rx~=2
dit (i,j,1) = mod(2*ak_2+2*bk_1+ak_1,md) ;
dlt(i,j,2) = mod(2*ak_2+2*bk+ak, md) ;

else
dlt (1,j,1)= mod(2*bk_1+2*bk+ak_1+2*ak,md) ;
dlt (i,j,2)= mod(bk_1+2*ak_2+2*bk+2*ak_1,md) ;

end
case 16 sl6state 4psk
if No_Rx~=2
dlt(i,j,1) = mod(2 * ak_2 + 2 * bk_1 + ak_1,md);

else
dit (i,j,1) =mod(2*bk_3+2*ak_3+3*bk_2+3*bk_1+2*ak_1+2*ak,md) ;
dit (i,j,2)=mod(2*bk_3+3*bk_2+bk_1+2*ak_1+2*bk+2*ak, md) ;
end
case 32 @32state_4psk
dlt (i,j,1) =mod(2*ak_3+3*bk_2+2*ak_2+2*bk_ 1+ak_1,md) ;
dlt (1,j,2)=mod(2*ak_3+3*bk_2+2*bk_1l+ak_1+2*bk+ak,md) ;
end
end
case 8 % 'rank & determinant' criteria only
for i = iss

dit (i,j,2) = mod(2 * bk 2 + 2 * ak 1 + 2 * bk + ak,md);

k= 1 = a;

ak_1 = bitget(k,1);       bk_1 = bitget(k,2) ;
dk_1 = bitget (k,3);       ak_2 = bitget(k,4);
bk _2 = bitget (k,5);

switch s

case 8

switch state
case '8 State 8PSK'
dlt(i,j,1) = mod(4*dk_1+2*bk_1+5*ak_1,md) ;
dit (i,j,2) = mod(4*dk+2*bk+ak, md) ;
case 'DelayDiv_8PSK'



===== PAGE 411 =====
PART If_ MIMO2! MATLAB

dlt (i,j,1)=mod(4*dk_1+2*bk_1+ak_1,md) ;
dlt (i,j , 2) =0ㅁ00 (4*dk+2*bk+ak, md) ;
end
case 16 sléstate 8psk
dlt (i,j,1)=mod(ak_2+4*dk_1+2*bk_1+5*ak_1,md) ;
dlt(i,j,2)=mod(5*ak_2+4*dk_1+2*bk_ 1l+ak_1+4*dk+2*bk+ak,md) ;
case 32 %32state_8psk
dlt (i,j,1)=mod(2*bk_2+3*ak_2+4*dk_1+2*bk_1+5*ak_1,md) ;
dlt(i,j,2)=mod(2*bk_ 2+7*ak_2+4*dk_1+2*bk l+ak_1+4*dk+2 ..
*bk+ak,md) ;
end
end
case 16%   % 16 QAM 'rank & determinant' criteria only
fer 1. = 155

k=i-1;

ak_1 = bitget(k,1);       bk_1 = bitget(k,2) ;
dk_1 = bitget(k,3);       ek_1 = bitget (k,4);
switch s

case 16

switch state
case '16 State 16qam'
dle, 9., L)=ste_bellé (141, 1) >
dlt (i,j,2)=stc_bel6 (k+1,2)-i+j;
case 'DelayDiv_16qam'
dlt (i,j,1)=mod(8*ek_1+4*dk_1+2*bk 1+ak_1,md) ;
dlt (i,j,2) =mod (8*ek+4*dk+2*bk+ak, md) ;
end
end
end
end
end

Te 프로그램 10.6 시공간 trellis 부호화기 함수

function data=data_generation(fr_ length, frames, ,ㅁ0, zf)
data = round((md - 1) * rand(fr_length,1,frames) ) ;
{m,n,o] = size(data) ;

n=m+i1:m+ 2£;

data(n,:,1:0) = 0;

Ti) 프로그램 10.7 ABZ! trellis 부호화기의 데이터 생성 함수



===== PAGE 412 =====
다이버시티와 시공간 부호화 기법

간

trellis encoder (data,dlt,slt)

function enc data
[fr_length,1,frames] = size(data) ;
잉크 |
for k = 1:frames
for i = 1:fr_length

d = data(i,1,k) +1;

enc data(i,:,k) = dlt(s,d,:)¢

sie Slt(s,d,2) ?

end
end

하스
함수

ja) 프로그램 10.8 시공간 6115 부호화기의 인코더

function sig_modul = sttc_modulation(data,md,sim_options)

Gamie=[1 1; 2 1; 31, 417 42) 3 2) 2 2; 1/23 13; 23; 3 3; 43; 44; 3 4;
24; 14);
[frame_length, space_dim, frames] =size (data) ;
for k = 1:frames
switch md
case 16       % 16QAM
for 1 = 1:space dim
k1(:,1) = gam16(data(:,1,k) + 1,1);
k2(:,1) = qam16(data(:,1,k) + 1,2);
end
q(:,:,k) = ((2 * kl - md- 1) -i* (2 * k2 - md - 1) ) ;
otherwise
expr = 2 * pi * i / md;
q(:,:,k) = exp(expr * data(:,:,k));
end
sig_modul=q;
end
함수

Ta! 프로그램 10.9 시공간 6115 부호화기의 변조

415


===== PAGE 413 =====
PART II \4140와 MATLAB

function varargout = channel (sig,snr,no_rx)
eh, conf=[2 no_rx] ;

[sig length, space dim, frames] =size(sig) ;
spowr=sum(abs (sig(:,1,1)))/sig length;
sigma =sqrt (0.5*spowr* (10*(0.1*-snr) ) ) ;
const = sqrt (2);

ch_coefs=(randn(ch_conf(1),ch_conf(2),frames) +...
i*randn(ch_conf(1),ch_conf(2),frames))/const ;
ch_noise=(randn(sig_length,ch_conf(2),frames) +...
i*randn(sig_length,ch_conf(2),frames)) * sigma ;

for k = 1:frames
sig add(:,:,k) = sig(:,:,k)*ch_coefs(:,:,k);
end
sig corr = (sig add + ch noise);
varargout = {sig corr,ch coefs};

수

에

ial 프로그램 10.10 시공간 61115 부호화기의 채널

ㅁ

function [data_est,state_est] = detect (8190 down,dlt,slt,ch_coefs)
[step final,space _dim,frames] = size(sig_ down) ;
[s,md,foo] = size(dlt) ;
qam16=[1 1;2 1;3 1;4 1;4 2;3 2;2 2;1 2;1 3;2 3;3 3;4 3;4 4;3 4;2 4;1 4];
for k = 1:frames
metric(1,2:s) = realmax;
for 1 = 1:step final
for | = 1:5 % current j

[s_pre,foo] = find(slt == j);

pos = mod(j - 1,md) +1;

data_test = dlt(s pre,pos,:);

data_test = reshape (data_test, [md 2] ) ;

if md == 16 % 16QAM

나
ay
이 0 |
K
i

gqam16(data_test(:,r) + 1,1);
qaml6(data_test(:,r) +

BK
Ul

end

gq_test = (2* kl -md-1) -i* (2 * k2 - md - 1);
else % 4,8PSK

expr = i * 2 * pi / md;



===== PAGE 414 =====
end

제10장_공간 다이버시티와 시공간 부호화 기법

q_test = exp(expr * data_test) ;
end
metric_d = branch _metric(sig down(1,:,k),q_ test,ch_coefs(:,:,k));
metric_md = metric(1,s_pre)' + metric 0;
[metric _min,metric_pos] = min(metric_md);

metric(1] + 1,j) = metric_min;
vit_state(1 + 1,j) = s_pre(metric_pos) ;
vit_data(1 +1,j) = pos - 1;
end
end

(foo, state_best] = min(metric(end,:));
state_est (step final + 1) = state best;
for 1 = step final:-1:1
state_est(1) = vit_state(1 + 1,state_est(1+1));
data_est(1,:,k) = vit_data(]1 + 1,state_est(1 + 1));
end

=

ie) 프로그램 10.11 ABZ trellis 복호화기

에
>

0
4

function [fer] =count (data_src,data_est,varargin)
[fr_length,space_dim, frames] = size(data_est) ;
frame_err = sum(sum(data_src ~= data_est) >0) ;

err
all

= sum(sum(data_src ~= data_est))j;
= fr_length * frames;

if frame_err~=0

fer=frame_err/frames;

else

end

fer=0;

im 프로그램 1012 시공간 trellis 부호화기의 FER 함수

417

0000 (enn



===== PAGE 415 =====
공간다중화 방식을 사용하는 MIMO 시스템은 다이버시티 기법을 사용하는 MIMO 시
스템과 비교할 때 높은 ASKS 달성하지만 수신부에서 공간스트림을 분리해야 하는 어
려운 점이 있다. 본 장에서는 다양한 수신기술에 대해 알아본다. 송신 안테나의 개수가 ^
이고, 수신 안테나의 개수가 Ne 일 때, 송수신 ALSO] 관계가 다음과 같다고 가정한다.

y=Hx+z                              (11.1)

여기서, ¥= [Ye ne] 이고, 7,,/=1.2,…#, 은 / 번째 수신 안테나에서 =
신호이고, X=[ x25. ay, | 이과 x, f= 12,-N, 는 / 번째 송신 안테나에서 송신된 신
호이며, HY (j,i ) aq element 1, /=1,2,+)Ngsi=1,2,+,Npt= i 번째 송신 안테나와
7 번째 수신 안테나 사이의 채널               | 자제 | 이코 2-J=12,
N,& j 번째 수신 안테나에서 받은 Gaussian BES 갖는 잡음성분이다.

GEIR az we om

선형 검출 방식은 다수의 수신 안테나에서 받은 ASS 사용해, 특정 송신 안테나로부
터 보내진 신호를 검출할 때 다른 송신 안테나로부터 보내진 신호들은 간섭신호로 여기고
nulling 또는 감쇠시키는 검출 기법이다. 선형 검출 기법에는 2#기법과 44549기법이 있
다. ZFS 가중치 행렬을 다음 식과 같이 구한다.

W,, =(H"H) 0"                                  (11.2)

418



===== PAGE 416 =====
제11장_ 공간 다중화 MIMO 시스템의 신호검출 기법

MMSE 가중치 행렬은 아래와 같다.
\, =(H"H+071) 07                             01.3)

여기서 #" 는 H 2] Hermitian 전치 행렬이다. MMSES] 경우 잡음에 대한 사전정보인
0? 가 사용됨을 볼 수 있다. 일반적으로 개에 비해 MMSE7} 우월한 성능을 보이는데, 이
는 채널 이득행렬의 60ㅁ01400 number7} 클 경우 가중치를 BS 때 발생하는 잡음증폭이
MMSE2] 경우가 개에 비해 적기 때문이다. 따라서, SNRo] 낮아 잡음의 크기가 클 때,
MMSES ZF 2] 성능 차이가 크고, SNR] 높아 잡음의 크기가 작을 때는 두 가지 기법의
성능이 유사하게 된다. ZF 방식을 사용할 때 달성하게 되는 다이버시티 이득은
N,—-N, +1이다. 송신 안테나가 하나인 경우에는 개 검출기법이 MRRC(Maximal Ratio
Receiver Combining) 기법과 동일하게 되고 달성하는 다이버시티 이득은 ^, 이다.

GEERT osic wa 71

선형 검출 기법은 비교적 간단하게 하드웨어 구현이 가능한 방법이지만, 일반적으로 성
능이 만족스럽지 못하다. 이러한 열악한 ASS 개선하기 위해, OSIC(Ordered Successive
Interference Cancellation) 기법에서는 검출 순서에 따라 순차적으로 ASS 검출하고, |
출된 ASS 성분을 수신신호로부터 제거하여 아직 검출되지 않은 신호관점에서 간섭으로
작용하는 신호성분을 제거하여 성능을 향상시킨다211][212][2331. 이 때 신호의 검출 순
서는 전체 시스템의 성능을 결정하는 중요한 요인이다. 0810 검출 기법에 사용할 수 있
는 대표적인 SAS SHE 아래와 같이 4가지가 있다.

방법 1 : MMSE 가중치 행렬을 사용할 때 활용 가능한 기준으로서 검출 후 SINR(Signal
to Interference plus Noise Ratio)®] 있다. MSE(Mean Squared Error)7} 최소가
되도록 생성한 MMSE 가중치 VAS 또한 다음 식으로 표현되는 AS 후 SINR
을 최대화 한다.



===== PAGE 417 =====
PART Il_MIMO2} MATLAB

wh,|
E. 2 |wh| +o
i

(11.4)

여기서 &, 는 송신신호의 에너지를 나타내고, \, 는 A (11.3)으로 표현되는 MMSE 가중
치 행렬의 7번째 YS 나타내고, 8, 은 채널 이득 행렬의 / 번째 SS 나타낸다. SINRS
최적으로 하는 순서화는 신호검출과 동시에 이루어져야 한다. 처음에는 먼저 ^, 개의
SINRS 계산하여 그 중 가장 큰 값에 해당하는 ASS 식 (11.3)으로 표현되는 MMSE
해 검출한다. 두 번째 SINR] 큰 ASS 검출하기 위해서는 WAS
분을 수신신호로부터 제거하고, 식 (11.3)과 유사한 MMSE 가중치 Bas
때 식 (11.3)에 사용되는 채널 이득행렬은 원래의 채널 이득행렬에서
해당하는 SS 삭제한 새로운 행렬이다. 이 새로운 YAS 기반으로 다시
식 _ 유사한 방식으로 ^, -1 개의 SINRS 계산한다. 이중 가장 큰 SINR 해당
하는 ASS 다시 검출한다. 이와 같이 매 신호를 검출하고 다음 ASS 검출할 때 MMSE
가중치 및 SINR 연산을 다시 수행해야 한다. 따라서, 총 연산해야 하는 SINR! 개
1

as  Dias = (N, +1) o} ch.

4

oe
ot
6

: 식(11.2)로 표현되는 개의 가중치를 사용할 경우, 식(11.4)의 간섭(10160406006)
부분이 4, >,|\,0,|=0 이고, 1\,0, P =1이므로, 검출 후 SNR] 아래 식으로
[#i

{=                         (11.5)
o: |, |

검출과정 및 SNR! S14 MMSE-OSICS} 유사하고, 단지 SNR 계산이 SINR J
fe)
방법 3 : 방법 12 MMSE 가중치 행렬 및 SINR] 반복적 연산이 필요하다. 방법 1에 비

해 성능 면에서 열화를 초래하지만 연산복잡도를 감소시키는 방법으로는 채널
벡터들의 0000값에 따라 순서화 하는 방법이 있다. 이 방법은 다음의



===== PAGE 418 =====
y=Hx+z =hx, +h,x, +---+hy xy +2                  (11.6)

위 식을 통해 i Aa] 송신신호가 수신신호에 포함되어 있는 정도가 채널이득 행렬의 i
열의 normo]] 비례한다는 것을 관찰할 수 있다. ^, 개 열 벡터의 2007값들을 계산하

번째                      을
여 그 순서대로 신호를 검출할 수 있다. 이 방법을 사용할 경우 방법 1과는 달리 순서화를
한번만 하고 이 순서에 따라 ASS 검출하게 되므로 순서화를 위해 지불해야 하는 비용

방법 4 : 지금까지의 방법에서는 채널의 정보와 잡음의 통계적인 정보만
호검출이라 함은 수신신호가 가용할 때 송신신호를 검출하는 것으로서 수신신호
의 ABS 추가적으로 사용하여 검출순서를 결정할 수 있다[234]. 이 HAS 가
장 많은 정보를 사용하는 순서화 방식으로서 최적의 Bes 보이지만, 방법 1.2
는 달리 채널 이득이 고정되어 있을 때에도 매번 수신된 신호가 바뀌므로 이
에 따라 순서화를 다시 수행하여 신호를 검출해야 하므로 이에 따른 추가적인
연산복잡도가 소요된다. 방법 1과 2에서는 채널 이득 행렬이 고정되어 있다면
순서를 한번만 수행하고 검출은 그 순서에 따라 수행하면 된다.

본 절에서 기술한 0510 방법들을 사용할 때 달성하게 되는 다이버시티 이득은 모든 심
볼에 대해 4, -4,+1보다 크게 된다. 맨 처음 검출되는 심볼의 경우에도 순서화를 수행
하기 때문에 얻게 되는 추가적인 다이버시티 이득이 있다. 두 번째부터 마지막까지 검출
하는 신호의 다이버시티 이득은 그 전에 검출된 신호의 오류 여부에 따라 결정된다. 만약
그 전에 검출된 we 모두 올바르게 검출되었다고 하면, ; 번째 ASS 검출할 때 얻게
되는 다이버시터 이득은 Ng —N, +i 7} 된다. 이 때, 번째 검출신호는 순서화 때문에 i
번째 송신 el 송신된 신호와 다르다. 프로그램 11.1은 다양한 0810검출 기법들
이다. 그림 11.1은 3가지 0810기법들의 성능을 비교한다. 연산량이 가장 많은 검출 후
SINR 기준 순서화를 했을 때의 성능이 가장 좋고, 나음이 검출 후 SNR, 그리고 연산량이
가장 AZ column norm 기준 순서화의 성능이 가장 냐쁘다는 AS 관찰할 수 있다.

421



===== PAGE 419 =====
PART 11 MIMO2} MATLAB

function [X_hat]=Detector_OSIC(y, H, noise_variance,nT,OSIC_type)
6 Input parameters
OSIC_ type
- 1 : Post_detection_SINR
- 2 : Column_max
- 3: Post_detection_SNR
y : received signal ,nRx1

HP WP AP oP OP

oe

H : Channel matrix, nRxnT

oe

noise_variance
nT : number of Tx antennas

ae ol?

nR : number of Rx antennas
Output parameter

oe ol?

X_hat : estimated signal,nTx1
if OSIC_type ==1 % Post detection SINR
Order=[]; % detection order
index_array=[1:nT]; % yet to be detected signal index
% V-BLAST
for stage = 1:nT
MMSEE=inv (H'*H+noise_variance*eye(nT+1-stage))*H'; % MMSE filter
MMSEEH=MMSEE*H;
sinr_array=[];
for i =1:nT- (stage-1)
tmp= norm(MMSEEH (i, [1:i-1 i+1:nT-(stage-1)]))*2...
+ noise_variance*norm(MMSEE (i, :))*2;
sinr_array (i) =abs (MMSEEH (i,i))*2/tmp; % SINR calculation
end
[val_max, index temp] =max(sinr_ array) ;   % ordering using SINR

Order=[Order index_array(index_temp) ] ;
index_array= index_array([1:index_temp-1 index_temp+1:end] ) ;
x_temp (stage) =MMSEE (index temp, :) *y;    % MMSE filtering
x_hat (stage) =QAM16 slicer(x_temp(stage),1); % slicing
y_tilde=y-H(:,index_temp)*x_hat (stage); * interference subtraction
H_tilde=H(:, [1:index_temp-1 index _temp+1:nT-(stage-1)]); %* new H
H=H tilde; y= y tilde;

end

422



===== PAGE 420 =====
X_hat (Order) =x_hat;

elseif OSIC_type ==2 % column_norm ordering detection
X_hat=zeros(nT,1);
G = inv(H);         % inverse of H

for i=lsnT            column_norm calculation
norm_array(i) = norm(H(:,i));

end

[sorted_norm_array Order_temp] = sort (norm_array) ;

Order = wrev(Order_temp) ;

% V-BLAST

for stage=1:nT
x_temp=G (Order (stage) ,:)*y;   6 TX Signal estimation
X_hat (Order (stage) )=QAM16 slicer(x_temp,1); % slicing
y_tilde=y-H(:,Order (stage) )*X_hat (Order (stage) ) ;

end
else % OSIC with Post_detection_SNR ordering
Order={];

index array=[1:nT]; % set of indices of| signals to be detected

% V-BLAST

for stage = l:nT

= inv(H'*H)*H';
norm_array=[];
for i=1:nT-(stage-1) % detection ordering
norm _array(i) = norm(G(i,:));

end
[val_min, index_min]=min(norm_array); % ordering in SNR
Order=[Order index_array(index_min)];
index_array= index_array([1:index_min-1 index_min+1:end]) ;
x_temp(stage)=G(index min,:)*y; % Tx signal estimation
x_hat (stage)=QAM16 slicer(x_temp(stage),1); % slicing
y_tilde=y-H(:,index_min)*x_hat (stage); % interference subtraction
H_tilde=H(:,[1:index_min-1 index_min+1l:nT-(stage-1)]); % new H
H=Htilde; y = y_tilde;

end

X_hat (Order) =x_hat;

end

!

! 프로그램 11 08910 신호 검출 기법 함수

!



===== PAGE 421 =====
:    PART If_ MIMO2} MATLAB

10° -                                               _
[                                               Column norm 기준 순서화
--]-@- 검출후 SNR 기준 순서화
--7—-— 검출후 91 기준 SAS
10가                                               '      {
107
o
10°22:
10”      |      |      i      i      :      i      |      !      |
0     5     10    15 _ 20    25    30    35    40    45
SNR (dB)
그림 11.1 다양한 순서화 방법에 따른 OSIC 성능비교

00000 wi ae

ML(Maximum Likelihood) 검출 방식은 송신 가능한 AS 벡터들을 모두 고려하여 i
래 식 (11.6)으로 표현되는 메트릭 값을 최소로 하는 송신 벡터를 찾아내는 방식

신심볼 벡터의 AS 확률이 모두 같을 때 최적의 성능을 달성한다. 그러나 송신   안테나 수 a
와 (또는) 변조차수 eee order)7} 중가함에 따라 소요되는 계산량이 지수함수적으

로 증가하게 된다[235]. WAS 위해 사용되는 성상도 상의 심볼들의 집합을 Ce} 하고 이

집합의 6810148114를 |0|로 표시할 때, 필요한 ML 메트릭 연산 횟수는 10| "로 표현할
수 있다.

X =arg min lly - Hx||                                                (11.6)

이 방식은 일반적으로 하드웨어로 구현하기에는 어려움이 있고, aise Bees

새로운 신호검출기법을 제안할 때 비교대상이 된다. [235]에서 ML 신호검출을 위해
|0|”회의 ML 메트릭 연산을 |C|*" '회로 줄일 수 있음이 증명되었다. [235]의 MML
(Modified ML) 기법은 ^, =2 인 경우에는 아주 적합한 방식이나, ^, 23 인 경우에는

"24



===== PAGE 422 =====
여전히 복잡도가 높다는 단점이 있다.

11.1절의 선형 검출 기법과 11.2절의 0510 검출 기법들은 본 절의 ML 검출 기법에 비
해 매우 낮은 연산복잡도를 보이지만 큰 성능 열화를 보인다. 그러므로 본 절의 ML 신호
검출 기법을 기반으로 하되 높은 연산복잡도를 낮추어 하드웨어 구현이 용이하면서 동시
에 50Ｌ에 근접한 성능을 보이는 다양한 준최적 신호검출 기법들이 연구되고 있다.

function [X_hat]=ML_detector(y, H) ;
QAM table2 = [-3-31, -3-i, -3+31, -3+1, -1-3i1, -1-i, -1+3i, -1+i,
3-31, 3-1, 3+31, 3+1, 1-31, 1-i, 1+3i, 1+i]/sqrt(10);
metric = 100000;
for 1 = ii 16
x_temp(1) = QAM table2(1);
Estiyl(:,1) =y - H(s;1)«*x1_temp;
for m= 1:16
x_temp(2) = QAM table2(m) ;
0864. V2 (2,1) = Esti -yi(#,1) - H(z,2) .*x2 ‘temp;
fer am = 116
x _temp(3) = QAM table2(n) ;
Esti_y3(:,1) = Esti_y2(:,1) - H():,3).*x3_temp;
Por © = 1:16
x_temp (4)    QAM table2(o);
Esti_y4(:,1) = Esti_y3(:,1) 47 H(:,4) .*x4_temp;
metric _temp = sqrt (Esti_y4(:,1)'*Esti_y4(:,1));

if metric_temp < metric
X_hat = x_temp;
metric = metric_temp;

end

end
end
end
end

A

Tm! 프로그램 11.2 ML 신호검출 기법 함수

[에



===== PAGE 423 =====
|. 11.4 sphere  Decoding 기법

SD(Sphere Decoding) 기법은 ML 신호검출과 같이 ML 메트릭을 최소로 하는 송신신
호 벡터를 찾지만, 모든 가능한 송신신호 벡터를 고려하는 대신 특정 600606안에 존재하는
벡터들만 고려함으로써 그 연산량을 줄이는 방식이다236][237]. QAM 맵핑을 사용하는
시스템은 실수부와 허수부를 구별하여 표현할 수 있다. 2x2 MIMO 시스템의 경우를 예로
들어 복소수 시스템(6007016% 579[60)의 실수 시스템(6681 system) °°) 변환과정을 설명
하면 다음과 같다. 송수신 신호의 관계는 아래 식과 같이 HS] 가능하다.

i + Mr |i + fly Moe + Thr, |= + Py 시저 내기 |         (11.7)

Vor + I>     쓰2 + My, Pop + Hyp || Xap + Pry     228 + JZ)

여기서, 은 J Bal 수신안테나에서 수신한 복소신호의 AP HS 나타내고, Vr 는 허
수부를 나타내며, Min Min Xin %r> Zin» Zu 유사하게 정의된다.
위 식으로 표현되는 시스템의 설수부는 다음 식으로 표현된다.

i 이조  Inyp |  i  hy; lk   ic
Yor   oir Mor |LXor    hy, Ny,         2208

-                i                     (11.8)
_ Fiz Mor ~My 427 te |  2R +i |
Pyg Mg ~My ~My, |)   222
27

가 =| hoor Muar ee 27 시제               (11.9)
Var   Fy, 07 yy Irene || Xr    227

식 (11.8)과 (11.9)로부터 다음 AS 얻을 수 있다.

_ 426



===== PAGE 424 =====
제11장_

Vir    Faiz Prop ~My — Mor || Ge    ZiR
Vor | _ Iya Map ~My — Mp, || Xe   224

=                       +
217      Par Mar Mare or |] Xr      Zi)                      (11.10)
227      Fy 2720 yp ne || Xa      227
Sa eee             ~            —     ——
y                        H                     x           z

11.10)으로 표현되는 실수 시스템에 SDAS 방식이 적용된다. 90에서는 아래의 관

이용한다.

I 8
flo

Al

arg min|y - Ax| =argmin(x-%) Hi Hi(x-*)          (11.11)

SAMA 증명한다. 9에서는 다음 식으로 Ease aar ree “Eee whe} gat 고
려한다.

x-i) H’A(x-2 < R2,                    (11.12)
(X-x) HA(x-x)<R;

(11.13)

식 (11.13)의 행렬 RS 채널 이득 행렬을 08분해하여 얻어진 행렬을 나타낸다. 4
(11.13)을 기반으로 92과정을 N,=N, = 2 로 가정하여 예를 통해 설명한다. 식 (11.13)
은 다시 아래와 같이 표현이 가능하다.

x, =x
hy 12 Ns Na 1 1

2

0 hy 3 Ny |] 2 —%       +

0 0    _ oan =u (% -%) vk -%,)+1,(%, -%,]
18 "ha || X, —&

00 0 mile,

427


===== PAGE 425 =====
PART 비 MIMO2} MATLAB

2

rn (¥,   -¥,)+7;(X,    -%,) +n, (x,    -%,|
(11.14)

2

in (% —% ) +72 (% -% ) +75 (% -  -%,)+n%, 년    -x,}

Al (11.12)와 4] (11.14)를 결합하면 SDA] 고려하는 90066는 아래와 같이 표현된다.

2                                2

+

2

+                        조조   -,)+r,(X,    —%, +7, (5,    -%,)

733 (x, -%,) +N, (x, =i, |

hy (% -%    %) hin (% ~x,) +7, (%,  -x,) +7, (¥ -%,)

EA -x,]
(11.15)

=                                                                                   ZR.

식 (11.15)로부터 출발하여 SDE 아래의 4단계로 진행된다.

Nie
단계 1 : "게티 -i) = 안에 존재하는 x, 값을 아래의 upper/lower bounds 만족

하는 임의의 값으로 선택한다.

_ + R
=4,63,+——                (11.16)

4

때         Pt  x  2
단계 2 : 063) +n (%-%) +n, (%-¥,)) SR, 내부에 존재하는 ZS 다시
아래의 upper/lower bound= 사용하여 임의로 한 개 선택한다. 이 때 지은 단

계1에서 선택한 값을 나타낸다.

조프 고
Ro — a He —X,)) -

53

Iq (%q -지)  115

2      = al     => oA
스   Ro —|Puu &, - 4)  = Tag %q ~)
x; —

IA
xp

SX,  +

733

위 구간에 해당하는 × 가 존재하지 않을 경우 ×,값을 단계1에서 얻은 다른 값과 다른
값으로 대치하여 식 (11.17)을 다시 연산한다. 만약 식(11.16)을 만족하는 모든 가능한 x,
를 대입하였음에도 불구하고 해당하는 × 가 존재하지 않을 경우 반지름 ^; 을 더 큰 값
으로 갱신한 후, 단계 1을 수행한다.

428



===== PAGE 426 =====
단계 3 : 단계 1과 2에서 선택한 값을 각각 x,, x, 라 하고 ChE sphere 내부에 존재하

(11.18)

선택 방법은 단계 22+ 유사하게 upper/ lower bound= 이용한다. 위 구간에 해당하는
× 가 존재하지 않을 경우, % WS 다른 값으로 대치하여 식 (11.18)을 다시 연산한다. 만
약 모든 가능한 × 을 대입하였음에도 불구하고 해당하는 × 가 존재하지 않을 경우, ×

다른 BOR 대치하여 단계2부터 다시 진행한다.

tuo

단계 4 : 단계 1~3에서 선택한 값을 각각 X,, =, 도라 하고 다음 50866 내부에 존재하

2

9 (% —%) +1, (x, —%,) +1, (%, -%,}

2

+l (% 3) +72 (% -x,) +73 (% -%) +7, (¥, -%,)

= Rey

선택 방법은 단계 2.3과 유사하게 42060 lower bound= 이용한다. 위 구간에 해당하는
x 가 존재하지 않을 경우, × 값을 다른 값으로 대치하여 식 (11.19)를 다시 연산한다. 만
약 모든 가능한 × 을 대입하였음에도 불구하고 해당하는 ㆍ 가 존재하지 않을 경우, HS
다른 GOS 대치하여 단계 3부터 다시 진행한다. 위 과정을 거쳐 X,, =, ×, oe 선택
하면 선택된 송신신호에 해당하는 반지름을 계산한다. 계산된 새로운 반지름을 사용하여

429

00009 00008)



===== PAGE 427 =====
PART Il_ MIMO2t MATLAB

다시 단계 1부터 시작한다. 송신신
부에 존재하는 유일한 신호

\Ｌ기반의 준 최적 검출기법들의 성능은 11.5절의 QRM-MLD 기법 설명 후 비교한다.

ue
코

cu it
~
°     illo
ol
au
eo
문
{KI
Hu
니
is
자
N
rs)
oh
nu
N
2또
으
=

function [X_hat]=Detector_SD(y,H,nT)
Input parameters

ae ol?

y : received signal, nRx1

H : Channel matrix, nRxnT

nT : number of Tx antennas
Output parameter

X hat : estimated signal, nTxl

HPF AP oP ol?

global x_list;       % candidate symbols in real constellations
global x_now;        % temporary x_vector elements

global x_hat;        응 inv(H) *y

global x_sliced;      % sliced x_hat

global x pre;        % x vectors obtained in the previous stage
global real_constellation; % real constellation

global R;            6 Rin the QR decomposition

global radius squared; % radius*2

global x metric;      % ML metrics of previous stage candidates
global len;           % nT*2

j=sqrt (-1);

QAM table2 = [-3-31, -3-i, -3+31, -3+1, -1-3i, -1-i, -1+3i, -1+i,3-3i,
3-1, 343i, 3+1, 1-31, 1-i, 1+31, 1+i)/sqrt(10); % 16—-QAM

real_constellation = [-3 -1 1 3]/sqrt(10);
y =[real(y); imag(y)];    % y : complex vector -> real vector
H =(real(H) -(imag(H)) ; imag(H) real(H)];

% H : complex vector -> real vector

len = nT*2; % complex -> real

x list = zeros(len,4); % 4 : real constellation length, 16-QAM
x_now = zeros(len,1);

x hat = zeros(len,1);

xX_pre = zeros (len,1);

X_ metric = 0;



===== PAGE 428 =====
[Q,R] = QR_Decom_nR_nT(H) ;    % nR x nT QR decomposition
x_hat = inv(H)*y;             % zero forcing equalization
x sliced = QAM16_real_slicer(x_hat,len)'; % slicing

radius squared = norm(R*(x_sliced-x_hat))*2; % Radious*2
transition = 1;
% meaning of transition
% 0: radius*2, 1~len : stage number
% 160+1 : compare two vectors in terms of norm values
% len+2 : finish
% transition tracing
0 : stage index increases by +1

flags= 1;

1 : stage index decreases by -1
2 : 1->len+2 or len+1->1
while (transition<len+2)
if transition ==     % radius _squared*2
[flag,transition, radius squared,x list]
= radius_control (radius_squared, transition) ;
elseif transition <= len
[flag,transition] = stage_processing (flag, transition) ;
elseif transition == len+1 %
[flag,transition] = vector_norm_comparison (transition) ;
end
end
ML = x _pre;
for i=1l:len/2
X hat (i) = ML(i)+j*ML(i+len/2) ;
end

function [flag,transition] = stage processing (flag, transition)
Input parameters
flag : previous stage index
flag = 0 : stage index decreased
-> X_now empty -> new x_now
flag = 1: stage index decreased -> new x_now
flag = 2 : previous stage index =len+1
-> If RoR'> start from the first stage
transition : stage number
Output parameters
flag : stage number is calculated from flag
transition : next stage number, 0 : R¥2, 1: next stage,
len+2: finish

a oP ol?

oe ol?

a iP 00 ㅇㅇ



===== PAGE 429 =====
PART Ill_MIMO&} MATLAB

global x list;

global x_ metric;

global x_now;

global x_hat;

global real_constellation;
global R;

global radius_squared;
global x_sliced;

stage index = length(R(1,:))-(transition-1) ;

if flag == 2 % previous stage=len+1 : recalculate radius R'
radius squared = norm(R*(x_sliced-x_hat) )*2;

end

if flag ~= 0 % previous stage=len+1 or 0

-> upper and lower bound calculation, x_list(stage_index, :)
[bound_lower bound_upper] = bound(transition) ;
for i=1:4 % search for a candidate in x_now(stage_index) ,
% 4=size(real_constellation), 16-QAM assumed
if bound_lower <= real_constellation (i)
&& real_constellation(i) <= bound_upper
list_len = list_length(x_list (stage_index,:))j;

x_list (stage_index,list_len+1) = real_constellation(1) ;
end
end
end
list_len = list_length(x_list (stage_index,:));
if list_len == 0    % no candidate in x_now
if x metric == 0 || transition ~= 1
% transition >=2 > if no candidate > decrease stage index
Elag = 0;
transition = transition-1;
elseif x_metric ~= 0 & transition ==
% above two conditions are met > ML solution found
transition = length(R(1,:))+2; % finish stage
end
else            % candidate exist in x_now > increase stage index
flag = 1;

transition = transition+1;
x _now(stage_index) = x_list (stage_index, 1) ;
x_list(stage_index,:) = [x_list (stage_index, [2:4]) 0];



===== PAGE 430 =====
function [bound_lower bound_upper] =ㅁ0400 (transition)
Input parameters

R: [이포] = 98808)

radius squared : R*2

transition : stage number

x hat : inv(H)*y

x now : slicing x_hat
Output parameters

bound_lower : bound lower

bound_upper : bound upper

oe

HP AP al? oP A OP Of 1?

global R;
global radius squared;
global x_now;
global x_hat;
len = length(x_hat) ;
temp sqrt = radius_squared;
temp_k=0;
for i=1:1:transition-1
temp _abs=0;
for k=1 21:1
index 1 = len-(i-1);
index_2 = index_1l+ (k-1);
temp_k = R(index_1,index_2)* (x_now(index_2)-x_hat(index_2))j;
temp_abs=temp_abs+temp_ k;
end
temp sqrt = temp_sqrt - abs(temp_abs) *2;
end
temp sqrt = sqrt (temp_sqrt) ;
temp_no_sqrt = 0;
index_1 = len-(transition-1) ;
index_2 = index_1;
for i=1:1:transition-1
index 2 = index_2+1;
temp_i = R(index_1,index_2)* (x _now(index_2)-x_hat (index 2));
temp _no_sqrt = temp no sqrt - temp_i;
end
temp lower = -temp sqrt + temp_no sqrt;
temp_upper = temp_sqrt + temp_no sqrt;
index = len-(transition-1) ;
bound lower = temp_lower/R(index,index) + x_hat (index) ;

433



===== PAGE 431 =====
PART 비 MIMO2} MATLAB

bound_upper
bound_upper
bound_lower

temp_upper/R(index, index) + x_hat (index) ;
fix (bound_upper*sqrt (10) ) /sqrt (10) ;
ceil (bound_lower*sqrt (10) ) /sqrt (10) ;

function [len]=list_length(list)
Input parameter

list : vector type
Output parameter

len : index number

00 ol?

HP oP

len = 0;

for 1=134
if list (i) ==0,   break;
else       len = len+1;
end

end

function [flag,transition, radius_squared,x list]
radius_control(radius_squared, transition)
Input parameters
radius squared : current radius
transition : current stage number
Output parameters
radius squared : doubled radius
transition : next stage number
flag : next stage number is calculated from flag
global len;
radius squared = radius squared*2;
transition = transition+1;
flag = 1;
x_list (len, :)=zeros (1,4);

00 il

oe

ae ole

00 oP ㅇㅇ

function [check] =vector_comparison(vector_1,vector_ 2)
check if the two vectors are the same
Input parameters

pre x * weetor 1

now x : vector 2
Output parameters

check : 1-> same vectors, 0-> different vectors
check = 0;
lenl = length(vector_1); len2 = length(vector 2);

oe

ae AP ol?

00 ㅇㅇ

434



===== PAGE 432 =====
제11장_ 공간 다중화 MIMO 시스템의

if 1601 ~= 1602
error('vector size is different');
end
for column_num = 1:lenl
if vector_1(column_num,1) == vector_2(column_num, 1)
check = check + 1;
end
end
if check == lenil, check = 1;
else   check = 0;
end

function [flag, transition] =vector_norm_comparison (transition)
% stage index increased(flag = 1) : recalculate x_list (index, :)
% stage index decreased(flag = 0) : in the previous stage,
no candidate x now in x list
Input parameters

flag : previous stage

transition : stage number
Output parameters

flag : next stage number is calculated from flag

transition : next stage number
global x _ list;
global x _pre;
global x metric;
global x_now;
global x_ hat;
global R;
global radius squared;
global x_sliced;
global len;
vector identity = vector_comparison(x_pre,x_now) ;
% check if the new candidate is among the ones we found before
if vector_identity ==

% if 1 ML solution found

len total = 0;

for i=l:len % if the vector is unique > len total = 0

len_total = len_total + list_length(x_list(i,:));
end
if len total ==       * ML solution vector found
transition = len+2; % finish

00 oP ㅇ0 AP oP Ol?



===== PAGE 433 =====
PART 11 _110와 MATLAB

flag = 1;

else                  % more than one candidates
transition = transition-1; % go back to the previous stage
flag =0;

end

else % if 0 > new candidate vector is different from the previous
candidate vector and norm is smaller > restart
x sliced_temp = x_now;
metric temp = norm(R*(x_sliced_temp-x_hat))*2;
if metric_temp <= radius squared
% new candidate vector has smaller metric > restart
X pre = X_now;
x metric = metric_temp;
x sliced = x_now;
transition = 1;      % restart
flag = 2;
x list=zeros(len,4); 6 initialization

f°)

x now=zeros(len,1); <% initialization
else % new candidate vector has a larger ML metric
transition = transition-1; % go back to the previous stage
flag =0;
end
end

oo
+

lm) 프로그램 11.3 Sphere Decoding BB7|4

OEM orw-Mip 검출기법

QRM-MLD= 채널 행렬의 QR 분해한 결과에 7 알고리즘을 적용한 방법이다[238]
[239]. 11.4절의 90기법에서는 실수 시스템(6681 system)2] QRZ} 사용되었고, 본 절
의 0084-541Ｌ에서는 허수 시스템(6000016 system)2] 008분해가 사용된다. 송수신 안테
나 수가 동일한 것을 가정하고, 채널 행렬 피의 QR 분해를 통해 아래와 같이 ML 메트
릭의 등가적 표현이 가능하다:

ly -41=16 — Rx] =|" [y -QRx]]=[y ~ Ra                 (11.20

436



===== PAGE 434 =====
제11장_ 공간 다중화 MIMO 시스템의

식 (11.20)의 ML 메트릭을 이용해서 QRM-MLD7} 수행된다. 용이한 ABS 위해
N, =, =4 로 가정하여 예를 통해 설명한다. 식 (11.202 아래 식으로 다시 표현이 가

—
능하다.
"                           2
J     11 "12 713 Na |} %
.      2     dy     0%) hs Na || %      "3        2
y — Rx =|] |-                   =|p — HX,
O 0 2422.18      + ile
V3              33/34 |] %                                             (11,21)
Dy   0. 0 0 호
2 」~                      개                            2
+|); -    13x     Taka  +5, - 7522 — 133% — FX,  + | THX THX 7133 — FigX,|

Al (11.21)에서 출발하여 QRM-MLD 신호검출은 4단계로 구성된다.

단계 1 : |, —ryx,{ 를 작게 하는 지의 후보군 HCl a 중)를 선택한다.

단계 Oy li, — 1X4} +|5, — 13%, —r,x,| 를 작게 하는 벡터 [x, ×] 를 Mx\C| 개중 M
개 선택한다.

단계 3 :  IF, = r4gX,) +15; - 7338 —14x,f + Hy Xy 7334 = 1%, 를 작게 하는 벡터
[x x, 4) 를 Mx|c|l We 2/개 선택한다.

단계 4 : Al (11.21)로 표현되는 ML 메트릭 값을 가장 작게 하는 벡터 [< x, x x,] 를
Mx\C| ASA 선택한다.

QRM-MLD2Y| 성능은 파라미터 74값에 따라 결정된다. 파라미터 24 Zo] 크면
QRM-MLD 성능은 ML 성능에 근접하게 되지만 복잡도가 증가하고, 작은 27 값을 사용
하면 복잡도는 감소하지만 성능이 열화 되는 trade-off 관계에 있다. 11.4절의 5기법의

As MLAS 동일하다. 그림 11.3은 90기법의 성능과 파라미터 Wo] 다양한 값일
때 QRM-MLD2] 성능을 비교한다.

function [X_hat]=Detector_QRM MLD(Y,H)
Input parameters

Y : received signal, nTx1

H : Channel matrix, nTxnT

M : Parameter M in M-algorithm

HP AP 00 ㅇㅇ

437



===== PAGE 435 =====
PART 141 MIMO2} MATLAB

nT : number of Tx antennas
Output parameter
X hat : estimated signal, 701
global QAM table;
global Q;
global R;
global Y_tilde;
global nT;
global M;
QAM table = [-3-31i, -3-i, -3+3i1, -3+i, -1-3i, -1-i, -1+3i, -1+i, 3-3i,
3-i, 3+31, 3+1, 1-31, 1-i, 143i, 1+i]/sqrt (10); % QAM table
[QR] = qr(H); % QR-decomposition
Y_tilde = Q'*Y;
symbol replica = zeros(nT,M,nT); % QAM table index
for stage = 1:nT
symbol replica = stage_processing(symbol replica,stage) ;
end
X_hat = QAM table(symbol replica(:,1))j;

aH WP ol?

function[symbol_ replica] = stage _processing(symbol replica, stage)
Input parameters

Y tilde : Q'*y

R: [QR] = qr(H)

QAM table :

symbol replica : M candidate vectors

stage : stage number

M : parameter M in the M-algorithm

nT : number of Tx antennas
Output parameter

symbol replica : M candidate vectors
global nT;
global M;
if stage == 1; m=1; else m = M; end
symbol _replica_norm = calculate _norm(symbol replica, stage) ;
[symbol _replica_norm_sorted, symbol replica_sorted]
sort_matrix(symbol_replica_norm) ;
* sort in norm order, data is in a matrix form
symbol _replica_norm_ sorted = symbol _replica_norm_sorted(1:M) ;
symbol _replica_sorted = symbol replica_sorted(:, [1:M]);
if stage>=2

for i=1l:m

oe

oe

HF WP WP WP IP oP 00 Ol?

we ㅣ |

438



===== PAGE 436 =====
다중화 MIMO 시스템의 신호검출 기법

symbol replica_sorted([2:stage],i) =

symbol replica([1:stage-1],symbol_ replica_sorted(2,i), (nT+2) -stage) ;

end
end
if stage == 1 % In stage 1, size of symbol _replica_sorted is 2xM,

the second row is not necessary

symbol_replica([1:stage],:, (nT+1)-stage)=symbol_replica_sorted(1,:);
else

symbol _replica([1:stagel,:, (nT+1)-stage) = symbol_replica_sorted;
end

function [symbol_replica_norm] =calculate_norm(symbol_replica, stage)
Input parameters

¥_ tilde: + O**Y

R: [QR] = 0208)

QAM table

symbol replica : M candidate vectors

stage : stage number

M : M parameter in M-algorithm

nT : number of Tx antennas

A AP WP oP

oH ol?

de oP ol?

Output parameter
symbol replica_norm : norm values of M candidate vectors
global QAM table;
global R;
global Y tilde;
global nT;
global M;
if stage ==1; m=1; else m=M; end
stage index = (nT+1) -stage;
for i=l:m
X_temp = zeros(nT,1);
for a=nT:-1: (nT+2)-stage
X_temp(a) = QAM table(symbol_replica((nT+1)-a,i,stage_index+1) ) ;

o\?

end

X_temp([(nT+2)-stage: (nT)]) = wrev(X_temp([(nT+2)-stage: (nT)]));
% reordering

Y_ tilde now = Y_tilde([(nT+1)-stage: (nT)]);
% Y_tilde used in the current stage

R_now = R([(nT+1)-stage: (nT) ] , [(nT+1)-stage: (nT) ] ) ;

% R used in the current stage



===== PAGE 437 =====
PART I] )4104/0와 MATLAB

for k = 1:length(QAM table) % norm calculation,
% the norm values in the previous stages can be used, however,
we recalculate them in an effort to simplify the MATLAB code
X_temp(stage_index) = QAM table(k) ;
X_now = X_temp([(nT+1)-stage: (nT)]);
symbol _replica_norm(i,k) = norm(Y_tilde_now - R_now*X_now) “2;

end

end

function [index_number] = find_vector (range, target) ;
Input parameters
target : target vector

Output parameters
index number : the index of range that corresponds to target
for index_number=1:size (range, 2)
if range(:,index_number)==target, break; end
end

옹
ㅇ
옹
(이
%    range : the range of target vector
%
&
(이

function [entry 80660 entry_index_sorted] = sort_matrix(matrix_form)
Input parameters

matrix form : a matrix to be sorted

M : parameter M in M-algorithm
Output parameters

entry_sorted : increasingly ordered norm

entry index_sorted : ordered QAM table index
row size,column_size] = size (matrix form) ;
flag=0; % flag = 1 >the least norm is found
vector form=[];
entry _index_sorted =[];

mr oP oP WP oP 00 ON?

[0

for i = 11709 8126 % matrix form > vector form
vector form = vector form matrix_form(i,:);
end
for m=1:row_size*column_size
entry_min = min(vector_form) ;
Elag=0;
for i = 1:row_size
if flag==1 break; end
for k = 1:column_size
if flag==1 break; end

440



===== PAGE 438 =====
entry_temp = matrix_form(i,k) ;

if entry_min == entry_temp
entry_index_sorted = entry index sorted [k; i];
entry sorted(m) = entry temp;
vector _form((i-1) *column_size+k) =10000000;

flag=1;
end
end
end
end
ig) 프로그램 11.4 QRM-MLD 검출기법 함수
10 [                               =
3-@- QRM-MLD, M=4
-&- QRM-MLD, M=16
10"                                        —— Sphere decording
107
aa)
10°
107       |              !       |
0      5      10     15     20     25     30     35
SNR (dB)

그림 11.3 SD2} Q@RM-MLD(7 = 4,16) 성능 비교
(QRM-MLD, 427 =16 성능과 6ㅁ의 성능이 동일하여 성능커브가 BAA)

(NIST Lattice 800401101을 wget 기법

으로 하는 0510 기법에서는 선형검출 과정에서
잡음 SS 의해 성능열화가 초래된다. 채널 이득행렬의 60ㅁ01400 number7} 크면 가중치
를 수신신호에 곱하는 과정에서 잡음이 크게 증폭되기 때문이다. 180106 16040007은
latticeo] 좋은 기저를 찾는 방법으로 LLL(Lenstra—Lenstra—Lovasz)3} 같은 알고리즘을
이용하여 채널 Be} condition numbers 감소시킨다. 그림 11.4의 위쪽의 기저를 다음

re
oft!
a
iN
pa
rE
ye
rx
oft!
마녀
nye
그
re
ito
건
ie

441


===== PAGE 439 =====
PART Il. MIMO2} MATLAB

re

An orthogonal basis
That spans the same lattice

그림 11.4 초기 채널 행렬의 기저와 11166 reduction 과정을 거친 채널 행렬의 기저

그림과 같이 직교 기저 혹은 직교에 가까운 기저를 찾음으로써 60001100ㅁ numberS 감소시
킨다. Lattice reductionS 수행하여 얻어진 새로운 가상 채널 ue 이용하여 MMSE,
0810와 같은 선형 및 비선형 검출 기법을 수행하면 잡음 증폭을 크게 줄일 수 있다
[240][2411.

14&40기법에서도, QRM—MLD#}4]0]U} SD(Sphere Decoding) 방식에서 사용하는 채
널 행렬 표의 QRS 이용하여 시작한다.

y =Hx+z =QRx+z                 (11.22)
식 (11.22)의 양변에 @" 을 곱하면 다음식이 유도된다.
y=Q”y=Rx+zZ                  (11.23)

여기서 QUAL unitary 행렬이기 때문에 잡음항의 SAA 특성은 변하지 않는다.
주의할 AS 원래 행렬 HL} 행렬 R Y condition number7} 동일하다는 것이다. 따라서
식 (11.23)을 이용해서 를 이용하는 방법은 심한 잡음 증폭을 초래하게 된다. 식
(11.22) 및 (11.23)의 0#분해가 필요하지 않는 검출기법들도 존재하나, 삼각행렬의



===== PAGE 440 =====
제11장_ 공간 다중화 MIMO 시스템의 신호검출 기법

condition number 감소시키는 절차가 일반행렬에 비해 단순하다. 삼각행렬 Ro} 주어
졌을 때 00001400ㅁ numberS 감소시키는 방법을 알아본다.

11.6.1 ㄴ 알고리즘

4x4 MIMO 지스템을 예를 들어 설명한다.|행렬 Ro] 4×4위 경우, 우선 T=L,
ㅅ=2,7=1로 초기화하고. w= "R(LA)/R(L)), 를 구한다. 만약 /《<※0이면, 식
(11.24)와 A} (11.25)에 의해 RI} TS 변형한다.

—s

22. 지키              (11.24)
=, —Mt,,,§=1,2,--,N;             (11.25)
4) (11.25)으로 변형된 행렬 Ro} 식(11.26)을 만족시키지 못할 경우 R(.k-1) ot

R(:,k) 의 a 치를 교환 eam, aR O} 상삼각행렬40067 triangular)S 유지하기 위해 4]
(11.27)을 수행한다.

Of, She tH,                                           (11.26)

R(k-1:k,k-1:N,)=OR(k—1:k,k-1:N,)            (11.27)

여기서 1/4< 651, OF 회전 BYA(rotation matrix\2A] 식 (11.28)과 같다.

o-|“ A _  R(k-Lk-1)     R(k,k-1)    TT

1-6       R(k 1:4, -1)]    ~ IR  k-1:k,k-1)|

식 (11.265 만족한 경우에는 kak+1S 증가시키고, 만족시키지 못한 경우에는
kK=k-12 감소시킨다. 이 과정을 KAN, +1 될 때까지 반복한다.

일반적인 N, x N, 140040시스템에 st lattice reduction 과정을 수행하는 LLL 알고
리즘이 표 11.1에 정리되어 있다.

443


===== PAGE 441 =====
PART Ill. MIMOS} MATLAB

표 11.1 LLL 알고리즘

T=.
while (k < N,)
For j=k-1: -1: 1
w= 6 R(LA)/R(L) ,
if w#0
1 - 7. — Lh; > Lan = -/,
End
End

if Ofek > Tes a Tuk
R(jk-Iek) = Rbk 1)
T(,4-1:k)=T(:,4:k-1)
R(k-1,k-1)     R(k,k-1)  8 _ [3 A
86 (k-1:k,k-1)]  86 (k-1:k,k-1)]   Ba
R(k-1:k,k-1:N,)=OR(k-1:k,k-1:N,)
Q(.4-1:k)=Q(.k-1:k) 0"
k = max( [k-1 2] )
else
k=k+1
End
End

Wy} Lattice Reduction 기법의 활용

앞 절에서 ASH lattice reduction AAO] 의해서 얻게되는 HBS RS Reesicca Zt St
A 다음의 관계가 성립한다.

묘 =                    (11.30)

out               reduced ~ out

이러한 11006 reduction 기법은 다양한 검출기법들과 Aso] 가능하다. Lattice reduction
기법을 선형 MMSE 검출기법과 결합하여 사용한 BPS 예로 들면 다음과 같다.
위 절차에 의해 식 (11.23)이 다음 식으로 변형된다.

F = R ogee TX +2                   (11.31)

reduced

식 (11.31)2} 는 4} (11.23)의 Ro 비해 같거나 다른 작은 condition numbers
가지게 된다. 또한 T BAS unimodular] determinant7} ‘1’o] 된다. 따라서 =
라 하면 다음 식을 구할 수 있다.

444

a



===== PAGE 442 =====
간 다중

WEE
| R reduced

R

reduced

A] (11.33) 22 구한 AS slicing ttt.

위에서 구한 값을 통해 송신신호는 아래와 같이

화 MIMO 시스

+ ol) Ro cca

reduced

(11.33)

(11.34)

(11.35)

프로그램 11.5 lattice reductionS 활용한 MMSE 검출 기법 코드이다. 그림 11.5는

lattice 760400800에 의한 성능 개선을 나타낸다.

function [X_ Estimated] =
Lattice Reduction with MMSE
Input parameters
H_ complex :
y : complex received signal, nRx1l
noise variance : noise variance
Output parameters

X_Estimated :

HP WP WP WP ㅇ00 OP OP

estimated signal, nTx1

Nt = 4; Nr = 4;   = 2*Nt;

H_ real=[[real(H_complex) -imag(H_complex)];

2

LRAD MMSE (H_complex,y,noise variance, delta)

complex channel matrix, nRxnT

{imag (H_complex)

real (H_complex)]]; * complex channel -> real channel



===== PAGE 443 =====
PART 미_ )4140와 MATLAB

= [8 17681;80ㄴㄴ(ㅁ0186 variance) *676 (피) ] ;
y_real=[real(y);imag(y)]; % complex y -> real y
y=l[y_real; zeros (N,1)];

[Q,R,P,p] = SQRD(H) ;       % sorted QR decomposition

[W,L,T] = original LLL(Q,R,N,delta); % W*L = Q*R*T

H tilde = H¥P*T;          > H*P = Q*R

X_temp = inv(H_tilde'*H tilde)*H_tilde'*y; % MMSE detection
X_temp = round(X_temp) ;    % slicing

X_temp = P*T*X temp;
for i=1:Nr % real x -> complex x
X_Estimated(i) = X_temp(i)+j*X_temp(i+4) ;

end

function [Q,R,T] = original_LLL(Q,R,m, delta)
Input parameters

Q : orthogonal matrix, nRxnT

R : Rwith a large condition number

m : column length of H

delta : scaling variable
Output parameters

Q : orthogonal matrix, nRxnT

aH WP cP WP oP WP WP Ol?

: R with a small condition number

oe

R

T : unimodular matrix
=eye(m); T=P; k=2;

while (k <= m)

for j = k-1s=1:1

round (R(j,k)/R(j,3));

Foy

)
j,k) =R(1:3,k)-mu*R(1:5,5);
:,k)=T(:,k) -mu*T(:,j3);

end

if (delta * R(k-1,k-1)*2 > R(k,k)*2 + R(k-1,k)*2) % column change
R(:, [k-1 k])=R(:, [k k-1]);
T(:, [k-1 k])=T(:, [k k-1]);

Scalculate Givens rotation matrix such that element R(k,k-1) becomes zero
alpha = R(k-1,k-1) /sqrt (R(k-1:k,k-1) .'*R(k-1:k,k-1));
beta = R(k,k-1) /sqrt (R(k-1:k,k-1) .'*R(k-1:k,k-1));
theta = [alpha beta; -beta alpha];



===== PAGE 444 =====
R(k-1:k,k-1:m) =theta*R(k-1:k,k-1:m);
Q(:,k-1:k)=0(:,k-1:k) *theta.';
k=max([k-1 2] ) ;

else
k=k+1;

end

end

function [Q,R,P,p] = SQRD(H)
Sorted QR decomposition
Input parameter
H : complex channel matrix, nRxnT
Output parameters
Q : orthogonal matrix, nRxnT
P ; permutation matrix

HW WF 00 00 DP oP OP

p : ordering information
Nt=size(H,2); Nr=size(H,1)-Nt; R=zeros (Nt) ;
Q=H; p=1:Nt;
for 1=1:Nt normes(1)=0(:,1)'*O(:,1); end
for i=1:Nt
{mini,k_ i] =min(normes(i:Nt)); k_i=k_i+i-1;
R(t, la ka) eRe, [ka a1)?
plz, [i k_iJj=p(:, [ea 11);
normes(:, [1 k_i])=normes(:, [k_i i]);
Q(1:Nr+i-1, [i k_i])=Q(1:Nr+i-1, [k_i i]);
6 Wubben's algorithm: does not lead to

0

a true QR decomposition of the extended MMSE channel matrix

00 ol

Q(Nr+1:Nr+Nt,:) 1s not triangular but permuted triangular
R(i,i)=sqrt (normes (i) ) ;
Q(2,4)=0(2 4) /Ra 2) 3
for k=i+1:Nt
R(i,k)=Q (2,1) '#0(2,k) ;
O(¢,k)=0(s,k)-R(1,k) *@(2, 2) 3
normes (<) =normes (k) -R(i,k)*R(i,k)';
end
end
P=zeros (Nt); for i=1:Nt P(p(i),i)=1; end

im! 프로그램 11.5 Lattice reduction 사용한 MMSE 검출기법

no
+

447



===== PAGE 445 =====
PART Il )/1140와 MATLAB

—*— MMSE
—e— MMSE +LLL

10°
10%     a
0      10     20     30     40     50

SNR (dB)
그림 11.5 Lattice reduction 사용에 의한 성능 개선

CET mimo 시스템에서의 soft Output

앞 절에서는 다양한 경포 aes  decision) 기법들에 대해 알아보았다. 그러나,
soft—input soft— output ah HSS 통해 성능을 개선하기 위해서는 신호검출기의 출력
이 soft 0040바이어야 한다. 본 000 MIMO 시스템의 90 output 연산 방법에 대해
알아본다.

LLR 표현

Soft output? 조건부 확률의 비에 대해 자연로그 ns 취한 값으로서 신호의 확률적
인 값을 나타낸다. 이때 사용되는 ML 메트릭을 유도하기 위해서는 MIMO 시스템의 송
신부에서 임의의 신호 벡터 xs SARS 때 수신된 의 확률밀도함수(810를 유도해야
한다. 이 때, 위에서 가정한 MIMO 시스템의 환형 대칭 백색 Gaussian 잡음 특성을 이
용한다.

y=Hx+z                          (11.36)

식 (11.36)으로부터 다음 식을 유도한다.

448



===== PAGE 446 =====
제11장_ 공간 다중화 MIMO 시스템의 신호검출 기법

y—-Hx=z                          (11.37)

위의 AS 통해 수신된 AS yo 채널의 이득과 송신신호 xB 곱하여 M 결과는 잡음벡

터와 같고, 이를 통해 7-&의 분포가 잡음벡터의 분포와 같음을 알 수 있다. 여기서 잡음
벡터의 분포는 가정에 의해 다음과 같다.

72(2)=     exp(-F(2-w) a («-»)|           (11.38)

oy dens

여기서 는 해당 랜덤 변수 2의 Bit(mean ge 갖는 벡터를 나타내고 LE
covariance 행렬을 나타낸다. A* covariance 행렬의 determinant= 나타낸다. 평균 벡터
는 잡음의 평균값이 0임을 가정했으므로 0 벡터이다. 또한 Bee y, Ht 에 관해서 표
현할 수 있으므로, 위의 joint 『때는 다음과 같이 표현할 수 있다.

off

1
£(2)= 2710 ex -그       rly -   보지 은      (y|x)                 (11.39)

위의 전력밀도함수를 이용해 600 output 수식을 유도한다.
먼저 심볼 WHS] soft outputS 알아본다. 자연로그 안에 있는 분모와 분자의 7066600ㅁ
probability bayes’ theorem®] 의해서 다음과 같이 쓸 수 있다.

ol P(X, ae | p(y|x,)p(%)/ Ply) | =| P(y|x,) p(x)

p(x 13)      P(y|x.) P(X)! PLY)      etal)     (11.40)

여기서 각 심볼을 ASS 확률이 같다면 다음과 같이 표현할 수 있다.

. 끼지 15) |, | py|x,)
 [se an               aes

조건부 확률밀도함수에 위에서 유도한 확률

IN
번
42,
ne,
i
nol
4>
Je
+>
Im
ttlo
pal
ro,
ec)
(묘
a,
Dio
ay

my,
>

449


===== PAGE 447 =====
PART I MIMO2! MATLAB

1        2
exp| -     — Hx,

fs  re    |  20" Be |
로거                                      (11.42)

(x, ly)       a -  1          2

   20;
위의 수식을 전개하면, 아래 식과 같다.
In  P(x ly)  =  y —-Hx |’ -  ly — Hx, |?               (11.43)
p(x, 15) ) 20%       더 Oe"                      ：

자연로그의 특성에 의해 soft 04000의 Be 양수, 혹은 음수 값을 갖게 된다. 양의 값이
고, 그 크기가 클수록 ×,를 전송했을 확률이 x, 를 전송했을 확률보다 크다는 것을 의미
다.
비트 단위의 11# 은 max-—log approximation] 의해 다음과 같이 정의된다.

이

P(b,=lly)) 4
쏘기바. 20% oi. by — Hx - a nin, 16 -빠    (11.44)

심볼 Ｌ1에서와 유사하게 ?(%.,=1) 와 p(b,, =0) 의 확률이 같다면 다음과 같이 표

현할 수 있다.

!      2
>, plylx)      pa 건 lym |    (11.45)

xe S(i, /)”

xeS(ij          =In

1
> 2009     개 “1 2 lyf |

36966)                     xe S(i,j)

여기서 《,, 는 / 번째 송신 안테나에서 보낸 심볼의 / 번째 비트를 의미하고, 5./| 는 /
안테나에서 보낸 심볼의 7 번째 비트가 《같을 갖는 송신 벡터 집합을 의미한다.

시
지수함수의 특징을 이용한 max—log approximations 적용하면, 다음의 관계를 얻을 수



===== PAGE 448 =====
ex -3!     lly  nt |
‘=i       9607)          210
이을 i  |=  pet 1 te                 (11.46)
ply | “7 =0)          max €XDp| —  1           i
xeS(i,j)”      20°

Log: 단조증가하기 때문에 위의 AS 전개하면 최종적으로 다음과 같은 식을 a

in. ly ~ Hf               (11.47)

&,=1
of "|.    _ly — Hx? -

20°  xe S(i, j)              207 x

MIMO 시스템을 위한 최적 LLR 연산

먼저 ML 신호검출방법을 사용했을 때의 정확한 118 gol 대해 알아본다. 정확한 11
값을 구하기 위해서는 모든 송신 가능한 심볼 벡터에 대한 ML 메트릭 값이 사용되어야
한다. 정확한 LLR 값은 아래와 같이 표현할 수 있다[242].

L(b,; \y)=minD(x) - minP(x)                      (11.48)

여기서, D(x) = ly-Rx| 이고, (iz) 은 %,=ㅡ1에 해당하는 벡터들의 집합이고,
Hj) 은 0   족하는 벡터들의 집합이다. 식 (11.48)에서의 이고   현은
1006-108 근사화를 사용했기 때문이고, 후보벡터의 개수가 적기 때문이 아님을 강조한다.

성상도는 16-QAMES 가정하고, 3x3 MIMO 시스템을 가정할 때 nies |=
zd, fy |=C"/2 =1672이다. 이렇게 많은 횟수의 ML 메트릭을 연산해야 하므로, 정
능을 달성할 수 있으나, 실용적이지 못하다.

확한 LLR 연산을 동

= 최적 LLR 연산

할

앞 절에서 언급된 ML 기반의 간소화된 수신기법들, 즉 50, 0804-\41.10등을
경우에는 모든 송신 가능한 심볼 벡터에 해당하는 ML 메트릭 go] 가용하지 않기 때문에
아래와 같은 근사화된 LLR 값을 발생한다.

451 ㆍ



===== PAGE 449 =====
PART II MIMO2} MATLAB

L(®,, |y)= minD(x) - minD(x)                   (11.49)

여기서, 90, )) 은 준 최적 검출기법으로 얻은 후보벡터 집합 Bo] 속한 벡터들 중
& ; =-! 을 만족하는 벡터들의 집합을 의미하고, 9(,, /)' 은 %;=+을 만족하는 벡터집
합을 나타낸다. 식 (11.49)를 사용한 근사화된 LLR 값을 사용할 때는 아래의 2가지 문제
가 발생하게 된다[242].

문제점 1 : 후보 벡터 집합에 존재하지 않는 비트 glo] 있어 ML 메트릭 WS 구할 수 없
는 경우가 존재할 수 있다.
문제점 2 : 후보 벡터 집합 내에 비트 값이 모두 존재하지만 해당 ML 메트릭 같이 정확하

않는 경우가 있다.

mas

clr

위의 2가지 문제점을 좀 더 세부적으로 분석한다. 후보벡터 집합에 어떤 특정비트의 특

A 값일 경우가 없을 때, 즉 Sli, j = SEE Si, i)’ = 0 경우에는, 식 11.49) 우편
의 2개 항 중 1개 항에 해당하는 값을 구할 수 없어 해당 비트에 대한 LLR 값을 구할 수
없게 되고, 존재하지 않는 비트 값에 대한 ML 메트릭 값을 특정 값으로 대치해야 한다. 식
(11.49)의 우편 2개 항 중 적어도 한 개의 Be 항상 연산이 가능하다.

후보벡터 집합에 특정 비트의 값이 0과 1일 때에 해당하는 후보벡터들이 모두 포함되어

있어 LLR 값을 구할 수 있을 때 즉 Sli, j) 4 OD SG, 7) HOY 때에도 오류
가 발생하며, 그 오류를 다시 2가지 경우로 나누어 분석할 수 있다. 벡터 은 식
(11.48)을 만족하는 벡터이고, 후보벡터 집합 Bol 속한 벡터 BML 메트릭이 가장 작은
벡터는 54. 로 표시한다. 유사하게 Fhe ×,/ 에 해당하는 4) 2] 비트 값을 의미하
고 pmo Xoo 에 해당하는 “의 비트 값을 나타낸다. 먼저 후보벡터 집합에 ML
해가 존재하는 경우, 즉 Xm -4.8 이고, 따라서 “4 -“./.0.8 의 경우에는 LLR 값

이 아래와 같이 표현된다.

L(b,)|¥)~minP(x) ~ minP (x) =P (Xa) - minP(x) < 0          (11.50)
식 (11.51)에서 8,500 = 5.00.0 =~) 임을 가정으로 하였다. 식 (11.50) 우편의 2개 항 중 174

항의 값은 정확하지만 다른 항이 정확하지 않고, 정확하지 않는 항은 항상 양의 오류를 나타내게

된다. 후보벡터 집합에 \Ｌ해가 존재하지 않는 경우에는 LLR 값이 다음과 같이 표현된다.

452



===== PAGE 450 =====
(6, ly) ~minP (x) 될 min? (x) = D(Xjz,2 ) - minP (x) < 0          (11.51)

xeS(i,j)               xeS(i,j)*                                  xeS(i,j)"

식 01.51)에서도 8, age =—1 임을 가정으로 기술하였다. 위 식을 관찰하면 식 (11.51) 우편의
2개의 항이 모두 오류를 포함하고 있으며 두 항의 오류는 모두 양의 오류라는 것을 알 수 있다.
위의 문제점들을 종합하여 아래의 그림 11.6으로 eae 아래의 그림 11.6에서는 QPSK
변조방식, 3x3 MIMO 시스템, ML 해가 후보벡터에 포함되어 있지 않다는 것을 가정하였다.
그림 11.6에서 볼 수 있듯이 정확한 18 값과 비교할 때 준 최적 검출 기법에 의해 생

성된 후보벡터를 사용한 근사화된 118 값의 절대값은 항상 크거나 같다는 것을 확인 할
수 있다. 또한 존재하지 않는 비트 값에 대한 ML 메트릭을 정해야 한다.

min      ice      2                       2                                         min              2
=a  ll y- Hx ll     bore a  ll y— Hx ll                    ly—Hxyc ll?       ext)  ieee! = eal
eh. Ei 80601     none | 7- Hal?                         ly—Hxaz | ?        비네 eee?
min      13      2 min      ni      2                 min      은       2           =         2
202"  | y—Hx ll     xy"  ll y—Hx ll                 hah  ll y— Hx Il        ll y-Hxag ll
min      fs      2 min      be      i             min      a       2           0         2
ay  ll y— Hx ll     62  y= Hex Il    =            62  ll y- Hx ll        ll y-— Hx yy ||
bore lly—Hx Il?  hans lly—Hx Il?          ll y—Hx yy?      aa ll y—Hx Il?
min      a      2 min      iB      2                 min      Ee       2           ed         2
Sear  ll y— Hx ll     xex(@.a)t  ll y—Hx Il                  uaa  ll y— Hx Il        | y—Hxag ||
min      =      2 min      ng      2                 min      ~       2          3         2
Baa  ll y— Hx ll     iy  ll y— Hx ll                  as  ll y— Hx ll        ll y-— Hx yg ||
pias ll y—Hx I?  Laer lly—Hx I?   ae   y—Hx yall?    ae ll y—Hx ll?

]

igo Hew el  Jae by-He I?

정확한 LLR

Min |y—-Hxi? MN, | y—Hx Il?

xeS(1,1)                                              xeS(1,1)*

min. jj y—Hx i?          ?                       | 22 으으            ?

min qy-Hxi? Min. yy—yx?                min y-Hxl? 0 |ly-Hxgsll?
a                 ‘          Eee ya al? =                 ?            ly— Hew, ?

stor 1-태트 SUB. yaa          17-8961? MD y—ax il?

min qy-Hxi? Min, yy_yx 13                     min |, 8613 00 ly—HBxy,all?

2            min.  ll y— Hx |?                        ie               | y—Hxyap ll?
min 12700 Nh y— uit                 Wy—Hxy_ th? = PUD, 17-86 132

근사화된 LLR
그림 11.6 적은 수의 후보벡터를 사용한 니값 SR(QPSK 성상도와 3×3 MIMO 시스템 가정)

453 —



===== PAGE 451 =====
PART Il_ MIMO2} MATLAB

부록 ^

1Ｌ8해 *=10”8) '8"*를 사용하면, arg min|y -프죄 =argmin(x - %)" H7H(x- %) 임
Walch. 위 관계는 실수 시스템 및 허수 시스템 모두에 성립하므로 대신 뻐를,
신 "를, 대신 xB 사용한다.

]
ly - Hx{> =|y - Hx - Hk+ Hi
=(y —Hx — Hx + Hx)’ (y — Hx —- Hx + Hx)
= (y — Hx)’ +(H&— Hx)! Ky — Hx)+ (H% — Hx))                             (A.1)
= (y — Hi)’ (y — H&)+ (Hx — Hx)’ (Hx — Hx)
+(Hx- Hx)’ (y -Hx)+(y- Hi)’ (Hx - Hx)

“<1 ttlo
on      =   a

0

호이 LS 해이므로, (Hx-Hx)’ (y—Hx)=(y — Hx)’ (HX-Hx)=0° 2H 위 식은 아래
와 같이 표현된다.
ly - Hx\)° =(y — H%)" (y — Hx) + (Hx — Hx)’ (Hi - Hx)                            (A.2)
위 식에 LS 해를 대입하면 아래 식으로 표현된다.
ly -따 =(y-H (HTH) n'y) (y -H(H"H) | Hy) +(%-x)" H’H(i-x)        (A3)
등식 y-H(HH)'H’y=(1-H(H"H)' Jy one 4 (A3) 우편 첫 번째 항은 다음
과 같다.
y"({I-    80001 1800] [ㄷ  H(H7H)    1H”) y
=y (1-H      rH)"  |  H(H’H)'H    H" Jy                     Aw

H(H
=i ‘te H(H’H)' H” —H(H’H)"H’ +H(H’H)"HTH(H"H)'H” J y
-H(H

TH)  H’ ) y.

lI
*
=
변
=

ㆍ 3454



===== PAGE 452 =====
따라서, 식 (ㅅ.3)은 다음 식으로 표현된다.

ly -Hxf =y"(I-H(H’H)'H") y+(x-%) HH (x-3)             (AS)
식 (&.5)의 첫 번째 항은 벡터 xo] 대한 상수임을 알 수 있다. 따라서,

argmin|y -Hx{’ =aremin y" (1-H(H"H) |”) y +(x—%)H"H(x-3)     26
=argmin(x—%x)H’H(x-x)                              .

455


===== PAGE 453 =====
10장과 11장에서 ^7개의 송신 안테나와 Ne 개의 수신 안테나를 가진 MIMO 시스템에
서 통신의 신뢰성을 증가시키는 다이버시티 기법과 통신 용량을 증대시키기는 공간 다중
화 기법을 각각 다루었다. 그림 12.1과 같이 다이버시터 전송 기법은 송신단의 여러 안테
나가 동일 정보를 내포하는 ASS 전송하고 신호가 여러 경로의 독립적인 감새를 거쳐
수신단에 도착하면 수신단에서 적절히 조합하여 데이터 전송의 신뢰도를 높일 수 있다.
다이버시티 전송 기법은 다중 경로 감쇄 채널에 의한 성능 열화를 극복하나, 단일 안테나
의 경우에 비해 전송 속도의 증대를 얻기 어렵다. 반면에 공간 다중화 전송 기법은 여러
송신 안테나가 각각 독립적인 정보를 내포하는 신호를 전송한다. 결과적으로 다수개의

Y          eee BER                     SNR
-2
…              SNR
SNR®
(a)                   SNR          .
J
Capacity
cs
(b)           No. of antennas min(N,, Ne)

그림 12.1 (a) 안테나 다이버시티 이득과 (b) 공간다중화의 효과

456



===== PAGE 454 =====
제12장_다이버시티-다중화 Trade-off 시공간 부호화 기법

ㅇ

[모   (pace

SISO (Single—Input Single—Output) 채널을 형성하는 ATS 얻게 하여 A
일 안테나의 경우에 비해 증대시킨다[243]. 공간 다중화 AS 기법은 AS |
이지만 다이버시티 이득이 낮아 데이터 전송 신뢰도가 낮다. 이와 Zo
기법과 다중화 AS 기법은 각각 얻고자 하는 이득이 다르고, 신뢰도와 채널 용량을
시에 크게 하기가 어렵다.
그러므로 MIMO 시스템에서 높은 전송 AES 달성하고, 동시에 비트 오류 확률이 낮
은 전송 Blo] 대한 연구가 다양하게 진행되었다[244]-[248]1. 본 장에서는 여러 연구 내
시공간 블록 부호에서 full—diversity 10411-1816 기법과 주파수 효율성 및 신호의 높
뢰도를 동시에 고려한 선형 분산 부호 기법을 살펴본다.

“
HI om
ulus

off px ml Sh
ob» He

rlo ofp
rm ON

OMY Futl-piversity Full-Rate 시공간 블록 부호

000 시공간 성상 회전 부호

10장에서 다룬 Alamouti 기법은 두 개의 송신 안테나의 경우 최대 다이버시티 이득을
얻으면서 BSS 1을 만족한다[214]. Tarokhe 3개 이상의 송신 안테나의 경우에 높은 최
대 다이버시티를 얻고 수신단에서 ML 복호를 선형 연산으로 수행하는, 직교 부호 설계를
제안하였다[221]. Hurwitz—Radon 정리에 의해 복소 신호에 대하여 2개 송신 안테나 경우
를 제외한 최대 전송률과 최대 다이버시티를 달성하는 직교 부호는 존재하지 않음이 증명
되었다[221]. 3 또는 4 개의 송신 안테나에서 최대 다이버시티와 3/4 부호율을 갖는 여러
방식 들이 발견되었고, 또한 일부 성상도에 대해서는 2개 이상의 안테나에 대해서도
full—diversity full-raeS 갖는 복소 부호 설계가 가능함을 보였다[249]-[251]. GAST
(General Algebraic Space—Time) 부    —  Hadamard 418 precoderS 이용하여 형상을 회
전시키며 full—diversity full—rateS 달성하였다[245]. 더욱이 이 부호는 큰 성상도와 많은
개수의 AS 안테나를 사용하는 경우, 직교 부호에 비해 부호화 이득이 더 크다. 성상도
회전을 위한 26000@는 Xino] 의해 일반화되었다[246]. 그러나 %1의 precoder= 시공간
블록 부호에 상관없이 수신부에서 ML 송신 ASS 복호해야 하므로 2개 이상의 안테나에
서 full—diversity 1411-ㅁ866를 얻을 수 있으나 수신부의 복잡도가 증가한다는 단점이 있다.

본 절에서는 위와 같은 문제점을 해결하고자 제안된 시공간 성상 회전 부호 기법을 다

457



===== PAGE 455 =====
PART Ill MIMO2t MATLAB

룬다. 시공간 성상 회전 부호 기법은 시공간 블록 BS 기법에서 2개 이상의 안테나에서
& full—diversity 1011-1866를 갖게 한다. 송신단에서 성상 회전을 위해 precoding 과정을
거치게 된다. 송신단의 2ㅠ6000@는 시공간 성상 S|Al(space—time constellation— rotating)
을 통해 부호가 최적화 된다.

Modulator-—>|__S/P_ || Precoder +>») SRBC  {  Channel  :  >
"     : decoding

Vandormonde Diagonal matrix
matrix       (ST-CR)
Alamouti STBC
(A-ST-CR)

그림 12.2 Full-diversity full rate= 위한 송수신 블록도

그림 12.2는 시공간 성상 회전 부호 시스템을 나타낸다. 식 (12.1)은 ^, =4 의 경우 입
력 벡터 d=[d,,d,,---,dy, ] 의 복소수 회전 행렬 @ 에 의한 ^, 차 벡터 = yy, |
로의 변환과정을 나타낸다.

1a a@ @||4,          Fj
1 |1 4 a@ aid         r
r=@d =—_—    개   2| =|?               (12.1)
JN,|1 @ a @ || 4;         ie
1 8 % a |l\d,         "%

여기서, a, = exp(j2a(i+1/4)/N,), 1=0,1…,, -1이다. 심볼 는 unitary 행렬을
통해 ^, 개의 전송 안테나 중 일부를 이용하여 시간 7 에 전송된다. 예를 들어 식 (12.2)와
같은 unitary 행렬을 고려할 때 심볼 는 7 시간에 7 번째 안테나를 통해 전송된다.

, 0 0 0

x= 1% 9 2               (12.2)
007, 0
00 0,4

458



===== PAGE 456 =====
Precoder @ 는 아래 식 (12.3) 성질을 만족시키므로 임의의 전송 안테나 수 및 QAM
성상도에 대해 최대 다이버시티를 달성한다.

2/

Nr
=          ;       사고:
@0.., = arg max min | ][o, (d    d)                                     (12.3)

여기서 0[ 는 © 의 i Mal 열이고, VE BE 송신 가능한 데이터 행렬 0 의 집합이다.
이러한 precoder © 는 최대 다이버시티 뿐만 아니라 최대 부호화 이득을 달성한다는 것이
증명 되었다. 수신 신호는 식 (12.4)9} 같이 표현되고 각 시간에 수신된 ASE 모든 데이
터의 선형 결합으로 이루어져 있기 때문에 채널 정보를 수신단에서 알고 있다는 가정하에
A} (12.9)와 같이 모든 입력 데이터 조합의 BOS 고려하는 ML 복호만이 가능하다.

21   1 0 0 0114   nN,
0    0 0
= = 0      소오 ath ey         (12.4)
| 10 O  O} Th} Jn,
Va   0 0 0 114   ny
도          au       2
dj, =arg max >|», -67ah,|              (12.5)

dy ,d3 dy  i=l

그림 12.32 시공간 성상 회전 부호 기법의 성능이다. BASS Rayleigh 페이딩 A
널이며, 시공간 블록 부호 시간 동안에는 변하지 않는 준 정적 페이딩이고, 블록 상이의
변화는 독립적이라고 가정하고, QPSK BAS 사용하여 2610/660432로 ARS 전송하였다.
송신 안테나가 4개, 수신 안테나가 1개, 수신단에서 채널 상태를 완벽히 알고 있다는 가정
하에 모의실험을 수행하였다. 신호 검출은 ML 기법을 사용하였다. 그림 12.3은 SISO 성
능, 1x4 MRRC 성능, 시공간 성상 회전 부호 기법의 성능을 비교한다. 다이버시티
얻지 못하는 SISO 시스템의 성능에 비해 큰 성능 향% 이 있음을 확인 할 수 있다. a

시공간 성상 회전 부호 기법은 종신                          블록 부호 기법

Ir

ea)
au)
so
ane
ma!
i,
을
it

[무
00
—
ofp
st
=
ofl
> 」



===== PAGE 457 =====
PART 11 _ MIMO2} MATLAB

Performance (QPSK)

104

10°}

SER

104

10°

t] —@— SISO (Tx:1, Rx:1)
10° —#- STBC (Tx:4, Rx:1)
더 —-O— FDFR (Tx:4, Rx:1)
[| —+— MRC (Tx:1, Rx:4)

'                 {
1                 1                1                 1                 1                 1                                  1

10"

0 2 4 6 8 10 12 14 16 18 20
SNR [08]

그림 123 시공간 성상 회전 부호 기법, SISO, 시공간 SS 부호, MRC 기법의 성능 비교

% Full Diversity Full Rate - space-time constellation rotating
% FDFR_STCR.m
function FDFR_STCR()
SNR_step=2; SNR_Value=[0:SNR_step:20] ;
SER=zeros(1,length(SNR_Value)); sq2=sqrt (2);
QPSK table=[1+j, -1+j, 1-j, -1-j]/sq2;
N_block=1000000; N bit=2; nT=4;
raw bit_per frame=N_bit*nT;
Theta=[1 exp(j*2*pi/4/4) exp(j*4*pi/4/4)   exp (j*6*pi/4/4;
1 exp(j*2*pi*5/4/4) exp(j*4*pi*5/4/4)  exp(j*6*pit5/4/4) ;
1 exp(j*2*pit9/4/4) exp(j*4*pit9/4/4) exp (j*6*pi*9/4/4) ;
1 exp (j*2*pi*13/4/4) (exp (j*4*pi*13/4/4) exp(j*6*pi*13/4/4)];
for SNR=SNR_Value
rand('seed',1);   randn('seed',1);
SE=0; sigma=0.5/(10*(SNR/10)); sq_sigma=sqrt (sigma) ;
for block_index=1:N_block
cost=1000;
s=randint (1,raw_bit_per frame) ;

X=QPSK mapping (s,nT) ;



===== PAGE 458 =====
제12장_다이버시티-다중화 Trade—off 시공간 부

X_hat=[];      X_Estimateds [] ;
H=(randn(4,1)+}*randn(4,1))/sq2;
trans_data=Theta*transpose (X) ;
r_data=diag(trans_data) ;
y= r_data*H + sq_sigma* (randn(4,1)+j*randn(4,1));
for i=1:length(QPSK_ table)
for p=1:length(QPSK_table)
for k=1: length (QPSK_table)
for w=1:length(QPSK_table)
x1=QPSK_table(i); x2=QPSK table (p) ;
x3=QPSK_table(k) ; x4=QPSK_table(w) ;
temp=norm(y-diag(Theta* [xl; x2; x3; x4])*H); % (12.5)
if temp<cost
X hat=[xl; x2; x3; x4]; cost=temp;
end
end
end
end
end
for 1=1 1107
if X(i)~=X_hat(i), SE=SE+1; end
end
if SE>1000, break;   end
end
SER (SNR/SNR_step+1) =SE/ (nT*block_index) ;
if SER(SNR/SNR_step+1)<le-6, break; end
end «for SNR=SNR_start:SNR_step:SNR_en

ie) 프로그램 12.1 Rayleigh 페이딩 채널에서 FOFR 시공간 블록 부호 기법 실행 프로그램

% 029 mapping.m
function [qpsk] =QPSK_mapping(bitseq,Nfft) ;
QPSK table=[1l+j, -1+j, 1-j, -1-j]; sq2=sqrt(2);
for i=0: Nfft-1,
temp = bitseq(2*i+1)*2 +bitseq(2*i+2) ;
qpsk(i+1) =QPSK_table(temp+1) /sq2;
end

ia) 프로그램 12.2 QPSK 맵핑 함수

461



===== PAGE 459 =====
PART 1 MIMOS} MATLAB

GAP) Alamouti DES 이용한 시공간 성상 회전 부

성상 회전 부호 기법에서 각 시간에 수신된 ASE     데이터의 선형 결합으로 이루
어져 있기 때문에 모든 송신 가능한 데이터 조합의 BPS 고려하는 ML 복호가 매우 복
잡하다는 문제점이 있다. 이와 같은 문제점을 보완하기 위해 그림 12.49} Zo] precoderS}
Alamouti 블록을 결합한다. 이와 같은 결합을 통해 부호화 이득 또한 증가한다. 206000@7
에 의해 생성된 심볼 /, 는 Alamouti SSS 통해 식 (12.6)과 같은 시공간 블록 부호로 변

환되어 전송된다.

모

비빈

2 it

혁 >

_d | Precoder | T | Alamouti                          mc fd
이          Block                         decoding

그림 12.4 Alamouti 부호를 이용한 시공간 성상회전 부호 기법의 블록도

0
=                                                                                            12;

H
0    0   =r   B

Alamouti 시공간 성상 회전 (Alamouti space-time constellation—rotating) 부호의 부호

화 이득 증가는 앞서 살펴본 다이버시티 곱 비교를 통해 알 수 있다. 식 (12.7)은
Alamouti 시공간 성상 회전 부호의 a   곱과 OF 절에서 설명한 시공간 성상 회전
부호의 다이버시티 곱을 비교한 것이다.

(gore )     티브

여기서, 오는 서로 다른 두 송신 신호 BEV} precoder OF 통과한 후 생성된 두 A

볼의 차를 나타낸다. 206000@ © 가 주어졌을 때 Alamouti 시공간 성상 회전 부호의 다이

버시티 곱이 시공간 성상 회전 부호의 다이버시티 곱보다 크거나 같기 때문에 260006@에
Alamouti BSS 연접함으로써 부호화 이득이 더 증가됨을 알 수 있다.



===== PAGE 460 =====
제12장_다이버시티-다중화 113ㅎ306-ㅇ1! 시공

009 본부

본 절에서는 시공간 부호화 기법의 낮은 전송속도의 문제점을 해결하는
(Linear Dispersion Codes)S 다룬다. 4|£= Hassibi2} Hochwald7} 제안한 선형
SE AS 심볼에 의해 결정된 계수 값을 이용하여 분산 행렬의 선형 조합인 부
하는 기법이다. 선형 분산 부호 설계의 핵심은 기저 행렬이 MIMO 시스템의 68001
을 최대화 하는 부호를 선택하는 것이다. 그러나 ㅁ1369101와 Hochwald7} 제안한 A
HOE ergodic 용량에 최적화 되어 있어 오류 성능을 보장하지는 않 않는   Al
하기 위해 Heath?} Paulraj7} 프레임 이론에 기반한 선형 분산 부
서는 Hassibi2} Hochwald7} 제안한 방식과 26801 와 Paulraj7} ae) a3  브
대해 자세히 다룬다.

rx

x ofl

1 AL
10
~ dn
oo -ㅁ fot

(소

oy

a
na 혐
=
(으
x OF
fi
tr rhe tho 09
또 Ee
2 te

cm
fol
2

03/84 Hassibi2} Hochwald2] 기법

본 절에서는 Np AS] 송신 안테나와 ^, A] 수신 안테나를 가진 비선택적(830 페이
딩 시스템을 가정하고 다음 식 (12.8)과 같이 나타낸다.

y= Pix+2                              (12.8)
T

여기서, # 는 BA 수신 신호 벡터이고 *는 BA 송신 신호 벡터이다. WE 채널 행렬
이고 2 는 zero—mean, unit—variance, complex—Gaussian 잡음 CN (0,1) 이다. 채널 행렬
H 9} 송신 벡터 xt 시 ㅁ(0880") |=^,,와 £[Tr(xx")]=N, 의 특성을 지닌 단위 분산
의 윈소들을 갖는다. 만약 수신부에서 채널 정보를 정확하게 알고 있다고 가정한다면, 채

=
널 용량은 다음 식 (12.9)9} 같이 주어진다.

al

Ry>0,T1(Ryx)= Ny

C(p,N;,Ng)=_ _ max    ee det

——*
gas

ly, +7 -HR,H" ㅣ              (12.9)

여기서 채널 행렬 HE SHA CN(01) 성분을 가지고 있다면, 위 AS AGH 하

463



===== PAGE 461 =====
PART II_ MIMO2} MATLAB

는 covariance YAR, =], 이다. 그러므로 AY 용량을 다음 식 (12.10)과 같이 표현할

수 있다.

^,

C(p,N,,N,)=   e} toe ae,  ine 은 0 |           (12.10)
선형 분산 부호화는 다음 식 (12.11)과 같이 설계된다.

26062)                           (12.11)
q=l
여기서 a, a2, … 30는 복소수 스칼라이고 (;와 DE TxNr 크기의 복소수 행렬이다.
PSE 분산 Ba {(C, Dj 의해 결정되므로, 부호 설계는 7; Nr {C,, D,}o] 의해 A
정된다. {Cy Dj} ABS 위해서 송신 신호 (xp 3, }와 수신 신호 사이의 상관 정보를
이용한다.
Xq 신호의 분해를 통해 실수부와 허수부로 나누어 아래 식 (12.12)과 같이 표현할 수 있다.

x, =@,+ jB,,q=1,....0                     (12.12)

그러므로 xS 다음 4 (12.13)과 같이 다시 표현이 가능하다.

Q
x=)'(a,4, + jB,B,)                               (12.13)
여기서 Ag=C, + Dy, By=C, — Dg 이다. an, **, 020 AH Bi, -  … 6, 는 분산이 1.2이고
상관관계가 없다. 또한 sy, …, xo 단위 분산이고 상관관계가 없다. 신호 행렬 x 9] 설계
시 ABS E{Tr(SS")|=7N, 으로 제한하여야 한다. 또한 행렬 {4,, &,}의 식 (12.14)과
같이 정규화를 한다.

Q

> (1r(4"4  , + Tr( BiB, )) =2TN,                 (12.14)

q=l

_ 464



===== PAGE 462 =====
need 유사한 방식으로 할 수 있다. 행렬식으로 선형
를 다음 식 (12.15)와 같이 정의한다.

Q
y= |2xH+2= |P ¥\(a,4, +768, )H+z        (12.15)
N,     ^, q=l

식 (12.15)를 실수부, 허수부로 분해를 통해 다음 식 (12.16)과 같이 표현할 수 있다.

7

0
Y,t+ JY, =  수219  %(4.+/4.)+ IB, (Bag + jB,,) 08, +jH,)+z,+z, (12.16)
=

여기서 H, =Re(H) H, =Im(H) 이고, 식 (12.16)을 실수부와 허수부로 나누어 AS
아래 식 (12.17)과 같이 정리할 수 있다.

은이,                  4.8.)6+(-8..80.-78.0,) B, | +2,
=                                                             (12.17)
LS T(4..H                ApH, ) @, + (Bp gH, -B, ,H,)B, |+2,

여기서 YY >H,,.H 2..2, 열 벡터의 원소들은 7) =재아모 이루어
진다. 4,.8,./,, 값을 이용하여 아래 식 (12.18)을 정의한다.

i= AR ,  —Ar   3, = —B,,  T Brg   h = hen            (12.18)
"           4, 4         Arg      때            B Rq         —B, 4             "          h, n
여기서 Z=1,....Np 이고 Yeo y, 을 결합하여 4] (12.19)와 같이 정리한다.

Yau                 a        ZR
221                  ^        271
f= {Pam : fa]:                                   (12.19)
^,
28,                Q      경어
| Vine |             | Bo |    | 27. |

465



===== PAGE 463 =====
PART ㅁㅁ 11040 와 MATLAB

여기서 채널 행렬 HS 2, 7'×20 크기의 실수 행렬이고 AY (12.20)과 같이 정의된다.

더     Ah,    Bh,   때   464    Boh,
H=| :          :      ：         :           :                                 (12.20)
Ahy,  Bihy,,     Ag Ne  Bo ‘Nr

위에서 정의한 AS 이용하여 와 x] 입출력 관계를 다음과 같이 정리할 수 있다.

= |슨+                       (12.21)
y ae

A) (12.21) V-BALSTS} 유사한 형태의 입출력 관계를 가지게 되므로 기존의
V-BLASTO] 사용되는 다양한 신호검출 기법을 사용하여 신호를 복호할 수 있다.

eYyP4 Hearth} Paulraj2] 기법

본 절에서는 26800 와 Paulraj 기법이 제안한 선형 분^
수신한 심볼 벡터는 다음과 같다.

401=|은따지                          (12.22)

여기서, HE N,XN, 채널 행렬이고, N,xQ 의 코드 행렬에 의해 변조된 2 복소
수 데이터 심볼의 0×1 인 sS 고려한다. 2(4) 는 N, x12] ZMCSCG 잡음 벡터이다.
또한 T 구간 동안 /개의 코드 행렬이 있다고 가정하면, 7 시간 동안 수신 신호의 형태는
식 (12.23)과 같이 나타낼 수 있다.

y(1)        x(1)    z(1)
|  종전   : 64 :                      (12.23)
y(T)       " [x(T)} [2(7)

Hearth2} Paulraj7} 제안한 선형 분산 12S ©] spatial rate =(2/7'이다. 만약 0=7'라
 spatial rate= 아래 A} (12.24)와 같이 나타낼 수 있다.

}으
u

466



===== PAGE 464 =====
제12장_다이버시티-다중화 Trade—off 시공간

1
det (I, y, + (0748.06 98)

여기서 R=  > 6.,이,폭 이다. 다이버시티 차수는 아래 식 (12.25)와 같이 표현한다.

^, 00 Som, ef x                 (12.25)

i,j

다이버시티 차수는 모든 가능한 코드워드 오류|벡터 &,; of 대해 최소값으로 결정된다.
다이버시티 차수는 908081 signal 186의 에이 의존하며 N,N, 와 ^, 사이의 BS 가지
Al 된다. 이와 같이 Heath?} 『8411는 다이버시티 이득과 다중화 이득 사이의 08006-0
를 고려하여 Hassbish 다른 접근 방범으로 선형 부호 설계를 시도하였다.

그림 12.5는 Hearth?} Paulraj7} 제안한 선형 분산 부호 기법의 모의실험 결과이다. 모
의실험의 파라미터는 4, =4, N,=1,7=4,Q=4 이고 QPSK 변조 YAS 이용하였다.
그러므로 908081 ratio ㅅㅁㅋ=1이다. 이와 같은 환경에서 선형 변형 ABS 프로그램 12.3-2
의 Linear _transformation_matrix_1.mz} 같다. N, = 3, N, = 3, 7 = 3, 0 = 1 인 경우 spatial
ratio R=30|7, 선형 변형 행렬은 프로그램 12.3-3의 11068 ㅁ8091010180400 14801× 2.01
과 같다. 이와 같이 선형 분산 부호 기법은 cSt spatial ratios 지원할 수 있다. 선형

Performance (QPSK)

10°

10° -| —8— SISO (Tx:1, Rx:1)
[= —B— LOC (Tx:4, Rx:1)
=| —O— STBC (Tx:4, 6801

0 2 4 6 8 10 12 14 16 18 20
SNR [dB]
그림 12.5 Hearth2} Paulraj7} 제안한 선형 분산 부

|]
고
o£
Jo
0x
이

467



===== PAGE 465 =====
PART 4 MIMO2} MATLAB

분산 부호 기법의 성능은 SISO 성능에 비해 향상된 ASS 보이나 시공간 블록 부호 7
에 비해 성능이 열화 됨을 알 수 있다. 그러나 선형 분산 부호 기법은 508081 ratio7} +
Al 안테나의 수에 따라 1보다 큰 YOR 전송 가능하므로 공간다중화 기법과 같이 주파
효율성이 커지는 장점을 지닌다.

ad

ATLAB 프로그램 : 선형 분산 부호 기법

% Linear dispersion code - Heath proposed
% LDC _HEATH.m
function LDC_HEATH ()
SNR_step=2; SNR_Value=[0:2:20];
SER=zeros (1, length(SNR_Value)); sq2=sqrt (2) ;
QPSK table=[1+j, -1+j, 1-j, -1-j]/sq2;
N_block=1000000; N_bit=2;    nr=4>    nR=1;
raw_bit_per frame=N_bit*ntT;
codeword=linear_ transformation matrix;
for SNR=SNR_Value
rand('seed',1); randn('seed',1);
SE=0; sigma=0.5/(10*(SNR/10)); sq_sigma=sqrt (sigma) ;
for block_index=1:N_block
cost=1000;
s=randint (1,raw_bit_per frame) ; X=QPSK_mapping(s,nT) ;
H= (randn(nR,nT)+j*randn(nR,nT) ) /sq2;

H_trans=[H          zeros(1,4) zeros(1,4) zeros(1,4);
zeros(1,4) H           zeros(1,4) zeros(1,4);
zeros(1,4) zeros(1,4) H           zeros(1,4);

zeros(1,4) zeros(1,4) zeros(1,4) 4H];
y = H_trans*codeword*transpose(X) +...
sq_sigma* (randn(4,1)+j*randn(4,1));
for i=1:length(QPSK_ table)
for p=1:length(QPSK_table)
for k=1:length(QPSK_ table)
for w=1:length(QPSK_table)
x1=QPSK_ table(i) ;  X2=QPSK table (p) ;
x3=QPSK table(k); x4=QPSK table(w) ;
temp=norm(y-H_trans*codeword* [x1; x2; x3; x4]);
if temp<cost, X_hat=[xl; x2; x3; x4]; cost=temp; end
end
end

end
end

468

“ㅇㅇ 2


===== PAGE 466 =====
제12장_다이버시티-다중화 Trade-off 시공간 부호화 기법

for i=1:nT
if X(i)~=X_hat(i), SE=SE+1; end
end
if SE>1000, break; end
end sfor index_block=1:N_ block
SER (SNR/SNR_step+1) =SE/ (nT*block_index)
end % for SNR=SNR_start:SNR_step:SNR_end

—

fm) 프로그램 12.3 Rayleigh 페이딩 채널에서 선형 분산 부호 기법 실행 프로그램

% Linear_transformation_matrix_1.m

function [codeword] =Linear_transformation_matix_1()

codeword= ...

[-0.036-0.014i -0.1156-0.4268i -0.0583-0.1780i -0.0659-0.1163i;
0.0048+0.40321 0.0929+0.01531 -0.0975-0.1916i -0.0508+0.1726i;
-0.0246+0.00431 0.1657-0.1040i -0.1332+0.2814i -0.3343+0.0493i;
-0.0394-0.28941 0.0796+0.03131 -0.1593-0.2154i -0.0463+0.28819;
0.1847+0.00481 0.0880-0.07521 -0.0380-0.0685i -0.2601-0.3587i;
0.1370-0.13061 -0.1296+0.04971 -0.3499+0.2283i1 0.1243-0.0701i;
-0.3409-0.06371 -0.0824-0.30471 -0.0908-0.0130i1 0.0320-0.1437i;
0.1476-0.19491 -0.3386-0.05561 0.2237-0.1041i 0.0864-0.0646i;
-0.1233+0.11691 0.11434+0.1568i 0.2468-0.3387i1 -0.0693+0.0554i;
-0.1089-0.19821 0.2081-0.0851i -0.0235+0.0812i -0.2386+0.2902i;
0.0808-0.2558i 0.1048-0.2848i 0.1622-0.1432i 0.0890-0.1766i;
-0.1831-0.25401 0.0930+0.24701 -0.1391-0.0329i1 0.2460-0.0362i;
-0.3397-0.26481 -0.0574-0.0096i -0.0025+0.1820i -0.0800-0.14681i;
0.0196+0.00931 -0.3445-0.22951 -0.1465-0.0248i -0.1780+0.1563i;
-0.2037+0.12501 0.1368+0.0360i -0.1406-0.2795i 0.0511+0.2691i;
0.0082+0.08251 -0.0188+0.23441 -0.2826-0.1305i -0.2044-0.2216i] ;

Te 프로그램 12.4 선형 변형 행렬 함수 (%,=4,,=1.7=4, 0=4 )

% Linear_transformation_matrix_2.m

function [codeword] =Linear_transformation_matix_2()

codeword=[0.3003-0.1273i -0.2303-0.1625i   0.3651-0.11921;
0.1390+0.3748i1 -0.2530-0.0734i -0.2446-0.2106i;
0.2137+0.14671   0.3677+0.22201   0.12718-0.25851?
-0.0699-0.37761   0.2833-0.16161 -0.2783+0.0445i;
-0.2410+0.21471   0.1819+0.35601 -0.2324+0.1240i;
-0.2401-0.12731 -0.2303=0.16251   0.3651-0.11921] ;

Tm 프로그램 125 선형 변형 행렬 SI (N, =3, N, =3,7=3,0=1)

469



===== PAGE 467 =====
본 장에서는 송신단에서 채널정보를 활용하는 기법들을 살펴본다. 송신부에서의 채널정
보 가용 정도에는 채널 HS 완벽하게 아는 경우와 일시적인 채널의 부분적인 정보나 A
널에 대한 동계적인 정보가 가응한 경우로 구분된대: 세 경우 모두 수신단에서만 채널정보
를 활용한 기법들에 비해 채널 용량, 성능, 또는 복잡도 측면에서 SS 얻는다. 예를 들
어, 4개의 송신 안테나와 2개의 수신 안테나를 가진 시스템에서 -508 SNR 환경에서는
두 배의 채널 용량과 508 SNR 환경에서는 1.Sbps/Hz 만큼의 추가 이득을 얻을 수 있다
[252]. 그러나 송신단에서 채널정보를 얻기 위해서는 통신 자원의 낭비, 시간 지연등의 문
제점들이 있다. 특히, 채널이 AMA 경우, 일반적으로 송신부에서 완벽한 채널정보를 획득
하기 어렵기 때문에 실용적인 측면에서는 통계적인 채널정보 등 부분적인 채널정보를 송
신단에서 활용한다.

송신단에서 채널정보를 활용하는 YAS 매우 다양하나, 본 장에서는 대표적으로 자주
사용되는 precodings} 안테나 선택기법을 소개한다.

GREED ㅅ신부이서의 채널 추정

통신시스템에서 ASE 송신부에서 출발하여 채널을 통과하기 때문에 직접적인 방법으
로는 송신부에서 채널정보를 획득하기 어렵다. 따라서 간접적인 방법으로 채널정보를 획
득하게 된다. 그 방법은 두 가지로 구분되는데 첫 번째 YS reciprocityS 활용하는 방
범이고 두 번째 방법은 피드백 방법이다.

470



===== PAGE 468 =====
제13장_채널 정보를

아오 Reciprocity 방법

Transceiver                                                                       Transceiver

ㆍ | 0995 ㄴ- |

Reciprocity 방법은 안테나 &에서 BES] 전방향 채널(00080 channel)2] 채널정보
(Channel State Information; CSI)7} 8에서 ㅅ로의 역방향 채널(0646796 channel)°] 정보와
같을 때 사용할 수 있는 방법이다. 이러한 조건이 만족하기 위해서는 같은 주파수 특성,
같은 시간 특성, 같은 안테나 특성이라는 요구사항이 존재한다. Reciprocity 방법은 이상
_ 그림 13.13} 같이 full-duplex 시스템에서 송신단(^&)은 역방향 AWB to ㅅ)로부
터 전방향 채널(& to 8)의 채널정보를 획득할 수 있다. 그러나 AA] full-duplex 시스템
에서 주파수, 시간, 안테나 특성이 모두 정확히 같을 수는 없고, 따라서 두 채널간의 시간
지연차(스,)가 coherence 시간(72)보다 작고 주파수 옵셋(스,)이 coherence 대역폭(22)보
다 작으며 안테나간의 위치차(스』)가 000600006 거리(/2.)보다 작을 때 근사한 방법으로
reciprocity 방법을 사용할 수 있다.

A, <<T, , A, << B,, A, <<D,                    (13.1)

TDD 시스템에서는 전방향 채널과 a =  채널간의 회기 지연이 있을 수 있지만
coherence 시간에 비해 매우 작다면 전방향 채널과 역방향 채널의 주파수 특성과 안테나
특성이 °F reciprocity 방법이 가능하다. sah FDD 시스템에서는 시간이나 안테나 특
성이 같을지라도 사용하는 주파수 대역이 상이해 두 채널간의 주파수 특성 차이가 크고
이 차이는 604606006 대역폭 보다 일반적으로 크기 때문에, 810 방법에서는 76010700165
방법이 적합하지 않다

채널추정은 기저대역에서 이루어지지만 실제 ASS 통과대역의 채널을 말한다. 이러
통과대역의 WAS 장비의 특성까지 포함하기 때문에 전방향 채널과 역방향 채널 특
성이 같기 위해서는 송신단과 수신단의 \단의 특성이 동일해야 한다. 그러나 이러한 RF
하드웨어들은 다른 주파수 특성을 가지고 있기 때문에 이것을 보상하기 위한 보정 작업이
추가적으로 필요하게 된다.

1"  rh



===== PAGE 469 =====
PART II MIMOS} MATLAB

Transceiver                                                                       Transceiver
A                                                                                       B

Feed back
그림 13.2 피드백 방식의 블록도

법은 그림 13.2와 같이 수신단08)이 얻
(&)으로 전송하는 방법이다. 이러한 피드백 '    4} © reciprocity 방법과는 달리 RFU} 보
Al 등이 필요 없지만, 피드백 지연시간이 AY] coherence 시간 보다 작아야

있다.

A, <<T,                             (13.2)

피드백 방법은 700, DD 방법 모두에 적용이 가능하지만 피드백 정보를 전송할 때

추가적인 통신자원이 요구된다. 최근 이러한 오버헤드를 줄이기 위해 많은 연구가 진행되
고 있다.

피드백 기법 사용시 고려할 사항들은 아래와 같다.
1. 피드백 정보는 시스템에 오버헤드로 작용한다.
2
3

. 피드백 정보는 채널의 탭 수, 안테나의 개수 및 사용자 수에 비례해서 증가한다.
. 시변 무선채널의 경우는 채널 상태가 계속 변하기 때문에 빈번한 피드백이 요구된다.

위 ARMS] 교려되어 피드백 awe 성능 aay} Wasi 않는 범위 Hela ae
압축되어 전송된다. 압축 방법으로는 크게 직접적 양자화 방법과 간접적 양자화 방법이
있다.

직접적인 채널의 양자화는 코
원소들로 HS 맵핑시킨다. 맵핑은 <
평균제곱오차498)가 가장 작은
소로 하는 0080를 선택한다. 그러

0006000[0이라고 불리는 양자화된 벡터들의 집합의
자화가 되지 않은 원 채널 Ht 양자화된 채널의
선택하는 역할을 한다. 즉, 4|8-0080)| } 을 최

직접적인 채널 양자화는 간접적인 양자화에 비해

eh

472


===== PAGE 470 =====
신 기법

제13장_채널 정보를 활용

[에
ob

fo}
려하지만 적응적 방법을 이용한 간접적인 방법은 성능이득을 목
"

Ww-/(H),       F={W,,W,,W;,---,5W,} L=2"               (13.3)

방법에 대해서는 13.2.2절과 13.2.3절에서 설명한다.

을 생성하는 빙

 0 precoding 기법          |

활용할 경우의 채널 By

= ©

송신 안테나가 Nr MOLL, 수신 안테나가 ^&《개이고, 송신단에서 precoding 수행하면,

이러한 시스템의 블록도는 그림 13.3과 같다.

Noise

x                   Pre-coding                 s           Channel                - :  ;         y  !

~”
(w)                               _ (A)

그림 13.3 Precoding ==

[선
+
of
Ps
08
mia
xy
도
Jo;

벡터 x(V; x1) = precoding 행렬 W(N, xN,) 과 곱해진
음과 같이 표현된다.

no

메시지

비선택적 페이딩이라면 송신신호과 수신신호의 관계는 다

E
y =,/"HWx+z                            (13.4)
Nr

473



===== PAGE 471 =====
PART 4 MIMOSt MATLAB

= |Hs+2                            (13.5)
Nr

E[xx"]=1, 이므로, 송신 419] covariance 행렬은 R, = WW" 로 표현된다. 이 때
precoding 행렬 WE 송신전력 제한조건을 만족하도록 설계해야 하므로, 전체 송신전력
이 Nr 제한된다면, 다음 수식을 만족해야 한다.

wi, =T(R,,) =N,                                            (13.6)

송신단에서 가용한 채널정보가 완벽하다면 2『6000108이 사용된 MIMO 채널 용량은 다

음과 같다.
Es         04
C = max log, det(I1,, + -ㅡ~ HR,, HH” ) 2297 Hz                    (13.7)
Rss             NrNo
R,, = WW" 이기 때문에 채널 용량은 \ 의 함수가 된다. 채널 용량을 최대화 하는 행
렬을 Rs} 하고, °]S eigen decompositions} 식 (13.8)과 같이 표현된다.
그.                                                     (13.8)
따라서 precoding 행렬은 다음과 같다.
토트 에 = 0 Noo                                        (13.9)

전체 전력 제한이 4] (13.6)과 같다면 채널 용량의 최대화를 $e covariance 행렬은 앞
장에서 설명했던 water—pouring 기법으로 구할 수 있다.

RY =VRZ'V"                               (13.10)

Ro =diag (7, 10” Fo" ss}                       (13.11)
opt           1   +

7;   = a                               (13.12)

i

474



===== PAGE 472 =====
제13장_채널 정보를 활용한

ob

신 기법

[aes

H=Uzv"”    X= diag(o; )               (13.13)

따라서, \ = 표 "로 정의 되고, 양변에 "를 곱하면 식 (13.4)는 아래와 같

이 표현된다.
~  Es ~ aid
7 lm S+zZ             (13.14)

여기서, 2=U"2, §=(R2)'?x 이다.

(2) 부분적인 채널정보

통계적인 채널 정보만 알고 있는 경우의 채널 용량을 살펴본다. 송신단 안테나들의 상
관관계 행렬 R,& 정확하게 알고 수신단의 안테나들이 서로 충분하게 분리되어 있어,
R, =Ｌ을 가정하면, ABBAS 다음과 같이 나타낼 수 있다.

H=H,R;”                            (13.15)

송신단은 채널의 통계적 정보만 이용가능 하므로 채널 용량 역시 통계적인 측면에서 이
득을 얻을 수 있다. 채널 용량을 최대화 하는 데 있어서 앞장에서 설명한 outage 채널 용
량과 ergodic 채널 용량 관점에서 최적화 할 수 있다.

전체 송신 전력이 |\|.=/^, 로 제한이 되어있는 경우, ergodic 채널 용량은 2
(13.16)과 같다.
E

oe 00040 |          (13.16)
TLYO

C= max e| log, te ty,  +

이 때 [253]의 결과를 이용하면 최대 80080 AY 용량은 \“' =Qz Ay 일 때 얻을

다. 0ㅠ은 벼 고유벡터로 이루어진 행렬이고 (R, =0ㅠ,^ㅅㅠ,0《, ), AME 전체 전
력할당 대각행렬이다. 이러한 ae RK, 2] 고유벡터 방향으로 물리적
하는 것을  [을 의 |한다. 또한 전력할당 방법으로 [254]에서와 Zo] ergodic 채널 용
대로 하기 위한 통계적 \866-ㅁ04008 방법을 사용한다. 통계적 water—pouring

+>
xe

=

tuo
ro
bn
에

ilo

of lo st
Hu =

py of Oe
ea

475



===== PAGE 473 =====
PART If _MIMO2} MATLAB

에서는 water—pouringS H 의 고유치에 대해 수행하는 대신 R, 의 고유치에 대해 수

GE] Pre-coded STBC 기법

STBC(Space-time block 000108)는 다중 안테나 시스템의 채널 페이딩
활용하는 기법이다. 이러한 STBCE 송신단에서 채널정보를 활용할 경우
을 얻을 수 있다.

Precoded STBC¥ space-time 코드워드(0006\010)를 (라고 할 때 precoding 행렬
를 곱해서 송신한다. 이 때 We 코드북(<={\.\.,\,,…,\,}) 에 존재하는 행렬

하나이다. 입출력 WAS 다음과 같다.

3 고지
성공적으

가적인 이

ru

   i
110

oN <

[E
y=  oo  C=[e,c, ¢,---¢,], e=[c, c, c,---¢,,]., M<N,     (13.17)

수신단에서 precoding 행렬 \ 를 정하기 위해 SER(symbol error rate)°] upper bound
중 식 (13.18)을 사용한다.

Pr(ERROR | H) < exp(—y HW}. )                                  (13.18)

A] (13.18)에서 는 SNRI 사용되는 성상도와 관계되는 변수이기 때문에 \ 와 관계
없고, 따라서 SER upper 60000를 줄이기 위해서는 [HWS 최대화 시켜야 한다.
[255][256] 따라서, precoding BAS 다음과 같이 선택된다.

AW                                    (13.19)

W =arg max
WeF

그러나 식 (13.19)를 만족하는 Wo 는 여러 개가 존재한다. 그 이유는 임의의 unitary
= [BW,

2
fe}   A>
다. = Use

행렬 LS Frobenius norm 값을 변화시키지 않으므로 |8\,,
고, W,,L 또한 4|A42] precoding 행렬이 되기 때문이다. 여러 개의 \,,, 중 각 채널 상
황에 맞도록 정형화하기 위해 H 의 SVD(Singular Value 106000100851100)를 H = UV”

opt



===== PAGE 474 =====
제13장_채널 정보를 활용한 송신 기법

와 같이 정의한다. 이 때, UE NrxXNr Ql unitary 행렬, V 는 NeXNe 인 unitary YAO]
고 LE A{H} 를 원소로 갖는 Nex Nr 2] 대각행렬을 의미한다. 를 의 A 번째 열
부터 4 까지의 SS 포함하는 행렬이라 QS 때 정형화된 W,,, = 식 (13.20)과 같다
[2571.

Woe =V                                                 (13.20)
Al (13.20)은 가 unitary 행렬이므로 1<7ㄴ/4 을 테러 는 io] 대해 4{1\.}가 1
임을 뜻한다. 이것은 최적의 226000108이 수행 되었을 경우 Zt effective Ao] 대해 최대
의 전력전송을 의미한다. 따라서 전력 제한조건이  el  상황에서 |8\/|, 을 최대화 하

은 \8166-ㅁ004008과 유사하다.

다양한 채널환경에 대해 좋은 코드북을 설계하기 위해 오차를 다음과 같이 정의하고 양
자화한다[2571.

E {min (HW.   |. -18찌[: }                            (13.21)

위의 수식의 이해를 위해, upper boundS 다음과 같이 나타낼 수 있다.

터민이 [WE] se (2 an}e {min} wwf | 0322)

A? {H} 은 채널의 90841& 18106들과 관련된 변수이므로 사용자가 변경할 수 없고, 따
라서 좋은 SMe 설계하기 위해서는 로 {ming VO" ww", | 항이 최소가 되도록
해야 한다.

N, XM 로 이루어진 unitary 행렬들의 집합을 u(N,,M)e} 할 때, HERS 설계하기
위해 u(Nr,M) 2) 몇 가지 특성을 정의한다. 4(/(7 ,44) 는 0ㅠ786801800180ㅁ subspace
packing 에 관한 문현들에 정의가 되어있다[258][259]. 0(//,,24)에 속하는 행렬들은 각
각 74 -차원의 부분공간으로 이루어져 있으며, 각 부분공간들은 ^, -차원 벡터공간

(0”)으로 이루어져 있다. 여기서 CL #,차원의 복소 벡터공간을 의미한다.



===== PAGE 475 =====
PART II]_MIMO2} MATLAB

Grassmannian packing®] 정의에 따라 u(N,,M) 의                 Grassmann
manifold packing #2271 g(N,,M) ol] 속한다. 예                44)일 때
각각 정의하면 Pu» Pv, 들은 8(^%,,44)에 속한다.

부분공간의 상대거리는 성능과 연관된다. 이 거리를

속한 부분

이 정의된다.

드  고기드ㅇ
= 열 공간늘은 복소

5 065

=
를 들면, \1, weu(NV.

이들의 열 Bz Py,» Py, 라고
Grassmann 1082011010에

chordal distancez} 하고 다음과 같
(13.23)

d(W,,W,)= 그 W;" — W,W;'|

최소의 chordal distance: 6 =  ymin n d(W, W,) 로 표현된다.
북의 성능을 나타내는 A (13.22)는 다음과 같이

Metric ball approachS 이용하면 보드

근사화된다[257].
5  2N;M+o(N;) ㅣ
E {A {HIE {wind [것 - ww" | 비드     [56 - |  (13.24)

57} 증가함에 따라 감소한다. 그러므로 를
최대화 시킴으로써 최고의 코드북            수 있다. 6 를 최대화 시킨다는 것은 그림
13.4에 나타난 바와 같이 EM 내에 존재하는 행렬들이 다양한 Ave) 성공적으로 동작
하도록 넓은 범위의 벡터공간을

위의 60400는 2N,M + o(N, 를:

Fe

최소거리

Channel

Fy

그림 13.4 precoding #47} chordal distance

| _ 478



===== PAGE 476 =====
제13장_채널 정보를

그러나 실제적으로 Grassmannian 20800018으로부터 임의의 송신 안테나 개수 ^7, 코드
북의 길이 74, 코드북의 크기 Lo] 대하여 좋은 코드북을 설계하기는 매우 어렵다
[258][260]. 따라서, 이러한 packingS 설계하는 방법 중 자주 사용되는 방법은 [261]에서
제안된 DFT 행렬을 이용하는 방법이다. 즉, 수식 (13.25)와 같이 코드북을 설계한다.

F={Woep 8 Woep 1 307 Woes}                                       (13.25)

가장 첫 번째 SEMEL Wor S 설계하기 앞서, N,xN; 의 DFT 행렬을 설계한다.

1 [행렬의 (k,/) 번째 원소는 /,ㅠㅇ            fe, 이두어져 있으며, 코드워드의 길이만
큼의 열벡터를 선택함으로써 \,,를 생성한다. 이 때, 선택된 열벡터의 인덱스를
c=[¢,,+-Cy ]로 정의한다. 0 = diag([ 6070 20000 ] 이며 1m, 는
OSu,.y, = ㅅ-1 을 만족하는 임의의 상수이다.

Won, 로 이루어진 벡터를 ㅁ=[,,%.'…‥:',,]로 Alt 때, ut 최소의 chordal
distance 갖도록 A] (13.26)을 이용해 구한다.

272006-00- 005 느

u=argmax min (Worr 8! Woerr)                         (13.26)

{uy usu, }   Isis

이러한 AAS WSsh= precoding 행렬을 찾기 위해서는 Lv AS] OS 필요로 하기
은 연산량이 요구된다. 따라서 적은 송신 안테나 수와 낮은 피드백 전송속도를
요구하는 경우에는 이러한 전체적 FAY (full-search)o] 가능하지만 실제적으로는 랜덤한
탐색(0000000 568700)을 통해 u=[m,u,---u,, ]를 찾아낸다.
IEEE 802.166에 기고된 송ㆍ수신 안테나와 코도북 크기에 따른 4=[,4,…'0,, ] 값들
은 표 13.1과 같다.



===== PAGE 477 =====
PART IL MIMO2} MATLAB

#131 코드북 설계를 위한 파라미터

8/(9)              [1]          0

2                     1

3                      1                   32/(5)                   [1]                 (1,26, 28]
4                      2                   32/(5)                  19]                (1,26, 28]
4                     1                  64/(6)                  (1]               (1,8, 61,45]
4                      2                   64/(6)                  [0,1]              (1,7, 52,56]
4                     3                  64/(6)               (0,2, 3]            (1,8, 61,45]

function [code_book] =codebook_gen

* N_Nt: number of Tx antennas

% NM: codeword length

% N_L : codebook size

N_Nt=4; N M=2; N L=64;

cloumn_index=[1 2]; rotation_vector=[1 7 52 56];
kk=0:N_Nt-1; 11=0:N_Nt-1;

w = exp(j*2*pi/N_Nt*kk.'*11) /sqrt (N_Nt) ;

w_1 = w(:,cloumn_index([1 2]));

theta = diag(exp(j*2*pi/N_L*rotation_vector)) ;

code_book(:,:,1) = w_l ;
for i=1:N_L-1
code_book(:,:,i+1) = theta*code_book(:,:,1);
end
Ta 프로그램 131 코드북 생성 함수

% Alamouti_2x1_precoding.m

clear all; clc;

$%%%%% Parameter Setting 6%%%%%%5%%

N_packet=100; N_ frame=1000;

mod_order=2; M= 2“mod_order;
mod_obj=modem.qammod('M',M, 'SymbolOrder', 'Gray','InputType','bit');
demod_obj = modem.qamdemod (mod_ob}) ;

% MIMO Parameter

T TX=4; 0006 _length=64; NTX=2; NRX=1; sq2=sqrt (2) ;
n_bits=NTX*mod_order*N frame; t_bits=n_bits*N_packet;
code_book = codebook_gen;

480



===== PAGE 478 =====
제13장_채널 정보를 활용한 송신 기법

fprintt !ㅠ= = = = 00000 두 00200” ) ;
fprintf(' Precoding transmission') ;                            |
fprintf ('\n %d x $d MIMO\n %d QAM', NTX,NRX,M);
fprintf('\n Simulation bits : «d', t_bits);
fprintf (
SNR_0=0; SNR _step=2; SNR_ f=10; SNRS=SNR_0:SNR_step: ae tr
for i_SNR=1:length (SNRs)
SNR = SNRs (i_ SNR) ; ;  e bits=0;
noise var = NTX*0.5*10*(-SNR/10); sigma = sqrt (noise. var) ;
rand('seed',1); randn('seed',1);               |
for p_index=1:N packet
육융융육응응응응응융융웅 Transmitter 응응응융응융응융융융융융응응응응응응
x = randint (n_bits,1); %* bit generation
8 = modulate(mod_obj, x);
Scale = modnorm(s, 'avpow',1); % rai apenas
Se 배구 하바 가    % transmit symbol
= [S(1,1,:) -conj (S(2,1,        2,1.) Gon) (S$ (1.4.2) ));
$%%%%%S%S%S%S%S%S%% Channel and Noise 23%
H = (randn(NRX,T_ TX) +j*randn (NRX,T_TX))/sq2;
for i=1:code_length

oP

Q

2
9

cal(i) = norm(H*code_book(:,:,i),'fro');
end
[val, Index] = max(cal); He = H*code_book(:,:,Index) ;

norm_H2 = norm(He)*2; % H selected and its norm2
for i=1:N_ frame
RX(:,:,i) = He*Tx symbol(:,:,1) + ..
sigma* (randn (NRX, 2) +j*randn (NRX, 2) ) ;

end
SESS SSSSSSSSS RECELVED 응융융응융응융융융융융융움융응융융육
for 1=1:;죄 72206
8 hat(1,i) = (He(1)'*RX(:,1,1)+He(2)*RX(:,2,1)') /norm_H2;
s hat (2,i) = (He(2)'*RX(:,1,i)-He(1)*RX(:,2,1)') /norm_H2;
end

8 hat = reshape(s_hat/Scale,NTX*N_frame,1) ;
x hat = demodulate (demod_obj,S_hat) ;
e bits = e bits + sum(x_hat~=x) ;
end
ber = e bits/t_bits; BER(i_SNR) = ber;
fprintf ('\tsd\t\t\t%1.4f£\n',SNR,ber) ;
end
semilogy (SNRs,BER,'-k*', 'LineWidth',2);hold on;grid on;
legend ('Precoded Alamouti') ;xlabel ('SNR |(dB)'),ylabel('BER') ;

를 프로그램 13.2 Alamouti Precoding 전송 프로그램

481



===== PAGE 479 =====
PART Ill_MIMO2} MATLAB

34—4— Alamouti 2x1
+|—8— Precoded Alamouti |]

ee ee a ee _

Fe ee

SNR (dB)
그림 13.5 Rayleigh 페이딩 채널에서 precoding 기법의 BER AS

그림 13.5는 비선택적(080 Rayleigh 페이딩 채널이고 송신 안테나 2개, 수신 안테나 1
개의 환경에서 Alamouti 부호 성능과 표 13.12] precoding 기법의 성능을 비교한다. 이
그림에서 볼 수 있듯이 26000108 사용시 성능 이득을 얻는다.

Kye Pre-coded 공간 다중화 시스템

본 절에서는 26000108을 이용한 공간 다중화 시스템에 대해 살프
스템에서도 목적함수를 최대로 하는 코드북 내의 한 행렬을 선택한다.

(1) SVD 기반 전송 기법
송신 안테나와 수신 안테나수가 Np = N, ola, 채널 H=ULV" S 가정한다. 그림
13.6과 같이 송신신호 x= \행렬과 곱한

+
ofp
ee
그
[리
+»
ea
ea
fol
rir
aay

lo
as
ny
을

비
[에
aul)
muy

그림 13.6 SVD 기반 MIMO 전송 시스템

482



===== PAGE 480 =====
(13.27)

될 때, 잡음 전력은 Efz'2"} =o diag(/A?,---,1/Ay, ) 이
다. S, N, 개의 부채널은 각각 고유치 만큼 잡음이 증폭된 of /4,, 인 잡음 AAS 갖는다.
SVD7| B& 송수신단에서 직교(00100ㅁ00081) 행렬인 U, VS 곱하기 때문에 precoding
행렬로 인한 송신전력     가시키거나 SAS 변경하지 않는다. 따라서 SVD 기법은 여러
채널들을 병렬로 분리시키는 기법이다[216]. 또한 SVD 기법은 각 부채널에 대해 전력할당
을 하지 않을 경우에는 높은 SNR 영역에서 ZF(zero—forcing) 등화기와 동일한 Bes
인다262]. ZF 등화기의 경우 잡음 증폭양은 다음과 같다.

M
N
구
23
feb)
09
내
~S
=~
~
rl
ox,
4°,

illo
olN

Tr(H'H™“”)=Tr(V>'U'UDY’ V’)
= 그 2)

호그

“거고

(13.28)

이것은 SVD2] 경우와 다르고, 낮은 580#영역에서는 SVDS} ZF 등화기가 성능차이를
보이게 된다.

그림 13.7은 수신단에서 ZF 등화기를 사용한 경우와 송신단에서 9\1기반 송신기법의
BER 성능곡선으로서 다음 MATLAB 27144 13.3(“transmission model SVD_based.m’’)
을 chilli 얻어진 것이다. 이로부터 높은 SNR 영역에서는 두 기법의 BER 성능이 동
하지만 낮은 SNR BSAA 9\1기반의 송신기법의 Boo] 더 우수하다는 AS =

있다.

4h oe



===== PAGE 481 =====
PART IIl_ MIMO} MATLAB

BE 00006 위 Rayleigh Channel(QPSK)

: = Linear-ZF |}
“[=* v0

BER

10각-

0         2         4         6         8

* transmission model SVD based.m
clear all, clc;

N_frame=100; N_packet=1000;

mod_order=2; M=2“mod_order;

mod_obj=modem.qammod('M',M, 'SymbolOrder', 'Gray','InputType','bit');
06000 0107 = modem. qamdemod (mod_obj) ;

NTX=4; NRX=4; sq2=sqrt (2);

n la = N_frame*NTX*mod_order; t_bits = n bits*N_packet;

(
Eprint£(' SVD_based transmission') ;
fprintf('\n %d x $d MIMO\n %d QAM', NTX,NRX,M);
fprintf£('\n Simulation bits : %d', t_bits);
fprinté ('
SNR_0=0; SNR_step=2; SNR_f=20; SNRs=SNR_0:SNR_step:SNR_f;
for i_SNR=1:length (SNRs)
SNR = SNRs(i_ SNR); e bits = 0;
rand('seed',1); randn('seed',1);
noise_var = NTX*0.5*10*(-SNR/10); sigma = sqrt (noise var) ;



===== PAGE 482 =====
융융응육옹응응융융응융융응 TYANSMItter 응융응융응응응옹융응응응웅응융융응응

for p_index=1:N_ packet
Input_bit = randint(n_bits,1); % bit generation
symbol = modulate(mod_obj,Input_bit).';
Scale = modnorm(symbol, 'avpow',1); % normalization
Symbol nomalized = reshape (Scale*symbol,NTX,N frame) ;
H = (randn (NRX, NTX) +j*randn (NRX, NTX) ) /sq2;
[U,S,V] = svd(H);
Tx_signal = V*Symbol nomalized;

6%%% Channel and Noise %%%%%%%%%%%

(      (

randn (NRX,N_ frame) ) ;

육응융융융응응융융응융융융융 RECEIVED 응융응융융응융융융융응융융응융융융응응응응
symbol hat = inv(S)*U'*Rx signal; % “| (13.27)
Symbol hat = reshape (symbol _hat/Scale,NTX*N frame, 1) ;

Out_bit = demodulate(demod_obj,Symbol_ hat) ;
6 bits = e bits + sum(Input_bit~=Out_bit) ;
if mod(p_index, 1000) ==0
fprintf£('packet : td passed\n',p index) ;
end
end
ber=e bits/t_bits; BER(i_SNR) =ber;
fprintf ('\t%d\t\t\t%1.4£\n',SNR,ber) ;
end
semilogy (SNRs, BER, '-k*', 'LineWidth',2);hold on;grid on;
legend('SVD-based transmission') ;xlabel('SNR (dB)'),ylabel('BER') ;

ml 프로그램 13.3 SVD 기반의 전송 프로그램

(2) 선형 AMIS S}(pre—equalization)

수신단에서 뿐만 아니라 송신단에서도 사전등화(066-60481128000)를 수행할 수 있다.
여기서 AVS She precodingy} 동일한 의미이며 Ve precoding?! 경우에 한해서 일반적
으로. 사전등와라그 쓴다.

먼저 ZF 사전등화에 대해 기술한다. 송신신호 s

clr

다음과 같다.

s= Wx                                   (13.29)



===== PAGE 483 =====
PART 141 MIMO2} MATLAB

i
2     B

— Ww   H     >

그림 13.8 선형 사전등화

이 때, ZF 사전등화 행렬 \ 는 다음과 같다.

N
= BH"           pz   소수:                       (13.30)

~    1a] 전력제한이 N, 일 때 사전등화를 통한 전체 송신전력에 변함이 없도록 하기
ve 이는 수신단에서 다시 AGC(automatic gain 000001)에 의해 /값으로 나

수신신호의 메시지 신호 를 복원할 수 있다. 수신신호 ye 다음과 같다.

ae,
|o oh
rovad rr
= "가 a

1
y=xt—z                     (13.31)
B

Dy!

ZF 사전등화는 BE 채널에 공통적인 YAS 곱하기 때문에 전력할당을 수행할 + 없
다. /값에 의한 BS] 증폭현상은 수신단에서 ZF 등화와 동일하므로 BER ASE 동일
하다.

MMSE 사전등화기법도 송신단에서 사용할 수 있다[2631. 송신단에서 MMSE 사전등호
기법을 사용할 경우에는 수신단의 MMSE 기법과는 달리 추가적으로 전체 전력제한이 고
려된다.

그림 13.8의 환경에서 MMSE 기반의 \ 는 다음과 같다.

\=  때 min E{ | B ' (HWx+z)—x |  *}                (13.32)

IN
a
ttlo

만족하고 전력제한이 고려되지 않은 최적 pre-MMSE 등화 행렬 \ 는

tio +o
부 jo
ms
Ay

2
W =H’ (HH i                  (13.33)

x



===== PAGE 484 =====
ut

고
[~]

[인
Ob
=
Pl
rt

제13장_ 채널 정보 보를

ZF 기법과 동일하게 사전등화로 인한 전체전력 증가를 제한해야 하므로, 사전등화 행
렬 \ 는 다음과 같다.

\-/2\ B=     __               (13.34)
Tr(WW’)

BER Curve for Rayleigh Channel(QPSK)_

10°F

ro ae    ]
| —6— Linear-MMSE |]
-<ㅎ- Pre-MMSE

BER

0   2   4   6   8   10 12 #14 16 #18 = 20
SNR (dB)
그림 13.9 ZF / MMSE 기법과 pre-MMSE 기법의 BER 성능비교

그림 13.9는 수신단에서 ZF/MMSE 등화를 한 경우와 송신단에서 MMSE 기법을 사용
하여 사전등화를 수행한 경우의 BER 곡선으로서 다음 MATLAB 프로그램 13.4
(“transmission_with_pre MMSE.m”)= 실행시켜서 얻어진 것이다. 이 그림에서 볼 수 있
듯이 pre-MMSE 등화를 수행한 결과 수신단에서의 ZF/MMSE 기법에 비해 성능 이득을

얻는다.

* transmission with pre MMSE.m

clear all; cle;

융융융응응응 Parameter Setting S%3%%%%%%

N_frame=100; N packet=1000;

mod_order=2; M=2“mod_order;

mod_obj=modem.qammod('M',M, 'SymbolOrder', 'Gray','InputType','bit');

487


===== PAGE 485 =====
PART Il_ MIMO2} MATLAB

demod_obj = modem.gamdemod (mod_obj) ;
NTX=4; NRX=4; sq2=sqrt(2); I=eye(NRX,NRX) ;
n_bits = N frame*NTX*mod_order; t_bits = n_bits*N_packet;
PO (===);
fprintf(' Pre-MMSE transmission') ;
fprintf('\n %d x %d MIMO\n %d QAM', NTX,NRX,M);
Eprintt('\n Simulation bits : %d',t_bits);
10111 Nee a ee = ==) I");
SNR_0=0; SNR_step=2; SNR_f=20; SNRs=SNR_0:SNR_step:SNR_f;
for i1_SNR=1: length (SNRs)
SNR = SNRs(i_ SNR); e bits = 0;
rand('seed',1); randn('seed',1);
noise var = NTX*0.5*10*(-SNR/10
육융응응응응응융융응응응응 Transmitter %%%%%
for p_index=1:N_ packet
Input_bit = randint(n bits,1); % bit generation
symbol = modulate (mod_obj,Input_bit).';
Scale = modnorm(symbol, 'avpow',1); % normalization
Symbol nomalized = reshape (Scale*symbol ,NTX,N_ frame) ;
H = (randn (NRX, NTX) +j*randn (NRX, NTX) ) /sq2;
temp_W = H'*inv(H*H'+noise var*I); % 식 (13.33)
beta = sqrt (NTX/trace(temp W*temp W'));
W = beta*temp W; % Eq. (13.34)
Tx_signal = W*Symbol_ nomalized;
육융융응응응응융융응융응응 Channel and Noise %

H*TX signal+sigma* (randn (NRX,N frame) +j*randn(NRX,N frame) ) ;

20090000900000    :   000000000000000090900090
$6 656660066606 RECELVEY F5S5SCSCCCCC EC CC CC CCCOCOS

symbol hat = Rx_signal/beta;
_hat = reshape (symbol hat/Scale,NTX*N_frame,1) ;
Out_bit = demodulate (demod_obj,Symbol_hat) ;
e bits = e bits + sum(Input_bit~=Out_bit) ;
if mod(p_index,1000) ==0,
fprintf('packet : d passed\n',p index) ;
end
end
ber=e bits/t_bits; BER(i_SNR)=ber;
fprint£ ('\t%d\t\t\t%1.4f£\n',SNR,ber) ;
end
semilogy (SNRs, BER, '-k*','LineWidth',2) ;hold on;grid on;
legend(' Pre-MMSE transmission') ;xlabel('SNR (dB)'),ylabel('BER') ;

!

| 프로그램 13.4 Pre-MMSE 등화 기법 프로그램

(



===== PAGE 486 =====
제13장_채널 정보

fui
mee
00
[이
Of
~
a
[또

(3) Tomlinson—Harashima Precoding

지금까지는 WA precodingS 다루었으나, 이번 절에서는 비선형 기법인 TH(Tomlin-
son—Harashima) precoding& 다룬다. TH 베바 Costa2] “writing on dirty paper
result”[264]°] 정보이론에 근거한다. 4, 송신단에서 간섭신호를 미리 안다면 채널 용량에
gag 주지 않는다. 따라서 송신단에서 적합한 부호화를 한다면 dao] 없는 채널환경과
한 채널 용량을 얻을 수 있다. 이를 간단한 블록도로 표현하면 그림 13.10과 같다.

Zz
4   Z       Decoder     :
WD                               >

이

ae
fe)

ne,

=.      Encoder     :

I
그림 13.10 Costa2| 정보이론 블록도

Xa)                      Sa                                                4   yo                      Xa
me                                         mH      ~                        ~

WY

Encoder1                >        mS     Decoder1
Za)
X)          Sa                       [1 y(2)           XQ)
——?| Encoder2       p> >}  He)    aU,  ~| Decoder2 ~
Za)
XG)          Se)                       | yo          XG)
——+¥ | Encoder3          | ———__>  He)    aa /  려 Decoder3 ;-—_>
;                            3           .
ㆍ                            e              ㆍ
           Si                            75          Kw
그늘 Encoderk  본            는  Hw    >) Decoderk >

그림 13.11 다중 간섭채널의 CostaQ| BEX

489



===== PAGE 487 =====
PART 비 MIMO} MATLAB

이 기법은 다중 간섭 채널에 적용할 수 있다. 다중 간섭 채널에서의 부호화는 순차적으
로 진행된다. 첫 번째 신호는 나머지 채널로부터 모든 간섭신호를 받게 된다. 이 시점에서
는 간섭신호에 대하여 알 수가 없기 때문이다. 두 번째 신호는 첫 번째 신호와 채널정보를
이용하여 Al 번째 신호에 의한 간섭성분을 제거 할 수 있기 때문에 Costa precoding] 가
능하다. 결론적으로 《번째 ASS 고려할 때 1부터 * -1까지의 모든 간섭의 영향은 제거
될 수 있다. 이 전체 과정을 그림 13.11과 같이 표현할 수 있다.

이러한 기법을 141040채널에도 동일하게 적용할 수 있다[265]. 만약 MIMO 시스템에
서 송신단이 Costa [00000108을 사용한다면 하위채널에서 상위채널로의 간섭은 발생하지
않는다. 즉, HS 하삼각행렬과 직교 행렬로 분해하고 Costa precodings 적용하면 하위
채널에서 상위채널로의 간섭을 제거할 수 있고 결국 대각행렬만 남게 된다.

Costas precoding? 개념적으로 수신단의 DFE(Decision Feedback 80481123000)와 매
우 유사하다. 여기서 비선형 연산인 modulo 작업을 추가적으로 사용하는 기법이 TH
206000108이다[266][267]1.

MIMO 채널환경에서의 TH 0『60000108[268]을 설명하기에 앞서 송신신호벡터 와
칭 00000연산을 다음과 같이 정의한다. 메시지 신호 ×,는 M-ary 0444으로 변조된
SEM 실수축과 허수축이 각각 [-4/2,4/2) 의 경계로 이루어져 있고 이 때 4=./74 을

ry

만족한다.
수 |mag
 Imag      Fy    내  ,  ㆍ    .  .
A Imag    해  "  년  *     ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ
ㆍ : Real   *  로  *  ㆍ: Real   ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ  ㆍ: Real
(a) 4-QAM        (b) 16-—QAM                  (c) 64-QAM

그림 13.12 M-ary QAMO|] 해당하는 성상도

_ 490



===== PAGE 488 =====
그림 13.13 대칭 modulo 연산의 예

. A 10789 .
C]   : (] J
O + | Qi + ©
oe
on  on + ©

그림 13.14 주기적으로 확장된 성상도

대칭 2ㅁ00410연산은 그림 13.13과 같이 경계 값을 넘는 점에 대하여 대칭적으로 modulo

mod,(=x-4| (+4) |                       (13.35)

위의 연산을 그림 13.124 적용하면 -4/2<x< 4/2 Fo 대해서는 대칭적으로
modulo 연산을 수행하고 결과는 그림 13.14와 같이 주기적인 성상도로 생각할 수 있다.

r2



===== PAGE 489 =====
PART 비 MIMO2} MATLAB

TH precoding 후 입출력 관계는 다음과 같다.

y=Bs+z                      (13.36)

B= H 7} Costas precoding 혹은 TH precoding] 의해 간섭이 제거된 유효한 채널
행렬이며, 행렬의 대각성분들이 1이 되도록 정규화된 행렬이다. 예를 들어 Ho] 대하여
QL decomposition? 수행하면 ㅋ=(@2"Ｌ로 분해되고 하삼각행렬인 Lo] 각각의 대각성

분으로 나뉘줌으로써 얻을 수 있다.

B = Diag(1/J,,,---,1/1, )L                     (13.37)

수신부에서는 직교 행렬 QS 수신신호 yo 곱함으로써 유효한 수신신호를 얻을 수
있다.

y=Qy                            (13.38)

유효채널 # 를 통과하는 HAE ASME SE 하위채널에서 상위채널로부터의 간섭이

제거됨으로써 얻을 수
에 미치는 간섭이 제거
는 간섭이 제거됨으로
TH precoding JE 변조된 ASH  i. s= 얻기 위해 추가적으로 대칭 modulo 연산을
행한다. 대칭 modulo 연산은 —A/2<s5, < A/2 Yo] 존재 할 수 있도록 $,에 대하여
000410연산을 수행한다. 따라서 s, = 다음과 같이 얻는다.

들면, 첫 때 신호가 두 번째, 세 번째 등 이후의 신호
두 번째 신호가 세 번째, 네 번째 등 이후의 신호에 미치

~ aor
떠요
al

Ae,
i   ie
in   >
ZO,
zo

s, =mod, (x, —b,,8,)                              (13.39)
여기서 / =지이다. 이를 일반화 하면 아래의 식을 얻는다.
1
s, =mod (x, - ¥ 656)                             (13.40)

492


===== PAGE 490 =====
제13장_채널 정보를 활용한 송신 기법
수신단에서의 최상의 수신신호 Py 는 다음과 같다.
Fg 0“하후
K      ~
= % DS tx                          (13.41)

여기서, \『 는 # 의 kw YS 말한다. b, =1이므로 최종적인 수신신호는 다음과
같다.

K-l      K-1
mod , (Fx, J=mMod, (X_ — Z de xy + Z bya + 2)                  (13.42)

=mod, (x, +2Z,)

따라서 대칭 modulo AALS 통해 메시지 벡터 xS 복원할 수 있다. TH-precoding &
도는 다음과 같다.

2

y
3

그림 13.15 TH-precoding 2S

vy?
a]

Vv

modulo                                                                      modulo [>

위 그림을 다시 유효채널을 이용하여 간단히 표현하면 그림 13.16과 같다.

2
Be                          modulo [>

그림 13.16 TH precoding 유효채널 블록도

노어

modulo

493



===== PAGE 491 =====
PART 11 )1140와 MATLAB

( 5. 인테나 선택 기법

MIMO 시스템은 추가적인 주파수를 사용하지 않으며 전송률을 높이는 장점이 gaz
추가적인 RF 모듈 등 높은 하드웨어 복잡도가 요구된다. RF 모듈에 속한 요소로는 저잡
음 증폭기(10\ noise amplifier), 하향 주파수 변환기(6604600 down converter), ADC 등
이 있고 이러한 RF BSS 일반적으로 매우 고가다. 이러한 문제를 해결하는 방안으로 of
러 개의 빼장비를 제외한 구리선으로만 이루어진 안테나만을 설치하고 이 안테나 중에
몇 개를 선택함으로써 적은 수의 RF PEWS 사용하는 기법이 있다. 이러한 기법을 안테
나 선택기법이라고 하고 간단한 블록도는 그림 13.17과 같다.

ee

2                 ;

ㆍ                                          .          Space time            Data

:                                          :             cording               sink
Y Nr

Nr

그림 13.17 안테나 선택기법 블록도

Data       | Space time
source} ~| cording

of
+)
.

신호의 관계는 A] (13.43)과 같다.
y=Hx+z                           (13.43)

여기서 xec™, yec™™, He ce, 26 Colt. 즉 N, 7} 안테
나 중에 개 만을 선택하여 송신한다.

GERRY 안테나 선택 기법 적용 시 채널 용량

안테나 선택기법에서의 채널 용량은 전체 송신전력이 로 제한이 되어있을 때 다음과
같이 얻을 수 있다.
C = max log, det(I  +s_HR H,") bps/Hz
ai  So    Ne” py ss   Pp                 (13.44)

0

494



===== PAGE 492 =====
제13장_ 채널 정보를 활용

ro
ob

=
고
rf

R,, 는 PXP 로 이루어진 600808006 행렬이고, HE HBSS] 선택된 열로 이루어
Al effective 채널을 나타낸다.

만약 채널에 대한 모든 정보를 알고 안테나마다 동일한 전력
표현할 수 있고 이 때의 채널 용량은 식 (13.49)와 같이 표현

C, =log, 0060                i") pps/Hz                          (13.45)

문제점은 어떻게 최대용량을 얻을 수 있게끔 HFS PH] SS 선택하는 방법이
다. 최적의 방법은 NCp 7A 조합에 대해 채널 용량을 모두 계산하여 비교하는 방법이다.
하지만 이 방법은 너무 많은 AAS 요구하므로 근사화한 WAS 사용한다. 이 근사화된
방법들에 대해 13.3.2절에서 다룬다.
그림 13.18은 각각 기본적인 401040에서의 채널 용량과 MATLAB 프로그램 13.6
(“MIMO_channel_capacity.m”)& 실행시켜서 얻어진 최적의 안테나 선택기법의 채널 용
FS 나타낸다. 그림에서 볼 수 있듯이 안테나 선택기법이 고려된 경우 전체 4개의 가용
안테나에서 3개만 AAS 하더라도 채널 용량측면에서는 4개를 모두 사용하는 BPS 거

의 동일한 성능을 얻는다.

Capacity of non-Antenna selection optimal                                        Capacity of non-Antenna selection optimal

11                                ;                7        7        7        ;                 11                                                ;        7        ;

—3— 4-1x         '        {        i        \        {        {        '                        —8— 4-Antenna select] |                '
10}| —@— 3-Tx     :     H     도니새재새나     $    -t- ae      10}| —— 3-Antenna select} -+------1------4-

—A— 2-Tx       {                                   {       {                    -ㅡ슬- 2-Antenna select} |
9         이지애                              1-Antenna select} _'                                   개
8
"                                                                                     주
6                                                                                     g
5
4                                                                                             ai
3                                                                                           i
2t                                                                                        2 |

0       1       2       3      4      5       6       7      8      9 10                  1       2       3      4      5      6              8      9 10
SNR (dB)                                                                            SNR (dB)

그림 13.18 기본적인 MIMO 시스템과 안테나 선택기법이 고려된 시스템의 채널 용량

495



===== PAGE 493 =====
PART 141 _01140와 MATLAB

MATLAB 프로그램 : 최적9

택기법의 채널 용량

* MIMO_channel_capacity.m
clear all; clc;
NT=4; NR=4; MaxIter=1000;
sel_ant=3;
I=eye (NR,NR); sq2=sqrt (2) ;
SNR_0=0; SNR_step=1; SNR_f=10; SNRs=SNR_0:SNR_step:SNR_f;
for i_SNR=1:length (SNRs)
SNR = SNRs(i_ SNR); tmp_c = zeros(1,1);
SNR_linear = 10*(SNR/10); SNR_sel_ant = SNR_linear/sel ant;
rand('seed',1); randn('seed',1); cum = 0;
for i=1:MaxIter
H = (randn(NR,NT)+j*randn(NR,NT) ) /sq2;
if sel_ant>NT||sel_ant<1
error('sel_ant must be between 1 and NT!');
elseif sel_ant==NT, indices = [1:NT];
else indices = NCHOOSEK([1:NT],sel_ant) ;
end

for n=1:size(indices,1)
Hn = H(:,indices(n,:));
log_SH(n) =log2 (real (det (I+SNR_sel_ant*Hn*Hn'))); ¢ “4 (13.45)
end
cum = cum + max(log_ SH) ;
end
sel_capacity(i_SNR) = cum/MaxIter;
end
plot (SNRs,sel_capacity, '-ko','LineWidth',2); hold on;
xlabel('SNR[dB]'), ylabel('bps/Hz'), grid on;
title('Capacity of Antenna seletion optimal')

i 프로그램 13.5 최적의 안테나 선택기법 적용시 채널 용량 실행 프로그램

GRR) 선택 복잡도 감소 기법
연

최적 안테나 선택기법으
순 선택기법이 있다.

산량을 줄이기 위한 기법에는 오름차순 선택기법과 내림차

496



===== PAGE 494 =====
제13장_채널 정보를 활용한 송신 기법

먼저 오름차순 선택기법은 처음에 하나를 선택하고 #깨까지 점진적으로 추가시키는 방
법이다. 즉, 번만큼 반복수행을 하였다면 HO] 채널 중 {p,...p,} 만큼 선택이 된다. 따
라서, 채널 HE ^,×로 HW, 선택채널로 바뀌게 된다. 추가적으로 / 번째 안테나를
추가하기 위한 기준을 마련하기 위해 / 번째 안테나가 고려된 채널 용량은 식 (13.46)과
같다.

bac)

E
C, =log, det(I,, +—*-(H     H’ | +H,H/’))
1          ^,   PN,                 가.

Pisa 기이

‘i                        x          i                     (13.46)
=log, det(Iy, + Py, 트, 80" rom) tog (+ 5 (dy, + PN, 브, 802.) Hr)
위의 유도과정에는 다음의 관계가 사용되었다.
det(A + uv’) =(1+v’ A ‘u)det(A)                                (13.47)
채널 BSS 최대화 하는 추가 열의 AAS 다음과 같이 수행된다.
Poo = AB MAX Hy,  +H, H)) HY                      (13.48)
위의 역행렬 연산을 효율적으로 하기 위해 다음 관계가 사용된다.
(Ataa”)'=A'-A'‘a(it+a“A'a)'a“ A"!                         (13.49)

내림차순 선택기법은 전체 채널 HS 가장 최소로 채널 용량을 감소시키는 채널부터
하나씩 제거해 나가는 기법이다. 따라서 식 (13.46)에서 HH! 대신에 -8.8/ 를 대입함
으로써 얻을 수 있다. 내림차순 선택기법은 처음부터 전체 VS 고려하기 때문에 같은

반복수행을 실행했다면 오름차순 선택기법보다 더 많은 연산 복잡도를 요구한다. 그러나

c
4

능 면에서는 내림차순 선택기법이 우월하다. 이유로는 내림차순 선택기법은 모든 채널
간 영향을 고려하여 최소로 영향을 미치는 열부터 하나씩 빼나가지만 오름차순 선택기
은 처음 시작 때 독립적으로 각 열의 영향만 계산하여 선택하기 때문이다. 내림차순 A

기법은 선택하는 안테나수가 전체 가용 안테나 수보다 하나 작을 때는 최적의 선택기법

비 i ch 08 ^

497

00095 tC


===== PAGE 495 =====
PART 때 41140 와 MATLAB

GEER STBCHA2] 최소 오류 확률

안테나 선택기준으로 채널 BES 최대화하는 기준뿐만 아니라 오류가 최소가 되도록
하는 기준을 사용할 수도 있다. 9180의 한 종류인 OSTBC(Orthogonal 818)에서의
SER 확률의 upper bound 아래와 같다.

오오            -N;Np
           !           N,              SNR
P(S(i) > S(j)) < fs [  |       e |                                   (13.50)

이 때, E,,= 코드워드인 SH SY)F 차행렬이고, 이는 고정된 값이므로 위의
60400는 5찌에 의해서만 영향을 받는다.

선택된 채널을 쁘,라고 하고 개의 안테나를 사용한다면 각 안테나별 수신 SNR
(13.51)과 같다.

clo

Al
a

‘NR
n= SH, |"                            (13.51)

따라서 최소의 SERS 달성하기 위해서 |8,|%가 최대가 되도록 안테나를 선택해야 한
다. 내림차순으로 정렬된 채널 중에 개의 평균은 전체 평균과의 관계가 다음과 같다.

(13.52)

또한, 전체 AL] Frobenius norm 은 선택된 채널의 Frobenius ㅁ010과의 관계가 다음
과 같다.

2
opt
Hy" |.

<|H |.                                    (13.53)

위의 FAS 결합하면 최적의 안테나 선택기법의 SNR 상위와 하위 경계는 식 (13.54)

498



===== PAGE 496 =====
제13장_채널 정보를 활용한 송신 기법

SNR           SNR

= IAl  = le      구비                    (13.54)

상위 경계와 하위 경계 모두 전체 채널의 Frobenius norm 의 영향을 받는다. 따라서
iid 채널인 Hy 의 경우 2N~N, 만큼 자유도를 가진 chi-square 변수가 되므로 송신 다
이버시티는 N,N, 가 된다.

10°

PA ee

「| —@— Alamouti with antenna selection 2x1 in 4x1

i

0            2            4            6            8           10          12          14
SNR (dB)

그림 13.19 Alamouti 부호를 이용한 안테나 선택기법의 BER AS

% Alamouti_2x1_ant_selection.m

clear all; cle;

$%%%% Parameter Setting %%%%%%%%%

N_packet=100; N_frame=100;

mod_order=2; M= 2“mod_order;
mod_obj=modem.qammod('M',M, 'SymbolOrder!, 'Gray','InputType', 'bit');
demod_obj = modem.qamdemod (mod_ob}) ;

% MIMO Parameters

T TX=4; NTX=2; NRX=1; sq2=sqrt (2);

n_bits=NTX*mod_order*N frame; t_bits=n_bits*N packet;

POMC h ("eee a ee eee ee |) ;
fprintf£(' Ant selection transmission') ;

fprintf('\n %d x ¢d MIMO\n %d QAM', NTX,NRX,M);

499



===== PAGE 497 =====
PART I]. MIMO&+ MATLAB

SNR_0=0; SNR_step=2; SNR_f=20; SNRs=SNR_0:SNR_step:SNR f;
for i_SNR=1: length (SNRs)
SNR = SNRs(i_SNR); e bits = 0;
noise_var = NTX*0.5*10*(-SNR/10) ;
육융융육응융응응응응응응 TYANSMItteEr SSSSSSSSSSSSSSSSSF
for p_index=1:N_packet
x = randint (n_bits,1); % bit generation
8 = modulate (mod_obj, x);
Scale = modnorm(s, 'avpow',1); % normalization factor
S=reshape (Scale*s,NTX,1,N_ frame) ;

rand('seed',1); randn('seed',1)

oP

Tx_symbol=[S(1,1,:) -conj(S(2,1,:)); S(2,1,:) conj(S(1,1,:))];

pa 2

융융융응융응응응응응응응응 Channel and Noise %%%%33%%%%3%%
= (randn(NRX,T_TX)+j*randn (NRX,T_TX))/sq2;
for TX_index=1:T TX
ch(TX_index) =norm(H(:,TX index), 'fro');
end
[7231 , Index] = sort (ch, 'descend') ;
Hs = H(:,Index([1 2] ) ) ;
norm _H2=norm(Hs,'fro')*2; % H selected and its norm2
for i=1:N_ frame
RX(:,:,1) = Hs*Tx symbol(:,:,i) +...
sigma* (randn (NRX, 2) +j*randn (NRX, 2) ) ;

end
육융융응응응응융융융융응응 RECCLVED SSSSSSSESSEEESESESEES
for i=1:N frame
s_hat(1,i) = (Hs(1)'*RX(:,1,1)+Hs(2)*RX(:,2,i)') /norm_H2;
s_hat(2,i) = (Hs(2)'*RX(:,1,i)-Hs(1)*RX(:,2,i)')/norm_H2;
end

S_hat = reshape (s_hat/Scale,NTX*N_frame,1) ;
=      demodulate (demod_obj,S_hat) ;
6 bits = e bits + sum(x_hat~=x) ;

end

ber = e bits/t_bits; BER(i_ SNR) = ber;

fprint£ ('\t%d\t\t\t%1.4f£\n',SNR,ber) ;
end
semilogy (SNRs,BER, '-k*','LineWidth',2) ;hold on; grid on;
legend(' Ant-selection transmission') ;
xlabel('SNR (dB)'),ylabel('BER') ;

ad
년"
00
다
1

—

i 프로그램 13.6 안테나 선택기법 실행 프로그램

500



===== PAGE 498 =====
다중 사용자 MIMO 시스템에서 상향 링크는 한 개 이상의 안테나를 가진 다수의 사용
자에서 송신한 신호를 두 개 이상의 안테나를 가진 하나의 기지국에서 수신하는 모델이다.
하향 링크는 두 개 이상의 안테나를 가진 하나의 기지국에서 한 개 이상의 안테나를 가진
다수의 사용자에게 신호를 송신하는 모델이다. 이와 같은 다중 사용자 MIMO 시스템 모
델을 그림 14.1과 같이 표현하였다. 단일 사용자 MIMO 시스템의 경우에는 송신 안테나
개수 N; 와 수신 안테나 개수 Ny 이 주어졌을 때, min(W,,N,) 에 비례하여 채널 용량이
증가한다[211][269]-[2711. 기지국의 안테나 개수 Ny =N, 이고, 이동 단말기 안테나 개
수 Ny =, 임을 가정하면, 다중 사용자 MIMO 시스템의 경우에는 송수신 안테나의 개
수뿐만 아니라 단말기의 개수 《 가 주어졌을 때, sum rate 응량이 00008,.2040)에 비례
하여 채널 용량이 증가한다[272][2731.

AS Base Station
Downlink                     rar                                                   Uplink

(Broadcast)                                                                            (Multiple access)

sy ye

Mobile Station
(User)

그림 14.1 다중 사용자 MIMO 시스템의 상향 링크와 하향 링크 채널

501


===== PAGE 499 =====
OOPS os 사용자 mimo 시스템 모델

절에서는 앞 절에서 설명한 다중 사용자 MIMO 시스템 모델을 정의한다. 본 절에서
는 ^ 개의 안테나를 가진 하나의 기지국과 ”,, 개의 안테나를 가진 “개의 사용자 단말
기를 고려한다. 먼저 MIMO 상향 링크 채널의 시스템 Bas 정의한다. 그림 14.2를 다중
접속 채널의 시스템 BAS 보여주고 있다. 그림 14.2에서 WY & i 번째 단말기의 상향 링
크 채널 행렬이고, x, "^ '는 1 번째 사용자로부터 전송된 신호이다. yy S C8!
는 기지국에서 수신한 신호이고, 2S CL 환형 대칭 Gaussian 잡음이다. 이와 같
은 다중 접속 채널의 시스템 모델을 수식으로 표현하면 다음과 같다.

re

x,
Yuac = HY x, + Hx, +--+Hex, +z=H"| : |+2               (14.1)

> Hy
\ |

xXK—>    Hy

그림 14.2 다중 사용자 MIMO 시스템의 상향 링크 모델

그림 14.3은 다중 사용자 MIMO 시스템의 하향 링크 채널 Bas 보여준다.
그림 14.3에서 BPE i Aa 사용자와 기지국사이의 하향 링크 채널 행렬이다. 벡터
포드 67 는 기지국에서 ASS 신호이고, y,eCM tL 1 번째 단말기에서 수신한
신호 벡터이다. =e ㅇ”*^'는 환형 대칭 Gaussian 잡음이다. 이와 같은 하향 링크 채
널의 시스템 모델에서 번째 사용자가 수신하는 신호를 식으로 표현하면 다음과 같다.

y, 2H + 2,                                            (14.2)

502



===== PAGE 500 =====
제14장_다중 사용자 MIMO 기법

H? a ~,

그림 14.3 다중 사용자 MIMO 시스템의 하향 링크 채널 모델

일 사용자 다이버시티 기법은 데이터 전송 속도의 향상보다는 높은 링크 품질을 얻는
bal 중 하나이다. 다중 정로 전파와 shadowing 효과 등에 의해 신호의 WH] 심하게 되
데 단일 사용자 다이버시티 기법에서는 다양한 페이딩 채널을 경혐한 여러 개의 신호를

|

합하거나 동일한 ASS 2번 이상 전송하여 결합함으로써 다이버시티 이득을 얻는다.

신호 결합 방법으로는 앞 장에서 설명한 것과 같이 MRC(Maximal Ratio
Combining), SC(Selection Combining), EGC(Equal Gain Combining)-5-°] 있다[274]. 다
이버시티 SS 통해 그림 14.49} 같이 신호가 시변한 채널이 아닌 정적 AUS 경험한
것과 같은 효과를 얻을 수 있다.

> ne clr ok
r= oh 프

Channel                Channel
Strength                         Strength
|                   |
^     | |
ㅣ     |
||
| |       \ |
|| /\ | | (\ |      a
VE VA 00
\ |    \  VU  V v
|             Time   |                Time
Time-varying channel                            Constant channel

그림 14.4 다이버시티에 의한 효과



===== PAGE 501 =====
PART IIl_ 41140 와 MATLAB

중 사용자 다이버시티는 단일 사용자 다이버시티 기법과는 달리 독립적인 채널상태
한 다수 사용자들의 신호를 기지국에서 선택함으로써 얻는 이득이다[275][2761.
대역에서 최적의 채널을 가진 사용자를 선택함으로써 얻는 다중 사용자 다이버시티
사용자 간 채널이 서로 독립적이라고 가정할 때 주파수 선택적 페이딩 채널을 활용한
. 많은 사용자들의 ASS 중 특정 시간에 상태가 좋은 채널이 존재할 가능성이 높으므
로 채널 상태가 좋은 사용자를 선택하여 통신한다면 전체 전송량을 극대화 할 수 있다. 그
러므로 채널 변화가 큰 Rayleigh 페이딩 환경이 채널 변화가 작은 81018 페이딩 환경에
비해 다중 사용자 다이버시티의 효과를 더 크게 얻을 수 있다. 그림 14.5는 4개의 송신 안
BUS 가진 기지국에서 1개의 수신 안테나를 가진 다수의 사용자들 중 채널 상태가 좋은
4명의 사용자를 선택한 후, 14.4.2절에서 7]S5]+ regularized channel inversion 기법을
이용하여 전송 시 사용자 수에 따른 성능 곡선을 나타낸 것이다. 사용자의 수가 증가할수
널을

 :

의

^

©.

Sh clr fm al

ilo

록 다중 사용자 다이버시티 이득이 커짐을 알 수 있다. 모든 사용자가 느린 페이딩 채
경험한다면 사용자간 채널 상태의 카이가 크지 않으므로 다중 사용자 다이버시티 이득을
크게 얻지 못한다. 이러한 환경에서는 다중 사용자 다이버시티 이득을 높이기 위해서 기
지국에서 다중 안테나를 사용하여 의도적으로 더 크고 빠르게 채널의 변화가 일어나도록
SoHE opportunistic 빔형성 기법을 사용할 수 있다[277]. Opportunistic 빔형성 기법은 그

림 14.6과 같이 기지국의 각 안테나에 불규칙한 형태의 크기와 위상을 갖는 SSS 곱
해 줌으로서 마치 불규칙한 방향으로 빔을 형성하는 효과를 얻게 되고, 이는 각 사용자들
의 채널 상황을 좀 더 역동적으로 바꾸게 된다. 따라서 채널이 느리게 변화하는 채널에서

Performance (QPSK)

-| —@— User 4 (N,:4, Selected user: 4) |
-|—8-— User 10 (N,°4, Selected user:4)
.--|—+— User 20 (N,:4, Selected user:4)
,__.|—@— User 30 (N,:4, Selected user:4)
—A— User 60 (N,:4, Selected user:4)

aes

0

0 2 4 6 8 10 12 14 16 18 20
SNR (08)

그림 14.5 사용자 수의 증가에 따른 다중사용자 다이버시티 효과

504


===== PAGE 502 =====
제14장_다중 사용자 MIMO 기법

\000)
_ >60 느
a(t)
Base =                  ae       Mobile

V1—alt) 600

그림 14.6 Opportunistic 빔형성 기법

opportunistic 빔형성 기법을 사용하고 가장 좋은 채널 환경의 사용자를 선택하게 되면 더
= OS bial 다이버시티 OSS oo 수 있다.

ISS 극대화하기 위해 특정 시간에 가장  At 채널을 갖는 사용자를 선택하는 스케
wag 선택한다면 전체 sum rate 채널 용량이 증가하겠지만 사용자간 자원의 할당
이 공정하지 않거나, 자원을 할당 받기 위해 = 시연 ㅣ 발생할 수 있다. 이와 같은 문제를
해결하기 위해 다양한 스케즐링 방식이 제안되었으며 대표적인 기법으로는 (00400 robin
스케즐링, 0660 274, proportional 131 스케즐링  is  ke ㅣ 있다. 이 중 proportional
fair AAS] 방식은 각 사용자의 순시적인 채널 상태를        적인 상태로 나눈 값이
가장 큰 사용자에게 자원을 할당하여, 다중 사용자 eee
공평성 문제를 해결한다[278][2791.

저
ue
#4

6. 43 사용자 mimo 시스템의 채널 용량

본 절에서는 다중 사용자 채널의 상향 링크와 하향 링크의 채널 용량을 살펴본다.
Gaussian 채널에서 상향 링크 채널과 하향 링크 채널에 대하여 앞 절에서 설명한 시스템
모델을 기반으로 설명한다.

EM 다중 사용자 Mimo 시스템의 상향 링크 채널 용량
본 절에서는 다중 사용자 MIMO 시스템의 상향 링크 채널 용량을 다룬다. 일반적인 상
향 링크 채널의 용량 영역은 [280]에서 처음으로 were 단일 안테나를 가진 두 사용
자가 상향 링크 채널에서의 용량 영역은 A) (14.3)과 같이 주어진다[281]. 여기서
h,f=1,2% i 번째 사용자의 채널을 나타낸다.



===== PAGE 503 =====
PART Il_ MIMO2} MATLAB

R, <log(1+|h, | 2)
R, Slog(1+[,[° 42)                              (14.3)

R, +R, <log(1+|h,|/ 2 +|h,|° 2)

A
A

Ry
log(1 + hy ||? Pi) 도기 ：

Ri + Ry < log( +|| hy ||P; + fe 120

\

ㅣ
|
|
|
1

R
log(1 +|| In ||? Pa)

그림 14.7 다중 사용자 MIMO 시스템 상향 링크 채널 용량 영역 (사용자의 안테나가 1개인 경우)

그림 14.72 단일 안테나를 가진 두 사용자가 상향 링크 채널에서의 용량 영역을 나
낸다. 위의 영역에서 A BS 달성하기 위해서, 제 1 사용자는 제 2 사용자의 신호를 간
으로 취급하여 데이터를 전송하고, 제 2 사용자는 제 1 사용자의 ASS 기지국에서 검출
및 제거하여 간섭 없이 데이터를 전송한다. 유사하게, CHS 달성하기 위해서는 제 2 사
용자는 제 1 사용자의 신호를 간섭으로 여기고, 제 1 사용자는 간섭이 없는 상황으로 여기
고 데이터를 전송한다. A 점과 0 Bo] 중간 지점을 나타내는 구간은 위의 두 가지 극단적
인 송신방식의 시분할 또는 전송량 분할로 달성할 수 있다.

여러 안테나를 가진 여러 사용자 시스템의 채널 Beko] 영역을 정적 채널에 대하여, 전
력은 P=(P,....P,) 2 제한하고, 주어진 채널이 HY 일 때 상향 링크 채널 용량은 아래
식 (14.4)과 같이 나타낼 수 있다.

08 -뛰

(20 )

비베" )S                       14.4
aso 214. 10801. +P)" QM! | WS hk me

ieS                                             ieS

 506



===== PAGE 504 =====
제14장_다중 사용자 MIMO 기법

여기서 @,=씨조페 |이다. 식 (14.4)를 통해 의 영역이 《차원의 다면체가 됨을
알 수 있다. 각 사용자의 안테나 개수가 하나인 경우 각 사용자의 000808066 행렬의 송신
일한 크기이므로 사용자를 위한 용량 영역은 다음과 같다.

YR, < log 테티 + 2000. |. c{i,...,K}                      (14.5)

ieS                                                  ieS

다중 사용자 MIMO 상향 링크의 910 rate 용량은 일대일 N,xN,K MIMOS] 용량과
유사하게 되므로, 대략 min(Ns, Nuk)log(SNR)2] 다중화 SS 얻을 수 있다[282].

으 다중 사용자 MIMO 시스템의 하향 링크 채널 용량

본 절에서는 다중 안테나 MIMO 시스템의 하향 링크 채널 용량에 대해 살펴본다. 먼 ;
일반적인 하향 링크 채널과 단일 안테나 하향  ale 채널에 대해 살펴보고, 하향 링크를
한 DPC(Dirty Paper Coding) 설명을 통해 용량을 살펴본다[264][2831. 상향 링크와 달
리 하향 링크 용량 영역에 대한 정확한 수식적 유도는 아직 해결되지 못한 문제로 남아있
다. 그러나 대략적인 하향 링크 채널의 용량 영역은 알려졌다. 먼저, 두 사용자가 단일 안
테나 하향 링크 채널에서 용량 영역은 식 (14.6)과 같이 표현할 수 있다.

5

R< 10811 +에띠 리

나 ae    ae [0,1]                     (14.6)

RS 1+
: = 이티 211

다중 사용자 MIMO 시스템의 하향링크의 채널 용량을 계산하는데, 하향링크와 상향링
AL RF} dualityS 이용할 수 있다. A] (14.7)과 (14.8)은 DPC 기법을 통해 계산된 채널
용량과 상향 링크 채널 용량과의 관계를 수식적으로 표현한 것이다.

Cope (PH) =  U  Cac (PR이PH’)          (14.7)

507


===== PAGE 505 =====
PART I_ MIMO2} MATLAB

Gigs Bet =| | Ce 이제 ]                  (14.8)

a>0             i=] 4;

- 4

10, 20.5 000, )sP|

(RyRy):                                               (14.9)
> 0% <logdet(I,, +) HQ,H,) VS cf{l,...,K}

여기서 @, 는 MAC covariance 행렬들이다.

GREET 다중 사용자 mimo 하향 링크 송신 기법

32259 Channel Inversion 기법

본 절에서는 다수의 안테나를 가진 기지국과 하나의 안테나를 가진 다수의 사용자를 가
정하고 송신 기법에 대해 설명한다. 하나의 안테나를 가진 단말기에서는 다른 단말기의
ASS 제거할 수 없다. 단말은 한 개의 안테나를 갖고, 즉, Ny =N,=1, 기지국은 N,
개의 안테나를 갖고 있으며, 사용자의 수 K=N, 라 가정한다. 이 때 1 번째 사용자의 신
SS d,,i=l,2,....K 라 하고, 4, 가 번째 송신안테나의 신호 지라 하고, y,,f=1,2,...,K
가 번째 사용자의 수신신호라 하면 다음 관계가 성립한다.

22 | _  h, || x,  +  22
|                                                       (14.10)

Vx      hy |      2x

y         H      x         2

 508



===== PAGE 506 =====
제14장_다중 사용자 MIMO 기법

여기서, hy 01^^는 7 번째 사용자의 채널을 나타낸다.

기지국에서 전송 시 미리 간섭 신호를 제거해 줄 수 QUE precodingS 이용한 송신 기법
을 사용할 수 있다. Precoding 7]'4ol+ channel inversion, regularized channel inversion,
sphere encoding, iterative interference balancing, 전력 제어와 같은 다양한 기법들이 있
다. 본 절에서는 018006| inversionZ} regularized channel inversiono] 대해 설명한다
[289]-[296].

Channel inversion 채널의 의사 역행렬 a  이용하여 precodings}o] 전송하는 기법
이다[289]-[293]. 아래 수식과 같이 AS 신호를 표현 할 수 있다. 본 절에서는 K=Nr
를 가정하였으므로 HO 의사 역행렬을 Ho] 역행렬과 동일하기 되나, 다음 절의
regularized channel inversionz}2] 일관성을 위해 의사 역행렬을 사용한다.

1
x =H" (HH”)'d                        (14.11)

et

스케일링 인자 y 같은 제한된 AS 전력 |제 = 을 이용하여 아래 수식과 같이 구할

수 있다

= HH" (HH")'d+2=—-d+z              (14.13)

vy   vy

여기서 값은 심볼에 따라 변경된다. 이런 문제점을 피하기 위해 》값은 평균 전
력을 이용해 계산할 수 있다.

ob»
로비

/=-피000) |                   (14.14)

|

509



===== PAGE 507 =====
PART 미_ MIMO2} MATLAB

Encoding             Channel

그림 14.8 Channel Inversion 기법

40254 Regularized Channel Inversion 기법

QF 절에서 설명한 channel inversion 기법은 rank—deficient 채널인 경우 잡음 증폭 A
상이 발생한다. Channel 10\619100에서 사용된 ZF 필터 대신 MMSE 필터 방식을 사용하
는 regularized channel inversion& 통해 잡음 증폭 현상을 감소시킬 수 있다[289]-[2931.
Regularized channel 107669100은 잡음이 공간적으로 화이트 잡음이고 적절한 정규화된 값
이 선택된다면 이것은 빔형성 계수 값을 MMSE 기준으로 계산하는 것과 같다. Regula-
rized channel 107689100된 전송신호를 수식으로 나타내면 식 (14.15)와 같다.

x =—=H"” (HH" +¢1)'4                        (14.15)

vy

Performance (QPSK)

10

10

—@— Channel Inversion (NB=NT=4, User:20/Selected User:4)         =
| | —&-— Regularized channel inversion (Tx:4, User:20/SelectedUser:4) |

0 2 4 6 6 10 12 14 16 18 20
SNR (dB)

그림 14.9 다중 사용자 MIMO 시스템의 하향 링크 전송 기법의 성능 곡선

510


===== PAGE 508 =====
제14장_다중 사용자 MIMO 기법

여기서 BES 정규화 파라미터이다. 수신부에서 MMSES} 유사하게, 사용자간의 간섭
은 어느 정도 혀용하며 잡음의 SES 작게 한다. C=K/p 은 각 수신단에서 SINRE 최
대화 하는 값을 선택한다. 그림 14.9는 channel 106161070과 regularized channel inversion
기법의 QBS 성능이다. 기지국의 안테나는 4개이고, 1개의 안테나를 가진 사용자는 20
명이라고 가정한다. Rayleigh 채널상에서 20명의 사용자 중 채널 상태가 가장 좋은 4명을
선택하였다.

% linear_mu_mimo.m
clear all, elec;
SNR_start=0; SNR_step=2; SNR_end=20;
N_frame=100; N_packet=1000;
mod_order=2; M=2“mod_order;
mod_obj=modem.qammod('M',M, 'SymbolOrder', 'Gray', 'InputType', 'bit') ;
demod_obj = modem. qamdemod (mod_obj) ;
NTX=4; NUSER=4; sq2=sqrt(2); I=eye(NUSER,NTX) ;
n_ bits = N_frame*NTX*mod_order; t_bits = n_bits*N_packet;
mode = 0; % ‘0’: channel inversion, ‘1’: regularized channel inversion
for SNR=SNR_start:SNR_step:SNR_end
e bits = 0;
rand('seed',1); randn('seed',1);
noise variance = NTX*0.5*10*(-SNR/10); sigma = sqrt (noise_variance) ;
$SSSSSSSSSSS% Transmitter SSSSSSSSSSSGSS5SSS
for packet_index=1:N_ packet
Input _bit = randint(n_bits,1); % bit generation
symbol = modulate (mod_obj,Input_bit) .';
Scale = modnorm(symbol, 'avpow',1); % normalization
Symbol _nomalized = reshape (Scale*symbol,NTX,N_ frame) ;
for user_index=1:NUSER

H(user_index,:) = (randn(1,NTX) +j*randn(1,NTX) )/sq2;
end
feedback H=[H(1,:); H(2,:);   H(3,|:); H(4,:)];
if mode ==
temp_W = feedback_H'*inv(feedback_H*feedback_H'+noise_variance*I) ;
else
temp W = feedback_H'*inv(feedback_H*feedback_H') ;
end

511



===== PAGE 509 =====
PART Ifl_MIMO2}! MATLAB

beta = sqrt (NTX/trace (temp W*temp W'));
= beta*temp W;
Tx_signal = W*Symbol_nomalized;
융응융응융응응융응융응융응 Channel and Noise $%%%%%%%%%%%%

Rx_signal = feedback _H*Tx signal +
sigma* (randn (NUSER,N_ frame) +j*randn(NUSER,N frame) ) ;
융응응응융융응융융융융융융융 RECCLVEY S3SSSSSSSSESSESSESSE%
symbol hat = Rx signal/beta;
Symbol_hat = reshape (symbol _hat/Scale,NTX*N_frame, 1) ;

Out_bit = demodulate (demod_obj,Symbol_hat) ;
6 bits = e bits + sum(Input_bit~=Out_bit) ;
if mod(packet_index,1000)==0,
fprintf('packet : td passed\n',packet_index); end

end
ber=e_bits/t_bits; BER((SNR-SNR_start) /SNR_step+1) =ber;
fprint£ ('\t%d\t\t\t%1.4f£\n',SNR,ber) ;

end

~

Tm) 프로그램 14.1 Channel inversion 기법과 regularized channel inversion 기법의 실행 프로그램

블록 대각화(8100 Diagonalization) 기법

앞에서 설명한 channel inversion, regularized channel inversion 기법은 단일 안테나를
가진 사용자를 가정하고, 다중 사용자 MIMO 시스템에서 하향 링크 전송 기법에 대해 다
루었다. 본 절에서는 다수의 안테나를 가진 사용자의 경우에 사용 가능한 전송 기법 중 선
형 기법인 블록 대각화(6100 diagonalization) 기법을 설명한다[294]-[2961]. 본 절에서는
다중 vey MIMO 하향 링크 채널 환경에서 K 명의 사용자가 존재한다고 가정하고 송신
안테나 개수는 ^, 로 나타내고, / 번째 사용자의 수신 안테나 개수는 ^/, ,로 나타내며,
전체 사용지의 수 수신 안테나의 개수의 합은 Ne toa 로 나타낸다. 기지국으로부터 번째
ASAE 송신되는 ASS Ne A 벡터 포라 하고, 여기에 곱해지는 ^/,×/^,,
precoding 행렬을 ,라 하면 /번째 사용자의 수신단에서 NR, 수신신호 벡터 ＊, 는

다음 식 (14.16) 같이 나타낼 수 있다.

K
yy =H,M,x;, 때 2 4M    4X FZ;                       (14.16)

512



===== PAGE 510 =====
제14장_다중 사용자 MIMO 기법

여기서 2, 는 수신단의 Nay 차원의 백색 Gaussian 잡음벡터이며, 각 _ 분산은
o lt. 삐,는 Ne XN; 채널 행렬로 각각의 원소는 평균이 0이고
(independent and identically distributed) 복소 Gaussian WY BYES 2 BD 기범은 은
각 사용자의 송신 신호 벡터 x, a 식 (14.17)의 AAS 만족하는 precoding 행렬
\1,ㅎㅁ(^,,7/, )를 곱해서 전송한다.

H;M ; =0 forall i# / and 1<i                   (14.17)

여기에서 U(nk) 는 nxk 차원의 unitary PIS 나타낸다. 위의 조건을 만족하는
방법은 다음과 같다. 먼저 채널 행렬 AS 다음 식 (14.18)과 같

=.
= 반드

precoder M ;

이 정의한다.

=| By ty «A

im  Hy |                 (14.18)

이 때 ( ) 는 행렬의 전치 행렬 연산을 나타낸다. 식 (14.17)의 제약 AALS 충족시키
기 Hai precoder 4, 7} H, 의 null 공간에 속해야 한다. ^, S Ne ,, 를 만족하는
H 2] rankS ^, =} aia,  H, 행렬의 SVD 결과가 다음과 같다고 하면 다음 4] (14.19)
와 같이 표현할 수 있다.

_TTr A  71 yO A
H,=0,A, [¥; v) |                            (14.19)

여기서 ( )" 는 행렬의 Hermitian 연산을 나타내고 Viz} \은 각각 A, 행렬의 첫
N, 개의 고유벡터와 마지막 (4, -#, ] 개의 오른쪽 고유벡터를 의미한다. 그러므로 vo

/ 행렬의 null 공간에 속한 기저 행렬이 된다. 그러므로 4,-/^,>270,,,, 인 경우
v? 만으로는 26000108 YA} Alo] 초과될 수 있으므로, ㅁㅠ6000108 행렬의 차원을 맞
추어 주면서 전송률을 최대화하기 위하여 다음과 같은 과정을 거친다. 우선 HV" 의 541)
를 다음과 같이 계산한다.

|ㅇ

HV? =u,[A, 0] V! Wey"                            (14.20)



===== PAGE 511 =====
PART 미 MIMO2} MATLAB

여기서 Vi 은 HV) 행렬에 의해 VID Mesos 차원의 기저 행렬이 된다. 따라서
Vv, 과 wg 곱함으로써 Nero AA 직교 기저 벡터를 생성할 수 있다. 그러므로 다
음 식 (14.21)과 같은 Bayz precoding 행렬을 결정하면 된다.
M,=V;V;                                       (14.21)
이와 22 BD precoding 기법의 이해를 돕기 위해 4개의 안테나를 가진 하나의 기지국
과 2개의 안테나를 가진 2명의 사용자가 존재하는 경우를 예로 들어 설명하고 모의실험을
수행한다. 기지국과 사용자 1, 2 사이의 채널을 다음 식 (14.22), (14.23)과 같이 나타낼
수 있다.

rN     0 0 0                    H
H, =[u,  Uj ㅣ 대  A. 0  이버  Vin V3  Via |            (14.22)
12
A     0 0 0                     H
H, =[u5,  Un ㅣ 배  A. 0  년  Von Vox Vaal           (14.23)
2

여기서 Mi=[Vis val Hy 행렬의 null 공간에 속한 기저 행렬이 되고
My =[Vos \4]은 Ho 행렬의 null 공간에 속한 기저 Belo} 된다. 사용자 1에게 전송
하고자 하는 2x1 차원의 ATS 피, 사용자 2에게 전송하고자 하는 2×1 차원의 신호를
Xe} 하고 기지국에서는 다음 식 (14.24)과 같은 BHR 전송한다.

x=M,x, +M,x,                           (14.24)

위의 형태의 전송하는 경우 사용자 1, 2가 수신한 ABS 식 (14.25)와 (14.26) 9} 같은

y, =H, (M,x, +M,x,)+z,                          (14.25)

여기서 4] (14.17)2] 기본 원리에 따라 HM, =0 3} HLM, =0 이므로 상대방의 신호
는 제거된다. 그림 14.10은 4개의 안테나를 갖는 기지국이 2개의 안테나를 갖는 2명의 사

514



===== PAGE 512 =====
제14장_다중 사용자 MIMO 기법

Performance (QPSK)
-|—@— Block Diagonaization-ZF detection |

BER

10°          = =         i
0          5          10         15         20         25         30
SNR [dB]

그림 14.10 다중 사용자 MIMO 시스템의 SS 대각화 기법 성능

용자에게 각각 2개의 공간 스트림을 ASRS 때의 사용자 평균 BER 성능이다. 많은 사
용자 중 좋은 채널 SAS 갖는 사용자를 선택하면 성능 개선이 크게 되나, 본 실험에서는
2명의 사용자에 임의의 채널을 할당하였다. 이외에도 60070108660 Tx/Rx 빔형성, combined
8212와 MMSE THP precoding 등 다양한 기법들이 연구되고 있다297]-[2991.

% Block Diagonalization.m
clear all, clc;

oe

6%%%% Parameter Setting %%%%%%%%%

SNR_start=0; SNR_step=2; SNR_end=30;

N_ frame=100; N packet=1000;

mod_order=2; M=2“mod_order;

mod_obj=modem.qammod('M',M, 'SymbolOrder', 'Gray','InputType','bit');
demod_obj = modem.qamdemod(mod_obj) ;

NTX=4; NRX=2; NUSER=2; sq2=sqrt (2);

n_bits = N frame*NTX*mod_order; t_bits = n_bits*N_packet;

for SNR=SNR_start:SNR_step:SNR_end
e bits = 0; rand('seed',1); randn('seed',1);
noise variance = NTX*0.5*10*(-SNR/10); sigma = sqrt (noise variance) ;
for packet_index=1:N_ packet

915



===== PAGE 513 =====
PART IIl_ MIMO2} MATLAB

Input_bit = randint(n bits,1); % bit generation
symbol = modulate (mod_obj,Input_bit).'
Scale = modnorm(symbol, 'avpow',1); % normalization
Symbol_nomalized = reshape (Scale*symbol,NTX,N_ frame) ;
H1 = (randn (NRX, NTX) +j*randn (NRX, NTX) ) /sq2;
H2 = (randn (NRX, NTX) +j*randn (NRX,NTX) ) /sq2;
[U1,S1,V1] = svd(H1); M2=[V1(:,3) V1(:,4)];
[U2,S2,V2] = svd(H2); Ml=[V2(:,3) V2(:  1
Tx_Data=M1* [Symbol nomalized(1 a);
Symbol nomalized(2,:)]+M2* [Symbol nomalized(3,:);
Symbol nomalized(4,:)];
Rx1 = H1*Tx_Data + sigma*(randn(2,N frame)+j*randn(2,N frame) ) ;
Rx2 = H2*Tx Data + sigma*(randn(2,N frame)+j*randn(2,N frame) ) ;
Precoding H1=H1*M1;
temp_W1 = Precoding H1'*inv(Precoding_H1*Precoding_H1') ;
x1_hat=temp_W1*Rx1;
Precoding H2=H2*M2;
temp_W2 = Precoding H2'*inv(Precoding H2*Precoding H2') ;
x2_hat=temp_W2*Rx2;
symbol hat=[xl_hat; x2_hat];
Symbol hat = reshape (symbol hat/Scale,NTX*N_frame,1) ;
Out_bit = demodulate (demod_obj,Symbol_ hat) ;
6 bits = e bits + sum(Input_bit~=Out_bit) ;
if mod(packet_index,1000) ==0,
fprintf('packet : td passed\n',packet_index) ;

end
end
ber=e bits/t_bits; BER((SNR-SNR_start) /SNR_step+1) =ber;
fprintf ('\t%d\t\t\t%1.4£\n',SNR,ber) ;
end

i 프로그램 14.2 블록 대각화 기법의 실행 프로그램

516


===== PAGE 514 =====
MIMO-OFDM
통신 시스템

제15장 IEEE 802.112/ㅁ
제16장 DMB/DVB 시스템
제17장 MB-OFDM 시스템
제18장 와이브로 시스템

제19장 3GPP LTE 시스템



===== PAGE 515 =====
GEES tcc 802.110

본 절에서는 IEEE 802.11a 무선 LAN 규격을 살펴보고, IEEE 802.11a 무선 2 y]O] 기
본블록, 동기부, PLCP(Physical Layer Convergence Procedure)o] 대하여 설명한다. IEEE
802.118에서는 5.15-5.25, 5.25-5.35, 5.725-5.825 002의 U-NII 대역을 사용하는 고
속 ALANS Seles 규정하고 있다[300]. OFDM 방식을 사용하는 IEEE 802.118
의 물리계층의 주요 파라미터는 표 15.1과 같다.

표 15.1 IEEE 802.113 물리계층의 주요 파라미터

PS co ㅎ。』 80 ee
a              6, 9, 12, 18, 24, 36, 48, 54 Mbit/s
20              (6, 12, 24 Mbit/s : mandatory)
      :                 BPSK-OFDM, QPSK-OFDM
00"            16-QAM-OFDM, 64—QAM-OFDM
오류정정 부호               K=7 (64 states) 컨볼루션 부호
 Se            1/2, 2/3, 3/4
총 부반송파 수           |       52
OFDM 심볼 주기                   |         4,0 ps
보호구간                     | . 08602
대역폭                       |         20 MHz

표 15.1에 나타난 바와 같이 IEEE 802.118에서는 총 52742] 부반송파(4개의 wpelel 부
반송파 포함)를 사용하여 6, 9, 12, 18, 24, 36, 48, 54 Mbps2] 가변 전송률을 제공하며,

519


===== PAGE 516 =====
PART IV_MIMO-OFDM 통신 시스템

a

이를 위해 BPSK, QPSK, 16-QAM, 64-QAM2] 다양한 변조방식과 BSL 12, 2/3,
3/49] 컨볼루션 부호를 사용한다. 또한 옥내환경에서의 다중경로 지연을 고려하여 보호구
간을 08s 2 하고 이때의 심볼 주기를 4.0/6로 하며 20 MHz] 대역폭을 사용한다.

00 IEEE 0602.11 규격 및 기본 블록

그림 15.12 IEEE 802.113 무선 Boo] BEES 나타내며, 표 15.2% 8가지 AS Hol]
따른 IEEE 802.118의 파라미터를 보여준다. 이 그림에 나타난 바와 같이 송신단에서 입력
된 데이터는 스크램블링되고 컨볼루션 부호기와 인터리버를 거쳐서 부반송파로 변조되는
데, 이 때 전송률에 따라서 각기 다른 BSS, 인터리빙 7 Nopps) 및 변조방식을 갖게
된다. 이러한 전송률에 따른 파라미터는 표 15.2에 주어져 있다. 그 후, 4개의 wale 톤이
데이터 부반송파에 더해져서 총 52개의 부반송파에 신호가 전송되며 12개의 가상 부반송
파가 더해져서 64 IFFTo]] 입력된다. IFFTS 통과한 시간영역 신호에 CP(Cyclic Prefix)7}
더해져서 하나의 OFDM 심볼이 형성되며, 여기에 윈도우를 취하여 전송하게 된다.

Convolutional                        Modulator               a
Scrambler} —>} Encoder         hee        Spe QPSK        Add Hd         Pe        ett ho    Ou
(1/2, 2/3, 3/4)                       Sosy          1   )

=   ener              |    |
scartier | decoder [| emer 00000 05    acer!    (64009
ㆍ -    <

그림 15.1 IEEE 802.113 무선 oolo|) 블록도

표 15.2 IEEE 802.118 전송률에 따른 파라미터

ee  ee

6               BPSK             1/2                       1

8               BPSK             3/4                       ll                             48                            36
12              QPSK             1/2                       2                             96                            48
18              QPSK             3/4                      3                             96                            72
24           16-—QAM           1/2                       4                            192                           96
36           16—QAM          3/4                      4                            192                          144
48           64-QAM          278                      6                            288                          192
54           64-—QAM          3/4                      6                            288                          216

520

ㅣ 002


===== PAGE 517 =====
제15장_166ㄷ 802.11a/n

수신단에서는 송신단의 역과정이 일어나며 동기화 과정이 추가된다. 먼저 정해진 훈련

3
ABS 사용하여 심볼 타이밍 옵셋, 반송파 주파수 옵셋, 채널을 추정하는 과정이 선행된
후 데이터가 FFTS 통과하여 48개의 부반송파에 신호가 출력된다. 이 신호는 등화기를
통과하여 채널 응답이 보상된 후 비트열로 변환되어 비터비 복호기와 디스크랩블러를 거

쳐서 최종 데이터로 출력된다. 다음은 위 기본 SS] 각 부에 대하여 설명한다.

(1) 스크램블러

IEEE 802.118에서는 스크램블러로 길이 127인 프레임 동기화된 스크램블러를 사용하
며 그림 15.2는 이러한 스크램블러를 보여준다.

Data in

| KOC ey '

(De-)Scrambier
data out

그림 15.2 데이터 스크램블러

(DL)

송신단에서 스크램블러는 전송시에 가상 랜덤 non-zero 상태로 초기화되고 127-비트
단위의 반복적인 스크램블링 AAMAS 생성하여 입력 데이터와 %0 한 뒤, 데이터를 출
력하게 된다. 송신 데이터의 스크램블링과 수신 데이터의 디스크램블링에는 같은 스크램
블러가 사용되기 때문에 송신단에서 스크램블링되는 처음 7 비트를 스크램블링되기 전에
0으로 초기화해서 수신단에서 스크랩블러의 초기 AHS 추정할 수 있도록 한다.

(2) 컨볼루션 부호기
오류정정 부호기로는 그림 15.3과 같이 구속장이 7이고 생성 다항식(133,171)을 갖는
BSL 1/2의 컨볼루션 부호기가 사용된다.

0                       Output data A
Input data           【           T           T           af           T           1
a                  Output data B

그림 153 컨볼루션 부호기

521


===== PAGE 518 =====
PART IV_MIMO-OFDM 통신 시스템

이러한 1/29] 기본 부호을 외에도 전송률에 따라서 2/39} 3/4의 부호을이 사용되기 때
에, 1/2보다 더 높은 부호율을 얻기 위해서는 “040004008`을 사용한다. ‘puncturing’
신단에서 부호화된 비트의 일부분을 규칙적으로 생략하여 전송함으로써 전송되는 비
를 줄이고 부호율을 높이는 것을 말하며, 그림 15.4는 부호율이 2/3, 3/4일 때의 puncturing
패턴을 보여준다.

이 그림에 나타난 바와 같이 1/2에서 23H 부호율을 높이기 위해서는 부호기에서 출력
되는 비트열에서 4비트마다 1비트씩을 생략해 주면 되고, 3/4으로 부호율을 높이기 위해서
는 6비트마다 2비트씩을 생략해 주면 된다. 이렇게 생략된 비트는 수신단에서 임의의 비트
로 채워지고 복호시에 같은 MNES (metric) 값, 일반적으로 OS 할당하여 복호함으로써 부
호율이 1/22) 하나의 비터비 복호기로 부호율이 2/3, 3/4인 경우의 HSE 가능하게 된다.

u
Ae
A
Oo

sen
ㄴㄴ
트

+

siurce data | x0 | x1 | Xe | Xe | X- | Xs |  | Xo | Xi | Xe | Xs | Xe | Xs |

Vv   mig

AofAr| Ac] As| Ae| As} [| Ao| Ar] Ae] As| Ar As| | | Stolen sit
encoder data
Bo | Bi | Be | Bs | By | Bs   Bo | By | Be | Bs | 84 | Bs
V7           V7
|        [Ao [8 [As [ac [Be [As [Ae | s] Ao [@> [as [Be [As [Be [ae] as |
mes            vy    transmitted/received    a7
bit inserted data 세 01 BSE OA Bar hd   fovea * | 0  |   ay i
Bo | B: | Be | Bs | Ba | Bs   Bo | 81 | Be | Bs | Ba | Bs
V7           V7
decoded data [Yo] Yi] Yo] Ya] Y«] Ys] [Yo] ¥: | Yo | Yo | Y« | ¥s |
Rate 2/3                   Rate 3/4

그림 15.4 Puncturing 패턴

(3) 인터리빙

인터리버로는 블록 크기가 한 OFDM 심볼에 실리는 부호화된 비트 수, 즉 Noss 인 블록
인터리버가 사용된다. 따라서 인터리버의 크기는 전송률에 따라 최소 48비트에서 최대 288
비트까지의 범위를 갖게 된다. 인터리빙은 두 단계에 걸쳐서 이루어지는데 A 단계는 인접
하는 비트가 서로 인접하지 않는 부반송파에 실리도록 하기 위하여 다음 과정을 거친다.

522



===== PAGE 519 =====
제15장1666 802.113/ㅁ

i=(Nepps /16)X(k mod 16) + floor(k/16)     K=O loses Nps 그         (15.1)

위 식은 인터리빙되기 전의 비트열의 순서가 *로 표시될 때 인터리빙 후의 비트열은 7

의 순서를 갖도록 인터리빙되는 것을 나타내며, Moor() 함수는 파라미터를 초과하지 않

는 최대 정수를 의: |한다. 두 번째 단계는 데이터|심볼 맵핑 성상도에서의 비트 위치를 바
꾸어 주는 역할을 하며 이는 다음 식과 같이 정의된다.

J =8X floor(i/s)+ (i+ Negps - 7//007/7(16×7/ Nepps)) mods    00092 —1 (15:2)

여기서 8 = max(Nppge /251) 이고, Norse 는 하나의 부반송파에 실리는 비트 수를 나타낸
다. 첫 번째 인터리빙 후 1의 순서를 갖는 비트열은 두 번째 인터리빙 후 최종적으로 /

7

©

의 순서를 갖는 비트열이 된다.
역인터리빙은 인터리빙의 역과정이며 인터리빙과 마찬가지로 다음의 두 식에 의해서
정의되는 두 단계로 이루어진다.
i=sx floor(j/s)+(j+ floor(16/ Nepps))mod s      i=0,1,....N cpp —1      (15.3)

k =16X1—(Nepps —1)x floor(16Xi/ Negps mods  1= Oly N Gepy 1   (15.4)

여기서 식 (15.3)은 식 (15.2)의 역과정을 수행하고, 식 (15.4)는 식 (15.1)의 역과정을 수

(4) 데이터 심볼 변조

부호화되고 인터리빙된 데이터는 전송률에 따라서 BPSK, QPSK, 16—QAM, 64—QAM
으로 변조된다. 입력 데이터는 먼저 하나의 부반송파에 실리는 비트 수(^,,ㅠ) 그룹으로
나뉘어지고, BPSK, QPSK, 16—-QAM 또는 64-QAM 성상도의 심볼을 나타내는 복소수
로 변환된다. 이렇게 변환된 복소수 값에는 정규화 값 Kaos 가 곱해지는데 정규화는 모든
변조방식에서 같은 평균 전력을 갖도록 하기 위해 필요하다. 변조방식에 따른 정규화 값
Kod 는 ar 15.33} 같다.

523


===== PAGE 520 =====
PART IV_MIMO-OFDM 통신 시스템

a

BPSK                                         1

QPSK                      1/2
16-QAM                    1/10
64—QAM                    1/J42

(5) Ia 심볼 삽입

각 OFDM 심볼에는 4개의 부반송파가 잔류 위상 옵셋을 보상하기 위하여 wpelel 부반
송파로 할당된다. wees 심볼이 실리는 gelel 부반송파는 그림 15.5와 같이 -26~26까
지의 전체 10608메버 -21, -7, 7, 21번째 부반송파이며, 이러한 -21, -7, 7, 21번
째 부반송파로 전송되는 welel 심볼은 다음과 같이 정의된다.

[=]  는

4 pilot subcarriers

if                                    \
i                                    \
fi
                       20 MHz
그림 15.5 meet 심볼 삽입

4개의 sel ASL 가상 이진 ALAA 에 의해 BPSK 변조되어 실리게 되는데, F
ABAE 127개의 BAS 순환 확장한 것으로 다음과 같이 주어진다.

2 0=(1.1.1.1=1=1=1.1=1.1.91.21.1.1,.1.1401.91.1.1=1.1.1.=1.1.1.1.1.1.1.131.1,
1,-1,1,1,-1,-1,1,1,1,-1,1,-1,-1,-1,1,-1,1,-1,-1,1,-1,-1,1,1,1,1,1,-1,-1,1,1,-1

-1,1,-1,1,-1,1,1,-1,-1,-1,1,1,-1,-1,-1,-1,1,-1,-1,1,-1,1,1,1,1,-1,1,-1,1,-1,1-1,
-1,-1,-1,-1,1,-1,1,1,-1,1,-1,1,1,1,-1,-1,1,-1,-1,-1,1,1,1,-1,-1-L-L-L-1-]}

여기서 P, 시퀸스의 각 요소는 mele 심볼에 순차적으로 적용된다. P, 시퀸스는
크램블링 시퀸스와 같은 방법으로 생성될 수 있으며 스크램블러의 초기 상태를 모두 '1'
로 하고 이 때 얻어지는 127개의 요소에서 VS VB, OS ‘VE 바꾸어주면 얻을
스
수 했다.

[>

ss

524



===== PAGE 521 =====
제15장_16ㄷ6ㄷ 802.11a/n

(6) OFDM 변조
표 15.4% IEEE 802.1la 물리계층의 OFDM 심볼 파라미터를 보여준다.

표 15.4 IEEE 802.118의 OFDM 심볼 파라미터

2: 데이터 부반송파 수
수

Ns             “                       48

No: HORA 부반송파                     4

No: 총 부반송파 수                      822 (NG NG)
Af: 부반송파간 간격                      0.3125 MHz (20 MHz/64)
1727: IFFT/FFT 주기                  Le 32 6 (AP)
1209“: PLCP 프리앰블 주기          [eG BE. Tg + Tag)
15904 > SIGNAL 심볼 주기                 4.0 us (To, +T rer)
To: 보호구간 주기                  2 0.8 gs (| /4)
Tog? 훈련심봄 보호구간 주기         | Sah gee (TD)
150:  심볼 주기    4 Ms (To, + T rer)
100: 짧은 훈련심볼 주기                    8 pus (1075 / 4)
Tiong: 4) Sage 주기                      8 os (Tey. + Trp)

하나의 데이터 OFDM 심볼은 48개의 데이터 부반송파와 4개의 Beal 부반송파를 더

총 52개의 부반송파로 구성되고, T,, =4/48 의 심볼 주기로 전송된다. 심볼 주기 7,
보호구간 7., = 0.8/ 와 IFFT/FFT 주기 7; , =3.2us 를 더한 값이며, 이 때의 부채
널간의 간격은 Af(1/Typp) =0.3125MHz 가 되고 전송 대역폭 (64×4ㅅ47) 은 20MHz 7}
된다. 표 15.4에는 데이터 OFDM 심볼외에도 동기화를 위한 훈련심볼이 정의되어 있으며
이에 대한 자세한 ABS 15.1.3절에서 이루어진다.

데이터 심볼 변조된 48개의 데이터는 부반송파에 각각 실리게 되는데 OFDM 심볼의
-26~26번째 부반송파중에서 부반송파로의 맵핑 함수 74()는 다음과 같다.

하
한

은
ㄴㄴ

k-26,0<k<4
k-25,5Sk £17
k-24,18<k<23
M(k)=3                            (15.5)
k-23,24<k<29
k-22,30<Sk<42

k-21,43<5k<47

525


===== PAGE 522 =====
PART IV_MIMO—OFDM 통신 시스템

여기서 0번째 부반송파와 -21, -7, 7, 21번째 부반송파는 DC 부반송파와 wpelyl 부반
송파이므로 이 부분을 제외한 나머지 부반송파에 48개의 데이터가 차례로 WYSE 것을
알 수 있다. abelel 부반송파에 spelel 심볼이 삽입된 뒤 총 52개의 부반송파가 41로
입력되며, 64-포인트 IFFTS 거쳐 OFDM 심볼이 형성된다. 부반송파와 IFT 입력사이
의 맵핑관계는 그림 15.6에 주어져 있다.

Null            0                   cea
+1 —                   a
#2 —i             —
ㆍ  | ㆍ                    ^
ㆍ           ㆍ                    _ :ㅅ『32뻐
#26 -ㅡ126    IFFT    …-
null          27                 27           time domain outputs
null           ㆍ                    —
null          37                 37
#-26 ——38                  381--
e           e                    meee!
oe ——e                    ＊‥-
#-2-ㅡ~                    _
#1 —163             63--

그림 15.6 IFFT 블록도

위 그림에서와 같이 1~26번째 OFDM 부반송파는 에서 1~26번째 입력이 되고
-26~-1번째 부반송파는 IFFTS] 38~63번째 입력이 된다. 나머지 27~37번째 입력과 0
번째 입력(00)은 0이 되며 이러한 가상 반송파는 채널간 간섭을 방지하기 위해 사용된다.
IFFT 후에는 심볼간 간섭을 방지하기 위해 보호구간을 삽입하며 이러한 보호구간으로는
16개의 샘플로 이루어진 CP(Cyclic Prefix)S 사용한다.

(7) 심볼 파형 성형

IFFTO] 의해 발생된 OFDM ABS 시간영역 윈도우에 의해 파형 성형된 후 송신된다.
그림 15.7은 윈도우가 곱해진 시간영역 OFDM ABS 보여준다.

T=TertT rer

T=T 612+ 2T per

Tovarp

Tovaro
=T6121

Trer

Trer

1                                           '
Tre                                              Tre

Training Sequence

그림 15,7 시간영역 OFDM 심볼

시간영역 윈도우의 주기 TE 데이터 OFDM 심볼의 주기 Tn 같으며, 특별히 초기

동기화를 위한 훈련심볼에는 그 두 배의 길이를 갖는 윈도우가 사용된다. 이 그림에서 알


===== PAGE 523 =====
제15장_!ㄷㄷㄷ 802.113/ㅁ

\

수 있듯이 윈도우를 적용함으로써 연속되는 심볼간에 유연한 천이가 일어나도록 할 수 있

^
는데 이 때의 윈도우 wy 다음 식과 같이 정의된다.
sin? | (0.5+1/T)} , +0, 7302.72
w(t) =     1.0    , 이 fiee<T 7/2      (15.6)
sin’ 2 (05- (-1)/T)} T=T,/Isrer +712

이렇게 천이시간 Tre

을 두어서 유연한 천이가 일어나도록 하면 전송 신호의 대역외 스
펙트럼의 크기를 감소시킬 수 있다. Try =100ns 을 갖는 윈도우는 실제 설계에서 다음 식

과 같은 이산화된 시간영역 윈도우 101으로 나타낼 수 있다.

a

1 , l<ns<79
w[n]=40.5, 0,80                    (15.7)
0 , otherwise
tyes, IEEE 802.lla 성능 분석
본 절에서는 전 절에서 설명한 IEEE 802.11a 무선 2°] BER 성능을 분석한다. 모의
실험에서는 OFDM 심볼 동기 및

베바 주파수 동기는 올바르게 이루어졌고. 등와기 Al
수 Me 오차없이 추정되었다고 가정하였다. 수신단에서는 단일탭 등화기와 truncation
200의 길이가 35인 경판정 비터비 복호기를 사용하였다.
그림 15.8은 AWGN 환경에서 BPSK/QPSK, 16-QAM, 64-QAM 변조방스
인 BER 성등과 모의실험 결과를 비교하여 보여준다.
그림 15.8에서 8289/0ㅁ9과 M—QAM 변조방식의 해석적인 BER 성능은 다음 식으
로 주어진더|1].

527



===== PAGE 524 =====
PART IV_MIMO-OFDM 통신 시스템

그림 15.8에서 64개의 부반송파에 데이터가 모두 Ale] OFDM 방식의 4-2(BPSK-
OFDM, QPSK-OFDM, 41-04-00240)에는 위의 단일 반송파(809/089, M—
QAM) 경우의 해석적인 BER 성능과 동일한 성능을 보임을 확인할 수 있다. 그러나 IEEE
802.118에서와 같이 총 52개의 부반송파에만 데이터가 실리는 경우에는 식 (4.37)에 나타
난 바와 같이 BER 성능이 향상되는 효과를 가져온다. 그림 15.9는 ABSA 부호화에 의

한 성능 향상을 보여준다.

1E+0                                                    1E+0

Using 52 Subcarreirs
-@- BPSK/QPSK
-6- 16-QAM

1-1 Sook  a 는00-----구기 fe BARQAM
             :      | | BPSK/OFOM
3 QPSK-OFOM
8+ 16-QAV-OFDM
162                      -%- 64-QAM-OFDM
잠바
고       {      {       {      {               =       d      {
606     4     8    12    16    20      = 8     4     8    12    16    20
Eb/No[dB]                                    Eb/No[dB]
(a) 64 부반송파를 사용한 경우                 (6) 52 부반송파를 사용한 경우

그림 15.8 변조방식에 C= IEEE 802.113의 BER 성능

4     8     12     16     20         0     4     8     12     16     20

Eb/No[dB]                                    Eb/No[dB]
(a) BPSK/QPSK                      (b) 16-QAM/64—QAM
그림 15.9 컨볼루션 부호화에 의한 성능 향상

528



===== PAGE 525 =====
제15장_ 1666 802.11a/n

IEEE 802.118에서 컨볼루션 부호가 사용되는 경우의 BER ASS 컨볼루션 부호가 없
는 경우보다 10 “의 88&에서 부호율이 1/2인 경우는 약 3 08, 2/3인 경우는 약 2.5 08,
3/4인 경우는 약 1.5 08 향상됩을 알 수 있다.

그림 15.10은 AWGN 환경에서 IEEE 802.118 무선 eo} 8가지 전송률에 따른 BER
성능 곡선을 나타낸다. BPSK} QPSK 변조방식의 BER 성능은 동일하기 때문에 BSS
1/22] 오류정정 부호를 사용한 6 Mbps} 12 \4608의 성능이 거의 유사하게 나타나고, 이
와 비슷하게 3/4의 부호율을 사용한 9 \4605와 18 Mbps©] 성능도 거의 같게 나타난다.
전체적으로 전송률이 높아질수록 성능이 감소하는 경향을 보이나 예외적으로 12 14608의
성능이 9 14608보다 더 우수하게 나타나는 이유는 같은 성능의 변조방식이 사용되므로
Mbps} 오류정정 능력이 더

NS)
atc)
4a
에
ㅇ
9
거부
clr
Ss)
2
n
N
aS
me
~
je,
4r
|에
ㅇ
ie
>부
rir
vo f

우수하기 때문이다.

jet | 쑥 그
5 1-3 }-—--
| nn 2 Oe eee | aeons ae aa

1E-6           &

0        4                 12        16

8
Eb/No[d8]
그림 15.10 AWGN 환경에서 IEEE 802. 11a FA Golo) 성능 비교

그림 15.112 옥내환경에서의 IEEE 802.118 무선 Heo] 성능을 비교하여 보여준다.
옥내환경 BAS 2.2.3절에서 설명한 클러스터 평균 도착 시간(1/ㅅ), ray 평균 도착 시간
C/A), 클러스터 전력 감쇄 ABA), ry 전력 감쇄 시정수(7) SS 토대로 모델링하
는 S-V 모델을 사용하였다[37]. 모의실험에 사용된 50152대 무선 채널은 평균 지연 확산
이 SOns[rms]°]31, 이 때의 채널 파라미터는 1/A=356ns, 1/A=60ns, 1=506, Y=
20208이다.

529



===== PAGE 526 =====
PART IV_MIMO-—OFDM 통신 시스템

1E+0

| ChanneltAWGN

|} Packet =1000bytes
| ~~ 6M bps
| 8+ 9M bps
{   | -@-12460066
c=] Ae 18M bps
1] —* 24M bps
| —O- 36 Mbps
| A= 48 Mbps
| -O= 54M bps

1-1 f----&

WW 1E-3}-- 고놈 가골조 ----- wen  ree     WIE 2

1E-3

8             0 68 10 12 14 16 18 20 2 240 2
Eb/No[d8]                 Eb/No[d8]
(a)                  (b)

그림 15.11 옥내환경에서 IEEE 802.118 무선 Goo) 성능

그림 15.11(a)= AWGN 환경에서와 마찬가지로 6 MbpsSt 12 Mbps°} 성능이 유사하
al, 9 Mbps2} 18 Mbps°] 성능이 유사하며, 전체적으로도 전송률이 증가할수록 성능이
감소함을 알 수 있다. 여기서 옥내환경인 경우에는 AWGN 환경에서와 달리 24 Mbps?
성능이 9 Mbpst} 18 54608와 거의 유사하게 나타나는데, 이는 연집 오류가 발생하기 쉬
운 주파수 선택적 채널인 옥내환경에서는 오류 정정 능력과 인터리버의 크기가 성능에 더
크게 작용하기 때문이다. 그림 15.11(6)는 옥내환경에서 IEEE 802.118 무선 walo] 패킷
오류율(08060 Error Rate; PER) 성능을 보여준다. 옥내 환경에서 8가지 전송률에 따른
PER 성능을 살펴보기 위해서 하나의 패킷은 1,000 바이트로 구성하였다. 각 전송률에 따

= PER 성능 특성은 위의 BER 성능 특성과 유사함을 확인할 수 있으며, 옥내 환경에서
무선 채널을 통한 전송 시에 1%의 PERS 만족하기 위해서는 최소 전송률 6 54668에서

그림 15.12는 IEEE 802.1la PLCP 프리앰블, PLCP 헤더, PSDU, Tail 비트, Pad 비트
로 구성된 IEEE 802.11a2] PPDU 프레임 2WS 보여준다.

 530



===== PAGE 527 =====
제15장_16ㄷ6ㄷ 802.11a/n

PLCP Header

RATE |Reserved| LENGTH | Parity| Tail | 6
4 bits roe 12bit | 1 bit |6 bits)

ea Goded/OFOM |    _Coded/OFOM
“> (BPSK, 1/2) |  (RATE is in dicated in SIGNAL)

Preamble             SIGNAL
12 symbols | one OFDM symbol

그림 15.12 IEEE 802.11a 무선 Sao] PPDU 프레임 HoH

PLCP dt] RATE, Reserved 비트, LENGTH, 짝수 Wee} 비트, Tail 비트,
SERVICE 필드로 구성되는데, 이 중 RATE, Reserved 비트, LENGTH, 짝수 패러티 4]
트, Tail 비트는 SIGNALZ 정의된 별도의 1 OFDM 심볼로 구성되어 가장 안정적인
BPSK 변조와 1/2 부호화를 거쳐 전송된다. PLCP 헤더의 SERVICE, PSDU, Tail 비트,
Pad 비트는 DATA 필드로 정의되고, DATA YEE RATES 정의된 전송률로 전송되며
OFDM 심볼들로 구성된다.

(1) PLCP 프리앰블

PLCP 프리앰블은 동기화를 위해 사용되며 OFDM 패킷의 앞부분에 전송된다. 그림
15.13은 IEEE 802.118에서 사용되는 2 프리앰블을 보여준다.

8+8= 16us
10x 0.8 = 848     |, 2x08x2x3.2= 848 1 0.8+3.2= 4451 0.8+3.2 = 4u8 10.8+3.2 = dys
비틱비비티티미빅복비 Ge  Ty   Te  ic
Signal detect,            Coarse Fi            Channel and fine freq               E
com         |          Offset estimation _ offset estimation                LENGTH         SERVICE+DATA 0814
Diversity selection          Timiming synchronize

그림 15.13 IEEE 802.11a 무선 Soo) PLCP 프리앰블

PLCP 프리앰블은  ~1《;으로 이루어진 10개의 짧은 훈련심볼과 7; 과 7; 로 이루어진
2개의 긴 훈련심볼로 구성된다. 전체 주기는 16//8 이며, 그림에서 점선으로 표시된 경계선
은 IFFT] 주기성에 의해 반복되는 것을 의미한다. 짧은 훈련심볼은 수신단에서 AGC, 다
이버시티 선택, 타이밍 동기화, 대략적인(60806) 주파수 동기화를 하는 데 사용되고 다음
과 같이 주파수영역에서 12개의 위상 변조된 부반송파로 구성된다.

531



===== PAGE 528 =====
PART IV_MIMO-OFDM 통신 시스템

5. = V(13/6) x {0,0,1+j,0,0,0,-1-j,0,0,0,1+j,0,0,0,-1-j,0,0,0,-1-j,0,0,0,1+j,0,0,  (15.10)
여기서 (13/6) 은 52개의 부반송파중에 12개의 부반송파만을 사용하는 OFDM 심볼의
평균전력을 정규화하기 위해 곱해진다. 짧은 훈련심볼은 주파수 영역에서 4배수에 해당되
반송파에만 OO] 아닌 신호가 실려 있기 때문에 FFT 주기의 1/40] 해당하는 0.8/68 의
기를 가지며, 10번 반복되는 짧은 훈련심볼의 총 주기는 8//5가 된다. 긴 훈련심볼은 A
널 추정과 Ul (fine) 주파수 동기화를 위해 사용되며 다음과 같이 주파수영역에서 53개
(DC2] 0을 BWI 위상 변조된 부반송파로 구성된다.

4Norir oft
4r

¢

때

696 = t 1,1,-1,-1,1,1,-1,1,-1,1,1,1,1,1,1,-1,-1,1,1,-1,1,-1,1,1, 1,1,0,       i
1,-1,-1,1,1,-1,1,-1,1,-1,-1,-1,-1,-1,1,1,-1,-1,1,-1,1,-1,1,1,1,1)   ae

긴 훈련심봄의 주기는 FFT 주기와 같은 3.2150] 0), 2번 반복되고 3.2us 9] 보호구간이
cial 총 86 가 된다, 2 Bele 보호구간은 de 8 OFDM na 보호구간의 두

(2) SIGNAL 필드

PLCP 프리앰블 다음에는 SIGNAL 필드가 전송된다. SIGNAL BEE DATA 필드에
A 사용될 전송률과 전송될 패킷의 길이에 대한 정보를 담고 있다. SIGNAL 필드는 24
비트로 구성되는데, 순서대로 비트 0~3은 RATE, 비트 4® Reserved, 비트 5~16은
LENGTH, 비트 17은 짝수 패러티, 비트 18~23은 Tail 비트로 각각 할당된다. 이 중
RATE 필드에는 DATA BEA 전송률에 따라 사용될 변조방식과 부호윤에 대한 정보
가 부호화되고, LENGTH 필드에는 MACI} 물리계층 사이에 전송되는 octet 수가 부호화
되어 전송될 패킷의 길이를 예측할 수 있다. 또한 짝수 패러티 비트는 0~16까지의 비트
에 대한 패러티 비트이며, Tail 비트는 Tail 비트의 수신 후에 즉시 RATES} LENGTH 필
ES 복조할 수 있도록 하기 위해 삽입되고 0으로 채워진다. SIGNAL 필드는 데이터
OFDM 심볼과 비슷하게 PES 1/2인 컨볼루션 부호화, 인터리빙, BPSK 변조, wale
삽입, OFDM 변조를 거쳐서 하나의 OFDM AS 형성하며 가장 낮은 전송률인 6 Mbps
로 전송된다. 이 때 SIGNAL 필드는 스크램블링되지 않는다.



===== PAGE 529 =====
제15장_!6ㄷ6ㄷ 802.11a/n

(3) DATA 필드
SIGNAL 필드 Oo] So] SIGNAL 필드에서 정의된 전송률과 길이를    eee DATA 필드
가 전송된다. DATA BE Service YE, PSDU, Tail 비트, Pad 비트로 구성되는데 이

tN

중 Service HEE 모두 0값을 갖는 16비트로 구성되며 AS THEE 디스크랩블러를
기화하기 위해 사용되고 나머지 9비트는 &6560060 비트로 사용된다. DATA 필드는 다수
의 OFDM 심볼로 구성되어야 하기 때문에 DATA 필드내의 비트 수는 하나의 OFDM 심
볼에 실리는 데이터 비트 (Noses )의 배수가 되도록 확장되어야 하고, 이를 위해 PSDU
다음에 Tail 비트 6개를 포함한 일정한 수의 비트가 추가된다. PPDU Tail 비트는 컨볼루
션 부호기를 0 FAS 되돌리기 위해 사용되며 6개의 “0' 비트로 이루어진다. DATA 필
드 내의 모든 비트는 스크램블링되기 때문에 28100 다음의 6개의 스크램블링된 비트를 0
으로 바꾸어줌으로써 Tail YES 형성할 수 있다. 이러한 Tail 비트의 추가는 컨볼루션
복호기의 오류 SHS 향상시킬 수 있다. Tail 비트외에 추가되는 비트는 Pad 비트로 정의
되며 추가되는 Pad 비트의 4 SIGNAL 필드의 LENGTH 필드에 정의된 PSDUS] 길이
로부터 계산될 수 있다. 이 때의 OFDM 심볼 4 Nom), DATA 필드의 비트 수(^),
Pad 비트 수(^,,,)의 관계는 다음과 같이 주어진다.

Nm = Ceiling((16+8x LENGTH + 6)/ 2.)                   (15.12)
Noara = Nova * Noppps                              (15.13)
Noan = Nopary ~16+8X LENGTH + 6)                     (15.14)

여기서 Ceiling() 함수는 파라미터보다 같거나 큰 최소 정수를 의미한다. PAD 비트
‘QO 채워지며 DATA 필드의 나머지 비트와 함께 스크램블링된다.

bees IEEE 802.lla 동기부
일반적으로 버스트 BAS] 수신단에ㅅ             용하여 데이터 전송 이전에 초
기 동기화를 이루게 되며, 이러한 초기 동기는     Ae (burs) 17 데이터를 전송하는 시스
템의 성능에 크게 영향을 미치게 된다. 본 절에서는 888 802.113 무선 Bayo} 초기 동기
화 방법을 설명하고 그 성능을 분석한다.

Le



===== PAGE 530 =====
PART IV_MIMO—-OFDM 통신 시스템

(1) IEEE 802.118 프리앰블
그림 15.14는 IEEE 802.118의 프리앰블 구조를 보여준다.

16                                                                                           32                      64                                64
< >                                                                         <— >

<                              ><           ><
<                      <        es

+

Signal detect               Coarse Freq.            Channel and fine greg
AGC                      offset estimation         offset estimation
Diversity selection           Timing synchonization

그림 15.14 IEEE 802.113 프리앰블 구조

프리앰블에는 주기가 각각 16, 64 샘플인 두 종류의 훈련심볼이 정의되어 있는데, aH
터 까지는 주기가 16 샘플인 짧은 훈련심볼을, Tap He 주기가 64 샘플인 긴 훈련심볼
을 각각 나타낸다. 한 ASS] 주기는 5008이므로 프리앰블 전체는 lous 길이를 갖는다.
IEEE 802.1la 규격에서는 그림 15.14와 같이 /1~7 구간을 신호검출, AGC (Automatic
Gain Control), 다이버시티 AAS 위해 할당하였고, 6 ~710 구간에서 대략적인(608796) Yt
송파 주파수 옵셋과 심볼 타이밍 옵셋 추정을, 7, TELA 미세(006) 반송파 주파수 옵
Ala} 채널 추정을 수행하도록 프리앰블을 할당해 놓고 있다. IEEE 802.118에서 사용하는
짧은 SAMA ~/()과 긴 훈련심볼(7, 7:)의 상관함수의 주파수영역 및 시간영역 특성
이 각각 그림 15.15와 그림 15.16에 주어져 있다.

10  T T T T T T T   1.0
08            1 08
3             8
『              를
i=             [=
을 06            | Zo6
E             E
Bu            | Eos
=             =
“O 8 16 24 3% 4 4% 5 64 “0 8 16 4 3 4 4 5 6 "0 8 16 2 3% © #8 5 64
Frequency            Frequency
(a) 주파수 영역             06) 시간영역           (0) 신호의 크기특성
그림 15.15 짧은 훈련심볼의 상관함수 특성
534


===== PAGE 531 =====
제15장_16ㄷㄷㄷ 802.113/ㅁ

=
=
『
°
o

1 08

은
&

0.12

은
i

°
Es
Normalized Magnitude

Normalized Magnitude

은
bo

은
ho

8 16 24 32 40 48 56 64
Frequency

은
S
co)
은
으
은
=
~

8 16 24 2 4 4 56 64 “0 8 16 20 32 4 48 56 64
Frequency    Frequency

(a) 주파수 영역 ㆍ           06) 시간영역            (0) ASS] 크기특성

(2) 반송파 주파수 옵셋 동기부

IEEE 802.118에서는 훈련심볼을 사용하여 반송파 주파수 옵셋을 추정할 수 있다. 수
된 두 반복 신호의 자기상관함수를 이용한 Moose 방식이 at 5.4.1절에서 설명한
시간영역 추정기법 또는 5.4.2절의 주파수영역 추정기법을 적용하여 추정할 수 있다
[107][111]-[113]. 이 경우 수신신호의 자기상관을 이용하기 he 타이밍 옵셋과 다중
경로 채널이 존재하는 경우에도 영향을 받지 않고 반송파 주파수 옵셋을 추정할 수 있다.

훈련심볼의 반복 주기가 DE 주어질 경우에 수신된 시간영역 신호 y[n] St yn + D] Aho]

에는 반송파 주파수 옵셋에 의해 각각 eM MMP" 만큼의 위상변화가 발생한다.
이 경우 두 신호의 위상 차이와 반송파 주파수 옵셋의 추정 범위는 다음과 같이 주어진다.

22n€(n+D)/N-Z2nen/N =2280727            (15.15)

|2eD/N| <a                            (15.16)

그림 15.172 짧은 훈련심볼과 긴 훈련심볼의 반송파 주파수 옵셋 추정 성능을 보여

준다.

그림 15.17(8)로부터 반복되는 훈련심볼을 사용하여 주파수 추정을 할 경우 주파수영역
기법과 시간영역 기법은 동일한 수의 HSS 사용하는 한 동일한 ASS 갖게 됨을 알 수
있다. 긴 훈련심볼을 사용할 경우에 짧은 훈련심볼에 비하여 샘플 수가 4배 많기 때문에
성능이 우수함을 알 수 있다. 그림 15.18은 짧은 훈련심볼과 긴 훈련심볼을 사용하여 반송
파 주파수 옵셋을 추정할 경우 추정 범위와 정확도를 보여준다.

535



===== PAGE 532 =====
PART IV_MIMO—-OFDM 통신 시스템

CFO Estimation                                                                                    ] CFO Estimation
—8- Coarse, Time                                                                                               | —A—STO
162                           —A- Coarse, Freq.                                        | —@—NosTo
—- fine, Time                             1&2                                                            —+— Channel
-※%- fine, Freq                                                                                                    —£}— No Channel
1E-3
w
a
=
1E-4
1E-5
-                                                                                                                166                                            :
IE 79       5      10      15      20      25      30                 0       5      10      15      20      25      30
SNR

SNR

(a) 시간영역과 주파수영역 비교

(6) 타이밍 옵셋과 채널의 영향

그림 15.17 반송파 주파수 옵셋 추정 성능

1타2

1타1

1타0|

1&1

1E-3

1E-4

165

~ CFO Estimation Range
—5— Short training signal(16 samples)
—+— Long training signal(64 samples)

1E-6

25 -2.0 -15 -10 -05 00 05 10 15
Carrier Frequency Offset

2:0 25

그림 15.18 반송파 주파수 옵셋의 추정 범위와 정확도

짧은 훈련심볼을 사용할

경우에 N=64, /2=16 이므로 1 FFT 주기에 신호가 4번 반

하게 되어 추정할 수 있는 주파수 옵셋 범위가 부반송파 간격의 4배가 되며(| <2), 긴

복

훈련심볼을 사용할 경우 N
수 Ue lel <0.

볼을 이

주파수 추정을 하게 된다

(3) 채널 추정부

536

=D =64 이므로 부반송파 간격 이내의 주파수 옵셋만 추
. 따라서 IEEE 802.118에서는 추정 범위를 넓히기 위하여 짧은 훈련

>                                                        건
용하여 대략적인 주파수 추정을 한 후, 긴 훈련심볼을 이용하여 정확하고 미세한
추

a a

a |



===== PAGE 533 =====
제15장_16ㄷㄷㄷ 802. 11a/n

송신단에서 부채널 Apolo] Beal ES 삽입하여 ASS 후 이 al ES 이용하여
Leto] A] 시간영역과 주파수영역의 보간법으로 채널을 추정하는 방법을 사용한다[127].
 IEEE 802.118와 같이 HAE 데이터를 전송하는 BAS] 경우에는 데이터 전송시간
이 짧고 그 시간동안 채널이 크게 변하지 않기 때문에 전송의 초기 단계에서 훈련신호를
사용하여 채널을 추정하고 그 값을 데이터 전송시 사용하는 것이 효율적이다. 따라서
IEEE 802.118에서는 한 OFDM 심볼 길이에 해당하는 긴 훈련심볼을 전송하고 수신단에
서는 이를 이용하여 전체 부채널에서의 AAS 추정하여 Sap] Ales 구한다. 그림
15.19는 6.3.1절의 LS 채널 추정 기법을 888 802.118의 긴 훈련심볼에 적용하여 a
추정할 경우의 성능을 보여준다. 이 그림에서 TN, 7;를 함께 이용하여 채널을 추정한
TUS 이용하여 채널을 추정한 경우에 비하여 OF 2~308정도 이득을 얻을 수 있으나,

연속적으로 데이터를 전송하는 방송용과 같은 OFDM 시스템에서는 채널 추정 방법으
Al

로
7r
수
반

BER

16-4

Channel Estimation                 ee eee
16-6 | |e Hae! channel                       {
1 Using 11 (no average)          ee             :                                A
—©— Using T1, 72 (average) | ===)           i      |
8                                                20

0    4

12    16
Eb/No [dB]
그림 15.19 IEEE 802.11a2| 채널 추정 성능

(4) 잔류 위상 추적부
IEEE 802.118에서 초기 반송파 주파수 동기화 이후 잔류 반송파 주파수 옵셋은 표
15.5와 같이 주어진다.

537



===== PAGE 534 =====
PART IV_MIMO-OFDM 통신 시스템

표 15.5 IEEE 802.118에서 잔류 반송파 주파수 옵셋

Coarse              0.0517            0,0264            0.0143            0,0079            0.0045            0.0025
Fine                 0,0119             0,0064            0.0035           0.00198           0.00111          0,00062

|

표 15.5에서와 같이 2번(60086, 806/에 걸친 주파수 SAL 보상 후의 잔류 주파수 옵셋은
SNR=10 08에서 OF 0.0064로 낮아진다. 그러나 초기 동기화 후에 남아있는 이러한 작은
주파수 옵셋도 시간이 지나감에 따라 옵셋의 위상이 증가되어 BER 크게 저하시키기 때문
에 이를 방지하기 위해 패킷이 전송되는 동안에 계속적으로 위상 옵셋을 보상하는 과정이
필요하다. 다중경로 채널 및 잡음의 영향을 무시할 때 초기 동기화 후의 잔류 주파수 옵셋

에 의한 영향은 다음 식과 같이 SAAS} 위상만이 왜꼭된 형태로 근사화될 수 있다.
”[/] = ” Sil aia 4                           (15.17)
여기서 심볼 수에 관계없는 상수 ㅇ※-" 성분과는 달리 eM 성분은 수신되

는 심볼 수에 영향을 받아서 심볼 수가 증가할수록 위상 왜곡이 더욱 증가하게 된다. 이러
한 위상 왜곡이 시스템에서 변조방식에 따른 위상 오차 허용 BAS 넘어서게 되면 수신
데이터의 오류가 발생하게 되는데, 이 때 오류가 발생하기 시작하는 위상 변화량과 심볼
수는 변조방식에 따라 차이가 나게 된다. IEEE 802.11la 물리계층에 정의된 4가지 HAY
식에서 오류가 발생하기 시작하는 위상 변화량과 심볼 수는 표 15.6에 주어져 있다.

표 15.6 오류가 발생하기 시작하는 위상 변화량과 심볼 수(잔류 주파수 옵셋: 0.0064)

7/16
31            16             8             4
32            16             i             4

, BPSK, QPSK2] 경우에는 오류가 발생하기 시작하는 위상 변화량이 각각 *72와
1/4 로 주어진다. 또한 16-QAM3} 64-0444의 경우는 각 심볼 위치에 따라 변화량이
다르므로 각 심볼의 발생 빈도를 같다고 가정하고 이를 평균하면 약 */8와 7/16 7} 된
다. 예를 들어, 잔류 주파수 옵셋이 0.0064일 경우, 식 (15.17)에 의해 BPSK, QPSK,

_ 538



===== PAGE 535 =====
제15장 IEEE 802.11a/n

16-QAM, 64—-QAM 변조방식에서 데이터 오류가 발생하기 시작하는 심볼 수는 각각 31,
16, 8, 47} 된다. 표 15.6에서는 모의실험을 통하여 오류가 발생하기 시작하는 심볼 수를
표시하였는데, IEEE 802.11a 무선 14]°] 6 Mbps(BPSK), 12 Mbps(QPSK), 24 Mbps
(16—QAM), 48 Mbps(64—QAM)9]]A]_ 각각 32, 16, 7, 4 위의 식 (15.17)에 의한 결과
와 거의 유사함을 확인할 수 있다. 또한 고차의 변조방식을 사용할 수록 잔류 주파수 옵셋
에 의한 영향이 급격히 증가함을 알 수 있다. 위상 오차 허용 BIS 넘어서서 데이터 오
류가 발생하기 시작하면 시스템 성능에 심각한 영향을 미치게 된다. 이를 보상하기 위하
여 ule] ES 사용한 잔류 위상오차 추적 및 보상 기법을 사용할 수 있다.

그림 15.20은 IEEE 802.118에서 사용되는 짧은 SAAS, 긴 SAAS, Fao] 위치
를 주파수영역에서 보여준다. AIS DCS 기준으로 -21번째, -7번째, 7번째, 21번째
위치에 4개가 실리게 되고, 이 TYAS 이용하여 위상 변화값을 추적할 수 있
잔류 위상 옵셋 추적 및 보상을 위한 식을 나타낸다.

é,= =p SS ole) (i) |: *[000(6이   (15.18)

sym                   j=l

ate                                           (15.19)
8.125 MHz-
Frequency 0-7
-8.125 MHz
~ <             a     <
800ns                    4us                            Time

그림 15,20 IEEE 802.113의 훈련 AST} Ua 구조

539


===== PAGE 536 =====
PART IV_MIMO—OFDM 통신 시스템

그림 15.21은 위의 방법을 사용하여 위상
아으 겨으르

ew OTS

BER 성능을

적을 한 이후에 보상을 한 경우와 그렇지
oe 비교하여 보여준다. 잔류 위상 옵셋을 보상하지 않은 경우에

107"는                   —_
0   2   4   6   8   10  12  14      18  20
Eb/NO
212 15.21 IEEE 802.11aQ| 잔류 위상 옵셋 추적 AS 비교
. 1ｌ5.1.5 IEEE 802.lla PLCP

(1) IEEE 802.118 물리계층 구성

그림 15.22는 Open System Interconnect (OSI) 기준 모델의 하위 계층에 해당하는
IEEE 802.11 무선 BAS) 데이터링크계층과 물리계
음의 세 기능 블록으로 구성되어 있으며, 그 역

oC ~

층을 보여준다. OFDM 물리계층은

할을 간단히 기술하면 다음과 같다.
-ㅡ32              |
MAC Sublayer
MAC_SAP | ,'      .
데이터링크               Management
계층               MAC 부계층                  Entity              MLME_SAP
MLME_PLME
PHY_SAP         SAP        Staion
aacenaen-----4i =             Management
PLOP 부계층 |               ey
물리계층                  PMD_SAP                     PHY layer
ㄴ- 55554 -ㅡ|  Management    PLME_SAP
000 부계총 “pS
그림 15.22

IEEE 802.11 무선 SAlo| 데이터링크계층과 물리계층
540


===== PAGE 537 =====
제15장 IEEE 802,11a/n

1) PLCP(Physical Layer Convergence Procedure) 부계층

PLCPH 물리계충에 수신된 신후로부터 MACHA] 필요한 물리계층 서비스로의 변환
또는 MACHA 발생된 서비스를 물리계층에서 요구되는 신호형태로 변환하여 주는 역할
을 한다. 즉, PLCP* IEEE 802.11 PSDU(PHY 부계층 8600106 Data Unit)S 사용자 데
이터와 2개 또는 그 이상의 스테이션 사이의 관리 정보(0180088001601 information)S 송 ㆍ
수신하기에 적합한 BHOS 변환하여 준다. PLCPE 물리계층과 MACY] 인터페이스로
볼 수 있으며, IEEE 802.11 MAC°] 물리계층과|관계없이 독립적으로 SA 수 있도록

하는 역할을 한다.

2) PMD(Physical Medium Dependent) 부계층
PMD+= 5 GHzo|A] OFDM 방식을 사용하여 2개 또는 그 이상의 스테이션과 데이터를

무선으로 송ㆍ수신하는 역할을 한다.

3) PLME(Physical Layer Management Entity)

PLME:= MAC 3<]*(management entity)2} 연동하여 물리계층의 기능을 관리한다.
물리계층 서비스는 PHY SAP(Service Access Point)S 통하여 MACo] 제공되며, PLCP
와 PMD 사이의 PMD SAPS 통하여 서비스 프리미티브(6041001016) 파라미터가 전달된다.

(2) IEEE 802.118 서비스 프리미티브 파라미터
IEEE 802.118의 peer2} peerZt 또는 부계충과 부계층간의 상호작용을 위한 서비스 프
리미티브 파라미터가 표 15.7에 주어져 있다.

EE 15.7 PHY 840의 서비스 프리미티브 파라미터

PHY—DATA, request           |                          peer to
DATA               00       Octet value 00-FFh
PHY-—DATA, indication                                                                                              peer
TXVECTOR PHY-TXSTART. request    A set of parameters
STATUS PHY-CCA, indication     BUSY, IDLE               sublayer
RXVECTOR PHY-RXSTART. indication A set of parameters              to
Noerror, FormatViolation,      sublayer

RXERROR PHY-RXEND. indication                |
CarrierLost, UnsupportedRate

541



===== PAGE 538 =====
PART IV_MIMO-OFDM 통신 시스템

전술한 바와 같이 MACS 물리계층과 관계없이 독립적으로 동작함을 목표로 하나, 물
리계층에 종속적인 MAC state machineo] MLME(MAC subLayer Management Entity)
라고 정의된 부계층에 존재한다. 이 MLME= 어떤 PMD 구현을 할 경우에는 PHY SAP
프리미티브를 사용하여 PLME(Physical LME)2} 연동하여 동작하게 되는데, 이 때 PHY
서비스 프리미티브 내에 정의된 파라미터 벡터는 TXVECTORS} ×※\8070이며 그 내
용은 표 15.8과 표 15.9와 같다.

= 15.8 TXVECTOR 파라미터

LENGTH                      PHY-TXSTART_ request(TXVECTOR)           1-—4095
6,9,12,18,24 36, 48,54

DATARATE     PHY-TXSTART, request(TXVECTOR)    (6,12 그리고 24는 기본적으로

지원해야함)

scrambler 초기화

7bit+9 null bits

TXPWR_LEVEL PHY-—TXSTART. request(TXVECTOR)    1-8

SERVICE                     PHY-TXSTART, request(TXVECTOR)

 15.9 RXVECTOR 파라미터

LENGTH                     PHY-RXSTART. indicate                                                      1-4095

RSSI                        PHY-RXSTART, indicate(RXVECTOR)                 O-RSSI Max
DATARATE            PHY-RXSTART. indicate(RXVECTOR)                  6,9,12,18, 24, 36, 48,54
SERVICE                    PHY-—RXSTART., indicate(RXVECTOR)                      null

(3) IEEE 802.116 PLCP 프레임 2 및 송ㆍ수신 절차

전술한 바와 같이 TEEE 802.1la PPDU 프레임 그림 15.12와 같이 PLCP 프리앰블,
PLCP 헤더, PSDU, Tail 비트, Pad 비트로 구성된다. 그림 15.23은 PLCP 송ㆍ수신 절차
를 보여 준다.

그림 15.23(8)에 나타난 바와 같이 데이터를 송신하기 위하여 14ㅇ에서 PHY-
TXSTART.requestS 보내면 물리계층은 송신모드로 전환되며, 이 때 PLMES 통하여 =
FASS 적절한 주파수로 동작할 수 있도록 준비된다. DATARATE3} TX 전력과 같은

= 송신 파라미터는 전 AoA) 기술한 PHY-TXSTART.request (TXVECTOR) #4}
PHY-SAPS 통하여 전달되고, 채널이 사용되고 있지 않는 PHY-CCA .indicate(IDLE)

542



===== PAGE 539 =====
제15장_1ㄷㄷㄷ 802.11a/n

PMD_TXSTART req.
(TXVECTER)
PHY_TXEND. cont

PHY_OOA ind
(STATUS-busy)

PMD_TXPWRLVL. req
따따

000.8616.100

PMO_TXSTART.req
PMO_DATA.rea

PHY                                           PHY
PLOP                                          PLCP
은 로
호 주
g 5.
gan                                                                                a 4
vee                                              a
PLCP preanble    SIGNAL        DATA
PHY                                PHY    12 symbols  One OFOM symbol ㅣ variable number of OFDM symbols
PMD                                          PMD
' Coded/OFOM '   Coded/OFDM.    '              ㄴ Coded/t       70060     .
(BPSK, =1/2)            (RATE is indicated in SIGNAL)                                                                      (BPSK, me)      (RATE is Poca mh SIGNAL)
x     =                                           =
(a) PLCP 송신 절차                        (b) PLCP 수신 절차

그림 15.23 PLCP 송ㆍ수신 절차

상태의 경우에는 PHY-TXSTART.request(TXVECT—OR) 프리미티브에 의해 PPDUS|
전송이 시작된다. PLCP= PMD_TXPWRLVL3} PMD RATES PMD# 전송하여 PMD
가 데이터를 송신할 수 있도록 준비시킨 후, PMD_ TXSTART.request= 전송하여 PLCP
프리앰블과 PLCP 헤더의 송신을 시작한다. 일단 PLCP 프리앰블이 송신되기 시작하면 물
리계층은 데이터 스크램블링과 부호화를 시작하며, 스크램블링과 부호화된 데이터는
PHY—DATA.request?} PHY—DATA.confirm 프리미티브를 사용하여 \44ㅅ0과 물리계층
사이의 교환이 연속적으로 이루어지게 된다. 데이터 전송은 5440에서 PHY-TXEND.
160468[를 608016하여 예정보다 일찍 중단하거나, OFDM 프리앰블 LENGTH 필드에 주
어진 숫자에 해당하는 마지막 PSDU octet] 마지막 비트 ASS 예정대로 Sts 수 있
다. 그림 15.23에서 컨볼루션 코드에 의해 부호화된 데이터를 coded PSDU(C—PSDU)=
정의하였고, 8540에서 보호구간은 매 OFDM 심볼마다 삽입되는 것으로 가정하였다.
그림 15.23(6)에 나타난 바와 같이 데이터를 수신하기 위하여 PHY-TXSTART. request
는 0188016되며, 물리계층은 수신모드에 놓이게 된다. ASS PLCP 프리앰블을 수신한
PMD RSSLindicate= 높은 수신신호 레벨을 ?Ｌ(#에게 전달하게 되며, MACS 이를
하여 신호가 수신된 것을 인식한다. 이 때 PLCPE PHY-CCA.indicate(BUSY) 신호를
발생시켜 신호가 수신되는 동안 그 상태를 유지한다. PHY—-CCA indicate7} 발생된 이후
물리계층은 훈련신호를 수신하고, 데이터의 길이, 복조방식, 복호율을 정하기 위하여
SIGNAL 부분을 찾게 된다. 일단 SIGNAL 부분이 짝수패러티에 의해 에러없이 검출되면,
에러 정정 복호가 시작되어 수신된 PLCP SERVICE 부분과 데이터 부분이 비터비 복호

11 에 of

ee

543



===== PAGE 540 =====
PART IV_MIMO-OFDM 통신 시스템

기에 의해 복호된 후, ITU-T (#0-32에 의해 검출된다. ITU-T CRC-32 검사는 복호
된 데이터를 수신한 MAC 프로세서에 의해 수행되며, MPDUS] FCS(Frame Check

필드의 검사가 실패할 경우 물리계층은 #× Idle 상태로 Both. PLCP 헤더
가 이상없이 수신될 경우에 PHY-RXSTART.indicate(DATA)7} 발생되며, 이 때 이 프리
미티브와 관련된 RXVECTORO]+= SIGNAL, SERVICE, PSDU 길이, RSSI7} 포함된다.
수신된 29100 비트는 일련의 PHY-DATA.indicate(DATA) 프리미티브 교환에 의해
00하으로 변환된 후 복호되어 MACO] 전달된다. PLCP 부계층은 마지막 PSDU octet2]
마지막 비트를 수신한 후 수신단을 Rx Idle 상태로 설정하고 PHY—RXEND. indicate
(NoError) 프리미티브를 발행한다. 만일 LENGTH 필드에 지정된 길이의 PSDU octet&
수신하기 전에 PHY-CCA..indicate(IDLE)°] 발생하면, PLCP 부계층은 반송파를 잃은 것
으로 판단하기 때문에 PHY-RXEND.indicate(CarrierLost) 프리미티브를 발생시켜 MAC
에 알리고 수신절차를 종료한다. 또한 RATE YEO] 지정된 속도가 IEEE 802.113 2 Ao]
서 지원하지 않는 전송속도이면, PHY-RXSTART.indicate7} 발생되지 않으며 PHY—
RXEND.indicate(Unsupported Rate) 프리미티브를 MAC 부계층에 전송하여 이를 알린
다. 반면, 수신한 헤더의 패리티 체크가 실패할 경우, PLCP 헤더를 유효하지 못한 데이터
로 인식하므로 PHY—-RXSTART.indcate 프리미티브를 발생시키지 않는다. 이 때, PLCP
부계층은 PHY-RXEND.indicate(Format Violation) 프리미티브를 통해 수신한 PLCP 4]
더가 무효한 데이터임을 MAC 부계층에 알리고 수신을 종료한다.

Sequence)

01666 802.1109 simulink

IEEE 802.lla 기본 블록

IEEE 802.118 물리 ASS 좀 더 자세히 이해하기 위해 SimulinkS 사용하여 먼저 이상
적인 환경에서 기본 SSS 구성한다. 이를 위해서는 여러 가지 파라미터들을 설정하는 다
음 MATLAB 프로그램 15.1(“ieee 802_1la_parameter_set.m”)o] 먼저 실행되어야 하며,
IEEE 802.112의 전체 블록도는 그림 15.24에 주어져 있다.



===== PAGE 541 =====
제15장 IEEE 802,11a/n

으

% 1666 802 lla parameter _set.m

N BPSC = 4; % Modulation Order , 1: BPSK, 2: QPSK, 3: 16QAM, 4: 64QAM
CODE RATE = 3/4; EbNOGB = 6;

n_symbol = 20000;

N_SD = 48;                          * # of Data Subcarriers
N_SP = 4;                           * # of Pilot Subcarriers
N_ST = 52;                          s # of used Subcarriers

N VC = 12;                          % # of Virtual Subcarriers
N_FFT= 64;                          % FFT Size

N GI = 16;                            Guard Interval Size

oe O°

Train_LEN = 160;

 0800. = 3. 26-6)

T PREAMBLE = 16e-6;

T_SIGNAL = 4e-6;

T GI = 0.8e-6;

T 672 = 1.6e-6;

T SHORT = 8e-6;

T_LONG = 8e-6;

N_CBPS = N_SD * N_BPSC;

N_DBPS = N_CBPS * CODE RATE;

End_bit=N_DBPS*n_symbol;

seed = 123213213;                     initial seed

if N_BPSC==1,   Normal = 1; end          6 Normalizatin Factor

if N_BPSC==2,   Normal = sqrt (2);

if N_BPSC==4,   Normal = sqrt(10); end

if N BPSC==6,   Normal = sqrt (42); end

if CODE _RATE==1/2,   Puncture vector=[1 1];end     % Puncturing

if CODE _RATE==2/3,   Puncture vector=[1 11 0]; end

if CODE _RATE==3/4,   Puncture vector=[1 11001]; end

long= [11 =h=L11-<Li-lil 1 bidld-ll-ll 1-11-L1i11
Q01-1-1 1 1-1 1-121-1-1-1-1-111-1-1d1-1i1-i1

1111 ] .「; % Long Preamble

ch=zeros (30,1); ch(1)=1/sqrt(2); ch(14)=1/sqrt(4); % Channel

Training sequence Length
FFT Time

Preamble Time

Signal Time, Symbol Time
Guard interval Time

oe Of ol?

Long Training seq. GI time

00 06 060

Short Tran. seq. time

oP

Long Tran. seq. time

1

oP

end

 프로그램 15.1 IEEE 802.118의 파라미터 설정

545



===== PAGE 542 =====
M-ary number: 2°N_BPSC
Input type: Bit

Receive delay: 34, Computation delay: 0
Computation mode: Entire frame

Probability of 3 zero:                                        Output data: Port                                            이 ordering: Gray .
Pa         t                                                                                                 .      .                                    ormalization method: Min. distance between symbols
Initial seed: seed                                        ( Reset port, Stop simulation                      Mininiuni distance: 2
Sample time: T_SIGNAL/(N_SD*N_BPSC*CODE_RATE])           Target number of errors: N_DBPS*n_symbol*10                   ee trad} 0                                                         _
  Frame-based outputs                                                Maximum number of symbols: N_DBPS*n_symbol*10             Samples pe symbol  1                                                       =
Samples per frame: N_SD*N_BPSC*CODE_RATE             aft                                                                                         =                 |                   제               는
Output data type: double                                     ra              [max(N_BPSC/2.1)+flooré [0‘N_CBPS-1]/max(N_BPSC/2, 1) }                   |                      hs            Oo
Bernoulli ee                               ee             +mod( ([0:N_CBPS-1] +N_CBPS - floor( 16+[0:N_CBPS-1]/N_CBPS ) ). | |                   “he     8
Generator p—--~------a9 ann nn anna nn일                 max(N_BPSC/2,1) ) + 1]'                                               |                      ~ ©
T                T
{       Trellis structure: poly2trellis(7,[171 1331)                     -              ㅣ             ㅣ                                 |                        iO
“aaa     |    =. mode: Continuous                       Number of rows: N_CBPS/16 | |                i                                        |                             | &
「                                                                                Number of columns: 16               |                      !                                                        ㅣ                                         ㅣ         |
14401 |                       (Puncture vector’)                       1        |                                           ㅣ      a/Nornial         |
| | Convolutional [28801 ,               [192x1]       x      Matrix                {        General Block | [19201]       =                  oa       9831]      를
>                              | Puncture                ㆍ                                                                     *) Rectangular        >                        2
09901]        Encoder                                                 Interleaver          |         Interleaver                          nay                                     i
|                                                                         '
Convolutional Encoder           Puncture                               {         |                                    Rectangular QAM     TxGain              nur
!          |                                       Modulator Baseband                            a
[14401]    TX Error Bate    3                    Slt   Variable name: BER       |         :                                                                                     때
:       +                   um Errors} |         F          |]          ㅣ               06       ;                                                                  >
Calculation     al                          !       Limit data points to last: 1 | |          i              Initial seed: seed                                                               <
[14461]   Rx                   ae  oe Bits    Decimation: 1          |        |          Made: Signal ta noise ratio [SNR]                                 ral
Error Rate                   e          Saar  Sample time: -1           |         |             SNR (dB): EbNOdB +10*log1 O(N_BPSC*CODE_RATE)                       or
Calculation     ㅣ   후 > sea |      Save format: Array        |          Input signal power {watts}: 1                    ) eel          은
ㅁ                                                          |          1
Selector4 To workspace                          ㅣ        |                                                    80644                | Ww
-                     -                                                              H          |                                                            Channel     AWGN      |    웅
Trellis structure: poly2trellis(?, [133 171]]                                                i          |                                                                                      |
(J Punctured code                                              |       i                                                     [48x1] 7   너
(J Enable erasures input port                                                   |         |                                                                       fo      uw
Decision type: Unquantized                                               ㅣ        |                                                             ~        =
=                              Traceback depth: 34                                                                   |           Ss                                                                       |              “
a                            Operation mode: Continuous                    Meynunber2                     i             Sy                                                               Zo                 re}
4                                         :                        1                Ny                                                              a
더                           [] Enable reset input port              Polarity: Negative                |              S                                            we                 70
|                       {                   (Puncture vector) | Output data type: Same as input     |                `                   더
=                             SSS                                       aul 또                Matrix                General Block                                  Ne |
=               | Insert Zero |e          Bipolar     주          Sg    '           t       Rectangular ==
S               1441) | Viterbi Decoder| 28%"              [192x1]   Convener     (192x1] |Deinterleaver| [192x1] | Deinterleaver    [192x1]     OAM      [48x1] east
I                            Viterbi Decoder               Insert Zero             Unipolarto Bipolar              Matrix                  Sencral Blok          Rectangular QAM

Converter             Deinterleaver                             Demodulator Baseband

Deinterleaver

=
be
a
<
a



===== PAGE 543 =====
제15장_16ㄷㄷㄷ 802.113/ㅁ

그림 15.24의 전체 블록도에는 각 Simulink 블록들에 대해 설정된 파라미터들이 주어져
있으며, 몇 가지 부가적인 설명을 덧붙이면 다음과 같다.

- Bernoulli Binary 0460018010[는 랜덤 비트를 생성하는 블록으로서, 0.5로 설정되어 있어
0과 1이 생성될 확률이 동일하다. 또한 Sample 0006은 한 심볼의 길이 T_SIGNALS
부호화를 포함한 모든 비트로 나눈 값으로 설정된다.

- Convolutional 80000@는 그림 15.3에 주어진 컨볼루션 부호화를 수행하도록 설정된다.

- Puncture 37} Depuncture (Insert Zero) 블록의 Puncture vector] 프로그램 15.1
(“ieee 802_1la_parameter_set.m”)o] 저장되어 있는 Puncture vector= 설정된다 (그
림 15.4 참조).

- Matrix Interleaver2} Deinterleaver, 그리고 General Block Interleaver2} Deinterleaver
블록의 파라미터는 식 (15.1)~(15.4)에 의해 설정된다.

- Unipolar to Bipolar Converter 블록은 0 또는 1의 AJBAS 1 또는 -1의 Bipolar= 바
WE 역할을 한다.

- 송신단과 수신단의 Gain 블록은 송신 ASS 1로 맞춰주기 위해 변조 차수(020041840ㅁ0
order)°]] 따른 정규화 인자(001000801126 factor)S 곱해주고 또 그 값으로 나뉘주는 역할
을 한다.

- AWGN 블록은 모드를 SNRE 하고 변조 차수에 따른 EbNOS} SNRY] 차이만큼을 더
해주되,부반송파당 비트 개수(4 8090)에 부호율6006 rate)S 곱해줘야 하며, input
signal power= 앞서 정규화 인자를 곱해 주었으므로 1이 된다.

— Error Rate Calculation 블록은 복조된 수신신호를 송신 데이터와 비교하여 오차 비트
개 수와 총 비트 개수, 그리고 오차 비트 개수를 총 비트 개수로 나눈 81 Error Rate

을 출력해 주며, Receive 0613*는 그림 15.3을 참조하여 Convolutional Encoder 블록
에서 설정된 컨볼루션부호(171 133’)2] 구속장 7의 Of Su 정도인 34로 설정된다.

“Ohya, IEEE 002.112 채널 추정부
그림 15.25(0)는 채널 추정부를 포함한 IEEE 802.118의 블록도이며, 각 블록의 파라미
터 설정에 대한 설명은 다음과 같다.
- Multiport Selector} 그 다음에 설치된 Matrix Concatenation 블록과 더불어 Zt Row
들사이에 그림 15.5에 주어진 FUSS 삽입하기 위한 블록이다. 예를 들어, 입력신호
의 5번째와 6번째 샘플 사이, 18번째와 19번째 샘플 사이, 24번째와 25번째 샘플 사이
등에 IRS 삽입한다.

547 —



===== PAGE 544 =====
PART IV_MIMO-OFDM 통신 시스템

OFDM Modulator

Generator polynomiat [10001001]        Pad over: Columns      aa

Initial states:                               Pad value source: Specify via dialog

ni   es: 1111111]       Pad value: 0                        -   -  os
:                          ae oe                                                             Number of input dimensions: 1

Output mask source: Dialog parameter           Output column mode: Userspecified/Next power of 2           Index mode: One-based

Column size: N_FFT

Output mask vector (or scalar shift value}: 7      Pad signel at: End                                                  Index vector: [27:64 1:26]

Sample time: T_SIGNAL                    Action when truncation occurs: None/Warning/Error J+,       nplib pores ern EBT

CO Frame-based outputs                                                                     301, | 9 VC eax)

16901],  {reer   (1
u      을 고                =격  G5
드  Reset on nonzero input                                                                                           Int                 680                                      브릴             Out

Output data type: double                                                                                                                                                                                                                                          IFFT4
T
1

Selector

ero Pad
(Virtual Carrier)

PN Sequence   »  oe 널                                                 3
Seneraton         Cinverter               qe          >                              Long_preamble
PI Seauenze                                                >        (Sample based)    ;       Gots         Index vector: (33.64 1:64 1:64]
타우                                   Si 08994                                「      OFDM      Bet, Add Prefix veoey
Bernoulli [Bernoulli Binary                          해              |              애써               Modulator        배
Binary     Generator                                1801                       Constant             Long signal             0

726Ｌ

1/Normal
00201 | Lt    zal          ral     Select
19201] > | Rectangular                                         Rows

QAM                  Gain                               0011
Rectangular QAM
Modulator Baseband                                       >
1301]                  os

회

mee signal

“ Selector
Number of input dimensions: 1
Index mode: One-based
Index vector: [49:64 1:64]
Input port size: N_FFT

Select: Rows                                    회 Bxt                                                               [0x1]           [160x1]
Indices to output: {1:5,6:18,19:24,25:30,31:43, 44:48}                                                                                   ¥                ¥

Matrix Concatenation
Mulnport                                                                     ch     ㅣ          Simple
elector!                                                             channel [Channel channelfcpannel
09200 | ^ Error Rate | 3                Error rate
Calculation      eee Num Errors                                                                            ㅣ
1960 Num Bits                                                                    68001 ~     16001]
Error Rate                   사이
Calculation                                                                                                          .
Rows
6         AWGN
Multiport        Goto                                                              Subsystem3
Selector2                                                                                                            16001]
Select: Rows
indices to output: {[1:5 7:19 21:26 28:33 35:47 49:53]}            (index vector: [39:64 1:27])                Cndex vector: [17:80
Normal                         Product     se                                              ㅁ
AL                                          x qty     40          70            FFT        }yRemove,,
b— pectangul                      Select                    3x1]            4x1]| Frame |“ [64x1]         16401] Prefix
19200 | PEC tangular [060]          xT]] Rows    16301]       중
Al             Gaini                                      Selector      Frame Status      FFT         Selector1
7                                         Conversion
Rectangular GAM                Multiport
Demodulator Baseband             Selector                                                                    16001]
6 로니 Estimation|
6301]
63010]           301]
브리              Subsystem9
Switch1         Subsystem10
_          eres es                                              | idesi channet | Channel
(a) AWS SATS 포함한 IEEE 802.1138의 SSH         Pa
Simple Channel with Delay                                       Pad over. Columns
Pad value source: Specify via dialog
Pad value: 0
Output column mode: User-specified/Next power of 2
Column size: N_FFT+N_GI
Pad signal at End
Select: Rows                                                     Action when truncation occurs: None/Warning/Error
Indices to output: {1:N_FFT+N_GI ,N_FFT+N_GH1:N_FFT+N_GH29}
6061]       가     70        101
Select              “| Frame
Bows [08901         Frame Status
                   Conversion3
이버                 Delay line size: length(ch)-1
Initial conditions: 0
DSP       Frame Status                                             To         S      Deley
Constant Conversion2                                  이      Frame              Line
Frame Status       Delay Line       Zero Pad
Conversion3

(6) 지연요소를 포함한 Simple Channel SS

Simple Channel                                         Select: Rows
Indices to output: {1(N_FFT+N_GI)+2}

0719]       70       1711         Select [[160x1]                      eB
SONY             Frame                Rows

Out1

[16091

Convolution       Frame Status               -
Conversion4            Multiport
Selector

Frame Status
Constant —Conversion2

(0) 지연요소를 포함하지 VES Simple Channel SS

그림 15.25 IEEE 802.113 채널 추정부의 블록도("1666 113 _아13006! _681.001` )

548



===== PAGE 545 =====
제15장_ 166ㄷ 802.113/ㅁ

— PN Sequence Generator= BUR 시퀸스를 생성하는 블록으로서 Generator poly-
nomial x7+x4+10|3l 초기 $660는 [1 1 1 1 1 1 1]이며, Sample time® 한 프레임
당 한 번씩 생성이 되기 때문에 T-SINGALS 설정된다.

- OFDM Modulatore}= subsystem] Zero Pad (Add VC) 블록은 53개 샘플로 구성된
신호에 가상 부반송파(\(: Virtual 081080로서 11개의 영점을 삽입하여 샘플의 개수
를 찌 바1=64개로 만든다. 그 다음에 설치된 96160607 블록은 앞에서 삽입된 00] IFFT
전에 가상 부반송파 자리에 위치시키는 역할을 한다.

- OFDM Modulatore}= subsystem 다음의 Selector2 (Add Prefix) 블록은 CP(Cyclic
Prefix)S 삽입하는 ASS 한다.

- Channel& 통과한 후, 수신부에서는 가장 먼저 Remove ㅁ76[&라는 Selector! 블록에서
Cyclic PrefixS 제거하고 그 다음 FFT 블록에서 FFTS 한 후, 그 다음 961601072 블록
에서 Virtual CarrierS 제거하여 데이터 부반송파만 선택한다.

- Product 블록에서는 다음 AS 수행하여 추정한 채널의 영향을 보상한다.

Yk]

24

(15.20)
- Select Rowe}= Multiport 50160[072에서 }UH 심볼과 DC 성분을 제거하고, Gain 블
록에서 제00081로 나눈 후에 QAM Demodulator 블록에서 복조과정을 수행한다.

14 15.25(b)= 294 15.25(a)2] ‘Simple Channel with Delay’ 5060979180의 블록도이
며, DSP Constant 블록에 입력되는 채널계수 벡터 애는 프로그램 15.1(“802 118 _
parameter_set.m”)2- 통해 주어지도록 되어 있다.

— Frame Status Conversion (To Frame) 블록은 sample 단위의 데이터를 프레임 단위로
바꿔주는 역할을 한다.

- Multiport Selector 블록은 컨벌루션을 거쳐서 나
과 다음 심볼에 나갈 부분으로 나누는 역할을 한다.

- Delay line 블록은 (30샘플의 채널과 80샘플의 데이터를 컨볼루션해서 얻어지는 109개
의 데이터 중 뒷 부분에 있는) 29개의 데이터 중 06137 line size 만큼을 지연시켰다가
그 다음 심볼에 더해서 내 보내는 역할을 한다.

- Zero Pad 블록은 그 다음의 Add 블록에서 더해지는 샘플의 개수를 맞춰 주기 위하여

을 추가함으로써 샘플의 개수를 찌 FFT+N 021=80개로 증가시킨다.

데이터를 현재 심볼에 나가는 부분

'

(에
1 개

549


===== PAGE 546 =====
MIMO-OFDM 통신

PART IV_

1%] 15.262 Add Noise subsystem2] 블록도로서 AWGN°|z}= Simulink 내장 블록

과 더불어 (설정된 SNR 맞는 크기의 FSS 생성하는 데에 필요한) 신호전력을 측정하
는 부분을 포함하고 있다.
(1 Jina magnitude*2        Running mean
fet ig ju   1 0 FH
0000          ;                     Display4
¥     Math Function      Mean        Meant

AWGN

Mode: Signal to noise ratio (SNR)
SNAI[dB] : EbNOdB+10+log10(N_BPSC)
Input signal powerlwatts] : 0.01289

Initial seed: 12345
-                  Channel

그림 15.26 Add Noise subsystem2] 블록도

하기 위해 구성한 9109796601이다. 그

그림 15.27은 식 (15.20)을 사용하여 채널 추정을
림 15.25(8)의 우상부에 주어진 long preamble(X[A])2 데이터 트래픽 신호와 별도로 =

로그램 15.1(“1666 802_1la_parameter_set.m”)-& 통해 식 (15.11)에 주어진 값으로 생성
되며, OFDM 변조 과정과 900016 channelS 통과하여 나온 출력(”[/])을 사용한다. 여기
서 OFDM 변조 과정이나 채널 BRS 데이터 신호가 거치는 과정과 거의 같기 때문에 A
명을 생략한다.

REL Sremove wc                  Number of input dimensions: 1

Index mode: One-based
Index vector: 39:64 1:27

Number of input dimensions: 1                                                                      Maes
Index mode: One-based                                                              Input port size: N_FFT
Index vector: STAN Shee ER FET          er          16401]               16901]            631
Input port size: (N_FFT+N_GI)}+2                097           us       To        LAP      ¥   3      1
:       1 fe  270      pu          (1 )
Number of input dimensions: 1                       a       101                                                                    0ㅁ41
Index mode: One-based                                            타거        Frame Status         eelector
Index vector: [1+STO(1}(N_FFT#N GIMENSTORTL                         Conversion
Input port size: CN FFT+N_GI)+2                               =
16001           | 1601             16901]    FFT &     [53x1]
(ㄱ et,  p———pU Ss Y          us ¥                            x
                 cond                 remove ¥C         시      631   a  polos   ae 7
6300 느                              레
Selector          Selector1         Subsystem         Product     63811       Gain            Outt
1.499 -0.2215i
Select                                          (1.56 -0.3767i]
Long_preamble > 211    raed   69001]                              6301]
From                          ns
Remove DC   a
f
63x11 [=
+      15381
us 이쁘] FFTs     6311    ee
[160x1] ,                   remove YC
Product
wf Selector2         Subsystem2

Index mode: One-based

Select: Rows
Indices to output: [1:26 (1) 28:53]

Index vector: STO(1)+N_GI#2+N_FFT+[1:N_FFT]

Ee of input dimensions: 1
Input port size: (N_FFT+N_Gh+2

그림 15.27 Long preambleS A

550

주정 subsystem


===== PAGE 547 =====
제15장_|6ㄷ6ㄷ 802.11a/n

apie of input dimensions: 1
Input Real                       Index mode: One-based
아비 part: 0                                  Index vector: [17: 80]
Sample aime ~iinherited)                  Input port size: N_FFT#N_Gl
+] teat)          0001,           BO} To       001. | Simple [06091           1690]
[1 26109.1,03))       | 가타     oy       Rl 1+1       se    Fane            아려        eu     Ed
DSP Constant       Add Prefix      me emriee i      eee    i“  channel       Remove Prefix
ㅣ
         두         0                a           |   {  Number of input dimensions: 1
ss                          0             u      ye         ql         ndex mode: One-base
FFT           Frame                       C4)! | index vector [3864 1:271
-                                          Gutt |     Input port size: N_FFT          ?
SUnSuRtam       Frame Status      Remove ¥C             {
부             Conversion1       and Tecider              |
ㅣ
(a) Ideal Channel subsystem                              |
고                                                         ㅣ
Simple Channel                                             Select: Rows
Indices to output: 11: N_FFT+N_GI}
qe                >          0101]                1x1                 01
si                  a     To         x           Select     x
101                              CONV         "| Frame                   Rows
Out1
Convolution       Frame Status                .
Conversion4              Multipart
ch H2        To                                                          Selector
Frame    [12x1]
DSP      Frame Status
Constant    Conversion2

(b) Simple Channel subsystem

그림 15.28 이상적인 xHE(Ideal Channel) subsystem

- 이 채널 44 subsystem2] 앞 부분에 설치된 9616060『는 원래 short preamblez} long
preampleS 분리하기 위한 것이나 여기에서는 8100 preambleS 생략하였으므로 사실
상 하는 역할은 없다.

- 다음에 나오는 961600071과 Selector2S 사용하여 각각 4 +[1(64)개의 ASH 구성된
이어진 두 개의 ASS 따로 분리한다. 두 심볼에 대하여 FFT 처리와 VC(Virtual
Carrier) 제거 및 식 (15.20)의 계산과정을 거친 후 두 채널 추정 결과의 평균치를 취함
으로써 잡음의 영향을 감소시킨다.

그림 15.28은 그림 15.25(8)의 하부에 주어진 이상적인 채널(10681 Channel) subsystem
을 보여준다. 여기서는 이상적인 ABS 구하기 위하여 임펄스 ASS 입력으로 사용하며,
프리앰블을 사용하는 Channel Estimation 94168751601과의 채널 추정 성능 비교 SS 위하

여 사용된다.

eye

SQA IEEE 802.113 반송파 주파수 옵셋 추정부와 잔류 위상 옵셋 추적부

u

본 절에서는 그림 15.292] Simulink 블록도 “1666 118 channel and CFO es.mdl’-
통하여 IEEE 802.118의 반송파 주파수 옵셋 (CFO) 추정부와 잔류 위상 옵셋 추적부를



===== PAGE 548 =====
Running

<= Num_symbol

pet          oun              60101
Pulse Generator! Cumulative Sum               ete
Pulse type :Sample based        ul if (u1==5)       Preamble_time2
Time(t)      : Use simulation time                                       cz
Amplitude    1                             114              60106
Period  .    : Pilot_tracking_duration
Pulse width :1                          ul if (ul==5)          Preamble_timet

Phase delay: Pilot_delay

Sample time : T_SIGNAL                          115                 60105

Pulse 006  : Sample based          허이 if (u1>=5) < Data_time1    |
Timett      : Use simulation time

amp livee   31                                     111                  60102

Pulse width 21                       aaa  if (ul==6)  < Data_time2    ㅣ

Phase delay: 0

| Sample time : T_SIGNAL                             ie                   90198
HH H+
tee                         해 if (ul==1)      Pilot_tracking_time
He HH +
Pulse Generator2                                   113                   90008
i                                                                 Matrix Concatenation1
                  :                           6301]       OFDM       1601
Bernoulli Binary          _               short           Modulator           é
Generator                   Timing                   Constantl              Short signal                         도
Bernoulli                                                                  [    F
Binary              Subsystem               long     63801]       OFDM       16001         “           7
[192x1]                                                Modulator                A       Simple channelt
1/Normal Constant             Long signal                              Channel
' =  :  ‘ * | fase]            is                             OFDM                            [2001]
>]  694 ar                                             “| Modulator          18001]
Gain                    Subsystem4
Rectangular QAM                                                                “                     Simple        AWSN
Modulator Baseband                                                  channel! channel        02001]
.001039]|ㄷ「「0「 rate
PIT Error Rate           396 ]]Num Errors                          Subsystem3
ㅣ         3.8282+005      i
—p1Ax Calculation    So = :  Num Bits                Zo) Ebnoas
EH             play                                   Total symbol
tror Rate                           loutputt- 4m         STO
Calculation         Select       BER            0.1]|CFO                                         Display
aa :      =i                   0.007034] | BER
ultipor:        oto                 i
Selector?              Subsystem8 Display3
1  ¥
Manual                Manual
Select Rows                                                           Switch2                 Switcha
Indices to output: {[1:5 7:19 21:26 28:33 35:47 49:53]}
N
WAI | sort 1. |                                     Box]
| Rectangular                age                                                                                          From
Gains                                                                                 If Action
Rectangular QAM              a ae                                                                   Supevelen!
Demodulator Baseband             SEES
Phase Tracking

Manual
Switch

Subsystem9
Subsystem10
Ideal Channel

552

ㅣ
ㅣ
102      Product   Matix Complex to  Magnitude-Angle 7U" !
54011 Magnitude-Angle to Complex    !
1
sy                     1
Select: Rows                                         Phase Tracker
Indices to output: {[1:53],[6 20 34 48]}
(1 Lp! select Rows |          ;        If Action
Int        Subsystem
Ind               1901]                _
ㅣ                           jut
Multiport Selector       > !
>       a  Subsystem1           '
i                  be
PN Sequencely | ype tl |          러| 2             Fran             |
Senetetor    Converter  Lo   1    Pilot_tracking_time 4
PN Sequence                                     Matrix
Generator                 Concatenation
A  x  A     x  wa   2 오
그림 15.29 반송파 주파수 옵셋 추정부 및 잔류 위상

(“ieee_11a_channel_and_CFO_es,mdl”)



===== PAGE 549 =====
제15장 IEEE 802 11a/n

설명한다. 여기에 사용되는 반송파 주파수 옴셋 추정 기범과 잔류 위상 Qa
15.1.4절에서 설명하였다.

적 기법

rlo

7

- 그림 15.292] 상단에 위치한 Timing subsystem]]4] Pulse Generatorl-2 T_SIGNAL2]
주기마다 크기와 길이가 1인 BAS 발생시키고 그 다음 Cumulative Sum 블록에 의해
누산되는 Num_symbol& 근거로(정해진 조건이 만족되는 시점에서 ASS 통과시키
는) 블록에서 채널 추정에 사용되는 1008 preamble] 위치를 지정한다. 또한, Pulse
Generator2 블록은 T_SIGNALS 주기로 sb 2|A(pilot delay) 만큼의 위상 지연
(phase 0618)과 D}Ue 심볼간 간격(0110! 0ㅁ80008 duration) 가지고 크기와 길이가
1인 BAS 발생시킴으로써 그 다음 블록과 더불어 위상추적에 사용되는 apelel 심
볼의 시간상 위치를 샘플 수로 지정해 주는 역할을 수행한다.

- 여기서 Goto 블록은 일단 구해진 데이터를 다른 곳에 쓰기 위해서 저장하고, 000 블

록은 0000에서 저장한 변수를 다시 불러오는 역할을 한다.

- 송신단의 OFDM Modulator= 앞서 그림 15.25에서 사용된 것에 CP(Cyclic Prefix)S
삽입하는 SSS 추가한 910559[60이다. USy 가상 부반송파의 삽입과 IFFT 과정
및 CPL] 삽입 과정을 수행하여 송신신호를 구성하고, 수신단의 OFDM 106010041410[는
그 역 과정을 수행한다.

- 데이터 신호가 통과하는 AWGN 채널이나 9100/1048 preambeo] 통과하는 채널에 대한
블록은 그림 15.25에서 사용된 것과 같다.
- 그림 15.29의 하단에 위치한 위상 추적기(0※1896 Tracker) subsystemo]A]= Select
Rows?}= Multiport Selector 블록을 사용하여 수신 신호의 wpe] 심볼 샘플 값들을
추출해서 EY 복소수를 취한 결과를 (자체적으로 생성한) 위상 추적용 wheel 심볼과
(From 통해 호출된 010 0ㅁ800108_0006에서) 곱한 결과의 위상으로부터 위상 변화값
을 추정해서 그 위상만큼 데이터 신호의 위상을 보상해 준다.

그림 15.30과 그림 15.31은 각각 그림 15.29의 오른쪽에 있는 CFO Estimation subsystem
과 CFO (인가 및 보상) subsystem 보여 준다.

- 먼저 그림 15.30(0)에 있는 CFO Estimation subsystem 보면 앞 부분에 가상적인
CFOS 도입하는 400 CFO subsystem®] 있는데, 그 자세한 블록도는 그림 15.31(3)에
주어져 있으며, 그 기능은 데이터 신호에 6724610/* (6: CFOS 곱해주는 것이다.

- 그 아래 Select 0\5라는 Multiport Selector$ 통해서 long preamblez} short

553



===== PAGE 550 =====
PART IV_MIMO-OFDM 통신 시스템

preamble 분리한다. 그 후에 Coarse CFOes_Te}+= subsystem®||4] short preamble
사용하여 그림 15.30(0)에 주어진 과정을 거쳐 개략적인 CFO 추정(00066 CFO
690108000)을 수행하고 그 결과를 가지고 long preambleS 보상해 준다. Fine_
(2069 2 9060979660에서는 coarse CFO7} 보상된 long 20『6801016을 사용하여 때
15.38(6)에 주어진 FAS 거쳐 보다 정밀한 CFO 추정(0106 CFO estimation)S

한다. 그 결과는 개략적인 CFO 추정 결과와 더해져서 CFO_est 값이 eres CFO
subsystem] 이를 받아 데이터 신호의 CFOS 보상하는 데 사용한다. 또한, CFOS
보상한 전 preamble 신호를 0011이라는 출력으로 내보내어 채널 추정에 있어서도 가
능한 CFO 영향의 감소나 AAS 도모한다.

- 그림 15.30(0)에 주어진 개략적인 CFO 추정부는 16개 샘플로 구성된 ASO] 10회 보
복되는 short preamble 사용하여 인접 심볼과의 공액복소수 곱을 취하여 CFOS
정한다. 8번째 심볼과 9번째 심볼, 그리고 9번째 심볼과 10번째 심볼간의 위상차를 이
용하여 추정한 CFO HS 평균함으로써 정확도의 향상을 도모한다. 그림 15.30(6)에 주
어진 미세 CFO 추정부는 64개 샘플로 구성된 심볼이 2회 반복되는 long preambles
사용한다.

- 그림 15.3106)에 주어진 CFO subsystem2 그림 15.29에 포함되어 있는 CFO
subsystem2] 상세 블록도인데, 이를 구성하는 두 가지 중요한 subsystem Add CFO 블
록과 CFO Compensation 32°] 그림 15.31(0)와 그림 15.31(0)에 주어져 있다. 그림
15.31(0)에 주어진 Add CFO subsystem? 가상적인 CFOS 도입한다는 AoA] 그림
15.31(8)에 있는 (프리앰블을 사용한 CFO Estimation subsystemo]*] 사용된) add
CFO subsystemi} 동일하다. 그림 15.31(a)°ol] 없는 From 블록과 DSP Constant! 블록,
그리고 Gain 블록은 지금까지 총 샘플이 몇 개이므로 지금 들어오는 샘플이 몇 번째
것인지를 계산하는 기능을 수행하는데, 이는 CFOS 도입하는 과정에서 심볼이 지나갈
때마다 위상이 초기화되는 현상을 방지하기 위한 것이다. 예를 들어, Num_symbol®] 1
일 때, 즉 첫번째 심볼일 경우에 DSP Constant] 블록의 1을 빼면 0이 남는다. 0에다가
Gain 블록을 곱하게 되면 어차피 0이 되므로 그 뒤에 더해지는 DSP Constant 블록의
상수가 그대로 latch. STO 0 이라면 부터 79 Abia] 1 ae ola: 다

으로 Num_symbol°] 2인 경우, 09『 000918011에서 1을 빼면 1°] 남고 CFOIS 곱
하면 80이 된다. 그 다음 stor 0일 4-2] 0~80 더하면 80번째 샘플부터 1594
째 샘플까지의 2번째 심볼을 의미한다.

     ae



===== PAGE 551 =====
제15장 IEEE 802.11376

Coarse CFO Compensation
16001]

Producti    Magnitude-Angle
to Complex

DSP Constant1

(a) Coarse CFO compensation subsystem
Overall CFO Compensation      7    20x41]                                           a
Int                                          >. [p20x1
cfo_es                                                    Product       밀기
                          =         7              ay!       Product! Magnitude-Angle
[| _-STO(1)+ [0:(N_FFT#N_GI#4-1]                    Convio
DSP Constant
=                                                                     10200] |"! uey 22091
2      add CFO              ‘,                                                mi cto_es               Outt
cs                                               CFO_comp1
.                                                                (1 )
Ny                      CFO_est
~                       !            2B |itAction
Select Rows                           is           Ee mea .   |Subsystem
Indices to output: {[1:160],[161:320]          ~               From                =                        CFO_er
eS ee                       ei,
Select      ’                ~
Rows     rCoarse_CFOes_T              Fine_CFOes_F2
| | 60001            natu     160x1
|                         ourt MEO int 01
Multiport |                  feicto_es
Selector                       CFO_comp               개

(6) CFO estimation subsystem

Number of input dimensions: 1      Coarse CFO estimation
Index mode: One-based
Index vector: [113:128]
Input port size: 2,54N_FFT

Column
Sum

Math            00
『40에001                 Product           -          Complex to
ext                                Mattix Sum MMagnitude-Angle

16x1
Selector
(ndex vector: [129:144])   tae

4                 16x1     Column
pst)              Function2             x     WSxtL |

te                  Sum

Producti        Matrix Sum1 ncemice Anais

Selector:

(index vector: [145:160] )

(d) Coarse CFO estimation

Fine CFO estimation
Index mode: One-ba:
Index vector: [0 0019657001

fee of input dimensions:  1
Input port size: 2,5#N_F

[1601]         901
님   a                     | Column
101
selector       Math                   Soin      Outt
Function4    Product          :     Complex to Gainl
Matrix — Magnitude-Angle
Sum2
Index vector: [97-570(1):160-570(1)1)

selector1

(6) Fine CFO estimation

그림 15.30 반송파 주파수 옵셋 추정부 및 보상부

555



===== PAGE 552 =====
PART IV_MIMO-OFDM 통신 시스템

    2081

101

Product

[rSTO@y-STOMN_FFT+N_Gira tp [Pe
DSP Constant                FON,  Magnifude=Angle [rt 2*pi/N_FFT*CFO(1)

to Complex       Multiplication: Element-wise(K.*u)
So Ssee= seas ee)  Sample time (-1 for inherited): -1

(a) CFO Estimation system] Qf FROM 가상적 다0의 [2S 위한 add CFO subsystem

CFO                                Add CFO
es  [z}cro-est                  Tx |

(C2+pi/N_FFT#CFOG)) CN_FFTAN_GI)

[80x 1]        |
pisbiey2     Butt      Product
!
Magnitude-Angle CFO
add_CFO|Add CFO
to Complex                               | |osP constantt
[0x1]                                         DSP Constant |-STOC)HO:N_FFT+N_GI1]
¥
CFO_est                                (6) Add CFO subsystem
CFO      ladd_CFOT                 ri
Compensation               CFO Compensation
1 )101
Pax)                                                             ~2epi/N_FFT
(+ Jour                                                                               CFO_est

Magnitude-Angle Producti
to Complex

(b) CFO subsystem

DSP Constant | ~STO(1)+128+[0:N_FFT+N_GI-1]'

| 8 |DSP constanti

(d) CFO compensation subsystem

그림 15.31 CFO subsystem2| 상세 블록도

ㆍ 주 cee 802.11n

8 IEEE 802.117 규격 및 기본 블록

본 절에서는 IEEE802.1In9} 물리계층 규격 및 기본 블록에 대해서 설명한다. TEBE
802.112은 기존의 무선랜 시스템인 IEEE 802.118/6&와 호환성을 유지하면서 고속의 데
이터를 보내기 위한 MIMO 무선랜 시스템이다. RTS/CTSS 이용한 protection
mechanism 적용하여 IEEE 802.11b2} MAC 레벨에서 호환성을 보장하고(116 패킷을
이용하여 예약한 후에 전송), 프리앰블 및 물리계층 SIS 1188와 호환 가능하게 구성하
였다[301].

표 15.10은 IEEE 802.117 물리계층의 주요 파라미터를 보여준다. IEEE 802.117은 기
(mandatory) 모드와 옵션 BES] 2가지 모드로 구성이 되어 있다. IEEE 802.111에서
송신 안테나는 기본으로 WHS 사용하고 옵션으로 4개까지 고려하고 있다. 안테나의 개수
에 따른 스트림의 개수도 총 4개까지 고려하고 있다. 대역폭은 IEEE 802.118와의 호환성

556

000



===== PAGE 553 =====
제15장_ 1666 802.113/ㅁ

표 15.10 IEEE 802.11ㅁ의 물리계층 주요 파라미터
1 and 2                3 and 4
2                Greater than 2
20 Mhz                40 Mhz
56 in 20 Mhz          114 in 40 Mhz
52                    108
4                      6

256QAM in
| Molton Order  EE cre    Beamforming mode

1/2,-2/8.3/4, 5/6
800ns                  400ns
R=1/2 k=7033:171)
Tx and Rx optional
Rx mandatory           Tx optional

때문에 20MhzS 기본으로 정하고 옵션으로 40Mhz7}A%| 고려하고 있다. 따라서 IEEE
802.110에서는 안테나 수의 증가와 추가 대역폭의 지원으로 인해 물리계충에서 데이터 전
송률이 최고 600Mbps7}4| 가능하다. 부반송파의 개수는 205402대역폭에서는 56개(데이
터 52개 + BLE 4개), 405462대역폭에서는 114개(데이터 108개 + 3}Uel 6개)로 구성
되어 있다. 변조방식은 888&에서 640414까지를 기본으로 지원하며, 옵션으로 빔형성 모
드에서는 2560414까지 지원한다. 보호 구간은 기본 80028로 정해져있고, 옵션으로 고속
데이터를 위하여 40078까지 지원하고 있다. 채널 부호화로는 부호화율이 1/2, 2/3, 3/4,
5/6인 컨볼루션 HSS 사용하고 옴션으로 LDPC HSS 사용할 수 있다. 위의 기본 사항
의 경우 최대 전송속도는 2 공간 스트림, 20MHz, 64-QAM, 5/6 HESS 사용하는 경우
130804608이고, 옵션 모드의 경우에는 4 공간 스트림, 40MHz, 64-QAM, 5/6 HESS A}
용하여 600Mbps7}4| 가능하다. 이와 같이 IEEE 802.110에서는 무선랜의 HT (high
10000480240과 성능 개선을 위해 다양한 기술이 기본 또는 옵션으로 채택되어 있다.

표 15.11은 IEEE 802.11에서 사용되는 타이밍 관련 파라미터를 보여준다. 205442대역
에서 Non—HT =F} HT 2S] 데이터 부반송파 수는 각각 48, 52개이며 apelele 모
두 4개를 사용하여 IEEE 802.118에서 사용하였던 가상 부반송파 12개중에서 4개를 HT
EMA 데이터 부반송파로 사용한 AS 알 수 있다. FFT 크기는 20542대역과 40MHz
대역 각각 64, 128이며, 부반송파 간격은 모두 312.51012로 동일하여 심볼 주기도 3.28
Suse.

|

Nw

557


===== PAGE 554 =====
PART IV_MIMO—OFDM 통신 시스템

E 15.11 IEEE 802.11의 타이밍 관련 파라미터

— 수 ae
Nop & BST               52                        56                   14                   104
Af: 부받송파 간격 9312, 5kH2(20Mhz/64) 312, 5kHz             312, 5kHz(40Mhz/128)
Depp AFPT/FFT 주기            3. 2us                   3, 2us                          3,2us

Tey BBR   0,848= Tppr/4       0.8 ps                0.8 pus

이 절를추시 1 007   4/46= 27277 Top        4//6            !       4s

A

saad                    —        —

I         C                        IDET    insert GI     Analog

mapper                          and Window    and RF

Constellation                         insert GI     Analog

aa interleaver na  ‘mapper ㆍ     050    |  이 IDFT | and Window   and RF
Constellation

이 때때 | [Sosa] Lee 1.
Constellation

me interleaver nal mapper _   - CSD

ce

그림 15.32 IEEE 802.11n 무선

Encoder Parser
Stream Parser
5186
Spatial Mapping

Insert GI          Analog
이  1OFT 1 and Window 더    and RF

Insert GI        Analog
| oe i and Window io!   and RF

tooo

그림 15.12 HT 29] IEEE 802.111 무선 Belo] 송신단 BEES 나타낸다. 여기서
스트림 파서(606800 081580)부터 성상도 맵핑부(600966111400ㅁ mapper) 사이의 스트림
(stream)2 공간적으로 멀티플렉싱된(60808117 multiplexed) 신호로서 ^/,,개의 스트림이
존재하며, 5180부부터 공간 맵퍼(500881 080080사이의 스트림은 시공간 신호로서 Nos
개의 스트림이 존재한다. 그 이후에는 안테나 개수(#&,)만큼의 스트림이 존재한다. 다음
은 위 기본 블록의 각 부에 대하여 설명한다.

(1) 스크램블러 / 파서 인코더

스크램블러는 888 802.113에서 사용하는 그림 15.2의 스크램블러를 그대로 사용한다.
스크램블된 데이터는 파서 인코더를 통하여 FEC 인코더 개수만큼 분할된다.

(2) 부호화기

IEEE 802.111에서는 FECE 컨볼루션 부호화기와 LDPC 부호화기가 사용된다. 컨볼루

_ 558



===== PAGE 555 =====
제15장_ 1666 802.113/ㅁ

션 부호화기는 85 802.118에서 사용하는 구속장이 7이고 (133, 171)을 갖는 부호
1/2의 부호화기를 사용한다. 보호 구간이 80028 일 때 데이터 전송율이 300Mbps 이상으
MCS(Modulation and Coding Scheme) 레벨이 사용되는 경우를 제외하고는 컨볼루션
호화기가 하나만 사용된다. 또한 HT BAS 사용시 높은 에러 정정 효 때 얻기 위해
볼루션 부호화 대신 LDPCS 옵션으로 사용할 수 있다. 이 때 LDPC 부호을은 수신단
로부터 받은 MCS 레벨에 의해 결정되며, 1/2, 2/3, 3/4, 5/6의 총 4가지 el    사용ㅎ
여 648, 1296, 1944의 길이를 갖는 코드워드를 체계적(69[601800)으로 생성한다.

(3) 스트림 파서
부호화된 데이터 비트를 공간적으로 멀티플렉싱된 스트림의 개수(^, ) 로 분할한다. 분
할 방식은 각 부호화기에 대하여 20000 robin 방식으로 순차적으로 분할한다.

(4) 인터리버

인터리버는 컨볼루션 부호화를 사용한 경우에 한해서 적용되며, 스트림 파서부를 통과
한 신호에 대하여 IEEE 802.118에서와 유사하게 수행된다. 인터리버는 열방향으로 입력
하고 행방향으로 출력하는 것을 기본 구조로 사용하지만 IEEE 802.111의 경우에는 사용
대역폭에 따라서 Bat 열의 길이가 달라진다. 또한 Nos 가 1 이상일 경우 주파수 회전 At
업이 수행된다. 표 15.12는 사용 대역폭에 따른 인터리버의 행과 열의 길이를 나타낸다.
이 때, Noor 은  en  열의 길이, Meow 행의 길이, Neor& 주파수 BAG,
0006 (iss) 는 번째 공간 스트림의 비트 수를 나타낸다.

표 15.12 인터리버 파라미터

16 레 ㅠ 16 to

Neor                                               13                                                 18
Nrow                                 4X Neppss (iss )                           6X Nespss (iss )
ae                                              i                                                 29

트림이 한 개일 경우(^/ㅠㅋ1) 인터리빙은 A} (15.21)과 (15.22)를 이용하여 두
는 JEEE 802.118에서와 유사한 방식이다.

i= Nyow (Kmod Neo, )+ floor(k/ Neo.) 906... (igs )—1       (15.21)

J =8(iss)x floor (i/ 8 (iss )) + (7+ Nespss (iss) — MOOr (Nenpss (iss ))) mod s (iss )

i=0,1,..    0090 (igs) 1

(15.22)

559



===== PAGE 556 =====
PART IV_MIMO—-OFDM 통신 시스템

하나 이상의 공간 스트림 존재시에는 식 (15.23)을 이용하여 주파수 BAS 적용한다.

|) -[(G<-022)metsx tor) eer Nar) %ar  (15.23)

j= 0,1,.-5 Neppss (iss ) 그

(5) STBC

Ss

STBCS 적용할 경우에는 시공간 ABA A Nozs 7b 공간 스트림의 개수(^, )보
다 많아지게 되며, AS 방식으로는 sree hybrid STBC/SM 방식이 사용된다. STBC
가 사용될 경우에는 HT-SIGS] STBC 필드에 표시되며, 성상도 맵핑부 이후와 공간 맵핑

부 이전에 이루어진다. 표 15.13은 시공간 4 ge 개수와 ae 스트림 개수에 따른 STBC
및 hybrid STBC/SM 전송 방식을 보여준다. 여기서, ㆍ “%』,>,/1 는 『 번째 안테나에서
ASE 2m, 2m+1 번째 OFDM 심볼의 번째 부반송파 ASS 각각 나타낸다.

rs  lr

표 15.13 시공간 스트림 개수와 공간 스트림 개수에 ME 전송 방식

d, 1,2m                              d,

1                   >                           k1,2m+1
2               ad. 1,2m+41                  d’, 12m
1                A                     d,. 1,2m+1
8~15
3                        :                2                     1                    2                oe                  re
383 ~38                                                                                k1,2m+1                    12,
3                  K,2,2m                    dy, 2,2m+1
1                 y.2m                      dy, 1,2m+1
2              ad ,. 1,2m+1                 0,
4                8~15                2                    2
3                d,. 2,2m                     d,. 2,2m+1
4              =a, 2,2m+1                 dips 2m
1                  d,. 1,2m                       dq, 1,2m41
16~23, 39                                                                            .                            .
:      ：                                                  2               -d k1,2m+1                d k,1,2m
4              41, 43,               3                     1
46, 48, 50                                                             3                  Ay 2.2m                       Fy > ome
4                di 3.2m                     d, 3,2m+1

960



===== PAGE 557 =====
제15장_16ㄷ6ㄷ 802.113/ㅁ

(a) Nors =2, Noss =1      00 Nsrs =3, Nss                 ST     ,                 ) Nors =4, Nos =3
그림 15.33 시공간

STBCS 통과한 ASL 공간 맵핑부로 입력된다. 이 때 STB 적용되지 않았다면
2

= 가 되고, Nos 229) 경우에는 공간 다중화가 이루어졌음을 의미한다. MCS
레벨에 의해 결정되는 공간 스트림의 개수와 시공간 스트림의 개수의 관계는 9780의 파
라미터에 따라 표 15.14와 같이 주어진다

= 00 080 60 60 NY FY HF
< eS ROL SS eS

if
2
2
8
4
8
4
4

(6) 공간 맵핑

IEEE 802.112의 송신단에서는 성상도 맵핑부의 출력 또는 STBCHS 출력을 회전/확
장 시킨 후 송신한다. 이와 같은 공간 맵핑은 안테나의 개수가 시공간 스트림의 개수보다
많을 때(^/,,<ㅅ,,) 수행된다. 공간 맵핑 시 CSD(Cyclic Shift Diversity)7} 적용될 수

@)

있으며, 공간 맵핑 행렬(0), 2 다음과 같이 3가지로 BRS 수 있다.
첫째, 직접 YB direct mapping) 방식은 단위 크기로 이루어진 복소수를 원소로 갖는
대각행렬 Q, 를 통해 이루어지며 다음과 같이 구분할 수 있다.
1) Q 는 단위행렬로서 아무런 AGE 이루어지지 않는다(0, =1).
2) Q, = AAAS] CSDS 주파수 영역에서 수행하는 행렬이다. 따라서

Q, = diag(exp(—j2#kA ,Tesp)) 로 이루어진 대각행렬이고, 이를 Mea (k) 로 정의한다.



===== PAGE 558 =====
PART IV_MIMO-OFDM 통신 시스템

둘째, 공간 확장(608081 expansion) 방식은 CSD YS(Mesp(k) )과 정방 BA(square
matrix)°] 곱으로 이루어지며, 시공간 스트림이 행렬 연산에 의해 공간으로 확장된다. 공
간 확장 방식은 다음의 3가지 경우로 구분할 수 있다.
1) @, 는 CSD 행렬과 26000108을 위한 Hardamard 혹은 『004@ 행렬의 곱으로 이루어
진다.
2) Q, 는 CSD YAM esp (k) )에 DBAS 곱하여 0, =14.65(4)ㆍ로 표현되며, 여기
서 DYAS 같은 시공간 스트림이 복사하여 여러 안테나로 확장하는 역할을 한다. 이
때 전체 전력을 정규화 하기 위해 4) ">, 를 곱한다. 0 행렬은 안테나 개수와 시공간
스트림의 개수에 따라 다음과 같이 주어진다.

.                1
i) Noy =2s Nors =], D=—-ll 00

..           1    T
ii) Ny =3, Noy =1, D=—[I 1 1
TX   STS    al   ]
10242 =4, Nos =] 0=그[1 1 1 ay
0
.           2
Iv) Npy =3, Nor =2, D= 3 0 1
1 0
[1 07
v) Nyy =4; Nery =2 i
TX  ? STS  ?   ft 1 0
10 1
1 0 Oy
.          4310 1 0
vi) Nx =2, Nos =3 D=~=! 9 ,
11 0 0

아래의 공간 확장 YAS HT mixed BWW 적용된다. Q, 행렬은 송신 안테나의 개
수와 공간 스트림의 개수에 따라 다음과 같이 주어진다.

562



===== PAGE 559 =====
제15장 166ㄷ 802.113/ㅁ

7

i) Ny =2, Nos =1, Q,=[1 이 또는[0 1]

1 0] |1 0]  0 0
ii) Ny =3, Ngs =2, Q,=/0 0|,/0 1|또는1 0
1 0} [0 0|   0 1
1 0] |1 0| [0 0   0 0
= =           0 0  0 0  1 0 = 1 0
00 00 oe 서위 = of lo it lo ol “la 1
0 1] [001 [01   0 0
1 0 0   1] 0 0
.            0 1 0}, |0 0 0
Iv) Niy =4, Nos =4, 0, = 000 Leen 010
0 0 1   0 0 1
셋째, 빔형성 행렬은 수신단의 성능 향상을 위해 사용된다. 빔형성을 하기 위해 송신단
ㅋ

=
해진 Q, = Greenfield SMo]A] 패킷의 모든 부분과 HT mixed 440]4] HT-STF Field
를 포함한 이후의 패킷의 모든 부분에 적용된다.

(7) Pilot 부반송파

IEEE 802.117에서는 IEEE 802.113에서와 같이 잔류 위상 추적용으로 Tayelo] 사용
된다. 20MHz 대역폭을 사용할 경우에는 Al (15.24)에 나타난 바와 같이 -21, -7, 7, 21
번째 부반송파 4개에 spaelo] 사용된다.

0,0,0,0,0,0,0,0,0,0,0,0, #0"?

(n+1)®4?

PS = {0,0,0,0,0,0,0,¥("")                  0,0,0,0,0,0,0

(ists                               n@4?
(15.24)

0,0,0,0,0,0, #0"?   0,0,0,0,0,0,0,0,0,0,0,0, #0)

n+2)®4?                                                    (n+3)84?

0,0,0,0,0,0,0}

40Mhz 대역폭을 사용할 경우에는 식 (15.24)에 나타난 바와 같이 -53, -25, -11, 11,
25, 53번째 부반송파 6개에 welalo] 사용된다.

= {0,0,0,0,0, ¥ ir.  0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0

(ists                                   206:

0,0, 80) .4.0,0,0,0,0,0,0,0,0,0,0,0,0, ¥\"")_..,.,,0,0,0,0,0,0,0,0,0
(15.25)
0,0,0,0,0,0,0,0,0,0,0,0, ¥("""), ..,,,0,0,0,0,0,0,0,0,0,0,0,0,0, FO) .  ,
0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, (=) ..,,0,0,0,0,0}
563


===== PAGE 560 =====
표 15.15는 각 시공간 스트림에서의 spe ge WG) 을 나타낸다.

표 15.15 각 시공간 스트림에서의 Dad Zt

(a) 20MHz 대역폭              —  (b) 40MHz 대역폭

1       1        1        1        1        =         1       1        it         1         1         은 |        =!         1
2       1        1        1        sik       =i         2       1        1         1         ak        il        그        들
2       2        1        =]       =}        1          2       2        1         =         iL         a1         a         1
3       1        1        1        때       =)         3       1        1         1         =        ak        al        =
3       2        al        cal        i        =i         3       2        1          1         1         ~.         1         1
8       3       rel        1        1        ls         3       3        1         ak         1         =i        =         1
4       1        1        1        1        =i         4       1        1         1         =        ie        ne        ol
4       2        1        1        =        1          4       2        1         1         1         is         1         1
4       3        1        =I        1        1          4       3        1         Bal         1         al        asl         1
4       4       ral        1        1        1          4       4        그         1          1         elk         1

Non-HT [SISO case(802.1 1a/a)]
8us                  808              448

2681          L-LTF 806

HT mixed format         [호환성이 있는 MIMO]                          Data HT-LTFs

Extension HT-LTFs

8us              8us           4us         8us         4us        4us per LTF           4us per LTF
me     =    o    sa   시 미드. = 1 00 Will
L-STF | L-LIF |L-SIG] HT-SIG | ore] ret | Cre] re

HT greenfield format [호환성이 없는 MIMO] DataHT-LTFs — Extension HT-LTFs
8us               8us              808             4us per LTF            4us per LTF
—— 으으 ~ 르르

    :     -gig | HT=]... HT=THT-]... [AT
HI-GE-SIF} HI-FI 으라 (i)... | 때

그림 15.34 IEEE 802.117 프레임 구조



===== PAGE 561 =====
제15장_ 1666 802.113/ㅁ

SEP) IEEE 802.117 프레임 구조

그림 15.34는 IEEE 802.11n2] PLCP(Physical Layer Convergence Procedure) 프레임
PAS 보여준다. Non—HT 2%, HT Mixed £4, sGreenfield Z™2] 3가지 PES] 프레
임 moO ge 구성된다. Non—HT 4-2 IEEE 802.118를 사용하고 있는 단말과의 완벽한
호환을 위한 SISO 프레임 구조이다. HT mixed 242 L—STF(Legacy Short Training
Field) 부터 L—SIG(Legacy 918081)까지 Non—HT 7} 동일하므로 IEEE 802.1la 단말
은 그 뒤에 오는 데이터를 수신할 수 있고, L-SIG 다음에 오는 HT-SIGHES 이용하여
IEEE 802.117 단말은 Mixed ¥™]-& 판단할 수 있다. Greenfield EHC IEEE 802.1 1a/g
단말과 호환성이 없는 BMOS IEEE 802.112 단말만 수신할 수 있다.

(1) L-STF 프리앰블

Ｌ-9깨는 IEEE 802.118에서 사용하였던 짧은 훈련신호와 동일하며 AGC, 타이밍 동
기화, 대략적인 주파수 동기화를 하기 위해 사용된다. 40540의 대역폭을 사용할 경우
20Mhz 대역에서 사용하였던 프리앰블을 기반으로, PAPRE] 감소를 위해 90* 위상희전을
하여 확장한다.

S 46.06 = V1/2{0,0,1+ j,0,0,0,-1— j,0,0,0,1+ ,0,0,0,-1— /,0,0,0,-1— j,0,0,0,1+ /,

(15.26)
0,0,0,0,0,0,0,-1— 7,0,0,0,—-1— j,0,0,0,1+ 7,0,0,0,1 + /,0,0,0,1+ 7,0,0,0,1+ 7,0,0}

S sgsg = V1/2{0,0,1+4 7,0,0,0,-1— j,0,0,0,1+ j,0,0,0,—-1— j,0,0,0,—-1— /,0,0,0,1+ 7,0,
0,0,0,0,0,0,—1— j,0,0,0,-1— j,0,0,0,1+ /,0,0,0,1+ /,0,0,0,1+ 7,0,0,0,1+ /,0,0,0,0,0
0,0,0,0,0,0,0,0,0,0, ;-1,0,0,0,—j+1,0,0,0, 7 -1,0,0,0,—/+1,0,0,0,-7 +1,0,0,0, j—
0,0,0,0,0,0,0,—j +1,0,0,0,—/ +1,0,0,0, ;-1,0,0,0, —1,0,0,0, j—1,0,0,0, 7—1,0,0}

| (15.27)

(2) L-LTF 프리앰블

L-LTF& IEEE 802.118에서 사용하였던 긴 훈련신호와
정과 채널 추정에 사용된다. 40Mhz2] ASS 사용할 경
위상회전을 통해 확장한다.

일하며 미세 주파수 옵셋 추

동
우, PAPRS| 감소를 위해 90°

26 ={1,1,-1, 14. 그1. 1. 1.1.1. 1111.11 111 4. 1 1 1 1 1 1 0

(15.28)
9000.19 0011.41 enone

565


===== PAGE 562 =====
PART IV_MIMO-OFDM 통신 시스템

해 = {1,1,-1,-1,1,1,-1,1,-1,1,1,1,1,1,1,-1,-1,1,1,-1,1,-1,1,1,1,1,01,-L-1,
L1-L1,—-1,1,-1,-1,-1,-L-L1L-L-11,-L1L—-L1L1L11,0,0,0,0,,0,0,0,0;.0,

Tears rar rer ee  (15.29)
0,0,0;0), 559s —J Is Js Iss s—JoI J oJ sds Is—J sIsJs—JsJ Jods J 75 0
(3) L-SIG

L-SIGE 데이터 ASHI} 데이터의 길이에 대한 정보를 포함하고 있다. HT mixed 포
맺에서의 L—-SIG2] 경우 As (Rate) 6Mbps= 고정하고 Length Fieldo] 실제 프레임
의 길이에 해당하는 값을 넣음으로써 1686 802.118.8 단말들이 mixed ZW 프레임을 수
신하였을 경우 Ｌ-810까지 디코딩이 가능하다.

Rate                                               Length                                                    Tail
(4 bits)                                          (12 bits)                                               (6 bits)

ORS OL Oe Oe or 0ns re:
o[sfe|s 4 s[e|7]e]e iol] re|is]r[ ss | 16 Ty: 18 | 19 | 20 | a1 | 22 | 23

그림 15.35 L-SIG2| 비트 구성

다중 안테나 사용시, L-STF, L-LTF, L-SIGS: 포함하는 Non-HT 11610에 의도하지
않은 빔형성 AAS 발생하는 것을 막기 위해 CSD(Cyclic Shift Diversity) 기법을 사용한
다. CSD 기법에서는 OStsT 구간 동안 송신 신호 50) 를 식 (15.30)에서와 같이 Tes
만큼 CS(Cyclic Shift) 한다.

' =| s(t -—T 5)    0<r< 7, +i          00
에    5(00-76 127) 1227 + Tes 주             |

여기서 Tes <0이다. HE 15.16은 각 송신 안테나에서 패킷의 non-HT 부분에 적용되는
CS HS 보여준다. Legay 부분을 다중 안테나로 전송할 경우, 이 부분은 IEEE
802.113/8 단말 들이 수신하는 신호이므로 TL, 를 200 ns 이하로 제한한다.

ㄴㄴ



===== PAGE 563 =====
제15장 IEEE 802 11a/n

그림 15.36은 시간영역에서의 CSD} 주파수 영역에서의 CSD AAS 보여준다.

| 이 =] sy sa] ~    | sw] 8047)                                               X(f)
| 4 sa | say] ~    | S(N- 이  =                     i        X(f)exp(—j22T,5f/ N)) i     ‘gt     T
[swf 50| sc] …   | 해이 |                              X(f)exp(— saawen. sin

(a) 시간 AS CSD                        (b) 주파수 BA CSD

그림 15.36 IEEE 802,11n0l] 사용되는 CSD 개요

그럼 15. ieee  각 안테나에서 송신하는 신호가 같거나 비슷한 BH (s(t) = s(t)) 위상

널을 통과하게 되면 수신신호  i 상쇄되어 00] 되는 현상을 보여주며, CSD

키법을 적용할 경우 이 문제를 해결할 수 있다. 또한, 각 송신 안테나에서 다른 크기의 CS

를 적용함으로써 수신신호는 지연된 송신신호의 Gee 표   이는 송신신호가 가상

적으로 많은 탭을 가진 ASS 통과한 형태가 된다. 결과적으로, CSDS 사용하면 송신신

호가 겪은 AAS CSDS 사용하지 않은 경우보다 주파수 선택성이 커지게 되고, 채널 부
호화와 인터리버 결합시 향상된 주파수 다이버시티 효과를 얻게 된다.

그림 15.37 의도하지 않은 빔형성의 예

567



===== PAGE 564 =====
PART IV_MIMO-OFDM 통신 A

(4) HT-SIG

;
pe

HT-SIGE HT 패킷을 전송하는
HT-SIG2] 비트 구성을 보여준

경우에 그에 대한 정보를 전달

한다. 그림 15.30은

그림 15.38 HT-SIG2] 비트 구성

Fa
MCS     g         HT Length
N
LSB       MSB  LSB                   MSB
ofifz|safals|s f 8 | 9 | 10[ 1] 12] 19] 14] 15 | 16] 17 | 18 | 19 | 20 | 21 | 22 | 29
(a) HT-SIG1
jong
Ke)
a
을
ol(Slels    2) | 35               cos
2/Pisls    8 _ | ss      CRC         Signal tail
= [2 | is     06 G2
8 B/s1¢  oO  Ole 은꼴
Eels 8 3  a  5 2 58
OD (tet | Oe et  no  = | Zo 7         00
0 1 2 3 a|s 6 7 8|9 1o[ 11 | 12] 19] 14] 15 | 16 17 18 19| 20 | 21 | 22| 28
(b) HT—SIG2

HT-SIGE HT-SIG13} HT-SIG29] 2개의 부분으로 구성되어 있다. 각각 24비트로
구성되어 있으며, Ｌ90의 Al 번째 비트가 가장 먼저 매개 HT-SIG= Ｌ-910와는 다

르게 90° 만큼 회전된 829로 전송된다. 따라서 이 부분

의 신호 전력비를 이용하여
임인지를 구분할 수 있다.

LSIG 44]

＊ㅇ

분에서 IEEE 802.117 단말은 10

수신된 신호가 legacy(non—HT) 프레임인지 mixed 모드 프레

'
=

4A +

Les

HT-SIG 44 4

그림 15.39 L-SIG2} HT—-SIG2| BPSK 성상도


===== PAGE 565 =====
제15장_ 1666 802.11a/n

(5) HT-STF 프리앰블

HT-STF 프리앰블은 mixed Zo] AGCS] 성능 향상 또는 미세 AGCS 위해 사용
되거나, Green Field 포맺에서 AGC, 타이밍 동기화, 대략적인 주파수 동기화를 위해 사용
된다. 전체 길이는 dus L-STF 프리앰블과 동일하나, 순환 지연(2016 Delay) 같은 다

Space = 1/2 {0,0,0,0,1+ j,0,0,0,—1— 7,0,0,0,1+ 7,0,0,0,-1— j,0,0,0,—1— j,0,0,0,1+ /,  15.44
0,0,0,0,0,0,0,—1—,0,0,0,-1— j,0,0,0,1+ j,0,0,0,1+ j,0,0,0,1+ j,0,0,0,1+ 7,0,0,0,0} meet)
0,0,0,0,0,0,—1—7,0,0,0,—-1—7,0,0,0,1+ 7,0,0,0,1+ 7,0,0,0,1+ 7,0,0,0,1+ 7,0,0,0,0,0  (15.32)

0,0,0,0,0,0,0,0,0,0, 7 -1,0,0,0,—7 +1,0,0,0, 7 -—1,0,0,0,—7 +1,0,0,0,—7 +1,0,0,0, 7-1
0,0,0,0,0,0,0,—j +1,0,0,0,—j +1,0,0,0, 7 -1,0,0,0, 7 -1,0,0,0, 7 -—1,0,0,0, 7 -1,0,0}

(6) HT-LTF 프리앰블

HT-LTF 프리앰블은 각 안테나별로 MIMO 채널 추정과 미세 CFO 28S 하기 위하
여 사용된다. 시공간 스트림의 개수만큼 채널을 추정해야하기 때문에 시공간 스트림의 수
에 따라 47-Ｌ깨의 개수도 증가한다.

소아 개 러바이태가 히뢰제나허제우 1가허가 개

(15.33)
1,-1,1,1,-1,-1,1,-1,-1,-1,-1,-1,,-1,-1,-L1-1.1,11,1,-L-]}

Lsg5¢ ={1,1,-1,-1,1,1,-1,1,-1,1,L1,1,1,1,-1,-1,1,1,-L—1,1,],1,1,01,-L-1,
01106 a a oe   11-151 1.1,1,0,0,0,0,0,0,0,0,0,

(15.34)

그가

다중 안테나 사용시, HT-STF, HT-LTF, HT-SIGS 포함하는 47 81600에 의도하지

않은 빔형성이 되는 것을 방지하기 위해 CSD 기법을 적용한다. 데이터 부분에서도 같은
Tes 를 사용하여 CSD 기법을 적용한다. 표 15.17은 패킷의 HT 부분에 적용되는 각 시공
스트림별 7, 값을 보여준다. 076601610 EW] 프리앰블 및 데이터 영역에서도 =
5.17에 주어진 CS 값을 적용한다.

구

—

569 —



===== PAGE 566 =====
스텐
—o

PART IV_MIMO-OFDM 통신 시

표 15.17 패킷의 HT 부분을 위한 Cs 값

1             Ons             =

2             0 ns          —400 ns           =              =

8             0 ns          -400 ns        —200 ns           =

4             0 28          -400 ns        -200 ns        —600 ns

570



===== PAGE 567 =====
지상파 디지털 오디오 및 비디오 방송 시스템은 크게 유럽의 DAB(Digital Audio
Broadcasting)?+ DVB(Digital Video Broadcasting) 방식, 미국의 IBOC(In Band On
Channel)?} IBAC(In Band Adjacent Channel) 방식, 244°] ISDB—T(Integrated Services
Digital Broadcasting—Terrestrial) 방식으로 BES 수 있다. 최초의 디지털 라디오 방송
을 위한 유럽의 DAB 방식은 847668-147 프로젝트를 시작으로 1997년 2월에 최종 표준
으로 확정되었다[302]-[3051]. 특히 우리 나라에서는 DAB 방식을 기반으로 세계 최초로
고품질의 음성 및 영상서비스를 언제 어디서나 제공할 수 있는 이동 멀티미디어 방송으로
발전시켜 “듣는 방송'에서 “보고 SS BE LS 확장한 지상파 디지털 멀터미디어 방송
(Terrestrial—Digital Multimedia Broadcasting; T-DMB)& 채택하였다. 또한, 유럽의 지
상파 디지털 TV 전송 방식으로 DVB-T(Digital Video Broadcasting-Terrestrial)?}+
DVB-—H(Digital Video Broadcasting-Handheld terminals)7} 있다[306]-[311]. T-DMB,
DVB-T, DVB-HoAJ= 모두 다중 경로 페이딩 영향에 강건하고 SFN(Single Frequency
Network) 구축이 가능한 OFDM 방식을 사용한다.

CRAY DMB 시스템의 개요

T—DMB(°]|s} DMB) 시스템은 유럽의 Eureka—147 DAB 규격에 기반을 두고 있다.
Eureka—147 DAB 시스템은 11811 System ㅅ로도 불리며, ITU-ROA, 초단파/극초단파



===== PAGE 568 =====
PART IV_MIMO-OFDM 통신 시스템

대 지상파 및 위성 디지털 음성 방송으로 이를 차량용, 휴대용, 고정 수신용으로 권고하고
있다. Eureka-147 프로젝트는 1986년 프랑스             5                톡
홀름 유럽 연맹 각료 회의에서 결정되었으며, 1988년부터 실질적인 활동이 시작되었다.
DAB 표준화는 EBU(European Broadcasting Union)2} ETSI7} 협력하여 조직한 기술분
과위원회 주관으로 1991년까지 1 단계로 기본적인 시스템 개발이 이루어졌으며, 1992년
부터 1994년까지 2 단계 개발이 추진되어 1994년 1월에 초안(8678 300 401)이 작성되었
고, 그 후 3년 뒤인 1997년 2월에 2 판이 발표되었으며, 2001년 5월에 최종 표준안이 완
성되었다.

Eureka—147 방식은 음성 부호화 방식으로 고효율 음성 부호화인 MPEG-2, 디지털 변
조방식으로 지상파에서 다중 경로
대역폭을 사용하여 단일 송신기로 고음질의 스테레오 프로그램과 데이터를 다중화하여 방
송한다. 이 때 가능한 프로그램 수는 비트율, HSS, 데이터 용량 등에 의하여 결정되는
데, 비트율이 192 Kbpso]at 부호율이 0.5일 경우 약 6개의 프로그램을 동시에 방송할 수
있다. 수신도 간단한 whip 안테나로 가능하며 도심지와 같이 다중 경로가 많은 환경에서
도 우수한 성능을 갖는다. DMB 방식에서는 위의 DAB 시스템의 기본 기능 외에, DAB
스트림 모드 데이터 채널을 통해 비디오 서비스 신호를 전송하기 위해 MPEG-2 TS
(Transport Stream)S 사용하고, H.264 비디오 부호화 및 BSAC(Bit Sliced Arithmetic
Coding) 오디오 부호화 기술을 사용한다.

le}

Eureka—147 DAB 시스템의 송-수신 기본 블록도가 그림 16.13} 그림 16.20] 각각 주
어져 있다. 그림 16.1의 송신기 블록도를 보면 각각의 사운드 서비스 신호는 개별적으로
오디오 부호화기를 거친 후 오류방지를 위하여 부호화된 후 시간영역 인터리버를 거친다
인터리빙된 각각의 사운드 서비스 신호들과 데이터 서비스 신호들은 다중화되어 MCS
(Main Service Channel)= 합쳐진다. 다중화된 신호는 FIC(Fast Information Channel) =
전송되는 MIC(Multiplex Configuration Information)2} Sl(Service Information)2} 함께
주파수 인터리버를 통과한다. 이 때 FICS 전송되는 정보는 시간 지연을 혀용하지 않기
때문에 시간영역 인터리버를 통과하지 않는다. 주파수 인터리빙된 비트열은 DQPSK 심볼
로 변조된 후 117를 통해 OFDM ABE 변환된다. 여기에 동기화를 위한 심볼이 부가되
어 최종적으로 DAB 신호가 발생된다.

572


===== PAGE 569 =====
제16장_미/86/ㅁ0'/8 시스템

ni                                        7                                                                                              대
브이                 audio                     channel                       time
N                   encoder                   encoder                 interleaver
other
services

cl                  data                      channel                  :    time
M                   encoder                   encoder                 interleaver
other
services

services                          MUX
configuration                controller

그림 16.1 Eureka-147 DAB 송신기의 블록도

sync
generator
OFDM     > ld
signal

frequency
interleaver
A

FIC
generator

7  ae         A/D          DFT and.       T/F de-interleaving         audio | 01
conversion        demodulator        and error correction        decoder ㄴ~ R
《           i             t                A               A
t             +
user |, || control and                                          | ㅣ data              dala
interface |     synchronization                    decoder    SEIVIGES

그림 16.2 Eureka-147 DAB 수신기의 블록도

그림 16.2는 DAB 수신기의 구성을 보여준다. 튜너를 통해 원하는 DAB 방송 신호
선택하고 동기화를 wet  음 ADCS 9 디지털 신호를 생성한다. 이렇거

호                  를 통과한 후 시간 영역과 주파수 BA
신된 데이터를 복원하면 최종적으로 오디오 신호와
오를 MPEG 복호 처리를 하면 좌우 신호가 분리된다.
수신 eo chet 지어는 FIC 기네 따라 수행된다.

Eureka—147 전송 FAS 지상 단일 주파수 방송망(614) WE Ｌ I, WS 사용하여 지
상파 방송에 적합한 전송 모드 Ｌ WE L IL 11, IV, \와 Ｌ 밴드에서 적합한 전송 모드
II} IV, 3 GHz 이하의 지상파 방송, 위성 방송, 케이블, 지상 및 위성방송에 적합한 전송
모드 IN9| 4가지 전송 모드로 구성된다. AS 프레임에는 1차 동기용 Null HES 선두로
하여 동기화 채널과 FIC7} 이어지며 다음에 MSC7} 할당된다. 데이터 전송은 FICS}
MSC# 이루어지는데, FICE 256 4|E FIB(Fast Information Block)= 구성되며 MSC
배열을 제어한다. 제어 정보의 핵심은 FICS 통해 전송되는 \/1인데 이에 따라 MSC7}
배열된다. 각 전송 BE] 따른 주요 파라미터는 표 16.1에 주어져 있다. 전송 프레임 지
속기간은 표 16.1에 나타난 바와 같이 전송 모드에 따라서 96 ms~24 0ㅁ8의 값을 갖는다.
전송 모드 [은 많은 수의 반송파를 조밀하게 배치하여 주파수 인터리빙 효과를 극대화하
고, 심볼 구간을 길게 함으로써 허용 가능한 다중경로 전파의 지연시간을 길게 하여 단일



===== PAGE 570 =====
16.) Eureka-147 전송 모드 파라미터

지상파(89854) 지상파/위성    위성/케이블 지상Ｌ-밴드)
375 MHz 이하 1,5 GHz 이하 3 082이하 _ 1.5 GHz 이하

1,536          384           192           768

1 kHz         4 kHz         8 kHz         2 kHz

246 us         62 us         831 us         123 us

1 ms         250 us        125 us        500 us

96 ms         24 ms         24 ms         48 ms
DQPSK

Convolutional : Variable rate, constraint length = 7
Depth = 384 ms
Width = 1,536 MHz
0,8~1,7 MHz
1,536 MHz

주파수 방송망에 적합하게 설계되었으나, 사용가능한 주파수 YAS 375 MHz7}|= 제
한된다. 전송 모드 MNS 반송파 간격을 넓게 하여 도플러 주파수의 허용치를 크게 하고 반
송파 주파수를 3 0412까지 확장한다. 국내 DMB 시스템에서는 전송 모드 [만을 사용하기
때문에 본 절에서는 전송 모드 [을 기준으로 DMB 시스템을 설명한다.

DMB 시스템은 현재까지 기술한 DAB 시스템의 기본 기능에 MPEG-2 TSS 사용하고,
H.264 비디오 부호화 및 BSAC 오디오 부호화 기술을 적용한 것이다. 즉, 그림 16.3에 나
타난 바와 같이 MPEG—4 규격의 콘텐츠를 MPEC-2 TSS 이용하여 DAB 전송 채널로

| avne |           다중화 규격            | 전송/채널 규격 ㅣ BAD Adaptation |
Video source       jest es     MPEG-4 |           Video SUP

1999     Video ES          OD/BiFs SIA                            ^               2)
Encoder                                가데이터 BLP                                    o                      ©

-                                                  그
. ~        100                     z            6
Audio source            fi        ideo ES                                                        6                  으
Audio                 Ss                                   30       는                 드
Encoder              zo                             2       =    System     o
부가데이터               을                 TS           믹 | JS || moe) | 3
(정지영상 S-———-+4 §               Mux        을      므            a

s                                   을       =
OD/BIFS                                                   을        에                &

g
Generator                                                            =                g
2                 QD
<                 a
10D                                                               ®                 @Q
Generato                                                                               그

그림 16.3 DMB 송신기의 블록도



===== PAGE 571 =====
제16장 DMB/DVB 시스템

전송하는 구조이다. 일반적으로 동영상 서비스는 10° 이하의 BER 성능이 요구되나
Eureka—147 DAB 시스템은 오디오 서비스를 위하여 BERS] 10 “을 목표로 설계가 되었
기 때문에 그림 16.3에 나타난 바와 같이 RS 부호화기와 컨볼루셔널 인터리버가 DMB
시스템에 추가되었다.

AGP] DMB 전송 프레임 구조

그림 16.4는 전송 모드 1의 프레임 구조를 보여줄다. 전송 프레임의 첫 부분에는 Nall
심볼이 할당되며, 00009 변ㆍ복조를 위한 PRS(Phase Reference Symbol)2] 동기화 채
널이 이어진다. 다음으로 『10가 할당되고 나머지 부분에 오디오 데이터와 일반 데이터를
전송하는 MSC7} 할당된다. OFDM 심볼은 1 08의 유효 데이터 구간과 0.25 ms 길이의
보호구간으로 구성된다. 따라서 하나의 전송 프레임은 그림 16.4에 나타난 바와 같이 Null
심볼, PRS, FICS 심볼 3개, MSCS} 실제 데이터용 심볼 72개로 구성되며 전체 길이는
96 ms7} 된다. 데이터 전송은 FICS} MSCH 통하여 이루어지며, FICE 다수의 FIBQSO 비
트 단위)로 구성되어 MSC was 제어한다. MSCE 여러 개의 CIF(Common Interleaved
Frame) ©. 구성되고 하나의 CIFE 55,296 비트로 구성되는데, 이는 24 ms 구간의 오디
오 프레임에 해당된다. CIF] 최소 주소 단위는 64 비트로 구성되는데, 이를 CUCapacity
Unit) 라고 한다. 서브채널은 CU} 정수배로 구성되며 MSC] 기본 전송단위가 된다. 즉,
MSCE 서브채널을 다중화하여 구성되며 시간 인터리빙되고 채널 부호화된다. 각 서브채
Be 한 개 이상의 서비스 성분을 나타내며 서비스 성분과 서브채널이 결합하여 다중화
배열이 된다.

Transmission Frame

Synchro-       Fast
nization         Information
Channel         Channel (FIC)

3 Symbols                                    72 Symbols (Mode |)

(Mode | )
2                    ㅣ                eee eee
| _ Phase Reference Symbol        OS

Null Symbol

Main Service Channel
(MSC)

Guard Interval

그림 16.4 전송 모드 19] 프레임 구조

575


===== PAGE 572 =====
PART IV_MIMO-OFDM 통신 시스템

표 16.2 전송 모드에 따른 파라미터

비          196,608 T,  49,1527,  49,1527,  98,3047,
e          96ms   24ms   24ms   48ms
=          2,656 Ts   6647,   345 T,   1,3287,
에         12977   324 ps   16866   64876
r          2,552T,   6387,   31927;   1,276T,
as          1,246ps   312s   156 ps   623 us
주          2,048 T;   512T,   2567;   10247,
=          ims   25076   12576   500ps
r          5047;   1267,   637,   2522
          246 us   62766   31719   123s

 DMB 물리계층 규격
(1)

저수
전송

기

Al (Main Signal)
레임은 연속된 OFDM 심볼로 구성되며, 송신 신호 ×0) 는 다음과 같이 정의된다.

별

K/2

x)= Ree" 가게 pa  X[k 8, (¢- mT. — Ty, — (1-1) Ty)   (16.1)

여기서

=                                      for /=0
8) =  el AHA) Tos Rect (1/T,,, )  for ]=1,2,---,L                    (16.2)
Eon aL

sym            sub

+r.

또한 X[k] = m    4 프레임의 /번째 OFDM 심볼의 *번째 부반송파에서
DQPSK 변조된 복소 심볼을 나타낸다. 나머지 파라미터는 표 16.2에 정의되어 있다. 표
16.2에서 7;는 샘플 주기를 나타내며, 1/2,048,000초이다.

pe
a
en

576


===== PAGE 573 =====
제16장_ DMB/DVB 시스템

(2) 동기 8 (Synchronization Channel)

동기 HAS 그림 16.5] 나타난 바와 같이 Null 심볼과 PRSS 이루어진다. Null 심볼
은 전송 프레임의 앞에 위치하며, 시간 간격 [0,7 yu] 동안 ×0)=0 이다. PRS ㅅ,[4]은
다음에 전송되는 OFDM 심볼의 DQPSK 변조를 위한 기준 위상이 되며, 다음과 같이 정
된다.

|

atc)

067“ — for  <p eWend 0<#<즈
조[]1=           2               2             (16.3)

0 tor k=0

여기서 g, ={0,2/2,,32/2} 이다.

Synchronization Channel

Guard
Null Symbol                 Interval         Phase Reference Symbol
7                   1.297 ms                    | 246us |                     1 ms                     -
(Mode 1)                  (Mode 1)               (Mode 1)

그림 16.5 동기 채널의 구조

(3) 시간 기준(1106 Reference)

동기 WAS FICS 전달하는 시간 정보에 대한 기준, 즉 시간 기준의 역할을 수행한다.
FICA] 전달하는 시간 BRE 전송 프레임에 있는 Null 심벌의 시작 시점을 기준으로 하
여 이루어진다.

(4) 채널 부호화

DMB 시스템의 채널 부호화기 구조는 그림 16.6에 나타난 바와 같이 기존 Eureka—147
DAB 시스템에 outer 코드로 RS 코드와 컨볼루셔널 인터리버가 추가되었다. 2808에 A}
용되는 RS 부호화기는 9410ㅁ6060 RS(204, 188, t=8) 부호화기를 사용한다. 컨볼루셔널 인
터리버는 12개의 branchS 가지고 있으며, 컨볼루셔널 인터리빙된 신호는 807668-147
DAB 시스템에 입력된다. AS 신호의 에너지를 확산시키기 위해 PRBS(Pseudo Random
Binary Sequence) ASS 가하며, 이 때 생성 다항식은 2(0)=ㅅ^"+ㅅ”+1이 사용된다.
타는 『18(『6891 Information Block)"}t}, MSCE 각 채널마다 PRBS 신호가 가산된다.

577


===== PAGE 574 =====
PART IV_MIMO-OFDM 통신 시스템

FICO MIC(Multiplex Configuration Information)2} 수신기의 디스플레이 표시용 데이
터와 제어용 데이터를 전송하는 91(96270106 Information), CA(Conditional Access) 관리
정보, FIDC(Fast Information Data Channel)7} 있다.

Outer coder

Eureka 47
DAB system

cow 다 eae woe ees ame d

그림 16.6 DMB 시스템의 채널 부호화기 구조

#163 보호 수준과 부호율

1 very high        special         0,34-0,36         8/32         8/25-8/28  8/19-8/22
2            high           mobile high 0,40-0,48        8/30-8/32  8/20-8/26 8/16-8/17
3           high                mobile             0.50051        8/23-8/24  8/16-8/18  8/14—-8/15
4     medium mobile weak 0,57-0,62     8/17-8/01 _ 8/14-8/17  8/10~-8/18
5      low         cable       0.72-0.75  8/18-8/16 8/11-8/14      8/10

Punctured 컨볼루셔널 PEL 부호화기를 사용하여 22 9(mother 0006)를 생성한 후,
모부호에서 실제로 전송할 ES 선정하는 방법(6040004008)으로 부호율을 가변한다. 부
호화기의 구속장 길이는 7이고, 유효 데이터와 모부호의 비가 1:4인 컨볼루셔널 부호화기
를 사용하며, 부호율은 8/9에서 8/32까지 24 단계로 조정할 수 있다. 이 때 중요도가 높은
부분은 적게 삭제하고 중요도가 낮은 부분은 많이 삭제하는 처리가 이루어진다. 모든 부
He 동등하게 27000000108하는 방법을 EEP(Equal Error 『*ㅁ0[60000)이라고 하고, 중요도에
따라 puncturingS 다르게 하는 YH UEP(Unequal Error Protection)°]e}31 한다. 부호
율은 데이터 비트수와 부호화 후의 비트수의 비로 나타내며 가장 성능이 우수한 보호 수
준(『#\70660010ㅁ Level) 1의 경우 부호율이 oF 0.34이고, 가장 성능이 낮은 보호 수준 5의 경

578



===== PAGE 575 =====
A162. DMB/DVB 시스템

우 HESS 0.757} 된다. 케이블 네트워크에서는 더   호율이 사용되며, 라디오 채널에
서는 채널 특성에 따라 낮은 부호율이 사용된다. 또한 음악 방송에서는 보호 수준을 높게
하고, 음성신호 전송시에서는 보호 FES 낮게 하는 등 오디오 서비스 내용에 따라 부호
율이 다르게 선택된다.

일반 데이터의 오류정정은 비트 단위인 논리 프레임을 4개의 클래스(01859)로 나누고 여
기에 부호을이 0.25에서 0.75까지인 24개의 puncturing 벡터를 적절히 적용하여 이루어진
다. FICE 전송되는 서비스와 오디오 프로그램 정보의 경우는 모두 1/3로 부호화된다. 표
16.3은 각 보호 수준에 따른 부호율을 보여준다.

(5) DQPSK 심볼 변조 및 BER
DQPSK HAE 다음과 같이 정의된다.

X[k] =X, [KIC [A]                                                       (16.4)
여기서 Clk] = /번째 ASO] 번째 부반송파에서 QPSK 심볼 변조된 신호이며, 신호

는 7/4-shift DOPSK 방식으로 변조된다.
이론적인 DQPSK 변조 방식의 BER 성능은 다음과 같다.

26
2:   !  erfe   S sin| | ||}, 2 24          (16.5)
log, M            No           2M

1€-002

1E-003

BER

1E-004

1E-005

1€-006

—©— simulation results(without virtual carrier) |

—©— simulation results(with virtual carrier) |

T       Tt       Tt       ice       (a (a       ‘ia

0              ie              4              6              8             10            12            14
Eb/NO

그림 16.7 DQPSK 변조 방식의 BER

!                 __ AWGN
—— analytic values

1E-007

579 _



===== PAGE 576 =====
PART IV_MIMO-OFDM 통신 시스

[포

1E+000

1E-001

1E-002

1E-003

BER
BER

1E-004                                                                                                                                                     1E-004

AWGN

no coding

1E-005       —#— code rate 1/2
—— code rate 8/18
—8— code rate 8/20

1E-006        —S— code rate 8/22

—F— code rate 1/3

no coding
—}— code rate 8/9
—f- code rate 8/10
—6— code rate 8/11
—A— code rate 8/12
—F— code rate 8/14
—#— code rate 1/2                                                                                     — code rate 8/32
1E-007 011 ㅠ     |] 고 | 1 |              16009 ㄴㄴ | 1 | ㆍ      으르 그 a
0          2          4          6          8          10         12         14                   0          2          4          6          8          10         12         14
Eb/NO                                                                                             Eb/NO

1E-005

1€-006

(a) 부호율 8/9~1/2 ABA) BER           060) 부호율 1/2~8/33 적용시 BER
그림 16.8 AWGN 환경 하에서 부호율에 따른 Eureka—-1472| BER 성능

여기서 4 은 성상도의 수이며, 25740 는 심볼당 0 에너지 대 잡음 에너지 비를 나
타낸다. 그림 16.7은 이론적인 DQPSK 변조  ae     R 성능과 모의 실험 결과를 비교
하여 보여준다. OFDM 심볼에서 00       보호 비바 carrier)-& 고려하지 않고
모든 부반송파에 데이터를 채운 경우 AWGN 환경 하에서 BER 성능이 이론적인 값과 같
Al 나타남을 알 수 있다. 또한 Eureka—147 DAB 시스템은 부호율 89부터 8/32까지 24가
지 부호율을 지원하는데 그 중 일부의 성능을 보여준다.

(6) 동기화 기법

그림 16.9는 PRS] 주파수 영역과 시간 영역에서 자기상관 특성을 보여준다. 이 그림
에 나타난 바와 같이 008의 3 자기상관은 임펄스에 가까운 SAS 가지므로 이를 이용하여

동기화 과정이 이루어진다.

초기 동기화는 대략적인 프레임 동기, 미세 프레임 동기, 정수배 반송파 주파수 옵셋
(Integral Carrier Frequency Offset; ICFO) 추정, 소수배 반송파 주파수 옵셋(『180010181
Carrier Frequency Offset; FCFO) 추정으로 구성되며, 그림 16.10에 초기 동기화 과정의
예를 보여준다. 초기 동기화에서 대략적인 프레임 동기는 Null 심볼을 사용하여 이루어진
다. 대략적인 프레임 시작 위치가 ASEH PRSS 이용한 미세 프레임 동기와 두 단계로
iis 반송파 주파수 옵셋 추정 과정이 이어진다. 반송파 주파수 옵셋은 정수배 반송

주파수 옵셋과 소수배 반송파 주파수 옵셋으로 나눌 수 있으며 각각의 옵셋을 별도로
정한다.

+\

580


===== PAGE 577 =====
AMli6St_DMB/DVB 시스템

Characteristics of Phase Reference Symbol, Model     Characteristics of Phase Reference Symbol, Model
0.8F                                                                       7            0.8F
옥                                                  g
을 0.64                                                 1      S 0.6}                                                 4
S                                                  5
Rss}                                                  3
© 04+                                                   1 _ 혼0사                                                   1
8                                                  8
0.2F                                                                 1           0.2F                                                                 1
0                                                  0
-1000     -500       0       500      1000     -1000     -500       0       500      1000
Frequency Index                                                                 Time Index
(a) 주파수 영역                               (b) 시간 영역
그림 16.9 『5의 자기상관 특성
Coarse Frame Synchronization / Mode Detection
(Null Symbol Detection using Signal Power)
Integral Carrier Frequency Offset Estimation
(Algorithm Using the Intercarrier Differential Correlation)
Fine Frame Synchronization
(Algorithm Using the Channel Impulse Response)
Fractional Carrier Frequency Offset Estimation
(Algorithm Using the Guard Interval based Auto-correlation)
그림 16.10 초기 동기화|과정의 예
———— | Window 1     Window 2     ~
그림 16.11 에너지비를 이용한 대략적인 프레임 동기
Signal Power Ration, SNR 508
4.00
3.00

Magnitude
02
So
oO

S
S

0.00                                                                 -2048                       0            |          2048
Time Index

그림 16.12 Null 심볼과 PRS2| 에너지비 (SNR=5cB)

-6144                   -4096

581    |



===== PAGE 578 =====
PART IV_MIMO-OFDM 통신 시스템

대략적인 프레임 동기는 그림 16.11에 나타난 것처럼 Null 심볼과 PRS] 에너지비를
이용한다. 그림 16.12에 나타난 바와 같이 두 윈도우의 에너지비는 첫 번째 윈도우와 두
번째 윈도우의 경계가 Null 심볼의 시작 위치일 때 최소가 되며, 두 윈도우의 경계가 PRS
의 시작 위치일 때 최대가 된다. 대략적인 프레임 동기화는 다음 식으로 나타낼 수 있다.

w=0                                                    w=0

(ae  = argmax| + + [nt+wt+W]  al [n+wly wv]       (16.6)

여기서 5 는 PRSS| 대략적인 시작 위치를 나타내며, WL 에너지를 구하는 윈도우의
크기를 나타낸다.

표 16.4는 정수배 반송파 주파수 SA 추정에 사용될 수 있는 방식을 요약하여 보여준
다. 이 표에서 &와 는 각각 추정된 BEM 반송파 주파수 옵셋과 순환 이동(05011
shift) 값을 나타낸다. 또한 &414]=ㅅ[414'[+-11, 21641=714]1^[4-11 을 나타낸다. 수
신된 PRSG} 『05의 ARES 이용하는 방식(4085)은 간단한 계산으로 정수배 반송파 주파
수 GAS 추정할 수 있으나 심볼 타이밍 옵셋이 존재할 경우 추정이 불가능하다. 그러나,
채널 임펄스 SHS 이용하는 방식(4010:이나 인접 부반송파간 차등 상관을 이용하는 방
식(&100은 심볼 타이밍 옵셋이 존재하는 경우에도 정수배 eso
수 있다. 4018 방식에서 정수배 반송파 주파수 옵셋과 4같이 일
은 수신 ASS} 심볼 타이밍 옵셋에 해당하는 위치에서 채널 임펄스 Seto] 최대가 된다.
ACIR 방식은 심볼 타이밍 옵셋이 존재할 경우에도 정확한 정수배 반송파 주파수 옵셋을

으며, IFFTS] 출력을 이용하여 심볼 타이밍 옵셋까지 추정할 수 있는
있으나, 많은 연산량을 요구하는 단점이 있다. 한편, 심볼 타이밍 옵셋은 주파수 영역에서

형적인 위상 ABS 발생하므로 심볼 타이밍 옵셋으로 인한 인접 부반송파간의 위상 변

me    개

o 던
N
S|
×
fo
10
\
건

ca

c

다. 이러한 SIS 이용한 것이 AIDC 방식이다. AIDC 방식은 심볼 타이밍
옴셋의 영향을 받지 않으며, ACIR 방식보다 적은 계산량을 가지는 장점이 있다.

미세 프레임 동기는 표 16.4의 ACIR 방식에서 d of 추정된 정수배 반송파 주파수 옴셋
값(& )을 대입하여 의 최대 출력값의 HAS 구함으로써 추정할 수 있다. 이 경우에
정확한 미세 프레임 동기를 위해서는 정확한 정수배 반송파 주파수 옵셋 추정이 선행되어
야 한다. 마지막으로 소수배 반송파 주파수 옵셋은 5장에서 설명한 보호 구간을 이용하는
방식을 사용하여 추정할 수 있다. 지금까지 기술한 동기화 방식은 하나의 예시이고, 이와
는 다른 순서와 알고리즘을 사용하여 동기화할 수 있다.

_ 582



===== PAGE 579 =====
제16장_6048/ㅁ0\8 시스템

표 16.4 정수배 반송파 주파수 옵셋 추정 방식의 비교

아이 고 using Phase Reference Symbol)

Dependent            N?           Impossible

é, =argmax
d

SYERIX [kdl

ACIR

Algorithm using Channel Impulse Response)                       N
000              ie        ‘         Independent WN »( vy ee N       Possible

é =argmax | max IFFT {Y[k]X [k -d]y }|

AIDC

(Algorithm using Intercarrier Differential
Correlation)

Independent         N?+N2=N?          Impossible

 16.3 pve a8

6 ㅁ\2 시스템의 개요

ㅁ0\8-ㅠ와 DVB-H 시스템은 유럽 디지털 방송 표준화 기구에서 제안한 지상파 디지
털 TV 전송 방식으로 OFDM 방식을 사용한다. DVB-TE 이동 수신의 Boo] 성능은 우
수하지만 실제 휴대 단말에서는 배터리 수명 문제로 서비스 확산이 어렵다고 판단하여
DVB-H 개발이 시작되었다. DVB-H 28-7에 기반한 규격이며, DVB-T2} 호환성
을 유지한다. 또한 DVB-HE DVB-T] MPEG-2 다중화기와 공유가 가능하며, ㅁ 기
반 서비스이고, 이동 단말 수신에 종점을 두고 있다. DVB-H7} DVB-TS} 차이가 있는
기능으로는 전력 감소와 핸드 오버를 위한 시분할(11016 Slicing) 기술, 중/대형 SFNeAI
의 이동성을 위한 4 모드, 효율적인 시그널링을 위한 Extended TPS 비트 So] 있다. 또
한, 링크 계층에서는 열악한 수신 환경을 극복하기 위해 MPE-FEC(Multi—Protocol

Encapsulation—Forward Error Correction) 기술을 사용한다.

583 _



===== PAGE 580 =====
PART IV_MIMO-OFDM 통신 시스템

604 DVB 시스템의 전송 방식

그림 16.13은 DVB-T} DVB-H 시스템의 송신단 BEES 보여준다. 이 그림에 나
타난 바와 같이 각각의 서비스 ASL 개별적으로 소스 부호화기를 거친 후 에너지 확산
부를 거쳐 오류방지를 위하여 부호화된다. 이 ASE 맵핑된 후 OFDM ASE 변조되어
전송이 이루어진다. 여기서 부호화기는 RS 부호화기, 컨볼루셔널 부호화기, 2개의 인터리
버로 구성된다.

Transport

MPEG-2
source coding and multiplexing

To aerial A

TERRESTRIAL CHANNEL ADAPTER

그림 16.13 DVB-T2} DVB-H 시스템의 송신단 구조

AGRE DVB 전송 프레임 구조

그림 16.14에 나타난 바와 같이 DVB-T2} DVB-H 규격에서는 68개의 OFDM 심볼
이 1개의 프레임을 이루고, 다시 4개의 프레임이 1개의 슈퍼 프레임을 구성한다. 이 때
OFDMY| 모든 심볼은 데이터와 기준 정보를 포함한다. 기준 정보는 분산 TAA, 연속 파
aa, TPS 신호 등이 있다. Baae 프레임 동기, 반송파 주파수 동기, 심볼 타이밍 동기,
채널 등화, 데이터 전송 모드 및 보호구간 모드 판단 등에 사용된다. 표 16.5는 대역폭에
따른 OFDM 파라미터를 보여준다. DVB-TE 2K 모드와 8K 모드만 지원하지만,
DVB-H DVB-T°] 4K 모드가 #7} 지원된다. 따라서 2+8-의 전송 파라미터는 표
16.5에서 4K HES 제외하고는 DVB-H2] 전송 파라미터와 동일하다. 또한, 85411 대



===== PAGE 581 =====
제16장_0\46/ㅁ0\5 시스템

역폭 외에 5, 6, TMHz2} 대역폭이 있지만, 8541 대역폭의 파라미터를 비례적으로 조정
하면 되므로 설명은 생략한다.

superframe                                                                       —

그림 16.14 DVB-T2} DVB-H 시스템의 전송 프레임 구조

EE 16.5 DVB-T2} DVB-H 시스템의 전송 파라미터

Number of carriers K             6817      3409      1705
Value of carrier number ㅅ             0         0         0
Value of carrier number ㅅ            6816       3408       1704
Duration 7,,,                 896 ps     448 jus     224 us
Carrier spacing 1727,              1116 Hz    2282 Hz    4464 Hz
Spacing between carriers K,,, and ㅅ     7,61 MHz 7,61 MHz 7,61 MHz

= 16.6 DVB-T} DVB-H 시스템의 전송 모드에 따른 유효 심볼 길이와 보호 구간 길이

2048x Ts, 224 ws 10240xT7;, 1120 ps

z                8192 x Ts         1024x Ts, 112 ws 9216x7s, 1008 ps
8K mode

1/16           896 ps       512xT;, 56 ws  8704XT7;, 952 ps

1/32                      956x 75, 28 us 8448xT7s, 924 ps

1/4                         512x Ts, 56 us  2560XT;, 280 ps

1/8             2048 x Ts        956xXT;, 28 ps  2304xTs, 252 ps
2K mode

1/16           224 ps       128xTs,14 pws 2176xTs;, 238 ps

1/32                       64x Ts, 7 ps    2112x Ts, 231 ps

1/4                             1024xT;, 112 ps 51204, 560 ps

1/8               4096 x Ts          819 56 us 4008, 504 ps
4K mode

1/16             448 jus         256XTs, 28 ps  4852xT;, 476 ys

1/32                             128xTs, 14 ps  4224xT7;, 462 ps

585


===== PAGE 582 =====
PART IV_MIMO-OFDM 통신 시스템

한 OFDM 심볼의 길이는 유효 심볼 구간과 보호 구간   질이의 합으로 FelzjEql, 의
때 보호 구간의 길이는 표 16.6에 주어진 바와 같이 유효 심볼 구간의 114, 1/8, 1/16, 1/32
인 4가지 경우가 존재한다. 표 16.6에서 7,는 샘플 주기로서 0.109375/68로 주어진다.

16.3.4 ㅁㅁ 물리계층 규격

(1) 채널 부호화와 변조

MPEG-2 transport multiplex 패킷은 길이가 188 바이트이고 1개의 sync—wordS 포
함하고 있다. 패킷의 데이터가 충분한 이진 천이(61087 transitions)S 갖기 위하여 스크랩
블러가 사용되며, 생성 다항식은 2(4) =1+ㅅ' +" 을 사용한다. 그림 16.13에 나타난
바와 같이 에너지 확산된 신호는 0466 부호화기에 …  outer 부호화기는 591006060
RS(204, 188, [= 8) 부호화기를 사용한다. 데이터의 전송에 앞서 51 바이트의 OS RS
(255, 239, [= 8) 부호화기에 입력하고 부호화를 수행한 후, 출력된 결과 중 null 바이트를
제거함으로써 길이가 204 바이트인 shortened FOS 얻을 수 있다. Outer 인터리버는
depth /=12 인(12개의 branch) 컨볼루셔널 바이트 단위의 인터리버가 사용된다. 각
branch /는 depth jx M 셀을 갖는 FIFO 쉬프트 레지스터이다. FIFO] 각 WS 1 바이트
를 포함한다. 동기를 Het sync—byte= 항상 branch 0과 연결된다.

Inner 부호화기로는 2740004600 컨볼루셔널 부호가 사용된다. 모부호(070016ㅠ 0000)는 부호
율 1/2이고, 64 개의 state 갖는다. Inner 부호화를 통해 비계층적/계층적(000ㅁ-11608011081/
hirerachical) 전송에서 원하는 서비스 혹은 전송율에 따라 에러 정정 레벨을 달리할 수 있
다. S, puncturing 통하여 1/2, 2/3, 3/4, 5/6, 7/8의 FESS 얻을 수 있다.

앞서 기술한 ASA 전송이란 하나의 텔레비전 주파수 채널을 통해 2개의 독립적인
DVB 스트림을 전송하는 기술을   을 말하며, 입력을 HP(High—Priority)2} LP(Low-Priority)
로 구분하여 처리한다. 특히, HPE 휴대 및 이동 VANS 위해서 사용된다. 100@ 인터리버
는 vise Je debs Pade 비드 Vedas 임력으로 최대 279 비드 스드림
을 가질 수 있다. 입력되는 비트 스트림은 "개의 서브스트림으로 디멀티플렉싱 된다. 여
기서, VE 변조 Blo] 따라 다른 WS 갖는다. 009&의 경우 v=2, 16QAMY] 경우
v=4, 64QAM2] 경우 1=6이다. B]A]sA\(Non-hierarchical) 전송에서는 하나의 입력
비트 스트림만이 존재하며, "개의 서브스트림으로 디멀티플렉싱 된 후 각 서브스트림에
대해 인터리빙을 수행한다. 계층적(846007001081) 전송의 경우 HP 스트림은 2개의 ABA

586



===== PAGE 583 =====
터리버를 사용할

ze ‘tet 그리고
비트의 심

변조

uniform) 변조(16044, 64QAM)7} 있다. 변조

트림으로, LP 스트림은 2) 개의 서브스트
해 인터리빙을 수행한다. 비트 인터리빙
리버의 SAS 하나의 데이터 심볼을 %

그림 16.15에 나타난 바와 같이 심볼 인터리버는 세 가지 모드에 따라 다양한 심볼 인
터리빙 방식을 사용한다. 단말기는 전송하는 모드에 따라 기본적으로 제공되는 2806 인
수 있다. 그러나 2&와 4K 모드의 경
모리를 사용하여 인터리빙 depthS
In—depth 인터리빙을 위해 4K 모드
, 8K 모드에서는 6,048 비

을 위한

증가시키는

제16장_046/ㅁ'\8 시스템

o=1,2,4) 에 따라 달라지며 값이 2 이상이면 비균일 변조가 된다.

Native 8K
inner interleaver

One OFDM symbol

Native 4K
inner interleaver

One OFDM symbol

In-depth 4K
inner interleaver

Two OFDM symbols

Native 2K
inner interleaver

$ [12 x 126 66 ㅣ

One OFOM symbol

In-depth 2K
inner interleaver

Four OFDM symbols

그림 16.15 DVB-T} DVB-H 시스템의 다양한 심볼

x(f)=Re    img

여기서

m=0 7=0 =

인터리버

Xn lk] X Wack 이

림으로 디멀티플렉싱 된다. 이후 각각에 대
블록 길이는 126 비트이다. 각 비트
형성하기 위해 그룹화 된다.

인터

경우에는 이와는 별도로 8K 모드의 메
in-depth 인터리버를 사용할 수도 있다.
는 2개의 OFDM 심볼을, 2K 모드는 4개의 OFDM 심
트의 심볼 단위로, 4K 모드에서는 3,024

볼 단위로, 2K 모드에서는 1,512 비트의 심볼 단위로 동작한다.
방식으로는 균일(404000) 변조(209, 16QAM, 64QAM)3} 비균일(000-
에 사용되는 성좌점의 위치는 파라미터

(16.7)

587


===== PAGE 584 =====
A Ell
|

PART IV_MIMO-OFDM 통신 시

J 2m FE (1-Teg—1 Toy ~68 Typ)

fan)

Wik (t ) =
0                                       else

|

여기서, 는 부반송파 인덱스,
반송파 전체 수, Tom 는 전체 심볼 구간, 7, 는 부반송
길이, /, 는 RF AS) 반송파 주파수, 은 반송파 주파수와 관련된 부반송파 인덱스
시 =4-(&,, - )/2를 나타낸다. 또한, X,, 1K] 은 m 번째 프레임의 / 번째 OFDM
심볼에서 ka 부반송파의 복소 신호를 나타낸다. 전체 심볼 구간 7. 는 유효 심볼 구
Zt Typ 2 보호 구간 길이 의 합으로 구성된다
(3) 기준 4lS (Reference Signal)
OFDM 신호는 일정한 크기를 가지는 HU 정보를 일정한 위치에 삽입하여 전송한다.
as) 신호에는 분산 ahaa, 연속 a}elel, TPS(Transmission Parameter Signaling) 신호
가 있다. 연속 WYO. 모든 심볼에 대해 같은 위치에 삽입되며, 분산 abelale 4가지 시
작모드를 가지고 12개의 부반송파마다 삽임된다.
연속 ae)ala} 분산 wpe #(%)=ㅅ!'+ㅅ"+1의 생성 다항식을 갖는 2088에 따
있다

라 생성된다. 분산 Bala] 크기와 위치는 Al (16.9)에 주어져
14=ㅅ+3×%(0 mod 4)+12p | p integer, p>0,k €[K yin? Kinax J}
.                       (16.9)

Re{X,, [k]} =4/3x2(1/2-w,)

Im{X,, [A] } = 0
= 1704 if 2K
Kor = 6816 F 8K

TPS pilots and continual pilots between Kmin aNd Kmax are not indicated

심볼 구조

@ boosted pilot
O data
그림 16.16 DVB-T2} DVB-H 시스템의 OFDM

588



===== PAGE 585 =====
A642! DMB/DVB 시스템

그림 16.162 2K PES} 8K 모드에서 OFDM 심볼 구조를 보여준다. 이 그림에서 A
은색으로 표시된 부분이 분산 upelal 또는 연속 wolae 나타내고, 흰색으로 표시된 부
분이 데이터를 나타낸다. 가로축은 주파수 영역의 부반송파를 나타내고, 세로축은 심볼을
나타낸다. 연속 wp]eLS 표 16.7에 나타난 바와 같이 BK 모드일 때는 총 177개, 4 모드
일 때는 총 89개, 2K WES 때는 총 45개의 vpoleto] 매 심볼 마다 일정한 부반송파 번
호에 위치한다. 연속 파일렀의 크기는 분산 파일렀의 크기와 동일하다.

778는 표 16.8에 나타낸 바와 같이 DVB 신호 전송에 관계된 파라미터의 정보를 수신
기에 전달하는 Tele 신호로서 한 개의 OFDM 심볼에 1비트가 할당된다. 따라서 & 모
드의 경우 68개의 THI}, 4K BES} 경우 34개의 upeletoy, 2 모드의 경우 17개의
HQ] Bo] 분산되어 전송되며, 한 개의 프레임, 즉 68개의 OFDM 심볼에 포함된 68비트가
모여야 전체 TPSS 구성하게 된다. 108는 정상 신호 레벨로 0808 변조되며, 각 비트
에 실리는 정보는 표 16.8에 주어져 있다.

779는 (67,53.7"=2) BCH 단축 부호로 부호화되어 53개의 정보 비트와 14개의 패리티
비트를 구성되며 생성 다항식은 다음과 같다.

eX 14 24°48 + 고" 주조 4? 4        (16.10)

TPS 추출기에서 출력되는 YESS (67,53,-2) BCH 단축 부       로서 (127,113.==2)
BCH 일반 복호기로 복호하기 위해서는 먼저 60비트의 0을 앞 1  임해야 한다. 패리티
검사 결과 오류가 모두 정정되었을 경우에만 TPS 정보를 버퍼에 저장하고 FECA) 최종적

표 167 연속 moeto] 위치
Continual pilot carrier position (index number k)

8K mode        0 48 54 87 141 156 192 201 255 279 282 333 432 450 483 525 531 618 636 714 759 765 780 804 873 888 918

939 942 969 984 1050 1101 1107 1110 1137 1140 1146 1206 1269 1323 1377 1491 1683 1704 1752 1758 1791
1845 1860 1896 1905 1959 1983 1986 2037 2136 2154 2187 2229 2235 2322 2340 2418 2463 2469 2484 2508
2577 2592 2622 2643 2646 2673 2688 2754 2805 2811 2814 2841 2844 2850 2910 2973 3027 3081 3195 3387
3408 3456 3462 3495 3549 3564 3600 3609 3663 3687 3690 3741 3840 3858 3891 3933 3939 4026 4044 4122
4167 4173 4188 4212 4281 4296 4326 4347 4350 4377 4392 4458 4509 4515 4518 4545 4548 4554 4614 4677
4731 4785 4899 5091 5112 5160 5166 5199 5253 5268 5304 5313 5367 5391 5394 5445 5544 5562 5595 5637
5643 5730 5748 5826 5871 5877 5892 5916 5985 6000 6030 6051 6054 6081 6096 6162 6213 6219 6222 6249
6252 6258 6318 6381 6435 6489 6603 6795 6816

4K mode        0 48 54 87 141 156 192 201 255 279 282 333 432 450 483 525 531 618 636 714 759 765 780 804 873 888 918
939 942 969 984 1050 1101 1107 1110 1137 1140 1146 1206 1269 1323 1377 1491 1683 1704 1752 1758 1791
1845 1860 1896 1905 1959 1983 1986 2037 2136 2154 2187 2229 2235 2322 2340 2418 2463 2469 2484 2508
2577 2592 2622 2643 2646 2673 2688 2754 2805 2811 2814 2841 2844 2850 2910 2973 3027 3081 3195 3387
3408

2K mode        0 48 54 87 141 156 192 201 255 279 282 333 432 450 483 525 531 618 636 714 759 765 780 804 873 888 918
939 942 969 984 1050 1101 1107 1110 1137 1140 1146 1206 1269 1323 1377 1491 1683 1704

5689



===== PAGE 586 =====
PART IV_MIMO-OFDM 통신 시스템

표 16.8 TPS 전송 정보와 형태

21/2
An initialization bit for                  은 ry         0 ; 며             0006 1816
80      the differential 2-PSK    Initialization        pacar              :                (HP stream,
modulation                   a, sat, 000        04: 5/6          LP stream)
(LP stream)         100 : 7/8
101~111 : reserved
0011010111101110                                    00 : 1/32
(Frame number 1 or 3) Synchronization                      01 : 1/16                :
sl- 816     1100101000010001        ate        s36, s37          10 : 1/8         Guard interval
(Frame number 2 or 4)                                       1/4
00 : 2K mode
—                     01 : 8K mode        Transmission
817 ~ 822         100001         Length indicator    838, s39         10 2 4K mode            ae
11 : reserved
00 : Frame number 1                              b8~b15 : Frame number 1
01 : Frame number 2                                         or 3                 H    _
828, 824    0 8 namber 3    Frame number    s40 - s47   BOT “Frame: Auber   Cell identifier
11 : Frame number 4                                          or 4
Ox : Time slicing is not
used
lx : At least one
os See                                  PE cena ts slicing
: 16-                                                                DVB-
825, 826       Of lie ores       Constellation    848 - 849    x0 : MPE-FEC not used      s    is
10 : 64-QAM                                       :                  signalling
X1 ‘At least one
11 : reserved
elementary
stream uses MPE-FEC
Note : “x”means whatever
리                      bit state
0 : native interleaver    alesis:
827      a        ‘             Interleaver      850 - s53        All set to “0”
1 : in-depth interleaver          ,
Information
00 : Non hierarchical
828, 829        바그          비0006007      854 - 867     BCH code (parity bits)    Error protection
Zs           1:a=2         information                         배~             i
ll:a=4

으로 전달하게 된다. 만일 패리티 검사에서 실패할 경우 버퍼는 이전의 TPS 정보를 유지
하고 현재 복호된 TPS 정보는 폐기하게 된다. BCH 복호된 신호의 sl~sl6 비트를 이용
하여 프레임 동기가 수행되는데, 복호된 비트 51 ~816까지의 비트 정보와 표 16.8에 주어
진 synchronization word7} 일치하면 프레임 동기가 이루어진다.

(4) 시분할(1106 Slicing) 기술

DVB-H 휴대 단말기를 위한 규격으로 제한된 배터리 HBS 갖는다는 제약 조건이
있다. 278-브가 DVB-T} 호환되게 만들어졌다는 것 자체가 DVB-H 단말기에는 부담
으로 작용한다. DVB-T 스트림과 같은 광대역 고속 스트림을 복조 및 복호화 하는 과정
에서 튜너와 복조기에서 전력 손실이 발생하기 때문이다. DVB-H 개발 초기에 DVB-T
front end 단은 1\ 이상의 AAS 소비하는 것으로 나타났고, 2006년까지도 600mW 이

590



===== PAGE 587 =====
제16장_미7686/ㅁ0'\8 시스템

하로 떨어지지 않을 것으로 조사되었다. 왜냐 하면, 멀티플렉싱 된 특정 서비스를 보기 위
해서 278-1는 전체 데이터 스트림을 복호해야 하기 때문이다.
DVB-H: 원하는 서비스 데이터를 가진 스트림의 특정 부
절전 기능이 사용된다. 2\8-꼬에서 여러 서비스는 TDM(Time Division Multiplexing)
방식으로 멀티플렉싱 된다. 특정 서비스의 데이터를 연속적으로 보내지 않고, 사이에 공백
이 있는 조밀하고 주기적인 버스트 형태로 전송한다. 서로 다른 다수의 서비스를 멀티플
렉싱해서 보내게 되면 스트림은 일정한 전송률을 가진 연속적이고 공백이 없는 형태가 된
다. 이러한 전송 방법을 통해 원하는 시간대에 서비스를 선택적으로 수신할 수 있다. 단말
기는 원하는 서비스의 버스트에 대해서 동기를 맞추고 다른 서비스들이 ASS 때는 절전

모드에 들어가면 된다. 이러한 비르 시분할(0106 slicing) 기술이라고 한다. 수신기는

력된 버스트 들을 버퍼링한 후 전송률에 따라 특정 서비스를 읽어낸다. 일반적으로 한 버
스트의 길이는 수백 밀리초에 달ㅎ ne 절전 시간은 수초에 달한다. 이를 위해 front end 단
에 전원을 켜고 동기를 다시 맞추는 데 걸리는 시간은 25008 미만이 되어야 한다. 시분할
기술을 사용할 경우에 0ㅁ-04006과 절전 시간 비율에 따라 최대 90%까지 절전효과를 볼
수 기 기마 그림 16.172 시분할 서비스를 포함한 데이터 스트림을 보여준다. 이와 같이 긴
절전 시간을 이용하여 인접 셀에서 현재의 서비스를 제공하는 채널을 찾을 수 있으며, 이
통해 두 셀간의 AAA 채널 핸드오버를 수행할 수 있다. 즉, 하나의 60041 600를 A+
하여 인접한 셀에서 제공되는 서비스에 대한 모니터링과 선택된 서비스 데이터의 수신

모두 할 수 있다.

만을 처리할 수 있는

주

띠ㅇ   때

service 8                 Burst size
|                    2Mbits

+
3.2 Mbit/s

TV Program 3
TV Program 2                  | Mbit/s
Data rate in
the DVB-H
channel               TV Program 1
time
|     |     |     100:     |     |     |     ㅣ      ~ ^

1660

그림 16.17 DVB-H 서비스를 위한 시분할(1016 slicing) 기술

591



===== PAGE 588 =====
PART IV_MIMO-OFDM 통신 시스템

(5) MPE-FEC

MPEC—2 표준에서 파생된 DVB transport AB YS 사용하는 DVB 시스템과는 달리
DVB-H 시스템은 1Po} 그 기반을 두고 있다. 따라서, DVB-H 시스템은 IP 인터페이스를
통해 이종의 네트워크와 ASS 수 있다. 데이터는 MPE(Multi—Protocol Encapsulation)
라는 DVB 데이터 방송 표준에 B}S adaptation =2ESS Fa transport AE Wo] 포
함된다. MPE 레벨에서 FEC7} 추가된 것이 MPE-FEC 기술이며 물리계층의 FECS 2
완하는 역할을 한다. \008-180는 그림 16.18에 나타난 바와 같이 RS 부호와 가상 블록
인터리버로 구성되며, 이 기술을 사용할 경우 278-1보다 oF 708 BES] SNR 이득이

발생한다.
Application Data Table               RS Data Table
RS Encoding                               Frame Cell
8
드
                                                                                   2
write                                                                                른
/1680                                                                               =
zs
N
을
|
191 columns                     64 columns: |
1P Sections                     FEC Sections

그림 16.18 DVB-H 서비스를 위한 MPE-FEC 기술

592



===== PAGE 589 =====
GA wessasey

UWB(Ultra—WideBand) 무선 전송 방식은 무선랜 등의 기존 무선 전송 방식의 전력에
비해 적은 전력으로 100\4608에서 10508까지의 전송 SES 제공할 수 있는 무선 전송

방식이다. UWBE 주로 군용 통신 및 레이더 기술로 개발되었으나, 2002년 FCC(Federal
Communications (2004001561020)에서 UWB2] 상용화를 허용한 이후 전자기기 간의 ASS
위한 근거리 무선 전송 방식으로 활발히 개발되고 있다. 표 17.1은 UWB 시스템과 타 통
Al 시스템의 특성을 비교하여 보여준다.

표 17.1 UWB 시스템과 EF 통신 시스템의 비교

2,4GHz       5oGHz         2.4GHz     868/915M/2.4G  3,1~10,6GHz

54Mbps         500Mbps             1Mbps_        20/40/250Kbps         500Mbps
1Km                        1Km                             10m                               30m                             2100
|                                       MB OFDM

그  OFDM/DSSS MIMO-OFDM Freq, Hoppi   CSMA-CA
-   /        req. Hopping       Ae OA

|
다양한 동신지원 -고수명, 저전력 -고속 데이터 전송
(음성, 팩스, |AV) -전송 안정성 = -간섭에 강함

근거리 유선 저전력, 저가의 근거리 고속
대체 기기 제어     통신

FCC UWB YAS 중심 주파수의 20% 이상의 점유 대역폭을 가지거나
500MHz 이상의 YASS 차지하는 무선 전송 기술로 정의하였다. 일반적으로 3.1GHz~
10.6GHz 대역에서 FCC7} 정의한 EIRP(Effective Isotropically Radiated Power)°] 제한

593


===== PAGE 590 =====
PART IV_MIMO-OFDM 통신 시스템

42                                    ia
AGS 다른 무선 전송 ALAMO] 사용하는 대역과 겹치기 때문에 주파수 2m
시스템에 간섭을 미치지 않도록 -41.3080 이하의 작은 전송 전력으로 넓은 대역에 걸쳐
분포한다. 그림 17.1은 UWB 스펙트럼과 타 통신의 스펙트럼을 비교하여 보여준다.
UWB} 저속 UWB 표준화가 시작되었다. IEEE 802.15.38에서 표준화를 진행하였던 고
속 UWB 전송 방식은 88 802.15.3의 고속 WPAN(Wireless Personal Area Network)°]
서 제공하는 전송속도(11~551\40679)를 향상시키기 위한 것이었다. 하지만 TEEE8O2.15.3a
의 물리계층 표준화에 있어서 DS-CDMA(Direct Sequence Code Division Multiple
Access) 방식과 MB-—OFDM(Multiband Orthogonal Frequency Division Multiplexing)
방식이 서로 대립하여 단일 표준 채택이 실패함에 따라 2006년 1월 IEEE 802.15.3ac 활
동을 중단하였다. IEEE 802.15.38의 표준화 중단 이후 MB-OFDM 방식과 DS-CDMA
방식의 표준 활동은 각각 WiMedia(Wireless Multimedia) Alliance2} UWB Forum®]A|
개별적으로 진행되면서 시장점유에 의한 실질적 표준으로 자리를 굳히기 위한 경쟁 체제
로 전환되었다. 2002년 PANA 장치간 무선 멀티미디어 연결과 상호 운용성을 장려하
기 위해 구성된 WiMedia Alliance} 2005년 MBOA(MB-OFDM Alliance)2} 합병하여
MBOA 기반의 물리계층과 MAC 계층 기능뿐만 아니라 상호 운용성 및 기타 응용에 필
요한 FAS 개선 또는 제정하고 있다. WiMedia Alliance} 2005년 ECMA International
등의
표준 채택, WiMedia 표준 규격 제정, 상호 운용성 시험 지원, 그리고 USB Forum, 무선
1394 등의 응용 분야 개발에 활발한 활동을 하고 있다.

(European association for standardizing information and communication systems)

Emitted
Signal 수
Power
802.1 1a WLAN
[| Cordless Phone
Bluetooth
802.1 1g WLAN
Cordless Phone
____— Micro Ovens

Sod

pueg 140

98059
pueg WS!

FCC Part15 Limit

-41.3
dBm/MHz

16     1.9    24     3.

그림 17.1 UWB 전력과 주파수 대역

594



===== PAGE 591 =====
제17장_\18-야0 시스템

(O27 40088 148-0『ㅁ14 전송 방식의 물리계층 규격

UWB 시스템을 위한 MB-OFDM 규격은 ECMA International®} 80144-368에 주어
져 있다[312]. MB-OFDM&. 기본적으로 OFDM 기반 전송 방식이기 때문에 다중 경로
지연에 의한 ISI(Inter—Symbol Interference)o] 강건한 방식이다. 그림 17.2에 나타난 바
와 같이 ECMA-368 규격에서는 700에서 정의한 3.10112에서 10.6GHz7}2] 2] 7.5GHz
의 대역을 14개의 대역으로 나누고, 인접한 대역들을 묶어 총 6개의 대역 그룹을 구성한
다. 대역 그룹 중 그룹 1은 기본적으로 사용되며, 그룹 2~6은 선택적으로 사용된다. 그룹
6은 각 국가의 주파수 사용 상황을 고려하여 추가되었다. 이 중 SGHz 비면허 대역을 포
함하는 그룹 2는 WLAN] 간섭 문제 때문에 사용하지 않을 수도 있다.

그림 17.2 ECMA-368 규격의 주파수 대역

ECMA~—368 규격에서는 OFDM 심볼 전송 시 TFC(Time Frequency Code)= 이용해
하나의 밴드 그룹 내에서 대역 간의 주파수 호핑을 수행하여 주파수영역에서의 다이버시
티 효과를 얻고 SOP(Simultaneously Operating Piconet) 간의 간섭을 최소화한다. 표
17.2는 MB-OFDM2] 그룹 1에 대하여 규격에서 정의된 기준 ASA AlAA(base
time domain sequence; preamble)2} TFC2] 관계, 그리고 TFCo] 따른 사용 대역을 보여
준다. 그림 17.3은 TFC7} 1인 경우 밴드 그룹 1 내에서 주파수 도약에 따른 OFDM 심
볼 전송 예를 보여준다. 표 17.2에서 TEC 5~7의 경우는 주파수 SYS 사용하지 않는
경우이다.

그림 17.3에서 각 ASS 128 샘플의 유효 심볼과 37 샘플의 2000-2080060 suffix= 구
성된다. 4.2.2절에서 설명한 바와 Zo] zero—padded suffixS 이용한 OFDM 심볼의 경우
CPS 이용한 경우에 비해 전력 스펙트럼의 리플이 감소해 FCCS] 전력 제한 기준 하에서
CPE 이용한 경우에 비해 높은 전송 전력을 달성할 수 있다. 표 17.3과 그림 17.4는 각각
물리계층 파라미터와 주파수영역에서 Fo] E|/2 S(guard)/Tpa a] 부반송파의 논리적 할당
을 보여준다. 보호 부반송파는 CE(Channel Estimation) 시퀸스부터 적용되며, 보호 부반
송파와 데이터 부반송파와의 전력 관계는 구현상의 이슈로 되어있다.

595



===== PAGE 592 =====
PART IV_MIMO-—OFDM 통신 시스템

596

표 17.2 밴드 그룹 1에서 에 따른 사용 대역

ik                 1           1     2     이     1     2     3
2                 2           1     3     2     1     S|     2
3                 3           i     1     2     2     3     3
4                 4           i     it     3     3     2     2
5                 5           1     1     1     il     1     1
6                 6           2     2     2     2     리     2
ii                 7           이     3     3     3     3     3
8                 8           1     2     1     2     1     2
9                 9           1     3     1     3     1     83
10                10           2     3     2     3     2     3
Symbol
3168 ㅜㅜ
4752                                    -                                 —         1» f
OFDM Symbol                        Zero-padded suffi
ous              (IFFT output)                 a

그림 17.3 밴드 그룹 1에서 TFC7} 1인 경우의 심볼 전송 예

= 17.3 MB-OFDM 물리계층 파라미터

Pee ee ee 이
.            Sampling frequency                    528MHz
Neer  Total number of subcarriers (FFT size)           128
es       Number of data subcarriers                100
Cee       Number of pilot subcarriers               12
ae       Number of guard subcarriers                10
ee     Total number of subcarriers used      122 (=Np + Np + Ne)
a       Sucarrier frequency spacing        4,125MHz (=f, /Nerrr)
aa          IFFT and FFT period                 242, 42ns
Naps Number of samples in zero—padded suffix          3

.   Zero—padded suffix duration in time     70,08ns (=Nzps / fs)
_-             Symbol interval              312.5ns (=Trrr + Tzps)
.             Symbol rate                3, 2MHz (=1/Tsym)
“he   Total number of samples per symbol     165 (=Nerr + Nzps)


===== PAGE 593 =====
제17장_ MB-OFDM 시스템

--- Data subcarrier ---- Pilot

Frequency domain ou

Time domain outputs

그림 17.4 GO|E/TUA/Hs 부반송파의 논리적 할당

그림 17.5에 나타난 바와 같이 ECMA-368 규격의 PHY 프레임 구조는 프리앰블,
PLCP 헤더, 프레임 payload, FCS(Frame Check Sequence), tail 비트, pad 비트로 구성된
다. 프리앰블은 표준(6800810)과 버스트(6079!) 두 개의 모드로 구분되고, PLcP age
payloadS 수신하는 데 필요한 정보를 포함한 물리계층 헤더와 MAC 헤더를 포함하고 있
다. PCLP 헤더 부분의 데이터 AS SEE 39.454608이며, 물리계층 헤더와 MAC 헤더
의 외부 부호기(0466 coder)= shortened Reed-Solomon (23,17) 부호화기를 사용하고,
주파수영역 확산(6604600/ domain spreading; 『129)과 시간영역 확산 (time domain
spreading; TDS)S 통해 주파수 다이버시티 OSS AES 데이터 ASS 부반송파에 할
당한다. PHY 프레임 구조를 구성하는 모든 OFDM ASS SOP 간의 간섭을 줄이고, 주
파수 다이버시티 효과를 얻을 수 있도록 각 피코넷(0100060에 할당된 TFC] 의해 주파수
도약되어 전송된다. 표 17.4는 ECMA-368 규격의 PHY 프레임 관련 파라미터를 보여준
다. 이 표에서 LENGTH= 프레임 2851080에 포함된 비트 수를 006 (8 비트) 단위로 나
타낸 것이고, ^,86 는 6 심볼 당 정보 HES 수를 나타내며, ^, 계산 식에 주어진 38
은 FCS t tail 비트의 길이를 나타낸다.

PSDU
(53.3, 80, 106.7, 200, 320, 400, 480[Mbps])

39.3 Mbps

그림 17.5 ECMA-368 7242] PHY 프레임 구조



===== PAGE 594 =====
PART IV_MIMO-OFDM 통신

표 17.4 ECMA-368 규격의 프레임 관련 파라미터

Number of Symbols in the           Standard Preamble: 24
packet/frame synchronization sequence       Burst Preamble: 12
Duration of the packet/frame         Standard Preamble: 7.5us
synchronization sequence            Bust Preamble: 3.75us
Number of symbols in the channel                 6
estimation sequence
Duration of symbols in the PLCP                1.875us
preamble
Number of symbols in the PLCP         Standard Preamble: 30
preamble                  Burst preamble: 18

Standard Preamble: 9.375us

Duration of the PLCP preamble        use Breeneie eeions

Number of symbols in the PLCP header               12
Duration of the PLCP header                  3.75us
Number of symbols in the PSDU      6xceil{(8x LENGTH +38)/N igr6s}
Duration for the PSDU         6xceil{(8x LENGTH + 38)/ Nipr6s}*Tsyu
Total number of symbols in the packet         ON ne TN ae TN jee)
Duration of the packet              None +N pce +N frame) * Tsyn4

ECMA-368 규격에서 정의된 표준 프리앰블은 PHY 프레임 시작 부분에 전송되며, 시
간과 주파수 동기를 위하여 24 심볼로 구성된 PFS(Packet/Frame Synchronization) 시퀸
스와 각 주파수 대역의 채널 추정을 위하여 6 심볼의 CE(Channel Estimation) 시퀸스로
구성된다. 반면에 스트림 패킷을 전송하는 스트림 모드 중에는 12 심볼의 PFS 시퀸스와
6 심볼의 CE WAS 구성된 버스트 프리앰블을 전송한다.

표준 프리앰블의 089는 하나의 OFDM 심볼에 해당하는 기준 시간영역 시퀸스와 심볼
단위 확산을 위해 정의된 표준 프리앰블을 위한 cover 시퀸스를 이용해 생성한다. 다음 수
식은 PFS9] 7번째 심볼의 / 번째 샘플 신호 FAS 나타낸다.

a

n| = ScoverL!]X Sex: [1], ne (0, Noy all and ke (0, N one=1]               (17.1)

‘one,

598



===== PAGE 595 =====
제17장_ MB-OFDM 시스템

앞의 식에서 Somes Scorer 은 각각 PFS 시퀸스, cover 시퀸스를 의미하고, Sexe 기준 시
Zt 영역 AMA Noes 만큼의 OS 추가해 얻     al  Ny 는 PFS AAA 내의 심
볼 수를 의미한다. 따라서 표준 프리앰블의 Prsg} 경        번 반복되는 기준 시간영역 시

퀸스에 대해 0016 시퀸스에 따라 심볼 단위로 1 또는 00 곱한 후 TFC] 따라 주파수
호핑하여 전송한다. CEA BAT 기준 주파수영역 채널 추정 AAAI IFFT 결과를 6 번
반복시켜 생성하여, TFC] 따라 주파수 호핑하여 전송한다. 그림 17.6은 표준 프리앰블
생성 방법과 프리앰블 전송 예(1『(:=1)를 보여준다.

2610-08060 base time           fn  Zero-paded base
equency domain channel
domain sequence                     estimation sequence

hy     sagen       비                           1

Cover sequence   fell           Spreader          |                   oo Se                  1
Lh ey       WE ete

Lth symbol of PES               Lth symbol of CE
sequence (/=[0, 23])          lsequence 1=[24, 29])

|

PFS sequence

f (MHz)
CE sequence          | |  PLCP header

[4 PFS sequence

4752
4224
3696
3168

그림 17.6 표준 프리앰블 생성 방법과 프리

ECMA-368 규격에서 지원하는 데이터 전송 속도는 PLCP 헤더의 경우에는 39.4
4628로 고정되어 있지만 29100 부분의 경우에는 53.3Mbps ~ 480Mbps= 가변적이다.
PSDUY] 데이터 AS SEE 변조 방식, 부호율, 주파수영역 확산(07604600% Domain
Spreading: 『129)과 시간영역 확산 (Time Domain Spreading: TDS) 여부에 따라 결정된
다. 부호화의 경우 1/32] 기본 부후  —   갖는 컨볼루셔널 부호화기에 가변적인 puncturing
을 적용해 수행하며, 변조 방식의 경        PSKS 기본적으로 사용한다. 또한 162444과
같은 성상도를 갖는 DCM(Dual Carrier 개가 러   지원한다. DCMS 구현 시 2개의
QPSKS 사용하여 생성될 수 있다. DCMS 4개의 입력 비트를 2개의 서로 다른 형태의
16QAM2.= 변조한 뒤 각각의 16QAM 심볼에 대해 다이버시티 이득을 AES 부반송파



===== PAGE 596 =====
PART IV_MIMO-OFDM 통신 시스템

를       방식으로 320Mbps 이상의 데이터 전송 속도에서 사용된다. 주파수영역 확산
과 시간영역 BLS. 주파수 다이버시티 이득을 AES ASS 반복시켜 전송하는 방식ㅇ
다. 주파수영역 확산 방식은 한 OFDM 심볼 내에서 데이터를 주파수영역에서 반복하여
전송하고, 시간영역 확산 방식에서는 동일한 데이터를 두 OFDM 심볼에 반복하여 ASE
다
파

—

. 표 17.5는 ?500에서 지원하는 데이터 AS 속도와 그에 따른 부호을, 변조 방식, 주

+
of
412,
St
ac
Se

확산과 시간영역 확산 여부를 보여준다. 그림 17.72 각 전송 속도에 따라 입력
비트 맵핑 방법, 변조된 심볼의 OFDM 심볼 내 부반송파 할당 방법, DCM 변조를 위한
핑 방법을 보여준다. 그림 17.7(a) TDS} FDS7} 모두 적용된 경우로서,
『05에서는 FY 복소수로 주파수 영역에서 확산하여 시간영역에서 실수 신호가 생성된
다. 그림 17.70)는 70만 적용된 경우로서, APRS} 허수부를 교환하여 확산한다. 그림
ITAA b, ARES 각각 입력 비트, 《번째 데이터 AWS 나타내고, 84 )는 DCM 적
용 시 입력 VES 《번째 데이터 심볼에 할당하기 위해 정의된 함수로 다음과 같다.

2k,      ke [0,24
=|           =e

17.2
2k+50, ke[25,49]              (17.2)

표 17.5 ECMA-368 규격의 데이터 전송 속도

586 3               QPSK               1/3            Yes Yes                    300                               100
80       QPSK      1/2     Yes Yes        300             150
106.7                QPSK                 1/3              No         Yes                      600                                  200
160                  QPSK                 1/2              No         Yes                      600                                  300
200        QPSK        5/8       No    Yes           600                 315
320         DCM        1/2      No     No          1200               600
400                   DCM                  5/8              No          No                      1200                                 750
480       DCM       3/4     No    No        1200             900
전술한 부분 이외에 타 시스템에 미치는 간섭을 줄이기 위해 = nullingS 통한 DAA

meet And Avoid) 선택적으로 적용할 수 있다.

_ 600



===== PAGE 597 =====
Al172_ MB-OFDM 시스템

aR END
ie

FEI conivoating and soreading

Subcarrier Mat

ㆍ | 47 | 48 | 49 Ries
symbol

ols ]2[s]    [ 47] 48 | 49] 49] 48] 47] . etl 06000

Even OFDM symbol

(Odd OFOM symbol

ㅣ
Frequency Time domain          FDS & TOS)

“sy

(a) 53,3Mbps, 80Mbps (QPSK, FDS, TDS)

때 기 기

oe @ 197] 198] 199] so
bits

sprea

Subcarrier Mapping

086
1977001
‘Subcarrier Mapping

3099                = = ___ _       =       PRL)
>|           Odd OFDM 50001

Even OFDM symbol

[o]:[2[s |e . «| 97 | 98] 99

Time domain                                                                                                                  >

(b) 106,7Mbps, 160Mbps, 200Mbps (QPSK, TDS)

| 0 | 1 | 2 | 3                 100] 10%] «  ㆍ 이15915  oe 198] 199] <2

50] 51] « ee

이디                 | 49 | 47 | 48 | 49

AS  ieleisis!

>|

(c) 320Mbps, 400Mbps, 480Mbps (DCM)

Imag{a{k]}                                              Imag{a{k+50}}
A                                                      4
[h(gtk)), b(g(ky+1), 0000+50) 66051) ]                                              [b(g(K), bl gtk+ 1), b(@()+50), b(gk}+51) ]
e        e +3 0        e                           e         e +3 @         ㆍ
0011      0111     1011      1111                        0110      1110     0010     1010
           e +1 @           e                                   e           e +1 @           e
0010     0110     1010     1110                        0100      1100     0000     1000
<I        =         +         +—> 604}        <r         +         }         > Re{q{k+50]}
-3        -1        1         3                          -3        -1         1         3
e      e +-1e      °                  e      e  +-1e      °
0001      0101     1001      1101                        0111      1111     0011      1011
ㆍ        e +-3*        e                           e         e +-3¢         ㆍ
0000     0100     1000     1100                        0101      1101     0001      1001
「                                                      v

(0) DCMS] 입력 비트 매핑

그림 17.7 데이터 전송 속도에 따른 입력 비트 맵핑, 부반송파 할당, Domo] 입력 비트 맵핑

601


===== PAGE 598 =====
 .  18-야미/의 동기화 절차

MB-OFDMo}\2] 동기화 및 채널 FAL 프리앰블을 이용하여 수행한다. 80144-
386에 주어진 PES ADAG 사용하여 패킷 획득과 검출, 대략적 bah 주파수 추정, 대

AAS 수행하며, CE 시퀸스를 사용하여 채널의 주파수 응답 추정, 미
세 반송파 주파수 추정, 미세 심볼 타이밍 추정을 수행할 수 있다.

YEA
킷 획득과 ASS 수행하여 패킷의 시작점과 해당 피코넷이 사용하는 TECH 검

우선 패

출하는 것이 바람직하다. 패킷 획득을 위해서는 윈도우를 이용한 전력 기반 4 a Al

호를 이용한 자기 상관 방식, 수신 신호와 훈련 ASS 이용한 상호 상관 방식을 사용할

수 있다. TEC ASS 위해서는 주어진 에 따라 피코넷이 전송하는 기준 시간영역 시
A                                                  °

로          =
시퀸스의 부호를 이용하는 방법을 통해 복잡도를 감소시킬 수 있다. 그림 1782 TEC}
1인 경우에 피코넷이 사용하는 기준 시간영역 시퀸스의 상관 결과(상)와 기준 시간영역
ABA ABA VES 이용한 상관 결과(하)를 비교하여 보여준다. 이 그림으로부터
부호만을 이용한 상호 상관의 경우에도 우수한 상관 특성을 유지하는 것을 알 수 있다. 위

와 같은 방식을 ALT 경우에 최소 한 심볼을 사용하여 패킷 획득과 TEC ASS 수행할
A
a\=

eel (base time domain sequence)

_        |        $ | — correlation (56666 (n), Sbase 00)
(aa         1         '
을 100녀어이2서91겨뽀글 이이 aa           ‘aaa
2         :          :                   |         !
a oe a ee ae one
7p)         i          ;                   i          1

0|   !         후   ? 00 00020 0,

-100       -50        0        50        100
sample offset

_ | — correlation (Sbase(n), Sign(Spase(n))
om
5 100
mse)
2
OSs (| ee ee ee ee ee
a
oO

0                                                 J

-100      -50       0       50       100
sample offset
그림 17.8 기준 시간영역 시퀸스의 SEAATFC = 1)

602



===== PAGE 599 =====
제17장_\46-00ㅁ1 시스템

패킷 획득과 TFCS YS 이 후에는 에 따라 주파수 호핑을 하면서 ABS 수신
하며, 각 대역을 통해 수신된 PSS  sae CFOS 추정한다. PFSS] 경우 동일한 심볼
을 cover 시퀸스에 0 부호만 변경하여 전송하므로 동일 대역을 통하여 수신되는 심볼
의 자기 상관을 사용하여 CFOS 추정할 수 있다. 이 경우 CFO 추정 범위의 최대 크기
(의 )는 {128 (m)}(2mDx165) 7} 되어 반복되는 심볼 간격(22 )이 최대 값인 3을 갖는
경우 0.1293이 된다. 이러한 추정 범위는 420 ppm] 오차 범위를 갖는 발진기를 고려할
때 가장 높은 주파수 대역의 반송파 주파수(10,2961480/에서 발생 가능한 CFOS] 범위인
—0.0998 ~0.0998 (=(f. x (£20) x10 x 2)/Af )를 포함하기 때문에 CFO #44] 어려움
이 없다.

패킷 획득 과정에서 추정한 시간 동기는 정확도가 낮기 때문에 FFT 시작점을 찾기 위
해서 CFO 추정 절차 이후 CFO7} 보상된 신호에 대해 미세 타이밍 동기 추정 절차를 수
행하며, CES] 시작점을 찾기 위해 cover 시퀸스를 이용하여 프리앰블 내에서의 시간 동기
를 획득한다. CE ADAG 시작점을 찾은 후 CE 시퀸스를 이용하여 채널 추정을 수행하
고 심볼을 복조한다. 데이터 심볼 시 함께 전송되는 welse 잔류 CFO] 의해 발생되는
상 추적을 위해 사용된다. 상기 설명한 MB-OFDM] 동기화 절차 이외의 동기화
알고리즘과 성능은 15장에서 설명한 IEEE 802.118에서의 내용과 유사하기 때문에 본 절
에서는 생략한다.

=

603


===== PAGE 600 =====
GREED swe 시스템 기요 -

휴대 인터넷은 “휴대 인터넷 단말기를 이용하여, 정지 및 이동 중에도 언제, 어디서나,
고속으로 무선 인터넷이 가능한 서비스“를 제공하며, 전송 속도, 이동성, 셀 반경 등의
면에서 이동통신 단말기와 무선 랜의 중간 영역에 위치하고 있으며, 1p 기반의 초고속
터넷과 이동통신이 결합한 형태의 새로운 서비스로 “유선 인터넷 서비스의 공간적 제약"
과 “이동통신 인터넷 서비스의 낮은 전송 속도 및 높은 요금”의 단점을 극복할 수 있는
유무선 통합형 서비스이다. 와이브로(\161655 Broadband Internet: WiBro)= 휴대 인터
넷 서비스의 명칭으로, 도심지역에서 대중교통 주행속도의 SYS 보장하고 높은 수준
의 전송속도로 초고속 인터넷과 멀티미디어 이용이 가능한 특징이 있다. 그림 18.1은 와이
브로를 포함한 무선 데이터 서비스의 AS SES 이동성을 비교하여 보여준다.

ro |e

이동성

그림 18.1 와이브로 시스템의 전송 속도 및 이동성

604



===== PAGE 601 =====
제18장_ 와이브로 시스템

와이브로는 한국정보통신기술협회(11&)를 중심으로 2003년 7월부터 2.3GHz 휴대 인
터넷 프로젝트 13(PG302)°] 결성되었으며, 와이브로 서비스를 위한 2단계 국내 표준
HA 제정 및 개정과정을 거쳐 2005년 말에 휴대 인터넷 표준을 완성하였다[313]. 국내
표준화 작업과 병행하여 와이브로 기술은 88 802.166 규격에 반영되었고, 2006년 9월
에 ITU-R WP8A]A] 와이브로 기술이 반영된 TERE 802.16-2004 및 IEEE 802.166-
2005 규격이 무선 광대역 접속 표준의 참조 표준이 되었다[315]. 2007년 1월 ITU-R
WP8F 회의에서 와이브로 기술이 반영된 IEEE 802.160/6 규격 기반의 모바일 와이맥스
(Mobile WiMAX) 기술이 ‘OFDMA TDD WMAN’°]z}= 이름으로 IMT-2000 기술 중
하나로 ITU] 제안되었고, 2007년 10월 제네바에서 개최된 &^&-07에서 모바일 와이맥스
가 국제 표준으로 채택되었다[314].

와이브로와 TEEE 802.166의 관계를 살펴보면, IEEE 802.166는 2~6GHz2] 면허 대역
(license band)= 사용하도록 규정하고 있으며, 단일 반송파 방식, OFDM, OFDMA PHY
WES 지원하며, IEEE 802.16-2004를 기반으로 차량 이동 SES] 이동성은 지원한다.
그리고 소프트 핸드오버와 하드 핸드오버를 지원하고, 슬립 모드, idle 모드, MBS,
매자 Base Station Switching) 등을 지원한다. 와이브로는 1008 802.166의 일부 기
으 지원하는 부집합(606960으로 IEEE 802.16e9} 완벽한 상호 호환성을 가진다. 와이브

표 18.1 와이브로 파라미터

시스템 대역폭(유효 대역폭)                10MHz(8,75MHz)
샘플링 주파수                            10MHz
샘플링 간격                         100nsec
FFT 크기                                 1024
사용된 부반송파 개수(8080)                        841
데이터 부반송파 개수(60080)                      720
TYR 부반송파 개수(8080)                      120
부반송파 간격                            9,765625KHz
유효 심볼 시간                           102.408
시간                              12, 8us
OFDM 심볼 시간                             115 208
프레임 길이                         5ms (42 심볼)

605



===== PAGE 602 =====
PART IV_MIMO-OFDM 통신 시스템

로는 2.3GHz2] 면허 대역을 사용하며, IEEE 802.166의 세가지 PHY 모드 중 OFDMAPHY
모드 만을 지원한다. 6000의 이동성을 지원하며, IEEE 802.166에 포함 된 성능 향상 기능

일부만을 사용하도록 되어있으며, 하드 핸드오버를 지원한다. 와이브로는 이중화 방식으
로는 TDD YAS 사용하고, 주파수 재사용을 1을 사용하여 스펙트럼 효율이 높다. 표 18.1
은 와이브로에서 사용되는 주요 파라미터를 보여준다[316].

와이브로 시스템은 2.3GH2~-24GHz YAS 사용하며, 그림 18.29} 같은 주파수 배치
구조를 가진다. 와이브로는 3개의 사업자가 사용할 수 있고, 각 사업자는 OMHZ2) 3개의
WES 사용한다. 각 사업자 간에는 4.55482의 보호 대역이 존재하고, 다른 대역(2.4082)
과의 간섭을 방지하기 위해 10\082의 보호 대역을 사용한다.

A Operator                      B Operator                       C Operator

1363         2372          2381

2309         2318      23227 12331.5     2340.5     2349.5 2358.

Al           A2           A3                Bi           B2           B3               Ci           02           08

C: 27 MHz BLOCKS
CONSISTING OF (3) 9 MHz
CHANNELS EACH

B: 27 MHz BLOCKS
CONSISTING OF (3) 9 MHz
CHANNELS EACH

4.5 MHz                                4.5 MHz                                  10 MHz
GUARD                               GUARD                                  GUARD
BANO                                 BAND                                    BAND

그림 18.2 와이브로 주파수 배치도

00300 es 구조

와이브로 시스템의 한 프레임은 하향링크 서브프레임과 상향링크 서브프레임으로 구성
되며, 한 프레임의 길이는 508이다. 하향링크 서브프레임은 프리앰블과 하향링크 2060
볼로 구성되고

두 심볼, 그리고 24개의 데이터 심볼로 이루어지며, 총 27개의 OFDMA 심볼로
상향링크 서브프레임은 세 개의 상향링크 PUSC 심볼과 12개의 데이터 ASH 구성되며,

ㅇ

총 15개의 OFDMA ABS 구성된다. 따라서 와이브로 시스템의 하나의 프레임은 총 42

606
SIE = --



===== PAGE 603 =====
제18장_ 와이브로 시스템

개의 심볼로 구성되며, 하향링크와 상향링크 비가 27 대 15가 된다. 와이브로는 TDD 구
조이므로 하향링크와 상향링크 비는 추후 변경 가능하다.

그림 18.3에 나타난 바와 같이 와이브로 프레임은 앞 부분에 하향링크 서브프레임이 위
치하고 그 후에 상향링크 서브프레임이 위치한다. 하향링크 서브프레임의 A 심볼에는 =
리앰블이 위치하고, 프리앰블 다음 2080 두 심볼에는 FCHS} 하향링크 MAP, 상향링크
MAP 정보가 맵핑된다. 그 후에 에서 지정한 위치에 각각의 데이터 버스트가 존재한
다. 상향링크 서브프레임의 처음 세 ASS 상향링크 제어 신호를 전송하기 위한 심볼이
다. 따라서 상향링크 첫 세 심볼은 레인징 채널과 00) 채널, ACK/NAK 채널이 위치하며,
그 뒤의 12개의 심볼에 상향링크 데이터 버스트가 존재한다. 하향링크 서브프레임과 상향
링크 서브 프레임 사이에는 TTG(Transmit/receive Transition Gap)o] 존재하며, 상향링크
서브프레임 다음에는 RTG(Receive/transmit Transition 080)이 존재한다. TTG 값과
RTG 값에 대해서는 뒤에 설명한다.

OFDMA Symbol Number

k+5 | k+7 | k+9  kH11 | kH14 | +17  k+21 k+22  |바24

|

UL-Burst#1

DL-Burst#3                                                   |.

UL-Burst#2

OL-Burst#1

DL-Burst#4               UL-Burst#3

Subchannel Logic Number

UL-Burst#4
DL-Burst#2
DL-Burst#5

UL-Burst#5

~

116

OL                            UL
그림 18.3 논리적 프레임 구조

그림 18.4에 나타난 바와 같이 sega Al 번째 심볼에는 항상 프리앰블이 위치하며
시간 동기 및 주파수 동기 수행 목적으로 사용된다. 프리앰블 이후의 2개의 심볼은 PUSC
심볼을 사용하고 이를 A 번째 2080 BS (First PUSC 2006)이라 명한다. 프리앰블 이후
에 FCHS} 하향링크 MAP, 상향링크 MAPS] 전송되는데, 셀내의 단말은 이 정보를 정

나

te

607 |



===== PAGE 604 =====
PART IV_MIMO-OFDM 통신 시스템

| 복조해야만 데이터 복조가 가능하다. 이를 위하여 셀내의 각 섹터에서 서로 다른 세그
IDS 가지는 프리앰블을 할당하여 전송하고, 단말은 프리앰블을 통해 세그먼트 DS
하고 세그먼트 10에 따른 부채널 집합에서 FCHS} 하향링크 MAP, 상향링크 MAPS
한다. PUSC 심볼 구조는 세그먼트 12에 따라서 서로 다른 부채널 집합을 생성하기
문에 세그먼트 10가 섹터마다 다르다면 각 섹터에서 전송하는 FCHS} MAP 정보 간에
간섭이 발생하지 않는다. 이와 같이 섹터간 간섭 또는 셀간 간섭을 고려할 경우에 FCHS}
MAPS] 전송에 2080 심볼 구조가 적합하기 때문에 프리앰블 이후의 제어 정보 신호 전
송에 PUSC 심볼 FAS 사용한다.

Ol

본

Ac 0!!!

ae i i

5 ms
하향 구간                         상향 구간
빈 76                  타일 빈 RIG
대역 0           늘빼                                    ㄷㅠㅜㅠㅜ
대역 1            21 、
=           co                             ===
대역 3          | ~                             ea os oe
대역 6-2        기 기          -            [ens coves ese [sos oes
Fr Ll                         Sa ie
CHS B-1         | 거 ,                            SSS SE —
TT          그            가           더해
PUSC 부채널 구간 | AMC 부채널구간 상향 제어심볼 구간  |      AMC 부채널구간
다이버시티 부채널구간                 다이버시티 부채널구간

그림 18.4 물리적 프레임 구조

첫 번째 PUSC 영역 이후의 데이터 심볼 구간에는 다이버시티 채널인 PUSC, FUSC,
OFUSCS] 부채널 구간이나 밴드 AMC 부채널 구간이 위치할 수 있다. 상향링크 서브프
레임 구간의 처음 3 ALS 제어 신호 ASS 위한 구간이고 2050 심볼로 구성된다. 상
향링크 제어 심볼 전송 구간 이후에는 다이버시티 채널인 PUSC, OPUSC 부채널 구간이
나 밴드 AMC 부채널 구간이 위치할 수 있다. 이렇게 다양한 심볼 구조가 사용되는 것을
다중 SA(Multiple 2000)이라 하고, 영역의 천이는 하향링크 MAPo|A] STC _DL Zone IE
또는 AAS DL 때에 의해 지시된다.

608



===== PAGE 605 =====
제18장_와이브로 시스템

DL Subframe                                                               UL Subframe

PUSC
(IDCell X)
Sous oes aes
Si pet hy Eh merle

그림 18.5 프레임 내의 다중 SS

FCH® Frame Control Header2] 약자로서 하향링크 Al 번째 PUSC 구간에서 4개의 부
채널을 점유하며, 하향링크 프레임 prefix(DL_Frame_Prefix) 정보가 『01에 맵핑된다.
향링크 프레임 prefix: 표 18.2와 같이 정의된다.

OM

= 18.2 하향링크 프레임 prefix

DL Frame_Prefix_format() {

Bit#0: Subchannel group 0

Bit#1: Subchannel group 1

Bit#2: Subchannel group 2

Bit#3: Subchannel group 3

Bit#4: Subchannel group 4

Bit#5: Subchannel group 5

reserved                       1     Shall be to be zero
QbO0O-No repetition coding on DL—MAP
Ob01—Repetition coding of 2 on DL—-MAP

Used subchannel bitmap                     6

Repeeion ea 에      ㆍ 라비 codeea of 4 on- DLEMAP
Ob11—Repetition coding of 6 on DL—MAP
06000-00 encoding used on DL—MAP
0b001-BTC encoding used on DL-MAP

:      Jett,                        0b010—CTC encoding used on DL—MAP

Coding Indication                 3                       i
0b011-—ZT CC encoding used on DL—-MAP
Ob100-LDPC encoding used on DL—-MAP
0b101 to 06111 - reserved

DL_MAP Length                  8

reserved                         4

}

609



===== PAGE 606 =====
PART IV_MIMO-OFDM 통신 시스템

하향링크 프레임 0ㅁ60%는 총 24개의 비트로 구성된다. 이 중 Used subchannel bitmap?
첫 번째 PUSC 영역과 STC _DL Zone IE()OA ‘use all SC’ 지시자가 “0'의 값을 갖는
PUSC 영역에서 사용되는 부채널 그룹을 표시하는 비트맵으로, ‘VS 이 세그먼트에서 사
용하는 부채널을 나타내고, O'S 사용하지 않는 부채널을 나타낸다. Repetition Coding_
Indication®. 하향링크 MAPo} 사용되는 반복 부호의 BAS 나타낸다. yo] “0'이면 반복
BES 사용하지 않는 것이고, '1'이면 한번의 추가 반복, '2"이면 3회 추가 반복, '3"이면 5
회 추가 반복을 의미한다. Coding 100108000은 하향링크 MAP] 사용되는 FEC 부호화 방
식을 표시한다. 하향링크 MAPS 부호을 1/29] QPSKS 변조되어 전송된다. 기지국은 필수
부호화 방식(컨볼루션 부호화)만 지원하는 단말의 동작에 문제가 없도록 하향링크는 필수
부호화 방식으로만 전송한다. DL_MAP Length= 반복 부호가 적용된 후의 DL_Frame_
Prefix] 바로 이어서 전송되는 하향링크 MAP 메시지의 길이를 슬롯 단위로 표시한다.
하향링크 프레임 prefix’: 그림 18.6에 나타난 바와 같이 『08에 맵핑되기 전에 FEC
소 블록 크기인 48 비트로 만들기 위해 2번 반복되고, Bos 1/29] tail-biting AS
루셔널 부호화를 거쳐 96 비트로 구성된다. 이 ASS QPSK 변조하여 48개의 QPSK 심
볼을 구성하고, 이것을 4번 반복시켜 192개의 QPSK ABS 생성하여 4개의 부채널에 할
당한다. 그림 18.6은 반복에 따른 상관 특성을 보여주는데, QPSK 변조 후에 4번 반복되
기 때문에 최종적으로 8번 반복되는 모양이 나타난다.

에

Correlation-FCH 48 bits(2 Repetition)

0 0               10              20              30              40              50              60              70              80
Correlation-Code FCH 96 bits

1                                                T
‘|       |                    |    |
0                              50                              100

Correlation-Coded FCH 388 bits(4 Repetition

1                     3                   T                   T                   T                   T                   T                   T
0             50           100          150          200          250          300          350

400           450

그
그림 18.6 『애에 할당하기 위한 DL_Frame_Prefix 구성 절차와 반복 패턴

610



===== PAGE 607 =====
제18장_ 와이브로 시스템

PUSC 영역에서 하나의 부채널은 총 48개의 부반송파로 구성된다. 따라서 QPSK 변조
되고 반복된 하향링크 프레임 prefix: 총 192개의 QPSK 심볼로 구성이 되고 이는 4개의
부채널에 나누어 할당된다. 그림 18.7은 3개의 세그먼트를 갖는 경우에 PCH 할당 방법을
보여준다. FCH 이후에는 하향링크 MAPo] 맵핑된다.

L       1

OFDMA symbol! Index
L       L       ㅣ      ny       L

Segment 0
FCH

Segment 1
FGH

Subchannel Index

Segment 2
FCH

Downlink
그림 18.7 FCH 할당 (3 세그먼트)

그림 18.8에 나타난 바와 같이 TTGS} RIGE 최종적으로 87.208와 74.408로 설정되었
다. 이는 초기 레인징을 통한 단말의 타이밍 조절시 셀내 최단 거리 및 최장 거리에 위치
한 단말들의 전송신호 지연시간을 감안하고, 중계기의 커버리지, 기지국에서의 scheduling
processing 시간, 단말에서의 처리 시간을 고려하기 위한 것이다.

ㅣ                  Frame Duration = 5 msec                —
들                                                        ^
RTG                                    TG
<                                  < >

기지국 air 신호         Rx                           1X  |                           Rx
광선로를 통한                                       |
중계기 신호                             이                        os
기지국 처리
TIMING

그림 18.8 716와 RTG

611



===== PAGE 608 =====
PART IV_MIMO-OFDM 통신 시스템

COE cow! 부반송파 할당

와이브로에서 사용하는 채널은 다이버시티 채널과 밴드 AMC 채널이 있다. 다이버시티
채널에는 하향링크에서 사용하는 PUSC, FUSC, OFUSC7} 있으며, 상향링크에서 사용하
는 2080, OPUSC7} 있다. 인접 부반송파를 사용하는 밴드 AMC 채널은 상향링크와 하
향링크에 모두 사용된다. 표 1832 와이브로에서 사용되는 다이버시티 채널과 밴드
AMC 채널의 구성과 BES 나타낸다.

표 18.3 다이버시티 채널과 밴드 AMC

PUSC      Scattered 48 tones     i = 5)
|                                              Data 전송
a      FUSC      Scattered 48 tones       Data 전송, 디지털 방송
08080     Scattered 48 tones       Data AS, 더지털 방송
Uplink      PUSC  6개의 분산 타일, 8톤/타일     Data 전송, 다이버시티
08080  6개의 분산 타일, 8톤/타일     Data 전송, 다이버시티
06001. 23400 ' ㅣ eq Sat 빈, exp) 001 oe ae

표 184% 하향링크에서 사용되는 다이버시티 채널과 밴드 AMC 채널의 주요 파라미터
를 보여준다. 밴드 4140는 상향링크와 하향링크에 동시 적용된다. 표 18.5는 상향링크에
서 사용되는 다이버시티 채널의 주요 파라미터를 보여준다.

표 18.4 하향링크 채널의 주요 파라미터

No, of Left Guard Subcarriers                          80
No, of Right Guard Subcarriers      91        86        19         79
No, of Used Subcarriers (no DC)     840       850       864        864
No, of DC Subcarrier (#512)        il         1         1         1
No, of Pilot Subcarriers        120       82        96        96
No, of Data Subcarriers        720       468       768       468
No, of Subcarriers per Subchannel     48        48        48         48
No, of Symbols per Subchannel      2        il        1       2206
No, of Subchannels / Symbols     30/2       16       16    48788, 6
Pilot Configuration         Common   Common   Common    Dedicated

Data Configuration       Distributed Distributed Distributed Adjacent



===== PAGE 609 =====
제18장_ 와이브로 시스템

표 18.5 상향링크 채널의 주요 파라미터

No, of Left Guard Subcarriers         |    92                80

No, of Right Guard Subcarriers             91                79
No, of Used Subcarriers (no DC)           840              864
No, of DC Subcarrier (#512)          |    1                i
No, of Tiles                   210              288
No, of Pilot Subcarriers per Tile             4                 1
No, of Data Subcarriers per Subchannel          8                 8
No, of Tiles per Subchannel               6
No, of Pilot Subcarriers per Subchannel         24
No, of Data Subcarriers per Subchannel         48                48
No, of Subchannels / Symbols          83883           48 / 3

하향링크 2080 심볼은 1024개의 부반송파중 841개의 부반송파를 사용하고, 나머지
183개의 부반송파는 보호 부반송파로서 왼쪽에 92개, 오른쪽에 91개를 사용한다. 유효 부
반송파는 841개이고 1개의 DC 부반송파와 120개의 wpelel 부반송파와 720개의 데이터
부반송파로 구성된다. 하향링크 PUSC YRS 클러스터(60960 단위로 이루어지며 하향
링크 2080 심볼에는 60개의 클러스터가 존재하고, 30개의 부채널이 존재한다. 그림 18.9
에 나타난 바와 같이 하나의 클러스터는 주파수 축으로 14개의 부반송파, 심볼 축으로 2
개의 ABS 구성된다. 한 프레임에서 프리앰블은 심볼로 간주하지 않기 때문에 프리앰블
이후의 첫 번째 심볼이 0번째 심볼이 된다. 따라서 하향링크 2080 심볼에서 클러스터를
구성하는 첫 번째 심볼이 짝수 심볼이 되고 그 다음 심볼은 홀수 심볼이 된다. 짝수 심볼
에서 BES 부반송파는 4번째와 8번째 부반송파에 위치하며, 홀수 심볼에서 wpo]sl 부반
송파는 0번째 부반송파와 12번째 부반송파에 위치하게 된다.

와이브로 시스템에서 데이터 할당은 부채널 단위로 이루어진다. 부채널은 부반송파으
집합이며 하향링크 2090에서 하나의 부채널은 각 심볼 당 24개씩, 총 48개의 데이터 부
반송파로 이루어진다. 하향링크 2080 심볼에서 부채널에 대한 반송파 할당 방식은 다음
과 같다.

se

613



===== PAGE 610 =====
PART IV_MIMO-OFDM 통신 시

Time

Odd Symbol

Even Symbol

Freq

Pilot Subcarrier                                     Data Subcarrier

그림 18.9 하향링크 PUSC 클러스터 구조

PUSC 심볼에서 반송파 0번부터 시작하여 14개의 인접한 부반송파를 포함하는 60개의
클러스터를 생성한다. 생성된 60개의 물리적 클러스터를 논리적 클러스터로 생성하기 위
하여 다음의 AS 사용하여 클러스터 WSS 재지정한다. 첫 번째 PUSC 영역이나 “Use
all SC? indicator=0@) 경우에는 식 (18.1)을 사용하여 클러스터 WSS 재지정한다.

Logical Cluster = Renumbering Sequence(Physical Cluster)                                (18.1)

그리고 첫 번째 PUSC 영역과 ‘Use all SC’ indicator=0¢! 경우
(18.2)를 사용하여 클러스터 번호를 재지정한다.

때

제외한 경우는 식

Logical Cluster = Renumbering Sequence(Physical Cluster + 13* DL_PermBase)mod60 (18.2)

Al 번째 PUSC 영역과 ‘Use all SC’ indicator=02] 경우에는 규격에 주어진 renumbering
시퀸스를 사용하고, 그 외의 경우에는 STC_DL_ZONE 18()나 AAS 101. 18()에 정의된
DL_PermBase 파라미터를 사용하여 renumbering 시퀸스를 생성한 후 클러스터 WSS
재지정한다.

번호가 재지정된 클러스터는 다시 그룹으로 할당된다. 60개의 클러스터를 6개의 그룹에
나누어 할당하게 되는데 그룹 0은 클러스터 0-11, 그룹 1은 클러스터 12~19, 그룹 2는 클
러스터 20~31, 그룹 3은 클러스터 32~39, 그룹 4는 클러스터 40~51, 그룹 5는 클러스터
52~59로 구성된다. 그룹 0, 2, 4는 12개의 클러스터로 구성되며, 그룹 1, 3, 5는 8개의 클
러스터로 구성된다. 세그먼트가 사용될 때 이 그룹들은 세그먼트에 할당되고, 적어도 하나
의 TBS 하나의 세그먼트에 할당이 된다. 기본적으로 그룹 0은 세그먼트 0번에 할당되
고, 그룹 2는 세그먼트 1번, 그룹 4는 세그먼트 2번에 할당된다. 서로 다른 그룹을 같은
세그먼트에 할당하지 않기 때문에 하향링크 2080 심볼 구조에서 각 섹터에서 사용하는
세그먼트가 다르면 섹터간 간섭이 발생하지 않게 된다[318].

614



===== PAGE 611 =====
제18장_ 와이브로 시스템

클러스터 그룹을 생성한 후, 각 그룹 내에서 부채널에 부반송파를 할당하는 것은 우
} OFDMA 심볼에 대하여 별도로 개별 클러스터 내의 vole 부반송파를 ager 후
|볼 내의 잔여 데이터 부반송파에 대해 할당을 하게 된다. 부채널에 데이터 부반송파를
할당하기 위해서 그룹 0에 존재하는 데이터 부반송파를 24개의 그룹으로 분할하고, 그룹
1에 존재하는 데이터 부반송파 역시 24개의 부그룹으로 분할하고, 그룹 2, 3, 4, 5에 대해
서도 데이터 부반송파를 각각 24개의 부그룹으로 분할한다. 다음 식에 따라 24개의 부그
룹에서 하나의 부반송파씩을 취하여 부채널을 생성하면 심볼 당 24개의 데이터 부반송파
로 이루어진 부채널이 생성된다.

oy N

에

xn, +{P.[n, mod N

subchannels
xn, +4 P.|n, mod N.
k   i$  k

subchannels

]+ Deell| mod N.

subchannels

]+ DL _ PermBase}mod N

subchannels

First DL zone (1 8,3)

N sitenaniats

subcarrier(k,s) = |                                                                                                               —
otherwise

subchannels

여기서 permutationBaseb6 = {3,2,0,4,5,1}, permutationBase6 = {3,0,2,1} 이다.

식 (18.3) A], subcarrier(k, 9)는 BAS 8에서 부반송파 《의 인덱스, ^, 은 전
Al 부채널의 개수, 0 는 부채널에 할당된 부반송파 수, 는 ^. 의 범위
갖는 부채널 인덱스, 《는 부채널 0~#*,』.647새의 부반송파 인덱스, FL] 기본
열 A;AA(PermutationBaseé 또는 PermutationBase4)\S 왼쪽으로 53) 회전하여 얻은
수, ceil [JE []의 정수값에 대하여 다음 정수까지의 인수를 반올림한 값이다. 또한, m

(6 +13ㆍ5)000.74,,., ,, 연산의 결과값, subcarrier(k,s) = 부채널 8에서의 부반송파
《의 인덱스, DL PermBase= 0~31 사이의 정수이다. Al 번째 PUSC 영역에서는 120811을
사용하여 부채널을 생성하고, 그 외에는 DL PermBaseS 사용하여 HAYS 생성하며,
그룹 0, 2, 4는 PermutationBaseéS, 그룹 1, 3, 5는 PermutationBase4S 사용한다.

그림 18.10은 하향링크 0090 부반송파 할당 절차를 요약하여 보여준다. 이 그림에 나
타난 바와 우선 클러스터 그룹을 생성한 후, 클러스터 그룹에서 24개의 부그룹을 생성하
고, 각 부그룹에서 하나의 부반송파를 선택하여 부채널을 형성한다. 이와 같이 클러스터
번호의 재정의를 통해 전체 대역에 부반송파가 클러스터 단위로 퍼져서 할당되기 때문에
하향링크 PUSC HSS 다이버시티 채널이 된다. 클러스터 번호 재정의 이후 부분부터 세
그먼트가 적용되어 부반송파가 부채널에 할당되기 때문에 섹터간 세그먼트가 다를 경우에
는 부반송파 충돌이 발생하지 않는다.

fle och AY oo



===== PAGE 612 =====
PART IV_MIMO-OFDM 통신 시스템

Subcarriers             에
:      !    tone    ca    | 97095
0      1       2          59
o~t1 | 12~19

oa

San 게드

groups           groups | rol
Segment 0                  Segment 1                  Segment 2

그림 18.10 하향링크 PuSC 부반송파 할당 절차

그림 18.11은 인접한 셀 A (IDcell=0)2} 셀 8 (00061=32)에서 동일한 PUSC
101. 『260008886(011)를 사용한 경우에 셀 경계지역에서 충돌0410이 발생하는 데이터 PUSC
영역의 부반송파 인덱스를 보여준다. 두 셀에서 사용하는 부채널이 겹치지 않을 경우에는
충돌이 발생하지 않지만, 이 그림에서와 같이 일부의 부채널이 겹칠 경우에는 충돌이 발
생함을 알 수 있다.

Cell A (IDcell = 0)

0      100 200 300 400 500 600 700 800 900 1000
Subcarrier Index

Cell B (IDcell = 32)

300 400 500 600 700
Subcarrier Index
Hit Distribution in PUSC

0 100 200 300 400 500 600 700 800 900 1000
Subcarrier Index

그림 18.11 셀 경계지역에서 PusC 부반송파 SS 모의실험

616



===== PAGE 613 =====
제18장_ 와이브로 시스템

 하향링크 7060

하향링크 8080 심볼 구조는 1024개의 부반송파 중에 851개의 부반송파를 사용한다.
보호 부반송파는 왼쪽에 87개, 오른쪽에 86개가 있고, 851개의 유효 부반송파 중 하나는
DC 부반송파, 768개는 데이터 부반송파이다. 하나의 하향링크 FUSC 심볼에는 16개의
부채널이 존재하며, 하나의 부채널은 48개의 부반송파로 구성된다. 하향링크 8080 심볼
의 soa] 부반송파는 Constant Seti} Variable Set] 있다. Constant Set 11개의 파일
A 부반송파로 구성되며, ae 부반송파의 간격은 72개이다. 그림 17.13에 주어진
Variable Set®- 71개의 HIS 부반송파로 구성되며, 그 간격은 12이고, 매 2 심볼마다 같
은 패턴이 나타난다. Variable Set? 수신단에서 채널 추정을 위하여 사용된다.

Time                                                                                                    ss
(    “)

"                                                              -~                                                                       Freq
&)  Pilot Subcarrier                                        Data Subcarrier

그림 18.12 하향링크 FUSC 구조

하향링크 8080 심볼의 부채널을 생성하기 위해 하향링크 FUSC 심볼의 데이터 부반
송파 768개를 48개의 그룹으로 할당한다. 그 후에 각 그룹에서 하나의 부반송파를 취해
48개의 데이터 부반송파로 구성된 16개의 부채널을 생성한다.

768 data subcarriers                             |

"
cla ate            님 toes 내전 be

a a 가태터
subchannel 2002            as)

그림 18.13 하향링크 FUSC 부채널 생성 절차

하향링크 0080 심볼과 달리 8050 ABS 중간에 IHS 나누고 각 그룹에서 부채널
을 생성하는 방식이 아니기 때문에 세그먼트로 구분이 불가능하다. 그리고 2080 구조는

617



===== PAGE 614 =====
PART IV_MIMO-OFDM 통신 시스템

각 그룹에서 6개, 또는 4개의 부채널을 형성하기 때문에 6개의 부채널을 생성하기 위한
PermutationBase62}+ 4개의 부채널 AAS  _ PermutationBase47} 따로 있었지만
0050의 경우 전체 48개의 그룹에서 하나의 부반송파씩을 취해 부채널을 형성하기 때문
에 하나의 2600041304008886만 사용한다.

그림 18.14는 인접한 A ㅅ&와 셀 에서 Permutation? = FUSCS, 서로 다른
DL_PermBase 파라미터와 다른 부채널 인덱스를 할당한 경우에 대한 셀 경계지역에서의
충돌0810이 발생하는 부반송파 인덱스를 보여준다. DL _PermBase7} 같고 서로 다른 부채
널을 사용하는 경우에는 충돌이 발생하지 않으나, 아래와 같이 DL_PermBase7} 다를 경
우에는 부채널 할당량과 할당된 부채널에 따라 충돌 확률이 달라진다.

~ AC (OL PermBase = = 13)

 “100 200 300 400 500 600 700 800 900 1000
Subcarrier Index

Cell Bi  SLU as    a

100  “200  ~ 300      500  600
*Gibcaver Index

Hit Distribution in FUSC

0          100 200 300 400 500 600 700 800 900 1000
Subcarrier Index

그림 18.14 셀 경계지역에서 FUSC 부반송파 충돌 모의 실험

00609 상양링크 2056

상향링크 2080 ASS AS] 92개의 보호 부반송파를 할당하고, 오른쪽에 91개의 보
부반송파를 할당하며, 841개의 유효 부반송파를 사용한다. 상향링크 2080의 기본 단
는 타일(1116) FAS 구성되며, 하나의 2080 심볼에 210개의 타일이 존재하고, 35개
부채널로 구성된다. 그림 18.15(8)에 나타난 바와 같이 상향링크 2080 심볼에서 타일
주파수 FOB 4개의 부반송파와 시간축으로 3개의 심볼로 구성된다. Bag 부반송파
첫 번째 심볼과 세 번째 심볼의 첫 번째 부반송파와 네 번째 부반송파에 할당되며 나

'



===== PAGE 615 =====
제18장_ 와이브로 시스템

머지 8개의 부반송파는 데이터 부반송파이다. 상향링크 2080에서 하나의 슬롯은 3개의
심볼과 하나의 부채널로 구성된다.

Time  A

Time | a=  ~

Data Subcarrier

Nw     .       —     Ge  Pilot Subcarrier

Pred
(a) UL PUSC                            (b) UL OPUSC
그림 18.15 상향링크 타일(116) 구조 (PUSC, OPUSC)

상향링크 ?050에서, 하나의 부채널은 6개의 타일로 구성된다 상향링크 0080 ABS
먼저 210개의 타일로 나뉘어진다. 210개의 타일을 각각 35개의 인접한 타일을 포함하는
6개의 그룹으로 분류한다. 이 때 타일이 연속하는 논리적 인덱스를 가지고 있으면 인접한
것으로 간주한다. 타일을 그룹으로 분류한 후에 규격에 주어진 맵핑 식을 사용하여 논리
적 타일은 물리적 타일로 맵핑하며, 부채널 당 6개의 타일을 선택한다. 논리적 타일을 물
리적 타일로 맵핑한 후, 각각의 타일 내에서 wpe 부반송파를 할당한다. 데이터 부반송
파는 0에서 47로 인덱스화 된다. 그림 18.16은 840개의 부반송파를 가지는 상향링
PUSC 심볼을 210개의 타일로 구성한 후에 35개의 타일을 6개의 그룹으로 할당하여 부채
널을 생성하는 과정을 보여준다. 그림 18.1500)는 상향링크 00080의 타일 FAS 나타
낸다. 하나의 타일은 주파수 축으로 3개의 부반송파와 심볼 축으로 3개의 심볼로 구성되
며, 가운데 부반송파에 wplel 부반송파가 할당된다. 총 288개의 타일이 존재하고 하나의
부채널은 48개의 데이터 부반송파로 구성되며, 부채널당 타일 수는 6개이다. 부채널 할당

절차는 위와 유사하게 수행되어 설명을 생략한다.

tu

840 subcarriers                                        |

|
ere      peat

Tiles                                     @0 0 @                209 | 210tiles
Tile group                                                                                                          ‘| 6 groups
subchannel 35 subchannels

그림 18.16 상향링크 PUSC 부채널 할당 절차

619


===== PAGE 616 =====
PART IV_MIMO-OFDM 통신 시스템

AMC ASS 상향링크와 하향링크에 동일하게 적용된다. 밴드 AMCE 865개의
반송파로 구성되며, 왼쪽에 80개, 오른쪽에 79개의 보호 부반송파가 할당된다. 파

파는 96개가 할당되며, 데이터 부반송파는 768개이다. 밴드 AMCE 총 24개
x — 구성되며, 주파수 축 방향의 4개의 빈(610)으로 구성된 열 AHS 하나
리적 밴드를 구성한다. 또한, 물리적 대역을 합하여 논리적 대역을 구성 가능하며 최
대 12개의 때 ASS 구성할 수 있다. We 그림 18.17(8)에 나타난 바와 같이
OFDMA 심볼 내에서 9개의 연속된 부반송파 집합으로 정의되며, 하향링크 및 상향링크
에서 기본 할당 단위가 된다. BS 부반송파의 위치는 빈의 위치와 심볼의 위치에 따라

결정된다.
bin A
Data tone
symbol
1“                   bin 』
| Pilott
=| Pilo one '
symbol           symbol
(a) 빈 구조                               (06) 부채널 구조

그림 18.17 밴드 AMC 구조

하나의 AMC 부채널은 6개의 연속된 빈으로 구성되기 때문에 48개의 데이터 부반송파
로 이루어져 있다. 그림 18.1706)에 나타난 바와 같이 AMC 부채널은 1 빈 x 6 심볼, 2
Bl x 3 심볼, 3 Bl × 2 심볼로 구성된다. 그림 18.18은 밴드 AMC 구조의 예를 보여준다.
하나의 물리적 밴드는 4개의 빈으로 이루어지며, 인접한 4개의 물리적 밴드가 한 개의 =
리적 밴드를 구성함으로써 총 6개의 논리적 밴드를 나타내고 있다. 또한, 물리적 밴드의
BIAS) 위치가 심볼의 위치에 따라 달라지는 것을 알 수 있으며, 이러한 sada 패턴을
사용하여 데이터 부반송파 영역에서의 채널 추정이 주파수 영역과 시간 영역에서 보간에
의하여 이루어진다.

_ 620



===== PAGE 617 =====
제18장_ 와이브로 시스템

으1          시
의              =
~    ;       0
2     4 bins     &
-| 이를        a
이콘              ©
a7)
>
=
a
| 를                 =
52)
=
oO
=     ㆍ
"     :             =
ㆍ
ㆍ
e _|1 subchannel

그림 18.18 밴드 AMC 구조의 예

18.5.5 Bd ime 자원 할당

하향링크 PUSC, FUSC, OFUSC, 밴드 4140에서 THe] 부반송파는 889 변조되고,
데이터 부반송파에 비해 2.5dB 부스팅되어 전송된다. wale AAA PRBS 생성기에
의해서 생성되며, PRBS 발생 다항식은 식 (18.4)와 같다. 그림 18.19는 PRBS 생성기 +
조를 보여준다.

1+※ +x"                           (18.4)

PRBS 생성기에서 레지스터에 채워지는 초기값으로 60에서 64까지는 12081의 하위 5
비트로 채워진다. 이 때 60는 MSB, 64는 LSBS 나타낸다. 65와 66은 PRBS IDZ 채워
지며, 67에서 610까지는 모두 ‘Ve 채워진다.

MSB                    LSB
610 69 68 67 66 65 64 63 62 61 60

1{ 2] 3] 4] 5[ 6] 7][/8] 9 [10] 1]

out

그림 18.19 PRBS 생성기 구조



===== PAGE 618 =====
PART IV_MIMO-OFDM 통신 시스템

와이브로에서 모든 데이터 할당은 슬롯(900 단위로 이루어진다. 표 18.6은 하향링크와
상향링크의 슬롯 단위를 보여준다. 이 표에서 나타난 바와 같이 PUSC PAS 하향링크에
서는 2 심볼이 슬롯 단위이며, 상향링크에서는 3 심볼이 슬롯 단위이다. 모든 채널 구조에

서 하나의 부채널은 48개의 부반송파로 구성된다.

표 18.6 하향링크와 상향링크에서의 슬롯 단위

2080 1 부채널 (3심볼    1 부채널    PUSC              1 부채널
Fusc 1 부재널 (심볼) 0, 2, 3, 648) OPUSC             (1, 2, 3, 6심볼)

0810144에서 데이터 영역은 그림 18.2006)에 나타난 바와 같이 연속된 OFDMA 심볼 그
룸과 연속된 부채널 그룹으로 구성된 2차원 할당 패턴으로 주어진다. 여기서 연속된 부채널
은 논리적 의미에서의 부채널을 의미한다. 와이브로 시스템의 \14에서 하향링크 버스트는
부채널 옵셋과 심볼 Gs, 심볼 수와 부채널 수로서 2차원적으로 할당이 이루어진다. 그림
18.2006)는 하향링크 PUSC AAS] 자원 할당 예를 보여준다. 하향링크 0050 채널에서는
한 슬롯이 2 ABS 구성되기 때문에 이 그림에서 슬롯 단위로 자원이 PIS 알 수 있다.
그림 18.2006)에서 가늘게 표시된 화살표 방향을 따라 식 (18.3)의 subcarrier(k, 9)를 통해
생성되는 부채널 인덱스 sof] 대한 0~23까지의 데이터 부반송파 인덱스에 데이터가 할당
되며, FA] 표시된 화살표 방향을 따라 부채널의 할당이 이루어지게 된다. 여기서 부채널
은 논리적 부채널을 나타내며, Beals] 위치는 물리적인 위치를 나타낸다.

Time Slot #n          Time Slot #n+1
symbol      No. of                                   공
offset      symbols               eat                +
A
subchannel
offset
=
No. of                                     SCH             >=
subchannels                          # pt         oo
(‘==
(a) 2차원 할당 패턴                06) 하향링크 2080 자원 할당 예

그림 18.20 2차원 할당 패턴과 하향링크 PUSC 자원 할당 예

_ 622



===== PAGE 619 =====
제18장_ 와이브로 시스템

와이브로 시스템의 5440에서 상향링크 버스트는 버스트의 길이(440000)를 나타내는 1
차원 할당 패턴으로 이루어진다. 그림 18.21은 상향링크 2080 채널의 자원 할당 예를 보
여준다. 하향링크 2080 채널에서는 한 SHO] 3 심볼로 구성되기 때문에 슬롯 단위로 자
원이 할당됨을 알 수 있다. 그림 18.21에서 부채널은 논리적 부채널을 나타내고, 검게 표
시된 BRS spls 나타낸다. 또한, BA) 표시된 화살표는 상향링크 2080 채널에서
버스트의 길이를 나타내고, 가늘게 표시된 화살표는 주어진 버스트에 자원을 할당하는 순
서를 보여준다.

Time Slot#n Time Slot #0+1 11006 Slot #n+2 Time Slot #n+3

SCH #p

SCH # p+1

Time

GREELY 이이브로 프리앰블과 orga 동기화

와이브로에서 제공하는 프리앰블 AMAL 114개이고, 한 셀을 3개의 섹터로 분할할 경
우에 각 섹터에 각각 38744) 할당된다. 그림 18.22에 나타난 바와 같이 프리앰블 시퀸스
는 주파수 영역에서 부반송파에 할당되고, 각 섹터에서는 3개의 반송파마다 값이 할당되
어 전체 1024개의 부반송파중 278개의 부반송파에 프리앰블 시퀸스가 할당된다. 서로 다
른 섹터에 할당된 프리앰블 심볼들은 주파수 영역에서 서로 다른 부반송파 위치에서 할당
되어 섹터간에 간섭이 없도록 구성한다. 각 섹터에 할당된 프리앰블은 3개의 부반송파마
다 신호가 실리게 되므로 시간 영역에서 반복적 특성을 갖게 된다. 각 단말에서 프리앰블

을 수신하지 못하면 초기 동기 및 셀 탐색 등을 수행할 수 없고, 핸드오버도 수행할 수 없



===== PAGE 620 =====
PART IV_MIMO—-OFDM 통신 시스템

DC

J      |     1     |      |                     |            i                  |      |      |      |      |             (ieee

|   |   T
511 S12 513

ow
Co
a
oo
a

ee:

a

:segment 0 © ~:segment 1  A: segment 2

그림 18.22 프리앰블의 주파수 영역 구성

개

프리앰블이 셀 경계 지역의 단말에서도 수신이 가능하도록 부스팅(60050108)되
다. 프리앰블 AAAS BPSK 변조되며, 데이터 부반송파에 비해 4.508 부스팅
된다.

와이브로 시스템에서는 위의 프리앰블을 사용하여 동기화 및 셀 탐색을 수행한다.
동기화를 위해서는 위 프리앰블의 시간영역에서의 반복적 특성을 이용하여 우선 대
프레임 검출을 수행한다. 그후 하향링크 신호의 CP(Cyclic Prefix)S 이용하여 좀 더
한 심볼 타이밍 동기화를 이루고 소수배 주파수 옵셋을 추정하여 보상한다. 셀 탐색을 위
해서는 프리앰블의 주파수 영역 ASS 이용한다. 이 때 세그먼트 추정, 프리앰블 인덱스
주정, AHH 옵셋 추정, CINR(Carrier to Interference and Noise Ratio) 추정을 동시에
이룰 수 있다. 초기 동기화가 종료된 이후 동기 추적을 진행한다. 반송파 주파수 옵셋 추

을 위해서는 CPS] 자기상관을 이용하고, 심볼 타이밍 컨트롤을 위해서는 프리앰블의 상
호상관을 이용할 수 있다.

또한 네번째 프레임마다 마지막 OFDMA Ase 공용 동기 심볼(0000000 synch
5900501)로 사용할 수 있다(00000). 공용 동기 심볼은 모든 기지국에서 동일한 시퀸스를
사용하고, 그림 18.23과 같이 구성되어 시간 영역에서 2번 반복되는 특성을 갖게 된다. 공
용 동기 HES 사용할 경우에 A 경계, 특히 3 섹터 경계에서 동기 ASS 향상시킬 수

fe)
있다.

(쓰 Ad

오
2 % 로
of it 으

41

ie

2s

Subcarrier Index

Null Subcarrier

Common Sync. Symbol Subcarrier

ug

그림 18.23 BS 동기 심볼의 주파수 영역 구성

624



===== PAGE 621 =====
제18장_ 와이브로 시스템

와이브로 시스템에서 레인징0808108)은 단말과 기지국간의 상향링크 동기 획득 및 전
력 제어 등의 목적으로 사용된다. 와이브로 시스템의 레인징은 초기 레인징과 핸드오버
레인징, 주기적(6640010) 레인징과 대역폭 요구(6800\1001 request) 레인징의 4가지로 분

인
류된다. 초기 레인징은 초기 망 Ads 상향링크 동기를 위해 사용되고, 핸드오버 레인징
은 핸드오버 도중 BA 기지국에 대한 동기화를 위해 사용된다. 초기 레인징과 핸드오버
|인징의 경우 기지국과의 상향링크 동기화가 전혀 이루어지지 않은 상태에서 수행되므로
연속적인 두 심볼에 같은 SES 실어 레인징 심볼을 구성한다. 그림 18.24는 두 개의
OFDMA 심볼로 구성된 레인징 심볼을 4명의 사용자가 송신하였을 때에 기지국에 도착한
수신신호를 보여준다. 기지국에서 도착한 신호가 모두 FFT 윈도우 내에 수신되어 부반송

파간 직교성을 유지하면서 레인징 심볼를 왜곡없이 복원할 수 WSS 알 수 있다.

=I

6068 |  Ranging Symbol]  」  Ranging Symbol | cs

Ranging Syr

FFT Window       |

그림 18.24 두개의 레인징 심

10
fo)
fe

주기적 레인징은 기지국과 단말간의 동기화 및 전력 제어를 트랙킹하기 위하여 사용되
고, 대역폭 요구 레인징은 단말이 기지국에 자원을 요구할 때에 사용된다. 주기적 레인징
과 대역폭 요구 레인징은 초기 동기화가 이루어진 상태에서 수행되기 때문에 한 개의
OFDMA 심볼로 구성된다. 와이브로 시스템의 경우에 상향링크 제어 채널은 그림 18.25
에 나타난 바와 같이 상향링크 부프레임의 앞의 세개의 OFDMA 심볼로 구성되는데, 초
기 레인징과 핸드오버 레인징 채널은 앞의 두 심볼에 할당되고, 주기적 레인징과 대역폭
할당 레인징 채널은 세 번째 심볼에 할당된다.



===== PAGE 622 =====
PART IV_MIMO-OFDM 통신 시스템

DL       a     UL

그림 18.25 상향링크 제어 채널 중 레인징 채널 구성

레인징 수행시 사용되는 부호는 PRBS 생성기를 통해 발생되고, 발생된 신호를 144 비
트씩 나누어서 부호를 생성한다. 식 (18.5)는 레인징 부호 생성 다항식을 나타낸다.

Lexi txt 수로 +x"                             (18.5)

그림 18.260] 주어진 레인징 부호 발생을 위한 PRBS 생성기의 A7] BLE s6~s0E
UL_PermBase7} 사용된다. 레인징 부호는 889 변조 방식을 사용하여 변조되며, 최대
256개의 레인징 부호가 생성된다.

Ranging Code Generator
LSB s6 65 54 53 52 51 50 1 1 0 1 0 1 0 0 MSB

11] 2] 3| 4| 5] 6| 7| 8] 910] 11] 12] 13/14] 15]

Ck
그림 18.26 레인징 부호 PRBS 생성기

PRBS 생성기를 사용하여 발생하는 256개의 사용 가능한 부호 중 A 번째 개의 부호
는 초기 레인징, 그 다음에 생성되는 WAS 부호는 주기적 레인징, 그 다음에 생성되는
개의 부호는 대역폭 요구 레인징, 마지막 (2개의 부호는 핸드오버 레인징을 위하여 사용
된다. nc 시도할 경우에 단말은 4714] 종류의 레인징 부호 집합들 중 자신의 목적
에 맞는 부호들의 집합에서 하나의 레인징 부호를 임의로 선택하여 12개의 레인징 영역
중 임의의 BAS 선택하여 전송한다. 기지국에서는 각 레인징 영역마다 레인징 부호와의

상호 상관 AW     는 부호에 대해 병렬로 수행하여 가장 큰 상관 값을 갖는 무호를 Al

re
cm

626



===== PAGE 623 =====
제18장_ 와이브로 시스템

택한다. 이러한 일련의 과정(61284 경쟁)을 통해 난발이 레인징을 성공할 경우에 기지국
은           레인징 내며 식별자로 하여 성공한 단말에 대해 응답 메시지를 전송

그
pz
10   oy,
4r
0   에
fo

al      을 종료한다. 이 때 응답 메시지에는 레인징의 목적에 따라 타
이밍, 전력 제어, 대역폭 할당 등의 BRS 담게 되고, CDMA 경쟁에서 레인징에 실패한
난 후에 다시 레인징을 시도하게 된다.

이
x

| 18.5.2 (이! 채널

CQL 채널은 48개의 부반송파로 구성되며 QPSK 변조되어 4비트의 CQ 정보를 ASS
다. 00) 채널은 고속 피드백 채널(009 feedback channel)& 사용할 경우, 단말은 측정한
SNRE 식 (18.6)을 통해 HOSE 비트로 양자화하고, 양자화된 비트 페이로드는 표 18.7
을 이용하여 벡터 인덱스를 구하는 데 사용된다. 그리고 백터 인덱스와 부반송파 변조간
의 맵핑 관계를 이용하여 기지국에 CINRS 보고한다.

0           S/N <-2aB
payload bits nibble=,n 2-n-4<S/N<2-n-2            (18.6)
15          S/N >26aB

Bale     a i |  |  Symbol 0

Subcarrier      Subcarrier      Subcarrier |     Subcarrier
os            ie)            (a)             (5)       Symbol 1
ewes        age                2   :    Symbol 2

Freq

그림 18.27 상향링크 PUSC 타일의 CQI 채널 부반송파 맵핑



===== PAGE 624 =====
PART IV_MIMO-OFDM 통신 시스템

표 18.7 고속 피드백 채널의 부반송파 변조

=     = 본 : : ft           0 PO, Pl, P2, P3, PO, Pl, P2, P3
ad     ‘ : : : : :           1 PO, 28, P2, Pl, PO, 28, P2, Pl
으으     : : 7 은 7 :           2 PO, PO, Pl, Pl, P2, P2, P3, P3
aa     : : : : ; :           3 PO, PO, P3, P3, P2, P2, Pl, Pl
aaa     : ; “ : :           5 PO, P2, PO, P2, PO, P2, PO, P2
aan      ; . : : ;           6 PO, P2, PO, P2, P2, PO, P2, PO
a      ; : - ; i -           7 PO, P2, P2, PO, P2, PO, PO, P2
여기서 각 부반송파에 할당되는 변조 값은 식(18.7)과 같다.

PO=exp(j-%), PL=exp(/: 내
3                                                                                                           (18.7)
P2=exp(-j-—1), P3=exp(-j-4)

밴드 AMC 동작의 경우, 단말은 선택된 4개의 WES] CINR 차이(증가: 1, 감소: 0,
108 단위)를 고속  3)  채널로 보고한다. 확장 고속 피드백 채널의 경우에는 페이로드
비트가 6 비트로 확장된다. 그림 18.28은 CQI 채널의 생성 과정을 보여준다. 고속 피드백
채널의 경우 4비트의 페이로드 비트(확장 고속 피드백 채널의 경우 6비트)를 생성한 후
블록 부호화를 거쳐 6비트의 코드워드를 생성한다. 그 후 생성된 코드 워드를 벡터와 맵
핑시켜 6개의 타일에 할당하여 고속 피드백 채널을 구성한다.

628


===== PAGE 625 =====
제18장_와이브로 시스템

6 Tiles

,a_ 도
^

Fast FeedBack        7               a el        Code Word

Channels     /         bit ee 이              ES |

~
— a       Block Coding f--->
| 를 |

DL

\          erie ss
. =
*, |e
\ =

그림 18.28 601 채널의 생성 과정

표 18.8과 표 18.9% 상향링크와 하향링크의 CINR ef         각 보여준다. 이 테이블
을 각 링크의 요구 0040 값으로서, 기지국과 단말은 CINK 값에 따라 변조방식과 부호율
을 결정한다. 이 HL PERS] 1% 미만을 만족하는 경우의 0148에 따른 변조방식과 부호
율을 나타내고, 0) 내의 숫자는 밴드 AMC 경우의 CINR 값이다.

표 18.8 상향링크 CINR 테이블

QPSK       1/12        -5.7        -5.6       -5.55        -5.6       -5.46
QPSK        1/6         -8.5        -8.5    |     -3.0        ~3.1        -8 28
QPSK        1/3         -0,4        04 | 40:15        -0.1        -0,35
QPSK        1/2          1,6          i (ee          2,2         2,03
16QAM        1/3          3,9          411 415         4,25        4,25
16QAM       1/2          6.5          G50 687         7.0         6,15
16QAM       2/3          9.7          90 |. 105        10.16        10.8

629



===== PAGE 626 =====
PART IV_MIMO-OFDM 통신 시

표 18.9 하향링크 CINR 테이블

-83.95          -8.8
QPSK     1/12      (-3, 35)     (-3.65)

00         -1,4
QPSK         1/6          (-1.65)         (-1.65)         S180)         -1,45        -1,45
QPSK       1/3        1,5(0,5)       2.1(0,6)        1.6         1,65        1,65
QPSK       1/2        4,3(2,5)      5,3(2,45)      4,25         4.3         4.4
QPSK       2/3       7 95(4 5)      9.4(4.6)        TY          8          8.15
16QAM       1/2       9.3(7,35)     10,15(7, 56)      9,25        9,35        9.5
16QAM      2/3      13, 1(10, 2)    14,6(10. 4)      13,2        13,5       13,65
16QAM       3/4       15, 8(11,5)     17,7(11,85)      16,7        16,5        15,7
64QAM       2/3      18,45(15,05)  19,7(15.6)      18,2        18,4        19.2
64QAM       5/6       24, 8(18.9)     27, 2(22)       24,4        24,7        27,5

OG ACK / NAK 채널
상향링크 ACK ABS 하향링크 패킷이 성공적으로 수신된 경우 “O(ACK)S, 수신이
경우 ‘V(NAK)S 전송한다. ns ACK ABS 부채널의 절반인 3개의 타일로
구성된다. ACK/NAKS 나타내는 1 비트는 표 18.10에 나타난 바와 같이 오류 보호를 위
알파벳으로 구성된 3개의 빅터(타일)로 부호화 된다.

표 18.10 ACK 채널의 부반송파 변조

0               0, 0, 0
4, 7,2

ACK 42-2 00) 채널과 유사하게 생성된다. ACK APS 1 HES SS 부호화를 7
쳐 3개의 코드워드로 맵핑된 후에 3개의 타일에 벡터 gto] 할당된다. 그림 18.29는 ACK
채널의 생성 과정을 보여준다.

630



===== PAGE 627 =====
제18장_ 와이브로 시스템

3 Tiles
_ < Z|          Code Word
Ea

ee

DL      wee     =
~     을 두 …  Block Coding

~   =

~   스는

~ 들 도
그림 18.29 ACK 채널의 생성 과정

ACK Channels

6 0: 와이브로 채널 코딩과 H-aRQ-

GM 컨볼루셔널 부호화

와이브로 시스템에서 송신하고자 하는 데이터 버스트는 그림 18.30에 주어진 채널 부호
화 과정을 거치게 된다. 채널 부호화는 FEC 블록 단위로 이루어지며, 각 FEC 블록은
채널의 정수배로 구성된다. 우선 채널 부호화 및 변조 블록에서 처리되는 기본 단위?
MAC PDUS] 길이가 허용된 입력비트 수가 아닐 경우에는 1`이 MAC PDUS] 뒤에 1
딩된다. 패딩된 패킷은 생성 다항식이 14+-.x 4x" 인 8#88와 XOR 과정을 통해 랜덤화
과정이 수행된다. 패덩과 랜덤화 ARPS 거친 패킷에 16비트의 CRC(Cyclic Redundancy
Check)7} 적용되고, 패킷의 길이가 4800의 배수인 패킷은 4800 비트 블록으로 분할되어
채널 부호화가 수행된다.

-ㅁㅠ

r

B=)

Subchannel

ㅁ                                                                                                            }           a
ata Burst                                                                                                                                                            aaa   Mapping

그림 18.30 채널 부호화 절차

와이브로 시스템에서는 채널 부호화 방식으로 컨볼루셔널 부호와 컨볼루셔널 Turbo 부
, LDPC FSS 사용할 수 있다. 컨볼루셔널 부호는 FCHS} MAPS] 사용되고, 데이터
스트에 대해서는 컨볼루셔널 Turbo 부호가 사용되며, LDPC 부호는 옵션으로 사용할
있다. 와이브로 시스템에서 사용되는 FAO] “7"이고 부호화율이 1/2인 컨볼루셔널
호의 생성 다항식은 식(18.8)과 같이 주어진다. 또한 puncturingy} 반복(76060000) 기법
사용하여 다양한 부호율을 지원한다. 이 때 FEC 블록은 tail-biting 방식에 의하여 컨

ilo 4t 4> 포 [에



===== PAGE 628 =====
PART IV_MIMO-OFDM 통신 시스템

볼루셔널 부호화기가 초기화되기 때문에 입력 데이터의 마지막 6 비트의 gow 레지스터
가 초기화된다. 이 컨볼루셔널 부호화기에 의하여 생성된 초기 12 Hee] 비트는 그 전에
입력된 FEC 블록에 의하여 부호화기에 남아있는 6 비트의 영향을 받게 되어 사용하지 않
고 버린다. Tail-biting 방식은 대역폭 효율면에서 약간 우수하나, 복호기의 초기 상태와
마지막 상태가 주어져 있지 않아 초기와 마지막 상태를 0으로 하는 기존 비터기 복호 방
식에 비해 복호 알고리즘이 복잡하다.

G,=1Tlocp Gy = 133 ger                                  (18.8)

0664 컨볼루셔널 Turbo 부호화

컨볼루셔널 Turbo 부호의 우수한 성능 때문에 데이터 HAE] 대해서는 컨볼루셔널
Turbo 부호가 사용된다[317]. 그림 18.31은 컨볼루셔널 70260 부호 부호화기의 블록도를
보여준다. HSDPAS} 1xEV—DOOA] 사용되는 61087 Turbo 부호화기와 달리, 와이브로
에서는 duo—binary Turbo 부호화기를 사용하기 때문에 두 개의 연속적인 비트가 부호화
기에 입력된다. 입력된 (A, 8)에 대해 부호율 1/3의 ASSAY Turbo 부호는 입력된 순
서에 따라 부호화하여 2 비트의 패리티 비트(7, M)7} 출력하고, 다시 (A, BS 인터리빙
한 후 컨볼루셔널 Turbo 부호에 의해 2 비트의 패리티 HEH, )'/2)를 출력한다.

output
A                 *                         A
B   GK          >                     B
| Ci              YW,
2 {   '       | Ce           Y.We
switch! =~~
~            ~. Systematic part
1
B     |    >            =F
                a
YP          |
>            | Parity part
aig
Ww

그림 18.31 컨볼루셔널 14[60 부호의 부호화기

_ 632



===== PAGE 629 =====
제18장_와이브로 시스템

ㅣ

AB

Subblock

|

1
ㅣ
‘Subblock      |
interleaver      |
| |

|         ㅇㅇㅇ         |
내              v
I        ㅇㅇㅇ        ea]
그림 18.32 컨볼루셔널 Turbo 부호의 서브블럭 인터리빙

그림 18.32에 나타난 바와 같이 4, BN, Ko, Wi, 의 6개의 부블록들은 독립적으로
각각 인터리빙되고, 패러티 비트를 포함한 부블록들은 El 부호율을 맞추기 위하여
puncturing 된다. Hybrid ARQS 사용할 경우에는 수신단에서 추가로 필요한 패러티 비트
의 LLR(Log Likelihood Ratio) 추정을 할 수 있기 때문에 패리티 비트의 puncturing 패턴
이 전송되는 패킷에 따라 변할 수 있다.

SUCK Hybrid ARQ

HARQ(Hybrid ARQ) 패킷의 MAC 버스트는 그림 18.334) 나타난 바와 같이 하나 또
는 그 이상의 MAC PUB 구성되며 080를 포함한 총 길이는 최대 3000 바이트까지 가
능하다. 와이브로에서는 하나의 HARQ 패킷으로부터 4개의 서브패킷이 만들어진다.

와이브로 시스템에서는 Type 1 HARQS} Type 11 HARQ 방식을 모두 지원한다. Chase
0010610108이라고도 불리는 Type 1 8400 방식에서는 모든 서브패킷에서 동일한

※-매체접근 제어 POU (가변 길이) ㅠ--매체접근제어 POU (가변 길이)

＊-                인코더 패킷(고정 길이)                  …

그림 18.33 HARQ 패킷의 구성

633


===== PAGE 630 =====
PART IV_MIMO-OFDM 통신 시스템

puncturing 패턴을 사용하기 때문에 이 HHO} 신호가 동일하다. 수신단에서는 현재와 이
전에 수신한 서브패킷을 모두 사용하여 복호화를 하기 때문에 사용하는 서브패킷의 수가
증가할수록 복호 시 에러 확률이 감소한다. 복호과정은 CRC 체크를 통과하여 에러없이
패킷이 복호되거나 최대 서브패킷 수에 도달한 경우에 종료된다. 그림 18.34는 8480
송ㆍ수신 과정의 예를 보여준다. 기본적으로는 900-800-'\%01 프로토콜로 동작하기 때
문에 단말에서 WAS 복호할 수 있다면 기지국으로 ACK 을 보내고, 기지국이 이를 수신
하면 이 패킷의 HARQ ASS 종료한다. 단말이 패킷을 복호할 수 없는 경우에는 기지국
으로 NAKS 보내고, 기지국은 재전송 WIS 수행한다.

Incremental Redundancy 라고도 불리는 1006 II HARQ 방식에서는 서브패킷마다 다
= puncturing WAS 사용하기 때문에 이 부분의 신호가 서브패킷마다 변한다.
Incremental Redundancy 방식은 패러티 비트의 LLRS 향상시키고 추가적이 서브패킷을
사용함에 따라 부호을이 낮아지게 되어 Chase Combining 방식에 비하여 낮은 BER 성능
을 갖는다. HARQ 에서 사용되는 240004008 팩턴은 SPID(SubPacket IDendity)= 표시
된다. 첫 번째 서브패킷의 SPIDE 항상 0으로 설정되어 있으며, 첫 번째 서브패킷에는 모
을

systematic 비트와 puncturing] 패러티 비트가 전송되어 수신단에서 SNR 환경이 좋
경우에 자체 복호가 가능하다. 일반적으로 전송하는 서브패킷의 SPIDE 증가하는 순
서(0.1.2.3)로 하지만, 첫 번째 5010(0;를 제외하고는 변경 가능하다.

Frame Length

5ms
——

08  | ieee oes

Ini Tx AC         Ini Tx AC         Ini Tx
ket 1            ket 2            ket 3

vst Be SN          iS                     |

Re Tx
NAK                    Packet 1            ACK

Ini Tx
Packet 1

MS2    |

NAK

그림 18.34 HARQ 송ㆍ수신 과정의 예

634



===== PAGE 631 =====
제18장_ 와이브로 시스템

와 AAS(Adaptive Antenna System)S 사용할 수 있다. 와이브로 MIMO 시스템의 하향링
크에서는 2~4개의 송신 안테나를 사용하여 다양한 모드로 전송할 수 있고, 상향링크에서
는 2개의 송신 안테나를 이용하여 다양한 모드로 전송할 수 있다. 본 절에서는 와이브로
MIMO 시스템에서 사용하는 다양한 MIMO 송신기법들을 하향링크와 상향링크로 구분하
여 설명한다. 또한 다중 안테나를 사용하여 빔 형성을 함으로써 커버리지 확장과 SDMA
(Spatial Division Multiple ㅅ00688)를 제공할 수 있는 AAS 기법에 대하여 설명한다.

. 0540 MIMO 하양링크

와이브로 MIMO 시스템은 하향링크에서 2~4개의 송신 안테나를 사용해 다양한 MIMO
Al 기법을 사용할 수 있다. 하향링크의 다양한 MIMO 전송기법을 요약하면 표 18.11과
다. 와이브로 MIMO 시스템의 하향링크에서 개루프 경우에는 전송 다이버시티 기법,
}이브리드 기법, 공간다중화 기법을 지원하고, 각 기법에 따른 전송 행렬은 표 18.12와
다. 행렬 AS 전송 다이버시티 기법을 적용한 송신 PAH rateE 1이다. 행렬 BE 전

다이버시티 기법과 공간 다중화 기법을 결합한 기법으로 하이브리드 기법이고 26는
2이다. 행렬 C= 각 안테나 별로 독립적인 ASS 송신하는 기법인 공간다중화 기법을 적
용한 송신 행렬 SHEA rate] 송신 안테나 개수와 동일하다. 폐루프 경우에는 안테나
그룹핑 기법, 안테나 선택 기법, precoding 기법을 이용하여 성능을 향상시킨다.

와이브로 MIMO 시스템에서 신호전송 시 PUSC 및 8080 모드에서 신호를 전송할 수
있다. PUSC 모드에서 2개의 안테나를 이용할 경우의 클러스터 구조는 그림 18.35와 같
다. 8080 모드에서 2개의 안테나를 이용할 경우에 클러스터 구조는 그림 18.36과 같다.
FUSC 모드에서 2개의 안테나를 이용할 경우에 각 안테나는 \328116 86[과 Constant Set
의 Haat 부반송파 중의 반만 사용한다. 즉, 짝수 심볼에서 A 번째 안테나는 Variable
Set 0과 Constant Set OS 사용하고, 두번째 안테나는 \3481016 Set 1과 Constant Set 1를
사용한다. 홀수 심볼에서 첫 번째 안테나는 \3081016 Set 1과 Constant Set 1를 사용하고,
두번째 안테나는 \304816016 Set 0과 Constant Set 0를 사용한다.

mS, ofp

에
»

of my
fol ol

ㅇ

|

Tr

635 _



===== PAGE 632 =====
PART IV_MIMO-OFDM 통신 시스템

표 18.11 와이브로 MIMO 시스템의 다양한

전송 기법

Open
loop

Tx BE

Closed
loop

Transmit
Diversity

Hybrid
Diversity
Spatial
Multiplex
SDM/SDMA

TD
HD
AS

AG

Precoding

표 18.12 와이브로 MIMO 시스

3         Matrix A     Matrix A         :       =
Matrix A      FDFR         AC       Spatial rate=1
Matrix B          :            :       i
FDFR      Matrix B    Spatial rate=2
Matrix C     Matrix C     Matrix C Spatial rate=Nr

Effective SISO or Matrix A,B,C

3 cases      3 cases
3 cases      6 cases
Rate 1      Rate 1,2    Rate 1,2,3
Reisie Rae 123 Ractgee. oe 00
precoding
템의 송신 안테나 개수에 따른 송신 행렬 ^,

2
8 4
4             A,

636

OF 02
lx,  -x; 0
~ ee
0 0 =x
0 0 tag

:        —(* +, TX t Xu  ;
as                            >
Vit r? Mia TMi IH; H Xin         c-|*|
- 145                                                   os)
2
ic         :
0 기        4            ~    ~*  ~    ~*
3       서 2 5 5          Bi
-x,| B,=| 0   1   Opera te 지이      C=/x,
er                5 구호 곡          x,
0   0    =
4
0              지 5 Xs 5                %,
0              지지                x.
의 2    1    6    8              epee)
*             B, 7          *          *                 CG ct
—x,              Rte 지지                 X;
|             oo a                 X,



===== PAGE 633 =====
제18장_ 와이브로 시스템

@QOdOWOOOO0 0 O O @ O 80004+8
@QOdOWTOOOO0 0 O O @ O smb 4k +2
OOOO B®OO0O BODO O O O smboi4k+1
OOOO BOO0 BOO O O O Ibo 4k

© Data Subcarrier
@ Pilot Subcarrier for antenna 0
@ Pilot Subcarrier for antenna 1

그림 18.35 2개의 SAI 안테나 시 STC PUSC 모드의 클러스터 구조

Frequency

@000000000000@00000000000000000000000000000000000095/0004(

@000000000000000000000000000000000000000000000005/0004<+1
0000000@0000000000000000000000000000000000000000005/70004<+2
0000000@0000000000000000000000000000000000000000005/07004<+3

@ Modulated Pilot for antenna 0
@ Modulated Pilot for antenna 1

Time
(symbol)

그림 18.36 2개의 송신 안테나 시 FUSC 모드의 클러스터 구조

4개의 안테나를 사용하여 2080 모드에서 ASS 전송하는 경우의 기본 클러스터
는 그림 18.37에 나타난 바와 같이 4개의 안테나를 이용하여 Ass
된다. 4개 송신 안테나를 사용한 0080 모드에서는 그림 18.38과 같은 클러스터 구
가진다. FUSC 모드에서 4개의 안테나를 이용할 경우에 각 안테나는 네 번째 staal
송파를 사용한다. 즉, 0번째 심볼에서 첫 번째 Cree Variable Set 0과 Constant Set 0
를 사용하고, 두 번째 안테나는 \3086016 Set 1과 Constant Set 1S 사용한다. 홀수 심볼에
서 Al 번째 안테나는 \3086016 Set 1과 Constant Set 1를 사용하고, 두 번째 안테나는
Variable Set 0과 Constant Set 0를 사용한다.

1124

+>

A

rir

aa

EN

Hu
dro Wore 그
r= 때0 of fN

@@ <. COO O OO ]D OC @asmux+s   © Data subcarrier
@ Pilot subcarrier for antenna 0
OB®QOOVWVWVOO OO O O @ @ symbai 4k +2
O 000 @ @ O O 0000 O O 90010919691   @ Pilot subcarrier for antenna 2
(<0000000000 @ (2 O (2 (2 80004    @ Pilot subcarrier for antenna 3
그림 18.37 47H 송신 안테나 시 STC PUSC 모드의 클러스터 PA

© Pilot subcarrier for antenna 1

637



===== PAGE 634 =====
PART IV_MIMO—OFDM 통신 시스템

Frequency

@6000000000000@0000000000000000000000000000000000005/0004<

@0000000000000000000000000000000000000000000000060/00004<+1
00000000000000000000000000000000000000000000000098/0004+2
0000000000000000000000000000000000000000000000005/0004<+3

@ Modulated Pilot for antenna 0
@ Modulated Pilot for antenna 1
@ Modulated Pilot for antenna 2
® Modulated Pilot for antenna 3

그림 18.38 4개의 송신 안테나 시 FUSC 모드의 클러스터 구조

GUE) Mimo 상양링크

와이브로 AAR] 상향링크에서는 2개의 안테나가 가용할 때 MIMO 기법이 사용 가
능하다. 행렬 AS 사용해 송신 다이버시티 기법을 이용하거나 행렬 BS 사용해 공간다중
화 기법을 이용하여 전송한다. 표 18.13은 상향 Ya] 송신 기법을 요약하여 보여준다.
다중 사용자 시스템에서는 601140078016 MIMO 기법을 사용할 수도 있다.

a-[* oi) a-|*              (18.9)
35 저     ^

표 18.13 와이브로 MIMO 시스템의 상향링크의 송신 기법

야

Matrix A          N/A                  Ns=1
ae           VE        Matrix B         N/A          Single user :
i                        Ns=2         =1
Toes Si       SU    Matrix B       N/A        s=2, um_layer
HE         Two MSs of    Two MSs of            ：
MU                                Collaborative MIMO

rate 2 each     rate 1 each

MIMO 상향링크의 PUSC 모드에서 alee] 배치는 그림 18.399} 같다.

638



===== PAGE 635 =====
제18장_ 와이브로 시스템

Antenna 0 (Pattern A)             Antenna 1 (Pattern B

(00600 @@@O

Antenna 0 (Pattern C)            Antenna 1 (Pattern D)

  Data subcarrier                                 O Data subcarrier

O    Null subcarrier                                                                  O   Null subcarrier

© Pilot subcarrier                     @ Pilot subcarrier
@ Pilot subcarrier

그림 18.39 UL PUSCOAM2| 클러스터 구조

GUHA 추가적인 성능 향상을 위한 MIMO 기법

추가적인 성능향상을 위해 안테나 그룹핑 기법, Ee 선택 기법, recoding 기법과 갈
은 다양한 기법들을 적용할 수 있다. 위의 기법들은 송신부에서 채널 정보가 가용할 때인
페루프 MIMO 기법들로서 각 기술 특징 및 장단점을 표 18.14에 정리하였다.

표 18.14 다양한 폐루프 MIMO 기법과 장단점

가조 아스  3 Tx 이상에서        High mobility 환경에서 성능이득이 low mobility
아아 matrix AEE 8에 성능 열화 없음         환경에서 As 대비 적음
적용될 수 있음
8 이상에서         단말의 계산량 적음 10868 mobilityoA] 성능
Antenna matrix Co          Low mobility 환경에서 열화 있음
Selection 적용될 수 있음        성능이득이 40대비 상대
적으로 큼
Quantized 8\ㅠ계열    채널이 full 고가 아닌 Feedback 양에 따라 성
Single/multiple        경우 VS 15°] F    동 의득 면화자 금, ee
Precoding stream                        에서 feedback 해야 할
Grassmanian BF                |          양이 많음, Codebook Al

택을 위한 계산량이 많음

639



===== PAGE 636 =====
PART IV_MIMO—OFDM 통신 시스템

3개의 안테나를 갖는 기지국에 대하여 송신 행렬 ^, 8, CL 단말로부터 CQICHE 이
용하여 피드백 되는 안테나 그룹핑 기법을 함께 사용할 수도 있다. 단말이 할당된 CQICH
를 이용하여 06000, 061111 혹은 0610110을 보고하면 기지국은 첫 번째 부반송파를 위
하여 안테나 0과 안테나 1을 묶고 두 번째 부반송파를 위하여 안테나 1과 안테나 2를 묶
는다. A 행렬에 대해 안테나 그룹핑 기법은 표 18.15와 같이 정리된다.

표 18.15 송신 안테나가 3개인 경우 행렬 AQ] 안테나 그룹핑

First      안테나 0, 안테나 1       안테나 0, 안테나 1       안테나 0, 안테나 2
Second 안테나 1, 안테나 2       안테나 0, 안테나 2       안테나 1, 안테나 2

~     ~                       ~     ~   ~     ~*            ~     ~
자 600 1 0            ea) ep 세 으시           eee Oren)
ss            ~     wt    ~     ~*           ~     ~*                                   ~     nt
Matrix: pA, =| XX ee ky Gli, 0. 10    4=|0 0 % -x,
~     ~                       ~     ~*            ~     ~    ~     ~
Ore 0 3 02             02 00 x. 호            ~ 지그

송신 안테나가 3개인 경우

ob»

신 행렬 Bol 대해서는 표 18.167} 같이 ASS 맵핑하여

표 18.16 송신 안테나가 3개인 경우 행렬 6의 송신 행렬

렬 Col 대하여 k 개의 부스트림이 구성될 경우 AS PAS CQICHS] 따라 적
변경된다. 표 18.17은 0010 값에 따른 <, 을 정리하여 보여준다. 사용되는 안
테나의 전력은 총 송신전력이 일정하므로 스트림의 개수에 따라 다르게 부스팅된다.

640



===== PAGE 637 =====
제18장_ 와이브로 시스템

표 18.17 송신 안테나가 3개인 경우 행렬 의 안테나 그룹핑

             0 |           | 0 |
1      C, =c} 0       C, =c} x,       C,=c} 0        Ca
| 0 |           | 0 |           | x5 |
lx, |           Ex           | 0 |          ;
2       C, =c| x        C,=c| 0        G—elx,           =
1   2       2           3   1       Cais
| 0 |           ES           x |

4개의 송신 안테나를 가진 기지국에서 전송 행렬 AL 단말로부터 피드백되는 정보에
따라 안테나 그룹핑을 수행할 수 있다. 표 18.18과 같이 단말이 피드백하는 00108 값에
따라 안테나가 2개씩 그룹핑된다. 4개의 송신 안테나를 가진 기지국에서 146 2를 달성하
는 위한 행렬 BE 단말이 기지국으로 피드백하는 안테나 그룹핑 정보와 함께 응용될 수도
있다. 단말이 피드백하는 0010에 따라 표 18.19와 같이 안테나가 2개씩 그룹핑되고, 이
에 따른 송신 행렬은 #, ~ #, 와 같다.

표 18.18 송신 안테나가 4개인 경우 행렬 의 안테나 그룹핑

First         안테나 0,1              안테나 0,3               안테나 0,3
Second        안테나 1,2              ore] 1,3               ore 1,2
x 주 D0         Geo 6 0 0          ee 00820
eee 0)          00406 =         020 으로 7.
~     1            ES     ;   3   4     =         3   |.
Matrix 4,    ~   A,   ra ey ee    A,    000 호

02000 호조   08034 4   a OD

641



===== PAGE 638 =====
PART IV_MIMO-—OFDM 통신 시스템

표 18.19 송신 안테나가 4개인 경우 행렬 6의 안테나 그룹핑
First        안테나 0,1            안테나 0,1            grey} 0,2
Second        안테타 23               안테나 28               안테나 18
Hh, ty oe         자 =e oe ey         =e, 제 ~
Matrix B= x,  i :  x,  개   B= xy  3  x,  %   B,= x3  ™  X6  ="
a a a         Te Se ae          시” ~
시이 Mee 8          tk, & mG         시 Chore dees
CQICH          0b101110                 0b101111                 0b101111
First         안테나 0,2               안테나 0,3               안테나 0,3
Second        안테나 1,3               안테나 12               안테나 1,2
지 eo ~         기 ae a         % Ae Roa
Matrix B,= X4  건  8  %   B,= x;  ™  X¢  =   B.= X4  개  xg  Xe
Ca Sie eee          aah oe mn          제 4 제 oe,
X, -X, 제 —X%         Go 시이          제기 ie aaa

H 18.202 CQICH 값에 따라 4개의 송신 안테나를 가진 기지국에서 사용하는 행렬 <;
을 정리하여 보여준다. 총 송신전력이 동일하므로 사용되는 안테나 ABS 부스팅 된다.

표 18.20 송신 안테나가 4개인 경우 행렬 의 안테나 그룹핑

aoe
그 띄케 “GETOOHT GEER HORAN “axiCIDO: on iot”
| 0 |             | 0 |

=              6
0       x       0       0
see he 8 :  이 = '  C,=e :  6. -ㅇ ,                  0=1
| 0      | 0 |     | 0      Lx |
lx, |     Ex     Pe |.    eee      0       0
Be       0       0       x               0      1
C=cl 7] G=     Cl=¢    C,=c|'| C.=c| '| C.=e        =
2  1ae 0  2 ae  3  0  4 Ale  5  0  6  x  on V2
| 0 |     | 0 |     | X> |     | 0 |      XS       x
rx, 1     rx. |     x, ]     C07
x       x       0       x                      1
C =c\"*|} G=cl 7] CG=c    2, =히 '                       --
8   10 ‘   2    0   3   ee   %                   c= 3
| 0 |     | Xs      | X3      | x3

_ 642



===== PAGE 639 =====
제18장_ 와이브로 시스템

와이브로 MIMO 시스템에서는 시공간 부호 출력에 대해 아래 식과 같이 precoding 기

법을 적용할 수 있다.

2- Wx                              (18.10)

, 44 는 스트림의 개수이다. 행렬 \ 는 크기가 Nrx 44; 인 행렬로 는 송신 안테나
를 나타낸다. A] (18.10)의 2 는 크기가 47×1 이고, Nr AS] 송신 안테나에서 전송되는
SS 나타낸다. 이와 같은 다양한 MIMO 기법들은 그림 18.40과 같은 과정을 거치며
드7

-2~4개의 송신 안테나에      _ Capabiltvol HE 2      - 다중 사용자 다이버시티
대한 A, 8, 0 행렬 선택       raat leew ig        이득 Sti} |].
- 피드백 Capability :          - 기존 : 사용자 AR (SNR)     -RF 상태를 고려하여

바빠 아이 6009: le! -안테나간 상관관계, 이동속도 fe] Bandwidth 할당 결정

=     ㅣ

- 필요한 피드백 정도 : cal,
AG/AS 인덱스, 프리코딩
인덱스, 채널 Sounding

그림 18.40 와이브로 MIMO 시스템 동작 절차

ative AAS(Adaptive Antenna System)

AAS(Adaptive Antenna System) 모드에서는 그림 18.41에서 HE 바와 Zo] AAS
DL/UL IE(Information Element)S 통한 영역 구분에 의해 non—AAS 단말과 AAS 단말
을 모두 지원 가능하다. 또한 AAS SDMA(Spatial Division Multiple Access) DL/UL IE
를 통해 자원 할당 및 H-ARQ 기능을 지원하고, 4) W(Orthogonal) DL/UL SDMA 프리
US 도입을 통해 공간채널 추정 성능을 개선한다. 커버리지 SS 위해 AAS DLFP
(Downlink Frame Prefix)S 이용하고, 빔 형성 °|S(beamforming gain)& 갖고 H-ARQ

정보를 지원하는 개인 WS 할당한다. 사운딩 심볼 YUL AAS 프리앰블을 통해 공간채

643 —



===== PAGE 640 =====
PART IV_MIMO—-OFDM 통신 시스템

00806 0066                AMC(2 x 3) / TUSC               (0)-ㅁ0056         AMC(2 x 3) / (0)-6086
~……       <                                      > >       <                            >
TTG
AAS-DLFP ㅣ  | AAS-DLFP ry
—                                                   UL burst #1
DL traffic burst #1                                       Ul burst #.
a                                                                                                 Tea
에                                       oS                    =
2        4       Broad     는         OL traffic burst#2                   6       는        essa             의
본        므         cast | 은                                                 rs       은                                 3
3                  Burst) &                                ae pe         UL burst #3          3
a                          =       OL traffic burst#8~#5             Oo      =                              a”
a                                                         B                       [ |
(ale
$                             DL traffic burst#6
*                                  1 ~ 도호                                        UL burst#4~#6
=
| (aas-oirp! =faas-pirp; 1
ae  oo eel
Non-AAS                       AAS Zone                     Non-AAS              AAS Zone

그림 18.41 와이브로에서의 AAS 모드

AAS 모드에서 AAS DL 영역은 AASH 규정된 BA(AAS 2006)의 경계에서 시작하
며, 다음 영역 혹은 하향링크 마지막까지의 모든 부채널로 구성된다. 206(:와 FUSC 영역
에서 DL 프레임의 최상위 번호의 2개의 부채널은 기지국에서 AAS 다이버시티-맵 영역
으로 지정할 수 있다. AMC 영역에서는 주어진 AMC 부채널에서 모든 sala 부반송파
및 데이터 부반송파에 대하여 동일한 안테나 BS 사용한다. AMC 영역에서 AAS DL 영
역의 첫 번째 및 최종 부채널은 기지국이 AAS 다이버시티-맵 영역으로 지정할 수 있다.
또한 AAS-DLFP2] 용도는 단말의 페이징과 대역 할당뿐만 아니라 초기 레인징이 가능하
도록 하기 위하여 기지국의 파라미터를 확실하게 전송하는 데 있다. 이를 위하여 QPSK
WAS 2회 반복하는 1/2 부호를 사용하며, AAS-DLFPS] 시작점은 AAS 하향링크 프리
앰블로부터 알 수 있다. 트래픽 버스트에 따라 서로 다른 빔들이 AAS 다이버시티-맵 영
역에 사용될 수 있으나, 각각의 AAS 하향링크 프리앰블과 이와 관련된 AAS—DLFP=
동일 빔에 전송되어야 한다.

와이브로와 같은 TOD 시스템에서는 사운덩 채널을 사용하여 기지국이 하향링크 채널
ABS 획득할 수 있다. 와이브로 시스템에서 사용되는 사운딩 채널은 2가지 유형이 있다.
타입 AWA 하나의 사운딩 WEE 그림 18.42에 나타난 바와 같이 인접한 두 개의 빈으로
구성된다. 타입 8에서는 특정 하향링크 2600418400(예: PUSC)S 사용하여 구성한다.

644


===== PAGE 641 =====
그림 18.42 타입 AS] 사운딩 채널

 MIMO} AAS] 비교

와이브로 시스템에서는 MIMOS} AASS] 다중 안테나 기술이 선택 사항으로 반영되었
다. 표 18.21에 나타난 바와 같이 AAS} MIMOL: 서로 다른 특성을 가지며 응용 목표도

}간 차이가 있다.

FE 18.21 AASS} MIMO2| 특성 비교

AL
ayes

ae ae
필수적

(궤환형)
AS 빔형성(펼요)
기정의된 빔형성(불필요)
Line of sight (LOS) _
매크로 셀

커버리지 증대

증대

안테나당 할당

필수적 또는 선택적

(궤환형 또는 개방형)
적응 precoding(4 &)
코드북 ㅁㅠ60001278(불필요)
Rich—Scattering

피코 셀/옥내

링크의 신뢰성(010)
가입자 전송률(814)



===== PAGE 642 =====
PART IV_MIMO-OFDM 통신 시스템

chs) 와이브로 MAC 계층

GON 와이브로 MACY 기본 개요

그림 18.43에 나타난 바와 같이 와이브로 시스템은 크게 4가지 상태로 구분할 수 있다.
Initialization state: 단말의 AAS AS 초기 동기를 완료하고 인접 Ao] 대한 정보를
수집하여 데이터를 전송 받을 Bd AS 결정하는 단계이다. 하향링크 프리앰블 이후의
두 심볼을 디코딩하여 FCH2} MAP ARS 얻을 수 Yu} Broadcast 채널인 DCD}
UCDE 디코딩하여 Epa 셀에 대한 기본적인 채널 QRS 얻는다. Access states fH
AZ 정한 후 레인징을 통하여 단말을 기지국에 등록시키는 ABS 나타낸다. Connected
state: 크게 슬립 모드, 액티브 모드, 핸드오버를 위한 스캐닝 BES 구분된다. 액티브
모드에서는 데이타 버스트를 송ㆍ수신하며, GAS] 전력 AWS 줄이기 위하여 슬립 모드
로의 전환 또는 핸드오버를 위하여 스캐닝 모드로의 전환이 가능하다. 106 states 단말의
전력 AVS 줄인다는 관점에서는 슬립 모드와 유사하나 HE connection 및 management
connection ID, IP address$ 해제 또는 반납한다는 관점에서 슬립 모드와는 차이가 있다.

Normal Re-Entry
Fast Re-Entry

Hi)

Initialization State                               Access State                                   Connected State

asaenese,

¥
 106 State

Handover
Execution

oa >   110 case of failure

~
을 ‘Normal case

그림 18.43 와이브로의 GOH 상태도

646



===== PAGE 643 =====
제18장_ 와이브로 시스템

08664 MAC 프로토콜 계층 구조

MAC 프로토콜은 그림 18.44에 나타난 바와 같이 3개의 부계층으로 구성된다.
Service—Specific CS(Convergence Sublayer)= CS SAP(Service Access Point)S 통해
수신된 외부 데이터를 MAC SAPS 통해 MAC CPS(Common Part Sublayer)=. 전달하여
MAC 5120로 맵평한다. 여기에는 외부 통신망에서 수신되는 SDU(Service Data Unit)S
구분하여 해당 MAC SFID(Service Flow 10600116)와 CID(Connection Identifier)S 관련
시키는 기능이 포함되며, 페이로드(0841080)의 헤더 e}4(Payload Header Suppression:
PHS) 기능을 포함될 수 있다.

Scope of standard

t           CS SAP           )

Data/Controls Plane                            Management Plane

i                                                        i
I                                                        1
|                                                        1
I                                                        1
1                                                        i
1                                                        I
1                                                        i
|]                      Sevice~Specific          <      +>         Management Entity        +
|                  Convergence Sublayer             }
|                      (08)                  1           Service-Specific
1                                                       if            Convergence Sublayers
| ㅇㅇ                    MAC SAP                    H
i =                                                  I
:              MAC Common Part Sublayer         '
ㅣ                        (MAC CPS)                  it                                 ;
|                                                 <      {    >         Management Entity
|                                                     :        MAC Common Part Sublayer <4
1                    Security Sublayer               11
|                                                       re          Security Sublayer          i
|                  {       PHY SAP       y             :
]                                                        I
|                                                       님
>               Physical Layer
|    =                     (PHY)               그집              Management Entity
i                                                       1                       PHY
1                                          111
1                                                        1
1                                                        1
1                                                        1
1                                                        1
1                                                        1
]                                          J!
!                                                        1

그림 18.44 MAC 프로토콜의 계층 구조

MAC CPS= MAC2] 핵심 기능인 시스템 액세스, 대역폭 es, connection 설정 및 연
결의 유지관리 기능을 제공하며, 특정 MAC 000060000으로 분류된 데이터를 다양한 C
로부터 MAC SAPS 통해 수신한다. 또한, MAC 계층에는 인증(040160008000), 안전 키
교환 (secure key exchange) 및 9+ 3kencryption) 기능을 제공하는 별도의 보안 부계층
(security sublayer)7} 포함되어 있다. PHY SAPS 통해서 MAC CPS2} PHY 사이의 정
보, PHY 제어 및 데이터가 전송된다.

N



===== PAGE 644 =====
PART IV_MIMO-—OFDM 통신 시스템

“AGRE MAC PDU 7%

MAC PDUS] 구조는 그림 18.45에 주어져 있으며, 크게 MAC 32](Management)
PDUS 사용자 데이터 MAC ?100로 구분된다. 각각의 PDUE 일정한 길이를 갖는
generic MAC header= 시작되며, MAC 관리 PDUS] 페이로드는 MAC 계층의 SAS
위해 미리 규정된 MAC 관리 메시지이다. 그림 18.462 MAC PDUS 구성하는 방법을
보여준다. 이 그림에 나타난 바와 같이 패킷 PDUE MAC 8100의 페이로드에 맵핑되고,
이 페이로드에 MAC 헤더와 CRC7} 추가되어 MAC PDU7} 구성된다. 또한 패킷 PDUS|
길이가 길 경우에는 MAC SDUS 더 작은 단위로 분할(0\8800600000)하여 다수 개의
MAC ?10로 구성하며, PDUS| 길이가 짧은 경우는 다수 개의 MAC SDUS 결합
(280008)하여 1개의 MAC PDU® 구성한다.

LSB

Payload (optional)    CRC (optional) |

그림 18.45 MAC PDUQ| 구조

MAC SDU                          MAC SDU
Fragn#entation …..
MAC Header ， 1440 8040 ㅣ CRC       MAC SDU     MAC SDU
<              MAC PDU               즈
MAG PDU nett naan                                3
를           Fragmentation (=e |            Fragmentation 4c    ae]
MAC Header | ‘gub-header” | MAC SDU f1 |    MAC Header ‘Sub header MAC SDU f2
<=              MAC PDU                  ~ 제              MAC 004 —
MAC Header    Packing     wac sou |. Packing . | Mac 904
|               846 - header           Sub- header ㅣ
제                         MAC 0004 —             -               >

그림 18.46 MAC PDU2| 구성 예

가

그림 18.47은 물리계층으로 전달되는 데이터 버스트의 실질적인 모습을 보여준다. J
MAC PDU* 고유의 CID(Connection ID)#. 구분되며, 하나의 데이터 버스트는 하나 또

648



===== PAGE 645 =====
제18장_와이브로 시스템

CID = 0x2555

그림 18.47 연접 과정을 통한 데이터 버스트 생성의 예

7 CID = 0x0399                        CID = Ox0EF 1        CID = OxSF3E

~CID=0x2301

= 다수 개의 MAC PDUS 연접(60ㅁ086648000)하여 구성한다. 물리 계층에서는 버스트
단위로 부호화와 HADIUC, UIUC 참조)를 수행한다. 그림 18.47에 나타난 바와 같이
한 버스트에 사용자 데이터0(08@ PUY 아니라 MAC 관리 메시지, 대역 요청 MAC
PDU 등도 함께 연접 가능하기 때문에, 데이터와 관리 메시지를 필요에 따라 연접하여 하
나의 버스트를 구성한다.

MAC 헤더는 0600040 MAC 헤더와 MAC Signaling 헤더의 두 종류로 구분된다.
Generic MAC 헤더의 구조는 그림 18.48과 같으며, 페이로드로서 140 관리 메시지나
사용자 데이터 MAC PDU7} 따라 온다. MAC Signaling 헤더는 페이로드가 존재하지 않
으며, 그에 대한 구분은 HT(Header 1500)에 의하여 이루어진다. 즉, HT = 00] Generic
MAC 헤더에 해당하며, HT = 1이면 상향 링크의 경우 MAC signaling 헤더에 해당한다.
Generic MAC 헤더의 경우에 MAC 『00는 헤더에 있는 010에 의해 구분된다. MAC
Signaling 헤더는 EC(Encryption Control) 값에 따라 Type-1 MAC Signaling 헤더와
Type—2 MAC Signaling 헤더로 분류된다. 1706-1 MAC signaling 헤더는 단말에서 CID
별로 상향링크에 대한 대역폭을 2-15 bandwidth request 헤더, CQICH allocation 4]
더 등이 있으며, 1506-2 MAC Signaling 헤더는 피드백 PDUS 구성하기 위한 피드백

헤더이다.
Ba                  jot                    ㅣ            다
아구스                                    EKS          LEN
|         은                    (2)         MSB (3)
는 |      ㅣ        i                        i            i    i
|                                                |
LEN LSB (8)                    CID MSB (8)
 408:                        |            | | ㅣ
T                            |            ㅣ    i    |
CID LSB (8)                     HCS (8)
pao                       i            |

그림 18.48 Generic MAC 헤더의 구조

649


===== PAGE 646 =====
PART IV_MIMO-OFDM 통신 시스템

 MAC 관리 메시지

MAC 관리 메시지는 그림 18.49에 나타난 바와 같이 메시지 타입과 타입에 따른 메시
지 페이로드로 구성된다. MAC 관리 메시지의 종류와 SEE 표 18.22에 주어져 있다. 이
들 메시지들 중에서 와이브로의 프레임의 구조, 대역 할당, 물리 계층 파라미터와 관련된
관리 메시지는 DCD, UCD, UL—MAP, DL—MAP 등이 있다.

Management Message Payload

그림 18.49 MAC 관리 메시지의 구조

표 18.22 MAC 관리 메시지의 종류 및 용도

UCD        Uplink Channel Descriptor    34     ARQ-Discard       ARQ Discard message
1        DCD       Downlink Channel Descriptor 35      ARQ —Reset         ARQ Reset message

Channel measurement

2       DL-—MAP      Downlink Access Definition    36       REP-—REQ
Report Request
:           가                             Channel measurement
3       UL-MAP       Uplink Access Definition     37       REP-RSP
Report Response
4      RNG—-REQ         Ranging Request        38         FPC           Fast Power Control
5      RNG-—RSP          Ranging Response         39      MSH-NCFG     Mesh Network Configuration
6      REG—REQ        Registration Request       40      MSH-NENT        Mesh Network Entry
7      REG—RSP        Registration Response      41      MSH-DSCH     Mesh Distributed Schedule
8                           Reserved            42      MSH-CSCF     Mesh Centralized Schedule
9      PKM-REQ      Privacy Key Management     43      MSH-CSCF      Mesh 66000011000 Schedule
Request                                           Configuration
Pri     Key M         t
10 PKM-RSP       mivacy Sey Manageme®™ 11 00 AAS-FBCK-REQ _AAS Feedback Request
Response
Dynamic Service Addition
11      DSA-REQ                                 45 AAS-FBCK-RSP    AAS Feedback Response
Request
D:     ic Service Additi
12      DSA-RSP       ynamie wervice seamen 46 ~AAS Beam Select AAS Beam Select message
Response
ic Service Additi
13     DSA-ACK      10뽀90 008     리아     47    AAS BEAM REQ AAS Beam Request message
Acknowledge
Dynamic Service Change                              AAS Beam Response
14      DSC-REQ                                  48    AAS BEAM RSP
Request                                             message
Dynamic Service Change                                     .     P
15      DSC-RSP                                  49      DREG-—REQ     SS De-registration message
Response
Dynamic Service Change
16      DSD-ACK                                  50     MOB SLP_REQ      sleep request message
Acknowledge
Dynamic Service Deletion
17      DSD-REQ              Request             51     MOB _SLP_RSP      sleep response message

650



===== PAGE 647 =====
제18장_ 와이브로 시스템

Dynamic Service Deletion

18      DSD-RSP                                 52    MOB _TRF-IND    traffic indication message
Response
neighbor advertisement
19                            Reserved             53    MOB NBR-ADV
message
scanning interval allocation
20                            Reserved             54    MOB_SCN-REQ
request
Multicast Assignment                             scanning interval allocation
21      MCA-REQ                                  55    MOB_SCN-RSP
Request                                             response
Multicast Assignment
22      MCA-RSP                                 56 MOB BSHO-REQ    BS HO request message
Response
Downlink Burst Profile
23     DBPC-—REQ                                 57 MOB MSHO-REQ    MS HO request message

Change Req,
Downlink Burst Profile
24     DBPC-—RSP                                 58 MOB BSHO-RSP    BS HO response message
Change Response
25      RES-—CMD          Reset Command         59     MOB_HO-IND      HO indication message

:       ay                                     Scanning result report
26     SBC-REQ     SS Basic Capability Request    60    MOB _SCN-REP

message
SS Basic Capability                                 BS broadcast paging
27      SBC-—RSP                                  61    MOB_PAG—ADV
Response                      ae                     message
SS network clock
28      CLK-CMP                    .               62       MBS_MAP          MBS MAP message
comparison
De/Re-register Command                           Power control mode change
29     DREG-CMD                                 63       PMC_REQ
message                                       request message
「                                        Power control mode change
30      DSX-RVD       DSx Received Message      64       PMC_RSP

response message

ieee                                        Setup/Tear—down of long
31     TETP—CPLT    Config File TFTP Complete    65    PRC-LT-CTRL                       :
term MIMO precoding

enleg                                            Association result report
832     TFTP-—RSP     Config File TFTP Complete    66    MOB _ASC-REP
message

Standalone ARQ Feedback    67-2
33  ARQ-Feedback                                                                reserved
message             55

MERRY 초기 망 진입 절차

단말의 초기 망 진입 절차에 대한 전체적인 흐름도는 그림 18.50에 주어져 있다. 초기

망 진입을 위한 절차는 크게 동기화, 초기 레인징, 기본 제공능력 협상, conection 설정으

로 나눌 수 있다. 단말의 세부적인 진입 절차는 다음의 단계로 구성된다.

(1) 하향링크 채널을 스캐닝하고 기지국과 초기 동기를 맞춘다. 초기 동기 취득 후에 얻어
지는 프리앰블 PN 인덱스로부터 10681과 세그먼트 BS 파악하고, 그를 통하여 물리

651



===== PAGE 648 =====
스텐
—o

PART IV_MIMO-OFDM 통신

=

그림 18.50 단말의 초기화 절차

(2) MAC 메시지를 디코딩하여 Aol] 대한 전체적인 채널 정보를 파악하고0010, UCD),
레인징 신호의 전송에 필요한 파라미터들을 취득한다.

(3) 지시된 초기 레인징 구간에서 초기 레인징을 수행한다. 단말에서는 RNG-REQ 메시
지를 기지국에서는 RNG-RSP 메시지를 사용하여 초기 레인징을 수행한다.

(4) 기본 제공능력을 협상하고, GAS 인중한 후에 키를 교환한다.

(5) PHS 기지국에 등록하고, 접속을 설정한다.

(6) 시간(0006 of day)S 설정한다.

(7) 운영 파라미터들을 전송한다.

(8) Connection 설정한다.

_ 652



===== PAGE 649 =====
제18장_ 와이브로 시스템

레인징은 단말이 전송한 신호가 OFDMA 기지국의 수신 구간에 해당 슬롯에서 일치하

록               을 동기화하고 전력 제어를 하는 절차이다. 레인징 부호는

초기 레인징, 핸드오버 레인징, 주기적(66040010) 레인징, 대역폭 요구(6340\1041 request)

부집합으로 분류된다. 단말이 이 중 한가지 alae 수행하고자 할

때에 해당 레인징 부호 부집합 중에서 랜덤하게 부호를 선택하여 상향링크 제어 채널의
부채널에 변조시켜 전송한다.

(1) 초기화/핸드오버 레인징 절차

초기 레인징 및 핸드오버 레인징은 새로운 Yo] 진입을 위한 절차이다. 초기 레인징을
위해서는 사전에 단말이 하향링크에 동기화되어 있어야 하며, UCD 관리 메시지와 MAC
관리 메시지를 통하여 상향링크 초기 레인징 HAS 획득하여야 한다. 전체적인 초기 레
인징 과정은 크게 세 단계로 나눌 수 있으며, 그림 18.51에 상세 절차가 주어져 있다.

첫 단계는 RNG-REQ 단계이다. PAS 상향렁크의 A 번째와 두 번째 심볼에 위치한
초기 레인징 구간에서 초기 레인징 CDMA 부호를 사용하여 RNG-REQ 메시지를 전송
한다. 기지국은 수신된 신호를 처리하여 각 단말의 상향링크 타이밍 옵셋을 구하고
RNG-RSP 메시지를 통해 단말에 전송하면, 단말은 그 후 신호 전송 시 그 만큼의 옵셋
= timing advances}o] 전송하게 된다. CDMA AES 전송한 후, 단말이 SHS 수신하

지 않으면 단말은 AAs backoff delay 후에 전력 레벨을 수정하여 새로운 CDMA 부호

2      Aus
를 전송한다
| 66 | -6 | 08 ae a ee ee ES a cs
i                      ry          i                        ry
UL-MAP.                             RNG-RSP _RNG-RSP                           RNG-RSP
DCD/UCD/                      Binary-         (Continue) (Success)      UL-MAP     eee (Management ClDs)
DL-MAP                 eo — … see eee coe
Backoff                                      RNG-REQ
RNG-REQ                         RNG-REQ
(Code)                  RNG-REQ      (Code)                    (MAC_Address)

(Code)

1) OL Syne     3) UL-MAP 5080 6) Backoff              8) Timing,

11)RNG-RSP 12) RNG-REQ              13) RNG-RSP

2)UL Burst 4) Random        7) Ranging Code Power, &         (Succes9 수신 message 4S              (Management
정보획득        Subch, Symbol,                              Frequency        mapped with with MAC                   CIDs) 수신
Code & &#                                   Adjustment       transmitted      Address
5) Ranging Code                           9) Random       Subch,
전송                                           Subch Symbol, Symbol, &
Code 4&        Code
“                            10) Ranging
Timer T3                             ox
Expire                      Code aS

그림 18.51 초기 레인징 절차

653 _



===== PAGE 650 =====
PART IV_MIMO—-OFDM 통신 시스템

단계로서, 기지국에서 RNG-RSPO] success 메시지를 전
코드 정보와 함께 CDMA Allocation 가 포함된

수신하면 단말은 RNG-RSP 수신이 성공적인 것으로 간주한다. 이 때 단말

상에서 unicast RNG-REQS 전송한다.

레인징 완료 단계로서, 기지국이 RNG-REQ 메시지를 성공적으로 수

초기 레인징 CIDE ~ basic 및 primary management CIDS°]
전송한다. 단말이 RNG-RSPS 정상적으로 수신하

eee 정상적으로 상향링크 HAES 전송할 수 있다.

신하면 기지국은
할당된 RNG-RSP 메시지를 단
면

기 레인징 절차는 종료되고

된
조7

(2) 주기적 레인징 절차

주기적 레인징은 초기 레인징이 완료된 후에 주기적으로 기지국과 단말 사이의 타이밍,
전력, 반송파 주파수 SS 갱신하기 위하여 수행되며, 그림 18.52에 상세 절차가 주어져
있다.

eS | "66 이     69 Ese     Shee] 00006 55 2026     BS           BS
|        ry                          ry                          Ly
UL-MAP                                             RNG-RSP               , RNG-ASP
Binary-              eee (Continue)            ~ (Success)
ANG-REQ          Backoff pNG- REQ                     RNG-REQ
(Code)                     (Code )                    (Code)

1) UL- MAP Scan
-Periodic Ranging
Domain Search

2) Random Subch
Symbol, Code & &
3) Ranging Code
as

Expired

Timer 13
Expired

단말은 주기적 레인징을 수행하려고 하는 시점에서 부채널과 부호를 랜덤하게
여 CDMA 부호를 기지국에 송신한다. 그 후에 단말이 RNG-RSPS
backoff delay 후에 다음의 주기적 레인징 구간에서 단말의 전력 As

4) Backoff
5) Random Subch
Symbol, Code 4 &

as

6) Ranging Code 7) RNG-RSP

(Continue) +4!

8) Timing, Power, &

Frequency
Adjustment

9) Random Subch
Symbol, Code  &
10) Ranging Code

전송

그림 18.52 주기적 레인징 절차

11) RNG-RSP
(Success) +4!

12) Timing, Power,
& Frequency
Adjustment

선택하
못하면

수신하지
조정하여 새로운

하여

CDMA 부호를 전송한다. 주기적 CDMA 레인징 부호를 성공적으로 수신한 즉시 기지국

은 레인징 정보(부호, 슬롯, 부

8송하여 해당 단말이 확인할 수

메시지를 단말에 전

654

있도록

부채널 등)와 수신된 주기적 레인징 부호를 포함한 RNG-RSP
한다.



===== PAGE 651 =====
제18장_ 와이브로 시스템

(8) 요구 레인징 절차
단말에서 전송해야 할 데이터가 있는 경우에 대역폭 요구를 위하여 CDMA 기반의 레
전송한다. 단말은 대역폭 요구 부호 부집합으로부터 0 부호를 랜덤하게
선택하고, 레인징 부호를 BPSK 변조하여 상향링크 세 번째 심볼에 전송한다. 세부적인
18.53에 주어져 있다.

065 |. . 65: |]. 85 | 65 |] es 10600 ee ee | 86
ry                                                i                                        ry                         ㅣ
UL-MAP/                                     3                                         UL-MAP                          UL-MAP
Binary-                                                                                 a
UCD                                 exporientiai      |                       (COMA.                     (BW Allocation)
Random         | eeccccce  Allocation_lE) | eessesecseee
wocccccce

Backoff

RNG-REQ               …ㅠㅠㅠㅠ ㅠㅠ…                                BW-REQ Header

(Code)

BW-REQ
(Code)

and/or User Data

1) UL-MAP Scan                   4) Backoff                           7) UL-MAP 수신                   9) UL-MAP 수신

2) Random                       --Contention-based               -CDMA_AllocationlE            -MAP_IE = Grants to
Subch, Symbol,                     Reservation Timeout                 with transmitted Subch,            the requested BW
Code a                             --According to the BW               Symbol, & Code

3) Ranging Code                   Req Backoff Start&                                8) BW-REQ Header

전송 (BW Req)                      End param. in UCD

and/or 0818 전송

5) Random Subch,
Symbol, Code 4 &
6) BWREQ Code 전송

그림 18.53 대역폭 요구 레인징 절차

제티 |
Timer 116
Expire

와이브로에서는 단말의 전력 AWS 최소화하기 위한 AA(power 58108) 모드로서 |S
립 모드(86620 mode)2} 1016 모드가 있다. 슬립 모드 동안은 POUS 송신하거나 수신하지
않기 때문에 단말의 전력 소모를 최소화하며 서빙 기지국의 자원 사용을 줄일 수 있

슬립 모드는 크게 수면 구간(61660 104660081)과 청취 구간(116660108 interval) ° = ye
어 있다. 수면 구간은 단말이 SY 모드로 들어가는 순간부터 Awake 모드로 돌아올 때까
지의 지속 시간을 의미한다. 슬립 모드의 지속 시간은 최소 및 최대의 시간 제한 하에서
지수적으로 증가한다. 단말은 슬립 모드로 전환하기 위해 기지국에 MOB SLP-REQS
사용하여 통지하며, 기지국은 MOB_SLP-RSPS 통해 슬립 모드로의 전환을 승인한다.
위 메시지 전송시에 단말이 슬립 BES 전환되는 시작 시점, 수면 구간의 최소값과 최대
값(프레임 단위), 깨어나서 기지국으로부터 신호를 수신하는 청취 구간의 값들이 함께 전
달된다. 슬립 모드 동안 기지국은 슬립 BE 있는 단말로 ASE PUSS 버퍼링하거
터 버릴 수 있으며, 청취 구간동안 GEES Traffic Indication Message()MOB_TRF-IND)

를 보고 슬립 모드로의 복귀 또는 Awake 모드로의 변환을 결정한다. 여기서 173180

655



===== PAGE 652 =====
PART IV_MIMO-OFDM 통신 시스템

Indication 4655886는 단말로 전송할 새로운 EAB] 있는지 여부를 알려준다. 청취 구
간에는 단말이 수면 구간으로부터 깨어나서 DCDS} UCD 변화 카운트, DL-MAP PHY
동기 필드의 프레임 번호 검사 SS 통하여 기지국과의 동기를 맞추고 기지국의 신호를
청취한다. 그림 18.54는 슬립 모드의 동작 예를 보여준다. 수면 구간을 찌1 프레임이라고
했을 때 NI 프레임 후에 단말은 깨어나서 Ｌ1 프레임 구간 동안 기지국으로부터 Ass
청취하고, 기지국이 그 단말에 대하여 전송한 트래픽이 없다면 단말은 수면 구간을 두 wy
로 하여 다시 슬립 모드로 재진입한다. 이 절차는 수면 구간이 Max—window 같을 넘지
않을 때까지 지속된다.

MS                                                                  BS
MOB_SLP-REQ

(Initial-sleep Interval = N 1)
(Final -sleep Interval = N2)

MOB_SLP-RSP
(Start-frame = M)

-                             (Initial-sleep Interval =N1)
노무 ot Frente Number = Mi)                                     (Final-sleep Interval = N2)

Sleep mode,
for NI frames
a sae 이                        MOB_TRF-IND
4
|        listening, for LI frames*            (Negative Indication)
;          1)
Sleep mode,                                                                    PDU for the MSS
for 2*N1 frames **
MOB_TRF -IND
~———
|        Listening, for Ui frames              (Positive Indication)
cn sees|
Sleep mode,
for4* NI frames
Awake Mode
y

그림 18.54 슬립 모드의 동작 순서

18.8.8 앤드오버 절차

핸드오버란 현재 서비스 중인 005와 단말의 이동성을 보장하기 위하여 단말이 서비스
인 기지국에서 다른 기지국으로 이동할 때, 연결이 지속적으로 유지될 수 있도록 무선
크를 새로운 기지국으로 전환하는 기능이다. 와이브로에서의 핸드오버는 기존의 AAS
저 끊은 뒤, 새로운 기지국으로 연결하는 4}4)(break—before—make)?] 하드 핸드오버를
지원하지만, 핸드오버 과정에서 2개 이상의 기지국을 이용하여 신뢰성 높은 핸드오버를
지원하기 위한 소프트 핸드오버 기법도 고려될 수 있다.

0

rot

656


===== PAGE 653 =====
제18장_ 와이브로 시스템

핸드오버의 종류는 크게 세 가지의 관점으로 구분이 가능하다. 첫째, 물리적 위치에 따
핸드오버 관점에서 섹터 간의 핸드오버인 InterSector WE OH, 기지국간의 핸드오버
Inter-BS 핸드오버, 40#간의 핸드오버인 0\60-ㅅ0 핸드오버를 들 수 있다. 둘째로,
오버의 시작 주체에 따라 구분이 가능하다. MS—initiated HE SHE 단말의 관점에
드오버를 요청하는 것이고, BS—initiated 핸드오버의 경우는 기지국에서 단말의 상
파악하여 핸드오버를 수행하는 것이다. 셋째로, 핸드오버 방식에 따라 하드 핸드오버
소프트 핸드오버로 구분이 가능하다. 핸드오버는 크게 셀 재선택, 핸드오버 결정 및 개
, BA 기지국과의 동기화 및 핸드오버 레인징, 네트워크 재진입 및 단말 Context 종료
총 4단계로 진행된다. 그림 18.55는 초기 네트워크 진입과 핸드오버 절차를 보여준다.

ba   a   E

opi Gn Se

~«      ——Cell Rejected ————                                                           _ cal Rejected»
ㅋㅠ Cell Rejected—                                                        —Cell Rejected:
061 Rejected —                                                            -—      —Cell Rejected—       -

061 Rejected

Cell Rejected ——

Serving BS
(initial network entry)

00000    Neighbor BS

20000     Target BS

HO decision

그림 18.55 초기 네트워크 진입과 핸드오버 절차

657



===== PAGE 654 =====
PART IV_MIMO-OFDM 통신 시스템

첫 번째 단계인 셀 재선택을 위하여 단말은 MOB_NBR-ADV 메시지로부터 인접 기
지국 정보를 획득한다. 이후 셀 재선택 및 핸드오버 결정을 위해서는 핸드오버 시작 주체
에 따라 약간 다르게 진행된다. 그림 18.56(0에 나타난 바와 같이 MS—initiated 핸드오버
의 경우에는 서빙 기지국의 CINR(Carrier to Interference and Noise 800)이 문턱치 이
하가 되면 단말이 MOB-SCN-REQS 기지국으로 전송하여 스캐닝 구간을 MOB_
SCN-RSPS 통하여 수신 받고 인접 Ao] 대한 스캐닝을 수행하여 인접 기지국의 신호
BAS 측정한다. 이 때 서빙 기지국은 단말에 대한 서비스를 중단하고, 단말은 적합한 타
AAS 찾게 되면 Ga 기지국의 CINR 값을 포함하여 MOB_MSHO-REQS 기지국으
로 전송한다. 기지국으로부터 MOB BSHO-RSP7} 수신하면 단말은 MOB _HO-IND 메
ANAS 통해 서빙 기지국과 링크를 BAY 핸드오버를 취소 또는 거절하는 등의 최종 결
AE 서비스중인 기지국에 통보한다. 그림 18.56(6)에 주어진 BS—initiated WE OHS] 경
우에는 기지국에서 MOB_SCN-RSPS 먼저 전송하여 단말에게 인접 기지국의 AAS
요청한다. 인접 기지국을 스캐닝한 후 단말은 MOB-SCN-REPS 기지국으로 전송하며,
기지국은 수신된 정보에 따라 핸드오버 결정을 MOB-BSHO-REQS 통하여 전송한다.

MOB_NBR-ADV                                           MOB_NBR-ADV

~ MOB_SCR-REQ                             -
ao>|
MOB_SCN-RSP                                               MOB_SCN-RSP

+

MOB_MSHQ-REQ                        MOB_SCN-REP
MOB_BSHO-RPS                       MOB_BSHO-REQ
~~ MOB_HO-IND                 ~~ MOB_HO-IND
(a) MS-initiated HEOH 절차             (b) BS-initiated HE OH 절차

그림 18.56 핸드오버 주체에 따른 핸드오버 절차

Idle BEL 여러 개의 셀로 구성된 페이징 영역(08818 area) 내에서 단말이 이동할 경우
에 특정 기지국에 등록하지 않고 하향링크 트래픽 전송을 주기적으로 깨어나 수신하는 단말
의 전력 AAS 위한 메커니즘이다. Idle BEL 단말과 기지국간의 DREG-REQICMD 메
시지 교환을 통해 시작되며, 단말은 주기적으로 깨어나 기지국으로부터 해당 단말을 페이

658



===== PAGE 655 =====
제18장_ 와이브로 시스템

징하는 메시지가 있는지 여부를 페이징 채널을 읽어 확인한다. 1016 모드에서는 슬립 모드

는 달리 핸드오버와 같은 액티브 BES) SAS 수행하지 않기 때문에 단말의 전력을
감소할 수 있다. 슬립 모드에서 수면 구간과 청취 구간이 존재하는 것과 유사하게, 106 모
드에서도 주기적으로 깨어나 기지국과 동기를 맞춘 후에 페이징 채널을 읽는 과정으로 A
행된더.



===== PAGE 656 =====
GEES serr cre 시스템의 개요

3GPP(3™ Generation Partnership Project)o] = 3세대 셀룰러 통신인 WCDMA 표준
화 이후에 고속 데이터 서비스를 위하여 HSDPA(High Speed Downlink Packet Access)
와 HSUPA(High Speed Uplink Packet Access) 규격을 작성하여 3세대 이동통신 시스템
기술을 개량하여 왔다. 2004년 11월부터는 최대 데이터 전송률을 높이고 진화된 서비스를
위한 낮은 지연(10\ latency) 제공하기 위하여 3GPP LTE(Long Term Evolution) 표준
화가 시작되었다. 3GPP Ｌ1ㅠ의 표준화는 3GPP TSG-—RAN(Technical Specification
Group—Radio Access Network)o]4] 이루어지고 있으며 현재 ※61-8까지 진행되었다.
3GPP Ｌ18에서는 기존 300『에서의 WCDMA 무선 접속 기술을 이용하는 대신에 하향링
크에 OFDMA 방식과 상향링크에 SC-FDMA 방식을 사용하여 E-UTRA/UTRAN
(Evolved Universal Terrestrial Radio Access/Evolved Universal Terrestrial Radio Access
Network) 시스템의 표준화 ANS 진행하고 있다. 본 장에서는 현재까지 진행된 3GPP
LTE 861-8을 기반으로 물리계층 표준 기술을 설명한다[40][53][320]-[3251].

00000 Scpp LTE 오구 사항
3GPP LTE 시스템 요구사항은 &ㅅ14#28 회의에서 정식 승인되었으며, 기본적인 요구사
항은 다음과 같다.
(1) 최대 전송률
* 20MHz 대역폭, 하향링크 100Mbps, 상향링크 SOMbps 지원
(2) 이동성(0020611650)
ㆍ 0~15100/8에 최적화

660



===== PAGE 657 =====
제19장_ 3606 LTE 시스템

ㆍ 15~120102의 이동환경에서도 고성능 보장
ㆍ 최대 250km/h 또는 500102/까지의 이동환경에서 송수신 7
(3) RAN 지연(11600) 최소화
(4) 셀 커버리지
ㆍ 5102의 셀 반경에서 신뢰성 있는 통신, 3002 셀 반경에서 적은 성능 감소,
100km 셀 반경까지 고려
(5) Scalable 대역폭 (1.25, 2.5, 5, 10, 15, 20MHz) 지원
(6) 3GPP 및 non—3GPP 시스템과의 연동 지원
(7) MBMS (Mobile Broadcasting Multimedia Service) 기술 개선
ㆍ MBMS 기술을 위한 SFN(Single Frequency Network)2] 지원 가능
(8) CAPEX/OPEX (CAPital EXpenditure / OPerating EXpense) 최소화
(9) 기존 시스템과의 호환성 (Backwards compatibility)
(10) PS(Packet Switched) 기반의 다양한 서비스 지원
(11) Paired 50600002과 unpaired spectrum 지원

ofr

(12) Co-existence/co—location 지원

(13) 셀 내의 200명의 액티브 사용자 지원

“CRW 500 LTE 주요 특징

(1) 다중 접속 기술
ㆍ 하향링크 : OFDMA, 상향링크 : SC-FDMA
(2) AMC (Adaptive Modulation and Coding)
}향링크 : QPSK, 16 QAM, 64 QAM
*상향링크 : QPSK, 16 QAM
* Turbo 부호 : 1/3의 부호화 율, 구속장 8의 부호화기
(3) 공간 다중화 기술
ㆍ (2 또는 4) × (2 EEA) 하향링크, 상향링크 지원
ㆍ 다중 사용자 MIMO 지원
(4) FDD2} TDD 지원
(5) MBMS= 위한 SFN 운영

0

어

661



===== PAGE 658 =====
PART IV_MIMO-OFDM 통신 시스템

3GPP LTE 하향링크

GQQPAT 3CPP LTE] 하양링크 구조

3GPP LTE 하향링크 무선접속기술로는 OFDMA 방식이 채택되었다. 기본적으로
150의 부반송파 간격을 지원하지만 MBMS 전용 셀을 지원하기 위해 7.501의 부반송
파 간격을 추가적으로 지원한다. 반송파 간격이 150 인 경우에 다른 길이의 cP, 즉
normal CP(4.69us)2} extended CP(16.67us)S 지원하며, 어떤 종류의 CPS 사용하는가에
따라 한 So] 포함되는 OFDM 심볼의 개수가 달라진다. Normal 애의 경우 7개의
OFDM 심볼이 한 슬롯을 구성하며, extended (의 경우 6개의 OFDM 심볼이 한 슬롯을
구성한다. Normal CPS 사용하는 경우, 한 슬롯의 길이를 0.508로 유지하기 위해 6개의
OFDM 심볼은 4.6908의 (#길이를 사용하며, 한 OFDM 심볼은 5.2108의 (?길이를 사용
한다. 즉, 66.6706×7+4.69106×6+5.2106×1 = 50018로 주어진다. Extended CPS 사용하는
경우에는 66.6706×6+16.6708×6 = 500us 로 주어진다. 반면에 7.5012 부반송파 간격의 경
우에는 한 SH CPU 지원되며 한 슬롯은 3개의 OFDM 심볼로 구성된다. 표 19.1은
3GPP LTES] 하향링크 전송 파라미터를 보여준다. 3GPP Ｌ1에서는 FDD/TDDEY] 두 가
지 전송 모드가 모두 지원되며, 810ㅁ를 사용하는 4S Half/Full Duplex 모드가 지원된다.

표 19.1 3GPP 1ㄷ의 하향링크 전송 파라미터

| Transmission 8001.95 MHz 0 2.5 MHz 0005 MHz      10 MHz 15 10606 20 MHz
_ Subframe duration                               0.5 ms
1,92 MHz 3,84 MHz 7,68 MHz 15.96 MHz 23,04 MHz 30,72 MHz
(1/23,84 MHz)                    (2x3,84 MHz) (4×8.84 MHz) (6×8.84 MHz) (83.84 MHz)
| “~ 0:        256         512         1024        1536        2048
Bl al     76         151         301         601         901        1201
(4.69/9) x6, (4.69/18) x6, (4.69/36) x6, (4,69/72) x6, (4,69/108) x6, (4,69/144) x6,
(5.21/10) x1 (5,21/20)x1 (5.21/40) x1 (6,21/80)x1_(6,21/120)x1_—_ (6, 21/160) x1
“Long (16.67/32) (16.67/64) (16.67/128) (16,67/256) (16.67/384) (16.67/512)

_ 662



===== PAGE 659 =====
제19장_ 3606 LTE 시스템

QQ] 3cpp Ｌㄴ패의 프레임 구조

3GPP LTE 시스템은 FDD2} TODS 모두 지원하며, 그림 19.1는 LTE FDDo] 사용되
는 프레임 구조 Type 을 보여준다. 그림 19.1에 나타난 바와 같이 한 프레임은 =
307.200 x T, = 10ms2] 길이를 갖고 20개의 슬롯으로 구성된다. 각 슬롯은 Tyo = 15,360

xT, = 0.5ms9] 길이를 갖는다. 연속된 두 개의 슬롯으로 구성된 108의 AS 단위를 서
브프레임(646681006)으로 정의한다.

One radio frame, 7;)= 307,200 x 7: = 10ms

One slot, Tw = 15,360 x 7; = 0.5ms

그림 19.1 3GPP LTE 프레임 742 Type |

FDD 모드인 경우, 상향링크와 하향링크 전송이 주파수 영역에서 서로 분리되어 있기
때문에 10ms2} 프레임 구간 동안 하향링크와 상향링크로 각각 10개의 서브프레임을 전송
할 수 있다. 반면, TOD 모드인 경우에는 1008의 프레임 구간 동안 매 서브프레임마다 상
향링크나 하향링크 중 한쪽 방향으로만 전송이 가능하다.

One radio frame, Ty =  BO G200K) 7, =  =)

1
| One half- “frame, 153,600 x 2; = Sms
a

One slot,                         SK
in = 15,360 * T,     30,720 x %        ~S

One subframe,
307207,                                                            |                \
DwPTS GP        UpPTS                                          DwPTS GP        UpPTS

그림 19.2 3GPP LTE 프레임 2 Type II

663



===== PAGE 660 =====
PART IV_MIMO-—OFDM 통신 시스템

그림 19.2는 TDD 사용되는 프레임 구조 Type US 보여준다. 그림 19.2에 나타난 바
와 같이 한 프레임의 길이는 프레임 FA Type 1와 동일하게 1005이고, Sms 길이 2 개의
+= Za] A (half—frame)°o 2 구성된다. 각 하프프레임은 0.5088 길이의 8개의 슬롯과 2개
슬롯 길이를 갖는 DwPTS(Downlink Pilot Time Slot), GP(Guard Period), UpPTS(Uplink
Pilot Time 8100)으로 구성된다.

GQ] 3cpP LTE] 슬로 구조

3GPP LTE 하향링크 ASASE 그림 19.30] 나타난 바와 같이 시간영역에서 NOL, 7H

의 OFDM 심볼과 주파수영역에서 NLP 72] 부반송파로 이루어진 RB(Resource Block)
단위로 자원 할당이 이루어진다. 따라서 한 RBS ^" XN, 개의 Resource Element
이루어진다. RB of NPL & 사용하는 부반송파 간격과 CPol] 따라 다르게 적용되며, 표
19.2에 나타난 바와 같이 시간영역에서 한 SKI 주파수영역에서 1801에 해당한다.
즉, 한 SEO 7개 또는 6개의 OFDM ASH 구성되며, 한 슬롯에 포함된 심볼의 APE
(#의 길이를 알려주는 상위계층 제어신호 정보에 의해서 결정된다. MBMSS 지원하는
경우 한 슬롯에 3개의 OFDM 심볼이 전송되고, 한 88에 24개의 부반송파가 할당된다.
그림 19.3은 normal CPS 사용하는 경우의 하향링크 물리계층 자원구조를 보여준다.

|

표 19.2 물리계층 자원 블록 파라미터

Ne                       Ne
7
12
6
24                           3

그림 19.3에 나타난 바와 같이 Ney ^," 개의 부반송

3GPP LTE 하향링크 전송신호
파와 40 개의 OFDM 심볼로 구성된 Resource Grid 주어진다. 하향링크 RB] 개수
Nee 는 전송 대역폭에 따라 따르며 다음과 같이 주어진다.

clr

Ne <N oN                                 (19.1)

여기서, Neh’ =6, Nes?" =110이다.

664



===== PAGE 661 =====
제19장_ 3660 LTE 시스템

One downlink slot 7,,,

Nyy OFDM symbols

}                       k= NDLx NRB-1
Resource block
al Nom X Ne? resource element
이
은 @
a ©
85
a §                     Resource element (k, /)
Ze 8
xb
a                a
k=0
1=0                    1=NQ%, 71
그림 19.3 3GPP LTEQ| 하향링크 자원 할당 구조
0 241 3005 LTEY] 하향링크 물리 채널의 기본 구조

3GPP LTE 하향링크 물리채널 구조는

그림 19.4에 나타난 바와 같이 입력
Precoding++, Resource Element 맵핑부, OFDM 신호   aes 거친 후에 각 안테나로 전
송된다. 여기서 Layer 맵핑부과 Precoding =         O 전송과 관련이 있어 19.4절에서 자
세히 설명한다.

채
그림 19.4와 같이 주어진다
신호

665


===== PAGE 662 =====
PART IV_MIMO-OFDM 통신 시스템
code words                                                                      layers                                                                         antenna ports
a |

12 19.4 3GPP Ｌ1ㄷ의 하향링크 물리채널 구조

“GURY 3GPP LTE] 하향링크 채널
3GPP LTES] 하향링크는 기본적으로 다음 6개의 채널로 구성된다. 각 채널의 기본적인
구조는 그림 19.4와 같으며 각 세부 블록은 채널에 따라 조금씩 차이가 있다.

(1) PDSCH(Physical Downlink Shared Channel)

PDSCH= 선택된 단말에게 데이터를 전송하는 데 사용되는 채널로서, POCCHS 통하
여 선택된 단말과 데이터 전송에 필요한 채널 부호화 등의 정보가 전송된다. PDSCHY|
구조는 그림 19.4에 주어진 바와 같고, 스크램블링의 경우 부호화된 비트 레벨에서 하향링
크 Al 기반 스크램블 부호가 사용된다. 하향링크 변조에는 QPSK, 16QAM, 64QAM 방식
이 사용된다. UE-specific RS7} 전송되지 않는 경우, PDSCHS| 전송에 사용되는 안테나
포트는 {0},{0,1},{0.1.2.3}이다. 다중 안테나 전송의 BPS] 안테나 포트는 전송되는 RS
에 따라 정의되며 6011-9060100 #8의 전송과 관련된 포트는 {0,1.2.3}이다. MBSFN RS
의 전송과 관련된 포트는 {4}, UE-specific 88의 전송과 관련된 포트는 {5}로 정의된다.

(2) PBCH(Physical Broadcast Channel)

PBCHE 셀의 특정한 시스템 파라미터와 같이 특정 셀 내의 BE 단말들이 수신해야
하는 정보들을 전달하는 방송용 물리 채널이다. PBCH 채널을 통해 이용 가능한 랜덤 A
세스 ALBA, 엑세스 슬롯, MIMO 타입, TxDiv 타입 등이 전달된다. 단말이 PBCHS 복
호할 수 없으면 Ao] 등록할 수 없기 때문에 커버리지 영역 내의 모든 단말들에게 적은
에러율로 전달될 수 있도록 상대적으로 높은 전력으로 전송된다. PBCHE 모든 단말이 복
호할 수 있도록 중심 주파수 근처의 6개의 RBO 할당되며 1번 슬롯의 0~3번 OFDM 심
=o] 전송된다. 그림 19.5는 서브프레임 내에 PBCH7} 할당된 HAS 보여준다.

666



===== PAGE 663 =====
AiO BGPP LTE 시스템

System bandwidth                 1,08 MHz (=6 RB)
>

Sub-frame

|                                                         \
‘                                    Z                   \

\
\
PBCH (slot 1)                                 SCH  (slot 0)

그림 19.5 3GPP LTE 하향링크 물리채널의 자원할당

(3) PMCH(Physical Multicast Channel)

PMCH+= MBMSS 위해 지원되는 방송 채널이며 HAE 그림 19.49} 같다. PMCHE
방송 채널이기 때문에 송신 다이버시티 기법이 적용되지 않으며, MBSFN RS7} 전송되는
안테나 포트 {4}를 통하여 전송된다.

(4) PDCCH(Physical Downlink Control Channel)

PDCCHE 단말에게 할당된 자원, 변조, H-ARQ 등의 스케즐링 정보와 그 밖의 제어
ABS 전송한다. POCCHE 하나 이상(1,2.4.8)의 인접한 CCE(Control Channel Element)
들의 집합으로 구성된다. 여기서 CCE Resource Element2] 집합을 나타낸다. PDCCH
의 각 채널은 다른 부호화 율과 다른 수의 부반송파로 구성되나, 모든 제어채널은 QPSK
단일 변조기법이 적용된다. PDCCHY 하향링크 슬롯의 처음 3개의 OFDM 심볼에 위치
할 수 있는데, 이 때 사용되는 OFDM 심볼의 = PCFICHS 통해 전달된다. 단말에서
PDCCHE 복조할 경우에 단말에게 할당된 몇 개의 20001 그룹에 대해서만 복조를 수

경우 모니터링 해야 하는 그룹 정보는 상위계층 신호를 통해 전달된다.

(5) PCFICH(Physical Control Format Indicator Channel)
PCFICH= 서브프레임 내에 PDCCHS] 전송에 사용된 OFDM 412] F(n=1,2,3)S
알려주며, 서브프레임의 첫 번째 OFDM 심볼에 (029로 변조되어 전송된다.

667


===== PAGE 664 =====
PART IV_MIMO-OFDM 통신 시스템

(6) PHICH(Physical Hybrid ARQ Indicator Channel)

PHICH= Hybrid—ARQ ACK/NCK2 전송한다. 동일한 Resource Element 집합으로
맵핑된 다수의 PHICHS PHICH 그룹으로 정의하는데, 이 때 동일 PHICH 그룹 내의 다
수의 PHICH=: 각각 다른 직교 AAAS 통해 분리된다. PHICH 자원은 인덱스 쌍
070 77899. JO 구분된다. 여기서 70. 는 PHICH 그룹 넘버, ny = 그룹내의

직교 AAA 인덱스를 나타낸다. PHICHJE BPSK 변조기법이 적용된다.

신호(00\101106 518081)는 상위 ASA 내려오는 정보가 아니고 물리계층에
소멸되는 제어 정보로서 SEAS 내에서만 의미가 있다. 하향링크 신호에는
등에 사용되는 RS(Reference 918081)와 동기를 획득하는 데 이용되는 SS
(Synchronization Signal)°] 있다. 하향링크 RS PDSCH, PDCCH, PCFICH, PHICH 등
의 채널에서 coherent SAS 위한 IIS ASS 제공한다. RSE 셀 내의 모든 사용자가
공유하는 061-806010ㅇ RS, MBSFN 전송 시 사용되는 MBSEN RS, 특정 사용자 만을
위한 UE-specific #8로 구분된다.

(1) Cell-specific RS

Cell—specific RS& 7] 24° non—MBSFN 414-2 위해서 사용되며, non—MBSFN
를 지원하는 셀에서 모든 하향링크 서브프레임에 ASH. Cell—specific RS2= PN 시
BAT 사용되고, 단말기에서는 #5가 제공하는 파일롯과 보간 기법 등을 사용하여 AS
추정한다. 또한 단말기는 0611-6060180 RSS 측정하여 CQK(Channel Quality Indicator),
PMI(Precoding Matrix Indicator), RI(Rank Indicator) 정보를 -기지국에 알려준다.
Cell—specific RS-2 한 개 또는 다수 개의 안테나를 통해 ASS 수 있으며, 1SKHzo] 부반
송파 간격에서만 사용된다. 061-806080 8#8는 다음 Alo} 의하여 생성된다.

r,,,, (m) =—=(1—2-c(2m))     1-2-c(2m+1)),  m=0,1,---,2NR™* -1      (19.2)

_ 1
고

‘al

여기서 는 슬롯 번호, 12 슬롯 내 OFDM 심볼 WSs 나타낸다. 또한 00) 는 PN
ANABAS 나타내며, 각 OFDM 심볼 시작 시 <, = 2° +2? -[n,/2 + Ni! 로 초기화 된

init

다. 여기서 U’=(n,mod2)-Nony +2 로서 서브프레임 내 OFDM 심볼 WSS 나타낸다.

_668



===== PAGE 665 =====
M192 SGPP LTE 시스템

식 (19.2)에 의해 생성된 RS 시퀸스 Ty, (Me 복소 변조심볼로 맵핑되어 슬롯 의 안
테나 포트 {7} 의 7|AX(reference) 심볼로 사용된다. Cell—specific RSH MBMS 사용여부,
MIMO 사용여부, 안테나 개수, CP 종류에 따라서 배치가 달라진다. 그림 19.6과 그림
19.7은 CP HES} 안테나 개수에 따른 0611-9060100 RS 배치를 보여준다. SISO 시스템
에서 normal CPS 사용하여 한 슬롯이 7개의 OFDM ASE 구성된 경우, 그림 19.7에
나타난 바와 같이 RSE 슬롯의 A 번째 심볼과 SHA ASS Ro 위치에 전송된다. 2개의
안테나를 사용하는 경우에 RS 첫 번째 안테나의 Ro 위치에, 두 번째 안테나의 4, 위치
에서 각각 전송된다. 안테나를 4개 사용하는 경우에는 #8가 각각 Ro, Ri, Ro, Rs 위치에
서 전송된다.

aia   TW

=                        |
a
at
aa!           더
그
이
=
@
오                           +—+
i=
6         지           my
1=0       :       1=6 [=0      |       1-6
i                i                                                   Resource element(k, 7)
별            ro        rr        a ae
-2e000 66" S66 a8 Se
은                           |                           an
등                                                       MN
a
a                                  i           4
5                                                      aa          Not used for transmission on this antenan port
=
기
°                           [|
é            더                mt 시                x
Reference symbols on this antenna port
a        Ts        TT                      |
0      1]      1=6 /=0      1=6 7=0            1=6 7=0            6
              (PES |      |      13]      |        |              le]           베베:         fete]
21020 seas ey  2240
iB                                       =            St Te
8
184 02                                  브리 Samm               5
노
|       | 」
AAT                                        | | 162 |        Q
1=0       :       1=6 1=0      :       1-6 1=0       :      1=6 I=0      :       1=6 1=0       :      1=6 1=0       :       1=6 1=0      ;      /=6 7=0       :       1-6
even-numbered slots odd-numbered slots     n-numbered slots odd         slots, ,e           slots odd-numbered slots    even-numbered slots odd-numbered slots
Antenna port 0                          Antenna port 1                          Antenna port 2                          Antenna port 3

그림 19.6 안테나 개수에 따른 Cell—specific RS 배치 (normal CP)

669



===== PAGE 666 =====
PART IV_MIMO-OFDM 통신 시스템

One antenna port

개

~ eons  element(k, 1)

aa RAV

Not used for transmission on this antenan port

Two antenna ports
|= |
Le
Heh

A
브
|

Reference symbols on this antenna port

1 | | 1 | «|      I]                |
150       i       I=5 1=0      :        =5 J=0              1=5 I=0               I=5
eS        1 S| Ba       더                테   [    (BEL
'    고            34 |       Oe           | | |         OK     니
은                                 C1                      년       2
        |       g
a    a    ^      UI            디
7=0       i       1=5 /=0      ‘       7=5 7=0       :       I=5 I=0       내        1=5 7=0       [1      71=5 /=0       1        71=5 7=0      7=5 7=0       1       71=5

even-numbered slots odd-numbered slots even-numbered slots odd-numbered slots, ,6460-1147106100 51015 odd-numbered slots. _ even-numbered slots odd-numbered slots

Antenna port 0                         Antenna port 1                          Antenna port 2                          Antenna port 3

그림 19.7 안테나 개수에 LH= Cell-specific RS 배치 (extended CP)

(2) MBSFN RS

MBSFN(Mobile Broadcasting Single Frequency Network) RSH MBSFN 전송 시에
사용되며, 안테나 HE {4}로 전송된다. MBSFN RS* extended (만 사용한다. 슬롯 번
호 %, 슬롯 내 OFDM 심볼 번호 /에서의 MBSFN RSE 식 (19.2)을 사용하여 생성되
FA, Cine = 21° +2? -Ln,/2]+ NIP 로 초기화 된다. 그림 19.8은 부반송파 간격에 따른
MBSFN RS2| 배치를 보여준다. 그림 19.806)는 MBSFN-dedicated 08]로서 Af =
7.51032 의 경우에 MBSFN 85의 배치를 보여준다.

670



===== PAGE 667 =====
제19장_36060 LTE 시스템

   | |

R;
Ry                                                                           Bee
2                 끄
Re                        m«.
Ry
Ry                         [mT
I=0        :        I=5 I=0         :         1=5                                       150 :i=2 10: 7=2
slots      odd:          slots                                    even-numbered slots odd-numbered slots
Antenna port 4                                                                Antenna port 4
(a) Af =15kHz                                               (b) Af =7.5kHz

그림 19.8 MBSFN RSQ] HHAl(extended CP)

(3) UE-specific RS

3GPP LTE 시스템은 넓은 셀 커버리지를 지원하며, 셀 경계에 위치한 단말의 전송률
증가 또는 QoS USS 위하여 빔형성 기법을 사용할 수 있다. 이 때 기지국은 안테나 가
중치를 AAS 위하여 단말이 전송한 상향링크 RSS 통하여 채널정보000ㅅ, 평균 경로 손
실)를 획득할 수 있다. 안테나 가중치는 6011-8060180 RS] 적용될 수 없으므로 빔형성을
위한 UE-specific RS2} Z& dedicated RS7} 필요하다. 이 경우 단말은 UE-specific RS
을 이용하여 PDSCHS coherent 복조할 수 있으며, UE-specific RSE 안테나 포트 {5}
를 통해 전송된다. UE-specific 88로 PN A)AA7} 사용된다.
단말은 상위 계층 시그널링에 의해 UE-specific RS7} 존재하는지, 해당 RS7} PDSCH
AS 위한 #8인지의 여부를 알 수 있다. UE-specific 88는 PDSCH] 맵핑된 88에만
며, 다음 식으로 주어진다.

마

OL

그

BA
Oo

671



===== PAGE 668 =====
PART IV_MIMO-OFDM 통신 시스템

rm) =e (I-2-e(m)) + je (I-2-e2m-+),       m=0,1--,12NRp -1 (19.3)

여기서 Neg = 해당 20901에 전송되는 RBS] 대역폭을 나타낸다. 또한 ㅇ0)는
PN AAAS 나타내며, 각 서브프레임 시작 시 PN ABA 발생기는 < =2'” 01 +
2°-[n,/2|+Nis' 로 초기화 된다. 그림 19.9% normal CPS 사용하는 경우에
UE-specific #8의 배치를 보여준다.

ㅁㅁ

oes
moe

3        a
Bi

1=6 1=0 :              1=6

even-numbered slots  ,。 ,    odd-numbered slots

Antenna port 5

그림 19.9 UE-specific RS2| HHXl(normal CP)

그림 19.100] 나타난 바와 같이 동기신호는 한 프레임내의 0번 슬롯
2번 전송되며, 각 슬롯의 SH 심볼에 서로 다른 SSS(Secondary Synchronization Signal)
와 각 슬롯의 마지막 심볼에 동일한 PSS(Primary Synchronization Signal)7} 전송된다. 또
한 그럼 19.5에 나타난 바와 같이 BCHS} 동일한 대역에서 전송된다. 이와 같이 동기신호
는 동일한 PSS} 서로 다른 95로 구성되어 504개의 셀을 구분한다. 504개의 셀 10 는
168개의 고유한 물리계층 AID 그룹과 각 그룹에서 3개의 고유한 물리계층 IDs] 조합을
통해 생성되며 다음 식으로 주어진다.

672



===== PAGE 669 =====
제19장_3666 LTE 시스템

One radio frame
006 shot
One subframe
#0      Pie] =o oe    #10     Ole 4 ————-————        #18     #19
x       “Ae            책
Be        Ns          NG
세           ~           \,
\ Ss.         \.
‘            *Ss       ‘
0)1)2/3)4    07; 1)213)4)51/6
: 686

그림 19.10 3GPP LTEQ| 동기 신호(프레임 구조 Type |)

Nip =320음 + NB                                          (19.4)
여기서 Nip 는 0~167의 범위를 갖는 물리계층 셀 10 그룹, ME 물리계층 AD 그
룸 내에서 0-29) WS 갖는 물리계층 IDS 나타낸다.

ㄴㄴ 5105 단위로 시간 동기, 주파수 동기와 물리계

리계층 IDS 획득
영역에서 Zadoff—Chu 시퀸스를 사용하여

획득할 수 있도록 Pass
다음과 같이 주어진다.
__,Aun(n+l)
e    63       n=0,1,--+,30
dy 00 ~    je                                                       (19.5)
e      es      n=31,32,:--,61

여기서 Zadoff—Chu root 시퀸스의 인덱스

표 19.3 PSS #

2 od
발생을 위한

673



===== PAGE 670 =====
개

PART IV_MIMO-OFDM 통신 시스템

그림 19.10에 나타난 바와 같이 프레임 구조 Type 1에서 PSS 0번 SEF} 10번 슬롯
의 마지막 OFDM 심볼을 통해 전송되는 반면, 프레임 TA Type [에서는 서브프레임 1
번과 6번의 3번째 OFDM 심볼을 통해 전송된다.
PSSS 검출한 후, 단말은 598를 이용하여 프레임의 시작위치와 물리계층 셀 12 그룹
T

(19.6)

여기서 8" (n) 와 s(n) 는 m-AJBA, 900) 와 (7) 는 288에 의해 주어진 스크랩
블링 시퀸스이다. AID TSS 인덱스 my (0~29)2}_m, (1~30)2] 조합을 통하여 Nip
(0~167)가 발생된다.

그림 19.112 PSS} SSSS 이용한 동기 및 Al
PSSS 이용하여 Sms 단위로 시간 동기, 소수배 반송
한다. 그 후, 888의 앞 심볼에 위치한 SSSS 이용하여 물리계
시작 위치, 정수배의 반송파 주파수 동기를 획
룹과 PSSS 통해 획득한 물리계층 IDS 조합하여 AIDS 추정함으로써 동기 및 셀 탐색

과정을 완료한다.

보여준다. 단말은

리계층 IDS 획

ce
|0 조

그림 19.11 3GPP LTES| 동기 및 셀 탐색 과정

674



===== PAGE 671 =====
GREED scrr cre vega

CRA] Scpp 의 상앙링크 구조

3GPP LTE 상향링크 전송신호는 그림 19.12에 나타난 바와 같이 시간영역에서 NYE,
개의 OFDM 심볼과 주파수영역에서 NLP 72] 부반송파로 이루어진 RB(Resource Block)
단위로 자원 할당이 이루어진다. 따라서 하나의 RBS NLP x NYE, 개의 Resource Element
로 이루어진다. 상향링크에서 NREL 12, NG, 는 normal CP2] 경우 7, extended (의
경우 6으로 하향링크와 동일하게 주어진다. 즉, 하나의 RBS 시간영역에서 한 슬롯과 주
파수영역에서 180KHzo]] 해당한다. 또한, 3GPP LTE 상향링크 전송신호는 그림 19.12에 나
타난 바와 같이 New Ne? 72] 부반송파와 ^ 개의 SC-FDMA 심볼로 구성된
Resource Grid 주어진다. 상향링크 RB 개수 Nes 는 AS 대역폭에 따라 따르며 다
음과 같이 주어진다.

NRIAUL < NUL < NEEUL                             (19.7)

여기서, Nes =6, Nap =110 이다.

SC) 3cPP LTE2] SC-FDMA

3GPP LTE 상향링크 무선접속기술로는 FDDS} 7200에서 모두 SC-FDMA 기술을 4}
용한다. SC-FDMA 기술은 7.2.4절에서 설명한 바와 같이 송신단 변조과정에서 IFFT 입
력 전에 사용자 별로 DET 처리과정을 수행하고, 수신단 복조과정에서 FFT 출력신호를
IDFT 처리함으로써 상향링크 송신단에서 발생할 수 있는 2400을 최소화하여 단말의 전
력소모를 줄인다. 그림 19.13은 SC-FDMA 송신단 구조를 보여주며, 표 19.4는 상향링크
전송 파라미터를 요약하여 보여준다.

675 _



===== PAGE 672 =====
PART IV_MIMO-OFDM 통신 시스템

One uplink slot Ty.

a                    S.
/                      +.

/

,                          S.
/                           내

‘NPE, SC-FDMA symbols

k=Neyx NEP-1

Resource block
a NSDL x NE® resource elements

Resource element (&, /)

x N®® subcarriers

N&® subcarriers

Nee

k=0
1=0         1= NDE -1

22 19.12 3GPP Ｌㄴ1ㄷ의 상향링크 자원 구조

Coded symbol rate=R

!                                                                                                                                                                        1
i                                                                                                                                                                        \
|                                                     !
ㅣ                                                                                                                                          '                                                                                                {
H        sel 11                                '  |Sub-carrier} !
'                                      ~                                                   '

|                                  _   Mapping | |         wii                                  |
|            ——’                                        .                             i                                                                     1
                                                               {                                            |
ㅣ                                                                                                                                          로                                                                                                1
1                                                                                                                                                           1
ㅣ                                                                                                                                                                           1
{                                                                                                                                                                           i
i                                                                                                                                                                           1
                                                                                                                                                                           ul

Nrx symbols

Size-Nrx                         Size-Nert

676



===== PAGE 673 =====
제19장 _3666 LTE 시스템

# 19.4 3GPP LTEQ| 상향링크 전송 파라미터

Slot duration (ms)                        |                                   0.5

Sub-carrier spacing (KHz)                         15
Sampling frequency (MHz)                15,36            30,72
FFT size                        1024            2048
Number of occupied sub-—carriers     |        600            1200
CP length                   Short              (4,69/72) x6,      (4,69/144) x6,
(us/samples)       :                                             (5.21/80) x1          (5, 21/160) x1
The # of sub-carrier per Resource Block (RB)         12               12
The # of RB per slot                   20              110
The # of Resource Element (RE) per RB       84 (10 × 0)          84
The # of Reference Symbols (RS) per RB ©        12             12
The # of RB used for PUCCH per slot             2               2
The # of RB used for PUSCH per slot            48              98

그림 19.130] 나타난 바와 같이 입력 데이터는 DET 처리 과정 후 정해진 규칙에 따라
해당 주파수 대역으로 연속적으로 할당된다. 이후 IFFTRS 거쳐 애가 삼입된 후 전송된
다. 10 MHz 대역폭을 사용하는 경우, 부반송파 간격은 15, 샘플링 주파수는
15.36MHz, 부반송파 == 1024, 유효 부반송파 수는 600, 유효주파수 대역은 9MHz°o =
주어진다. 최대 DFT 크기는 1200, CPE 하향링크와 동일하게 normal (와 extended CP
가 존재한다. 한 0.508 슬롯은 normal (#의 경우에 7개의 SC-FDMA 심볼, extended
CP2] 경우에 6개의 SC-FDMA 심볼로 구성된다.
연속시간에서 / 번째 상향링크 SC-FDMA 심볼은 다음과 같이 정의된다.

[VRB NE? /2 | 그          |
s(t)= xy, eM ME) | 0<7흐(00 + N)XT.              (19.8)

k=-| NeENE? /2|                                                                                           "

여기서 KO =k+ [NR /2 |, N=1024/ 2048, Af =15kHzS 나타낸다. 상향링크
SC-FDMAA}= 하향링크 OFDMAS} 달리 반송파 주파수 옴셋(0.5)을 발생시커, DC
해당하는 부반송파에 데이터를 전송한다.

677



===== PAGE 674 =====
PART IV_MIMO-OFDM 통신 시스템

soos 물리 채널의 기본 구조

링크 물리채널 구조는 그럼 19.14와 같이 주어진다.

그림 19.14 3GPP Ｌㄴ1ㄷ의 상향링크 물리채널 구조

그림 19.14에 나타난 바와 같이 입력 신호는 스크램블링부,， HAD, Precoding},
Resource element 맵핑부, SC-FDMA 신호 발생기를 거친 후에 각 안테나로 전송된다.

000 SGPP LTES] 상양링크 채널

(1) PUSCH(Physical Uplink Shared Channel)

PUSCHE 단말이 기지국에게 데이터를 전송하는데 사용하는 상향링크 채널이며,
PUSCHY] 구조는 그림 19.14에 주어져 있다. 스크램블링코드의 경우 부호화된 비트레벨
에서 UEZ|8} 스크램블 부호가 사용되며, QPSK, 16QAM, 64QAM 변조기법이 사용된다.

(2) PUCCH(Physical Uplink Control Channel)

PUCCH 상향링크 제어 정보를 전송하는 채널이다. 상향링크 데이터 전송이 없는 경
우, PUCCHE 제어정보만을 사전에 예약된 자원영역을 통하여 전달한다. 그림 19.15는
PUCCHY] 자원할당을 보여준다.

7200=/말-1

Nexs=0

<— One subframe ——>

그림 19.15 PUCCH9| 자원할당

_678



===== PAGE 675 =====
제19장-36『『 LTE AJA

그림 19.15에 나타난 바와 같이 ?20001의 자원단위는 하나의 부호와 2개의 RBZ 이
루어져 있으며, 슬롯 경계에서 호핑이 가능하다. 상향링크 단일주파수 SYS 유지하기 위
해서는 한 단말이 두 다른 자원을 동시에 사용할 수 없기 때문에 단말이 PUCCHS 전송
하는 경우에는 PUCCHS} PUSCHS 동시에 전송할 수 없다. 즉, SC-FDMAAE
100811260된 자원이 단말에 할당되며, 이와 같은 10084200된 자원이 단말에게 여러 개가
할당될 경우에는 PAPR| 증가하게 된다. 따라서 상향링크 데이터 전송이 있는 경우에는
단일주파수 특성을 유지하기 위해 할당 받은 데이터용 자원영역을 통해 데이터와 제어정
보를 함께 전송한다: PUCCHS 통해 ASHE 제어 정보에는 001, HARQ, ACK/NAK,
scheduling request 등이 있으며, MIMO2] 경우에는 CQI2} 함께 PMI(Precoding Matrix
100108100)와 같은 피드백 정보가 추가되어 전송된다.

(3) PRACH(Physical Random Access Channel)

PRACHE 단말이 기지국에 접속을 요청할 경우에 사용되며, 1.08MHz 대역(6 RB)
전송된다. 그림 19.16은 랜덤 엑세스 프리앰블을 보여준다. 그림 19.16에 나타난 바와 같
이 PRACH= CP(T., St 프리앰블 ABATE 구성된다. 8#ㅅ01의 각 필드별 길이
는 상위계층 신호에 의해 설정되며 표 19.5에 그 값이 주어져 있다. 표 19.5에서 프리앰블
2M 4는 TDD 프레임 구조에서만 사용된다.

fo | 28000

270                                                   7680

<            ae)                                                                 we
<         >t                                                 …

그림 19.16 랜덤 엑세스 프리앰블

19.5 랜덤 엑세스 프리앰블의 파라미터

3168-T,                       24576-T,
21024-T,                      24576 -T,
6240-T,                     2-24576-T,
21024-T,                    2-24576-T,
448-T,                          4096-T,

679



===== PAGE 676 =====
PART IV_MIMO-OFDM 통신 시스템

PRACH*: Zadoff-Chu 시퀸스를 순환 이동시켜 생성된 64개의 프리앰블
프리앰블 시퀸스는 다음 식에 의하여 생성된다.

을 사용하며,

_ Tun(n+1)

x,(n)=e 제 , OSnNSNyc-]          (19.9)

여기서 Nec ABA 길이를 나타내며, 표 19.60] 그 값이 주어져 있다.

표 19.6 랜덤 엑세스 프리앰블의 시퀸스 길이

0-8                                      839
4                                                           139

“S085 3GPP LTE2] 기준 신호(86+6760ㅁㅇ06 Signal)

상향링크 &8는 PUSCH2} PUCCHE] coherent 채널추정에 이용되는 일반적인 DM-
RS(DeModulation Reference Signal)2} 상향링크 스케즐링을 위해서 상향링크 채널품질
을 측정하는 데 사용되는 S—RS(Sounding Reference Signal)7} 있다. 할당 대역폭이 3
개 이상의 RBS 구성된   sii 상향링크 RSS AWS 48°] $2 Zadoff-Chu 시퀸스
를 Agta, 2개 이하인 경우에는 2    passe 주 좋은 시퀸스를 컴퓨터로 생성하여 사용
한다. DM-RSS} S-RSE 동일한 ABA 집합을 통해 다음과 같이 생성된다.

h(n) =e!"7, 00, OSn< MR               (19.10)

여기서 RSS] 길이는 ME =mNEP, 1S ms Ngy' 을 만족하며, 다수의 단말을 위한
RS ABA )는 기본 ABA, (1) )를 oc VES 순환 이동시켜 생성된다. we (0,1....,29}
와 는 각각 그룹 넘버와 그룹내의 기본 ABA 넘버를 나타낸다. 그룹 번호 vo} 그룹
내의 AMA 번호 "는 시간에 따라 변화될 수 있다. 기본 ABA FM) 는 ABA 길이
MS oj) 따라 다음과 같이 정의된다. 먼저 44>340쁜인 경우, 기본 시퀸스
7,.(0),--%,,(MS -1) 는 다음과 같이 주어진다.

__ 680



===== PAGE 677 =====
제19장_36066 LTE 시스템

F,y(n)=x,(nmodN7e), O<n< MRS              (19.11)

여기서 g=|7+1/2\+v-(-D°", F=NE-(ut+)/312 주어지고, 40 root Zadoff—Chu
ABAE 다음 식으로 주어진다.

__mgm(m+l)
RS
x,(m)=e    Nec  O<ms NBS -1

(19.12)

A} (19.12)에 주어진 Zadoff—Chu 시퀸스의 길이 NOE My wr} 작은 최대의 Ao]
다. 또한 기본 ABAD] 길이가 MB =7740", m=l,2 2 주어지는 경우, 기본 AAA
는 Che 쉬으로. 주어진다:

02) =67001. O<n< MSS-1               (19.13)

여기서 @00) 의 값은 mo 그룹 번호 /에 따라 주어진다.

(1) DM-RS

DM-RS*= PUSCH$} PUCCH®] 채널추정에 이용된다. 4] (19.10)에 나타난 바와 같
이 RS= 30개의 AAA AHS 가지고 있다. 이 30개의 A]BA-4=E (sequence shift)
패턴과 17개의 호핑 패턴을 통하여 각 셀에서 사용될 88 시퀸스 THO] 결정된다. 19.2.7
절에서 설명한 504개의 Cell IDS} 이 RS 시퀸스 AHS 일대일의 관계가 있어 셀간 간섭
을 최소화하도록 셀 구성을 한다. PUSCHS| 채널추정에 이용되는 DM-RSE 각 슬롯의
3 번 OFDM 심볼을 통해 전송되며, PUCCHS| 채널추정에 이용되는 DM-RSE 각 슬롯
의 2, 3, 4 번 심볼ㅠ0ㅁ0(끄 2 =1,1a,1b) 또는 1, SH 심볼(ㅁ\0ㅁ(71 4 =2.28.26)에서

전송된다.

(2) S-RS

S-RSE 각 단말의 상향링크 채널품질을 측정하는 데 이용되는 신호로서, 각 서브프레

임의 마지막 심볼에 위치하고 4개의 RB 단위의 정수 배의 길이를 갖는다.



===== PAGE 678 =====
PART IV_MIMO-OFDM 통신 시스템

. 00008 Scpp LTE 랜덤 엑세스 절차 및 타이밍 제어

랜덤 엑세스는 단말이 기지국에 등록하고자 할 때 수행하는 과정으로서 랜덤 엑세스는
비동기(000-585000001260)와 -§-7](synchronized) 방식으로 구분된다. 비동기 엑세스 방식
은 단말이 기지국에 최초 접속하거나 상향링크 동기를 상실했을 때 수행되며, 단말은 64
개의 랜덤 엑세스 시퀸스 중 임의로 한 개를 선택하여 랜덤 엑세스를 수행한다. 비동기 엑
_ 상향링크 AASVS 적용하기 전에 수행되므로 다른 단말들로부터 전송되는 상향

A 신호와 셀 내에서 충돌이 발생할 수 있다. -|F7|(synchronized) 엑세스 방식은 기지국
3} 시간 동기가 수행된 WH] 1016 모드 또는 핸드오버 Ajo] 수행하는 엑세스 방식으로
64개의 랜덤 엑세스 ABA 중 한 개를 할당 받아 랜덤 ANAS 수행한다.

랜덤 엑세스 절차를 요약하면 다음과 같다. 우선 랜덤 엑세스가 시작되기 전에 상위 계
층으로부터 사용 us 랜덤 엑세스 채널 4A B(frequency position, time period, timing
offset), 프리앰블 VW, 초기 프리앰블의 AS 전력 등의 AHS 획득한다. 그 후, 단말은
사용 가능한 채널과 프리앰블 시퀸스 중에서 한 채널과 하나의 시퀸스를 무작위로 선택
한다. 또한, 상위계층으로부터 PS 정보를 이용하여 초기 프리앰블 전송 전력과 최대
재전송 횟수를 설정한다. 단말은 선택한 채널, 시퀸스, 전송 전력으로 비동기 랜덤 엑세
스를 시작한다.

3GPP LTES] 동기 랜덤 엑세스에서는 다른 단말로부터 전송되는 상향링크 신호와의
AL 내에서 SSH 인한 지연을 줄이기 위하여 비경쟁ㅁ00ㅁ-000[600020) 기반으로 진행된
다. 즉, 단말이 랜덤 엑세스 프리앰블을 전송하기 전에 기지국에서 단말에게 PRACHS
할당하고, 단말은 고유하게 지정된 PRACHS 사용하여 랜덤 ANAS 함으로써 SSS

3GPP Ｌ7ㅠ에서는 타이밍 조정 명령어(110108 Advance)S 이용하여 각 단말의 송수
타이밍을 제어함으로써 각 단말이 전송하는 상향링크 신호가 기지국에 동시에 eases
한다. 상향링크 동기가 유지중인 단말은 위의 타이밍 조정에 의하여 타이밍 제어를 하며,

동기를 잃은 단말은 PRACH 을 전송함으로써 동기 정보를 획득한다. OFDM 시스템에서
의 자세한 상향링크 동기화 절차 및 동기화 기법은 5.8.2절, 18.5.1절, 18.8.6절에서 기술

하였기 때문에 본 절에서는 생략한다,

_ 662



===== PAGE 679 =====
제19장_ 3666 LTE 시스템

(ADE 3606 ite 시스템의 MIMO 기법

3GPP Ｌ1ㅠ에서는 하향링크에서 100Mbps, 상향링크에서 5OMbps2] 전송속도를 목표로
  이와 같이 높은 전송속도를 달성하기 위해 MIMO 기술을 사용한다. 송-수신단에 다
중 안테나를 사용함으로써 독립적인 페이딩 채널을 다수 형성하여 다이버시티 이득 또는
멀티플렉싱 이득을 얻는 MIMO 방식이 사용된다. 3GPP LTE 시스템에 제안된 MIMO 기술
들은 크게 2가지로 나눌 수 있다. 송신부에서 채널상태정보 없이 다이버시티 또는 멀티플렉

4 이득을 얻는 ARE 방식과, 채널상태정보를 이용하여 ele 할당하거나 000000을 수

행하는 페루프 방식이 있다. 또한 다중사용자가 통신 자원을 공유하는 -\4140(\0481
MIMO) 또는 MU-MIMO(multi—user MIMO) 기법을 사용하여 셀 4>8(throughput)-& 향
상시킬 수 있다. 이러한 MIMO 기술을 사용하기 위하여 안테나 개수는 기지국과 단말기
모두 1.2 또는 4개까지 사용할 수 있다. MRE 방식 사용 시 송신단은 수신단으로부터 다

(1) RI(Rank Indicator) : 공간차원의 개수
(2) PMI(Precoding Matrix Indicator) : precoding 행렬의 인덱스
(3) CQI(Channel Quality Indicator) : 채널의 상태 정보

이러한 정보를 이용하여 SAIS layer 맵핑, precoding, CDD, SFBC2] 사용 여부를
결정한다. 그림 19.172 3GPP LTE 송신부의 BEES 보여준다.

Codeword                     Layers                                                      Antenna
ports

그림 19.17 3GPP LTE 송신부의 MIMO 기술

6936 Layer 맵핑
QAM 변조된 심볼들의 layer YY 방식은 코드워드의 종류에 따라 3가지로 분류할 수
있다.



===== PAGE 680 =====
PART IV_MIMO-OFDM 통신 시스템

(1) Blast(Single CodeWord; SCW): 한 개의 코드워드로 이루어진 데이터를 공
로 분리한다. 단일 코드워드이기 때문에 작은 오버헤드를 필요로 하지만, 수신부에서
채널 복호기와 신호검출기법의 효과적인 결합이 어렵다.

(2) PARC(Per Antenna Rate Control) (Multi-CodeWord; MCW): 다수 개의 코드워드들
이 각기 다른 10하로 맵핑되는 방식이다. 수신부에서 채널 복호기와 신호 검출기법,
특히 510 기법과 성공적인 결합이 가능하나, 코드워드 개수만큼의 정보를 처리해야
하기 때문에 오버헤드가 커지는 단점이 있다.

(3) PGRC(Per Group Rate Control): 185@의 개수에 따라 다음과 같이 맵핑을 수행하며,
최대 두 개의 코드워드를 사용한다.

@) Rank 1:
(2) Rank 2:

10
-lo

JE 1 — layer 1

10
+o

비드 1 — layer 1
|= 2 — layer 2

|
+o

(3) Rank 3:     1 1 = layer 1
\= 2 — layer 22} 3
-J= 1 — layer 12} 2

워드 2 — layer 39} 4

+

10
to

10
보이

(4) Rank 4:

pe ee eee

10

그림 19.18은 rank7} 3일 경우 PGRC 적용 시 블록도를 보여준다.

CQI feedback

그림 19.18 Rank 32! 경우의 공간 맵핑

공간 다중화 방식 사용시, 위의 PGRCS 적용하여 rankel] 따라 코드워드의 맵핑이 이
루어진다. 송신 다이버시티 기법 적용 시에는 90\를 사용하여 맵핑이 이루어진다.

684



===== PAGE 681 =====
제19장 3666 LTE 시스템

QCRPA Precoding 기법

일반적으로 AEE 설계 시 다음 사항들이 고려되어야 한다.

(1) Chordal distance 크게 한다.
(2) Precoding 수행시 연산복잡도를 낮게 한다.
(3) Precoding 으로 인하여 송신전력을 크게 증가시키지 않도록 한다.

위의 사항들을 고려하여 설계한 코드북 내에서 수신부는 가장 적합한 precoding 행렬을
선택하여 이에 해당하는 PMI, RIS 송신부로 1[(606080한다.
3GPP Ｌ1의 코드북은 4018 행렬로 이루어져 있거나 그 행렬의 열벡터로 이루어져
있고 layer2] 개수에 따라 세분화 된다. 표 19.7은 송신 안테나가 2개인 SPS 보여준다.
드북을 이루는 ayo) EAS ANH layer 개수가 2일 때는 단위행렬, DFT 행렬,
we  만큼 회전된 DFT 행렬로 이루어져 YOu, layer 개수가 1일 ASE 29 경우의 행렬
이루는 열 벡터로 구성된다.
안테나가 4개일 경우는 20 1,2,3,47} 가능하고 각 rankel] 대해 16개의 precoding

at

"ah |

# 19.7 Nr=29l 경우의 FES

ie ik
Nn —  a
| —  씨 Lae
~.

| Eee

685


===== PAGE 682 =====
PART IV_MIMO-OFDM 통신 시스템

Bao] 존재한다. 3GPP LTESA|= precoding YAS 생성하기 위해 다음의 Householder
reflection 행렬을 사용한다.

W, =1-2u,u,” /|u, |)                                 (19.14)

벡터 U, 는 표 19.80] 주어져 있다. 이 표에서 WS 0,을 이용하여 구성한 행렬 중
첫 번째 열 벡터를 의미한다.

표 19.8 송신안테나가 4개인 경우의 precoding FES

0        리트 이기       Wo”  wi V2 Wo WP
aL        a,=(1 <j <1 97      w  wi? V2 W813 we /2
2        uw, =[1 1 그 1      We wR Whe ow 72
3       u,=[1 ¢ -1 기      WP Wy OWS ON 2
4 w=[1 Cl-piv2 -7 0-2/62] WP Wha wi wi /2
5   us=[1 -p/v2 7 Cl-piv2P WP WSPN2 wi ws 12
6 oug=[1 + p/v2 -7 (64076 | WE WEP 2 WEP wi /2
7   uy =[1 (77012 7 dt aiv2P WWE wi 1/3 wi 12
8        비그 0      We OWE 2 WE owe
9       wal ay oy      WP wh 2 wis woP” 72
10        weet bap      We WH WEE Whe
Jul       때 = f=      wo  we /J2 we //3 wo /2
12       u,=[1 -1 -1 1]      \ Wel WP NE
13       u,=[1 -1 1-1]      We We a We ee
14       u,=[1 1 -1 -1}'      Ww,  wo /J2 wi (3 Wee 2
15        (eSena iy      we  wo? //2 we? 3 wi) /2

686



===== PAGE 683 =====
제19장 SGPP LTE 시스템

19.4.3 ㅁㅁ 기법

3GPP Ｌ1에서는 각 안테나마다 CDD(Cyclic Delay Diversity)& 사용한다. 이는
IEEE 802.111에서 사용되는 기법과 동일하며, 15.3절에서 이에 대한 내용을 설명하였다.
CDD= 지연시간의 양에 따라 0, 큰 지연으로 구분되며 앞 AS} precoding} 결합되어 A}
용된다.                                                    |

(1) 0 지연(2600 delay): CDDS 사용하지 않고, precodingyt 사용하여 전송하는 방식으로

입출력신호는 다음과 같이 표현된다. 여기서, WE precoding 행렬이고, P = layer
맵핑 행렬이다.
y =HWPs+z                           (19.15)
(2) 2 순환 지연(1486 cyclic delay): 이동성이 =          우에 사용하는 기법으로 주파수 A
택성을 크게 증가시킨다. 따라서 채널    부호화와 cleje ol 의한 이득이 더욱  =
A 된다. 입출력 ASS] 관계는 식 (19.17)에 주어져 있                등
더욱 높이기 위한 40187 행렬이다.
y = HDUWPs +z                         (19.16)
# 19.9 CDD 행렬 (large delay)
U         |                D
[1]                        [1]
1    1                     1   0
1 ei?                   i  a
1    1      1               1    0     0
1  ei  i473             0  e 72008  0
1 e i488 |, 80             0    0 ems
1    1      1      1         1    0     0      0
{ert gles , , /애       0 208    0      0
1 , 8 281 ao 1201      0    0    eal    0
1 67799 20 2 16      0    0      0    27694

687



===== PAGE 684 =====
PART IV_MIMO-OFDM 통신 시스템

0 행렬과 1 행렬은 185@의 개수에 따라 표 19.9로부터 선택된다.

Ae SFBC 7/4

채널의 시변 정도가 커서 연속된 OFDM 심볼 사이의 채널이 변하는 경우에는 9180 4
용이 어렵다. 이 때 채널의 주파수 선택적 특성이 크지 않아 인접 부채널간의 채널 주파수
응답이 유사한 경우에는 부호화가 주파수영역에서 이루어지는 SFBC(Space—Frequency
Block Code) 기법을 사용할 수 있다. 3GPP Ｌ1에서의 SFBCE 인접 부채널에 Alamouti
부호를 적용하여 다이버시티 - 을 얻는다. 송신 안테나가 2개인 경우에는 SFBCS 사용
하고, 송신 안테나가 4개인 경우에는 SFBC2} FSTD(Frequency Switched Transmit
Diversity)S 사용한다.

# 19.10 SFBC 부호화

d(4i) — d (47+1)          0                0

d©(2i) a (2741)                -d(4i+1)  d (4i)               0                     0
-d)(2i+1) — d (24)                           0                    0             d(4i+2)  d (41 +3)
0                     0           -d(4i+3) (4142)

. 00898 Virtual MIMO 기법

2개 이상의 송신 안테나를 이동 단말기에 구현하기 위해서는 단말기 크기의 문제뿐만
아니라 송신 안테나 수에 비례하여 추가적인 소모 전력의 비용이 소요 된다. 이를 해결하
는 한 가지 방안으로써, 하나의 송신 안테나를 가지는 여러 사용자에게 동일한 자원을 할

당하여 전송함으로써 여러 사용자와 기지국 간에 가상의 MIMO 채널을 구성할 수 있으며
이를 0481 MIMOz}32 한다. V-MIMO* LTEo]A] \00-40040라고도 한다.

그림 19.19는 하나의 송신 안테나를 가진 두 단말과 두 개의 수신 안테나를 가진 기지
국으로 구성된 2x2 V-MIMOS 나타낸다. 두 단말이 동시에 같은 주파수 대역으로 데이
터를 전송하므로 WIS 발생하지만, 기지국에서 적절한 MIMO 수신기를 사용함으로써
두 단말로부터의 ASS 분리할 수 있다. 이 경우 단말기는 하나의 송신 안테나만을 가지

구

688



===== PAGE 685 =====
제19장 3GPP LTE 시스템

V-MIMO

그림 19.19 Virtual MIMO 기

rf

고 다른 단말에서의 신호와 무관하게 자신만의 데이터를 전송하기 때문에 복잡도는
SIMO 단말기와 같게 되고 전력 소모, 크기, 가격 면에서 효율적이다. Virtual MIMO 기
법에 대해서는 14장에서 자세히 기술하였기 때문에 본 절에서는 생략한다.



===== PAGE 686 =====
MIMO-OFDM 무선 통신과 MATLAB

참고문현

[1] B. Sklar, Digital Communications: Fundamentals and Applications 2/E., Prentice Hall, 2002.

[2] T.S. Rappaport, Wireless Communications: Principles and Practice 2/E., Prentice Hall,
2001.

[3] D. Greenwood and L. Hanzo, “Characterization of mobile radio channels,” Mobile Radio
Communications, edited by R. Steele, Chapter 2, Pentech Press, London, 1994.

[4] H.T. Friis, “A note on a simple transmission formula,” Proc. JRE, vol. 34, no. 5, pp.
254-256, May 1946.

[5] W.C.Y. Lee, Mobile Communications Engineering, McGraw Hill, New York, 1985.

[이 Y. Okumura, E. Ohmori, T. Kawano, and K. Fukuda, “Field strength and its variability in
VHF and UHF land mobile radio service,’ Review of the Electrical Communication
Laboratory, 16, pp. 825-873, Sep./Oct. 1968.

[7] M. Hata, “Empirical formula for propagation loss in land mobile radio servies,” [EEE
Trans. Veh. Technol., vol. 29, no. 3, pp. 317-325, Aug. 1980.

[8] V. Erceg, L.J. Greenstein, S.Y. Tjandra, S.R. Parkoff, A. Gupta, B. Kulic, A.A. Julius,
and R. Bianchi, “An empirically based path loss model for wireless channels in suburban
environments,” JEEE J. Select. Areas Commun., vol. 17, no. 7, pp. 1205-1211. July 1999.

[9] IEEE 802.16j-06/013r3, “Multi-hop relay system evaluation methodology (channel model
and performance metric),” Feb. 2007.

[10] IEEE 802.16.3c-01/29r4, “Channel models for fixed wireless applications,” July 2001.

[11] IST-4-027756 WINNER II, D/.J.1 WINNER II Interim Channel Models, July 2004.

[12] R.H. Clarke, “A statistical theory of mobile radio reception,” Bell Systems Technical

Journal, 47, pp. 987-1000, 1968.
[13] LR. Capoglu, Y. Li, and A. Swami, “Effect of doppler spread in OFDM based UWB
systems,” JEEE Trans. Wireless Commun., vol. 4, no. 5, pp. 2559-2567, Sep. 2005.
[14] G.L. Stuber, Principles of Mobile Communication, Kluwer Academic Publishers, 1996.

[15] C. Tepedelenliglu and G.B. Giannakis, “On velocity estimation and correlation properties

690



===== PAGE 687 =====
[16]
[17]

[18]

[19]

[22]

[23]

[24]

[25]

[26]
[27]

[28]

a
ki
Ao
rat

of narrow-band mobile communicatio channels,” JEEE Trans. Veh. Technol., vol. 50, no.
4, pp. 1039-1052, July 2001.

A.S. Akki and F. Haber, “A statistical model of mobile-to—mobile land communication
channel,” JEEE Trans. Veh. Technol., vol. 35, no. 1, pp. 2-7, Feb. 1986.

A.S. Akki, “Statistical properties of mobile-to—mobile land communication channels,”
IEEE Trans. Veh. Technol., vol. 43, no. 4, pp. 826-831, Nov. 1994.

J.B. Andersen, T.S. Rappaport, and S. Yoshida, “Propagation measurements and models
for wireless communications channels,” JEEE Commun. Mag., vol. 33, no. 1, pp. 42-49,
Jan. 1995.

A.S. Bajwa and J.D. Parsons, “Small-area characterisation of UHF urban and suburban
mobile radio propagation,” Inst. Elec. Eng. Proc., vol. 129, no. 2, pp. 102-109, Apr.
1982.

P.A. Bello, “Characterization of randomly time-variant linear channels,” JEEE Trans.
Commun., vol. 11, no. 4, pp. 360-393, Dec. 1963.

D.M. Black and D.O. Reudink, “Some characteristics of mobile radio propagation at 836
MHz in the Philadelphia area,” JEEE Trans. Veh. Technol., vol. 21, no. 2, pp. 45-51,
Feb. 1972.

G.E. Corazza and F. Vatalaro, “A statistical model for land mobile satellite channels and
its application to nongeostationary orbit systems systems,” JEEE Trans. Veh. Technol.,
vol. 43, no. 3, pp. 738-742, Aug. 1994.

COST 207, “Digital land mobile radio communications,” Office for Official Publications
of the European Communities, Final Report, Luxembourg, 1989.

B.H. Fleury and P.E. Leuthold, “Radiowave propagation in mobile communications: An
overview of European research,” JEEE Commun. Mag., vol. 34, no. 2, pp. 70-81, Feb.
1996.

L.J. Greenstein, “A multipath fading channel model for terrestrial digital radio systems,”
IEEE Trans. Commun., vol. 26, no. 8, pp. 1247-1250, 1978.

W.C. Jakes, Microwave Mobile Communications, John Wiley & Sons, New York, 1974.
C. Loo, “A statistical model for a land mobile satellite link,’ JEEE Trans. Veh. Technol.,
vol. 34, no. 3, pp. 122-127, Aug. 1985.

E. Lutz and E. Plochinger, “Generating Rice processes with given spectral properties,”
IEEE Trans. Veh. Technol., vol. 34, no. 4, pp. 178-181, Nov. 1985.

691



===== PAGE 688 =====
MIMO-OFDM 무선 통신과 MATLAB

[29] Recommendation ITR-R M.1225, Guidelines for Evaluation of Radio Transmission
Technologies for IMT-2000, 1997.

[30] D.L. Schilling, et. al, “Broadband CDMA for personal communications systems,” JEEE
Commun. Mag., vol. 29, no. 11, pp. 86-93, Nov. 1991.

[31] S.Y, Seidel, et. al, “Path loss, scattering and multipath delay statistics in four european
cities for digital celluarl and microcellular radiotelephone.” JEEE Trans. Veh. Technol.,
vol. 40, no. 4, pp. 721-730, Nov. 1991.

[32] S. Stein, “Fading channel issues in system engineering,” JEEE J. Select. Areas Commun.,
vol. 5, no. 2, pp. 68-89, Feb. 1987.

[33] W.J. Vogel and J. Goldhirsh, “Multipath fading at L band for low elevation angle, land
mobile satellite scenarios,” JEEE J. Select. Areas Commun., vol. 13, no. 2, pp. 197-204,
Feb. 1995.

[34] Y. Xie and Y. Fang, “A general statistical channel model for mobile satellite systems,”
IEEE Trans. Veh. Technol., vol. 49, no. 3, pp. 744-752, May 2000.

[35] N. Youssef, T. Munakata, and M. Takeda, “Fade statistics in Nakagami fading
environments,” in Proc. IEEE 4th Int. Symp. on Spread Spectrum Techniques &
Applications, Mayence, Germany, vol. 3, pp. 1244-1247, Sep. 1996.

[36] IEEE P802.11-97/96, “Tentative criteria for comparison of modulation methods,” 1996.

[37] A.M. Saleh and R.A. Valenzuela, “A Statistical model for indoor multipath propagation,”
IEEE J. Select. Areas Commun., vol. 5, no. 2, pp. 128-137, Feb. 1987.

[38] IEEE 802.15-02/144, “UWB channel modeling contribution from CEA-LETI and
STMicroelectronics,” Nov. 2002.

[39] J.I. Smith, ““A computer generated multipath fading simulatio for mobile radio,” JEEE
Trans. Veh. Technol., vol. 24, no. 3, pp. 39-40, Aug. 1975.

[40] 3GPP, “3rd Generation Partnership Project; technical specification group radio access
network; spatial channel model for multiple Input multiple mutput simulations (Release
7),” TR 25.996, v7.0.0, June 2007. |

[41] J.G. Wang, A.S. Mohan, and T.A. Aubrey, “Angles-of-Arriaval of multipath signals in
infoor environments,” JEEE VTC’96, pp. 155-159, 1996.

[42] K. Pedersen, P. Mogensen, and B. Fleury, “Spatial channel characteristics in outdoor
environments and their impact on BS antenna system performance,” JEEE VTC’9S, pp.

719-723, Ottawa, Canada, May 1998.

692



===== PAGE 689 =====
o%
kl
Ho
ra

[43] M. Nilsson, B. Lindmark, M. Ahlberg, M. Larsson, and C. Beckman, “Characterization of
a wideband radio channel using spatio-temporal polarization measurements,” P/MRC’99,
pp. 1278-1283, Sep. 1998.

[44] P.C.F. Eggers, “Angular dispersive mobile radio environments sensed by highly directive
base station antannas,” PIMRC’95, pp. 552-526, Sep. 1995.

[45] U. Martin, “Spatio-temporalradio channel characteristics in urban macrocells,’ JEEE
Proceedings on Radar, Sonar and Navigation, vol. 145, no. 1. pp. 42-49, Feb. 1998.
[46] M. Pettersen, P.H. Lehne, J. Noll, O. Rostbakken, E. Antonsen, and R. Eckhoff,
“Characteristics of the deirectional wideband radio channel in urban and suburban areas,”

IEEE VTC’99, pp. 1454-1459, Amsterdam, Netherlands, Sep. 1999.

[47] K. Kalliola and P. Vainikainen, “Dynamic wideband measurement of mobile radio
channel with adaptive antennas,” JEEE VTC’98, pp. 21-25, Ottawa, Canada, May 1998.

[48] P. Pajusco, “Experimental characterization of DoA at the base station in rural and urban
area.” IEEE VTC’98, pp. 993-997, Ottawa, Canada, May 1998.

[49] Q. Spencer, B. Jeffs, M. Jensen, and A.L. Swindlehurst, ” Modeling the statistical time
and angle of arrival characteristics of an indoor multipath channel,” JEEE J. Select.
Areas Commun., vol. 18, no. 3, pp. 347-360, Mar. 2000.

[50] W. Lee, “Effect on correlation between two mobile radio base-station antennas,” [EEE
Trans. Commun., vol. 21, no. 11, pp. 1214-1224, Nov. 1973.

[51] L. Schumacher, K.I. Pedersen, and P.E. Mogensen, “From antenna spacings to theoretical
capacities~guidelines for simulating MIMO systems,” PIMRC’02, vol. 2, pp. 587-592,
Sep. 2002.

[52] IST-METRA project, [Online] Available: http:/www.ist-imetra.org.

[53] 3GPP, “3rd generation partnership project; technical specification group radio access
network; physical layer aspects for evolved UTRA (Release 7).” TR 25.814 V1.2.2 Apr.
2006.

[54] Available: http://legacy.tkk.fi/Units/Radio/scm/

[55] D.S. Baum, J. Salo, G. Del Galdo, M. Milojevic, P. Kyosti, and J. Hansen, “An interim
channel model for beyond-3G systems,” JEEE VTC’05, Stochholm, vol. 5, pp.
3132-3136, May 2005.

[56] C.C. Chong, C.M. Tan, D.I. Laurenson, 9. McLaughlin, M.A. Beach, and A.R. Nix, “A
new statistical wideband spatio-temporal channel model for 5 GHz band WLAN

693


===== PAGE 690 =====
MIMO-OFDM 무선 통신과 MATLAB

[57]

[58]

[59]

[60]

[61]

[62]

[63]

[64]

[66]

[67]

[68]
[69]

694

systems,” JEEE J. Select. Areas Commun., vol. 21, no. 2, pp. 139-150, Feb. 2003.

V. Erceg, L. Schumacher, P. Kyritsi, A. Molisch, and D.S. Baum et al., TGn Channel
Models, IEEE 802.11-03/940r2, Jan. 2004.

D.S. Baum, H. El-Sallabi, et al., Final Report on Link Level and System Level Channel
Models, WINNER Deliverable D5.4, Oct. 2005.

COST 231, “Urban transmission loss models for mobile radio in the 900- and 1800
MHz bands,” TD(90)119 Rev. 2, Sep. 1991.

T. Jamsa et al., “Multi-demensional radio channel measurement and modeling for future
mobile and short-range wireless systems,” /5th WWRF WG4 &WG5 white paper, Dec.
2005.

A. Karlsson, R.E. Schuh, C. Bergljung, P. Karlsson, and N. Lowendahl, “The influence
of trees on radio channels at frequencies of 3 and 5 GHz,” JEEE VTC’01, vol. 4, pp.
2008-2012, Oct. 2001.

N. Kita, A. Sato, and M. Umehira, “A path loss model with height variation in
residential area based on experimental and theoretical studies using a 5G/2G dual band
antenna,” IEEE VTC’00, vol. 2, pp. 840-844, Sep. 2000.

P. Kyosti, J. Meinila, et. al, WINNER II Interim Channel Models, WINNER Deliverable
D1.1.1, Nov. 2006.

A.J. Rustako, Jr., V. Erceg, R.S. Roman, T.M. Willis, and J. Ling, “Measurements of
microcellular propagation loss at 6 GHz and 2 GHz over NLOS paths in the city of
Boston,” IEEE GLOBECOM’95, vol. 1, pp. 758-763, Nov. 1995.

K. Yonezawa, T. Maeyama, H. Iwai, and H. Harada, “Path loss measurement in 5 GHz
macro cellular systems and consideration of extending existing path loss prediction
methods,” WCNC’04, vol. 1, pp. 279-283, Mar. 2004.

X. Zhao, J. Kivinen, P. Vainikainen, and K. Skog, “Propagation characteristics for
wideband outdoor mobile communications at 5.3 GHz,” JEEE J. Select. Areas Commun.,
vol. 20, no. 3, pp. 507-514, Apr. 2002.

X. Zhao, T. Rautiainen, K. Kalliola, and P. Vainikainen, “Path Loss Models for Urban
Microcells at 5.3 GHz,” COST 273 TD(04)207, Duisburg, Germany, Sep. 2004.

S. Haykin, Communication Systems 4/E., Wiley, 2001.

H. Nyquist, “Certain topics in telegraph transmission theory,” Trans. AIEE, vol. 477,
pp.617-644, Apr. 1928.



===== PAGE 691 =====
i
ki
Ao
rah

[70] G.L. Turin, “An introduction to matched filters,” ZEEE Trans. Info. Theory, 1960.

[71] A. Goldsmith, Wireless Communications, Cambridge Univ. Press, 2005.

[72] J.A.C. Bingham, “Multi-carrier modulation for data transmission: an idea whose time has
come,” JEEE Commun. Mag., vol. 28, no. 5, pp. 17-25, Mar. 1990.

[73] R.W. Chang, “Synthesis of band-limited orthogonal signals for multi-channel data
transmission,” Bell System Technical Journal, vol. 46, pp. 1775-1796, Dec. 1966.

[74] P.P. Vaidyanathan, Multi-rate System and Filter Banks, Prentice Hall, 1993.

[75] B.R. Saltzberg, “Performance of an efficient parallel data transmission system,” JEEE
Trans. Commun., Technol., vol. COM-15, pp. 805-811, Dec. 1967.

[76] S.B. Weinstein, “Data transmission by frequency division multiplexing using the discrete
fourier transform,” [EEE Trans. Commun. Technol., vol. COM-19, no. 5, pp. 628-634,
Oct. 1971.

[77] J.A.C. Bingham, ADSL, VDSL, and Multicarrier Modulation, Wiley, 2000.

[78] A. Peled, “Frequency domain data transmission using reduced computational complexity
algorithms,” JEEE ICASSP, vol. 5, pp. 964-967, 1980.

[79] G. Cherubini, “Filter bank modulation techniques for very high-speed digital subscriber
lines,” JEEE Commun. Mag., vol. 38, no. 5, pp. 98-104, May 2000.

[80] V. Lottici, “Blind carrier frequency tracking for filter bank multicarrier wireless
communications,” JEEE Trans. Commun., vol. 53, no. 10, pp. 1762-1772, Oct. 2005.

[81] S.D. Sandberg, “Overlapped discrete multi-tone modulation for high speed copper wire
communications,” JEEE J. Select. Areas Commun., vol. 13, no. 9, pp. 1571-1585, Dec.
1995.

[82] 3GPP TSG-RAN-1 Meeting #31, “Technical description of the OFDM/ IOTA
modulation,” Feb. 2003.

[83] M. Alard and R. Lassalle, “Principles of modulation and channel coding for digital
broadcasting for mobile receivers,” EBU Tech. Review, no. 24, pp. 3-25, Aug. 1987.

[84] H. Sari, G. Karam, and I. Jeanclaude, “Transmission techniques for digital terrestrial TV
broadcasting,” IEEE Commun. Mag., vol. 33, no 2, pp. 100-109, Feb. 1995.

[85] D.G. Mestdagh, et. al, “Zipper VDSL: a solution for robust duplex communication over
telephone lines”, JEEE Commun. Mag., vol. 38, no 5, pp. 90-96, May 2000.

[86] W. Alliance, Multiband OFDM Physical Layer Specification, Release 1.2, Feb. 2007.

[87] J.G. Proakis, Digital Communications 5/E., McGraw-Hill, New York, 2008.

695



===== PAGE 692 =====
MIMO-OFDM 무선 통신과 MATLAB

[88]

[89]

[90]

[91]

[92]

[93]

[94]

[95]

[96]

[97]

[98]

[99]

P.S. Chow, J.M. Cioffi, and J.A.C. Bingham, “A practical discrete multitone transceiver
loading algorithm for data transmission over spectrally shaped channels,” JEEE Trans.
Commun., vol. 43, no. 234, pp. 773-775, Feb./Apr. 1995.

B.S. Krongold, K. Ramchandran, and D.L. Jones, “Computationally efficient optimal
power allocation algorithm for multicarrier communication systems,” JEEE ICC’98, vol.
2, pp. 1018-1022, June 1998.

I. Kalet, “The multitone channel,” JEEE Trans. Commun., vol. 37, no. 2, pp. 119-124,
Feb. 1989.

T.J. Willink and P.H. Witteke, “Optimization and performance evaluation of multicarrier
transmission,” JEEE Trans. Commun., vol. 43, no 2, pp. 426-440, Mar. 1997.

A. Czylwik, “Adaptive OFDM for wideband radio channels,” JEEE GLOBECOM’96, vol
1, pp. 713-718, Nov. 1996.

S.K. Lai, R.S. Cheng, K.B. Letaief, and C.Y. Tsui, “Adaptive tracking of optimal bit and
power allocation for OFDM systems in time-varying channels,” JEEE Wireless Commun.
and Networking Conf., vol. 2, pp. 776-780, Sep. 1999.

T. Pollet, M. van Bladel, and M. Moeneclaey, “BER sensitivity of OFDM systems to
carrier frequency offset and wiener phase noise,” JEEE Trans. on Commun., vol. 43, no.
2/3/4, pp. 191-193, Feb./Apr. 1995.

M. Pauli, and H.P. Kuchenbecker, “Minimization of the intermodulation distortion of a
nonlinearly amplified OFDM signal,” Wireless Personal Commun., vol. 4, no. 1, pp.
93-101, Jan. 1997.

C. Rapp, “Effects of HPA-nonlinearity on a 4-DPSK/OFDM signal for a digital sound
broadcasting signal,” Proc. of the Second European Conf. on Satellite Commun.,
N92-15210 06-32, pp. 179-184, Oct. 1991.

H. Rohling and R. Grunheid, “Performance comparison of different multiple access
scheme for the downlink of an OFDM communication system,” JEEE VTC’97, pp. vol. 3,
1365-1369, May. 1997.

S. Hara and R. Prasad, “Overview of multicarrier CDMA,” JEEE Commun. Mag., vol.
35, no. 12, pp. 126-133, Dec. 1997.

IEEE 802.16e-2005, Part 16: Air Interface for Fixed and Mobile Broadband Wireless
Access Systems, Dec. 2005.

[100] C. Muschallik, “Influence of RF oscillator on an OFDM signal,” [EEE Trans. Consumer

_ 696



===== PAGE 693 =====
[에
로:
Ao
ra

Elect., vol. 41, no. 3, Aug. 1995.

[101] T. Pollet and M. Moeneclaey, “Synchronizability of OFDM signals,” JEEE GLOBE-
COM’95, pp. 2054-2058, Nov. 1995.

[102] L. Tomba, “On the effect of Wiener phase noise in OFDM systems,” JEEE Trans.
Commun., vol. 46, no. 5, pp. 580-583, Nov. 1998.

[103] H. Minn, M. Zeng, and V.K. Bhargava, “On timing offset estimation for OFDM
systems,” JEEE Trans. Commun., vol. 4, pp. 242-244, July 2000.

[104] P.J. Tourtier, R. Monnier, and P. Lopez, “Multicarrier modem for digital HDTV
terrestrial broadcasting,” Signal Processing, pp. 379-403, Dec. 1993.

[105] M. Speth, F. Classen, and H. Meyr, “Frame synchronization of OFDM systems in
frequency selective fading channels,” JEEE VTC’97, pp. 1807-1811, May 1997.

[106] J.J. Van de Beek, M, Sandell, M. Isaksson, and P.O. Bérjesson, “Low-complex frame
synchronization in OFDM systems,” JEEE ICUPC, pp. 982-986, Nov. 1995.

[107] J.J. Van de Beek, M. Sandell, and P.O. Bérjesson, “ML estimation of time and
frequency offset in OFDM systems,” JEEE Trans. Commun., vol. 45, no. 7, pp.
1800-1805, July 1997.

[108] T.M. Schmid] and D.C. Cox, “Low-overhead, low-complexity burst synchronization for
OFDM,” JEEE ICC’96, pp. 1301-1306, June 1996.

[109] T.M. Schmidl and D.C. Cox, “Robust frequency and timing synchronization for OFDM,”
IEEE Trans. Commun., vol. 45, no. 12, pp. 1613-1621, Dec. 1997.

[110] K. Taura, M. Tsujishta, M. Takeda, H. Kato, M. Ishida, and Y. Ishida, “A digital audio
broadcasting(DAB) receiver”, JEEE Trans. Consumer Electronics, vol. 42, no. 3, pp.
322-326, Aug. 1996.

[111] F. Daffara and O. Adami, “A new frequency detector for orthogonal multi-carrier
transmission techniques,” IEEE VTC’95, pp. 804-809, July 1995.

[112] P.H. Moose, “A technique for orthogonal frequency division mutiplexing frequency
offset correction,” ZEEE Trans. Commun., vol. 42, pp. 2908-2914, Oct. 1994.

[113] F. Classen and H. Myer, “Frequency synchronization algorithm for OFDM systems
suitable for communication over frequency selective fading channels,” JEEE VTC’94,
pp. 1655-1659, June 1994.

[114] B. Yang, K.B. Letaief, R.S. Cheng, and Z. Cao, “Timing recovery for OFDM trans-

mission,” JEEE Journal on Selected Areas in Commun., vol. 18, no. 11, Nov. 2000.

697



===== PAGE 694 =====
MIMO-—OFDM 무선 통신과 MATLAB

[115] M. Speth, D. Daecke, and H. Meyr, “Minimum overhead burst synchronization for
OFDM based broadcasting transmission,” JEEE GLOBECOM’98, pp. 3227-3232, 1998.

[116] T. Pollet, P. Spruyt, and M. Moeneclaey, “The BER performance of OFDM systems
using non-synchronized sampling,” JEEE GLOBECOM’94, pp. 253-257, Nov. 1994.

[117] HJ. Zepernick and A. Finger, Pseudo Random Signal Processing, John Wiley & Sons,
2005.

[118] K.S. Kim, S.W. Kim, Y.S. Cho, and J.Y. Ahn, “Synchronization and cell search
technique using preamble for OFDM cellular systems,” JEEE Trans. Veh. Tech., vol. 56,
no. 6, pp. 3469-3485, Nov. 2007.

[119] IEEE Std 802.16e, JEEE Standard for Local and Metropolitan Area Networks Part 16,
Feb. 2006.

[120] E. Dahlman, S. Parkvall, J. Skold, and P. Beming, 3G Evolution: HSPA and LTE for
Mobile Broadband, Acacdemic Press, 2007.

[121] Y. Tsai, G. Zhang, D. Grieco, F. Ozulturk, and X. Wang, “Cell search in 3GPP long
term evolution systems,” JEEE Trans. Vehicular Techno., June 2007.

[122] H. Nogami and T. Nagashima, “A frequency and timing period acquisition technique for
OFDM systems,” JEEE PIMRC, pp. 1010-1015, Sep. 1995.

[123] M. Schilpp, W. S-Greff, W. Rupprecht, and E. Bogenfeld, “Influence of oscillator phase
noise and clipping on OFDM for terrestrial broadcasting of digital HDTV,” JEEE
ICC’95, pp. 1678-1682, June 1995.

[124] H.K. Song, Y.H. You, J.H. Paik, and Y.S. Cho, “Frequency-offset synchronization and
channel estimation for OFDM-based transmission,’ JEEE Trans. Commun., vol. 4, no.
3, pp. 95-97, Mar. 2000.

[125] W.D. Warner and C. Leung, “OFDM/FM Frame synchronization for mobile radio data
communication,” JEEE Trans. Veh. Technol., vol. 42, no. 3, pp. 302-313, Aug. 1993.

[126] L.J. Cimini, “Analysis and simulation of a digital mobile channel using orthogonal

frequency—division multiplexing,” JEEE Trans. Commun., vol. 33, no. 7, pp. 665-675,

July 1985.

F. Tufvesson and T. Maseng, “Pilot assisted channel estimation for OFDM in mobile

cellular systems,” JEEE VTC’97, vol. 3, pp. 1639-1643, May 1997.

J.J. van de Beek, O. Edfors, M. Sandell, 9. K. Wilson, and P. 0. Borjesson, “On

channel estimation in OFDM systems,” JEEE VTC’95, vol. 2, pp. 815-819, July 1995.



===== PAGE 695 =====
[129]

[130]

[131]

[132]

[133]

[134]

[135]

[136]

[137]

[138]

[139]

[140]

[141]

ad
a)
Ho
[위

S. Coleri, M. Ergen, A. Puri, and A. Bahai, “Channel estimation techniques based on
pilot arrangement in OFDM systems,” JEEE Trans. on Broadcasting, vol. 48, no. 3, pp.
223-229, Sep. 2002.

J. Heiskala and J. Terry, OFDM Wireless LANs: A Theoretical and Practical Guide,
SAMS, 2002.

M. Hsieh and C. Wei, “Channel estimation for OFDM systems based on comb-type
pilot arrangement in frequency selective fading channels,” JEEE Trans. Consumer
Electron., vol. 44, no. 1, Feb. 1998.

R. van Nee and R. Prasad, OFDM for wireless multimedia communications, Artech
House Publishers, 2000.

H.K. Lau and S.W. Cheung, “A pilot symbol-aided technique used for digital signals in
multipath environments,” JEEE ICC’94, vol. 2, pp. 1126-1130, May 1994.

W.Y. Yang, W. Cao, T.S. Chung, and J. Morris, Applied Numerical Methods Using
MATLAB, Wiley Inter-Science, 2005.

R.J. Lyman and W.W. Edmonson, “Decision-directed tracking of fading channels using
linear prediction of the fading envelope,” 33rd Asilomar Conference on Signal
Processing, Systems, and Computers, vol. 2, pp. 1154-1158, 1999.

J.J. Ran, R. Grunbeid, H. Rohling, E. Bolinth, and R. Kern, “Decision—-directed channel
estimation method for OFDM systems with high velocities,’ JEEE VTC’03, vol. 4, pp.
2358-2361, Apr. 2003.

D. Xinmin, A.M. Haimovich, and J. Garcia—Frias, “Decision—-directed iterative channel
estimation for MIMO systems,” JEEE I[CC’03, vol. 4, pp. 2326-2329, May 2003.

H. Minn and V.K. Bhargava, “An investigation into time-domain approach for OFDM
channel estimation,” JEEE Trans. on Broadcasting, vol. 45, no. 4, pp. 400-209, Dec.
1999.

M.J. Fernandez-Getino Garcia, J.M. Paez-Borrallo, and S. Zazo, “DFT-based channel
estimation in 2D-pilot-symbol-aided OFDM wireless systems,” JEEE VTC’01, vol. 2,
pp. 810-814, May 2001.

J.J. van de Beek, O. Edfors, M. Sandell, S.K. Wilson, and P.O. Borjesson, “Analysis of
DFT-based channel estimators for OFDM,” Personal Wireless Commun., vol. 12, no. 1,
pp. 55-70, Jan. 2000.

Y. Zhao and A. Huang, “A novel channel estimation method for OFDM mobile

699


===== PAGE 696 =====
MIMO—OFDM 무선 통신과 MATLAB

communication systems based on pilot signals and transform-domain processing,” JEEE
VTC’98, vol. 46, pp. 931-939, May 1998.

[142] X. Daofeng and Y. Luxi, “Channel estimation for OFDM systems using superimposed
training,” International Conference in Central Asia on Internet, pp. 26-29, June 2004.

[143] P. Hoeher and F. Tufvesson, “Channel estimation with superimposed pilot sequence,”
IEEE GLOBECOM’99, pp. 2162-2166, 1999.

[144] Z. Ding and Y. Li, Blind Equalization and Identification, MARCEL DEKKER, 2001.

[145] D.N. Godard, “Self-recovering equalization and carrier tracking in two-dimensional data
communication systems,” JEEE Trans. Commun., vol. 28, no. 11, pp. 1867-1875, Nov.
1980.

[146] S. Haykin, Adaptive Filter Theory, 4th edition, PHIPE, 2001.

[147] Y. Sato, “A method of self-recovering equalization for multilevel amplitude-modulation
systems,” [EEE Trans. Commun., vol. 23, no. 6, pp. 679-682, June 1975.

[148] C. Shin and E.J. Power, “Blind channel estimation for MIMO-OFDM systems using
virtual carriers,” JEEE GLOBECOM’04, vol. 4, pp. 2465-2469, Nov. 2004.

[149] L. Tong, G. Xu and T. Kailath, “A new approach to blind identification and equalization
of multipath channel,” Proc. 25th Asilomar Conf. Signals, Systems, and Computers, CA,
vol. 2, pp. 856-860, Nov. 1991.

[150] R. Zhang, “Blind OFDM channel estimation through linear precoding: a subspace
approach” JEEE ACSSC, vol. 2, pp. 631-633, Nov. 2002.

[151] C.H. Aldana, E. Carvalho, and J.M. Cioffi, “Channel estimation for multicarrier multiple
input single output systems using the EM algorithm,” JEEE Trans. on Signal
Processing, vol. 51, no. 12, pp. 3280-3292, Dec. 2003.

[152] A.P. Dempster, N.M. Laird, and D.B. Rubin, “Maximum likelihood from incomplete
data via the EM algorithm,” Journal of the Royal Statistical Society, vol. 39, no. 1, pp.
1-38, 1977.

[153] K.I. Lee, K.S. Woo, J.K. Kim, J.-H. Yi, S.B. Yun, and Y.S. Cho, “Channel estimation for
OFDM based cellular systems using a DEM algorithm,” PIMRC’07, Athens, Sep. 2007.

[154] X. Ma, H. Kobayashi, and S.C. Schwartz, “EM-based channel estimation algorithms for
OFDM,” EURASIP Journal on Applied Signal Processing, pp. 1460-1477, 2004.

[155] T.K. Moon, “The expectation—maximization algorithm,” JEEE Signal Processing
Magazine, vol. 13, no. 6, pp. 47-60, Nov. 1996.

700



===== PAGE 697 =====
oO
니
Ao
rah

[156] X. Yongzhe and C.N. Georghiades, “Two EM-type channel estimation algorithms for
OFDM with transmitter diversity,’ JEEE Trans. on Commun., vol. 51, no. 1, pp.
106-115, Jan. 2003.

[157] D. Hu and L. Yang, “Time-varying channel estimation based on pilot tones in OFDM
systems,” JEEE Int. Conf: Neural Networks & Signal Processing, vol. 1, pp. 700-703,
Dec. 2003.

[158] W.G. Jeon, K.H. Chang, and Y.S. Cho, “An equalization technique for orthogonal
frequency~division multiplexing system in time-variant multipath channels,’ JEEE
Trans. Commun., vol. 47, no. 1, pp. 27-32, Jan. 1999.

[159] Y. Li, L.J. Cimini, Jr., and N.R. Sollenberger, “Robust channel estimation for OFDM
systems with rapid dispersive fading channels,’ JEEE Trans. on Commun., vol. 46, no.
7, pp. 902-915, July 1998.

[160] Z. Tang, R.C. Cannizzaro, G. Leus, and P. Banelli, “Pilot-assisted time-varying channel
estimation for OFDM systems,” JEEE Tran. Signal Processing, vol. 55, no. 5, pp.
2226-2238, May 2007.

[161] K.W. Park and Y.S. Cho, “An MIMO-OFDM technique for high-speed mobile
channels,” JEEE Commun. Letters, vol. 9, no. 7, pp. 604-606, July 2005.

[162] Y. Zhao and S.G. Haggman, “Intercarrier interference self-cancellation scheme for
OFDM mobile communication systems,” JEEE Tran. Commun., vol. 49, no. 7, pp.
1158-1191, July 2001.

[163] S. Litsyn, Peak Power Control in Multicarrier Communications, Cambridge Univ. Press,
2007.

[164] S.H. Han and J.H. Lee, “An overview of peak-to-average power ratio reduction
techniques for multicarrier transmission,” JEEE Wireless Commun., vol. 12, no. 2, pp.
56-65, Apr. 2005.

[165] J. Palicot and Y. Louét, “Power ratio definitions and analysis in single carrier
modulations,” EUS/PCO, Antalya, Turkey, Sep. 2005.

[166] H. Ochiai and H. Imai, “Block coding scheme based on complementary sequences for
multicarrier signals,” JEJCE Trans. Fundamentals, vol. E80-A, no. 11, pp. 2136-2143,
Noy. 1997.

[167] H. Ochiai and K. Imai, “On the distribution of the peak-to—average power ratio in
OFDM signals,” JEEE Trans. Commun., vol. 49, no. 2, pp. 282-289, Feb. 2001.

701


===== PAGE 698 =====
MIMO-OFDM 무선 통신과 MATLAB

[168] R. van Nee and A. de Wild, “Reducing the peak-to-average power ratio of OFDM,”
IEEE VTC’98, vol. 3, pp. 18-21, May 1998.

[169] H. Ochiai and K. Imai, “On clipping for peak power reduction of OFDM signals,”
IEEE GTC, vol. 2, pp. 731-735, Dec. 2000.

[170] E.C. Ifeachor and B.W. Jervis, Digital Signal Processing-a Practical Approach 2/E.,
Prentice Hall, 2002.

[171] D.C. Chu, “Polyphase codes with periodic correlation properties,” JEEE Trans. Info.
Theory, vol. 18, no. 4, pp. 531-532, July 1972.

[172] H.D. Like, H.D. Schotten, and H.H. Mahram, “Binary and quadriphase sequences with
optimal autocorrelation properties,” JEEE Trans. Info. Theory, vol. 49, no. 12, Dec. 2003

[173] S.B. Slimane, “Peak-to-average power ratio reduction of OFDM signals using pulse
shaping,” JEEE GTC, vol. 3, pp. 1412-1416, Dec. 2000.

[174] W.G. Jeon, K.H. Chang, and Y.S. Cho, "An adaptive data predistorter for compensation
of nonlinear distortion in OFDM systems," JEEE Trans. on Commun., vol. 45, No. 10,
pp. 1167-1171, Oct. 1997.

[175] X. Li and L. J. Cimini, “Effects of clipping and filtering on the performance of
OFDM,” JEEE Commun. Letter, vol. 2, no. 20, pp. 131-133, May 1998.

[176] T.A. Wilkinson and A.E. Jones, “Minimization of the peak-to-mean envelope power
ratio of multicarrier transmission scheme by block coding,” IEEE VTC’95, Chicago, vol.
2, pp. 825-829, July 1995.

[177] M.J.E. Golay, “Complementary series,’ JEEE Trans. Inf. Theory, vol. 7, no. 2, pp.
82-87, Apr. 1961.

[178] B.M. Popovic, “Synthesis of power efficient multitone signals with flat amplitude
spectrum,” JEEE Trans. Commun., vol. 39, no. 7, pp. 1031-1033, July 1991.

[179] R.D.J. van Nee, “OFDM codes for peak-to-average power reduction and error
correction,” JEEE GTC, London, vol. 2, pp. 740-744, Nov. 1996.

[180] J.A. Davis, and J. Jedwab, “Peak-to-mean power control in OFDM, Golay complementary
sequences, and Reed-Muller codes,” JEEE Trans. Info. Theory, vol. 45, no. 7, pp.
2397-2417, Nov. 1999.

[181] J.A. Davis, and J. Jedwab, “Peak-to-mean power control and error correction for
OFDM transmission using golay sequences and reed-muller codes,” Electronics Letters,
vol. 33, no. 4, pp. 267-268, 1997.

702



===== PAGE 699 =====
a
EI
Ho
rah

[182] R. Urbanke and A.S. Krishnakumar, “Compact description of Golay sequences and their
extensions,” Proc. of the Thirty-Fourth Annual Allerton Conference on Commun.,
Control and Computing Pagination, Urbana, IL, pp. 693-701, Oct, 1996.

[183] X. Li and J.A. Ritcey, “M-sequences for OFDM peak-to-average power ratio reduction
and error correction,” Electronics Letter, vol. 33, no. 7, pp. 554-555, Mar. 1997.

[184] C. Tellambura, “Use of m-sequences for OFDM peak-to-average power ratio reduction,”
Electronics Letters, vol. 33, no. 15, pp. 1300-1301, July 1997.

[185] M.H. Park, et. al, “PAPR reduction in OFDM transmission using hadamard transform,”
IEEE ICC’00, vol. 1, pp. 430-433, 2000.

[186] S.H. Muller, et. al, “OFDM with reduced peak-to—average power ratio by multiple signal
representation,” In Annals of Telecommun., vol. 52, no. 1-2, pp. 58-67, Feb., 1997.

[187] S.H. Muller and J.B. Huber, “OFDM with reduced peak-to-average power ratio by
optimum combination of partial transmit sequences,” Electronics Letters, vol. 32, no. 22,
pp. 2056-2057, Oct. 1996.

[188] R.W. Bauml, R.F.H. Fischer, and J.B. Huber, “Reducing the peak-to-average power
ratio of multicarrier modulation by selective mapping,” Electronics Letters, vol. 32, no.
22, pp. 2056-2057, Oct. 1996.

[189] N. Ohkubo and T. Ohtsuki, “Design criteria for phase sequences in selected mapping,”
IEEE VTC’03, vol. 1, pp. 373-377, Apr. 2003.

[190] S.H. Muller and J.B. Huber, “A novel peak power reduction scheme for OFDM,”
PIMRC'97, vol. 3, pp. 1090-1094, Sep. 1997.

[191] L.J. Cimini, Jr., “Peak-to-average power ratio reduction of an OFDM signal using partial
transmit sequences,” JEEE Commun. Letters, vol. 4, no. 3, pp. 86-88, Mar. 2000.
[192] C. Tellambura, “A coding technique for reducing peak-to-average power ratio in

OFDM,” JEEE GLOBECOM’98, vol. 5, pp. 2783-2787, 1998.

[193] J. Tellado-Mourelo, “Peak to average power reduction for multicarrier modulation,”
Ph.D. Dissertation, Stanford Univ., Sep. 1999.

[194] K. Bruninghaus and H. Rohling, “Multi-carrier spread spectrum and its relationship to
single-carrier transmission,” JEEE VTC’98., vol. 3, pp. 2329-2332, May 1998.

[195] D. Galda and H. Rohling, “A low complexity transmitter structure for OFDM-FDMA
uplink systems,” JEEE VTC’02, vol. 4, pp. 1737-1741, 2002.

[196] H.G. Myung, J. Lim, and D.J. Goodman, “Single carrier FDMA for uplink wireless

703



===== PAGE 700 =====
MIMO—-OFDM 무선 통신과 MATLAB

transmission,” JEEE Veh. Technol. Mag., vol. 1, no. 3, pp. 30-38, Sep. 2006.

[197] H.G. Myung, J. Lim, and D.J. Goodman, “Peak-to-average power ratio of single carrier
FDMA signals with pulse shaping,’ PJMRC’06, pp. 1-5, Sept. 2006.

[198] R1-050896, Qualcomm, “Description and simulations of interference management
technique for OFDMA based E-UTRA downlink evaluation,” 3GPP RAN WGI #42,
London, UK, Sep. 2005.

[199] R1-060298, Nokia, “Uplink inter cell interference mitigation and text proposal,” 3GPP
RAN WGI #44, Denver, USA, Feb. 2006.

[200] R1-051341, Samsung, “Flexible fractional frequency reuse approach,” 3GPP RAN WGI
#43, Seoul, Korea, Nov. 2005.

[201] L.J. Cimini, J.C. Chuang, and N.R. Sollenberger, “Advanced cellular internet service
(ACIS),” IEEE Commun. Mag., vol. 36, no. 10, pp. 150~159, Oct. 1998.

[202] S.B. Yun, S.Y. Park, Y.W. Lee, D.Y. Park, Y.S. Kim, K.H. Kim, and C. G. Kang,
“Hybrid division duplex system for next-generation cellular services,” JEEE Trans. Veh.
Technol., vol. 56, no. 5, pp. 3040~3059, Sep. 2007.

[203] D.G. Jeong and W.S. Jeon, “Comparison of time slot allocation strategies for CDMA/TDD
systems,” JEEE J. Select. Areas in Commun., vol. 18, no. 7, pp. 1271-1278, July 2000.

[204] G. Auer, “On modeling cellular interference for multi-carrier based communication
systems including a synchronization offset,” WPMC’03, pp. 290-294, Oct. 2003.

[205] R1-050764, Ericsson, “Inter-cell Interference Handling for E-UTRA,” 3GPP RAN
WG1 #42, London, UK, Sep. 2005.

[206] R1-050608, RITT, “Inter-cell Interference Mitigation based on IDMA,” 3GPP TSG
RAN WGI Ad Hoc on LTE, Sophia Antipolis, France, Jun. 2005.

[207] R1-062851, Ericsson, “Frequency hopping for E-UTRA uplink,” 3GPP TSG RAN WGI
#46, Seoul, Korea, Oct. 2006.

[208] IEEE 802.16e-2005, Mobile WiMAX forum, “IEEE Std 802.16e-2005 and IEEE Std
802.16-2004/Cor 1-2005” New York, USA, Dec. 2005.

[209] G.E. Bottomley, “Adaptive arrays and MLSE equalization,” JEEE VTC’95, vol. 1, pp.
50-54, July 1995.

[210] A. Paulraj, R. Nabar, and D. Gore, Jntroduction to Space-Time Wireless Communications,
Cambridge Univ. Press, 2003.

[211] G.J. Foschini, “Layered space-time architecture for wireless communication in a fading

704



===== PAGE 701 =====
a2
EI
Ho
ra

environment when using multi-element antennas,” Bell Labs Technical Journal, vol. 1,
no. 2, pp. 41-59, Oct. 1996.

[212] G.D. Golden, C.J. Foschini, R.A. Valenzuela, and P.W. Wolniansky, “Detection algorithm
and initial laboratory result using V-BLAST space-time communication architecture,”
Electronics Letters, vol. 35, no. 1, pp. 14-15, Jan. 1999.

[213] S.M. Alamounti, “A simple transmit diversity scheme for wireless communications,”
IEEE J. Select. Areas Commun., vol. 16, no. 8, pp. 1451-1458, Oct. 1998.

[214] V. Tarokh, H. Jafrakhani, and A.R. Calderbank, “Space-time block codes from orthogonal
designs,” JEEE Trans. Inform. Theory, vol. 45, no. 5, pp. 1456-1467, July 1999.

[215] S. Sanhdu and A. Paulraj, “Space-time block codes: a capacity perspective,” JEEE
Commun. Letters, vol. 4, no. 12, pp. 384-386, Dec. 2000.

[216] I. Telatar, “Capacity of multi-antenna Gaussian channels,” European Trans. Tel., vol.
10, no. 6, pp. 585-595, Nov./Dec. 1999.

[217] J. Grimm, M.P. Fitz, and J.V. Krogmeier, “Further results on space-time coding for
Rayleigh fading,” 36th Allerton Conf., pp. 391-400, Sep. 1998.

[218] S. Baro, G. Bauch, and A. Hansmann, “Improved codes for space-time trellis coded
modulation,” JEEE Commun. Letters, vol. 4, no. 1, pp. 20-22, Jan. 2000.

[219] M.K. Simon, “Evaluation of average bit error probability for space-time coding based
on a simpler exact evaluation of pairwise error probability,” Journal of Commun. and
Networks, vol. 3, no. 3, pp. 257-264, Sep. 2001.

[220] G. Taricco and E. Biglieri, “Exact pairwise error probability of space-time codes,”
IEEE Trans. Inform. Theory, vol. 48, no. 2, pp. 510-513, Feb. 2002.

[221] V. Tarokh, H. Jafarkhani, and A.R. Calderbank, “Space-time block coding for wireless
communications: performance results,” JEEE J. Select. Areas Commun., vol. 17, no. 3,
pp. 451-460, Mar. 1999.

[222] H. Jafarkhani and N. Seshadri, “Super-orthogonal space-time trellis codes,” JEEE
Trans. Info. Theory, vol. 49, no. 4, pp. 937-950, Apr. 2003.

[223] J.H. Winters, “The diversity gain of transmit diversity in wireless systems with Rayleigh
fading,” IEEE Trans. Veh. Technol., vol. 47, no. 1, pp. 119-123, Feb. 1998.

[224] J.V. Traveset, G. Caire, E. Biglieri, and G. Taricco, “Impact of diversity reception on
fading channels with coded modulation—Part I: coherent detection,” JEEE Trans.
Commun., vol. 45, no. 5, pp. 563-572, May 1997.



===== PAGE 702 =====
MIMO-OFDM 무선 통신과 MATLAB

[225] V. Tarokh, N. Seshadri, and A.R. Calderbank, “Space-time codes for high data rate
wireless communication: performance criterion and code construction,” JEEE Trans.
Inform. Theory, vol. 44, no. 2, pp. 744-765, Mar. 1998.

[226] B.L. Hughes, “Differential space-time modulation,’ JEEE Trans. Info. Theory, vol. 46,
no. 7, pp. 2567-2578, Nov. 2000.

[227] B.M. Hochwald and W. Sweldens, “Differential unitary space-time modulation,” JEEE
Trans. Commun., vol. 48, no. 12, pp. 2041-2052 , Dec. 2000.

[228] M. Uysal and C.N. Georghiades, “Error performance analysis of space-time codes over
Rayleigh fading channels,” Journal of Commun. and Networks, vol. 2, no. 4, pp.
351-355, Dec. 2000.

[229] V. Tarokh, A. Naguib, N. Seshadri, and A.R. Calderbank, “Combined array processing
and space-time coding,” JEEE Trans. Info. Theory, vol. 45, no. 4, pp. 1121-1128, May
1999.

[230] Z. Chen, J. Yuan, and B. Vucetic, “Improved space-time trellis coded modulation
scheme on slow Rayleigh fading channels,” JEE Electronics Letters, vol. 37, no. 7, pp.
440-442, Apr. 2001.

[231] W. Firmanto, B. Vucetic, and J. Yuan, “Space-time TCM with improved performance on
fast fading channels,” JEEE Commun. Letters, vol. 5, no. 4, pp. 154-156, Apr. 2001.

[232] B. Vucetic and J. Yuan, Space-Time Coding, Wiley, 2003.

[233] P. Wolniansky, G. Foschini, G. Golden, and R. Valenzuela, ““V-BLAST: an architecture
for realizing very high data rates over the rich-scattering wireless channel,” Proc.
ISSSE’98, Pisa, Italy, pp. 295-300, Sep. 1998.

[234] S. Kim and K. Kim, “Log-likelihood ratio based detection ordering in V-BLAST,”
IEEE Trans. Commun., vol. 54, no. 2, pp. 302-307, Feb. 2006.

[235] J. Kim, Y. Kim, and K. Kim, “Computationally efficient signal detection method for
next generation mobile communications using multiple antennas,’ SK Telecommun.
Review, vol. 17, no. 1C, pp. 183-191, Feb. 2007.

[236] E. Viterbo and J. Boutros, “A universal lattice code decoder for fading channels,” /EEE
Trans. Info. Theory, vol. 45, no. 5, pp. 1639-1642, July 1999.

[237] B.M. Hochwald and S. Brink, “Achieving near-capacity on a multiple-antennas
channel,” JEEE Trans. Commun., vol. 51, no. 3, pp. 389-399, Mar. 2003.

[238] K.J. Kim and J. Yue, “Joint channel estimation and data detection algorithms for

706



===== PAGE 703 =====
oy
a
00
[인

MIMO-OFDM systems,” Proc. 36th Asilomar Conf. Signals, System Comput., vol. 2,
pp. 1857-1861, 2002.

[239] H. Kawai, K. Higuichi, N. Maeda, M. Sawahashi, T. Ito, Y. Kakura, A. Ushirokawa,
and H. Seki, “Likelihood function for QRM-MLD suitable for soft-decision turbo
decoding and its performance for OFCDM MIMO multiplexing in multipath fading
channel,” JEJCE Trans. Commun., vol. E88-B, no. 1, pp. 47-57, Jan. 2005.

[240] H. Yao and G.W. Wornell, “Lattice-reduction-aided detectors for MIMO communication
systems,” JEEE GLOBECOM'02, vol. 1, pp. 424-428, Nov. 2002.

[241] C. Windpassinger, L. Lampe, and R.F.H. Fischer, “From lattice-reduction-aided detection
towards maximum-likelihood detection in MIMO systems,” WOC’03, pp. 144-148, July
2003.

[242] T.H. Im, J.K. Kim, J.H. Yi, $.B. Yun, and Y.S. Cho, “MMSE-OSIC2 signal detection
method for spatially multiplexed MIMO systems,” JEEE VTC’08, pp. 1468-1472, May
2008.

[243] G.J. Foschini and M. Gans, “On the limits of wireless communication in a fading
environment when using multiple antennas,” Wireless Personal Commun., vol. 6, pp.
311-335, Mar. 1998.

[244] L.A. Dalton and C.N. Georghiades, “A four transmit antenna orthogonal space-time
code with full diversity and rate,” 40th Annual Allerton Conf. on Commun. Control,
and Computing, Oct. 2002.

[245] M.O. Damen, K. Abed-Meraim, and J.C. Belfiore, “Transmit diversity using rotated
constellations with Hadamard transform,” Adaptive Systems for Signal Processing,
Commun. and Control Conf., pp. 396-401, Oct. 2000.

[246] Y. Xin, Z. Wang and G.B. Giannakis, “Space-time diversity systems based on linear
constellation precodinng,” JEEE Trans. Commun., vol. 2, no. 2, pp. 294-309, Mar.
2003.

[247] B. Hassibi and B. Hochwald, “High-rate codes that are linear in space and time,” [EEE
Trans. Info. Theory, vol. 48, no.7, pp. 1804-1824, July 2002.

[248] R. Heath and A. Paulraj, “Linear dispersion codes for MIMO systems based on frame
theory,” JEEE Trans. Sig. Proc., vol. 50, no. 10, pp. 2429-2441, Oct. 2002.

[249] G. Ganesan and P. Stoica, “Space-time diversity using orthogonal and amicable orthogonal

designs,” JEEE Int. Conf: Acoust., Speech, Signal Processing, pp. 335-338, June 2000.

707


===== PAGE 704 =====
MIMO-OFDM 무선 통신과 MATLAB

[250] O. Tirkkonen and A. Hottinen, “Complex space-time block codes for four Tx antennas,”
IEEE GLOBECOM’00, vol. 2, pp. 1005-1009, Nov./Dec. 2000.

[251] B.M. Hochwald, T.L. Marzetta, and C.B. Papadias, “A novel space-time spreading
scheme for wireless CDMA systems,” 37th Annual Allerton Conf. on Commun. Control,
and Computing, pp. 1284-1293, Sep. 1999.

[252] M. Vu, “Exploiting Transmit Channel Side Information in MIMO Wireless Systems,”
PhD Thesis, Stanford University, July 2006.

[253] S. Jafar, S. Vishwanath, and A. Goldsmith, “Channel capacity and beamforming for
multiple transmit and multiple receive antennas with covariance feedback,” JEEE
ICC’01, vol.7, pp. 2266-2270, June 2001.

[254] D. Shiu and J.M. Kahn, Power Allocation Strategies for Wireless Systems with Multiple
Transmit Antennas: Internal Report of the University of California, Berkley and Lucent
Technologies, July 1998.

[255] E.G. Larsson and P. Stoica, Space-Time Block Coding for Wireless Communications.,
Cambridge Univ., New York Press, 2003.

[256] E.G. Larsson, G. Ganesan, P. Stoica, and W.H. Wong, “On the performance of
orthogonal space-time block coding with quantized feedback,’ JEEE Commun. Letters,
vol. 12, no. 6, pp. 487-489, Nov. 2002.

[257] D.J. Love and R.W. Heath Jr, “Limited feedback unitary precoding for orthogonal
space-time block codes.” JEEE Trans. Signal. Proc., vol. 53, no. 1, pp. 64-73, Jan.
2005.

[258] J. H. Conway, R.H. Hardin, and N.J.A. Sloane, “Packing lines, planes, etc.: packings in
Grassmannian spaces,” Experimental Math., vol. 5, pp. 139-159, 1996.

[259] A. Barg and D.Y. Nogin, “Bounds on packings of spheres in the Grassmann manifold,”
IEEE Trans. Info. Theory, vol. 48, no. 9, pp. 2450-2454, Sep. 2002.

[260] T. Strohmer and R.W. Heath Jr, “Grassmannian frames with applications to coding and
communications,” Appl. Comput. Harmon. Anal., vol. 14, pp. 257-275, May 2003.

[261] B.M. Hochwald, T.L. Marzetta, T.J. Richardson, W. Sweldens, and R. Urbanke,
“Systematic design of unitary space-time constellations,’ JEEE Trans. Info. Theory, vol.
46, pp. 1962-1973, Sep. 2000.

[262] T. Vencel. Tomlinson—Harashima Vorcodierung fiir Mehrkanalund Mehrbenutzersysteme.
Diploma Thesis (in German), Universitat Erlangen—Niirnberg, Mar. 2002.

708

ee,,r h —cr—=>rrrTCC—=Eea....



===== PAGE 705 =====
om
kJ
Ao
ray

[263] M. Joham, W. Utschick, and J.A. Nossek, “Linear transmit processing in MIMO
communications systems,” JEEE Trans. Signal Processing, vol. 53, no. 8, pp.
2700-2712, Aug. 2005.

[264] M.H.M. Costa, “Writing on dirty paper,” IEEE Trans. Info. Theory, vol. 29, no. 3, pp.
439-441, May 1983.

[265] M. Schubert and H. Boche, “Joint ‘dirty-paper’ pre-coding and downlink beamforming,”
IEEE International Symposium on Spread Spectrum Techniques and Applications, Prague,
Czech Republic, Sep. 2002.

[266] M. Tomlinson, “New automatic equalizer employing modulo arithmetic,” Electronics
Letters, vol. 7, pp. 138-139, Mar. 1971.

[267] H. Harashima and H. Miyakawa, “Matched-transmission technique for channels with
intersymbol interference,” JEEE Trans. Commun., vol. 20, no. 4, pp. 774-780, Aug.
1972.

[268] R.F.H. Fischer, C. Windpassinger, A. Lampe, and J.B. Huber, “Space time transmission
using Tomlinson-Harashima precoding,” /TG Conference on Source and Channel
Coding, pp. 139-147, Jan. 2002.

[269] G. Caire and S. Shamai, “On the capacity of some channels with channel state
information,” JEEE Trans. Info. Theory, vol. 49, no. 7, pp. 1691-1706, July 2003.

[270] C. Chuah, D. Tse, J. Kahn, and R. Valenzuela, “Capacity scaling in MIMO wireless
systems under correlated fading,” JEEE Trans. Info. Theory, vol. 48, no. 3, pp.
637-650, Mar. 2002.

[271] A. Goldsmith, S. Jafar, N. Jindal, and S. Vishwanath, “Capacity limits of MIMO
channels,” JEEE J. Select Areas Commun., vol. 21, no. 3, pp. 684-702, June 2003.

[272] D. Aftas, M. Bacha, J. Evans, and S. Hanly, “On the sum capacity of multiuser MIMO
channels,” Jnt/. Symp. on Inform. Theory and its Applications, pp. 1013-1018, Oct.
2004.

[273] A. El Gama and T. Cover, “Multiple user information theory,” JEEE, vol. 68, no. 12,
pp. 1466-1483, Dec. 1980.

[274] T.K.Y. Lo, “Maximum ratio transmission,’ JEEE Trans. Commun., vol. 47, no. 10, pp.
1458-1461, Oct. 1999.

[275] C. Mun, M.W. Lee, J.G. Yook and H.K. Park, “Exact capacity analysis of multiuser

diversity combined with transmit diversity,” Electronics Letters, vol. 40, no. 22, pp.

709


===== PAGE 706 =====
MIMO—OFDM 무선 통신과 MATLAB

1423-1424, Oct. 2004.

[276] C. Chen and L. Wang, “A unified capacity analysis for wireless systems with joint
antenna and multiuser diversity in nakagami fading channels,” JEEE ICC ’04, vol. 6, pp.
3523-3527, June 2004.

[277] P. Viswanath, N.C. Tse, and R. Rajiv, “Opportunistic beamforming using dumb
antennas,” JEEE Trans. on Info. Theory, vol. 48, no. 6, pp. 1277-1294, June 2002.

[278] O.S. Shin and K.B. Lee, “Antenna~-assisted round robin scheduling for MIMO cellular
systems,” JEEE Commun. Letters, vol. 7 no. 3, pp. 109-111. Mar. 2003.

[279] H.M. Chaskar and U. Madhow, “Fair scheduling with tunable latency: a round-robin
approach,” Networking, IEEE/ACM Trans., vol. 11, no. 4, pp. 592-601, Aug. 2003.

[280] R. Ahlswed, “Multi-way communication channels,” Intl. Symp. Info. Theory, pp. 23-25,
1971.

[281] T.M. Cover and J.A. Thomas, Elements of Information Theory, 2/E. Wiley, 1991.

[282] N. Jindal and A. Goldsmith, “Dirty paper coding vs. TDMA for MIMO broadcast
channel,” JEEE Trans. Info. Theory, vol. 51, no. 5, pp. 1783-1794, May 2005.

[283] G. Caire and 8. Shamai, “On the achievable throughput of a multi—antenna Gaussian
broadcast channel,” JEEE Trans. Info. Theory, vol. 43, no. 7, pp. 1691-1706, July 2003.

[284] D.J. Love, R.W. Heath Jr., W. Santipach, and M.L. Honig, “What is the value of
limited feedback for MIMO channels?,” JEEE Commun. Mag., vol. 42, no. 10, pp.
54-59, Oct. 2004.

[285] P. Vishwanath and D. Tse, “Sum capacity of the vector Gaussian broadcast channel and
uplink-downlink duality,’ JEEE Trans. Info. Theory, vol. 49, no. 8, pp. 1912-1921,
Aug. 2003.

[286] W. Yu and J. Cioffi, “Sum capacity of a Gaussian vector broadcast channel,” JEEE
Trans. Info. Theory, vol. 50, no. 9, pp. 1875-1892, Sep. 2002.

[287] S. Vishwanath, N. Jindal, and A. Goldsmith, “Duality, achievable rates and sum
capacity of Gaussian MIMO broadcast channels,” JEEE Trans. Info. Theory, vol. 49, no.
10, pp. 2658-2668, Aug. 2003.

[288] H. Weingarten, Y. Steinberg, and S. Shamai, “The capacity region of the Gaussian
MIMO broadcast channel,” JEEE Trans. Info. Theory, vol. 52, no. 9, pp. 3936-3964,
Sep. 2006.

[289] C.B. Peel, B.M. Hochwald, and A.L. Swindlehurst, “A vector~perturbation technique for

_710



===== PAGE 707 =====
oY
Ei
00
[인

near-capacity multiantenna multiuser communication-part I: channel inversion and
regularization,” IEEE Tran. Commun., vol. 53, no. 1, pp. 195-202, Jan. 2005.

[290] B.M. Hochwald, C.B. Peel, and A.L. Swindelhurst, “A vector—perturbation technique for
near-capacity multiple-antenna multi-user communication-part II: perturbation,” /EEE
Tran. Commun., vol. 53, no. 3, pp. 537-544, Mar. 2005.

[291] T. Haustein, C.V. Helmolt, E. Jorwieck, V. Jungnickel, and V. Pohl, “Performace of
MIMO systems with channel inversion,” JEEE VTC’02, vol. 1, pp. 35-39, May 2002.

[292] M. Stojnic, HL Vikalo, and B. Hassibi, “Rate maximization in multi-antenna broadcast
channels with linear preprocessing,” JEEE GLOBECOM’04, vol. 4, pp. 3957-3961, Nov.
2004.

[293] Q.H. Spencer, C.B. Peel, A.L. Swindlehurst, and M. Haardt, “An introduction to the
multi-user MIMO downlink,” JEEE Commun. Mag., vol. 42, no. 10, pp. 60-67, Oct.
2004.

[294] Q.H. Spencer, A.L. Swindlehurst, and M. Haardt, “Zero—forcing methods for downlink
spatial multiplexing in multi-user MIMO channels,” JEEE Trans. Signal Processing, vol.
52, no. 2, Feb. 2004.

[295] 2. Pan, K. K. Wong, and T. Ng, “MIMO antenna system for multi-user multi-stream
orthogonal space division multiplexing,” JEEE ICC’03, vol. 5, pp. 3220-3224, May
2003.

[296] R. Choi and R. Murch, “A transmit preprocessing technique for multiuser MIMO
systems using a decomposition approach,” JEEE Trans. Wireless Commun., vol. 2, no.
2, pp. 20-24, Jan. 2003.

[297] A. Bourdoux and N. Khaled, “Joint Tx-Rx optimization for MIMO-SDMA based on a
null-space constraint,” IEEE VTC’02, vol. 1, pp. 171-174, Sep. 2002.

[298] M. Rim, “Multi-user downlink beamforming with multiple transmit and receive
antennas,” Electronics Letters, vol. 38, no. 25, pp. 1725-1726, Dec. 2002.

[299] V. Stankovic, M. Haardt, and M. Fuchs, “Combination of block diagonalization and THP
transmit filtering for downlink beamforming in multi-user MIMO systems,” ECWT, pp.
145-148, Oct. 2004.

[300] IEEE 802.1la, Part 11: Wireless LAN Medium Access Control(MAC) and Physical
Layer(PHY) Specifications: High-Speed Physical Layer in the 5 GHz Band, Supplement
to IEEE 802.11 Standard, Sep. 1999.

711



===== PAGE 708 =====
MIMO-OFDM 무선 통신과 MATLAB

[301] IEEE 802.11nTM/D2.00, Part 11: Wireless LAN Medium Access Control(MAC) and
Physical Layer(PHY) specifications, Feb. 2007.

[302] ETSI EN 300 401, Radio Broadcasting Systems; Digital Audio Broadcasting (DAB) to
Mobile, Portable and Fixed Receivers, Sep. 2004.

[303] A. Sieber and C. Weck, “What’s the difference between DVB-H and DAB - in the
mobile environment?,” EBU Technical Review, Jan. 2005.

[304] K.S. Woo, K.I. Lee, J.H. Paik, K.W. Park, W.Y. Yang, and Y.S. Cho, “A DSFBC-
OFDM for a next-generation broadcasting system with multiple antennas,” JEEE Trans.
Broadcasting, vol. 53, no. 2, pp. 539-546, June 2007.

[305] F. Kozamernik, “DAB~-from digital radio towards mobile multimedia,’ EBU Technical
Review, Jan. 2004.

[306] ETSI EN 300 744, Digital Video Broadcasting (DVB); Framing Structure, Channel
Coding and Modulation for Digital Terrestrial Television, Nov. 2005.

[307] ETSI EN 301 192, Digital Video Broadcasting (DVB); DVB Specification for Data
Broadcasting, Nov. 2005.

[308] ETSI EN 302 304, Digital Video Broadcasting (DVB); Transmission System for Handheld
Terminals, Nov. 2005.

[309] ETSI EN 101 191, Digital Video Broadcasting (DVB); DVB Mega-Frame for Single
Frequency Network (SFN) Synchronization, June 2004.

[310] ETSI EN 300 468, Digital Video Broadcasting (DVB); Specification for Service
Information (SI) in DVB Systems, Nov. 2005.

[311] M. Kornfeld and U. Reimers, “DVB-H-the emerging standard for mobile data
communication,” EBU Technical Review, Jan. 2005.

[312] ECMA~368, High Rate Ultra Wideband PHY and MAC Standard, 2/E., Dec. 2007.

[313] TTAS.KO-06.0082/R1, 2.3GHz #4 y FF Fe] AZ 2 WA FZVIAS 2005.

[314] WiMAX ForumTM, Mobile System Profile Release 1.0 Approved Specification, Revision
1.4.0, 2007.

[315] IEEE Std 802.16eTM-2005 and EEE Std 802.161TM-2004/Cor1-2005, Part 16: Air
Interface for Fixed and Mobile Broadband Wireless Access Systems, 2006.

[316] TTA, 2.3GHz Portable Internet (WiBro) Overview, 2004.

[317] J.G. Andrews, A. Ghosh, and R. Muhamed, Fundamentals of WiMAX: Understanding
Broadband Wireless Networking, Prentice Hall, 2007.



===== PAGE 709 =====
[에
kK
Ao
rat

[318] IEEE C802.16maint-05/083, Hit Ratio Problems with PUSC Permutation, 2005.

[319] Yossi Segal, Tutorial on Multi Access OFDM (OFDMA) Technology, Runcom, 2005.
[320] 3GPP TS 36.201, E-UTRA; LTE Physical Layer-General Description, R8, Nov. 2007.
[321] 3GPP TS 36.211, E-UTRA; Physical Channels and Modulation, R8, Mar. 2008.

[322] 3GPP TS 36.212, E-UTRA; Multiplexing and Channel Coding, R8, Mar. 2008.

[323] 3GPP TS 36.213, E-UTRA; Physical Layer Procedures, R8, Mar. 2008.

[324] 3GPP TS 36.213, E-UTRA; Physical Layer-Measurements, R8, Mar. 2008.

[325] 3GPP TS 36.300, E-UTRA and E-UTRAN; Overall Description, R8, Mar. 2008.

713



===== PAGE 710 =====
MIMO—-OFDM 무선 통신과 MATLAB

찾아보기

0 지연(2600 delay) / 687
1차원 맵핑 _/ 210

1차원 할당 패턴 / 623
2-ray 모델 / 53

2차 다항식 보간 _/ 264
2차원 맵핑 _/ 210

2차원 할당 패턴 / 622
3GPP LTE(Long Term Evolution) / 660
3GPP LTE / 660

3GPP LTE Rel-8 / 660
3GPP LTE 시스템 / 245

AAS(Adaptive Antenna System)

AAS-DLFP / 644

Access state / 646

ACI(Adjacent Channel Interference) / 165, 191

ACIR(Algorithm using Channel Impulse
Response) / 582, 583

ACK 채널 / 630

ACK/NAK  / 679

ACK/NAK 43 / 607

ACPR(Adjacent Channel Power Ratio) / 290

ADC(Analog-to-Digital Converter) / 180

ADS(Azimuth-Delay Spread) / 112

AGC(Automatic Gain Control)  / 534

AGCH(Access Grant Channel) / 248

/ 635, 643

714

AIDC(Algorithm using Intercarrier Differential
Correlation) / 582, 583

Alamouti / 462

Alamouti 부호화기 / 391

aliasing / 308

AMC(Adaptive Modulation and Coding)
/ 198, 208

Antenna Grouping / 639

Antenna Selection / 639

AoA(Angle-of-Arrival) / 42, 112

AoD(Angle of Depature) / 142

APRS(Algorithm using Phase Reference
Symbol) / 582, 583

arrival time / 59

AS(Azimuth Spread, Angular Spread) / 113

Awake HE / 655

backoff delay / 653, 654

base time domain sequence; preamble / 595
bayes’ theorem / 449

Bernoulli Binary Generator / 547
Blast(Single CodeWord; SCW)  / 684
Blind 채널 추정 / 274
break-before-make / 656

Broadcast 채널 / 646

broadside / 135

BS-initiated 핸드오버 / 657

BSAC / 574



===== PAGE 711 =====
Bussgang 알고리즘 = / 275

CA(Conditional Access) / 578

CAPEX(CAPital EXpenditure) / 661

cardinality / 424

CAZAC 시퀸스 / 243

CAZAC(Constant Amplitude Zero-Autocorre-
lation Code) / 303

CCDF(Complementary Cumulative Distribution
Function)  / 293

CCE(Control Channel Element) / 667

CDD(Cyclic Delay Diversity) / 687

CDF(Cumulative Distribution Function) / 293,
294

CDMA 부호 / 653, 654

CDMA 코드 / 653

CE(Channel Estimation) A] #2

Cell ID / 681

cell-specific AH#44e{(scrambler) / 350

Cell-Specific 스크램블링 / 351

Cell-specific °1=|2]4/(interleaver) / 350

Cell-Specific 인터리빙 = / 352

Cell-specific RS  / 668

central Chi-square 분포 / 293

/ 598, 602

central limit theorem / 44

CF(Crest Factor) / 292

channel inversion / 509

Channel Inversion 기법 / 508
Channel State Information; CSI / 471
Chase Combining / 633

Chernoff bound / 389

Chordal distance / 478, 685

Chu AJA / 304

CID(Connection Identifier) / 647, 648

CIF(Common Interleaved Frame) / 575

CINR(Carrier to Interference and Noise Ratio)
/ 624, 658

CINR 추정 / 244

CINR 테이블 = / 629

Clarke / 42

Clarke/Gan 모델 / 73

Classical 도플러 스펙트럼 / 139

Classical 모델 _ / 80, 84

CMA(Constant Modulus Algorithm) / 275

Coarse CFO estimation / 554

coherence 거리 / 471

coherence 대역폭 / 38, 182, 273, 471

coherence 시간 / 41, 273, 471

coherent / 231

collaborative MIMO  / 638

Comb 구조 / 251

Comb 타입 _ / 208

complex equalizer / 182

Compression and Expanding 기법  / 307

concatenated 코드 / 204

condition number / 441

Connected state / 646

connection 11) / 646

Constant Set / 617, 635

Constant Set 0 / 637

Constant Set 1 / 637

Convolutional Encoder / 547

Cosine Function PAS 모델 / 118

COST 207 모델 _/ 99

COST 259 모델 / 153

COST-Hata 모델 / 152

COST-WI(Walfisch-Ikegami) 모델 / 152

Costa precoding / 490

Costas precoding / 492

cover AJA / 598

715


===== PAGE 712 =====
MIMO-—OFDM 무선 통신과 MATLAB

CP(Cyclic Prefix) / 165, 184, 526, 624
CQ\(Channel Quality Indicator) / 668, 679, 683
001 채널 _/ 607, 627

CQICH / 640

CR(Clipping Ratio)  / 309

CRC(Cyclic Redundancy Check) / 631
critical sampled case / 168

CS(Cyclic Shift) / 566

CS(Cyclic Suffix) / 184, 188

CSD(Cyclic Shift Diversity) / 561, 566, 567
CU(Capacity Unit) / 575

Cubic runout spline / 268

Cubic spline / 259

Cubic Spline 보간 / 264

Cyclic Prefix / 224

DAA(Detect And Avoid)  / 600

DAB / 571

DAC(Digital-to—Analog Converter) / 180
DCD _ / 646, 650, 652

DCM(Dual Carrier Modulation) / 599
DD(Decision-Directed) 채널 추정 / 268, 282
Decision—Aided Reconstruction 기법 / 306
deep fading / 203
Deinterleaver / 547

DEM 채널 추정 _/ 282
Depuncture 블록 / 547

/ 376, 389, 409
Deterministic MIMO 채널 용량
Deterministic AY 용량 / 375
DFDMA(Distributed FDMA)  / 330
DFE(Decision Feedback Equalization) / 490
DFT 기반 채널 추정 / 269

DFT 행렬 _/ 479

Determinant
/ 362, 364

716

DFT 확산  / 307, 329

Digital Duplexing / 212

Digital System A / 571

Direct Realization / 167

Direction-of-Movement; DoM_  / 134

distributed 타입 _ / 208

DL-MAP_  / 650

DM-RS(DeModulation Reference Signal)
/ 680, 681

DMB / 243, 571

DMT(Discrete Multi-Tone) / 165, 200

DoA(Direction-of-Arrival) / 79, 135

DoM(Direction-of-Movement) / 79

DoT(Direction of Travel) / 145

DPC(Dirty Paper Coding) / 507

DQPSK_ / 576, 579

DS(Delay Spread) / 113

DS-CDMA(Direct Sequence Code Division
Multiple Access) / 594

duo-binary Turbo 부호화기 / 632

DVB-H(Digital Video Broadcasting-Handheld
terminals) / 243, 571, 583

DVB~-T(Digital Video Broadcasting-Terrestrial)
/ 243, 571, 583

DWMT(Discrete Wavelet Multi-Tone) / 174

DwPTS(Downlink Pilot Time Slot) / 664

E-28)  / 280
ECMA International / 594
ECMA~-368  / 595, 598

EEP(Equal Error Protection) / 578
Efficient Realization / 169
EGC(Equal Gain Combing)  / 382
EGC 기법 / 384



===== PAGE 713 =====
eigen decomposition / 474

eigenvalue / 376, 389

EIRP(Effective Isotropically Radiated Power)
/ 593

EM 알고리즘 / 279

EM 채널 추정 / 282

equiripple 통과 대역 필    / 310

ergodic 채널 용량 / 370, 475

Euclidian 거리 _ / 389

Eureka-147  / 571

EVM(Error Vector Magnitude)  / 290

Expectation Maximization / 279

extended CP / 662, 675

eye diagram / 160

FCC(Federal Communications Commission)

/ 593
FCH  / 607, 609
FCS(Frame Check Sequence)  / 597
FDD(Frequency Division Duplexing) / 212, 471
FFFR(Flexible Fractional Frequency Reuse)

/ 345
FFR(Fractional Frequency Reuse)  / 342
FH(Frequency Hopping)-OFDMA  / 353
FIB(Fast Information Block) / 573
FIC(Fast Information Channel) / 572
FIDC(Fast Information Data Channel) / 578
Fine CFO estimation / 554
Flat 도플러 스펙트럼 / 84
FMT(Filtered Multi-Tone) / 164, 167
Fourier Projection 기법 / 306
Fourier 행렬 / 329
Frame Control Header / 609
frequency reuse / 341

frequency reuse factor / 341

Friis 자유 공간 방정식 / 22

Frobenius norm / 476, 498

FSTD(Frequency Switched Transmit Diversity)
/ 688

full rank  / 365, 375

full-diversity full-rate / 458

full-duplex 방식 / 212

FUSC / 355, 608, 612

FWGN(Filtered White Gaussian Noise) 모델
/ 73

GAST(General Algebraic Space-Time) 부호
/ 457

Gaussian 분포 / 280, 293, 298, 299

Generic MAC 헤더 / 649

Godard 알고리즘 / 275

Golay 상보 시퀸스 _/ 307, 315

Gold AAA / 243

GP(Guard Period) / 664

Grassmannian subspace packing / 477

greedy 스케즐링 _/ 505

Greenfield 2% / 563, 565

H.264  / 574
Hadamard 변환 / 317
HARQ(Hybrid ARQ)
Hartly-Shannon / 198
Hassibi / 463

Hata 모델 / 28
HDD(Hybrid Division Duplex)  / 348
HDD(Hybrid Division Duplexing) / 212

/ 633, 679



===== PAGE 714 =====
MIMO-OFDM 무선 통신과 MATLAB

Hearth?} Paulraj 기법  / 466

HF /19

High Frequency / 19

Hochwald / 463

horizontal 맵핑 / 210

Householder reflection 행렬 / 686

HP(High-Priority) / 586

HSDPA(High Speed Downlink Packet Access)
/ 660

HSUPA(High Speed Uplink Packet Access)
/ 660

HT greenfield format / 564

HT mixed format / 564

HT Mixed 2 / 565

HT(high throughput) / 557

HT-LTF 프리앰블 / 569

HT-SIG_  / 568

HT-SIG1 / 568

HT-SIG2 / 568

HT-STF 프리앰블 / 569

Hurwitz-Radon 정리 _ / 457

hybrid STBC/SM_  / 560

Hybrid-ARQ_  / 668

I-METRA / 77, 125
I-METRA(Intelligent Multi-element Transmit
and Receive Antennas) MIMO 모델 / 132
i.i.d(independent, identically distributed) / 126
IBO(Input Back-Off) / 289
ICI(Inter-Channel Interference)
IDeell / 615, 651
IDFT(Inverse Discrete Fourier Transform) / 179
Idle state / 646

/ 163, 283

718

Idle 모드 / 605, 655, 658

IDMA(Interleaved Division Multiple Access)
/ 352

IDMA 기법 / 356

IEEE 802.11 TGn 모델 / 153

IEEE 802.11 모델 / 56

IEEE 802.118 / 243, 519

TEEE 802.11ㅁ / 556

IEEE 802.117 모델 / 83

IEEE 802.16-2004 / 605

IEEE 802.16d 모델 / 30

IEEE 802.166 / 605

IFDMA(Interleaved FDMA) / 330, 337

IFFT(Inverse Fast Fourier Transform) / 179

IMD(Inter-Modulation Distortion) / 290

IMT-2000 / 605

Incremental Redundancy / 634

Initialization state / 646

Inner 부호화기 / 586

Inte-ACR 핸드오버 _/ 657

Inter-BS 핸드오버 / 657

Inter-Sector 핸드오버 / 657

Interim B3G 모델 / 152

Interleaved 타입 / 208

Interleaver / 547

IP address / 646

IRC(Interference Rejection Combining) 기법
/ 355

ISI(Inter-Symbol Interference) / 158, 595

iterative interference balancing / 509

ITU Pedestrian A / 137

ITU Pedestrian B / 137

ITU Vehicular A / 137

ITU-R /99

ITU-R WP8A_ / 605



===== PAGE 715 =====
Jakes 모델 _/ 86

L-LTF 프리앰블 _/ 565

L-SIG(Legacy Signal) / 565, 566
L-STF(Legacy Short Training Field) / 565
L~STF 프리앰블 / 565

Laplacian PAS  / 93, 137, 144
Laplacian 도플러 스펙트럼 / 84, 139
Large-scale 페이딩 _/ 19, 22

Lattice reduction  / 441, 444

Lattice 구조 / 251

Layer 맵핑 / 683

Layer 맵핑부 / 665

LDPC 부호화기 / 558

LDPC 코드 / 204

LENGTH 필드 / 543
LFDMA(Localized FDMA)  / 330, 337
LLL(Lenstra-Lenstra-Lovasz) / 441, 450
LLL 알고리즘 / 443

LLR(Log Likelihood Ratio) / 633
Localized 타입 / 208

Log-distance 경로 손실 모델 / 23
log-likelihood 함수 / 225

log-normal shadowing 모델 / 24

long preamble / 554
LOS(Line-of-Sight)  / 22, 47
LP(Low-Priority) / 586

LRAD7|¥ _/ 442

LS 채널 추정 기법 / 252

M modulo 연산 / 406

MA)AA / 317

M-28] / 280

MAC / 647

MAC CPS(Common Part Sublayer) / 647

MAC PDU_ / 648

MAC SAP_  / 647

MAC Signaling at} / 649

MAC 관리 메시지 / 649, 650

MAI(Multiple Access Interference) / 246

MAP / 607

max-log approximation  / 450

MB-OFDM(Multiband Orthogonal Frequency
Division Multiplexing) / 189, 594

MB-OFDM Alliance / 594

MBMS(Mobile Broadcasting Multimedia
Service) / 661

MBOA_ / 594

MBS, FBSS(Fast Base Station Switching) / 605

MBSEN RS _  / 670

MC-CDMA __ / 205

MCS(Main Service Channel)  / 572

Metric ball approach / 478

MIC(Multiplex Configuration Information)
/ S72, 578

midray / 152

MISO 채널 _/ 369

ML(Maximum Likelihood) / 225, 424

ML 메트릭 / 436

MML(Modified ML) / 424

MMSE  / 419

MMSE 사전등화 = / 486

MMSE 채널 추정 기법 / 254

MMSE-OSIC_ _ / 420

MMSE7]|"}_ _ / 418

Mobile WiMAX  / 605

modal decomposition / 376



===== PAGE 716 =====
MIMO—OFDM 무선 통신과 MATLAB

Modified IEEE 802.160 모델  / 32
Modulo-D 연산 / 327
20001410연산 / 490
Moose 방식 / 535
MPE-FEC(Multi-Protocol Encapsulation—Forward
Error Correction) / 583, 592
MPEG-2 998 / 574
MPEG-4_ / 574
MRRC(Maximal Ratio Receiver Combining)
/ 382, 419
MRC 기법 / 384
MS-initiated HEEB / 657, 658
MSE(Mean Squared Error) / 253, 419
MT-CDMA _ / 206
MU-MIMO(multi-user MIMO)
Multi-CodeWord; MCW / 684
multicarrier DS-CDMA  / 206

multiuser demodulator / 357

/ 683, 688

mutual information / 363

NAK 채널 / 630
Nakami 분포 / 66
Natural spline  / 266
NLOS / 47
non-critical sampled case / 168
non-contention / 682
Non-HT  / 564
Non-HT 2 / 565
noncoherent / 231
Normal CP / 662, 675
null symbol / 243
Null 심볼 / 575
Nyquist criterion / 159
Nyquist rate / 159

720

Nyquist 대역폭 / 159, 162
Nyquist 샘플링 이론  / 250, 251
Nyquist 필터 / 159

O-PUSC  / 355

OBO(Output Back-Off) / 289

OFDM(Orthogonal Frequency Division Multi-
plexing) / 165

OFDM Demodulator / 553

OFDM Modulator / 549

OFDM 신호 발생기 _/ 665

OFDM-CDMA _ / 206

OFDM-FDMA / 205

OFDM-TDMA _ / 206

OFDMA _ / 206, 660, 662

OFUSC / 608, 612

Okumura 모델 / 27

Open System Interconnect(OSl) / 540

OPEX(OPerating EXpense) / 661

Opportunistic 빔형성 기법 / 504

OPUSC / 612

OR 분해(볼드) / 436

orthogonal overlap / 178

OSIC(Ordered Successive Interference Cancella-
tion) / 419

OSTBC(Orthogonal STBC) / 498

outage 채널 용량 / 370, 475

Outer 인터리버 _ / 586

overlapped-add 방식 / 84

PADS(instaneous Power Azimuth~Delay Spec-
turm) / 112



===== PAGE 717 =====
Pair-wise 오류 확률 / 388
PAPR(Peak-to—Average Power Ratio)
292, 565

PAPR 감쇄 기법
PAPR 특성 _/ 243
Parabolic runout spline  / 266

PARC(Per Antenna Rate Control) / 684
PAS(Power Azimuth Spectrum, Power Angular
/ $2, 91,. 113

/ 289,

/ 289, 306

Spectrum)
PAS 모델 / 116
PBCH(Physical Broadcast Channel) / 666
PCFICH(Physical Control Format Indicator

Channel) / 667
PDCCH(Physical Downlink Control Channel)

/ 667
PDP(Power Delay Profile) / 39
PDS(Power Delay Specturm) / 113
PDSCH(Physical Downlink Shared Channel)

/ 666
PEP(Peak Envelop Power) / 292
permutation / 644
permutation formula / 355
PermutationBase / 618
/ 615, 618
PermutationBase6  / 615, 618
PFS(Packet/Frame Synchronization) 시퀸스 / 598
PGRC(Per Group Rate Control)  / 684
phase ambiguity / 221

PermutationBase4

phase factor optimization / 321

phase reference symbol / 243

Phase Tracker / 553

PHICH(Physical Hybrid ARQ Indicator
Channel) / 668

Pilot 부반송파 _/ 563

PLCP(Physical Layer Convergence Procedure)
/ 541, 565, 597

PLCP 프리앰블 / 531
PLME(Physical Layer Management Entity)
/ 541
PMCH(Physical Multicast Channel) / 667
PMD(Physical Medium Dependent) / 541
PMEPR(Peak-to-Mean Envelop Power Ratio)
/ 291
PMI(Precoding Matrix Indicator)
683
PN Sequence Generator / 549
PN AJA / 243
poly-phase 필터 / 170
poly-phase 필터 뱅크 / 169
Power Spectrum Density / 45
PPDU 프레임 / 542
PRACH(Physical Random Access Channel)
/ 679
PRBS(Pseudo Random Binary Sequence)
/ 577, 588, 621, 626
Pre-distortion 기법 / 307
Precoded STBC  / 476
/ 459, 462
Precoding / 458, 473, 639
Precoding 기법  / 509, 639, 685
precoding 행렬 = / 474
Precoding+ / 665, 678
proportional fair 스케즐링 / 505
PRS(Phase Reference Symbol)  / 575
PRT(Peak Reduction Tone) / 324
PSS(Primary Synchronization Signal)
/ 245, 672
PTS(Partial Transmit Sequence) 기법
/ 307, 319
PUCCH(Physical Uplink Control Channel) / 678
Puncture / 547

Punctured 컨볼루셔널 코드 / 578

/ 668, 679,

precoder

71



===== PAGE 718 =====
MIMO—-OFDM 무선 통신과 MATLAB

puncturing / 522

PUSC / 355, 607, 612

PUSC 채널 _/ 244

PUSCH(Physical Uplink Shared Channel) / 678

Q:) / 394
QL decomposition / 492
QRM-MLD_ / 436, 437

08분해 _/ 427
quadrature 변조기 _/ 291

RA(Random Access)  / 246
RA 프리앰블 / 248

raised cosine 필터 _ / 160, 336
rank / 409

ray / 59, 529

Ray 모델 / 91

Rayleigh 분포 / 50, 293, 298

Rayleigh 확률밀도함수 / 48
RB(Resource Block) / 664, 675
RC(raised cosine) 윈도우 / 192
Reciprocity / 470, 471

Reed Muller 부호 / 317

Reference Signal / 668

/ 509, 510
regularized channel inversion 기법  / 504
renumbering 시퀸스 / 614

/ 664, 675

Resource Element 맵핑부 / 665, 678

/ 664, 675

regularized channel inversion

Resource Element

Resource Grid
RF 모듈 / 494

RI(Rank Indicator) / 668, 683

722

Rician factor / 147

Rician K-factor / 50

Rician 채널 / 47

Rician 페이딩 _/ 134

Rician 확률밀도함수 / 50

rms 지연 확산(079 delay spread)

RNG-REQ_ / 653

RNG-REQ 메시지  / 652

RNG-RSP_ / 653

RNG-RSP 메시지 / 652

roll-off factor / 160

root 시퀸스 _/ 673

round robin / 559

round robin AASA / 505

rounded 도플러 스펙트럼 / 106

RS(Reference Signal) / 668

RS 부호화기 / 575

RS 시퀸스 _/ 681

RS(Reed-Solomon) 코드 / 204

RTG(Receive/transmit Transition Gap) / 607,
611

RXVECTOR / 542

S-RS(Sounding Reference Signal) / 680, 681

S-V(Saleh-Valenzuela) PB / 59, 529

SAM(Scalable Adaptive/Advanced Modulation)
/ 174

Sato 알고리즘 / 275

SC(Selection Combining) / 382

SC-DFE(Single-Carrier
Equalization) / 330

SC-FDMA(Single Carrier-FDMA)  / 307, 329,
660, 675

SC-FDMA 신호 발생기 / 678

/ 38. 39

Decision Feedback



===== PAGE 719 =====
Scalable 대역폭 / 661
scattering 성분 / 47
scheduling request / 679
SCM(Spatial Channel Model) / 141
SCM Text / 151
SCM(Spatial Channel Model) 모델
SCM-E MIMO 모델 / 151
SD(Sphere Decoding) / 426
SDMA(Spatial Division Multiple Access) / 635
SDU(Service Data Unit) / 647
/ 476, 498
Service-Specific CS(Convergence Sublayer)

/ 647
SFBC(Space-Frequency Block Code) / 688

/ 92, 141

SER(symbol error rate)

SFN(Single Frequency Network)  / 571, 661
SG3a UWB 다중경로 모델 / 66

shadowing / 19, 20

SHF / 19

short preamble / 554

shortened Reed-Solomon  / 597

shortened 6 / 577

shortened RS 부호화기 / 586

SlI(Service Information) / 572, 578

SIGNAL 필드 / 532

SIMO 채널 / 368

Simulink / 544

sinc 함수 _ / 159

SINR(Signal to Interference plus Noise Ratio)
/ 419, 420

skip/duplicate / 240

SLM(Selective Mapping) 기법

Small-scale 페이딩 / 19, 36

Smith 모델 / 73

Soft output / 448

spatial rate / 466

/ 307, 318

specular 성분 / 47

sphere encoding  / 509

SPID(SubPacket IDendity) / 634

SQNR 값  / 300

Square Root 분해 / 130

squared Frobenious norm / 362

Square-root raised cosine 필터 / 160

SS(Synchronization Signal) / 668

SSS(Secondary Synchronization Signal) / 245,
672

staggered 프레임 / 347

State / 410

STBC  / 560

steering matrix / 132

subray / 93, 145

SUI(Stanford University Interim) 모델 / 104

SUI-6 채널 / 106

sum rate / 501

sum rate 용량 / 507

Super HF / 19

Superimposed 신호 / 272

SVD(Singular Value Decomposition)  / 362,
476

SVD7]#} 송신기법 _/ 483

systematic 비트 _/ 634

T-DMB / 571

Tail-biting / 632

Tarokh / 457

TCM(Trellis Coded Modulation) / 204

TDD(Time Division Duplexing) / 212, 471,
607

TDL(Tapped Delay Line) / 126

TDL 모델 / 101

TDM(Time Division Multiplexing) / 591

723 _



===== PAGE 720 =====
MIMO-OFDM 무선 통신과 MATLAB

TETRA 11 / 174                        UWB 채널 모델 / 66
TFC(Time Frequency Code) / 595

TH(Tomlinson-Harashima) precoding / 489,

492                                  V-MIMO(virtual MIMO)  / 683, 688
TI(Tone Injection) 기법 / 307                Variable Set / 617, 635
Timing Advance / 247, 653, 682              Variable Set 0 / 637
Tone Injection 기법  / 326                  Variable Set 1 / 637
TPS(Transmission Parameter Signaling) / 588     VCXO(Voltage-Controlled Crystal Oscillator)
TR(Tone Reservation) / 324                    / 240
TR(Tone Reservation) 기법 / 307            VDSL_ / 188
trace / 409                             vertical 맵핑 / 210
Truncated Gaussian / 132                 virtual MIMO / 688
Truncated Gaussian PAS 모델 / 120          Viterbi 알고리즘 / 409

Truncated Laplacian PAS 모델 / 122, 132

TTG(Transmit/receive Transition Gap) / 607,                a
611

Turbo 부호화 / 632                       Walsh AYA _/ 319
TXVECTOR / 542                       water filling / 199

Type I HARQ / 633                       water-pouring / 199, 367, 474
Type 11 HARQ / 634                     WCDMA _ / 660

WiMedia Alliance / 594

cote                WINNER 모델 / 35
WSS(Wide-Sense Stationary) / 44

U-mer / 91

UCD / 646, 650, 652

UE-specific RS / 671                               >.
UEP(Unequal Error Protection) / 578          XO(Crystal Oscillator) / 240
UHF / 19

UL-MAP_ / 650

Ulva HF) 19                                        ae
Uniform PAS / 137, 144                   Zadoff-Chu 시퀸스  / 673, 680, 681
unitary 행렬 / 458, 685                    zero padding / 309
UpPTS(Uplink Pilot Time Slot)  / 664          zero-padded suffix / 595
UWB Forum / 594                       ZF / 418

UWB(Ultra Wide-Band) / 189, 593           ZF 사전등화 / 486

724



===== PAGE 721 =====
개기법 _/ 418

Zipper / 188

ZMCSCG(Zero Mean Circularly Symmetric
Complex Gaussian) / 363, 382

ZP(Zero Padding) / 184, 189

가상 Been} Virtual Carrier; VC)  / 165. 193
각도 Cho} HA] E|(Angle diversity) / 380

4] AlAl(interference-sensing) / 347
간섭 평군(101601600006 averaging)  / 206
w(interference avoidance) / 206
}식 / 683
Z(decision metric) / 401
}(packing) / 648

4A\(boundary condition) / 265
손실(68041 loss) / 19

손실 지수 / 23
Al(hard decision) / 448
A\(Hierarchical) 전송 / 586

이동 / 283

페이딩 / 20

페이딩 채널 _/ 40

피드백 채널(39 feedback channel) / 627
증폭기(011 Power Amplifier, HPA)
290
다이버시티(90806 diversity) / 380
다중화(608081 multiplexing)  / 361

/ 561
행렬 / 561

/ 115
64 i(symmetrical spatial correlation
matrix) / 128
스트림 / 559
+ 확장(608081 expansion) / 562

a
rt
of    =

a 뼈
- (m

KL 2h ot of of oD pm ot
Hu 고

HoH 빈
ny 2 Jp SP SP of fu

KI
~ Jd

mm of

야 off off off off off

aA eS we
om

 rl off oft

oF

주

ok} off
mm

공용 동기 A4}2(common synch symbol) / 624
광대역(\10066300) 채널 / 38

구형파 윈도우((60[200841& window) / 174

구형파((6068084182) 함수 _ / 159

GUS PAS 모델 / 119

기저대역(68960800) 신호 _/ 178

기준 시간영역 ABA = / 595, 598

기준 AlS(Reference Signal) / 588, 668, 680

기하평균 _/ 376
긴 훈련심볼 / 531, 535

내림차순 선택기법
널 심볼 _/ 243

다이버시티 모드 / 355
다이버시티 부채널 / 209
다이버시티 이득 / 391
차수 _/ 467
다이버시티 채널 _/ 612
다중 반송파 / 157

다중 사용자 MIMO / 501, 505, 507
다중 사용자 다이버시티 _/ 503, 504
다중 사용자 복조기 _/ 357
다중
다중
다중
다중

/ 496, 497

ot
x5
=z
>=
끄

Ni

사용자 수신기 _/ 356
(Multiple zone) / 608
%\+(multiple access) / 205
접속 ZHA(MAT: Multiple Access Inter-
ference) / 206
다중 채널 전송 방식 / 163
다중 클러스터 _/ 124
다중경로 파(0410-ㅁ0801 wave) / 36
다중사용자 검출(02410-1486 detection) / 206

725



===== PAGE 722 =====
MIMO-OFDM 무선 통신과 MATLAB

다중사용자 다이버시티(07410-14667 diversity)
/ 207

다중안테나 기술 / 361

단일 반송파 / 157

단일탭 등화기 _/ 163

단일탭 복소 Sey) / 181

대략적 반송파 주파수 추정 / 602

대략적 심볼 타이밍 추정 _/ 602
대략적 주파수 추정 / 536
대략적 프레임 검출 / 624

대역폭 2-(bandwidth request) 레인징 _/ 625
대역폭 확장 인자 _/ 330
대칭 modulo 연산 _/ 492
대칭적 맵핑 행렬(500006400 mapping matrix)
/ 130
AlAl(symmetric) 채널 / 213
도플러 스펙트럼 / 79
플러 전력 스펙트럼 / 46
플러 주파수 / 218
플러 확산0200016ㅠ spread) / 19, 40, 250
동기 4l3(Synchronization Signal)  / 672
동기 엑세스 / 682
동기 4's(Synchronization Channel) / 577
*57|(synchronous) 샘플링 방식 / 240
동기화 기법 _/ 214
동일 Ae Subray 방식 _/ 93
동적 패킷 할당(0570802116 Packet Assignment;
DPA) 기법 / 346, 347
등방성 산란 모델(1600ㅁ02010 scattering model)
/ 86
디지털 04016008 / 188

운딩(00400108) / 102
랜덤 MIMO 채널 용량  / 369

726

파 할당 기법 / 354
/ 682

스 프리앰블 / 679

입 _/ 208

Al(ranging) / 625

채널 / 607

모바일 와이맥스 _/ 605

모부호(02004166 code) / 578, 586
미세 반송파 주파수 추정 _/ 602
미세 심볼 타이밍 추정 _/ 602

sai
fo}
미세 주파수 추정 / 536

반복적인 간섭 제거 / 356
반사((6060000) / 20
반송파 주파수 옵셋(08016 Frequency Offset;
CFO) / 214, 218
반송파 주파수 옵셋 추적 / 624
배열 조정 wWel(array steering vector) / 112
밴드 AMC / 608
밴드 AMC #2 / 209
밴드 AMC 채널 / 612, 620
밴드 타입 / 208
밴드 행렬6800 matrix) / 286
변조부 _/ 678
변조차수(0ㅁ00418000 order) / 424
/직렬 변환기 _/ 180
]법 / 263
계층(66040 sublayer) / 647
/ 165, 526
간 블록 부호 _/ 399
43A\(complex orthogonal design) / 391

Bete oe
= zz 뚜
[> of}

rm (은 of of of off

om

M2 2 +t

x HX

HE HL of
be b> fo ce NS @
ae 그 in, 의
a)

dz Jt ft
IN
EI oft



===== PAGE 723 =====
부가 정보(6106 information) / 318

부공간 기반 채널 추정 _/ 276

부반송파(640080160) / 178

부반송파 맵핑 방식 _/ 330

HAE (boosting) / 624

4442 (subchannel) / 207

부채널 맵핑 방식 / 210

Hos / 397

부호화 이득 / 391

분산 파일컷 _/ 588
+1cl(fragmentation) / 648

블록 구조 / 250

== 대각화(6100 diagonalization) / 512
블록 랜덤 타입 / 208

블록 스케일링 기법 / 306

블록 타입 / 208

블록-대각(6100-01880081) 행렬 _ / 286
비경쟁 _/ 682

비동기 엑세스 방식 / 682
비동기(000-85500700048) 샘플링 방식 / 240
비용 함수(009 function) / 252

빈(610) / 620

사전등화(066-60481128000)  / 485
Atel(scattering)  / 20
AtetAlscatter) / 20
산술평균  / 376
상관-성형 BH (correlation-shaping matrix)

/ 130
상삼각행렬4006『 triangular) / 443
상향링크 _/ 246, 337
상향링크 채널 용량 / 505
상향링크 MAP 정보 _/ 607
상향링크 02090  / 619

상향링크 2090  / 618

상호 분산 행렬(00099-00\80ㅁ8006 matrix) / 255
샘플링 동기화 / 223

샘플링 클럭 BA / 238

샘플링 클럭 위상 옵셋 / 238

샘플링 클럭 주파수 옵셋 / 238

생성 다항식 _/ 521

서브패킷 _/ 633

서브프레임(64088006) / 245, 663
서비스 프리미티브 _/ 541

선형 검출 기법 _/ 418

선형 보간 _/ 263

선형 분산 부호(10687 Dispersion Codes)

/
먼트 _/ 244, 617, 651
세그먼트 ID _ / 608
THE 추정 _/ 244, 624
섹터 _/ 244, 623
셀 ID _ / 672
셀 10 그룹  / 672
셀 탐색 _/ 242, 244, 624
셀간 간섭 랜덤화 기법(006670611 Interference
Randomization Technique) / 341, 350
AZ} 간섭 완화 7) (Intercell Interference
Mitigation Technique) / 341
셀간 간섭 제거 7] "(Intercell Interference
Cancellation Technique) / 341
셀간 간섭 조정 7) A(intercell Interference
Coordination Technique)  / 341
셀룰러 시스템 / 242
소수배 반송파 주파수 옵셋(18000081 Carrier
Frequency Offset; FCFO)  / 222, 580
배 주파수 BAL / 624
트 핸드오버 / 605, 656, 657
다이버시티(68050011 diversity) / 361, 386
구간(61660 interval)  / 655

4y of be
rho fet >

727



===== PAGE 724 =====
MIMO-—OFDM 무선 통신과 MATLAB

다이버시티 _/ 381
다 이종《0100비0 shift) / 170, 221
확상(00116 extension) / 184
= / 646
/ 521, 558
부호 / 350
(scrambling) 시퀸스  / 307
부 _/ 665, 678
파서 _ / 559
스펙트럼 효율 / 397
SF(slot) / 622, 663
슬립 모드(86620 mode) / 605, 646, 655
시간 기준(1106 Reference) / 577
시간 다이버시티(1106 diversity) / 211, 380
시간 지연 확산 / 37
시간 확산(07006 dispersion) / 36
시간영역 FWGN 모델 / 83
시간영역 FWGN 채널 모델 / 84
시간영역 SNR / 194
시간영역 보간기 _/ 240
시간영역 확산(11016 Domain Spreading: TDS)
/ 597, 599
]공간 ㅁ6118 복호기 / 409
trellis 부호화기 / 405
부호화 / 387
블록 부호 / 391
블록 부호화기(60806-11016 Block
Codes) / 396
시공간 성상 S]Al(space-time constellation—rota-
ting) / 458
시공간 성상 회전 부호 / 462
시변 채널 / 283
시분할(1106 Slicing) / 583, 590, 591
시스템 손실 계수 _/ 22
실수 시공간 블록 부호 / 397
심볼 타이밍 동기화 _/ 624

> A> Ay 4>
ju = = fo pe,

[> [> [>
14 14 fy
no! of ot ot ot

qc 0 006 0ㅁ

of of of 포

|»
m

a

>»

of} off off off 이

,
 Se ee

스 주
I

ae,

이

on

r

심볼 타이밍 -4(Symbol Timing Offset; STO)
/ 214

심볼 타이밍 컨트롤 / 624

심볼 파형 성형 / 526

안전 키 교환(660416 key exchange) / 647
안테나 그룹핑 _/ 640
안테나 그룹핑 기법 _/ 639
안테나 그룹화 _/ 643
안테나 선택 _/ 643
안테나 선택 기법 / 494, 639
암호화(6007500400) / 647
액티브 모드 _/ 646
양자화 잡음 / 299
에러 전달(60ㅁ0『 propagation) / 269
역스크램블링 부호 _/ 351
연속 aa / 588
A\(concatenation) / 649
연집 °F (burst error) / 204
오류정정 부호기 / 521
오름차순 선택기법 / 496, 497
오버샘플링 / 276, 301
오차 마루(66ㅠ07 floor) / 539
옥내 채널 모델링 / 52
옥외 채널 모델 / 73
와이브로(\161699 Broadband Internet: WiBro)
/ 604
와이브로 시스템 _/ 244
외부 부호기(04666 coder) / 597
원형000[06026) 필터 _/ 167
위상 기준 심볼 / 243
위상 변화량 / 538
위상 Z-2(phase noise) / 218
위상 추적기 / 553

i 6

¢

¢

은


===== PAGE 725 =====
위상 회전 / 215                           수배 옵셋 추정 / 624
위상왜곡 _/ 222                        정합 필터(0860160 filter) / 163
윈도우 / 526                           조정 대각 행렬(66660108 diagonal matrix) / 135
이산화된 Laplacian 방식 / 95               조정(6666008) 행렬 _/ 132, 135
이중 지수 감쇄 모델 / 61                   주 신호04400 Signal) / 576, 587
인접 심볼간 간섭(1066ㅠ-9\001001 Interference;       주기적(6600010) 레인징 _/ 625, 654
191) / 38                        주기적 확장(6600010ㅇ extension) / 170
인증(340160008000)  / 647                       주파수 다이버시티(1604600 diversity) / 207,
인터리버 _/ 522, 559                         380
인터리빙(10660468\08)  / 204               주파수 비선택적 채널 _/ 163, 182

주파수 비선택적 페이딩 _/ 20, 37

주파수 선택적(6604600/ selective) 채널 _/ 38,
po |                    163, 182

자기 분산 @ A(auto-covariance matrix) / 255     주파수 선택적 페이딩 / 20, 37, 99

자원 할당(7(6904706 allocation)  / 208           주파수 자원 할당 기법  / 341
자원 할당 방식 _/ 209                      주파수 재 사용률(자: frequency reuse factor)
자유 경로 손실 / 22                           / 206, 341
자유 공간(666 space) 전파 모델 / 22           주파수 재사용윤 / 606
작은 순환 지연(60811 cyclic delay) / 687        주파수 호핑 / 595
잔류 반승가 주파수 옵셋 / 587               주파수 호핑 기법 / 353
잔류 위상 추적 / 563                     주파수 Sl(frequency dispersion) / 36
잔류 위상 추적부 / 537                  주파수영역 FWGN 모델 / 77
잔류 주파수 옵셋 / 538                  주파수영역 SNR / 194
저속 페이딩 _/ 20                         주파수영역 확산(『7604600＊ Domain Spreading:
저속 페이딩 채널 / 40                     FDS) / 597, 599
ALA 간섭 조정 기법 / 345              준 3A LLR / 451
전력 스펙트럼 / 45                    준정적 AlA(quasi-static channel) / 52
전력 자원 할당 기법 / 343                   중심 극한 정리(660081 limit theorem) / 44, 293
전력 제어 _/ 509                        지수 모델 / 54
전방오류정정 1S (forward error correction        직교 부호 행렬 / 329
code) / 204                          직교 ©]=(orthogonal theorem) / 254
AS 대역폭 / 36                         직교 자원 Ga(channel segregation) / 347
전송 BEI / 575                     A|alAJ(orthogonality) / 165, 174
절전(00\6 saving) 모드 / 655              직렬/병렬 변환기 _/ 177
정수배 반송파 주파수 옵셋(10[68181 Carrier        직접 맵핑(01760 mapping) / 561
Frequency Offset; ICFO) / 221, 580       짧은 훈련심볼 / 531, 535

729



===== PAGE 726 =====
MIMO-OFDM 무선 통신과 MATLAB

차등 엔트로피(01046060081 entropy) / 364
채널 상관관계 / 376
채널 용량(0180061 capacity)

495
채널 임펄스 응답 / 230
채널 추정 _/ 249, 617

채널 추정 벡터 _/ 255

청취 구간(119660108 interval) / 655
초기 네트워크 진입 / 657

초기 레인징 _/ 247, 625, 652, 653
최대 지연 확산 / 251

최적 LLR / 451

추적 WE(tracking mode) / 235

볼루셔널 부호화 / 631
볼루셔널 인터리버 / 575

/ 684

순환 2| (large cyclic delay) / 687

A E\(cluster) / 59, 529, 613, 637
터 타입 / 208

/ 299, 308

|벨 _ / 300, 309

a / 299

과 필터링 기법

inl
1ㅁ
고
ia}

=

클러
클러
클리
클리
클리
클리

730

off off off off [>
Ae

로 호

/ 306, 308

/ 198, 367, 369,

일(116) / 619
탭 보간(002 interpolation) / 102
탭 재샘플링(040 resampling) / 102
탭 조정 방법 _/ 102
터보(0060) 코드 / 204
통과대역(68590800) 신호 _/ 178

파서 인코더 _/ 558

we 구조 / 249

mae 부반송파 / 524, 617

mY 심볼 / 524

패리티 비트 _/ 632, 634

패킷 9° 4-2(Packet Error Rate; PER)  / 530
패킷 획득 / 602

펄스 4°] (pulse shaping) / 336

페이딩 파라미터 _/ 79, 96

페이로드 _/ 649

페이징 YA(paging area) / 658

페이징 채널 / 659

편파 To] HA] E](Polarization diversity) / 380
평균 지연 확산 / 529

평균 초과 지연(07680 excess delay) / 39
H=Z(closed-loop) / 246

폐루프 MIMO / 639

폐루프 방식 / 683

£0}4(Poisson) 프로세스 _/ 59

=U (folding) / 77

ql prefix / 609

프레임 검출(8016 detection) / 244
프레임 구조 _/ 606

프리앰블 _/ 243, 623

프리앰블 PN 인덱스 _/ 651

프리앰블 인덱스 추정 _/ 624

피드백 / 470, 472

m=)



===== PAGE 727 =====
피드백 비트 _/ 473                        한국정보통신기술협회(11)  / 605
피코넷 / 602                           해석적(30817040) BER  / 193, 527
피크 윈도윙(6646 windowing) 기법 / 306       eo o(handover) / 243, 646, 657
피크 제거(0686 cancellation) 기법  / 306        핸드오버 레인징 _/ 625, 653

핸드오버 절차 _/ 657
을 을 -«               협대역(080ㅁ0\0800) 채널 _/ 37
3}0]EU(whitening) / 351

하드 핸드오버 / 605, 656                  확률적(60008611900) 기법 _ / 307
3s} 2a] A(half-frame) / 664                회전 BA(rotation matrix) / 443
하향 링크 채널 용량 / 507                  3|Al(diffraction) / 20

하향링크 / 243                           획득 모드(4004191400 mode) / 235
하향링크 FUSC  / 617                      훈련 신호 / 233, 252

하향링크 MAP / 607                   훈련 심볼 / 224

하향링크 2080 / 613                   휴대 인터넷 표준 _/ 605

731



===== PAGE 728 =====
조용수

*중앙대학교 전자공학과 졸업 (공학사)

*ㆍ연세대학교 전자공학과 졸업 (공학석사)

*The University of Texas at Austin (공학박사)

한국전자통신연구원 이동통신단 (초빙연구원)

TTA 휴대인터넷(와이브로) 무선접속실무반 (의장)

*현재 중앙대학교 전자전기공학부 교수

전공분야 : MIMO-OFDM #4) 알고리즘 개발 및 FPGA 구현

WV

NS

김재권

*중앙대학교 전기공학과 졸업 (공학사)

ㆍ 중앙대학교 전기공학과 졸업 (공학석사)

*The University of Texas at Austin (공학박사)

*삼성종합기술원 (전문연구원)

aq 연세대학교 원주캠퍼스 컴퓨터정보통신공학부 조교수
"ASH : 신호검출, 통계신호처리

ㆍ서울대학교 전기공학과 졸업 (공학사)

*서울대학교 전기공학과 졸업 (공학석사)

* University of Southern California (공학박사)
ㆍ 현재 중앙대학교 전자전기공학부 교수

정가 39,000원

20084 108 79 초판 인쇄
20084 109 174 초판 발행
Al 자 : 조용수ㆍ김재권ㆍ양원영
발행자 : 우 명 찬ㆍ송    준
발행처 : 홍릉과학출판사
서울시 강북구 수유5동 455-60
(1]4J2|-[88]5]
: 197614 104 219 제5-66호
: 999-2274 ~5, 996-8341, 903-7037
: 905-6729
hongpub@hongpub,co, kr

by

Zz
=

뽀뽀 off
[> fe Hu

www.hongpub,co,kr

※ 낙장 및 파본은 본사나 구입처에서 교환하여 드립니다.
※ 판권 소유에 위배되는 사항(인쇄, 복제, 제본)은 법에 저촉됩니다.
