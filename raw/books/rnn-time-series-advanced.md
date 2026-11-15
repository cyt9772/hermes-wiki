---
source_url: "/run/media/yutae/Data/RNN과 시계열처리 심화.pdf"
ingested: 2026-11-15
sha256: 8d870dbb4c18a252f77eddbfd285a24b2708550697547ca629764dc90e917d89
type: raw-source
method: ocr
---

# RNN과 시계열처리 심화 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/RNN과 시계열처리 심화.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** tesseract 5.5.3 (kor+eng, 300dpi)로 OCR
> **쪽수:** 282쪽 | **추출 텍스트:** 604 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/rnn-time-series-advanced.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** RNN과 시계열처리 심화
- **Pages (PDF):** 282
- **Source:** RNN과 시계열처리 심화.pdf
- **Ingested:** 2026-11-15

## Extracted text (all 282 pages)



===== PAGE 1 =====
사외반출가능

ｌ 2
실무역량

RNNat 시계열처리 심화

SAMSUNG


===== PAGE 2 =====
RNNGt 시계열처리 심화                  [제 45 판

[주]한국에이아이연구소 대표이사 홍근선 저


===== PAGE 3 =====


===== PAGE 4 =====
저자 및 강사

홍 24 (gshong@ai-camp.kr)

ㆍ전자계산기 기술사
ㆍ웹게이트(주) 대표이사, 연구소장
ㆍ남서울대학교 전산과 교수

ㆍ시기술 관련 자문 및 특강

-                                       고

path 허시 .
Code ngert ord mA           oem By,
reek (pe)

나우 가  (0)            Cot)
이직믹낮 ie ae  진리.

pert: 0       ae NA, 15
‥ vleva¥@ Codekpert: MF .          4

pre ng        te 4
e200 Hal HF

org 049 .

*식융까우보  cole eer

@ 본 EMS 저작권은 SBRAISTA 및 저자가 보유하고 있음
© 저작권자의 허가 없이 무단으로 전재, 복제, LA, 디지털화 하는 것을 금합니다.
@ 교재 구입 및 출강 문의 : 070-8740-2124 (=) ae



===== PAGE 5 =====


===== PAGE 6 =====
자레

1부. Deep Learning 개념 정리
1.1 Deep Learning 개요

1.2 Keras Model 설계 workflow
1.3 Keras.layers API

2. Recurrent Neural Network

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char—RNN)
2.5 RNN Model Design (MNIST—RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

a
fo]

*K Ayre Qa
bel 498 7%

o>.

3.1 Time Series 개요

3.2 Time Series Analysis

3.3 Time Series Generation : WaveNet

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.0 Time Series Classification : CTC

4부.
4.1 Word Embedding
4.2 Attention Mechanism
4.3 Self-Attention

4.4 Transformer
4.5 GPT: Generative Pre-trained Transformer

글
=
cD
63
cD
그
cD
60
geo
aged
63
=a]
=

>
pay
purge
4)
=
=
=)
—
CO
©
”
14°)
은
즐
©
a
으


===== PAGE 7 =====


===== PAGE 8 =====
1부. Deep Learning 개념 정리


===== PAGE 9 =====


===== PAGE 10 =====
=.  Deep Learning 개념 념 정리                             1.1 Deep Learning 개요

Chapter 1. Deep Learning 개념 정리
( 핵심 개념 및 용어 정리 )

1.1 Deep Learning 개요
1.2 Keras Model 설계 workflow

1.3 Keras.layers API

% 인공지능 Artificial Intelligence
8 지 식(정적)
@ 어떤 대상에 대하여 알게 된 인식이나 이해
어떤 것에 대한 인식,이해
a 지 능(동적
* 어떤 것에 대한 올바른 의미나 사실을 파악하고 대응하는 능력
D> AAS 알아내고 (학습)상황에 대응하는(추론) 능력
8 지 성(목적/목표지향)
© ASS 자신의 삶에 적용시키고 활용하는 것
지능을 활용하는 성향/성질
8 인공지능 : 기계적으로 지식을 알아내고, 대응히
* 지식의 획득(학습) ㅎ 상황에 적용(추론)
(현재의 핵심은 지능의 아기사에트 미래에는?)
심의 지성:  동일한 지능수준에서.           를 얻을 수 있을

fir
olr
J

SAP DEEP LEAR!

-9- 무단 전재, 복제, eal, 디지털화 금지



===== PAGE 11 =====
1부. Deep Learning 개념 정리                               1.1 Deep Learning 개요

2 Machine Learning vs. Deep Learning(Layered Learning)

8 기계학습 Machine Learning : 데이터로 부터 스스로 학습          (    alk  (en nore
© 데이터에 내재된 패턴, 규칙 등에서               % deep  oye

수치형 특징 : 밝기, 온도, 구매량,…

범주형 특징 : 색, 제품의 종류, 고객의 성별,…

추상적(개념적) 특징 : 예술작품, 감정, 사상, 개념화된 속성,…

특징을 구분하고 기억하는 것.

해
jo @
+p hp eee ©

때

4o ilo

»2 de

00 3

Jct

al>

에

rir

N

=

jn 2

oM ry
모
으
cL
Jo
of
NJ
nu
에
의
dim
on
ilo
we
rir
~~

들의 조합으로 고차원의 특징을 찾는 것 : Layered Learning( = Deep Learning)

| |
>오
으
din
ox
ro
AJ
a
dim
om
rlo
mc
r=
ro
NJ
=

@  이미케키 색상, 텍스처, 모양 등
추세, 주기성, 변곡점 등
© 통계적 특징
@ 이미지의 밝기, 대비, 색조 등
@ 시계열의 분산, 자기상관성, OS (skewness), 첨도((41【0515)등

—— ee

% 세상은 복잡 계, 복잡 계를 해석하는    새로운 기술의 등장
m 대표적인 복잡 계 : 영상인식, 음성인식, .….
* Deep Neural Network : 인공신경망 계층화에 성공
＊* 영상인식 분야에서 혁신적 성과
> 10만장의 사진을 1000종류로 분류하기
@ MLP(shallow net) > Deep NN

Revolution of Depth

“152 layers

22 layers |  19 layers :
홈 G7     7.2

3.57

HLSVRC'IS ILSVRC'14 ss ILSVRC'14— ss ELSVRC'13) «CO LSVRC'12)ILSVRC'1i—ILSVRC'10
ResNet GoogleNet  VGG      AlexNet

i          ;                                   imageNet Classification top-5 error (%)
@한국시연구소 홍근선                      -10- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 12 =====
1부.

Deep Learning 개념 정리

1.1 Deep Learning 개요

|

a 인

뻐
인공신

® Neural node = Regression model
ㅎ Linear Regression : Linear activation

® Logistic Regression: Logistic (Sigmoid) activation

@Ot(ANN: Artificial Neural Network)

@ Nonlinear Regression : nonlinear activation

@ Deep Neural Network
® Linear regression nodeO
@ C2Fst activation functions 결합하고
@ 동일한 2749] regression node
@ Layer2| 계층화를 이루는 구조

output layer

input layer

hidden layer 1 hidden layer 2

들을 laer& 구성하고

|

0

axon irom a neuron ~

wo
synapse
~ Wor

인소 기
out tput axon

activation
function

자동으로 학습하기 : Training, 기보
- Kernel method, SVM (‘90 ~ )

- Decision tree, Random Forest (‘00 ~ )
- Gradient booting machine (‘14 ~ )

‘Deep Learning, 2

더 복잡한 것도 학습하기
- Deep, hierarchical layering

Reinforcement Learning

+ , Expert system(

: Layered learning

- Backpropagation, ReLU, Drop-out
- CNN, RNN, GAN, GNN, Transformer,

Deep Learning = Deep Neural Network

Meet

= 7

ㅎㅇ

009 >

각아테 Srhgcey

백치.

Gein 8014 Newel Net.

> 재그 Be

“RR DEEP LEARNING |

-11-

무단 전

ㄴㄴ

1재, 복제, 2

24, 디지털화 금지


===== PAGE 13 =====
1.1 Deep Learning 개요

14, Deep Learning 개념 정리

% Artificial Intelligent 분류(1)

io

레이블이 있는 데이터     1 | (       레이블이 없는 데이터       ) |      HBAAAHOR HG)
1 | |   stole 공통 72/84 ce | :의사결정을 위한 최적 행동 습득 ：

 ：학습결과로 입력데이터 예측
—                                                                                                                                                                                                            agent                                                            environment
-               trom state & take ection &

|
스팸메일분류 | 주가예측 | | ㅣ seul ㅣ ㅣ 데이터생성

pet 제제까시고 태사 wanes

 데이터로부터 레이블 정보를 생성       |

i:   =       2           .
데이터들의 공통 구조/특징 학습  4au yrrjot 3 사요

| - 레이블 비용 절감
| > 일반화 성능 향상

| - 새로운 데이터 적용 용이

' - 모델 성능 예측 어려움 발생

： 정보가 부족환레이블 사용

_ 보다 높은,추상화 문제해결 7
제

ie eee eer rere

oir

n JOR DEEP LEARNING |

XX Artificial Intelligent 분류(2)

해  브
a 기능적 분류

® Perceptual(ajZt) Al: 시각, 청각,
@ 컴퓨터 비전, 음성 인식 등

® Cognitive(2l2]) Al: 사고, 히
@ 기계학습, 자연어 처리 등

$ alee Al: 인간의 HES 모방하여 물리적 또는 디지털 환경에서 작업을 수행

a            자율주행, AgentGPT 등

8 접근방식에 따른 분류

@ Discriminative(ZtS) Al: 주로 지도학습
@ 입력 데이터 내에서 서로 다른 클래스를 구분하는 결정 경계를 학습
@ 입력 데이터 분포를 modelingsh= 대신 레이블의 분포를 포집 하는데 집중
® Generative(44) Al: 주로 비지도학습(0: 자기지도학습)
 입력 데이터의 분포를 심층적으로 분석
 입력 데이터와 레이블의 결합 확률 분포를 학습 이해함
& 학습 데이터와 매우 유사한 새로운 HSS 생성할 수 VES
* 데이터 내의 복잡한 패턴과 구조를 들여다볼 수 있는 HS 제공
/* 창의적인 데이터 합성,생성 및 증강이 가능함

pie ome 33330

4s                   -12- Sot 전재, 복제, all, 디지털화 금지



===== PAGE 14 =====
1부. Deep Learning 개념 정리

1.1 Deep Learning 개요

iE

m@ Neural Network= Regression model(1)

® Regression(S|7) : 어떤 입력 데이터에 대해, 출력에 AHS 주는 조건을 고려한
@ y= (6222.26 i Bi Bo Bo te, (56) : 회권모델, 입력(>)에 대한 영향(0)
* 선형 S17 Linear regression : 통계적으로 [의 SHS 분석할 때 주로 사용(모델 해석이 중심)

@ 회귀계수(8)의 선형 결합(곰의 함)으로 표현되는 모델

@ y= Bo + Bix + Box* + 63” + pol 대해서 선형 결합 이면서 (×에 대해서는 비선형)
= Bo + Bix, + 0232 + 03 선형결합유로 표현 가능 > feature 60910661100으로 전처리

@ y= Box*t = log(y) = log(Box*1) = 10000 + 0고0800

=y' = Bo + Byx’ : 엄밀하게 linearizable regression modelO|2} 함(변환을 통해 선형화 가능한 경우)

* 비선형 회귀 Nonlinear regression : 딜러닝은 대부분 비선형 회귀 사용
—eVwe—wowoa“n—esrseaeeerr’

@ y= * po] 선형결합으로 표현되지 않는 모델

B2t+x
© 유연, 목장한 데이터 모델링 가능 : 예측에 주로 사용(해석은 어려움

@ SHet(univariate), 다변량((04104801016) regression        ]
@ 종속변수(:)의 수에 따른 분류                      이 이.
/ univariate / multivariate regression                               : :

@ 독립 변수(/의 수에 따른 분류                   Spr

/ Simple regression / multiple regression                             ㅣ      i

—_

Linear / Nonlinear regression 비교 ]
Fel      $

y= Box’! = 2205

Test Passed?

1.00.        © @ on                    =                           6!
i   "  oe finear                    fra         A  )     i+e ~Ka~tg}
0.75                             가| -slacal constant            /                        :

@ Neural Network2 Regression model(2)

® Regression : 어떤 입력 데이터에 대해, 출력에 SHS 주는 조건을 고려한 평균값
* Linear regression / Nonlinear regression                           | rant  ewe valve |

 최적 value 추정, 모델이 선형결할이면 |068「, OFL|H nonlinear regression

@ Logistic regression : Classification regression2| 확장

@ logistic function4 So #50) 사용 (성장모델 SME 회귀로 사용하는 경우도 많음)

@ Logistic: SH, 병참 > 적절한 것을 적절한 곳에 제공하는…                 바가

ㅎ Logistic function : 존재할 확률(0~1)로 HSt(logit 역변환)

 물리적으로 볼 때 특정 값을 중심으로 Sete 특성을 Wig                 > logit: 090(곰) =

/ Standard logistic sigmoid function vs. sigmoid function

logistic(sigmoid):  ire) = 확률:

inp

le  Logistic. 2  sym ddet  Emre
[ Logistic regression ]              [ Linear regression ]           [ Logistic / Sigmoid function ]
;                                                                      E

14         26

fg     더 나       L  pc |  i  i  i  i
기저                      ~6 -4 ~2    6    2    4    6
;

RID 이. 의. on Standard ogistic sqmond tunctinie L~ Ike Ize G 어

[ Odds / Logit function ]
eS
ye
2        \
Xo
cg                       /

-13- 무단 전재, 복제,

24, 디지털화 금지


===== PAGE 15 =====
1.1 Deep Learning 개요

144, Deep Learning 개념 정리  리

s&s
:종속변수

@ Logistic regression        60가  414 (categorical), Classification
* 출력 범주의 + : 0/S(Binomial), Cfét(Multinomial) logistic regression
@ 범주의 수가 2(이항) or 3이상(다항), SHO] 범주의 확률값(5410 to 1)

® 이항 로지스틱 회귀 (Binomial logistic regression) : 두 범주 분

at =
@ 3 logistic function(sigmoid func.) S 적용
 0개의 실수정보 ×를 1개의 확률 값에 mapping 하는 함수를 찾는 것

리 > 하나의 출력

Age

Height             f

Weight | ---42.___.;   Clean(0)          f:R¢—— R154  |
Blood pressure                        Cancer(1)

£9        wo
Input features                                    — i                         axon from @ neuron ~
d                            ye R 7O0~1
xeéER

® Linear regression + logistic function                                               020  )
Ze
i

¥1 = OCD + WyXy + WoX2 + …+ WaXq)
output axon
= 6 Qi wixi + 0)                                                                       activation
function
a: sigmoid func. = = , nonlinear func.
se eu ene ee                    —      —
.                                                                                              CERNING”

@ Multinomial Logistic Regression(Chet 로지스틱 회귀) (= Multi class logistic regression)
@ Chet 로지스틱 회귀를 사용한 Multi class Classification
®@ Logistic regression2| 4S 여러 개로 확장

@ 다수 출력을 확률로 변환 필요                   |
> 0개의 실수정보 xB 개의 확률 값에 mapping SHe 함수를 찾는 것

az A

Age                                                     Clean
Height                     f                         Cancer
Weight ss es See 고                               >                   Cold

Blood pressure                       High blood pressure

Outputs
ye  RY sumtol

input features
x €R4

ㆍ pd     >
f:R        R™, sumto1

/@ Sum 10 1 : 각 값이 확률이므로 합하면 1

0

@한국시연구소 홍근선         -14- 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 16 =====
1부. Deep Learning 개념 정리                               1.1 Deep Learning 개요

® Multi class logistic regression (2)
$ 0개의 실수정보 ×를 개의 확률(6410 to 1)로 mapping 하는 함수를 찾는 것

전                      1
2                      22
~ f                         . 20            7272
-->    =       f:         >R  7 52002 701
70                      Ym                                                —        [ Single neuron ]

pmeseeemieemamens |
axon from a neuron "~
. 40000

 함수 를 matixe 표현하면, (선형결합으로 표현하면)

=      m
[4%1%2 ~ 0 ]         +[b]=[91¥2 … Ym], sumto1
outpul axon

«| a                           activation
d    Ww                                 로         .             10020            function

w 6 Raxm

f:Y=o(X -W+b),  o = softmax(sum to 1 변환함수) |

00
® 112101009의 목표 (Y = (×)인, +( ) 만들기 )

최적의 parameter W , 8 를 찾는 것(주어진 031356[에서)
® Softmax activation: cell 밖에 있음, layer= 동작함
/* 구현상, 헤내부에 activationO| $47 (linear activation)
/* 다음 !376「에 activation 함수를 명시함

® Softmax Activation : n-class 분류 모델 마지막 layerOl] 적용
® Softmax activation : K-dimension z 값을
0~1사이 값(5417 to 1)으로 변환, logistic func.(sigmoid func.)S n-class=@ 일반화

226             j                                                         1
= 가 0      707) = 1...                        sigmoid = ㅜㅡ~

& Classifications 위해 모델이 추정한 결과값(!00|[표현)을 확률로 변환

roe
Softmax                                    Oe ~~  = 6
371.0-007=군= 702 >                  (00
|    0.1 으                   Pia <,    6
Scores(logit) > Probabilities(sum to 1)        ae  IS
에제
Target       :[0100],K=4  one-hotcoding(3t#Z)

을   고   =        Softm    Lexp(3) exp(—1) exp(2) exp(10)]
Estimation : [3 —1 210]        jax,  ra ee > [0.009 0.0001 0.0009 0.99]

Scores(logit)                                                                   probabilities
/ Logistic regression 1001【역변환, 확를로 변환하여 분류 하는 것이므로                          수
- loss function? & Cross entropyS 사용하는 것이 적합 (두 확률값 간의 무질서도, 정보량)  eed  uty ,
/@ Cross entropy : 두 확률 분포 6와 q2| 211 entropy= 표현
- 두 확률변수의 유사도를 측정하는 함수로 사용 가능, 2(2,0) = —E,, [log ail

@한국시연구소 홍근선                - 15 - 무단 전재, 복제, S4ll, 디지털화 금지


===== PAGE 17 =====
he - [2

1부. Deep Learning 개념 정리                        th.  1.1 Deep Learning 712

3% Cross Entropy

ALE
8 Entropy: 정보량(정보의 기대값), 무질서도, 불확실성
® 확률이 적은 사건(0)의 발생 정보는 정보량이 많은 것 = 정보량은 발생 확률과 반비례 (1/p)
애마 cae a cr a
* 독립사건의 발생확률은 곱, 두 사건의 정보량은 합이 LOSS > log(1/p)

© 정보량 : 발생 가능한 모든 사건의 평균을 취하자 > peg?) =[-Yipdog(d = 0@0)|

정보량 = 5 = log (5) = Lipilog) ㅋ-2.2.000000 = Hp) = Entorpy,

i     RDO aOOEHOU ISOS"
m KL divergence: 정보 손실 량의 기대값 (7,를 전송하고, 0,를 받았을 때, 손실을 추정)
© 확률분포7,와 0,사이의 정보량의 차이(정보의 손실량)를 AHA, 4,기대값을 Dy Me

시= —log(qi) +ㅜ10902 = 80.) = 히2141=1- 22.009(00 + Yipilog@d = Dr (lla) }
® Variational Inference        We YAU - AGI MILE   }

@ PES 수 없는 분포, 0는 알고 있는 분포 : 알고 있는 0로 모르는 [를 설명한다(『 분포 추정)

mS Cs)

0의 245 수정하면서 2《,최소가 되게 하는 것
& Cross Entropy : 0(정답),0(예측값)간의 무질서도(확률분포 차이의 기대값)
@ Dg AA 뒷 항은 0와 무관하므로 앞 항만 최소화 시키면 됨
® Qf & :(CrossEntropy(CE) = — Yipilog(q,)| > 낮추면 두 확률분포의 유사성이 높은 것
anew OOO OOOOOOOw“™™—=—™"'

u

DEEP LEARN

|

= Machine learning 이란

® 7HISZt(hypothesis space) 내에서 eyo, ve 우 있는 자요 wizee\ Set.
@ 좋은 HH (representations)S, 7}#HS(transformations)S 통해
we @ 자동으로 검색하는 과정

DHS} 쉬운 새로운 좌표 계로 변환 > 새로운 data 표현 > 특징을 이해

eae                                  2: Coordinate change                        3: Better representation
}
e ㅎㅎ
y
일                                                                                                              e @
e®                                                                                                                     e
% S                                                                                      o Flets
°, #e                                                                              06.
ㅇ                                                                                                                           x
Ce                                                                            0        명    e
본                                                                                                         @
x
 가설공간 Hypothesis space : model0| 제공하는 4205[0107의 집합
ould                                                                                                                                        이레"

@한국시연구소 홍근선                   -16- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 18 =====
|요

Input X
:        !

1)

1부. Deep Learning 개념 정리                              1.1 Deep Learning 7
_1.1 Deep Learning 개요                                                           |
K ASA 표현 학습
= Layered(hierarchical) representations learning (= Deep Learning)
©@ Layer(filter/transform)S 통과하며, 정제된 정보(표현)로 변환
© 출력의 표현을 학습하는 다단계 처리 방식
Layer 1                     Layer 2                    Layer 3
representations      representations      representations
i                           Layer 4
representations
(final output)
Original     a                                | '               | |        이  a
input                                                                    2 =
4  '
— pa
6  0
=
HNIST = LI                                ir               | |        9 0
Layer 1                                                       Layer 3                      Layer 4
33                                                                                                                                               SOx DEEP LEARNING”
_ 1,1 Deep Learning 개요                     ve
3% Deep Neural Network2| Training
|         - Layer : weightsS parameter= 갖는 『( )
- Y’ = F(X,W)
- Cs = Y Lo(Y’-Y)

Layer
(data transformation)

:

Layer
(data transformation)

I
y
Predictions
y

Weights     자
A

-W =W- Op(Cs)

-- W update (= backpropagation)
Y Input, Data, Sample , X
< Weight 가중치, parameter, W

Y Loss function E28, Loss score ANZ

Y Cost function 비용함수
Y Object function 목적함수
Y Prediction 예측값, Y’ (> Inference 추론)

True targets
4

Y Target S32f, True targets, Y

Weight
update
™
Back ee
34               .                                ai                       ’           SC DEEP LEARNING”
@한국저연구소 홍근선                       -17- 무단 전재, 복제, Ball, 디지털화 금지


===== PAGE 19 =====
1부. Deep Learning 개념 정리

1.1 Deep Learning 개요

본

XK 최적화 알고리즘 Optimization Algorithm

@ Momentum : 기울기에 속도 개념을 추가

560
Momentum
NAG
Adagrad
~~ Adadelta
~ Rmsprop

Training data2| 평가(1055)에 따라 7-2] (parameters)S 계속 수정하여,
Loss func.2| 값을 최소화하는 알고리즘 > 학습 속도와 성능향상을 위해 하이퍼 파라메터 조정 필요
@ SGD(Stochastic Gradient Descent ) : 82[대단위로 기울기를 계산하여 \ 수정

@ NAG(Nestrov accelerated gradient) : momentum 적용 후 Gradient 적용
@ Adagrad: W 변화 량에 따라 가중치 부여, 변화 량이 AS PE 좀더 변화 S 증가
@ Adadelta, RMSProp, Adam : Adagrad 단점 개선

SGD
Momentum
NAG
Adagrad
Adadelta
Rmsprop

AS  =—=—[L. 즈
estes 방해하는 주 요인

Backpropagation

ft nd t
@ Vanishing Problem                                               =
Optimization such as
@ Backpropagation of error                                                                             Paes
®@ Error=costfunc(z,y)=5 iol we We oe                  [—cabeataon ot
@w =w- ()                                                  /_ ew
ow                                                                        a       1
@ 57} 작아지면?                                                                  Te OR SO) = Tea
' 변화량이 작아짐                                  ~
ig ad 변화량  |작  |짐                                    Net input             Activation          —
> 학습 둔화 or 멈춤                                              function                function
@ SA} 작아지는 원인                                                     bo                              1
08
1) Activation func.2|                                                    “4                          l+e7        a
saturation S4Oz 값이 입력 되는 경우                              원
2) \값이 작아서 AAD 되는 6 가 너무 작은 경우            nt X    pi

(가 너무 커지면 어떻게 되는가?)             0062

~               TE DESETEARWNE”
무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 20 =====
1부.  Deep Learning 개념 정리                             1.1 Deep Learning 개요

a |

x 학습률 Learning rate : 학습 속도와 성능에 큰 영향, 학습 경로와 local minima 영향
1065)                                             100A             [ 너무 2 학습률의 영향 ]

~. Avoiding
“Minima

iow learning rate                                                                                Smoother

high learning rate

good learning rate

epoch

두 개의 파라메터에서 보이는 Loss2| 복잡도 ]

초기값에 따라 다른 결과                                       -수많은 로컬 미니마

XX Overfitting : Training Data] 최적화 되어 성능이 저하되는 문제
® 데이터의 일반화된 특성을 학습하는 단계를 Lt, Training 0218에 특화됨
® 모든 모델의 Se overfittingS 향해 학습함

egression:                                  | |
Ri g                                                   ; | vA      Und
Es       [로
낳      i 4
1
a              7      8              원 !     é             gt
predictor too inflexible:                                                          predictor too flexible:
cannot capture pattern                                         fits noise in the data
Classification:

@한국시연구소 홍근선          - 19 - 무단 전재, 복제, BS), 디지털화 금지



===== PAGE 21 =====
1.1 Deep Learning 개요
7

144. Deep Learning 개념 정리
[                  g

mw 모델의 복잡도와 Overfitting2| 관계
© 모델 복잡도와 53010165의 관계(상대적으로)에 따라 0601[400의 민감도가 결정 됨

out-of-sample error

제   out-of-sample  error| Test error |

|
| bad | Generalization performance |
i

error

error

in-sample error

VC dimension, dyc                   VC dimension, dvc:

들  Overfitting 해결방법                                  [Complexity of the algorithm |
1. Data 늘리기 : more data, Augmentation, create fake data
2. 모델 capacity 최적화 하기: Architecture tuning(Network-reduction), Early stopping,
Weight-decay(L1,L2 regularization ), Learning rate decay, Feature Selection
(input features 제한하여, 모델을 더 작게 만들기 : Variance Thresholds, Correlation Thresholds,
Genetic Algorithms, Stepwise Search )
3. 다수 SAS Ensemble 하기 : Ye] SAS 만들어 개별 학습 필요

번 —
4. Layer 추가 하기 : Dropout layer, Normalization layer, Noise i
—. Bee    88360        ee         9           레지

EEE TET EOE

jection layer 추가
“Sie DEEP LEARNING ©

a 몇 가지 용어 정리
® Data / Data set
@ Input data, Sample, Target data, Label             .          ynmes
oy             0”           <, rel. \0 서
@ Training data, Validation data, Test data               686  ote.
@ Epoch / Batch size / Iteration
@ 1Epoch :2£ training datad 학습에 한번 사용                                   :
~ 을 얼지 de. Hn 이.   / 는. ©
® 1 Iteration : training dataS 학습에 적용, 한번의 전,후방학습이 진행 perv  /    OKs
® Batch size : iterationO] 사용된 subset2| 크기
> 1 epoch= batch size® 나뉘어 여러 번의 jterationl & 시행 됨 > Mini-Batch Gradient
@ Objective function > Cost function > Loss function
@ Objective function : 학습을 통해 최적화 대상이 되는 함수
/* Maximum Likelihood ㄷ51078101같이 학습을 통해 HSS 최대화하려는 1400101은
Objective function®|A], Cost, Loss function 아님
® Cost function: 학습을 통해 최소화 하려는 함수
@ Input 0212에 대한 모델 출력에 대한 오차를 계산하는 함수
/*＊ (65최소가 성능을 보장하지 않음 : cost function #717; 중요

@ Loss function : 모델의 출력과 목표값 사이의 오차를 계산하는 함수

/* cost functionS 구성하는 94056 , Cost = 10551 + 10552 +...
“@ loss func. = cost func. 인경 우가 많아서 일반적으로 Ss st

~



===== PAGE 22 =====
1부. Deep Learning 개념 정리                     1.2 Keras Model 설계 workflow

Chapter 1. Deep Learning 개념 정리

( 핵심 개념 및 용어 정리 )

1.1 Deep Learning 개요
1.2 Keras Model 설계 workflow

1.3 Keras.layers API

3 Model 설계 workflow
a 1. Dataset 준비
® Dataset 정비, 구성 또는 생성
ㅋ8 2. Model 정의
* Dataset] 적합한 model 구상, 설계
© Sequential, Functional, Subclass 방식
= 3. Model 컴파일 : model.compileQ)
® Training 과정에 필요한 환경 설정:
@ optimizer, loss, matric 등 설정
= 4, Model 학습 : model.fitQ
® Model Training 진행
® Validation option 통한 진행 상황 monitoring
@ 5. Evaluation : model.evaluation0)
© 학습 결과에 대한 평가 > 결과에 따라 위의 과정 반복
a 6. Model 적용/활용 : model.predict()



===== PAGE 23 =====
1부. Deep Learning 개념 정리                       1.2 Keras Model 설계 workflow

% 첫 모델 만들기

i import keras
2 # 데이터 준비
3 (x_train, y_train), (x_test, 7 test) =k
4 모델 49)
5 ## Sequential model 사용
6 model = keras.models.Sequential()
7  ## 레이어 추가
8 model.add(keras.layers.Flatten(input_shape=(28,28)))
9 model.add(keras.layers.Dense(units=1@, activation='softmax'))
10 # 학습과정 설정
1    model. compile (loss= ‘sparse categorical _crossentropy', ©
12                        optimizer="adam', metrics=['acc'])
13 # SS
14 model.fit{x train, y train, epochs=3, batch_size=128)
15 # 시험
16 classes = model.predict(x test)
17 p(classes)

Epoch 1/3
469/469                      is 2ms/step - acc: 8.6976 - loss: 27.0829
Epoch 2/3
469/469                15 ims/step - acc: @.8745 - loss: 5.2819
Epoch 3/3

469/469                      15 ims/step - acc: @.8842 - loss: 4.0863

3% 2. Model Define : 세가지 방법

# 1. Sequential model
¢@ Single/ Sequential data flows
® 2 HOHE 하나의 입,출력을 가짐
® 레이어를 쌓는 구조
@ 2. Functional API
© 복잡한 모델 구조 설계
® Multi-input models                                    |          「
@ Multi-output models  Seqeeenet  |   |  Boles amie  |     [_Subelassing |
@ Shared layers (동일 레이어를 반복 호출)
@ Non-sequential data flows (e.g. skip connections)

@ 3. Subclassing API
@ 상속을 통해 MLSS model LE layer 생성

@한국시연구소 홍근선                      -22- 무단 전재, 복제, Wai], 디지털화 금지


===== PAGE 24 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

8 1. Sequential model
® SA;AOSe layerS 쌓는 방식 keras.models.Sequential( ) model.add()
® Data 입,출력이 하나인 단순 구조 모델에 사용

1 import keras

2 from keras import layers
3

4

7

6

7

8

9

11 _model.summary()

@ Keras.Input() 을 제거하고, 첫 layer2| 2l4+(argument) input_shape=() 로 정의할 AS

# 모델 정의 ; Input Layer 제거
2 model = keras.models.Sequential()                        때   '    sai
3 model.add(layers.Flatten{input_shape=(28,28))) | 첫 레이어에서 Input] 18
model.add(layers.Dense(64, activation="relu"))
model. add(keras.layers.Dense(units=10, activation='softmax‘))

Ao

om

@ 2. Functional API
® layer2| 입력, SHS 지정 : 어떤 layer SHS O/H layer 도 입력으로 받을 수 있음
® Inception 및 ResNet 같은 비 순차 네트워크 모델링에 적합
® 앞장의 네트워크를 변형하여 『40010021 ^미로 구현
@ 레이어의 그래프를 작성 : 레이어간 DataFlowS 정의
@ 모델 생성시에 Data 입,출력 관계를 알려 주면 Graph(DataFlow)S 따라 모델이 생성됨

# 1. DataFlow(Graph) S’2/

i
2 input_x = keras.Input(shape=(28,28))                ~ 224 Inpute Bo
3 x®@ = layers.Flatten()(input_x)          00         =
4 x1 = layers.Dense(32, activation="relu")(x@)
5 x2 = layers.Dense(32, activation="relu")(x@))
6 x3 = layers.concatenate([x1, x2])
< gutput_x = layers.Dense(18,activation="softmax")(x3) ©
8 #2. SH SIAEIA : input,outputO£ DataFlowS 주석
y
@ 레이어의 출력이 다른 레이어의 입력으로 연결 : Graphs(or DataFlows) of layers
영봉     Soa     eras           -        =       SOBER LEARNING”

@한국시연구소 S24                  -23- 무단 전재, 복제, Hall, 디지털화 금지


===== PAGE 25 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

& Model 구조 보기
*  Model.summary( )               그   오이 이시 이시이 시 ‘model.png', 51000 51120065=11[006,
@ 모델 구조를 테이블로 출력         12                                     show layer _activations=True)
@ layer! : type(name), output shape, #parameters, input layer 보여줌
@ keras.utils.plot_model( )
@ layer2| 입출력 shape 변화와 layer7! 텐서 SEBS 그래프로 출력

.         .            .                                                                                                         Plot_model vat_3       input: | [(None, 28, 281]
Model: “functional_53                                                  model summary              트    | mpurLayer | output: | (None, 28, 281]
Layer (type)           Output Shape          Param # | Connected to                                   u
"                                                                                                                               flatten_6 | input: | (None, 28, 28)
input_layer_3?            {     , 28, 28)                  |-                                                                None,
{inputlaver)}      tend

flatten 41 (Flatten) | (onc, 788)          @ | finput_layer_37/[6]..            =      —

dense_i0 | input: | (None, 784) | (dense 11 | inpur: | (None, 784) |

dense 106 (lense)     (ee, 32)          25,126 || flatten_4ife][e] || Dense [ relu | 0000 | (None, 32) | Dense | relu | ouput: | (None, 32) |
dense_1@7 (Sense)      (Hone, 22)           25,128 || flatten_41[9][@]

| concatenate | input: | {(None, 22), (None, 32)] |
concatenate_32          《    , §8)                   은 | dense 106[01[8],                | Concatenate | ‘output:       (None, 64)      |
(Concatenate)                                       dense_107[8][2]                                 |
06056 108 (06656)      (0066, 308)              356 | concatenate_32/¢]..                  i   rr)    —  (None, 64)
Total params: :      (198.79 KB)                                                      Dense | softmax | output: | (None, 10)
Trainable params: S€,29¢ (498.79 KB)

Non-trainable params: © (0.00 8)

# Function’? = Model 생성하기
® FunctionO| 2212 Return
@ SAS 다시 Training 하려면 모델이 다시 생성되어야 St
@ AMS SAS al 생성하여 학습하기 쉽게(1「210109 조건 변경 시)

i def create_model2():

2      #1. Data Flow 2S

3      input_x = keras.Input(shape=(28,28))

4      ×0 = layers.Flatten()(input_x)

5      x1 = layers.Dense(32, activation="relu”)(x@)

6      x2 = layers.Dense(32, activation="relu”)(x@)

고      x3 = layers.concatenate([x1, x2])

8      —— x = layers.Dense(ie, rained acing <a,
5      #2.          Ei’ : input, output C= DataFlowS #4
10      model = keras. Rodel Gnpute- input_x, outputs=output_x)
in
12

13 model2 = create_model2()

@한국시연구소 홍근선         -24- 무단 전재, 복제, al, 디지털화 금지



===== PAGE 26 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

|

m 3. Subclassing API
® ME layer / model 을 클래스로 정의 하여 사용, saveS 위한 처리 주의

i from keras.saving import 『06815ㄴ60 (60605 serializable

2 @register_keras serializable()       # keras formatO@ 저장시 Bo

3--class MyModel(keras Medel):

4     def init__(self, **kwargs):    # “kwargs: keras formatO@ 저장시 BO

5        super (MyModel, self). init __(**kwargs) # **kwargs: ‘'

6         self.flatten = layers.Flatten()

7         self.dl = layers.Dense(32, activation="relu")

8        self.d2 = layers.Dense(32, activation="relu")

9        self.d3 = layers.Dense(i@, activation="softmax")

10     def call(self, x):

14       | x@ = self.flatten(x)                             Plot_model

12       | x1 = self.d1(x@)

13       | x2 = self.d2(x)

14       | cl = layers.concatenate(/x1, x2?)               Input shape: (None, 28,28) | Output shape: (None, 10)
15       |_return self.d3(c1)
「  인스턴스 한다고 graph7} 완성되지 않음      Layer (type)              Output Shape         Param #

® Input data shape setting B2                flatten_5 (Flatten)       (Hone, 784)

1 model = MyModel()                         dense_5 (Dense)           《    5 32)            25,126
2 input_x = keras.Input(shape=(28,28))   dense_6 (Dense)        (Here, 32)

3 output_x = model(input_x)            dense 7 (Dense)        (tiene, 10)

4  model.summary()

Total params:        (198.79 KB)

Trainable params:     90 (198.79 KB)
® summary(), plot_model() API 부분 지원 non-trainable parans: 0 (6.00 8)

0)                                                             ‘Sie DEEP LEARNING

kflow

%€ 3. Model compile : compile method

model.compile(optimizer='rmsprop', loss=None, metrics=None,
loss _weights=None, weighted _metrics=None,.. )

® 내장된 optimizer, loss, metrics 함수들이 다양함
@ Optimizers

Adadelta: Adadelta algorithm.
Adagrad: Adagrad algorithm.
Adam:      Adam algorithm.
Adamax:    Adamax algorithm.                               '
Fir li         FTRL algorithm.                                   #2 metric 함수
Nadam:     NAdam algorithm.
RMSprop; RMSprop algorithm.
$GQ; Stochastic gradient descent.                 loss functions +
Accuracy
TopkCategoricalaccuracy: 상위( accuracy
binary_crossentropy                              AUC: AUC(Area under the curve)
categorical_crossentropy                        Precision
sparse_categorical_crossentropy                   Recall
mae: mean absolute error                         TruePositives
mse: mean squared error                        FalsePositives
msle: mean squared logarithmic error              PrecisionAtRecall
kid: Kullback-Leibler divergence                 MeanIoU{intercection over union )
ste: i ys en          rer        ee SE DEEP LEARNING

@한국시연구소 홍근선                      -25- 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 27 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

1

® Compile 인수, 함수의 UAHAS 설정하기

1 opt = keras.optimizers.Adam(learning_rate=@.@1)
loss_fn = keras. losses. SparseCategoricalCrossentropy()
metric fn = keras.metrics.Accuracy()

VE 8 9 Re

model.compile(loss=loss_ fn, optimizer=opt, metrics=[metric fn])
@ 사용자 1055 , metric 함수 만들어 사용하기

import tensorflow as tf

# loss BA BIB

Awe OR 3

4
5    return tf.math.reduce_mean(tf.square(y_true ~ y_pred))
6 # metric BP 아웅
7 def custom mean error(y_true, y_pred):

&   return tf.math.reduce_mean(y_true - y_pred)

3

16

model. compile(optimizer=keras.optimizers.Adam(),

a2                         loss=custom_mean_sguared_ error,
12                 metrics=["Accuracy',¢ustop_mean_errer])
13

14 eh dees 유양 AYES one-bot encoding
15 y_train_one_hot = tf.one_hot(y_train, depth=10)
16 model.fit(x_train, y_train_one_hot, batch_size=64, epochs=3)

Epoch 1/3
938/938 [                              ] - 6s 6ms/step - loss: 8.1148 - accuracy: @.8046 - custom_mean_error: 8.4781e-12
Epoch 2/3
938/938 [                              ] - 5s 5ms/step - loss: @.0714 - accuracy: 0.9000 - custom_mean_error: 1.3298e-11
Epoch 3/3

938/938 [                              ] - 5s Sms/step - loss: @.0646 - accuracy: 6.9146 - custom_mean_error: 4.7865e-12
asa ce Been nnn nE..KCqnJHMiiiiii    0          20000    주000000000
51      URC DEEP LEARNING

|

|

% 4. Model 학습 : fit / tain_on_batch method
= Fit method 기본 사용

1 #model.fit(x_ train, y_ train, epochs=3, batch_size=128)
2 history = model.fit(x_train, y_train, epochs=3, batch_size=128)

® 42 argument? 기본 값
model. fit(x=None, y=None, batch_size=None, epochs=1, verbose=1,

1
2    callbacks=None, validation_split=¢@.@, validation_data=None,
3      shuffle=True, initial_epoch=@, validation_freq=1,..)

# verbose=1: 학습 진행상태 표시, 0 = silent, 1 = progress bar, 2 = one line per epoch
@ callbacks=None: 학습 중 특정 지점에서 유틸리티 함수를 콜 백하도록 B+ list 제공
@ validation_split=0.0: 검증 데이터로 사용될 훈련 데이터의 비율
® validation_data=None : 각 epoch 끝에서 손실 및 메트릭 계산용 데이터(검증 데이터)
® shuffle=True: 각 000대시작 전에 학습 데이터를 섞음
@ initialepoch=0 : 이전의 학습 과정을 재개할 경우 사용
@ validation_freq=1: 검증하는 간격, 1 = 매 600대마다 검증
* Return : history object, Epoch 1055와 metric 값들이 dictionary 형태로 기록되어 있음

i history.history

{'loss': [4.613648414611816, @.7099044919013977, @.49114447832107544],
‘accuracy’: [0.7314000129699707, @.8331666588783264, @.8775500059127808],
‘mse’: [27.376232147216797, 27.3741397857666, 27.378881454467773]}

yd

@한국시연구소 홍근선                -26- 무단 전재, 복제, Sil, 디지털화 금지


===== PAGE 28 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

 BS 데이터 사용

i history = model. fit(x_train, y_train, epochs=3, batch_size=128, validation_data=(x_test, y_
oe ae aes oe Gh mee 매매 anos
Epoch 1
469                           - is 3ms/step - loss: @.2265 - accuracy: @.9382 - mse: 27.3866 - vai_ioss: 6.3159 - val_accuracy: @.9284 - val_mse: 27.3325
=e ee ee 을 를 을 a ae ee 보

- is 2ms/step - loss: @.21@3 - accuracy: @.9413 - mse: 27.5873 - val_loss: 6.2941 - val_accuracy: @.9338 - val_mse: 27.3330

36                          ] - ds ams/step - loss: 9.1897 - accuracy: @.9465 - mse: 27.3876 - val_ioss: 9.2671 - val_accuracy: @.9368 - val_mse: 27.3333

@ History 확인 : validation data 관련 값이 추가됨

i history. history|

{'loss': [@.2265392392873764, @.21034255623817444, @.1897350102663e4@2],
‘accuracy': [@.9381833@76477051, @.9412833452224731, @.9466333389282227],
‘mse’: [27.386621475219727, 27.38726043701172, 27.38761329650879],
‘val_loss': [@.31586676836013794, @.2940868139266968, @.2671375870704651],
'Val_accuracy’: [@.9283999800682e68, @.93379998287e9229, 0.93680000305175781,
'val_mse': [27.33248519897461, 27.333045959472656, 27.33333969116211]}

m train_on_batch method : 데이터 배치에서 한번 그라디언트 계산, 가중치 업데이트를 실행

for i in range(n epochs):
# prepare real samples
x_real, y_real = generate_real_samples(half_batch)
# prepare fake examples
x_fake, y_fake = generate_fake_samples(g_model, latent_dim, half_batch)
# update discriminator
d_model.train on batch(x_real, y_real)
d_model.train_on_batch(x_fake, y_fake)

라즈

※% 5. Model 평가 : evaluate method
a 기본 사용

1 model.evaluate(x=x_test, y=y_test)

313/313 [                      ] - 2s 5ms/step - loss: @.3616 - accuracy: @.91
[@.36155572533687483, 0.9169999957884656, 27.33106803894043]

@ #2 argument2| 기본값
® Batch_size=32
@ Verbose=1 : 학습 진행상태 표시, 0 = silent

# returen : Less + metrics

2 values = model.evaluate(x=x_test, y=y_test, batch_size=i¢24,verbose=1)
3 values
10/10 [s=sesssssessseeceseessesssssse] - 05 Sms/step - loss: 9.3616 - accuracy: @.9176 - mse: 27.3311

[@.3615557849407196, @.9169999957084656, 27.33195231689453]

| 은 # returen ; Loss + metrics
| 2 values = model.evaluate(x=x_test, y=y_test, batch_size=1024,verbose=@) |
|3  p(values)                                                            i

Type: <class ‘list'>
Values: [4.9937744140625, 0.8858000040054321, @.02231762208518982]

gs                              He DEEP LEARNING

@한국시연구소 홍근선                      -27- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 29 =====
1부. Deep Learning 개념 정리

1.2 Keras Model 설계 workflow

% 6. Model 시험/적용 :
= Input 4S= output HSE 추정, 추론, 예측 St
w |= 사용 : 예측(출력)값은 10개 category] 대한 확률

predict method

i y_predict = model.predict(x_test)
2 ply_predict)

Shape: (19000, 10)

Type: <class “numpy.ndarray!>
Values: [[3.7@@9611e-37 2.4586847e-37 7.98730116-11 ... 9.99998576-01
0.00000000+00 2.25990146-08]
[4.1258621e-19 1.05057226-06 9.99998816-01 ... 2.96746816-17          2 def p(var) :
5 .939201@e-12 2.7856535e-28]                                         3    if type(var) l=type([]):
[6.8293329e-24 9.9970764e-01 1.1013448e-68 ... 2.5967884e-04         4      try:     '
6.5968328e-@7 1.34030986-09]                                     |          print(f’shape: (var. shape}')
                                                                         6        except :
[1.1335743e-36 2.3277246e-16 2.2123304e-06 ... 5.0458520e-06          Z           -
1.7323557e-14 6.3203368e-03]                                    :     ie  =  ee      ,
[2.0966374e-35 0.00000006+00 1.5035899e-31 ... 0.00000000+00          sR 베니 1 {type(var)}")
9.5313243e-18 0.00000000+001                                      2 __print(f'Values: {var}")
[7.3439289e-85 3.7271026e-37 6.4168218e-17 ... 1.9873503e-35
1.1872521e-11 2.1955921e-31]]                                 a xe ronk, shape, axis
* Return : 예측 값의 numpy 배열 -> category 값으로 변경하기  、 A= wee)
i import numpy as np                                       |    4 0(0)
2 index = np.argmex(model.predict(x_test), axis=-1                |    S # rank = 3,
ind      angen,        ict (x_test), axis=-1)                       ‘i
3 p(index)                                          |   6 # shape=(2,3,4),
Shape: (10088, )                                                  7. # axis: (6,1,2) or (8,1,-1)
Type: <class *numpy.ndarray'>                                           il    Me Ys x)
Values: [7 21... 45 6]

% Callback functions
1 Model. Fit(                                                                    |
2     ‘xeNone, =:             # fe} 402                                                   |
3    -y=None,                # Gab Gojef
4 =~ ‘batch_size=None,                    ,
5     ‘epochs=1,
6        iverbose=1,
7      callbacks=None, = CR
8     validation 1 split= =9 8,
9     validation data= =None,
10     shuffle=True,
이     class weight=None,
12     sample_weight=None,

13      initial_epoch=6,

14      steps _per_epoch=None,

15      validation_steps=None,

16      validation_batch_size=None,

317     validation freg=1,

18      max_queue_size=12,            # 가       Sequence

19      workers=1,                    # generator       Sequence FH?

26      use_multiprocessing=False,     # generator 2 Sequence £//O/?!

21 )

cee                                                                  :             RX DEEP LEARNING”

@한국시연구소 홍근선                      -28- 무단 전재, 복제, SH], 디지털화 금지


===== PAGE 30 =====
1부. Deep Learning 개념 정리

57

orkflo’

m Fit method callbackAH26}7|
®@ Callbacks : 학습 과정에 적용할 함수의 세트. 상태와 통계자료를 확인 가능

def scheduler(epoch, Ir):
if epoch < 16: # 18, 20, 30, 50,
return @.001 # Lr, @.61, @.0@1, ...
else:
return lr * tf.math.exp(@.002 * (10 - epoch))

myacalloacks = [*-- ai
keras.callbacks.EarlyStopping(monitor="val_accuracy”,patience=5),
keras.callbacks.LearningRateScheduler(scheduler),
keras.callbacks.TensorBoard(log dir='./logs'),
keras.callbacks.ModelCheckpoint(filepath='./ckpt/cp.ckpt’,
save_best_only=True, save_weights_only=False,),

]

model. fit(x_train,y_train, epochs=100, batch_size=1024, callbacks=my_callbacks,

은

validation_data=(x_test, y_test))

1.2 Keras Model 설계 workflow

® callbacks.EarlyStopping( ) : patience 동안 AS 성능이 향상되지 않으면 학습 중단

® callbacks.LearningRateScheduler( ) : $4#(learning 「316)을 동적으로 변경

@ callbacks.TensorBoard(): 텐서보드를 사용하여 모델을 모니터링

@ callbacks.ModelCheckpoint() : 일정 간격으로 모델의 체크포인트(모델 또는 가중치) 저장

+ 가츠 부시시

8 callbacks.EarlyStopping() : overfittingHOl] 학습 중단

# fit option : EarlyStoping 스스
my_callbacks = [ keras.callbacks.EarlyStopping(monitor="val_accuracy”,patience=2,_
restore best weights=True) |]         |

I

validation_data=(x_test, y_test))                                      |
model.evaluate(x_test, > test)|                                                  |

락이 5 wh

oy

Epoch 27/166

59/59 [                      ] - 66 4ms/step - loss: @.1289 - accuracy: 6.9609 - val_loss: 0.5518 < val_accuracy: @.9231
Epoch 28/106

59/59 [                      ] - @s 3ms/step - loss: 8.1155 - accuracy: 6.9637 - val_loss: @,5398 + val_accuracy: 0.9255
Epoch 29/108                                                              —
59/59 [                      ] - @s 3ms/step - loss: @.1109 - accuracy: @.9661 - val_loss: 9.5378 = val_accuracy: 0.9243
Epoch 38/100

59/59 [                     ] - @s 3ms/step - loss: @.1137 - accuracy: @.9642 - val_loss: @.5324 + val_accuracy: 0.9256
313/313 [                     ] - 1s 2ms/step - loss: 0.5398 - accuracy: 8.9255

(@.5397588610649109, 9.9254999756813049]

© BHAA] 기다릴 것인가? 이것도 hyper parameter.

am  -   ene     ,       DEEP LEAR

@한국시연구소 S24                    -29- 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 31 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

[i

@ callbacks.LearningRateScheduler( ) : $4 (learning rate) S 동적으로 AA
® 기본 learning rate 설정 : compile 에서 초기값 설정 > 로 가져와서 00001

5 model.compile(loss='categorical_crossentropy',

6                                   야느01268[=66005:00트01265 .RMSprop(learning rate=initial lrate),
i                         metrics=[ ‘accuracy’ ])

bes

9 ## Learning rate schdueler 2} 93207 유어 ALA

10 historyl = model.fit(x_train,y train, epochs=5@, batch_size=1024,
313                 validation _data=(x_test, y_test), verbose=2 )

@ Learning rate scheduling by callback
@ Scheduling 함수 선언

1 def ExponentialDecay s(step)
2     initial_lrate = 6.605

3     decay_steps = 10.
4
5

decay_rate=0.5
return initial_lrate * decay_rate ** (step // decay_steps)

# Callbacks.LearningRateScheduler0l| 인수로 함수 전달

4 model.compile(loss='categorical_crossentropy',
5                       optimizer=keras.optimizers.RMSprop(),

6                metrics=[ ‘accuracy’ ])

8 my_callbacks =
9 history2 = model.fit(x_train,y train, epochs=5@, batch _size=1024, callbacks=my_callbacks,
10                 validation_data=(x_test, y_test), verbose=2)

=iiliothaaeasaneiansanmaneeneen      |   ㆍ     I Al

* 적용할 그래프와 적용 후 그래프를 Sell!

0005     ~                - ExponentiaiDecisy |                                                       |  F     H              oc
|    |
000       {                 1 plt.plot(history2.history['1r'],               000
iat          :                         2               linestyle='--', label="1r_schedule")    |
 “…빼            3 plt.legend()                                     |
0002                        4 plt.grid()                                    0002
Licitexasany       5 plt.show()
나                 | 비해      |                                            a
6    30    20    EJ    eo    ‘a                                               [ o    10    nD    »    oJ    x
® Learning rate 진행 확인 : verbose=1 설정
Epoch 1/100

16
os
608
62
86
es
ba
603
2
ei

~~ ir schedule_val_loss

0    1    Pa    %    40    50

@한국시연구소 홍근선                     - 30-


===== PAGE 32 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

@ WAS learning rate scheduler 사용하기 : 00ㅁ0010116()에서 사용해야 됨
& \0에 callbackSt= 대신 compile(°ll optimizer 001100사용 > monitoringO| 어려움

# (YS! Scheduler 2
tf.keras.optimizers.schedules.ExponentialDecay(
initial_learning_rate, decay_steps, decay_rate, staircase=False, name=None

)

tf.keras.optimizers. schedules .PolynomialDecay(
initial_learning_rate, decay_steps, end_learning_rate=@.¢001, power=1.0,
cycle=False, name=None

)

tf. keras.optimizers.schedules.InverseTimeDecay(
initial_learning_rate, decay_steps, decay_rate, staircase=False, name=None

3 Ir_fn = keras.optimizers.schedules.ExponentialDecay( —

4                   initial_learning_rate= 6.985,

5                  decay _steps=60710,
6                  decay _rate=0.5,
7                  staircase=True)

8 # compile option
9 model.compile(loss='categorical_crossentropy’,

10                optimizer=keras.optimizers .RMSprop(learning_rate=lr_ fn),
11                 metrics=[’ accuracy’ ])

12

13 history2 = model.fit(x_train,y train, epochs=58, batch size=1024,

14                        validation_data=(x_test, y_test))

@ 내장된 learning rate scheduler 사용하기             0.0020 4
“ CosineDecay                                      oe
optimizers. schedules. CosineDecay (

initial_learning_rate, # warmup 시작 Ir    meee
decay_steps,          # cosine cycle 구간 |
alpha=0. 0,         # 최종 Ir

warmup_target=None   ,# warmup 종료 Ir    ee
warmup_steps=0,       # warmup 구간       ㅣ

3 # initial_learning_rate = 0.0
4 # decay steps = 60*45

5 # alpha=0.0

6 # warmup_target = 0.001

7 = # warmup, steps = 60*5

8

9

10    initial_learning_rate, decay_steps, warmup_target=warmup_target,
11      warmup_steps=warmup_steps )
12
13 model. compile (loss=' categorical _crossentropy’ ,
14                         optimizer=keras. optimizers. RMSprop (learning_rate=CosineDecay_Ir).
15                      metrics=[' accuracy’ |)
| 62        60006    ee    panes    2           SES   SSIES IE POSSE OEE gO RE ESTO ne Nore tor meen   들 DE ia  LEARNING”

@한국시연구소 홍근선                      -31- 무단 전재, 복제, Yall, 디지털화 금지


===== PAGE 33 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

@ callbacks, ReduceLROnPlateau( ) : 학습이 AAIE|H learning rateS 감소

reduce Ir = keras.callbacks.ReduceLROnPlateau(monitor='val loss’,

(oon tt so a ie See sot mon se oe Set an ab sos sme

verbose=1,factor=0.3, patience=7, min_Ir=1e-6)

history7 = model.fit(x_train,y train, epochs=50, batch _size=1024,
| callbacks={reduce_Ir],validation_data=(x_test, y_test))

1
2
3
a
5

Max Val_Acc(normal/ir_schi)
10.951/0.956

104
Serres       Se :
ti
'
4                       4
08             ;       ;
으으 normal _val_acc
oe4+-t      가 It_scheduie_val_acc             i
"=" normal_val_loss                re 7,
개 11 schedule val loss      ag’ 년
04               나오시 seh                벼
¥        anes
H
요2 4           +             은          들                 10000 <   r
i                          |
=a
Ves wo aw hes                   i
0.2    T           +           +           +           a         +
9          10          2          30          40          50

m callbacks.ModelCheckpoint() : 일정 간격으로 모델의 체크포인트(모델 또는 가중치) 저장
* Arguments                         학습결과를 재사용하거나, 중지된 학습을 이어서 할 수 있음
keras.callbacks .ModelCheckpoint(
filepath,                # AGA Bs

save_weights only=True, #      or 72
monitor=‘val acc’,    #   7 metric

mode= ‘max’,         # best 의 FH(auto, min, max)
save_best_only=True)   # HAH APR AS ME

* 모델 전체 저장하기

1 #528 전체 저장하기

2 project = './aicamp/'

3. checkpoint_path = project+"cp.keras”
4

5 00 callbacks = | keras.callbacks.ModelCheckpoint(filepath=checkpoint_path,

6                      save weights only=False, save best_only=-False), |

7

8 vmodel.fit(x_train,y train_one_hot, epochs=10, batch_size=1024, callbacks=my callbacks,
g           validation data=(x_test, y test_one_hot))

ㅎ 저장된 체크포인트 파일 확인
- 모델은 keras +010라으로 저장
¥  을 aicamp

2  cp.keras

@한국시연구소 S24        -32- 무단 전재, 복제, Wall, 디지털화 금지



===== PAGE 34 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

© 저장된 모델 읽어 오기
ㅎ Keras.models.load_model()S 사용하여 모델과 가중치 값을 읽어 새로운 모델 생성
- 저장된 값 : 가중치, 모델구조, 0<0100116설정

3 new_model.evaluate(x_test,y test)

313/313 [====                 ==] - 1s 3ms/step - loss: 0.8088 - accuracy: @.8434
[@.8088116645812988, 0.84340000152587891

* 모델에서 가중치만 저장하기

# 가중치만 저장하기

checkpoint_path = project+"m.weights.hS” # must end in ~ .weights.hS”

my_callbacks = | keras.callbacks.ModelCheckpoint(filepath=checkpoint_path,
            save_weights only=True ),]

model. fit(x_train,y_train_one_hot, epochs=3, batch_size=1024, callbacks=my_callbacks,
validation_data=(x_test, y_test_one_hot}}

@ 만들어진 모델에 가중치 loadst7| (2AS 생성하고 !080해야 됨)

# 새로운 모델 생성
model = create_model <01()
model.evaluate({x_test,y test_one_hot}

nu PWN ~

ㆍ

A Pe 내 RD 14

# 훈련되지 않는 SAO 가중치를 1000
model. load weights(checkpoint_path)
model.evaluate(x_test,y_test_one_hot)}

   ae    ~                   ee      oe 90999 0999”
| _65

OF

< 파일이름 지정해서 저장하고 읽어 오기

1 # ckpt file 이를 지정해서 저장하기
2 checkpoint_path = project+"cp. {epoch:@2d}-{val acc: .41} weights 내5"
3
4 my_callbacks = [ keras.callbacks.ModelCheckpoint(filepath=checkpoint_path,
5                                save_weights only=Irue ), ]
6 model.fit(x_train,y train, epochs=3, batch_size=1024, callbacks=my_callbacks,
7         validation_data=(x test, y_test))
® 파일 지정해서 읽어오기                                          [ABE files ]
1 model = create_model_cpl()                        ~ BB aicamp
2 # file 이름으로 지정해서 읽어오기                         oe            .
3 model. load_weights(project+' cp.@3-0.9283.weights.h5")         BB &9.01-0.9077.weights.hs
4 _model.evaluate(x_test, y test, verbose=1)                  “BR op.02-0.9203 weights hs

“AB cp.03-0.9283.weights.hs
| ep.keras
2 m.weights.h5

@한국시연구소 홍근선                        -33- 무단 전재, 복제, Wall, 디지털화 금지



===== PAGE 35 =====
1부. Deep Learning 개념 정리                      1.2 Keras Model 설계 workflow

%※% 모델 저장과 복원 : model.save / keras.models.save_model
ㅎ 모델의 아키텍처((6ㅁ01091), 가중치, optimizer 상태 등 학습 당시의 ABS

하나의 파일에 저장
> 모델 정의 또는 교육에 사용되는 코드 없이 동일한 상태로 다시 인스턴스화 됨
> 동일한 모델, 동일한 상태에서 추가 훈련 가능
> 저장 형식 : ‘keras’ 또는 ‘HDFS’

HDFS 형식은 보안문제로 지원 중지
> 전체 모델 저장하기
# 전체 모델(가중치, 학습환경-6000116)을 Hee 저장 (keras BM 저장)
model.save(project+‘model save.keras’)                       # Model save

keras.models.save_model(model, project+'save_model.keras')
model.save(project+"model save.h5") # HDFS format AA # 보안문제로 지원중지

* 전체 모델 복원하기

Bm WN ke
i)
haa
w
FE
fi)
5
foots
09
=
하
w
on
고
be
°
onde
i)
o
rt
+
i)
fo
0]
©
<
^
te
cn
아
a)
~
wi)
~
te
09
a
oe
fo)
s
0
~
wy
a
<
40)

Wi

model _5.load_weights(project+'model_save.weights.h5')
model 5.summary()

1 # 2S 읽어오기

2 model 3 = keras.models.load_model(project+'model_save.keras') | ~ (§ aicamp

3 model 3.summary() 때

4 model 4 = keras.modeis.load_model(project+'save_model.keras')           =

5 model 4.summary()                                                         B model_save-keras

6 model 5 = create_mymodel()                                   BB model_save.weights.h5
7

8

a  save_model keras

68                    -               더           … ER DEERTEARNING”
@한국시연구소 홍근선                     -34- 무단 전재, 복제, S43, 디지털화 금지



===== PAGE 36 =====
1부. Deep Learning 개념

1

1

정리                                               1.3 Keras.layers API

Chapter 1. Deep Learning 개념 정리

( 핵심 개념 및 용어 정리 )

.1 Deep Learning 개요
1.2 Keras Model 설계 workflow
.3 Keras.layers API

X* keras.layers API

.                              =         1 4 PPPS shape, type, value BP
¢  Layer = 텐서 입력/출력, 계산 함수 + 상태(가중치)           2 def p(var) :
a                                   3      af type(var)!=type({]):
@ 레이어 인스턴스는 함수와 유사하게 호출 가능                        4           try:
© 8491 다르게 상태를 유지하고, £21 중에 undated              :         —
layer = layers.Dense(32, activation='relu‘ ) |             매매         ,
2 inputs = tf.random.uniform(shape=(10, 20)) |    2   ee ae ee )
3 outputs = layer(inputs)                                             °
/ Layer                      주
             i p(layer)   Callable
Type: <class ‘tensorflow.python.keras. Layers, core. Dense’ >
Values: <tensorflow. python. keras.layers.core.Dense object at 0x@080023E77830B20>

/ layer.weights

p(layer.weights) 상태00000)

Type:

<class ‘list'>
Values: [<tf.Variable ‘dense_1/kernel1:@' shape=(20, 32) dtype=float32, numpy=
array([[-@.02848014, -@.11695404, -0.2513118 , 9.31205732, 0.00771165,
@.06414306, -@.03926027, 0.13838434, -8.23792146, -0.13853726,
-@.28225848, -@.29197153, @.25246686, @.04308635, 0.09293702,
a ㅜ04ㅋㅋㄷ    ㄴ@0ㅋㅎㄷㅋㅎ0ㄷ0 a ㅋ7<4ㅋ944     ㅋ07ㅜ1ㄷ4ㅅ4ㅠㄷ a arraaca

@ outputs

i p{outputs)

a

| Shape: (18, 32)

Type: <class ‘tensorflow.python. framework.ops.EagerTensor'>
Values: [[0.73668003 0.            @.            Q.            6.6605805 0.
@.3870389 @.           8.           @.61188703 6.           0.

ey

pda

-35- 무단 전재, 복제, 발

4, 디지털화 금지


===== PAGE 37 =====
1부. Deep Learning 개념 정리                                   1.3 Keras.layers API

® Activation 함수 : 내장 함수

# ArgumentsS = PES

keras. layers.ReLU(max_ ve Ue ROne negative slope=0.0@, threshold=@.8)
# 80% value:  , BSF @ a2,     (AY

fs    Be                    : LeakyReLU
# 애여매이바 #       /          : Thresholded 4610
keras. layers. LeakyReLU{alpha=0.3)      # x < oot OP f(x) = alpha * x

keras. layers .PReLU(alpha_initializer='zeros’, alpha_regularizer=None,   —by Male  3b
alpha_constraint=None, shared_axes=None)
#leakyReluQWA? ABAB      수 QA

= +

keras. layers .ThresholdedReLU(theta=1.6) # x > theta O/ f(x) = x,
keras. layers .Softmax(axis=-1)                  alization FEF
keras. layers.ELU(alpha=1.0)                  alpha * (exp(x)

# alpha l= 1 WH ‘'setu' 가 A
& Arg uments 7F ti
keras.activations.sigmoid(x)            # 1/(1+0%-x)
keras. activations. tanh(x)
keras.activations.softplus(x)         # Log(exp{x) + 4)
keras.activations.softsign(x)         # x/(abs(x) + 1)

15                         38

2S do Leaky Reto

>> ELLNExpenential near unit)
281 man Theeshoided RELL

* 함수의 모습비교 6)

05

00

71

「    향상된  Activation  함수      nee    yvot     y               :       soo!          Testing Accuracy vs Number of Layers an MNIST
ㅎ SELU: Scaled Exponential Linear Unit (2017)                                                                   ㆍ
/* alpha=1.67326324, scale=1.05070098                   zi
/ ifx>0: scale * x, ifx<0: scale * alpha * (exp(x) — 1)
 Selu(x) = scale * elu (alpha)                                       3
장단점                     로
- Self-normalization: S422] 분산을 자동으로 조절, z
gradient vanishing/ exploding 감소                    ao

- negative input: 음의 입력이 중요한 데이터,
이로 인한 gradient vanishing=Allol] 효과적

19                2
Number of Layers

Swish(x) = x * sigmoid(x)

/ 장단점
- ReLUS 대신하녀 대부분 좋은 학습 결과
계산비용 : 91910010보다 약간 높음, mish > swish > sigmoid > relu
@ (Misb/activation (2019)
(-Mish(x) = x « tanh(softplus(x))
- 많은 경우(주로 imager 2|) Ol swish} 좋은 학습 결과
- 특정 작업에서 5“/15나 『614보다 성능이 저하 될 수 있음
실험적 결정이 필요함

는  는            eee    SSE

@한국시연구소 홍근선                    -36- 무단 전재, 복제, Sil,  디지 털화 금지

pent

n



===== PAGE 38 =====
1.3 Keras.layers API

144. Deep Learning 개념 정리

@ 새로운 Activation 함수                                      낚여      Cy
@ GELU (Gaussian Error Linear Unit)                                  Ate

f& GELU(x) = xP(X <x) =x (x), (x)= Gaussian_CDF(x)

> GELU(x) = 0.5* (1 + tanh (sare (2) «(x+ 0.447152°)))
 입력 US 가우시안 분포를 이용해 변환하는 비선형 함수,
@ ReLUSC} 부드러운 비선형성을 제공, 복잡한 함수를 표현, 모델의 표현력과 수렴 속도 향상 가능
“> BERTL 6『1등의 transformer 기반 모델에서 널리 사용
®@ GeGLU: GELUS| 변형
 두 개의 선형 AS GELUS 조합
 효율적인 계산이 가능, 대규모 모델에도 적합
@ 안정성 향상가능, vanishing gradient 문제 완화
+ 특히 NLP, Speech, Time seriesS 복잡한 WHS 더 잘 표현

6 GeGLU(x) = x * sigmoid(W, * x + by) * sigmoid(W, * x + 02)

：                                 * Gru Groteel Lear U4
(460
«(mW tb) 0680+이

ReGLU(z, W, V, b,c) = max(0,2W + 0) @ (2V + 0)
GEGLU(z, W, V, b,c) = GELU(aW + b) @ (2V +c)
SwiGLU(z, W, V, 6,¢, 8) = Swishg(«W + 0) @ (aV + 0)

ow GEL
ome ROLL
… LY
2

~

시뇨 )

~

Figure 1: The GELU (4 = 0,0 = 1), ReLU, and ELU 레애~     :        '
(a = 1).

® Activation 함수 사용 방법 두 가지
@ 1. layers.Activation(...) 에 인수로 전달 : arguments 없는 경
@ 2. 자신이 레이어로 사용되는 경우 : arguments 전달 가능

fo

®@ Sequential model 에서 사용하기
6 model.add(layers.Activation('relu')) # 으수 서는 경은
7 model.add(layers.ReLu())          # 일주 Ce 경은
8 model.add(layers .ReLU(max_value=None, negative_slope=0.8, threshold=0.@ ))
® Functional model 에서 사용하기
6 x2 = layers.Activation(‘relu')(x1) # argument 애스
7 x2 = layers. ReLuU()(x1)           # argumet A=
8 x2 = layers RelU(max_values?.9, negative_slope=9.3, threshold=@.@)(x1)
e  614에서 『9410610+적용한 결과 비교                    Max _val_acc:0.957099974155426
> 학습속도 향상, 성능향상                  버티
08  ta
‘                    “* elu val ace
os                      www BOL Para val acc
~~ Rell) val joss

wwe Rel Para val toss

치태

@한국시연구소 홍근선                                 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 39 =====
1부. Deep Learning 개념 정리                                   1.3 Keras.layers API
7

m= Regularizer : 가중치 또는 출력값에 Ｌ1 / L2 패널티 적용 (Overfitting 방지)
@ 적용 대상 / 방식 : kernel, bias, activity’) 에 L1, L2, L1_L2 적용

layer = layers.Dense{ units=32,

= 1 아베 빠따 배띄 배서 | 배어 개 애서 메어 | 에 | 에에 | 배바-개에 — 여 며

bias regularizer=keras.regularizers.12(1¢-4),
activity _regularizer=keras.regularizers.12(1e-5) )

4 input_x = layers.Input(shape=(28,28), name=‘input‘)
5 × = layers.Flatten(name='flatten‘)(input_x)
6 «x = layers.Dense(32,

7            Kernel regularizer-keras regularizers:12(0.01),

8                  bias_regularizer=keras.regularizers.12(@.@01))(x)

9  × = layers.Activation(‘relu', name="relu’) (x)

10 x = layers.Dense(10,

11                                  kernel regularizer-keras. regularizers.12(@.01)) (x)
12 output_x = layers.Activation( ‘softmax', name=‘softmax’)(x)

i         *
@ Val loss 지속적 감소                                        Max Val acc(0.9463 / 0.9681)
> 성능향상                           Ts

0.9 4+
> Overfitting 감소                                            084)
0.74
~~~ val_accl
06 4                               ~ Yast acc?

> val_loss2

= DropOut Layer

@ DropOut : OyerfittingS 방지하기 위한 Regularization 기
@ 학습과정에서 일정 확률로 노드들의 HSS 차단 (노드 무작위 선정)

/* 노드의 출력에 강제로 ‘O'S 곱해 학습 차단
* 수시로 모델의 형태가 a
/* 다양한 모델이 협력하는 ㄷㅁ056000!6 모델이 됨
@ 노드간에 연결이 많음= 노드간 협력이 많음
f 상호 의존 발생, 다양성이 결여됨 (generalization 약화)
@ 적용 및 성능 비교
/* Val_loss 감소 지연 , val_acc 상승 지연
/*% Val_loss 지속적 감소
> overffiting 감소, 학습 지연
input_x = 1280605.10041(50206=(28,28), name="input')
x = layers.Flatten(name='flatten’}(input_x)
x= layers Dropout (0.1)(x)
x = layers.Dense(32){x)
x = layers.Activation(‘relu’, name='relu’)(x)

x= Layers Dropout (?.1)(x)
10 x = layers.Dense(10@){x)                                     aS
11 output_x = layers.Activation(‘softmax', name='softmax' ) (x)

(hb) After applying dropont.

76 "  ze                            .      Ss                 =    :     Soe DEEP LEARNING”
-38- 무단 전재, 복제, Sal, 디지털화 금지

@
ro
HU
>
[요
ae
b
04
i
rz


===== PAGE 40 =====
1부. Deep Learning 개념 정리                                 1.3 Keras.layers API

= BatchNormalization Layer

 BatchNormalization: 학습속도 향상을 위한                          batch        고토
ㅎ SH |S (internal covariate 5111{[)때문에                    ae   mean gid
/* 배치 단위로 통계적 특성이 다름                                relesles
> 레이어 출력의 통계적 특성이 흔들림 KL DHE  anininmoes
> 레이어가 깊을 수록 부정적 영향을 주게 됨    al     0  ninin     호    ;
> 학습속도 둔화                       Brat 암석,  %니이디피 . [|
@ 배치 단위로 node 출력값(활성화 전)을 00「00201126함       Xx) is | (2 히 . [3| [2
+ Normalize : 평균을 '0'에 가깝게, 표준편차를 '1'에 가깝게 ※× 、 11 0 1     [2]

 결과적으로 WS 범위제한으로 안정적 학습(학습속도 향상)

Batch 1

Batch 2

77

@ BatchNormalization 알고리즘
@ 1. 배치단위에서 통계적 특성(평균, 분산) 계산
@ 2. 활성함수 입력을 평균, BASS normalization 하여
활성함수에 제공
@ 3.348 scaling & shifting
@ Normalize= 발생한 비선형성 감소 해결을 위해
* 출력값에 곱(50201109) , 합(51111409)
> 활성함수로 들어가는 값의 범위를 넓혀줌
활성함수의 비선형성을 활용할 수 있도록
> scaling factor r2} shifting factor 는
역전파 과정에서 학습 (파라메터 추가)
ㅎ 추론 할 때는 평균, 분산 AS 어떻게 찾나?
A 학습단계의 평균과 분산 AS 평균하여 적용
A 또는 학습단계의 평균과 분산 US 이동 평균한 값을 적용
® Batch size2| 영향을 받음 : 적당히 커야 함(주의사항)

@ #『 : 2trainable+2non-trainable / node

'          c
* 장점 :빠르고, 안정적                           mt
@ Gradient vanishing 해결, learning rate/decay rate 가속
@ 가중치 초기화 영향 감소                                                  —                                5
ㅎ Drop outS 제거해도 성능 유지                         Dox OWA     pose 내
78                     Maier             0 30 DEEP LEARNING
@한국시연구소 S24                    -39- 무단 전재, 복제, 44], 디지털화 금지


===== PAGE 41 =====
1부. Deep Learning 개념 정리                                 1.3 Keras.layers API
0                                                                                 .

*＊ BatchNormalization 적용                          오구           으으         =,
4  100바 × = layers. Input(shape=(28, 28), name=" input’)        fngut (inpoliayer)       1 0. 00}
5 x = layers.Flatten(name="flatten’)(input_x)
flatten (Flatten)         (None, 784)           @
6 x = layers.Dense(32)(x)
7 Xe layers. BatchNormalization()(x)                             dense_8 (Dense)           (None, 32)            25120
8 x = layers.Activation(‘relu’, 02006='『610')(×)             batch normalization 9 (Batch (None, 32) "128  fy
기 기 layers .Dense(1@) (x)                                   relu (Activation)        (None, 32)           C)
106 x= layers.BatchNormalization() (x)                                        ：                   14
—— '가잊"아글승미니        :       06056 9 (Dense)           (None, 10)            330
11 output_x = layers.Activation('‘softmax', name="softmax') (x)
Batch sores) tration 28 (Satc Gnesi 4
softmax (Activation)       (Hone, 18)            @    녀
[  성능 비교                                                 Total params: 25,618                                g
Trainab)      : 25,    oo 느
^ 10 epoch 정도에서 최적화                                   soritralatl arcane  34
@ Accuracy® 최고                                                                83567 BatchNormalization
> 학습이 빠르고, 좋음                                            —       Max Val_acc(0.9463 / 0.9679)
~ 시어                                     See eee cpa "areca rere rer
0.94 0          }      |
@ 파라메터 수                                           os yy
'
tv 4 x features                               waaay                   --- val_accl
- 2 trainable : gamma, beta                          0.6 7-\                          — val_acc2
- 2 non-trainable : running mean , running std        05 |                                  =z Matos}
0.4 4
0.3 4
0.2 4
0.1       '       ~       7       -       .
-                                       에 케케      rot      태태. .케메테 에
_79                                                                                                Rk DEER LEARNING

1 Deep Learning 개요

ai.
® Machine Learning 정의, 분류

@ Regression, Logistic Regression, Multi class logistic regression

© ASA 표현 학습 개념, 역전파 학습, Vanishing Problem

® Optimization Algorithm

® Overfitting, Generalization

m 1.2 Keras Model 설계 workflow

® Model Define API : Sequential model, Functional model, Subclassing model
® Model Compile API : Optimizer, Loss functions, Multi loss

® Model Fit API : Training / Validation dataset, Epochs, Batch size

@ Model Evaluate , Predict APT : Test dataset

@ Mode Save API

@ Callback functions

= 1.3 Keras.layers API

@ Layers API, Activation func., Regularizer, Dropout, BatchNormalization



===== PAGE 42 =====
=. Recurrent Neural Network


===== PAGE 43 =====
2.1 RNN Cell Architectures

2부. RNN

x 학습 목표

a RNN 구조
@ RNNO| 사용되는 FL Cell PAA} SAS 이해한다
> 시간축에서 역전파 학습이 이루어지는 SAS 배운다
® RNN architectures 구성 방식을 배우고,
* 실제 구현되는 다양한 구조들 파악한다

® One to many, many to one, many to many

® Stacking, Bidirectional, Residual , Dense RNN

@ Handwriting Generation with RNN
@ 필기체 문장을 생성할 수 있는 RNN 모델의 구조와 동작 방식을 배운다
eas
® Stock prediction : 주가 시계열을 RNNCS 처리하는 모델
@ Char-RNN : 문장을 학습시키고, 스스로 문장을 생성하는 모델
® MNIST-RNN (Basic , Bidirectional, Hierarchical RNN )
@ SYS 시계열화 하여 인식하는 BAIS 이해하고,
@ 다양한 구조의 RNN 모델을 만들어 HSS 비교해 본다.

HC DEEETEARHING”

83.

000 DEEP LEARNING

eee

-42- Sat 전재, 복제, Sl, 디지털화 금지



===== PAGE 44 =====
2부. RNN                                                                   2.1 RNN Cell Architectures

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures
2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)

2.6 Optimization
2.7 Handwriting Generation with RNN

DEEP LEARNIN

RECIPE FOR YOU

3 Recurrent Neural Network(#3t4! 24h)
w SHS 이전 계산 결과의 SHS 받음 : 현재까지 계산된 an-712)

* YAS 시간 축에서 순차적으로 공급되고

© 입력 정보를 내부에서 기억함
* 새로운 입력과 기억된 정보를 가공하여 출력함

@한국시연구소 홍근선                     -43- 무단 전재, 복제, 244), 디지털화 금지


===== PAGE 45 =====
2부. RNN

2.1 RNN Cell Architectures

%* Recurrent Neural Network(2-3t4! 2 25)(2)
ek 시점에서 볼 때 입,출력 관계

pee td
600

0

BEEP LEARNS”

% Recurrent Neural Network(2:3}4! 2 2#)(3)

= 세 종류의 가중치 : 확장해서 RNN 모델(4ㅁ011이 아니라) 전체를 볼 때
® weight, recurrent_weight , output_weight(RNN 밖에 있는 가중치)

0

O                        oy       o,         Ort
V                         V         f        mI
Cs      셀               Ww 에 Ce    때 0:       Oe
Oo} 6600      ㆍ      w \ +        Ww

Unfold

U                            U        U         U

x                         Xe        x,        x

@ Unfold = unroll : 점차 unrollS 많이 사용

/@ RNN cell, LSTM module, GRU unit : 하지만 혼용

ㄴㄴ =

z        -44- 무단 전재, 복제, ail, 디지털화 금지


===== PAGE 46 =====
2부. RNN                                         2.1 RNN Cell Architectures

% RNN 적용 사례

8 순서 데이터에 꼬리표 달기 (Sequence labeling)
© 리뷰 읽고, 감정 분류하기(660110ㅁ7601 classification)
© 필기체 인식 / 음성 인식 (handwrite recognition/ speech recognition)

8 시계열 예측 (time series prediction) / 파형 4444 (periodic function generation)
* 차량/고객 예측, 경제 예측, 날씨 예측 / 필기체 생성

we 비정형 정보 처리
* 사진 훌어보고 인식하기 (Sequential processing of fixed image)

BAAS 인코딩/디코딩, trnshorwer
© 자연어처리 : NLP(Natural Language Processing) : 요약, 질의 응답, 대화, HA
® 기계 번역 : NMT(Neural Machine Translation)
* ALZ(story) 2a 질문에 답하기

= CNN 모델과 결합
 사진 보고 주석 달기(1089ㅇ captioning)

—            ~             |                 “HR DEER 64006

2 RNN cell 구조
® Basic RNN cell
@ LSTM(Long Short Term Memory) cell(module)
® GRU(Gated Recurrent Unit) cell(unit)

(                     »\
———,
|         of
고
%) Basic RNN cell                (0) sta cel                               GRU cell
oo          .            0 개     00000 Colas biog: httn‘//colah github iof WW" DEEP LEARNING
@한국시연구소 홍근선                    -45- Sct 전재, 복제, 24], 디지털화 금지


===== PAGE 47 =====
2부. RNN                                                                   2.1 RNN Cell Architectures

of Basic RNN cell : #2+£ single cell, #P+ layer 단위로
.                     yrons    :
m Basic RNN cell ~"       a,
e  h, = tan     h    t-1          t + b,)
= tanh(Wh,_; + Ux, + b,) (다른 표현)
® #p > Hn*Hn + Hn*Xn + Hn = (Hn+Xn+1)*Hn
® Xn: input feature 수

® Hn: RNN layer 의 cell +                                                           에

3 NNOJA] Parameter2| 수 :

f:x—yY
:Y=o(X -W+b                     (%:)
f     (     let   m                (0 Basic RNN cell
[020 ~ Xa)         +[0]  =[3132… Ym]
1 W
we Rom
een    om          mae    itr      2 마타 allah

Neural Network       Pointwise        Vector

Layer         Operation     Transfer     Gonearenats       Copy:

Output

Pointwise = Entrywise product, o or ©

> Next (Cell) State

@utput Gate

>  Next
ie      Hidden State

Output = Hidden state

dann yy
© cl WN  |
SYP pare
3   |       a    i sn

@한국시연구소 S24                     -46- 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 48 =====
2.1 RNN Cell Architectures

HSER LEAN

Forget Gate

Input Gate

3% The Core idea : Conveyer belt & Gates

De o (Wy-[he-1, 24]  + 23

cell 9136에서 버릴 정보를 선택
- 무엇을 얼마나 버릴 것인가

iy = 0 (W;-[he-1, 24] + 00)

cell state] 저장할 정보를 선택
- 무엇을(6,) 얼마나(』,) 저장할 것인가

i

-47- 무단 전재, 복제, S4ll, 디지털화 금지


===== PAGE 49 =====
2부. RNN                                                          2.1 RNN Cell Architectures

XX The Core idea : Conveyer belt & Gates

Update (cell state)

Cs.             Ce
t—1   ~         <
0.                               기억할 정보를 수정
prev_state * forget_gate -> forget_state
forget_state+curr_state*input_gate -> update_state
Output Gate              he

(hidden state)
.                  0: =o (Wo [Fe-1,2:] + Bo)
hy = 04 * tanh (C;)

출력할 정보를 선택
개                                                           updated_state * output_gate -> output(hidden state)

761

Es       ~       |    aren

% LSTM 연산
Basic RNN                                     LSTM
시그             i           o
h, = tanh (w( x,  )        f   _     o     w("1)
0           o           Xt
0         tanh
Ce = fOCe_1 + iOg : cell state
h, = 0 © tanh(c;) ㆍ hidden state
벡터가 계산 됨
@한국시연구소 홍근선                      -48- 무단 전재, 복제, Sl], 디지털화 금지


===== PAGE 50 =====
Upd

Pee (W. - [ht—1, 21])
Reset gate    ,

r, = 0 (W,.- [he-1, 2¢])

h, = tanh (W - [ry * hei, @1])

hy = (1 — 2) * he_ + 2 * hy

* = Pointwise = Entrywise product, o or ©

sp fic : hy tildet= 현재와 과거 정보를 기준으로,
sy Lstholmn    Foyt gate Sy 과거정보 일부를 지워서 기억할 정보를 유도
leapt                     LSTMS] FAS 유지하면서도 계산 복잡성 낮

~
ao 25)

Cho, Kyunghyun, et al. "     ni

H

ion.” arXiv preprint arXiv: 1406. 1078 (2014).

.1 RNN Cell Architect

3 RNN layer # of Parameter
m@ Basic RNN cell

\e aM
1110  ol, vert +  Dat a ae { ) yx UW    T
= LSTM cell

=(( Xn + Hn + 1) * Hn) * 4 #Tensorflow — bios  (Yah)

or ((Xn + Hn 42)+ Hn) +4 #PyTorch —  21 (ht 락스 ef bias 34 )
m= GRU cell
= ((Xn + Hn +2) * Hn) *3_

rng MAS.
1
기고 오구 거
60    0
[0 6 |
aa           0 '
고대
00  LSTM cell            GRU cell
뉴는 4".
한국시연구소 S24       -49- 무단 전
@한   「   et t                TE eas

전재, 복제, S4ll, 디지털화 금지

2.1 RNN Cell Architectures



===== PAGE 51 =====
2부. RNN                                                                   2.1 RNN Cell Architectures

XX BPTT Vanishing Problem
@ Basic RNN 은 시간 축에서 Vanishing 문제가 자주 발생, LSTMZt GRUE 상당히 개선됨

00600 00666:

00000     배후
Basic RNN                                                rs GRU

® Vanishing 발생 감소
1) Activation func. 통과하지 2S (activation func.2| saturation S49 0| 문제)

2) Weight 22] 37/2} 상관 AS (weightZt2| 소멸이 문제)
# Backpropagation of error: Error = cost f(z,y)=5, W = w-lIr 개  개별

3% BPTT Vanishing Problem 이해

= Sigmoid , tanh activation2| $2
@ 다음 layer 2HOA sigmoid activationS 사용하면 학습이 가능할까?

Epoch                      Learning rate             Activation                Reguiarization              Regularization rate              Problem type
000 ,000                       1                               ”           Sigmoid               -            None                                      0            Classification
EATURES                                        + -— 4 HIDDEN LAYERS                                 OUTPUT
Test loss 0.602

hich pro per wes
"                    ie                  eS                                                              Training loss 0.575

§ neurons                    5 neurons

jee

무투투두

1000                                                            일만 DEEP LEARNING

@한국시연구소 홍근선                     -50- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 52 =====
2부. RNN                                                          2.1 RNN Cell Architectures

3% RNN 『

© 동일한 파라메터(가중치 행렬)가 매 time step] 사용됨
* _초기값 /:,는 VEE 학습결과

Tgp, 골든 oat Dd 1

= tanh(Uay tf Ws, 1)

a                                                                         = softmaz(V'
20             vy             XQ             x3             4                   Ut = 9080000(09)      x 2,

'법

w E32| 6「아를 시간 | 축에 따라 미분하자 (chain rule 적용)
® \에 대해 편미분하면         \에 대해 편미분하면         4에 대해 편미분하면

OF;    _ SEs 008          oe      OE OE 006 Oss Os,    OF;    = 6A gr
067 Oy BV               ye Oy O55 Os, OW 00
_ OF Oy Oz                             5°) _ aR, _. OF 058 092
- 008 Oz av.                         2  때 Oz 때 Os3 885 020
= (04 - y3) @ 98                                     2 = Ur, + 181
® ‘tensor product
현재의 값으로 계산 가능      > 시간 축을 따라 역전파                > tanh 이전 값으로 미분 가능

SE                                                                                                   a

YR DEEPLEARNINE™

@한국시연구소 홍근선                      -51- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 53 =====
2부. RNN                                             2.1 RNN Cell Architectures
|

bg TBPTT(Tru ncated Backpropagation Thought Time)
w A| BAZ} 긴 0씨모델의 문제
* 순전파(1055계산), 역전파(\수정)에 많은 메모리 필요

8011의 순.역전파

= TBPTT                                                                       전 Al LAOW 대해 연산

@ 순전파는 계속 진행
@ 무한길이 데이터 학습 시에 반드시 필요

vt
TBPTT 의 순,역전파
Wry (¥)                                역전파 ALBAS 제한
—   RAN   ^
Win)
W,,(U)
x,

103

@한국시연구소 홍근선                       -52- 무단 전재, 복제, all, 디지털화 금지



===== PAGE 54 =====
2부. RNN                                            2.2 RNN Model Architectures

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNING

CiPE FOR

0 RNN Architectures : 입출력을 중심으로

one to one         one to many           many to one                 many to many                many to many

DDD  oon a
| 베베 ooetd 떠

(1) Vanilla mode, without RNN : image classification
(2) Sequence output : image captioning

(3) Sequence input : sentiment analysis

(4) Sequence input and sequence output : Machine Translation

(5) Synced sequence input and output : video classification with many labels

if training vanilla neural nets is cotimization over functions,
training recurrent nets is optimization over programs.

106                                                                                                        a ala

!국씨연구소 홍근선        -53- 무단 전재, 복제, wall, 디지털화 금지

@
[에


===== PAGE 55 =====
2부. RNN                                            2.2 RNN Model Architectures

= RNN Architectures 별 기본 코드

| Keras.layers.LSTM / GRU &미의 arguments LL

tf.keras. layers .LSTM(
units,
activation="tanh",
necurrent_activation="sigmoid”,
use_bias=True,
kernel_initializer="glorot_uniform’,
recurrent_initializer="orthogonal”,
bias_initializer=“zeros",
unit_forget_bias=True,
kernel _regularizer=None,
recurrent_regularizer=None,
bias_regularizer=None,
activity_regularizer=None,
kernel constraintcNone,
recurrent constraint=None,
bias_constraint=None,
맘앵에버 0:

True: 조284/ 70006 gate #18 GF
kernet F YEE

recurrent_dropout=@.0,             ce
return sequences=False,            time 2d GE

neturn_state=False,
go_backwards=False,
stateful=False,

560; 주 동 0  Gale
True:  input seq
True: batch 너가 i

amie: ba. fan Ue

es ‘batch 2    he
time_major=False,               # True  in, out shapes
unroll=False,                 # BPA BAS -

**kwargs

import tensorflow as tf
from tensorflow import keras
from tensorflow.keras import a

= One to one 구조
@  Dataol 시간개념이 없는 Data : image classification

=                               :                   x_dim = data_dim = features =
# ALVA OL GIO, Ff image classification 운사               timesteps = sequence length 0)
model = : hatacmsicle. camenthe (i                         units = cells & 50

model. add(layérs.Dense(units, input_shape=input_shape))            £€o           7)
-         s                      a

#RANNOPAT timestep ~ 12/ GF -                          24  Veu  ¥    ML        =

model.add(layers.LSTM(units, input_shape=(_1, x_dim)))

OW 5: 년 Ne

One to one

Many to one

soko

8 many to one 구조
시계열 또는 ABA 데이터를 처리하는 기본 모델
*@ Data shape : (samples, timesteps, features )
@ 기본 코드

은 일

|i units = units # RNN cell 수
, 2 model = keras.models.Sequential()
3 _model.add(layers.LSTM(units, input_shape=(timesteps, x _dim)))       D1 | 8
시              = | ㅁ216|
:     :                    을 | 0316
au   like   + :   T>  Feok Aves 을 04 9
ｌ
wr     L     L                    은 | 05/o|
ho                  2  06/8
07 6 ㅣ

BAIA 홍근선          -54- 무단 전재, 복제, Wal, 디지털화 금지



===== PAGE 56 =====
@ RNN Architectures 별 기본 코드

Many to one

1 x_dim = data_dim = 25
2  timesteps = 7
3

HEAHSERESS many to one #eHRH THE

i                                        units +~ 5@
2 model = keras.models.Sequential()                 —
eo |       3 model.add(layers.LSTM(units, input_shapes(#imesteps, data_dim),
— tL   4             return _sequencesfralse)) # default : False
om ort                        input: | [(, 7, 25)]                     =
Istm_56_input: InputL.                     Ph)
tot 그      S| 900 | 12, 7,25)            Daler Ar,
         복학 vou © Av kd
Rm      input: | (?, 7,25)
return_sequence=False           isim_56: LSTM  output: an 50)
‘i   ;                             ll
any 9 04815      | #HREBEEEE many to many sHsHeeeS                           |
2 model = keras.models.Sequential()                          |
3 model.add(layers.LSTM(units, input_shape=(timesteps, data_dim), |
4                    re           3     4                 |

input: | [(2, 7, 25)]

output: | [(?, 7, 25)]          [ㅣ
때                           |

— 트기                                         input. | (2. 7, 25)

지어 주라아0 6     Ism_57:LSTM [—         —      os 삐
ao C29)    (2<0)이 tive cep  be aM,

istm_57_input: InputLayer

[우기
_

le
e~

eee     z                :                 Scene Ome     sonore     ssa ccmmennnre!
ane                                                                              ee                 ‘See DEEP LEARNING
레베 1                                                         Seater sss sehr

= RNN Architectures 별 기본 코드   ew \p ~

1     im =      im = 25
/ 5 We                     × dis  data_dim  25
|                       2  timesteps = 7

Many to many                                                    3 units = 50

#HBHeHHEEH many to many : TimeDistributed #####8##8#
model = keras.models.Sequential()
model.add(layers.LSTM(units, input_shape = (timesteps, data_dim),

1

2

=

4                    return_sequences =     5]

5 model. add(layers.TimeDistributed(layers(Dense(T)))

5 print(model.output_shape) # (None, 7, 1)        aw ct py my
i 쁘기 주아

*LSTM 출력을 Dense® 받기                                            ;                  Sunhg
가                                              a) So 로 BP

- TimeDistributed( layer ): layer
- Dense layer2] 파라메터 +=?

input: (| [(@, 7, 25)]
output: TT, 7, 25

Istrn_8_input: InputLayer

ory

님 여

input: | (?, 7,25
output: 407, 50)

           -르19 prebriloed

oS.
input: |\%,/7, 50
time_distributed(dense): TimeDistributed(Dense) inpu Ne (
output:(| QR, (

Istm_8: LSTM

@한국시연구소 홍근선                   -55- 무단 전재, 복제, Yay 디지털화 금ㅅ
=                         aie      ㆍ ㅋ시|, St,    2



===== PAGE 57 =====
2부. RNN                                            2.2 RNN Model Architectures

@ RNN Architectures 별 기본 코드
@ many to many: iene ( many to one + one she 00007

속 데이터를 UOT ie   학습할 때,  슬할 때, batchets| 학습에서 ED oa apoE   전달하는 용도

@ Stateless a  BA     로운 batch(&           서 2&7            5, features )
Many to many - 2                                           2 Bape v0PVV {se     premee 471)

1 batch_size = 1            a
2 inputs = keras.Input(shape=(Nong    i        게스 2009 7
3                  batch_sizé=batch size) ## stateful 4/SA/ 전으4/
4 outputs = layers. LSTM(units=units,

return te a 900

#output_shape ~> ela steps, a
8 model = keras.Model(inputs=inputs, outputs=outputs)

[ shape] stateful 보이지 않음 ]
input: | [(1, ?, 25)]
output: | [(1, ?, 25)]

input_16: InputLayer

input: | (1, ?, 25)

Istm_19: LSTM
output: | (1, ?, 50)

@ RNN Architectures 별 기본 코드
® many to many: stateful ( many to one + one to many ) (2)

@ Training : batch7} 바 때 이전 batch2| 상태에서 학습을 계속
/* ‘1’ epoch 를 반복 실행 : 상태 27   요하기 때문 (epoch 마다 상태 27
@ 021대내부의 데이터 조오 이자 지을 TO saps   shuffle 금지
@ Batch_size= 모델 정의할 때와 같은 값, 내부에서 구분할 상태의 수

에 aq

Many to many - 2

## Training
# epoch = 2 OfAT batch 두

의

# epoch A/4f
# epochLfOYA? stateful
# model OfA{2} Zhe
# batch GO/E] shuffle =
print(f'Epoch({i}/{epochs})')

낙 AYPAWY OIE

침3 00 이 08 Wt 에 ow oh

om

~      eng Beer LEARNS”
-56- 무단 전재, 복제, 발춰, 디지털화 금지

@ |.
rol! =
nf
2
[요
4) :
b>
Ojok
ru
rz


===== PAGE 58 =====
2부. RNN                                           2.2 RNN Model Architectures

@ RNN Architectures 별 기본 코드

* many to many: stateful ( many to one + one to many ) (2)
@ Prediction: = 결과를 다음 추론의 입력으로 전달하며 반복
@ time_steps=1 이어도 상태를 유지하며 추론 가능 ( 매우 긴 ABA 처리 가능 )
 추론 시작할 때 상태를 초기화
 이전의 모든 HAS 넣어 첫 추론 시행
* 추론된 값을 사용하여 다음 추론 진행, 반복

Many to many - 2

at isl [e| | aodebceset-statesO #422 dase
년    a       predicted = model. predict (totalSequenc

firstNewStep = predicted[:,-1:] #
# 2:
output_sequence = [firstNewStep] #    3     7        ㅣ
last_step = firstNewStep                                 |
for i in steps _to_predict:
Rew Step = Sao eet Cee seep) 2 "1
output_sequence. append (new_step)   # 글
last step = new step          #*
model.reset_states() # A/H#A GA/BYOA; Af

mH

PEARS

= RNN Architectures 별 기본 코드
® 가변 ABA 학습 : 길이가 CLE dataset 처리
® inputs = keras.Input(shape=(None, data_dim))                 inpait SF Inpail apse
@ 학습과정에서 62[다단위로 A| HAI] 길이를 변동 가능

/* 단어를 학습 한다면, 단어마다 (문자의)길이가 다름

oe Ta
/ 문장을 학습 한다면, 문장마다 (단어들)길이가 다름               90250 | | 06220
이     .     a ty

[AIHA 182 shape]

~
input: / [0 7, 25)1\
output: \ (1/7, 25)) ])

® Stateful 적용 : batchZ 상태 전달, stateless= batchZ! 독립          [ AIA o}afol shapel
@ SAPS 가지 데이터 SS 학습가능                                         input: | [0,2.25)]
/* 몇 종목의 주가를 [51\/으로 학습할 때                                  input_10: InputLayer   output | (2 25)

 각 종목의 시계열을 batchS 묶고, statefulZ 상태를 연결하면,                                               :
/* 다음 82[대에서도 종목별로 고유 상태를 전달하며 학습                                    ,
+ _ 따(에서 shuffle=False 해야 종목들이 섞이지 않음                     tet 13910 | 고아 Oe 2)
A 가변 BAS 하면 일주일에 개장 일이 변하는 것도 처리 가능                           i

time_sptep=3               time_sptep=5              aos Stateless, batch=None
요일 | 월 SF sik fier Sie

= a

~

종목1 | ohlvclohive Johive johive |ohive |ohive |ohive |아1 | ~

#32 | ohivclohlive lohive Johive |ohive Johive johive Johive     Stateful, batch=3

$3 | ohivclohive johive |ohive |아1 |ohive lohlve |마1\% | -

114

.           |                     age DEER LEARN”
@한국시연구소 홍근선           -57- 무단 전재, 복제, etal), 디지털화 금지



===== PAGE 59 =====
« Ropentblewtor 6
Cbg , 60045 a Cbs, m, Feature)
22. RNN                                           2.2 RNN Model Architectures

@ RNN Architectures 별 기본 코드                  Input  Cea nence =pultpu    epee.
@ RepeatVector (layer) : LSTM 입력에 반복 값을 공급
Many to many

HHABHERERE many to many + (RepeatVector) ##é#RRRRAR             |
| |  | |  |       model. add (layers. RepeatVector (repeat times, input_shape=(data_. ain)))

model. add(layers.LSTM(output_size, return | sequences=True) )

* LSTMOl] 전달되는 데이터 shape : ( repeat_times, input_shape )
나아가
LSTM AutoEncoder 42 Oj
PHHBHHAHHAH LSTM AutoEncoder

*

1

2 latent_dim = 2                                       에
pag

3 inputs = keras.Input(shape=(timesteps, ( (data _dim)) ~ bs, Ya

4

5

encoded = layers. LSTM(latent_dim) (inputs)       「       )

decoded
decoded

layers .RepeatVector(timesteps) (encoded)
layers.LSTM(data_dim, return_sequences=Nue) (decoded)

1 1

wo

Many to many - 3                                                  meat TQ En

input_29: InputLayer capac TIT BS   \    3  cae wh
LSTA    | 【

| 35 rene Se      “Vm, ster

A

output:         (?, 2)

input: | (2,2) |
output: | (?, 7, 2) |

 repeat_vector_12: RepeatVector

|

input, | (2,7, 2)

00006 | 0.7.29| | 006 BEER EARNING”

1900..39: LSTM

0 RNN Architectures : 레이어를 중심으로               |
< Stacked RNN >                                  < Bidirectional RNN >

이 우우 우고
내

HORE

toes

< Skip connection LSTM >        < Residual LSTM >
SD FUP OS

om ,

rm       sileeeeassini      see     |             Se aie DEEP LEARNING”

한국시연구소 홍근선                   -58- 무단 전재, 복제, Sl, 디지털화 금지



===== PAGE 60 =====
2부. RNN                                           2.2 RNN Model Architectures

@ Parallel LSTM
* .레이어를 수평으로 확장 : 0312의 특성이 다른 경우                       2 parallel LSTM

1 ##### parallel LSTM ###8#                                               output

2 input_ = layers.Input(shape=(15, 26), name=’input')

3 input_i = input_[:,:,312]

4 input_2 = input_[:,:,1@:                                         Dense

5 Istmi = layers.LSTM(64, name=’lstm1’)(input_1)

6 15102 = layers.LSTM(64, name='Istm2‘)(input_2)                   an
7 concat = layers .concatenate([istm, istm2])     |    |          LsTM       LsTM
을 output = layers.Dense(6, activation='tanh', name='dense’)(concat)

9 model = keras.models.Model(inputs=[input_], outputs=output)

: | [(None, 15, 20)
eget wpatayes input: | [@None, 15, 20)]
output | [(None, 15, 20)]

tf _operators__ getitem: SlicingOpLambda                       tf__operators__getitem 1. SlicingOpLambda
ae                                         ontpat: | (None, 15, 10)

Input(1+2)
input: | (None, 15, 26)
output: | (None, 16, 10)
Ye Ze Datwrt

input | (None, 15,10)          input | (None, 15, 10)

19041: LSTM                               istin2. LSTM
optput:   (0906.64)
| 100 | [여906.640.009066.640] |
Coneatenate       +
amen! output | 여9806.28 |
input | (None, 128
dense: Dense   ss           기
output | (None, 6)
eer              ‘                                       rn          STEARNING |
117                              .                                                        SME DEEP LEARNING

8 Stacked LSTA

ㅣ #8PHS Stacked LSTM #####
2 model = keras.models.Sequential()
3 model.add(layers.Input(shape=(7, 20), name='input'        x     만스시 AES,
4 model.add(layers.LSTM(5@, activation='relu' ,( return_sequences=True)
S model.add(layers.LSTM(5@, activation="relu', neturn_sequences=True
6 model.add(layers.Dense(1))
? model.output_shape #(None, 7, 1)
Stacked LSTM
a       Pe      .             input: | [(, 7, 20)]
input: InputLayer
output: | [(?, 7, 20)]
input: | (?, 7, 20)
Istm_40: LSTM
i            a                output: | (?, 7, 50)
그           극              input: | (?, 7, 50)
레 에               00       1990 _41: LSTM
output: | (2, 7, 50)
na                   input: | (?, 7, 50)
a                7        06056 2: Dense
:                           output | @,7, 1).

@한국시연구소 S24                   -59- 무단 전재, 복제, Sail, 디지털화 금지

Er 다른 AML ST


===== PAGE 61 =====
2부. RNN                                                       2.2 RNN Model Architectures

대               -

= Bidirectional LSTM
 Bidirectional layer : RNN layers 양방향 레이어로 HStA[7|= wrapping 레이어
e  이 과거로부트  까지의 정보로 미래를 예측하는데 더ㅎ
/현재부터 과거의 정보를 살펴서 미래를 예측하는 SAS 결합

###8# Bidirectional LSTM #####                                                                     |
model = keras.models.Sequential()                                                                  |
model. add(layers.Input(shape=(7, 20), name=‘input'))                               |

내 12 bt

model .add( layers .Derise                                 |
model.output_shape #(None, 1)

wow

—

® LSTM layer 에 return_sequences=True 를 적용하면, output_shape2?

input: | [(?, 7, 20)]
output: | [(?, 7, 20)]

input: InputLayer

input: | (?, 7, 20)

bidirectional_ 16(istm_51): Bidirectional(LSTM)

input: | (?, 100)
output:    (7, 1)

dense_29: Dense

를 ResNet : Residual learning(2t} 학습)적용
매우 깊은 망을 만들 수 있는 효율적인 방식
mae

* 일반적 학습 : 160 - ) 를 최소화 하는 것                —
《 새로운 학습 SH: 잔차 학습                             stacked layers

SAD 입력의 잔차라 하고,

> 학습 목표가 명확하므로 학습이 잘될 것 이라 가정
@ AS H(x) = F(x) +×가 되고,
 그래프에 skip connectionO| 발생함
® Skip connection 의 가치
@ O|6+%, weight7} 아무리 작아도
ㅎ Gradient 7} 사라지지 않음
> vanishing 문제가 해결됨

SASL

@한국시연구소 홍근선                       -60- 무단 전재, 복제, 발춰, 디지털화 금지

output: | (2, 100)    W) naa)


===== PAGE 62 =====
2. RNN                                            2.2 RNN Model Architectures

® Residual block 구조 개선
® Conv> bn > relu> conv > bn > + skip > relu
> bn > relu > conv > bn > relu > conv > +skip
(post-activation > pre-activation )
> 1) Skip 0855에 연산이 제거됨 (backpropagationOl| 유리)
2) 844위치 변경 > BN 역할 강화

2
f            … ResNet-1001, original (error: 7.61%)
~~ ResNet- 1001, proposed (error: 4.92%)                                 ~
님                                                                                                      (a) original           (06) proposed
~ 개                               ts
02         Par     ;
3                  Nein                               g dataset | network                baseline unit | pre-activation unit
Fy                           =                         we                 ResNet-110(1layer)       9.90               8.91
더                                                        z                     Net-                    i                   :
os                                                              CIFAR-10   ResNet-110                 6.61                  37
ResNet-164               5.93               5.46
ResNet-1001)         761 . | . . 492
CIFAR-100          =                   25.16              24.3:
ResRet-1001          27.82          22.7.

m_Residual LSTM : Residual skip connections 가지는 LSTM

amare | nb | ones 7107    1 ##### Residual LSTM 06
1440.31: 0000.08 output: | [(None, 7, 10)]    2  units = 20
2 inputs = layers.Input(shape=(7, 30) )
|                 4 x = layers.Dense(units) (inputs)
input: | (None, 7, 10)     5 x_rnn = layers.LSTM(units, return_sequences=True) (x)
dense_42: Dense                             개
a       output | (None, 7, 20)      6 x= layers .add( een 000) )
? × 000 = layers.LSTM(units, return_sequences=True) (x)
WA                 8 x = layers.add([x, x 000] )
input: | (None, 7. 20)            9 x = layers.Dense(1)(x)
Istm_70: LSTM                              ape    '
—     output: | (None. 7, 20)           i@ model = keras.Model(inputs=inputs, outputs=x)

\                                                 |  Outpul())x7

imput: | [(None, 7, 20), (None. 7, 20)]
add_69: Add                                                                                   :
r=                output:                (None, 7, 20)                            Dense(i)x?

input: | (None, 7. 20)                                           |
19014 71: LSTM
i              output: | (None, 7, 20)                                 LSTM2(20)
aia S00Add    input: | [(None, 7, 20), (None, 7, 20)]
=                output:                (None, 7, 20)                            LSTM1@Q0)
input: | (None, 7, 20)

dense 43: Dense

output: | (None. 7.1)

sae

feature(10)x7

Sa a:

화 금지

Mit

-61- SE 전재, 복제, 24], Cl2lE


===== PAGE 63 =====
2부. RNN                                            2.2 RNN Model Architectures

Dense 5114 : Densely connected LSTM
® Dense Net
®@ LayerZtojj fully-
connection 구조
@ Feature-mapS
concatenate 함
 여러 수준의
feature mapO|
출력에 결합되어
반영

Dense Block 구조

:
2
:
i
i
i
:
i

고

pa Wo Y= WoXt
Lig FW

RUNS evevennsnseneery rebel sverernnnnenseh!

hax)

me.

|                     is                 _.
ee

123

@ Dense LSTM

1 #888 Dense LSTM #Htit
2 units = 20
3 inputs = layers.Input(shape=(7, 10))
4 x_rnn = layers.LSTM(units, return_sequences=True) (inputs)
5 x1 = layers.concatenate([x_rnn, inputs])       :
6 x_rnn = layers.LSTM(units, return_sequences=True) (x1)
7 x2 = layers.concatenate([x_rnn, x1])                 input_6 | input:
을 x3 = layers.Dense(5)(x2)                     InputLayer | ourput: ieee 2 이 | 1 에 그어
9 00061 = keras.Model(inputs=inputs, outputs=x3)                 WA
ere 노오 (None, 7, 10) | (None, 7.20 |
Stiri en {(None, 7, 20), (None, 7, 101] | (None, 7, 30
Concatenate | output | ===    06. 730
| 52.  나  {None, 7, 30) | (None, 7, 20)
| LSTM | output:
| cnocatenate_¢!| input:  {(None, 7, 20), (None, 7, 30)] | (None, 7, 50)
| Concatenate || output: | ㅋㄷ ====ㄷ= = = =      0
서애] 때 | Clone, |
Dense | output:

@한국시연구소 홍근선                       -62- 무단 전재, 복제, Yall, 디지털화 금지



===== PAGE 64 =====
2부. RNN                                            2.2 RNN Model Architectures

@ “Densely Connected Bidirectional LSTM with Applications to Sentence Classification”,
2018

[ Stacked Bi-LSTM ]

r- Seft-max

r Average Pooling

> Dense Bi-LSTM

+  Network Inputs

® “THU NGN at SemEval-2018 Task 3: Tweet Irony Detection with Densely Connected
LSTM and Multi-task Learning”, 2018

Word POS
Embedding Tag                                             ge Btttennnen,
a                 te
E,          이 ~                   mae
ㅣ >                                     naw Ee             a
love +]                                                  a
exams»                                      ox

Embedding    psism "1 gusty 42 94.504 43 sitstm

Layer     Layer    Layer    Layer    Layer
비게      NNR
@한국시연구소 홍근선        -63- 무단 전재, 복제, Wall, 디지털화 금지


===== PAGE 65 =====
2부. RNN                                           2.2 RNN Model Architectures

® “DENSELY CONNECTED PROGRESSIVE LEARNING FOR LSTM-BASED SPEECH
ENHANCEMENT”, 2018

(a) Noisy
1
1
1
|
1
1
1
|                                               06) Clean:
1
Fy 1 ㅣ
eid
sit
Bit
= ㅣ                        숙고 layers
a :                                                 (a) PL
244
it
1 ㅣ
it |
ae
iby
a8 |       ~  ant an ~ ~ <a oe os
i 1
[대고                                            (0 PL*Dense
1
iia
1 | {
vv
Input (noisy speech, one frame)
nent : Data copy

붕이    지지자
| 2.2 RNN Model Arch

@ “The CAPIO2017 Conversational Speech Recognition System’, 2018
@ bLSTM : Bi-directional LSTM Layer

hf aoa 00 SSR Ta
~        LSTM
.          Residual LSTM
>       ~~ Dense LSTM (S/ block) |
&              Dense LSTM (10 / block) |
5 254 [                    2
를 IR               /
을 | |             호
220} & wt
17.5          a
16
15                                                         |
1       5        10       15       20       25       30
Number of LSTM Layers
128             “                                                     ：              4A

@한국시연구소 홍근선                    -64- 무단 전재, 복제, SH], 디지털화 금지


===== PAGE 66 =====
2부. RNN                                             2.2 RNN Model Architectures

= Sequence to Sequence (seq2seq) 모델
Oo      hon
© (Many to one) + (one to many)            C we Re   4, )
© 입력 AJBWAS 단일 벡터로 ODS (hidden state & cell state )
@ 인코딩 값을 디코더 초기값 에 전달
@ ‘return state=True’ : 마지막
Checeder 35

@ 단일 벡터를 출력 AlaAe 디코딩                                                ;
@ AHA BAS 다음 time step 입력으로 전달   ie value + 6057 UW

® Ｌ3094896모델에서 자주 사용 : 번역, 문장의 의미를 6ㅠㅇ00109한 후 새로운 문장 생성

many to one: Encoder     _ one to many : Decoder

® seq2seq 모델 : encoding vector = 20 = #of encoder unit

#H##F Seq2seq ###HH

units = 26

e_inputs = keras.Input(shape=(None, 10) )

#enc_LSTM, _h, _c = Layers.LSTM(units, return_state=True)(e inputs)

enc_LSTM  ayexs.LSTM(units, return state=True, name="enc”)
enc_out\ 0, o¢  nc_LSTM(e_inputs)    ©Woderet 0

ik RO be

Rw 으

7
8 d_inputs = keras.Input(shape=(None, 10) )
© dec_LSTM = layers.LSTM(units, return_sequences=Tfue, name="dec")
316 dec_out = dec_LSTM(d_inputs, initial _state=[_h, _c]) ##24; = -##
11 output = layers.Dense(5)(dec_out)
12
13 00061 = keras.Model(inputs=[e_inputs,d _inputs],outputs=output)
-    Eas   input | [(None, None, 10)]
® Sequence(time_steps)S           PL ERAS 기이
None aff 하나?                                                |
어떤 차이가 있는지 설명해 보자. ㅣ, |         (None, None, 10)          was mange  14006 | (None, ear
output | [(None, 20), (None, 20), (None, 20)       me wn oor Fee | output: | [None None. 10}]

a

input: | [(None, None. 10), Nove, 20), (None, 20)]
ontput                   (None, None. 20}

|

input | 여여6.230006. 20)
output ㅣ (None. None, 5

130      pie  :   com       Sf DEEP LEARNING”

@한국시연구소 홍근선      -65- 무단 전재, 복제, wall, 디지털화 금지

dec: LSTM

dense: Dense



===== PAGE 67 =====
2부. RNN                                    2.3 RNN Model Design (Time Series)

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNING
RECIPE FOR YOU

m Keras.layers.LSTM(GRU) API Review

tf. keras. layers .LSTM(

대                                                                  /     2
units,                                   Bao He

none fF? Leiner
recurrent path HAE?

use_blas=True,
kernel_initializer="glorot_uniform”,
recurrent_initializer="orthogonal",
bias_initializer="zeros",
unit_forget_bias=True,

ry

True: R74 3A4/ forget 9060 1 Fz
kernel F FEE 11,42
recurrent kernel @ FELHE 11,12

recurrent _regularizer=None,
bias_regularizer=None,
activity_regularizer=None,            BYY FRE 1,12
rernet & YSHE WYRE

recurrent kernel **

bias_constraint=None,
dropout=¢.e,

recurrent path] FEE ㆍ

서서 ioe oan soe woos               ~

go_backwards=False,
stateful=False,

True: input seq. S 7¥.
True: batch Al i HH 6

True: in,out shape [timesteps, batch, feature]
BPAY] BOF -> SEA (BL seq. 9 FE)

time_major=False,
unroll=False,
**kwargs

^"
mp
“3
그
iD
내
io)
‘2
고
wn
ae
ay
my
ne
wa]
ed
Lis
=
6
고
시
ee RE RRR EER ER ER ER H RH RH HR HH
;

@한국시연구소 홍근선                    -66- 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 68 =====
2부. RNN                                   2.3 RNN Model Design (Time Series)

% Time series 24-3 통한 RNN Model Design 이해
m [실습 1] Stock prediction
Forecasting(AlZ! 개념 필요) vs. Prediction(4t?| 개념)
 실습 개요

ㅎ 20년 간의 주가 정보를 이용하여 주가 예측 modelS tf.keras= 구현

ㅎ Ｌ5114 RNN layeré 하나 갖는 basic model 구현

@ Stacking, Residual, Dense LSTM model ……   $\  600   Aran    성  .

ㅎ 7일치 주가(아100)로 RNNS training      gos | — Pred Se ce A
* 주가 정보를 읽어 들여,                     090
* 주가(아100)를 1(6314165로
/* 7일치 단위로 41016 56065를 생성하고,

8일차 종가(0)를 13[9하으로 설정

/*＊ Ｌ514으로 모델을 훈련

@ Prediction

“Ga 주가를 way 여                          ~
/* 8일차(다음날) S71(0)S prediction   더

675

Normatized Stock Price

e
&

ONO Oo     a    100    200    ane    ae    ao
© 입출력이 숫자                              때
@ Regression 문제 임
 모든 숫자를 00「008126하여 사용                          7
뼈             —      rere Beer ies

fi              es      “4            fe
=u)                        (     Open High Low Close Volume Change
a Data 56Ｌ[준비하기                           bate
:    :       =      ae               2000-01-04 6006 6112 5660 6118 1483967 9.148496
그 # bttps://github.com/FinanceData/FinanceDataReader     2080-01-05 5800 6060 5528 5580 1493604 -0.086743
2 1010 install finance-datareader                  2000-01-06 5750 5780 5588 5628 1087810 0.007168
2000-01-07 5560 5670 5360 5540 806195 -0.014235
2000-01-10 5680 5772 55806 5772 937615 8.841516,
Open  igh        1   E
1 import FinanceDataReader as fdr               Sate    Geen tee 0
2 #pd_data = fdr.DataReader('KS11', ‘2006-@1-@1') # KOSPI/| 2024-04-08 85200 86000 34509 84500 18953232 0.000000
3 # Samsung(0@5930)                            2024-04-09 34588 84900 83100 83600 23725956 -0.010651
=           ‘    - 5   aa ads       2026-04-11 83200 84700 82500 84102 25538809 2.005981
i as eae fdr DataReader (005930 + 2000-01-01')       2024-84-12 84708 84908 83200 83700 1706177@ -2.004756
5 _pd_data.head() ,pd_data.tail()                   2024-04-15 82900 83200 61200 82200 26110522 -0.017921
트
@ Change rate 특성 확인
Min:@.@@0, Max:@.150
Abs _Mean:1.52%
Mean :8.064
Std dev:2.13%                        Open      High      Low     Close    Volume    Change

Mean without max values:1.41%
count 6008.000002 6000.000000  6000.080000  6000.000000 6.000000e+23 5999. 008000

Standard deviation: 2.1% / 4.3% / 6.4%   mean 29239.754000 29523.789167 28943.209667  29255.695800 4.416800e+06 0.008631
250 +     a  std  22904.099624 23084.147197 22704.894822 22879.538665 7.854231e+06  0.021346
200 4         !           nin   8.200008  8.020008  0.000006  2730.000000 0.000000e+08  -0.137566
150                        253 11060.000000 11220.000000 10960.000006 11100.000000 2.943073e+05  -0.010792
100                        50% 22870.000000 _23100.000000 22590.000000 22910.000000 5.041160e+05 9. 008000
=.                         75% 46350.000000 _46800.000000 45900.000000 46285.000008 6.608643e+06 0.011545
                  !   , || 60 90300.000000 96800.000006 89500.000000 91000.000000 9.030618e+07 ㆍ 0.150000
-15                 10   15

@한국시연구소 홍근선                    -67- 무단 전재, 복제, S4ll, 디지털화 금지


===== PAGE 69 =====
2부. RNN                                     2.3 RNN Model Design (Time Series)

* Data 전처리
@ ‘0’ value 처리

1 pd_data[‘oOpen'] = pd_data[ “Open” ].replace(@,np.nan)
2 pd_data[ ‘Open’ ]=pd_data['Open‘].interpolate()

[제

@ Normalize                           ian

1 #88 ScaleHe 정규화 하기 sat                  02

2 def MinMaxScaler(data):

3      min = np.min(data[:,:4])                    ia            ‘    :    +    }
4      max_ = np.max(datal:,:4])                       가르
5     data[:,:4] = (data[:,:4] - min_) / (max_ - 016 ) # ohlc price
6     data[:,4] = (data[:,4]-np.min(data[:,4])) / \

?                 (np.max(data[:,4])-np.min(data[:,4])) # volume

8      return data

@ Sequence data build

2 #8 ※×:7일치 데이터, 1:8열자 종가

3 timesteps = seq length = 7

4

5 datax = |]

6 dataY = |]

7 for i in range(@, 160(\) - seq_length):

8      _x = x[i: itseq_length]          # 6-62 테이터(0~6)

9 #   _y = x[i+1: i+seg_length+1,3]    # 3~7일 종가
310     _y = ×[1+500 length:i+seq_length+1,3] # 7일차 종가
11                dataX.append(_x)

테:              datay. append(_y)

m Sequence(sample) generator : Data sequence build
@ RNN data(time-series / sequence) shape : ( samples, timesteps, features )
@ x: 7일치 data(ohlvc)7} 하나의 sample : ( ?s, 71, 5f)

®@ ”: 8일차 종가 : (2s, 1f)
1 time_steps

® Split test data

14 # train data : test data=9: 1

15  train_size = int(len(datay) * @.9)

16 test_size = len({datay) - train_size

17 x_train = np.array(datax[@:train_size])

18 y_train = np.array(datay/0:train_size])

19 x_test = np.array(datax[train_size:len(datax) ])
20 y_test = np.array(datay[train_size:len(datayY) |)

time_steps(7)

[x_train] Shape(4537, 7, 5)
[y_train] Shape(4537, 1)

[x_test] Shape(se5, 7, 5)                              때
{y_test] Shape(5@5, 1)                                    Features(5)

@한국시연구소 홍근선     -68- 무단 전재, 복제, Wal), 디지털화 금지



===== PAGE 70 =====
2부. RNN                                     2.3 RNN Model Design (Time Series)
N

= Model_B : Basic Model define                                         모델의 정적 표현

Output(1)

= Sequential model
@ keras.models.Sequential 사용                                                                               7

@ keras.layers.LSTM API 사용
@ units: hidden_dim=10 > LSTM output dim
@ Input_shape=(x_train.shape[1], x_train.shape[2]) >

@ Dense layer                | [x_train] Shape(453X 7, 5)
@ Units = 1: LSTM 출력(100107)을 받아 종가를 예측     Sox
® Activation function: default = None(linear)              (0 ‘Ss

모델의 동적 HA(many to one)         a

1 hidden_dim = 10
2 ##8# Basic LSTM model                                                 2   x
3 #basic model = LSTM + dense                                   |    |
4 00061 8 = keras.models.Sequentiai(name='model_basic')                       ee
5 model_B.add(keras.. Input (shape=(x_train.dhape[1], x_train.shape[2]))) [:   4
6 model_B.add(keras.layers.LSTM(units = hidden_dim))                      {   {         {
? 00061 _B.add(keras.layers.Dense(units = 1))                       이      yy iy
  EB     > >
Total params: 651                               =  =     = |=
Trainable params: 651  [=|     를 -
Non-trainable params: 0                            ||  | 9|     | 의  | 이      °
a 48     & 46 8 6
emt et       en          네스     ,        =     Ax DEEP LEARNING”

X Model_S : Stacked LSTM                                             모델의 동적 표현
a (LSTM) * 3 + dense

##8# Stacked model: stacked LSTM
#Stacked mode = {LSTH) * 3 + dense
model_S = keras.models.Sequential(name='model_stacked')
model_S.add(keras.Input(shape=(x_train.shape[1], x_train.shape[2])))
# LSTM Layer 1,2,3
model_S.add(keras.layers.LSTM(units = 18,
model_S.add(keras.layers.LSTM(units = 16,
model_S.add(keras.layers.LSTM(units = 1¢))
# dense

model S.add(keras.layers.Dense(units = 1))

~ 저기 지기 에 UAE eh

~
oo oO ow

@ ‘return_sequences = True’
@ 각 A/HAOA S43 리턴 함
# Many to many 구조를 형성

@ Many to many + many to one
> many to one

LSTM(10)

Total params: 2,331
Trainable params: 2,331                    a
Non-trainable params: @        모델의 정적 표현 | feature(5)x7_

138                                                       fara             :
@한국시연구소 홍근선                      -69- 무단 전재, 복제, tal), 디지털화 금지



===== PAGE 71 =====
2부. RNN                                    2.3 RNN Model Design (Time Series)

checkpoint_path = "./aicamp/cp.weights.h5"

% Model Compile & fit                      :

2 epochs =

100

를 Basic model                             3  batch_size = 64
2 opt = keras.optimizers.Adam{learning_rate=0.¢e5)
3 model 8.compile(optimizer = opt, loss = ‘mse’, metrics=(|\mape’/)
4
5  my_callbacks = [keras.callbacks.ModelCheckpoint(filepath=checkpoint_path,

save weights only=True, save_best_only=True), ]

6

?

8 history_B = model B.fit(x_train, y_ train,

3                           validation data=(x test, y_test},callbacks=my_callbacks,
2                     epochs = epochs , batch_size = batch_size)

m Stacked model
opt = keras.optimizers.Adam(learning rate=0.005)
model _S.compile(optimizer = opt, loss = ‘mse’, metrics=|‘mape‘ |)

[keras.callbacks.ModelCheckpoint (filepath=checkpoint_path,
save weights only=True, save_best_only=True), ]

history_S = model_S.fit(x_train, y_train,
validation_data=(x_test, y_test),callbacks=my_callbacks,
10                     epochs = epochs , batch_size = batch_size)
11. model S.load weights(checkpoint_path)

® loss: loss 함수 지정 > ‘mean_squared_error (=‘mse’)

: value2| 차이를 구하는 것이므로 055 entropy 쓰면 안됨     ¢ APE = baad x
* MAPE : 직관적이나, 정답이 0에 가까울 때 너무 커짐                       "

2
3
4
5  my_callbacks =
6
7
8
9

139

TestData[:100}

@ Prediction                                 gcc
1 # Test SA 시작 100일                      # ose
고 50 = -6                                                 z 0.56
3 호    = 100                                                8
4  ne x_test[s_p:e_p!                        5 os
5 Y= y_test[s_p:e 0]                                     ose
6                                                                 0.50                                   1
7 #plot_predict (X,Y, "TestData[@:100]")                   .         20         bes        a        100
8 plot_predict({model_$,X,Y,title="TestData[ :100]",names=[ ‘True’, ‘Basic’, 'Stacked'])
1 history_n = [’Basic’, 'Stacked’]
2 colors=['green','blue','red’]
3 def stock _plot(prices,title="",names=[]):
4         pit.figure(figsize=(8, 4))
5         for i, pred in enumerate(prices):
6                  plt.plot(pred,color=colors[i], label=names[i})
7         pit.title(title)
8        plt.xlabel('days')
3         plt.ylabel('Normalized Stock Price’)
18           plt.legend()
11           plt.grid()
12           plt.show()
43           return
34
15 def plot_predict(model,X,Y,title,names):
16      pred_price B = model_B.predict(X, verbose=@)
417    pred_price_o = model.predict(X, verbose=@)
38        stock_plot({Y,pred_price_B[:,-1],pred_price_o[:,-1]],title,names)
"140°  319      return                                                                i         a0       PE DEEP LEARNING |
한국시연구소 S24                     - 70 - 무단 전재, 복제, Bll, 디지털화 금지


===== PAGE 72 =====
2부. RNN

2.3 RNN Model Design (Time Series)

Wor +o OW"

—

8 실습과제
v 과제 1. timesteps = 580 length = 7를 줄여보자

odel   A 53,12 줄이고 Aas 비교하자:       ey, 벽꺼 시  함미  weve saat
—model_BOJlAj 53,12 줄이고 Bays 비교하자:        Cha he Tilt & 20

ㆍ 과제 2. model_SB 개선하여 model_S2S 만들어 보자
ve     Do 7%
~ 개선할 수 있는 BES 생각해 보자    시  \"Jey  4 \   적.

~ LSTM layer 주가?

Abe woods Te

RK REmje    tegen
~ Dense layer 추가?                                                                               Tole                           사나

~ 과제 3. LSTMS Dense layer2 교체한 model& 만들어 보자             BB  buyper    yorameten

-성능을 비교해 보자
~ 과제 4. Basic 010061에 Bidirectional LayerS 적용하고, ASS 비교해 보자
~
°        wt
1) Bidrectionnla Layer@ LSTM layerS 감싸서 구현하자.           10 2+ Oye   =) 4 yah  0

2) return_sequences = True 로 HASH 어떻게 될까? 결과를 검토 해보자                  =)  Ye 씩      htt ㆍ
3) LSTM, Dense 사이에 Flatten layerS 넣으면 어떻게 달라질까 생각해 보고, 결과도 확인하자

과제 5. 7일치 B7-S Targeto 2 하는 many to many model2 수정해 보지
war to worg 과제   일치   [를 189    하    y     y      수정해   }

- 과제 4에서 사용한 SAS 수정하자

~ 과제 6. 과제 5에서 Bidirectional layerS stackingstZ, 성능을 비교해 보자

2

개

“Sf DEEP LEARNING”

[ LSTM model 입출력 ]
8

Mey
%y

Dense(S0)

Features(5x7)

이

-71- 무단 전재, 복제, etal, 디지털화 금지


===== PAGE 73 =====
2부. RNN                                   2.3 RNN Model Design (Time Series)

과제 7. Indicators Al Al SO] 추가하여 SSS 개선해 St At.(SBmape 0.40] s+)

~ hidden_dim 늘리기

- 과제 6에서 사용한 BAS 수정하여 ASS 높여보자 (Add_Indicators. ipynb fileS 사용하여 과제 진행)

30 그

10                     10                 10° 7+"

1075 4

~ stack 늘리기
- &, 뒤에 Dense 추가하기
02
~seq_length 늘리기 ye    {argh At ony ez]
~ learning rate 수정하기                                                                                  5          ;
sBlL Fuarcow|eru) &
Training loss                                     validation loss                    validation mape((B:0.485)(B2:0.297)
~ ss B | 1073 4          |             ~ \31.10558
… 1055.82  val_lossB2

9            20          40           60          806 100                   9           20           40           60          80 100

% Model_R : Residual LSTM : (Residual LSTM) * 2 + dense
i

###8# Residual LSTM ###8#
2 units = 10
3 inputs = layers.Input(shape={x_train.shape[1], x_train.shape[2]))
4 x = layers.Dense(units) (inputs)
5 x_rnn = layers.LSTM(units, return_sequences=True) (x)
& x = layers.add([x, x_rnn])
? x_pnn = layers -LSTM(units, return_sequences=True) (x)
8 x = layers.add([x, x rnn])
9 x = layers.Flatten()(x)
16 x = layers.Dense(1)(x)
11 00061 8 = keras.Model(inputs=inputs, outputs=x,name="model_residual")

모델의 정적 표현

106056(1)

70

LSTM2(10)

Total params: 1,811

Trainable params: 1,811                                    [Dense(1) |

Non-trainable params: 0                     2  개
|          Flatten          |

모델의 동적 표현

으으                     =                                                         ss

LSTM1{10)

Dense(10)

@한국시연구소 홍근선

Lot oA.



===== PAGE 74 =====
2부. RNN                                   2.3 RNN Model Design (Time Series)

8 Model_R: Residual LSTM                                            이
input_43: InputLayer              -
output: | [여0066. 7. 5)]
Model: “model residusl”                                                        |
input | (None, 7, 5)
Layer (type)               Output Shape       Param #    Connected to              dense_S0: Dense  output: | QNone. 7, 10)
input_43 (InputLayer)        {{None, 7, 5)]     8                                  rd
dense_5@ (Dense)           (None, 7, 18)      66       input_43[@][@]    istm 98: LSTM  때만 | (None, 7,18)
~       output | (None, 7, 10)
Istm_98 (LSTM)            (None, 7, 10)     840      06058_50[01[0]
300 30 (Add)           (None, 7, 10)     @      06058 _50[01[01               : | [(None, 7, 10), (None, 7, 10)
'              '              lstm_9g[@] [ei       add_30: Add =  Gone, 7.10)
Istm_99 {LSTM)                  (None, 7, 10)        848         300_30[01[0]                           WA
300_ 31 (Add)             (None, 7, 10)     @       add_3@[@] [0]     tit: 90: 가 | Nome 7: 10)
Istm_99[@][@]               output: | (None, 7, 10)
flatten_13 (Flatten)         (None, 70)        8        add_31[@][8]                   “he
input: | [(None, 7, 10), (None, 7, 101]
dense_51 (06056)           (None, 1)        res       flatten_13[@][8]       add_31: Add  output      (None, 7,10)
Total params: 1,811                                                                   |
Trainable params: 1,811                                                               nae      aa
Non-trainable params: @                                                              아바나 13 Walter oe   Wone, 7,
©       output | (None, 70)
input:   lone, 70)
dense SL: Dense       a    -
output: | (None, 1)
145

3X Model_DR : Deep Residual LSTM
m (Residual LSTM) * 4 + dense

1 #### Deep Residual LSTM
2 def residual_lstm(inputs, rnn_units, rnn_depth, rnn_dropout=6.9):
3      x = inputs
4      for i in range(rnn_depth):
5          x_rnn = layers.LSTM(rnn_units, dropout=rnn_dropout,
6                              return_sequences=True) (x)
?          x = layers,add([x, x_rnn])
8      return x
9
18 units = 10

11 inputs = layers. Input(shape=(x_train.shape[1], x_train.shape[2]))

2 x = layers.Dense(units) (inputs)

13 output = residual _Istm(x, rnn_units=units, rnn_depth=4, rnn_dropout=@.1)
14 output = layers.Flatten() (output)

15 output = layers.Dense(1)(output)

16 model DR = keras.Model(inputs=inputs, outputs=output,name="model residual deep")  as

Total params: 3,491
Trainable params: 3,491
Non-trainable params: 0

-73- Sit 전재, 복제, Si, 디지털화 금지



===== PAGE 75 =====
2부. RNN                                    2.3 RNN Model Design (Time Series)

3% Model_D : Densely connected LSTM : (Dense LSTM) *3 + dense   wag  “te 우럭

inper@ | input:

1807.38 | son 7, |         ##8## Dense LSTM #8##8
re                                          units = 10

ral                               |       inputs = layers.Input(shape=(x_train.shape[1], x_train. shape[2]))
100 [moe | fone, 7,5) | om 테 |                    i       x_rnn = layers.LSTM(units, return_sequences=True) (inputs)

쩌 = layers concatenate( [x ran inputs |)

x_rnn = layers.LSTM(units, return_sequences=True) (x1)
x2 = layers.concatenate([x_rnn,x1])

x_rnn = layers.LSTM(units, return_sequences=True) (x2)
x3 = layers.concatenate( [× 008 2X2] )

ao 19004. 7, 10}, (None, 7,53} | None, 7,15) |

04 | 08               0
eee (None, 7, 153 | 000. 7, 10) |

roncatenaie_t | input:

OO 세어 Ww & WN 에

x3 = layers,Flatten() (x3)
xo = layers.Dense(2)(x3)
model D = keras Model (inputs=inputs, outputs=xo,name='model dense’)

see 7,105, 0007.58 | om 72

Layer (type}                Output Shape        Param #    Connected to
6                             E                          a
ber iT 롤`                  1               input_6 (Inputtayer)        [(None, 7, 5)]     60        {}
iste           (None, 2, 25) | eee 7, 10 I
a                              Astm_13 (LSTM)            (None, 7, 18)      649      [ ‘input_6[@][@]}*]
cocina ome                       ; | concatenate_3 (Concatenate)   (None, 7, 15)      8        {'Istm_13[0][@]’,
ss     ;      4 {(Noue, 7, 1 om 725 | an 7.38 i                                                         *input_6{0][@]°]
Astm_14 (LSTM)            (Hone, 7, 10)      1848      [ ‘concatenate_3{@][@]}°]
:  S    i (No, 7.35) | en, 245 |        concatenate 4 (Concatenate)   (None, 7, 25)      e        [istm_14{0][@]’,
3002 ouput:          i                                                                          ‘concatenate _3{@}[@]"]
았       !                     1lstm_15 (LSTM)             (None, 7, 18)      1448      [concatenate _4[2][@]‘]
 가 레티 Pend (Nowe, 245) | (None, 15 |
Dense | ouput:                        concatenate_5 (Concatenate)   (Rone, 7, 35)      @        [‘istm_15fe][e]",
‘concatenate _4[83{6]']
Total params: 3,366               flatten_3 (Flatten)         (Nane, 245)       e        {*concatenate_5[@][@]‘]
Trainable params: 3,366
Non-trainable params: 0            dense _7 (Oense)            (None, 1)         246       [‘flatten_3[0][@}"]}

147

ae ee

Kiyo BE

X€ Model Compile & fit

2 opt = keras.optimizers.Adam(learning rate=0.0905)
3 model _R.compile{optimizer = opt, loss = 'mse', metrics=/'mape’])
4
5  my_callbacks = [keras.callbacks .ModelCheckpoint (filepath=checkpoint_path,
6                    save_weights_ only=True, save_best_only=True), ]
Z
8 history_R = model R.fit(x_train, y train,
대                                                       validation_data=(x_test, y_test),callbacks=my_callbacks,
18                     epochs = epochs , batch_size = batch_size)
11 model_R.load_weights(checkpoint_path)
& History plot
1 titles=["68" "kh" |
2 pit_history([history B-.history,history R.history],titles)

Training 1055                                   validation loss                    validation mape((B:1.372)(R:1.398)

~ loss B                     —— val_lossB
nome loss R                     —— val_lossR
lo?                                                                                                     x 10°
1073 4-4     i      —      +

x 10°

1073 4

x 10°

+                                           y                            T                     ㅜ              ㅜ              t              +              t              T                                    T              +              t              t              T

0      20     40      60     80     100          0      20      40      60     80     100          0      20      40     60     80
a ee                        ee        “     SSS                   e     LLL           ee

@한국시연구소 홍근선           |          -74-
+ C6 p LSTA [계시

Mies:

단 전재, 복제, Sal, 디지털화 금지

—>-o


===== PAGE 76 =====
2부. RNN

2.

3 RNN Model Design (Time Series)

pee

. 실습과제

~ 과제8 : Technical indicators 추가하고, 개선된 모델에 적용하여 최고의 결과를 얻어 보자

1) 가능성 있는 모델을 선택하

2) Add_Indicators.ipynb

고하여 모델과 datas 준비하자.

3) 모델의 구조, 크기,16301179_1316를 최적화 하자.

3.1) hidden_dim 늘리기
3.2) stack 늘리기

3.3) 앞, 뒤에 Dense 추가하기

4) seq_length 를 7, 14, 21, 35 로 수정해 보자.

5) Learning rate SchedulingS 적용해 보자

149

0.010         i ExponentialDecay step
0.009 +     ae           ^ 시 ASR .
0.008 4      로
을
0.007 +     Foca men
0.006
0.005
val_mape
none                                                                                                                  val_loss                                       (B:0.396)(D0:0.328)
~ B
+                         1073 4
8      20      40                                                eee
1073
30           ae”            rot A [|   i
20°5                           a                 내  i
10%       |        !                  +
0 2 40 60 80 100 6 20 4 60 80
181 0182
val_loss         (B:0,356)(DR:6.291)  04 27/ /s |
we
to?           ^
10-4                 10
10°5   Wy         wh
SEAT        8                               dull                         i                     Hi
150                        9   20       60   30   100     o   20   40   659   80   109     요   20   40   60   80   300 _
=                           _   . a             =       하 그
@한국시연구소 홍근선                        75- 무단 전재, 복제, 24], 디지털화 금지


===== PAGE 77 =====
2부. RNN                                     2.4 RNN Model Design (Char-RNN)

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNING
RE        FOR YOU

Ciee

,           he
Me  Wwe
수   1

\ 시퀸스처리 RNN Model Design(Char-RNN 모델을 통해)

실습 2] Char RNN 모델 설계
m Char-RNN 모델 : 문장을 학습하여 새로운 문장을 생성 하는 모델

m 개요 : 1802} 길이의 문장으로 RNNS training         #3) Poke UI
® 주어진 문장으로 char sequences 생성하고,                         이 106 주
* Ｌ5114으로 모델을 훈련 시킨 후,                                   Deowtedt WHE
@ 10개의 임의 SAS seed sequence= 하여 11번째부터 연결하여 170749] 문자를 예측
a 입출력이 문자                                                      wy A BLT
® Classification 문제 임                                                onthe  3}
@ 2S one-hot coding 해 야함                                         *       때

※ 4가지 모델을 설계해 봅니다.

@ Model-1 : many to one               #10개의 입력문자로 다음 1개의 문자 예측
@ Model-2 : many to many               #10개의 입력문자로 각각의 다음 문자 1074 예측

@ Model-3 : many to many + stateful _ #62[대단위로 state 초기화 하지 않음
®@ Model-4 : many to many + stateful + batch_size=2_ # ~ + 개의 batch 사용

152

«J DEEP LEARNING”

@한국시연구소 홍근선                     -76- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 78 =====
2부. RNN                                         2.4 RNN Model Design (Char-RNN)
2.4RNNI

= Model2| 기본 구조
© YH: one-hot coding£! 10개의 문자열
® Shape: (samples, timesteps, features)
(sample
® LSTM layer : 75개의 unit                     모델의 동적 표현
© Dense layer: LSTIMBHS 받아서 25개 출력
® Activation : softmax func. 사용

/@ Classification 2A] 이므로 확률로 변환

7 Loss func, : CrossEntropy 사용
LOL NIN pre

모델의 정적 표현

one-hot encoded Char

2
3            "collect wood and don't assign them tasks and work, but rather =
4            “teach them to long for the endless immensity of the sea.")     ㅣ

© BAO] 포함된 문자를 숫자로 mapping
@ 4 문자가 숫자로 변환 > 문자 indexing

i
2 char_set = list(set(sentence)) # char set 장상
3

CHARACTERS:
25
DICTIONARY:
25

{y's Oy “es aa 0 나가 4, “erg 5, “ais 6, “hs 7. “ets B, “ws; 8, “Ke ey. Ses T1, ‘ws 12,

33. 4 1, “Ee aS, 1016 36, PF) 27, TBS BL ANT SO, ‘ats 20. “gts ee. 4 .%c! Be. Ys 28, 8) ah
@ 변수 설정                                                   lo
~          —
i data_dim   = len(char_set) # train data X:input   2M Ae4  BIA   OWe-    ay
2 num_classes = len(char_set) # trian data Y:target
2 sequence_length = 10       # any arbitrary number
& features = 1              # X,Y index

@한국시연구소 홍근선                        -77- 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 79 =====
2부. RNN

2.4 RNN Model Design (Char-RNN)

mw StS Sequence 생성
® Input sequence: dataX[ ]
@ 107] 단위로 2S sequence 생성 > 170 sequence

® Target sequence: dataY[ ]
® datax[1:] + next char

i dataX = [] # input sequence List
2 dataY = [] # terget sequence List

f

# we will make 17@ sequences

for i in range(@, len(sentence) - sequence_length):
# 20 characters = 1 training sequence
x_str = sentence[i : i+sequence_length]
y_str = sentence[iti : i+sequence_length+i]
# convert x, y str to index(int)

18      x_idx = [char_dic[c] for c in x_str]

il      y_idx = [char_dic[c] for c in y_str]

12      # append to dataset List

：            dataX.append(x_idx)

14      dataY.append(y idx)

OW ON Dw 와 Ww

X:f[if you wan], Y¥:[f you want]                  tor
117. 7. 9, Os 23. by 9s 22 Sy 4] © 17, 9. Gy 23. Gs Ss 고. 5, 4, 24]
X:[f you want], ¥:[ you want J

17, 9; ©, 23, 6, 9, 2, Sy 4, 24] = 19, 0, 23, 6, 9, 2s Sy 4, 24, 9]

F
uw
Ul

Serer

Sequence 를 tensor= 변환

@ One-hot coding 사용시
@ Input tensor : x 2} Target tensor: 를 모두 one-hot coding
/* × shape: (170, 10, 25) ndarray, y shape : (170, 25)
@ keras.utils.to_categorical APIS 이용하여 one-one hot coding 변환
/* numpy.array APIS 이용하여 listS array= 변환

# input tensor YY
X = np.array(dataX)      # ndarray(170,1@)<-{178,16]

## One-hot coding : 3d List [176,18,25] <- 2d arrary (176,10)

= np.array{sequences) # ndarray(170,10,25)<-[170,18,25]

Traget tensor YY

Dé

Y = np.array(dataY)[:,-1] # datay%A/ Of4/2' 운사, (176, )<-[170,10]
¥

ig

[keras.utils.to_categorical{y,num_classes=data_dim) for y in Y]

= np.array{Y)          # ndarray(17@, 25)<-{170,25]
® Compile(loss=‘categorical_crossentropy’) A
=) Abgayn\ chou
Qwe st ,            mse —
2 P

(eget

al - 40 (4d.

@한국시연구소 홍근선                       -78- 무단 전재, 복제, al], 디지털화 금지


===== PAGE 80 =====
2부. RNN                                        2.4 RNN Model Design (Char-RNN)

® One-hot coding 사용하지 않을 AS
© Model 입출력 Zk(samples, targets)2| type : ‘ndarray tensor

@ One-hot coding 을 사용하지 YOO features = 1 (index)

# input tensor 2/4)

X = np.array(dataX) # ndarray(17@,1@)<-[176,1@]

X = np.reshape(X, (X.shape[@L, xX. shape[1 1. features ))
print (X.shape)      # (176,10,1)

# Target tensor 장상 # ndarray(176@,18,1)<-[170,10]

Y = np.array(dataY) # (176,18)<-[17@,1@]

Y = Y= np.reshape(Y, (¥.shape[@],Y. shapel ii fasiures))

Ww 00 기 07 uw Be WwW oN pe

Y1 = np. array(autey [ yet]  # 주 @APED, (170, )<-[176,16]|| (170, 10, 1)
Yi= np.reshape(Y1,(Y1.shape[@],features)) # (17@,1)         (178, 1@, 1)
print _(Y1.shape)     # (176,1)                         (170, 1)
@ Y,Y1 shape , X:(170,10,1)
@ Y:(170,10,1) : many to manyO|A] 사용
@ Y1:(170,1) = many to 006에서 사용
® Compile( loss='sparse_categorical_crossentropy’) 사용 & & Swed we 본 ,
+ 입력 Z(samples, targets)Oll 1006×값을 직접사용
~ x shape: (170,10, 1) ndarray, y shape: (170,1)
@ 1006×값이 2 경우 메모리 소비를 줄이기 위해 필요

er
>

Er
es

157 .    베                   St DEER LEARNING

xshape He| x
® List 2} ndarray(np.array) 표현 : np.arrayE n-dim HAE 가짐

A                 |

4 list_ = [1,2,3,4,5]    | 42 na = np.array([1,2,3,4,5])

2 print(list_)        | 고 print(na) &      '

3 list_          | 3 na
=
{1, 2, 3, 4, 5             12345       |

  ?  >  ]           Ｌ       ]           a       아그게  130)
ft, 2, 3, 4, 5]         array([1, 2, 3, 4, “s)) <8               iad

/* Vector 표현 : (1,2,3)
/* 행렬표현 :[123]
/* Ｌㄴ19 표현       +1123]
/* ndarray 표현 : [1 2 3] or array([1,2,3]) > array( 1191 )로 BAS
@ shape: n-dim 행렬의 shape : 14016( , )로 표현 , 값이 하나면 (0,)로 표현

4 list_ = [1,2,3,4,5]
2 # List shape? HAY 수 AGHA OY)                       aoa
2 p(list_)                   # [1,2,3,4,5]         shape (x)= oe od peta 5]
4 na = np.array(list_)                                         a
5 p(na)                   #1234 5]        (5,)       Shape: (5,)
6 p(np.reshape(na,(5,1)))   # [fa] [2] [3] [4] [38]]   (5,4)     Type: <class ‘numpy.ndarray ‘>
7 p(np.reshape(na,(1,5)))    #([123 4 5]]      (1,5)      Values: [1 2 3 4 5]
8 p(np.reshape(na,(1,5,1))) # ([[1][2][3]{4]{5]]] (1,5,1)
9 p(np.reshape(na,(1,5,1,1)) )# (ECE1IIEC2IIC 03] 10 [4] 1005] 11
19 p(np.reshape(na,(1,1,5,1)))# [[[[1][2][3][4][5]]]]
11 에 oan en 6. (1,5,1))))# 12 2 3 4 5} (5,)
nA heleaien                   .                    a

@한국시연구소 홍근선          -79- 무단 전재, 복제, wal, 디지털화 금지


===== PAGE 81 =====
2부. RNN                                         2.4 RNN Model Design (Char-RNN)

= Model-1 설계 : many to one 기본 모델
@ WH: 10742] 문자열 ㅁ006×, one-hot coding(x)
® Shape : (samples, timesteps, features)
(samples, 10, 1)
@ LSTM layer : 75742] unit
® Dense layer : LSTMB3S 받아서 2574 출력 (SHS index7t 아님)
®@ Activation : softmax func, 사용
@ Classification 문제 이므로 확률로 변환
/ Loss func. “503156_00169011021_.0705560100”사용

(, y= indexS 넣어주는 것, 모델은 정상출력 필요)

모델의 정적 표현
Output(25)

a 학습 후 추론(문자열 생성) :
10개의 문자 시퀸스로 모델 학습을 완료하고,                      Gobel eX.

@
@ 10개의 seed 문자를 넣어 11번째 문자를 추론,
@ 11번째 문자를 포함한 10개의 문자를 넣어 12번째 문자를 추론,
@ 반복하여 180문자의 문장 생성
학습                           =           추론(문장생성)              fil lel le

Ex
be

|

“|

Traingind Char Seq.
(one-hotencoded Char}

Seed Char Seq.
{one-hot encoded Char)

(oo"" L000)

160        seas     ciara  —    “SAP DEEP LEARNING

@한국시연구소 홍근선                    - 80 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 82 =====
2. RNN                                         2.4 RNN Model Design (Char-RNN)

= Model-1 define : many to one

® LSTM layer:
~ units: 75, LSTM output dim (= # of units )
@ \nput_shape=(sequence_length, features) : (10, 1) (saraples, timesteps, features)
samples 442#(default=None)3}Oj 가변 형으로 설정 가능
® Dense layer
@ units: num_classes = 25 (문자 종류
/ Activation function: softmax(classification)
# Sequenctial model define: LSTM + Dense
hidden_dim = 75 #15¢@
model=keras.models.Sequential()
#model.add(keras. Input (shgne=(None, features))) # (None, None, fuatures)

에 W Pe be

ㅣ
5 00061.800((6『85 . Input (shape= (sequence length, features) ))  # (None, timesteps,  fuatures)|
5 model.add(keras.layers.LSTM(hidden_dim))       # output. shape: (none, 75)               |
?. 00061.800((6065.126「『5.06056(040. classes, activation='softmax'))                             |
고정 AWA                       input: | (6, 10, 191 |          가변 ALIA! .                      input: | 1@, 2, DI

:                                                     2: 10040              al
ap Atop aves:  output: | [(?, 10, 13] |                      “ape    0000608  output: | [(2, ?, 1)]

:    :    =                                                       i     4    2.    1

Istm_16: LSTM   pe | ee)                          istn_15: LSTM   input | S20

output:     (2, 75)                                                             output: | (2, 75)

dense_16: Dense    ee 1 60. 790                                       dense_15: Dense    input. | (2, 75)

output: | (2, 25)                                                                 output: | (2, 25)

161                                                                                                           SX DEEP LEARNING

Aodel

= Model summary

© LSTM param #

= 4 * hidden_state * (inputs + outputs + bias(1) )
(4: W_forget, W_input, W_output, W_cell ),( hidden = output )

=4 * 75*(1+75 +1) =23,100

® Dense layer param #
= (inputs + bias(1)) * outputs
= (75 +1)*25 = 1,900

Model: “sequential 18”

Layer (type)             Output Shape           Param #
lstm_18 (LSTM)           (None, 75)            23100
dense 18 (Dense)          (None, 25)            1900

Total params: 25000
Trainable params: 25,e00
Non-trainable params: 0

@한국시연구소 홍근선                    -81- 무단 전재, 복제, Hal, 디지털화 금지



===== PAGE 83 =====
2부. RNN

2.4 RNN Model Design (Char-RNN)

= Model Compile
®@ loss: ‘sparse_categorical_crossentropy
: 0/27} target labelZt2| crossentropy, LabelS index= 넣은 경우
®@ optimizer: Optimizer 지정 > 'adam’
® metrics: train 중 monitor= 것을 지정 > accuracy

1 model.compile(loss
2                       optimizer='adam',

‘sparse_categorical_crossentropy’, # one-hot coding(x)

2               metrics=['‘accuracy'])                   # classification 4             b
Kt             le
= Model Train                                                                        1
a         ah ie =
1 2étime
Z epochs = 266 #200 #5¢
3 history = model.fit(X, # X.shape : (176, 10,0)                 내
4        Y1,        # Y1.shape : (170, 1)                  Sy
5          batch size=1,                            ie              ct          배
쁘               a   reg                                               ~~          b>
6         epochs=epochs,                          mee VPP      . 2 bd
7            validation_data=(X,Y1) ##                     이] ain oss .               ean
=" vel_ace                        ~
:         )                                       185 BS
0 BS 05 % 100 as | 150 Urs * 20
@ Batch_size=1 : 다른 모델과 비교하기 위해서 설정한 Z(default=32)
Epoch 200/200
1706/170 [                      ] - 35 16ms/step - loss: 3.1@27e-84 - accuracy: 1.0000 -
val_loss: 2.9@84e-04 - val_accuracy: 1.0000
Wall time: 7min 405

163

® Layer Normalization H2S}H 어떻게 될까?

sore LEARNING”)

m 문자 sequence 생성 : prediction = 문자열 만들기
@ 생성 함수 정의: generate_seq
@ 10개의 5660문자를 시작으로 개의 문자열을 생성하는 함수
/* model: 생성 model object(#S2! 모델)
/* Char_dic : dictionary (‘char’ : index)

/ seq_length
/* seed_text: 4        1S 시동 걸기 위한 10개의 문자열
@ n_chars: 생성하고자 하는 문자열

® Return
~ In_text: “seed_text” + “generated text”

Md oe

3 # EAE BAO]

4 def{generate_seq(model, char_dic, seq_length, seed_text, 0 chars)]:  _

5     intext = seed text                       # seed ES + YS FA

6     # Yet 운사음의 수 = n_chars

7    for i in range(n_chars):

char € Generate a character

21        intext + 앤향 ㅎ © 4/807 주

22     return in text
=                               oO            5      하그
한국시연구소 홍근선                    -82=       ct 전재, 복제, 24ll, 디지털화 금지


===== PAGE 84 =====
2부. RNN

2.4 RNN Model Design (Char-RNN)

@ For loop "문자 444 routing

ㅎㅎ In_text(=At) > 1ㅁ006×(숫자)
@ keras.preprocessing.sequence.pad_sequence APIS 이용
- 문자들의 마지막 maxleng(=10)74#3 얻음 : truncating=pre’
ㅎ model.predic : 10개의 indexS 넣고, 25개의 확률(아|하별 확률)을 얻음
@ 입력값(6000060)의 shape ? : (1,10,1) , (samples, time_steps, features) 유
@ np.argmax : 가장 = 값의 위치(1006×)를 얻음
@ AS indexS 문자로 바꾸어 in_textol] 넣고 반복
7     for i in range(n_chars):
8        # 운사 encode : PA -> int
9        가 현   [char_dic[char] for char in in_text]
10         EAD 그가 조정 : 00<오7 TM Stee 424
ii           비마 여 = pad_sequences([encoded], maxlen=sequence length, truncating='pre’ )
12        encoded = np.array(encaded)
13       바0:  aS Zeshene encoded, (1 encoded.shape[i],1)) #(1,18,1) <- (1,1@)
14              #  tf <    eA 주 zx
15       | Vink =   us oil,  verbose=@) ©  \# yhat.shape=(1,25):\class HS
16        yhat = np.argmax(yhat,  axis=1)          # index <-  pb.
17       # 군사 고승 : integer -> character
18        for char, index in char_dic.items():                    Yu]    이거 0
을                                  0”
19            if index == yhat:                                 esl  |  Ut 로
20                 break
21        intext += char  # FAS SOY FF

BEL EE EF BR MA

* 생성된 문자열 결과

sentence = ( “if you want to build a ship, don‘t drum up people together to "
“collect wood and don"t assign them tasks and work, but rather ”
“teach them to long for the endless immensity of the sea.” )

aw Ne

fos 2s ote

print( ‘Trigger characters: “want to bu "\nResult: \n“{}"'.format(
generate_seq(model, char_dic, sequence length, ‘want to bu’, 200)))

# test _mid-line_

print('\ntrigger characters: “collect wo"\nResult: \n"{}"'.format(
generate_seq(model, char_dic, sequence_length, ‘collect wo’, 200)))

& 내만 nes Societe

print(’\nTrigger characters: “aabbcr than"\nResult: "{}"'.format(

OU me 나 54

@

9     : generate_seq(model, char_dic, 56006068 16208타, ‘abbcr than’, 200))) r) 3b a .

.

* epoch 200

Trigger characters: "want to bu "
Result: “want to build a ship, don't drum up people together to collect wood and don't assign them tasks

and work, but rather teach them to long for the endless immensity of the sea.mestt collueit th barc, but aorathe”       J

iy

Trigger characters: “collect wo"
Result: “collect wood and don't assign them tasks and work, but rather teach them to long for the endless
immensity of the sea.mestt collueit th barc, but aorathe endless immensity of the sea.mestt collueit th bare, "           Dd

나 7

Trigger characters: “aabbcr than"
Result: “abbcr thanhe sea.mestt collueit th barc, but aorathe endless immensity of the sea.mestt collueit
th barc, but aorathe endless immensity of the sea.mestt collueit th barc, but aorathe endless immensity of ”

@한국시연구소 S24                     -83- 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 85 =====
2부. RNN                                      2.4 RNN Model Design (Char-RNN)

m= Model-2 : many to many

@ LSTM layer : return_sequences=True 로 설정                                    좀더 안정적인 학습
|
hidden_dim <                                                             rs
model=keras. models .Sequential()
model. add(keras .Input(shape=(sequence_length, features) ) )           ae

model. add(layers.LSTM(hidden_dim,
return sequences=True) )## many to many
model. add(layers.TimeDistributed (
layers .Dense(num_classes, activation='softmax')))
@ 2tstep2| 예측출력이 모두 1055
산출에 참여하게 됨

47100

‘~ 07 Vi fh Ww ho 아그

ㅁ휴~
고.

elo?

B 0 % 0 1S 180 15 mo

Model-1

> 10개의 예측 결과를 같이 검토 fs           ae

> 문자열을 검토                          |                     .
@ Loss 참여 비율을 변경하기

> loss weight control                   ts    ts    fs

75

ri be St |

bet
bo]

10

|: 님

63506

# 학습할 문장
sentence = ( “if you want to build a ship, don't drum up people together to "

* 생성된 문자열 결과

1
2
쓰                           3            “collect wood and don’t assign them tasks and work, but rather ”
Model-2 제 epoch 200               4            “teach them to long for the endless immensity of the sea.” )
(~  Trigger characters: “want to bu"                                                                                                       ^
Result: “want to build a ship, don't drum up people together to collect wood and don't assign them tasks and
\__ work, but rather teach them to long for the endless immensity of the se@.oer Jeach them to long for the endles’          기
하거                                  ~)

-
Trigger characters: “collect wo"
Result: "collect os ae om assign them tasks and work, but rather teach them to long for the endless

a  immensity of the ¢ea,oer teach them to long for the endless immensity of the sea.oer teach them to long for the 6"      )
ss                                                                                                                                       세

( Trigger characters: “aabber than"
Result: “abber thanhe 2.95 t teach them to long for the endless immensity of the sea.oer teach them to long

해  for the endless immensity of the sea.oer teach them to long for the endless immensity of the sea.oer teach the’          J

Model-1. epoch 200 이상한 문자열이 지속되는.경향이 더 많음

Ae                       ‘                                                                                                                개
Trigger characters: “want to bu "
Result: “want to build a ship, don't drum up people together to collect wood and don't assign them tasks
and work, but rather teach them to long for the endless immensity of the sea.mestt collueit th bare, but gorathe”       J
<

(~ Trigger characters: ‘collect wo"
Result: “collect wood and don't assign them tasks and work, but rather teach them to long for the endless

\_ immensity of the sea,mestt collueit th barc, but agrathe endless immensity of the sea.mestt collueit th bare, "           ,

(  Trigger characters: “aabber than”
Result: “abbcr thanhe sea_mestt collueit th barc, but agrathe endless immensity of the sea.mestt collueit
di         mensity of the sea.mestt collueit th barc, but aorathe endl

endless immensity of *
03163

a     ce

th bare, but aora

6 eaten       ve                                             f DEEP LEARNING
한국시연구소 홍근선                     - 84 - 무단 전재, 복제, 24, 디지털화 금지

the endless imi

sammie:



===== PAGE 86 =====
2부. RNN

               2.4 RNN Model Des

= Model-3 : many to many
® LSTM layer : stateful = True 로 설정

i # many to many + stateful

요일 | 월 |화|수|월|화 |수|목|금
종목1 | ohlvelohive Johive |아1 |ohivc ohive |ohive Johive | ~

종목3 |ohlvcilohive |ohivc |ohlve johive johive ohlve Johlve

ee

169

2 hidden_dim = 75 #15¢                                                                      ae
3 model=keras.models .Sequential()
4 model.add(keras.Input(shape=(seqyence_length,features),
6 model.add(layers.LSTM(hidden_dim>
2                                      return_sequences=True,
8                                      stateful=True)) ### epoch fYA/ batch ZY 247
9 model.add(layers.TimeDistributed(
18          layers.Dense(num_classes, activation='softmax')))
® 1) Input LayerJA] batch_size 4% vs. fit( )에서 선언
ㅎ 2) LSTM( stateful=True...)
@ 3) Fit( )에서 shuffle=false 선언
@ #Parameters? : 동일함 (51316 초기화 방법이 다를 뿐)
time_sptep=3            time_sptep=5            + Stateless, batch=None

32 | ohivelohive Johive johive ohive lohive johive Johive     Stateful, batch=3

commen mie 4.5   FEP LE RNIN

0”

&

= Model-3 : many to many + stateful (2)

@ Model,fit() | 1 spochs=200 #52                                   |
3 h=
4 for i in range(epochs):
2    moge LTS se scares.       # epoch A/4/4/    EAR
a     h.appe
7   er me 1 ~ Y, epochs=1, # epoch#OfA/ stateful
ano WAM   3 으르 .6856 size=1,      # model defineif 을지 000
Apa           shufflezfalse,      # epoch 4/4f/A/ shuffte 27
\ ao, itl x B             validation_data=(X,Y)#¥
Us AVE             ))

® LSTM 초기 상태 (hidden state, cell state) 전달
@ Stateless : Cell state= sample 마다초기화 = )tyjay  예스
@ Stateful : 이전 sample2] 상태를 초기값으로 사용
epoch 시작 시 state 초기화 필요                            차? 0
S O/H 상태를 안다는 것의 의미

ws
a
s
a
[2
wn

bl
rl
hl

A 제한된 ABAS 넘는 과거의 정보를 갖는 것

 예) 일주일 과거정보만 보는 일기 예보관 + 메모
Layer (type)             Output Shape           Param #
lstm2 (510 00000 09 0. 7S)23100
06 _distributed_1 (TimeDist (1, 10, 25)          1900

Total params: 25,060
Trainable params: 25,000    #P= 동일함
Non-trainable params: 0

sng

TH

으르

@
rok
nt

시연구소 홍근선                      -85- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 87 =====
2.4 RNN Model Desig

n (Char-RNN)

* 생성된 문자열 결과
Model-2 « epoch 200

sentence = ( “if you want to build a ship, don’t drum up people together ta ”
“collect wood and don't assign them tasks and work, but rather "
“teach them to long for the endless immensity of the sea." )

PUN 다

Trigger characters: "want to bu"
Result: "want to build a ship, don't drum up people together to collect wood and don't assign them tasks and
\__work, but rather teach them to long for the endless immensity of the sea_oer teach them to long for the endles"

Trigger characters: ‘collect wo"
Result: “collect wood and don't assign them tasks and work, but rather teach them to long for the endless
immensity of the sea,oer teach them to long for the endless immensity of the sea.oer teach them to long for the e”

No
7

IP

Trigger characters: ‘aabber than”
Result: "abbcr thanhe sea.oer teach them to long for the endless immensity of the sea.oer teach them to long

에   for the endless immensity of the sea.oer teach them to long for the endless immensity of the sea.oer teach the"          )
Model-3 + epoch 200 학습하지 못한 상황이 문제를 지속시킬 수도 있음
~

Trigger characters: “want to bu "
Result: "want to build a ship, don't drum up people together to collect wood and don't assign them tasks and
work, but rather teach them to long for the endless immensity of the seat at d td d and don't assign them ta’

2 a
IX

Trigger characters: “collect wo"
Result: "collect woollect wood and don't assign them tasks and work, but rather teach them to long for the
endless immensity of the sea‘tatdtd d and don't assign them tasks and work, but rather teach them to long fo’        J

Trigger characters: “aabber than”
Result: “aber than isudem toh them to long for the endless immensity of the sea,t at dtd d and don't assign
them tasks and work, but rather teach them to long for the endless immensity of the sea.'t at d td 0 and don”

se

171        eae Tee eee

m™ Model-4 : many to many + stateful + batch_size=2
® 두 개의 SIS 학습 하기 : 두 번째 문장으로 CAS 배울까?

1 # HEY #2 1804}

2 sentencel = ("if you want to build a ship, don't drum up people together to "
2            “collect wood and don't assign them tasks and work, but rather ”

4            “teach them to long for the endless immensity of the sea."

8 )                                       -

6 # PH #2 1804}

7 sentence2 = (“Our developer guides are deep-dives into specific topics such “
8           “as layer sublassing, fine-tuning, or model saving. They're one"

g           " of the best ways to become a Keras expert. Most of our ")

® batch_size=2 로 설정하고 두 개의 문장을 동시에 학습하도록 설정

time_sptep=10                                           time_sptep= 10
char |011121314151617181910111213141516|71819
fa   .
문장1 |; | +  | 014  \|8|ㅁ|  y|oju  wiaj|n|t  a
2a |olul ec dlelvielllolulr dje|vile|ljolp
6 om  :        eran  00  - 1 DEEP CEARNING |

@한국시연구소 홍근선                     -86- 무단 전재, 복제, SF, 디지털화 금지


===== PAGE 88 =====
2부. RNN                                         2.4 RNN Model Design (Char-RNN)

= Model-4 : many to many + stateful + batch_size=2
® 3 번째 layer: batch_size=2 로 설정

i # many to mony + stateful + batch_ size=2
2 hidden_dim = 150 # res          개
3 model=keras. models. “Sequential()
4 model.add(keras .Input(shape=(sequence_length, features),
5                       batch _size=2 )) ## 24/°9/ YUS FA/GES
6 model.add({layers. LSTM(hidden_dim,
7                       return_sequences=True,
8                    stateful=True)) # epochLfOPA/ batch 2190 GA/
9 model.add(layers.TimeDistributed(
18      layers.Dense(num_classes, activation="softmax’)))

® #P LSTM: S& (hidden_dim = 75Y 경우)
Dense: HS, 2432=(75+1)x32, char_classes7} 32로 증가한 것에 기인
/* state= 학습할 『가 아님: States 분리, 두 AAMAS 분리해서 학습

Layer (type)                 Output Shape              Param #
lstm_4 (LSTM)           (2, 10, 75)          23100
time_distributed_3 (TimeDist (2, 10, 32)           2432

Total params: 25,532
Trainable params: 25,532
Non-trainable params: @

[에                    83

173          “   '   atten   rata   Sk DEEP LEARNING”

= Model-3 : many to many + stateful (2)
ie  Model. predict() :   두 개의 ABAS 넣고 두 개의 예측을 받음
~짓익지 사지

#4} encede :   f -> int

eae = [char_dic[char] for char in in_texti] ##
encoded2 = [char_dic[char] for char in in_text2] ##
# PHS 그 조정 : mx#G 2G Yee WA

encodedi = pad_sequences([encodedi], maxlen=sequence_length, truncating='pre') #(1,1¢)
encoded2 = pad_sequences([encoded2], maxlen=sequence_length, truncating=‘pre’) #(2,7@)
encoded3 = np.array([encoded1, encoded2])             ##(2,1,18) < (1,10)*2
encoded3 = ci, (2,encoded2, shape[-1],1)) #9(2,18,1) <- (2,1,18)

fe   Pod

순

FAO 82

(18, )<(2,18, 32)
Hz! (10, )<(2,10, 32)

np.argmax(yhat[@], axis=1) # PE:
yhat2 = np.argmax(yhat[i], axis=1) #4

@ 추론결과 : 동일한 5660로 다른 AWA 출력
> 추론과정에도 두 개의 상태를 관리 함
> 섞어서 학습하는 것과 무엇이 다른가?

174                    해    _—     =
@한국시연구소 S24                - 87 - 무단 전재, 복제, 24i], 디지털화 금지

ㆍ


===== PAGE 89 =====
2부. RNN                                        2.4 RNN Model Design (Char-RNN)

* 생성된 문자열 결과
Model-4 ㆍ00001400 같은 듯 다른 듯.…. 최소한 ''

/ Trigger characters: “want to bu ”

\. endless immensity of the sea. the best ways to become a Keras expert. Most of our the endless immensity of the *

ao.

일 Trigger characters: “collect wo "
Result1: ‘collect work,ond work, but rather teach them to long for the endless immensity of the sea. the best

ways to become a Keras expert. Most of our the endless immensity of the sea. the best ways to become a Keras e”

Result2: ‘collect wor best ways to beceme.a Keras expert. Most of aur the endless immensity of the sea.
에 the best ways to become a Keras expert. Most of our the endless immensity of the sea. the best ways to become a Kera”/

i Trigger characters: “abber than "                                                                                                        >
Result1: “abber thans suhopics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics
suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics suchpics "
Result2: “abber thangasks aar tohg for the endless immensity of the sea. the best ways to become a Keras expert.

Most of our the endless immensity of the sea. the best ways to become a Keras expert. Most of our the 60016"           J

S

ode RMNG NE Digerete sim) Hever <A

@ 실습과제 ~ 과제 1. model-1,20/44 batch_sizeS 322 바꾸고 1055 함수의 모습을 확인하자

epoch& 200->1000로 수정하자
변화를 설명해 보자

i
106
기
의

선 하자(|100600_0101, layer7}), batch_size, epoch 바꿔보자
문장이 BOHASH statfulS 사용하는 것이 유의미 한지 확인해 보자

과제 4. 입력 ZAPS one-hot ㅇ00109하여 입력으로 사용해 보자
변

성능 변화의 원인을 생각해 보자
Base Model1 Min Loss:0.00003                      One-Hot 적용 Min Loss:0.000003                        Batch:32 Min Loss:0.001528
es            배에야                         2    그        4                       eee           ss
30°     ~ 개               }             a     x $     is                         108     oy
et ]족                 a                       ew Of     ‘                                          my
a                  a               a
oe           :                                 10           eo                     i                4   내
Ht                   .           SLES,                    n               >
                 at                   10                   Bek                      ey
10"            Se          ut                          a   해              을 도      107            ase
8                                           6                후   %,                             ~
제      ics          10"?               ae         fay                 ~
7                    .        1s,                                        *                 재                          제
10-3      ‘mee o                                    ~                                         SS
*      H      ac         10“                           <       ;          ee a  a
!    나                 도        개                                       자     f                                         ~
나 ee           a        ~] | gor fe7 르드      |         ed          il oe               뜨거
~~~ 1055                   5                 memel me 1055                         BA                ~~~ loss                            wh
의 25 0: 25 360 125 80 325 200        0 25 50 75 100 125 150 175 200        0      200 400 600 800 1000

176 _

@한국시연구소 홍근선                      -88- 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 90 =====
2부. RNN                                    2.5 RNN Model Design (MNIST-RNN)

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures)

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNIN
RE        FO

CiPeE  R YOU

oS
@ Image= 2차원 정보, images 한 line*! 보면 인식할 + 있을까?

8 Model-1 설계 : many to one 기본 모델
® 입력 :사진1장(28×28) : 28line, 28pixel/line
® Shape : (samples, timesteps, features )
@ Features = 28(pixels)

~ Timesteps = 28(lines)                                              ㅣ
/* Batch size = 가변                                                       ines(v.

> (None, 28, 28)

® 출력 : 10개의 숫자에 대한 확률
> (None, 1, 10)
WAAnm

28 pixels(h28)

—e    oe
@한국시연구소 홍근선     -89- 무단 전재, 복제, Yall, 디지털화 금지



===== PAGE 91 =====
2부. RNN                                      2.5 RNN Model Design (MNIST-RNN)
m Layer 2} 입출력 shape 예측
® Input       X (bs, v28, h28) ,Y(bs, )
® Dense : 64, (bs, v28, h28) > (bs, 28, 64)               모델의 정적 표현
® LSTM : 16, (bs, 28,64) ㅎ (bs, 16, 1)                   ihn
@ Dense :10, (bs,16,1) > (bs, 10, 1)                Output(10)
© Output: 10, (bs, 10, 1)                                      10.
Dense(10)
f6x1
LSTM(16
[ 100바의 3-dim 모습 ]                                TM(16)
(bs,v28,h28)                                      [64,28
h28                                            Dense(64)
v28
Batch

179

m 모델의 내부의 Sequence 동작 : line 단위로 scans+=0| 동작

모델의 동적 표현

7

모델의 정적 표현

Output(10)

Dense(10)

‘ext
1 64,x28
Dense(64)
28,x28

_feature(28)x28

ESLER RL

180                                                     SR DEEP LEARNING”

-90- 무단 전재, 복제, 23, 디지털화 금지



===== PAGE 92 =====
2부. RNN                                   2.5 RNN Model Design (MNIST-RNN)

= Model-1 define
© 첫번째 06056 layer : LSTMO] AAS|O2 TimeDistributed layer= wrapping
@ time_steps 만큼 반복 동작
® 두 번째 Dense layer : LSTMS340| 마지막에 한번만 나오므로 1ㅁ없이 사용
마지막 time_stepOl] 한번만 동작

】

## Model~1
def_model_1():
#layer 410!                                                                   Colley
in_layer = keras.Input(shape=(time_steps, features))  400
in_dense_layer = layers. LimeDi stributed (layers Dense(in_dense))-_.. eA lsnoe  34

istm_layer = layers.LSTM(stm_units)        # LSTM

out_dense_layer = layers.Dense(out_ dense, activation='softmax')

: many to one 7/;

oN AM 제 Wh el @&

Cy

i

Re
%
4

= keras.models.Sequential (name="Basic-RNN")
model. add{in_layer)
model.add(in_dense_layer)
model.add(1stm_layer)
model .add{out_dense_layer)
14      return model

be

oO 0
3
Qa.
iy
a

fod pad
ies

Ww he

he

# 주요 변수 정의

features = 29 #pixels

time_steps = 28 #lines

in_dense=64    # GO| 값

lstm_units = 16 # 염의 값
out_dense=19   # BAS 숫자(0~9) 확률

ray
냐에

16 model 1 = model 1() # Model Instance

nN ve &

soe scrsescecocniei

ARNING |

181

= Model summary
® LSTM param #
= 4 * Istm_size * (Inputs_size + outputs_size + bias)
( 4: W_forget, W_input, W_output, W_cell )
=4 * 16*(64+ 16+ 1) =5184
In_Dense param # : (28 +1)*64 = 1856
ㅎ Out_Dense param #: (16 + 1)*10 = 170

©

Model: “Basic-RNN"

Layer (type)             Output Shape           Param #
Istm_8 (LSTM)            (None, 16)            5184
dense_18 (Dense)          (None, 18)            170

Total params: 7,216
Trainable params: 7,210
Non-trainable params: 0

i alll                      -91- 무단 전재, 복제, Bal, 디지털화 금지


===== PAGE 93 =====
2부. RNN                                      2.5 RNN Model Design (MNIST-RNN)

= Model Compile & Train
®@ Compile

® loss 함수 : 'sparse_categorical_crossentropy’ (label index 값을 사용)
1 model_1.compile(loss='sparse_categorical_crossentropy',

2                              optimizer='adam',

3                          metrics=['accuracy'])
® Model Train

1 %%time

2 batch_size = 512

3 history_1 = model_1.fit(x_train, y_train,  #(600@0,28,28), (60000, )
4        validation_data=(x_test, y_test), #(1000@, 28,28), (14008, )
5          batch_size=batch_size,                               |
6          epochs=30)                                          |

® Return 값을 history_10] 전달 : dict_keys(['loss’, ‘accuracy’, ‘val_loss', ‘val_accuracy'])

m= Model-2 설계 : many to one, Bidirectional LSTM 모델
@ tHZAASE: LSTM layer 》 Bidirectional(LSTM layer)

Model-1                        [> |
7               Bidirectional LSTM
fe                                                               모델의 정적 표현
Dense                                                                Output(10)
ce                                                                       10,x1
- | »
~~ es                                                                 16,x2

Bidir(LSTM(16))

28

ea _-

한국시연구소 홍근선     -92- 무단 전재, 복제, Ball, 디지털화 금지



===== PAGE 94 =====
= Model-2 define

® Bidirectional LSTM : LSTM layerS Bidirectional layer wrapping

1 ## Modei-2 2A: Bidirectional 수스

2 def model_2():

3     in_layer = keras.Input(shape=(time_steps, features))

4     in_dense_layer = layers.TimeDistributed(layers.Dense(in_dense))
5     istm_layer =/layers.Bidirectional( # Bidirectional wrapper

6                 layers.LSTM(lstm_units)) # LS7TM

7     out_dense_layer = layers.Dense(out_dense, activation='softmax')
8    #layer GA We/

9       model = keras.models.Sequential (name="Bidirectional-RNN")

10     model.add(in_layer)

ii             model.add(in_dense_layer)

2      model.add(1lstm_layer)

13             model .add(out_dense_layer)

14     return model

as

16 model_2 = model_2()

2. RNN                                     2.5 RNN Model Design (MNIST-RNN)

= Model summary
® LSTM param #
= 4 * Istm_size * (Inputs_size + outputs_size + bias)
( 4: W_forget, W_input, W_output, W_cell )
= 4 * 16*(64+ 16+ 1)=5184 x2 = 10368
@ In_Dense param # : (28 +1)*64 = 1856
@ Out_Dense param #: (32 + 1)*10 = 330

Model: “Bidirectional-RNN”

Layer (type)             Output Shape           Param #

time_distributed_2 (TimeDist (None, 28, 64)         1856

bidirectional 2 (Bidirection (None, 32)           19368

06146 022 06056) ㆍ   ~(None, an     7    33000      [’     =) CANE
Total params: 12,554                      Jes ee            t

Trainable params: 12,554                   Layer (type)

Non-trainable params: 0                         time distributed (TimeDistri (None, 28, 64)        1856

stm 8 (LST)            (None, 16)            5184

46056 18 (Dense)              Gone

10)                  170

Total params: 7,216
Trainable params: 7,210
Non-trainable para

a

186

coe
싱지 Pe

Ome  = ㅁ 6 OM

@한국시연구소 홍근선                      -93- 무단 전재, 복제, Bal], 디지털화 금지


===== PAGE 95 =====
2부. RNN                                     2.5 RNN Model Design (MNIST-RNN)

= Model Compile & Train 동일

| | 성능 비교                                             60           Max Val_Acc:0.9635/0.9780

4 max_accl = np.max(history! ‘val_accuracy’ |                                                   sas
5 max_acc2 = np.max(history2/{‘val_accuracy' |)             825         ~

6                                                     0.90

7 pilt.figure(figsize=(10,3))

8 plt.subplot(i21)                                                           oss 4                            =              ~

9 plt.title(f"Max Val Acc: {max_acc1:.4f}/{max_acc2: .4f}")

10  plt.plot(history! ‘accuracy'], lebel="acc1')          0.80   /                   자아
11 plt.plot(history{'val_accuracy’], label='val_acc1’)            |                       내 2 |
312 plt.plot(history2[’accuracy’], label="acc2')           7                          아아 eck
13 plt.plot(history2{‘val_accuracy'}], label="val_acc2')                       |               어가 vet sce |
14 pit.ylim(@.7, 1)                              am    5    10    15    20    25    30
15  plt.legend()                                                                                                                                                    nee

16 «plt.grid()
17 plt.subplot(122)                                                                                     때 aya
18 plt.title("loss")                                      eget                         | 10592

19 plt.plot(history! ‘loss'|, label="loss1')                                  |. TTT val_loss2
20 plt.plot(history/ ‘val_loss'], label="val_lossi')                               ㅣ
21 plt.plot(history2{‘loss'], label='loss2')

22 plt.plot(history2{‘val_loss*}, label='val_loss2’)

23 plt.semilogy()

24 pilt.legend()

25 plt.grid()                                                                                                 10그

26 0바.5000()

187

a 실습과제
과제 1. BI-LSTMO| 구조적 성능향상이 있는지 확인해 보자

~ 두번째 모델(8Ｌ51\0)이 #P7} 크므로 성능비교가 어렵
~ #parametero} 엉향을 제거하기 위해,
번째 모델에서 Istm_units=?72 들려서 학습시켜보자

것
동일한 #※0818006\하에서 성능을 비교해 보자

       Max Val_Acc{Basic/Bi-LSTM):0.9807 / 0.9763                                                 Loss
|                                    a             \                                —— loss
i                                                                       me val loss
0.95                            oe     생애     t                                       ~~ 10552 00 1
——~ vat_loss2 |
0.90 +
0.85 +-
oso 4                                      —          4
0.70                      '                 '         1        고              +        ，                 +                 +         +
0        5       10       15       20       25       30             0        5       10       15       20       25       30
=             oe

@한국시연구소 홍근선                      -94- 무단 전재, 복제, oi], 디지털화 금지


===== PAGE 96 =====
2부. RNN

2.5 RNN Model Design (MNIST-RNN)

= Model-3 : Hierarchical RNNC= MNIST classification
® 변경사항 : LineSt?|= scan » Pixel scan(line 단위) 정보를 LSTMO|] 공급

@ 첫 번째 LSTM layer : TimeDistributed layer wrapping 된 LSTM
* 첫 LSTM 레이어가 time_steps(28 line) 만큼 반복 동작
@ 첫 Ｌ5114에 1,x28 입력이 x283] 반복 공급 > 50.×28 출력

@ 두 번째 LSTM layer : 50,x28 받아서 16,x1 출력         ce el 절인
2. pixel = i      ## features
® Dense layer: 16,x1 받아서 10,×1 출력                 3 col = 28       #8 pixels
4 row = 28
> (bs,28,28,1))>(bs,28,50)>(bs, 16)> (bs, 10)               6 Late unite
9 def model_3():                                    6  lstm2_units
18     #layer (10%                                7 out_dense =         ㆍ 숫자(0~9) 확률
44    in_layer = keras.Input(shape=(lines, pixels, pixel))
i2     istml_layer = layers. TimeDistributed(layers.LSTM(1stmi1_ units) )     모델의 정적 표현
13     lstm2_layer = layers .LSTM(1stm2 units)
14     out_dense_layer = layers.Dense(out_dense, activation='softmax’)
15    #layer A Ot
16     model = keras.models. Sequential (name="Basic-RNN")                 Dense(10)
17      model .add(in_layer)                                                            Next
18      model .add(1stmi_layer)                                                 LSTM_2(16)
19             model .add(lstm2_layer)                                                                                                                 ee
28            model. add(out_dense_layer)
fal     return model
22
23 00061 3 = model 3() # Model Instance
etre te

= Model-3 표현하기
© LSTM_10| 학습하는 것
© LSTM_27} 학습하는 것

—

모델의 동적 표현
- TimeDistributed(LSTM)2| 동작에 주의

모델의 정적 표현

Dense(10)
16.x1

LSTM_2(16)
150,x28

(1,x28),x28

- Feature((1)x28)x28

10븐 Ucy Seg   ：
> age eral .

A

|   =>
>     ar, et
대          -          때 > We 업어
@한국시연구소 홍근선           -95- 무단 전재, 복제, Ball, 디지털화 금지

Yatn= 채기


===== PAGE 97 =====
2부. RNN                                     2.5 RNN Model Design (MNIST-RNN)

@ Model summary                                            |             input: | {@, 28, 28, 1)]
.                                                                    input_1: InputLayer            개미
@ TimeDistributed (LSTM1) param #                         0006 | 0
= 4 * |stm_size * (Istm_inputs + Istm_size + bias)
=4+*50+*(1+50+1)=10,400                  tine. dist: TneDisibued(.STM) |p ne
output: | (2, 28, 50)
@ LSTM2 param #
=                          =                                              #
=4 *16*(50+16+ 1) =4,288                        —  input | (2, 28, 50)
¢ Dense layer param#                                             =      output: | (2, 16)
=(16 +1) * 10=170
dense: Dease  input: | @, 16)
을     output: | (2, 10)

Model: “Basic-RNN"

Layer (type)              Output Shape           Param #
lstm_1 (LSTM)            (None, 16)            4288
dense (Dense)            (None, 10)            178

Total params: /14,858
Trainable payams: 14,858
Non-trainable\ params: 0

191

= Model Compile

1 model_3.compile(loss='sparse_categorical_crossentropy',
2                             optimizer='adam',

5                           metrics=['‘accuracy'])

= Dataset preprocessing

i # Reshapes data to 40 for Hierarchical RAN.

x_train = x_train.reshape(x_train.shape[@], 28, 28, 1)
x_train = x_train.reshape(x_train.shape[@], 28, 28, 1)
x_test = x_test.reshape(x_test.shape[@], 28, 28, 1)

% woh

a  x_train.shape, y_train.shape, lines, pixels, pixel |

| ((60000, 28, 28, 1), (60000,), 28, 28, 1)|     10
09
08
67
@6
= Model fit                                      05
1 %%time                                                           os                                      rr
2 epochs = 30                              aay)          ‘   ;       a
3 batch_size = 512                             624            eH :
4 history_3 = model_3.fit(x_train, y_train,        a1           +                   ,
5                 batch_size=batch_size,    .    -   =    =   =   a
6                  validation_data=(x_test, y_test),|
7                 epochs=15)                   |
192 |

한국시연구소 홍근선                    -96- 무단 전재, 복제, Sl,  디 지 털화 금지


===== PAGE 98 =====
2부. RNN                                     2.5 RNN Model Design (MNIST-RNN)

과제 2. Model_3 변형 : LSTM_19| unitso| 적절할까? 너무 큰것 아닐까?

-최적의 unitso| 얼마일까? 최적인 이유는?

-『81801어리의 수의 차이도 확인해 보자

J       b
과제 B: in.Dense Layer2} LSTM1 Layer 성능 비교      Gl    myn    a   여우 파악  .
model! {| Aj in-Dense Layer2} 0ㅁ0061!3에서 LSTM192] 역할과 성능 비교 하기

- 동일한 수준의 parameters 가질때 성능차이 확인 하기

과제 4: HierachicalRNNQ Bidirectional !6하추가 하기
과제2 에서 수정된 모델에서 LSTM?2 layerS bidirectional layer2 수정하고, modei2e} ASS 비교해 보자

과제 5. 추가 변형 : LSTM2 argument ‘return_sequence=True’S 넣어보자

-Ｌㄴ5102 Layer output shapeS 확인하고, 최종 출력 shapeo| 되도록 Layers 추가 하자

                     See     PLS       총            바치    ee    59696682553880305   =    straps
193                                                       .                      Sk DEEP LEARNING

© RNNGZ ADEA Arie aa |

194 _        세제       on      ae      sk DEEP LEARNING”
@한국시연구소 홍근선                       -97- 무단 전재, 복제, 발춰, 디지털화 금지


===== PAGE 99 =====
2부. RNN                                                                   2.6 Optimization

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNING
RE        FOR YOU

610

\ Optimization              %제빅 ESP 7Y  『0 EY
= 0011011232101 (협의의 최적화)

© 목적함수(605 function, loss function)7t 최소가 되도록 Parameters 변경하는 과정

® Optimization algorithm 선택

® Deep learning= 많은 parameterSS 최적화 하여야 St

여러 가지 요소들이 HS ASS 야기하여 최적화를 방해 함

8 OptimizationS 위해 결정해야 하는 요소들 (광의의 최적화)

® 광의의 최적화 목표 : Generalization performance 향상
Weight Initialization : zeros, normal dist., xaiver, He init.,---
Hyper parameter search : grid search, random search,---
Optimization algorithm : SGD, NAG, Adagrad, Rmsprop, Adam,--:
Regularization : L1, L2, L1_L2
Learning Rate schedule : Exponential decay, Polynomial decay, :--
Normalization : Batch norm., Layer norm.,-::

e¢¢oe 4 <

rem   a ETN RSNA VERTEC ICH 4.50 AAA
@한국시연구소 홍근선     -98- 무단 전재, 복제, 발춰, 디지털화 금지


===== PAGE 100 =====
2.6 Optimization

m Regression model 평가하기                     Var(y) = “x01 - 302
® MSE = Bias? + Variance
@ 값의 단위가 직관적이지 않음  ne ,            MSE = an — ¥;)
~       TV 4         [~]    Varro te  £                   = n       u    Yi

@ 대상 값의 크기에 영향을 받음

@ 큰오차에민감    > ~ Nonualire, - RMSE = E01 - I?
n

@ RMSE = Bias? + Variance

 같이 직관적임 대상 값의 크기에 영향을 받음      MAE = 217. - 이 |
® MAE
관적임, 오차에균등                                    ~, 파피
@ 값이 직관적임, 오차에 균등한 민감도                   MAPE = ~~ X17 |
® MAPE(Mean Absolute Percentage Error)                      7      "<9;
ㅎ 대상 값의 크기로 나누어 normalize                        SAME = = | ppp

@ 대상 값의 크기에 영향 없음, 직관적                                                                   !

대상 값의 크기에 영향 없음, 직관적               17      leel
@ yi < 1, 값이 커지며 불안정, 폭주 sey               pow ee:  노호 yy
> y:7 '0에 수렴하는 경우,        BB (보가 ol Hee a A
SAME(Symmetric Mean Absolute Error) 사용   Pre 4) )    = oe
12S 가지며, 확률로 해석 됨 <                     a 제기
or tases  an Abse    caled Error) | ' 9 WAE      ~ MAE naive
676/의 Bae 값 변동의 평균으로!  나눈     :
@ 값의 변동대비 오차의 변동 관계를 평가
~ ~더즈서 차이가 있는 경우 사용     caaamaamae

Sh DEEP LEARNING |

08 Oe

2
오차 값보다 비율 오차에 민감             곤드 ROM       og(1+ ¥;
@ 매출, 수요 예측, 금융 : 몇 % 오차인지가 중요 “*                           가
@ 지수적으로 증가하는 생물학, 인구                           0 =1-- =
we uel wae            aie”

© R? or r?(R-squared :

독립변수로 설명되는 종속변수의 변동소                       cS = Tam =    =o

U(fraction of variance unexplained)                                               jp? 29
 설명되지 않는 분산의 비율

@ R2=0.49: 종속 변수 변동성의 49%가 설명되었고

%의 변동성은 설명되지 않음
»(couine str
@ FEZ 각도의 60506 값으로 두 벡터의 유사성 8K on   Sy

(> NLPOIAY 단어나 문장의 유사도 측정에 사용. —        oo Vat”
A fy)              예측값 (9)               MSE             MSLE
10       8       4     0.0044
10       2       64     0.43
100      90       100    0.0053

@한국시연구소 홍근선                  -99- 무단 전재, 복제, SH, 디지털화 금지


===== PAGE 101 =====
2부. RNN

2.6 Optimization

m Regression model 평가하기(2)
© 주가 시계열에서(종가기준)
- 금일 값을 ㅠ46, 다음날을 060
- 값 차이를 0ㅁ아로 보고
- Matric function2| 특징을 비교해 보자

Varfy) : mean(squarefy_true - y_mean))

MSE : mean(squarefy_true - y_pred})

RMSE : sqrt(MSE}

MAE : mean(abs(y_true - y_pred)}

MAPE : 100 * mean(abs((y_true - y_pred) / y_true}}

MSLE : mean(square(log{y_true + 1) - log(y_pred + 1)))

MASE : mae/mae_naive mae_naive: MAE of one-step ‘naive forecast method”

Peed aS            =
- 값의 scale2| 변화 : modelo] 집중하는 부분이 달라질 수 있음 <. > 부분 오차의 영향이 커짐
le
MAE(Min:58, Max:1780, Std:267            MSEIE ASE: Max:5626000, Std:527845, Mean:310692)    MSLE(Min:0.00004, Max:0.0060, Std:0.0006176
1750} — mae                                                                    “Dot-comBubble =
1500 | mae_mean                            5                                                                  ~ msie_mean
ae                                                                                             회    너       ag 받음
1250 …앉.클기의-원향을:반음                    4                                                             Ex,  차의   |율 영향을    2a
a            에
750                           re               S|    2
wk            Sealer RST 개                     *        ad 이               (
Mase 0. 90,  Max:1. ey var:0. 0010거26 >    Huy    MSE(Min:68, Max:2372, Std:339, Mean:447}           pained 0.50, Max:6.17, Std:0,79, Mean:1.56
18 Fi                                                                               6                           —- mape
owen hase mean                                                                                                      ~ mape_mean
16%                .                                                                                 5
값 크기의 앵향을 제거                                                                         HT St 비율을 %로
14                                                                                                   Ve             제
tote
12                                                                                                   개   ㅣ
찌니
104+                                                                             ieee

* R2: 모델이 얼마나 전체 변동

성을 설명하는가

R2(Min:-6.74, Max:0.83, Var:0.43, Mean:0.08

@ 독립변수로 설명

직관적이고

해석이 쉬움 (1: 완벽, 0: 무의미)

변수의 변동성

전체 설명력 평가로 모델의

전반적 성능

판단에 유리

조주 주

Baseline 비교에 유리 (항상 평균으로 예측하면 R*=0)
음수가 나올 수 있음 (모델이 평균보다 못할
두 벡터의 유사성 측정
@ 두 벡터 간의 방향 유사도를 측정하는 지표
* 1에 가까울수록 유사한 방향, 크기 보다는 방향에 집중
@ 크기 무관 유사도 측정 — 스케일 민감도 낮음

경우)

 고차원 벡터 예측에서 유용 (예: 임베딩 회귀)    ali
 normalize=! 회귀 문제에 강함                             eb.
@ 적용                        soul
 시계열 방향성 유사도                빼!

 문장 임베딩 유사도
 추천 시스템에서의 벡터 회귀

0.9975

0.9970

R2: 1-FVU, F¥U=sum(square(y_true - y_pred)}}/sum/(square(y_true - /_07080))
CS : np.dot(x,y) (np. linalg.norm(xnp.tinalg.norm(y))

"캐이     sounemtenunnennanennes eeaninnetahie #91 oA
@한국시연구소 홍근선      -100- 무단 전재, 복제, il, 디지털화 금지


===== PAGE 102 =====
2부. RNN                                                                   2.6 Optimization

% 실습: Loss function] 따른 성능 변화

8 Loss function] 따른 성능 변화도 있을까?
@ 2.3 Time Series Forecast 에서

@ Loss Func. S 다음으로 수정 후 적용

* Metric function 별로 [055 functionS 바꾸면 어떻게 달라지는지 확인

@ Loss functionS 바꾸어 성능 변화가 있는지 확인해 보자

# mse_loss=100* mse, msle_loss = 10000 * msle
ㅎ mase_loss = mase / 10000

@ r2_loss= 1-12 =FVU

# cs_loss = 100 * (1- cs)

from keras import ops — Numpy operation@keras operation? =

mae = keras. losses.mean_absolute_error

def mse_l(x,y): return 10@* mse(x,y) # mse = keras. losses.mean_squared_error
mape = keras. losses.mean_absolute_percentage_error

msle = keras. losses.mean_squared_logarithmic_error

CMON OU SBWN

def fvu(x, yt
10   return ( ops.sum(ops.abs(x — y)#*2) / (ops.sum((x - ops.mean(x) )**2)+1e-7) )
11 def r2_l(x,y): return fvu(x,y)

32 def cs_1(x,y):

13    return 10@*(1-(tf.einsum(' 30318. X,Y) /(tf.norm(x,ord=2)*tf.norm(y,ord=2) ) ) )

Sf DEEP LEARNING”

m Loss functions 바꾸며 학습 하기

2 history list = list()
3 model list = list()
4 lossf list = [mse,mape,msle 1,mase,r2_1,cs_1]
5 metrics list = [mse,mape,msle_1,mase,r2_l,cs_1]
6 for Joss f in lossf list:
7     model = ResidualLSTM()
8       model.compile(optimizer="adam', loss=loss f, metrics=metrics list)
9     print(f"\n<<Loss:{loss_f. name__}>>")
10     my_callbacks = [ keras.callbacks.ModelCheckpoint (filepath=checkpoint_path,
11                                             save_weights_only=True,
12                                         save_best_ only=True), ]
13     history_list.append(model.fit(x_train, y_train,
14                                 validation_data=(x_test, y_test),callbacks=my_callbacks,
15                        epochs = _epochs, batch_size = _batch_size))
16     model. load_weights(checkpoint_path)
17     00061 list. append(model)
18
19     print(f”<<Loss: {loss +, name__}>>")
20      for metric_f in metrics list: 0
21       |  min_ = np.min(history_list[-1].history["val_“+metric +, . 0006 . |)
22      | print(#"{metric_f._name_}, Val_min:{min_:.4f}")
<<Loss:mean_squared_error>>
mean_squared_error, Val_min:@.0@01
mean_absolute_percentage error, Val_min:1.2848
msle 1, Val_min:@.4533
mase, Val_min:2.7993
r2_1, Val_min:@.8746
<5 1, Val_min:®@.@134
| 20         어여                         --~              PE DEEPLEARNING
@한국시연구소 홍근선                    - 101 - 무단 전재, 복제, S4, 디지털화 금지


===== PAGE 103 =====
2부. RNN

2.6 Optimization

~

103

wi

102  1 ER.

m Loss function 변경에 따른 matric function 값
| 4       대             ~                                  =
@ Cs 제외한 모든 matricol 대해서 mape loss} 최적, 변동성도 확인하자
mse loss / (min metric}                           mape loss / (min metric}                           msie loss / (min metric)
10 국기     —— val_mse(0,0160)                  ~ val_mse(0.0198)
~~~ val_mape(1.3669)                   거시 mape( 1.5207)
~ vai_msie(G 5567)            \        om val_mste(0.6898)
~ val_mase(0.5990)          my        —— val_mase(9.6532)
—~ val 2(tvu) (0.1015) |                  ~~ val r2ifve}(0.1180)
168        ~ val es(0.0176)                    = val_es{0.0208}
10° 4
wt
wt
Qo    20    4“    60    80    100       °    20    0    60    80   100
00056 loss / (min metric)                           r2(fvu) loss / (min metric)                             cs loss / (min metric)
지아스애서 MEN
3
1 Mae ally
~ val_mse(0.0200}              00 VOL MSA(10,6291) enn on
107! 4 > val_mape(2.5188}      |            ~ val_mape(47.0793)
~~~ yal_msle(0.6949)                        —— val_msie(306.4203)
~~ -val_mase(0.6461)}          !    It val_mase(18.9839)
ㅡ val y2(fvu}tO.1224)                  som OL r2(fvu)58.6726)
~ val_cs{0.0214)                   moe MBE CS(O.O1 TD} --
10°?
[내    20    2    60    80    100       o    20    40

mse metric / loss_fimin metric)

@ Metric function 최적의 Loss function 찾기
@ CsB 제외한 모든 matricOll 대해서 mape loss7} 최적의 결과를 보임

mape metric / loss_f(min metric)

msie metric / loss_f(min metric)

10

… mse_loss(1.59957)
Ar mape_loss(2.36699)
per msle_loss(1.52070)
~ mase_foss(2.48474)
~ raffvu)_less{2.51820)
~ <3_foss{47.07925)

103

102

wey

\       46000

아아 mse_loss(0.74376}
~ mape_1oss(0,55674)
eee mgle_loss(0.68984}
~ mase_loss(1.74863)
~ r2ftvu)_lossi0.69490)
~ 6 1055(306.42032)

mase metric / 1055 (0010 metric)

0           20          40          60          80         100

r2{fvu) metric / loss_fimin metric)

©        20       40       60 ㆍ 80       100

cs metric / loss_fimin metric)

163

10°

19!

10? fe

30! +-

~ mse_foss(0.13218)
cm mape_loss(Q, 10292)
~ msie_loss(0.11798)
wer -mase_loss(0.32565)
“o>. s2{fvu)_loss{0.12245)

-——~ smse_loss(0.02292)
|                  mape_toss(0,01760)
msle_loss(0.62077)
mase_loss(0.05423)
s2ifvul_lass{0.02143)
<s,Joss(0.01705)

-102- 무단

my

dai, 복제, Si), 디지털화 금지


===== PAGE 104 =====
2부. RNN                                                                   2.6 Optimization

m MAPE7} 보다 좋은 결과를 보이는 이유
© 주가 데이터가 비정상적 스케일(크게 다른 수치대)를 가지고 있음

 어떤 시점은 100원, 어떤 시점은 100,000                    _ 흐
@ MSEE 큰 수치의 오차에만 반응 — 저가에서 상대적 예측 품질 무시
@ MAPEE 모든 값에 대해 비율 기반 오차를 계산 ㅡ> 전체 구간에서 균형 있는 학습
> 전체 시계열의 다양한 주가 수준에 고르게 예측 잘하는 모델이 되었을 가능성
* 모델이 큰 오차보다 작은 오차를 고르게 줄이도록 유도됨

우주
@ 1456는 특정 시점의 큰 오차(폭락, 급등 등)에너무집중됨 < MAE Pl omnia
@ MAPEE 각 구간에서 상대적 정확도를 유지하는 데 더 중점을 S             P31) BH.

> 모델이 극단적 오차보다는 전체 구간의 일관된 성능 향상을 추구하게 됨
© 특정 구간에서의 중요도와 균형

@ MAPES 정상적 구간과 비정상적 구간에 동일한 중요도를 부여

@ MSEE 이상치나 급등락 구간의 오차에 민감하게 반응하여 모델이 그 구간에 overfitting 가능성 있음

> 실무에서는 전반적으로 예측이 일관되게 "비율 오차가 낮은 모델"이 더 유용한 경우 많음
®@ MSEY| 문제점 보완 하려면                                      mn       .

 지수적 증가를 제한 하기 위해 가격 0313에 log(1+x) 적용

® Loss = mse + (mape or CS or Huber ) 결합                           oN

“@ Huber loss : smoothL1 1055에서 L1, L2 구간을 조정                   Aaa ee
@ 전체 시계열을 스케일에 따라 몇 개 구간으로 나누어 normalizest7|                 :

“205

EZ FT AL

= Weight Initialization 방법들

* 학습 성능에 중요한 영향을 끼침
00081 distribution : W~N(0,1) , 가우시안 분포에 따른 랜덤 값
@ Uniform distribution : W~U(0,1), 균등 분포에 따른 랜덤 값

 가중치가 편중되는 현상이 발생
® LeCun initialization : Ww ~ N(0,Var(W)). Var(W) =  그

“~

| \ Nin                  Nin/Nout :
—" ae      이전레이어/
® Xavier initialization : W~ N(0,Var(W)) , Var(W) = =<     Piya
in T bout
(Xavier Glorot Initialization)                                       0                     7
© He initialization :       W ~ N(O, Var(W)) ,  Var(W) a 대
Oe en                                              in

Qupqee 자음.           0”         가     1 inn ©

i tf.keras.leyers.Conv2D(
:

2    filters, kernel_size, strides=(1, 1), padding=‘valid',
> activationat=O 따라 성능이 다름 >    data_format=None, dilation rate=(1, 4)     zi, activation=None,
SI   id;    : Xavier AS

-ReLU: He 선호                       bias_regularizer=None, activity_regularizer=None,

?     kernel_constraint=None,
i                  차
『6[65에서는         g    bias_constraint=None, **kwargs )

대부분 XavierAH (‘glorot_uniform’)
ig eg Et IO

bias_initializer='zeros', kernel_regularizer=None,

oe ke
[~
&
o
1
or
e
ow
a
[13
더
[…….
[~
me
a
om
Ss
=
wm
fis
「
7
그
더
+
eo
wy
halt
는
대
mo
5
"
60
°o
or
°Q
+
=
J
mal
o
Ss
티

(11710159배9재태이 stn         ‘ir DEEP LEARNING
@한국시연구소 홍근선      -103- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 105 =====
2.6 Optimization

x Hyper parameter Optimization
m@ Hyper parameters

m Manually
@ Manual Search, Grid Search, Random Search
= Automatically
® Bayesian optimization
® Surrogate model : Gaussian process, ...
® Acquisition function
- PI (Probability of improvement)
- El(Expected Improvement)

@ Gradient-based optimization
® Evolutionary optimization
® Population-based

207

@ Epochs, batch_size, learning_rate, optimizer_params, regularization_params.,...
> 선택해야 할 많은 hyper parameter7} 존재, 또한 최적화에 중요한 요소

_2.6 Optimization _

m Random search

® Grid search 보다 random searchS 해야 됨
다음 H 입력 Zt 선정에 앞서 찾은 값이 사용되지 않도록

Grid Layout

Random Layout

인                                                         o
[기                                                         o
기                                                         E
as}                                                         08
a                                                         a
a.                                                         Qa
~                                                         +
&                                                         cod
=                                                         £
5                                                         5
은                                                         E
=        @         [         i)                       터
=                                                         =>
important parameter                             Important parameter
@한국시연구소 홍근선                        -104- 무단 전재, 복제, 243i), 디지털화 금지


===== PAGE 106 =====
2부. RNN

2.6 Optimization

XX Optimization Algorithms
@ Optimization
* Loss 함수를 최소화 A|7/= parameter(weight) |
를 찾는 과정
m Gradient Descent (기울기 하강법)
 모든 03「31005의 미분값(기울기)을 계산하여
(vector2| 미분 = 편미분) 모아놓은 +6아아를
gradient 라 하고, 전체로 볼 때 기울기가 가장 큰 방향으로
15160만큼 parameter 수정하는 것
8 Step 크기(!62[010ㅁ9 「216)의 영향
© SHS 결정했는데
수정하는 크기는?
© AS 문제, 작아도 Bj...
> Learning rate control

100
PX)      Avoiding

\             Minima                                                    ra

V7

/
/                                                                           a
4
시

ee ee

\
\

% Optimization Algorithms
a Batch size : 학습 효율의 문제 (hyper parameter)
® Batch Gradient Descent : 모든 dataOl] 대해 gradient7jAtepo], 1번 수정
data7} 100만개 라면? > 효율적이지 못함
@ Mini-batch Gradient Descent (1460): 작은 batchtt9|@ dataS 나누어 60를 수
® Stochastic Gradient Descent (SGD): 60[대단위가 '1'인 경우, 0313하나씩 GDS 수
프로그램이 벡터, 행렬처리를 하는데. 하나씩? 효율적이지 못함

* SGD: 일반적으로 MGDS 구분하지 않고,    고초
® Batch size: 연산효율 때문에.2^17 값(32.,64,128....) 주로 사용

ber Cakes -- -
CI oe 옷으. .

210.    Se
@한국시연구소 홍근선      -105- 무단 전재, 복제, tall, 디지털화 금지



===== PAGE 107 =====
2부. RNN                                                                   2.6 Optimization

,              ：                                                   VGG-56
%# Optimization Algorithms

8 Ｌ055함수의 복잡도와 초기값 문제

{a) without skip connections                                  (6) with skip connections

Figure 1: The loss surfaces of ResNet-56 with/without skip connections. The proposed filter
normalization scheme is used to enable comparisons of sharpness/flatness between the two figures.

『 6 0 후

[

% 최적화 알고리즘 Optimization Algorithm
@ SGD(Stochastic Gradient Descent ) : 82[대단위로 기울기를 계산하여 \\ 수정
Momentum : 기울기에 속도 개념을 추가
NAG(Nesterov accelerated gradient) : momentum 적용 후 Gradient 적용
Adagrad: W 변화량에 따라 가중치 부여, 변화량이 AS 『는 좀더 변화량 증가
Adadelta, Rmsprop : Adagrad 단점 개선
Adam(Adaptive Moment Estimation) : RMSPropO| momentums 혼합한 특성
Nadam (Nestrov Adaptive Moment Estimation) : ^40807에서 ㅁㅠ010600140대신 NAGS 적용

$e? %¢ 9 9 <

560
Momentum

SGD
Momentum
NAG
Adagrad
Adadelta

Rmsprop

212

yalee=radtords=animations=for Htal" "SAP DEEP LEARNING”
@한국시연구소 홍근선                    -106- 무단 전재, 복제, Sail, 디지털화 금지



===== PAGE 108 =====
2부. RNN

2.6 Optimization

mw 최적화 알고리즘 Optimization Algorithm
@ SGD(Stochastic Gradient Descent )      (
@ Momentum : 2, memoryOl AB_#Px3)

@ NAG(Nesterov accelerated gradient) :

® Adagrad: 6, 지정, 4x3)

® Rmsprop : Adagrad 6,를 이동평균으로
® 7= 0.9 , Elg?| Aa

@ Adam(Adaptive Moment Estimation) :
® Momentum, £,=0.9 추가
e

※ ge: 역전파 과정에셔 stepee = 갱신, 삭제 되므로 #증가로 보지 않지만, 실제로 필요함

2.6 Optimization

A141 = 0 —VoI(8)
Ue = Yur-1 + 1V0,F (4)
O41 =O —%

9141 = Op —%         ~
6141 = % —- 2 Og:
:            VGi +e

Gti = Vo,F(P3)

Gui = 91, + 92, aa 9,
Cumulative gradient

Elg?|t = 0.9E[g?|:-1 + 0.197

644 = 6; - ——
t+1   t   0

m, = Bym,_; + (1 - 70100
란 = 7820.71 + (1 - Bz) 9?

n
9144 = 0 - Vite *

—————" «4

Adam without cosine annealing

Adam with step-drop learning rate decay     「

Initia} learning rate to be muitiptied by 0. 1
Initial earning tate 19 be multiplied by 0.1
intial leaming rate to be muitiptied by 0.1

려108

4:                   14
ㅁ 12 We 18 owe | 1210 1        0 WS Ine WH ta te

initial learning rate to be multiplied by 0.1

initial learning rate to be multiplied hy 0.1

initial learning rate to be multiplied by 0.1

ar rer | 14 | 12        =

es     EG
Weight decay to be multipked by 0.001

6 2196 18  2
Weight decay to be multiplied by 0.001

21 3 14007/000.00012/마하.000772015703/78160-8010106-810101811006-101.10011 ^ ‘SOf DEEP LEARNING»
_ 2.6 Optimization —                           ae

wera >
Decoupled Weight Decay Regularization,2019”   V  『「

* Weight Decay 가 learning 『2[6에 민감하지 않도록 함(&030은 민감함)

Adam with cosine annealing
1

3
2                                                               중      2        i               0 we We 8 1m 12     t      2
(2 regularization factor to be multiplied by 0.001      12 regularization factor to be multiplied by 6.001      2 reguianzation factor to be multiplied by 0
AdamW without cosine annealing                   AdamW with step-drop leaming rate decay   /                 Adar with cosine                     38

내 오조
a

CIFAR-10 path j

dae iamW

PLAY  ae

4

Test error (%)

fy DEEP LEARNING

13

무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 109 =====
2부. RNN                                                                       2.6 Optimization

들 Lion : “The Lion Optimization Algorithm (LOA): A nature-inspired metaheuristic algorithm*,2019
@ 사자들의 협력과 경쟁 HSS SHS 적용하여 다양한 최적화 BAS 해결하는 데 사용
* 부호 연산자를 사용하여 업데이트 크기를 제어하는 SSA 경사 하강 방법
ㅎ momentum?! 추적하므로 메모리 효율성 향상됨, 2차 moments 에 의존하는 Adama} 달리 ( #Px3 )
@ ^0807에 비해 성능 향상은 배치 크기에 따라 증가

Accuracy of BASIC-L on ImageNet and several robustness benchmarks

이 |                 Zero-shot                   Fine-tune
| ImageNet V2     A     R Sketch + ObjectNet | ImageNet
Adafactor |    85.7      80.6 85.6 95.7    76.1       82.3         90.9
Lion       |    88.3      81.2 864 968 77.2       82.9         91.1
89                             6.0      는
\ | ~ Lion (ours)
는 gg                                                   들
u
~                                       5.5
43 87               ~3x speedup     a
=                                                   i 5.0
wu                                    i 2.
& 86
6            ~@~ Lion (ours)
Ess          = Adamw       aa
~2.3x speedup
. 1000 2000 3000 4000       0.00 0.25 050 075 1.00
Training Compute [exaFLOPs]                   Iteration        166
wa Learning rate : AdamW 보다 3~10배 작고
/* Weight Decay rate : AdamW£=C} 3~10배 더 커야 됨(일반적으로)
a ee
^ 215                          ,                                 “Symbolic Discovery of Optimization Algorithms’,2023 ‘ee DEEP LEARNING —

들 Adafactor(Adaptive Factored Learning Rate) :
“Adafactor: Adaptive Learning Rates with Sublinear Memory Cost”,2018
® Gradient 일부 정보만 저장하므로 메모리를 덜 차지함, NLP 작업에서 흔히 사용
ㅎ Adam: RMSProp + Momentum, 2[2f2] gradient 저장함 ( #Px4 )
® Momentum: 이전 단계의 가중치 업데이트를 고려하여 다음 단계의 가중치 업데이트를 ZF ( #Px3 )

ㅎ RMSprop : 가중치의 제곱 이동 평균을 사용하여 가중치 업데이트를 조정 (#『×3)

> Adam’ 쓸 BF Optimizer= 모델 크기의 3배의 GradientS 메모리에 필요

@ Adafactor= Momentum 사용하지 않고, RMSP          ms 적은 메모리로
® Relative Step Size

@ 27| learning rate7} 주어지면, AA@ learning rate S 조절 함
® Memory size : Weight matrix7} 2d(N x M) 일때,

@ 인수 분해하여 N + M7H2| weights 저장

ㅎ Parameter dimension

/ Dense: 2d(out_f, in_f)

Convid : 3d(out_ch, in_ch, kerne

근사 Bt (=#Px2)

ㅇㅇ
~

Adam optimizer: 6,,; = 0, -

n
Vite"

¥, = B2v,-1 + (1 - B2)g?
m, = Bym,_4 + (1 - By) gat

1 sane    ae seer ene”

@한국시연구소 홍근선                       -108- 무단 전재, 복제, Wall, 디지털화 금지



===== PAGE 110 =====
2부. RNN                                                                   2.6 Optimization

% StS Learning rate                                          |
loss     }

@ Time-Based Learning Rate Schedule

@ Drop-Based Learning Rate Schedule(step decay)
@ ao 쉬워서 좀더 선호됨

low learning rate

high learning rate

|     327)      C  hetoh Give     ae |
OGG  eed)      learn  pare       | good teaming rate            woe
01                         01 om     0   .    _
0.075                                   0.075
0.05                                    005 |<
0.025                                   0.025 |
aes
ㄴ 마마
"                              4     25    50    75    100
“217          seston            ae BEEP LEARNING |

= Learning rate control
@ 학습속도는 1055함수의 모습에 따라 상대적으로 해석
Too low                                                   Just right                                                Too high

160) |            /    16) .            ;     1060) ?

8                                        @                                         6
leaning rate is toe             i
26     Jo, loss Junction      JO
Gresn's improve
as                                \
\
을                                                             이           :                                                learning rate is too high,
녁                       begins to diverge
is
6s
00
=                         …                         ww
evening rate
218                        4                                                                                                                              S8f DEEP LEARNING

@한국시연구소 홍근선                     -109- 무단 전재, 복제, Bail, 디지털화 금지


===== PAGE 111 =====
2부. RNN                                                                   2.6 Optimization

A                                                                                 CIFAR-16
= Learning rate Control methods                   :     |     3
® Cyclical Learning Rates
Maximum bound
(max_ir)
0.4                              ---Original ec
03                              ~~ Exponential
|                   Minimum bound                                                                                         —— CLR (our approach) |
0          (base_ir)                                  0       I       2       3       4       5       6       7
stepsize                                                                                                                                    Iteration                                 x10°
『  Cosine annealing                                    … elie                    “| Suen
au:                  f                   é                                    es                    ^ Hea                 23:                   al

mL  Tee.      VY

a a a ㅠㅠㅠ ㅠㅠㅠ

3% Generalization performance 향상 (optimization )

을 “OverFitting’S 막는 것 ( Overfitting : Training data] 최적화 되는 것 )

© OverfittingS 막으면 > Generalization 향상

© 모델이 S2s+H overfittingO| 쉽게 발생 vs. 모델이 작으면 표현력이 낮아짐
@ 어떻게 OverfittingS 막거나, 늦추거나, 피하거나 할 것인가?

out-of-sample error                   \
Test error
out-of-sample error
5                                                  5          |
os                                                  노
              잇반학               5
Over fitting
in-sample error
.                                                                                                        Training error
in-sample error
Complexity of the model(algorithm)                                  Complexity of the model(algorithm)
[220 _        '                    a        .           “RR DEEP LEARNING

@한국시연구소 S24                    - 110 - 무단 전재, 복제, Bal, 디지털화 금지


===== PAGE 112 =====
2부. RNN                                                               2.6 Optimization
ㅣ

= Bias-variance trade off

© 학습중인 모델에 CHS validation error                                    |
® Error(x) = bias(x) + variance(x) + noise(x)                                 A

® Bias(x) : 학습 부족으로 lst under fittinga} BA                                4    |

|

‘

^
@ Variance(x) : 00156까지 St%t over fittingz} 관련           al | ^
® validation errors 줄이기 위해 trade offS 찾아야 함           se ae a aaa naa ame
A                                                 f

Optimum Model Complexity

$                                  Variance          Ey yo    \
=                                                                                   ES             ¥
ia          ‘
Bias*
Model Complexity          "         ig     yi
MCE = Brag  ‘ VYartouce .                    “           \
221                                               j

izati

XX Overfitting 을 막는 4가지 BY (overtittingS 막는 것 = Regularization)
Approach 1: Get more data                Approach 2: Use a model with

PY Rh.
NO
wore,

m@ Approach 3: Average man

1

고           oa eee LEARNING”
- 111 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 113 =====
:  Augmentation  ：

2부. RNN                                                                   2.6 Optimizatio

2 Approach 1 : Data Augmentation : overfittingS 막는 최고의 방법 —
= OverfittingS 막고, Generalizationd sf 높이는 최고의 방법은: more data!

@ Dataset augmentation : : Generalization 성능을 극적으로 증가시킬 수 있음.
 라벨보존변환(3061 preserving transformation)

n

=

® UCR Time Series Classification:      :                   -

.   '         때    —   :   —    &        ;        DEEP L LEARNING

/& Data] label2 유지하면서 변환시키기                         리타 호
/ Data augmentation2| 기본 개념                      ee ee
® Noise 추가: DataOl| noiseS 추가하기             개
® 아무래도 모자라면 : create fake data      고 en       ~
SE ESS]
®@ Decomposition / Reconstruction          JL) Le   Ine | Wer
® AutoEncoder                              ㅣ       i       |          a   \
® Generative Models                     a eee 아며벼
* “Time Series Data Augmentation for Deep Learning: A Survey’,2020
@ httos://arxiv.ora/pdf/2002.12478.pdf
® “Data Augmentation techniques in time series domain: A survey and taxonomy’,2022
® Time Series Data Augmentation Library                                                   7
@ i soem aici anaes 거    MAIS         4        ONAL.
® Time Series Extrinsic Regression:       imeseri     ification.com/index

= “An empirical survey of data augmentation for time series classification with
neural networks”,2021 https://aithub.com/uchidalab/time_series augmentation

@ Random transformation-based data augmentation
@ Magnitude domain transformations
/ Jittering / Rotation / Scaling / Magnitude warping
@ Time domain transformations
Gaussian noise(u = 0, c= 0.03) 더하기
/-(Rotation(flipping): 50% 2] training dataS 반전
aling: Gaussian dist.(u = 1, 0 = 0.2)2] randomztS 곱하기
/* Magnitude Warping: 32¢ spline line(4 knots), knot(peak or valley): Gaussian dist.(u = 1, 6 = 0.2)
/@ Permutation: 2 ~ 5 segment 분할 및 교환.
f Window Slicing: 무작위 위치에서 90% 8 자르고, 원 Boje 보간
/* Time Warping: Warping Path 부드러운 3차 501106 line(4 knots). Knot(u = 1, 0= 0.2)
/* Window Warping: 10% 2| 무작위 구간에 대해 0.5x or 2x= warping
@ Frequency domain transformations
“+ Frequency warping / Fourier transform-based methods / Spectrogram augmentation
@ Pattern mixing
“+ Magnitude domain mixing : Averaging and interpolation, Deviation from the mean
/ Time domain mixing / Frequency domain mixing / Mixing in multiple domains
® Generative models

@ Statistical generative models / Neural network-based generative models

17 배배태배배배배대     재배   :   비이매매   베개!

@한국시연구소 홍근선                     -112- 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 114 =====
2부. RNN                                                                   2.6 Optimization

(a) time domain             (b) (time-)frequency domain

= Data Augmentation,

24-3
~ Original                        —— AAFT augmented
0    50   100            250      너    50   100   150   200   250
24
04 ^ Flipping     \n        wh      ~ IAAFT augmented          i
UVvoroy            |
\        of VU     a      |
=                    WW VN                             aS SS
fi                             °        100   150   200   250

ㅇ

i — Pown-semaling    ANA wy      ae Yala WV

ㅁ       20      40      60      ac                                  ㅁ

1509

50      3608
“Adding slope  as  |        ~   = earns via A (Mas
그             ——                 ia       FP

o         50        100       150       200       250             o         50        100        150       200       250

ee                                                                                                                          (8) Window Slicing [29]
|                                                                                               BS" abe
{d) Scaling                             {e) Magnitade Warping (30]               00 Time = Waring Bol  때      oe  ay ibid Warping [29]
Soe               :                                  Renny E ERNE”

3X Approach 2: Right Capacity, 모델이 44st capacityS 갖도록 하는 방법

= 2.1 Architecture 측면                 ㆍ 1Y3) dle   Wwodel MM .
© Layer2| 숫자와 node2| 숫자를 제한                  ~

@ 2.2 Early stopping
* 학습 Sl validation dataS 사용하여 학습 시간을 제한
® Overfitting 이전에 학습을 중단
8 2.3 Weight-decay(Regularization)
© 7SAl(weight)2| 크기를 제한
© 가중치의 squared values (Ｌ2) £= absolute values (Ｌ1)의 크기에 따라 7A] penalty 부여

@ Weight-decay (Regularization )                            The Results
A = 0.0001              A= 0.01

*  a 부과

® 모델의 표현력(학습력)을 제한
> weightZi 분포를 제어

overfitting                                                                        underfitting

philosophy: a fitie regularization goes a jong way!

@한국시연구소 홍근선       -113ㆍ 무단 전재, 복제, Bal, 디지털화 금지


===== PAGE 115 =====
2부. RNN                                                                       2.6 Optimization

= 2.2 Early Stopping: Regularizer 42S 함
@ Large model : training error= 지속 감소
validation error= 다시 증가

ast 발생          성급한 조기종료          적절한 조기종료

as        ~ Gain oss

224 > val loss

oem Bl BEE           ot  10              aL
8  「  B  x  «@  b    ° 2 “ 6 & 1060 ue
‘Spach                 epoch
EarlyStopping()                                              EarlyStopping(patience = 20)
se      _    eae        ae      “RE DEEP LEARNING”

m 2.3 Regularization (weight decay) : weightZt 분포를 제어
@ Cost function] Regularization termS Gas

LI Regularization: Cost = Costo|+ A} |w|
=

n
L2 Regularization: Cost = Costy!+ ^ Sow?
fl

® Regularization term’ 미분하면
® Ｌ1160은 : —A,ifw >0 or +4A,ifw <0
@ L2tem2: — 2Aw

® Weight 업데이트 : w < w- Acost
ㅎ L1 Regularization : 상수 만큼 증감
@ L2 Regularization :\에 비례하여 증감

@한국시연구소 홍근선      -114- 무단 전재, 복제, wall, 디지털화 금지



===== PAGE 116 =====
2부. RNN                                                                       2.6 Optimization

| 갖는 의미
® (05[를 미분하여 Weight update 할 때 \에서 상수값()을 빼게 St

@ 가 커지면 weight 가 '0'인 항이 빠르게 증가 함

@ 소수의 node7| 책임짐 > 중요한 16314[6만 사용함
@ shri           m           로동

* 사바      “                  Ne Wer a SBE tom ‘A
> 상관관계가 높을 것으로 생각되는

featureS0| 많을 때 적절히

04
골라내는 효과가 발생함    i
02
ot
00
0.1
~0.2
-0.3

= L2 Regularization (Ri                      0) 이 갖는 의미
© Cost S 미분하여 Weight update 할 때 일정비율로 빼는 효과
@ Weight7} 비정상적으로 커지지 못하게 함
ㅎㅎ weight 가 적어도 '0'이 되지 않음
@ 다수의 0006가 책임지게, 강제로 2 feature7} 사용됨
> USSEE 늦추면서 1601416들이 자기 역할을 찾을 수

있도록 조정하는 효과가 발생함, 일반적으로 Ｌ2 선호

010

005

rr     ms      때때    은   “=n” DEED LEARNING

@한국시연구소 홍근선                     - 115- 무단 전재, 복제, weal), 디지털화 금지



===== PAGE 117 =====
2.6 Optimization

Output

Boosting: 8165감소

Ensemble  -        Final Prediction

4

Mode! Stack

Bak Bowl career |
Bre Bhat
개                               Boks _ yp wh \ rn Se BEEP TEARNING™

3X Approach 4 : DropOut / BatchNormalization / GaussianDropout
= 4.1 DropOut, DropConnect(2013) : 모델의 capacityS 제한
@ DropOut2 모델 용량을 제한하여 신경망의 일반화 ASS 향상
@ Ste 좋지만 학습 속도가 느려짐
@ DropConnect= DropOutS 일반화 : \61911에서 masking
® Dropout&C} 더 249「65514@한 regularization 228 증가),
@ Dense laterOl] 적용(일반적으로 사용하지 않음)
® Ｌ5114에서는 “6041「611_9「0004『으로,유사한 효과
/ \6191110「00 : recurrent_dropoutC} 안정적

No-Drop Network                         DropOut Network                         DropCennect Network

eer wee

@한국시연구소 홍근선                     -116- 무단 전재, 복제, eal], 디지털화 금지


===== PAGE 118 =====
2부. RNN                                                                   2.6 Optimization

®@ Spatial Dropout : Conv layer 다음에 있는 Dropout
ㅎ 출력 feature mapOll 01×61단위로 masking =
 4006 &t9|(ch 단위)로 ㅠ39!100하려면
ㅎ 5021210『000마사용해야 함 : SpatiatDrapout2D(rate=0.2)

vat pak (os, Seth)
dyer  이 69464 (ra)

*
;
4

0047

rate 값            분산 72

® GaussianDropout : 출력을 랜덤하게 약화 시키기                       7             를 4 0.111

@ 24 feature map0l pineletS]= Gaussian Noises 곱하7 |

05                         25 = 1.0
rate

® GaussianDropout(rate=0.5) : x’ =x-z, z~N(1,-——)                   09              92 9.0

’4~rate’

© GaussianNoise : 주로 입력층에 사용, SHS 랜덤하게 흔들기
@ 출력 16314[6 mapOl 01×6!단위로 63455180 NoiseS 더하기
® GaussianNoise(stddev=0.1) : x’ = x + €,€~N(0, stddev*)

Sy 있음 + Growecian Neve

SRBEEE CEARNING

Bb tk

m 4.2 BatchNormalization Layer
© BatchNormalization: 학습속도 향상을 위한                          batch        saree shat

training examples
® SH 0|= (internal covariate shift)H]20|                              wo i
/* 배치 단위로 통계적 특성이 다름

} mean std

~

> 레이어 출력의 통계적 특성이 흔들림                     EEE     8    i

> 레이어가 깊을 수록 부정적 영향을 주게 됨                iolalc            ;

> 학습속도 둔화                                    Ofellelat— te] fs

@ 배치 단위로 node 출력값(활성화 A) normalizest         ※% 니디[2181 fs) [2

@ Normalize : 평균을 '0'에 가깝게, 표준편차를 '1'에 가깝게   TICE      1     1
@ 결과적으로 \의 범위제한으로 안정적 학습(학습속도 향상)

/
|<

Batch 1

버커                 SX DEEP LEARNING ”
-117- 무단 전재, 복제, lal], 디지털화 금지

Batch 2



===== PAGE 119 =====
2부. RNN                                                                   2.6 Optimization

® BatchNormalization 알고리즘
@ 1. 배치단위에서 통계적 특성(평균, 분산) 계산
@ 2. 활성함수 입력을 평균, 분산으로 00「0ㅁ281123101 하여
활성함수에 제공
@ 3.248 scaling & shifting
@ Normalize= 발생한 비선형성 감소 해결을 위해
/* 출력 값에 곱(6631109) , $t(shifting)
> 활성함수로 들어가는 값의 HAS WAS
활성함수의 비선형성을 활용할 수 있도록

> scaling factor r2} shifting factor 8 는         yi = Xi + B
역전파 과정에서 학습 (파라메터 추가)                                      ¥, 0 to be learned
@ 추론 할 때는 평균, 분산 값을 어떻게 찾나?
 학습단계의 평균과 분산 YS 평균하여 적용                                                    hi
A 또는 학습단계의 평균과 분산 값을 이동 Best 값을 적용                                   |
@ Batch 5126의 영향을 받음 : 적당히 커야 함(주의사항)                                  니그 bi)
@ #P : 2trainable+2non-trainable / node
* 장점 : 빠르고, 안정적                     o>
@ Gradient vanishing 해결, learning rate/decay rate 가속                      =  내    |         bi
총 가중치 초기화 영향 감소                                                        batch siz
@ Drop outS 제거해도 성능 유지                                                      ht \Wi

x

m Layer Normalization            %K    (명   Noyw%        Bote    arrewte WE ,
@ 동일한 층의 뉴런간 Normalization
@ mini-batch 5301010간 의존관계가 없음
@ 온라인 및 RNNO® 확장 가능
@ RNNOWPAY 효과적 (+  Trandune )
® Node & 271 parameter( 평균, 분산 2S 저장하지 않음 )

batch
           :        :     hi         hi+1
BEG                |           |

× 21212              f(ai+1+bi+1)

0904 | 0:

서미 제어

eu lags
Same for all           mean (2)(3) (3)           pes Fe ®
feature dimensions    std  (2](2][2]          |   x  Wi      x Witt

@한국시연구소 홍근선                  - 118 - 무단 전재, 복제, 4), 디지털화 금지


===== PAGE 120 =====
2부. RNN                                                                   2.6 Optimization

8 LSTM + Normalization Layer 동작
@ LSTM(units, return_sequences=True) : (bs, seq, f)  Kb OX a! Xx {  NE
® LayerNormalization2| 동작       —e           SWriih sl  Novel ord
® Sample#® feature 차원에서만 정규화, 시간축은 정규화 대상이 아님

\\
@ 따라서, f-dim72| 값이 각 sample(bs)H#=, 각 시점(660)별로 65 * 560희 정규화 됨    aaah
@ 정규화 대상 : sample, 520별 features                                                       식간321
© BatchNormalization2| 동작           o RNN 4  DatchNovre “   atch 병.   mat

@ bs * seq 단위로 정규화 하므로,
® bs * seq 개의 값이 f-dimS] 정규화 됨

/ 정규화 ASS unit’ 출력(65 * 560)개의 Zt, 시간축이 무시됨 > 시계열에 부적합

AK      =                          ( bs, 64) (bs, 4)
| model.add(LSTM(..., return_sequences=True) )   =)        는,          그    =!

model.add(TimeDist ributed(BatchNormalization()

ee -9800000때
@ 이렇게 하면, 65개의 값이 각 f-dimB= 정규화 되어 560번 HSE! seq * f-dimS| 정규화
 정규화 HAS 65개의 값, +-0107별 : 시간축 반복을 통해 평균화 > 시계열에 부적합

0 PUN t Batchtovm + Tre Dietri buted : Cea 쳐다
rRNA Hager Mow * Sample BE EL. (입격 pata Gumplea) 484

i   i     i                                                   =   *            <.  .※   plat       a   |
 > a      ¥   Peak      . . e a" 5
% Imbalanced data (비대칭 데이터 문제)              a nee oe      vote.
SMOTE ‘~        e  * e "  놀         ㆍ  « e .  려

® Deep Learning2| 일반적인 과제
® Class# data #27} 불균형
® Modelo] 227} AS classS 잘 표현하지 못함            mete
* 기본 전략                oh
® Resampling : Oversampling : 소수 classOj 대한 샘플 복제 또는 생성
@ Undersampling : 다수 01855에서 일부 4174 (Tomek links, Neighborhood Cleaning RuleS 적용)
“ SMOTE(Synthetic Minority Over-sampling Technique): 소수 sample2t interpolation 을 통해 생성
® Data augmentation: 회전, 뒤집기 및 확대/축소와 같은 변환을 적용, US sample] 수정된 버전 생성
® Transfer learning : pre-trained modelS 시작점으로, imbalanced dataset? & fine tune
 관련 작업의 사전 지식을 활용하기 때문에 잘 알려지지 않은 클래스에서 모델의 ALS 향상시킬 수 있음
® Weighted loss function :/소수 01655에 더 높은 가중치를 할당; 소수 클래스의 오류에 66021 부여
/* Weighted cross-entropy : 직관적임, 적절한 가중치 BAO] 난이도
@ Focal loss 극단적 불균형에 적합, 가중치를 자동 조정, 직관적이지 않음
® Ensemble methods : 0312의 서로 다른 54056으로 여러 modelS 학습 후, 예측을 결합
® Cost-sensitive learning : 01855별로 다른 0051 func. 적용
@ Evaluation metrics : F1-score, precision, recall, ROC-AUC, PR-AUCS, 적절한 평가 지표 사용
/* \|mbalanced datasetO|A] accuracy#C} 많은 정보를 제공
® Cross-validation2} 다양한 metricg 통해 모델 ASS 비교
@ 사용하는 전략의 유효성을 확인, 검증 해야 함

_ Tomek links   ms 6 8     2 ~ ：

ㆍ
ㆍ,
"를 고 시 세라 에,

~

YW

AL eh,

+.

(be, 4)
[개

00

wi i   ">pip Install -U imbalanced-learn .            mesma      - OR DEEP LEARNING”
@한국시연구소 홍근선                     -119- 무단 전재, 복제, 발취, 디지털화 금지



===== PAGE 121 =====
2부. RNN                                                                   2.6 Optimization

3X Imbalanced data(2)
@ Weighted cross-entropy : class 비율에 맞게 가중치 조절
———— ae
CE(pr) = —wr log (20)

from sklearn.utils import class_weight

Woe

weights = class weight.compute class weight(class weight = ‘balanced’,
classes = np.unique(train_y),
y = train_y)

4 CR Ot 8

model.fit(train_x, train_y, batch_size = batch_size, epochs=epochs,
_ Class weight={i:weights[i] for i in range(len(weights))})

~

| 1 tf.nn.weighted cross entropy with_logits( labels, logits, pos_weight ) |

® Focal loss : Hard Negative sampleOl| 가중치를 높이는 (7055 Entropy 확장
®@ Easy/Hard sampleOl 대해 가중치를 자동 조정, 극단적 불균형에 ASt(e.g., object localization),

® Cost-sensitive learning
@ ASAE 사기 검출
@ 환자 SF: Type 2 601「「0「(환자를 놓치는)에 민감하도록 가중치 설정

_239

|

3% Not enough data

®@ Deep Learning2| 일반적인 과제

® 기본 전략

ee ㄴㄱ
@ Pre-training + fine tuning 강력한 SAS 사전 교육 후, 적은 샘플 MES 사용하여 미세 조정
® Semi-supervised learning : 레이블이 있는 샘플과 레이블이 없는 HSS 함께 학습
@ Active learning: 가장 가치 QUE unlabeled samplesS 선택하는 방법을 학습, labeling 비용/시간 절감
@ Pre-training + dataset auto-generation : 사전 훈련된 SAS 통해 unlabeled samples 에 labeling

Ss

i-supervised learning : 1
Pseudo Labeling

/ 600 labeled data MNIST
model 출력에 대한 t-SNE (2)
“+ + 60000 unlabeled data
( Pseudo labeled )
model 출력에 대한 t-SNE (우)

@ 반복 프로세스로 진행, teacher model& 의사 레이블을 생성, student model= 학습

한국시연구소 홍근선                     -120- 무단 전재, 복제, wal, 디지털화 금지


===== PAGE 122 =====
2.6 Optimization

@ Semi-supervised learning

® Label Propagation : “Label Propagation for Deep Semi-supervised Learning”
/ Feature embeddings 기반으로     간의 SA       프        고,
/* Labeled 5800016에서 유사성이 있는 unlabeled 581001@에 pseudo labelS '확산', k-NN 분류기와 유사

Qn dake o\ 늘려메는 아시 .

Phase 1                                                                       Train for | epoch with
Train for T epochs with                                                   이
LX, 610

(all examples)
(labeled examples only)

Extract descriptors V       Phase 그: fterae 7” times:
Compute shanty A)
Wie Ata’

WeDo wo vs

wy “Xe > , i
Is ag?

ABA | labeis           @ : missing labels 00 @ @ @ : pseudo-iahels (size proportional to cenainty w,)

® Self-Training : “Self-training with Noisy Student improves ImageNet classification”

/* 모든 0313에 labelingO| 끝날 때 까지 반복
® Contrastive Learning : Self-Supervised Learning2| 일종
é  Positive Pair 와 Negative Pair= similarity ,  dissimilarity 학습 :  ‘Deep Representation learning 가능

a                  :                  “Sip DEEP LEARNING’
% 최적화를 위한 그 밖의 전략들
@ 다양한 시도.…

® Curriculum Learning
@ AS 문제부터 어려운 SAS, 의미 있는 SMR training 시키기
@ 시간축에서 통계적 특성의 변화가 있는 경우 적용할 수 있을까?
® Gradient noise
®@ Gradient 계산 값에 적절한 noiseS 추가 > overfittingZiz, 최적화 개선
@ NoiseRobustness 00000
@ Hidden units] noiseS #7}(Dropout, GaussianDropout, GaussianNoise=} 같이)
®@ Dataset2| labelOl] noise 추가( Label-smoothing)

기법                                                               추식                                                 노이즈 타입                                         적용 시점
| Additive Weight Noise                                 W'=W+e                                e~N(0,07)                                학습 중 Lt inference 중
Multiplicative Weight Noise                        W=W-z                              z~N(1,o7)                             주로 학습 중
DropConnect                                     W'=W-m                           m ~ Bernoulli(p)                     학습 중
Bayesian Neural Nets (Bayes by Backprop)      W ~ N(u,07)                             stochastic weight                           모든 시점
Variational Dropout                                  가우시안 드롭아옷의 일반화                   adaptive noise                             학습 중
격계예에메제대메새제에                        :          ee                  cla          ;           ;    “i DEEP LEARNING”

@한국시연구소 홍근선         -121- 무단 전재, 복제, tal), 디지털화 금지


===== PAGE 123 =====
2부. RNN

2.6 Optimization

※ 그 밖의 학습 전략

8 Multi-Task Learning (ensemble2: 같은 0313에서 결과를 모음)
$ 여러 135(에서 나온 결과를 DotA generalization 하는 것.

* 요점은 학습된 특징 값의 HSS 공유하는 것
수스 스스 ~ 시아 4

특성이 다른 504『66(185|0)의 데이터를 한꺼번에(모아서) 학습하면 어려움
@ 504[66별로 학습 시키고, 결과를 종합하여 전체 성능 향상 시키자
@ 다양한 장비 별, Lot 별로 모델을 수립하고, 특히 개별 source] data7t 적을 때 특히 유용
= Fourier Feature Embedding
® YH AlA(time index) sine/cos 임베딩 추가
& DropConnect
* LSTM(64, recurrent_dropout=0.2) 으로 유사한 효과를 볼 수 US
® Quantile Loss                   Ly aecr OY 거린 ,
@ for uncertainty-aware prediction

= Contrastive Self-Supervised Pretraining for data-scarce tasks

XX Learning rate control 실습 : CosineDecayRestarts

4 initial_learning_rate = 0.002
2 first _decay_steps = 50   # epoch
3 t_mul=1 # period 증가
4 m_mul=0.8 # peak lr GAS
5
6 Ir_decayed_fn = keras.optimizers.schedules.CosineDecayRestarts
7    _ initial_learning_rate,
8      first_decay_steps,
9      t_mul=t_mul,
10                m_mul=m_mul,
131     alpha=@.0, #1lr 최저점
2              name="SGDRDecay”, )
int 11:0.002, t:1.0, m:0.8,                                     int_rl:0.002, t:1.5, m:0.5,
0.00200 +          ~~~ ExponentialDecay step :     ete at         “=== ExponentialDecay_step
‘
0.00175 4%                              0.00175 4%
0.00150 4  *   rs                0.00150 +… *
i
0.00125 {+4}   Py              0.00125 4   도
‘   t     호
0.00100 oe |  4   |   bin         0.00100 +  *  oe
로   을      t  두    호                    A   f  개
0.00075 |     ae oe eee ce ee          0.00075 +     aE ic
도      .      ‘      ‘                   ‘
0.00050     Soong   :     A  |  ‘        0.00050 4     를 4   aS    그
+ &    \      ‘      도                   1       ‘        sn
0.00025       는      호    제        0.00025 |     wet      Mme      —
ve      도        sf      도                       ue         “ot           ie
0.00000 +       st      이      :      내      0.00000        책         Sal
0 25 «50 75 100 125 150 175 200           0 25 50 75 100 125 150 175 200
a ————————   —
244                          “                 96 DEEP LEARNIN
ㅎ         A 조그                로     =   Oc           바츠      턴히 근
@한국시연구소 홍근선                  122 - 무단 전재, 복제, $4, 디지털화 금지


===== PAGE 124 =====
2.6 Optimization

= RNNOIA{ BNZ} LN2] 적용 방식 차이

9 00061 60 = keras.models.Sequential({                            ：
10                keras.Input(shape=(time_steps, features)),        Layer (type)              Output Shape         Para &
11           layers.LSTM(1stm_units),                        Istm_22 (157)        (kes, 16)          et
12                  layers .BatchNormalization(),
13            layers .Dense(out_dense, activation='softmax')  Lote el    (ong; 16)            si
14            1 )                                                                                   (Rate
15  model_bn.summary()                                      dense_26 (Geese)       (ee, 18)
16
17 00061 10 = keras.models.Sequential({/                            Layer (type)             Output Shape         Param #
18                keras. Input (shape=(time_steps, features)),        seas Gow           ;                      -
19               layers.LSTM(1stm_ units),                                 ae see           =              _
20               layers.LayerNormalization(),                           layer_normalization9 ㅣ (Hrs, 16)              32
21               layers.Dense(out_dense, activation='softmax’) _ (v*ronmlizetion)
22         1)                                                                dense 27 (Dense)         (Hone, 30)            128
23 model_in.summary()
4: None / BatchNorm / LayerNorm
Max Val_Acc:0.9199 / 0.9268 / 0.9312                                                  Loss
0304                                     2592.09. recaline™                                                      ㅋㅋㅋ val_loss
.                                                              3004                                      — val_loss1
0.85 4                                                                                                      -———« val 10552
0.80 4
6x 107}
0.75 4
0.70 J                                             ;
=e valacc        4x 107!
0.65 5                                   ~ val_accl
_ 0601 +                          위 621, 3×10그                |
245         0      5     10     15     20     25     30                5     10     15     20     25     30 |

x Augmentation Library

@ https://gith  m/uchidalab/tim

ri
= Time Series Generative Modeling (TSGM)
® https://github.com/AlexanderVNikitin/tsam/blob/main/README,md

m

Augmentation                               Class in TSGM

Gaussian Noise /

.         .                                            tsgm.augmentations.GaussianNoise
Jittering

Slice-And-Shuffle

Shuffle Features               tsgm. augmentations. Shuffle

Magnitude Warping

tsgm.augmentations .SliceAndShuffle

5808.      ations .Magnitudeliarping
Window Warping          tsgm.augmentat ions .Windowbiarping
BTW Barycentric
"                                     tsgm.augmentations .OTWBarycentricAveraging
Averaging

ntation

sees                     ee              ee

| 246.

Method
Structural Time

Series

GAN

WaveGAN

ConditionalGAN

BetaVAE

cBetaVAE

TirmeGAN

SineConstSimulator

Lotka Volterra

PdM Simulator

Link te docs

GAN

BetaVAE

cBetaVAE

SinetConstSimulator

LotkaVolterraSimulator

PdMSimulator

1 9 비

@한국시연구소 홍근선

= 123 -

무단 전재, 복제, 24, 디지털화 금지


===== PAGE 125 =====
2부. RNN                                 2. 7 1600001000 Generation bled RNN

Chapter 2. Recurrent Neural Network
( Basic Cell, RNN Architectures )

2.1 RNN Cell Architectures

2.2 RNN Model Architectures

2.3 RNN Model Design (Time Series)
2.4 RNN Model Design (Char-RNN)
2.5 RNN Model Design (MNIST-RNN)
2.6 Optimization

2.7 Handwriting Generation with RNN

DEEP LEARNING
RECIPE FOR YOU

x RNN Application

Generating Sequences With
Recurrent Neural Networks

Alex Graves
Department of Computer Science
University of Toronto
graves@cs.toronto.edu

mae 이 natromoadl 나비
mvc Of 서0170씨 A emperanvomt

mote of vial ional, temperament

ane tb watetiel tenportmal

hove. of nah of 00070

mole  of  ver tool   temperment

se                                               surnames

248 _                     7 htos //ansi ora/abs/1308 O80 Graves PPT :hitps.//coo.aiiz7GGu Jah DEEP LEARNING”
@한국시연구소 홍근선                    -124- 무단 전재, 복제, 블     3, 디지털화 금지



===== PAGE 126 =====
2부. RNN                                  2.7 Handwriting Generation with RNN

2% MDN(Mixture Density Networks) 0|2#?
® Handwriting Generation= MDN + RNN 구조임
8 Mixture Density Networks, (bishop 1994 중심으로 설명
® Neural Network? = Inverse ProblemS 해결
* 출력을 여러 개의 확률분포를 갖는 Neural Network modelS 제안

Mixture Density Networks

Christopher M. Bishop

Neural Computing Research Group
Dept. of Computer Science and Applied Mathematics
Aston University
Birmingham. B4 7ET, U.K.
C.M.Bishop@aston.ac.uk

February, 1994

@ Inverse Problem
 일반적인 문제의 모습
@ MLP regression 0601/00「(으로도 잘 동작
MLP(20 hidden) regression net

y = 7.0sin(0.75r) + 0.52 + 6                        .          ：
Y = Woy tanh(WX +b) + bow

Training Data                                      %                         Regression Results
8                           2 Faining Data
10  = Regression Result

10

5                         5

KZ                        “5

~10                        -30

15                        -15           ：

-30    ~5    0    5    19
ne           —     see nnn     SC DEEP LEARNING

@한국시연구소 S24           -125- 무단 전재, 복제, all, 디지털화 금지


===== PAGE 127 =====
2.7 Handwriting Generation with RNN

= Inverse Problem
® x, 축이 뒤집히면, inverse problem
ㅎ Linear Regression(linear algebra)° = HS 찾을 수 없음

x = 7.0sin(0.75y) + 0.5y + €

MLP(20 hidden) regression net
Y = Woy tanh(WX + 0) + bout

Wnt Mar ayo) Ai
Cpr em”)

Traiming Data
19                =
é
5
를 0
8
Gi
-10 4 ㅎ
“35  -~10  -5  8  5  10  15
Inout

= Inverse Problem2 사례
 로봇 팔의 운동
® Forward problem : 관절 각을 알면 > 위치를 알 수 있다

“ two inputs: position (x1,x2)
/ two outputs: angles (61,62)
“ two solutions : (elbow up, elbow down)

“SEE DEEP LEARNING”

@한국시연구소 S24                       -126- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 128 =====
2부. RNN

@ Inverse Problem2| 사례

Linear regression2| 기본 가정): data2| S4'44(homoscedasticity)
@ S244 (homoscedastici

 변수들의 정규분포의/표준편차가 동일하다는 것
@  0/2444 (heteroscedasticity}——

* 분포의 변화가 있는 것

/ 현실에는 더 많이 존재힘                     서니                         ott
Heteroscedasticity
“~                                 ㆍ
ad                                *
e~                     eG
ㆍ a      =
%        foes 을
mai,  ere  i.
we
-       ;      i           …
호      26      [=      [그      |      [개
페)                       oN                        =
oe                 x   에                gos
Variance does             gq 00000 4        ee
«                                                       0.0                    02                    a4                    0.6                    OR                    1.0
not remain constant                                    y

@ Inverse Problem2| 사례

@ 헤드폰의 가격대 판매량 분포도 : multimodal(AH2| 모습/특성이 0434)

a 혼합가우시안(71416 of Gaussian) #= 임                      wenn (84413 Mixture 88% Histogram
 이 SRE 멀티모달 임
 세 개의 피크를 가짐

/* 세 개의 혼합가우시간 componentS 가짐

|            0 es | es
Price of Headphones in SUSII

= MDN 개념

® xO 대해 yo 확률분포 p(ylx)S 예측하자

® NetworkO| 확률분포 0(|>)를 표현

ㅎ 정규분포(가우시안분포)로만 표현하자

® mixture model 의 parameter(z,u,0) 를 가짐 、

 입력 ×로 SE parameter(z,u,0) 를 출력
하도록 모델을 구성하고, 학습시키자

* SamplingS 통해 최종결과를 예측                              ：
0             Hidden            Mixture               Mixture
Layer            Parameters             Disteibunon
254 _                 ~                                              on                   2 마태 LEARNING”
@한국시연구소 홍근선

- 127- 무단 전재, 복제, 4, 디지털화 금지


===== PAGE 129 =====
8 혼합 가우시안 모델의 일반화
® 『()를 혼합가우시안 모델로 가정, 개의 컴포넌트를 갖는 SAS 일반화 하면
20720 = >, me(2)M(ylaex), 089)
@ Component: 컴포넌트는 연속변수(6001104045 variables) 또는 이진변수(66「004110)를 가짐

Mixing coefficient x : sum to 1
@ meanu, variance 0: 등분산성 (입력 xB 부터 산출 가능한) 가우시안 BRS 가정

* 3개의 컴포넌트를 갖는다면

K
pet x)= Sm, (X)N(t | 44 (%),0; (8). KB

k=l

pitixde

255,

a 모델의 출력 수
* 24개 components 모델이라면, 24 x 3(x, 0, 1 ) = 72개의 출력
 출력 2= tanh (44 + bp)
@ 출력을 각 6032「2016【6「에 할당 :            2h} )
© My: B01 1인 확률 Bolas sofimax sae Who, 차.
@ ㅇ, : 분산이므로 항상 양수(18: -1~1)로 만들기 위해 expe 변환                      될            :

On = EXP(Z24~43) Ma = Zaa~71

nd

en

ero

256       Se           이박사 대타 LEARNING
@한국시연구소 홍근선         -128- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 130 =====
2부. RNN                                    2.7 Handwriting Generation with RNN

글

= Network 모델 define

1 # input features

<1 =
4 # Network                Sk=-5# FFHED 수
5 input = tf.keras.Input(shape=(1,))
6 layer = tf.keras.layers Dense(50, activation="tanh')(input) “<i=41
고
9 mu = tf. carat. layers.Dense(1 * k )(layer)            , 261   modeling
10        Ewer 16046. 10467".                     ：    1
11 # variance(sigma) He   SE (HA SS gh                  =k oo
12 var_layer = tf.keras.layers.Dense(k})(layer) (We Bre.     k=b 4     |        .
13 var = tf.keras.layers.Lambda(lambda x: tf.math.exp(x), output_shape=(k, )
14           M   Ge)        » Name='variance_layer')({var_layer)
(bey 5%
16 # pi(mixing coefficient) “BE 도스 (sum to 2)
17 pi = tf.keras.layers.Dense(k, activation=|softmax', name='pi_layer')(layer)
18
19 model = tf.keras.models.Model(inpu 2 (pi, mu, var])
구내                                   7
mput_3: InputLayer output. 6 Dr                     3   7
/
=                                    /
dese 4 Dena |e |  Fd
글     output: | ©, 50) |                             /
5    ry             i    >             "  °               2
| eve Dense  cc Bae  | ane Deuse  pee a | ame Dense  pee | 이이         …
output | (?, 51           output: | (?. 5)           output | (2. 5)        an
4           1
00 | (2.5)
variance_laver. Lambda
output | (?. 5)
oman             :                                               sensei       |
257           a      “na               dae DEEP LEARNING”

@ Maximum Likelihood Estimation(MLE)
® Data 지인 Likelihood 기여되 : P(x;,6) = x;P(@)

주황색 후보 분포에 대해 각 데이터들의 점선의 높이

$* Likelihood(7H$) :£0or £()                       ~  a a>
L(O|x) = P(X|@) = MMhar P(xxl)                           P(2\@) = Il 20010)
지금 얻은 데이터가 0분포로부터 나왔을 가능성                                                k=1
데이터 샘플에서 0분포의 +0] (likelihood 기여도)를 찾고
다 곱한 것                                                      Data distribution p(6)
@ Log-Likelihood : 1() = logL£() = logL()   i ,
(종종 1() = <*() = 1004()로표현 함 )    i   ;   ’    ;    :    :    :
l(6|x) = logL(x|@)                         아어”
= logP(x|@) = 인 logP(x;|@)      |    | |     tt
® Maximum Likelihood Estimation
@=arg max £(8)                                         Likelihood L(6|x)
보어, 0=060)이고,                                                     /                                   ，
= (칭지)/기 , 0? = 이 - 0272             ee el               f       |
3       2       A       0       1       2       3
a                 재배            TTT EINE

@한국시연구소 홍근선                    -129- 무단 전재, 복제, Sl], 디지털화 금지


===== PAGE 131 =====
a 모델의 Cost Function
© pix) = Lame (x)N(y|ux (x), og (x) : 개의 정규분포로 표현된 SZ
® 학습 대상 : 입력 ×에 대한 의 확률분포
@ 학습방식 :【개의 정규분포의 조합으로 최적의 2(>12) 함수를 만들기
@ K=32 경우, 3개의 정규분포로 x10] 대한 11의 확률분포를 표현 하는 것
® 학습 효과 측정 : y_trued| 확률분포와 7(>|2) 확률 분포가 최대한 겹치는 것

> Maximum Likelihood Estimation

=— 53             2
Training Data     \ ph        P(W1) = jar We (X1)N Ue 1), 7% (41)

|       é

i      a 해이
’       i
!       '
| Oy         H
ag exaneasnannncnan Tene4       |
i       1
i       i
을                              las     i
|       i
}       i
『       i
¥       |

/                       나    | |
t       i
6646~       Hi
i       '
『       i
H       :
       |

26321)    202)

1 aa   를    |    =     eK DEEP LEARNING

2부. RNN                                  2.7 Handwriting Generation with RNN

* 학습 효과 측정 : y_trueS| 확률분포와 2(>|)확를 분포가 최대한 겹치는 것

> Maximum Likelihood Estimation (P(x|u,0)) : sample xB 표현하는 최적의 uw, 0를 찾는 것

® Cost func. : 예측된 확률분포 27(>1)와 SHU y_true9| log LikelihoodS 사용
> Cost Function oe —log (SE Tn) POerue M(x), o(x))) ZB 정의 Bt
/* 출력 [1, 0 로부터 계산 되는 확률분포 0(/_ㅁ60) 와 YE y_true               밀도
(joint 01590164100)를 구하고( 가중치 [1,(3)적용하여), -log )적용
* calc_pdf(): 결합 확률밀도 7(7,,』<1/6,ㅇ,) 계산                              Cs
@ Likelihood 기여도 : pyeruell4x: Fx) = N(Ux, x) Verue) = ic erp Led 0      4, 4    Ye
He .

2 ## By trues BOA FRIAS EY Besse FE /옥은은노 사신 Retum 같은 각/ trueoll cist
3 def calc_pdf(y, mu, var):                     #(n,5,5)   eae te aence
4     “""Calculate component density"""                      | 의 확률밀도 값이 5개의 학습된
5    value = tf.subtract(y, mu)**2  #(x - mu)*2            r=     aaa   역할
6     value = tf.math.exp((-1/(2*var)) * value)
7     value = (i/tf.math.sqrt(2 * np.pi * var)) * value
| 8     return value #yOf of 4 5.49/ 확윤일도 CE AF #(n,5)
ce | icemortte      0              :       -     = RR 마태 LEARNING”

=|

i

@한국시연구소 홍근선                 - 130 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 132 =====
2부. RNN                                   2.7 Handwriting Generation with RNN

® loss 계산 : CostFunction(y|x) = —logL = —log(ok TI, (x) p(y, u(x), o(x)))
@ 각 분포(출력값 oS 표현된)와 /_[ㅠ46의 결합확률 밀도를 계산하고,

값에 가중치(01)를 곱하여,          #(420,5,1)
@ 571 componentSS 모두 더하고, #(420,1,1)
@ -Ｌ09(정보량화) 후, 평균(기대값)을 취하여 batch] loss Z(scalar)S 리턴

| 36               ㆍ NOmu, var) OFA) y PBs!    AGA 72,                    ㅣ
| a2            ) & recuce_sum -> Loss                          |
| 32 def mdn_loss(y_true, pi, mu, var):               #(n,5,8,5)

fas     out = calce_pdf(y_true, mu, var)              #(n,5)<-(n, 5,5)
14     out = tf.multiply(out, pi) # Beg ssp   & #(n,5)

145    out = tf.reduce_sum(out, 1, keepdims=True)     #(n,1)

| 16     out = -tf.math.log(out + 1e-16)              # -Log(n,1)

| 47     return tf.reduce_mean(out)                     #(1,)

261         =      내                                  :           Six DEEP LEARNING

a 24! Training
@ 모델의 SHO] 많고, !055계산이 복잡한 경우에 주로 APAVSEE Training 방식

#fraining Loop
for epoch in range(EPOCHS):
for train_x,trainyin dataset: # data Load

loss =\train_stepdmodel,  optimizer, train x, train y)/ #4
losses. append(Ioss)

i @tf.function,

2 def train step(model, optimizer, train_x, train_y):

3     # GradientTape: Trace operation   OES,   e gradients

호     with tf.GradientTape

5       pi_, mu_, var_ =

6        # calculate Loss

Z       less = mdn in_logs(trainy, pi, mul, \ var.)

8     # compute and apply gredies

3     gradients = tape. gradient(loss, model.trainable va                ;
ig  ¢ rtind co agedy_acodierts ipUGradTende, nodal. Urainablevardables))) #7
ii     retary 1655

@ Data pipeline 구성

1 : DataSet #4): Use Dataset APT
2     = flipped_x.shape[@]
2 eben =   tf.data.Dataset.from_tensor_slices((flipped_x, flipped_y)).shuffle(N). batch(N) |

.RNING

Cee See ee

-131- 무단 전재, 복제, Sl, 디지털화 금지



===== PAGE 133 =====
2부. RNN                                   2.7 Handwriting Generation with RNN

= Sampling 학습된 확률분포로 부터 SHU 찾기
4 # Prediction’ © 3 parameter 신주

5 pi_vals, mu_vals, var_vals = model.predict(x_test)

6 # parameter EAS ISLE samplings of 안가

? sampled_predictions = sample predictions(pi_vals, mu_vals, var_vals, 10)
&

5

#sampLed_predictions.shape : (420,10,1)
fig = plt.figure(figsize=(6, 6))
10 plt.plot(flipped_x, flipped_y, ‘ro’, label='train')

ii for i in range(sampled_predictions.shape[1]): # 1     |
12     plt.plot(x_test, sampled predictions[:, iJ, ‘'b.', alpha=@.3, label='predicted’)

@ 확률 parameters 받아, test samples(420) x samples(10)7H2] sampling 결과 리턴

2 def sample_predictions(pi_vals, mu_vals, var_vals, samples=1@):           |e 재아
2     n, k = pi_vals.shape #:426, k:5                                 ar
3     out = np.zeros((n, samples, 1)) # (420,16,1)
4     for i in range(n): # #in_sample(42@)
5
6
7?

for j in nee eae)
a

& Training 중 중간 A2t= sampling 및 Parameters 확인 하기

[1499] Sampled Results        [1499] Means : Mu(x)       [1499] Mixing Coeff. Pi(x) [1499] Variance Coeff. Pi(x)
06                     ~

05
04
03 +4
02 T+

6 8 0 8 8

ol

00 +7
   +    +    +   7    r    >

-10         0                   -10         0          10       -10          0          10  -10          0          10
[5999] Sampled Results       [5999] Means : Mu(x)       [5999] Mixing Coeff. Pitx) [5999] Variance Coeff. Pi(x)

oO

-10           0            10         -10           6            10        -10            0            10

[|

@한국시연구소 홍근선                     -132- 무단 전재,


===== PAGE 134 =====
2부. RNN                                  2.7 Handwriting Generation with RNN

8 Training 결과가 좋지 않을 결과 : 종종 좋지 않는 결과가 발생
[5999] Sampled Results       [5999] Means : Mu(x)      [5999] Mixing Coeff. Pi{x) [5999] Variance Coeff. Pi(x)
|               25
08
063                              15
04                             10
02                               5                        /
00                             o>
-10         0         10       -10         0         10                                      -10         0          10
@ 초기값의 SH: 해결이 쉽지 않음
® Overfitting : 학습속도, model capacity, dataset
/* 빠른 학습속도 : 초기에 weightZt0| 6185되는 경우(초기값에 Overfitting) vs. modelo] 너무 큼
- Learning rate 줄이기 0 learning rate scheduling
/* Regularization 42(weight decay) : Ｌ1, L2 42°2 weight 4S control
“ Model capacity 줄이기 : node/layey 줄이기, Dropout, Regularization
/ Batch Normalization 적용 : Weight bias, vibration control
> 7|2AL= components7} 너무 AS!
…       :       nena nn

= Overfitting 해결하기(예) : k=52 고정된 경우
@ Model Capacity / Model learning rate / Weight learning balance / Data Augmentation
1) Regularization(weight decay)42 + Learning [216 낮추기

5 input = tf.keras.Input(shape=(1,))

6 layer = tf.keras.layers.Dense($8, activation='tanh') (input)

7 ## 00 MB lf

를 mu = tf.keras.layers.Dense(1 * k,  Fornell _regularizer=keras.regularizers.12(@.2)) (layer)
9 # variance(sigma) 중 £E (BAS       20)

19 var_layer = tf.keras.layers. 리타,  (60061_「684120「120『「=6「005 .「664233012005 21(9 01) )(13760 )
li #ver_lLayer = tf.keros. layers, Dense(r) (Layer)

i2 var = tf.keras.layers.Lambda(lambda x: tf.math.exp(x), output_shape=(k,)

13  , name=‘variance_layer' )(var_layer)

314 # pi(mixing coefficient) 4    의 (sum to 1)

15 pi = tf.keras.layers.Dense(k, activation=‘softmax', name='pi_layer’,

16                              kernel_regularizer=keras.regularizers.12(8.2))(layer)

17 model = tf.keras.models.Model(input, [pi, mu, var])

i8 optimizer = tf.keras.optimizers.Adam( learning rate=9,9905 )#default:@.ee1

2) Model 줄이기

5 input = tf.keras.Input(shape=(1,))
6 layer = tf.keras.layers.Dense(3@, activation='tanh') (input)

3) 학습 방해 하기 : model capacity HS}, ensemble 효과 (학습이 늦어짐)

| § input = tf.keras.Input(shape=(1,))
| 6 layer = tf.keras.layers.Dense(5@, activation='tanh' ) (input)
|? layer = tf.keras.layers.Dropout(@.2) (layer)

@한국시연구소 홍근선                   - 133 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 135 =====
2부. RNN                                   2.7 Handwriting Generation with RNN

%* Prediction Architecture : 필기체 생성을 위한 예측기 구조

output                    < Deep RNN Architecture >
layer                                 m RNNS 사용하며 하나 이상의
=             hidden layers 2} skip connections 사용
eo             Bw BAS 한번에 하나씩 주어지고
LSTM                   ~            출력은 예측 값의 확률분포

CP       다음 입력으로 사용
sn Modele

mos SO) Nowe
NOD Le eer 카이,

0660 RNN prediction architecture
= Generation= 출력에서 sampling 되어 입력으로 공급되는 과정

Outputs                                                                            *Probability of sequence x
을

Pr(x) = ] ] Pr(ersilye)
tl

*Sequence loss L(x)

T
tid =- log Pr(zep ily)

fi

Hidden Layers

Inputs.

06. ×.9

@한국시연구소 홍근선                     -134- 무단 전재, 복제, 23), 디지털화 금지



===== PAGE 136 =====
2.7 Handwriting Generation with RNN

j: mixture components

Mixture Density Network
: 혼합밀도 함수의 조합으로 예측

2부. RNN

_2.7 Handwriting Generation with RNN

yt=( 획 확률 6,
{혼합 가중치 xj,

평균 yj,
표준 편차 이,
상관계수 pj} )

% Handwriting Prediction
poco co me -----------
xt = Pen 위치 (xt = x1, x2),

I Outputs
Hidden Layers
획 상태 (x3 : 획을 SUH 1)
inputs
End of stroke as Bernoulli
gp TTT200           |
|         ;   1   iif (ra le = 1
P         ,              r         jo     ;    t             t+1)3
Pr(cze+ilye) = pe wy N (resi |i. 07. pil                      .
=                     i[ L—e,, otherwise
| hr
Next pen displacement as mixture of Gaussians
269                                                            Mixture Density Network 설명자료 : httns://oo0 al/diisTx  xe DEEP LEARNING

X€ Handwriting Prediction
= Mixture density outputs(density map)

mixture component weight :
측은 획 중의

획의 끝점 예

가장 SSAA 구성 요소가 세 곳에서 단절
| 예측과 다

- 135 =  단

5]

[건

    Ph 0 대사마
재, 복제, S4], 디지털화 금지



===== PAGE 137 =====
2부. RNN

2.7 Handwriting Generation with RNN

3 Handwriting Synthesis

= Prediction network? 2 불가능
 문자의 길이에 따른 필기체의

변화가 너무 크다
> ‘Soft window model 을 적용한

Handwriting Synthesis network 개발

iy)
Gore Comp, & TH eel

VY

nde

님          (24~  ye AX om Ane  ; pipers ‘

;              해:    ㅣ
^        Aig    Wig  (A FA.
4 gare cm ene d.     {
,      Sn cuarre DT mA 6
a Loan &, 7
et  Bou 4                      “~

+             /
-   np    ler &£   ad
\       cri dtr 6S err ay
pore i Ui yPaeee      .
E5 with Cre

))     iB    wy
bof ^ 4   bak oh  (amu sae

a

‘

>)-.f7   Ca hod    ^          5        ,
ALE               e +—~    ae               jt

ov le  Satet   [Jenuig 7S Som ~~,   In a

0

\       pa |
ave & ye  0 | %9 . , ead

때  is       <p

xf Synthesis Network + Heuristics

를 Soft window :

U
we = >: O(t, ucu

길이 UX] 문장 ce      u=1

c 에 대한 에서 \, = 각 char7} 적절한
에 있도록 유도하는 확률분포가 됨

- Sequence c: {c_1, c_2, ---, c_U}

- Sequence t: {x_1, x_2,--, x_T}

Window weights during sequence

Thought that the muster from

Generation with RNN

Hidden 2

Hidden 1

-136- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 138 =====
2부. RNN                                 2.7 Handwriting Generation with RNN
_2.7 Handwriting Generation with RNN

% Conclusion

LSTM is important in now days
LSTM is important in Now days

RNN is a deterministic model

Rn 1S O delerministic model

However, it is also possible to generate sequences

Heuristics are required for synthesis            |
Leuristics  are  requived Jor  synthesis

Has a lot of opportunity

tlas a \ot of opportunity

mir          !            a     cai          mesa       Met cid cinch

_Chapter 2. Recurrent Neural Network

= 2.1 RNN Cell Architectures

@ Basic RNN cell, LSTM module, GRU unit
® Cell architecture, #Parameter,
® BPTT Training sequence, BPTT vanishing problem, TBPTT(Truncated BPTT)

=@ 2.2 RNN Model Architectures

® One to many, many to one, many to many model
® return_seqeuence, stateful / stateless , layer. TimeDistributed()
ㅎㅎ layer.RepeatVector(), LSTM AutoEncoder

© Parallel, Stacked, Bidirectional, Residual, Dense LSTM, Seq2Seq
@ 2.3 RNN Model Design (Time Series) 실습 : 4 가지 모델
= 2.4 RNN Model Design (Char-RNN) 실습 : 4 가지 모델
m@ 2.5 RNN Model Design (MNIST-RNN) 실습 : 3 가지 모델
= 2.6 Optimization : Weight initialization, Hyper parameter search, Optimization Algorithm,
Regularization , Learning Rate schedule , Dropout
@ 2.7 Handwriting Generation with RNN
@ MDN(Mixture Density Network) : Inverse Problem, Mixture Gaussian model
® Deep RNN + skip connection Architecture

@한국시연구소 S24         - 137 - 무단 전재, 복제, 24, 디지털화 금지



===== PAGE 139 =====


===== PAGE 140 =====
3부. Time Series & LSTM


===== PAGE 141 =====


===== PAGE 142 =====
3부. Time Series & LSTM                                           3.1 Time Series 개요

Chapter 3. Time Series & Other Architectures

3.1 Time Series 개요

3.2 Time Series Analysis

3.3 TCN and Other Architectures

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.5 Time Series Classification

3 EP LEARNING
RECIPE FOR YOU

% 시계열 데이터 (Time Series)
6 특징
© 시계열 데이터 : 관측 값이 시간에 따라 변하는 자료
: 온도, 습도, 바람, 기계의 진동, 주가, 주가 수익률...
* 시계열 자료의 특징 :                             ae       이
@ 인접된 값들이 상호 종속적, 현재는 과거에 종속 : 완전 독립적 시계열( 백색 잡음)
@ 일반적인 통계 이론이나 통계적 분석 방법으로 다루기 어렵고,
별도의 시계열 분석 (Time Series Analysis) 방법을 사용
@ 자연적, 인공적 정보 중 변화하는 정보는 대부분 시계열 자료의 SYS 가짐
@ 경제,금융 시계열 : 통상의 시계열 자료 (월별 출생자수, 태양의 월별 흑 점수 등) 보다 복잡한 구조를 가짐
w 시계열 분석의 목적
© 자기종속 구조를 파악(전통적인 접근)하고, 표현하는 Model 개발
> 미래의 값이나 상황을 예측하기 위해
> 변화 감지, 상태 판단을 위해

Standardized Temp (2)

1950         2000

New Representations

Original Time Series                                                                                     :                                 Downstream Tasks
(representation space)
Ｌ   wow   we        hohe                                  =   뽀  :  |                   ㆍ
_ 282                                                 se bad
@한국시연구소 S24                     -141- 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 143 =====
3부. Time Series & LSTM                                             3.1 Time Series 개요

w 시계열 데이터의 특징 : 표현하는 주요 BOS
Trend) : 시계열 자료는 같은 방향으로 직선이나 곡선을 따라 상승, 하강하는 경향

@ 경제, 금융에서 나타나는 성장 (ㅁ8이나 증가 등으로 발생 ( 결정적 추세 / 확률적 추세 )
@ 결정적 추세 : 시계열의 평균값이 시간의 함수
@ HEA 추세 : 특정 시구간에서만 과거 값들의 종속관계

© (AH (Seasonality) : 절기나 분기 또는 연, 월, WHS 관측되는 정보는 시간에 상관됨
@ 계절성은 긴 주기의 순환과정을 갖는 주기적 SSS 포함

* \이변성/(&66「7ㅠ8100) : 일부이긴 하지만 관측 값이 일반적인 패턴에서 크게 이탈하는 경향
@ 단순한 이상 값으로 보기보다는 순간적으로 근본적인 확률구조의 변화가 발생하는 것
@ 시계열의 예측모형 개발에서 예측 오차를 최소화하기 위해 반드시 고려해야 할 사항

(Volatility) : 분산이 시간의 추이에 따라 변하는 성질
@ BASS 시계열의 대표적인 특징. 새로운 정보의 유입, 해석 및 외적 사건의 출현으로 야기됨
@ 불확실성 및 위험 (0150)을 설명하는 수단
* \비선형성 0400110ㅁ6806) : 값들의 종속 관계나 인과 관계가 비선형관계로 설명되는 것
@ ZA(event)o] SHS 주는 정도가 강도에 비례하지는 않으며, 서로 반대가 될 수도 있음

:        ame        SEE LEARUNG

a AAS 분석 방법
* 일반 시계열 자료 : 종속 구조가 주로 시간에 따른 평균에 의해 설명됨 . 역고! TH.
© 금융, 경제 시계열 자료 : 종속 구조는 평균은 물론이고 변동성을 설명하기 위해 이차적으로
시간에 따른 분산, 표준편차들 사이의 종속구조까지 분석 필요
© 강한 일반화 필요 : 동일한 기간, 동일 장소에세|독립적인 반복 관측이 허용되지 않음
관측된 한 계열자료만을 사용해야 하기 때문에 더 일반화된 이론이 요구됨
© 시간영역 분석 방법 : 인접한 자료 사이의 종속성, 상관성이 BAR 회귀한다는 가정
추세와 같은 결정적 요인 + 잡음과 같은 확률 성분으로 분석
PRA Ae, Se)
* 주파수영역 분석 방법 : 평균이나 분산 SO] 비교적 안정된 정상 시계열을 대상으로
주기함수들의 일차결합으로 분해하여 모델 구성

주기 함수로 시계열의 주기성을 파악
( Fourier, Coherence, Wavelets
“ely

yer Wa -

@한국시연구소 S24                 - 142 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 144 =====
3부. Time Series & LSTM                                            3.1 Time Series 개요
3.1 Time Series 712. __

BAIZSS 분석 방법 (고전적 시계열 모델)
* AR(Auto Regressive) 모델 : 자기 회귀 모델, 현재는 과거에 종속된다는 모형
@ 종속성이 없으면 독립적이며 백색 잡음 (white noise) 시계열이 됨
ㅎ 데이터의 자기상관성을 분석하기 위해 사용
® MA (Moving Average 모델 : 현재는 과거 잔차 들의 가중 평균이라는 모형
@ 잔차는 백색 잡음, 그러므로 현재는 과거 백색 잡음들의 평균값으로 설명 됨,
@ 백색 잡음들은 BI (Stationary)o| 높고 평균회귀 특성을 가짐, 이 모델도 평균회귀 특성을 가짐
® ARMA 모델 : AR+MA, 두 모델이 평균회귀 특성이 있음, ARMA 모형도 동일함
@ 88a (Stationary)S 갖는 시계열 분석에 적합
@ ARIMA (Auto Regressive Integrated Moving Average) 22 :
@ B84, 평균회귀 특성이 없는 AAAS 차분하면, 평균회귀 특성을 가질 수 있음
@ 차분 시계열에 ARMAS ASS , 주가를 차분하면 주가 수익 시계열이 됨
® SARIMA 모델 : 주기성 (Seasonality) 을 추가함, 자기상관성을 분석하여 주기를 검출
@ 주기적 시간(일, 주, 월, 년,..)과 관련된 데이터는 주기성을 가짐
> DAAC 시계열 SAS 적용하려면
- 시계열의 분포와 특성에 관한 엄격한 가정, 검정이 필요
- 시계열의 SAS 이해하고 적용하지 못하면 효과가 매우 제한적임
- 경제, 금융 시계열은 매우 복잡하고, 비정통적이며, 매우 노이즈가 많음

285                                                                                                                                                                0660 LEARNING

Toes 상서, 2 .

. 3.1 1106 Series 개요

8 시간영역 분석 방법의 성능 : 데이터특성을 분석하며 진행
@ AR(Auto Regressive): AR(p) + Xp = 01421 + 02422 + a3Xp3t¢-- te ALM w

ㅎ MA (Moving Average ): MA(q) : 현재는 과거 잔차 들의 선형 조합
X =; + 26 “lhe bye¢-4 of 220-2 pes   7 ays ,
* ARMA 모델 : AR ? MA      aU Ne   Za                           |
ARMA (p,q) : 세 = a, Xp—1 + 0 Xy_g + …시-, + 6 + 16,3) Doe + 아가 의,
* ARIMA 모델 : 차분 시계열에 ARMAS 적용

ㅎ SARIMA 모델 : 주기성 (Seasonality) 을 추가함
ARIMA  (2*9.9)       (P, D,Q)m
@ 유로17국 분기별 소매거래 지수, 예측에 AS                                =      느니

모렐의          모델의    magn
—\

|
;

2번 차분한 결과                  ARIMA(0,1,3)(0,1, 1) 22 얻은 예측값

286      '     ni            __ https://otexts.com/fppkt/non-seasonal-arima.html xx DEEP LEARNING
@한국시연구소 S24                  - 143 - 무단 전재, 복제, 24], 디지털화 금지



===== PAGE 145 =====
3부. Time Series & LSTM                                             3.1 Time Series 개요

wa

너

mw 주파수영역 분석 방법 : 자세한 설명은 하단 [참조
® Fourier transform : 데이터의 주기성을 주파수 0070811으로 변환, 주파수의 Foe 모델링
@ 144 주기 peak    4

홍역 발생 추이    .    |      주파수로분해

 변화에 둔감   g                       F}     |
;                 3    |
&   |

으으으 으응 속으 이 ip 8 0 | ㅣ  ; 4

® Coherence(L#4) : 신호간의 상관관계를 의미, UZ! (stationary:As) SYS 표현
@ 변화 분석에는 부적절, 일관성의 변화 분석 가능
https://en.wikipedia.org/wiki/Coherence_(signal_processing)
® Wavelet transform : 여러 scale2| 0313에서 주파수 정보를 추출, 변화에 민감한 분석 가능
SS 으으으 고 6 Oo 새

4         ㅇㅋ
|     Lee       3]
4  pr ie 머   $4        .
|   x   wee
LX XxX   Na?

287

@ Wavelet transform : 여러 scale2| 0313에서 주파수 정보를 추출, 변화에 민감한 분석 가능

“|
eee

7.
g,
Scale

| 다비] aaa Pret 20000 |          Time
1 99909 | Wavelet Analysis  】
LR RL Abarer tive dows 4B
      ne     | oh ol ial

7 SG) Se SS Se I A A

A
_                       1
@한국시연구소 홍근선                      - 144- 무단 전재, 복제, Bay) 디지털화 금지


===== PAGE 146 =====
3부. Time Series & LSTM

3.1 Time Series 개요

3.1 Time Series 개요 _

Level

=
3

~~ i Mm

a
Level 3

® Wavelet transform

5) ©

(42

Level 2

w)—>  Level 1

coefficients

Frequencies Samples
0 to f,/8
fn/8to fr/4 4
fa/4 to fa/2 8
fn/2 to fr

4

16

Level i

Levelt 2
—                coefficients

\_}

Bi

Level 3
coefficients

~ 289

노블: 빨.

‘Lawl

meds. DEEP LEARNING

_3.1 Time Series 개요

= Quality Metrics

|  Metric  |                Meaning                |        Formula         |
MSE             Mean Squared Error              mean ({y — ¥)*)
R         Coefficient of Determination        1 — MSE / var (y)

RMSE         Root Mean Squared Error                   MSE
NRMSE             Normalized RMSE                RMSE/mean (y)

MAE            Mean Absolute Error               mean (|y — 위)

MAPE | Mean Absolute Percentage Error | 100 mean eae |
sMAPE              symmetric MAPE              200 mean   분 : 4

MAE(model
MASE       Mean Absolute Scaled Error          aAER a
290                              브러                                                                                                             Soe DEEP LEARNING
@한국시연구소 홍근선                    - 145 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 147 =====
3부. Time Series & LSTM                                             3.1 Time Series 712

= Time-Series Analysis 분류
® Time Series Classification
@ Time Series Clustering

® Time Series Regression
@ 과거의 데이터와 다른 HFS 간의 BAS 분석하여 미래의 AS 예측
 과거 데이터(독립변수)의 미래를 예측

 시계열 데이터 내부의 MHS 분석하고 예측하는 데 사용
® Time Series Extrinsic Regression(A|A|S 외재/외인성 회귀)

© 시계열 데이터와 wate 설명하기 위해,외부 요인을 고려 >
* GDP, 실업률 등의 외재 변수가
소비자 지출과 같은 시계열 데이터에 어떻게 영향을 미치는지 분석
 외부 변수나 독립 변수가 시계열 데이터에 어떤 영향을 미치는지를 분석하는 기법
 외부 변수를 포함한 독립변수로 새로운 변수의 미래를 예측
/* 목표 변수가 독립변수(입력)로 포함되면 일반 Regression model0| 됨
ㅎ 외부 변수의 영향을 고려하여 시계열 데이터를 분석하는 데 사용
> Extrinsic 869165500(외인성 회귀) : 외부요인/변수가 종속변수에 미치는 SHS 분석
> Intrinsic Regression (내인성 회귀): 변수들 간의 내부적 관계를 분석

“Deep Learning for Time Series Classification and Extrinsic Regression: A Current Survey’,2023
“Universal Time-Series Representation Learning: A Survey”,2024

291  ssi   :       오브 비보 CARNE 3 I nN

x

8 Deep Learning 에서 접근하는 주요 구조           이매 절보를 yeaa sae 72
oe oe                        (즉,과거와현재의 정보만사용)
( 시간정보를 통합하는 구조 측면에서 )

Dilated causal 0
1) TCN: Temporal Convolutional Network             Outputs

“yh            CNNS Time 56065에 적용                              Convolutional ,

®@ hidden layer 의 S42                         i 2.    é       >  안서 [ )
pitt = 4 ( 와 10000 wo ht.            Layer       2     수 ~
      Poke       (Lt) Rear )       seen     e6 S   e   ee

A: activation func. 07: dilation rate
RNN Mod

‘ 최종 Output & encoding! 값 2, = hi 로 표현 가능     Outpats   @ 2 | & @ 8 =

We 2) RNN Model

3) Attention-based Model                                      개 기구 EEE 는

® Long term dependency 개선

oat Rot 성능 개선 효과                ms 00000000

S 과거의 중요한 시점의 정보에 집중 가능                                   Attention-based Model
ag    ey-value lookup based query       Outpus @ OO COO    @ Dynamic
* Attention
h,= pe (Kp, Ar) Ve-r                       oS 을 @       Weights
ny        a(): attention weight              때       ee         때
Encoder        A
a           k,: key, 0: query, 다: 7071           Layer    은 든 [|  :          :
Carats         inpts 00000000
292. 일반화하여지청 _                                            XX DEEP LEARNING

@한국시연구소 홍근선                     -146- 무단 전재, 복제, 발춰, 디지털화 금지


===== PAGE 148 =====
3부. Time Series & LSTM                                          3.1 Time Series 개요
8 Time-Series ForecastingS 위한 주요 Sas
“A Survey of Deep Learning and Foundation Models for Time”,2024
¢ 모델의 유형 분류

Neural Network                         Neural Network                         1988
< 파리 1)                    Recurrent Neural Network              1989
FDA/FTSA          Functional Data/Time-Series Analysis 1991
CCNN)                    Convolutional Neural Network            1995
SVR                          Support Vector Regression                 1997
TM)                    Long, Short-Term Memory              1997
ELM                       Extreme Learning Machine              2007
Gated Recurrent Unit                  2014
E)  €oder-Decoler          Encoder-Decoder with Attention          2014
MGU                           Minimal Gated Unit                   2016
( TCN/                Temporal Convolutional Network         2016
GNN/GCN           Graph Neural/Convolutional Network [2016
vIRF                           (Vanilla) Transformer                  2017

ees

= Time-Series ForecastingS 위한 주요 모델들(2)
© Transformer 계열의 주요 모델

LogTrans                    Local and LogSparse Attention             2019
Reformer         Only Similar Queries and Keys Are Compared 2020
Informer                      Uses Selected Query Prototypes             2021
Autoformer _ [Replaces Self-Attention with Auto-Correlation| 2021
Pyraformer                  Hierarchical/Pyramidal Attention            2021

Series Stationarization and

iimilidesiaisie                  Use of De-stationary Attention            2022
Triformer           Triangular Structure for Layer Shrinking 2022
CrossFormer                        Cross-channel Modeling                   2023
——— 0
(PatchTST ¥;            Replaces timestep inputs with patches        2023
4           년
Ayr, 분란

@한국시연구소 홍근선                  -147- 무단 전재, 복제, Sl, 디지털화 금지



===== PAGE 149 =====
3부. Time Series & LSTM                                             3.1 Time Series 개요
a

를 Time-Series ForecastingS 위한 #2 모델들(3)
@ Representation Learning for Time-Series #2 모델

TS2Vec                Local and LogSparse Attention            2022
CoST  |Only Similar Queries and Keys Are Compared | 2022
FEAT                 Uses Selected Query Prototypes            2023
SimTS _ [Replaces Self-Attention with Auto-Correlation} 2023

® GNNAS 주요 모델

GCN [56] | Graph Convolution Network        f(x; (did;  -tWh j)        2016
Message Passing                        ：         ：

MPNN [27]        Neural Network             f(hj, Xj mji)        2017

GAT [119]        Graph Attention Network              (Xj (aij Why))            2017
GraphSage [32]| Neighborhood Sampling         algorithm 1 in [32]       2017

GIN [133]  |Graph Isomorphism Network| —_ equation 4.1 in [133]       2018

TGN [103]      ‘Tempore! Grup . raid   embedding equation in [103]|2020

(dynamic)
enn    pace     Tae Beer PERRO

= Time- Series ForecastingS 위한 주요 모델들(4)

ㅎ Type 1: 대규모 언어 기반 모             고 시계열 데이터용으로 『106-14116
@ Type 2: 시계열 데이터 세트에 대해 광범위하게 사전 학습, Lag-Llama(open source project)

® Type 3: 특정 도메인의 시계열 데이터 세트로 사전 학습
@ 19064: 뉴스 등 텍스트 및 시계열을 사용한 다중 모드 사용하여 OSS 개선할 수 있는지 확인

Model Type       Model       |              Short Description              | Backbone |   Date  |
2        ‘TimeCLR [136, 137]        Contrastive Learning pre-training       ‘Transformer| Jun 2022
2           TimesNet [129]                  2D variation modeling                TimeBlock | Oct 2022
1             GPT4TS [153]                LLM with patch token input                GPT-2 [May 2023
1              LLMATS [14]               Temporal Encoding with LLM               GPT-2 [Aug 2023
4           (UniTime [714 )      Input domain instructions + time series        GPT-2  |Oct 2023)
2             TimeGPT [26]            Added linear layer for forecasting        (Transformer| Oct 2023
4           cFime-LLM [44])           Input context via prompt prefix             LLaMA | Oct 2023
2         ~PreDet [20]                 Patch-based Decoder-only            ‘Transformer| Oct 2023
2           Lag-Llama [100]                Lag-based Decoder-only                 LLaMA | Oct 2023
3            AutoMixer [90]              Adds AutoEncoder to TSMixer             TSMixer | Oct 2023
1             TEMPO [12] __Pre-trained transformer + statistical analysis) _GPT-2 | Oct 2023
296.            1           PromptCast [134] | Text-like prompts for time series with LLM | GPT-3.5 |Dec 2023/7

@한국시연구소 홍근선                   - 148 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 150 =====
3.1 Time Series 개요

8 주요 모델 성능 비교

m              mn-           a            이        i-n         -f

“SegRNN: Segment Recurrent was Network for Long-Term Time Series”,2023

IRNN bate
Categories |               RNNs               |   Transformers 7       |          MLPs          |         CNNs
er    SegRNN    DeepAR     GRU     PatchTST © FEDformer —_ Informer     TIDE     Diinear     MICN    TimesNet
ai         (ours)           (2020)          (2014)          (2023)           (2022)          (2021)          (2023)           (2023)           (2023)          (2023)

Metric | MSE MAE MSE MAE MSE MAE| MSE MAE MSE MAE MSE MAE | MSE MAE MSE MAE| MSE MAE MSE MAE

_ | 96 | 0341 0.376 1.128 081 1.126 0831 | 03) 04 037 0415 0941 0.769 | 0375    -         aT
| 192 | 0385 0.402 1.077 0.776 1.133 079 | 0.413 0429 0423 0446 1.007 0786/0419 gan] \          So
5 | 336 | 6401 0417 1.043 0.766 1.053 0.774 | 0422 044 0.444 0.462 1.038 0.784 | 0.439    1         oT

720 | 044 0447 1.075 0.795 107 0795 | OAT 0468 0469 049 114 0857 | 0454 06404 ~~» ETI
4 | 96 {0263 032 2602 1329 21 1004/0274 0337 0332 034 1549 0952 | 0271 4g | ~
=| 192 | 0321 0.36 3.198 1368 2548 1249 | 0341 0382 0407 0446 3.792 1542 | 0334 =      a 제”
| 336 | 035 0374 3.139 1353 3142 1.343 | 0.529 030 04 0447 4215 162 | 036] . a             J

720 | 0.394 0.424 3.164 1352 3.138 1343} 0379 0422 0412 0.469 3656 1.619 | 0419     러버   7
2| 96 | 0.128 0.219 0575 0535 0404 0434 | 0.129 0222 0.186 0.302 0304 039310139 0204    =
SZ} 192 | 014 0.239 1.061 0809 0844 0.717} 0.147 024 0.197 0311 0327 0417 | 0:87    yyy
B | 336 | 0.166 0.258 1.04 0.795 1.015 0.775 | 0.163 0259 0213 0328 0333 0422 | 0.161    ee acer ay 88 "에
=| 720 | 0201 0.29 1.048 0.804 1.041 0.783} 0.197 029 0.233 0.344 0351 0.427 | 0.196                 -
4 | 96 | 0543 0235 1.377 O717 1349 0715 | 036 0249 0576 0359 0733 041 | 0336 0써              ore
| 192 | 0567 0.246 1442 075 142 075 | 0319 0256 O61 038 077 0435/0346              i
E | 336 | 0.602 0.286 1489 0778 147 0.776 | 0.392 0264 0.608 0375 0776 0434 | 0355                 oa

720 | 0.671 0281 1526 0.793 1.524 079 | 0432 0.286 0.621 0375 0.827 0.466 | 0386 B a5}                은

[                fe

| 9 [O12 018 0278 0301 010 0231 | 0149 0.198 028 034 0354 0405 | 0.166 ||               "3
S| 192 | 0.186 0.227 0.376 0.369 0.299 0336 | 0.194 0241 0.275 0329 0419 0434 0209 °*7 |             | 8
| 336 | 0.237 0.269 0.568 0527 0376 0.374 | 0.245 0282 0339 0377 0583 0543 | 0254 agp]       ms loz e
* | 720 | O31 032 0571 0533 0.459 0.433 | 0314 0334 0389 0409 0916 07050313 gee 2 2 고
Couff | 에     0     o ] 3t     0     a ~     . Segment Length

   =        저때      제       en                   660 LEARNING”
ee 3 DEEP LEARNING

m SegRNN 개요, Long-term Time Series ForecastingS 위한 접근

® RNN2AY 문제 : 반복적인 회귀 횟수 증가로 LTSF 분야에서 성공하지 못함

© 해결책 : Segment-wise iteration 기법 + Parallel Multi-step Forecasting 전략
® Segment-wise iteration 기법

® point-wise iterationS segment-wise iterationl = 대체

@ 반복의 횟수(560. step) S L 에서 L/w 감소(\: segment length)

® L>nxw(Seg.) > nx d(linear projection) >GRU > h,,

® Parallel Multi-step Forecasting 전
@ 반복의 AS 4/에서 12 감소                                ane ae

ae are a             Decoding
® (Relativet+channel) encoding + repeat(h,,m)>GRU        108      = (ase
> mx d > mx wi(linear projection)                                 oy      세
Encoding                                                           ^
 GRU Cell
| | | Vector   xe 6 Rd   FE]   [ |    |                          [ 」
기 &       건                                누
|                       Linear(w, d) & ReLUQ)                       bei |
t       t       t                                  |
x eR \         aN   것               >      ~“  ol                                                       ad 6 Rw
I       t       1       t       t       t            |       |       |       |
=    :          xO eRe     ad agi ee            “~                    > YOerR!
298                                                                                    Na a Oa             .
@한국시연구소 홍근선        -149ㆍ 무단 전재, 복제, wall, 디지털화 금지


===== PAGE 151 =====
3.1 Time Series 개요

34. Time Series & LSTM

©) thumi/Time-Series-Library )@ official                     we 8.424           |
term Forecasting
{Average MSE)
Long-term Forecasting (*)                                              Anomaly Detection
(Average MSE)                                                           (Average Fi-Score}

Short-term Forecasting
(Average OWA)

LSTNet       a
\

mmo MIPbased | 개어 CNNbased     see RNNebased    {
가 GNNbosd = Transformerbosed ㅣ 7586 Implementation  |
| 00010 }-ㅡ~                   스미아이미라 —>,     NStronsformer —\        TIDE      \
|                                                      \ 60000       :       TimeMixer

OCRNN                                            {                           SCINet
91004          ASIGCN —4       “AGCRN
Graph WaveNet          StemGNN |      ih
299                                                              [tHoc

“Deep learning for time series forecasting: a survey”,2025

Energy                            Healthcare                 Transportation;              Meteorology                      E              i                              보라애대
\
Methodology1:     ‘                                                    Paradigm1:
Dimension Decomposition                                                                                                                                                            Encoder-Decoder Model
Datasets in
Primary Domains}
-                                                                                                 Paradigm2:
‘|                                                                                        Transformer Model
abeaoide      <4 Deep Time Series _              p    Lpens                                             Paradigm3:
Meth                     ~ | Forecasting (DTSF)                Paradigm                      ig           Integrated Model
Methodology3:                 6                                                                              i                                                                                               Paradigm4:
Pre-Training                                                                                                    a                                                                                      Generate Adversarial
Challenges and
Prospects
Paradigm5:
Methodology:                                                                                 |                                                                              Cascade Model
Patch-Based Segmentation                           ¥
+      +      y      +      +         ‘=     +       +              +
Lack of Data                                           Lack of                                           Challenges of                       Potential            Counterfactuat
Privacy                 Lasket              Temporal |p 다 | Parallel                     Representation | Forecast and ] | TS Diffusion                                         Se
Protection                                  Contionity Jf Lette Motels FT computing                    Learning} (Causal inference)                                                            sere

ry

= 150-    |

oO
ai

Al, 복제, S4l, 디지털화 금지



===== PAGE 152 =====
3부. Time Series & LSTM

Chapter 3. Time Series & Other Architectures

3.1 Time Series 개요

3.2 Time Series Analysis

3.3 TCN and Other Architectures

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.5 Time Series Classification

pte EEP LEARNING
RECIPE FOR YOU

0“
= 24 : Time Series 데이터를 다루는 기본적인 접근과 분석 기법 확인
ade 개요
® 시계열 데이터를 (6416\하는 기본적인 접근방법 학습
 데이터를 07616\하고, 기본적인 분석방법을 적용

= DataSet

7 |

[실습] Time Series Analysis https:         mn    0"

© 적용할 분석 방법
# ACF/PACF
@ ARIMA
®@ Auto-ARIMA
®@ Prophet                  :
® Augmented Dickey-Fuller(ADF) jy
@ LSTM

@ 4가지 수역의 특징 예측
@ Water springs
@ Lakes
@ Rivers
@ Aquifers(Ci-3)

Steves tock          _ Water (not ground water) heid by molecular attraction _          Gravel 4,

surrounds surfaces of rock particles

«== «+ Approximate level of the water table = «=. «=

All openings below water table
full of ground water

How ground water occurs in rocks.

©

fw
o
N

rt

ee eee eee ee

국시연구소 홍근선                     -151- 무단 전재, 복제, 발춰, 디지털화 금지


===== PAGE 153 =====
3부. Time Series & LSTM                                       3.2 Time Series Analysis

. 대수층, 2. 반대수층, 3. 비포화영역,
을 DataSet Download                                    1 시하수위 5. mgs 이 anise

® 1) kaggle install 하고 : pip install kaggle
2) kaggle API token 받아서 저장
kaggle home page > Account > API > "Create New API Token"
> down load "kaggle.json" > copy to "~/.kaggle/*

eo) 1 !tkaggle competitions download -c acea-water-prediction

® Unzip to ./datasets/acea-water/         niet Sater
922,401 Aquifer_Auser.csv

468,078 Aquifer_Doganella.csv
486,481 Aquifer_Luco.csv

261,818 Aquifer Petrignano.csyv
10,462 datasets_description.ods
41,039 datasets_description.xlsx
264,151 Lake_Bilancino.csv
372,405 River_Arno.csv

441,576 Water_Spring_Amiata.csv               oo    으으
1202,700 Water_Spring_Lupa.csv                  Agee

76,992 Water_Spring Madonna_di_Canneto.csv | Water_Spring Amiata —
3,448,095 바이트                                  a

Quiput (Feature to predict

1 df = pd.read_csv(path+"Aquifer_Petrignano.csv") a
2_df.describe()                                ee! a eee
Water Spring Lupa          Flow Raie Lupa    :
River_Arno         Hydrometry Nave di Rosano
| 303                  에메                            1            =

& Cleaning DataSet                                                  eager ee              :
 Check missing value                                         ia                                        |

— |

+, ax = plt.subplots(nrows=1, ncols=1, figsize=(16,4))      에

505 .heatmap(d¥.7 isna(), cmap="Blues‘)

ax.set_title(‘Fields with Missing Values’, fontsize=12)

#for tick in ax.xoxis.get_major_ticks():

# tick. Label. set_fentsize(14)

for tick in ax.yaxis.get_major_ticks():
tick.label.set_fontsize(1@)

plt.show()

Depth to Groundwater P25 -

Emperazure Bastia Umbra
Tenperature Pevignane
Volume C10 Fetrignane:                                               +02]

en 9 치가 나

Hydrometry Fasme_Chiascio Petrignane

oe

@ Remove rows, columns

# Remove old rows

df = df[df.Rainfall_Bastia_Umbra.notna()].reset_index(drop=True)

# Remove not usefull columns

df = df.drop(['Depth_to_Groundwater_P24', ‘Temperature _Petrignano'], axis=1)

@ Simplify column names
# Simplify column names

df.columns = [‘date’, ‘rainfall’, ‘depth_to_groundwater’, ‘temperature’, ‘drainage volume’, 'river_hydrometry‘]

i
z
3
4

targets = [‘depth_to_groundwater']
features = (feature for feature in df.columns if feature not_in targets]

@ Convert ‘date’ column type to datetime type

Uy Dr he ke

from datetime import datetime, date

호
=
그

df['date'] = pd.to_datetime(df['date'], format = ‘'%d/%m/%Y')

304                                     .       *        :                '
한국시연구소 홍근선                  - 152 - 무단 전재, 복제, Sal, Cl



===== PAGE 154 =====
3부. Time Series & LSTM

3.2 Time Series Analysis

# To compelte the data, as naive method, we will use fFFiLL
+, ax = plt.subplots(nrows=5, ncols=1, figsize=(12, 25))
for i, column in enumerate(df.drop('date’, axis=1).columns):
sns.lineplot(x=df['date'], y=df[column].fillna(method='ffill’),

ax=ax[i], color='dodgerblue')
“wal aut eiciat Feature: {}‘.format(column), fontsize=18)
axf{i].set_ylabel(ylabel=column, fontsize=1¢)
ax[i].set_xlim([date(2009, 1, 1), date(2e2@, 6, 3@)])

4

@ Rainfall(mm)      2

@ Temperature(°C)    :

@ Drainage Volume    5
/* 취수량(07^3)           :

® Hygrometry(m):     3
 강 수위

/* level from the ground floor

Feature: rainfall

a

®@ Depth to Groundwater(m): Target

Feature: temperature

raintait
월 «© & &€ ®

drainage_volume

depth_to_groundwater
를

we            게드            20            me              내
Feature: river hydrometry

Not

fiver hydrometry
cS

2010                    2012

더

= Data Preprocessing
© Time: 연대순, 등 간격 확인, 필요 시 resampling
@ Missing value
® ‘0’: “Drainage_Volume’”, “River_Hydrometry” 칼럼에 비 정상 ‘0’ Zt 존재

f ‘NaN’ o@ 대체 후, 다시 정리 필요                                                                          =<
Fill NaN with 0
@ NaN: 남아있는 NaN              |    ®                              |                                        = me
3 df.isna().sum() |          iia eatin baa ee                                Wf
depth_to_groundwater      27        & 20000 |                                       -
temperature                 0            2019.05            2013-06           2039.97            ieee                           218-10
sate
drainage _volume                   그                                                                 Fill NaN with Mean Value {-28841)
river_hydrometry           0       은 20000      -                              &
5 om  ~      ‘c yg A AN ~ Au. Cod 5  Ly pore eA part fet
® Missing value Handling(fill)   i   eel                                            ¥
“      ㆍ                                     2039.05            2019.96           2019.67            2019.88            2019.09           wis
1: Outlier or Zero                                                                                           ste
Frill
2: Mean Value |      |               jom    dP A  ahi JD   ey seiner
3: Last Value with .ffillQ              i      credited                                                 “.
은 -40060    .
4: Interpolated Value                    2019.05        - 20906            2019.97            2018.08            2019.09           “pid
068
with .interpolate()                    !        F
ㅣ oe ae  J ah Sale,             z
me  - A          nef a ee            oy 어나나내 너머
2019.05      ITE. 2019.07.            2019.08            2019.09           5-10
i df[’drainage volume'] = df[ ‘drainage volume’ \interpolate( )  년     5           34
2 df{‘river hydrometry'] = df[‘river_hydrometry']. eae          Now        U
3 df[‘           _Broundwal   re  "led
Sa               재개                                                      이 BEER LEARNING

@한국시연구소 홍근선

- 153 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 155 =====
3부. Time Series & LSTM                                       3.2 Time Series Analysis

® Resampling(Up, Down sampling)

fig, ax = plt.subplots(ncols=2, nrows=3, sharex=True, figsize=(16,12))

sns.lineplot(df[‘date'], df[‘drainage_volume'], color="dodgerblue’, ax=ax[@, @])
ax[@, O].set_title(‘Drainage Volume’, fontsize=14)

be Nhe

내

ea)

resampled_df = df[[‘date', ‘drainage _volume’]].resample(" 7D’, on=idate').sum().reset_index(drop=False)
sns. lineplot(resampled_df['date'], resampled_df[ ‘drainage _volume'], color="dodgerblue’, ax=ax[i, @])
ax[1, @].set_title('Weekly Drainage Volume’, fontsize=14)

8 9 4

16 resampled_df = df[[‘date', ‘drainage volume’]].resample('M', on=‘date’).sum() reset index(drop=False)

11 sns.lineplot(resampled_df[‘date’], resampled_df[‘drainage_volume'], color=‘dodgerblue', ax=ax[2, 6])
12   2, @j].set_tit  “Month    i   vi     ize=i4
2 ax[{2, @].set_title('Monthly Drainage Volume’, fontsize=14)                       Pies aLevife

Drainage Valume

「
bale

13                                                                                                      -1$000

44 for i in range(3):                         20000
15    axf{i, @].set_xlim([date(20e9, 1, 1),     -25000 홀리
16                 0216(2020, 6, 36)])    건
ㅋ -3ㅋ5006
® Down sample 적용 Cae AoA )            -40000
2 downsample = df[['date’,                              -2400000                     y_Orainage
3                                  ‘depth to groundwater’,                       <sbieon
4                           ‘temperature’,                               “180000                                 Anny
5                 ‘drainage volume‘,              을 ae
€                            ‘river_hydrometry',                     | =                   Ma
7                  ‘raintfall*                         “260000
8             ]].resample¢'7o'),              이
9              on='date’).mean().r        index(drop=False)                                 Monthiy Orainage volume                  =
16 df = downsample.co                                 =e                             vw,          Aan
npr             Gos     av     A  A pay             u     시
|”    )     |  AM
307                        ‘        "                                주      as      saa      aie      aia       2056

t

Non-Stetionary sees                             Nu Stationary 하기                             Noe Stationary series

correlation
coefficient                            An illustration of the principles of stationarity, Source: BeingDatum

© Stationary Check
®@ 시각화 : trend, seasonality 확인
 통계적: mean, variance 확인
@ 방법론 : ADF (Augmented Dicke   ler) test

ature: Non-stationary
variance is time-dependent (seasonality)
—— rolling mean                                                  i                                                           Mean, Variance :
|       a i               - not constant
1:        1                  ( but close constant )

@한국시연구소 홍근선         -154- 무단 전재, 복제, wl, False


===== PAGE 156 =====
3부. Time Series & LSTM                                       3.2 Time Series Analysis

Tim

® ADF (Augmented Dickey Fuller) test            Katia      check  ,
ull Hypothesis (귀무가설), HO : datat not stationary 하다.
® Alternative Hypothesis (대안가설), H1 : datat stationary 하다.

>HO7} reject=|H, data stationary
@ HO Reject ZH

/ p-value < 0.05(default value p-value 조건으로 하는 것에 여러 가지 문제점이 있지만…
/* ADF statistics < critical value: 1%, 5%, 10% 값을 확인 S(sample 숫자 확인 필요)

4 result = adfuller(df{'depth_to_groundwater’ ].values)
5 result

© B27} 모순될 때는 어떻게 해석해야 하는가?

"; -2.8664345376276454,}

{40% : _.2.569376663737217}1,
ADE Statistic 3.374, p-value 0.012,                                     ADE Statistic, $,922..2721Ng,9 000,
ae                                                           critical Valbdd tee $485 See “2867, 165: -2.569                     Critical Values 1%: :3.441. 5%: -2.866, 10%: -2.569

Sample size 1%   5%                                    2” h "|    Hy 6 기  f Hi    ;
T=25 375 | -300 | -438 -360                     을 4 iA) ¢     1
T=50 | -358 | -293 | -415 | -3.50                       ~ ge ee?
T=100  -351 . -289 | -404 -245    cnt he 구671062569 00,   critical 바오 기아 066 2.569
7=250 -346  -288 | -399 -343 ,             i;  _ig@       IA

6     2010   2022   204   2016   2018   2020  i     206   Riz -  2034   2086   206   2020

ㅎ ‘Depth to groundwater® Ｌ00적용
# Log Transform of absclute values

# (Log transoform of pegative values, will return NoN)
df[’depth_to_groundwater_log’] = np.log(abs(df[‘depth_to_groundwater’]))

+, ax = plt.subplots(nrows=1, ncols=2, figsize=(2@, 3))
visualize_adfuller_results(df['depth_to_groundwater_log'], ‘Transformed \n Depth to Groundwater’, ax[@])

critical Haas Re SAR Oe SES TO: 2.569

UT Re Wee et

3
&

wow

aoe

1
te
&
“
wo

we
N

fo!
8
ww
ss
,
«

Depth_to_Groundwater
¥
Transformed
Depth to Groundwater

2010         20312         2014         2016         2038         2020                           2030         wiz         2034         2036         2038         2026

® ‘Depth to groundwaterO| Diff. 적용
1 # First Order Differencing
ts_diff = np.diff(df['depth_to_groundwater’])
df[‘depth_to_groundwater diff 1'] = np.append([@], ts_diff)
첫 diff=0

+, ax = plt.subplots(nrows=1, ncols=1, figsize=(3, 3))
visualize_adfuller_results(df['depth_to_groundwater_diff_1'],

‘Differenced (1. Order) \n Depth to Groundwater’, ax) ‘    ee   a

Statistic ~   . 0.000
Critical Sees Pe a ee -2.569

wt bo BM

& ㅎㅎ
에 오어

Differenced (1. Order)
Depth to Groundwater
ㅎㅎ oe
eos &
=

aaa

ee,

4 85

:          ;      :                                     .       cx     om
en  RNIN A lk

@한국시연구소 S24                - 155 - 무단 전재, 복제, Sa, 디지털화 금지



===== PAGE 157 =====
3부. Time Series & LSTM

3.2 Time Series Analysis

= Feature engineering
*         내                                               ~4  개
* Encoding Cyclical Features           .        op] ee aN
@ Cyclical features can confuse the model                       —
3 sns.lineplot(x=df[‘date'], y=df[‘month’])                 ay

4 sns.lineplot(x=df[’*date'], y=df[‘quarter'‘])

5S sns.lineplot(x=df[‘date'], y=df['season'])                  3802
205

18

month

a

in
ae

시
8

2010         2032         2014        2036        2018        2020
® Encoding to polar coordinates

i month_in_year = 12
2 df[‘month_sin'] = np.sin(2*np.pi*df[ ‘month‘]/month_in_year)
3 df[*month_cos'] = np.cos(2*np.pi*df['month’]/month in year)
&
5 f, ax = plt.subplots(nrows=1, ncols=1, figsize=(3, 3))           10       에
6 sns.scatterplot(x=df.month_sin, y=df.month_cos, color='dodgerblue')       se      a
7? pit.show()                                                051 ＊            *
3
Yarz Cycle | ANE              cy              :
~0.5  *            *

19110

@ Decomposition ( 시계열 분해 ) : 4가지 2A(Level, Trend, Seasonality, Noise)= 분해
VO eee
@ Level: 전체 평균 , Trend: 상승, 하강

ㅎ Seasonality: 반복적인 짧은 사이클 , Noise: random 값
# As 0000010109 : Additive(229| 합으로 구성), 4411011681006(곱으로 구성)
@ API: statsmodels.tsa.seasonal.seasonal_decompose( )

3 core_columns = ["rainfall’, ‘temperature’, ‘drainage volume’,
4             "river cid , ‘depth to_ groundwater’ ]

5 for column i

6     decomp   재고 오오 이에 period=52, model=‘additive', extrapolate_ trend=' Enea. )

7      df[f"{colum

8    df[f"{column}_ “seasonal” ] =       seasone

]     df[f"{column} residual”] =   0. resid # Noise comp.
ARAR of 소기

Decomposition of 006 _to_groundwater

30                                -20             ^
Bn  nA     AAS ay         WV Af A\y ;    ae     als   ial     ON PL rl
ELAMAWW       이 ~
3 '                               Fs    /        J
eG qe
mans LU Pry“,        nn ae                 Sn
뜨는    fo hen  i 7        =     ae  /       seep
“4    wt                          -30
me 2
3
&
=r
5 °
cs

무단 전재, 복제, Si), 디지털화 금지



===== PAGE 158 =====
3부. Time Series & LSTM                                      3.2 Time Series Analysis

= Exploratory data analysis : 다양한 시도를 통한 정보 획득
® 2 feature2| seasonal 요소에서 특징을 찾아 보자
@ 년 단위 사이클이 확실하게 보임
@ 요소 별로 고점과 저점의 시간차가 보임

Seasonal Components of Features
2

마레
2

ww \  vA awl A hay VAN 01 vain

217-10 2016.01 2018.04 2018-07  2018-10 mabe 3 2019-04 쁜 2019.10 2020.01 2020.04

"           ea                  ^
~ 0                                            0 ae

2027-10 2018-01 2018-04 2038.07  218-10 2039.01  Tesi  2019-07  2019710 2020.01 2020.04

temperature
©

g

|       5 아이             ow          ait
1 0

        ~                                                               Vw”

£ ~2000

217-10 2016.01 2018.04  2016-07 = WG-10 2019.01 2019.04 2015.07 2019.10 2020-01 2020.04

을                                             i
 7 fers ~ aL ^

20317-10 2018.01 2018.04 2018.07 2018.10 ee aso WIS-OT 2019.10 2020-01 2020-04

PN FN

“1
2017-10 2018.01 2018-04 2018.07 218-10 2019-01 ore 2019-07 iy 2020.01 2020-04

[그

i  to_groundwater        &

313                     =                    !         ;                    144                 :           7          Sof DEEP LEARNING™

® 2 feature2| seasonal 요소에 대한 Lag(time shift)2| 영향을 찾아 보자
@ 4주를 기본 단위로 -2, -1, 1, 2, 3 씩 이동하고,
@ 기본 16314[6의 selation 결과와 shift$t seasonal component9 correlationAz}S 비교

i weeks_in_month =

2 for column in core_columns:

3      df[¥*{column}_seasonal_shift b 2m'] = df[¥'{column}_seasonal'],s

4      df[F* {column}_seasonal_shift 6 im! ] = df[#'{column}_seasonal'].   AC. 4° weeks _in_month)
들      df[f'{column}_seasonal_shift_im‘] = df[F'{column}_seasonal'].shift(i * weeks_in_month)
6      df[f' {column} _seasonal_shift_2m'] = df[#'{column}_seasonal'].shift(2 * weeks_in_month)
7      df[f'{column}_seasonal_shift_3m'] = df[f' {column} _seasonal'].shift(3 * weeks _in_month)
3 corrmat = df[core_columns].corr()

4 sns.heatmap(corrmat, annot=True, vmin=-1, vmax=1, cmap="coolwarm_r', ax=ax[@])

5 __ax[@].set_title('Correlation Matrix of Core Features’, fontsize=16)

8 shifted_cols = ['depth .to_groundwater_seasonal',

9                   “temperature_seasonal :

18                  “00010980 volume _.

a                   ‘river _hydrometry.. seasonal. shift, - 3m" ]

12 corrmat = df[{shifted_cols].corr()
13 sns.heatmap({corrmat, annot=True, vmin=-1, vmax=1, cmap=‘coolwarm_r', ax=ax[i])
14 ax[i].set_title('Correlation Matrix of Lagged Features’, fontsize=i6)

Correlation Matrix of Core Features                                              Correlation Matrix of Lagged Features

100
ozs           temperature sessons!_stuR b 2m

025 qrainage_votume_seasenel_shit_2m

O58
“27S sver_hydrometry seasenat_shitt_3et

- 157- 무단 전재, 복제, 24), 디지털화 금지



===== PAGE 159 =====
3부. Time Series & LSTM

3.2 Time Series Analysis

8 Autocorrelation Analysis (자기상관분석) : 자기상관 함수, 편자기상관 함수

: 앞에서 DifferencingSt dataO|A] ARIMA 적용하고 싶어, 이때 AR, MAS 필요성 확인
@ ACF (AutoCorrelation function): P(=lag), 이전 정보의 조합으로 표현된, 상관도

S tists S     a
@ Data2| seasonality 확인, 필요한 항의 수를 개략적으로 식별 ye '\:3 yaphr    Aska = 잔으헤0\  2p}

@ PACF (Partial AutoCorrelation): D(=differencing order), 차분결과의 조합에서 상관도
@ Differencing ㅁ0813의 stationarity 확인, 필요한 항의 +S 개략적으로 식별

@ 『830085와 statsmodels API 사용                  os

56
3 from pandas,plotting import autocorrelation_plot           ors}
2 autocorrelation_plot(df['depth_to_groundwater_diff_1'])  | sae

O25
1 from statsmodels.graphics.tsaplots import plot_acf         basa
2 from statsmodels.graphics.tsaplots import plot_pacf       a
3 f, ax = plt.subplots(nrows=2, ncols=1, figsize=(10, 8))          as Sel CL
4 plot_acf(df['depth_to_groundwater_diff_1'], lags=100, ax=ax[@])
5 plot_pacf(df['depth_to_groundwater daft : EY ]; lags= 100,  ax=ax[1])

Autocorrelation                                                                         Partial Autocorrelation
16

"  |              40000 --으르르 ytrk)          PAC F(k) = Corr(e;, &-«)
si                      _var(y:) | °°         = Ye — (AY bo + Yay)

a            Errorgio] 상관도

a2

00

ould

@ Cross Validation:
Test dataOl] overffiting 방지하고,
SE dataol 대한 성능을 추정하기 위해 사용
® K-fold Cross Validation

@ DataS 개로 분할하고,

/* 하나는 43110310ㅁ0 data=,
/* 나머지는 10109 data= 사용 ㆍ

@ KH 반복 학습결과를 평균

> data 56[이 적을 때,

성능의 변동성을 낮춰줌

2 from sklearn.model_selection import TimeSeriesSplit
2 N_SPLITS = 3

3    = df[‘date']

4 y = df[‘depth_to_groundwater']

5 folds = TimeSeriesSplit(n_splits=N_SPLITS)

&

for i, (train_index, valid_index) in enumerate(folds.split(X)):

Rolling Window with Adjusting Training Size (Spit 1)           Rolling Window with Constent Training Size (Spiit 1)
-20            ^      해부       ~            xe      -… trai
as     ats     i            —~ validation      ae     af *     }            oom valication
* 시계열에서 고려 사항           BY ON /                 tal \/
"                                      0             났
® Constant size vs.                  j     2010 2012 02014 2016 2018 2020     2010 2012 0204 2016 2018 2020
—    :                                           cote                                    cate
6 Adjusting size                    Rating Widow wih Adjusting Taming Size (Spt 2)        Rolling Windaw with Constant Training Size (Split 2)
-20                fr"                    0! 6        (스지 wt
~25    ad’    {"      ~~"            <2 | validation /~     wh,
q     fs}                         ~ 606         그            Me yf
lea           /            —~ yaiwsstion | 2%?           나
총     2016 2012 «MI 2016 2018 2020         2010 2012 00204 2016 2018 2020
dete                                     date
Railing Window with Adjusting Taining Size (Spit 3) 는. , Roling Window with Constant Training Size (Spit 3)
~20                              i      ~~ fain        wae
“22.5 | = validation            기
내    /                              Laws                    aa  iN   A
=                              a                                  8,                            WML
316                                                   2010              2016 2018 . 2020 FS      2010 2012 2014 2016 _ 2086 2020
S       소 홍근소            =    >        1, 복제, Sal, 디지털화 금지
@한국시연구소 홍근선          158- 무단 전재, 복제, Ball, 디지털화 a2



===== PAGE 160 =====
3부. Time Series & LSTM

test_size

WOON OW bh WN 가

train_size = int(@.85 * len(df)) # 85%, 520

univariate df = df[{['date', ‘“depth_to_groundwater']].gepy(),
univariate_df.columns = ['ds', ‘y']

# train(date,depth_to_groundwater)

cain = univariate_df.iloc(z:train size, :] #(51@,2)

# x(date), y{depth_to_groundwater)

x trains wutrain = (pd.DataFrame(univariate_df.iloc[:train_size, @]),

1@ x_valid, y_valid = (pd.DataFrame(univariate_df.iloc[train_size:, @]),

= Univariate Time Series Forecasting

= len(df) - train_size # 25%, 90

pd.DataFrame(univariate_df.iloc[{:train_size, 1])

pd.DataFrame(univariate_df.iloc({train_size:, 1]))

3.2 Time Series Analysis

NM etn              러                                             MAE: 100, RMSE 222.
m(Prophet Model    thodel,   =

from prophet import Prophet    |
a
&

4
5 # Train the model
6

model. fit(train)

8 # (666,1)<-(96@,1)              2009     wi     213     2015     2017     2039     202)

9 x valid = model.make_future_dataframe(periods=test_size, freq='w')

10                                                                             .

ii # Predict on valid set

32 y_pred = model.predict(x valid)

& model.plot(y pred, ax=ax)

7 sns.lineplot(x=x_valid[‘ds'], y=y_valid['y'],
8          ax=ax, color='orange', label='Ground truth')}"           ‘Sif DEEP LEARNING |
317        ee                     aa      ass                  BBR BB 7080 VO A.

¢

= ARIMA Model : Auto-Regressive Integrated Moving Average (ARIMA)

ARIMA(p, d, 0)

® p: Trend autoregression order
# 0: Trend difference order

# 0: Trend moving average order

y_pred, se, conf = model _fit.forecast(90)

1 from statsmodels.tsa.arima_model import ARIMA
# Fit model

model = ARIMA(y train, order=(1,1,1))

model _fit = model.fjt()

# Prediction with ARIMA

Aw bw wh

6 sns.lineplot(x=x_valid.index, y=y_valid['y'],

7                ax=ax, color="orange’, label='Ground truth‘)
Prediction
18                          MAR 2 CA AMSK. 2 89,
“20                                                            Grounel truth                      ied
Fy 22                                                                  3 -250                                      f
-24                                                    5
Be     [NK]         \                                                은 260
를   [                                                을
12                 ‘                  en      9 2265
~-34                                                     0 55% confidence interval
oe     200    208    400    500    600        520    E     566 880    00
a        “            oe             배서        “      Xk DEEP LEARNING
@한국시연구소 홍근선                     - 159 - 무단 전재, 복제, 4], 디지털화 금지


===== PAGE 161 =====
3부. Time Series & LSTM                                        3.2 Time Series Analysis

        :            —       ws     - | AIC: Akaike information criterion
= Auto-ARIMA Model  2 dod  AB, 93| Mee nates the quality of each model, relative to each of the other models,

© Parameter search to min. AIC          AIC = 2k —2In(L)

2 import pmdarima as pm           Let k be the number of estimated parameters in the model.

3 model = pm.auto_arima(              Let L be the maximum value of the likelihood function for the model.

4              y_train, start p=6, start_q=@,

5           test=‘adf',      # ADFtest to find ‘d’

6            max_p=5, max_q=5, # maximum p and q

고             m=1,             # frequency of series

8           d=None,         # determine 'd’

3             seasonal=False, # No Seasonality

310                       start_P=@,                                                       SARIMAX Results

11               D=6,

12                 trace=True,                   Dep. Variable:                y No. Observations:             518
33                error_action='ignore',     Model:          SARIMAX(4, 1, 1) Log Likelihood           327.517
14                  suppress _warnings=True,     Date:            Sun, 05 Sep 2021 AIC                    643.034
15               EERE) ee              15:32:07 BIC                ~617.648
16 print(model.summary())                 Sample:                 80 10                -633.077
Performing stepwise search to minimize aic

ARIMA(@,1,0)(6,0,6)[8] intercept :; AIC=-242.692, Time=0.04 sec

ARIMA(1,1,2)(@,8,8)[@] intercept  : AIC=-574.047, Time=0.08 sec

ARTMA(@.1.1)(@.6.@\)f@1 interrent   + ATC=-477.347. Time=A@.A7 sec

ARIMA(5,1,0)(@,8,8)[@]          : AIC=-636.112, Time=@.16 sec

ARIMA(S,1,2)(@,0,8)([@]          : AIC=-639.713, Time=@.42 sec

est model: ARIMA(4,1,1)(@,@,6)[@]
Total fit time: 5.956 seconds

es

jail hi

m Auto-SARIMA Model : SARIMA(p, 0, q)(P, D, Q)m
@ P: Seasonal autoregressive order
@ D: Seasonal difference order
®@ Q: Seasonal moving average order
# m: The number of a single seasonal period
4 model = pm.auto_arima(
5        y_train, start_p=1, start_q=1,
6         test=‘adf', ~    # ADFtest to find 'd’
고          max_p=5, max_q=5, # maximum p and 0
8          m=12,           ## frequency of series
cE)         d=None,         # determine ‘d’      1
10             seasonal=True,     ## Seasonality          i
2        Del.          ##             별:
13                   trace=True,                                                 건
14                     error_action='ignore',
15           suppress _warnings=True,                         Prediction
16           stepwise=True)            “18                 SSA RTE TERE LER,          a
1 # Fit model                    . -                dN
2 model_fit = model.fit(y_train)    ie          st      os       we.    ^
3 # Prediction with ARIMA         2 2      ri    |             Lf  wyhy 1
4 y_pred = model_fit.predict(98)    ei f\y      Kf               ^
>   i  에         홈
-32   '            VU
320                                   삐      6      00   200     300     400    _ 500     00

한국시연구소 홍근선                    - 160 - 무단 전재, 복제, Si, 디지털화 금지


===== PAGE 162 =====
3.2 Time Series Analysis

34. Time Series & LSTM

= LSTM Model

© Pre-Processing

© Normalize

@ Normalize the features. (-1 ~ 0)
® Split & Create sequence : X=datali:i+52], Y=data[i+52+1]
® Reshape (samples, timesteps, features).

Os UY Bel Ba pet

《

from sklearn.preprocessing import MinMaxScaler

data = univariate_df.filter([‘y'])
dataset = data.values # np <- pd

© Split & Create Sequence

look_back = 52

Wook Ww bo

# Split inte train and test sets
train = scaled_data[:train_size-look_back,:]
test = scaled_data[train_size-look_back:,:]

? def create _dataset(dataset, look_back=1):
8   % Y=) []
을      for i in range(look_back, len(dataset)):
16          a = dataset[i-look_back:i, 0]
ii          X.append(a)
12          Y.append(dataset[i, 0])
213      return np.array(X), np.array(yY)

© Create Sequence & Reshape

18 # x_train: (486,52,1)

15 x train, y_train = create dataset(train, look_back)#/(4@6,52), (406, )

26 x_test, y_test = create_dataset(test, look_back)  #(96,52),(98,)

19 x_train = np.reshape(x_train, (x_train.shape[@], x_train.shape[i], 1))
29 x_test = np.reshape(x_test, (x_test.shape[@], x_test.shape[1], 1))

© Define Model

#Build the LSTM model
model = Sequential()

wi 46

Oo Oo 14 0

model .add(Dense(25))
16 model.add(Dense(i))

model.add(Input(shape=(x_train.shape[1], x_train.shape[2])))
model.add(LSTM(128, return_sequences=True))
model.add(LSTM(64, return_sequences=False))

Layer (type)               Output Shape            Param #
istm_2 (LSTM)           (None, 52, 128)        66568
istm_3 (LSTM)                (None, 64)                49498
dense_2 (Dense)          (Nene, 25)           1625
dense_3 (Dense)               (None, 1)                  26

Trainable params: 117,619
Non-trainable params: @

322                                                                          o f DEEP LEARNING ‘
@한국시연구소 S24               - 161 - Sot 전재, 복제, 2, 디지털화 금지


===== PAGE 163 =====
3부. Time Series & LSTM                                       3.2 Time Series Analysis

,

¢ Training
1 model. compile(optimizer='adam', loss='mean_squared_error')

bid

3 model.fit(x_train, y_train, batch_size=1, epochs=5, validation_data=(x_test, y_test))
® Prediction

# Prediction

train_predict = model.predict(x_train)

test_predict = model.predict(x_test)

a
그
2
6
5 # tavert with scaler

6 train_predict = scaler.inverse transform(train_predict)
es

a

=

8

y_train = scaler.inverse_transform([y_train])

test_predict = scaler.inverse_transform(test_predict)
y_test = scaler.inverse_transform([y_test])

Prediction
MAE O16, BMSEL OA)

no            \        = 을      -245
B ~22                              f   "\                 ~ Ground inth |S _
3                    .            nS         \                             을 250
g -24              a         /             WAS | fl              3
3                  _        |                       \ i          ^ | 5 255
B ~-26            a ns                             Kd                8
3-4    Ph]       \    |                   é             2
3        [N            4 |                                             8260
Ey -30      ii                           i   ;                                                                  =
° x                    \ ;                                      호 -265

"                          |                                              옹

NJ
~34

2039                     2032                     2014                     2036                     2018                     2020

ultivariate Prophet _  a a  100
4 구제 model     ^ 내   \
4 model = Prophet()                                    때 es
5 model.add regressor('r                 “8                    :              ~ Grou uth
을 model.add_regressor( Aemperature')      을
7 model.add_regressor({'drainage_volume’  를 고
8 model.add_regressor\ 'river_hydrometry') oe
9                                   a”
10 # Fit the model with train 508         i
21 model.fit(train                      we
12                                    3
13 # Predict en valid set                   2008     Eas     213     205     ma     209     202:
14 y_pred = model.predict(x_valid)
Prediction
MAE: 0.82, RMSE: 0.98
a                                                 owes ‘Ground truth
8 -26                :             :
:           AE
2 -28                             4
을                     는 그
를 -
a) 4G               : f
-32                   3 i
¥
-34                     ;         .                  :
2009       211       2033       2035       207       2019       2021
     이                            es         :      .   =sepapepeb animes sores  EE eee EEE

한국시연구소 홍근선                 - 162 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 164 =====
3부. Time Series & LSTM                                      3.2 Time Series Analysis
Fa                                         7|

Time Series Anal

2

@ Analysis
® Prophet Model :     MAE: 1.0 , RMSE: 1.23
@ ARIMA Model :     MAE: 0.74 , RMSE: 0.89      리엄 feveeart
@ SARIMA Model:     MAE: 0.78, RMSE: 0.88      !
@ LSTM Model :     - MAE: 0.16, RMSE: 0.21 -)    | Rolling Forecast          ,
® Multivariate Prophet: MAE: 0.84, RMSE: 1.02      8              ,     Lf
$ LSTMS| 성능이 뛰어난 특별한 이유는?                :                   NO
Aen we          으네

@ LSTM: Rolling forecasting 4%, >fe3to      ;         0
@ 다른 2G! iterated forecasting vie pez UA AE, 6          :     Forecast Origin 1

® Forecast(A|ZtO| 포함된 prediction) methods 분류                              nate nce" pa
irect forecast (point forecast)                                             .                                       오리 오비

/@ One step ahead forecas                            3)            2                     @ New Observation
+ N-step ahead forecast        Pho yay AE Wert a    6    8    10    12

@ /tterated(recursive) forecas            — oe
A 2B?  5 Unt| a ASovservations
@ Probabilistic forecast    |  qh     |   Le ‘Density Forecast        4

a EnsemdPensity 10「6085【(불확실성 정량화
/* le 107600851(강건한 예측)

- 평균, 가중평균, SH.                        we

@ Rolli                                                   inci

nt

% 실습과제 : 1511\4모델에도 Iterated forecasts ALS 보자
PVA 지애매
= Regression methods
® Simple regression: 단일 독립변수(3), 단일 종속변수(>)
® Multiple regression: 다수의 독립변수(×,), 종종 상위개념인 Multivariate 라 지칭함

© Univariate regression: 단일 종속변수(>
® Multivariate regression: 다수 종속변수(3,)

 어떤 방법이 가장 좋을지 생각해 보자                     11004 {00028 3
© AS 결과를 비교하고, 성능 개선을 위해 어떤 것이 더 중요한지 생각해 보자  i's  ifr 점
= Analysis
© Prophet Model :       MAE: 1.0 , RMSE: 1.23
© ARIMA Model :         MAE: 0.74 , RMSE: 0.89
® SARIMA Model:        MAE: 0.78, RMSE: 0.88
ㅎ LSTM Model :          MAE: 0.16, RMSE: 0.21

© Multivariate Prophet: MAE: 0.84, RMSE: 1.02
® Iterated Forecast
@ Simple LSTM:                           RMSE: 0.86
® Multivariate LSTM Model :            RMSE: 0.67

-163- 무단 전재, 복제, Ball, 디지털화 금지


===== PAGE 165 =====
(2 suit Vowale Pogreasiom Models

@) <rople Ye greg iou
342. Time Series & LSTM

Rrra Ars >

wld? Amzwr 40% Sap 1

3.2 Time Series Analysis

= LSTM-based Iterated Forecast
© Simple Regression Iterated Forecast
RMSE                                                                       Simple, terated : RMSE
istep: 0.127, iterated: 0.859                                        istep: 0.127, iterated: 0.859
’                                                                    --~ iterated Forcaset                   eee
ae                                                             ~~- Istep Forecast            Bs   ;
S -22                                                        ~25.07 Ground truth            7    :
혈                                                                                       a.         | 고
3  24 4                                                                         ahs    %        eu            고
2                                                                               ~ | 10       , PR
§ ~°                                                                           ‘\ f 4
8
os                                                                             ~26.0                    ai 헤어
=  28                                Train Set               xX Z      Xie   i  a re
a -30                                                         ~~~ Estep Forecast           bbe       wg       x   000;
& ~32 +                       1        이거 Iterated Forcaset |     °       cee lt      te
~~ Ground truth                                             wy
344     seat      Se eee       |        :                    :
2010     2012      2014      2016     2018     2020            S      28      8      8      =
® Multivariate Regression Iterated Forecast
Multivariate, tterated : RMSE
depth | re                                                step: 0.348, iterated: 0.675
~24.5                            ss
~20  |                     watt
들                                                                                    “~     “a,                wry
2 -22                                                                                  6                            13     주
: -24 4               FX         pe          ie                                         a        or
“         4    f
| 때         AL          |                         Age.    -25.5   1     고각  rae 7       ‘
g -284      : /            j                                    =    내    1     ed    ;
& -30   |               |  )                    ——~ Train Set                  ?        ~
용 ~32                    \                       ~~~ tterated Forecast | -26.54~~- iterated Forecast   aaa      |
wa                     닙                      이 Ground truth           =» Ground trath       a        ㅣ
2010       2012       2014       2016       2018       2020           이      20      “0      60      80

m= Long-term Time Series Forecasting

: Multi-step forecastingSOlM] 예측구간이 긴 ASS 지칭 .
© Multi-step forecasting 접근 방법
/* Rolling F.    st:
@ [Direct Forecast

Cobia >              ,
rer Ym, 717 0

Oy 9, / 90므

N-step ahead forecast (One step ahea         ast= 아님                                    £%
x                                 *             정   이             o

/* 오차 누적이 없다는 점에서 [63160 Forecasting @#C} 안정적인 경향이 있음

 한 번에 전체 시점을

&

예측하도록 학습하는 방식

Look-back |                          마흔 이
Window |               Forecast Horizon =. =
L
|
{
:
i
:
:
i
01632 64     128            256                           532
a) Long-term Time Series Forecasting (LTSF)
Serer oe eer

/ 각 미래 시점(나 1, t+2, ..., tHH)ON 대해 개별적인 모델을 사용 또논 _

Categories |       RNNs
    SegRNN _DeepAR
Models | (ours)   (2020)
Metric | MSE MAE MSE MAE
~ 96 | O44 0376 1128 031
E192 | 0388 0.402 1077 0.776
E336 | 0401 0417 1.043 0.766
720 | 4434 0447 1.075 0.795
mm 96 | 0263 032 2602 1.329
은 192 | 0321 0.36 3.198 1.368
| 336 | 0325 0324 3.139 1.353
720 | 0394 0.424 3.134 1.352

| ‘Soe DEEP TL J

단 전재,

[베니

=
iS) ag 8

@한국시연구소 aca                    - 164 -

복제, S4ll, 디지털화 금지



===== PAGE 166 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

Chapter 3. Time Series & Other Architectures

3.2 Time Series Analysis

3.3 TCN and Other Architectures

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.5 Time Series Classification

DEEP LEARNIN

Ciek FOR YOU

 Temporal Convolutional Network(TCN): Conv.Net 을 사용한 시계열 처리
® 1D Convolution : = 함수의 #4 fxg
 한 함수를 반전+전이(9 11{{)하며 ( time 56065에서는 시간의 함수를 반전 )
@ 두 값을 곱하고

@ 그 결과를 적분한 값                    Convolution         Cross-correlation Autocorrelation
Cross-correlationz} 유사                  f       7

D> ASHA(vector)2| 유사성

> 특정신호 통과 : Filter                   9      NK

¥TCON                                 89 NN.

해 Sues oho 결품

.                    TA.
마츠    저의 £2    ont) inca
srk ~Ayy £      .



===== PAGE 167 =====
3부. Time Series & LSTM

3.3 Time Series Generation : WaveNet

을 TCN: Temporal Convolutional Network

® Dilated convolution : CNNS Time series] 적용
/* hidden layer 1 의 S42
A = a(S WNL ae )
A: activation func. d;: dilation rate
/* 2| Output € encoding#! 값 2, = hi 로 표현 가능
®@ receptive fieldS 지수적으로 확장
* 장기 의존성을 효율적으로 포착 가능

@ RNNG} 달리 병렬처리 가능, 빠른 학습 속도

ㅎ TCN 단점

 구조적인 민감성 : dilation rate, stacking SZ
® TCN vs. WaveNet

® Dilated causal convolutionS 중심으로 장기 시계열처리에 사용되는 PAS 일반화 하여 지칭
@ Causal convolution : 출력이 미래 정보를 참조하지 못하는 구조(즉, 과거와 현재의 정보만 사용)

Dilate
Outputs

Convolutional
Layer
Convolutional

Layer

Inputs

@ 추론 속도 느림: autoregressive POM SHO] 다음 입력이 됨)로 추론 단계에서는|병렬 처리 BE
@ 고정된 receptive field: 시계열의 주기성이 복잡하거나 길 경우 한계가 있음

® TCNE WaveNetS 일반화, 단순화한 구조 > 안정성, 추론 속도 향상

® Dilated causal convolution model       0 0 0

®@ Stacked Causal convolution            666

& 필요한 장시간의 정보 수집이 어려움
(layer7t 깊어짐, 연산이 많아짐 )

<
<

stacked causal conv. net
888 8 & 8 0

OPO OD Po eS

>

@ Stacked Dilated(Atrous) convolution   6069068 08 6 0 5 9
@e¢¢e¢¢e¢6¢666666
*붉은 위치의 값과         [ 3x3 ,1rate Atrous conv ]   [ 2rate Atrous conv ]
나머지는 0으로

6001\.연산 수행

*Receptive 11810의 크기가

3x3, 7x7, 15x157} 됨

*연산 BS 3x3 Conve} 동일

> Conv 연산 한번에 넓게 보기

Stacked dilated causal conv. net

무단 전재, 복제, S4ll, 디지털화 금지



===== PAGE 168 =====
3부. Time Series & LSTM                      3.3 Time Series Generation : WaveNet
3.3 WaveNet,                                                                                 |

2 WaveNet : 2016.9 “WaveNet : A Generative Model for Raw Audio”

DeepMind
= Over view : 1-dim Convolution based time series generation
¢ Audio wave generate : Long term dependency 문제가 핵심
® Dilated causal convolution model 제안
® 확률기반의 Auto Regressive model
* 1,600}2의 고해상도 신호 생성 : 고주파와 저주파가 섞이고, 변화가 심한
00 4@00060006000000000

Hidden -. 2, 2

90900900600000000000
1 Second         mt @@OCSOCHOKHSOHOOHOS
333             ae    a      il deeds

@ Dilated causal convolution
® Dilation rate= receptive 11010를 극적으로 확대 가능
@ 계산 량에 대한 부담은 매우 적음, 쉽게 1024이상의 (666016 field 가능
> (1,2.4,8,… 512) rate 사용 (10 layer ) :10 layer network 3개를 쌓아서 총 30 layer model
O™60> OO ae

= Output : quantization & multinomial logistic regression

Regression 문제를 multi-class classification 문제로 변                                   발열
utp

es          !                  128                                        1
® Quantization : audio= 보통 1601((65,536) 사용 =:                                 005
@ 65.536개의 US 분류하는 것은 너무 어려움                 84                                                      fos
48                                        0.375
@ 8bit(256)712| = quantize                         32                                          025.
/* mu-law companding 기법을 적용 (109 50816로 변환)    ra     … 골골 ue ae ae a   0
4                                              Normalized input
7 (260) = sign(ay) et lee   —1 < a < land p = 255.            _

© 다항 로지스틱 회귀
@ 관찰 된 특징과 0001!601-50600110ㅁ08「2006[6[의 선형 조합을 사용하여,
특정 값의 확률을 추정하는 분류 문제에 적용, 0「001601-50600110ㅁ8「『210610값은 훈련 데이터에서 결정
© Output
@ SoftmaxS 통해 256742] 값에 대한 확률로 계산

@한국시연구소 홍근선      -167- 무단 전재, 복제, Ll], 디지털화 금지



===== PAGE 169 =====
3부. Time Series & LSTM

3.3 Time Series Generation : WaveNet

= Gated Activation units

Gated activation unit

WEE

000                                                                                             6
@ Gated Activation Conv.                                              features DO gate conten “MEQ MDE
2 = tanh (Wy. *x) Oo (W,  ak *X) »   cane 께서 .
feature term                    sad                                                         “U
*: convolution operator                                            Wyre  "                      Wor
이 element—wise multiplication operator
k: layer index
fg: filter, gate > W is learnable convolution filter
@ = 개의 conve] 조합으로 SHS 결정, 학습 능력 St (like LSTM gate operation)
m Residual / Skip connection                                      rn Vn|
‘             -         =                                         ㅣ Residual                 i
® Residual learning : 잔차 학습                        |                       |
고
 내부의 Skip connectionS 통해                             ：             |, |  아가
* 학습량 감소                                                          I                                   :
/ 역전파에서 skip pathS 통해 errors 용이                    |
/* Ensemble 효과                                                   ㅣ
> 깊은 모델에서 안정적이고, 빠른 학습 가능                            ：
@ Skip connection                                 |
@ 외부로 연결되는 02내                                  |
[ eau activation + Residual + skip-connection ]
SC DEEP LEARNING”

m= WaveNet Architecture
® 2t layer2| 출력
® Gated activation 결과를
1x1 conv skipped Fmap2}
더하여 다음 layer AS
@ Skip-connection

두 모아서 출력 값을 생성
@ FmapS 256으로 맞추기 위해

# 2t layer2| Gated activation 값을

Skip-connections

Output

1x1 conv. 추가

®@ 30712] FmapS 더하여
(ReLU > 1x1) x2

® SoftmaxS 통해
출력 값을 확정

적능              ：     :
때 90011 |     { _540-690000000
——
- 0 __‥
input
0
006 1000800 + tx! (256
512
we 512          이           aa 8 14)

Ek eee 이오 으

256

> Sequential data2|   —_—  레미 512 age
dependencyS 학습,         대     [siz
다음 024확률을 예측 an BR) Ch. ^"
는 0 19
Causal Filler
336                                             SR DEEP LEARNING”
@한국시연구소 Sa           -168- 무단 전재, 복제, will, 디지털화 금지



===== PAGE 170 =====
3무. Time Series & LSTM                                     3.3 Time Series Generation : WaveNet
=  Results                                                                                      |             Subjective 5-scale MOS in naturalness
Speech samples                 | North American English            Mandarin Chinese
LSTM-RNN parametric      |          3.67 + 0.098                   3.79 + 0.084
HMM-driven concatenative |          AB6 + 0.137                    3,47 + 0.108
WaveNet (L+F)               |          4.21)+ 0.081                     4.08 + 0.085
Nataral (8-bit j-law)                    4.46 + 0.067                     4.25 + 0.082
Natural (16-bit linear PCM)             4.55\+ 0.075                      4.21 + 0.071
Ss              uv ^  oy
입              =     s
Par, Gee

© Text To Speech
@ MOS: 사람에 의한 평가
/* mean opinion score
aw1~5
® L: linguistic features,
®@ F: Focondition 추가 (Fo: logarithmic fundamental frequency)
© Multi-Speaker Speech Generation
학습하여 SAS 구분 학습하고, 생성
, 녹음 품질도 모방함

® Music

® 10989) 음성을
@ 화자의 호흡, 입 움직임 + 음향
@ 장르, 악기 139에 따라 음악 생성
< Speech Recognition
® Model 변형하여 실험 , TIMIT datasetOJA] 18.8per (최고수준은 아님)

제비

“S8P DEEP LEARNING

Pais

3.3 WaveNet, TCN, Non
[실습 1] WaveNet
8 목적 : WaveNet 모델을 살펴보고, 간단한 0313
we 실습 개요
@ WaveNet 전체 codeS 살펴보고,
© 모델에 적합한 data 형태로 00 datas 수정,
* 모델을 0312에 맞도록 부분적으로 수정하여,

* 학습 및 추론 과정을 실습

= \316461에 맞는 ㅁ0313561?
¢ Audio signal2| 특징
ㅎ 평균 00] 수렴
 크기 Alét(max magnitude7t fix)
0’ crossing 하는 경향
oO

@ Stock data2| 특징
@ 장기적인 경향성, 중기적인 파동, 단기적

fas

Ojo
ru

@ 큰 신호일 수록 '0
@ 작은 신호가 상대적으로 중요 (인간의 인지 방식)
, 단기적인

-169_

pseudo random, 큰 신호가 중요(수익)

개
무단

Sl,  디지털화 az

Al, 복제, 2

is

cee

@한국시연구



===== PAGE 171 =====
3부. Time Series & LSTM                      3.3 Time Series Generation : WaveNet

= Dataset 준비
@ EMA (Exponential Moving Average) S 기준으로 가격 HSS 표시
@ ema5, ema20, ema100z} 현재 가격의 차이 값을 사용해 보자
/* Close 0218에 ema 적용 > 각 ema 0212생성 > diff( ema - close ) 계산
/* Normalize : diff 0213를 각 6008로 나눔

a df[’ema5'] = df['Close'].ewm(5).mean()
3 df_data["diff5"] = (df_data[”ema5"]-df_data["Close"])/df_data[“emaS"]

 층분하진 않지만 Audio 991히과 유사해 보임
 충분하진 않지만 44010 990리과 유사해 보임

a2
so et  A 7   Fre rg!   az
기] 해   eraser | °°

03                                           ad       ie
고                                             \ vi        -ㅇ~
B.S.
C        ea       20      pres      200      parry      Baer            =            그새          BOOS          BOSD          00

@ Sequence 생성 : audio} 매우 긴 data, stock 0312는 상대적으로 매우 BS data
 전체 datas 544 time stepS 갖는 560.로 변환 : ( 4708,3 ) > ( 129, 544, 3 ), skip_rate=32
/ xs_train (input samples), ys_train (target samples)

= WaveNet coding : ref. httns://aithub.com/basveeling/wavenet

일
® Residual Block : pseudo code
&     def residual_block(x):                                                i
5          original_x = x                                                             :
6        tanh_out = CausalAtrousConvolutioniD(..., activation=‘tanh')(x)         ‘
?        sigm_out = CausalAtrousConvolution1D(..., activation="sigmoid’ )(x)       |
a        X= layers.Multiply() ([tanh_out, sigm_out]) ## element-wise            1
5
16       res_x = layers.ConvolutioniD(nb_filters, i, kernel_regularizer=12(res_12))(x)
골도       skip_x = layers.ConvolutioniD(nb_filters, 1, kernel_regularizer=12(res_12))(x)
12        res_x = layers.Add()(foriginal_x, res_x])                             ㅣ
33       return res_x, 5616 ×

® Stacking Layers : pseudo code
a5    input = Input(shape=(fragment_length, nb_output_bins}, name='input_part')
16     out = input
iy     skip_connections = []
18     out = CausalAtrousConvolution1D(..., name=‘initial_causal_cony’ }(out)
18     for s in range(nb_stacks): 0000메서는3                   4
20        for i in range(@, dilation depth +1): 6077”              her
2           out, skip_out = residual block (out)                 기
2           skip_connections. append(skip_out)
Me
340
=       AS                _    =            HF      턴ㅎ[ 그
@한국시연구소 홍근선                 170 - 무단 전재, 복제, S4, 디지털화 금지



===== PAGE 172 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

+ pee pseudo code

cut = layers.Add(}{skip_cennections) # element-wise
out = layers. Activation(*relu‘) (out)

out = layers.ConvolutioniD(i){out) # ixi cenv

out = layers.Activation(‘relu') (out)

out = layers.ConvolutioniD(i)(out) # xi conv

out = layers. Activation(’ softmax‘) (out)

model = Model{input, out)

Skip-connections

® CausalAtrousConvolution1D(Conv1D)

### Pseudo code : CausalAtreusConveLlution1o(>)
class CausalAtrousConvolutioniD(ConviD) :

def init__(self, filters, kernel_size,...}:
super (CausalAtrousConvolutioniO, self)..init__(filters, kernel_size-kernel_size,...)

def call{self, x):
x = asymmetric_temporal_padding(x, self.dilation_rate[@] * (self.kernel_size[@] - 1), @)
× = super (CausalAtrousConvolutioni1D, self) .call(x)
return x

tf. keras. layers. Convib(
filters, kernel_size, strides=1, padding=‘valid’,
data_format=' channels   sti,  dilation rate=1. 1, groups=i,
activation=None, 456 |   True, kernel _   {tielizer='glorot_uniform’,
bias_initializer='zeros’, kernel_regularizer=None,
bias_regularizer-None, activity_regularizer=None, kernel_constraint=None,
bias_constraint=None, **kwargs

OM DEEP LEARNING |

————

® Model modify

@ Output activation : softmax > linear

“ Audio| log base encoding 된 256(8bit)\S29| classification 모델 사용
_@ 우리는 3가지 diff_ema signal 예측으로 사용

| 51 4    out = Layers. Activation( ‘softmax', name="output_softmax") (out)
| 52      out = layers.Activation('linear‘, name="output_activation") (out)
| 53     model = Model(input, out)

주요 Hyper parameters
/* dilation_depth : 9 > 8 (1,2,4,8 16,32,64,12
/ desired_sample_rate : receptive field 계산에 사용, 4410 > 7
“ nb_filters : # feature map, 256 > 64
“+ nb_output_bins : # 보비 elas,  256(class) > ‘isk regression)

p-conmections
>   Model t test                                                                                    Generation data(red) / Test data 비교
#8 Generation 50                                                          들
out_list=[]                                                               :

for i in range(5@):
output = model.predict(last_sample) # seed@ 사용혜시 50 point 성상
last_sample = np.append(last_sample[:,1:,:],output[:,-1:,:],axis=2)

ty 6 RA Be ee

- 171 - 무단 전재, 복제, Stl, 디지털화 금지


===== PAGE 173 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

* TCN(Temporal Convolutional Network)
: “An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling”, 2018

® TCNE Causal convolution® = 구성, 미래에서부터 과거로의 정보 유출이 없다는 것
®@ 1d-dilated causal convolutional networks 사용

/* WaveNetOlj 기반, Layer stackOl|A        오는 skip connection 제거,6216 activations

@ 100바과 동일한 길이의 output (RNN 방식)

® RNN 대비
@ 병렬처리, 더욱 긴 시계열 처리(안정적 학습), 학습 memory 감소
@ 추론 시 memory 증가, 구조적으로 길이 결정(전이학습 어려움)

* Architecture                   TT ick 이사나해) a
‘Residual block (k, d)                       :
to th oe      ia      e-2 97-1 Pr       :          t                  기분. block .
a MB ourpue   :            wi                        i
가      :        iegeio
;        Dilated Causal Conv
MP viacen :               +                  707 Conv
「'           @=3                           +
;                               RelU
을 viiaaen                       +
WeightNorm
"/]0=1
을 애마
fo 41 02       ove     27271 LT
343                            Devoe aseiens

@ Receptive Field = 1 + (kernel size - 1) x (sum of all dilation rates)
/ Kernel size = 3

/* 각 블록에 두 개의 Conv layer7} 92.0}, dilation rate7t 각각 [1, 2, 4, 8]

/* 전체 8개의 layer2| dilation rate sequence : [1, 1, 2, 2, 4, 4, 8, 8]                  {              가의
/* sum of dilation rates: 1 + 1 + 2 + 2 + 4 + 4 + 8 + 8 = 30" te   >:
wv

「     vy
@. 20] receptive 11810를 활용하려면 61 time step                                           보내서   44   V4.
ㅎ seq. length7} Receptive 11810보다
* 짧은 경우 : Model 설계와 불일치, 학습할 수 UWE pattend| 제한 되므로 성능 감소
 긴 경우 : 입력 AHAY 추가적인 앞부분은 직접적으로 최종 SHO] SHS 주지 않음

player
yrbt 사용한다면 추가 길이는 의미 없음                        AS

/
© 마지막 시점 출력만 사용하는 경우(단일시점 예측)                           페레          ~  aul
® Seq. length >= Receptive field                                              De a hee
/* yr tt 출력으로 사용 하거나,                                                              때
/* 》…7-1출력을 묶어서(1360, avg. pooling) 사용                      싸서
@ Sequence-to-Sequence 예측의 경우                            0        비애

ㅎ Seq. length >= Receptive field
A 출력들을 모두 사용
* yo 충분한 정보를 가지려면.
/* Seq. length = Receptive field *. 2



===== PAGE 174 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

“Temporal Convolutional Networks for Action Segmentation and Detection”

© \1060에서 인간 동작을 식별하고, st(action segmentation or detection) task
@ ED-TCN: Encoder Decoder TCN 구조, Dilated TCN 구조 제안

고 두                                                 Predict: ¥
|
|

50 Salads                                                 GTEA

“MS-TCN: Multi-Stage Temporal Convolutional Network for Action Segmentation”

© \1060에서 인간 동작을 식별하고, 분할(30100 segmentation or detection) task
@ 여러 단계의 dilated conv, Layer(causal 000\.아님))로 구성, 행동 간의 의존성을 포착
@ 각단계는 고해상도 시계열 정보를 유지
@ Total lose = class loss + Smoothing Loss(T-MSE: Truncated MSE)
/ 각 state 의 loss 를 sum

l= pa      ies a ~ ss ALT MSE:
8

1                               글       —                Peslct: ¥
Lets = T ” -609(0.0ㆍ   Creuse = TC 0”                      Stage N              _—— 벼
:             “^ 6           ㅇ<.0 ㅇㅇ 으으우이0.0.0.0 04 우

/* Truncated Mean Squared Error (T-MSE):
& Ay = [10g Yee — log yx-1.cl

t2} t—1 ALO] 2] class 에 대한 109 prob. 차
/* 2, .: AS 7크기로 제한
7: frame 수, C: class 수

6  Ui! 006

@한국시연구                    무단 전재, 복제, Lal, 디지털화 금지


===== PAGE 175 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

nS 주요 연구
® MS-TCN++ (Li et al., 2020)
 여러 stage TCN SSS 사용하되, Zt stage 사이에 정교한 refinement 추가
@ 초기 예측이 부정확한 구간을 후속 스테이지가 점진적으로 보정
* ASFormer (Action Segmentation Transformer, Yi et al., 2021)
@ 1D convolution(local context) + multi-head self-attention(global context)
@ MS-TCN2} 비슷한 multi-stage 구조 + attention
© TCFPN (Temporal Convolution Feature Pyramid Network),2018
@ Feature Pyramid Network(FPN)S 적용, different dilation rates 에서 추출한 SAS 결합
@® YAS 결합해, 작은/큰 동작 변화를 모두 잡으려는 접근.
@ Temporal Deformable Convolution,2019                       K
@ Deformable Convolution: 학습된 dilation(A,) 추가                02 ~060ㅜ+
/* 불규칙한 시계열 데이터를 처리할 때, 고정된 0113400보다 효과적으로 정보 포착
@ Non-Local blocks(Wang et al.),2018
@ ConvNetOl self-attentionz} 유사한 메커니즘을 삽입
@ 시계열 전역의 정보(먼 과거~미래 프레임)를 한 번에 참조할 수 있음

_ 347                                                                                           “St DEEP LEARNING  |

a 이후 주요 연구

® 기타 구조 및 변형
@ C2F-TCN (Coarse-to-Fine TCN): 거친 time 508!6에서 먼저 예측 후, 세밀한 time scale= 점진적
refinement
®@ ASRF (Action Segmentation from Restricted Frames): CNN/TCNS “S|, S44 sampling=! frame
정보를 사용하여 segmentation
a 정리
ㅎ MS-TCN++, TCFPN, ASFormer(Transformer 혼합), Deformable/Non-Local 기법 등은
모두 긴 시계열에서 다양한 시간 스케일을 포착하기 위해 발전한 구조들
 시계열 SegmentationS event 경계를 정확히 찾는 것이 핵심이라, multi-stage
refinement} multi-scale feature aggregation 기법이 자주 도입 =

8재, 복제, S4l], 디지털화 금지

@한국시연구소 홍근선                    -174- SH



===== PAGE 176 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

© TCFPN (Temporal Convolution Feature Pyramid Network)
@ Encoding-Decoding2}AOlAj 만들어진 feature map 을 U-Net 구조로 결합하여 사용
/＊ Object detectionOJA] 주로 사용
 시계열 분할을 위해 사용하였음

Encoder                                                                                 Decoder
1x1 Conv

1D Conv
1D Conv + BN + ReLU + Pool  —— 욱

Upsample

1x1 Conv
                        :
1D Conv + BN + ReLU + Poo!

Upsample
a                                  1D Conv

iD Conv

1x1 Conv

ee

때     ise) FC + Soft

=

= Non-Local blocks, 2017) ye ie  wee  사  (시케며이  E34   cp) )
* 임의 두 점의 관계를 계산, long range dependencyS 직접적으로 계산
®@ Non-local Neural Networks9] 핵심 구조, 모델의 일부에 Non-Local blockS 삽입해서 사용
 임의 두 점의 관계를 계산. lona range dependencyS 직접적으로 계산할 수 있음

호 = 가 2, f (xis 809(000)

© f(%. yi): Pairwise term, = 점의 관계 학습, g(x;): Unary term, Ha} 전체의 관계 학습

@ Self-attentionz} 구조적으로 동일

 107890에서 object detection / segmentation, Video 500.에서 action recognition 적용
> YS} 되어 attention PAAH 사용 가능함

@ 시계열처리에서 1dCNN, RNN2} 결합해서 사용함

&

-175- 무단 전재, 복제, Shall, 디지털화 금지



===== PAGE 177 =====
3부.11

me Series & LSTM                     3.3 Time Series Generation : WaveNet

Disentangled Non-Local Neural Networks, 2020

®@ Pairwise, Unary term 더하기로 분리, 역할이 분리됨
/* 각각 SoftMax= add

@ Whiten: 각각의 평균을 빼서 bias Ai]7{(Layer Normalization 사용)

@ Relative bias 추가
& (0) 위치와 (@)위치의 상대 차이를 계산, 시계열의 경우 각 시간 |와 ]의 차이 i-jS
/& Pairwise = softmax(relative_bias + (LN(q)" « LN(k))

Disentangled Non-Local Neural Networks

i
1
1
1
'
1
i
1
1
ㅣ Attention
| … ㅣ Generation
OW,  1 Block
i
1
1
1
1
'
1
|

x    x
——

ee ee 쓰】애에에 싸애아세아

‘
'

'

'

'

'

'

'

'
us
'

'

I

'

'

'

'

'

'

eee ee

s       호       a

eee ee            Rew ewe ewe   wee eee eee

T
a
8
용

18

12

12

13

14

15

36

32

318

19

20

23

22

23

24

25

26

22

28

20

30

34

32

33

34

35

aims
CN 모델 구현                                                                  ‘Residual block (k, d)

def build_tcn_model2(seq_length, num_features, dropout_rate=@.15):   1
inputs = Input(shape=(seq_length, num_features})
x = inputs
num_filters = 64
kernel_size = 3
# 여러 dilation rate 사용한 BEG 쌓습니다.
for dilation_rate in [1, 2, 4, 81:
prev_x = x
# 첫번째 dilated conv layer (causal padding)

x = ConviD(filters=num_filters, kernel_size=kernel_size,     ;
dilation_rate=dilation rate, padding=‘causat’)(x) |

x = BatchNormalization() (x)                                 }

x = Activation(‘relu’) (x)

x = Dropout (dropout_rate) (x)

# 두번째 dilated conv Layer

x = ConviD({filters=num_filters, kernel_size=kernel_size,
dilation_rate=dilation_rate, padding=‘causal')}(x}

x = BatchNormalization(} (x)

x = Activation('relu'}(x)

x = Dropout (dropout_rate) (x)

# 입력과 출력의 채널 수가 다르면 1x1 convolution©ee 맞춤

if prev_x.shape[-1] != num_filters:
prev_x = ConviD(filters=num_filters, kernel_size=1, padding='same')(prev_x)
# residual GB
x = Add()(iprev_x, x))
x = Flatten() (x)
outputs = Dense(i, activation="Linear’) (x)
model = Model(inputs, outputs)
return model

@ Receptive Field = 1 + (3 - 1) x (30=1+1+2+2+4+4+8+8) = 61

Al, 복제, Sl, 디지털화 금지

무단 전


===== PAGE 178 =====
3부. Time Series & LSTM

3.3 Time Series Generation : WaveNet

® output mode 지정 하도록 수정
®@ last_one: 마지막 》〉,만 출력으로 사용
® flat_one: 모든 >,를 13161 layers 거쳐 출력으로 사용
® Many: 560.10 500. mode, 모든 y,B 출력
# Target data& output modeOl 맞도록 준비

oe

21         # residual 연결

22         x = Add()((prev_x, x))

23     if out_mode == ‘last_one' :

24        print('last_one')

25         ## 마지막 ety 출력만으로 예축 ： many to one ##

26          x= ×[1,       aul

27       outputs =  1661, activation=’ Linear’) (x)             # (bs,1)
28     elif out_mode == ‘flat_one' :

29               print( HH ane! )

30         버 BARS] SAB 결합해서 예측 ; many to one ##

31                        = Flatten() (x)

32        we  - Dense(1, activation=' Linear’) (x)             # (bs,1)
23     elif out_mode == ‘many' :

34         print(‘many')

35        ## 각 시점의 BABB 예측 ： many to many HH

36        outputs = Conv1D(filters=1, kernel size=1, padding='same')(x)# (bs,seq,1)
37     else : print(' ‘out mode error!)

38     model = Model(inputs, outputs)

39      return model

| 7 seq_out = False if out_mode in ['last_one', ‘flat_one'] else True
ㅣ 8 x_train,y_train,x_test,y_ test = seq gen n(X,Y,seq_length, seq out=seq_out)

isha

‘SOP DEEP LEARNING”

가

8 WaveNet 모델 구현 : Receptive Field = 1 + (3 - 1) x (31=1+2+4+8+16) =

1 def 「6510486ㄴ6106, filters, kernel_size, dilation_rate):

고     # 두 개의 BB convolution (Aloe)
3     conv_filter = ConviD(filters, kernel_size, dilation_rate=dilation_rate,
4                         padding=‘causal’) (x)
5     conv_gate = ConviD(filters, kernel_size, dilation_rate=dilation_rate,
6                                            padding='causal') (x)
7      tanh out = Activation('tanh’)(conv_filter)
8      Sigm_out = Activation('sigmoid') (conv_gate)
9      merged = Multiply()([tanh_out, sigm_out!)
10     # 1x1 6000014【101으로 skip 연결 생성
311    skip = ConviD(filters, 1, padding='same') (merged)
12     # residual 연결; 입력과 skip 더합 (채널 수가 Cel 1x1 conv 사용)
13     if x.shape[~1] != filters:
14        x = ConviD(filters, 1, padding='same') (x)
a5      res = Add()(ix, 56101)
16     return res, skip
18 def build_wavenet_model(seq_length, num_features,out_mode):
19     inputs = Input(shape=(seq_length, num_features} )
28      x = inputs
21     skip_connections = []
22      num_filters = 64
23     kernel_size = 2 # WaveNet0iAle 보통 kernel size 28 사용
24     dilation_rates = [1, 2, 4, 8, 16]
25     # 여러 residual blocks BSH" Sip connection 수집
26     for dilation_rate in dilation_rates:
27       x, skip = residual block(x, num_filters, kernel_size,.dilation_rate)
28            skip connections. append(skip)
29     # 모든 skip connections 더한 후 활성화 및 flatten
30      x = Add() (skip_connections)
31      x = Activation('relu'){x)
32      x = Flatten{) (x)
33     outputs = Dense(i, activation='linear')(x)               # (bs,1)
eas ot     model = Model(inputs, outputs)
|  354 35     return model
@한국시연구소 S24                  - 177- 무단 전재, 복제, 4,  디지 털화 그지


===== PAGE 179 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet

= Non-Local blocks 구현

1 def non_local_block(input_x, intermediate_dim=None, compression=2}: Compre
2               input_shape = tf.keras. backend. int_shape(input_tensor)
3      channels = input_shape[~-1]
4    theta = ConviD( intermediate dim, kernel_size=1, padding="same use_bias=False) (input_x)# (B, 1, C')
5     phi = ConviD(intermediate_dim, kernel_size=1, padding='same', use_bias=False)(input_x) ¥# (B, T, C‘)
6     phi = tf. keras. layers.MaxPool1D(pool_size=compression, strides=compression) (phi)       # (B, T//div, C')
a     g = ConviD(intermediate_dim, kernel_size=1, padding='same', use_bias=False) (input_x)   #1, C)
8     g = tf.keras. layers.MaxPooliD(pool_size=compression, strides=compression) (g)          # (8, Tdi, C)
9    # Compute similarity: (6, T, C’) x 18, €’, T//compression) -> (8, 1, T//compression)
10      = Lambda(lambda x: tf,matmyl(x[@], ×[11, transpose_b=True))({theta, phi!)
a     # Apply softmax along last axis
12      f softmax = Softmax(axis=~1) (f)
13     # (B, T, T//compression) x (B, T//compression, C') -> (8, T, C‘)
314     y = 1806086(180008 x: tf,matmul(x{@], x{1]))( [ft softmax, 91)
a5     # Restore channel dimension
16     y = Convib(channels, kernel_size=1, padding='same’, use_bias=False) (y) 2                           iE
17     output = Add()({input_tensor, 1) # Residual connection     i                x
18      return output                                          i                 |
i

@ Conv. use_bias = False ?
ㅎ Non-Local 연산에서는 theta2} phi2] 내적으로 유사도 계산
* bias7} 포함되면, 내적에 offset] 추가되어
 유사도 값이 왜곡될 수 있음
@ Residual connection
@ Weighted 된 feature= 입력 feature 와 pointwise add

i

i
i
i
i

@ Non-Local Neural Network (with CNN)

9     inputs = Input(shape=(seq_length, num_features))

18      x = inputs

at

12     # 초기 Convil 블록 (SAKES 추출)

13      x= Cony1p( filter<64)  kernet_sishes, padding='same', activation='relu') (x)  28  모  인성
34     x= Conv1D({ filters=64, kernel_size=3/ padding='same', activation='relu')(x)*  에즈

a5

16     # Non-Local Block 4: 전체 시원스의 전역 정보를 반영

17     x = non local block(x, intermediate_dim=64, compression= a

18     x = non local block(x, intermediate_dim=64, compression=2    e Obvipt- 이이 땐 ANE”
19

20     # 추가 Convid (선택 사항, 더 복잡한 Se 추출을 위해)                             그기 Poke?
21    x = Conv1D(filters=64, kernel_size=3, padding='same', activation='relu')(x) |        t
22

23     x = Xie ed 11

24     outputs = Dense(i, activation="linear')(x)               # (bs, 1)

25      model = Model(inputs, outputs)

4 Leh -Local Neural Network (with RNN)

inputs = Input(shape=(seq_length, num_features?)

4      x = inputs

i

12     : RNN Layer (seq. BQ 추출)

13           = Bidirectional (GRU(64, return_sequences=True) } (x)

34           = 8101[「660Ｌ1008니660(64, return_sequences=True)) (x)

15     ? Non-Local Block 적용; 전체 APACS! 전역 정보를 반영

16     x = non local block(x, intermediate_dim=64, compression=1)

1?     x = non_local_block(x, intermediate_dim=64, compression=1)

18                            SS

19     # 추가 Convid (선택 사항, 더 목집한 BA SBS 위해)

20     x = Convi1D(filters= 64,  kernel_size=3, padding=‘same’, activation=‘relu'}{x)

21

22     ## 마지막 시점의 출력만으로 예측 : many to one HH

23    =, -1, 3]

24     outputs = Dense(1, activation='linear’)(x)               # (bs,1)
| 356 | 25     model = Model(inputs, outputs) —__

@한국시연구소 홍근선             -178- 무단 전재, 복제, Bal, 디지털화 금지


===== PAGE 180 =====
3부. Time Series & LSTM                     3.3 Time Series Generation : WaveNet
3              TCN                                                                       |

“Time Series is a Special Sequence: Forecasting with Sample Convolution and Interaction”, 2021
 특정 A|AlSOA Transformer 계열이상의 ASS 보임
@ 시계열의 S82 Trend, Seasonality, Irregular Component= 분해될 수 있다고 봄
기존 YHYS Irregular <0010ㅇ01060[처리에 취약함
® SCINet(Sample Convolution and Interaction Networks) 구조 제안
® SCI-Block : odd, even frame 2 & L}+=0} Irregular Component =4S

/ Features odd, even? = 나누고, 0,$,,0는 서로 C= convolutional kernel
f+ ㅇ: element-wise product

@ SCiNet : 섞여 있는 FeatureSS 병합하고 정렬, 입력과 더하고, FC LayerOlAq 시계열의 길이를 rz 수정
@ Binary Tree2| PAS 만든 것이 5046 추출되는 시계열의 길이는 27} 됨

(a) SCI-Block                                               (b) SCINet                                       (c) Stacked SCINet
Input: F                                         Input: RF~! (x if k = 1)                                       Input: X
|
『.                                      [ey
| Split                            *                                                                                       Aevel=1
30                                      evel =2
odd          Leaming          :  even              ad                     G 가여: 개
호
\                                       a               !                       us                       J
*                                iJ                                           ㆍ
Foaa                                  Foven                                            Onput: K*                                                          Output: R®

DEEP LEARNING

ee eee

m SCINet 구현

® SCI-Block : odd, even frame2& 나누어 Irregular Component 특성을 학습
@ 분할과 특징 추출
@& MASS 짝수와 SES 분할하여, 각 분기에서 00110 레이어를 통해 local SAS 추출
- 두 분기가 독립적으로 SAS 학습 > 특정 패턴이 한 분기에만 국한될 수 있음
 상호작용(1016「3800101) 메커니즘
 각 분기에서 추출된 SAS 반대 분기의 정보를 활용하여 03160 =
* 짝수 분기의 SAS 홀수 분기의 SAS 기반으로 03160 신호로 변환됨
* 98[6신호에 exp 이 사용되어, 서로 다른 분기의 특징이 얼마나 중요한지를 비선형적으로 조절

4 def SCINet_block(input_tensor, filters=64, kernel_size=3, dropout_rate=@.1):

5    #1. Split : Be/Bp 인덱스로 분할

6    even = Lambda(lambda x: x{t, 112, :])(input_tensor) # shape: (6, T/2, C)

ig    odd = Lambda(lambda x: x{:, 1::2, :])(input_tensor) # shape: (6, T/2, C)

8     #2. 지역 특징 추출 : 분기에서 local feature 추출 (Convid + Dropout)

9    conv_even = Convl1D(filters, kernel_size, padding='same', activation=’relu') (even)     (a) SCL-Block
18      conv_even = Dropout (dropout_rate) (conv_even)                                           Input: F
11    conv_odd = ConviD(filters, kernel_size, padding=‘same’, activation='relu') (odd)
12     conv_odd = Dropout (dropout_rate)({conv_odd)                                  「                 1
13     # 3. 상호작용(10【『6(666【『100): 반대 분기의 특징으로부터 1x1 Conv 및 exp 통해 gate value 계산   를  ,             t
14     gate_from_odd = ConviD(filters, 1, padding='same') (conv_odd)                  an

a5     gate_from_odd = Lambda( lambda x: tf.exp{x)) (gate_from_odd)                    :

16     gate_from_even = ConviD(filters, 1, padding='same'}(conv_even)                y

312     gate_from_even = Lambda( lambda x: tf.exp(x)) (gate_from_even)                   t

18     #4. Residual Interaction: 원본 분기와 상호작용 결과의 곱을 더함

19     even_out = 400() (16060, Multiply()({conv_even, gate_from_odd!)})
28     odd_out = Add()(fodd, Multiply()({conv_odd, gate_from_even] )})
21     #5, Merge: interleavingee 병합

22     merged = Lambda( lambda tensors:

ㅣ 23           interleave_layer{tensors[@], tensors[1]}}(leven_out, odd_out!)
g 24    return merged

@한국시연구소 Sc            -179- 무단 전재, 복제, Wi, 디지털화 금지


===== PAGE 181 =====
3부. Time Series & LSTM                      3.3 Time Series Generation : WaveNet

® SCI-Net : Sample Convolution and Interaction Block
@ 섞여 Qe FeatueSS 병합하고 정렬, 입력과 더하고, FC Layer AAS] BOS t= 수정
/ Binary 1166의 구조로 만든 것이 5014허, 추출되는 시계열의 길이는 그가 됨

4 def SCINet_recursive(x, level, max_level, filters=64, kernel_size=3,                   ib) SCTNet
5                dropout_rate=@.1, num_blocks=1):                          faput: R-? OER = 1)
6      if level == max_level: # max_leveld] 도담하면 num_blocks7i2] SCINet_block# 적용
7         out =
8        for _ in range(num_blocks):
9          out = SCINet __block{out, filters, kernel_size, dropout_rate}
18         return out
11     else:              #2 외의 경우, 입력을 분할, 각 분기를 하위 레벨로 재귀 Se
12       «# BE: 찍수/을수로 나눔
233        even = Lambda(lambda x: 1, 112, :]) (x)
14       odd = Lambda(lambda x: x[:, 1:22, :}) (x)
15         # 하위 레벨로 재귀 호출
16         processed_even = SCINet_recursive(even, level + 1, max_level,
127                        filters, kernel_size, dropout_rate, num_blocks)
18        processed_odd = SCINet_recursive(odd, level + 1, max_level,
19        7                    filters, kernel size, dropout rate, num blocks)
28       TP 상푸작용: 하위 레멜에서 얻은 분기 각각에 대해 추가 Convid 및 게이트 연산을 적용
231        conv_even = ConviD(filters, kernel_size, padding='same',
22                                                                 activation='relu') (processed_even}
23       conv_odd = ConviD(filters, kernel_size, padding='same',
24                               _ activation='relu') {(processed_odd)
25        gate_from_odd = ConviD(filters, 1, 0000109='5306')(000\_000)
26         gate_from_odd = Lambda(lambda x: tf.exp(x))(gate_from_odd)
27        gate_from_even = ConviD(filters, 1, padding='same')(conv_even)
28         gate_from_even = Lambda(lambda x: tf.exp(x))(gate_from_even}
29       1,
30         even_out = 600()([0『0665560_6460, Multiply()([conv_even, gate_from_odd])}/)}
31        odd_out = Add(}{[processed_odd, Multiply(}([conv_odd, 9216 _7「00_60\601)1)
32
33:        merged = Lambda(lambda tensors: interleave_layer{tensors{@], tensors{i]}}({even_out, odd_out!)
34         return merged

@ Stacked SCINet
@ 각 스택마다 부분 예측과 Loss 구해 합산함

8 def 6410. Stacked _SCINet_with_intermediate_losses(

g              seq_length, num_features,

10                stack_times=2,

ai             max_level=2, num_blocks_per_level=2,

12                   filters=64, kernel_size=3, dropout_rate=8.1):

33     inputs = Input(shape={seq_length, num_features) }

14      x_current = inputs

15     intermediate_predictions = [] # 2] 스택의 MSS HBB 리스트

16     for i in range(stack_times):

37         # 비거 layer

18       x  = Convin( tat hers kernel_size, padding=’same', activation="relu’ ) (x_current)

19       # 멀티레벨 ScINet (재귀적) AB: (6) 구조                                 ：
20       x Stack =  SCINet_recursive(x, level=1, max_level=max_level,           (c} Stacked SCINet
21                          filters=filters, kernel_size=kernel_size,       Inpot: X
22                                 dropout_rate=dropout_rate,                   ‘     2
23                               num_blocks=num_blocks_per_level}

24        # 중간 WE: GlobalAveragePooling + Dense BA 출력 생성

25          pool = GlobalAveragePooling1D({ ) (x_stack)

26        pred = Dense(1, activatinn='Linear', name=f"pred_{i+1}") {pool}

27                         intermediate_predictions.append(pred)

28        # 다음 스택으로 입력으로 사용할 RS 생성하기 위해 현재 스택의 출력과 기존 BSB concat

29         x_current = Concatenate(axis=—1)}{{x_current, x_stack!)

38     # GWE 여러 중간 예축을 출력하므로, multi-output 모델이 됨,

ae     model = Model{inputs=inputs, outputs=intermediate_predictions}

32      # 2} 출력에 대해 동일한 MSE [.056를 사용하고, SW 가중치로 Besse 설정

33     losses = {f"pred_{i+1}": "mse" for i in 「8006(5180 ㄴ065)}

34     loss_weights = {f"pred_{i+1}": 1.@ for i in range(stack_times)}                 :
35    model. compile(optimizer='adam', loss=losses, loss_weights=loss_weights}      Ouspus: R*
36      return model

y DEEP LEARNING”
@한국시연구소 홍근선                   - 180 - 무단 전재, 복제, SH, 디지털화 금지



===== PAGE 182 =====
3부. Time Series & LSTM

3.3 Time Series Generation : WaveNet

® Seq. length! 결과 (stack_times=2)

val_mape
Training loss                                   val loss            (val_pred_1_mape:1.695)(val_pred_2_mape:1.683)
i          —~ SCINeAvgPoot) | 10!         same SCINGRLAV GP OOH?
xed)                     :
     5         100                          10?
|      seq_length: 8
30:  |                       x02                            nem SCINEtAvgPoolval pred 1 mape
:                              거너 SCINet(AvgPool)val_pred_2_mape
108-2  i                      622  4                       208  :
~
10?      ao                  ad                        on ae             ;
Ri 00 | | 30        거버 OOF TN PE ar                       fol edases,
8   20 «4 60 80 3100     6   20 49 60 80 100     a   20 40 68 86 300
val_mape
Training 1059                                   val loss            ival_pred_1_mape:1.825)(val_pred_2_mape:1.736)
10%             SCINEt AvgPoo!}              oem StINET AYgPORT)    거세 SCINeL(AvgProlval_pred_I_mape
10?          “             | 36
commen SCUMOt AvgPoolval pred Z mape
10?     ~      Sones      ‘
‘          et
seq_length : 16                                          』
383     =                     108                          10
zo"?
19-1                                                        '
                   103 | aE                  104  ‘.
alia      ina  10?     ae           se OUP Oe         Ot inonsatittschcmedioscens|
2   20 4 60 80 100     @   20 40 68 80 100     °   20 40 66 86 100
val_ma
Training loss                              val_loss          (val_pred_1_mape:2.319)}(val_pred 2 mape:2.545)
a                                                    6 4                          =                            -
a  4     ~~ SCINeLAvgPaol)  sa  :     ————  SCINGNAvgPast)  ae 홈
107  \                       305                       sor fe)
108 + seq-length: 3          apa id                              10%                   i     :
worded                            |                         ~om SCINEt AvgPoolval_pred_1_mape
：   |                       29?   |                       Wem SCINet{ AvgPoal)val_pred_2_mape
305   3
|                       209 -  |                       yo? 14}
오글 Sees oesa    coed 10      aoe         ee   aie     ome
6   20 40 60 60 100     o 20 40 66 80 100     0 2 4 66 60 300

55995

=

치시 DGIO] AD} -
* 최신 모델의 성과 : h                                                   ETTh1 (336) Multivariate          D-PAD
® Seq. length3= SOTA7| 다른 이유는?                                     ~ 56016088
@  Univariate vs  Multivariate                                          ETTh1 (720) Multivariate          DiPE-Linear
ivari.     성능          쁘
시 왜 Multivariate 성능이 더 US7t?     ㄱ yr nba  자는  ETTh1 (192) Multivariate         PatchMixer
@ 왜 Seq. 1609해가 길어지면 성능이 더 Ls}?
Dakelert  ：      ETTh1 (96) Multivariate           SegRNN
ETTm1 (192) Multivariate                  xPatch
RESULTS OF MULTIVARIATE LONG-TERM FORECASTING
Methods |   D-PAD   |   DLinear     *N-HITS      *LaST     2SCINet, | FEDformer | Autoformer | Informer [|     IMP
00008 | (Ours)     (AAAI 2023) | (AAAT 2023) | (NIPS 2022) | (NIPS 2022) | (ICML 2022) | (NIPS 2021) | (AAAT 2021) |

Metrics | MSE MAE || MSE MAE MSE MAE MSE MAE MSE MAE MSE MAE MSE MAE MSE MAE

192
336 | 0.374 0.406} 0
720 | 0.419 0.442 3| 0.472

0.416

ETThI

96 | 0.357 _.0.376,1| 0.375 0.399 0.475 0.498 0.395 0.407 [0.401 0.400: 0.376 0.415 0.435 0.446 0.941 0.769 4.80% 5.76%

0.394 0.402      z   0.492 0,519 0.463 0.456 10.468 0.457} 0.423 0.446 0.456 0.457 1.007 0.786 2.72% 3.37%
0.550 0.564 0.556 0.502 10.516 0.509! 0.444 0.462 0.486 0.487 1.038 0.784 14.81% 8.35%
0.598 0.641 0.714 0.612 10.554 0.535! 0.469 0.492 0.515 0.517 1.144 0.857 10.66% 9.80%

96 | 0.270 0.327 || 0.289
192 | 0.331 0.368 || 0.383
336 | 0.321 0.370 || 0.448
720 | 0.369 0.415 |) 0.605

0.328 0.364 0.313 0.372 0.315 0.359 0.332 0.374 0.332 0.368 1.549 0.952 657% 7.37%
0.372 0.408 0.519 0.554 0.402 0.425 0.407 0.443 0.426 0.434 3.792 1.542 11.02% 9.80%
0.397 0.421 0.722 0.684 0.414 0.437 0.400 0.447 0.477 0.479 4215 1.642 19.14% 12.11%
0.461 0.497 0.817 0.741 0492 0.513 0.412 0,469 0.453 0.490 3.656 1.619 10.44% 11.51%

2 ETTh2

ESULTS OF UNIVARIATE LONG-TERM FORECASTING

192
336 | 0.077 0.219
720 | 9.085 0.230

0.204 0.086 0.231 0.079 0.215
0.244 0.097 0.249 0.097 0.243

ETTh1

96 |.0,052..0,171 || 0.056 0.180 0.068 0.184 0.058 0.184 [0X
0.068 0.194 || 0

0,359 0.152 0318 0.193 0.366 10.16

0.079 0.215 0.071 0.206 0.193 0.377 7.14%  5,00%
0.104 0.245 0.114 0.262 0.217 0.395 4.23% 4.90%
0.119 0.270 0.107 0.257 0.202 0.381 15.38% 7.98%
0.142 0.299 0.126 0.283 0.183 0.355 32.54% 18.73%

96 | 0.115 0.262
192 | 0,148 0.308
336 | 0.152 0.319

720 | 0.198 0.360

0.279 0.134 0.289 0.135 0,283
0.329 0,166 0.325 0.176 0.330 0.

0.204 0.356 0.204 0.363
0.426 0.264 0.405 0.255

ETTh2

0.408 0.25

0.128 0.271 0.153 0.306 0.213 0.313 10.16% 3.32%
0.185 0.330 0.246 0,351 0.227 0.387 10.84% 4.05%
0.231 0.378                                               0.401 15.08% 6.18%
0.278 0.420                                    0.439 22.35% 11.11%

ae

LEARNING

Hi DEEP

1- 무단 전재, 복제, Ball, 디지털화 금지


===== PAGE 183 =====
Time Series & LSTM                     3.3 Time Series Generation : WaveNet

® Univariate vs. Multivariate : 2i Multivariate 45-0] 더 LHE7}?       컬럼 이름 | 설명

 모델 복잡도 증가 및 0+6ㅁ10100 가능성 증가                                            HUFL | 고부하시 Upper Load

 입력 차원 수 증가 > 파라미터 증가 > overfitting(noise 학습) 가능성 증가
0848의 크기가 부족하면 심각함

HULL      고부하 시 Lower Load

®@ Target OT 예측에 크게 기여하지 않는 변수들(560 길이에 따라 다름)             MUFL | 중부하시 Upper Load

@ Data Noise(sensor ㅁ0156)증가 및 추가 변동성 발생                               나 개 의
* 모델이 학습해야 할 FSS 그만큼 늘어나 오히려 예측이 HAMA 가능성

 목표 변수 포함 방식의 차이 : 13「96@}을 포함할 것인가?                               1066. | 저부하이 00606

@ Hyperparameter 세팅 및 학습 전략의 차이                                       LULL - | 저부하 Al Lower Load

@ Univariate : 구조가 단순해 학습이 용이하고 최적화도 간단
/ Multivariate : 많은 hyperparameterS 세밀하게 조율해야 St
® Seq. 1009내가 길어지면 성능이 더 나쁜 이유는?
ㅎ 불필요한 노이즈, 불필요 정보의 증가
@ 더 다양한 패턴, 더 불규칙한 노이즈를 포함, 추가 정보가 중요한 HAS 학습 방해
@ 장기 의존성 학습 한계
/ RNN, Transformer 등 모든 SAS 장기 의존성을 학습에 한계가 있음
/* 특정 모델의 YS vanishing gradient, exploding gradient 문제가 발생 확률 상승함
@ 모델 복잡도 상승으로 학습 최적화 어려움
@ 정보 중복과 모델의 집중도 저하
/* 한 시계열에 패턴이 반복되면, 중요한 특징에 집중하는 AS 방해함(중복정보)
/* 불필요한 정보와 유의미한 정보 구분에 어려움 증가(집중도 저하)

OT          변압기 오일 SS (Target)

~

Al, 복제, Si), 디지털화 금지

-182- ola



===== PAGE 184 =====
3부. Time Series & LSTM                                        3.4 LSTM AutoEncoder

Chapter 3. Time Series & Other Architectures

3.1 Time Series 개요

3.2 Time Series Analysis
3.3 TCN and Other Architectures

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.5 Time Series Classification

[5114 Encoder Decoder 기본형)
1) Encoder outputS 060006[입력으로 사용
® Stateful 사용하는 경우(상태가 유지)
 6021다내에서 i 샘플 상태는
C+S batch i 샘플의 초기 상태로 사용
® Char-RNN 참조

Many to many - 3

WL) 0 0

® RepeatVector 사용하는 BP (AEE 초기화)        Ofer 것갖- 아이누 이 시께벽을    64\600서

Sok

BHRGRESHEAS LSTM AutoEnceder

latent_dim = 2

inputs = keras.Input(shape=(timesteps, data_dim))
encoded = layers.LSTM(latent_dim) (inputs)

he

decoded
decoded

wd OV MT te be

layers .RepeatVector(timesteps) (encoded)

layers.LSTM(data_dim, return_sequences=True) (decoded)

Ho

ui DEEP LEARNING —

@한국시연구소 홍근선                     -183- 무단 전재, 복제, Ball, 디지털화 금지

0



===== PAGE 185 =====
3부. Time Series & LSTM                                       3.4 LSTM AutoEncoder

Seq2Seq (Sequence to Sequence) 모델 이라 St
ㅠㅠ 입력 AJ WAS 단일 HIE/= Encoding( hidden state & cell state )
- 인코딩 값을 디코더 초기값 hy 에 전달
- ‘return_state=True’ : 마지막
/* 단일 벡터를 출력 A/HA= Decoding
- JHA 출력을 ChE time step WHOS 전달

one to many : Decoder

many to one: Encoder

9 a    -     since     :      Sit DEEP LEARNING”

x Stacked AutoEncoder                                                AutoEncoder         eal

= AutoEncoder
* AEE 수학적으로 주성분분석(『ㅇ와 유사
 고차원 정보를 저 차원으로 압축하고,
고차원 공간으로 복원 하는 기능을,
ㅎ 스스로 최적화 (40540611560 learning)

@ 압축된 저 차원 공간을 13160 space                                          +e

ㅎ 저장된 A+ Latent VariablesO|2} st
® Encoder, Decoder layer7} 많으면 > Deep AE                   output SSG

m Stacked AE : Deep AES] 학습능력 향상이 목적                               도
@ Unsupervised 16210100으로    | 500

 고차원 정보를 효과적으로 추출/압축하기 위해 ㅅ       ~

® LabelO| 있는 경우에 마지막에 Fine-Tuning                           … 19000 .
w Sparse AE : Hidden layerS 효과적으로 학습 시키기        | |

* Hidden 1316[의 parameter 학습을 00ㅁ01
* 일부 nodeGt 활성화 되도록 유도
ID

@한국시연구소 홍근선      -184- 무단 전재, 복제, wal], 디지털화 금지

-

Minimize (x — £)?



===== PAGE 186 =====
aT  Time Series & LSTM |                                       3.4 LSTM AutoEncoder

Bs AutoEncoder 사용한 Time series Anomaly detection   2. 나 )
m [실습] Time series Anomaly detection

® https://keras.io/examples/timeseries/timeseries_ anomaly detection/

.              :                                         .            *                          AutoEncoder
Timeseries anomaly detection using an
nal      X Output         in’
Autoencoder                                                            Pes                              g
U
ㆍ                               요
Author: pavithrasv                                                                                                 |                                          é
Date created: 2020/05/31                                                                               &                                    [의
Last modified: 2020705/31                                                                               G
Description: Detect anomalies in a timeseries using an Autoencoder.                                        £                                        ZN
=                               £
c ViewinColab + €) GitHub source                                                   는                               3
&
po                                              1600
1490                                             is                 adh aha
250                                                                                                                   At!
a                                                  1200                                             is
es                           i
3 150                                            = 990         i                                                                ㅣ
 190                                고 eo       {                          .                    |
00         i                                   ~ 두
bad                                               200         {                                   ：    1 15086               ,
o                                                a         :                             _  She             100    190    200    256    300
8180     105     0130    OLS     aie        ar       02         a3       a4
Fain MAE loss                                                 test MAE loss
t
：      Yeap Nee wane 6
369 _                           ri                                                                   “S80 DEEP LEARNING”

3X Time series Anomaly detection
= UCR Anomaly Benchmark Datasets an      UCR_AnomalyDataSets.pptx 참고

h                                                  n/tim                                         Ti         ri

PO de, Wipedieatke caalieauenedine cate tata Ge

Mars Science Laboratory: A4                                                       Ground Truth Ancmaiy

200       1      ae       ㅣ
1

T                  ue

= , . Ground Truth Anomaty          다                                                 Ground Truth Anomaly
Z                                                                           i
32 ~          삐
/                           =                                                '
이바 60 Positive                                        ]
:                                                                   |
poe         7            ;            1            ;            +            +            7            i
;                                                                                                  7006
Raa                                                ‘i    Ground Truth Anomaly            ‘Ground Truth Anomaly     .
“7
i
|
oot                                                  T            7            T                         T
1                                                                                                   000:

Steep
Rate of
Increase \

@한국시연구                                 -185- 무단 전재, 복제, Wal, 디지털화 금지


===== PAGE 187 =====
3부. Time Series & LSTM                                       3.4 LSTM AutoEncoder

28 WSAE-LSTM : Wavelet + SAE + LSTM

2017.7 “A deep learning framework for financial time series using stacked autoencoders and long-short term memory”

m Over view
@ Wavelet Transform(WT) : 주파수 분할하여 noise 제거 |:
@ Stacked AutoEncoder(SAE) : 깊은 수준의 특징 학습
* LSTM : 다음날 종가 예측

> 최초로 SAES 적용, 0312의 추상적 SAS 학습

* Data: OHLC + 기술적 지표 + 거시경제변수

® 결과:
@ 6개의 시장 지수와 그에 상응하는 지수 HSS 선택
@ 예측 정확도와 수익성 향상

371

mw Wavelet Transform(WT) : 주파수 분할하여 00156 제거, (2f:JPEG2000)
® Mallat 2t12|2 : Father wavelet y(t), Mother wavelet p()= PM — oiphi), w (psi), x(pi)
+

® <(0) : 저주파 성분, pO : 고주파 성분   |                |              \
@ 분할레벨 ]에서 Fw: Mul!) = 2 10(27'-/)          ~
MW: Wyult) = 22W(27 — k)            [      X       Ss

/* j(scale parameter), k(shift parameter)                                     |      ’       X               뼈
© 신호의 재구성 : 분해된 HES sumat-H 됨                                        ———
@ x(t)= > 2970.10) 기 Yo day(s) 1 Sa aWy-ralt) + -.. + Saul)
«Father       ㄴ Mother      *      Mother             * Mother

@ 5900 =즈59140) 라하고, Dt) = T.dih(t) 라 놓으면

@ 100 =500+20+ㅁ00 +…+20)라할수있음 Lerreyz 선호  Sab ( Vart Wah)
/* 5100) : 저주파 성분 (개략적 근사), Dj(t) : 단계별 고주파 성분

® Filtering : 1-d Conv. filter       |
> 재구성된 신호= 40156제거된 신호 |

S stxyaw( 4) ax

|
JU                    0.5)
| | V \    V \}             °°                                00
||          Vv             ”                         ~05
|                           10
|                          o 7              |         5
0
372                                                                               V5
한국시연구소 홍근선                      -186- 무단 전재, 복제, etal), 디지털화 금지



===== PAGE 188 =====
= 2 WS   t.Wavelet( haar”)                           ,
spot,   la > pywt.wavedec(y, w, level=2, mode='per', axis=@)         ;

3. Time Series & LSTM
ㅣ

3.4 LSTM AutoEncoder
“4

® Haar Wavelet Transform                         x(t) = S(t) + D,(t)+D,_,(t)+---+D,(t)
@ Encoding : Decomposition                                                      t;--Haar Wavelet _
/ “haar” filterA-2, 2번 분할, mode(padding option)                             파우

i #impert pywt as pywt

®@ Decoding : Reconstruction                                                                      “         !

 Coefficients 넣어 신호를 재구성 _

1 reconstructed_signal = pywt.waverec(coeffs, ‘haar', mode='per‘, axis=@)

2 plt.plot(reconstructed_signal)

@ Coefficients 구성 : Sn,Dn,Dn-1,--,D1

w = pywt.Wavelet( ‘haar’ )                                다     | Haar    ;    /684590071
coeffs2 = pywt.wavedec(y, w, level=2, mode='per’, axis=@)       |     :    /
$2,d2,d1 = coeffs                                           i

ps(s2),ps(d2),ps(d1)

에 나 10 라

{] 56306(1308, 1)
[] Shape(13e@8, 1)
{] Shape(2615, 1)

®@ CoefficientOll thresholdS 이하의 값을 0 방향으로 > 작은 값을 더 작게 변환
> Detail 제거 ( 고주파 성분 제거 )

# Attp: //connor~jo

on. com/2016/@1 /24/using-pywavelets-to-remove-high-frequency-noise/

he lb A bt

be
[3
그
1
“

at
te
o
Est
…
fal
[nd
그
|,
때
a
>
&
S
6@
ee
6
rt
S
Ay
ay
py)
%
ee
id
3
에
i

# calculate a threshold Se, did.

sigma = mad(coeff[-level]) Fathercoeff. 기준으로 0066600계산
is     print(? ‘Coeff 02 mean : {np.mean(coeff[1}}}‘}

aL     print(#*Coeff 01 mean : {np.mean(coeff[2])}')                                  il.       t

42     uthresh = sigma * np.sqrt( 2*np.log(len(x))) * sm               d     cA AS    wesladlel te
coeff[i:] = ( pywt.threshold( i, valuesuthresh, mode=“hard” ) for i in coeff[i:] )   ake, ya  a

print(?'Tresohold value : {float(uthresh):024}')                                 4766 ~

LO Oh 1405 허

Mad: 중앙값 절대 편차
(median absolute deviation)

print(f’Coeff d2 mean : {np.mean(coeff[i])}')
print(f ‘Coeff di mean :
# reconstruct

{np.mean(coeff[2])}‘)         ‘a

return y
r_data = waveletSmooth(y)

dio} '0'이 &                                               802

sm= 2 인 경우 :

Coeff 02 mean
Coeff di mean :

Coeff 02 mean :

Tresohold value :

> -0.00024918333345430864

~9.5785744753682672-85
@. 833363
. 7282846728573883¢-85

Coeff 01 mean

2
18.8

EP LEARNING —

1k

@한국시연구소 홍근

1

- 187- 무단 전재, 복제, Ball, 디지털화 금지


===== PAGE 189 =====
3부. Time Series & LSTM                                       3.4 LSTM AutoEncoder

= Stacked AutoEncoder : extract deep features from input data
Sine ale Ja er AutoEncoder
input

® Single layer Autoencoder

# Inputz} output 이 동일하도록 S2l< latent spaced] 저장
@ Stacking AutoEncoder Training

 4개의 Single layer AES stacking

@ 1% AE 학습 후, 194 Reconstruction layer 제거

@ 15t AE Hidden layerS 2"4 Input layer 로 사용

@ 2,3,4 새에 반복 적용                                                 Reconstruction

/ Daily input data 7} 18 ~ 25일 경우
Hidden layer nodeS 10712 설정 함
¢  리어 1055 추가 설정
좋은 특징을 간추리도록 강제
 활성화되는 0006의 평균값을 지정해 1055에 추가
® Hidden 401에서

4 autoencoders

/¥ sparsity_target = 0.5                                 Input daily                                         Output deep
features                                                  features.
/ sparsity_weight = 0.01                                   =                 e   oe    e   ®
Layer                2        3        4        5
375                                                                                                                                                                SAP DEEP LEARNING |

® Encoder Sparsity loss
@ 학습을 강제하여 좋은 SAS 발견할 수 있게 유도 하기 위해
® hidden 4115에서 activationS|= 값의 확률에 대한 SRS 주고, 통제
@ KL divergence : 두 확률분포의 차이를 계산하기 위해 도입
/* 기본 적인 KL divergence=                                    P(z)
sampling! 값의 확률로 표현 Deu (PQ) = Exp [os oak

= By..p (log P(x) ~ log Q(z)

/* SlopS 극대화 하기 위해            2 (0210) = plog © + (1 ~ p) log wot   a, 우측 cuves 생성
두 개의 KL diver. 사용                         0000 ---
/* 6ㅁ00086「에서는 508「91 1055만 구함                                            — 69999 KL Diver, MSE slop 비교
최종 Loss: Loss = MSE + sparsity_weight x sparsity_loss °°) ~~ ~                           s
— ：           ~
Cost                                  「

® Sparsity loss Code
/ KL diver, 가 기대값이므로 평균값으로 계산
7 2, (sparsity_target||mean(hidden unit))                      a2

00              02               oe              06              08               19
Actual sparsity

i4    def sparsity_loss(self, h):

15        mean activation = tf.reduce mean(h, 3×15=0)

16        kl_loss = (keras.losses.KLD(self.sparsity target, mean activation) +

12               keras.losses.KLD(1 - self.sparsity_target, 1 - mean_activation))
18        return self.sparsity weight * kl loss

is ib comlageronthandson-al "Rie SEES CERNING”
@한국시연구소 홍근선          - 188 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 190 =====
3부. Time Series & LSTM

3.4 LSTM AutoEncoder

® Encoder class ( layer class )

_

i class Encoder(keras. layers. Layer):

2     def __init_ (self, h_units=18, name='encoder', sparsity_weight=ie-2, sparsity target=@.5, 12_reg=le-3

3        super().__init  - (namesname)

4        self.dense = keras.layers.Dense(units=h_units, activation= “sigmoid',

등                        kernel_regulerizerskeras. reguiarizers.12(1=12 reg))

6        self.sparsity_target = sparsity_target

7        self.sparsity_weight = sparsity_weight

8    Pe ee;

3    jdef call(self, inputs):             |

12    i    h = self.dense(inputs)            i

11    ‘    self.add_loss(self.sparsity_loss(h))}{ loss

EL

초구

14    def sparsity_loss(self, h):

5        mean_activation = tf.reduce_mean(h, axis=@) 4/3, )<-(128,3)

16        1 1055 = (keras.losses.KLD(self.sparsity_target, mean_activation) +

317              keras.losses.KLD(i - self.sparsity_target, 1 - mean_activation)}

a8        return self.sparsity weight * kl_loss
은 class Decoder(keras.layers.Layer):

® Decoder  2    def init__(self, original_dim, name=‘decoder’, 12_reg=ie-3):
2       super().__init__(namesname, **kwargs)
4        self.outputs = keras. layers Dense(units=original dim, activation='sigmoid’,
5                                                         kernel_regularizerskeras.regularizers.12(1=<12_reg))
é    ee
7    ] def call(self, inputs):     |
을    !    x= self.outputs(inputs) |
$    i    return x              |

® Single AutoEncoder class ( model class )

| class AutoEncoder(keras.Model):

2    def init__(self, original_dim, intermidiate_dim, 12_reg=ie-3, sparsity_weight=te-2, sparsity_target=@.5):
3                super().__init__()

4        self.encoder = Encoder(h_units=intermidiate dim,

5                          Sparsity_weight=sparsity_weight,
6                          sparsity_target=sparsity_target,
i                          12_reg=12_reg)

g         self.deceder = Decoder(original_dim-original_dim,

16    | def ca call(self, inputs):     i

iu    :    x= self.encoder( inputs)!

12 | x = self.decoder(x)    {

Di     return x               「

378

x! DEEP LEARN

@한국시연구소 S24        - 189 - 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 191 =====
3부. Time Series & LSTM                                       3.4 LSTM AutoEncoder

@ Stacked AutoEncoder class : stacking, training ( model class7} 아님 )
@ AutoEncoder modelS listo] 넣는다고 입출력이 연결되지 않음( Sequential model X )
@ AE modelSO| 각자 독립적으로 존재
i class StackedAutoEncoder: Modelx
2    def init__(self, layers, original_dim, intermidiate_dim, 12_reg=ie-3, sparsity_weight=le-2, sparsity_target=@.5):

5        for k in range(layers - 1): 108에넣어서 stacks

self.ae. append(AutoEncoder(intermidiate_dim, intermidiate_dim, 12_reg, sparsity_weight, sparsity_target))

@ Training : Stacked AE, SAEE 모델이 아니므로 자체로 학습 불가능
/* 첫 번째 AE model 부터 ACH Training, 한번 학습된 AEE 학습되지 않음
/* MZ AE Training input : 학습된 이전 에서 『ㄷㅁㅇ0086『만 사용 (hidden layer 출력)

36    def train_stacked_ae(self, inputs, learning_rate=@,01, n_epochs=2@, batch_size=128):
print(f‘AE_1')

4

pe

32       self.train one ae(self.ae[9], inputs, learning_rate, n_epochs, batch_size)

|        h = inputs           “oa

| 34        for i in range(1, len(self.ae)):

35          b= self.ae[i - i].encoder(h).numpy() 이전 다음 입력으로 공급
36          print(f'AE {141} ')

23
a

self.train_one_ae(self.ae[i], h, learning rate, n_epochs, batch_size)

-—           ae      "Sp BEEP LEARNING”
로                             Se 00 그 게어이개

@ Training : Single AE model (AEE 모델이므로 ㅠ10100가능 )
/ Input: single AE model, input data, training options
/@ GradientTape : training®| model.fit() 사용 하지 않음
- 82[대단위로 Sal forward path 진행,
- loss 계산
- gradient 계산 및 Optimizer 전달
을    def train_one_ae(self, model, inputs, learning rate=8.91, n_epochs=2@, batch_size=128 ):
3        optimizer = keras.optimizers.Adam(learning_rate=learning_rate)
18        num_train = inputs.shape[@]
131        n_batches = int(num_train / batch_size)
42
iB        loss_Ist = []
28        for epoch in range(n epochs):
15           total_loss = @
16           for iin range(n_ batches):
17              sample_idxs = np.random.choice(num_train, batch_size) RandomBatchsampling —
is         :     x_batch = inputs[sample_idxs, :]
19        …ㄱㄱㄱ        ——
28            iwith tf.GradientTape() as tape:               Model dissel method          ‘
2            i   x_rec = model(x_batch) Single AE Forward path _ LZ   —_                ㅣ
22              H    regularization_loss = tf.add_n(model.losses) Element-wiseadd, list of add lossO.     H
i                                                        더   *      i
23             | loss = 0.5 * 나 06006 sum(tf,square(x rec_- x batch)) + regularization 1055!
28              igrads = tape.gradient(loss, model. variables)     MSE         ‘Sparsityloss      i
26                                 loss_lst.append(loss.numpy())
ai               total_loss += loss.numpy()

-190- 무단 전재, 복제, SHI], 디지털화 금지



===== PAGE 192 =====
3부. Time Series & LSTM                                         3.4 LSTM AutoEncoder

@ SAE Object (model x) instantiation & Training
@ Input data : Open, High, Low, Close, Volume, Change
/ WaveletSmooth)S 사용하여 00156 제거한 0313 준비
@ SAE object instantiation

#SAE = StackedAutoEncoder{layers=5, original_dim=18, h_units=1@)

layers=3

original_dim=6

h_units=3                                                           :
SAE = StackedAutoEncoder(layers=layers, original_dim=original_dim, h_units=h_units) |

woe ow he

®@ Training
/* SAEQY| stacked_training_ae method 호출 > AE modelSS 순서대로 학습

|  1 SAE.train_stacked_ae(x_r_data, learning_rate=@.01, n_epochs=10,  batch_size=i28)

@ SAE output Feature 확인

16

1 outputs = SAE.ae[@].encoder(x_r_data)

2 outputs = SAE.ae[i].encoder(outputs)          08
| 3 outputs = SAE.ae[2].encoder(outputs)

4 p(outputs)                               a6

Shape: (5232, 3
Type: <class ‘tensorflow.python. framework .ops.EagerTensor'> a4
Values: [[@.75592124 @,16664584 9. 75074357]
[0.7099946 ©.216404 ©.70362747]                       az
[8.73955756 8.18398469 6.73398906]

00
0      1900 2000 3000 4000 5000

= LSTM Block ( model class )

@ Stacked LSTM : 5 layer
® 64 cells, 4 time steps

i

고

3                1002 79 sas se ee 에의
4     # ad Layers using Loop

5     model.add(keras. layers. Input(shape=inputs_shape))

6      model. add(keras. layers. LSTM(units=units, return_sequences=True))
7     for i in range(i, layers-1):

8
9

model. add(keras.layers.LSTM(units=units, return_sequences=True) )                  Dense(1)   |
model. add(keras.layers.LSTM(units=units))                              :
19       model.add{keras.layers.Dense(1)) Linearactivation                                                          |
a                                      | LSTM5(64) |
model.compile(loss=’mse°, 9ee
43                                    optimizerskeras.optimizers.Adam(learning_rate=learning_rate),                   LSTM4(64)
14          metrics=[keras.metrics .MeanAbsolutePercentagetrror(),
is #           LinearCorreLation(),                          aes
16 #          theilue)                          | 15103640 |
17             |                                     ai
18          )                                  [ LSTM2(64) :
LSTM1(64)
feature(10)x4_
382 _                                                가 이

@한국시연구소 홍근선               - 191 - 무단 전재, 복제, 4, 디지털화 금지


===== PAGE 193 =====
3부. Time Series & LSTM

3.4 LSTM AutoEncoder

들 Metric
@ MAPE( mean absolute percentage error)
@ Wat 절대 백분율 오차(편차) : Regression loss 함수로 사용
 100 * abs(y_true - y_pred) / y_true
® Linear Correlation(=Pearson Correlation soll

eet

al   Ri

MAPE =

데이터 SES x,  a 피어슨 상관계수

@ 두 변수의 자르고 표준편차의 sel 나눈 값
(=? (%-X) fer (u-¥)
® Theil’s U (=Uncertainty coefficient)

‥ 불확실성 계수 : 정규화된 상호정보량
 결합분포가 얼마나 다른지를 측정 함

Txy =

[내
WV

an a a

6.8       O44                 -O.4       6.8       그

- 상호정보량 (MI: mutual information) : 1063)
- BES (entropy) : A(x

AGI) IO
00190 = Hy) PAD

E> by om yey
Vi doe pr ail
Vy > 00?  *< Vv Sai

Theil U =

HOY)

을 Results
@ Prediction approach

@ Input datasets                                     -

Name                                                                Defini
__ Panel A, Dally Trading Data
Open/Close —_nominai daily open/close price
Price
ic 성능 비교                       분
High/Low Price _ nominal daily hi       price                                       Metric 성능 비교 , Year(4 분기 평균)
Trading volume _ Daily trading volume       ：                                                                                                                                                                    S&P 500 index
Panel B. Technical indicator
MacD          owing average conwestionica divecqerva: depiays vend jllowing                 fceand             Year            Yeari Year2 Year3 Year4 Year5 Year6 Average
.               "                    18                             :          ：                                                                                                                Panel A. MAPE
cei              Commodity channel index: helps 10 find the start and the end of a trend.                            WSAES-LSTM 0.012 0.014 0010 6.008 0.011. 0.010         001
ATR            Average true range: measures the voiatiliy 아 0006. 08000
BOLL            Bollinger Band: provides a relative definition of high and low,  which aids i in 1 rigorous                 WLSTM             0.015 0.020 0.012 0.010 0.015 0.015         0.015
pattern recognition                      :                    LSTM     0.021 0.018 0.013 0.012 0.017 0.022 0.017 __
EMAZD.... 22G8y Eponental Moving Average                         RNN 0017 0.019 _ 0.013 0.019 0.020 0.019 0.018
MAS/MAIG       5/10 day Moving Average
MIMG/MTM12 6/12 month                    helps pinpoint the end of a deciine or advance                                                                                                                                              Panel C. Theil U
ROC            Price rate of change: shows the speed at which a stock's price is changing                      WSAEs-LSTM 0.009 0.010 0.006 0.005 0.008 0006 0.007
SMI           Stochastic Momentum Index: shows where the close price is relative to the midpoint of          WLSTM          0.011 0.014 0.008 0.007 0.011 0.011        0.010
the same range.                     a                     :                     .
WVAD           Williams's Variable Accumlation/Tistrbpution: measures the buying and selling                       LSTM             0.014 0.012 0.009 0.007 0.011 0016 0.011
Pressfe                                       RNN    0.012 0.012 0.009 0.012 0.013 0.012 0.012
Panel C.                          ic Variable
rate US dollar Index

@한국시연구소

-192=

단

전재, 복제,       디지털화 금지

al,



===== PAGE 194 =====
3부. Time Series & LSTM                                       3.4 LSTM AutoEncoder
i"                            7

WSAE-LSTM 모델을 살펴보고, 간단한 Data 적용해 본다.
1S 개요
ㅎ Wavelet Transform’ 사용하여
® Decomposition, Reconstruction 과정을 확인하고,
® Coefficient Threshold7| Smoothing 27}3 가짐을 확인
® Stacked AutoEncoder CodeO|]
@ 구조적 특징과
@ 독특한 학습과정을 이해함
@ 학습된 SAES 적용하여 STMYS 0313를 생성한다.
® LSTM 모델을 만들고
ㅎ SAESS datat, target 0212로 학습을 진행하고,
@ Test dataS WSAES 통과시켜 LSTMO|l 넣어 prediction 수행한다.
ㅎ 결과를 시각화 하여 확인한다.

=

% [실습 2] WSAE-LSTM
a 목적:
a

>

2019.12 “Unsupervised Pre-training of a Deep LSTM-based Stacked Autoencoder for
Multivariate Time Series Forecasting Problems”

들 Over view

® LSTM SAE : LSTM layerS 사용한 SAE 제안

© Deep LSTM2| 초기값 문제를 해결하고자 함
® LSTM SAE& Deep LSTM2| 초기값을 사용
ㅎ Unsupervised learning? = 효율 향상

* Deep LSTMS| 성능 향상, 빠른 수렴이 가능

© 동일 저자 선행 논문의 DLSTM 개선
@ 2018.9,” Time series forecasting of petroleum production using deep LSTM recurrent networks”
® DLSTM results

Forecasting model RMSE  RMSPE
ARIMA                0.310 4.705
Best results of DLSTM with static scenario.                                             NEA 128!   |           ~         4.221
DLSTM(static)                  0.209  2.995
No. of layer No. of hidden units No.of Epochs lag RMSE  RMSPE       DLSTM(dynamic)      0.219     3.124
1               141                     953             5 0234  3.337        Single-RNN            0.233 3.290
2               [4.2]                   787      0.227     3.253        Multi-RNN            0.219     3.129
3               [54,2]                 800             5 0209 2.995        DGRU                  0.222 3.175
(i                             ~                         |                                      - DEEP LEARNING
@한국시연구소 홍근                         - 193 - 무단 전재, 복제, Bll, 디지털화 금지


===== PAGE 195 =====
3부. Time Series & LSTM                                         3.4 LSTM AutoEncoder

을 Architecture, Training process            글 AutoEncoder block        i
many to many 3)                 |

® LSTM AE block
® LSTM SAE Training

® Phase1 : Greedy 0 pre-training                                              -
1, 첫 번째 LSTM-AE block 훈련, \저장
2. 두 번째 LSTM-AE block 훈련                       ea           Bing
- 첫 번째 encoderS 사용하여 244 encoding          |                      |
- 이를 사용, 두 번째 LSTM-AE BSS 훈련                 —
- 첫번째 encoder] 출력이 아니라 input layer2] 입력을 재구성 하도록 훈련

(새로운 인코더가 원래 입력의 특징을 학습 )   바이저 자 Bee bee SEE
3. 세 번째 LSEM-AE block 훈련 : 두 번째와 동일   %* SAE UPA Aver PG 5h 향시

rary

® Phase2 : Fine-tuning
/ output layer 추가
/* 13[061값으로 x(t+1)AHS
(ABE 22 2B AB)  |,-------~
/ Trainin                        |      :
°                 i                          J
|                                                            고: 2nd Hidden layer) (2nd Hidden layer )
ㅣ                                                      |                      |
1, Go                            (ist Hidden layer) (ist Hidden layer)
|                      |
+ (oon tave)         (ey =
Figure 4. The greedy layer-wise pre-training of LSTM-SAE model,
a       .      .             i DEEP LEANN

@ Results
® Rental bikes 0218에서 상당히 좋음 그

xd                         04                  20 | 146           52,062         32,468         12.088

1
DLSTM       2                ‘ol             0.3          25 | 219      49.811     31.524     12.183
eB            느                                                        LSTM-SAE     1                   3                 OL             30 | 219       49.389      32.192       13.878
(CE data= 별로 )                                                                                Ee                                                      3s
LSTM-SAE     P                                     ol             30 173         46.927      30.041       11.646
Hourly totat rental bikes prediction from 27/12/2032 to 31/22/2022
[~                                                                                                     i

거에 penitent eI)
mee pesictionsi STH SAS

* 모델 수렴 속도 비교

@ DLSTM 대비 060내가 클수록 효과가 있음

ee        내 00
1          2                  414                255
1                  500                355
1                  123                244
10          2                  127                463
3                  1182               197
ref code : httos://cithub.com/DeenWolf90 ，, Keras (2.1.5)
se eee een enor                                    —— ee   pee   Ee
388                           SX DEEP LEARNING

@한국시연구소 홍근선                     - 194 - 무단 전재, 복제, SH], 디지털화 금지



===== PAGE 196 =====
3부.

Time Series & LSTM

we 주파수 영역 분석, Frequency Domain Analysis

3.4 LSTM AutoEncoder

| AutoEncor

* 데이터의 주기성을 주파수 domaine= 변환, 주파수의 합으로 모델링
주로 사용되는 용어들
@ 신호의 주파수 성분이 시간에 따라 어떻게 변하는지 시각화
/* Time-Frequency Map, Time-Frequency Spectrum
@ Spectrum : 주파수 성분과 그 크기( Amplitude, Phase 포함 )
/@ Power Spectrum : 주파수별 에너지 분포, 단위 시간당 에너지 (진폭의 제곱 )
@ Scalogram : Wavelet 11305[0107으로 주파수 SMS 시각화한 것 _
 고주파 성분은 짧은 시간 간격으로, 저주파 성분은 긴 시간 간격으로 분석되어
국소적이고 비정상적인 변화 감지에 우수
~ Wavelet Power Spectrum : Wavelet coefficient2| 제곱을 시각화
/@ Time-Scale Representation : Wavelet coefficient 주파수가 아니므로, 56816개념이 적용된 것임
+ Wavelet Analysis Results : Wavelet Transform’. = 분석하는 일반적 표현
® Spectrogram : Short-Time Fourier Transform’ = 주파수 정보를 시각화
@ 각 시간 구간별 주파수 성분의 세기
/ 시간 해상도와 주파수 해상도 간 트레이드오프
® Coherence vs. Wavelet Coherence
/@ Coherence : 전체 주파수에 대한 정적 상관성(정적)
/ Wavelet Coherence : 두 신호의 주파수 성분의 상관성의 변화(동적)
OPO

oceans

390

3.4 LSTM AutoEncoder : V

mw 주파수영역 분석 방법 : 자세한 설명은 하단 40!참조

이

© Fourier transform : 데이터의 주기성을 주파수 0010811으로 변환, 주파수의 합으로 모델링
© 1년주기 0886                           홍역 발생 추이              |
@ 변화에 둔감

20000

9 5000 10006
1                          1

| |

06400 10098 ㆍ 20008  36+08

r                                          r                                                                            ;
19306 1935 1940 1945 1960 1965 0 1960 1965                o

einer

® Coherence(V#4) : 신호간의 상관관계를 의미, UFEl (stationary:A4}) 특징을 표현
@ 변화 분석에는 부적절, 일관성의 변화 분석 가능

https:     iki      ra/wiki          i

© Wavelet transform : 여러 scale2| 0313에서 주파수 정보를 추출, 변화에 민감한 분석 가능

apy

‘        -
|       -_        8
ry        é
|   xX   © 이
a. a  해제

a       2       4

nl 300 DEEP LEARNING”



===== PAGE 197 =====
3부. Time Series & LSTM                                        3.4 LSTM AutoEncoder

re

® Wavelet transform : 여러 scale2| 0318에서 주파수 ASS 추출, 변화에 민감한 분석 가능

Signal 고                                 Frequency Sp        Signal 1
i 이                                                              1
®                                   후   >   2   *   =   od       =   2
Frequency [Hz]              8
.            Frequency Spectrum Signal? _____  ”
ied                                  emis     4      A      1             j
3  Prt                                                      ane        ;          i         Ht                    i
를 ee.                                    | Et     | |      1      i                                                   —
he                                 i     t   칩             nh                            fi
i  이                                  er Le el 허니 0.                 Time

이시이] Wavelet Analysis

|      Ai 2

a 배

99000 yg, BE 간시 ;

h   VET Ger

% [실습 3] Scalogram’S 사용한 11076 56065 Classification
ㅎ 목적 :시계열을 2차원 주파수영역으로 바꾸고 분류모델을 적용해 보자
ge 실습 개요
® Data set
rchive.i i      +activitytr itiontusing+
@ ADE ZO 움직임 감지 센서정보를 사용 사용자의 6가지 동작을 분류
@ Scalogram
® Continuous Wavelet Transformation 사용하여 시계열을 주파수 영역 2차원 AHS 변환
 9종류의 MA 시계열을 9장의 Scalograme= 변환                 = bs     yours   ae ad
@ CNN 모델을 만들고                             qe? TH               s
2  ScalogramS 입력으로, 6가지 SAS targetoe 학습

oe 4-4                                       0010
60.005 +
0.005 +                                      a
16                            40.005 +-
40.010 +
~0.005

0           a          50          75         100 325

@한국시연구소 S24                       -196- 무단 전재, 복제, tall, 디지털화 금지



===== PAGE 198 =====
3.4 LSTM AutoEncoder

34. Time Series & LSTM

© Scalogram 생성
3 def create_cwt_images(X, n_scales, rescale_size, wavelet_name = "morl"):
4      n_samples = X.shape[@]
5      n_signals = X.shape[2]
6     # range of scales from 1 te n_scales
7     scales = np.arange(1, n_scales + 1)
8      # pre allocate array
9      X_cwt = np.ndarray(shape=(n_samples, rescale_size, rescale_size, n_signals), dtype = ‘float32’)
10     for sample in range(n_samples):
il          if sample % 500 == 0:
12            print(sample)
13        for signal in range(n_signals):
14           serie = X{sample, :, signal]
15            # continuous wavelet transform
16           coeffs, freqs = pywt.cwt(serie, scales, wavelet_name})
317            # resize the 20 606 coeffs
18           rescale_coeffs = resize(coeffs, ‘rescale_size, rescale_size), mode = '‘constant’)
19            X_cewt{sample,:,:,Ssignal] = rescale_coeffs
28      return X_ewt

a © © F fe mR mo

Signabtindy gyre y

나기 오시오

Signaktiody ayre x

® CNN model

i n_scales = rescale_size = 64

2 X_train_cwt =

3 ps(X_train_cwt,"X_train_cwt")

create_cwt_images(X_train[:2048], n_scales, rescale_size)
#(2048, 64, 64, 9)

def

build_cnn_model(input_shape):
model =

Sequential()

에 5 년 00 기 mu BWN 허그

에 허그

model. add (Input { shape=input_shape) )
model.add(Conv2D(32, 5, activation='relu‘, padding
model. add (MaxPooling2D(})
model.add({Conv2D(64, 5, activation=
model. add(MaxPooling2D() )
model.add(Flatten())
model.add(keras. Layers.Dropout(@.4) )
model.add(Dense(6, activation = '‘softmax'))
return model

‘relu', padding

‘same'))

‘same'))

a 실습과제

Val Accuray. 0.954

308

09           남방  서애
® RNNGSS 적용해 보자           8
 기본 모델로 실험하고,                  때     i
모델을 개선하여 ASS 높이자 a! /(
ae   HH                       se
o24-y        ere          ee ~
[1       5       39      6

394

@한국시연구소

무단 저지

전

&

홍근
=ㄴㄴㄴ

재, 복제, Sl, 디지털화 금지


===== PAGE 199 =====
Time Series & LSTM                          3.5 Time Series Classification :

Chapter 3. Time Series & Other Architectures

3.1 Time Series 개요

3.2 Time Series Analysis

3.3 TCN and Other Architectures

3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
3.5 Time Series Classification

&

%€ Connectionist Temporal Classification

2006, “Connectionist Temporal Classification: Labelling Unsegmented Sequence Data with Recurrent Neural Networks”

m 음성인식 학습의 어려움              The pe
* 문자와 음성의 대응이 어려움                      오대 도
@ 대응 자체가 정확하지 않음(정확도가 떨어짐)
- 251005단위로 나누어 labelS 달게 됨
@ 시간축에서 대응되는 label 0218생성에 비용이 높음

(un-segment data > segment data)          " 이 ㅣ : ! " : ‘

@ 시간 변화 큼(사람/상황에 따라)          | , | 으으,
© 유사한 0856가 많음                  g0000000 848

@ 필기체 인식                 666666666 6

@ 단어(이미지) 인식

@ 비디오 1366109                     Reet | 기 | | |
> 입력과 출력의 시퀸스 길이가 일치 하지 않는 문제들 |" " ㅎ | | € € 1 6 ㅇ

RNN model 학습이 어려움            68606 제이 개
 입력(음성)과 출력(단어/음소)간 alignment BH 없이, ye y

학습할 수 있는 모델 필요            ode

(= Temporal Classification Model )        6 8 8

@한국시연구소 홍근선



===== PAGE 200 =====
3부. Time Series & LSTM                         3.5 Time Series Classification : CTC

m Unsegment Data : 라벨 순서만 있고, 클래스의 위치는 모르는 시퀸스 데이터
® Unsegment Data® sequence 102[0100에서 일반적
@® HMM(Hidden Markova Models)2| 한계
@ 다양한 사전분석 및 가정들이 요구됨, HMM2 생성모델임
© RNNQ| 한계 : Pre-segmented 0312필요, Post-processing 필요
= Connectionist Temporal Classification(CTC): Temporal classificationS 위한 RNN 모델
 Output : Input sequenced] 대한 label sequences®] 확률 P(L|x)2 모델링
® Objective function 정답 label] 대한 SES 최대화하는 방향으로 유도
® Temporal classification : Unsegmented data sequenceQ| labelingsH= 것
® Framewise classification : input sequenceOl 대한 frame 별 독립 labelingsH= 것

: Waveform

—

>

label probability

—

~

. 3.5 Time Series Class

m CTC: unsegment data7} 사용되는 = sequence classificationOl] 적용 가능
* ABA 출력을 가지는 어떤 모델의 마지막에 CTC layers 추가하여 사용함

© Label + 1(6:013010)개의 확률 벡터를 <1<입력으로           내 tc |
® LabelZ} LabelZt9] transition 규칙                   Bi i aii i
@ self-loop : 자신을 반복(입력560.길이에 따라 반복 제한)     이기 이 이 이이 이 이.
® left-to-right : labelO| 순방향으로 하나씩 전이        0 7 | rT | ij | | 1
@ Blank : blank > non-blank, non-blank > blank 전이    tin ' i 4 oe
® Paths         -|0+0+0/ 0/alololeal ie te eee e¢e @€ ee
@ 4M: ‘hello-~   110 이어 해 | ㅣ | we
@ AEH: ---hello’      |    ;         fof0 oo 00 00 6 8
* 식으로 표현하면   히히 이후 | lele Mie WMI « € c
exazaege — | |2/O/O/a/e/0/0]) 5°      a       J
qr       _           3    %
0"  -|O|O}OPOFOLO | 0 | 0 | |   CTC layer   |
20013) = 11121,                :
® Ulabel 560.)의 확률은  [해 호 이 = QO be         Festive )
villa) =    20페- 010|1@0100ㅇ010         <=
eB     TO.        700 = Laes-1 POX)
@ s:bink Har | |으의의의의의의으     000겨      -
/* B(bheel-lo-)=hello @0101010910 © OO         oe nextel
2-0:1이나올수있는 | |OlO|OlO|OlOlolo         =
든 경로의 집합   -|O/O/O|O|O|O+0+0 ||        a
tl 2 8 4 8 6 +7    is        “SRE DEEP CEARNING |

cc
단 전재, 복제, 24, 디지털화 금지

@
re)
4a
r


===== PAGE 201 =====
3부. Time Series & LSTM                          3.5 Time Series Classification : CTC

Bw 경로상의 모든 상태에 대한 확률 계산
® Forward Computation : <(5)
@ a3(s=4="e") = 323 의 전방 확률(4번째 상태)
@ Uj 개의경로 : he’, ’hhe’, ’h-e’, hee’
@ a3(4) = p(' — he'|x) + pChhe'|x) + p( )+pC )
= yl yhye + YaYae +
a,(s) = xeNT BCe4)=l1:s liter Vee , 갑의 합으로
@ 연산이 너무 많아 > 반복적인 동일 연산에
07081010ㅁ0『091「800011009적용(이전 연산 값을 재사용)
a3(4) = {02(2) + @2(3) + a2 (4)}y2
@ 상태의 연결 규칙은 두 가지, 두 가지 case 일반화 시키면

a,(s) =            {ar-1(s) + ar1(s— DY          if l; = b or l,_, = U,(case1)
{050 + my — 1) tap —D)yp 이 Perm ewleaenz)

= {l, blank}

@ Backward Computation : B;,(s)
@ B.(9) = pC — —o'|x) + p(‘— 00|x) + p(' - 0 —" |x)
= 275 27 78 +75 22 vot 75327
@ 일반화 하면                                                                         °

B,(s) =   Dents Bry7)=ls,)1) Tt  =),                                =

tr

®@ Dynamic ProgrammingS 적용하고 64561, case2= 정리하면

«|Ol Oto |«

{Br-1(s) + Br-s(s + D} yp,           if U, = bor U,,, = U,(case1)
B (s) _                                                 Ss         S+2
‘    (Br-a(s) + Br-s(s+1)+Br1(s+2)}yy,, — otherwise(case2)

a                      - (efolo/e/elelole
® Complete Path Calculation :   Ss
ey 가 별   wo                  " 이아티0 에 후 레아
- p('— hel — lo'|x) + p(' — hhel — 1o'|x) + p(‘hhhel —lo'|x) _ bt at el hal
= ans                            . 이이이익이이01@
=                                   -|10|0191010101010
ys(2) =쓰모의                        「'19|9|하하이9|9|1@
‘                      -[e/e/elerefelele
'|elelele/eferale
-[e/e/ele|eorole
- Elelelelolelo}o
“191618 18/2/9978)
@한국시연구소 홍근선          - 200 - Sat 전재, 복제, 44, 디지털화 금지



===== PAGE 202 =====
3부. Time Series & LSTM

_ 3.5 Time Series Classification                  ia
@ Likelihood Computation                       - | O+O. @|ele @|1@01@|!
@ p(lix): 입력 seq. ×에 대해 출력 seq. ! 이 나올 확률(우도)을 최대로! , | OlCn@ ㅎㅇㅎㅇ oO
/* Seq. x, :의 길이가 다르므로, 직접 1056계산 불가                  ~ -
* ICAL U'(blank7} 포함된 560.)에서 우도를 계산해야 함        1 e O ©|0/ 0/06
@ (에서 우도 405) = 732) +153) +r) +136) t736)  * |O_ CJO/O/O}O/O ©
일반화 하면4(0) = 7013) = PL KOKO yc OB —* |OLO OTOL O10 10 10
%          %  .|010100901010 0
, 10: 에서 나올 수 있는 '          lelelelotetelele
@ Gradient Computation
@ (6) = plllx)S 최대로 하는 OB 찾아야 함              ' 3 5 5 > 3 = = 5
@ 계산의 편의성을 위해 Ｌ00우도를 편미분 하여 6를 수정함             ：                               -
@ [에서 《번째 음소(9)로 108(0) 편미분하여 gradients 구하면    2 10/0 | 0/0) O| OOO
-|0/0/0/0/@/|0/0-0
alog(p(l|x)) 1 02030)                     1 2 8 tf 6 6 0 tB
ay, 70120 ay                   가프 onl etal ae
ap(I\x                                   130 Oe
정리하면 ,   oe =  a Ysetab(nk) %(S) Br(s)              ： ie alele
®@ 예를 들어 seen —                               10 < 0 1@
L(ts) = p (“hello"|x) = as) pal)  pas 05 )  4 28 BsO 이고,        ㆍ 010 0
      "      버          °)/@[@fofe
편미분하면 CHER) _ 4 fas 6600 +0+as(0 850) ㆍ216191910|.
401              ei      가"    si ee        :    : :     4 6 6 t7 8

mw Decoding
® Best Path Decoding : 시간축에서 가장 SHE 0| 높은 SAO] 레이블의 seq. S 출력, “-he-ll-o”

® Prefix Decoding : best childrenAE4, 반복
ㅎ parent 23(0.7) = children} $t(0.1+0.5+0.1)

@ Beam Search : 2! time 5160에서 Beam 5120만큼의 후보를 선택
T=1            T=2 ©                   … 626

)                '               266
® CTC Beam Search : 각 time 5160에서 중복 S429 blank 제거 + path 통합기능 추가(좀더 복

  - 대타 L LEAR  ING ©

무단 전재, 복제, S4l|, 디지털화 금지

ir a

Oot AIS=

b
나
rH
Nv
=


===== PAGE 203 =====
3부. Time Series & LSTM

3.5 Time Series Classification

x CTE

a cTICsz2

@ Deep Speech : 대표적인 Speech Recognition Model
@ CRNN : 대표적인 OCR Model

“America”

Connectionist Temporal
Classification output

[ CRNN Model 구조 ]                               [ Deep Speech 구조 ]
“state”             a
Transcription      t       |          ((@00000001."
나이 |. ESET Tete        ae                  (60000000
Deep                     eeeeeeee    Re
5       에
배가                                LSTM                                                GRU
Layers                      Batch   feeeee¢ee 8)
=     6000000의
sequence
t                 é                                                  1D or 2D
Convolutional                                             ‘
<         feature maps   Pdi
:                                     (606@000000|
Layers
Convolutional                                    2
feature maps
Input image

: Speech Recognition , OCR(Optical Character Recognition)

16 |
]

@ CAPTCHA 이미지를 읽어

8  SCR Cptical C Character Recognition) Model
: CTCS 사용한 OCR 모델을 통해 (1( HH 방식을

문자열로 바꾸는 scr)

@ Input data : CAPTCHA

ㅎㅎ 200x50 이미지와 5자의 label
ㅎ 이미지 file nameO| label?!

® CRNN 구조

® Input images Conv. Layer2} RNN layerS 거쳐서
* 두 개의 Conv. Layer
/* 두 개의 Bidirectional LSTM Layer
® CTC LayerS 통해 Ｌ055값을 계산
/* keras.backend.ctc_batch_cost(y_true, y_pred, input_length, label_length )사용

* CAPTCHA: (Completely Automated Public Turing test to tell Computers and Humans Apart)

2fxgd

이해한다.

@& wey ah ee

404

로

> < Ok

개

@한국시연구소

- 202 -

무단 전재, 복제, 빌

Pl,  디지 털화 금지



===== PAGE 204 =====
3부. Time Series & LST

3.5 Time Series Classification : CTC

o               s            =

eS 구조
© Training
®@ CTC layerOJA] 계산된 loss 사용
@ Model.compile( )에서 1055지정하지 않음
@ Inference
® Training=! 모델의 중간 S44 (Dense_21)S
CTC decoder= 넣어 출력 |36히얻음

@ Loss 설정 방법
ㅎ 41008!에서 지정
/* model.add_loss (loss)
@ Layer 지정
/* self.add_loss (loss)

docs LPR

= “|

Training                                         Inference

CTCLoss +

CIC Laver(CTC loss)

14        ah.
| 60, 21) Fy

| 650, 64x2)

| BHISTM5(64) |
(50. 128x2)

| _ BHISTM(128) |
i

|   Dense(50,64)   |
i

| Reshape(S0,768) |
160, 12, 64)

| Conv2D(64), Max_pool |
(100, 25, 32)

| Conv2DG2), Max_pool |
t

i
i
i
|
|
i
i
|
i
!
'
'
i
;
|
1
t
t
i
'
'
'
|
i
|
'
'
t
|

LS

© Dataset 준비
1) KaggleqlA 직접 다운로드
2) 저장된 10106확인, 압축이

from : https://www.kagg/e.com/fournierp/captcha-version-2-images
뜨   i=
풀렸는지 확인 필요!

1 import pathlib
4

data_dir = pathlib.Path(data_dir)
data_dir

3 95

dataset_url = "https://github.com/AakashKumarNain/CaptchaCracker/raw/master/captcha_images_v2.zip"
data_dir = tf. keras.utils.get_file(origin=dataset_url,
fname='captcha_images v2‘,

untar=False)

은 #8 check data files
2. 1016 {data_dir}

ere es

® FolderO|A] image file 이름의 list 얻고, 이름에서 label] lists 얻음

20-06-25 오후 92:36           8,569 23mdg.png
1020-06-25 오후 02:36           8,664 23n88. png
1020-06-25 오후 02:36           8,797 24300.002

20-@6-25  오후 0236           용 748 2440? nos

i # Get List of images & Labels
2 images =
3

sorted(list(map(str, list(data_dir.glob("*.png")})))

4 characters = set(char for label in labels for char in label)

@ File 08내에서 앞부분 떼어내고, 뒷부분(.0ㅁ9)떼어내고
@ Label2| char. SetS 구하고, label 2/CH 길이 확인

Number of images found: 1040
Number of labels found: 1048
Number of unique characters: 19

_ 406           Max. Char. Length:

Characters present: {‘f', 'b', "6", 'm', '8', 'y', "gi, 매기, "34, 'x', 2, @, tpt, tet, tw, tet, 5%, 4}

5
@한국시연구소 홍근선

- 203 -

무단 전재, 복제, Lal), 디지털화 금지


===== PAGE 205 =====
3부. Time Series & LSTM                           3.5 Time Series Classification : CTC

® Dataset Preprocessing
@ Char <-> Index

char_to_num = layers.experimental.preprocessing.StringLookup(
vocabulary=list(characters), mask_token=None

3
4
5 )

6 # Mapping integers to original characters

? num_to_char = layers.experimenteal.preprocessing.StringLookup(

8      vocabulary=char_to_num.get_vocabulery(), mask_token=None, invert=True
2

)

@ Split : Train, Validation dataset w/ shuffling

def split_data(images, labels, train_size=@.9):
size = len(images)
indices = np.arange(size)
np.random.shuffle(indices) #for shuffling

train_samples = int(size * train_size)

x_train, y_train = images[indices[:train_samples]], labels[indices[:train_samples]]
x_valid, y_valid = images[indices[train_samples:]], labels[indices[train_samples:]]
return x_train, x_valid, y_train, y_valid

ai OV ge Wo NS

w ow

Pe
&

rey
ey

x_train, x_valid, y_train, y_valid = split_data(np.array(images), np.array(labels))

@ Check Contents   pst(x_train) # (936,)
print(x_train[@:2]) # ['captcha_images_v2/scm46.png’,..]
print(y_train[@:2]) | 86046) ‘25m6p',...]

/ NdarrayOl string 저장

A

@ Image Read & Shape Convert: (50,200,1)>(200,50,1), Label convert: Char. > Index

1 def encode_single_sample(img_path, label):

2      # Read image, type: EagerTensor

2      img = tf.io.read file(img_path)

4      # to Decode (& to gray)->(50,260,1)

§      img = tf.io.decode png(img, channels=1)

6      # to float32 in 10, 1] range, (5@,20@,1)

7      img = tf.image.convert_image dtype(img, tf.float32)

8      # Transpose the image, (200,50,1)=(bs, timestep, feature,1)
9      img = tf.transpese{img, perm=(1,_9,_2])

310      # Map the characters in Label to numbers

44      label = char to _num(tf.strings.unicode_split(label, input_encoding="UTF-8"))
12      return {“image”: img, “label": label}

14 encoded = encode_single_sample(x_train[¢],y_train[®])
15 pst(encoded[”image”])

16 p(encoded[“label"])

317 plt.imshow(encoded[ "image" ])

[] Shape(2ee, 50, 1), <class ‘tensorflow. python. framework.ops.EagerTensor’ >
Shape: (5,)

Type: <class ‘tensorflow.python.framework.ops.EagerTensor' >

Values: [12 16 19 6 9]

“+ RNN data shape : (batch_size, timesteps, features)

@한국시연구소 홍근선                    -204- 무단 전재, 복제, Sl), 디지털화 금지



===== PAGE 206 =====
3부. Time Series & LSTM                           3.5 Time Series Classification : CTC

@ Create Dataset Generator for input pipeline

i train_dataset = tf.data.Dataset.from_tensor_slices((x_train, y_train))
2 train_dataset = (

3      train_dataset .map(

4

6

86 )

® Visualize Dataset

1 _, ax = plt.subplots(4, 4, figsize=(10, 5))

2 for batch in train_dataset.take(i):

3      images = batch[{“image"]

aA      labels = batch["label"]

5      for i in range(16):

6          img = (images[i] * 255).numpy().astype("uint8")

7          label = tf.strings.reduce_join(num_to_char(labels[i]))\
8                                         -numpy().decede({"utf-8")
9          ax[i // 4, i % 4].imshow(img[:, :, 0] .7, cmap=“gray”)
10        ax[i // 4, i % 4].set_title(label)       mol    6
1i          axfi // 4, i % 4]. axis("off")
12 plt.show()

® Define CTC Layer

1 ## Compute the training-time loss and add it to “loss”
2 class CiCLayer(layers.Layer):
3       def init__(self, name=None):
4           super().__init__(name=name)
5           self.loss_fn = keras.backend.ctc batch cost_
6       def call(self, y_true, y_pred):
7          batch_len = tf.cast(tf.shape(y true)[0], dtype="inte4") #bs<-{bs,5}
8         input_length = tf.cast(tf.shape(y pred){1], 아06="10664")#50<-(65,50.21)
9           label_length = tf.cast(tf.shape(y true)[1], dtype="int64")#5<-(bs,5)
16          input_length = input_length * tf.ones(shape=(batch_len, 1), dtype="int64")#(bs,1):[[50]...]
131          label_length = label_length * tf.ones(shape=(batch_len, 1), dtype="int64")#(bs,1):[[5]...]
12           loss = self.loss fn(y true, y pred,    input length, label length)
13                               (bs,5) ,(bs,56,21),(bs,1):[[58]..],{bs,1):[[5]--]
14           s¢lf.add loss(loss)
15       re  ore  7 dummy valde (ouonet  ( 0¢¢   MA  -
a ㅣ
17 for batch in train dataset.take(1):    es
1g      _label = batch[ "label ][:2]      #(2,5)=(bs,targets)
19      _y = tf.random.uniform( (2,50,21}))}#(es,timesteps, featues)
26       output = CTCLayer(name="ctc_loss“)(_label, _y)
21       p(output, ‘output’ )

Shape:(2, 50, 21)

Type: <class ‘tensorflow.python.framework.ops.EagerTensor ' >

Values: [[[@.5649483 0.4640832 ©.9419186 ... @.8970927 @.16261174 6.5842545 ]
[@.34@69455 9.743611   0.5902029 ... 8.7769792 @.17329288 @.24586676]
[0.23380935 @.06910626 @.33749294 ... @.54426897 @.3377334 @.45563245]

ee

"410

|         000 4A
@한국시연구소 홍근선      -205- 무단 전재, 복제, Bl], 디지털화 금지



===== PAGE 207 =====
3부. Time Series & LSTM

3.5 Time Series Classification : CTC

@ Build Training Model

1 def build_model():

2 # Inputs to the model eee1
3    ‘input_img = layers.Input(shape=(20¢@, 5@, 1),name=“image", dtype="float32")     }
4          labels = layers. Input(shape=(max_length,), name="label", dtype="float32") _ _  :
=    Hd Conv. ~-> MaxPool ~> Conv. ~-> MaxPool

6     ix = layers.Conv2D(32, (3,3),activation="relu",kernel_initializer="he_normal",

=                 padding="same", name="Convi" )(input_img)

g    x = layers.MaxPooling2D((2, 2), name="pooll")(x) #(18@, 25,32)

)     x = layers.Conv2D(64, (3,3), activation="relu",kernel_initializer="he_normal”,

310                  padding=“same", name="Conv2")(x)

it     x = layers.MaxPooling2D((2, 2), name="pool2")(x) #(56,12,64)

12     # Reshape(5@,768) -> Conv.(5@,64) ~> Dropout

13     new_shape = ((img_width // 4), (img_height // 4) * 64) #(58,12*64)

34     x = layers.Reshape(target_shape=new_shape, name="reshape")(x)

15      > layers.Dense(64, activation="relu", name="densel”)(x)#(58, 64)

316       = layers. Dropout (@. 2Od

17    # BL-RNN(128) -> Bi-RNN(64)      —~——_——eS—=—"—"
18        = layers .Bidirectional(layers.LSTM(128, return_sequences=True, dropout=0. 25))(x)
19       = layers.Bidirectional(layers.LSTM(64, return_sequences=True, dropout=6.25))(x) |
20      Output Layer # (5@,21) <- (5@,64x2)                                  ‘
21         = layers .Dense(len{char_to_num.get_vocabulary())+1,                         :
22      a... a¢tivation="      nname="densgee ) (x)              scutes
2       고 Add Cte “Layer for calculating CTC loss at each step                         |
24    bel pte loss" ) (labels, x) -add_loss()                  !
25 Define the moder eee      “         수
26    :00061 =  keras.models.Model(inputs=[input_img, labels],outputs=output,name="ocr") >
2?     ‘model. compile(optimizer=' Adal  )                                 ~       ;
28    ‘return model    라오 F--CT Cnet. ork    _    -Loce.apyy 시.

All

yy DEEP LEARNING”

2

[ Training Model ]                                                         [GNone. 200. 50.1]                     input. | [None 5)]
| me 006      [@vone, 200, 50.1)}    나 Fat | lions, 5)1
Layer (type)                Output Shape       Param #
4                                  =        :                                            (None, 200, $0, 1)                      input.
image (InputLayer)           [(Hone, 200, 56, 1)] @                | cane Conyv2D =  Tey on  [tom cCTCLaya  ors
Convi. (Conv2D)             (Hone, 208, 50, 32) 320
<               f     4         y                   ge    sad         (None, 100, 25, 32)
00011 (HaxPooling2D)        (None, 100, 25, 32) @
69002 (Conv2d)             (None, 108, 25, 64) 18496                   -      20006 | (Nome, 100, 25, 32)
스타즈 Sema   output | (34006. 100, 25. 64)
00012 (MaxPool ing2))         (Hone, 50, 12, 64) @                              i                       .
Fi                                                    a                                                           벽           19434 | (Nome, 100, 25, 64)
reshape (Reshape)           (None, 50, 768)     8              pool 2: MaxPooling?D  재개 | (tone, $0, 12.64)
densel (Dense)             (None, 50, 54)     49216                          |
wits      Be            input:     (None, $0, 12,64)
reshape: Reshape      -          ~
dropout _1 (Dropout)          (None, 50, 64)     @                            Mein ina Meccano
bidirectional_2 (Bidirectional) (None, 50, 256)    197632                   Dense | 파머 | Clone, 50. 768)
ene: Dene    output | (None, 50. 64)
bidirectional 3 (Bidirectional) (None, 50, 128)    164352
x           개                                                             1434   (None, 50, 64)
label (Laputiayer)             [(None, 5)]         a                     dropout_i: Drepout  catgut: | (Nous. 50, 62)
dense2 (Dense)             (None, 58, 21}     2709
~      cay, | 000 | O¥oue, 0.64) |
back      1 290 2):        al (LSM) [ 아사 | tone 30-3567 |
ctc_loss (€7CLayer)         (Hone, 50, 21)     6                                      -     —
|         시      가 ] input: | 여006. 50.250) |
Total params: 432,725                                                                      [ output: | vone, 50, 128) |
Trainable params: 432,725
Non-trainable params: 0                                                 :
| denve2: Dense  oa   sot |                                         11

@한국시연구소 홍근선

-206- 무단 전재, 복제, Si, 디지털화 금지



===== PAGE 208 =====
3부. Time Series & LSTM                           3.5 Time Series Classification : CTC

@ Training

1 %*étime
2 epochs = 100
3 early_stopping_patience = 10
4 # Add early stopping
5 early_stopping = keras.callbacks.EarlyStopping(
6    monitor="val_loss", patience=early stopping patience, restore_best_weights=True)
8 # Train the model
3 history = model. fit(train_dataset,validation_data=validation_dataset,
19                                        epochs=epochs, callbacks=[early_stopping])
Epoch 98/100
59/59 [=====s=s==ss=s==         =] - 25 28ms/step - loss: @.0389 - val_loss: 0.0083
Epoch 99/120
59/59 [                      ] - 2s 28ms/step - loss: 8.0388 - val_loss: 0.0075
Epoch 100/160
80058 |==      i iii) = 26 207 | TET
Wall time; 2min 56s                                                          ~~ yal_loss
10:                                개 train loss
1 4
1071              aA Cr acs 000
10°?               i
103
0     20     40
해자           nes       aia

413

@ Build Inference Model : output shape: (50,21)

1 # Get the prediction model by extracting Layers till the output Layer
2 prediction_model = keras.models.Model(
4     제지 4                           i      “
3     model. get_layer(name="image") input, model.get_layer(name= ‘dense2") . output
4)
5 prediction_model. summary()
i     ] impot | Lavone, 200, 59- 371 |
Layer (type)              Output Shape                  | tmneme: 22 [apa | 10766. 200. 50.171 |
image (InputLayer)        [(None, 200, 5@, 1)]            우러 이, | 39096 | Cree 500, 50040 |
      ] 아버] CNene. 200. 50. 32) |
(0041 (Conv2D)           (None, 200, 50, 32)
=       op | 29006 | Gvone, 200. 50. 327 |
기에   | outpoe |] Gvone. 3100. 25. 32) |
00011 (MaxPooling2D)      (None, 100, 25, 32)
_                          .                           |  .      .      [opus T None 500. 고. 523 |
-                                                                     Cov 2. Coma DD
Conv2 (Conv2D)            (None, 100, 25, 64)                          ] 여버버버 | GFone, 100.25. 64) |
+                                                         ap Leet | GNone 31090. 35. 69) |
00012 (MaxPooling2D)       (None, 50, 12, 64)          | poots         > eet | See ee
reshape (Reshape)        (None, 50, 768)                7         [impot [aie sors en]
nage       [outputs | Gvone, So 763 5  |
060561 (Dense)           (None, 50, 64)                 —
cropout_1 (Dropout)       (None, 50, 64)                                       a
Soe   5       oN   :                                  ：      ] 09929 | GNone, 50-64) |
bidirectional 2 (Bidirection (None, 50, 256)                | SEDONA NESS Fai 이. 90. 06 |
bidirectional_3 (Bidirection (None, 50, 128)       | 내에 수          GEIS I ee | Pees 20. SAY, |
dense2 (Dense)           (None, 5@, 21)                               4
=      souesesseescess            ta    ‘    aiietes_Sy: Biciewomomciareies jes oe eee) |
ne                     al            wai      af                    ] output: | Gvone. so. 12a) |
Total params: 432,725
vereewed Trainable params: 432,725                                               input. | Grone, 50, 128) |

denwe2 Denne |
[outpaa [Gone so- 217 |

| 414 | Non-trainable params: @

@한국시연구소 홍근선                    - 207- 무단 전재, 복제, Sal], 디지털화 금지



===== PAGE 209 =====
3부. Time Series & LSTM                           3.5 Time Series Classification : CTC

@ Inference + Decoding

keras.backend.ctc_decode( y_pred, input_length, greedy=True, beam_width=1 00, top_paths=1, )
- greedy: perform much faster best-path search if “true”.

- beam_width: if ‘greedy’ is “false: will be used this width.

- top_paths: if “greedy is ‘false’, #of paths will be returned.

results = keras.backend.ctc_decode(pred, input_length=input_len, greedy=True)

# results : ([(1,5@)],[(1,1)])

# results[@][@] :(2.50)= [17, 4, 10, 8, 18, -1, -1, -1, -1, ..., -1, -1, -1, -27
1 def decode_batch_predictions(pred):

7      input_len = np.ones(pred.shape[@]) * pred.shape[1] #(5@x21, )

3      # Use greedy search. For complex tasks, you can use beam search

4      results = keras.backend.ctc decode(pred, input_length=input_len,

5                                         greedy=True)[@][@][:, :max_length]
6     # Iterate over the results and get back the text    "Gere asa ge
7      output_text = []

8      for res in results:

9          res = tf.strings.reduce_join(num_to_char(res))

18          output_text.append(res)
33      return output_text

14 for batch in validation_dataset.take(1):

is      batch_images = batch["“image"][:1] #(1,26@,5@,1)<-(16,20@,5@,1)

16      preds = prediction_model.predict(batch_images)#(1,56,21)<-~-

17      pred_texts = decode batch predictions(preds) #(1,5)

is

13      img = (batch_images[@, :, :, ®]).numpy()

20      img = img.T

21      plt.title(f"Prediction: {pred_texts[@]}")

415

ae      plt.imshow(img)

@ 3.1 Time Series 개요
시계열 데이터를 설명하는 LO] (Trend, Seasonality, Aberration, Volatility, Nonlinearity)
@ 시계열 분석 방법 분류 : 시간영역 BA(SARIMA), 주파수영역 ZA (Fourier, Wavelet Transform)
® Deep ㄴ620[0100에서 시계열 분석 접근 BAI (Dilated Conv., RNN, Attention)
© 3.2 Time Series 개
# Time Series 데이터를 다루는 기본적인 접근과 분석 기법을 ASS 통해 확인
ㅎ 3.3 TCN and Other estarecturee
@ WaveNet
@ TCN
® Non-Local Block
® SCiNet
® 3.4 LSTM AutoEncoder : WSAE-LSTM, LSTM-SAE
® Seq2Seq 기본 구조와 Stacked AutoEncoder 이해
® WSAE-LSTM : Wavelet + SAE + LSTM 분석, 실습
@ LSTM-SAE : LSTM-based Stacked AutoEncoder 구조
@ Frequency Domain Analysis : Scalogram 변환
® 3.5 Time Series Classification

총         onnectionist Temporal Classification 이해, OCR(Optical Character Recognition) 실습

416 -

-         —               ~~

@한국시연구소 홍근선      -208- 무단 전재, 복제, Wall, 디지털화 금지



===== PAGE 210 =====
4부. Attention Based Model


===== PAGE 211 =====
4부. Attention Based Model                               4.1 Word Embedding

Chapter 4. Attention Based Model

4.1 Word Embedding

4.2 Attention Mechanism

4.3 Self-Attention

4.4 Transformer

4.5 GPT: Generative Pre-trained Transformer

= Word embedding+t Transformer                             .

© Word embedding                                            i aala    Parana   erbedelf '
@ 단어를 의미(의미적, 문법적 관계)있는 (6아아공간에 000100(학습)하는 것
®@ RNN2|¥FS| 에서 성능 향상을 위해 개발 됨
® Word2Vec(’13), 610\6('14), FastText(’17)

® Transformer= Positional Encoding} 함께 학습 가능한 embedding 사용
@ 사전 학습된 word embedding
# Embedding 초기값으로 사용하여 학습 속도 향상 가능, 최종 ASS 좋지 않았음

Large pre-trained

-RNN/LSTM            language models          76                   PaLM
rn     ㅣ                        :     :                      i                        i
'                                        t                  ‘
Word2ve and
N-grams                                        를       i
'           ;                                        i      :            i
'               Fane my                                             1         +                i
'                  '                                 {      1            |
…………      1                                 t 4            ‘
;      i                                 i      ‘            ;
i                                 i 4
eo. @     6            *      「 0]     *        ae

2013 2014 2015         2017 2018 2019 2020      2022

422         ee                빼                     "= Si DEEP L LEARNING

@한국시연구소 홍근선       - 211 - 무단 전재, 복제, Say), 디지털화 금지


===== PAGE 212 =====
4.1 Word Embedding

4, Attention Based Model
4 1 Wo      mbedda i  @

® VectorOl 의미나 관련성이 부여되지 않음
@ 주변 단어와의 관계를 고려하여 vectors 부

/ FastText(’17)

i,

= Random embedding , Word embedding, Word2Vec
- One-hot Encoding= 매우 2 희소 벡터를 생성, 확장성과 효율성 측면에서 문제가 큼
- Embedding 접근: Random, Term Frequency, Context based,---
@ Random embedding : 단어, 문장, 이미지 SS random vector mapping 하여 사용

® Model 초기화, 6356 line model, 의미를 부여하기 어려운 경우 사용
© Word Embedding : 단어를 의미(의미적, 문법적 관계)있는 (6아아공간에 mappingst= 것, 또는 방법

5

@ NLPOWAY 성능 향상에 기여함                                     Auto Embedding Weight Matrix
@ owe:                                       [| want to search for blood pressure result history”,
“> Word2Vec(’13)                          “Show blood pressure result for patient”, ... ]
^ Glove('14)                                    내                   Lod dod

im ㅣ       Input Layer

‘Learned
Vector0j] 의미 부여하기                                                                                   (Learned Vectors)
Ronaldo 1      0                                     ：   |    i 2
;         5                                     — ………
Messi}      0
Dicaprio 0        1                                                                         Embedding Layer

Togs

history

ae
2S

ar

3

@ Word2Vec

@ CBOW(Continuous Bag of Words)

 주변 단어들의 벡터를 평균하여 중심 단어를 예측
® Skip-gram

@ GloVe : Global Vectors for Word Representation

@ AZ: Google 검색, Netflix 추천 시스템, Apple Siri,---
® FastText : https://fasttext.cc/

®@ Shallow Neural Network= 구성

@ 부분 단어(506 Words)S 사용, 0/3 character 단위

A 학습 효율향상,단어 구조가 학습에 반영
® OOV(Out of Vocabulary) 문제 해결에 적합, 의미론적

ee                     ,             King         Man = Woman

A quick brown fox jumps over the lazy dog
문맥 안의 주변 단어를 이용해 SA 단어를 예측하는 방식으로 학습

a
- "Se 그의 ** 에게 ASS 주었다"라는 문

서 “**"에 “왕비"를 맞추는 과정을 통해 학습

A quick brown fox jumps over the lazy dog

 중심 단어를 가지고 주변 단어를 예측하는 방식으로 학습
- "왕 " 입력에서 "비서", "신하", "궁전" 등과 같은 관련 단어들의 출현 가능성을 계산하며 학습

@ Word2Vec9| 단점을 보완하기 위해, 전체 말뭉치(60ㅠㅁ45)에서 공동 출현 빈도를 활용
®@ Co-occurrence frequency(2s 출현 빈도) 두 가지를 고려하여 vector 학습 , 의미의 유사성 향상됨
AAS 출현 빈도: 전체 말뭉치에서 두 단어가 함께 출현하는 빈도 계산
 로컬 공 출현 빈도: 단어가 나타나는 문맥에서 두 단어가 함께 출현하는 빈도 계산

n-gram2 = 6770600109함

@ “eat”, “eaten” 같이 동일한 어근의 경우, \00「02\6<와 다르게 매개변수를 공유함

유추 작업 성능은 저하(65. word2vec)

P LEARNING |
E;    스다 사부 다노

ones rey

@한국시연구소 홍근선

- 212 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 213 =====
4부. Attention Based Model                               4.1 Word Embedding

% [실습] Word Embedding 실습
= 목적 : keras.layers.Embedding layerS 사용한 학습과정을 이해한다.
a 실습 개요
ㅎ IMDb Movie Reviews Dataset: 50K reviews (25K train, 25K test)
® Embedding layer 준비
 단어 인덱스를 06056 vector= mappingst+= lookup 13116역할을 St
® vector dimension= 실험적으로 결정할 02「(2006【6[임
@ 『300007으로 초기화 되고, 학습과정에서 단어간 유사성에 따라 변경됨

® Embedding Projector: https://projector.tensorflow.org/
® 학습된 embedding tableS                          안겨 BD 19 sn jt sects               .

“+ UMAP, T-SNE, PCAS2& projection 하여            @                               a            .

“ 단어들의 mapping(embedding) 22S                                          ni

(> 시각화 하여 확인하자                                                        oa

A 4-dimensional embedding                               ee
cat =>                                     e                         are       ‘
og      ‘

on => |              ;                                      >    are os

=]

= Dataset 준비
@ IMDb Movie Reviews Dataset: 50K reviews (25K train, 25K test)

i url = “https://ai.stanford.edu/~amaas/data/sentiment/aclimdb vi.tar.gz°

dataset = keras.utils.get_file("aclimdb vi.tar.gz", url,
4                                    untar=True, cache _dir='.',
5                                    cache_subdir="')

7 dataset_dir = os.path.join(os.path.dirname(dataset), ‘aclimdb‘)
8 dataset_dir, os.listdir(dataset dir)

(*./aclImdb', [*imdb.vocab‘, ‘README’, ‘train’, ‘test’, ‘imdbEr.txt’])        > Gm aclimdd
® train directory 사용하지 않을 '40540' directory 제거                             ㆍ Be test
> 를 train
© tf.data.Dataset 준비
@ 20% validation 031250[으로 분리

batch_size = 256
seed = 123

~""*gclimdb/train’, batch size-batch size, validation split-0.2,
subset='training’, seed=seed)

Re et

‘acl imdb/train’, batch_size=batch_size, validation split=e.2,
subset=’validation’, seed=seed)

ON Oh
<
ey
pay
a.
rr)
1
~
-
5
a
w
c
ch
ot
bed
w
ch
m
×
ef
oS
의
ct
o
“
f°)
fad
aS
5
[9]
닐
oo.
lon
a
fp
is]
oF
°
5
oe
^

Found 25000 files belonging te 2 classes.
Using 28000 files for training.
cone   =. Found 25000 files belonging to 2 classes.                          =                  바우 ae
“426     - Using 5000 files for validation.                ‘          나            ~    Ox DEEP LEARNING |

@한국시연구소 홍근선                   - 213 - 무단 전재, 복제, S4ll, 디지털화 금지



===== PAGE 214 =====
4부. Attention Based Model

4.1 Word Embedding
E                                =                                                                                       spas

for i “in range(S):
|    print(label_batch[i].numpy(), text_batch.numpy()[i])

Olas Me

b‘This movie is 50000 funny!!! The acting is WONDERFUL, the Ramones are sexy, the jokes are subtle, an
b"Alex D. Linz replaces Macaulay Culkin as the central figure in the third movie in the Home Alone emp
b’“Elvira, Mistress Of The Dark” is a sort of “Harper Valley P.T.A.” with touches of the supernatural.
0 b'If you\'re looking to be either offended or amused or both, you\'ll probably have to look elsewhere,

eo

@ Embedding layer 준비
@ 1,000 word vocabulary into 5-dim Embedding 레이어
2 embedding layer = keras.layers.Embedding(1006, 5)

3 result = embedding layer(tf.constant([1, 2, 3])) #1,2,3: word idx

4 result #(3,5):(seq., dim)                       a

<tf.Tensor: shape=(3, 5), dtype=flost32, numpy=

array([[ @.84859@83, -8.04520179, @.@4413471, @.04964267, @.0362782 J,
[ @.02328647, -6.04031762, -@.04686765, @.04236424, ©.82742431],
[-0.04306356, -@.0331414 , @.00599@79, @.93060374, 0.0264936411,
dtype=float32)>

@ embedding_layer(samples, sequence_length) : 정수로 구성된 2D 텐서

 가변 길이의 AWA 포함

/* (32, 10): (길이가 10인 32개의 문장/배치)

/@ [61417은 (32, 10, 5:vec-dim)
1 result = embedding layer(tf.constant({[@, 1, 2], [3, 4, 5]])) #(2,3)
2 _result.shape #(2,3,5)

427

<      see                "    ‘     "      5      "                     i

@ Text preprocessing

@ keras.layers.TextVectorization LayerS 사용하여, standardize, tokenize, vectorize 함
/* standardize : 구두점이나 HTML 요소를 제거, 데이터를 단순화 하기
@ Tokenize  ：문자열을 여러 토큰(단어)으로 분할
/* Vectorize ：토큰을 숫자로 변환

@ HTML tag 제거하기, <6『/>와 같은 다양한 HTML 태그가 포함되어 있음
/* TextVectorization layerOJA] 제거되지 않음
* HTMLS 제거하기 위해 표준화 함수를 만들어야 St

1 # standardization function to strip ‘<br />'.

2 def custom_standardization({input_data):

3    lowercase = tf.strings.lower(input_data)

4    stripped_html = tf.strings.regex_replace(lowercase,’<br />‘,' °)# ‘<br />’->' °
5   #문자열에서 추출된 ‘[¥%s]‘ (whitespace, [\t\n\f\r ])를 빈 문자열로 대체

6         return tf.strings.regex replace(stripped html,

7                           ‘[%s]' % re.escape(string.punctuation), °')

9 vocab size = 10000

16  sequence_length = 100

11 # Normalize,split,mapping(to an integer)
12 vectorize layer = TextVectorization(

13       standardize=custom_standardization,

44       max_tokens=vocab_size,

a5       output_mode="int’,

16                   output_sequence length=sequence_length)

17 +# vecorize_layer@] text dataset(no 136615)적용
| 18 text_ds = train_ds.map(lambda x, y: x) # x<-(x,y)    ee

| 428 |19  vectorize_layer.adapt(text_ds)           =       RK DEEP LEARNING
한국시연구소 홍근선                     -214- 무단 전재, 복제, Ll), 디지털화 금지



===== PAGE 215 =====
4부. Attention Based Model                                4.1 Word Embedding

= Classification Model-1: Average Pooling + Dense

@ GlobalAveragePooling1D Layer:
® sequence dimOll 대해 Bas 계산하여
 예제에 대해 고정 길이 출력 벡터를 반환

1   embedding dim=8                                           Layer (type)             Output Shape Param #
3                                                     >

3 ‘eadel = Sequential ({                           — (TextVe (None, 100)   &

4 -vectorize layer,                     #(bs, 168)

5    Embedding(vocab_size, embedding dim) ,#(bs,18@,8)| emeedding_4 (Embedding)    (None, 100, 8) 80000
6    GlobalAveragePoolingiD(),          #(bs,8)     global_average_poolingid 3 (None, 8)    0

7     06056(16, ‘relu'),                   #(bs,16)      (GlobalAveragePooling1D)

:  Bic sigmoid’ )                          dense 6 (Dense)        (None, 16)   144
106 model. summary ()                                     dense_7 (Dense)          (0006, 1)     17

1 optimizer = Adam(learning rate=0.0015)                        Max yal 0000 030

2 model.compile(optimizer=optimizer,               as

3                loss= ‘binary_crossentropy’,       06

4                metrics=[ ' 300406『0060'])              … Fe

z   ‘     .                      86 fio

6 history = model.fit(train_ds,                           SA

7                    | validation_data=val ds,      =       aw

8                  : epochs=10)                  Le Pa      =페소오오오고우오오오나우구에에

® Visualize embedding : https://projector.tensorflow.org/
® 학습된\0「0 embedding 저장하기
/* Embedding layer 읽어 오기

1 weights = model.get_layer(index=1).get_weights()[@] #(1000,8)
2 vocab = vectorize_layer.get_vocabulary() #['", [UNK]’,‘the‘,’and‘,...]

out_v = io.open('vectors.tsv', ‘w’, encoding=‘utf-8')
out_m = io.open(‘metadata.tsv', ‘w', encoding="utf-8")

for index, word in enumerate(vocab):
if index == 0:
continue # skip 0, it's padding.
vec = weights[index]
out_v.write(*\t’.join([str(x) for x in vec]) + “\n")
out_m.write(word + "\n")
16  out_v.close{)
11 _out_m.close({}

CON Du & wn eR

선반                                                           Nearest points in the original space:

great

superb

Dest

세니 |
:

트

, 디지털화 금지

2 06 ED:



===== PAGE 216 =====
4부. Attention Based Model                            4.2 Attention Mechanism

Chapter 4, Attention Based Model

4.1 Word Embedding

4.2 Attention Mechanism

4,3 Self-Attention

4.4 Transformer

4.5 GPT: Generative Pre-trained Transformer

_ & Attention 개요;        서게 제  ro cre argu) TE

w Seq2Seq 모델의 문제점 (Long Term Dependency Problem) .
@ MT(machine translation) 7|A|HS 에서 ~~0 빼 aia ae ee     So
@ 500.가길어지면 성능이 급격히 Boy                    !
® Decoder 전달되는 정보가 너무 제한적 ㅣ                             !
H    A          8          &          ＊…>       Leal         x          4          [

© 추가적인 정보 전달, 사용 방법?
@ 2014.9 “Neural Machine Translation by Jointly Learning to Align and Transiatir,   Bahdanau, Cho
@ Align 개념 제시 > Attentione = 발전
/* Encoder] hidden state= ( alignment weight2} 연산하여 )
/ Decoder hidden state 입력에 전달
“@ Alignment weight& 동시에 학습(자동으로 학습)
@ Decoder2| outputS           »
 결정하기 위해
input 특정 시점 정보와
연결시키는 학습 가능한
path7} 추가됨
 이전과 OSE 다른 세상!

BLED score

10           20            30            my           50           iH
Sentence length

432 __             이아 에                    mei che nat      “SR DEEP LEARNING |
@한국시연구소 S24                   - 216 - 무단 전재, 복제, #4, 디지털화 금지



===== PAGE 217 =====
2 content vettor 의 MPL (48)

4. Attention Based Model                           4.2 Attention Mechanism

8 Attention 동작(6390)         00900                                              pie
® Attention score              . i 06e-——         : ok
ㅎ Enc., Dec.2| hidden state2]    8 : f    ayy,                              Concatenate & i *)
Dot product > scalar score     8 =                 i =>~~~ Softmax(score to probability)   |    기

고: 고 cami      sf hy] 6 RN
@ Attention distribution
® ScoreS softmax 처리
확률로 변환
a’ = softmax(e’) € RY
> decoder state|A]
연관된 단어의 확률 분포
® Context Vector
® Encoder state 와                               Source sentence (input)
a i dist. weighted sum ( Attention output )

=      ‘h; S R*
a,    2 oO     S                         at

® Concatenate ( {a;;s,| < R2"            ie                  :
® Context vec.2} Decoder hidden state concatphate,   후에 > dense > softmax > output 7;

Dot-preduct attention

a"
^

Attention

Encode’

it  a m’ — entarté  <START> he hit me with a

Seq2Seq with Attention model

433                             http://web.stanford.edu/class/cs224n/slides/cs224n-202 1-lecture07-nmt.pdf         bd on LEARNING

= Attention 분류
® values {hy, ...,hy}= Rt 와 query 5 6 R°27} 주어져 있을 때 ( h:encoder / s:decoder state )
@ Attentione 항상 다음 요소들로 구성됨
1) attention scores       [e=far(h,s) ERY <—— 변형들은 이 값을 얻은 방법이 다른 것
2) attention distribution : a = softmax(e) € ^ (=attention weight)
3) attention output       ta=yM,a;h;] R“ (=context vector )

® Attention scores 계산하는 방법 (https:
Name                                             Alignment score function                                            Citation

Content-      score(s;, h;) = cosine[s;, hj!                                        Graves2014

base

attention

Additive?) score(s;,h;) = 이 tanh(W,|s,; h;))                                               Bahdanau2015,

Locations 0 007 = softmax(W, 8)                                                     Luong2015

Base               Note: This simplifies the softmax alignment to only depend on the target
position.

Ceneral              score(s;,h;) = 8, Wah;              = Maltiplicative                                                       Luong2015
where W, is a trainable weight matrix in the attention layer.

DotzProduct score(s,, hy) = 9, hj

.                                           ^

Scaled Dot= score(s;, hi) =  Fz

기          Ay

00064 ^)      Note: very similar to the dot-product attention except for a scaling

434                           factor; where n is the dimension of the source hidden state.                                          이 DEEP LEARNING

한국시연구소 S24                  -217- 무단 전재, 복제, Sl, 디지털화 금지


===== PAGE 218 =====
4부. Attention Based Model                            4.2 Attention Mechanism

들 2014.9 “Neural Machine Translation by Jointly Learning to Align and Translate”, Bahdanau, Cho

® Bahdanau Attention (Bahdanau,15 or Additive Attention)         1
@ 최초의 Attention                                          Ane      |
@ Context vector: 이 = 22917) :이는싸의 aj, weighted sum
+ Weight: 0,/ = softmax(e;;)      : weight align score2| 확률분포로 보자
@ Align score : e,; = a(s;-1, hy)        : score(energy)= decoder state s;_;7} encoder h,2| 연관성
+ Aligned model a: a() = vitanh(W,5;-1 + Ugh;)
feed forward network? = system2} 함께 StS =|0] soft alignmentS = 수행

"Encoder
“(Bi-dir RNN)

x = [X4, Ky]

7 eimai   —   '       ^ 대타 LEARNING )

@ Bahdanau Attention code
f@ Context vector: c       = Dye 1%jhj : encoder states 잘 수정해서 알려줘!
f Weight: a;; = fea
@ Align score : e;; = a(s;-1,hy)

/ Aligned model a: a() = vitanh(W,s;_1 + Ugh;)

class BahdanauAttention(tf.keras.layers.Layer):
def _ 101 (self, units):
super(BahdanauAttention, self). init__()
self.Wi = tf.keras.layers.Dense(units)
self.W2 = tf.keras.layers.Dense(units)
self.V = tf.keras.layers.Dense(1)
# si-l:queray: (batch, dec_s)
# h:values: (batch,N,enc_s)
def call(self, query, values):
query_with_time_axis = tf.exp nd_dims(query, 1)
score = self V(tf.nn.tanh(     #score: (batch,N,1(v))
self Wi(query_with_time_axis) 4 self.W2(values)))
attention_weights = tf.nn.softmax(score,  axis=1)
context_vector = attention_weights 7, values
context_vector = tf.reduce_sum(context_vector, axis=1)
return context_vector, attention_weights

436 _                                                                                                                                                            SOE DEEP EARNING”
bse es                                                                       i                                      si         £     fF OR,    Bods
@한국시연구소 홍근선                     -218- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 219 =====
4부. Attention Based Model                           4.2 Attention Mechanism

© Decoder GRU 재정의

Decoder

8; =tanh(WEy_1 +U [rs 0 S;.. 1| + Ce)                         나
,            r                                             or
2 =o (W, Ey; + Uzsj_1 + C.¢;)                        Attention
r; =o (W,Ey—1 + Upsi_1 + C,c;)                      E : word embedding metrix
Sp hh = 2a OR,     s._, / Decoder GRU for Attention                FEN
i=                                              i     >
@ GRU 2} 비교
hy = tanh (W - [ry * hy, 24)       Ey,
i
Cj

hy = (1 — 2%) * heer + 24 «hy

2000. U.,C,) = o(W.y, + U.s. + C.c.)

437                                              < DEEP LEARNING

® Architecture & Results                   P(yil¥i,---,¥i—-1,X) = 9(Yi-1, $i, Gi)
@ 긴 A/HAS 조건부 SSS 해결하는 모델 제안
@ 단어간의 연관성을 시각적 확인 (3460101효과 )

:    A ~s SER :                      Eyi-1
classifier

Eyi-25)    Decoder

Attention

hi» layer

Decoder

Was
he = 711 in
°                     확장 확인
.         Sentence length  ule                   Encoder
            매빼~       ae      (Bi-dir RNN)
20 ~       eee                       3 = ty 00001
150                           9

BLEU score

RNNewc-#)

1}          20          301          ay          30          60
Sentence length

…                           ;                                ｌ                                          입맛 DEEP LEARNING

-219- 무단 전재, 복제, Sal], 디지털화 금지

438
@한국시연구소 홍근선



===== PAGE 220 =====
4부. Attention Based Model                            4.2 Attention Mechanism

a                      내

@ 2015.8 “Effective Approaches to Attention-based Neural Machine Translation”, Luong

@ Overview                     me he ar     Local Attention                Ye
® direct prediction( h; > >, )
@ Local attention                                 보우건
@ MZZAttention(LuongAttention) | (=
@ Input-feeding-approach
@ Luong Attention

enc:        37 eC: s;—>h, s:source,t:target
/ Context vector: <, = Dt, a; hy

_i.. _| softmax(e,)
+ Weight: a, = Nene) : location-based
+ Align score : e, = a(h;,h;)                                                        hy = tanh(Welev; hy)
—           : Dot product                  P(wly<t, ©) = softmax(W hz)
nh,              pe
!'                                       =      : Multiplicative(general
/ Aligned model : a() =        hi Wah,            "       —

vi tanh(W,[hy; hs]
© direct prediction (h; > y;)
® Bahdanau Attention: s;_, 필요 했음

Concat

GRU

| for
Attention
—    —_—_—_—___ eee

@ Local attention (vs. Global attention)                        Local Attention                           일
: 부분적인 input stated 보자
/* 060006[는 504[66의 위치 P, 를 예측하고,
> [를 중심으로 작은 windowS 사용하여 6ㅠㅇ006『 state##Z
> Attention layerS Fixed dim. Vector= 관리 가능
> Windows Gaussian distributionAF=
soft / hard attention2] 조합

= Attention output 계산방식으로 분류

: Soft vs. Hard attention

®@ Soft: Alignment weight7| 확률분포형태로 학습 : 기본방식
* 장점 : 미분 가능 모델 ( 학습이 쉽다 )
* 단점 : source7} 크면 비용이 많이 요구됨

@ Hard: attention 위치가 하나로 지정 되도록 SS(one-hot)
@ 장점 : inference 시간을 줄일 수 있음
 단점 : loss 미분 불가 복잡한 학습방법이 요구됨 성능은 좋음

@ Self attention : ㄷ0ㅁㅇ006@「만 있음
®@ 504[「06560.내에서 연관성을 찾음, 5604『66에서 queryS 생성,

anne                                    ae           ~            SAC SEER LEARNING”
@한국시연구소 홍근선                     -220- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 221 =====
4부. Attention Based Model                            4.2 Attention Mechanism

w Attention2| 장점

@ NMT(Neural Machine Translation) 45S 크게 향상

a Decoder7t input data 특정 부분에 집중하는 것은 매우 유용함
ㅎ Seq2Seq2 29] bottleneck 문제 해결
“@ Decoder7} data sources 직접 볼 수 있도록 함(병목 현상 우회)
® Gradient vanishing 해결에 도움이 =
@ 먼 상태에 대한 shortcuts 제공
@ 모델의 해석을 좀더 가능하게 함
/* Attention distributionS 확인하여 Decoder 무엇에 초점을 맞추고 있는지 확인 가능
@ Alignment systemS 명시 적으로 훈련하지 않음

Sof DEEP LEARNING
CESS ee ee

% [실습] Neural machine translation with attention

w 스페인어를 영어로 변역 하기 위해 AWA-F-A|WA (seq2seq) 모델
® Transformer 모델보다 다소 구식이지만,
® Seq2seq.2} attention mechanism’ 이해하기 쉬운 모델

* 왼쪽의 모델을 약간 수정하여 오른쪽 모델로 구현

What
time
is
[END]

it

Je

suis étudiant </s>

attention
vector

context
vector

attention
weights ~

os:
<

=
EREET) PEEia

Peri) bE |
fttt fttt

{        그
>        | |e
ee  내내 ols   래  2 oe
| am a student <s> je suis étudiant   O/5/2/ 8/0) |으 $|§]2| =
@한국시연구소 S24               -221=   Be 단 전재, 복제, SH, 디지털화 금지


===== PAGE 222 =====
4.2 Attention Mechanism

4. Attention Based Model

= Dataset

준비
® http://www.manythings.org/anki/ 에서 제공되는

언어 dataset 사용

import pathlib

ue oi

path_to_zip = tf.keras.utils.get_file(
‘spa-eng.zip',

tet

| origin="http://storage.googleapis.com/download.tensorflow.org/data/spa-eng.zip’,

|  extract=True)
path_to file =

ow

pathlib.Path(path_to_zip).parent/'spa-eng/spa.txt*

| 1 _ text = path to file.read text(encoding=‘utf-8')|

io! \nFire!\t;Disparad! \nHelp! \t;Ayuda! \nHelp!\tjSocorro!

pi\tjPara! \nStop!\t;Pare!\nWait!\t;Espera!\nWait.\tEsperen.\nGo on.\tContinta.\nGo on. \tConting

jAuxilio! \nHelp!\t;jAuxilio! \nJump!\t;5|

® Target22tz} 입력문장(60016×!) 분리

[target_raw]:

Shape: (118964, )
Type: <class ‘numpy.ndarray'>
Values: [‘Go.’ “Go.* ‘Go." ...
‘A carbon footprint is the amount q
‘Since there are usually multiple
‘If you want to sound like 8 native
[context_raw]:
Shape: (118964, }

1 def load_data(path):

2 | text = path.read_text(encoding="utf-3")

3    lines = text.splitlines()

4    pairs = [line.split('\t') for line in lines]

5    context = np.array([context for target, context in pairs])
6    target = np.array([target for target, context in pairs])
c    return target, context

1 target_raw, context_raw = load_data(path_to_ file)

2 p(target_raw, ‘target_raw’)

3 _p(context_raw, ‘context raw’)

Type: <class ‘numpy.ndarray’>
Values: [’Ve.' ‘Vete.' ‘Vaya.’
‘Una huella de carbono es la cantid
“Como suele haber varias paginas we
‘Si quieres sonar como un hablante

Unicode normalize : 약센트 부호가 있는 문
@ 각문장에[51401] 및 [ENDJE2S 추가

분할하고 호환 문자를 해당 ASCH 문자로 대체

is_train =

# is train:[ True

4

4                              False
6 train_raw = (

7

8

9

True True ...      True
tf.data.Dataset
-from_tensor_slices((context_raw[is tr.

.shuffle(BUFFER_SIZE)

np.random.uniform(size=(len(target_raw),
True]

ain],   target_raw[is_train] ))

.batch(BATCH_SIZE))
11 val raw = (          :
12       tf.data.Dataset
13              .from_tensor_slices((context_raw[~is train], target_raw[~is_train]))
14      . shuffle(BUFFER_SIZE)
15      .batch(BATCH_SIZE))

coe

J

4. def tf 10066 000 split_punct(text):

2    # Split accented characters.

3    text = tf_text.normalize utf8(text, ‘NFKD')
4

text = tf.strings.lower(text) # b’\xc2\xbftedavi\xcc\x8la esta\xcc\x81 en casa?’

5    # Keep space, a to 2, and select punctuation.

6    text = tf.strings.regex_replace(text, "[* a-z.?!,g]', '')# b’\xc2\xbftodavia esta en casa?"

Z    # Add spaces around punctuation.        ;할    외는 제;

8    text = tf.strings.regex_replace(text, "[.?!,g]', r’ \@ ')# 6) \xc2\xbf todavia esta en casa_?_"
9    # Strip whitespace.                   _ 문자 SSO 삽입    ue

16    text = tf.strings.strip(text) # b’\xc2\xbf todavia esta en casa 2' BS SON 제거

il   text = tf.strings.join(["[START]*, text, "[END]‘], separator=' ‘)   Mpnnnn
12    return text
elodavia esta en casa?
22            we) [START] ¢ todavia esta en casa ? [END]   =                  SEEP LEARNING |
@한국시연구소 홍근선                  - 222 - 무단 전재, 복제, S4l, 디지털화 금지



===== PAGE 223 =====
4부. Attention Based Model                           4.2 Attention Mechanism

4.      tention Mechanism

* Data 준비(2)
@ 단어 Hola} 역방향 단어 색인 만들기
/ TextVectorization layerS 사용하여 token index 생성

max_vocab_size = 5000

3          standardize-tf lower and split punct,
4       max_tokens=max_vocab_size,
5    | ragpged=True)

context_text_processor.,adapt(train_raw.map(lambda context, target: context))
8 _context_text_processor.get vocabulary()[:16]

['', *[UNK]*, "[START]*, “[END]*, ‘.', ‘que’, ‘de’, ‘el’, ‘a’, ‘no’]

/ Strings to tokens

1 print(example_context_strings[:3])

2
|3 example tokens = context_text_processor(example_context_strings)
| 4 example tokens[:3, :]

tf.Tensor(

[b’Quiero que vayas a ver si sigue ah\xc3\xad.°

b'Mi mam\xc3\xal me dio permiso para ir al cine.’
b*\xc2\xalNo te emociones tanto!'], shape=(3,), dtype=string)
<tf.RaggedTensor [[2, 48, 5, 812, 8, 118, 45, 668, 213, 4, 3],
12, 24, 749, 18, 208, 1389, 31, 70, 37, 828, 4, 3],

® Data 준비(3)
@ 단어 색인과 역방향 단어 색인 만들기
/* get_vocabulary method 를 사용하여 token 105를 text= 변환
context_vocab = np.array(context_text_processor.get_vocabulary())
# context_vocab:array([‘", “[UNK]', "[START]', ...,'descubri* ])
tokens = context_vocab[example_tokens[@].numpy()]

print (tokens)
5 print(’ *.join(tokens))

bm uw Nm be

[°[START]’ ‘quiero’ ‘que’ ‘vayas* ‘a’ ‘ver’ ‘si' ‘sigue’ ‘ahi’ ‘.* ‘[END]"]
[START] quiero que vayas a ver si sigue ahi . [END]

@ 각 문장을 최대 길이로 수정하고, masking 하기

| 1 example tokens.to tensor() |

aeray({[ 2, 48, 5, ..., 0, 06, 0],
[ 2, 24, 749, ..., 0, 6, 6],
[ 2, 9, 3@,..., 0, 0, 0],

plt.subplot(i, 2, 1)                           |
plt.pcolormesh(example_tokens.to_tensor())     |
plt.title( Token IDs‘)                           %0
pit.subplot(i, 2, 2)

pit.pcolormesh(example_tokens.to_tensor{) != @)
plt.title('Mask')                               |»

Token IDs

Aw & wnK we

|    <tf.Tensor: shape=(64, 29), dtype=int64, numpy

Mask

10    20
@한국시연구소 홍근선                    - 223 - 무단 전재, 복제, Se, 디지털화 금지



===== PAGE 224 =====
4부. Attention Based Model

[

4.2 Attention Mechanism

® Data 준비(4)
ㅎ (.010[6짜와 Target textS model.fit(OlA APS dataset object= 만들기

& 고정길이 10<605으로 바꾸고,

/* 1319하은 target-in: [0, .…, 0-1] , target-out : [1,....0] 을 생성하여,

/ (context, target-in), target-out) 쌍으로 반환

def process text(context, target):

context = context_text_processor(context).to_tensor(}
target = target_text_processor(target)
targ_in = target[:,:-1].te_tensor() # token: [@,...,n-1]
targ out = target[:,1:].to_tensor() 호 token:[1,...,n]
return (context, targ_in), targ_out

train_ds = train_raw.map(process text, tf.data.AUTOTUNE)
val_ds = val raw.map(process text, tf.data.AUTOTUNE)
context_vocab = np.array(context_text_processor.get_vocabulary())
target_vocab = np.array(target_text_processor.get_vocabulary())

for (ex_context_tok, ex_tar_in), ex_tar_out in train_ds.take(1):

print(ex_context_tok[@, :1@].numpy())
print (context_vocab[ex_context_tok[¢, :2¢].numpy()])
print(ex_tar_in[@, :1¢].numpy())
print(target_vocab[ex_tar_in[@, :10].numpy()])
print (target_vocab[ex_tar_out[@, :10].numpy()])

[   고   10 355   16 111   35    6 3830    4    3]

| [51200] ‘tom’ ‘necesita’ ‘un’ ‘poco’ ‘mas’ ‘de’ ‘practica’ 1. '[6600]')

ON AW hm wR RPO MN OD 내 &% ww 하하

cad

i 2    9 440 106 175 91 1935    4    a    0]
[5101] ' ‘tom’ ‘needs* ‘a’ ‘little’ ‘more’ ‘practice’ '.' 1 11]

447 [190 ‘needs" ‘a’ ‘little’ ‘more’ ‘practice’ '.° "[END]' °° ‘"]       .   “Sy DEEP LEAR! ING

® Model 만들기
ㅎ Encoder= 왼쪽, Decoder= 오른쪽
®@ 각 time 5[60에서 060006「출력은 6ㅁ006 출력과 결합하여
@ 다음 단어를 예측함
@ Encoder
# Encoder2| $= context sequences
Decoder7} 2+ time stepO] 대한 다음 SHS 예측하려 할 때
유용한 vector sequences 생성 하는 것
양방향 RNNE 사용

Target-out

t        ee
E      | 두
isle) |못| |즌호오
으16|으| 8|쁘 |으흐|등으|=
Context      Target-in
as           ne                anneal 91a

@한국시연구소 홍근선                    -224- 무단 전재, 복제, 24], 디지털화 금지



===== PAGE 225 =====
4부. Attention Based Model

4.2 Attention Mechanism

@ Encoder

ㅎㅎ context_text_processorO|A] 토큰 10 목록을 가져 옴.

ㅎ layers.EmbeddingS 사용, 각 토큰에 대한 embedding vector 를 찾고,
ㅎ bidirectional GRUS 사용, embedding vector 처리

@ 처리된 AJ HAS YS, attention head= 전달

1 class Encoder(tt.keras.layers.Layer):

2

3     super(Encoder, self). init 0

4      self.text_processor = text_processor

5       self.vocab_size = text_processor.vocabulary_size()
6      self.units = units

7      # The embedding layer converts tokens to vectors
ㅎ

9

0

1

self.vocab_size, units, mask_zero=True)

1       # The RNN layer processes those vectors sequentially.

13       self.rnn = tf.keras.layers.Bidirectional(merge mode='sum",

12                              layer=tf.keras.layers.GRU(units, return_sequences=True,
13                              recurrent_initializer='glorot_uniform’))

14    def call(self, x):

15      # embedding vector <- each token.

16     x = self.embedding(x)

17      # GRU processes                   _

18      x = self.rnn(x)

encoder = Enceder(context_text_processor, UNITS)
ex_context = encoder(ex_context_tok)

ps(ex_context_tok) #{batch, s):(64,16)
ps(ex_context)    #(batch, s, units): (64,16,256)
——                  -—

450

@ Attention Layer(1)
@ Decoder7} EncoderOAj 추출한 정보에 접근하는 경로를 제공
ㅎ Context 560.에서 \6다아를 계산하고,
® Decoder $40|] 추가함

1 class CrossAttention(tf.keras.layers.Layer):

2   def init__(self, units, **kwargs):

3      super{)._init__()

4     self.mha = tf.keras.layers.MultiHeadAttention(key dim=units, num_heads=1, **kwargs)

5              self.layernorm = tf.keras.layers.LayerNormalization()

6      self.add = tf.keras.layers.Add()

7   def cali(self, x, context):

8     attn_ output, attn_scores = self.mha(

9               query=x,      #005, t, units)                                ca

10               value=context, #(bs, s, units)                                뽀 듬

11                           return_attention_scores=True)                                                          £ 을

32     #(bs,t,s)<-(bs, heads, t, 5)                                         x

13      attn_scores = tf.reduce_mean(attn_scores, axis=1)

14      self.last_attention_weights = attn_scores

15     x = self.add([x, attn_output])                   |] , |, |, | LLL

ie     BOI wg acetate 이                              Key, Value         Query  |

1 # ((ex_context_tok, ex_tar_in), ex_tar_out) <- train_ds.take(1}

2  attention_layer = CrossAttention(UNITS)

3 # Attend to the encoded tokens

4 embed = tf.keras. layers.fmbedding(target_text_processor.vocabulary_size(),

5                           output_dim=UNITS, mask_zero=True)

6 ex_tar_embed = embed(ex_tar_in) #(64,16,256)<- (64,16)

7 result = attention layer(ex_tar_embed, ex_context)#(64,16,256)<-((64,16, 256), (64,16, 256) eee
from Encoder 00                 어그

@한국시연구소 홍근선                    - 225 - 무단 전재, 복제, Fall, 디지털화 금지


===== PAGE 226 =====
4부. Attention Based Model                             4.2 Attention Mechanism

@ Attention Layer(2)
@ Attention weight

f Target seq.2| 각 시점에 대해서
“ Context seq.(Encoder 560.)들의 attention weightS sum 하면 '1'
/* softmaxS 통해 S22 표현 되었으므로 4470 10 1

2 ps(attention_layer.last_attention weights) #(batch, t, s):(64, 16, 16)
2 p(attention_layer.last_attention weights[@].numpy().sum(axis=-1))

[] Shape(64, 16, 16)

[9.9999999 1.          4.          cs          4.          Ass          1 .0000001    |                              =
1.             1.             4.             1.             ‘i.             3             1.                |                                       a2
1.             1.           ]                                                                                                                     28
® target seq.(t=0)01] 대한 context seq.2|
@ attention weightS 확인하기 위해                                                    |
@ 「085(처리하여 시각화 해 보자                                                                 Key, Value             Query
1 attention weights = attention_layer.last_attention weights #(bs,t,s):(64,16,16)

2  mask=(ex_context_tok != 6).numpy()                        #(bs,s): (64,16)

3                                                                                                    Attention weights
4 pilt.subplot(1, 2, 1)                                       비타
5 plt.pcolormesh(mask*attention_weights[:, 0, :])           도
6 plt.title( ‘Attention weights’)
>                                                                                             *

8 plt.subplot(1, 2, 2)                                       =
9  plt.pcolormesh(mask)

210 plt.title('Mask');                                         cod
/* 학습하기 전이므로 ASS 1/seq_len 29S 초기화 되어 있음 wee
451 _                      :                                    ：                  newly

@ Decoder

®@ Decoderé Target 560.의 각 시점에서 다음 tokenS 예측(생성)함
@ Target seq.2| 각 1061에 대한 600ㅁ600100결과를 얻어오고,
/* RNN layerS 통해, target 560.를 처리하여 지금까지 생성한 HSS 추적함
/* RNN $23 Attention layer2| 0461`값으로 넣어, Encoder2| 출력에 attendingst7ll 함
 각 시점에서의 출력은 다음 10(60의 예측임
@ 훈련할 때 모델은 각 위치에서 다음 단어를 예측
@ 따라서 정보가 SAS 통해 한 방향으로만 흐르도록 해야 st
@ 따라서 060006「는 13『96Ｌ 560.처리를 위해 단방향(양방향이 OF Y)RNNS 사용
@ AES 실행할 때 한 시점에 하나의 HOS 생성하고, 피드백 되어 입력으로 추가 됨.

ㅎ Decoder call method

@Decoder.add_ method
def call(self, context, x, state=None, return_state=False):
# x:(bs,t), context: (bs,s,units)

x, state = self.rnn(x, initial_state=state) # x:(bs,t,units)

x = self.attention(x, context)

0 Ow Oa Vim Wh

18     if return_state: return logits, state
41    else:            return logits

@한국시연구소 홍근선                   -226- 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 227 =====
4부. Attention Based Model                            4.2 Attention Mechanism

@ Decoder(2) : 10110

1 class Decoder(tf.keras.layers.Layer):
2    @classmethod
3   def 300 method(cls, fun):
4     setattr(cls, fun. __name_, fun)
5      return fun
6    def init__(self, text_processor, units):
7     super(Decoder, self). init ()
8      self.text_processor = text_processor
9      self.vocab_size = text_processor.vocabulary_size()
10    | self.word_to_id = tf.keras.layers.StringLookup(
11          ㅣ             vocabulary=text_processor.get_vocabulary(),
12        mask_token="", oov_token="[UNK]*)
13              self.id_to_word = tf.keras.layers.StringLookup(
14                       vocabulary=text_processor.get_vocabulary(),
5          mask_token='', oov_token="[UNK]",
16         invert=True)
17    | self.start_token = self.word_to_id('[START]‘)
18    | self.end_token = self.word to id(’[END]")
19      self.units = units
20             self.embedding = tf.keras.layers.Embedding(self.vocab_size,
21                                      units, mask_zero=True)
22      self.rnn = tf.keras.layers.GRU(units,
23                                return_sequences=True,
24                                return_state=True,
25                                                                recurrent_initializer="glorot_uniform’ )
26    | self.attention = CrossAttention(units)
27    | self.output_layer = tf.keras.layers.Dense(self.vocab_size)
7]

@ Decoder(3)
® context2} target tokensO| 주어지면, C+ target tokenS 예측

1 decoder = Decoder(target_text_processor, UNITS)
2 #(bs,t,target_vocab_size):(64,14,5000) <- (bs,s,units):(64,17,256),(bs,t): (64,14)
3 logits = decoder(ex context, ex_tar_in)

® InferenceS 위한 method 추가

1 @Decoder.add_ method

2 def get_next_token(self, context, next_token, done, state, temperature = 9.6):
3    logits, state = self(_ _##Decoder

4     context, next_token,

5      state = state,

6     return_state=True)

7    # logits:(bs,t,50e0)

8    if temperature == 0.0; # 무작위성 BSc(ereedy)

9      next_token = tf.argmax(logits, axis=-1)

10   else: # temperaturee 무작위성을 HA (epsilon-greedy)

11     logits = logits[:, -1, :]/temperature

12      next_token = tf.random.categorical(logits, num_samples=1)

13    # “end token 을 만나면, ~done’<-1

14    done = done | (next_token == self.end_token)

315   # 560.에서 “done 을 만나면, next_token="@ padding

16 ： next_token = tf.where(done, tf.constant(@, dtype=tf.inte4), next_token)
17 ㅣ: return next_token, done, state

1 @ecoder.add_method
2 def get_initial_state(self, context):
batch_size = tf.shape(context)[¢]
VAS on              :                 0            eomein                 ae                                                                        :   DEEP LEARNIN

| 호  pees

@한국시연구소 S24                   - 227- 무단 전재, 복제, Sl, 디지털화 금지

\ <



===== PAGE 228 =====
4부. Attention Based Model                             4.2 Attention Mechanism

® Inference test

@ Test generation loop: 학습 전이므로 무작위 단어 배열

1 # Setup the loop variables.

2 next_token, done, state = decoder.get_initial state(ex_context)
3. tokens = []

4

5 for n in range(5):

6    # Run one step.

7    next_token, done, state = decoder.get_next_token(

8      ex_context, next_token, done, state, temperature=1.¢)

9    # Add the token to the output.

16     tokens .append(next_token)            #(n,64,1)

a2     print(f'n[{n}]:{decoder.tokens to text(tokens)[:,0].numpy()}")
12 # Stack all the tokens together.

13. tokens = tf.concat(tokens, axis=-1) #(bs,t)<-(t,bs,1)

14  # Convert the tokens back to a a string

15 result = decoder.tokens_to_text(tokens)#(bs,)

16 ps(result, result’) #(bs,)

17__ print(result[:3])#.numpy())

n{@]:[b’ lawyer’
n{1]:[b’ lawyer’ b'visited']

n[2]:[b’ lawyer’ b’visited’ b‘goats’]

n[3]:[b’ lawyer’ b'visited’ b'goats’ b’mark"]

n[4]:[b’ lawyer’ b'visited’ b'goats’ b’mark' b‘decision’]

[result] Shape(64,)}

tf. Tensor(

[b' lawyer visited goats mark decision’

b'dried talked eventually conditions accused‘

b'unwilling more hitch competent entered'], shape-(3,}, dtype=string)

10

428

@ Translator model 만들기

1 class Translator(tf.keras.Model):

2    @classmethod

3    def add_method({cls, fun):

4     setattr(cls, fun._name_, fun)

5      return fun

6

7    def init__(self, units,

8               context_text_processor,

9                                       target_text_processor):
10      super().__init__()
11      # Build the encoder and decoder
12      encoder = Encoder(context_text_processor, units)
13      decoder = Decoder(target_text_processor, units)
14
35      self.encoder = encoder
16      self.decoder = decoder
17
18    def call(self, inputs):
19    | context, x = inputs
20     context = self.encoder(context)
21    _ logits = self.decoder(context, x)

22    | return logits

1 model = Translator(UNITS, context_text_processor, target_text_processor)
2  logits = model{(ex_context_tok, ex_tar_in))

3 # ex_context_tok(bs,s}:(64, 2@)

4 # ex_tar_in(bs,t): (64,2¢)

5 # logits(bs,t,target_voca_size):(64,20,5000)

에                             ss   2                        ES ae                             ve
_ 456                                                          :      ARNING

한국시연구소 S24                       -228- 무단 전재, 복제, i), 디지털화 금지



===== PAGE 229 =====
4부. Attention Based Model                            4.2 Attention Mechanism

ㆍ

* Masked Loss, Masked Accuracy function
@ 24 문장의 길이가 다르므로, 1055, accuracyAlAtalol] 보정이 필요함
 의미 있는 부분만 남기고, 의미 있는 560.길이로 나누어 보정

1 def 0059660 _loss(y_true, y_pred):

2              loss fn = tf.keras.losses.SparseCategoricalCrossentropy(
3     | from_logits=True, reduction='none')

4     loss = loss_fn{y_true, y_pred)

5      # Mask off the losses on padding.

6      mask = tf.cast{y_true != 6, loss.dtype)

7      3055 _*= mask

8      return tf.reduce_sum(loss)/tf.reduce sum(mask)
1 def masked_acc(y_true, y pred):

2      y_pred = tf.argmax(y_pred, axis=-1)

3      y_pred = tf.cast(y_pred, y_true.dtype)

4      match = tf.cast(y_true == y_pred, tf.float32)

5     mask = tf.cast(y_true != 06, tf.float32)

6      return tf.reduce_sum(match)/tf.reduce_sum(mask)
1 model.compile(optimizer="adam',

2             : loss=masked_loss,

3         _ metrics=[masked_acc, masked_loss])

457

=]

@ Translator model Training

2 history = model.fit(
3     _ train_ds.repeat(),
4     : epochs=100,
5    _ steps per_epoch = 106,
6       validation_data=val_ds,
Z      validation_steps = 20,
8             callbacks=[tf.keras.callbacks.EarlyStopping{patience=3) ] )
Masked_Acc                                Loss
07                            대           이 oss
—— val_loss
0.6 4                          44
05 +                      ¢
34
0.4             ve     oh
034 /          ,      :              24
024                        4                                                                        a
ween accuracy                                 14
ea Py 5 val_accuracy 0    |
06         T       T              T        o-—       T       T              +
0      5      10      15      20          is]      =      10     15      20
~                =                                        1]                     2           roy
@한국시연구소 S24                    - 229- 무단 전재, 복제, Sai, 디지털화 금지


===== PAGE 230 =====
4부. Attention Based Model                            4.2 Attention Mechanism

© Translator model : Translate method 추가하기

2 @franslator.add method

3 ©6def translate(self, texts, *, max_length=56, temperature=90.9):

4    # Encoder: context<-RNN{context)

5     context = self.encoder.convert_input(texts)

6    batch_size = tf.shape(texts)[¢]

7    # Setup the loop inputs

g    tokens = []

9    attention_weights = []
10    next_token, done, state = self.decoder.get_initial_state(context)
11    for _ in range(max_length):

2      # Generate the next token
13   | next_token, done, state = self.decoder.get next 10660(
14   |    context, next_token, done, state, temperature)
15    |  # Collect the generated tokens
16     tokens .append(next_token)
17              attention_weights.append(self.decoder.last_attention_ weights)
18    |  if tf.executing_eagerly() and tf.reduce_all(done):
19   |   break # tf.reduce_all(done):done BS True?
20    # Stack the lists of tokens and attention weights.
21    tokens = tf.concat(tokens, axis=-1) # (bs,t)<-(+,bs,1)
22    self.last_attention_weights = tf.concat(attention weights, axis=i) # (bs,t,s)<-(t,bs,1,s)
23    result = self.decoder.tokens to text(tokens)
24    return result

1 result = model.translate([';Todavia esta en casa?‘]) # Are you still home
2  result[@].numpy().decode()

“is still at home 2 “|

“459°

@ Translator model : Attention weight plot 하기
2 @franslator.add method

3 Vdef plot_attention(self, text, **kwargs):

f    assert isinstance(text, str)

output = self.translate([text], **kwargs)
output = output[].numpy().decode()

>

wi

fon

1태미

8          attention = self.last_attention_weights[9]

10        context = tf_lower_and_split_punct(text)                                          we

11     context = context.numpy().decode().split()

12        output = tf_lower_and_split_punct (output)
3     output = output.numpy().decode().split()[1:]                      a

15    fig = plt.figure(figsize=(is, 10))
16    ax = fig.add_subplot(i, 1, 1)

i?   ax.matshow(attention, cmap="viridis', vmin=6.9)

18                                                     tex}

19    fontdict = {'fontsize’: 14}                                       _
20   ax.set_xticklabels([‘"] + context, fontdict=fontdict, rotation=9@)

21    ax.set_yticklabels([‘‘] + output, fontdict=fontdict)             |
2    ax.xaxis.set_major_locator(ticker.MultipleLocator(1))            |
23       ax.yaxis.set_major_locator(ticker.MultipleLocator(1.))                     |
A    ax.set_xlabel(’ Input text’)                                  |
25    ax.set ylabel( ‘Output text’)                                 |
1  00061.010Ｌ _attention( ‘jTodavia esta en casa?') # Are you still home

2 model.plot_attention(’Esta es mi vida.') # This is my life. |

460
국시연구소

근선                    -230- 무단 전재, 복제, all, 디지털화 금지

@
ro

00



===== PAGE 231 =====
4부. Attention Based Model                           4.2 Attention Mechanism
_4.2 Attention Mechanism __

© 성능 검토 : 입력이 길면 모델은 문자 그대로 초점을 잃고 합리적인 예측 제공을 중단
®@ Teacher-forcing : 이 모델의 학습은 모델의 예측에 관계없이
& 각 단계에서 올바른 SSS 강제로 공급하여 SHS
ㅎ Normal-training: 자체 예측을 입력으로 제공하면 모델이 더 견고해질 수 있음
@ RNN 상태를 통해서만 이전 출력에 access 할 수 있음
+ RNN 상태가 60016짜 seq. 위치를 추적하지 못하면 SAS 복구할 방법이 없음
/* Transformer= Decoder7} 이전의 모든 출력 내용을 볼 수 있어, 개선 됨

® Ｌ00965【560.에 대한 결과 확인

print(f'source context ({len(context_raw[-1])})::{context_raw[-1]}')
4 _print(f'Target text({len(target_raw[ -1])})::{target_raw[-1]}')

Source <
Target text(247}::If you want to sound like a native speaker, you must be willing to practice say

£
c
호
8 3           90000 99006                             “Twot            6009"           "running?
ae                      \                 \
sf      ES             ‘|                  |                                                  4
35. S509             |         |                  ㅣ                  |             |                   |
B28 >5a29                     a     ㅣ                   pose ms       "=

sai ae a 시   ㅣ

/   \  f   ee:   \   rf   도  a   \  f   4
ANN )구걱 RNN }-f-{ RNN }-+> | ANN }—> RNN po ORNN }—>

A  rd  \    i Me A   개      개     a  of
ㅣ   1  \      \          |
=                                        <Star> | Two Se bids" Se 아나    “Two?
:                                                                                   Normal training                      *      ：           ㅡ
|  Ground Truth  |

Teacher forcing training

461               Sov DEEP LEARNING

462   i        eee     a et    수태 LEARNING

@한국시연구소 홍근선               - 231 - 무단 전재, 복제, Sail, 디지털화 금지

i
00


===== PAGE 232 =====
4부. Attention Based Model

Chapter 4, Attention Based Model

4.1 Word Embedding
4.2 Attention Mechanism
4.3 Self-Attention

4.4 Transformer

4.5 GPT: Generative Pre-trained Transformer

4.3 Self-Attention

DEEP LEARNING
RE           R YOU

Cree FO

= Attention mechanism2| 일반화: Scaled dot-product Attention
¢@ “Attention Is All You Need”Oj|Aq 제안
@ ParameterS Al2|stz attention operation?! 있는 구조

@ FSS 위해 외부에 layerS 두어야 함

Bahdanau(Additive) Attention

…

Scaled dot-product Attention
r

i

Bil 뽀즈여다녀 abode 1네게제디제 iousctadd deedi
Quen      Key      Vaiue|

| Query Layer | Key Layer | Value Layer |

464                                                                                 ㅎ            TER DEEP CEARNING™
@한국시연구소 홍근선                    - 232 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 233 =====
4부. Attention Based Model                                   4.3 Self-Attention
_4.3 Self-Attention Mechanis

@ Attention(Q,{K:V}); Q: query, <: key, V: value (key value= 찾기 위해 참조하는 값 )
{K:V} : dicti
ㅎ Attention(Q,{K:V}¥= softmax (2) V
Vax.
@ (에 연관된 정보 ve 전

* \와 연관된 (와의 유사도를 구하고: QKT
/* 값이 너무 커지지 않도록 나누어 _ ：0&*『/,/@,
* 유사도(500「6)를 확률로 변환하고, softmax(QK"/,/d, )
 결과를 vo} 곱한다 ,         softmax(QK" //d, )V
& 0에 연관 정도에 따라 변환된 \를 얻음

@ 일반화 정의 : 벡터 431406와 벡터 query7} 주어지면,
query 에 따라 value2| weighted 5417을 계산하는 기술
@ Queryol 따라 임의의 표현 집합(66【 of 「(60「656013100)에 대한 고정길이 RAS 얻는 방법
®@ Weighted sum : 값들에 포함된 정보의 선택적 요약으로 해석 됨
# ㅁㅁㅇ0006「의 hidden state(query)S 받고, Encoder9] hidden 5【+23165(4\81469)에서
관련정보를 선택적으로 요약하여 제공

465                                            a          |           ge DEEP LEARNING

w Self-Attention Mechanism
® Key7t 없으면 VE 사용
| Output data
© Q& 없으면 Q=K=V                                        때에

® Self-attention : K, Q, V from same source
@ Same 504106에서 Layers 통하여 전                    ;  Scaled dot-product Attention

@ 학습 가능 \는 입력에 있는 layery
D> 입력 560.내에서 관계를 학습 ( intra-attention )

Query                 Key               Value

| Query Layer | Key Layer | Value Layer |

Input data
everyone in the world is watching us very closely
FSSSZaR80S 85 .  eeeeee) Ge:
r     A
mary Jat
~ a 가       ^
s 8   €228   2bsbeoBs 828
So288_%32   Fses2e23.$33
466           saat    …. AAR

@한국시연구소 홍근선                    - 233 - 무단 전재, 복제, 4], 디지털화 금지


===== PAGE 234 =====
4부. Attention Based Model                                   4.3 Self-Attention
-

@ Self-Attentionz} RNN 비교

® RNN
® input= CHS step] hidden 444404] 관여
@ 순차적으로 처리, 병렬처리 불가능
A 순서가 중요함

® Self-Attention
@ 동시에 h2, h3 처         처리 가능
 순서가 의미 없음
 순서가 필요한 경우 순서 정보 추가 필요

we

9 Eabyey EM, ms Say       | 」  LJ  wil
—      on         aii         I     go   home

Bans hike wa,

@ Self-Attention 의 처리 과정 : K, 0, V from same source
q=x*W4 = dense(w1)(x),k= ...,v= ...

Input                           Thinking Xy              Machines X,

Embeddi
mbedding                               a

Queries

Keys

Values

Score

Divide by 8 ( a )

be iran as sera _ _ Attention Laver , 0010 수    으으

!              Attention Operation             |

Softmax

Sum         (      ]
1) 고,
Fred

rat af
http://jalammar.github. io/illustrated-transformer/      bid SEESTLEKRINE”

("0

- 234 - 무단 전재, 복제, Sal, 디지털화 금지

×

1
4 Value Layer |  Key Layer  ㅣ Query Layer |



===== PAGE 235 =====
4부. Attention Based Model                                    4.3 Self-Attention
4.3 Self-Att

m Self-Attention 개념
* 맛있는 케이크를 찾기 Sel Self-AttentionS 사용한다면
@ 케이크 목록 생성
@ 케이크 5개의 SSS 만들고, 각각의 맛, 크기, 가격 등 속성 표현
 케이크 0000600109
 각 케이크 SAS 벡터(80ㄱ76600109)로 변환
® Query, Key, Value 벡터 분리: 케이크의 벡터를 세 부분으로 분리
* Query :케이크 선택에 관여할 주요 특징
Key :：케이크들의 특징에 대한 평가 요소
@ Value ：각 케이크의 정보 (맛, 크기, 가격,…)
# Attention score 계산
 원하는 케이크 특징(60460`)과 케이크의 특징평가 요소((6))의 관계를 산출
/* 0, K vector YAS 계산하고, softmax 함수로 0~1 사이의 attention score 계산
 중요도 2A (weighted value)
 각 케이크의 SA (value)2} F$2= (attention score)\S 곱하여 원하는 특징에 높은 weightS 부여
@ 최종 케이크 벡터
/* 0460》에 대한 각 케이크의 특징을 weighted 5411하여 벡터를 생성
* 이 벡터는 query} 모든 케이크와의 HAS 고려한 정보를 담고 있음
® 케이크 선택
@ 최종 케이크 벡터를 고려하여 가장 맛있을 것으로 예상되는 케이크를 선택
여러 데이터(이미지,음악,단백질구조,…)간의 BS 고려해 특정 목표에 맞는 결과를 도출

Sof DEEP LEARNING

469

4.3 Self-Attention Mechanism

w Self-Attention 의 특징
® 자기 AMIS 설명하는 SAS 찾아내는 모델
@ AutoEncoder2} 차이점
® AutoEncoder : Seq.2| 특징을 찾아서 압축
@ Self-Attention : 560.내에서 관계를 특징으로 학습
@ Enc.+ attention + Dec. > self-attention + RNN
»> Self-attention(Enc.) + Self-attention(Dec.) = Transformer
®@ Self-attentionft2 = Enc, Dec. 구성
* 병렬처리에 적합한 구조
@ 560.를 한번에 동시에 처리 가능 수 수 수 수 수
@ RNNS!C} 빠르게, <44보다 멀리 처리 가능
® 순열동등 : (500) = (f(x)
@ 동시에 처리가능 > 순서를 모른다!
> 순서 정보를 같이 제공하여 해결                                Ｌ
® Stacking 하면 value2| average7} =!
ㅎㅎ nonlinearity #7} 필요
® Decoder 사용하려면(660.를 생성하려면)                                 Query
® CS stepS 못 보도록 0ㅠ25109이 필요함

weights

Key, Value
Attention

_ ba

470                                                                                                                                              Pd ed Sota an

@한국시연구소 S24                      -235- 무단 전재, 복제, ai], 디지털화 금지

[


===== PAGE 236 =====
4부. Attention Based Model                                     4.3 Self-Attention

a 병렬처리에 적합한 구조
* 560.를 한번에 넣어 처리 가능                       Bidirectional RNNs and CNNs
* RNNSICH 빠르게     RA Ge
® CNNSECH 멀리 처리 가능

Attention
weights

Key, Value

The global self-attention layer

w 병렬처리에 적합한 구조(2)
@ One query / input vector
® X KV EMS 같이 바꾸면 > Y= 같이 by

@ 순서를 모름
® ×에 Position code 추가 필요
@ Masked self-attention : NLP decoderS 에서
다음 값에 대한 WSS 제거하기 위해 사용

Inputs:

Input vectors: X (Shape: Ny x D,)

Key matrix: W, (Shape: Dy x Dx)

Value matrix: W, (Shape: D, x Dy)

Query matrix: WW. (Shape: D, x Dg)

Computation:

Query vectors: © = XW,

Key vectors: K = XW, (Shape: Ny x Dg)

Value Vectors: V = XW, (Shape: N, x Dy)

Similarities: E = QK' (Shape: Ny x Ny) E,, = Q;- K,/ sqrt(Dg)
Attention weights: A = softmax(E, dim=1) (Shape: Ny x Ny)
Output vectors: Y = AV (Shape: Ny x Dy) ¥,= 3)A\;V) (Seq, Vaim)

ij

472            ERK DEEP LEARNING”
@한국시연구소 홍근선                   -236- Sot 전재, 복제, 24, 디지털화 금지



===== PAGE 237 =====
4부. Attention Based Model                                   4.3 Self-Attention
Self-Attention Mechat
a 순열동등 : 순서가 바뀌어도 결과는 같다 > 순서를 모른다!

> 순서 정보를 같이 제공하여 해결
* Position code concatenate : Sinusoidal position representations

( sin(i/100002"2/4) )
cos(i/100007*1/4)
P= |        :
|        ㆍ    a
| sin(i/10000"*2/*)
 6050 10000“"2/03)                             Index in the sequence
Dy = V; + Di
Gi = G+ Pi
ki = ki + pj

@ nonlinearity : Feed Forward Net.

® Stacking 하면 value2| average7} 됨
® nonlinearity 추가 필요
@ FF: m; = MLP(output;)
® Seq.2| 각 출력에 개별적으로 다 실행

self-attention
a     a     a   … &f
Wy               W2                W3                        Wr

‘DEEP LEARNING

9 8 > 다트

mw Feed Forward Net 개선

® 75(2019):                  FFNreiu(x, Wi, We) = max(2W,,0)W
FFNgg.u (2, Wi, W2) = GELU(xW)We

® GeGLU base(2020): FFNeiu (2, WV, W2) = (o(cW) @ xV) We
FFNopjinear(, W, V, W2) = (zW @ «V)We
FFNreciu(z, W,V, W2) = (max(0,2W) @ 2V)We
FFNcecuu(2, W, V, We) = (GELU(zW) @ 2V)W2
FFNswicnu(z, W, V, We) = (Swish; (xW) @ cV)W2



===== PAGE 238 =====
4부. Attention Based Model                                     4.3 Self-Attention

XX [실습] Self-Attention

m= 목적 : 간단한 Self-Attention 2AES 만들고, 특징을 이해 하자.
a 실습 개요
® Scaled Dot-Product Attention Layers 만들고
® Max 찾기 : 560.에서 maxi 찾는 SAS 만들어 특성 검토
®@ Input data : Random seq. (batch, 10, 1)를 만들고
®@ Target data : input 560.에서 max2tS 찾아 (batch, 1) 생성
@ Attention2]2, ㅁ6056모델을 만들어 비교해 본다.
© OCS 두수 합 찾기 : '0'다음에 나오는 두수를 더한 US 찾는 SHS 만들어 특성 검토
® Input data: Random2= seq. (batch, 20, 1)를 만든다.
/* Randome& 임의의 위치 값을 '0'으로 바꾸고
Target data : OCHS 값 SS 더한 값으로 (621, 1, 1) 생성
Attention22, ㅁ6050모델을 만들어 비교해 본다.
Input data] Position codeS concatenates}O] (batch, 20, 5)로 수정
Dense, LSTM, Self-Attention, LSTM + Self-Attention,
Self-Attention + LSTM, Stacked Attention 22S 만들어
Attention layer2| 특성을 확인한다.

475             |            여               아태 LEARNING

@ Scaled Dot-Product Attention Layer 만들기

1 def myAttention(Q, K, V, l=""):

2    | ak       = Lambda(lambda x: tf.matmul(x[0],x[1],transpose_b=True),name="q_k")({Q, K))

3    |  dk       = Lambda(lambda x: tf.cast(tf.shape(x)[-1],tf.float32),name="d_k”){K)

4    ㅣ sacaled_qk = Lambda(lambda x: tf.divide(x[0],xf1]),name="sacaled_gk”)((g_k, tf.sqrt(d k)))

5 、 | weight     = Activation(’softmax',name="attention weieht”"+1)(sacaled_qk)

6    | output    = Lambda(lambda x: tf.matmul(x(@J.x[iJ]), name='output'+1)( (weight, v))

7    __return output

® Plot_model= 확인하기 위해 모두 layer= 구성                                          alt attewtiyu  Oe !
/* Lambda layer= 연산을 wrapping                                          Scaled Dot-Product Attention Layer

/* StackingA| ‘name’0| 겹치지 않도록 해야 함

1  1710060 010=106 # input Dense hidden_units
2 n_classes=16 # out_dim

3 shape=(20,5) # (seq., features)
4
5

inputs = Input(shape=shape)
Q% Dense(hidden_dim, name='y')(inputs)#(bs, seq, hidden dim)
K 4 Dense(hidden_dim, name='K')(inputs)#(bs, seq, hidden_dim)
V7 Dense(n_classes, name="V')(inputs) #(bs, seq, out_dim)
9 output = myAttention(Q, K, V)       #(bs, seq, out_dim)
16 model = Model(inputs,output)

@ Q.K,V: input based value , dense= 가공

/ Attention layer= parameter7} 없음
 내부 \확인을 위해 UH dense '10'로 놓고 확인

Q KV

@한국시연구소 홍근선                    - 238 - 무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 239 =====
4부. Attention Based Model                                    4.3 Self-Attention

® Scaled Dot-Product Attention model : 자체로는 #P 적고, 연산은 ㅠ811×연산으로 가능한 구조

* K, 0 matrix 연산 > (seq, seq)
/ Attention_weight:(seq, seq)                                             malt ie Te
4 AttW, V matrix > (seq, out)                                             estan | onset 이

@ 차: 180                                                    |
Layer {type}            Output Shape             Param 분

그 | input: | (None, 20, 5)    의 | 00 | (None, 20, 5)
input_13 (InputLayer)     [(None, 20, 5)]          8              Dense | output: | (None, 20, 10)   Dense | output: | (None, 20, 10)
K (Dense)             (None, 28, 18)          co              J.      Ss     j           \
@ (Dense)             (None, 20, 10)          개     dk | 때: | (None, 20, 10)   066 | input: | ((None, 20, 10) (None, 20, 10)  \
Lambda | output:   0    Lambda | output:    (None, 20, 20)
d_k (Lambda)            ()                    @        로        \
4
Ly
q_k (Lambda)           (Hone, 20, 20)          8        녹    timathsat 6 | input. | 0                 고 | ina | (None, 20, 5
‘.
“S| TOpLambda | 0004: | 0            Dense | output: | (None, 20, 10)
tf.math.sqrt_6 (TFOpLambda ()}               8           ane       는                |
)                                                         ~

~ 9000.06 | 406 | (00062020.0| |

sacaled ok Soambia) one, 20, 28)           2                             1409 [ome] om m2 ||
abcention wetgnt (Activati _ (Nove, 20, 20)           8                                       '              '
an)                                                                     atiention_wei   it     (None, 26,
'                                                                     계기 그르
V (Dense)              (Hone, 20, 10)          2                                     oe
output (Lambda)            (None, 20, 10)              8                                                    \
court | input: | ((None, 20, 20), (None, 20, 10)}
Lambda | output:      (None, 20, 10)
Total params: 180 (728.0 Byte)
477                     =o                                                         30 DEEP LEARNING

= Find max model       1 a iereth = 10
2  num_samples = 5000
® Data generation        3 x dim = 1
.                  4 ## x_data.shape:(bs,seq,x dim)
@ Attention model       5  x_data = np.random.uniform(size=(num_samples, seq_length, x_dim))*i2
ㅎ 최소한으로 만들어 BA ©  y_data = np.max(x_data, axis=1) #(bs,x 010)1(565.1)
1 hidden 01055                                          [x_data] Shape(seee, 10, 1)
2 n_classes=1                                  7      [y_data] Shape(5eee, 1)
3 shape=(16,1) #(seq, x_dim)
4                                                     ee
5 inputs = Input(shape=shape)                       Wax YY ah,
6 Q = Dense(hidden_dim, name='Q')(inputs) #(bs, 10, 5)
7 K = Dense(hidden_dim, name='K')(inputs) #(bs, 16, 5)
8 V = Dense(n_classes, name='V')(inputs) #(bs, 16, 1)
29 x = myAttention(Q, K, V)           #(bs, 16, 1)
18 x = Flatten()(x)                  #(bs, 30)
11 output = Dense(1)(x)                 #(bs,1)
12                                                Outputpart \    K
13 model = Model(inputs,output)                  output | input: | ((None, 10, 10), (None, 10, 1))
Total params: 33                          때 개포
Trainable params: 33          Input part
mput | [(None, 10,1                input:
애마 pene  input’ | [@None, 10, 1)]          flaten_6 | input’ | (None, 10, 1)
output: | [@Voune, 10, L)]          Flatten | output: | (None, 10)
ane  input. | (None, 10. 11   Diese  input: | (None, 10. 1)             dense_6 | input: | (None, 10)
output: | (None, 10, 5)         output: | (None, 10. 5)              Dense | output: | (None, 1)

@한국시연구소 S24                   - 239 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 240 =====
4부. Attention Based Model                                    4.3 Self-Attention

@ Attention model                                Attention_weight
® Attention Weight 보기                                         atteution_ weight: Activat     ial   a ve "
ol    벡    One,  A
/* Callback3}+3 통해 feature map 시각화                                              uutput: | Qrons, 10102

/ keract.get_activation( ) : modelOl| xB 넣고, layer nameS 참조하여 feature map 받아옴

10 #88 Training 중에 feature map 시각화 하기
31 class VisuelizeAttentionMap(Callback):

17     def on epech begin(self, epoch, logs=None):

18         attention_map = get_activations(self,model, self.x)[‘attention weight’ ]
19       Hit (b, 5602) <- (b,seqi,seq2)

20          attention_map = tf.reduce_sum(attention_map[:,:,:],axis=1)

@ Compile & Fit (with callback function)
2 batch size = 256
3
4

max_epoch = 100
model = Model(inputs, output)
model.compile(loss='mse', optimizer="adam', metrics=['mape'])

5

6

7 # visualize the attention on the first samples.

8 visualize = VisualizeattentionMap(model, x_data[@:10])

9 history = model.fit(x_data, y_data, epochs=max_epoch,
18                 batch_size=batch size, validation split=e.2,

—         wpe             ,   배메  os       ,     ‘  "Se BEER nT

ee ees

® Attention model 학습 결고
® Attention layer output : x_data [0:10] 을 모델에 넣어서 outputZte| 변화를 확인

Min mape.1.43, mse:0.029

i                            =~" mape
3                              ~                                                                     ——— valmape
홈                                                 \
5                                     A                                     :                                                    .
aw                                  ae                                 Qe                                                \
다                                            개                                            등호
ce                                 ea                                38
9                                      y                                      2
BE                                 BE                                 gE
58                                     oS                                     x8                                                                .
ey                                      5                                      ag
<                                      i                                      E
Li                                     2                                                                                al
nee.
time steps                                 time steps                                 time steps                               0          20         40         o         80         100

Min mape:1.43, mse:0.029

@ Dense model 학습 결과 : 동일한 를 갖는 모델 설계

00606
inputs = Input(shape=shape)    |                          \               은 aes
x = Dense(7)(inputs) #{bs,10,7) |
x = Dense(1) (x)      #(bs,10,1) |                               \

x = Flatten()(x)    #(bs,10) |                               ~
cutput = Dense(1)(x) #(bs,1)   |                               | 에
model = Model(inputs, output)   | | Total params: 33                      ‘

Min mape:6.85, mse:0 597

10?

Abe

Wd Ae

OO

® Dense model& 잘 학습하는걸?!!                     0   2   제   or   aos aa

SELLS  £

@한국시연구소 B24                   - 240 - 무단 전재, 복제, S44], 디지털화 금지



===== PAGE 241 =====
4부. Attention Based Model                                    4.3 Self-Attention
_ 4.3 Self-Attention Mechanis

= Add two number (: 20개의 Seq. OA] '0'다음에 나오는 두수를 더한 값찾기 )
ㅎ Data generation                                                s€  02 S\    Septet
@ Input data 44 : x_train (20000, 20, 1), y_train( 20000, 1)                                     이
/* 8300011으로 560. (batch, 20, 1) 생성 , 0~10 값                    eye 시   Up)  4
@ Random 위치 = 곳의 값을 '0'으로 바꾸고
/* Target data : '0'다음 값 SS 더한 2O= (batch, 1) 생성
5 560 = 20
6 x_train, y_train = task_add_two_numbers_after_delimiter(n_train, seq, test=True)
7 prime)
8B test_index_1 = 4
| 9 test_index 2 = 9
10 x_test, y_test = task_add_two_numbers_after_delimiter(

11                           | n test, seq, 0, test_index 1, test_index 2, test=True)

13

[e.        7.79918792 0.        7.23465178 9.77989512 5.3849587
5.01120464 @.72051133 2.6843898 4.998825@1 6.79229996 8.@3739836
3.80941133 @.65936347 2.88145599 9.99593528 2.13385354 4.52123962
9.3120602 @.24899228] [15.0338397]

19 2

[6.80548917 0.        2.30302879 5.48489919 9.09128375 1.33169446
5.23412581 7.50409859 6.69013241 4.6775286 2.484989 4.90765889
3.72384689 4.77401155 3.6589@386 8.37917994 7.68647507 3.13994677
Q.      2. 76049048] [5.06351927]

49

(2.35120407 9.64971 9.45048224 0.        4.72323996 8.41476715
1,31110642 3.08733657 0.       7.41847201 4.85825229 1.36876119
3.4353653 3.2442617 3.90418904 1.655014 4.14981773 4.48120658
774900376 7.96390701} [12.14171197]

® Position coding’

1 def positional encoding(length, depth):          #(seq, x_dim)

2    depth = depth/2

3    positions = np.arange(length)[:, np.newaxis] #{seq, 1): @ ~ 560 168
4     depths = np.arange(depth)[np.newaxis, :]/depth #(1, x _dim/2): @~ 1
5

6

angle rates = 1 / (10@@0**depths)               #(1, x_dim/2): 1 ~ 1/(10@08)
angle rads = positions * angle rates           #(seq, x_dim/2)
8
9    pos_encoding = np.concatenate([np.sin(angle rads), np.cos(angle rads)], axis=-1)
10    return tf.cast(pos encoding, dtype=tf.float32) #(seq len, x dim)

© Append position code

2 def idx _value(x) :

3      idx = positional encoding(length=x.shape[1], depth=4)
4       idx = np.tile(idx,(x.shape[@],1,1))
5      ps(x,'x'),ps(idx, ‘idx’)
6
7

ret = keras. layers.concatenate([x,idx],axis=-1)
| ps(ret,'[x,idx]’)
| return ret

50 75 «2S 925 150 175
Position

@한국시연구소 홍근선                     -241- 무단 전재, 복제, tall, 디지털화 금지


===== PAGE 242 =====
4부. Attention Based Model

4.3 Self-Attention

ㅣ

shape=x_train.shape[i:] # (20,5)
inputs = Input(shape=shape)

x = Dense(32)({inputs) #(bs,20,32)
x = Dense(1)(x)        #(bs, 20,1)
x = Flatten() (x)      #(bs ,26)
output = Dense(i)(x)  #(bs,1)

model = Model{inputs, output)

Dewe'th 72)

m Dense w/ index : 전체를 보고 학습, 560. 학습불가

Layer (type)

Output Shape

input_17 (InputLayer)
dense_26 (Dense)
dense_27 (Dense)
flatten_13 (Flatten)

th.

dense_28 (Dense)

ON MW Mi Ue uM ke

max_epoch = 100
batch_size = 256

model.compile(loss='mse", optimizer="RMSprop', metrics=['mape’ ])
history = model.fit(x_train, y_train, validation_data=(x_val, y_val),
epochs=max_epoch, verbose=1, batch _size=batch_size,)

{(None, 20, 5)]
{None, 20, 32)
{None, 20, 1)
(None, 20)

(tone, 1)

Total params: 24

Min val_mape: 82.76789093017578
Min val_mse: 17.733716964721 68

160 Py            pre   4   wen   aed    901                       배부
i                                      |                         val joss
F                             8  '                          :
340 나                                  i
;                             1
q                             @
120 +4                    ma
:                             ~~ valmape | 50
'
100 +!                             °
(AAA ana Vy   30
ad                               20 | Aen ae
8     20    ©    ©    80    100     8     20    2     @    Es    300

w LSTM wo/ index : Sequences 보고 학습, 학습가능

4

세 나 de ww Ne

shape=(26,1)
inputs = Input(shape=shape)
x=

x = Flatten()(x)
output = Dense(1)(x)
model = Model(inputs,output)

LSTM(5,return_sequences=True) (inputs) #(bs, 20,5)

#(bs, 100)
#(bs,1)

Layer (type)

Output Shape

input_23 (InputLayer)
Istm_5 (LSTM)
flatten_19 (Flatten)

dense_38 (Dense)

[(None, 20, 1)]
(None, 20, 5)
(None, 108)

(None, 1)

Tota

l params: 241

Min
Min
166

1406

pee

zeae 8

val_mape: 15.595877647399902
val_mse: 1.256827712059021

2 print(‘target:\n’,y test)
3 _print(‘predicted:\n',y pred)

1 y_pred = model.predict(x_test[:,:,6],verbose=0)

~                          ~ 0006
             i     “ee val mae

em
me

omen

ee

e B56 8 8 8 © 8 BS B

== toss
~ val_loss

target:
[[15.84450581]
[ 1.97304869]
[ 1.67674111]
[ 5.56544162]
[15.773@2879]
[12.651858@7]
[ 4.65781466]
[ 6.28355721]
[11.68882215]
[ @.423285e7]]
predicted:
[[16.568476 ]
[ 2.4197466]
[ 2.7751539]
[ 6.002926 ]
[13.1431265]
[13.001986 ]
[ 5.575@327]
[ 6.303639 ]
[10.06079 ]
[ 2.72331 76]]

6      20      40      &      80     1099

ee            04

@한국ㅅ^

|연구소 ec

무단 전재, 복제, Sil, 디지털화 금지



===== PAGE 243 =====
4부. Attention Based Model                                   4.3 Self-Attention
If-Attention Mechanism

를 Attention wo/ index : 가장 간단한 Self-Attention 22, 학습 불가

1 hidden_dim = 16                             Min val_mape: 53.92655181 8847656
2 n_classes = 5                            Min val_mse: 14.080591201782227
3 FFN = FeedForward(n classes, n_classes*4)

6 inputs = Input(shape=shape)                   mas:
!   Q= Dense(hidden dim, name='Q') (inputs)
| 은 K = Dense(hidden_dim, name='K")(inputs)
19 V

x

= Dense(n_classes, name='V‘)(inputs)

HO__ Xx:    =_myAttention(Q, KV)

11 x = FFN(x)                    #(b,20,5)

12 x = Flatten()(x)                 #(b, 100)

13 output = Dense{1)(x)             #(b,1)            8     a    2     ©    80    100

14 00061 = 000061(1004ㄴ5,00ㄴ0 )              Total params: 400

2  max_epoch = 1060

3 batch_size = 256

4

5 history = model.fit(x_train[:,:,@], y_train, validation_data=(x_val[:,:,0], y_val),

6                epochs=max_epoch, verbose=2, batch _size=batch size,
47                         callbacks=[VisualiseAttentionMap wo()])

2 from keract import get_activations

3 class VisualiseAttentionMap_wo(Callback):

4     def on epoch end(self, epoch, logs=None):

5       if (epoch%2) 1= 6 : return

6         attention_map = get activations(model, x test[i:,@])[ ‘attention weight’ ]# wo/inde

7         attention map = tf.reduce sum(attention map[:,:,:],axis=1) #(10,28)<-(16, 2, 22)     ,

485        : 20 마타 LEARN

® Feed Forward Network 만들기                                           orbs, Steatue®)

1 class FeedForward(tf.keras.layers.Layer):

2   def init__(self, 0 00061, dff):

3     super()..init_()

4      self.ff = tf.keras.Sequential([

5         tf.keras.layers.Dense(dff, activation='relu'),

6       tf. keras.layers.Dropout(¢@.1),

7                 tf.keras.layers.Dense(d model),

8     ])

9   def call(self, x): #(bs, 500 168, 90)

18     return self .ff(x) 2(      len, 0)

1 class FeedForward2(tf.keras.layers.Layer):

2    def init__(self, d_model, dff):

3     super({).__init_()

4      self.ff = tf.keras.Sequential([

5      layers.ConviD(dff, kernel_size=1, activation="relu"),

6       layers.Dropout(@.1),

?      layers.ConviD(d_model, kernel _size=1),

8     ])

8   def call(self, x): #(bs, 560 160, 0)
18   return self.ff(x) #(bs, seq len, 0)

1 en_emb = tf.random.uniform((64, 20, 5))

2 sample ffn = FeedForward(5, 32)        |

4 ps(en_emb)                     | [] Shape(64, 20, 5)             1204
5  05(520016 ffn(en_emb))             | [] Shape(64, 20, 5)

5

oa                  - 243 - 무단 전재, 복제, S4l], 디지털화 금지

@
rok
nf

씨연구소

00


===== PAGE 244 =====
4부. Attention Based Model

4.3 Self-Attention

i hidden dim = 16 # 32
2 nclasses = 5 #1
FFN = FeedForward2(n_ classes, n_classes*4)

had

4  shape=x_train.shape[i:] # (20,5)

5

6 inputs = Input(shape=shape)       #(b, 20,5)
? Q = Dense(hidden dim, name=‘Q') (inputs)

& K = Dense(hidden dim, name="K‘)(inputs)

2 V = Dense(n_classes, name="V')(inputs)

16 x = myAttention(Q, K, V)         #(b,26,5)
11 x = FFN(x)                     #(b, 20,5)
12 x = Flatten()(x)                #(b, 108)
13 output = Dense(i)(x)             #(b,1)
14 model = Model(inputs, output)

Total params: 548

® Visualize Attention Map
ㅎ Test data : 값은 randomO|2, ‘0’ 위치는 4, 99! data sample 1074 준비
® CallbacketOlA x_testS 입력으로 넣고 Attention_weight2| 출력 Z
 학습이 진행되면서, 165 0312에 대해 4, 9 번 22/S attentionsH= 것을 시각화

a Attention w/ index : 가장 간단한 Self-Attention 22, 학습 거의 안됨

160

140

Min mape: 76.43, mse. 16.642

:
A Noy
Yep ga i:
zl We ale ha 개

att

을 받아서 시각화

def

if (epochk2) I= 0 :

I
| attention_map = get activations(model, x test)[‘attention_weight'] ## w/index
i
i

"487

attention map =

tf.reduce sum(attention map[:,:,:],axis=1) #(18,20)<-(16,20, 29)

Si DEEP LEARNING

| Self-Attention Mechanism

0           20          40          60          80

@ LSTM + Attention wo/ index : 15114을 통해 560. 정보를 획득, 학습 가능
Set ONE) ctm unit 2g  |
2 hidden_dim = 3
3 n_classes = 5
4 FEN = FeedForward(n_classes, n_classes*4)
5  shape=(seq length,1)
| Seacrest
? inputs = Input(shape=shape)       #{(b, 20,1)
8 × = LSTM(istm_unit, return_sequences=True)(inputs)#(b,26,9)          iteration 098 / 100
cM 9 ee Dense(hidden_dim, name='Q'}(x) #(b, 28,9)
10 K = Dense(hidden_dim, name='K‘)(x) # °’
11 V = Dense{n_classes, name='V'}{x) #(b,20,5)
12 x = myAttention(Q, K, V)         #(b, 20,5)
313 x = FFN{x)                     #{b,20,5)
14 x = Flatten{){x)               #(b, 100)
15 output = Dense(1)(x)             #(b,1)
16 model = Model(inputs,output)
Min mape:3.66, mse.0.153)
150 4.7%                 rane           |                   --- 1055
Hi                  -ㅡ~ val_mape     a aaa aa GU WA- val_loss
125 4-4-4                             i
‘                      4015
190                              i
75  나                      * '
‘                      207-4
254    (해          TE away때     10    +
We   "
이       nite | gf SS
100       0         40              100

P LEARNING
ee eee es

@한국시연구

i

aca

무단 전재, 복제, Si, 디지털화 금지



===== PAGE 245 =====
4부. Attention Based Model

4.3 Self-Attention

_4.3 Self-Attention Mechanism

@ LSTM + Attention w/ index : LSTMO| 있어서 1ㅠ06×정보의 의미가 없음

RoW hm

lstm_unit = 9 #

hidden_dim = 9

n_classes = 5

FFN = FeedForward(n_classes, n_classes*4)
5 shape=x_train.shape[1:] # (20,5)

? inputs = Input(shape=shape)

16 model = Model(inputs, output)

Min mape:3.82, mse:0.166

8 xX = LSTM(Istm_unit, return_sequences=True) (inputs)#(b, 20,9)
9 Q = Dense(hidden dim, name="Q")(x)#(b,26,9)

10 K = Dense(hidden_dim, name='K‘)(x)

i V = Dense(n_classes, name="V')(x) #(b,20,5)

x = myAttention(Q, K, V)         (b, 20,5)

3 xX = FEN(X)                   #(b, 28,

4 x = Flatten()(x)               ie,
15 output = Dense(1)(x)            #(b,1)

|

iteration 098 / 100

|  1  19헤1 unit =9
| 2 hidden 010 = 9

| 3 n_classes = 5

4  shape=x_train.shape[i:] 4 (28,5)

150  명                  ~~~ mape       25 dete                  ~~~ loss  ai
5                 —— val_mape        {                   —— val_loss
125                                   204-4
：    4                        10 +44
해        eee ee at mancant ates        0 a cena      사아:
0    20    40    60    80    100       0    20    40    60    80    100
489                                                                                                                                              9 DEEP LEARNING
4.3 Self-Attention Mechanism                                         ce
a Attention + LSTM w/ index:  Attention 뒤에 LSTMS 놓     경우( 성능 저하됨

5 FFN = FeedForward(n_classes, n_classes*4
7 inputs = Input(shape=shape)          #(b,20,5)
8 Q = Dense(hidden_dim, name="Q')(inputs) #(b,2@,9)
9 K = Dense(hidden_dim, name='K’){inputs) #
10 V = Dense(n_classes, name='V')({inputs) #(b,20,5)
11 x = myAttention(Q, K, V)             ib, 20,5)
12 xX = FFN(x)                        #(b, 20,5)
13 x = LSTM(1stm_unit, return_sequences=True){x) #(b,2
x = Flatten()(x)            #(b,20*9)
output = Dense(1){x)         #(b,1)

model = Model(inputs,output)

Min mape:19.09, mse:1.911

28,9

ee)
32
80

Iteration 098 / 100

160 47> Neerinmwetenney:    ~~~ mape       35 7-4                 ~~ 1055
140 4 :             주    ——— Val_mape     30 4 |                   0
1204                            4                              254  }
100                                         :
80                       ee                  t
i  romping hy  =_—, 8    10              Ne
40 + LSTM Layer 학습 진              aes                     」                                            “
36                          fen      =                       NASA
6     20     40    60    80    100        0     20    40    60    80    100
490                                                                                                                                Xx DEEP LEARNING
@한국시연구소 홍근선                    - 245 - 무단 전재, 복제, 24], 디지털화 금지


===== PAGE 246 =====
4부. Attention Based Model                                    4.3 Self-Attention
4.3 Self-Attention Mechanism

m Stacked Self-Attention w/ index : (Self-Attention + FF) x 2

1 hidden_dim = 16 #32
n_classes = x_train.shapef -i]           #5                            iteration 098 / 100
FFNI = FeedForward(n_classes, n_classes*4)
FFN2 = FeedForward(n_classes, n_classes*4)
shape = x_train.shape[i:]            #(28,5)

Loo VI 8 WwW he

Dense(hidden | 이농. name="Q" )( init D, 2€
Dense(hidden dim, name='K")(inputs)i

Dense(n_ classes, name="V")(inputs) |
K(b, 20,5)

Q = Dense(hidden_dim, name="Q2")(x)  sa ie)
K = Dense(hidden dim, name="K2’ )(×)    1
V = 06052(6 6135565, name="V2"){x)    |
5 1X = myAttention(Q, 50400 #¢
= FEN2(x)
= Flatten()(x)
output = 06056(1)(×)
model =  Rides (inputs, output)

pe
6“
x x

Min mape:28.54, mse:4.473
Single Attention
Min mape: 76.43, mse:16.842

tio nmMap 2(Callb
}    nd(self, epoch, logs= 6
if (epoch%2) != @ : return

4       plt.figure(figsize=(16, 8))                              |

5       | attention_mapi = get_activations(model, x_test)[‘attention_weight*] ## |

6       | attention 0301 = tf.reduce sum(attention mapi[:,:,:],axis=1)         |

7       | attention_map2 = get_activations(model, x_test)[‘attention_weight2’] ™

Ey        attention_map2 = tf.reduce_sum(attention_map2[:,:,:],axis=1)            i 어
491                                     Si DEER LEARNING

4.3 Self-Attention Mechanism

m Stacked Self-Attention w/ index : (Self-Attention + FF) x 3

8 inputs = Input (shape= Sse      __# (0; 20,5)                   Iteration 198 / 200

K = Dense(hidden | dim, name=‘K') (inputs)
11 | = Dense(n_| classes, name=‘V" i,

‘Dense( hidden. dim, name='Q2°){x)
Dense{hidden dim, name=  lan! }{x)

= Flatten() (x)

25 output = Dense(1)(x)

26 model = Model(inputs, output)
Min mape:15.84, mse:2.186

"1 00 ~제       =                  …        Min mape:15.84, mse:2.186
re             제          val_mape     내                        val_loss |
125                  Me                     ㆍ                                                 Min mape:28.54, mse:4.473
+                20        을                     1

200 + 바나:                              |      Min mape:76.43, mse:16.842
x               Ya.  _          0                  iy
26                         ha ax       5                            errs

0     50     100     150    200       0      50     100     150    200

@한국시연구소 홍근선                   - 246 - 무단 전재, 복제, S4l, 디지털화 금지



===== PAGE 247 =====
4부. Attention Based Model

4.3 Self-Attention

#(b, 28,5)

8  _inputs = = = Input (shape= eon acl

K = Dense(hidden 010, name='K*) (inputs)
V = Dense(n_classes, name='V')(inputs)
RA myAttention(Q, _ K,  0

fot pak fk fk fd
PWN em Do

= Dense(n_classes, name="V2")(x)

x
[0

15 'K = Dense(hidden dim, name=‘K2" )(x)
16 | 한

Dense(hidden dim, name="K3' 3')00
Dense(n_classes, name="V3‘)(x)
_A = myAttention(Q, K, V,1="3") __
x_A + FFN3(X, A)

24  × = 7 13나아()(00)

oi
25 output = Dense(1)(x)      #(b,1)
, 26 model = Model(inputs, output)

Min mape:38.03, mse:6.884

m Stacked Self-Attention w/ index : (Self-Attention + FF) x 3 + skip connection(half)

Sieg Oy        학습속도 지연
Min mape:38.03, mse:6.884
Min mape:15.84, mse:2.186

20

160 4  ies             -~~ mape

00 리암,   ~ val_mape     =  |.                 ~~ val_loss

=o                Wiha, 6,     14      ae

100       7                  a) nye      3

iG                   f

80      Vay

“            Wil  WW       °

도                     Wh | °                       hu
493      8     50     100    150    200       0     50     100     150    200

OX DEEP LEARNING

_4.3 Self-Attention Mechanism

8 inputs = Input(shape=shape)       #(b,20,5)
| = Dense(hidden_dim, name="6") (inputs) ~~~

!
310 1 = Dense(hidden_dim, name='K") (inputs)
11 ;V = Dense({n_classes, name='V‘)(inputs)      !
12 1× ^ =_myAttention(Q, K, V) _        #(b, 20,5)
a aero 7 a win il     HURT Sil bed ase Bal.
14 x = 60000
15  | 0 = Dense(hiddén dim, name="O2"){xy 1

= Dense(hidden_dim, name='K2‘)(x)
Dense(n_classes, name="V2‘)(x)
i myAttention(Q, Ks, 332 고)

80200 + x
= Dense(hidden dim, name="63")(x) ~
= Dense(hidden_dim, name='K3‘)({x)
Dense{n_classes, name='V3*)(x)
a 하서 0 느메(02 5 050 그 고
제이 기조

1     = FEN3(x) + x

27 x = Flatten(){x)

28 output = Dense(1)(x)   #(D,1) _

* cedtecsieeke Ay

Min mape:54.82

m Stacked Self-Attention w/ index : (Self-Attention + FF) x 3 + skip connection(full)

Add & Norm

29 model = Model(inputs, output)

학습속도 지연                         150
Min mape:54.82, mse:12.209
Min mape:38.03, mse:6.884

i

sins   Nettie:

50 4

. mse:12.209
~~~ mape                           ~~ loss   |
vom val loss |

whee

>  채비  ‘Nal ata i

~——= Val mape |

emacs:

494           내             |                                                                             0              50             100

150                  200

- 247 -

무단 전재, 복제, Sal, 디지털화 금지



===== PAGE 248 =====
Model

4.3 Self-Attention

5

4부. Attention Based

tion Mechanism

mw Stacked Self-Attention w/ index:(Self-Attention + FF)x3 + skip+ Layer_Normalization

& inputs = Input(shape=shape)        #(b, 20,5)

9 1Q = Dense(hidden dim, name="0")(inputs)                                    ‘Add & Norm
16 = Dense(hidden_dim, name='K')(inputs)

11 | = Dense(n_classes, 0ㅁ306='누')(1004+5)

12 |x A = myAttention(Q, K, V)         #(b, 20,5)

13 x = LayerNormalization() (inputs + × ^ )  oe

4 X=            -ion()(FFN1(x) + x )

15 19           m, name='O2°)(x)      7

16 | = Dense(hidden dim, name="K2')(x)        H

17 iV = Dense(n_classes, name='V2")(x)          i

18 [XA = myattention(Q, K, V,1="2") ___#(b,20,5)

19  × = LayerNormalization()(x A+ x }

20 × = Lavernormal ize aon (FEN2(x) + ×) |       eration 198 / 20015

24 10 = Dense(hidden dim, 0306='03')(×)        i

22 1K = Dense(hidden_dim, name="K3')(x)        i
23  iv = Dense(n_classes, name='V3" }{x)          i
24 1x A = myAttention(Q, K, V,1="3") __#(b,20,5)!
25  × = LayerNormalization()(x_A +x )
26 x = Layerlormalization() (FFN3(x) + x )
27 x = Flatten()(x)                #(b, 108)
28 output = Dense(i)(x)               Min mape:31.23, mse:3.961
29__model = Model(inputs,output) 1604. pricy        ~ mape      =  i                i

240  H        가나    val_mape    304 i               나나 vat_foss
3Y23, mse:3.961 ix             ha     mol
Min mape:54.82 mse:12.209        배 itil)              ; *     .  ations
Min mape:38.03, mse:6.884            06   Wy           ia                        hy
'       Min mape:15.84, mse:2.186       6       5               nm
495                                    ㅇ     50    100    150    200      ㅇ     50    200    150    200

If-Attention Mechanism

= Multi Head Attention

Bart |

>

ONG NE

8
6
1 ## Append position code                                      4
2 # concat(x,idx(half_7),x,idx(half_7)):(bs,20,16)              2
3  def idx_value(x) :                                 “a0        30.0 12.5 = 17-5 20.0
4     idx = positional_encoding(length=x.shape[1), depth=14) #(bs,20,14)
5      idx = np.tile(idx, (x.shape[@],1,1))
6     ret = keras.layers.concatenate({x,idx[:,:,:7],x,idx[:,:,7:]],axis=-1)
7     return ret                                     #(bs 26,16)
1 def MultiHeadattention(v,k,g, 1=""):         inum_heads = 2           Multi-Head Attention
2     q = Dense(x dim)(q) # (bs, se      16) | n_classes = x_dim = 16
3      k = Dense(x_dim)(k) (65, 560 100, 16) | depth = 8
4     v = Dense{x_dim)(v) # (bs, 560 160, 16)
5    # split heads:(bs, seq len, 16) -> (bs, 2, seq_len, 8)
6     q = tf.reshape(q, (batch_size, -1, num_heads, depth))
7     9 = tf.transpose(q, perm='@, 2, 1, 3])
8     k = tf.reshape(k, (batch size, -1, num_heads, depth))
9     k = tf.transpose(k, perm=[@, 2, 1, 3])
10    v = tf.reshape(v, (batch_size, -1, num_heads, depth))
il    v = tf.transpose(v, perm=(0, 2, 1, 31)
12     # (bs, 2, 560 1000, 8)
13     scaled_attention = scaled_dot_product_attention(q, k, v, 1)
14     ## (bs, 500 1060 0, 2, 8)
15     scaled_attention = tf.transpose(scaled_ attention, perm=(@, 2, 1, 31)
16     ## (bs, 560 160 0, 16)
17     concat_attention = tf.reshape(scaled_attention,(batch size, -1, x_dim))
318    ## (bs, 560 160 6, 16)
19      output = Dense(x dim) (concat_attention)
20      return output
496                                                                     2      '
@한국시연구소 홍근선                   - 248 - 무단 전재, 복제, 44, 디지털화 금지



===== PAGE 249 =====
4부. Attention Based Model

4.3 Self-Attention

4.3 Self-Attention Mechanism

@ Multi Head Attention(2)

| 12 inputs = Input(shape=shape)       #(b, 28,16)
1   x= inputs
14 batch_size = tf.shape(x)[o]
15 cae “MultiHeadattention(x, x, x) 12111) |
16 i x = LayerNormalization()(x + x_A )      1
17 {x = LayerNormalization()(FFNI(x) +x) |
18 1 × A = MultiHeadAttention(x, x, x, 1="2") |
19 |x = LayerNormalization(}{x + x_A )
20  x = LayerNormalization()(FFN2(x) +x) |
21 | x_A = MultideadAttention(x, x, x, 1="3") |
22 x =   rermrmalietinn sic +X A 1      i
24 X= = Flatten()(x)                #(b, 120)
25 output = Dense(1)(x)            #(b,1)
26 model = Model(inputs, output)

Min mape:4.44, mse:0.160

iteration 198 7 206

1504-1,               aoe MPS      20 4+-4.-4               --- 1055
7                 em Val Mape                            ~—— val_loss
in mape:4.44, mse:0.160 1254   *                                 -
in mape:31.23, mse:3.961 100}  도  !
Min mape:54.82, mse:12.209    3  Ay |                          40
Min mape:38.03, mse:6.884
Min mape:15.84, mse:2.186 3                                   5
25             oe 아아 Bee
;        eat tea       ;          an vas OVE OE
0      50     100     150     200       0      50     100     150     200
497                                                                                                                                                                SE DEEP LEARNING ©

w Bidirectional LSTM ( wo/ index)

| 4 shape=(20,1)
2 units = 9 #46
10045 = Input(shape=shape)
을 =

| 5 × = layers.Bidirectional(LSTM(units,return_sequences=True) ) (inputs)

6 x = Flatten()(x)
| ¥% output = Dense(1)(x)
| 8 00061 = Model(inputs, output)

Layer (type)

Output Shape

Min mape:6.55, mse:0.337
Min mape:4.44, mse:0.160

1)

input_28 (InputLayer)

bidirectional (Bidirectiona

flatten_22 (Flatten)

dense_86 (Dense)

[(Mone, 20, 1)]

(None, 28, 18)

{None, 3

{None, 1

Total params: 1,153
Min mape:6.55, mse:0.337

gents                 --- 00006          4                   am 055

21                  ———- val mape         i                    women Wal loss.
125   4                         za
200 Foy 「                                                     !
734-4                                                  204  i
50    ‘.    me                                5
os      ML                              10 4-4

ot,         .                            25                         +
0       59      100      iso     200        o       50      100      150     200
498                    “sn                                                                                                        Sot DEEP LEARNING
@한국시연구소 홍근선                   - 249 - 무단 전재, 복제, $4, 디지털화 금지


===== PAGE 250 =====
4부. Attention Based Model

4.4 Transformer

Chapter 4, Attention Based Model

4.1 Word Embedding

4.2 Attention Mechanism

4,3 Self-Attention

4.4 Transformer

4.5 GPT: Generative Pre-trained Transformer

DEEP LEARNIN

6106 FOR ¥OU

@ Transformer 개요                        |
® Self-Attention 기반: AJ HA 데이터 처리
®@ Bi-RNN2} 달리 Aj WAS 모든 위치에서 다른 위치의 ASS 참조함
@ Bi-RNNE 순서에 민감하고, Transformer 관계에 민감함
@ Long-term Dependency 문제를 잘 학습함

@ 병렬처리에 유리함                                       일
lam astudent
@ Encoder Decoder model
ㅎㅎ Self-Attention based                RNNILSTM   Tanguage models  16     2
Encoder Decoder             ~ 할    - 도       !       :
N-grams   :   mechanism 1    BERT | GPT-3
a     a i    i
2013 2014 2015    2017 2018 2019 2020   2022
Decoder only
GPT-3
GPT-2
@한국시연구소 홍근선                     -250- 무단 전재, 복제, tall, 디지털화 금지



===== PAGE 251 =====
4부. Attention Based Model

4.4 Transformer

.4 Transf

= Transformer7|#t 주요 모델

® BERT (Bidirectional Encoder Representations from Transformers,’18)
® YSIS self-attentionS 사용하여 FAS 고려한 AMSA (pre-training)S 수

@ GPT(Generative Pre-trained Transformer,’18): auto-regressive model
@ 텍스트를 생성하는 데 SAS = Decoder only 언어 생성 모델
ㅎ 레이어 간의 얄은 양방향 self-attentionS 사용하여 문맥을 이해하며,
@ 사전 훈련된 SHS Fine tuningdtO} 다양한 작업에 적용
® Transformer-XL(’19)
처리하기 위한 모델, 긴 AAA 데이터를 다루는 작업에 특히 유용
@ 상태(51316)를 유지하여 AAAS] 끝 부분까지 정보를 전파함
® XLNet(’19)
 양방향 self-attentionz} permutation language modelingS 결합
/@ BERT} 6『1의 SAS 결합한 형태
@ 다양한41『작업에서성능향상
® 15 (Text-To-Text Transfer Transformer,’19):
@ DSENLP 작업을 HAS 표현하여 SUS! 형태로 OAs 설계
ㅎ 입력과 출력을 통일된 형태로 정의하며, 문제의 종류에 따라 텍스트로 변환되어 학습
@ 다양한 작업에서 효과적으로 활용

So   Zs
@ 긴 문맥을

501

ㅎ SF 끝에서부터 동시에 단어를 이해하는 SAS 사용하여 다양한 자연어 처리 작업에 효과적

8 느

_4.4 Transformer

® Overview

= Attention Is All You Need : 2017.6 “Attention Is All You Need ”,Vaswani

ㅎㅎ Attention mechanism? 사용한 Sequence 모델 제안
/* QNN, CNN 완전 제거

 병렬연산가능 구조, 학습시간 대폭 감소
@ NMT 135(에서 최고의 성능 확인

@ 일반화 가능함 확인
® Architecture overview

Output
Probabilities

[predictions!}
기 4                 Nx
J                        \ [decoder attends          t
M     \teencoder states  4
>           호
t      Te  +
      Positional        Positional
|           |     Encoding        Encoding
input   Output
a a ae) ) 수
Inputs   Ouiputs
{input sequence]                                        [output sequence]                              os                 (shifted right)
SS
@한국시연구소 홍근선      -251- 무단 전재, 복제, al, 디지털화 금지


===== PAGE 252 =====
4부. [60100 Based Model                                     4.4 Transformer

@ Transformer2| 동작

® 동작 개요
@ Input 0213(단어)를 토큰으로 분할 및 embedding vector 생성
 여러 층의 Encoder, DecoderS S4 input data2} output dataS 처리하며, update 진행

@ 2+ Encoder layert Self-Attention 메커니즘과 Feed-Forward Networks 활용하여 입력 문장의 의미를
추출

ㅎ 각 Decoder layer= 다음 HOHE 예측하며 출력 문장을 생성

arrived                                   at                                       the

@ Self-Attention mechanism
@ 입력 데이터 내의 각 SS 간의 상호 BAS 파악하고,            ®               @               e               @
@ 2} 토큰에 대한 가중치를 조절(학습)하여,

@ 입력 데이터 내에서 중요한 정보를 집중적으로 선별하고, ㅣ              .              .             a
@ 이를 다른 토큰과 연결하여 최종적인 의미 표현을 생성 ㅣ 。             '
* 장점, 단점 나은 w2 복수 ge | *    .

® CaF WU GORI BORE Ete       ‘        °        0
@ 기          자연어 이해 등의 분야에서 혁신적인 발전을 주도하고 있음

@  (2a gous Ae aSS 사용량이 500..7^으로 급격하게 증가 /
여사 1809100891.008686 Self-Attention(19) 등에서개선방법제시

= Transformer2| 구조적 특징
@ 순열 SHA (Permutation Invariance)
® Attention mechanism2 £29} 순서     향을 받지 않음
 요약, 번역 등 순서가 중요하지 않은 작업에서 유용
@ 위치 BH4 (Positional Invariance)
® Attention mechanism2 토큰의 절대 위치보다 상대 위치에 BS et
 이미지 인식, 음성 인식 등 토큰의 위치가 중요하지 않은 AAA 유용
* 스케일 불변성 (56316 Invariance)
® Attention mechanism2 A|HA9| 길이에 관계없이 모든 토큰 간의 관계를
A UABAS 처리하는 작업에서 유용
 변환 SHA (Transformation Invariance)

@ Attention mechanisme 입력 Al HAO 대한 다양한 변환을 학습할 + 있음
a 입력 Wench 즈나 왜곡이 있어도 정확한 SHS WHS 수 있음

tb

® CNN CHYLinductive bias7# Fst __ㅎ×     rE n\ A at an.
@ 많은 데이터 BL overfittingo| 적어 일반화 성능 높음
Narra” Nna—_——_-_eeaesesesannax~r,r"
504    에    2          nto             SEe DEEP LEARNING”

@한국시연구소 홍근선                   - 252 - 무단 전재, 복제, S4l, 디지털화 금지



===== PAGE 253 =====
4부. Attention Based Model

4.4 Transformer

4.4 Transforme

m 2H Inductive bias7} 약한가?
@ Attention mechanism £3) arate 2]. Po

ㅎ CNN& data9| LocalityS 전제 함
ㅎㅎ RNN& data} SequentialityS 전제 함

® Positional Encoding
@ 토큰의 절대적인 위치보다는 상대적인 위치에 더 집중
@ 모델이 데이터의 순서에 대한 사전 가정을 하지 않음

mw 약한 Inductive bias2| 효과
* 새로운 데이터에 대한 일반화 성능 향상이 가능
* 다양한 데이터 형식에 대한 적용 가능
@ 이미지, 텍스트, 음성 등 다양한 데이터 형식에 적용가능

@ 모델이특            형식에 대한 사전 가정을 하지 않음
© 단점: 많은 양의 데이터 필요, 학습이 효율적이지 않음
eae

|,
@ 데이터의 특성에 대한 사전 가정 없이 모든 토큰 간의 관계를

a 작한 .
직접 학습

일 DEEP LEARNING .
Bobet BB tO ROM.

= Multi-Head Attention
 다수의 Attention head=
@ 서로 다른 부분에 집중
~ “it?0| “the animal’2}
“tired” Ol] 집중하고 있음
f 그 밖의 단어 들과도
복잡하게 연관되어 있음

(seq, Xaim)

| Value Layer |  Key Layer  ㅣ 이오 Layer |

Vv

0
 (seq, Xaim)

Layer:| 5 $ Attention:' input - input 수           “Layer: 5 수 Attention: | Input-Input — $
animal_ abe
didn_
=
cross_
the_
street_
개   because_
>
- \25
me          too_
tire
o                                                            8_
506
@한국시연구소 홍근선                  - 253 - 무단 전재, 복제, 244i), 디지털화 금지



===== PAGE 254 =====
4부. Attention Based Model                                       4.4 Transformer

® Architecture overview                     —          Output aem='s42
w/ skip-conn. (1)              Probabilities
0                                                          i
Attention(Q, KV) = si     ie Ww                                      한)
Vd                                                                                                        pean
Scaled Dot-Product Attention                                                                                       ea!                Attention

해 케샤 fs 제재 9

were                                                          ost ional     distance
Encoding Or BO  — — GOL staae=:

Inputs
X: (seq, 512)
| 607       oe) 2018.11 “Visualizing the Loss Landscape of Neural Nets”   Sof DEEP LEARNING ©
1

Positional encoding : concatenate([sin(angle),cos(angle)])

Ai def positional encoding(length, depth):          # (560 160, 512)
2    depth = depth/2
3    positions = np.arange(length)[:, np.newaxis] # (seq_len, 1): 0 ~ 560 100
4     depths = np.arange(depth)[np.newaxis, :]/depth # (1, 256): @~ 1
5.                 -
6   angle rates = 1 / (10000**depths)           # (1, 256): 1 ~ 1/(10000)
더    80816 『805 = positions * angle rates           # (seq_len, 256)
8
9    pos encoding = np.concatenate([np.sin(angle rads), np.cos(angle rads)], axis=-1)

10   return tf.cast(pos_ encoding, dtype=tf.float32) #(seq_len, 512)

1 pos_encoding = positional_encoding(length=2048, depth=512) |
2  print(pos_encoding. shape)                           |
3 plt.figure(figsize=(12,6))
4 plt.pcolormesh(pos encoding.numpy().T, cmap='RdBu’ )

106

( sinci/100002°1/4) )
cos(i/100007°3/4) |
.            i

i

i

Dj

ig tt:     t
sin(i/10000°°2/¢) i
_cos(i/100007°2"*) ,

Dimension

pe a se  OSES Uae RO see             Paella ks ea
508              :        1000   1250   1     750   2      "   o       iii    Sf DEEP LEARNING

Position

@한국시연구소 홍근선                    - 254 - 무단 전재, 복제, Sail, 디지털화 금지



===== PAGE 255 =====
4부. Attention Based Model                                       4.4 Transformer

Positional

@ Positional Embedding = Word Embedding + Positional Encoding         Encoding
1 class Positionalfmbedding(tf.keras.layers.Layer):
2    def init__(self, vocab_size, d_model):
3      super().__init_()
4      self.d_model = 0 model                                                 Inputs
5      self.embedding = tf.keras.layers.Embedding(vocab_size, d model, mask_zero=True)
6      self.pos_encoding = positional_encoding({length=2048, depth=d_ model)
(별
8    def compute_mask(self, *args, **kwargs):
9      return self.embedding.compute_mask(*args, **kwargs)
16
11    def call(self, x):
12      length = tf.shape(x)[2]
13      x = self.embedding(x)
14      # This factor sets the relative scale of the embedding and positonal_ encoding.
15      x *= tf.math.sqrt(tf.cast(self.d_model, tf.float32))
16      x = x + self.pos_encoding[tf.newaxis, :length, :]
17       return x

 그 밖의 Positional Encoding 방법
® Learned Positional Encoding: 정확하지만, 학습 과정이 더 복잡함 (GPT 3에서 적용)
 학습 과정에서 모델이 직접 위치 정보를 학습, 학습 데이터의 길이에 제한이 없음
®@ Rotary Positional Encoding: Sinusoidal + Learned Positional Encoding
& 간단하고 효율적이며, 학습 데이터의 길이에 제한이 없음
ㅎ Sparse Attention: 주변 토큰 간의 관계만 고려, Positional ㄷㅁㅇ00109필요없음

_509

@ Scaled dot-product Attention for Multi-Head Attention

for self-Att. K, Q, V from same source                                                                             “T
q =x*W14 = dense(w1)(x) ,k= ...,v= ..                   Attention(Q, K,V) = softmax(         yv
vai.
1 def scaled_dot_product_attention(q, k, v, mask):                   - (bs, heads, seq len, Vaim/h)
2      # q: query shape == (bs, num_heads, seq_len_q, v_dim/h)
3      # k: key shape == (..., seq_len_k, v_dim/h)
4      # v: value shape == (..., seq_len_v, depth _v)
5      # mask: mask shape == (bs, 1, 1, seq len_k). Defaults to None.
6
ry    # (..., 560 160 04, seq len _k)
8    matmul_gk = tf.matmul(q, k, transpose b=True)
9

18    # scale mataul qk
11    dk = tf.cast(tf.shape(k)[-1], tf.float32)
12 scaled_att_logits = matmul_qk / tf.math.sqrt(dk)

14 | # add the mask to the scaled tensor.

15    if mask is not None:

16      scaled_att_logits += (mask * -1e9)                              Q    K    V
17                                                                          (bs, heads, seq len, Vaim/h)
18    # softmax is normalized on the seq len_k. (..., 500 100 0, seq len_k)

19    att_weights = tf.nn.softmax(scaled_att_logits, axis=-1)              ㅣ

20

21 output = tf.matmul(att_weights, v) # (..., 560 160 0, depth v)
22 ~~ ~return output, att_weights

@한국시연구소 S24                   - 255 - 무단 전재, 복제, Si, 디지털화 금지


===== PAGE 256 =====
4부. Attention Based Model                                       4.4 Transformer
                                                                                      :

® Multi-Head Attention : Self-Att.Uj 병렬처리 > self-Att gS 병렬처리         Multi-Head Attention

@ dnoaeidim(512)S 얻기 위해 single attention||A] d,dim 한번에 처리 보다,
개의 single attentiong 병렬로 처리         @.0871/8,개를 얻는 것이 좋음

@ 논문에서 4 = 8, dy = 0, = 4 64
D> AMS 비슷하고, 속도는 빠르고, 64559 attention weight 학습
@ 결과값은 60ㅁㅇ8『.해서 0「01601010 > 0,,,,2070171(512) vector 출력
MultiHead(Q, K, 7) = Concat(head,, ..., head;,)W 0
where head; = Attention(QW?, KW ,vw’)

Head?
we K=KWE Vv =v!           1 ow
Sottmax ㅣ 개스: ㆍ 리
수
adj = A(Q,.K,V) 0 (6=10)    |         |         |
"        Qn a Boe ae 비  ‘
[head,, head», ..., head), |                         t                            '                            ;
Multi-Head       :                                       :
Attention                Multi ead(Q, K, 7)                                                                                                              |

@ Multi-Head Attention(1)

Multi-Head Attention
1 class MultiHeadAttention(tf.keras.layers.Layer):
2   def init__(self, d_model, num heads):
3     super(MultiHeadAttention, self). init__()
4     self.num_heads = num_heads          #8
5     self.d_model = 0 00061              # 512
6     self.depth = d_model // self.num_heads # 64
Zz   ‘
8      self.wq = tf.keras.layers.Dense(d_model)
9      self.wk = tf.keras.layers.Dense(d_model)
10      self.wv = tf.keras.layers.Dense(d_model)
41      self.dense = tf.keras.layers.Dense(d_model)
12
13 ~ def split_heads(self, x, batch_size):
14    # (bs, seq_len, 512) -> (bs, 8, seq len, 64)
45    x = tf.reshape(x, (batch_size, -1, self.num_heads, self.depth))
16     return tf.transpose(x, perm=[@, 2, 1, 3])               i

A

@한국시연구소 홍근선                   - 256 - 무단 전재, 복제, 24, 디지털화 금지

이 이                 ee       =                              id ee   ARNING™



===== PAGE 257 =====
4부. Attention Based Model

4.4 Transformer

@ Multi-Head Attention(2)

head; = A(Q, KV) @=1..h)

= QW? K=KWS ee

18 def call(self, v, k, q, mask):                  수
19       batch_size = tf.shape(q)[e]                          ($€4,Vaim)                A
20    9 = self.wq(q) # (bs, seq len, 512)             =e  [head,, heads,  .0680610
21     k = self.wk(k) # (bs, 560 160, 512)        sunken OR ater
ultiHead(Q, K,V)
22      v = self.wv(v) # (bs, seq len, 512)            Attention
23      q = self.split_heads(q, batch_size) # (bs, 8, 500 100 04, 64)
24       k = self.split_heads(k, batch_size) # (65, 8, seq _len_k, 64)
25       v = self.split_heads(v, batch_size) # (bs, 8, seq_len_v, 64)
26
27       # scaled_attention.shape == (bs, 8, seq 160 0, 64)
28      # attention_weights.shape == (bs, 8, 560 160 0, seq _len_k)
29       scaled_attention, attention_weights = scaled_dot_product_attention(
30           9, <, v, mask)
31
32      ## (bs, 560 1600 0, 8, 64)
33      scaled_attention = tf.transpose(scaled_attention, perm=[9, 2, 1, 3])
34
35      ## (bs, seq_len_gq, 512)
36       concat_attention = tf.reshape(scaled attention,
37                                    (batch_size, -1, self.d_model))
38       ## (bs, 560 100 0, 512)
39       output = self.dense(concat_attention)
40       return output, attention_weights
513                                                ~               eee

@ GlobalSelfAttention: Encoder] At+2 2 Self-Attention layer
® Multi-Head Att. + Layer Norm. + Skip-connection

1

Wm WR

a

class BaseAttention(tf.keras. layers.Layer):

| def init__(self, **kwargs):

i   super().__init__()

|   self.mha = tf.keras. layers.MultiHeadAttention(**kwargs)
ㅣ   self.layernorm = tf.keras.layers.LayerNormalization()

| self.add = tf. keras.layers.Add()

Wd ND et

won Ou &

class GlobalSelfAttention(BaseAttention):
06 call(self,  ae

바바

x = self.add([x, attn_output])
x = self. layernorm(x)
return x

Key, Value

oO 나 & whe we

pt_emb = tf.random.uniform((64, 72, 512))

sample_gsa = GlobalSelfAttention(num_heads=2, key_dim=512)

print(pt_emb.shape)                 (64, 72, 512)

print(sample_gsa(pt_emb).shape)     (64, 72, 512)

- XK DEEP LEARNING ”

@한국시연구소 홍근선       - 257- 무단 전재, 복제, wal, 디지털화 금지


===== PAGE 258 =====
4부. Attention Based Model                                       4.4 Transformer

@ Causal SelfAttention: Decoder] 사용할 Self-Attention layer

@ UDA (causal): 출력 seq. 이전 출력 560.에 의존함  ，
ㅎ Single-directional RNN& 동작이 인과적(이전출력에 의존)
ㅎ Self-       100은 maskS 작용하여 이전에 의존하게 해이

10           return x

1 class CausalsSelfattention(BaseAttention):      nik, 감개
def call(self, x):
attn_output = self.mha(                       ×.
query=x,                                    .
value=x,
key=x,
use causal mask = _True)##
3     x = self.add([x, attn_output])
9      x = self.layernorm(x)

wt ON WI Be oe

Key, Value
Attention
weights

sample csa = CausalSelfAttention(num heads=2, key _dim=512)

ps(en_emb)                #(64,94,512)                                        「
ps(sample_csa(en_emb))#(64,94,512)

@ | re

출력은 이전 요소에 의존하므로 요소를 자르는 것은 영향이 없음

outi
out2

sample _csa(embed en(en[:, :3])) #(64,3,512)
sample_csa(embed_en(en))[:, :3] #(64,3,512)

1 ㅣ

매지 bet

tf.reduce max(abs(out1 - out2)).numpy()#4.7683716e-07

RE

re    t              4.  jot mo
Add & Norm 1) ae          |
Feed                  iL__ Attention           '
Forward                | RH                   !
:                           [ieceee                 시
Encoder                          Decoder

# Seq2Seq229| attention 동작을 모방
@ Q: from decoder, * K, V: form encoder
@ Decoder] queryOl] 대한 답을 찾기 위해 encoder2] K, VB 사용하는 것

/ Attention 식이 : output = softmax(XQ(XK)") x XV,

/＊ Z(Decoder 4), H(Encoder 출력) 이라면

/ Cross-Attention 42: output = softmax(ZQ(HK)") x HV

/* Z:(Dseq,dV-dim), H:(Eseq,eV-dim) > (seq, model-dim)

( Dseq = Eseq = ModelSeq, dV-dim = eV-dim = model-dim = 512 )
® Decoder= 6개의 230] stack,
Enc.-Dec. Cross-Attention= 641 수행 =

516

~   a  He DERE LEARNING”

@한국시연구소 홍근선                    -258- 무단 전재, 복제, Sal], 디지털화 금지



===== PAGE 259 =====
4부. Attention Based Model                                     4.4 Transformer

® CrossAttention Layer: Decoder0l] 42 Attention layer
®@ Multi-Head Att.(Q,(K,V)) + Layer Norm. + Skip-connection

1 class CrossAttention(BaseAttention):

2    def call(self, x, context):

3    fattn_output, attn_scores = self.mha( |

4     !    query=x,      He              |

5     i    key=context,  ##              H

6     :    value=context, ##             !

7      1. . 16640. 8타 60100 560065=1[046)|

8      # Cache the attention scores for plotting later.
9      self.last_attn_scores = attn_scores

18     x = self.add([x, attn_output])
11      x = self. layernorm(x)

2      return x

1 sample_ca = CrossAttention(num_heads=2, key _dim=512)

2

3 ps(pt_emb)             #(bs, s, dim):(64,72,512)
4  ps(en_emb)              #(bs, t, dim):(64,94,512)
5  ps(sample_ca(en_emb, pt_emb))#(bs, t, dim):(64,94,512)

ㆍ 출력 560. ZO|E query 560. 길이로 AAS
$ㅎ Query 각 pointe 모든 (6, value= 참고함
＊ 그러나 Query 각 00101간에 정보가 공유되지 않음

© Feed Forward Network ( Position-wise Feed-Forward Network )

® Position-wise : Attention 24 (seq, v-dim)S 처리 _ 1? : Mulloy er - 때

@® FFN(x) = ReLU(xW1 + b1)W2+b2

FFN(x) : dense(n)( dens( n, ’relu’)(x) )          |   1   aaa a   as
® Layer normalization                               |
@ 동일한 Layer node 42 Normalization                                    —_               : 에
@ 각ㅁ006의 계산 값을                                                             |
norm. > + bias > activation()                              200      “Wes
> 학습속도 증가 ( 알 수 없는 변동성 낮아짐 ) 요 es 이             (Rage 102
+              suis            étudiant             ae                               mae

bg     :                        t
|        Self-Attention

Encoder #1
| Sey stection                                                    :
Feed    Feedforward    Feediorward    Feedforward           ]   8 |   tod     |
forward          neural network           neutal network            peural network                                                                                                                                                               _—
ㅣ         ㅣ         |                                        Input
works   otra ot ee                                  Embedding
ee oe
:         ‘         ‘                                        Inputs
518        Ref.: 2019, “Understanding and Improving Layer Normalization «SOR DEEP LEARNING ©

@한국시연구소 홍근선                     -259- 무단 전재, 복제, wai], 디지털화 금ㅅ


===== PAGE 260 =====
4부. Attention Based Model

4.4 Transformer

|.

@ Feed Forward Network ( Position-wise Feed-Forward Network )

1 class FeedForward(tt.keras.layers.Layer):

2   def init__(self, d_model, dff, dropout_rate=0.1):

3             super().__init__()

4      self.ff = tf.keras.Sequential([

5      tf.keras.layers.Dense(dff, activation='relu'), # 2048

6        tf.keras. layers .Dense(d_model),               # 512

고                    tf.keras. layers .Dropout(dropout_rate)

8      ])

9      self.add = tf.keras.layers.Add()

16               self.layer_norm = tf.keras.layers.LayerNormalization()

ga

12   def call(self, x): #(bs, seq_len, 512)             T

13    | x = self.add([x, self.ff(x)])                  |

14    | x = self.layer_norm(x)

15   | return x #(bs, seq len, 512)

2 sample ffn = FeedForward(512, 2048)

2

3 ps(en_emb)           #(64, 84,512)                                :
4  ps(sample_ffn(en_emb))#(64,84,512)               d   = :
1 ps(sample ffn.get_weights()[e]) #(512,2048)                    6
2  ps(sample ffn.get_weights()[2]) #(2048,512)

519

@ Encoder layer
® GlobalSelfAttention + Feed Forward Network

1 class EncoderLayer(tf.keras.layers.Layer):
2   def __init__(self,*, d_model, num_heads, dff, dropout_rate=0.1):
3      super().__init__()                                                ~
4
5      self.self_attention = GlobalSelfaAttention(
6          num_heads=num_heads,                                         Feed
7          key dim=d_model,                                            =
8         dropout=dropout_rate)
본                                                                      Nom
10     self.ffn = FeedForward(d_model, dff)                          Muli Head
fa                                                                   Attention
12    def call(self, x):
13      x = self.self_attention(x)                                 ae
14      x = self. ffn(x)
15      return x
1 sample encoder layer = EncoderLayer(d_model=512, num_heads=8, dff=2048)
2
3 ps(pt_emb)                    #(64,87,512)
4 ps(sample_encoder_layer(pt_emb) )#(64,87,512)
한국시연구소 S24                   - 260 - 무단 전재, 복제, Bl, 디지털화 금지



===== PAGE 261 =====
4부. Attention Based Model

4.4 Transformer

© Encoder Block layer

—

11      self.dropout = tf.keras.layers.Dropout(dropout_rate)

13    def cali(self, x):
14     # “x is token-IDs shape: (batch, seq len)

16       # Add dropout.

17       x = self.dropout(x)

18    _ for i in range(self.num_layers):

i9       x = self.enc_layers[i](x)

20     return x # Shape (batch 5126, 500 160, 0 00001) .

1 class Encoder(tf.keras.layers.Layer):

2    def init__(self, *, num_layers, 0 00061, num_heads,

3             dff, vocab_size, dropout_rate=@.1):

4       super().__init__©

5      self.d_model = d_model

6       self.num_layers = num_layers

7       self.pos_embedding = PositionalEmbedding(

8          vocab_size=vocab_size, d_model=d_model)

9       self.enc_layers = [EncoderLayer(d_model=d_model, num_heads=num heads,
10                        720, dropout_rate=dropout_rate) for Ie

in range( num_layers) ]

15     x = self.pos_embedding(x) # Shape “(batch 5120, seq len, 0 00001).

sample_encoder = Encoder(num_layers=4, d_model=512,
num_heads=8, dff=2048, vocab_size=850@)
sample_encoder_output = sample _encoder(pt, training=False)
# Print the shape.
ps(pt)                   #(64,87)
ps(sample encoder_output)#(64,387,512)

wi WT fh Wo NM

Positional

En

@ Decoder Layer

1 class DecoderLayer(tf.keras.layers.Layer):

2    def init__(self, *, 0 00061, num_heads, dff, dropout_rate=0.1):

3      super(DecoderLayer, self). init ()

4      self.causal_self_ attention = CausalselfAttention(

5          num_heads=num_heads, key_dim=d_ model, dropout=dropout_rate)

6      self.cross_attention = CrossAttention(

7          num_heads=num_heads, key 010=0 00061, dropout=dropout_rate)

8       self.ffn = Feedforward(d_ model, dff)

9
10    def cali(self, x, context):
331       x = self.causal_self_attention(x=x)
12       x = self.cross_attention(x=x, context=context)
13      # Cache the last attention scores for plotting later

14       self .last_attn scores = self.cross_attention.last_attn scores
15      x = self.ffn{x) # Shape “(batch_size, seq_len, 0 model).
16      return x

1 sample_decoder_layer = DecoderLayer(d_model=512, num_heads=8, dff=2048)
2

3 sample_decoder_layer_output = sample_decoder_layer(

4      x=en_emb, context=pt_emb)

5

6 ps(en_emb)                     #(64,84,512)

7 ps(pt_emb)                     #(64,87,512)

8 _ps(sample decoder_layer_output)#(64,34,512)

522          on         :            —                 Ok DEEP LEARNING
@한국시연구소 홍근선                  - 261 - 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 262 =====
4부. Attention Based Model                                       4.4 Transformer

@ Decoder Block Layer
4 class Decoder(tf.keras.layers.Layer):
교   def init__(self, *, num_layers, 0 00061, num_heads, dff, vocab_size,
3                                dropout_rate=0.1):
4     super(Decoder, 5637). init_()
5      self.d_model = d_model
6      self.num_layers = num_layers
7         self.pos_embedding = PositionalEmbedding(vocab_size=vocab_size,
a                                           d_model=d_model)
2             self.dropout = tf.keras.layers.Dropout (dropout_rate)
18      self.dec_layers = [DecoderLayer(d_model=d_model, num_heads=num_heads,
호          dff=dff, dropout_rate=dropout_rate) for _ in range(num layers)]
12      self.last_attn_scores = None
13
14   def call(self, x, context):
16   | # x is token-IDs : (batch, target_seq_len)                              J
16     x = self.pos embedding(x) # (batch 5126, target_seq_len, d_model)              Positional
317      x = self.dropout(x)                                                          Encoding
18     for i in range(self.num_layers):
39      x = self.dec_layers[i](x, context)
20     self.last_attn_scores = self.dec layers[-1].last_attn scores
23      return x #(batch_size, target_seq_ len, 0 00061)
1 # Instantiate the decoder.
2 sample decoder = Decoder(num_layers=4, d_model=5i2,num_heads=8, dff=2648, vocab_size=se0¢)
3 output = sample decoder(x=en, context=pt_emb)
4
5  # Print the shapes.
6 ps{en)    #(64,84)
7  ps(pt_emb)#(64,87,512)
8 ps{output)#(64,84,512)
523

® Transformer Model

1 class Transformer (tf. keras.Model):

2   def init__(self, *, num_layers, d_model, num_heads, dff,

3                    input_vocab_size, target_vocab_size, dropout_rate=0.1):

4      super().__init__()

5     self.encoder = Encoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads,

6                      dff=dff, vocab _size=input_vocab_size, dropout_rate=dropout_rate)
7     self.decoder = Decoder(num_layers=num_layers, d_model=d_model, num_heads=num_heads,

8                     dff=dff, vocab_size=target_vocab_size, dropout_rate=dropout_rate)
9              self.final_layer = tf.keras.layers.Dense(target_vocab_size)

10

11    def cali({self, inputs):

42   | context, x = inputs

13    _ context = self.encoder(context)#(bs, context_len, d_model)

14   | x = self.decoder(x, context)  #(bs, target len, d model)

45   | logits = self.final_layer(x) #(bs, target_len, target_vocab_size)
16    | # Return the final output and the attention weights.

47    __return logits

1  transformer = Transformer(               Total params: 10,184,162
f                                         °   1   2

고     num_layers=num_layers, #4 4

3      d_model=d_ model,      # 128

4      num_heads=num_ heads, # 8

5      dff=dff,              # 512

6              input_vocab_size=tokenizers.pt.get_vocab_size().numpy(),

Zz             target_vocab_size=tokenizers.en.get_vocab_size().numpy(),

8     dropout_rate=dropout_rate) # 9.1

1 output = transformer((pt, en))

2 ps(en)     #(64,84)

3 ps(pt)     #(64 87)            .                                         _
4 ps(output) #(64,84,7010)                      ‘             aaa  SK DEEP TEARR Libr

@한국시연구소 홍근선                  - 262 - 무단 전재, 복제, Si, 디지털화 금지



===== PAGE 263 =====
4부. Attention Based Model

4.4 Transformer

© Transformer Model

Output
Probabilities

Positional  602 5                        mee)  Positional
Encoding                                   q           Encoding
Inputs                Outputs

(shifted right)

Sho DEEP LEARNING”

고소 686 + 본  om

1 class CustomSchedule(tf.keras.optimizers.schedules.LearningRateschedule):
2   def init__(self, d_model, warmup_steps=400e):
3   | super(CustomSchedule, self). init ()
4    |                                               00014    \
1
5    |  self.d_model = d_model                           매기
6      self.d_model = tf.cast(self.d_ model, tf.float32)    . 0000     내
7                                                                                  로 00008     i         a
8      self.warmup steps = warmup_steps                  은 00006   |         Sin
9                                                                                                                   아버
10   def 6811 (self, step):                     fone  ;
11     step = tf.cast(step, tf.float32)                 ey
12     argi = tf.math.rsqrt(step)                       00001
13     arg2 = step * (self.warmup_steps ** -1.5)               900 30000 55000 ee 3006 조매치 80002
14
15     return tf.math.rsqrt(self.d_model) * tf.math.minimum(argi, arg2)
1 learning rate = CustomSchedule(d_model)
2
3 optimizer = tf.keras.optimizers.Adam(learning rate, beta_1=0.9, beta_2=0.93,
4                                  epsilon=ie-9)
i temp_learning rate_schedule = CustomSchedule(d_model)
2
3. plt.plot(temp_learning rate_schedule(tf.range(4geee, dtype=tf.float32)))
Ｌ 526                                                     개 마타 telat
re]                          =    ie               바츠       Ss.
@한국시연구소 홍근선                     263        ct 전재, 복제, 24, 디지털화 금지


===== PAGE 264 =====
4부. Attention Based Model                                       4.4 Transformer

@ Masked_loss, Masked_acc : 길이가 C}e2 2 custom 함수 필요
1 def masked _loss(label, pred):
2 _ mask = label != 0
3          loss_object = tf.keras.losses.SparseCategoricalCcrossentropy(
4     from_logits=True, reduction=‘none')
5    loss = loss_object({label, pred)
6
7    mask = tf.cast(mask, dtype=loss.dtype)
8 00 Loss_*= mask
9
16    loss = tf.reduce_sum(loss)/tf.reduce_sum({mask)
11    return loss
12
13 def masked_accuracy(label, pred):
14    pred = tf.argmax(pred, axis=2)
15    label = tf.cast(label, pred.dtype)
16    matched = label == pred
17
18    mask = label != 0
19 | matched = matched & mask
20
21    matched = tf.cast(matched, dtype=tf.float32)
22    mask = tf.cast(mask, dtype=tf.float32)
23    return tf.reduce_sum(matched)/tf.reduce sum(mask)

® Training

1. transformer .compile(

2         : loss=masked_loss,

3               optimizer=optimizer,

4               metrics=[masked_accuracy])

2. transformer.fit(train_batches,
3                                    epochs=2¢,
4                                    validation_data=val_batches)

® Inference

| 1 translator = Translator(tokenizers, transformer)

|

sentence = ‘os meus vizinhos ouviram sobre esta ideia.‘
ground_truth = ‘and my neighboring homes heard about this idea .'

translated text, translated tokens, attention weights = translator(
tf.constant (sentence))
print_translation(sentence, translated text, ground truth)

TMP wh 하

Input:        : OS meus vizinhos ouviram sobre esta ideia.
Prediction      : my neighbors heard of this idea .
Ground truth   : and my neighboring homes heard about this idea .

def print_translation(sentence, tokens, ground truth):
print(f’{“Input:":15s}: {sentence}‘)
print(f‘{°Prediction":15s}: {tokens .numpy().decode(“utf-8")}")

1
2
3
4     print(¢‘{"Ground truth":15s}: {ground truth}‘)

한국시연구소 홍근선                     - 264 - 무단 전재, 복제, 44, 디지털화 금지



===== PAGE 265 =====
4부. Attention Based Model                                     4.4 Transformer

4 Transformer

© Translator

class Translator(tf Module):
def init__(self, tekenizers, transformer):

self.tokenizers = tokenizers

4      self.transformer = transformer
5   def call (self, sentence, max_length=MAX_TOKENS):
6     # The input sentence is Portuguese, hence adding the [51481]. and “[END]” tokens.
7     if len(sentence.shape) == @: sentence = sentence[tf.newaxis] #(1,)<-()
a      sentence = self.tokenizers.pt.tokenize(sentence).to_tensor()
9     encoder_input = sentence
16
a1      start_end = self.tokenizers.en. eerie ot. #(2,)<-(4, none)
a2     start = start_end[o][tf.newaxis] #(1,    = [START]
13     end = start_end[i][tf.newaxis]   eeu  = [END]
14
15     # tf. Tensorarray : instead of a Python list
16     애나 arc = tf. Tensorarray(dtype=tf. intea, size=0, dynamic_size=True)
17      output_array = output_array.write(9, start)
ia     for 4 in tf. sanme max Tenement
SuepUL — Ef teanspaseCoutput array ateckes5
=  otter isipiut , 셔재즈저치적 3  spatipud ep Ad aul cop ask see)
predictions = prediccionsl:. 25, 3] # Cbs tase toner velos.
Predicted ia - tr aremantpreaicticas, Bxtal 15
SUtpEt Srreay = output array weiteciek, prealeted 1dfe1>
i¥ predicted ta ~~ and:

28     output = tf.transpose(output_array.stack()) #(1,tokens):[[13 23 234 ...
29     text = tokenizers.en.detokenize(output}[@] #(): 615다61305 300... 1
38        tokens = tokenizers.en.lookup(output)[9]     #(tokens,):[b’ [START] b'scholars',...]
32     # attention_weight   얻기위해 한번터 Bact. function® 방해)
33     self. transformer([encoder : input, output[:,:-1]], training=False)
34     attention_weights = self.transformer.decoder.last_attn_scores
529 | 36     return text, tokens, attention weights

11

4.4 Transformer

© Translator(2)

19    |  for i in tf.range(max_length):

28    i   output = tf.transpose(output_array.stack(})

21   ㅣ   predictions = self.transformer([encoder_input, output], training=False)
22    i   predictions = predictions[:, -i:, :] # (bs,last_token,7e10)"

23    |   predicted 10 = tf. ane pees, axis=-i)}

24    ㅣ   output_array = output_array.write({i+i, predicted_id[9])

25    :   if predicted_id == end:

26    /     break

® 43601 plot : 8개 headoll 있 QI= attention weight plot

“Sif DEEP LEARNING

-265- 무단 전재, 복제,

0 Lo

sal, 디지털화 금지


===== PAGE 266 =====
4부. Attention Based Model                                       4.4 Transformer

※ 주요 A2:Longer Context 중심

[Vanilla Transformer ]
= Longer Context :500가 늘면: AlZH2 O(L2d) memoryE 002)로증가“ 。 “^
® Context fragmentation: context2| 정보가 분리          22 a” ~
@ 긴 00016짜의 경우 char 개수로 분리되어 정보의 단절이 발생       220
= Context Memory (or Context-dependent Memory)     eS 55 £228
Segment1     Segment2

@® Transformer-XL(2019)

® segment level recurrence mechanism: 세그먼트 간의 상태를 저장, 재사용

(a) Training phase.                  ：                                           (b) Evaluation phase.
0 0 0 010    @|6 000099 © 0 0

6 0 0 0 9 0

e@|o © oo 06 0

" Fized(lie Grad) "ee Semmes                 Fixed(No Grad)   New Segment                  Extended Context
® Relative Position Encoding: 학습 가능한 상대 위치 표현을 사용
® Compressive Transformer(2019)      - — ge 0        sie
® Transformer-XL 확장                      os       died   ee 00000 6606

® memoy4#S 압축한 memorsS 추가                        0 00000 000

+ + + t

= Non-Differentiable External Memory
® K-NN-LM(2019)
@ LM 예측과 KNN OSS 선형 결합 p(y) = A puewn(y|x) + (1 — A) pr (y|x)
® KkNN model: (LM embedding representation of context, next token) HOS 전처리 되었음

LMSC} 더 3 dataseto= SH
AESe 조조느~
@ SPALM(Adaptive Semiparametric LM)(2021) =”      ae                                     \

® Short-term memory: Transformer-XL style memory
+ Long-term memory: kKNN-LM style memory

@ 현재 context= kNNS 검색하여 관련성이 높은
(개의 token2| embedding representation 확보
(representation: pretrained LM = 준비된)

@ 0, :현재의 상태 /?와 7<;의 선형결합 계수(학습됨)

long-term memory aggregate
¢                                            om
{yi iE t=1    ㆍ

| retrieve

|
ㅣ
ㅣ
|
|
|
ㅣ

|투루투루| |뿌무투

i
i
1
'
ㅣ
1
1
i
ㅣ

tt-2          aad

ee    ne   "        할 DEEP LEARNING |
한국씨연구소 홍근선         -266- 무단 전재, 복제, esi, 디지털화 금지



===== PAGE 267 =====
4.4 Transformer

= Non-Differentiable External Memory(2)
『 0 _ Transformers(2022)

@ 약간의 변경으로 memoryS 262k token = 확장
@ kNN-augmented attention layer 사용(마지막 layer?20]])

- 추가적으로 외부 memoryOlA k-nearest-neighbor search 수행 삐 된
@ KNN search
|         softmax

- local attention2z} 동일한 query 사용
- 최근에 사용된 key, value pairS 대상으로                                          |       local attention + FFN
- ZF query 개의 근접한 key, value#tS 반환
00 — augmented attention layer... -  "eras
ae

i
i
:
i
i
i

we

© ENN attention          Ses _extemal pur sastie ore 006  i Aad:
- (개의 query, key, value attention 실행
® Combine (kNN attention + Local attention)
- learned gate= 결합
@ External memory(FIFO)
- local attention2| key valueztS 저장
: a key. y, value normalize 적용: distribution 5111[방지

= Low-Rank Attention
@ Linformer(2020)

®@ Attention matrix low-rank matrix= 근사하여,
시간과 공간 복잡성을 선형적으로 감소

@ Key, ValueO projection layers 추가하여
/ Attention memory2A: Lxd ~k xd, k«KL

Linformer                  x)
we (WY)

a

kxn                   dm X dy

nkda                           120 + …… Linformer, k=2048
~ Linformer, k=1024
—#— Linformer, k=512
- Linformer, k=256
wow Linformer, k=128
~e- Transformer

/* 관계를 9000!6하게

1]

just                                 just                           512/128 1024/64 2048/32 4096/16 8192/8 16384/4 32768/2 65536/1
Sequencelength/  / batch size

3                                                           “Re DEEP LEARNING
@한국시연구소 홍근선                      -267- 무단 전재, 복제, Yl], 디지털화 금지



===== PAGE 268 =====
4부. Attention Based Model                                       4.4 Transformer

실습 : https://keras.io/examples/audio/transformer_asr/

Automatic Speech Recognition with

Transformer

Author: Apoorv Nandan                                  ‘                                 Dataset = 3.660

Date created: 2021/01/13                      4 Vy,             Training : 3시간                            4

Last modified: 2021/01/13                           지소                                        @           svt went a
te       C  rahe.

co ViewinColab + ©) GitHub source

(2L
Description: Training a sequence-to-sequence Transformer for automatic speech recognition.            eit

Introduction

Automatic speech recognition (ASR) consists of transcribing audio speech segments into text. ASR can
be treated as a sequence-to-sequence problem, where the audio can be represented as a sequence
of feature vectors and the text as a sequence of characters, words, or subword tokens.

For this demonstration, we will use the LiSpeech dataset from the LibriVox project. It consists of short
audio clips of a single speaker reading passages from 7 non-fiction books. Our model will be similar
to the original Transformer (both encoder and decoder) as proposed in the paper, "Attention is All
You Need".

oy

mw 실습 : Time series classification with a Transformer
© Dataset : FordA Dataset, 36017H9 training, 1320개의 test data
@ 모터 센서에 의해 포착된 엔진 ASO] 측정값
2
@ SH: 엔진에 특정 문제가 있는지 감지하기

3. def transformer_encoder{inputs, 1620 5120, num_heads, ff_dim, dropout= :
2      # Attention and Normelization                                ote
3      x = layers.MultiHeadAttention(                                       ㅣ

4       key_dim=head_size, num_heads=num_heads, dropout=dropout === _, 4.                      4
5     }{inputs, inputs}                                         q

6      x = layers.Dropout (dropout) (x)                                -2   을
7      x = layers.LayerNormalization(epsilon=te-6)}(x)                      1
      res = x + inputs                                ㆍ            0    100   200   300   400   90
3     # feed Forward Part                                            |

18     x = layers.Convib(filters=ff_dim, kernel_size=1, activation="relu”)}(res).

11      x = layers. Dropout (dropout) (x)                           =

12      x = layers.conviD(filters=inputs.shape/-1}, kernel_size=1)}(x)}

13      x = layers.LayerNormalization(epsilon=ie-6) {x}

a4      return x + res
1 def build _model( input_shape, head_size, num_heads, ff_dim, num_transformer_blocks,
2     mip units,   dropout=¢, mip _dropout=e, ):
a      inputs = keras.Input(shape=input_shape)

4      x = inputs
S      for _ in range(num_transformer_blocks)}:

6        x = transformer_encoder{x, head_size, num_heads, ff_dim, dropout)
7      x = layers.GlobalAveragePool ingiD(data_format="channels first”){x)
g      for dim in mlp_units:

g         x = layers.Dense(dim, activation="relu")(x)

ie          x = layers.Dropout{mip_dropout)(x}

it     outputs = layers.Dense({n_classes, activation="softmax™ } {x}

gots     return keras.Model(inputs, outputs)
93

한국시연구소 홍근선                    -268- 무단 전재, 복제, S4ll, 디지털화 금지



===== PAGE 269 =====
4부. Attention Based Model

Chapter 4. Attention Based Model

4.1 Word Embedding

4.2 Attention Mechanism

4.3 Self-Attention

4.4 Transformer

4.5 GPT: Generative Pre-trained Transformer

x ChatGPT vs. Al
@ ChatGPT& 시작된 시의 새로운 흐름 : 시에 대한 관심이 같이 상승

8 주요 LLM 성능 비교 (23.11)

를 ChatGPT + chatgpt + open ai...            @ 시 + artificial Intelligence

https:  reddit,com/r/LocalLLaMA/commen  fho9    Im_comparisontes
models_tested_7b70b/

@ GPT4 > GPT3.5 = 70B models > others       Models tested:
@ Sparse MoE(Mixture of Experts) 기법

/ 분야별로 학습된 LLM 모델을 결합하여                    oe
큰 모델 구성 > 추론에서 일부만 활성화                      ee
4 단일모델은 효율이 떨어짐(학습,추론)                   11 706
@ GPT4E 16개의 모델을 결합하여(406) 구성            * GPT-3.5 Turbo + Instruct (175B)
/ 추론 시 2개 모델을 선택적으로 사용(추정)                apn

___. Sparse MoE vs. Dense MoE(Ensemble)                                 BEEP LEARNIN
oe       —                   -         pS MS alta

@한국시연구소 홍근선                     -269- 무단 전재, 복제, etl], 디지털화 금지



===== PAGE 270 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

내 그르 vs.   9091 vs, GPT

w 비교                                        -Pre-trained
:    — model
situ      《
oe       Decoder           =      _—
BERT     2018   Encoder    0    개  Self-supervised
2018  066006「    o- ay

@ Transformer 계열의 단점
@ 56046066로 묶어야만 됨, 순서에 기반(6051400-60ㅁㅇ00109)하여 중요도가 결정됨
ㅎ 56046066길이 0, embedding 0일때                    Transformer

@ SU&e O(n’ +d)                      ee a        =
> 길어질수록 너무 복잡해짐
© 유추편향(100401146 bias) 부족
@ 회귀모델은 FAA 패턴에 유추편향 임
유추(귀납)편향이 0312의 SAS 일반화
더 YE dataset 필요

_ Output GPT

539          ™       esas                      —.         som             EX DEER LEARNING

Xf Transformer vs. BERT vs. GPT

= BERT(Bidirectional Encoder Representations from Transformers)
® Transformer2| EncoderGt 사용            Encoder
두 가지 모델의 크기

Layers
® BERT base model: 110M            pee
:                networks      768       1024       512
® BERT large model : 340M                 eae           Ie badd cg vector size
® 다양한 downstream task 적용 가능       _        :         -          3
® Single sentence classification.          —
®@ Sentence Pair Classification            [ow | fe | | 6] | |] fw |e
® Question Answering              t   테제 제   t ;
@ Single sentence tagging                ai     t      수      t     수
|] | % |    |“ | |“ 」
000:                   (3     (때
Transformer Model

Base : 12x
Large: 24x

540_                   t     | [ower] ㅣ |

=
-   | |           ac
@한국시연구소 S24               - 270 - 무단 전재, 복제, S4ll, 디지털화 금지



===== PAGE 271 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

= BERT Training
© Training
ㅎㅎ max 512 sequences(tokens), 1 million steps
® Wikipedia(~2.5B word), Books Corpus(~0.8B word)

@ Task 1: 15%의 단어를 maskingdtal(mask language model), 양방향에서 예측

@ Task 2: 주어진 문장, 다음에 S 문장 예측

# Sentence 분리                                              The man went tothe fgg] to 자 of milk.
문장 내에서 분리를 위해
Segment Embedding 사용                                                store             gallon

Sentence A The man went to the store.         Sentence A The man went to the store.

,      88 He bought a galion of milk.      "Sentence B Penguins are flightless.

or

mm
»

an)

541                                                      Sot DEEP LEARNING”

m BERT 파생 모델들 :

그밖에 ALBERT, ELECTRA, 502008타1,…

BERT                         RoBERTa                   DistilIBERT                XLNet
Size (millions)       Base: 110                Base: 110                Base: 66                 Base: “110
Large: 340                 Large: 340                                             Large: ~340
Training Time         Base: 8 x V100 x 12        Large: 1024 x V100x1 | Base: 8x V100 «3.5       Large: 512 TPU Chips x
days*                         day; 4-5 times more       days; 4 times less than | 2.5 days; 5 times more
Large: 64 TPU Chips x 4 | than BERT.                  BERT.                         than BERT.
days (or 280 x V100 x1
days*)
Performance          Outperforms state-of- | 2-20% improvement      3% degradation fram | 2-15% improvement
the-art in Oct 2018        over BERT                   BERT                         over BERT
Data                           16 GB BERT data             160 GB (16 GB BERT        16 GB BERT data.           Base: 16 GB BERT data
(Books Corpus +           data + 144 GB              3.3 Billion words.          Large: 113 GB (16 GB
Wikipedia).                   additional)                                                    BERT data + 97 GB
3.3 Billion words.                                                                        additional).
33 Billion words.
Method                     BERT (Bidirectional         BERT without NSP**       BERT Distillation             Bidirectional
Transformer with MLM |                                                                Transformer with
and NSP)                                                                                           Permutation based
modeling

oP! DEEP

_ Permutation based: 단어들을 무작위로 섞은후,
542                                                           모델이 이 순서를 복원하도록 학습
@한국시연구소  =                 -271- Sat aa}, 복제, 빌

P|, 디지털화 금지



===== PAGE 272 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

1 Generative Pre-trained Transformer, GPT
= Transformer 구조에서 Decoder 부분만 사용
서다 PE           3

- 양방향 Transformer Encoder

- 단방향 Transformer Decoder
Architecture      : 으으으                    - 텍스트를 왼쪽에서 오른쪽으로 처리
단어 주변의 이해를 포착              - 다음 단어를 예측, 단어의 왼쪽에 대한 이해가 제한 됨
- Bidirectional Understanding                    - Unidirectional Understanding
- MLM(masked language model) 사용. |- CLM(causal language model) 사용
Training = |- SS] 임의의 단어는 85009                   - 문맥의 순차적 특성을 이해
Objective  |-주변 문맥을 기반으로 단어를 예측     - 일관되고 문맥에 맞는 HACE 생성하도록 학습

- 문장 내에서 단어 Zt 관계를 이해하도록 학습|- 단어의 왼쪽에서만 문맥을 이해
- 문장 구조와 의미에 대한 포괄적인 이해           - 문장 내에서 관계를 완전히 파악하는 SHO] 제한
- 사전 학습된 모델 위에 taskS 계층을 추가 |- HAS 생성 및 번역과 같은 특정 작업에 맞게

Fine-tuning

- 다양한 특정 NLP 작업에 맞게 fine tuning |- SAS 특정 작업에 맞게 fine tuning

- 문장 및 토큰 수준 분류 작업에 매우 능숙
- 문장 생성에 특화

Use Cases |” haat eta ae        (BERTHS 인코더 모델은 텍스트를 생성할 수 없음)
- 텐스트         버       과 같은
few-shot prompti!ct 종정 선호됨             텍스트 생성, 번역 등과 같은 작업에 적합
Real-World |- Google 검색에서 검색어의 맥락을 파악       - ChatBot, 콘텐츠 제작 SS 다양한 응용에서

= Example _ |-검색결과의 관련성과 정확성을 높이게 됨 __ _|-인간과 유사한 텍스트 응답을 생성하게 될 . .

x Generative Pre-trained Transformer, GPT
@ GPT 1,2,3,4 기본 구조, 모델 크기

Transformer Biock (0090

(— a |)

100T

10

10000
ra                        fare              aw
호                  6758 sg
한                           7    o
은 100                     0.
i=
GPT1: 12                                                               g       ‘a      li        iv
GPT2: 48                                                                                       은           rae      Turing NLG
GPT3: 96                                                                               =                     ~       (17.28)
GPT4: 120                                                           5                  Ps
=                  £ 030
2                 -
들               ? . 9법골
g                    (1.58)
a
Positional                                                         3                   BERT-Large
Encoding                                                         3                    (340M)
2020     2021     2022     2023 2024

@한국시연구소 홍근선                  - 272 - 무단 전재, 복제, Sal, 디지털화 금지

544         ’    we                                       체이 input



===== PAGE 273 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

= GPT Series 비교: ChatGPTE GPT3& fine tuning

Decoder                                    utput
GPT1 18,06 ‘2layer 117M 5k          Shove 바투
GPT2 ‘19,02 48 layer        1.5B            1k           €                      Fine-tuning#2t5|0o] 범용성 증가
'                                                                                                      파라미터 100배 이상 증대
GPT3 ‘20,06 96layer      175B       2k,4k       <           사람수준 글쓰기, 코딩, 번역, 요약 등 수행 가능
GPT3.5 '22.12 96layer 1758- 46166  €                   보다 saa sa og ae
-                 .                    .                    .                                          GPT 3.5 기반, ChatBot2& fine tuning
Chachi                                                               :            대화 형태로 상호작용, 인간과 대화하는 것과 유사
,               16x                                                                     창의적이고, 기술적인 글쓰기
GPT4 ‘23,03    120layer       1,8T        8k,32k        <                               Image 입출력
GPT-4 _.,                                 :
a 2311                                         128k          4k                                   + 음성 입출력
ANGPT 이용자확보 기간현활

30660안사용자착토:

eo

에어비멘티

@ GPT-3 vs GPT-3.5 vs ChatGPT vs GPT-4
© GPT-3

@ 175Billion(1750%) parameters

@ 대규모 언어 2S(LLM:; Large Language Model)2] 시작
@ GPT-3.5

® GPT-3 Fine tuning (Human Feedback RL 적용)
@ ChatGPT(3.5)

@ GPT-3.5 Fine tuning (ChatBot 2& Tuning)

@ 미국 변호사 시험에서 하위 10%의 성적

ㅎ SAT 읽기 및 쓰기 800점 만점 기준 670점

ㅎ 547 수학 능력 590점                           [ 신경 세포의 변화 ㅣ]

© GPT-4                                   |     Voy WW
@ 1.8 trillion(1.8%) parameters              W VY
45   17    19     21

@ 미국 변호사 시험에서 상위 10%의 성적

@ SAT 읽기 및 쓰기 710점
® SAT 수학 능력 700점                x  '     !
@ 의학지식 자가 진단 정답 를 75%
40 urd

546                       scmmaiagnucaiai         si     :          :      St DEEP LEARNING”
@한국시연구소 S24                  -273- 무단 전재, 복제, Ball, 디지털화 금지



===== PAGE 274 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer
ㅣ     :                               ‘

¥t GPT-32] 특별함
w 기존의 ＬＬ\/은(2단계 처리가 필수)
1) 대규모 031856[으로 사전학습 후: 언어 체계를 학습
2) 해결하려는 문제에 Fine Tuning : 문제 해결법 학습
@ 정답이 포함된 031356필요, 일반화 능력이 소실됨
3) 일반적 문제에 대응 능력이 매우 제한적
를 6『1-3의 접근
© 모델 키우기 + In Context Learning ® Fine 1411100없이 다양한 문제 해결해 보자!

Zero-shot       One-shot                        자아
       :            |      -               GPT-3
wn 17568
Naiural Language                                     oid                    ‘arams
60                    Prompt                     0 ~
a              _—— sf oe                                               _
z                         A              a                                                                               *성능개선*
은               J                 \
8 30        fe a Proengt                                                       ㆍ 더 Be Contexts 제공받
"     이                                                   ：       =< 138 Params            s  Az

GPT-2
seem 1.368 Params
10"

Number of Examples in Context (K)

547,

r
mGPT-3 : Fine Tuning Qo] 다양한 SAS 해결 할 수 USS 확인
@ 인터넷, 책, 백과사전 데이터로 학습
® Common Crawl: 다양한 도메인, 언어와 주제 (93%영문,7%기타 AS)
@ WebText: 문서 품질에 SAS 두고 웹페이지 스크랩하여 만든 내부 자료
/ Raddit 등
® Books1 & 8001652: 고전문학, 현대문학, 과학, 역사 SS

Quantity       Weight in       Epochs elapsed when

Dataset                           (tokens) training mix training for 300B tokens
ANLI Round3 Common Crawl (filtered) 410 billion          60%                        0.44
Fine-tuned SOTA WebText2                              19 billion            22%                           2.9
4                                                                        Books!                                 12 billion            8%                            19
46                                                         Books2                          55 billion          8%                     0.43
Fine-tuned ROBERTa-Large            Wikipedia    =      3 billion     3%           3.4
44 Fine-tuned BERT-Large
대 42 ne Zero-Shot
5 gg TP One-Shot                                               4
8    ~ Few-Shot (K=50)                          ^
36                   A
|          ae      Bs                                       -
& 어등                   어떠
32         나                             .
6.18     64B 088 138 268    67B 138                 1758
Parameters in LM (Billions)
etna            =                      :              .           내                  이 DEEP LEARNING”

한국씨연구소 홍근선                     -274- 무단 전재, 복제, 발춰, 디지털화 금지



===== PAGE 275 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer
4.5 GPT: Generative Pre-trained Transformer

mChatGPT: 6『1-3.5이후의 2S! ChattingOl Fine Tuning
® GPT-32| 한계
@ 다음 단어를 예측하는 데 SAS = 대규모 데이터를 기반으로 학습됨
/* 매우 정교하게 [3[[된 프롬프트에 대해 놀라운 SHS 생성할 수 있지만,
* 생성된 출력이 거짓일 가능성이 있고
 유해한 내용을 포함할 수 있음
® 강화학습(나 『: Reinforcement Learning with Human 『600630)적용
@ 인간이 작성한 설명과 인간이 판단한 아웃풋의 랭킹을 모델에 반영
A AZ| 선호도를 보상 신호로 사용
/* 모델을 미세 2A (fine-tuning)
> 대화 모델의 목표: 안전과 사용자의 의도, 가치와 일치 하는지를 반영
> 일상적인 [1080 1으로 사용 가능

_4.5 GPT: Generative

% GPT-4 개요 (대규모 멀티모달 생성모델)
8 Training dataset : 13조 Token, program code, images, YouTube,-:-
@ Input Token: 25,000 € 3,000
= Model
@ 120 layer < 96 layer
 1.8T Parameters < 175B
© MoE(Mixture of Experts): 16742] Expert@2lgs 결합
a 단어 추론
$16개 중 2개의 Expert]! 활성화
 280B parameter
@ 560TFLOPs 연산으로
(뇌: 수천나[0[669)
a 비용
© 훈련 : $6,300만
@+ 시스템 구축

ㅎ 5$1억 ~ 추정

550

@한국시연구소

00

근선                    -275- 무단 전재, 복제, Wal, 디지털화 금지


===== PAGE 276 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

mw GPT-4 특징
@ 이미지, HAE 입력 텍스트 출력을 생성
@ 이미지 형태로 제시된 시험 문제와 HSS 이해
@ 인터넷 BY 이미지의 유머 포인트를 이해
@ 변호사시험과 미국 생물올림피아드에서 각각 백분위 90%, 99% 달성
@ MMLU 테스트에서 인간 전문가 평균 89.8에 가까운 86.4점에 도달
/* 각 분야 전문가만큼 SS 이해하고 쓸 수 있음
$#강화된 안전 필터                                       What is funny about this image? Deseribe it panel si ome
@ 시 보정, 사이버보안, 의학, 사회 안전 등                   7              o~
전문가 50명과 만든 안전필터 적용

si  aon  nnn

를 (01 : “Chain-of-Thought Prompting Elicits Reasoning in Large Language Models”,2023

®@ Chain-of-Thought Prompting: <input, chain of thought, output>
/ 결과 생성에 중간 과정을 같이 AWAS-== in-context few-shot learning 제시
- 중간 과정 : 문제 푸는 과정을 단계별로 분해해 추론하도록 유도
 모델의 출력 결과에 대해 해석가능성을 부여하여, 오류를 찾기 AAA
* 사람이 해결하고자 하는 대부분의 태스크에 적용 가능

/* 관련된 YH (relevant knowledge)S 더 많이 줬기 때문인가 ?                        [ Symbollc Reasoning task ]
- CoT prompt answer 이후에 넣으면 성능이 좋아지지 않음                                 —+— Standard prompting
산술, 상식, 기호 42 (symbolic reasoning) HA 두드러진 성능 향상          tr ialacabdong es prompting
복잡한 문제에서 성능이 좋음, 쉬운 문제에는 성능이 별로임                        Letter Concat: 2 Letter Concat: 4
(in domain)             (OOD)
ㅎ Reasoning(#=): 알고 있는 지식에서 새로운 지식(결론)을 이끌어 내는 과정        100          _®
Standard Prompting                             oe -Thought Prompting            R75       Pa                          a
|   Q: Roger has 5 tennis bails. He buys 2 more cans of ㅣ Q: Roger has 5 tennis balls. He buys 2 more cans of       ES 25  af                                  A
tennis balis. Each can has 3 tennis balls. How many    |     tennis balls. Each can has 3 tennis balls. How many       &   "10                           8
tennis balis does he have now?                              || tennis balls does he have now?                                      0   gee enn2       ee

A: The answer is 11.                                                                                                               Coin Flip: 2       Coin Flip: 4

|
|
|
|
|
|
|
|

Q: The cafeteria had 23 apples. If they used 20 to                                                                                                  & domain)             (OOD)
| make lunch and bought 6 more, how many appies            Q: The cafeteria had 23 appies. 11 they used 20 to          100}        2
| do they have?                                              || make lunch and bought 6 more, how many appies        =   Py ^                          2
\                                                                               / | do they have?                                                             380}     ge                                 「
nN                                                                               | x                              gf
ee                                                                          ~                                                                              BS |                                             Ed
| A: The answer is 27.  x                                        || A: Eee          ia had 23 3                                                 40 [                                      ~

8 62 540 8 62 540
Model scale (# parameters in billions)

%                * Inference : Reasoning 과정 또는 행위 ANS 지칭         :           ‘           Sof DEEP LEARNING”
@한국시연구소 홍근선                   -276- 무단 전재, 복제, Wall, 디지털화 금지

\_answeris 8



===== PAGE 277 =====
4부. Attention Based Model

4.5 6

PT: Generative Pre-trained Transformer

5 GPT:

@ 대규모 강화 학습 알고리즘

@ OpenAi 01 (Sept. 12, 2024): https://openai.com/index/learning-to-reason-with-llms/

& 11810109 프로세스에서 일련의 사고 SAl(CoT)S 사용하여 생산적으로 생각하는 방법을 모델에 가르침

이
preview

ot
preview

@ 더 많은 강화 HS (train timex} 더 많은 생각 시간((65【 time)oll 따라 성능이 지속적으로 향상됨
@ 물리학, 생물학 벤치마크에서 인간 박사 학위 수준의 정확도를 능가(논리적 처리의 약점을 보완)
기 000     Sanco om SUNOS 자격 시
a9          |                   as                                       = 641 AHS 81 OW 83%
80                       ee                                                                                           PQA(   ete, 화학 및 생물학 전문
일                                    i                                                                                     "aN 수준 BBN 수준을능가
§ 40                            i                                                                 ‘*+MMLU(Multi-Task Language
0                                                                                                              : 시각적 S801 활성화되면 78.2%의
만                                                                                       - 최초로 인간 전문가와 경쟁가능

**Codeforces: 프로그래밍 대회

oT AIME accuracy                                                   01 AIME accuracy
during training                                    at test time
100                                                                       100
80                                                                         60
>                                                                  ㆍ      3
s   60                                                                   5 60                                            ㆍ
더
i           j
ㆍ
20                                                                         rote
0                                                                          0

train-time compute (log scale)                                     test-time compute (log scale)

A? DEEP LEARNING |
tLe eee eee ee

@ OpenAi 01 추론 절차

® 『62500109에서 CoT(chain of thought,A-ZALKS) Aled : 단계적 추론에 특히 적합

* Thinking token : 생각, 절차, 생성, 분석, 다른 접근방식 검토
~ Prom         만 사용하여 3회 심
ee   chisel ao     PUN                    @;  aden {o1)
RLHF      Inference
RLHF       + CoT     + CoT
4                                                    ~     ™,    ya
ng    oe                                | Prompt |     Prompt
Input                      개.    \
…      나      |
| 00000 ]      Mines

ㅎ 01 : 문제의 단계를 식별하고, 단계별 해결
 문제를 단계별로 분해하고,
f 다양한 전략을 시도하고,
& 실수를 수정하는 과정과 유사 하게
"답하기 전에 깊이/다양하게 생각하고
점차적으로 다듬도록 학습

Reward
Model

554           _ (강화학습을 통해 생각하는 방법을 배움)

@한국시연구소 홍근선

-277-

무단 전            tai), 디지털화 금지

=

Al, 복제, 2


===== PAGE 278 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

_4.5 GPT: Generative Pre-trained Transformer

@A MM @ 6   OQ G

Price                        te.              :                          Context Window

555

4.5 6

Ss

@ OpenAi 01 code 생성

ㅎ Prompt: WGAN-GP= =O] 있는 874 또는 25개의 Gaussian 분포의 데이터를 생성하고, 시각화하는
python codeS 생성해줘.

@ vz 동안 생기 ~                                                           8 Gaussians 25 Gaussians
Gaussian 분  데이터                   ft  a   “           gee  s  scares  별,

___ 8 Gaussians  —               25 Gaussians
|    a       210 ¢€ w@ @ |
"                          |
1 *    *    1% © @ & &|
of        @    le 0 @ & ®
그 | aie @ & @ @|
|     를 ㅣ                |
2     ®    | 2{¢ 0 © © |
-2    9    2      -2  -1  0  z  2
556                                                                RE DEEP LEARNING

@한국시연구소 홍근선                   -278- 무단 전재, 복제, Sal, 디지털화 금지


===== PAGE 279 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer
_4.5 GPT: Generative Pre-trained Transformer _

8 OpenAi 03(21.12, 2024): https://Awww,datacamp.com/blog/o3-openai

®  at AGI Prize https://arcprize.org/blog/oai-03-pub-breakthrough
@ 인간에게는 쉽고(95%이상), 시에게는 어려운 SAS 제시 -> 차이가 없어지면 AGi= 보자
@ 대부분 시 벤치마크는 기술을 측정
* ASS 지능이 아님
* AGE 새로운 기술을 효율적으로 습득하는 능력이라고 생각함(유동적 지능)
@ 유동적 지능을 확인하기 위해
 즉석에서 새로운 기술을 습득할 수 있는지 즉, 새로운 he 대한 ASSIS 측정하기 위해
/* 특별히 고안된 문제 들로 구성하여, =e 학습된 patternS 출력하는 것으로 답할 수 없도록 함
* LLMO| 단순히 수백만 개의 mini programS 호출하는 것이 아님을 증명해야 St
@ 인간에게는 쉬운 일이지만, 시에게는 어려운 일을 지속적으로 개발
object contact                             gravity

symmetry, occlusion                        jumping

pathfinding

te aa                   Soe DEEP LEARNING

® ARC AGI Prize
@ 인간에게는 쉬운 일이지만, 시에게는 어려운 일
ㅎ 아직 풀지 못한 문제의 예

Example 1:

J

SSS ER OS Ce Oe

Seoew
=,

[ㅋㅋ
yy
아

Seo eo owe oOOrwO OG 다
BOM UVMSOPVUMNUN YS SC SM @ SS S et

SS Vs We de ce Ut Ut Gh a ++
De SSO DWH OOS ~
~ OS OH SS OS
MOOK eevtounw
SOreoeoocouuv
SQerHeSSTSHSS
Y OOOO O89 @

558                                               :                              vet           30. DEEP LEARNING

@한국시연구        a                  -279- 무단 전재, 복제, SH, 디지털화 금지

[『
00
i


===== PAGE 280 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer

@ GPT-3(2020.6):0% > GPT-40(2024.5):5% > 03(2024.12):87.5%

GO SERIES PERFORMANCE / ARC-AGI SEMI-PRIVATE EVAL

10                                @ Siew GRAD
88%
O3 HIGH (TUNED) @
76%
75% $ A¥E. MIVRKER       @.03 LOW ATUNED).
@ KAGGLE SOTA
=
§ 9%
a
219 32%
256
13.33%
780%        @O1 PREVIEW
@ O1-MINI
o%
$10                   $10.0                   $100.0                  $1,000.0

COST PER TASK

SESE TERNS

Pre-trained Tr: nsformer_

w Al Agent: 목표를 지정하면 세부 목표와 행동 계획을 수립하고 행동, 작업 자동화가 목표
@ Agent GPT, Auto GPT= Al Agent2| 형태

® Agent GPT
@ 질문에서 SHS 생성하고,
@ 목표 달성을 위해 작업과 할 일 SSS 생성하고(이를 위해 A= prompt 생성),
 각 과정을 수행하여 결과 제공
 인간과 유사한 계획과 실행
@ Al ^9601에 대한 쉬운 ALS 보장
© Auto GPT : 자동화된 콘텐츠 생성, 정보 제공 또는 간단한 질의
 설정한 SHU 요구사항을 기반으로 all 작업을 수행
 사용자의 입력에 따라 자동으로 반응하.
 사전에 정의된 작업을 수행 St
& 주로 반복적이거나 표준화된 작업에 사용
ㅎ 작업의 세부적인 설정이나 조정을 사용자가 직접 제공 해야 St
/* 특정 스크립트나 시나리오에 따라 작업을 수행
@ 사용자의 입력을 받아 해당 스크립트에 맞게 응답

olo

답 등, 정적인 작업이 대상

25 ann        —    Qa» BEEP LEARNING
@한국시연구소 S24          -280- 무 단 전재, 복제, wall 디지털화 금지



===== PAGE 281 =====
4부. Attention Based Model        4.5 GPT: Generative Pre-trained Transformer
ed Trans:

® LLM Powered Autonomous Agents https://lilianweng. github jo/posts/2023-06-23-agent/
@ Planning
@ 하위 목표 및 분해: 대규모 AAS 더 작고 관리 가능한 하위 SHS 나누어 작업을 효율적으로 처리
 반성 및 개선: 과거 행동에 대한 자기비판 및 반성, 실수로부터 학습, 최종 결과의 품질 향상

@ Memory
+ 단기 7/4: in-context learning2 모델의 단기 기억을 활용하여 학습하는 것으로 간주 됨
* 장기 기억: 외부 벡터 저장소와 빠른 검색을 aia 장기간에 걸쳐 (무한) ALS 유지
® Tool use

@ 최신 정보, 코드 실행, DBMS S, 학습되지 않은 정보(사전 학습 후 변경하기 어려운 경우가 많음)를
획득하기 위해 외부 APIS 호출하는 방법을 학습

[ LLM-powered autonomous agent system ]

| Short-term memory | Long-term memory |

| Calendar() +                 7 ro

Calculator {)

@ 4.1 Attention Mechanism
@ Seq2Seq2| 문제점과 Attention 기본 동작
® Bahdanau, Luong Attention 및 일반화 모델
®@ “Show, attend and tell’ : CNN + LSTM + Attention model

® 4.2 Self-Attention
@ Self-Attention 개념과 동작
® Self-Attention 실습 ( LSTM + Self-Att. Stacked Self_Att. )
@ 4,3 Transformer
® Architecture Overview
@ Scaled dot-product Attention
@ Multi-Head Attention
® Enc.-Dec. Cross-Attention
© 4,5 GPT: Generative Pre-trained Transformer
® Transformer vs. BERT vs. GPT
ㅎ Generative Pre-trained Transformer, GPT
@ Al Agent

SBS DEER LEARNING”

@한국시연구소 Sa   선              -281- 무단 전재, 복제, Za, 디지털화 금지



===== PAGE 282 =====
RNNit 시계열처리 심화 |

SAMSUNG

