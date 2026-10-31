---
source_url: /run/media/yutae/Data/제대로배우는 Matlab_Simulink.pdf  # USB PDF (local-only; raw/books/matlab-simulink-jeodeuro.pdf gitignored)
ingested: 2026-10-31
sha256: 5556c6d49ef9e650724a35561a9e135d7068b2ba127e69b57c4b0e784721c465
---

# 제대로 배우는 MATLAB & Simulink (raw source)

## Book metadata
- **Title:** 제대로 배우는 MATLAB & Simulink
- **Authors:** 방성완 저
- **Year:** 2020
- **Publisher:** 한빛아카데미
- **ISBN:** 979-11-5664-482-1
- **Pages:** 577
- **kind:** text-layer

## Body

제대로배우는

八IATLAII&
Simulink
방성완 지음

H= 힌빛이，熬카UI

天믄이 방성완 sungbang@yahoo.com
서강대학교 전자공학과에서 학사 과정을 마친 뒤, 다우가술에서 UN以 기반의 메인 프레임 시스템에 관한 기술 영업으로 근무했다. 미국 메인주립
대학교（Univ아引ty 아卜ii톄ne) 전기 및 컴퓨터공학과에서 석사 학위를 받고，2006년 미국 러트거스 뉴저지주립대학교（The State University 아
New Jersey) 전71 및 컴퓨터공학과에서 광통신 시스템 분야 박사 학위를 벋뻥다. 201 ] 년부터 중앙대학교 전자전7긍학부에서 공업수학 C 프로
그래밍, 물리전자. 수치해석．회로이론을 영어로 강의하고 있으며, 현재 관심 분야는 머신러닝을 응용한 통신 시스템과 5G 등이다. 저서로 r제대로
배우는 MATLA已（한빛아카데미, 2014). r처음 민니는 회로이론i한빛아카데미, 2016), rMAT나＼B으로 배우는 공학 수치해석（개정판M한빛아카
데미, 2018）이 있다．

제대로 배우는 MATLAB & Sim메nk
초판밭행 2020년 3월 5일
工은이 방성완 / 펴낸이 전E暐
펴낸곳 한빛아카데미（주） / 주소 사울시 서대문구 연흐厚 2길 62 한빛아카데매주）2층
전화 02-336-7112 / 팩스 02-336-7199
퉁록 2013년 ] 월 ] 4일 제2017-000063호 / 田BN 979-11-5664小482田 93560
총괄 김한용 / 책임편집 박현진 / 기훠 고지연 / 편집 박현잔 박민정
디자인 표지 이아란, 내지 츠拾훈 / 잔산편집 0峰연 / 저1작 박성우．김정우
영업 이윤형．길진철，김태잔 김성삼，이정훈 임현기．이성훈, 김주성 / 영업7悖1 김호철. 주희
이 책에 대한 의견이나 오탈자 및 잘못된 내욤에 대한 수정 정보는 아라1 이메일로 알려주십사오．
잘못된 책은 구입하신 서점에서 교환해 드립니다．책값은 뒤표지에 표시되어 있습니다．
홉페이지 니八vw.hanb比co.kr / 이메일 question@hanbit.co.kr
Published by HANBIT Academy, Inc. Printed in Korea
（力pyright @ 2020 방성완 & HAN테T Academy. Inc.
이 책의 저작권은 방성완과 한빛아카데매주）에 있습니다．
저작권법에 의해 보호묠 받는 저직뮬이므로 무단 복체 및 무단 전재睡 금합니다．
자금 하지 않으면 할 수 없는 일이 있습니다．
책으로 펴내고 싶은 아이디어나 원고를 메일（wr仕er@hanb仕. co.kr）로 보내주세요．
한빛아카데미（주）는 여러분의 소중한 경험과 지식을 기다리고 있습니다．

머리말 H

기초부터 畿i까지, 흐름을 타고 익히는 MATLAB과 Sim네ink
八4ATLAB은 공학의 기초인 행렬을 이용하여 문제를 처리하고 데이터와 함수를 그래프로 표현할 수 있는 프
로그래밍 언어로, MATLAB 내장함수와 사용자정의함수를 이용하여 공학문제를 빠르고 효율적으로 해결할
수 있다. 또한 확장된 기능을 갖춘 MATLAB 툴박스를 사용하여 과학 및 공학 분야의 많은 문제를 더욱 편리

하고 효과적으로 해석할 수 있다．

미국의 공과대학（또는 공학 관련 학고f)에서는 1학년 정규 수업 과정으로 MATLAB 과목을 개설하여
八4ATLAB을 이용하는 상위 학년 과목의 기초를 미리 다지게 한다. 국내 대학에서도 MATLAB을 이용하는
강의가늘어나고 MATLAB 과제의 비율도 점차높아지고 있다. 이와 같은 이유로 MATLAB의 중요성을 인식
하고 MATLAB을 배우려는 공학 전공又P} 늘고 있다. 하지만 시중쇠］나와 있는 MATLAB 관련 책은 기본적
인 설명 없이 곧바로 복잡한MATLAB 코딩을 다루는 응용 예제로 넘어가는 경우가 많다. 이처럼 入4ATLAB
의 기본과응용이 매끄럽게 연결되지 않으면 주어진 코딩의 한두 줄을 수정하는수준에 머무를 수밖어］ 없다．
필자는 MATLAB 초보자의 가려운 곳을 긁어주는 효자손 같은 책을 선보이고자 2014년에 F저때로 배우는
入4ATLABj을 출간한 바 있다. 당시 책에는MATLAB을 설치하는 방법부터 入4ATLAB의 기본적인 기능과 응
용 기능의 사용법, 수식을 간단히 계산하는 데 활용하는 심벌릭 툴박스의 사용법을 담았다. 또한수치해석, 제
어, 신호 및 시스템, 전자기학, 통신 관련 이론을 바탕으로 MATLAB의 스크립트 파일을 활용하는 방법을 소
개했다. 기초부터 응용까지 차근차근 실행해볼 수 있도록 구성하려 했던 의도를 이해하고 호평해준 독자에게
감사드린다．
이 책에서는 새로운 八4ATLAB 버전을 적용하고 내용을 다듬는 한편, 초판 당시 맛보기 정도로만 실었던
Simulink를 본격적으로 다루었다. Simulink의 기본 개념은 물론이고 다양한 예제를 통해1 설계 과정을 보여
줌으로써 기존의 r제대로 배우는MATLA均에서 한발 더 나oj-7｝고자 노력했다. 학부생뿐만 아니라 대학원생
도 부담 없이 MATLAB과 駐mulink를 배울 수 있계 730여 개의 그림으로 실행 결과를 확인하도록 구성했으
며, 학습자의 편의를 위해 예제어］쓰인 120개 스크립트 파일을 온라인으로 제공한다.
감사의 글
F제대로 배우는 MATLAB. 초판을 집필할 때는 새로움에 대한 용기가 필요했고.2쇄 · 3쇄1 등 중쇄할 때는 독
자어］ 대한 감人P} 필요했다. 이 책을 집필하면서는 나 자신에 대한 인내심이 필요했다. 초판혀1 많은 관심을 보
여준 독자에게 다시 한 번 깊이 감사드리며, 5년 만에 업그레이드 버전을 펴내는 뎨 도움을 준 한빛아카뎨미佯）
에 고마움을 전한다 ．기술 동향혀］ 대한 의견을 피력해준 최은수 군과 바쁜 개인 스케줄어匡 Simulink 설계
모델의 테스트를도와준윤해인 양에게 ' Thanks'를전한다.
지은이 방성완

이 책을 쉽게 보는 방법

니

01

2차원 그래프 그리기

1 학습 목표／Keyword I

그래프1 이욤히여 켤괴

시각적으로 표현히언 살험이나 수식으로 얻은 복집한 수치외 자료岳 各｛브 명쾌하거1 해샥함 수 있

해당 절에서 학습하려는 핵심 내용을
키워드로 정리하여 제시한다．

Key나아d

fiLM시LBB에서 선혐 工기 그래프（2치원 그괘프）표 그리기 위에 시용히는 명렴어뚬 잎이보지，
I 1yot i Fy斗d l 羽n的X 1 SeHn作四p 1 2차권그래포의 모양과퐁류 t

1 口伯t
p匕t 명령어는工축（가로축）에 지정되는 입력 자료 벡터 i에 대웅하여 y축（세로축）에 지정돠는출력 자
료 벡터 V의 그래프를 섕성한다．여러 개의 입력값（UI. 工2. ··．）에 대한출력값（p1. p2, ,,,)의 그래프믈

1 본문 I

생성，臣plo：명령어의기본형태는다욤과같다．

MATLAB과Simulink의
기본 기능부터 핵심적인 기능까지，

plot(xl,yl,x2,y2,...)

꼭 필요한 내용을 간결하게 설명한다．

입력값이 지정된 벡터 X와출력값이 지정된 벡터 y룰 이용하여 그래프를 그릴 때 plot 명령어의 기본 헝
태는 다옴과 같다．
p由t侮y,'s')
, X: 입력값이 지점된 벡fl-I
'V: 官력값01 지정된 벡터
, r5 ' : 치료 기호 선 험fil, 싹상 치젬생락 가뇽하여 순서논 싱괸없뮴）

컴믄셕

k

빰간색

r

그립 파임 불러오기川1보L中1
생성되치 않은 그림 파일을 M月nAB 명령 첨으로 불러오는 빔법과，반대로 M시니B 환겸에서 생성된
그림 파얼로 변환하는 방볍읕 앝이보자
I Inc日ad I Inc目c i

I

image

MATLAB 명령 칭어］서 열어볼수 있도록 변환된 그림 파일의 이미자륩 보여주는 mnage 함수의 기본 형
태는 디음과 같다．
m叩아시
1 片 함수 kflay的S 사K하여 빈깐된 N사니0 그팀 파임

일반척으로 컴퓨터어P4 열어볼 수 있는 그림 파일은 다양하다．파일 이름기 'f培me’라고 해도 확장지에

1
!

!

'］

"1

'｝

"1않올수도있다．

거나그림

'1열리

나그
게曲r:

"培

'

리고

!

따라서 'figurc.bmp', 'figure.gif', 'fl叩re.Jpeg'. '1坦tcre.U且’ 등 여러 가지가 있다．각칵의 유형은 장단
점이 있으므로 사용목적에 맞게 선택하면 된다．그림 유형을 잘못 사용하면 작업을 망칠 수도 있고 ．메모

01日 득뾰한소프트웨에설치하지엽0匠모든컴퓨터몌서C居한획짐X뾔그림파일뮬얼어뮴수있다그러나N戶T녀B읖人好古뼈
샘섬뇐mU酊呵파띄芒M月TLAB0섶치되어밌지26으면사뇽닫수口다．또한M月T녀日퇀召에서샘섬되지26놘T自Ur巳bm口

,

' “帥

" '' "" "

" "

"

叫小m寸，

IT下 1
실습 과정에서
주의하먀 할 사항과 참고로
알아두면 좋은 내용을 담고 있다．

和卜F心e

1 예체 5中31
H

Grade Ir.m

시험 점수큠 나타내는 변수 i의 범위는 0 드 r B 100이며，입력하는 변수의 값에 따라 다．뮴과 같이 A B, C, 0,
F로 성적이 구분된다，
A 工 크 90 日： go 드e509. C: 70B 工 드 79
0: 60 드 X 드 69. F: 工 < 50
스크립트 파일 'GrcdeJf.m’에 조건문율 작성하고， e '90. r- 60, 工 =37울 입력한 결과를 확인하라 이때
tt口Ut 명령어를 이용하여 시험 점수를 입력받아라

-i r小디LE I
해당 예제 학습에 필요한 실습 파일로，
온라인에서 다운로드할 수 있다．

제대로 배우는 MATLAB & Simulink
PART 여"-'03 : MATLAB 활용
1 예제 9小

MmB如 1 lii幻nn n]

1

시간 0夕드10일 때 전달함수 G巾）,G,Le）의 직렵 연결과 병렵 연결에 대한 계단 웅답을 그래프로

나타

-I 예제 1

내라

대표적인 공학 예제를 제시하고，

G (a)＝그＝
：三릎

(a)

MATLAB 함수／명령어를 사용하여

業

해결하는 과정을 실습해 본다．

1series, parallel
SeneS 함수와parallel 합수는 전달함수 2'卄룔 각칵 직렬． 병렬로 연걸하는 함수미다‘ 직렬 또는 병렬로 연
결된 전달함수 so引과eye2를 곱하거나 더하여 새로운 전달힘수 SyS묠 생성한다．두 함수의 형태는

다옴과

1 배경지식 1

갇다，

공학 예제를 해결하기 위해
필요한 전공 지식 및

sys = series(sysl, sy82)
sys = parallel(sysl, sys2)

茹

MAT나＼B 함수／명령어
사용법을 제시한다．
1 풀이 1
완성된 MAT나＼B 코드와
결과화면은 물론, 함수／명령어의
쓰임을 이해할 수 있도록
라인별 상서1 설명을 제시한다．

그핌 9-li 직I 면겊과 볍I 언겊 丑딤 S괴｛11口med
0 시간0드1010올 지정한다，
0ff함수를 이용하여 전달함수 G,(s牌｝G2m）믈 지
0 series 함수푤 이용하여 두 전달함수를 직렬 연결호
Opera)!이 함수묠 이용하여 두 전달함수묠 병렬 연켭
0 계단출력 옹답을 얻기 위해 step 합수를 이용한다
0 전달합수의 직렬 연궐 결과묠그래프로 나타낸다．
0 전탈함수의 병렬 연결 결과을 그래프로 나타낸다；

! 예제 16- 10 1
계단입력 합수.(s) =l

(0 드 , 드 4). 전딜합수G(a)＝갸古万일 때 비려卜미분제어기匹구현6는

시뮬링크 모델을 설겨빠고 그 결과쿰 스코프 챙川 나타내라．이때 비례 아득 瓦 = IS0 미분 아득

翡

凡 = 10이다，

비톄미분 쟤어기는 시스템 옹답의 미래 오류 예측미 가눙하기 때문에 제어 눙궉의 향싱에 의톄 시스텝의
안정성을 증가시키논 더j 사용합 수 있다， 갑작스럽게 변하는 오류 신호의 영함을 피하기 위볘 미분은 오류
신호 대신 시스텝 변수의 츨력 움딥에서 실행된다．띠라서 D 모드는츰력 변수의 변회에 비례하도록 설계되
어 있어 오류 신호의 갑작스러운 변화에 의한 쟤어 출력의 급격한 변화뮴 방지한다．또한 D는 공정 소옴올

PART 04 : Simulink 활용

직접 증폭하기 때문에 D 전용 졔어가사용되지 않는다；

r +(8＋尺d)1 +(l2＋尺P)

1 예처I I
대표적인 공학 예제를 제시하고，
Sim메nk률 활용하여 설계하는 과정을
실습하1 본다．

(a) 끼12 Controller불콕을 人降하지 않는 겅우
Os노P 블폭올섕성하고（[S이玎CeS卜田妃p1) 블록의 이름읕0(1)로 바꾼다，
0 Add 블륙 2개믈 생성하고（小lath Opeeeflon引-thddl) 블륙의 이륨을 각칵 Addl Add2로 바꾼
다．뷸콕Addl올 더블클릭하여 [L油 町없肛S:］에＋ 률 설정한r十
0 Gain 볼콕 37卄쁠 챙성하고（[Comm毗yUsed Blocks卜［Geini) 뷸록의 이롬을 각각 Kp, Kd.
Fil把nme民 바꾼다．블톡 Kp, Kd. Fil油m凹f묠 더블쿨릭하여 [Ga血：
］에 각칵 ISO, Ill, IS0
올 입력힌디1

1 배경지식 1
시뮬링크 설계를 진행하7뻬 앞서，
예제 해결에 필요한 사전 지식을
제시힌따．

0

I-1- 묩설정힌디1

Ols妃gm奴블륙을 생성한다（[Commonly I力odB岫1冬］-these可alor[(
0

Sim베nk를 활용한 설계 과정을
직접 따라하1 볼 수 있도록
진행 과정을 상세하게 제시한다．

Tam好Pen七n 묠록을생성하고（)Co恤lm珌나Ta田四缸 Fc刈） 블록의 이룝올 G佃로 바꾼후 더블
클릭히여 {14山l町star no얘km四卞款나 띠malninator coeffici帥蝴에 [I 8 12］룰 입력힌디，

0 Scope 볼록율생성하고（Is뇨ka卜四叫川）뷸록의 이롬을 C台）로 바꾼다；
0

1 퓸이 1

Scm 블록을 생성하고（)Commo川yUsed B佃sic可나鈿ml) 더룔클릭하여 [List of aigeso:］에

생성된 뷸콕을 文볘로 연결힌디＝

H

예제 파일과 참고 문헌

파일
m 예제
이 책의 예제 파일은 다음 주소에서 다운로드할 수 있습니다．
http://www.hanb比co.kr/src/4482

耳 참고 문헌

=K. E. Atkinson & W. Han, rElementary Numerical Analysis, 3 ' Ed..,
JohnWiley & Sons, 2004.
·W. J. Palm III, nlntroduction to Matlab 7 for Engineers, McGraw-Hill, 2005.
· R. V. I沁kk恥ti, nAnaly曲 and Des培n 可C이出이 Systems I招ing MATLAB.L
New Age International Publishers, 2006.
· B. C. Kuo & F. Golnaraghi, rAutomatic Control Systems, 8 Ed.J,
John Wiley & Sons, 2006.
.A. V. Oppenheim, A. S. Willsky & S. H. Nawab, nSignals & Systems, PrenticeHall, 1997.
· 이철희, 0디지털 신호처리J, 한빛아카데미, 2013.
:A. T. Adams &J. K. Lee, rElectromagneticsJ, Cognella, 2011.
- D. K. Cheng, nField and Wave Electromagnetics, 2nd Ed.J, Addison Wesley
Publishing Company, 1989.
:M. P. Fitz, 印undamentals of Communications Systems, McGraw-Hill, 2007.
- MathWorks Korea, http://wwV.mathworks.co.kr

耳 함꺼1 읽으면 좋은책

MAT나＼B으로 배우는
공학 수치해석（개정판）

핵심이 보이는
제어공학（개정판）

방성완 지음

김성중 지음

전자기학
A. T. Adams. J. K. Lee 지음
유태훈, 허노정 옮김

Contents

PART

01

MATLAB기본기능익히71

CHAPTER 01 처음 만나는 MATLAB

15

저는 MATLAB을 처음 배워요
LESSON 01 M4山＼B 소개

16

LESS아'J 02 M.ATLAB 설치하기

]8

LESSON 03 卜AATLAB 실행하고 종료하기

24

LESSON 04 M月T냐＼B 화면 살펴보기

25

LESSON 05 자료 저장하기

29

LESSON 06 도움말 명령에 사용하기

30

CHAPTER 02 명령어쁠 담는스크립트파일

33

코딩 내용의 기록은 저한테 주서隍

PART

02

LESSON 01 스크립트 파일 생성하고 실행하71

34

LESS아J 02 현재 폴더 변경하71

38

MATLAB핵심기능익히71

CHAPTER 03 데이터를 저장하는 배열과 변수

43

수식 표현은 이것만 이용하면 0K
LESSON 01 산술 연산자 사용하기

44

LESSON 02 내장함수와 변수 사용하기

48

LESSON 03 배열 입력하기

52

LESSON 04 규칙적인 배열 표시하71

58

LESSON 05 배열 원소 다루21

60

LESSON 凹 배열 특성 구하기

65

LESSON 07 출력 서식 변경하기

67

Contents

CHAPTER 04 데이터를 한눈에 보는 그래匹

69

자료를 시각적으로 표현하고 싶어요
LESSON 01 2차원 그래프 그리기

70

LESS（기\J 02 그래프 속성 지정하기

74

LESSON 03 3차원 그래프 그리기

84

CHAPTER 05 흐름올 바꾸는 프로그래밍

93

프로그램1 구성을 한눈에
LESSON 01 관계 연산자사용하기

94

LESSON 02 논리 연산자 사용하71

96

LESSON 03 조건문 사용하기

98

LESS아寸 04 순환문 사용하71

101

LESS아＼J05 사용자정의함수 작성하71

105

CHAPTER 06 수식 계산이 편한 심벌릭 툴박스

109

컴퓨터도 수식을 쑬 수 있어요
LESSON 01 심벌릭 툴박스 사용하기

110

LESS아q02 수식 표현하기

112

LESSON 03 조판 형태로 출력하기

118

LESS(：八 04 심벌릭 그래프 그리기

]19

LESSON 05 대수방정식과 초월방정식 계산하기

120

LESSON 06 심벌릭 미적분함수 사용하기

122

LESSON 07 상미분방정식 계산하기

128

LESS아d08 라플라스 변환하기

131

LESS(가d09 행렬의 특성 다항식 계산하기

133

CHAPTER 07 외부 파일 불러오기／내보내끼

135

서로 도우면서 지니恨
LESSON 01 그림 파일 불러오기／내보내기

136

LESSON 02 엑셀 파일 불러오기／내보내기

139

Contents

PART

03

MATLAB 활용하기

CHAPTER 08 수치히썩

145

정확한 수치히忙I은 MATLAB의 능력을 빌리세요
LESS아.J 01 2진수와 ]0진수 변환

146

LESSON 02 오차

1馭）

LESSON 03 역행렬

152

LESSON 04 선형연립방정식

155

LESS아寸 05 가우스 소거법

159

LESSON 06 상하행렬 분해

]61

LESSON 07 테일러 급수

166

LESSON 08 테일러 다항식의 근삿값과 오차

168

LESS아d09 선형 보간법과 스플라인 보간법

171

LESSON 10 함수의 근 구하기 .

175

LESSON 11 함수의 근을 구하는 다양한 방법

178

LESSON 12 수치 적분법

184

LESSON 13 수치 미분법

190

CHAPTER 09 제어

197

MATLAB 사용의 시초는 제어 분야여阻
LESSON 01 닫힌 루프 시스템

]98

LESSON 02 라플라스 변환

204

LESSON 03 전달함수

208

LESS（가J04 상태방정식

2怡

LESSON 05 시간 응답

220

LESS아q06 안정도

225

LESS아J 07 근궤적

228

LESSON 08 주파수 응답

234

LESSON 09 나이퀴스트선도

239

LESSON 10 니콜스선도

241

Contents

CHAPTER 10 신호 및 시스템1

243

신호의 개넘은 MATLAB 그래프로 이해하세요
LESS아J 01 신호

244

LESS아1 02 이산 시스템

252

LESS아q03 컨벌루션

256

LESS아q04 샘플링

260

LESSON 05 신호 복원

264

LESSON 06 연속 신호의 주파수 표현

266

LESSON 07 이산신호의 주파수표현

272

LESSON 08 라플라스 변환

277

LESS아J09 z 변환

2的

LESSON 10 디지털 필터

286

CHAPTER 11 전자기학

291

어려운 벡터 해석도 MATLAB이 쉽게1 해주네요
LESSON 01 벡터

292

LESSON 02 벡터 좌표7카

298

LESSON 03 벡터 적분

302

LESSON 04 벡터의 발산

306

LESS아405 벡터의 회전

310

LESS아406 전하

314

LESSON 07 가우스 법칙

319

LESSC가寸 08 커패시터와 커패시턴스

321

LESSON 09 전위

325

LESSON 10 경계 조건

327

LESS아寸 11 인덕터와 인덕턴스

331

LESSON 12 라플라스 방정식

333

LESSON 13 비오e사바르 법칙

3：梵

LESSON 14 암페어 법칙

339

LESSON 15 맥스웰1 방정식

341

LESSON 16 균일 평면파

344

Contents

CHAPTER 12 통신

347

스마트 통신은 스마트한 MATLAB이 최고지요
LESSON 01 확률

348

LESSON 02 누적분포함수와 확률밀도함수

353

LESSON 03 아날로그 변조와복조

358

LESSON 04 아날로그1디지털 변환

365

LESS아q05 신호 잡음

弱7

LESSON 06 디지털 변조

369

APPENDIX MATLAB과인공지능의 만남

PART04

［온라인제공I https://cuff.Iy/yr3MmpI]

Simulink설계하71

CHAPTER 13 시뮬레이션을 위한 시뮬링크

385

다양한 블록을 이용하면 시뮬레이션이 가눙해요
LESS아401 시뮬링크 실행하기

386

LESSON 02 기본 블록을 활용하여 설계하기

390

LESS（가寸 03 그림 창에 결과 나타내기 .

4｛兀

LESS（가寸 04 사칙연산 활용 및］차 함수 입출력 그래프 설계하기

403

LESSON 05 복소수 활용하기

410

CHAP丁ER 14 미분방정식

415

복잡한 수식을 한 번어i 줄여나가요
LESS아寸 01 1차 미분방정식 시뮬링크 모델 설계하기

416

LESSON 02 2차 미분방정식 시뮬링크 모델 설계하기

423

CHAPTER 15 삼각함수

435

기하해석을 위해1 필요하군요
LESSON 01 사인 파형 이해하기

436

LESSON 02 코사인 함수 생성하71

443

LESSON 03 정현파 응용 설계하기

449

Contents

CHAPTER 16 제어

453

제어 시스템의 분석 및 설계를 체계적으로 도와줘요
LESSON 01 닫힌 루프 시스템

454

LESS아J 02 전달함수

弱8

LESS아q03 상태방정식과신호흐름선도

463

LESSON 04 다양한 제어71 설계 및 비교하기

468

LESSON 05 보드선도와 니콜스선도 설계하기

476

CHAPTER 17 신호 및 시스템1

485

신호 처리 및 분석 수행을 시각적으로 볼 수 있어요
LESSON 01 다양한 함수의 신호 나타내71

486

LESSON 02 신호를 전달하는 모델 설계하기

496

LESSON 03 필터 설계하기 .

501

CHAPTER 18 벡터

505

크기와 방향을 블록으로 이해해요
LESSON 01 벡터와 행렬 연신하기

506

LESSON 02 벡터를 활용하여 설계하71

515

CHAPTER 19 통신

521

시뮬레이션을 통히｛ 통신 시스템을 검증할 수 있어요
LESSON 01 확률 나타내기

522

LESSON 02 아날로그 변조 및 복조 설계하71

528

LESSON 03 디지털 변조 설계하기

538

CHAPTER 20 회로

545

복잡해1 보이는 회로 설계를 쉽게 접근하네요
LESSON 01 회로의 기초 도입하71

5弱

LESSON 02 저항, 인덕터, 커패시터 조합하기

551

LESSON 03 연산증폭71 이해하기

558

LESSON 04 전력 사용하기

563

짖K가보71

567

함수／명령어／블록 찾아보기

573

MATLAB

기본 기능
익히기

처음 만나는 MATLAB
"저는 M씨U\B을 처음 배워요"
명령어를 담는 스크립트 파일
"코딩 내용의 기록은 저한테 주세요"

\\

PAR丁 01에서는
무엇을 배울까？

MATLAB 소71$
小始TLAB은M카rix Laboratory를줄인 말로, 미국 매스웍스에서 개발한고급 테 !
｝크니컬 프로그래밍 언어이다. 이름에서 알수 있듯이 MATLAB은 행렬을 이용하여 ;
.데이터와 함수를 처리8洌 쉽고, 그래프어］ 표현할 수 있으며, 다른 프로그래밍 언어 4
＼와 연결하여 신속하게 프로그램을 개발할 수 있도록 돕는다. 따라서 과학 또는 공학 三
1을공부하는사람들에게흘륭한개발환경을제공하는유용한프로그래밍 언어이다．
小LATLAB은 뎨이터 분석, 알고리즘 개발, 모델 작성을 위해1 다양한 수치 연산 메소 二
」드를 제공한다. 일반적인 공학 및 과학 연산을 지원하는 수학 함수가 포함되어 있으 }
며， 핵심 수학 함수는 벡터와 행렬 연산을 빠르거1 실행할 수 있도록 프로세서 최적 二
화 라이브러리를 사용한다. 또한 필요에 따라 툴박스 패키지를 추가하면 더욱 확장 ;
『된 기능을사용할수있다.

\

MATLAB 기본 기능 익히71
;，좋은 자동文f7} 있어도 운전하는 방법을 모르면 쓸모없는 물건이 되고 만다. 1부어l
；앞으로운전할MATLAB의 시동 거는 방법과유용한운행 방법을 학습한다．
江장에서는 MATLAB을 설치하는 방법부터 화면 구성과 함수／명령어의 쓰임을 알 /
：아볼 수 있는 도움말 명령어까지 MATLAB을 시작할 때 꼭 알아야 하는 기능을 다
룬다.

「

i2장에서는 MATLAB의 코딩 작업을 편리하게 해주는 스크립트 파일에 대해1 배운 :
꽈. 또한 스크립트 파일을 사용하기 위해 현재 파일의 경로를 추가하고 변경하느二
1

J

」법을 살펴본다．
; 이 책을 이용하여 MATLAB을 실습하려면 MATLAB R2015b 이후 버전을 사용하71 바란다．
三 202아크 현재 MATLAB 최신 판은 MATLAB R2019b이다．

!1
!1
i}
t1
I!
I
H 十m小山 n
nm 小H
기m小m나 4Hh11녀1戶 H小小小＋+m寸如
口mr小十如
r二叫jm寸

나＋1뇨1- =＝小느＋+++4a二二二4
小뉴41. ,＝工니艸 」 +；二J小卜나Hdm二＋나 1
4
1

!

mm{

二二 느二-1-

1

r

m1mm小니 m 寸小4小U1 尸山 r如rmm=

I
I
!
1
!
1
1
1
1mmm니니 小h니 二小m七 工 H 小m4 m
三
!
!
i
!

= m m n1 U m 4小

二i

!

{; !

i

1

}
]

卄 LH小

!

mr m

1

L.J. i

1

1
小 hHHm나

!

1

m

규mm m

1

r

!

!

!

i

I

1

}

r卄十n나

二

1

日m 1

i

!

L그삐tm1

}
l

! IL Li I ! ] I i ! ! I

小나

i小4

4小4나二니ma叫dm 上 나

二

二

1小卄나

十艸1叫＝

r 卄 少才 ;}
H

1

1

t

i

}

01

寸

14 1

t

1 1 丁 了기

丁m까

1如！ m｝小샤

卜！시니 { i ! ! :
十나卄 小냐小＋ f H+

니

i

너

了十十
1

m

처음 만나는
MATLAB

1

艸

L
小

卜

十

十

1

4

1

1二

i

1

J

小上十mL小U十
！

' a如L上上工小L上

牛

I世卄出甘｛i

+ 나L小뇨J j J

: 나나如卜뇨나小和
1 !
}
1 1 1 1

十나커小卜나H小

1

I

4

i

寸

1

于

I

十
1

t
!

-t

＋나

卄

卜卜나 ,j F寸 : 寸 十＋=
1

CONTENTS

.t.L.甘甘 기寸 f-t 4H나

+

.1

;

i 二

4-

4---

十

+

I-나

샤

Hj

卄

十小

i

＝二나二＝

= 1 느！=
H4

4

니

나나

-I

그 } ! =i4工二- f니＝
t t 三 卜 j (寸 十 j 나 +
十十十如卄卄十十丁十寸 !
L

七F
J

4

!

1
!

i1

LESSON 02 MATLAB 설치하기

1

1

1

寸

1

1

r

ml 二 工그二
!

LESSON 01 MATLAB 소가1

二11卜

! 1- t-＋나 +＝卄H 尸 r 寸

卜

:

r" 1 1 了 卞 了

寸中-t

"

i

CHAPTER

1

'

i

寸小中H卜小i

,

小 小

Ij .
I 1 卜＝二三
! If 卜＋

! : ;- {
1

十1나小

=
!

나』나寸二十＋4니나 ＋나（小＼」

＝小卄-1-

m1

1

卞너H丁寸寸如r十寸 十十r寸‘

1

t

I

니H

寸山

小亡1

1

mnH 卜 小小

丁 “十艸卞

LESS아寸 03 MATLAB 실행하고 종료하기
LESSON 04 MATLAB 화면 살펴보기
LESS아4 05 자료 저장하기
LESSON 06 도움말 명령에 사용하71

r小了 T叫中

LESSON

MATLAB 소'H

01

MATLAB唾 미국 매스웍스（Math叭幻水하에서 개발한 고급 테크니컬 프로그래밍 언어이다. 이 레슨을 통해 MA1TAB이 왜
필요한지 어느 정도 짐작할 수 있다. MATLAB으로 할 수 있는 작업에 대하1 알아보자．
Keyword

I

I MATLAB I 수치 계산 1 데이터 분석 1 데이터 시각화 1

MATrix LABoratory

MATLAB은 MATrix LABoratory를 줄인 말로, 공학의 기초인 행렬을 만들고 조작하는 프로그래밍 언
어이다. 따라서 행렬을 이용하여 데이터와함수를 처리하기 쉽고, 그래프어］표현할수 있으며, 다른 프로
그래밍 언어와 연결하여 사용할 수 있다. 또한MATLAB 내장함수와 사용자정의함수를 이용하여 과학 및
공학 분야의 문제를 빠르고 효율적으로 해결할 수 있다. 필요에 따라 툴박스佃olbox) 패키지를 추가하
면 더욱 확장된 기능을 사용할수 있다．

I

MATLAB으로 무엇을 할까？

신호 처리 및 통신, 이미지와 비디오 처리, 제어 시스템, 테스트 및 측정 등 다양한응용분0卜네서 MATLAB
을 사용할 수 있다. 八4ATIAB을 사용하면 수치 계산, 데이터 분석 및 시각화, 프로그래밍 및 알고리즘 개
발, 응용 프로그램 개발 및 배포 등을 할 수 있다. 이 가운데 이 책에서는 수치 계산, 데이터 분석 및 시각
화를주로다룰 것이다. 이를간락히 소개하면 다음과같다．

수치 계산
入4ATL&B은 데이터 분적, 알고리즘 개발, 모델 작성을 위해 다양한수치 연산 메소드를 제공한다. 일반적
인 과학 및 공학 연산을 지원하는 수학 함수가 포함되어 있으며, 핵심 수학 함수는 벡터와 행렬 연산을 빠
르거］실행할수 있도록 프로세서 최적화 라이브러리를 사용한다．

데이터 분석 및 시각화
入4ATLAB은 데이터를 수집 · 분석하고 시각화함으로써 스프레드시트나 기존의 프로그래밍 언어를 사용할
때보다 시간을 단축할 수 있다. 또한 플롯과 자동 리포트 생성 기능, 자동화된 MAUAB 코드 등으로 결
과를 공유할 수 있다．

16

PART01. MAT녀B 기본 기능 익히기

1
注1

2

3

1

4 石 J 月 4 如mi甲小

0111걱

I0128

10132

也凹的

00111

0끄IS

.00期

02引b

oa끄

七1112

따三批

工4478

4］刃I

43230

也6聊

42叭I

1未虧

.30釘5

也lb幻

]I四2

-4.1306

｛나묘7

-1W7

43柳

七고Zn

I.的臼

.3- I

416(7

工0포月

三on

口Jl여｝

4邸5

424恥

日a"

工'II,

{）們'7
n n 印

n

口mmmH너mm比蜘呻

4n 11

八 r M

시

A 수치 계산
亘 I-

· 乙山m니m 出n斗

.'m

H

-

--U

(d1m h니m1

e呻H

--

e-

1

_

II.

m1꺼1=

=

_!k

-小mm
nm hn Lmmm
'

\ 卜k

4

n1너Hm

므

느

-

件새

1? 1m HH

m41 4

뇌 1HH Hm
뇌！
H1Nm

n113 "1
11a m

노1 nd Nm

11！
너d 1

1i시m N匕

11J1 1

叭j11 UW
VmlJ Hm

n 1n 11
n；
月 11

乍114 Nm

mn 4

甘？mJ H너

11 1 1

11 m가 HH

크 1기1 下

m nn Vm

i; 미n 까

小r116] U나

凸m

卄 m 1 Um

N] +

H PH 나A

H Jn 11

小如 N니

가]

A 데이터 수집

m m m m M m 艸 m 二 m m m 名

니 M H M M 나 놔 小 M M 낟 H M H 놔

늬 느川 U니

1
1 口 1
1 1

尸：:

n

1 1 1

i

p._ ..＝山．. m.d...m m.4m1 升mm

二

田띠日宜
(mH

1 느m=1nm1111

-

rJ

mm

目10

r

1
1

4d a寸 m1 1

1

t

1 1 11J

1
111

1

H ra

=J
H뇨J

'

肛匕，1,
노娜出二 N

, a；
十 忌， "

A 데이터 분석

a叫r弓戶1. 11 吼,11
rigt 1m
A.- I- j.

A 데이터 시각화

A 결과 문서화 및 공유

CHAPTE日 01. 처음 만나는 MATLAE

17

LESSON

02

MATLAB 설치하기

MATLABR을 정식으로 구매하71 전에 30일 무료 평가판을 시험적으로 사용해볼 수 있다. 매스웍스 홈페이지에 접속하여 다운
로드 요청 양식을 작성하면 제품 전문가어洲 시험 사용에 대한 지원을 받을 수 있다, 학생이라면 ‘卜가ATLAB 및 Sim매nk 학생
용 버전'을 사용할 것을 권한다. MAT나＼B을 실행하:7뻬 앞서 설치하는 방법을 알아보자．
Keyword

I

I 사용 환경 1 설치 버전 1 설치하기 1

사용 환경

표］너 운영체제별 시스템 권장 사항
구분
해당 제품군

윈도우

매킨토시

32/64비트 MATLAB 및 Si叫川nk 저1

64비트 MATLAB 및 Sim매nk 제품군

품군
· 윈도우 xP（서비스팩 3. x64 에디션 서
비스팩 2)
운영체제

리눅스
32/64비트 MATLAB 및 Sim메nk 저1
품군

· 맥 OS X 10.5.5（레오파드）이상
· 맥 ()S X 10.6.x（스노우 레오파드）

· 윈도우 서버 2003 R2 서비스팩 2

· 우분투 9.10 및 ] 0.04 LTS
· 레드햇 엔터프라이즈 리눅스 5.x
·SUSE 리눅스 엔터프라이즈 뎨스크

· 윈도우 비스타 서비스팩 ] 혹은 2

톱 Deskt야）11.x

· 운位우 서버 2c好 서바스팩 2 혹은日2

1 데비안 5.x

디스크

SSE2 ins甘uction 세트를 지원하는 인
텔 또는 AMDx86 프로세서

프로세서

촤소 3"4GB 여유 디스크 공간

RAM

최소 4GB 이상（Sim네nk 사용 시 8GB 이상）

인텔 기반 맥(tnt이 C아e2 등）

55E2 instruction 세트를 지원하는 인
텔1 또는 AMDx86 프로세서

이 책에 실린 모든 실행 화면은 윈도우 10. tnt쇰 Core2 i7-7700 CPU. RA卜月 ] 6GB 시스템 환경의 컴퓨터에서 구동한 결과이며. 설치
버전은 MATLAB 日2015b이다，

I

설치 버전

이 책의 모튼 실습은 MATLAB R2015b 버전에서 진행했다. 八'IATLAB을 설치할 때 八'IATLAB R2015b
이후 버전을 사용하끼 바란다．

I

설치하7I

入4ATLAB을 설치하는 방법에는 두 가지가 있다. 정식으로 CD를 구매한 경우에는 먼저 八4ATLAB을 설치
할 컴퓨터의 운영체제를 확인한 뒤 인스톨러 (Installer）를 실행한다．

18

PART01. MATLAB 기본 기능 익히기

표1-2 운영체제별 설치 방법
운영체제

설치 방법

윈도우

컴퓨터에 DVD를 삽입하고 인스톨러 파일을 더볼클릭하면 자동으로 인스톨러가 실행된다．

매킨토시

컴퓨터에 DVD를 삽입하고 바탕 화면에 In밟訓Fo汁／acOSX 아이콘이 생기면 더블클릭하여 실행한다．
컴퓨터에 DVD룔 삽입하고 /path_to_由배nstall & 명령어를 실행한다. 이후 다운로드 파일이 설치되면 .力nstall

리눅스

을 입력하여 인스톨러를 추출한다．

또 다른 방법은 매스웍스 홈페이지에서 최신 버전을 구매하거나 평가판을 다운로드하여 설치하는 것이
다. 여기서는 평가판을 다운로드하여 설치하는 방법을 소개한다．

n

평가판 다운로드하기

0 https :1/＼杯vw.mathworks.com/downloads/web_downloads어］ 접속하여 평가판을 다운로드
하는 메뉴를 클릭한 후 O신청 양식을 작성하고 [Submit] 버튼을 클릭한다. O이어지는 화면에서
［入4ATIAB basics] 를 선택한 후 0자신이 사용 중인 운영체제를 클릭하여 설치 파일을 실행하거나 저
장한다．
＋恤tht幻rtw

4 MatlMTorks'

Dow砒山ds

Free MATLAB Trial

t1 C0n1a(iSU아刃d

Get S伯rted No니／ Wi由 Your Free 30-Day Tn이
Get Latest Release
G마 lEot Soh\V口r日
TrEMOR)巴 出m力沚 a닙
0m甘nm(b

R2019a

小

小

=

山 包） i

刃 口ei肛 a my
1 蜘d0的 m 口出1刃

ma

L叩m아

CMOe.艸1

"

'

,""" "

00 化如

P에Cy

니11d11Pr0d나口t10n1yt01Va山m1m1n1fm

Am V에 o, bd. e出
Y0J5Crm呻叩nVH托h싸녀Err如너寸七

1司a0ree

..L,,*，여
,,叫沁引呼畔 玎＝n
V

I

m0rman0n 니1
「e0U1 口nVaCy 머기（／幻rde1訓5

+Math\'Urkc

,

+m曲Vbrk母

吃

人

中

Free MATLAB Triof

Get Started Now with Your Free 30-Day Trial

D帥Iood 52019rr u ").urOrM'rre) .E
D0m卄md m녑 nm mm kmtH11r

!

4

"'

1t

r km
mm 9q까如 띄m m 月
m心너m m h 거녑 蜘
kaae d
8鈿

Select 口 Tn이 九吐四訂or沁나n이｝d

出六d y미11mm

玲

d21 Ct거山d 뇩甘1n1

1 마m口e甘m）口뇨d1 如J넙
比由4m m1m m11m 1叫

I.岫JLI,kr

-,
니 do누3

R20伯a Sy出m Reqt川em七nn

· Hm d口 1 h出놔1 d나 m어tm工11 aM

V比나mb出m=bmmNm1d

:-5,

R;m19aL巾dUd11Ph1m1=e卜h加1

呻

Lamn Crm HAnJ咽 Mdn나4y mm
月Ced mJ1e
dU1m1也 느叫m브m m｛

\

"m
『 '曲"四

［旬 二器忿密 "M
m h1md5甘d5y늬em'

노마, i&ATLkBNr나
1

娑芬i
:}:1客二珏；「；／可번

茗밖5-Is"蜘-

Dh(0叱『II, td,IrI

RUmh미n5m녑；am rD匕Wme 引emm
山m1口1d y口U1 HCen5e aM neW
m너啞1

Cmmm1口I- 끼mtnm 미月긔兵a너
b啣
m m 1 H1巾的杜m
如月m在

' 呻m " “帥 "
H小느4m立m蜘片HU川m1)

느14거니 거y口시31니가？

-a

斗p自 H m1口

CHAPTER 01. 처음 만나는MAT녀B

19

目 설치 방법 선택하71
入4ATLAB을 설치하는 과정에서 인터넷 연결을 사용할지 여부를 선택한다. 여기서는 인터넷을 사용하여
MATLAB을 설치해보자．
+.,코hi心口出t0스든eJ

口

0

S겉旦塑 M斜년呱K·

[ ' 짧茗：::：幻" " "
OPR묀 쏘치 키甲妃 m1翊相SOT Ft功 사뮴 파社 二치 ! 드묘맏
인터多 면ioI i요 멈뮴

Math뾔며ho 머odiUts tiC peG作0.1 by points (A的 n1小bet口卄玉C口n1／口.SSR]] teed eepytlM
甘町 By intenT5 let口 甘比 Soft나ace Linen汗 A甲.0,1.0TH日t 似ALeS YeS WA 出5口 agme t0
心dm0r녜 i.thlcnr00000y에r U5e 于 tht鉀 m口們net. My undUtheitEld tier叩.edt,ERMr. PR
出5tn느n席口nmay Out Cmii and (dm100 pen카mi
ATAPRM ond 듸m네tithe itS以m叱 n的emaiitolTheMWAt畔MR IT( 하ea5e me
mathYd口AeEotIStEdert크It 幻h aiNt Of t的蜘nal Intl미기却比 아Yen plod岵 Of brand nameS
115 be badtnna作5 丁 m9 in肝.1 bed.t,t.eb드 elmS引rneoptyt知IS미don]

m

m

i. _

mf=

..1 Matl*NboeL,

日 소프트웨어 라이선스 동의서 확인하:il
O소프트웨어 라이선스 동의서 (Software License Agreement)의 내용을 살펴보고, O그 내용에 동의
한다면 '여］'를선택한후［다음］ 버튼을클릭한다．

n키Sib TUE 駐ntd꿔SIR ICES또 札R珏hi日IT (THE "1.GR뜨서日In OFT｝在 MATH呻心 INC 기dAn｛呻工S.) 曲
THE PROGRAMS TO矩 PROS只A,市 立RE I（日心日工 NOT S아｛) 姓AD 了GE TERMS ANT CONDTO아us on TAdS
AG只旺NEOn CAMERA止no日
（現ECOT싸(NO, iNSTA山NO. OR US싸flOE P烈兀RAMS. OCR INFORMAT]마d 1BDtFr
Y1거ti LIE日姑E 어：PERSIA CON引凡ISlE PROGRAM OFFER]?나GSUITE PR匹日unto aense TUE *더止EMENT
TUE AURROP在NT REPR匹日iTS THE ENTiRE HARlEM日AT RAT出EON GO]] (THE UCE小珏lAND Miii中螂is
CO艸旺mn샤S YOUR tuG卜｛ES 0015묘Au 如LOUSE THE PROGRAMS UI虹乂只 Ti任 UCENSE 0朴0R]忖Un어I ACOT月EL
0013 loiS了 虹 C日T T｝任 T田1才5 아 TH巧 Ac只ERR日AlTO CORn, 入STALL OR USE THE PROGRAMS ii IOU［兀 NO
肛cOPInGS LIC日好ETGTUt5. THET니 nCR] MUST RIM日0시｛LUST아'U듸NO THE PROGRAMS
IF YOU TEEMInLATE 114冬 UCEWSE T0

口 설치 정보 제공하71
O매스웍스에서 만든 계정의 정보를 입력하면 다운로드한 평가판의 라이선스 정보까 나타난다. 그중 하
나를 선택하고 0 ［다음］ 버튼을 클릭한다．

C) 븍1口1 之는 라이선스뫼 I썽파 키 밉 다．

旦쏘 LflU 라머선스 = ；차로투터 받으

20

PART 01. MATLAB 기본 기능 익히71

日 설치 경로 지정하기
八4A皿AB을 설치할 경로를 지정한다. 기본 설치 경로는 C:\Program Files＼八4ATLAB\R2019a이지만
이는 사용자의 편의어］ 따라 변경할수 있다. 방법 1 0 ［짖아보기... ] 버튼을 클릭하고 설치 경로를 지정
하거나, 방법2 직접 설치 경로를 입력한후O［다음］ 버튼을클릭한다. 여기서는기본설치 경로로설치
폴더를 지정했다．

71
日 설치할 제품 선택하:
O설치할제품을 선택한후 0 ［다음］ 버튼을클릭한다．
小

小 斗I 선텍
I지V 끼I 신닉
7

)

고

m1

口a }n1지m1!J
目 口mMA

知쁘쁘 l트흐
旦＋쓰쓰빤쁘J9햇呼姐
日 5心m川 P以的四TTCIbQX 82
日 引pEveflts 56
돠m1C1阡 '-5
S5.M66 l 00

昌

다욘로드 i요
다욘토드 크묘
다포토드 i요
다포로드 i묘
다포로드 t요

叫

m

口

x

M饌k壤，,,..

나由1蜘收于

口 설치 옵션 선택하기
O바로가기를 어디에 추가할 것인지 선택한 후 0 ［다음］ 버튼을 클릭한다．

V하七！치 V신 신쩍
7F

MATLAB"
人닒MULINK"
1205知

MARAS 가신Oil召하'I
口 더 걔선된 MAT나B이 니I 수 있됴4 사I자 01 겅뵤186帥Wm4 전古名니80
자세히 함하보' 0

CHAPTER 01. 처음 만나는 MATLAB

21

回 설치 환경 확인하'I
지금까지 선택한 설치 환경을 확인한다. 설치 환경을 바꾸고 싶다면 ［뒤로］ 버튼을 클릭하여 변경할 수
있다. 설치를계속진행하려면 ［설치］ 버튼을클릭한다．
+

가인

m

1치 I더：
亡mm07mm 디As甘MAR43쀼620 91
다묜토드 크7l4烈片MB
甘치 크기：'4月O2MB

口

x

M, TLAB'

s11너ULII따（"
R2아叱

끼g:
MATUB 3.6(93묜로드）
듸p911mnB 93（다욘로드）
Cant이 5朴ten, ,口이669t0七따욘 드）
DSP Syt相PT rAo91aa 98(99욘로드）
S1}M 미n＜們引凹 T唎bOA 82工｝문로드）
듸mEtes心 St｛다욘로드）
Sim叱켜片 4,6｛다묜도드）
"staT메 too（다묜로도）

日 설치 완료 후 활성화하71
정상적으로 설치되면 설치 완료 칭히 나타난다. MATLAB을 사용하기 위해 라이선스를 확인하는 과정을
활성화（act押ation）라고 하는데, 이를 위해 0 '入4ATh&B 활성화'가 체크되어 있는지 확인한 후 0 ［다
음］ 버튼을클릭한다. 0활성화어］대해 설명한칭미 나타나면 ［다음］ 버튼을클릭한다．

I쳐가 뫈료되몄e니다．

Mat枷665 소프트I어 I첨파

召고 소프트I머11섬희司야 s6ATLBAI 사뮴I 수 밌e니다．

1셤촤（ACUV川幻n）는 리이선스'F 부며된 MItOW여499
'丹 사뮴I 가인하는 프로I스밉니다 이
프로上t스0148눈 라이션스의 뮤I섶I 컴사따고 Jig차기 구36한 라미선스아서 선쩍 가늉한 각 仁
지 욤션51서 허가된 사스딤 I侄파 가늄 契수* 초과66지 匹는지 가민험니CF

陋ATLAS卿p

E可 활성화한 라이선스와 사용자 정보 확인하기
활성화한라이선스와사용자 정보를확인한후 ［확인］ 버튼을클릭한다．
+6땐
선쩍 ＝언：
: 6294429
자：t3nlC6snb比taBs
이 정보가 M故ttW며虹토 젼台딤니디

22

PART01. MAT나＼B 기본 기능익히기

MATLAB
, 1MULH나（"

fl u 활성화 완료 후 MATLAB 실행하71
활성화가 완료됨으로써 MATLAB의 설치가 끝나 MATLAB을 실행할수 있다．

CHAPTER 01. 처음 만나는MAT녀B

23

LESSON

03

M酊LAB 실행하고 종료하기

MATLABO I 컴퓨터에 설치되어 있다면 다른 응용 프로그램을 실행할 때와 마찬가지로 MATLAB을 실행하고 종료할 수 있다．
설치한 MAT나＼B을 실행 및 종료하는 방법을 알아보자．
Keyword

1 ［시작］메뉴에서 실행 1 바탕화면에서 실행 I MAT녀B종료 1

MATLAB 싶행하71

I

八IIATIAB을실행하려면 방1

［시작］1［컴퓨터］H［로컬 디스크（C:)］를클릭하여 [八4ATLAB] 디렉터

리 그룹을짖아 선택하거나，

바탕 화면에 있는 바로가기 아이콘을 선택한다．

［시작］메뉴에서 실행하71
入4ATLAB을 실행하기 위하1 ［시작］ ［컴퓨터］1 ［로컬 디스크（C:) ] - [Program File引- [Matlab]
[R2o15b]-田in] 메뉴를 클릭한다. 入'IATLAB 로고 寸IT岫b 를 클릭하면 MATLAB 실행 화면이 나타
난다．

바탕 화면에서 실행하71
八IATLAB을 컴퓨터어］ 설치하면 바탕 화면어］ 바로가기 아이콘이 자동으로 생성된다. 바로가기 아이콘을
더블클릭하면 MATLAB 실행 화면이 나타난다．

I

MATLAB 종료하71

人IAThAB을 종료하려면 방법 ] 실행 화면 오른쪽 싱단의

［닫기］ 버튼을 클릭하거나， 방법 2 皿I

+ [1刃 키 또는匣可 +［희 키를 사용한다. 또는 방법 3 다음과 같이 명령 창의 프롬프트（力）에서 qu仕 또
는 ex仕 명령어를 입력하여 MATLAB을종료한다．

>> exit

24

PART01. MATLAB 기본기능 익히기

LESSON

04

MATLAB 화면 살펴보기

MATLAB 실행 화면을 구성하는 요소의 이름과 역할을 잘 알아야만 MATLAB을 제대로 사용할 수 있다. MATLAB을 배우기
에 앞서 MATLB 화면을 익혀보자．
Keys川ord

I

1 전체 화면 구성 1 세부 화면 구성 1

MATLAB 전처1 화면 구성

MATLAB의 전체 화면은 다음과 긷미 네 부분으로 나눌 수 있다. a 명령 지시 부분으로 제목 표시줄, 메
뉴 표시줄, 현재 폴더 상자 등이 있다. 日 현재 폴더 창으로 M肛'LAB 작업을 실행하고 저장한 파일을 보
여주며 그 파일을 찾는 뎨 사용한다. 日 명령 창으로 MATLAB 명령어를 입력하고 실행할 수 있는 영역을
보여준다. a 작업 공간 창으로 현재 진행 중인 MATLAB 작업에서 사용하는 임의의 변수 및 배열의 이름
과값을보여준다．
"+MAT녀S R201.tb. academicuse

/

PLOTS

) 肛

; n，夕多

New Variabu}
Mew
!

S口en
-

戶 Coetnare

ttAOrt
Data

Save
Workopaca

二 느三

斗J 甲

n ii

Current 日깃Tier

'

'
, C匕arWortapace

SAC汭夙A

卜 C 卜 마o. tarn F引七5 卜 MATLAB 卜 R2015b 卜
｛니

卜始me y

Y

나
\ / C1earCorreeOands !

; m4m느毛小口

0旺泛

묘

씨P
더

Lm

.ER
；이 마eferPn.

Satrukrk
山e出y

Layovt
!

=
td1 Perolel

1$1M바a?心4.

n
Art小dna

ENVURONRENT

巧

He如

> Recuest Sup口Oat
A드SOunDED

in 卜

마舟
Workspace

可

>> a = 3口
스

重！

二 ADD.Stx
包 사Sri.밗X
圃曲pit가a刈.bat
幼Fig2_3.m
邕 lcd吼a.xrnl
H Icdata工sd
邕 IcdatautfBxmi
4 matlab.exe
國m帥的at

寸 Ann卜／7eCode

I
H
dO b = ［니 0 II

日

訊，

Me나
ScrAt

理如납轟g 1 主二뇨醫小斗珏叫
中i

APPS

口

r
V

Deta出

Select a n陌 to 너ew d叭a出

q

}
ft

. >>

,
기

그림］너 M月TLAB 전체 화면

CHAPTER 01 처음 만나는 MATLAB

25

명령 지시 부분
명령 지시 부분은 제목 표시줄, 메뉴 표시줄, 도구 모음, 현재 폴더 상자 등으로 구성되어 있다. 대표적인
구성 요소의 명칭과 기능은 다음과 같다．
0 제목 표시줄：프로그램명을 보여준다．
日 메뉴 표시줄小4ATh&B에서 사용하는 명령어가 메뉴별로 구분되어 있다．
日도구 모음：많이 사용되는 메뉴를 아이콘 형태로 보여준다. .
口현재 폴더 (Current F이der) 상자：현재 폴더 경로를 보여주며 간단한 방법으로 변경할 수 있다．
日문서 검색 창小t&TLAB에서 사용하는 문서의 내용을 찾을 수 있다．

0
日
日
口
그림卜2

명령 지시 부분

현재1 폴더 창
현재 폴더 (Current 恥ider) 창은 현재 폴더어］있는 파일을 보여주는 영역과 선택된 파일의 정보를 보여
주는 영역으로 구성되어 있다. 대표적인 구성 요소의 명칭과 기능은 다음과 같다．
Current Folder
Name 小

0

包 ADD引x
[I ARIfl.slx
團 depk如ol.bat
固 Fig之3.m
：竺blcdata'xml
山 lcdata．好d
L‘邕lcdatautf8.xml
4 matlab.exe
國 mbuild;bat
V

DetaiFs

日

S쉬ect a file to 니e네 deta出

0 파일 목록：현재 폴더어］있는 파일을 보여준다．
日 정보：선택된 파일의 정보를 보여준다．

그림卜3 현재 폴더 창

명령 창
명령 창（Command 싸indow）은 입력한 명령어와 함수를 실행한다. 명령 창에는 力 기호가 나타나는데
이를 프롬프트（pron巾t）라고 한다. 이 기호는 키보드로 입력한 MATL&B 명령어를 즉시 실행할 준비가

26

PART01. MAT녀B 기본 기능 익히기

되었음을의미한다. 프롬프트뒤어］실행할명령어를 입력하고 Enter 키를누르면새로운 입력을기다리는
프롬프트가 다시 나타난다. 같은 방법으로 필요한 명령어를 계속 입력할 수 있다. 이때 이전에 입력한 명
령어는 현재 사용 중인 명령 창어］계속 보관되고 유지된다．
口LI) 명령 창에 dc 명령어를 입력하면 명령 창의 모든 내용을 지울 수 있다．

작업 공간 창
작업 공간（玳Torkspace) 창은 현재 진행 중인 작업에서 사용하고 있는 임의의 변수 및 배열의 이름과 값
을보여준다. 대표적인 구성 요소의 명칭과 기능은 다음과같다．

wo(Icspace

0

Name 4

Va山e

日a
크b
E크C

30
卜1,0,1]
卜30,0,30]

4

1

111

1

0 작업 공간 정보：현재 작업에서 사용하는 모든 변수, 배열의 이름과

卜

값을보여준다．

그림卜4 즈J업 공간 창

El11 명령 창에서 clear 명령어를 입력하면 작업 공간 창의 모든 내용을 지울 수 있다．
r clear: 작업 공간 창에서 모든 변수를 지운다．
* clear 변수 이툼：작업 공간 창에서 해당 변수를 지운다．
· clear a比 작업 공간 창에서 모든 변수. 광역변수, 함수 등 모든 정보를 지운다．

명령 창의 기록 보기
八1ATLAB을 종료한 후 다시 八LATLAB을 실행하면 이전에 작업한 명령 창의 내용이 보이지 않는다. 그러
나 명령 칭에서 키보드의 田키를 누르면 이전어］명령 칭에 보관된 기록을 보여주며, m 키를 한 번씩 누를
때마다 이전어］입력한 명령어를 역순으로 볼 수 있다. 그리고田키를 한 번씩 누를 때마다 다시 최근어］입
력한 명령어를 볼 수 있다. 또한 키보드의 日 , 日 키는 일반 문서 편집기와 마찬가지로 글자의 앞뒤로 이
동하는 뎨 사용한다．

I

MATLAB 세부 화면 구성

入4ATLAB에서는 기본 실행 화면과는 별도로 그림 (F培ure) 창, 편집 (E小tor) 창, 시뮬링크 라이브러리
브라우저（Simu如kL小raw Browser), 변수편집（Variable Ed妃or) 창, 비교툴（Comparison To이）
창등이 사용된다. 이 책에서는주로 그림 창, 편집 창, 시뮬링크 라히브러리 브라우저를사용한다（시뮬링
크 라이브러리 브라우저는 13장에서 설명할 것이다）. 이 중어써 그림 창과 편집 창을간략히 살펴보자．

CHAPTER 01. 처음 만나는MATLAB

27

그림 창
그림 창은그래프를출력하기 위한창으로, 그림 창을 여는방법은4장에서 설명할 것이다. 대표적인 구성
요소의 명칭과 기능은 다음과 같다．
0 제목 표시줄：그림 창 이름을 보여준다．
日 메뉴 표시줄：그림 창에서 사용하는 명령어가 메뉴별로 구분되어 있다．
日 독（Dock) 버튼：그림 창을 MATLAB 실행 화면에 포함하여 보여준다．
口도구 모음：많이 사용되는 메뉴를 아이콘 형태로 보여준다．
日그래프 결과：그래프 결과를 보여준다．

n日日

=

莖叱ure I

［늬」
＝

址

1日te Ed艮 V仁w 批est To어＄Desktop 네ind애 H미

日
［d

t그 d a 企 自 小＼＼好 自咀 a卜目 口自石面

1

引nus이dat SIgneI: A亡0叫口Jn+e)
C) L)

.

日

0.8

:

O

6)

0.6

m

O

0.4

O

O

0.2

1

尋 0

I

.0.2

/\

1

4l4(b

'

-0.6

O

O
戶느

'

口．

m

‘文「m

1

O

0
0

2

O
1

4

6

8

10
12
Time En]

14

16

18

20

口t二1

그림卜5

1

그림 창

편집 창
편집 창은 스크립트 파일을 작성하기 위한 창으로, 편집 창을 여는 방법은 2장의 'Lesson 01'어꺼 설명할
것이다. 대표적인 구성 요소의 명칭과 기능은 다음과 같다．

0 吃 Ed1tor Unt띠ed
UntTtled

1

0 제목 표시줄： 편집 창 이름을 보여

日

준다．
日 입력 부분' 스크립트 파일의 내용을
입력한다．

그림卜6 편집 창

28

PART01. MAT나＼B 기본 기능 익히71

LESSON

05

자료 저장하기

명령 창에 입력한 자료를 임시로 저장하고 불러올 때 사용하는 명령어를 살펴보자．
Keyword

I save i load I

I save
현재 작업 공간 창어］나타나는 모든 자료를 임시로 저장할 때는 save 명령어를 사용한다. 다음은 명령 창
에서 data라는 이름으로 자료를 임시로 저장하는 과정이다．
Command Vendow
>> x=2七3

二
>> y=2日

Nan始 A

Vali片

Max

Mn

5
-1

5
-1

5
l

a> save data

그림卜7 sa＼尼 명령에 실행 결과와 작업 공간 창

I load
임시로 저장한 자료를 불러올 때는 幻ad 명령어를 사용한다. 幻ad 명령어를 사용하면 명령 창에는 다음
입력을 기다리는프롬프트（力）가 나타나고, 작업 공간창에는불러온자료가 나타난다. 다음은 명령 창어］
서 임시로 저장한data라는 자료를 불러오는 과정이다．

>> 1 cad data
a>
V퀴ue

Max

Mci

5
1

5
-1

5
-1

그림卜8k出 명령에 실행 결과와 작업 공간 창

CHAPTER 01. 처음만나는 MATLAB

29

LESSON

도움말 명령에 사용하기

06

MATLAB은 다른 컴퓨터 프로그래밍 언어에 비해 다양한 내장함수를 제공한다는 것이 가장 큰 장점이다. 이런 함수의 정보를
알고 싶을 때 사용하는 도움말 명령어를 살펴보자．

1 he巾 I doc 1 Iook幻r 1

Keyword

I

he巾

함수명은 알지만 함수의 기본 정보를 모를 때 he巾 명령어를 사용한다．
1 （川저Il_ I I
[1二：二： - I
he恒 명령어를 사용하여 tan 함수의 기본 정보를 확인하라．
系i

晤과같' ] 입력가고I玉a키를누르면帥斟의기본정보가명령各뇌］나타난다
. 기본정보에는tan
함수의 기본 입력 혁태．학수와과려되 힌닉그 두．이 平하되i-i-

'> help tan
tan

Tangent of argument in radians.

tan(X) is the tangent of the elements of 0.
See also aTon』 atan2』 tand. atari2d.
Reference page for tan
Other functions naned tan
그림卜9

30

hel ) 명령에 실행 결과

PART01. MAT녀B 기본 기능 익히기

I doc
함수의 기본 정보뿐만 아니라 더 상세한 설명과 간단한 예제를 보려면 doc 명령어를 사용한다．
1 예제 1- 2 [
doc 명령어를 사용하여 tan 함수의 상서1 정보를 확인하라．
=

百UI

명령 창에서 ' 力 面C姐n'을 입력하고 E쿄a 키를 누르면 다음과같이 tan 함수의 상세 정보가 인터넷 브라
우저에 나타나고 활용할수 있는 관련 예제도 함꼐 보여준다．
乍 4 企 背' O
m 아加r 出e5

三

田 띠 日回

' mn 니브

n 斗rttb的oT4p

C아町ENdS

tan

( A1F가m1比tg
<MATLAB

0

'Malt比mm卜CS
lEAnlentany Math

T가母enx of a띠U口ent in rati日nS
Syntax
Y = tam;X1

(TI口t月H川1e하
ta n

SinCa )
00001甲Ion

口m

Dea亡n1比幻in
Y =toniC) na缸tnr the tangentoneath elefflelltota. Ther. etndlon 0口0reirs 叫ement-war en arrads T坦
幻nr如n accee四 both real and cornS已
（m叫包 Forte키 Ya山eS 아 X n me n由trail-let mc :a尸 re山m5 rea
Ya山C5 in the interval )-lrt,lnT Fore口m口g( Ya山eS 아 X tdn m山m5 C0m이e1 Ya山Is Allan여cc are in ra OaTs

I

Eoam미eS
i 't0ut 409Utttefl各
C山中Ut bogumen匹
Mona About
See pdso

Examples

如d

! 디Ott가）9터吐 F니nCh미n
F기아the tangent tunoben eo凹寸｝edoe니n1 t／
그 드 i 드 n/2

1

i = （小i/a）也eL已BI:(ri/ 2)S. S1;
plot（자t甘
（eli. Videe

그림卜］0 （幻C 명령에 실행 결과

CHAPTER 01. 처음 만나는 MATLAB

31

I

look化r

앞서 배운 he巾 명령어나 doc 명령어의 경우와달리 찾으려는함수명을 정확히 알지 못할 때 lookfor 명
령어를사용한다. Iookfor 명령어를 사용하면 찾으려는 정확한함수명은물론이고 입력된 영문 철자가포
함된 함수도 함꺼］나타난다. 마치 카드놀이의 조커처럼 와일드카드（wild-card) 기능을 하는 것이다．
1 예제 1- 3 1
tangent 값을 구하는 함수를 사용하려고 할 때, look化r 명령어를 사용하여 관련 함수를 찾아라．
二＝
코돋"I

다음과같이 입력하고 [교I 키를누르면 ' tangent '라는 철자가포함된 함수가 명령 창에 나타난다. 함수의
이름을 클릭하면 그 함수의 기본 정보가 lookfor 명령에 실행 결과의 아래쪽에 나타난다．

>> lookfor tangent
acot
acutd
acoth
atan
atan2
atan2d
at and
at anh
cot
cotd
ruth
tan
tand
tanh
f i apt_atan21dego
cord i catart2
dtansin

- Inverse cotangent, result in radian.
- Inverse cotangent, renult In degrees.
- Inverse hyperbol ic cotangent.
- Inverse tangent, reoult in radians.
- Four quadrant inverse tangent.
- Four quadrant inverse tangent, result In degrees
日 Inverse tangent, result In degrees.
- Inverse hyperbol ic tangent.
- Cotangent of argument in radians,
- Cotangent of argument in degrees
e 巾pa比ol lc cotangent,
- Tangent of argument in radians
- Tangent of argument in degrees
= 山pg比ol Ic tangent
- Calculate Fixed-Point Arctangent
- CF{)IC-based four quudrant inverne tangent.
- 汁／perbol ic tangent sigmoid trannfer derivative function

그림 1-11 look幻r 명령에 실행 결과

El1} MATLAB의 명령어와 함수는 다음과 같이 구분한다．
· 명령어는 기본적으로 괄호 없이 단독으로 사용한다．
· 명령어에 괄호를 사용하는 경우는 문자열을 작은따옴표 사이에 지정하고 이 문자열을 출력한다．
· 함수는 괄호 안에 입력 인자（숫자 또는 배열로 지정된 변수）를 입력하여 해당 함수를 계산한 결과를 출력한다．
· 함수에서 여러 개의 입력 인자를 지정할 때는 콤마로 분리한다．

32

PART01. MAT녀B 기본 기능 익히기

CHAPTER

명령어를 담는
스크립트 파일

CONTENTS
LESSON 01 스크립트 파일 생성하고 실행하기
LESSON 02 현재 폴더 변경하71

LESSON

스크립트 파일 생성하고 실행하기

01

스크립트 파일을 생성하려면 메모장이나 편집 창을 0용한다．0陣 명령 창에서 스크립트 파일명을 입력하면
파일을 실행할 수 있댜. 스크립트 파일을 생성하고 실행하는 여러 가지 방법을 알아보자．
Keyword

생성한 스크립트

1 스크립트파일（M파일） 1 편집 창 1 메모장 1 주석 1 디버깅 1

자료와 명령어를 입력하는 방법은 두 가지이다. 방법］ 명령 창어］ 직접 자료와함수／명령어를 입력하면
작업이 완전히 끝나기 전에 중간 결과를 볼수 있어 작업의 정확성을 높일 수 있다. 방법 2 스크립트 파일
을 작성하여 입력하면 모든 함수／명령어를 알고리즘（a坦아妊hm) 에 맞게 코딩한 뒤 MATLB 파일어］ 저
장하고 한꺼번어］실행할 수 있다．
스크립트 파일은 MATLAB 함수／명령어를 포함하는 텍스트 파일로 확장자가 .m이다. 그래서 스크립트
파일을 M파일이라고도 한다. 스크립트 파일을 생성하려면 방법 ] 入4ATIAB 명령 창 안에서 제공하는
편집 창을이용하거나, 방법2 일반문서를편집할수있는메모장을이용한다．

스크립트 파일（M中파일）

스크립트 Me파일

함수 Mm파일（사용자정의함수）

그림 2너 스크립트 파일의 종류

스크립트 파일은［그림 }1］과 같이 두 가지 종류가 있다. 스크립트 M파일은 MATLAB 명령에, 수식，
변수, 내장함수, 사용자정의함수 등을 포함하며, 명령 창에서 스크립트 M파일을 실행하면 해당 파일어］
작성된 순서대로 명령을 수행한다. 그리고 함수 M파일（사용자정의함수）은 입력값혀］대해 원하는 값을
출력하도록사용자가 직접 함수를 만든 것이다. 함수M-파일을생성하는 방법은 5장에서 설명할 것이다．

I

편집 창을 이용하여 스크립트 파일 생성하'I

편집 창 열'I
먼저 편집 창을 열려면 MATLAB 명령 창이 열려 있는 상태에서 [HO毗］-[New］中［Script] 메뉴를
클릭한다. 이때 [HOME］에서 [EDITOR］로자연스럽게 이동한다．

34

PART 01. MATLAB 기본 가능 익히기

스크립트 파일 저장하기
저장된 파일이 없는 새로운 편집 창이 열리면 편집 창 안어］ 스크립트 파일의 내용을 입력하고 [Save] 머］
뉴를 클릭한 후 새롭게 열리는 [Selected File for Save As] 창의 ［파일 이름（N) :］어］ 저장할 파일명
(file）을 직접 입력한다. 그러면 확장자가 자동으로 생성되어 [Curret止 Folder］에 file.m 파일이 저장
된다．

스크립트 파일 불러오71
이미 저장된 스크립트 file.m 파일을 다시 불러내어 확인하거나 수정할 때는 방법 ]
[Open] 메뉴를클릭한후 ' file.m'을 선택하거나， 방법 2

[HOME] -

[Current Folder] 창어］ 있는 ' file.m'을 더블

클릭한다．

1 예工112-1 I
편집 창에 다음 그림과 같이 입력한 후 스크립트 파일로 저장하라 ．저장할 때1 파일명은 'script] ' 로 하라．
풀이

스크립트 파일명을 저장할 때는 파일명 뒤의 확장자가 . m인지 확인한다．

ii 丘nptl.m

브I

A = 1 2 3;4 S S;7 891;
A = Ii 2 3;4 5 6;7 8 91
= lL2,3;4,5,6;7』日, 91

A

卜45

12-

그림 十2 scriptl.m

ni}

명령 창과 편집 창에서 명령어와 함수를 입력할 따1 다음 사항을 주의한다．
0 MATLAB은 대문자와 소문자를 구별하여 사용한다．
0 변수 이름을 입력하면 현재 변숫값을 명령 창에 보여준다．
0 명령문 끝에 세미콜론(;)을 입력하면 변숫값이 명령 창에 나타나지 않는다．
0 변수 또는 함수 이름을 입력하던 중 i西 키를 누르면. 작성된 이름으로 시작하는 변수명과 함수명의 목록이 보이는 자동 완성 71
능이 실행된다．

I

메모장을 이용하여 스크립트 파일 생성하71

메모장을 실행하려면 ［모든 프로그램］H［보조 프로그램｝
［메모장］ 메뉴를 클릭한다. 메모장히 열리면
스크립트 파일의 내용을 작성한 다음 파일명 뒤에 MAUAB 확장자（.m)를 붙여 저장한다（여］:file.m).
또한 저장한 파일을 컴퓨터어］ 보관하는 디렉터리 (directory) 확인도 중요하다. M-파일은 MATLAB을
설치할 때 자동으로 설정되는 서브디렉터리 (subdirectory) ［로컬 디스크（c:)] > [Program Files] >
［入4ATLAB] > [R2015b] > [bin] > file.m으로 보관되거나［문서］> ［八'IATLAB] > file.m으로보관된다．

CHAPTER 02. 명령어를 담는스크립트파일

35

주석 작성하기

I

스크립트 파일의 내용을 쉽게 이해하도록 풀어 쓴 글을 주석 (C帥ment)이라고 한다. 주석은 명령에 실
행에 영향을 미치지 않으며, 다른 명령어와달리 초록색으로 나타난다．

71
주석 처리하:
방법］ 한행 또는한행의 일부를주석으로처리하려면주석이 시작되는위치어］퍼센트mb) 기호를삽입
한다. 방법2 여러 행을주적으로 처리하려면 주석으로 처리할코드를마우스로드래그한후 回 +［司
키를누른다．

주석 해제하기
방법 ]

주적을 해제하려면 주석 시작 부분에 있는 퍼센트 기호를 지운다． 방법 2 여러 행의 주석을 한 번

어］ 해제하려면 주석을 해제할 코드를 마우스로 드래그한후匹回 +［뢰 키를 누른다．
LI F也口m 弑降身

i nt_a = 1 ;
mnt上 = 2;
sum = i nt코 + I ntb;

] 中
23 -

呈 nt_a메 1믈 지점한다，
茗 m t上메 2를 지졍한다．
茗 두 변수의 합을 sum메 지점한CL

4-

그림 2心 주석을 삽입한 스크립트 파일

I

스크립트 파일 실행하기

스크립트 파일을 실행하려면 먼저 스크립트 파일이 저장된 경로를 현재 폴더로 변경해야 한다. 현재 폴더
를 변경하는 방법은 다음 레슨에서 자세히 설명할 것이다. 방법 ] 저장된 스크립트 파일을 명령 창에서
실행할때는확장자（.m)를제외한파일명만 입력하고日回1 키를누르거나, 방법2 편집 창에서 [Run]
메뉴를클릭한다. 또는 방범3 편집 창에서［回키를눌러 스크립트파일을실행한다．

1 ｛계저1 9m9 1
L二二二二m二J

M-F加 i SC까）tl.m

［예제 2-1]에서 저장한 스크립트 파일 scriptl.m울 명령 칭뻬서 실행하라．

풀이

저장된 스크립트 파일을 실행할 때는 먼저 현재 폴더어］해당 스크립트 파일이 있는지를 확인한다. 만약 스크
립트 파일이 현재 폴더에 없으면 스크립트 파일이 저장된 경로로 현재 폴더를 변경해야 한다．
저장된 스크립트 파일을 명령 창어써 실행할 때는확장자（in)를 제외한파일명 ' script1'만 입력하면 된다．

36

PART01. MATLAB 기본 기능 익히71

Command Window

(9

>) scriptl

A

1
4
7

2
5
8

3
6
9

1
4
7

2
5
0

3
6
9

=

그림 午4 scnpt1.m 실행 결과

I

스크립트 파일 디버깅하7J

디버깅 (debugging）은 일반적으로 프로그램의 오류를 발견하고 수정하는 작업을 말한다. 스크립
트 파일을 디버깅하려면 검사할 행을 표시하는 중단점 (breakpoint)을 설정해야 한다. 중단점을 설정
하려면 중단점을 설정할 행어］ 마우스 커서를 놓고 방법 1 I目 키를 누르거나, 방법2 편집 창에서 圄
[Breakpoints] - 咽［Set/Clear] 메뉴를 클릭한다. 중단점이 설정되면 그 행에 빨간 동그라미가 나타난
다. 중단점을 설정한 다음 편집 창에서 必 [Run] 버튼을 클릭하거나［回키를 누르면 스크립트 파일을 실
행하고 디버깅할수 있다.

2
4
6 7 8
0
U
二
口
n
U
0

UF3g25.m
xJ +l
1 epsi lon0 = 巳田如너2;
H
-

a

Q =4e.-9;
S= O. 02;
d =1e-3;
Ds =Q/S;
凡ste口S = 200;
ds = d/x. .steps;
Le = 0;

1

! 무' " " ::;;；客二：-1).dx;

-

S.

2*

=

e:

-

epsi lon,
epsl lon0.(2+ x*x.
dv
106) ;
e = ds; 2.dv) /(2.epsi l。
= We
dl_
n) ;
(Ds

-

d_

-

Ie

11
12
1314
15
16I?

end
C = 寸2/(2네그） ;

그림 十5 중단점이 설정된 스크립트 파일

중단점을해제하는방법은중단점을설정하는방법과같다（켜기／끄키）. 단, 편집 창에서 [Breakpoints] 稠 [Clear A川 버튼을 클릭하면 모든 중단점을 한꺼번에 해제할수 있다．

CHAPTER 02. 명령어를 담는스크립트파일

37

LESSON

02

현재1 폴더 변경하기

특정 위치에 저장된 스크립트 파일을 실행하려면 현재 폴더를 스크립트 파일이 저장된 경로로 변경하거나 추가로 지정해야 한
다, 현재 폴더 경로를 변경하거나 추가로 지정하는 방법에 대해 알아보자．
Keyword

1 cd 1 addpath, rmpath I 현재폴더 상자 1 현재폴더 창 1

MATLAB 명령 창 이용하'I

I

현재 폴더 경로 변경하:7'
cd 명령어를 명령 창어］ 입력하여 현재 폴더의 경로를 변경할 수 있다．
力 cd E:＼八4y八4atlab

현재 폴더 경로 추가 지정하71
명령 창에 addpath 명령어를 입력하면 현재 폴더의 경로를 추가로 지정할수 있다. 이때 현재 폴더는 변
경되지 않는다. 또한rmpath 명령어를 입력하면추가로 지정한현재 폴디의 경로를해제할수 있다．
力 addpath E:＼入lyMatlab
力 rmpa仕1 E:\My入Tatlab

I

현지1 폴더 상자 이용하기

명령 지시 부분에 위치한 현재 폴더 상자를 이용하여 현재 폴더를 변경할 수 있다. 현재 폴더 상자에서
현재 폴더를 변경하려면 방법 l
방법
방법2

경로L7} 표시된 경로 표시줄을 더블클릭하고 변경할 경로를 입력하거나，

珂 버튼을 클릭하면 나타나는 새로운 폴더 선택하기 창에서 현재 폴더를 원하는 경로로 변경한

다. 또는 방법3 囹 [Up One Level] 버튼을클릭하여 현재 폴더를상위 폴더로 변경한다. 이를그림으
로 간단히 나타내면 다음과 같다．

38

PART01. MAT나＼B 기본 기능 익히71

卜 Pr口口ram 테01 卜 加ATLAB 卜 R20i5b 卜 bin 卜

P

卜 C

니14 경로 표시줄

구

뇨乞搖諍小

! - p0）丁거'if佃5 1 的10小SI 只兀'Sb 卜

폴더 선택

口

상위 폴더로 이동

！擘 컴퓨텨

上 叫戶pace

心 로료 디스크 (C그

I- 'en伯te

m 이듕식 디스크 (J
I뎌

R20I5b

＝丕m
그림 즈6 현재 폴더 상자와 폴더 찾아보기 창

1ll}

I

명령 창에 口＼사d 명령어를 입력하면 현재 폴더의 경로를 확인할 수 있다，

현채 폴더 창 이용하기

실행 화면어］ 위치한 현재 폴더 창에서 현재 폴더를 변경할 수도 있다. 이는 폴더 이동으로 가능한데，
방법 ]]
방법
현재 폴더보다상위 폴더로 이동하려면 ［壹 버튼이나 中 버튼을클릭하고, 하위 폴더로 이동하려면

中 버튼을클릭한다. 또는 방법 2 경로가 표시된 경로 표시줄을 더블클릭한후 변경할 경로를 직접 입력
하여 현재 폴더를 변경한다. 이를그림으로 간단히 나타내면 다음과 같다．
하위 폴더로 이동
TLAB 卜 R20i5b 卜 bin
상위 폴더로 이동
田 恥 013ire9i1打y
田 三三 regiat匹
如， util
田 知 七v1n32
姓 ADD.s뇨
因A畔ce.m
的An朋mm
的Ana次mDem.m
營AnAmFreq.m
孕An非m.m
拙An抑加q.m
孕 昨陌C.rn
拍BcMagn.nr
쓰 叱MagnErn
幼 미仗Iii陀m
因 B畔呻O.m
因 師tin채rre.m
的 b曲ctm
孕比e比啣rral.m
始帥曲叩.01
幼 CapEner.m
們 C柳ara.m
Dot引江
그림 十7 현재 폴더 창

CHAPTER 02. 명령어를담는스크립트파일

39

MATLAB

핵심 기능
익히기
CONTENTS
PART 020私仁 무엇을 배울까？
CHAPTER 03;
CHAPTER 04
CHAPTER

호롬을 바꾸는 프로그리惶j
"프로그램 구성을 한눈어！"

CHAPTER 06，'
CHAPTER 07 외부 파일 불러오기／내보내기
' 서로 도우면서 지내요"

PART 02에서는
무엇을 배울까？
\\

MATLAB 핵심 기능 익히71
2부에서는 MATLAB의 핵심 기능을 배운다. 초보 운전자가 교통이 혼잡한 도심에
서 빨리 운전하여 목적지까지 가기란 쉬운 일이 아니다. 이처럼 MATLAB도 핵심
기능을 이해하지 않고 활용하려 한다면 고전을 면치 못할 것이다．
MATLAB은 배열을 이용하여 빠르게 연산할수 있는 것이 특징이다. 3장에서는 배
열이 무엇인지 알아보고, 배열을 입력하는 방법과 배열 연산자를 사용하여 연산하
는 방법을 살펴본다. 또한 MATLAB 내장함수의 의미와 활용법을 배운다．
MATLAB은 실험이나 수식으로 얻은 복잡한 수치와 자료를 그래프로 표현하여 쉽 三
게 이해할 수 있도록 돕는다. 4장에서는 2차원 그래프와 3차원 그래프를 그리는 방！
법, 그래프의 속성을지정하는방법을익힌다.

=

5장에서는 관계 연산자, 논리 연산자와조건문, 순환문을 학습하여 프로그래밍하는
방법을 익히고, 또한 사용자의 필요에 따라 직접 함수를 만들어 사용하는 사용자정
의함수도 학습한다．
MATLAB의 심벌릭 툴박스를 사용하면 복잡한 수식을 간편하게 계산하고, 계산三
과정을 자세히 표현할 수 있다. 6장에서는 심벌릭 툴박스에 대해 이해하고 ，심벌락｝
툴박스로 수행할 수 있는 계산법을 알아본다．
7장에서는 MATLAB에서 생성되지 않은 일반 그림 파일과 엑셀 파일을 MATLA]3
"
1{
작업공간으로불러오거나외부로내보내는방법을살펴본다.

CHAPTER

데이터를
저징하는
배열과 변수

CONTENTS
LESSON 01 산술 연산자 사용하기
LESSON 02 내장함수와 변수 사용하기
LESS아1 03 배열 입력하;71
LESSON 04 규칙적인 배열 표시하기
LESSON 05 배열 원소 다루기
LESSON 06 배열 특성 구하기
LESSON 07 출력 서식 변경하기

01

산술 연산자 사용하기

MATLAB은 계산 기능을 수행하는 데 가장 많이 쓰인다, 덧셈, 뺄셈, 곱셈, 나눗셈 연산자를 산술 연산자라고 하는데, 이를 사
용하여 기본적인 사칙연산을 수행하는 방법을 살펴보자．
Keyword

! +, 小 1 牛, /, \ 1 八, exp I () 1 산술연산자우선순위 1

덧셉과 별셈（+, 1)

I

"

MATLAB에서 덧셈과 뺄셈은 ＋와 m를 사용한다. 예를 들어 '3+ 4'와 '步4'를 계산하는 방법은 다음과
같다．
>> 3+4
ans =
7
>:）卜4

-1

ans =

I

곱셉과 나눗셈（水 , / , \)

入(IATLAB에서 곱셈은 水（별표）를 사용하고, 나눗셈은 /（오른쪽 나눗셈 연산자）와 \ （왼쪽 나눗셈 연산
자）를 사용한다. A/B의 결과는 A를 B로 나눈 값이지만, A\B의 결과는 B를 A로 나눈 값이다. ／와＼를
이용하여 꼐산하는 방법을 살펴보자．
力 12/4

< L 오른쪽나눗셈（12를4로나눈값）

ans =
3
力2\10 ＜왼쪽峠셈10을2로나눈값）
ans =
5
口마 왼쪽 匕方：셈 기호＼는［回 키로 입력한다．

44

PART 02. MAThAB 핵심 기능 익히기

1 예저Is-I

I

MATL.AB에서 사용하는 덧셈, 뺄셈. 곱셈과 두 가지 형태의 나눗셈 연산자를 이용하여 2+3. 2-3, 2心，
3+6 , 命3을 계산하고, 결과를 비교하라．
Comm和ci 'tindc小／

풀이

군）

>> 2.3 0
ans =
S
>> 2日
ans =
니

>> 2*3
ans =

6
>> 3/6 0

그림 3너 사칙연산 실행 결과

0 덧셈, 뺄셈, 곱셈은＋, , 水 연산자를이용하여 계산한다．
0 오른쪽 나눗셈은 /（오른쪽 나눗셈 연산자）를 이용하여 계산한다．
0 왼쪽 나눗셈은＼（왼쪽 나눗셈 연산자）를 이용하여 계산한다．

li i}

I

별도로 출력 형식을 지정하지 않으면 결과는 소수점 아래 네 자리까지만 나타난다．

지수승（시, 지수함수（exp)

入t&TLAB에서 어떤 밑수어］대한 지수승을 표현할 때는八을 사용하고, 지수함수를 표현할 때는 exp 명령
어를사용한다. e자）명령어를사용할 때는반드시 소괄호 안어］지수승을 적어야하며, 소괄호를사용하지
않으면 오류가 발생한다. 예를 들어 밑수가 2이고 지수승이 5인 才과 지수함수 可2을 계산하는 방법은 다
음과 같다．

CRAP在R 03. 뎨이터를 저장하는 배열과 변수

45

力2 '5

＜밑수가2이고지수승이5)

ans =

＜지

2)

(-

力exp

32

수斟四口승

]

ans =

0.1353

나껜斗기
지수승 1.23 x 10巧. 4.56 x i 10과 치수함수 可5을 명령 창에 입력하여 결과를 확인하라．

풀이

>>

.23e-5 0

ann =
1 .2300e-05
>> 4, 56e*10
ano =
［그e* 1［그
4. 56［그

>> en口毛 0

Err口r using 르쯔므 0
Not enough input arguments

>> eep(-5) 0
ann =
口0067
그림 3쿄 지수승과 지수함수 실행 결과

Oe를 이용하여 1.23 x 10巧을 간략하게 입력한다．
0 exp 명령어를소괄호 없이 사용하면 오류메시지 (O）가 나타난다．
0 可5을 입력한다．
口II} 밑수7口0이고 지수승이 幻7인 1o' "올 표현할 때는 10의 거듭제곱을 뜻하는 e를 이용하여 in士n으로 나타낼 수 있다．이런 경우 소괄
호를 사용하지 않아도 된다．

46

P／놔극T 02. MAT냐＼B 핵심 기능 익히기

I

소괄호
（)

MATLAB에서 소괄호는 가장 중요한 연산자 중의 하나이다. 수식을 입력할 때 소괄호를 사용하면 복잡한
수식을 간결하게 만들어 코딩 (coding) 오류를 줄일 수 있다. 소괄호를 적절히 사용하면 연산순서를 명
확히 하여 계산의 오류를 방지할수 있다．

I

산술 연산자 우선순위

연산자의 우놘순위어］따라 연산의 결과가 달라지기 때문어］ 연산의 순서를 정하는 연산자의 우선순위는
매우 중요하다. 산술 연산자의 우썬순위는 다음과 긷陋］ 소괄호, 지수함수, 곱셈 또는 나눗셈, 덧셈 또는
뺄셈이다. 소콸호가 중첩된 경우 가장 안쪽부터 바깥쪽으로 확장하여 해석하며, 같은 우전순위의 연산자
는 왼쪽어］위치한 연산자부터 해석한다．

우선순위를 고려하지 않고 연산자를 사용함으로써 사용자가 의도한 것과 다른 결과가 나오더라도
入IATLAB에서는 경고나 오류 메시지를 표시하지 않는다. 따라서 연산자를 사용할 때 우선순위를 고려하
지 않으면 전체 프로그래밍의 결과어］ 심각한 영향을 미칠 수 있고, 때로는 부정확한 결과가 나타나므로
주의해야한다．

CHAPTER 03. 데이터튤 저징하는 배열과 변수

47

LESSON

내쟝함수와 변수 사용하기

02

MATLAB에서 변수를 사용하는 방법을 익히고, 내장함수의 의미와 자주 사용하는 내장함수를 알아보자．
Keyword

I 변수 1 허수 단위 변수 1 내장함수 1

1 변수
八'IATLAB에서는 변수를 이용하여 정보를 저장하고 계산한다. 변수는 정보를 임시로 저장할 메모리 공간
을 의미하며, 변수어］정보를 저장하는 것을 '지정한다’고 한다．
八/IATLAB어］서 수식을 계산하거나 변수 또는 배열의 값을 지정할 때는 등호를 사용한다. 등호의 오른쪽어］
는 지정할 값, 변수명, 수식 등을 입력하고, 왼쪽에는 반드시 변수명을 적어야 한다. 이따L변수명은 반드
시 영문자로 시작해야하고, 이후에는다른 영문자, 숫자, 밑줄(-）을사용할수 있다. 八4ATLAB에서는소
문자와 대문자를 구분하므로 'a'와 'A'는 전혀 다른 변수명이다．
변수명 (var奴bles) = 값
변수명 (variables) = 변수명
변수명 (variables) = 수식 (expression)
예를들어 등호를 이용하여 변수 x어］ 1을 지정하는 방법은 다음과 같다．

I

허수 단위 변수

入4ATLAB어］서 i와／는 복소수의 허수 단위 戶1을 의미하는 예외적 내장 변수이며，이는 일반 변수명으
로도 사용할 수 있다. 만약 허수 단위 변수로 i와／를 사용한다면 미리 값을 지정하지 않아도 되지만，변수
로 사용할 경우에는 반드시 값을 미리 지정해야 한다．
48

PART02. M酊LAB 핵심 기능 익히기

1 예工｛I :}-q

I

다음 값을 명령 창에 나타내라．
(a) 실숫값 1과 허숫값 2를 가진 복소수 z률 입력하라．
(b) 변수 / =5, 戶 8일 때 汗：
I를 계산하라．

푿이

［쏘mm諦（i Windo川

>> e=1.2*a 0
Undefined function or variable a 'J 0

>> z=1+21 C
2 =

>' i
>>

=5;

1 . 0000 + 2. 00001

B;

j=

>> w=sqrt (i-j) e
口 =

0. 0000 + 1 7321 i
그림 +3 허수 단위 변수 실행 결과

(a) 변수口를 미리 지정하지 않았으므로（이 오류 메시지 (O）가 나타난다．
1／를 허수 단위 변수로 사용할 때는 미리 지정하지 않아도 된다. 이 경우 i는 일반 변수가 아니므로 곱
셈 연산자를 사용하지 않아도 된다（回．
(b) 값을 지정한 이후에 1,／를사용하면 戶1의 값을 가진 내장 변수가아닌 일반 변수로 취급된다（이．

I

변수에 문자열 지정하기

일반적으로는변수에 숫자나배열 등을지정하지만경우에 따라문자열을지정할수도 있다. 지정할문자열
을작은파옴표 인어］입력한후등호를 이용하여 지정한다. 이때 작은파옴표를생락하면 오류가발생한다．
예를들어 변수Characters어］문자열 'String'을 지정하는 방법은 다음과같다．
>> Characters = 'String'
Characters =
String

CHAPTER 03. 데이터를저잗后1는 배열과 변수

49

1 예제3- 4 I
변수명이 Name인 변수에 문자열 ' MATLAB ' 을 지정하라．

쭐이

@

（뇨mmand Wire托싸
>> 的iii已 = NAIL比 0
U口del i刈 luridt on or variab比

MATLA日

0

Did you mean:
>> Name = Mat lab 0
>> Name = MATLAB
Name =
MAIL사3
>> Num = 123 0
Num =
123
>> burn = ' 123
Narn =
1 23
그림 +4 변수에 문자열 지정하71 실행 결과

0 문자열에 대한 변수명을 지정할 때 작은따옴표를 생략하면 오류 메시지 (0）가 나타나고, 이어서 자동으
로 두 번째 프롬프트 명령줄이 나온다. 이때 ti田 키를 누르면 의미를 알 수 없는 숫자가 나오므로 두
번째 프롬프트 줄은삭제하고 다음 명령줄을 실행하는 것이 좋다．
0 작은따옴표를 문자의 앞뒤에 붙여서 변수에 문자열을 지정한다．
0 기술적으로는수와수식에 작은파옴표가 있는 경우와 없는 경우모두오류 메시지가나타나지 않고 같은 결
과가 나온다. 작은따옴표를 사용하지 않은 경우의 결과를 영어로 읽으면 'one hux岫七d twen口 three'가
되고, 작은따옴표를 사용한 경우의 결과는 문자열처럼 읽어서 'one two three'가 된다.

I

내장함수

내장함수란 자주 사용하는 연산 또는 계산을 함수로 만들어 入IAThAB어］정의해둔 것이다. 내장함수는 항
상 소문자로 표기하고, 소괄호 안어］ 필요한 인자를 넣어서 사용한다. 모튼 내장함수를 알고 있을 필요는
없으며, 도움말 명령어를 이용하여 필요한 내장함수는 찾아서 사용하면 된다. ［표 3-1] 어］ 자주 사용하는
내장함수를 정리했다．

50

PART 02. MATLAB핵심 기능익히71

표3너 자주사용하는 내장함수
함수명

기능

사용 0tt

결과

abs

절댓값 계산 함수

abs(-1)

cos

코사인 함수

cos(0)

]

log

자연로그 계산 함수

log(exp(1))

l

]

log化

밑수가 ]0인 로그 계산 함수

loglo(1e+1)

]

미n

사인 함수

sin(pi/2)

]

sqrt

제곱근 계산 함수

sqrt(4)

2

1 예저1：크-5 i
!.H：
규；
＝니
工 = 60' 일 때 計n. cos 함수를 이용하여 Yi = Si可功, Y2 = COS仁）를 구하라．

풀이

Command Wir十
>> x＝미／3; <1
>> 비＝引n(X) 0
yl

（무）

=

0. 匪刃
>> y2=cos(x) 0
y2 =
0.5000
>> x=p1/3; y!＝引n(X), y2=cos(X) 0
yl

=

0.8타刃
y2 =
0.5000
그림 +5 甘n. cos 함수 실행 결과
0 Sin, COS 함수는 라디안 값을 인자로 사용하므로 60" 를 刃3 라디안으로 변환하여 工어i 지정한다．
0 Sin 함수를 이용하여 工 = 60' 에 대한 사인 값을 y1에 지정한다．
0 COS 함수를 이용하여 工 = 60' 에 대한 코사인 값을 y2에 지정한다．
0 세미콜론을 이용하여 명령줄 하나어］여러 문장을 입력한다. 명령줄 하나어］여러 문장을 입력하려면 문장
과 문장 사이에 콤마 또는세미콜론을 사용한다．

CHAPTER 03. 데이터를 저장하는 배열과 변수

51

LESSON

03

배열 입력하기

MAT나＼B에서는 주로 배열을 이용하여 연산한다．배열이 무엇인지 이해하고, 배열을 입력하는 방법을 알아보자．
Keyword

! 배열 1 중괄호（[ I) 1 세미콜론（;) 1 콤마（, ) I eye I zeros I ones I 콜론(:) i 전치 연산자（' ) 1

I 배열
배열（array）은문자, 기호, 자료 등 같은 성격을 가진 수치 정보가순서에 따라무리 지어 표시되는 것을
말한다. 그중 하나의 행으로 구성된 배열을 행벡터, 하나의 열로 구성된 배열을 열벡터, 2차원 배열을 행
렬（m吼dX）이라고한다. 공학에서는 배열과 행렬을 자연스럽게 교환해서 사용한다．

I 배염 입력하기
배열을 입력할 때는 중콸호（[ ] ) 안어］원소를 넣는다. 배열의 행을 바꿀 때는 중괄호 안어］ 세미콜론（;）을
넣고, 열을바꿀때는한칸을띄우거나콤마（,）를넣는다．
. .

H

H

.

. .

.

,

[1

예늘늘어 배떨 兀 = 1 4
Li

. 1는 다늠과 샅이 입딕한다．
4i

>>x=[1 2;34];
>> x=[1,2;3,4];

1 여江II % -R I
1H:：二：二＝ -I
배열 A를 입력하라．

11 2 3
A기4
[7

52

PA日T02. MAT냐＼B 핵심 기능 익히71

5
8

6
9

푿이

e)

녑／ndc나

>> A=L1 2 3;4 6 6;7 8 9] ;Q
>> A=L1 2 3;4 S 6;7 8 91 0
A =
口U
mb
口나

nr

7
느 =
U B

d1 4

>> A비1, 2, 3; 4, 5,6；加，910
A =
1
4
7

2
6
8

3
日
9

그림 3小 배열 입력하기 실행 결과

0 배열을 지정한후 세미콜론을 사용하면 결과가 명령 창에 나타나지 않는다．
0 원소를공백으로 구분하여 입력한 배열의 결과가 명령 창에 나타난다．
0 원소를 콤마로 구분하여 입력한 배열의 결과가 명령 창에 나타난다．

I

푹정 배옅 만듣기

eye 명령어를 사용하면 배열의 주 대각선（main diagonal)에 놓이는 원소는 모두 1이고 그 외 배열의
원소는 모두 0인 단위행렬(identity matrix）을 생성한다. 또한 zeros 명령어는 배열의 크기와상관없이
모튼 원소를 0으로 지정하고, ones 명령어는 모튼 원소를 1로 지정한다．
특수한형태의 m 자2 배열을만드는 eye, zeros, oi妃S 명령어의 기본형태는다음과같다．
嚼巍m蜘斗礪難聽畔發解轉聲群
eye(m,n)
zeros(m,n)
ones(m,n)
口d1 행의 수와 열의 수가 같은 nXn 배열을 만들 때는 명령어의 인자값 伽,n) 대신에 伽）만 입력하면 된다．

CHAPTER 03. 데이터툴 저장하는 배열과 변수

53

1 예工113-7 I
대각선 원소의 값이 모두 1인 3행 3열 배열을 나타내라. 또한 모든 원소의 값이 0인 3행 3열 배열과 모든 원
소의 값이 1인 3행 3열 배열을 나타내라．

풀이

e)

Command V. n:

>> eye (3) 0

ann =
1

0

0

0

1

0

0

0

1

>> zeron(3) e
ann =
0

口

0

U
0

U
0

0
0

>> anen (3) 0
ann =
1

I

1

1

I

1

1

1

1

그림 +7 특정 배열 만듈71 실행 결과

0 eye 명령어를 이용하여 대각선 원소가 1인 3x3 배열을 지정한다．
0 zeros 명령어를 이용하여 모든 원소가0인 3x3 배열을 지정한다．
0 ones 명령어를 이용하여 모든 원소가 1인 3x3 배열을 지정한다．

I

배염 원소 다루기

배열의 동일한 행에 포함되는 원소들을 분리하려면 콤마（,）를 사용한다. 배열의 색인을 생성할 때와 각각
의 차원어］ 해당하는 행과 열에 대한 색인을 분리할 때도 콤마를 사용한다. 콤마의 왼쪽쇄는 지정하는 행
의 번호를, 오른쪽에는 지정하는 열의 번호를 입력한다. 예를 들어 배열 A의 1행 2열 원소를 분리하려면
A(1,기를 입력한다．
콜론（:）은주어진 배열어］대한각원소, 행, 열 및 부분 배열을다양한방법으로표시하는 데 사용한다. 또
한콜론은 전체 행 혹은 열에 대해 와일드카드 역할을한다. 예를들어 v(:）은 벡터 V의 모튼 행과 열의 원
소를나타내고, v(2:5）는벡터 V의 두번째부터 다섯 번째 원소인v(2), v(3), v(4), v(5）를나타낸다．

54

PART02. MI노ThAB 핵심 기능 익히71

1 예제3出 1
배열 A가 다음과 같을 때 문제를 풀라．
2

3'

4

5

6

.7

8

9.

A=

'1

(a) 콤마를 이용하여 배열 A의 1행 1열 원소와 2행 3열 원소를 찾아라．
(b) 콜론을 이용하여 배열 A의 2열 모든 원소와 3행 모든 원소를 찾아라．
VI

/n

Ccmmand 7ind口卉
(a)

系i

"

A=L1 2 3;4 S 6;7 日

1
4
7

2
5
日

3
6
9

S
그림 3田 콤마를 이용한 배열 원소 찾기 실행 결과

0 배열 A를 지정한다．
0 배열 A의 l행 1열 원소를 나타낸다．
0 배열 A의 2행 3열 원소를 나타낸다．
(h)

Command Window

侄）

>> A= fI 2 土4 5 5;? 日 9]
q
1
4
7

2
5
8

3
6
9

a) A( :,2) 0
ann =

2
S
8

그립 +9 콜론을 이용한 배열 원소 찾기 실행 결과

CHAPTER 03. 데이터를 저장하는 배열과 변수

55

0 배열 A의 2열 원소를 나타낸다. 이때 콜론은 배열 A의 모든 행, 2는 배열 A의 2열을 의미한다．
0 배열 A의 3행 원소를 나타낸다. 이때 3은 배열 A의 3행, 콜론은 모튼 열을 의미한다．

1 예제 3四 1
콜론을 이용하여 배열 A의 3행과 4행 사이의 모든 원소, 2열과 4열 사이의 모든 공통 원소를 찾아라. 또한
배열 A의 ] 행과 3행 사이의 모든 원소, ] 열과 5열의 공통 원소를 찾아라．

A

==

0

1

2

3

4

5

6

7

8

9

1 -2

-3

-4 -5

-8

-9

-6

풀이

-7

0

Command Window
>> A=10 I 2 3 4;5 6 7 5 9;-I -2 -3 -4 -5;-6 -7 -8 -9 0)
A =
4

口
니

口
U

4

口
U

口
니

0

m
1
1

口
니

口U

ans =
-2
-7

-3
-8

-4
-9

>>*(I:3, (1 51) 0
aiis =
口
5
니

4
9
5

그림卜］0 콜론을 이용한 배열 원소 찾기 실행 결과

0 배열 A의 3행과4행 사이의 원소 중 2열과4열 사이의 원소를 지정한다．
0 배열 A의 1행과3행 사이의 원소 중 1열과 5열의 원소를 지정한다．
m}

행이나 열을 연속해서 지정하는 경우가 아니면 중괄호를 이용하여 개별적으로 선택할 수 있다．

56

PART02. M月ThPB 핵심 기능 익히7)

1

nr

小
b

nd

n<

1
1

n/

小b

:
U

n<

11

0

>> A (3:4, 2: 4) <1

I

전치 연산자（' )

전치 연산자는 입력한 배열의 행과 열을 서로 바꿔주는 역할을 하며, 배열에 아平人드 쿠피 (apostrophe

)

를붙인다．

i 예工fi 3- 10 I
L二두＝1= =J
배열 A를 입력하려다가 실수로 행과 열을 서로 바꾸어 >>B = [1 47; 25 8; 3 69］를 입력했다고

배열 B를 지정하고, 배열 B에 전치 연산자를 이용하여 배열 A를 입력하라．
n
乙

n
A
口

d나

＜
口

6

m/

8

0
/

1

샤

Cammand ＼차따do甘／

P

4 7;2 5 8;3 6 9J;
'> A=11 2 3;4 5 6;7 S Si U
L1

'>8=

풀이

가정하자．

A =
1
4
7

2
5
日

3
6
S

2
5
8

3
6
9

>> A=8 'Q
A =
1
4
7

그림 3놔11 전치 연산자 실행 결과

0 행과 열을 서로 바꾸어 입력한 배열 B를 지정한다．
0 배열 A를 직접 입력하여 지정한다．
0 배열 B에 전치 연산자를 이용하여 행과 열을 바꾼 배열 A를 지정한다．

CHAPTER 03. 데이터를 저장하는 배열과 변수

57

0

규칙적인 배옅 표시하기

MAT냐＼B에서 규칙적으로 나열되는 배열의 원소를 쉽게 지정하기 위해 사용하는 콜론 연산자와 hnspace 함수를 알아보자．

Keyword

1 콜론 연산자 ! linspace

1

量 콜론 연산자
콜론 연산자는 규칙적으로 증가하거나 감소하는 배열의 원소를 지정하는 더］ 사용한다. 예를 들어 1에서
1000까지 1씩 규칙적으로증가하는 자료를 입력해야하는 경우, 수많은 자료를 하나씩 입력하는 대신 콜
론 연산자를 이용하면 훨씬 쉽게 배열을 지정할 수 있다．
벡터 x를 생성하기 위한 콜론 연산자의 기본 형태는 다음과 같다．
x= i: j: k
· i: 초깃값
· j: 규칙적으로 증가하거나 감소하는 값
· k: 최종값

음수여야
日F'工 규칙적으로 감소하는 원소를 지정할 때는 반드시 초깃값이 최종값보다 큰 수여야 하고, 규칙적으로 감소하는 값이

I

힌타．

linspace

초깃값, 최종값, 원소 개수를 입력벋아 벡터어］규칙적인 원소를 지정하는 un아氾ce 함수의 기본 형태는
다음과같다．
Iinspace(xl ,x2,n)
· xl: 초깃값
. x2: 최종값

linspace 함수를 사용하여 배열을 지정한다．

58

PART02.卜朋ILAB핵심 기능익히71

fin！
三인
力＝
크기

예를들어 수치해석어］서 사다리꼴적분법을＼陪할때 간격

毗를구하기

· n: 초깃값콰 최종값 사이의 원소 개수

위해

다음은8장의 ［예제 8-23］에서 다루는코드의 일부이다．
力 xl = linspace (1,3，卦
xl =
1.0000

1.5000

2.0000

2.5000

3.0000

1 예제 3- 11 I
HH = . . . .H ．小 1, . n. . . . .. . , 37r . . 7r ... 1. .
H . ..
』． . . . 1. . . 1 1. ' .
골돈 언산人듣 이뇽O뼈 권소 的 0에셔；까지 4씩 규직석으로 승7r
"는 벡터 U들 지성한 걸고들 확긴
하라. 그리고 linspace 함수를 이용하여 벡터 U를 지정한 결과를 확인하라．

풀이

Command 쌔nd야V
>> u=0：미/4:3*미／20
u

=

U

0. 7854

1 . 5708

2. 3562

3, 1416

3. 9270

4. 7124

2. 3562

3. 1416

3. 9270

4. 7124

>> U＝니nspace (0，小이尼7) e
11

U

0. 7얹54

1 . b'ILU

그림 +12 규칙적인 배열 지정하기 실행 결과

{1

兀
0 콜론 연산자를 이용하여 일정하제 증가하는 벡터를 지정한다. 0은 초깃값, H는 규칙적으로 증가하는

幷프는최종값이다．
2
0 lmspace 함수를 이용古Hj 일정하게 증가하는벡터를 지정한다. 0은초깃값, 프는 최종값, 7은초깃값
2
과최종값人卜기의원소개수이다.

II I}

묶여 있는 계수나 변수도 반드시 곱셈 연산자를 이용하여 연산해야 한다．

CHAPTE日 03. 데이터를 저장하는 배열과 변수

59

L 旨 S $ ON

05

배열 원소 다루기

배열 연산에 사용하는 배열 연산자를 알아뾰 ，배열 원소를 추가 ，삭저i ，대체하는 방법과 두 배열을 연쇄 ，덧붙이기하는 방법
을 익히자．
I 배열 연산자 1 배열 원소의 추가, 삭저1, 대체 1 배열의 연쇄, 덧붙이기 1

Keyword

邕 배열 연산자
행과 열의 수가 같은 두 배열은 배열 연산자를 이용하여 항목별 연산을 할 수 있다. 배열 연산자는 곱셈，
나눗셈, 지수승 바로 앞어］마침표（.）를 붙여서 사용한다. 배열 연산자를 이용하면 평가하려는 자료를 더
욱 쉽게 생성하고, 읽고, 문서로 작성할수 있다．
표 3-2 배열 연산자
연산자

의미

항목별 왼쪽 나눗셈

.\

의미
항목별 오른쪽 나눗섣1

.1

항목별 곱셈

연산자

八

>>A= [246];B= [123];
<; A, B의항목별곱셈
力A．串B

항목별 지수승

J

ans =
2

8

18

力A./B

<

邸의항목별오른쪽峠셈．

ans =
2

2

力A.\B

2
＜人B의항목별왼쪽峠셈

ans =
0.5000
力A. 'B

0.5000
<

0.5000

A, B의항목별지수승

ans =
2

60

16 216

PART 02. MATLAB 핵심 기능 익히기

]

1 （川工카 q -12 I
I二二二H- -J
벡터 u = [2 3 4］와 v= [1 9 8］에 대한 배열 연산의 항목별 곱셈과 오른쪽 나눗셈을 실행하라．

Command＼心nd口」
／甘
>> u=[2 3 4] ;
>> V=[1 므 8] ;

>> 이＝艸0

Error using
Inner matrix dimensions must agree,
_

__

>> m2＝已*V e
s2 =
2

27

32

>>dl=u/v 0
dl =
0. 4178
>> d2u. /vQ
d2 =
2.0000

0. 3333

口．50［刃

그림 3-13 배열 연산자실행 결과

0 배열 연산인 ml의 연산에서 산술 연산자를 이용했으므로 오류 메시지 (O）가 나타난다．
0 배열 연산자를 이용한 m2의 연산은 벡터 U와V의 같은 자리에 있는 원소를 항목별로 곱한 결과가 출력
된다．
0 오른쪽 나눗셈 산술 연산자를 이용한dl의 연산은 원래 의도한 항목별 오른쪽 나눗셈의 결과가 출력되지
않는다．
0 배열 연산자를 이용한 d2의 연산은 벡터 U와 V의 같은 자리에 있는 원소를 항목별로 오른쪽 나눗셈한
결과가출력된다．
口nl

I

벡터와 배열의 원소를표시할 때는 x(2). A(4, 5）와 같이 쓴다. 각 원소의 자리 번호는 반드叭1 j번부터 지정해야 한다．

배열 원소의 추가, 삭저1, 대처1

배열 원소의 추가, 삭제, 대체는 배열의 특정 행 또는 열에 원소를 지정하는 것으로 배열 원소 다루기와동
일한방법을사용한다．
배열 원소의 추가는 콤마와 콜론을 이용하여 추가하려는 행 또는 열의 색인을 주어진 배열에 지정하고，
추가하려는 새로운 배열을 등호의 오른쪽어］지정하여 실행한다. 배열 원소의 삭제는 삭제할 행 또는 열의
색인을 주어진 배열에 지정하고, 콤마의 오른쪽어］ [ ］를 지정하여 실행한다. 배열 원소의 대체는 배열 원
소의 추가와 같은 방법으로 실행하며, 주어진 배열의 크기 변화 없이 생성된 원소의 내용만을 수정한다．

CHAPTER 03. 데이터를 저짐后1는 배열과 변수

61

>>A=[1 2;34];
>>A (3,:) = [56]
A

二二

1

2

3

4

5

6

力 A (3, :) =[]

, 배열 원소삭제

A=
1

2

3 4
>>A (2,:) = [56]

띠，1 배열 원소 대체

A=
1

2

5

6

1 예제 3- 131
콜론을 이용하여 배열 A의 5행에 원소 [-1 -2 -3］을 추가한 결과와 2열의 모든 원소를 삭제한 결과를 확인
하라. 또한 3행의 원소를 [ 7 -8］로 대체한 결과를 확인하라．
11

2

A기4
[7

8

풀이

그림 +14 배열 원소의 추'F. 삭저L 대체 실행 결과

62

PA日T02. M사녀B 핵심 기능 익히기

3]

5 61
9J

0 배열 A는 3x3 배열이므로 5행의 원소를 추가할 경우4행의 모든 원소는 0으로 지정된다．
0 배열 A의 2열에 [］를 지정하여 2열을삭제한다．
0 배열 A의 3행 원소를［刃 -8]로 대체한다．

I

배열의 연쇄, 덧붙이기

배열의 연쇄（conc毗enate）와 덧붙이기 (append）는 두 배열을 하나로 묶는 것이다. 배열의 연쇄는 크
기가 같은 두 배열을 하나로 묶는 데 사용하므로 반드시 두 배열의 행과 열의 수가 긷-o｝야 한다. 반면에 배
열의 덧붙히기는 배열의 크기와상콴없이 두 배열을 하나로 묶는 데 사용한다．
>>A=[o 1; 23]; B=[4 5;67] ; c=[89]';

D=

力D=[A,B], E=[A;B] ＜배열원소연쇄
0

1

4

5

2

3

6

7

E=
0

1

2

3

4

5

6

7

>> F=[A,c]

＜배열원소덧봔］기 "

F=
0

1

8

2

3

9

i 에xli 숙口口．1t I
［二二：느：
＝二J
배열 A와 B를 연쇄하여 새로운 2행 4열의 배열 C로 나타내라. 그리고 배열 A와 B를 연쇄하여 새로운 4행

L3

21
4]

61

L7 8]
I5

'

B=

1

A=

2열의 배열 D로 나타내라．

CHAPTER 03. 데이터를저장하는 배열과변수

63

풀이

그림 3-iS 배열 연쇄 실행 결과

0 콤마를 이용하여 2x2 배열 2개를 2x4 배열 C로 연쇄한다．
0 세미콜론을 이용하여 2x2 배열 2개를 4x2 배열 0로 연쇄한다．

1예저13-151
배열 A에 벡터 b와 C를 차례로 덧붙이기하여 새로운 3행 4열의 배열 B로 나타내라. 그리고 벡터 ii에 배열
A와 벡터 C를 덧붙이기하여 새로운 3행 4열의 배열 C로 나타내라．
1 21

131

A=

4 키，
b기이，
c= t-1 -2 巾31
8i
19]

7

풀이

｛工n그m引1그

>> 肛I1 2;4 S;7 B] ; (1
>> b= ]3;6;9] ;
>> c= ]-I -2 -3] '

>> 먀［凡b,c] 0
B

>> C=

]bA.

3

2
5
日

5
9

-l
-2
-3

2
5
日

-I
-2
3

0

c]

1
4
7

C =
3
B
9

I
4
7

그림 +16 배열 덧붙이기 실행 결과

0 배열 A와 벡터 b, c를 지정한다．
今 배열 A에 벡터 b, c를 덧붙이기한3x4 배열 B를 지정한다．
0 벡터 b에 배열 A와 벡터 C를 덧붙이기한3x4 배열 C를 지정한다．

64

PART 02. MATLAB 핵심 기능 익히71

LESSON

06

배열 특성 구하71

명령어를 사용하면 배열의 행과 열의 개수를 쉽게 알 수 있다. 배열의 특성을 알71 위해1 사용하는 find, size, length 명령어룔

알아보자．

Keyword

I

I find 1 size I length I

find

주어진 배열 중에 0이 아닌 값을 가진 원소의 자리 번호를 표시하는 find 함수의 기본 형태는 다음과 같다．
find(A)
·A: OOI 아닌 원소의 자리 번호를 구할 행렬

이때 자리 번호는 1부터 시작한다．

1 예工113-161
배열 xl= [O

풀이

-1 3

0 0 -6

9］에서 값이 0이 아닌 원소의 자리 번호를 찾아라．

Command Wind=
>> x=[O-l, 3.毗，七，의 0
K1

（自

=

0

너

3

0

6

7

0

-6

9

>> p= find(nl) Q
p=
2

3

그림 十］7 fin} 함수 실행 결과

0 배열 xl을 지정한다．
0 find 함수를 이용하여 배열 xl에서 0이 아닌 값 -1. 3, 小6. 9의 자리 번호인 2, 3. 6, 7을출력한다．

CHAPTER 03; 데이터를 저장하는 배열과 변수

65

I size
행 m개와 열 n개로 구성된 m X77 배열에 size 함수를 사용하면 m, n 값을 출력한다. 따라서 size 함수는
시뮬레이션 혹은 무작위로 생성된 새로운 배열어］대한 자료의 개수를 확인하는 데 유용하게 사용할 수 있
다. S倪e 함수의 기본 형태는 다음과 같다．
size(A)
. A: 행과 열의 개수를 구할 행렬

I

length

행 m개와 열 m귀로 구성된 m X7i 배열에 length 함수를 사용하면 m과 n의 개수 중어］ 더 큰 하나의 값만
출력한다. length 함수의 기본 형태는 다음과같다．
length(A)
,A: 행과 열의 개수 중 더 큰 하나의 값을 구할 행렬

1 예工II q -17
-- I
二二1L二：
배열 A는 각각 몇 개의 행과 열로 구성되어 있는지 구하라. 그리고 배열 A의 행과 열의 수 중 큰 값을 나타내라．
2

A

1

3

5

4

8

1 -2=
Command Wind口나
>> A=E2, I ;3』5;4,8;-L-2]
4

풀이

@

=

4

]58

1

n
叱

n
d
n
口

>> 引ze(A)
aris =
4

2

>> Iength(A)
ann =
4
그림 3-18 섧ze. len아h 함수 실행 결과

0 size 함수를 이용하여 배열 A의 행과 열의 개수를 출력한다．
0 length 함수를 이용하여 4 x2 배열 A의 행 개수 4와 열 개수 2 중 더 큰 수인 4를 출력한다．

66

PART02. M사냐＼B핵심 기능익히기

LESSON

07

출력 서식 변경하기

MATLAB에서 출력 서식을 변경하71 위해 사용하는 명령어를 알아보자，
Keyword

I

I format short 1 format short e 1 format long I format long e 1

출력 서식

숫자 또는 숫자가 저장된 배열을 출력할 때는 출력 서식을 변경하여 사용자가 원하는 형태로 숫자를 나타
낼 수 있다. 기본 출력 서식을 적용하면 소수점 아래 네 자리까지 나타나며, 이는 化rmat short를 이용한
결과와 같다．
출력 서식 명령어와그 기능을 ［표 3-3］에 정리했다．
표 于：3 출력 서식 명령어
명령어

p1를 출력한 oh

기눙

幻rmat sh아t

소수점 아래 네 자리까지 출력

3.14化

幻rmat short e

지수승 e를 이용하여 소수점 아래 네 자리까지 출력

3.1416e+ 000

幻rmat long

소수점 아래 열다섯 자리까지 출력

3.141692653589793

幻rmat long e

지수승 e를 이용하여 소수점 아래 열다섯 자리까지 출력

3.141592653589793e + 000

1 ｛뇌1工fi q -i1t

I

배열 C를 지정한 후 化rmat short, 幻曲at long, 幻rmat sho八 e를 이용하여 출력 서식을 변경한 결과를 확
인하라．

1.

[2

2小
3

匕

2345/ 10口

CHAPTE日 03. 데이터를 저장하는 배열과 변수

67

舌이

侄）
>> c=L2 2/3 1 .2345e-6] 0
c =

2. 0口：l)

0.6667

0.(刃0

>> 化rmat shortQ
>> c=I2 2/3 1.2345e-6]
C =

2. 0000

0. 6667

0. 0000

>> 化n1at 比ng e

>> c=[2 2/3 1 . 2345e-61
c =

2. 0口nnrn口口00口끄00

口 866686668856667

0. 000001234500더그0

0

>> 化rinat short 已 O
>> c '[ 2 2/3 1 . 2345e-61
=

2. 0000e+00

6. 6667e-01

1 ,2345e-06

그림 3-19 출력 서식 변경하기 실행 결과

0 출력 서식을 적용하지 않으면 기본 출력 서식이 적용되어 소수점 아래 녜 자리까지 결과가출력된다．
0 format short를 적용한 경우 소수점 아래 네 자리까지 결과가 출력된다．
0 form毗long을 적용한 경우 소수점 아래 열다섯 자리까지 결과가출력된다．
0 format short e를 적용한 경우 지수승 e를 이용하여 소수점 아래 네 자리까지 결과가 출력된다．
m>

모든 원소가 정수일 때는 소수점 없이도 표현되지만, 만일 원소 중에 하나라도 실수가 있다면 지정된 출력 서식에 따라 소수점 자리가
자동으로 표시된다. 또한 이미 지정한 배열은 배열을 재지정할 필요 없이 배열 이름만 입력해도 배열의 내용이 퐈1된다．

68

PART02. M戶nAB핵심 기능익히기

CHAPTER

i

a

t-

1H卜
十
小
小
+
l
L
L
｛
卜
H
d
!1나
H
나
그
！
니
니
r
卜
卜나
小
卜小n
1艸 丁十

t-

4中

小

04

小

丁

十

H

데이터를
한눈에보는

＋

j

叫

小十 +小 十＋+
上

十

그래프

i

卜
1
1
十
1
上
卞

小

＋

卄

十工
＋
CONTENTS
LESSON 01 2차원 그래프 그리기
LESSON 02 그래프 속성 지정하기
LESS아寸 03 3차원 그래프 그리71

LESSON

01

2차원 그래프 그리기

그래프를 이용하여 결과를 시각적으로 표현하면 실험이나 수식으로 얻은 복잡한 수치와 자료를 훨씬 명쾌하게 해석할 수 있
다. MATLAB에서 선형 工-v 그래프（2차원 그래프）를 그리기 위해 사용하는 명령어를 알아보자．
Keyword

I

1 히야 I h이d 1 semilogx I semilogy I 2차원그래프의 모양과종류 1

이아

plot 명령어는工축（가로축）에 지정되는 입력 자료 벡터 x에 대응하여 y축（세로축）에 지정되는 출력 자
료 벡터 y의 그래프를생성한다. 여러 개의 입력값（xl , 工2, ···）에 대한출력값（yl, y2, ···）의 그래프를
생성하는 plot 명령어의 기본 형태는 다음과 같다．
pIot(x1,y1,x2,y2, ..)
입력값이 지정된 벡터 x와 출력값이 지정된 벡터 y를 이용하여 그래프를 그릴 때 plot 명령어의 기본 형
태는 다음과 같다．
小

plot(x,y,'s')
· X: 입력값이 지정된 벡터

入八／

· y: 출력값이 지정된 벡터
, 1S ': 자료 기豆 선 형태, 색상 지정（생략 가능하며 순서는 상관없음）

표 4너 다양한 자료 기호 및 선과 색상
자료 기호

선 형티i

색상

동그란 점（. )

실선

검은색

k

별표（日

일점쇄선

파란색

b

x표似）

x

쇄선 · 점선 혼합

청록색

C

원형（O)

O

점선

초록색

g

플러스 기호（+)

+

자홍색

m

정사각형（［그）

S

빨간색

r

다이아몬드（아

d

目呂

w

별（女）

p

70

PARTQ2. M月ILAB 핵심 기능 익히기

y

I

h이d

2개 이상의 선을 그림 창 하나어］나타내는 경우 그래프 하나를 먼저 그리고 hold 명령어를 사용하면 그려
진 그림을 확인한 후 그다음쇠］그릴 그래프를 추가할 수 있다. 如id 명령어를 번갈아 입력하면 hold 명령
어 기능의 켜기／끄기를 반복할수 있다．

1 예제 <1너 1
1부터 7까지 증가하는 입력 자료에 대한 3개의 출력 자료 yl, y2, y3이 있다. 이때1 입력변수 x에 대한 출력
변수 yl과 y2률 그래프로 나타내라. 또한 h이d 명령어를 이용하여 입력변수 x에 대한 출력변수 y3을 그래
프로 나타내라．
yl= [0 0.480.8410.910.60.14]
y2 = [0.2 0.5 1 0.84 0.6 0.32 0.09]
y3 =[0.5 0.24 0.31 0.7 1 0.8 0.44]
Command Window
>> a = [I 234557] ;
>> yl = [0 .40 .84 1 . 91 .6 .14] ;
>> y2 = [ .2 .5 I .04 .6 32 .09] ;
>> y3 = 1.5 .24 .31 .71 .8 .441;
>> plot (n,yl, ' -*O ', x, y2, -.oh ') ; 0
>> ho너 0
Current plot held

>> plot (e, y3, :r '); e

>> ho너 0
Current 미st released

그림 4너 2차원 그래프 그리기 코딩 결과

0 한번의 입력으로2개의 그래프를그려 서로 비교할수 있다. 이때 xl. x2의 값O江로동일하기 따문에 yl
과y2의 입력 순서가바뀌어도 된다. 두 선을구분하기 위해 yl은 초록색 실선으로 나타내고, 각자료점을
별표로표시한다. y2는파란색 쇄선·점선 혼합으로 나타내고, 각자료점을 원형으로 표시한다．
Oh아d 명령어가 활성화되어 현재 그림
창의 그래프를 계속 나타낸다. 따라서

Ale

日址

｛그 d 日

W曲 岫et

Toels

(耐top

낙i岫片

目 注＼ :\ 物自咽 I二 니 晷 目 區크 a 口

현재 그림 창어］다른 그래프를 추가하여
나타낼 수 있다．
0 벡터 x, y3을 이용하여 그래프를 그린
다．

풀이

0h아d 명령어가 비활성화되어 현재 그림
창어］다른 그래프를 추가할수 없다．

그림 4쿄 2차원 그래프 그리기 실행 결과

CHAPTER 04. 뎨이터를한눈에 보는그래프

71

I

semilogx

semilogx 명령어는 工축을 로그 눈금으로 그린다. semilogx 명령어의 기본 형태는 다음과같다．
sem加gx似！y)
, X: 입력값이 지정된 벡터
. y: 출력값이 지정된 벡터

I

semilogy

sen皿ogy 명령어는 y축을 로그 눈금으로그린다. sen皿ogy 명령어의 기본 형태는 다음과같다．
semilogy(x, y)
· X: 입력값이 지정된 벡터
· y: 출력값이 지정된 벡터

예를 들어 제어공학에서는 x축이 로그 눈금인 보드선도를 그려서 시스템을 분적한다. MATLAB을 이용
하여 보드선도를 그릴 때는 工축을 로그 눈금으로 설정하기 위해 semilogx 명령어를 사용한다. 다음은
9장의 ［예제 9-1이어］서 다루는BodeD奴g.m의 일부와그 결과이다．
num=30* [0 1 5];
den=conv([1 2], [110] ):

F카e

Edit

Vi曲

：그 (j 日 由

公

1n5gt

4\

化이I

oookl하｝

m耐OW

N랴）

\ i"7 @ 모 J; , 艮 口 듣크 匹 口

omega=0.1:0.1:1e3;
G2=freqs (num,den,omega) ;
mag=abs (G2) ;

10

0

phase=angle (G2):

10

semilogx (omega, 20*Iog10 (mag) )

-20

.30

10.1

72

PART 02. MATLAB핵심 기능익히기

100

101

i02

1o3

1 2차원 그래프의 모양과 종류
방향 그래프

ot(X,Y)

feather(U,V)

J카

\

＼于

1

,, , ,

,, 小, )

선점도 그래프
scatter(X,')

已 ad小如 1
戶戶
느느

｛羽） }.1,m
寸뇨叱 小
기

quiver(x,y,u,v)

凡7M

\\ \ \

10이og(x,y)

comet(x,y)

k

rose(theta씨

\

spy(S)

km뇨寸

\ \ \

7

J肛’i

\

「

?,m甘十可

\

1느

「 "（뉵／
‘

馨
廛）

ezp이a巾un)

이아matrix(X,'y

11朴 따卜J
！뉴

的切(xl,yl,xl .y2)

r
i

r\ Ai

극 형식 그래프
帥，

선 그래匹

r끼片J

每 甫 pp기

LESSON

02

그래프 속성 지정하기

그래프의 정보를 명확히 전달하는 데 도움이 되는 그래프 속성 지정 명령어를 살펴보자．
Keyword

I t出e l 川abel. ytab이 ! axis I grid I 야ext I text I legend I sub이아 {
i figure I 그래프 저장하고불러오71 I

I title
그래프 제목을 지정하는 title 명령어의 기본 형태는 다음과 같다．

title('text')
· 'text' 그래프 제목

I 川abel, 니abel
x축（가로축）과y축（세로축）의 축 이름을 나타내는xlabel, ylabel 명령어의 기본 형태는 다음과같다．
xlabel('text')
ylabel('text')
. 'text느 축 이름

그림 창에서 각 축의 크기를 조절하는 axis 명령어의 기본 형태는 다음과 같다．

axis([xmin xmax ymin ymax])
- xmin, xn怡x: 工축의 시작점에 해당하는 최소 크기와 끝점에 해당하는 최대 크기
·ymin, ymax: y축의 시작점에 해당하는 최소 크기와 끝점에 해당하는 최대 크기

I

grid

그래프에 모눈을 생성하려면 grid 명령어를 사용힌다. grid 명령어를 번갈아 입력하여 켜기／끄기를 반복
하거나, grid on 명령어를 입력하여 모눈을 생성하고 grid o侄 명령어를 입력하여 모눈을 지울수 있다．

74

PART 02. MATLAS 핵심 기능 익히기

예를 들어 신호에서는 실제 파형을 그래프로 그려서 확인하는 것이 매우 중요하다. 八4ATLAB에서는
plot, grid, xlabel, ylabel, title 명령어를사용하여 실제 파형을그래프로 그리고속성을추가할수 있다．
다음은 10장의 ［예제 10-1］에서 다루는 ConSinus.m의 일부와그 결꽈이다．
t=-i :0.01:1;

Fib

日61 出I'.

bgt

TSr出5

r片幽啣1

늬巾岫'w

I1目p

！그 t3 1a 由 臣 '\ \ 的自咽 i= , 盈 日目 I 口

···（생략）

Sin,好C耐川 미grralA이片佃t＋巾）

plot

(t,

xt=A水cos (omega永t+p址）;
xt) ;

二

grid;
xlabel('Tirne (t)'.).;
ylabel ('x (t)') ;
title ('Sinusoidal Signal: Acos(\ 끄llegat+\
phi)') ;

I

-04

-02

0

02

04

06

08

gtext

마우스를 이용하여 원하는 위치에 문자열을삽입하는 gtext 명령어의 기본 형태는 다음과 같다．
gtext('s')
· 令！: 삽입할 문자열

그림 창어］십자선이 표시되면 클릭하여 문자열의 위치를 지정한다．

I text
그래프를 그리기 전에 미리 삽입할 문자열의 가로와 세로 좌표 위치를 설정하기 위한 text 명령어의 기본
형태는다음과갇다．
text(x,y,'s')
· X: 문자열이 위치할 工 좌표
· y: 문자열이 위치할y 좌표
· 낳：삽입할문자열

그래프가그려짐과동시어］해당 위치에 문자열 'S'가표시된다．

CHAPTER 04. 데이터를 한눈에 보는그래프

75

1 예제 4- 2 I
0<工< 2兀（게 위치한 사인 함수 y1 = 없可功와 코사인 함수 Y2 = CO町工）에 대한 그래프를 그리려 한다. 주
기는 兀／180 라디안이며, 兀축 이름은 'Radian Value', y축 이름은 'Mag테加de', 그래프 제목은 'Sine and
Cosine Func如n'으로 지정한다．
(a) gtext 명령어를 이용하여 각각 문자열 'sin(x)'와 'COS伍）'를 표시하라．
(b) text 명령어를 이용하여 좌표 위치 (3.0. 0.5）에 'sitm()'를, 좌표 위치 (1.5. -0.6）에 'COS似）'를 표시하라．
色）

Comrriond Window
(a)

系；

>> X＝먀이／田U:小미 ;
>> 비＝引n（的 ;
>> y2=cos(x) ;
>> 이叭似41 JXJy2J ' : ' ) ;

>>aois([ 02.pi -1 n);<1
>> olabeiC 'Radian value ');O
>> ylabel ( 'Magnitude ') ;

>> it le( ' Sine and Cosine Functi0n " );e
>> 日r너；C
>> gteat (' sin(x) ') ; 0
>> gtext ( cos(x) );

그림 小3 아ext 명령어를 이용한 코딩 결과

Oads 명령어를 이용하여 工축의 범위는 0 라디안부터 2兀 라디안까지, y축의 범위는 -1부터 1까
지 지정한다．
0 xlabel, ylab이 명령어를 이용하여 工축과y축의 이름을 지정한다．
0 title 명령어를 이용하여 그래프의 제목을 지정한다．
0 grid 명령어를 이용하여 그래프에 모눈을 생성한다．
0 사인 함수와 코싸인 함수를 나타내는 두 선이 쉽게 구별되도록 gtext 명령어를 사용한다. 필요한 수
만큼 gtext 명령어를 입력하면［그림 4-4］와 같이 문자열의 위치 선정을 위한 십자선이 나타난다. 문
자가 위치할곳을 클릭하면［그림 午5］와같이 문자가삽입된다.
태I 邸1 Vhm

加m1 相此

r느吐螂1

늬5

W

HI印

쩍

D 心 a 的 斗 \ q1 1 自小 4 , a 口 툐크 ..
斟near넙 Co出la Fur（心머l

4
1

08
0,6

\

04

듐

「

/’

0 02

「

\\

0
> {L2

「

-04
七6

= 1

. .

\\

-08

/

\

0

1

2

3

4

Ra비anV81t始

그림 小4 문자열의 위치 선정을 위한 십자선

76

PART02. M戶JU\B 핵심 기능 익히기

,/

a

.

6

F甘帥 SCm, 邱uio roots ［地5蚣Op 幽岫汁
므J 巴 日 色 1 b 1 曳 曳 的 兮 뻗 d '

14的P

曼 口目

U口

미no 키너 Co닯08 Function

的
M
0
m

m호료： g}

吐
鈿
幽
鈿
2

4
3
Radian Valt用

5

그림 午5 gtext 명령어를 이용한 실행 결과

/n

口mm크nd 냄／m曲刎
>> X＝口pill日0: 2士口 i ;
>> 비＝引0(0) :
>' y2ocos(o) ;
>> plot (e,yl,x, y2, : ) ;
Warning: H A1LAB has disabled some advanced graphics rendering features by s川tching to
soft甲are 0pen吼. For more information, cl ick here
>> ax油([ 0 小p1 七1 II) :
>> 키 abel (Radian ha 山e ) ;
>> 미ab이 (. 卄的Ti tude ) ;
,> titfe (Sine and Cosine Function ) ;
>> text (3. O,0.5, sin(v) ') ;4
>> teot (I. 5,-0. 6. 'cos(o) );

그림 4十 text 명령어를 이용한 코딩 결과

0 妃xt 명령어로工 좌표 3.0과y 좌표 0.5를 지정하여 (3.0, 0.5）에 문자열 '駐n似）'를 표시한다．
0 把xt 명령어로工 좌표 1.5와y 좌표 -0.6을 지정하여 (1.5, -0.6）에 문자열 'cos似）'를 표시한다．
PS. 帥t

W曲 b eet

！그 t3 니 由

t뇽

Tools

Do＄比｛) 베ado나

4ef口

' \ -' 1) 包 욧 J二 , 已 口 匡크

U 口1

Sine a,녑 Co引ne Function

1
Se
06
0.4
/
/

0
\,

m

쁨글듬m>

吐

1

「＼

(b)

m
批

仗뼈of

\',

部

,

0
d

,\'\

2

3
4
！相dian Va山0

,,

,;

C

그림 午7 text 명령어를 이용한 실행 결과

CHAPTER 04. 데이터를한눈에 보는그래프

77

legend

I

각그래프에 대한내용을 'si', 's2', ··· 등문자열 형태로지정하여 범례 형태로표시하는legend 명령어의
기본 형태는 다음과 같다．
legend('s1','s2', · , 'Location', 'Legend location')
· 'si', 's2느 범례로표시할그래프의 이륨
· 'Locat油nH 기본 정의 설정
· 'Legend 佃cation' : 그림 창 안에서 범례의 동서남북 표시 위치를 자동으로 지정하는 역할을 한다. 예를 들어 왼쪽 아래는 'SW,.
왼쪽 위는 'nW,, 오른쪽 아래는 'se'. 오른쪽 위는 ne' 등으로 지정한다．

加t 명령어에 사용한순서대로문자열을 지정하며, 반드시 하ot 명령어를사용한후에 사용해야한다. 또
한표시된 범례는 마우스 왼쪽 버튼을누른 채 드래그하면 원하는 위치로 이동할수 있다. legend 명령어
를사용하지 않고도 듣크 ［범례 십쉽］버튼을클릭하면 범려］가표시된다．
예를 들어 제어공학에서 감쇠비 값의 변화어］ 따른 계단 응답의 결과를 비교하려 할 때 入4ATLAB에서
legend 명령어를 사용하면 범례를 표시하여 여러 그래프를 비교할수 있다. 다음은 9장의 ［예제 아13]
에서 다루는CtrlDan巾Rt.m의 일부와그 결과이다．

t=0:o.1:io;
···（생략）

F加

Edt

VH毗

t,el.t

To에r月呻口蜘

He巾

!J d 日 全 4 1 (j\ 戈 的自嶼 而 r 邑 口 區｝ 固 口1
Un作 Step Resp 川se

plot (t,y (1:101,1),'r-');
h이d:
加t (t,y (1:101,2) , l戶）;
··＜생략）
legend ('\ zeta=0.0', ' \zeta=0.2',
'\ zeta=0. 5', ' \zeta=0,8', '\ zeta=1.0',4);
10

1 예저'4- 3 I
0< x< 2兀에 위치한 사인 함수 Yi = Sj可x)와 코사인 함수 Y2 = CO吼x)에 대한 그래프를 그리려 한다. 주
기는 'rIl80 라디안이며, x축 이름은 'Radian Value', y축 이름은 'Magni恤Je', 그래프 제목은 'Sine and
Cosine Function'으로 지정한다. egend 명령어를 이용하여 그래프의 왼쪽 아래에 計n(x)와 Co吼D의 범례
를 표시하라．

78

PART02.卜肛ILAB핵심 기능익히71

풀이

Command 바4nd小月
x=O:pi/lOO: 2*pi ;
미＝引 n(n ;
y2=cos（的 ;
이ot (x，미 ,x,y2, ' r ) ; 0
axis([ 0 2*pi -l 11) ;
nlabel ( 'Radian Value ') ;
ylabel ( 'Magnitude ') ;
tltle ( 'Sine and Cosine Function' );
I egend( ’引n佃匕 'cos似匕 'Locat I nn '

鈿thWest ) ; 0

그림 午8 恒gend 명령어를 이용한 코딩 결과

0 벡터 yl은 실선으로 그래프를 그리고，
벡터 y2는 점선으로 그래프를 그린다．

i 1 악曳 心自嘆 J= r 鼠 口 區卜 a 口
미no and Co川no Function

0 plot 명령어의 괄호 안과 동일한 순서로
legend 명령어의 괄호 안을 입력하고，
범례 위치를 왼쪽 아래로 지정한다. 범
려］ 위치를 지정할 때는 대문자나 소문자
어느 것을 사용해도 무방하며, 전체 이
름（'SouthWest' ) 혹은 머리글자（'SW,
또는 'SW,）를 사용해도 된다．

그림 4四 b9eM 명령어를 이용한 실행 결과

I

subplot

주어진 그래프 결과를 차례대로 쉽게 비교하기 위해 그림 창을 분할하여 그리는 S的plot 명령어의 기본
형태는다음과같다．
subplot(mnp)
·m: 그림 창 안에 분할하려는 행의 개수
.n: 그림 창 안에 분할하려는 열의 개수
· P: 그래프가 나타날 분할된 칸의 위치

sub하아（mnp) 명령어를사용할 때 p는 행과 열을곱한수보다큰수를 지정할수 없으며, 반드시 plot
명령에 이전어］실행되어야한다．
예를 들어 제어공학에서 임펄스 응답의 결과와 계단 응답의 결과를 비교하려 할 때 MATLAB에서
subplot 명령어를 사용하면 한 그림 창에서 두 그래프를 비교할 수 있다. 다음은 9장의 ［여께 9-5］에서
다루는TfResp.m의 일부와그 결과이다．

CHAPTER 04. 데이터를 한눈에 보는그래프

79

t=o:o.01:io;

R巨

6411 너e冽

l,6e,t 1006

···（생략）

3

4
5
6
Tin祀（nec)
Step Response

3

4

subplot (211) ;
11
Cd

·．K생략）

0
g＝ 돛 甘 ＜

plot (t,yimp);

盈 口

1mpulse Resp기se

0
5
n

y_st=step (G_s,t) ;

He巾

5 0
0
띠
乙
쿠
＝口
E<

yimp=impulse (Gs,t) ;

\00,40w

1

G_s=tf (num,den) ;

00朴：S叩

.. 」': 兮 七j 1= , 已 ［그 i그

subplot (212) ;
plot (t,y_st) ;

5
6
Time(sec)

7

8

9

10

·．·（생략）

figure

I

여러 그래프를 각각 다른 그림 창에 그리키 위해 그림 창을 생성하는figure 명령어의 기본 형태는 다음과
같다．
figure(n)
. n: 그림 창의 번호（지정하지 않으면 자동으로 지정됨）

1 예제4- 4 I
0 드 x 드 2?r에 위치한 사인 함수Yi = sin仁）와 코叭r인 함수 Y2 = CO町x)에 대한 그래프를 한 그림 창 안에 각
각 분할된 2개의 그래프로 그리려 한다. 주기는 7t1180 라디안이며, x축 이름은 '日adian Value', y축 이름은
‘卜Aagnitude', 각그래프의 제목은 'Sine Function', 'Cosine Function'으로 지정한다．
(a) subplot 명령어를 이용하여 두 그래프를 좌우로 분할하여 그려라，
(b) sub이아 명령어를 이용하여 두 그래프를 상하로 분할하여 그려라．
(c) figure 명령어를 이용하여 두 그래프를 두 그림 창에 각각 그려라．

80

PART02. MAT녀B핵심 기농익히기

(a)

Comn口：口 :1

巨）

>> x=O:pj/180:2,pi ;
>> 미＝引n(x) ;
>> y2丸os(a) ;

>, subplot (121); e

)> pIot (x』,1) ;
>> axis(I0 2시놔 中1 ii) ;
>> 뉘ab이 ( 日adlan Va山a ) ;

>> ylabel (Masnitude ') ;
>, title (Sine Function' );

>> subplot (122); e

>> plot (x .t,2) ;
>>axis([02*pl -l 1] );
>> xlabel (Radian Value ');
>> ylabel ( Masnitude ') ;
>> tit leC ' Cosine Funct inn ) ;
그림 4너0 얹jbpk乂 명령어를 이용한 코딩 결과

0 subplot (1기 ) 명령어를 이용하여 함수 刃의 그래프를그림 창 왼쪽에 그린다．
0 subp幻t (122) 명령어를 이용하여 함수 Y2의 그래프를그림 창오른쪽에 그린다．
F陌 E｛奴 ＼艇시Y 娜et TO여5 De心t아1 \8ndaw He'p
{J d 日 邕 i 다 1 曳 曳 吻自嘔 / ' 目 口 토크 U 口
Co寸ne Functon

SWia F미出lion
0.8
0.6

0

4 2 0 2
0 0
4
g
＝芒旨五

M 吐 0 m 小 批 幽
量d론g}
-1

풀0

2
4
F相마any미此

6

그림 4-11 좌우로 나타난 subplot 명령에 실행 결과

(h)
>> a=O:pl/1田:2.pi ;
>> 미＝引n(幼 ;
>> y2=cos(tt) ;

>> subplot (211); e

>> F니ot (x . 미）;
>> ax冶（10 2士p1 -I 11) ;
,> xlabel (Radlan Value' );
>> ylabel ( 'tlagnitude ') ;
>' tltle ( 'Sine Function ');
>> subplot（기기 ; C
>> plot (x, y2) ;
>, axisU0 2.pl -1 11) ;
>> xlabel ( 'Radlan Value ');
>> ylabel ( 'liasnltude ') ;
>Dtltle(Cosine Function ') ;
그림 午12 텨Jb口k乂 명령어를 이용한 코딩 결과

CHAPTER 04. 데이터를 한눈에 보는그래프

81

0 subplot (211) 명령어를 이용하여 함수乃 의 그래프를 그림 창 위쪽에 그린다．
0 subr加t (212) 명령어를 이용하여 함수Y2의 그래프를 그림 창 아래쪽에 그린다．
日由

帥t

p／卜叫5

IraeO

Too뇹

De51tnP

냉1M畔

Is印

D ta 日曲 1 4 } a可曳 凸自 興 在 니 目 日 툐크 ! . 口
Sine Functbn
5
5 0
0
0
쁨글旨m듣
2

3
IR台出an V川此

5

6

5

6

Co미ste Functi아1

0

쁨글C冒듣

的
幽
0
d

3

2

4

由d目nVah此

그림 4中13 상하로 나타난 subplot 명령에 실행 결과

(c)

（兮
>> o=O:pl/ l凹：2.pi ;
>> 미＝sin(s) ;
>3 p2=cos (x) ;
>> figure(I)

>> 미ot佃p1) ;
>> ax b8o [o 칸p1 나 I) );
>> 小ab이 ( II如泊nValue' );
>> 비ab이 (Sagnitude' );
>> titl이Sine Function ) ;

0

>> 1 igure(2)
>3 ptot (o.y2) ;
>> aois(F0 2up1 -1 II) ;
>> 있ab이(.由띠an Value );
>> 미ab이 0 貶unit ude ) ;
>> tltle ( 'Cusine Function' );

그림 4-14 均ure 명령어를 이용한 코딩 결과

0 figure 명령어를 이용하여 그림 창（figure 1）을생성한다．
0 figure 명령어를 이용하여 그림 창（fi옘配 2）을생성한다．
5'.

咀

01心 1甘St Ta出 SIan叩

0665야1 쌔的m Hap

出h너汁 1＋탸P

{) d 日 色 } b 曳 曳 凸 自 딛 dL

a

口 들크

兮 4? J{ , 邑 口 區크

a 口

Co늬no Fur比Is口n

Sne Func出)0
u.s
吐

0.6

M

04

그림 4-15 두그림 창에 나타난幻U尼 명령에 실행 결과

82

PART02. MATLAB핵심 기눙익히기

m

5

0

쁨글듬m즈

m
3
4
F뇹曲nVak,e

叱

0

各릍gi

吐
2

3
4
什吼幻nt/ak月

a 口1

I

그래프 저장하고 불러오'I

入4AThAB에서는 그림 창어］ 나타낸 그래프를 저장할 수 있다． 방법 ] 그림 창의 메뉴 표시줄에서 [File]
-[Save As... ] 메뉴를클릭하고저장할파일이름에확장자（.f琯）를붙여서 저장하거나, 방법2 명령 창
에서 saveas 명령어를 사용하여 그래프를 저장할 수 있다. 그래프를 'Filename.f增'로 저장하는 saveas
명령어의 기본 형태는 다음과 같다．
saveas佃此 'Fit이iame', 'f呵）
·gcf: 저장할 파일이 그래프임을 지정하는 파일 형식
. 'Filename': 저장할 파일 이름
· 'fig': MATLAB의 그림 파일 확장자 형식

또한 방법 ] 그림 창의 메뉴표시줄에서 [File] - [Open... ] 메뉴를클릭하여 사용하려는그림 파일을두
번 클릭하거나， 방법 2 명령 창에서 openfig 명령어를 사용하여 그래프를 불러올 수 있다. 'Filename.
fig' 파일을불러오는叩e出g 명령어의 기본 형태는 다음과같다．
openfig('Filename')

CHAPTER 04. 데이터를한눈에 보는그래프

83

LESSON

03

3차원 그래프 그리기

그래프를 입체적으로 생성할 수 있는 3차원 그래프 그리71 명령어를 알아보자．

1 p10t3 1 meshgrid I mesh 1 su汗 I contour I meshc I meshz I waterfall I

Keyword

1 3차원 그래프의 모양과종류 1

I

이아3

x축, y축, z축의 직선을 서로 연결하여 3차원 공간어］차례로 그리는 p1아3 명령어의 기본 형태는 다음과
같다．

4弓

plot3(x,y,z)
, 凡뇨工 동일한 원소의 수를 가진 벡터

1 예제 4- 5 I
다음 방정식은 시간 변수／가 변화함에 따라서 3차원 곡선을 생성한다．
x ==cost, y= slnt, z =t
t가 0에서 15兀까지 兀／30씩 증가할 때 이아3 명령어를 이용하여 3차원 그래프를 그려라. 축 이름은 각각
뇨ax洽 ', '少ax恰 ', '乃a川S'로 지정하라．

풀이

쿄mm引］d 心Lndr그六
>> t =0:p／羽：15＋口i ;
>) s=cos(t) ;
>> S＝引n(t) ;
>> z=t;

)> pIot3(x,y』z); <1
>> xlabel ( x-aais ); 0
>> 미 abel ( s-asi 可 ) ;
>> 기 abel ( 十ax is ) ;

>> grid; 0

그림 4-16 이아3 명령어를 이용한 코딩 결과

0 plot3 명령어를 이용하여 3차원 그래프를 그린다．
0 xlabel, ylabel, 기abel 명령어를 이용하여 工, y, z축 이름을 지정한다．
0 그래프어］모눈을 그린다．

84

PART02. M戶끄AB 핵심 기능 익히기

그림 4-17 口b日 명령어를 이용한 실행 결과

I

meshgrid

벡터 x와 y로 지정된 영역을 3차원 그래프로 나타내려면 두 변수x와y를 배열 x와 Y 형태로 변환해야
한다. 이때 사용하는meshgrid 명령어의 기본 형태는 다음과 같다．
[X, Y] = meshgrid(x, y)
· 乂Y: 배열로 나타난 결과
· 凡 y: 배열로 나타낼 벡터 또는 변수

I

mesh

배열 x와y의 함수로구성된 z의 그래프（z = f (x,y)）를그리는mesh 명령어의 기본형태는다음과긷다．
mesh（凡％z)
· 凡y: 축 정보가 저장된 배열
· Z: 배열 x. y의 값으로 이루어진 배열

L亡斗

mesh 명령어를 이용하면 3차원 격자무늬를 그릴 수 있다. 이때 洲 비례하여 표면의 높이와 그래프의 색
상이 결정된다．

CHAPTER 04. 데이터를 한눈에 보는그래프

85

I surf
3차원 격자무늬어］색을 채워 그리는 surf 명령어의 기본 형태는 다음과 같다．

呼
臂
澍

. 凡 y: 표면의 구성 요소를 정의하는 벡터
·z: x, y로 표현된 식 또는 벡터

surf 명령어는 함수의 모든 곡면에 색을 채워 그려주므로 mesh 명령어를 사용했을 때보다 색이 더 뚜렷
하다. 이때 z어］비례하여 표면의 높이와그래프의 색상히 결정된다．

I contour
x와y를 이용하여 z의 값을2차원등고선 그래프로나타내는Co曲ur 명령어의 기본형태는다음과긷다．

: 凡 y: 工축과y축의 한겨를 결정하는 벡터

0

心）

contour(x,y,z)
' Z: 瓦 y로 표현된 식 또는 벡터

1 예제4小 1
-3<工 <3과日 5y 5 3에 0.1 간격으로 놓여 있는 함수 z ＝工2ey2이 있다. 3개의 축 이름은 각각 'x小axis'.
'y田x洽', 'z-axis'로지정하라．
(a) mesh 명령어를 이용하여 3차원 격자무늬를 그려라．
(b) su卄 명령어를 이용하여 3차원 격자뮈닉 사이에 색을 채워 그려라．
(c) contour 명령어를 이용하여 2차원 등고선을 그려라．

系； （旬

Command Window

>> Ix，小.eshgrid(-帥J :3L e
>> z=x．八2-y．八2;
>> 1esh(x.y.z);'Q

>> xlabel( 'x-axis'); e
>> 비ab이 C 少axis ') ;
>> 기abe I ( 'z口axis ') ;

그림 4너8 mesh 명령어를 이용한 코딩 결과

0 meshgrid 명령어를 이용하여 工, y의 범위를동시어］벡터로 표현한다．
0 mesh 명령어를 이용하여 3차원 격자무늬를 그린다．
Oxi的el, ylabel, ziabel 명령어를 이용하여 工, y, z축 이름을 지정한다．

86

다\RT 02. MAT녀B핵심 기능 익히71

日It

vIw

In蛇a

Too놈

Do針To口

THTdOW

He巾

｛그 t三 니 今 自 ' , ;. 凸自 +J != , 口 ［그 回 曲 ［口

m又m1N

그림 4-19 m크sh 명령어를 이용한 실행 결과

(h)

(9

Command 냄긔ndo叫
>> [x, y] =meshgrid(_3: 0, 1 : 3) ; C
>> Z=X．八2-y．八2;
>> surf (x』

;

0

z)

y,

>> xlabel ( 's-axis '); O
>> 미 abel ( 少an 油 ' ) ;
>> zlabel ( 'z-axis ') ;
그림 小20 surf 명령어를 이용한 코딩 결과

On比shgrid 명령어를 이용하여 x, y의 범위를 동시어］벡터로 표현한다．
0 surf 명령어를 이용하여 3차원 격자무늬에 색을 채워 그린다．
0 넜abel, ylabel, 기abel 명령어를 이용하여 工, y, z축 이름을 지정한다．
Ed吐

\04W

SuIt

0｛刃I4

DWkt마） 쌔odow

H미P

n2

mn'-- , 抑 自 宴 / , 目 口 덥 . 口1

y日X出

-4

-4

(c)

그림 十21 surf 명령어를 이용한 실행 결과

Comm帥d 쌔ndo나

군）

>> [x,yj=meshgrid(-3:0. l :3); e
,> z-X. A2-y. 八2;

>> contourCx』',z); O
>> xlabel(' x-aais' ); O
>> 미 帥引 ( ' a小a川 s ') ;

그립 中刀 （刃nt(기r 명령어를 이용한 코딩 결과

CHAPTER 04. 데이터를한눈에 보는그래프

87

0 meshgrid 명령어를 이용하여 工, y
의 범위를 동시어］벡터로 표현한다．

F가o

Ed仕

\／伯W

1flF머I

T洲5

m嫌top

놔在m片

Fi醉1

口 ,J a 4J 다 ' , , 4『『）自咽 / H 匐 ［그 區크

0 contour 명령어를 이용하여 2차원
등고선을 그린다．
0 xlabel, ylabel 명령어를 이용하여
工, y축 이름을 지정한다．
1n}

contour는 3차원 그래프를 그리는
명령어이지만, 2차원 등고선 그래
프를 묘사하'I 때문에 기abel 명령
어를 쓸 필요가 없다．

그림 午23 contour 명령어를 이용한 실행 결과

I meshc
3차원 격자무늬 그래프와등고선을 함께 그리는 meshc 명령어의 기본 형태는 다음과 같다．
n犯針｝C偶또z)
, 凡V: 축에 대한 정보가 저장된 배열
· Z: 배열 x, y의 값으로 이루어진 배열

예를 들어 전자끼학에서는 특정한 점에서의 전기 에너지 분포인 전위의 형태를 알아보기 위해 전위를 그
래프로 나타낸다. MATLAB에서는 meshc 명령어를 이용하여 전위의 형태를 3차원 그래프로 나타낼 수
있다. 다음은 11장의 ［예제 11-23］에서 다루는Potential.m의 일부와그 결과이다．

．·，（생략）

디匣

[xy] = meshgrid(-O.25:0.025:0.25) ;
·．K생략）
v= (1/ (4*pi*epsionOfl* (ql./rl+
q2./r2) ;
meshc (x,y,V);
xlabel('x'),

88

')

(

'z

ziabel

ylabel Cv');
;

PART02. M月FLAB 핵심 기능 익히기

Ed忙

\dew

I,玎e吐

To마5

［乂出op

叫1的口거V

Help

그 J di 由 뇨 ' , , ｛孕自몇 石 니 骨 口 匡갚 曲 口

I meshz
x축과y축 양방향으로 수직선을 그리는 3차원 격자무늬 그래프와 장막을 함께 그리는 meshz 명령어의
기본 형태는 다음과 같다．
meshz似,y,z)
· 凡y: 축에 대한 정보가 저장된 배열
.z: 배열 x. y의 값으로 이루어진 배열

waterfall

I

工축 또는y축 한 방향으로 수직선을 그리며 폭포 형태를 생성하는 \waterfall 명령어의 기본 형태는 다음
과같다．
waterIall(x,y,z)
, 凡y: 축에 대한 정보가 저장된 배열
· Z: 배열 x. y의 값으로 이루어진 배열

1 예저14- 7 I

I1m

I

-3 5工5 3과 小3 5y 53에 0.1 간격으로 놓여 있는 함수 z ＝工2 中2y2이 있다.3개의 축 이름은 각각 '卜 axis'.
'少ax恰', 'z-axis'로 지정하라．

(a) meshc 명령어를 이용하여 3차원 격자무늬 그래프와 등고선을 함께 그려라．
(b) meshz 명령어를 이용하여 3차원 격자무늬 그래프와 장막을 함께 그려라．
(c) w欲e片all 명령어를 이용하여 3차원 수직선 그래므라 폭포 형태의 그래프를 함께 그려라．
.

oI

乙二ri기man2 心md口n
(a)

=

>> [x』y] =meshgrid(-31J. l : 3) ; 0
>> z=x戶？y戶2;

>> meshc(x,y,z); e
>> xlabel('x-axis'); e

>> 미 abel ( ' y叫ax 油 ' ) ;
>> 기 的el ( 'z-a< I s ) ;

그림 十24 n毛寸'K; 명령어를 이용한 코딩 결과

0 meshgrid 명령어를 이용하여 工, y의 범위를동시에 벡터로 표현한다．
0 meshc 명령어를 이용하여 3차원 격자무늬 그래프와등고선을 함께 그린다．
0 xlabel, ylabel, 기abel 명령어를 이용하여 工, y, z축 이름을 지정한다．

CHAPTER 04. 데이터믈 한눈에보는그래프

89

그림 午25 me삵（ 명령어를 이용한 실행 결과

(h)

Command WindoVr
>> 1 x, y] =meshgrid(-3: Q. 1:3) ; 0
>> Z=X．八2-y戶2;

>> meshz(x,y, z);Q
>> xlabel(艸小出 0
>, ylabel ( 'y-aais' );
>> zlabel ( 'z-axis ');

그림 午而 rT毛shz 명령어를 이용한 코딩 결과

0 meshgrid 명령어를 이용하여 工, y의 범위를동시에 벡터로 표현한다．
0 meshz 명령어를 이용하여 3차원 격자무늬 그래프와 장막을 함께 그린다．
0 xlabel, ylabel, ziabel 명령어를 이용하여 工, y, z축 이름을 지정한다．

D 凸 a $ 1 自 1 戈 民 抑自 咽 d , 目

그림 午27 meshz 명령어를 이용한 실행 결과

90

PART 02. MAT나＼B 핵심 기능 익히기

口 듣크 U 工工1

(C)

e)

Command Window

>> [x,yl=rneshyrid(寸O.l:3);O
>> Z=X 戶？y. 坦；

>> watertal l(e,y,z); e
>> elabel ( 'o-a is'); e

>> ylabel ( ' '-aeis ') ;
,> zlabel ( 'z-axis ) ;

그림 午羽 waterfall 명령어를 이용한 코딩 결과

0 meshgrid 명령어를 이용하여 x, y의 범위를동시에 벡터로 표현한다．
0 waterfall 명령어를 이용하여 3차원 수직선 그래프와폭포 형태의 그래프를 함께 그린다．
0 xlabel, ylabel, ziabel 명령어를 이용하여 工, y, z축 이름을 지정한다．
F카e

Ed作

＼加w

Inse仕

Ti刃놈

De

平

쎄IN土汁

Help

1

:) 口 a 小 臣 ' \ \ 抑 包 嗔 /= n 圃 t} 匡크 ! 1 口

5
0

m又m1N

巧

그림 十29 wat여all 명령어를 이용한 실행 결과

CHAPTER 04. 데이터플한눈에 보는그래프

91

1 3차원 그래프의 모양과 종류
격자무늬 그래쏘F
막대 그래프

공간 그래區

이아3(X,Y.Z)

mesh(X,Y,Z)

口e3V,exI加de)

contour3(X,Y,Z)

meshc(X,Y,Z)

fl113(X,YZ,C)

quiver3(x,y,z,u,
v,w)

sca仗아3(X,YZ.S,（가

comet3(x,y,z)

coneplot休,Y,Z,U,V,
W,Cx,Cy,Cz)

납二 L：望

七包

迂弓

체적 그리i프

毛包

선 그래匹

su呱X,Y.Z)

contourshce(X,Y,
Z,V,Sx,Sy,Sz)

匐k
= 'I= 枉

ezp幻t3(funx,funy,
funz)

meshz(X.Y,Z)

surfc(X,Y,Z)

唾뇨 可1 邕
ezmesh(fun)

cylinder (X,Y,긱 =
cylinde巾）

ezsurf (fun)

口， 令

返弓
stem3(X,Y,Z)

ellipsoid 氏y,z] =
e呻）S이d(xc.yc,
zc,xr,yr.zr)

bar3CY)

sphere(n)

ezsurfc(fun)

streamslice
侃Y나V)

m客

streamline休,Y,Z,U,\(
W,startx,starty,startz)

streamribbon休,Y,Z,
U,\(W,startx,starty,
startz)

唾

streamtube0<,Y,Z,U,
V,W,sta比x絿arty, startz)

毛됴

waterfall(X,Y,Z)

patch恍Y.C)

玉드

羲唯

逢三

bar3h(Y)

92

PART 02. M戶MB 핵심 기능 익히71

U色

뇨

（

CHAPTER

05

CONTEN 了 S
LESSON 01 관7I 연산자 사용하71
LESSON 02 논리 연산자 사용하기
LESSON 03 조건문 사용하기
LESSON 04 순환문 사용하기
LESSON 05 사용자정의함수 작성하기

LESSON

01

관겨I 연산자 사용하기

관:7非 연산자는 논리적인 수식을 표현할 때 쓰인다. 논리는 그 결과를 '참', '거짓'으로 출력하며, 이는 논리적인 수식을 표현하
는 데 활용할 수 있다. 특히 MAT나＼BO似1 프로그래밍을 할 때 조건문 또는 순환문의 '조건'에 자주 사용되는 관:
7非 연산자어i
대히1 살펴보자．

Keyword

I

I A (B 1 A 仁B I A) B I A> B I A= B 1 AnJ= B I

관겨1 연산자

관계 연산지는 두 벡티의 같은 위치어］놓인 원소를 비교하는 연산자이다. 관계 연산자의 결과는 '참'이면
'l '로, ' 거짓'이면 ' 0 '으로 나타난다. 부등호와등호를 함꼐 쓰는 관계 연산자를 사용할 경우, 반드시 부등
호를 먼저 사용하고 부등호와등호를 붙여서 써야 한다. 변수와 부등호 사이에는 공백을 넣어도 상관없다．
관계 연산자와그 의미를 ［표 5-1] 에 정리했다．
표 5너 관계 연산자

의미

연산자

의미

A (B

A는 B보다 작다．

A (= B

A는 B보다 작거나 같다

A) B

A는 B보다 크다．

A )= B

A는 B보다 크거나 같다．

A == B

A와 B는 같다．

A N= B

A와 B는 같지 않다．

연산자

1 예제 5- 1 I
벡터 x = [8,-2工4,-il과 y = [9,-1,5,4,--기를 지정하고，관7카 연산자를 이용하여 다음 연산 결과를 확인弓巳F.

(a) 벡터 x에서 l보다 작은 값인 원소를 찾아라．
(b) 벡터 x가 벡터 y보다 작거나 같은 값인 원소를 찾아라．
(c) 벡터 x가 벡터 y와 같은 값인 원소를 찾아라．
(d) 벡터 x가 벡터 y와 같은 값이 아닌 원소를 찾아라．

94

PA日T 02. MATLAB 핵심 기능 익히:7 '

Commond lyinch1';

()

>> a = [8, -2,1,4,-li; 0

>> zl =

(e<

>> y = 19.-1,5, 4. 小21 ;

I) 0

zl =
0

I

0

0

I

1

1

0

>> 22 : (a＜剖 0
z2 =
1

1

>> z2 = (x< =y) e
z2 = (v'c =y)

t
Error: The expreosion to the left ef the equals sign ie not a val id target for 크r:
asnianment.

'> z2 = (e='cy) e
z2 = (v='cy)

t
Error: The eepression to the left of the equals sign is not a val id target far an
ass i gnneet1

e

>> z3 = (e=y) 0
z3 =
0

0

0

I

0

1

0

1

>> z4 = 佃＝y) e
z4 =
1

1

그림 5너 관계 연산자실행 결과

(a) 먼저 등호를 이용하여 x, y를 지정한다佃I).
(b) 벡터 x의 원소 중 l보다 작은 원소라면 그 자리어］ l을 지정하고, 1보다 크거나 같으면 0을 지정한 결과
를 벡터 zi어］지정한다（回．
(c) 벡터 x의 원소 중 y의 원소보다 작거나 같은 원소라면 그 자리어］ l을 지정하고, y의 원소보다 크면 0을
지정한 결과를 벡터 z2어］지정한다（O) . 이때 부등호와 등호가 함께 쓰이는 관계 연산자를 사용하는 경
우 등호와 부등호 사이에 공백이 있으면（回 오류 메시지 (0）가 나타난다. 또한 부등호와 등호가 함께
쓰이는관계 연산자를 사용하는 경우 등호를 부등호 앞어注끼하면（回 오류 메시지 (O）가 나타난다.
(d) 벡터 工으i 원소 중 y의 원소와 값이 같으면 그 자리어］ 1을 지정하고, y의 원소와 다르면 0을 지정한 결과
를 벡터 z3에 지정한다（O).
(e) 벡터 x의 원소 중y의 원소와값이 다르면 그 자리에 1을 지정하고，y의 원소와 같으면 0을 지정한 결과
를 벡터 z4에 지정한다（回．

CHAPTER 05. 흐름올 바꾸는프로그래밍

95

LESSON

02

논리 연산자 사용하기

논리 연산자는 관계 연산자와 함께 논리적인 수식을 표현할 때1 사용한다. 특히 MAT녀B에서 프로그래밍을 할 따1 조건문 또는
순환문의 '조건'에 논리 연산자를 자주 사용하므로 유의하여 알아보자．
I A& B I AIB I " 'A

Keyword

I

I AXORB I

논리 연산자

논리 연산자는 벡터의 원소가 0이 아닌（no'也er이 경우는 '참인 값으로, 0인（zer이 경우는 '거짓'인 값
으로 지정한다．
&(AND) 논리 연산자는 두 벡터의 같은 위치에 놓인 원소가 모두 0이 아닌 경우에만 '1' 의 값을 지정한
다. 1 幻R) 논리 연산자는 원소가 모두 0인 경우를 제외하고 그 결과를 '1'로 지정한다. N(NOT) 논리
연산자는 벡터 원소의 '참', '거짓'을반전한 결과를 지정한다. ）幻R (A. B）는（시B) -(A&B）와같은
결과를 지정한다．
이를［표 5-2] 에 정리했다．
표 千2 논리 연산자

m

A& B

시B

AXOR B

"A

A

0

zero

zero

0

0

zero

nonzero

0

j

l

nonzero

zero

0

]

0

nonzero

nonzero

]

日II} 的R) 논리 연산자는 囹皿 + 回 키를 눌러 입력할 수 있다．

96

PART02. M月ThAB핵심 기농익히기

0

]

0

1 예제 5- 2 I
벡터 工 =[-4,-1,0, 2, 3,9］와 y = [-2,0,0,1, 4,7］이 있다．

(a) 벡터 x와 벡터 y에 &(AND) 논리 연산자를 실행하라．
(b) 벡터 x와 벡터 y에 1(OR) 논리 연산자를 실행하라．
(c) 벡터 x에 '(NoT) 논리 연산자를 실행한 결과 중어써 벡터 y보다 큰 값인 원소를 찾아라．

풀이

C口rr그mand ' 'in出y斗
>> X =E-4.-1,0.2, 3.9] ;

>' y= L-2, O.O.L4J7] ;
>> 기＝x&y 0
z1 =
1

0

0

1

1

1

0

1

1

1

1

0

0

0

>> z2＝川y e
z2 =

1

0

그림 5丑 논리 연산자 실행 결과

(a) 벡터 x, y를＆(AND) 연산한값을zi에 지정하고 결과를확인한다（이．
(b) 벡터 x, y를 (OR) 연산한값을끄에 지정하고 결과를확인한다（回．
(c) 벡터 x에 =(NoT) 연산한 값이 벡터 y보다 큰 원소의 자리어］ l을 나타내고 그 값을 z어］ 지정한후 결
과를확인한다（O).

CHAPTER 05. 흐름을 바꾸는프로그래밍

97

LESSON

03

조건문 사용하기

MATLAB에서 조건의 참과 거짓을 판단하여 흐름을 변경하는 if, 派이se, 이se作 조건문에 대하1 알아보자．
Keyword

I if문 1 牛이se문 ! else作문 1 end I

if문

I

if문은 순차적 알고리즘의 흐름을 변경할 때 사용한다. 영어에서 if가 들어 있는 문장은 '만일 ···한다면 ···
할 것이다’로 해석되는데, 八4ATLAB의 if문도 이와 같은 의미로 사용된다. 제시된 조건이 '참'이면 알고리
즘의 변경 없이 차례대로 순차적 알고리즘이 진행되지만, '거짓'이면 더 이상 순차적 알고리즘을 진행할
수 없다. if문의 기본 형태는 다음과 같다．
갚纛쏘

if lo暫cal express幻n
statement
end
if 명령에 다음에는 관계 연산자 또는 논리 연산자 등을 이용한 논리적인 수식을 사용한다. 함수를 표현할
때 여는 괄호로 시작하고 닫는 괄호로 끝내는 것과 같이 if 명령어로 시작하면 반드시 end 명령어로 종료
해야한다. 위의 기본형태에서는 'logical expres針on' 조건이 '참'이면 'statement'를 실행하고if문을종
료한다. 그러나 'lo昏cal expression' 조건이 '거짓'이면 'statement'를 실행하지 않고 end 명령에 밖으로
빠져나간다．

I

if- e怜e문

小else문은 제시된 조건의 '참’ 또는 '거짓'을 구별한 후 그 결과어］따라 프로그램을 수행한다. if- el配문은
if 명령에, else 명령에, end 명령어의 순서로 진행되어야한다. if-else문의 기본형태는다음과같다．
if logical expression
statementi
이se
statement2
end

98

PART02. M戶m\B 핵심 기능 익히71

만약 'logical expression' 조건이 '챰이면 'statementi'을 실행한 후 end 명령에 밖으로 빠쪄나가지만，
'logical express幻n' 조건이 '거짓'이면 'statemen口'를 실행한후end 명령에 밖으로 빠져나간다．

I 이se汗문
논리적인 수식 조건이 2개 이상인 경우에는 알고리즘의 흐름을 다양하게 제어하기 위해 if-else문어］
elseif문을 덧붙여 사용할 수 있다. else正문은 if문처럼 새로운논리 수식을통하1 조건을 비교하는 데 쓰인
다. if문과 else문 사이에는 여러 개의 else迂문을 사용할 수 있고, else문은 반드시 맨 마지막어］사용하는
elseif문다음어］작성해야한다. elseif문의 기본 형태는 다음과같다．
玄多1

毋＝

'

나磁羅m斟難難難響瓣攝難難望秘難醬難茗裂好激督鞋豁多恥小曜籌難群m出羅客臂“
立心烈毋好8너吐 m好恥믄
g
口孕斗m

IT logical expressionI
statementi

小

小

이seif lo으ical exores, 幻n2
m

二

statement2
이se

多

statement3
end

好

'lo曾cal expression1' 조건이 '참’이면 'statementi'을 실행한다. 하지만 'lo얹cal expressioni' 조건이
'거짓'이면 이se正문의 'logical expression2' 조건을 살펴보고, 'logical express幻n2' 조건이 '참'이면
'statement2'를실행한다. 만약elseif문의 ' logical express幻n2' 조건마저 '거짓'이면 'statement3'을 실
행한 후 end 명령에 밖으로 빠져나간다.
1 예제 5- 3 I

M-FiIe I Grade f.m

시험 점수를 나타내는 변수 工의 범위는 0< 工 S 1000뼈, 입력하는 변수의 값에 따라 다음과 같이 A, B, C. D,
F로 성적이 구분된다．
A: 工 之 90. B: 80 5 工 5 89. C: 70 5 工 드 79
D: 60 5 工 5 69. F: 工 < 60
스크립트 파일 'Grade_If.m'에 조건문을 작성하고, 工＝90, 工＝68, 工＝37을 입력한 결과를 확인하라. 이따1

input 명령어를 이용하여 시험 점수를 입력받아라．

CHAPTER 05. 흐롬을 바꾸는프로그래밍

99

］23456

臼刈日f.m 旨： i + !
X = 1nput ( 'Enter the grade (I - 1凹) : ); 0

나

小

풀이

1

it a >= 90 e

囹

小
4
1

n
/

grade 믄 A
이 sel f x >= E刃
grade 三 B
elneit a >= 70
grade 三 'C.
elseif a >=60
grade = Jy
else
grade ! F
end
小

8

1

0
U

4

1

m

／
n

1

느

]11

1

0

그림 于3 조건문을 이용한 코딩 결과（GmdeJ.rn)

0 input 명령어를 이용하여 원하는문자열을 명령 창에 나타낸 후 값을 입력받아工에 지정한다．
Oif문을 사용하여 점수 구분에 따라문자열을grade어4 지정한다. 점수가 입력되면 '90점 이상，80점 이상，
70점 이상, 60점 이상, 그 외' 조건과 차례로 비교하여, 그 조건이 '참'일 때 grade에 해당문자열이 지정
되고 명령 창에 문자열이 나타난다．
口II> 각 조건문 앞의 들여쓰기는 코드를 이해하3I 쉽게 해준다. MATLAB에서는 기술적으로 이 공백을 무시하여 프로그
램을 실행하는 데 아무런 영향을 주지 않는다．
UI>

일반적으로 스크립트 파일을 생성한 후 빨간색 밑줄 물결 기호는 오류 알림을 나타내므로 MATLAB에서 제시하는
올바른 문징으로 바꿔야 힌다. 그러나［그림 于3］에 나타난 물결 기호는 실제 코딩을 실행하여 정확한 결과를 얻
는 데 아무런 영향을 미치지 않기 때뭔）II 무시해도 된다．

Con까rnand Win曲｝加
>> GradeJt
Enter the grade (1 - 100) ;90
grade =
4
>> ［打ade_I t
Enter the grade (1 - 1IJO) ;68
grade =
D
>> Grade_It
Enter the grade (I - 1a:)) ;37
grade =
F
그림 于4 조건문을 이용한 실행 결과

100

PART 02. MAT녀B 핵심 기능 익히7)

LESSON

04

순환문 사용하기

순차적 알고리즘의 흐룸을 제어하는 幻r문，小씨le문에 대하1 알아보자．

Keyi사ord

I

1 幻r문 ! while문 1

化r문

for문은 차례대로 입력되는 자료어］대해 같은 명령어로 적용할 때, 각각의 자료어］같은 명령어를 반복하
여 사용하는 대신 명령어를 하나로 고정하고 입력 자료를 반복하여 명령어를 실행하는 제어문이다．
for문의 기본 형태는 다음과 같다．
for loop variable = m : q : n
statements
end

『「

輛

澍

for 명령에 다음에 놓이는 변수는 반복어］필요한 변수라는 의미에서 순환변수(loop variable）라고 한다．
m은 초깃값, q는 일정하게 증가하는 값, n은 최종값을 나타낸다. 순환문도 조건문과 마찬가지로 end 명
령어를 사용하여 종료한다．
순환변수에 초깃값 m을 지정하여 'statements'를 실행한 후 end 명령어로 벗어나서 결과를 출력한
다. 그리고 다시 for 명령어로 돌아가서 초깃값보다 q만큼 증가한 m+q를 순환변수어］지정하여 동일한
'statements'를 실행한 후 end 명령어를 벗어나서 결과를 출력한다. 순환변수의 값이 최종값 n이 될 때
까지 이 과정을 반복하여 계속 실행한다．

CHAPTER 05. 흐름올 바꾸는프로그래밍

101

M-File ! trig.m

1 예제 5- 4 I
L山山-

J

幻r문을 사용하여 0八／360' 범위의 사인 함수와 코사인 함수 그래프를 그리는 스크립트 파일 'trig.m'을 작성
하라. 그래프를 그리는 데 필요한 MAT나＼B 명령어他tie, axis, 酬d, 야아t 등）를 사용하라．

.jtrigm
나．+{
11m
i=
3-

l u)

-

,

二

;:

，「 "叱" "

' "

7

plotty) ;
acis([ 0 咀

-

hold;

8

-

0d

ID-

0

;

1
[：
=j.

a

2*

t=

1J;
C; 1r
j1
iJfor,.
pi/ 180: pi
O:

2-

-slflu)

풀이

'

-1 1] );

p比t (z . ' : ') ;
axis( [[) 知 -1 1 ] ) ;

11 尸
12 -

xlabel ( 'Degree ") ;

1314-

ylabel ( "Magnitude' );
title ( 'Sine and Cosine Function' );

15 -

grid;

16-

gtext ( 'sin(t) ') ;
gtext ( 'cos(t) ');

1? -

그림 5巧 for문을 이용한 코딩 결과（trig.m)

0 for문의 순차적 흐름을 실행하는 색인으로 i를 지정한다．
0 for문을 처음 실행할 때 江 1, t= 0이다. 戶 1은 삼칵함수 그래프의 첫 번째 위치를 나타내고, t= 0은 삼
각함수의 인자값으로 사용되어 工축의 첫 번째 각도인 0을 표시한다. for문이 다시 실행되면 i= 2가 되어
두 번째 위치를 나타내고, t=pi/ 1的는工축의 두 번째 각도를 표시한다. 이러한 방법으로 t가 for문의
최종값27r가 될 때까지 순환문을 반복하여 실행한다．
Fl陌

Edit

Vi叫V

픈J 凸 d 小

自

Insert

10心

蜘p

win出그川

' ,, \ 舒 自 瓊 尻 ' 目

出

4目p

口 듣크 . 口

Sm. and Coi四Fu,妃IXtn
o.e
D
m
0
4
0
0
0
n
/
n
t
n
山乙二블4g>
4
O
部
批
反）

100

150

끄10

Degree

그림 千6 幻r문을 이용한 실행 결과

102

PART 02. MATLAB 핵심 기능 익히기

250

300

350

I 出h扼문
while문은 논리적 수식에서 제시한 조건이 만족될 때까지 해당 구문을 반복한다. while문의 기본 형태는
다음과같다．
while logical expression
statements
end

M-File I Exam while.m

I 예제15-5 I

학생 ] 0명의 MATLAB 중간고叭r 점수 분포가 다음과 같을 때, 小씨le문과 if踞 사용하여 평균보다 높은 점
수를 받은 학생 수를 구하는 스크립트 파일 'Exam1while.m'을 작성하라. 학생 수를 명령 창에 나타내;71 위
해 미S이ay 함수를 人용하라．
scores =[77

E泌am 놔州陌J1}
1

풀이

66

72

75

90

86

58

98

89

59]

+

n
r

scores = [77
count = 0;

5日 72

75

90 06 田 田 的 田｝;

Q
U
4

n = 0;

二
U

日뿌hu e n < Iength(score的 <1

n
b
n
r

1

口
U

10 -

U

n
U

count = count + 1 ;

end

U

it scores(n) > mean(scores) e

尸

0 = fl + 1 ;

-end

11-

비splay (score引 0
di＄口I ay(n)

12 -

display (count)

그림 5-7 w州e문을 이용한 코딩 결과（EXa吐whfle.m)

0 배열 scores에 length 명령어를 이용하면 1고｝ 10 중어］서 최때1 수인 10이 출력된다 ．이때 while문은
n< 10의 조건을 만족하는동안 반복하여 실행한다．
0 배열 scores의 각 원소가 毗an 함수를 사용하여 구한 평균보다 클 때는 count 값을 1씩 증가시키지만，
배열 scores의 각 원소가 평균보다 작을 때는 if문을 종료하고 다시 \vhile문을 반복하여 실행한다．
0 display 함수를 이용하여 10명의 점수（scores), 전체 학생 수（기, 평균보다 높은 점수를 받은 학생 수
(count)를 명령 창어］ 나타낸다. 이때In 값은 9까지 증가하지만 이후 刃 =n+1에 의해1 10을 출력한다．
if문에서 scores 값이 평균보다 큰 경우만 '참'이므로 count 값은 0에서 시작하여 4를 더한 4가 최종값
으로출력된다．

CHAPTER 05. 흐름을 뱌꾸는 프로그래밍

103

乙｝mmand V朴ndow

（今

>> Exom_whi le
scores =
77

n

8日

72

75

9［그

日日

5日

98

59

=

10

count =
4
그림 도8 while문을 이용한 실행 결과

El11 mean 함수를 이용하여 배열 A의 평균을 구하려면 mean(A）를 입력한다．

104

PART 02. MAT녀B핵심 기능 익히71

59

LESSON

05

사용자정의함수 작성하기

사용자의 필요에 따라 직접 함수를 만들어 사용하는 사용자정의함수에 대해 알아보자．
Keyword

I

! 사용자정의함수 I funct山n } 출력변수 1 입력변수 1

사용자정의함수

八4ATLAB에서 제공하는 내장함수는 공학이나 과학어써 자주 사용되는 수식에 대해 최초 개발자인 엔지
니어가 정의하여 만든 함수이다. 그러나 연구 분야가 다양하고 연구자마다 원하는 기능이 저마다 다르기
때문어］ 모든 기능을 내장함수로 제공하지는 못한다. 이러한 경우 소프트웨어 엔지니어가 내장함수를 개
발하는 것처럼 연구자 개인이 필요한 함수를 직접 만들어 사용하기도 하는뎨, 이렇게 작성된 스크립트 파
일을MATLAB에서 제공하는 내장함수와구별하여 사용자정의함수라고 부른다．
入4ATh&B을 사용하는 전 세계 많은 태학의 연구실에서는 좀 더 편하고 일반화된 연구를 위해 스스로 적
합한 사용자정의함수를 작성하여 사용하고 있다. 이렇게 만든 사용자정의함수는 유사한 연구를 진행하는
다른 연구실과 공유하기도 한다. 이처럼 사용자정의함수의 사용 범위가 확대되면 내장함수의 역할을 충
분히 수행할수 있다．

I

사용자정의함수 작성하기

사용자정의함수의 형태는 다음과 같다．
function [output variables] = name (input variables)
이를 구성하는 요소의 의미와 작성 규칙을 살펴보자．
0 사용자정의함수는 반드시 스크립트 M尸파일로 작성해야 한다．
日 구문은반드시 '凡nction'으로 시작하고, 첫 철자 'f '는물론이고모든 철자를소문자로작성한다．
日 'output variables'어］는 사용자가 현재 작성하는 수식에서 지정된 출력변수와 동일한 변수 이름을 사
용한다. 출력변수가 여러 깨일 때는 반드시 중괄호를 사용하고, 출력변수가 하나라면 중괄호를 사용
하지 않아도 된다．
0 출력변수다음에는등호를사용한다．
日 'name'어］는스크립트파일과같은이름을사용한다. 확장자（.m）는생략하고파일명만쓴다．

CHAPTER 05. 흐룝을 바꾸는 프로그래밍

105

日 'it叩Ut variables'어］는 입력변수의 이름을넣는다. 입력변수는반드시 소괄호안어］작성해야한다．
日 출력변수나입력변수가하나이상일 때는각변수를콤마（,）로구분한다．
0 명령줄끝어］세미콜론을사용해도상관없다．
日 앞의 0- 日 과정을 거쳐 작성된 사용자정의함수 'name.m' 을 저장한다．
四 작성된 사용자정의함수 첫 번째 행의 ' function' 부분을 제외한 나머지 [output variables] = name
(input variables）를 MATLAB 명령 칭어］직접 입력한다. 이때 input variables어］는 입력변수 대신
어］ 실제 사용자정의함수로 작성된 수식에서 계산하려는 입력 상숫값을 지정한다．
口 위의 m을 실행하면 입력 상숫값으로 계산된 수식의 출력값이 즉시 入4ATLAB 명령 창에 나타난다．

M-FiJe ! Eva! area.m

1 예제5-6

［그림 5-9］에서 보듯이 같은 크7떽 원 2개가 직사각형 안에 딱 맞7카 놓여 있다 ．가로 길이가 꺼／，세로 길이
가 ／인 직사각형에서 반지름이 r인 원 2개를 뺀 나머지 부분의 면적 area를 구하는 사용자정의함수 'Eva匕
aream'을 작성하고, 반지름 r= 3을 입력하여 출력값 area를 확인하라. 입력변수는 원의 반지름인 r이고, 출
력변수는 area이다．
w

\
N人，1

/

y

그림 도9 사용자정의함수의 도형

EvaLarea.m

풀이

蕉

+

무tunct ion (area! = Eval_area(r)

2. 四rc I e＝帥r2);e
1 미r2Area=2 미rcle "
1 2r;
1!
I=

=4

트-

I陀Ct＝

브e

!-

3-

'

따

7-

'r

'"

口
'i;

1

tj

4

! area=Hect-Ui rZArea; e
end

그림 5-10 사용자정의함수 코딩 결과乍va匕area.m)

0 입력변수가r, 출력변수가area인 사용자정의함수를 정의한다．
0 변수 Circle어］원의 면적을 계산하는 식 刃2을 지정한다．
0 변수 Rect어］직사각형의 면적을 계산하는 식 wx／을 지정한다．
0 출력변수 area어］구하고자 하는 면적을 계산하는 식 Rect寸Cir2Area를 지정한다．

106

PART02. M月ILAB 핵심 기능 익히기

Command Window
>> area=Eval ..area(3)
area =
15 』45田
그림 5-11 사용자정의함수 실행 결과

M-File I field.m

1 예제 5- 7 I

직사각형의 너비 w와 직사각형 내부의 면적 크가 입력변수이고, L과 P가 출력변수인 사용자정의함수 ' fi이d.

m

Jfield.

풀이

1
2 -

:d: i

i

，三 function [L,P] = f i이d（屯
L=(A-l. 八2/8) .／吼

34-

P

=

2L＋

？쯔

-

\／三

/8

刃＋

2

w
刃

-

A

L=

m'을 작성하라. 또한 너비 W= 6. 면적 A =80을 입력하여 출력값 乙고나를 확인하라．

)

P=2士L.W+2女W/sqrt (2) ;
-end

그림 5-12 사용자정의함수 코딩 결과（field.m)

입력변수가 万, A이고 출력변수가乙, P인 사용자정의함수를 정의한다．
Command Window

（自

>> [L. 미＝f i e Id(6. 日0)
L =
1 2. 5833

P =

그림 5-13 사용자정의함수 실행 결과

CHAPTER 05 흐름을 비꾸는프로그래밍

107

S＝미mmmm月s-s_ S口＝1=1= =mm球晦心鈿鈿mm口＝1=1mm!

I. ..쪄5. 쩍a.目느U-.'口mama崗耘嬅蜀啼쩍UI'S＝唯因寸1
n11mmmm目a.月U口口--S기'- S口U川刈玄쩍口S口a.唯蜘碎1
p口1mn目am. 月a.'. 口S口U口口＝a '呻唯羅a...까a鈿熬羅！
U- -a- ..-口口＝
口＝口S口口＝U芬a口-a甘難嫡難！
-a'a＝끼如社a出a끼a'心-a口U＝口＝-a. 杯哺蜂朗m毖a愍母啣斟雉三
i= U5m口텍U茗a骨mm日a-口月1mm胃聲補蘿肄幽川a.曲a斟嚮磁！
口m=1m mmam川a'. 口S.口口-a- 냅出熙坤困口a.喀m麟賤建！
11111mmmmmm芦m＝川a--口口口-u月U難U月a'＝目月塑齬羅！

p口口-a- US明出S日＝m111mm二mm巾까U哺.5_ S由a磁難礫i
U亡U口口느닌느닌U냅느出EU.口S느U,口i川心拙姑님岫mm曲出姓磁的！

'a- a戶＝*二끼禹m쿠'a. .기m1=1=mmm稗祿斗作耳甘用犀再解嬅i
i1= =H口dmH蚣哨I口U니S.니口ESU也堪납峀哺加甘由A出닙幽椰蜘！

I기口111a11am二aaaaUaa口口a口뗘a心渾湃mmmm杯熙薛鼎三
口aauiuuauaaaa口a-a-a-口a口二玄a夙a-月口뗘a礪堪熙！
'a口口aaa月a-目a끼＝口1111＝月a月月a月好a끼a日田固翌好嘴三
口二aaaaa目a心四口aaaau口口-a口a月甘aaa月目區a月恥名a
1a口a口aaa月口a月口aaua기'a. 口口目匹多因aaaaaa弦立叫！
I口미1a1aaaa目aaaaaaa1口a口aa目目甘a口口a日aa心姓i
U口a기1aaaaaaaaaaaaa기1a口a.月a.月aa口aaaa蜀
口aaa1口Ru...月aaaaauaaaaa피a目小aa口a口a月名出1
口N.기口1aaa1口aa口a....口aaa田딤多月日aaaaa三匹嘴i
U口aaaa끼口a111a口aaa1a11口1口a月aa口口nm口a出堪

11m口口口口amuamu...aa口口U'- .拉뗘mm口口口IS口曲出
口u-rn崩碎三
U'S. 口口口a口mnmm1m11口S口끼-'U. ,四am＝
口＝S口＝口口---S口a. .口口＝a口a月U斗m1ma.기目牡磁
口Na..日텍끼日喀麟a出1口a1口口11口Hmm必好mm쩍'U月U萍蠶

1111m口斗as耘啼aa.aa.u.口＝U- .牡烈mmmmmmm批耀

出出出出蹄州旨斗a.
.U.
.出aa出뿌斟出韶出客斟

U口S口川뼈1m11m1mmm1口'a. 口＝mm4m打a口月口U＝口U.
1a. .口U＝目川川在15口-S口＝5- -二月U如姓am끼1==mmm
U口'u1- U'S出U- -口11口月＝a州川뼈a.＝四口a口a.田

1==1=mm1mmmm끼sa.a. aam'a明目牡聯社aarn＝口目a同

口S＝
口口usa,.目4m＝
口＝S口＝
＝月叫＝崗崗在牡毋口mmSUU匕枉

I口S口U..'川벼弗心am口＝口a1aaaamm타a,口mm1111在
1- -＝月'S. 心胃U四m4d口口口S...心自珌朔mmm1mmmn4
I口＝口mmmmm出曲田'U. S.口S口U,同羽同啄毋川川口S＝니mm匹
口月U＝口a口心a胃翊的目am口S.-口U曲U聲料哺聲牡a'固a."如
U口U_U. .'. .拉- U.月끼口口＝口a姓U辯餌韶mmm1m二mm唯

Ia_ a. 口a川U蜂蚣必川mm口S＝口口U恥好U翔磁磁峀'U쳐口川U口出
口U口＝目U在a出砬U肺用-S口US口＝-U쩍U好胃町ma-＝끼ma.崗
U口U口SR브口心弗聲拉曲U口口기aSSaa
'心明准羽的心＝二口＝a口U
I口月U-a
'旺U. 奴U常a.口-S. 口口U麟在恥胃轟姐a心二a
'S.
唯
U.
U口＝ ...川鳳ma却口a口口口口"a唾U心崗磁蜘'a口a. '. 好
口mu目a目U.心拉凞奴U'- .-口＝
口U.社埠枉拉國胃S**UU乍a臂

出벼出出쀼拙뿌出S-a
- a--出州蛇朴出IAa.田出

la- -a月a--a- -a目月a--a口川I-.月---a- -a二月a-

姓心브甘立甘-Auau立立立立甘a----.뽀뽀

i

==
十
t r「 j 『

二

t

}

'

그

1

}

『

r

寸4

「

1
1

!

;

1-

!

L

「

j !

1

i

!

r小｝

卜寸-

小

卜

CHAPTER

06

1

니mH

+

1
卜

小｛

i
m

小

小工

수식 계산이 편한
심벌릭 툴박스
i
如
叫

m
口
m
1
打
；L！뇨i=i二i十1

!:1

卜 卜
叫r

++

11丁111寸

!!11｝ 才141! !

1

CONTENTS
LESSON 0] 심벌릭 툴박스 사용하기
LESS아나 02 수식 표현하71
LESS아1 03 조판 형태로 출력하기
LESSON 04 심벌릭 그래프 그리71

L

LESSON 05 대수방정식과 초월방정식 계산하'I
LESSON 06 심벌릭 미적분함수 사용하기

H+

1

叫中

LESSON 09 행렬의 특성 다항식 계산하기

!

丁_

1

,

1
m나十

!

i I !

I斗山

!
나

LESSON 08 라플라스 변환하기

小4-

-4-

-

I-

1

＋

나

나

LESSON 07 상미분방정식 계산하기

니

:

1

'.

=

심벌릭 툴박스 사용하기
MATLAB에서 제공하는 심벌릭 툴박스를 사용하면 수학 계산을 편리하7카 할 수 있다. 심벌릭 툴박스에 대해 이해하고, 심벌릭
툴박스를 시작하는 데 이용하는 sym, syms 명령어를 살펴보자．
Keyword

I 심벌릭 툴박스 I sym I syms i

I 심범릭 툴박스
MATLAB은 다양한 공학 및 과학 분야어］ 매우 유용하게 사용되는 심벌릭 툴박스（Symbolic 八4ath
Too小ox）를 제공한다. 심벌릭 툴박스를 이용하면 수식을 복잡하게 계산하지 않고 문자를 사용하여 수식
을 계산하거나, 수식을 간단하게 만들어 계산하므로 매우 편리하다．
심벌릭 툴박스는 미분, 정적분 및 부정적분, 한계 계산, 테일러 급수생성, 라플라스 변환, 푸리에 변환등
미적분 계산어］도움이 되며, 특성 방정식, 고윳값, 고유 벡터를구하는 선형대수에도폭넓게 쓰인다. 또한
대수방정식과상미분방정식의 풀이에도 사용할수 있다．

I

sym, syms

심벌릭 툴박스를 시작하려면 주어진 수식에서 사용할 변수를 지정해야 한다. sym 명령어는 수식에서 사
용하는 변수를 17귀 지정할 때 이용하고, syms 명령어는 수식에서 사용하는 변수를 여러 개 지정할 때 이
용한다．
x = sym('x')
= X: 심벌릭 툴박스에서 사용할 변수를 지정할 변수
, 노n 심벌릭 툴박스에서 사용할 변수

口ii)

일반적으로 sym 명령어의 인자 'x'와 심벌릭 변수를 지정하는 변수 x는 같은 변수를 사용한다．

syms x y z
=x. y, z: 심벌릭 툴박스에서 사용할 변수

1i11 x = symCx'）의 실행 결과와 syrr冶 x의 실행 결과는 같다．

1 10

PART 02. MATLAB 핵심 기능 익히71

1 예저I 6- 1 I
심벌릭 툴박스를 이용하여 수식 万］ = （工

푿이

5)5을 입력하라．

C며girrand］邸indDw

>> El=(x15) '5 0

Error using 二 e

Inputs must be a scalar and a square matrix.
To Compute 이 ement밖 ice P0姃凡 use PC뿌ER ( . ) instead

>> syms y

>> 티＝(a中5) ' 5e
Error using 二 0

Inputs must be a scalar and a square matrix
To com口ate 이ementm泊e P0뿌E日. use PC뿌ER ( . ) instead
>> sy.s S

>> El=(x-5) '5 0
El =
(x 尸 5）石
>> 이 mar
>> syim x s'
>> 티＝
（小디石
El

=

(S - 5）石
그림 6너 심벌릭 툴박스를 이용한 수식 입력 실행 결과

Osym 명령어나 syms 명령어로 변수를 지정하지 않고 심벌릭 툴박스를 사용했으므로 오류 메시지 (O）가
나타난다．
0 syms 명령어로 지정한 변수와사용할 변수가 일치하지 않으므로 오류 메시지 (O）가 나타난다．
0 syms 명령어로 수식에서 사용할 변수工를 지정한 후 주어진 수식을 입력했으므로 오류 메시지가 나타나
지 않고 수식 입력 결과가 나타난다．
0 나중에 사용할 변수y를 미리 지정해도 상관없다．
口口｝ 심벌릭 툴박스에서 이미 지정한 명령어와 새롭게 지정한 명령에 사이에 충돌이 발생하는 것을 방지하기 위하I clear 명령어를 사용할
수 있다．

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

111

수식 표현하기
수식을 차수 순으로 전개하는 방법, 인수분해 형태로 나타내는 함수, 수식을 간단히 나타내거나 형태를 변환하는 함수를 살펴
보자. 또한 다항식과 다항식에 사용하는 계수 사이의 상호 변환에 사용하는 함수에 대하1 알아보자．

Keyword

I

I expand I factor I collect 1 simplify I subs 1 double I sym2口이y I poly2sym I

expand

수식을 멱승（power) 형태로 전개하고 그 결과를 내림차순으로 나타내는 expand 함수의 기본 형태는
다음과 같다．
expand(E)
· E: 멱승 형태로 전개할 수식

I factor
다항식을 인수분해 형태로 나타내는 factor 함수의 기본 형태는 다음과 같다．
factor(E)
· E: 인수분해 형태로 나타낼 다항식

1 여以II 6- 2 I

다음 문저를 풀라．
(a) 수식 E1 = （工

旬5을 멱승 형태로 전개하라．

(b) 수식 E2 = 工4+ 12工3+ 54工2 +108工 + 81을 소인수 형태로 나타내라．

112

PART02. MAT녀B 핵심 기능 익히기

岳이

0

>> syms H
>> 티＝（小引石；
>> E2=(4. 12.x3+54*s八2,I月. x*6l;
>> 肛aspand（테 0

A

=

S八5 - 25* x八4 中 25［그＋X八3 - 1250士S八2 + 引 25士）< m 3125
>> 5=factcr (E2) '

日

=

[ x * 3, X + 3, 5 + 3, 5 * 3]
그림 6-2 今四and, fac幻r 함수 실행 결과

(a) 먼저 syms 명령어로 수식 月구｝万2에서 사용할 변수工를 지정한다化1) .
(b) expand 함수를 이용하여 수식 局을 멱승 형태로 전개하고 내림차순으로 나타낸다（回．
(c) factor 함수를 이용하여 수식 尻를 소인수 형태로 나타낸다（O).

I c에ect
다항식을 전개한 결과를특정 변수에 대한 내림차순으로나타내는Co끄ect 함수의 기본 형태는다음과같다．
coUect(P,var)
· p: 다항식
·var: 항의 나열 기준이 되는 변수

1 예저I A- q I
다음 문제를 풀라．
(a) 수식 /1=（工 + 1)(x+ 2)（工 + 3）을 변수 工에 대한 내림차순으로 나타내라．
(b) 수식 .[2 = 口2b ＋口b H 口2 寸 2口를 변수 口와 b에 대한 내림차순으로 나타내라．

CHAPTER 06. 수식 계산이 편한 심벌릭 튤박스

113

>> syms a

<1

今

>> f 1=(x+1)*(x '2).(x.3) ;

>> C1=coI IectU1) e
Cl =

'C八3 + f弘r2 + ll* x + 6
그립 今3 (a）의 실행 결과

Os戶ns 명령어로수식 五 에서 사용할변수工를 지정한다．

(b)

Oc아lect 함수를 이용하여 수식 玉을 변수工어］대한 내림차순으로 전개한다．

C口mm訊d Wir,clcw

>> syms a b 0

>> 12=a八小b.a比寸a八2-2*a;
>> c2丸ol lect (12,a) 0
C2 =
(b - 1)姐竺 + lb 尸 2）士a
>> C3=col lect (12,b) O
C3 =
(a2 * a）比 小 a2 - 2*a
그립 中4 (b）의 실행 결과

0 syms 명령어로수식 石에서 사용할 변수口，b를 지정한다．
0 collect 함수를 이용하여 수식 万를 변수口에 대한 내림차순으로 전개한다．
Oc이lect 함수를 이용하여 수식 石를 변수b어］대한내림차순으로 전개한다．

I

simr川fy

복잡한 형태의 수식을 좀 더 간단하게 나타내는 sin巾ii匈 함수의 기본 형태는 다음과같다．
simpify(E)
, E: 긴략하게 나타낼 수식
轟蠱難無蛾礁難軸罐轟轟麟酢瀉轟蜘哺照黨難瑟埠鹹轟聲耕名磁轟鞠坦3每建瑟懈堪彗料

114

PART 02. MATLAB 핵심 기능 익히71

I subs
현재 심벌릭 수식에서 사용하는 심벌릭 변수를 다른 심벌릭 변수또는 숫자로 대치하는 subs 함수의 기본
형태는다음과같다．
subs(E,x,a)
· E: 심벌릭 수스1
· X: 대치할 심벌릭 변수
· a: 새로운 심벌릭 변수 또는 숫자

예를 들어 전자기학에서 함수의 곡선을 따라 이동하며 적분하는 선 적분을 꼐산할 때 subs 함수를 이용
하는데, 선 적분에서는특정 경로를 계산하기 위해 심벌릭 변수를숫자로 대치한다. 다음은 11장의 ［예제
11小9］에서 다루는Linelnt.m의 일부이다．
syms x y z
A= [2永x水y永z.x小2水z.x勻永y] ;
maxy=0;
mmn z=o;
Path1=subs (A (1), ]y,z}, {max_y,min_z});

I doub旭
주어진 수工를 소수점을 포함한수치 형태로 변환하는 double 함수의 기본 형태는 다음과 같다，
dou이이지
· X: 소수점을 포함한 수치 형태로 변환할 수

1 예제 아4 1
수식 E1 = 工4+ 12工3 +54工2+108工 + 81, 万2 =（工 - 3)2 +12工일 때 다음 문제를 풀라．
(a) 수식目을 E2로 나눈 결과를 간략하게 나타내라．
(b) 工 = 2.5일 때 수식 目 과 万2를 더한 결과를 심벌릭형으로 변환하라．
（이 工 = 2.5일 때 수식 目 과 E2를 더한 결과를 수치형으로 변환하라．

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

115

Commend Windc=v
)> syms x
>> 티 =x八4+12出r3巧4古x八2.1(月卉）什81 ;
" E2=(s-3)六2+12*x;
>> 미＝E1/E2;
>> D2=sImpI I fy (D1)<1

쭐이

今

D2 =
(x + 3Y2
>> S1十1.E2;

Q

,

.

-

>> S2=sym(subs(SI, x, 2.5) ) V
S2 =
1 듸 25／比
>> 53=double (52) 0
S3 =
9453125

그림 于5 simp和, subs, doubb 함수 실행 결과

(a) 計mph勺 함수를 이용하여目을月2로 나눈 결과를간략하게 나타내고 그 결과를D2어］지정한다佃目．
(b) 同과月2를 더한 결과를 & 어］ 지정한다（回. subs 함수를 이용하여 ＆에서 사용 중인 심벌릭 변수工에
상수2.5를 지정하고, 5恥n 명령어를사용하여 易를 심벌릭 상수로 지정한다（0).
(c)double 함수를 이용하여 수식 曷를소수점을포함한 정밀한수치로 나타낸다（0).

I

sym2p이y

심벌릭 다항식의 계수를 행 벡터로 변환하여 내림차순으로 나타내는 sym2p이y 함수의 기본 형태는 다음
과 같다．
sym2poly(P)
, P: 행 벡터로 변환할 심벌릭 다항식의 계수

1 P이y2sym
다항식의 계수 행 벡터를 심벌릭 다항식으로 변환하는 poly2sym 함수의 기본 형태는 다음과 같다．
p이y2sym化'v')
· r: 다항식 계수 행 벡터
· V': 변환할 심벌릭 다항식의 변수명

116

PART02. M시LAB핵심 기능익히71

1 예제 6巧 1
함수 므과 只가 다음과 같을 때나）= 尸I + P2의 계수를 행 벡터로 나타내라．
/i =5尸+ 2x2小3. 1}卜2工3m工2 + 4x +6
풀이

侄）

Conimarid Wfridow

0

>) syms K
>> F기＝5士）（八4+2*a八2-3;
>> P2-2ei(3-x八2+4古a+6;
>> P=P1+P2; 0
>> syrn印山（P) 0
ails =
5

-2

1

4

3

그림 6田 Sym2q加 함수 실행 결과

0 syms 명령어로 변수工를 지정한다．
op의 결과를 구한다．
Osym印이y 함수를 이용하여 尸의 계수를 내림차순으로 나타낸다．

1 예제 6- 6 I
다항식의 계수 벡터 r =［그 0351 尸4］일 때 이에 해당하는 심벌릭 다항식을 짖K）봐, 변수는y룔 사용하라．

푿이

Commarai Wiild:I

0

>> syms y
>> r=1-2 0 3 5 1 -41;
>> po1y2sym(r,y) 0
ans =
-2四石 + 3*y四 + S씩竺 + y m 4
>> r1=1-2 35 1 -41;
>> poly2syi(rl, y) 0
ans =
m 小／4 + 3四四 + 5士y坦 + y -4
그림 6寸 口dy2syrr) 함수 실행 결과

0 syms 명령어를 이용하여 변수y를 지정한다．
0 poly2sym 함수를 이용하여 행 벡터 r을’변수 y를 포함한심벌릭 다항식으로 변환한다．
Op아y2s刃n 함수를 이용하여 행 벡터 rl을 변수）를포함한심벌릭 다항식으로 변환한다. 이때 생략된 차수
항도반드시 0드로지정해야하며, 만약지정하지 않으면 가장높은챠수가5차가아닌 4차로 변환된다．

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

117

LESSON

조판 형태로 출력하기

03

수식의 가독성을 높이기 위하1 사용하는 조판 형태의 출력 방법을 살펴보자．
Keyword

1 pretty

立 口retty
대부분의 MATLAB 출력 결과는 가로줄 쓰기 형태이지만 가독성을 높이기 위하1 조판 형태로 출력할 수도
있다. 수식을 조판 형태로 출력하는 pretty 함수의 기본 형태는 다음과 같다．
pre姓y（타
. E: 조판 형태로 출력할 수식

I （비저I 6 -7 I
i=：二二＝-J

함수 /i , 石가 다음과 같을 때, 玉을 万로 나눈 결과를 pretty 함수를 이용하여 함수 万으로 나타내라．
五 ＝工64 1, ／三 =x3 +1
풀이

Command \山n口m\
>> syms H <1
>> Ii =x汪；니 ;
>> 12=x八3.1;

>> 13=11/12 e
13 =
(x下

1)/tx四 + 1 )

>> pretty (13) 0
S
-

x

1

3
x

* 1

그림 6田 petty 함수 실행 결과

Os恥ns 명령어로 변수工를 지정한다．
Of；
을 구한다．
0 pretty 함수를 이용하여 月을 조판 형태로 나타낸다．

118

PART02. MAT냐＼B 핵심 기능 익히71

侄）

LESSON

04

심벌릭 그래프 그리기

하나의 변수로 표현된 심벌릭 수식의 그래프를 쉽게 그릴 수 있는 ez히아 함수의 사용법을 살펴보자．

! ez히야 1

Keyword

I

ezplot

하나의 변수로 표현된 심벌릭 수식의 그래프를그리는 ezplot 함수의 기본 형태는 다음과같다．
ezplot(E, [xmin xmaxj)
· E: 그래프로 나타낼 심벌릭 수식
. 지ilin: 사용하는 변수의 최소 범위
·xmax: 사용하는 변수의 최대 범위

변수의 범위를 지정하지 않으면 범위는 기본인 [-2兀, 2川로 지정된다. 또한 title. xlabel 명령어를 사용
하지 않아도 자동으로 제목과工축의 히름이 표시된다．
1 예玉II 6- 8 I
-3 < 工 <5일 때 심벌릭 수식 E = 工2 -2工 +5의 그래프를 그려라．

풀이

Command ＼사1nd口싸
>> syms K

<1

>> E=sy.( ' xA2-2*x+5' );

>>ezpIot(E.I-3 51) 0
>> ylabel (1E) 0

그림 6四 e긱켜아 함수를 이용한 코딩 결과

0 syms 명령어로 변수工를 지정한 후, sym 명령어
의 괄호 안에 주어진 수식을 직접 입력한다．

F朴口 的t

Wm 出Ill TO& ［片166叩1 mmtw

D 볍니 企

1t

曳 \

好自 咽 /

L 晶

64出1
t} g立 1 口

X2 -2 X + 5

0 ezplot 함수를 이용하여 工 의 범위어］따른 심벌릭
수식 万의 그래프를 그린다．

1666

oy축의 이름은 자동으로 지정되지 않기 때문에
ylabel 명령어를 이용하여 y축의 이름을 표시한
다. 이때 제목과 工축의 이름은 자동으로 지정
된다．

64 H
11j

8
6

4

-2

3

4

5

그림 6-10 ez口kt 함수듬 이용한 실행 결과

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

119

LESSON

05

대수방정식과 초월방정식 계샨하기

심벌릭 툴박스를 이용하여 대수방정식과 하나 이상의 초월함수를 포함하는 초월방정식의 해를 구하는 방법을 살펴보짜．
I solve 1 구조 배열 1

Keyword

I ＄이ye
심벌릭 방정식의 해를 구하는 solve 함수의 기본 형태는 다음과 같다．

so如e 함수를 사용할 때는 syms 명령어로 변수를 지정할 필요가 없다. 하지만 변수를 지정한 후 사용해
도상관없다．

2

풀이

Ccrrm帥a 났1n

-

-

2

x+

고차방정식曷＝

!3『1! 2
x +-x

5

1 예저I 6- 9 I
1의해룔구하라·

<1

>> syms x
>> 티＝S八3벼坦尼巧쌔尼+1 ;

>> 얽＝$이呵El) 0

-2

SI =

1/2
1
>> 32=so1ve(s' 乎x'2/2-S中x/2너 ) 0

-2

S2 =

1/2
]
그림 6너］ solve 함수 실행 결과

120

PART 02. MAILAB 핵심 기능 익히71

0 syms 명령어를 이용하여 변수를 지정하고, 고차 방정식目을 지정한다．
Os아ye 함수를 이용하면 3차 방정식의 근 3개를 구할수 있다．
0 syms 명령어로 변수를 지정하지 않아도 5아ye 함수를 이용하여 고차 방정식目의 하를 구할수 있다．

I

구조 배염

구조배열（structure array）은구조（S汀ucture）로구성되어 있으며, 구조배열에는서로다른배열을함
꺼］ 저장할 수 있다. 구조 배열 S어］ 원소工, y가 저장되었을 때 S는x와y어］대한 상위 분야（field）이고，
工와y는 S어］ 대한 하위 분야이다. 이렇게 상위 분야와 연결된 하위 분야를 지정할 때는 점 (d야） 부호를
사용한다. 예를들어 구조 배열 S를사용하여 원소工와y를구하는 경우 각칵S.x와S.y로쓸수 있다．

1 예저16-101
L二二：H-mH-1=
- I
다음 ] 차 연립방정식을 만족하는 工, y의 값을 구하라．

伊月.
Command Window

x-

3*

2*

y ==9

,

>> S2. x 0

e)

.6*

>> syms
S2s。
>,
Ivey

(x.

풀이

y: =9) ;

0

ans =
27/5
>> S2. y
ann =
3/5
그림 6-12 구조 배열 실행 결과

0 syms 명령어를 이용하여 두 변수를 지정한다．
Os아ye 명령어를 이용하여 l차 연립방정식의 해를구하고 그 값을 S2어｝지정힌다．
0 구조 배열 S2.X-Q1- S二y를 이용하여 l차 연립방정식의 해 肛I-y의 값을구한다．

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

121

LESSON

06

심벌릭 미적분함수 사용하기

심벌릭 미적분함수 d咐, 1nt, tay幻r, un我, symsum의 사용법을 살펴보자．

Keyword

I

I duff ! mnt 1 taylor I limit 1 symsum I

diff

주어진 수식을 미분하는 di什 함수의 기본 헝태는 다음과 같다．
小州秋！n)
. fx: 함수
· n: 연속으로 실행하는 미분의 차수｛생략 시 n=1로 지정된다.)

예를 들어 전자기학에서는 직교좌표에서 벡터의 회전을 구할 때 diff 함수를 사용한다. 小ff 함수를 이용
하면 벡터의 각 성븐을 원하는 변수의 차수로 미분할 수 있다. 다음은 11장의 ［예제 11-14] 에서 다루는
CuriCar.m의 일부이다．
syms x y z
H= [y水z, 4幻卄y,y];
curlH=[diff(H(3),y)나diff (H (2),z) diff(H(l),z)-diff(H (3),x) diff(H (2),x)-diff(H (1),y) ];

1 여以II A- Il I
H- - I
1.=：二二．

함수 y = 工4
풀이

8X3+ 2工2_ 3의 2차 미분을 계산하고, 2차 미분이 0이 되는 부분을 찾아라．
3
>> syms x

<1

>> y=x人4-(8/3).,（八a卜2士xn2口3;
>' 02di11(y, 2) 0
02=
12.xA2 - 16.x + 4

>) soive (02) 0

루

1／

그림 6-13 d咐 함수 실행 결과

122

PA日T02. MAT녀B 핵심 기능익히기

0 syms 명령어를 이용하여 변수工를 지정한다．
Odi奸함수를 이용하여 2차 미분을 계산한다．
0 solve 함수를 이용하여 2차 미분이 0이 되는 점을 구한다．

I

mlt

연속 함수 /(x)가 미분 가능하면 함수 /（功의 모든 역도함수를 함수 /(x)의 工어］ 대한 부정적분
(indefinite integral）이라하고／/（工）威로나타낸다．정적분（definite integral）은일정한구간 [a,
b］어］서 연속함수／(!）에 대한적분으로／
:1(x) dx로나타내며，함수／(!）와：축／k］의 면적을의미
한다．
주어진 수식을 적분하는 mlt 함수의 기본 형태는 다음과 같다．
int(f(x), a, b)
· 肛）: 피적분함수
·a, b: 적분의 하한값과 상한값

1 예제 6- 12 I
부정적분 /cost:
）赤와정적분 ,
／' COs2(X）赤롤 계산하라．
풀이

Command Window
>> syms x
>> fcos(XY2;
>> Inf_ IntHnt (f) 0
Inf_Int =
x/2 + sin(2.x)/4
>> 院f_ Int=int (f, O,pi) 0
Det_Int =
미 /2
그림 6-14 nt 함수 실행 결과

0 mt 함수에 피적분함수 /(x）를 입력하여 부정적분을 계산한다．
0 mt 함수에 피적분함수 /(x), 하한값 0, 상한값pi를 입력하여 정적분을 계산한다．

CHAPTER 06 수식 계산이 편한 심벌릭 툴박스

123

I

taylor

테일러 급；=(Tay1or ser妃S）는 어떤 함수를 미분 가능한한 점의 값으로 계산되는 각항의 무한한합으로
나타내는 것으로, 미분 가능한 함수를 다항식의 형태로 근사시킨다. 이때 특정 조건을 만족하는 임의의
함수가 테일러 급수로 표현된 것을 테일러 정리라고 한다．
테일러 급수의 수식과주어진 함수의 테일러 급수를 계산하는tayl아 함수의 기본 형태는 다음과같다．
tay幻r(f, 'ExpansionPoint', a, 'Order', n)
.f: 테일러 급수를 적용할 함수

(a)

,'

""
客／

· n: 함수／에 의하1 정의되는 테일러 급수의 처음 n- I 항

(x-

a)

· a: 工 == 口에서 평가되는 값
· 'O川er之 테일러 급수의 항을 정의

"

매개변수口가생략되어 있다면 a= 0을 의미하고 이 경우 'ExpansionPoint' 부분도삭제한다．

1 예저［6中13 1
다음 문제를 풀라．
(a) 함수月 = sinx를 테일러 급수로 전개한 처음 네 항을 구하라．
(b) 함수／52 = ey
-e을 工 = 0인 점에서 테일러 급수로 전개한 처음 여섯 항을 구하라．

1口rnn텨크1)口 寸n
(a)

귤；i

斤＼

>> syflis H

>> fi＝引ri(n;
>> taylor(fl, Order ', 4) <1
ass =
- )r3/6 + a
>> Ti=t a小r(fi, 毗叱8) 0
Ti =
- x7/5040 + a5/120 - x八3/6 + X
그림 6-15 (a）의 실행 결과

0 taylor 함수를 이용하여 玉을 테일러 급수로 전개한 처음 네 항을 나타낸다. cos（兀／2) =0 인 항을
제외한2개 항이 출력된다．
0 taylor 함수를 이용하여 五을 테일러 급수로 전개한 처음 여덟 항을 나타낸다. cos（兀／2) = 0인 항을
제외한4개 항이 출력된다. 이때 계숭（factorial)은 7! =7x6x5x4x3x2x1 =5040이다．

124

PA日T02. MAT녀B핵심 기능익히기

(bJ

回

Command Win出N心
>> ssms
>> f2=eap (y) ;
>> 12=tayIor (t2 0rder ', 6 'a O) Q
12 =
y5/120 + yA4/24 + y3/6 * y2/2 * y * I
>, T3=tayIor (f2 ' 0rder' ,6)
T3 =
y5/ 120 + y八4/24 中 y八3/6 + V2/2 + y + 1
그림 6-16 (b）의 실행 결과

0 taylor 함수를 이용하여 方를 테일러 급수로 전개한 처음 여섯 항을 나타낸다. 매개변수口가 생략되
었다면口 = 0을 의미한다．

limit

I

변수가 어떤 값어］가까워짐어］따라 함숫값히 가까워지는 값을 극한값이라고 한다. 어떤 점에서 함수의 극
한을 구하기 위한 극한의 수식과血nit 함수의 기본 형태는 다음과 같다．
limit(f, x, a, 'direction')
· f: 주어진 함수
, X: 함수／에 지정된 변수

urn f (x)

· a: 변수 工가 접근하는 값
· 'direction' : 극한을 구하'I 위해 접근하는 방향(left ' 또는 'right'를 입력하거나 생략할 수 있음）

1 예工B E5-14 I
다음 극한값을 계산하라．
/

\ 1.

\a) ll m

2 1
n
J, 十 兀 叫 乙

3

工- I

兀

. . ..
lC) iirn-

Mnx2
-

工＋0

工d

,

＝尸 I

/ 1\

1.

2
1 /
工 e 1O

tU) 11111
工-.4+ 工1- 8工 + 16

CHAPTE日 06 수식 계산이 편한 심벌릭 툴박스

125

횰이

Comm크ad C.
>> syis a

分

0

>> Ll=I iiit ( (a'2*a-2) /(x '3-1L1) 0

Li =
1

>> L2=I i.it( (s너)/x, Inf) e
L2 =
1
그림 아17 (a), (b）의 실행 결과

(a) s戶ns 명령어를 이용하여 변수 工를 지정한 후（이, limit 함수를 이용하여 x= 1어］ 접근하는 극한값을
구한다（O).
(b) limit 함수를 이용하여 x = 的에 접근하는 극한값을 구한다（回．
Command＼뾔ado町
>> syis a

e

>> L3=I iiit (引n(x"2) /x'3,a,O, Ie1t ) O

-

L3 =
Inf

>> L4=I iiit ( (x'2-16)/(x'2-小x시6),s,4, 'rjght ') 0
L4 =
1ni

그림 6-18 (c). (d）의 실행 결과

(c) syms 명령어를 이용하여 변수工를 지정한 후（回, limit 함수를 이용하여 工 =0의 왼쪽（D 방향어써
접근할 때의 극한값을 구한다（0).
(d) limit 함수를 이용하여 x =4의 오른쪽（+) 방향에서 접근할 때의 극한값을 구한다（回．

蚤 symsum
급수란 어떤 수열의 시작 항부터 마지막 항까지의 합을 말한다. 급수를 구하는 수식과 주어진 급수를 구
하는symsum 함수의 기본 형태는 다음과 같다．
symsun咐(x)小同b)
· f（자：심벌릭 변수로 표현된 수식
. n: 심벌릭 변수
· a: 급수의 시작 값
. b: 급수의 마지막 값

126

PART02. M戶ILAB 핵심 기능 익히기

b

2f(x)

刃= a

1 예제 6- 15 !
다음 급수를 계산하라．

(a)夕．
二
'나' 烏．凡片
Command V바ndow

（兮

>> syms k n <1
>> A=symsum(l/k '4,k,Linf) 0
A=

풀이

口 尸4/90

>> 6=symsu日(n'2,n,O,7) 0
B =
1 40
그림 아｝9 symsum 함수 실행 결과

(a) syms명령어를이용하여변수凡刃을지정한후（이, symsum함수를이용하여급수의합을구한다（O).
(b) symsum 함수를 이용하여 급수의 합을구한다（回．

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

127

LESSON

07

상미분방정식 계산하기

심벌릭 툴박스를 이용하여 다양한 상미분방정식（하나의 방정식, 2개 이상의 방정식, 초71 조건이 지정된 방정식, 경계 조건이
지정된 방정식, 비선형방정식 등）을 계산하는 방법을 알아보자．
Keyword

I

I dsolve 1

ds이ye

상미분방정식을 계산하는 ds이ye 함수의 기본 형태는 다음과 같다．
d＄이陀作quation',y田）)
'equation': 상미분방정식의 심벌릭 식
. y(o): 초깃값

2개 이상의 상미분방정식을 계산하는 dsolve 함수의 기본 형태는 다음과 같다．
dsolve ('equationi', 'equation2', y (0) )
dsolve 함수를사용할 때는S아ye 함수와마찬가지로 syms 명령어로 미리 변수를 지정할 필요가 없다．
또한 독립변수의 이름과상관없이 심벌릭 툴박스의 미분변수는 항상 t를 사용한다．

또한독립변수
（어］
대한1차"］분을나타내는三는기호D로대치하고1차미분방정식多를MAll朋
증가시킨다·

128

2차미분방정식字는MATLAB코드D2

『로표시한다．
미분어］대한 초깃값을 포함하여 2개의 초깃값이 필요하다．

PART 02. MATLAB 핵심 기능 익히기

2차상미분방정식을푸는데1차

코드刀y로표시한다．같은방법으로미분차수가브三, 르인2차미분과3차미분은기호D2와D3으
dt乙 d尸
로 대치하여 사용하고, 계속해서 미분방정식의 챠수가 4차, 5차로 증가하면 I) 바로 옆의 숫자를 4, 5로

0St (b0일 때 다음 방정식의 해를 구하고 ez이야 함수를 이용하여 y(t)의 그래프를 그려라. 초깃값은 0이

라고 가정한다．

dv

2

-

J，느＋ . ,, . 八 y = 4
口I
IU 十 /I

풀이

Command 邪昨j（升V

（多

>> syms V t <1

>> ditteq='Ds,=_(2*y) /(10.2士t)*4' ;
>> y=d＄이呵dif伯q, 'y(0)=n e
y =

(2女t士（t + lofl/(t + 5)

,> ez小t (y, 010) e

>> axis(F0 10 0 凹J)
>> 이 ear
>> y=dsolye( 'Dy.-2.y/(10+2*t) =4' , ' y (O)=0) C

y =

(2.t*(t + 10))/(t + 5)
>> ezpIot (y, 0, 10) C
>> axis([0 10 0 301)
그림 小20 ］차 상미분방정식 코딩 결과

Osyms 명령어를 이용하여 변수 y, I를지정한다．
0 dsolve 함수를 이용하여 방정식의 하를 구한다．
Oe可,lot 함수를 이용하여 l차상미분방정식을 그래프로 나타낸다．
0 심벌릭 변수를 지정하지 않고 dsolve 함수를 이용하여 방정식의 해를 구한다．
0 ezplot 함수를 이용하여 l차상미분방정식을그래프로 나타낸다. 이때의 결과는O과같다．
Ale

田I

Slew

王rewt

To必

1：뇨如呻1 mM汁 卜1的P

!.) C} 너 由 ［뇽 i (‘뇨 ’禹느 幼 自 嗔 d 기 目

口 튿크

=

S口

(2 I (I + 1아玳I + 5)

0

2

3

4

5

6

9

10

그림 今21 ］차상미분방정식 실행 결과

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

129

1 예저16-17 1
2차 상미분방정식 )+13 '+ 40y =f (t）는 t< O일 때 只t) =O이고, t三0일 때 /(D =4이다. 초깃값이
y(O) =o, v(0) =0일 때1 방정식의 해를 구하고 그래프를 그려라. 이때 그래프의 범위는 0< / 드 0.9이다．

푤이

Command Windo ';
>> y=dsolve(陷너3*如4啣叱 'y(0)=0' 1 Dy(O)=0)
y =

exp(-B.t) /6 - （巾매p（石士t) )／侮 + 1/10

::：二벎'凉0.1]) <)
그림 伊22 2차 상미분방정식 코딩 결과

0 심벌릭 변수를 지정하지 않고 ds아ye 함수를 이용하여 2차상미분방정식의 해를 구한다．
0 ezplot 함수를 이용하여 2차상미분방정식을 그래프로 나타낸다. ezplot 함수의 인자는 정수만 가능하므
로 문제에서 제시한 범위를 표현할수 없다．
0 axis 명령어를 이용하여 문제에서 제시한t의 범위를 지정한다．

그림 于23 2차 상미분방정식 실행 결과

130

PART02. M사녀B 핵심 기능 익히기

LESSON

08

라플라스 변환하기

시간 영역에서 미분방정식을 푸는 것은 매우 복잡하'I 때문에 라플라스 영역으로 변환한 뒤 계산하면 쉽게 해결할 수 있다.
심
벌릭 툴박스를 사용하여 라플라스 변환 문제를 해결하는 방법을 살펴보자．
Keyword

I 라플라스 변환 1 冶히ace I 라퓰라스 역변환 1 陀히ace 1

laplace

I

변수 t를 사용하는 시간 영역의 함수를 변수 S를 사용하는 라플라스 영역으로 변환하는 것을 라플라스 변
환이라고 한다. 이를수행하는laplace 함수의 기본 형태는 다음과 같다．
IapIace(f)
· f: 시간 영역의 함수

ilaplace

I

변수S를 사용하는 라플라스 영역의 함수를 시간 영역의 함수로 변환하는 것을 라플라스 역변환이라고 한
다. 이를수행하는ilaplace 함수의 기본 형태는다음과같다，
ilapIace(f)
· f: 라플라스 영역의 함수

1 예제 6- 18 I
다음 함수의 라플라스 변환을 수행한 후 다시 역변환을 수행하여 주어진 함수와 비교하라．
뜨

竺

l

(a)

e

e

e
5

6

而

(b) -2cos2t + 3sin2t

CHAPTER 06. 수식 계산이 편한심벌릭 툴박스

131

色）

4*

(-

>> L
IapIace l타exp(t)/5. 25.exp (2.t)/타exp
t
>> nyms,

(-

Command Wn七
t)/凹)

0

LI =
巧/(6.(s -2) ) - 16/(5.(s 尸 1) ) + 1/(可k (s + 4) )
>> IL1=iIapIace(L1) 0
ILl =
(巧士exp(2卄) )/6 + exp(-4+t)/30 - (16'exp(t))/S
그림 6-24 (a）의 라퓰라스 변환 및 역변환 실행 결과

0 syms 명령어를 이용하여 변수t를 지정한다．
0 laplace 함수를 이용하여 주어진 식의 라플라스 변환을수행한다．
0 湘place 함수를 이용하여 라플라스 역변환을수행하면 최초의 식과동일한 결과를 얻는다．
(b)

Commarsd Window
>> syms t 0
>> L2=IapIace(-2.cos(2.t)--3s1n(2*t) ) 0
L2=
6/(s'2 * 4) - (2.s)/(s2 + 4)
>> IL2=i Ia미ace(L2) 0
IL2 =
小引n（肛t) - 2.cos(2士t)
그림 아25 (b）의 라플라스 변환 및 역변환 실행 결과

0 syms 명령어를 이용하여 변수r를 지정한다．
0 laplace 함수를 이용하여 주어진 식의 라플라스 변환을수행한다．
0 ilaplace 함수를 이용하여 라플라스 역변환을수행하면 최초의 식과동일한 결과를 얻는다．

132

PART 02. M／노TLAB 핵심 기능 익히'I

LESSON

09

행렬의 특성 다항식 계산하기

행렬에 대한 특성 다항식과 특성 다항식의 근을 구할 따1 사용하는 심벌릭 함수 터g와 p이y에 대해 알아보자．
Keyword

I

I eig

고윳값 ! 고유 벡터 ! charp이y l 특성 다항식 !

eig

크기가 刃인 정방행렬 A가 있을 때 Au = 2u를 만족하는 0이 아닌 벡터 U가 존재하면 스칼라 2를 행렬
A의 고윳값k坦印value）이라하고, 벡터 U를 행렬 A의 고유 벡터 k培帥vect아）라한다．
특성 다항식 (characteristic polynomial)은 det(A-21）로 정의되며, 여기서 2는 특성 다항식의 근이
다. 심벌릭 고윳값 변수는 기본값으로x를 사용한다．
심벌릭 정방행렬 A에 대한고윳값을구하는 eig 함수의 기본 형태는 다음과같다．
아g(A)
· A: 심벌릭 정방행렬

I

charp이y

심벌릭 정방행렬 A어］대한특성 다항식을 내림차순 계수로 구성된 벡터 형태로 나타내는 charp아y 함수
의 기본 형태는 다음과같다．
charp아y(A)
· A: 심벌릭 정방행렬

CHAPTER 06. 수식 계산이 편한 심벌릭 툴박스

133

1 예제 6- 19 1
다음 행렬의 특성 다항식과 특성 다항식의 근을 구하라．

풀이

21
I
1 3k -7]
r-6

=I

A

Comman二

>> syms k 0

A=

>> A=［七. 2;3시
（. -71

[ - 6. 21
1 3.k, -7]

>> P=poIy2sym(charpoly (A) ) 0
P=
X八2 + 13士x = 6味 + 42

2

2

田 m2

11 甘

sqrt (24 k + 1)

田 m2

1

1

11 1 1 1 1 /

>> R=eIg (A) ; 0
>> pretty (R) 0
/ sqrt (24 k * 1)
1

그림 小26 행렬의 특성 다항식과 근 구하기 실행 결과

0 syms 명령어를 이용하여 변수无를 지정한다．
0 cha叩아y와poly2sym함수를 이용하여 행렬 A의 특성 다항식 寸 + 13工 + 42 - 6k를 얻는다．
' 이다．
0 eig힘수를이용햐뇌특성다항식의근을구하면：= 13 + Ji+ 24k
0 pretty 함수를 이용하여 주어진 수식을조판 형태로출력한다．

134

PART02. M戶:1-녀B핵심 기능익히기

CHAPTER

외부파일
불러오기／내보내기

CONTENTS
LESSON 01 그림 파일 불러오기／내보내기
LESSON 02 엑셀 파일 불러오기／내보내71

LESSON

01

그림 파일 불러오기／내보내기

생성된
MAT나＼B 환경에서 생성되지 않은 그림 파일을 MAT냐＼B 명령 창으로 불러오는 방법과, 반대로 MATLAB 환경에서
알아보자．
그림 파일을 보통의 그림 파일로 변환하는 방법을
Keyword

1 imread I image I

甘 imread
入4ATLAB을 사和｝치 않고생성된 그림 파일에서 이미지를 읽는imread 함수의 기본 형타는다음과긷다．
露難難

A 꾜 imr好瑟娃｛' 匙掛r客多）
. 'figure' : 변환할 일반 그림 파일
·A: MATLAB 그림 파일 이름

I

image

MATLAB 명령 창에서 열어볼 수 있도록 변환된 그림 파일의 이미지를 보여주는 image 함수의 기본 형
태는다음과같다．

image(A)
. A: 함수 mread률 사용하여 변환된 MATLAB 그림 파일

일반적으로 컴퓨터에서 열어볼 수 있는 그림 파일은 다양하다. 파일 이름이 ' figure'라고 해도 확장자어］
따라서 ' figure.bmp', 'flgure.gif ', 'figure.jpeg', 'figure.tiff ' 등 여러 가지가 있다. 각각의 유형은장단
점이 있으므로 사용 목적에 맞게 선택하면 된다. 그림 유형을 잘못 사용하면 작업을 망칠 수도 있고, 메모
리 공간을 지나치게 많이 차지하거나 그림이 열리지 않을 수도 있다．
사용하여
口if> 특별한 소프트웨어를 설치하지 않아도 모든 컴퓨터에서 다양한 확장자의 그림 파일을 열어볼 수 있다. 그러나 MATLAB을
figure.bm口'
'
않은
섕성된 ' figure.fig' 파일은 MATLAB이 설치되어 있지 않으면 사용할 수 없다. 또한 MATLAB 환경에서 생성되지
파일도 MATLAB에서 사용하지 못한다．

136

PART 02. MATLAB 핵심 기능 익히71

Fife I Matlab.bmp

1 예저I 7- 1 I

［그림 가1]은 MATLAB에서 생성하지 않은 파일（Ma扼b.bm히이다. 0I 파일을 MATLAB 명령 창으로 불러
와 MATLAB에서 사용할 수 있는 파일（Matiab.fig）로 변환하라．

그림 7너 그림 파일（Maab.bmp)

0 'Matlab.bmp' 파일을 불러오기 위해 명령 창어］다음과 같이 입력한다. 이때 반드시 현재 명령 창이 지정
된 경로（C:\Program Files\MTALAB\R2015b\bin)의 현재 폴더（작업 공간）에 'Matlab.bmp' 파일
이 저장되어 있는지 확인한다. 만일 여기에 파일이 없으면 함수가 작동하지 않는다．
Command Window
>> 州atlab = imread( Matlab. bnip ) ;
>> image(Matlab)
그림 戶2 'M졔bb.bm口' 파일을 MATLAB 명령 창에 불러오기

El11

첫 번째 명령줄의 세미콜론은 반듸1 지정해야 한다. 지정하지 않으면 그림의 코드를 나타내는 숫자의 배열이
연속적으로 표시된다．

0 ［그림卜2］를 실행하면 다음과 같은 그림 창이 열린다．
Fm

Et

5,ili

0甘口5

10此

r加哨娜1

獅m片mto씨夕 =

枷包

和

1

D (3 日 企 斗 曳 客． 好 自咀 / H 레 目 1크 a 口

50
100
1的
250
250
300
3텨）
'VM焄；

풀이

奴刃
450

蔑璉藝1 .' .
;

'

'

·

.

.

"

=

"

m"
.

500
'

스D{J

印

口＝

100

550

25刃

2的

헒刃

白

300

400

그림卜3 M川lAB 명령 창에서 보는 변환된 그림 파일（Maflab.f力

CHAPTE日07. 외부파일불러오기／내보내7i

137

File 1 graph.fig

1 예工II 7- 2 I

［그림 갸4］는 MATLAB 명령 창에서 생성한 파일（graph.fi이이다. 0I 파일을 MATLA日이 아닌 다른 환경어i
서도 열어볼 수 있는 파일（graph.bmp）로 변환하라．
F甘e

日墩

ve냅

h肖目t

TOOtS

地攷SI꾸 ＼사昨幻出 卜leip

抑 自 咀 J= , 艮 口 匡크 口 口
引nuB이dal Sign出：Acos如川1＋功
C)

0.8

0

0.6
0
八

0.4
0

1

甲

0.2

1
It

1

릎 0

1

0

0

0

0
0
8

10

12

14

16

18

껌

lilT月 [ni

그림 7닉 MAThAB을 사용하여 생성한 파일佃aph.fig)

==

I臣"I

0 'graph.fig' 파일을 열고 [File] -[Save as...］를클릭하면［그림 7-引와같은팝업 창이 열린다．

꼬 디스크 (C그 卜 Pr아prr F,Ier 卜 MAT녀B 卜 R2U15b 卜 bir, 卜

J겨羹기

自 "j료

！쁘파낸

卜置 李re中打y

竺다묜로도

邕 죄근뀌지

浮

上er3he9目fly

囹

少 Ii벼

수정한나
'짜
유험
파St뎌
2018-02＜蛤오후
2018七2吼오毛 파밀卦

꼰18心2띠6오乳

파畏 쯔4

파앝 미i(N) 曲
파낄 쥠식rn MAI8AS FIgure ('.8日)
뇨 to{ 合기기

그림 7凸 M시U\B 그림 파일을 일반 그림 파일로 내보내는 과정

0 ［파일 형식 (T) :］의 스크롤 바를 아래로 내리면 다양한 형식의 확장자가 있는데, 그중어］서 'Bitmap file
卜 .bmp) '를 선택하면 자동으로 현재 폴더에 'graph.bmp' 파일이 생성된다．
0 현재 폴더를 확인해보면 새롭게 생성된 'graph.bmp ' 파일이 존재한다. 확장자가 .bmp인 비트맵
(Bitmap) 파일은 기본적인 이미지 편집에 표준으로 쓰이고 있다. 다른 이미지 파일어］비해 고화질이고
편집과수정이 간편하다는 것이 장점인 반면 파일 크기가 대용랑이다．
EiD

MAT나＼B 명령 창이 열려 있는 상태에서 .fig 확장자의 MATLAB 그림 파일을 더블클릭하면 그림 창이 열린다．
그러나 .fig 확장자가 아닌 그림 파일은 더블클릭해도 그림을 볼 수 없다．새롭게 생성된 '아aph.bmp' 파일은
卜,1TALAB\R2015b\bin 디렉터리로 가서 열어야 한다．
현재 지정된 C:\Program 日！es＼

138

PART02. M戶ILAB 핵심 기능 익히기

LESSON

엑셀 파일 불러오기八H보내기

02

MAT나＼B 환경에서 생성되지 않은 엑셀 파일을 MATLAB 명령 창으로 불러오는 방법과, 반대로 MAT나＼B 환경에서 생성된
배열을 엑셀 파일로 변환하는 방법을 알아보자．
Keyword

I

! xlsread I xlswnte

xlsread

엑셀 파일을 읽어와MATLAB 명령 창에서 사용할 수 있는 행렬로 변환하는 넜sread 함수의 기본 형태는
다음과 같다．
A = xlsread('file')
· 'file' 변환할 엑셀 파일 이름
·A: 변환한 엑셀 파일이 저장될 MATLAB 행렬의 변수

I

川swrite

MATLAB 명령 창에서 생성된 행렬을 엑셀 파일로 내보내는赳swrite 함수의 기본 형태는 다음과 같다．
A = 州e.x怜
xlswrite(A, B)
.A: 변환하여 내보낼 엑셀 파일의 이름（加.xis）을 지정하는 변수
·B: MATLAB에서 생성된 행렬의 변수

CHAPTER 07. 외부파일 불러오기／내보내71

139

File 1 Data-in.xls

1 예제 7小

［그림 가6］은 엑셀 파일（Data니n.川히이다. 이 파일을 MATLAB 명령 창으로 불러와서 사용할 수 있는 행렬
변수 A로 변환하라．

;

日
파낄

홈

삽입

Da切dn ｛호환모드］ Excel
파이지 Z1미아믓

수식

X

뎌이El

겁토

困

E丙yD乂Urnent Creat아

보기

.

,

5

맞줌

口 표시 험식 口

D
3
0
l
l

B

三，

코딘

.

V 수헐촬 착멉읕 알려 주I요

瑪조건부서식 ,

昏삽밉 ,

스탸밑

뷸

口
토了亡

=

요 금묘

*」如3,：뇨，:, ,，‘二，’낳；其玉 旨 甘 ' 缸i 歡：1 프：薰랗嘉
쿨랖보드

口

A
19

1
2
3
小

14!
151

'7

14
2
4
4
9

二

11
l
l
2
l
l
l
B
l

5

2

7

4
8
5
3
15
12

3
8

10
3

F

G

H

3

l
l
l
l
l
l
l
l
l
l

다음과긷삐 입력하면 원래 엑셀 파일과동일한행렬을확인할수 있다．

m
山
m
1
1
1
1
1
1
1
1

>> A=oloread(Data- in. xls ')
A =

그림 7나 명령 창으로 불러온 엑셀 파일의 내용

140

편집

八

V
4C
9
13

그림 入6 엑셀 파일（Data니n.x始）

= .
굴（J1

C)

五
B
4
2
3
15
3

3
8
4

5
6
7
8
9

글꼴

中

C28

三 . ＝寸

PART02. t (AT냐＼B 핵심 기능 익히71

1

J

1<

L

미

i 예저I 7- 4 I
다음과 같은 행렬을 엑셀 파일（D欲于out.川旬로 변환하라．

l

87 巧 4

11上

百UI

96 好 3

52 m 2

n
J 4
1

캬

==

04행 4열의 행렬 B를 엑셀 파일（Data-out.xl帥로 생성하기 위해 명령 창어江十음과 같이 입력한다．

>> B = [3 6 9 S;4 2 6 7;1 10 13 I6;1 2 3 4[ ;
>> f 1 1 ename = Data-out xis ;
)> nls뿌rite(fi Iename .0) ;
그림 7田 행렬 B를 엑셀 파일로 내보내는 과정

0 현재 폴더를 확인해보면 엑셀 파일（Dat十out.xl旬이 있다. C:\Pro얗am Fil明小4TALAB\R2015b\
bin 디렉터리로 가서 해당 엑셀 파일을 열면［그림卜9］를 확인할수 있다．
;

H
I

町이지 레이아욧

수식

,:S寸兀 -U;.
쿨립보드
88

;
!

［恥거E1

검토

보기

Eay 0（乂Urnent Cr0카or

口

0 수험할작멸클 알O 주세요

로그인

乙

묘줄

4

표A 춈 1

F

G

H

二단밀

퓰

,t

5= 공뮤

：繫：二 和冬茗冬31 '-冬晏

굴굴

A
l
2
3
4
5

固

Data＜가Jt ［호롼 모드］ EX떠

삽업

젼집

小

二

B

C

D

F

3

3

9

8

4
1

2
10

6
13

15

1

2

3

4

I

J

K

L

M

"

그림 石9 새롭게 생성된 엑셀 파일（0졔a-o吼xis)

CHAPTER 07. 외부파일불러오기／내보내기

141

MATLAB

활용하기

"정확한 수치해석은 MAThAB의 능력을 빌리세요“
제어
'MAThA8 사용의 시초는 제어 분야예요"
신호 및 시스템
'신호의 개념은 MATLAB 그래프로 이해하서阻"
CHAPTER 1

전자7障t
" 어려운 벡터 해석도 MATLAB이 쉽게 해주네요"
룡신
"스마트 통신은 스마트한 h肛ILAB이 최고지요"

難蠶蠶囊鞋囊
驥韆蘿蠱驛蠶
蠶韆蠶醫鹽
鞋蠶轟鹽鹽烈發
雖韆囊豫蟹騷盈
釀驀瑟鹽恥毋疊
也坦發盤磁磁發堪礎曝礎轟堪小

mm匹阻隘隘圈匹國恥麒隘發回

＃照凞m

三
a目a拉m目好明月懈

11m目丑匹g月目月匹聽h

초보 운전에서 벗어나 자신이 가고 싶은 곳으로 운전해 가는 방법을 배워보자．
MATLAB은 수치해석， 제어， 신호 및 시스템, 전자기학, 통신 등 다양한 분야어囚
활용할 수 있다． 3부에서는 MATLAB을 활용하여 분야별 예제를 해결해본다．
수치하［석은 수치적인 근삿값을 구하고 오차를 줄이는 학문으로 정확한 값을
는 것이 매우 중요하다． 8장에서는 다양한 MATLAB 함수／명령어를 이용하여 선형
방정식의 해를 구하고， 가우스 소거법과 상하행렬 분해를 이용하여 변숫값을 찾아
본다； 또한 보간법과 미적분을 수행하는 함수를 이용하여 편리하고 정확하게 계산
한다．
제어는 MATLAB을 처음으로 활용한 공학 분야이므로 MATLAB은 제어에 대한
다양한 기능을 제공한다． 9장에서는 MATLAB을 이용하여 전달함수어i 대한 계단‘
응답을 그래프로 나타낸다．
공학에서 입력 신호와 출력 신호를 해석하는 것은 전체 시스템의 성능과 구조를 이
해하는 뎨 큰 영향을 미친다. 수학 계산쇄만 의존한 신호 해석으로는 전체 시스템을
이해古끼 어렵기 때문에 10장에서는 신호를 그래프로 나타내어 한눈에 신호와 전체
시스템을 이해할 수 있도록 돕는다．
벡터를 이해하지 못한 상태어1A1 전기장과 자기장을 이해하는 것은 매우 어렵다. 11
장에서는 MATLAB 함수／명령어를 이용한 벡터의 연산부터 장전기장과 정자기장에
서의 전자기적 특성을 계산하는 방법을 배운다. 또한 MATLAB의 심벌릭 툴박스를
이용하여 전기장과 자기장의 특성을 간편하게 계산할 수 있는 스크립트 파일을 작성

해
苞m 二 =J 1 m工H

듄

쿄

1i'

L+ 1 'J

口 IL

l1

入1

万4

장어｝서는 아날로그 변조와 복조，디지털 변조 등 통신의 기초 내용을 MATLAB 스
크립트 파일로 작성하고， 그래프를 통해1 더욱 쉽고 간편하게 결과를 이해하는 과정
을 학습한다．

CHAPTER

수치해석

CONTENTS
LESSON 01 2진수와 ]0진수 변환
LESSON 02 오차
LESS아寸 03 역행렬
LESSON 04 선형연립방정식
LESSON 05 가우스 소거법
LESSON 06 상하행렬 분하1
LESSON 07 테일러 급수
LESSON 08 테일러 다항식의 근삿값과 오차
LESSON 09 선형 보간법과 스플라인 보간법
LESSON 10 함수의 근 구하71
LESSON 11 함수의 근을 구하는 다양한 방법
LESSON 12 수치 적분법
LESS아止 13 수치 미분법

LESSON

01

2진수와 10진수 변환

10진법온 10진수의 ]0개 숫자（0N9）를 사용하여 숫자를 표현하고, 2진법은 2진수의 2개 숫자（0.1)를 사용하여 숫자를 표현
힌타. MATLAB올 통해1 인간이 데이터를 처리할 때 사용하는 숫자인 ]0진수와 컴퓨터 내부에서 데이터를 처리할 때 이용하는
2진수의 상관관계플 알아보자．
Keyword

I bin2dec i dec2b1n 1 Fr_biri2dec 1 Fr_dec2bin I

1 2진 정수를 10진 정수로 변환
2진 정수（b血ary integer) B는 다음과 긷미 0과 1로 구성된 유한수열 형태로 표현된다．
(8.1)

B = (bib刃日 ···Zb自b0)2
식 (8.1）을 10진 정수（decimal integer) .1）로 변환하기 위해 다음과긷枸］계산한다．

(8.2)

D=b2"+ b_12" '+ ·..+b12'+ b。
예를 들어 2진 정수B =(1001)2를 10진 정수로 변환하면 다음과 같다．
D = 23 + 20 =9

I 10진 정수를 2진 정수로 변환
10진 정수를 2진 정수로 변환하려면 식 (8.2）를 2로 나누어 생긴 몫 1기을 다음과 긷삐 표현한다. 이때
나머지는 b0라고 한다．
D1 =b.2' 1+b_12' H2 +...+k20
I기을 2로 나누면 다시 몫이 생기고 나머지는 히 이 되는더］, 몫이 0이 될 때까지 이 과정을 반복한다. 이때
의 나머지를 역순으로 나열하면 2진 정수를 얻을수 있다．
예를 들어 10진 정수 9를 2진 정수로 변환하면 다음과 같다．

2

= D2

2）三

1

=

b0 = I

=

2J

=

= I긔

2J

4

PART03. M月TLAB활용하71

= I兀

b2= 0

1 = 0 = ／가 Zb = l

2)
146

b1= 0

각단계에서 구한나머지를 역순으로 나열하면 (b3b2自b0)2 = (1001)2와긷미 2진 정수를 얻을수 있다．

1 예처18-1 I

而；
지식

'

2진 정수 1001을 10진 정수로 변환하라. 반대로 10진 정수 9를 2진 정수로 변환하라．

bin2dec

2진정수를10진정수로변환하는bin2dec함수의 기본형태는다음과같다．

bin2dec('num')
I加2dec 함수를 사용할 때는 반드시 숫자를 작은따옴표로 묶어야 한다. 그렇지 않으면 오류 메시지가 나타
난다．
口 dec2bin
10진 정수를 2진 정수로 변환하는 dec2bin 함수의 기본 형태는 다음과 같다．

dec2bin(num)
dec2bin 함수를 人卜용할 때는 숫자만을 입력해야 한다. 만약 숫자를 작은따옴표로 묶어서 입력하면 그 값을
아스키코드로 변환한후 2진 정수로 변환하므로 원하는 결과를 얻을 수 없다．

풀이

Command Windcr
>> bin2dec ( 山01 ) <1
ans =
9
)> dec2帥(9) Q
ans =
1001
그림 8너 10진수와 2진수 상호 변환하기 실행 결과

0 bin2dec 함수를 사용하여 2진수 10아을 10진수로 변환한다．
0 dec2bin 함수를 사용하여 10진수 9를 2진수로 변환한다．

CHAPTE日 08 수치해석

147

專 2진 소수를 ]0진 소수로 변환
일반적으로 2진 소수伯mary fraction) B는 다음과같히 0과 1로 구성된 무한1＝열 형태로 표현된다．
B=(.b1b2b3 ·..bn ··.)2

(8.3)

식 (8.3）을 10진 소수（decimal fraction) D로 변환하기 위해 다음과 긷미 계산한다．
(8.4)

D= 히2e1+ b22m2 +b32e3 + ···
예를들어 2진 소수 (0.10001h를 10진 소수로 변환하면 다음과같다．
D= 2 ' +2巧 =0.5+ 0.03125= 0.53125

1 예저18-2 I

M-File I Fr bin2dec.m

2진 소수 (11.1101万와 (0.10001万를 10진 소수로 변환하라．

bin2dec

'

지식

2진소수를10진소수로변환하는사용자정의함수Fr_bin2dec의 기본형태는다음과같다．

Fr_

-

Fr_bin2dec('num')
Fr_bin2dec(num)
2진 및 10진 정수와 달리 작은따옴표가 있거나 없어도 실행 결과는 같다. 단, 사용 중인 현재 폴더어］
'Frbin2dec.m'이 있을 때만 이 함수를 사용할 수 있다．

풀이

Comm크

:: 怨磊；::：魚叫0
3.미떠刃0000D000IJ
>> Fr上In2dec( 口 10001 ) 0
a08 =

0. 531客i互刃CDCDoo
그림 +2 2진 소수릎 10진 소수로 변환하기 실행 결과

0 소수쩜 자리를확장하기 위해 format long을설정한다．
0 氏너n2dec 함수를사용하여 2진 소수 (11.1101)2를 10진 소수로 변환한다．
0 氏bin2dec 함수를사용하여 2진 소수 (0.10001)2를 10진 소수로 변환한다．

148

PA日T 03. M』町냐＼B활용하기

10진 소수를 2진 소수로 변환

I

10진 소수를 2진 소수로 변환하기 위해 식 (8.4）를 다음과 같이 다시 쓸 수 있다．
D =1긔 ＝히2'' 十b22"2 +b32m3 + ·．·
여기에 2를곱하면 히은 정수가 되어 다음 식부터는사라진다．
D2 =b22 ' +b32'2 +b42e3 + ···
D2어］다시 2를 곱하면 b2는 정수가 되며, 소수 자리가 0이 될 때까지 이러한 과정을 반복하여 진행한다．
생성되는 정수를 차례대로 나열하면 변환된 2진 소수를 얻을 수 있다．

M-File

1 예저18-3 I

Fr dec2bin.m

10진 소수 (97．끄25)io과 (0.6125)m을 2진 소수로 변환하라．
-

' Fr_dec2bin

지식

10진소수를2진소수로변환하는사용자정의함수Fr_dec2b血의 기본형태는다음과같다．

Fr_dec2bin('num')
Fr_dec2b1n(num)
2진 및 10진 정수와 달리 작은따옴표가 있거나 없어도 실행 결과는 같다. 단, 사용 중인 현재 폴더에
'Fr小c2bin.m'이 있을 때만 이 함수를 사용할수 있다．
풀이

Command Windo,/
>> f口rniat

1三

<1

" Fr_dec2b1n(97. 3l25) 0

iicn刃1. 0101
>> Fr_dec2bin(0.6125) 0
ans =
0. 1［刃iiicxjiicx기 11刃1
그림 8田 10진 소수를 2진 소수로 변환하71 실행 결과

0 소수점 자리를확장하기 위해 form毗long을 설정한다．
0 Fr_dec2bm 함수를사용하여 10진 소수 (97．끄25)m을2진 소수로 변환한다．
0 Fr_dec2bin 함수를사용하여 10진 소수 (0.6125)10을2진 소수로 변환한다．

CHAPTER 08. 수치해석

149

오차
실젯값과 근삿값의 차이를 오차라고 한다．오차가 발생하는 근본적인 원인은 미지의 현상을 분석하71 위하1 수학적으로 모델링
하여 계산하는 과정에서 오류가 발생하기 때문이다．MATLAB을 이용하여 오차를 계산하는 방법을 알아보자．
Keyword

I

I 절대 오차

상대 오차 I round I

절대1 오차

절대 오차는오차어］절댓값을취한 결과이다. 실젯값을工, 컴퓨터로끝수 처리 또는잘라버리기를 실행하
여 구한근삿값을 x라고 할 때 절대 오차는 다음과 같끼 쓸 수 있다．
절대 오차늬x-士I

(8.5)

잘라버리기를 척용하여 구한 근삿값은 실젯값보다 작고 오차는 항상 양의 값이다. 끝수 처리 중 올림을
적용한 경우는 근삿값이 실젯값보다 크기 때문어］오차가 항상 음의 값이고, 내림을 적용한 경우의 오차는
항상 양의 값이다．

I

상대1 오차

상대 오차는 오차와 실젯값의 비율을 의미하며, 절대 오차와 유효자리를 맞추어 계산한다. 상대 오차는

三1

상대 오차 =

즈二，

다음과 긷히 쓸수 있다．
(8.6)

즉 절대 오차는 오차의 절댓값이고, 상대 오차는 비교 대상어］따라 크거나 작거］ 느껴지는 오차이다. 결국
절대 오차가 작으면 상대 오차도 작다．

1 예제8니 1
유효숫자 여섯 자리伽 = 6). 지수의 최소 정숫값 -40(in = -40）과 최대 정숫값 40(M= 40), 그리고 끝수 처
리 기능이 있는 컴퓨터가 있다고 하자. MATLAB을 이용하여 2.99792458X 10뱌cm/s] 에 대한 절대 오차와
상대1 오차를 구하라．

150

PART 03. WkTLAB활용하71

배경
지식

1round
round 함수를사용하면 올림 또는 내림을 실행할수 있으나사용이 제한적이다. 따라서 먼저 지수승을 제외
한부동 소수점어］대한 끝수 처리를 round 함수로 실행한후 지수승을 곱하여 표현한다．
끝수 처리를위해 벡터 工의 각 원소를 가장가까운 정수로반올림하는round 함수의 기본 형태는 다음과같다．

round（지
· X: 반올림할 벡터

풀이

r mand Window

,, ,,,,, 0
:,:，三多三照，
凡hat =
2, 납냠／늬. ,J-JuuuIJ벼i_U
>> abs_error=abs(o너了10-a_hat시了10) 0
abs_error =
45& )
>> a_real=round (a시13그）/1며J e
s_real =
3
>. rel_errar=abs (abs_error/(a_real시了10)) 0
rel_errar =
1 526666066666667e-06
그림 小4 절대 오차와 상대 오차 구하71 실행 결과

0 소수쩜 자리를확장하기 위해 format long을설정한다．
0 계산의 편의를 위해 주어진 값에서 1010을 생략하여 지정한다．
0 유효숫자가 여섯 자리이므로 100000을 곱하여 여섯 자리 정수로 만든 후 round 함수를 사용하여 끝수
처리를 실행한다. 그런 다음 100000으로 나누어 근삿값을 계산한다．
0 생략한 1010을 실젯값과 근삿값에 곱한다. 그리고 실젯값몌서 근삿값을 뺀 값혀1 절댓값을 취하여 절대
오차를 구한다．
0 절대 오차는 4.58 x104으로 유효숫자가 세 자리이다. 따라서 상대 오차도 유효숫자를 세 자리로 맞추기
위해 100을 곱한후 round 함수를 사용하여 끝수 처리를 실행한다. 그런 다음 100으로 나누어 상대 오只下
에 사용할 실젯값을 계산한다．
0 상대 오차를구하기 위해 절대 오차를3.00 x 1010 (0에서 구한값）으로 나누고 절댓값을 취한다．

CHAPTER 08. 수치해석

151

LESSON

03

역행렬

행렬방정식 Ax = c의 하Ix를 구하려면 상수 벡터 C를 행렬 A로 나누어야 한다. 행렬방정식의 해를 구하:7 ' 위하1 나누는 행렬
A는 K '로 나타내며, 이를 행렬 A의 역행렬이라고 한다. MAT나＼B 명령어를 이용하여 역행렬이 존재하는지 확인하고， 역행
렬을 구해보자．
Keyword

I

! 정칙행렬 1 비정칙행렬 1 행렬식 1 det i m v 1

역행렬

행렬 A의 역행렬（inverse matrix) 可l이 존재하려면 행렬 A는 반드시 정방행렬이면서 행렬식의 값이 0
이 아닌(IAI / 0) 정칙행렬（nonsii乷ular matrix）이어야 한다. 행렬식의 값이 0인(IAi =0) 비정칙
행렬（singular matr汶）은 역행렬을 가질 수 없다．
역행렬 A '과 행렬 A 자신을곱하면 다음과 같이 단위행렬 I가 생성된다．
A已＼= AA ' = I

(8.7)

행렬방정식을 일반화한 식 Ax = c의 양변에 역행렬 A크를 곱하면 다음과 같다．
A1Ax = A二＝

(8.8)

여기어］식 (8.7）을 이용하면 행렬방정식의 하나를 구할수 있다．
x = A 'c

(8.9)

행렬 A의 역행렬 A니을 구하는 과정은 다음과 같다．
(7l2
a12

a13

(722
a22

a23

口32

口33.

0 정칙행렬 조건을 만족하는 행렬 A의 행렬식을 구한다．
det(A) = 口11口22口33 卄112口23口31 + 口l3(732口21 m 口13口22口31 - 口12口21口33 크lila32屯3 尹 0

152

PART03. M月T나＼B 활용하기

日 (111이 포함된 행과 열을 제외한 나머지 원소만으로 새로운 2x2 행렬어］대한 행렬식을 만들고 M11이
라 지정한다. 이를 口11어］ 대한 소행렬식 (n血均r）이라고 한다. 같은 방법으로 나머지 원소어］ 대한 소
행렬식을구한다．
det（兀／n) =

口22

口23

口32

口33

= a22口33- a23口32

日 口11 자리에 A介 값을 지정하고 다른 자리에도 소행렬식 방법으로 구한 나머지 값을 지정한 뒤 행과 열
을 전치한다. 이렇게 구한행렬을 행렬 A에 대한수반행렬（ad如m t）이라고하며 A由（A）로표현한다．

[M11

MMM

珦 怖 怖

MMM

나I3l

r

怖 怖 岷

=

刈（시＝甲21

怖 怖 岷

=

1

日 수반행렬의 여인자（C可actor）를 지정한다. 여인자는 행과 열의 수를 더한 결과가짝수이면 양의 부호

M12

-

+M11

(+）를, 寄 이면 음의 부호(-）를 붙인 것을 의미한다．

M13

+

日 위의 口에서 구한 행렬을U에서 구한 행렬 A의 행렬식으로 나누면 최종적으로 행렬 A의 역행렬 A1
을 얻을 수 있다．

-

e

+ +
e
H

+

乙 乙 石
A A A

勾 勾 行
A A A

\

仄
시 工
l 工
1

A

e
d

j 4 A

l

A 1

4

1 （계저18-5 I

[1

MATLAB을 이용하여 행렬 A. B의 행렬식 값과 역행렬을 구하라．
0

11

A디0 1 키， B=
L2 2
3j

배경
지식

1

5

3'

2

8

6

1

2

3

1det
역행렬이 존재하는지 확인하기 위해 행렬 A의 행렬식 값을구하는det 명령어의 기본 형태는 다음과같다．

CHAPTER 08. 수치해석

153

det(A)
. A: 행렬식 값을 구할 행렬

I

ll} \/

행렬 A의 역행렬 A '을구하는 血V 명령어의 기본 형태는 다음과 같다．

inv(A)
'A: 역행렬을 구할 행렬

풀이

>> H =H 0 1;0 1 -1;2 2 31;
>> d町的 0
ann =

>> inn（肋 0
ass =
1 . 5타；7
-0 旼石7
-0. 6667

0.656'l
0. 3了田
-0, 旺；57

-0.3333
0．芻33
0. 3333

,> 6=11 6 3;2 8 6;l 2 31;
>' det (B) 0
극 m극 =

>> inv (B) e

日3rflifl9: Matrin is singular to working precislon. O
ans =
mnl
mnl
mnl

1 nt
1 ni
mnl

mnl
1 ni
lot

그림 8巧 역행렬 구하기 실행 결과

0 det 명령어를 이용하여 행렬 A의 행렬식을 구하여 역행렬이 존재하는지 확인한다‘
0 mv 명령어를 이용하여 행렬 A의 역행렬을 구한다．
0 det 명령어를 이용하여 행렬 B의 행렬식을 구하여 역행렬이 존재하는지 확인한다．
0 행렬 B는 행렬식의 값이 0인 비정칙행렬이므로 역행렬을 구할수 없다는 메시지 (0）가출력된다．

154

PART03. M凡AB활용하71

LESSON

04

선형연립방정식

j차 방정식에 미지수 3개（工, y, z)가 있다면 최소한 3개의 1차 방정식이 있어야 모든 미지수의 값을 구할 수 있다. 이따1 서i ] 차
방정식을 동시에 만족하는 값이 바로 연립］차 방정식의 해이다. 수학의 가감법, 대입법, 등치법을 이용하면 세 j차 방정식을
동시에 만족하는 工, y z의 값을 쉽게 구할 수 있다. 이와 동일한 방법으로 MATLAB의 다양한 명령어를 이용하여 선형연립방
정식의 해를 구히보자．
Keyword

I

i 선형연립방정식 ! 왼쪽 나눗셈（N)

역행렬 1 크래머 법칙 1

선혐연립방정식

방정식의 각 항히 상수와 변수의 곱으로 이루어져 있다면 이를 선형방정식이라고 한다. 선형방정식에 미
지수가n7]] 있다면 n711의 선형방정식이 있어야모든 미지수의 값을구할수 있다. 선형연립방정식은 2개
이상의 미지수를 포함하는 방정식의 조합으로, MATLAB에서는 선형연립방정식의 해를 구하기 위해 왼
쪽나눗셈, 역행렬, 크래머 법칙을이용한다．

I 왼쪽 나눗셉
행렬방정식을 일반화하면 다음과 같이 표현할수 있다．
(8.10)

Ax = C

왼쪽 나눗셈 방법은 가우스 소거법을 근거로 이용한다. 가우스 소거법에 대한 자세한 내용은 다음 레슨을
참조한다. 왼쪽 나눗셈을 이용하여 행렬방정식을 풀면 다음과 같다．
x= A\ c
1 여以｛IR- f

I

7z

=

[

나3y

2y-

5y+ 4z

=

9x+

1

6x+

MAT냐＼B의 왼쪽 나눗셈을 이용하여 다음 선형연립방정식의 하나, y. z를 구하라．
55
43

+6z = 49

CHAPTER 08. 수치해석

155

侄）

Ccr가n그3nd \\j n由y.V

풀이

>, A=[6,2,-7;9,5, 4;-5,-3,61 0
A =
6
9
-5

2
5
-3

-7
4
6

>> c=[55; 43;-491 0
c=

묘5
43
-49

ans =

-3,

5．口더叩
2. 013J0

'> A/c e

Error using 工 0

Matrix dimensions must ogres

그림 +6 왼쪽 나눗셈을 이용하여 선형연립방정식의 하1 구하기 실행 결과

0 선형연립방정식의 미지수x, y, z를구하기 위해 계수행렬 A를 지정한다．
0 상수 벡터 C를 지정한다．
0 왼쪽 나눗셈 연산자（\）를 이용하여 선형연립방정식의 미지수를구한다．
0 왼쪽 나눗셈 연산자（\ ) 대신 오른쪽 나눗셈 연산자（/）를 이용하면 행렬의 차수가 일치하지 않는다는
오류 메시지 (0）가 나타난다．

I

역행렬

Ax = c는 선헝 시스템을 행렬방정식으로 전환한 것으로, x어］대한 해를 구하려면 상수 벡터 C를 행렬 A
로나누어야한다. 행렬A의 역수형태는A니로나타내며, 이를행렬A의 역행렬이라고한다．

1 예제8-7
역행렬을 이용하여 다음 선형연립방정식의 해를 구하라．

9x+

'

=

[ 缸＋2y口 55
1 5y+ 4z= 43
1-5x- 3y+ 6z =-49

156

PART03. M月TLAB활용하71

9, 4;

-6,

-7;

5,

>> A L6,

2,

I

-3,

6)

4=

풀이

6
9
-5

2
5
-3

-'7
4
6

>' c=(弱;43;-49J e

또
43
-49

>> 1nv (A）蛇 0
5. Xln
2. c1표｝
召JllL
그림 +7 역행렬을 이용하여 선형연립방정식의 해 구하기 실행 결과

0 연립방정식의 미지수 工, y, z를구하기 위해 계수행렬 A를 지정한다．
0 상수 벡터 C를 지정한다．
0 mlv 명령어를 이용하여 행렬 A의 역행렬을구한후 행렬 C와곱하여 선형연립방정식의 해를 구한다．

I

크래뻐 법칙

행렬식 1 Al는 행과 열의 수가같은 정방행렬에 수를 대응시키는함수이다. IAI가0이 아닌 경우에만 연
립방정식의 해가 존재하기 때문어］행렬식을 이용하여 연립방정식이 유일한 해를 갖는지 결정한다．
행렬식으로 된 연립방정식은 크래머 법칙을 이용하여 체계적으로 풀 수 있다. 두 연립방정식에 대한 행렬
식이 다음과 같다고 가정하자．
[all,

(11,21{ xh,
口21

l [ ]

口22 ii工2i

c1,

[C2

이때 미지의 변수차과工2는 크래머 법칙에 따라 다음과 같은 순서로 구할수 있다．
口 계수행렬 A의 행렬식을구한다．
det(A) = a11a22 -a12a21
日 행렬방정식의 오른쪽상수 벡터를 계수행렬 A의 첫 번째 열에 모두 대치한 행렬의 행렬식을구한다．
det(A1) = c1a22 -c2a12

CHAPTER 08. 수치해석

157

日 앞의 O와 같은 방법으로 샹수 벡터를 두 번째 열에 모두 대치한 행렬의 행렬식을 구한다．
det(A2) = C2口11 -C1口21

0 앞의日와日에서 구한 값을 O에서 구한 값으로 나누어 미지의 변숫값을 구한다. 그 결과는 각각 다

,

det

x2=

,

UCt(A)
)

aet(A)
(A1)

x1-

(A2

初＝

det

차-

음과같다．

1 예제8田 1

9x+

2y口'

=

[
1

缸＋

크래머 법칙을 이용하여 다음 선형연립방정식의 해를 구하라．
55

5y+ 4z= 43

匕5工 -3y + 6z = -49
풀이

>> A=(6, 2J-7;9,5, 4;-5,-3,6] ;
>> C늬弱；43;-491 ;
>) D=det ( ) ;
>> AI=[또,2,-7;43. 5,4;-49, -3.6I;

>> 미내日t(AI); e

>> A2=(6, SS, -7;9, 43,4;-5, -49,6J;
>> D2내叭（A2) ; 0
>> A3=[6, 2, 55;g, 5,42;_5, _3,-.49J;
'> D3=det (A3) ; 1
>> X늬기／D e
X =

5. Oat刃
>> y=D2/D
y =
2. m O口
>> Z=OO/D
Z =

-3.미000
그림 小8 크래머 법칙을 이용하여 선형연립방정식의 하1 구하기 실행 결과

0 det 명령어를 이용하여 행렬 A의 행렬식을구한다．
0 상수 벡터 C를 계수행렬 A의 첫 번째1 열에 모두 대치한 행렬의 행렬식을 구한다．
0 상수 벡터를A의 두 번째 열에 모두 대치한 행렬의 행렬식올 구한다．
0 상수 벡터를A의 서1 번째 열에 모두 대치한 행렬의 행렬식을구한다．
0 대치하여 구한 행렬식들을 처음꼐 구한 행렬식으로 나누어 미지의 변숫값을 구한다．

158

PART03. M月TLAB활용하71

LESSON

05

가우스 소거법

방정식이 II 개이고 미지수가 'I 개인 선형 시스템을 풀려면 '7 번째 방정식의 미지수가 하나
（x)만 남을 때까지 계속 소거해야 하
는데 이를 가우스 소거법이라고 한다. MAT나＼B에서 가우스 소거법을 이용하여 변숫값을 찾아보자．
Keys月ord

I

1 순수 가우스소거법 i 피벗 방정식 } Gauss I

가우스 소거법

가우스 소거법 (Gauss elimin餌on）은 행렬의 자리 바꿈을 이용하는 피버팅 방법과 피버팅을 사용하지
않는 방법으로 나뉜다. 피버팅을 사용하지 않는 가우스 소거법은 피버팅을 사용하는 방법과 구별하여 순
수 가우스 소꺼법이라고 한다. 순수 가우스 소커법은 다음과 같이 실행한다．
0 피벗（p加아） 방정식이라부르는 첫 번째 방정식에 적당한 인수를 곱하고, 다른 방정식의 변수 하나를
소커하기 위해 더하거나 뺀다. 같은 피벗 방정식을 이용하여 나머지 방정식어］대해서도 같은 과정을
실행한다. 이러한 과정을 거치면 첫 번째 방정식을 제외하고 나머지 방정식은 변수 하나가 줄어든 새
로운 방정식 세트를 형성한다．
日 새롭게 형성된 방정식 세트의 첫 번째 방정식을 다시 피벗 방정식으로 놓고 앞의 과정을 계속 실행한
다. 방정식 하나, 변수 하나가 남을 때까지 이 과정을 반복한다. 이 방법은 컴퓨터로 구현하끼어］'척합
하여 선형방정식을 풀끼 위해 고안된 많은 방법의 기초로 이용된다.
日 변환된 상숫값cn을 변환된 뉵의 계수로 나누면 斗의 해를 구할 수 있다. 또한 刃번째 방정식에서 계산
돈뇨刃의 값을 바로 앞刃크번째 방정식에 대입하면瓦-1 의 해도 얻을수 있다. 같은 방법으로 계속후진
대입법 (backward substitution）을 실행하면 첫 번째 방정식에서 차 의 해까지 구할수 있다.

M-File i Gauss.m

1 예제 8- 9 I

선형 시스템 Ax = C에 대한 행렬이 다음과 같을 때 순수 가우스 소거법을 이용하여 변수 工l , 工2 , 工3 , 工4를 구
하라，

0

n
乙

口8

n
乙

x

工2
c=

m
乙

八
乙

八
U
n／

0

尸
＼口

0

n
니 0 0

A=

工l

工3
x4

1
3
4
4-

CHAPTER 08. 수치해석

159

배경
지식

1Gauss
순수가우스소거법을실행할수 있는사용자정의함수Gauss의 기본형태는다음과같다．

Gauss(A川
· A: 계수행렬
· 0: 상수 벡터

명령 창에 계수행렬 A와 상수 벡터 C를 먼저 지정한 후 함수의 인자로 이용한다. 단 ，사용 중인 현재 폴더
에 'Gauss.m' 이 있을 때만 이 함수를 사용할 수 있다．

풀이

>> A=[1 -1 0 0;-1 5 2 10 2 2 2;0 0 2 61 0
A =
D

n
< D
느

D
7
느

n
亡

日

1

0

二
나

1

n
< 0

00

d
1

1
11
1

>> c=[1;3; 4; 41 0
C =
d
1
n
口
4
4

>> 0auss (A』c) e
ans =
]
0
n
< 0

그림 小9 순수 가우스 소거법을 이용하여 하1 구하기 실행 결과

0 계수행렬 A를 지정한다．
0 상수 벡터 C를 지정한다．
0 Gauss 함수를 이용하여 순수 가우스 소거법으로 변숫값을 구한다．

160

PART 03. MAT녀B활용하71

LESSON

싱하행렬 분히I

06

방정식의 상하행렬 분해는 가우스 소거법을 기초로 한다. 가우스 소거법을 이용하면 선형 시스템을 간편하고 안정적으로 풀
수 있지만 행렬의 차수2} 커지면 연산 카운터가 매우 증가하여 컴퓨터의 실행 속도가 떨어진다. 따라서 가우스 소거법의 단점을
보완하기 위해1 실행 속도가 빠른 상하행렬 분해를 사용한다. MATLA.B에서 상하행렬 분해를 이용하여 변수 벡터를 짖하보자．
Keyword

I

I 가우스소거법을 이용한상하행렬 분해1 I lu I 치환행렬 1 부분피버팅을 이용한상하행렬 분하I I

가우스 소거법을 이용한 상하행렬 분히1

상하행렬 분해 (LU: Lo＼叱卜Upper）를 이용하여 주어진 선형 시스템의 정방행렬 A를 다음과 같은 형태
로 나타낼 수 있다．
A= LU

(8.11)

여기서 L은 하삼각행렬(lower triangular matr奴）'U는 상삼칵행렬佃pper triangular ma甘汶）을 나
타낸다. 하삼각행렬은 주 대각선을 기준으로 위쪽에 위치하는 모든 원소가 0인 행렬이고, 상삼각행렬은
주 대각선을 기준으로 아래쪽어］위치하는 모든 원소가 0인 행렬을 말한다．
예를 들어 fl X77 정방행렬 A어］대한 상하행렬 분해는 다음과 같이 표현된다．
口11

a12

'""

a21

a22

...

"'
..

a1刃
a2n

l

0

121

1

131

0
0

0

U11

U12

"

U177

0

0

u22

·

U2fl

0

0

0

132

0
ani

a772

"""

'"

口nfl

.'nl

ln2

" " " ／刃，刃크

1

(8.12)
0

0

0

0

i/72n-

여기서 하삼칵행렬은 순수 가우스 소거법에서 사용한 승수와 같고, 상삼각행렬은 순수 가우스 소거법에
서 마지막 단계의 계수행렬을 나타낸다．
선형 시스템 Ax = C를 간단하게 풀기 위해 식 (8.11）을 이용하면 다음과 같다．
LUx= c

(8.13)

OH／놔JTE日08, 수치해석

161

식 (8.13）은 다음과 긷히 두 단꼐로 나누어 쓸 수 있다．
Ly = C

(8.14)

Ux = y

여기서 시스템 Ly = C는 하삼칵행렬 L을 포함하는 선형 시스템 형태가 된다．
ill

= Cl

'21Y1 + Y2

= C2

131Y1 +132y2 + y3

=c3

(8.15)

lnly1 +...+ln,n_iyn_i+ yn = cn

식 (8.15）를 전진 대입법 伽rward substitution）으로 풀어서 변수 벡터 y를 먼저 구한다. 그리고 시스
템 Ux =y어］후진 대입법을 적용하여 최종적으로 변수 벡터 x를구한다．

1 예제 8- 101

지식

'

1

5

-1

6 "x1'

19

2

-1

1

-2

x2

7

1

4

-1

3

x3

20

3

-7

-2

1 - -x4 '

-75

lu

；而

가우스 소거법을 이용한 상하행렬 분해를 통하1 하삼각행렬, 상삼각행렬 및 치환행렬을 구하라．

MATLAB에서 상하행렬 분하를 이용하여 선형 시스템의 변수 벡터를 구하는 'U 함수의 기본 형태는 다음과
같다．

[L,U尸卜山（A)
. L: 하삼각행렬
· U: 상삼각행렬
· P: 부분 피버팅에서 실행된 자리 바꿈을 보여주는 치환행렬
· A: 선형 시스템의 계수행렬

162

PARTU3. M月ILAB 활용하71

Command Window

侄）

>> A=[l 5 니 6;2 -l I -2；너 4 -1 3;3 小7-2 II; 0
>> [ L.U. P]＝山（시 0
L=

풀이

i .[mJ
0.3333
0，旼；67
七.3羽3

0
1 .0000
0．印00
0. 2273

0
0
1 . mU
-0且蛤4

0
0
0
1 .0000

3. 0000
0
0

-7. 0000
7．羽羽
0
0

-2. (fl刃
七.田33
2.SIXU
0

1. [lll)
5.1正百7
-s, 모xi
-1. 4645

U =

口

1
1
0 0 口

0
0
1
U
n 1

0 0
D
1
1

0 1 0 D

그림 &너0 가우스 소거법을 이용한 상하행렬 분해 실행 결과

0 선형 시스템의 계수행렬 A를 지정한다．
Olu 함수로 가우스 소거법을 이용한상하행렬 분해를 실행한다．

I

부분 피버팅을 이용한 상하행렬 분히1

부분 피버팅을 이용하여 싱하행렬 분해를 실행하는 경우에는 식 (8.11）을 다음과 긷미 수정할 수 있
다. 이때 P는 어느 행 어느 열이나 단 하나의 원소가 1이고 다른 모튼 원소가 0인 정방행렬인 치환행렬
(permutation m毗퍼이다．
LU= PA

(8.16)

부분 피버팅을 이용하여 행렬 L과U를 구하는과정에서 절댓값이 가장큰 피벗 원소를 선택하려면 행의 자
리 바꿈이 필요하다. 그러므로 반드시 상수 벡터 C의 자리 바꿈을 실행한 다음 변수 벡터 x를구해야한다．
치환행렬 P를 선형 시스템 Ax = 四］적용하면 다음과 같다．
PAx= Pc= d

(8.17)

치환행렬 P의 가장 기본적인 형태는 단위행렬과 같다．
행렬 L과 U를 구하는 과정에서 자리 바꿈을 두 번 했다고 가정해보자. 만약 첫 번째 자리 바꿈에서 1행과
3행을 바꾸고 두 번째 자리 바꿈어］서 2행과 3행을 바꿨다면 최종 치환행렬은 각각의 치환행렬을 곱한 결
과인 다음과 같은 형태가 된다．
CHAPTE日05. 수치해석

163

'1 0 0 "0 0
P = P2Pi = 0

0

0

1

1

0 0

0

1 0 0

1 0 0

0 1 0

0 1

1 0

1

자리 바꿈을 적용한새로운상수 벡터 d를 식 (8.13）과식 (8.14）에 적용한다．
LUx = d
(8.18)

Ly = d
Ux = y
1 예제 8- 11 I
부분 피버팅을 이용한 상하행렬 분해로 다음 선형 시스템의 변수 벡터 x를 구하라．

6
工2

7

3

工3

20

l

工4-

-75-

-2

풀이

>> 4=11 5 -1 6;2 나 1 -2;-1 4 -1 3;3 -7 -2 I] ; 0
>> [LU. 叩Iu(劤 0
>> c=[ 1먀7;211;-佰］;

>> dP.c 0
d =
病 四 7 如

>> y늬－加 0
y =
小75 0口00
44, 0000
35 0000
7 2727

>> X=UlIty 0

2. 0口00
10 , 0000
3 口口00
5. 0000

그림 予］] 부분 피버팅을 이용한 상하행렬 분하1 실행 결과

1 64

PART 03. MAT녀B활용하기

19 '

0 선형 시스템의 계수행렬 A를 지정한다．
Olu 함수로 가우스 소거법을 이용한상하행렬 분해를 실행한다．
0 Pc= d이므로 d를 구하기 위해 P와C를곱한다．
0 Ly = d이므로 y를 구하기 위해 왼쪽 나눗셈을 한다．
0 Ux= y이므로 x를구하기 위해 왼쪽 나눗셈을 한다．

CHAPTER 08. 수치해석

165

LESSON

07

테일러 급수

MATLAB에서 심벌릭 툴박스를 이용하여 테일러 급수 전개를 실행해보자．
1 테일러 급수 1 테일러 정리 I taylor I

Keyword

I

테일러 급수

테일러 급수는 한 점에서 미분 가능한 함수를 계산하여 무한한 합으로 표현되는 다항식 형태로 근사시키
는 방법이다. 이때 특정 조건을 만족하는 임의의 함수가 테일러 급수로 표현되면 이를 테일러 정리라고
한다．
테일러 정리는 평균값 정리를 임의의 n차佃rder) 도함수에 일반화한 형태로 전개된다．
m
rr 1=1J

'

(X

rnn / \

/
已1
.

(qJ

=

y

/（工）

/7 1

口）"

i 예처18-12 I
심벌릭 툴박스를 이용하여 함수 只功의 테일러 급수를 전개한 결과를 처음 3711 항까지 나타내라. 이때 口 = 0
이라고 가정한다．

；涵

／仁）= e노呵x)

지식

'

taylor

심벌릭툴박스어써 테일러급수를계산하는taylor함수의 기본형태는다음과같다．

tay佃r(f, 'Expan섧onP아nt', a! 勺rde已 n)
. f: 테일러 급수를 적용할 함수
· a: 工＝口에서 평가되는 값
- 'Order之 테일러 급수의 항을 정의
· n: 함수／에 의해 정의되는 테일러 급수의 처음 刃니 항

166

PART03. M月ILAB활용하기

Comlmand Window
syrus

0

（兮

'> f=exp(rr)*sin(x) 0
->

풀이

f
日xp(x）士引riCe)
>> taylor(t, Order ' , 3) 0

X坦* x

그림 8-12 테일러 급수 전개하71 실행 결과

0 syms 명령어를 이용하여 이후에 사용할 변수를 지정한다．
0 함수八刃를 지정한다．
0n= 3을 지정하여 처음3개 항을 나타낸다. 그러나샹수항을 구하는 과정에서 e0 sin(이 = 0이 되는부분
이 생략되므로［그림 平12］에는 2개 항의 결과만 나타난다．

CHAPTER 08. 수치해석

167

LESSON

08

테일러 다항식의 근삿값과 오차

테일러 정리를 좀 더 일반화하면 테일러 다항식의 근삿값을 구할 수 있다. 또한 구하려는 함수／仁）의 실젯값과 근사시켜서 찾
아낸 테일러 다항식의 근삿값 차이를 테일러 다항식의 오차라고 한다． MATLAB에서 테일러 다항식의 근삿값과 오차를 구해
보자．
Keyword

I

1 테일러 다항식의 근삿값 1 테일러 다항식의 오차 { abs 1 max 1

테잎러 다항식의 근삿값

나i兀／ 1工＝口

' . . 1(d2f \

U) 十 :1

中1=

1

. ',

（兀 -

乙＼ (ite / 工＝口

'. 2 .

U)

. 1 (dkf

十 ' " 十；기 11i1

凡！\arj

1

"+

·

·

.

+Rn

/'

（兀 -

a)

r. . . (df\

1

. .

/ （兀) = ./ (LU) 十 I- 中 I '

(x

함수／
（工）를 전개하여 工＝口 근처에서 다음과같이 나타낼 수 있다면 테일러 정리라고 한다．

(8.19)
식 (8.19）를 좀 더 일반화한 것을 테일러 다항식의 근삿값（approximation）이라고 하며 다음과 같이
나타낸다. 이때 마지막항凡은함수只功 나머지 항의 미분이라고한다．

加）=／回m的寸小1f如冷可卄＋勻如冷놔卜．.+R
乙

凡!

(8.20)

일반적인 테일러 다항식의 근삿값은

.(: - a) f(4)(a)
.(: - a)2f (a) +... +Jp,(x) = f(a) + (x - a)f'(a) +J2!
fl!

(8.21)

또는 다음과 같이 쓸 수 있다．

pn呼客 (x-3刃"'（미
工가口어］근접할 때 식 (8.20）과식 (8.21）을 비교하면 只功 七川刃이다．

168

PART03. M月TLA8활용하71

(8.22)

1 예제 8中13 1
工 = 0인 점에서 함수 只工沁카 대한 선형 및 2차 테일러 다항식의 근삿값을 구하고．MAT녀B을 이용하여 그래
프를 그려라. 이때

] .0 드 工 < 1.001고 工 값은 0.1씩 증가한다．

f (x)

eX

（今．

Command Window
>> a＝니 .5:0. 1 : ] 口；
)> fa=exp(x) ;

>> 미＝1,x; 0
'> p2=p1+x. '2/2; e
>> pIot (x, tx, -r ‘』x,pl, ' --g‘』x』p2, ' -.b' ); e

'> 1egend( ' fX " , 'P1 ' , 'P2' 』 " L0Cat 比n " , ‘卜向rtrmeSt ' ) ;
>> 비abel ( 'Equal Spaced P이 吐可 ) ;
>> 미abelC 'Eva山at ion Va山es ') ;
>> grid;
그림 8叫13 테일러 다항식의 근삿값 구하71 코딩 결과

of （工）의 선형 테일러 다항식의 근삿값을 지정한다．
0 f (x)의 2차 테일러 다항식의 근삿값을 지정한다．
of仁）와 선형 테일러 다항식의 근삿값, 2차 테일러 다항식의 근삿값을 그린다．
Fi陌

日址

v咐

If巧aft

To아5

r沌5姓op

!

W耐J牡

：그 -i d 由j 侖 曳 曳 助 自몇 d 기 目 口 圖

1口

3
f乂

1누
-

-

- p1
p2
/i

2.5
1
U
人
1
mm고m> 도니二m므m＞ 山

2

，』7';

/

,,／」／＞乙1

.,/‘夕

///

J戶／/

0.5 如二二二二才f"

0
-1

풀이

=

也8

.0.6

.0.4

.0.2
0
02
0.4
Eau川 Soaq叱 P아nts

0.6

0.8

1

그림 8-14 f仁）와 비교하여 그린 선형 테일러 다항식과 2차 테일러 다항식의 근삿값 그래프

그래프를 통해2차 테일러 다항식의 근삿값 곡선이 선형 테일러 다항식의 근삿값 곡선보다 구하려는 함숫값
어］ 더욱 가까운 것을 알 수 있다. 그러나 구하려는 함수와완전히 중첩되지 않고 일정한틈새가 있는데, 이를
테일러 다항식과 구하려는 함수 사이의 오차라고 한다．

CHAPTER 08. 수치해석

169

I

테일러 다항식의 오차

실제 함수只기와 테일러 다항식의 근삿값 pn（工）를工＝口에서 근사시킨 결과와의 오차를 구하는 공식은
다음과같다．

(x) - p, (x)
= - +a)'1)! ' j (n+l)(ci)
R, (x) = f
(:)=/(:)1끄
(:)=(x
(n

(8.23)

식 (8.23）은식 (8.20）의 나머지 항과같으며, 점 cx는x와口 사이에 있을때만그값을알수 있다．

1 예저18-14 I
［그림 8-1引의 코딩 결과를 이용하여 선형 테일러 다항식의 근삿값과 2차 테일러 다항식의 근삿값의 절대
오차 최댓값을 계산하라．

；而
지식

' abs
절대 오차를 구하려면 실젯값어써 계산 결과를 뺀 값의 절댓값을 구해야 한다. 이때 x의 절댓값을 계산하는
abs 함수의 기본 형태는 다음과 같다．

abs（川
1max
테일러 다항식의 절대 오차 최댓값을 구하는 과정어弘I 행렬 A 각 열의 원소 중 최댓값을 찾는 max 함수의
기본 형태는 다음과 같다．

>> format long
>> i1=max
(af如十xp

풀이

(x)

max(A)

))

口1 =
0. 기 82B182845J川6

>> m2＝口a蜘bs (p2七op(x))) 0
口2

11. 218281a즈345l舛8
그림 小］5 테일러 다항식의 근삿값의 절대 오차 최댓값 구하기 실행 결과

0 abs 명령어를 이용하여 只功와 선형 테일러 다항식의 근삿값의 절대 오차를 구한 후, max 명령어를 이
용하여 절대 오차의 최댓값을 구한다．
0 abs 명령어를 이용하여 只功와2차 테일러 다항식의 근삿값의 절대 오차를 구한후, max 명령어를 이용
하여 절대 오차의 최댓값을 구한다．

170

PART03. MAT냐＼B활용하71

선형 보간법과 스플라인 보간법
보간법（내삽법）은 측정이나 실험으로 얻은 자료점 사이에 위치한 자료점의 평균을 추정하는 것이다. 이는 주어진 자료점을 다
항식과 같은 형태로 표준화하는 데 유용하므로 수치해석에서 자주 이용된다. MATLAB에서 선형 보간법과 스플라인 보간법율
사용하여 자료점의 평균을 구해보자．
Key니,ord

1 선형 보긴뼙 1 interpi I interp2 1 스푤라인보간법 1 s'川ne I

선형 보간법

I

선형 보간법은 2차원 그래프상의 양 끝 값만 주어졌을 때 그 샤이어］위치한 임의의 값을 계산하는 것을 말
한다. 주어진 자료점이 여러 개 존재하더라도 선형 보간법을 이용하여 임의의 값을 추정하는 경우에는 2개1
의 자료점만 필요하다．

1 예저18-151
화학물에서 발생하는 거품 반응을 화학적 센서를 통하1 전력으로 변환하여 측정하려고 한다. 거품 발생 후 30
초부터 4분까지 전력을 측정한 결과는 다음 표와 같다．
표 8너 시간 변화에 따른 전력 발생 측정
시간

30초

］분

］분 30초

2분 30초

3분

4분

전력（pW)

110

270

350

260

200

150

선형 보간법을 이용하여 2분 경과 후, 3분 30초 경과 후 발생하는 전력을 각각 추정하고 그 결과를 그래프로

지식

'

interpi

；而

나타내라．

변수가하나인함수를보간할때나｝용하는恤帥）l 채＝의 기본형태는다음과같다．

interpi (x,y,x_int)
· X: 독립변수 자료점
· y: 工 값에 따라 달라지는 자료점
·x mnt: 추정하려는 의존변수y 긺뻬 상응하는 工 값

CHAPTER 08 수치해석

171

1interp2
변수가2개인 함수z =f（工，y）의 工＝차와y =yi어］대한 변수z를추정하려면 in佃꾸2 함수를사용한다. 변
수가2개인 함수를 보간할 때 사용하는in自p2 함수의 기본 형태는 다음과 같다．

in扼rp2似,y,z,xJnt,y_int)
·x, y: 독립변수 자료점
·z: 工. y 값에 따라 달라지는 자료점
·xJnt, y_int: 추정하려는 으죤변수z 값에 상응하는工, y 값

풀이

4\

CcmrT1,카기d 년기n｝그1

.

>> x=L0. 5 1, I .5, 2.53, 41; 0
>> y=1110, 270. 缸 . 呱）. aL. 1印］;
>> n_ m t타乙3. 51 ;

>> yi interpl(x,y,n_mnt) 0
y1=
305

175

,

'

x_

'

o'

' :
Int, yl.
);
" xlabel ( 'Time(min) );
>> ylabel ( 'Power (,icro 甘 ) );
>) axms(10.5 4 50 4［刃1) ;
y,

>) plot (x,

0

그림 8너6 선형 보간법으로 값 추정하기 코딩 결과

0 선형 보간법을 사용하기 위한자료점을 지정한다．
0 interpi 함수를 이용하여 임의의 값을 추정한다．
0 선형 보갼법을 이용하여 구한 값을 그래프어］나타낸다．
下如

帥t

V由w

亡그 ka 日 白 自

lnse作

To이5

De帥0야｝

Win山刻

He巾

1

'\ =\ 4나 白 七J-; , 昆 口 圓 困 口1

啣
跏
却
枷

小르口b山E亡m主乙n

m

그림 小17 선형 보간법으로 값 추정하기 실행 결과

전체 시간어써 측정된 각칵의 자료점을 연결한 것은 점선으로, 추정된 값은 작은 원으로 표시된다．

172

PA日T 03. MA11,AB활용하기

I

스플라인 보간법

스플라인 보간법은 고차 다항식의 단점을 보완하기 위해 인접한 자료점의 각 쌍 사이에 저차 다항식을 사
용하여 자료점을 맞추는 것을 말한다. 이는 주어진 자료점을 통과하는 부드러운 곡선을 그릴 수 있다는
것이 장점이다．

1 예제 8叫161
［예제 哥］5］의 ［표 8-1］을 이용하여 2분 경과 후, 3분 30초 경과 후 발생하는 전력을 각각 스플라인 보간

지식

'

spline

；而

법으로 추정하고 결과를 그래프로 나타내라．

sp恤IC 함수는 인접한자료점의 각쌍을 더 세밀하게 추정하여 interpi, interp2 함수보다곡선 모양의 그래
프를 그릴 수 있기 때문어］일반적으로 3차 다항식에 많이 사용된다．
스플라인 보간법을 실행하는 spline 함수의 기본 형태는 다음과같다．

y_int = spline(x,y,xJnt)
· X: 독립변수 자료점
· y: 工 값에 따라 달라지는 차료점
· 凡int: 추정하려는 의존변수y 긺뻬 상응하는 工 값

Command Window

)) o=]D.5, 1 l .5,2. 5, 3, 41 ; 0

x_

y,

(oy,

>> y=[110, 270, 3SO, 2印.200. 1 50] ;
)> x.Jnt=I0.5:0,01:41;
>> y_ intspI Ine
t (n y, 。
int) ;inty_Int) ;<)
>> pl。
,x,

풀이

,x_

>> xlabel ( 'Time(min) ') ;
>> 미abel (Po밖er (micr口 11) ) ;
>> axis([0. 5 4 印 400] );

그림 &너8 스풀라인 보간법으로 값 추정하기 코딩 결과

0 스플라인 보간법을 사용하기 위한 자료점을 지정한다．
0 spline 함수를 이용하여 임의의 값을추정한다．
0 스플라인 보간법을 이용하여 구한 값을 그래프에 나타낸다．

CHAPTER 08. 수치해석

173

File

Ed吐

＼기ew

：그 (3 a 方

Insert

臣

初口In ［油It따1

WIT啣

1

14러p

' \ '\ 抑 @ 唯｝ / 니 目 口 匡그 口 口

400

350
聊
卿
聊

小르으으EV뇨立쿄

100

.5

。'

50

1

1.5

2

2石

3

3.5

4

Tlme(min)

그림 8너9 스플라인 보간법으로 값 추정하기 실행 결과

spline 함수를 이용하여 좀 더 정밀하게 의존변수y의 값을 추정할 수 있다. interpi 함수나 in把rp2 함수를
사용한 경우보다 spline 함수를 사용한 경우 곡선의 자료점이 실젯값에 접근할 가능성이 높다는 것을 알
수 있다．

174

PART03. M戶TLAB활용하71

LESSON

10

함수의 근 구하기

두 미지수 工와V를 포함한 선형방정식에서 출력변수y의 좌표는 독립적 입력변수 工（게 따라（工미로 형성되며, 2차원 평면에
직선으로 나타난다. 只x) = 0을 만족하는 .r 값의 집합을 근이라 하고, 근은 그래프가 工축과 만나는 .r좌표Cr절편）로 나타낼 수
있다. MATLAB의 함수를 이용하여 함수의 근을 구해보자．

Keyword

I roots I fzero I

1 예제 8- 17 I
roots 함수를 이용하여 다항식 /（功 = x4 + 7x + 10의 근을 구하라．

Ii而
지식

' roots
선형방정식의근을구하는roots함수의 기본형태는다음과같다．

ro야히이
· O: 다항식의 계숫값을 차수의 내림차순으로 나열한 배열

함수의 인자에는 내림차순으로 工 차수의 계숫값을 입력한다. 이때 계숫값이 0인 경우에도 모두 입력해야 한
다. 홀수차 실수 계수 다항식의 모든 근은 실수이며, 짝수차 다항식의 경우 대수학의 기본 정리어｝따라 모든
刃차 다항식은 중근을포함하여 n개의 복3녀＝근을 가진다．
Command Window

>> 恤毗ct=roots( il叱7. 叩 0
to_correct =
1 . 31미 + 1 .74兀i
1 .31미 느 1 74꺾｝1
1 . 3131 + J. 6170j
-13101 H 0, 6170i

>> tx_cr叩g=roato(I1, 7,l叩 0
tx_ crane =

：三

풀이

그림 +20 선형방정식의 근 구하기 실행 결과

0 roots 함수를 이용하여 4차다항식 ／仁）= 工4 +7工＋10의 근4개를구한다．
Or어說S 함수를 이용할때 계숫값이 0인 항을 입력하지 않으면 2차다항식 ／仁）= 工2 +7工＋10이 되므로
주의한다. 工3 항과寸 항의 계수가 0이므로 수학적으로는 다항식에 해당하지 않지만, MATLAB에서 배
열을 입력할 때는 반드시 모두 입력해야 한다．

CHAPTER 08 수치해석

175

M-File i NA仁ero.m

1 예제 8- 181

방정식 exp(-0.2x)缸可工 + 2) = 0.1을 풀면 0 < 工 < 10에서 근이 3개이다. MAT나＼B을 이용하여 방정식의
근을 모두 구하고 그래프를 그려라．

；而
지식

' fzero
비선형방정식의 근을구하는尨町O함수의 기본형태는다음과같다．

仁er이仟unction',xO)
· 斗unction': 사용자정의함수의 이름
·x0: 근에 접근하는 값
也ero 함수는 구하려는 함수에 대한 사용자정의함수를 먼저 생성한 뒤 사용해야 한다. 단 ，사용중인 현재 폴
더에 'funct幻n.m' 이 있을 때만 이 함수를 사용할 수 있다．

풀이

12-

Efunction p = NAfzero(x)
Ly = exp（七．2*n) ，引n(X,2）七．1; 0

그림 &21 NfAfzero.m
Command W0dow

>> tzero( fIAfzero .0) e

=I

.

ann

。151

>> fzero( 'HAtoern',引

4. 5334

7. 。。66
그림 乎22 tzero 함수를 이용한 비선형방정식의 근 구하기 실행 결과

>> x=I0:0.1:10) ;

「'0
:：二：
：二二
，（
山，
，『各" ""'""七．
>> hold
Current plot held
>> 비＝zeros( I 1미）;

>> 미ot (x，미）; e

>> olabel ( 'x ');
>> 미 ab비 C y ' ) ;

그링 予23 비선형방정식 그리기 코딩 결과

176

PART03. MA凡AB활용하71

드）

0 문제에 제시된 방정식을 지정하여 사용자정의함수를 생성한다．
0 fzero 함수를 이용하여 0 근처어써 근을 찾는다．
0 fzero 함수를 이용하여 5 근처에서 근을 찾는다．
0 fzero 함수를 이용하여 9 근처에서 근을 찾는다．
0 방정식을 지정한다．
0 plot 함수를 이용하여 문제에 제시된 방정식을 그래프에 나타낸다．
0 工축을표시하기 위해 y= O을그래프로 나타낸다．
F甘e

日甘t

碼떼

口奴

r地幽加p

Wn刈

H帥）

1

그림 +24 비선형방정식 그리기 실행 결과

CHAPTER 08; 수치해석

177

LESSON

11

함수의 근을 구하는 다양한 방법

5차 이상인 비선형방정식의 근을 구하기란 쉽지 않다. 따라서 수치해석에서는 근삿값과 관련된 오차 해석을 이용하여 다양하
7目 근을 구한다．이분법, 뉴턴법, 할선법, 가위치법을 실행하는 MATLAB의 사용자정의함수를 이용하여 함수의 근을 구해보자．
Keyword

1 이분법 I bisect i 뉴턴법 I newton I 할선법 1 secant 1 가위치법 1 reg내a l

이분법

I

이분법 (bisection method）은 반복법 (iterative n妃小（Dd）을 기초로 하여 반복적으로 근삿값을 구하여
정확한 값을 계산한다. 또한 범위가 정해진 구간을 항상 반으로 나누어 근을 검색한다．
만약주어진 구간어］서 함수의 부호가 (+）에서 G）로 또는 (-）에서 (+）로 바뀌면 이 구간 내에 근이 있
다는 의미로, 이 구간의 중앙값을 이용하여 함숫값을 계산한다．

1예제8-191

M-File I bisect.m

비선형방정식 /(x) = 工3 ＋工- 7이 구간 [1. 2］에 놓여 있을 때, MAT녀B에서 여섯 번의 이분법으로 근을

지식

'

벼sect

；而

구하라. 편의를 위해 모든 결과는 소수점 아래1 네 자리까지 나타내라．

이분법을실행하기 위한사용자정의함수bisect의 기본형태는다음과같다．

bisect佃由戶rror,n,inde지
· a: 구간의 상한값
· b: 구간의 하한값
. error: 허용 오차
. n: 반복 횟수
· index: 사용자정의함수에서 함수只x)를 지정한 색인

단, 사용중인 현재 폴더에 'bisect.m'이 있을 때만 이 함수를 사용할수 있다．

178

PART03. MATLAB 활용하기

풀이

>>bisect (l, 2, 1 .I:f- 6,6, 1)
iteration =
1 .11111

1 .11111

2.11111

1 .니llI

-2,12刃

0.니LIl

1．印LU

2.11133

1．石［13

0. 1014

0．有13

1．印［13

1．石（刃

1．田印

+1 .［月町｝

0.1珂

I .}i시I

1. 1늬Ui

1 . 너了凸

七．묘ru1

o. n｛耳1

1 . tif月）

I 1/i乂JJ

1 .7!咬｝

七J기E'-l

0.13引3

1 .7!田

1 . '／났JJ

1 .7344

七．04田

0.0!댜；

iteration =
2. 0133

iteration =
3．미I工

iteration =
4.11111

iteration =
5.11111

iteration =
6.11111

그림 小25 이분법을 이용한 근 찾71 실행 결과

이분법으로 근을 구하기 위해 bisect 함수를 이용한다. bisect 함수의 결과는 6열로 표현되는데, 이는 각칵 72,
a, b, c, f (c) , 所C를나타낸다. 다음출력을보려면 回田 키를눌러야한다．

I 뉴턴법
뉴턴법 (Newt（끄l n妃thod）은 비선형방정식의 근을 결정할 때 사용한다. 먼저 주어진 구간 ［口, b］에서
함수／O）가 미분 가능하고, 구간 내에 함수의 해도 포함되어 있다고 가정한다. 이때 미분을 이용한 접선
으로 수렴해가는 방법을 사용하면 처음 해 却를 추정할 수 있다．

1 예제 小20 I

M-File I newton.m

비선형방정식 /（工） = 工3 ＋工- 7이 구간 [1, 2］에 놓여 있다. 처음 시직h하는 값工0= 1.5000일 때, MAT나＼B
에서 뉴턴법을 사용하여 반복적으로 치 工2 . 工3을 구하라. 편의를 위해 모든 결과는 소수점 아래 네 자리까지
나타내라．

CHAPTER 08. 수치해석

179

.

배경

지식

nofl,
"

뇨 "

nt,

' U "

뉴턴법을실행하기 위한사용자정의함수newton의 기본형태는다음과같다．

new如n(xO戶作or,n,inde지
· xO: 초71 추정값
· error: 허용 오차
· n: 반복 횟수
· index: 사용자정의함수에서 함수只x)를 지정한 색인

단, 사용중인 현재 폴더어］'new的n.m'이 있을 때만 이 함수를사용할수 있다．
Command Window

풀이

>> ne,ton(1.5, I .1七,6, l) ;
iteration =
0

1 .58] )

-2. 1250

7.兀11

0. 2742

1 .7742

0. 3닿9

10. 4433

-0.0344

1.7.3田

0.11臣

10.［互｝10

七Jlli;

] .73묘2

0. 口더00

10. 0745

-0. 0000

iteration =
1 .1100

iteration =
2.OX9

iteration =
3, 0끄口

ro口t =
I .7.392
그림 予26 뉴턴법을 이용한 근 찾기 실행 결과

뉴턴법으로근을구하기 위해 n이毗on 함수를 이용한다. new的n 함수의 결과가 5열로 표현되는데, 이는각
각 반복 횟수 兀 동일한 과정을 반복할 때마다 새롭게 계산되어 추정하는 각 근의 값 工刃, 輧＝어］ 斗을 대입
한 /(xv)의 결과, l차도함수에 工, 을 대입한／t工,）의 결과, 새롭게 계산된 추정값과 바로 이전 추정값의
차이인 工n m 瓦-1을 나타낸따．

I

힌선법

할선법 (secant method）은 접선으로 함수를근사시키는 뉴턴법을 기초로 이용하지만, 뉴턴법과 달리 1차
도함수 / ' 仁）의 계산이 필요 없는 유용한 방법이다. 그래프싱어］있는 두 점을 연결하여 생긴 직선을 할선
이라하고, 이 할선을통해 그래프를근사시킨다．

180

PART 03. MATL4B활용하기

M-File I secant.m

1 예제 小21 1

11

비선형방정식 ／仁）= 工3 ＋工小 7이 구간 [1. 2］에 놓여 있을 때, MAT녀B에서 할선법을 사용하여 반복적으

H而

로初, 工l, 工2. 工3 , 工4를 구하라. 편의를 위해 모든 결과는 소수점 아래 네 자리까지 나타내라．

지식

' secant
할선법을실행하기 위한사용자정의함수secant의 기본형태는다음과같다．

secant似0,川尸作or,n,inde지
· xO, xl: 초71 추정값
· error: 허용 오차
· n: 반복 횟수
· index: 사용자정의함수에서 함수／b）를 지정한 색인

단, 사용중인 현재 폴더어｝ 'secant.m'이 있을 때만 이 함수를사용할수 있다．

풀이

C아Or?治nd 쌔ndow
>> secarit (2, 1 ,l .0e七, 6 . l)
terat ion =
1 , 0000

1 . 0000

-5. 0000

0. 6250

1 .5260

-1.0840

0. 1730

] 7950

口6山5

-0. 0523

1 . 7367

-0. 0366

0. 0034

1 . 7391

-0. 0011

0. 0001

1 . 7392

0. 0000

-0. 0000

iteration =
2. 0000

iteration =
3 001J0

iteration =
4. 0口口0

iteration =
5. 0000

t日rat ion =
巳0000

그림 小27 할선법을 이용한 근 찾2I 실행 결과

할선법으로 근을 구하기 위해 secant 함수를 이용한다. secant 함수의 결과가 4열로 표현되는뎨, 이는 각
각 반복 횟수 兀 동일한 과정을 반복할 때마다 새롭게 계산되어 추정하는 각 근의 값 Xe , 함수어나.을 대입
한／似n) 의 결과 새롭게 계산된 추정값과바로 이전 추정값의 차이인 xn+I -x.을 나타낸다．

CHAPTER 08. 수치해석

181

I

가위치법

가위치법 (regula falsi method, false叩ositi이. method）은 이분법을 수정한 형태로, 주어진 구간의
폭을 반복적으로 좁히면서 정확한 근을 구하지 않고, 반복어］ 의해 새롭게 설정되는 구간의 끝점을 직선으
로 연결하고 절편의 위치를 결정하여 다음 근을 추정해나가는 방법이다. 그러므로 이 방법을 사용하면 함
수／仁）가주어진 구간 내에서 근을포함하고 있을 때 반복적으로 미리 결정된 근의 값을수행한다．
M-File 1 regula.m, NAregulam

1 예제 小22 I

비선형방정식 /（工）= 工3_ 4工 + 1이 구간 [1. 2］에 놓여 있을 때, MATHAB에서 가위치법을 사용하여 반복
적으로 나타나는 근을 구하라. 모든 결과는 실제 근과 같은 값이 나올 때까지 반복하여 계산하고, MATL/＼日
의 출력 명령에 幻rmat long을 이용하여 나타내라，

而梱

1regula
가위치법을 실행하기 위한사용자정의함수regula의 기본 형태는 다음과같다．

regula('F1',I,r,error,n)
· 'Fl': 함수에 대한 사용자정의함수 이롬
· 1: 초7뻬 지정한 왼쪽 끝점
, r: 초기에 지정한 오른쪽 끝점
· error: 허용 오차
· n: 반복 횟수

단, 사용중인 현재 폴더에 'NAregula.m과
' 있을 때만 이 함수를 사용할수 있다．
' 'regula.m이

폴이

UN如e申뇨m 可 爭’

二： 민，":'，“므；
二객，A.reguI' (" )

그림 小羽 N匈的ub.m
4)

C口rnma口＝ 1 .
>> format long

Iteration =

熙

>> tlterationl=regula( 'NAregula .l .2je- 08.20)

.旺m표幽44町

그림 8-囚 가위치법을 이용한 근 찾71 실행 결과

182

PART 03. M/ TLAB 활용하71

가위치법을 사용하여 근을 구하기 위해 regula 함수를 이용한다. regula 함수의 첫 번째 인자NAregula는
함수／仁）에 대한사용자정의함수의 이름, 1과2는 처음에 지정한 왼쪽끝점과오른쪽끝점, i0'8은 허용
오차，20은 반복 횟수를 나타닌拉干. 사용자정의함수 NAregula는 regula 함수에서 호출할 수 있다. 20회 반
복 실행을 지정했지만 열한 번째 계산 결과가 실제 근과 비교하여 혀용 오차 10出보다 작은 범위이기 때문에
열한 번째 계산까지만표시된다.

CHAP在A 08. 수치해석

183

LESSON

12

수치 적분법

복잡한 적분방정식을 정확히 계신하7는 어려우므로 수치해석적으로 적분의 근삿값을 구할 수 있는 사다리꼴 적분법, 심슨 적
분법, 가우스 구적법, 롬버그 적분 등을 사용한다. MATLAB의 함수를 이용하여 실제 적분값에 근사시키는 방법을 알아보자．
Keyword

I 사다리꼴 적분법 I trapz I 심슨 적분법 I simpson I 가우스구적법 I quad I qua네 1
1 mnt I 롬버그 적분 I romberg I

I

사다리꼴 적분법

사다리꼴（trapez아dal) 적분법은수평 바닥면과2개의 끝점 口, b를 연결하는 경사진 윗면을 가진 사다리
꼴 면적을 근사시키는 방법이다．

1 예저18-23 I

H而

지식

力亡이다．

는 力＝

{,

MAT녀B에서 사다리꼴 적분법을 실행6는tra口z 함수를 이용하여 /.31n工（抗의 값을 구하라. 이때 간격 크71

' trapz
사다리꼴적분법을실행하기 위한trapz함수의 기본형태는다음과같다．

trapz似肛）
· X: 부분 구간에 있는 자료점의 배열
· fx: 피적분함수

풀이

』

>> T4놔rapz

(xl

>> x1
toraat.
11nspace
long(l 3. 5) ;
>> fx1=log(Xl) ;
fxl)

0

0

T4 =
1 2821 045824羽1印

>> x2=1 inspace(1.39); 0
>> 似2＝比叭x2) ;

>, T8=trapz(x2, fx2) 0
TO =
1 .202374얹l好［E1凹

그림 +30 사다리꼴 적분법을 이용한 적분 실행 결과

184

PART 03. MATLAB활용하기

0 소수점 자리를 확장하기 위해 form毗long을 설정한다．
0 간격 力 근에대해血恥鉀수를사용한결괴를蛔녀정한다．
乙

0 如呻수를이용햐뇌 간격 方 그．일때사다리꼴적분법을적용한다．
乙

<1

<) 간격 方 그蛔枷螂四힘수를사용한李昏쪄 지정한다．

(1

0 卿啼수를이용햐여 간격 方 그일때사다리꼴적분법을적용한다．

I 심슨 적분법
심슨（Sir叩son) 적분법은 사다리꼴 적분법을 확장하여 2차 다항식어］대한 피적분함수를 근사시키는 방
법이다. 사다리꼴 적분법에서는 간격 크키를 줄이고 부분 구간의 수를 증가시켜 1차 다항식으로 그리는
직선이 점점 함수只功의 곡선 형태와 겹치도록 근사되었지만 여전히 매끄럽지 않다. 이때 자료점 3개를
이용하는 2차 보간법을 사용하면 2차 보간 다항식을 얻을 수 있고, 2차 다항식은 포물선 형태이므로 함
수只x) 에 좀 더 매끄럽게 겹쳐질 수 있다．

1 예저I 8- 24 I

M-File I simpson.m

지식

力亡이다．

'

Simpson

；而

는 方＝

{,

MATLAB에서 심슨적분법을실행O는引mpson 함수를이용弓K겨 /’노！
方의 값을구하라. 0빼 간격 크71

심슨적분법을실행하기 위한誼npson함수의 기본형태는다음과같다．

帥iipson (f,a缸n)
· f: 피적분함수
· a: 전체 구간의 시작점
· b: 전체 구간의 끝점
· n: 부분구간의 수

단, 사용중인현재 폴더에 'simpson.m이
' 있을때만이 함수를사용할수 있다．

CHAPTER 08. 수치해석

185

Command Window

풀하

>> format

moo;

<1
e.

(x)

>> f (x) Iog
;
>> S4=8i .psQn(t l. 3.4) 시
-

S4=
] .囚5321타爻忍梵213
>> 田＝Si口pson( in니rae ( I i四나T) ,L3』
日） C
SB =
1 .師准好4또爻il拓7

그림 小31 심슨 적분법을 이용한 적분 실행 결과

0 소수점 자리를 확장하기 위해 form毗long을 설정한다．

三일때심슨적분법을적용한결괴를S4에지정한다1

力：
三일때심슨적분법을적용한결괴를S8에지정한다戶］

0

simpson힘수를이용8뼈간격

0

simpson힘수를이용3뼈간격方＝

e @ 仕）를 사용하면 함수의 변수工를 벡터 형태로 미리 지정할 필요가 없다．

리힘수를

정의하지 않은 경우, 필요할 때마다즉시 처리하는 inline 함수에 작은따옴표를 붙여 사용할수 있다．

I

가우스 구적법

7牌스 구적법 (Gauss（和adrature）은 적분의 영역 내 지정된 점에서 함수의 값을 가중치 (weight) 합으
로 표시하여 적분하는 방법이다. 자료점의 간격이 균일한 경우 가우스 구적법이 항상 좋은 결과를 제공하
지는 않지만, 자료점의 간격이 균일해야한다는 제한이 없을 때는싱당히 좋은 결과를 얻을수 있다．

1 예제 8叫25 1
MATLAB에서 가우스구적법을실흔茹陪quad 함수와qua비 함수를이용弓K겨 /,'！노x赤의 값을구하라．
；而

'quad, quad!

지식

quad함수와quad! 함수는모두가우스구적법을실행한다. quad함수는심슨적분법을기초로하고quad!
함수는 로바토 적분 알고리즘을 기초로 적용한다. quad 함수와quadi 함수의 기본 형태는다음과같다．

quad('f(x)',a,b)
quadl('f(x)',a,b)
· 1f(X)1: 피적분함수
· a: 적분의 하한값
· b: 적분의 상한값

186

PART03. MA凡AS활용하'I

Command Window

1,

,

)

'

*Icg

(x)

;rq

>> thriat,
jadquad
.I (inhine

5\.

(a.

풀이

6)

0

（뇨ad =
23 묘기 67047宬표X끄4
>> kjalL콕uadI (inh ine(x. *log(x) L1.6) 0
山alL =
23. 3引町0446IIi23
그림 +32 가우스 구적법을 이용한 적분 실행 결과

0 소수점 자리를확장하기 위해 format long을 설정한다．
0 quad 함수를 이용하여 심슨 적분법을 기초로 한 가우스구적법을 적용한 결과를Quad어］지정한다．
0 quad! 함수를 이용하여 로바토 적분 알고리즘을 기초로 한 가우스 구적법을 적용한 결과를 QuadL에 지

23.501670446104988이다
.

quad함수를／

노！

실제로적분을실행하면／,'！

赤=

정한다．

陪한경우의 절대오차

는 3.2755 x 10-8이고, quad! 함수를 사용한 경우의 절대 오차는 5.5280 xm쩌다. 그러므로 quad보다
quad!을 사용했을 빼1 실젯값혀江1 가깝다．

1 예제 8- 26 I
l1HH11HH1＝

口

지식

'

mnt

；涵

MATbAB의 심벌릭 툴박스에서 저1공하는nt 함수를 이용弓K겨／6xln：赤의 값을구하라．

적분의 하한값이 口이고, 상한값이 b인 피적분함수／似）에 대한mt 함수의 기본 형태는 다음과같다．

in布써,a力）
· 肛）: 피적분함수
· a: 적분의 하한값
· b: 적분의 상한값

CHAPTER 08; 수치해석

187

Command＼사inth）나
>> t 口 mmat
)> syrns P1

풀이

9

.> lntegral=int (x. .Iog(xLl, 6) 0

Integral =

18*log(6) - 35m e
>> Re a 1=1小log(6)-弱／4 e
Real =
23 . 501 5704451 04988

그림 +33 m)t 함수를 이용한 적분 실행 결과

Oii式 함수를 이용하여 적분을 계산한다. 이때 mt 함수의 인자로 피적분함수／仁）= 工in工, 적분의 하한값
l과상한값6을 각각 지정한다．
0 심벌릭 툴박스를이용하면 적분의 斗산과정을문자열로표시하기 때문에 恪 牛 log(6) - 35/ 4로출력된다．
0 적분결괴를숫자로변환하면실제 적분값은／'！노xdx = 23.501670446104988이다．

I

롬버그 적분

롬버그（Romberg) 적분은 적분을 계산하기 위한 사다리꼴 공식어］ 리차드슨 외삽（Richardson extrapolation) 공식을 이용하는 방법이다. 이 방법을 사용하면 실제 오차를 감소시켜 실젯값어］가까운 근삿
값을 구할수 있다．

1 예제 8- 27 1

M-File

romberg.m

MATLAB의 롬버그 적분을 이용하여 각각 ]711. 2개, 4개로 나누어진 부분구긴뻬 대한／
。
,'sinirx赤를 실행

；而

하라．

지식

'

romberg

롬버그적분을실행하기 위한romberg함수의 기본형태는다음과같다．

romberg(f（지a缸n)
· f(x): 피적분함수
· a: 적분의 하한값
· b: 적분의 상한값
· n: 외삽 횟수

단，사용증인 현재 폴더어］'rot油erg.m'이 있을 때만 이 함수를 사용할수 있다．

188

PART03. M月TLAB활용하71

풀이

Command Window
)) 1ormat 1 1H크 ;

>> lntegraI=romberg(inl ine( sin(pi*a) )』01,2) 0
xc =
0. 50000000000口000

xc
0. 250000000000000

0, 750000000000000

1-table 0
0 000000000000000
0. 5口Jo凹000000000 0. 田6665666666田7
0.Hr們5足月J1吐｛사4 0. 6笠｝0711 87451b日8 0, 63미64822177100
탸table
0. 1 晦；
E蚊；68666667
0. 034517700864425 山. 001 906365280598
Integral =
0. 6羚11珥a꼬17기［刃
그림 于34 롬버그 적분을 이용한 적분 실행 결과

0 roi的erg 함수를 이용하여 롬버그 적분을 적용한다. 이때 romberg 함수의 인자로 피적분함수曲l 兀兀는
加line 함수를 이용하여 지정하고, 적분의 하한값0과상한값 1, 외삽 횟수2를 지정한다．
0 卜table은구한 결과, E-table은각칵의 오차 계산, Integral은 실제 적분에 근사시킨 값을보여준다．

CHAPTER 08. 수치해석

189

LESSON

13

수치 미분법

복잡한 미분방정식을 정확히 계신하기는 매우 어려우므로 수치해석을 이용하여 복잡한 미분방정식을 계차방정식으로 선환함
으로써 좀 더 간편하게 미분값에 근사시킨 결과를 구한다. MATLA.B의 함수를 통해 수치해석적으로 미분값을 구할 수 있는 오
일러 방법과 룬게쿠타 방법을 알아보자．
i d附 I subs I （把uble i ds이ye i 룬게쿠타 방법 I ode23 I ode45 I 오일러 방법 1

Keyword

! 수정된 오일러 방법 1

I

룬게쿠타 방법

함수八／, y）의 여러 계산어］ 테일러 급수를 근사화하는 방법으로 룬게쿠타（Runge -Kutta) 방법을 이용
한다. 이는 수정된 오일러 방법보다 오차를 더 줄일 수 있다．

i 예저18- 28 I
MATLAB의 심벌릭 툴박스에서 제공하는 비卄 함수를 이용하여 함수 /(x) = 前nh(3x)cosh(5x)의 1차 미분함
수를 구하고 미분값에 工 = 0.2를 대입한 결과를 계산하라，

；而
지식

' duff
심벌릭 툴박스에서 제공하는미분계산함수인di什함수의 기본형태는다음과같다．

d附（f凡n)
·fx: 미분하는 함수
· n: 미분함수의 차수

1subs
l차 미분함수를 구한 결과가 주어졌을 때 어떤 한 점에서의 미분값을 계산하려면 심벌릭 변수를 상숫값으로
대치해야 한다. 심벌릭 수식에서 사용 중인 심벌릭 변수를 새로운 심벌릭 변수 또는 숫자로 대치하는 S的S
함수의 기본 형태는 다음과 같다．

subs(dfx,x,a)
· dfx: 함수／
（功의 j차 미분방정식
· X: 미분 변수
· a: 변수工에 대입할 상숫값

190

PART03. MAT녀B 활용하71

1double
面uble은 상숫값을 배정밀도로 변환한다. 만일 상숫값이 이미 배정밀도 배열이면 double을 사용해도 변환
되지 않는다. 面uble 함수의 기본 형태는 다음과 같다．

dot制e（지
· X: 배정밀도값으로 변환하는 상숫값

풀이

>> for.at long;
>> sy.s x
>> dfx=iIff (sinh(3.x).cosh(5*x) l) 0
df x =
3*cosh(3소0）士cosh(5士x) + 타引nh(3*x）士引nh (5士o)
>' double(subs(dlo, x.O. 2) ) 0

9 . 22879551囚411丑5
그림 小35 d肝 함수를 이용한 미분 실행 결과

0 duff함수를 이용하여 함수只功를 미분한다. 이때 小侄함수의 인자로 함수／仁) =sm址缸）cosh(5功
와 미분함수의 차수 l을 입력한다．
O只功를 미분한（垢어］ subs 함수를 이용하여 工 = 0.2를 대입한다. subs 함수의 인자로 계산된 l차 미분방
정식 함수非, 미분 변수工, 미분 변수에 대입할상숫값0.2를 입력한다 ．만일 面uble을 사용하지 않고
subs(狐J,0.2）만사용하면 弘cosh(1）卞cosh(3/5 )+5臧nh(1)相加h（引5）의 결과를보여준다.

1 예제 8- 29 I
MAT나＼B의 심벌릭 툴박스0似 제공하는 ds이ye 함수를 이용하여 초기 조건이 v (O) =l으J 미분방정식

지식

'

ds아ye

；而

y'(t) = y(t) cos(t）의 y(O.lir) 값을 구하라．

심벌릭 툴박스에서 상미분방정식을계산하는dsolve함수의 기본형태는다음과같다．

dsolve('equation',y(O))
·equation: 상미분방정식의 심벌릭 식
,y (0): 주어진 함수의 초깃값

이때 sym, syms 명령어를 입력하지 않아도 사용가능하다．

CHAPTER 08. 수치해석

191

2개 이상의 상미분방정식을 계산하는 dsolve 함수의 기본 형태는 다음과 같다．

dso!ve('equationl ','equation2',y(O))
만일 주어진 미분방정식이 l차일 吼quation은 l차 미분방정식 y'(t)를Dy로 나타내고, 나머지 상수와 변
수는 MATLAB 기본 표기에 맞게 나타낸따. 또한 2차 미분방정식 y '(t)는D勾로 나타내고, 계속해서 미
분방정식의 차수가 3차, 4차로 증가하면 D3y, D4y로 증가시킨다. 그리고y(0）은 1차 미분방정식을 풀기
위해 주어지는 함수의 초깃값이다．

풀이

Comman그
:i
>> format 1 ong;
,, yt=dsolve( 'Dy=g*coo(t) , g(O)=1 ) <1

9

yt =
map（引n(t))

(sin

>> t=o小吐 0

>> ytexp

(t))

Pt =
1 . 田2085516四8737
그림 予36 심벌릭 푤박스에서 상미분방정식 계산하기 실행 결과

0 상미분방정식을 계산하기 위해 dsolve 함수를 사용한다．
Ot값을0.1兀로지정한다．
Ods아ye 함수를 이용하여 구한 식에 t 값을 지정한다．

1 예제 8小30 1

M- FiIe i odecos.m

0de23 함수와 0de45 함수를 이용하여 초기 조건이 y(0) =1인 미분방정식 y'(t) = cost으1 그래프를 그리
고 그 결과를 비교하라. 이때1］차 미분방정식의 실제 풀이는 y(t) = sint+1이다．

HH?j
；而
지식

'ode23, ode45
MATLAB은 다양한 간격 크기를 이용하여 룬게쿠타 공식의 구현을 돕는 'S이vers'를 제공한다. 여기서
ode23 함수는 2차와 3차 룬게쿠타 공식의 조합에 이용하고， ode45 함수는 4차와 5차 룬게쿠타 공식의 조
합어］이용한다．
ode23 함수와ode45 함수의 기본 형태는 다음과 같다．

192

PART03. MAT녀B활용하기

[t, y] = 0de23('ydot',tspan,y(O))
[t, y] = 0de45('ydot',tspan,y(O))
· 'ydot七 주어진 1차 미분방정식
·tspan: 미분 변수 r가 시작하고 끝나는 시간의 범위
·y (o): 주어진 함수의 초깃값

붚이

U 毗U丘m Xt+l
二： 就只"才，느 """""' ' 算）0
그림 乎37 odecos.m
Corr:斗

Lnj:n

忙

>>tl=10:0.01:4*pi1;
>> su뱌니ot ( 2, I, 1)
>> [t, yj=ode23(' odecos ', [O, 4.plj,I) ; 0
>> y作I.引n(tl) ;

>> 이ot(t.y. ' o',tl.yl) e

>. o1abel ( 'Time (see) ')
>> 미ab이(y (t)=I+sin(t) ')
>> axS( 10 巾P1 山石 2.51)
>> subplot (2. l, 2)
>> Lt,yl=0de45(dodecos , [0,4.p11,1) ; 0
>> y2=1s引n(tl) ;

>> plot(t,v. " o',tl, y2) 0

>> xIabe (T油日 (sec) )
>> 비ab이 (.叭t)미四in(t) ')
>> axis(10 4pI -0.5 2.51)
>) gteat (ode23') ;
)) gteat (ode46' );
그림 予羽 （너e23 함수와 ode45 함수를 이용하여 미분방정식 그리71 코딩 결과

0 문제에 주어진 함수를 입력한다．
0 ode23 함수를 이용하여 미분을 계산한다．
0 ode23 함수로 구한 결과를 그림 창 위쪽에 그린다．
0 ode45 함수를 이용하여 미분을 계산한다．
0 ode45 함수로 구한 결과를 그림 창 아래쪽에 그린다．
［그림 斗39］는 수치로 계산된 결과를 연결하여 매끄럽지 않은 곡선 형태이다. 일반적으로 ode45 함수는
ode23 함수보다 1日 빠르고 정확한 결과를 보여주지만, ode23 함수보다 간격이 더 크기 때문에 그래프의
곡선이 덜 매끄럽다．

CHAPTER 08. 수치해석

193

그림 +39 0de23 함수와 0de45 함수를 이용하여 미분방정식 그리기 실행 결과

I

오임러 방법

오일러 방법의 장점은 미분방정식의 수치적 풀이에 대해 가장 간단한 알고리즘을 제시한다는 것이다. 하
지만 시간 상수의 작은 변화에도 비교적 큰 오차가 발생한다는 단점이 있다. 따라서 시간 간격이 미분 풀
이의 정확성에 미치는 영항을 이해하는 것이 매우 중요하다. MATLAB에서는 기초 수학에서 사용하는 시
간의 증분량 사와 같은 개념으로 力를 사용한다．
오일러 방법은 다음과 긷히 정의한다．
y(tn+1) =y(t) +hf(tn,y(tn)) (n = 0,1, ·,N -1)

(8.24)

y+i =y, +hf(tn, yn) (n= 0,1, .·,N- 1)

(8.25)

1 예저I 8- 31 1

M-F朴e l e벼er.m

0초부터 l초까지 0.04초씩 시간이 증가하고 초깃값이 2인］차 미분방정식 yl' = 巧y의 해를 오일러 방법으
로 구하려고 한다. 미분방정식의 실제 풀이가 y(t) = 2eH針일 때1 실제 결과와 오일러 방법을 이용한 결과를
그래프로 비교하는 스크립트 파일 e네er.n）을 작성하고 그래프로 나타내박．

194

PART 03. MATLAB활용하기

1234567B9mn泛四

m片町J1t

풀이

-

-

「

+

1
1
4
e
느
e

h=O庶可
y(1 )=2;
0-n;
기or 小lh:h:11 0
n=n+1 ;
y(n+1 )=y (n)15士y(n）升n
end
t=tO:h:11;

1
1

::：就빠甲C

1
1
H

olabel ( 't (t 油e) ')
ylabel ( 'y(t) ')
axio(10 1 0 21) ;

그림 8-40 오일러 방법을 이용하여 舌｝1 구하기 코딩 결과佃ubr.m)

0 초깃값을 지정한다．
0 凡r문을 반복하기 위해 계수 n 의 초깃값을 0으로 지정한다. 이때 식 (8.24）를y (n+1) =y（기
-5*j'伽）功로 표현할수 있다．
0 실제 결과를 지정한다．
0 실제 결과와오일러 방법을 이용한 결과를그래프로 나타낸다．

口 t3 日 曲 1 臣 ! 聲＼ 戈 的 匈 咽 尻 , 呵 口 匡그 1 口

그림 斗41 오일러 방법을 이용하여 해 구하기 실행 결과

I

수정된 오일러 방법

오일러 방법은 수치적으로 미분방정식을 풀 때 큰 오차가 발생한다. 따라서 이러한 오차를 줄이기 위해
수정된 오일러 방법을 사용한다. 수정된 오일러 방법은 시간 간격 tn과 白＋l 에서 식 (8.24）의 오른쪽을
평균으로 치환하여 사용한다．

y(i, . ;)=y0,
y(t+1)
=y(t)+-(
)+h
f +f,+,)
乙

(8.26)

CHAPTEF극08. 수치해석

195

M..-File 1 euler edit.m

1 예저I 8- 32 I

0초부터 1초까지 0.04초씩 시간이 증가하고 초깃값이 2인 1차 미분방정식 y' = -5y의 해를 수정된 오일러
방법으로 구하려고 한다. 미분방정식의 실제 풀이가 y(t) = 2可5t일 때 실제 결과와 수정된 오일러 방법을 이
용한 결과를 그래프로 비교하는 스크립트 파일 eu厄乙的仕.m을 작성하고 그래프로 나타내라．

d
1

m止酊 甘侃rn

=

4

y (I (-2;
n=O;

e

n
< n
J

h=0. 04; 0

=

풀이

1

：으，,.;
r "多；“，「

二
U

4

八
b

m

n
/

1

y (nn1)=y(n),(h/2).(- S.y(n)-5.x(n.I ));
, end
t寸Q:h:lJ ;

8

1

口
U

e
e

1

e

9
느

e

xlabel ( 't (time) )
yIabeI ( ' y(t) )
anis(F0 1 0 21) ;

口
U

1

4

1 1 1 1 1

0

,'：『，
르；
:".}．“三씨．‘,0t) 0
1

그림 小42 수정된 오일러 방법을 이용하여 해 구하기 코딩 결과佃uler_e매.m)

0 초깃값을 지정한다．
0 for문을 반복하기 위해 계수 n의 초깃값을 0으로 지정한다. 이때 식 (8.26）을y(n+1) =y(n)日加2)
水（-5抄(n)巧斗x(n+1)）로 표현한다．
0 실제 결과를 지정한다．
0 실제 결과와수정된 오일러 방법을 이용한 결과를 그래프로 나타낸다．

그립 8-43 수정된 오일러 방법을 이용하여 하1 구하기 실행 결과

196

PART 03. MATLAB활용하기

CHAPTER

CONTENTS
LESSON 01 닫힌 루프 시스템
LESSON 02 라플라스 변환
LESS아寸 03 전달함수
LESSON 04 상태방정식
LESSON 05 시간 응답
LESSON 06 안정도
LESSON 07 근궤적
LESSON 08 주파수 응답
LESSON 09 나이퀴스트선도
LESSON 10 니콜스선도

LESSON

01

닫힌 루프 시스템1

제어（con卄이）는 입력이 제어 시스템의 구성 요소를 거쳐 목표한 출력을 얻도록 시스템을 조절하는 것을 말한다. 제어 시스템
에서는 입력과 출력 사이의 관계를 블록으로 나타내는 블록선도률 이용하여 시스템을 설명한다. MATLAB율 이용하여 오차를
수정할 수 있는 귀환을 가진 닫힌 루프 시스템에 대한 해석과 실행 과정을 살펴보자．
I 닫힌 루프 시스템 i 단위 귀환시스템 I if I feedback I step I 囹ml

Keyword

I

닫힌 루프 시스템1

닫힌 루프 시스템（c1osed-1oop system)은 입력과 출력이 일치하는지를 비교하고, 입력과 실젯값 사이
의 오차어］비례하는 신호를 다시 보내 오차를 수정하는 귀환 경로（feedback path）가 있는 제어 시스템
을 의미한다. 반면에 귀환 경로가 없어서 오차를 수정할 수 없는 제어 시스템은 열린 루프 시스템 佃pen
loop system）이라고 한다．

I

단위 귀환 시스템1

귀환 경로의 배숫값（mu川plicative V키ue）이 1인 귀환 루프를 가진 시스템을 단위 귀환 시스템 (un卿
feedback system)이라고 한다．

1 예工｛19- 1

M-File I FdSysStep.m, FdSysPara.m, FdSysRamp.m

I

다음과 같은 단위 귀환 시스템이 있다．

R(s)

耶）

G(s)

그림 9너 단위 귀환 시스털1 블록선도

198

PA딕T03. M』町냐＼B활용하기

:）이다·

,)

，“

(

4

, (, +묘
(s

=

s

는전딜함수이다· 이때전달함수G

(s)

G

출력신호의！匿라스변환，

(s）

［그림 아1酬서 匙0는 입력 신호의 라플라스 변환, 耶）=R（刃 -1如）는 오차 신호의 라플라스 변환, ）七）는

(a) 계단 입력 함수를 사용하여 닫힌 루프 응답을 그려라．
(b) 포물선 입력 함수 風t) = 0.寸 (I 加）을 人용하여 닫힌 루프 응답을 그려라．
(c) 램프 입력 함수 r (t) = t(t > 0）를 사용하여 닫힌 루프 응답을 그려라．

；而
지식

' tf
tf함수는전달함수모델을생성하는함수이다. 라플라스 변수S로표현되는유리함수를사용하여 전달함수
모델을 지정하는tf함수의 형태는 다음과 같다．

S = tf('s')

num과den을 각칵분자, 분모로 사용하는 연속시간 전달함수를 생성할 때 tf함수의 형태는 다음과같다．

sys = tf(num,den)
. sys: 전달함수
·num: 전달함수의 분자
·den: 전달함수의 분모

1 也edback
色edback 함수는 두 선형 시불변 모델의 귀환을 연결하는 함수이다. 닫힌 루프 귀환 시스템에 대한 선형 시불
변 시스템 sys를계산하는feedback 함수의 기본 형태는 다음과같다．

sys = feedback(sysl, sys2)
·sys: 닫힌 루프 시스템에 대한 선형 시불변 시스템
· Sysi: 전달함수
·sys2: 귀환 경로의 배숫값

. step
step 함수는 선형 시불변 모델의 계단 응답을 구하는 함수이다. 시뮬레이션에 사용되는 출력 웅답y와 시간
벡터 t의 값을찾을 때 step 함수의 형태는 다음과 같다．

[y,t] = step(sys)
· y: 출력 응답
· t: 시간 벡터
· SYS: 전달함수

전달함수 sys에 시간벡터 t 동안시뮬궤이션을실행한후출력 응답y를 계단응답으로 나타낼 때 step 함수
의 형태는 다음과 같다．

CHAPTER 09. 제어

199

y = step(sys,t)
동적 시스템 sys의 계단응답을그릴 때 step 함수의 형태는 다음과같다．

step(sy히

1isim
임의의 입력어］대한 선형 시불변 모델의 시뮬레이션 시간웅답（time response) y의 값을 구하는 1shi 함수
의 형태는 다음과 같다．

y = Isim(sys川t)
· y：출력행렬
·sys: 시스템 벡터
, U: 입력 함수
· t: 시긴벡터

A

PA日T 03. MATLAB활용하기

(sys)

'

111l

200

1

0 문자열이 위치할자리를클릭하면문자열이 삽입된다．

e

0 계단 입력 함수와출력 응답을 그래프로 나타낸다．

e

Hn
d
/
n

0 계단출력 옹답을 얻기 위해 step 함수를 이용한다．

e

1

0 feedback 함수를 이용하여 전달함수 G佃）와귀환 경로 값 l을 연결한다．

1

0

Otf함수를 이용하여 전달함수 모델을 생성한다．

1

0
U

그림 +2 계단 입력 함수 코딩 결과（FdSysSte口.m)

U

8

0

m

n
r

gteat ( Input ) ;
gt eat ( ' Out put ) ;

中

n
b

xlabel (Time(sec) ') ;
ylabel (dmpl itude ') ;
titleC 'tinity Feedback System: Step function) ;
arid;

m

二
U

pIot (t.y 'b-' ,t,u. ' r-'); e
ads(I0 150 in) ;

戶

4

0

m

n
J

[y,t)
;
u=ones(size(t));
=step

9
느

匠5＝小佃＋2)/(SdS+3)dS+7) ) ;
sys= feedback (G_s』1) ; 0

m

LI FdSysStep.m X
s=tf ( 's' ) ; e
1

系i

(a)

이때 출력행렬 y의 행 크기는주어진 시간 벡터 t와 같고, 열 크기는 시스템 벡터 sys와같다．

下tie 帥t

Viw 뗘a川t To必

DeS岫呻 朔的州 He巾

Dd 日 曲 ! 臣 1曳民好自堤 / 니昌 口 因 U 口
Un御 Feedback System: Step function
1

啣
0.8
8
0

8쿄죤之

4
0
02

0

0

奴｝

5

15

什no（羽（力

그림 아3 계단 입력 함수 실행 결과

U
U
U
4
中
寸
4

gtext ( Input ') ;
gt ext ( Out put ' ) ;

e

olabel ( ' Time(sec) ') ;
미 abeI ( '/川키 itude ) ;
title ( 'Unity Feedback System: Parabol ic function') ;
grid;

e

[y;t]:lsi.(sysp
pl。t(ty, b- 註“．
：牟0

4

t =O:O. l : l刃;

p_t=O. St.,t; e

=

oys= feedback (G_s,l); e

4

오S＝巾（5+2)/(5KS+3)K5+7) ) ;

=

抄"’娑,寸3,
123456789mn促m

(b)

계단 입력 함수에 대한 단위 귀환 시스템을 실행한 결과의 정상상태 오차는 0이다．

그림 +4 포물선 입력 함수 코딩 결과伯好羚F뇽m.m)

Otf함수를 이용하여 전달함수 모델을 생성한다．
0

feedb缸水 함수를 이용하여 전달함수 G(s）와 귀환 경로 값 1을 연결한다．

0 포물선 입력 함수風t)를 지정한다．
01誼n 함수를 이용하여 포물선 입력 함수의 출력 응답 y와 시뮬레이션에 사용하는 시간 벡터 t를 찾
는다．
0 포물선 입력 함수와 출력 응답을 그래프로 나타낸다．

CHAPTER 09 제어

201

日｝e

태it

"伯咐

Ins心t

：그 t;J 닢 申

Tools

Des卞Sop

쌔出｝w 卜佃tP

a뇨 =\ 곤7 包 \e J; ' a

口 住크 . 口

UrutyF啣back Sy며미TEF汭毗세帥批1km

5（刃0
4風10
4000
3500
쁨귿죠E <

3000
2500

10

入1

或1

40

印

60

70

凹

佚）

100

Th月
（羽c)

그림 9小 포물선 입력 함수 실행 결과

포물선 입력 함수어｝대한 단위 귀환 시스템을 실행한 결과의 정상상태 오차는 무한대이다. 즉 시간이 증

(c

가함에 따라오차가무한대로 증가한다．

jJ1 - FdsysRamp.m
X
s=tf ( 'u ') ; 1
나
口

2寸

6

r t=t;

=

t=O:O. I：印；

m

나
二

4

G..s=4.(s'2)/(s士（su3）士（5,7) );
oys=feedback (오s,l) ; 0

1

0

小

r-

.)

t.

t,

r.

5-

(sys,

y,

Fy.

'

;

1

0

1

grid;

1

gtext ( lrspat ') ;

m

gtext ( " Output ) ;

1

1111

title ( 'Ursity Feedback Sputem ' Ramp function' );

=

1
1 L
口
DU

니 abel ( 'Am口l itude ');

e

8 9 0

_t.

)

r
n
pl。
tl:
t(t,lsi.
t r_ ;
olabel ( 'Time(sec) ') ;

그림 9田 램프 입력 함수 코딩 결과（田旬sRa叫）.rn)

Off함수를 이용하여 전달함수 모델을 생성한다．
0 扼edback 함수를 이용하여 전달함수G臼）와귀환경로값 1을 연결한다．
0 램프 입력 함수r(t）를 지정한다．
0 isim 함수를 이용하여 램프 입력 함수의 출력 응답 y와 시뮬레이션어］ 사용하는 시간 벡터 t를 찾
는다．
0 램프 입력 함수와출력 응답을 그래프에 나타낸다．

202

PART 03. MATLAB촨용하기

r

뇨

ins.作

TOO匕

Deskt야）

쌔n的w

什eip

' , \ 믄7 @ 포 J二 ! 目 口 目 I. 口
Un御 F的（北ack System: Ramp h月M出이l

그림 +7 램프 입력 함수 실행 결과

램프 입력 함수에 대한 단위 귀환 시스템을 실행한 결과의 정상상태 오차는상수이다．

CHAPTE日 09. 제어

203

LESSON

02

a匿리스 변환

복잡한 제어 시스템의 입출력 관계를 미분방정식을 이용하여 수학적으로 해석하기란 매우 어렵다. 이때 라플라스 변환을 이용
하면 복잡한 형태의 선형상미분방정식을 간단하게 풀 수 있다. 卜IlATLAB에서 라플라스 변환을 이용하여 제어 시스템의 입출
력 관계 해석과 설계를 간편하게 실행해보자．
Keyword

I

1 라플라스 변환 1 라플라스 역변환 1 부분분수 전개 I residue 1

라퓬라스 변환

어떤 시간 함수／(t) 어le " 를 곱한후 시간 t어］대해 0부터 的까지 적분한 것을 함수人t) 의 라플라스 변환
(Laplace transform)이라고 한다. 라플라스 변환은 다음과 같이 정의한다．

F(s) =工[f(t)] = J, f (t) e_stdt

(9.1)

라플라스 변환의 1차 도함수와 2차 도함수를 정리하면 다음과 같다．

뇌브／(t)卜伊（小／(0)

(9.2)

뇌뜩加나卞이可仙寸（0)

(9.3)

Ldt

dte

J

J

이때 只0）과 /' (0）은 초기 조건을 의미한다．

M-File I CtrlLap.m

1 예工119- 2 I
직렬 RLC 회로를 해석하여 얻은 미분방정식이 다음과 같다．
LCi0(t) + RCi0(t) + v0(t) = RC亡1(t)

라플라스 변환을 이용하여 R= l000[(2], R= 10뜨긱인 경우에 대하1 단위 계단 함수 v1(t)를 입력으로 인가
할 때 출력 전압 v0(t)의 단위 계단 응답을 각각 구하고, 그래프로 그려서 비교하라. 이때1 시간은 t= 0부터
t = 5[msec｝까지 변화하고. C= 105[F], 乙 = 5 x 103[H], 모든 초기 조건은 九(0) = 比（0) = V1(0) = 0이다．

204

PART03. M酊녀B활용하기

1234567B9mn促日H巧佰口田円

!J CM呻．m 놔明

to'

4

ss'ms a A
Vo_s = le-5.R*s/( (Se-O怜'2*le-S*R,o*l).o) ; 0
Vo. .ol = oubo(Vo_oRlOOO) ;

=
-

=

vo_ti = l laplace (Yo_sl); 0

=
=
=
m
e
m

Yo_o2 = oubs(Vo_o .R, 山) ;
vo_t2 = i laplace(Vo_s2) ; 0
t= O: tfl刃l : lXl3;
vol = subs(vo_tLt) ;
vo2 = oubs(vo_t2.t) ;
oubplot (211) ;

寸

plot (t.vol); 0

m
e
m
m

xlabel ( 'Time (sec) ');
ylabel (’寸bt{ V_o_u_t} '); O
title(Broadband fI lter: A = lOW甘Omega' );
oubplot (212) ;

中

plot(t, vo2); O

m
m
4

xlabel ( 'Time (sec) ') ;
이 ab미 C.싻mL工山t} );
title( 'Narro밖尸band fi lter: fl = 1 口骨Omega ) ;

그림 9田 라플라스 변환을 이용하여 단위 계단 응답 구하기 코딩 결과（Ctd녀口.m)

0 초깃값이 0일 때 라플라스 변환식은 [LCs2 +RC노 +1] V0(s) = RCsV (s)이다. C, L, 巧(s)를문제에
서 제시한 값으로 지정한다．
OR= 1000侄기일 때의 라플라스 변환 식을 라플라스 역변환한다．
0 R= 10侄긱일 때의 라플라스 변환 식을 라플라스 역변환한다．
0 R= 1000[(］일 때의 단위 계단응답을 그래프로 나타낸다．
0 조판 형태로 아래 글자를 표시할 때는 밑줄을 사용한다．
QR= 1아Q］일 때의 단위 계단 응답을그래프로 나타낸다．
F斗e 帥I VIew S巧art Tools C珀吐t아1 嚼1心7*

1

：그 d 1d 曲 1 公 i 曳 民 心 @ 嘆 / 니 目 1 目 토크 U 口
白m成lend 介侄ecf之 心 1000C
드
小
놔
0.5
0

1

15
2
Tin怜（羽C)
Narro畔心카닙 filter: R = 1011

2.5
=10"

//\

n
<

H

0

///H＼

//,

「＼

,,\

.,

020

0.5

1.5
Tin怡（胡c)

2

2.5

3
X10a

그림 9四 라플라스 변환을 이용하여 단위 계단 응답 구하7 ( 실행 결과

필터는 전송하는 신호어써 원하지 않는 주파수 성분을 제거하고 필요한 주파수 성분만을 걸러내서 신호를
보내는 역할을 한다. 대역 필터는 일정한 대역 범위에 속하는 주파수 성분만을 통과시키고 대역 범위 밖의

CHAPTER 09. 제어

205

주파수 성분은 모두 차단한다. 이때 대역 범위에 따라 협대역 필터（narrowband flu把r）와 광대역 필터
(broadband filter）로 구분한다. R= 1000[C］일 때는광태뼉 필터의 결과가, R = 10[n］일 때는 협대역 필
터의 결과가 나타난다．

'

a出F라스 역변환

라플라스 변환으로 구한 함수 F(s)를 다시 시간 함수／(t)의 형태로 바꾸는 것을 라플라스 역변환
(inverse Laplace transform)이라고 한다. 라플라스 역변환은 다음과긷히 나타낸다．
t

'[F (s)] = f (t)

(9.4)

기본 함수의 라플라스 역변환은 라플라스 변환 표를 직접 이용하여 짖아낼 수 있다. 예를 들어 함수
1 의 근搢라스 역변환은可.，이고, 힘：수 드의 己搢라스 역변환은cc］다．

S 十 (7

S

I 부I站 수 전'II
부 분분수 전개（partial fraction expansion）는 다항식으로 표현되는 분자나분모의 차수가높은 분수식
을 차수가 낮은 여러 분수식의 합으로 나타내는 방법이다. 만약 분모의 차수가 높거나 식이 길어서 라플
라스 변환표를 이용할수 없다면 주어진 라플라스 식을 부 분분수로 전개하여 기본 함수의 형태를 먼쩌 찾
은 다음 라플라스 변환 표를 이용하는 것이 효과적이다．
M-F加 I PartLap.m

1 예처19-3 I
부분분수 전개를 이용하여 함수 F0）의 라플라스 역변환을 구하라．
. .

s2+12

r (s) =s3 +5s2+ 6s

배껑
지식

口 residue
residue 함수는 부 분분수 전개를 통해 구한두 다항식 num(s) /den(s）의 비율을 이용하여 열벡터로 표현되
는 부 분분수 계수 r. 극점 p와 행벡터로 표현되는 직접 항 k를 구한다．
residue 함수의 기본 형태는 다음과 같다．

(r, p, k] = residue(num, den)
·num: 분자의 다항식 계수를 내림차순으로 나타낸 벡터
·den: 분모의 다항식 계수를 내림차순으로 나타낸 벡터

206

PART 03. M月ILAB활용하기

I

1

PartLap.m 可
symost
12比＝i Iapiace( (s'2너2) /1s '3+5怜 ' 小타8) ); <1
3display( IL =');
4pretty(IL) ;
5num=[1 0 121;
6den=ll 5601;
7lr, p.k! = residue(num, den) ; 0
8coeft薑r '
9尸
PU陀 多 口’
10direct = k
+

풀이

4

그림 9너0 라플라스 역변환과 영점, 극점 구하기 코딩 결과（由rtLa口.m)

0 ilaplace 명령어를 이용하여 라플라스 역변환함수를구한다．
0 residue 함수로 계산된 r, p, k 값은 열벡터로 나타나는데, 결과를 보기 쉽도록 전치 연산자를 통해 행벡
터 형태로 전환하여 사용한다．
Command Window

군）

>> PartLap
IL =
exp（召 t) 7 - exp（丑 t) 0 + 2

coeff =
7. 000口

七.In

2.010)

pole =
-3.［刃00

-2.［刃00

U

direct =

[1
그림 9너］ 라플라스 역변환과 영점, 극점 구하71 실행 결과

residue 함수의 계산 결과는 계수를 극점에 각각곱해서 더하는 형태인 7e_3t - 8e_2t +2이며, 심벌릭 명령
어로 직접 구한 라플라스 역변환과 같은 결과를 보여준다. 만일 분자 항의 수가 분모 항의 수보다 적다면 직
접 항 계수의 벡터 direct는 빈 형태가 된다（문제에서 분자 항은 2개, 분모 항은 3개이다）.

CI-IAPTE日09. 제어

207

LESSON

03

전달함수

선형 시불변 시스템의 전달함수는 출력 응답 함수의 라플라스 변환에 대해1 인가되는 입력 함수의 라플라스 변환 비율로 정의
된다. 이따1 시스템의 모든 초:7 ' 조건은 0으로 지정된다, 전달함수는 시스템의 입력과 무관하므로 여러 입출력이 있는 다변수
시스템에도 전달함수의 정의를 적용할 수 있다. MATLAB을 이용하여 전달함수의 계단 응답과 임펄스 응답의 결과를 비교하
여 살펴보자．
1 전달함수 I imp네se l 전달함수 직렬 연결 1 전달함수 병렬 연결 1 senes I para呵 1

Keyword

I

전닫합수

전달함수（如）는 임펄스 응답 g(t)의 라플라스 변환으로 정의한다. 출력 y(t) 의 라플라스 변환 ｝佃）를
구하기 위해 입력 x(t)의 라플라스 변환 X(s) 에 전달함수（耶）를 곱하면 다음과 같다．
Y(s) = G(s)X(s)

(9.5)

또한 전달함수는 출력의 라플라스 변환을 입력의 라플라스 변환으로 나눈 값이므로, 식 (9.5）에 라플라
스 역변환을 적용하면 출력에 대한 시간 함수 y(t）를 얻을 수 있다．
M-File I TfResp.m

i 예제 9- 4 I

시간 0 드 t됴 10일 때 전달함수 G(s刃II 대한 임펄스 응답과 계단 응답을 구하고 그래프로 나타내라．
s+ 5

nre\ =
U ' "'
s2+

배껑
지식

2s+ 5

U impulse
impulse 함수는 전달함뉴 SYS를 시간 벡터 t 동안 시뮬궤이션한 후의 출력 응답 y를 임펄스 응답으로 나타
낸다. 단위 임펄스 응답을 계산하는 im삐se 함수의 기본 형태는 다음과같다．

y = impu怡e(sys,t)
· y: 출력 응답
· sys: 전달함수
· t: 시간 벡터

208

PART03. M月T녀B 활용하기

1
1

iJ 加sp.m )｛羽

t=0: 0. 01 :10;

e

풀이
=
m
U
1
1
1
4

subplot (211) ;

plot (t,y_Imp); 0

1
1

xlabel ( 'Time(sec) );
ylabel ( 'Ampl itude ') ;
title ( Impulse Response ') ;
subplot (212) ;

U
U
느

1 1 1 1 1 1 1

e

n
<
4
6
B
0
2 3 4
6
U
口
1
口
U
口
1
1
나
二
U
L

m

num=]1 5] ; (1
den=]1 25] ;
G_s=tf (num, den) ; 0
y_iip=impuIse (O. s』t); 0
y_st=step (G_s,t); 0

plot(t,y_st); 0

1

xlabel ( 'Time(sec) ' );
미 ab이 ( 'Ampi itude ') ;
title ( 'Step Response) ;

그림 +12 임펄스 응답과 계단 응답 코딩 결과（ltResp.m)

0 분자와분모의 다항식 겨｝수를 라플콰스 변수S의 내림차순으로 지정한다．
Off함수를 이용하여 전달함수（如）를 지정한다．
0 impulse 함수를 이용하여 임펄스응답 결과를 얻는다．
0 step 함수를 이용하여 계단응답 결과를 얻는다．
0 임펄스옹답결과를그래프로나타낸다．
0 계단응답결과를그래프로나타낸다．
Fik甘

Ed注

\hew

Ins꺼S TOO七5

De5kt야1 WEsdo나

H이p

D d 日 邕 臣 '\ =\ 抑 包 咽 d r 包 ! 口 目 吐 口
In私腐eRespon羽

1,5
0
n
U
=
召코죤之

1

舶
0
2

1
0
U
=
쁨＝ 붚 E <

/

,/“

1/

「1\

0
0

1

3

2

4

5
6
了U'旨（羽C)
Sb하：1Reap아好e

1

8

9

10

7

8

9

10

r

3

4

5
6
'rim始（Se타

그림 아13 임펄스 응답과 계단 응답 실행 결과

그래프의 위쪽에는 임펄스 응답 결과가, 아래쪽에는 계단응답 결과가 나타난다．

CHAPTER 09. 제어

209

전달함수 직렬 연결

I

식 (9.5）를 단일 전달함수블록선도伯lock diagram)로 나타내면 ［그림 9-14］와같다．
耶）
그림 9-14 단일 전달함수 블록선도

＝가 놓
전달함수의 직렬 연결（se如s connection）은 입력 X(s）와출력 Y(s) 사이에 2개 이상의 전달함；
여 있음을 의미한다. 전달함수의 직렬 연결을 블록선도로 나타내면 ［그림 9-15］와같다．

X(s)
> （기（s)

G如）

如）

그림 9너5 전달함수의 직렬 연결 블록선도

전달함수의 직렬 연결은 다음과 같이 전달함수 2개를 곱한 형태로 나타낸다．
Y(s) = G1(s)G2(s)X(s)

I

(9.6)

전닫합수 병I 연겸

전달함수의 병렬 연결（parallel cor끄lection）은 실행 전어］ 결함을 예측하고 실행하는 귀환 과정을 제어
하는 기능미 있어서 피드포워드（fee小brward）라고도 한다. 전달함수의 병렬 연결을 블록선도로 나타내
면 ［그림 아16］과같다．

그림 9-16 전달함수의 병렬 연결 볼록선도

전달함수의 병렬 연결은 다음과 같이 전달함수 2개를 더한 형태로 나타낸다．
Y(s) = [G1(s) + G2(s)]X(s)

210

PART03. M月兀AS휨용하기

(9.7)

M-FJe I TfConn.m

1 예저19- 5 I

시간 O<t<10일 때 전달함수 G1(s), G如）의 직렬 연결과 병렬 연결에 대한 계단 응답을 그래프로 나타
내라．
／겨 . .

1

(J'lI.S) = 1m= ,
S 十I

series,

／기 . .

s+ 2

LJIS) = 十
S+ 3

지식

ser妃S 함수와parallel 함수는 전달함수2개를각각 직렬, 병렬로 연결하는함수이다. 직렬 또는 병렬로 연

parallel

'

II

1

11117:

-_

결된 전달함수 sysi과 sys2를 곱하거나 더하여 새로운 전달함수 sys를 생성한다. 두 함수의 형태는 다음과
같다．

sys = series(sysl, sys2)
sys = parallel(sysl, sys2)

푿이

1 札毗m X + !
t0也미和；<
I-

Gi_s=t1(EO 1Lii nLe

plot (t, yl.
;
xlabel ( 'Tise(sec) ') ;
비ab미(.帥pl itude ') ;
tltle ( 'Series Connection) ;
grid;
subplot (212) ;

U
L

6 7 8
U
0

-

1
1

2

m
-

U
口

4 5 6

-

-

1
口

-

Bm

-

..st)

O

plot (t,y2. .st); e

nlabel ( Tlme(sec) ');
ylabel ( 'Aspl itude ') ;
titie ( 'paral lel Connection' );
grid;

1 1 1 1 1 1 1 1 1

m...s=tt (ii 21. 11 31) ;
SC引＝series（미J庄느寸 自
sys2=paral I미（31_s.叱S戶0
yL. st=step(sysi,t); 0
y2. .st=step(sys2, t);
subplot (211) ;

4

中
叫
-

0

U
口

2-

그림 9-17 직렬 연결과 병렬 연결 코딩 결과（TfConn.rn)

0 시간 0St 10을 지정한다．
Off함수를 이용하여 전달함수 G1(s）와 G2(s）를 지정한다．
0 series 함수를 이용하여 두 전달함수를 직렬 연결한다．
0 parallel 함수를 이용하여 두 전달함수를 병렬 연결한다．
0 계단출력 응답을 얻기 위해 step 함수를 이용한다．
0 전달함수의 직렬 연결 결과를 그래프로 나타낸다．
0 전달함수의 병렬 연결 결과를 그래프로 나타낸다．

CHAPTER 09. 제어

211

File

Ed仕

View

Irr5e竹

Deskto口

!0이s

Window

He如

口 j a 4J 1i ', , 尸」 兮 七］ j= . 邑 口 國 ：그 ［口
8
0

SenesC4거111兀lion

6 4 2
0 0 0
g쿄죤之
/

/

0

2

3

2

3

8

1

0

5
6
Tier咆（ow이
Parallel C에nemi에
4

8

9

10

7

8

9

10

g글죠E <

7

161.4

12
4

5

6

Tw旨佃e이

그림 9-18 직렬 연결과 병렬 연결의 계단 출력 응답 실행 결과

태e 日lit

View

D心 a $

lnswt

Tools ［允寸由야1 山ndo나

He巾

自 ‘瓦 g\ 抑 自 浸 川 ' 巳 口 匡크

그 工工1

Transfer functi川 G1(s)
5
0
쁨르죠E <
3

8

9

10

6
5
Tin始（明c)

8

9

10

9 B
0 0 r
0
1
쁨글죠E <

\

6
7
5
Tire忙（se아
Transfer fur花tionG2（引
4

D
毗

2

3

4

7

그림 9-19 G由）와 G如）의 계단 출력 웅답 실행 결과

이해를 돕기 위해 2개의 전달함수 G1(s）와 G2(s)에 대한 계단 출력 응답을［그림 9-19］에서 보여준다．매1
초 단위에 상응하는 전달함수 G1(s）와G如）의 진폭을 곱하면［그림 9-18] 위쪽의 직렬 연결 결과와같고，
전달함수 G小）와G如）의 진폭을 더하면［그림 아堈 아래쪽의 병렬 연결 결과와같다．

212

PART 03. MAThAB활용하기

LESSON

04

생때방정식

전달함수를 이용한 제어 시스템 해석의 결점을 보완하기 위하1 상태방정식을 이용하는 상태공간 모델을 많이 사용한다. 상태방
정식은 상태변수의 ］차 미분방정식으로 구성되고, 상태공간 모델은 刃개의 ］차 결합 미분방정식으로 물리적 시스템을 나타낸
다. 일반적으로 상태변수는 시스템에서 에너지 저장 요소의 상태를 나타내는 변수이다．
Keys사ord

I

1 상태공간모델 I tf2ss I ss 1 ss2tf 1 斗pud 1 flipir

상태공간 모델

선형 제어 시스템의 상태공간（state-space) 모델은 다음과 긷히 나타낸다．
文 = Ax + Bu

(9.8)

y = Cx + I沁

(9.9)

상태방정식 (state equation）인 식 (9.8）어］서 A는 m勺I 시스템행렬（system matr汶）, B는 n)＜刃7 입력행
렬（input matdx), x는 刃 상태 벡터, U는 m 제어 벡터라고 한다. 그리고 출력방정식인 식 (9.9）에서 C는
r><刃출력행렬佃Ut叫mati奴）, D는r사刃전송행렬（transmi豁ion rn北奴）, y는r출력벡티라고한다．

1 예제9-6
다음 시스템에 대한 상태공간 계수행렬을 구하라. 이따1 인가되는 기준 입력 匙s)는 계단 함수이고, C(s）는 출
력 제어 변수이다．
C(s)
35s+ 7
R(s) m S3 + 5S2 + 36s + 7

；而
지식

' tf2ss
단일 입력 전달함수로부터 상태공간의 계수행렬 A. B. C. D를 구하는 tf2ss 함수의 기본 형태는 다음과
같다．

(A, B, C, D] = tf2ss(num, den)
· A, B, C, D: 계수행렬
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

CHA다rER 09. 제어

213

풀이

日）

Command Window
>> num=[0 0 36 71; 0

訂：";[.;．瑥熙小,)0
4 =
6
1
U

-35
U
1

-7
0
0

35

7

B
l
C
C

C
0

D
0
그림 앍20 상태공간 계수행렬 구하71 실행 결과

0 전달함수분자의 다항식 계수를 내림차순으로 지정한다. 차수 중간어］빈 차수가 없으므로 분자를 지정할
때 3차와2차의 계수를 0으로 지정하지 않아도 된다．
0 전달함수분모의 다항식 계수를 내림차순으로 지정한다．
0 전달함수를상태공간의 계수로 변환하는tf2ss 함수를 이용하여 상태공간의 계수행렬 A, B, C, D를구
한다．

I

계수행렬에서 전달함수구하기

초기 조건이 0일 따씩 (9.8）과식 (9.9）의 라플라스 변환은다음과같다．
sX(s) = AX(s) + BU(s)

(9.10)

Y(s) = CX(s) + DU(s)

(9.11)

식 (9.10）은 다음과 같이 다시 쓸 수 있다．
X(s) = (sl - A)m1BU(s)

(9.12)

식 (9.12）를식 (9.11）어］ 대입하면 다음의 식을 얻는다．
Y(s) = [C(sl 小 A)e1B + D]U(s)

214

PA日T03. MA兀AB활용하기

(9.13)

'B

-

A)

=

(sl

(S)

U（키

C

Y

=

G

(s)

계수행렬을 이용한 전달함수는 다음과 같이 정의한다．

(9.14)

+D

M-Fite i StateTf.m

1 예제 9- 7 I
제어 시스템은 다음과 같은 상태공간 방정식에 의해 정의된다．

1*,'1- -1.5 -1.
2511
x1卜Lro.。5j卜 y=[O O.5]I X2
[X2]- L 2 。 j
Lx2i

시스템의 전달함수 G(s）를 구하고 단위 계단 응답을 그림으로 나타내라. 또한 심벌릭 툴박스를 이용하여 식
(9.14）의 결과를 직접 구하고 전달함수（如）의 결과와 비교하라．

배경
지식

口 ss
ss 함수는 계수행렬 A, B, C, D를 이용하여 연속 시간 상태공간 모델을 의미하는 sys를 생성하므로 이를
이용하면 상태방정식을 화면에 출력할수 있다. ss 함수의 기본 형태는 다음과 같다．

sys = ss(A,B,C,D)
· sys: 연속 시간 상태공간 모델
· A, B,C,D: 계수행렬

R ss2tf
상태공간의 계수행렬 A, B. C. D를 이용하여 전달함수 분자와분모의 계수를 구하는 ss2tf함수의 기본 형
태는 다음과 같다．

[num,den] = ss2卄(A,B,C,D)
·num: 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 전달함수의 분모 계수를 내림차순으로 나열한 벡터
, A 已 C, D: 계수행렬

1-

H ""' 黑；싻恐；加］;<)

7-

6-

2-

2m
3451
6m
7m
Be
8-

푤이

日＝10. 5이 ;
C=10 0.61;
0=0;
eys횬．ss(A，日，C,D) e
(num, denl=ss2tl(A,B,C,D); 0
i＄추，
tf (nu吼den) 0
step(sys) ; 0

團

:：增 于기 계수행렬에서 전달함수 구하기 코딩 결과（S떼可fm)

CHAP1匡R 09. 제어

215

0 계수행렬A, B. C. D를지정한다．
0 상태방정식을 화면에 출력하기 위해 SS 함수를 이용한다．
0 tf2ss 함수와반대 기능을가진 ss2tf함수를 이용하여 계수행렬을 전달함수로 변환한다．
0 전달함수를 화면에 출력하기 위해 if 함수를 입력한다．
0 시스템의 전달함수 G（砂의 단위 계단응답을 그래프로 나타낸다．
Tools Des났야｝ Wosdow He巾
D 巴日 缸 r

' \ -s y'1 自 嘔｝ 可： , 晟匕 ［그 듣

感 ［口

Step Response

二U

m
n
쁨
＝ 芸드 ＜

4

3
4
기me 臼미刃nds)

三

6

7

그림 乎22 전달함수의 단위 계단 응답 실행 결과

C아smand＼斗IN抑w

xl
x2

o2
xl
-1.5 -1.25
0
2

b =
xi
ci 0. 5
X2
口
C

=

yl

xl
o2
0 0.5

d =
yl

ul
IJ

Continuous-time state-space model .

0_s =
0.5
s2 x i .So + 2. 5
Continuous-time transfer function
그림 +23 계수행렬에서 전달함수 구하71 실행 결과

宅字6

PART 03. MAT냐＼B활용하71

꾼）

Command Window
>> sswm二
>> A=［니 ,5 -l．西；2 0] ;
>>B=]0.5;0] ;
>> 0=10 0.5] ;
>> 0=0;
>> 0...s=C* inv(s.eye(2,2)-A)*B;
>> pretty(G. .s)
1
2
2s

+ 3s * 5

그림 아24 심벌릭 실행 결과

［그림 아23］어써 구한 전달함수 결과와［그림 아24］에서 심벌릭 툴박스를 이용하여 구한 결과가 같음을 확
인할 수 있다．

I

위상변수 표준형

신호흐름선도(s培nal flow graph）를 이용하여 전달함수를상태방정식으로 변환하는 경우，상태변수를 어
떻게 정하느냐에 따라상태방정식이 다르게 나타난다. 예를 들어 다음과 같은 전달함수가 있다고 하자．

Sn
" ＋口,

"

小l

하S"+ b. lS" l +... + b s + b。
＋· 口iS＋口0
·

尸iS

G(s) =

(9.15)

·

식 (9.8）의 상태방정식이 다음과 긷히 행렬 A와 열벡터 B로 표현된다면 이를 위상변수 표준형 (phasevariable canonica나brm)이라고 한다. 위상변수 표준형은 시스템 상태변수 사이의 관계가 1차 미분이
되도록 하는 방법으로 가제어성 표준형 (cot出이lab血y canonical form）이라고도 한다. 이때 행렬 A와
열벡터 B, 출력 행벡터 C는 다음과 같다．
-o

i

o

·..

0

0

0

1

...

0

A=

(9.16)
0

0

0

...

1

h口0

-a1

-口2

'"

=b- 1

0

B=

0
(9.17)

i
0
1_

C = {b0 - a0b

自 - a1b

外2 - an_2b

b_1 - an_1bn]

(9.18)

CHAPTER 09. 제어

217

I

제어기 표춘형

식 (9.8）의 상태방정식이 행렬 A, 열벡터 B, 출력 행벡터 C로 표현된다면 이를 제어기 표준형 (C아l尸
troller canonical form)이라고 한다. 제어기 표준형은 tf2ss 함수를 이용하여 얻을 수 있으며, 상태방
정식을통해 제어기를 설계할 때 편리하게 사용할수 있다. 제어기 표준형에 사용하는 행렬 A, 열벡터 B,
출력 행벡터 C는 다음과 같다．

1

1

1

1

1

1

0 0

가0

1

1

0 l

m 0

1

0 0

l 0

가0

吼 l 1

A

꺄
0
0
C = [br2_1

an_1bn

b_2 -a刃_2bn

·．· b -a1b?2 b。-a。
bn]

韜卜돠沌 1 StatePhase.m

1 ,예제 9- 8 J
다음 전달함수를 상태공간에 위상변수 표준형으로 나타내라．
,,, .

C(s)

s2+ 9s+18

1八키 = 二：尸H = 그
. . )
1八
.
K (S)
sV +I1s日 +38s+ 4U

；在

' flipud

지식

계수행렬을 위상변수 표준형으로 바꾸려면 행렬을 위아래 방향으로 뒤집어야 한다. 주어진 행렬의 열 형태
는유지하고 행의 위아래 방향을 뒤집는flipud 함수의 기본 형태는 다음과같다．

:

flipud(x)

. flipir
계수행렬을 위상변수 표준형으로 바꾸려면 행렬을 좌우 방향으로 뒤집어야 한다. 주어진 행렬의 행 형태는
유지하고 열의 좌우 방향을 뒤집는磁ph 함수의 기본 형태는 다음과 같다．

218

PART 03. MATLAB활용하71

LI StatePhase.m 拿n둬
1234567느
8片

num= ]l 918] ;
den=]1 Ii 3840] ;
G_s=.tf (num, den) 0
(Ac』Oc』Cc, Dc) =tf2ss(num, den) ; 0
시引I pud（加） 0
A引l ip냐（川 0
B引i i pud（叫 0
c=f H口나（CC) 0

m

그림 +25 위상변수 표준형으로 나타내7] 코딩 결과（S怡냠汁日se.n,)

Off함수를 이용하여 전달함수 G(s）를 지정한다．
ot끄ss 함수를 이용하여 전달함수로부터 상태공간의 계수행렬 Ac, Bc, Cc, Dc를 구한다．
0 위상변수 표준형으로 바꾸기 위해1 계산된 계수행렬 Ac의 위아래 방향을 뒤집는다．
0 다시 좌우 방향을 뒤집어야식 (9.16）과 같은 위상변수 표준형 행렬 A가 된다．
0 계산된 계수행렬 Bc는 위아래 방향을 뒤집어야 식 (9.17）의 위상변수 표준형 행렬 B가 된다．
0Cc는 좌우 방향을 뒤집어야 식 (9.18）과 같은 위상변수 표준형 행렬 C가 된다．

>> State다ase
B 5=
s2 * 9 s + 18
s3 + II s2 + 羽 s + 40
Continuous-time transfer function

Af =
0 D 如

1
（그
-田

［그
1
-Il

18

9

1

d
1

1 0 田

0
［그
0
口40

4=

1

8=

풀이

C =

그림 +26 위상변수 표준형으로 나타내기 실행 결과

CHAPTER 09. 제어

219

LESSON

05

시간 응답

입력 신호를 가한 후의 시간에 따른 출력을 시간 응답이라고 한다. 시간 응답의 특성을 해석하면 제어 시스템의 성능에 대한
평가가 가능하다. 제어 시스템의 시간 응답은 과도 응답과 정상상태 응답으로 나눌 수 있다. MATLAB율 이용하여 과도 응답
과 정상상태 응답의 실행 결과를 그래프를 통하1 비교해보자．
Keyword

I 감쇠비 1 특성방정식 1 과도응답 1 정상상태 응답 1

I 감쇠비와 푹성방정식
표준 2차 제어 시스템의 전달함수는 다음과 같이 나타낸다．
M(s)

=

3'

三

0)

,

=

,

乙
八
寸
乙CO九3'
寸 (I).,
V
r 1
r1

(9.19)

식 (9.19）의 분모를0으로놓고 얻는방정식을특성방정식（characteri師c equation）이라고한다. 여기
서 c는 감쇠비 (damping rati이, U뇨은 고유주파수（natural frequ帥cy）이며, 이는 2차 제어 시스템을
해석하고 설계할 때 중요한 역할을 한다. 고유주파수는 모든 감쇠가 제거된 후 진동의 주파수이고 응답의
빠르기를 나타낸다．

M-File ! CtrlDampRt.m

1예제9四 1

시간 0 드 r 드 10일 때 감쇠비 5 = 0.0, 0.2, 0.5, 0.8, 1.0을 이용하여 닫힌 루프 시스템의 전달함수 M(s째t
대한 계단 응답의 곡선을 각각 그려라．
M (s) =

220

PA日T03. M月TLAB활용하71

l
S二 + 25s + 1

jJCtnloampRtm

3 4 5 6 7 8 9 m H 俚 侶 H 侮 怜 n 化 円

二：

풀이

t=0:0. 1:10;
zeta=[0. 0 0. 2 0. 5 0月 1 .0] ;
Eifor n=1 : 5; 0
num=[0 0 1] ;
den=[1 2.zeta(n) II;
tn 1 :l01,n) ,n, t] =ste口(num, den, t) ;
end
plot (t, y(1:101,1L 'r- ') ; 0

hold;
plot (t, y(l: 101, 2), 'b-') ;
plot (t, y(I: 101, 3), ' 9_') ;
plot (t , y( 1:101, 4) , ' r: ') ;
plot (t, y(1:l01,5), b: ');
grid;
elabel C Time(sec) ') ;
ylabel ( A畔니 itude ') ;
title ( 'Unit Step Response ') ;
legend( '甘zeta=0. 0, 'Wzeta'0. 2', '甘zeta=0. 5', 'tzeta=0.8 '. . . . 0
’單zet a=] 月 . '［끄cot 向n . ’駐r ) ;

그림 9-27 감쇠비에 따른 정상상태 응답 코딩 결과（CtrlDa叫）닥.m)

0 for문으로 5개의 감쇠비를 반복적으로 이용하여 계단 응답을 계산한다．
0 감쇠비가0,0, 0.2, 0.5. 0.8, 1,0일 때의 계단응답결과를그래프로나타낸다．
0 legend 명령어의 내용을 다음 행까지 이어서 나타내기 위해 ..．를 人卜용한다．
汨隘好的t小晦叫 Insert
口 已日 缸

臣

To이S

', \

t乂帥t야｝ WIndow

好 包咽 而 끼 骨

H帥）
口國

釀

Unit Step Response
t8
1.6 1

2

3

4

5
6
Tin始（Se아

7

8

9

10

그림 于羽 감쇠비에 따른 정상상E卄 응답 실행 결과

c= 0일 때 특성방정식의 두 근은 모두 복소평면에서 허수축어i 존재하며, 이러한 출력을 무제동 응답
(undamped re하兀nse) 이라고 한다．
O< c< 1일 때 세 감쇠비에 대한 특성방정식의 두 근 모두 복소평면의 좌반평면에 위치하며, 이러한 출력은
부족제동응답（underdamped response）이라고한다．
c= 1일 때 특성방정식은 s= -1에서 이중근을 갖는뎨, 이러한 출력을 임계제동 응답（critically d跏ped
re하兀nse）이라고한다．

CHAPTE日09. 제어

221

I

과도 응답과 정상상태 응답

시스템에 인가된 입력은 일정 시간이 경과한 후어］ 안정된 출력을 나타낸다. 과도 응답（transient
re叩이始e）은 초기 시간부터 값이 변화하는 동안의 시간 응답이고, 정상상태 응답（steady飢ate
response）은 값이 안정된 후의 시간응답이다．
계단함수를 입력으로 가했을 때 얻는과도 응답의 특성으로는상승 시간（rise 帥e), 정정 시간（sett如g
time), 첨둣값 시간（peak time) , 백분율 오버슈트（percent overshoot) , 정상상태 오차（steady
state error）가 있다．

1 2차 제어 시스템의 사양
특성방정식의 계수를 구성하는 감쇠비와 고유주파수만 알면 특성방정식의 근을 구하지 않고도 계단 응답
의 특성을나타내는 매개변수를 계산할수 있다．이에 필요한상승시간 乙，정정 시간 乙，첨둣값시간 7}
와백분율오버슈트는 다음과 같히 나타낸다．
口， 人』0.8 + 2.5;

1r N

(9.20a)

(On

4
73 之 1
5o)i

(9.20b)

-

冗
7;

(9.20c)

。jn,.Ji구

-(r1riJi二기
%OS= e \ ' " ' 'xlOO

(9.20d)

상승 시간은 출력값이 최종값의 10％에서 909幼'1-지 도달하는 더］ 걸리는 시간이다. 식 (9.20b）의 분모
부분은 감쇠지수주파수（exponential damping frequency）라고 한다. 첨둣값 시간은 제어량이 극점
값을 갖는 시간으로 미분값이 0이며, 식 (9.20이의 분모 부분은 감쇠진동주파수（dan巾ed oscillation
frequency）라고한다. 백분율오버슈트의 경우 최대 출력과최종값의 차를 백분율로표시한다.
M-FiIe I CtrI2ndSys.m

1 예저19-101
二；
11.=mH. -HI
L．

2차 제어 시스템 M (s）에 대한 상승 시간 ，정정 시간 ，첨둣값 시간과 백분율 오버슈트를 계산하고 계단 응답
을 그래프로 나타내라．
100
兀／(s) ===
"
s2+ lOs+100

222

PART 03. M／玎냐＼B활용하기

斗

Ctrl2ndSys.rn

d
1

num=100;
den= t1 10 1 00) ;

n
< n
d

中

:

4

},：낀，
num'
=sgrt(nur。
,den); ); 0
zeta새en(2)

二
U
6

/(2啣em工이 ; 0

nr1

: 位捷；少，胃，客笞－" <)

8
0
d1

(N_

0

pct_oyer ;l00* eap
step
grid;

-

寸

((-zeta*pi) /(sgrt (l-

-zeta

'2)

0
니

Tp芬pi/(omega_n.sqrt ( 1-zeta'2)) 0
s)

풀이

))

title ( 'Step rasp口rise 口I the sec口rid 口rder system ') ;

그림 +29 2차 제어 시스템의 사양 구하기 코딩 결과（C川2nd匐s.m)

Otf함수를 이용하여 제어 시스템의 전달함수를 지정한다．
0 고유주파수con를 지정한다．
0 감쇠비 c를 지정한다．
0 상승 시간 乙을구한다．
0 정정 시간乙를 구한다．
0 첨둣값시간乙를구한다．
0 백분율오버슈트를구한다．
＝의 계단응답을 그래프로 나타낸다．
0 step 함수를 이용하여 전달함；
ri1

>> Ctrl2rrdSys
Tr =
0 2050

Is =
0. SOC0

T口 =

0. 3628

pct_over =
16. 3034

그림 아30 2차 제어 시스템의 사양 구하기 실행 결과

과도 응답 사양을 먼저 정하면 역으로 감쇠비와 고유주파수의 계산이 가능하므로 시스템 특성방정식 근의
위치를 지정하여 시스템을 설계할수 있다．

CHAPTER 09 제어

223

F沁

Ed仕

\lie나

' iJ 3J

自

Insert

Inc血

t地針生야）

w耐아V

H帥）

\ 抑 匈 咽 寸＝ , 邑 口 쿄 ：三

'\

Step response of the second order system

\

12

'\

k,

:：尸

‘

6
n
쁑글죠＝之
02

0.4

0.6
08
Time (s이onds)

그림 아3] 단위 계단 응답 실행 결과

224

PART03. MATLAB활용하71

12

안정도
시스템은 안정해야만 사용할 수 있다. 선형 시불변 시스템에서 한계가 있는 입력을 가해서 한계가 있는 출력을 얻으면 그 시스
템을 안정한 시스템이라고 하며, 이러한 특성을 안정도라고 부른다, 절대 안정도로는 제어 시스템의 안정 여부를 확인하고, 상
대 안정도로는 안정한 정도를 확인한다. MAT냐'B의 routh 함수를 이용하여 시스템의 안적도름 판별해보자，
Keyword

I

1 안정도 판별법 i 루스후르비츠 판별법 i routh i

안정도 판별법

시스템의 안정도（stab血y）를 판별하려면 S 평면에서 전달함수의 특성방정식에 대한근의 위치를확인해
야 한다. S 평면의 우반평면（right half）어］ 특성방정식의 근이 하나라도 존재하는 경우 불안정한 시스템
이라고 한다. 반면에 특성방정식의 모든 근의 실수부가음의 값이어서 S 평면의 좌반평면（left half）에 존
재하면 안정한 시스템이라고 한다．

I

루스1후르비츠 판별법

루스느후르비츠（Routh-Hurwi口） 판별법은 제어 시스템의 절대 안정도（absolute stab小ty）를 빠르게
판단하는 대표적인 안정도 판별법 (stab표蜘 criterion）이다. 다음 세 가지 조건을 모두 만족하면 안정한
시스템이라고 정의한다．
0 판별하는 시스템에 대한 특성방정식의 모튼 계수 부호가 같다．
日 어떤 항의 계수도 0이 아니다．
日 계산된 루스 표에서 제1열의 모든 값의 부호가 변하지 않는다．
다음과같은刃차특성방정식이 있다고하자．
a,s'2 +a,_1s" ' -i- ". +a1s+ a。=0

(9,21)

식 (9.21）과같은특성방정식에 루스H후르비츠 판별법을 적용하려면 다음과같은루스 표를 이용한다．

CHAPTER 09. 제어

225

Sn
Sn-i

an

口刃크

(b극

'"

口n-i

口刃日

口刃巧

" "

C1

C2

C3

Sn크

(9.22)

so
서］ 번째 행의 b] , b2와네 번째 행의 Ci, C2는다음과긷미 계산한다．

自

a7i

（布크

(b-i

口n-3

(9.23a)

口n-i口n그 H口nb日

=

b2 =

ar_i

口刃d

an

（亐i-4

(7n니

(b巧

(9.23b)

(bKb콕 - anan_5

a,？니

口n-i

(9.23c)

尿뇨3 - an고）2

Cl =

131

(9.23d)

b1a月-5 - 口n_il）늉

C2 =

自

루스 표에서 나머지 행의 원솟값이 0이 될 때까지 계속 실행한다. 판별의 필요충분조건은 식 (9.21）에서
S 평면의 좌반평면에 놓여 있는근이 루스 배열 첫 열의 원소와같은 부호여야 한다는 것이다. 만약 첫 열의
원소 부호가 바뀌면, 바뀐 부호의 개수는 양의 실수 부분을 가진 근의 개수를 가리킨다．
M-FiUe I RouthTable.m

i （川저Iq_ 11 1
仁：
：二：二4H：
二，J
(a) 닫힌 루프 시스템의 전달함수 A如刃카 대한 안정도를 판별하라．
M (s) =

5
s4+ 2s3+ 3s2+ s+ 5

(b) 다음 특성방정식에 대한 안정도를 결정하라．
s4 +10s3 + 35S2 +50s+ 24 = 0

226

PART 03. MATLAB활용하71

；而
지식

' routh
특성방정식에 루스卜후르비츠 판별법을 적용하려면 양의 실수 부분을 가진 다항식의 근의 개수를 결정하는
'1차 다항식어］대한루스 배열을 생성하는routh 함수를 사용한다. routh 함수의 기본 형태는 다음과 같다．

routh（이
· O: 특성방정식의 계수를 포함하는 내림차순의 행벡터

?<t

R어.

,thlab矩m

1 2 3 4 5 6 7 8 9 m n

풀이

numa=5;

尸
H

dena= ]1 231 5] ;
ca=dena;
比＝11 10 弱 50 241 ;

-

Ta=routh(ca) ; 0
dlsp( " );
disp( ' (a) 日outh-Hur쁘itz Arr카／ ) ;
disp(Ta)

1
-

Tb=routh (cb) ; 0
비S口（ (b) Ass나） Hurwits Array ) ;
disp(Tb)

-

그림 +32 rxxith 함수를 이용한 안정도 판별 코딩 결과（Ro出ffable.m)

(a) routh 함수를 이용하여 전달함수 분모의 계수를 내림차순으로 지정한 행벡터 ca어］ 대한 안정도를 판별
한다（O).
(b) routh 함수를 이용하여 특성방정식의 계수를 내림차순으로 지정한 행벡터 cb어］대한 안정도를 판별한다

(O)

.

Command 叫indo川
>> flouthlable

D 0 0 n

(a) 日Dut h냐lu r뿌itz Array
1 .刃00
3. 0IXE
5. 0000
2．더刃0
1 . 0000
2. 5000
5. 0000
-3. 00t0J
0
5. 0000
0

35
50
24

42
24

0
0

n
d

1
10
30

4 0 0 0 0

(b) R그uth-Hurwitz Array

그림 +33 routh 함수를 이용한 안정도 판별 실행 결과

(a）의 결과는 1열의 3행과4행 사이, 4행과 5행 사이에서 부호가 두 번 바뀌므로 특성방정식의 두 근이 S 평
면의 우반평면에 존재하는 불안정한 시스템이다. (b）의 결과는 l열에서 모든 행과 행 사이의 부호가 바뀌지
않기 때문에 안정한 시스템이다．

CHAPTER 09 제어

227

=]n工｛
I_ Ill -,

07

궤적如cus）은 임의의 조건을 만족하는 모든 점의 집합을 말하고, 근(root)은 닫힌 루프 전달함수의 극점과 같은 특성방정식의
근을 의미한다. 그러므로 러忙1(root locus）은 다양하게 변하는 이득과 같은 시스템 매개변수를 사용하여 닫힌 루프 전달함
수의 극점 위치퓰 보여준다. MATLAB을 이용하여 다양한 전달함수에 대한 근궤적을 구하고 근궤적에서 이득 계수와 극점을
찾는 방법을 알아보자．
Keyword

I 근궤적 ] axis I riocus 1 cony I sgrid 1 rlocfind !

I 근궤적
［그림 아34］와 같은 귀환 제어 시스템을살펴보자．

山

（2

尺

C(s)>

1

H (s)
그림 아34 근궤적 해석을 위한 귀환 제어 人 스템

［그림 9-34］와같은 시스템의 닫힌 루프 전달함수는다음과같다. 이때 尺는 이득 꼐수（g鈿 factor）이다．
C(s)

KG(s)
1+ KG(s)H (s)

R(s)

(9.24)

(s

.

"

(s

)

+ Z
+ z1) + z2
m)
(S 十 Pi 乂S 十 /72J " " " (S 十 /77i J
(s

K

)=

(:
H

(s)

(s)

(:

KG
尺G

)j/

열린 루프 전달함수는 다음과 같다．
(9.25)

이때 m은 전달함수에서 유한한 영점의 개수이고, n은 전달함수에서 유한한 극점의 개수이다．
식 (9.24）로부터 닫힌 루프 전달함수의 특성방정식을구하면 다음과 같다．
1+ 尺G(s)尸(s) = 0

(9.26)

식 (9.26）으로부터 크기 조건（magn如de c血e加n）과 각도 조건（angle criterion）을 구하면 다음과
같다．

228

PART 03. MATLAB활용하기

(s)

H

(s)

G

I

I

=

4:

(9.27)

人

(9.28)

乙G(s）丑0) = 士1800

M-File I RtLocOpen.m

1 예제 9- 12
다음 열린 루프 전달함수에 대한 닫힌 루프 시스템의 근궤적을 그려라．

K

；而

尺G(s)1끄s') =
"
"
s(s+ 2)(s+ 4)

지식

' axis
axis 명령어는2차원공간에서工축과y축의크기를조정한다. 工축과y축을같은크기로조정하기 위한axis

명령어의 기본 형태는 다음과 같다．

ax治( 'equaI')

1riocus
전달함수의 분자num과분모 den어］대한 근궤적을 그리는riocus 함수의 기본 형태는 다음과 같다．

rlocus(num, den)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

num:
,l;
11 6801:
rI。
cug
;
grid:
e

1-

U R吐｛乂（긔呼m 놔브

：
니

小

m
b

0

4

n
/

4

8

axisCequal ;
xiabsi ( 'Reai axis ') ;
ylabel ( ' Imagiriary axis ') ;
t 나le( ' 而ot locus diagram ) ;
)

-

'

3
4 -

(numden)

,0

des=

2-

푤이

1

그림 +35 근궤적 그리71 코딩 결과（R七cOpen.n今

0 닫힌 루프 시스템의 분자 계수를 내림차순으로 지정한다．
0 닫힌 루프 시스템의 분모 계수를 내림차순으로 지정한다．
0 riocus 함수를 이용하여 전달함수의 분자num과 분모 den어］대한 근궤적을 그린다．
0 axis 함수를 이용하여 그려진 근궤적선도의 가로축과 세로축 크기를 같게 조정한다．

CHAPTER 09. 제어

229

F艇

Ed健

\/15W

Insert

그d a 可 臣

（刃jO

E沁毖t叩 蜘너m

거

F蜘1

' \ \ 好 自咽 / , 目 日 툐크 a 口
Ri帥 bd月di끼甲mn1

15

5

：귿8邕쓰쥬간m드m쁠1

0

0
巧
10

-IS

-20

-15

-10

-5

0

5

10

IS

Real 日xis (se口가넘8'1)

그림 아36 근궤적 그리71 실행 결과

근궤적은 극점（S = 0, S = 크, s= -4）에서 출발하고 실수축에 대해 상하 대칭이다 ．빨강 ，초록 ，파랑으로
나타난 근궤적의 분기 (branch) 수는 3이며, 이는 열린 루프 전달함수의 극점 수와 같다. 또한 실수축에서
근궤적이 존재하는곳은 크 드 S 드 0, 5 드 戶4이다．

M-FiIe 1 RtLocGain.m

1 예제 9- 13 1

다음 열린 루프 전달함수에 대한 근궤적을 그리고 ，감쇠비가 C = 0．6인 경우의 이득 계수 尺를 구하라 ．그리고
근궤적과 감쇠비 직선이 접하는 점을 찾아라．
K(s2 -6s +34)
(s + 2)(s + 6)

배명
지식

1cony
다항식p아yl과poly2를곱한결과인다항식叩를내림차순으로나타내는cony함수의기본형태는다음과
같다．

＼사 = conv(p이yl! p아y2)
·w: 두 다항식을 곱한 결과
· P이yl, p이y2: 곱할 다항식

1sgrid
riocus 함수에 의해1 이미 생성된 근궈怪1 위에 감쇠비 c와 고유주파수 O,fl의 선을 그리는 sgrid 함수의 기본
형태는 다음과 같다．

230

PART 03 卜／ATLAB 활용하71

sgrid(zeta,om的乞n)
· zeta: 감쇠비
' omega_n: 고유주파수

1rio（浜nd
riocus 함수어］ 의해 생성된 시스템의 근궤적과 감쇠비 직선이 접하는 점을 선택하여 이득 계수 兀와 극점
poles를 얻는rlocfmd 함수의 기본 형태는 다음과 같다．

[K, poles] = rlocfind(num,den)
. K: 이득 계수
= p이es: 극점
·num: 입력 전달함수의 분자 계수를 내림차순咀 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

lIRtLO＜好a沇m 捉T目
num=11 -6341;

1-

den=corw([l 21, 11 51) ; e
시ocus(nu日，den); e

叫

3-

2

axis(卜7 4 -6 61) ;

5-

4-

serid(O.6, 11),; 0
1K,p。Iesl rIccfind(num,den) 0

6-

그림 +37 이득 계수와 극점 생성하기 코딩 결과（R七)cGain,m)

0 COnV 함수를 이용하여 열린 루프 전달함수분모의 인수분해 항을 전개하지 않고 변수S에 대한 내림차순
으로 다항식을 계산한다．
0 riocus 함수를 이용하여 근궈쩍을 그린다．
Osgrid 함수를 이용하여 그려진 근궈쩍선도에 감쇠비와고유주파수의 선을 그린다．
0 rlocfind 함수를 이용하여 이득 계수와극점을 구한다．
0陋

든d比

Vk？叫

Io5ot

亡J 口 w $ 三 七 \

30어丘

0e$kt아）

。1 自i

Wk心D놔

MI巾

Jf , 盈 目 g3 I. 心
R｛刃iL刃口后

흖

'

貫

H

0

!-2

극
）
.6

景이

.7

心

느6

.4

-3

中2

-T

0

3

2

3

4

Re씨 缸b (se口1月油勺

그립 아38 선택된 한 점

CHAPTER 09. 제어

231

出1翩t To벼S

m5kk耳1 帥1出批

H的口

뜬；) 心｝ a 蜘 L뇹 '\ '\ 助 匈 曜 而 , 鼠 ! 口 匡크 1 口1
Root Locus

2
0
2
gq듬晷나뽀준之m드담트
4
-4

-3

-2

-1

0

1

R的IA烟 r羽con由' 1)

그림 아39 근궤적과 감쇠비가 만나는 지점

｛그 t3 日 曲 L뇽 i ：曳 民 聊 匈 咽 戶＝ , 昆 ［그 圓 U 口
F之이幷 Loct后

2
0

그

r뇽듬晷나m妾之量留至
.8

4
.7

好

何5

-4

-3

-2

-1

0

1

2

Real A岫n明刃耐r}
그림 아40 근궤적의 허수축 교차점

［그림 아38]).
加efind 함수를 이용한 R比ocGain.m 파일을 실행하면 십자선 커서가 그림 창어］나타난다（
이 십자선을 이동하여 근궤적과 감쇠비 직선이 만나는 한 점을 선택하면 나머지 접하는 점도 자동으로 빨간
'X '로 나타난다（
［그림 아39]). ［그림 +38］과［그림 아39］의 과정을 반복하여 ［그림 아40］과 긷이 근궤적
의 허수축 교차점을찾는다. 이때 그림의 파란 ' >< ' 표시는 전달함수의 극점이고, 파란 ' O ' 표시는 전달함수의
영점이다．
m}

근궤적과 감쇠비 직선이 만나는 지점을 마우스 커서로 정확히 지정하기가 쉽지 않은데, 가능한 한 가깝게 접근한
다음 클릭하면 정확도에 따라서 실제 계산한 이득 계수와 극점값에 일치하게 된다．

232

PART03. MAT냐＼B활용하기

do七가

'> RtLocGain
Select a 口01st in the graphics 비cdt밖
selected...point =
-3.5201 * 3. 97521

K
0. 27田

psi en =
-2.印17 * 3. 23271
-2. 5017 - 3. 23271
그림 +41 이득 계수와 극점 생성하기 실행 결과

［그림 아41］은 근궤적과 감쇠비 직선이 만나는 임의의 한 점을 마우스로 클릭한 후 나타나는 결과이다. 되
도록 근꿰적과 허수축의 교차점어］정확히 마우스 커서를 놓고 클릭하면 이 선택된 점어］ 의해 자동으로 생성
된 근퀘적의 허수축 교차점은 士／4.9549이고, 이득 계수尺는 1.3282이다. 그러므로 이 제어 시스템은 이득이
1.3282보다크면불안정해진다．

CHAPTER 09, 제어

233

LESSON

08

주파수응답

시스템의 주파수 응답은 정현파 입력 신호의 정상상태 응답이다. 주파수 응답 방법의 장점은 시스템의 전달함수를 주파수 응
답 검사에 의해 실험적으로 결정할 수 있다는 것이다. 설계자는 주파수 영역에서 시스템 설계를 통해 시스템 대역폭과 시스템
응답에 발생하는 잡음, 방해를 조절할 수 있다. 선형 시스템에서 주파수 응답은 시스템의 전달함수를 통해1 이론적으로 계산한
다, MATLAB을 이용하여 주파수 응답의 보드선도를 그려보자．
Keyword

I

I 주파수응답 1 보드선도 1 t兀de I 卄eqs I an이e I sem的gx I semilogy 1 打gure I

주파수 응답

주파수응답（frequency resp아哨e）은 닫힌 루프 시스템의 전달함수 G(s) 어］ 정현파 입력 r(t) = Asino万
를 가했을 It下1, 전달함수의 식에서 S =JW를 대입하여 얻는 주파수 전달함수 G(jw)의 절댓값과 위상각을
이용하여 구한다. 즉 입력 주파수 w의 변화에 대한 진폭비 (ampi奴ide rati이 四(jw) I와 위상차（phase
difference) 乙G（和))의 변화를주파수 응답이라고 한다．

I

보드선도

보드선도（bode diagram)는 가로축이 log co이고 세로축이 데시벨 값인 크기 IG(jco) I 의 주파수 응답
과 가로축이 log w이고 세로축이 위상각 乙G(jw) 인 주파수 응답을 그리는 선도를 말한다. 이때 이득은
데시벨 [dB］로 나타내며 다음과 같이 계산한다．
20 log10 1 G(joi) 1

(9.29)

r町＝File 1 다eqResp.m

1 예저19-14 1
주파수 0 5w 드 5 [radls］에서 닫힌 루프 전달함수 G(s）의 주파수 응답을 구하라．
G(s) =

4
S二 + 2s + 4

而胛

口 bode
주파수 범위와 점의 수를 자동으로 선택하여 시스템에 대한 주파수 응답의 보드선도를 그리는 加de 함수의
기본 형태는 다음과 같다．

234

PA日T03. MATLAB활용하기

bode(num, den)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

진폭 mag와 각도 phase로 나타내는 위상 응답을 찾아 보드선도를 그리는 bode 함수의 기본 형태는 다음과
같다．

[mag, phase] = bode(num,den,omega)
· mag: 진폭
· phase: 각도
·num: 입력 전딜함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터
' omega: 각주파수

三

1 R쩍好esp.m

e
e
e
1
e
寸
H

뉘 帥日1 ( 깹0s日ea ) ;

m

미 abel (Phau日 " ) ;

m

grid;

4

미ot（毗ga, phase) ; 0

1

elahel ( 半seega );
ylabel ( Magnitude ) ;
it I e( Frequency Response) ;
grid;
subp lot ( 21 2) ;

m

plot (omega,mag); 0

m

omega=0: 0괴 巧；0
]mag, phase] bode (numden,omega) ; C
8ubp10t (211) ;

呵

m

num=4; <1
den=]1 24] ; 0

m

123 45678 gm n促m닉侮

풀이

그림 아42 주파수 응답 구하7j 코딩 결과乍尼qResp.m)

0 전달함수 G(s）의 분자 계수를 내림차순으로 지정한다．
0 전달함수 G(s)의 분모 계수를 내림차순으로 지정한다．
0 주파수 U刈 범위를 지정한다．
0 加de 함수를 이용하여 전달함수의 크기와 위상을 자동으로 구한다．
0 전달함수의 절댓값 I G(jw) I를 그림 창 위쪽에 보드선도로 그린다．
0 전달함수의 위상각 乙G(j（끼를 그림 창 아래쪽어］보드선도로 그린다．

CHAPTER 09. 제어

235

F湘

Ed在

jj

d 白 L뇹 ' \

Vtew

Issert I喇S

O小比斗1

V니n小：汭Y

He巾

\ 鉀｝ 孕 뚜근 而 r 邑 ［그 匡크 日 口
Frequency Response

0
쁨글旨m듣
2

1.5

2

2,5

3

35

3

35

4

4.5

4

4.5

U

1.5

拓

1

n
/

0.5

m
\
\
\
\
\
1
1
1

伽

m
m
m
二
n

枷
跏
05

5

k7

그림 +43 주파수 응답 구하71 실행 결과

시간 응답은 입력을 가한 직후에 나타나는 과도 현상에 중점을 두지만 주파수 응답은 정상상태1 출력어］중점
을둔다．

M＋加 1 Bode［긔ag.m

1 예제 9너5 1

전달함수가（和）인 시스템에 대한 주파수 응답의 보드선도를 그리되, bode 함수를 이용한 경우와 이용하지
않은 경우를 각각 그려라．

；而
지식

(s+

=

(s)

2)

G

3O(.v + c

(s+ lO)

' 僉eqs
전딜함수q勺에대한복소주파수벡터G（和D를찾는取那함수의기본형태는다음과같다．

G = freqs(num, den, omega)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터
· on冶ga: 각주파수

1angle
복소수 배열 x어］대한 위상칵을 라디안값으로 나타내는 an멤e 함수의 기본 형태는 다음과 같다．

an이이지
. X: 복소수 배열

236

PART 03. M月r녀B촬용하71

1semilogx
semilogx 명령어는x축만을 로그 눈금으로 그린다. sen血ogx 명령어의 기본 형태는 다음과 같다．

sem加gx似！y)

1semilogy
semil略y 명령어는y축만을 로그눈금으로 그린다. semilogy 명령어의 기본 형태는 다음과같다．

sen｝加gy似y)

1figure
figure 명령어는 MATLAB 그래프 여러 개를 각각 다른 그림 창에 그린다. figure 명령어의 기본 형태는 다
음과같다．

figure(n)

Bode마agsT) 蔑 Hi너
H] s=t1( s );

旨

Gl=30*(s.5) /( (s+2)*(s*lUfl; <1
-

1
1
1
1
1
1
1

semi logo（口mega, 20니09山（may) ) e

e
H
1
1
1
1
m

grid;
ylabel ( Magnitude (dB) );
title( 日口do ［기 a日ram ) ;
so印山t (212) ;
semi logx (omega』phame. (180/pi) ); 0
grid;
olabel (Frequency (Rad/s) );
미abel ( Phas日 (dee) ) ;

1

02=treqs (num』deo, omega) ; 0
mag=abs (02) ; 0
phase=arigle(02) ;
subplot (211) ;

H

figure (2) 0

num=3口니0 1 5) ;
den=coov( (1 21 . )1 1W) ;
omega=0. 1 :01: 1e3;

1

grid;

1

tigure (1) 0
bode (01) ; 0

1

3 45 6 7 B 9 m n 口 日 m侮 出 W m 四m 기刃
2-

풀이

그림 아44 보드선도 그리기 코딩 결과（B어把미ag.n)

0 전달함수 G（刃를 직접 입력한다．
0 bode 함수를 이용하여 보드선도를 그리는 경우, 두 그림 창을 동시어］ 보여주기 위해 figure 명령어를 사
용한다．
0 bode 함수를 이용하여 보드선도를 그린다．

CHAPTER 09. 제어

237

0 새로운 그림 창을 연다．
0 行eqs 함수를 이용하여 전달함수 G(s）를 지정한다．
0 bode 함수를 사용하지 않을 때는 전달함수의 크기와 위상이 자동으로 생성되지 않기 때문어］ abs 명령어
와a璡le 함수를 이용하여 주어진 전달함수의 크기와 위상을구한다．
0 semil唯x 명령어를 이용하여 工축을 로그함수로 지정하고, 크기를 이득 형태로 지정한다．
0 semilogx 명령어를 이용하여 工축을 로그함수로 지정하고, 라디안 단위의 주파수를 각도（degree) 단위
로 변환한다.
＼가的V

D t3 너 白 自

1n9猷

To아5

Deskt야） ＼사ire主J出r

He巾

' \ '\ 抑 匈 唯j 而 r 匹口 ［그 匡1 困 口1
Bode Diagram

0
札
加

八g므留쁜4

"

100

「 ',
\,,\1

小띰나m召長留＞

5

l{)1

102

1o3

Fre口U이也V fta出引

그림 아45 比de 함수를 이용하여 보드선도 그리기 실행 결과

그림 아46 bode 함수를 이용하지 않고 보드선도 그리기 실행 결과

［그림 아4引에서 축의 범위는日0 듸 G(／
이 匡 20[dB］과 0O< 乙G(jco) 5 -90"이지만，［그림 아46］에
서 축의 범위는 놔0 듸 G(jw) 注 20{dB］과 0O< 乙G（加D 5 크00"이다. bode 함수를 이용하여 보드선도
를 실행한 그림과bode 함수를 이용하지 않고 보드선도를 실행한 그림의 크기와 위상 제한 범위를 동일하게
설정하면 두 결과가 같음을 알수 있다．

238

PART 03. MAT녀B활용하71

LESSON

09

나이퀴스트선도

주파수 응답 방법인 나이퀴스트 분석은 기본적으로 닫힌 루프 제어 시스템의 절대 안정도와 상대 안정도률 결정하는 데 열린
루프 주파수 응답의 그래프를 이용한다. 루스1후르비츠 안정도 판별법은 직접 안정도 결정에만 사용된다는 제한이 있지만, 나
이퀴스트 판별법은 특성방정식에서 변수 S로 표현되는 시스템에 적용할 수 있다. 또한 나이퀴스트 판별법은 실험적인 주파수
응답 자료에서 시스템의 전달함수에 관한 정보를 얻는 데에도 유용하다. MATLAB을 이용하여 나이퀴스트선도률 그리는 방법
을 알아보자．

Keyword

I

1 극좌표그래프 ! 나이퀴스트선도 I nyqu暾 1

극좌표 그리但

극좌표（p아ar) 그래프는 주파수가 0에서 무한대까지일 때의 진폭과 위상각을 나타낸다. 이때 사용히는
극좌표 형식은 다음과 같다．
G(jw) 늬 G(jw) 1 乙G(jco)

(9.3이

식 (9.30）을 직교좌표 형식（복소 형식）으로 변환하면 다음과 같다．
G(joi) = Re{G(joi)} + jlm{G(jco)}

(9. 꾜 )

그러므로 G(jcv）의 극좌표 그래프는 m <m＜的에서 G(jw) 평면의 유한 부분 Tm {G(jw) }에 대한
Re {G(jw) }를 나타낸다．

I

나이퀴스트선도

나이퀴스트선도（Nyq邸t 曲gram)는 주파수의 값어］따른 열린 루프 전달함수의 크기와 위상을 극좌표
상어］ 표시한다. 나이퀴스트 판별법은 벡터궤적을 이용하여 특성방정식의 영점이 우반평면어］존재하는지
판별하는 것이다. 이때 S 평면에 놓여 있는 점의 궤적이 나이퀴스트선도 내에 있는 G(s) 평면으로 사상
(mapping）된 것을 나이퀴스트 경로라고 한다. 이 경로는S 평면의 전체 우반평면을 완전하게 에워싸는
곡선 형태 (contour）이며, 제어 시스템이 안정하려면 특성방정식의 근이 모두 음의 실수부여야 한다．

CHAPTE日09; 제어

239

難卜斜掩 ! NyquCrit.m

1 예제 9蜘唾各 量

단위 귀환 제어 시스템에서 열린 루프 전달함수 （耶）의 나이퀴스트선도를 그리고 시스템의 안정도를 결정
하라，

3s

+ 5s+ 1

nyquist

'c

;ii

'

3

-

,
s 3+O. ,
0.

(s)

G

l
=

지식

주파수 범위와점의 수를 자동으로 선택하여 나이퀴스트선도를그리는nyquist 함수의 기본 형태는 다음과
같다．

nyquist(num, den)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
.den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

이때 가로축과 세로축의 이름은 nyqu胤 함수에 의해 자동으로 생성된다．

풀이

quCr花01

烈! + ]

nun,=[0 00 I] ;
der,=(1 0. 35 I I ;

(Nyquist

e

H

p比t ) ;

n

title

H

0

nyqU1st (num, den)
axis(j- 3 3 -2 2] );
grid;

그림 +47 나이퀴스트선도 그리기 코딩 결과（NyquCritni)

0 nyqui亂 함수를 이용하여 나이퀴스트선도를 그린다．
0 title 명령어를 이용하여 나이퀴스트선도의 제목을 입력한다．

口口 A 出

L늉 戈 戈 吻 今 啞 d , 曼 口 國 口口

그림 앍48 나이퀴스트선도 그리기 실행 결과

S 평면의 우반평면 위치어］ 열린 루프 극점이 2개 있고 임계점 (en如a! point）을 에워싸지 않으며，위 그래프
의 벡터궤적이 원점을 내포하고 오른쪽으로 돌기 때문에 이 제어 시스템은 불안정하다．

240

PA딕T03. MAT녀B 활용하기

니콜스선도
니콜스선도는 주파수 응답에 바탕을 둔 나이퀴스트선묘｝보드선도를 응용한 방법이다. 니콜스선도는 귀환 시스템의 닫힌 루
프 주파수 응답과 안정도를 결정하는 유용한 기술로, 기본적으로 극좌표 그래프상에 있는 M 원형과 』V 원형을 직교촤표의 위
상 축과 데시벨 크기 축에 비원형 A／과 N 카운터로 변환한다. MAT냐侶을 이용하여 니콜스선도를 그리는 방법을 알아보자．
I 니콜스선도 1 nich이S I

Keys사ord

니콜스선도

I

열린 주파수 전달함수 G(和))의 이득 20 log IG（和D 1와 위상칵 乙G(jco）가 주어졌을 때, 닫힌 루프 주
파수 전달함수 MOw)의 이득 2010g jjJ丑加D 1와 위상각 ＝小仄肋의 관계를 나타낸 그래프를 니콜스선
도（Nich아s chart)라고 한다．

M-File I NichCtit.m

1 예제 9- 17 1
단위 귀환 저뻐 시스템0私1 열린 루프 전달함수 G(s）의 니콜스선도를 그려라．

G(s) = .

'S

1.

-.

지식

'

nich아S

；而

跌S 十 I乂S + 3)

주파수 범위와 점의 수를 자동으로 선택하여 시스템어］대한 니콜스선도를 그리는 nich아S 함수의 기본 형태
는 다음과 같다．

nich이s(n내11, den)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터

I NichCr花m 3: ]

1 23456-

+"

풀이

:

이때 가로축과 세로축의 이름은 nichols 함수에 의해 자동으로 생성된다．

nura=[0 00 61;
den=coriv (conv(]l 0] . [1 11) . 11 31) ;

田

nichcls(num』den) 0
axis(卜270 0 -30 40] );
grid;
title ( NicholsPlot ) ;0

그림 아49 니콜스선도 그리기 코딩 결과（N耐Cntm)

CHAPTER 09 제어

241

0 nichols 함수를 이용하여 니콜스선도를 그린다．
0 title 명령어를 이용하여 니콜스선도의 제목을 입력한다．

그림 아50 니콜스선도그리7I 실행 결과

242

PART03. M戶TLAB활용하기

CHAPTER

신호 및 시스템

CONTENTS
LESSON 01 신호
LESSON 02 이산 시스템
LESS아J 03 컨벌루션
LESSON 04 샘플링
LESS아寸 05 신호 복원
LESSON 06 연속 신호의 주파수 표현
LESSON 07 이산 신호의 주파수 표현
LESSON 08 라플라스 변환
LESSON 09 z 변환
LESS아1 10 디지털 필터

LESSON

01

신호

신호帥n帥는 하나 이상의 시간을 독립변수로 가진 함수로, 다양한 물리적 현상의 동작과 성질에 관한 정보를 표현한다. 연
속적인 시간에 대해1 끊7休1 않고 나타나는 신호를 연속 신호라 하고 ，특정한 시간에 띄엄띄엄 나타나는 신호를 이산 신호라 한
다. MATLAB의 그리기 기능을 이용하여 다양한 입력 신호에 대한 이산 신호의 출력을 살펴보자．
Keyword

1 정현파함수 1 싱크함수 I s也m 1 stepfun I sub히아 i 임펄스함수 1

I 정현파 합수
연속 신호（continuous-t恤e signal)는 시간과 크기가 모두 연속인 아날로그 신호（analog signal)와
함께 사용하기도 한다. 일반적으로 연속 신호에서 함수工어］대한 시간 변수는 x(t）로 나타내며, 다음 조
건을 만족하는 연속 신호 工（t）를 기본주기가 T인 주기 신호라고 정의한다．
x(t) =x(t+kT),

k= 1, 2, 3,．··

(10.1)

대표적인 연속 주기 신호인 정현파 함수（sinusoidal function）는 다음과 같다．
x(t) = Acos(｛刃t + 砂）

(10.2)

진폭 A는 정현파 함수가 진동하여 가질 수 있는 값의 범위, 각주파수 U)는 단위 시간어］ 정현파 함수가 이
동할수 있는 각을 라디안으로 표시한 값, 위상 中는 시간 0에서 정현파 함수의 출발 위치를 결정하는 각
이다．

1 예제 伯너 1

M- Fite i ConSinus.m

진폭 A =2, 주파수凡 =2.4[H기, 위상 中 = 60"인 정현파 함수 x(t) 의 파형을 그려라． 파형의 시간축은
-1 드 t 5 I [sec］이고 0.01초씩 증가한다．

244

PART03. M／玎LAB활용하71

玎1 -

co哨inE丘m

t=-I :0.01 :1;
A=2;
fo=2. 4;
omega=2.pi.f0;
口hi=60士p1/IS0;
xt=A*cos(omepa*t*phi) ; <1
口比t (t,mt) ; 0
arid;
xIabeI ( 'Tme (t) );
ylabel ( xlt) );
씨tle(Sinu드olda 引moo匕 Acos冊cm日gat*毋口hi) '); 0

2345
67H
891011 -

그림 1O너 정현파 함수 그리기 코딩 결과(ConSinus.m)

0 정현파함수x(t）를지정한다．
0 정현파함수x(t）를그래프어］나타낸다．
0 문서 조판에 사용하는 레이텍（LaTeX) 프로그램으로 정현파함수 工（t) = Acos（毗 ＋中）의 그리스 문자
Ct)와中를 나타내기 위해 \O毗ga와＼phi를 입력한다．
1ll}
F沁

MATLAB에 내장된 레이텍 프로그램을 이용하면 수식과 수학 기호를 입력할 수 있다．
Ed弦

\Flew

그 1J d 出

lnget

뉵

.0.8

TO捌5

Deskt아｝ 쌔ndaw

1目p

' \ '\ 抑 匈 咽 寸＝ 기 晶 口 因 吸 口

.0.6

也4

.0.2

0

0.2

04

0.6

0.8

그림 10中2 정현파 함수 그리기 실행 결과

I

싱크 함수

정현파 함수처럼 동일한 파형이 지속적으로 반복되는 신호를 주기 신호（per幻dic signal)라 하고, 동일
한 파형이 반복되지 않는 신호를 비주기 신호（aperiodic signal)라 한다， 연속 비주기 신호의 대표적인
함수로는싱크함수（sinc 血nc如n）가 있다. 싱크함수는사인 함수와그 인수（argument)의 비로 나타
내며, 다음과같이 정의한다．

CHAPTER 1O. 신호 및 시스템

245

,m.(r)
sinc(t) = sin(兀t)

(10.3)

7rt

식 (10.3）의 푸리어］ 변환이 구형 함수（rectan叩lar 凡nction）이고 그 적분값이 동일하기 때문어］ 정규
화된 싱크 함수라고 일컫는다．

乳昏켜斜油 ! ConSinc.m

1 예제 10- 2 1

끊0씩증가O는파형의시간축4兀< t< 4兀［Sec］에서 싱크함수의파형을그려라．
rcc,
1-

풀이

！丘쯔

m 弑 =1
t=-4士p1 :p 7弱0：肛pi ;

2-

xt=sin(pi士tL/(pi.t); 0

e

4-

xt)

3-

plot(t,
;
axis(1-.4*pi 4.pi 也3 1.21) ; 0

8-

7-

6-

5-

9rid;
p.IabeI (11m8 (t) );
미 ab이 (x (t) ) ;
title (Sinc 듸 gnaI : 引 n（枷 it U伽it ' ) ;

그림 10田 싱크 함수 그리71 코딩 결과（Co困兀．m)

0 배열 연산자를 이용하여 항목별 나눗셈을 실행한다．
0 plot 함수를 이용하여 싱크 함수를 그래프에 나타낸다．
0 axis 명령어는 반드시 plot 명령어를 실행한 다음에 사용한다．
F41e

Edit

\/ie叫

‘口 心｝ a 由

m5因t 1O,比
t눋

出n小J畔

f+e41口

' \ '\ 抑 匈 嚼 戶g · 昆 口 區

團口

昏ncS也na比in佃t蜘II

&
그림 10-4 싱크 함수 그리기 실행 결과

246

PART 03.卜肛TLAB활용하71

10

I

이산신호

이산 신호（discrete -time signal)는 시간과 크기가 모두 이산적인 값인 디지털 신호（d培佃1 signal)와
혼용하기도 한다. 일반적으로 이산 신호에서 함수工어］대한 시간 변수는玎미 으로 나타낸다. 신호값히 발
생한시간또는순서를 나타내는n은 항상 정숫값이다. 이산주기 신호는 다음과긷히 정의한다．
工［n＋无N]＝工［n],

丸＝···，-1, 0,1, 2, ..·

(10.4)

식 (10.4）를 만족하는 가장 작은 N 값, 즉 파헝이 반복되는 최소 시간을 기본 주기 (fundamental
period）라고 한다. 이때 식 (10.4）를 만족하는N값이 존재하지 않는 신호를 이산 비주기 신호라고 하
며, 이산신호 정현파함수는다음과같이 나타낸다．
x[n] = Acos(orn +0)

(10.5)

여기서A는진폭, U)는각주파수, 0는위상칵이다．

秘卜斜油 i 미sSEnus.m

1 （눼저I 1fl- ．1크 i
L二二＝二＝J

21개의 지속적인 표본을 가진 이산 정현파 함수 玎미의 파형을 그려라. 이때 진폭 A= 1, 각주파수 co= 0.5,
위상 0= 2이다．

i而
지식

' stem

工어］ 의해 지정된 값으로 생성되는y의 자료값을 줄기 형태의 그래프로 나타내는 stem 함수의 기본 형태는
다음과같다．

stem(x, y)

1

［汁ISift上sm

-

-

}r

5=21;
1;

omega=0. 5;
theta=2;
n=0:N니 ;

xn＝肛cos(o.ega..n 'theta); q1

stem
grid;
(n,

-

A=

1234567B9mn

푤이

xn) ;

e

xlabel (Time [ri] );
ylabel ( < [n) );
title (Sinus口ida! 돼 anal : Acos（寸加flies an＋卄theta) ) ;

그림 10-5 이산 정현파 함수 그리기 코딩 결과（DbSnus.m)

0 x[n]을 지정한다．

CI-IAPTER 10. 신호 및 시스템

247

0 stem 함수를 이용햐：셔 21개로 지정한 기본 주기 N의 개수만큼 입력값 刃을 지정하고 이 값어］ 의해 생성
되는 출력값 玎川을줄기 형태로 그린다．
F沁

Ed捷

inw

lOse作

TO아5

D心岫op

Win由w 卜似p

D 1 d 41 自 ' \ "\ 劫 自 唯｝ J= , 艮 i 口 國 匹 口1
텨TUS아daiS呻目l: Aco햐Un+e)
0.8
0.6 1
0.4 2
0
0

H
드
乂

-0.4
-0.6
.0.8
-1

6

8

10

12

14

16

18

入1

Tin衿 [ni

그림 10-6 이산 정현파 함수 그리기 실행 결과

이산 신호 단위 계단 함수

I

여러 종류의 신호를 표현하는 데 매우 유용한 단위 계단 함수（unit step 凡nction）는 다음과 같이 정의
된다．
. ,
fi
uLnj= \ n
IU

(n之0)
'\.
(n.(U)

M-F加 1 DisUstep.m

1
1 에xi in．口＝LI. 'I
=

"

"

"

'

V

'

신호값이 발생하는 시간

5< 刃 5 5[sec］에서 sub이아 명령어를 이용하여 단위 계단 함수 U［川과, u[n]을

；而

시간 2만큼 이동한 단위 계단 함수 工[n] = u［刃 H기의 파형을 그려라．

지식

' stepfun
단위 계단함수를시간加만큼이동하는stepfun 명령어의 기본형태는다음과같다．

stepfun(n, nO)
. n: 시간을 나타내는 변수
·nO: 지연시킬 시간

口 subpi야
그림 창을분할하여 여러 그래프를 그리는S的plot 명령어의 기본 형태는다음과같다．

248

(10.6)

PART 03. MATLAB활용하71

subplot(mnp)
.m: 그림 창 안에 분할하려는 행의 수
· n: 그림 창 안에 분할하려는 열의 수
.p: 그래프가 나타날 위치

ID告뗘把pill 寸씨
1 -

n=-5:1 : 5;

ustep_n=stepfun(n, O); e
an=steptun(n,2); 0
H

3 4 5 6 7 8 9 m H 俚 侶 H 佰 比 行

2-

m

subplot (211); e
stem(n, ustep. .n); e
m
m

axis(E-5 5- 0; 5 1 .51) ;
arid;
xlabel (Time )n] );
미帥引 ( 七 En) ');
4
1
U
H

tit le( ' Un it Step Si anal : u in) ) ;
subplot (212) ;
m

0

(n,

斗

stem
xn) ;
a川 si［巧 S 中0. 5 1 .5) );
arid;
+
1
H

xlabel ( 'Time En) ') ;
미 ab引 (. Mn] ' ) ;
it le( Unit Step Si anal : a En-21 ');
1
1

그림 10-7 단위 계단 함수 그리71 코딩 결과（D烈始衿口.m)

0 단위 계단함수川미을 지정한다．
0 step丘in 명령어를 이용하여 단위 계단함수를오른쪽으로2만큼 이동한u[n-기를 지정한다．
0 두 단위 계단함수를 비교하기 쉽도록subi加t 명령어를 이용하여 그래프를 위아래에 나타낸다．
0 stem 함수를 이용하여 u[,日을 줄기 형태로 그린다．
0 stem 함수를 이용하여 u[n-기를 줄기 형태로 그린다．
File

Ed往

V降＼v

lIne作 no毗

D 亡｝ A 由 L뇽 ' ,

Desktop ＼付ire幻畔

늬

Mel

\ 4'} 自 咽 而 , 盈 目 目

口

Unit Step＄呼mh 바n}

1.5

O
0.

좋 5
0
4L5
-5

-4

-3

-2

-4

-3

-2

1.5

-1

0
1
Time [nE
Unit Step Signal: u(n-2)

1

투 5
0.

풀이

0
.05
니5

-1

0
丁如帑 [n]

5

그림 10田 단위 계단 함수 그리기 실행 결과

CHAPTE目 ]U. 신호 및 시스템

249

0보다 크거나 같은 모든 정수 n어］ 대한 단위 계단 함수의 크기는 l이고, 2보다 크거나 같은 모든 정수 n에
대해 오른쪽으로 2만큼 이동한 계단 함수의 크기는 l이다．

I 임펼스 합수

(10.7)

0)
。

1。

(n

=

S[

n]

5

(n;

11

=

[4]

임펄스함수伍Tipulse function）는특정한단위 시간의 파형을추출할때 사용하며, 다음과긷이 정의한다．

)

계단 신호를 이용하여 임펄스 함수를 다음과 같이 표현할수 있다．
8[n] = u[n] - u[n -1]

1 예제 10피

(10.8)

M-F扼 I Di읽m口ulse.m

신호값이 발생하는 시간 巧 드 n 드 5[sec］에서 단위 계단 함수를 이용하여 임펄스 함수 하끼의 파형을 그려라．

O附n叩K虧eJ1l

1

풀이

n
< n
J

나

?{ 三 +

n=-5:l :5;
ustep. .n=step{un(n,0); 0
ustep口nl=st日口fun(ni); 0

4

u省j,1; 0
- xnustep.
stem(n,xn);
.n- 0

드
니
6
n
r

as始（
［占 5 七．5 1 .5J) ;

8

grid;

口니

川abeI (Tiee [ni ) ;

小

-

IabeI ( 'n[ n] );
title ( IepuIse 引9nal : 甘deItainI =u[ni-u)n시1 ) ;

그림 10-9 임펄스 함수 그리기 코딩 결과（D崗m口내sem)

0 단위 계단함수 u[n]을 지정한다．
0 stepfin 명령어를 이용하여 단위 계단 함수를 오른쪽으로 1만큼 이동한U［刃크］을 지정한다．
0 식 (10.8）을이용하여 임펄스함수를지정한다．
0 stem 함수를 이용하여 임펄스 함수의 출력값을 줄기 형태로 그린다．

250

PART 03. MAT냐＼B활용하기

F퍼kg

田弔t

Ww

:a (3 a 鈿 IF
1.5

h15甘t

T며升5

먀sic따卜

쌔r岫汁

H目p

\ ' \ 好 厄1 是 d ' 匹 i ［그 匡크 因 口
Imp내韶 $ugnal: 印小＝바n)-ujn川

O

HC立

0.5

0

.2

.1

0

1

3

4

5

Tin始 [nj

그림 化너0 임펄스 함수 그리71 실행 결과
임펄스 함수는 시간 0에서만 그 값이 l이고 그 외의 모든 시간에서는 0이다．

CHAPTER 10. 신호 및 시스템

251

LESSON

02

이산 시스템1

이산 시불변 시스템과 시변 시스템을 MATLAB 그래프 그리기 기능을 이용하여 살펴보자．
Ke恥사ord

! 시불변 시스템 i 시변 시스템 1

I 이산 시스템1
이산 시스템은 이산 신호를 입력한후 어떤 조작이나 연산을 수행하여 이산 신호를 출력하는 장치 또는 알
고리즘을 의미한다. 이는 입출력 관꼐어］따라 선형 시스템과 비선형 시스템으로 분류하거나, 입력되는 시
간과상관없이 같은 입력어］대해 항상 같은출력 반응을 보이는 시불변 시스템과 그렇지 않은 경우인 시변
시스템으로 분류한다. 그 밖혜도 인과 시스템과 비인과 시스템, 안정 시스템과 불안정 시스템, 기억 시스
템과 무기억 시스템 등으로 다양하게 분류할수 있다．

I

시불변 시스템1

입력이 玎미 이고 출력이 y[n] 인 이산 시스템에서 시간이 k만큼 지연된 새로운 입력 玎刃十k] 어］ 대한 시스
템 출력 특성이 바뀌지 않으면 시불변 시스템（血iie-invari缸 system)이라고 한다. 시불변 시스템은 시
간어］대해 출력이 변하지 않으므로 지연된 출력 y{n寸匐는 y[n］과같은 형태이다．

M＋加 1 ［거slnvSys.m

［갠：쯔＝
：二二J
이산 신호 玎川이 단위 계단 함수일 때 입출력 관계가 다음과 같은 시스템이 있다．
y［미 = 工［n] - 工［n -2]

신호값이 발생하는 시간 0< 刃 5 5 [sec］에서 시스템의 파형을 그리고, 이 시스템이 시불변 시스템인지 시변
시스템인지 판별하라．

252

PART03. MATLAB활용하기

H
e
1
1

subplot (211) ;

1

O

1
1
U
U
m

stem
;
axis([ 0 6 0 2] );
川abe1 ( ‘끼me En] ) ;
비abel] ' yEn] );
title ( uEn] - u]n-2] 1;
nubp lot ( 21 2) ;
n)

m

y_n=x_n-x_s2; 0
九nk=x_nkl尸X口nk3; e
y_

1

凡nk3=st a口tunEs , 3) ;

(ri,

m

平
n=U:5;
n_rpstepfun(ri,U) ; 0
x_n2=otepfun(n.2) ;
xnkl=steplun(n, fl; 0

: i DislnvSys.m

U
H
中
H

1 2 3 4 5 6 7 8 9 冊 n 俚 出 m 侮 出 W 冊 m

U

풀이

stee(ny_rnk); O

axis(]0 6 0 21) ;
川abel ( lime in] );
미abel ( 'yEn] );
title ( 'u[ n-k] - u]n卞굳］ ) ;

그림 ]0-1] 시불변 시스템 그리기 코딩 결과（D囹nvSys.m)

0 step丘m 명령어를 이용하여 주어진 이산시스템 枷］과 工[1卜幻를생성한다．
0 stepfun 명령어를 이용하여 시간이 1만큼 지연된 이산 시스템 玎刃-1］과 x[刃 3］을생성한다．
0 시간 지연이 없는 이산시스템 y[n]을 지정한다．
0 시간이 l만큼 지연된 이산시스템 y[n-lj을 지정한다．
0 stem 함수를 이용하여 y［川을 줄기 형태로 그린다．
0 stem 함수를 이용하여 y[n크］을줄기 형태로 그린다．
F陀

Edo ＼月e빠

표肖甘I Tools

Oasktop

｛그 亡j 日 $ 1 Li ! 再＼ 戈 好 自 唱

W｝岫批

He巾

鼠

[3 團

黛口

2

e U[n42]

H

C

山

＞

00

on
2

2

on
on
3
4
了泗旨 [ni
u[n-kj - u[n-k-2]

5

6

on
5

6

1.5

岺

!

'

0.5 0O
0

2

q;
3
Time [n)

on
4

그림 10-12 시불변 시스템 그리기 실행 결과

입력 신호가 시간 k= 1만큼 이동하면 출력 신호도 그만큼 시긴中］ 이동한 파형이 나타난다. 따라서 이 시스
템은 시불변 시스템이다．

CHAPTER 10 신호 및 시스템

253

I 시변 시스템1
입력이 工[n] 이고출력이 y[n] 인 이산 시스템에서 시간히 k만큼 지연된 새로운 입력 玎刃 H幻 에 대한시
스템 출력 특성이 변하면 시변 시스템 (time-v町戶ng system)이라고 한다. 즉 y[n] / y[刃 U 幻이면 시
변 시스템이다．
卜月-File 1 ［거sVarSys.m

1예제 ]0- 7 !
이산 신호 玎川이 임펄스 함수이고 다음과 같은 입출력 관계를 가진 시스템이 있다．
y［川 = nx［미

신호값이 발생하는 시간 0 드 n 5 5[secj0們 시스템의 파형을 그리고, 0J 시스템이 시불변 시스템인지 시변
시스템인지 판별하라．

듣 ! 마5\／田sy묘m
-

n=0:5;

xn=stepfun(n，띠1眺e口fun(n, 1); 0
나＝stepfun(n肛眺eplun(n,2); e

自

n=n川小
y. nk=n.+xJ< ;
y-

i 2 3 4 5 6 ? 8 9 m n 促 仔 닉 垢 恰 m

풀이

subplot (211); 0
stem(n,y. .n); O

-

axis(10 602] );
cIabeI (Time In] ');

-

ylabel ( yIrI] ');
titIe ( n甘cJeIta[nI ') ;

-

小
-

subplot (212); e

stenm(n,y..nk); e

카is([0 60 21) ;
xlabel ( 'Time [n] ') ;
ylabel ( 'y[ n] ') ;
trtle( 'n付deltaln-kj ');

그림 ]0-13 시변 시스템 그리기 코딩 결과作兆VarS邱.rn)

0 시간 이동이 없을 때의 시스템을 지정하기 위해1 단위 계단 함수를 이용한 임펄스 함수 하川에서 l만큼
이동한 임펄스 함수 a[n-1]을 뺀 값을 지정한다．
0 시간이 1만큼 이동한 후의 시스템을 지정하기 위해 단위 계단 함수를 이용한 임펄스 함수 d［刃크］에서
1만큼 이동한 임펄스 함수 印기를 뺀 값을 지정한다．
0 시간 이동이 없을 때의 시스템 y[,玎을 지정한다．
0 시간이 l만큼 이동한후의 시스템 y[n-l]을 지정한다．
Osu햐加t 명령어를 이용하여 시간이 이동하기 전 시스템의 파형을 위쪽 그림 창에 그린다.
0 stem 함수를 이용하여 시간이 이동하기 전의 출력값 刃5回을 줄기 형태로 그린다.
0 subplot 명령어를 이용하여 시간이 이동한후 시스템의 파형을 아래쪽 그림 창에 그린다．
0 stem 함수를 이용하여 nS{n크］을 그래프로 나타낸다．

254

PART 03. MATIAB활용하기

F艇

口 亡｝ 4 曲 臣 曳 （프＼好 徊 堤 Jg , 昆 目 듣갚 m 口1
nd[n]

HC보

2

3
Time In)
n4[n=kl

e)
2

巴
3
辰n柑 [nl

2

5

6

4

C
5

6

41

H
C
玄

4

<
U

0

0
0

그림 10너4 시변 시스템 그리기 실행 결과

시간이 이동하기 전의 출력은 모두 0이지만 시간을 k= 1만큼 이동한 후의 출력은 파형 자체가 n3[n-1] =
d[n-1]로달라진 것을확인할수 있다. 따라서 이 시스템은 시변 시스템이다．

CHAPTER 10. 신호 및 시스텀I

255

LESSON

03

컨벌루션

컨벌루션은 선형 시불변 시스템을 통과하는 입력 신호오｝ 시스템의 임펄스 응답 사0떽 상호 관계를 명확히 나타내는 연산이
다． 0扈적 계산 방법을 工빵하고 MATLAB에서 제공하는 컨벌루션 명령어와 그리기 7능을 0용하여 출력 결과를 샐펴보자．
Keyword

I

I 연속 신호에 대한 컨벌루션 1 cony I 이산신호에 대한 컨벌루션 1

연속 신호에 대한 컨벌루션

연속 입력 신호工(t）와 임펄스 응답 신호 風t) 에 대한 컨벌루션（C아w아Ut幻n）은 다음과 같이 적분 형태
로 정의된다．

y (O= f,x(T)h(t- T)dr= x(t) * h(t)
L멘젠，I아81

(10.9)
M-File ! ConConv.m

연속 신호에 대한 입력과 임펄스 응답이 다음과 같을 때1, 신호값이 발생하는 시간 6 5t 56[sec］에서 입력
신호 x(t)와 임펄스 응답 신호 灰t), 입력 신호와 임펄스 응답 신호를 컨벌루션하여 생성된 출력 신호 y(t)의
파형을 각각 그려라．
兀（r) = u(t + 1) - u(t 寸 1)
h(t) = (- t + 2)[u(t) - u(t -2)]

배경
지식

' cony
입력 벡터 신호x와 임펄스 벡터 신호h를 컨벌루션하여 새로운다항식을생성한다. 컨벌루션하는cony 명
령어의 기본 형태는 다음과 같다．

conv(x, h)
· X: 입력 벡터 신호
. h: 임펄스 벡터 신호

256

PART 03. MATLAB활용하71

CanCorw.m

;3: ! + !

1 2-

t=七:0. Ul :6; 1 p
x_t=ntep佃（t，니卜如pfun(t, l) ; 0

3-

h_t=(-t*2) .u(stepfun(t, 0)-stepfun(t, 2) );

5-

subplot (311) ;

41

y_t叱ony(x. .t,h. t)*0.01 ; e

6 7 8 9 m H 促 仍 化 佰 作 口 冊 m

叫

이at(t.n比 0

H

an i so田 60 引）;
ylabelO sOt) ') ;

H
U

title ( Input Signal ) ;
subplot (312) ;

e
1

plot(t,h. ,t); O

U

auis0]七 6 0 3] );

m

비abel ( hOt) ');
ti티이 h o口aloe Response 데gsal ' ) ;
sub미 叭 田田）;
미ot (t, y1t (601 : l텨긔）); 0
xxi s0［七 60 引 ) ;
비 ab이 ( yOt) ) ;
tltle (0utpst Signal ') ;

H
H
中
H
1

그림 ]0-15 연속 신호 컨벌루션 코딩 결과（ConConvm)

0 컨벌루션 적분의 근삿값이 실젯값에 가깝도록 하기 위해 시간 간격을 충분히 작은 0.01로 지정한다．
0 연산에 필요한 입력 신호와 임펄스 응답 신호를 지정한다．
0 COllV 명령어를 이용하여 입력 신호와 임펄스 응답 신호를 컨벌루션한 후, 시간 간격 0.01과 비례를 조절
하기 위해 0.01을 곱한다．
0 히ot 명령어를 이용하여 x(t)를 그래프로 나타낸다．
0 plot 명령어를 이용하여 可t)를 그래프로 나타낸다．
0 plot 명령어를 이용하여 y(t）를 그래프로 나타낸다. 출력 결과를 그리려면 다른 배열의 원소 수와 같은
12011로 맞춰야하므로 출력 결과의 원소 601부터 1801까지 1201개의 뎨이터를 이용한다．
F沌 日j作

\／田W

｛그 d 日 由

a好心t 祀아5
o

De孜的p

no幻吐

04啣

미

'\ -\ 抑 自 咀 J二 , 昆 ［그 國 曲 回
Input Signal

0-

2

6

-4

-2
0
2
I,了巾IL除a 急駙ponse 아305

6

-2

6

0
Output 햐斗甘

0

2

6

그림 ]0-16 연속 신호 컨벌루션 실행 결과

CHAPTER 1O. 신호 및 시스템

257

I 이산 신호에 대한 컨벌루션
이산 입력 신호 町미 과 임펄스 응답 신호 可川 에 대한 컨벌루션은 다음과 같이 합의 형태로 정의된다．
m

H

y［小 2堈枷-k]＝工回* h[川

(10.10)

（刃

M-File I DisConv.m

lot빤I아9j

이산 신호에 대한 입력과 임펄스 응답이 다음과 같을 때, 신호값이 발생하는 시간 6 드 刃 5 6[sec］에서 입력
신호 町미과 임펄스 응답 신호 可미, 입력 신호와 임펄스 응답 신호를 컨벌루션하여 생성된 출력 신호y［미의
파형을 각각 그려라．
x[n] =u[n+1] -u[n- 2]
h[n] = (-n + 2)(u[n] - u[n -2] )

풀이

-

마oConvm ｝唯硼

3 4 5 6 7 8 9 m n 促 仍 m 垢 怜 n 祀 氾

2-

n=-6:1:6;

x_n=stepfun(n,-1)-stepfun(n』2); 0
h.ji=(-n*2) .+(step1un(n』0)-stepfun(n,2)); e

y. .n=conv(x..nh. n); e

subplot (311) ;

stem(n,xmn) ; 0

-

axis(卜6 60 51) ;
yIabeI ( s1n1 ');
tltle ( In口Ut 미goal ' ) ;
subplot (312) ;

-

axls(1-6 6051) ;
ylabel ( 'hln] );
title ( ' ImpuIse Response Signal ') ;

-

subplot (313) ;

-

aais(卜6 60 51) ;
ylabel (y[ n] ') ;
title (Out口Ut 引 goal ) ;

stem(n, h_n); 0

stem(n,yjg(7:19)); 0

0 입력 신호 工［기을지정한다．
0 출력 신호 可川을 지정한다．
0 COnV 명령어를 이용하여 이산 입력 벡터 신호 玎미과 임펄스 벡터 신호 力[n］을 컨벌루션한다．
0 stem 함수를 이용하여 입력 신호 玎미을 그래프로 나타낸다．
0 stem 함수를 이용하여 응답 신호 h[n]을 그래프로 나타낸다．
0 stem 함수를 이용하여 응답 신호 y[n]을 그래프로 나타낸다. 25개 원소의 중앙부터 좌우로 6개 원소인
원소 7부터 19까지의 13개 데이터를 이용하여 줄기 형태를 그린다．

258

PART 03. MATLAB활용하71

小

그림 10-17 이산 신호 컨벌루션 코딩 결과（Dbo冊m긔）

Efle

Ed捷

'내們V

[n5e八

To帥； 0出加p

쌔M汁

比拓

횰

口 d d ir 臣 ' \ '\ 好 匈 堤 月니 邑 口 國 ! a 口

"

甲

甲

甲

0}

-2
0
2
ImpuiseR叫'C기的 $'9心

-2

0
ot却(itS枷l出

芭｝

4

2

0

6

6

릊
0

4

그림 10너8 이산 신호 컨벌루션 실행 결과

CHAPTER 10. 신호 및 시스템

259

LESSON

04

샘플링

연속 신호를 일정한 시간 간격을 두고 띄엄띄엄 추同1 정렬된 수열 형태로 만들어 0싼 신호를 얻는 과정을 샘플링이라고 한다．
주어진 정현파 신호에 사용한 주파수와 다른 주파수를 이용하여 샘플링하는 과정을 그래프로 나타내어 알아보자．
Keyword

I 샘플링 1 나이퀴스트율 1

I 샘퓬링
연속 신호에서 일정 신호를 취해 이산 신호를 생성하는 것을 샘플링 (san巾ling）이라고 한다. 이산 신호
xm兀］는 시간 t=n乙에서의 연속 신호工(t）와같다．
工［n] = 工（태t=nI = 工［n7;]
n= · ' ·,-1, 0, 1, 2, ···
여기서 乙는 샘플링 주기이고, 乙의 역수兀는 샘플링 주파수가 된다. 특히 정현파 신호는주파수가 다른
정현파의 1차 결합으로 나타낼 수 있기 때문어］샘플링 효과를 살펴볼 때 흔히 사용된다．

r예제 伯-1이

M-File 1 SamoSinus.m

주파수가 100[H기인 정현파 신호 x(t)가 있을 때, 샘플링 주파수 100[I也］와 200［出］에 대한 샘플링 신호
를 그래프로 나타내라．
x(t) = cos(22rf0t)
5am外m瓜nl 二 +1
I10 = 山2;
21 = I/ fl;
3tmm = {)1
4小
tmoo = 4.1;

듬： 忿'能自
7a-

d12 = ]/2[lL
t = t, ir,:dt:tmoo;

10n-

41 = tmin:d1l:1：缸;
t2 = t目in:dt2:11oo;
o-t = coo(2.pi. to.t) ;

1314-

o_t I = 印9 (2，이너0.11) ;
o42 = cos(2女미너마臣）;
oobolot (211) ;

16 叫

p) ot (to.
hold;

_t)

;

e
0

0

m 円 四 끼

ote.(t山me
oobplot (212) ;
plot (t, o.

.t)

;

O
e

o1,.)02, 0 t2) ;

그림 ]0-19 정현파 신호 샘플링 코딩 결과（Sam口&n出．m)

260

PART 03. MATLAB활용하71

02개의 샘플링률을 입력한다．
0 샘플링 범위를 입력한다．
0 샘플링 주파수에 따른 정현파 신호를 지정한다．
0 정현파신호를그림 창 위쪽어］나타낸다．
0 stem 함수를 이용하여 100[H기로 샘플링한 결과를 그림 창 위쪽어j 나타낸다．
0 정현파 신호를 그림 창 아래쪽어］나타낸다．
0 stem 함수를 이용하여 200[H기로 샘플링한 결과를 그림 창 아래쪽어］나타낸다．
!n5e作
+\

!0口Is

Desktop

Window

lie巾

J二 n 昆 目 國 咽 1그1

自 느

m\

E

{.) t3 났 由

:)

'

4

/

0.5
0
-05
아K版

0.01

0.0侄

(1.02

0025

01｝菊

{1.04

0.035

0.04

丘／／
匕

그
＼\

1

0.03

戶

0.5
0
/

/

-0.5
/

-1

J

0

0.005

0.01

0.015

002

0.025

0.03

그림 ]0-20 정현파 신호 샘푤링 실행 결과

샘플링 주파수가 100[H기인 위쪽의 그래프보다 샘플링 주파수가 200[H기인 아래쪽의 그래프가 더 촘촘하
거］ 신호를생성했음을 알 수 있다．

CHAPTE日 ]0. 신호 및 시스템

261

I

나이퀴스트율

샘플링하는 연속 신호 工（t) 의 최대 주파수를 月／이라 하자. 工(t）가 대역 제한（bandlimited) 신호일 때
샘플링 주파수／
；가 신호의 최대 주파수인 月i의 두 배 이상인 경우, 샘플링된 이산 신호로부터 연속 신호
x(t）를 재생할수 있다는 것이 섀넌（Shannon）의 샘플링 정리이다．
/; 三2／뇨

(10.12)

여기서 /;=2月戶］되는 주파수를 나이퀴스트율（Nyquist rate）이라고 한다. /; 之 2fM인 경우는 원래
신호와 샘플링된 신호의 주파수가 같다는 것을 의미하고, /; <2j뇨인 경우는 샘플링된 신호가 원래 주파
수의 반만큼주파수 겹침 (aliasing）이 발생한다는 것을 의미한다．

1 예제 10- il

M-File i SampNyqui.m

1

주파수가 2[H기인 정현파 신호 .X(t)가 있을 때1, 샘플링 주파수 6[H기와 3 [Hz］에 대한 샘플링 신호를 그리고
서로 비교해서 설명하라，
x(t) = sin(27rf0t)

n

풀이

2戶
34567891011 1213寸
14 15 16I? -

mp卜中y｛和Lnl :n: 斗i
t = O:O. WI :2;
f口＝2;
札t = 引n(2삐H마t) ;0
I引 = 6;
t引 = 0:1/fol :2;
凡51 = S n(2삐，伽tsl 0
作2 = 3;
ts2 = 0:1/1s2:2;
x-s2 = 引n(2삐나마t820
subplot (211) ;
이ot(t . 凡t) ;
hold;
stem(t針，凡町rs- );0
subplot (212) ;
미ot(t . 凡t) ;
hold;
ste.(ts2, x_町小出0

그림 10-21 나이퀴스트 샘플링 신호 코딩 결과（San）口N四내.m)

0 정현파신호工(1）를지정한다．
06田기로 샘플링한 신호를 지정한다．
0 3[H기로 샘플링한 신호를 지정한다．
0 stem 함수를 이용하여 샘플링 주파수 6[H寸비 대한주파수 신호를 그린다．
0 stem 함수를 이용하여 샘플링 주퍄수 3［地］어］ 대한주파수 신호를 그린다．

262

PART 03. lvtATLAB활용하71

File

Edit

/
/
View

Inseet

口나 d 可 旨

"\

1

Tools

0.5
0
日．5

1
0

02

1

0

1

0

Wndow

He:p

거

04

\／

0.6

「

0.8

12

1.4

,

/

「＼

0.5

Desktop

'.' ' '. 抑 匈 七二 j.7 , 包 口 困 二｝ 唾

J

1.6

1.8

2

1.
6

2

,5r

/

02

0.4

0.8

0.
6

1

12

1.4

1.6

그림 10-22 나이퀴스트 샘플링 신호 실행 결과

아래쪽 그래프와 긷미 샘플링 주파수의 정수배마다 반복되는 원래 신호의 주파수 스펙트럼이 서로 겹쳐서
나타나는 것을 주파수 겹침이라고 한다. 이 경우에는 원래 신호와 많이 달라지므로 제대로 복원할 수 없다．
MATLAB에서 보여주는 신호는 모두 이산 신호이지만 샘플링률이 나이퀴스트율보다 아주 높은 경우어臣
연속 신호처럼 보인다．

CHAPTER 10. 신호 및 시스템

263

LESSON

05

신호 복원

주파수 겹침이 생긴 이산 신호를 원래 신호처럼 정보 손실이 전혀 없는 상태로 복원하는 것은 불가능하다, 그러나 이론적으로
는 섀넌의 샘플링 정리를 만족하도록 샘플링 주파수를 충분히 높이면 정보 손실을 최소화하여 신호를 복원할 수 있다. 샘퓰링
된 이산 신호를 영차 홀드 방법을 이용하여 다시 연속 신호로 나타내는 과정을 그리71 기능을 통해 확인해보자．

Keyword

I 영차홀드 i stai田 1

영차 홀드

I

샘플링된 이산 신호로부터 원래 연속 신호를 복원하는 가장 간단한 방법은 하나의 샘플 간격어］대한 각 샘
플의 값을 유지하면서 이 샘플 사이의 값을 근사적으로 짖아내는 것이다. 이러한 형태의 신호 복원 시스
템은 임펄스응답의 차수가0이므로 영차홀드（zero -order hold）라고 한다．
영차 홀드를 이용한 신호 복원의 경우, 주파수와 주기의 역수 관꼐에 따라 샘플링 주파수가 높을수록 시
간축의 간격이 줄어들어 샘플링이 더 촘촘해지므로 복원 신호는 원래 신호의 파형에 1기 가까운 형태를 띠
거］ 된다．

M-FiIe ! RecoZero.m

1 예저I 10- 12 1

샘플링 주파수 I0口也］와 40[H기룰 이용하여 연속 신호 玎t)를 샘플링하고 이산 신호를 생성했다. 신호값이
발생하는 시간 0< / 드 4[se이 에서 영차 홀드를 이용하여 생성된 신호를 원래 신호로 복원하라．

；而

x(t) = cos(27rt)

지식

'

stairs

영차 홀드를 이용하여 복원한 신호를 연결하여 계단 형태로 나타내면 원래 신호와 근접한 파형을 얻을 수 있
다. x에 대응하는y의 위치를 계단형태로한단씩 그리는stairs 명령어의 기본 형태는 다음과같다．

stairs(x, y)

264

PA日T03. M／玎LB활용하71

릍 I Reco

小
m
小
1
1
U
m
m
叫
小
1
4
4
1
n

123456789mn促四m幅祐n

m

풀이

1

1819게-

m
f引미0; 1o2=40; 0
tmin=0; tmax=4; clt=1/1000;
nl = tmin:1/f引:tmax; n2 = tmin:1/1o2:tmao; 0
凡nl = cos(2ap汁nl) ; x. .n2 = cos(2,pi*n2) ; 0
t = tmio:dt:tmao;
x_t = coo(2.pi*t) ;
subp 比t (211) ;
이ot (t , 凡t, r= ) ;
axio(1tmin tmax -1.2 1 .21) ;
hold;
ota汁s(nl,x_nl) ; O
시 abel ( t ');
title( "Rec口nstruction Signal by zero-order hold: Is = 10 Hz' );
subp lot ( 21 2) ;
plot (t,x_t, ' r-');
aoio(ltrain tmax -1.2 1. 21) ;
hold;
otairo(n2, x1n2) ; 0
olabel ( 't ') ;
title(Reconstroction Signal by zern-order hold: Is = 40Hz ) ;

그림 10-23 영차 홀드를 이용한 신호 복원 코딩 결과（Rec고ero.m)

0 샘플링 주파수 10田기, 40[H기를 각각 지정한다．
0 샘플링 주파수가 10{H기일 때의 시간축 간격 0.1과 샘플링 주파수가 40[H기일 때의 시간축 간격 0.025
를 지정한다．
0 영차홀드로생성하는신호를지정한다．
0 stairs 명령어를 이용하여 샘플링 주파수가 1아H기일 때의 연속 신호를 한단씩 계단 파형으로 복원한다．
0 stairs 명령어를 이용하여 샘플링 주파수가40[H可일 때의 연속 신호를 한단씩 계단 파형으로 복원한다．
Fl拒 Ed仕 너ew InSert TO머5
口 t二 닢 出

L뇹 ' \ 戶＼ a'7 包 ＼世 J; ' 4

U 區｝ a 匹工1

Re（力go杆Ucbon 아anal by o月｛tH가derh야d: fB 丘 10Hz

0 砧 d
3.5
t
Rec 기肖tructk片｝ Signal by 四ro여rderh야4: 相 = 凝｝Hz

4

t
그림 1아24 영차 홀드를 이용한 신호 복원 실행 결과

샘플링 주파수가 10咀기일 때보다 40[H기일 띠1 신호가 더 촘촘하게 복원된다．

CHAPTER 10. 신호 및 시스템

265

LESSON

06

연속 신호의 주파수 표현

시간 영역에서 나타내기 어려운 신호는 주파수 영역에서 좀 더 쉽게 표현할 수 있다. 신호에 포함된 다양한 주파수 성분을 구
분하여 주파수의 함수로 나타낸 것을 스펙트럼이라고 한다. 주파수 영역에서는 연속 주71 신호를 해석하기 위하1 연속 시간 푸
리에 급수를 이용하고, 연속 비주:7 ' 신호를 해석하기 위하1 연속 시간 푸리에 변환을 이용한다. 대표적인 연속 신호인 정현파
신호（게 대한 진폭 및 위상 스펙트럼을 찾아내고 푸리에 변환의 컨벌루션 과정을 그래프로 나타내보자．
Keyword

I

I 신호스펙트럼 I fft I 진폭스펙트럼 1 위상스펙트럼 I angle I ifishift 1 iffi {

신호 스펙트럼

시간 영역에서 진폭A , 주파수兀 , 위상中인 연속코사인 함수는 다음과같이 나타낸다．
x(t) = A cos(2wf0t + 砂 )

(10.1引

여기서 위상 中는 시간 0에서 신호가 한주기의 어느 위치어］ 있는지를 나타낸다. 식 (10.13）에서 위상을
0으로 놓고 오일러 공식 (Euler's 的rmula）을 이용하면 식 (10.13）은 다음과 같이 정의된다．

x(t)＝브.j2兀加 +4e_j2：兀／
2

(10.14)

2

X(J) = 1 A!2
[0

(/
(f = -.Jo)
＝无！

[A12

식 (10.13）에서 2개의 항으로 분해된 주파수를함수로 표현하면 다음과 같다．

(10.1引

（그 외）

여기서 신호를주파수 함수로 표시한X/）를 신호의 스펙트럼 (spectrum）이라고 한다．

1 예제 10- 13 1

M-FiIe I ConSpect.m

주기가 4[sec］이고 샘플링률이 0.01인 코사인 신호 x(t) = cos(2兀／）의 파형과 진폭 스펙트럼 파형을 그려라．

；而
지식

' ifi
신호를 주파수 함수로 변환하려면 푸리어］ 변환을 사용한다. 신호의 스펙트럼을 나타내기 위하1 벡터 x어］ 대
한 이산 푸리어］변환을 나타내는 ifi 함수의 기본 형태는 다음과 같다．

266

PA日T03. M戶T냐＼B 활용하:7 '

ffi(x)

三 r ConSpect.m ：可『 4夕
1
1
1
=
=
n
1
=
=
m
=
m
m
1
e
e
4

123456=
789IDII 1213 141516 1? 18 寸

m

l 2 3 4 5 6 7 8 9 m n 泛 伺 H巧 伯 n m

풀이

0

dt = 1/！미上 t· 때 = 4;
t = 0:dt:t. ax;
x_t = cos(2*pi.t) ;
X_f = llt (x_t) ; 0
N = length(x_t) ;
Xs口ec=abs(X느1) /N; 0
I rgq=(0川너 );
subplot (211) ;
pIot(tx_ t) ; C
grid;
aXis([O tiax -2 2) );
xlabel (' Time (t) );
비ab이 ( 'X(t) ) ;
subpiot (212) ;
piot (ireq.Lgpec) ; 0
grid;
xlabel ( 'Frequericy (Hz) );
미ab이 C默f) );

4

그림 10-25 코사인 신호 그리기 코딩 결과（CoOS口e伐m)

0 샘플링률과샘플링 범위를 지정한다．
0 고속 푸리어］변환함수 航를 이용하여 코사인 함수蚊t)에 대한푸리에 변환을 계산한다．
0 진폭 스펙트럼어｝대한 절댓값을 균일화한다．
0 코사인 신호를 그림 창 위쪽에 그래프로 나타닌仁｝.
0 주파수와 위상스펙트럼을 그림 창 아래쪽에 그래프로 나타낸다．

그림］小쏘 코사인 신호 그리71 실행 결과

진폭 스펙트럼의 5번째와398번째 위치에서 진폭이 05인 2개의 정점이 나타난다．

CHAPTER 10. 신호 및 시스템

267

I

진폭 스펙트럼과 위상 스펙트럼

푸리에 급수를 이용하여 구한주파수 성분의 진폭 그래프를 진폭 스펙트럼, 위상 그래프를 위상 스펙트럼
이라고 한다．일반적으로 신호x(t)가 실수이더라도 푸리에 급수에 의해 계산된 스펙트럼 X(f）는 복소수
가 되므로 진폭 스펙트럼을 정확하게 그림으로 나타내는 경우에는 절댓값 匹
（別로 표현한다. 여기서 주
기 신호와주기가같은정현파를기본피라고하며, 이때의 주파수／0를기본주파수라고한다. 또한기본
주파수의 정수배인 kf0의 주파수를k고조파라고 한다．

M＋如 ! SpecSinus.n겨

1 예저110-14!
{

신호의 주기가 2이고 샘플링01 512개인 서로 다른 두 정현파 신호를 혼합한 신호 x(t)의 진폭 스펙트럼과 위
상 스펙트럼을 그려라．

；而

x(t) = cos(52rt _60O) + 3c0s(87r1 -90")

지식

' angle
위상스펙트럼을나타내기 위해 복소수배열 x에 대한위상칵을라디안값으로 나타내는angle 함수의 기본

형태는 다음과 같다．

an이e（지
-x: 복소수 배열

이때 위상칵은 너r와Jr 사이에 놓여 있다．

풀이

2-

3 45 6 7 B9m H促 沼 m佰 陌 W 伯 円 加

, Specnn小．m 批：：半g
J
1 1=2; N=512; Ts=T/N; <1
t=T＄士（0:(N니 ) ) ;
帥n긔니／3; ph12=pi/2;
凡t = cos(5.pi毗-phil) + 3士cos(6士미，t-ph12) ; 0
X_ f=fft (x_t) ; 0
2_am呻呵XJ)/H; 0
X_phase=an引e(X_f); O
k=O: 3J; 0
subplct (211) ;

stem(k .X_amp(l :length(k))); e

grid;
almbel ( 'k ');
미 mbe 나 12(1) 1 ) ;
tltIe(Ampl itude Spectrum) ;
subplot (212) ;
st日m(k, X_phase(l : length(k) )); O
grid;
xlabel ( 'k ') ;
미abel ( 'WarigleX(f) ') ;
title (十as日 Spectrum ) ;

그림 10-27 혼합된 정현파 신호의 스펙트럼 그리기 코딩 결과（31光（Sirtus.m)

268

PART 03. M月ILAB활용하기

0 샘플링 주기와시간축, 2개의 다른 위상을MATLAB에서 일반적으로사용하는 라디안값으로 지정한다．
0 工（t) = cos(52Tt -60") + 3 cos(8兀／ 900）를 지정한다．
Offi 함수를 이용하여 x(t)를푸리에 변환하여 X(f）로 나타낸다．
0 abs 함수를 이용하여 匹(f) I를 구한 다음 샘플링률로 나누어 진폭을 지정한다．
0 angle 명령어를 이용하여 복소수 원소의 위상칵을 라디안 값으로 전환한다．
0 총 512개 샘플링 중어因 처음 31개1 데이터만 고조파 차수어］사용한다.
0 stem 함수를 이용하여 31개 데이터에 대한 진폭 스펙트럼을 그림 창 위쪽에 그린다.
0 stem 함수를 이용하여 31개 데이터에 대한 위상 스펙트럼을 그림 창 아래쪽에 그린다.

D 亡｝日 曲 ! 臣 1 曳 曳 幽自뻗 而 , 晟 1 爵 匡크 ! 日 口1
Am메地de 햐冶drum
1
口
x
0.5
V

0 OOOO
0

OO

O 巴 OOOO（끄 ｛그 O (:)｛그 5O ｛그 O；그 S ｛그 (> ｛그 ｛그
I0
15
25

k
Phase Spedrum

4

듕.

'

0

'?

'1

O

了1

古
5

1 小』
少n"mJP士 시士古
10

15

25

k

그림 10-羽 혼합된 정현파 신호의 스펙트럼 그리:7 ' 실행 결과

진폭스펙트럼의 여섯 번째 신호는 0.5, 아홉 번째 신호는 1.5를 나타낸다. 푸리에 변환을 한스펙트럼 X(f）의
여섯 번째 값과아홉번째 값의 위상인 了에 대한라디안값크 .0472와 互어］대한라디안값-1.,5708
3
.
2
.
을 위상 스펙트럼에서 보여준다．

I

연속 시간 푸리에 변환의 컨벌루션

시간 영역어］대한 컨벌루션은식 (10.9）와같다. 입력 신호 x(t) , 임펄스응답신호h(t) , 출력 신호 y(t)
의 푸리어］ 변환이 각각X(f) ,H(f) , Y(f）일 때, 푸리어］변환어］대한출력 스펙트럼은 다음과짙히 정
의된다．
Y(f) = H (f) X(f)

(10.16)

즉 시간 영역에서의 컨벌루션은 주파수 영역에서의 곱셈과 일치한다. 입력 신호는 시스템을 통과하면서
주파수별로／/(/）만큼의 이득이 곱해져 출력된다．

CHAPTER 10. 신호 및 시스템

269

뻔제 I아佰 J

舟卜斜拇 } ConFtConv.m

연속 시간 주7! -6 5t 56[sec］에서 입력 신호 工(t）와 임펄스 응답 신호 h(t)에 대한 출력 신호 y(t)의 파형
을 시간 영역에서 그려라．그리고 푸리에 변환의 컨벌루션을 이용하여 Y(f) = 月
（f)X(f）를 구한 다음, 이
에 대한 푸리에 역변환을 이용하여 시간 영역에 대한 출력 신호 파형을 다시 그려라. 이때1 샘플링 데이터는
5000개라고 가정한다．
x(t) = u(' + 1) - u(t -2)
h(t) =u(t) -u(t- 1)

；而
지식

'fftshift
0주파수성분을스펙트럼의 중앙으로이동하여 스펙트럼을좌우대칭으로보여주는侃曲侃함수의 기본형
태는 다음과 같다．

=

if始hi州지

iffi

주파수 함수를 다시 시간 영역 신호로 되돌리기 위해 벡터 x의 푸리에 역변환을 구하는 出1 함수의 기본 형
태는 다음과 같다．

or甘RCOn也m 挑 L翌쿄
t이下七； t. au=6; N＝텨 刃；
dt=(t. aX-t. in)/f;
t=t川n:dt:tmax;
x_t=stepfun(t, 시)-stepfun(t, 2) ; 0
h_t=stepfun(t, O)-stepfun(t,1) ; e
y_t=cony似t,h蜘dt; 0
X_f=dt* fft (s_t) ;
Hf=dt士f ft (h느t) ;
Y_ f=X口f．士H1f; 0
y_ ft=fftshift ( (1/dt).ifft (V_f)); 0
subplot (211) ;
pIot (t, y_t (250l: 750l) ); O
aels(1七 60 1.5] );
xlabel ( t ) ;
斗
비abel ( s(t) ');
title(Gonvulution Result in tiCs domain ') ;
subplot (212) ;

1 2 3 4 5 6 7 8 9化 n 坦日 m巧 佰 口冊佇 四 기刃

풀이

e
-

plot(t,y_ ft); e

axis(]七 60 1 .5] );
xlabel ( 't ') ;
미ab미 (y (t) );
title ( 'Csnvolution Result by Fourier Transform ') ;

그림 10-29 푸리에 변환의 컨벌루션 그리기 코딩 결과他onFIC이刊.m)

270

PART03. MA凡AB활용하기

0 입력 신호 工(t）를 지정한다．
0 임펄스응답신호h(t)를지정한다．
0 工(t）와7仰）를 컨벌루션하여 y(t）를 지정한다．
OX(f）와／/(/）를곱하여 Y(f）를지정한다．
Oi俄 함수를 이용하여 주파수 함수를 다시 시간 영역의 신호로 변환하고, 俄shift 함수를 이용하여 스펙트
럼의 중앙으로 주파수 성분을 이동한다．
Odt로 나눈 시간 간격 5001개에 대한 출력 결과인 원소 2501부터 7501까지 5001개의 데이터를 시간축
으로 지정하여 시간 영역어써 직접 계산한 컨벌루션의 파형을 그린다．
0 plot 함수를 이용하여 푸리에 변환한 컨벌루션의 파형을 그린다．
目b

帥t

出BW

鈿It

To出 t加出00

川包낳0汭’

H目p

口 (3 日 由 Li 曳 艮 幼自 堤 Jr 미 昆 口 녑 겅 口1
O미l咐1川on Result in time domain

릊，

1.5

,

\

0-

1

6

1

-2

1)
2
t
Convoluti긔l Resu仕 by Fourier Transform

\

,
/r\

릊，

1.6

-4

r

0毛

-2

'

\,,
0

2

그림 10-30 푸리에 변환의 컨벌루션 그리기 실행 결과

시간 영역에서의 컨벌루션 결과와푸리어i 변환후 실행한 컨벌루션 결과가동일하므로, 편리한 계산을 위해
서는 푸리에 변환을 실행한후 단순한 다항식의 곱으로 계산하는 것을 추천한다．

CHAPTER 10. 신호 및 시스템

271

LESSON

07

이산 신호의 주파수 표현

주파수 영역0私寸 반복 주기를 이용하면 이산 정현파 신호도 연속 정현파 신호처럼 쉽게 표현할 수 있다. 그런데 연속 정현파는
주파수의 값에 상관없이 항상 주71 신호이지만, 이산 정현파는 디지털 주파수가 유리수인 경우0艇 주71 신호가 된다. 따라서
주파수가 力T의 정수배만큼 차이 나는 이산 정현파는 같은 신호이고, 주파수의 차이가 27碑l 정수배가 아니면 이산 비주;71 신
호로 분류된다. 이산 푸리에 변환을 이용하여 이산 신호에 대한 스펙트럼을 나타내는 과정을 알아보자．
Keyword

1 이산푸리에 급수와 계수 1 이산푸리에 변환 1

I 이산 푸리에 급수와 계수
이산 신호玎끼은 유한한주기에서 순차적인 값을 갖는다. x[n] 이 한주기 동안주기적 순서를 가진 신호
x［川이라고할때, N- 以）가되면 i[ n}은 玎미으로대체할수 있다. 이산시간푸리어］급수는N개의 이산

口ke- （2兀／N)n

［n］

'丸

2

k= <N>

誨

［n]

=

따＝

工

시간주기 신호를入／개의 고조파합으로 나타내는 것이며, 이산시간푸리에 급수와계수는 다음과같다．

可" " " ' ""

식 (10.17）에서 k = <N＞은 연속된 N개의 샘플을 뜻한다．

r匹＝Fi旭 1 DisFtCoef.n갸

1 예제 10-16 1

272

PART03. M月1냐＼B활용하기

{:

nj=

x[

"’

三）

::::'

한 주7뻬 8개의 신호 샘플이 있는 이산 푸리에 급수가 다음과 같을 때, 이산 푸리에 계수 (2k에 대한 진폭과
위상을 그려라．

今

三 [ 머sFtCoef.m 烈：I 等i
1-

N=5;

笞

pi/

2*

二；

[l

ri;
egaO=1 1 1 N;
「0
"
rp-N/2.l :N/2;
W_N=exp(-lJ*omega마n) ; 0
化r k=1 :6 Q
乞k( k)=sum(x...s. *9_札 (k니) )/N;
end

45릉：

e

6789m卜卜卜川沔怜n侶円m기m
4
H
中

a_

-k)

小

a_mag=abs
k;
;
工phase=an引이工k) ;
k=0川너 ;
S먀m 比t (21I)
(a

1

stem(k』a_may) ; O

e

xlabel ( k ') ;
ylabelt 嫩l) la_ku } );
title( Magnitude Response ');
subplot (212)
stes(k, a1phane) ; O
xlabel ( 'k ) ;
미 abel ( 개b I｛咐angIea_k} ') ;
title(Phase Response' );
1
1
1
U
中
斗
4

그림 10-31 푸리에 계수의 진폭과 위상 스펙트럼 그리기 코딩 결과（Dis디q甘.m)

0 한 주기 신호에 았는 샘플 8개를 푸리에 급수 벡터 신호로 지정한다．
4 .H . . ,
, ,
22r .
0 신．호의. 기．본 주파수 Wy = 二二와 신호의 총합 구간 ("N）을 지정한다．
"
N
0 복소 정현파를 생성한다．
'

'

V

'

'

V

H

H

"

'

나

'

V

나

'

."

0 for문과sum 명령어를 이용하여 벡터로 표현된 식 (10.18）의 원소를모두 더한다．
0 stem 함수를 이용하여 k 값과 진폭을 그림 창 위쪽에 그래프로 나타낸다．
0 stem 함수를 이용하여 k 값과 위상을 그림 창 아래쪽에 그래프로 나타낸다r
ElD

문서 조판에 사용하는 례이텍 프로그램으로 굵은 글씨체를 나타내려면 \bf{ ｝롤 사용하고 ，각도를 나타내는 기호
／는 \an아e로 입력한다．
拓마＄ E地5蚣야｝ Y聊姓（겨臂 -4帥）

U 心日 曲 臣 1曳 \

鬱 匈 咽 伊＝ , 晷 口 圓 蠶 口
Magn6ude Response

0.8
0.6
S芦 0.4

0
,,

?

耳’

0.2
「？

풀이

3

4
k
Ph羽e Response

6

6

7

Y
m
닉

?
0
O 2

1

O
3
k

6

7

그림 10-32 푸리에 계수의 진폭과 위상 스펙트럼 그리71 실행 결과

CHAPTE日 ]0. 신호 및 시스템

273

I 이산 푸리에 변환
이산 푸리어］변환（DFT: Discrete 恥urier Transform）은 주파수 영역에서 이산 시간 유한 주기 신호를
분석하는 뎨 사용한다. 이산 비주기 신호를 주파수 영역의 표현으로 바꾸고, 다시 시간 영역 표현으로 되
돌리는 이산 시간 푸리에 변환쌍은 다음과 같다．
l

坰

=

-f X(w)e/' '1dw
2兀．/ 二7r

e/

2

n]

=

x[

)

' '

H的

(a)

X

m

합성방정식 (synthesis equation）으로 표현된 식 (10.19）는 이산 시간푸리에 역변환이라 하고，분적방
정식 (analysis equation）으로 표현된 식 (10.20）은 이산시간푸리에 변환（Dl下r）이라한다．

繫／크呻斜！毋 ! DisSpect.m

I 01111 1 (1-17 I
I二二：
二二＝-:J

시간 -10< 刃 5 5[sec］에서 이산 비주31 입력 신호 玎미에 대한 진폭 스펙트럼과 위상 스펙트럼을 그려라．

［響］

=

枷］ cos
DISS附tm 址麟身

n＝너0:5;
omeaa=-pi :1/Sf]그：P匕 <I

x_n=cos (3.pi*n/2) ;e
(-

(eap

0

1
e

aais(] -pi pi 09) );

1

xlabel ( Woroega) ;

1

비 abelt ' i 默蜘ooeaa) 1 ' ) ;

H

title ( 'Ampl itude Spectrue ');

H

sub口 比t（끼 2) ;

1
H

aais(] -pi pi -4 4] );

U

xl abel ( 개加mega ) ;

1

미 abel ( ' 甘anal eX（毋aaeaa) );

m

미0小mega兀phase); e

title (Phaae 鈿ect r베 ) ;

그림 ]0小33 이산 비주71 신호의 진폭과 위상 스펙트럼 그리기 코딩 결과（DbSpect.m)

0 모든 이산 정현파는 -it 5 U) 드 兀에서 표현할수 있다．
0 이산 비주기 입력 신호玎미을 지정한다．

274

1

plot (omega』X_spec); O

1

Lphas日＝an引e的）; 0
subplot (211) ;

1

ll_ x丹
lj* n * omeaa) );
X_spec=abs (X_t) ; O
f=

-

小

1 2 3 4 5 6 7 8 9 m H 侘 沼 m 隔 恰 W 娼

풀이

PART03. MA凡AD활용하71

0 식 (10.20）을 지정한다. 이때 벡터 n과 on妃ga어］대한 벡터 곱셈은 서로 차수를 맞춰 계산하기 위해 벡
터 n을 전치 벡터로 바꿔서 사용한다. 복소수의 허수 단위는／이지만 코딩 속도를 향상하기 위해I i／를
사용하기도한다．
0 abs 명령어를 이용하여 진폭을 구한다．
0 angle 명령어를 이용하여 위상을구한다．
0 plot 함수를 이용하여 진폭 스펙트럼을 그래프로 나타낸다．
0 히야 함수를 이용하여 위상스펙트럼을 그래프로 나타낸다．
F沌

Ed仕

口 (3 a

U
乙d

-1

Amp砒此e 햐冶（如urn

Phase Spectrum
2 0 그
兮文＼h
/
/

-1

a
그림 10小34 이산 비주71 신호의 진폭과 위상 스펙트럼 그리기 실행 결과

I

이산 시간 유한 주'I 정현파

연속 시간에서 톤주파수 a)0어］대한푸리어］변환쌍은 다음과 같다．
e/my＜今 22rS(a) -w。
)

(10.21)

예를들어 cos(如t)에 대해 푸리어］변환을 하면 정점은 a)0와 Hn)0 임펄스에 놓인다．

系匹叫同油 i 미sFtTone.m

1 여1제 10켜.18J

이산 시간 유한 주기 정현파가 다음과 같을 때, 이산 푸리에 변환을 이용하여 톤 주파수에 대한 진폭과 위상
을 계산하고 파형을 그려라．
x[n] = 2cos[0.8兀n -1],

n = 0, 1, 2, · ", 20

CHAPTE딕 ]0. 신호 및 시스템

275

三 ! 마5다T가祀Jn ｝芎r苧 1
1 2 3 4 5 6 7 8 9 m H俚 4

풀이

N=2l ;
aet乙tone=2;
omeea0=1J, 8.pi ;
하II＝니 ;
n=0川너 ;

e

尸
e
-

m
m

a-n = amp_帥毗os(omega마n啣）; 0
X_ormega = fft (e_n); 0

H

sub口let 1211) ;

中

中
m

stem(n ,abe (X_omega)); O

title( 겨ago山川eResponse' );
subplot (212) ;

U

尸
尸
m

stee(n, angle (X_om日gafl; 0
title ( 'Phase Response ');

1

-

그림 10-35 이산 시간 유한 주71 정현파의 진폭과 위상 스펙트럼 그리기 코딩 결과（DbFtTone.m)

0 샘플 21개를 지정한다．
0 톤을 생성하는 이산시간유한주기 정현파玎川을 입력한다．
0 航 명령어를 이용하여 玎미을 푸리에 변환한다．
0 stem 함수를 이용하여 진폭 스펙트럼을 그래프로 나타낸다．
0 stem 함수를 이용하여 위상스펙트럼을 그래프로 나타낸다．
F如

E（奴

1띠eW

끄Is잼t

n 二 d dL L뇹

TI丸Is

O吼姓四

쌔4났汁

\ 퀸7 匈 啞 而 ' 曼 口 匡그 田 工工1

'\

Magniti닢計b叩）nsa

10

? 甲 甲 甲 :P9 o

12

14

16

18

5) 巴

巴 口 U 寸

14

16

20

마日se 曲明가isa
n

2
二＞ r,

0

cS O

0

（口 q)

G)

0

윤
-4

0

0

2

4

8

0

10

12

18

20

그림 10-羽 이산 시간 유한 주71 정현파의 진폭과 위상 스펙트렴 그리기 실행 결과

진폭 응답의 아홉 번째 샘플과 열네 번째 샘플에서 2개의 정점을 볼 수 있는데, 이러한 점은 주파수 0.8兀오｝
-0. 勘p어］해당한다．

盆76

PART03. MAT냐＼B활용하기

LESSON

a匿라스 변환

08

연속 시간 푸리에 변환을 확장한 개념인 라플라스 변환은 연속 시간 푸리에 변환과 유사한 성질을 갖고 있다. 라플라스 변환을
이용하여 연속 시스템을 분석하면 좀 더 구체적으로 시간 영역에서의 동작을 볼 수 있다, 심벌릭 툴박스를 사용하여 함수의 라
플라스 변환과 라폴라스 역변환의 결과를 살펴보자，
Key1月ord

I

I 라플라스 변환 1 라푤라스 역변환 1 冶目ace I 陀히ace 1

라플라스 변환과 라퓰라스 역변환

연속 신호x(t）를 라플라스 영역으로 변환하는 라플라스 변환（Laplace trans的rm)은 다음과 같이 정의
된다．

x（昕亡x(加1dt

(10.22)

여기서 복소 변수 s=（了 + JO)이다. 반대로 라플라스 영역의 신호를 시간 영역의 신호로 변환하는 라플
라스 역변확 방정식은 다음과 같다．

1/ "뇨（s)estci노
x(t)＝구－
22rJJ(j／以）

(10.23)

M- 현好

1 예제 10-19 1

La口Tra昭na

라플라스 변환 함수枷）에 대한 시간 영역의 함수 x (t）를 구하고, 시간 0 드 r 드 15[sec］에서 변화하는 工(t）의
파형을 그려라．
+1

7c

X(s) = . 11 ' . ‘.
s(s느 + 2s 十 1U)
而胛

1laplace
변수／를 사용하는 시간 영역의 함수를, 변수 S를 사용하는 라플라스 영역으로 변환하는 것을 라플라스 변환
이라고한다. 이를수행하는laplace 함수의 기본형태는다음과같다．

IapIace(f)
· f: 시간 영역의 함수

CHAPTE日 ]0. 신호 및 시스템

277

1ilaplace
변수S를 사용하는 라플라스 영역의 함수를 시간 영역의 함수로 변환하는 것을 라플라스 역변환이라고 한다．
이를수행하는ila바ace 함수의 기본 형태는 다음과같다，

ilaplace(f)
· f: 라퓰라스 영역의 함수

L且F汀ran&m 挺 丁斗r
이 ear;

e

syms a t
L8=（小的 V佃H$' 小小刊0) ); <1
引 sp( 默引＝ ) ;
4
m
m

pretty(X...s) ;
5-너 回ace I

1
1
尸

나
n

引; 0
x_t=si.pl ify(x. t) ;
diap( 'o(t)=') ;
口r日tty(x_t) ;

1

1 2 口U 4 二U 6 7 8

菖；;

m

1

U
m
小

0 1 9느 nJ 4 二U

t=0:01:15; Q
S肛口＝dou버e(subs（나）) ; 0
plot (t,x..amp); 0

m

slabel ( 'Time (sec) ') ;
비abeI ( 'Aepl itude ') ;
tltle ( 'Pist of Inverse Laplace Transform ') ;
grid;
m

1 ]

n

b
m

1

그림 10-37 라플라스 역변환 코딩 결과(La帥ans.m)

0 라플라스 영역의 함수X(s）를 지정한다．
0 ilaplace 함수를 이용하여 라플라스 역변환을 실행하면 시간 영역의 함수工(t）로 돌아온다．
0 시간 벡터를 0 드 i 드 15[sec］로 지정한다．
0 subs 함수를 이용하여 시간 응답을 구하고, 面uble 함수를 이용하여 소수쩜을 포함하는 수치 형태로 변
환한다．
0 工（t)를 그래프로 나타낸다．

>> Laplrane
X (S)=
2s*

I

2
ala

.2a

. 10)

X (t) =
/
1

eap(-t) I cos(3 t)
甘

10

10

引n(3 t) 19 !
I

그림 10-38 라플라스 역변환 실행 결과

278

:／놔극T 03. MATLAB활용하71

3

/

同挺

日難

蜘曲 It甘M

To아도

r油St뻐） 냄Indow

H帥｝

｛그 g3 日 蜘 臣 斗＼ \ 明自咽 尻 , 目 ] ［그 國 蠱 口
Pit出 of twa田eLapl키月 Tr恥｝前orm

0.

0.5

3

n

2

n
8글互느 ＜

心.1
0

5

10

15

Tin犯（羽c)

그림 i아39 라플라스 역변환으로 구한 함수 그리기 실행 결과

CHAPTER 10. 신호 및 시스템

279

LESSON

09

z변환

z 변환은 연속 신호와 연속 시스템에서 정의된 라플라스 변환 및 이산 신호와 이산 시스템에 대해1 같은 역할을 한다. 시간 영
역0似｛두 신호의 컨벌루션 연산율 z 변환의 유용한 성질을 사용하여 z 영역에서는 단순 곱 연산으로 바꿔 계산할 수 있다, 함
수의 z 변환과 역 z 변환을 사용하여 이산 선형 시스템의 영점과 극점 및 주파수 응답의 결과에 대한 그래프를 살펴보자．
Keyword

I

I z변환 i 영점 1 극점 1 皿map I freqz i 削ane i 역z 변환 1 이mp내se I i才rans i

z 변환

입력되는 시간어］상콴없이 같은 입력어］대해 항상 같은 반응을 나타내고 입출력 관계가 선형인 시스템을
선형 시불변 시스템이라고 한다. 선형 시불변 시스템의 신호를 해석하기 위해 주파수 영역을 변환하지 않
고 직접 z 변환(z比ransform）을 사용한다. 이산 신호玎미 의 z 변환은 다음과 같이 정의한다. 이때 z는
복소 변수이다．

刃＝-m

(10.

n

z-

［刃］

工

2

=

(z)

X

+a)

24)

시간축 n 20에서만 존재하는 인과（causal) 시스템의 신호어］대한 z 변환을 단방향 z 변환이라고 하며，
식 (10.24）는 다음과 같이 다시 쓸 수 있다．

I

2

n=O

n]

=

x[

(z)

X

+m

z

'

(10.25)

전달함수의 영점과 극점

이상 선형 시불변 시스템의 임펄스 응답 力［n] 어］ 대한 z 변환은 전달함수 月仁）가 된다. 만일 전달함수가
, , . . N（기 r1 -,1- 亡， H -人 寸1,-11r1 () -,i人：그 ：了눠r]m , , . . -.1 H口］ , ,. . ,, 0 r1不＋1 __ 0］二］e m7q
H (z) =：쑤끄와 같은 분수 형태의 유리수로 표현되면 H (z) 의 분자八，r(z) =0을 만족하는 위치를 영점
"
D（기
"
"
(zero）이라하고, 분모D（기 = 0을만족하는 위치를극점（p이e）이라한다. 극점 · 영점 그림은z 평면에
서의 영점과극점을보여준다.

280

PA日T 03. MATLAB활용하71

I

주파수 응답

e1w를 따라 계산한 값으로， 전
주파수 응답（freqt妃ncy response）은 전달함수를 복소평면의 단위원 zZ =e
달함수의 극점과 영점을 이용하여 구할 수 있다. 주파수 응답과 전달함수의 관계는 다음과 같다．
月佃）= H (Z)1z =ejm

(10.26)

복소수의 곱과 나눗셈 성질을 이용하여 주파수 응답 //k)) 의 진폭 응답 田（cv) 1와 위상 응답 乙／I ( e/')
를 구할 수 있다．

知卜斜油 i ZTrans.m

W뗀！아犁j

0 드 刃 드 30[sec］에서 이산 선형 시불변 시스템의 전달함수 /／仁刃카 대한 극점과 영점, 주파수 응답을 각각 그

2

2z2

+2 口
于3

z"

小

／카二7=

려라．

배명
지식

1pzmap
시스템 S어］대한 연속 시간혹은 이산 시간의 영점과극점을그리는pzmap 함수의 기본 형태는 다음과같다．

pzmap(S)
시스템 S의 극점과 영점을 열벡터 p와z로 계산할 때 p기ilap 함수의 기본 형태는 다음과 같다．

[p, z] = pzmap(S)
. P: 시스템의 극점
· Z: 시스템의 영점

이 경우 그래프는 나타나지 않는다．
1freqz
시스템 S의 주파수 응답을 그리는 丘eqz 함수의 기본 형태는 다음과 같다．

freqz(S)
벡터 a와b에 의해 계산된 주파수응답을 벡터 h로 나타낼 때 freqz 함수의 기본 형태는 다음과 같다．

h = freqz(a, b)

CHAPTER 10. 신호 및 시스템

281

1zplane
열벡터 z로 지정된 영점과 열벡터 p로 지정된 극점을 현재 열려 있는 그림 창에 그리는 zplane 함수의 기본
형태는다음과같다. 그려진그래프어써 ' O'는영점을, 'x '는극점을나타낸다．

zplane(z, p)
· Z: 열벡터로 표현된 영점
. P: 열벡터로 표현된 극점

I-

f

n=0:30;
num=(I -22- Il ;

2-

1-

풀이

:：『二：
品헒：으,.,.,0

느

4-

3

7-

6-

0-

h=1reqz(num, den); 0
figure (l)
zplane(num, den); 0

grid;
titleC 嫩f{PnIes and Zeroni ) ;
I igure(2)

8-

9
10
11
12

-

treqz(num, den); 0

-

title ( ’猷f-[Frequency Renporise} ') ;

-

그림 10-本） 시스템떽 극점과 영점 그리기 코딩 결과（zT同四.m)

0 전달함수의 분모가 3차이므로 den = [1 000］으로 지정한다. 이 경우 전달함수 분자의 가장 높은 챠수와
분모의 가장높은 챠押｝같으므로 den = [1]로 지정해도 상관없다. 하지만 전달함수 분자와분모의 가장
높은 차수가 같지 않을 때는 반드시 정확하게 지정해야 한다．
Op刀nap 함수를 이용하여 전달함수의 극점과 영점에 대한 열벡터를구한다．
0 丘eqz 함수를 이용하여 전달함수의 분모와분자에 의해1 계산된 주파수 응답 벡터를구한다．
0 그림 창2개를동시어］열기 위해 fi別配 명령어를사용한다．
Oz하ane 함수를 이용하여 전달함수의 분모와분자어］의해 지정된 영점과극점을 그린다．
0 行eqz 함수를 이용하여 주파수응답 벡터를 그래프로 나타낸다.
To아5

Do드kt야） Mndo甘

!4e巾

［뇽 {'\ 戈 抑 兮 4三 Jg , 匹 ［그 圓

m口

Poles and Zeros
毗
的
0
m

亡m口쓰믄弓m口노

m m
m
批
批
也5

0
日eel P名rt

스5

그림 10叫41 시스템의 극점과 영점 그리기 실행 결과

282

PART 03. MAT냐＼B활용하71

口圄屯m鈿t斗m二哺澍毖羽嘴炙霹蜘

｛그 d 日 $

mMm F叫p
4 包＼ 텍b 曲自 喀 在 기 口 口 토크 i 匹 口

m

Fr.qu.n亡yRl片p어出8

0

百므쁨귿듬m>

1
m
的

\

0
的

0.1

02

03

0.4

0.5

0.5

0,7

0.5

聊

I

0.9

1

m

小mm山뇨g므山m믄丘

0.9

Norm出lied Freq此m:y ( X 升 ra四羽mp빠

1\

尸
伽
戶
印
0
0

0.1

02

0.3

0.4

0.5

0.6

0.7

0.8

Nc甘ma虹Gd Frecp好flcy (ocrrad/samp빠

그림］아42 이산 선형 시불변 시스템의 주파수 응답 그리기 실행 결과
［그림 10-41］에서 분모가 0인 점을 만족하는 극점은 ' X '로, 분자가 0인 점을 만족하는 영점은 ' O '로 표시된
n］八11 l, hI. n O In n＼八11,
그그口O 7 I.乙r] L 기O (ci,
n끼］}n] m그i O 7 i. ii.
] + y三
의미한다．3개의
영점은각각 1, 스
다．' 入. '' 위에
나타냔3은 (0, 0）에서 3개의] 극점을갖는다는것을
2
2
.

.

-,］굿hn

\／可

.

-,llt,

'

.]

,-1

느互에위치한다．
2 2

I

역 z 변환

역 z 변환은x口）에서 玎미을 구하는 방법으로 다음과긷히 정의된다. 여기서 C는z 평면 내에서 반시계
방향의 폐쇄 경로이다．

"比

):"

（:

石三3聆

n]

x[

(10.27)

실제로 역 z 변환을 복소 적분식인 식 (10.27）에서 직접 구하는 것은 쉽지 않다. 따라서 역 z 변환어］대한
변환쌍 표와 결합하여 사용하는 부 분 분수 전개를 보편적으로 이용한다．
M-F카e 1 InvZT治ns.m

1 에工II 1fl_ 91 I

시간 0< 刃 드 20[se이에서 전달함수／끄z)에 대한 임펄스 응답 h(n）을 계산하고 파형을 그려라. 그리고 임펄

1)

(4z-

-

z

=

-

H

(z)

스 응답을 직접 구하는 네mpulse 명령어를 이용하여 결과를 비교하라，

4z日 - 2z 十 l

CHAPTER 10. 신호 및 시스템

283

dimpulse

'

；在

지식

전달함수의 분모와분자의 차수를 이용하여 임펄스 응답을 직접 찾는 dimpulse 함수의 기본 형태는 다음과
같다．

dimpulse(num,den,N)
·num: 입력 전달함수의 분자 계수를 내림차순으로 나열한 벡터
·den: 입력 전달함수의 분모 계수를 내림차순으로 나열한 벡터
·N: 표시할 점의 수

1iztrans
z 변환된 수식을 다시 시간 영역으로 역 z 변환하는 iz打ans 함수의 기본 형태는 다음과 같다．

iztrans(f)
·1: z 변환된 수식

삭쁘갸”s.m,yes나塑

a

disp(H(z)=');
pretty(H그) ;

1
1
1
e
e
m
m
m
H
m
m
=

促 田 H 佰 佰 仰 m 四 加 기 左 四 川

1011 -

(nui.

678 9-

-1

num:dlmpulse
0] ;. den=
den.
]4. I!
Iength(n)
;
);
比Z=(ZK巾2너 ))/（巾z-冬各칸I) ;

-

[4.

4
5-

d=

n=0:20;

h_

2 -

3-

풀이

-2

0

h...n=iztrans (H寸z) ; 自
h...ri＝引川니 1 fy(h1n) ;
disp(ht이＝');
pretty (h.j,);
h. amp＝如的 le(subs(h...n) );
subplot (211) ;
stem(nh_.d) ; 0
xlabel ( n ') ;
미 的이 ( h [n] ' ) ;
tltleC Impulse response by 甘bt{dimpuIse} ') ;
grid;
subp lot ( 21 2) ;

stem(n小鈿P) ;0

e

xlabel ( n) ;
ylabel ( hErd ');
tltle ( Impulse response by tbf{ iztrans} );
grid;

그림 10-43 임펄스 응답 그리기 코딩 결과(mv刃哈四.m)

0 전달함수／
／仁）의 분모와분자 차수를 지정한다．
0 dim까小e 함수를 이용하여 전달함수의 분모와분자 차수만으로 임펄스 응답을 직접 찾는다．
0 切的ns 함수를 이용하여 역 z 변환을 계산한다．
0 dimpulse 함수를 이용하여 구한 임펄스 옹답 결과를 그래프로 나타낸다．
0 iztrar好 함수를 이용하여 구한 임펄스 응답 결과를 그래프로 나타낸다．

284

尸A日T 03. M月兀AB활용하기

e)

Corrrrsnd 년nndow
>> InvZTrans
H(Z)=
2 (4 z - I)
2
4z

-2z

+ I

hlnl=
1

n
(니)

/ 2 pi n 寸

-- cosi n
甘

I
/

3

2
그림 10-44 임펄스응답 실행 결과
日le

Edit

너1咐

ln5at

化어s

O哨蚣햐｝ 나In血）叫

He巾

1

D t크 1a 金 自 '\ '\ 聊 @ 咽 i1 , 晶 目 듣그 1a 口

'r

Impul羽 呼pof｝朗 by din叩uls.

6 小 <>
2

4

0

0

6

0

0

0

0

10

8

0

12

0

0

0 0 0

0

14

16

18

0

20

S
Imp미se response by 注trans

우
-0.5

0

0 0

2

4

6

0

8

0

10

0

12

14

16

0

0 0

18

20

n

그림 1아45 임펄스응답그리기 실행 결과

시간축이 n? O인 인과 시스템에 대한 임펄스 응답은 단위 계단 함수 u [n I을 생략한 형태인

力［n]=({)'(. 予小．

CHAPTER 10 신호 및 시스템

285

LESSON

10

디지털 필터

디지털 필터는 이산 신호를 처리할 때 불필요한 성분을 줄이고 필요한 성분을 향상하는 데 사용하는 시스템이다. 특정한 형태
의 주파수 응답을 가진 디지털 필터를 이용하면 필요한 성분의 이산 신호만 통과시킬 수 있다. 필터 설계에서는 영점과 극점의
개수 및 위치를 결정하거나 필터 계수의 값을 결정한다. 디지털 필터는 아날로그 필터보다 복잡한 구성으로 비용이 높다는 것
이 단점이지만. 아날로그 필터보다 더 실제로 사용 가능한 설계를 할 수 있다는 것이 장점이다. 상쇄1 필터와 하닝 창 함수를 사
용하여 입력 신호 중의 불필요한 신호를 제거하는 과정을 그리기 기능으로 이해해보자．
Keyword

I

I 디R 필터 1 상쇄 필터 1 꿰ter I 해닝 창 함수 1 inline 1 hann I

디R 필터

필터는 입력 신호의 스펙트럼을 주파수 응답으로 변형하여 출력 스펙트럼을 생성하는 시스템이다. 유한
구간 임펄스 응답을 가진 FIR (Finite -duration In叩ulse Response) 필터는 출력의 회귀가 없어서 항
상 안정한 필터인 비순환 필터에 대응된다. FIT之 필터의 입출력 관계는 다음과 같이 나타낸다．
n

I

(10.28)

k]

x[

n-

k]

h[

=。

n]

y[

=

싱쇄1 필터

상쇄 필터 (nulling filter）는 불필요하게 신호를 방해하는 것을 차단하고 정현파 간섭 신호를 제거하는 데
유용하다．

cos

일 때， 입력 주파수 +回.

증에서

=

(c00n）

nl

입력 신호

x[

' +z '

이고

-

)z

1

(o。

=

2cos

z]

H[

전달함수

＝

M-File I FirNulling.m

1 예工｛110-22 I

H[기의 상쇄 필터 작용으로 출력 신호y[nj에서 신호가 제거되는 파형을 그려라. 이때F 입력 신호 샘플 51.711
는 0< n 드 50에 놓여 있다．

배병
지식

1filter
filter 함수는 차분방정식 (d姸缸ence equation）에 의해 표현되는 지연선（帥ped delay-line) 필터이다．
filter 함수는 벡터 a와 b로 표현되는 필터로서 벡터 x의 데이터를 처리하여 여과된 데이터 y를 생성한다．
filter 함수의 기본 형태는 다음과같다．

286

PART 03. MA兀AB활용하기

y = filter(b, a, x)
.y: 여과된 데이터
· 라 b: 필터를 표현한 벡터

니 디rNulling.m ：텨 1

느1

12 -.

n =0:50;
omegaU = pi/3;

34567-

凡n = C四（omegaO*n); 0
so = fi lter ([ l -2*cos (ome9a0) 1] ,l, x,n); 0
stem(n,x. .n); 0
hold;
stem(n,y. .n, 'fi l led ', 'r ); C

8-

aoio(L0 50-1 . 2 1. 21) ;

9-

olab日l ( 'n') ;

ID -

이ab이 I, 帥口1 나ude ) ;

II 尸

title ( 'circle: olol, fi l ledcircle: y[ o] ') ;

12

arid;

-

그림 10尸46 상쇄 필터의 신호 제거 코딩 결과（日rNu小四.m)

0 입력 신호玎미을 지정한다．
0 filter 함수를 이용하여 입력 벡터 신호의 데이터를 여과한출력 벡터를 생성한다．
0 stem 명령어를 이용하여 입력 신호玎미을줄기 형태로 그린다．
0 stem 명령어를 이용하여 출력 신호y[,日을줄기 형태로 그린다．
F屯

的t

V1m i哨目t

Tools ［珀＄岫먀,

1

Wln的w 卜相如

｛그 d 1a 白 1 臣 1 戈 戈 好 自 唯I?: 니 目

口 匡크 1 口

出沁：a｛川, 8出이I ck亡le: yfnl

0.5 <:)

OO

g글쥬h쿄

mssssssMSsssMsSssssSsMpuSs

05 寸：)

00

OO

O

upSssss

OO

psssMsss

OO

0

d)

-1

쥴；i

+1

· X: 여과할 필터

5

10

15

衣）

25
n

30

35

40

45

50

그림 10-47 상쇄 필터의 신호 제거 실행 결과

입력 샘플이 n= o부터 적용되었기 때문에 n= 1까지 작은 일시적인 신호가 나타나고, 그 이후의 출력은 상
쇄 필터의 작용으로 정현파의 주파수m0어］대한 정수배에서 0의 값이 나타난다．

CHAPTER 10. 신호 및 시스템

287

히1닝 창 함수

I

창佃md이V) 함수법은각주파수 신호에 대해 정확히 일치하는주파수응답을가진 이상적 필터(ideal f血er)
의 무한 구간 임펄스 응답을 유한 구간 임펄스 응답으로 근사화하고, 이를 통해 필터의 계수를 결정하는
방법이다. 그중 해닝（Hanning) 창함수는 불연속을 없애는과정에서 코사인 함수를 이용하여 중심값부
근을 더욱 강조하면서 부엽佃de lobe）의 성능을 개선한다．

Mm科！e 1 日rHanning.n기

1 （계저I 10叫．23 I

저역 통과(low pass) 필터의 원하는 주파수 응답 /:1쨔功와 원하는 임펄스 응답 幻佃）이 있을 때, 해닝 창 함

=

(Ja <,r/
(

=j

(w)

Hd

月』

11

（0)

수를 이용하여 필터의 차수 M= 21에 대해 구현되는 임펄스 응답과 주파수 응답을 그림으로 나타내라．

1L21)

4)

지식

'

inline

；而

hd[n]＝三Si니枷 쓱긔）
필요할때마다수식expr을문자열로지정한후에수식에서사용하는입력 인자argi, arg2, arg3등을지정
된 수식어］입력하여 수식을 계산하는 血line 함수의 기본 형태는 다음과 같다．

inhine('expr', argi, arg2, arg3,．·· )
. 'expr': 수식
·argl, ar92, arg3: 입력 인자

EiD 日2015b 이후에 출시된 MAT녀B 버전에서는 inline 함수를 더 이상 사용할 수 없다． 대신에 익명 함수 기능을 가
진 (＠을 사용한다．

1hann
열벡터 형태로 표시되는 양의 정수 점 A／개의 대칭 해닝 창 함수를 구하는 hann 함수의 기본 형태는 다음과
같다．

hann(M)

288

PART03』MAT녀B 활용하71

iJFlrHanningm
1M= 21;
2-

n = 0: (14니) ;

3 45-

0me9a=-pi :pj/1ljf:pj ;
c_ f＝이／4;
노d = m山ie(c_ f／이 + 引nc (c_ f/p나(n-Of니 )/2) ) ', 'n . 七_1
比6 = ［址iii艮（' 1+( abs ( em ego) < c_ f) . 七mega . 七-I, );

6-

78-

h_n = h_d(n. c_i, M) .* hann(M) ' ; e
subplot (211) ;

10-

axis(10 14- 1 -0.1, 0.31)
olabel ( s ') ;
미ab日I ( 'hlnl );
title (' HanningLsgpass, 川＝21 ) ;
subplot (212)
H = freqz (h_n, 1, omega) ;
plot (omega, 20미og10(abs(H) ));
hold;
plot (omega, 2마logl0(mao(H_d(omega, c_ f),epa)),
xlabel ( 毋aoega' );
비ab이 ( IH呻叩ega) I (dO) ');
titl이 겨的nitude Response ) ;
aoio(L-pi 口i 니(051) ;

9-

11 12 1314 15IS17IS1920 中
21 끄-

e

stem(n, h_n); O

r: ); 0

그림 10-48 해닝 창 함수 코딩 결과伯rHan대ng.m)

0 주파수응답의 간격을지정하고，차단주파수변수cf어］플를지정한다．
0 inline 명령어를 이용하여 미리 지정된 인자를 직접 받아서 입력하는 형태로 전달함수와 임펄스 응답 함
수를지정한다．
0 해닝 창함수를 이용하여 이상적인 임펄스웅답을구현한다．
0 필터의 차수 M= 21어］대해 구현되는 임펄스 응답을 그림 창 위쪽에 그래프로 나타낸다．
0 주파수 응답을 그림 창 아래쪽에 그래프로 나타낸다．

그림 10-49 해닝 창 함수 실행 결과

주파수응답의 중심값부근에 신호가 집중되어 성능이 향상된다．

CHAPTER 10. 신호 및 시스템

289

J心呼＝ 그二三已： ,F. 쩍y 河 쓰 m斗：r ，已；必 그江 = 1뇨 lL心낟！ 니心m

쏘每和 d心콘 1 必m

mi}

甘r37m

J; m

1 tn

노

4

髓轟難難難驪驥蠶難髓難難鷺驩料翎mmm月쩍rn끼崙

難騷蘿發瑟鹽蔑蟹發饗醬弱蠶捕好咽U目RU月UI侄
難難髓難騷蠶磁蠶韆驢瑟驢鞋瑟蘿心明口U目U及I匹
轟聽驪瑟無鹽烈照難驀臘隘鹽礪駐月R月U口RU月匹
難轟驪醫聽難饉髓醬發驃驪醬驪飄好目III口U口U
蠶難麓難驪驪熬攝難髓蠶蕪蘿蠶發烈只U月月出U口쩝

難蘿雜轟難礪難難蘿驛蘿巍鞠融潮mmm杯杯mm器
蠶難聽難聽饑難難攝鱉難聽驢韜團目U口mmm끼拓

麟難韆難瓘蘿驥驩難難難驥辯斟뾔材棹삐빠빠뼈하g

難纛韆藜難難轉蘿驥髓購蘚驛烈社쩍眸月끼口1m必
驪轟饑難難難難轟蘿購蠟難輯解us. ...在
難驩難難蠱難蘿難蘿蘿難醫單薛蚣棒뼈斗쁘1＝끼U
難蘿難雜難驢難驢蘿黨酩蠱鞋粗明쁘川뼈뼈뼈月月
難羅難蠶轟難蘿難臘驛難蠶難哺님닙A出A니口曳
礪難蘿難臘難麟蠱驪離難鷺雜羅神m社U끼끼＝4

蠶難纛驢難難難難難難斜臘驛뼈mHmmm너너比
繫羅驪髓雜驥驩鹽蘿難蘿繇藻用烈科m=m4m布

鱗鸚韆驢球購麟驪轟聽聰稠鞋擢끼뼈빠＝＝口口m
驢驢鹽籬蠶驪蠶難髓照塑巍好也RURUR月U
難瑟騷巍髓蠶蟹蠶鹽覆髓烈珏RURU口UI月
發難饉蘿難難盈驪觀磁鰍堪明RU口口RU口月
蘿驪離鹽瑟轟髓發凝聽蠶盟U끼UUUUUUR
等뻠牡砦뻠幽堪驩韆蠶難難難驢驢難麴臘轟礎驢撥群驪蠟撰弊目口口끼n口＝끼뗘
鞋戴斟斟補斟麟購饑難蘿轍難驩罐難難難難難驩鞋難鞋麟鮮轟弊杯mmmm杯U桶
難鞋蘿鞋羅拉'U月U口U月喀
群蠱希蚣蘿露鹽難蘿驪難蠱臘鑒難轟鹽攝烈驩
暫烈羽照熬照瑟報難難難驢囊韓韆鸚蕪弊杯驪解 蟹慰轟鱉髓好川口口口RU口咨
發難歿馨嘴輔攝驩醬韆難醬鞋難髓驢難蛙聾耀難難騷韆馨麟斟嫩好川月RU＝川畔
瑟器嫌牲饉醬難難難驢驩轉難轉驩蘿蠱雜煎蘿驩鞋難纛驢難蘿融m口U口口RU唯
器韜鮮淋辯難鸞難難難難鸚難鞋繫驢滯驀斟麟難攝蠶難降嬅礪蜂月m二m==m싸
!1好斜曲越購羅難聽難蠶難難藕蠣轟罐碌融蘿蘿艱髓蘿蠱轉韓蘭州川IRURU쁘
討뽀茗茹嘴鞋驢鞋難難難蠟難臘難難斟핵羅難蘿輯群斛嬅醬雜滋U.쩍'RU기＝
笠斟熬圄發無鞋難蘿驪難驪聽聯難難難麟鞋曄辦群鮮馨嬅群聲뼈耕S月U＝口기U
3：也固芯聲群蘿驢蠶蠶蘿驪蠱難驩轟驩驩發蘿難難驩難難斟難杯好U. -甘U
『，鼠U熙蠣蘿轟驪髓驪繇驢蘿難釀難群醇瞰麟難難蠶驀琿聲曜無舜쩍拉UUUU 二
毖杯帑熙嬅攝蠣難齬難驛饌蘿鞋蘚融胡羅杯嫩鱗難耀驩曝雄麟耀明坦끼＝mm4 \
쿄料群斟稠羅驛難韆蘚鷺轟難驥籬羈轟難群驀麟轉礪馨難崗握姓啣町＝=m=m心
箋斟傑捕韓群韓驩麟鸞難難鞋錨齬難醬難難難難轟難礬嶽鬪斟塔뼈UURIRIR
y甘쩍嬅斟礁翠巖難難韆驪轟蠶難驢鞋罐雖驢韆難難難鞋羅羅料口U口＝=UU 「4
: 枉mm川智虹驥難戀難鞋難驢雖聽難繇藻驛蘿驛聯齒聲韓堪뿌口口U. ...
朴枉mm帛肄難難難難難髓斟灘難轟騷聽韓難羅無邸解班好皿U口'U亡U니m
，』，
\ IRU妊包明發髓難難蠶驢騷凝發國髓嚼聽驢崗嶺黨拉區好皿＝口亡川1UUR
, "U싸뼈草硝堪難驥難韆臘熬礪聲澍萍崗礁嬅肄鷺蹄搏趨驟-U- 口＝-U- :，口＝H拉斟拉礪豫蕪難飄礫聲肆U心唯珌崗驟熙拉聲拉盛뼈쩍1m==== U
1 5m까弗珥曄蠟鞋羅難照爵U固U田川固粗心群甘까쩍끼＝UUUUUU U
5. 텍料拉葬羅驟嬅聲聾聾拉뼈뾰뾰벡堪磁텍뼈叫씨쁘川U口U. 口U. 口
,/ =＝쩍U好皿磁鞋雜肛翅蚣茹mmm心汗芯材뼈川1=a===11=＝口 U
H中小4小＝

＝斗出m呻나心且山汁mmm=

m4月m日득놔＝

H브바＝

mH小小中HH1H小놔山H小中HHHHHH

口＝U. 各好嚼攝磁毖照器U因好出心aUUURU1U口口口--U

H

-

UUU껌也因好磊撰發騈骨月茹斗U月U日URR月RU. .口lUll
I
UURRR쏘姓苾愁醫芯蛋URUR口RRRUURRU口RRUUUUU U
URURU月U區U켜RU口三UUUURRRRUURUUUURUU

CHAPTER

CONTEN 了 S
LESSON 01 벡터
LESSON 02 벡터 좌표계
LESSON 03 벡터 적분
LESSON 04 벡터의 발산
LESSON 05 벡터의 회전
LESSON 06 전하
LESSON 07 가우스 법칙
LESSON 08 커패시터와 커패시턴스
LESSON 09 전위
LESSON 10 경계 조건
LESSON 11 인덕터와 인덕텬스
LESSON 12 라풀라스 방정식
LESSON 13 비오小사바르 법칙
LESSON 14 암퍼때 법칙
LESS아1 15 맥스웰 방정식
LESSON 16 균일 평면파

LESSON

01

벡터

］차원 공간에서 시간, 질량, 거리를 하나의 실수로 나타내는 스칼라（scalar）와 달리, 벡터（vector）는 2차원 또는 3차원 공간에
서 힘, 속도, 가속도를 크기와 방향을 함꺼1 사용하여 나타낸다. MATLAB 함수를 사용하여 벡E倒 기본 연산 및 벡터의 내적，
외적과 삼중적을 계산해보자．
I 단위 벡터 I nomi I 벡터 뺄셈 I d아 1 아oss I acos I

Keyword

I

단위 벡터

단위 벡티 (unit vector) aA는 벡터 A와 방향이 같고 크기가 1인 벡터로 다음과 같은 수식을 만족한다．
여기서 A는 벡터 A의 크기이다．
A

A

aA = 1= = e
IAI
月

I norm
norm은3차원 벡터의 단위 벡터 계수 4,，小，A：를제곱한값을 더한후제갑근 을 취한값을구하는힘수
이다．MATLAB에서 벡터 A의 크기는 norm (A）로 구한다． 예를 들어 벡터 A = 凡a工 + 凡카 + A兀의
크기를 구하는 식은 다음과 같다．

n시H伽，뇨A,2 ＋月，"
I 예工1111-1 I
벡터 A = a; + 2ay - 3a새 대한 단위 벡터 aA를 구하라．
풀이

r쿠

［노rnnlarld '. r1：二＼
>> A= E1 2- 31;

>i magA=norm (A) 0

mag_A =
3. 7417

.> a_A=A/.ag..A e
a_A =
0. 2673

0. 5345

七.8018

그림 서너 단위 벡터 구하71 실행 결과

292

PART03. MAT녀B활용하기

0 벡터 A에 A:, A, A,：를입력한다음norm 함수를이용하여 벡터 A의 크기를구한다1
0 식 (11.1）을이용하여 aA를구한다．

I 벡터 1셉
벡터 뺄셈은 다음과 같히 벡터 덧셈을 이용하여 정의한다．
A -B = A + (-B)
여기서 -B는 B와 크기가 같고 방향은 반대인 벡터이다．

i 예제 11-2 I
벡터 A = 毛 + 2ay 寸3丸와 B = 叫4ay + a：를 사용하여 IA 中 BI를 구하라．

ioI

@
>> A=11 2 -3J;
>> 8=[O -4 ii ;
>> S=A-5
s =
1

6

-4

>> rpag_ S=norm(S) 0
mag소 =
7. 2a미
그림 11모 벡터 크71 구하기 실행 결과

0 벡터 뺄셈 S= A- B를구한다．
0 norm 함수를 이용하여 벡터의 크기 囹를구한다．

I 벡터의 내적
벡터 A와B의 내적 (d야 product）은 다음과 같이 정의한다．
A.B= jAIIBIcosOAB

(11.2)

여기서 9AB는 A와 B 사이의 각 중 180보다 작은 각이다．

CHAP作R 11. 전자기학

293

I

벡터의 외적

벡터 A와C의 외적 (cross product）은다음과같이 정의한다．
AxC= a7i lAliCisinOAc

(11.3)

여기서 꺄은 벡터 A와 C를 동시어］ 포함하는 면에 수직인 단위 벡터이며, 9AC는 A와 C 사히의 각 중
180
『보다작은 각이다．

1 예제 11- 31
벡터 A = a, + 2ay - 3a:. B = -4ay + a小 C = 5a: -2丸가 있을 따1 벡터의 내적 A "B와 벡터의 외적 AX
C를 구하라．

；而
지식

' d야
벡터의 내적을계산하려면두벡터의 크기가긷아야한다. 즉주어진 벡터의工, y, z 성분에서 빠져 있는단위
벡터 부분의 계수도0으로 지정하여, 실행하는 벡터가항상3개의 원소를 갖도록한다．
크기가 같은 벡터 A와B의 내적을 계산하는 面t 함수의 기본 형태는 다음과 같다．

D =（把t(A, B)
벡터 A와B가모두 열벡터인 경우 dot (A.B）의 결과는 A'* B와같다．
1cross
벡터 A와B의 외적을 계산하는 cross 함수의 기본 형태는 다음과 같다．

C = cross(A, B)
이때 벡터 A와B는반드시 원소가3개여야한다．
풀이

>> A=[1 2 -31 ;
>> 0=10-4 11;
>> C=I5 0 -21;

먀）

>> 며느dot（凡B) e
=

]1

>> C小山ss（凡미 0
CF =
4

너3

네0

그림 11-3 벡터의 내적과 외적 실행 결과

294

PART03. MAThAB 활용하기

0 dot 함수를 이용하여 벡터의 내적을 구한다. 그 결과는 스칼라 값이다．
0 cross 함수를 이용하여 벡터의 외적을 구한다. 그 결과는 벡터이다．

I

스칼라 삼중적

벡터 A, B, C의 곱하기는 스칼라 삼중적 (scalar triple product）과 벡터 삼중적 (vector triple
product）으로 나뉜다. 삼중척한 결과가 스칼라인 경우 스칼라 삼중적, 벡터인 경우 벡터 삼중적이라고
한다. 이 중스칼라삼중적은다음과같이 계산한다．
A· (BxC) =B. (CxA) =C. (AxB)

(11.4)

1 예제 11- 4 I
벡터 A = 乞 +2乞 - 3a小 B = -4斗 +a小 C= 5毛 누2a새 대한 스칼라 삼중적을 구하라．

풀이

>' A=11 2 -31; 41

>> B=1D -4 11 ;
" C=15 0 -21;
)' SlP=dot (*,cross(5.C) ) 0
SIP =
-42

그림 11-4 스칼라 삼중적 실행 결과

0 벡터 A. B. C를지정한다．
0 괄호로 묶인 부분의 우소l순위가높으므로 cross 함수를 먼저 사용한 다음 面t 함수를 人卜용하여 스칼라삼
중적 A. (BxC）를구한다．

I

벡터 십충적

벡터 A. B. C어］대한 벡터 삼중적은Ax (B XC ) 이며 다음과 같이 확장하여 나타낼 수 있다．
Ax (BxC) =B(A- C) -C(A.B)

(11.5)

CHAPTE日 ]]' 전자기학

295

1 예저111-51
벡터 A = 戈 + 2朴 - 3a, B = -4ay + a小 C= 5毛 -2丸（川 대한 벡터 삼중적을 구하라．

푿이

)) A=I1 2 -31;
>> B=10 -4 II;
>> c=is 0 -21;
>> YTP=cross(Across(B,C) )
VIP =
55

-44

-11

>> YIP工＝小dot (A, C)-C.dot（凡B) O
YIP上 =
弱

-44

-11

그림 11巧 벡터 삼중적 실행 결과

0 괄호를 이용하여 cross 함수를 두 번 연속으로 사용한다．
0 面t 함수만으로 벡터 삼중적을 계산하는 경우 식 (11.5）를 이용하여 계산한다．

I

벡터 사이의 각

-

o

(

ms-

'

벡터 A와B 사이의 각 0AB는 180c（兀 라디안）보다 작은 값이고, 식 (11.2）를 이용하여 구할수 있다．

1A B

)

1 예제 11-6 I
벡터 A = a: + 2ay -孤：와 B = -4毛 +a: 사이의 각을 구하라．

배경
지식

'
역코사인값을구하는acos함수의 기본형태는다음과같다. 이때 결과는랴디안값으로나타난다．

acos(X)
· X: 코人r인 값

296

PA日T 03. MATLAB활용하기

(11.6)

풀이

Command V미ndc小／

（分

>' A=[1 2 -31; <1

>> 8=10 -4 11;
>> theta_AB=acos(dot (A,8)/(norm(A)*nor.(B) ))*(I日IJ/pi) 0
thetaAB =

그림 11小 두 벡터 사이의 각 계산하기 실행 결과

0 벡터 A. B를지정한다．
0 식 (11.6）을 계산한다. 이때 acos 함수를 이용하여 역코사인 값을 구한다. MATLAB에서는 기본적으
－日 日1 n H1H1八1 八 m . 1.-i. 11_.1 aln _11 1800 := 小＝1H]
로 각을 라디안으로 나타내기 때문에：쓰二를 곱한다．
2r

CHAPTER 11. 전자7I학

297

LESSON

02

벡터 좌표겨I

직교좌표계는 좌표 仁,y,z）가 서로 직교한 상태로 3차원 공간에 놓여 있는 것을 의미한다. 원통좌표계는 (p，中，z) 좌표로 이루
어지며，구면좌표계는 (r，오中） 좌퐈큔 이루어진다. 벡터 좌표계의 상호 변환을 MATLAB의 함수 또는 간단한 스크립트 파일
을 이용하여 실행해보자．
Key叫ord

1 벡터 좌표계의 상호 변환 1 atan2 I

I 직교좌표와 원통좌표의 상호 변환
직교좌표 佃,y,z）를 원통촤표 (p中,z）로 변환하려면 다음관계를 이용한다．
=
p-

／그 . 2
v兀 十y

中 = tan1

2
工

z= z

반대로 원통좌표 巾，中,z）를 직교좌표 佃,y,z）로 변환하려면 다음관계를 이용한다．
工＝pcos砂

(11.8a)

y= psin砂

(11.8b)

z= z

(11.8c)

口d} MATLAB은 좌표 변수의 상호 전환을 위해 cart2p이, cart2sph, p이2car. sph2ca作 함수를 제공하는데. 원통좌표의 입력 순서가 일
반적으로 人용誰nD
oIJ닌
（小,'rn, Z)'이다. 또한 구면좌표에서도 각 e 대신에 }e를 人용하7 때문에 혼란을 일으킬 수 있
' ,, '小,, Z）
"가 .
H "'r
' , '-'. H H '
'1 " 2
1 '' '
다. 따라서 혼란을 줄이기 위하1 사용자정의힘수를 사용할 것을 권한다.

1 예제 11-71

M-File i CarTcyl.m

MATLAB을 사용하여 직교조1표의 점 (2, -3, 1）에 상응하는 원통좌표의 점 (p ，色 z)를 구하라．
(a) 명령 창에 직접 변환 과정을 입력하여 변환하라．
(b) 변환 과정을 포함하는 사용자정의함수를 작성하여 좌표를 변환하라．

298

PA日T03. M酊녀B활용하기

' atan2

；而
지식

역탄젠트값을계산하는atan2 함수의 기본형태는다음과같다．

P = atan2(Y, X)
· P: 라디안으로 표시된 역탄젠트 값
·x ,Y: 실수부의 값

이때의 결과는 [-7t, 兀］ 범위 안어］있는 라디안 값이다．
Command Window
)> x=2;
>> y=-3;
>> z=1 ;

>> rho=sqrt (x'2.y'2) e
rho =
3.

>> phi=atan2(y』x)=(180/pi) 0
phi =
66, 3099
>> 2=2
Z
1
그림 ]1-7 식을 이용한 직교좌표와 원통좌표의 상호 변환 실행 결과

0 식 (11.7a）를이용하여p를구한다．

-a

三-

玎 CarT아m
1 - 투 function cyl = CarTcy1(Car)
-

4-

1j y=X늬노r[1)
"
Car(2) ;
1 Z늬沮r(3) ;

.

11

! rho=sqrt (xnayZ);SJ

-

i cyI(Z)

=phI;

U-

?-

二： 唱毘器！"""田'" 1" e
J:

(b)

0 식 (11.Th）를 이용하여 中를구한다. 이 과정에서 atan2 함수를 이용하여 각도를구한다．

[:：二

（3）끄 "

그림 11田 사용자정의함수를 이용한 직교좌표와 원통좌표의 상호 변환 코딩 결과（Carlc니.rn)

0 식 (11.7a）를이용하여p를구한다．
0 식 (11.7b）를 이용하여 中를구한다. 이 과정에서 毗an2 함수를 이용하여 각도를 구한다．

CHAPTER ]]. 전자71학

299

@

Command Window
>> Car＝汪. 3. 1 ] ;
>> cyl =CarTcyI (Car)
ci i =
3. 60弱

3[l四

i .c｝刃

그림］卜9 사용자정의함수를 이용한 직교좌표와 원통좌표의 상호 변환 실행 결과

I

직교좌표와 구면좌표의 상호 변환

직교좌표 仁,y,z）를구면좌표 (r, 0, 中）로 변환하려면 다음관계를 이용한다．
r

=

sjx2

+y2 +z2

"
0= tan , 1二；
1
m 1

1

y1 X

帥
t
d

반대로 구면좌표 (r,日中）를 직교좌표 仁,y,z）로 변환하려면 다음관계를 이용한다．
x = rsin0cos砂
y = rsin0sin砂
z = rcos0

1 예제 11-8 1
MATLAB을 사용하여 직교좌표의 점 (2,日 ,I）에 상응하는 구면좌표를 구하라．
(a) 명령 창에 직접 변환 과정을 입력하여 변환하라．
(b) 변환 과정을 포함하는 사용자정의함수를 작성하여 좌표를 변환하라．

300

PA日T03. M月TLAB활용하기

M-FiIe I CarTsph.m

佃） Command＼니nd아V

（두）

>> x=2;
>> y＝日3;
)) z=l;

>> r=sqrt (e'2四' 깐Z' 2) 0
r =
3, 7417

>> ,=sqrt (a八2+y八2) ;
>> theta=atan2(,,z).(l凹/pi) 0
theta =
74. 4표蛤
>> phi=atan2(y, x).(l印/pi) 0
phi =
-56.3四9
그림 11너0 식을 이용한 직교좌표와 구면좌표의 상호 변환 실행 결과

0 식 (11.9a）를 이용하여 r을구한다．
0 식 (11.9b）를 이용하여 9를 구한다. 이 과정에서 atan2 함수를 이용하여 각도를 구한다．
0 식 (11.9c）를 이용하여 中를구한다．

(b)

휼苛

CarTspV.m X 斗r
크function aph = Carlsph(Car)
e=Car(1) ;
y'Car(2) ;
z=Car(3) ;
r=scirt (x '2"s' '2'z'2); <1
甘＝sqrt (a八2's'八2) ;

1卜卜卜卜卜卜卜卜n

낙

三

’，客黑然學，仁，守
sph(1)=r;
sph(2)=theta;
sph(3)=phi;
end

그림 11-11 사용자정의함수를 이용한 직교좌표와 구면좌표의 상호 변환 코딩 결과（CarTsph.m)

0 식 (11.9a）를 이용하여 r을구한다．
0 식 (11.9b）를 이용하여 0를 구한다. 이 과정에서 atan2 함수를 이용하여 각도를 구한다．
0 식 (11.9c）를 이용하여 中를구한다．
도）

Command Window
>> 6ar=[2,-3, I1;
>> 하巾＝CarTs的(Car)
sph =
3, 7417

74. 4986 -56. 3099

그림 ]1-12 사용자정의함수를 이용한 직교좌표와 구면좌표의 상호 변환 실행 결과

CHAP1匡A ]]. 전자기학

301

LESSON

03

벡터 적분

선 적분은 적분을 따라서 움직이는 큰 폐쇄1 경로를 선택하고 이를 매우 작은 부분으로 나누어 따로따로 적분한 후 각 부분을
더해서 구한다. 곡면 적분은 곡면에 대한 정적분을 계신后陪 것으로 선 적분의 이중 적분 해석과 같다. MATLAB의 심벌릭 툴
박스를 사용하여 선 적분과 곡면 적분을 계산하는 스크립트 파일을 작성해보자．
Key＼사ord

I

i 선 적분 I subs 1 곡면 적분 1

선 적분

선 적분（line integral)은 함수의 곡선을 따라 이동하면서 적분하는 방법이다. 다음 식의 적분 구간은
0
0
0
（工o, Yo, z0) -+(x1, Yo , z0) -' (x1,乃, z0)수（x1,力戶D과 같이 분할한다．
H = /／工a工 + Hay + Ha:
경로O은工성분만初에서차로, 경로O는y성분만Yo에서Yi로, 경로O은z성분만zo에서z1로이동
하면서 각각 적분을 계산한다. 이를 다음과 긷삐 나타낼 수 있다．

뇨＝加·dL=/“月，d,=，口＝
= j H dL
j x。H I 。, 。dx
，砂+J,I.z1
z。,H m, dz
：伊，
+f", H
／
如，1: :,, =,
M-File I Linelnt.m

1 예제 11-9 !
다음과 같이 자기장과 직선 분할 경로가 주어져 있다．
H = 2乂yza: ＋工2zay ＋尸ya2 [Aim]
0
0
0
(0, 0, 0) 수 (2, 0, 0) -(2, -1, 0) -(2, -1, 4)
심벌릭 툴박스의 폐쇄 선 적분을 사용하여 자기장에 대한 폐쇄 전류를 구하라．

；而
지식

'subs
현재 심벌릭 수식어써 사용巧｝는 심벌릭 변수를 다른 심벌릭 변수 또는 숫자로 대치하는 subs 함수의 기본 형
태는다음과같다．

302

PA日T03. M月T냐＼B 활용하71

subs(E,x,y)
1 E: 심벌릭 수식
, X: 대치할 심벌릭 변수
· y: 새로운 심벌릭 변수 또는 숫자

U,녑ntm
X +
syms 0 0 0

풀이
2-

1-

4 = [2.a*y*z,a'2*z,a'2*yJ ; 0

7-

6-

5-

4-

3-

mmn_a = 0;
max_a = 2;
川1y = -1 ;
max_y = 0;
이0그 = 0;
.ax_z = 4;

9-

0-

Pathi = subs(A (1),(y,z),{.ax. .y,min그)); e

-

-

-

-

小

10
11
12
13
14

m

-

I陌th1 = Int (Pathl,a,min_x,max. .x) ; 0
Path2 = subs (A(2),4a, zL (maxx . 이n..카) ;
1Path2 = int (Path2.y,max_y . 川n_y) ;
Path3 = subs (A(3) 』｛a , y} . {max_a . 川n. y));
叩ath3 = Int (Path3, z .min_z, max. z) ;
니neintegral 끈 I Path I티Path2니Path3 0

그림 作13 선 적분율 이용하여 폐쇄 전류 구하71 코딩 결과仙1님nt.m)

0 자기장을 지정한다．
0 subs 함수를 이용하여 심벌릭 수식 A (1）의 변수 y, z 대신에 y의 최댓급b牡의 최솟값으로 대치한다．
Omt 함수를 사용하여 적분 변1뇨를 가진 피적분함수 Path1어］대한 적분을 계산한다．
0 분할한3개의 경로를 더하여 폐쇄 전류를 구한다．
Command Wind口叫
>> Lineint
Lineiritegral =
니6
그림 11너4 선 적분을 이용하여 폐쇄 전류 구하기 실행 결과

6개 경계면 兀0 5 工 5 丙 , Yo 5Y 5Yi, Z0 5Z 5 긔 에 둘러싸인 벡티장 A= A工a工 + 小ay+ 4毛는다
음과 긷히 계산한다．
앞면 工 =x1에서는A工 성분만 표면에 수직을 이룬다．
A ' a외戶Ont = 겊x Ix= x1（机亡

JJA ' 刻加，, 丁，7뇨니方d느
CHAPTE日 ]]; 전자J빡

303

뒷면 x ＝工0에서도A工 성분만표면에 수찍을 이룬다．
A ' d히ba比 = A小蜘 H加劫

小 ' 刻，ack =/",,' /",,AI＝匈（－方比）
오른쪽 면Y = Yi 에서는小 성분만표면에 수직을 이룬다．
Y=Yi,dx毗
A ' d이ri뇽加 = Aly=y

小·小岫，丁，I JPXInXA
Yy_y1砥比
왼쪽 면Y = Yo에서도小 성분만표면에 수직을 이룬다．
YY。
, (-dr比）
A ' d히left = Aly:y

小·d짜／/Vm抄,(-威比）
윗면z = z1 에서는AZ 성분만표면에 수직을 이룬다．
A ' d히加p = A니：=:, d的7

小' d외，
叩 =/:，月A니：=:，威力
아랫면z = z0에서도A, 성분만표면에수직을이룬다．
A ' d뇌b아torn = 月：나J＝衣力）

，A뇨d砥力）
ffA ' d히切加，寸丁’
위에서 계산한 각칵의 적분값을 더하면 폐쇄 곡면의 척분값이 된다．

304

PA日T 03. VLAT냐＼B 활용하기

1 （川저I 11- in I

M-FiIe I Surflnt.m

0< 工 <2, 크 5y 5 0. 0 5 Z 5 4의 경계에 벡터장 A가 있을 때， 이 경계의 표면에 대한 폐쇄 곡면 적분
#A " 小릍계신后빠．
A = 2刃／za: ＋工2zay ＋尸ya。

iJSurftnt.m
1-

1

풀이

56=

synsxyc
A= [2士）卄y*z . x坦坦坦, a人2*y] ;
m in1X=0;
rnax. x=2;
roirLY니 ;
nao...y늬｝;

7-

o in...z=O;
rnao. .zr4;

4 5 6 7 B 9 m n 促 口 H 陌 佑 作 冊 四 게 기

23-

front=subs(A (T)』x,maox); 0

1

front늬nt ( 吐(front ,y川哨，ma柚）,Z帥二m眺기 ; 0
back=-nubn(A(1Ln.min...x) ;
Ibackrint (Int (back, y .min. y . mao. y),z ,min_z, max. z) ;
right=subo (A(2),y .max_y) ;
I r; ght=Int ( int (rIght .x . 미n口n, maa_o) ,z , in_z .max_z) ;
left=1subs(A (2) 』y . 이n_y) ;
1 let t=lnt ( int ( let t. x,.in. o .max_o) . c , 川n_c . mao. .z ) ;
top=subn(A(3Lz,max_z) ;
It op=1 nt ( mnt (t op . a .m in_x . oaO_o) . y . 미 n.y . maa_y ) ;
bott om=-subo (A ( 3) , Z . m in_c ) ;
나）ottor=int (int (bcttom.x .miri...x』mao口nLy,min_y,maxy) ;
1

U

1

e

e

U

U

e

U

U

1

Surfac帥tegr岫front티bock니曲베帥*It咐加ttoM e

그림 11-15 폐쇄 곡면 적분 구하기 코딩 결과（Surflnt.m)

0 subs 함수를 이용하여 심벌릭 수식 A (1）의 변수工를 工의 최댓값으로 대치한다．
0 mlt 함수를 이용하여 적분 변수）릍 가진 피적분함수 丘ont어］대한 적분을 계산하고 다시 적분의 변수z에
대해 적분을 계산한다．
0 폐쇄 곡면의 적분값을 구하기 위해 앞면, 뒷면, 오른쪽 면, 왼쪽 면, 윗면, 아랫면을 적분한 값을 모두 더
한다．

>> Surf mnt

今

Surfoceintegral =
16
그림 ]1-16 폐쇄 곡면 적분 구하기 실행 결과

CHAP1匡A ]] . 전자기학

305

LESSON

04

벡터의 발산

벡터에서 발산은 벡터장이 한 점에서 장이 퍼져 나오는지, 아니면 모여서 없어지는지를 측정한다. MAT나＼B 스크립트 파일을
작성하여 직교좌표, 원통좌표, 구면좌표에 대한 벡터의 발산을 구하는 과정을 살펴보자．
Keyi사ord

I

I 벡터의 발산 1 쇄mplify I

직교좌표에서 벡터의 발산

직교좌표에서 벡터의 발산（d加ergence）을 구하는 식은 다음과 같다．

d如D＝쁘h므뜨＋쁘
ax

y

az

벡터 미분 연산자 델（del)을 사용하여 구하는 식은 다음과 같다．

V . D＝므츠＋쁘쓰＋쁘三
ax

1 （비저I ll_

Il

ay

az

M-File I DivCar.m

I

직교좌표의 점 (2,1,0）에 있는 벡터 D의 발산을 구하라．
D= 10工v2(z+I冶. +10工2y化＋1杻., +5工2v2a,
/

；而
지식

\

/

n

/

\

r

e

복잡한형태의수식E를좀더 간단하게나타내는simplify함수의 기본형태는다음과같다．

, E: 간략하게 나타낼 수식

1D汁C計．
m X난l

1234-

syms x y Z
D=I10*x四'2.(z너) 10* x '2*y.(z너),5*x '2*y '2] ; 0
divD=diff (D(1),x)+diff (D(2),y) dLff (D(3),z) 0
subs(divD』{s』y, z} A2I . Ofl0

그림 小17 직교좌표에서 벡터의 발산 구하기 코딩 결과（DsCar.m)

306

/

' simplify

simplify(E)

풀이

戶

PART03. M戶TLAB활용하:7 '

0 벡터 D를 지정한다．
0 小什함수를 이용하여 D의 工, y, z 성분어i 대한 미분을 계산한다．
0 subs 함수를 이용하여 수식 d加D의 변수工, y, z를상숫값2, 1. 0으로 대치하여 발산을구한다．
C口mr,1訊d \'indrw
>> ［기yCar
dioD =
10士Xn2士（z + 1) + 10士1／八2士（z + ] )

020 =

E刃
그림 11-18 직교좌표에서 벡터의 발산 구하기 실행 결과

벡터 D의 발산을구하는 식과 점 (2. 1. 0）에서의 발산값이 명령 창에 나타난다．

I 원통좌표에서 벡터의 발산

J-

t9D

+1

P)

(PZ)

.

a

V

D=

원통좌표어써 벡터의 발산을 구하는 식은 다음과 같다．

/) 帥

op

p

+ aD

aZ

1 （川저I 11- 12 I

M-File ! DvCyI.m

원통좌표의 점 (4, 30已 m기에 있는 벡터 D의 발산을 구하라．
pz . r
八
1
八 2
U = 4中小sin口a, + 乙ozcos (Pa小 + 乙／) sin(Pa,
2
'

尸

"

"

DivCyLm 恥：r到

풀이
n
d

24

syrfis rho 아니 Z
D= frho*z*sin(phi) /2,2*rho*z*cos(phi),2.rho'2*sin(phi) ] ; 0
disD=(l/ rho)*diff (rho士D(1) ,rho)*(I/rho)*difl(D(2),phi) *diff (D(3) .z) ;

=
U

客：::',:(，‘쀼，魚．印，(,,/，印）
: diS0：
』丑｝
)<)

그림 l］小］9 원통좌표에서 벡터의 발산 구하기 코딩 결과（DivC닌.m)

0 벡터 D를 지정한다．
0 simpli勺 함수를 이용하여 수식 d加D를 간단한 형태로 나타낸다．
0 subs 함수를이용하여 수식 divD의 변수p, 中, z를상숫값4, 30', -2로 대치하여 발산을구한다．

CHAPTER 11. 전자기학

307

回

Command＼사［ndow
>> ［키 닉Cyl
diaD =
尸Z士sin(phi )

ans =
1
그림 价20 원통좌표에서 벡터의 발산 구하71 실행 결과

벡터 D의 발산을구하는 식과 점 (4. 30g. -2）에서의 발산값이 명령 창에 나타난다．

I

구면좌표어써 벡터의 발산

구면좌표에서 벡터의 발산을 구하는 식은 다음과 같다．

「勺功＋ 1 a(sinOD9) + 1
\7 . n＝끄 （
" 尸 r2 3r
rsinO
aO
rsinO a砂
따

1

L여뗀 11-13J

M＋加 1 미vS的nl

구면좌표의 점 (1, 300, 600）에 있는 벡터 D의 발산을 구하라．
11

r . ,,

.

cosO

,

. ,l

,

LI = - sinu cos qar + 二＝ 印S甲a8 -sint八；
Os甲a中
sinJ
J

풀이

phm
I 23
45
67-

+1
syis r theta phi
4
D=[ (r/3)*sin(theta)士cos(phi ) .(cos(theta)/引n(theta) )*cos(phi),
-sin(theta)士cos(phi) ] ;
divD=(I/ (r '2)).difI(r '2*D(l) ,r)o(I/ (r*sin(theta) ))山 0
*diff (引n(theta)士D(2) .theta)o(I/ (r*sin(theta) fl *dj ff (D(3Lphi) ;
djvLsiipI ify(diyD) 0
doubIe(subs(diyD,{r.theta,phik』{1.印.(pi/laJL60*(Pi/l印) })) 0

그림 作21 구면좌표0和d 벡터의 발산 구하기 코딩 결과（DivSph.m)

0 벡터 D를 지정한다．
0 식 (11.14）를 이용하여 벡터의 발산을 구한다. 줄임표（···）는 현재 명령줄혀］ 이어 다음 줄을 연결하여
하나의 명령줄이 되도록 한다．
0 sin叩血y 함수를 이용하여 수식 divi）를 간단한 형태로 표시한다．
0 subs 함수를 이용하여 수식 d加D의 변수r, 0, 中를상숫값 1, 300, 60"로 대치하여 발산을구한다．

308

PA日T 03 卜船ILAB 활용하기

Command \'lindcw

今

>> [) vS帥
divU =
（引n（아1i ) 느 cos(phi) + r士cos(phi)*引n(theta) )/r

ans =
0. 6160
그림 11-22 구면좌표에서 벡터의 발산 구하71 실행 결과

벡터 D의 발산을구하는 식과점 (1, 300, 600)에서의 발산값이 명령 창에 나타난다．

CHAPTER ]]. 전자기학

309

LESSON

05

벡터의 회전

회전은 3차원 벡터장에서 아주 작은 회전 벡터로 정의되며, 단위 면적당 최대 순환의 크기와 이 면적의 수직 방향을 갖는다．
MAT나＼B 스크립트 파일을 작성하여 직교조F표, 원통좌표, 구면좌표에 대한 벡터의 회전을 구하는 과정을 살펴보자．
1 벡터의 회전（직교좌표, 원통좌표, 구면좌표） i

Key出ord

I

직교좌표에서 벡터의 회전

직교좌표에서 벡터의 회전을 구하는 식은 다음과 같다．

毛 으七 m

b a1
匈瓦

凡a 缸 瓦

VxH=

raH1,
H 1
raH, 3HVi
raH. aH,i
=I- -------Iar +I- ----口Iat, +I_ H_ _
iaZ
j
a工 j - t 工
azj " L az
[ a))

. (11.15)

M-FiIe I CurlCar.m

1 예工II 11- 141
벡터 H에 대한 회전을 구하고, 점 (1, -2, 3）을 이용하여 구한 회전의 결과를 평가하라．
H = 刃凡 + 缸婢y + ya:

: ! Curk：前j1}

235-

4
5

弑

syms x y z
H=[y士z. 4士S士yJ yj ;
cur나I=tdiff (H(3),y)--diff (H(2Lz) di H (H(1),z)-ditf (I1(3),X)
diii ( H(2) . x)-d it I (H( 1). y) ] ;

1-

풀이

小

4

0

:
二：杆，::',:',：二쌥.,包나.카，,<)

그림 서-23 직교좌표에서 벡터의 회전 구하기 코딩 결과（CuriCar.m)

0 duff함수를 이용하여 벡터 H의 x, y. z 성분에 대한 미분을 계산한다．
0 simpli勺 함수를 이용하여 수식 curlH를 간단한 형태로 나타낸다．
0 subs 함수를 이용하여 수식 curlH의 변수工, y, z를상숫값 1, -2, 3으로 대치하여 회전을구한다．

310

PA日T03. MA凡AB활용하기

Command Window
>> Cur mar
curlH =
[ 1 . p, 4ay - Z}

an 三 =

그림 11-24 직교좌표에서 벡터의 회전 구하기 실행 결과

벡터 H의 회전과 점 (1, -2, 3）에서의 회전 결과가 명령 창에 나타난다．

I

원통좌표에서 벡터의 회전

원통좌표에서 벡터의 회전을 구하는 식은 다음과 같다．

誓

18HO

ii a(pH)

aH, 1
+=

1 1d中 小 H1=1 i a，人 十 1 HH
n_
'1_ I 'V
I ..
[. O乙
('p J
[. p
H

P
a

HP

H

p t9p

쁘帥
l P

V, F

丸 으出 m

抑aH却叫

aP
［그 a

I

2）

(I좋，

H에

대한회전을구하고，점

yr
11 =

풀이

1 t月O 1

1mH尸 i a.
4

下,

1,i

I

U甲 -I

e

를이용하여구한회전의결皓평가하라·

m m二＝ 上n
. m2 m
n m 1_
PSIIII厘I '-, 十 I) 乙a小 十 乙 euswa.
r
느
J/

1

y

'ISlS,Xrh學,
H'毗yim
234

op

'

M-File 1 CurlCyl.m

1 예저1 11- 15 I
1中m二二1---J

벡터

's =

녑

l=1rho.sIn(phI), rhoA2士z, vcos(phIfl;
curl十네If C HC 3) ,P川）/r加m미ff (H(2),z) diff (11(1),z卜미I f (H(3),rh이山 <I
diff (rho*H(2),rho)/rho너lff (H(1),phl)/rhoj;

믐： 二：
，「幷，:::::(,：二口
「，
熄．z},{1,pl/6．라）)<)

그림 小25 원통좌표에서 벡터의 회전 구하기 코딩 결과（CuriC닌.IT今

0 duff함수를 이용하여 벡터 H의 p, 中，z 성분에 대한 미분을 계신한다．
Os血叩lify 함수를 이용하여 수식 curlH를 간단한 형태로 나타낸다．
o subs 함수를 이용하여 수식 curlH의 변수／), 中, z를싱숫값 1, Z1, 2로 대치하여 회전을구한다．
6

CHAPTER ]] 전자기학

311

Como그and Win（妃w

@

>> Curl 口／ 1
curlH =
[

rho坦

(z士sin（口hifl/rho, 0. 3士rhu* z - cos（아lU

5115 =

2. 0000

5. 1340

0

2）

벡터H의회전과점

（1좋，

그림 11-26 원통좌표에서 벡터익 회전 구하71 실행 결과

에서의회전결과가명령칭어］나타난다·

I 구면좌표에서 벡터의 회전
구면좌표에서 벡터의 회전을 구하는 식은 다음과 같다．

1

a,.

ra9

rsinOa砂
0

VxI{ =
' -- r2 sinO 0r

3

0
30

帥

H,
.

rH0

rsin0H

『怖） 흐뜨］抑
『月中）
］抑*![a（
m) 반｛이：, +-［구1．흐牛 a（
．
: rsinui
l .[a( '"甲
r L or
au7 J
r Lsinu o甲
or j
dU
dq) J

M-FiIe 1 CurlSph.m

1 （네저I 11- IA I
兀1
6

즛）
를이용하여구한회전의결ii?

.욜평가하라·

벡터 H에 대한 회전을 구하고, 점

H = 2rcos9cos中a: +r1'2a0

푿이

j_J Cwlsph.m 55
syms r theta phi
12H=12竹.cos(theta)*cos(phi), 0』rn(1/2)1 ;
3curlH=[(diff (引n(theta)*H(3Ltheta)녀itf (H(2).phi))/(r*sin(theta) )
(di ff (H(1),phi)/(sin(thetafl-di I f (r.H(3),rfl/ r. . .
4
S
(dlll (r士H(2) . r)너itf (It(1),theta) )/rl;

67:

二：
，『杆，::’，二’
，:',：二쏀．,0theta,phiL(I,pi/6,pi/3})) C

그림 11-27 구면좌표에서 벡터의 회전 구하71 코딩 결과（Cu作Sph.m)

312

PA日T 03. M月T냐＼B활용하기

0 duff함수를 이용하여 함수표의 r, 9, 中 성분에 대한 미분을 계산한다．
0 sin叩lify 함수를 이용하여 수식 C出1-I를 간단한 형태로 나타낸다．
fl subs 힘：수를 이용하여 수식 curlH의 변수r. 0. 砂를상숫값 l , 프. 프로 대치하여 회전을구한다. 그리고
'
6 3
面uble 함수를 이용하여 소수쩜을 포함한수치 형태로 변환한다．
Command Window
>> CurSph
ans =
1 7321

-4. 5000

0. 5000

3）

'

증

벡터H의회전과점

(1，

그림 ]1山28 구면좌표에서 벡터의 회전 구하기 실행 결과

에서의회전결과가명령칭혀1나타난다·

CHAPTER] ]. 전자기학

313

LESSON

06

전하

전하 q는 물질이 갖고 있는 전기의 양으로 단위는 쿨롱（Co내0mb）이다. 전자가 갖는 전하는 -e로 나타내는데, 그 전하의 양
e =1.602X10小［C］과 같다. 따라서 6.242x 10田개의 전하가 모여 1[C］이 된다. MATLAB 스크립트 파일을 작성하여 점전
하, 선전하, 표면전하에 대한 전기장을 구하는 과정을 살펴보자．
Keyword

1 점전하로 생성되는 전7짱 1 쿨롱의 법칙 1 선전하로생성되는전:7짱 i
! 표면전하로 생성되는 전기장 1

I

점전하로 생성되는 전기장

위치 벡터 r1과 r2어］놓여 있는 점전하（poii표 charge) qi과 q2가 거리 R만큼 떨어져 있다. 이때 qi 어］
의해 q2가받는 벡터 힘을 나타내는 쿨롱의 법칙 (Coulomb's law）은 다음과 같다．
4q

1q2

12

4,

且2=

rs。
R

2aR

I,

여기서 상수80를 자유공간의 유전율（pern血tivity）이라하고 그 값은 다음과 같다．

6n = 8.l54X l (J
"

-

.

-

.

.

,

IU+

3&

--

1

.

-

-

전끼장E는F12를q2로 나누어 구할수 있는데 이를 다음과긷미 나타낸다．
E==

q , FL
4,rc0 I R I"

(11.20)

N개의 점전하q1, q2, ' " , 伽이 위치 벡터 rl, r2, ···,rN에 각칵놓여 있을 때 위치 벡터 r에서의 전기장
은 다음과 같다．

E＝그긍qk(r -rk.)
47rc0 念｛ 江 r뇨 Ii

314

PART03. MA兀AB활용하기

M-File

1 여江fi 11- 17 I

PtChar.m

점전하 크 [nC], 4[nC], 3[nC］가 각각 (0, 0, 0), (0, 0, 小1), (1, 0, 0）에 있을 ［대1 좌표（크，1, 2）에서의 전기
장을 구하라．

町割
1J1 -叱tw.m
epsi
m

t 2 3 4 5 6 7 89 m n俚 口 m巧 怜 口 侶

풀이

=

2=
345670910 Ii 12 1314 =
IS 16 1? m
m
n
1
H
e
e
m
1
m
=
=
1
1
e
1

10 -

lon먀B·田40너2; 0
이＋m召；
q2=4日口9;
q3=3e-9;
r=［너 I 21 ;
rl=1000I;
r2=[0 0- 1] ;
r卞[ 1 00] ;
R1=r-rl ;
F?=r-r2;
B3:'r- r3;
.ag.ill=norm (R1) ; 0
mag_92=nor.(R2) ;
mae口日3=no r目（R3) ;
E1=g1/(4ap1. epsi lon마magJ41'3).Rl ; 0
E2a2/(4'pl. epsl lonO*maeJeA3)士R2;
E3口031(4*이士Op引 I onO*mag_R3A3）奸13;

m

巳E1，口，E3 e

그림 ]1-29 점전하로 생성되는 전기장 구하기 코딩 결과伯Char.m)

Oeo 값을 지정한다．
0 norm 함수를 이용하여 벡터의 크기를 구한다．
0 전기장을구하기 위해 식 (11.21）올 계산한다．
0 서］ 전기장을 모두 더하여 전체 전기장을 구한다．
Command 卯in巾列／
>> Pt Char
E =
-2.3712

1 .37拓

3刀宬E

그림 셔-30 점전하로 생성되는 전기장 구하기 실행 결과

I

선전하로 생성되는 전기장

선전하恤e charge）어］서 생성되는 전기장은 다음과같다．

느三，小츨川？/m}

(11.22)

여기서 pZ[C/m］는 선전하 밀도，[’ 은 전하가분포되어 있는 선을나타낸다· 선 요소는원점으로부터 임
의의 工' 까지의 거리 dt'= dx'으로 나타낼 수 있다．

CHAPTER ]] . 전자7빡

315

벡터 R은다음과 같다．
R = a可）-a工工'

(11.23)

미분 선전하요소 p1dt'=／恥加' 때문어］발생하는 전기장 dE는 다음과 같다．

兆＝巴app_
p2+，岑如民*3쿄瓦

(11.24)

식 (11.24）를 적분하는과정에서 a: 성분이 상쇄되므로dE 부분만 적분하면 된다. 이때 무한히 긴 선전
하의 전기장은 다음과 같다．

／若，(Co
f_C。
(,二 3/2끼Pd?,
rc。,p [V／蝴

E= a

(11.25)

M-File 1 LineChar.m

1 （계저I il- igl
[= :=:==1二二J

자유 공긴뻬서 工축을 따라 ／가 = 3 [nC/i미인 무한 선전하가 놓여 있을 때 좌표 (3, 寸3, 4）에서의 전기장을 구
하라．

풀이

늑U帥，。I。n峀缸：,,

꾜

rho_I＝鈿-9;

r＝田 -3 4] ;
匕ctr=]3 0 0] ; e
匕steps=llom그；0

먀o=norm( r-匕ctr) ;
lenet h=1 00町ho
del=Iength/I口steps.I1 0 미; 0
de=norm(do1) ;
巳11ne=]0 0 미 ; 0
匕Ct r_s日g=1_ctr-(匕ot eps/2.dx卜山d /2) ;

ifor 1=1 :1:1_steps 0
R=r-匕Ctr日see;

.ag_F1괘orm (R); O

end

E. I Ir氾＝E그 ine.ds*rho_I/ (4＋이 始四i Ion0+mag_R人3)+R ;
匕ct r_seg＝匕Ct r_ee日＋dxl ; 0

EEI Inc 0
그림 作31 선전하로 생성되는 전기장 구하기 코딩 결과（나reChar.m)

0 工축어］놓여 있는 선전하의 중심을관측쩜의 工 성분만을 가진 lctr = (3. 0, 0）으로 지정한다．
0 무한 길이의 선전하를 동일한 작은 선전하 간격 1_steps = 100000으로 나누어 선전하어］대한 전기장을
구한다．
0 工축에 놓여 있는 선전하의 길이를동일한 간격으로 나눈분할 벡터 d1을 설정한다．
0 전기장의 초기 상태田_line = [000｝을 지정한다．

316

PART03. MAT녀B 활용하기

01부터 100000까지 반복하여 분할하기 위해 for문을 지정한다．
0 첫 번째 분할의 중심에서 관측점까지의 벡터 R을 지정한다．
0 100000번 반복 실행에 대한i번째 분할의 중심을 지정한다．
0 좌표 (3, 小3. 4）에서의 전기장을지정한다．
Con기rr크od \VindOw

@

>> Line다iar
E =
Ii ［刃00

-6. 4699

0. 6各；5

그림 11-32 선전하로 생성되는 전기장구하기 실행 결과

I

표면전하로 생성되는 전기장

표면전하（surface charge）에서 생성되는 전기장은 다음과 같다．
。

rJ= -i

1

/ -*1月p z- a)
工，r1r/"-]
i v/ L11I

4ns0JS'

Rz

..

-

(11.26)

여기서夙［C/rn勺는표면전하밀도, S'은전하가분포되어 있는표면을나타낸다．

1 여ixi ii-

M-FiIe I SurfChar.m

iq I

］
와 -1 5y 드 1[rn] 영역 안 ,＼』Z평면에 p5 = 3 [C/rn2] 인 표면전하가 있을 때 좌표 (0, 0, -3)
-3 5 工 5 3[rn
[I미에서의 전기장을 구하라．
SudCh可J1l

多： +

B口si 1on00. 054e니 2;
rho_n＝出4;;

e
m

P=10 0 -31;
已surf=l0 0 01 ;<1

1
U

s_steps=100;, y_steps=100;e

느

s_I o,er- 3;J n_u口per=3;
p_ lace r=니;, y_upper=l ;

m
小
1

9

dX=m叩per-s_lacer)／凡敬epa; e

寸
H

0

1

（．니）
.．血；

m

' " "

1
U

무 ：劣；:::：二．

m
H

U 4 二U nD 7
0 1 9느 Q
1
! 1 1
1 1 1 1

dy=(y긔pper四_lo.er)/y_ste口a;
ds=dx.dy;
dq=rho十的；0
日lor J=l: y_steps
1
:/．小

U n
b n
r 8
1
1 2 A
口 4 二

풀이

1

冊 四
四

I

90」
, , ,

E_surf 毛surfs (dq/(4.epai lono.pkmagJr3) ).R

end

기

end
탸．댜urf 0

그림 11-33 표면전하로 생성되는 전기장 구하기 코딩 결과（SurfChar.rn)

CHAPTER 1] 전자71학

317

0 표면전하에 대한 전기장을 구하기 위해 초기 상태 Ee引irf= [O0 0｝을지정한다．
0 工축과y축방향으로분할한값, 표면전하가놓여 있는工 값의 범위와y 값의 범위를 지정한다．
0 표면을 아주작은크기의 dt와力로균등하계 나누어서 해석한다．
0 각 셀은 전하 dq = Pd六力／를 갖는다．
0 각좌표의 셀 증심 위치는 다음과 같이 놓는다．
cfr . . . . .
. dy , . . . .
1\
工 == -3 + =e + a杖i-1) . y = -1+ 亡m + ayu -1), 乙 = U
2
2
O (0, 0, 놔3）에서의 전기장을구한다．
Command 邪indn닉／

군）

>. SurfDnar

E
] . Oe+04 士
0. 0000

0. 0000

-2. 4323

그림 11-34 표면전하로 생성되는 전기장구하71 실행 결과

318

PA日T 03. MAT냐＼B활용하71

LESSON

07

가우스 법칙

가우스 법칙은 닫힌 표면에서 표면을 통과하여 밖으로 향하는 전체 전기선속이 이 표면에 의하1 둘러싸인 전체 전하량과 같다
는 것이다. 이를 적용하여 점전하에 대한 전기선속을 계산할 수 있다. 가우스 법칙의 기초 개념을 사용하여 점전하에 대한 전
기선속을 계산하는 MAT나＼B 스크립트 파일을 작성해보자，
i 점전하에 대한전기선속 1

Keys사ord

I

점전하에 대한 전기선속

가우스 법칙 (Gauss's law）은 다음과 같다．

q1。1寸S S ' ds =q,.

(11.27)

여기서 똬of는 닫힌 표면 S에 대한 전체 전기선속（electric flux), 口毗는 닫힌 표면 S에 둘러싸인 전체
전하를 나타낸다．
구면좌표에서 점전하 口가 원점어］ 놓여 있을 때, 관측점 P에서 전기선속 밀도 I가는 모튼 가우스 평면
R의 수직 방향에 분포되기 때문에 Ds =DRaR로 나타낼 수 있다. 식 (11.27）을 이용하여 이를 다시 쓰
면 다음과 같다．

口］

-,]

, ] 人

n]

H

,\

과같다．

,
, .
.
,
,
r]
,,11
] 口.
2J入O
10
n 4R "나l. as== 口S（十ar J= a机iyaY / r 그거그J) ＼시1工i1ITl i그／Iti＝쑤；= L丁＝=
4

八lH

.,]

-

八］

r

, ]

(11.28)

1口］

1니l

1上仁：
｛시 소!' I소 크i= 덛＝- 1-'S =

口enc

Qenc=
fdb2=Dk/LIT
Q硫寸D5
fDs ' ds=
小＝Z)k
DRfrSR =
DRf , /IT, R2sinOdOd升DR4jrR2
47口r

吼，＝五Ds·小可（九니·（力比乞）

(11.29)

.y,z

口m 가우스 법칙의 기본 개념을 이용하면 전체 전7썬속은 앞쪽과 뒤쪽 평면을 통고陌는 전기선속만을 고려한 甲tot = 甲加,tt +1IJbOck
t =416mt이다．그러므로 전체
= 口가 된다. 여기서 앞쪽과 뒤쪽 표면의 면적은 주어진 점전하 口에 대해 대칭성이 있으므로 kji戶n。
, ,',＝으， - I.(1 [C］이다．
전기선속은甲
, ,' =7甲戶
, ,",' =1)가되어문저1에대한전71선속은甲尹
m/ - I -I ' j_.'II'II 111_ I_ II_ It_
H ' H '14 - ,tot
front
front - 2 .

CHAPTER ]]. 전자7짝

319

M-File I Gaus引그t.m

i 예工II 11- 2O !
L二二듀＝1- - I

점전하 2.0{C］이 좌표 (-2, 0, 0）에 놓여 있을 때 무한한 yz 평면을 통과하는 전체 전기선속을 구하라. 이때
직교좌표에서 앞쪽은 工의 양의 방향, 오른쪽은y의 양의 방향, 위쪽은 z의 양의 방향으로 각각 지정한다．

률苛

Ptm
l ==
23 45 -

57-

nl+

l

日＝2;
P미丑 0 七］;
a_e=11 0 01 ;
p니0斗er＝니00;; 止up口er=loO; 0
u_I ower=-I0먀4 乙up口er=100;

y_uteps＝印0；小 乙uteps=500; 0
dp=(y1up口er四lo口er)/y1stepu; 0

dz=(z山口per꼬니0叩er)／乙計e口3;

0 -

陶＝0; 0
Ejfor j=l: z_oteps;
for i=1 : y. .steps;
do=dy. dz; 0
p긔／Jo뿌er*0石내반(I 너 )*dy;
z=zJ叫er*0.5*dz*(j 너 hdZ ;
0=10 p zl ;
R=C-P;
mao4fl=norm(FO;
a..R=R/ma工R;
a占U r f =a0;
陶=P引，小ds.dot (a..eurf,a1R) /(4.pi.magR2) ; 0
end

22 23-

니 end
F岫內I,

e

n 杻 日 m 侮 怜 n 侶 四 게 기

910-

1
1
m
m
1
1
1
H
4
1

그림 거-35 전기선속 구하기 코딩 결과（Gau82다.m)

0 工 방향에 대한단위 벡터 a1x와무한한yz 평면에서 y의 낮은 경곗값과높은 경곗값을 지정하고, z의 낮
은 경곗값과높은 경곗값을 지정한다．
Oy축과z축 방향으로 분할한 값을 지정한다．
0 평면을나눌매우작은크기 力7, 比를지정한다．
0 점전하어］의한 전기선속을구하기 위해 초기 상태 Psi = 0을 지정한다．
0 각표면 면적의 요소 小＝力xd느와각표면 면적의 y 성분, z 성분을 지정한다．
0 식 (11.29）를입력한다．
0 점전하2.0[C］이 （그, 0. 0）에 놓여 있을때 무한한yz 평면을통과하는 전체 전기선속을구한다．
C口mmnnd Wind니그3뇨
>> GausoPt
Flue =
0.9820
그림 11-36 전기선속 구하71 실행 결과

口fl) MATLAB을 사용해서 얻은 결과와 이론적 계산으로 얻은 결과의 차이는 실제로 무한한 평면을 MATLAB 코딩에
적용하기가 쉽지 않71 때문에 무한한 평면 대신에 표면 S를 유한 평면으로 이용한다．

320

PART03. M月ILAB활용하기

L 표 SSON

08

커패시터와 커패시턴스

커패시터는 동일한 2개 0쌍의 도처까 서로 반대 극성 전하를 갖는 형태로 구성된다. 한쪽 도처때써 흐르는 전7썬속은 반드
시 다른 쪽 도처1 표면에 도달하는데，이 때문에 도체를 커패시터의 판이라고 부르7匠 한다． 2개의 판은 유전율 E으로 분리되
어 있다. 그리고 커패시턴스 C는 두 도체 시스템 중 한 전하의 크7뻬 대한 두 도체 사이의 전위차（p아enti졔 네iference) 비율
로 정의한다. 커패시터와 커패시턴스의 상호 관계를 계산하71 위한 간단한 MATLAB 스크립트 파일 작성법을 알아보자.
Keyi月ord

I

1 커패시턴스 1 input 1 네sp I 커패시터에 저장된 에너지 1

커패시턴스

도체판 사이의 거리가 d, 표면적이 S인 2개의 평행 도쩨판으로 구성된 평행판 커패시터 (capacitor) 의 커
패시턴스（capacitance）는 다음과같다．

C＝으＝S旦
乙2

(11.30)

(/

내부 도체의 반지름 口와 외부 도체의 반지름 b로 이루어진 원통 커패시티의 커패시턴스는 다음과 같다．

미기

=

으m

C

2,rgL

여기서 L은 커패시터의 길이를 나타낸다．
내부 도체 구의 반지름 口와 외부 도체 구의 반지름 b로 이루어진 구면 커패시티의 커패시턴스는 다음과
같다．
l

으m

C

47rs
1

n

H

47rsab
b- a

(11.32)

1

D

CHAPTE日 11, 전자:7國

321

M凹Fi地 ! Ca아ara.m

1 （川저1 11- 21 !

자유 공간0私d 거리 (/, 길이 L, 반지름 r인 평행한 두 도체의 커패시텬스를 구하는 식은 다음과 같다．
7rc0L
k I d- r\
i씨

Crr

1

H니卜

r

/

f

여기서 자유 공간의 유전율은 80 = 8.854 x 10-12 仕Im1이다．이때 임의의 d, L, r 값을 입력하여 커패시턴스
C를 출력하는 스크립트 파일 CapParam을 작성하라. 또한 d= 5[mm], r= 2[mi미，L= 2[i미를 입력하여
코딩한 스크립트 파일을 검사하라．

；而
지식

' input
加put명령어를이용하면문자열또는문장S를출력한후키보드로내용을입력할수있도록프롬프트가명령
창에 나타나며 입력받은 내용은R에 지정한다. input 명령어의 기본형태는다음과같다．

R = input('s')
· R: 입력받은 내용을 저장할 변수
· 낭：출력할 문자열 또는 문장

1disp
배열 또는 문자열의 내용을 명령 창에 보여주는 disp 명령어의 기본 형태는 다음과 같다．

disp('s')
· 낳：출력할 배열 또는 문자열

이때 변수명을 지정해도 변수명이 출력되지 않는다．

Ucapp겸立m 姓團

7-

6-

5-

4-

3-

2-

1-

횰可

二"：出：:：客퓨'烈，d in me：
아訂y, e
L = input (Enter a value for L i fl Meters: ') ;
r= input (Enter a value 伯r r iv meters: ') ;

듬lap客：",,':：뗀，:'三5(d出呼뇨)
disp(C)

그림 11-37 커패시턴스 구하3'I 코딩 결과（Ca口Paa.m)

(1 60 값을 지정한다．
0 임의의 세 값을 명령 창에 직접 입력하는 input 명령어를 이용한다．
0 문제에서 주어진 식을 이용하여 커패시턴스 값을 계산한다．
0 직접 입력한 세 값으로 계산된 커패시턴스의 결과를 명령 창에 출력하기 위해 disp 명령어를 이용한다．

322

PART 03. MATLAB활용하기

Command 汭4nd口町
>> CapPara
Enter a value for d in netero:0. [l巧
日ter a va山a 化r L In 1eters:2
Enter a value for r in .eters:O.1끄
The capacitance in farade Is:
l .3l2［뇨너 (}

그림 11-38 커패시텬스 구하71 실행 결과

I 커패시E刪 저장된 에너지
전기장 벡터 E와 전기선속 밀도 벡터 D를 이용하여 구한 에너지 밀도는 다음과 같다．

吼

그rD
. E加[ii
2JV

(11.33)

식 (11.33）에 D = 8E의 선형 관계를 적용하면 다음과 같은 새로운 두 식을 얻을 수 있다．

叫工，&万"加［J}

(11.34)

J]

v[

/,，쓰』

心｛

(11.35)

식 (11.34）에 万＝!，를대입하고식 (11.30）을이용하면다음과같다．
a

吟料）
「' 글cv2 [J]
口

;=

］八1_

_i,

-.a

il ,1, -

]

口］尸］

1- :i

그

.

나］ . , H]

== 二二言 나八押I-,힌 기파I,니口rn1 시Q只크 L끼니시言 나닥넨나．
C
-.1-

八．

.

］八．

.

口］

.

H,

,

＜긔 \11.jO) \J가 r

(11.36)

.

-.1；

少正

까

[J]

1 예제 11- 22 1

(11.37)

M-FiIe I CapEner.m

工l= 0과 毛 =d에 평행 도체가 놓여 있고 두 도체 사이의 유전율은 &0(2+ 2 x106工2)이다. 이따 도체의 표
면적은 S= 0.02[m勺이고 도체 사이의 거리는 d= 1.O[mmj이다. 양극판（pos川ye 이計이이 전하 Q = 4[nC]

의 값을 가질 때, 커패시터에 저장된 에너지 식을 이용하여 커패시턴스를 구하라．

CI-IA）在Ruj. 전자기학

323

m
H
m
e
1
1
e
e
n
H
小
小
e

1 2 3 4 5 6 7 8 9 m n 俚 仍 伍

}

i

小

풀이

CapEner.rn
e口引 Ion0=8. 咬汕e너 2;
댜＝45-9;
Sm.［묘；
d=1 e-3;
Ds=Q/S;
L欲e口s=2113;

dx=4屈如PS; 0
Le=0; 0

크fcr i=1:x. .steps
x==0. 5士dx+(卜1).dx;
epsi Ion=epsi lon0士（2+2士x.x女1 [l八6) ;

1

加＝S士dx;
dLe=(Ds' 冬的／(2*e四ilon) ; 自
Le=1He+d11e ;
Lend

15-

16 -

cr2/(2.Le) 0

그림 作39 커패시터에 저장된 에너지 식을 이용한 커패시턴스 구하기 코딩 결과（Ca口Ener.m)

0 工 방향의 간격을 지정한다．
0 저장된 에너지에 의한 커패시턴스를구하기 위해 초기 상태 we = 0을 지정한다．
0 식 (1L35）에서 오른쪽의 적분식이 없는상태로 만든수식을 입력한다．
0 커패시터에 저장된 에너지 식을 이용하여 커패시턴스를 구한다．
Command WftdCV

0=

>> CapEner

4. 묘 9鈿녀 lJ
그림 11-40 커패시터에 저장된 에너지 식을 이용한 커패시턴스 구하기 실행 결과

324

PART03. MAT녀B활용하71

色）

LESSON

09

전위

전위는 시간에 따라 변하지 않는 전기장에서 단위 전하의 전기적 위치 에너지이다, 3차원 그래프를 사용하여 전하 분포에 의
하1 생성된 전위를 살펴보자，
Keyword

I

I 전위 i 전위차 I meshc !

전위와 전위차

점전하q가놓여 있는 점으로부터 거리 R만큼 떨어진 위치에서의 전위（electric p아ential)는 다음과같다．

r=

q lvi

4w0R

(11.38)

'

점전하 q가놓여 있는점으로부터 거리 R1, R2만큼 떨어진 임의의 점 P1과尸2의 전위차는다음과같다．

乙1=VP2－느모，卄，－加］

(11.39)

M-FiIe 1 PotentiaLm

1 예제 11- 231
임의의 점에서 2개의 점전하 的과 q2에 의해 생성되는 전위는 다음과 같다．
TT_
r

1

1 (q1 q2\
I 丁I

小-

47rc0\ r1

r2)

刃7 평면상에서 점전하 q1 = 2 xl丁10은 (0.3. 0）에 놓여 있고, q2 = 中< 1丁10은 (-0.3, 0）에 놓여 있다．
-0.25 드 工 5 0.25와 -0.25 5 y 5 0.25에 놓여 있는 전위를 격자 표면과 등고선으로 동시에 나타내는 3차원

；而

그래프를 생성하라. 여기서 乙과 r2는 각각 임의의 점에서 점전하 q1. q2까지의 거리이다．

지식

'

meshc

3차원 격자무늬 그래프와등고선을함꼐 그리는meshc 명령어의 기본 형태는 다음과같다．

meshc(x,y,z)
. 凡 y: 축에 대한 정보가 저장된 배열
· Z: 배열 x, y의 값으로 이루어진 배열

CHAPTER ]]. 전자기학

325

加ten針al.m 弑 ! + j
epsi 1on0=8.85的너2;
qi = 2e나먀
q2 = 4e-10;
LX y 1 = 日eshgrid(-O. 25:O.15:O. 西) ; 0

;

q2.

/r2)

/rl

C

V.eshc
=,, (1/(.
pi名lonO) )*(ql
V) ;
xlabel (x ) ;
ylabel (y ') ;
zIabeI ( 2 ') ;

.

r2 = sqrt ( (x + O. 3) .八2 * y. A2) ;

4.

--

ii -

ri = sqrt ((e - O.3) . '2 * y. '2); e

y,

3 4 5 6 ? 8 9m

2-

(x,

룔可

그림 11-4] 전위 그래프 그리기 코딩 결과（n:)tent님.m)

0 meshgi-id 명령어를 이용하여 x와 y의 간격을 각각 0.025로 지정한다．
O거리n＝如_ 0.3)2 +y2, 乃＝如＋0.3)2 +y2을지정한다．
0 전위 V를 계산한다．
03차원 그래프를그리는meshe 명령어를 이용하여 전위 V를 그래프로 나타낸다．

그림 作42 전위 그래프 그리기 실행 결과

326

PART 03. M戶T녀B활용하기

LESSON

10

경겨I조건

서로 다른 2개의 매질이 경계면 사이에 존재할 때 정전71 공긴뻬서 각 영역에 대한 전기장과 전기선속 밀도의 관계를 구한다．
마찬가지로 정자71 공간에서 각 영역에 대한 자기장과 자기선속 밀도의 관계를 구한다. MATLAB 스크립트 파일을 작성하여
정전기장과 정자기장에 대한 경계 조건을 분석하는 방법을 알아보자．
Keyword

1 정전기장의 경계 조건 1 정자기장의 경계 조건 1

立 정전기장의 경계 조건
전기장 El 은 다음과 긷미 2개의 직교 성분으로 나뉜다．
El= E11 + El7i

(1L40)

경계면 사히에 위치한 2개땍 완전 유전체에서 전기장의 접선 성분은 경계면을 따라 연속이기 때문어］다음
과 같이 나타낼 수 있다．
E11 =E2r [V/rn]

(11.41)

Fl刃 = (E1 . aN)aN [V/rn]

(11.42)

전기장 E겨 수직 성분은 다음과 같다．

만일 경계면에 표면전하 밀도가 존재하면 전기선속 밀도의 수직 성분은 경계면을 따라 불연속이므로 다
음과 같다．
D1, -D2, =i , [C/rn2]
그러나 완전 유전체 사이의 경계면에는 표면전하 밀도가 존재하지 않으므로（Ps =0) 식 (11.41）은 다음
과 같이 나타낼 수 있다．
Dl刃 =1)2刃

(11.44)

CHAPTER ]] 전자7悸1

327

M-.阡佃 I BcElec.m

1 예제 11- 241

y< 0인 영역 1에 상대1 유전율 er1 =2.5인 완전 유전처까 있고, y> 0인 영역 2에 상대 유전율 8r2 =4.0인
완전 유전체가 있다1 영역 l에 전기장 El卜30a: +50카 니旽 [V姻가 있을 때 영역 2의 전기장 E2와
전기선속 밀도 D2를 구하라．

1 2 3 4 5 6 7 B 9 m H 泛 仍 m 惰

] Sc터ec.m 戈 i +
1

epsi 1on0=8. 咬i4e니 2;
工뼈0 1 0] ; <1
dinp(Enter E1. epsi len. .rl ,epsi lon_r2' );
1
小
1

E1=input ( 'El日ctric field intensity in region I: ' ); e
H

epsi lon_rt=input ( Flelatiye pernittivity in region 1 : ' ) ;
epni lon_r2=input ( llelatiye pereittivity in region 2: ' );
El...n=(dot (EI, ail) )*a..N; 0
EI_t=E1七L.n; 0
놔
小
e
巾

E2_t=E1_t; 0
E之n=E1. .n1epsi Ion_rl/ epni lnn_r2; 0
E2=E2. .t=E2. n;
1
n
1

disp(Electric field intensity in region 2 iS'); e
匯
H
m

disp(Electric fl나y density in region 2 is ') ;
D2黨e口si InnO士e口引 lon_泛奸꼬
H

그림 作43 정전기장어나1의 전기선속 밀도 구하기 코딩 결과（Bc日ec .m)

0 경계면y= 0의 수직 방향이 단위 벡터 방향이다．
0 벡터 目과상대 유전율Cr1, 8r2를 명령 창에 직접 입력하기 위해 血멕t 명령어를 이용한다．
0 식 (11.42）를이용하여 피, 을지정한다．
0 식 (11.40）을 이용하여 丑If를 지정한다．
0 식 (11.41）을 이용하여 瓦i를 지정한다．
0 식 (11.44）에 따라 디Em =勿E加이므로E2, 을지정한다．
0 계산된 벡터 E2와D2의 결과를 명령 창에 출력하기 위해I disp 명령어를이용한다．
Co！끼mond 甘／1nd（批1了
>> EcElec
Enter E1, epsi lgn_rl. epni lon_r2
티ect r比 field inten引ty in reginn 1 : [1m 印 40]
日lative permittivity in region I: 2.5
Relative permittivity in region 2: 4.0
Electric field intensity in region 2 is
E2=
＜刃 (ELf]

31 . 25013

40.［끄口U

티ect r比 flux den引ty in regino 2 is
02=
1 .0e-tf] +
七．1［砬

0. 1107

0. 1417

그림 11-44 정전기장에서의 전기선속 밀도 구하기 실행 결과

328

PART 03.卜肛玎녀B활용하71

I

정자기장의 경계 조건

자기선속밀도 B의 수직 성분은 경계면을 따라 연속이므로 다음조건을만족한다．
(11.45)

B1n = B2n [TI

만일 경계면에 자유 표면 전류가 존재하면 자기장의 접선 성분은 경계면을 따라 불연속이므로 다음 조건
을 만족한다．
an2 x (H1 -112) =J5 [A/rn]

(11.46)

여기서 카2는 경계면에서 영역 2의 수직 방향으로 향하는 단위 벡터이다．
만일 자기장 경계면에 자유 표면 전류山가 없으면 식 (11.46）은 다음과긷미 쓸수 있다．
H11 = H21

(11.47)

H17i =(H1 ' aN)aN [A/rn]

(11.48)

자기장 H1의 수직 성분은 다음과 같다．

자기장 H1은 다음과 긷히 2개의 직교 성분으로 나눌 수 있다．
H1 = H11 + H1刃

I 1뇌IxII ii- 9c I
L二：二：二二＝
：二J

(11.49)

M-File I BcMagn.m

반무한（semi-infinite) 공간상의 경계면 2工中5y >0인 영역 l에서 상대 투자율（r이ative permeal川ty)
/／기 = 3인 매질과 2工 -5y< 0인 영역 2에서 상대 투자율／42 = 4인 매질이 있다（경계면에는 표면 전류가 존
재하지 않는다）.
두 영역 중 한 곳의 자기장（H] 혹은 H2)만을 알고 있을 때 나머지 영역의 자기장을 계신后卜는 MATLAB 스크
립트 파일 BcMagn.m을 작성하라. 또한 자기장 H1 = 30a[A/m]에 대해 자기장 H2와 자기선속 밀도 B2의
결과를 확인하라．

CHAPTER ]]. 전자기학

329

풀이

三 ! 8CM因n.m
mu04奸n너十7;
12-

aJl=[2 -5 0h/sqrt (22. (-5)八2) ;

3-

dinp(Enter vectors ) ;

4-

mu_rl=input ( ’닥elatiye permeabi l ity in region I : ' );
1 u_r2input (Relat ice permeabi l ity in region 2: ' );
a...12=input (' Unit vector from region 1 to region 2: ') ;

5678-

다Bglon=lnput (' Region 쁘here field is kno斗n (1 or 2) : ' );
比k=input (Knoen magnetic field intensity vectnr: ' );

910 -

if 陀미nn늬 <I
口uerk=riu_rl ;, .iu_ru=mu_r2; , k=a...12;

11 -

이55

12 -

iu1rk=.ur2; , ma_ru=mu_rl ;. k=-aJ2;

1314 -

end
Ik...n=dot (lLk,k).k; 0
Ikt＝比k卄.n;. Hut＝出1t; e
叱0=mu0.m나내m』血5=8山； 0

1516 17 18 -

Hu. .n＝
日..n/(muO..u_ra) ;
比U쉬J_t，汁LJ; 0
巳u=muO.mu_ru，比U; 0
미splay(Unkno밖nmagnet 沇 Ii이d inten引ty in the other region 泊： '
F倭Hu

IS 21} 尸
21

-

22四H

display(Unkn叫n magnetic flee density in the other region is: ' );
日2多．B-JJ

그림 11-45 자기장과 자7Rd속 밀도 구하기 코딩 결과（BcMagn.m)

0 입력받은 영역어］따라 변수를 지정한다．
0 식 (11.48）을이용하여 H1, 을지정한다．
0 식 (11.49）와식 (11.47）을이용하여 Hit와珏r를지정한다．
0 B1 =p0 "u51 "H1。
과식 (11.45）를이용하여 B1과B2。
을지정한다．
02개의 직교 성분을 더하여 자기장을 구한다．
0 구한자기장H2를 이용하여 자기선속 밀도B2를구한다．
C: :'ar:d 啣04（꽈V
)' 8cMayn
Enter vectors
Relative per.eabi l ity in region 1: 3
Relative permeabi l ity in region 2: 4
Unit Vector fro. region I to region 2: 0卜
Region .here field is kno.n (1 or 2) : 1
lOnomn magnetic field Intensity eector: Im 0 01
tkkno.n magnetic field intenoity in the other region In:
1끄 =
28. 9555

2. 5952

0

Unknown magnetic flue density In the other region is:
82 =
I .lh-f_03 *
0. 14弱

0．미印

[}

그림 11-46 자기장과 자기선속 밀도 구하기 실행 걸과

/／日과月r2를 차례로 입력한 후 영역 i에서 영역 2로의 단위 벡터를 입력한다. 자기장값을 알고 있는 영역을
입력하고 그 영역의 자기장값을 입력하면 나머지 영역의 자기장값과자기선속 밀도가 명령 창에 나타난다．

330

PART 03. MATLAB활용하71

LESSON

11

인덕터와 인덕턴스

도선의 코일로 구성된 인덕터는 자기장의 에너지를 저장할 수 있는 소자이며, 인덕터가 가지고 있는 성질을 인덕턴스라고 한
다. 인덕턴스는 L로 나타내고 단위는 헨리（H）이다. 인덕터 전류는 인덕터에 흐르는 전압을 적분하여 얻을 수 있다. 인덕터와
인덕턴스의 상호 관계를 계산하71 위한 간단한 MATLAB 스크립트 파일 작성법을 알아보자．
Keyword

I

I 인덕턴스 1

인덕턴스

인덕터 (inductor）의 성질을 나타내는 인덕턴스（inductance）는 다음 식으로 정의한다．
乙＝으
I

(11.50)

도선을N번 감은 코일의 자기선속 m는 다음과 같다．
令 = N中S
여기서（과는한 번 감긴 도선어］의해 둘러싸인 표면을통과하는 선속이다．

M-FiIe 1 IndSe卄.m

1 예제 11- 261

도선에 코일을 N번 감은 환상체(tor이d톄 frame）가 자유 공간에 놓여 있을 ［대1 자체 인덕턴스 L은 다음과 같
다. 口와 b는 각각 환상체 안쪽과 바깥쪽 반지름, h는 높이이며, 자유 공간의 투자율은 ／幻 = 4冗 xlO口田Im]
이다．
L = p0N2h
22r

hlb
a

임의의 (z. b, 力. 入／ 값을 입력하여 인덕턴스 L을 출력하는 스크립트 파일 IndSe什.m을 작성하라. 또한
口= 3 [mni], b= 6[mm], 方 = 1.5[mm], N= 400［회］을 입력하여 코딩한 스크립트 파일을 검사하라．

CHAP在R ]] . 전자기학

331

풀이

「 1 !ndS叫tm i{

+

1-

mu0=4朴n시于7;

2345-

a = input (Enter a value for inner radius 0
b = iripst (Enter a value for outer radius
h = input (Enter a value fur height of tu
N = input ( 'Enter a value fur number of tu

8-

disp(L)

S7: 능“，
，二빱，
"nductanc：
껍：:(,",/,',):e,e

그림 11-47 인덕턴스 구하기 코딩 결과(lMSe忙m)

0 임의의 口, b, h, N값을 명령 창어］직접 입력하는in叩t 명령어를 이용한다．
0 식 (11.50）을 이용하여 인덕턴스를구한다．
0 입력한 값으로 계산된 결과를 명령 창에 출력하기 위해 disp 명령어를 이용한다．
::n丁m.r: Jnn
>> IndSeif
Enter a value for inner radius in meters: 0. 끄3
Enter a value for outer radius in meters: 0.11
Enter a value for height of toroidal in meters: 0. 刃15
Enter a value for number of turns: 41)3
The inductance is henrys in:
3. 王？lie-I巧
그림 11-48 인덕턴스 구하기 실행 결과

332

PA딕T 03. MATLAB활용하기

L 드 SSON

12

a匿라스 방정식

선형 유전처뻬 2차 편口분방정식 형태의 체적 전하7卜 주어天는 경우． 전위는 반드시 푸아송 방정식을 따라야 한다．반면에 라
플라스 방정식은 체적 전하가 없는 영역에서 전위를 구할 때 꼭 필요한 방정식으로 전자7陣t에서 매우 중요한 부분을 차지한
다. MATLAB 스크립트 파일로 작성된 라플라스 방정식을 사용하여 커패시턴스를 계산하는 과정을 알아보자．
Keys사ord

I

1 라플라스 방정식 1 char I ds이ye i pretty I grad I

원통좌표겨唾 사용하는 라푿라스 방정식

푸아송 방정식은 다음과 긷미 정의된다．

v2v = pv

(11.52)

여기서 寸는 라플라시안 연산자라하고, p, 는 체척 전하를 나타낸다．
식 (11.52）어］서p, =0인경우라플라스방정식은다음과같이 정의된다．
v2v= o

(11.53)

원통좌표계에 대한 라플라스 방정식은 다음과 같다．

，口2.,
\/

I 에xii 11_ ')7 I
［二二二二二＝::J

1 a / aV\

i a2v

a2v

/) op \

/）乙 a少

az乙

V == 111:1

八

1 /J 二1 1 十 1 O1H1O1 가＝ 11丁 = (J

op /

(11.54)

M＋加 I grad.m, La히ace.m

내부 원통 도처1 반지름이 口이고 외부 원통 도처1 반지름이 b인 동축 케이블이 있다, 두 원통 사이는 유전율이
C인 선형 유전체로 채워져 있고, 내부 원통 도체에는 전압 V0가, 외부 원통 도체에는 전압 0이 인가되었다．
두 원통의 길이가 무한히 길다고 가정할 때, 라플라스 방정식을 이용하여 口 5 p 5b 영역에서의 전위와 전
기장을 구하고, 원통 커패시터의 길이가 /(1 >> b）인 경우에 대한 커패시턴스를 구하라. 모든 결과는 pretty 명
령어를 사용하여 출력하라．

CHAPTER 11. 전자기학

333

；而
지식

' char
음수가아닌 정수의 배열을문자배열로 나타내는char 명령어의 기본형태는다음과긷다．

S = char(x)

口 dsolve
상미분방정식을 계산하는 ds아ye 함수의 기본 형태는 다음과 같다．

ds이ve('equation났倒）
· 'equation七 상미분방정식의 심벌릭 식
, y(o): 초깃값

dsolve 함수를 사용할 때는 solve 함수와마찬가지로 syms 명령어로 미리 변수를 지정할 필요가 없다．
口 pretty
심벌릭 수식을 조판형태로 출력하는pretty 명령어의 기본 형태는다음과긷다．

pretty(E)
· E: 심벌릭 수식

1grad
원통좌표계에서 전압을 이용하여 전기장을구하는사용자정의함수grad의 기본 형태는다음과같다．

grad(F, cyl, var)
· F: 전위차를 나타낸 벡터
·cyl 원통좌표계로 변환하기 위한 벡터 [rho 口hi z]

·

岵

빠：벡터 ［朴，

屯］

단, 사용중인 현재 폴더어］ 'grad.m'이 있을 때만 이 함수를사용할수 있다．

푿이

J

어adm

+

I(Fcy；
斗；;：二：
(1);
var)
二－카：":'二In,：0ng
3-

f 旺 = ditt (F,cyl (2) ).yar (2) ;

45-

1 L3 = dItt (t. cyI (a) ).yar (3) ;
LI = L11 52 3J;

그림 11-49 grd.m

334

PART 03. M月TLAB 활용하기

町

1 m的ce.m X 旺盈
syms rho phi z V a b I V_O epsi lon DV D2V 1
equat Ion = rho士0낌 + ［싸；
equation = char (equat ion) ;
disp( 'Potential difference ')
V = dsolye(equation, V(a):V_0'. 'V (b):O', rho) ; 0

3 4 5 6 7 8 9 m n 促 日 m 佰 佰 口

1日
2+
-

V = si.pl ily(V) ;
pretty(Y)
cyl = Irho phi z] ;
ear = 11 1/rho II;
dlop( '티吼tr比 lie너 intensity' )
E = 田rad(Y.cyl, var) ; 0

=
-

pretty(E) ;

rho. s = epsi lon.subo(E(lLrho,a); e

U = rho...s.(小미＋a니）;
d沽口（'Capacitance bet斗een t斗0 cyl indr比ol c카）acitors ')
C = 口／V10;

-

=
1

pretty (C) 0

그림 小50 라플라스 방정식을 이용하여 전위, 전기장. 커패시턴스 구하기 코딩 결과(La아欲冶.m)

0 심벌릭 툴박스를 사용하기 위해 syms 명령어를 이용하여 필요한 변수를 지정한다．
1 1,,

U

八1 上 벼1八1 1,J＝』］尸 尸t1] n1n1 八 八 m H a

y亡 z놔 (p 自｛비

a

,, ,1 / . . 戶, \ ,

of

OV\

n . , 尸,m.

번애느二 딛다시시 送＝=＝도 = = H.; = U, 스J l,11.)'1)亡 ：니 P= e 1 = U미 뇐L十．
c,z
c甲
d/) \
d/)/

ds아ye 함수어써 사용하는 1차와2차를 나타내는 미분 심벌릭 DV와D2V를 지정한다．
八 .1 n =-1H, 八,=, ,
. 山 . , /, -, . . H, . -,. =m ．小寸，
av
1 a"
av ,. .... . .
O사용자정，의，함수grad를이，용方臼. 전，기．장 E = -VV = a, 二：-+a小二- +a, 二：m를계．산한다．
"pa中 , aZ
尸 0p
0 subs 함수를 이용하여 계산된 전기장에서 변수p를口로 대치한다．
0 구한 커패시터 값을pretty 명령어를 이용하여 조판 형태로 출력한다．
二nd \'/ind口／/
>> Laplace
Potential difference
V_U (Iog(b) - Iog(rho) )
Iog(a) - fog(b)
11 /

Electric field intensity
V山
/
1
, 0, 0
$
rho (log(a) - log(b) )

Capacitance between teo cyl indrical capacitors
2 epoi lon I p1
log(a) - fog(b)
그림 ]1-51 라퓰라스 방정식을 이용하0켜 전위． 전기장，커패시턴스 구하:7 ' 실행 결과

CHAP作All . 전자기학

335

LESSON

13

비오1사바르 법칙

H隍m사바르 법칙은 닫힌 경로상에 흐르는 전류에 의해 생성되는 자7썬속 밀도를 결정하는 식으로 벡터 자71 전위에 회전을
적용하여 얻는다. 비오－人빠르 법칙을 기초로 작성한 MATLAB 스크립트 파일을 사용하여 무한 선전류와 유한 선전류에서 자
기선속 밀도률 구하는 과정을 알아보자．
Key卯ord

I

I 무한 거리에 존재하는 선전류 i 비오4사바르 법칙 I mnt I 유한선전류에서의 자기선속 밀도 1

무한 거리에 존재하는 선전류

선전류가／일 띠1 비오사바르 법칙 (Bi야 Savart's law）은 다음과 같다．

B考址dZ‘二
, "' 口］

(1L55)

여기서 抑은 원천점 (source point)에서 장점 (field point) 방향인 단위 벡터이다．

『］

':

,(

d8寸｛ " f,R " '
4z

(11.56)

T]

dB[

)［

B=

j,

식 (11.55）는 편의어］의해 다음과 같이 두 과정으로 분리한다．

1 여以｛I 11- p요 1
L二二二＝m二二J

(11.57)
M-科！em E引otlnfline.m

비오m사바르 법칙을 이용하여 무한 z축상에 놓여 있는 선전류／로부터 자기선속 밀도 B를 구하고, 그 결과

지식

'

jilt

；而

를 pretty 명령어를 사용하여 나타내라．

주어진수식을적분하는m t함수의 기본형태는다음과같다．

int(f,var,a,b)
· f: 피적분함수
·var: 적분 변수
· 瓦 b: 적분의 하한값과 상한값

336

PART 03. MATLAB활용하기

풀이

U B幻tin拍r比JT 鷺凝曳
1 2-

SYmS S S S 乙prime moO I real
a_u = 1001] ;

345_
67 69-

r= IxyOl;
r...prirne = 10 0 乙prim日］;
P = r-r_마I me;
norm_ 극 = snrt (A(lY2*R(2)n2+A(3)八2) ;
工R = P/norm_A;
dO = (muo* l )/（小川蛇roms( a_u，乙A) /norm_R'2; <1
disp( 'l4agnetic Hun density 6' )

IC 11 -

B = int (dB,z. .pr油e,니nf, lnf); e
pretty (S) 0

그림 1］巧2 비오m사바르 법칙을 이용하여 자기선속 밀도 구하71 코딩 결과佃에뻬ne.m)

0 식 (fl.57）을 이용하여 dB를 지정한다．
0 식 (11.56）을 이용하여 자기선속 밀도, B를 구한다. 이때 mnt 함수를 이용하여 적분하며, 인자 dB는 피
적분함수, 乙pnn妃은 적분 변수, -Inf와Inf는 무한한z축에 놓여 있는 전류어］대한 적분의 하한값과상
한값을 나타낸다．
0 pretty 명령어를 이용하여 자기선속 밀도B를 조판형태로 나타낸다．
Command Win小二w

@1

.

2小

;

1

2小

>> Biotinfl ine
Magnetic flux density B
I muDs
/
I muOy
1

咐
.

2

0 I
I
/

그림 11-53 비사바르 법칙을 이용하여 자기선속 밀도 구하7] 실행 결과

I

유한 선전류어快1의 자기선속 밀도

원천 성분 比쐬］서 장점 P까지의 거리 벡터는 다음과 같다．
R = 하p - az'
(/Z'x R = a:z' x (app - az') = apdz'
식 (11.56）과식 (11.57）을 이용하여 구한자기선속 밀도는다음과같다．

B= a中

쀼尤（: +
!2pdzp2)' 312=a:,,芦1+ j;

(11.58)

CHAPTER 11. 전자기학

337

M-F加 1 BiotFline.m, CarlcylM.m

1 예저I 11- 291

비오4사바르 법칙을 이용하여 크，드z 드［에 놓여 있는 선전류／에 의해匈(z = 0) 평면에서 생성되는 자기선
속 밀도 B를 pretty 명령어를 이용하여 나타내라. 다시 말하나y 평면을 이등분하는 선으로부터 p만큼 떨어진
점에서의 자기선속 밀도 B를 구하라．
弓 } Bh共Fiji祀rn
1

syms S S 乙口rise L i muD
a_z = 10011;
r = lx y 01;
r니）rim日 = (0 0 乙prim日1 ;
U

풀이

n
r
느

m

n
J

H

4

1

二
니

U

A = r-r_마me;
normJl = sqrt (k( I )2. R(2) 2.R(3) 2) ;
a._Fl = R/normii;
dB = (mu마1m巾네札ross（心m小）/nurm_斤2; <1
disp(Maynetic fl ux density B in Cartesian system' )

n
n

느

口
1

m

8

1

口
나

1

0
1

B = int (dB.z. prime,닉－,L); e
pretty(B) 0
4

1
1

1

2
1
1

4

disp( 'Magnetic flux density B in cyl idrical system ')

口
U
1

尸

cy匕化rm = 由rlcylM(B); O
pretty(cyl_ form) 0

4
1
1

1

그림 11-54 비오사바르 법칙을 이용하여 자7R크속 밀도 구하기 코딩 결과（Bki태ne.m)

0 식 (11.57）을 이용하여 dB를 지정한다．
0 mlt 함수를 이용하여 적분 변수乙prime에 대한피적분함수dB를 하한값 L과상한값L로 적분한다．
0 pretty 명령어를 이용하여 직교좌표로 표현된 자기선속 밀도 B를 조판 형태로 나타낸다．
0 CarTcy小4 함수를 이용하여 직교좌표를 원통좌표로 변환한다．
0 pretty 명령어를 이용하여 원통좌표로 변환한자기선속 밀도 B를 조판 형태로 나타낸다．

1甘

>> 미utFl bne
Magnetic flux density B In Cartesian system
/
I Lau0y
I

I Lmuoic

,

2
2p1 (e

2

2
2
2
* y ) sqrt (L + x + y )

』

2
2pi Cx

2
2
2
2
+ y ) sqrt (L .5 + y )

0 l
I
/

甘

Magnetic flux density B in cyl idrical system
/
I Lmu0
1
l 0.
. 0I
I
2
2
I
2 rho pi sqrt (L * rho )
/
그림 11-55 비

사바르 법칙을 이용하여 자기선속 밀도 구하71 실행 결과

El1} 명령 칭K게 力BiotE괘ne를 입력하면 경우에 따라［그림］1-55］의 결과가 나오지 않고 오류 메시지가 나올 수도 있다．
이럴 때는 다소 불편하더라도 현재 사용 중인 MATLAB올 로그아웃하고 다시 시작하여 ))Bk片Fline룔 입력하면 올
바른 결과를 얻을 수 있다．

338

PART 03. jt:凡AB활용하기

LESSON

14

암페어 법칙

암페어 법칙은 가우스 법칙과 비숫하게 전류 분포가 대칭일 때 자기장 H를 결정하는 데 쉽게 적용할 수 있다
. 암페어 법칙은
비오中사바르 법칙으로부터 유도할 수 있다. 암페어 법칙의 기초 개념을 사용하여 동축 전송선을 해석해보자．
Key싸ord

I

t 암페어 법칙 1 암페리안 경로 1

암페어 법칙

닫힌 경로 주위에 놓여 있는 자기장 H의 접선 성분에 대한 선적분은 이 경로어］둘러싸인 전체 전류／와
같고, 이를식으로나타내면다음과같다．
(11.59)

／毗

多H·

de=

가우시안 표면（GaL好sian surface）과 유사한 개념으로 암페어 법칙 (Ampere's law）을 적용하는 경로
를 암페리안 경로（Amperian path）라고 한다．
식 (11.59）에서 암페리안 경로로 동심원을 선택하면 다음과 같이 자기장을 정의할수 있다．
--

I

11 = -aA-

八
乙71下)

(11.60)

Yr

이 경로는 전체 전류／를 둘러싸고 있기 때문어］암페어 법칙을 적용하여 구한 전류는 다음과 같다．

乙，. =／甘伊中 ' pd蜘＝川p伊恥叩

1 예저1 11-301

(11.

dZ =

27rpH

fH·

식 (11.59）와식 (11.61）을 이용하면 자기장을다음과긷히 정의할수 있다．

62)

M-File i Ampere.m

반지름이 각각 口, b. c（口＜b< c）이고 축이 같은 3개의 원통이 z축을 따라 놓인 동축 전송선이 있다. p<a,

口＜p<b. b<p<c, p>c 각 영역에 대한 자기장을 구하고 pretty 명령어를 이용하여 나타내박．

CHAPTER 11. 전자기학

339

니 Amp미毛m
1
1

1

풀이

m

n
G n
J

spas rho phi I H a b C

J_a = l/(pi*a'2); <1

U

4
m
1

二
니 h
b

J_bc = -l/ (pl=(c'2七'2)); 0
disp( Magnetic field intensity in each regions' )

L日seth_I oop = 小口나rhn; e

H

nrr
4

8
H

Q
나
0
中

1
1
e

n
C
4
m

口
나 4

1

戶hU
1

r
n
b n
m

8
1

H_c ! 0 e

1 l 1 1 1 1 1 11

叫

dinp( (1) rho < a)
匕enc_a = 上十如i.rh／기 ;
比a = 匕e吃a九ength_l asp; 0
pretty (H_a)
disp( (2) a ( rho < b' )
H_nb = I/Length_ loop; 0
pretty(H口ab)
dlsp( (3) b < rho < c ')
匕eoc_bc = 1 1 J_t比K이1rho2니키比八2) ;
H上C = 匕en汕c/L日ngth_ loo口； 0
pretty(H_bc)
disp( (4) rho , ci

그림 作56 암퍼때 법칙을 이용하여 자기장 구하71 코딩 결과（Ampe他m)

I

/

1J口

凡口

0 P < 口 영역에서 도처1 내부에 둘러싸인 전쳬 전류는 +／이므로 전류 밀도 J口 = (, =；万들 지성한다·
,

,

-

，卜三＝ . , / ，,．를 지정한다．
0 h< n< .영역에서전류밀도J."
中 V r ' U ' " ' 니" 나
口,C
SAC
,r(c2- b2)
.
0 동심원의 둘러］ 길이는2irp이다．
Op＜口 영역에서의자기장값을지정한다．
0 口 <p< b 영역에서의 자기장값을 지정한다．
0 b<p< c 영역에서의 자기장값을 지정한다．
0 p> c 영역에서의 자기장값을지정한다．
回
>> A叫：'era
Magnetic h ield intensity in each regions
(1) rho < a
I rho
2
2 a pi
(2) a < rho < b
i
2 rho r나
(3) b < rho < c
2
2
1 （口i b 1 pi rho )
1 +
2
2
pi (b 1 c )
rho p1 2
(4) rho > C
｝七C =
U
그림 11呻57 암페어 법칙을 이용하여 자기장 구하기 실행 결과

340

PART 03. M戶TAB활용하기

H

.

.

=

.

.

LESSON

15

맥스웰 방정식

맥스웰 방정식은 전자기장에 대한 전하의 작용｛전하가 전자기장을 어떻게 발생시키는지）을 나타낸다. 전자기학의 기반이 되는
맥스웰1 방정식은 모든 거시적 상황에 적용되는데 ，시간에 따라 변화하는 경우에도 적용할 수 았다．심벌릭 툴박스를 사용하여
맥스웰 방정식을 이용한 전기장과 자기장의 변환 과정을 살펴보자．
Keyi사ord

I

1 맥스웰 방정식 1

맥스꾀1 방정식

맥스웰 방정식 (Maxwell's equations）은 시간에 따라 변화하는 장에서 성립하는 패러데이 법칙, 암페어
법칙, 전기장과자기장어］대한가우스 법칙 등4캐의 식으로구성되며, 다음과긷히 정의한다．
V , E =－크프
카

（패러데이 법칙）

(11.63키

V》H= J＋쁘
at

（암페어 법칙）

(11.63b)

V ' D = ／兀

（전기장어］대한 가우스 법칙）

(11.63이

V ·B= O

（자기장어］대한 가우스 법칙）

(11.63d)

여기서 夙는 자유 전하의 체적 밀도, J는 자유 전류의 밀도를 나타낸다．
맥스웰 방정식은 적분형으로도 표현할수 있다. 2개의 회전 방정식인 식 (11.63a）와 식 (11.63b）를 표
면 S어］ 대해 적분하고 入두긔入 정리 (Stokes' theorem)를 적용하여 식 (11.64a）와식 (1L64b）를유
도할 수 있다. 또한 2개의 발산 방정식인 식 (11.63c）와 식 (11.63d）를 공간 V어］ 대해 적분하고 발산
정리 (d如ergence theorem)를 적용하면 식 (11.64c）와 식 (11.64d）를 유도할 수 있다. 그 결과는 다
음과 같다．

(11.64b)

f尹 ' ds =f p油

(11.64이

f,

Js B

O

(11.

五H· dZU;(1*罕）·db.
ds=

(11.64키

'

五E· dI =｛罕·必

CHAPTER ]]. 전자기학

64d)

341

식 (11.63）의 모튼 스칼라장과 벡터장을복소 위상（coo叩lex phasor）으로 다시 나타낸 시간조화전자
기장어］대한 맥스웰 방정식은 다음과 같다．
VxE= -jwpll

(11.65a)

VxH= J+ jwE

(11.65b)

V·E= p, /8

(11.65c)

V·H= O

(11.65d)

식 (11.65）는 ／兀 = J= o인 원천이 없는 단순 매질 속에서 다음 맥스웰 방정식을 만족한다．
VxE= -jcopH

(11.66a)

VxH= jogE

(11.66b)

V·E= O

(11.66c)

V·H= O

(11.66d)

M-File i Maxwell.m

［예제 11- 311

위상형（phaso사orm)으로 주어진 전기장 E(y）에 대한 위상형의 자기장과 시간형의 자기장을 구하라．
E。
ej ' '
E(y) = a。

系i

MaxW斟Ln1 無 +
1myms y k t omega eta EO real
dlmp(Electric field intensity in yhasor domain )
已帥amor = EO螂口（季k싸川0 0 II ; <
pretty(E_phamor) ;
工y = (0 I 01 ;
dlmpYflaonet 比 fi led intensity in phanor domain')
ll_phasor = (1/eta)*cromm(a..y다hasor) ; 0
p ret t y ( H_phamor ) ;
dimp( Magnet 比 field intensity in time domain)
比t 1mm = re이（比曲more如如mama砒）); 0
比tlme = 引mpl lly(fLtlme) ;
pretty (H_ tlme) ; 0
그림 11-58 맥스웰 방정식을 이용하여 자기장 구하71 코딩 결과佃aXV咬孔m)

0 전기장 E(y）를 지정한다．
0전기장과자기장의쌍대원리H(y）그a, x [a, 万.可」
初］를이용하면주어진위상형의전기징혀］서위
11
상형의 자기장을 구할수 있다．
0 위상형의 자기장에 少를곱한후 실수부분만을 선택하면 시간형의 자기장을구할수 있다．
0 pretty 명령어를 이용하여 시간형에 대한 자기장 결과를 조판 형태로 나타낸다．

342

PART 03. MA11AB활용하71

Command Wind口
>> 4axwel I
타ect r比 field jot日n引 ty in phasor domain
(0, 0, EU exp(-k p 11) )
Nasnetjc fi led Intensity In phasor doaain
/ EU 日xp(-l< y ii)
卞
I -甘

eta

1111m. 0, 0 I
/

Magnetjc field Inten引ty In t 油e 如maj n
/ 印 cos(o.ega t = k y)
甘
I
, 0. 0 I
甘
日to
/
그림 11-59 맥스웰 방정식을 이용하여 자기장 구하기 실행 결과

CHAPTER ]]. 전자기학

343

LESSON

16

균일 평면파

전기장에 대한 맥스웰 방정식의 특정한 해법은 균일 평면파가 전파하는 방향에 수직인 무한 평면에서 같은 방향 ，같은 크기，
같은 상을 갖는다고 가정힌匹f, 균일이란 말은 등위상면에서는 전자기파의 진폭이 위치에 상관없이 균일하다는 의미이다. 평면파
를 이용하기 위한 MATLAB의 스크립트 파일을 작성하여 균일 평면파를 특정 짓는 다양한 매개변수를 찾는 과정을 살펴보자．
Keyword

I

i 원천이 없는 매질0私倒 균일 평면파 1 헬름홀츠 방정식 i （幻uble

원천이 없는 매질에서의 균일 평면파

균일 평면파（uniform plane wave）는 원천이 없는무손실(lossless) 매질과 원천이 있는 손실(lossy)
매질로구분하여 해석할수 있다. 이 책에서는무손실 매질인 경우를 다룬다．
원천이 없는 매질에서 이용하는 헬름흘츠 방정식 (Helmholtz's equation）은 다음과 같다．
투2E + k2E = 0

(11.67)

여기서 파수（wavenumber) k는 다음과 같다．
k = co-.j而 {radlm]

(11.68)

고유 임피던스（II血insic impedance) ,i는 다음과 같다．

I百rr

CO/i
1
q 1 mm,H 1 \/H LbdJ
丸
Y 6
-i

(11.69)

344

PART03. M/玎녀B활용하71

尸

＝

k0c

－

그

k0

0=

(.

원천이 없는 무손실 매질인 경우어］각주파수는 다음과 같다．

7이

(11.

s]

[m/

V，

亡，

위상속도（phase velocity) v1,는다음과같다．

자유 공간의 고유 임피던스는 다음과 갇으며, 자유 공간의 위상속도는 빛의 속도와같다．

(11.72)

Q]

;: 377[

.I브으

q, =

V 80
8n

M-File 1 Planewave.m

1 여以｛I 11- 32I
원천0I 없는 시간 조화 평면파의 위상형 전기장 月는 다음과 같다．

=0인

[A/

점에서 자기장의 크71가

[V/

e " 3 '

jay)

(a,

+

4승中，

때：

0일

시간t=

=

3

.2兀

E

]

rn

］인 경우 전기장의 시간영역에 대한식을 구

rn

하고, 매질의 고유 임피던스 '1, 상대 유전율 8:, 상대 투자율 外을 각각 구하라. 단, 자유 공간어써 유전율은

이다·

V

（=

,[m8］

=

빛의속도는

;

E0= 8.854 x i0l2 [F/rn
］
이고 투天율은 尸。=47rxl07[}TJm］이다. 또한 유전율과 투工율의 관계를 이용한

；而

' double

지식

주어진수를소수점을포함하는배정밀도값으로변환하는double함수의 기본형태는다음과같다．

（幻ub旭（미

풀이

미areewave.rn 莪r+ 1
SYRIa Z t k 口cean real
ma0 = 小미＋1 e-7;
日ps l 山n0 = 巳054니e너2;
3
4c = sqrt (l/ (muO*epsi lonO) );
5etsO = oqrt (muO/epsi lonO) ;
6a_k H00 ii;
7die口（日ect r比 tie내 intensity in tine 加Cain )
1 n
／느

B9-

化 四四 끼겊 拓

1011 1213 14 小
IS 161? 尸
-

已phas口r = 小mop（和k.z).[l 蜚 01; 0
巳time = real (E_phaoor=gop (重.omegaet)); 0

E_tlme=,simpl ily (E口time)
E_val = oubo(E. .time, {k .oeega』z, t},{2*pl/3, 2.pi니0'B,O, O} ); e

巳mao = norm(E_ 'al) ; O
比mao = 11(4마이 ) ;
disp( lntrinsic impedance )
eta !, double(E_mag/H_mag) 0
mur0日psl lonr : eta/etaO; 0
phase_v = omega/k;
murMe口ol lsnr = (c/phaoe_v)A2;
rnurMe口si lonr = subo (murMapoi leer』 (k,omega｝』｛2api/3』2*pi*山'8} ); 0
disp(Relnt} veperseabi l ity )
mu_r 르. double(nqrt (murHepsi 山nr.murDepai lonr) ) O
die口（多미at ice 口eraintiv나느r )
epsl lon_r 多 double (murMepsi 比nr/mu_r) @

그림 11-60 균일 평면파의 톡성 구하기 코딩 결과（Ranewave.m)

CHAPTER 11. 전자기학

345

0 위상형 전기장에 e加'를 곱한후 실수 부분만을 선택하는 데 사용하는 연관 변수를 심벌릭 변수로 미리 지
정한다．
0 위상형 전기장을 지정한다．
0 위상형 전기장어써 실수 부분만을 선택한다．
0 위상형 전기장의 실수 부분에 사용하는 변숫값을 대치하여 지정한다．
0 위상형 전기장의 크기를 구한다．
0 面uble 함수를 이용하여 고유 임피던스 叩를 배정밀도값으로 변환한다．
0 뜨 =！를나타낸다．
8r 710
0 subs 함수를 이용하여 파수 k와각주퍄수 CL)에 싱숫값을 대입한다．
0 상때1 투자율／/, 을 지정한다．
四 상대 유전율따을 지정한다．
Cole그mand Win出｝1가
>> F기one뽀ave
티 act r 比 ii引d inten引to Ire time domain
已time =
[3中005( omega卄 - k.z) , 臼＋sln(ome明吐 七 k.z), 0]
intrire引C 油口edance
eta =
376 . 99ii
Relat iv日 p日reeabi I Ito
mu. r =
0, 999'?
Relative permittivity
epei lon_r =
0 9990
그림 거니5i 균일 평면파의 특성 구하기 실행 결과

346

PA日T03. M月TLAB활용하기

1__LJ

L iL 口
I f_I I I j r

11' m斗『

1 T I I I li_ _i i

!

! i j

! '-II-口 LI I
i 1
[ I
1
I I i i I ' I
, I I I , I i I I 1
1 P i I I Fl] . nr I 口TJ丁-I ! ! : !
}
1
i rllrflL
I TI 1 1 1 1 1 i
Lit r I 1 1 了 LT i 1 I i
1 TT1 I 1 I 1 小： 1 그그
'

1

LIERL
士
1

{1

I-

I I I
匕1卜亡寸
尸r丁小1卞

,1卜．

，小
：그小

叫

小＋

!

12 L

itiiiiI I I ,

I

i

II

r나 卄갸”

亡

I-거 卜hr 「
나a1

寸1

小m卜叫

토人I

나匕L，小』교

小卄」

I i i !

T

r)

1』

1.1

I

1寸”中

나寸小

,--

茸

니山r什

나
二1J

H-

,1j1

-

1

!m "
亡“'

CHAPTER

니H 뇨나＋-I小小卄HH小i小

iT丁丁了

：卄；

I-

H-I

:" ' [ T 1 ! ! ! I t ( 1 LT T 1 I l I 1 1 I
.
't"'
"小丁二 H. '

;

了

It：

‘

r

L

「 ti
L「丁十二“

I

-

14

i:

-I

It

I

卜4叫뇨4小

i;

芽
i1
-i

小

!

甘斗4

f-

!

그’

I I I

샤

H

-L나＋

d크，

1
i

I-

!

十 i

1

＝十니

4414 Ha＋上4- CONTENTS
小나 -r나，-, 三

11十，工

'

!

!

LESSON 02누적분포함수와확률밀도함수
LESS아寸03아날로그변조와복조

中-t小L小뇨j 山

LESSON 04아날로그H디지털변환

L叫L如乙냐H

了 丁 !

r寸寸寸＝寸山

m卜小小
1!
I三

!i1
!
1
H나나＋山卜H＋二中-4小 니 m 二 小小I小小-i 小H H

艸L二小뇨叫나H ---I

!
小

i
H !

LESSON 06디지털변조

+1

小小L

土小中

LESSON 05 신호잡음

4
=L1＝寸丁“十呻4m工的二mL,
,＋

m小上m그H小

i

L_ L그小 1

11卜나긱-J
H 'j

叫L

LESSON 01 확률

小뇨小工그小

니

I I
]

니＋

1끼

尸小卜寸艸t艸十

n
L

r
I

1m

m4m小

-I了二

F1

'

1

I

I

卞’

I!

LL

브
.

1巴少才I i丁r丁了 ! ! 1r了丁丁丁小口＝小1如
L

1

{

11
r

1

11

1

r1

-]-1-

小！

小

尸mI I ,if :t十fi-t:
J:_r__
JilV Il표二111L
山上I

LESSON

01

확률

확률은 실험에 의해 여러 가지 결과가 나올 수 있는 표본 공긴뻐因 어떤 사건이 일어날 것인지를 실수로 변환하는 방법이다．
통신의 기초인 확률을 MATLAB 스크립트 파일로 작성하고 그래프를 통하1 그 결과를 확인해보자．

Keyword

1 cell 1 hist I rand I randn I max I mean I mm

I round I std I

주사위의 확표

I

육면체 주사위를 한 번 던질 때 나올 수 있는 1부터 6까지의 주사위 눈, 즉 발생할 수 있는 모튼 경우를 표
"

.

6

본공간（samnie snwe）이라고한다. 이때 주사위 눈이 2가나올사건의 획률은 느］다. 획률은원古陪
.

사건이 발생하는 경우의 수를 모든 가능성을 지닌 표본 공간의 수로 나누어 구한다．

I 예工II 12- 寸 !
!
륙
'

"

"

M-File I 베stD池.m

H

；在

육면체 주사위를 ] 00번 던졌을 때 주사위 눈의 빈도수를 히스토그램으로 나타내라．

지식

' ceil

벡터 x의 원소를양의 무한대에 가장가까운정수로반올림하는ccii 함수의 기본형태는다음과같다．

ce카지

1hist
벡터 x의 원소를 陟II의 막대그래프（히스토그램）로 나타내는 노St 함수의 기본 형태는 다음과 같다．

h治t(x, n)

1rand
0과 I 사이의 실수를 무작위로 골라7刃 X77 행렬을 생성하는 rand 함수의 기본 형태는 다음과 같다．

rand(m,n)
.m 생성할 행렬의 행 수
· n: 생성할 행렬의 열 수

348

PA日103. M月ILAB활용하기

rand(n）은 0과 1 사이의 실수를무작위로 골라n Xi 행렬을 생성한다．
1randn
평균값이 0이고 표준편차가 1인 정규분포된 무작위 실수로 구성된 m ><n 행렬을 생성하는 randn 함수의 기
본 형태는 다음과같다．

randn(m,n)
· m: 생성할 행렬의 행 수
· n: 생성할 행렬의 열 수

1-

JJ 네5tDiem
m=U1J;

5-

4-

3-

2

6-

풀이

寸

x=cei I (6.rand(l . n)); <1
hist (x』1:6); 0

xlabel ( 'Spots an a Die ) ;
미ab이 ( ’北so 山te Frequency ) ;
title (Rsl l aDie Histogram ) ;

그림 12너 주사위 눈의 빈도수로 히스토그램 그리기 코딩 결과（H暾De.m)

Orand 함수의 결과어］ 6을 곱하여 1과 6 사이의 실수를 생성한다. 여기에 ceil 함수를 이용하여 가까운 정
숫값으로올림한다．
0 hist 함수를 이용하여 무작위로 얻은 값을 히스토그램으로 나타낸다．

그림 ]2-2 주사위 눈의 빈도수로 히스토그램 그리기 실행 결과

HistDie.m에서 randn 함수를 사용했으므로 무작위로 실수가 발생한다. 따라서 이 결과는 HistDie.m을 다
시 실행할 때마다 다르게 나타난다．

CHAPTER 12. 통신

349

평균, 표준편차, 분산

I

확률에서 평균mx와기댓값E的는같은의미로, 이는확률변수工의 위치를 나타낸다. 분산은확률변수

[（工 mx)

(12.1)

2]

=

E

var

（工）

가 평균으로부터 얼마나 떨어진 곳에 분포하는지를 나타내며 다음과 같이 정의한다．

표준편차 ax는 분산의 제곱근으로 분산보다 더 자주 사용되며 다음과 같이 정의한다．

ax = 而砥x)

r예저112-21

(12.2)

M-FiIe I HistMean.m

평균이 10, 분산이 9인 정규분포의 확률 수 2000개를 생성하라. 또한 생성된 확률에 대한 평균과 분산을 겨1
신后泣 히스토그램으로 나타내라．
H

배명

지식

=

rn 口V
"

' 나八

벡터 x의 원소중에서 가장큰값을가진 원소를선택하는max 명령어의 기본형태는다음과같다．

m針（지

1mean
벡터 x어］ 저장되어 있는 자료의 평균값을 계산하는 mean 함수의 기본 형태는 다음과 같다．

mean（지

1mm1l
벡터 x의 원소 중에서 가장 작은 값을 가진 원소를 선택하는 mm 명령어의 기본 형태는 다음과 같다．

mm （지

1round
벡터 x의 각 원소를 가장 가까운 정수로 반올림하는ro叫I 함수의 기본 형태는 다음과 같다．

round（지

350

PART 03. MATLAB활용하기

1std
벡터 工어］ 저장되어 있는 자료의 표준편차를 계산하는 std 함수의 기본 형태는 다음과 긷다．

std（지

摩

H台nm려tm Sq
n = 四（刃；
e3.randn(I, n)너O; <1

工쿄

4

1J 秀meanCe) 0

二
d

S겹 = std(x) ; 自

八
b
n
r
1
8

vari ance. .x 쯔 S겹坦 U
C = lround(.ln(x)):round(.ax(x))1 ; 0
tiist (x, ; O
y)

n
< Q
U

2-

1

풀이

口
나
0

elabel ( 'Randore Values ');
미abel ( 'Absolute Frequency ');
title ( 'Histograa of Randum Numbers) ;

그림 ]2-3 평균과 분산 계산하71 코딩 결과（HistMeanm)

Orai너n 함수를 이용하여 평균이 10이고 표준편차가 3인 정규분포된 실수2000개를 무작위로 생성한다．
e 1n明n 함수를 이용하여 2000개 무작위 실수의 평균을 계산한다．
Ostd 함수를 이용하여 2000개 무작위 실수의 표준편차를 계산한다．
0 표준편차를 제곱하여 2000개 무작위 실수의 분산을 계산한다．
0mmll 명령어와 max 명령어를 이용하여 무작위 실수의 최솟값과 최댓값을 구한 후 round 함수를 이용하
여 반올림한다．
0 생성된 확률을 히스토그램으로 나타낸다．
Commend

n

>> Hi stMean
m 乂 =
1 0. 0697

variance_c =
8 8255
그림 12-4 평균과 분산 계산하기 실행 결과

CHAPTER 12. 통신

351

F沁

Ed往

\／田咐

：그 L3 d 立

ime代

뉵

10口Is

Desktop

Window

H미口

" , 4,. 4nb 9 宦 J1 . 口』 ［그 回 =} 口
네S幻gram of Rare杓m Numbers

聊
m
伽

＞은山그g上 山弓a8 <

5

10
Ran幻m Values

그림 ]2小 히스토그램 실행 결과

352

PART 03. MAT냐＼B 활용하71

15

LESSON

02

누적분포함수와 확률밀도함수

누적분포함수는 임의의 확률 분포에 대해 확률변수가 특정 값보다 작거나 같을 확률을 나타낸다. 확률밀도함수는 확률변수의
분포를 나타내는 함수로, 특정 구간에 대해 적분한 값이 구긴에 포함될 확률값이 되는 함수이다． MAT나＼B 스크립트 파일올
이용하여 누적분포함수와 확률밀도함수의 그래프를 그리고 차이점을 알아보자．
Keyi사ord

I

I 누적분포함수 I sum 1 St졔rs 1 sort I 확률밀도함수 1 normcdf I normpdf 1

누적분포함수

확률변수x는 계산한 확률을 서로 연결한 것이다. 누적분포함수（cumul餌ye distr小Ut幻n 凡nction) 에
서 확률변수는 다음과 같이 집합 （小以）, 兀］에서 사건 伍 드 工｝의 확률로 정의한다．
/；노（功 =／江x< 키

1 예제 12- 3 I

(12.3)

M-File 1 CumDistFn.m

주사위 2개를 동시에 20번 던질 때 나오는 주사위 눈의 합에 대한 누적분포함수를 나타내라．

jjj

지식

'
sum
벡터 x의 원소를모두더하는sum 명령어의 기본형태는다음과같다．

sum（지
口 stairs
지정된工에 대응하는y의 위치를 계단 형태로 그리는 St耐S 명령어의 기본 형태는 다음과 같다．

stairs(x, y)

1sort
벡터 x 의 원소를 오름차순으로 정렬하는 sort 명령어의 기본 형태는 다음과 같다．

sort（지

CHAf玎ER 12. 통신

353

1

CumDistFn.rn
I-

n =20;

r

2- u:sui,
(ceiI(6.r삥，
3stalrs(Iiin(x)
s。2n)));
rt(x)]..[O:1/Iength(x):1J); 0
)ilabel ( 嫩m尉 ' ) ;
미ab이 C俄川已舡X) } );
tltle ( 'Cumulative Distribution Function ) ;

卜

4中
5-

그림 12中6 누적분포함수 그리기 코딩 결과（CumD暾Fn.m)

0 주사위 2개를 동시에 던졌을 때의 확률을 지정하기 위해 rand 함수의 결과에 6을 곱하여 1과 6 사이의
실수를생성한다. 여기에 C네 함수를 이용하여 올림한 결과를sum 명령어로 더한다．
Omm 명령어를 이용하여 최솟값을 구하고 sort 명령어를 이용하여 오름차순으로 정렬한다. 여기어］ stairs
명령어를 이용하여 결과를 계단 형태로 그린다．
F加

帥t

View

｛그 d a 曲

If匕eut

To야5

［沌5虹op

Wi,心D놔

b 1 鼠 曳 劫自 是 尻 니 目

1

Help

口 듣多 U 口

（hon
Cum마alive［가stributi이iF出

5

6

7

8

10

11

x

그림 12규 누적분포함수 그리기 실행 결과

가(x）는단조 증가함수이고 O 5F노（x) Si이다．

I

확률밀도함수

확률밀도함수（probab小口 density 凡nction）는 다음과 같이 누척분포함수 F노（工）의 도함수로 정의
한다．
（:)= dF, (x)
人
（在

354

PART 03. MATLAB활용하기

(12.4)

싸I-Ale i Gum다obFn.m

1 예제 ]2- 4 I

평균이 2이고 표준편차가 3인 정규분포의 확률변수 x에 대하1 균일한 간격으로 x값이 200개 놓여 있을 때
누적분포함수와 확률밀도함수를 각각 나타내라．

비1껑
지식

1normcdf
평균m x, 표준편차Si압na x인 정규분포의 확률변수工에 대한누적분포함수P를구하는normcdf함수의
기본 형태는다음과 같다．

P = normcdf(x, m_x, sigma_x)
· p: 누적분포함수
· x: 확률변수
· m,下 평균
· 引gma_x：표준편차

1normpdf
평균 m玉 표준편차 sigma工인 정규분포의 확률변수工어］대한확률밀도함수尸를 구하는 normpdf함수의
기본 형태는 다음과같다．

P = normpdf(x, m_x, sigmamx)
· p: 확률밀도함수
· x: 확률변수
· mx: 평균
' 引gma_x: 표준편차

1

iJCumPw,bFn.m 미 + l
4

1 23-

U
F

6
r
n

8

-

9-

n
亡

It ] n
J
4
L
U

-

16-

n=2EU;
rn_x=2;
引 am乞未＝3;

x=-12:O.UI: 2;

F기＝norrncdl Cx, ._兄引grna_x) 0
P2=no rip小似rn_a，引a虹砧 0
oubplot (211) ;

plot(x,Pl); e

비的이 C.俄m尉J ;
ylabel ( 개bf{F_X(o) ));
title (Cumulative Distribution Function) ;
subplot (212) ;
이ot (x，陀）; C
xlabel ( ‘싻m尉 ‘ );
비abel ( 俄) f{ f_X(X) } ) ;
tltle (Probabi l lty Density Function ') ;

그림 12田 누적분포함수와 확률밀도함수 그리기 코딩 결과（CumProbFn.m)

CHAPTE日 ]2. 통신

355

0 normcdf함수를 이용하여 평균이 2, 표준편차가 3인 정규분포의 누척분포를 구한다．
0 normpdf함수를 이용하여 평균이 2, 표준편차가3인 정규분포의 확률밀도를구한다．
0 누적분포함수를 그림 창 위쪽에 나타낸다．
0 확률밀도함수를 그림 창 아래쪽어］나타낸다．
Ed作

＼加W

I,姑甘t

(相攷top

1

WIn&畔

C내m山ativa Dbtiibution Fwdion

1

0
-15

ToOEE

'\ '\ 抑自咽 而 , 邑 口 困 1 口

-10

-5

뀌佃

｛그 d 니 缸 b

0

5

10

15

a

Probe벼良y Den甘却 F벼ct아l

a

그림 ]2+ 누적분포함수와 확률밀도함수 그리기 실행 결과

I

가우시안 확률변수

확률변수x의 항으로 확률밀도함수를 정확하게 기술하기란 쉽지 않다. 따라서 일반적인 조건에서 확률변
수 성분을 증가시키면 확률변수의 누적분포함수는 가우시안 확률변수（Gaussian random variable）로
접근한다는 사실을 이용한다. 가우시안 확률변수는 정규 확률변수라고도 하며, 임의성을 포함하는 문제
어］ 자주 등장한다. 또한 전체 실숫값을 취하는 연속 확률변수로, 확률밀도함수는 다음과 같다．

，耳叫 (' ;？口
加）=V/

(12.5)

I 중심극한정리
평균이 n吹이고 분산이 畦 이며 서로 독립적으로 동일하게 분포하는 확률변수 刃깨의 합을욱이라 할 때，
n 이 커지면 적절히 정규화된 S뛰 누적분포함수가 가우시안 확률변수의 누적분포어］ 가까워진다는 것을
중심극한정리 (central 血nit theorem)라한다．

356

PART03. MA凡A8활용하71

M-File I Cent니m比m

1 예체 12- 5 I

동시에 주사위 10개를 20000번 던져서 나오는 결과를 누적분포함수로 나타내라. 독립이며 동일하게 분포하
는 확률변수x의 평균 肋'= 3.5일 때의 결과를 중심극한정리를 이용하여 구하고 그래프에 나타내어 비교하라．
풀이

;

CentLim4m

I2345-

可

+

n=2W叩；
k=lIJ;
x=sum(cell (타rand(k』n))); (1
stairs([min(x) sort (m) ] j0:1/length(x):l] ); 0
m. .x=3. 5;

-,m,,x, 2); 0
var:(sum( 11:6] .,2)/，므，
m1k.i...m*sqrt (k*var)*randn(l n); C

67-

8910 ==
Ii 12-

hold;
stairs(]min(al) sort (xl) J, [O:1/ leogth(川) :1] 'r ) ; 0
川abel ( 甘바｛澍 ) ;
비abel ( 壯)HF_Xb) } ) ;
title( Central Limit Theorem ) ;

그림 ]2너0 중심극한정리를 이용하여 누적분포함수 그리기 코딩 결과（Con山m4m)

0 rand 함수를 이용하여 얻은 값어］ 6을 곱하여 l부터 6 사이의 실수를 생성한다. 여기에 ceil 함수를 이용
하여 무작위로 얻은 가장큰 정수의 값을 sum 명령어로 모두 더한다．
0 누적분포함수를 그린다．
0 하나의 주사위를던졌을때의 분산식 아 =E（戶卜磁을지정한다．
<) 주사위 10개를동시에 던질 때 평균이 丸mx이고표준편차가Si瓦｝인정규분포를계산한다．
0mm 명령어를 이용하여 최솟값을 구하고 sort 명령어를 이용하여 오름차순으로 정렬한다. 여기에 stairs
명령어를 이용하여 결과를 계단 형태로 그린다．
F如 曲t

vle나

D t3 H 命

Inset

To帥三

0甘虹op

Window

He巾

臣 3\ （료也的自 嶼 尻 r 昆 ［그 目

南口

由niral Lii忖tTheorem

1
0.9 니
0.8 1
0:7
0.6
Se
二 (}5 "
111
0.4 0.3 느
0.2
0.1
0
10

15

20

25

支I

35

40

45

x

그림 12-11 중심극한정리를 이용하여 누적분포함수 그리기 실행 결과

가로축은주사위 10개를동시어］던질 때1 나오는주사위 눈을합한 것이다. 계단 형태로 그려진 누적분포함수
는 단조 증가하고．주사위를 던지는 횟수를 20000회 정도로 늘리면 이 누적분포함수는 연속적인 곡선 형태
를 띠는 가우시안 확률변수의 누적분포에 가까워진다．

CHAPTER 12 통신

357

LESSON

03

아날로그 변조와 복조

아날로그 변조는 아날로그 신호에 의해 반송 신호의 진폭, 주파수, 위상 정보를 변경한 신호를 얻는 것이다. 이는 여러 신호를
주파수 대역에서 분리하여 동시에 다중 신호를 전송하거나, 잡음을 걸러내어 증폭이 용이한 대역으로 스펙트럼을 이동한다，
이와 반대로 아날로그 복조는 변조된 반송파어써 원래의 정보를 갖고 있는 메시지 신호를 추출하는 과정이다. 메시지 신호와
반송 신호를 사용하여 시간 영역과 주파수 영역의 진폭 변조 및 주파수 변조를 짖빠내고 그래프를 통하1 비교 · 분석하는 과정을
알아보자．
Keyword

I 아날로그 변조 1 양측파대 진폭 변조 1 주파수 영역에서의 진폭 변조 1 nextpow2 1
1 시간 영역에서의 주파수 변조 I cumsum 1 아날로그복조 1

I

아날로그 변조

아날로그 신호를 사용하여 반송 신호의 매개변수를 변경하는 것을 아날로그 변조라고 한다. 변조 방식으
로는 진폭 변조, 주파수 변조, 펄스 변조 등이 있으며 이 책에서는 진폭 변조와주파수 변조를 다룬다．

I

양측파디1 진폭 변조

진폭 변조（AM: An叩血ude Modulation）는 전송하고자 하는 메시지 신호 m(t) 에 코사인 파형 반송 신
호 c(t) = AC cos(2兀／Ct）를 곱함으로써 코사인파의 진폭에 정보를 실어 보내는 것으로, 주파수 영역에서
차지하는 대역폭이 신호 대역폭의 두 배가 되므로 양측파대1 진폭 변조（DSB-AM）라고 한다．
메시지 신호와 반송 신호에 의해 양측파대 진폭 변조 방식으로 변조된 신호는 다음과 같다．
mDsB(t) = m(t) x c(t)

(12.6)

M-FiIe 1 AnalAni.m

I 1뇌IiII 19- a I

양측파대 진폭 변조 방식을 이용하여 반송 신호 c(t)로 메시지 신호 m(t）를 2초 동안 변조시킬 때 메시지 신
호. 반송 신호, 변조된 신호를 나타내라. 이때1 반송 주파수는 15[H기이다．
c(t) = 3cos22rft
m(t) = cos22rt

358

PA日T 03. MAT냐＼B 활용하71

끄

Aria出m.m
t_ l=0; t_s=1/lX刃; t_ f=2;
t=t_ i :t_s:t_ f

1
U
U
1
U
4
U
1
m
1
1

subp比t (212) ; 0
plot (t .....D田) ;
뉘 abel ( 'T 油8 (sec) ');
title ( 卜｛odulated signal ') ;

그림 12-12 양측패41 진폭 변조 코딩 결과（AnalArn.m)

0 메시지 신호加(t)를 지정한다．
0 반송 신호 c(t）를 지정한다．
0 식 (12.6）을 지정한다．
Osi小plot 명령어와1如t 명령어를 이용하여 메시지 신호를그림 창위쪽어匕1린다．
0 plot 명령어를 이용하여 반송 신호를 그림 창 위쪽에 함께 그린다．
0 subplot 명령어와plot 명령어를 이용하여 변조된 신호를 그림 창 아래쪽에 그린다．
F七 띠t

View Inset To必

E沁＄姓햐） 珝'I넜ow

p

끼

｛그 d 日 邕 b 戈 民 聊 匈 啞 d , 晷 ［그 匡그 m 口
Mess叩es抑n刊 and camr汨rsign出
2
0

1

1

1

0.2

0.4

1 1 )

4

\

1

0.8
1
1.2
Time (sec)
Modulated signal

4

L
16

18

2

1.6

1.8

2

H

2

-2

0

-4。

1

1

0.8

.

e

hold;

plot (t,c_t); 0

1'

n

미ot (t . 兀t. : ) ;
뉘abel ( Time (sec) );
title ( Plessage signal and carrier signal ');

.

1

f_c=15;
m_t=cos (2.pi.t) ; 0
c_t＝小cog（小미* i_c.比 0
LDSB=1=t．士Cmt; 0
subplot (211) ; 0

\

1

1 2 3 4 5 6 7 8 9 m n 俚 m H 巧 恰

1

풀이

02

0.4

0.6

0.8
1
1.2
기m이朗C)

1.4

그림 ]2너3 양측파대 진폭 변조 실행 결과

실선으로 표시된 반송 신호의 진폭은 점선으로 표시된 메시지 신호의 진폭 절댓값에 정비례한다．

CHAPTER 12. 통신

359

賈 주파수 영역에서의 진폭 변조
주파수 영역에서 식 (12.6）의 스펙트럼은 다음과 같다．
,

.

／口DSB 'J)

dC , //r

r\ , A ,

= ＝二／W (J HJc) 十 二二／口 (/
/
乙

(12.7)

十 .'C,

식 (12.7）에는 반송 스펙트럼이 드러나 보이지 않으므로 반송 억압（suppressed carrier) 양측파대 진
폭 변조 방식이라고 한다. 이 방식에서 차지하는 전송 대역폭은 메시지 신호 대역폭의 두 배이다．

M-FiIe J AnalAmFreq.m

1 여以II 12- 7 I

[0카저112-이과 동일한 메시지 신호와 반송 신호를 사용하여 주파수 영역의 진폭 변조를 나타내라，

；而
지식

'nextpow2
2尸2 1미 조건을만족하는첫번째P의 값을구하는ne晦刃w2 명령어의 기본형태는다음과같다．

nextpow2(n)
이 명령어는 고속 푸리에 변환 실행에서 두 연속 길이의 가장 가까운 멱승을 찾는 데 유용하다．

m x +l
'J1 - AnafAmFteq,
t_卜刃； t_o=1/1lI刃； ti= 2;
H
1
1
느
4
m
4
4
1
n
4
1
느
e
小
U
斗
1
4

t=LJ :t.,,o :t_ f;
L,e＝陌; f,..s=I/ t_o;
L川n=O. 3; <1
n=2 ' (max(nextpo.2(length(t)Lnextpo.2(f日s/L. ln) )); 0
f,,,act=f_o/n; 0
f=(fJ: f.,,act :f,,,aCt*(n너 )）나小o/2; 0
Lt孔oo(2ap1.t) ; 口t＝小cos(各小Lcat) ; 0
N_f=fft (m_t, n)/l,,.s; 0
m_D田팎肥上0
t呻＝Ift (.－呻，n）月小 0
subplot (211) ;
미ot ( f I I tabI岫呵HJ))); e
a川S( [a 印 0 I .II) ;
olabel (Frequency (七) ') ;
title ( 'Message signal in frequency domain ') ;
subp lot ( 212) ;
plot山ftshift (ab咐羽3) )); m
acIo(L-印 600 1 .6) );
olabel (Frequency (Hz) ') ;
title( '卜伯dulated signal in frequency domain) ;

U

2 3 45 6 7 8 9 mn 泛 日 H佰怜 n 化四 계 기

폴이

그림 12-14 주파수 영역에서의 즈목 변조 코딩 결과仍r也tAmFreq.m)

0 원하는 최소 주파수 해상도를 지정한다．
0 nextpow2 함수를 이용하여 2."P >= abs (length(t)）와 2.午 >= abs (fs戊工血1)의 조건을 만족하는
P의 값을 각칵 구한다. 여기에 max 명령어를 이용하여 구한 최댓값의 2의 멱승을 계샨한다. 이렇게 겨1
산된 刃 값을 이용하여 고속 푸리어］변환을 실행할수 있다．

360

PART 03. MAUAB활용하71

0 실제 주파수 하상도를 지정한다．
0 주파수 벡터를 지정한다．
0 메시지 신호 m(t）와 반송 신호 c(t)를 지정한다．
0 메시지 신호어｝대한 고속 푸리에1 변환을 계산한다．
0 식 (12.6）을지정한다．
0 변조된 신호어i 대한고속 푸리에 변환을 계산한다．
0 주파수어］따른 메시지 신호를 그래프로 나타낸다．
@ 주파수에 따른 변조된 신호를 그래프로 나타낸다．
F作9

EdIt

W州 批mt

Tools

沁5i娜1 蜘岫：刈

U帥）

：그 =} 日 由 m \ 느＼畇自咽 / 니 晟 口 듣크
M日嚼age signal in 加quer叱ydornain

-40

-20

0

20

40

60

40

仗｝

Frequency (Hz)
枾Dd미ated 섧gnal in frequ미-It斗（幻main

-40

-20

0

寸

才）

Frequency (H지
그림 12甘］5 주파수 영역에서의 진폭 변조 실행 결과

위 그림에서 스펙트럼은 정확히 반송 주파수 15[H기만큼 대역이 이동된 것을 확인할 수 있다. 이 방식어써
차지하는 전송 대역폭은 대략 80[H기로, 메시지 신호 대역폭40[H玎의 두 배이다．

I

시간 영역에서의 주파수 변조

8)

(12.

k／
小帥］

［cot+

=

叩）

4呻

시간 영역에서 주파수 변조伍M小equet乂y Modulation) 신호는 다음과 긷히 표현된다．

여기서 勺는 변조기의 주파수 감도（se的帥ty）를 나타내는 샹수이고，주파수 변조 신호 s(t)는 메시지
신호 m(t)의 비선형 함수로 정의된다. 주파수 변조 방식은 대역폭이 넓기 때문어］진폭 변조와 달리 신호
의 스펙트럼을 메시지 신호와 연결하여 해석하기가 매우 어렵다. 반면어］잡음어］대해서는 강력한 성능쇠
라는 장점이 있다．

CHAPTER 12. 통신

361

M山File I An톄Fm.m

1 예제 12- 8 I

-0.04 5 t < 0.04[sec] 동안 주파수 감도 t/ = 80兀이고 반송 주파수 兀 = 150[H기． 샘플링 주파수
/;= 10000[H기인 다음과 같은 삼각 아날로그 메시지 신호에 주파수 변조 방식을 이용한 결과를 나타내라．

m(t): -1+
1-1 亡：；」荇：t.。2)
。깖，
0)
h雁i

지식

'cumsum

蚌江의 원소누적 합을포함하는벡터를생성하는cumsum함수의 기본형태는다음과긷다．

cumsum(x)

乙rAl畔仇m 냐聾鼠

10ii
12-

1314 -

兀t=a2*m4; 0
k_f＝好pl ; 0
..

18 19-

미ot (t, m口t) ; O
xlabel ( 'Time (nec) );
미ab이 ( 'rn(S) );
tltl이 겨essage 引anal );
arid;
subplot (212) ;

2021 222324 -

p比t (t, s_t) ; 0
xlabel ( 'Time (sec) ') ;
ylabel ( 's(t) ') ;
titl日C FM 引anal );
arid;

1516 I? -

1

0

lnt. t= s. cu.su.
;
s_t=cos(2.pl너....c.t. k_f* lnt_._t) ; 0
subplot (211) ;
_t)

6789中

Lsr1U刃； LC미田；0
t_l=-O.04; t_s=1/f_s; t_f=0.04;
t=t_ l :t_s:t_ f;
tl=-.lJ. 02:l/ 1 MIXJ:0; t2=O:1/1l1刃:O.1 ;
ml＝니83*ahs (tl. .0.Ol) ;
m2= ]zeros(lI 2刃] L. 1.,zeros(] 1 4刃] )];
ffl3＝너너［刃＋a뇨(62-0.미）;
m4=[Zeros( (l 4111] ) ,.3,zeros(I1 2111] )] ;

(.

l m

2 3 4 5 -

6_

풀이

그림 12-16 시간 영역에서의 주파수 변조 코딩 결과（A1님Fm.m)

0 샘플링 주파수五와반송주파수兀를 지정한다．
0 메시지 신호는 모두 801개의 원소를 갖는다．
0 주파수 감도를 지정한다．
0 cumsum 함수를 이용하여 식 (12.8）의 적분 항을 계산한다．
0 식 (12.8）을 지정한다．
0 시간에 따른 메시지 신호를 그림 창 위쪽에 그래프로 나타낸다．
0 시간에 따른 주파수 변조 신호를 그림 창 아래쪽에 그래프로 나타낸다．

362

PA日T03. M月江AB활용하기

D t3 日白 Lt i 曳 {\ 好 @ 咽 d , 目 口 匡크

그림 12-17 시간 영역에서의 주파수 변조 실행 결과

I

아낟로그 복조

변조된 신호의 복조（den珣dulation）는 다음과긷히 변조 신호에 반송파 신호를 곱해서 구한다．
mDEM(t) = mDsB x c(t) = m(t)(c(t))2

(12.9)

식 (12.9）에서 반송 신호가 叩）= A cos22rft 일 때 삼칵함수 항등식을 이용하면 다음과 같이 계산

(1 + cos

(12.10)
42rft)

(t)

孕
m

=

mDEM

(t)

된다．

복조신호는크키가 笙배인메시지 신호와이 신호의주파수를4可，[Hz］로변조하여 대역 이동한신호
2
의 합이다．

CHAPTER 12. 통신

363

M-File I AnalAmDem.m

1 예제 12- 91
［예제 ] 2-이의 진폭 변조된 신호에 대한 복조 신호를 나타내라．

풀이

1 1

Ana山Dem.m
+
t_i=U; t_s미/icx刃； t_ f=2;
t=t_ i :t_s:t_ f ;
1

< n
J
n

1 -

4

f_c=I5; 0
兀t批s(2*小t);0
口t=3*ccs（帥汁f_c，比 0
rfl_DSB=m_t,*c_t; C

二
U
n
b
r
n
B

m_DEM=m_DSB.,c_t; 0
p比t (t, 9.io_t, 'r: ' , t;m_D태) ; 0
xIabeI ( Tme (sec) );
ylabel ( 卜1agnitude ');
title (Demcdulated 引9nal );

口
U

小

10-

그림 ]2-18 복조 신호 그리기 코딩 결과（Am山nDeni.m)

0 반송 주파수를 지정한다．
0 메시지 신호 加(1)를 지정한다．
0 반송 신호 c(t)를 지정한다．
0 식 (12.6）을 이용하여 양측파대 변조 신호를 지정한다．
0 식 (12.9）를 이용하여 양측파디：1복조 신호를 지정한다．
0 복조 신호와 복조 신호를 따라 움직이는 포락선 형태의 메시지 신호를 그리기 위해 반송 신호의 제곱인
9를 메시지 신호어］곱한다．
F加 Ed作

\／他卄 岵ert To머$

｛그 巴 日 $

b

\"\

De帥t아） 쌔ndow

H叫p

抑 自 咀 d , 邑 口 듣크

시

m口

［뇨mod내ated 出gnal

10
8
6
4
n
i

m꼬d릎담玉

/

0

1

\

1

11

1 1/

1

4
七
8

1
0.2

0.4

06

0.8
1
1.2
기n也（羽c)

1.4

1
1.6

1.8

2

그림 12너9 복조 신호 그리기 실행 결과

위 그림에서 복조 신호의 시간 파형 포락선이 메시지 신호임을 알 수 있다．

364

PART 03. M月TLAB활용하기

LESSON

04

아날로그－디지털 변환

아날로그 신호를 편리하게 처리． 통신， 저장하71 위해 디지털 신호로 바꾸는 과정을 아날로그－디지털（ND: an톄og/d呼tal)
변환이라고 한다. ND 변환은 연속 신호를 이산 신호로 d나는 샘플링, 이산 신호를 특정한 레벨 값으로 지정하여 디지털
신호로 만드는 양자화, 디지털 신호를 디지털 시스템의 처리 방식에 적합한 코드로 표현하는 부호화의 단계로 이루어진다．
MATLAB 스크립트 파일로 작성된 반올림 양자화기佃uantizer）를 사용하여 양자화된 신호를 실행해보자.
Keyword

I

I ND 변환 1 양자화 1

양자화

앙자화（quantization）는 샘플링으로 얻은 이산 신호를 크기어］대해 이산화하여 시간과 크기를 모두 디
지털 신호로 바꾸는 과정이다. 디지털 시스템에서 b비트 신호를 처리할 때는 신호를 2b개의 레벨로 나누
고 원래 신호의 값을 반올림한 앙자화 레벨 값으로 대치한다. 이 과정에서 발생하는 정보의 손실인 양자
화 오차는 디지털 시스템의 성능을 떨어뜨리는 원인이 된다．

M-FiIe 1 Quantize.m

1 예저I 12- 10 I

정현파 신호 工（t) = 誼l2兀t를 주7탕 1000개의 표본으로 샘플링하여 3비트와 4비트 반올림 양자화기로 양
자화한 각 신호를 나타내라．

-

( jan恤e,m ;t

1+ f

勺

小3; b七4;
t=O:O.13J1: l;

Lt＝
引n(2奸j.t) ;

4

fJ=1aX(X1t)1川n(X1t);0
이上＝2b1; q2. .L=2b2; 0
ql_d=L.R/ql上; q2. d=t_fl/ q2_L;
xl中q긔l....d*round(a_t/ql_d) ; C
x2. .q=q2. .d.round(a. .t/q2. .d) ;
subplot (211) ;

1
4
4
e
1
1

pIot(t,x_t. ' r ,t:xl_q); 0

1

axis([ U 1 - 1 . 1 i .i] );
xlab引 ( 삐 H나 ) ;

U
e

이 ab이 ( 겨a므nit ude ) ;

4

title (2uantizerbyasing3bits ') ;

中

subp 比t（기 2) ;

U

pIot (t,x_t, ' r ', t』x2_q); 0

1

aais( [0 1 -1 . I 1.1] );
xlabeI ( 甘it{ t } ');

m
1

미 ab이 ( 겨agriitude ') ;

4

1 2 3 4 5 6 7 8 9 m n 口 口 m 侄 冊 口 田 円 계

풀이

1

title ( '0uantizerbyusing4bits ' ) ;

그림 12-2() 양자화 신호 그리기 코딩 결과（(）月n血e.m)

CHAPTER 12 통신

365

0 서로 다른 양자화기의 비트 수를 지정한다．
0 신호의 전체 구간을 지정한다．
0 비트2개에 대한 잉짜화 레벨의 수와 잉짜화간격을 계산한다．
0 샘플링된 이산 정현파 신호의 값을 앙자화 간격으로 나눈 뒤 round 함수를 이용하여 반올림하면 양자화
레벨을 얻을 수 있고, 여기에 잉짜화 간격을 곱하면 잉짜화한 신호를 얻을수 있다．
0 원래 신호와 3비트 양자화 결과를 그림 창 위쪽에 나타낸다．
0 원래 신호와4비트 잉짜화 결과를 그림 창 아래쪽工네 나타낸다．
Hb 日艮

啣

Dl哨幻p

싸In汁

He乍

D d 日邕 1 巨 1 吼 艮 凸自咽 石 기目 口 匡갚is 口
QI心1吐E8f by u出也 3L出$
5 0 5
0
n
m乙그卄三g>
녀
01

02

0.3

0.4

0.5

06

07

08

09

0月

09

f
1

QI川iter by ui出目4 bls

5 0 5
0
e
쁑글듕m듣
0

0.1

02

03

0.4

05

08

0,7

1

i
그림 12-기 양자화 신호 그리기 실행 결과

양자화한 신호에서는 정현파 신호의 값이 바로 샘플링된 이산 정현파 신호이므로 양자화 전후의 차이를 잘
살펴볼 수 있다. 유한개의 비트로 연속척인 값을 나타내는 것은 양자화오차의 근본적인 원인이므로 비트 수
를증가시키면오차를줄일 수 있지만, 비트수는다른문제와결부되어 있으므로무조건 늘릴 수만은 없다．

366

PAAT03. M月I냐＼B 활용하기

LESSON

05

신호 잡음

통신 시스템에서 피할 수 없는 현상인 잡음은 메시지 신호의 전송을 방해하므로 원치 않는 파형이라고도 한다. 잡음은 시스템
내부와 외부의 영향에 의해 발생하며, 잡음의 영향을 정량적 방법으로 설명하는 시스템 매개변수는 데시벨（dB) 단위를 사용하
는 신호 대 잡음 비율이다. 균일분포 백색잡음과 정규분포 백색잡음에 대한 파형을 MAT나＼B 스크립트 파일로 작성하여 분석
해보자．
Keyword

I 백색잡음 1 신호 대 잡음 비율 1

I 백색잡음
통신 시스템의 잡음 분석은 백색잡음佃hite noise）이라고 하는 이상적 잡음 형태에 바탕을 둔다. 백색
이라고 일컫는 이유는 백색 빛이 전자파의 가시대역 내 주파수 성분을 모두 포함하고 있기 때문이다. 전
력 스펙트럼 밀도（PSD: Power Spectral Dens幻）는 신호에 포함된 전력의 주파수 영역에서의 전력 밀
도분포를 나타내는데, 백색잡음의 전력 스펙트럼 밀도는동작주파수와상관이 없다．

I 신호 LH 잡음 비율
신호 전력이 잡음 전력을 초과하는 데시벨 수를 신호 대 잡음 비율（SNR: Signal-to-N아se Ratio）이라
고 한다. 신호는 단독으로 존재하지 않고 보통 잡음과 공존하기 때문어］ 그 배분을 나타내는 척도로 신호
대 잡음 비율을 사용한다. 이는 다음과 같이 구한다．
평균 신호 전력
1(J1og10 평균잡음전력 [dBI

[ 예工1I12-11 I

秘＋的 1 SigN이se.m

0 드 t 드 2[sec] 에서 정현파 신호 m(t) = sin2兀t（게 균일분포 백색잡음이 섞였을 때와 정규분포 백색잡음이

섞였을 ' 卄신호 ",）
『 m(t) + An(t）의파형을각각그려라．이때잡음의크기는 凡 1a：
。쇼忽 이고，균일
분포 백색잡음에 대한 신호 L卜1잡음 비율은 10[dBI, 정규분포 백색잡음에 대한 신호 대 잡음 비율은 5[dB]
이다．

CHAPTER 12 통신

367

+
t=O:O. 01 : 2;
m_t＝引n(2＋미吐）;
Un小rand（引Ze（耐n七．5; 0
m

的N出e.

E

剖

1

U
D

1 2小

1

H

4
中

U
二

H
1
1
1
m

(uni帥r/20川·, 0
gau_mas=(std(1_t) /std(gau_n) )士(1/(l了(gau. .snr/20 ) ;
Un匕S=N_t*U吐a呼삐小 C
gau. .s=m_t. gau. .Iag*gau. .n;
subplot (211) ;
P比t (t, m_t』十，t, un匕a) ; 0

m
4
1
1
H
m
m

1 1 1 1 1 1 1 1 1 1

寸

6 ? 8
0 1 2
4 5 6 7 B g
U
口
니
口

1

gau_rprandn(引
uni_snr=10; ga上咐＝5; 自
an匕mag=(std(m_t) /std(u쿄汕 (1/咐

xlabel ( 싸bt{ t} ) ;
미 的el ( 'Magnitude ) ;
title ( 'Un 向nfl 띠 at r i but ian 叫 th 밖hite no泊6 ) ;
sub口lot (212) ;

plot(t.._t, r ', t,gau_s); O
뉘 abel ( ‘咐）H나 ) ;

1

ylabel ( 'Magnitude ') ;
title ( 卜1口real distribut 比n 비th 뽀hite namSe ) ‘,

그림 12느22 백색잡음이 섞인 신호 그리71 코딩 결과（SigN)어sam)

0 균일분포 잡음과 정규분포 잡음을 생성한다．
0 균일분포 백색잡음과 정규분포 백색잡음어］대한 신호 대 잡음 비율을 지정한다．
0 균일분포 백색잡음과 정규분포 백색잡옴의 크기를 지정한다．
0 균일분포 백색잡음과 정규분포 백색잡음이 섞인 신호를 생성한다．
0 정현파 신호와균일분포 잡음이 섞인 신호를 그림 창 위쪽에 나타낸다．
0 정현파 신호와 정규분포 잡음이 섞인 신호를 그림 창 아래쪽에 나타낸다．
日tit

Vb므나

D 巴日 曲

We心t beta

臣

C珀5岫1耳1 叫Widow

’曳 曳 心 自 咽 /

, 目

$4目p
口 匡크

. 口

2

Uniform 小 hb川에 with 叫忖t目n야58

1

1 0 d
쁨글듬m>

1

0
2

0.4

02

0.4

2

02

0e

1
12
1.4
1.6
t
N아mat distribution 나仕h 나세te noise

0.6

0.8

1.8

2

i.e

2

1 0 d
쁨＝ 릍留玉

0.6

J
1
t

12

1.4

1.6

그림 12-23 백색집음이 섞인 신호 그리기 실행 결과

신호 대 잡음 비율이 작을수록 잡음쇠 섞여 있는 신호의 진폭도 감소한다．

368

PART 03. MATLAB 활용하71

LESSON

06

디지털 변조

아날로그 변조가 연속 파형을 나타내는 방식이라면 디지털 변조는 0과 i율 사용하는 2진 전송 시스템으로, 아날로그
변조보다
용량이 크71 때문에 더 많은 정보를 전송할 수 있다. 디지털 변조는 더 많은 정보 용량, 디지털 데이터 서비스와의
호환성, 더1
이터 보안의 우수성, 보다 나은 통신 품질, 빠른 시스템 가용성이 장점이다. MATLAB 스크립트 파일을 작성하여 그래프를
통
해 다양한 디지털 변조 방식의 차이를 살펴보자．
Keyword

I

1 진폭천이 변조 1 2진 주파수천이 변조 1 2진 위상천이 변조 1 卜小직교 진폭 변조 1
1 reshape 1 bi2de I modulate 1 modem.qammod I scatterplot I eyediagram I

진폭 천이 변조

진폭 천이 변조（ASK: Amplitude Sh侃 Keying）는 가장 간단한 디지털 변조 방식이다. 진폭 천이 변조
는 아날로그 변조의 진폭 변조처럼 반송파의 진폭을 통해 이루어진다．
0 드 r < 乙에서 전송되는, 심벌이 0인 파형은却(t）를 사용하고 심벌이 1인 파형은幻(t）를 사용하는 경우，
이 파형은 다음과 같이 나타낸다．
(t) =O
s。

(12.lla)

s1(t) = Acos(2刃t)

(12.llb)

여기서 兀는반송주파수를나타닌仁干．

1 （뇌1工朴 i: ,-i:

' I

M-File I DigiAsk.m

진폭 천이 변조의 통신 시스템을 이용하여 무작위로 생성되는 20개의 심벌（0 또는 l）을 연속으로 0 5t 510
초 동안 전송한다. 이때 반송파 叩）= sin(2兀t)룔 사용하여 기저대역 신호와 진폭 천이 변조된 신호를 나타
내라. 기저대역과 진폭 천이 변조된 신호를 나타내71 위해 2100개의 샘플을 사용하라．

CHAPTER 12. 통신

369

1 2 3 4 5 6 7 B 9 化 n 促 떠 伯 巧 出 W 化 円 四 기 匹

트 ! O呼AsLm 莪！浮j
叫i 工d = round('iand(1,20fl; 0
t = 0:0.01:10;
23N＝껌00; 0
4o = 1 :1:N;
5- 무for i =1:20
6- 芒] for 3 = j :0. 1니＋1
7- ! 뇨t(x(i시00：小1).lcxl) ) = 工dny,
8g 小 L end
H

e

풀이

中
1
1
H
m
m
1
小
1
1

1011-

b_t = bt (100:1100); e
c. .t = sin(20p1.t);0

4
1
1
1
m
中
4
H
+
1
1

12 13-

뇨t = 느t ．士C＝上 ;
subplot (211)

141516 l? 中
18-

plot (t, b_t) 0
aois(10 10 -2 *2) );
xlabel ( 寸바｛나 (nec) ') ;

2021 22-

aois([0 10-2 +2] );
비ab미 C物H나 (nec) );
title ( ModulatedtSKsignal ') ;

title ( 'Baseband di引tal 引snal ' );
subplot (212)

19-

p比t(t,s_t) e

그림 12-24 기저대역 신호와 진폭 천이 변조 그리기 코딩 결과（DigLAsKm)

0 무작위로 2진 심벌 20개를 생성한다．
0 기저대역과 진폭 천이 변조된 신호를나타내기 위해 2100개의 샘플을 지정한다．
0 缸晤 이용하여 100개의 샘플마다 무작위로 생성된 심벌을 나타낸다．
02진 데이터 10개에 대한 기저대역을 구한다．
0 주어진 반송파와 진폭 천이 변조 신호를 입력한다．
0 무작위 심벌을 이용한 기존 신호를 그림 창 위쪽에 그래프로 나타낸다．
0 쟈두천이 변조신호를그림 창 아래쪽에 그래프로나타낸댜．
F沁

Ed健

\new

Insert

Tools

Desktop 出no口畔

Help

J J d 可 自 十＼ =\ 抑 自 堤 d , 昆 口 匡크 三 口
Ba羽band d甘t카 sbnal

-2。

0

2

3

2

3

7
5
6
t（的디
Modu冶ted ASK 的3naI

8

9

10

7

8

9

10

4

4

5
t (s.c)

6

그림 12-25 기저대역 신호와 진폭 천이 변조 그리기 실행 결과

370

PAF국T03. M戶TLAB활용하71

rand 함수를 이용하여 무작위로 신호를 생성했기 때문에 DigiAsk.m올 실행할 때마다 신호 형태가 다르거1
나온다. 심벌 0에 대한 부분은 0으로 변조되고, 심벌 l어］대한 부분은 반송파 형태로 변조된다．

1 2진 주파수 천이 변조
2진 주파수 천이 변조（BFSK: B岫ry Frequ이icy Sh近 Keying）에서 부호 0과 1은 고정된 값만큼 다른
주파수를 가진 2개의 정현파 중하나를 전송함으로써 서로 구별된다．

같다．
i
匈

m

片片

시간 0St< 乙에서 부호 0을 나타내는 정현파 s0(t)와 부호 1을 나타내는 정현파 s1(t)의 쌍은 다음과

)

11

/

r
旬

cos(2 'r而t)

r

)

1H

\

/

여기서 Tb는 심벌 기간, 尻는 비트당 전송된 신호 에너지를 나타낸다．

1（네xII 寸9口_1!4 I

M-FiIe ! DgiFsk.m, DigiFskSpec.m

(a) 주파수 천이 변조의 통신 시스템을 이용하여 심벌 수가 io개인 디지털 데이터를 연속으로 전송하려고
한다. 디지털 데이터는 무작위로 동일한 확률을 가진 0과 l을 생성한다. 전송되는 데이터의 심벌 기간
乙 = I [Se이이고, 비트당 전송된 신호 에너지 Eb = 小Whit］로 가정한다. 그리고 데이터를 변조하는
. .

.

.

戶，

-

.

.

=

..

'

.

,

.

.

m1

.

.

m

,1

1

.

.

1

.

,

-

--

.

.

.

2

데. 사용하는 2개의 반송파 중 부호 l을 전송하는 주파수는 /1-；이，고, 무호 0을 전．송하는 주파수는
/6
4
肛計다 이때 기저대역 신호와주파수천이 변조된 신호롤 나타내라·
.

.

.

_

小

-4

.

.

m

,

.

m1

.

.

(b) 주파수 천이 변조를 사용하여 변조된 신호의 스펙트럼을 나타내라．

CHAPTER 12 통신

371

ii - Di"tFs認；
Os = 10八5; Tb = 1 ; E크）=1 ;
1

(a)

小쓰

丘

措뇨下耳m

1

< nJ 4
n

罰

11) = 4/Tb; ii = 2/Tb;
fs = 4* fo; N = fe/Tb; 0
t = 0:1/ fs:Hs.Tb;
工d = round(rand(l, Os) ); 自
b.t = zeros(l, Iength(t) );

2 U 6 nr
=

小
小
小

- 甲fsr i = i:NsQ

1 나 工d(i) U
노t ( (1：卜l) .N.( i니 )) = 1 ;

卜

8-

卜

! end

11 12-

Len4
s...t = zeros(1, length(t) );

1415 卞
16 尸
I? -

! if d_.d(i)
乞t ( (1:N）나h0너 )) = (sqrt (2＋日)/sqrt (Tb) ).cos(2士이＋ii. .t (1:H) );
日 lee
土t ((1:N)=H士（i너 )) = 佃qrt (冬日）/nqrt (Tb) ).c四（小이H0．士t (1 :H) ) ;

쁨：

13- 무far i = 1:Nse

2021 中
222324西而m
27田四-

0

[:：二

subplot (211)
이ot (t (1 :flf3) . 뇨t (l :113助自
axin([06.2 田. 1 1. fl ) ;O
xIabeI ( 嫩f{ t} (sac) );
title (Baseband digital signal ') ;
subr키ot (212)
이ot (t (1 :11 ), 乞t (1:I1JJ) )
axis(L0 6. 2 -1.6 1 .61) ;
xIabeI ( ‘嫩f t} (nec) ') ;
tltle ( f如dulated FSK 引gnal ' ) ;

그림 12-26 기저대역 신호와 주파수 천이 변조 신호 그리기 코딩 결과（미이円Km)

0 심벌의 수와심벌 기간을 지정하고, 서로다른 반송주파수2개를 입력한다．
0 샘플링 주파수와 심벌 하나어｝대한샘플의 수를 나타닌Ii斗．
0 rand 함수를 이용하여 디지털 데이터를 무작위로 생성한다. 메시지 신호는 종종 기저대역 신호로 변
환되며 시간축의 샘플수만큼 0으로 지정한다．
0 凡r문을 이용하여 1부터 10切｝지 지정된 심벌 수를 지정한다．
0il문을 이용하여 무작위로 생성된 디지털 뎨이터 값이 0이면 기저때뼉 값을 0으로 유지하고, 1이면
기저대역 값을 1로 유지한다. 이때 16개 심벌의 위치에 모두 0 또는 1을 연속으로 지정한다．
0

앞허Pd 기저때뼉 신호를 생성한 것과동일한 방법으로 디지털 변조된 신호를 생성한다.

O for문을이용하여 식 (12.12a) , 식 (12.12b）를 입력한다．
0 실제로 실행에 사용한 시간 영역의 전체 신호를 사용하지 않고 신호의 작은 구간 100개의 결과만을
咎펴본다．
0

37交

axis 명령어를 이용하여 100번째 시간값인 6.1875어］맞춰 축의 범위를조정한다.

PART 03. MATLAB 활용하기

n d a 幽 任 1 艮 曳 好自咽 而 니 島 ! 囹 匡引 匹 口

그림 12-27 기저대역 신호와 주파수 천이 변조 신호 그리71 실행 결과

반송파 무작위 신호 생성을 사용했기 때문에 DigiFsk.m을 실행할 때마다 신호 형태가 다르거］나온다．
심벌 0에 대한부분은 반송주파수兀을 가진 정현파 형태로 변조되고, 심벌 1어｝ 대한부분은 반송주파
수人을 가진 정현파 형태로 변조된다．

녑

=.
겨S.
if d_d(i)
뇨tC1 川）＋小（I-i) ) = (sqrt (2士Eb)／台qrt (Tb)）士cos (2士p1士tl,.t (1:Nfl;
1．

3 4 5 6 7 8 g m
H

무tsr

(b)

1 D呼FskSpecm ；晦 降斟
1Ns =l05; Tb =1; Eb=1;
2 t0 = 4/Tb; Ii = 2/Tb; Is = 4.10; N = ta/Tb;
t = 0:l/ ts:Ns*Tb;
d_d = round(rand(1, Na) );
b_t = zeros(1, length(t) ); s_t = zeros(1, length(t) );
1
나
11 ==

else
已t ( (l 洲）+H士（i나）) = (sqrt (2=Eb)/sqrt (Tb) )*cos (2士口1士to. .t (1 卞）) ;
尸．
nd

121314IS 1617l 卞
19-

end
ri = 2 (nextpow2(lenrith(b_t) fl ; Q
dl = ta/n; I = (0:dt:dt*(n-l) ) -ts/2;
오F : ttt (s..t, 5)／佯 10
semi Iagy(t. tltshitt (abs(S..F) )); O
asis()0 S le-4 183) );
비abel ( 下r日quence ) ;
title ( 小佃巾ilated FSK S口act rum 引ariaI ) ;

그림 12-28 주퍄수 천이 변조 신호 스펙트럼 그리기 코딩 결과（D甘氏kSpec.m)

0

for문을이용하여 식 (12.12a) , 식 (12.12b）를 입력한다．

0 nextpow2 함수를 이용하여 2. 'P > abs (length(b_t力의 조건을 만족하는／꾀 값을구하고, 2의
P승을 계산한다．
0

俄 함수를 이용하여 St어］대한푸리에 변환을 계산한다．

0

semulogy 명령어를 이용하여 y축을 로그함수로 지정하여 그린다．

CHAPTER 12; 통신

373

Re

E出t

\／治w

口心 님 鈿

1flSt

自

'\

,

Too虹

m喇빠） ＼庠in4o나

\ 仰 自 堤 I二 ' 目

He巾

［그 目

曾口

M汕出1ted FSK spectrum 덟goal

10 '

0

1

2

3

4

5

6

7

8

Fr以和ency

그림 12-29 주파수 천이 변조 신호 스펙트럼 그리71 실행 결과

蔓 2진 위상 천이 변조
2진 위상 천이 변조（BPSK: Binary Phase Sh玭 Keying）에서 부호 1은 0" 위상을，0은 180" 위상 변화
를 주어 전송함으로써 서로 구별된다. 그러므로 전송 신호어］따라 신호의 극성이 결정된다. 2진 위상 천이
변조에서 심벌 1과0을나타내는 신호幻m와SMt)는다음과같이 나타낸다.

小片小fat)

(12.13a)

小片cos(2r如1片小fat)

(12.13b)

여기서 0 5t< 乙이고, 尻는 비트당 전송된 신호 에너지, 兀는 반송 주파수를 나타낸다. 정현파의 한 쌍
이 상대적으로 180" 위상 천이를갖는 것을 정반대 (antipodal) 신호라고 한다．

! 예제 12- 14 1

M-Fde 1 DigiPsk'm, DigiPskSpec.m

(a) 위상 천이 변조를 이용하여 심벌이 i05개인 디지털 데이터를 연속으로 전송하려고 한다, 디지털 데이터
는 무작위로 동일한 확률을 가진 0과 l을 생성한다. 그리고 전송되는 데이터의 심벌 기간 Tb = 1[se이，

三이다·

兀＝

비트당 전송된 신호 에너지 Eb =1[W/bit］로 가정하며, 데이터를 변조하는 데 사용하는 반송 주파수는

이때기저대역신호와위상천이변조된디지털신호를나타내라．

(b) 위상 천이 변조를 사용하여 변조된 신호의 스펙트럼을 나타내라.

374

PART03. M月ILAB활용하71

圄

7- 日for i = 1:Nn e

8910ii 12 1314 15 16I? 1819-

it d...d(l)
b_t ( (1:N)*N.( i니) ) = 1 ;
end
나 end

2! 23 23-

anin( (0 12. 4 -1.6 1 ,61) ;
nIabeI ( '嫩t{ t} (nec) ') ;
title( 겨ad이 ated PSK 引 gnal ) ;

bt寸1t*2-1 ; 0
n...t = b_t.,(nqrt (2.Eb) /nqrt (Tb) )..cos(2=pi.tc, ,t) ; 0
subplot (211)
plot (t (1 :1133), b. .t (1 :113그) ) 0
axis(10 12. 4 -1. 1 1 川) ;
nIabeI ( 斗bHt} (nec) ') ;
title( 'Basebanddigital signal ') ;
nubplot (212)

20-

plot (t (1 :lm), s. .t(1 :1m)) O

그림 12-30 기저대역 신호와 위상 천이 변조 신호 그리:7 ' 코딩 결과（D甘內km)

0 심벌 수와 심벌 기간을 지정하고 반송 주파수를 입력한다．
0 샘플링 주파수와 심벌 하나어］대한 샘플의 수를 나타낸다．
0 무작위로 디지털 데이터 0과 1을 생성하고, 시간축의 샘플 수만큼 기저대역 신호를 0으로 지정한다．
0 for문과汪문을 이용하여 심벌 수를 지정한다．
0 기저대뼉 신호 l과-1을생성한다．
0 식 (12.13a), 식 (12.13b）를입력한다．
0 무작위로 생성한 디지털 데이터를 그림 창 위쪽에 그래프로 나타낸다．
0 위상천이 변조 결과를 그림 창 아래쪽에 그래프로 나타낸다．
Ale

帥C

VIew Ii甘rn Tools

r乂出햐｝ 獅hd1汁

거

He巾
[:} 園 咽 口

:J 亡｝ a 曲 ! b 1 （曳 曳 抑 自 咽 4 , 目

Baseb司ldd甘tel olgn川
0.5
0
.0.5
-1

1
6
8
t（的티
比d岫始dPSKs目nal

1

11

I I
2

1
4

6
t (sic)

10

'/I

12

1

'p

1

2

I

0

-1

]

D呼Pskm 挺 [ + 1
Sn : 1了5; Tb ! 1 ; 日미 ; <
21c =2/Th;
3to = 小允； N = tn/Tb; 0
4-.
t = 0:1/tn：卜怡＋Tb;
5d_d = rotjnd(rand(I, No) ); 0
6b. .t = zeros(1, length(tfl;

그림 12-31 기저대역 신호와 위상 천이 변조 신호 그리71 실행 결과

CHAPTER 12. 통신

375

rand 함수가 무작위로 신호를 생성하므로 D增Psk.m을 실행할 때마다 신호 형태가 다르커1 나온다. 심
벌 0에 대한부분은 반송파가 180' 위상 천이를 가진 정현파 형태로 변조되고 ，심벌 1어］ 대한부분은 반

(b)

송파와 같은 정현파 형태로 변조된다．

ifo呵PsbSpec.m 町＋l
1-

卜匡 = 1了5; Tb = 1 ; 日＝1 ;

2-

3 4 5 67 B gm n促 日 H 沔 比n 沼 円 게 기

Ic = 2/Tb;
is = 4.fc; N = is/Tb;
t = O:l/ is:Ns*Tb;
d...d = round(rand(1. Ns));
b_t = zerosCi. length(t) );

-

尸기 1 m나

!

1

1 .L1= 小

4

it 工d(I)
b_t ((l :N).N士（1니 )) = 1 ;
end
end
노t=b-t士2니 ;
乞t = 뇨t ..(sqrt (2.日2) /50rt ( Tb)) . 士cos(2士p1士Ic．士t) ;
n = 2 (nextpo.2(length(b_t))); 0
di = is/n;
f = (Q:df :d卜m니）) -l計2;
S.F = ttt (s_t, n)/fs; e
semi logy(I, fftshiit (abs(S. .F) )); O
8ci5(L0 4 le녀 Ie3] );
xl abe I ( Frequency ' );
title ( itoduluted PSI( spectrum signal ') ;
1
1
H
4
小
1
H
1
1
1
1
4

그림 12뇨-32 위상 천이 변조 신호 스펙트럼 그리71 코딩 결과（DiF뇽kS口ec.m)

0 的r문을 이용하여 심벌 수를 지정한다．
0 nextpow2 함수를 이용하여 2.午 戶 abs (length化t力의 조건을 만족하는P의 값을구하고2의 P
승을 계샨한다．
0 俄 함수를 이용하여 乞t어］대한푸리에 변환을 계산한다．
0 abs 명령어를 이용하여 y축상에 푸리어］ 변환된 町F의 절댓값을 구하고， fftshift 함수를 이용하
여 이 스펙트럼의 0 주파수 성분을 이동하여 스펙트럼의 왼쪽과 오른쪽을 대칭으로 놓는다. 여기에
semilogy 명령어를 이용하여 y축을 로그함수로 지정하여 그린다．
F陀

Ed比

\Ed나

In肖et

To아5

Do攷幻p

쌔mnw

}＋叫P

1

三J (=} 너 由 ［뇽 土＼\ 抑 @ 咽 而 , 晏 ［그 匡1 目口
Mod먀帥ed PSK specrum S目nal

"

H

102

10j

0

0.5

I

1.5

2

2.5

3

35

Pro叩태icy

그림 12-33 위상 천이 변조 신호 스펙트럼 그리기 실행 결과

376

PAAT03. M사LAB활용하71

1i
4

I

직교 위상 천이 변조

디지털 통신 시스템의 설계에서 중요한 목표는 오류가 적은 신뢰할 만한 통신을 제공하고 채널 대역폭을
효과적으로 이용하는 것이다. 직교 위상 천이 변조（QPSK: Quadrature Phase Sh血 Keying）는 신호
간격 T 동안어］대역폭의 확장 없이 2개의 비트를 동시에 전송하끼 때문어］비트율（bit rate)이 두 배가 된
다. 단일 비트 스트림 m으로부터 짝수 비트 ml과홀수 비트 加2로 표시되어 전송된 비트는분리된다．
두 비트를 서로 혼합하여 동시어］ 전송된 2개의 정규 직교佃rthonormal) 기저 함수는 다음과 긷K기 나타

(2

毗t)

+s

05t ＜乙

寸三sin
(2：

仍（/

)＝

'4Tb

自（/

):

낸다．

刃） .」t ＜乙

직교 위상 천이 변조로 전송된 신호는 다음과 같다．
s1(t) = s1自(t) + SE2砂2(t)

(12.15)

i = 1, 2

2진 위상 천이 변조의 위상차는 180"이고, 직교 위상 천이 변조의 위상차는 90"이므로 직교 위상 천이 변
조를 千위상 천이 변조라고 한다．

M-File

1 예제 12- 15 1

Digiopsk.m

직교 위상 천이 변조를 이용하여 심벌 수가 i05인 디지털 데이터를 연속으로 전송하려고 한다. 디지털 데이
터는 무작위로 동일한 확률을 가진 0과 l을 생성한다. 전송되는 데이터의 심벌 기간 Tb = 1{sec］이고, 데이터

를변조O는데＼용하는반송주파수兀북

이다．

(2硫t）를반

71저대역동위상신호에는sin

그리고;

［Hz］

송파로 사용하고, 기저대역 직교 신호에는 cos(mfat)를 뱐송파로 사용한다. 이때 직교 위상 천이 변조로 변
조된 각각의 동위상, 직교, 전송된 디지털 신호를 나타내라.

CHAPTER 12; 통신

377

剖

D也53小km }t + !
1No = 10'5; Tb = 1 ; Ic = 2/Tb; Is = 4* fc; N = is/Tb; <1
2t = O:I/ is:Ns,Tb;
3d_d = round(rand(l, Ns) ); 0
4d_I = d_d(1:2: Iength(d_d) ); d. Q = d_d(2:2: Iength(Ldfl;

b_I = zeros(1, Iength(tfl; b_Q = zeros(I, Iength(t)); e
1
H
H
m
m
4
e
1

!;::：三：

::'

b니 = 뇨1*2너 ; 뇨a = L小2너 ; 0
s_I = b_I .*(sqrt (2)/sqrt (化）) .＋引n(冬이＋Ic．吐）;
5꾜 = 뇨O.+(sqrt (2)/sqrt (Tb) )．叱四俚叩汁fc..t) ;
s_t=0_ 1=0_U;
subplot (311)
中
U

0

m
=
e

plot(t(1: IOO), s_I(I :l凹)) e
m

aols(10 12. 4 -1.6 1.61) ;
title( Modulated PSK signal : In-phase) ;
subplot ( 31 2)
이ot (t (l :113九 s_Q(1:1m) ) O
asis(10 12. 4 -1. 6 1 .61) ;
t汁 Ie( ‘卜伯dulated PSK 引gnal : 山ad rat u re ) ;
subp lot ( 31 3)
U
느
e
느
m
4
1

plot (t (1 :l몌),s_t (1:lw)) O
小

asis(I0 12. 4 -1.6 1 . 61) ;
title ( Madulated3PSK 引grial ) ;
H

6 7 B 9 m H 吃 沼 m 巧陌 口 田 円 m 기 끄 招 m 즈 而 까 田 四

5-

그림 12-34 위상 천이 변조 그리71 코딩 결과（DigK3psk.m)

0 주어진 배개변수를 지정한다．
0 동일한 확률을 가진 원래의 기저대뼉 뎨이터 1과0을 생성한다. 데이터를 동위상 변조와 직교 위상 변조
를 위한2개의 분리된 스트림으로 나눈다．
0 시간축의 샘플 수만큼동위상 기저때뼉 신호와 직교 위상 기저때뼉 신호를 0으로 지정한다．
0 for문과 if문을 이용하여 동위상 기저대역 신호와 직교 위상 기저때뼉 신호를 지정한다．
0 동위상 기저대역 신호 1과 직교 위상 기저대뼉 신호 크을 생성한다．
0 식 (12.14a), 식 (12.14b), 식 (12.15）를입력한다．
0 위상 천이 변조로 변조된 동위상 신호률 그림 창 위에 그래프로 나타낸다.
0 위상 천이 변조로 변조된 직교 위상 신호를 그림 창 가운뎨에 그래프로 나타낸다．
0 직교 위상 천이 변조 결과를 그림 창 아래에 그래프로 나타낸다．

378

PART03. M月兀AB활용하71

File

Ed注

View

j 니j d ;J

Inswt

臣

TOds

'\

Des岫DP

빠inow 卜螂p

\ {n7 自 啞 d , 晷 ［그 듣크 . 口
Modul카ed PSK 덟gnal: In.pha羽

/V \

1

f

2

VV/

\/\\./V\

\W\

0

1\

V

0
1

4
6
8
10
ModuF帥ed PSK signa': Quadrature

2

4
6
8
M어札h帥日dQPSK 미了nd

2

4

12

10

12

10

12

1
누

}
6

8

그립 12-35 위상 천이 변조 그리기 실행 결과

rand 함수가 무작위로 신호를 생성하므로 DigiQpsk.m을 실행할 때마다 신호 형태가 다르거1 나온다. 2진
데이터를 독립된 동위상 신호와 직교 위상 신호로 분리하고 서로 90"의 위상차를 가진 두 반송파를 동위상
신호와 직교 위상 신호의 2진 데이터로 진폭 변조한후 합성하여 전송한다．

I 卜十직교 진폭 변조
M-직교 진폭 변조（M-quadrature an巾血ude modulation）는 진폭과 위상을 모두 고려하여 서로 다른
심벌을 구별해서 전송하며, 각칵의 심벌은k비트를 이용하여 변조한다. 비트 k와 단꼐 Il／의 관계는 다음
과같다．
(12.16)

k= log2M

예를 들어 16직교 진폭 변조 시스템에서는 4비트를 이용하여 변조하므로 직교 진폭 변조 심벌은 각칵의
신호 간격어］대해 4비트를 동시어］전송한다. 그러므로 가능한 신호점 (constell犯on）은 16개이다．
M느직교 진폭 변조로 전송된 신호는 다음과같다．
욱（t) =Sn自（1) + si2砂2(1)

江1, 2, ···,M

(12.17)

여기서 기저 함수 吻(1)와仍(1)는 직교한다．

CHAPTER 12. 통신

379

1 예제 12- 16, 1

M-File I 미이Mqam.m

64-직교 진폭 변조를 이용하여 심벌 수가 i04 x k인 디지털 데이터를 연속으로 전송하려고 한다. 직교 진폭

；而

변조로 변조된 신호에 대한 산점도와 아이 다이어그램을 나타내라．

지식

'

reshape

원래 배열A를이용하여새로운nX刃7크기의배열B를생성하는reshape명령어의 기본형태는다음과같다．

B = reshape(A, n, m)
· B: 刃 >Km 크7厚 변환된 배열
· A: 원래 배열
·n, m: 새롭게 지정할 배열의 크71

口 bi2de
2진 벡터 B를 10진수 D로 바꾸고msbflag로 입력 방향을 결정하는bi2de 명령어의 기본형태는 다음과같다．

D = bi2de(B, msbflag)
· D: 변환된 ]0진수
·B: 2진 벡터
·msb加g: 입력 방향

msbflag는 'right-msb'와 'left-msb' 중 하나를 사용한다. 2진 입력의 디폴트 방향은 'righ卜msb'로 2진 벡
터 B 의 첫 번째 원소는 최하위 비트(least significant bit）를 나타내고, 'left-msb'로 지정되면 최상위 비트
(most significant bit）가 입력 방향의 왼쪽에 위치하므로 'right-msb'와는 반대 위치가 된다．
1modulate
변조하려는 배열 x에 다양한 디지털 변조 방법 Method를 사용하여 변조된 신호 V를 생성하는 modulate
함수의 기본 형태는 다음과 같다．

Y = modu怡te(Method, X)
. Y: 변조된 신호
·Method: 디지털 변조 방법
. X: 변조하려는 배열

380

PART 03. M月ILAB 활용하:7 '

1modem.qammod
M-직교 진폭 변조에 대한 변조기를 생성하는 mod印l.qanimod 명령어의 기본 형태는 다음과 같다．

modem.qammod(M)

nscatterplot
산점도（scatter plot)는 두 변수 간의 함수 관계를 나타내는 2차원 그래프로 두 변수의 관계를 시각적으로
표현한다. 배열 x의 산점도를 생성하는 scatteq加t 명령어의 기본 형태는 다음과 같다．

scatterp幻t(X)

1eyediagram
배열 x의 아이 다이어그램 (eye dia얗am)을생성하는eyediagram 명령어의 기본 형태는 다음과 같다．

eyediagram(X)

0-

7-

6-

5-

4-

3-

1 D呵Mq目mm J느
1N=64; 1
k=log2(H) ;
2-

9-

系i

:：二！
,:::；悤뇨，. ,,.,<)

三！
，釜；pe(ed(
te(三：
，二，
::：芬，
읍·，),;．會；
O
::：据’
，點’
．品

그림 12-36 변조 신호의 산점도와 아이 다이어그램 그리기 코딩 결과（D呼Mqam.m)

0 변조의 단계 A／에 64를 지정하고, 심벌당 비트 수를 계산한다．
0 전송되는 비트 수를 지정한다．
0 전송 뎨이터 也d를 지정한다．
0 전송데이터 d1d의 크기는 1 x60000이지만, reshape 명령어를 이용하여 k= 6비트를새로운 배열의 행
수로 지정하고 可互 = 10000을 새로운 배열의 열 수로 지정하면 새로운 배열 d d4의 크기는 6 x 10000
이 된다．
0 데이터 d1d4의 6개 비트를 전치한후 0과 15 사이의 10진수로 변환한다．
0 modulate 함수를 이용하여 직교 진폭 변조된 신호를 생성한다.
0 변조된 신호로 산점도를 그린다．
0 변조된 신호로 아이 다이어그램을 그린다．

CHAPTER 12. 통신

381

디陌

Ed仕

너e나

a J d ;1

Irwelt

E

Too匕

H베）

1

' \ , 」r『7 @ +? 戶＝ · 昆 口 目

Deskto口

쌔totow

m 口1

Scatter 아아

4
-4

2
0
쿄
뽄크m듬m= O
七
七

-4

寸2

0

2

4

6

In-Pha羽

그림 ]2叫37 변조 신호의 산점도 그리기 실행 결과

디le

EdO

Vi싸

J1 d 코
10

Ins미t

妊

初이5

'\

D吐t야） 硼ndow

' @ + 而 , a』 口 트그 쓰 口

Eye Dagrorrr for 小Phase Spgnal

5
0

쁨귿aE <

巧
-10
七S

0

0.5

Trne
日忙 댜甲amfoiQu刈rature S甘뇌
5
0

8쿄죤눈

七
0.5
T0Thste

그림 12-38 변조 신호의 아이 다이어그램 그리기 실행 결과

382

PA日T03. MATLAB촬용하71

이mulink

설계하기

CONTENTS
PART 04에서는 口，

口

CHAPTER 13 시뮴레이션을 위한 시뮬링크
' 다양한 블록을 이용하면 시뮬레이션이 가능해요"
CHAPTER 14 「．미분방정식
'복잡한 수식을 한 번에 줄여나가요"
CHAPTER 15 } 삼각함수
' 기하해석을 위해 필요하군요"
CHAPTER 16 ,!제어
'제어 시스템의 분석 및 설계를 체계적으로 도오F줘요"
CHAPTER 17 ;신호 및 시스템1
'신호 처리 및 분석 수행을 시각적으로 볼 수 있어요"
CHAPTER

벡터
“크기와 방향을 블록으로 이해해요"

CHAPTER 19 目퓽신
' 시뮬레이션을 통하1 통신 시스템을 검증할 수 있어요"
CHAPTER 20 i 회로
'복잡하1 보이는 회로 설계를 쉽게 접근하네요"

PART 04에서는
무엇을 배울까？

\
Simulink 설계하71
：小4ATLAB의 시휼링크는 다중 영역 시뮬레이션 및 모델 기반 설계를 위한 블록 선
: 도 환경을 제공한다. 시뮬링크를 이용하면 실제 구축하는 시스템을 모델링하여 광
범위한 설계 공간을 미리 탐구할 수 있다. 또한 하나의 시뮬링크 설계 창에 다중 도
: 메인 환경을사용하여 시스템의 각부분이 어떻게 작동하는지 시뮬레이션할수 있다．
13장에서는 기본 블록부터 블록을 이용하여 모델을 설계하는 방법, 시뮬레이션 결
과를그래프로나타내는기본방법과다양한응용예제를살펴본다．
미분방정식은 하나 이상의 독립변수（입력변쉬에 상응하는 하나 이상의 종속변수
1 （출력변쉬의 도함수또는 미분을포함하는 방청식을말한다. 14장에서는다양한 1차
미분방정식과2차 미분방정식 모델을 설계하고살펴본다．
15장에서는 사인 파형의 기본을 이해하고 사인 함수와 코사인 함수의 관계를 설계 三
, 하여 두함수사이의 유사점과상이점을알아본다.
16장에서는 9장과 유사한 내용을 다루지만 시뮬링크를 이용하여 제어 시스템 모델
: 을 설계하고 그 결과를 비교 ·분석한다. 또한9장에서 다루지 않았던 다양한 제어기
; 를 설계하고 그 결과를 비교 . 분석한다．
17장어써는 시뮬링크를 이용하여 신호 및 시스템 모델을 설계하고, 주파수를 7] 注
로 하는 시스템 모델도 함꺼］ 설계하여 그 결과를 비교 . 분석한다．
18장에서는 벡터 및 행렬의 연산, 벡터의 활용을 위한 시뮬링크 모델을 설계하고 그
결과를 알아본다．
19장에서는 시뮬링크를 이용하여 통신 시스템 모델을 설계하고 그 결과를 비교 ·분
석한다. 또한통신의 기초가되는확률 및 확률변수의 개념을 이해하는시뮬링크모
: 델을설계한다．
20장에서는 시뮬링크 모델을 통해1 저항, 전류, 전압의 상호 연관성을 알아본다. 또
한다양한 기능을수행하는 연산증폭기 모델을 설계하고 그 결과를분석한다．

/

CHAPTER 1

13

d心쩍

小
r
出
m
m

m
茗
兵

m孔幷打玉薑茹發薑薑薑i巫小

0茗月好貿

시뷸坰션을위한
시뮬링크

CONTENTS
LESSON 01 시뮬링크 실행하:7 '
LESSON 02 기본 블록을 활용하여 설계하기
LESSON 03 그림 창에 결과 나타내기
LESSON 04 사칙연산 활용 및］차 함수 입출력 그래프 설계하기
LESSON 05 복소수 활용하71

LESSON

01

시뮬링크 실행하기

시뮬레이션을 해볼 수 있는 시뮬링크를 실행하는 방법을 알아보자．
Keyword

I

I 시뮬링크 1 시뮬링크라이브러리 브라우저 1 설계 창 1 블록 1

시뮬링크의 개요

시뮬링크（Simulink）를 이용하면 직접 동적 시스템의 시뮬레이션을 실행해볼 수 있다. 시뮬레이션을 실
행하기 위해 블록伯lock）이라는 다양한 시스템 원소의 유형을 직접 생성하커나, 시뮬링크에서 제공하는
블록 라이브러리 세트를 이용하여 블록을 설계한다. 각블록을삽입한후 블록의 재배치, 크기 조절, 매개
변수 지정을 하고 각 블록을 서로 연결하여 전체 시스템을 구축한다．
口d} r저1대로 배우는 MAT나＼BJ 초굔k게서 사용한 MAT나＼B 2010b 버전의 시뮬링크 확장자는 .mid였으나 이 책에서 사용하는 MAT녀B
2015b 버전의 시뮬링크 확징자는 .S以이다. 일반적으로 상위 버전에서 생성된 파일은 하위 버전에서는 사용하지 못하지만, 하위 버
전에서 생성된 파일은 상위 버전에서도 사용할 수 있다. 예를 들어 2015b 버전에서 설계한 시뮬링크 파일 'fiiel5.引x'는 2010b 버전
의 시뮬링크에서는 사용할 수 없다. 반면 2010b 버전에서 설계한 시뮬링크 파일 '꿰elO.mid'는 2015b 버전의 시뮬링크를 실행하여
불러온 후 꿰elO.엷x'로 시俚 저장하면 사용하는 데 문저까 없다．

I

시뮬링크 시작하기

시뮬링크를 시작하기 위해 명령 창 [HOME］에서 圈Simulink 라이브러리 버튼을 클릭한다. 또는 시뮬
링크를 시작하기 위해 MATLAB 명령 창어］다음과 긷히 입력한다．
>> simulink
그러면 시뮬링크 라이브러리 브라우저가 열리고 시뮬링크를 사용할수 있다．

I

시뮬링크 화면 구성

시뮬링크아는시뮬링크 라이브러리 브라우저, 설계 창등히 사용되는데 이를간략히 살펴보자．

시뮬링크 라이브러리 브라우저
시뮬링크 라이브러리 브라우저 (Simulink Library Browser）는 시뮬링크를 시작함과 동시어］ 나타나는
창으로, 시뮬링크에서 사용하는블록을 라이브러리별로 모아둔 것이다. 대표적인 구성 요소의 명칭과 기
능은다음과같다．
386

PART 04. Sim메nk설계하71

0 이동 화살：시뮬링크 라이브러리 브라우저의 실행 이전 및 이후화면으로 이동한다．
日 검색 상자： 검색어를 입력하여 원하는 블록을 찾을 수 있다．
日 검색 블록 선택 버튼：검색 상자어］입력해서 찾는블록의 선택을 지정한다．
口 설계 창 생성：시뮬링크 설계를 위한 새 설계 창과 이미 작성된 설계 창을 열 수 있다．
日 라이브러리 창： 기본 시뮬링크 설꼐를 위한 라이브러리와 응용 라이브러리가 알파벳순으로 나열되어
있다．
日 볼록 목록 창： 사용하려는 라이브러리의 이름을 클릭하면 해당 라이브러리가 제공하는 블록이 알파벳
순으로 나열되거나 검색 결과가 나열된다.

갸告蜀쀼擢生泂
Dashboard
미scontinuiti日S
미screte
Lo미c and 미t Ooers如ns
Lodku Tables
Math ODeratlons
M이｝미 Verlfic冽on
M미相卜Wide U씨出es
Ports & Subsvs伯n怡
미on쉬 씨bibufee
$！亘n쉬 日Cu甘ng

I型
I 」藝
I 貫
L發
卜妥
I蟹
I 豪
I努
口卦
I ：甘
I 크

口口Db

Sources
匡i1
User-Defined Functions
1 甘
r Mditlon히 Math & 미scr貳e
I쳐
如rosoace 미ockset
卜斗
Comniunications System Toolbox
1
Communications Sistem Toolbox 卜 I
Comsu泊r 너引on 帥＄相m Toolbox ! i1
I 曾
Contiol Svs伯mT的七ox
Data Ac口U忖卜don To미box
I烈
I ！君
DSP System Too出ox
DSP S岫相m To미box HDL Suooort 巍
bEmbedded Coder
"
！蟹
x Fuzzy Lo미c Toolbox
!烈
b I1DLCoder
I 哲
山
Image Acq낸이tion I口0由ox
Instrument Con打미 Too由ox
Model Predictive Control Toolbox
> Neural Network Toolbox
bD

b

卒

-

丙

日us
Creator

'
Bus
Selector

Cons伯nt

Data Type Conversion

恒：}

{>

巨｝

I
mnl

미＄crete＝기me
Integrator

Ground

닉j}

Integrator

+

齬齬譜甘미 Too巾ox

> 미mRF

之 熬湍隔 Anim州on
4 '- TT-

,

if 1

>1

日 4 미mulirik
엷需얹났sed Block'

Gain

횬｝
Lo미c궤
Operator

Moo
N

i

Nr

1

그림 仍너 시뮬링크 라이브러리 브라우저

설계 창
설계 창（S岫ulink Editor）은블록 다이어그램을 그리는 데 쓰인다. 설계 창을 열려면 區크에서 화살표룔
스크롤다운하여 [New Model] 버튼을클릭한다. 대표적인 구성 요소의 명칭과 기능은다음과같다．
0 메뉴 표시줄：설계 창에서 사용하는 명령어가 메뉴별로 구분되어 있다．
日 도구 모음：많이 사용되는 메뉴를 아이콘 형태로 보여준다．
日 저목표시줄：설계창의이름을보여준다．
口 입력 부분：블록을삽입하여 모델을구성한다．

CHAPTER 13; 시뮬레이션을 위한시뮬링크

387

0 F沁 Ed仕 V9ew D唎啣 r汁好曲t stl'卄出Ith口C 如텍麟； 口巾 自味I ii뱌1
鸚 心 , 昏 니t始 4夕 b, 小 口 匹 , 而万
日 昆! 圄
1
日 untitled
回untitled

叫

》》(9 ! 幽 ,

二口
a

回
［回
［그
Et

幽
100%

Ready

吻eia比鈿pA北a

그림 13-2 설계 창

또는 블록 목록 창에서 처음 설계 창어］ 그리는 블록을 마우스 왼쪽 버튼으로 선택한 후 마우스 오른쪽 버
튼을 눌러 [Add block to a new model] 메뉴를 선택하면 ［그림 13-2］와 동일한 설계 창어］ 최초로
선택한 블록이 그려진다．

I

블록 삽입하'I

시뮬링크를 사용할 때는 설계 창어］다양한 블록을 삽입하여 수식을 설꼐한다. 블록을 삽입하는 방법은 여
러 가지이므로 사용자의 편의에 따라 방법을 선택한다．

블록 이름과 뷸록이 속한 라이브러리의 이름을 모두 아는 경우
0 시뮬링크 라이브러리 브라우저의 왼쪽 화면에 위치한 라이브러리 창에서 삽입하려는 블록이 속한 라
이브러리를 클릭하여 라이브러리를 연다．
日 블록 목록 창어］나타난블록 중 삽입할블록을 짖아 클릭한다．
日 다음 세 가지 방법 중 하나를 택하여 실행한다．
· 선택한블록 위에서 마우스 오른쪽 버튼을 눌러 [Add block to model （설계 창 이름）] 메뉴를 선
택한다. 아직 설계 창을 열지 않았다면 [Add block to a n巴w model] 메뉴를 선택한다．
· 선택한 블록을 설계 창에 삽입하기 위해 匣刃 +［끄 키를 누른다．
· 선택한 블록을 설계 창으로 드래그 앤드 드롭한다．
블록 이름만 알고 블록이 속한 라이브러리의 이름을 모르는 경우
0 검색 상자에 블록 이름을 입력하고 匡回 키를 누르거나 A ［찾키 ] 버튼을 클릭한다．
日 검색 결과가 나타난 블록 목록 창에서 삽입할블록을 짖아클릭한다．
日 다음 세 가지 방법 중 하나를 택하여 실행한다．

388

PART 04. 針nulink 설계하71

· 선택한 블록 위에서 마우스 오른쪽 버튼을 눌러 [Add block to model （설계 창 이름）] 메뉴를 선
택한다. 아직 설계 창을 열지 않았다면 [Add block to a new model] 메뉴를 선택한다．
· 선택한블록을 설계 창에 삽입하기 위해 匣刃 + 回 키를누른다．
· 선택한블록을 설계 창으로 드래그 앤드 드롭한다．
블록을 복제하는 경우
다음 세 가지 방법 중 하나를 택하여 실행한다．
· 설계 창에 삽입된 블록을 선택하고 마우스 오른쪽 버튼을 눌러 [Copy] 메뉴를 선택한 후, 설꼐 창
의 빈 공간에서 마우스 오른쪽 버튼을 눌러 [Paste] 메뉴를 선택한다．
· 설계 츠뇌］삽입된 블록을 선택하고匣刃 +［희 키를눌러 블록을복사한후, 설계 창의 빈 공간에서 마
우스 오른쪽 버튼을클릭하고［西그 +［피 키를 눌러 블록올붙여넣는다．
· 설계 창에 삽입된 블록을 선택하고匣刃 키를 누른 채 드래그 앤드 드롭한다．

CHAPTER 13. 사므레이션을위한시묠링크

389

LESSON

02

기본 뷸록을 활용하여 설계하기

시뮬링크의 블록을 이용하여 덧셈, 뺄셈을 계산하는 Sum 블록과 신호 형태로 결과를 나타내는 Sc야兀 블록의 기능을 알아보
자. 그리고 사인 파형과 코사인 파형을 출력하는 Si陀 Wave 블록과 Co帥e Wave 블록. 적분을 계산하는 Integrator 블록의
기능도 살펴보자．
I Sum블록 I Scope블록 I Sine Wave블록 I Cosine Wave블록 I Integrator볼록 1

Keys사ord

亘 Sum 블록
Sum 블록을 이용하면 상수, 벡터, 행렬 형태의 입력을 서로 더하거나 뺄 수 있다. 즉 Sum 블록의 부호
매개변수를 + 또는

I

로 설정하여 덧셈 또는 뺄셈 연산을 할 수 있다．

Sco口e 블록

Scope 블록을 이용하면 설계된 시스템의 시뮬레이션 결과를 신호 형태로 나타낼 수 있다．

! 예저h ia- i I
시뮬링크를 이용하여 수식 z＝工hy를 설계하라. 또한工 = 5, y= 2일 때 수식의 결과를 그래프로 나타내라．
푤이

0 Cons恤it 블록2개를 설계 창에 생성한다（[Commonly Used 미ocks]-[Constantj).
ElD
F4뇨

日It

Constant 블록을 이용弓H브 상수를 입력할 수 있다．
V卜曲

대5加y

曷r目

Dm{Fam

듸mU1ad머1

사니b디5

Co1므

b：
片5

1+H口

.！느 $ , 團 , 呻 出 U 恥＞ 」 쓰 ! Iuo

,, 寸 r 管自 !

Un寸ded
的 回unVied

!

탁
目
二＝

回
i回
口

LiI

it
毖
力
Rm句

그림 13中3 Constant 블록 생성

390

PART 04. Sim메nk 설계하71

100%

山油k曲畔1廂＝

OSum 블록을 설계 창에 생성한다（[Commonly Used Bloc畑卜田urn]).
O Scope 블록을 설계 창에 생성한다（[Si川心］-[Scope]).
F겪브

E固L

VkW

r거5F甘ay ［거a亭am

囹! =

듸m이誨on

鵠 每!

Analy引5

Code

bc引S

" 呻 텍1 也／ 作

He巾

回 ,,, 口 , 蟲 ,

Unt刈ed
!

團unti如d

e

面
1a
=5

E回

D

回
［그

X돛＞

네므，

[가

】 如11

［三

幽
>>
Ready

l凹％

＼屈iableStepAuto

그림 13닉 필요한블록 생성

0 Constant 블록을 더블클릭하여 [Source Block Parameters] 창을 열고 [Cons切nt value:］를 5（工 = 5)
로 바꾼 후 回K] 버튼을클릭한다．
Constant
Output the Constant specified by the 'Constant value' parameter. If
'C口nstant v톄ue' is a vectc甘 and Interpret vect口r 口arameters as 卜［) ' 冶
on』打eat the cons伯nt va山a as a卜 ［) array. 아herwise, 1기it口ut a ma卄ix
咐If, the sam日 山Sen덟ons as the c口nstant V궤u已
Main m$ dJ乙蚣b'！磊J,＝日
C口nst日nt va山a.
5
國 In也rpretve아or 口aram日t마s as ] 山
Sample time:
1ni

J

OK

Cancel

H日巾

AnP坦

그림 13巧 Constant 블록에 상수 지정

0 Constant! 블록을 더블클릭하여 [Source 미ock Parameters] 창을 열고 Constanti의 [Constant
value:］를2(y= 2）로 바꾼후 回싸 버튼을클릭한다．
0Sum 블록을 더블클릭하여 [Fun야幻n 미ock Parameters] 창을 열고 [L慨 of signs:］에 !+- 를 입력한
후 回K] 버튼을클릭한다．

CHAPTER 13 시뮬레이션을 위한시뮬링크

391

Sum
Add 口r 日ubtract inpu怡． Specify one of the 幻比M叩：
a) string c口nt비fling + or - 幻reach in口Ut 口ort, I 幻rspacer b비꿔een
p口rts (e.g. -I니 ++)
b) scalar. >= i. e口日c什1臼s the number of input p口rts to be summed.
m 日n 出日r日 冶 口nly 口ne in口Ut PU凡 add 口r subtract elements over all
비men引ons or one spec州ed 비men引（긔）
M눼n

SIgnal Attributes

Icon shape: round
Li澍 of 引gn5:

9

OK

Cancel

Help

Apply

그림 13田 Sum 블록에 부호 지정

0 블록에서 뾰족하게 나온 부분에 마우스 커서를 놓으면 커서가 십자 형태로 바뀐다. 이때 마우스 왼쪽 버
튼을누른 채 다음블록에서 뾰족하게 나온 부분에 정확하게 연결하면 화살표 선이 생성되고 블록이 연결
된다. 이러한방법으로Constant블록과Sum 블록, Sum 블록과Sc叩e 블록을 연결하면 블록의 설계가
완료된다．
블록을 회전시키려면 마우스 오른쪽 버튼을 눌러 [Rotate & 다p] 메뉴를 선택한다. 잘못 연결된 선을 제거하

1l1>

려면 제거할 선에서 마우스 오른쪽 버튼을 눌러 四Ut］나 [D이아e] 메뉴를 선택한다．
F沁

Ed作

Vie나 ［거splay

西｝！圄

O治字帥l

듸m너小向S

琵 好,

Arm卜疥is

Code b畔i

He巾

" 呻 똬 !8 m> . 쯔 中，, @

!

描

!

wit出ed
!

브희unt川ed

的

風
四
4

回

口

0
（뇨m山-

S口까七

圄
口
Et

團
>>
Rea旬

1凹%

VanableStepAuto :

그림 13-7 블록 연결

0 이제 시뮬레이션을 실행하여 스코프 창에 결과를 출력해보자 ．설계 창의 메뉴 표시줄에서 [Simulation]Er'如del Configuration Parameters] 메뉴를클릭하면 [Configuration Parameters] 창이 열린다．
0 [Solv町 아必ons］의 [S아ver:］에서 d始Crete (no cont血uous states）를 선택하고 回K] 버튼을클릭한다．

392

PART 04. Simulink 설계하71

미m내刮on Urn日

S日1日Ct:
S이四r
Deta Irrr口口可Er口0n
7 0口tar注aton

Start Urn日： GE

籌旨""""
:1HOLE口de Genera如n

S幻口 Urn日： lag

SobVer 미刈口n5
ly口a: Vanab岫帥日口

미陀

盆｛忿츄t二忿斗守，겅
口de45 (D먀m8n小Princ日）

卜 戶ddiUon비 口口的nS

염冒湖腱寫Sharn口bee)
謐醫畿楹 H四帥b耐）
ode2a (rood, at町Era口eZ미dab)
odeS긔0 (a毗／T下卜00F2)

그림 13田 새로운 시뮬레이션 매개변수 설정

四 [Simulatio미나Rui日메뉴를 선택하거나0[Run] 버튼을 직접 클릭하여 시뮬레이션을 실행한다．
Q Scope 블록을 더블클릭하면 실행 결과를 스코프 창어Pd 확인할수 있다．
A뇨

化야5

View

듸muLtion

IV目p

그림 ]3四 스코프 창 결과

e 스코프 창의 오른쪽 아래에서 마우스 왼쪽 버튼을 누르면 대각선 화살표가 나타난다. 화살표를 움직여 스
코프창의 크기를조정하면 최적화된 스케일의 그래프를볼수 있다．
El[l

시뮬레이션 실행 후 명령 창에 나타나는 경고 메시지는 무시해도 괜찮다. 이 경고 메시지가 보이지 않게 하려
면 囹m너ation]-[Mod이（力nfiguration Parameters] 메뉴를 선택한 후 [Configuration Parameters] 창에
서 [D峽nos抛S］를 클릭하여 [Au加matic solver parameter se冶에on:］을 none으로 지정힌따. 이때 계속
열려 있는 설계 칭을 사용하여 시뮬레이션을 실행하는 경우에는 경고 메시지가 계속 보이지 않지만. 설계 창을
새롭게 열어서 사용하는 경우에는 잎k게서 설명한 과정을 다시 설정해야만 경고 메시지가 보이지 않는다．

CHAPTER 13. 시뮬레이션을 위한시뮬링크

393

iSo泊Ct
S이四r
D日to In,口0,550口Dn

Soloat
川gebra匕 匕D口

油amhq

N叫mZ日 미gebno比 1口D口

唱
「畜轟：
드口nneCn나斗

,,.

曾

難寵．

擡醫醫쏀'"
' nclng

fr HOL Cod日 donoratl口n

toock 口H口r却 내口1ad口n

:

S.am。
。。

attn St日P 引？e 너II削On

namm

San,비日 ShIm, a비HInd:

non.

C口m日CmVe 2er0 Cm9引no드 너olatlor

error

tons口日C而日d ,ntattltabjl啣 口f 的mpl日 hm包 낵arnng
鈿h日rdata incon引引BnCy:

i 川）
e

atalmooc S이叩r 口arameter 5日1日clot
E000n日0UB 네oc tote 0日n\md妃 引gn미B
마日由 nam日 니日8h

11

的
照

SO기Smt日ntod000checkSuntntlono七h [
SO기Stat, objoct front ea세日rreea8甘

I. ,,口

Cart,叫

I

H이P

1

柚口坦

그림 13-10 경고 메시지 생략

m 匡如卜囹ave as] 메뉴를 클릭하고 'Siml(파일명）'을 시뮬링크의 확장자（.引x）가 붙은 'Simi.six'로 현
재 폴더어］저장한다. 저장한 설계 파일은 언제나 다시 사용할수 있다．
File

Ed作

\／治w ［站的y

舜, 圄

듸mulat幻n

鸚 好,

Anab5法

Cod甘

取病

H叫p

" 됴摯 <g 出7 昑 / E小片 U , 幽 ,

I
!

』；

回미ml

Simi

Diagram

侄크
自

E回

（油alant

口
S口耳）e

團
［그
Em
宙
Rmdy

l仗）%

그림 13-11 완성된 시뮬링크 모델（Siml.s以）
m}

出ia寸e또epoN口050
1

시뮬레이션 실행을 마친 후 설계 창 하단을 보면 ' \／咆w 1 warning 100%'라는 메시지가 있다. 이 메시지는
[File］놔［Save] 메뉴를 선택하여 파일을 저장하면 사라진다．

I Sine Wave 블록
Si'妃珉rave블록은 [Sources] 라이브러리에서 제공하며, 이를이용하면사인파형을출력할수있다. 이
블록 은 시간 의존척 형태나 표본 의존척 형태로 사용할수 있다．

i Cosine Wave 블록
Cosine 찌町e 블록은 [Sources] 라이브러리에서 제공하지 않는다. 따라서 코사인파의 위상이 사인파의
위상보다 90" 뒤처져 있는 성질을 이용하여 Sine Wave 블록어］ 兀／2 라디안 위상 오프셋을 설정하고 사용
한다．

394

PART 04. Sim메nk 설계하기

I 예제 13- 2 1
시뮬링크를 이용하여 다음 모델을 설계하고 시뮬레이션 결과를 스코프 창에 나타내라 ．이때1 시간은 0초부터
20초까지 변화한다．
(a) 진폭이 2인 사인 파형 모델
(b) 진폭이 2인 코火r인 파형 모델
(a) 다음과 같은순서로 설계한다．
0 Sine Wave 블록을 설계 창에 생성한다（[Source司-[Sine Wave]).
O Gain 블록을 설계 창에 생성한다（[Commonly Used Block司나G缸미）.
1l1} （珣n 뷸록을 이용하면 입력에 상수를 곱할 수 있댜．
0 생성된 Gain 블록을 더블클릭하여 [Fm毗幻n Block Parameters] 창을 열고 [Gai미을 2（사인 함수
의 진폭이 두 배로 증가）로 바꾼 후 回K] 버튼을클릭한다．
0 Scope 블록을 설계 창에 생성한다（[Sit止司-[Sc이刈）.
0 생성된 블록을 연결한다．
F晦

Ed仗 ＼기ew

D먀肋y ［거agram

區｝ r 圄

鸚

돠rnulation

Analysia

伽巾 iX站

" E摯 텍1 ＼브 且1> !

Help

쯔 ！》， 已） ! 幽 !

미m2
e

!

團돼m2

푿이

風
目
4

,:）士

'二？

"딜

回
i回
［그
E三
齒
力
Ready

10民

ode45

그림 13-12 완성된 Sine Wave 모델

0 설계 창 위어］ 있는 [Simulation]-[Model Configuration Parameters] 메뉴를 선택하면
[Coni砲uration Parameters] 창이 열린다. [Sta毗 ti毗］과 [St叩 time］에 각각 0.0. 20.0을 입력한
후 回K] 버튼을 클릭한다．
0 囹imulatio미-[Run] 메뉴를 선택하여 시뮬레이션을 실행한다．
0 Scope 블록을 더블클릭하면 스코프 창어써 실행 결과를확인할수 있다.

CHAPTER 13 시뮬레이션을 위한시뮬링크

395

F艇

Too놈

唾r

磻 G) q> 孕 率 , 目 , ［二 」 兮

\rimv

引dl祉前bn

Fk텍P

씌

月,

,

\/＼》，

／

『

0,5
/

．쇼5

Re如p

1=20；啣

그림 13-13 스코프 창 결과

0 스코프 창의 오른쪽 아래에서 마우스 왼쪽 버튼을 누르면 대각선 화살표가 나타난다. 화살표를 움직
여 스코프 창의 크기를 조정하면 최적화된 스케일의 그래프를 볼수 있다．

-

I

-

I 1L

It_

_

I I (3 +H

/ \

r

,'

-

I.

I

'

'I

0

I 0

-

I

r

-

1 1그

I

t二t_

_

l.

.

-

t

I

IH1

L二

I_

I

'=

\V/

-

(h）사인파와코사인피는위상오프셋챠이가즈．이다.' 이 특징을이용햐켜 다음과같은순서로설계한다．
'
1 2 I
0 ［그림 13-12］와동일한모델을구현한다．
'

II 1二

-

.'

0 생성된 Sine Wave 블록을 더블클릭하여 [Soe丁ce Block Parameters] 창을 열고 [Phase (rad) :]에
사인파와코사인파의 위상오프셋 차이인 pi尼를 입력한후 回K] 버튼을클릭한다．
1l1} Sine Wave 블록의 [Source 테ock Parameters] 창에서 사인파의 유형으로 시간 기본（기me based), 샘
플 기본（SamF兆 based) 중 하나를 선택할 수 있다．
텨n日 Wave
0u巾ate 늬fle wan日
0(t)

小텨rr)Freq너냐These) + 日las

미tte ty口日 dat日nnin日sth日 cam口utat幻sal technique used, The
parame伯rs lath日 twa types ar日 r비ated through
Sampi日5 口er 口wind = 2까Ii,（다日quency = Sample 甘me)
Number of加et Sam이es = Phase * Samples F｝日r 口日riod/ )2吐M)
Use the sear비日七used 틔n日 ty口B 卄 numeric졔 口roblems due to
running for large 小n日5 (e.g 口serf伯＼sin abs이ate rime) occur,
P日ram日也r5
gn日 ty口e: t;m1m
lime (e: n 꼼胃才．엾e.

-__.__.__.._.- -卜

Might川日：
1
B治8:
U
Fr日qu日ncy )rad/s日oh:
1
Phase (red)
pV2
Sample dma
0
國 Intert그ret vector 口aramelers as卜0

0

0K

Cancel

hi帥）

肖Pt꽈V

그림 13-14 Sine Wave 블록에 위상 오프셋을 설정하여 Co늬ne Wave 지정

396

PART 04. Simulink 설계하기

0 Sine Wave 블록의 글자 부분을 클릭하여 이름을 Cosii妃 砥rave로 바꾼다．
F沌

Ed祛

\Iiew

O匕머ay ［거agram

540｝이a0o0

囹 ' 圄 ,,:; 吟 슘 鸚

Aoaly引5

Code

Toc出

H叫p

" 呻 邸宙 聆 帑 E쩝，，》＠니幽，

미m2
回미m2

r

型， '玄

：自j

e

{i}
4

'딜

E5크
回
口

E亡

曲
易
Re丑却

너e叫 1 error 100%

auto(r/anab4eStepORcr甘te)

그림 13-15 완성된 Cosine Wave 모델

0 [Simulation] - [Run] 메뉴를클릭하여 시뮬레이션을 실행한다．
0 Scope 블록을 더블클릭하면 스코프 창에서 실행 결과를확인할수 있다．
目k므

杓的i

出拙

@니也e 聆

引m山ti긔l

F扼｛p

各 니 익 ' ［꾜 ' 1 + 國 ,

T=20凹0

그림 ]3-16 스코프 창 결과

I

Integrator 블록

Integrator 블록을 이용하면 입력 신호를 시간에 대해 적분한 값을출력할수 있다．시뮬링크에서는 적분
기호／흘대신古뼈 瞻라스변환변수！
，을사용한다．

CHAPTER 13. 시뮬레이션을위한시뮬링크

397

1 여恢｛I 1q- 1，
크 1
L二：
二：
＝二＝
申I
출력변수y를 시간변수 t에 대해 미분하면 진폭이 5인 사인 파형이 출력된다. 시뮬링크를 이용하여 출력변수
y 값을 구하는 모델을 설계하고 시뮬레이션 결과를 스코프 창에 나타내라 ．이때 시간은 0초부터 20초까지 변
한다．

횰可 제시된문제를수식姐표현하면多＝y=Ss血t이다·여기서출력변수
『를구하려면미분과상호보완
古臣성질을가진적분을이용한다. 즉 y(t) =f5 S血tdt이고, 근搢라스 변환변수！올적분기호대신사용
(!

(5)

）로변환할수있다．

(sint)

하면

『=

S

0 Sine Wave 블록을 설계 창에 생성한다（[Sources卜田me Wave]).
O Gain 블록을 설계 창에 생성한다（[Commonly Used Block引m四帥1]).
O 생성된 Gain 블록을 더블클릭하여 田unction Block Paran妃ters] 창을 열고 [Gain］을 5 (5sint）로 바꾼
후 田K] 버튼을 클릭한다．
0 Integr毗or 블록을 설계 창에 생성한다（[Commonly Used 미ocks］丑ntegrator]).
0 생성된 Integrator 블록을 더블클릭하여 [Function Block Parameters] 창을 열고 [Initial condition:]
에 0을 입력한후 回幻 버튼을 클릭한다.
lntegrstor
C口ntinu口us-tim日 lot日gra卄or, of the in口Ut 히goal.
Paramet酊5
External reset; none

!

in出쉬 C口nditi口ns口urce: in岫rnal

!

in川톄 口口nd化口n.
U
國Limit output
［그 \wrap 引a地
口 Sho나 satur日ti口op口Ii
［그 Sho나 sta地 p口rt
Abs口山也 t口leranc日：
auto
口 ignore urn卄 and reset 나hen Uneari키ng
團 Enab冶 Zen그m口r口ssing d日t日C如n
Ste地 Nam甘 (e.g., 'pa引如0 ')

印

OK

Canc비

H日巾

知비y

그림 13-17 1nt四rator 블록에 초깃값 지정

0 Scope 블록을 설계 창에 생성한다（[Sin蝴-[＆叩이）.
O 생성된 블록을 연결한다．

398

PART 04. Sim메nk 설계하71

F艇

E（址

Vie나

마splay

師, 圄

E기agram

Simulation

峀D

An키y5法

Code

h이5

He巾

'S 呻 ＜妊 \b 耶＞ 密 쓰，力 回 ! 釜主 !

Sim3 i
r

團돼m3

田

烈
目

B>1＋
日

/\U

OS的

二I

l's'字atJ

S口玎七

=t

Cmn忙w크峙

圄
團
口

日月

齒
力
Ready

100呱

미拓451

그림 13-18 완성된 시뮬링크 모델

0 설계 창 위에 있는 毆mulation卜小如del Co曲암玎ation Paran妃ters] 메뉴를 클릭하여 [Coi沮guration
Parameters］창을열고［Sta此time］과［St叩time］에각각0.0, 20.0올입력한다．
0 [Simulation]-[Run] 메뉴를 클릭하여 시뮬레이션을 실행한다．
四 Scope 블록을 더블클릭하면 스코프 창에서 실행 결과를확인할수 있다．
F기e

lm뇌＄

vi們V

Smulat曲o

He巾

거

回 r 愁 (8 哈 難 率 , qi , ［꾜 기 f 鬪 ,

,

/

4

:/\

/

1

\

\

7
!T2口oc心

그림 13-19 스코프 창 결과

CHAPTER 13 시뮬레이션을 위한시뮬링크

399

LESSON

그림 창에 결과 나타내기

03

시뮬레이션 결과를 MAT나＼B 그림 창에 나타내는 방법을 살펴보자．
Key1사ord

I

I To Workspace 블록 1 （긔ock 블록 I Mux 블록

To Works口ace, 이ock. Mux 블록

시뮬네이션 결과를 그림 창어］ 나타내려면 시뮬레이션 결과와 시간 정보가 있어야 한다. 이 두 가지 정보
를 하나의 벡터로 묶어 작업 공간 창으로 보낸 다음 명령 창어］ 그래프 그리기 명령어를 입력하면 그림 창
어］ 결과가 나타난다．
시뮬레이션 결과를 작업 공간 칭에 나타내려면 To 硼brkspace 블록을 이용하고, 시뮬레이션 결과를 그
림 창어］ 현재 시간 영역으로 그리려면 Clock 블록을 이용한다. 또한 작업 공간 창어］ 결과를 보내기 위해
다양한블록의 결과를 하나의 벡터로 묶으려면 Mux 블록을 이용한다．

1 예저113-4 I
I HHHH4
-

I

［예제 ]3-3］의 시뮬레이션 결과를 그림 창에 나타내라．

풀이

0 ［그림 13小18］에서 Sc叩e 블록을 제거한다．
0 Clock 블록을 설계 창에 생성한다（[Sources]-[Clock]).
OMux 블록을설계 창에 생성한다（[Commonly Used 미ocks］ 小如刈）.
0 생성된 Mux 블록을 더블클릭하여 [Function Block Paran妃ter司 창을 열고 困Un小er of ii叩uts:］에 2
를 입력한후 回K] 버튼을 클릭한다．
Mux
Mu出plex Sc졔ar 口rye아or 引gn톄S.
Param日抱rs
山mber 口ft叩내S.

留
미日비ay 야）如n: 1 bar

OK

Cancel

그림 ]3小20 Mux 블록의 입력 개수 지정

400

PART 04. Sim매nk 설계하기

He巾 뇨 {

Apply

!

0 To Workspace 블록을 설계 창에 생성한다（[Sit血可-[To Workspace]).
0 생성된 To Workspace 블록을 더블클릭하여 [Sink Block Parameters] 창을 연다. [Variable name:]을
y로바꾸고, [Save format:］에서 Array를선택한다．
T口 누V口rks口ace
汁如 in口utt口 8口日CS日d tim日$日rice, array, 口r 싻r니Clur日 In a 나口rk하冶C已 比rmenu七ased
늬m미帥on, da怯 Iv 니片Ilten In 作l日 MATLA日 base works口ac包 Data is n口lay톄冶b冶 Un川 the
引m니a如0 沽 S的口口日d 口r 口cue日d
To log a b나8 틔Sit톄，use ilmeserie甘님aye 幻tin日t
Pararn日伯ra
Variable name:
y
Urn卄 data p口in怡 t口 lest
jot
Decirn베on:
1

S' 唯format: 絮恥，lure WIth佈, ' /, 4

;n

Save 2山 비g Shrun仙re

巴L口a tie日d-t lime드日ii日8

日亡스心

L}

Sample km日（니 f口r inher仕日d)
-

l

L 0K_jLC日flCel ] [I긔百呵1匕却p坦

a

그림 13-21 To Workspace 블록의 변수 이름 지정

0 생성된 블록을 연결한다．
File

Ed吐

V洹w ［긔op啣

芒乙 , 圄

i거egram

旨atO

듸m出ation

An川V引5

伽de

i出O

H帥｝

"=口華 43 岫 聆 黨 巨卜力 臼 , 區計

Sim4 [
團5im4

二

!

口
4

回
m
［그

갚中흉？ 났
會4H,，닢

［交
i蚤
易
Reach'

100%

ode45

그림 13-22 완성된 시뮬링크 모델

0 [Simulation卜［Run] 메뉴를 클릭하여 시뮬궤이션을 실행한다．
0 y(t)를 그림 창에 그리기 위해1 명령 창에 다음과 같이 명령어를 입력한다．

>> plot (y(: ,2),y(: ,l) );
>>elabel ( 't ) ;
>> 미 北el ( 'y) ;
>> grid;

그림 13-23 시뮬레이션 결과를 그림 창에 그리는 명령에 입력

CHAPTER 13 시뮬레이션을위한시뮬링크

401

口ii} 的t 명령어의 첫 번째 파라미터인 y(:,2）는 x勘1I 해당하는 입력 벡터（여기서는 변수 r률 사용）로 Sim내ation
time에서 설정한 Start time(0.0）부터 St야）time(20.0）까지의 원솟값을 의미한다. 시간이 시뮬레이션 결과의
두 번째 열로 설정된 이유는［그림 ]3-22］에서 Clock 볼록이 Mux 블록에 두 번째 입력 단지로 연결되어 있
71 때문이다. 이때1 시간은 시뮬링크0似1의 기본값인 0.4씩 증가한다. 두 번째 파라미터인 y(:.1)은 입력 벡터
값에 상응하는 출력 벡터 y의 값을 나타낸다．
@ 그림 창에서 시뮬귀伯］션 결과를 확인할수 있다．

그립 13-24 그림 창에 나타난 시뮬레이션 결과

402

PART 04. Sim메nk설계하71

사칙연산 활용 및 1차 함수
입출력 그래프 설계하기
두 행렬의 뺄셈을 계산하는 Constant 블록，사칙연산의 곱셈과 나눗셈 결과를 계산하는 Product 블록과 Divide 블록，출력
결과를 수치적으로 나타내는 미S이ay 블록에 대해 알아보자. 또한 j차 함수 그래프의 상수항과 계수항을 더하는 Add 뷸록도
살펴보자．
Keyword

I Constant블록 I Product뷸록 I Divide블록 1 미S히ay블록 I Add블록 1

I Constant 블록
Constant 블록을 이용하면 실수와 복소수의 상숫값을 생성할 수 있다. Constant 블록 은 상숫값 매개변
수의 차원에 따라숫자, 벡터, 행렬의 출력을생성한다．

1 예저113-5 1
시뮬링크를 이용하여 y = 口 -b의 모델을 설계하고 그 결과를 명령 창에 나타내라．
[3
a -l
[

풀이

21
[1
I, b= I
쉬
Ii

11
I
ii

0 Constant 블록 2개를 설계 창어］ 생성하고（[Commonly Used Blocks卜[C毗tan日） 뷸록의 글자 부분
을클릭하여 이름을각칵a, b로바꾼다．
0 Cot坮tant 블록 a를 더블클릭하여 [Sou丁ce Block Parameters] 창을 열고 [Constant value:］어］ 행렬 口를
입력한다．
Constant
Out口ut th日 c口natant specified by the 'Cons怡nt V궤ue' 口ararn바日r. If
'Constant Va山a' 冶 as日ct口r and 'mnt日rpret sect口rparameters as l- D' is
on, treat the constant value as a 1-0 array. Otherwise, output a matrix
V며rth the same dimen引ons asth日 constant vslu日．
Main 諦融目目烈越蜘題8蜘
C口nstant va山e:
[3,21,4]
團 Inter口ret sec幻r 口arameters ax卜0
Sam미e 打me:
mnt

9

小꾜比m

Canc日I

H到口珏無 ! A而可j

그림 13-25 Constant 블록 a에 행렬 지정

CHAPTER 13 시뮬레이션을 위한 시뮬링크

403

0 ［그림 13-25］와동일한 방법으로 Constant 블록b의 [Cons愧nt V出ue:］에 행렬 b를 입력한다．
0 Sum 블록을 이용하면 상수, 벡터, 행렬 형태의 입력을 서로 뺄 수 있다. Sum 블록의 부호 매개변수를
로 설정하여 뺄셈 연산을 할 수 있다. Sum 블록을 설계 창에 생성한다（[Commonly Used B奴永司
[Sum]),
0 생성된 Sum 블록을 더블클릭하여 [Fm毗ion 미ock Parameter司 창을 열고 [L慨 of signs:］에 + I -를
입력한다. 수직선（ver如小 bar) I를 입력하면 부호 사이의 간격을 설정할수 있다.
0 열려 있는 [Function Block Paran妃ters] 창어써 [Icon shape:］를 rectangular로 바꾸면 Sum 블록의
형태가 원형에서 직사각형으로 변환된다．
Sum

M궤n

的亡n

a그

Add or subtract inputs. Spec啣 one of the 幻加帖ng:
a) string c口ntaining + or - 幻r 日ach inp니t port, If口rs口acer between
p口rts (e.g. .*I나＋+)
b) scalar, >= 1. specifies the number of input ports to be summed.
＼硏冶n there is 口nly on日 inp니tport, add or subtract etemen怡 0蛇r all
비men틔口ns or one s口ec附ed 비men引口n

Icon shape: 姆C拇ng내er
Li없 口f 引gns:

OK, J

挻點封鈿吼二 :

A口口佃

그림 13-羽 Sum 블록의 단자 지정과 직사긱형 변환

0 시뮬켸이션 결과를 명령 창에 나타내기 위해 To Workspace 블록을 생성한（[Sink司냐To Vt幻rk叩配e])
후 더블클릭하여 [Variable name:］을y로 바꾸고 [Save forma씨으로An'ay를선택한다．
I （그 叫orks口ace
누Vri也 inputt口 S口ec而ed tim日series, array, or structure in a 부六3rkS口ace. F口rm日nu-bes日d
帥TIu冶如n. data is 밖n仗en in the MATLAB base 낚mrks口ace. Data 治 n마 as日ilab沌 un出 the
싫muleS口n 治 S幻pped or 口aus日d.
To 佃g a bus 引gnat, 니se Ttmeseries" save f口rmat
Parame也rs
Variable name:
y
Lim什 data 口oin怡 t口 Ia就
mnl
Decimation:
1
Save化rmat: Array

寸

Save 2-D 引gna冶 as: 子D 日rray Ic口ncateoa也 a幻ng third 出！liensi口n)

Y

國 L口g fixed中point data as a ft 口bject
Sample time (-1 for inherited):
1

孕

,

OK

그림 13中27 To Workspace 블록의 변수명과 저장 형식 변환

404

PART 04. Sim베nk 설계하71

,

Canc引

1

H日巾

!

肖1갸기S

0 생성된 블록을 연결한다．
Edit ＼키忿w ［來的Y

囹，冒
SUB 1

二

團SUB

臣쿄

囹
回
［그

D的ram

Simulation

, i/ 鸚 每！

:I

却刈ys놈

Cn心n

it刈5

He巾

" 呻 好的 和 쁘 E斗斗 臼 r蟲 ,
!

，而

F升c

陌

宙
Rea旬

100%

＼血r冶ble앉epAu的 ;

그림 13-28 완성된 시뮬링크모델

0 직사각형으로 변환한 Sum 블록은 마우스 왼쪽 버튼으로 선택한 후 네 모서리 중 한 곳어］커서를 놓았을
11가1대각선 형태의 화살표가 나타나면 크기를 조정할 수 있다．
@ [S뇨iulation t油e］은 [S愧rt time］과 毆叩 tim司에 각각 0.0. 0.0을 입력한다. [Stop time]어］ 0.0이 아
1d 임의의 값을 입력하면 시뮬레이션을 실행한후 명령 창에 동일한 결과가 여러 개 나타난다．
01 명령 창에 명령에 y를 입력하면 다음과 같은 결과가 나타난다．
Command 1舟따由交甘

4\

>> y
y

=

2
0

1
3

그림 13-29 명령 창 결과

I Product 블록
Pr(쿄uct 블록은 다수의 입력어］대한 곱셈 또는 나눗셈을 수행할 때 사용한다. 곱셈 매개변숫값에 따라 원
소 단위 또는 행렬 곱셈을 사용하여 출력을 생성한다. 문자 永와／는 입력어］대해 수행할 곱하기 및 나누기
연산을 나타낸다．

I

Divide 블록

D如ide 블록은 첫 번째 입력을 두 번째 입력으로 나눈 계산 결과를 출력할 때 사용한다. 기능적으로 이미
설정된 2개의 블록 매개변숫값이 있는 Product 블록처럼 동작한다．

CHAPTER 13 시뮬레이션을 위한시뮬링크

405

I

Display 블록

Display 블록은 연산 결과를숫자로 보여줄 때 사용한다. 이때 Format을 이용하여 출력 형태를 다걍하게
선택할수 있다．

1 예제 13田

1

수식 d= ax b -- c를 계산하는 시뮬링크 모델을 설계하라. 여기서 a = 40. b = 3. C = 5로 지정한다．
系i

O Cons扼.t블록3개를생성하고（[Commonly Used Bloc畑］-[Constant]）블록의 ' ］름을각각 “，b, c로
바꾼다．
］어］ 40을 입력한다．
0 블록 a를 더블클릭하여 [Constant vah妃：
Constant
Ou巾ut the constant specified by the Constant value parameter, if
'C口netani valu日 冶 an日clor and In也rpret sec伯r 口aram日tars as 卜 ［) ' is
口n, 甘日atthe c口nstant salu日 as a卜0 array. 0th日r\MSe, 0U巾니ta rnatr法
咐if, the same 버men引one as the constant vs山5

1Constant

r誦工藪面爾函重自
value:
40Interpret vector parameters as 1-0
Sample 1ime
m l

抄

.trprp11 r- -

m

L塑쁘그

그림 ]3-30 Constant 블록 a에 상수 지정

0 ［그림 13-30］과동일한방법으로블록b와C의 [Cot坮tant V出ue:］에 각각3. 5를 입력한다．
［卜4a血 Opera加ns卜回oduct]) 블록의 이름을 ab로
02개의 입력을 곱하는 Product 블록을 생성하고（
바꾼다．
0 블록 ab를 블록 C로 나누는 D加ide 블록을 생성하고（[Math Operation司Hm如ide]) 블록의 이름을
ab/c로 바꾼다. 블록 ab/c를 더블클릭하여 困umber of inputs:］의 기본값 町를 그대로 유지한다．
1

Product
Mu뺘加 or didde inputs. Choose 이ernest＼
너Se 口r maths 口rod나ct and
5口Sc加 one ci the 幻妃뗘四
a) 士 0r / 幻r 日ach input port For 日Xam口1日』士士／士 口日rtormn fir日 D口日ration
s1*uZ/u3*v4',
bi scalars口巳cities th日 numb日r 口tin口ut p0,1510 b日 mob口lied
lithers is 口Sip 口no input p口0 and lb日 }d山呵七帥口n 口arame也r 陌 5日t t口
E陌m8n卜州胡卜）, 日 引n미日 1 or / C미a口see the in口니I sign쉐 U引ng the
specifi日dop日raIl口o. Ho무lever, fi th日 }d나川plicali口n 口aram日也r 泊 5日t t口
Matrisi.). a 引vs旭 ! causes the 벼口ck 幻 011巾01 the maths 너nchansed,
and a 引ngl日 / cc너日日sth日 너ocklo out口utth日 maSts in晦rB日

Main ；函n쉐／뻬b嶇司
Numb日rolin口ulo
t/
卜札lip比all口n: ［目亘m日lIt岾8e(,.L ,

毋

i

（가（

Cancel

Help

그립 13-31 DMde 블록에 부호 지정

01玉splay 블록을 생성하고（[Sit止引-[미叩lay]) 블록의 이름을 d로 바꾼다. 블록 d를 더블클릭하여
[Forn狙t:］의 기본값 출력 형식 short를 그대로 유지한다．

406

PART 04. Sim메nk설계하71

0 설계 창의 메뉴 표시줄에서 圄mulation] 메뉴를 클릭하여 ［卜4odel Configuration Parameters] 창을 열
고 田top tin妃］을0.0으로 바꾼후모델을 시뮬레이션하면 다음과같은 결과를 얻는다．
Rie

EdO

Vew

囹 1目

마xmay

Dt1ae 出'5出내0n

Aol恥括

C끄4加

t剛＄ 卜｛帥1

守 " 鸚 " 呻 4 8 盼 多 因 , ,, 凹 ! ..
幽. ,

MDI 1

e 回MD1

鐵
口

!

40
1

0

4

臼
心
［그

X
+

2'
"

3

0

5
口

a
{1
分
F匣i岫r

VIew 1w가Ed四 100%

Vr,abIx았epDiscrete

그림 13-32 완성된 시뮬링크 모델

0 시뮬링크 모델을 다음과 같이 설계할수도 있는뎨 그 결과는［그림 13-32］와동일하다．
m

Ed往

V由m

囹, 圄

l긔splay

D吼邸m

듸rnulatioo

角玘卜ys匹

Code

b帥i

Help

" 鵠 " C咽 也 七夕 汐 67 E小，
, 凹, 幽,

MD2

e 回MD2

蕪
a
4

回
團

!
40
1
X
X
I
aty乙

b

［그

5

心

0

d

出
力
Ready

VIew 1 WI出目 1O啼

\/axiable많eFOsa吼e

그림 13-33 ［그림 ]3-32］과 동일한 시뮬링크 모델

0 ［그림 13-33］에서 Divide 블록able를 더블클릭하여 [Number of inputs:］에 串水／를 입력한다．

비0

小귤墨孕료글冬壹言玉료

F가oduct
MutE口ly or di너d日 inputs. Choose 미日ment-＼너on or maIns 口roduct and
5口ec加 one of lt日 幻n口＼너ng
a) 1 or / 幻r 日aol, in口Ut 口cr1. For exam口1日，士t／士 口日norms the o口erallon
ul -uZfu3tu4'
I) scalars口eciltes lh日 numb日r 口fin口Ut 口orts to be mu川비冶d.
卄 Ed日r日 is 口nIp 口ne In口Ut 口口rt 日nd the Mu川口1ic日g（가l 口aramet日r 冶 S日tb
티日ment- wise(.') 』日 引ogle * 口n /C미laps日s th日 in口Ut 늬gnal U引ng the
S口ecilled 口perati口n. H口늬over. lithe I너U出1내call口0 口arameter is set t口
Matxix(*), a 이ns旭 升 causes Ed日 비口ckl口 0나巾Vi the mall似 unchang日d,
and a 引ogle / causes Ed日비ocktc) 口U巾ul the matrix inverse.
SI묘oat 餉rib山日S

Number of m口U怡
--I

卜／ulti미cut口0: ! E冶menl-wise(．日

1

OK

H Canc日口

He巾

그림 13-34 Divide 블록에 세 부호 지정

CHAPTER 13. 시뮬레이션을 위한시뮬링크

407

I

Add 뷸록

Add 블록 은 Sum 블록과 유사하게 입력을 더하거나 빼는 데 사용한다．

1 예저113-7 I
1
1
'

"

"

!

］차 함수 y =ax+ b를 계산하는 시뮬링크 모델을 설계하라. 여기서 口 = 2. b = 小3 이고 입력변수 工는 1부터
10까지 1씩 증가하는 벡터이다．

배경
지식
풀이

l차함수y =ax+ b에서 x는 입력변수, 계수（coeffici毗）a는 1차함수의 기울기 (slope) , 상수 b는 절편
位吐ercept)이라고부른다．
0 Constant 블록 3개를 생성하고（[Commonly Used Block司[C毗tant]) 블록의 이름올 각각 x, a, b
로바꾼다．
0 블록 x를 더블클릭하여 [Constant value:］에
[1:10］을 입력한다．
0 블록 a의 [Constant value:］어］ 2, 블록 b의

C口nstant
0나巾utthe con싻日nt S口日cited by the 'C口net日nt V日lu日‘ par日m甘目r. tf
C口ns伯at 떼U可 冶 a 蛇ctor and 'triter口ret Vect口r 口arame伯rs as ] 나［) ' is
on, treat th日 constant Ca山e 日sa 卜 ［) array, 0th日rwi＄日， output a matr似
＼나to the same 비men틔口as as the c口n嗽ant valu日．
Main { Sipnat拉曲岫8 1

[Cons愧nt value:］에 -3을 입력한다．

Cons伯nt va山e:

0 벡터 x와 계수 a를 곱하는 Product 블록을 생
성하고（
［卜4ath Operations]-[Product]) 블록
의 이름을ax로 바꾼다．
0 블록 炚와 절편 b를 더하는 Add 블록을 생성
하고侮4ath Operations]-[Ad괴） 블록의 이

n to]

國 tn也rpret vector 口arameters as 卜 ［)
Sam히etime
mnt

, :j魏t)具赳m 耐捌枷難 L如ply '
, 砥＼

9

그림 13-35 Constant 볼록 x에 벡터 지정

름을 ax+b로 바꾼다．
0 시뮬레이션 결과를 명령 창에 나타내기 위해 To Workspace 블록 2개를 생성하고（[S址司可To
Workspace]) 블록의 이름을각각毛m, 兄out으로 바꾼다．
0 블록凡血을 더블클릭하여 [Variable name:］을x. [Save forma川을Array로 바꾸고, 마찬가지로 블록
兄out의 [＼向r佃ble name:］을y, [Save format:］을Array로 바꾼다．
Ts 們torttapace
＼시1吼日 In口altoS口日trill日d times日des, array, or slilictur日 in a 내姓叩吼日 F口rmenu-based
늬m네at幻n, data 治 咐tten tn to日 MATL,48 base 나orbs口an已 Data 冶 not avalleb伯 Un씨 a日
引m네帥Dn 治 引口pped or 口aU8日d
Te匕gab니S 퍼gnat, us日 ' Ttmaserles" save 化rmat
Par日m日也r5
甛dabte narne:

List夙 d日tap口late to Is就
自寸
0目cboa加n:
1
Save 幻rteat: At了ay

岫 丑月

Sa比 2七 늬aria冶 a$ 匡0 array (concat日nate 졔口ng 由ird din｝日n5幻n)

r

團 L口a 似ed-point data on at obi日Ct

-

Sam口1日 也me （나 幻r inhert咆d)

l

汾

匕그卜

! 1 Cancel H H미pJ

그림 13-36 블록 xjn의 변수명과 저장 형식 변환

408

PART04. Sim메nk설계하기

1＼민기U

0 생성된 블록을 연결한다．
Fih므

Ed往

\/i的y

舜, 目

{：卿枳y

Da孕隘rn

SIT,겪i坦翔冊口勵幽瞬針C斟如삐缸油n1嫡材

二 卞： 납 鸚 每 !

外 呻 邱 呻 吟 唾카 匹 中扮 回 ! 硅計

FUNI
V

jFUNl

的

風
!3

-

'1며

I1

:

口：

"

多

m

二；

回
口
[：그

E므

曲
Rea句

虹10拓

V鈿怯뱌eStepAuto

그림 13-37 완성된 시뮬링크 모델

0 [Simulation time］은［Startt恤e］과［S따time］에 각칵0.0, 0.0을 입력한다．
m 시뮬레이션을 실행하고 다음과 긷이 명령 창에 명령어를 입력한다．
r 0mm帥d
>> plot (g! y) ;
>) glabel ( x ') ;
>> ylabel ( y , rot .-380) ;
>>title (Linear Function ') ;
>> grid on;

그림 13-38 시뮬레이션 결과를 그리는 명령에 입력

111) 명령어를 입력하기 전에 시뮬레이션을 실행해야（[Sim내a如n]-[Run] 또는 圄）변숫값이 작업 공긴뻐1 저장된다．

q1 입출력 그래프를 나타내는 그림 창이 생성된다．

그림 ]3-39 1차함수그래프 생성

CHAPTE日 ]3 시뮬레이션을 위한시뮬링크

409

LESSON

05

복소수를 실수부와 허수부로 분기시키는 Dernux 블록, 각각의 실수부와 허수부를 복소수로 변환시키는 Re켸니rn的 to
Corn히ex 블록에 대해 알아보자. 또한 복소수를 크기와 편각으로 분리하는 Corn히ex to Magni山由-An寸e 뷸록, 반대로 크
기와 편각을 포함하는 복소수로 나타내는 Magnitude-An이e to Corn히ex 뷸록도 살펴보자．
Keyword

1 Dernux블록 I Rea니rnag to（力叫)Iex블록 1 Corn히ex to Magnitu由-An이e블록 1
1 Magni加de-Angle to Con制ex블록 1

I

Dernux 블록

Demux 블록을 이용하면 입력 신호의 성부을 추출하여 각각의 출력 신호로 분기할 수 있다．

I

Re톄니mag to Corn이ex 블록

Real-Imag to Con巾lex 블록을 이용하면 분리된 복소수의 실수부와 허수부의 입력을 완전체의 복소수
로 나타낼 수 있다．

복소수 z = -3 + i 률 시뮬링크 모델로 생성하고 그 결과를 나타내라．

배명
지식

복소수z는다음과같이 실수부분을나타내는工, 실수y와허수단위（ima帥皿yur血）i (또는／
）를곱한허
수부분을 더한 직교 형식 (rectangul町 凡rm)으로 나타낸다．
z = 工+ 砂

풀이

0 Constant 블록을 생성하고（[Commonly 小ed Blo出引-[Constan日） 블록의 글자 부분을 클릭하여 이
름을x卄y로바꾼다．
0 블록 x＋汐를 더블클릭하여 [Cons杻nt value:］에 [-3 1］을 입력하고 回幻 버튼을클릭한다．

0s中old伯 C口nslafll 5口e口而日d by lb日 Ccl,引0010日仙日 口arameler. ft
'C口nstanl Va山a' Is a 陀미or and 'Interpret aector 口aramel日r5 a5 卜 ［1 is
口0, Ir日at tha C（그n引ant a計ue as a 1 나그 array 마herwlse, a나巾Ut a ma們X
U片th lb日 Sam日 녜m日n쇠ens as lb日 C口r,stanl S눼U日

[-3

Main

風9110] 面rib西司

1]

!

S日epic Sn］日

分

!

i OK j 的Ill到m m回m. ypply

그림 13-40 （兀ns怡nt 블록 x+. ,에 상수 지정

410

PART04. Sim메nk설계하기

0 Demux 블록을생성하고（[Conimonly Used Blocks卜[D印mx]) 더블클릭하여 囚umber of o啣uts:]
에 2를 입력한다．
Demux
Spilt vector siynals into scalars or smaller vectors. Check 'Bus
Se冶C如n,化d日’ to a口lit bus 引gna沽，
Parameters
Numb日r 口f 口utr）니t各
2
0冶play 야川0川 b日r
國 B나as쉬日cli口nm口de

U

Cancel j i

OK

Help

그림 13-41 Demux 뷸록의 출력 개수 지정

0 Real-Imag to Complex 블록을 생성한다（
［卜'Lath Operation引나Real-Im雎 的 Corn히아］).
0 시뮬레이션 후복소수로 변화된 입력값을 직접 보여주는 D始play 블록을 생성하고（[Sii永可-ED迪,la列）
블록의 이름을 z로 바꾼다. 블록 z를 더블클릭하여 [Format:]의 기본값 출력 형식 short를 그대로 유지
한다．
0冶play
Numeric dist놔ay ot In口나t Va山es
Parameters
F口rTnat: 帥미t
0日cimati口n
1
E그 日口a心ng d沽비sit

roK1 r七日n口日i 1 小쁘브그

0

그림 13-42 미하)Iay 블록에 출력 형식 지정

0 블록을 모두 연결한후 설계 창의 메뉴 표시줄어써 [S뇨iulation] 메뉴를 클릭하여 小4ode1 Configuration
Paran妃ters] 창을 열고 [Stop time］을 0.0으로 바꾼다．
0 완성된 모델을 시뮬레이션하면 다음과 같은 결과를 디스플레이 창을 통해 확인할수 있다．
Edit

\／沌V프

昆! 胄

F作e

1

OVsplay ［거aevam

듸m出Otis,

Ani卜r5匹

Cs蜘

毛아s

He巾

m旨醫 好 唯薑 ! 呻 唾 宙 昨 」乞匹 ,

쿄9

r

幽

!

COMPI

商

!

團COMPI

e

토｝

냅

,I ＝烈, ，「 , ""11

圄
團
［그

Em
i쿄
Rea旬

l伉嘴

it켸a뱌弱tepO目口以e n

그림 13-43 완성된 시뮬링크 모델

CHAPTER 13 시뮬레이션을 위한 시뮬링크

411

弓 Corn이ex to Magn什ude -Ang旭 블록
Complex to 八4agnitude -Angle 블록을 이용하면 복소수 입력을 복소수의 크기와 편각으로 각칵 변환
할 수 있다．

1 예처113-9 I
1
t
복소수 z = -3 + j를 크기와 편각으로 변환하는 시뮬링크 모델을 생성하고 그 결과를 나타내라．
；藻
지식

복소수 ' ＝工＋沙의크기는『로나타낸다．복소수의크기와！
축人1O1의각도0는복소수：의편각또는위
상칵이라고하며다음과긷b］나타낸다．

r니기＝／工' +y'
ta可

'}

=

町gz

0＝

Constant 블록을 생성하고（[Commonly Used 미ocks]- [Consta蝴） 블록의 글자 부분을 클릭하여 이
覇； 0 름을
z로 바꾼다．
0 블록 z를 더블클릭하여 [Constant va1ue:］에 3+i를 입력하고 回K] 버튼을 클릭한다．
Con밗ant
Quip니tth日 C口n引ant 日pen出日d by the 'Con日taft sa山e' parame伯r. If
'C口netant va山e' 冶 a 叩아or and In伯r口ret 陀마Or 口arame也re as 卜 ［y 沽
口r , treat the c口netant valu日 as a 卜 ［) 日rray. 0th日rwis已 口u巾Ut C matne
낵卄h the a日me 비m日n비one as the cone治nt Va山e
Main

拭日nal Attribut日5 !

-3i

C口nstarnt Va山e:

團 In伯r口r日t sect口r 口arame也rs a日卜 ［)
Sam비5 卄m日：
int

心

,

OK

Cancel

H日巾

I A口비y )

그림 ]3-44 Con없ant 블록 z에 상수 지정
0 Complex to 入4agnitude-Angle 블록을 생성한다（
［卜4ath Operation司[Co啣lex to 入ila얍nitude
Angle]).
O Display블록2개를생성하고（[S址5］丑玉splay]) 블록의 이름을각각Mod, Arg로 바꾼다. 블록을 더
블클릭하여 [Fom也固의 기본값출력 형식 short를 그대로 유지한다．
0 블록을 모두 연결한 후 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 [Model ConfIgurati아l
Parameter司 창을 열고 [S幻p tin妃］을0.0으로 바꾼다．
0 완성된 모델을 시뮬레이션하면 다음과같은 결과를 디스플레이 창을 통해 확인할수 있다．

412

PART04. Sim메nk 설계하기

1日b

帥t

" '빛

I I芍 ' 目
1 C0M匹

Display

Diagram

Simulation

駙r

Ma堈료

C出e

初이S

He巾

"呻 邸四 昑 (\ 巴 ' " L寸
'釜Ii.

團COMP2

니
1

a1叫

1

f七a
3.i
i

斗
由n1斗므Xt口
「啣m四e'm
"

11三可

rt
4

>
I Re刊p

100%

au螂帥比닯eP蜘鉀｝

!

그림 13-45 완성된 시뮬링크 모델

모델1
설명

Mod 블록의 값 3.162는 주어진 복소수의 절댓값을 계산한 결과와동일하다．
口= /（日）' + 12 = 3.1623
Arg 블록의 값 2.82는 주어진 복소수의 편각을 계산한 결과와동일하다．

argz= tan나；= 161.5741.

I

"

2.

5了끎：

161.

=

다음과같은 계산으로 각도 161.5741' 를 라디안으로 변환할수 있다．

82

Magnitude- Angle to Corn이ex 블록

八4agnitude-Angle to Complex 블록을 이용하면 복소수의 크기와 편각을 입력하여 완전체 복소수로
변환할수 있다．

1 예제 13-10 1
복소수의 크기가
「= 2이고편각이 日＝증일 때．시뮬링크를 이용하여 복소수z를시뮬링크모델로생성하고
그 결과를 나타내己F.
1.1,=

茄

삼각함수의 기본성질을 이용하면복소수의 직교 형식 z = 工＋加를x와y로 나타낼 수 있다．
工＝rcosO, y= rs如［日
그러므로 복소수는 다음과 긷삐 극 형식 巾이ar form）으로 나타낼 수 있다．

CHAPTER 13. 시뮬레이션을위한시뮬링크

413

z = r (cos日＋isin功
覇；

0 Cons帥t뷸록을생성하고（[Commonly Used Blocksll-[Cons鈿t]）블록의 ' ］름을「theta로 " 超다·
0 블록r-出eta를 더블클릭하여 [Constai式 value:］에 口pi/6］을 입력하고 回K] 버튼을클릭한다．
C口nstant
Ou如it the c口nstant 5口ec附ed by the 'Constant vs山e' 口arameter. if
'Cone伯nt V눼U日‘ 冶 av日ctor and interpret V日Ocr 口arameters as 卜 ［3 ' is
on, 甘日at lii日 C口nstant valu日 as a ] 七 array 아hersds已 口utput a matrie
쌔仕hth日 sam日 비m日0引口ns as the constant Va山已

!Constant

i Main 匯區亶歷孤藿豆j

-[3

[2pV61 value:
Ri interpret vector parameters as I
Sample
nt

time:

OK

9

J Canc日i j

ke奴融 f Apple 「

그림 13-46 （力nstant 뷸록 r寸heta에 상수 지정

0 각칵의 크기와편각을출력하기 위해 D이flux 블록을생성한다（[Commonly Used Blocks卜［D帥ux]).
0 Magnitude-Angle to Complex 블록을 생성한다（
［入4ath Operati이瑚小[Magnitude-An멤e to
Comple刈）.
01玉splay 블록을 생성하고（[Sii血日나D蜘la月） 블록의 이름을 z로 바꾼다. 블록 z를 더블클릭하여
[Format:］의 기본값출력 형식 short를 그대로 유지한다. 복소수가 전부 보이지 않을 때는 마우스를 사용
하여 블록z의 크기를 알맞게 조절하면 된다．
0 블록을 모두 연결한 후 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 [Model Conftguration
Parameter可 창을 열고 囹的p time］을0.0으로 바꾼다．
0 완성된 모델을 시뮬레이션하면 다음과 같은 결과를 얻는다．
多뇨 드出L ＼丹咐

0뗘此旴

舜! 冒 寸 二

D,a甲en

s加,ut吐kfl

As畇S's 口心 1刃t; 卜卞叫p

' 鸚 ’『呻 텍 回 昑 毖 쯔 !，『 @ ! 宦彗 ,

C0MP3
!

團C0MP3

：咬

的

因
at

갚 { ＝烈,

」 唯'1.

區
四
口
I.

出
力
Rea匈

l佚）%

auto恤rmb陌닦epo的曲｝

그립 13-47 완성된 시뮬링크 모델

모델1
설명

414

블록z의 값은주어진 크기와 편각을 이용하여 계산하면 다음과 같다．

z = 2(c畔+is喝니孕朴口32+il
PART 04. Simuhnk설계하기

CHAPTER

14

미분방정식

1丁丁丁二

CONTENTS
LESSON 01 ］차 미분방정식 시뮬링크 모델 설계하71
LESSON 02 2차 미분방정식 시뮬링크 모델 설계하기

LESSON

01

1차 미분방정식 시뮬링크 모델 설계하기

j차 도함수만 포함하는 4차 a분방정식을 계산하는 Subtract 볼록과 Gain 뷸록，블록의 위文屠 회전 및 뒤집7后田1 각 뷸록
율 시각적으로 최적화하는 태p 블록에 대해1 알아보자．
Keyword

I Subtra（艾불록 I Gain 블록 1 태p블록 1

I Subtract 블록
Subtract 블록은 Sum 블록의 뺄셈과 동일한 기능을 한다．

丘 G졔n 뷸록
Gain 블록을 이용하면 입력에 상숫값을 곱하는 계산을 할 수 있다. Gain 블록은 口4ath 帥eration引小
[Gain] 또는 [Commonly Used Blocks] - [G諦ii 에서 동일하게 사용 가능하다．

1 예工II 14- 1 I
1
I
"

"

'

-

다음과 같은 1차 미분방정식의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이때1 시뮬레이션
의 실행은 0초부터 5초까지 진행한다．
j'(t) = 4sin3t - 5y, y(0) = 1

풀이

0 Sine Wave 블록을 설계 창에 생성한다（[Soi玎ces] -[Sine 砥rave]).
0 [Source Block Parametet司창을열고囚nplitude:］에 진폭4, [Frequency (rad/sec) :］에 각주파수3을
입력한다．

416

PART04. Sim메nk 설계하기

돼ne 小治ye
0u如ut a 引n日 way呵
0(t) = 向ii口士Sin(FreqH.Phase) + 日1as
텨n日 h／口e detertn比5 tiie C（그m口utatlonal日chnlque used. The
口arame伯rs in 甘）e two ty口es are related through:
Samples 口er pen口d = 2士口i/ (Frequ日ncy ! Sam비etime)
Number of offset samples = Phase t Samples per period / (2싸）l)
Use the sample七as日d 引ne ty口eif numeric톄 口roblems du日 to
running 幻ri日rge tin冶s (e.g. 口yerfiow in absotu也 time) occur.
Param日t마5
돼n日ty口e: 1 Tim目自孕＄ed

y

기m日（ty ［브多日simulati口n time

니

Mi口日山de
4
미as:
0
Frequency (rad/sec):
3
Phase (rad):
0
Samp旭 time:
0
團 In伯r口ret sec幻r par日me佃rs as 卜 ［)

奴Ca口csl h He而그 1而曲m

山 ,OK

a

그림 似너 Sine Wave 블록에 진폭과 각주파수 입력

0 Subtract 블록을 설계 창에 생성한다（[M毗i Operation引1田ubtract]).
0 Gain 블록을 설계 창에 생성하고（[Commonly 小ed Blo出司 ［Ga刈） 더블클릭하여 [Gaii피에 5를 입
력한다．
0 Intergrator 볼록을 설계 창어］ 생성하고（[Continuous］小nte얗鈿日） 더블클릭하여 [Initial condition:］어｝
초깃값 l (y(0) =1）을 입력한후 回K] 버튼을클릭한다．
0 Scope 블록을 설계 창에 생성한다（[Sinks] -囹cope]).
O 생성된 블록을 연결한다.
F如

Ed忙

\dew

西｝! 冒

D바血V

t거agram

돠matatton

An칡ys匹

Code

勿a注

He巾

" 器 " 呻 站 노늉 胎 ( E小力 （拉！堪恥

LDE2 I
的 團LDE2

發

烈1＝닢

짊

'3

巨크

寸

믈

/=L

E弓
mh1

\<f

團
［그
E之

由
力
Ready

苡夙

Vanab地立epAut口

그림 14丑 완성된 시뮬링크 모델1

0 m如del Configuration Paran妃ters] 창을 열고 [S切rt time］과 囹加p time］어］ 각각0.0. 5.0을 입력하면
다음과같은 실행 결과를 얻는다．

CHAPT日극 ]4. 미분방정식

417

F沁

Tools

Vie뾰

듸n0Ut卜야｝

He巾

出

@ 니 啞 (8 聆 好 三率 , 텍 , ［꾜 , f 區 ,
同

Rrady

-T=5.OO0

그림 ]4中3 스코프 창 결과

I

F印 븀록

Flip 블록을 이용하면 블록 또는 블록 그룹의 회전과 뒤집기가 가능하기 때문에 블록의 위치를 조정할 수
있으며, 이를통하1 시뮬링크모델의 시각적 위치를향상할수 있다．

! 예제 14- 2 I
다음과 같은 ] 차 미분방정식의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이때1 시뮬레이션
의 실행은 0초부터 ] 0초까지 진행한다．
5'(t) = 1.5y(1 -y),

풀이

y(0) = 0.1

0 Gain 블록을생성하고（[Commonly Used 미oc畑］-[Gain]) 더블클릭하여 [Gait피에 1.5를 입력한다．
0

Intergr貳or 블록을생성하고（[Cont血uous卜[Integrat川）더블클릭하여 [Initial condition:]에 초깃값
0.1 (y (0) =0.1）을 입력한다．

0 두 입력값을곱하는Product 블록을 설계 창에 생성하고（[Commonly Used Block司- [Product]) 마우
스오른쪽 버튼을눌러 [Rotate & Fli1小［Flip 미ock］을 실행한다．
OSum 블록을생성하고（[Commonly［殆ed B!어：1匐 田urn]) 마우스 오른쪽 버튼을눌러 田야ate &Flip][Counterclockwise］를 실행한다. Sum 블록을 더블클릭하여 [List of s咆好q를 니 나로 바꾼다．
Sum
Add or subtract 汭Pu忖 sP日cUy 口0日 口fth日 幻比내n9:
a) 렇눠ng containing. or = 佃 日a帥 in口Ut 口（吼 1 幻rs口日car bets尼日0
ports 伯.g. =I- l++)
b) so졔Cr, >= t, op日C川as the numb日r 口in口Lft ports to be surnm日d
Wien there 冷 only 口ne in口U냐ort, add or subtract 비em日r,ts over au
네m日n이口no or on日 하尼cifled 비mans油n
)

! Main 哺蜘眺蜘鈿拇晷
Ic口n sha口日： i密啣毖i1各椰
L油tot 틔gns:
느

II,

OK

{ 1 Canoe니 i

그림 14-4 Sum 블록에 부호 지정

418

PART 04. Simulink설계하기

H日ip

1

0 Constant 블록을생성하고（[Commonly 小ed 미ocks卜[Constan日） 더블클릭하여 [Constant value:]
어］ l을 입력한다．
0 Scope 블록을 설계 창에 생성한다（[Sii止引-[Scope]).
O 생성된 블록을 연결한다．
!m1 Ed吐 니ew

固, 圄

o畔lay

Dia9rar

듸,culatlon

韜 每,

Ana卜-

Cc巾 功nm5

H帥）

" 呻 의 唯 且目 『 巨3 , ,, （汐 , .d茴 ,

LDE3
回山E3

e

烈
11

!

U

口

=

m

小

I

烈11U
M．

므

［그

뇨

m
出
力
Re畇

100%

＼翩a벼I出B的岫口

그림 14-5 완성된 시뮬링크 모델

0 [Model Configuration Paran妃ters] 창어써 [S切rtt油e］과 毆叩 time］에 각각0.0. 10.0을 입력한다．
0 실행 결과는 다음과 같다．

F的
그림 14田 스코프 창 결과

졔시된 미분방정식은로지스틱 (log慨ic) 방정식이라고 하며 스코프 창은 인구증가의 모델을보여준다．

11 （뇌II카 1d_ !4 I
1

"

'

"

"

V

다음과 같은 연립미분방정식의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이때1 시뮬레이션
실행은 U초부터 10초까지 진행하며 각각의 계수는 口 = 0, b= 2, c =-l. d= 0이다．
x＝口x + by,

工（0) =2

y= C工＋力,

y (0) = 1

CHAPTER 14. 미분방정식

419

풀이

OSum 블록을 생성하고（[Commonly Used 미ocks卜囹UI川） 마우스 오른쪽 버튼을 눌러 [Rotate &
Flip]-[Flip Block］을실행한다. Sum 블록을더블클릭하여 [Li眺of signs:］를 1+＋로유지한다．
0 Gain 블록 2개를 생성하고（[Commonly Used 미ocks] - [Gain]) 볼록의 이름을 각각 Coef-a,
Coef-b로 바꾼후［如tate & Flip卜[Flip Block]을 실행한다．
0 블록 Coef-a를 더블클릭하여 [Gait비에 0（계수 口 = 0）을 입력하고, 블록 Coef-b를 더블클릭하여
[Gait비에 2（계수 b= 2）를 입력한다．
0 Cot好tant 블록을 생성하고（[Commonly i招ed Blocks卜［Constant]) 블록의 이름을 x-initial로 바꾼
다. 블록 x-initial을 더블클릭하여 [cot瑁tant V出ue:］에 2（초기 조건 工（0) = 2）를 입력한다.
0 Intergr毗or 블록을 생성하고（[Continuo出卜[Integr毗아］) 블록의 이름을x-恤로 바꾼다. 초기 조건을
외부 신호로 받는 입력 지정을 위해 블록 x-mt를 더블클릭하여 [Initial cond就油邱olj丁ce:］를 ex妃mal
모드로 바꾼다．
Integrator
Continuous-time integration ci the input signal.
Pararnet아S
External reset: O口ne
Initial condition source: 日eternal
巴 [Jo卄I ou如Ut
巴 V汁a口 致ate
口 Sh口나 sa山ration port
巴 Sho낵 eta也 port
Abs口山伯 t미日ranc日：
aut口
口 Ignore uirn什 and reset 늬4,en lineari기05
回Enable zero-crossing detection
State Name: (e.g.. 'p口帥的n,)

OK

Canc日1

He巾

그림 14-7 Integrat아 외부 신호 입력 지정

0 마우스 왼쪽 버튼을누른 채 지금까지 생성한블록을 지정한후 마우스 오른쪽 버튼을눌러 [Copy］를 선
택하고 설계 창의 공간어］ [Paste］를 실행한다．
0 붙여넣기로 생성된 Gain 블록 2개의 이름을 각각 Coe卜c, Coef-d로 바꾼다. 블록 Coe卜c를 더블클
릭하여 回au피에 -1계수C = 寸1)을 입력하고, 블록C叱卜d를 더블클릭하여 田毗m에 0（겨｝수d= 0)
을 입력한다．
0 붙여넣기로 생성된 Constant 블록의 이름을 少initial로 바꾼 후 블록을 더블클릭하여 [Constant
value:］에 l （초기 조건 y(0) = 1）올 입력한다．
0 붙여넣기로 생성된 Intergrator 블록의 이름을y-int로 바꾼다．
由 Scope 블록을설계 창에 생성한다（[Sii止司dScope]).
Q 생성된 블록을 연결한다．

420

P／뇌극T04. Sim메nk설계하71

Ftte

Ed仕

new

t雍的y ［거agranr

曷! 目

引or山1tk川

Anafys枉 口巾 b머s

He巾

琵 " 呻 ＜也 叫 陪 鞋 匹 !,, \g? , 幽 !

山E5

e 團LDE5

我

dh
tP

므

n
1
Cm寸b
n

녑

C이4 a

回

1
七드

느

::'

n
니

g

C口'- a

C蜘
寸

;

I
ym和

1
V
yi1

力

Rea旬

1O片

0de45

그림 14- 8 완성된 시뮬링크 모델

모델1
설명

· 주어진 연립방정식은포＋入= 0과y＝즐어］대한l차방정식의 선형 시스템을나타낸다．
· 두 연립미분방정식의 결합 성질 때문에 블록 x-int 출력 姓三 블록 Coe卜C에 연결하고 블록 y-int 출력 y
는 블록 Coef냐州1 연결한다．
' 초기 조건을 나타내는블록 x-油tial과블록y-initial은블록x-int와블록y奴의 단자工0어］ 연결한다．
mScope 블록을 더블클릭하여 스코프 파라미터 창을 열고, 두 연립미분방정식을 입력 단자로 지정하기 위
해 [Fi뇌e困Un小er of Input Port司H口］를선택한다．
10os

圻咐

Simulation

He巾

Open at Start of S,mulation
Number 。' Input P。
rN
Print ..

CUI.P

口one

/

2
3

Pont to flgcee
口t.w

口core All Sc뎌片 싸In南邸

그림 14田 스코프 파라미터 창 열기

CHAPT日극 ]4. 미분방정식

421

侄） 두 결과를 하나의 스코프 창어］ 나누어 나타내려면 다음과 긷삐 실행한다. [Layot川을 클릭하면 행과 열
로 나누어 결과를 보여준다．
Fl晦

To｛코5

\／卜ew

Sin,uL試幻O

H帥1

1

O 니 4e 肛 e i 各 U 包 , 띠 1 f 囹 ,

目
oj

Ir!月［1

1
to
F七帥小r

그림 似너0 스코프 창에 입력축 27H 지정

m ［卜4odel Configur曲on Paran妃ters] 창을 열고［鈿nulation tin刈의 [S切rt time］과 [St叩 tim司어］각
각0.0, 10.0을 입력한다. 回K] 버튼을클릭한후 시뮬레이션 실행을 시작하는 버튼을클릭한다．
四 匹）의 [Layout] 좌측 2개1 블록을 마무즈로 클릭하면 다음과 같이 두 연립방정식의 풀이 결과가 2행 l 열
형태로 나타난다．
日如

T毗

V沌w

鈿蜘

晦p

O 니 兮 8 g> 芬 g} , 咬 , 『：

入1

U/

「＼

．

/”

「

「」

//\7／

L\

j

니

三b 會 ,

:

Ree印

그림 14-11 스코프 창 걸과

422

PART 04. Sim메nk설계하71

C

F

7

口

a

In

T=10.OO0

LESSON

02

2차 미분방정식 人불링크 모멜 설겨后F71

] 차 미분방정식을 계산하는 시뮬링크 모델을 기초로 2차 도함수를 포함하는 2차 미분방정식의 해를 계산하는 시뮬링크 모델
을 설계해보자. 또한 2차 미분방정식으로 나타내는 단순 조화 진동자의 운동 방정식과 감쇠 단순 조화 진동자의 운동 방정식
에 대한 시뮬링크 모델을 살펴보자，
Keyword

I

I 단순조화 진동자운동 방정식 1 감쇠 단순조화 진동자운동 방정식 1

감쇠 단순 조화 진동자

감쇠 단순 조화 진동자（damped simple harmonic oscillator)의 운동 방정식은 단순 조화 진동자
(simple hamn均nic oscillator）의 운동 방정식에서 속도에 따라 비례하는 감쇠 부분 x를 더한 형태로 나
타낸다．

M＋加 1 qde.m

1 예제 14- 4 1

다음과 같은 2차 미분방정식의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이따1 시뮬레이션
실행은 0초부터 8초까지 진행한다．
)(t) +2j (t) +y(t) =O, y(o) =10, j' (o) =o

!11.
liii겸
지식

제시된 식은 다음과 같이 다시 쓸 수 있다．
y (t) = -2j'(t) -y ()

풀이

(-

(})+(- (})(})
1)

y=

2)

죄측의 2차미분형태胴분을두 번 실행한후瞻라스 변환변수｝을 적분기호 대신사용하면 다음과
같은 형태가 된다．

OSum 블록을 설계 창에 생성한다（[Comm이ily Used Blocksl-[Sum]).
0 생성된 Sum 블록을 더블클릭하여 [Function 미ock Para毗ters] 창을 열고 [List of signs］에 1 小를
입력한 후 回K] 버튼을 클릭한다．

CHAPTE日 ]4. 미분방정식

423

Sum
Add or subtract In口Ida. S口ec的 on日口Ithe 幻妃wing:
a) 引ring c口ntaining + or 伯r each In口ut 口ort. I t口rs口acer between
ports (e.g. .+I-I. +)
b) scalar, >= 1, specifies the number ot input ports to be summed
\Vh日n there is only 口ne In口ut 口（가t add or subtract el日ments 口nor all
네men引ons 口r one a口日c州ad 네men引on
Main

돼gnal 向thbut日a

Icon ohs口a

round

Ust 口f 쉬gns
I-

I

-

1

OK

Cancel

Help

그림 14-12 Sum 블록에 부호 지정

0 Gain 블록 2개를 설계 창에 생성하고（[Math Operations卜田ai미）블록의 이름을 각각 G帥I, Gain2
로 바꾼다. 이때 Ga血l은 y를 귀환해서 (feedback) 사용하고, G帥끄는 y를 귀환해서 人卜용한다．
0 Gain 블록 2개의 방향을 거꾸로 바꾸기 위해 마우스 오른쪽 버튼을눌러 [Rotate & Flip]＋小p Block]
을 선택한다．
0 블록 Gain1을 더블클릭하여 [Gain:]에 2를 입력하고, 블록 G如2를 더블클릭하여 [Ga沇］에 1을 입력
한다. O에서 Sum 블록의 已慨 of signs:］를 기본값 1+＋로 유지하는 경우에는 블록 Gain1의 [Gain:]
어］ -2, 블록Gair그의 [Gaii피에 -1을선택적으로 입력할수 있다．
0 Integrator 블록 2개를 설계 창어］ 생성하고（[Continuous] - [Integr毗야］) 블록의 이름을 각각
Integrator1, Integra加r2로바꾼다．
0 블록 Integra的rl의 [Initial condition:]에 l차 미분 초기 조건 0 (j' (0) =0）을 입력하고, 블록
Integra的r2의 [Initial condit油피에 초기 조건 10 (y(0) = 10）을 입력한다．
0 Scope 블록을 설계 창에 생성한다（[Sii止司-[Scope]).
O 생성된 블록을 연결한다．
디陌

Ed吐

\／낟w

D印啣

亡극｝, 呂

Diagram

닯rys片1tk口n

Asa卜115t5

" 旨昏）呻 愁 ＼多 II;:' ,

Cn巾 bIds

Help

巨3 , 力 （크 ! 幽 ,

由

團ODE

QDEI

烈
1：크

I

0

!

}

}

口

fl eqet31

甘tE{raiCr2

S口耳＞e

4
團

只
畔

朔

Gam1

a

젼

)>
R舫旬

10畔

出i1bk9ePAUt0

그림 14-13 완성된 시뮬링크모델

m m如del Coni砲uration Paran妃ters] 창을 열고 [S切rtt油e］과 囹的p time］에 각칵0.0, 8.0을 입력한다．
0 시뮬레이션 실행 결과는 다음과 같다．

424

PART 04. Sim네nk설계하71

F晦

ro이5

V卜ew

듸mulat幻n

14曲）

m

@ ' 吟（9 1> 醬 率 ! e\ ,［꾜디 f 囹，
F;

汀＝＆啣
그림 14-14 스코프 창 결과

m 2차 미분방정식의 해를 생성하기 위한스크립트 파일을 코딩한다．
然
}
t = 0:0. 01 ;8;

23 尸

이ot (t .y_t) ;

4
5
6-

+

1 -

I

기 qde.m

y_t=（따니마t) . eup(寸 ) ;
olabel ( t ) ;
이 ab미 C 奴 t) ) ;
grid;

그림 14-15 미분방정식 해의 파형을 생성하는 스크립트 파일
1iD

2개의 초기 조건을 이용하여 2차 미분방정식을 풀면 해는 y(t) = 10+ 10加 ' 이다．

四 명령 창에 스크립트 파일을 실행하면 다음과같은 그림 창이 생성된다．

그림 14-16 그림 창 결과
명령 창어냐＝크립트 파일을 실행하여 얻은［그림 14놔16］의 파형은［그림 14크4］의 결과와동일하다．

CHAPTER 14 미분방정식

425

1 예저114-占

1

다음과 같은 2차 미분방정식의 시뮬링크 모델을 설계하고 그 걸과를 스코프 창에 나타내라 ．이따1 시뮬레이션
실행은 0초부터 8초까지 진행한다．
5 (t) = 4sin3t + 2cos2t, y(0) = 2, j' (0) = 1

于丁
.

甁

주어진 식은다음과긷미 다시 쓸수 있다．
(t) = -.-[4sin3t + 2c。
s2t1
r

푿이

"

그

느

0 Sine Wave 블록 2개를 생성하고（[Sources] -圄ne Wave]) 블록의 이름을 각각 4sin3t, 2cost2t로 바
꾼다．
0 블록4sin孰를 더블클릭하여［如1plitude:］에 4, [Frequency (rad/sec) :］에 3을 입력한다．
얹n日 나a始
O내巾uta 引n日 叫a5e:
O(t) = Am口.Sin(Fr日q너＋F가tas日） + 日ias
돼n日 匈p日 d日termin日sth臼 computati口nat techniqu日 us日d. Th日
param日佃rs in the I니／sty口日5 ar日 r日lated 甘卄口ugh:
Sampi日5 口er 口日加d = 2싸기 / (Fr日qu日ncy 1 Sampi日 lime)
Numb日r of 口竹S日I samF이日S = Phas日 1 Sam口les 口日r 口erlod / (2아ti)
Us目 the sampi日＝based 引ne typ日 if num日tic눼 pr口bi日me du日 t口
running f口rlarge tim日a (e. g 口V日네ow in abs미ut日 tim日） occur.
Param日t마5
텨n日 ty口甘 Time based
Tim日（t): [

내all口n time

小J

向n베tude

B'ias
0
Fr日qu日ncy (rad/s日c):
3
Ph日5日 (rad):
0
Sample time:
0

9

團 tnt日r口r日I Vector 口arameters as ! 山

OK

] [ Canc引 ]

H미p

A口口lit

그림 14-17 Sine Wave 볼록 써nt帥게 진폭．각주파수 설정

0 마찬가지로 블록 2cos2t를 더블클릭하여 ［知rnplitude:］에 2, [Frequency (rad/sec) :］어口를 입력하고，
코사인 파형의 변환을 위해 [Phase (rad) :］에 위상 오프셋 pi/2를 입력한다．
0 사인 파형과 코사인 파형을 더하기 위해 Add 블록을 생성하고（
［卜4ath Operation可-[Add]) 더블클릭
하여 [List of signs:］의 기본값 +＋를 그대로 유지한다．
0 Gain 블록을생성하고（
［卜'ath Operations]-[(扼血］) 더블클릭하여 田air비에 1/5를 입력한다．
0 Integr毗or 블록2개를생성하고（[Cont血uous卜帥egr帥川）블록의 이름을 각칵y'(o)=1, y (0)=2로
바꾼다．

426

PART 04. SimUlink 설계하71

0 블록y,(o）日을 더블클릭하여 [Initial cond而on:]에 1(초기 조건 只0) = 1）을 입력하고, 블록y (O)=2
를 더블클릭하여 [hiiti出 condition:］에 2（초기 조건 y(0) = 2）를 입력한다．
Integrator
C口ntinu口Us내rn日 integration otth日 in口Ut 引gnal.
Paramet카S
Eo也m졔 rae日r none

r

In川톄 C口nhr的C SCUrC日： in也mel

r

mnd졔 口口nditi口n:
2
口 Urn卄 CU巾Ut
［已 S1升a口 state
口 Show sa山ra如n 口口ii
口 Show 欲a也 p（그rt
Aso山te 刎日rance:
aU幻
口 Ignore limit and r日S日twhen in日au기ng
團 Enab陌 Z日rn-cr口seine detec如n
Ste伯 Nam日 (e.g . ‘口口引h口II')

0K

9

II日Ip

Can口톄

[

Pd口ly

'

그림 仙너8 Integrator 블록 y(0)=2에 초기 조건 설정

0 Scope 블록을설계 창에 생성하고（[Sinks卜田cope]) 블록의 이름욜y (t)로 바꾼다．
0 생성된 블록을 연결한다．
F爬

Ed作

\/1am ［거SF啣

D治gram

Simul欲幻S

匈｝ , 冒 기． 少 났 渭믐 口 ,

Ana腑心

伽巾 b마5 卜倒p

' 呻텍(

聆 . 回，》》 凹 , 芒．計

00E2

E1

E르
I
［그

回QDE2

;

!

鼻1口＋
七H
:"'
"
""
""

區才그 枷

E土
齒
Rea

100%

vanableStepAuto

그림 14-19 완성된 시뮬링크 모델

四 ［卜(odel Configuration Paran妃ter司 창을 열고 [Start 血ne］과 田的p time］어］각칵0.0. 8.0을 입력한다．
q1 시뮬레이션을 실행하면 다음과같은 결과를 얻는다．

CHAPTER 14 미분방정식

427

印e

T出＄

m曲

$m出a缸미1

시

H甘口

宰 , 兮 (3 吟 S 믐亨 , 텍 , ［끄 , I 囹 ,

T=8 000
그림 14-20

스코프 창 결과

M-FiIe ! sim h osc.m
단순 조화 진동자의 운동 방정식은 다음과 같은 2차 미분방정식으로 나타낼 수 있다． 여기서 rn은 질량
(mass), k는 용수철 상수（S剛ng constant)이다．

질량이 2이고 용수철 상수가 8일 때 0초부터 10초까지 진동하는 시뮬링크 모델을 설계하고 그 결과를 스코
프 창에 나타내라.2차 미분방정식의 초기 조건은 각각 工（0) = 1. k(0) = 00다．
용수철의 운동은단순조화운동의 가장대표적인 예이며, 주어진 식은다음과같이 다시 쓸수 있다．
=

(
)

H工

풀이

缸
l2

1m=n
.
dIt겸
지식

0 Gain 블록 2개를 생성하고（[Commonly Used Block引小田ai미） 첫 번째 블록의 이름을 Mass로 바꾼
다. 블록Mass를 더블클릭하여 [Gait비에 -1/2 (m =2）를 입력한다．
0 두 번째 블록의 이름을 Spring으로 바꾼후마우스오른쪽 버튼을누르고 [R야砒e & Flip]-[Flip Block]
을클릭하여 입출력 방향을 변환한다. 블록 匈州ng을 더블클릭하여 [Qaii피에 8(k= 8）을 입력한다．
0 Integr毗or 블록2개를 생성하고（[Cont血uous卜帥egr汕川）블록의 이름을 각각x '(0) '0, x (0)=1로
바꾼다.
0 블록 x '(O)=O을 더블클릭하여 [Initial condition:]에 0（초기 조건 文（0) = 0）을 입력하고, 블록
x (0）日을 더블클릭하여 [Initial condition:］에 l （초기 조건 玎o) =1)을 입력한다．
0 Scope 블록을 설계 창에 생성하고（[Sir水司-[＆叩司）블록의 이름을x (t)로 바꾼다．
0 생성된 블록을 연결한다．

428

PART 04. Simulink 설계하기

F如 帥t

VIew

O탸啣 ［加gram

囹 ! 目 ／尸 L口 h{ 踞

Simulat卜m}

如的5仁

"呻 텍8

Code

b뇌s

1P !

He巾

囹 ,,, (3 r 硅自 ,

0053
r

團0DE3

e

烈

老

토크
4

'잃

'캄

'투

回
i回
自：

［그

;

I'

曲
>>
Rea旬

100%

VanableStepAuto 1

그림 ]4-기 완성된 시뮬링크 모델

0 ［卜如del Conf培uration Paran妃ters] 창을 열고 [Start time]과 [S幻p 山ne]에 각각 0.0. 10.0을 입력한
후 시뮬레이션을 실행한다．
Ale

T어必5

Vi酬

SimuL曲沁n

Help

1

O 기 也 8 吟 斗 i 各 나 目, ［꾜 니 f 國 ,

그림 ]4-22 스코프 창 결과

oY축을조절하려면 스코프창에서 마우스 오른쪽 버튼을누르고 [Configuration proper出S...］를클릭한
다. 다음과 같은 冬巾］ 나타나면 [Y小mits (Minimum) :］어］ -1.2, [Y-limits 小4aximum) :］에 L2를
입력한다．

口 Show leg日nd

團 Show grid

巴 F기口t 引en계s an magnitude and 口hane
V-limits (Minimum):

-1.2

V-un卄Is (I너asimum): 1.2
V-lab이：

그림 14叫23 스코프 창 최적화

CHAPTER 14 미분방정식

429

스코프 창 설명

수학적으로 제시된 문제의 경우 2차 미분방정식의 일반적 해는 다음과 같다．
工（t) = C1sin（刃。t+ C2cos口)ot
2개의 초기 조건을 이용하면 상수 Cl과 C2는 다음과 긷다．
工（0) = C2 = 1
t (0) = CK2J0 = 0

.'.C= 0

그러므로 工（r) = cosw。
t이다．
각주파수와주기는 다음과 같이 계산할수 있다．
2포（t) + 8工（t) = -2w긍cos（刃。t+ 8cos（刃ot = 0 - (U0 = 2
m, 2,r
/ = 二＝
+ = 7r
IL'0
［그림 14크2］는주기 兀 ==3.1415로 반복되는코사인 파형을 보여준다．
0 시뮬레이션 결과를 검증하기 위해 다음과 같은 스크립트 파일을 코딩한다．

II 읽m_h_oscm IC 擘’

5-

4-

1中
2戶
3-

寸

7-

6

！口

t = 0:0.Ci:lO;
,l_t=Cos（小t) ;

ptot(t, x_t) ;
aICls(10 10-1. 2 1. 21) ;
1

비abel ( 't ) ;
끼ab이 ( 'i (t) '. rot . 1羽C) ;
grid or, ;

그림 14-24 단순 조화 방정식 해의 파형을 생성하는 스크립트 파일

四 명령 창에 스크립트 파일을 실행하면 다음과 같은 그림 창이 생성된다．
F的 E出t

View

=) 二 a

코

moe戊 了oolo
臣

',

Des났야） Window

, 'L'7 自 ｝侄l /

He巾

' 邑 口 匠크

1 口

그림 ]4-25 그림 창 결과

명령 창에 스크립트 파일을 실행하여 얻은［그림 14-25］의 파형은［그림 14-22］의 결과와동일하다．

430

PART 04. Sim메nk설계하기

M-Fie 1 dam h osc.m

1 예제 14- 7 1

감쇠 단순 조화 진동자의 운동 방정식은 다음과 같은 2차 미분방정식으로 나타낼 수 있다． 여기서 /7 > 0인
경우의 p를 감쇠 상수佃an가긔ng con없ant)라고 부른다．
n伐 +／伉 + 缸 = 0
질량이 2, 용수철 상수가 8, 감쇠 상수가 0.2일 때 0초부터 10초까지 진동하는 시뮬링크 모델을 설계하고 그
결과를 스코프 창에 나타내라.2차 미분방정식의 초기 조건은 각각 工（0) = 1, (0) = o 이다．

；而

주어진식은晤과긷미다시쓸수있다·

지식

戈＝글似＋帥
OSum 블록을 설계 창에 생성하고（[Commonly Used Block司小囹urn]) EL慨 of s培ns:］의 기본값 1++
를 그대로 유지한다．
0 Gain 블록 3개를 생성하고（[Commonly 小ed B뇨：k司-[G曲ill) 첫 번째 블록의 이름을 Mass로 바꾼
다. 블록Mass를 더블클릭하여 [Gain:］에 -1/2（加 = 2）를 입력한다．
0 두 번째 블록과 서］ 번째 블록의 이름을 각각D跏ping, Spring으로 바꾼 후 마우스 오른쪽 버튼을 누르
고 [R아就e & Flij小［Flip B如ck]을클릭하여 입출력 방향을 변환한다．
O 블록 Da呻ing을 더블클릭하여 [Gaii비어］ 0.2（끄 = 0.2）를 입력하고, 블록 Spring을 더블클릭하여
[Gain:］에 8(k= 8）을 입력한다．
0 Integrator 블록2개를 생성하고（[Continuoi刈小[Inte얍毗아］) 블록의 이름을각각x'(0)=0, x (0)=1로
바꾼다．
0 블록 x '(0)=0을 더블클릭하여 [Initial condition:］에 0（초기 조건 k(o) = 0）을 입력하고 ，블록
x (0)=1을 더블클릭하여 [In消카 cond也on:］에 l （초기 조건 工（0) = 1）을 입력한다．
0 Scope 블록을 설계 창에 생성하고（[Sink司-[Scope]) 블록의 이름을x (t)로 바꾼다．
0 생성된 블록을 연결한다．
4

iait

Me나

D匕하ay （거a9am

圓, 因

듸m너at自fl

Anaty5匕

Code 自oI5

He巾

" 呻 咽 出／ 1P ( 囹 ,，》 U , 芯打

鸚 守,

GD든4
e

Y
回ODE4

烈
툐크

0

>

日

}

口

4
四

骨

"
"

'

，규

푤이

E口
由
力
肛a旬

100%

＼似的뇨幽叩加to

그림 ]4小而 완성된 시뮬링크 모델

CHAPTER 14. 미분방정식

431

0 [Model Configuration Paramete心］창을 열고 [S切rtt恤e］과 囹top tin妃］에 각각 0.0과 10.0을 입력
한 후 시뮬레이션을 실행한다．

m; Too놈 \hew 듸mu治tion Help
@ '

兮 G) 非 包

午'

1

奴 ' 띠'

罕 臼'

T10 000

R

그림 14- 27 스코프 창 결과

四 Y축을조절하려면 스코프창에서 마우스오른쪽 버튼을누르고 [Configuration proper如S...］를클릭하
여 창을 연 후 [Y-1油its 小4ii血ium) :］에 -1.2, [Y小mits 小4aximum) ］에 1.2를 입력한다．
스코프 창 설명

수학적으로 제시된 문제의 경우 2차 미분방정식의 일반적 해는 다음과 같다．
x( t) = e冽／' ' [C1co5刃。t+ C2 sinw。
t]
초기 조건 加 = 2, 끄 = 0.2를이용하면샹수C，과C2는다음과같이 계산할수 있다．
工（0) = C' = 1

i (0) =1孚아w。G= 0 ·'· C2＝뽕흐
그러므로小戶叫呻的＋뽕뇨wet］가된다．
2차 미분방정식의 해를 이용하면 각주파수와주기는 다음과 같이 계산할수 앴斗．
2戈（t) +0.2 (t) + 8工（t) = 0 나 (0o ;= 2
2兀
m
/ ＝二 =;H = 兀
uJ0

［그림 14小27］의 파형은주기 7r = 3.1415로 반복되면서 진폭이 점점 감쇠되는 형태이다．
0 시뮬레이션 결과를 검증하기 위해 다음과 같은 스크립트 파일을 코딩한다．

432

PART 04. Simulink 설계하71

+'

:

I damh_osc.m ?:
1-

45-

t = 0:0.21:10;
x_t=eKp(-0.1巧＋t) ..(cos(2士t）山．02타引n(2+t) ) ;
plot (t, x_t) ;
axis(10 1 0- 1 . 21. 21) ;
clabel ( 't ) ;

5-

비aS미 C, 奴t) . rot . 弱C) ;

7 -

grId on;

2 3-

!m

그림 14-28 감쇠 단순 조화 방정식 해의 파형을 생성하는 스크립트 파일

e 명령 창에 스크립트 파일을 실행하면 다음과같은 그림 창이 생성된다．

그림 14-29 그림 창 결과

명령 창에 스크립트 파일을 실행하여 얻은［그림 14-29］의 파형은［그림 14-2刀의 결과와동일하다．

CHAPTE日 14. 미분방정식

433

=Li
+

+--

I

i

나卄

1.

4--卜 나 나

!

i

1

i

1卜i i ! 4 } ! !
1

.

i!

I

I

!

! 1

［丁

4-

I

!
.

!

i

4

1

-

-

＝二二
나나

CHAPTER

15

나H

1

t

i

뇨

삼각함수
1니

日寸

1

口

H

尸

ji1iH; 1
나

H구 나

CONTENTS
LESSON 01 사인 파형 이해하기
LESSON 02 코叭f인 함수 생성하기
LESSON 03 정현파 응용 설계하기

!

LESSON

01

사인 파형 이해하기

사인 함수로 주어진 일정한 진폭의 주7쩍 진동을 매끄러운 사인 파형으로 그리는 데 사용하는 Sine Wave 블록, Mux 블록에
대해 알아보자．
Keyi月ord

I

1 진폭

각주파수 1 위상 1 편향 각도 1

진폭

진폭（ampi如de）은 사인 파형의 크기가주기적으로 변할 때 평형 상태를 기준으로 양의 최대 크기 또는
음의 최대 크기 절댓값을 말한다．

I

각주파수

각주파수（radian frequency）는 단위 시간에 사인 함수가 이동할수 있는 각을 라디안으로 표시한 값으
로 단위는 rad/s이다．

I

위상

위상（phase）은 주기적으로 반복되는 파형의 한 주기에서 시간이 0일 때 사인 함수의 출발 위치를 결정
하는각을말한다．

I

편향 각도

편향（bias) 각도는 사인 함수어］일정하게 더하거나 빼는 상숫값의 각도를 말한다．

1 예제15너 1
다음과 같은 사인 파형의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라． 이따1 시뮬레이션의 실
행은 0초부터 ]0초까지 진행한다．
玉（I) = sint
f2(t) = 2sin1
f (t) = sm21

436

PART 04. Simulink설계하71

풀이

0 Sine Wave 블록 3개를 설계 창에 생성하고（[Source引-[Sine Wave]) 블록의 이름을 각각 fl (t).
f2(t), f3 (t）로바꾼다．
0 블록fi (t)를 더블클릭하여 기본값으로주어진 [Amplitude:］의 l , 田requency (rad/sec) :］의 l을그때1
로유지한다．
듸fle Wa比
Ou如uta 引n日 나aye
O(l) = 向n口.Sin(Freq.t.Phane) + 日las
듸ne 勺口a del마mines th日 C口m口나t削onal日chniq나e 니ned. The
paramel日rs in the two 勻pes are r日lat日d lhr口ugh
Sanrtyles F｝日r 口日H口d = 小비 / (Fr日quen口p 1 Sam비e 寸m日）
Number ci 口ifs日I Sam口1日S = Phas日 1 Sarnpl日a per 口crIed / (2.口1)
Use the sampi日based 틔n日 ly口e 卄 numerical 口r미이日ms du日 幻
running I口rlarge 0mes （日S 口V日ci口나 in abs口lute time) 口noun
Param日地r5
미ne ty口可 1 Time baa日d

!

Time (U: Use 針mu冶t由0 甘m日

!

thnpiitude
]
Bias
0
f누eguency (md/s日ci
1
Phae日 (r日d)
0
Sample rIm甘
D
回 ni日rpratS日ctsr 口aram日tare as卜O

OK

0

C邸旽： mlie也 , 塑므IC 「

그림 15너 기본 Si陀 Wave 블록 설정

0 블록 f2(t)를 더블클릭하여 [Amplitude:］에 2를 입력한다. [Am州tude:］의 기본값 l을 유지하는 경우
G恤 블록을 연결하여 [Gain:］에 2를 입력해도 동일한 결과를 얻을 수 있다．
돼ne 叫aye
O나巾cia 틔ne way日
O(1) = Mr口.Sin(Freg*t.Phas日）+ 日泊8
미ne lb口ed日佃r例n日e lb日 C0m口U伯t幻nail日chnlgue us日d. The
param日t日rs in the 1w口 lb口es are related through
Sompl日日 Per 口日nod = 2.pi / (frequency - Sam이日 rIme)
Numb日rot o如甘 samples = Phase. Sam히as 口er 口eli口d/ (2까M)
Uee lb日 Sam비c-bee日d 늬n日 typ日 if num日nc비 口r口blems due to
running 幻r iarg日 Pm日8 （已9, ouertl口wIn abse山伯 rime) occur.
Param日t酊＄
텨ne ICC）日： Time baa日d

,

!

Tim日（0: [Pica引m내日b口n Pm日

긔

Mr口litude:
2
Bias:
S
Frequency (r刊屈日C):
1
Phaee (red)
0
S日m미a rIme
0
團 mnIenr玎日tu日clor 口enamelers as卜O

e

OK

] mi

！尸戶而n

q口口Ii,

그림 ]5丑 Sine Wave 블록 f2(t）에 진폭 변경 후 설정

CHAPTER 15 삼각함수

437

0 블록t키t)를 더블클릭하여 [Frequency (rad/sec) :］에 2를 입력한다．
텨ne 나a四
0u巾Ut a 늬n日 \sac甘
Oit) = knptSin(fr日qd旴개as日）+ S冶S
Sin日 typ日 determines th日 computatic그na나echniqu日 us日d. The
口aran,eters in theta사 勻pes ar日 r日lated hr口ugh:
Sample日 口er 口日nod = 2*pi / (Frequ日ncy 1 Sam이日 甘me)
Number 口tot冶日tcamp)日S = Phas日 1 Sampi日sp日r 口日r幻d/ (2가ci)
Us日 the samp)中based 늬ne typ日 If n니merical pr야旭ms due to
running 伯r 冶rg日 times (e.g. cv日nit（그win abs미Ut日 time) occur.
Paramet마5
미ne typ甘 Tim日 bas日d

t

lime (0: USe 引mu冶don 出S日

!

Ps 口It山de:
1
日治S:
U
Fr日quency (rad/s日c)
2
Phase (red)
U
Sam비e time
U
望 Interpr日to日clor 口aramet日rs as 卜 ［)

뇩夕

16 K1J [ Canc日1 1 H미p

r 如口匈

그림 15小3 Sine Wave 뷸록 仍(t)에 각주파수 변경 후 설정

0 다양한 신호블록의 결과를하나로묶는Mux 블록을 생성한다（[C아flU끄only Used Block司H小4u川）.
0 入4ux 블록을 더블클릭하여 a沁mber of inputs:］에 3을 입력하고（기본값은 2) [Display optiot비을
signals로바꾼후回K] 버튼을클릭한다. 기본값인bar를그대로사용해도상콴없다．
1너us
Mu州pies sca나 口ry日C幻r 引gna陌．
Parame也rs
Number Olin口니ts:

3
D冶plait op如n 引gna冶

Canc日1

AP미y

그림 15닉 Mux 블록에 입력 단자 3개 설정

0 signals 형태로 변환한 Mux 블록은 마우스 왼쪽 버튼으로 선택한 후 네 모서리 중 한 곳에 커서를 놓았
을 때1 대각선 형태의 화살표가 나타나면 크기를 조정할 수 있다．
0 Scope 블록을 설계 창에 생성한다（[Sii出司-[Scope]).
0 생성된 블록을 연결하여 모델을 완성한다．

438

PART 04. S)m메nk설계하기

F加

Ed注

\lie네

마splay

囹, 圄

Diagram

듸mulation

寸 납 琵 每,

Analys何

Code

自이S

He巾

" 呻 」姻 四 m> / 因 ,，》 回 , 區自 ,

미N上Ikl
團引N페kl

!

Al

！확

므

뿌

L녘

單

回
［그

m
LJ1
mq

m

""'"

日，

J "

1'

8

出
力
陌向

l며｝%

出riableStepAuto

그림 15小 완성된 시뮬링크 모델

@ 시뮬레이션을 실행하기 전에 설계 창의 메뉴 표시줄어꺼 [Simulation] 메뉴를 클릭하여 [Model
Configuration Paran妃ter可 창을 열고 [Start 山ne］과 囹top tin蝴의 기본값 0.0과 10.0을 그대로 유지
한다．
q1Scope 블록을 더블클릭하면 스코프 창에서 사인 파형 3개의 실행 결과를 확인할 수 있다. 실행 결과를
최적화하기 위하1 마우스 오른쪽 버튼을 누르고 [Cos小guration properties...］를 클릭하여 창을 연 후
[Y-l耐ts (Mm油urn):］에 -3. [Y-limits 小4aximum) :]에 3을 입력한다．
F朴e

T的5

View

S什mutation

He巾

1

@ r 心 (9 11> 心 各 , （왁 , ［꾜 r f 囹 ,
4러

Re的y

T.10 000

그림 15田 스코프창결과

신호 五(t) (가운더］파형）는 진폭 -1부터 1 사이에 주기 2ir 동안 반복되는 사인 파형의 기본을 보여준
다. 신호 f2(t)（위 파형）는 신호 玉(t）에 비해 진폭이 두 배 늘어난 -2부터 2 사이에 주기 力r동안반복
되는사인 파형이고, 신호 玉(t) (아래 파형）는 신호 玉(t）와진폭은동일하지만각주파수가두 배 증가
하여 주기 2兀 동안 사인 파형이 두 번 반복된다．

CHAPTE目 15 삼각함수

439

1 예工II 15- 2 I
다음과 같은 사인 파형의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라． 이때1 시뮬레이션의 실
행은 0초부터 ] 0초까지 진행한다．
玉（t) = Sint
f4 (t) = sin(t+ 30O)
fi (t) = sin(t+ 30O) _45O

=6i

0 Sine Wave 블록 3개를 설계 창에 생성하고（[Sources]-[Sine Wave]) 블록의 이름올 각각 fi (t),
f4(t), f5 (t)로바꾼다．
0 블록 fi (t）를 더블클릭하여 기본값을 그대로 유지한다．
0 블록f4 (t）를 더블클릭하여 [Phase (rad) :］에 위상pi陌을 입력한다．
미ne Wave
Output a 引ne 낵ave:
O(t) = Nn口t텨n(Freq小Phase) + B油5
돼ne 勻口a determines the computa甘口nat technique used. The
口arameters in the two ty口es are r日tated 小ro四h
S日mt기日5 口er 口eriod = 2.pi / (Frequ日ncy 1 Sam口te time)
Numb日r 口fotis日t 日am히es = Phase 士 Samples 口er 口erlod / (2町)i)
Use the sam口e七ased 引fle typ日 汗 n니mer比톄 pr口blems due to
running 化r larg日 times (e.g. overft（그win abs미내e 甘me) occur.
Param日t마S
듸ne typ甘 Tim日 based

!

lim日 (t): Use 히mulati（기l 打rr｝日
mpli山de:
1
Bias:
0
다equency (rad/sec)
1
F꺼日se (red):
pV6
Sample time
0
團 Inter口ret vector 口aram日t마S aS卜U

8

OK

Canc日I

Help

A口口如

그림 15-7 Sine Wave 블록 f4(t）에 위상 설정
UI>

주어진 위상은 도（degree) 단위인 30' 이지만, 위싱을 나타내는 매개변수에는 라디안을 입력해야 하므로 라디
안으로 변환된 p116을 입력하는 것이다．

0 블록 f5 (t）를 더블클릭하여 [Bias:］에 편향 각도에 -pil4를 입력한다．

440

PART 04. Sim메nk설계하71

돼p日 Way日
Output a 引ne 나目v9
0(t) = Pn,p.Sin(Frect*t+Phase) + Pias
미ne type de也r씨nes the corn口utati口nd1 technlqu日 used. The
口arameters in th日 佃0 ty口cc are related through:
Samples 口er 口crIed = 2가M / (Fr日quency 1 Sample 打me)
Number 口to加et sam비日5 = Phas日 t Sam비as per period / (2畔）I)
Us日出e sample-based 벼n日 type 汗 numeric톄 pr口bi日ms due 幻
running 幻기a円e 甘mes (e.g 口vert七叫 in abs이ute b me) 口ccur.
Parame也rs
미n日 押pe: Tin伯 bas日d
TIm日（出 t始日simul日如ntim日

V]

M,pl仙d日：
1
B洽8:
-t比／4
Frequency (rad/sec):
1
Pha日日 (rad):
pb'5
믐叩비

' " ' "『

1l11
주어진 편향 각도는 도 단위인 -45' 이지만. 편향

團 Interpret vector 口cram日ters 日S ] 七

9

[

OK

Cancel

JL

]

Help

각도를 나타내는 매개변수에는 라디안을 입력하뺘
하므로 라디안으로 변환된 가町4를 입력한 것이다．

Apply

그림 15田 Sine Wave 블록 而（t）에 편향 각도 설정

0Mux 블록을생성한다（[Commonly Used 미ocks] -［卜Ii狀］).
OMux 블록을 더블클릭하여 囚Un小er of it叩uts:］에 3을 입력하고 [Display option:］을 signals로 바꾼
후 回K] 버튼을 클릭한다．
0 Scope 블록을 설계 창에 생성한다（[Sink引나Scope]).
0 생성된 블록을 연결하여 모델을 완성한다．
日Ic 日lit

昆' 目

tee나

0螂啣

[Xa9甘am

듸muta作)5

』 :> 會 雕 r

An카吟士5

Codc

勿이＄ H帥）

"呻 ＜也 @ 聆 ,

巨크，,, U , 邕自，

미N_테k2 {
e
回미N떼k2

!

風

므
E르

回
［그

Fm

甲
四

口

mm,

m

［月

甲

齒
>>
Re的r

100%

Variab1eStepAuto

그림 15四 완성된 시뮬링크모델

CHAPTE日 ]5' 삼각함수

441

0 시뮬레이션을 실행하기 전에 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 ［入4ode1
Configuration Paran妃k江S］창올열고［Start曲e］과［Stop time］의기본값0.0, 10.0을그대로유지한다．
@Scope 블록을 더블클릭하면 스코프 창에서 사인 파형 3개의 실행 결과를 확인할 수 있다. 실행 결과를
최적화하기 위해 마우스 오른쪽 버튼을 누르고 [Configuration properties...］를 클릭하여 창을 연 후
[Y小limits 小4inimum) :］에 -2. {Y-limits 小4aximum) :]에 2를 입력한다．
日le

祀毗

V1eW

듸mul硼kn

U川p

@ 나 也 0 肛 SI 各 니 q d꾜 니 I 國 ,

Re月小／

그림 佰너0

T.loa凹

스코프 창 결과

신호 五(t) (가운더｝ 파형）는 진폭 크부터 l 사이에 주기 2兀 동안 반복되는 사인 파형의 기본을 보여준
다． 신호 五（t)（위 파형）는 신호 五（t）와 진폭은동일하고 위加1 죄측으로 증＝30 ' (- 0.5236）만
큼 이동한파형이고，신호玉（r)(.忙卄 파형）는신호玉（r）에 비해 진폭은.빼로 편향각도증＝450
(- 0.7854）므培이동하고위상은신호五（t）와동일하게죄측으로증므搢이동한파형이다．

442

PART 04. Simu加k설계하'I

코사인 함수 생성하'I
Sine Wave 블록을 이용하지 않고 코사인 파헝을 생성하는 From F陀 블록에 대해 알아보고 Co듸ne Wave 블록과 To F陀
블록을 이용하여 데이터를 생성하고 그림 창에 나타내는 방법을 익히자．
Key＼사ord

I

I From F陀 블록 I To 테e블록 1

From File 블록

From File 블 록 을 이용하면 둘 이상의 행으로 이루어진 행렬이 입력된 스크립트 파일에서 데이터를 읽고
출력할 수 있다．

I

To File 블록

입력할 데이터를 MAT 파일어］저장한다．

M＋沁 I MyCo引n.m

I 예玉II 15- 3 I

Sine Wave 블록을 이용하지 않고 진폭이 2인 코叭r인 파형의 시뮬링크 모델을 설계하고 그 결과를 스코프
창에 나타내라 ．이따1 시뮬레이션의 실행은 0초부터 10초까지 진행한다．
;:

1i 'JI

0 From File블록을설계 창에 생성한다（[Sources］ 田rom File]).
0 코사인 파형올 생성하기 위한 스크립트 파일을 코딩한다．
畇Coi衿月I x
1234S-

+

t = 0:0.01:10;
d = cos(t) ;
x = Cud) ;
ts = tlueserles(x(2:endJ :),x(1, :fl;
saye( llyCosine , ' ts ' 尸 -v7, 3 ') ;

그림 15-11 코사인 파형을 생성하기 위한 스크립트 파일

0 명령 창어］ '入4yCosine.m' 스크립트 파일을 실행하면 현재 사용 중인 MATLAB 작업 공간어］ 자동으로
MATLAB 데이터 파일 'MyCosine.mat'가생성된다．
0 From File 블록을Gain 블록과Sc叩e 블록에 연결한완성 모델은다음과같다．

CHAPTE日 ]5. 삼각함수

443

F礁甘

帥t

vh附

D떠出1y

Di呵曲） Simulation

昆 ! 目 뇨」 [，」 」니1旨믐 毋 ,

Ma卜Is忖

CO巾 bm트

" 呻 왜1 ＼브 昑 !

F妃iP

匹 H ({) , 幽 ,

COS5rom 1
團Co요加m

二

r

臣｝

k:r 卜따妾？

目

團
團
口

E口

臼
Re叫r

V늠flata므StepAuto

lm戊

그림 15-12 완성된 시뮬링크모델

0 From File 블록을 더블클릭하여 [Source Block Parameters] 창을 열고 [File name:］에 MyCos血e.
Er也t를 입력한후 回K] 버튼을클릭한다．
From 日1日
Read data va山cc from a variab洹 in the s口ecifi日d MAT섀沌．
The data values may be specified in MATLA日 tlmeserles or matrix 幻rmat
MATLA8 tim日sen日s may b日 us日d 幻r any data typ已 C아lt口laxity, or 비men引ons. T口 幻ad 'if,日 bus
늬gnal, use a MATLAB structur日 小at matches if,日 t기is 네日rorchy. Ea나）leaf otth日 structure must be a
MATLAB timeserles object
Maths 幻rtnat can be 니sed only 伯r vector』如U너C, flOflC口m1뇌日X 引gna怡 Each c（그나nn of the matr似
must have a time stamp in the first row and a vector containing the corresponding data sample in the
a니bseguent ro낵5
텨tn네ttk lncr日mania的 reads data from MAT-file台 口tver引口n 7.
士五峀1

Th日 MATLA日 卄tneseries and 引r니C仙rca 口I timeseries must be saved in卜IAT섀旭5 of ver引on 7.
Param甘바S

回［團

테e cam可 MyC口引ne.mat

[

Output data type: Inherit auto
Samt기日 fime (-I 佃r inher相d):
0
Data estr日polat向n be幻r日 加引 data 口이nt: 나near estra口olation
Da伯 intert）口lation 叫刊hin time range: Unear int日r）미削口n
Data 日strap口lati口n at冶rlast datat兀,irt 니0日ar 日）,trap이at由n
［그 Enab也 zer小cros引ny detection

OK

Cancel

帥비V

그림 15-13 From F陀 블록에 데이터 파일 이롬 입력

0 설계 창의 [View卜[Model Explore日-[Model Ex히orer C出＋H] 메뉴를 선택한후From File 부분을
클릭하면［그림 15크3］과동일한 정보를 다시 보여준다．

444

PART 04. Sim메nk설계하기

듸汁日rCon拍M!

Contents of: COS..Frcm 化nly)

darnS

Saonoe Black P010口elero. From File
From File
Oesd dots o이ueo Iron eoarloble In the Specified MAT-Ole

Ia

器

Co仙mcvi口叫 蜘魚區丘而瓦引 Sho나D日folio 7019口bloc))引

00叫in O바U

미ooblyp, Oo山af0lypeSfr

心 Model 나口rhopac日
l

Conltguna000 (Ace

目

Code for CO요Front

MATLAD bIn日anti日smayb亡 U3日dfor soy data ty口e』00m口1日刃to, 口rd,oen引0n1.
To 伯ad the buooion바 U如 a MATLAD efruot山口 that matchao Ore bus
hierarchy. Each lest of the n甘uc tire oust be OMATLOD 5000edeo obiect

(g) advice for COS_Fnom
0

From File

什edmta 비usa may be operA日d In MA孔AD 亡me3eneS 口r0000 把rtnst

FnomFile

Inherit au切
InhetiC Inherit 너aintern비 n

0

3山n

二쾨；」

{

Scope

Scope

Matrix formal coc be used only for 000tot doOb也 n0n口000plex 시00씨o. E口나）
column Of the may10 ount harm acme stomp 10 the first roo 00000ector
000t시nlng the coeeapoodicg dots soirrpie in Ore subsequeot coos

[]

듸mulink in口remmflf씨四 reads data from MAT-files Of ocr引On lb
기e MATLAD 甘meserlea and structures of bmneoerles most be eared In MAT
2100 of oen시on 7.3
p0000,口t可1

固團 "

F加 name: MyCosin已nat
Out口ut data type:

InSeCt mute

San,미e hm日（너 for Iflhortt日d)
0
Data aofrapoiaf on be化ra 伽針 da뇨 P叱t 山naar 口Ouapola如n
Data icterpola0on aithin One rorroe

Liceooicl5tp이02口n

Data eofrapolsbon after last data point ! Ucoor ootrapol00口0
巴 Enab比 2er0Cr01引no detechon
卜

沚蜘三斟垂嚼脚m岫蜘社쓰늬
Search ReSOlfo
Content,
t

今

r 竺竺뜨J r

yelp

1

040D10

그림 15-14 생성된 모델의 세부 내용 살펴보기

0 小4어奴 E사加rer] 창에서 Model M幻rkspace 부분을클릭하여 [Data source:］를MAT-File로 바꾸고，
[File name:］에는 저장되어 있는 'MyCosii妃.mat'의 경로를 설정한다．
O[ R帥iitialize from Source] 버튼을클릭하고 열려 있는［卜4叱el E사加rer] 창을닫는다．
器

B｛畔虹虹撫融冊矗出泛 Show Doloils

Boone
固

F叭Cr C口nfomfi三

Content, of COS. From士 佃0(y)

C이umm Visa

7019 曲他내引

Mad이 나aebapaoe
字누

Otto source

0山세r 000,4

미口okTy口I OutDo佃lypmOtr

나口tbspace data

小的 枷如paOe+

蟲 Com0gOratiOn (A口t卜

MA丁＋Is

File name: OWcmu快1O xcumss to甘斗OATLAD咐MyCo引n已ma
Os蜘b帥as from SoucOo

Brolsom ,.r

5mme to Source

目Cods ton COO_From
0

Adoice ton COS_ynore

0

From File

013시n
0

500pe

Contents

Model mrgonento (for rnlmrsncing thit model)

yr그mplte

Inherit auto

1뇨in

ImberIt Inherit 니B intann미 P

[1

[1

Sb0口e

r

管琶騎特nn

i

ReVert

1

Ho巾

그림 1千15 생성된 데이터의 작업 경로 설정

0 시뮬레이션을 실행하기 전어］ 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 [Model
Configur師Lon Parame把rs］창을열고［Start time］과毆op恤ne］의기본값0.0, 10.0을그대로유지한다．
四 Sc叩e 블록을 더블클릭하면 실행 결과를확인할수 있다．

CHAPTER 15. 삼각함수

445

再駟 汀O幽

vi曲

5km出哺k마1 卜岫p

1

心 니 寸 @ 吟 1 i 各 n目, ［꾜 ' f 囹 '

1.10000

由1H1y

그림 15-16 스코프 창 결과

i 예저115- 4 I
［그림 15-12］에서 From 대e 블록을 제거하고 Co엷ne Wave 블록을 사용하며, Scope 블록을 제거하고 To
테e 볼록을 사용하는 시뮬링크 모델을 설계하고 그 결과를 그림 창에 나타내박 ．이때1 시뮬레이션의 실행은 0
초부터 10초까지 진행한다．
系1

0 ［그림15크2］에서From File블록과Scope블록을 ' Ii거한다·
0 Cosine Wave 블록과To File 블록을 설계 창에 생성한다（[Sin蝴나To File]).
O 생성된 블록을 연결한다．
F晦

Ed吐

\1kw

DLSE片ay

(거a1ram

Simulat卜on

琵 心,

囹, 回

Analysis

C的e

k）이O

" 呻 唾 @ q1> .

H叫p

Ed ,,, （녑j , 筐自 ,

:;

g[}

S_

!

To

回CO

COSnTo

封H}>

，汭Os-니

回
i月
［그

[m

幽
Ready

l仗朕

＼加able吼po鈿甘e n

그림 15-17 완성된 시뮬링크모델

0 To File 블록을 더블클릭하여 [Sink 미ock Parameters] 창을 연다. [File name:］에 Mytofile.mat,
[Variable name:］어I cos_out을 입력하고 [Save format］으로Array를선택한후 回幻 버튼을클릭한다．

446

PART 04. Sim네nk 설계하71

To 日le
lncr日menta向ow陀data in幻a varlab泊n the s口ecffi日d MAT-file,

『1
i1
i1
치
峀
置
妥
多
I
크
크

The variable may be created as a MATLAS timeseries, an array, or a MAT녀B structure,
MATLAP timeseries may b日usedf口rany data押口e. C口m미ma啣. or dimensi口n已 L口going a bus
引gn톄 口roduc日s a MATLAP 引ructure that matches the bus h泊rarchy. Each I日at 口t the
a甘ucture 冶 a 卜SIATLAS tim日5日tie$ 아）1ect
Use知ray幻rmat only幻rvector, do니bl日』n口ncompteo in口나Is. EachC口山mn미小earrayhasa
time 없amp In the 伽ntr口나 and a vector containing the corren口口ndlng da伯 S日m口冶 in 小5
subs日qu日nt rows
由rame伯rn
日Ic sam日：

母

Mytotila. mat
Vartab油name:
c。
s

車

Jt

Save torrnat

Array

:m

1

1

Decima如n:

1

m

녀

-

1
Sac）口泊 time (-I 幻rinherited)
t

9

OK

Cancel

]

Help

Apply

그림 15-18 To 日le 뷸록에 데이터 파일 이름 입력

0 설계 창의 [View卜[r如del Explorer]-[Model E叩lorer Ctrl+H] 메뉴를 클릭하고 To File 부분을 클
릭하면［그림 15-18］과 동일한 정보를 다시 보여준다．
器

Filter Contents

Conten忖 eli COO_Tv (only)

C이sen V七H

k岫sk Dots Typea 1

Nettle

Sho나Dc伯帖

Tot B的旭네타

eleokType O山oatolepeSto

Sink Block P. eaglet.r. '. To File

Y뇨

OotMit 005,4

心 Mod口1 너0巾1口aCe
qCoefigetenon lac卄
日

Cosin日 닙aYa

5m

00미n

3刻n

日

T口F比

To Ftc

The ocrleble ney be erected as a HATL.40 0mesehee, ee array, ore
MA11朋 absclsre
MATL.*8 tlm.senee may be used for coy data type, coepmeosty, or
비man引0n包 Logging abs$ 引en川 psodunes MAThAB 1打UC加to that
comCbo, era hoe hietayehy, Each loot of nrc nttus加r日 in o MAulAS
Unseen., ebleyt

Cod口 for COO加

@Melee for COO_Tn
0

Te File
tnot口cent川lii 叫rite dote in拍 a satiable in lb日 3口eC忖池d HAT寸lie

Inhent mnb口ill 니01st口mcii'

It

[I

Use Array I口snot only 化r YeC幻L 如먀ii,, n口n口Dm이en Input乞 Es口h
eo山nn of It. array has abe. s뇨mp in the heat roe end a vector
vnntemning fire eneenponding dote ccrtpie in the subsequent toes
Parse,日tern
FIle nelne
Mytottie,n. t
Variable eagle
ens_cot
Save I口eeoC 月ray
Desleagon
]

Conten捻

0

1

11

ScorE沌 tine （너 幻r in hen ted)

Revert

1 = Help

그림 15-19 생성된 모델의 세부 내용 살펴보기

0 ［卜4ode1 Explorer] 창에서 M에el \恥永space 부분을클릭하여 [Data source:]를MAT-File로 바꾸고，
EFile name:］어i는 저장되어 있는 'M批Dfile.mat'의 경로를 설정한다．
0 EReinitia血e 丘om Sot丁ce] 버튼을 클릭하고 열려 있는 EMo如1E사加rer] 창을 닫는다．

CHAPTER 15. 삼각함수

447

C口山inn Vie叫

미口口kO口to Types !

None

Model 놔미C op SC口

Filter Contents

Conton捻 of: COD_I口* (Only)
Sho낵 (eta怡

7 이 9ob冶Cl)的

미ookTypt OiitostsTypoStr

Y누

005Cr 00

麟 Model 나orks poe日＋
蟲configuration tAos
目

出口rkspooe dots
Data soorce:

IMATFi10

羅

iIT1Ifl

File nellie. .rsWcou쳐rDocunaflts臂HATl_ABWUytOtile.nrt
N미015.050 from Soulu口

ia닙. to 3그Un；亡

Code I아 coS-ro

回 Mv比. for COS_TO

Model arguments (Ins referencing thin model)

Sin

t고1Cosine 나aY口
｛크 0사e

Gain

0

Topile

To File

Inherit 1nh口rlt vie Intern니 n· []

[]

畔明彎弱r타ffr的oils

Contents

Revert

1

grip

1

Apply

]

그림 ]5- 20 생성된 데이터의 작업 경로 설정

0 시뮬레이션을 실행하기 전에 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 [Model
Configuration Parameter司 창을 열고 [Start time］과 毆op time］의 기본값0.0k 10.0을그대로유지한다．
0 ［그림 15-17］에서 완성된 모델의 시뮬레이션을 실행하면 자동으로 My的flle.mat가 생성된다．
四 入4ytoflle.mat를 명령 창에 불러올 때는 load 명령어를 사용한다.
q1To File 블록을 이용하여 생성한 데이터를 그림 창어］ 그리기 위해 다음과 긷미 명령 창어］ 명령어를 입력
한다．
1尸nn기弓rid 出indCU/
>' load 14yt0fi 1e
>> t = cos_oot (l, :);
>> cosine o cos_out (2. r) ;
'> plot (t,

cosine) ;

>> 뉘 的el ( t ) ;
>> 미 abel ( cosin已 ) ;
>' grid;

그림 15-21 시뮬레이션 결과를 그림 창에 그리는 명령에 입력

m 그림 창에서 시뮬레이션 결과를 확인할수 있다．

그림 15小22 그림 창 결과

448

PART 04. Sim메nk설계하기

정현파 응용 설계하기
서로 다른 정현파를 더하거나 빼는 연산울 하는 시뮬링크 모델을 설계하고, Demux 블록을 이용하여 정현파의 곱을 합으로 나
타내는 삼각함수 항등식의 설계를 알아보자．
Keyi사｛,rd

1 삼각함수 항등식 1

I 삼칵함수 항툼식
삼각함수 힝등식의 공식을 이용하면 삼각함수가 포함된 복잡한 식을 간편하게 정리할 수 있다. 이는 치환
적분에서 매우 유용하게 사용된다．

1 예工II 15- 5 I
다음과 같은 삼각 항등식이 성립하는 시뮬링크 모델을 설계하고 그 결과를 디스플러떼 창에 나타내라．이따1
日 = 30O, 功 = 60'이다．

sin蜘햐 如in(o如)+s血（0寸）]
푿이

O Sine Wave 블록 4개를 설계 창어｝ 생성하고（[Source司-[Sine Wave]) 블록의 이름을 각각 Sinel,
Cosine, Sine2, Sine3으로바꾼다．
0 블록Sine1을 더블클릭하여 [Frequency (rad/sec) :］에 0. [｝小ase:］에 0 = 30 "를나타내는pi石을 입력
한다．

CHAPTE日 ]5. 삼각함수

449

텨flu 나eve
Out口Ut a 引ne was日
0(t) = Amp.Sln(Freq=t.Phase) + Bias
텨nety口日 d日t日rmin日s the c口m口utah口nal t日chnique used. The
口arameters In 巾日 t니a types are rela也dthr口니gh
Samples 口er r）日dod = 2-pi / (Fr日qu日icy t Sample 卄me)
Numb日r of o加미 samples = Phas日 * Sam口1日sp日r 口cr1口d/ (2昨）I)
Us日 the sam이c-based 引nety口eifn니merical t玎obl日ms due t口
running 幻rlarge times (e.g. 口verflo나 in abs口山te time) occur.
Param日t마5
미fl日勻p甘 1기me based

!

Tim日 (t): Use 帥viulat幻的me

!

Mt베山de:
1
日las:
0
Fr日quency (rad/s日c):
0
Phase (rad)
pV6
Sam目帥me
0
望 Inter口ret vector 口arameters as 卜［)

心

OK

Cancel

H日巾

4쁘브＝

그림 ]5-23 Sine Wave 블록 Sinel의 각주파수. 위상 설정

0 블록 Cosine을 더블클릭하여 [Frequency (rad/sec) :］에 0. [Phase:］에 사인파와코사인파의 위상오프
셋文回증오m= 60'를더한값pi/2+pi/3을입력한다1
미ne 甘治cc
Ou巾Ut a 쉬n日 a日V甘
Ott) = 肉np*Sin(freqt.Phase) * Bias
Sine type determines the computational technique used. The
pararne也rs in the t叫Oty口日5 are related through:
Samples 口er 口en口ci = 2朴）i/ (Fr日quency 1 Sample time)
卜山mber of 口卄set samples = Phase t Samples 口er 口日rind / (2作바
Use the cern口lu-based 引ne ty口e 仟 numerical 口rob伯me due 幻
running for large times (e.g. overflow in absolute 甘me) occur.
Perameters
미Ice type: Time bae日d

r

Time (t): Use 引m내allan time

!

Mt미加dc:
1
미a客
0
Frequency (rad/sec)
0
Phas日 (r日ci):
pi/2.pi/3
Sample tie｝日：
0
匣｝ mnt日rt그ret Se아or 口日ram아ers as卜0

8

i

]

Canc日I

He巾

坦힌y

그림 15-24 Sine Wave 블록 Co封ne의 각주파수. 위상 설정

450

PART 04. Simulink 설계하7I

0 블록 Sine2를 더블클릭하여 [Frequency (rad/sec) :］에 0, [Phase:]에 日 + 功 = 30O + 60 "를 나타내는
pi/6+pi乃을 입력한다．
0 블록 Sine3올 더블클릭하여 [Frequency (rad/sec) :］에 0, [Phase:］에 日1 功 = 30 " 小 60 "를 나타내는
pi/6叫甘乃을 입력한다．
0 입력 2개를곱하여 출력 1개를생성하는Product 블록을 생성한다（
［卜'lath Operations卜[Prodi兀t]).
O 입력 2개를 더하여 출력 l개를 생성하는Add 블록을생성한다（小4ath O꺄rations卜[Add]).
O Gain 블록을생성하고（
［卜'lath Operations卜田如］) 더블클릭하여 [Gait피에 1/2를 입력한다．
0 삼칵항등식의 좌변과우변을묶는Mux 블록을생성한다（[Commonly Used Block司-[Mux]).
四 Mux 블록으로 묶인 입력 2개를 출력 2개로 분리하는 Demux 블록을 생성한다（[Commonly Used
B!어永司dD帥lii刈）. 출력 개수는 앞어써 연결된 Mux 블록의 입력 개수와 일치시킨다．
Demux
Split日C幻r 늬gna冶 into scalars 口r sm訓er sec幻rs. Check ‘日us
Select由n Mod日’ to a口lit bus 引gnals.
Param미마S
Nun出er of otib加：
2
0治play 마川on: bar

!

巴 日us selec卄口n mod日

뇨）

OK

Cancel 1

A口口m

그림 ]5- 25 Demux 블록의 출력 개수 설정

q1 시뮬쾨忖1- 크 후 입력값을 직접 보여주는 Display 블록을 생성하고（[Si砥司-[Display]) , 삼칵 항등식의
좌변 결과를나타내는L-Result, 우변 결과를 나타내는R-Result로 이름을 바꾼다．
0 블록을 더블클릭하여 소수점 아래 열다섯 자리 출력이 가능하도록 [Format:｝을long으로 바꾼다．
0冶play
Num日nc d冶play 口fin口ut va山55
Parame也rs
Format: long
Decim日ti口n
1
［크！初吼ng 네S히ay

a

（그K

Cancel

He巾

1

햐갸：咽1

그림 15-筍 D洽이ay 볼록의 출력 형식 설정

四 블록을 모두 연결한 후 [Simulation]-[Configuration Parameters] 메뉴를 클릭하여 [Configuration
Paran妃ters] 창을 열고 囹幻p ti毗］을0.0으로 바꾼다．

CHAPTER 15 삼각함수

451

C) 완성된 모델을 시뮬레이션하면 디스플레이 창을 통해 다음과 같은 결과를 확인할수 있다．
Ella

Ed忙

\h1ew

Oi5口lay

D以恥Fri

듸mulation

龍 好!

陣 中圄

Ar닉ry5匕

Co巾 b汁i

Help

" C字 心 @ 1> 型 匹！力 回 ! 幽 r

듸N꾀k4
!

也 亡剪SIN_BIk4

［그

心
i三

與
四
四

3쯔1

I

P1出d

H

口二；

믐

1rmm

-

4

四

=,

風
口

口 >
柚

ri _ I

쯔

a

'

冷
F1帥r

！苡戊

그림 15-27 완성된 시뮬링크 모델과 디스플레이 창 결과

452

PART 04. Sim베nk 설계하71

려庶거：唯油lettepo巧CT甘e)

CHAPTER

16
제어

CONTENTS
LESSON 01 닫힌 루프 시스템
LESS아1 02 전달함수
LESSON 03 상태방정식과 신호흐름산도
LESSON 04 다양한 제어기 설계 및 비교하71
LESSON 05 보드선도와 니콜스선도 설계하;71

LESSON

닫힌 루프 시스템1

01

단위 계단 함수와 램프 입력 함수를 입력 파형으로 이용하여 입력과 출력이 일치하는지 비교하고, 원하는 입력과 실젯값 사이
의 오차에 비례하는 신호를 다시 보내어 오차를 수정하는 귀환 경로가 있는 닫힌 루프 시스템의 시뮬링크 모델을 설계하는 방
법을 알아보자．
Keyword

I

I 단위 계단 함수 1 램프 함수 ! Step 블록 I Trans伯r Fcn 블록 I Ram口 블록 1

단위 계단 함수

단위 계단 함수를 입력 함수로 이용하면 일정한 제어 시스템에서 출력이 얼마나 목푯값과 일치하는지 알
수 있다．

I

괩프 합수

램프 함수（ramp function）를 입력 함수로 이용하면 시변 시스템에서 출력이 얼마나 입력에 상응하는지
알 수 있다．

I

Step 블록

Step 블록을 이용하면 지정된 시간에서 두 레벨 사이의 계단 입력을 나타낼 수 있다. 이때 시뮬레이션 시
간이 주어진 계단 시간보다 작으면 블록의 출력은 초깃값이 되지만, 시뮬레이션 시간이 계단 시간과 같거
나 계단 시간보다 크면 블록의 출력은 최종값히 된다．
또한 Step 블록에서 계단 시간은 계단 입력 신호의 시작을 의미한다. 예를 들어 단위 계단 함수 U小）의
계단 시간은0, u5(t- ti)의 계단 시간은 tl이 된다. 또한 단위 계단 함수의 계수는 최종값을 나타내는데，
예를들어 단위 계단 함수 2u (t)의 최종값은 계수인 2이다．

I

Transfer Fcn 블록

Transfer 民n 블록을 이용하면 라플라스 영역 변수 S를 사용하는 전달함수로 선형 시스템 모델을 설계할
수 있다. 전달함수는 전적으로 분수의 분모와 분자어］ 지정되는 매개변수어］ 의존한다. 단일 입력어］ 대한
단일 출력 시스템에서는 상수 시간 영역 신호 모델을 설계하고, 단일 입력어］ 대한 다중 출력 시스템에서
는 상수 입력어］대한 벡터 출력 모델을 설계한다．

454

PART 04. 針nulink설계하기

I

Ramp 블록

Ramp 블록을 이용하면 램프 함수를 입력 파형으로 하여 상태공간 함수와 연결되어 동작하는 시뮬링크
모델을 설계할수 있다. 일정한 제어 시스템에서 출력이 얼마나 목푯값과 일치하는지 알아보기 위해 꼐단
함수를 입력 함수로 사용하지만, 램프 함수를 입력 함수로 사용할 때는 시변 시스템에서 출력이 얼마나
입력에 상응하는지 알아볼 수 있다．

1 예저116-1 I

풀이

(s+

4

,
(s+

=

(0 드 r 드 15）을 사용하여 닫힌 루프 응답을 구현하는 시뮬링크 모델을 설계

s

하라· 이때전달함수.

(s)

단위 계단 입력 함수 u(t) =l

）이다·

3)(s+
2) 7

0 Step 블록을생성하고（[Source司d針ep]) 더블클릭하여 [Step tim因에 0을 입력한다．
0 Sum 블록을 생성하고（[Commonly 小ed Block引H田urn]) 더블클릭하여 [List of signs:］에 나H를
설정한다．
0 Gain 블록을 생성하고（[Commonly Used 미oc畑］-[Ga노］) 더블클릭하여 [Gait피에 4를 입력한다．
0 Transfer Fcn 블록을 생성하고（[Continuous] -[丁ran訂缸 Fcn]) 블록의 이름을 G(s）로 바꾼다．
0 전달함수 분자의 계수를 내림차순으로 지정하기 위해 [Numerator coeffic妃nts］에 [12］를 입력하고,
분모의 계수를 내림차순으로 지정하기 위해 [Denominator coefficients:］어[1 10 210］을 입력한다. 분
모의 샹수항이 없어도 0으로 표시해야만 분모의 전체 차수인 3차까지 나타낼 수 있다．
Tran出erFen

1

The nurnerat口rca日ific泊nt can be a sect口r or matrix espres引on.
The den口minat그r Co日fficient must b日 a vector. Th日 口U如uty. dth
日qua怡 It,日 number of r口＼as in the numeratc그r Co日佈ci日nt You
나tou너 5口日C啣 the coe佈ci日n始 in d日scending order of 口01人ersot
5.

4
]
?
!1
y
耳
旨

Parameters
Numerator coefifcients:

,n

(t2]
D日nomina幻rca日fficient可

3
J
극

(I 1。
21 。)

4

Absolute tolerance:

?

aulo
no也 N日m日 (e.g.. 'p0引出그n')

0

L OK

卄

1 Cancel j i H日1口 L A口口ly

그림 16너 블록 G(s）의 분자와 분모 계수 설정

0 계단 입력 함수와 닫힌 루프 웅답을 동시어］ 나타내기 위한 Mux 블록을 생성한다（[Commonly Used
미ocks卜[M好］).
O Scope 블록을생성하고（[Sink引냐Scope]) 블록을차례로 연결한다．

CHAPTE日 ]6 제어

455

Ed作

\flew

陣, 冒

,

File

［기splay

미agram

듸mUlatlon

Analy引5

Code

目꼼 " 呻 텍1 凹 吟 !

b帥5

H甘p

匹！汁 @ , 幽 ,

SYS I

e 團SYS1

!

1Hq)＋三：>

4

믐

9-

[,

爺

i;

-「
‘'U

Ga.,

.

J1
r

미5)

H

H1,

［그

m
曲
>>
ede45

l（麟

Rea旬

그림 16丑 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 EM어妃1 Con地uration Parameters] 창을 열
고［St町tt恤e］과歐叩time］에각각0, 15를입력한다．
0 시뮬레이션을 실행한 후 Scope 블록을 더블클릭한다. 마우스 오른쪽 버튼을 누르고 [configuration
properties...］를 클릭하여 창을 연 후 실행 결과를 최적화하기 위해 [Y小mits (Minimui미 :］에 -0.1,
EY小mits (M畔血mm) :］에 1.1을 입력하고 回K] 버튼을 클릭한다．
Ft挺

To여5

@,

兮 @ 1> 已 믐호 r 익 , ［끄 ,

View

듸m미ation

H甘p

U

+ 囹,
m
]

1.15괴叩

Pew打

그림 16-3 스코프 창 결과

계단 입력 함수어］대한 단위 귀환 시스템을 실행한 결과 정상상태 오차가0이다．

1 예제 16- 2 1
램프 입력 함수 /(t) =2r(t) (0 드 t 드 25）를 사용하여 닫힌 루프 응답을 구현하는 시뮬링크 모델을 설계
4(s + fl

가라． 0I때 전달함수G(s）乙
（小)(규7）이다·

456

PART 04. Sim매nk설계하71

ORamp블록을생성하고（[Sources] - [Ramp]）더블클릭古뼈［Slope:］에2 (2r(t)）를입력한다·
Ramp (mask) (link)
아1巾Ut a ram口 늬gn톄 start土ray at thee口日C出ed tme
Pan日m마日rS
S幻口e
2
소art tme;
0
in也al oil巾Ut
0
回 lrrte,pr甘 叩CI口r 口aramoterS as卜D

OK

N日巾

Canc미

그림 ]6닉 Ram口 블륙의 기울기 설정

0 ［예제 16크］의 0- 0을 반복하고 블록을 차례로 연결한다．
F七

Ed忙

\/ien,

C거＄play

0的ram

듸mulatlon

Ar日ly되5

Coda

初이5

140巾

'呻 45也7 印 , 因 " ' 臼 ' 幽 '
"旨旨
固 ' 呵＼, 口1
0V02 1

:

回SYS2

!

奴
트．
i
4

/

回

8

,4,

品

4上

匹
［그
吐
由
力

4
[i크꾜

系j

![1

口

凡H吻

/00%

1

0d040

그림 16巧 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를클릭하여 ［卜如del Cont如ration Paran妃ters] 창을 열
고田恤tt油e］과［S的p血ne]에각칵0, 25를입력한후시뮬레이션을실행한다．
0 시뮬러和］션을 실행한 후 Scope 블록을 더블클릭한다. 마우스 오른쪽 버튼을 누르고 [Confi엣ration
properties...］를 클릭하여 창을 연 후 실행 결과를 최적화하기 위해 [Y-li毗s (Minimum) :］에 Or ['i
limits 小laximum):]에 50을 입력하고 回珣 버튼을 클릭한다．
r；而瓦0/s V沌1Y 돠mulation H여口
$ , 啞 (9 耶＞ 簪 咨 , ei . ［二 , f 回 ,

그림 16七 스코프 창 결과

램프 입력 함수어］대한 단위 귀환 시스템을 실행한 결과 정상상태 오차가싱나＝이다．

CHAPTE日 ]6. 제어

457

LESSON

02

전달함수

전달함수는 시간 영역의 임펄스 응답에 대한 라플라스 변환이다. 전달함수의 직렬 연결 및 병렬 연결에 대한 계단 응답을 구현
해보자．
1 라퓰라스 변환 1

Keyword

!

라플라스 변환

변수 t를 사용하는 시간 영역의 미분방정식을 변수 S를 사용하는 라플라스 영역으로 변환하는 것을 라플
라스 변환이라고 한다. 라플라스 변환을 이용하면 미분이나 적분처림 복잡한 함수를 수학적으로 곱셈 또
는 나눗셈과 같이 훨씬 간단한 대수함수의 모양으로 변환할수 있다．

1 예저116-3 I
1.1: 1:1- 11 m-. I

시간 0 드 t 드 8일 [[Ft 전달함수 G如）, G2G兀卄 대한 계단 응답을 구현하는 시뮬링크 모델을 설계하고 그
결과를 스코프 창에 나타내라．

l

s+ 1

G如）＝詳万· 이s)亡卄
풀이

0 Step 블록을 생성하고（[Sour此司4飢ep]) 블록의 이름을）小）로 바꾼다. 블록 X (s）를 더블클릭하여
[Step time:］에 0을 입력한다．
0 Transfer Fcn 블록 2개를 생성하고（[Cont血uous] - [Transfer Fcn]) 블록의 이름을 각각 Gi (s),
G2 (s）로 바꾼다．
0 블록 Gi (s）를 더블클릭하여 [Nu毗rator coeffic油吐S.］에 [1], [Den애lina的r coeffic妃nts:］에
[1,2］를 입력하고, 블록 G2 (的를 더블클릭하여 困U毗ra的r coefficients:］어］ [1,1], [Denominator
coeffici이its:］에 [1,좌을 입력한다．
0 Scope 블록을 생성하고（[Sii出司｛駝ope]) 블록의 이름을 Y (s）로 바꾼다. 블록Y (s）를 더블클릭하고
[Configuration Properties...］아이콘을클릭하여 困m小er of蜘ut ports:］어口를입력한후［Layout]
버튼을클릭하여 아래위 창을 설정한다. 이때 小加mber of in까ti均rts:］는［卜4ai미에서 수정할수 있다．

458

PART 04. Sim메nk설계하71

Main
因 0口日n at 引m너aft口n 尉art
回 0冶play 小a full 口aft,
卜仙mb日rot in口Ut ports: 2

Layout

]

Samp泊 蜘11日：

日ements ax chann日冶 佃日mF加 based) r

Maximiz日 ax日S

off

無日s scaling:

Manual

I

In口Ut proces引ng:

U

OK

Cancel

C口nfi口니re

..

A口口如

그림 ]6寸 Scope 블록에 입력 단자 2개 설정

0 생성된 블록을 차례로 연결한다．
Rie

帥C

\／化나

Dis머ay

囹 , 『i

t거agrarn

닯mulatt｛曳｝

Analysis

" 鸚 " 呻 텍5 \9 昑 ,

COi브

Tcx出5

H뱌1

E小，
, 回 , 筐恥

Tff F] 1

e 回TRF1
억
口
4

1i

咽
回
［그

!

"'f

口

1+1

80%

Rea旬

ode45

그림 16田 완성된 시뮬룅크 모델

0 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 ［卜4od이 Cot小guration Parameter司 창을 열
고［S切rtt恤e］과［Stc巾time］에각각0. 8을입력한후시뮬리徊］션을실행한다．
0 시뮬레이션을 실행한 후 Scope 블록을 더블클릭한다. 위 창어囚 마우스 오른쪽 버튼을 누르
고 [Configuration properties...］를 클릭하여 창을 연 후 [Y-lirnits （入4inimum) :］어］ 0, [Y-l的ts
小4aximum) :］에 0.8을 입력하고 回K] 버튼을 클릭한다. 마찬가지로 아래 창의 [IT-limits 伍伽鈿urn乂］
에 0.2. [Y小mits (Maximum) :］어｝ l을 입력하고 回K] 버튼을 클릭한다．
f카x lix朽 V他w
0 , 寸 (8 吟 S

듸mufatt아t

ia甘p

各 니 咬 , ［꾜 f

긔

區,

그림 16田 스코프 창 결과

그래프의 위쪽에는 G1(s)의 계단웅답 결과가, 아래쪽에는 G如）의 계단응답 결과가 나타난다．

CHAPTE日 ]6' 제어

459

I

전닫합수 직렬 연겸

전달함수의 직렬 연결은 입력 X(s）와출력 Y(s) 사이에 2개 이상의 전달함수가 있음을 의미한다．

1 예제 16- 4 I
시간 0 드 t 드 8일 때 전달함수 G如). G2(s)의 직렬 연결에 대한 계단 응답을 구현하는 시뮬링크 모델을
설계하고 그 결과를 스코프 창에 나타내라．
n_I. 1
1
G如）= S寸三， G2佃갸卄

覇i

0 ［예제16-3］의o, o을반복한다·
0 Scope 블록을 생성하고（[Six出司-[Scope]) 블록의 이름을Y (s）로 바꾼다．
0 생성된 블록을 연결한다．
Ed祛

\lie빛

Dis히ay

Dia了am

Sin｝네atk川

Analy늬＄

C어加

Tm必

" 琵 " 드a和 q3 \9 11> , E斗，》

回! 亡

(3

Ale

F＋미p
!

蟲

!

TAF2 1

으

!

團T#F2

;

川파

［二

:::,

1.

茗 그

GIIH

02（引

Y{5)

100%

Rea旬

0de45

그립 ]6-10 완성된 시뮬링크모델

0 설계 창의 메뉴 표시刮P寸 [Simulation] 메뉴를 클릭하여 [Model Configuration Parameter司 창을 열
고［S切it time］과［St叩time］에각각0, 8을입력한후시뮬레이션을실행한다．
File

To이s

VIe叫

듸mulation

Help

Y

@ , 的 G) 1口 藝 弓로 , d1 , ［二 , f

0.

l5

小叫卄

,

기

.

r]

\,.,,,1

/r

2

"'

尸

0.

K순 ,

I
-

Os

:

LH 1

二

r

口

干＝8스D0

그림 ]6-11 스코프 창 결과

전달함수의 직렬 연결은 다음과 같이 전달함수 2개를 곱한 형태로 나타낸다．

460

PA日T 04. Simulink설계하기

Y(s) = G小)G2(s)X(s)
그러므로 매초 단위에 상응하는［그림 16寸이의 전달함수 G如）와 G2(s）의 진폭을 곱하면［그림 16寸
11］과같다．

I

전달함수 병렬 연결

전달함수의 병렬 연결은 실행 전에 결함을 예측하고 실행하는 귀환 과정을 제어하는 기능이 있어 피드포
워드（fee小아ward）라고도 한다．

1 예저116-5 I
시간 0 드 / 드 8일 때 전달함수 Gj(s), G2(s)의 병렬 연결에 대한 계단 응답을 구현하는 시뮬링크 모델을
설계하고 그 결과를 스코프 창에 나타내라．
／기 / \
1
』거 / \
S+1
(-I八S) =;4万· (-7八키＝ 5-1-중

0 ［예제16-4］의0Ne를반복한다·
0 Sum 블록을 생성하고 생성된 블록을 연결한다．
［而e Edi' 니ew 머뺀斗啣'In Sim出施on 蜘恥뇹『岫 自어5 벼
「
1
느｛d " ' 回 ' 幽 ' ]
鵠字 ' " 呻 왜唯 昑
回 ' r

1 THF3 1
回TRF3

1
쁘日

11

i

!:!

1二

j

1 二고
=E

1二
Li>>

5+2

그

Gil引

!+1

IL

系1

5+3

G2( )

1Ready

11
[

4)
1

100%

1

,1

;
i
i

『r

0d045

1

그림 16니2 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄어써 囹油띠的on] 메뉴를 클릭하여 小如del Configi玎ation Paran妃ter可 창을 열
고［S切rt time］과囹的pt油e］에각각0. 8을입력한후시뮬레이션을실행한다．

CHAPTER 16. 제어

461

H知

T0O$

\／七나

돠mula抑Jn

0.

心미也@ 哈 8

He巾

긔

率 r 風 , ［끄 r f 區 '

95

。88
小

\,,:．

。8

I

S

朗mdy

1-80凹

그림 16-13 스코프 창 결과

전달함수의 병렬 연결은 다음과 긷H기 전달함수 2개를 더한 형태로 나타낸다．
Y(s) =[Gi(s)+ G (s)]X(s)
그러므로 매초 단위에 상응하는［그림 16-이의 전달함수 G小）와 G2(s）의 진폭을 더하면 ［그림 16小
13］과같다．

462

PART 04. Simulink설계하71

LESSON

03

상태방정식과 신호흐름선도

시뮬링크를 이용하여 상태방정식에 대한 싱퇘공간 모델을 설계하고 상태방정식을 전달함수로 변환하는 방법을 알아보자. 블
록선도는 제어 시스템0似寸 각 요소 사이의 신호가 전달되는 모양을 나타내는 방법이다. 시뮬링크를 이용하여 시호흐름선도와
동등한 모델을 설계해보자．
Key니／ord

I

I Sta也-Space블록 1 신호흐름선도 1

State-Space 블콕

State -Space 블록을 이용하면 선형 상태공간 시스템을 구현할 수 있다. 이때 필요한 상태방정식과 출력
방정식은 다음과 같다．
交 = Ax + Bu

=

工.

=

to

뇌t

y =Cx+ Du

여기서 x는상태 벡터, U는 입력 벡터, y는출력 벡터, 知은상태 벡터의 초깃값이다. 또한 꼐수행렬 A는
n)＜刃伽은상태의 개수）, B는n)伽伽i은입력의 개수）'C는rxn(r은출력의 개수）, D는r>＜刃I형태이다．

I

신量晝묩선도

신호흐름선도는 선형대수방정식의 변수 간 입출력 관꼐를 도식적으로 나타내는 방법으로 블록선도보다
수식적 표현이 간편하다. 상태방정식을 적분하여 상태변수를 구하는 성질과 미분방정식을 이용하여 시뮬
레이션에 사용하는 블록선도 모델을 구성할 수 있는데, 블록선도에서는 적분기 블록을 기본으로 사용한
다. 신호흐름선도에서 변수는 마디 (node) , 신호의 흐름은 화살표, 이득은 마디와 마디 사이를 나타내는
가지 (branch）로 표시한다．

1 예제 16小 1
0 드 t 드 3 범위의 다음과 같은 방정식을 푸는 시뮬링크 모델을 생성하고 그 결과를 스코프 창에 나타내라．
万（t) = 3u5(t), 玉(t) = -3us(t- 1)이고 초기 조건은 工，(t) =0.2, 汕(t) =o이다．
i1= -6兀 + 4工2 +/;( D
x2 = 5工1- 7工2+f2(t)

CHAPTER 16. 제어

463

==
口na
지식

Sta把-Space 블록을사용하기 위해 주어진 방정식을상태방정식과출력방정식 형태로 다시 쓴다．

，H＝求，나 :］目
상태방정식上’
。 1 x2

。。

f2

Y2

f

[:

출력방정식： ', = 1 0 x1 + 0 01

[-6 41
[1 01
[1 01
[0 01
시스템행렬A= [ 5 寸7]，입력행렬B= [0 ii，출력행렬c= [o ii，전송행렬D= I[。 。］으로표시
된다．

풀이

0 Step 블록2개를설계 창에 생성하고（[Son丁ce司4宬ep]) 블록의 이름을 각각Step!, Step2로바꾼다．
0 블록 Step1을 더블클릭하여 [Source Blo味 Paran妃ters] 창을 열고 [Step tin妃：
］에 0, [Initial value:]
에 0. [Final value:］에 3을 입력한후（3珤(t)) [OK] 버튼을 클릭한다．
Ste口
Out口Ut C Ste口
Param日也rs
Step tIme:
0
mE톄 valu日：
U
Anal V궤U日：
3
Sam히日 dme:
U
團 In甘口ret 晦C幻r 口aramet日re as ] 七
回 Enable zero-cros引ny detecti口n

[

0

OK

)

Cancel

Help

J[

Apply

그림 16-14 뷸록 Stepi에 새로운 변숫값 설정

0 블록Step2를더블클릭하여 [Sou丁ce Block Paran妃ter可 창을 열고 [Step time:］에 1, [Initial value:］에
0. [Final value:］에 -3을 입력한후(-3u小- 1)) 回지 버튼을클릭한다．
Ste口
Out口Ut C 澍日p
Parameter드
S自日口 dma;
1
Itt ti톄 Va山e.
U

-3

日n비 Va山a

Sample time
U
回 In伯r口ret ＼尼clor 口arameters as ] [)
國 Enable zero-cros引ny da也cli口n

0

[

m

1 Canc日｛

그림 16-15 블록 S螂尸에 새로운 변숫값 설정

464

PART 04. Sim메nk설계하'I

H日巾

Ap미y

0 入4ux 블록을설계 창에 생성한다（[Commonly Used Block日-[Mu幻）.
0 생성된 Mux 블록을 더블클릭하여 [Fm毗ion 미ock Parameters] 창을 열고 [Nun北er of inputs:] 에 2
를 입력한후 回K] 버튼을 클릭한다．
OSta把-Space 블록을 설계 창에 생성한다（[Contii叱이瑚m囹愧te-Space]).
O 생성된 Sta把-Space 블록을 더블클릭하여 [｝恤兀tion Block Parameters] 창을 열고 상태방정식과출력
방정식의 행렬 A, B, C, D와초기 조건 [0.2:0］을 입력한후 回K] 버튼을클릭한다.
St日lB S口ac日
State-s口ace mod日n
do/at = An * Bu
y = Co + Du
Parameter드
A:
卜6.1;5-刀
B:
Fi.eot1
C:

(t. oail
口
10.口0,0]
In出ci condill口Os:
(0201
柚S미utet미erance:
auto
Stat日 Nam日：伯．g., po帥如n,)

O

i

OK

Canc희

MJ如虹量羅舜 滋出却地니

그림 ]6-16 Stat今Space 블록에 행렬 입력

0 Scope 블록을 설계 창에 생성한다（[Sii血可H田cope]).
O 생성된 블록을 연결한다．
F作n

Ed吐

V超w

耳！圄

ont初y

D域恥m

돠m出求批계

鸚

Anal好A

Cm押 b：
虹

" C뿌 心 七J q1)

14目p

므3r,, 녑7 ! 幽！

미mE
!

包SimE

e

蕪
n
4

回
回
［그

ii
I.

：헒
r，岩，

［그

"呼蜘

如m

心

朗
>>
Re畇

KKm

이노as L

그림 1今17 완성된 시뮬링크 모델1

四 설계 창 위에 있는 [Simulation]-［卜4ode1 Configuration Parameters] 메뉴를 클릭하여 [Configuration
Paran妃ter司 창을 열고 [Sta眈time］과 [Stop time］어］ 각각0.0. 3.0-을 입력한후 [OK] 버튼을클릭한다．
0 [S노iulation] - [Run] 메뉴를 클릭하여 시뮬레이션을 실행한다．
mScope 블록을 더블클릭하면 스코프 창어써 실행 결과를확인할수 있다．

CHAPTER 16. 제어

465

TOas

t. w

引m山必Dfl

1

出口

O 니 41 I> 1l 各 · 1 侄1 , ［꾜 ' I 囹 '

1.10烈Pa

그림 16-18 스코프 창 결과

1 여以1116-7 I
, =j , (n에 대한위상변수표준형의 신호흐름선도를보여
二음그림은 미분방정식 刃＋2刃＋3쁘＋4
l-1
1m '111 ' d , ' H dr, ' V 口r 1- 'P3/ = 3U '
준다. 시간 0 드 t 드 30에서 계단 응답을 구하기 위한 신호흐름선도와 같은 시뮬링크 모델을 설계하고 그 결
과를 스코프 창에 나타내박．

鈿 (t) o

1

s_I

s크

S니

' '"낮＝므
：1;

l

"

oy

그림 ]6中19 신호호룝선도

듈；
i

OSteP블록을생성하고（[Sources]-[Step]）블록의 ' 1름을”(t）로 " 超다·
0 블록u(t)를 더블클릭하여 [Final value:］에 5 (5u(t力를 입력한다．
S伯p
Output a 아a口
Parameters
Step time:
0
In柑ales山e:
D
日nal va山e:
S
Sam비e time
0
團 Inter口ret sect口r 口arameters 日S 卜［)
團 Enab泊 Z日r口-cr00引rig detection

OK

Cancel

그림 16-20 블록 u(t)에 최종값 입력

466

PART 04. Simulink 설계하71

Help

OSum 블록을 생성하고（[Commonly Used Block]-[Sum]) 더블클릭하여 [Icoi피을Rec切I唱ular로

바

꾸고 [L慨 of s蜘S.］에 ＋小mm를 설정한다．
0 Gain 블록3개를생성하고（[Commonly Used Bloc뇌m四帥끄） 블록의 이름을각각Gi, G2, G3으로
바꾼다．마우스오른쪽 버튼을누르고 [Rot毗e &Flip卜田lip 미ock｝을 선택하여 방향을 바꾼다．
0 블록Gl. G2. G3을더블클릭하여 [Gan피에 각각2, 3, 4를 입력한다．
0 Integrator 블록 3개를 생성하고（[Commonly 小ed 미oc녑[Integr毗아］) 블록의 이름올 각각 Tnt!,
Int2, In日으로바꾼다．
OSc叩e 블록을생성하고（[Sii水舒-[鈿叩司）블록의 이름을叭t)로 바꾼다．
0 생성된 블록을 차례로 연결한다．
也畔 V杉 斗世r斗咐恥鉀呼如if Aifalj固' C呼 1姚 H叫p
固 ' 目 ＜규 딕7 ' 볍昌 " 呻 也 @ 吟 m Ee3 " 回 ' 蟲 '
ST02

尸十

!

團STE2

8

烈
口
4

11

-

牛 븝U 日 ,}

臼
m
［그

셔

떠

日

므

,

1m

由
力
Ready

100%

0de45

그림 ]6-21 완성된 시뮬링크모델

0 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 ［卜'lode! Coi出guration Paran妃ters] 창을 열
고［St町t time］과囹的p time］에각칵0. 30을입력한후시뮬혜이션을실행한다．
F如

T出드

Wm

듸if蜘幻fl

H틔：

@ r ＜小 (9 目＞ m g주 , ＝也 , ;J , 李 囹 ,

그림 16-22 스코프 창 결과

CHAP正R 16. 제어

467

LESSON

다양한 제어기 설계 및 비교하기

04

시뮬링크를 이용하여 시스템의 성능을 향상하71 위한 디D 제어7떡 다잉촨 모델 설계를 알아보자. F：기［) Contr이甘 블록을 사
용하는 경우와 사용하지 않는 경우의 시뮬링크 모델을 설계하고 그 결과를 비교해보자．
Keys사ord

I

1 열린 루프 시스템 1 F기［:) 제어기 I PlDContr에er블록 1

열린 루프 시스템1

닫힌 루프 시스템과 달리 귀환 경로까 없어서 오차를 수정할 수 없는 제어 시스템을 열린 루프 시스템이라
고 한다．

I

PID 제어기

PID (Proportional小孔egral-D帥vative) 제어기의 전달함；
＞는 다음과 같이 라플라스 변환을 사용하

'

孕＋

凡＋

＝

(s)

C

여 나타낼수 있다. 여기서 凡는비례 이득, 凡는적분이득, 局는미분 이득沁］다．

尺』
：

P山 Contr에er 블록

PID Controller 블록출력은 입력 신호, 입력 신호 적분, 입력 신호 미분의 가중 합이다. 가중치는 비례，
적분 및 미분 이득 매개변수이다．

1 예저116-8 I
계단 입력 함수 u(t) =1 (0 드 t <4）을 사용하여 열린 루프 응답을 구현하는 시뮬링크 모델을 설계하고 그
결고릍스코프칭K게나타내라，이때전달함수G(5)
G(s) - ,s2+
:+81
8s+ 12이다．

풀이

0 Step 블록을 생성하고（[Source司-[Step]) 블록의 이름을u(t)로 바꾼다．
0 Transfer Fcn 블록을 생성하고（[Cont血uous］小［가ansI缸 Fcn]) 블록의 이름을G(s）로 바꾼다．
0 블록 G(s）를 더블클릭하여 小｛U毗ra的r coeffic妃nts:］에 [1]. [Denominator coefficients:］에 [1 8 12]
를 입력한다．

468

PART 04. Sim네nk설계하71

Transfer Fcn

-

Th日numer日t口rC口efficient can b日a nec幻ror matrix ax口ress油nO
The d日n口mbna的rc口efficient must b日 a Sec幻r. 재e ou切Ut 니Id小
equa冶 tfi日 numb日r of rows In the num日rator C口e佈dient You should
＄口日city the Co叫fidients in d日scending ord日r of powers of 5.

ii
d
1寸
n
:1

Parameters
Numerator coefficients:

g!

척

I

Den口mmn日for coefficien佃：

丑

(t8t2l
Abs口1ut日t이日ranc日；

a

I

aut。
State Nam日：伯．9., 'p口S蜘n,)

I

11

'

I-fe坦1 『 A口口如 기

Canc미

OK

8

그림 ]6- 23 불록 G(s）의 분자와 분모 계수 설정

0 Scope 블록을생성하고（[S血ks卜田cope]) 블록의 이름을C (s）로 바꾼다．
0 생성된 블록을 차례로 연결한다．
A他

Edit

View

0바加y ［기agraTTI

臣｝ , 目

Simu비掩n

Analy引5

" 旨昏＞呻 唯 的 且目 ,

Code

if刈S

He巾

E서 ,,, （汐 ! 筐自 ,

PID1
!

風
口
05

그

+

며'I

1
尸心＋'2
0｛이

느

r1

團叩1

e

C（돠

臼
i回
［그
E口
宙
力
S舶旬

100%

0de45

그림 16-24 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄어써 [S油ul餌on] 메뉴를클릭하여 ［卜如del Configuration Paran妃ter司 창을 열
고［Start time:］에0, 田的p time:］에4, ［卜4ax step si配：
］에0.01을입력한후시뮬레이션을실행한다．
Ale

0 ' 4 @ IS

SimulatIon

Help

各 ' 目, ［끄 ' 1 f i껌 ,

汨1似竹0汀吐伽
그림 16-25 스코프 창 결과

CHAPTER 16 제어

469

전달함수의 이득 0.08은 단위 계단 입력에 대한 최종 출력값이 된다 ．이는 정상상태 오차 0.92어i 해당
하므로 상당히 큰 오차이다. 게다가 상승 시간（小e time）은 약 2초이고 정정 시간（set如 time）은 약
2.5초이다. 그러므로 상승 시간과 정정 시간을줄이고 정상상태 오차를 제거하는 제어기를 설계한다．

(s)

드『드 4). 전달함수G

(5)

1

(0

=

계단입력 함수u

(t)

1 예斗16四 I
s2+ 8s+ 12일

=

, :+81

때 비례제어기를구현하는시뮬

링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이때1 비례 이득 瓦 = 10이다．

；涵
지식

푿이

"］려i제어기（皿.portional control!町）는기댓값과측정값의文H］어］ 비례8臣제어변수어｝보정이적용되는
선형 귀환제어기이다．
(a) PID Controller 블록을 사용하지 않는 경우
0 ［예제 16-幻의 (1Ne을 실행한다．
［卜4a血 O倂rations卜［Add]) 더블클릭하여 띠戚可signs:］에 +H를설정한다．
0 Add블록을생성하고（
0 Gain 블록을 생성하고（[Commonly Used Blocks卜四amn]) 블록의 이름을 Kp로 바꾼 후 더블클
릭하여 [Gain:］에 10를 입력한다．
二견

Gain

Main

fj4J

E油men卜내8日 gain (y = K. n) ormab似 95111 (y = 小U or y = U미0
텨90푀枷bu旽 'P斗imbr汕曲必8

G비n:
IC
Mn出plc日Con

C甘'C외

그림 16-茹 블록 Kp의 이득 설정

0 Scope 블록을생성하고（[Sin]心卜田cope]) 블록의 이름을C (s）로 바꾼다．
0 생성된블록을차례로연결한다．
F沁

帥t ＼月e늬

昆, 好

0il'加y ［加9m"

듸m出1t幻11

1005卜／oil

斗 喘 " 呻 떠 的 qP

Co巾 b아5

Ho作1

/ 낟j , 目 凹 , 芯自 ,

미D2
!

團叩2

8

念
1}
O*

甲 = ,,H8> ＋工，
늡

므

囹
心
口
m
由
力
RN旬

loon口

그팁 16-27 완성된 시뮬링크 모델

470

PART 04. Sim메nk설계하71

0d545

0 설계 창의 메뉴 표시줄에서 圄mulation] 메뉴를 클릭하여 [rb.如del Con地urat加n Parameters] 창
을 열고 [S切it time:］에 0. [S的p 血ne]에 4, 卜'tax step size:］에 0.01을 입력한 후 시뮬레이션을
실행한다．
F作e

祀아； V池뾔

Simula坎>n

出

Hdp

@ 기 心 @ 匹＞ 缸 믐r 曳 ' ［꾜 ' I

囹'

T=4'0此

그림 ]6-28 瓦＝ 10에 대한스코프 창 결과

전달함수의 이득 0.45는 단위 계단 입력어］대한 최종 출력값이 된다. 비교 제어기가 없는 경우와 비
교하면 정상상태 오차를줄이고 상승 시간 2초를 l초로, 정정 시간2.5초를 2초로 감소시킨다．
만일 O어써 비례 이득을 凡 = 100으로 바꾸고 시뮬레이션을 다시 실행하면 다음과 같은 결과가
나타난다．
F艇

T比虧

W咐

@ , 4 8 少 S 密 니 욕 , ［꾜

그림 個m四 瓦＝ 100에 대한스코프 창 결과

비례 이득을 증가시키면 상승 시간과 정상상태 오차가 더 줄어들고 정정 시간도 감소하지만 오버슈
트는증가한다．
(b) PID Controller 블록을 사용하는 경우
0

Gain 블록을 제거한 후 PID Controller 블록을 생성하고（[Continuous卜[PID Controller]) 블록
의 이름을P-con打oller로 바꾼다．

0 블록 P-con打oiler를 더블클릭하여 [Controller:]를 P로 설정하고 [Pr叩ortional (P) :］어］ 10을 입
력한다．

CHAPTER 16. 제어

471

Thsu뿌ck，i껍忍漕헒겪커，瑥“：깝器駐牲咎武쁨凞恕謂穽喘詰業擄恣謐'
'Tune,.. ' button (requires Simulink Control Design).

Conlr에er: P

!

m:＝出小立拉三a啣懈蜘懈滋mn蜘姓的解奴

F七rm: P미닙br

毋 Continu口us-time
可） D冶crc也새m日
卜hamn [ 디O Advanc日d 1 DataTypes I 앉ate Astribu由5
C口n如11cr poram미ers
imn

S口urce:

蚤

ternai

!

日 C（그m口日nsa幻r幻rmula

roportional (p): 10

P

Tune...

니

團 Ena너C zero-cros引ng d日teclion

1的

蜘i的的耐日柳1mm놔m小

,r口心m呼NmH口＝3 m,

OK

111

4

9

』

C帥回

「

小

H쉬p

Apply n.

그림 16-얹） 블록 円COfltr에아으J 비례 이득 설정

0 생성된 볼록을 차례로 연결한다．
同e

Edit

\／相w

Dlv｛乂ay

D啣眸n}

듸mulati（거v

at帥川S

Code

k）어S

I.化Ip

,, 琵 " L摯 好 也） 昑 , 巨3 !,. @ , 區打

舜, 目
미D3
的 亡封미03

風

므

m

!

I I

=
-*

-

-

Ma

나

日5}

n口11iDn日

1

느

!2+8i+12

G{5!

[1
C 注）

回
向

四

口
Em

出
>
ode45

奴戊

Ready

그림 16牛31 완성된 시뮬링크모델

0 설계 창의 메뉴 표시줄쇄서 [Simulation] 메뉴를 클릭하여 [Mod이 Configuration Parameters] 창
을열고［S切rt time］과囹的p time］에 각각0. 4를입력한후시뮬레이션을실행한다．
Ale

lo比

Vtew

@, 兮0 吟 S

SImulation

H甘p

率 , 익 , 띠기 + 囹'

T-4.000

그림 16-32 스코프 창 결과

472

PART 04. Sim매nk설계하기

전달함수G

, 나8s+

)=

(!

．

(0드t드4)

1

=

계단입력함수u

(t)

1 예제 16-10 I
니
12일때비려卜미분제어기를구현하는

시뮬링크모델을 설계하고 그 결과룔스코프 창에 나타내라. 이때1 비례 이득 尺P= 100, 미분 이득 凡 = 10이다．

배경
지식

비례1미분 제어기는 시스템 응답의 미래 오류 예측이 가능하기 때문에 제어 능력의 향상어］ 의해 시스템의
안정성을 증가시키는 데 사용할 수 있다. 갑작스럽게 변하는 오류 신호의 영향을 피하기 위해 미분은 오류
신호 대신 시스템 변수의 출력 응답에서 실행된다. 따라서 D 모드는 출력 변수의 변화에 비례하도록 설계되
어 있어 오류 신호의 갑작스러운 변화어｝ 의한 제어 출력의 급격한 변화를 방지한다. 또한 D는 공정 소음을
직접 科하기 때문에 D 전용 제어가사용되지 않는다．
Kds＋瓦
/ +(8 + 凡뇨 H口＋凡）
(a) PD Controller 블록을 사용하지 않는 경우
0 Step 블록을생성하고（[Sot丁ce可- [Step]) 블록의 이름을u(t)로 바꾼다．
0 Add블록2개를생성하고（
［卜lath Opera如ns] -[Add]) 블록의 이름을각칵Add1. Add2로 바꾼
다. 블록Addi을 더블클릭하여 [List of s培ns:］에 +h를 설정한다．
0 Gain 블록 3개를 생성하고（[Co帥lon1y Used 미ocks卜四ai미） 블록의 이름을 각각 Kp. Kd,
Fil奴小coef로 바꾼다. 블록Kp. Kd, Fi如卜印ef를 더블클릭하여 四帥비에 각칵 100. 10. 100
을 입력한다．
0 Sum 블록을 생성하고（[Commonly Used Blocks]-[Sum]) 더블클릭하여 [List of signs:］에
나 를설정한다．
0 Integrator블록을생성한다（[Commonly小ed Blo味司-[Integr毗0日）.
0 Transfer Fcn 블록을생성하고（[Continuous]-匡ransfer F鈿）블록의 이름을 G(s）로 바꾼 후 더블
클릭하여 [Nu毗rator coefficients:］어］ [1]. [Denominator coeffic慨心：
］에 [1 8 12］를 입력한다．
0 Scope 블록을 생성하고（[S雌司-[＆叩e]) 블록의 이름을C (s）로 바꾼다．
0 생성된블록을차례로연결한다．
F陀

Ed仕

\／呻w

O마,Iay

囹! 圄

미agrarn

듸malat匕r,

AIII如is

Coda

自여O

H帥｝

琵 心 ! 團 , 呻 텍 吃／ 印 袋 E즈 ,

斗 （汐 , d．
彗,

미D4 1
!

團叩4

e

蕪
目
4

毋1

!

,

回

1

0

뇨

폅：12

,므 「

咽
h.

;，南

r기

曲
出，

폴이

Ready

100%

od4卜

그림 ]6- 33 완성된 시뮬링크 모델

CHAPTER 16. 제어

473

0 설계 창의 메뉴 표시줄어써 [Simul毗ion] 메뉴를 클릭하여 [Model Configurat幻n Paran妃ter玎 창
을열고［S切rt山nd과［St叩time］에각각0, 4를입력한후시뮬러伯困을실행한다．
F卦口

To벼S

Vb州

tam出我卜며1 卜似p

0 , 也 (9I, .

이

粉 디 風 , i:i 니 f 國 .

m1녑F

!T.4啣

그림 16-34 스코프 창 결과

비례 제어기에서 비례 이득 凡 = 100을 사용한［그림 16-29］와 비교했을 때1, 미분 제어기를 함께
사용한 비례H미분 제어기는 오버슈트와 정정 시간을 줄이고 상승 시간콰 정상상태 오차에는 작은
영향을 미쳤음을 알수 있다．
(b) PID Controller 블록을 사용하는 경우
0 ［그림 16-33］에서 Gain 블록 3개, Sum 블록, Integrator 블록, Add2 블록을 제거한 후 PID
Controller 블록을 생성하고（[Cont加uo出]-[PID Controller]) 블록의 이름을 PD-con仕oiler로
바꾼다．
0 블록 P-contr아ler를 더블클릭하여 [Controlle川를 PD로 설정하고 [Pr아兀rtional (p) :］어］ 100.
[Derivative (D):］에 10을 입력한다．
F기D Coriltol冶r
Th冶 비ock 油비日ments contiri니0니a- arid 버scr日t日＝tim日 미0 con甘미 비gorittims and Inc山des advanc日d 伯atures

花紫喆羅벎濯甑器黑驃喆"녑"g. You"' " ""' "
C口ntr미岫r

PD

!

"" " " ' "' " "

Form: Parall톄

，소虹

孕 C口n甘nuous-tin,日
的 0油cr日t日-time
1Main ［至마函而而寸］ Da伯Ttp甘了I State Altribu伯a]

翌

1 C口n甘이1日r口aram日t日rs

:

1

1

I

S。
urc日：

1at日.0미

Pr口口ord口nal (P):

1 0口

Den始甘始 （D):

10

코

,

回 Comoens計or幻rio미a

1

P+D그

Filter coefficient

(N): l

Tune,

,.

"

"

三

1 In川눼conditions

針

1

So니rc，區雨
Filter:

,

0
『esec non毋

1E넋emn졔
！團Enable

i!

兀

i回Ign口r日r日set

ii1

a汁）err in日an기rig

I

ze
『小.rousing dete.的n

.1

4 [, m口n小

』m *比伊計：寸，.，小叫， , ,

H

小』
m口

多

質）
그림 16놔35 블록 PD-control呼으j 비례 이득. 미분 이득 설정

474

寸
I

I

如

PART04. 針nulink설계하기

;；그 卜

0K,

臼ncel

1

기 i 柶ci느l.1

0

생성된블록을차례로연결한다．
File 的1 哨的 야叫하 아呵；려o

回 ! 目 돠그 乙拉 l

Simulation

At니恥朽

Code

bios

H叫p

琵 今 , " 呻 心 ＼孕 昑 째 巨3 !,} (3 ! 蟲 ,

댁D5

: uJ- :
回叩5

!

口小

a

미11

1
H나
1랴m＋侄
뎌引

P6石i南

［그
C仁）

=i

mn

回
A

口
A
臼
F姓崎y

1伉夙

ode45

그림 16-36 완성된 시뮬링크모델1

0 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 ［卜4odel Configuration Parameters] 창
을열고［S切rt time］과田的아ime］에 각칵0. 4를 입력한후시뮬레이션을실행한다．

그림 ]6-37 스코프 창 결과

［그림 16-34］와 동일한 결과를 보여준다. ［그림 16-33］의 시뮬링크 모델은 다음과 같이 설계
할 수 있지만 이러한 설계는 측정 잡음을 증폭하기 때문어］ 순수 De加ative 블록（[Continuo出］e
[De加ative]）을 직접 이용하는 것은 바람직하지 않으며, ［그림 16-33］과 긷미 저역 통과 필터를 사
용하는 것이 좋다．
F晦

Edit

aew

［거5口lay ｛거agram

츠＞ , 딤

듸mulatlon

Anaiy引5

Code

1［刈s

He巾

鸚 好 , 團 , 丘學 站 @ 吼＞ 多 E쯔！

片 () , 幽 !

1 PIE히
!

回叩6

色1

1：크

.

\

=

＞二小
'夕

1
雋-I
-

回

.

-.

1
12＋由＋12

臼
1口
［그

HHF그
CAt

4
+

규쓰j

;

R.畇

100%

nde45

그림 16-38 Derivative 블록으로 대체한［그림 佑 33］의 시뮬링크 모델

CHAPTE日 ]6. 제어

475

LESSON

05

보드선묘II, 니콜스선도 설계하기

Bode F기아 블록을 이용하여 보드선도 모델의 설계를 알아보자. 또한 Nich이S 디아 블록을 이용하여 열린 주파수 전달함수가
주어졌을 때 닫힌 루프 주파수 전달함수의 이득과 위상각의 관계를 나타내는 니콜스선도 모델의 설계를 알아보자．
Keyword

I

1 보드선도 1 니콜스선도 1 Bode Plot 블록 ] Nich이SF기아블록 1

보드선도

보드선도는 가로축이 log口t 세로축이 뎨시벨 값인 크기 IG(i口J)1의 주파수 응답과 가로축이 log口) 서］
로축이 위상각乙 G(jw)인 주파수응답을그리는 선도를 말한다. 이때 이득은 데시벨（dB）로 나타낸다．

I

니콜스선도

니콜스선도는주파수응답어］바탕을둔 나이퀴스트선도와보드선도를응용한방법이다. 니콜스선도는 귀
환 시스템의 닫힌 루프 주파수 응답과 안정도를 결정하는 유용한 기술이다．

I Bode Plot！耳
助de Plot 블록을 이용하면 비선형 시뮬링크 모델에서 선형 시스템을 계산하고 보드선도어］이 선형 시스
템을 나타낼 수 있다. 시뮬레이션을 실행하는 중어］ 지정된 선형화 입력과 출력 사히의 모델 부분을 선형
화하고 선형 시스템의 크기와 위상을 동시어］나타낸다．

I

세ch이SI:기아 블록

Nichols Plot 블록을 이용하면 비선형 시뮬링크 모델에서 선형 시스템을 계산하고 니콜스선도어］이 선형
시스템을 나타낼 수 있다. 시뮬레이션을 실행하는 중어］ 지정된 선형화 입력과 출력 사이의 모델 부분을
선형화하고 선형 시스템의 열린 루프 이득과 위상을동시에 나타낸다．

476

PART 04. Sim베nk설계하기

1 예제 16-11 I
전달함수가 G(s)인 시스템에 대한 주파수 응답의 보드선도를 그리는 시뮬링크 모델을 설계하고 그 결과률

2)

(

_

(s)

5

1。
)

0 Cons帥t블록을생성하고（[Commonly Used Blocks]-[Constant]）블록의 '］름을Cons但 " 超후
더블클릭하여 [Constant value:］어］ 0을 입력한다．
Constant
Outpu내｝e constants口ecified by the 'C口nstant vs山日‘ parameter 作
'Constant value' Is a V日clor and m也r口r日tv日Ct口r 口arameters as卜0' 冶
on. treat the constant value as a t -D array. Otherwise. out口니t a may-in
叫th the same 네men引口ns 日s the c口nstant value.
M쉐o L＄吼카娥由U蜘］
Constant value:
0
回 In甘까et 妃마or parameters as卜D
Sam口Ic 甘me:
tnt

[

e

Cartc실；

OK

, Ha加

Ap口Ii) ]

그림 16-39 Const 블록의 상숫값 설정

OSum 블록을 생성하고（[Commonly Used Blocks] - [Sum]) 더블클릭하여 [List of sips:］어］ 나e를
설정한다．
0 Gain 블록을 생성하고（[Commonly Used Blocks卜［Ga刈） 더블클릭하여 [Gaii피에 30을 입력한다．
0 Transfer Fcn 블록을 생성하고（[Continuous］ 口ransfer Fc미）블록의 이름을 G(s）로 바꾼다．
0 블록 G (s）를 더블클릭하여 [Nu毗ra的r coefficients:］에 [1,5], [Denominator coefficients:］어］
[1,12,20］을 입력한다.
0 Scope 블록을생성하고（[Sink引-[Scope]) 블록의 이름을C (s）로 바꾼다．
0 생성된 블록을 차례로 연결한다．
月相 日虹

Vt呻

陣 中目

0硝啣

마呵帥

Sin艮然苡卜on

An帥戶t도

cc心

b鹹5

卜＋甘p

" 旨骨｝呻 叱 白 聆 「 돈5 , ，『（多 ! 區計

=5

I

!

=jH9 ,>
C口1t

'. 5

더口l

｝斗20
q5)

1

I

1

，뫼

令

夕＋

e

團BODE

RODE 1

E;

듈可

(

)

G

-

,

(s+

( 30

6

(5)

보드선도 창에 나타내라．

C｛되

回
且回
［그
E口
t크
力
Re帥1'

10畔

ode45

그림 16-40 연결된 시뮬링크 모델

CHAPTER 16 제어

477

0 마우스 커서를 G(s) 블록과 C(s) 블록 사이에 놓고 마우스 오른쪽 버튼으로 [Linear Analysis P毗蝴m
回utput Measuren妃蝴를선택하면 다음과긷이 출력점을나타내는화살표가설정된다．
F船

Ed作

\h1ew ［거splay

區｝ ! 圄

Diagram

듸mu欲山S

Analys巧

" 鸚 " 呻 ＜心 也7 昐

Code

i) ols

1＋텨p

k졉 ，》》 U ! 蟲 !

BODE 1
V

團日0DEI

@
色

d

갑匹>-+>-Co石t

=t

卞5

1

卜므1

月mm1

0i

（和）

cB)

［回

回
[：그
［出
I!蚤
力
b(C朕

Ready

岫45

그림 16-41 출력점이 표시된 시뮬링크 모델

0 마우스 커서를（允nst 블록과 Sum 블록 사이에 놓고 마우스 오른쪽 버튼으로 [Linear Analysis
Poii出］丑nput Per加rbat幻n］를선택하면 다음과긷미 입력점을 나타내는화살표가설정된다．
F艇

Ed忙

\／伯나

아splay

［거agram

듸mulation

Analy勺5

Code

b어：S

N帥）

" 鸚 " 됴爭 때 8 1P , E小》》回 , 蟲 ,

昆,呂
回BODE

BODEI
e

I

!

骨 =J녹）H＞나

:

COI.t

卞5
큐12드＋20

더m

더1)

므
C｛되

區
m
口
E口

出
方
Bee向

1伉戊

od日45

그림 16-42 입력점이 표시된 시묠링크 모델

G Bode Plot 블록을 생성하고（[Simulink Control I光計甲卜[Lii妃ar Analysis 餉倒 田ode Plot]) 더
블클릭하여 Show 히야 on block open에 체크한후 [Apply卜［OK] 버튼을클릭한다．

478

PART 04. Sim네nk설계하기

日ode Plot
Corn口U也 and d治play a lInear SI'밗日re on a Bed日 plot V口u can 톄So
specify be니nds 口n the lInear 日yst日rn and ass日rttt,atthe 1兀und日 are
sa甘引泊d.
Ur,earizations
Un日ariza甘口n Inputs/ca典）U佰：
B뇨ck : P口rt : Bus E泊m日nt

Configuration

日OD타／C口rcst : 1

In叩I Pertu巾at油n

BOD티／C（引 : ]

Ou巾UI h伯日sur日m日icc

Unearlze 0n:

!

啣嗽口n snapsh口t8

Snapsh口t卄m日日： (01
Trlgy日r ty口日：

F키引ng edg日

卜 씨gorhn) 야川口ns
卜 Labs冶

r百而；i百6n 團 Oh口나plot 口nb幻ck口pen

Res口口nag 야川rn注帥on..,

Canc叫

If)

Apply

그림 16- 43 日ode 디아 블록의 설정

Q ［그림 16-43］은 Bode P1아 블록의 설정 환졍을 보여준다．
臼 Bode 끼야 블록을 더블클릭하여 [Bode Plot] 창을 열고, 시뮬레이션을 실행하는 [Run] 버튼을 클릭
한다．
Ft地

Ed比

Votw

囹! 呂

O印啣

Diageam

듸mulaS｛가｝ 肉1帥y啞도

cc心

初이O

H叫P

" 旨旨呼
" 努 45 （孕 盼 芭 匹 !，》 已） ! 邕 !

芝

I

!

=：尸91＞나
Cent

S帥

1+5
12+1갑；面
더5)

，므

e

回BODE

BODE I

C{1)

1

=。

回
1口

0
E=
!i>
Ready

足三
1凹%

0de45

그림 16- 44 완성된 시뮬링크모델

CHAPTER 16. 제어

479

치口回

B岫DI呵-n

Q.

圓固庫留淨皿.

=

L肛站눈 bbCt

的

而므m호드＝ 旨＞

01
的

小g으富m工n

으0

101

Frequency (rad/s)
F印y

그림 16-45 Bode F거아 블록 창

四 Bode 끼ot의 크기를 알맞게 조정하면 다음과 같은 시뮬레이션 결과를볼 수 있다．
VI농

帥t

Tools

Sliw

Sini出心ni

I1却

圓 目 疊 (9 口 各 익 K건 玉 口

끼

듣크
山며i出e比以1

Ba巾 마叩ram

自 -10

亘，

晷

,

,

\\\,

듣 -30
m41J

孕
留

\\\\1

룬

.45

100

l01

化2

103

Fi띠J이
（y (reiVa)
nm升

了＝0啣1

그림 16-46 보드선도 창 결과

주파수 범위와 점의 수를 자동으로 선택한 시스템에 대한 주파수 응답의 보드선도이다. 위 창은 진폭
ma앉iitude로나타낸 위상응답을보여주고, 아래 창은각도phase로 나타낸 위상응답을보여준다．

480

PART 04. Simulink설계하기

l二, +3）의 니콜스선도룰그리는 시뮬링크

0 Cons切I丘 볼록을 생성하고（[Commonly Used Bloc畑卜[C毗tant]) 블록의 이름을 Const로 바꾼 후
더블클릭하여 [Constant value:］어］ 0을 입력한다．
OSum 블록을 생성하고（[Commonly Used Block司나Su蝴） 더블클릭하여 [L慨 of signs:］에 나1률
입력한다．
0 Transfer Fcn 블록을 생성하고（[Continuo出卜口ransfer Fcn]) 블록의 이름을 G(s）로 바꾼 후 더블클
릭하여 困umer毗or coeffic妃nts.］에 [6]. [Denominator coefficients:］에 [1,4.3,0］을 입력한다．
0 Scope 블록을 생성하고（[Si炚司-[Scope]) 블록의 이름을 C (s）로 바꾼 후 생성된 블록을 차례로 연결
한다．
0 마우스 커서를 G(s) 블록과C(s) 블록 사이에 놓고 마우스 오른쪽 버튼으로 띠near Ai好lysis Po岫］寸
[（九印ut 入4e羽uremet파를 선택하여 출력점을 설정한다. 또한 마우스 커서를 Const 블록과 Sum 블록
사이에 놓고 마우스 오른쪽 버튼으로 [Linear Analysis Points］丑nput Perturbation｝을 선택하여 입력
점을 설정한다．
F七

E出t ＼八eW

囹 1目

tX刑ay

［거agram

닯mulation

Anatys心

Co1目 iX比

He如

" 鸚 " C爭 愁 也） 聆 手 巨弘，
, 回 , 區打

00DE2

Q 團OODE2

風
토｝

二

따뇨9H
너t}

!

1
[
0仁）

LI
科七촤缸 1
0

풀이

=

(s+

(s)

단위 귀환제어 시스템에서 열린 루프 전달함수G

모델을 설계하고 그 결과를 니콜스선도 창에 나타내박．

s

1 예제 16-12 I

느口
亡ii)

團
［그
m

由
冷
_

100%

ode45

그림 16-47 입력점과 츌력점이 표시된 시뮬링크 모델

01小ch이S 끼야 블록을 생성하고（[Simulink Control Desi甲i]-[Linear Analysis P加t司-[I小c如ls
Plot]) 더블클릭하여 Show plot on block o꺄n어］체크한후 [Apply]-回K] 버튼을클릭한다．

CHAPTER 16. 제어

481

N七h口怡 P幻t
C口mpute and 비S비ay a linear system on a 세ch이S 미ot Ye니 can a怡口
S口日c加 L兀나nds 口0 小e in日ar system and assert that the bounds are
sa的fled.
Lineariza打口ns

코ounds 1 1刃88in8 1 栖Se加0

Unearization inputs/outputs:
H뇨ck : Port : Bus 티em日nfl

Confi만iratlon

日ODE2/u(t) : 1

In미it Perturbal汨0

玉

日0DE?.'이旬 1

0叭putM日aSur日ment

!

[1
[：二그

［二그

[1

Unearize 口n

帥rot相如0 en羽shots

Sna口澍l口t卄me5: [01
Trigg日r ty口甘

Ri引no ecig日

二7

卜 Algorithm 야거幻05
卜 Labs冶
Shi｝나F가OF 團 She나1引口ton block o口日n
OK

9

J

A日sponse Opit耐za如n...

Canc비

A口p汐

II이p

그림 16-48 Nk巾이SF거아 블록의 설정

0 완성된 시뮬링크 모델은 다음과 같다．
F加

Edit

V沁벼

0往play

國' 圄

더叩ram

듸m네哉ion

Anity斗5

Code

p：刃is

" 娼 " 呻 心七） 昨 1 E目 "

比巾

凹 ' 幽'

I 000E2]

으1團BODE?
1

骨 =J니9

53＋七2中3$

Cd出

，디

:

니
6

G{5 )

1

1
1

1

1

圈

1

！因

口

!i

(1

1

‘

">,

耐

心

1Ready

1凹%

0de45

그림 16- 49 완성된 人區룅크 모델1

o l小chols Plot 블록을 더블클릭하여 [Nichols I기ot] 창을 열고, 시剖1이션을 실행하는 曲m] 버튼을 클
릭한다．

482

P.ART04. 텨m메nk설계하기

F艇

Ed比

!ools

Vie텍

듸mulat卜야i

H叫p

目 툐l 甘 拿缸 各 텍 땍 承 心 雹
札

曲

U口idte I,匕C'

N比h이a Chart

凹

008
05 0B

加

小m므드mOn8닛b스O

025dB
lOB

1 08

化
0
和

-20
0

100

50

15$
200
250
ape小m卯 Phase世多吐

3刃

350

그림 16-50 Nich이S 디아 블록 창

0 시뮬레이션 결과는 다음과 같다．
F沁

Ed作

IC刈5

圓 目1目I1.

너ew

듸mulati아｝ He巾

爭 1 텍 畔 玉 1：그 國
H1寸ID뇨 Chart

兀
如
加
的
m

八띰나＝ 而O스8무CmnO

0
-180
느얹｝
0
op帥叱的p Phase (d四）

180

呻r
그림 16-51 니큘스선도창결과

四 니콜스선도의 x축, Y축 범위를 바꾸려면 마우스 오른쪽 버튼을 누르고 [Pr아妃rties...］를 클릭하여
[Pr아犯向 Edito日 창을 연 후 [Liii血S] 버튼을 클릭하고 以寸Limi同와 [Y-L帥倒를 설정한다．

m；司 · 口i;T; 1 0m由noJ
戶d三小Scd且 口

Un寸n -270 小iii드＋ j
5-LinEo
AC0C-Sc,Ie ［그
LEn孔S口-30

10140

a蜘

1仰

그림 16- 52 시ch이SF거아 창의 범위 설정

CHAP在R 16. 제어

483

帥8

F枷臣

Too뇹

니eW

듸m미atior,

'

He巾

1

目 目 甘 j8 m :;9 奴 냐 k 因 國
Uodte be

二0dB

Chan
Nich。
N七hd1
ls Chart

30

曾 20
훔 10

1dB

-1dB

1，

0

ID

-20

-Jo
니270

-225

-90
-180
-135
印en七刃p Phase (d的）

P미1小r

그림 16-53 새로운 범위의 니콜스선도 창 결과

484

1

「／
,,:,，三二

阜
용-

025dB
。5dB

PART04. 텨m메nk설계하71

-45

0

T＝也啣

1

下니
CHAPTER

17

나

신호 및 시스템
小

1

1

4

누 느 卜

규

+;]J

L

나H

F

CONTENTS
LESSON 01 다양한 함수의 신호 나타내기
LESSON 02 신호를 전달하는 모델 설계하기
LESS아'1 03 필터 설계하기

LESSON

01

다양한 함수의 신호 나타내기

연속 비주71 신호의 대표적 함수인 싱크 함수와 이산 신호를 스코프 창과 그림 창에 나타내는 방법을 알아보자 ．또한 연속 신
호에 대한 임펼스 응답 신호를 컨벌루션하는 모델을 알아보자．
Keyword

단위 계단 함수

(t,

):

Ii

(t

[。

=

(t)

u

.(/

연속 신호의 단위 계단 함수는 다음과 같이 정의된다．

=

<。)
0)

I

I 단위 계단 함수 1 임펄스 함수 1

I 임펄스 함수
연속 신호의 임펄스 함수（또는 델타 함；=）는 다음과 긷미 단위 계단함수를 미분한 형태로 나타낼 수 있다．

니 무정의
I

1 0

(t< 0)
.

0)

1 0

(t=

UI

t)

-

(,

(r)

a(t)

du

. .

-

(t> 0)

1 예저117-1 I
굻0씩 증7陌는 二음과 같은싱크 함수의 시뮬링크모델을 설겨1하고그 결고릍스코프 칭뻐1 나타내라. 이때
시뮬레이션의 실행은 시간축 幻r 드 t 드 4兀에서 진행한다．
x(t) = sin2rt

系；

0 Sine也ave블록올생성하고（[Sourcesl-[Sine W如e]）블록의 "］름을！(t）로日區다·
0 블록x (t)를 더블클릭하여 [Amp!恤de:］에 1, [Frequency (rad/sec川에 pi를 입력한다．

486

PA只T 04. 텨m메nk 설계하'I

돼ne H畑ye
Output a sine wave:
O(t) = MiptSin(Fr日q.t=Phase) * Bias
돼ne typ日 d日t日rmin日sit,日 口口m口Uta甘口n눼 t日口hniqu日 used. The
paramet마a In th日 t叩口 ty口es are r비ated thro니gh
Sam비es per 口日nod = 2朴ii / (Fr日quency 1 Sam비e 打m日）
袖imber 口f 口If s日tsampt日5 = Phase t Sam비日S 口er 口en口d/ (2싸기）
Use the sample中b日S日d 引fly ty口e If numeric톄 口roblems d니et（그
running 佃r lang日 卄n）日5 （日g 口vertow in absol出e 甘me) 口ccur.
Param甘ens
Sine type: 1 Time based
lbn犯 (t): Us日 늬mulati口ntis）日

!

knplf山de:
1
Bias:
0
다equency Crad/e日C):
p1
Phase (rad):
0
Sam口Ic 甘m日：
0
國 In泊rpret 恒ctor 口日rams伯rs as卜D

Cancsl

그림 17너 Sine 블록의 진폭, 각주파수 설정

0 사인 함수의 인수를 나타내는 Constant 블록을 생성하고（[Commonly Used Block釘나Consta씨）
블록의 이름을Argument로 바꾼다．
0 블록Argument를 더블클릭하여 [Cons恤it value:］에 pi를 입력한다．
Constant
Output the constant specified by the 'Constant value ' parameter. ft
'C口nstant V日lu日’ 冶 av日ctor and 'In伯rpret Ye아마 口arametens as卜 ［) 冷
口n, treat the c口nstant valu日 as a卜 ［) array. Otherwise, 口u巾Ut 5 matnle
내附i the same 비m日n引口ns as the constant va山e
Main

奴0乳脚bit峻昇

Constant value:
1기
團 Inter口ret 蛇CtOr 口arameters as 卜［)
Sam이e 11me:
jot

9

OK

Canc비 比 H日1p

A口비y

그림 ]7丑 （丸nstant 블록의 진폭, 각주파수 설정

0 각각 시뮬레이션 단계에서 현재 시뮬레이션 시간을 출력으로 나타내는 이ock 블록을 생성하고
([Sos丁ces]-[Clock]) 블록의 이름을 t로 바꾼다．
0 블록 t를 더블클릭하여 신호의 샘플링 비율을 줄이는 과정을 의미하는 [Dec油ation:]i 1을 입력한다
（기본값은 10).

CHAPTER 17 신호 및 시스템

487

Clock
Ou巾utth日 current 前mutation time.
Paramet아S
［二］ 0冶1기日ytime
0日cima的n:

1

}

OK

1

H아口

그림 17-3 Clock 뷸록의 Decim帥on 설정

OD如ide 블록을 생성한（[Ma小 OPera如ns］丑万vide]) 후 더블클릭하여 [Number of i叩uts:］에 串／ 를
입력하고［Sa卿le time:］을0으로설정한다. 마우스오른쪽버튼을눌러블록의 크기를확대한다．
Pr口duct

=

Mu出ply or 비너de iii口니ts. Choose 톄ement小너S日 or mal拙 F玎oduct and
S口en加 on日 otth이애0내n9:
a) t or / 幻reach in口ut port For 日eamt丑e, 11/* pertorrns 甘l日 0口日rati（그n
'ut .u2/u3'u4'.
b) scaler specifies the number of input ports to be multiplied.
ti there 沽 only 口ne 汭口of pot相nd the h仙뺘네ca的n parameter 沽 set to
티em日nt- wlse(.*), a 틔ii미e * or /c에a口ses the in口Ut 引gnat 니引ng the
specified 0口erat向n. H口＼V日ver, 什the Mu뺘네ca如n parameter 冶 S日tt口
Mattie(日，a 引ng伯 1 caus日sthe 비ockto Out口utthe matrix 니nchang日d,
帥da 비n미日 / caus日sth日 비ock to output th日 matrix inner＄日．
卜lain

미日flat Altribi的日S

-'I

Numb日r 口tin口uts

卜lu忖口ticat幻n

타미nent-내S日（．놔

0

Canc日1

H日巾

그림 17-4 마너de 블록의 Decimation 설정

0 Scope 블록을 생성하고（[Six出司-[Scope]) 블록의 이름을 鈿c (t）로 바꾼 후 생성된 블록을 연결하여
모델을완성한다．
F晦

Ed在

View

0却Lay

曷, 딤

Oiagraxn

Slew出曲on

Ax畇gin

1唱訃 呻 聳 回 1> ,

Cot늦

tmb

F岫p

全 ，片 9 ! 筐自 ,

S떠1
!

團師1

好

風
口
4

叩

:

口

回
i回
口
Em

曲
力
Reacbg

100%

ode45

그림 17-5 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄어써 田imul餌on] 메뉴를 클릭하여 [Model Configuration Paran犯ters] 창을 열
고 [S切rt 血ne:］에 -4水pi, [Stc巾 血ne:］에 恥pi, Max step 前四셔1pi/360을 입력한 후 시뮬러伯1션을
실행한다．

488

PART 04. Simulink설계하기

匿三如呵江璽區3
듸m미帥on Ow日
Start tint日

4아H

Sw口 00w

小口

S미伯r 야川口nS
Ty口日 Vane닙寸etap
!

딥 S미csrt 區j旦 （0 orman于Puns日）

Add出anal D口don日

Mat et日P 늬Z日

ci／띠

딕미到四！이eranC日

1日日

卜川n 引日口 引Z可

out口

OO드D山let口leranc包

auto

nAsi 5伯口引Ze: a며0

Sha口日Ores日rm如It: [ 0由able 00

Numb日r 口lcon500Litbe mm 尉日pn

1

Zero -cros引fly 口口打口nB
Z日r口CrD5引fly o口nIT아 山日tao태B曲095
Ott日 toleranc日

ID너羽m口5

니 川ye曲m

Nonade口出e

돼yn引 Otr日oh이d a::山

Numb日rot conseca如日 i日r口 Cr口8퇴figS

ID刃

Ta的ing and samp油 Ott日 口口d口nB
勻卄1

T日B닙ng trod日 化rp日H口d七 5am미e 甘me5
好 A的m削Ca加 hand岫 rate 甘an므m口n 幻rdata 090引自r
已 네gher 口H口rhyoa山endlcatao higher task 口dod四
口：
；교＝ 乍斗＋斗臼m놔m斗；
;4二系쿄
；교；

口

1

二 됴n1

二m
0K

9

I 1 Cancel 1 1

Help

1

A口口m

그림 17小 시뮬레이션 매개변수 설정

四 시뮬레이션을 실행한 후 Sc叩e 블록을 더블클릭하면 스코프 창어써 싱크 함수를 확인할수 있다. 마우스
오른쪽버튼을누르고 [Configuration properties...］를클릭하여 창을 연후, 실행 결과를최적화하기 위
해 [V小limits 小4mimum上쪄］-0.3, [Y-limits (Max如mn) :］에 1.2를 입력한다．
q1 X축을최적화하기 위해 열려 있는 [Configuration 皿叩的es...] 창의 [Time］을클릭하고 [T油e span:]
에 肛pi, [Time display o侄配r］에 H恥pi를 입력한다．
i

기m日

0汨p由A

limes口an

L羽的9
9싸｝i

limes口an 0唯rrUn aC如n 八사ra口
lime an仕g
lim日 d治口lay 口Its oh
lime-acts lab日喀

싼叩므
小미
1 Bottomd冶口lays on奴

口 Show七m日aK治 lab日1

9
그림 17-7 스코프 창의 매7眼크수 설정

m 최적화된 시뮬궈昶］션 결과는 다음과같다．

그림 17田 스코프 창 결과

싱크 함수는 정숫값에서 모두 0을 지나고 진폭이 점차 감쇠하는 진동 함수를 보여준다．

CHAPTE日 ]7. 신호 및 시스템

489

1 예제 17- 2 1
지속적인 217卄 표본을 가진 이산 정현파 함수 玎川의 파형을 나타내는 시뮬링크 모델을 설계하고 그 결과를
그림 창에 나타내라 ．진폭 A= 1 ，각주파수 CL) = 0.5 ，위상 0= 2이다．

풀이

Os血e Wave 블록을 생성하고（[Sou四es卜囹mle 砥／aye]) 블록의 이름을 cos (0.5n+2）로 바꾼다．
0 블록cos (0.5n+2）를 더블클릭하여 [Amplitude:］에 1, [Frequency (rad/sec) :］에 0.5, [Phase (rad):]
에 pi尼+2를 입력한다．
미ne 叫aVe
oa巾ate 引n日 V18V甘
O(t) = Mcp.SIn(Fr日q.t.Phas日）+ B冶8
돼cc typed日伯rmln日5 小日 compute如nal日chr,i叩日 US日d. The
口aram日tern in lb日 押／口 ty口eS ar8 r미日ted through
Sam口les 口日r 口8加d = 乃pi/ )Fr日qu日ncy 1 Sa,ttpl日巾n日）
Number olaf눔미 5am口陋s = Phas日 1 Sam)이日日 口日r 口cried/ (2.pi)
Use the camp冶based 引ne 勻口e 卄 nUm日nC톄 口r口blame du日 t口
mn州叩 幻r Iarg日 rim日5（日9. cc日59口나 小 abs口山t日 rim日） 0CCUn
Forum日t마5

［如日 bee日d

미n日typ日：

lime It): Us日 늬mula甘口n亡m日

!]

the히的de
r
테a甘
D
Freqa日ncy (rad/ces):
as
Pheea (red):
p1/2.2
Sanrp伯 Wn日：
0
回 Inter口ret vent口r 口arameter5 aS ] 山

1

OK

1

Cancel

그림 17四 Sine 블록의 진폭, 각주파수, 위상 설정

0 시뮬레이션 결과를 명령 창에 나타내기 위해1To Workspace 블록을 생성하고（[Sink引中口0
Workspace]) 블록의 이름을蜘1]으로 바꾼다．
0 블록 蜘n을 더블클릭하여 [Variable name:］을 毛n으로 바꾸고, [Limit data points to last:］에 21,
[Sample time (-1 for i川ierited) :］에 1을 입력하며, [Save 白rmat:］을知ray로설정한다．
To 놔orbs口aC日
니卄日 in口U to sp日cited 卄m日serle已 array. Sr sfrucd네目 Inc 나口1客口aC已 For menu-besed
引m내a如n, data 冶 V汗loon In lb日 MATU好 base 니odvepace. Data is not aoai)ab匕 and) the
씨m내eden 出 猷口pp日d 口rpaused
To leg a bun 늬gnat, use Thmased日5 " 5a吃 佃seat
Parameters
Variable nemo:
K n

三1

Unrit data 口口intet口 1a5r

Denim的0n:
]
S日叩f口rmat 1 threy

! 1

Sc四 2 [) 引gsa冶 a可 +S 日reap (coecatena뇨 ci口n目 third 비m日nB幻n)

!

「7그 L口gte日d-p미U data as at ob)日Ct
Sample rime （나 幻기nherlt日d)
1

뇨）

1

OK

]

Cane日I

그림 17-10 블록 x[n］의 변수명. 자료점, 저장 형식 변환

490

PART 04. Sim메nk 설계하기

H日巾

rids다y

0 생성된 블록을 연결한다．
Fl矩

Ed作

\Flew ［거5하ay

昆, r
S巧

0기ago카It

듸mutation

An帥吟is

Code

Too枉

H帥1

" 邕믐 " L爭 心 ＼多 吼＞ 發 回 ,,, （弓 ! 幽 ,

1

e 團미G2
！皎

시

{i
4

,

1

(.

回
i回
［그
[m
t코
力
Rea旬

100%

＼加tab的叩먀ante

그림 17-11 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 [Model Configuration Parameters] 창
을 연다. [Start 血ne:］에 0, 囹幻p time:］에 20, [Max step size:］에 l을 입력하고 [S이ver 야)tions］의
[Solver:］를 小screte (no continuous states）로 바꾼 후 시뮬레이션을 실행한다．
：立Ca伯쿠口ryE區區쿄
十十1

散 ?nnnnat。口口It
:> 0pthrr注at岫n

籌毖믐'" "
) MDL Cod目 Gen自r削口n

Ome

띄muladon

S日lesS

Ste口 Un,日 20

Statt doe: 0
Solo日r 야刈DnS

司 S口loer: 區db百如 C0而U0나5 5由뇨미

Ty口미 i Variablo-otop
rAddffional 口口的n8
Mao Ste口 引ze:
Z日r0{mS由no 마｝ton日
Z日r0mCr口88n目C0n甘야 Uo日 'Os叫Be싸1四8
lime to岫ranC日

티 씨geriltin,.

山너28四口S

i 8口nod日p如日

미on계 U.日Sh口Id

Numb日r01 COflO日CU巾e Z8r0 CrD5引noo

크U小
1dL

T日0150 and sompi日 So 口口tono
Tao녑no mode 伯r 口日dod七 日am口뇨 dm日5;

向工0

野 加幻m削Ca四 handle rote 甘an出如nor data 甘an8伯r
團 I4坦her 口n0r却 wise ind七at日C hIgh日na敬 口n미却
1

노＝m斗＝

m曲心如뵤쏘소二二二느日H小＝

m뇨呻기如

1

r

口口

9

U

,

尸

［玉洹五；
匣仄그

! 卜

m

如ply ]

그림 17-12 시뮬레이션 매개변수 설정

0 시뮬레이션을 실행한 후 다음과 같이 명령 창어i 명령어를 입력한다．
Comma d T/ir,dm

今

>> 000:1:20;
>> stem(nx. n) ;
,, grid on;
>> olahal ( 'Tinte [n] ');
>> 니 oh미 ( S [n] " ) ;
>>title ( Discrete 돼ooal ) ;

그림 17--13 시뮬레이션 결과를 그리는 명령에 입력

CI-IAPTE日 ]7. 신호 및 시스템

491

0 이산 신호 정현파 그래프를 보여주는 그림 창이 생성된다．
File

Ed注

Vtsw

II肖1甘t

Toots

r比出t叩1 叫hMm 卜Ietp

D 亡｝ a 色 i 4 匹＼曳 助自咀 / 니目1 日 1긔 . 口

智們Signal
O

0,5

45

i
,

O

O

,
"O

O

1

E낯

1

O

O

O

0

5

10

20

Time In]

그림 ]7-14 이산 정현파 함수 그리기 실행 결과

MATLAB에서 제공하는 stem 함수를 이용하여 21깨陀l 기본 주기의 개수만큼 입력값20을 지정하고 이
값어］ 의해 생성되는 출력값x[n｝을 줄기 형태인 이산 신호 그래프로 보여준다．

1 예제 17-3 1
연속 신호에 대한 입력과 임펄스 응답은 다음과 같다．
x(t) =u(t+ 1)-u(t- 1)
h(t) = (- t+ 2)[u(t) -u (t- 2)]
신호값이 발생하는 시간 -6 드 t 드 6에서 입력 신호와 임펄스 응답 신호，입력 신호와 임펄스 응답 신호를
컨벌루션하여 생성된 출력 신호 y(t) 파형의 시뮬링크 모델을 설계하고 그 결과를 그림 창에 나타내라．

푿이

0 Step 블록4개를생성하고（[Sot丁ce司-[Step]) 블록의 이름을각칵u(t+1), u(t크）, u(t), u(t-2）로
바꾼다．
0 블록u(t+1),u(t-1),u(t),u（卜기를더블클릭하여 [Step血ne:］어］각각크, 1, 0, 2를입력한다．
0 Sum 블록 3개를 생성하고（[Comm恤y Used Blocks卜田m미） 더블클릭하여 [Icon shape:］를
rectat鳩ular로 바꾸고블록2개의 工奴 of signs:］에 +e, 블록 1개의 工慨 of signs:］에＋瑨 입력한다．
0 직선 함수 나를 나타내는 Ramp 블록을 생성하고（[Source日 ［Ramp]) 더블클릭하여 [Slope:］에
[S杻rt time:］에 十, [Initial 에tput:쪄陌을 입력한다．

492

PART 04. Sim네nk설계하'I

1,

Ramp (mask) (tnk)
Ou巾Lit S ram口 引gnai eta州ng at tile a口日C出ad
甘me.

I
!

由rameters

:

Start time:
4
1

]
1

in付졔口U巾Utt

!

［包 mnt日r口ret vector 口cram日mere as 卜［)
i

]

Canc텍

H미p啣a,

그림 ]7-15 Ramp 블록의 기울71. 시작 시갼 초기 출력 설정

0 Constant블록을생성하고依ommonly Used Bloc虹］水力ns切蝴）더블클릭하여 [Con戚ant value:］에 2,
[Sample time:］어m을 입력한다．
Constant
Output 出cc口netant a口日cifled by tile 'Constant va山e param日Icr, if
'Constant V눼나日 Is 日 V日C幻r and 'in伯rpret V日ctor 口arametere as卜D' 冶
on』h日at the constant vs山e as a 1나） array 아l日i-wise, a니tl그Ut a mali-Ia
叫附） tile same 비men引one as th日 constant valu日．
Main 1 Siyrial Attributes
Conetant value:
2
團 Inter口r日tv日ct口r paramet日rs as 卜［)
Sample 打me:
0

Canc톄

0K

0

H日巾

! A口口！/

그림 17너6 （丸rtstant 블록의 상숫값, 샘플 시간 설정

0 Product 블록을 생성하고（[Commonly Used Blocks卜[Product]) 더블클릭하여 [Number of inputs:]
어］ 2를 입력한다．
Product
M山如ii or di너d日 in口U怡． Cho口55 미em日nt小너ee or matrit< 口roduct and
spec的 on日 of th日 f口lowing:
a) * or/ I口r 日ach in口u냐tort, For 日sampi日』1t/1 口日forms tile 야甘削on
'ul*u2/u3.u4.
b) sc톄ar a口日C州evil日 number of In口Ut 1그口nv t（그be mu出口H日d
U there 治 口nly oil日 input 口口rt and Il日 M山如妃at幻n 口arame伯r 冶 S日Ito
티日msnt-L너5日（1）』 a 引ngle 1 or / coila口C日eth日 in口Ut 引fin비 니引ng th日
S口日口hi日do口eration, Hoe心V日r, if th日 Mu恤꿰cation param日ter 冶 8日Ito
Ma州xl.), a 비n이日 1 causes th日 비ock to 口U巾Ut the matrix 니nchanged,
and a 引n미日 / caus日elI日 비0口kt口 口니tp나I the maids inn日re日
卜Aain

텨gnal A쌔bu伯百그

N니mbsr 口I In口ute
2
Mi朮巾n口all口K 티em日nt-a的日（미
4

rr1 心tH，出．m＝心3小

0

니
11r

匕그卜＝匹可而r] 1匪亘그

，叱吐쿠쿠日日m寸J 卜

A口ply

그림 17-17 Product 블록의 입력 단자 개수 설정

0 To Workspace 블록2개를생성하고（[Sinks]-[To W아kspace]) 블록의 이름올각각由put, in叩ulse로
바꾼다．

CHAP在R 17. 신호 및 시스템

493

On叩Ut 블록을 더블클릭하여 [Variable name:］을 毛t로 바꾸고, [Limit data points to last:］에 1201,
[Sample time］에0．아을입력하며, [Save format:］을A口ay로설정한다．
0 impulse 블록을 더블클릭하여 [Var佃ble name:］을ht로 바꾸고, [Limit data points to last:］에 1201,
[Sa끄叩le仕me:］에 0.01을입력하며, [Save format:］을Array로설정한다．
四 생성된 블록을 연결한다．
q1 설계 창의 메뉴 표시줄어써 [Simulat伯n] 메뉴를 클릭하여 [Model Configuration Parameters] 창을
연다. [Sta毗 time:］에 -6, [Stop 血ne:］에 6, [Max step s倪e.］에 0.01을 입력하고 [S이ver options］의
[Solver:]를ode45 (Dormand-Prince）로바꾼후시뮬레이션을실행한다．
File

Edit

Vie나

[)isplay

回, 圄

［거a드pram

듸m出ation

Ana啼5

Code

bogs

Help

" 龍 " 呻 田 唯 q> C Ed ,,, 回 , 芯｝ ,

미64
團師4

!

띠1

：臂

묘1}
=6

咐1}

느업가1늬 ,J

r下-

I

낟JH4니

團
1回
口

따기
'"

E口
的

1

1거｝山

:

h4잡1긔11

［끄U

口H P "

' "'

늠U
"

＝口

으

>>
Rea旬

101）美

그림 17-18 완성된 시뮬링크모델

m 다음과 같이 명령 창어］명령어를 입력한다．
0ommari4 lVndow
0> t=-6:0. 01 :6;
>> y._t=conv (x_t . 九t）山口1 ;
>> subplot (311) ;
>> 미口t (t, x느t) ;
>> 카ds(［七 6 0 31) ;
>> ylobel (x (t) );
>> su뱌lot（데 2) ;
>> 미 叭 (t 小-t ) ;
>> axls([七 6031) ;
>> ylabel (h (t) );
>> oubplot (313) ;
>> 이 ot (t. y_t（印1:1m1 1) ;
>>ylabel (y (t) );

그림 17-19 시뮬레이션 결과를 그리는 명령에 입력

494

PART04. 針ilu加k설계하:7 '

ode45

m 입력 신호, 임펄스 신호, 두 신호를 컨벌루션하여 생성된 출력 신호의 파형이 그림 창에 생성된다．
円e

Ed比

VS？卄

h均ert

化아S

D喀求的p

쌔n寸w

H叫p

｛그 d a 企 公 1！曳 二＼ 抑 @ 曜 而 , 邑 口 들引 口 口
3
;

2

'S i
0

.4

0
七
3

2

6

= 2
V

= 1

-2

-4

-6

0

0

4

6

4

6

0
好

-4

長2

4

0

2

그림 17-20 연속 신호 컨벌루션 실행 결과

MATLAB에서 제공하는 cony 함수는 입력 벡터 신호와 임펄스 벡터 신호를 컨벌루션하여 새로운 다항
식인 출력을 생성한다. 컨벌루션 적분의 근삿값이 실젯값어］ 가깝도록 시간 간격을 충분히 작게 0.01로
잡았다. 컨벌루션 후 시간 간격 0.01과 비례를 조절하기 위해 0.01을 곱한다．
0.01씩 나눈 시간 간격 1201개에 대한 입력 신호와 임펄스 응답 신호의 원소 수는 1201개이고, 컨벌루
션 연산을 한 이후 출력 결과의 원소 수는 2401개이다. 이때 출력 결과의 그림을 그리려면 다른 배열 원
소 수와 같은 1201개로 맞춰야 한다. 출력 결과의 원소 수를 12011로 조절하려면 2401깨1 원소의 중앙
부터 좌우로 600개 원소를 배정한다. 즉출력 결과 원소 601부터 1801까지 12017거1 데이터를 이용한다．

CHAPTER 17. 신호 및 시스템

495

LESSON

02

신호를 전달하는 모델 설계하기

갸ans旭r Fcn 블록을 사용하여 또는 사용하지 않고 신호를 전달하는 모델을 설계하는 방법을 알아보자．
I 전달함수 1

Keyt사ord

I

전달함수

전달함수는 분수의 분모와 분자어］지정되는 매개변수어］ 전적으로 의존한다. 단일 입력어］대한 단일 출력
시스템에서는 상수 시간 영역 신호 모델을 설계하고, 단일 입력어］ 대한 다중 출력 시스템에서는 상수 입
력어］대한 벡터 출력 모델을 설계한다．

1 예저117- 4 1
0 드 r 드 5에 있는 방정식 y +3j+ 2yr2u(t) -3가(t -3）을 푸는 시뮬링크 모델을 설계하고 그 결과를 스
코프 창에 나타내라 ．초기 조건은 y(0) = 0 ，只이 = 0이다．
;:;

쿄iuI

(a) 2차미분방정식의완성된시뮬링크모델은다음과같다．
File

Edit

니eW ［거splay

Diagram

區｝ , 圄

듸mulaton

All叫ysis

C에e

bo匡

Hel口

琵 " 呻 왜 3 1卜 匹 凹，》》＼口 , d．
彗！

TPN'il ]
!

團T日AN1

e

風

ii
ii

-

,．訌
됴

匠쿄
4
［回
國
［그

,三，

三，

,

品

f亡
幽
>,
Rea旬
그림 17- 21

l伉胱

oda4s

2차 미분방정식을 이용한 시뮬링크 모델

(b) 라플라스 영역 변수S를 사용하는 전달함수로 주어진 시스템 모델을 설계하자．
0

Step 블록2개를생성하고（[Source司- [Step]) 블록의 이름을각칵ul, u2로바꾼다．

0 블록ul을더블클릭하여 [Step time:］에 0, [Final value:］어口를 입력하고（2u(t) ) ，블록u2를 더
블클릭하여 [Step time:］에 3, [Fii也1 value:］에 3올입력한다（3u(t寸3)),

496

PART 04. Sim메nk설계하71

Ste口
Cu如니ta 引e口
Paramnt마5
St目口 timtr
3
In出ci 恒山e:
0
日n계 Ca山e.

百

Sam이日 WOe
0
團 inter가日I vector 口aram日也rs as 1-ID
團 Scab由 Z日ro-cr口S늬ng d日虹如n

OK

C帥C日i , 口回＝

그림 17-22 블록 u2에 계단 시간과 계수 설정

0

Sum 블록을 생성하고（[Commonly Used 미ocks卜囹urn]) 더블클릭하여 [Icon shape:］를
rect町엣lar로 바꾸고 [List 可sigl好：
］에＋ 를 입력한다．
Sum
Add or subtract in口U怡， S口cc加 one of that에0늬tng:
a) uSing containing + or 幻r 日ach in口Ut 口nit I 幻r spec日r betwe日n
口orts (e.g. -I니＋+)
b) see泊r, >= i, s口edt日5the number of in口Ut 口orts to b日 summed.
WI-ten there is only one input port, add or subtract elements over alt
dimens幻Os Or 口fle specified 버men引on
Main

Signal Attributes

to口n sha口e: ft日St日nguiar
U引 of 引g0s:

. 1

1

1

1 뇨C日PC빈

쁘P j

543Pty

그림 ]7-23 Sum 블록의 형태와 부호 설정

0 직사각형으로 바뀐 Sum 블록을마우스로 클릭하여 크기를 확대한다．
0

전달함수를나타내는Transfer Fcn블록을생성한다（[Continuous卜［Trans也rFcn]),

0

Transfer Fcn 블록을 더블클릭하여 困Un配rator coefficien臼：
］에 단위 계단 함수의 라플라스 변환
값 따을 입력하고, [Denominator coeffic油its:］에 출력의 라플라스 변환인 s2+ 3s+ 2에 대한 계
수 [132］를 내림차순으로 입력한다．
Trans伯r Fcn

4

The numerator coefficient can be a V日Ctor Or matrix 日X口r日S引on
Th日 denomina幻r Co日fflcient must b日 as日ctor. The ou如Ut 니衣批Ii
equals the number of ro나s In the numerator coefficient You
should op日city the co日Sc汨n始 In desc日nding on地ro如애甘usfs.

"
q

Paramet카S
Num日ra幻r cue伽扼ntB:
[I]

'
卑

［沁nomin餉口r COe佈C陀nit틔
[1321

j

敞田olute I미crane可
auto

Stat日 Name: (e.g., ’口5sf的n.)

8

i

OK

1 1 Canc日1 1 1H而

1

Ap帥

그림 17- 24 뀨ansfer Fcn 볼록의 분자와 분모 계수 설정

CHAPTER 17 신호 및 시스템

497

0

Scope 블록을 생성하고（[Sinks]- [Scope]) 블록을 연결하여 모델을완성한다．
File

帥I

Ww

0R好m1

0固：出寸

되mul川把C

Ana四S

同 ' 圄呻 中 ' 渭듬 ' 呻 텍8 1P !

Code

七ols

囹"

He巾

回 ' 幽'

TRAN2 1
!

團TRAN2

e

煎
툐l

ii

=1

ii

團
口
［立
鹵

I

工士；
Tr日거iferF口기

11

［二
5口耳e

力
100%

Rea旬

ode45

그림 17-25 완성된 시뮬링크 모델1

0

설계 창의 메뉴 표시줄어써 [Simul硝on] 메뉴를 클릭하여 [Model Configuration Par町neters] 창
을 연다. 115切rt 血ne］에 0, [Stop 山ne:］에 5를 입력하고 [Solver options］의 [Solver:］를 ode45로
바꾼 후 시뮬레이션을 실행한다．
日le

To此

니州

돠mid毗Rei

Help

m

@ 나 宅 e b n 1 帑 n q 4꾜 나 f 囚 ,

旺S而

그림 17-26 스코프 창 결과

［그림 17-21］의 모델을 시뮬레이션하고 스코프 창을 클릭하면［그림 17-26］의 결과와 정확하게 일
치함을 확인할수 있다. 결국［그림 17-26］어써 추가적으로 사용한 Integrator 블록과Gain 블록을
Transfer 民n 블록 하나로 대체해도 결과는동일하다．

1 예제 17小

1

0 드 t 53에 있는 다음과 같은 방정식을 푸는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라．
이따1J(t) = 20u( tm1다，
戈＋3i: +2工＝/(t) , 工（0) =i (o) = 0
戶4尹＋15y＝工（t).

498

PART04. Sim매nk설계하기

y(o)＝多（0) =0

(a) 2차미분방정식의완성된시뮬링크모델은다음과같다．
F泌

Ed比

\hew

Dis텬ay

［긔agran}

듸mutation

鸚

"呻 때 8

픈弓 , 圄

Analyr；朽

Cc巾

昑 ,

in的＄

H叫P

匹，甘 9 , 硅自 ,

]
니

THAN3

同而；

1
1
目
烈
{1
4

1

..
口

回

i
i1

,

t田片0

,；的

e

a

于
10甘2

ii

口

1

드

if 戶勺
；

叫0片0

:"

I

11

a

뇨

CDd3

브

,,

岫；

甘身 "I

!,1

二＝

Ready

100%

ode45

1

그림 17-27 2차 미분방정식을 이용한 시뮬링크 모델

(b) 라플라스 영역 변수S를 사용하는 전달함수로 주어진 시스템 모델을 설계하자．
0

Step 블록을 생성하고（[Sour四司-[Step]) 블록의 이름을f(t)로 바꾼다．

0 블록只t)를더블클릭하여 [Step time:］에 0, [Iin카value:］에 20을입력한다（20u(t) ).
O 전달함수를 나타내는 Transfer Fcn 블록 2개를 생성하고（[Cont血uous］寸Frans免r Fc미） 블록의
이름을각각Trans_fnl, Trans 如2로바꾼다．
0 블록 Trans fnl을 더블클릭하여 困U毗rator coefficients:］에 [1］을 입력하고, [Denominator
c此fficien始：
］어］출력의 라플라스 변환인 52+ 35+ 2어］대한쟈수 [1,3,2］를내림차순으로 입력한다．
0 블록 Trans_fn2를 더블클릭하여 [Numerator coefficients:］에 [1］을 입력하고, [Denominator
coe丘'C奴吐5.］에 출력의 라플라스 변환인 s2- 4s+ 15어］ 대한 계수 [1,-4,15］를 내림차순으로 입
력한다. 여기서 [1,-4.15］와 [1 -4 15］는동일한 입력 방법이다．
Tren酊or Fcn
The numerator cc日捐ci日itt can be a vector 口rmatrix 日X口r日S引口n.
Th日 d日n口minator coeffici日nt must be a vector. Th日 0니巾ut wi배n
equals die number of ro느V8 in 出enumerator C口efficient V口u shou川
specify di日 coetfici日n怡 iri d日scending order 口1 口owers 口f5,

긱
H
디

Parameters

=

Num日r計口r cv日州c汨nt酊
[ii

르d

거甘

Denomin帥가 c口帥cl帥to:
(t.-4.15]

三

仙80山佃 t口1日ranc5

--

as伯

三

드

St日Ia Name: 佃．9'. 'pacitl口0')

9

OK

' Cancel ]

He巾

VP西그

그림 ]7-28 블록 Trans_fn2의 분자와 분모 계수 설정

CHAPTER 17 신호 및 시스템

499

0

Scope 블록을 생성하고（[Sink司-F毓畔］) 블록을 연결하여 모델을완성한다．
태o

ld吐 ＼艇W

匈｝ ! 圄 놔」

O탸加y

DI寸帥） 듸m미ab에

加낙川5

" 龍 " 呻 ＜吐 四 恥＞

Co巾

b帥드

H叫p

E크 !，》 (9 , 幽 !

THAN4 i
回Th州4

口
4

[n
i1

!

, 姑미1
I

- 7:i;1i

耳ii而m

i미1 忙

尸1

:

［二
Smm

好
團
［그
心
由
套
l伉戊

F出畇

새b45

그립 17느四 완성된 시뮬링크 모델

0 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 [Model Conf培uration Paran妃ter可 창
을 연다. [S切rttime:］에 0, [Stop time:］에 3을 입력하고 [S이ver options］의 [S아ye川를 ode45로
바꾼 후 시뮬레이션을 실행한다．
目h

1岫

니m

的마1

O 니 4 0 b 끼 各 n 風 ,［그 1 + 囹 ,

그림117-羽 스코프 창 결과

［그림 17-27］의 모델을 시뮬레이션하고 스코프 창을 클릭하면［그림 17-30］의 결과와 정확하게 일
치한다. 입력只t)를가진 2차미분방정식의 변수工를 먼저 풀고 입력 工를가진 2차미분방정식을풀
면 변수.3릍 찾을 수 있다. 그러므로 변수工를 사용한 2차 방정식의 라플라스 변환에 대한 각 계수를
Trans_fnl의 분모에 먼저 입력하고 ，이어서 변수y를 사용한 2차 방정식의 라플라스 변환에 대한
각 계수를Trai好느血2의 분모에 입력한다．

500

PART 04. Sim메nk설계하71

LESSON

03

필터 설계하기

특정한 형태의 주파수 응답을 가진 필터를 이용하면 필요한 성분의 신호만 통과시키고 잡음 혹은 회로의 동작을 방해하는 특
정 주파수는 감쇠人키거나 제거할 수 있다． 다양하게 사용되는 필터 중에서 저역 통과, 고역 통과 필터의 시뮬링크 설계를 알
아보자．
Keyword

1 저역 통과필터 1 고역 통과필터

Lowpass 디ter블록 i 네ghpass 테ter블록

1 Spectrum An졔yzer블록

I

저역 통과 핌터

저역 통과 필터 (LpF: Low-Pass Fil妃r）는 낮은 주파수를 통과시키고 높은 주파수를 저지한다. 이때 통
과 대역과 저지 대역을 구분 짓는 경계 주파수를 차단 주파수（cut可r frequ이兀y）라고 한다. 즉 저역 통
과 필터는 차단 주파수까지의 주파수만통과시키도록 설계한다．

I

고역 통과 핌터

고역 통과 필터 (HPF: i玉gh-Pass Filter）는높은주파수를통과시키고 낮은주파수를 저지한다. 저역 통
과 필터와 반대로 고역 통과 필터는 차단 주파수 위의 모튼 주파수를 통과시키도록 설계한다．

I

Lo出pass Filter 볼록

입력 신호의 각 채널 중독립적으로 낮은 주파수만 통과시키는 저역 통과 필터용 블록이다．

I 네ghpass Filter 블록
입력 신호의 각 채널 중독립적으로 높은 주파수만 통과시키는 고역 통과 필터용 블록이다．

I

Spectrum Analyzer 블록

Spectrum Anabzer 블록을 이용하면 신호의 주파수 스펙트럼을 나타낼 수 있다．

CHAPTE日 ]7. 신호 및 시스템

501

1 예제 17出 1
주710 드 t 드 3.5이고 샘플링률이 0.0001인 다음 세 정현파 신호 중 가장 낮은 주파수 100[Hz］만 통과시키
고 300[H지와 500[H기를 저지하는 필터의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라．
x(t) = sin(200,rt)+ sin(600irt)+ sin(1000,rt)

풀이

0 Sine Wave 블록을 생성하고（[DSP System To아bo川-[Sot丁ce司-[Sii妃 Wave]) 블록의 이름을 각칵
xl (t), x2(t), x3 (t)로바꾼다. 블록xl (t), x2(t). x3 (t）를더블클릭하여 [Frequency (H기:1에 각각
100. 300. 500을입력하고［S跏pie time:］에는모두1/10000을입력한다．
0 Add 블록을생성하고（小4ath Operation司-[Add]) 더블클릭하여 [List of signs:］어］ ++＋를 설정한후
[OK] 버튼을 클릭한다. 그리고 마무스：를 이용하여 블록의 크기를확대한다.
0 Spectii口m Analyzer 블록을 생성하고（[DSP System Toolbox]-[Sinks]-[Spectrum Analyzer]) 블
록의 이름을x (f）로 바꾼다．
0 블록 x (f）를 더블클릭하여 스코프 창의 환경 설정을 위한 [Spectrum Settings] 버튼을 누르고 [Fstart
(Hz) :］에0, [Fst이） (Hz):］에 600, [Wind이기ength:］에 16384를입력한다．
0 Lowpass Filter 블록을 생성하고（[DSP System To이比町U四沚帥l닙- [Filter Designs]-[Lowpass
Fi娩r] 블록의 이름을 LPF로 바꾼다．
0 블록 LPF를 더블클릭하여 다음과 긷＜기 매개변숫값을 지정한다．
山叩a88 日11目r
0日밗日neARer H日 佃州ass titer
S口나rca cod日
Main
Data 了y口e旨
'cram日伯r目
日如rtu口日

麟t寸

團 D日늬gnmiflimum Order n卄er
Paseband edge frequency (H,):

(刃

S幻pband adg日frequency (H寸

an

M日뇌mUm 口a55band n口미目 (d日）:

001

베nimum St미北日nd 01的nU帥on Idol: 10
巴 nh日.0 sampler日tefr口minpid
H口01 semI뇌日 m的 (Hel

1dl刃
出岫 如r日aa帥刊

미rnula伯 U引ng 1k如1W的dec日C1加n

1 0K

9

f Ccrrc日I L Ho如

그림 17-31 블록 四F의 매개변수 지정

0 블록을 연결하여 모델을 완성한다．
nit

日itt

nl.寸

Dl；꺄까

曷,目

1乂呵거기

1 鸚

SAc出啣1 M畇哨 口巾 t心

1螂

片呻 弔 回 11> , 巨r片 (9 , 筐自r

日LI I
01

｝團日LI

먹
툐i
4
巨i
口
口

臼，

m

!

碼

母 I =.
mg目

뿌

心吻

柚

l（刃花

그림 17-32 완성된 시뮬링크 모델1

502

PART 04. Sim몌nk설계하71

!
＼似rat卄e또epa站cell

0 설계 창의 메뉴 표시줄에서 圄mulation] 메뉴를클릭하여 ［卜4odel Configuration Parameter司 창을 연
다． [S切rt time:］에 0, [Stop time:］어］ 3.5, [Max step s倪e.］에 1/10000을 입력하고 [S아ver options]
의 [S아ver:］를 discrete로 바꾼 후 시뮬레이션을 실행한다．
F如

Tools

VI汁

S如札岫be

巾

固 ' @ 卜 1 1 各 ' 1 目 ' i［꾜 囹 四咽 團［夏

그림 17-33 스펙트럼 스코프 창 결과

저역 통과 필터를 사용했기 때문어］가장 낮은 주파수인 10이I初］만통과시킨 진폭 스펙트럼을 보여준다．

1 예제 ]7- 7 I
주3Io 드 t 5 3.5 이고 샘플링률이 0.0001인 다음 세 정현파 신호 중 가장 높은 주파수 500[H지만 통과시키
고 100[H기와 300[H기는 저지하는 필터의 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라．
x(t) = s自n(200,rt)+ sin(600,rt)+ sin(1000,rt)

풀이

0 ［예제 17小］의 ONo를 반복한다．
0 Highpass 꺼iter 블록을 생성하고（[DSP Sys奴n Tool加幻-[Fi如血뒝-[Filter Desig祠-[Highpass
Filter] 블록의 이름을HPF로 바꾼다．
0 블록 HPF를 더블클릭하여 다음과긷岫1 매개변숫값을 지정한다．
f카gh口ass F카也r
Se引gn a 日R or hR 비ghpass filter
a口urc日 code
Main

Data Types
Paraneters

19fterty口日

風B出二珏協磁朴騷融m蜘m的如玉

團 Do引gn minimum 口rd日r Ii忙Cr
S幻口band edge fr日qu日ncy (Hz):

可L

Passband edge fr日qu日ncy (H寸

A仄）

Minimum St口pband 帥enUa心口, (dO): 60
Maximum 口assband ri口비e (d日）:

clot

巴 1nh日r卄 Sam미e rate from In口Ut
input sampi日 ra也 (liz)

卜而可日恒rR日S口口nsa
Simulate using:

9

reted 日X日C나t油n
OK

Canc늬

H日巾

그림 17-34 HPF의 매개변수 지정

CHAPTER 17. 신호 및 시스템

503

0 블록을 연결하여 모델을 완성한다．
F油甘

E出t

W曲 D螂切

昆 ! 四 k1 ,

D1們1

Sh1HJ1哺口｝ M빽戶枉

C0巾 自帥i

He巾

m旨믐 心 ! 片 呻 텍1 8 1PU 匹 ！勿 @ ! 蟲 !

日L2

토｝
=0

므

쁘
心

!

1凸
I \?
X1{4

1n戶P

卜
HUF11

［그교
Xaq

I까sP
［그I?

1

叩c
뇨．

：哄

，으

回日L2

H1

U끼

1 지n

'

,

幽，

X긔q

Rea旬

100%

＼屈帥1eepDt

ete

그림 17小35 완성된 시뮬링크 모델1

0 설계 창의 메뉴표시줄어써 [Simulation] 메뉴를 클릭하여 ［卜4어lel Configuration Paran妃ter引 창을 연
다． [Start time:］에 0, [Stop time:］에 3.5, 小4ax step s切e.］에 1/10000을 입력하고 [Solver 아泊毗］
의 [S이ye川를 小screte로 바꾼 후 시뮬레이션을 실행한다．

그림 17-弱

스펙트럼 스코프 창 결과

고역 통과 필터를 사용했기 때문어］가장 높은 주파수인 500[｝七］만통과시킨 진폭 스펙트럼을보여준다．

504

PA日T 04. Simulink 설계하기

CHAPTER

CONTENTS
LESSON 0] 벡터와 행렬 연산하기
LESSON 02 벡터를 활용하여 설계하21

벡터와 행렬 연샨하기
시뮬링크를 이용하여 벡터과 행렬의 연산을 시각적으로 나타내보자. Math Function 블록을 사용하여 전치행렬의 모델을 설
계하고, Determinant of 3x3 Matrix 블록과 Invert 3x3 Matrix 블록을 사용하여 행렬식과 역행렬의 모델을 설계해보자, 또한
Log七계 Operator 블록을 사용하여 논리 연산자를 이해하고 Matrix Concatenate 블록을 사용하여 크래머 법칙을 알아보자．
Keyword

I Math Function 블록 1 전치행렬 1 Determinant 아3x3 Matrix블록 1
I Invert 3x3 Matrix 블록 1

행렬식 1 역행렬 I LogicalOpera的r블록 i

I Matrix丸ncatenate 블록 1 크래머 법칙 1

I

Math Function 블록

入4ath Funct幻n 블록을 이용하면 수많은 수학 함수의 계산을 실행할 수 있다．

I

전치행렬

행렬은 실수나복소수를 직사각헝 배열로 나타낸 것으로, 행이 m7거1, 열이 7尸11인 행렬 A의 형태는 일반적
으로 다음과 긷미 나타낸다. 행렬 A를 간략하게 m Xn 행렬이라고 한다．

A卄a1,

,,,,
,a,

행렬 A의 행과 열이 서로 바뀐 행렬을 전치행렬（transposed matrix）이라고 하며 AT로 표시한다. 전치
행렬 A씌 크기는fl Xj刃이고 다음과같이 나타낸다．

1 예제 18너 1

506

PART 04. Sim메nk 설계하71

[

3 1

9

。6

2

-

3] ,

0=

1 2

B=

4

A=

-

다음과 같은 두 행렬이 있을 때 새로운 행렬 C= A)< 甘를 구하는 시뮬링크 모델을 설계하고 그 결과를 나
타내라．

:;=

日
［IQ

지식

수학에서2행3열인행렬A와행렬B를곱하는것은불가눙하다. 수학에서는앞행렬의 열과뒤행렬의행
의크기가같아喉｝곱셈이 가능하다．BT의 위 첨자T는행렬B의 행과열을서로바꾸는전치（transpose)
를 의미하며，2행 3열인 행렬 B를 전치하면 3행 2열이 되므로 행렬 A와의 곱셈이 가능해진다．

풀이

0 Cons切nt 블록 2개를 생성하고（[Commonly Used Blocks卜[Const姻）블록의 이름을 각각 A, B로
바꾼다．
0 블록A, B를 더블클릭하여 [Cons愧nt value:］에 각칵［크 23:547]. [319:06-2｝를 입력한다．
Con欲ant
0u巾Ut the 口onstant sp日cified by the 'C口n日taft ye山e' 口arame也r. It
'Constant ye山e' 陌 a vect口r and In也r口ret vec幻r 口crams也rs as卜0' Is
on, beat 甘ye C口nstant ye山S as a 卜 ［) array. 0th日rwlse, o니tp나t a matr出
내仕h the same 曲neri引ons as the c口nstant valu日
Main

否自祠 商ribu也S !

Constant V카U日
［니 23547)
回 Interpret eec幻r par日me也rs as ] 山
Sam이e 心S）日：
nt

如布 嫡枷cc[

9

角He巾 包 P而而기

그림 18너 블록 A의 행렬 설정

0 행렬 B를 전치하는 Math Function 블록을 생성하고曲ath Operations]-[Math Function]) 블록의
이름을 TrHB로 바꾼다．
0 블록TrHB를 더블클릭하여 [Fun야jo'川을打anspose로 바꾼다．
Matti
Ma小ema配히 仙Sc如ns inclui出ng logarithm七 eaponential, p口＼yer,
and modulus 仙nctions 小hen 小e tunc卄口n has more than 口ne
argument, 꺼he 伽欲 argument corr日5口口nds to the t口p （口r 油It) inp나t
口口a
卜,lain

되gnal Attribu伯 "

Func如S [It anspos日
Out口Ut 引gnal ty口e

0

日U幻

0K

Cancel

H日巾

J

Apply

그림 18丑 Math Function 블록 뀨mB의 transpose 설정

0 두 행렬을 곱하는 Product 블록을 생성하고（
［卜4ath 야）町硝毗］- [Pro血ct]) 블록의 이름을 AB'로 바
꾼후 더블클릭하여 [Multiplicati아비을Matrix卜）로 바꾼다．

CHAPTER 18. 벡터

507

군
스 骨
i
t 年
4 i {i흩i玉毛毛m\ d

Product
Multiply or di4de In口내S. Choose 미ement- wise 口r ma甘怏 口rod니Ct and
S口日C啣 one otthe 幻如wing:
a) * or／伯reach inp니tport. For exam미e, 1t/ t 口ertorrns the 먀）er帥on
'ul*u2/u3*u4'.
b) sc쉐Sr s口ecities th日 number ot In口ott兀rtstob日 mu뺘川ed.
甘 It,日r日 冶 only 口ne Input port and the Mutt巾licat油n 口arameter is set to
日日m日n卜M鉀G), a 引ng冶 t 口n /c口ha口sea the Input 引gn톄 U引ng the
5口ecliled 야旭ra如n. H口叫e怡n. if th日 N仙州p1七硝口n 口aram日ter is set to
Matrlx(*), a single t causes the block to o니tput the matrio unchanged,
and a 引ngl日 / causes the block to a니的ut the matrix in蛇rse.

Main 뇨晷gnat脚bu始S
Number 口t inp나Is:
2
Multiplicat油n: 卜4abi戚0

0

!

Canc日1

0K

He巾

AP口如

그림 18-3 Product 블록 AB'의 곱셈 형태 행렬 설정

0I거splay 블록을생성하고（[Sit血可-[마叩lay]) 블록의 이름을C로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행한다．
File

Edit

\／田w

Disp啣

耳, 目

0咬恥m

S,mulation

Ma卜ns

C이契

秋出 卜k{P

萱,
" 呻 ＜心 上） 1口 』 囹 ,，》 U , d．

琵

WdC1

今 團h11Ct
m과1

h권中

규
A

뗍

I

zil

e

1

口- II

小1

1

11

1

M

二4

回
g團
口

.r

尸却1싸
寸

m

드크

4

욘

!

껸上

E刃

出
力
Re啣

a川mi吐蜘｛
蜘屯）

100%

그림 1+4 완성된 시뮬링크 모델

拍

6
10

I Determinant of 3x3 Matr以 블록
Determinat止 of 3妨 入latrix 블록을 이용하면 입력으로 주어지는 행렬의 행렬식을 계산할 수 있다．

I Invert 3x3 Matr以 블록
Invert 3好 入仁trb( 블록을 이용하면 3행 3열 행렬의 역행렬을 계산할 수 있다．

508

PART 04. Simulink 설계하71

H
1

陀

0 6 2

m/

3 l 9

X

4

U

<

八4V

:

스
二

C+

행렬 A와행렬 B에 대한 전치행렬 BT를곱하면 다음과같은2행 2열의 행렬 C를 얻을수 있다．

I

행렬식

행렬식 (determinant)은 행과 열의 수가 같은 정방행렬에 수를 대응시킨 함수로 기호 IAI 또는 det(A)
로 나타낸다. 행렬 A의 역행렬 A1이 존재하려면 행렬 A는 반드시 정방행렬이고, 행렬식의 값이 0이 아
닌(IAI 手 0) 정칙행렬（nonsingular matrix）이어야 한다. 행렬식의 값이 0인似1= 0) 비정칙행렬
(singular ma吐汶）은 역행렬을 가질 수 없다．

I

역행렬

행렬 A의 역수 형태는 A1로 표시하는데 이를 행렬 A의 역행렬이라고 한다. 행렬과 역행렬의 관계는 다
음과 긷히 단위행렬을 이용하면 쉽게 이해할수 있다．
A 'A =AA '= I

i

1 0似II ]8- 2 11
1

행렬 A의 행렬식과 역행렬을 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라．
寸

4,

그U

l

1

=

八
乙

l

l

A

니

U
4
n

0 Cons恤It 블록올 생성하고（[Co跏lonly Used Bloc畑卜[C毗tan日）블록의 이름을A로 바꾼 후 더블
클릭하여 [Constant value:］에［크 34；크 1 2;3 -11］을 입력한다．
0 행렬 A의 행렬식을 구하는 D毗erminant of 3x3 Matrix 블록을 생성하고（[Aerospace Blockset］中
[Utilities卜[Math Operations]-[1）毗erminant of 3焰 入4atrix]), 행렬 A의 역행렬을 직접 계산할 수
있는 血vert 3x3 Matrix 볼록도 생성한다（[Aerospace 미ockset卜[Utilities卜[1恤h Operations][Invert 3x3 Ma枉奴］).
O Display 블록2개롤생성하고（[Sit止s]山거splay]) 블록의 이름을각각det(A). Inv(A）로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행한다．
F켜b

E, t

V卜ew

DV甘ay

브各 ! 目

DIaVr. n

鸚

llmoVt幻C

An. 恥在

Code

boV

H叫P

丸唾多 q1 \9 小＞ 塑 巨3，片 回 , 芯自 ,

VMC2

自 團V?lC2

戴
E1
4

二
［그

!

쿠 ；璽，

' .

-+置J

壬이

]
;]

느3m勺h

h/［三）

m
丑1
力
m向

l며珌

aUt여＼缸mb沁StepD5crke)

1

그밈 18巧 완성된 시뮬링크 모델

CHAPTER 18. 벡터

509

［거agram

View ［긔splay

區｝ , 圄

Simulation

Ar녜州S

Cc＜如

가’

"

'1주어”

5]

［그림

Edit

，

t이s

八
乙

F妃

fCf

3]

8

' 8- 의모델에
행렬 ' 를행렬 "
대한 역행렬 BU1이 존재하지 않는다．

7-

0.

-

1.

-

。.2」批1
0.2

[1

-0.

.2

。.8
75

<
V

」」」小如뾰螂나0. 。
0.7
3

이로 " 枰면晤과긷히 " 1정칙행렬B에
3]

H심p

" 呻 叱 (8 聆 毋 낟3 나 回 ! 幽 中

目믐

VMC3
!

回VMC3

皎
1i크

'

"

=5

［뇨司1

，畿

e

븜

m\

啣

m1

m11r

啣

i 't

-"II

，到

I

m니

1
1

口

가31加h口

h州B)

E立

齒
分
View 1 esror 100%

Ready

aut* aiiabIe앉바）Oiscrete)

그림 ]8田 역행렬이 존재하지 않는 시뮬링크 모델

시뮬러卜기션 실행 후 역행렬 값이 표시되지 않은 디스푤귀徊］ 결과를 보여주고 이어서 오류 창이 열린다
（여기서는 생략했다）.

I

Logical 0口erator 블록

Logical Operator 블록을 이용하면 입력에 따라서 지정된 다양한논리 연산AND, OR, XOR 등을수행
할 수 있다．

1 예제 18小

1

벡터 x와 y가 다음과 같을 때 논리 연산자 AND. OR. XOR를 이용하는 시뮬링크 모델을 설계하고 그 결과를
나타내라．
x= [-4, -1, 0, 2]
y = [-2, 0, 0, 1]

푤이

0 Constat吐 블록 2개를 생성하고（[Commonly Used 미ocks卜[Consta蝴） 블록의 이름을 각칵 x, y로
바꾼다．
0 블록x, y를 더블클릭하여 [Coi始tant V可ue:］에 각칵［짜, 1,0,2],卜2.0.0.1］을 입력한다．

510

PA日T04. 針nulink설계하71

0 Logical Op町吼or 블록 3개를 생성하고（[Logic and B札 Opera如ns卜EL唯ical Operator]) 블록의 이
름을각각사JD. OR, XOR로바꾼다．
0 블록사寸D를 더블클릭하여 回perator:］는 기본값AND를 그대로 유지하고 [Icon shape:］는dis血ctive
로 바꾼다．
L口미C비 Oper計or
Lo미cat o口日rotor且 比ra 引09泊 input. o口erators are ap口lied ocr口ss the in口Ut vectc兀 F七r
mu川pie inp니to, 口口erat口rs are ap口1泊d across the in口U恒．
M궤0

: Da佑兀'p百］

O口日rat口r: PND

!

Number of inp나t ports
2
Icon sha口日： m娥nc加已

!

OK

9
그림 侶d

Canc日1

H日巾 ]

Apply

L四匕쉐 Operator 블록 AND의 아이콘 형태 변환

0 블록OR를 더블클릭하여 回pera加r.］는 (:)R로, [Icon shape:］는小毗ictive로 바꾼다．
0 블록XOR를 더블클릭하여 回perato川는XOR로, [Icon shape:］는dist血ctive로 바꾼다．
01거splay 블록3개卜를생성하고（[Sit虹］m［마叩lay]) 블록의 이름을각칵X&y, 시y, xXORy로바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행한다．
E0it

File

'ie叫 ［거sp匈 ［거agrarn

引mulation

AFOO如站

Code

i:）이＄

踞 年 , 團 , 呻 斗 @ 耶＞ !

囹! 圄

H叫p

巨크 ,

》，（多 ! 幽 ,

WC4
團Vt너C4

뷰

i

하
U1
心y

巨크

胃

'I

1
1
1

=

11

4

I
m田

［뇨q
y

1띠1

1
1

기

1

미

OR

1

1

1
1
I
1

11

믐

!

l]

e

켜y

11
01
01

!

이

工X{}ty

[1
曲
力
Pea旬

l仗民

000小危rlabiestepDiocrete)

그림 18田 완성된 시뮬링크 모델

주어진 벡터 x와 y의 같은 위치에 놓인 원소를 각각 비교한다.0인 값과 0이 아닌 값을 비교하는데，
AN]) 연산자의 경우 비교하는두 값 중 하나라도 0이면 결과가 거짓값인 0으로 표시되고, OR 연산자의
경우 비교하는 두 값이 모두 0일 때만 거짓값인 0으로 표시된다. 한편 XOR 연산자는 (xory)-(xand
y）와같은 결과가나타난다. 즉두 값이 모두 0 또는 0이 아닐 때 결과가 거짓값인 0으로 표시된다．

CHAPTER 18. 벡터

511

I

Matr以 Concatenate 블록

入4atrix C이icatenate 블록을 이용하면 메모리의 인접한 위치어］ 있는 출력 신호의 원소를 생성하기 위한
입력 신호를 연결할수 있다．

I

크래뻐 법칙

크래머 법칙 (Cramer's rule）을 이용하면 행렬식으로 된 1차 연립방정식을 체계적으로 풀 수 있다．

1 예제 ]8- 4 1
크래머 법칙을 이용하여 다음 선형연립방정식의 해를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라．

1 鈿＋入2U 7 55
j 9石＋5工2+ 4工3= 43
' 3=

匕5工'- 3工2 + 6工3 == -49
주어진 선형방정식이 3개, 변수가3개（石, 工2, 及）인 선형 시스템 Ax = c를 배열 형태로 일반화하면 다음과
같다·

푤이

6

＝二

2

［시

[ 55]

9 5 4 I' X지工
' I, e키L -49j
43
-5 -3 61
Lx3J
7]

A

-

m月＝
빼台
지식

0 행렬 A의 각 열을 입력할 수 있는 Constant 블록 3개를 생성하고（[Comm恤y Used 미ocks][Constant]) 블록의 이름을각칵A cl, A c2, A c3으로바꾼다．
0 블록A ci, A c2, A c3을 더블클릭하여 [C아istant value:］에 각각 [6 9 -5], 口 5 -3], [-7 4 6］을 입
력한다．
Constant
Ou巾Ut the c口nstant 5口ecifled by the 'Con針ant valu日‘ 口日ramet日r. If
'Constant Va山e ' is a 始Cf口r and Intert玎日t nedt口r 口aram日伯rs as卜0' 冶
口n, tr日at the c口nstant Va山日 ass I- U array. Othen너Se』口U如니t a mayix
내卄） the same 비men引ens as th日 constant nalu日．
卜lain

텨ynal 帥rib마es

C口nstant Va山日：
[69- 6]
團 In伯r口r日IV日Ct口r 口cram日也rs as 卜 ［)
Sam口泊 time:
mnl

He巾
口田口 C日nc日I
9
그립 18四 블록 凡C伯n 행렬 A의 첫 번째 열 입력

知口ly

0 상수 벡터 C를 입력할 수 있는 Cons佃此 블록을 생성하고（[Commonly Used Blocks卜[C毗tan日）블
록의 이름을 C로 바꾼 후 [Constant value:］에 [55 43 -49］를 입력한다．

512

PART04. Sim메nk설계하7I

0 크기가 같은 두 행렬을 하나로 묶는 데 사용하는 入4atrix Concatenate 블록 4개를 생성한다（[DSP
System Toolbox]-[Math Functions]-[Matrices and Linear Algebra]-[Matrix Operations][Matrix Concatenate]).
04개의 블록을 더블클릭하고, 3개의 열을 입력받을수 있도록 困umber o作叩uts:］를모두 3으로 바꾼다.
C口oca也nat日
Conca也na也 in叩t 引gna冶 미 小e Sam日 data type to crea伯 a
con甘gUoUS 0니t口Ut 引gnal. S비日Ct vector 口r mu川dim日n引on톄 array
mode
In vector mode, all input 引gnats must b日 帥h日rv日Ct口rs or One-rn낵
[toM] matric日日 口ron日＝C口lurnn [I巾dim甘눠CBS nra corn비nation of
vectors and 미ther 口ne寸ow maO'ic日s or one-c口lumn matrices. The
口Ut口Ut 冶 a sec伯ri all in口its are vectors. 재日 ou巾Ut 冶 a or,于ro나 마
one-c口山mn matHs 卄 any of the In口U怡 are 口n日＝0그나 or 口p日C口lumn
malrlc日5, respe口加e奴
In rnUltidirn日ns向nal mod日. use tonc計日na也 벼m日n늬口n' to sp日C啣
the 口U伯Ut 네men引口0 計口ng 니4,七ht口 C（그nc計enate the in口Ut arrays.
F七r esam미日』t口 C口rrcateflate the in口Ut arrays vertic톄］y 口r
horizontally, specify t or 2, respectively, as the concatenate
비rn日n引005
Parani日也r5
Number of inputs
3
Node: Mu싸뎨m日is幻nal array
Conc카日nate 비rn日OS油n.
2

0

乙町to臼1

1

H日巾

肉刑y

그림 18-10 Matrix Concatenate 블록의 입력 단자 3개 설정

0 행렬식을 구하는 Determinant of 3x3 入4atrix 블록 4개를 생성하고（[Aerospace 미ockse日H
[Utilitie司JMath Operations卜［Determin帥t of 3x3 入4atrix]) 블록의 이름을 각각 det (A),
det(A1), det (A2), det (A3）으로바꾼다．
［卜4ath O꺄rat油司-[D加ide]) 더블클릭하여 [Nun化er of i叩uts:］를 모
OD如ide 블록 3개를 생성하고（
두 序로 바꾼다.

Mu뺘tly or 비너de input요 Choose 틔日ment叫／S日 Or matr法 口r口du口t and

탑；“穹外旱빎썲怒楹 陌的巾.. .,/. 口.rf마mu th帥口.ra如.
'ut uZ1u3.u4'.
b) scalar 5口ecilies the numb日rot mnt가it 口Uris 幻 be multit川ed
If there is 口nly on日 input 1兀rt and if, 日 Mulllplicat幻n 口arameter 冶 set to
티日men卜wis日I..), a 引ng冶 t 口r/ colla口5日sth日 in口Ut 引gnal 니引ng the
specifi日d 口perat油p. Howener, ti the Mu如叱帥on parameter 洽 S日t to
Matrls(.), a 引n이B t causes if,日 비ockto out口Ut th日 matrix unchanged,
and a 引ngl日 //causes th日 비ock t口 口Ut口Ut the matris inverse.
卜Aain

蛋gn비脚but日＄ }

Number of in口U怡：
I.
Ix仙曲뇌七at山rr 旦日ment-vxfee（미

d ［面函

0

艸斗阡mm弘枷小m
[

m《劈
0K

尸

卞忖呻四

C日n口비

1

小小 叫忙닉 卜

H帥）

Apply

{

그림 18-11 DMde 블록의 새로운 부호 설정

0 Display 블록3개를 생성하고（[S如ks卜[Display]) 블록의 이름을각각xl, x2, x3으로 바꾼다．
0 블록을 모두 연결하고 시뮬러띠션을 실행한다．

CHAP正R 18. 벡터

513

F如

\/ie텍 ［거splay ［거agram

Ed捷

듸mulalon

Analys住

Code

bols

鸚 字 , 團 ! 呻 똬 @ 止＞ (

區3 , 目

-4叫p

므3 , D

月 (9 , 蟲 ,

V? 1C5

田 回Vs1C5

［그

구

A

I-

1
；
句1HH器】
4r
mH玉r!

A 口

＋十

C口呻'a

I

L;A臼
::J
1

, hm

1

中가

！石퀘1
:r I-孕
＜1[1
H11 1 1

1

뇨

릎

=

, , Ym1

i미

三

1
i:

I

風
口

!

-tt尸二-JI

1
1

d쩍All
仕과 1

U什口＝

山벼A1)'

1J山뇨

Xl

C이m1m11

！后겪11
:1경比111
1
r

H寸

1
1

d벼MI
｛뇨匈 1

냐團

.

I.

1

=

'

1

也씌，

:F

r二J

面려

1

U亡k
由U山m; !

U.口a
C이申出3

Ready

I

m;

到1

：싶

叫A3)

100%

' ,냐

I自

auto(VanableStepolscrete)

그림 ]8-12 완성된 시뮬링크 모델

블록 det (A）는 계수행렬 A의 행렬식을 구한다．

det(A) =

6

2- 7

9

5

-5 -3

4 = 118
6

블록 det (A1）은 행렬방정식의 오른쪽 상수 벡터 C를 계수행렬 A의 첫 번째 열에 모두 대치한 행렬의 행
렬식을구한다．

det(A1) =

55

2 -7

43

5

-49- 3

4 ＝二590
6

같은 방법으로 상수 벡터를 두 번째 열과세 번째 열에 모두 대치한 행렬의 행렬식을 구한다．

det(A2) =

6

55 -7

9

43

-5 -49

6

2

55

4 = 236, det(A3) =

9

5

43 ＝二 -354

6

-5 -3 -49

대치한 행렬의 행렬식을 계수행렬의 행렬식으로 나누면 선형연립방정식의 미지의 히；13개를 구한 결과를
블록xl, x2, x3에서 보여준다．
det (A3)
det(A1)
590 det(A2)
236
-354
工' = det(A) ＝了1죵＝> ' 工' = det(A) =11죵＝乙' 工" = det(A) ＝了i可＝乃

514

PART04. Sim메nk설계하71

LESSON

벡터를 활용하여 설계하기

02

Normalization 블록을 이용하여 벡터와 방향이 같고 크7마 j인 단위 벡터를 나타내는 시뮬링크 모델을 설계해보자. 또한
D아 Product 블록을 이용하여 벡터의 내적을 나타내고, Cross F가oduct 블록을 이용하여 벡터의 외적을 나타내는 시뮬링크 모
델을 알아보자．
I Norm訓zation 블록 1 ［兀tProduct 블록 1 Cross Product 블록 i

Keyword

I

Normalization 블록

Normalization 블록을 이용하면 입력의 지정된 차원에 대한 각각의 행, 열, 혹은 벡터를 독립적으로 정
규화할수 있다．

I

D야 Product 붙록

D아 Product 블록을 이용하면 두 벡터의 내적을 생성할 수 있다．

I

아oss Product 블록

Cross Product 블록을 이용하면 두 벡터의 외적을 생성할수 있다．

1 예제 18巧

1

풀이

1

2]

,

니
B=

\

A=

-

다음 두 행렬을 곱하는 시뮬링크 모델을 설계하고 그 결과를 나타내라．

36 0

0 Constant 블록 2개를 생성하고（[Commonly Used 미ocks卜田毗tant]) 블록의 이름을 각각 A, B로
바꾼다．
0 블록A, B를 더블클릭하여 [Constant v카ue:］에 각각 [-1 2;5 4]. [3 0;6 9］를 입력한다．

CHAPTER 18. 벡터

515

Constant
Outputth日 constants口日cifi日d by the 'C（그ns伯nt vs山e 口arameter, H
'Constant valu日’ is a vector and 'mnt日rr片日tv日c幻r 口aram日ters as 卜 ［)' 冶
口n. treat the con引ant value as a 卜 ［) array 아herwis日』Output S matr枳
with the same 네men引one as the c口n針ant va山包
M졔n 1 Sign뎄／싸ribut日S
C口nstant valu日：
［니 Z5 4]
團 1nt日r口ret vector 口日rameters as 卜 ［)
Sampi日 dm日：
mnt

뇨）

OK

]

Cancel

H日巾

Ap五그

그림 18-13 블록 A의 행렬 설정

0 두 행렬을 곱하는 Product 블록을 생성하고（[Commonly Used Blocks]-[Prod王ict]) 블록의 이름을
凡（B로 바꾼다．
0 블록AxB를 더블클릭하여 [Mult巾licati이r］을Matrix伊）로 바꾼다．
Product
Mu枷忖 口r 비너de in口U怡． Choose 비ement- wise 口rmatnls 口n그duct and
spec向 one 아 the 幻的내nyt
a) * or／幻r 日ach input po凡 比r exa叫de. "/ . 口erlarms the ot그erati口n
'ul. u2Ju3寸니4,
b) xc日lar 5口ecifles th日 number ot input 口口rts 幻 b日 mu出口n日d.
11th日r日 Is only one in口Ut 口art and th日 N仙脚lica如n 口aram日也r is set t口
티em日nt小너seC..), a 引n템日 1 口r/ colla口ses the in口Ut 틔gn톄 u늬ng the
5口日clued 0口erat向n. H口낚ever, 汗 the M니뺘쎄cati口n 口arameter Is s日tt口
Matrlx(.), a 引n미5 t causes the 비ockto output 甘伯 matrix unchang日d,
and a 引a미C / ca니5日sth日 t기口ck to out口at the matrix ins日rse.
M눼a

a

朴融蜘融士

Number of inputs

2
Mu出川ca如n.

'a

OK

[1西h而i그 ［ He巾 I

App

그림 18-14 1가OdUCt 블록 AxB의 곱셈 형태 행렬 설정

OI거splay 블록을생성하고（[Sii止可나n叩lay]) 블록의 이름을C로바꾼다．
0 선택적으로 이미 생성된 블록 A를 복사하여 붙여넣기를 실행한 후 블록의 이름을 Al로 바꾸고, 생성된
블록 C를 복사하여 붙여넣기를 실행한후블록의 이름을Cl로 바꾼다．
0 행렬을 곱하는 Product 블록을 사용하지 않는 대신에 (3am 블록을 생성하여 ([Commonly Used
Blocks卜［Ga血］) 블록의 이름을 B!로 바꾼다．
0 블록 Bl을 더블클릭하여 [Gaii비어］ [3 0:6 9］를 입력하고, [Multiplication:]을 행렬 곱셈이 가능한
入4atr奴 (U永K）로 바꾼다.
Gain

二

티日m日nt- wise g톄a (!/ = K,*u) 口rmatrix gain (y = K.u 口ry = u.K)

;

Main

目i'

텨gnat AtUibut日s

Parameter Attrtbu始S

Saint

立

13 口69]

J

Mu뺘네ca甘口at Matrlx(u나0

!

4 뇨心心恥甲斟鉀斟啣心畔畔蚣料‘斗只七4中斗和蜘神寸m뇩小卄心心呻mH小J 卜

'a

如-

Can口el

Help ,

Apply

그림 18-15 Gain 뷸록 Bi의 행렬 B 입력 및 곱섣1 형태 행렬 설정

516

PART 04. Sim매nk 설계하기

0 설계 창의 메뉴표시줄어써 毆mulation] 메뉴를클릭하여 [Model Configuration Parameter司 창을 열
고 田top ti毗］에 0.0을 입력한다．
@ 완성된 모델의 시뮬레이션을 실행한후 행렬의 곱셈 결과로 나오는 네 원소를 나타내기 위해 마우스 왼쪽
버튼을 누르고4개의 창이 모두 보일 때까지 블록 C를 확장하면 다음과 같은 결과를 얻는다．
c出 日虹

＼月e七V

미splay

O的ram

昆! r

듸mulatmn

鸚窄V

An키ys뇹

m心

"C肇 也 e

自여5

14e巾

1P ,1 回 !,, 凹 ! 邕 ,

WT1 ]
e 回h?.ITI

黛

!

二노a

므

A
Mi亡k
上

a出

taa

戶

｛六긔

1口
口

B

쓰.1

色＞

3

1드

Dq

二戶

=

C,

由
斗
R叫,

100%

auto(variabte닯epDlscrete)

그림 侶m恰 완성된 시뮬링크 모델의 동일한 두 결과

Product 블록 AxB를 생성하지 않고 Gain 블록을 행렬 B로 사용해도 두 행렬의 곱셈 결과는
C나니 2]lxi
>< [3 01= 1[9 18 뇨동일하다. 7陪하면블록의수가적으면서정확한결괴를얻는
L 5 41 [6 01 i39 361
모델을 이용하는 것이 최적의 설계라고 할수 있다．

i 예제 18- 6 I
i
벡터 A = 카 + 2幻

O Constant블록을생성하고（[Commonly Used Blocks］尸［Constant]) 블록의 "］름을A로닙睡후
[Constant value:］에 주어진 벡터의 각 계수 [1 2 -3］을 입력한다．
Constant
O山P니tO)日 C口nstanl op日口0日d by th日 'Cons怡nt 5졔U日 param日t日C 卄
'C口n마ants셰U日 Is a a日Ct口rand 'tnt日r口r日tyen幻r 口arameters as 卜 ［) 治
on, tr日atti,日 constant valu日 as a 卜 ［) array, Oth미V船B, oUtp니ta matrix
咐m m日 same 비m日n8幻Os as the constant valu日．
Main

미pit카姓曲肛5

Constant value:
It 2- 31
回 tnt日rpret 四ctor param日由r日日8 ] 寸）
Sam口岫 0n,日：
tnt

e

e

系i

3如에 대한 단위 벡터를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라．

OK

J

Can口ci

II叫）

二

그럼 18-17 블록 A의 단위 벡터 계수 입력

CHAPTEF국 ]8. 벡E寸

517

0 단위 벡터를 직접 계산할 수 있는 Normalization 블록을 생성하고（[DSP System Toolbox卜[Math
Fm姓幻ns卜[Math O꺄ra如ns卜[Normalization]) 더블클릭하여 [Norm:］을 2小norm으로 바꾼다（기
본값은 Squared 2-norm).
卜幻rma血計由n

-

Normallo日 th日 Input o叩r 由en口ecifled dimen引on by the nec幻r 2-nonir, sqrt（니'u)ob, 口r by 小e sq니ared 2-norm, u'u
+b, where b is a bias used to protect against di너de-by-zero. Normalization Is psrtormed over ro니／s, columns, or
the 비m日n引口n of the inp나t 引gn히 5口cc出ed in the 'Dimens幻n' 口arameter.
폴i
三

Main
C拍 Type디
Paramet마S
Norm: 匡norm
N口rrnalizati口nbins:

le니 0

Normalize oee(

Each column

旨拉可出出小小m如
d 나小小，

小

-

十m=m岫如出蜘七心用山山뇨小

,

出m小小，小

1 0K

9

mm,d 卜

] Can口비

[ Re巾

Ap따y

그림 侶너8 卜幻rio쉐zation 블록의 norm 설정

OI거splay 블록을 생성하고（[Si川（司-[꺄叩lay]) 블록의 이름을 乞A로 바꾼다．
0 블록을모두 연결하고 시뮬레이션을 실행한다．
F加

帥it

View

Dl唎啣

[)L呵ram

Sir!化以on

曷 ' 町4a 斗＞ , 踞每 '
VMT4 1

A.naly듸5

Code 自이S

He巾

" 呻 心七／ 8口 因 " ' 凹 ' 幽，

的 團V卞riT4

!

e

卜

A

I

1

e m,이
n田茹1

1

口m씨

N= m旺工1J기
_A

4

1似긔
H

亡i

d
［뎡
國
口

E口

幽
力
Rea肉

10啼

려血邱/ariab뇨璧e可가vcrete)

그림 18小19 완성된 시뮬링크 모델

시뮬링크에서 벡터 A의 크기를 구하는 norm은 3차원 벡터의 단위 벡터 계수를 제곱한 값
을 더한 후 제곱근을 취한 값을 구하는 함수이다. 디스플레이 창어써 보여주는 단위 벡터는
aA= 0.2673a工 + 0.5345勿 0.801鈿z를 의미한다．

1 예제 18- 7
벡터 A = 缸＋2ay- 3如와 B = -4ay +a죄 내적 A ·B를 구하는 시뮬링크 모델을 설계하고 그 결과를 나
타내박．

518

PART04. 鋤iuIink 설계하71

풀이

0 Cons切nt 블록 2개를 생성하고（[Commonly Used 미oc畑卜[C毗tan日）블록의 이름을 각각A, B로
바꾼다．
0 블록A, B를 더블클릭하여 [Coi胤ant:］에 각칵 [1 2 -3], [0 콕 1｝을 입력한다．
0 두 벡터의 내적을구하는Dot Product 블록을생성한다（
［卜4ath 야）町餌呻］-[Dot Product]).
O Display 블록을 생성하고（[Sink司-[Di叩lay]) 블록의 이름을C로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행한다．
F11甘

EdR

View

01W初y

固! 目

r再i9前1 Simulation

驅 巾,

Anafy引5 口心

Tools

Help

" 呻 邸 孕 聆 《7 E斗，》 也） , 蟲 ,

ViAT5

二

回VMT5

!

口

「

ThtPrn fl

C

.111

,

겅·

'
「：

臼
i回
［그

S

m
幽
Ready
그림 18-加

SOC戊

미J奴出泌m吼ePm町的町

완성된 시뮬링크 모델

벡터 내적의 결과는 방향 정보가 없는 스칼라 값 -11이므로 내적을 스칼라곱으로 부르기도 한다. 방향이
서로 다른 두 단위 벡터의 내적은 0이므로 벡터의 내적은 다음과 같다．
C =A ·B= (1)(0) + (2)(- 4) +(- 3)(1) = -ii

1 예제 怡田 1
벡터 A =-4ay +az와B = 鈿工 -2a의 외적 AXB를구하는人뮬링크모델을 설계하고그 결과를 나타내라，

系i

O Cons恤t블록2개를생성하고（[Commonly Used Blocks]-[Constant]）블록의 '］름을각각A, B로
바꾼다．
0 블록A. B를 더블클릭하여 [Constant:］에 각각 [o-41].[50 가를 입력한다．
0 두 벡터의 외적을 구하는 Cross Product 블록을 생성한다（[Simulink 3D Animation卜[Utilitie日H
[Cross Product]).
0 Display 블록을생성하고（[Sink司e［마叩lay]) 블록의 이름을C로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행한다．

CHAPTER 18' 벡터

519

F沁

Ed作 ＼加w

마5하ay

邸, 目
r VMT6 1

O畔ram

Simulat)on

目믐 每 ,

Ana)y引$

Code

" C申 唱 9

b汁I He巾

므目 1 匹 n (9 ! 幽 ,

的
團VMT6

!

侄긔

二

回
［그

[lx司

x
口m1枷C

!1=
中

U
口

41

風

C

(lx씌
日

心
幽
力
艇a旬

'C們

auto(V出rab)estepD四crete)

그림 18-21 완성된 사묠링크 모델

벡터 외적의 결과는 크기와 방향을 계속 보여주기 때문에 외적을 벡터곱으로 부르기도 한다 ．방향이 동
일한 두 단위 벡터의 외적은 0이므로 벡터의 외적은 다음과 같다．
C = A )< B = 鈿工 + 5ay + 入)az

520

71
PART04. Sim베nk설계하:

匹丘1匡

CHAPTER

19
통신

-戶口也R
--.口U口m1

1m1口II

a 1 irni

U口U.口II
기1口II
.-'.

a.

U.
기111

口＝11=
1= 1

U
U.

11
口＝

U...

..-口m口1
-口-

＝口＝1111111口- 口.口

'.

甘IRUl

--U.
I.
.--.

.

心트甘II
......I.

＝口口111m11口＝1
U-

.-...
....'＝
口1

毋哺芒

끄＝＝口브 끄m므I'口1

CONTENTS
LESS아1 01 확률 나타내71
LESS아寸 02 아날로그 변조 및 복조 설계하기
LESSON 03 디지털 변조 설계하기

1

LESSON

01

확률 나타내기

［예제 ]2-11과［예저12-2］의 시뮬링크 모델을 사용하여 확률 및 확률에 대한 평균과 분산을 히스토그램으로 나타내뵤匹I..
I Uni幻rm Random Number블록 1 日ounding Function 블록 I Random Number블록 1
1 卜川n卜相x블록 1

Keyword

Uniform Random Number 블록

I

Un표brm Random Number 블록을 이용하면 지정된 구간에서 균일 분포된 난수를 생성할수 있다．

I

Rounding Function 블록

Rounding Funct幻n 블록을 이용하면 입력 신호에 반올림 함수를 적용하여 출력 신호를 생성할수 있다．

［껜뗀型크J
육면처1 주사위를 100번 던졌을 때 주사위 눈의 빈도수를 보여주는 시뮬링크 모델을 설계하고 그 결과를 히
스토그램으로 나타내박．
；而
지식

=

百VI

획률은실험에의해여러가지결과가唯수있는표본공Z뇌써어떤사건이일어날것인지를실수로변
蜘陪방법을밀힌다주사위의획률은육면체주사위를한번던질때唵수있는l부터6까지의주사위
눈이 발생할수 있는 모든 가늣섯읔 지니 표보곳가희 수쿠 냐느이 구云1rl
00부터 1 사이의 실수를 무작위로 생성하는 Uniform Random I나umber 블록을 생성하고（[Sour此引
띠ni凡rm Ran面m Number]) 더블클릭하여 伍小nimun피을0으로 바꾼다．
Uniform Random Number
0U巾Ut a un札ro仰 d冶tributed random 引goal.
Ou巾Ut 冶 r日peata니e 伯ra 卵en s日ad.
Param미카S
Minimum:
U
卜.la川mum:
1
S日日d:
0
San四冶 血ne
at
區］ lot日r口ret vector paramet마5 a5卜D
（珉m

Canc이

H터p

그림 19너 Un的rm Rand아11 Number 블록의 최솟값 설정

522

PART 04. Sim베nk 설계하기

0 무작위로 생성된 0부터 l 사이의 실수에 6을 곱하는 G缸n 블록을 생성하고（[Commonly Used
미oc畑卜［Gain]) 더블클릭하여 四ab비에 6을 입력한다．
0 실숫값을 가까운 정숫값으로 반올림하는 Round由g Function 블록을 생성하고（
［卜4ath Operations][Rounding Function]) 더블클릭하여 [Funct油피올 ceil로 바꾼다．
F祐Un비ng
Roun비09 0pera如ns
Parameters

[

Function: cell

[

OK

Canc日1

H帥）

그림 19-2 Rounding Function 블록의 C에 함수 설정

0 시뮬레이션 결과를 명령 창에 나타내기 위해 To Workspace 블록을 생성한（[Sii血引-[To Workspace])
후 더블클릭하여 [Var坮ble name:］을x로 바꾸고 [Save fern毗：
］으로N丁ay를 선택한다．
To 叫or如pace
Write inp니Ito 印ecifued tim日ser厄已 array, 口r structure In 日 w口rks口an已 For men니bas日d
引m네ation. da伯 泊 니미tt日n In the MATLAB base workspac已 0日伯 Is n口I as켸冶비e Un出 tire
simulation 泊 St口口ped or 口aused
To 幻9 a bus 引gnal, use "Tim日sen日5" 55蛇 f口rrnat
Parameters
Variable name:

Umft data 口미015 切 Ia吼
ini
0日d1ma如n:
1
Sane化rmat: 肖tray

니

Save 2-0틔gna匕a뵤 Inherit tram in口ut (this ch이cc니세b日removed - S日日release not日S)

니

回 Log ftc日d口이01 data as a fi obi日Ct
Sample 出It日 (-I 佃r inher如d):

0K

O

Can口日I

H日巾

A口p竝

그림 19-3 而Workspace 블록의 변수명과 저장형식 변환

0 생성된 블록을 연결한다．
肛

出t

vi咐

固，目

f片甲啣

r汁呵却1 鈿在螂m

如畇引5

Code

1겨켜5

H帥1

새큼늬呻 咀岫 恥＞ 」《 匹，,, 臼 , 幽，

PROBA1

e

t月PIlOBAt

烈
口
4

回
口
口
i=

!

烈， '홑？ ‘릎 a.T。
W*s tp.

Re必r

100%

F以edSt바）Discrete

그림 19-4 완성된 시뮬링크 모델

CHAPTER 19. 통신

523

0 설계 창의 메뉴 표시줄에서 [Simulation] 메뉴를 클릭하여 伍4ode1 Configuration Parameters] 창을 열
고 [Start time:］에 0.0, 毆叩 time:］에 9.9를 입력한다. [Solver options］의 [Type:］을 Fi配d小就ep,
[S아ver:］를 discrete (no continuous states）로 설정하고 [F奴ed-step size:］에 0.1을 입력한 후 시뮬
레이션을 실행한다.
0 시뮬레이션을 실행한 후 MATLAB 명령 창에 생성된 확률을 히스토그램으로 나타내기 위한 명령어를
입력한다．

그림 19巧 히스토그램을 그리는 명령에 입력

nn

0 히스토그램은다음과같다．
In胡月t

日b

｛缸3 日 毖

T自5

'\ 物 自 堤 / 니口 ［그 目

Li

nIl.

겅）

1 口

미I 141W口-U

5
0
5
i
1
宣b= gtm弓乃史之

2

3
4
Sbc杉 이iaD冶

5

그림 19-6 그림 창 결과

주사위를 많이 던질수록주사위의 각눈이 唵사건의 획昏］吉批근할 것이다． 또한U耐brm
Random I如mber 블록을 더블클릭하여 [Seed:］를 1로 바꾼 후 시뮬레이션을 실행하면 다음과 같이 ［그
림 19-司과는 다른 결과가 나타난다. 즉 무작위로 생성된 실숫값은 Seed 값을 바꿀 때마다 다른 결과를
보여줄 것이다．
Ole

n끼
TOOlS

T0아1 어蜘却 mm片

｛그 (3 日 曲 Li '\ :'\ 的 自 咽 / , 目 目 덥 1 口
n口II.미.1卄m4m11

25

m

m
佑
＞욘m그g亡m甘石m스＜
5

0

2

3

4

5

匐ISIS 이oaD治

그림 19-7 다르게 나타나는 그림 창 결과

524

PART 04. Sim메nk설계하7I

6

I Random Number 블록
Random Number 블록을 이용하면 정규분포된 난수를 생성할수 있다．

I 세nMax 뷸록
入小小lax 블록을 이용하면 최소 또는 최때1 원소, 입력 원소를출력할수 있다．

1 예저119-2 I
평균이 ] 0, 분산이 9인 정규분포의 확률 2000개를 생성하는 시뮬링크 모델을 설계하고 그 결과를 히스토그
램으로 나타내라．

;

i巨VI

0 정규분포된 실수 2000개를 무작위로 생성하는 Random Number 블록을 생성하고（[Sources][Random Nun小er]) 더블클릭하여 小4ean:]에 10, [Var恤ce:］에 9, [Seed:］에 3. [San그pie tin妃：
］에
0.아을 입력한다．
Random Number
Out口ulan口rma加 (Gaus틔日n) d冶tribut日（Jrandom
引gnal. Ou최口나tie rep日stab伯 幻ra 미yen $日日d.
Paramet아S
Mean:
10
Varienc日：
9
Seed:
3
Samt）伯 tim日
0.01
團 nt日r口ret yes伯r 口ararneterS as ] 七

I

OK

]

Cans비 1 1

He巾

]

그림 19田 Random Number 블록의 평균．분산, 시드. 표본 시간 설정

0 무작위로 생성된 실수의 최솟값과 최댓값을 구하는 入tin入4ax 블록 2개匿 생성하고d入4ath
Operatioo刈e小小nMa피）블록의 이름을 각각 Mm油urn. Maximum으로 바꾼다．
0 블록 Maximum을 더블클릭하여 [Function:］을 m瞰로 바꾸고, 블록 M血imuon은 [Function:］의 기본
값mm을그대로 유지한다．
MinMax
Out口마 mm 口rm日X 口fin口ut Fora 引ng冶 input, 口口erators are 카가川日d
across the in口uteector. F口r mu川미e In口utS』0口日rat口rs are 키가눼日d
ocr口cc the inpu怡，

M비n t璽塑？而瓦白히
Funcdon: max
Numb日rot In口니tp口r15:
1
［끄 Ens비日 ocr口-cr05引ng d日t日口卄口n

9

Can口바

그림 19四 블록 Ma川mum의 최댓값 함수 설정

CHAPTER 19. 통신

525

［卜Lath O꺄ra如ns卜[Rounding Func如n]) 더블클릭하여
0 Rounding Func如n 블록 2개를 생성하고（
[Funct奴피올동일하게 round로 바꾼다．
0 시뮬레이션 결과를 명령 창어］ 나타내기 위해 To W幻rkspace 블록 3개를 생성한다（[Sink이-[To
Workspace]).
0 블록을 더블클릭하여 [Variable name:］을 각칵 x, ymin, ymax로 바꾸고 [Save format "］으로 모두
Array를 설정한다．
0 생성된 블록을 연결한다．
File

Edit ＼丹ew

D啣ly

e弓 , 딤

Olagoam

듸n｝미aloe

肉'a卜ysls

C어卞？

k）어S

H叫p

朴踞 ,, 呻 왜 @ 膀 多 E小，》 U) , 筐自 ,

P1905A2
寸

團P日0日A2

e

吼

風
亞크
mE

回
［回

m느

口口

M th1,,.

R口.,d, n
Furt口11

"m

UJ

汪
匪

nU

,mm.

'中
"

To 버o.t, .岬

分
Ready

1伏）%

日xed았ep［거screte

그림 19尸］0 완성된 시뮬링크모델1

0 설계 창의 메뉴 표시줄어써 團mu!毗on] 메뉴를 클릭하여 [Model Co曲guration Parameters] 창을 열
고 [St町tt油因에 0.0, [Stop time:］에 19.99를 입력한다. [S아ver options］의 [Type:］을 Fi配小就ep,
[Solver:］를 discrete (no continuous sta把5）로 설정하고 [F奴ed田tep size:］어1 0.01을 입력한후 시뮬
레이션을 실행한다．
0 시뮬레이션을 실행한 후 MATLAB 명령 창에 생성된 확률을 히스토그램으로 나타내기 위한 명령어를
입력한다．
Command Win寸二
>> 川st (x .O:20』ynin:y.ae) ;
>> 川abel (Paadum values ') ;
>> ylabel ( 'Absolute Frequency ) ;
>> title (Histogra,n ol Random Numbers ) ;
그림 ]9- 11 히스토그램을 그리는 명령에 입력

四 히스토그램은 다음과 긷다．

526

PART 04. Sim메nk 설계하71

Fife

刻仕

if恥虹 h陌ert

T0Os

Des岫口p

刊k岫片

H바1

｛뇨3 日 拿 i 臣 民 '\ 好 自咀 d 니 艮 1 [3 匡크 U 口
H的口gr出not R口蜘us Nun吐ier$
啣
抑
佃
m

寸듬그g止山弓즈8 <

m
0

5

10
15
Rarx幻m Vak用S

才｝

25

그림 19-12 그림 창 결과

Ei1} Random Number 블록의 Seed를 바꿀 때마다 그림 창에 실행 결과가 다르게 나타난다．

CHAPTE日 ]9. 통신

527

02

아날로그 변조 및 복조 설계하기

［예제 12忖히과 ［예제 ]2-7］의 시뮬링크 모델을 사용하여 양측파대 진폭 변狂r 주파수 영역의 진폭 변조를 알아보자. 또한
시간 영역에서의 주파수 변조 방식을 구현하는 시뮬링크 모델 2개를 설계하고 서로 비교해보자．
I Trigonometric Function블록 1 양측파대1 진폭 변조 1 주파수영역에서의 진폭 변조 1

Key1사ord

1 시간영역에서의 주파수 변조 I Zero-Order H이d 블록 1

I

Tr勾onometric Function 블록

Trig아珣metric I七nction 블륵 을 이용하면 일반적인 삼각함수를 실행할수 있다．

1 예Xii 19-3 I
양측파대 진폭 변조 방식을 이용하여 반송 신호 巾）로 메시지 신호 m(t）를 2초 동안 변조시킬 ［대1 메시지
신호，반송 신호，변조된 신호를 구현하는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．이때1
반송 주파수는 15[Hz］이다．
巾）= 3cos2兀／沚
m( t) = cos2irt

풀이

0 코사인 파형 반송 신호를 나타내는 Sine Wave 블록을 생성하고（[Source可4없ne Wave]) 블록의 이름
을c (t)로바꾼다．
0 블록c (t)를 더블클릭하여［加nplitude:］에 3, [Frequency (md/see) :］에 2串pi*15를 입력하고, 사인파
를 코사인파로 변환하기 위해 [Phase 佃d):］에 pi尼를 입력한다．

528

PART 04. Sim메nk 설계하71

S汭ehr늄Ye
Os如Ste 늬ne 낵aVe:
0 (t) = 帥p.Sin(Freq나＋Phas日）+ Bias
미se ty口e determines 出e CDm口Ste如sal technique used. The
parame也rs in the two types are related through:
Sam口1es 口日r 口mind = 2町H / (F누equenCy 1 Sam미e 亡me)
Nembe尸 at offset samp冶5 = Plies日 1 Sam히es 口er 口eriod / (2士口1)
山e thy samp伯based 引Se to口e 汗 numerical 口reb冶ms duet口
running for large limes (e.g. ovet如w in absolute rime) occur.
Param日也r5

니

미n日ty口e{ lint日has日d
Pm日 (t): 1D됴而而네a如slime
Nn口卄山d日：
3
日冶8.
n
다eq（始ocy (red/s日c):
츠Fl.陌
Phase (red):
pV2
Sam미e 甘me:
0
크 1st日rpret Ye比玎 口aram미町Sus I -D

OK

J Cancel ( Help 1

그림 19-13 블록 c(t）의 매깨변수지정

0 메시지 신호를 나타내는 Sine Wave 블록을 생성하고（[Sources卜囹me Wave]) 블록의 이름을 m (t）로
바꾼다．
0 블록 m(t）를 더블클릭하여 ［加mp1itude:］에 1, [Frequency (md/see) :］에 갸甘를 입력하고, 사인파를
코사인파로 변환하기 위해 [Phase (rad) :］에 pi尼를 입력한다．
0 메시지 신호와 반송 신호를 동시에 받기 위한 Mux 블록을 생성한다（[Commonly Used 미oc畑］
[Mux]).
0 메시지 신호와반송신호를곱하는Product 블록을생성한다（[Commonly Used 미ocks卜[Proc加Ct]).
O ＆叩e 블록 2개를 생성하고（[Sii水司-[跳叩e]) , 메시지 신호와반송 신호를보여줄 Scope 블록의 이름
은c (t)鈿s (t）로, 변조된신호를보여줄Sc야光 블록의 이름은m_DSB (t）로바꾼후생성된블록을차
례로 연결한다．
F개k므

p出t

v伯냅

r滋枓旴

舜' 冒

Di呵酊1

鮎m岫떼ten

riJ나戶15

CC巾

b必

卜相Ip

' 驕 ' 呻 好 臼 1P , 匹 ' 斗 @ ' 磁 ,

riNMOD口
e 回ANMOD1

風
11
느1

四
as

斗
回

團吼
［그

rL

!

I

口
cit月n甲）

!

니

m
出
力
Ras旬

1伐民

0（相45

그림 19-14 완성된 시뮬링크 모델1

CHAPTEF국 19; 통신

529

0 설계 창의 메뉴 표시줄어써 [S뇨rul毗On] 메뉴를클릭하여 ［卜'lodel Conflgur曲on Paran妃ters] 창을 열
고［Sta毗time:］에0, [Stop血ne:］에2, 小'tax step size:］어11/1000을입력한후시뮬레이션을실행한다．
0 블록 c (t)&m (t)를 더블클릭한 후 마우스 오른쪽 버튼을 누르고 [Configuration properties...]
를 클릭하여 창을 연다. 실행 결과를 최적화하기 위해 [Y-limits 小'lii如lum):］에 -4, 呼limits
小4aximum) :］에 4를 입력하고 [Title:］에 Message signal and carrier s唾ial을 입력한 후 回K] 버튼
을클릭한다．

加加ed沽play:

I

I升e:

1너日ssage 引gnal and carrier 引goal

［口 돠to叫eg日nd

團 Sho나grid

國 나O1 引gna怡 as magnitude and phase
V-limits (Minimum):

-4

V小m帖 (Maoimum): 4
V녀ab비：

그림 ]9-15 스코프 창의 최솟값, 최댓값 설정 및 자목 입력

m 다음 스코프 창은 메시지 신호와 반송 신호를 보여준다．
印e

Tools

\／沌w

돠mula甘on

;3, ,

回 , 啞 (9 i1> 0

汁lip

1

罕 回.

c* . ［二

.

1

4-

；斟排朴i
,

-

04

= :

므

1

'

Re由

=2（卜머口

그림 19-16 스코프 창 c(t)&m(t) 결과

q1 블록 mDSB (t）를 더블클릭한 후 마우스 오른쪽 버튼을 누르고 [Configuration properties...]
를 클릭하여 창을 연다. 실행 결과를 최적화하기 위해 [Y-limits (Minimum) :］어］ -4. [Y-limits
小'laximum) :］에 4를 입력하고 [Title:］에 Modulated signal을 입력한후 回K] 버튼을클릭한다．
m 다음 스코프 창은 양측파때1 아날로그 진폭 변조 방식을 이용하여 메시지 신호와 반송 신호어］의해1 변조된
신호를보여준다．

530

PART04. S寸nulink 설계하기

F艇

To이＄

\／陌w

鉀0너씨on

H斟p

@ , 兮 @ 中 e 믐亨 , q , ［끄 , f 汾 !

R叫y

그림 19-17 스코프 창에 나타난 변조 신호

I

Zero- 0rder H이d 블록

한 샘플 주기의 영차 홀드를 실현할 수 있다. 이 블록 은 하나의 입력을 받아서 하나의 출력을 생성한다．

1 예제 ]9- 4 I
1
［예제 19-3］과 동일한 메시지 신호와 반송 신호를 사용하여 주파수 영역의 진폭 변조를 그리는 시뮬링크 모
델을 설계하고 그 결과를 스펙트럼 분석기에 나타내라. 이때1 주710 드 i 드 4.5이다．

풀이

0 ［예제 19-引의 0N0를 반복한다．
0 Zero-Order Hold 블록 2개를 생성하고（[Discrete]-[Zero十Order I如id]) 더블클릭하여 [Sample
山ne］에 1/1000을 입력한다．
0 Product 블록을 생성한다（[Commo曲 Used Bloc畑卜[Product]).
0 Spectrum Scope 블록 2개를 생성하고（[DSP System Too小ox卜田inks卜田pectrum Analyzer]) 블
록의 이름을각각M(f), 入4DSB (f）로바꾼다．
0 블록 M(f）를 더블클릭하여 [Spec打urn Settings] 창을 열고 다음과 같은 환경을 설정한후 스코프 창을
닫는다．

CHAPTER 19. 통신

531

F簪目

To아5

W畔

Sk1lU1哺H며｝

H目p

긔

密L G) g> 馝 斗 , 익 , ［二 ，多 旺 旺 5d ［刃
: V SF乂寸ftofl= 才’나1
n

「 'm「
: 크n百片己 r吼亡

/ 乂

P。

wer

1H乙

,

n

.

n

:

!

口
F돠出t (H기

!

:U
凹

0.2

YY1，如닙Ho,的

!

m

2048

好

蛋

三r

느二＝ 1;

m．《．

刀

Run simulation

g
口

see

8

릎
믈

, ：나느느

h

HH1

'1

0

results.

Redan며1br

그1

005

n

n
日
m 크工1n口Ctrazz
口 」0小.dt「毗

田 d，먀돠1o,d 520（뵤re,

七뇨

ii

卜
H

曲旴＝Hz 由m巾Re뇨10 目｛z

그림 19- 侶 블록 M(f）의 Spectrum Settings 매개변수 지정
il l}

입력한 값은 시뮬레이션 실행 후 생성된 파형을 보기 좋게 하기 위해 다시 조정했다．

0 [Configuration Pr아光rties...] 버튼을클릭하고다음과긷미 Y축 이름을 입력한다．
미splay
1개a:
巴 Show le므end

團 닯10나 grid

V네It朮＄（卜녜nimum):

-alT引四i翩17S98496

V-limits (Maximum): a28439169143344423
V-a川s lab이：

Magnitude-sq니ared
OK

Cancel

그림 ]9-19 블록 M(f)의 Y축 이름 입력
0 블록 M_DSB (f）를 더블클릭하여 0N0을 반복한다．
0 블록을 연결하여 모델을 완성한다．

532

PART 04. Simulink설계하기

Ale

Ed竹

\/ie나

區i！目

Display

Dia91otT}

닯molatlon

Analys匕

Code

" 鸚 " 呻 4뇨 由 吼＞

下j아S

He巾

난3! ,, 臼 ! 幽 !

帥小내0D2

:二

t코ANM002

!

卄뇨卜나J\ m1

브

H

1

11

z可04>d目

dI

HD녑

나

Ltf)

녑

m

1노

回
［그

'00

i

"

之各口

吐0$태I)

E므

自
力
100%

000旬

＼加幽小0epD匕Crete

그림 ]9-20 완성된 시뮬링크모델

0 설계 창의 메뉴 표시줄에서 圄mulation] 메뉴를클릭하여 [Mod이 Config呻tion Parameters] 창을 연
다. [Start time:］에0, [Stop time:]어］4.5' ［卜1ax step size:］에 1/1000을입력하고［S아ver optiot瑚의
[S이ye川를discrete (no continuous sta妃S）로 바꾼 후 시뮬레이션을 실행한다．
@ 시뮬레이션을 실행한 후 M(f) 창과入4 DSB (f) 창이 열리면 다음과 같은 결과가 나타난다．
F七

Tools

Vtl汁

S融쩍J七刈iecs

H幽于

琶出

昴 , G) 帑 羽 1 各 나 風 n［꾀 囹 匹 咽 團［刃
亘0

2$

多
百 52
프1
貫015

8
a
;

-40

.가｝

1
0

251

d.

油S町＝488쏘 "a枉 蜘 '0巾0.蜘1 났枉 1T=4聊

"

그림 19-21 스펙트럼 M(f）의 결과

F켜b

似片5

나咐

SI,'겨거aticr

He巾

1

昱4
Re40y

11

貫03

訃4

始 , 回 甘＞ 豫 帑 , e乞 , ［二 囹 國 圈 團［刃

「

的W-480그8,,8仁 冷-

1
!bb=I甘40 11.4．的0

그림 19-22 스펙트럼 屹DSB(f)의 결과

CHAPTER 19. 통신

533

1 예저119-5 I
0 드 t 드 0.2 [se이 동안 주파수 감도 幻 = 80兀이고 반송 주파수／느 150[Hz], 반송 진폭 A戶 1, 샘플링 주
파수 /;= i0000[H기인 메시지 신호 m(t) = cos(2刃t)에 주파수 변조 방식을 구현하는 시뮬링크 모델을 설
계하고 그 결과를 스코프 창에 나타내라．이때 메시지 신호의 주파수 /= io[H기이다．

풀이

(a）주파수변조신호는s(t) =Accosf2兀［五t+kjj; m(r)dv]｝로나타낼수 있다·
0 메시지 신호를 나타내는 Sine Wave 블록을 생성하고（[Source引4엷ne Wave]) 블록의 이름을
可t)로바꾼다．
0 블록m(t）를 더블클릭하여 [Frequency (rad/sec) :］에 가pi*10을 입력하고, 사인파를 코사인파로
변환하기 위해 田hase (rad) :］에 pi尼를 입력한다．
OG曲l 블록 3개를 생성하고（[Commonly Used Bloc뇨卜四曲I]) 블록의 이름을 각각 k_f, 2pi,
Ac로 바꾼다.
0 주파수감도를 나타내는블록kf를 더블클릭하여 [Gain:］에 札半pi를 입력한다．
Gain
티日ment小너se ga汭 (y = 1乙1U) 口rmatrix gain (y = K.u or y = U나0.
Main 1 돠goal川ibutes

Paramet日r 胤ribut日S

Gain:
a뇨口i
MuWp比a如n: 터Sri冶nt-叫se(K..u)
d

1

1
그림 19-23 뷸록 kf에 주파수 감도 설정

0 블록2pi를 더블클릭하여 [G如n에 2如i를 입력하고, 반송 진폭을나타내는블록A下의 [Gain:］은
기본값 l을 그대로 유지한다．
0 Integrator 블록을생성한다（[Commonly Used B뇨：ks］丑ntegra的r]).
0 기울기 兀인 입력변수 t어］ 대한 l차 함수를 나타내는 R；知叩 블록을 생성하고（[Source可-[Ramp])
블록의 이름을 (fc汁로 바꾼후 더블클릭하여 團ope］에 반송주파수로 지정된 150을 입력한다．
Ramp (mask) (link)
Out口Ut a ram口 늬go히 startng atthe x口ec而ed 打me.
Paramet마S
S幻口e:
13
Start ttme:
a
Initial ou的ut
0
凹 In他rpret vector 口arameters as卜 ［)

1

OK

1

Cance니

그림 19- 24 블록 吃아t에 반송 주파수 설정

534

PART 04. Sim메nk설계하기

0
0

Add 블록을 생성한다（
［卜fath Opera如ns卜[Add]).
Trigonon娥如 Function 블록을 생성하고（
［卜4a血 Operat油司-[Trigonom毗如 Function]) 블록
의 이름을 cos[］로 바꾼 후 더블클릭하여 [Fm毗jo瓦띠1 cos를 설정한다．
1卞每二3? J뷰i中｝ 尸 J

Trigon口metric Functi口n
Trigonometric and htperboIic functions. Wlien the function has more
than one arg니m日nt, the 伽at argumen比on.日sponds 幻 the to口 佃기eft)
in口Ut p口比 F口r 引n, coo, 引ncos, c口5,' 引n. atan2 functions, CUR미C
a口prosimation can a놈口 be 니5日d 幻 c口m口ute the ou如Ut.
Paramet酊S
日.jncti口n: C口5

OL!巾Ut sign히 ty口e

J

!]

却口ro川m訓口n method: None
auth

9

OK

C日nC이 ]

H日巾

그림 19- 25 블록 cos[］에 코사인 함수 설정

mScope 블록을 생성하고（[Sink司-[鈿唯］) 블록의 이름을s (0로바꾼후 생성된 블록을 연결한다．
A뇨

Etht

VSew

DlsH自y

蚌！目

Dt呵ant

Simulation

鸚

A.naiy引S

C亡4把

b머$

t妃4p

" 曦努 唾 (8 雅 器 匹，》》e) ! 邕，

사1DEM3
!

團ANDEM3

e

烈
長｝

爭 '牙 甘뇨I ，牙 ，랖나＞耳
回
갑
圄
4

［그
E文
齒
力
R叫自／

10叱

그림 19- 而

ade45

완성된 시뮬링크 모델 j

Q 블록 s (t)를 더블클릭하고 B크 [Layout] 버튼을 클릭하여 다음과 같이 2개의 스코프 창을 상하로
설정한다．
F旽

1以虧

View

Simulate짜｝ H帥）

!

@ ! 蜀 8 吟 S 峯 r （曳 , ［끄 . f 冶 ,
트王니．

I. .口

i 1u.

甘111
I. .
C거姻

그림 19- 27 상하 2개 스코프 창 설정

CHAPTER 19. 통신

535

m 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 [r'如del Coi血guration Paran妃ter可 창
을 연다. [Start time:］에 0, [S的p time:]에 0.2, [Max step s切e］에 1/10000을 입력하고 [S이ver
options］의 [S아ver:］를ode45 (Dormand尸Prince）로바꾼후시뮬레이션을실행한다．
四 블록 s (t)를 더블클릭한 후 위쪽 스코프 창어써 마우스 오른쪽 버튼을 누르고 [Configuration
properties...］를 클릭하여 창을 연다. [Title:］에 Message signal을 입력하고, 실행 결과를 최적화
하기 위해 [Y-limits (Minimum):]에 -1.2, [Y-limits (Max血llllm :］에 1.2를 입력한 후［아(1
버튼을클릭한다．

Aches 비S이ay:

I

Title:

Message signal

巴 Sho나legend

Y Sho낵 grid

巴 F기口t 引gna놈 as magn仙de and phase
V내m的 (Minimi꾜11):

-1.2

V네m心 (Ma뇌mum): 1.2
V-lab미：

그림 四U羽 위쪽 스코프 창의 최솟값. 최댓값 설정 및 제목 입력

C) 마찬가지로 아래쪽 스코프 창어써 마우스 오른쪽 버튼을 누르고 [Cot血guration properties...］를
클릭하여 창을 연다. [Title:］에 FM signal을 입력하고, 실행 결과를 최적화하기 위해 [Y-limits
小什umum) :］어］-1.2, [Y-limits 佰flax뇨lU1m:］에 1.2를 입력한후 回K] 버튼을클릭한다．
四 다음스코프창은메시지 신호와주파수 변조 신호를보여준다．
File

Tools

View

自mit川h마1

He乍

1

@ 1 心 (8 b 小 g亨 , 억 , ［끄 ,

f

i2 ,

n노 工m,

十

「＼
,.,,

"

,,/,,'

,/／小

'

"
:,,,

1!

j!

FM白沙刻

1附小M料牡\I/ 1
/\.!斗i1!

Re.出rT4枷

그림 19-四 스코프 창 결과

시간에 따른 메시지 신호를 스코프 창 위쪽어］ 그래프로 나타내고 시간어］ 따른 주파수 변조 신호를
스코프 창 아래쪽에 그래프로 나타낸다．
(b) 주파수 변조 신호는 다음과 같이 다시 쓸수 있다．

s( t) =A.COS[ 2兀（上［k／加（「）＋五］dr) ]
O (a）의O을제외하고O '- -由을실행한다．

536

PART 04. Simulink설7IaF7I

0 반송주파수兀를 나타내는Cons伽吐블록을생성하고（[Commonly Used Blocks卜[C毗t耐］)
블록의 이름을 fc로 바꾼 후 더블클릭하여 [Coi喊ant v키ue:］에 150을 입력한다．
0 생성된블록을새롭게 연결한다．
F켜b

曲1 Vi曲

0婢恂

回! r

먀好am

듸mulatton

肉l키y引＄

Ca.土e

叱이s

He巾

旨욤 每 中 " 呻 心 ＼上夕 昑 『＼ E3 ! ,, (3 ! 蟲 !

可叩타.14
回mDEM4

;

!

툐l

因
回
［그

> ，三나二，戶口
y '牙 : .,, -.,: 尸＋三，
卜아

曲
毖
R的dy

lco%

며te45

그림 19-羽 완성된 시뮬링크 모델 2

O (a）의 0N四를 반복한후 모델 2를 실행하면［그림 19-29］와동일한 결과를 얻는다．

CHAPTER 19. 통신

537

디지털 변조 설계하기
［예제 ]2-12], ［예저1 12-］引의 시뮬링크 모델을 사용하여 기저대역 신호 진폭 천이 변조, 주파수 천이 변조 및 기저대역의 디
지털 신호를 나타내보자．
I 진폭 천이 변조

Keyi사ord

I

1 주파수 천이 변조

1

진폭 천이 변조

진폭 천이 변조（ASK: Amplitude Shift Keying）는 반송파 진폭의 변동 형태로 디지털 2진 데이터를 나
타내는 진폭 변조 방식이다．

I

주파수 천이 변조

주파수 천이 변조（FSK: Freqt比ncy Sh次 Keying）는 디지털 신호의 변경어］따라 반송파 신호의 주파수
가 변하는 주파수 변조 방식이다．

1 예저II＋이
진폭 천이 변조의 통신 시스템을 이용하여 무작위로 생성되는 21개의 심벌（0 또는 1）을 연속으로
0 드 r 드 10초 동안 전송한다. 이때1 반송파 c(t) = sin(2,rt）를 사용하여 기저대역 신호와 진폭 천이 변조된
신호를 나타내는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라．

풀

00부터 1 사이의 실수를 무작위로 생성하는 Ui出bnn Random Nu岫er 블록을 생성하고（[Sou丁Ce引
[Un派）rm Random Number]) 블록의 이름을 b (t)로 바꾼다．
0 블록b (t）를 더블클릭하여 小4inimum:］어］ 0. [Seed:］에 5, [San町)le 血ne:］에 0.5를 입력한다．
Uniform Random Nomber
0山口Ut a un加rmli, 비sbib山目drandom 引an毗
0내巾Ut is re口eatabi日 幻r a gi四n 8日ed.
Param日t바S
Minim내n:
0
Ma川mUm:
]
S日ed:
5
Sample dma
as
凹 Interpret Uect口r 口arame旭r5 a5 卜 ［)

QK

1 1 드aricnl 1 1

姓a如

그림 19-31 Uni幻rm Random Number 블록의 최솟값, 표본 시간 설정

538

PART 04. Sim메nk 설계하기

0 실숫값을 가까운 정숫값으로 반올림하는 Rounding Fw姓幻n 블록을 생성하고(1入4ath Operations][Rounding Function]) 더블클릭하여 [Fun曲이피을round로 바꾼다．
Roun비ng
R口unding a口era亡one.
Param日t마S
Func如n: round

Canc日1

He巾

口

그림 ]9-32 Rounding Function 블록의 round 함수 설정

0 반송 신호를 나타내는 跏ie Wave 블록을 생성하고（[Sources] -[Sine Wave]) 블록의 이름을 c (t)로
바꾼후 더블클릭하여 [Frequency (rad/sec) :］에 2永pi를 입력한다．
태I,日 叫a晦
Ou如uta 비ne 叩aye:
O(t) = mp*Sin(Freq口t.Phase) + 日ias
Sine type determines the computational technique used. The
parameters in the two types are related through:
Samples 口yr 口eriod = 乃pi / (Fr日quency * Sample 卄me)
Number o比加日tsamples = Phase t San）이es p日r 口eriod / (2.pl)
use the sam口1日-based 이n日 typ日 作 numerical pr아기ems due 幻
running 幻rlarge tim日s (e.g. overlo나 in abs미U也 甘m日） occur.
Param甘하＄
텨n日 ty口甘 기me based

!

기m日（出 Us日 曲S너帥on tim日

r

A까出山de
1
Bias:
U
Frequency (rad/sec):
2.口1
Phase (rad):
0
Sample time
U
團 Inter口ret vect口r paramet마s as卜0

1

OK

} i Canc日1 j 1 H톄p

그림 19-33 볼록 c(t）의 각주파수 설정

0 Product 블록을생성한다侮4ath 0꺄rations卜區oduct]).
0 Scope 블록을 생성하고（[Sii血司m田cope]) 블록의 이름을 s (t）로 바꾼다．
0 생성된 블록을 연결한다．

CHAPTEF국 ]9. 통신

539

F舵

Edit

Vit므w

Display

舜! 目

듸nmbt11며｝ Anai戶is

Diagran}

力 日日 )>
됴磅 聲 (9
U［크

11> ,

Co巾 i）
曲； He巾

全 ，力 (9

!

占主言 !

DGMODI
!

團DGMOD1

e

5'

:

封1三三 T
혀I,

,．口
卜 X

r入그

'

引q

，

닉lJ

團
必
口

胃g：므 !

=,m』

黛

m
由
力
0d甘45 .

I（刃％

Rea旬
그림 19-34 완성된 시뮬링크 모델

0 블록 s (t)를 더블클릭하고 [Layou日 버튼을클릭하여 두 스코프 창을상하로 설정한다．
0 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 ［卜4ode1 Configuration Parameters] 창을
연다. [Start time:］에 0, [Stop time:］에 10, ［卜4ax step size:］에 0.01을 입력하고 [Solver options］의
[S아ye川를ode45 (Donnand-Prince）로바꾼후시뮬레이션을실행한다．
q) 블록 s (t)를 더블클릭한 후 위쪽 스코프 창에서 마우스 오른쪽 버튼을 누르고 [Configuration
properties...］롤클릭하여 창을연다. [Title:］에 Baseband digital s培nal을 입력하고, 실행 결과를최적
］에 1.5를 입력한 후 [OK] 버
화하기 위해 [Y-limits 伍4加imum) :］에 -1.5, [Y-limits (Maximui미：
튼을클릭한다．
a) 마찬가지로아래쪽스코프창어伊如｝우스오른쪽버튼을누르고［Configuration pr叩帥es...］를클릭하
］에小如삐ated ASK signal을 입력하고, 실행 결과를 최적화하기 위해 [Y-limits
여 창을 연다. [Ti如：
小恤如玭ll) :］에 -1.5, [Y-limits 伍4aximw미 :］에 1.5를 입력한후［아(1 버튼을클릭한다．
l 卜dam

I Tim이 D治1川ap

Active display

2

Tide:

化d내ated ASK 引gnal

回 Shon기egend

1 Sh口뛰 grid

巴 믹마 引gnats as magn什ude and 口hase
V-lim心 (Minimum):

-1.5

V-limits (Maximum):

.5

V니ab미：

U

OK

H Canc이 1

1"4그口In

그림 ]9- 35 스코프 아래쪽 창의 최솟값, 최댓값 설정 및 제목 입력

a) 다음 스코프 창은 기저대역 신호와 진폭 천이 변조의 실행 결과를 보여준다．

540

PART 04. Simuhnk 설7 I5l7I

Fl相

了0015

View

Slmt甘m1D11 卜i텍P

거

@ ' 也（9 1口 難 믐亨 ' q -I꾜니 f 國，
ij1

r

小

'1

[:

1

lr
卜兆dUm1川 슥OKS.字目

J＼그八m\J\/=/\
'”「，
1
'

t

d

Re.旬

드

r:

?

a

L
T=1且啣

그림 19-36 스코프 장 결과

무작위 심벌을 이용한 기존 신호의 그래표를 스코프 창 위쪽에 나타내고 ，진폭 천이 변조 신호의 그
래프를 스코프 창 아래쪽에 나타낸다 ．전송되는 심벌이 0인 파형은 0을 사용하고 ，심벌이 l인 파형은
sin(2兀t)를 사용한다．

1 예제 19- 7 I
주파수 천이 변조의 통신 시스템을 이용하여 심벌 수가 21개인 디지털 데이터를 연속으로 전송하려고 한
다. 디지털 데이터는 무작위로 동일한 확률을 가진 0과 l을 생성한다. 전송되는 데이터의 심벌 기간은 Tb = l
[se이이고, 비트당 전송된 신호 에너지 月b = I [W/bit］라고 가정한다. 그리고 데이터를 변조하는 데 사용하는
27卄의 반송파중부호 l을 전송弓陪주파수는 玉＝읖이고，부호0을 전송弓는주파수는五＝去이다．이때
기저대역 신호와 주파수 천이 변조된 디지털 신호를 나타내는 시뮬링크 모델을 설계하고 그 결과를 스코프
창에 나타내라．

푿이

00-부터 1 사이의 실수를 무작위로 생성하는 Uni的rm Random Number 블록을 생성하고（[Sour此司e
띠ni白rm Random Number]) 블록의 이름을b (t）로 바꾼다．
0 블록b (t)를 더블클릭하여 小Ii川mun피에 0, [San叩le time:］에 0.5를 입력한다．
0 실숫값을 가까운 정숫값으로 반올림하는 Rounding Function 블록을 생성하고（
［卜lath Operation引寸
[Rounding Function]) 더블클릭하여 [Functi아비을round로 바꾼다．
0 반송 신호를 나타내는 Sine Wave 블록을 2개 생성하고（[Sot丁ces卜囹恤e 꿔aye]) 블록의 이름을 각각
s0(t), si (t）로바꾼다．
0 블록 s0（比 sl (t)를 더블클릭하여 [｝그requency (rad/sec) :］에 각칵 2串pi*4, 2水pi水2를 입력하고, 코
사인 파형으로 변환하기 위헤Phase (rad) :］에 모두pi尼를 입력한다．
0 Constant 블록을 생성하고（[Commonly Used 미oc뇨卜[C毗ta蝴） [Cons杻nt value:］어］ sqrt (2）를
입력한다．

CHAPTER 19. 통신

541

Constant
Output the constant specified by the 'Constant value' parameter.
'C口0引ant valu日 is a sector and 'In伯ryret sec幻r 口arameters as卜0' 冶
on, treat the constant value as a 1-D array. 마herwise, output a matris
叫fit, the sam日 비men引ons as the constant ye山e
卜,lain

Si '函 m，뵤b L冷

Con澍ant yalu日：
sqrt(2)
團 lnterpr日t sect口r 口arame也rs as卜 ［)
Sets口le time:
in)

OK

沙

]

Canc日I

H帥）

A口口11/

그림 }9-37 （丸ns佃nt 블록의 상숫값 설정

0 Product 블록2개를 생성한다（
［卜4ath Opera如ns卜[Product]).
0 기저 입력 신호를 기준으로 두 뱐송파 사이의 출력을 전환하는 데 사용하는 小vitch 블록을 생성하고
([Commonly Used 미ocks卜田w如h]) 더블클릭하여 [Threshold:］에 0.5를 입력한다．
S내妃h
Pass thr口U마t 1nt爻it 1 wIt日n input 2 sati酊泊nth日 5日1日cted cr11edar;
oth日0너5日，pass through in口ut a The in口니Is are numbered top 也 bofi口m
(or left to right). The first and third Input ports are data ports, and the
5日C口nd In口Ut port 冶 th日 cOntr이 port. The cr11日nat口r con打이 port 2 are u2
>= Thr日sh이d, u2> Thr日sh이d or u2 尸＝ a
Main그 ＄坦n敏枷thu伯a
Cr11日na It玎 口as引ng first in口Ur u2>= Thr日하l이d
Thr日Sb口Id:
15
團 Enab佃 2日rn-cry＄引ng d日也ction

I

Canc이

OK

He巾

A口口匈

1

그림 19-38 Sv바tCh 볼록의 한계치 설정

0 Scope 블록읕 생성하고（[Sir血司- [Scope]) 블록의 이름을s(t)로 바꾼다．
四 생성된 블록을 연결한다．
F爬

Ed往

너C텍

Dlsp士ny

d4 , 圄

Di하｝tam

Simulation

Aye卜吟15

" 鸚 力 呻 와 叫 恥＞ ,

CC巾 bols

He如

므3，片 回 ! 蟲 ,

DG卜伺O2

e 團呻呵）2

團
［그

,

'itt)

다m町

m11

甲t［力

區

1
1

,

Rot.닙1(

r\

+11

＝寸

느

小

LJ
'

乂 1

Ready

PART 04. Simulink설계하71

Sotth

1

니닒

그립 19-39 완성된 시뮬링크 모델

542

: 入

;
FJ1dbn

Em
峀，

CO1＝山1

卜；

므

［쿄

口m

1+

烈

!

l以夙

ode45

q1 블록 s (t)를 더블클릭하고 [Layout] 버튼을클릭하여 두 스코프창을상하로 설정한다．
0 설계 창의 메뉴 표시줄어써 [Simulation] 메뉴를 클릭하여 ［卜4odel Configuration Parameters] 창을
연다. [St町ttime:］에 0, 囹的p time:］에 10, [Max step size:］에 0.01을 입력하고 [S이ver options］의
[S이ver:］를ode45 (Dormand-P如Ce）로바꾼후시뮬레이션을실행한다．
侄） 블록 s (t)를 더블클릭한 후 위쪽 스코프 창어써 마우스 오른쪽 버튼을 누르고 [Configuration
properties...］를클릭하여 창을 연다. [Title:]에 Baseband digital signal을 입력하고, 실행 결과를 최적
화하기 위해1 [Y-limits 小4ii血aim) :］어｝ -0.2, [Y-limits (Max血ium) :]에 1.2를 입력한 후 回K] 버
튼을클릭한다．

I개e:

日aseband 뎨gital 引gnal

口 Show legend

團 Sho낚grid

口 F기口t 引gna눔 as m日gn加de and phase
v-I伽怡 (M씨mum): -a2
f師始 (Ma川mum): 1.2
V니ab日r

그림 19-40 위쪽 스코프 창의 최솟값, 최댓값 설정 및 제목 입력

C) 마찬가지로아래쪽스코프창에서 마우스오른쪽버튼을누르고［Conflgura如n prop毗妃S...］를클릭하
여 창을 연다. ［好如：
］에 入如dulated ASK signal을 입력하고, 실행 결과를 최적화하기 위해 [Y小mits
伍恤如mm) :］어］ -2. [Y-lii小ts 小4aximum) ］에 2를 입력한후 回K] 버튼을클릭한다．
四 다음 스코프 창은 기저대역 신호와주파수 천이 변조의 실행 결과를 보여준다．
出口

@ , 4各 (9 甘；
>

Hp

m

m

率 기 따 , ［꾜 니 + 國 ,

T-Is.000
그림 19-4]

스코프 창 결과

심벌 0에 대한 부분은 반송 주파수가 五인 정현파 형태로 변조되고 ，심벌 1에 대한 부분은 반송 주파수가
五인 정현파 형태로 변조된다．

CHAPTER 19. 통신

543

20

CONTENTS
LESSON 01 회로의 기초 도입하기
LESS아寸 02 저항, 인덕터, 커패시터 조합하기
LESSON 03 연산 증폭기 이해하기
LESS아'1 04 전력 사용하기

n
t
k
m

CHAPTER

LESSON

01

회로의 기초 도입하기

간단한 시뮬링크 모델을 설겨后뼈 회로의 저항에 걸리는 전압과 전류를 저항의 H율을 0용하여 구하는 전압 분할 방법과 전류
분할 방법을 알아보자．

Keys사ord

I 그래픽 사용자 인터페이스 1 power列1 블록

DC V이tage Source 블록 1

i Series AL（二 Branch 블록 1 \／이怡ge Measurement 블록 1 전압분할 법칙 1
I Current Measurement블록

I

전류분할 법칙 1

그래픽 사용자 인터페이스

MATLAB의 시뮬링크를 이용하는 회로 설계에서는 모든 상태변수（인덕터 전류와 커패시터 전압）뿐
만 아니라 전류와 전압의 정상값을 측정하여 그 결과를 나타내기 위해 그래픽 사용자 인터페이스（GUI:
Graphical U記r Interface）를사용한다．

I

powergui 블록

powergui 블록을 이용하면 그래픽 사용자 인터페이스를사용할수 있다．

I

DC \／이怡ge Source 블록

DC Voltage Source 블록을 이용하면 이상적인 직류（DC) 전압원(voltage source）을생성할수 있다．

I Series RLC Branch 블록
Series RI兀 Branch 블록을 이용하면 저항, 인덕터 및 커패시터의 서1 가지 소자 중 하나 또는 모두를 직
렬 조합으로 연결하여 선형 부하를 구현할수 있다．

I

\／이怡ge Measurement 블록

＼幻Itage Measuremei止 블록을 이용하면 두 전기적 접점 사히에 있는 저항어］걸리는순간 전압을측정할
수 있다．

546

PA日T04. Sim베nk설계하71

I

전압 분할 법칙

전압분할 법칙臼oltage divider rule）은옴의 법칙과 키르히호프의 법칙을 기반으로 하는 회로 해석 방
법 중 하나이다. 전압 분할 법칙은 주어진 입력 전압을 이용하여 회로의 저항어］ 걸리는 전압을 계산하는
방법으로, 회로의 저항 비율을 고려한다．

1 예저120- i

i

다음 회로의 전압 끼과 巧를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라. 여기서 ／乙 =

R2 = 2[ )], I승 = 5{V］이다．

3［列，

그림 20너 전압분할 법칙의 적용

풀이

0 powergui 블록을 생성한다（[Simscape卜［SimPowerSystem引냐Specialized Technology]
[Fui닢amen姐l 미ocks］士螂比rgui]).
0 DC Voltage Source 블록을 생성하고（[Simscape卜田加甲이妃rSystems卜囚恥ci曲zed I比hnology]
[Fundamental Blocks卜田lec打ical Source引-[DC Voltage Source]) 블록의 이름을Vs로 바꾼 후 더
블클릭하여［知mplitude (V) :］에 5를 입력한다．
DC Voltage Source (mask) (link)
Ideal DC V口Itage S口urce
Parameters
向까小山de (V):

S
Mea日uremen怡

OK

掘如U

H쉬p

그림 20쿄 블록 Vs의 전압 설정

0 Series RLC Branch 블록을 생성하고（[S油scape卜囹油P이作rSystems卜田꺄cialized Technology]
1在？undamen扼I Blocks]-田lemen制 田eries RLC Branch]) 블록의 이롬을Ri, R2로 바꾼다．
0 블록 R2를 클릭한 후 마우스 오른쪽 버튼을 누르고 [Rotate & F匈小［Counterclo比wise］를 실행하여
회전시킨다．
0 블록 Rl을 더블클릭하여 [Branch type:］은 저항을 나타내는 R로 바꾸고, [Resistance ((：血nS上] ]13
을 입력하며，[Measurements］는 Bran曲 voltage로 설정한다．

CHAPTER 20. 회로

547

Series PLC Branch (mask) (link)
Im비emen怡 as日rl日a branch 口I PLC 미ements
Use th日 ‘日ranch ty口日‘ parameter t口 add or rem口ye 이emen四
fr口md日 branch
Parameters
日ranch ty口日： P
Res冶tanc日 (Ohms):
3
M日asur日menlo Branch 너가taBs

mm

Cancel

[ Help

그림 20心 블록 대의 소자 변경과 저항값 설정

0 마찬가지로 블록R2를 더블클릭하여 [Branch type:｝을 R로 바꾸고 [Resis切nce (Ohms) :］에 2를 입력
한다．
0 Voltage Measurement 블록 2개를 생성하고（[Simscape］小［SimPowerSyste螂卜田pecialized
Techn이ogy]-[Fw녑amental Blo比司-[Measuren妃nt司-[Voltage Measuremen日） 블록의 이름을 각
각Measure1, Measure2로바꾼다.
0 블록 Measure1을 클릭한 후 마우스 오른쪽 버튼을 누르고 [Rotate & Flip]-[Counterclockwise］를 실
행하여 회전시킨다．
OI거splay 블록2개를생성하고（[Sit血司dm叩lay]) 블록의 이름을 각칵vi, v2로 바꾼다．
四 블록을 모두 연결하고 시뮬레이션을 실행하면 다음과같은 결과를 얻는다．
＝舟b

View ［肛的y

Edit

E片a9mm

듸mu以Ion

dutaiys住

Code

bolt

F＋베口

鸚 好 , 圄 , 呻 也 出） 陟 > E쯔 , ,, 回 , 芯自 ,

囹, 圄
m）日1

臂
cm

恥m月＝

e 回VDPI

p口n=qdi

甲

1

目 臼mImi

긔

1==

八 八 八
= V V V

匹1

1

［그

1斗

Meeaare2

也
力
Rae啣

l的％

l
][

卜

1뇨

"

tariebiestept기SC fete

그림 m닉 완성된 시뮬링크 모델

전압 분할을 이용하여 주어진 입력 전압 1승 = 5 [V］어］ 대한 출력 전압 끼과 V2를 구하려면 다음과 같
이 분모에는 회로어］ 존재하는 저항 凡 = 3[ 기, R2 = 2[ 기의 직렬로 연결된 2개 저항의 등가 저항
凡q= Rl + 凡 = 5[ )] 값을 대입하고，분자에는 찾으려는 출력 전압에 놓여 있는 저항을 대입한후 주
어진 입력 전압을 곱한다．

?;= R，즈‘R2 兀乙들 \ 5= 3[V]
V2= R，三’R,V
2，乙슬 / 5= 2[V]

548

PART 04. Simulink설계하기

I Current Measurement I록
Current Measurem이11 블록을 이용하면 임의의 전기척 블록 또는 연결선에 흐르는 순간 전류를 측정할
수 있다．

I

전류 분할 법칙

2개의 저항이 병렬로 연결된 접점어］ 전류가 도달하면 두 저항의 비율어］따라 전류가 분할되어 흐르는데，
이 부분 전류의 값을 결정하는 회로 해석 방법을 전류 분할 법칙 (current divider rule)이라고 한다．

1 예제 20- 2
다음 회로의 전압 /S. il, 2를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라. 여기서 /?1= 3［회，
凡 = 2［列, 乙 = 6[V］이다．

그림 20小 전류분할법칙의 적용

풀이

0 powergui 블록을 생성한다（[Simscape卜［SimPowerSystem町-[Specialized Techn아ogy][Fund帥ental 미ock引七兀＼vergui]).
O Voltage Source 블록을 생성하고（[Simscape卜田油P이化rSystem하小［Specialized Technology][Fundamental 미ocks卜田lee打ical Sour此引-[DC Voltage Source]) 블록의 이름을Vs로 바꾼후 더
블클릭하여 [Amplitude:］에 6을 입력한다．
0 Series RI兀 Branch 블록을 생성하고（[S油scap이-[SimPowerSyste跏］4跏印ialized Technology]
-[Fundamental Blocks卜田lements]-[Series RI兀 Branch]) 블록의 이름을 RI. R2로 바꾼다. 블록
R2를 클릭한 후 마우스 오른쪽 버튼을 누르고 [Rot毗e& F自小［Counterclockwise｝를 실행하여 회전
시킨다．
0 블록 Ri. R2를 더블클릭하여 [Branch type:］을 모두 R로 바꾸고 [Resistance 幻노ns) :］에 각각 3. 2
를 입력한다．
0 Current Measurement 블록 3개를 생성하고（[Simscape］小［SimPowerSyste邱］-[Specialized
Technology]-[Fundamental Blocks]-［入4easurements]-[Current 入4easurement] ) 블록의 이름을 각
각Measurel. Measure2, 入4easure3으로바꾼다.
0 Display 블록3개를생성하고（[Sink司 ［Di叩lay]) 블록의 이름을각각Is, ii. i2로바꾼다．
0 블록을 모두 연결하고 시뮬러］이션을 실행하면 다음과 같은 결과를 얻는다．

CHAPTER 20』회로

549

[ F沁

Ed作

\[,ew

Dis川ay

0的ran,

亡已 ' 冒

Analys好

(:0de

初여S

He巾

"臼 ' 堪自 '

E三3 ' 0,2

cDAl
!

團CDfll

I

듸mulatio4,

琵字 ' 團 ' E摯 ＜各心 膀

1으

1貫
4

cc.吐imJ며石

母

1

1

티
k

r蜘JJ1
Men묘Jre1

"

}

1

"

b

卜

mr듦；.忙2

11

[MeacJre3

닉

니m !

:

L小 +

1J
口

!:

口

LRe由

V帥able앉epDiscrete ::

i여挑

그림 20田 완성된 시뮬링크 모델

병렬로 연결된 두 저항의 전체 등가 저항은 다음과같다．
6
,
3X2
R+R2 = 3+ 2 =

=

R1R2

R,

R

=

옴의 법칙을 이용하면 다음을 얻는다．
.

Vs

6

-

/' ＝瓦＝云万＝小J
전류 분할을 이용하여 주어진 입력 전류 I = 5 [A쪄1 대한 부분 전류를 구하려면 다음과 같이 분모어七
구하려는 부분 전류가 흐르는 저항을 대입하고, 분자에는 병렬 저항 연결의 등가 저항 凡9 값을 대입한
후 주어진 입력 전류를 곱한다．

,:＝층Is：等／5=2[A]
12＝知은x 5 = 3[A}

550

PART 04. Sim매nk설계하2I

LESSON

02

저항, 인덕터, 커패시터 조합하기

저항은 자체적으로 에너지가 발생하지 않는 수동 소자이다. 저항과 함께 회로를 구성하는 데 반드시 필요한 수동 소仄F인 커패
시터와 인덕터의 조합으로 이루어진 RL 회로, RC 회로, RLC 회로의 시뮬링크 모델을 설계하여 그 역할을 살펴보자．

Keyword

1 ACVoItageSoute블록 I

IACV이怡ge Source 블록
AC Voltage Source 블록을 이용하면 이상척인 AC 전압원을 생성할수 있다．

1 여I iI 20- q !
J
J
'

"

"

1

!

卞

다음 日L 회로의 전류 IL ( t)를 나타내는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．여기서
/? = 10［회, L = l[H], 乙 = lOsin(150t)[V］이다．

그림 20-7 RL 회로

풀이

0 powergui 블록을 생성한다（[Simscape卜田imPowerSyste邱］ 田pecialized Technology]
[Fundamental 미ocks］七刃werg네）.
0 AC Voltage Source 블록을 생성하고（[Simscape］ 田imPowerSystem이 田pecialized
Technology］小［Fundamental Blocks卜田le面cal Sources]-[AC Voltage Source]) 블록의 이름을
Vs로 바꾼다．
0 블록＼'S를더블클릭하여 [Peak amplitude (V) :］어］10, 田requency (H기 :］에 1501(2如i)를입력한다．

CHAPTE日20. 회로

551

肖C Va艮ag日 Source (mask) (link)
Ideal 引nus이d引 AC Vohage sourc已
Param日tars 出쿄뇨二六F｝口뾰
Peak amr小山d日 (V):
10
Phase (deg):
0
다日qu日ncy (H力：
1표玖冬p1)
Sample lime:
0
Measurements！
卜妃ne

OK

y

[ Canc日I

H日巾

Apply

그림 20田 블록 Vs의 진폭. 주파수 설정

0 Series RLC Branch 블록 2개를 생성하고（[Simsc카）이 ［罰mPowerSystems卜囹pecializecl
Techn아og피4助ndamental 미ock司4目emet出卜田eries RLC Branch]) 블록의 이름을 각각 R, L
로 바꾼다．
0 블록 L을 클릭한 후 마우스 오른쪽 버튼을 누르고 [Rotate & Flip卜[Counterclockwise］를 실행하여 회
전시킨다．
0 블록 R을 더블클릭하여 [Branch type:］을 R로 바꾸고 [Res慨ance (Ohms) :］에 10을 입력하며，블록
L을 더블클릭하여 [Branch type:］을L로 바꾸고［如uctance (H) :］에 1을 입력한다．
Series RLC Branch (mask) (link)
Implements a series branch at PLC elements
Use the 'Branch type' 口arameler to add or r日m口ye 비emen怡
fr口mlii日 branch.
Parame伯rs
Branch type: LI.
Inductance (H):
1
기 Set the in崗al inductor current
h相asur日men佃 None

Cancel

그림 21）四

He巾

如ply

블록 L의 소자 변경과 인덕턴스 값 설정

0 Current 八4easurement 블록을 생성하고（[Simscape卜［SimPowerSystem引可Specialized
Techn아og列-[Fundamental 미ocks卜[Me朗uren妃nt司 ［Current Measuremen日） 블록의 이름을
Measure로 바꾼다．
0 Display 블록을 생성하고（[S趾司-[꺄叩lay]) 블록의 이름을 iL로 바꾼 후 블록을 모두 연결한다．

552

PART 04. Sim메nk설계하71

半핌b

Ed札

\flew

Of邱11ay

舜r 滔

Ot呵帥l

Simulation

Analys虹

Code

k刃七； He巾

力I哥
"呻 唾 姑 胎 雙 巨予미9 ! 蟲 ,

ALl L

的 團ALl

읖

!

C七.,tin町石
\i多

1

Pm甘O너i

二李
H十

八 八 八
'
；亡

n

團
1回

肇,

口

目
匕匕多H

i亡
宙

므

>>
Rea旬

l{y：吼

ode45

그림 20너0 완성된 시뮬링크 모델

0 시뮬레이션을 실행하면 다음과 같은 결과를 얻는다．
F如

玉刃t5

V足／/

S*mul笠口l

H핌口

Y

「＼

：「

1,

「

‘

,,，《／

\,

「＼

「

「

O ' i 兮 e 努 好 g亨 , 억 , ［꾜 , ! 李 國 ,

1
肛ody

R /V
Ii

2

IT-O2e0

그림 20너］ 스코프 창 결과

1 예제20니 1
다음 R(; 회로의 전압 Vc ( t）를 나타내는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．여기서
R = 6[c]. C = i0[mF], V = l5sin(150t) [V]0IEF.

그림 20-12 RC 회로

CHAPTER 20 회로

553

풀이

0 powergui 블록을 생성한다（[Simscape]-[SimPowerSystem玎-[Spe아alized Technology]
[Fundamental 미ocks］由川比rgii]).
O AC Voltage Source 블록을 생성하고（[Simscap司-[鈿nPowerSysten司-[Specia血ed I比뇨이ogy]
-[Fundamental Block司-[Electrical Soi丁ce玎-[AC Voltage Soi표ce]) 블록의 이름을＼'Is로 바꾼다．
0 블록Vs를 더블클릭하여 [Peak an町）litude:］에 15, [Frequency (Hz) :］에 150/ (2勺h）를 입력한다．
0 Series RLC Branch 블록 2개를 생성하고（[Simscape］나엷mPo吼rSystem玎- [Specialized
Technology]-[Fundamental Blocks]-[Elements]-[Series RLC Branch]) 블록의 이름을 각각 R, C
로바꾼다．
0 블록 C를클릭한후 마우스 오른쪽 버튼을누르고 [Rotate & Flip卜[C叱riterclockwise］를 실행하여 회
전시킨다．
0 블록 R을 더블클릭하여 [Branch type:］을 R로 바꾸고 [Resistance 幻hms) :］에 15를 입력하며, 블록
C를 더블클릭하여 [Branch type:］을C로 바꾸고 [Capacitance (F) :］어］ lOe-3을 입력한다.
Series ALC Branch (mask) (link)
Im머em日nts a s日n日s branch of 日LC 미ements.
Use the 1Branch type1 parameter to add or remove elements
from tie branch.
Parame也N

C

日ranch 如口e:

Capacitance (F):
t0e召
巴 Setthe initial Ca口ac的r voftage
Measurements 1幻ne

OK

Cane터

: ,j押去目幽，j

A口口如

그림 20-13 블록 C의 소자 변경과 커패시턴스 값 설정

OCi玎rent 入4easurement 블록을 생성하고（[Sirnscape卜田imPowerSystems卜田pecialized
Technology]-[Fundamental Blocks]-[Measure毗nt日-[Current 入4easurement]) 블록의 이름을
Measure로 바꾼다．
O1거splay 블록을 생성하고（[Sb止玎丑거spla피）블록의 이름을vC로 바꾼 후 블록을 모두 연결한다．
日i目 帥5

VIew

0娜4呼 i:Xa9rm1

닯mul ion

幻畇心

cc巾 크1唯 i卞晦L

섀訃呻 心 （孕 聆 ！匹 mk3! 發喜寸

唾，目 《
r HC]
念 團ACt

!

貫 HH!
=1

므

幽1

口
曲
翩
片

呻

"

...
1

J

V V V
a

軒

1
1

Re宅｛如

그림 20-14 완성된 시뮬링크 모델

554

PA日T 04. Simulink설겨同기

1L
1[
l以夙

1

"

1

므
0de45

O 시뮬레이션을 실행하면 다음과 같은 결과를 얻는다．
F가e

To어5

\／沌w

Simulation

咨'

H뺘）

出

a1 , ［二 . f 國 ,

/\/\/

끄＼

9, ' 嶝 (9 匹＞ S

「

／「

\\，《，

「

「
i弓

{; 2

T=O.2口：

肛ady

그림 20-15 스코프 창 결과

1 예제20小 1
다음 직렬 RLC 회로에서 R = 5[c], c = 0.25[F], L = i[I끄일 때 인덕터에 흐르는 전류 ZL ( t）를 구하는 시뮬
링크 모델을 설계하고 그 결과를 스코프 창에 나타내라. 단 ，전압원은 V5 = l0sin仁챠乂V］이고 초기 조건은
iL(0) = l[A], vc (0) = 5[V]0I다.
'R(t)

R

lj (f)

L

V5(t)

그림 20-16 직렬 RLC) 회로

풀이

0 powergui 블록을 생성한다（[Simseap이｛SimPo吼rSystem町4Specialized Technology][Fundamental Blocks]-[powergui]).
O AC Voltage Source 블록을 생성하고（[Simscape] -[SimPowerSystems卜田pecialized
Teemn아ogy］나Fundamental Blocks]-[Electrical Sources]-[AC Voltage Sos丁eel) 블록의 이름을
Vs (t)로바꾼다．
0 블록＼
／叭t)를 더블클릭하여 [Peak amplitude:］에 10, [Frequency (I七）:］에 l을 입력한다.
0 Series RLC Branch 블록 3개를 생성하고（[Simseap司-[SimPowerSyste邸］m田pecialized
Techn이ogy]-[Fundan妃n奴1 Blocks卜田lement引-[Series RLC Branch]) 블록의 이름을 각칵 R, L,
C로 바꾼다．
0 블록R을 더블클릭하여 [Resistance (Ohm乂H陌를 입력하며, 블록 L을 더블클릭하여 [Branch type:]
을L로 바꾸고 [In血야or 血而al current (A) :］에 1을 입력한다．

CHAPTEF극 20. 회로

555

Series PLC Branch (mask) (link)
Implements a series branch of PLC elements
Use the 日r日n口h 四口e 口aramnet마 t口 adder remuso 미日m日nb5
from the branch

1L

Paramne伯rs
日ranch by口甘

Inductance (H):
1
國Set the inital inth,ctor CUrrent
Induct口r In出al current (A):
1
Measuremen佑 ！幻Se

Cancel

1

He巾

Apply

그림 20卞］7 블록 L의 소자 변경과 인덕턴스 값, 인덕터 초기 전류 설정

0 블록 C를 클릭한 후 마우스 오른쪽 버튼을 누르고 [Rotate & Flij小［Counterclockwise］를 실행하
여 회전시킨다. 그런 다음 더블클릭하여 [Branch type:］을 C로 바꾸고 [Capacitance (F) :］에 0.25,
[Capacitor initial voltage (V) :］에 5를 입력한다．
Sen日日 日LC Branch (mask) )fsk)
Im미em日n相 a series branch of PLC element툐
Us日 the 'Branch HP日 param日伯rt口 add or remose 日伯m日sb
trots the branch,
Paramet마5
Branch type: C
Cape口it日one (F)
a25
團 Setthe in出씨 C日口actor so忙age
Ca口a口如nn出at ooltage (H)
5
Measurements N口ne

=｛巨r=

四面.

A口口山

그림 如-18 블록 C의 소자 변경과 커패시턴스 값. 커패시터 초기 전압 설정

0 Current Measurement 블록을 생성하고（[Simscape卜［SimP ow erS y stem玎-[Specialized
Techn이四列-[Fundamental 미ocks卜小k朗urements卜[Current Measurement]) 블록의 이름을
Measure로 바꾼다．
0 Scope 블록을 생성하고（[Sink司-[Scope]) 블록의 이름을LL (t）로 바꾼후블록을모두 연결한다．
目to

帥t ＼艇A

D畔thy ［瓦呼rant

琵

昆，目

Sinsolasen

An叫牌i

Code

is呻； 汁叫p

“呻 뗘 @ 昑 ,

匹 r甘 臼 , 蟲 ,

ffLCt }
e

團ALC1

臂

!

（上加h m1l巧

母

二

口0ne4和r

1

E回

VU U

5

L

枷）

i團
［그

V V V

力
ePa旬

556

PART 04. Sim메nk설계하71

.

［그

=

+

＝니q

]

虹
蜘

그림 20-19 완성된 시뮬링크 모델

!

Me.텨Jr七

i四％

0d45

0 시뮬레이션을 실행하면 다음과같은 결과를 얻는다．
Fib

初n{5

냅硼

simula0｛珌

14斛p

今 니 吟 8 和 小 帑 니 奴 d꾜 n f 囹 ,

그림 20-2() 스코프 창 결과

四 미분방정식을 이용하여 동일한 직렬 RLC 회로어｝대한 시뮬링크 모델을 설계하자．
F척b

帥t ＼月剛

囹r 圄

O邸by

C汁a伊am

針m甘1弑＄며i

Ar旺自r＄裡

Co<如 自어S

Help

: g븜 好，團！呻 愍 (8 雕＞ " 쓰 r

n

,, （多 r 饉 !

#LC2 1
田 團I9LC2

!
/n.

風
臼

<1

=0

뇨N
R

二

封 ,; ,
V뇨

,>

F-+

仇

m甘

E1
i쿄

, L
二J
hte4川口

乂j.

，二

hl뇨g甘a1

．了＝i
'

翩

LL。

,4

［回

1/C

冷
Re旬

100%

ode45

그림 20-21 미분방정식을 이용한 동일한 직렬 RLC 회로 모델

q1［그림 20 기］의 모델을 이용하여 측정한lL (t）의 결과는 다음과같다. ［그림 20-22］는［그림 20-20］과
거의 동일한 결과를 보여준다．

그립 20-22 스코프 창 결과

CHAPTER 20. 회로

557

연산 증폭기 이해하기
연산 증폭기（op amp: operation졔 amp甛er）는 출력 전압을 제어하는 전압원으로 사용할 수 있는 전자 장치로, 실제 회로를
구성하는 수동 소자와 함께 중요한 부품이다. 시뮬링크 모델을 통하1 반전 증폭기와 비반전 증폭기의 기본 개념 및 구성을 알아
보자．
Keyword

I 반전증폭71 I Op-Amp블록 1 日ectric졔 Reference블록 I S이ver Configuration블록 1
l v이atage Sensor블록 I PS-Simulink Converter볼록 1 비반전 증폭71 I

I

반전 증폭기

반전 증폭기（it싸erting an叩可ier）를 사용하면 출력 전압이 증푹됨과 동시에 연산 증폭기 내부에서 입력
신호의 부호 전확 때문에 입력 신호와 반대되는 음의 극성을 갖게 된다．

且 Op- Amp 뷸록
Op-Amp 블록을 이용하면 이상 연산 증폭기의 모델을 생성할 수 있다．

I 티ectr七al Reference 블록
Electrical Reference 블록을 이용하면 전기적 접지를 생성할 수 있다．

I

S이ver Configuration 볼록

S아ver Configuration 블록은 Simscape 라이브러리를 이용하여 연결되는 모든 블록을 시뮬레이션하기
위해 항상 필요한 블록이다．

I

\／이計age Sensor 블록

Volatage Sensor 블록을 이용하면 이상적인 전압 센서, 즉 회로의 두 지점 사미에서 측정된 전압을 전압
어］ 비례하는 물리적 신호로 변환하는 장치를 생성할 수 있다．

I PS-Simt川nk Converter 블록
PS -Simulink Converter 블록을 이용하면 회로의 물리적 신호를 시뮬링크의 출력 신호로 변환할수 있다．

558

PA日T04. 帥iutnk설계하:7 '

r예제20田 1
다음 반전 연산 증폭기 회로의 출력 전압 比를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라. 여기서
VS = i[V］이다．
4kt

그림 20小23 반전 연산 증폭기

풀이

0 DC Voltage Source 블록을 생성하고（[S恤scape卜伍oundation Libr町列-[Elect如al]-[Electrical
Soa丑ces]-[DC V毗age Source]) 블록의 이름을 vs로 바꾼다．
0 블록vs를 더블클릭하여 [Coi心tant voltage:］의 기본값 1V를 그대로유지한다．
DC Voltage Source
The ideal voltage 5口urc日 maintains a Constant 너出age aCr口vs Its 口U如나tterr州09冶』ind日pendent of the
current P口wIng through 由日 source. The 口utputu아tage is deltn日d by the Constants口卄age parameter and
can be any real value.
S口urn日 C口de
Settings
Pgram日也rs

i

C口netarlt 00陌ge:

口1

그림 20-24 블록 Vs에 전압 설정

0 Resis的r 블록 2개를 생성하고（[Simscape卜田oundati이i Library]-[Electrical]--[Electrical
Elemen蝴H區esistor]) 블록의 이름을각각RS, RF로 바꾼다．
0 블록RS를 더블클릭하여 [Resistance:］를 I. kO노U으로 바꾼다．
P日引針口r
The volt日ge-current (V나）rela卄口nshlp I口ra linear r日引帥or 冶 V=l*t4, a才mm n 泊 th日 C口nst日nt re引stance in
口hms.

忿篇紫烈譚蠶黑瓷읖器瑞뚫罵韶躍臘謐富觀詐麓豁鵠，.

w4,日nan니月ng thro나gh the de너Ce fr口m 小e 口0틔doe 幻 the n日gative terminal. Th泊 convent向nensures th日t
the 口ower absorb日d by a res沽切r 沽 al,晦ys p口澍live
S口니rc日 C口dv
Setdrras

kOhm

1 Cance口 L li민已J

A口ply

그림 20-25 블록 RS의 저항 설정

CHAPTER 20. 회로

559

0 마찬가지로블록RF를 더블클릭하여 [Resistance:］를4, kOhm으로 바꾼다．
0 Op-Amp 블록을 생성하고（[Simscap이[Foundation L小rai口卜田lectric出]-田lectric키 Elemen司
[Op中如Ip]) 클릭한후마우스오른쪽 버튼을누르고 [Rotate & Flip卜匹lip Block］丑巾-Dow미을 실
행하여 회전시킨다．
0 Simscape 라이브러리를 이용하여 연결되는 모든 블록을 시뮬레이션하는 뎨 항상 필요한 S아ver
Conf地uration 볼록을생성한다（[Simscape］小九ilitie司｛Solver Configuration]).
O 접지 (ground）를 나타내는 Electri沁 Reference 블록을 생성하고（[Simscape卜田oundati이I
Libra口卜田妃C打妃찌小끄毗油1Elements]-[Electrical Refere毗］) 블록의 이름을GND로바꾼다．
0 Voltage Sensor 블록을 생성하고（[Simscap이 伍oundation Library]-[Electrical]-[Electrical
Sensors]-[Voltage Sensor]) 클릭한 후 마우스 오른쪽 버튼을 누르고 [Ro扼te & Flip卜[F却 Blo味］
[Lef卜Righ日를실행하여 회전시킨다．
的 PS-Simulink Converter 블록을 생성한다（[S油scape卜띠tilities卜[PS-S油ulink Conve代en).
0 Display 블록을생성하고（[Sin蝴-[D娜）lay]) 볼록의 이름을vo로 바꾼다．
m 블록을 모두 연결하고 시뮬레이션을 실행하면 다음과 같은 결과를 얻는다．
F晦

E出t

View ［긔피出y ［거aqram

욘芬 , 冒 노

針m내苡幻n

An的4S

Code

i比45

H帥）

1 1旨믐 拿！國Y 呻 也 @ 恥＞ m 匹 !

斗 臼 , 筐自寸

OPAl 1
!

團OPAl

的
角j

므
RS

8

卜
야卜An뿌

'

臼蜘蜘

［團
國
[：그

FtF

f江）=0

［交

幽

帥b" 蜘

1

卜 1낀＝ q
;+

BdU目

=．미O

커

瓷客

易
Ready

100%

Vaiiabie닯epDi5crete

그림 20中而 완성된 시뮬링크 모델

출력 전압은 다음과 같은 비율로 나타낼 수 있다．

560

PART 04. Sim메nk 설계하기

RF

4 .. .

M

Vo = 1

j= Vs == H=
八2
1

7(

I

1

4

I 비반전 증폭71
비반전 증폭기（nor血가erting an巾姸ler）는 반전 증폭기에서 얻는 음의 이득값을 피하려 할 때 사용하는
연산증폭기이다. 비반전 증폭기를 사용하면 출력 전압이 증폭됨과동시어］입력 신호와동일한 양의 극성
을갖게된다．

1 예제20-7
다음 비반전 연산 증폭기 회로의 출력 전압 vu를 구하는 시뮬링크 모델을 설계하고 그 결과를 나타내라．
20kQ

그림 2(）呼27 비반전 연산중폭기

품이

0 직류 전압원（DC voltage source) 六를 나타내는 DC V毗age Sou吼e 블록을 생성하고（[Simseape］놔
[Foundation L小ra口]-田lee仕ical]-[Elect如al Sources卜[DC V毗age Source]) 블록의 이름을vs로
바꾼다．
0 블록vs를 더블클릭하여 [Coi好tant voltage:］를 3V로 설정한다．
0 저항을 나타내는 Resistor 블록을 2개 생성하고（[Simscape]-[Foundati아i Libra口卜田lectrical][E뇨沚ical Element寸［Resist아］) 블록의 이름을 각각RS. RF로 바꾼다．
0 블록RS, RF를 더블클릭하여 [Resis恤兀e.］를각각5kOhm, 20kO노n으로 설정한다．
0 Op Amp 블록을 생성하고（[Simscape卜[Foundation Libraj明-[日ec仕ical]中［Elee打ical Ele毗nt司
回p-Am히）클릭한후마우스오른쪽 버튼을 누르고 [Rotate & Flip卜田如 Block卜[I巾-Down搢 실
행하여 회전시킨다．
OS아ver Conflgura如n 블록을 생성한다（[S恤iscape］小Itilities卜田olver Con地uration]).
O Elee甘ical Re免rence 블록을 생성하고（[Simsca꺄卜田oundation L小rai明-[Electrical]-[Electrical
Elements卜田lee仕ical Reference]) 블록의 이름을GNI）로 바꾼다．
0 Voltage Sensor 블록을 생성하고（[S油scape卜田oundation Library]-田뇨滋ical卜田lectrical
Sensors]-[Voltage Sensor]) 클릭한후 마우스 오른쪽 버튼을 누르고 [Rotate & Flip卜[Flip Blo味］
[Left-Righ日를 실행하여 회전시킨다．
O PS-Simulink Converter 블록을 생성한다（[Simseape卜[Utilities卜必S油ulink Converter]).
G Display 블록을 생성하고（[Sink司 ［Di叩lay]) 블록의 이름을vo로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행하면 다음과 같은 결과를 얻는다．

CHAPTER 20. 회로

561

디挺

E出t

＼月태

O却切

[Xa多카TI

Sin카bt由a

ArIa卜ys朽

C｛그K如

自出5

'佃4P

昆 ! 딤 》，m公 n g믐 好 , 團 r 呻 4i @ 昑 毋 낟3!

，『（多 ! 幽 !

OPA2 1
!

團0PA2

宙

慰

므

RF

卜

［료

RS

國1
［그

야山1叩

4

\

肛）=0

E心

幽

, 뜨i

＄山口
Gnm口da自l

PS，斗mnt
（뇨m口뇨

L1＝ 희
茹

G11D

>>
R盛岫r

100%

V計m比ltepO虹rete

그림 2(卜28 완성된 모델의 결과

출력 전압은 다음과같은 비율로 나타낼 수 있다．

切= (畔加小*誓江15Ev]

562

PART 04. SirT띠link설계하71

LESSON

04

전력 사용하71

교류 회로에서는 시간에 따라 변하는 순간 전류와 순간 전압을 이용하여 순간 전력을 구한다. 그러나 순간 전력을 구하는 것이
쉽지 않기 때문에 순간 전력의 평균긺인 평균 전력을 이용한다. 순간 전력과 평균 전력을 나타내는 시뮬링크 모델을 설계해뵤짜．
! 순간전력 1 평균 전력 1

Keyword

I

순간 전력

순간 전력 恤stantaneous power）은 다음과 긷히 시간어］ 의해 변화하는 순간 전압과 순간 전류의 곱으
로 구한다．
可 t) = V（小(t) [W]

1 예제20田 1
순간 전압 v(t) = 165cos(l0t+ 20 ")[V］와 순간 전류 巾）= 20sin(l0t+ 60 ")[A］에 의해 생성되는 순간 전
력을 5초 동안 보여주는 시뮬링크 모델을 설계하고 그 결과를 스코프 창에 나타내라 ．표본 시간은 0.01同로
설정한다．

晉이

0 Sine Wave 블록 2개를 생성하고（[Source引-[Sine
Wave]) 블록이름을각각v (t),i (t)로바꾼다．
0 블록 v (t）를 더블클릭하여 [Ampli毗e.］어1 165.
[Frequency (rad/sec) ;]에 10, [Phase (rad) :]에
pi/2+pi/9, [Sample time:］에0.01을입력한다. ; ,
0 블록 i (t）를 더블클릭하여 [Amplitude:］에 20,
[Frequency (rad/sec) :]에 10, [Phase (rad) :]에
pi/3, [Sample time:］에 0.01을 입력한다．
0 순간 전압과 순간 전류를 곱하기 위한 Product 블록
을 생성하고侮4ath Operations卜[Product]) 더블
클릭하여 [N毗ber of ii叩uts:］에 2를 입력한다．

텨ne Wave
Out口uta 여flu was日
O(t) = harp士Sln(Freg.t.Phase) + 日泊日
돼flu S口日 d日t日rmines We C口m口ut日ti口sal 佃的niqu日 us日d. Th日
口aram日伯rs in the toO ty口as are r日sled 小rough
Samples 口Sr 口目hod. 츠pi / (Frequency 士 Putt口1a tSr日）
Numb日rot 口卄B日team口陀B =Phase * Samples 口er 口日r1口d/ )2*口D
Us日 the Sam히c-based 引ne type 什 numerical 口r口blsms 山a to
s.vnnlns f口rlarge 卄mes （日g 口ourt口win abs口lu佃 甘mB) 口Ocur.
Parameters
텨n日 tll口日： 끄me ba＄日d

m

lim日（牡 雁百i而而的0甘me

;]

肉npit나d峀
1gb
日1a5:
0
杆日as日nec (red/see):
IS
Phas目 (mud)
하／2＋아9
Sent히e 甘me
S0)
團 1star口r日to日Ct口r 口ar日m日tars CS ] 山

匹玉重그 小H믿p ]
9
그림 20-29 Sine Wave 볼록의 매개변수 지정

CHAPTER 20. 회로

563

Pr口duct
Mu娜加 or 뎨너d日 in叩怡． Cho（始e 미ernent씨／Se 口r matrlo 口roduct and
S口日city on日 of th日 幻如帖n5:
a) * or / 伯r 日ach input ）口凡 F七rena까H日，"11 口日r化rms th日 0口eratlon
'ut 口u2/u3*u4'
b) scalar op日clii日Sthe number of input 口orts to be mu川口h日d
11th日r日 治 only one in口내 port and the Mu뺘네Ca如n 口cram日icr 冶 Set to
티日m日nt-sd的C1), a 이ngle * or / C에a口S日stir日 In口ut 틔gn졔 니引ng the
S口日dli日d operation. H口＼Meyer, 卄 the Multh川cation 口ararn日佃r 冶 sell口
Maple).). a 引n이B * causes the 비ockto o나巾ut the matylo 니nchenged,
and a single / causes the block to output fEte matrix Inverse.
Main L昴gn셰枷加相8 1
Number of inputS:
2
M니h巾licati口n: 1Elemenl- wise)，日

,

.，싸

I1

Cancel

1

OK

II日巾

知p如

그림 a卜30 Prt刈uct 볼록의 입력 단자 수 설정

0 Scope 블록을 생성하고（[Sin畑卜田cope]) 블록의 이름을p (t）로 바꾼후블록을모두 연결한다．
日Ic

Ed忙

Vi引Y ［站머aty

Diagram

듸mel盛K月s

Mut好d

cc巾 bete

l枉Ip

" 旨骨1 呻 叫 @ 昑 『 回 ,,, 凹 , 幽 !

蚣｝ , 目
P0놔1

V

回P0나1

e

烈
U

吼

드

自 旦

4
團
匹
口

ode45

l伉戊

Red旬

그림 20-31 완성된 시뮬링크 모델

0 [Simulation] 메뉴를 클릭하여 [Model Configura如n Parameters] 창을 열고 [S切rt time:］에 0, [Stop
血ne:］에 5를 입력한다．
0 시뮬레이션을실행한후 Sc叩e 블록을 더블클릭하면 다음과같은 결과를 얻는다．
日b

To出； Ww

@

心 (9 i> 1

Sin甘J1吼inn

卜佃｛P

끼

咨 · q , 匠J

至 a,

1r “，니 r' n U r

a尤亡

1二q:

느．
=:
1

L

느

m

,

\

,

,

'

.

1

1

,

.

.

.

J

,
녀

40

,
5

T.S 000

Ready
그림 加32

,

스코프 창 결과

시간이 小5초 동안 계속 변할 때1 교류 회로는 전류와 전압의 값이 계속 바뀌는데, 이러한 전류와 전압을
각각순간 전류, 순간 전압이라고 한다. 이 순간 전류와순간 전압을 통해 회로의 소자에서 소모되는 전압
인 순간 전력을 확인할수 있다．

564

PART 04. Sim메nk설계하71

I

평균 전력

순간 전력을 1주기 T 시간 동안 시간어］ 대해 적분하고 평균을 꼐산하는 평균 전력 (average power）은
다음과같이 정의한다．

Pavg나f'p(t)町WI
1 예제 20-9 I
5초 동안 순간 전압 v(t) = 165c05(l0t+ 200)[V］와 순간 전류 巾）= 20sin(l0t + 600) [A］에 의해 생성되
는 평균 전력을 보여주는 시뮬링크 모델을 설계하고 그 결과를 나타내라. 표본 시간은 0.0小］로 설정한다．

푿이

Os加eW鉀C 블록2개를생성하고（[Sourc明卜田血e Way司）블록의 이름을각각v (t), i (t)로 바꾼다．
0 블록 v (t）를 더블클릭하여 [Amplitude:］에 165, [Frequency (rad/sec) :］에 10, [Phase (rad):]
에 pi/2+pi/9, [Sample time:］어］ 0.01올 입력하고 ，블록 i (t)를 더블클릭하여 [Amplitude:］에 20,
[Frequency (rad/sec) :］에 10, [Phase (rad) :］에 pi/3, [Sa끄riple time:］에 0.아을 입력한다．
0 Integrator 블록을생성한다（[Commonly Used Block司-[Inte孚毗or]).
O Cons恤止 블록을 생성하고（[Commonly Used B뇨永引-[Constan日） 블록의 이름을 주기를 나타내는
I로 바꾼다．
0 블록T를더블클릭하여 [Cor喊ant value:］에 5. [Sam마아恤e.］에 0.01을 입력한다．
Constant
Out口Ut the con引ants口ec而日d by th日 'Constant 四山日’ 口arametar. 忖
ton針ants쉐U日‘ in a sect마 and 'Intert가etsector 口ararnet日r5 aS卜0' 泊
口n, 的auts日 C口nctant Va仙e as a 卜 ［) 카ray. OtherwIse, ou如at a nab似
내g, the same 네m日n5幻no as th日 C口n引anti刮Ue

투二帥
r瓦而 i：횰｛go赳角自哥J西百그

0K

0

Cancel

H日巾 m 1 A口ply

그림 20-33 （力ns怡nt 블록의 상숫값 설정

OD加ide 블록을 생성하고([入4ath Operations]-[Divide]) 더블클릭하여 [Number ofh叩uts:］는 기본값
水／를 그대로 유지한다．
Pr口dact
h仙川Pill 口r dl너da In口ate. Chons目비8mar51十M5e 0r ma打ix 口r口duct and
5口8c加 On日 ntth이0的wtrtg
a) . 口r／伯r 日act, in口Cd O凡 F七r 日nampl日』n/ 1口日rl口rs,sth日 nperat向n
'alrw2Ju3.x4.
F.) scalers口日cItes the number 口1input porlst口 b日 mU뺘꿰ed.
卄there Is Only On日 input port and the Mu뺘川Cat幻n 口amamo也r 治 S日Ito
티日mont-U相吼0』a 引no伯 士 口r/ cxlia口south日 n口it 引goal U引ng the
spec州ad o口日ra如1. HO낚e蛇r, it the 卜／U뺘네Cat匕n 口aramet日r 泊 set to
Manis(-). a 引n미e 1 Ca나non th日 벼口ckt口 口J四utth日 matrix unchang日d.
and a 引n미日 / causes H他 늬ack I口 0U加utth日 matrix In叩rS已

maln ［函匣巫如區그
Number 口n叩너由：
'I
Miii如licati口n

J

E冶men卜MB日C나

1而而可1

H日巾

i

A口口1y

그림 20-34 D卜／ide 블록의 입력 설정

CHAPTER 20. 회로

565

0 Display 블록을생성하고（[Sink司-[Di叩lay]) 블록의 이름을Pavg로 바꾼다．
0 블록을 모두 연결하고 시뮬레이션을 실행하면 다음과 같은 결과를 얻는다．
FUe

由5

'／
卜e咐 ［거喇可

昆中圄

"

匹呵켜n

鸚

"

S卞mUaUon

呻也8

Anay出s

Code

下)ols

He巾

聘 匹 匹 !,, ＼已7 寸 幽

!

P0쌔2

企 團P0놔2

烈
長코
4

團

田

自

!

x' 未

肛「

團
［그
E毖

毖
冷
Roe小／

'cc比

0de45

그림 20-35 완성된 시뮬링크 모델1

순간 전력을 l주기 T= 5초 동안 시간어］대해 적분하고 평균을 계산하면 평균 전력 1053[W］를 얻는다．
이론적 계산으로 평균 전력을구하면 대략 1060EV띠인데, 이는 시뮬레이션의 결과와 미미한차이이다．

566

PART 04. Simi川nk설계하기

I

n d e

x

단위 귀환 시스템

198

186

단위 벡터

292

가우스 법칙

319

닫힌 루프 시스템

가우스 소거법

159

대처1

가우시안 확률변수

356

덧붙이기

가위치법

182

더1
a

가제어성 표준형

217

등고선 그래프

86

가중치

186

디버깅

37

각주파수

436

디지털 신호

247

감쇠 단순 조화 진동자

423

감쇠비

220

감쇠지수주파수

222

라플라스 방정식

감쇠진동주파수

222

라플라스 변환

경계 조건

327

라플라스 역변환

경우의 수

348

라플라시안 연산자

고역 통과 필터

501

램프 함수

고유 벡터

133

레이텍

고유 임피던스

344

롬버그 적분

고유주파수

220

루

고윳값

133

룬게쿠타 방법

고조파

268

리차드슨 외삽

곡면 적분

303

맥스웰 방정식

과도 응답

222

메모장

관계 연산자

94

명령 창

광대역 필터

206

무손실

가우스 구적법

2

198, 454
61
63
306

1 口

333
131, 204, 277, 458

333454

후르비츠（Routh냐札rw仕기 판별법
22519。

3526

구면좌표

300

무제동 응답

구조 배열

121

문자열

구형 함수

246

귀환 경로

198

균일 평면파

344

반송 억압

360

그래픽 사용자 인터페이스

546

반전 증폭기

558

발산 정리

341

그림 창

28, 400

너

그림 파일

136

배열

52

극점

280

배열 연산자

60

극좌표

239

백색잡음

367

극한값

125

범례

78

급수

126

벡터

292

근꿔1적

228

벡터 삼중적

295

기본 주파수

268

벡터의 내적

293, 515

기저 함수

377

벡터의 발산

306

벡터의 외적

294, 5佰

벡터의 회전

310

나이퀴스트선도

239

변수

나이퀴스트율

262

보드선도

48
234, 476

내장함수

50

복소수

410

논리 연산자

96

복소 위상

342

누적분포함수

353

복소 주파수 벡터

236

뉴턴법

179

부분분수 전개

206

니콜스선도
단위 계단 함수

241, 476
248, 454, 486

부분 피버팅

163

부엽

288

찾아보기

567

I

d

n

e

x
123

순간 전력

563

221

순수 가우스 소거법

159

230

순환문

101

350

스칼라 삼중적

295

붜 밖

부정적분
부족제동응답

분석방정식

274

스크립트 파일

34

블록

388

人두극人 정리

341

비례1미분 제어기

473

스플라인 보간법

173

비례 제어기

470

시뮬링크

386

비반전 증폭:7 '

561

시뮬링크 라이브러리 브라우저

386

비순환 필터

286

시변 시스템

254

비사바르 법칙

336

시불변 시스템

252

비정칙행렬

152

시스템행렬

213

비주기 신호

245

신호 대 잡음 비율

367

비트율

377

신호 복원

264

人

신호점

379

신호흐름선도

463

사다리꼴 적분법

184

심벌릭 툴박스

110

사상

239

심슨 적분법

185

싱크 함수

245

사용자정의함수

105

사인 파형

436

사칙연산

403

0

삭저1

61

아날로그 변조

358

산술 연산자

44

아날로그 복조

363

산점도

381

아날로그 신호

244

삼각함수 항등식

449

아스키코드

147

상대1 오차

150

아이 다이어그램

381

상대 유전율

328

안정도 판별법

225

상미분방정식

128

암페리안 경로

339

상삼각행렬

161

암퍼때 법칙

339

상쇄 필터

286

양자화

365

상승 시간

222

에너지 밀도

323

상태공간

213

엑셀 파일

139

상태방정식

213

여인자

153

상태 벡El

213

역 z 변환

상하행렬 분해

]61

역행렬

샘플링

260

연산자의 우선순위

47

샘플링 주71

260

연산 증폭기

558
244

283
152, 156, 509

샘플링 주파수

260

연속 신호

섀넌（Shannon）의 샘플링 정리

262

연쇄

선 적분

302

열린 루프 시스템

선전하

315

영점

280

선형 보간법

171

영차 흘드

264

선형연립방정식

155

오버슈트

222

설계 창

387

오일러 공식

266

세미콜론

53

오일러 방법

194

완전 유전체

328

63
198, 468

소괄호

47

소행렬식

153

왼쪽 나눗셈

155

손실

344

우반평면

225

수반행렬

153

원통좌표

298

수정된 오일러 방법

195

위상

436

568

찾아보기

I

n d e

x

위상각

234

제어기 표준형

218

위상변수 표준형

217

제어 벡터

213

위상 속도

344

조건문

98

위상 스펙트럼

268

조판 형태

118

위상 응답

281

좌반평면

225

위상차

234

주기신호

244

유전율

314

주석

36

이득 계수

228

주파수 감도

361

이분법

178

주파수 겹침

262

이산 비주기 신호

247

주파수 변조

361

이산 시스템

252

주파수 응답

234, 281

이산 신호

247

주파수 천이 변조

이산 푸리에 급수와 계수

272

중괄호（[ ])

52

이산 푸리에 변환

274

중심극한정리

356

인덕터

331

지수승

45

인덕턴스

331

지수함수

45

임계점

240

지연선

286

임계제동 응답

221

직교 위상 천이 변조

임펄스 응답

208

직교좌표

임펄스 함수

250, 486

입력행렬

213

乂

538

377
239, 298

진폭

436

진폭 변조

358

진폭비

234

진폭 스펙트럼

268

자기선속 밀도

329

진폭 응답

작업 공간 창

27

진폭 천이 변조

저역 통과 필터

501

전기선속 밀도

319

281
369, 538

첨둣값 시간

222

208, 280, 496

체적 전하

333

전달함수 병렬 연결

210, 461

초기 조건

204

전달함수 직렬 연결

210, 460

추가

61

전력 스펙트럼 밀도

367

출력 벡터

213

전류 분할 법칙

549

출력 서식

67

전송행렬

213

출력 서식 명령어

67

전압 분할 법칙

547

출력행렬

213

전위

325

치환행렬

163

전위차

325

커패시터

321

전기장
전달함수

314

전진 대입법

162

커패시턴스

321

전치 연산자（' )

57

컨벌루션

256

전치행렬

506

코사인 함수

443

절대 안정도

225

콜론（:)

54

절대 오차

150

콜론 연산자

58

점전하

314

콤마（,)

54

정방행렬

152

쿨롱의 법칙

314

정상상태 오차

222

크래머 법칙

15工 512

정상상태 응답

222

테일러 급수

124, 166

정적분

123

테일러 다항식의 근삿값

정정 시간

222

테일러 다항식의 오차

168
170

정칙행렬

152

테일러 정리

166

정현파 함수

244

톤 주파수

275

짖아보71

569

I

n d e

x

특성방정식

220

끄 It

Constant 블록

403

contour

86

cony

230

파수

344

Cosine Wave 블록

394

편집 창

28

cross

294

편향 각도

436

아oss Product 블록

515

평균

350

cumsurn

362

Current Measurement 블록

549

평균 전력

565

포물선 입력 함수

201

표면전하

317

표본 공간

348

DC V이tage Source 블록

546

표준편차
피드포워드

350
210

debugging
dec2bin

147

DI E
37

피벗

159

Demux 블록

410

하삼각행렬

161

det

153

할선법

180

Determinant of 3x3 Matrix 블록

합성방정식

274

뎨ff

288

뎨mpulse

284
322
405

해닝 창 함수
행렬식

了52, 509

508
122, 190

허수 단위 변수

48

데sp
미5이ay 블록

헬름휼츠 방정식

344

Divide 블록

현재 폴더

38

d（兀

31

현재 폴더 창

26

d아

294

406

협대역 필터

206

[）아 Product 뷸록

확률

348

double

115, 191, 345

확률밀도함수

354

ds이ye

128, 191, 334

후진 대입법

159

日g
日ectric졔 Reference 블록

AIBIC

515

133
558

els帥문

99

abs

170

end

98

acos

296

ex口and

112

AC \／이tage Source 블록

551

eye

53

addpath

38

eyediagram

381

ez히아

119

Add 블록

408

angle
atan2

268

ax円

74, 229

factor

112

bi2de

380

feedback

199
266

299

F

bin2dec

147

ftt

bisect

178

fftshift

270

bode

234

figure

80, 237

Bode I긔아 블록

476

꿰ter

286

cd

38

find

65

cell

348

日F극필터

286

char

334

fliplr

218

charp이y
clear

133

什pud

218

Ill

Fur) 블록

418

Clock 블록

400

幻r문

101

c에ect

113

Fr bin2dec

148

Corn이ex to Magnitu由An이e 블록

412

Fr dec2bin

149

570

찾아보기

I

n

d e

x

freqs

236

mesh

85

freqz

281

rneshc

88, 325

From File 블록

443

meshgrid

function

105

meshz

89

fzero

176

mm

350

卜川n卜기ax 블록

525

G ' H ' I

85

modem.qammod

381

mod미ate

380

Gain 블록

416

Gauss
grad

160

Mux블록

400

334

卜小직교 진폭 변조

379

grid

74

卜小파일

34

야ext

75

newt（기a

180

hann

288

nextpow2

360

hel口

30

nich이S

241

네gh口ass 테ter 블록
hi計

501

Nich이s Plot 블록

476

348

norm

292

hold

71

Norm帥zation 블록

515

十이se문

98

n아mc(打

355

if ft

270

normpdf

355

f문

98

nyquist

240

ila히ace

131, 278

image

136

impulse

208

0de23

192

imread

136

0de45

192

nline

288

ones

53

n口Ut

322

O口Am口 블록

558

mnt

123, 18乙 336

m t四rator 블록

397

O ' P rO

口arallel

2서

디［) Con打에er 블록

468
468

interpi

171

F：기D 제어기

nterp2

172

plot

70

1nv

154

이ot3

84

Invert 3x3 M欲rix 블록

508

p이y2sym

116

ztrans

284

F兀werg네 블록

546

아etty
Product 블록

118, 334

L 'Mi

N

Ia이ace

131, 277

405

PS-Sim메nk（沁nverter 불록

558

legend

78

口wd

39

len야h

66

281

limit

125

pzmap
quad

186

linspace

58

quadi

186

load

29

Lo이c졔 Opera加r 블록

510

look幻r

32

Ram口 블록

455

Lowpass 日仕er 블록

501

rand

348

Isim

200

randn

349

Magnit내把An이e to Corn口ex 블록

413

Random Number 블록

525

Math Function 블록

506

Real-Imag to Corn이ex 불록

410

Matrix（兀nc計enate 블록

512

regula

182

R

max

170, 350

reshape

380

mean

350

residue

206

찾아보기

571

I

d e

n

x

rloctind

231

text

75

riocus

229

tf

199
213

rmpath

38

tf2ss

romberg

188

title

74

roots

175

To File 블록

443

round

151, 350

兀 Workspace 블록

400

Rounding Function 뷸록

522

가ansfer Fcn 블록

454

routh

227

卄apz
Trigonometric Function 불록

184

Un幻rm 딕andom Number 블록

522

S

528

save

29

V이atage Sensor 블록

558

scatter이ot

381

\／이怡ge Measurement 블록

546

Scope 블록

390

waterfall

89

secant

181

wh陀문

103

semilogx

72, 237

sen꿰ogy
series

72, 237

Series 日[C 탸anch 블록
sgrid

XIYI

Z

211

xlabel

74

546

川sread

139

230

川swrite

139

ylabel

74

185

Zero-Order H이d 뷸록

531

Sine Wave 블록

394

zeros

53

미ze

66

z이ane

282

z변환

280

引mplify
simpson

114, 306

5이ye

120

S이始八二on徊내帥on 블록

558

5아t

353

Spectrum Analyzer 블록

501

卞（별표）

44

하케ne

173

/（오른쪽 나눗섣J 연산자）

44

ss

215

\（왼쪽 나눗셈 연산자）

44

ss2tf

215

stairs

264, 353

工자

State-Space 블록

463

］차 미분방정식

416

std

351

2진 소수

148

stem

247

2진 위상 천이 변조

374

step
stepfun

199

2진 정수

146

248

2진 주파수 천이 변조

371

Ste口 뷸록

454

2차 미분방정식

423

小위상 천0I 변조

377

115, 190, 302

伯진소수

148

Subtract 블록

416

10진 정수

146

sum

353

Sum 블록

390

subplot
subs

79, 248

surf

86

sym

110

sym2p이y
syn冶

116

symsum

126

110

T i Ui V iW
taylor

572

찾아보기

124, 166

Function

m
abs

&

Block

Demux 블록

예제 13田

예제 8너4, 예제 +19, 예저110-13, 예저I 10-14

det

예제 10너6, 예제 10叫17, 예제 10-23, 예제 12田

Determinant아3x3 Matrix *톡

acos

예제 11十

AC Voltage Source 붚륙

예제 2아3, 예제 20닉

Add볼록

예제 仍규

ang厄

예제乎19, 예제 化너4, 예저110-16

atan2
a川S

d附

Index

예제 8巧. 예제 于8
예저1 侶모

예제 6너］, 예제 서-11, 예제 11-12, 예저Ill中］3
예저111-14, 예제 11-15, 예제 j］너6, 예저Ill小27
예제 10-21

dimpulse
d治p

예제 9-15, 예저110너9, 예제 10-21, 예제 11叫껌

예제 10-17, （계저110너8

（계저111-24, 예제 11-25, 예제 ]1-26

예제 11-7, 예제 j］田

예제 11-27, 예저111-28, 예제 11-29

예제 哥］5, 예제 8너6, 예제 9-16, 예제 乎］7
예제 9-19, 예제 9-20, 예제 化丑, 예저110-4

예저111-30, 예저111-31, 예제 11-32
예제 아4, 예제 11-25

d治히ay

예저110毛 예제 ]0-但，예제 10-13, 예저10-15

［거S히ay 블록

예제 13田

예저110-刃，예제 1아22, 예저1 10-23, 예제 ]2-7

D押뗘e 블록

예제 13十, 예제 17너, 예제 20+

11
bi2de

doc

예저i卜2

d야

예저i11-3, 예저111-4, 예제 l］巧

예제 12-16

bin2dec

예제 8너

bode

예저Ill田, 예제 ]1-24. （계저！11-25
D야 Product 믈록

（계저1 侶4

예제 아］8, 예제 9너9

doub怡

예제 于4, 예제 ]0너9, 예제 10-어, 예제 11-32

예제 16-11

ds이ye

예제 6너6, 예제 6-17, 예제 11-27

Bode Plot 블록

日느

4

cell

예제 12너, 예제 促田, 예저너2巧

eig

예제 6-19

char

예저111-27

티ect,祀al Reference 블록

예제 20田

예저113-4

expand

예제 6-2

collect

예제 今3

eye

예제 +7

eyediagram

Corn히ex to Magn仕ude-An아e붚륙

예저13田

Constant 블록

예저113巧

contour

예제 4．田

cony

예제 아17, 예제 10-15

cos

예제 3巧

Cosine Wave블폭

예제 仍丑, 예제 ]5巧
예저I ll田, 예제 11-4, 예저I ll巧

cros$

ezp幻t

예제 12너6
예제 于8, 예제 6너6, 예제 6너7

1=
factor

예제 于2

feedback

예제 乎j

fft

예저110-13, 예저110-15, 예저110너8

예제 11-28, 예저111-29, 예제 11-31

예저112-7, 예저112너4

Cross Product붚콕

예저I 18-8

fftsh附

예저1 化너5, 예제 12寸. 예제 ]2너4

cumsurn

예제 12田

figure

예제 于］9, 예저110-20

Current Measurement 블록

예제 2아2, 예제 20巧

find

예제 于］6

filter
F印！톡

예저114-2

DC Voltage Source *록

예제20너

f먀)lr

예제 9-11

dec2bin

예제 8너

flipud

예제 9-11

함수／명령어／블록 찾아보기

573

Function

& Block

化r

Index

예제 아13, 예저1］아］6, 예제 j］너8

11

예제 11-19, 예저Ii］尸20, 예저111-22

laplace

예제 6너8

예저112-13, 예저112-14. 예제 ]2너5

legend

예제 4-3. 예제 8-13, 예제 9너3

예제羽＆ 예제8-4, 예제的4

length

예제3-17, 예제5巧，예제 价仔，예저110什］4

化rmat ong
freqs

예제 9너9

freqz

예저I 10-20, 예제 幻-23

예저1 10딥, 예제 12-3, 예저12巧
예저1 12크 예제 促너3, 예제 促너4

From F加 볼록

예제 15-3

uirn仕

仁ero

예제 8-18

linspa（冶

예제 6너4
예제 3-11, 예제 8-芻
예저너8田

목
L四化키 Operator！

m
예저1 14너, 예저1 14-4, 예제 14-5

Gain*R

예제 午2, 예제 8-13, 예제 9너, 예제 9田

grid

예제 아13, 예제 9너4 , 예제 9너6, 예제 9너8

Iookfor

예제］田

Lo놔pass Filter블록

예저17十

忖im

예제 9너

lu

예제 8너0

예제 乎20, 예저110너, （계저110丑, 예저i10中：3
（계처110닉, 예저Ii아5, （계저110-14, 예저110-19

1m

예제 10中기, 예제 10-22, 예제 10-23, 예저I 12-8

Magn仕ude-A四厄 to Corn히炚 블록

예저i13너0

Math Funct向n 블록

예저1 侶너

Matrix Concatenate 블록

（계저！18-4

예제 4-2. 예제 5-4, 예제 9-1. 예제 9-2

gtext

1[1

max

예제 8-14, 예저i12-2, 예제 12-7, 예저112-10

hann

예제 10-23

mean

예제 12-2

he巾

예저Ii너

mesh

예제 4田

예저117-7

meshc

예제 午7. 예제 11-24

네ghpass Filter븀콕
h治t

（계저1 促너, （계저112丑

h이d

예제 9-13, 예저110너0, 예저110-11, 예제 10-12
예저1］아22, 예제 10-23, 예제 12巧, 예저112田

예제 4十，예제 4크 예제］卜23

meshgnd

예제 午7

me針그
mmn

예제 12丑, 예저1 12-3, 예제 12巧, 예제 12너0

MinMax 블폭

예제 19-2

modem.qarnmod

예제 但너6

예저！11中25, 예저！12너3. 예제 12너4, 예제 12-15

modu怡te

（계저i12-16

예저110-15

Mux븐륙

예제 侶-4

iffi

예제 6-18. 예제 9크 예제 9-4, 예제 10-19

ilaplace

impulse

예제＋5

inline

예저1 10-23

input

예저1＋기，예제 서-24, 예제 11-25, 예제 서小26
예제 6-12, 예제 乎而, 예제 11-9

mnt

예저Ill너0, 예제 ]1-28, 예제 11-29
Integrator 뷸록
interpi

11
예처12크 예제 12너3. 예저112너4

nextpow2
n七h이＄

예제 +21

N七h이＄ F기ot 뷸록

예제 16-12

norm

예저Ii］너, 예저111-2, 예저Ill田, 예저Ii］中17

예제 仍-3' 예제 似田，예제 ]4규
예제 8너5

예저Ill너8, 예제 11너9, 예제 11-32
Normalization 블록

예제 侶田

예제 于5, 예제 +7

nomicdf

예저112-4

Invert 3x3 Matr以 볼록

예제 侶丑

normpdf

예저112닉

iztran$

예제 10-21

nyqu治t

예제 9-20

mnv

574

함수／명령어／블록찾아보기

Function

&

Block

Index
예제 ]2什］6

reshape
0de45

예제 +30

residue

예제 아4

0de23

예제 乎30

Res治如r뷸록

예제 20田

ones

예제 于7. 예제 9너

iloctind

예제 9-너7

예제 20田, 예제 20-7

r幻cus

예제 9너6

OP-Amp 블록

m

ro야5

예제 小］7

round

예제 乎4, 예저112-2, 예제 12-10, （계저i12-12

예제 9田

parallel
F기D Contrc川er 볼록

예제 ]6田, 예저1］于9, 예저116너0

예제 8너3, 예제 乎］5, 예제 8-16, 예제 9너

plot

예저112-13. 0杯｛112-14, 예제 ]2너5
Rounding Function 뷸록

예제 伶너．예제］乎7
예제 9너5

routh

예제 乎3, 예제 9巧, 예제 9-6, 예제 +13
예제 9-18, 예제 9너9, 예제 伯너, 예제 10쿄

m

예저110너0, 예제］아］j, 예저110-12, 예제 ]0-15

scatter下加t

예저1 12-16

예저110-17, 예제 10-19, 예저112田, 예저112叫7

Scope볼록

예저13-1, 예처14田

예제 12七, 예제 12田, 예제 12너0, 예제 ]2-11

sernilogx

예제9-19

（계저1 12-12, 예저112너3, 예저112너4, 예제 12-15

sem如gy

예제 ]2너4

p10t3

예제 4巧

series

예제 9田

p이y

예제 6너9

Series RLC Branch 볼록

예제 20너

p이y2sym

예제 6田

sgnd

예제 9너7

powergui 블록

예제 20너

미etty

예제 今7, 예제 아4, 예저110-19

예제 11-13, 예저Ill너4, 예제 11-15, 예제 11너6

예저110-껌, 예저111-27, 예제 ]1-28

예저Ii］中27, 예제 11-31, 예졔 11-32

예제 ]1-29, 예제 11-30, 예제 ]1-31
Produ（比 붙록

針mplify

예제 6닉, 예저10-너9, 예제 ]0中21. 예제 11-12

예제 13田, 예저117日, 예저118巧

PS-Sim매nk Converter 붚록

예제 20田

1끄map

예저1］아20

예제 于5

섧n

예저113쿄, 예저115너

Sine Wave 뷸록

예저1 行丑, 예제 20田
이ze

예제 十17, 예저112中］j

＄이ye

예제 于9, 예제 6너0

S이四八允nfigurat幻n 뷸록

예제 20田

quad

예제 8-25

sort

예제 ]2-3, 예저112巧

quadl

예제 乎25

Spe야rum Ana忖zer 볼록

예제 ]7田, 예저117尸7

4

sqrt

randn

예제 9너4, 예제 ]1-7, 예제 ]1-8, 예저111-25

예제 伶丑

예저1 11-28, 예제 ]1-29, 예제 11-32, 예저112-5

예저i12너, 예제 12-3, 예저i12巧

｛계저112너3, 예제 12-14, 예저112-15

Ramp뷸록
rand

예제 8너6

SI：川ne

예저112너］, 예저112-12, 예제 12너3

ss

예제 9너0

예저112너4, （계저112-15, 예제 12-16

552ff

예제 9너0

예저112丑, 예제 12巧, 예저i12-11

stairs

예저1 好너2, 예제 12-3, 예저i12巧

Random Number블록
real
Real-Imag to Corn히ex블록

예저i19丑
예저1 11-31, 예제 ]1-32
예제 仍田

State-Space 블록
std
stem

예저1 16田
예졔 12-2, 예제 12-11

예저i10田, ｛계저110巧, 예저1 好毛, 예저110-7

함수／명령어／블록 짖아보기

575

Function

Block

&

Index

예제 10너0, 예제 10-11, 예저I 10-14, 예제 10甘16

예제 j아21, 예제 ]0-22, 예저Ii아23, 예제 12丑

예저1 伶너8, 예제 ]0-21, 예제 ]0-22, 예저Ii아23

예저112-3, 예제 12-4, 예저112巧

예제 9너, 예제 아5, 예제 9-毛

step

예제 乎］0, 예제 9-13, 예제 9너4
Step뷸록

예저116너, 예제 化田, 예제 佑닉, 예저116규

stepfun

예저1 10-4, 예제 10-5. 예저110七 예저110-7
예저10너0, 예제 ]0너1, 예저110너5
예제 +3, 예제 9巧，예제 9十，예저i10-4

sub히ot

예제 15-4

To F扼 블록
To Workspace 블록

예저113-4, 예제 17-2

Transfer Fcn 블록

예저Ii아j, 예제 ]6巧
예제 ]7닉, 예제 17巧
예제 乎23

trapz
Trigonometric Funct幻n 블록

예제 19-3, 예저119巧

예제 10田, 예저Ii아7, 예저Ii아8, 예제 ]0四
예제 ]0小］0, 예제 好너］, （계저110中］2, 예제 10-13
예저110-14, 예제 ]0-15, 예제 10너7, 예제 10-18

11
Uniform Random Number블록

예저119너, 예제 19-6

예제］아21, 예저110-23, 예제 12닉, 예제 12田
예저112田, 예저i12너0. 예제 12너2
예저112-13, 예저112너4, 예저112-15
예제 于4, 예제 9田, 예제 10너9, 예제 10-껌

subs

예저1 ]]+ , 예저111-10, 예저111-14
예저1 作-15, 예제 11-16, 예저｝11-32

m
V이tage Measurement블록

예제 20너

V이tage Sensor블록

예제 20田

Subtract 블록

예제14너

m

surf

예제 4十

waterfall

예제 十7

sum

예저110너6, 예저I 12-3, （계저112巧

while

예제 5巧

예저113너

Sum 블록
syms

예제 8너2. 0似II 아3, 예제 아4, 예저110너9
예제 10-21, 예제 11円, 예제 11너0, 예저Ill-li

예제 8너3, 예제 +15, 예제 8-16, 예제 9너
예제 아3, 예제 9巧, 예졔 9十, 예제 9-13

예저Ill叫16, 예제 j］尸27, 예제 ]］尸28, 예제 11-29

예제 9너6, 예제 +18, 예제 ]2十

예저111-30, 예저111-31, 예저111-32

예제 ]2-7, 예저112너3, 예저112너4

sym2p이y
symsum

예제 于］5

m
넌ab이

11

예제 8너3, 예제 8寸］5, 예제 8-16, 예제 9너
예제 +19, 예제 10너, 예제 ]0모, 예저110-3

taylor
text
if

예제 아13, 예제 8너2

예저Ii아4, 예저110巧, 예저110너3, 예제 10-14

예제 4-2

예제 j아］5, 예제 ]0너6, 예저110너7, 예제 好-19

예제 아5, 예제 9너0, 예제 9-11

예저110-21, 예제 j아22, 예제 j于23. 예제 12丑

예제 乎14, 예제 아］9

예저｛12田, 예제 12-4, 예제 12巧

예제 +8, 예제 乎11

tf2ss

예제 9-너, 예제 +3, 예제 9巧, 예제 9十

4

예제 9너3, 예제 9너／1, 예제 9너6, 예제 9너8

zeros

예제 于20. 예제 好너, 예저110丑, 예제 10-3

Zero-Order H이d 블록

예제 ]9닉

zplane

예저Ii아20

예제 j아4, 예제 ]0巧, 예저1 伶너2, 예제 10너4
예저110-15, 예제 10中］6, 예제 ]0-17, 예저110너9

576

川abel

예제 11-12, 예저1 쳐너3, 예저111-14, 예제 ]1-15

예제 6巧

title

m

함수／명령어／블록 찾아보기

예제 +7, 예저i12田, 예제 ]2너3, 예제 12너4

MATLAB & Simulink

한 권으로 제대로 배우자！
MATLAB과 Sirn小nk는 공학 문제를 쉽고 빠르계 해결할 수 있어
전기／전자 공학도들어꺼 꼭 필요한 프로그램이다．
하지만 아무리 좋은 프로그램이라도 단지 도구일 뿐이며
각각의 기능을 언제, 어떻게 사용할지 아는 것이 핵심이다．
이 책은 MATLAB의 기본 기능부터 핵심 기능까지
공학도에게 꼭 필요한 내용을 설명한 후 이를 전공 예제에 차근차근 적용해 본다．
또한 Simulink까지 범위를 확장하여 주요 블록들의 기능을 소개한 후
이를 다시 전공 예제어］ 접목하여 설계해 본다．
전공 예제를 해결하는 도구로써 MATLAB과 Simulink 활용법을 익히는 것，
이것이 바로 프로그램을 제대로 배우는 확실한 방법이다．

PART 01

PART 02

PART 03

PART 04

MATLAB
기본 기능 익히기

MATLAB
핵심 기능 익히기

MATLAB
활용하기

Simulink
설계하'I

MAT匕AB을
시작하며

가장 많이 사용하는
중요한 핵심 기능만

이것만은 꼭！

쏙쏵

MAT나＼B으로

시뮬링크로

주저뻗 대표 예제
해결하기！

주저뻘 대표 예제

· 배열과 변수
· 그래프그리기

· 수치해석
· 제어

· 미분방정식

· 프로그래밍

· 신호 및 시스템

· 심볼릭 툴박스

· 전자:7확

· 제어
· 신호 및 시스템

· 파일 불러오7! / 내보내기

·통신

· 벡터

설계하기！

· 삼각함수

·통신
·회로

기술 / 공학

111I 11H li ii
93560

9 79 56 644828
ISBN 979-11-5664-482-8 정가29,000원

